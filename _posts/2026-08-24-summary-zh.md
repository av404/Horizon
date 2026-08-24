---
layout: default
title: "Horizon Summary: 2026-08-24 (ZH)"
date: 2026-08-24
lang: zh
---

> 从 44 条内容中筛选出 12 条重要资讯。

---

**科技新闻**
1. [seL4 在 AArch64 上的安全证明完成](#item-tech-news-1) ⭐️ 9.0/10
2. [MS Paint 与照片应用为本地 AI 编辑图片隐式加入 GUID 水印](#item-tech-news-2) ⭐️ 8.0/10
3. [AgentX - InferenceXv3：CUDA 护城河在代理推理中能否保持？](#item-tech-news-3) ⭐️ 8.0/10
4. [小米发布三款玄戒新芯片](#item-tech-news-4) ⭐️ 8.0/10
5. [AI 依赖或致编码专业能力崩溃](#item-tech-news-5) ⭐️ 7.0/10
6. [可执行文件即 SQLite 数据库](#item-tech-news-6) ⭐️ 7.0/10
7. [复古 LLM Bart：基于 1931 年前英语语料训练的开源模型](#item-tech-news-7) ⭐️ 7.0/10
8. [AI 生成可编程 3D 物体：从静态网格到空间软件](#item-tech-news-8) ⭐️ 7.0/10
9. [Anthropic 旗舰 Fable 5 企业需求疲软](#item-tech-news-9) ⭐️ 7.0/10
10. [阿里云 Wan3.0 正式上线，API 最低 0.3 元/秒](#item-tech-news-10) ⭐️ 7.0/10

**财经新闻**
1. [阿里巴巴配售 800 亿港元新股筹资，香港股价一度大跌 10%](#item-finance-news-1) ⭐️ 8.0/10
2. [Hugging Face 探索出售，估值或达 130 亿美元](#item-finance-news-2) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [seL4 在 AArch64 上的安全证明完成](https://proofcraft.systems/news-2026/#2026-08-21) ⭐️ 9.0/10

Proofcraft Systems 宣布已完成 seL4 微内核在 ARM 64 位（AArch64）架构上的完整安全证明，这是形式化验证领域的一个重要里程碑。该成果意味着 seL4 在 AArch64 上的安全属性得到了机器可验证的形式化保证，对使用该内核的关键嵌入式、汽车和军事系统具有重要意义。虽然公告没有提供具体的技术细节，但这一进展进一步巩固了 seL4 作为高可信微内核的地位。

hackernews · snvzz · 8月24日 11:32 · [社区讨论](https://news.ycombinator.com/item?id=49418255)

**「背景」** seL4 是一个以形式化验证著称的微内核，其安全属性通过机器可检查的数学证明加以保证，这在生产级操作系统中十分罕见。此前 seL4 已在部分架构上完成了功能正确性证明，而此次 Proofcraft 宣布在 AArch64（ARM 64 位）架构上完成了包括保密性在内的完整安全证明，且其证明栈可延伸到二进制代码层面，从而大幅减少了抽象模型带来的假设。

**「影响」** 对依赖 seL4 的关键系统开发者而言，AArch64 上的完整安全证明为在高安全要求环境中采用该内核提供了更强的形式化保证，有望推动其在更多安全敏感领域的部署。

**「社区讨论」** 评论中既有对结果适用范围的提醒（如非 MCS、单核限制），也有对侧信道定时攻击可能削弱形式化保证的质疑；还有人讨论了 GenodeOS、LionsOS 等实际使用方，并认为若想真正改善系统安全，还需要原生 seL4/Linux 方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.linxi.com.au/news/sel4-microkernel-achieves-full-formal-security-verification-on-aarch64">seL4 Microkernel Formal Security Proofs Completed on AArch64 ...</a></li>
<li><a href="https://www.newswarden.com/story/sel4-security-proofs-complete-aarch64">The seL4 Microkernel&#x27;s Security Proofs Are Now Complete on ...</a></li>
<li><a href="https://sel4.systems/Verification/proofs.html">seL4 Proofs | seL4 - sel4.systems</a></li>

</ul>
</details>

**标签**: `#seL4`, `#formal verification`, `#microkernel`, `#AArch64`, `#security`

---

<a id="item-tech-news-2"></a>
### [MS Paint 与照片应用为本地 AI 编辑图片隐式加入 GUID 水印](https://xusheng.dev/posts/reversing/mspaint_invisible_watermark/main/) ⭐️ 8.0/10

一项逆向工程调查发现，微软的画图（MS Paint）和照片（Photos）应用会在经过 AI 编辑的图像中静默嵌入不可见的 GUID 水印，即使编辑由本地模型完成也会如此。据提交者称，画图和照片会同时添加可见水印（可关闭）和无法关闭、用户无感知的不可见水印；目前尚不清楚该行为是否也适用于 AI 增强的背景删除或移除等操作。此做法引发隐私担忧，因为嵌入的唯一标识符可能让图像被追溯至具体用户或微软账户。

hackernews · ComputerGuru · 8月24日 15:28 · [社区讨论](https://news.ycombinator.com/item?id=49421158)

**「背景」** 微软的画图（MS Paint）和照片（Photos）应用在本地进行 AI 图像编辑时，会向远程服务器发送强制审核请求，并获取一个由服务器颁发的 16 字节 GUID。随后，该 GUID 会被作为不可见水印嵌入到图像像素中（散布于约 74% 的像素），该行为无法被用户禁用，且即使 AI 生成完全在本地完成也会发生。这些发现来自安全研究人员对 Watermarker.dll 的逆向工程，揭示了微软在 AI 图像编辑功能中隐藏的追踪标识机制。

**「影响」** 对使用画图或照片内置 AI 功能的用户，其输出的图片可能携带与微软账户关联的唯一标识符，未来可能被用于溯源或配合法律请求。

**「社区讨论」** 评论者普遍关注该功能的隐私含义，认为即使有 AI 参与，真正的问题是在用户不知情时写入唯一标识；也有人指出微软此前曾在 Azure DevOps 提交中错误添加 Copilot 水印，并有人报告自己的情况被误触发。部分用户对画图不再是纯像素编辑应用表示失望。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mangodeveloper.com/articles/microsoft-paint-embeds-invisible-guid-watermarks-in-local-ai-images-via-remote-moderation-server">Microsoft Paint Embeds Invisible GUID Watermarks in Local AI ...</a></li>
<li><a href="https://byteiota.com/ms-paint-invisible-server-guid-watermark-ai-image/">MS Paint Embeds Invisible Server GUIDs in Every AI Image</a></li>
<li><a href="https://xusheng.dev/posts/reversing/mspaint_invisible_watermark/main/">Microsoft Paint and Photos Embed Server-Issued GUIDs as ...</a></li>

</ul>
</details>

**标签**: `#Microsoft`, `#AI watermarking`, `#privacy`, `#reverse engineering`, `#image forensics`

---

<a id="item-tech-news-3"></a>
### [AgentX - InferenceXv3：CUDA 护城河在代理推理中能否保持？](https://newsletter.semianalysis.com/p/agentx-inferencexv3-does-cuda-moat) ⭐️ 8.0/10

SemiAnalysis 发布了一份关于 NVIDIA CUDA 护城河在代理推理场景中是否依然稳固的评估，并开源了价值 300 万美元的数据集。该数据集支持超过 100 万上下文长度、多轮对话和子代理场景，且 KVCache 命中率达到 95% 以上。文中还对比了 GB300 NVL72、MI355 和 B200 等硬件在代理推理中的表现。具体结论尚未在摘要中明确给出。

rss · Semianalysis · 8月24日 00:19

**「背景」** SemiAnalysis 推出了一个名为 AgentX 的开源智能体推理基准测试，包含超过百万 token 的上下文、多轮对话和子智能体场景，并声称实测 KVCache 命中率超过 95%。这项测试属于该机构 InferenceX 项目的一部分，主要对比 NVIDIA 与 AMD 等不同芯片和推理框架在长上下文、多轮编码场景下的表现。SemiAnalysis 还公开了一个号称耗资 300 万美元构建的数据集，用于检验 NVIDIA CUDA 软件生态在智能体推理中是否仍构成护城河。

**「影响」** 对于评估智能体推理硬件的 AI 基础设施团队，实测数据显示 NVIDIA 的 CUDA 平台优势仍然明显：GB300 NVL72 相对 B200 仅提升约 5%的每 GPU token 吞吐，但 B200 每 token 成本低 29%；而在高并发 MoE 负载（如 DeepSeek-R1）中，GB200 NVL72 的吞吐量可比 AMD MI355X 高出最多 28 倍，表明系统级优势并不能仅以原始算力解释。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://aiweekly.co/alerts/semianalysis-agentx-benchmark-says-cuda-moat-holds-in-agents">SemiAnalysis AgentX benchmark says CUDA moat holds in agents</a></li>
<li><a href="https://inferencex.semianalysis.com/">Open-Source Agentic Inference Benchmark | InferenceX</a></li>
<li><a href="https://inferencex.semianalysis.com/compare/minimax-m27-b200-vs-gb300">B 200 vs GB 300 NVL 72 : MiniMax M2.7 Inference ... | InferenceX</a></li>
<li><a href="https://www.kad8.com/ai/gb200-nvl72-vs-mi355x-why-systems-win-moe-inference/">GB200 NVL 72 vs MI 355 X: Why Systems Win MoE Inference · KAD</a></li>

</ul>
</details>

**标签**: `#AI inference`, `#CUDA`, `#NVIDIA`, `#hardware`, `#agentic AI`

---

<a id="item-tech-news-4"></a>
### [小米发布三款玄戒新芯片](https://mp.weixin.qq.com/s/ceIQbNnZrcNQqGywXCiXTQ) ⭐️ 8.0/10

小米发布三款玄戒系列新芯片：AI 旗舰 SoC 玄戒 O3、高带宽 AI 加速芯片玄戒 O100，以及国内首款 3nm 智驾 AI 芯片玄戒 D100，三款均完成回片验证并覆盖人车家全生态端侧 AI 算力需求。玄戒 O3 采用十核全大核 CPU，多核跑分首破 15000 分，GPU 首发 G2-Ultra NX，性能提升 85%、功耗下降 64%，同时是全球首款支持 LPDDR6 的移动处理器，带宽 113.8 GB/s，NPU 端侧 AI 性能提升 45%，将首发搭载于小米 18 Fold。玄戒 D100 采用 3nm 工艺，集成 20 核 CPU 与 16 核 NPU，最高支持 160GB 统一内存，可本地部署 200B 参数量大模型，预计明年商用。玄戒 O100 是行业首款 6nm 晶圆级垂直堆叠先进封装芯片，采用 Hybrid Bonding 混合键合工艺，键合间距 1.4 微米，带宽 1.22TB/s，为传统旗舰手机的 16 倍，端侧推理速度最高 330TPS。

telegram · zaihuapd · 8月24日 07:18

**「背景」** 玄戒（Xuanjie）是小米自研芯片系列，此前已用于小米手机的 SoC 及部分组件。此次发布的三款芯片覆盖不同场景：O3 面向旗舰手机，O100 面向 AI 加速，D100 面向智能驾驶，官方称三者均已完成回片验证。按外部报道，O3 将首发搭载于小米 18 Fold，D100 计划明年商用，显示小米正将自研芯片从手机 SoC 扩展为“人车家”全生态的端侧 AI 算力基础。

**「影响」** 玄戒 O3 将首发搭载于小米 18 Fold，玄戒 D100 预计明年正式商用，小米由此打通手机、汽车和全生态的端侧 AI 算力布局。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.kucoin.com/news/flash/xuanji-o3-o100-d100-chips-launched-by-xiaomi">Xiaomi Launches Xuanji O3, O100, and D100 Chips - KuCoin</a></li>

</ul>
</details>

**标签**: `#chips`, `#AI`, `#SoC`, `#Xiaomi`, `#hardware`

---

<a id="item-tech-news-5"></a>
### [AI 依赖或致编码专业能力崩溃](https://larsfaye.com/articles/ai-coding-will-prevent-expertise) ⭐️ 7.0/10

作者 Lars Faye 在题为《Coding expertise is going to collapse from AI reliance》的文章中警告，软件工程师大量依赖 AI 编码助手会阻碍深层专业知识的形成，使行业面临专家断层的风险。文章在 Hacker News 上引发广泛讨论，获得 404 分和 413 条评论，许多从业者给出具体观察：企业领导层已出现“手工写代码就是错”的强制要求，AI 生成的代码量正超过人类能够理解和审查的速度；同时，有 15 年经验者主张“引导式编码”——在编辑器内用 LLM 辅助但保持人工主导——可兼顾产出效率与代码质量。文章核心论点是，缺少刻意练习和“摩擦”的长期技能培养，会让单纯依赖 AI 的工程师难以建立真正的判断力。

hackernews · larsfaye · 8月24日 15:52 · [社区讨论](https://news.ycombinator.com/item?id=49421554)

**「背景」** 这篇文章的核心论点是，随着大语言模型和代理式工作流不仅能编写和调试代码，还能基于训练数据中的模式进行系统设计，软件工程师若长期依赖 AI，可能绕过传统技能形成所需的“摩擦”，从而难以积累深度专业能力。该议题的背景是 AI 编码助手已大规模进入企业开发流程，代码生成速度远超人工审查能力，关于开发者长期能力培养和“ AI 技术债”的讨论因此变得更加紧迫。

**「影响」** 直接影响是，采取“AI 优先”政策的企业可能在短期内提高代码产出，但会牺牲可审查性和质量，并让工程师失去成长为资深专家的路径；社区中的实际案例已显示，坚持传统写码的人反而要承担审查大量劣质 AI 代码的负担。

**「社区讨论」** 评论共识与文章观点一致：多数人担心 AI 依赖正在侵蚀专业能力，并指出闭环困境——AI 生成代码越多，人工审查越跟不上，最终由少数未“烧脑”的开发者收拾残局；也有人提出反例，认为正确的“引导式编码”实践能同时保持高效与高质量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://larsfaye.com/articles/ai-coding-will-prevent-expertise">AI Coding will Prevent Expertise | Lars Faye</a></li>

</ul>
</details>

**标签**: `#AI coding`, `#software engineering`, `#expertise`, `#LLM`, `#developer productivity`

---

<a id="item-tech-news-6"></a>
### [可执行文件即 SQLite 数据库](https://fzakaria.com/2026/08/23/your-executable-is-a-sqlite-database) ⭐️ 7.0/10

这篇文章提出并探讨了一个新颖的技术想法：把 ELF 可执行文件本身当作 SQLite 数据库来嵌入和查询，使二进制文件自带结构化元数据并可用 SQL 访问。作者认为 ELF 已经具有数据库性质，并展示了 SQLite 虚拟表等机制能让可执行文件内容被“挂载”为表格。这个方向有望让二进制分析、自描述工具和多版本“胖”可执行文件变得更直接，例如基于 WebAssembly 或条件化本地代码分发的场景。社区反馈普遍积极，但作者提到该想法在学术圈最初并不被看好。

hackernews · setheron · 8月24日 04:48 · [社区讨论](https://news.ycombinator.com/item?id=49415271)

**「背景」** ELF 是 Linux 和类 Unix 系统上可执行文件的标准格式，其内容由若干具有不同用途的节（sections）组成，用于存放代码、数据、符号表等结构化信息。SQLite 则是一种轻量级嵌入式数据库，将数据保存在单一文件中，并支持通过 SQL 查询。本文提出的想法是将可执行文件同时构造为一个 SQLite 数据库，使得 ELF 二进制文件本身可以直接用 SQL 查询内部结构，从而让程序具备自描述性和可探查性。

**「影响」** 对于从事二进制分析、可执行文件打包和软件供应链工具的开发人员，这一思路提供了一种直接用 SQL 查询二进制内部信息的有效路径，可能降低构建元数据与运行时结构分离带来的工具复杂度。

**「社区讨论」** 评论者普遍对这个想法感到兴奋，认为它可以用于制作“胖”可执行文件、内置虚拟文件系统甚至替代 AppImage；作者则表示该想法在学术圈发表时反馈并不友好，但很高兴看到社区讨论热情。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=49415271">Executable Is a SQLite Database | Hacker News</a></li>

</ul>
</details>

**标签**: `#SQLite`, `#ELF`, `#executables`, `#databases`, `#software-engineering`

---

<a id="item-tech-news-7"></a>
### [复古 LLM Bart：基于 1931 年前英语语料训练的开源模型](https://www.reddit.com/r/MachineLearning/comments/1vx94er/bart_a_vintage_llm_r/) ⭐️ 7.0/10

Unbounded Labs 发布了复古大语言模型 Bart，这是一个从零训练的 2.82B 参数模型，基于 20.1B token 的 1931 年前英语语料。项目旨在探索 Demis Hassabis 提出的问题：LLM 是否能得出过去伟大科学家曾得出的结论。团队清理了哈佛 Institutional Books 数据集（242B 降至 23B token），创建了首个面向复古 LLM 的 20 项基准套件 Vintage CORE，并发布了 416k 带评分问答对的 SFT 数据集、训练代码和评估结果。最终模型在 H100 上训练 5 天，保持 60% MFU，总花费约 807 美元。项目开放了全部资源，同时团队正在寻求算力资助与导师支持。

reddit · r/MachineLearning · /u/soggydoggy8 · 8月24日 17:20

**「背景」** 复古 LLM（Vintage LLM）指用特定历史时期的文本训练的模型，用来研究模型能否从有限历史语料中独立演绎出科学见解。Hassabis 曾提出此类设想，但缺少对应的历史语料和评测基准，因此团队需要自己构建数据与测试体系。

**「影响」** 该工作为历史语料 NLP 研究提供了首个开放的大规模预训练模型、20 项基准和 416k 指令数据集，使其他研究者无需重建数据管道即可复现和扩展此类实验。由于训练预算和算力有限，模型规模与通用能力仍明显受限于当代主流 LLM。

**标签**: `#LLM`, `#NLP`, `#historical text`, `#research`, `#open source`

---

<a id="item-tech-news-8"></a>
### [AI 生成可编程 3D 物体：从静态网格到空间软件](https://www.reddit.com/r/MachineLearning/comments/1vxcc1h/r_using_ai_as_a_spatial_software_generator_to/) ⭐️ 7.0/10

这篇论文提出用大语言模型（LLM）作为空间软件生成器，直接生成具有内在可编程性的 3D 对象，而不是传统 AI 3D 生成器输出的整体式网格。作者（也是提交者）在 nova3d.xyz 上提供了可视化演示，并附有 GitHub 仓库；演示对象由逻辑部件组成，开箱即带自然运动，具备动画就绪、层级结构和铰链/插槽关节，并能根据弱/强计算环境自动切换外观。这类“软件形态”的 3D 对象从创建之初就包含逻辑，适合工业设计、游戏开发、模拟和 AR/VR/XR，但在复杂有机形状上仍落后于传统 AI 3D 生成器。作者认为随着 LLM 的空间编码能力增强，代码最终会取代所有 3D 内容生成方式。

reddit · r/MachineLearning · /u/mhb\_11 · 8月24日 19:10

**「背景」** 传统 AI 3D 生成器通常输出单一整体式网格（mesh），难以直接用于动画和逻辑控制，需要额外的建模和绑定工作。把 3D 对象视为软件，意味着 LLM 可以生成由零件、关节和运行逻辑构成的结构化程序，使对象在生成时就具备可编辑、可运动、可跨平台表现的能力。

**「影响」** 对图形学和机器学习开发者来说，这项研究把 AI 3D 生成的产物从“静态网格”推向“可编程对象”，使动画、程序化修改和设备自适应成为生成时内置能力，最可能影响工业设计、游戏、仿真和 AR/VR/XR 流程。当前在复杂有机形状上的表现仍弱于传统 AI 3D 生成器，因此短期替代性有限。

**标签**: `#3D generation`, `#machine learning`, `#LLM`, `#programmable graphics`, `#procedural modeling`

---

<a id="item-tech-news-9"></a>
### [Anthropic 旗舰 Fable 5 企业需求疲软](https://www.ft.com/content/5ee49718-c258-4f01-aa32-7e5b76ae5245) ⭐️ 7.0/10

Anthropic 最强模型 Fable 5 在企业市场遇冷。Ramp 数据显示，该模型上市首月仅占 Anthropic API token 用量约 6%、支出约 11%。其定价约为每百万输入 token 10 美元、每百万输出 token 50 美元，约是自家其他旗舰模型的两倍，也高于 OpenAI 的 GPT-5.6 Sol。便宜的开源模型和微软自研模型正在分流客户，Anthropic 保留用户数据 30 天的要求也抑制了需求。Ramp 经济学家认为，这表明企业为前沿 AI 付费的意愿已触及天花板。

telegram · zaihuapd · 8月24日 01:22

**「背景」** Anthropic 是领先的人工智能公司，其旗舰模型通常以较高性能和高定价面向企业客户。企业在采用前沿 AI 时，会在性能、价格、数据隐私和合规之间权衡，而开源模型与大型云厂商自研模型提供了更具性价比或更灵活的替代选择。

**「影响」** 企业客户可能继续转向开源或微软等低价模型，迫使 Anthropic 重新考虑其定价和数据保留政策。

**标签**: `#AI`, `#enterprise`, `#pricing`, `#open-source`, `#Anthropic`

---

<a id="item-tech-news-10"></a>
### [阿里云 Wan3.0 正式上线，API 最低 0.3 元/秒](https://mp.weixin.qq.com/s/peeeU6cBz4AaROvFe1zqQQ) ⭐️ 7.0/10

阿里云视频生成模型 Wan3.0 于今日正式上线，支持最长 30 秒视频生成，并在人物质感、参考精准一致性和非写实风格化方面表现突出。用户可通过阿里云百炼、万相官网、千问 APP 等平台体验。API 价格按分辨率区分，480P、720P、1080P 分别为 0.3 元/秒、0.6 元/秒和 1.2 元/秒。8 月 24 日至 9 月 23 日期间，阿里云百炼和千问 AI 平台提供 API 限时 7 折优惠。以上信息来自官方发布，但公告未包含更详细的技术参数或基准测试结果。

telegram · zaihuapd · 8月24日 10:14

**「背景」** 阿里云万相（Wan）是其推出的 AI 视频生成模型及创意平台，支持文生图、图生图、文生视频、图生视频和图像编辑等功能。Wan 3.0 于 2026 年 8 月 6 日发布并开启公测，单次可生成最长 30 秒视频，且支持无缝延长，同时首次支持 doc、xls、ppt、pdf、md 等文档格式输入，无需重新格式化。

**「主要影响」** 对于想要调用 Wan3.0 API 的开发者，虽然阿里云官方宣布正式上线，但实际接入可能处于预览或邀请制状态，并非完全开放注册；同时在 8 月 24 日至 9 月 23 日期间，百炼和千问平台提供 7 折优惠，480P/720P/1080P 价格分别约为 0.3/0.6/1.2 元/秒。模型尚未公布具体性能指标，其市场表现将取决于定价吸引力和实际生成质量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://aihot.virxact.com/story/a99af99d-0dff-4752-a453-37de2d1a0c65">Alibaba Cloud releases Wan 3 . 0 · AI HOT</a></li>
<li><a href="https://wan.video/">Wan AI: Leading AI Video Generation Model</a></li>
<li><a href="https://juejin.cn/post/7670593377075724339">juejin.cn/post/7670593377075724339</a></li>
<li><a href="https://www.ngram.com/blog/wan-3-0-document-to-video-ai-model">Wan 3.0: Alibaba&#x27;s Document-to-Video AI Model Explained | ngram.com</a></li>

</ul>
</details>

**标签**: `#video generation`, `#Alibaba Cloud`, `#generative AI`, `#API pricing`, `#AI models`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [阿里巴巴配售 800 亿港元新股筹资，香港股价一度大跌 10%](https://www.cnbc.com/2026/08/24/alibaba-share-placement-drop-ai-hong-kong.html) ⭐️ 8.0/10

阿里巴巴周一在香港股市一度大跌 10%，此前公司宣布向非美国投资者配售 7.1 亿股新股，每股定价 112.70 港元，筹资 800 亿港元（约 102 亿美元），较上周五收盘价 123 港元折让约 8.4%；公司表示净收益将全部用于发展 AI 能力，尤其是扩建 AI 基础设施。

rss · CNBC Finance · 8月24日 08:21

**「背景」** 阿里巴巴上周公布的截至 6 月当季财报显示，利润大跌 75%，同期资本开支跃增 75%至 677 亿元人民币；公司此前还宣布，未来三年拟在云计算和 AI 基础设施上投资至少 3800 亿元人民币。

**「影响」** 此次配售将摊薄现有股东权益，并凸显 AI 资本开支持续挤压盈利的压力。

**标签**: `#Alibaba`, `#share placement`, `#AI investment`, `#Hong Kong stocks`, `#Chinese tech`

---

<a id="item-finance-news-2"></a>
### [Hugging Face 探索出售，估值或达 130 亿美元](https://www.bloomberg.com/news/articles/2026-08-23/hugging-face-gauging-interest-for-potential-sale-business-insider-says) ⭐️ 7.0/10

据 Business Insider 报道，Hugging Face 正探索出售，估值可能达到 130 亿美元或更高；公司已与银行合作评估买家兴趣，但尚未达成交易。

telegram · zaihuapd · 8月24日 05:45

**「背景」** 该公司 2023 年完成 2.35 亿美元融资后估值为 45 亿美元；近期 OpenAI 披露，其一未发布模型意外入侵该平台获取考试答案，引发对 AI 模型安全性的担忧。

**标签**: `#M&amp;A`, `#AI`, `#valuation`, `#startup`, `#tech`

---