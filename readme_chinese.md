Rex 白皮书<br><br>
**一个兼顾去中心化的多重挂牌服务和不动产交易的应用**

●	Rex: 指平台, Rex<br>
●	REX: 指代币, REX

*译注:*<br>
* Token 代币<br>
* Tokenized 代币化<br>
* List 挂牌<br>
* Title 产权<br>
* Closing 交割，过户<br>

## 执行概要<br>
不动产，被定义为对土地、房地产或在之上的改进利益相关的人所拥有的任何东西。自公元前4500年人类首次落户美索不达米亚的古老的土地时，不动产就已经存在[3][5]。 自古以来主要有两种类型的不动产交易:

1. 数据(Data)
2. 交易(Transactions)

传统上来说，获得可靠的财产信息是困难的。 而今天，随着技术的进步，数据变得更容易确定。然而，数据却被中心化的组织控制，操纵和管理，从而导致高昂的交易和挂牌(list)费用。依赖于点对点数据分发(peer-to-peer data distribution)和区块链技术的近期发展，Rex将提供全球接入的不动产信息渠道和简化的交易流程。

Rex将首先建立一个全球多重挂牌服务(multiple listing service)，创建一个可供大家访问的数据层。 这个数据库将尽量减少挂牌费用，并最大限度地提高挂牌的曝光量。在我们的第三阶段，Rex将为用户提供创建用于销售和租赁的智能合约的功能。 优点包括节省时间，沟通和行政费用。最后，Rex将开发一种架构使得资产代币(property token)可以通过创建一个代币化的合约完成交易。

## 内容
 
**1.0 多重挂牌服务(MLS)<br>**
1.1 什么是多重挂牌服务?<br>
1.2 多重挂牌服务的进化<br>
1.3 Rex的挂牌服务概述<br>
1.4 为什么Rex从挂牌开始<br>
1.5 Rex运转的细节<br>
1.6 技术架构<br>
1.7 技术栈和未来发展方向<br><br>
**2.0 区块链<br>**
2.1	 什么是区块链?<br>
2.2	 什么是以太坊?<br>
2.3 为什么Rex建立于以太坊之上?<br>
2.4 数据分发<br> 
2.5 IPFS<br>
2.6 REX的优势<br><br>
**3.0 问题和解决方案**<br>
3.1 问题<br> 
3.2 解决方案<br><br>
**4.0 Rex的模型**<br>
4.1 模型<br>
4.2 阶段<br>
4.3 代币分配<br>
4.4 代币使用<br>
4.5 挂牌奖励<br>
4.6 验证系统<br>
4.7 支付延迟<br>
4.8 费用<br>
4.9 订阅模型<br>
4.10 代币销售<br><br>
**5.0 结论**<br><br>
**6.0 创始人履历**<br>
6.1 Stephen King<br>
6.2 Russell McLernon<br><br>
**7.0 联系方式和引用**<br>
7.1 联系方式<br>
7.2 引用<br><br>
**8.0 附录**<br>
8.1 附录 A: 不动产交易: 今天<br>
8.2 附录 B: 租赁交易<br>
8.3 附录 C: 代币化拥有权<br><br>

## **1. 多重挂牌服务(MLS)**<br>
#### 1.1 什么是多重挂牌服务?
多重挂牌服务是一套服务，使房地产经纪人能够建立合同报价（来自经纪人），促进与其他经纪人参与者的合作，并通过积累和分发信息完成估价。 MLS还可以作为一个设施，用于有序地关联和传播挂牌信息，以更好地为经纪人的客户，房东，租户和公众服务[4]。多重挂牌服务的数据库和软件被房地产经纪人和房地产业主用来与其他经纪人，业主，买方，卖方和租户分享有关物业的信息。
#### 1.2 多重挂牌服务的进化
*挂牌服务 1.0 (前互联网时代)*<br>
在互联网之前，房地产行业依靠印刷可靠的房地产信息。 打印版本是每年两次，过期的财产信息。
 
*挂牌服务 2.0 (后互联网时代, 前区块链时代)*
 <br>大多数国家拥有少量垄断的在线MLS提供商。

典型费用结构:<br>
●	约 $299.95/月 最多10个挂牌项<br>
●	约 $399.95/月 挂牌一个“白金资产”(Platinum Property)<br>
●	约 $90.00 浏览最多3个类似资产

