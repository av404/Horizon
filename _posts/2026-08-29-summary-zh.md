---
layout: default
title: "Horizon Summary: 2026-08-29 (ZH)"
date: 2026-08-29
lang: zh
---

> 从 35 条内容中筛选出 14 条重要资讯。

---

**科技新闻**
1. [GLM-5.3 开源：后训练带来编程与防御能力跃升](#item-tech-news-1) ⭐️ 9.0/10
2. [Triton 3.8.0 发布：新增聚合类型、topk 降序与后端增强](#item-tech-news-2) ⭐️ 8.0/10
3. [Htmx 4.0 发布：超媒体 UI 库带来 Alpine.js 兼容性等新特性](#item-tech-news-3) ⭐️ 8.0/10
4. [一条漏洞传闻就足以让 AI 代理快速找到漏洞](#item-tech-news-4) ⭐️ 8.0/10
5. [美国制裁 Autistici/Inventati 引发基础设施担忧](#item-tech-news-5) ⭐️ 7.0/10
6. [开发者在 RP2350 上实现微型潜流 Transformer 人脸图像生成](#item-tech-news-6) ⭐️ 7.0/10
7. [腾讯混元发布 Hy4 preview](#item-tech-news-7) ⭐️ 7.0/10
8. [美国 FTC 调查 YouTube 封号政策，或面临诉讼](#item-tech-news-8) ⭐️ 7.0/10
9. [OpenAI 因 SpaceX 收购终止与 Cursor 合作](#item-tech-news-9) ⭐️ 7.0/10

**财经新闻**
1. [玉米和小麦期货创逾三年新高](#item-finance-news-1) ⭐️ 8.0/10
2. [美上诉法院：体育赛事事件合约不属于联邦监管互换，可能上诉至最高法院](#item-finance-news-2) ⭐️ 8.0/10
3. [两部门将个人住房贷款期限上限延长至 40 年](#item-finance-news-3) ⭐️ 8.0/10
4. [美联储 9 月加息概率因沃什讲话上升，市场预期接近对半](#item-finance-news-4) ⭐️ 7.0/10
5. [美股盘前异动：PayPal 大跌，Affirm 与 Gap 上涨，多家科技股因财报波动](#item-finance-news-5) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [GLM-5.3 开源：后训练带来编程与防御能力跃升](https://huggingface.co/zai-org/GLM-5.3) ⭐️ 9.0/10

智谱 AI（Z.ai）发布开源权重模型 GLM-5.3，权重已开放下载、运行和定制，官方博客和 Hugging Face 页面同步上线。该模型与 GLM-5.2 共用同一基础模型，全部能力提升来自后训练，重点强化智能体编程与网络防御等场景；官方给出的 Terminal Bench 2.1 得分 88.2、DeepSWE 得分 66.9，均大幅领先 GLM-5.2。许可证为自定义 GLM-5.3 License，个人与中小企业可自由使用、微调与商用，但针对连续 12 个月营收超 100 亿美元且对外提供模型服务的大型企业设有额外限制（原文未完整列出）。社区反馈认为它在自托管和商业部署中具有实用价值，性能接近或达到闭源高端模型水平，因此对开源大模型格局有重要意义。

hackernews · jeudesprits · 8月28日 15:20 · [社区讨论](https://news.ycombinator.com/item?id=49479878)

**「背景」** GLM 是智谱 AI（Z.ai）开发的大语言模型系列。GLM-5.3 于 2026 年 8 月 14 日以开放权重形式发布，与 GLM-5.2 共享同一个基础模型，全部提升来自后训练，重点增强智能体编程与网络防御等场景，并支持个人与中小企业自由使用、微调和商用。其权重可开放下载、运行和定制，采用自定义的 GLM-5.3 License，但对大型企业的商用范围设有营收条件。

**「影响」** 开发者和企业现在可以下载、微调并商用 GLM-5.3，在自托管环境中获得接近高端闭源模型的推理与编程能力；不过大企业商用前需确认自定义许可证的额外限制。

**「社区讨论」** 社区普遍认可 GLM-5.3 的推理直觉和综合表现，用户称其能处理 DeepSeek Flash 等模型难以解决的难题，并在实际使用中“最像 Opus 4.8”；也有用户指出它比 Kimi 略弱但更易运行，且相比 Qwen3.8、GLM 5.2 等中文模型在复杂数据分析任务中“过度思考”更少，token 效率更好。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GLM_%28AI%29">GLM (AI) - Wikipedia</a></li>
<li><a href="https://github.com/zai-org/GLM-5">GitHub - zai-org/GLM-5: GLM-5: From Vibe Coding to Agentic Engineering · GitHub</a></li>

</ul>
</details>

**标签**: `#open-source`, `#LLM`, `#GLM`, `#AI`, `#HuggingFace`

---

<a id="item-tech-news-2"></a>
### [Triton 3.8.0 发布：新增聚合类型、topk 降序与后端增强](https://github.com/triton-lang/triton/releases/tag/v3.8.0) ⭐️ 8.0/10

Triton 3.8.0 发布，主要新增公共聚合类型 API（@triton.aggregate 和 @gluon.aggregate，支持继承字段、默认值、不可变实例和 aggregate\_replace\(\)），并为 tl.topk 增加 descending 参数以支持返回最小值；编译器与后端改进包括多 CTA/TMA 支持、布局转换修复、确定性 JIT 缓存键、Python 3.14 注解兼容性，以及针对 AMD gfx1250/CDNA5 的 TDM、WMMA 和原子操作增强；同时引入了 FpSan、GSan、ConSan 等调试与验证工具，覆盖 NVIDIA 和 AMD 目标。

github · warrendeng · 8月28日 18:25

**「背景」** Triton 是一个开源的、基于 Python 的 GPU 并行编程语言与编译器，用于编写自定义深度学习内核，目标是让没有 CUDA 经验的开发者也能高效编写 GPU 代码。该项目最初由 OpenAI 于 2021 年以 Triton 1.0 发布，现由 triton-lang 组织维护，并在 AI/ML 生态中被广泛使用。本次 v3.8.0 发布属于该项目的常规版本更新，主要面向 GPU 内核开发者和编译器研究人员。

**「影响」** 使用 Triton 的开发者和 AI/ML 工程师现在可直接使用聚合类型与 tl.topk\(descending=False\) 编写更简洁的内核，并借助 FpSan/GSan/ConSan 检查浮点一致性、数据竞争和并发错误，同时 AMD gfx1250/CDNA5 用户可获得更完整的 TDM 与 WMMA 支持。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://triton-lang.org/main/index.html">Welcome to Triton’s documentation! — Triton documentation</a></li>
<li><a href="https://github.com/triton-lang/triton">GitHub - triton-lang/triton: Development repository for the ...</a></li>
<li><a href="https://openai.com/index/triton/">Introducing Triton: Open-source GPU programming for neural ...</a></li>

</ul>
</details>

**标签**: `#Triton`, `#GPU`, `#compiler`, `#AI/ML`, `#release`

---

<a id="item-tech-news-3"></a>
### [Htmx 4.0 发布：超媒体 UI 库带来 Alpine.js 兼容性等新特性](https://four.htmx.org/announcements/2026-08-28-htmx-4.0.0-is-released) ⭐️ 8.0/10

Htmx 4.0 已发布，这是面向超媒体（hypermedia）的 Web UI 库的一个重大版本更新。新版带来了包括 Alpine.js 兼容性在内的新功能，并在开发者社区中引发了大量讨论。该版本延续了 htmx 以 HTML 片段和服务器驱动交互为核心的设计理念，具体变更内容仍需查看官方公告。此次发布也获得了不少支持者的好评，他们认为它保持了简单性并减少了前端复杂度。

hackernews · rmsaksida · 8月28日 13:28 · [社区讨论](https://news.ycombinator.com/item?id=49478178)

**「背景」** htmx 是一个基于超媒体理念的前端 JavaScript 库，允许开发者通过在 HTML 中使用属性（如 hx-get）直接发起 AJAX 请求、更新页面片段，从而避免编写大量前端 JavaScript。htmx 4.0 是其重大版本发布，重点重构了内部实现，转向基于 fetch\(\) 的机制，并新增了与 Alpine.js 的兼容层（hx-alpine-compat），官方同时提供了从 htmx 2 迁移到 4.x 的升级指南。

**「影响」** 对 htmx 用户而言，4.0 版本提供的新特性（如 Alpine.js 兼容性）可能让超媒体方案与现有基于 Alpine.js 的项目更好地协同，但该版本是否值得升级还需结合具体项目架构评估。

**「社区讨论」** 社区反应总体积极，许多开发者称赞其简洁性并用于实际项目。也有人提出不同看法，认为在前后端分离架构下 htmx 会增加复杂度，或建议更小的替代方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://four.htmx.org/announcements/2026-08-28-htmx-4.0.0-is-released">htmx 4 . 0 . 0 has been released ! ~ htmx</a></li>
<li><a href="https://web.archive.org/web/20251103222343/https://htmx.org/essays/the-fetchening/">htmx ~ The fetch() ening</a></li>

</ul>
</details>

**标签**: `#htmx`, `#web development`, `#open source`, `#javascript`, `#hypermedia`

---

<a id="item-tech-news-4"></a>
### [一条漏洞传闻就足以让 AI 代理快速找到漏洞](https://simonwillison.net/2026/Aug/28/just-a-rumour-of-a-bug/) ⭐️ 8.0/10

剑桥大学计算机科学教授、OCaml 核心维护者 Anil Madhavapeddy 报告称，安全补丁讨论发布后约十分钟，项目网站就遭到百分号编码路径遍历探测，显示 AI 代理正监控公共仓库并迅速利用漏洞线索。他指出现代编码代理已能仅凭最轻微提示找到缺陷，并用自己的代理演示了这一点，在 Claude Fable 拒绝后改用了 DeepSeek V4 Pro。rclone 维护者 Nick Craig-Wood 在 Hacker News 证实，项目前 10 年约收到 20 份安全披露，而最近一个月超过 40 份，其中约 75%含有需要处理的问题；GitHub 的 CVE 分配也从 2-3 天延迟到 3-4 周，导致发布版本需带上 CVE-PENDING。这一速度使现有开源安全保密流程显得过时，需要为社区设计新的安全流程。

rss · Simon Willison · 8月28日 22:12

**「背景」** 传统开源安全披露通常先私下修复再公开发布，给维护者数天时间准备补丁。现在 AI 编码代理可以阅读公开的补丁讨论或提交信息，在几分钟内自动推测并验证漏洞利用方式，使原有的保密窗口几乎失效。

**「影响」** 对维护者和开源项目而言，安全披露必须默认按“即刻可利用”处理，否则可能在修复完成前就被 AI 代理利用。GitHub CVE 分配延迟也进一步加重了维护者负担，迫使他们以 CVE-PENDING 名义发布点版本。

**「社区讨论」** Hacker News 评论者基本认同威胁真实存在，但看法有分歧：有开发者认为管理层的“求快”文化削弱了修复意愿，另一些人则指出漏洞研究本身不新，LLM 只是将利用门槛降低并普及到低价值目标；还有人强调即使立即修复，部署更新也常超过十分钟，自动更新又带来供应链风险。

**标签**: `#security`, `#AI agents`, `#open source`, `#vulnerability exploitation`, `#OCaml`

---

<a id="item-tech-news-5"></a>
### [美国制裁 Autistici/Inventati 引发基础设施担忧](https://www.inventati.org/) ⭐️ 7.0/10

美国政府将意大利托管服务商 Autistici/Inventati（A/I Collective）及其平台 noblogs.org 列入制裁名单，并冠以“全球恐怖分子”相关定性。这是首次针对托管基础设施提供者采取此类行动，引发对隐私工具、开源项目及独立媒体生存空间的寒蝉效应担忧。A/I Collective 运营着 autistici.org 和 noblogs.org 等服务，目前这些站点部分已不可访问。该事件也促使社区讨论其对 I2P、Monero、Signal 等去中心化隐私项目的潜在影响。

hackernews · exiguus · 8月28日 12:58 · [社区讨论](https://news.ycombinator.com/item?id=49477854)

**「背景」** Autistici/Inventati（A/I Collective）是一个意大利组织，长期运营加密电子邮件、聊天和网站托管服务，并维护博客平台 Noblogs，常被视为隐私与开源社区的基础设施提供者。2026 年 8 月，美国国务院与财政部将其列为“特别指定全球恐怖分子”，称其“为暴力反法西斯组织及极左激进分子构建和运营数字基础设施”。这一认定意味着该托管服务被美国官方定性为恐怖主义关联实体，引发对基础设施提供商和隐私项目受制裁的担忧。

**「影响」** 美国财政部外国资产控制办公室于 8 月 26 日依据反恐权力将意大利数字服务提供商 Autistici/Inventati 列为特别指定全球恐怖分子，冻结其相关财产，并使其合作银行、主机托管商和基础设施提供商面临制裁风险，从而威胁到 Noblogs 平台及该组织提供的加密电子邮件、聊天、视频会议等隐私服务的持续运营，也可能波及更广泛的独立通信项目。

**「社区讨论」** 评论普遍认为这一制裁开创了将基础设施提供者视为“恐怖分子”的危险先例，可能波及 I2P、Monero、Veilid、Tox、Signal 等项目。也有用户质疑制裁依据，指出目前难以找到该组织直接支持 PKK 的证据，并提到 noblogs.org 与 autistici.org 已部分不可用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.state.gov/releases/office-of-the-spokesperson/2026/08/designation-of-autistici-inventati-as-a-specially-designated-global-terrorist/">Designation of Autistici/Inventati as a Specially Designated ...</a></li>
<li><a href="https://home.treasury.gov/news/press-releases/sb0616/">Treasury Takes Action Against Violent Far-Left Terrorist ...</a></li>
<li><a href="https://techandbusiness.org/newswire/IfCKeYYCbu4DC4Tb4R0aWk">US sanctions Italian digital-services provider Autistici ...</a></li>
<li><a href="https://www.state.gov/releases/office-of-the-spokesperson/2026/08/designation-of-autistici-inventati-as-a-specially-designated-global-terrorist/">Designation of Autistici/Inventati as a Specially Designated ...</a></li>
<li><a href="https://news.lavx.hu/article/u-s-sanctions-put-autistici-inventati-s-resilient-network-under-pressure">U.S. sanctions put Autistici/Inventati’s resilient network ...</a></li>

</ul>
</details>

**标签**: `#sanctions`, `#internet infrastructure`, `#privacy`, `#hosting`, `#open source`

---

<a id="item-tech-news-6"></a>
### [开发者在 RP2350 上实现微型潜流 Transformer 人脸图像生成](https://www.reddit.com/r/MachineLearning/comments/1w10tax/i_implemented_a_very_tiny_image_generation_model/) ⭐️ 7.0/10

一位开发者（/u/cpldcpu）在 RP2350 微控制器上实现了一个极小的潜流 Transformer（latent flow transformer）图像生成模型。该模型参数量为 240 万到 400 万，经 int8 量化后，可在芯片上完全运行，最长约 20 秒生成一张 128×128 的人脸图像，结果可通过显示器或 USB 输出。实现采用 12 层 AdaLN-Zero 条件化，并支持 CFG（Classifier-Free Guidance），显著提升图像质量。推理引擎通过 DMA 从闪存流式加载权重，利用 ReLU²激活带来的稀疏性跳过部分计算。作者称经过大量消融实验，惊讶于在如此少参数下能达到的效果。

reddit · r/MachineLearning · /u/cpldcpu · 8月28日 19:48

**「背景」** RP2350 是树莓派公司于 2024 年 8 月发布的第二款微控制器，采用双 Arm Cortex-M33 内核，主频 150 MHz，常见于售价约 5 美元的 Raspberry Pi Pico 2 开发板。潜在流变换器（Latent Flow Transformer）是一种将多个离散 Transformer 层压缩为单个连续输运算子、并通过流匹配训练的神经架构，可大幅缩小生成模型规模。该演示正是利用这类轻量架构，在资源极有限的微控制器上实现图像生成。

**「影响」** 对嵌入式 ML 和边缘推理开发者而言，这展示了在低功耗低成本微控制器上运行生成式视觉 Transformer 的可行性，尽管约 20 秒延迟和 128×128 分辨率使其更偏技术验证而非实用产品。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/RP2350">RP2350 - Wikipedia</a></li>
<li><a href="https://arxiv.org/abs/2505.14513">[2505.14513] Latent Flow Transformer - arXiv.org Latent Flow Transformer - arXiv.org Latent Flow Transformers (LFT) - emergentmind.com Latent Flow Transformer (LFT) - emergentmind.com GitHub - itz-sayak/Latent-Flow-Transformer Paper page - Latent Flow Transformer - Hugging Face Latent Flow Transformer - catalyzex.com</a></li>

</ul>
</details>

**标签**: `#embedded-ml`, `#microcontrollers`, `#transformers`, `#image-generation`, `#edge-inference`

---

<a id="item-tech-news-7"></a>
### [腾讯混元发布 Hy4 preview](https://mp.weixin.qq.com/s/ymr3X878B8oa2XP15CH8TQ) ⭐️ 7.0/10

2026 年 8 月 28 日，腾讯发布迄今最强的开源模型 Hy4 preview，总参数量 770B、活跃参数 49B，上下文窗口达 1M token，主攻长周期软件工程、文档办公与科学研究。该模型已上线腾讯云、GitHub、HuggingFace、ModelScope、AtomGit、OpenRouter 等渠道。在盲评 203 个工程任务中，Hy4 preview 以 2.99 分略胜 GLM 5.3（2.92 分）和 Kimi K3（2.94 分）。API 定价为每 1M tokens 输入 0.834 美元、输出 2.501 美元。

telegram · zaihuapd · 8月28日 06:11

**「背景」** 腾讯混元此次发布的 Hy4 preview 是一款采用混合专家（MoE）架构的开源大语言模型，总参数量达 770B，但每次推理仅激活 49B 参数，以降低计算成本。其上下文窗口为 1M token，能够处理超长文本，主要面向长周期软件工程、文档办公与科学研究等生产力场景。此类开源旗舰模型的发布延续了国内大模型厂商开放权重、多平台分发的趋势。

**「影响」** 对需要长上下文和工程文档处理能力的开发者和研究者而言，Hy4 preview 提供了开源可用的新选择，其盲测分数虽小幅领先竞品，但综合平台覆盖和 API 定价已形成实际可用的替代方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.aibase.com/news/30694">Tencent Hunyuan launches open - source flagship model Hy 4 preview ...</a></li>

</ul>
</details>

**标签**: `#tencent`, `#hunyuan`, `#large language model`, `#open-source`, `#AI`

---

<a id="item-tech-news-8"></a>
### [美国 FTC 调查 YouTube 封号政策，或面临诉讼](https://www.bloomberg.com/news/articles/2026-08-27/us-ftc-probing-youtube-over-social-media-policies) ⭐️ 7.0/10

美国联邦贸易委员会（FTC）正在调查 Alphabet 旗下 YouTube 的封号与内容降权行为是否违反消费者保护法。知情人士称，调查自去年启动，目前已进入准备潜在诉讼的最后阶段，但公司尚未被指控不当行为。调查重点包括 YouTube 封禁或降权内容时是否违反自身用户政策，以及用户是否被政策误导、以为可发布某些内容却遭下架或封号。YouTube 与 FTC 均拒绝评论。

telegram · zaihuapd · 8月28日 07:48

**「背景」** FTC 是美国负责消费者保护的联邦机构，可就企业的不公平或欺骗性行为发起调查和诉讼。此次调查聚焦 YouTube 内容审核规则：平台承诺的用户政策与实际封号、降权操作之间是否存在落差，以及这种落差是否构成对用户的误导。

**「影响」** 若 FTC 提起诉讼，可能迫使 YouTube 调整账号封禁和内容政策，并增加 Alphabet 的合规成本与平台治理压力。由于调查仍处准备阶段，最终结果尚不确定。

**标签**: `#YouTube`, `#FTC`, `#content moderation`, `#regulation`, `#Alphabet`

---

<a id="item-tech-news-9"></a>
### [OpenAI 因 SpaceX 收购终止与 Cursor 合作](https://openai.com/index/our-decision-on-cursor-following-its-acquisition-by-spacex/) ⭐️ 7.0/10

OpenAI 宣布，因 SpaceX 收购 Cursor，将终止通过 Cursor 提供 OpenAI 模型的合同，建议停服日期为 2026 年 11 月 12 日，并给出了合同允许的最大通知期。OpenAI 表示无法确信 SpaceX 会遵守服务条款，理由是马斯克旗下公司有违约记录：收购 Twitter（现并入 SpaceX）后曾违反合同，xAI 今年早些时候在宣誓下承认违反 OpenAI 服务条款。OpenAI 与 Cursor 的定制协议允许其在控制权变更后限时取消合作，双方已合作近四年。这一决定将影响依赖 Cursor 内置 OpenAI 模型的用户和 AI 编程工具生态。

telegram · zaihuapd · 8月29日 02:24

**「背景」** Cursor 是一款 AI 驱动的代码编辑器，长期通过与 OpenAI 的定制合作调用 OpenAI 模型。该协议包含控制权变更条款，允许 OpenAI 在 Cursor 被收购等情况下限时终止合作，因此 SpaceX 收购 Cursor 触发了这一终止程序。

**「影响」** 对当前使用 Cursor 并依赖其内置 OpenAI 模型的用户而言，最直接的影响是需要在 2026 年 11 月 12 日停服前规划替代模型或迁移方案。

**标签**: `#OpenAI`, `#Cursor`, `#SpaceX`, `#AI tools`, `#industry`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [玉米和小麦期货创逾三年新高](https://www.cnbc.com/2026/08/28/corn-and-wheat-prices-jump-to-highest-prices-in-more-than-three-years.html) ⭐️ 8.0/10

受美国供应预期收紧和黑海出口中断影响，玉米和小麦期货升至三年多来最高水平。小麦期货周五收于每蒲式耳 784 美分，本周上涨 12.1%，创 2023 年 2 月以来新高；玉米期货收于每蒲式耳 536.5 美分，本周上涨 5.5%，创 2023 年 7 月以来新高。

rss · CNBC Finance · 8月28日 20:00

**「背景」** 小麦涨势主要源于俄罗斯与乌克兰在黑海地区的紧张局势扰乱全球供应，两国合计占全球小麦出口逾四分之一；玉米则因美国农业部下调单产预估、田间调查显示极端高温影响作物以及欧洲干旱而受到支撑。

**「影响」** 全球谷物供应收紧可能推高食品和饲料成本，影响依赖进口的国家以及养殖和食品加工业。

**标签**: `#corn`, `#wheat`, `#commodity prices`, `#supply disruptions`, `#agriculture`

---

<a id="item-finance-news-2"></a>
### [美上诉法院：体育赛事事件合约不属于联邦监管互换，可能上诉至最高法院](https://www.cnbc.com/2026/08/28/appeals-court-rules-against-prediction-markets-tees-up-scotus-fight.html) ⭐️ 8.0/10

美国第九巡回上诉法院裁定，体育赛事相关的“事件合约”不属于联邦监管的互换合约，并驳回了 Kalshi、Crypto.com 和 Robinhood 要求阻止内华达州执法的禁令请求。这一裁决与第三巡回法院先前的结论相矛盾，可能使案件进入最高法院。

rss · CNBC Finance · 8月29日 02:23

**「背景」** 此前，美国商品期货交易委员会（CFTC）认为所有事件合约都属于“互换”，应由其独占监管，并已起诉九个州；而 44 个州认为这些体育赛事合约只是体育博彩。

**标签**: `#prediction markets`, `#CFTC`, `#sports betting`, `#regulation`, `#Supreme Court`

---

<a id="item-finance-news-3"></a>
### [两部门将个人住房贷款期限上限延长至 40 年](https://news.ifeng.com/c/8vxm6huJOMR) ⭐️ 8.0/10

中国人民银行与国家金融监督管理总局 28 日联合发布文件，将个人住房贷款期限由最长 30 年延长至最长 40 年，具体期限由购房人与商业银行协商确定。

telegram · zaihuapd · 8月28日 12:16

**「背景」** 此前个人住房贷款期限上限为 30 年；新政策旨在适应经济社会发展需要，给予借贷双方更大灵活度。

**「影响」** 购房人可选择更长还款期限，从而降低每月还款额，但贷款期限越长，累计支付利息通常也越多。

**标签**: `#中国房地产`, `#住房贷款`, `#信贷政策`, `#央行`, `#金融监管`

---

<a id="item-finance-news-4"></a>
### [美联储 9 月加息概率因沃什讲话上升，市场预期接近对半](https://www.cnbc.com/2026/08/28/-september-fed-decision-now-a-coin-flip-as-rate-hike-odds-increase.html) ⭐️ 7.0/10

美联储主席沃什在杰克逊霍尔讲话后，市场对 9 月加息预期上升：Kalshi 显示加息概率约 48%，CME FedWatch 显示约 56%，Polymarket 显示约 49%；此前市场预计 9 月按兵不动的概率接近 70%。

rss · CNBC Finance · 8月28日 15:22

**「背景」** 7 月美联储维持利率不变，但有三名 FOMC 成员反对并主张加息；随后公布的 7 月就业报告弱于预期且通胀有所降温，导致 9 月加息预期回落。沃什在讲话中承认近期通胀数据好于预期，但认为仍需看到更明确的证据。

**标签**: `#Federal Reserve`, `#monetary policy`, `#interest rates`, `#inflation`, `#market expectations`

---

<a id="item-finance-news-5"></a>
### [美股盘前异动：PayPal 大跌，Affirm 与 Gap 上涨，多家科技股因财报波动](https://www.cnbc.com/2026/08/28/stocks-making-the-biggest-moves-premarket-pypl-afrm-gap-mrvl.html) ⭐️ 7.0/10

8 月 28 日美股盘前，多只个股因并购和财报消息较前收盘价大幅波动：PayPal 跌近 16%，因有报道称收购方放弃潜在交易；Affirm 涨 13%，因第四财季营收 11.7 亿美元高于预期的 11.1 亿美元；Gap 涨近 15%，因更换 Old Navy 负责人且二季度调整后每股盈利 0.52 美元高于预期的 0.48 美元；Elastic 涨逾 17%，因全年指引高于预期；Marvell、Rubrik 和 Autodesk 则分别下跌近 8%、逾 5%和近 4%。

rss · CNBC Finance · 8月28日 11:43

**「背景」** 盘前交易指美股常规交易时段开始前的交易，价格会先反映隔夜或盘前发布的消息；杠杆收购指买家主要通过借款收购公司。PayPal 潜在交易如果成行，原本可能成为规模最大的杠杆收购之一。

**标签**: `#earnings`, `#mergers and acquisitions`, `#premarket movers`, `#technology stocks`, `#retail`

---