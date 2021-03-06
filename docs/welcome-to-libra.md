---
id: welcome-to-libra
title: 来到 Libra 世界
---

原文链接：[https://developers.libra.org/docs/welcome-to-libra](https://developers.libra.org/docs/welcome-to-libra)<br/>
译者：humyna<br/>

**欢迎来到Libra开发者网站**！ Libra的使命是为数十亿人建立一种简单的全球货币和金融基础设施。

> 世界真正需要的是一种可靠的可以实现“价值互联网”的数字货币和基础设施。能够很方便地保障你移动设备上的金融资产。不论你生活在哪里，你做什么的，或你挣多少钱，在全球范围内转移资金应该像发送短信或者分享照片一样简单经济，甚至更安全。 — [Libra 白皮书](https://libra.org/zh-CN/white-paper/)

Libra建立在一个安全可靠、可扩展的区块链上。它由储备资产来支撑并赋予其内在价值，并由独立的Libra协会(主要职责是发展 Libra 生态)来管理。

> Libra 区块链的目标是成为金融服务的坚实基础，并使用一个全新的全球性货币来满足数十亿人日常金融需求。Libra 区块链从建立初，就优先考虑扩展性、安全性、存储、吞吐量效率及未来的适应性 — [Libra 白皮书](https://libra.org/zh-CN/white-paper/)



Libra 货币建立在 Libra 区块链上。网站中Libra Core文档是一个Libra协议的开源原型 ，它为这个全新区块链提供支持。网站也提供了一个[测试网络 testnet](https://learnblockchain.cn/docs/libra/docs/reference/glossary/#testnet)用于演示。与即将推出的Libra[主网](https://learnblockchain.cn/docs/libra/docs/reference/glossary/#mainnet)不同，testnet使用的是没有实际价值的数字货币。


文档主要讨论以下三个主题：

* 如何通过将[交易](https://learnblockchain.cn/docs/libra/docs/my-first-transaction/)送到测试网testnet来对原型进行试验。
* 学习 Libra协议、Move语言，LibraBFT 等新技术
* 如何加入社区共建Libra生态

<blockquote class="block_note">
**注意**：这个项目目前处于早期原型阶段。Libra协议和Libra Core APIs不是最终版本。原型的关键任务之一就是确定正式的协议和APIs。当前，我们的关注基础架构建设和构建CLI客户端。我们的直接路线图中包含公共API和相关的库。我们欢迎开发者在testnet对软件进行相关测试，更期待开发人员使用这些API来发布应用程序。作为我们定期交流的一部分，我们将公布我们在稳定API方面的进展。
</blockquote>

## Move: 一种新的区块链编程语言

“Move”是一种新的编程语言，用于在Libra区块链上实现自定义的交易逻辑和“智能合约”。由于Libra的目标是每天服务数十亿人，因此安全是设计Move时考虑的最高优先级。

Move从过去智能合约的安全事件中总结经验，创建了一种语言，使编写符合作者意图的代码更加容易。它降低了不可预知的bugs或安全事件的风险。具体来说，Move可防止资产被复制,它使用“资源类型”约束数字资产与物理资产有相同的属性：一个资源只有单一所有者，只能被花费一次，并且新资源的创建被限制。

Move 让关键交易代码开发更容易，它能够安全地实现Libra生态的治理策略，比如Libra货币和验证节点网络的管理。我们预计为开发人员创建智能合约的能力将随时间的推移而可用。这将支持Move的演进和验证。

进一步了解参考 [开始使用Move 语言](https://learnblockchain.cn/docs/libra/docs/move-overview/) 


## Libra系统生态

Libra生态由下面几个部分组成：

* [客户端](#客户端)
* [验证器节点](#验证器节点)
* [开发者](#开发者)

### 客户端

Libra客户端：

* 是一种能够与Libra 区块链交互的软件
* 能被终端用户或者代表终端用户(如一个托管客户机)运行
* 允许用户构建，签名并将交易提交给[验证节点](reference/glossary.md#validator-node)
* 可以向Libra区块链发出查询（通过验证节点），请求交易或帐户的状态，并验证响应。

Libra Core包含一个可以将事务提交到testnet的客户端。[我的第一笔交易](my-first-transaction.md) 指导你使用Libra CLI客户端在Libra区块链上执行你的第一笔交易。


### 验证器节点  

[验证节点](reference/glossary.md#validator-node) 是Libra生态系统中的实体，它们共同决定哪些交易将被添加到Libra区块链中。 验证者使用[共识协议](reference/glossary.md#consensus-protocol)以便它们可以容忍恶意验证者的存在。 验证节点维护区块链上所有交易的历史记录。 在内部，验证节点需要保持当前状态以执行交易并计算下一个状态。我们将在交易的生命周期中了解关于验证节点的组件的更多信息。


测试网络testnet是一组公开可用的验证器节点，用于试用这个系统。你也可以使用Libra Core自行运行验证节点。


### 开发者

Libra 生态系统支持各种各样的开发者，从为Libra Core做出贡献的人到使用区块链构建应用程序的人。术语"开发者"包括所有这些组。开发者可以：

* 构建Libra客户端
* 构建与Libra客户端进行交互的应用程序
* 编写在区块链上运行的智能合约
* 为Libra区块链软件做贡献

这个网站面向开发人员。

## 参考

* [Libra 协议: 关键概念](libra-protocol.md) — 介绍Libra协议的基本概念。
* [我的第一笔交易](my-first-transaction.md)— 指导你使用Libra CLI客户端在Libra区块链上执行你的第一笔交易。
* [开始使用 Move ](move-overview.md)— 介绍新区块链编程语言Move。
* [交易的生命周期](life-of-a-transaction.md) — 介绍交易被提交和执行的底层实现
* [Libra Core 概述](libra-core-overview.md) — Libra Core 组件的概念和实现细节。
* [CLI 指南](reference/libra-cli.md) — 列出了Libra CLI客户端的命令及其用法。
* [Libra 术语表](reference/glossary.md) — 提供了一份Libra技术的快速参考。
