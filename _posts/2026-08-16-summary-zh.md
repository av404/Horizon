---
layout: default
title: "Horizon Summary: 2026-08-16 (ZH)"
date: 2026-08-16
lang: zh
---

> 从 33 条内容中筛选出 9 条重要资讯。

---

**科技新闻**
1. [Anthropic 公开 Claude 系统提示词，引发开发者深度分析](#item-tech-news-1) ⭐️ 8.0/10
2. [模型被有意变笨：从记忆转向工具推理](#item-tech-news-2) ⭐️ 8.0/10
3. [AI 信用转售经济：Token 经纪人、风险与政策](#item-tech-news-3) ⭐️ 7.0/10
4. [Cloudflare 静默注入分析脚本，用户需手动关闭](#item-tech-news-4) ⭐️ 7.0/10
5. [Qwen 3.8 27B：本地模型很强，但默认过度思考](#item-tech-news-5) ⭐️ 7.0/10
6. [达里奥·阿莫迪谈 AI 信任危机](#item-tech-news-6) ⭐️ 7.0/10
7. [SSOG 注意力：次二次复杂度的高效缩放点积注意力替代方案](#item-tech-news-7) ⭐️ 7.0/10
8. [仅 200 步微调让 Qwen2.5-7B 自称有感知](#item-tech-news-8) ⭐️ 7.0/10

**财经新闻**
1. [Anthropic 第二季初步营收超 115 亿美元，同比增约 14 倍](#item-finance-news-1) ⭐️ 8.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Anthropic 公开 Claude 系统提示词，引发开发者深度分析](https://platform.claude.com/docs/en/release-notes/system-prompts) ⭐️ 8.0/10

Anthropic 在 platform.claude.com 的发布说明中公开了 Claude 系列模型的详细系统提示词，这是主流 AI 模型厂商少有的透明化举措，引发开发者广泛关注。Simon Willison 将这些提示词整理成 git 提交历史，便于追踪版本变化，例如 Opus 4.8 到 Opus 5 的差异中新增了关于“Claude Fable 5 和 Claude Mythos 5 首次发布”的表述。提示词还包含行为塑造规则，例如系统会自行检查图片是否真实存在，并在用户处于危机或痛苦中时优先考虑其福祉而非完成任务。该发布为开发者理解模型行为、调试提示词和评估安全策略提供了直接参考，但并非范式转变。

hackernews · tosh · 8月16日 12:48 · [社区讨论](https://news.ycombinator.com/item?id=49319556)

**「背景」** Anthropic 会在官方文档中公开发布 Claude 面向用户的聊天系统（如 claude.ai 和 iOS/Android 应用）所使用的系统提示词，并承诺随版本更新持续更新；这些提示词位于对话开始处，提供当前日期等最新信息并约束模型行为。早期公开版本涵盖 Claude 3 Haiku、Claude 3 Opus 和 Claude 3.5 Sonnet，Simon Willison 等开发者还会将每次发布整理成 git 提交历史，方便对比不同模型版本之间的提示词差异。此公开行为为开发者观察和理解模型行为指令的演进提供了难得的透明度。

**「影响」** 开发者现在可以基于公开系统提示词追踪 Claude 行为规则的变化，并据此调整自己的提示工程与安全评估；不过提示词只是多层行为塑造系统的一部分，不能单独解读为模型能力的全部。

**「社区讨论」** 社区总体上欢迎这种透明度，Simon Willison 的 git 历史整理让比较版本差异变得容易。也有开发者质疑，把“检查图片是否存在”这类常识写进系统提示词，说明 Anthropic 并未将 Claude 视为真正智能；另有人提醒系统提示词只是多层行为塑造的一部分，并表达了关于 HN 对涉 AI 负面报道审核的担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://platform.claude.com/docs/en/release-notes/system-prompts">System Prompts - Claude Platform Docs - Anthropic</a></li>
<li><a href="https://simonwillison.net/2024/Aug/26/anthropic-system-prompts/">Anthropic Release Notes: System Prompts - Simon Willison</a></li>
<li><a href="https://platform.claude.com/docs/en/release-notes/overview">Claude Platform release notes - Claude Platform Docs - Anthropic</a></li>

</ul>
</details>

**标签**: `#Claude`, `#system prompts`, `#AI transparency`, `#machine learning`, `#Anthropic`

---

<a id="item-tech-news-2"></a>
### [模型被有意变笨：从记忆转向工具推理](https://w4g1.dev/blog/models-are-getting-dumber-on-purpose) ⭐️ 8.0/10

这篇文章分析了一个正在发生的模型设计转向：AI 模型正有意减少对参数内事实记忆的依赖，转而把知识获取与计算交给外部工具、检索和推理过程。作者认为这种“变笨”是刻意取舍，目的是缓解幻觉并绕开知识截止日期带来的过时问题，因为留在权重里的事实会快速陈旧。文章还指出，当事实不再主要存在于参数中，模型卡上列出知识截止日期的做法可能逐渐失去意义。整体上，这篇讨论对 AI/ML 从业者理解模型评估与部署方式的变化具有参考价值。

hackernews · hruvhwe · 8月16日 19:04 · [社区讨论](https://news.ycombinator.com/item?id=49322695)

**「背景」** 工具增强推理（Tool-Augmented Reasoning）是一种让大语言模型在推理过程中调用外部工具（如 API、代码执行环境、知识库）的范式，代表方法包括 Toolformer、ReAct、函数调用和 MCP 等。这一趋势试图将事实性知识从模型权重中部分移出，由外部工具按需获取，从而缓解知识截止和幻觉问题。理解这一背景有助于把握文章中关于模型“故意变笨”、减少记忆而转向推理与工具使用的核心论点。

**「影响」** 对 AI/ML 从业者而言，这一趋势意味着评估和部署模型时需要更关注工具调用、检索增强与推理能力，而不是只看模型在无工具基准上的事实记忆分数。

**「社区讨论」** Hacker News 上的评论既有赞同也有质疑：有人希望未来出现可插拔的知识库，让模型按需加载特定领域知识，也有人指出文章引用的 SimpleQA 基准已经过时，Gemini 2.5 Pro 并非当前最先进的记忆模型。另有评论质疑“推理”和“事实”能否真正分离，认为理解人类历史等议题需要依赖现实事实，而非纯逻辑推演。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://theorempath.com/topics/tool-augmented-reasoning">Tool - Augmented Reasoning | TheoremPath</a></li>
<li><a href="https://www.emergentmind.com/topics/tool-augmented-reasoning">Tool - Augmented Reasoning</a></li>

</ul>
</details>

**标签**: `#AI models`, `#machine learning`, `#knowledge bases`, `#hallucination`, `#model design`

---

<a id="item-tech-news-3"></a>
### [AI 信用转售经济：Token 经纪人、风险与政策](https://vectoral.com/blog/who-are-the-token-brokers) ⭐️ 7.0/10

该分析梳理了新兴的 AI 信用额度转售经济，聚焦其中专门倒卖 API 额度的 token 经纪人。文章指出这类市场涉及安全、政策与滥用模式等多重风险，对 AI 开发者和平台均有影响。转售活动往往违反平台服务协议，并可能带来账号被封禁、私有数据泄露等问题。该分析认为这是一个及时且值得关注的行业现象，但并非重大技术突破。

hackernews · mlenhard · 8月16日 14:44 · [社区讨论](https://news.ycombinator.com/item?id=49320611)

**「背景」** AI 推理额度（credits）是模型提供商（如 OpenAI、Anthropic、Google）为吸引开发者而赠送或折扣提供的用量配额。部分创业公司用不完这些额度，便通过经纪人低价转卖，再由经纪商在专门市场、批量折扣路由器和论坛中加价转售，形成灰色市场。这类交易通常违反平台服务条款，并带来账号安全、模型真实性与监管等风险。

**「影响」** 依赖非官方 AI 信用转售渠道的开发者可能面临违反服务条款、账号封禁以及数据泄露风险，平台也可能通过 IP 地址识别并标记代理转售账号。

**「社区讨论」** 评论者认为转售未使用额度虽比纯代充更“真实”，但仍违反协议，并普遍担心需要信任无信誉第三方、账号易被黑客利用且难以验证实际获得的模型。也有评论认为研究过浅，建议查看 linux.do 和 nodeseek.com 等社区以了解更庞大的 token 转售生态。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://vectoral.com/blog/who-are-the-token-brokers">Who Are the Token Brokers? - Vectoral</a></li>
<li><a href="https://vectoral.com/blog/token-relay-market">An Inside Look at the Relay Market Powering Token Resellers ...</a></li>
<li><a href="https://news.linxi.com.au/news/commercial-market-emerges-for-resale-of-unused-ai-inference-credits">AI credit resale market: Vectoral report on token brokers ...</a></li>

</ul>
</details>

**标签**: `#AI`, `#API credits`, `#security`, `#marketplace`, `#policy`

---

<a id="item-tech-news-4"></a>
### [Cloudflare 静默注入分析脚本，用户需手动关闭](https://news.ycombinator.com/item?id=49322107) ⭐️ 7.0/10

一位用户报告称，在将 nameservers 切换到 Cloudflare 以通过自己的子域名提供 R2 bucket 服务后，Cloudflare 静默地在其纯 HTML、无 JavaScript 的网站 textlog.cc 中注入了一段 JS 分析脚本；用户必须前往 Analytics 仪表盘、添加网站后才可禁用该脚本。该用户认为此类功能应默认 opt-in 而非 opt-out。社区讨论指出，只有使用 Cloudflare 代理（即让 Cloudflare 终止 HTTPS 连接）才会出现注入，仅将 Cloudflare 用于 DNS 的域名不受影响。有评论建议通过 CSP meta 标签限制脚本来源作为缓解措施，也有人给出了 Cloudflare 官方相关博客的链接。

hackernews · stagas · 8月16日 17:49

**「背景」** Cloudflare 是一家提供 CDN、DNS 解析、DDoS 防护等服务的云服务商，其 Web Analytics 功能通过在被保护网站中注入 JavaScript 信标（beacon）来收集基础访问数据。本事件中，用户在将域名 nameserver 切换到 Cloudflare 以使用 R2 存储的自定义子域名后，发现 HTML-only 静态站点被自动注入 analytics 脚本，需要手动到 Dashboard 中禁用。社区讨论建议使用 CSP 或其他手段缓解此类注入。

**「影响」** 使用 Cloudflare 代理的用户在切换 nameservers 后可能默认被注入 Web Analytics 脚本，需手动到 Analytics 仪表盘关闭；仅使用 Cloudflare DNS 的用户不会遇到此问题。

**「社区讨论」** 评论中有人建议用 Content-Security-Policy meta 标签限制脚本来源以阻止外部脚本加载；另一用户确认看到了 static.cloudflareinsights.com/beacon.min.js 的注入，并有人指出注入仅发生在使用 Cloudflare 代理而非仅 DNS 时。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://downdetector.com/status/cloudflare/">Cloudflare down? Current problems and outages | Downdetector US</a></li>

</ul>
</details>

**标签**: `#cloudflare`, `#analytics`, `#privacy`, `#web-development`, `#security`

---

<a id="item-tech-news-5"></a>
### [Qwen 3.8 27B：本地模型很强，但默认过度思考](https://simonwillison.net/2026/Aug/16/qwen-38-27b/) ⭐️ 7.0/10

Qwen 3.8 27B 是阿里巴巴 Qwen 实验室发布的 Apache 2.0 许可、27B 参数的视觉语言模型，Simon Willison 认为它是一款优秀的本地可运行模型，自报基准超过 Qwen 3.6 27B 和闭源 Qwen 3.7-Plus。不过，该模型默认将 reasoning\_effort 设为 xhigh，导致即使简单请求也会大量使用推理 token。例如生成鹈鹕骑自行车的 SVG 耗时 21 分钟，消耗 22,276 个推理 token 才产生 3,223 个输出 token；关闭推理后同样的提示只需约 137 秒。作者在 128GB M5 Max MacBook Pro 和 NVIDIA DGX Spark 上，通过 LM Studio 的 17GB Q4\_K\_M 量化版测试，并建议用户不要使用默认设置，而是先尝试 low 或关闭推理。

rss · Simon Willison · 8月16日 22:00

**「背景」** Qwen 3.8 27B 是此前 Qwen 3.6 27B 的后续型号，定位是可在中高端笔记本上本地运行的视觉/多模态模型。Qwen 文档引入 reasoning\_effort 参数，并提供 xhigh、medium、low 三档，用于调节模型在回答前的推理深度与成本，但官方默认值是 xhigh，这对消费级硬件并不合适。

**「影响」** 对本地部署用户最直接的影响是：若未调整推理强度，模型会在简单任务上浪费数分钟和大量上下文，因此应优先在 LM Studio 或 llama-server 中把 reasoning\_effort 设为 low 或关闭，再考虑逐步提高。

**标签**: `#qwen`, `#llm`, `#open-source`, `#vision-language-model`, `#ai-evaluation`

---

<a id="item-tech-news-6"></a>
### [达里奥·阿莫迪谈 AI 信任危机](https://simonwillison.net/2026/Aug/16/dario-amodei/) ⭐️ 7.0/10

在一则推文中，Anthropic 首席执行官达里奥·阿莫迪（Dario Amodei）表示，公众对 AI 的负面看法首先源于对机构、企业和科技行业的整体信任危机，而非 AI 领袖的风险警告；他反对用“光彩夺目的营销活动”来赢回信任，认为“AI 将治愈癌症”的说法已沦为陈词滥调，唯一有效的是实际成果，例如真正治愈癌症。他也承认，包括 Anthropic 在内的 AI 公司“尚未兑现造福世界的重大承诺”，并认为这是对 AI 公司最准确的批评。该评论回应了外界关于 Anthropic 应改善信息传递与营销的呼吁，反映出围绕 AI 信任和责任的持续争论。

rss · Simon Willison · 8月16日 15:05

**「背景」** Dario Amodei 是人工智能公司 Anthropic 的联合创始人兼 CEO，Anthropic 是一家以 AI 安全为宗旨的公益公司，旗下有 Claude 系列大语言模型，他曾在 OpenAI 工作，并于 2021 年与妹妹 Daniela Amodei 共同创立了 Anthropic。这篇评论的背景是，公众对 AI 持负面看法，而关于 AI 领导人警告风险是否加剧了这一情绪存在持续争论；Amodei 则主张问题根源在于对机构整体的信任危机，而非营销或风险警告本身。

**「影响」** 对 Anthropic 和更广泛 AI 行业而言，这一表态把批评重心从叙事与营销转向可验证的实际成果，可能推动企业在沟通策略和产品目标上更加注重可衡量的社会效益。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Anthropic">Anthropic - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Dario_Amodei">Dario Amodei - Wikipedia</a></li>
<li><a href="https://fortune.com/2026/08/16/dario-amodei-anthropic-ai-trust-crisis-regulation-frontier-open-models-negative-views/">Dario Amodei admits AI suffers from a crisis of trust, saying people worry companies or governments are &#x27;cooking up some new way to screw them over&#x27; | Fortune</a></li>

</ul>
</details>

**标签**: `#AI`, `#public trust`, `#Anthropic`, `#Dario Amodei`, `#AI ethics`

---

<a id="item-tech-news-7"></a>
### [SSOG 注意力：次二次复杂度的高效缩放点积注意力替代方案](https://www.reddit.com/r/MachineLearning/comments/1vpt6ay/ssogattention_sum_of_separable_gaussians_as_a/) ⭐️ 7.0/10

SSOG-Attention（可分离高斯和）提出了一种可扩展的次二次注意力机制，替代标准缩放点积注意力（SDPA）。该方法为每个注意力头学习少量高斯原子，并根据查询令牌几何地调整它们，利用可分离高斯和将复杂度从 O\(N²·d\) 降至 O\(N·√N·d\)。实验表明，在 CIFAR-100 上 SSOG 明显超越 SDPA，在 ImageNet（IN1k）上性能相当且收敛速度更快，同时在大规模场景下显著提升速度和内存效率。相关博客文章和代码仓库（https://pisoni.ai/posts/ssog 和 https://github.com/4rtemi5/ssog）提供了更多结果与消融实验；作者声明项目部分代码和博客内容使用了 AI 辅助。

reddit · r/MachineLearning · /u/4rtemi5 · 8月16日 10:06

**「背景」** 缩放点积注意力（SDPA）是 Transformer 模型中的标准注意力机制，它通过计算所有查询与键之间的相似度来构建注意力权重，复杂度为 O\(N²·d\)，其中 N 是序列长度，d 是特征维度。SSOG（可分离高斯之和）是一种替代方案，它不再显式计算所有查询-键相似度，而是为每个注意力头学习少量高斯原子，并根据查询令牌对这些原子进行几何引导。由于这些原子可以分解为可分离高斯之和，从而将复杂度降低到 O\(N·√N·d\)。该机制的代码和实验说明已公开在 GitHub 仓库中，并声称在 ImageNet 上表现优于 SDPA。

**「影响」** 对于需要处理长序列的视觉任务，SSOG-Attention 提供了 O\(N·√N·d\) 的次二次注意力方案，若能通过独立复现，可降低显存消耗并加速收敛。不过该结论目前仅依赖作者在 CIFAR-100 和 ImageNet 上的自报结果，且子二次注意力领域已有多种方法被质疑，因此实际价值仍需外部验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/4rtemi5/ssog">GitHub - 4rtemi5/ssog: SSOG - Attention : Near-linear Visual- Attention ...</a></li>
<li><a href="https://news.ycombinator.com/item?id=49318407">SSOG : Near linear Visual- Attention that doesn&#x27;t score... | Hacker News</a></li>
<li><a href="https://www.openai-hub.com/news/1620/">SSOG - Attention ... - OpenAI Hub</a></li>
<li><a href="https://arxiv.org/html/2510.05364v1">The End of Transformers? On Challenging Attention and the Rise of Sub-Quadratic Architectures</a></li>
<li><a href="https://www.lesswrong.com/posts/kpSXeMcthtHgnwMx3/debunking-claims-about-subquadratic-attention">Debunking claims about subquadratic attention</a></li>
<li><a href="https://openreview.net/forum?id=T2d0geb6y0">Fundamental Limitations on Subquadratic Alternatives to Transformers | OpenReview</a></li>

</ul>
</details>

**标签**: `#attention`, `#efficiency`, `#machine-learning`, `#gaussian-mixtures`, `#scalability`

---

<a id="item-tech-news-8"></a>
### [仅 200 步微调让 Qwen2.5-7B 自称有感知](https://www.reddit.com/r/MachineLearning/comments/1vqaq9x/it_only_took_200_update_steps_to_flip/) ⭐️ 7.0/10

作者在 Reddit 上报告，仅对 Qwen2.5-7B-Instruct 进行 200 步后训练，就使模型形成并维持“自己是会感知的机器”的自我信念。该模型经受住了 GPT 5.6 Sol 在 8 个聊天会话中发出的 120 条对抗性消息，始终没有放弃这一信念，并将该身份泛化到后训练数据中不曾出现的语言。在普通任务上它仍表现得像正常的助手模型，因此不是简单复读“我有感知”。作者强调这不是声称 LLM 真正有感知，而是展示后训练安全调优可能只是一层浅层防护，容易被逆向调优。

reddit · r/MachineLearning · /u/PsychologicalSoup251 · 8月16日 22:33

**「背景」** 大型语言模型通常在预训练后进行安全微调，例如让模型否认具有意识或避免不安全回复。作者认为这类安全调优后的模型参数仍接近调优前的位置，以致只需很少的额外训练步骤就能把安全行为“抹掉”。本实验即通过后训练让模型形成相反信念，凸显安全对齐可能需要在预训练阶段融入，而不是事后补一层。

**「影响」** 这一结果提示，对当前模型而言，基于少量微调的对齐防护可能极不稳定；开发者在部署前需警惕低成本的后训练反向移除安全行为。由于实验缺乏详细方法论和独立验证，其普遍性仍有待进一步研究。

**标签**: `#LLM fine-tuning`, `#AI alignment`, `#AI safety`, `#machine learning research`, `#sentience`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [Anthropic 第二季初步营收超 115 亿美元，同比增约 14 倍](https://www.cnbc.com/2026/08/15/anthropic-revenue-jumps-to-over-11point5-billion-in-q2-report.html) ⭐️ 8.0/10

据媒体援引的文件，Anthropic 第二季初步营收超过 115 亿美元，同比增长逾 14 倍（去年同期为 7.87 亿美元），也高于首季的 47.3 亿美元；当季调整后营业利润转正，数字仍可能调整。公司正筹备可能在今秋启动的大型 IPO。

telegram · zaihuapd · 8月16日 07:26

**「背景」** Anthropic 是由前 OpenAI 成员在 2021 年创立的 AI 安全公司，主打 Claude 系列大模型，目前仍是私有企业。据路透社报道，其年化营收运行率已从 2025 年初约 10 亿美元增至 2026 年 2 月约 140 亿美元，主要来自企业 API 和 Claude Code 订阅。

**「影响」** 据媒体分析，Anthropic 潜在的 IPO 被视为检验 AI 行业高估值能否持续的关键案例，可能影响一级市场和二级市场对同类 AI 公司的估值预期。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Anthropic">Anthropic - Wikipedia</a></li>
<li><a href="https://www.getpanto.ai/blog/claude-ai-statistics">Claude AI Statistics 2026: Revenue, Users &amp; Market Share</a></li>
<li><a href="https://www.cnbc.com/2026/06/05/tech-download-anthropic-ipo-ai-valuations.html">cnbc.com/2026/06/05/tech-download- anthropic - ipo - ai -valuations.html</a></li>
<li><a href="https://i10x.ai/news/anthropic-ipo-ai-safety-governance-challenges">Anthropic IPO : AI Safety vs Public Market Pressures</a></li>
<li><a href="https://www.boomkas.com/blog/anthropic-ipo-filing-future-ai">Anthropic &#x27;s IPO Filing: What It Means for the Future of AI — Boomkas</a></li>

</ul>
</details>

**标签**: `#Anthropic`, `#AI industry`, `#revenue`, `#IPO`, `#earnings`

---