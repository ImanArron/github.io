# iOS 包大小二进制优化

优化思路：移动 iOS 可执行文件中的的 `__TEXT` **段** 中的部分 **节** 到其它 **段** 中，提高可执行文件的 **压缩效率**，从而减少 APP 下载大小。

# 技术原理

## Mach-O 文件格式

iOS 可执行文件是 Mach-O 格式，主要由 `Header`、 `Load Commands`、 `Data` 三部分组成：

* `Header` 描述文件的大概信息
* `Load Commands` 由多条 `Load Command` 组成，描述 `Data` 在二进制文件中的布局信息，可知道 `Data` 在二进制文件中和虚拟内存中如何排布，相当于修房子时的图纸
* `Data` 存储实际内容，主要是程序指令和数据，根据 `Load Commands` 的描述排布，以 Segment(段) 和 Section(节) 的方式组织内容

`Data` 中有 5 个 Segment：

* `__PAGEZERO`
* `__TEXT`
* `__DATA_CONST`
* `__DATA`
* `__LINKEDIT`

除 `__PAGEZERO` 和 `__LINKEDIT` 外，每个段中都有多个 `Section`。

`__PAGEZERO` 不可读不可写，用来捕捉 NULL 指针的引用，若访问 `__PAGEZERO` 段，会引起 `EXC_BAD_ACCESS` 错误。

`__TEXT`、`__DATA_CONST`、`__DATA` 用于保存程序的代码指令和数据。

`__LINKEDIT` 包含启动 APP 需要的信息，如 bind & rebase 的地址，代码签名、符号表等。

## __TEXT 段迁移原理

程序构建主要包含 `预处理` -> `编译` -> `汇编` -> `链接`，四个阶段，完成之后可生成 Mach-O 可执行文件。

通过 `$ man ld`，可发现链接器有一个参数：`-rename_section orgSegment orgSection newSegment newSection`，使用该参数可将 `orgSegment/orgSection` 修改为 `newSegment/newSection`。可在 `Other Linker Flags` 中传递该参数：

```
-Wl,-rename_section,__TEXT,__text,__GT_TEXT,__text
-Wl,-segprot,__GT_TEXT,rx,rx
```

`-Wl` 告诉 Xcode 它后面的参数是添加给 `Ld` 链接器的，参数将在链接阶段生效。

在最低支持 iOS 8 的时代，很多大型 App 都遇到过可执行文件中 __TEXT 段超 60 MB 的问题。facebook 当时采用了 -rename_section 的技术来避免该问题。他们使用的链接参数为：

```
-Wl,-rename_section,__TEXT,__cstring,__RODATA,__cstring
-Wl,-rename_section,__TEXT,__gcc_except_tab,__RODATA,__gcc_except_tab
-Wl,-rename_section,__TEXT,__const,__RODATA,__const
-Wl,-rename_section,__TEXT,__objc_methname,__RODATA,__objc_methname
-Wl,-rename_section,__TEXT,__objc_classname,__RODATA,__objc_classname
-Wl,-rename_section,__TEXT,__objc_methtype,__RODATA,__objc_methtype
```

## 下载大小减少的原理

可以认为苹果只会对 Mach-O 文件中的 `__TEXT` 段加密，而不会对其它段加密。只要能把 `__TEXT` 段中的节移到其它段，就能减少苹果的加密范围，从而使压缩效率提升，减小下载大小。这也解答上个小节提出的问题。

一般来讲，在 App 中可执行文件占 80% 的大小，而加密部分占可执行文件中的 70%，加密会影响 60% 的压缩率，因此移走该加密部分，会提升 34% 的下载大小。根据我们在多个 App 的实践，本方案可以减少 32~34% 的下载大小。