我们可以做出如下估计，每个订阅者至少要支付每个挂牌项每月$30或者每年$360的费用:
	
    300/10 = 30
 
	30 * 12 = 360

订阅了白金和同类资产的用户至少要支付每个挂牌项每月$520或者每年$6,240的费用:

	30+ 400 + 90 = 520.00
 
	520 * 12 = 6,240.00

用户的常见投诉包括缺乏价格透明度，用户体验和日期信息。 MLS还限制“非订阅用户”可以查看的数据量。

#### 1.3 Rex的挂牌服务概述
Rex提供了一种新型的多重挂牌系统，其中数据是通用的、可以其他系统互操作的。原始数据库是去中心化的，由所有挂牌者拥有。对于用户来说，在拥有权和控制权之上的是基于REX代币的一套奖励系统来补偿用户在网络中的参与。对于每个经过验证的挂牌项（参见“验证系统”）用户需要用REX支付费用。 传统MLS通过收集用户数据和收取费用将其发布到平台来盈利。用户创造价值(数据)，而MLS确是受益者。在Rex平台，用户拥有数据并且可以通过贡献得到回报: 用户挂牌数量越多，获得的奖励越多。Rex上的挂牌数量越多，会吸引更多眼球。越多的眼关注就会增加REX代币的需求。价值是由挂牌者驱使的，并且他们也会成为受益者。另外，用户可以售卖或交换数据，例如市场调研、调查报告和广告空间。最后，一个挂牌者将从地方走向全世界。Rex是一个不受国家或边界约束的大型同构数据库。

#### 1.4 我们为什么要从挂牌开始？
Rex设想3年的时间框架来部署三个工具：

1.	第一年: MLS和过滤层
2.	第二年: 交易
3.	第三年: 基于RexDex的代币化拥有权 (美国/澳大利亚) 

Rex的规划致力于完善以太坊生态的成熟度，扩展政府的参与度和稳定用户使用。首先，块链技术还处于起步阶段。 基础设施仍在建设和测试中。房地产行业和监管机构在基础设施被证实之前，还没有准备好冒险进行交易。因此建立一个MLS，是基于众多原因的最合逻辑的起点。首先，数据是每个房地产交易开始的地方。 第二，如果在测试期间数据丢失，则是可恢复的事件。 第三，以太坊带存在一个学习曲线。Rex的功能包括交易，代币和虚拟钱包。用户需要的是和互联网一致的直观流畅的体验。因此REX在交互体验(UX)上投入了大量的精力。随着技术的提升，流程的完善和用户信心的扩大，Rex将进入交易服务领域。

#### 1.5 Rex运转的细节
任何拥有计算机和互联网连接的人都可以免费访问Rex的数据库。为了有资格获得挂牌奖励，用户需要先在Rex注册。注册过程包括提交用户姓名，联系方式，公司（如适用）和房地产许可证（如适用）。一旦注册，用户可以开始挂牌，并有资格获得奖励。挂牌将立即公布，奖励将在随后两周发放。在两周的时间内，其他用户有机会将该列表标记为垃圾信息。如果挂牌被标记，两个用户都将进入仲裁期。 仲裁期的获胜者将收到挂牌报酬。用户一旦被发现游戏奖励合同将失去其验证状态，不再有资格获得进一步的奖励。REX代币具有多种应用场景，如减少垃圾信息，市场赞助，专业侧写(professional profile)和数据交换，详细说明如下（见“代币实用程序”）。

#### 1.6 技术架构
Rex 技术栈:<br>
●	NodeJS<br>
●	Mithril<br>
●	Solidity<br>
●	Web3.js<br>
●	IPFS<br>

Rex 合约栈(合约代码):<br>
**ListingRewards.sol**: 这个合约用来记录等待中的奖励请求和其状态<br>
**Metafeed.sol**: 这个合约管理平台的主要垃圾信息源。用户会自动订阅Rex的元数据源，但是可以随时取消订阅或者订阅其他用户的数据源<br>
**Datafeed.sol**:  这个合约处理独立的数据源。例如独立部署于各个国家和市场组合的合约。<br>
**DatafeedCoordinator.sol**: 这个合约处理数据源的收集。<br>
**Dex.sol**: 这个合约为REX提供了一个基于Rex去中心化的交易。<br>
**RexCoordinator.sol**: 这个合约被其他Rex合约用来确认其他合约的地址。<br>

#### 1.7 技术栈和未来发展方向

