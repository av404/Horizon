---
layout: default
title: "Horizon Summary: 2026-09-11 (ZH)"
date: 2026-09-11
lang: zh
---

> 从 41 条内容中筛选出 10 条重要资讯。

---

**科技新闻**
1. [Shopify 从 React Native 迁回原生 Swift 与 Kotlin](#item-tech-news-1) ⭐️ 8.0/10
2. [微软将 Rust 列为一级语言](#item-tech-news-2) ⭐️ 8.0/10
3. [trynix.dev：在浏览器里启动任意 Nix 包](#item-tech-news-3) ⭐️ 8.0/10
4. [能否信任 OpenAI 处理未发表数学](#item-tech-news-4) ⭐️ 7.0/10
5. [果蝇连接组打乒乓失败：突触审计比成功更有价值](#item-tech-news-5) ⭐️ 7.0/10
6. [蚂蚁国际携手 Visa 与 Mastercard 制定 AI 代理支付标准](#item-tech-news-6) ⭐️ 7.0/10
7. [DeepSeek V4.1 Flash：552B 多模态模型上线 API](#item-tech-news-7) ⭐️ 7.0/10
8. [腾讯混元发布开源音频模型 AuK 与 AuK-Flash](#item-tech-news-8) ⭐️ 7.0/10

**财经新闻**
1. [卡尔希获 CFTC 批准推出黄金和白银永续期货](#item-finance-news-1) ⭐️ 7.0/10
2. [HBM 短缺推高中国 AI 芯片价格，华为、寒武纪上调报价](#item-finance-news-2) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Shopify 从 React Native 迁回原生 Swift 与 Kotlin](https://shopify.engineering/back-to-native) ⭐️ 8.0/10

Shopify Engineering 正在把其移动应用从 React Native 迁回原生 Swift 和 Kotlin，这一决定以公司工程博客文章的形式公开。Shopify 工程师在 Hacker News 讨论中表示，LLM 改变了 2020 年技术选型背后的一个核心假设，因此团队重新评估了当年选择 React Native 的决定。对于一家大型电商平台而言，此举意味着其移动端未来将更多依赖平台原生技术栈和专门的 iOS/Android 工程能力，而非以共享代码库为中心。相关讨论还显示，这次迁移是否主要依赖 AI 辅助仍存在不同经验，但“共享代码库收益是否已被高估”是争论的核心。

hackernews · fnthawar2 · 9月10日 14:09 · [社区讨论](https://news.ycombinator.com/item?id=49643982)

**「背景」** React Native 是 Meta 推出的跨平台移动开发框架，允许开发者用 JavaScript 和 React 编写一次代码，同时运行在 iOS 和 Android 上。Swift 是 Apple 主推的 iOS 原生开发语言，Kotlin 是 Android 平台广泛采用的原生语言，两者各自针对平台特性进行优化。Shopify 工程博客宣布，公司将把移动应用从 React Native 迁移回 Swift 和 Kotlin 原生开发。

**「影响」** 对 Shopify 的移动开发者来说，这意味着日常开发将从 React Native 的单一共享代码库转为分别用 Swift 与 Kotlin 维护 iOS 和 Android 原生代码，跨平台复用带来的成本收益需要重新评估。作为一个高知名度的迁移案例（工程博客于 2026 年 9 月 10 日发布，并将编码智能体改变移动开发成本列为动因），这一决定也为其他团队在 React Native 与原生方案之间做取舍时提供了可参照的先例。

**「社区讨论」** 评论者大多支持迁回原生并质疑共享代码库的长期价值，但关于 LLM 是否让迁移变得可行存在明显分歧：有开发者称借助 Codex 等工具在一夜之间完成大部分迁移，另有人以自身在 2026 年 1 月前、基本无 LLM 辅助完成中型 React Native 到 Swift/Kotlin 重写为例反驳。实践层面的共识是原生平台通常需要专门工程师做深度优化，而 React Native 借助 Web 开发者做移动端的传统优势正在减弱。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://shopify.engineering/back-to-native">Native is now the future of mobile at Shopify (2026) - Shopify</a></li>
<li><a href="https://news.ycombinator.com/item?id=49643982">Shopify moves back to Native from React Native | Hacker News</a></li>
<li><a href="https://shopify.engineering/back-to-native">Native is now the future of mobile at Shopify (2026) - Shopify</a></li>

</ul>
</details>

**标签**: `#React Native`, `#Mobile Engineering`, `#Swift`, `#Kotlin`, `#AI-assisted Migration`

---

<a id="item-tech-news-2"></a>
### [微软将 Rust 列为一级语言](https://rustfoundation.org/media/guest-post-rust-is-tier-1-language-at-microsoft/) ⭐️ 8.0/10

Rust 基金会发布客座文章称，微软已将 Rust 列为一级（tier-1）语言。这一认定被视为 Rust 成熟度、产业采用度以及在系统编程领域地位提升的重要行业信号。由于提供的来源没有正文内容，文章未披露具体的支持范围、版本、时间表或兼容性约束。

hackernews · mmastrac · 9月10日 13:39 · [社区讨论](https://news.ycombinator.com/item?id=49643546)

**「背景」** 微软所称的 tier-1 语言工程状态，指内部团队获得从本地开发到生产的“铺好路”支持，包括安全工具链构建、开发者工具、质量工作流、平台深度集成与合规支持。微软正式将 Rust 归类为 tier-1 编程语言，这被视为其语言策略的一次重要转变，不过相关官方细节仍然有限。Rust 属于系统编程语言，该分类意味着它在该公司软件开发生态中具有关键作用。

**「影响」** 对在 Windows 上使用 Rust 的开发者来说，这一地位的直接影响体现在工具链已与微软自有生态绑定：微软官方文档要求 Windows 上的 Rust 开发以 Microsoft C++ 生成工具作为前置依赖，并通过 VS Code 的 rust-analyzer 扩展提供代码补全、内联报错、跳转定义与调试支持。不过，由于目前缺少公告本身的细节，这一“一级语言”定位在多大程度上会改变现有工具链、支持承诺或迁移时间表，尚不明确。

**「社区讨论」** 评论普遍欢迎该认定，认为 Rust 已足够成熟，可与 C++、C\# 等竞争，并让主要操作系统厂商在系统编程语言上更加多元化；有评论者提到微软的内存安全需求和减少 CVE 的动机，以及 MSVC 集成传闻。实际经验方面，有人称已专业使用 Rust 五年并看好其在应用开发中的适用性，但也指出 wasm 和 macOS/Windows/Android/iOS 原生 UI 支持不足；另有评论提及到 2030 年将 10 亿行代码转换为 Rust 的目标和 DARPA 的自动化 C 到 Rust 转换工作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://rustfoundation.org/media/guest-post-rust-is-tier-1-language-at-microsoft/">Guest Post: Rust Is Tier-1 Language at Microsoft</a></li>
<li><a href="https://qatrial.com/developer-open-source/rust-is-tier-1-language-at-microsoft/">Rust Is Tier-1 Language At Microsoft - QAtrial</a></li>
<li><a href="https://bestcadpapers.com/art-and-society/rust-is-tier-1-language-at-microsoft/">Rust Is Tier-1 Language At Microsoft - Best CAD papers</a></li>
<li><a href="https://learn.microsoft.com/ru-ru/windows/dev-environment/rust/setup">Настройка среды разработки в Windows для Rust | Microsoft Learn</a></li>

</ul>
</details>

**标签**: `#Rust`, `#Microsoft`, `#programming languages`, `#systems programming`, `#open source`

---

<a id="item-tech-news-3"></a>
### [trynix.dev：在浏览器里启动任意 Nix 包](https://simonwillison.net/2026/Sep/10/trynix/) ⭐️ 8.0/10

Farid Zakaria 发布了 trynix.dev，他称之为自己 Nix 工作的“magnum opus”。该站点通过 qemu-wasm 在浏览器中以 WebAssembly 运行一台 x86\_64 Linux 虚拟机，可以启动过去 13 年间的任意 Nix 包，并且这些包是 URL 可寻址的：访问 https://trynix.dev/?pkg=python3%403.6.2 并点击“Load”，就能得到一个运行 2017 年发布的 Python 3.6.2 的交互式 shell。在此基础上，Zakaria 还推出了 trynix-preview——一个 GitHub Action，会在 pull request 下评论一个链接，让审阅者用 trynix.dev 在浏览器中启动该 PR 的构建，无需任何服务器，只用浏览器。

rss · Simon Willison · 9月10日 23:44

**「背景」** Nix 是一套函数式包管理器，其软件包集合 nixpkgs 强调可复现构建，因此历史上发布过的每个包版本都被完整保留下来。trynix 借助 qemu-wasm（用 Emscripten 把 QEMU 编译为 WebAssembly）在浏览器标签页内运行 x86\_64 Linux 虚拟机，并通过 virtio-9p 将 Nix store 挂载进 guest，使启动过程无需任何服务器。它索引了 13 年 nixpkgs 历史中超过 310,083 个包版本，但只提供串行控制台，没有图形界面。

**「影响」** 对 Nix 用户与代码审阅者来说，这意味着无需本地安装、也无需服务器，就能在浏览器中直接启动某个历史版本的包或某个 PR 的构建结果进行验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/fzakaria/trynix">fzakaria/ trynix : Boot anything nixpkgs ever shipped, in your browser .</a></li>
<li><a href="https://fzakaria.com/2026/09/04/any-nix-package-live-in-your-browser">Any Nix package, live in your browser | Farid Zakaria ’s Blog</a></li>
<li><a href="https://trynix.dev/">trynix</a></li>

</ul>
</details>

**标签**: `#Nix`, `#WebAssembly`, `#qemu-wasm`, `#browser-based virtualization`, `#reproducible builds`

---

<a id="item-tech-news-4"></a>
### [能否信任 OpenAI 处理未发表数学](https://mathstodon.xyz/@andreasthom/117240535270608201) ⭐️ 7.0/10

Hacker News 上一则链接讨论帖引发对研究人员能否信任 OpenAI 处理未发表数学的关注，该讨论获得 631 分和 613 条评论。帖子本身仅由链接组成，核心指控尚未得到证实，但评论者围绕 OpenAI 是否在未署名的情况下使用研究者的未发表数学与聊天内容展开辩论。争论焦点包括训练数据来源、对可验证数学进行强化学习，以及模型在开放问题上的进展是否真实。多位评论者以人类合作者作为类比，认为若 OpenAI 是人类研究者，未署名发布沿合作方向的工作会被视为不道德；也有人认为模型预训练中吸收聊天直觉与通过大规模强化学习独立发现数学技巧可以同时成立。

hackernews · pred\_ · 9月10日 06:49 · [社区讨论](https://news.ycombinator.com/item?id=49639408)

**「背景」** 这一争议发生在一系列围绕 OpenAI 数学成果与训练数据来源的质疑之中：此前 Levent Alpöge、Tristan Buckmaster 等数学家已提出类似指控，若这些指控均被证实，就不再是孤立事件。据支持性报道，数学家 Andreas Thom 曾在数月间与 ChatGPT 讨论 expander matching 问题，随后 OpenAI 宣布其模型构造出首个非 sofic 群（non-sofic group）的成果，Thom 就此致信 OpenAI 数学方向负责人 Sébastien Bubeck 与 Mark Sellke 提出疑问。上述指控目前尚待证实，核心争议在于 OpenAI 的模型是否使用了研究者未发表的对话内容。

**「对研究者协作意愿的影响」** 对使用 OpenAI 模型处理未发表数学工作的研究者而言，这类争议直接触及协作意愿：有报道指出，OpenAI 一方面向至少 10 万名研究者提供免费访问，另一方面被指在未署名的情况下发布与研究者对话相关的成果，并卷入关于署名、伦理与隐私的争执。由于核心指控尚未得到证实，当前更接近信任与训练数据来源层面的风险预警，而非已确认的违规结论。

**「社区讨论」** 评论者意见分歧：一方以人类合作者类比，认为 OpenAI 使用研究者聊天并沿合作方向发表而不署名是不道德的；另一方主张模型预训练吸收聊天直觉与大规模可验证数学强化学习独立发现技巧可以同时为真。还有评论者怀疑 OpenAI 内部模型解决开放问题的速度，并指出研究者使用 Codex 等工具时会把未发表问题的新鲜信息反馈给公司，而企业保护用户数据的承诺往往不可信。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://lemmy.world/post/51743560">OpenAI might have stolen another major math proof - Lemmy.World</a></li>
<li><a href="https://officechai.com/ai/mathematician-andreas-thom-questions-if-openai-used-his-chatgpt-chat-data-for-its-non-sofic-groups-proof/">Mathematician Andreas Thom Questions If OpenAI Used His...</a></li>
<li><a href="https://ai-tldr.dev/releases/andreas-thom-openai-math-data/">Andreas Thom — a second mathematician questions OpenAI on his...</a></li>
<li><a href="https://theconversation.com/openai-claims-another-huge-mathematical-result-amid-fights-over-credit-ethics-and-privacy-291575">OpenAI claims another huge mathematical result amid fights over...</a></li>
<li><a href="https://news.ycombinator.com/item?id=49639408">More questions about whether researchers can trust OpenAI with...</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#AI research ethics`, `#training data provenance`, `#mathematics`, `#LLM attribution`

---

<a id="item-tech-news-5"></a>
### [果蝇连接组打乒乓失败：突触审计比成功更有价值](https://www.reddit.com/r/MachineLearning/comments/1wc67ci/i_tried_to_make_a_real_fly_connectome_learn_to/) ⭐️ 7.0/10

Reddit 用户 /u/oPeraza2007 尝试让真实果蝇连接组的一小块子图通过多巴胺式可塑性学会玩 Pong，但没有成功；作者认为，弄清失败原因所做的突触级审计比一个成功演示更有信息量。实验基于新发布的 MaleCNS v1.0 连接组（16.6 万个神经元、真实 EM 重建），过程中修复了 neuPrint 正则 bug——该 bug 因全匹配与子串语义差异静默清零两个神经元群体，并发现原始神经元选择中光感受器到其他节点毫无路径，因为真实光感受器并不直接突触到运动检测器，中间缺少一整层。修好流水线后，开启与关闭学习在多个随机种子下得到逐位相同的结果，尽管权重确实在变化；追踪发现 4 个可用运动神经元中有 2 个从任何感觉通路都没有突触输入，它们仅因数组索引被划入“球拍向下”组，无论学习规则如何都不可能发放。作者随后围绕更好的生物学假设重建电路，将威胁检测通路换成与求偶追逐中视觉目标追踪相关的通路，但该假设被数据否定，最终找到另一个真正端到端连接的下降神经元，才首次让学习开/关出现差异；不过效果更像是学习规则让整个系统安静下来，而非技能提升，因为未命中多于命中时惩罚占主导并缩小运动响应。作者还检查了更热门的病毒式项目：Doom 项目自己的仓库称经六次迭代未通过自身验证门槛，Minecraft mod 的限制部分承认真实运动检测通路保持沉默、逃跑和觅食行为是手工注入或反射层回退，Beat Saber 创作者回复承认模型过拟于单首曲目且回放数据混入了输入。

reddit · r/MachineLearning · /u/oPeraza2007 · 9月10日 02:28

**「背景」** 果蝇连接组（connectome）是对黑腹果蝇神经系统中各神经元及其之间化学突触的结构图谱，覆盖脑与腹神经索，且雌雄个体间差异明显。本文所涉的 MaleCNS v1.0 是 Janelia 研究团队发布的雄蝇全中枢神经系统重建成果，包含约 16.6 万个神经元及数百万条连接，并非简化玩具模型。研究者通常借助 neuPrint 及其 Python 接口，按细胞类型、实例名和正则表达式检索神经元与突触数据；正则匹配中整串匹配与子串匹配的语义差异，正是本次排查里导致若干神经元群体被静默过滤的原因之一。

**「影响」** 对尝试用 MaleCNS v1.0 等真实连接组做行为仿真的研究者和开发者而言，这项逐突触审计意味着在采信演示效果前必须先验证光感受器到运动神经元的完整通路，因为作者指出 Doom、Minecraft 与 Beat Saber 等项目自身也承认未过验证门槛、关键运动检测通路静默或依赖手工注入行为，而同期报道仍把这些演示解读为验证了果蝇脑图的实用价值。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Drosophila_connectome">Drosophila connectome - Wikipedia</a></li>
<li><a href="https://male-cns.janelia.org/">Male CNS Connectome - MaleCNS connectome</a></li>
<li><a href="https://www.janelia.org/project-team/flyem/male-cns-connectome">Male CNS Connectome | Janelia Research Campus</a></li>
<li><a href="https://connectome-neuprint.github.io/neuprint-python/docs/neuroncriteria.html">NeuronCriteria — neuprint-python 0.6.2 documentation</a></li>
<li><a href="http://natverse.org/neuprintr/reference/neuprint_search.html">Search for body IDs based on a given name — neuprint_search • neuprintr</a></li>
<li><a href="https://hothardware.com/news/google-mapped-a-fruit-fly-brain-so-engineers-taught-it-to-play-doom">Google Mapped A Fruit Fly Brain, So Engineers Taught It To Play Doom</a></li>
<li><a href="https://www.dexerto.com/gaming/googles-digital-fly-brain-gets-its-own-heaven-after-going-through-beat-saber-hell-3407304/">Google’s digital fly brain gets its own heaven after going through Beat Saber hell - Dexerto</a></li>

</ul>
</details>

**标签**: `#connectome`, `#computational neuroscience`, `#plasticity`, `#machine learning`, `#negative results`

---

<a id="item-tech-news-6"></a>
### [蚂蚁国际携手 Visa 与 Mastercard 制定 AI 代理支付标准](https://www.cnbc.com/2026/09/10/ant-international-visa-mastercard-ai-agent-payment-standard.html) ⭐️ 7.0/10

蚂蚁国际宣布与 Visa、Mastercard 合作，为 AI 代理支付制定通用标准。三方将建立“了解你的代理”（Know Your Agent）机制，将代理与有效实体关联、评估其行为并监测风险，以提升不同支付系统之间的互操作性与安全性。三方援引麦肯锡的预测称，到 2030 年 AI 代理可能处理全球消费者商业交易中的 3 万亿至 5 万亿美元。该消息由 CNBC 报道，经 Telegram 频道“在花频道”转述，目前仍属早期合作公告，未披露技术规范或具体实施细节，因此独立验证受限。

telegram · zaihuapd · 9月10日 03:00

**「背景」** AI 代理支付指的是由自主 AI 代理代表用户完成比价、下单与付款的商务场景，其难点在于支付网络无法像核验真人持卡人那样确认代理的身份、授权范围和行为是否可信。蚂蚁国际、Visa 与 Mastercard 提出的“了解你的代理”（Know Your Agent，KYA）框架，旨在把代理与一个有效实体关联起来，并对其行为进行评估和风险监测，从而在不同支付系统之间建立互操作性与安全性。此前三方各自推进的代理支付协议彼此竞争，此次合作是对这些分散路线的一次对齐，但据外部报道，该框架目前仍属高层意向，尚无技术规范、治理安排或时间表。

**「影响」** 对支付机构、商户和 AI 代理开发者而言，若该“了解你的代理”框架落地，代理的身份核验与授权方式将由 Visa、Mastercard 和蚂蚁国际的网络共同界定，跨支付系统的代理交易有望获得统一的识别与风控口径；但目前三方仅宣布合作意向，尚无公开技术规范、时间表或适用范围，短期内不会改变现有接入要求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.unite.ai/ant-international-visa-mastercard-align-on-ai-agent-verification-rules/">Ant International, Visa, Mastercard Align on AI Agent ...</a></li>
<li><a href="https://forkast.news/ant-international-visa-and-mastercard-agree-on-agent-identity-standard-now-comes-the-hard-part/">Ant International, Visa, and Mastercard Agree on Agent ...</a></li>
<li><a href="https://mitsloanindia.com/article/visa-mastercard-ant-push-common-standards-for-ai-agents-making-payments/">Visa , Mastercard , Ant Push Common Standards for AI Agents ...</a></li>
<li><a href="https://political.org/2026/09/09/visa-mastercard-and-ant-international-develop-standards-for-ai-agent-payments/">Visa , Mastercard and Ant International Launch ‘Know Your Agent ...</a></li>
<li><a href="https://www.hokanews.com/2026/09/visa-and-mastercard-back-ant.html">Visa and Mastercard Back Ant International’s ‘Know Your Agent ...</a></li>

</ul>
</details>

**标签**: `#AI agents`, `#payments`, `#standards`, `#fintech`, `#interoperability`

---

<a id="item-tech-news-7"></a>
### [DeepSeek V4.1 Flash：552B 多模态模型上线 API](https://mp.weixin.qq.com/s/qg0NU3NNUbp1co2PdkAPAg) ⭐️ 7.0/10

据发布信息，DeepSeek 推出 V4.1 Flash，称其为全新模型结构系列中最小尺寸的模型，采用 552B 参数的 Causal-Encoder-Decoder 结构，输入激活为 8B、输出激活为 16B，并原生支持多模态视觉理解。该模型已在 DeepSeek API 上线，模型名为 deepseek-flash。新价格将于 2026 年 9 月 10 日 12:00 生效；自 9 月 14 日 12:00 后，deepseek-v4-pro 请求将被路由至 V4.1 Flash，并按 V4.1 Flash 的价格计费。上述内容来自聚合消息，未附基准测试、技术评估或官方额外确认，实际能力与定价影响仍需以 DeepSeek 官方信息为准。

telegram · zaihuapd · 9月10日 05:54

**「背景」** DeepSeek V4.1 Flash 是 DeepSeek 新架构系列中尺寸最小的模型，采用非对称的 552B 参数混合专家（MoE）设计，输入与输出分别仅激活 8B 和 16B 参数，并原生支持视觉理解；官方称其目标是在提升能力与推理速度的同时扩大吞吐，并能向上扩展至更大模型。其 Causal Encoder-Decoder 结构把 40 层 Transformer 拆分为各 20 层的因果编码器与解码器两段，主要面向需要处理大型文档、代码库或长对话历史等输入密集型智能体任务，以压低这类负载的算力成本；相关模型卡显示其为多模态 MoE 发布，采用 MIT 许可并支持 1M 上下文。在 API 侧，新价格与把 deepseek-v4-pro 请求路由至 V4.1 Flash 的安排，属于厂商在推理成本、吞吐与能力之间重新权衡的常见做法。

**「影响」** 对生产环境调用 DeepSeek API 的开发者而言，最直接的后果是：2026 年 9 月 14 日 12:00 之后，发往 deepseek-v4-pro 的请求将被自动路由至 V4.1 Flash 并按新价格计费，相当于在未改动代码的情况下发生模型替换，因此需要固定模型 ID，并在切换生产流量前用自身验收测试重新验证效果。不过相关说法目前来自聚合渠道和第三方页面，缺少官方确认与基准数据，实际路由行为与性能表现仍待核实。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.deepseek.com/en/news/deepseek-v4-1-flash/">DeepSeek | Introducing DeepSeek-V4.1-Flash: smarter, faster ...</a></li>
<li><a href="https://www.gate.com/news/detail/deepseek-releases-v41-flash-ai-model-with-552b-parameters-24165404">DeepSeek Releases V4.1-Flash AI Model With 552B Parameters</a></li>
<li><a href="https://aiweekly.co/alerts/deepseek-posts-v41-flash-552b-moe-8b-active-1m-context">DeepSeek posts V4.1-Flash: 552B MoE, 8B active, 1M context</a></li>
<li><a href="https://benchlm.ai/deepseek/api-pricing">DeepSeek API Pricing (September 2026): $0.30–$1.20 per 1M ...</a></li>

</ul>
</details>

**标签**: `#DeepSeek`, `#LLM release`, `#multimodal AI`, `#API pricing`, `#AI news`

---

<a id="item-tech-news-8"></a>
### [腾讯混元发布开源音频模型 AuK 与 AuK-Flash](https://x.com/TencentHunyuan/status/2097996926876795197) ⭐️ 7.0/10

腾讯混元正式发布开源音频编辑模型 AuK，可通过自然语言指令和参考音频统一完成语音生成与编辑，支持零样本文本转语音、音色/风格/情绪编辑、去口音及多人语音分离等功能。同步推出的 AuK-Flash 采用 4 步推理，在匹配条件下速度约提升 4.5 倍。代码、模型权重和演示已上线，面向语音与音频 AI 开发者开放。此次公告未披露基准测试结果、模型规模与许可细节，AuK-Flash 的约 4.5 倍加速也附带条件且尚待独立验证。

telegram · zaihuapd · 9月10日 11:56

**「背景」** 在 AuK 之前，零样本文本转语音与语音编辑通常由不同模型或专用工具分别承担，降噪、去口音、说话人分离等任务往往各有独立方案。AuK 的定位是把这些能力统一到一个模型和一个自然语言接口中，并同时覆盖语音、通用音频与音乐（tool-1-1、tool-1-3）。据外部报道，该模型规模约 1.5B 参数、以 MIT 许可开源，被描述为用一个开源模型替代约 16 项语音工具（tool-1-3）。

**「影响」** 对语音与音频 AI 开发者而言，AuK 将零样本语音合成与基于参考音频的语音编辑统一到同一套自然语言接口，可省去为生成与编辑分别部署模型的工作；AuK-Flash 以 4 步推理且不使用分类器无关引导，在匹配条件下报告约 4.5 倍墙钟加速。需要注意的是，4.5 倍属于采样层面的对比数字，而非端到端实测结果，实际收益取决于具体部署流程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mmlong818.github.io/ai-pulse/articles/tencent-auk-audio-model.html">Tencent Hunyuan Open - Sources AuK for Speech and Audio Editing ...</a></li>
<li><a href="https://alphasignal.ai/news/tencent-s-auk-replaces-16-speech-tools-with-one-open-source-model">Tencent &#x27;s AuK Replaces 16 Speech Tools With One Open - Source ...</a></li>
<li><a href="https://www.orcarouter.ai/blog/auk-vs-auk-flash">AuK vs AuK - Flash : 4 Sampling Steps vs 32, and Who Wins</a></li>
<li><a href="https://arxiv.org/pdf/2609.08936">AuK Technical Report: An Open-Source Foundational Model for...</a></li>
<li><a href="https://cctest.ai/en/articles/auk-unifies-open-source-speech-generation-and-editing">AuK : An Open-Source Model for Speech Generation and Editing</a></li>

</ul>
</details>

**标签**: `#open-source-models`, `#audio-editing`, `#text-to-speech`, `#generative-ai`, `#Tencent-Hunyuan`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [卡尔希获 CFTC 批准推出黄金和白银永续期货](https://www.cnbc.com/2026/09/10/kalshi-launches-perps-for-gold-and-silver-following-cftc-approval-expanding-futures-offerings.html) ⭐️ 7.0/10

卡尔希（Kalshi）本周获得美国商品期货交易委员会（CFTC）批准，并于周四上线与黄金、白银挂钩的永续期货，这是该公司首款获批的非加密类永续合约；此类合约没有到期日，通过资金费率机制跟踪标的资产价格。该公司称，包括金属和石油在内的大宗商品事件合约在七个月内交易量超过 4 亿美元，达到同一规模所用时间是其加密事件合约的一半。

rss · CNBC Finance · 9月10日 14:00

**「背景」** Kalshi 原本以事件预测类合约（押注事件结果的衍生品）为主业，此前已于 5 月底获 CFTC 批准，首次将加密货币永续期货引入美国境内交易。此次金银合约是该公司首个获批的非加密货币永续期货，也标志其从预测市场和加密资产向传统大宗商品扩张。

**「影响」** 传统期货交易所（如 CME 集团和 CBOE）面临交易被分流至这类无到期日合约的竞争压力，其投资者是直接受影响方：据 CNBC 报道，Kalshi 推出永续合约后 CBOE 和 CME 股价下跌；外部报道显示，此前 Kalshi 加密永续合约获批后，CBOE、CME、ICE 等交易所运营商股价也曾走低，CME 集团更以竞争受损为由起诉 CFTC 试图阻止批准。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://finance.yahoo.com/markets/commodities/articles/kalshi-launches-gold-silver-perpetual-175449558.html?fr=sycsrp_catchall">Kalshi launches gold and silver perpetual futures with CFTC ...</a></li>
<li><a href="https://www.kucoin.com/news/flash/kalshi-launches-gold-and-silver-perpetual-futures-with-cftc-approval">Kalshi Launches Gold and Silver Perpetual Futures with CFTC ...</a></li>
<li><a href="https://finance.yahoo.com/markets/stocks/articles/cboe-cme-ice-ndaq-stocks-183845986.html?fr=sycsrp_catchall">CBOE, CME, ICE, NDAQ Stocks Take A Hit After Kalshi&#x27;s Bitcoin ...</a></li>
<li><a href="https://scanx.trade/stock-market-news/equity-markets/cme-sues-cftc-over-kalshi-perpetual-futures-approval/43780384">CME sues CFTC over Kalshi perpetual futures approval</a></li>
<li><a href="https://fenado.ai/articles/cboe-shares-drop-76-as-cme-group-sues-cftc-over-perpetual-futures-approval">Cboe Shares Drop 7.6% as CME Group Sues CFTC Over Perpetual ...</a></li>

</ul>
</details>

**标签**: `#CFTC`, `#perpetual futures`, `#Kalshi`, `#gold and silver`, `#market structure`

---

<a id="item-finance-news-2"></a>
### [HBM 短缺推高中国 AI 芯片价格，华为、寒武纪上调报价](https://www.reuters.com/world/asia-pacific/chinas-ai-chipmakers-raise-prices-high-bandwidth-memory-shortage-bites-2026-09-10/) ⭐️ 7.0/10

据路透社报道，受全球高带宽存储器（HBM）供应紧张和美国出口限制影响，华为、寒武纪等中国 AI 芯片厂商已上调产品价格。华为升腾 950DT 芯片的报价较两个月前上涨约 20%—50%，部分老款芯片上涨约 30%；寒武纪新一代思元 690 的价格预计上涨约 20%—30%。

telegram · zaihuapd · 9月10日 09:29

**「背景」** HBM 是 AI 芯片配套使用的高速内存，主要由 SK 海力士、三星和美光供应，美国的出口限制使中国市场获取更加困难；与此同时国内 AI 算力需求仍在增长，HBM 短缺正成为国产 AI 芯片扩大供应的瓶颈。

**「影响」** 对采购国产 AI 芯片的云计算和数据中心企业来说，芯片涨价意味着算力建设的采购成本上升。

**标签**: `#HBM shortage`, `#AI chips`, `#China semiconductor industry`, `#price increases`, `#export controls`

---