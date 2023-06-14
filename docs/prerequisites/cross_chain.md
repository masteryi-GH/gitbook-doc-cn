Cosmos是一个去中心化的跨链生态系统，其跨链原理是通过**IBC**（Inter-Blockchain Communication）协议实现的。IBC协议是一种通用的跨链协议，它允许不同的区块链之间进行安全、可靠和高效的通信和交互。

在Cosmos生态系统中，每个区块链都是一个独立的主权状态机，可以自主地定义其规则和状态转换。这些区块链可以通过IBC协议相互通信和交互，从而形成一个跨链生态系统。具体来说，**当两个区块链需要进行跨链交互时，它们之间会建立一个IBC通道，通过这个通道进行数据传输和验证**。

IBC协议的核心是一组标准化的接口和协议规范，包括通道建立、数据传输、状态确认和安全性保证等方面。这些接口和规范可以让不同的区块链之间进行跨链通信和交互，同时保证安全性和可靠性。

接下来以交易对跨链交易为例介绍整个生命周期：

设你有两个区块链： `Mars`和`Venus`， `Mars`的原生代币是`marscoin`,`Venus`链的原生代币是`venuscoin` 。

在本例中，来自 `Mars`链的用户出售`marscoin`币。 `Venus`链的用户购买`marscoin`币。 `Mars`链我们称之为源链， `Venus`链为目标链。

IBC Packet跨链消息的生命周期，在传输期间，数据包会经历下面几个阶段

- 源链上传输前的消息处理
- 目标链上接收数据包
- 源链上确认数据包
- 源链上的数据包超时

![](/Users/Myron/Myfile/agg-chain/gitbook-doc-cn/images/v2-d637531c9631ab83ae3d34c2189163b1_1440w.png)