### HTTP 协议

HTTP 是计算机世界里专门在 **两点** 之间传输文字、图片、视频等 **超文本** 数据的 **约定和规范**

### HTTP 常见字段

* Host
* Content-Length
* Connection
* Content-Type
* Accept
* Content-Encoding
* Accept-Encoding

GET - 只读，安全且幂等

POST - 不安全、不幂等

### HTTP 优缺点

HTTP 优点：简单、灵活和易于扩展、应用广泛、跨平台

HTTP 缺点：无状态(于是诞生了 Cookie 用来解决状态问题)、不安全(于是诞生了 HTTPS)

HTTP/1.1 - 长连接、管道网络传输，由于是 请求-应答 模式，服务器按队列顺序给客户端返回请求，会产生 **队头阻塞**

### HTTP 明文传输会产生的风险

* 窃听风险 - HTTPS 对交互信息加密，混合加密(对称和非对称混合)
* 篡改风险 - HTTPS 校验机制(摘要算法)，篡改后就无法正常显示
* 冒充风险 - HTTPS 身份证书(服务器公钥)，证明服务器是真的服务器(比如，淘宝网是真的淘宝网)

### HTTPS 与 HTTP 区别

* HTTP 明文传输，HTTPS 在 HTTP 和 TCP 之间加入 SSL/TLS，加密传输
* HTTP 连接简单，TCP 三次握手后即可进行 HTTP 报文传输，HTTPS 在 TCP 三次握手之后，还需进行 SSL/TLS 握手，然后才可进行加密传输
* HTTP 端口号是 80，HTTPS 端口号是 443
* HTTPS 需要向 CA 申请证书，以保证服务器的身份可信

### HTTP/2 相对 HTTP/1.1 的优势：
* 头部压缩，HTTP/1.1 只能压缩 Body，HTTP/2 会通过 HPACK 算法压缩头
* 二进制格式，头信息和数据体都是二进制，统称为帧：头信息帧和数据帧
* 数据流，解决 HTTP/1.1 无法指定请求优先级的问题
* 多路复用，HTTP/2 可以在一个连接中并发多个请求或相应，不用按顺序一一对应，解决 HTTP/1.1 队头阻塞的问题
* 服务器推送，HTTP/1.1 只能由客户端发起请求，服务端进行响应，而不能由服务端主动向客户端发送消息

HTTP/3 将底层传输层由 TCP 改为 UDP，基于 UDP 的 QUIC 协议可实现类似 TCP 的可靠传输

### TCP 如何实现可靠传输？

* 序列号
* 确认应答
* 重发控制
* 连接管理
* 窗口控制

### 重传机制

* 超时重传 - 定时器，超时重传时间 RTO 的值应该略大于报文往返 RTT(Round-Trip Time) 的值，每遇到一次超时重传，都将下一次超时时间间隔设为先前值的两倍
* 快速重传 - 不以时间驱动，以数据驱动，三次同样的 ACK 触发
* SACK(Selective Acknowledgment 选择性确认) - TCP 头部字段添加 SACK，将缓存地图发给发送方，发送方就可以只传丢失的数据
* D-SACK(Duplicate SACK) - 通过 SACK 告诉发送方有哪些数据被重复接收了


### 滑动窗口

窗口大小就是指：**无需等待确认应答，而可以继续发送数据的最大值**

TCP 的 `Window` 字段，是接收端告诉发送端自己还有多少缓冲区可接收数据，所以，窗口大小是由 **接收端** 的窗口大小决定。

发送方滑动窗口指针：

* `SND.WND`: 发送窗口大小(大小由接收方指定)
* `SND.UNA`: 绝对指针，指向 **已发送但未收到确认** 的第一个字节的序列号
* `SND.NXT`: 绝对指针，指向 **未发送但可发送** 范围的第一个字节的序列号
* 相对指针: `SND.UNA + SND.WND`

可用窗口大小 = SND.WND - (SND.NXT - SND.UNA)

接收方滑动窗口指针：

* `RCV.WND`: 接收窗口的大小，会通告给发送方
* `RCV.NXT`: 指向 **期望从发送方发送来** 的下一个数据字节的序号
* 相对指针：`RCV.WND + RCV.NXT`

### 流量控制

流量控制：**让 发送方 根据 接收方 的实际接收能力控制发送的数据量**

TCP 规定：**不允许同时减少缓存又收缩窗口**，而是先收缩窗口，过段时间再减少缓存，以避免丢包情况

窗口关闭：**窗口大小为 0 时，会阻止发送方给接收方发送数据，知道窗口变为非 0**

解决窗口关闭潜在死锁问题：只要收到零窗口通知，就启动持续计时器，计时器超时时，发送 **窗口探测报文**

糊涂窗口综合症：发送方不停发送几个字节的小数据(联想到可以坐 50 人的大巴车，但是每次只坐两三个人就上路)

解决糊涂窗口综合症：

* 让接收方不通告小窗口给发送方 - 窗口大小 < min(MSS, 缓存大小/2) 时，向发送方通告窗口为 0
* 让发送方避免发送小数据 - Nagle 算法，1、窗口大小 >= MSS 或 数据大小 >= MSS；2、收到之前发送数据的 `ack` 回包；条件 1 和 2 满足其一才发送数据

### 拥塞控制

有了流量控制，为什么还要拥塞控制？流量控制，是为了避免 发送方 的数据填满 接收方，而拥塞控制，是为了避免 发送方 的数据填满整个网络

怎么判断网络是否出现拥塞？只要 **发生了超时重传，就会认为网络发生了拥塞**

拥塞控制算法：

* 慢启动 - 发送方每收到一个 ACK，拥塞窗口 cwnd 大小就加 1，慢启动算法，发包个数是 **指数性增长**，慢启动门限 `ssthresh`，当 `cwnd < ssthresh`，使用慢启动算法，当 `cwnd >= ssthresh`，使用拥塞避免算法
* 拥塞避免 - 发送方每收到一个 ACK，cwnd 大小增加 1/cwnd，发包个数 **线性增长**
* 拥塞发生 - 超时重传时，`ssthresh` 设为 `cwnd/2`，`cwnd` 设为 `1`，快速重传时，`cwnd = cwnd/2`，`ssthres = cwnd`
* 快速恢复 - `cwnd = ssthres + 3`，重传丢失的数据包，若再收到重复 ACK，cwnd 增加 1，若收到新数据的 ACK，说明网络已恢复，可再次进入拥塞避免状态