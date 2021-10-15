# 开发者体验：探索与重塑

> 开发者体验，与用户体验类似，只是对象是软件开发人员。将之与进行对应，便是开发人员对于针对使用或期望使用的产品、系统或者服务的认知印象和回应。有所不同的是，用户关注的内容变为库，SDK，文档，框架，开源解决方案，通用工具，API 等的开发人员的体验。

2019，在经历了多个低代码前端项目的售前，以及一个低代码项目的技术实践强化，发现国内的 IT 企业缺乏对于『开发者体验』缺乏系统性的思考。便想着结合自己的项目经历、社区经验、国内外实际情况等，编写一个简要的开发者体验电子书。 

# 定义开发者体验

来，先我们来看一个开发者体验（DX，Developer Experience）的定义：

> 开发者体验，与用户体验类似，只是对象是软件开发人员。将之与国际进行对应，便是开发人员对于针对使用或期望使用的产品、系统或者服务的认知印象和回应。有所不同的是，用户关注的内容变为库，SDK，文档，框架，开源解决方案，通用工具，API 等的开发人员的体验。 

而完善开发者体验是有一些基础条件的：

 - 稳定性。SDK、库、框架等具备满足使用方持续可用的状态。
 - 功能完备。可以满足大部分的正常的功能需求。

简单来说，就是只有在可用的情况下，设计开发者体验会更加有价值，即开发者体验是一个加分项。而如果我们能在开发的前期就考虑用户体验的话，它会为后续的开发带来便利。

## 开发者在体验什么？

什么是开发者体验？那不就是让开发人员觉得爽吗。

什么才叫爽呢？来一起看几个例子。

### 安装谁更简单？

先让我们来看一个软件安装的例子：

1. 一键命令行安装。如 `curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh`
2. 按步就班下载和使用。如打开官网，找到对应的平台（操作系统）下载可执行文件，打开安装软件，执行安装步骤，一步步进行。

这是 Rust 官方提供的两种不同的 Rust 安装方式。

### 谁的引入更简单？

再看个使用软件的例子：

1. README 即起步文档，添加依赖，复制示例代码。
2. README 里没有起步，需要跳转到文档网站，添加依赖，添加构建脚本，复制示例代码。

两者都是 Rust 里的语法解析器，前者是拥有 2.2k stars 的 pest，后者则是拥有 1.7k stars 的 lalrpop。

这里，先不讨论两个不同的库在开发上的区别，从直观感受来说，我们就可以直接区别。

### 起步谁更快？

来两看两个上手指南

1. 学习新的语言，学习新的语法，入门文档很长（start），还需要编译，文档不易访问。
2. 通过 script 标签引入 ，直接开始编写代码。

你觉得新手会选择 Vue 还是 Angular？

## 定义开发者体验

这样一来，我们对于开发者体验都能有一个简单的体会。也就能理解什么是开发者体验了。

### 什么是开发者体验？

开发者体验是指开发人员在使用软件、工具、代码等的体验，它与用户体验类似，只是对象是软件开发人员。将之与国际进行对应，便是开发人员对于针对使用或期望使用的产品、系统或者服务的认知印象和回应。有所不同的是，用户关注的内容变为库，SDK，文档，框架，开源解决方案，通用工具，API 等的开发人员的体验。 

国内开始关注开发者体验主要有以下的一些原因：

 - 外部开源。即越来越多的开发人员开源了自己的软件，迫切地需要提升软件的体验。
 - 内部开源。在内部通过开源来进行部门之间的协同效应。
 - 内部基础设施共享。让内部的开发人员使用内部的基础设施时，获得比外部开源软件更好的体验，提升其在内部的口碑。
 - API 经济。对外提供 API，需要与更多的业内组织竞争。
 - 云原生。云厂商面向开发者提供服务。
 - 生态构建。面向合作伙伴需要提供更便捷的接入服务。
 - SDK 等工具提供方。
 - ……

原因多种多样，但是其核心都是想通过开发者体验来提升竞争力。

## 开发者体验六要素

再次强调一下：关注开发者体验之前，应该确保核心功能：完善 + 稳定。即你需要提供可用、稳定的特性，再去提升总体的用户体验。除非，对于你的系统来说，你在一开始就不缺用户。

从我在开发社区的使用经验、网上了解的相关信息以及与一些专业人士的沟通中，我认为以下几点是进行 DX 时要考虑的要素：

 - 错误呈现。即出错时，以何种方式来呈现。
 - 文档体验。
 - 易用性。如何简化开发。
 - 交互式。降开发者学习成本。
 - 触点。让更多的人知道这个软件。
 - 支持。

太长不看版：

|  错误呈现 | 文档体验 | 易用性 | 交互式 | 触点 | 支持 |
|-----|-----|-----|-----|-----|-----|
|  错误描述 | 开发者门户 | 一键式安装 | 低配置/零配置 | 文章 | 问题反馈渠道 |
|  报错即文档 | 发布日志 | 自动化版本迁移工具 | 声明式使用 | 演讲/分享 | 问题响应时间 |
| 报错即修改建议 | 代码生成文档 | 自助式搭建 | 可交互文档 | Hackathon | 开发者即服务 | 
|  | 版本迁移指南 | |  沙盒及产品环境 | | 开发者社区 |

