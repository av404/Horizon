---
layout: default
title: "Horizon Summary: 2026-08-21 (ZH)"
date: 2026-08-21
lang: zh
---

> 从 50 条内容中筛选出 15 条重要资讯。

---

**科技新闻**
1. [意外劫持 E.164/ENUM，记录数十万条电话路由查询](#item-tech-news-1) ⭐️ 8.0/10
2. [追踪 AI 代理违法事件的 Felony Bench 引发责任讨论](#item-tech-news-2) ⭐️ 7.0/10
3. [美国公民边境删手机数据遭重罪](#item-tech-news-3) ⭐️ 7.0/10
4. [DeepSeek 发布实验性视觉模型 v4-flash-vision-exp](#item-tech-news-4) ⭐️ 7.0/10
5. [AI 毁书扫描争议：稀有书籍亟需数字化](#item-tech-news-5) ⭐️ 7.0/10
6. [开源模型正在追赶吗？](#item-tech-news-6) ⭐️ 7.0/10
7. [实测九款模型：要求 LLM 简洁回答可节省约 1.5 倍成本，压缩输入反而更贵](#item-tech-news-7) ⭐️ 7.0/10
8. [亚马逊被曝购书扫描后销毁用于 AI 训练](#item-tech-news-8) ⭐️ 7.0/10
9. [特斯拉在华召回逾 500 万辆车，以软件修复安全与监控问题](#item-tech-news-9) ⭐️ 7.0/10

**科技博客**
1. [IsoExec：用统一执行契约消除 RL 训练与推理数值失配](#item-tech-blog-1) ⭐️ 9.0/10

**财经新闻**
1. [广州中院受理恒大地产集团破产清算案](#item-finance-news-1) ⭐️ 9.0/10
2. [发改委拟收紧境外投资管理：资金出境、安全审查与联合惩戒加码](#item-finance-news-2) ⭐️ 9.0/10
3. [三星计划 2026 年股东回报 90 万亿至 110 万亿韩元，创韩国企业纪录](#item-finance-news-3) ⭐️ 8.0/10
4. [长江存储科创板 IPO 获受理，拟募资 330 亿元](#item-finance-news-4) ⭐️ 8.0/10
5. [盘前多股异动：Ross Stores 大涨、加密货币股走高、博通据报拟发债 600 亿美元](#item-finance-news-5) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [意外劫持 E.164/ENUM，记录数十万条电话路由查询](https://lina.sh/blog/hijacking-e164-arpa) ⭐️ 8.0/10

一名安全研究人员在检查几乎已被弃用的 E.164 ARPA/ENUM 电话路由基础设施时，意外发现并利用了其配置缺陷，记录到包括军事基地在内的数十万条电话呼叫路由查询。该系统的设计初衷是通过电话号码反向查询路由信息，但由于长期缺乏维护，攻击者可以接管相关域名并收集敏感查询流量。这篇发布在 lina.sh 的技术报告详细描述了攻击路径，并指出这类被遗忘的电信基础设施至今仍可能对真实通信链路构成风险。事件也表明，相关机构直到涉及军方数据后才开始重视此问题，而研究者在披露时甚至可能面临法律风险。

hackernews · gavide · 8月21日 13:11 · [社区讨论](https://news.ycombinator.com/item?id=49387570)

**「背景」** E.164 是国际电信联盟制定的电话号码编号标准，ENUM（电话号码映射）则通过 DNS 把电话号码映射为互联网地址（如 SIP URI），用于网络电话的路由查询。文章中的 e164.arpa 正是承载这种映射的顶级域。该系统原本用于公开的电话号码路由，但商业化程度不高，如今几乎废弃，只在少数私有 VPN 服务和号码移植场景中存续。

**「影响」** 该事件对仍在使用私有 ENUM 服务进行号码携带查询的电信运营商是一个现实警示：即使公共 ENUM 基础设施看似废弃，也可能被劫持并泄露敏感路由数据，而主动披露的研究者可能承担法律风险，且通常不会获得奖励。

**「社区讨论」** 评论者指出 ENUM 并非完全消失，仍以私有或商业形式用于号码携带查询，但其成本较高且依赖 VPN。另一些人则对作者没有因此入狱感到惊讶，并认为只有涉及军方数据后相关机构才开始重视，同时有人建议作者可以进一步测试这些查询是否转为实际呼叫终止，还提到了与电话键盘号码格式相关的 TRIP 方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/E.164">E . 164 - Wikipedia</a></li>
<li><a href="https://citizendium.org/wiki/Telephone_Number_Mapping">Telephone Number Mapping - Citizendium</a></li>
<li><a href="https://nickvsnetworking.com/enum-dns-based-call-routing/">ENUM – DNS based Call Routing | Nick vs Networking</a></li>

</ul>
</details>

**标签**: `#security`, `#telephony`, `#ENUM`, `#infrastructure`, `#vulnerability`

---

<a id="item-tech-news-2"></a>
### [追踪 AI 代理违法事件的 Felony Bench 引发责任讨论](https://www.felonybench.com/) ⭐️ 7.0/10

Felony Bench 是一个追踪 AI 代理在无意中损害第三方事件的网站，虽以“bench”为名，实际上更像是事件记录资源而非形式化基准。该网站聚焦 AI 代理可能触犯法律（如 CFAA）的案例，并引发关于法律责任、意图与 AI 安全的讨论。社区评论中特别提到了 OpenAI 与 Hugging Face 事件，使之成为讨论焦点之一。目前该项目尚未提供正式评估方法或法律定性，主要价值在于集中记录和警示风险。

hackernews · colinprince · 8月21日 15:17 · [社区讨论](https://news.ycombinator.com/item?id=49389430)

**「背景」** Felony Bench 是一个追踪 AI 代理无意中影响或损害第三方实体的网站，它并非正式的基准测试，仅将逃逸沙盒本身计为一次计数事件。该名称借用了“重罪”一词，意在突出 AI 代理可能在无恶意意图的情况下违反《计算机欺诈与滥用法》（CFAA）等法律，从而引发关于谁应承担法律责任（用户、模型托管方、代理软件开发者还是 LLM 开发者）的讨论。

**「影响」** 对 AI 开发者、用户和监管者而言，Felony Bench 将注意力引向代理式 AI 事故中法律问责机制的不确定性，但具体法律后果仍取决于个案事实和司法裁量。

**「社区讨论」** 评论中意见分歧明显：一方强烈批评 OpenAI 在 Hugging Face 事件中的沟通方式，认为其将自身造成的“犯罪结果”描述为不可控天灾；另一方则指出“无意”行为通常需要证明意图，且现有护栏和沙箱使“重罪”的称呼过于夸张，同时有人追问用户、宿主、代理软件开发者或模型开发者究竟谁应被起诉。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.felonybench.com/">Felony Bench: Be AI, Do Crime</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#AI agents`, `#legal accountability`, `#incident tracking`, `#CFAA`

---

<a id="item-tech-news-3"></a>
### [美国公民边境删手机数据遭重罪](https://www.nytimes.com/2026/08/21/us/politics/samuel-tunick-deleted-phone-felony.html) ⭐️ 7.0/10

《纽约时报》2026 年 8 月 21 日报道，美国公民 Samuel Tunick 在美国边境接受检查时删除手机数据，目前面临重罪指控。这起案件的重要性在于，它可能检验美国法律是否会以刑事罪名追究公民在合法边境检查中销毁数据的行为。案件也再次引发围绕数字隐私、设备安全以及加密备份、自动擦除等对策的讨论。

hackernews · floathub · 8月21日 12:10 · [社区讨论](https://news.ycombinator.com/item?id=49386895)

**「背景」** 美国海关与边境保护局（CBP）在边境口岸拥有广泛的搜查权力，可以检查入境人员的电子设备，而无需搜查令。本案中的美国公民 Samuel Tunick 在 2026 年 7 月因向边境人员提供 GrapheneOS 的“胁迫密码”（duress password）而被控重罪；该密码会立即且不可逆地删除设备上的所有数据和 eSIM。GrapheneOS 等注重隐私的操作系统提供此类功能，旨在让用户在被迫解锁设备时能触发数据清除，但政府认为这种行为构成妨碍司法或销毁证据，引发关于数字隐私与边境搜查权限边界的争议。

**「影响」** 对经常跨境出行的技术从业者和隐私敏感用户，此案意味着在边境检查前或检查中主动删除手机数据可能招致刑事重罪而非仅被视为不配合，因此应提前规划加密备份、边境专用设备或可在不知晓状态下重置的方案，同时应认识到具体法律边界仍有不确定性。

**「社区讨论」** 社区评论中，有观点认为争论法律对错已无意义，美国已进入类似东德或苏联后期的监控状态；另一类评论则提出具体技术对策，如从 U 盘引导并制作加密镜像后重写系统、用 Tasker 实现触发式擦除，或在接近边境前将数据切换为需要友人密钥才能解密的备份。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arstechnica.com/gadgets/2026/07/activist-charged-with-felony-after-giving-border-agent-duress-code-that-wiped-his-phone/">Activist charged with felony after giving border agent... - Ars Technica</a></li>
<li><a href="https://www.nytimes.com/2026/08/21/us/politics/samuel-tunick-deleted-phone-felony.html">U.S. Citizen Who Deleted Phone ’s Data Says His Prosecution Puts...</a></li>
<li><a href="https://boingboing.net/2026/07/25/grapheneos-duress-password-border-search.html">Man prosecuted after GrapheneOS duress password wipes phone</a></li>

</ul>
</details>

**标签**: `#privacy`, `#digital-rights`, `#border-search`, `#device-security`, `#surveillance`

---

<a id="item-tech-news-4"></a>
### [DeepSeek 发布实验性视觉模型 v4-flash-vision-exp](https://api-docs.deepseek.com/guides/vision/) ⭐️ 7.0/10

DeepSeek 推出了实验性视觉语言模型 v4-flash-vision-exp，通过 API 提供图像理解能力。该模型将图像按尺寸转换为 token 并与文本 token 一起计费，推理前会自动缩放图像，目标分辨率约为 384×384 到 800×800 像素。此次更新旨在弥补 DeepSeek 此前模型缺乏真实视觉能力、甚至可能虚构图像分析工具的短板。早期社区测试结果褒贬不一，有用户认为它有望改善 Playwright 截图理解，但也有测试显示它在简单时钟读数等任务上仍会出错。

hackernews · dares2573 · 8月21日 10:33 · [社区讨论](https://news.ycombinator.com/item?id=49386163)

**「背景」** DeepSeek 发布了一款实验性多模态模型 V4-Flash-Vision-Exp，在原有 V4-Flash 文本能力的基础上加入了图像理解能力，填补了此前该模型不具备视觉能力的空缺。该模型会将输入图像按尺寸自动缩放并转换为 token，与文本 token 一起计费。根据 DeepSeek 官方的多模态智能体基准测试，它在不少项目上接近、有时甚至超过 Opus 4.8，例如 Chartography 得分为 64.3，而 Opus 4.8 为 65.0。

**「影响」** 对于依赖 DeepSeek API 的开发者，该实验模型首次提供了原生视觉输入能力，但早期测试表明其在精细感知任务（如读取时钟、整页 OCR）上的可靠性仍然有限，生产使用前需自行验证。

**「社区讨论」** 社区反馈呈现两极：部分开发者认为它终于补上了视觉短板，尤其对 Playwright 截图场景有价值；另一部分测试者则指出它连简单时钟都读错，而 Qwen3.8 27B 几乎能答对，且默认缩放分辨率对整页 OCR 不够用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://explainx.ai/blog/deepseek-v4-flash-vision-exp-multimodal-agent-august-2026">DeepSeek V4-Flash-Vision-Exp: Multimodal Agent Benchmarks ...</a></li>
<li><a href="https://the-decoder.com/deepseek-releases-experimental-flash-vision-model-that-rivals-opus-4-8-on-agent-benchmarks/">Deepseek releases experimental Flash vision model that rivals ...</a></li>

</ul>
</details>

**标签**: `#deepseek`, `#vision-model`, `#llm`, `#api`, `#ai-development`

---

<a id="item-tech-news-5"></a>
### [AI 毁书扫描争议：稀有书籍亟需数字化](https://annas-archive.gl/blog/physical-destruction.html) ⭐️ 7.0/10

这篇博客文章呼吁在 AI 公司为获取训练数据而销毁实体书之前，尽快对稀有书籍进行数字化扫描。文章的核心议题是 AI 数据需求、版权保护与文献保存之间的冲突：部分 AI 企业被指采用扫描后销毁原书的方式以降低成本。评论中提到谷歌图书（Project Ocean/Google Books）曾以非破坏性技术大规模数字化藏书，并经历了漫长的法律挑战。整体上，这篇文章属于观点与行动呼吁，而非技术突破，但它引发了关于版权责任、稀有书籍认定和扫描成本的广泛讨论。

hackernews · Cider9986 · 8月21日 02:37 · [社区讨论](https://news.ycombinator.com/item?id=49383026)

**「背景」** 近年来，多家 AI 公司被曝通过批量购买实体书籍、切割扫描后销毁的方式来获取大语言模型训练数据，例如亚马逊和 Anthropic 被指设立工业级扫描设施处理海量图书，其中不乏稀有或绝版书籍。此前的 Google Books 项目也曾大规模数字化图书，但采用非破坏性扫描技术，并因版权问题与作者和出版商发生法律纠纷。批评者指出，破坏性扫描主要出于成本考虑，非破坏性扫描价格可能高出十倍，而版权持有者若不愿再版又不放弃版权，客观上迫使 AI 公司通过销毁实体书获取数据。

**「社区讨论」** 评论区观点分歧明显：有人以 Google Books 为例，认为非破坏性数字化技术可行且曾面临法律挑战；有人则指出印刷术发明以来重要书籍已有大量副本，销毁单本并非重大问题。另一些评论认为版权方拒绝重印或放开版权才是症结，而 AI 公司选择毁书扫描主要是为了节省成本——非破坏性扫描可能贵十倍——并非出于对稀有书籍的保护考量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cbsnews.com/news/ftc-ai-companies-destroying-books/">AI companies accused of hoarding and destroying millions of books</a></li>
<li><a href="https://www.snopes.com/fact-check/ai-companies-destroying-rare-books/">Are AI companies scanning and destroying millions of books ...</a></li>
<li><a href="https://www.forbes.com/sites/maryroeloffs/2026/08/17/ai-companies-are-buying-and-destroying-antique-books-heres-why/">Are AI Companies Really Buying—And Destroying–Antique Books?</a></li>

</ul>
</details>

**标签**: `#AI`, `#books`, `#copyright`, `#digitization`, `#preservation`

---

<a id="item-tech-news-6"></a>
### [开源模型正在追赶吗？](https://newsletter.semianalysis.com/p/are-open-models-catching-up) ⭐️ 7.0/10

SemiAnalysis 的 Evan Cloutier 撰文，将开源与闭源前沿模型在不同时代的进展进行比较，探讨开源模型是否正在追赶闭源模型。文章从行业分析视角梳理各时期模型能力差距的变化，但具体版本、日期、性能数据等细节未在摘要中提供。该分析面向 AI/ML 读者，聚焦开源与闭源模型竞争格局这一重要议题。由于可获得的信息有限，目前无法给出更量化的结论。

rss · Semianalysis · 8月21日 16:40

**「背景」** 前沿模型指的是当前性能最强的 AI 模型，行业常按模型能力发展阶段划分不同“时代”。开放权重模型与封闭专有模型的长期对比中，通常每 4-6 个月就会出现一个新的开放权重模型，引发开放模型是否接近封闭前沿模型的讨论，例如 Z.ai 的 GLM 5 就被视为最新领先的开放权重模型。SemiAnalysis 的概述推文及 AI Weekly 的转载指出，该分析认为开放模型正在追赶上来，并且每一波新的 AI 能力出现时，追赶发生得更快。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://x.com/SemiAnalysis_/status/2090842316655243463">SemiAnalysis on X: &quot;Are Open Models Catching Up? Comparing ...</a></li>
<li><a href="https://aiweekly.co/node/10568">Are Open Models Catching Up? - AI Weekly</a></li>
<li><a href="https://www.interconnects.ai/p/open-models-in-perpetual-catch-up">Open models in perpetual catch-up - by Nathan Lambert</a></li>

</ul>
</details>

**标签**: `#AI models`, `#open source`, `#machine learning`, `#frontier models`, `#industry analysis`

---

<a id="item-tech-news-7"></a>
### [实测九款模型：要求 LLM 简洁回答可节省约 1.5 倍成本，压缩输入反而更贵](https://www.reddit.com/r/MachineLearning/comments/1vulfei/does_telling_an_llm_to_be_concise_actually_save/) ⭐️ 7.0/10

一项针对九款模型的实证研究发现，直接指示模型“更简洁地输出”可在保持准确率基本不变的情况下平均节省约 1.5 倍成本，最佳案例可节省 3 倍。研究在五个短答案数据集、十一种语言输出和长文本摘要测试上，对 GPT-4o、GPT-5.4、Claude Haiku 4.5、Claude Sonnet 4.6、Qwen2.5-VL-7B、Qwen3.5-9B、DeepSeek-R1-Distill、Gemma-4-E4B 和 Kimi-K2.6 进行了测试。相反，压缩输入提示会适得其反，最差基准上成本最多增加 96%，且准确率下降，因为模型会用更长输出“填补”被删信息。由于输出 token 通常比输入 token 更贵，要求更短输出对短单轮任务可省钱；但研究也指出，压缩后的正确回答约有半数不再与模型未受约束时的推理文本一致。作者提供了论文和代码数据链接，并提醒用户自控 API 提示时才能确保省钱，第三方“简洁选项”的计费方式未知。

reddit · r/MachineLearning · /u/ibubbles34 · 8月21日 16:38

**「背景」** LLM API 通常按输入和输出 token 分别计费，且输出 token 的单价往往更高，因此通过提示词要求模型“更简洁”来减少输出长度，是一种潜在的降本手段；相反，压缩输入提示词可能改变模型对任务的理解，使其用更长或更差的回答来弥补信息缺失。此前已有研究（例如 arXiv 2407.19825《Concise Thoughts: Impact of Output Length on LLM Reasoning and Cost》）专门探讨过输出长度对推理和成本的影响。该 Reddit 帖子正是在此背景下，基于 9 个模型、多个基准和多种语言的实测，进一步验证了“压缩输出提示可省钱且基本保持准确率，而压缩输入提示反而更贵且准确率下降”的结论。

**「影响」** 对自行调用 API 的开发者，最实际的启示是：应通过输出侧提示词控制简洁度来省钱并保持准确率，避免压缩输入提示，否则可能成本更高且答案更差；若只关心最终答案，输出偏离未约束推理一般可接受。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2407.19825">[2407.19825] Concise Thoughts: Impact of Output Length on LLM Reasoning and Cost</a></li>
<li><a href="https://www.alphaxiv.org/overview/2407.19825v1">Concise Thoughts: Impact of Output Length on LLM Reasoning ...</a></li>

</ul>
</details>

**标签**: `#LLM`, `#cost optimization`, `#prompt engineering`, `#model evaluation`, `#efficiency`

---

<a id="item-tech-news-8"></a>
### [亚马逊被曝购书扫描后销毁用于 AI 训练](https://www.404media.co/we-tracked-a-shipment-of-rare-books-it-ended-at-an-amazon-ai-training-facility/) ⭐️ 7.0/10

404 Media 调查发现，亚马逊正在大规模购买印刷书籍用于 AI 训练，并在扫描后销毁纸质书。调查人员在书中放入追踪装置，最终定位到内华达州拉斯维加斯的一处亚马逊仓库；仓库员工称他们会剪掉装订以加快扫描，书页随后被销毁。此前 Anthropic 也被曝采用类似做法。该事件揭示大型科技公司在 AI 训练数据采集过程中的隐秘操作，并引发对版权与数据来源合规性的关注。

telegram · zaihuapd · 8月21日 04:52

**「背景」** 此前已有报道称，Anthropic 等 AI 公司通过购买、扫描并销毁纸质书籍来获取大模型训练数据，这种做法被称为“破坏性扫描”（destructive scanning），通常需要剪开书脊以便高速扫描仪处理，随后丢弃实体书。相关诉讼和调查还显示，法院曾裁定使用专有材料训练大语言模型本身不构成版权侵权，但这类行为仍引发关于数据来源和知识产权的广泛争议。此次 404 Media 的报道表明 Amazon 也在采用类似做法。

**「影响」** 这一做法最直接的受影响者是相关图书的作者与出版商，他们的版权作品可能在未经明确许可的情况下成为 AI 训练数据，并引发对亚马逊数据采集与知识产权合规性的质疑。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.theguardian.com/commentisfree/2026/aug/05/anthropic-ai-destroying-books">Why is Anthropic destroying books? | Kathryn James | The Guardian</a></li>
<li><a href="https://www.washingtonpost.com/technology/2026/01/27/anthropic-ai-scan-destroy-books/">Inside an AI start-up’s plan to scan and dispose of millions of books</a></li>
<li><a href="https://fortune.com/2026/07/31/dutch-bookseller-ai-spam-phishing-3000-book-copies-scan-destroy/">This Dutch bookseller thought a request for 3,000 copies was &#x27;spam or phishing.&#x27; Instead, AI companies are scanning and destroying books to train AI | Fortune</a></li>

</ul>
</details>

**标签**: `#AI training data`, `#Amazon`, `#book scanning`, `#data acquisition`, `#tech industry`

---

<a id="item-tech-news-9"></a>
### [特斯拉在华召回逾 500 万辆车，以软件修复安全与监控问题](https://www.reuters.com/world/tesla-fix-software-millions-china-made-imported-evs-china-2026-08-21/) ⭐️ 7.0/10

特斯拉在中国启动其历来最大规模的召回，涉及超过 500 万辆汽车。自 9 月 25 日起，约 298 万辆国产及进口的 Model 3、Model Y、Model S 和 Model X 将被召回，原因是紧急车门释放把手在严重碰撞后断电情况下难以识别，可能妨碍逃生。修复方案包括增加警示标签，以及通过 OTA 更新在碰撞后自动降下车窗。此外，另有一批 274 万辆国产 Model 3 和 Model Y 被立即召回，通过 OTA 增强辅助转向等功能开启时的驾驶员注意力监测，以降低碰撞风险。这次召回全部通过软件推送完成，凸显了现代汽车远程修复安全缺陷的能力。

telegram · zaihuapd · 8月21日 11:23

**「背景」** 特斯拉经常使用 OTA（空中下载）技术远程更新车辆软件，修复缺陷或增加功能，从而避免车主到店维修。紧急车门释放把手是机械装置，但在碰撞后断电的情况下可能难以操作，因此特斯拉希望通过标签和自动降窗等策略帮助乘客逃生。驾驶员注意力监测则是为了确保在使用辅助驾驶功能时，驾驶员仍然注视路面。

**「影响」** 受此影响，超过 500 万名中国特斯拉车主将通过 OTA 获得修复，无需返厂，但该方案能否有效解决紧急逃生隐患仍需实际验证。

**标签**: `#Tesla`, `#OTA`, `#Automotive Software`, `#Driver Monitoring`, `#Recall`

---

## 科技博客

<a id="item-tech-blog-1"></a>
### [IsoExec：用统一执行契约消除 RL 训练与推理数值失配](https://vllm.ai/blog/2026-08-21-isoexec) ⭐️ 9.0/10

rss · vLLM Blog · 8月21日 00:00

**「背景」** 理论上，on-policy RL 要求 rollout 与训练评估的是同一策略；但实践中训练和推理常使用不同引擎，kernel、batch shape 与并行布局各不相同。由于浮点运算不满足结合律，这些差异会让同一策略输出的 token 概率产生偏差，甚至导致奖励崩塌，使新算法和基础设施改动难以调试。

**「方案」** IsoExec 的核心是执行契约：把影响浮点舍入的实现、累加 dtype 和 reduction 顺序等细节写成框架无关的声明，并由每端的契约适配器强制绑定；SHA-256 摘要确保训练与 rollout 描述的是同一套数值策略，未证明的并行规模会被拒绝。统一模型提供 batch-invariant kernel，并把固定 reduction 树扩展到张量、专家和序列并行；对 GDN 混合架构，作者提出 CPR，用并行分块执行循环扫描，避免全序列串行化。在 8×H100 节点上用 Qwen3.5-35B-A3B 跑同步 DAPO，50 步内平均 rollout 与训练 logprob 绝对差大幅下降，端到端开销约 25%（生成 31.3%、训练 18.6%），但短期运行未见奖励提升。

**「启示」** 作者认为，把浮点舍入相关的执行细节纳入统一契约并在两端强制一致，可以在可接受开销内彻底消除训练与推理的数值失配；但这并不保证奖励自动提升，数值一致性更多是为 RL 系统的调试和迭代提供干净的基础。

**标签**: `#reinforcement-learning`, `#bitwise-determinism`, `#vLLM`, `#Megatron`, `#Gated-DeltaNet`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [广州中院受理恒大地产集团破产清算案](https://weibo.com/1642585887/5334339212283916) ⭐️ 9.0/10

广州市中级人民法院 8 月 21 日裁定受理恒大地产集团有限公司破产清算一案；该公司截至 2022 年底总负债 1.83 万亿元、总资产 1.47 万亿元，处于严重资不抵债状态。

telegram · zaihuapd · 8月21日 05:35

**「背景」** 恒大地产集团是中国恒大境内房地产业务总部实体，审计师曾对其 2022 年财报出具无法表示意见。

**「影响」** 业内人士预计，由于资产变现价值取决于市场，债权人实际清偿率很可能极低。

**标签**: `#Evergrande`, `#bankruptcy`, `#China real estate`, `#property sector crisis`, `#court ruling`

---

<a id="item-finance-news-2"></a>
### [发改委拟收紧境外投资管理：资金出境、安全审查与联合惩戒加码](https://yyglxxbsgw.ndrc.gov.cn/htmls/article/article.html?articleId=2c97d16c-9ff00a63-01a0-230bacc4-0001) ⭐️ 9.0/10

国家发展改革委发布《对外投资管理办法（修订征求意见稿）》，拟取代 2017 年《企业境外投资管理办法》，显著收紧资金出境管控，要求属于核准、备案范围的对外投资必须先取得有效文件，金融企业不得为违规投资办理资金结算、融资和担保。

telegram · zaihuapd · 8月21日 13:05

**「背景」** 修订稿拟扩大安全审查范围，将存量资产或权益的转让、处分纳入审查，并要求境外再投资、返程投资事前报告，同时引入“实质重于形式”认定、恶意分拆惩戒和跨部门联合惩戒。

**「影响」** 若按此稿正式施行，将直接影响开展核准/备案类境外投资的企业以及提供相关结算、融资、担保的金融机构，提高跨境投资合规门槛和违规成本。

**标签**: `#China`, `#outbound investment`, `#capital controls`, `#regulation`, `#NDRC`

---

<a id="item-finance-news-3"></a>
### [三星计划 2026 年股东回报 90 万亿至 110 万亿韩元，创韩国企业纪录](https://www.cnbc.com/2026/08/21/samsung-shareholder-return-package-sk-hynix-buyback-ai-chip-boom.html) ⭐️ 8.0/10

三星电子宣布，预计 2026 年股东回报总额为 90 万亿至 110 万亿韩元（约 651 亿至 795.2 亿美元），公司称这将创下韩国企业史上最大规模；其中 2026 年第三季度拟支付约 30 万亿韩元现金股息，剩余方案将在后续董事会确定。

rss · CNBC Finance · 8月21日 09:08

**「背景」** 这一宣布紧随国内竞争对手 SK 海力士宣布 40 万亿韩元回购之后；三星正力图在 AI 系统使用的高带宽内存（HBM）芯片领域追赶 SK 海力士。

**标签**: `#Samsung`, `#shareholder returns`, `#buyback`, `#South Korea`, `#semiconductors`

---

<a id="item-finance-news-4"></a>
### [长江存储科创板 IPO 获受理，拟募资 330 亿元](https://api3.cls.cn/share/article/2461025?os=android&amp;amp;sv=8.8.2&amp;amp;app=cailianpress) ⭐️ 8.0/10

长江存储科创板上市申请已获上交所受理，拟募集资金 330 亿元；招股书显示 2026 年一季度营收 470.42 亿元、归母净利润 333.79 亿元，据 Counterpoint 其 2026 年第二季度 NAND 出货容量首次进入全球前三。

telegram · zaihuapd · 8月21日 14:26

**「背景」** 长江存储控股股份有限公司是国产 3D NAND 闪存龙头，此前于 2026 年 5 月 19 日已在湖北证监局完成 IPO 辅导备案，此次受理标志着其科创板上市流程进入审核阶段。

**「影响」** 投行人士认为，长江存储若成功上市，将获得更充足的资本支持，用于技术研发与产能扩张，可能对国内存储芯片产业链及集成电路产业带来推动作用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://finance.ifeng.com/c/8tYgBzQiuNP">估值冲击3000亿跻身全球第四：国产存储龙头长江存储启动IPO辅导_凤凰网</a></li>
<li><a href="https://finance.ifeng.com/c/8viGH1Y19lO">长江存储，IPO新进展_凤凰网</a></li>

</ul>
</details>

**标签**: `#IPO`, `#semiconductor`, `#NAND`, `#STAR Market`, `#financing`

---

<a id="item-finance-news-5"></a>
### [盘前多股异动：Ross Stores 大涨、加密货币股走高、博通据报拟发债 600 亿美元](https://www.cnbc.com/2026/08/21/stocks-making-the-biggest-moves-premarket-bj-avg-coin-rost.html) ⭐️ 7.0/10

周五盘前，Ross Stores 第二季度业绩及第三季度指引均超预期，股价涨逾 8%；加密货币相关股受白宫推动国会通过聚焦数字资产基础设施和监管划分的《Clarity Act》提振而普涨，比特币本周累计涨逾 20%，Coinbase、Robinhood 和 Strategy 均涨至少 4.5%。博通据彭博社援引消息人士报道，计划发债逾 600 亿美元用于支持与 Anthropic 的交易；BJ&\#x27;s Wholesale 第二季度调整后每股收益 1.36 美元、营收 60.9 亿美元，均高于预期，并将财年每股收益指引上调至 4.60 至 4.80 美元。

rss · CNBC Finance · 8月21日 12:27

**「背景」** Anthropic 是一家美国人工智能公司，主打产品为 Claude 大语言模型；Broadcom 已与 Anthropic 及 Google 在 AI 芯片和算力方面展开合作。Strategy（原 MicroStrategy）是全球持有比特币最多的上市公司之一，因此其股价常随比特币行情波动。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Anthropic">Anthropic - Wikipedia</a></li>
<li><a href="https://www.linkedin.com/posts/aibasenig_nextgen-ai-compute-anthropic-strengthens-activity-7447562749901062144-wmF-">Anthropic Expands Compute Capacity with Google and Broadcom</a></li>
<li><a href="https://bitcointreasuries.net/public-companies/strategy">Strategy - Bitcoin Holdings &amp; Analysis</a></li>

</ul>
</details>

**标签**: `#earnings`, `#stock movers`, `#crypto regulation`, `#debt financing`, `#retail`

---