一旦数据层被确认，Rex将会扩张到第三阶段:
交易。Rex将会交付一个简单租赁合约(附录B)，出于以下原因:
1. 流程: 很少政府会监管租赁协议
2. 合约变量的数量: 小的租赁合约大约需要3-5个变量就可以完成一笔交易: 验证，时间，金钱，接入(交易额等)
3. 对方: 租赁合约平均需要五个交易对方:
a. 出租人<br>
b. 承租人<br>
c. 代理人<br>
d. 律师<br>
e. 银行<br>

Rex将提供软件/图形化界面(GUI)来引导用户通过智能合约创建交易过程。Rex将会为第三方银行和DApp开发者提供整合工具。
Rex的第四个阶段是将代币化所有权（附录C）纳入RexDex。代币化拥有权是可以将众多不动产拥有者的拥有权碎片化的一种手段。数字化所有权提供许多好处，包括流动性，可负担性和可转让性。

RexDex将会有多个应用，其中一个将被用交易通过代币化拥有权创建的数字产权。 

代币所有权将会遇到一些主要的法律障碍，特别是在美国和澳大利亚(参见“模型: 阶段3和阶段4”)。因此REX将会把代币化拥有权分成两个阶段：

1.	向RexDex添加代币化所有权：在美国和澳大利亚之外，有更友好的司法管辖区已经创建了dApps来标记房地产资产。 RexDex将为这些标记资产提供交易的地方 
2. 代币化所有权：Rex的实力是构建和建立代币化所有权的技术基础设施。 Rex将以两种方式之一引入代币化化所有权：
a.	与一家成立的公司建立伙伴关系（Rex目前正在与两家公司进行讨论中）
b.	授权许可在RexDex上交易的资产可以使用该技术

## 2.0 区块链
 
#### 2.1 什么是区块链?

区块链是一种分布式数据库或公共账本，随着比特币的发布得到普及。它维护了在一个不断增长的特定网络中执行过的事务列表。“块”按照时间顺序加密，以防止篡改，从而成为网络中每个交易的不可磨灭的记录，每个参与者都可以访问[1]。
 
####  2.2 什么是以太坊?

以太坊可以被描述为一个运行在由用户组成的网络之上的单体共享计算机，在其中资源在以太(Ether)中完成分配和支付。实质上，它是一台世界电脑。
 
#### 2.3 为什么Rex基于以太坊建立?
 
数据需要保存在服务器上，服务器通常由公司拥有或租赁。 因此，个人只能放弃对其数据的控制。

这导致成本增加，可访问性低下，系统之间几乎没有互操作性。

我们现在有了去中心化的手段。 BitTorrent，Swarm和IPFS可以独立做到这一点，但是b区块链提供了在没有中央权限的情况下组织和排序数据的能力。以太坊提供了一个方案，使得区块链，数据分布和货币网格化并存在同一个屋檐下。以太网作为一种方便的介质，以太币可以交换为REX，REX将为应用程序提供燃料。 这是Rex看到区块链和以太坊技术中的绝对价值。
 
Rex建立在以太坊协议上有几个原因。 第一个是提供一个分布式数据库，任何人都可以免费获取房地产信息。

分布式数据库拥有两个优势:
 
1. 用户总是拥有并可访问他们的信息。第三方广告，特别是竞争经纪人的广告，除非发起私人广告，否则不会出现在浏览用户的页面。
2. 价格稳定性: 没有中央权力机构拥有信息，从而对数据进行资本控制。

以太坊还提供了代币货币的手段。Rex利用以太坊代币的概念来奖励提供内容的贡献者，并且提供了一个可供不动产数据自由交易的数字交易所。

当Rex的数据库存储所有挂牌信息90天后，就可以为每一个独立挂牌信息创建一个综合历史。
 
#### 2.4 数据分发
 
自90年代以来，HTTP协议一直是从一个或多个中央服务器向请求节点发送和接收数据包的有用工具。如今我们分发更加庞大的信息数据包，如果请求过多会导致服务器不堪重负。结果是延迟增加，停机和维护。 费用由业主转交给用户。 在2017年，HTTP协议已经变得效率低下。节点不再需要通过集中式路由进行通信，而是可以进行点对点连接。
 
