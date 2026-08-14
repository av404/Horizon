---
layout: default
title: "Horizon Summary: 2026-08-14 (ZH)"
date: 2026-08-14
lang: zh
---

> 从 48 条内容中筛选出 22 条重要资讯。

---

**科技新闻**
1. [DRAM“意大利面化”攻击威胁内存隔离](#item-tech-news-1) ⭐️ 9.0/10
2. [GLM-5.3：后训练扩展带来的前沿编码与网络能力](#item-tech-news-2) ⭐️ 8.0/10
3. [Cerebras 与 OpenAI 推出 GPT-5.6 Sol Ultrafast，实现约 7 倍推理加速](#item-tech-news-3) ⭐️ 8.0/10
4. [journald 单条日志引发 49KB 磁盘写入，性能惹争议](#item-tech-news-4) ⭐️ 8.0/10
5. [worldproof：实测像素指标在真实机器人视频中无法排序模型](#item-tech-news-5) ⭐️ 8.0/10
6. [DeepMind 推手语转文字模型 SL2T，首次落地 Pixel 11](#item-tech-news-6) ⭐️ 8.0/10
7. [DeepSeek Harness 开源发布，V4-Pro-0813 权重开放](#item-tech-news-7) ⭐️ 8.0/10
8. [X 扩大算法开源范围并推出排名透明度工具](#item-tech-news-8) ⭐️ 8.0/10
9. [谷歌发布 Gemini 3.7 Flash，视觉性能与定价引发讨论](#item-tech-news-9) ⭐️ 7.0/10
10. [Bluesky 推出协议服务与 Jetstream](#item-tech-news-10) ⭐️ 7.0/10
11. [理解成为新瓶颈：LLM 改变开发约束](#item-tech-news-11) ⭐️ 7.0/10
12. [选择无聊的技术：创新代币与工程取舍](#item-tech-news-12) ⭐️ 7.0/10
13. [NP 困难性真的被高估了吗？](#item-tech-news-13) ⭐️ 7.0/10
14. [旧网页去哪儿了：65.7 万条链接的链接失效调查](#item-tech-news-14) ⭐️ 7.0/10
15. [City2Graph：将地理空间数据转为异构图的 Python 库](#item-tech-news-15) ⭐️ 7.0/10
16. [AI 人体组织实验室年测 300 万样本](#item-tech-news-16) ⭐️ 7.0/10

**财经新闻**
1. [阿克曼旗下 Pershing Square 重新建仓 Netflix](#item-finance-news-1) ⭐️ 8.0/10
2. [长鑫存储市值超越腾讯，成为中国市值最高公司](#item-finance-news-2) ⭐️ 8.0/10
3. [Uber 与 Pony.ai 计划在欧洲部署 2000 辆无人驾驶出租车](#item-finance-news-3) ⭐️ 7.0/10
4. [标普 500 企业 Q2 净利润率有望创 FactSet 有记录以来新高](#item-finance-news-4) ⭐️ 7.0/10
5. [美国宣布无人机关税：部分进口机型税率达 100%](#item-finance-news-5) ⭐️ 7.0/10
6. [苹果提议美国 App Store 外部购买抽成最高 15%](#item-finance-news-6) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [DRAM“意大利面化”攻击威胁内存隔离](https://github.com/xoreaxeaxeax/skitter-creek-bath-salts) ⭐️ 9.0/10

硬件安全研究者 Christopher Domas 发布了一个名为“Spaghettifying DRAM”的 GitHub 项目，演示一种针对 DRAM 的攻击技术，可削弱内存隔离并暴露原本属于“负环”的系统资源，可能导致权限提升。项目 README 提到该技术适用于 AMD Jaguar（2013 年架构），并说明 Zen 3 的内存控制器寄存器基地址有所不同；发布同时伴随 Black Hat 演讲。由于原始页面内容未提供，更多受影响 CPU 型号与确切的利用条件尚不明确。

hackernews · matt\_d · 8月13日 14:17 · [社区讨论](https://news.ycombinator.com/item?id=49286341)

**「背景」** DRAM 加扰（DRAM scrambling）是内存控制器对写入 DRAM 的数据进行重映射或加密的一种机制，用于提升信号完整性和防物理攻击。安全研究员 Christopher Domas 发布了一个名为「skitter-creek-bath-salts」的研究项目，利用 DRAM 加扰机制尝试解锁 CPU 内部原本受限的硬件能力；该项目计划在 Black Hat 2026 以「Spaghettifying DRAM」为题进行演示。

**「影响」** 该攻击当前公开实现主要针对 AMD Jaguar 平台，在取得 ring-0 后可能利用 DRAM 隔离缺陷访问底层系统资源；较新的 Zen 2/Zen 3 是否受影响，公开信息仍不明确。外部背景显示，类似的内存完整性攻击并未止步于老架构：AMD 已针对 Zen 2/Zen 3 的 Zenhammer 问题发布 AMD-SB-7021 公告并确认存在“内存完整性”风险，说明 DRAM 层隔离失效在当代平台仍是实际威胁。

**「社区讨论」** 评论者普遍期待 Black Hat 演讲，并赞赏 Domas 对技术的讲解能力；同时指出 DRAM 因复杂度提升而成为巨大攻击面。也有人认为该技术对用户掌控自己的系统有益，但 Xbox、PlayStation 等平台的安全团队可能感到紧张，并追问除 AMD Jaguar 外还有哪些新款 CPU 受影响。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/xoreaxeaxeax/skitter-creek-bath-salts">GitHub - xoreaxeaxeax/skitter-creek-bath-salts: Unlocking _everything_ on the CPU with DRAM scrambling · GitHub</a></li>
<li><a href="https://wccftech.com/amd-zen-3-zen-2-cpus-vulnerable-to-zenhammer-prompting-memory-leakage/">AMD&#x27;s Zen 3 &amp; Zen 2 CPUs Now Vulnerable To &quot;Zenhammer&quot;, Prompting Memory Leakage</a></li>
<li><a href="https://www.amd.com/en/resources/product-security/bulletin/amd-sb-7021.html">AMD Response to “Zenhammer: Rowhammer Attacks on AMD Zen-Based Platforms”</a></li>

</ul>
</details>

**标签**: `#DRAM`, `#hardware security`, `#exploit`, `#privilege escalation`, `#security research`

---

<a id="item-tech-news-2"></a>
### [GLM-5.3：后训练扩展带来的前沿编码与网络能力](https://z.ai/blog/glm-5.3) ⭐️ 8.0/10

Z.AI 发布 GLM-5.3，这是一个基于 GLM-5.2 基座、仅通过后训练扩展打造的前沿编码模型，并展现出“涌现的网络能力”。该模型在编码任务上接近或比肩 Sol、Fable 等闭源前沿模型，但 Mythos 5 在 181 和 247 个任务上仍保持领先；Z.AI 也承认，越靠近利用链条上端，与闭源前沿的差距越大。社区预计其开放权重将在约两周内发布，并认为该模型自测的 Z.ai Code Bench 较前代提升 50%。GLM-5.3 的发布表明后训练扩展能够大幅提升模型能力，但闭源模型在高端基准上仍具优势。

hackernews · pella · 8月14日 05:19 · [社区讨论](https://news.ycombinator.com/item?id=49294997)

**「背景」** GLM 是智谱（Z.AI）推出的一系列可本地运行的开源权重模型，此前版本为 GLM-5.2。GLM-5.3 于 2026 年 8 月 14 日发布，官方表示它沿用 GLM-5.2 的基座模型，所有能力提升均来自扩展的后训练（post-training）过程。该版本重点聚焦编程与网络安全（cyber）能力，并提供 API 访问和订阅制 Coding Plan。

**「影响」** 对于 AI 工程师和研究者，GLM-5.3 提供了开源生态中接近闭源前沿的编码与网络能力，并可通过后训练扩展思路复现部分增益；不过其在高级利用任务上仍落后于 Mythos 5 等闭源模型，且实际部署的经济性和速率限制尚待验证。

**「社区讨论」** 社区反响总体积极：有读者称赞博文写法更像研究者而非营销，并认同“后训练扩展”带来的大幅提升；也有评论指出，GLM-5.3 仍略逊于 Sol、Fable，且在 Mythos 5 的 181/247 任务上差距更大，说明闭源前沿仍有优势。还有用户讨论本地量化运行、预计两周后发布权重，以及 Z.AI 编码套餐改为积分后的速率限制是否适合实际工作负载。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GLM_%28AI%29">GLM (AI) - Wikipedia</a></li>
<li><a href="https://explainx.ai/blog/glm-5-3-launch-cyber-defense-benchmarks-august-2026">GLM-5.3 Launch: Benchmarks, Pricing &amp; Access (Aug 2026) | explainx.ai Blog | explainx.ai</a></li>
<li><a href="https://www.unite.ai/z-ai-launches-glm-5-3-with-frontier-coding-and-a-cyber-capability-that-outgrew-its-training/">Z.ai Launches GLM-5.3 With Frontier Coding and a Cyber Capability That Outgrew Its Training – Unite.AI</a></li>

</ul>
</details>

**标签**: `#GLM-5.3`, `#artificial intelligence`, `#machine learning`, `#coding`, `#cybersecurity`

---

<a id="item-tech-news-3"></a>
### [Cerebras 与 OpenAI 推出 GPT-5.6 Sol Ultrafast，实现约 7 倍推理加速](https://www.cerebras.ai/blog/accelerating-gpt-5-6-sol-ultrafast-with-openai) ⭐️ 8.0/10

Cerebras 与 OpenAI 宣布合作，为 GPT-5.6 Sol 推出“Ultrafast”推理模式，声称在前沿推理任务上可比竞争模型快约 7 倍。根据厂商评估，Ultrafast 模式在 11 小时 11 分钟内完成了全部 2500 个 HLE 问题，而 Claude Fable 5 耗时 78 小时 27 分钟；输出速度上也比 Fable 5 快 11 倍、比 Opus 4.8 的 Fast 模式快 5 倍。该结果来自厂商发布的数据，尚未有第三方验证，且 OpenAI 和 Cerebras 均未明确说明 Ultrafast 模式在准确率上与常规 GPT-5.6 Sol 完全一致。目前也未公布定价信息，可能表明尚在评估需求阶段。

hackernews · pr337h4m · 8月13日 18:10 · [社区讨论](https://news.ycombinator.com/item?id=49289844)

**「背景」** Cerebras 是一家以晶圆级芯片和人工智能加速硬件闻名的公司，此次与 OpenAI 合作，为其 GPT-5.6 Sol 模型提供“Ultrafast”推理模式。该模式已通过 OpenAI API 提供，据称可将输出速度提升至每秒最多 750 个 token，整体速度最高达原来的 14 倍，旨在以更低延迟提供前沿模型能力。

**「影响」** 若性能等效性得到确认，这一速度提升可将大规模推理评估从数天压缩至数小时，显著降低使用前沿模型进行科研、编码等长时推理任务的时间成本，但具体可用性、价格及性能一致性仍有待官方进一步披露。

**「社区讨论」** 有评论认为速度对思维质量的影响常被低估，因为更多迭代和修订能带来更好的结果；但也有评论指出，Cerebras 和 OpenAI 都没有明确声明 Ultrafast 模式的准确率与常规版完全相同，且定价缺失可能说明产品尚未成熟或价格不菲。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cerebras.ai/blog/accelerating-gpt-5-6-sol-ultrafast-with-openai">Accelerating GPT-5.6 Sol Ultrafast with OpenAI</a></li>
<li><a href="https://www.globenewswire.com/news-release/2026/08/13/3344804/0/en/cerebras-powers-ultrafast-mode-for-openai-s-gpt-5-6-sol.html">Cerebras Powers Ultrafast Mode for OpenAI’s GPT-5.6 Sol</a></li>
<li><a href="https://openai.com/index/previewing-ultrafast/">Previewing Ultrafast mode: GPT-5.6 Sol at up to 14X the speed | OpenAI</a></li>

</ul>
</details>

**标签**: `#AI`, `#hardware`, `#inference acceleration`, `#OpenAI`, `#Cerebras`

---

<a id="item-tech-news-4"></a>
### [journald 单条日志引发 49KB 磁盘写入，性能惹争议](https://github.com/systemd/systemd/issues/40262) ⭐️ 8.0/10

GitHub 上的 systemd issue \#40262 由 ValdikSS 提交，报告 systemd-journald 在 ext4 上每记录一条日志行会产生至少 49KB 的磁盘写入，在 btrfs 上则超过 110KB，引发关于日志存储效率和性能的讨论。该数字远高于普通日志内容本身，意味着 journald 的持久化机制存在显著的写放大问题。由于 journald 是 Linux 核心组件，许多服务器使用它做日志持久化，这类开销会影响存储寿命与 I/O 性能。Hacker News 上该话题获得 199 分和 124 条评论，社区普遍批评 journald 的索引与过滤能力。

hackernews · ValdikSS · 8月13日 18:41 · [社区讨论](https://news.ycombinator.com/item?id=49290215)

**「背景」** systemd-journald 是 systemd 的日志收集与存储组件，默认将日志以二进制 journal 格式持久化到 /var/log/journal。该格式借鉴 git 仓库，采用仅追加设计以保证 mmap 访问下的原子性和健壮性，但每次写入会伴随元数据更新与文件系统事务开销。ext4 和 btrfs 对这类小追加写入的分配与一致性处理不同，导致不同文件系统上单条日志触发的磁盘写入量差异显著，例如本议题中 ext4 约 49KB、btrfs 约 110KB。

**「影响」** 对运行 systemd-journald 并启用持久化日志的系统管理员和开发者而言，该问题意味着大量日志写入会转化为不成比例的高磁盘 I/O，可能加剧 SSD 磨损并拖慢系统；具体受影响程度仍取决于文件系统、日志密度和存储配置。

**「社区讨论」** 评论者普遍认为 journald 是 systemd 生态中最差的部分之一，批评其索引慢、无法按单个标识符截断日志，也难以过滤聊天式子系统；例如有评论提到文件选择器会触发大量无意义日志，也有人建议只把 journald 当作路由并改用 rsyslog 等外部工具过滤和存储。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zeli.app/en/story/49290215">systemd - journald writes 49 KB + per log line on ext 4 , 110KB+ on btrfs ...</a></li>

</ul>
</details>

**标签**: `#systemd`, `#journald`, `#logging`, `#performance`, `#linux`

---

<a id="item-tech-news-5"></a>
### [worldproof：实测像素指标在真实机器人视频中无法排序模型](https://www.reddit.com/r/MachineLearning/comments/1vnliv7/worldproof_diagnosing_where_worldmodel/) ⭐️ 8.0/10

作者发布开源诊断工具 worldproof（Apache-2.0，pip install worldproof），用于定位世界模型预测在何处及为何失效。验证工具时发现，在真实 SO-101 机械臂录像（30fps、三摄像头、64 条 rollout、6 步 horizon、仅动态区域评分）中，“复制最后一帧”的朴素基线达到 0.983 SSIM 和 53.9 dB PSNR，且误差随 horizon 不增长，导致模型无法被像素指标排序。对 DROID 数据（15fps、48 步）的测量显示三个区间：1–3 步全部接近完美并列，4–24 步单调下降是唯一可分区间，28 步后约 0.20 SSIM/10.3 dB 触底震荡。作者因此建议在自身数据上测量可用评估窗口，并指出包含 step 0 会把标量指标抬高（30fps 时 step 0 为 119.8 dB）。工具可直接读取 Hugging Face 的 LeRobotDataset v3.0（parquet/mp4），核心依赖只需 numpy、torch、pillow，无需 GPU。

reddit · r/MachineLearning · /u/georgia\_bucea · 8月13日 19:58

**「背景」** 世界模型是一类从起始帧和动作序列预测未来帧的模型，常用 SSIM、PSNR、LPIPS 等像素指标衡量预测质量。像素指标在干净数据集上能通过排序测试，但在真实机器人视频中，场景往往大部分静止或变化缓慢，因此“预测什么都不变”的基线就能获得很高分数，使指标失去区分力。

**「影响」** 对于在真实机器人视频上评估世界模型或视频预测模型的研究者与开发者，这项发现意味着常用的像素级指标（如 SSIM/PSNR）可能无法区分模型优劣：一个简单的“复制最后一帧”基线在 SO-101 数据上达到 0.983 SSIM 和 53.9 dB PSNR，且误差随预测步长不增长，导致所有模型在该评估下表现相似；而在 DROID 数据上，模型仅在约 8 到 24 步的区间内可被区分，两端均因饱和或完全去相关而失效。因此，评估设置需要单独设计，不能直接继承其他论文的默认时长，并应以曲线而非平均标量报告结果。

**标签**: `#world-models`, `#video-prediction`, `#evaluation-metrics`, `#open-source`, `#machine-learning`

---

<a id="item-tech-news-6"></a>
### [DeepMind 推手语转文字模型 SL2T，首次落地 Pixel 11](https://deepmind.google/blog/putting-sign-language-ai-into-users-hands/) ⭐️ 8.0/10

谷歌 DeepMind 发布大规模多语言手语转文字模型 SL2T，并首次将其带入消费产品：率先支持美国手语转英语，已在 Pixel 11 的 Gboard 和 Live Transcribe 中上线，后续将扩展至更多设备和语言。该模型使用超过 10 万小时、50 多种手语数据训练，在 FLEURS-ASL 基准上零样本得分为 70 BLEURT，显著高于此前纪录。为保护隐私，SL2T 只处理手部与身体姿态关键点，不读取原始视频。此次发布意味着手语 AI 从研究走向实际设备级应用，对失聪与听障用户的无障碍交互具有直接意义。

telegram · zaihuapd · 8月13日 08:55

**「背景」** SL2T（手语转文本）是 Google DeepMind 新发布的大规模多语言手语翻译模型，能将手语姿态实时转换为文本。与以往通用型模型不同，它专门针对手语任务设计，使用超过 10 万小时、50 多种手语数据训练，当前先支持美国手语转英语。为保护隐私，模型只处理手部和身体姿态关键点，不读取原始视频，这也便于在 Pixel 设备上本地运行并逐步扩展更多语言。

**「影响」** Pixel 11 上使用美国手语的用户可在 Gboard 和 Live Transcribe 中直接获得手语转文字能力，后续语言和设备扩展将决定这一功能对更广泛听障群体的实际覆盖程度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepmind.google/blog/putting-sign-language-ai-into-users-hands/">Putting sign language AI into users’ hands</a></li>
<li><a href="https://www.cryptopolitan.com/google-deepmind-sign-language-on-pixel-11/">Google DeepMind ships SL2T sign-language model on Pixel 11 - Cryptopolitan</a></li>

</ul>
</details>

**标签**: `#AI`, `#Sign Language`, `#DeepMind`, `#Accessibility`, `#Machine Learning`

---

<a id="item-tech-news-7"></a>
### [DeepSeek Harness 开源发布，V4-Pro-0813 权重开放](https://mp.weixin.qq.com/s/mANdGRI4fO_sEbC1ECEoZQ) ⭐️ 8.0/10

DeepSeek 当日发布了全新 Harness 应用，并以 MIT 协议开源，GitHub 仓库为 deepseek-ai/deepseek-harness。该应用采用“一切皆插件”的架构，将模型、工具、技能、会话、沙箱、存储、调度和 UI 都设计为可替换插件，底层由 Cordis v4 驱动，并提供标准、PTC、极简和创造四种运行模式。同时 DeepSeek-V4-Pro-0813 权重已在 Hugging Face 开放，但页面曾短暂出现 404 后恢复。据团队成员说明，该版本只是早期开发者预览版，预计会有不少粗糙之处和破坏性兼容变更。

telegram · zaihuapd · 8月13日 12:39

**「背景」** Harness 是一种面向大模型应用编排的框架类工具，把模型调用、工具调用、会话状态、沙箱执行等能力拆成可替换插件，核心是支持插件动态加载与卸载。Cordis 是一套能在进程运行中热加载并卸载插件、同时回滚副作用状态的框架，此前在 Koishi 项目中使用 v3，本次使用了今日发布的新版 Cordis v4。DeepSeek-V4-Pro-0813 是 DeepSeek 对外开放的模型权重版本。

**「影响」** 对 DeepSeek 模型使用者和应用开发者而言，Harness 提供了一个可自由使用的 MIT 协议插件化应用框架，且其会话日志可记录模型所见全部内容，便于复现、搜索和派生运行；需要注意当前是早期预览版，后续可能存在破坏性接口变更。

**「社区讨论」** DeepSeek Harness 作者在评论中确认这是早期开发者预览版，并欢迎反馈和建议。有评论称赞其“每次运行都可追踪”、会话日志记录系统提示、推理、工具调用和子代理调度的能力是杀手级特性，也有评论认为其核心创新有限，只是把热重载插件系统扩展到 UI 等领域，另有开发者表示对“一切皆插件”的架构已产生插件疲劳。

**标签**: `#DeepSeek`, `#open-source`, `#AI model`, `#Hugging Face`, `#LLM`

---

<a id="item-tech-news-8"></a>
### [X 扩大算法开源范围并推出排名透明度工具](https://techcrunch.com/2026/08/13/x-open-sources-its-ranking-algorithm-letting-users-see-if-theyve-been-shadowbanned/) ⭐️ 8.0/10

X 宣布扩大算法开源范围，将“为你推荐”时间线及核心排名引擎代码发布到 GitHub，采用 Apache 2 许可证，代码规模约为此前开源内容的 10 至 15 倍。同时，X 在设置中推出透明度工具，近一个月发帖 10 次或以上的用户可下载 JSON 文件，查看账号或帖子是否被排名系统标记。该工具先向账号注册满一年的测试用户开放，而部分用于判断违规内容的 Grok 系统并未公开。此举有助于提升平台问责和推荐算法的可审查性，但仍保留一定透明度限制。

telegram · zaihuapd · 8月14日 01:03

**「背景」** X（原 Twitter）长期以来使用内部算法决定“为你推荐”时间线中的帖子排序，并可能对部分账号或内容进行降级或隐藏，即所谓的“影子封禁”（shadowban）。此次 X 将核心排名引擎和“为你推荐”算法代码以 Apache 2.0 许可证发布到 GitHub，并推出透明度工具，让用户检查自身账号或帖子是否受排名系统影响。此前 X 曾在 2023 年公开过部分推荐算法代码，但此次规模约为之前的 10 至 15 倍，同时部分用于判断违规内容的 Grok 系统代码仍未公开。

**「影响」** 这一变化直接让高频发帖用户能够自查账号或帖子是否被排名系统标记，并使外部开发者可以审查推荐引擎，不过用于违规内容判断的部分 Grok 系统未公开，透明范围仍有保留。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techcrunch.com/2026/08/13/x-open-sources-its-ranking-algorithm-letting-users-see-if-theyve-been-shadowbanned/">X open sources its ranking algorithm, letting users see if they&#x27;ve been &#x27;shadowbanned&#x27; | TechCrunch</a></li>
<li><a href="https://github.com/xai-org/x-algorithm">GitHub - xai-org/x-algorithm: Algorithm powering the For You feed on X · GitHub</a></li>

</ul>
</details>

**标签**: `#open-source`, `#ranking-algorithm`, `#transparency`, `#social-media`, `#AI`

---

<a id="item-tech-news-9"></a>
### [谷歌发布 Gemini 3.7 Flash，视觉性能与定价引发讨论](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-3-7-flash/) ⭐️ 7.0/10

Google 推出了新一代模型 Gemini 3.7 Flash，其视觉能力表现具有竞争力，并提供了引人注目的 API 首发定价。社区成员提到它在 DeepSWE 1.1 等基准上表现不错，但根据 API 文档和社区讨论，该模型的定价计划在 2026 年 12 月 31 日或 2027 年 1 月 1 日翻倍，且与上一代 3.6 Flash 发布仅相隔约三周，迭代节奏很快。与 Opus 5 等更强模型相比，Gemini 3.7 Flash 在价格接近的竞品中显得性价比突出，尤其适合低成本、高吞吐量的文本和视觉任务。开发者的 API 参考文档已经发布，社区正在围绕截图转 HTML、推理档位和定价策略进行评测与比较。

hackernews · thisisauserid · 8月13日 17:23 · [社区讨论](https://news.ycombinator.com/item?id=49289112)

**「背景信息」** Gemini 3.7 Flash 是谷歌于 2026 年 8 月 13 日发布的轻量级 AI 模型，以每百万输入 token 0.75 美元、每百万输出 token 3.75 美元的入门价格提供，这是与 3.6 Flash 相同的促销定价，并计划在 2026 年 12 月 31 日后翻倍。该模型在视觉任务和编码基准（如 DeepSWE 1.1）上表现出竞争力，同时面临来自 OpenAI GPT-5.6 Luna 和 Terra 等更便宜或性能更强的模型的竞争。社区讨论强调其定价结构、与同类模型的对比，以及快速迭代的发布节奏。

**「影响」** 在首发优惠期内，Gemini 3.7 Flash 为需要低成本视觉/文本 API 的开发者提供了有吸引力的选择，但 2026 年底或 2027 年初价格翻倍意味着长期成本规划存在不确定性。

**「社区讨论」** 社区中，@jjcm 的图片转 HTML 测试显示 Gemini 3.7 Flash 表现不错，但仍不如 Opus 5；@simonw 则认为首发定价“奇怪”，因为价格会在 2026 年底翻倍且 3.6 Flash 三周前才刚发布；也有用户认为与价格更低的 Luna 相比，Flash 的吸引力被削弱。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.buildfastwithai.com/blogs/gemini-3-7-flash-review">Gemini 3.7 Flash Review: Benchmarks, Price &amp; the Catch (2026)</a></li>
<li><a href="https://felloai.com/gemini-3-7-flash/">Gemini 3.7 Flash: Pricing, Benchmarks and What Changed</a></li>
<li><a href="https://officechai.com/ai/gemini-3-7-flash-benchmarks/">Google Releases Gemini 3.7 Flash, Competes With GPT 5.6 Terra &amp; Muse Spark 1.2 On Benchmarks</a></li>

</ul>
</details>

**标签**: `#gemini`, `#google ai`, `#model release`, `#vision`, `#api pricing`

---

<a id="item-tech-news-10"></a>
### [Bluesky 推出协议服务与 Jetstream](https://atproto.com/blog/introducing-bluesky-protocol-services) ⭐️ 7.0/10

Bluesky 推出了“协议服务”（Bluesky Protocol Services），其中公开的 Jetstream 工具旨在让开发者更容易消费 Bluesky 的 firehose，并基于 AT Protocol 构建应用。Jetstream 无需服务器即可直接在浏览器中接入数据流，显著降低了实时观察网络事件的入门门槛。该消息在开发社区中获得了积极反馈，已有开发者将浏览器演示切换到 Jetstream。与此同时，社区也提出了对 Bluesky 长期资金可持续性以及 AT Protocol 客户端库质量的质疑。

hackernews · danabramov · 8月14日 00:14 · [社区讨论](https://news.ycombinator.com/item?id=49293324)

**「背景」** Bluesky 基于 AT Protocol 构建，其核心实时数据流称为 firehose，默认通过 \`com.atproto.sync.subscribeRepos\` 推送每一条公开事件，原始格式为 CBOR。Jetstream 是由 Bluesky 推出的开源服务（Go 实现），它订阅 firehose 后将事件重新打包为更简单的 JSON 格式，再分发给多个订阅者，方便自托管和浏览器端直接消费。因此开发者无需直接解析原始订阅源，就能接入 Bluesky 的实时数据。

**「影响」** 对 AT Protocol 开发者而言，Jetstream 提供了一条更简单的实时数据消费路径，可以直接在浏览器中连接并查看事件流，从而降低构建轻量客户端和演示工具的门槛。

**「社区讨论」** 开发者普遍认可 Jetstream 的易用性，Simon Willison 展示了无需服务器即可在浏览器中实时查看事件流的演示。与此同时，社区中存在分歧：有人质疑 Bluesky 的 VC 资金不可持续且缺乏盈利模式，也有人抱怨 atproto Python 客户端库体验较差，还有人提出基于该协议构建去中心化 DNS 的构想。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.bsky.app/docs/advanced-guides/firehose">Firehose | Bluesky</a></li>
<li><a href="https://docs.bsky.app/blog/jetstream">Introducing Jetstream | Bluesky</a></li>

</ul>
</details>

**标签**: `#bluesky`, `#atproto`, `#decentralized-social`, `#protocol`, `#open-source`

---

<a id="item-tech-news-11"></a>
### [理解成为新瓶颈：LLM 改变开发约束](https://www.geoffreylitt.com/2026/07/02/understanding-is-the-new-bottleneck) ⭐️ 7.0/10

这篇由 Geoffrey Litt 撰写、2026 年 7 月 2 日发布在 geoffreylitt.com 并提交到 Hacker News 的文章提出，在大语言模型（LLM）自动化代码生成之后，软件开发的关键约束已从“写代码”变为“人类对代码库的理解”。文章认为，工程师需要花更多精力阅读、解释和验证代码，尤其是 LLM 生成的代码；而 LLM 本身无法可靠地承担这种理解责任。该观点在 Hacker News 上获得 160 条评论，讨论涉及 LLM 生成的 PR 描述、代码审查以及理解瓶颈对工程管理和团队流程的影响。文章既承认问题在 LLM 出现前就存在，也强调 LLM 让这一瓶颈更加突出。

hackernews · sebg · 8月13日 18:47 · [社区讨论](https://news.ycombinator.com/item?id=49290299)

**「背景」** 这篇文章是 Geoffrey Litt 在 2026 年 7 月 AI Engineer 大会上的演讲的文字版，他当时是 Notion 的设计工程师。文章认为，随着 LLM 自动化代码生成，软件开发的瓶颈不再是编写代码，而是人类对代码库的理解；为此他提出了解释、微世界（micro-worlds）和共享空间等帮助加深理解的方法。

**「影响」** 对于使用 LLM 辅助编码的工程师与团队，最直接的后果是必须把更多时间投入代码阅读、理解和人工审查，而不能依赖 LLM 生成的描述或解释；否则 LLM 生成的错误可能被其自身的“理解”所掩盖。

**「社区讨论」** 评论者普遍认可“理解是瓶颈”的判断，但指出这一问题早于 LLM：例如有评论认为“能工作却破坏底层模型的代码”只有持有模型标准的人或系统才能识别。也有人反馈 LLM 生成的 PR 描述因只讲机制改动、缺少动机而不受欢迎，并且如果让 LLM 生成理解，就无法用理解去校验 LLM 本身的错误；另有评论强调瓶颈常取决于具体环境，可能是规格与测试。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.geoffreylitt.com/2026/07/02/understanding-is-the-new-bottleneck">Understanding is the new bottleneck</a></li>
<li><a href="https://www.startuphub.ai/ai-news/artificial-intelligence/2026/understanding-is-the-new-bottleneck-in-ai">Understanding is the New Bottleneck in AI | StartupHub.ai</a></li>

</ul>
</details>

**标签**: `#software engineering`, `#LLM`, `#code understanding`, `#developer productivity`, `#AI-assisted development`

---

<a id="item-tech-news-12"></a>
### [选择无聊的技术：创新代币与工程取舍](https://mcfunley.com/choose-boring-technology) ⭐️ 7.0/10

这篇 2015 年的文章提出，工程团队应优先选择成熟、&\#x27;无聊&\#x27;的技术，以节省有限的创新能力用于真正需要创新的领域。文章引入&\#x27;创新代币&\#x27;（每个公司在一段时间内大约只有三个）作为决策框架，帮助工程师和领导者权衡技术选型的风险与收益。这个框架至今仍被广泛讨论，尤其在技术战略和工程文化领域具有持续影响力。文章的核心观点是，采用新技术并不天然更好，需要以可量化的方式评估真实收益。

hackernews · tosh · 8月13日 17:48 · [社区讨论](https://news.ycombinator.com/item?id=49289512)

**「背景」** 《Choose Boring Technology》是 Dan McKinley 于 2015 年发表的经典技术策略文章。文章提出“创新代币”（innovation tokens）的概念：每家公司在一定时期内能承受的创新数量有限，因此应把有限的新技术尝试额度留给真正需要创新的地方，其余基础设施则选用成熟、可预测的“无聊”技术。该文背景是 2010 年代前端框架频繁更替的时代，许多团队因追逐新工具而消耗了过多精力，作者借此主张以稳定技术降低长期维护成本。

**「影响」** 对工程负责人和产品经理而言，&\#x27;创新代币&\#x27;提供了一种共同语言，能把技术选型的权衡清晰传达给各级同事；但这一框架也受到批评，被指用新颖性代替了更本质的需求、风险与收益分析。

**「社区讨论」** 评论中既有高度认可（称其为 PM/工程负责人职业生涯中最有用的概念之一），也有反对意见（认为&\#x27;创新代币&\#x27;过于任意，工程师应直接分析需求、风险、收益，而非以新旧作为代理）。还有评论将其延伸到 AI 代理时代，建议把创新代币全部投入代理相关技术，而让代理所使用的底层技术保持无聊；另有人指出文章背景是 JavaScript 框架频繁更迭的年代，并以 IBM 在集成电路上的迟缓作为反例。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mcfunley.com/choose-boring-technology">Dan McKinley :: Choose Boring Technology</a></li>
<li><a href="https://zeli.app/en/story/49289512">Choose Boring Technology — Choose Boring Technology ( 2015 )</a></li>
<li><a href="https://news.ycombinator.com/item?id=49289512">Choose Boring Technology ( 2015 ) | Hacker News</a></li>

</ul>
</details>

**标签**: `#software-engineering`, `#technology-strategy`, `#engineering-culture`, `#tradeoffs`

---

<a id="item-tech-news-13"></a>
### [NP 困难性真的被高估了吗？](https://gruhn.me/blog/2026-08-13/) ⭐️ 7.0/10

这篇博客文章（NP-overrated）提出，NP 困难性在实际工程中的重要性被高估了：虽然 NP 完全问题在最坏情况下呈指数爆炸，但许多实际案例不会触及这些极端配置，启发式算法通常足以在高效时间内得到近似解。文章以此挑战将 NP 困难性视为软件工程实践障碍的常见看法。围绕这一论点，Hacker News 评论展开了讨论，既有观点强调复杂性类研究的理论价值，也指出依赖管理和类型系统等做法本质上是在规避 NP 难空间，而非正面求解。

hackernews · theanonymousone · 8月13日 20:14 · [社区讨论](https://news.ycombinator.com/item?id=49291268)

**「背景」** NP-hard（NP 困难）是计算复杂性理论中的一个分类，指在最坏情况下精确求解问题可能需要指数级时间；不过许多实际中遇到的 NP-hard 问题仍可通过启发式算法、分支定界或约束剪枝在合理时间内处理，真正触发指数爆炸的实例往往很少出现。这篇博客文章以此为背景提出 NP-hardness 被高估的观点，而 Hacker News 评论区的讨论则进一步涉及复杂性理论的目的、启发式方法的必要性，以及通过限制问题域来规避困难实例等话题。

**「社区讨论」** 评论者大体认可“最坏情况在实际中很少出现”的观察，但认为文章没有充分正视理论价值与行业常态做法：例如 pron 强调复杂性类研究旨在理解计算的极限，Guvante 指出依赖管理器和类型系统通常直接阻断难例。另有评论提到即使近似求解，某些搜索问题仍可能非常困难，并援引旧版 Debian 升级中的实际体会。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=49291268">NP - Overrated | Hacker News</a></li>

</ul>
</details>

**标签**: `#algorithms`, `#complexity theory`, `#NP-hard`, `#software engineering`, `#heuristics`

---

<a id="item-tech-news-14"></a>
### [旧网页去哪儿了：65.7 万条链接的链接失效调查](https://0.mk/blog/link-rot) ⭐️ 7.0/10

一项发表在 0.mk 博客上的分析追踪了 657,607 条链接，试图回答“旧的网页去了哪里”。结果显示，链接失效呈现出明显模式，大量旧网页内容已经无法访问，为网络衰变和网页消失提供了具体的量化证据。这项数据驱动研究有助于网页开发者、档案工作者和互联网历史研究者了解内容丢失的规模与规律。

hackernews · tdx · 8月13日 17:49 · [社区讨论](https://news.ycombinator.com/item?id=49289532)

**「背景」** 链接腐烂（link rot）是指由于域名过期、服务器关闭或内容被移除，导致超链接逐渐失效的现象，通常表现为 404 错误或重定向失效。互联网档案馆（如 Wayback Machine）通过定期爬取和存档网页来缓解这一问题，但档案覆盖并不完整，且旧网页的互动功能与动态内容往往无法完整复原。理解链接腐烂有助于评估“旧网络”消失的速度与范围，以及网页存档在数字历史研究中的价值与局限。

**「影响」** 这项基于 65.7 万条链接的分析为网页开发者、档案工作者和互联网历史研究者提供了一份关于链接失效和旧网页消失规模的实证参考，可作为讨论网络保存策略时的数据基础。

**「社区讨论」** 评论者对“旧网页”的时间界定产生分歧：有人认为它结束于 Facebook 兴起和博客圈衰落，有人以谷歌搜索公开前（约 1997 年）或 2009-2014 年为界。也有评论提醒，网站历来像橱窗一样随季节更换，永久存档的想法只适用于在线新闻等少数内容。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://web.archive.org/web/20250214072411/https://en.wikipedia.org/wiki/Wikipedia:Link_rot">Wikipedia: Link rot - Wikipedia</a></li>

</ul>
</details>

**标签**: `#link-rot`, `#web-preservation`, `#internet-history`, `#data-analysis`, `#web-archiving`

---

<a id="item-tech-news-15"></a>
### [City2Graph：将地理空间数据转为异构图的 Python 库](https://www.reddit.com/r/MachineLearning/comments/1vn8oya/city2graph_a_python_library_for_heterogeneous/) ⭐️ 7.0/10

City2Graph 是一个新发布的开源 Python 库，可将地理空间数据转换为适用于空间分析、网络分析和图神经网络（GeoAI）的异构图。描述该库的论文已发表在《Computers, Environment and Urban Systems》2026 年第 130 卷，文章编号 102492，作者为 Sato、Pietrostefani、Mahabir 和 Arribas-Bel。该库支持从 OpenStreetMap 和 Overture Maps 构建城市形态图，通过 DuckDB 加载 GTFS 和 GBFS 数据以生成交通图，将 OD 矩阵和流数据表示为加权空间图，并提供 KNN、Delaunay、Gilbert、Waxman 以及女王/车相邻性等邻近和邻接图。它还能在 GeoDataFrame、NetworkX、rustworkx 和 PyTorch Geometric 的 Data/HeteroData 之间往返转换，同时保持几何与图结构一致。该库填补了 GeoAI 工具链中从原始地理数据到异构图建模之间的空白，为城市系统研究提供了可直接使用的开源方案。

reddit · r/MachineLearning · /u/Tough\_Ad\_6598 · 8月13日 11:59

**「背景」** 传统上，城市数据常被表示为扁平的特征表或同构图，难以表达建筑物、街道、交通站点和人口流动之间的多种关系类型。异构图允许在一个图中同时存在多种节点类型和边类型，并通过元路径组合跨类型关系，因此更适合建模城市系统的复杂性。City2Graph 提供了从多种地理数据源构建此类异构图的统一接口，并能直接输出到图神经网络框架，降低了该领域的研究门槛。

**「影响」** 对于从事城市计算、空间分析和 GeoAI 的研究人员，City2Graph 提供了一个经过论文描述和代码公开的现成工具，可将 OSM、Overture、GTFS 和 GBFS 等数据直接转换为 PyTorch Geometric 兼容图，从而减少重复编码工作并提高实验的可复现性。该库目前仍处于开发初期，功能覆盖范围和性能尚需社区验证与扩展。

**标签**: `#graph-neural-networks`, `#geospatial`, `#python`, `#urban-systems`, `#geoai`

---

<a id="item-tech-news-16"></a>
### [AI 人体组织实验室年测 300 万样本](https://www.fastcompany.com/91589344/the-worlds-largest-biological-datacenter-could-help-make-animal-testing-obsolete) ⭐️ 7.0/10

据 Fast Company 报道，Vivodyne 在旧金山南部运营衣柜大小的机器人实验室，利用 AI 设计实验，每年可对 300 多万个人体组织进行受控试验，容量约为美国全部临床试验总和的两倍，旨在更好地预测新药疗效与安全性，并有望减少或替代动物测试。报道指出，目前约 90%的临床试验在通过动物测试后仍告失败。这些数据主要来自公司自身宣传，尚不能视为已验证的突破。

telegram · zaihuapd · 8月14日 01:48

**「背景」** 传统药物研发通常先进行动物测试，但约 90%通过动物测试的候选药物在后续人体临床试验中仍以失败告终，因为动物生理与人体存在明显差异。Vivodyne 是一家利用机器人实验室培养人体组织并结合 AI 设计实验的生物科技公司，其公开资料称这些实验室培养的组织与活体人体组织难以区分，并可通过自动化流程生成影像、单细胞转录组和蛋白质组等多组学数据。该公司在 2025 年 6 月宣布获得 4000 万美元融资，据称每次机器人运行可独立完成超过 1 万项人体组织实验，以支撑更大规模的药物测试。

**「影响」** 如果该系统经独立验证有效，制药和生物技术公司可能以更高通量和更低成本筛选候选药物，降低对动物实验的依赖；但当前缺乏第三方验证，实际替代进程仍存在不确定性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.vivodyne.com/">Vivodyne | Make biology computable</a></li>
<li><a href="https://hlth.com/insights/news/vivodyne-raises-40m-to-transform-drug-development-with-ai-powered-human-tissue-testing-2025-06-03">Vivodyne Raises $40M to Transform Drug Development with...</a></li>
<li><a href="https://www.bastillepost.com/global/article/6076655-vivodyne-launches-the-worlds-largest-human-biological-datacenter-to-train-the-first-world-model-of-human-biology">Vivodyne Launches the World’s Largest Human Biological Datacenter...</a></li>

</ul>
</details>

**标签**: `#AI`, `#biotech`, `#robotics`, `#drug discovery`, `#lab automation`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [阿克曼旗下 Pershing Square 重新建仓 Netflix](https://www.cnbc.com/2026/08/13/ackman-buys-netflix-again-four-years-later-says-it-won-streaming-wars.html) ⭐️ 8.0/10

比尔·阿克曼旗下 Pershing Square 在半年报中披露重新建仓 Netflix，认为该公司已“有效赢得流媒体战争”。Pershing Square 称，Netflix 拥有逾 3.25 亿订阅用户，股价已从 2025 年 6 月高点 134 美元回落约 50%，远期市盈率从 40 多倍降至约 21 倍。

rss · CNBC Finance · 8月13日 18:04

**「背景」** 阿克曼曾在 2022 年初买入 Netflix，但在该公司报告十多年来首次订阅用户下滑后约三个月内清仓。

**标签**: `#Netflix`, `#Bill Ackman`, `#Pershing Square`, `#Streaming`, `#Valuation`

---

<a id="item-finance-news-2"></a>
### [长鑫存储市值超越腾讯，成为中国市值最高公司](https://www.bloomberg.com/news/articles/2026-08-13/cxmt-overtakes-tencent-to-become-most-valuable-chinese-company) ⭐️ 8.0/10

长鑫存储（CXMT）市值已超越腾讯，成为中国市值最高的公司：周四跌 1.2%后市值仍有 5240 亿美元，腾讯估值则为 5100 亿美元。CXMT 上月在上海上市，首日暴涨 467%；腾讯因加大 AI 投入，今年以来股价累计下跌超 26%。

telegram · zaihuapd · 8月13日 10:10

**「背景」** 长鑫存储（CXMT）是总部位于安徽合肥的半导体存储器（DRAM）制造商，上月在上海上市后股价大涨。腾讯则因加大 AI 投入而股价承压，导致市值排名发生变化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ChangXin_Memory_Technologies">ChangXin Memory Technologies - Wikipedia</a></li>

</ul>
</details>

**标签**: `#CXMT`, `#Tencent`, `#China market cap`, `#semiconductor`, `#IPO`

---

<a id="item-finance-news-3"></a>
### [Uber 与 Pony.ai 计划在欧洲部署 2000 辆无人驾驶出租车](https://www.cnbc.com/2026/08/14/uber-partners-with-chinas-ponyai-for-2000-robotaxis-in-europe.html) ⭐️ 7.0/10

优步（Uber）与中国自动驾驶公司小马智行（Pony.ai）于周五宣布，计划在欧洲部署 2000 辆无人驾驶出租车（robotaxi），并将双方合作扩展至中东。公司未公布具体城市或明确时间表。

rss · CNBC Finance · 8月14日 01:02

**「背景」** 今年 3 月底，双方已在克罗地亚首都萨格勒布推出商业无人驾驶出租车服务，据称是欧洲首例。

**标签**: `#Uber`, `#Pony.ai`, `#Robotaxi`, `#Autonomous Vehicles`, `#Europe`

---

<a id="item-finance-news-4"></a>
### [标普 500 企业 Q2 净利润率有望创 FactSet 有记录以来新高](https://www.cnbc.com/2026/08/13/these-charts-show-why-stocks-keep-rallying-profit-margins-are-highest-on-record.html) ⭐️ 7.0/10

据 FactSet 数据，标普 500 指数成分股公司第二季度混合净利润率为 16.9%，高于一季度的 14.8%和去年同期的 12.9%，也高于五年均值 12.4%；若该数据成立，将是 FactSet 自 2009 年开始追踪该指标以来的最高水平。

rss · CNBC Finance · 8月13日 20:21

**「背景」** 净利润率是指企业扣除所有费用后保留的营收占比。FactSet 数据显示，除 Alphabet 和亚马逊外，标普 500 的净利润率仍达 15%，同为纪录高位；11 个行业中有 8 个的利润率高于去年同期。

**标签**: `#S&amp;P 500`, `#profit margins`, `#corporate earnings`, `#FactSet data`, `#stock market`

---

<a id="item-finance-news-5"></a>
### [美国宣布无人机关税：部分进口机型税率达 100%](https://www.whitehouse.gov/presidential-actions/2026/08/adjusting-imports-of-unmanned-aircraft-systems-and-unmanned-aircraft-systems-components-into-the-united-states/) ⭐️ 7.0/10

美国总统 8 月 13 日签署公告，对进口无人机及部件加征新关税。自 2026 年 9 月 3 日起，最大起飞重量超过 25 公斤的无人机、搭载热成像仪的无人机、无人机基站及部分关键部件税率达 100%，25 公斤及以下无人机税率为 25%；公告还称，另一部分无人机部件的 25%关税将于 2027 年 2 月 9 日起生效，并授权商务部长将更多部件纳入征税范围。

telegram · zaihuapd · 8月14日 01:24

**「背景」** 白宫称此举旨在扩大美国国内无人机制造并减少对关键零部件海外来源的依赖，相关措施也被视为针对中国等外国供应商。

**「影响」** 新关税将直接影响依赖进口无人机的美国经销商、商业用户和消费者，可能导致相关机型与部件价格上升；美国市场对中国产无人机的依赖程度较高，供应链成本或进一步承压。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.aa.com.tr/en/world/trump-imposes-tariffs-of-up-to-100-on-imported-drones-components/4027001">Trump imposes tariffs of up to 100 % on imported drones , components</a></li>
<li><a href="https://www.bloomberg.com/news/articles/2026-08-13/trump-imposes-100-tariffs-on-certain-drones-countering-china">Trump Imposes 100 % Tariffs on Some Drones ... - Bloomberg</a></li>
<li><a href="https://www.datamintelligence.com/news/trump-drone-tariffs-2026-impact-on-global-drone-market-us-china-uav-supply-chain">Trump Drone Tariffs 2026: 100% Duty on Chinese UAV Imports ...</a></li>
<li><a href="https://www.whitehouse.gov/fact-sheets/2026/08/fact-sheet-president-donald-j-trump-bolsters-national-security-and-strengthens-u-s-supply-chains-by-imposing-tariffs-on-drones-and-their-parts-and-components/">Fact Sheet: President Donald J. Trump Bolsters National Security and...</a></li>
<li><a href="https://www.dslrpros.com/blogs/drone-trends/the-impact-of-tariffs-and-geopolitical-challenges-on-the-drone-industry">The Impact of Tariffs and Geopolitical Challenges on the Drone ...</a></li>

</ul>
</details>

**标签**: `#tariffs`, `#drones`, `#trade policy`, `#United States`, `#import duties`

---

<a id="item-finance-news-6"></a>
### [苹果提议美国 App Store 外部购买抽成最高 15%](https://9to5mac.com/2026/08/13/apple-proposes-commissions-of-up-to-15-for-off-app-store-purchases-in-the-us/) ⭐️ 7.0/10

苹果已向法院提交美国 App Store 外部购买抽成方案：标准应用抽成 15%，视频、新闻等合作项目及订阅续费抽成 10%，小型企业计划应用抽成 5%。该方案尚待法院审理，目前只是提案而不是最终政策。

telegram · zaihuapd · 8月14日 02:33

**「背景」** 这是 Epic 诉苹果案的一部分；美国最高法院此前拒绝了苹果暂停下级法院审理费率问题的请求。Epic 将有机会回应，苹果预计于 9 月 14 日前向最高法院提交书面意见。

**标签**: `#Apple`, `#App Store`, `#regulation`, `#Epic Games`, `#commissions`

---