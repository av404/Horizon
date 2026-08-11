---
layout: default
title: "Horizon Summary: 2026-08-11 (ZH)"
date: 2026-08-11
lang: zh
---

> 从 45 条内容中筛选出 17 条重要资讯。

---

**科技新闻**
1. [窃取专有大模型 API 推理痕迹的技术引发争议](#item-tech-news-1) ⭐️ 8.0/10
2. [Meta 发布开源 30B 智能体模型 Muse Glimmer](#item-tech-news-2) ⭐️ 8.0/10
3. [Nvidia Nemotron 3.5 Lightning 与 NeMo Switchyard 发布](#item-tech-news-3) ⭐️ 7.0/10
4. [Mojo 1.0 发布：面向高性能 AI 的 Python 超集语言](#item-tech-news-4) ⭐️ 7.0/10
5. [Nvidia 的风险生意：分析其 AI 硬件与软件战略](#item-tech-news-5) ⭐️ 7.0/10
6. [伦敦地铁试点面部识别](#item-tech-news-6) ⭐️ 7.0/10
7. [解耦下降：用 AMP 修正实现精确训练-测试误差追踪](#item-tech-news-7) ⭐️ 7.0/10
8. [HyperSAE：为稀疏自编码器引入解耦庞加莱几何，MSE 降 9.8%](#item-tech-news-8) ⭐️ 7.0/10
9. [Anthropic 将为 Claude 输出加入 AI 标记与 C2PA 元数据](#item-tech-news-9) ⭐️ 7.0/10
10. [石墨烯软性镜片：电控变焦的新突破](#item-tech-news-10) ⭐️ 7.0/10
11. [Manus 与 Meta 分离，部分数据限期删除](#item-tech-news-11) ⭐️ 7.0/10

**财经新闻**
1. [盘后大涨：超微电脑、CoreWeave、H&amp;R Block 发布超预期业绩或指引](#item-finance-news-1) ⭐️ 8.0/10
2. [英伟达 5000 亿美元 AI 融资计划面临中国芯片价格战风险](#item-finance-news-2) ⭐️ 8.0/10
3. [SK 海力士重启大连二厂建设，NAND 产能将提升约五成](#item-finance-news-3) ⭐️ 8.0/10
4. [美国选举押注禁令引发预测市场法律不确定性](#item-finance-news-4) ⭐️ 7.0/10
5. [Amkor 据称考虑出售中国业务股份，估值或达 15 亿美元](#item-finance-news-5) ⭐️ 7.0/10
6. [恒生科技指数拟扩容至 50 只并调整选股机制](#item-finance-news-6) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [窃取专有大模型 API 推理痕迹的技术引发争议](https://stolen-thoughts.com/) ⭐️ 8.0/10

一篇名为《Stealing Reasoning Traces from Proprietary LLM APIs》的文章展示了如何从专有大模型 API 中提取隐藏的推理痕迹，方法包括将前沿模型生成的痕迹回放到较弱模型中，并对较弱模型进行越狱。有评论者还指出，只需禁用思考并提供一个“deep\_think”工具，模型便可能以内部思维链格式输出推理内容。此事引发了关于模型输出所有权、透明度以及“窃取”一词是否恰当的广泛辩论。有评论预期未来模型可能会拒绝分享推理过程，或要求使用企业级 API 才能获取。

hackernews · quantumgarbage · 8月11日 13:22 · [社区讨论](https://news.ycombinator.com/item?id=49257876)

**「背景」** 主流大型语言模型提供商为了保护知识产权和减少信息泄露，开始隐藏模型逐步推理过程（即思维链），但并未完全在服务端存储这些痕迹，而是将其作为加密文本块返回给客户端，由客户端在后续请求中回传。此前已有研究指出这种机制存在安全弱点，本文在此基础上提出了重放和越狱等具体技术，能够从专有 API 中提取被隐藏的推理痕迹，引发关于模型输出所有权和透明度的讨论。

**「影响」** 对于依赖专有大模型 API 的开发者与 AI 安全研究者，该技术可能使封闭模型隐藏的推理过程更易被获取，从而削弱厂商对模型输出的控制，并影响其基于推理隐藏而设计的商业模式。

**「社区讨论」** 讨论中有人质疑“窃取”这一说法，认为用户已为 token 付费且模型基于人类知识训练，对模型输出进行再训练应属正常；另有实践者报告用两句话的&lt;developer&gt;提示即可让加密压缩数据以明文输出，还有人好奇跨模型回放是否是有意放任。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2608.09867">Stealing Reasoning Traces from Proprietary LLM APIs</a></li>
<li><a href="https://stolen-thoughts.com/paper.pdf">Stealing Reasoning Traces from Proprietary LLM APIs</a></li>
<li><a href="https://devsandlogics.com/blog/stealing-reasoning-traces-from-proprietary-llm-apis">Stealing Reasoning Traces from Proprietary LLM APIs: A 2026 ...</a></li>

</ul>
</details>

**标签**: `#LLM`, `#AI security`, `#chain-of-thought`, `#proprietary APIs`, `#jailbreak`

---

<a id="item-tech-news-2"></a>
### [Meta 发布开源 30B 智能体模型 Muse Glimmer](https://simonwillison.net/2026/Aug/10/introducing-muse-glimmer/#atom-everything) ⭐️ 8.0/10

Meta 发布了 Muse Glimmer，一个全新的 30B 开源权重模型，采用 Apache 2.0 许可，专注于端到端智能体任务完成、可靠工具调用和多步推理。官方称其在 DeepSearch QA、MCP-Atlas、tau-Bench 和 SWE-Bench 等完整任务基准上取得较好成功率。该模型同时支持视觉输入；Simon Willison 用 LM Studio 提供的 18.16 GB 量化版本测试了本地运行，并让它通过 llm-coding-agent 插件在 Datasette 代码库中执行“how does auth work?”任务，记录了完整工具调用过程。作者表示在 32GB 或以上内存的机器上，这类尺寸的模型可留出充足空间运行其他应用。Muse Glimmer 的开放许可是对早期 Llama 许可证的一次改进。

rss · Simon Willison · 8月10日 23:56

**「背景」** Muse Glimmer 是 Meta 新发布的一款 300 亿参数（30B）的开源权重模型，采用 Apache 2.0 许可证，针对端到端智能体任务、可靠工具调用和多步推理进行了优化。它可以在配备单个消费级 GPU 的 Mac 或 PC 上本地运行，例如约 24GB 显存即可运行，因此适合本地智能体与函数调用等场景。据外部报道，该模型是从 Muse Spark 蒸馏而来，旨在兼顾本地运行效率与智能体任务表现。

**「影响」** 对于希望在本地运行开源智能体模型的开发者和研究人员，Muse Glimmer 提供了 30B Apache-2.0 选项，可在 32GB 以上内存的机器上与其它应用并行运行，并支持工具调用和视觉理解，免去专有许可限制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://research.meta.ai/blog/introducing-muse-glimmer-open-agentic-model">Introducing Muse Glimmer: An Open Agentic Model That Runs on Your Device | Meta AI Research</a></li>
<li><a href="https://venturebeat.com/technology/meta-returns-to-open-source-with-muse-glimmer-an-apache-2-0-licensed-30b-parameter-ai-model-optimized-for-agents-available-now">Meta returns to open source with Muse Glimmer, an Apache 2.0 licensed 30B parameter AI model optimized for agents — available now | VentureBeat</a></li>
<li><a href="https://explainx.ai/blog/meta-muse-glimmer-open-weight-30b-agentic-model-2026">Muse Glimmer: Meta&#x27;s 30B Open Model Runs on 24GB VRAM | explainx.ai Blog | explainx.ai</a></li>

</ul>
</details>

**标签**: `#Meta`, `#open source`, `#AI`, `#agentic`, `#large language model`

---

<a id="item-tech-news-3"></a>
### [Nvidia Nemotron 3.5 Lightning 与 NeMo Switchyard 发布](https://blogs.nvidia.com/blog/nemotron-lightning-switchyard-rtx-dgx/) ⭐️ 7.0/10

Nvidia 发布了 Nemotron 3.5 Lightning 小型模型和 NeMo Switchyard 开源库，后者用于智能地将请求路由到最合适的模型。这一发布凸显了行业向更小、更专用模型转变的趋势，并为高效模型部署提供了实用工具。Nvidia 表示，NeMo Switchyard 部署后可以根据请求特点选择能力与成本最匹配的模型；Nemotron 3.5 Lightning 则是面向高效推理的小型模型系列。现有信息未提供具体模型尺寸、性能数据或可用日期，因此这些细节仍有待官方进一步说明。整体上，该发布对 AI 基础设施和模型路由工具链具有重要意义。

hackernews · droidjj · 8月11日 19:35 · [社区讨论](https://news.ycombinator.com/item?id=49263340)

**「背景」** NVIDIA 发布了 Nemotron 3.5 Lightning，这是一个 300 亿参数的混合专家（MoE）模型，专为大型多智能体系统中的特定任务而设计，旨在提升智能体应用的效率与效果。同时，NVIDIA 还推出了 NeMo Switchyard，这是一个开源库，能够智能地把每个请求路由到最合适、最强大的模型上。这一背景反映了 AI 行业从追求超大规模参数模型转向更小、更专业模型的趋势。

**「影响」** 对于正在构建或部署 AI 服务的开发者，NeMo Switchyard 提供了一种开源的路由方案，可以在不同模型之间分配请求，从而可能降低推理成本并提升响应效率；但实际效果取决于路由策略、提示缓存处理以及模型选择等具体实现。

**「社区讨论」** 评论中，有用户认为算力紧张正促使行业更关注小而高效的模型，并看好其推动结构性的进步；也有用户质疑路由器如何处理提示缓存和会话粘性，另有人批评基准图表未包含 Qwen 系列，还有用户报告 Nemotron 3.5 Lightning 30b 在 Apple Silicon 上运行良好但速度较慢。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blogs.nvidia.com/blog/nemotron-lightning-switchyard-rtx-dgx/">NVIDIA Nemotron 3 . 5 Lightning and NeMo Switchyard Deliver...</a></li>

</ul>
</details>

**标签**: `#nvidia`, `#nemotron`, `#small-language-models`, `#model-routing`, `#open-source`

---

<a id="item-tech-news-4"></a>
### [Mojo 1.0 发布：面向高性能 AI 的 Python 超集语言](https://www.modular.com/blog/modular-26-5-mojo-1-0-is-here) ⭐️ 7.0/10

Modular 公司发布 Mojo 1.0，这是面向高性能 AI 计算、定位为 Python 超集的新编程语言的首个稳定版本。Mojo 旨在结合 Python 的易用性与接近 C/C++/Rust 的性能，目前聚焦于 AI/ML 工作负载。然而，社区对该版本存在明显疑虑：编译器仍为闭源，官方仅承诺在 2026 年开源 Mojo 编译器和工具链；同时路线图显示 Mojo 是否能成为完整 Python 超集已被弱化，官方表示“可以不是”。此外，有用户认为官网缺乏一页式概述，难以理解语言定位和选型理由。总体而言，1.0 是 Mojo 的重要里程碑，但开放性与定位问题仍限制其被更广泛采用。

hackernews · dayanruben · 8月11日 16:56 · [社区讨论](https://news.ycombinator.com/item?id=49261128)

**「背景信息」** Mojo 是由 Modular 公司开发的一种编程语言，Modular 由 Chris Lattner（Swift 语言和 LLVM 的原始架构师）与 Tim Davis（前 Google 员工）共同创立。其设计目标是弥合 Python 易用性与 AI 应用所需高性能之间的差距，希望开发者能用 Python 的直观语法编写面向 CPU、GPU 和其他加速器的系统级代码。此次 Mojo 1.0 发布是该语言发展的重要里程碑，但其编译器尚未完全开源，社区中也存在对其开放性和定位的讨论。

**「影响」** 对考虑在 AI/ML 项目中使用 Python 兼容高性能语言的开发者而言，Mojo 1.0 提供了一个可评估的稳定基线，但闭源编译器、2026 年开源承诺和超集定位弱化都意味着在正式生产依赖前需要更多验证。

**「社区讨论」** 社区讨论中，部分用户希望官方提供一页式定位说明，并对闭源编译器表示不信任，认为已有 Pydantic/Rust 等替代方案；另有用户注意到路线图中“完整 Python 超集”目标被弱化，并对 2026 年才开源编译器的安排提出质疑。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mojo_%28programming_language%29">Mojo (programming language) - Wikipedia</a></li>

</ul>
</details>

**标签**: `#mojo`, `#programming-language`, `#ai`, `#python`, `#release`

---

<a id="item-tech-news-5"></a>
### [Nvidia 的风险生意：分析其 AI 硬件与软件战略](https://stratechery.com/2026/nvidias-risky-business/) ⭐️ 7.0/10

Stratechery 发表分析文章《Nvidia&\#x27;s Risky Business》，审视英伟达在 AI 硬件与软件领域的商业风险与战略位置。文章结合公司对算力需求持续增长的押注，认为尽管第一层假设（算力、芯片与数据中心需求巨大）大概率正确，第二层假设（需求增长速度）可能被高估。分析还涉及英伟达在机器学习研究中的软件生态优势——其技术早已深入下游——以及 CUDA C/C++ 开发体验糟糕、CPU 与 GPU 计算根本差异等争议点；此外，英伟达正布局机器人领域，并仍是西方市场的主要玩家。由于本次仅提供元数据与评论，具体论据与数据以原文为准。

hackernews · jonbaer · 8月11日 10:02 · [社区讨论](https://news.ycombinator.com/item?id=49255710)

**「背景」** Stratechery 的 Ben Thompson 于 2026 年 8 月 11 日发表分析文章《Nvidia 的冒险生意》，探讨英伟达在 AI 硬件与软件生态中的战略风险与市场地位。文章提到，英伟达 CEO 黄仁勋通过其新的 X 账号可以直接向公众发声，而不必依赖传统媒体。该分析受到 Hacker News 社区关注，讨论涉及英伟达在 CUDA 软件生态、投资预期以及机器人领域布局等方面的优势与不确定性。

**「社区讨论」** 评论者普遍认可文章对英伟达位置的独特剖析，同时指出其真正的护城河是嵌入机器学习研究的软件生态，而非单纯硬件性能；但 CUDA C/C++ 的开发体验被认为极差。也有人认为这类投资逻辑的第一层假设正确、第二层增长假设容易失准，并补充英伟达还有机器人业务与西方市场主导地位等长期变量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://stratechery.com/2026/nvidias-risky-business/">Nvidia ’ s Risky Business – Stratechery by Ben Thompson</a></li>

</ul>
</details>

**标签**: `#Nvidia`, `#AI hardware`, `#business strategy`, `#software ecosystem`, `#industry analysis`

---

<a id="item-tech-news-6"></a>
### [伦敦地铁试点面部识别](https://www.btp.police.uk/news/btp/news/england/btp-expands-live-facial-recognition-lfr-trial-into-london-underground-stations/) ⭐️ 7.0/10

英国交通警察局（BTP）将实时面部识别试验扩展到伦敦地铁站，开始在地铁站内扫描乘客面部。官方称这次是“实时面部识别（LFR）”试点，但具体识别范围、数据处理方式和试验期限没有在来源中说明。该部署延续了执法部门在公共交通中扩大监控技术的趋势，也引发对隐私、公民自由和 AI 伦理的强烈关注。由于缺乏公开的试验结果数据，其实际成效和是否转为永久部署仍属未知。

hackernews · BlueBerry2001 · 8月11日 09:40 · [社区讨论](https://news.ycombinator.com/item?id=49255496)

**「背景」** 英国交通警察局（BTP）正在把实时面部识别（LFR）试验扩大到伦敦地铁（London Underground）站点，此前已在大伦敦多个主要火车站部署。根据警方部署日志，2 月至 7 月间该技术在主要火车站使用 18 次，扫描超过 53 万张面孔。此次扩展旨在评估这一技术在地铁不同交通环境中的表现，并继续改进其在铁路网中的使用方式。

**「社区讨论」** 评论普遍担忧隐私与公民自由被侵蚀，并质疑试验的成效：有用户讽刺称“这样就能解决街头犯罪吗”，也有人认为试验缺乏明确的失败条件，最终只会用于识别、渗透和压制活动。另一部分评论指出匿名出行伦敦地铁早已因非接触式支付而消失，英国在监控议题上被视为“老大哥社会”，还有人将其与中国对比并批评治安政策。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.btp.police.uk/news/btp/news/england/btp-expands-live-facial-recognition-lfr-trial-into-london-underground-stations/">BTP expands Live Facial Recognition (LFR) trial into London Underground stations | British Transport Police</a></li>
<li><a href="https://www.bbc.co.uk/news/articles/c07r0gvgjxyo">Facial recognition cameras to be trialled at London Tube stations - BBC News</a></li>
<li><a href="https://www.itv.com/news/london/2026-08-11/live-facial-recognition-technology-to-be-deployed-at-tube-stations">Live facial recognition technology to be deployed at Tube stations | ITV News London</a></li>

</ul>
</details>

**标签**: `#facial recognition`, `#privacy`, `#surveillance`, `#AI ethics`, `#London`

---

<a id="item-tech-news-7"></a>
### [解耦下降：用 AMP 修正实现精确训练-测试误差追踪](https://www.reddit.com/r/MachineLearning/comments/1vlu1se/decoupled_descent_enforcing_exact_traintest_error/) ⭐️ 7.0/10

研究者提出了一种名为“解耦下降”（Decoupled Descent, DD）的神经网络训练方法，利用近似消息传递（AMP）中的 Onsager 修正，在每次参数迭代时生成证书，保证训练误差在渐近意义上等于测试误差，从而缓解全批量梯度下降中训练误差归零而测试误差不降甚至上升的问题。该理论工作基于高维统计，在风格化的高斯混合模型和两层网络的高维 XOR 模拟中展示了 DD 相对标准 GD 的优势，但作者强调这是理论论文，距离大规模模型仍有距离，并计划未来开发 PyTorch 兼容包。

reddit · r/MachineLearning · /u/mlovik1 · 8月11日 21:06

**「背景」** 近似消息传递（AMP）是一种源于高维统计推断的技术，最初用于压缩感知和线性模型，其关键“Onsager 修正”项可消除迭代过程中的相关性，使算法能在渐近意义下被精确分析。Decoupled Descent（DD）借用了这一思想，针对风格化的高斯混合模型设计训练算法，使训练误差在每一参数迭代处渐近地等于测试误差。该工作发表于 arXiv（2604.27883），属于理论性论文，尚需进一步推广到 SGD 或更大规模模型。

**「影响」** 该研究可能为理解神经网络的泛化与数据重用偏差提供新的理论视角，并为最优停止和超参数调优提供基于精确误差追踪的训练策略，但目前仅限理论模型，实际应用尚需验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/html/2604.27883v1">Decoupled Descent: Exact Test Error Tracking Via Approximate Message Passing</a></li>
<li><a href="https://arxiv.org/abs/2604.27883">[2604.27883] Decoupled Descent: Exact Test Error Tracking Via Approximate Message Passing</a></li>

</ul>
</details>

**标签**: `#machine learning`, `#generalization`, `#optimization`, `#approximate message passing`, `#neural networks`

---

<a id="item-tech-news-8"></a>
### [HyperSAE：为稀疏自编码器引入解耦庞加莱几何，MSE 降 9.8%](https://www.reddit.com/r/MachineLearning/comments/1vlpyh2/hypersae_decoupled_poincar%C3%A9_geometry_for_sparse/) ⭐️ 7.0/10

HyperSAE 是一个新的 PyTorch 库，将解耦的庞加莱双曲几何应用于稀疏自编码器。作者在经验验证论文中报告，在 Gemma-2-2B Layer 13、20M tokens FineWeb-Edu 数据和 NVIDIA L4 GPU 上，HyperSAE 相比 FlatSAE 将重建 MSE 从 4.5724 降至 4.1232（降低 9.8%），CE Loss 恢复从 75.5% 提升至 78.9%（+3.4 个百分点），死潜变量从 3.8% 降至 0.2%（-3.6 个百分点）。架构采用解耦双速设计：前向传播完全保持欧几里得计算，因此推理零开销；仅在训练时将字典权重投影到庞加莱球内，并加入包含锥损失来组织父概念和子概念。该库提供共激活队列跟踪、TriPartite 损失（重建 + L1 稀疏 + 包含锥）和单类训练器接口，可通过 pip install hypersae 安装。MMLU-Pro 准确率从 16.11% 略升至 16.26%，GPQA Diamond 保持 100%。

reddit · r/MachineLearning · /u/visha1v · 8月11日 18:37 · [社区讨论](https://www.reddit.com/r/MachineLearning/comments/1vlpyh2/hypersae_decoupled_poincar%C3%A9_geometry_for_sparse/)

**「背景」** 标准稀疏自编码器在欧几里得空间中嵌入字典原子，体积随维度按多项式增长，而 LLM 学到的概念形成按基数扩展的分支层次结构；当字典规模达到 16K 以上时，这种不匹配会导致特征碰撞、死潜变量和重建退化。HyperSAE 在训练阶段将字典权重投影到庞加莱球，利用双曲空间中体积按指数扩展的特性，并通过包含锥损失把父概念组织在原点附近、子概念组织在边界附近，从而缓解上述问题。

**「影响」** 对于从事稀疏自编码器和机械可解释性研究的研究者，HyperSAE 提供了一个可直接安装且推理零开销的训练替代方案，在相同基准上重建误差更低、死潜变量大幅减少，但其收益仍需独立复现和更大规模验证。

**标签**: `#sparse autoencoders`, `#mechanistic interpretability`, `#hyperbolic geometry`, `#PyTorch`, `#LLM interpretability`

---

<a id="item-tech-news-9"></a>
### [Anthropic 将为 Claude 输出加入 AI 标记与 C2PA 元数据](https://support.claude.com/en/articles/16266773-how-claude-marks-ai-generated-content) ⭐️ 7.0/10

Anthropic 已签署欧盟《人工智能法案》第 50\(2\) 条关于 AI 生成内容透明度的行为准则，并宣布从 2026 年 8 月 2 日及以后在欧盟发布的新 Claude 模型起，为生成文本嵌入不可见的机器可读水印，同时在支持的文件中加入符合 C2PA 来源标准的数字签名元数据。这些标记适用于 Claude、Claude Code、Claude Cowork、Claude Tag 及 API 等产品，覆盖全球使用场景。Anthropic 正在为 2026 年 8 月 2 日前发布的旧模型补充标记功能，并计划公开检测技术细节。检测到标记只说明内容可能经 Claude 处理，未检测到标记也不能证明内容非 AI 生成。

telegram · zaihuapd · 8月11日 03:06

**「背景」** 欧盟《人工智能法案》第 50\(2\) 条要求 AI 系统提供者确保其生成的内容以机器可读格式标记为 AI 生成，主要针对文本、音频、视频等生成内容的透明度。C2PA 是一种内容来源与真实性标准，通过加密签名记录媒体文件的创建和编辑历史；机读水印则是一种人眼不可见、可由程序识别的嵌入信息。

**「影响」** 对使用 Claude API 及产品的开发者而言，后续输出中携带的 C2PA 元数据和机读水印可能影响内容存储、校验与下游处理流程；检测结果需谨慎解读，因为未检出并不等于非 AI 生成。

**标签**: `#AI transparency`, `#Anthropic`, `#Claude`, `#watermarking`, `#EU AI Act`

---

<a id="item-tech-news-10"></a>
### [石墨烯软性镜片：电控变焦的新突破](https://www.qmul.ac.uk/news/latest-news/2026/science-and-engineering/se/new-graphene-powered-soft-lens-could-pave-the-way-for-smarter-glasses-cameras-and-medical-devices.html) ⭐️ 7.0/10

伦敦玛丽女王大学 James Busfield 教授团队研发出一种基于还原氧化石墨烯的透明软性镜片原型，可通过施加小电场改变焦距，无需传统镜片所需的笨重移动部件。该成果发表于《Advanced Functional Materials》。原型模仿人眼工作原理，通电时软膜拉伸镜片改变形状，从而对不同距离的物体对焦；团队将超薄透明石墨烯电极直接集成到镜片下方的驱动层上，解决了传统电极因不透明而只能置于镜片边缘的瓶颈，大幅缩小了器件体积。研究人员表示，该技术未来可应用于自动对焦相机、可穿戴显示器、VR/AR 头显及微型医疗成像设备等领域，但目前仍需进一步优化电极透明度与性能。

telegram · zaihuapd · 8月11日 12:27

**「背景」** 传统可变焦镜头通常依靠移动光学部件来改变焦距，因此体积较大，难以满足小型化设备的需求。石墨烯电极透明且柔韧，可直接嵌入镜片区域，这一原型利用电场驱动软性镜片变形，为紧凑型自动对焦光学系统提供了新思路，同时也在电极材料制备和性能优化方面提出了新要求。

**「影响」** 该原型为微型自动对焦光学器件提供了一种无需传统移动部件的新技术路径，有望影响相机、VR/AR 头显和医疗成像设备的未来设计，但因仍处原型阶段，距商用应用尚需进一步优化电极透明度和性能。

**标签**: `#graphene`, `#optics`, `#AR/VR`, `#medical-imaging`, `#materials-science`

---

<a id="item-tech-news-11"></a>
### [Manus 与 Meta 分离，部分数据限期删除](https://manus.im/zh-tw/blog/a-note-to-our-users) ⭐️ 7.0/10

AI 助手 Manus 宣布从 Meta 剥离并恢复独立运营，作为分离过程中遵守特定司法管辖区监管要求的必要步骤。受影响用户在 2025 年 12 月 29 日（Meta 收购当日）及之后生成的数据，将于 2026 年 8 月 23 日 8:00 至 24 日（新加坡时间）被删除；用户需在 8 月 23 日 7:59 前通过备份工具导出数据，并于 8 月 25 日 8:00 起恢复访问。备份期间，受影响付费用户不会被收费，恢复访问后还将获得回归奖励。不受影响的用户可正常使用，无需任何操作。

telegram · zaihuapd · 8月11日 14:14

**「背景」** Manus 原本是一家独立 AI 初创公司，2025 年 12 月被 Meta 以约 20 亿美元收购。中国监管机构于 2026 年 4 月要求 Meta 撤销这笔交易，因此 Manus 宣布将恢复独立运营，并需在拆分过程中处理部分用户数据，包括删除特定时间后生成的数据并提供导出选项。

**「影响」** 受影响的 Manus 用户必须赶在 2026 年 8 月 23 日 7:59（新加坡时间）前导出数据，否则其在 2025 年 12 月 29 日及之后生成的数据将被删除。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/08/11/manus-china-meta-acquisition.html">Manus to return as independent company after China forced Meta to unwind $2 billion deal</a></li>
<li><a href="https://www.theinformation.com/briefings/manus-return-independent-company-meta-deal-unwinds">Manus to Return as an Independent Company as Meta Deal Unwinds — The Information</a></li>
<li><a href="https://qz.com/manus-independent-meta-acquisition-china-unwind-081126?.tsrc=rss">Manus returns to independence after China blocks Meta acquisition</a></li>

</ul>
</details>

**标签**: `#AI`, `#data governance`, `#Meta`, `#startup`, `#industry news`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [盘后大涨：超微电脑、CoreWeave、H&amp;R Block 发布超预期业绩或指引](https://www.cnbc.com/2026/08/11/stocks-making-the-biggest-moves-after-hours-smci-crwv-hrb.html) ⭐️ 8.0/10

超微电脑、CoreWeave、H&amp;R Block 等公司在盘后发布财报或业绩指引后股价大涨。超微电脑预计第一财季调整后每股收益为 1.01 至 1.10 美元，高于市场预期的 0.76 美元；CoreWeave 第二季度收入同比增长 112%至 25.8 亿美元；H&amp;R Block 预计 2027 财年调整后每股收益为 6.04 至 6.24 美元，均高于分析师预期。

rss · CNBC Finance · 8月11日 21:18

**「背景」** 这些公司大多在美股常规交易时段后公布财报或新财年业绩指引，因业绩超过分析师共识，引发盘后股价明显波动。

**标签**: `#Earnings`, `#Guidance`, `#Artificial Intelligence`, `#After-Hours Movers`, `#Super Micro Computer`

---

<a id="item-finance-news-2"></a>
### [英伟达 5000 亿美元 AI 融资计划面临中国芯片价格战风险](https://www.cnbc.com/2026/08/11/nvidia-ai-funding-jensen-huang-china-risk.html) ⭐️ 8.0/10

英伟达本周一宣布与贝莱德、黑石、阿波罗、KKR、Brookfield 和高盛等六家资产管理公司达成协议，计划筹集 5000 亿美元，用于为缺乏现金或信用评级的企业建设数据中心和 GPU 集群。分析师本·埃蒙斯指出，这一计划的关键风险是中国可能发起芯片价格战，导致 GPU 作为贷款抵押物加速贬值，使投资者面临损失。

rss · CNBC Finance · 8月11日 21:01

**「背景」** 传统资产支持融资中，银行在借款人违约时可收回并出售建筑物等实物资产，但 GPU 的可用寿命和二手市场尚不确定。目前英伟达在美国 AI 芯片市场约占 75%以上份额，H100 租金已从 2025 年末约每 GPU 小时 1.70 美元升至今年约 2.35 美元。

**「影响」** 若 GPU 贬值快于债务期限，参与这些私募贷款的投资者以及无法进入传统债务市场的高风险 AI 初创企业和“新云”公司可能首当其冲，面临抵押品价值缩水或再融资困难。

**标签**: `#Nvidia`, `#AI infrastructure`, `#financing`, `#GPU depreciation`, `#China risk`

---

<a id="item-finance-news-3"></a>
### [SK 海力士重启大连二厂建设，NAND 产能将提升约五成](https://en.sedaily.com/finance/2026/08/11/sk-hynix-to-boost-china-nand-output-50-percent-with-dalian) ⭐️ 8.0/10

SK 海力士将重启大连 NAND 闪存第二工厂的建设，当地产能将提升约 50%；新产线计划今年底开始搬入设备、明年上半年实现量产，月产能约 5 万片晶圆。公司在 AI 数据中心推动企业级 SSD 需求、NAND 价格一年涨近 10 倍的背景下，采取大连生产 100 层 NAND、清州聚焦 300 层以上产品的双轨策略。

telegram · zaihuapd · 8月11日 16:21

**「背景」** 大连二厂四年前动工后因内存行业下行长期停工；SK 海力士 2021 年完成收购英特尔 NAND 业务，旗下 Solidigm 运营大连基地。此次重启建设，目标在 2027 年上半年量产，新产线月产能约 5 万片晶圆，使当地 NAND 产能提升约 50%，但仍需继续获得美国出口管制下的设备进口许可。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.sedaily.com/finance/2026/08/11/sk-hynix-to-boost-china-nand-output-50-percent-with-dalian">SK hynix to Boost China NAND Output 50% With Dalian Plant ...</a></li>
<li><a href="https://xenospectrum.com/en/sk-hynix-dalian-v8-nand-expansion-us-export-license/">SK hynix&#x27;s Dalian Fab 2 restart plan surfaces — NAND 50,000 ...</a></li>
<li><a href="https://huggingnews.com/tech/sk-hynix-boosts-china-nand-capacity-50percent-with-dalian-fab-2-restart-775c6cbd">SK Hynix Boosts China NAND Capacity 50% With Dalian Fab 2 ...</a></li>

</ul>
</details>

**标签**: `#SK Hynix`, `#NAND`, `#capacity expansion`, `#AI datacenter`, `#memory market`

---

<a id="item-finance-news-4"></a>
### [美国选举押注禁令引发预测市场法律不确定性](https://www.cnbc.com/2026/08/11/do-state-election-betting-bans-apply-to-prediction-markets.html) ⭐️ 7.0/10

威斯康星州选务机构上月发布指引，重申根据一部逾 175 年的旧法，押注选举（包括在预测市场交易）属违法，违者可能丧失在该场选举中的投票权。全美已有 23 个州禁止选举押注，但州法是否适用于预测市场交易仍不确定。

rss · CNBC Finance · 8月11日 18:44

**「背景」** 商品期货交易委员会\(CFTC\)认为事件合约属于其监管的互换，应适用联邦法律并优先于州法；多个州则认为这是赌博并归其管辖，并援引宪法赋予州管理选举的权力。

**「影响」** 直接受影响的是 Kalshi、Polymarket 等预测市场平台及其用户；在密歇根州和内华达州，法院已迫使这些平台停止运营或限制用户访问。

**标签**: `#prediction markets`, `#election betting`, `#regulation`, `#legal uncertainty`, `#CFTC`

---

<a id="item-finance-news-5"></a>
### [Amkor 据称考虑出售中国业务股份，估值或达 15 亿美元](https://www.bloomberg.com/news/articles/2026-08-11/amkor-is-said-to-explore-stake-sale-in-1-5-billion-china-unit) ⭐️ 7.0/10

据知情人士透露，全球第二大外包半导体封装测试厂商 Amkor Technology 正考虑出售中国业务的部分股份，估值可能在 10 亿至 15 亿美元之间；公司已聘请顾问试探初步意向，但讨论尚处探索阶段，Amkor 拒绝置评。

telegram · zaihuapd · 8月11日 07:21

**「背景」** Amkor 总部位于美国亚利桑那州坦佩，2001 年在上海设立封装厂；今年 7 月刚宣布与英伟达达成 15 亿美元多年协议，共同开发下一代 AI 半导体封装技术。该公司是众多重新审视在华业务的跨国公司之一。

**标签**: `#Amkor`, `#semiconductor`, `#China`, `#M&amp;A`, `#divestiture`

---

<a id="item-finance-news-6"></a>
### [恒生科技指数拟扩容至 50 只并调整选股机制](https://www.stcn.com/article/detail/4068889.html) ⭐️ 7.0/10

恒生指数公司就修订恒生科技指数征询市场意见，拟将成分股从 30 只增至 50 只，并引入 40 只按市值、10 只按过去 12 个月收入增长选取的双组别选股机制，修订预计 2026 年 9 月底公布、12 月生效。

telegram · zaihuapd · 8月11日 09:06

**「背景」** 恒生科技指数自 2020 年推出以来，因权重集中于外卖、互联网平台类股票而被调侃为“外卖指数”，这轮调整旨在纳入先进硬件、人工智能等领域的高增长公司。

**标签**: `#Hang Seng Tech Index`, `#index reform`, `#Hong Kong market`, `#ETFs`, `#technology stocks`

---