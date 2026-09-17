---
layout: default
title: "Horizon Summary: 2026-09-17 (ZH)"
date: 2026-09-17
lang: zh
---

> 从 42 条内容中筛选出 15 条重要资讯。

---

**科技新闻**
1. [英伟达宣布支持在 Rust 中编写原生 GPU 内核](#item-tech-news-1) ⭐️ 8.0/10
2. [美光展示全球首款 512GB DDR5 服务器模组，2027 年具备量产条件](#item-tech-news-2) ⭐️ 8.0/10
3. [训练 4B 模型生成比 Postgres 快 81%的查询计划](#item-tech-news-3) ⭐️ 7.0/10
4. [小米 MiMo 2.6 实时后训练仪表盘引关注](#item-tech-news-4) ⭐️ 7.0/10
5. [Mistral 与 Mozilla 合作推出私密多语言 AI 浏览](#item-tech-news-5) ⭐️ 7.0/10
6. [黑客入侵 Flock 摄像头 暴露硬编码凭证与安全缺陷](#item-tech-news-6) ⭐️ 7.0/10
7. [Anthropic 将 Claude Cowork 与聊天合并为统一 Claude](#item-tech-news-7) ⭐️ 7.0/10
8. [TMLR 联系 10 篇拟直接拒稿论文作者，多数难以解释论文](#item-tech-news-8) ⭐️ 7.0/10
9. [GoBench：以 9x9 围棋评测大模型推理能力](#item-tech-news-9) ⭐️ 7.0/10
10. [Cloudflare 推出可保留搜索收录并禁止 AI 训练的域名设置](#item-tech-news-10) ⭐️ 7.0/10
11. [约 170 万中文赌场网站被 APT 用作恶意软件 C2 基础设施](#item-tech-news-11) ⭐️ 7.0/10
12. [新浪云 SAE 将永久下线 早期 B 站视频源文件启动归档](#item-tech-news-12) ⭐️ 7.0/10

**财经新闻**
1. [美联储加息 25 个基点至 3.75%-4%，为三年多来首次](#item-finance-news-1) ⭐️ 9.0/10
2. [香港推出 11 项鼓励生育措施](#item-finance-news-2) ⭐️ 7.0/10
3. [平陆运河建成通航 西南货物经北部湾直通东盟](#item-finance-news-3) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [英伟达宣布支持在 Rust 中编写原生 GPU 内核](https://developer.nvidia.com/blog/introducing-cuda-rust-two-tracks-for-writing-gpu-kernels/) ⭐️ 8.0/10

英伟达在其官方开发者博客发文介绍 CUDA Rust，宣布开发者可以用 Rust 原生编写 GPU 内核，并给出两条编写内核的技术路线。这使 Rust 首次进入英伟达官方 CUDA 工具链的叙事范围，被视为对 Rust 与 CUDA 生态结合具有意义的一步。由于本条目未提供原文内容，两条路线各自的具体形态、支持的编译器与硬件版本、性能数据及限制条件均未得到确认，目前只能视为工具链能力的增量扩展。

hackernews · nonmaskable · 9月16日 11:15 · [社区讨论](https://news.ycombinator.com/item?id=49724881)

**「背景」** CUDA 是 NVIDIA 的 GPU 并行计算平台，传统上核函数需要编译到 PTX 才能由 GPU 执行；CUDA Rust 的目标是让开发者直接用 Rust 编写 GPU 核函数并原生编译到 PTX，而不是在 Rust 中包装其他语言实现的核函数。它沿袭 CUDA 原有的两条编写路径，并对应提供 SIMT 与 Tile 两种轨道。具体由 NVlabs 的两个开源项目实现：cuda-oxide 面向 SIMT 模型，cutile-rs 面向较新的 Tile 模型，二者都用 Rust 的所有权规则在编译期拒绝别名（aliasing）错误。

**「影响」** 对在英伟达平台上工作的 Rust 与 AI 基础设施开发者而言，这意味着除了 CUDA C++ 之外多了一条官方支持的内核编写途径，但实际价值取决于工具链成熟度与硬件覆盖范围。

**「社区讨论」** 评论区意见分化：有人期待 Rust 的安全性改善内核编程，并认为它可与 Hugging Face 的 Candle 推理库衔接；也有评论者强烈批评 CUDA 造成的厂商锁定，主张像 Metal、OpenCL、D3D12 那样把内核写在独立文件中手动启动，或直接使用 Triton 等 DSL。另有评论质疑该公告文章由大模型代写、内容质量存疑。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.nvidia.com/blog/introducing-cuda-rust-two-tracks-for-writing-gpu-kernels/">Introducing CUDA Rust : Two Tracks for Writing GPU Kernels</a></li>
<li><a href="https://blockchain.news/news/nvidia-cuda-rust-gpu-kernels">NVIDIA Launches CUDA Rust for GPU Kernels... - Blockchain.News</a></li>
<li><a href="https://www.marktechpost.com/2026/09/08/nvidia-announces-cuda-rust-with-cuda-oxide-simt-and-cutile-rs-tile-for-compile-time-safe-gpu-kernels/">NVIDIA Announces CUDA Rust with cuda -oxide... - MarkTechPost</a></li>

</ul>
</details>

**标签**: `#Rust`, `#CUDA`, `#GPU programming`, `#Nvidia`, `#systems programming`

---

<a id="item-tech-news-2"></a>
### [美光展示全球首款 512GB DDR5 服务器模组，2027 年具备量产条件](https://videocardz.com/newz/micron-says-worlds-first-512gb-ddr5-module-will-be-production-ready-for-2027) ⭐️ 8.0/10

美光宣布展示全球首款 512 GB DDR5 RDIMM，面向服务器，速率最高 9200 MT/s。该模组采用 3D 堆叠 DRAM 芯片，24 根可组成 12 TB 内存容量。功耗方面，美光称单根功耗为 16W，低于 4 根 128 GB 模组的 44.2W，降幅超过 60%。AMD 和 Intel 正为未来服务器平台对其进行验证，美光预计 2027 年具备量产条件。该产品目前仍处于展示与验证阶段，并非已落地产品。

telegram · zaihuapd · 9月16日 16:15

**「背景」** DDR5 RDIMM 是带有寄存缓冲（Registered）的服务器内存模组，靠模组上的寄存器减轻内存控制器的电气负载，从而支持更大的单模组容量，是数据中心与 AI 服务器的常见内存形态。美光的 512 GB 模组采用先进封装，将多颗 DRAM 裸片垂直堆叠并以硅通孔（TSV）互连，从而在标准模组形态下容纳远超常规的容量。随着 AI 服务器对内存容量与能效的要求提高，单根容量和每瓦性能成为平台设计的关键约束，因此 AMD 与 Intel 正为未来服务器平台验证该模组。

**「影响」** 若按计划在 2027 年具备量产条件，该模组可在相同插槽数量下提供更高服务器内存容量与能效，对 AI 等内存密集型负载有实际意义；但其仍处展示与验证阶段，实际量产时间与平台支持仍存在不确定性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tomshardware.com/pc-components/dram/micron-announces-512gb-ddr5-9200-memory-modules-with-16w-power-draw-up-to-12tb-per-server-claims-60-percent-less-energy-intensive-than-four-128gb-modules">Micron announces 512 GB DDR 5 -9200 memory ... | Tom&#x27;s Hardware</a></li>
<li><a href="https://www.guru3d.com/story/micron-builds-worlds-first-512gb-ddr5-rdimm-with-9200mt-s-transfer-rate/">Micron Builds Worlds First 512 GB DDR 5 RDIMM With...</a></li>
<li><a href="https://investors.micron.com/news/press-release/2026/Micron-Advances-Memory-Innovation-With-the-Worlds-First-Ultra-Dense-Module-for-Next-Generation-Servers/default.aspx">Micron Technology, Inc. - Micron Advances Memory Innovation With...</a></li>

</ul>
</details>

**标签**: `#DDR5`, `#服务器内存`, `#美光`, `#3D堆叠DRAM`, `#硬件`

---

<a id="item-tech-news-3"></a>
### [训练 4B 模型生成比 Postgres 快 81%的查询计划](https://rohanbansal.com/qorl) ⭐️ 7.0/10

Hacker News 上讨论的一篇博文（rohanbansal.com/qorl）描述了训练一个 4B 参数模型来生成查询计划，并声称在该基准上比 Postgres 快 81%。这一结论建立在较窄的测试条件上：数据集约 8 GB 且完全驻留内存，shared\_buffers 被限制为远小于数据集的一个比例，查询在测量前已预热，且只涉及只读 SELECT。评论者进一步指出，除主键外各表没有其他索引，也没有额外统计信息，并且存在相关列，因此该数字可能反映的是特定基准条件，而非普遍优势。评论区还质疑这类规划器的可靠性，例如模型可能偶发漏用索引，但现有证据并未对这一点给出结论。

hackernews · polyphilz · 9月16日 18:50 · [社区讨论](https://news.ycombinator.com/item?id=49731285)

**「背景」** 数据库的查询规划器负责把 SQL 语句转换为执行计划，PostgreSQL 传统上依据表统计信息做代价估算，在多个候选计划中挑选它认为代价最低的一个，因此统计信息是否准确、代价模型是否贴合实际工作负载会直接决定查询性能。当统计信息不准确时，工程师常用提示（hints）强制指定计划，但社区经验认为这往往只是掩盖统计问题，并可能在数据分布变化后反噬。本次项目的背景正是这一环节：作者用强化学习训练一个 4B 参数模型来生成查询计划，在每次更新中为所有到达训练器的 rollout 分配锚定信用，并声称其生成的计划优于 PostgreSQL 的默认计划。

**「影响」** 对于考虑以学习型查询规划器替代 Postgres 启发式规划器的数据库工程师而言，上述基准条件意味着 81% 的加速不能直接外推到更大规模或更接近真实 OLTP 的生产负载。相关可靠性问题（如偶发漏用索引）尚未得到验证。

**「社区讨论」** 评论者普遍认可该项目在技术上值得关注，但对结论的泛化能力持保留态度，反复强调内存驻留数据集、预热查询、缺少二级索引与额外统计信息、相关列等因素会显著影响结果，其中一位评论者指出多数使用查询提示的场景其实源于统计信息不准确。也有评论者担心 LLM 规划器偶发漏用索引会造成生产故障，并认为查询计划优化更适合数学与算法方法或 AlphaGo 式的神经网络启发式，而非把 LLM 当作钝器使用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://rohanbansal.com/qorl">Training a 4 B model to produce 81 % faster query ... - Rohan Bansal</a></li>
<li><a href="https://news.ycombinator.com/item?id=49731285">Training a 4 B model to produce 81 % faster query plans than ...</a></li>

</ul>
</details>

**标签**: `#LLM`, `#query optimization`, `#databases`, `#machine learning`, `#benchmarking`

---

<a id="item-tech-news-4"></a>
### [小米 MiMo 2.6 实时后训练仪表盘引关注](https://mimo.xiaomi.com/rl/) ⭐️ 7.0/10

小米为 MiMo 2.6 提供了实时后训练仪表盘，地址为 mimo.xiaomi.com/rl/，用于观察模型的强化学习与后训练过程。该仪表盘在 Hacker News 上引发关注，因为这种对模型 RL 训练过程的实时透明度并不常见。相关讨论还包含评论者的使用体验和未经核实的基准比较，但现有信息未提供更多技术细节。仪表盘具体展示哪些指标、数据刷新频率以及 MiMo 2.6 的发布时间和参数规模，目前仍不明确。

hackernews · krackers · 9月16日 20:09 · [社区讨论](https://news.ycombinator.com/item?id=49732270)

**「背景」** 小米的 MiMo 是一条自有大模型产品线，此前已发布 MiMo-V2.5、MiMo-V2.5-Pro 以及面向智能体任务的 MiMo-V2-Pro 等版本。后训练（post-training）与强化学习（RL）是在预训练之后借助任务反馈继续调整模型行为的过程；这次引发关注的页面正是把 mimo-v2.6-pro 与 mimo-v2.6-flash 的 RL 训练指标从训练器日志实时公开出来。小米在 MiMo-V2-Pro 上曾强调通过更广范围智能体任务的后训练扩展，使模型从回答问题转向完成任务。

**「影响」** 对关注 MiMo 的开发者而言，该看板把 mimo-v2.6-pro 与 mimo-v2.6-flash 的强化学习训练指标实时公开，使其能在模型发布前直接观察训练进展。不过看板本身只呈现训练日志指标，并不构成性能结论，社区中关于旧版 MiMo 基准得分的对比说法仍未经证实。

**「社区讨论」** 评论者分享了实际体验：有人称长期用 MiMo-V2.5 做软件工程，认为 ROI 很高、成本极低、质量接近其此前使用的 Anthropic 模型，但偶尔会遇到幻觉循环；另一人把 2.5-Pro 比作“健忘的新项目高级工程师”，认为可靠但多任务能力一般，并对试用中的下一版模型评价积极。讨论也出现分歧：有人担忧开源 AI 的竞争与安全影响，有人贴出 MiMo-V2.5-Pro 在 DeepSWE 1.1 上 19% 的分数并与 Fable、Kimi K3、Astra 比较，这些基准数字未在来源中得到独立核实。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mimo.xiaomi.com/rl/">mimo-v2.6 RL</a></li>
<li><a href="https://news.ycombinator.com/item?id=49732270">Xiaomi Mimo 2.6 live post-training dashboard | Hacker News</a></li>
<li><a href="https://mimo.xiaomi.com/mimo-v2-pro">MiMo-V2-Pro | Xiaomi</a></li>
<li><a href="https://mimo.xiaomi.com/rl/">mimo -v 2 . 6 RL</a></li>

</ul>
</details>

**标签**: `#AI models`, `#post-training`, `#open-source AI`, `#Xiaomi MiMo`, `#RL training`

---

<a id="item-tech-news-5"></a>
### [Mistral 与 Mozilla 合作推出私密多语言 AI 浏览](https://mistral.ai/news/mistral-x-mozilla/) ⭐️ 7.0/10

Mistral 与 Mozilla 宣布了一项私密、多语言的 AI 浏览合作，消息在 Hacker News 上引发讨论（532 分、186 条评论）。该合作的核心争议在于本地推理与云端推理的选择，以及用户是否被明确告知并同意将浏览数据上传云端。评论指出宣传页未清楚区分本地与云端推理，也没有充分说明需要用户同意启用云端方案。支持者认为多语言和隐私特性可用于检索非英语开发者文档。由于未提供完整原文，具体功能范围、部署方式和数据流细节尚不明确。

hackernews · vertigoruntime · 9月16日 08:08 · [社区讨论](https://news.ycombinator.com/item?id=49723408)

**「背景」** Firefox 的「Smart Window」是 Mozilla 推出的浏览器 AI 助手，目前处于 beta 阶段，可帮助用户跨标签页搜索、整理信息，并找回此前访问过的页面。此次它改由法国 AI 公司 Mistral 的模型驱动，双方将合作定位为把「开放、私密且多语言」的 AI 带入用户日常浏览场景，强调隐私、控制与选择。浏览器内置 AI 助手近来成为趋势，而模型推理究竟在本地还是云端运行、用户数据是否上传，正是这类功能最受关注的分歧点。

**「影响」** 对 Firefox 用户和多语言开发者而言，这一合作意味着将出现一个由 Mistral 支持、以隐私和选择为卖点的 AI 浏览方案，被视为 Chrome 内置 Gemini Nano 之外的替代路径；但其实际隐私影响取决于本地与云端推理的区分及用户同意机制是否明确，社区对此已有质疑。

**「社区讨论」** 有评论者批评 Mozilla 在适合完全本地小模型推理的场景下，却试图将上传私人浏览历史到云端正常化，并认为营销页面至少应清楚说明本地与云端推理的差异及同意机制。其他人则看好隐私与多语言组合对非英语开发文档检索的价值，也有人将这项合作与 Chrome 内置 Gemini Nano 类比，并指出 Firefox 及其合作方能否兑现隐私承诺、避免漏洞，对终端用户而言仍难以验证；还有评论提出可在浏览器内内置小模型，把长查询改写成高级搜索查询。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mistral.ai/news/mistral-x-mozilla/">Mistral x Mozilla : Private , Multilingual AI Browsing</a></li>
<li><a href="https://digg.com/tech/a90064fc-f0ba-40a2-97f1-ac972efc5192">Mozilla taps Mistral to power Firefox Smart Window · Digg</a></li>
<li><a href="https://upstract.com/x/a1d4820c4e4f178e">Mistral X Mozilla : Private , Multilingual AI Browsing</a></li>
<li><a href="https://mistral.ai/news/mistral-x-mozilla/">Mistral x Mozilla: Private, Multilingual AI Browsing</a></li>
<li><a href="https://blog.mozilla.org/en/firefox/mozilla-mistral-partnership/">Mozilla and Mistral partner to expand AI competition, user choice | The Mozilla Blog</a></li>
<li><a href="https://news.ycombinator.com/item?id=49723408">Mistral X Mozilla: Private, Multilingual AI Browsing | Hacker News</a></li>

</ul>
</details>

**标签**: `#AI browsers`, `#privacy`, `#local inference`, `#Mozilla Firefox`, `#Mistral AI`

---

<a id="item-tech-news-6"></a>
### [黑客入侵 Flock 摄像头 暴露硬编码凭证与安全缺陷](https://www.wired.com/story/hackers-flock-camera-data-shows-how-system-works/) ⭐️ 7.0/10

据 Wired 报道及社区讨论，黑客据称进入了 Flock 的一台监控摄像头，并由此暴露出硬编码凭证以及该系统更广泛的安全弱点。评论者指出，此次发现的不是硬编码管理员密码，而是可用于请求凭证的 API 密钥；这些凭证以明文存储，看起来可能让持有者访问 Flock 服务器，不过目前尚不清楚成功以摄像头身份认证后具体能做什么。多名评论者还批评 Flock 的漏洞披露政策，认为它更像是在宣称拥有 VDP 并营造负责任的安全姿态，而非真正鼓励研究人员报告问题，其中包含要求不“交互”设备或服务、不下载数据等限制。另有评论者认为，问题根源在于为缩短上市时间而忽视安全启动、密钥管理和物理访问威胁模型；driverdan 表示该报道与 404 Media 合作完成，Distributed Denial of Secrets 已发布分区镜像。还有评论称，相关数据可能被任何未经授权者直接取走，且未得到适当加密；这些说法来自社区讨论，细节和影响仍待更多验证。

hackernews · driverdan · 9月16日 13:18 · [社区讨论](https://news.ycombinator.com/item?id=49726586)

**「背景」** Flock Safety 是美国最大的自动车牌识别（ALPR）摄像头供应商之一，其设备被安装在警察部门、企业和业主协会等场所，用于记录车辆通行情况。由于这些摄像头部署在公共空间，攻击者可以物理接触设备本身，固件安全与密钥管理因此成为威胁模型的核心；安全研究者 Micah Lee 的调查指出，该相机固件中嵌入了硬编码 API 密钥，可依据 MAC 地址为任意同型号摄像头换取凭据（返回内容包含 Auth0 客户端 ID 与密钥）。这一背景有助于理解为何硬编码凭据与漏洞披露流程会成为此次报道及社区讨论的焦点。

**「影响」** 对部署 Flock ALPR 摄像头的美国城市与执法机构而言，硬编码的 API 密钥及明文存储的凭据意味着攻击者只要获得设备的物理访问权，就可能提取数据并尝试访问 Flock 后端服务器；不过目前尚不清楚成功以摄像头身份完成认证后究竟能取得哪些权限。

**「社区讨论」** 评论区的共识是，硬编码凭证和薄弱的漏洞披露流程反映出 Flock 在安全工程上的系统性不足；分歧主要在于实际危害范围，因为可用于请求凭证的 API 密钥是否真能访问服务器、以及认证后能做什么仍未明确。也有人强调，设备部署在公共空间意味着必须把本地物理访问纳入威胁模型，而现有实现在这方面明显不足。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://micahflee.com/flock-cameras-are-riddled-with-security-vulnerabilities-and-hard-coded-credentials/">Flock cameras are riddled with security vulnerabilities and...</a></li>
<li><a href="https://deflock.org/">Find Nearby ALPRs | DeFlock</a></li>
<li><a href="https://clashreport.com/world/articles/hackers-expose-how-flock-mass-surveillance-works-05q58b65rsj">Hackers Expose How Flock Mass Surveillance Works · Clash Report</a></li>

</ul>
</details>

**标签**: `#security`, `#IoT`, `#surveillance`, `#embedded systems`, `#vulnerability disclosure`

---

<a id="item-tech-news-7"></a>
### [Anthropic 将 Claude Cowork 与聊天合并为统一 Claude](https://simonwillison.net/2026/Sep/16/one-claude/) ⭐️ 7.0/10

Anthropic 宣布将 Claude Cowork 与聊天合并为一个统一的 Claude：用户既可以提出简短问题，也可以把任务（例如中午前要交的报告）交给它处理，即使关闭笔记本电脑后它仍会继续执行。该功能首先面向 Pro 和 Max 订阅方案推出，并将在未来几周内逐步覆盖网页版、桌面端和移动端的 Claude 应用，适用于这些方案的新老用户。Simon Willison 认为，这意味着 Claude 正在成为一个独立的通用智能体（general agent），与 OpenAI 几周前把 Codex 桌面应用更名为 ChatGPT 的做法相呼应。他还表示，这次合并省去了他原本计划梳理 Cowork 与普通 Claude 边界的后续写作，但他预计要弄清这次合并在实际功能与界面层面的具体含义仍需不少工作。

rss · Simon Willison · 9月16日 18:09

**「背景」** 在本次调整之前，Anthropic 的 Claude 产品线分为三种形态：普通聊天、面向任务的 Claude Cowork 以及开发者用的 Claude Code，功能边界重叠让不少用户（包括长期跟踪该产品的评论者）难以分辨各自定位。Claude Cowork 属于让 Claude 承接完整任务、即使在用户关闭设备后仍继续执行的一类代理式工作界面，与日常问答式聊天并行存在。随着两者合并，Claude 的模式从三种缩减为 Claude Chat 与 Claude Code 两种，同一时间 Anthropic 还推出了 Claude Docs 与 Claude Slides，并让 Claude Design 直接在对话中工作。

**「影响」** 对 Pro 和 Max 用户来说，他们不再需要区分 Cowork 与普通聊天的入口，可在同一个 Claude 应用中跨网页、桌面和移动端延续任务执行；不过合并后的具体功能边界仍待观察。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://claude.com/blog/cowork-is-now-claude">Claude Cowork and chat are now one Claude | Claude by Anthropic</a></li>
<li><a href="https://9to5mac.com/2026/09/16/anthropic-merging-claude-cowork-with-chat/">Anthropic merging Claude Cowork with chat - 9to5Mac</a></li>
<li><a href="https://www.zdnet.com/innovation/claude-chat-absorbs-cowork-anthropic/">Anthropic merges Claude chat and Cowork into one - ZDNET</a></li>

</ul>
</details>

**标签**: `#AI agents`, `#Anthropic`, `#Claude`, `#product strategy`, `#AI assistants`

---

<a id="item-tech-news-8"></a>
### [TMLR 联系 10 篇拟直接拒稿论文作者，多数难以解释论文](https://www.reddit.com/r/MachineLearning/comments/1wid67h/tmlr_reached_out_to_the_authors_of_10_papers/) ⭐️ 7.0/10

TMLR 联系了 10 篇原拟被直接拒稿（desk rejection）的论文作者，要求他们解释自己提交的论文；相关结果来自 TMLR 在 Medium 上发布的文章，并由 Reddit r/MachineLearning 用户转发讨论。10 篇论文中有 1 篇的作者撤稿，1 篇的作者称因其他事务无法参加，1 篇的作者安排了会议但未出席，3 篇的作者无法回答关于论文的基本问题，3 篇的作者能回答高层思路但在进一步技术细节上遇到困难。只有 1 篇的作者回答了全部问题，不过参与访谈的 TMLR 联合主编仍指出该论文存在一个重大缺陷。该事件凸显了机器学习出版中围绕作者身份、论文真实性和可能由 LLM 生成或论文工厂产出的稿件的担忧。

reddit · r/MachineLearning · /u/hihey54 · 9月16日 23:20

**「背景」** TMLR（Transactions on Machine Learning Research）是一份采用滚动投稿、并在 OpenReview 上进行公开评审的机器学习期刊，编辑部会先对来稿做初步把关，把不符合基本要求的论文直接退稿（desk rejection），使其不进入完整同行评审。公开统计显示，在把撤稿与直接退稿一并计入时，该刊 2025 年已评审投稿的接收率约为 46.3%，不计入则为 70.6%；该刊还引入了作者投稿配额制度。这些筛选与限流机制，与近年学术界对代写、论文工厂以及疑似大模型生成投稿的担忧交织在一起，构成了编辑部主动联系作者核实其论文内容这一做法的背景。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/@TmlrOrg/annual-author-submission-quotas-for-tmlr-1db785e51548">Annual Author Submission Quotas for TMLR | by Transactions on Machine Learning Research | Medium</a></li>
<li><a href="https://phdflow.ai/guides/tmlr-explained">TMLR explained: a differently shaped bar, not a lower one</a></li>
<li><a href="https://openreview.net/group?id=TMLR">TMLR | OpenReview</a></li>

</ul>
</details>

**标签**: `#machine learning`, `#peer review`, `#academic integrity`, `#TMLR`, `#LLM-generated papers`

---

<a id="item-tech-news-9"></a>
### [GoBench：以 9x9 围棋评测大模型推理能力](https://www.reddit.com/r/MachineLearning/comments/1wi68jg/gobench_evaluating_llms_on_the_game_of_go_r/) ⭐️ 7.0/10

研究者发布了 GoBench，一个面向大语言模型的开源基准与排行榜，通过 9x9 围棋对局评估模型的通用推理能力。评测让模型与从随机水平到超人水平的 KataGo 对手天梯对弈，并报告其成绩与 ARC-AGI 2 的相关系数达到 r=0.83，且该基准目前远未饱和。作者称 GPT-6 Astra 的最高成绩为 2500 Elo，远低于最强 KataGo 的 4400 Elo；若允许使用编码工具并给予两小时准备时间，Codex 搭配 Astra 可达到 3560 Elo。项目提供了排行榜、GitHub 代码与论文链接，作者表示只要基准未饱和就会持续更新排行榜。这些结果由作者自行发布，尚未经过独立验证。

reddit · r/MachineLearning · /u/Roland31415 · 9月16日 18:54

**「背景」** 围棋长期被用作衡量 AI 推理能力的棋盘游戏，而 KataGo 是一个开源、经自我对弈训练、结合深度神经网络与搜索算法达到超人水平的围棋引擎。ARC-AGI 由 François Chollet 于 2019 年提出，旨在用抽象与推理任务衡量流体智力，已成为评估 LLM 推理泛化能力的常用基准之一。等级分（Elo）则用于把棋力或模型表现换算为可比较的强弱数值，这也是 GoBench 借助 KataGo 对手阶梯来定位 LLM 棋力的背景。

**「影响」** 对需要评估大模型推理能力的研究者而言，GoBench 提供了一个尚未饱和、并以与 ARC-AGI 2 的相关性作为佐证的新选择，但其分数为作者自报且未经独立验证，采纳时需谨慎对待。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arcprize.org/arc-agi">ARC Prize - The only AI benchmark that measures AGI progress.</a></li>
<li><a href="https://www.stork.ai/en/katago">KataGo Review (2026): Pricing &amp; Alternatives | Stork. AI</a></li>

</ul>
</details>

**标签**: `#LLM evaluation`, `#Go`, `#reasoning benchmarks`, `#KataGo`, `#AI research`

---

<a id="item-tech-news-10"></a>
### [Cloudflare 推出可保留搜索收录并禁止 AI 训练的域名设置](https://blog.cloudflare.com/accountable-mixed-use-ai-crawlers/) ⭐️ 7.0/10

Cloudflare 于 9 月 15 日宣布推出“禁止 AI 训练”设置，允许网站继续被搜索引擎收录，同时阻止不符合其要求的 AI 训练爬虫。苹果、谷歌和微软已符合或承诺符合相关要求。该设置按域名配置；如果网站选择“阻止”，包括混合爬虫在内的所有爬虫都会被拦截，搜索收录也会因此受影响。Cloudflare 还计划在明年初让网站控制内容被 AI 摘要引用的比例。

telegram · zaihuapd · 9月16日 05:46

**「背景」** Cloudflare 的新设置名为“Disallow AI Training”，它针对的是同时承担搜索索引与 AI 训练的混合爬虫：网站若直接拦截所有非合规爬虫，可能连带失去搜索引擎收录。为解决这一矛盾，Cloudflare 对爬虫引入“Accountable”（可问责）标记，允许苹果、谷歌、微软等已符合或承诺符合要求的爬虫继续抓取，其余 AI 训练爬虫仍被拦截。此前在 Training 中选择“Block”或“Block on pages with ads”的站点会自动迁移到该设置，且谷歌、苹果、微软还分别计划推出 URL 层级的透明度工具。

**「影响」** 网站运营者现在可以按域名选择只拦截 AI 训练爬虫、同时保留搜索引擎收录，但选择“阻止”后混合爬虫也会被一并拦下，搜索收录与相关流量随之受影响。Cloudflare 说明 AI 公司可声明其爬虫用于训练、推理还是搜索，网站据此决定放行对象，落地效果取决于各爬虫方是否如实声明用途。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bannedbook.org/bnews/itnews/20260916/2360152.html">Cloudflare 推出设置：可保留搜索收录并禁止 AI 训练 - 禁闻网</a></li>
<li><a href="https://k.sina.cn/article_1826017320_6cd6d02802001wxju.html">Cloudflare推出新设置：可允许搜索引擎爬取，同时拒绝AI训练|rain|it之家|爬虫|谷歌|微软_新浪新闻</a></li>
<li><a href="https://www.ithome.com/1/003/108.htm">Cloudflare 推出新设置：可允许搜索引擎爬取，同时拒绝 AI 训练 - IT之家</a></li>
<li><a href="https://blog.cloudflare.com/content-independence-day-ai-options/">Your site, your rules: new AI traffic options for all customers | Cloudflare Blog</a></li>
<li><a href="https://www.cloudflare.com/press/press-releases/2025/cloudflare-just-changed-how-ai-crawlers-scrape-the-internet-at-large/">Cloudflare Just Changed How AI Crawlers Scrape the Internet-at-Large; Permission-Based Approach Makes Way for A New Business Model | Cloudflare</a></li>

</ul>
</details>

**标签**: `#Cloudflare`, `#AI爬虫`, `#搜索收录`, `#AI训练数据`, `#网络基础设施`

---

<a id="item-tech-news-11"></a>
### [约 170 万中文赌场网站被 APT 用作恶意软件 C2 基础设施](https://www.theregister.com/security/2026/09/15/low-quality-casino-sites-conceal-highly-dangerous-threat-actors/5296652) ⭐️ 7.0/10

一家网络安全公司发现，大量中文赌博和成人网站表面上是普通娱乐场所，实际可能充当网络攻击基础设施。该公司追踪到约 170 万个中文赌场网站，其中部分被用于恶意软件传播和间谍活动。自 2023 年以来，与中国有关联的 APT 组织利用名为“PeckBirdy”的框架，将恶意软件的命令控制（C2）域名隐藏在低质量赌博网站中，并通过虚假软件更新诱骗用户下载恶意程序。由于这些站点外观与普通赌博网站高度相似，安全人员容易把相关访问误判为员工违规浏览而忽略。

telegram · zaihuapd · 9月16日 07:31

**「背景」** PeckBirdy 是一个基于 JScript 的命令与控制（C2）框架，自 2023 年起被与中国有关联的 APT 组织使用，可在多种环境中灵活部署。安全研究机构 Infoblox 指出，约 170 万个非法中文赌博网站中存在一类被威胁组织用作掩护的站点，这些站点同时承载 C2 基础设施与恶意软件分发网络。这类低质网站中还有一部分从事所谓“scambling”（诈骗赌博）：访客可以下注，但赢钱后无法提现，其外观与普通赌博网站高度相似，因而容易被误判为普通娱乐或员工违规浏览行为。

**「影响」** 对防御方而言，最直接的后果是：指向这些被当作 C2 的赌博域名的访问流量可能被误判为员工违规浏览而未被深入调查，从而延误对相关 APT 活动的发现与处置。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cyberpress.org/peckbirdy-hides-in-casinos/">PeckBirdy Malware Uses Chinese Casino and Adult Websites to Hide...</a></li>
<li><a href="https://www.trendaisecurity.com/en-gb/resources-insights/trendai-security-blog/peckbirdy-script-framework">PeckBirdy : A Versatile Script Framework for LOLBins Exploitation...</a></li>
<li><a href="https://thehackernews.com/2026/01/china-linked-hackers-have-used.html">China -Linked Hackers Have Used the PeckBirdy JavaScript...</a></li>
<li><a href="https://www.theregister.com/security/2026/09/15/low-quality-casino-sites-conceal-highly-dangerous-threat-actors/5296652">Low - quality casino sites conceal highly dangerous threat actors</a></li>
<li><a href="https://lustich.de/news/low-quality-casino-sites-conceal-highly-dangerous-threat-actors">Gefährliche Schadsoftware hinter illegalen Casino -Webseiten entdeckt</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#APT`, `#malware C2`, `#threat intelligence`, `#Chinese-language gambling sites`

---

<a id="item-tech-news-12"></a>
### [新浪云 SAE 将永久下线 早期 B 站视频源文件启动归档](https://tracker.archiveteam.org/sinavideo/#show-all) ⭐️ 7.0/10

据 Telegram 聚合消息，国内首个 PaaS 平台新浪云 SAE 将于 2026 年 9 月 16 日 24 时正式永久下线，所有用户数据将被彻底删除。该平台 2009 年上线，曾以低成本、免运维吸引大量开发者；早期 B 站曾依赖其存储大量视频源文件。目前仍有约 420 TB 历史数据存放在新浪云 S3 桶中，Archive Team 已发起分布式归档项目，称累计抢救约 680 TB、完成度 96.26%。该消息缺少一手技术分析，部分表述可能不确定，但 Archive Team Tracker 为归档进度提供了佐证。

telegram · zaihuapd · 9月16日 15:00

**「背景」** 新浪云 SAE（Sina App Engine）于 2009 年上线，官方将其描述为国内具有影响力的分布式 Web 应用与业务开发托管、运行平台之一，属于 PaaS（平台即服务）模式，开发者无需自行运维服务器即可部署应用。凭借低成本、免运维的特点，它曾被大量国内开发者采用，早期 B 站也将视频源文件托管在该平台的存储中，这批历史数据因此与本次下线直接相关。Archive Team 是一个由志愿者组成的分布式网络归档组织，常在平台关停前发起众包抓取，本次对约 420 TB 新浪云数据的抢救进度即由其追踪页面统计。

**「影响」** 对新浪云 SAE 上的开发者与用户而言，2026 年 9 月 16 日 24 时之后未迁出的数据将被彻底删除，必须在此前完成迁移或备份。早期 B 站视频源文件的存续则取决于 Archive Team 归档项目能否在截止前抢完剩余部分，目前该行动尚未完成，仍存在无法全部保存的风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.sinacloud.com/sae.html">云 应用 SAE - 云 服务 - 云 托管</a></li>

</ul>
</details>

**标签**: `#cloud computing`, `#data preservation`, `#Archive Team`, `#Sina Cloud SAE`, `#Bilibili`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [美联储加息 25 个基点至 3.75%-4%，为三年多来首次](https://www.cnbc.com/2026/09/16/fed-rate-decision-september-2026.html) ⭐️ 9.0/10

美联储周三宣布将联邦基金利率目标区间上调 25 个基点至 3.75%-4%，为 2023 年 7 月以来首次加息，联邦公开市场委员会 12 名投票委员一致支持。会后公布的利率预测（点阵图）显示，18 名参与者中有 16 人预计年内还会再加息，其中 4 人预计可能加两次；美联储同时把今年个人消费支出物价指数预测上调至 3.7%、核心指标上调至 3.4%。

rss · CNBC Finance · 9月16日 21:07

**「背景」** 美联储上一次加息是在 2023 年 7 月，此后一直按兵不动，本次加息前联邦基金利率目标区间为 3.50%–3.75%，而美联储的通胀目标是 2%。现任主席凯文·沃什（Kevin Warsh）于 2026 年就任，此前曾在 2006 至 2011 年担任美联储理事。

**「影响」** 对需要借钱的家庭和企业来说，加息会直接推高借贷成本：30 年期固定利率房贷已升至 7.19%，较一年前高出逾一个百分点，住房市场专家称这已是逾一年来的最高水平。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simple.wikipedia.org/wiki/Kevin_Warsh">Kevin Warsh - Simple English Wikipedia, the free encyclopedia</a></li>
<li><a href="https://www.federalreserve.gov/aboutthefed/bios/board/warsh.htm">Federal Reserve Board - Kevin Warsh, Chairman</a></li>
<li><a href="https://edition.cnn.com/2026/09/16/business/live-news/federal-reserve-interest-rate-september">Fed raises interest rates for the first time since 2023 | CNN Business</a></li>

</ul>
</details>

**标签**: `#Federal Reserve`, `#Interest Rates`, `#Monetary Policy`, `#Inflation`, `#FOMC`

---

<a id="item-finance-news-2"></a>
### [香港推出 11 项鼓励生育措施](https://www.info.gov.hk/gia/general/202609/16/P2026091600265.htm) ⭐️ 7.0/10

香港行政长官李家超在新一份《施政报告》中宣布 11 项鼓励生育的“组合拳”措施，包括把原定今年 10 月 24 日到期的 2 万港元新生婴儿奖励金计划延长 3 年，并将今日或之后出生的第二名及之后子女的奖励金提高至 3 万港元，同样为期 3 年。措施还涵盖子女免税额由 14 万港元上调至 16 万港元、最高 2 万港元印花税减免、居屋白表家庭按揭成数上限提高至 95%，以及增加体外受精名额和幼儿托管服务等。

telegram · zaihuapd · 9月16日 08:01

**「背景」** 香港行政长官李家超在 2026 年施政报告中改变过去的不干预立场，转为以现金奖励、税项宽免、房屋及托育等 11 项措施营造生育友善环境。此前香港已设 2 万港元新生婴儿奖励金计划，原定今年 10 月 24 日到期，这次是延续并加码。

**「影响」** 在香港生育第二名或以上子女的家庭将直接受益：现金奖励与子女免税额提高可减轻养育开支，有新生婴儿的居屋白表申请家庭按揭成数上限升至 95%，首期负担随之下降；香港生育率长期处于全球最低水平，措施针对的正是“想生但不敢生”的家庭。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.ifeng.com/c/8wT4qi5kBpU">2万港元新生婴儿奖励金计划延续3年……香港推11项鼓励生育措施_凤凰网</a></li>
<li><a href="https://www.zaobao.com.sg/news/china/story20260916-9684664">香港施政报告加码催生 | 联合早报</a></li>
<li><a href="https://h5.ifeng.com/c/vivoArticle/v002leYk281--pBRDxcsIcLUjR0tndmXHLMihreMj8jqIehQ__?isNews=1&amp;showComments=0">家庭月入三万不敢 生 娃？ 香 港 生 育 率 全球最低</a></li>

</ul>
</details>

**标签**: `#Hong Kong`, `#fertility policy`, `#fiscal incentives`, `#tax allowances`, `#housing policy`

---

<a id="item-finance-news-3"></a>
### [平陆运河建成通航 西南货物经北部湾直通东盟](https://www.news.cn/politics/20260916/4d3b671357d14c8db202cbf6120f2c43/c.html) ⭐️ 7.0/10

据新华网报道，平陆运河建成通航，全长 134.2 公里，投资 700 多亿元，可通航 5000 吨级船舶，当日“南宁港—越南芹苴港”“南宁港—洋浦港”两条江海直达航线首航。报道称，西南货物经该通道可较传统路径缩短航程 560 公里以上，物流成本降低 18%至 30%。

telegram · zaihuapd · 9月16日 09:10

**「背景」** 平陆运河是中国“西部陆海新通道”（把西部货物经广西沿海港口运往海外的通道体系）的骨干工程，2022 年 8 月开工，为新中国成立以来首条“通江达海”即内河航道直接连通海洋的运河工程，定位是让西南地区货物经北部湾以更短运距出海通往东盟。

**「影响」** 对广西、湖南等西南及中部依赖大宗货物运输的出口企业而言，这条通道把出海路径改经北部湾，据测算每年可节约社会运输费用超 50 亿元，大宗货物综合物流费用有望下降 18%至 30%；广西则可能从长期的内陆腹地转为面向东盟的开放前沿。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.cyol.com/gb/articles/2026-06/04/content_BbNGmOTlYQ.html">通 江达 海 西 部 陆 海 新 通 道 跑出高水 平 对外开放“加速度”</a></li>
<li><a href="https://www.ddgx.cn/show/59283.html">当代广 西 网 -- 读懂 平 陆 运 河 的重大 战 略 意 义</a></li>
<li><a href="https://www.chinanews.com.cn/dxw/2026/09-15/10697067.shtml">东西问丨余虹：平陆运河通航将如何重构中国—东盟经贸格局？-中新网</a></li>
<li><a href="https://www.chinanews.com.cn/aseaninfo/2026/09-16/10697442.shtml">一河通江海 平陆运河铺就中国—东盟经贸合作“水上高速路”-中新网</a></li>
<li><a href="https://www.sohu.com/a/1076477959_121443915">东西问丨余虹：平陆运河通航将如何重构中国—东盟经贸格局？_广西_产业链_物流</a></li>

</ul>
</details>

**标签**: `#平陆运河`, `#基础设施投资`, `#中国-东盟贸易`, `#物流成本`, `#区域经济`

---