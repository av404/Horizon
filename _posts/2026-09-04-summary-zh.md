---
layout: default
title: "Horizon Summary: 2026-09-04 (ZH)"
date: 2026-09-04
lang: zh
---

> 从 35 条内容中筛选出 7 条重要资讯。

---

**科技新闻**
1. [GPT-6 Astra 发布：基准亮眼但评测对比存在争议](#item-tech-news-1) ⭐️ 9.0/10
2. [借助 LLM 将 1993 年 Amiga 汇编游戏移植到 Godot](#item-tech-news-2) ⭐️ 8.0/10
3. [Audacity 4.0 发布：Qt6 全新 UI](#item-tech-news-3) ⭐️ 8.0/10
4. [美国政府意见书支持 OpenAI，主张 AI 训练属合理使用](#item-tech-news-4) ⭐️ 7.0/10
5. [微软将从 2026 年 10 月起默认启用 Win11 内存完整性保护](#item-tech-news-5) ⭐️ 7.0/10

**财经新闻**
1. [美政府考虑对进口芯片加征新一轮关税以推动制造业回流](#item-finance-news-1) ⭐️ 8.0/10
2. [韩国电力公社提议三星与 SK 海力士预缴约 184 亿美元电费建设电网](#item-finance-news-2) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [GPT-6 Astra 发布：基准亮眼但评测对比存在争议](https://openai.com/index/gpt-6-astra/) ⭐️ 9.0/10

OpenAI 发布了新版旗舰模型 GPT-6 Astra，并在部署安全页面提供了系统卡；Hacker News 上同时出现了关于该模型在 ARC-AGI-3 上表现以及其在 Artificial Analysis Coding Agent Index 取得进展的讨论。评论指出，ARC-AGI-3 的记分表容易误导，因为同一模型在使用 Responses API harness 时的估计得分约 30%，而表上却显示 GPT-5.6 Sol 为 7.8%，两套评测条件并不一致。另有观点认为，除 ARC-AGI-3 高分外，多数基准提升幅度与其他实验室的“点版本”更新相当，因此仍需等待细节来确认该模型在推理保留与压缩等环节上的真正水平。

hackernews · kibae · 9月3日 18:41 · [社区讨论](https://news.ycombinator.com/item?id=49554643)

**「背景」** GPT-6 Astra 是 OpenAI 于 2026 年发布的旗舰模型，接续 GPT-5 系列，OpenAI 称其为“世界上最有智能且最对齐的模型”，并同时发布了系统卡和多项基准测试数据。在 ARC-AGI-3 上得分约 99.9%，但评论指出该得分依赖特定响应 API 测试框架，而推理、逻辑等分类下的公开排名暂未单独列出。这属于 OpenAI 迭代式大版本更新的一部分，系统卡用于披露安全评测与部署评估。

**「影响」** 对依赖第三方基准比较模型能力的开发者和评测者，GPT-6 Astra 的发布提供了一个实际警示：若不同模型在 ARC-AGI-3 等任务上使用不同的 API 或 harness 评测，直接对比分数会产生误导。

**「社区讨论」** 社区中有评论对 GPT-6 Astra 在 ARC-AGI-3 上约 99.9% 的成绩感到惊艳，但也有评论认为该分数是在不同评测条件下取得的，不能与表中其他模型直接比较。还有用户指出演示频繁出现自主购买场景并不贴近真实需求，另有评论称前沿模型的进展仍更像技能习得而非通用智能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deploymentsafety.openai.com/gpt-6-astra">GPT - 6 Astra System Card - OpenAI Deployment Safety Hub</a></li>
<li><a href="https://thenewstack.io/openai-gpt6-astra-benchmarks/">OpenAI launches GPT - 6 Astra and says welcome to... - The New Stack</a></li>
<li><a href="https://benchlm.ai/models/gpt-6-astra">GPT - 6 Astra Benchmarks &amp; Pricing (September 2026)</a></li>

</ul>
</details>

**标签**: `#openai`, `#gpt-6`, `#large language models`, `#ai benchmarks`, `#ai safety`

---

<a id="item-tech-news-2"></a>
### [借助 LLM 将 1993 年 Amiga 汇编游戏移植到 Godot](https://babyloniantwins.com/blog/porting-a-1993-amiga-game-to-godot/) ⭐️ 8.0/10

一位 1993 年在巴格达用摩托罗拉 68000 汇编语言编写 Amiga 游戏的开发者，最近借助 Claude 在 Mac 上使用 vasm 反复汇编，直到生成二进制与其原始游戏逐字节一致，并在一个晚上完成了到 Godot 的可用移植。之后他又花了几周时间，把 33 年来对游戏构建方式的记忆、笔记和 git 仓库交给模型分析，并逐行编辑成文；最终调整游戏“手感”并正式发布又用掉几个周末和晚上。作者指出，原版使用 AsmOne 把代码汇编进内存，再从运行中的游戏内存保存成发布文件，因此原版二进制并非干净的汇编输出，导致与重新汇编结果存在约 108 字节的偏差。作者此次还介绍了由 LLM 阅读 68000 汇编并逐字节校验后迁移旧代码的工作流，同时免费放出原版 1993 年游戏。

hackernews · rabahs · 9月3日 14:28 · [社区讨论](https://news.ycombinator.com/item?id=49550375)

**「背景」** Amiga 是 1980 至 1990 年代流行的个人电脑平台，许多游戏使用底层摩托罗拉 68000 汇编语言编写，以榨取硬件性能；这类旧二进制通常没有现代源码工程，移植时往往要从汇编或反汇编重新理解逻辑。Godot 是目前开源的主流游戏引擎，适合承载被重写的游戏逻辑与表现层。文中的 vasm 是跨平台汇编器，AsmOne 则是 Amiga 时代的汇编环境，二者对代码生成的差异正是那 108 字节偏差的来源。

**「影响」** 这一案例说明，借助 LLM 和字节级一致性校验，旧平台汇编游戏可以被高效、可验证地迁移到现代引擎，为复古软件维护和游戏遗产保存提供了一条可行路径。

**「社区讨论」** 评论区普遍对这种“二进制考古”表示认可：有人把 ZX81 游戏内存转储交给 Claude 后成功转换成 Go 程序，也有人询问作者当年在资料匮乏时期的调试故事，并希望 Claude Code 能导出一份可复用的移植工程指南。另有读者表示正计划用相同方法移植另一款被遗忘的游戏。

**标签**: `#retrocomputing`, `#LLM code analysis`, `#game development`, `#Godot`, `#assembly porting`

---

<a id="item-tech-news-3"></a>
### [Audacity 4.0 发布：Qt6 全新 UI](https://github.com/audacity/audacity/releases/tag/Audacity-4.0.0) ⭐️ 8.0/10

Audacity 4.0（4.0.0）已作为这款广受欢迎的开源音频编辑器的主要版本在 GitHub 发布，最大变化是采用基于 Qt6 的全新用户界面，并伴随大量改进与修复。此次大版本升级对桌面录音与音频编辑用户群体意义重大，因为界面框架迁移到 Qt6 可能带来更现代的操作体验。不过，本次官方发布说明本身未提供完整变更明细，实际新增功能、兼容性限制和已知问题仍需查阅后续文档或实际测试确认。作为一款持续演进的成熟工具，这次发布更多属于渐进式升级而非范式转变。

hackernews · ClydeN · 9月3日 10:53 · [社区讨论](https://news.ycombinator.com/item?id=49548395)

**「背景」** Audacity 是一个广受欢迎的开源音频编辑器，历史上基于 wxWidgets 构建界面。Muse Group 收购 Audacity 后引入遥测功能，曾引发社区争议并催生了 Tenacity、Sneedacity 等分叉项目。Audacity 4.0 将界面迁移至 Qt6，复用 MuseScore Studio 4 的框架，同时保留旧版项目导入功能，并提供 Windows ASIO 支持。

**「社区讨论」** 讨论区的共识并不一致：有用户强烈推荐 Muse 软件主管的介绍视频，也有人分享官方发布的 Qt6 新界面演示；而部分 Linux 用户认为 Audacity 4.0 仍没有解决 JACK/Pipewire 缺少持久客户端等长期痛点，另有一些用户则担心遥测、audio.com 整合以及 Tenacity/Sneedacity 等分支的去向。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linuxcompatible.org/story/audacity-40-beta-4-ships-with-qt6-ui-windows-asio-and-legacy-imports">Audacity 4.0 Beta 4 Ships With Qt6 UI, Windows ASIO, and Legacy Imports</a></li>
<li><a href="https://www.phoronix.com/news/Audacity-4.0-Released">Audacity 4.0 Audio Editor Released With Qt6 Based UI - Phoronix</a></li>
<li><a href="https://www.theregister.com/software/2021/07/07/audacity-fork-maintainer-quits-after-alleged-harassment-by-4chan-losers-who-took-issue-with-tenacity-name/1461730">Audacity fork maintainer quits after alleged harassment by 4chan...</a></li>
<li><a href="https://butthurtfork.com/fork/tenacity">Tenacity — The Butthurt Fork</a></li>

</ul>
</details>

**标签**: `#audacity`, `#open-source`, `#audio-editing`, `#qt6`, `#release`

---

<a id="item-tech-news-4"></a>
### [美国政府意见书支持 OpenAI，主张 AI 训练属合理使用](https://www.reuters.com/legal/litigation/us-government-backs-openai-new-york-times-copyright-case-2026-09-02/) ⭐️ 7.0/10

美国政府向曼哈顿联邦法院提交了支持 OpenAI 的法律意见书，主张用受版权保护的内容训练大语言模型一般属于合理使用。这是美国政府首次在 AI 训练版权案件中正式表态，尽管意见书没有法律约束力，但可能增强科技公司应对类似诉讼的底气。《纽约时报》批评政府偏向少数万亿美元级 AI 公司而牺牲创作者权益；该报于 2023 年起诉 OpenAI 及微软擅自使用其数百万篇文章训练 ChatGPT。

telegram · zaihuapd · 9月3日 05:45

**「背景」** 美国版权法中的合理使用原则允许在某些条件下未经授权使用受版权保护的作品，例如用于评论、教学或研究，判断标准包括使用目的、作品性质、使用比例和市场影响。本案中，《纽约时报》指控 OpenAI 和微软未经许可利用其大量文章训练 ChatGPT，而 OpenAI 等公司认为这种训练方式属于合理使用。美国政府的意见书正是就此争议首次在诉讼中表明立场。

**「影响」** 这一表态虽无法律约束力，却标志着美国政府在 AI 版权争议中首次选边，可能增强 OpenAI 等技术公司的应诉底气。它也可能影响其他未决案件中对合理使用界限的论证，但法院最终是否采纳仍是未知数。

**标签**: `#AI`, `#copyright`, `#policy`, `#OpenAI`, `#legal`

---

<a id="item-tech-news-5"></a>
### [微软将从 2026 年 10 月起默认启用 Win11 内存完整性保护](https://techcommunity.microsoft.com/blog/windows-itpro-blog/expanding-memory-integrity-protection-across-windows-devices/4551984) ⭐️ 7.0/10

微软宣布自 2026 年 10 月 13 日“周二补丁日”起，对符合条件的 Windows 11 设备默认启用内存完整性保护（HVCI）。这项基于硬件虚拟化的功能会创建隔离环境，仅允许受信任的内核模式代码和驱动运行，从而降低恶意程序借底层驱动接管设备的风险。启用要求设备支持硬件虚拟化、UEFI 与 Secure Boot 等条件。旧驱动或不兼容驱动可能阻止该功能启用，极少数情况下可能导致蓝屏。

telegram · zaihuapd · 9月3日 06:09

**「背景」** 内存完整性保护（HVCI）是 Windows 基于虚拟化的安全功能，利用 CPU 的虚拟化能力隔离内核模式代码，仅允许符合签名策略的受信任驱动加载。它主要用于防御内核级恶意软件和驱动劫持攻击。此前该功能多为可选或部分设备预启，微软此次计划将其推广为更多 Windows 11 设备的默认安全基线。

**「影响」** 从 2026 年 10 月补丁日开始，使用兼容硬件的 Windows 11 设备将自动开启该保护，IT 管理员和安全团队需要提前验证驱动程序兼容性，以避免旧驱动或未签名驱动被阻止，甚至引发蓝屏。

**标签**: `#Windows 11`, `#HVCI`, `#Security`, `#Microsoft`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [美政府考虑对进口芯片加征新一轮关税以推动制造业回流](https://www.bloomberg.com/news/videos/2026-09-03/trump-to-levy-more-chip-tariffs-to-boost-manufacturing-video) ⭐️ 8.0/10

美国商务部长霍华德·卢特尼克表示，特朗普政府正考虑对进口半导体加征新一轮关税，以鼓励芯片制造回流美国；政府还倾向对在美国建设生产能力的企业提供关税减免。具体税率与实施时间尚未确定，措施仍在考虑阶段。

telegram · zaihuapd · 9月3日 07:00

**「背景」** 征税范围可能从芯片本身扩大至数据中心服务器、消费电子等含有半导体的进口产品。报道称，在台湾半导体展会现场，芯片供应链企业仍持乐观态度，因为美国市场的 AI 芯片需求强劲。

**标签**: `#semiconductors`, `#tariffs`, `#trade policy`, `#manufacturing`, `#AI supply chain`

---

<a id="item-finance-news-2"></a>
### [韩国电力公社提议三星与 SK 海力士预缴约 184 亿美元电费建设电网](https://mp.weixin.qq.com/s/HgZUrbwwGGGGBh1-qiyLFQ) ⭐️ 7.0/10

韩国电力公社提议，三星电子和 SK 海力士在未来五年合计预缴约 25 万亿韩元（约 184 亿美元）电费，用于建设半导体集群配套电网，其中三星约 147 亿美元、SK 海力士约 37 亿美元。该方案仍在研究中，具体利率、预缴金额与期限尚未敲定。

telegram · zaihuapd · 9月3日 12:01

**「背景」** 韩国电力公社是韩国主要的国有电力公司，目前负债规模较大，这使其寻求让大客户预缴电费来支撑电网投资。

**标签**: `#KEPCO`, `#Samsung`, `#SK Hynix`, `#semiconductor`, `#South Korea`

---