#### 2.5 IPFS<br>
星际文件系统（InterPlanetary File System，缩写IPFS）是一个旨在创建持久且分布式存储和共享文件的网络传输协议。它是一种内容可寻址的对等超媒体分发协议。在IPFS网络中的节点将构成一个分布式文件系统。IPFS使得完全分布式应用变为可能。它致力于让互联网变得更快、更安全、更开放。
  
#### 2.6 Rex的受益<br>
IPFS为Rex以分散的方式分发数据提供了一种手段。当一个挂牌信息提交给Rex时，Rex散列化挂牌标识并将详细信息推送到IPFS。数据默认加密，并全局传播到运行IPFS实例的计算机。由于数据分布并不存储在一台计算机上，所以成本降低，而数据确实全球都可访问的。IPFS的架构提供了一个内置的监管程序，因此Rex（或者其他建立在Rex之上的其他dApps）不能收取大量资金费用或拒绝用户的访问。

## 3.0 问题/解决方案
 
#### 3.1 问题
 
1. 用户牺牲其房地产数据的所有权和控制权给第三方供应商。
2. 交易的房地产是昂贵和耗时的，沟通渠道很差。

#### 3.2 解决方案
 
1. 建立一个全球房地产数据库，利用以太坊和IPFS。 用户维护其数据的所有权/控制权。
2. 提供便于出售/租赁合同的交易层。

## 4.0 Rex的模型
 
#### 4.1 模型

Reed Hastings建立了Netflix，旨在简化用户查看和接收数字内容的方式。首先，Hastings从现有的技术基础设施中获得了价值。 用户在线租用DVD，并通过快递实物发送，避免了传统零售（时间，旅行和滞纳费）的不便。 随着基础设施的成熟，交付从物理到数字化，Netflix实现了指数级增长。

Rex同样采取的是长期策略。 基于Ethereum的技术基础，Rex将开始以多重挂牌服务的形式组合数据库。 随着数据库规模和网络的稳定，Rex将逐步实现交易层。
 
#### 4.2 阶段 
 
●	阶段 1: 建立全球不动产数据库<br>
●	阶段 2: 过滤层<br>
●	阶段 3: 实现交易层<br> 
●	阶段 4: 在RexDex交易所引入代币化拥有权，”液化不动产“<br>

