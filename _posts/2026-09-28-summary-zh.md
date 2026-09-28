---
layout: default
title: "Horizon Summary: 2026-09-28 (ZH)"
date: 2026-09-28
lang: zh
---

> 从 24 条内容中筛选出 7 条重要资讯。

---

**科技新闻**
1. [无法解释的软件故障正在被正常化](#item-tech-news-1) ⭐️ 7.0/10
2. [Simon Willison 回顾 2026 年 LLM 发展主题演讲](#item-tech-news-2) ⭐️ 7.0/10
3. [开源确定性《皇室战争》模拟器与强化学习实验](#item-tech-news-3) ⭐️ 7.0/10
4. [用强化学习训练双智能体格斗：奖励劫持与联赛训练](#item-tech-news-4) ⭐️ 7.0/10
5. [中国发布“太空之弦”计算星座计划](#item-tech-news-5) ⭐️ 7.0/10
6. [中国数据中心超 24GW，大厂资本开支激增](#item-tech-news-6) ⭐️ 7.0/10

**财经新闻**
1. [美国国债收益率飙升，推高 AI 与数据中心企业的借债成本](#item-finance-news-1) ⭐️ 8.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [无法解释的软件故障正在被正常化](https://www.ihatethefuture.com/2026/09/the-normalization-of-inexplicable.html) ⭐️ 7.0/10

一篇题为《The Normalization of Inexplicable Failures》的文章认为，软件故障正在被正常化，尤其是随着 AI 辅助开发普及，不可预测的缺陷变得更加常见。该文在 Hacker News 上引发广泛讨论，反映出工程社区对可靠性和可复现性的担忧。评论者围绕 agent/LLM 驱动开发的“够用就好”心态、故障责任归属，以及库、基础设施和编译器是否也会被这种心态侵蚀展开争论。由于原文未提供完整技术细节，目前只能确认这是一篇观点与分析文章，而非具体技术突破、版本发布或原创研究。

hackernews · pxx · 9月27日 15:26 · [社区讨论](https://news.ycombinator.com/item?id=49867486)

**「背景」** 这篇文章所讨论的“不可解释故障的常态化”，指的是当失败原因变得难以追溯时，工程师与用户逐渐不再追问原因，而把它当作可接受的常态。相关的工具结果指出，这一担忧的背景是 AI 辅助与智能体驱动开发的普及：模型可能节省开发时间，却无法免除理解任务本身的需要，团队因此可能推迟测试套件、靠用户反馈发现问题，并在下游代码出错时以“模型不确定性”为由免责。与此同时，已有研究把关注点从 AI 的“能力风险”转向组织层面，认为构建这些系统的机构本身可能倾向于逐渐滑向失败。

**「影响」** 对依赖第三方库、基础设施与编译器的开发者而言，一旦不可解释的失败被当作常态，缺陷责任将变得模糊，排查与修复成本被转嫁给下游，讨论者担心这会拖慢整个生态——社区评论中以汽车故障“它有时就这样”的遭遇作为这种体验的类比，也有人把不稳定测试的排查流程整理成应对指南。需要说明的是，这些判断来自社区经验与观点，原文并未提供可量化的数据支持。

**「社区讨论」** 评论并未形成一致结论：pmarreck 表示自己坚持可复现性、确定性和测试，同时仍使用 agent 辅助开发，但强调必须配套严格检查；adamddev1 则担心“够用就好”的心态若蔓延到库、基础设施和编译器，会拖慢整个生态。theamk 和 layer8 把无法解释的故障与责任缺失、用户对故障的无力感联系起来，WorldMaker 还质疑“置信分数”被赋予拟人化含义。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ihatethefuture.com/2026/09/the-normalization-of-inexplicable.html">i hate the future: the normalization of inexplicable failures</a></li>
<li><a href="https://news.lavx.hu/article/i-hate-the-future-the-normalization-of-inexplicable-failures">i hate the future: the normalization of inexplicable failures</a></li>
<li><a href="https://arxiv.org/abs/2609.05749">[2609.05749] The Normalization of Deviance in AI Development</a></li>
<li><a href="https://news.ycombinator.com/item?id=49868291">The &quot; normalization of inexplicability&quot; is indeed... | Hacker News</a></li>
<li><a href="https://gist.github.com/andywang0191-stack/acf839c646eb9ba97a4abd8250132075">Flaky Tests Are Not Bad Luck: A Practical Playbook for Hunting...</a></li>
<li><a href="https://viblo.asia/p/flaky-tests-are-not-bad-luck-a-practical-playbook-for-hunting-inexplicable-failures-pPLkNbE6JRZ">Flaky Tests Are Not Bad Luck: A Practical Playbook for Hunting...</a></li>

</ul>
</details>

**标签**: `#software reliability`, `#AI-assisted development`, `#LLM coding agents`, `#testing and reproducibility`, `#software engineering culture`

---

<a id="item-tech-news-2"></a>
### [Simon Willison 回顾 2026 年 LLM 发展主题演讲](https://simonwillison.net/2026/Sep/27/2026-in-llms-so-far/) ⭐️ 7.0/10

Simon Willison 于 2026 年 9 月 25 日在圣何塞举行的 WeAreDevelopers World Congress North America 上发表闭幕主题演讲，按时间顺序回顾 2026 年迄今的大语言模型进展，并于 9 月 27 日发布配套的注释幻灯片与讲稿，视频已上传 YouTube。他把 2026 年的起点定在 2025 年 11 月，认为 Claude Opus 4.5 与 GPT-5.1 虽属渐进式改进，却让各自的编码智能体（Claude Code 自 2025 年 2 月起、Codex 稍晚）从“经常出错”跨越到“足以日常使用”。他沿用“生成骑自行车鹈鹕 SVG”这一自嘲为“世上最蠢”的基准展示当时模型的不足，并提到 2025 年 11 月 24 日 GitHub 仓库 steipete/Warelay 的首次提交，称稍后会再回到这个仓库。他还列出 2026 年预测，包括 LLM 写出好代码将变得无可否认、沙箱问题终将解决、编码智能体安全可能发生“挑战者号式”事故，以及教皇将就 LLM 及其经济影响表态。所给节选仅覆盖演讲开头部分，正文在提及 Oxide and Friends 播客处即被截断，后续详细技术内容未在摘录中呈现。

rss · Simon Willison · 9月27日 23:54

**「背景」** Simon Willison 是长期跟踪大语言模型发展的软件开发者与博客作者，习惯用诸如「生成一只骑自行车的鹈鹕 SVG」这类非正式测试来观察新模型的能力边界。2026 年 9 月 23 至 25 日，WeAreDevelopers World Congress North America 在圣何塞举行，他在大会闭幕主题演讲中按时间顺序梳理了 2026 年 LLM 领域的关键进展。这篇博文正是该演讲的幻灯片与注释整理稿，其叙述起点被作者定在 2025 年 11 月——Claude Opus 4.5 与 GPT-5.1 发布，使配套的编码代理从「经常出错」变为「可靠到可以日常使用」。

**「影响」** 对开发者而言，这场回顾把 2026 年定位为编码智能体由实验性工具转向日常可用工具的转折点，并据此主张应更大胆地承接新项目；但该判断主要基于演讲者的个人使用经验，节选也未提供基准分数等量化证据，实际效果仍有待更长周期的验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/">Simon Willison’s Weblog</a></li>
<li><a href="https://www.wearedevelopers.com/world-congress-north-america/speakers">Speakers · WeAreDevelopers World Congress · 23–25 Sep 2026 · San José, CA · North America</a></li>
<li><a href="https://www.wearedevelopers.com/world-congress-north-america/agenda">Agenda · WeAreDevelopers World Congress · 23–25 Sep 2026 · San José, CA · North America</a></li>

</ul>
</details>

**标签**: `#Large Language Models`, `#AI trends`, `#conference talk`, `#software engineering`, `#2026 retrospective`

---

<a id="item-tech-news-3"></a>
### [开源确定性《皇室战争》模拟器与强化学习实验](https://www.reddit.com/r/MachineLearning/comments/1wrj0t3/clashroyaleai_an_opensource_deterministic_clash/) ⭐️ 7.0/10

开源项目 ClashRoyaleAi 发布了一个确定性的《皇室战争》模拟器，供强化学习智能体学习该游戏，由 /u/Potential-Barber8658 与 Ambash 开发（后者负责大部分卡牌名单）。引擎为 C++ 并带 Python 绑定，单个笔记本核心上约 10 毫秒可跑完整局，任意状态可在微秒级分叉，使前瞻搜索成本很低；作为对手的启发式机器人每秒会把候选操作在引擎中向前模拟 10 秒来打分。目前最佳结果是简单 1-ply 前瞻将策略对启发式机器人的胜率从 0.625 提升到 0.944（160 场配对对局），但把该策略蒸馏回网络的专家迭代尝试只保留了 +0.045。作者还报告了 PPO 的奖励劫持失败案例：智能体学会把加农炮停在自己国王塔后面，因为战斗中损失建筑会扣奖励，而让其自然衰减则没有代价。作者强调智能体目前还不强，自己并非强化学习领域专家，欢迎更熟悉该领域的人反馈；仓库地址为 https://github.com/itzik123/ClashRoyaleAi，开发过程中使用了 AI 编程工具作为结对编程助手。

reddit · r/MachineLearning · /u/Potential-Barber8658 · 9月27日 12:30

**「背景」** 《皇室战争》（Clash Royale）是一款实时对战的卡牌策略游戏，双方在共享战场上按圣水费用出牌、争夺塔防目标，出牌时机与位置选择都很关键，因此适合作为强化学习环境。PPO（近端策略优化）是常用的策略梯度算法，前瞻搜索（lookahead search）则通过前向模拟评估候选动作，而把搜索结果蒸馏回策略网络是常见的做法。据项目仓库描述，ClashRoyaleAi 是一套用 C++ 编写的确定性战斗模拟器，带 Python 绑定，包含循环 PPO 智能体、前瞻搜索，以及连接真实游戏的计算机视觉桥接。

**「影响」** 对强化学习研究者和开发者而言，该项目的价值主要在于工程效率：C++ 引擎加 Python 绑定可在单核约 10 毫秒完成整局、以微秒级分叉任意游戏状态，使 1-ply 前瞻搜索成为低成本实验手段，并把对抗启发式机器人的胜率从 0.625 提升到 0.944（160 场配对）。不过作者明确表示智能体目前并不强，前瞻结果蒸馏回网络仅保留 +0.045 的增益，且同类开源游戏模拟器（如 crforge、ClashAI）已经存在，因此它更像是可复用的实验工具而非可直接依赖的强基准。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/itzik123/ClashRoyaleAi">GitHub - itzik123/ClashRoyaleAi: A fast, deterministic Clash ...</a></li>
<li><a href="https://github.com/itzik123/ClashRoyaleAi/blob/main/README.md">ClashRoyaleAi/README.md at main · itzik123 ... - GitHub</a></li>
<li><a href="https://github.com/itzik123/ClashRoyaleAi">GitHub - itzik123/ClashRoyaleAi: A fast, deterministic Clash ...</a></li>
<li><a href="https://github.com/voonhous/crforge">GitHub - voonhous/crforge: Headless Clash Royale battle ...</a></li>
<li><a href="https://github.com/vegetableleaf/ClashAI">GitHub - vegetableleaf/ClashAI: An AI DL model that learns ...</a></li>

</ul>
</details>

**标签**: `#reinforcement-learning`, `#open-source`, `#game-simulation`, `#PPO`, `#lookahead-search`

---

<a id="item-tech-news-4"></a>
### [用强化学习训练双智能体格斗：奖励劫持与联赛训练](https://www.reddit.com/r/MachineLearning/comments/1wr99bn/teaching_neural_nets_to_fight_with_rl_p/) ⭐️ 7.0/10

这是一个个人强化学习项目，作者训练两个神经网络智能体在一个类《街头霸王》的格斗游戏中互相对战，原本想观察是否会出现有趣的涌现行为。作者表示，事后看来或许显而易见，但智能体非常擅长奖励劫持（reward hacking），以至于必须对奖励进行一定程度的塑造（reward shaping），才能让它们愿意靠近彼此。此后作者引入联赛式训练（league play）进一步改进智能体；他指出，如果没有联赛训练，智能体学不到通用策略，只会学会如何针对某个特定对手进行利用。作者在博客文章 https://blog.lukesalamone.com/posts/fighting-game-rl 中记录了完整过程，并提供了可亲自与主智能体对战的演示。

reddit · r/MachineLearning · /u/microscope1024 · 9月27日 03:10

**「背景」** 强化学习（RL）常用于游戏这类任务：模型需要连续采取一系列动作，而评价只针对整段动作序列给出好坏，例如在游戏中「向右走一步」就是一个动作。在这个项目里，两个神经网络智能体在同一款类《街头霸王》的格斗游戏中互为对手进行训练，而「奖励黑客」（reward hacking）指智能体钻奖励函数的空子、拿到高分却并未学会设计者真正想要的行为。多智能体训练中常用的「联赛」（league play）做法，是让智能体轮换面对多个不同对手，以避免只针对某一特定对手过拟合，从而学到更通用的策略。

**「影响」** 对从事多智能体强化学习或自对弈训练的开发者而言，这个项目的经验表明：仅靠胜负信号容易遭遇奖励劫持、需要额外塑造奖励，而只针对单一对手训练会得到只会利用该对手的策略，只有联赛式训练才能带来更通用的策略。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.lukesalamone.com/posts/fighting-game-rl/?ref=home">Teaching a Neural Net to Fight :: Luke Salamone&#x27;s Blog</a></li>

</ul>
</details>

**标签**: `#reinforcement learning`, `#reward hacking`, `#multi-agent RL`, `#game AI`, `#neural networks`

---

<a id="item-tech-news-5"></a>
### [中国发布“太空之弦”计算星座计划](https://www.thepaper.cn/newsDetail_forward_34156091) ⭐️ 7.0/10

东方星链与地卫二于 2026 年 9 月 25 日发布“太空之弦”计算星座计划，拟建设面向全球与深空的太空计算基础设施。该计划分 G1 验证星、G2 标准星和 G3 旗舰星三个阶段推进，其中 G1 验证星预计于 2027 年第四季度发射。架构上，业务层计划部署 720 余颗数据星（推理星）负责数据获取与业务任务，计算层计划部署 360 余颗算力星（训练星）提供计算支持，两层通过星间激光链路连接，并逐步实现计算资源协同调度。这体现出中国企业在天基 AI 计算与卫星网络方向上的布局，但目前公布内容主要是计划框架，尚未给出性能指标、可行性验证或更完整的部署时间表，后续进展仍待观察。

telegram · zaihuapd · 9月27日 03:35

**「背景」** “太空之弦”是一项新发布的太空计算星座计划，被定位为中国首个面向全球与深空的太空计算基础设施，旨在探索天基数据处理、模型部署及计算资源协同调度的新模式。该概念三年前首次提出，规划目标为“千星蓝图”，并设定了 2030 年与 2035 年两个关键节点；项目由地卫二与东方星链共同推进，其中东方星链负责总体设计。2026 年 9 月 25 日，该计划在杭州举行的第五届全球数字贸易博览会产业活动——东方太空计算产业大会暨“太空之弦”计算星座启动仪式上正式启动。

**「影响」** 对中国的卫星运营商与星载 AI 开发者而言，该计划若推进，将把在轨算力从数据采集延伸到训练与推理，形成新的太空计算资源入口；但此前同类星座的实践显示，星间激光链路（如在 1500 公里外锁定十几毫米的通信终端）、太空散热与自主任务管理仍是主要工程瓶颈，且“太空之弦”目前只是发布计划、首颗验证星预计 2027 年第四季度发射，实际能力尚待验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.guandian.cn/article/20260927/607237.html">近日东方星链与地卫二发布“太空之弦” 定位中国首个太空计算基础设施</a></li>
<li><a href="https://www.sohu.com/a/1080873856_122094388">让卫星“看得懂”地球！中国首个太空计算星座“太空之弦”杭州启动，迈向...</a></li>
<li><a href="https://www.toutiao.com/article/7689422405508383251/">让卫星“看得懂”地球 “太空之弦”计算星座在杭州启动 - 今日头条</a></li>
<li><a href="https://blog.csdn.net/WL_ZHG/article/details/147982658">中国“太空计算星座”升空：人工智能上太空的里程碑与战略意义_战略意义:抢占全球太空计算制高点-CSDN博客</a></li>
<li><a href="https://hznews.hangzhou.com.cn/kejiao/content/2025-05/17/content_8996847.htm">把人工智能送上太空 之江实验室牵头组建我国首个整轨互联太空计算星座</a></li>

</ul>
</details>

**标签**: `#space computing`, `#satellite constellation`, `#AI infrastructure`, `#inter-satellite laser links`, `#China tech`

---

<a id="item-tech-news-6"></a>
### [中国数据中心超 24GW，大厂资本开支激增](https://newsletter.semianalysis.com/p/the-chinese-ai-infrastructure-boom) ⭐️ 7.0/10

据 SemiAnalysis 最新模型测算，中国已交付数据中心容量突破 24GW，涵盖 60 余家运营商和 1000 多个设施，规模反超 EMEA 与亚太其他地区总和，并成为全球仅次于北美的庞大物理算力池。此前被市场严重低估的存量零售型机房，正借助高密电气与液冷升级被快速“翻新”为 AI 集群。字节跳动独家包揽全国近 1/5（20%）的交付容量，并在核心节点创下“12 个月落地 100MW”的交付纪录。与此同时，阿里、腾讯、百度 2026Q2 合计资本开支激增至 200 亿美元（同比翻倍），历史性地首次全员录得负自由现金流，显示行业正全面迈入重资产押注电力的军备竞赛。不过，上述数据来自 SemiAnalysis 单一模型测算，当前摘要未披露方法论或独立验证。

telegram · zaihuapd · 9月27日 08:36

**「背景」** 数据中心容量通常以吉瓦（GW）衡量可承载的 IT 负载与供电规模；AI 训练和推理集群对高功率密度机架与液冷的需求，使大量存量零售型机房可通过电气和冷却升级被改造为 AI 算力设施。阿里巴巴、腾讯和百度（BAT）的资本开支与自由现金流是观察这轮基础设施投资强度的重要指标；相关报道显示，三家公司 2026 年第二季度合计资本开支约 200 亿美元、同比翻倍，并首次同时录得负自由现金流。\[tool-1-1\]\[tool-1-3\]

**「影响」** 若 SemiAnalysis 测算成立，中国 AI 算力供给的物理底座将更难被低估，数据中心运营商、液冷与高密电气供应链以及云厂商客户将面对更紧张的电力与机房资源竞争；但该数据仍缺乏独立验证，需谨慎看待。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.polaris7.io/signals/chinas-ai-datacenter-boom-24gw-capacity-20b-bat-capex">China&#x27;s AI Datacenter Boom: 24GW Capacity, $20B BAT Capex</a></li>
<li><a href="https://phemex.com/news/article/chinas-data-center-capacity-hits-24gw-surpassing-emea-and-rest-of-asia-combined-97994">China Data Center Capacity Reaches 24GW, Exceeds ... - Phemex</a></li>

</ul>
</details>

**标签**: `#AI infrastructure`, `#data centers`, `#China tech`, `#capex`, `#SemiAnalysis`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [美国国债收益率飙升，推高 AI 与数据中心企业的借债成本](https://www.cnbc.com/2026/09/27/debt-hungry-data-center-companies-increased-risk-bond-yields-spike.html) ⭐️ 8.0/10

随着美国 10 年期国债收益率升至约 5.17%、为 2007 年以来最高水平（较年初上升约 1 个百分点），依赖发债融资的 AI 与数据中心企业借贷成本上升；摩根大通 6 月估计，到 2030 年 AI 相关债务发行规模将达 4.1 万亿美元。

rss · CNBC Finance · 9月27日 15:35

**「背景」** AI 数据中心建设高度依赖发债融资，而国债收益率是公司债定价的基准，收益率走高意味着发行人必须给出更高的回报率才能吸引投资者；相比之下，亚马逊、谷歌、Meta 和微软等拥有投资级评级的大型科技公司融资成本更低，其余企业压力更大。

**「影响」** 影响最直接的是缺乏投资级评级的“neocloud”等数据中心运营商：CoreWeave 在最新季度文件中披露，截至 6 月，利率每上升 1 个百分点，其利息支出可能增加约 3000 万美元；一位要求匿名的私募信贷投资者称，此类交易今后更难融资，三菱 HC 资本美洲公司的 Riley Thompson 则表示，贷款机构对项目的挑选更严格，市场上真正感兴趣的项目可能从约 50 个减至 20 个。

**标签**: `#AI infrastructure`, `#corporate debt`, `#Treasury yields`, `#data centers`, `#SoftBank`

---