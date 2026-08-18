---
layout: default
title: "Horizon Summary: 2026-08-18 (ZH)"
date: 2026-08-18
lang: zh
---

> 从 37 条内容中筛选出 14 条重要资讯。

---

**科技新闻**
1. [Mojo 编程语言现已开源](#item-tech-news-1) ⭐️ 8.0/10
2. [Qwen 3.8 27B 获人工智能分析指数 52 分](#item-tech-news-2) ⭐️ 8.0/10
3. [国产 AI 芯片 2026 年或占中国近九成市场，寒武纪与华为领跑](#item-tech-news-3) ⭐️ 8.0/10
4. [Turbovec：用 Rust 实现 Google TurboQuant 的向量搜索库](#item-tech-news-4) ⭐️ 7.0/10
5. [Linux 7.3 改进显存耗尽时的性能](#item-tech-news-5) ⭐️ 7.0/10
6. [实地测量：数据中心废热使下风向街区升温约 0.8°C](#item-tech-news-6) ⭐️ 7.0/10
7. [Polars 双页速查表：Python 数据分析快速参考](#item-tech-news-7) ⭐️ 7.0/10
8. [macOS 26.7 代码揭示中国大陆 Apple 智能审查机制](#item-tech-news-8) ⭐️ 7.0/10
9. [中国要求部分政府机构卸载定制版 Windows 10](#item-tech-news-9) ⭐️ 7.0/10

**财经新闻**
1. [美债收益率上行挤压普通家庭：房贷利率升至 6.75%，柴油价格同比涨 48%](#item-finance-news-1) ⭐️ 7.0/10
2. [Kalshi 申请推出股指永续合约，挑战传统交易所](#item-finance-news-2) ⭐️ 7.0/10
3. [美国“先买后付”贷款 2025 年达 1600 亿美元，覆盖水电房租](#item-finance-news-3) ⭐️ 7.0/10
4. [汇丰要求部分内地投资客户提交资金来源声明](#item-finance-news-4) ⭐️ 7.0/10
5. [苹果美国 App Store 佣金收入降 18%，二季度用户消费额同比降 6%](#item-finance-news-5) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Mojo 编程语言现已开源](https://simonwillison.net/2026/Aug/18/mojo-is-now-open-source/) ⭐️ 8.0/10

Mojo 编程语言在发布 1.0 一周后，正式将其编译器与工具链以 Apache 2 许可证开源。这一动作兑现了自 2023 年 5 月以来多次承诺的开源计划。Mojo 不再追求成为 Python 的完整超集，而是发展为一种语法受 Python 启发、针对 GPU 编程优化的独立语言。开源后，开发者可以自由查看、修改和分发其编译器与工具链，这对 AI/ML 编程语言生态具有重要影响。

rss · Simon Willison · 8月18日 21:39

**「背景」** Mojo 于 2023 年推出时，最初目标是成为 Python 的超集，从而借助现有 Python 代码启动自己的生态。但在 2025 年 8 月左右，官方调整了路线图，承认 Mojo 不一定会完全兼容 Python，而是强调在 Python 风格语法基础上优化 GPU 编程。如今的开源版本标志着这一独立语言路线的正式落地。

**「影响」** 开发者现在可以在 Apache 2 许可下使用、修改和重新分发 Mojo 的编译器与工具链，这为 AI/ML 编程语言生态带来更开放的底层基础设施。

**标签**: `#mojo`, `#open-source`, `#programming-language`, `#ai`, `#compiler`

---

<a id="item-tech-news-2"></a>
### [Qwen 3.8 27B 获人工智能分析指数 52 分](https://simonwillison.net/2026/Aug/17/qwen-38-27b-scores-52/) ⭐️ 8.0/10

Qwen 3.8 27B 在人工智能分析指数（Artificial Analysis Intelligence Index）上取得 52 分，与 GPT-5.6 Luna（max 配置）持平，仅比 GLM-5.2（max）和 DeepSeek V4 Pro 0813（max）低 1 分。这些对比模型的规模远大于 27B：GLM-5.2 为 753B 参数，DeepSeek V4 Pro 0813 为 1.7T 参数，而 Luna 的规模未公布，但大概率也远大于 27B。Simon Willison 报道了这一结果并称 Qwen 3.8 27B 是“真正令人惊叹的模型”，认为这是效率上的重要里程碑。

rss · Simon Willison · 8月17日 23:58

**「背景」** Artificial Analysis Intelligence Index 是一个由 Artificial Analysis 发布的大语言模型综合智能评分基准，用于横向比较不同模型的推理与综合能力。Qwen 3.8 27B 是通义千问系列的开源权重模型，参数量约 270 亿；在该指数中，同类规模开源模型的中位得分仅为 9 分，因此 52 分属于显著的效率跨越。

**「影响」** 对于计算资源有限的开发者和组织，27B 参数模型现在可以在该指数上与规模大得多的模型竞争，可能大幅降低高性能 AI 部署的基础设施和成本门槛。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://artificialanalysis.ai/models/qwen3-8-27b">Qwen3.8 27B - Intelligence, Performance &amp; Price Analysis</a></li>

</ul>
</details>

**标签**: `#qwen`, `#artificial-analysis`, `#llms`, `#benchmarks`, `#ai`

---

<a id="item-tech-news-3"></a>
### [国产 AI 芯片 2026 年或占中国近九成市场，寒武纪与华为领跑](https://www.tomshardware.com/tech-industry/artificial-intelligence/chinas-homegrown-ai-accelerators-to-supply-90-percent-of-the-countrys-domestic-market-analysts-suggest-cambricon-and-huawei-expected-to-be-the-biggest-winners-in-the-shift-away-from-nvidia-and-amd) ⭐️ 8.0/10

TrendForce 预计，到 2026 年中国本土 AI 加速器将供应国内市场近 90%，较 2025 年的 45% 大幅提升，寒武纪与华为被视为最大受益者。数据显示，2025 年英伟达以 220 万颗占 55% 市场份额，华为出货 81.2 万颗占 20.3%。中国需要将高端 AI 芯片年产量提升约 2.2 倍至约 196 万颗，产能能否跟上仍是关键疑问。该预测由 TrendForce 给出，并经由 Tom&\#x27;s Hardware 报道。

telegram · zaihuapd · 8月18日 13:03

**「背景」** 中国科技产业正加速推动 AI 芯片自主化，以减少对英伟达、AMD 等外国供应商的依赖。美国出口管制促使华为、寒武纪等本土厂商扩大 AI 加速器出货，并推动国内供应链建设。

**「影响」** 若预测成真，英伟达在中国 AI 加速器市场的份额将从 2025 年的 55% 大幅下滑，华为和寒武纪将获得主导地位；但 196 万颗高端 AI 芯片的产量目标对国内产能构成严峻考验。

**标签**: `#AI accelerators`, `#China semiconductor`, `#Huawei`, `#Cambricon`, `#AI hardware`

---

<a id="item-tech-news-4"></a>
### [Turbovec：用 Rust 实现 Google TurboQuant 的向量搜索库](https://github.com/RyanCodrai/turbovec) ⭐️ 7.0/10

Turbovec 是一个用 Rust 实现的向量搜索库，基于 Google 提出的 TurboQuant 量化技术。项目托管在 GitHub（RyanCodrai/turbovec），目标是通过更高效的内存使用和检索速度，支持本地、隐私优先的搜索应用。该库尚处于早期阶段，README 主要介绍其设计方向；社区评论中提到了千万级文档约 4GB 内存占用的说法，以及未来可能提供的 SQLite 绑定。作为对 FAISS 等现有工具的替代或补充，它值得关注，但尚无官方基准测试或正式发布版本可供验证。

hackernews · fittingopposite · 8月18日 18:07 · [社区讨论](https://news.ycombinator.com/item?id=49349898)

**「背景」** Google TurboQuant 是一种面向向量搜索引擎的量化技术，旨在以极低内存占用和近零预处理时间构建与查询大规模向量索引，同时保持较高的搜索准确率。其核心思路是先对向量进行归一化，再施加随机旋转，从而与传统的量化方法（如乘积量化）形成区别，使压缩后的向量仍能有效支持语义搜索。Turbovec 则是这一技术在 Rust 语言中的实现，目标是让本地化、隐私优先的向量搜索应用受益。

**「社区讨论」** 评论者对内存效率和开发体验表示期待，认为这能加快反向索引和调试/性能测试，并有人询问是否已尝试编译为 WASM 以在浏览器扩展中运行。也有人提出与 Qdrant 的比较，认为 Qdrant 已在数月前集成 TurboQuant 并运行良好；同时有反馈希望 README 更面向人类读者，另有人指出 FAISS 已不再是 SoTA 并附上基准链接。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://research.google/blog/turboquant-redefining-ai-efficiency-with-extreme-compression/">TurboQuant : Redefining AI efficiency with extreme compression</a></li>
<li><a href="https://medium.com/data-science-in-your-pocket/turbovec-googles-turboquant-makes-vector-search-smaller-faster-and-simpler-fdea72674aad">turbovec : Google ’s TurboQuant Makes Vector Search ... | Medium</a></li>

</ul>
</details>

**标签**: `#rust`, `#vector-search`, `#quantization`, `#ai`, `#library`

---

<a id="item-tech-news-5"></a>
### [Linux 7.3 改进显存耗尽时的性能](https://pixelcluster.dev/VRAM-Overcommit/) ⭐️ 7.0/10

这篇文章讨论了 Linux 7.3 在显存（VRAM）耗尽时带来的性能改进，重点提出了 VRAM overcommit 以及由应用告知内核显存“粘性”需求的思路。作者认为，相比内核的猜测式分配，应用自身更清楚哪些数据应该留在显存中，这也是文章的核心论点。不过，该文章带有推测性质，目前缺乏完整可验证的实现细节和测试数据，实际效果仍需等待上游合入后再确认。此外，社区讨论也提出了系统内存耗尽时系统卡死、NVIDIA 驱动不支持显存分页等现实挑战。

hackernews · flaburgan · 8月18日 07:51 · [社区讨论](https://news.ycombinator.com/item?id=49342719)

**「背景」** VRAM（显存）是 GPU 上的专用内存，容量有限；当游戏或应用申请的显存超过物理 VRAM 时，就需要依赖内核与驱动进行换页或驱逐来“超额使用”（overcommit），处理不当会导致性能骤降或崩溃。本文作者此前提交的改进内核显存管理的补丁已被上游合并并排入 Linux 7.3，相关代码已经开始在 SteamOS 内核的稳定版和预览版中提供。该系列工作属于 Linux 7.3 的初始显存管理改进，后续更进一步的优化仍在为未来主线上游版本开发。

**「影响」** Linux 7.3 的 VRAM 过量分配改进主要惠及 AMD GPU 用户，可在显存耗尽时减少性能下降；而 Nvidia 用户仍受限于 Nvidia 驱动不支持显存分页，难以获得同等的改进效果。

**「社区讨论」** 评论者普遍对改进表示期待，并希望相关功能尽早进入主线内核，但也有人指出，在 NVIDIA 驱动上仍然无法使用显存分页，限制了实际收益。另有用户结合亲身经历对比了 Linux 与 Windows 在内存耗尽时的表现，并赞同应用进程比内核更清楚显存分配“粘性”的观点。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.phoronix.com/news/Linux-7.3-Improving-vRAM-Mgmt">Linux 7.3 To Land Initial Code Improving vRAM Management, More Improvements Coming - Phoronix</a></li>
<li><a href="https://pixelcluster.dev/VRAM-Overcommit/">VRAM Management Part 2: Beyond the Limits of Physical VRAM | pixelcluster&#x27;s GPU blog</a></li>
<li><a href="https://news.ycombinator.com/item?id=49342719">Linux 7.3 improves performance when running out of vRAM</a></li>

</ul>
</details>

**标签**: `#linux`, `#vram`, `#memory-management`, `#gpu`, `#kernel`

---

<a id="item-tech-news-6"></a>
### [实地测量：数据中心废热使下风向街区升温约 0.8°C](https://asmedigitalcollection.asme.org/sustainablebuildings/article/7/2/024501/1233035/Data-Center-Waste-Heat-as-an-Emerging-Urban) ⭐️ 7.0/10

一项实地研究量化了数据中心废热对城市局部气温的影响：在凤凰城，数据中心下风向约 500 米范围内的街区平均气温升高约 0.8°C，上风向约 42.7°C 升至下风向 43.5°C。研究强调数据中心废热是新兴的城市热源，但影响范围有限。该证据对数据中心选址、城市规划和热缓解策略具有参考意义。

hackernews · cwwc · 8月18日 17:24 · [社区讨论](https://news.ycombinator.com/item?id=49349147)

**「背景」** 数据中心运行时会产生大量废热，有报道称单座数据中心产生的废热可超过 4 万个美国家庭；近期亚利桑那州立大学在凤凰城都市区的研究显示，数据中心废热可使下风方向邻近社区气温最多升高约 4 华氏度（约 2 摄氏度），而本项 ASME 论文则是在该背景下对邻近街区尺度进行的实地测量。此类测量有助于评估数据中心作为城市新兴热源对局部气候的实际影响。

**「影响」** 对凤凰城等干旱城市中数据中心周边居民和规划者而言，这一测量结果提供了具体的局部升温数据，显示影响约为 0.8°C 而非更大；有助于基于证据评估数据中心热影响，避免夸大或忽视。

**「社区讨论」** 社区评论中有人质疑“数据中心恐慌”是否被夸大，并指出实测平均ΔT 约 0.8°C，远小于标题暗示的幅度；也有人感叹讨论难以客观进行，并呼吁对炼油厂等同类热源给予同等关注。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.rediff.com/news/report/data-centers-heat-impact-on-downwind-localities/20260519.htm">Data Centre Waste Heat : Impact On Neighbourhood Temperatures</a></li>
<li><a href="https://techxplore.com/news/2026-05-centers-nearby-temperatures-degrees-phoenix.html">Data centers raise nearby temperatures by up to 4 degrees in Phoenix</a></li>
<li><a href="https://gizmodo.com/data-centers-can-make-neighborhoods-up-to-4-degrees-hotter-study-finds-2000761977">Data Centers Can Make Neighborhoods Up to 4 Degrees Hotter...</a></li>

</ul>
</details>

**标签**: `#data centers`, `#environmental impact`, `#urban heat`, `#sustainability`, `#field measurements`

---

<a id="item-tech-news-7"></a>
### [Polars 双页速查表：Python 数据分析快速参考](https://opensource.posit.co/resources/cheatsheets/polars/) ⭐️ 7.0/10

该速查表由《Python Polars: The Definitive Guide》（近 500 页）压缩为两页，提供 PDF 和可访问的 HTML 版本。它覆盖常见 DataFrame 操作，方便 Polars 用户快速查找列选择、变换、聚合等常用语法。作为基于 O&\#x27;Reilly 权威书籍的实用参考，它降低了 Pandas 用户转向 Polars 时的学习成本，也与社区中关于 Polars 相对 pandas 更顺手的讨论相呼应。项目作者邀请读者反馈遗漏操作或排版建议，说明该资源仍在迭代完善。

hackernews · jeroenjanssens · 8月18日 13:38 · [社区讨论](https://news.ycombinator.com/item?id=49345476)

**「背景」** Polars 是一个面向 Python 和 Rust 的高性能 DataFrame 库，以惰性求值和并行处理为特色，常被视为 Pandas 的替代方案。这份速查表基于 Jeroen Janssens 与 Thijs Nieuwdorp 合著的 O&\#x27;Reilly 图书《Python Polars: The Definitive Guide》，将书中近 500 页内容压缩为两页，提供 PDF 及可访问的 HTML 版本，涵盖常见 DataFrame 操作。

**「影响」** 对使用 Polars 的 Python 数据分析师而言，这是一份免费、可直接收藏的权威双页参考，并因提供 HTML 版本而便于屏幕阅读器使用。

**「社区讨论」** 评论者普遍认可 Polars 改善了 pandas 的挫败感，但有人怀念 R 的 dplyr/tidyverse 或 data.table 体验，也有人对每次写 pl.col\(&quot;...&quot;\) 的冗长表示不适，还有人表示已转向 DuckDB。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://opensource.posit.co/resources/cheatsheets/polars/">Python Polars: The Definitive Cheatsheet :: Posit Open Source</a></li>

</ul>
</details>

**标签**: `#polars`, `#python`, `#dataframes`, `#cheatsheet`, `#data-analysis`

---

<a id="item-tech-news-8"></a>
### [macOS 26.7 代码揭示中国大陆 Apple 智能审查机制](https://www.macrumors.com/2026/08/17/macos-26-7-unreleased-apple-devices/) ⭐️ 7.0/10

据 MacRumors 报道，macOS 26.7 等系统代码显示，苹果的“写作工具”将登陆中国大陆，并为该地区引入独立的内容安全过滤与处罚机制。代码片段提到，用户需先完成“内容安全更新”才能使用写作工具；若多次触发安全警报，工具将暂时受限。对无法用 Apple 智能编辑的文本，系统会显示提示，或建议将文本发送给其他处理方。相关安全审查规则据称可通过云控远程下发。目前该功能尚未正式发布，具体规则与实施时间仍存在不确定性。

telegram · zaihuapd · 8月18日 02:16

**「背景」** Apple 智能（Apple Intelligence）是苹果的 AI 功能套件，其中的“写作工具”可在系统内进行文本改写、摘录等操作；由于中国大陆的内容监管要求，苹果一直未在当地正式提供完整服务。MacRumors 报道称，今日推送的 macOS Tahoe 26.7 候选版代码中出现了面向中国大陆的“写作工具”引用，并包含内容安全提示与触发警报后的限制字符串，显示该版本可能为本地合规审核机制预留接口。

**「影响」** 对中国大陆用户而言，Apple 智能写作工具一旦启用，将内置内容安全过滤与处罚机制，多次触发安全警报会导致该功能被暂时限制，且相关安全审查规则可经云端远程下发、动态调整；Apple 官方支持页面也显示，已购买的支持 Apple Intelligence 的设备届时可在该地区激活使用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.macrumors.com/2026/08/17/macos-26-7-unreleased-apple-devices/">macOS Tahoe 26 . 7 is Full of References to Unreleased... - MacRumors</a></li>
<li><a href="https://support.apple.com/en-us/121115">How to get Apple Intelligence - Apple Support</a></li>

</ul>
</details>

**标签**: `#Apple`, `#AI censorship`, `#content moderation`, `#macOS`

---

<a id="item-tech-news-9"></a>
### [中国要求部分政府机构卸载定制版 Windows 10](https://www.bloomberg.com/news/articles/2026-08-18/china-axing-microsoft-windows-from-state-agencies-ahead-of-plan) ⭐️ 7.0/10

据彭博社报道，中国国家安全部已要求部分政府相关机构卸载定制版 Windows 10，令原定于 2027 年 2 月执行的停用计划提前数月。知情人士称，该指令源于数据安全担忧，但未披露具体漏洞细节。微软回应称，未发现影响该产品的安全事件，该产品目前仍在定期获得安全更新。这一提前行动可能反映中国政府加速减少对特定操作系统依赖的意图。

telegram · zaihuapd · 8月18日 06:22

**「背景」** 微软曾为中国政府专门推出定制版 Windows 10，即“Windows 10 中国政府版”，它基于 Windows 10 企业版进行了本地化修改，以符合中国政府部门的使用要求。该版本是在微软 CEO 萨蒂亚·纳德拉与中国财政官员谈判后推出的。此次中国国家安全部要求部分政府机构卸载该定制版系统，是出于数据安全担忧，并意味着原定于 2027 年 2 月的停用计划被提前了数月。

**「影响」** 受影响的政府相关机构被要求提前卸载定制的 Windows 10 政府版，原定 2027 年 2 月的停用计划因此提前数月；消息人士称这一指令源于数据安全担忧，但未说明具体漏洞。这一举措可能使微软在中国政府市场的业务面临更大压力。不过微软表示，未发现影响该产品的安全事件，且该产品仍在定期获得安全更新。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bloomberg.com/news/articles/2026-08-18/china-axing-microsoft-windows-from-state-agencies-ahead-of-plan">China Removes Microsoft Windows at State Users Ahead of Plan</a></li>
<li><a href="https://www.techspot.com/news/113529-china-finally-pulling-windows-10-government-machines-ahead.html">China pulls the plug on Windows 10 for government ... | TechSpot</a></li>
<li><a href="https://www.tomshardware.com/software/operating-systems/china-reportedly-orders-state-agencies-to-uninstall-its-government-only-edition-of-windows-10">China reportedly orders state agencies to uninstall its government-only edition of Windows 10 — Beijing accelerates planned retirement over data security concerns | Tom&#x27;s Hardware</a></li>
<li><a href="https://www.tradingkey.com/analysis/stocks/us-stocks/262114664-win10-government-removal-microsoft-china-headwinds-tradingkey">Win10 Government Edition Phased Out Early as Microsoft&#x27;s China Business Faces New Headwinds</a></li>
<li><a href="https://seekingalpha.com/news/4634187-microsoft-windows-older-version-being-removed-at-china-state-linked-entities-ahead-of-plan">Microsoft Windows old version being sunset in China state-linked firms | Seeking Alpha</a></li>

</ul>
</details>

**标签**: `#Windows 10`, `#China`, `#government policy`, `#data security`, `#Microsoft`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [美债收益率上行挤压普通家庭：房贷利率升至 6.75%，柴油价格同比涨 48%](https://www.cnbc.com/2026/08/18/bond-market-treasury-yields-warsh-main-street.html) ⭐️ 7.0/10

美国国债市场近期遭抛售，长期收益率上升，10 年期美债收益率已突破 4.7%。这已推高普通家庭的关键成本：30 年期房贷利率升至 6.75%，柴油价格同比上涨 48%至每加仑 5.46 美元。

rss · CNBC Finance · 8月18日 16:48

**「背景」** 收益率曲线趋陡主要因长期端推动；伊朗战争、科技公司为 AI 基础设施大量发债，以及美国本财年预计约 2.1 万亿美元（约占 GDP 的 6.4%）的财政赤字，都加剧了市场对长期发债和通胀的担忧。

**「影响」** 房贷和柴油成本上升将直接影响购房家庭以及运输、物流、农业等用油行业；在长期收益率回落前，这些压力可能持续。

**标签**: `#bond yields`, `#Treasury market`, `#consumer debt`, `#fiscal policy`, `#inflation`

---

<a id="item-finance-news-2"></a>
### [Kalshi 申请推出股指永续合约，挑战传统交易所](https://www.cnbc.com/2026/08/18/kalshi-wants-to-launch-perps-tied-to-equity-indexes.html) ⭐️ 7.0/10

Kalshi 周二向美国商品期货交易委员会（CFTC）提交申请，计划推出追踪股票指数的永续合约（perps），其中包括挂钩 MerQube 美国大盘股指数的“US500”产品。该申请尚待批准，是 Kalshi 从预测市场向多资产交易所扩张的最新一步。

rss · CNBC Finance · 8月18日 16:49

**「背景」** 永续合约没有到期日，交易者无需持有标的资产，合约通过资金费率保持与市场价格同步。Kalshi 于 5 月底刚获准推出加密货币永续合约；该公司称这类合约 2025 年全球成交额超过 90 万亿美元，而其自身产品上线一周内名义成交额突破 10 亿美元。此前 CME 已就 CFTC 批准国内永续合约提起诉讼。

**标签**: `#Kalshi`, `#perpetual futures`, `#CFTC`, `#equity indexes`, `#exchange competition`

---

<a id="item-finance-news-3"></a>
### [美国“先买后付”贷款 2025 年达 1600 亿美元，覆盖水电房租](https://www.nytimes.com/2026/08/17/business/buy-now-pay-later.html) ⭐️ 7.0/10

美国消费者 2025 年通过“先买后付”贷款借入 1600 亿美元，较 2023 年接近翻倍；这类贷款已从网购扩展到水电、房租、医疗等日常支出。LendingTree 调查显示，半数用户表示没有此类贷款就难以维持收支，四分之一曾同时背负至少 3 笔贷款。

telegram · zaihuapd · 8月18日 01:41

**「背景」** “先买后付”是一种让消费者先取走商品或服务、后续分期还款的贷款方式。美国联邦储备委员会估计，2025 年这类贷款发放额约 1600 亿美元，其中约一半为常见的四期分期（pay in 4）计划。

**「影响」** 依赖“先买后付”支付水电和房租的家庭，在还款失败时容易因自动扣款产生透支费，且因多数贷款未上报征信，银行和监管者难以察觉其债务风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.federalreserve.gov/econres/notes/feds-notes/buy-now-pay-later-beyond-pay-in-4-a-comprehensive-product-overview-20260605.html">The Fed - “Buy Now, Pay Later” Beyond “Pay in 4”, A Comprehensive Product Overview</a></li>

</ul>
</details>

**标签**: `#buy-now-pay-later`, `#consumer-credit`, `#household-debt`, `#fintech`, `#financial-regulation`

---

<a id="item-finance-news-4"></a>
### [汇丰要求部分内地投资客户提交资金来源声明](https://36kr.com/newsflashes/3944605562797192) ⭐️ 7.0/10

据 36 氪报道，汇丰香港要求部分内地存量投资客户于 9 月 12 日前通过 App 提交《开立/维持账户之声明书》并更新联系信息，确认投资资金来自中国内地以外的合法来源；若 8 月 20 日前未提交，投资相关服务可能被暂停，若 9 月 12 日前仍未提交，相关服务可能被终止。

telegram · zaihuapd · 8月18日 07:30

**「背景」** 汇丰香港要求部分内地投资客户提交资金来源声明，是银行在反洗钱和“了解你的客户（KYC）”监管要求下进行的客户尽职调查，目的是确认资金合法来源并更新客户资料。此类要求通常只适用于投资服务客户，不涉及一般银行服务。

**「影响」** 未按时完成声明的内地投资客户，其汇丰香港投资相关服务可能被暂停甚至终止。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.163.com/dy/article/L4KAO89P0512B07B.html">163.com/dy/article/L4KAO89P0512B07B.html</a></li>
<li><a href="https://m.nbd.com.cn/articles/2026-08-18/4545030.html">m.nbd.com.cn/articles/2026-08-18/4545030.html</a></li>
<li><a href="https://cj.sina.com.cn/articles/view/1649173367/m624c637703301ijyq?finpagefr=p_104">cj.sina.com.cn/articles/view/1649173367/m624c637703301ijyq?...</a></li>

</ul>
</details>

**标签**: `#HSBC`, `#compliance`, `#KYC`, `#cross-border investment`, `#regulatory`

---

<a id="item-finance-news-5"></a>
### [苹果美国 App Store 佣金收入降 18%，二季度用户消费额同比降 6%](https://www.macrumors.com/2026/08/18/apple-app-store-revenue-falling/) ⭐️ 7.0/10

苹果美国 App Store 佣金收入自 2026 年初以来下降 18%；Sensor Tower 估计美国用户第二季度 App Store 消费额同比下降 6%，而去年同期增长 9%。

telegram · zaihuapd · 8月18日 12:17

**「背景」** 佣金收入指苹果对应用内数字交易抽取的分成；报道称多国近期实施的监管新规是收入下滑的大背景。

**「影响」** 苹果称监管变化已拖累服务业务增长，意味着 App Store 收入下滑正在影响其服务板块表现。

**标签**: `#Apple`, `#App Store`, `#regulatory impact`, `#services revenue`, `#consumer spending`

---