这是在第三阶段和第四阶段将介绍的监管障碍。首先，智能合同需要由法院确认定为合法，可执行的合同。首先，明确的合同需要由法院确认为合法，可执行的合同 [Arizona’s House and Senate approved HB 2417 bill on a nearly unanimous basis.](http://www.swlaw.com/blog/data-security/2017/04/04/arizona-authorizes-smart-contracts-on-a-blockchain/)

接下来，银行监管需要为数字加密信贷采用合适的语言(译注:还是说，要为数字加密信贷发声？)。消费者财政保障局（CFPB）监管美国的抵押贷款行业。 银行需要在其中充当主动的角色来赢得CFPB的关注和参与。

代币化的拥有权引入了另一套政府监督。美国证券交易委员会（SEC）要求充分的公开披露，从而保护投资者免受市场欺诈和操纵，并监督美国的公司收购行动。 一般来说，州际商业中通过邮件或互联网提供的证券的大多数问题必须向证券交易委员会注册。 此外，IRS（美国税法）和FINRA将在代币化所有权中也起着部分作用。 FINRA作为监管机构，负责管理经销商，经纪人和所有公共投资者之间进行的所有业务往来。

第一阶段以外的一些层次包括订阅服务，优化UI，高级过滤技术和用户服务将不会开源。
 
####  4.3 代币分配
 
![Alt description](assets/token_dist.png)
 
创始人和天使投资人将有两年的归属期(vesting period)，每年不超过1,000,000 REX。 这是为了确保REX代币之间的价格稳定性。

#### 4.4 代币使用<br>
阶段1 和 阶段2
 
1. **挂牌奖励 Listing Rewards**: 验证过用户将会通过他们贡献给数据库的每一次挂牌信息获得x个REX。
2. **垃圾信息处理器 Listing Spam Reductor (LSR)**: 当用户提交挂牌信息时需要支付x个REX。LSR是用来防止滥用挂牌奖励合约的。 挂牌奖励总会高于LSR。此外，每个新的验证用户首次挂牌后将会得到5个REX，以补贴其首次交易和LSR。
3. **定向数据源Curation Feeds**: 默认情况下，用户会订阅Rex的定向数据源。
Curation feed是一个筛选过程，其中不良列表被从用户查询结果中除去。 例如，Bob住在纽约，他相信可以比Rex的默认Curation Feed更好地过滤垃圾信息。 鲍勃创建一个独特的数据源，并获得了订阅。 订阅Bob的Curation Feed的用户现在只能通过Bob的Curation Feed查看纽约的查询结果。 鲍勃可以利用广告和挂牌促销通过他的定向数据源获利。
4. **定向广告Curation Ads**: 用户可以通过创建定向数据源并获取订阅用户来收取REX。收取的REX主要用于为挂牌信息搞活动和做广告。
5. **市场赞助 Market Sponsorships**: 用户通过支付x个REX来赞助某个地区市场。
6. **特征属性 Featured Properties**: 通过定向数据源来实现. 
7. **代理人和房东的职业简历 Broker & Landlord Professional Profiles**: 用户通过支付x个REX来创建一个职业简历。拥有职业简历的用户可以在Rex的数据库中搜索到。
 
阶段 3 和 4
 
1. **交易服务 Transaction Services**: 用户支付x个REX来使用Rex建立好的合约/用户交互界面来完成交易目的。 
2. **代币化合约 Tokenized Contracts**: (RexDex)*
 
在第四阶段，Rex将引入代币化所有权。 资产将通过Rex的内部交易所RexDex进行交易。 REX代币将用于交易和结算服务。 我们将在未来几个月内发布更多关于代币所有权的信息。
  
#### 4.5 挂牌奖励 Listing Rewards 

挂牌奖励提供分布式方法来构建和扩展数据库。 任何人都可以将挂牌信息上传到Rex。 经过验证的用户每次上传都有资格获得挂牌奖励。 经过验证的用户（见下面的验证）将收到挂牌奖励。 

挂牌奖励由平台自主资助。 交易费不符合奖励需求的情况下，奖励付款将被降低或停止。

除REX资金挂牌奖励外，REX DAO可以从奖励储备中取出奖励，以资助未来的优先级更高的发展。 DAO有责任说服Rex社区资助进一步发展项目的重要性。

#### 4.6 验证系统 Verification System
Rex需要用户注册才能收到挂牌奖励。 不是经纪人，业主或卖方的用户提交的挂牌信息必须提供批准证明*以获得挂牌奖励。

* Rex将向提交不属于您自己的商家的用户提供认证证明（PoA）。 PoA将要求用户提供证据，证明上市经纪人或房东已经授权他们代表他们提交挂牌。 没有PoA提交的列表将不符合挂牌奖励的资格，并可能导致用户失去验证状态。
 
#### 4.7 支付延迟 Payment Delay

注册挂牌人将需要提交其挂牌报酬表，平台其他用户需要2周的时间就该报酬表提出抗议投票。如果没有抗议，则挂牌人可以在两周周期的最后提取奖励。如果挂牌人输掉了一次抗议判决，那么他将会失去等待支付的报酬，甚至有可能失去认证状态。

* 2周付款延迟过程：在两周的延迟期间，其他用户可以将该列表标记为垃圾信息。 如果挂牌没有被其他用户标记，则被挂牌人有资格申报奖励。 如果挂牌被标记，则标志者和被标记者将被识别并通知。 挂牌人可以做两件事之一： 

1. 如果挂牌是垃圾信息，挂牌人将待支付的金额给予标记着，作为滥用挂牌系统的惩罚
2. 抗议: 用户向Rex提交一张不正当目标的工单。 发起仲裁期间，Rex进行中介。 识别为恶意用户的标记者或被被记者将会失去他们的费用，并且声誉将会被降级。
 
#### 4.8 费用

REX的费用将会在数据源合约中进行收集，并在必要的时候用作奖励或者被用于RexDAO(Rex自制组织)合约。
 
#### 4.9 Rex 订阅模型

Rex 将会提供一个基于订阅的模型来处理用户的所有后端交易
 
#### 4.10 代币销售 Tokensale
 
REX代币将会按照如下计划进行发售:<br>

第一周: 贡献1以太币获得 1,000 REX;<br>
第二周: 贡献1以太币获得 900 REX;<br>
第三周: 贡献1以太币获得 800 REX;<br>
第四周: 贡献1以太币获得 700 REX;<br>

合约变量<br>

贡献期将会在满足以下两个条件中任一个时结束:<br>

四周贡献期结束.<br>
达到安全边界: 133,333 ETH(以太币).<br>

#### 币池A（代币销售）由全部REX代币供应量的50％组成。币池A将被分配给在代币销售期间作出贡献的用户。<br>

#### 币池B由全部REX代币供应量的20％组成。 币池B将在REX平台上分配给挂牌奖励合同。<br>

#### 币池C由全部REX代币供应量的5％组成。 币池C将分配给天使投资人。<br>

#### 币池D由全部REX代币供应量的15％组成。 币池D组将分配管理人员，创始人，参与REX理念的构想，技术的实现和结构支持等工作的人<br>

#### 币池E由全部REX代币供应量的7％组成。 币池E将分配给REX项目的合作伙伴和/或顾问，以及奖金运动(Bounty campaigns)的参与者。<br>

#### 币池F由全部REX代币供应量的3％组成。 币池F将分配给公司的附属公司<br>

REX代币销售地址: 0x99d439455991f7F4885F20C634c9a31918D366E5<br>

代币销售合约基于OpenZeppelin框架。 我们已经与OpenZeppelin签订了REX代币销售合约创建和测试的合同。我们还与马修·迪·弗兰特（Matthew Di Ferrante）合作，Matthew Di Ferrante先前曾与Ethereum基金会的成员合作，并最近审核了一个处理日均百万笔交易的大型交易所的智能合约基础设施。<br>

#### 发送须知 Sending Instructions<br>

在代币发售期间，请检查我们代币发售页面的地址并至少与我们认证的至少两个社交媒体(下面列出)上面公布的地址进行核对后进行贡献。我们将会在接下来的一周在我们的频道持续公布该地址。<br>

## 5.0 结论

Rex坚信我们应该控制我们的挂牌数据。我们应该有能力更有效地交易。

## 6.0 Founder Bios
 
#### 6.1 Stephen King

Stephen 是一位专注不动产商业和区块链科技的企业家。自2013年起，Stephen便带领新泽西普林斯顿的King Realty集团参与了上千万美元的不动产交易。Stephen参与了几家房地产相关技术创业公司的设计。 Stephen是普林斯顿以太坊见面会的创始人。
 
#### 6.2 Russell McLernon
 
Russell是以为技术战略家。 他在企业软件开发方面拥有超过15年的经验，并在区块链相关开发和项目方面拥有7年以上的经验。 他技术精湛，能够迅速参透用户需求，没有他处理不了的软件开发或集成挑战。
## 7.0 联系方式和引用
#### 7.1  联系方式
**邮件 Email**<br> support@rexmls.com
 
**官网 Rex Landing Page** <br>http://www.rexmls.com
 
**博客 Rex Blog**<br>http://www.rexmls.com/blog/
 
**Slack**<br>https://rexmls.herokuapp.com/

**twitter**<br>https://twitter.com/REXmls

**Facebook**<br>https://www.facebook.com/theREXmls/

**LinkedIn**<br>https://www.linkedin.com/company-beta/11070246/

**Instagram**<br> @theREXmls

#### 7.2 引用 

1. https://cre.tech/will-sleepy-real-estate-industry-wake-blockchain/
 
2. https://ipfs.io/
 
3. http://legal-dictionary.thefreedictionary.com/Property+(ownership+right)
 
4. https://en.wikipedia.org/wiki/Multiple_listing_service
 
5. http://digitalcommons.law.yale.edu/cgi/viewcontent.cgi?article=1409&context=fss_papers
 
6. http://www.ibtimes.co.uk/ethereums-viktor-tron-talks-about-swarm-skeleton-web-3-0-1560654

## 8.0 附录
#### 8.1 附录 A<br>不动产交易: 今天
数据:<br>
当一个买家、租户或经纪人想找房屋、办公室、仓库、土地或者零售空间时，他们大多会在在线MLS进行搜索。可访问的数据在用户付费之前是受限制的。付费会员需要交纳高昂的年费并被平台收集客户和交易相关的额外数据。

交易:<br>
用户订阅并确定物业位置后，他们将与挂牌代理人协商价格。 买方和卖方都由自己的律师起草，编辑和完成采购与销售协议（PSA）。 在PSA内是买方和卖方必须执行的交易清单。 允许买方约30-90天对被称为尽职调查的财产进行分析。 尽职调查包括但不限于：

1. 结构检查
2. 电器检查
3. 毒物检查
4. 屋顶检查
5. 环境检查
6. 联结查询
7. 调查

买方的贷方将进行：
 
1. 抵押发票（买方资格）
2. 评估
3. 产权搜索(title search)

在尽职调查中，卖方将履行PSA中规定的某些义务：
 
1. 建筑维修
2. 市政批准
3. 治愈判断/留置权(Cure judgments/liens)
4. 获得入住证（如有必要）

在整个交易中，买方和卖方通过银行，律师，检查员和房地产经纪人进行沟通。 通信链不可避免地导致买方和卖方的延迟和成本上涨。一旦尽职调查到期并且双方履行各自的义务，将会设定一个交割日期。 以下是交割止日期前所需文件的简要列表：

1. 交割单(Closing Statement)
2. 产权调查报告 Title report
3. 税/保险单
4. 检查/调查报告
5. 身份证明
6. 银行对账单/授权
7. 资金

在美国，房产交割的附加费用对于住宅用房平均增加约10000美元，商业用房平均增加约20000美元（取决于交易规模和地方税务管辖范围）。

假设实例

Bob想在新泽西州普林斯顿出售一个混合用途的建筑物：

* 地址：Nassau街236号
* 价格: 350万美元
* 9间一卧室公寓
* 2个零售单元
* 净营业收入：17.5万美元
* 资本化率：5％

数据: <br>
Bob决定在当地的MLS上挂牌Nassau街236号。 经过几周的时间，没有吸引到任何用户，Bob咬牙注册了MLS的高级增值服务（约合299.95美元/月）。高级版本授予Bob访问周围财产数据的能力。三周后还是没有任何动静，Bob决定花90美元做一次类似产权分析(Comparable Property Analysis)。然而这些信息是过期的并且毫无用处。Bob意识到Nassau街234号一直出现在查询页面的最底部。Bob发现MLS上面还有一个约$399.95 每30天的一个附加费用，可以让出现在搜索结果页中的Nassau街234号打上“白金”标签，Bob决定使用这个白金挂牌服务。

Bob为Nassau街234号的挂牌支付了约790美金/月或790美金/挂牌信息的费用。

交易: <br>
Alice的经纪人发现了Bob在MLS上的挂牌信息，并转发给了Alice。Alice提出了340万美金的报价。Bob接受了Alice的报价，双方律师便开始在以下条款中进行PSA(协商采购与销售协议)的商议.

1. Alice允许使用30%的贷款(疑问，Alice is to obtain 70/30 financing)
2. 尽职调查期：60天。
3. 尽职调查期满五天后完成交割。
4. Bob必须修理受损的人行道，并进行电气检查。
5. Bob必须用PVC代替铸铁废料线。
6. Bob必须更换损坏的屋顶瓦。
7. Bob的建筑必须通过火灾检查。

Alice在其律师的托管帐户中存入17万5千美元。由于所有权机构与银行之间沟通不畅，交割延迟两周，由Bob和Alice负担律师费用和相关费用。交割最终定下日期，并在几小时的文书工作后，产权完成了交割并在普林斯顿市政务员办公室被人工记录。
Alice和Bob总共支付了大约4万美元的交易成本，Bob每月支付约790美元的挂牌费用。

#### 8.2 附录 B<br>租赁交易

Alice是CBRO的经纪人，在REX上挂牌了一个25,000平方英尺的办公室。 Ether Realty经纪人Bob为其客户Osprey Inc.显示了123 Alpha这个资产。Osprey按照以下条款进行10年租赁：
合同细节
物业：澳大利亚悉尼，阿尔法街123号
租客：Osprey Inc.
价格：50美元每平方英尺每年
期限：10年

Osprey Inc租赁条件(租户)
1. Osprey Inc.在合同执行时需保证两个月的安全期
2. Osprey Inc.在合同执行时托管第一个月的租金给阿尔法街211号（业主）
3. 在合同执行时保留室内展示墙30天
4. 在合同执行时履行和发布一个25美元每平方英尺的工作函(25万美元)给Osprey Inc.
5. 履行和支付2%的中介费给CBRO 2%的中介费给Ether Realty。在签约时支付一般，合同执行后90天支付另一半

123 Alpha 和 Osprey的委员会决定在REX上合作签署上述合约。双方可以在任何时间通过在合约上面双向广播一笔交易来完成合约的修订。合约和更改在区块链上是实时可见的。 123 Alpha Inc.和Osprey Inc.同意使用一种稳定的货币来进行资金交易。 所有的钱根据智能合同的条款进行托管和发放。
123 Alpha Inc.和Osprey Inc.受益于透明的智能合同，在其中可以快速查看和同意内容的修改。高效的沟通渠道带来了时间和费用的减少。 交易永久记录在区块上，为记录保留和租赁续订提供了安全的手段。 根据智能合同，CBRO和Ether Realty按时付款，免去了开具发票和付款跟进的需要; 自此完成我们的租赁示例

#### 8.2 附录 C<br>代币化拥有权

如果你可以交易克莱斯勒大楼的1000个代币如同交易1000股的苹果股票，你会作何感想？

背景
克莱斯勒大楼于1930年5月27日完工。由沃尔特·克莱斯勒（Walter P.Chrysler）拥有，是克莱斯勒的新总部。 克莱斯勒大楼高77层，办公面积约2,062,772平方英尺。 自从克莱斯勒家族在1953年出售以来，这座建筑已经换了几次手。1998年，蒂什曼派派尔物业和旅行保险以220,000,000美元的价格购买了克莱斯勒大楼。 2001年，蒂斯曼出售了阿布扎比投资理事会75％的股份。 今天，阿布扎比投资理事会拥有90％的股份，而Tishman则保留10％。

重新定义房地产所有权：Chrysler Dapp
假设Rex通过4％的资本化率以3,000万美元现金购买了阿布扎比和蒂什曼在克莱斯勒大楼的全部股权：

克莱斯勒大厦的90％被长期租赁，平均价格为108美元每平方英尺每年。 总收入为每年2亿5千万美元。 费用约为40％或80,200,500美元。 因此，净营业收入为1.2亿美元。

基于采用区块链技术的以太坊，Rex创建了一个名为Chrysler Dapp的分布式应用程序。Chrysler Dapp创造了1,000,000,000个CHRY代币。 Chrysler Dapp分配7.5亿个CHRY代币（占总供应量的75％）在广泛的人群中出售。 CHRY代币将以每个代币3.00美元（估价为3,000,000,000美元）上市。

Chrysler Dapp的开发商创建了一家名为克莱斯勒管理公司的公司。克莱斯勒管理公司将是克莱斯勒大楼的管理实体，负责管理，租赁和法律。 克莱斯勒管理公司将保留100,000,000CHRY或占总量的10％。 剩余的1.5亿CHRY将用于资本储备。 每季度，克莱斯勒管理公司将将所有正的现金流量（费用后）转换为CHRY令牌，并将其存入社区智能合约。合约将根据每个利益相关者所拥有的代币的百分比进行CHRY代币的发放。

在克里斯勒管理公司（Chrysler Management Inc.）的章程中，克莱斯勒管理有限公司（Qurysler Management Inc.）有义务每季度公布上市公司的详细收入和费用报告。

经济数据
代币参与者有机会在纽约市拥有一个标志性的建筑物，附带潜在的10％的上涨空间：如果克莱斯勒管理公司将10％的空闲房间出租出去，它将增加净营业收入，随之带来的是建筑价值的上升：

> 闲置 + 租户 = +营运净收入 = +建筑物价值 = +CHRY代币价值

市场供需平衡显示我们价值的上涨通常会导致价格上涨。 相反，如果克莱斯勒失去一个主要租客，那么代币的价值就会减少。

实体资产<br>
正如我们看到近期的代币销售情况，价格波动巨大，市场也可能变得非常不合理。 然而，像克莱斯勒大厦这样的实体资产可以与当地的房地产市场挂钩，从而更准确地确定价值和感知风险。

例如：<br>
ABC公司以108美元每平方英尺的价格租用了50万平方英尺。当租约到期时，他们离开了克莱斯勒大楼。在这笔交易中，该资产的年度总收入损失5400万美元。CHRY代币价格跌至1.00美元，估值为10亿美元。 一些复杂的个人发现实际的市场价值（在损失ABC公司这个客户之后）应该接近17亿美元：
$ 146,500,000 - $ 80,200,000 = $66,300,000 NOI 在4％的资本化率下 = $16.57亿或$1.67每CHRY代币。
投资者可以从代币价值潜在的0.67美元的上涨空间、长期建设升值以及剩余10％的空缺填补后中获利。

同样可以看到，如果代币价值跳转到$4.00或$4,000,000,000，而NOI没有真正增加，复杂的投资者可能会减持CHRY代币，通过市场供需平衡稳定价值。