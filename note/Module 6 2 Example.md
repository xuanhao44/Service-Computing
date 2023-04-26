# Module 6 Example **RailCo** Ltd.

Service Engineering

[TOC]

## 0 RailCo's Start

It started out as a brokerage for various  railway wholesalers, but then came to  specialize in air brakes.
- The narrowed business focus resulted in increased  opportunities, as RailCo was able to become a  wholesaler in its own right by dealing directly with  air brake parts manufacturers.

它最初是为各种铁路批发商做经纪，但后来专门从事空气制动器。

- 业务范围的缩小带来了更多的机会，因为 RailCo 能够通过直接与空气制动部件制造商打交道而成为自己的批发商。

## 1 RailCo's automated environment

- Outdated technology
- A two-tier client-server system governing all accounting  and inventory control transactions.
  - Two administrative clerks manually feed this solution with  standard transaction document data (primarily incoming and  outgoing purchase orders and invoices).
  - Receipt and submission of these documents typically initiates corresponding inventory receiving and order shipping processes.
- A contact management system in which customer and  business partner profile information is stored and  maintained.
  - This simple application consists of a database fronted by Web-  based data entry and reporting user-interfaces.
  - Users range from managers to administrative assistants and accounting personnel.

- 过时的技术
- 管理所有会计和库存控制事务的双层客户端-服务器系统。
  - 两名行政文员手动为该解决方案提供标准交易文档数据（主要是进出境采购订单和发票）。
  - 这些文件的接收和提交通常会启动相应的库存接收和订单运输流程。
- 一个联系人管理系统，其中存储和维护客户和业务伙伴的个人资料信息。
  - 这个简单的应用程序由一个数据库组成，前端是基于Web的数据输入和报告用户界面。
  - 用户范围从经理到行政助理和会计人员。

## 2 Observed Problems

- Profit margins have been noticeably declining over the past year.
  - Clients have been switching to a competitor providing the same  products in a more efficient manner and at a lower cost.
- Further investigation led to the discovery that this competitor has  implemented an extension to their existing accounting system,  allowing them to perform various transactions online via B2B  solutions provided by some of the larger clients.
- A further unpleasant revelation was that RailCo's primary client,  Transit Line Systems, has started an online relationship with this  competitor as well.
- RailCo is a company with outdated technology automating inefficient business processes.
  - Need to better respond to new business trends and automation requirements.
- 去年利润率明显下降。
  - 客户已经转向以更有效的方式和更低的成本提供相同产品的竞争对手。

- 进一步调查发现，该竞争对手对其现有会计系统进行了扩展，允许他们通过一些大客户提供的 B2B 解决方案在线执行各种交易。
- 另一个令人不快的消息是，RailCo 的主要客户 Transit Line Systems 也与这家竞争对手建立了在线关系。
- RailCo 是一家技术过时的公司，将低效的业务流程自动化。
  - 需要更好地响应新的业务趋势和自动化要求。

## 3 RailCo problems

- RailCo's original goals
  - upgrade its automation systems
  - remain competitive
  - continue its business relationship with its primary client, TLS.
- RailCo had lost TLS as a customer when a competitor managed to provide air brake parts at a lower price while also interfacing with TLS's B2B system.

- 铁路公司的最初目标
  - 升级其自动化系统
  - 保持竞争力
  - 继续其与主要客户 TLS 的业务关系。
- 当竞争对手设法以更低的价格提供空气制动部件，同时还与 TLS 的 B2B 系统接口时，RailCo 失去了 TLS 的客户。

## 4 RailCo initial services

To remain competitive and minimize losses, RailCo must  upgrade its automation environment as soon as possible.  Its top priority is to participate in online transactions with  TLS. Before our storyline begins, RailCo has already  hurried to build a pair of Web services.

- RailCo rushed to catch up, producing a pair of Web services designed only for use with the TLS system.
- This allowed RailCo to regain its position as a TLS vendor.
- These two initial Web services were
  - Invoice Submission Service
  - Order Fulfillment Service
  - (Another service was added later to interact with the TLS Notification Service.)

为了保持竞争力并尽量减少损失，RailCo 必须尽快升级其自动化环境。它的首要任务是通过TLS参与在线交易。在我们的故事情节开始之前，RailCo 已经匆忙地构建了一对 Web 服务。

RailCo 急于赶上，生产了一对仅用于 TLS 系统的 Web 服务。

- 这使得 RailCo 重新获得了 TLS 供应商的地位。
- 这两个最初的 Web 服务是
  - 提交发票服务
  - 订单执行服务
  - （后来添加了另一个服务来与 TLS 通知服务交互。）

## 5 RailCo case example - summary

- RailCo realised that it was loosing their clients to their competitor
- To prevent loosing their primary client, Transit Line Systems (TLS), they decided to build a pair of Web Services to participate in online transactions with TLS
  - RailCo-to-TLS Invoice Submission Process
  - TLS-to-RailCo Purchase Order Submission  Process

RailCo constructed their services based on **Bottom-up** approach.

- RailCo 意识到他们的客户正在被竞争对手抢走
- 为了防止失去他们的主要客户端，运输线路系统(TLS)，他们决定建立一对 Web 服务来参与与 TLS 的在线交易
  - RailCo-to-TLS 发票提交流程
  - TLS-to-RailCo 采购订单提交流程


RailCo 基于**自下而上**的方法构建他们的服务。

## 6 RailCo bottom-up Web services construction results

- The services were assembled quickly, to accommodate a single client
- The services were delivered to accommodate a specific need
- fulfilled immediate business requirements
- Efficient
- Cost-effective
- **Initially considered successful**

- 服务快速组装，以适应单个客户端
- 提供服务以满足特定需要
- 满足即时业务需求
- 高效的
- 成本效益

\- **最初被认为成功**

## 7 However, very soon RailCo needed to respond to multiple changes

- TLS implemented **a new policy** that affected some of the purchase order business logic on RailCo’s end
- RailCo’s own internal business process underwent a **change** as a result of a module upgrade within their legacy accounting system
  - Affected low-level data access parameters processed by the RailCo Invoice Submission Service
- Other RailCo’s legacy systems that interfaced with their Web services also underwent **changes**
- Numerous **changes** were made to existing automation processes

- TLS 实施了一项新政策，影响了 RailCo 端的一些采购订单业务逻辑

- RailCo 自己的内部业务流程由于其遗留会计系统的模块升级而发生了变化
- 影响 RailCo Invoice Submission Service 处理的底层数据访问参数
- 其他 RailCo 的遗留系统与他们的 Web 服务接口也经历了**变化**
- 对现有自动化流程进行了大量更改

## 8 Redeveloping web services challenges

- A significant redevelopment effort
- There was no separation of business and application logic
  - Change impacted a broader part of their solution environment
- None of the services were reusable
  - Less chance that the new requirements could be fulfilled by existing services
- With each programming modification came the overhead 
  - Testing and development phases

- 重大的重建工作
- 业务逻辑和应用逻辑没有分离
  - 变更影响了解决方案环境的更广泛部分
- 所有服务都不可重用
  - 现有服务满足新需求的可能性较小
- 每次编程修改都会带来开销
  - 测试和开发阶段

## 9 RailCo decides to start from scratch

- **The agile delivery strategy** is chosen
- Only application and business service layers will be modeled (cannot afford to invest in the middleware required to implement an orchestration layer)
- **选择敏捷交付策略**
- 只对应用程序和业务服务层进行建模（无法负担实现编排层所需的中间件的投资）