可能还有其它内容，如果有的话，欢迎与我探讨。

### 错误呈现

PS：出于安全原因，有些内容不适合在外部暴露，因此并不建议所有的东西都应该对外呈现。

对于开发者体验来说，错误呈现就是让开发者有办法快速定位问题和修改问题。常见的一些可优化的部分是：

 - 错误描述。即软件的出错以合理的方式描述出来，可能是一段文字，一个错误码等。
 - 报错即网站。即复杂的出错场景里，可以通过可访问的链接来告诉开发者如何修改问题。
 - 报错即修改建议。即出错时，告诉开发人员可以尝试以下的方式来修改问题。

这里，我们可以看一个 Rust 出错的示例：

```bash
error[E0425]: cannot find value `RE_ACCESS` in this scope
...
177 |           if let Some(capts) = RE_ACCESS.captures(line) {
    |                                ^^^^^^^^^ help: a static with a similar name exists: `RE_CLASS`
```

虽然，这个提醒不一定那么智能。但是，它在帮助定位问题的同时，还在一定程度上来解决一点问题。

### 文档体验

文档是一种传统知识的载体。优秀的程序员即能通过代码来传递知识，还会通过文档来表达自己。

> 软件编程即理论建立与传递。 ——  Peter Naur

对于文档来说，依旧的，我们还会关注于：

 - 开发者门户。作为整个知识体系的承载
 - 发布日志/更新日志。即 CHANGELOG.md
 - 代码生成文档。
 - 版本迁移指南。针对于出现 Breaking Change 的场景，需要详细给出每一部分的迁移示例。
 - 测试用例。在开源世界里，除了文档，还有测试用例可以读懂一些特别的用法。

开发者门户是一个复杂的话题，后面我们会再介绍。如下是 D3.js 6.0 的 [migration guide](https://observablehq.com/@d3/d3v6-migration-guide)  示例：

```
For example,

  selection.on("mousemove", function(d) {
    … do something with d3.event and d…
  })

becomes:

  selection.on("mousemove", function(event, d) {
    … do something with event and d …
  })
```

我们还会在易用性里提供更好的方式。

### 易用性

易用性本身是非常难度量的，

 -  一键式安装。可以是一行命令，也可以是 `1-click` 之类的。
 - 自动化版本迁移工具。即针对于版本升级时的 API 修改，可以提供自动修改工具，典型的如 Angular CLI 来升级 Angular。
 - 自助式搭建。如 Spring Initializr，可以让开发人员选择合适的服务和工具，而后生成项目等。

在高中时期，我尝试了市面上的一个又一个 GNU/Linux 改行版。如 Ubuntu 和 OpenSuSE 会向我们寄一些安装 CD/DVD，用来帮助新手快速安装 GNU/Linux 操作系统。在我体验了 OpenSuSE 之后，我被它文档上的 `Install software via 1-click` 所惊艳（当时年轻）。

如我们找到了中文输入法：Fcitx （[https://zh.opensuse.org/Fcitx](https://zh.opensuse.org/Fcitx)），文档上包含了各种的介绍、如何安装，以及一键安装 —— 现今的 macOS 和 Windows 似乎也没有这样的功能。

### 交互式 

在各类 PAAS 服务流行的今天，交互式的 API 体验已经成为了一个主流的方式。进细一步地，我们可以

 - 低配置/零配置。人们为了灵活性而引入的各种配置本身是反人性的，大部分的配置应该是内置的，不应该由普通的开发者来配置。
 - 声明式使用。即 API 应该尽可能简化，只需要简单的声明即可使用。
 - 可交互文档。如 Swagger 可以在线尝试 API。
 - 沙盒及产品环境。即提供一个在线的类可编程环境。

最典型的一些例子就是现代化的编程语言里提供的 Playground，如 Golang 和 Rust 都提供了 Playground。它可以让开发人员查看文档，同时运行应用的代码，还能修改代码并运行。

### 触点

触点是指如何去提供加深与开发者的关系。虽然有一个更专业的名称是『开发者关系』，但是它有一个更复杂的模型。这里就简化为触点，意思就是如何与开发者进行接触的点：

 - 内容/文章
 - 演讲/分享
 - Hackathon/黑客松
 - 论坛。只在形成一定规模时才考虑

从某种意义上来说，它是叫推广，但是呢，从个人的角度来看，触点这个用法比推广好得多 —— 触点可以让你意识到：现有的机制是不是无法连接到更多的开发者。

### 支持

这部分就是对于开发人员的支持了，每个人也都非常熟悉：

 - 问题反馈渠道
 - 问题反馈与响应
 - 开发者即服务。源自我之前的一篇文章《[开发者即服务](https://www.phodal.com/blog/developer-as-a-services/)》，意指开发者一对于指导问题。
 - 开发者社区。

再说说开发者即服务，是（Developer-as-a-Service）的，亦可称为 “按需即用的开发者”。即当开发者使用某一工具、库，遇到任何相关的问题，可以随时找开发者为我们提供服务。哪怕是使用者使用了我们的 A 框架，但是遇到 B 框架有问题，他/她们也会觉得 A 框架有问题 ——因为 A 框架的开发者们是一种服务，一种开箱即用的服务。

## 度量开发者体验

考虑到度量开发者体验是一个复杂的问题，这里只简单列一下我所认为的两个易于度量维度：

 - 首次运行所需时间
 - 文档触达速度

其它的则是**常规度量指标**，以及对于开发者门户的度量。

### 首次运行所需时间

> 首次运行所需时间即开发人员从接触到创建第一个可运行的应用或者测试等所需的时间。

它可以让我们关注于：

 - 设计最小的使用步骤
 - 提供更好的 Get Started 设计
 - 提供有限次数限制的 Demo Token。
 - 更快的体验速度。对于下载服务，采用 CDN，适用于国内网络的下载机制。
 - ……

这个指标体系可以帮助我们，理解开发人员在过程中遇到的过程痛苦。

### 文档触达速度

> 文档触达速度，即从修改完文档到所有开发人员可见所需的时间。

我们最常见的一个例子是 GitHub Pages，当我们更新完文档时，它可以实现分钟级的部署。这个维度的指标的目的主要是：

 - 有意识地加快文档更新过程
 - 让经常出错的问题可以快速更新
 - 提醒开发人员修复了哪些问题

它可以让问题的反馈快起来。

### 常规度量指标

接下来，就是我们常见的一些指标，受限于框架和 SDK 等的不同会有些变化 ，典型的如：

 - API 响应时间 
 - API 出错率
 - API（可选），『每周活跃调用者数』、『API 响应时长』

对于开发人员，可以展示 **API 情况的 dashboard**，用于展示 API 服务的当前状况，如 GitHub Status。这样一来，就不需要再回答 API 是否挂了的问题。

### 开发者门户成熟度模型

在编写这篇文章的过程中，刚好看到了一篇对于门户的度量模型，《[How Mature Are You? A Developer Experience API Maturity Model](http://jennywanger.com/speaking/dx-maturity-model/)》简单地翻译了一些**国内适用**的部分（详细见原文）：

| Level 1 |  Level 2 | Level 3 | Level 4 |
|-------|-------|-------|-------|
| 封闭的系统 | 门户是自服务的，但是不连贯的 |  完全自服务 |  可个性化的统一门户 |
| 文档缺乏成功调用 API 的信息 |  1 天内可以调用  API | 10 分钟内可以调用 API |  分钟级 API 调用 |
| API 和功能没有正确对应 | 快速开始指南、修改日志和教程 | 提供沙盒和生产环境 | 认证流程 |
| 响应问题需要一周的时间 | 交互式文档 | 代码示例和库 | | 
|   | 问题在 2 ~ 3 天内被回答 | 24 小时回答问题 | |

## 如何提升开发者体验

从个人的角度来看，提升开发者体验是一个相对麻烦的过程。除了上述的两个指标之外，我觉得还有两种方式可以帮助提升开发者体验：

 - 竞品对比。
 - 新用户引导流程。

嗯，基本上和用户体验是类似的。

### 竞品对比：看齐

竞品对比，主要是通过与类似产品的对比，让自己与业内保持一致的水准。

如下是 Rust 和 Golang 的对比（只选取部分，出自于《[Android Go vs. Rust: Features, Similarities & Differences](https://www.konstantinfo.com/blog/android-go-vs-rust-features-similarities-differences/)》）

|   | Rust | Golang |
| --- | --- | --- |
| 性能 | 高效能，比Swift语言快一点 | GO和Java的性能不及Rust |
| 方便性 | 零成本运行时抽象，非常容易且安全地用于内存等处理 | 使用和管理容易 |
| 易于学习 | 需要花时间来学习和掌握用于内存管理的语言抽象 | 有完整的开发文档，大量的用户社区 |
| 发展速度 | 与Go程序相比，RUST的编译时间更长 | 既简单又快速 |
| 并发与并行 | RUST没有具体的并发或异步操作。 | Go 具有例程（轻量级线程）和通道（go例程的通信机制），可简化应用程序的创建过程。具有本机测试机制，可在运行时发出警告。 |

通过这样的对比，从其它产品学习。

### 新用户引导流程

站在开发人员的角度出发，梳理新用户从使用过程中的痛点问题。一个详细的例子可以见：[Onboarding journey](https://toddmoy.com/sendgrid-journeymap)

# 运营模型：技术产品化运营

> 技术产品化运营，是将技术产品（如开放 API、开源软件、开放平台、SDK、工具等）视为产品，在组织内部或者外部进行推广，以吸引更多的用户、开发者等参与到其中，加入到技术产品开发中，或者是采用该技术产品在其应用域构建解决方案。

## 技术产品化运营

与几年前相比，国内与技术产品化运营相关的岗位越来越多，诸如于布道师（Evangelist）、开发者关系（DevRel）、技术运营、开发者运营等。虽然，岗位职责稍有不同，也就是目标 KPI 是不同的。但是呢，其中有相当多的相交之处，诸如于从技术社区出发，去为技术产品（如开源项目、云服务、商业化工具等）带来某一方面的价值 —— 如品牌、销售量等。

基于这一个基本的模式（从社区-产品），我提取了第一版本的『**技术产品化运营元模型**』（请原谅我图画的丑）：

![技术产品化运营元模型](https://dts.plus/technology-product-marketing/community-technology.png)

从某种意义上来说，这个领域所做的事情和现在的新媒体运营有点相似。但是，它的强技术背景大大提升了准入的门槛。而如果你也有一定的经验，你可以从上图中的四个步骤，看出产品化运营的困难之处，它涉及到多个领域：技术、社区运营、开源者体验设计、开放式协作等。

### 定义技术产品化运营

> 技术产品化运营，是将技术产品（如开放 API、开源软件、开放平台、SDK、工具等）视为产品，在组织内部或者外部进行推广，以吸引更多的用户、开发者等参与到其中，加入到技术产品开发中，或者是采用该技术产品在其应用域构建解决方案。

如上所述，市面上已经有一系列的技术产品化运营的岗位，这些岗位受限于角色定义的不同，所承担的职责也有所不同。如：

1. 布道师（Evangelist）。从语义上来定义，这个岗位的主要职责是布道。也几乎（90 %）承担了技术产品化运营的所有职责，诸如于自身成为影响力中心，构建对应的技术社区，以吸引用户。再手把手帮助客户上手应用，维护和开发者的关系等。
2. 开发者关系（DevRel）。从语义上来定义，这个岗位的主要职责是维护和开发者的关系。从职责来看，它 99.99% 接近于承担了所有职责。
3. 开发者运营。从语义上来定义，这个岗位的主要职责是开发者相关的社区运营。主要偏向于活动与相关的内容策略等，可以由低技术背景的角色来承担。
4. 技术运营。从语义上来定义，这个岗位的主要职责接近于传统的营销岗位。
 
 其它的诸如于技术品牌等与我们这所描述的职责有些远。
 
## 如何构建技术产品化运营战略

### 构建基本策略

在上图的元模型中，我们定义了基本的模式。基于这个模式，我们可以扩展我们的策略，如下图所示：

![开源软件产品化运营策略](https://dts.plus/technology-product-marketing/opensource-comunnity.png)

它以 KOL（关键意见领袖） 和布道师构建了影响力的中心，模式也稍微有一些变化。随后，我们需要：

1. 定义我们在**社区**和**产品**上的目标
   - 以社区成员价值为出发点构建社区策略
	 - 以客户价值为出发点构建产品化策略
2. 完善每一步所需要的任务和阶段化目标。
3. 制定不同社区繁荣阶段的演进方案。
4. 持续迭代和优化方案。

其中最重要的是考虑对于社区的价值。

### 1. 构建影响力中心

在设计模型的时候，我考虑了几个不同的方案，最后定义为『构建影响力中心』。原因是，我们需要一种持续的机制来影响越多的人，也因此是一个影响力中心。

它可以是通过一定角色的人去影响社区，诸如于：

1. 开发者关系（DevRel）、技术布道师（Evangelist）。
2. 意见领袖（KOL）。

通过构建影响力中心，我们可以辐射到更多的人群上，从而达到更好的触达率。它的构建方式比较有意思，可以通过特别的岗位，如开发者关系去构建，进一步去带动 KOL 们的兴趣。

### 2. 构思社区文化，凝聚人心

当有越来越多的人参与到社区中时，我们就需要去构建社区如何构建？社区的文化又是如何的问题？我们在社区上，需要：

1. 以社区和成员价值为核心，产品第二。
2. 创造协作空间，实现个人价值。

作为一个开放式的社区，我们需要有自己的主题，有自己的价值宣言，并坚守它们。

与此同时，我们需要分析我们的目标用户，随后：

1. 提供**易于触达的访问路径**。诸如于，如果我们提供的是论坛，那么它应该易于访问；如果我们通过 IM 来通讯，它应该有一定的安装率。
2. 考虑**对于用户的个人价值**。他们是谁，它为什么要来到这个社区？

社区是向人们提供价值，而不是向利益相关者提供价值的。

### 3. 设计新手体验

开发者也是一个用户，为了吸引他们参与到项目中来。我们需要设计好新手的体验，以让他们能更快地上手到项目中。所以，我们视不同的情况，可能还需要：

1. 设计入门之旅 Onboarding Journey
2. 打造新手体验
3. 设计**开发者体验**指标
4. 提供、透明协作（如开放式管理等）

如果目标的新手成员不能快速参与到项目中，那么我们将流失大量的用户。

所以，这是实现转换率非常重要的一步。

### 4. 帮助客户创造价值

作为一个技术产品，它能吸引到开发者和用户的一大原因是，它能帮助我们创造价值。从创造客户的价值出发，而非售卖自己的产品，这个是非常重要的。

所以，我们需要去设计我们的提升计划，诸如于：

1. 构建第一个成功的案例。
2. 参与到客户产品的设计中。

视不同的产品，这里的差异会非常之大。

# 实践：文档体验设计

这一部分结合了对于文档代码化的理解和实践，并展开对于 Rust、Julia、Dart、Kotlin、Swift 等语言的文档研究（详细见：《[API 库的文档体系支持：主流编程语言的文档设计](https://www.phodal.com/blog/api-ducumentation-design-dsl-base/)》），重新思考了如何做了文档工程的开发者体验设计。

## 文档工程师的痛点

我尝试性的去梳理过去在编写文档的一些痛点，诸如于：

* 文档代码不同步。即文档的 API 变化可能落后于代码，导致 API 与文档出现不一致。
* 频繁的 API 变更。API 变更时，文档需要手动进行更新，不能自动化同步。
* 概念不统一。对于同一个概念，文档的不同地方描述不一致。
* 重复的文档块。文档需要重复引用某一部分的文档，不能像代码一样引用。
* 代码无法运行。按照文档的步骤下来编写的代码、复制的代码，是不能运行的。

还有一些问题，可能是难以通过自动化的方式来解决的，诸如于：

* 风格不一致。不同的人编写文档的风格不一致，可能需要类似于 code review 的 document review 的方式来解决。
* 语法不准确。使用的是不同形式的中文描述方式。（PS：难道是回去再上上语文课）

于是，我们可以尝试性地借用业内一些通用的方式来解决问题。

## 文档工程体验

再回到标题上，让我对标题做一些解释：

文档工程用于帮助我们指定、设计、和实施计算机技术相关的文档，如产品特定规格或详细说明，以及创建和使用它们的流程。它的特点是以“文档为中心”，以帮助我们构思和理解如何支撑其所在的商业模式。

而文档工程体验设计，则是围绕于构建和设计文档的过程进行的体验改善。即目标用户是**编写文档的工程师**，改善其编写文档的体验。并针对于文档的目标用户，改善他们在文档方面的体验（PS：这部分不是本文讨论的重点）。

文档体验是开发者体验的一个关键性因素，用于指导新手快速上手技术产品。在我们设计各类[开发者体验指标](https://www.phodal.com/blog/developer-experience/)时，一个非常重要的指标就是 TTFHW（Time to first hello world），即从零到第一个 Hello World 需要的时间，而这个指标是严重依赖于开发者文档。

因此，本文的意图是从文档开发者的体验出发，以重新塑造整体的开发者体验。

既然文档工程体验归属于开发者体验，它面向的是开发者提供更好体验，对于自身而言，更需要非凡的体验。只有以此为出发点，才能减小文档团队人员的流 动，毕竟不是程序员想写文档，也不是程序员都想看文档的。

## 卓越文档工程体验要素

作为一个程序员，我设计和参与过两个文档系统（Ledge 便是其中之一），它们之间有各自不同的思想。再结合我对于多个语言的文档体系的分析和设计，我觉得一个优秀的文档工程应该是满足这样的条件：

* 编辑-发布分离。架构设计上，编辑态和发布是完成分离的，各自可以使用不同的语言和技术来实现，诸如于使用 markdown 编写，但是输出可以是丰富多彩的形式。
* 过程自动化。特别好理解，它应该能实现快速的自动化发布，以代码开发保持一致和构建频繁。
* 文档形式化。XML 是上一个世代比较流行的文档形式化格式，从我的研究情况来看，定制化的 markdown  是这一个世代流行的方式。形式化的输入，它便意味着在输出上会有多种形式，如 markdown 结合 Pandoc 可以转换为 PDF、Word、HTML 等一系列的格式。
* 开放式协作。文档面向使用者开放修改，使用者可以通过 pull request 的形式来对文档进行改进，并可以针对文档提出建议。
* 版本化管理。在编辑态上，所有的历史修改都是可见的，可以回溯所有变更；在发布上，可以看到关键的历史版本，以适应不同人的需求。一种特别简单的示例，就是使用 git 来版本。
 
对于多数语言、框架的文档系统来说，它们都是面向特定领域定制的，以带来更好的编写体验和一致性。所以，从某种意义上来说，定制化开发也是非常重要的一点 —— 即我们往往难以获得一个通用的解决方案。

### 面向场景设计呈现

除了上述的要素之后，我们还需要提及一个非常重要的因素，即针对于不同的场景，应该要有不同的文档呈现形式。诸如于：

 - 一页文档。诸如于搭建指南，在项目初始化的时候，可以在一个网页内快速完成，而不需要进页面挑战。
 - 模块化文档。诸如于面向 API / SDK 场景下，以让每**部分** API 都可以独立访问，也能通过搜索引擎优化。
 - 可交互文档。诸如于编程语言 REPL、组件库场景下，让用户可以零成本学习和试用技术产品。
 - ……

尽管文档很重要，但是请不要忘了，我们的初衷是带来更好的用户体验。

## 文档模式

为了更方便于讨论，我尝试性对所接触的文章进行了模式上的分类，以及它们所适用的场景：

| 模式                | 场景                                         | 优点                         | 缺点                  | 一致性机制               | 原则                 | 
|---------------------|----------------------------------------------|------------------------------|-----------------------|--------------------------|----------------------|
| 文档代码化 | 需要协作的在线文档、侧重于开发指南编写       | 提升社区参与度、灵活扩展系统 | 实现成本略高          |                          | 以领域特定语言为核心 |
| 文档测试            | SDK、API 等功能性描述文档                    | 文档代码强一致性             | 实现成本略高          | 编译时保证               | 注释设计             |
| 可执行文档          | 文档为核心，代码为辅助、Demo 编写            | 轻量、文档一致性             | 大型工程比较难 handle | 编译时保证               | 文档优先             |
| 灵活代码块          | 代码为核心，文档为辅助、Demo 编写            | 动态响应代码变化             | 注释在 demo 代码中    | 代码正确编译，则文档正常 | 代码优先             |
| 测试即文档          | 业务系统开发，文档为核心，确保文档和代码一致 | 文档代码强一致性             | 实现成本略高          | 持续集成时保证           | 文档驱动开发         |
| 文档同构            | 文档驱动开发、业务系统开发                   | 文档代码强一致性             | 实现成本高            | 双向确保代码-文档一致    | 双向绑定             |

在文档工程这个上下文下，其详细的定义如下。

### 基础模式：文档代码化

定义：文档代码化是将文档以类代码的领域特定语言的方式编写，并借鉴软件开发的方式（如源码管理、部署）进行管理。 它可以借助于特定的工具进行编辑、预览、查看，又或者是通过专属的系统部署到服务器上。

示例：各类的开源软件文档、Rust、Julia 等编程语言的文档系统

文档代码化其中是现代化的文档工程里的基石。现有的开源软件文档体系，都是以 markdown + 开源的形式而展开的，所有的人都可以在这之上进行协作。除此，基于不同文档的需求，它们会在 DSL 的基础上进行扩展，如新一代的编程语言的文档系统。它们的方式是这样的：

1. 为扩展设计：文档 DSL
2. 为准确性设计：文档测试
3. 构建开放协作平台：开放协作

更详细可以参考：《[API 库的文档体系支持：主流编程语言的文档设计](https://www.phodal.com/blog/api-ducumentation-design-dsl-base/)》

### 文档测试：一致性

定义：文档测试的原始定义是，一种测试方式，用于确保系统的文档与系统的功能相匹配。在文档工程的上下文里， 我们定义为针对于文档中的代码验证其有效性，以及其结果的准确性。

示例：Rustdoc、DocumenterTools.jl

如在 Rustdoc 中**代码中的注释中的代码**会被提取出来，它会被独立编译，确保代码是可运行的。

```
  ```rust
assert_eq!(2 + 2, 4);
  ```
```

如下是 Rustdoc 中将上述的代码生成测试代码的测试用例：

```rust
fn main() {
   #[allow(non_snake_case)]
   fn _doctest_main__some_unique_name() {
       assert_eq!(2 + 2, 4);
   }
   _doctest_main__some_unique_name()
}
```

一旦上述的代码编译并运行通过，则说明文档中的注释是正确的。具体的步骤如下：

- 解析 markdown，寻找 Rust 语言的语法块（如果没有标注语言类型，默认是 Rust）
- 根据语法块，做一些简单的处理，生成可编译的代码
- 编译上述的测试代码 （如果编译失败，则说明测试失败）
- 运行这些测试 or 文档

详细见 Rustdoc 相关源码：[librustdoc](https://github.com/rust-lang/rust/tree/master/src/librustdoc)

### 可执行文档

定义：可执行文档是指文档本身已经是代码化的结果，它像代码一样可以执行， 并且可以将结果动态地与文档结合在一起。

示例：Julia 的 DocumenterTools、R Markdown、Exemd

在 R Markdown 里，它可以结合文档与 R 语言源码，可以进行动态的渲染。我们可以在 markdown 文件中，“随意”地调用 R 中的函数，并动态地嵌入数据、代码、计算结果、可视化图表等到输出的文档中。在结合了 Pandoc 之后，文档可以输出到所有主流的文档格式。如下的示例：

```markdown
    ```{r fig.show='animate', dev='jpeg', ffmpeg.format='gif'}
    for (i in 1:10) plot(runif(100), ylim = c(0, 1)) # for example
    ```
```

它将会运行并在文档中嵌入运行的结果。

### 灵活代码块

定义：灵活代码块是指文档可以通过 DSL 动态引用源码中的内容。

示例：DocumenterTools.jl、Forming 里的 Writing

以我设计的 Writing 为例，它可以动态解析 markdown 中设计的 Writing DSL，并从代码中读取对应的代码块。如下是 Writing 的示例：

```
// doc-code: file("src/lib.rs").line()[2, 5]
// 读取 "src/lib.rs" 文件的第 2 到第 5 行
// doc-section: file("src/lib.rs").section("section1")
// 读取 "src/lib.rs" 文件中的 section1 相关的代码块
```

通过简单的自定义函数，将文档与代码有机结合到一起。只要应用编译运行成功，那么文档本身也是正确的。

### 测试即文档

定义：测试即文档即指测试用例以文档的形式编写，文档本身就是测试用例。

示例：Cucumber 

相信大家都很“熟悉”了，主要是在自动化测试中使用非常广泛。Cucumber 示例如下：

```cucumber
# language: zh-CN
@math
功能: 加法
 加法计算器的验证用例

 @sanity
 场景: 两个数相加
   假如我已经在计算器里输入6
   而且我已经在计算器里输入7
   当我按"相加"按钮
   那么我应该在屏幕上看到的结果是13
```

测试是文档，文档即是测试。

### 文档同构（概念）

文档同构。[文档同构](https://www.phodal.com/blog/isomorphism-document/) 是一种将代码与文档保持一致的技术理念，它能读取格式化的文档，并将文档自动加入到代码中，如以注释的形式或者是只在 IDE 呈现；同时，还能将读取代码中的文档，自动更新到文档中，或是对文档进行测试和差异对比。

PS：我正在设计的一种方式，暂时没有 DEMO。

# 实践：错误处理（TBC）

# 实践：交互式设计（TBC）

# 实践：开发者关系（TBC）

这是两个岗位或者角色：

 - 开发者关系，主要是要与身为开发者的用户们建立起良好的关系。
 - 布道师， 将自己热爱与信仰的技术，持续不辍地传递。

对于以 SDK、云服务等为主的公司而言，他们都会通过这与之相似的岗位来建立与开发者的联系，从而提升开发者体验。

# 实践：开发者体验度量

## 示例：API 度量

 API 开发者体验度量指标：

| 错误呈现 | 文档体验 | 易用性 | 交互式 | 触点 | 支持 |
| --- | --- | --- | --- | --- | --- |
| 错误描述 | 开发者门户 | 一键式安装 | 低配置/零配置 | 文章 | 问题反馈渠道 |
| 报错即文档 | 发布日志 | 自动化版本迁移工具 | 声明式使用 | 演讲/分享 | 问题响应时间 |
| 报错即修改建议 | 代码生成文档 | 自助式搭建 | 可交互文档 | Hackathon | 开发者即服务 |
|   | 版本迁移指南 |   | 沙盒及产品环境 |   | 开发者社区 |

## 度量体系

### 度量驱动 

文档的度量本质上还可以使用开发者相关的指标进行度量，诸如于：

1. TTFHW，Time to first hello world 所花费的时间，是否存在改善。
2. PR 数 & Issue 数，适用于开源项目相关的文档，指在完善文档。随着文档的成熟，相关的内容应该越来越少。

从 API 相关的用户体验来说，它还可以是：

1. API 占比覆盖率。即通过文档测试等的方式，可以知道是否所有的 API 都有文档覆盖。
2. SEO 指标。即当开发人员从搜索引擎搜索时，是否能被搜索到？以及它在搜索引擎的排位？避免被乌龙。

还有一些不是那么易于衡量的：

1. 美观。这个很重要吗？？大概是吧
2. 易用性。这个怎么用指标衡量？

不过呢，线上的文档作为一个网站 ，常规的 Web 应用的指标也是适用的：文档访问速度等。

### 优化开发者体验

为了这个文档的概念完整性，我复制/粘贴了一些我司关于开发者体验优化相关的步骤：

1. 定义价值度量维度
2. 匹配用户旅程，细化维度至可量化的指标
3. 建立体验度量体系
4. 度量与诊断
5. 分析与体验提升 
6. 构建体验管理机制

从模式上来说，它和用户体验是极为相似的，同样的也是出于指标度量的维度来考虑问题的。

# 开发者体验反模式

## 反模式：开发者即服务

> 开发者即服务，是（Developer-as-a-Service）的简称，亦可称为 “按需即用的开发者”。即当开发者使用某一工具、库，遇到任何相关的问题，可以随时找开发者为我们提供服务。哪怕是使用者使用了我们的 A 框架，但是遇到 B 框架有问题，他/她们也会觉得 A 框架有问题 ——因为  A 框架的开发者们是一种服务，一种开箱即用的服务。

最近几年，我陆陆续续参与了一些公司的基础设施的开发和咨询。从组件框架、组件、平台到 IDE，各式各样的基础设施都有。作为一个参与者或者是负责人，我经历了一些辛酸的故事：要快速响应所有的问题、要提供贴身的技术支持……。所以，我决定写一篇文章来调侃一下使用者，并解释一下开发者的不易。

## 基础设施团队的挑战

每当有同事从我司离职时，我们通常的一个反应是，去的是技术为主的部门还是业务为主的部门。因为，从待遇上来说，技术部门和业务部门就是两个截然不同的存在。相同的月薪之下，业务部门可能会多个月的奖金，而技术部门这样的可能性极极极低。在这里我们简化一下这两个概念：

 - **技术部门**。组织中的技术支持部门，提供各种基础设施能力，如 DevOps 平台、框架、工具、组件库等。
 - **业务部门**。仍然是开发人员，只是围绕着业务构建应用的，如 Web 应用、APP 等。

值得注意的事，对于有些公司来说，这可能是三个组织：业务部门是纯粹的业务人员，不包含技术相关的东西；而技术部门是支持所有业务的一个大部分；同时，还会在技术部门内构建一个基础设施团队。

所以，在这里我们简化模型为：基础设施团队，即那些提供各种 平台、框架、工具、组件库等开发应用所需基础能力的团队。

作为基础设施团队的一员，我们可以发现项目中的一些挑战：

**挑战与收入不成正比**。我们所知道的市场的一个现状，作为一个基础设施团队：**有着极高的技术挑战**，**待遇不与之成正比**。当难度和收入没成正比时，基础设施部门的架构腐烂就非常快，不过这是另外一个故事了。

**过长与破碎的『售后』服务时间**。当开发的工具被越来越多的人使用时，我们就面临着需要随时支持他/她人的处境。这样一来，我们就不可避免地需要花费大量时间在支持开发者，并且我们的开发时间就会不断被打扰。如此一来，我们在做这事上的成就感就会越来越低。甚至于我们会觉得这是一项累赘。

**推广与 KPI 压力**。这个怕是众所周知的问题。不过呢，多数时候，团队需要换一个角度来考虑问题：其它团队使用框架时，能给自身真正地带来什么好处？

**提升开发者体验与成本的均衡**。提升开发者体验，就意味着我们要用更高的投入，换取一点点的更好的开发者体验。比如说，提供长期性的完整文档、交互性的 API 试用、友好的报错机制等等。

**缺少高水平开发人员**（潜在）。原因同上，收入与难度不能成正比时，容易导致招不到高水平的开发人员。同样的原因，也会导致另外一个问题，高水平的开发人员在项目中流失。对于一些大公司来说，这并非是问题。

**过高的生态建设期望**。我们经常指望组织内能有其他人为工具贡献代码。而这种期望往往是非常不现实的。一来，缺乏明显的奖励机制；二来，需要提升他们的能力。

## 开发者即服务

于是呢，在早期推广的时候，团队会为了更多人的使用，在模式上发生的一些变化。它会导致基础设施团队的开发人员变成了一种开箱即用的服务，就有了开头的定义。

> 开发者即服务，是（Developer-as-a-Service）的，亦可称为 “按需即用的开发者”。即当开发者使用某一工具、库，遇到任何相关的问题，可以随时找开发者为我们提供服务。哪怕是使用者使用了我们的 A 框架，但是遇到 B 框架有问题，他/她们也会觉得 A 框架有问题 ——因为  A 框架的开发者们是一种服务，一种开箱即用的服务。

在这种工作方式之下，会出现一些特定的服务模式：

 - 一对一的专属支持
 - 及时响应问题请求
 - 优先帮助开发者解决问题。即使判断不是工具的问题，还要给开发者一些方案。
 - ……

在些模式之上，开发者就好像一种随时可使用的服务。这和我们日常使用的 SAAS 服务一样，被期待开箱即用，被期待没有 bug。

## 解决方式

**尽可能的开箱即用**

繁琐的安装过程须完成各种的自动化。

**构建开发者社区**

让开发者帮助开发者，并赋予活跃的用户荣誉或利益，以此来促进生态的发展。

**详尽细致的文档**

作为服务的提供方，我们一直都有一个共识：开发者们不会看文档。以致于有些人走入一些误区，既然不没看，那我就写少一点。事实上，这是一个误区。

经常写作的人，会达成一种共识：**文章写给自己看的**，而文档也是写给自己用的。作为一个在社区上活跃的开发者，我经常看到别人的提问，于是我就从我的 800+ 的博客里找到一个链接，然后你懂的。

同理于，当我们作为一个基础设施团队服务时，使用者们不懂得也占多数，所以你只需要抛出一个链接即可。

## 缺失的关键角色

对于一个提供基础设施服务的团队来说，他/她们急需要一种方式来推广服务，并希望能获得反馈，以完善工具。

而在最近的几年里，在我经历了亚马逊、腾讯云、阿里云等公司的邀文之后 —— 它们需要在行业内有一定经验的云开发者，还需要有一定的写作和演进能力。我便意识到『**开发者关系**』将是一个非常稀缺的岗位 ——  市场上缺少这样的人才。与此同时，从来没有这样一个工作，它的要求高，但是它的工资确……。

### DevRel

我所说这个关键性角色便是，DevRel，即开发者关系（Developer Relations）。对于这个词，不同的公司有不同的岗位，还有一种相近的岗位是：开发者布道师。这个职位的产生便是国外的公司也有类似的痛点而导致的，它们都想要：

1. 维护开发者关系
2. 在社区进行宣传
3. 对社区进行支持、收集社区反馈
4. 建立连接内部的通道
5. 促进内部进行改进。

于是，便诞生了这么一个岗位。即要与代码打交道，而且还要与人打交道。

# 相关资料

开发者体验相关资料：

 - 《[Understanding a Path](https://toddmoy.com/sendgrid-journeymap)》
 - 《[APIMatic](https://www.apimatic.io/developer-experience-portal/)》 构建 Developer Experience Portal SAAS 服务
 - 《[Backstage](https://github.com/backstage/backstage)》 开源 Developer Portal 构建工具
 - 《活文档：与代码共同演进》如何让文档活起来
 - 《[How Mature Are You? A Developer Experience API Maturity Model](http://jennywanger.com/speaking/dx-maturity-model/)》

文档体验相关资料：

* [API 库的文档体系支持：主流编程语言的文档设计](https://www.phodal.com/blog/api-ducumentation-design-dsl-base/)
* [DocumenterTools](https://github.com/JuliaDocs/DocumenterTools.jl)
* [swift-doc](https://github.com/SwiftDocOrg/swift-doc)
* [Dokka](https://github.com/Kotlin/dokka/)
* [librustdoc](https://github.com/rust-lang/rust/tree/master/src/librustdoc)
* [数字技术战略：开发者体验 —— 内部工具的“最后一公里”](https://www.phodal.com/blog/developer-experience/)

## License

[![Phodal's Book](http://brand.phodal.com/shields/book-small.svg)](https://www.phodal.com/)

© 2020~2021 [Phodal Huang](https://www.phodal.com). This code is distributed under the Creative Commons Attribution-Noncommercial-No Derivative Works 3.0  License. See `LICENSE` in this directory.