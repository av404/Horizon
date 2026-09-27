---
layout: default
title: "Horizon Summary: 2026-09-27 (ZH)"
date: 2026-09-27
lang: zh
---

> 从 30 条内容中筛选出 7 条重要资讯。

---

**科技新闻**
1. [SemiAnalysis 拆解英特尔 Panther Lake 与 Intel 18A](#item-tech-news-1) ⭐️ 8.0/10
2. [Reladraw：人机皆可用的相对定位图表语言](#item-tech-news-2) ⭐️ 7.0/10
3. [Conversations 退出 Google Play 并转为免费](#item-tech-news-3) ⭐️ 7.0/10
4. [美上诉法院 2 比 1 维持五角大楼将 Anthropic 列入黑名单](#item-tech-news-4) ⭐️ 7.0/10
5. [Excel 首次支持单元格内多值列表与数组](#item-tech-news-5) ⭐️ 7.0/10

**财经新闻**
1. [10 年期美债收益率升至 5.23%，为 2007 年以来最高](#item-finance-news-1) ⭐️ 8.0/10
2. [香港证监会与普华永道香港就恒大审计达成 10 亿港元和解](#item-finance-news-2) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [SemiAnalysis 拆解英特尔 Panther Lake 与 Intel 18A](https://newsletter.semianalysis.com/p/intel-panther-lake-teardown) ⭐️ 8.0/10

SemiAnalysis 发布了针对英特尔 Panther Lake 处理器与 Intel 18A 工艺的拆解分析。该拆解为免费的 STEEL 拆解，旨在深入芯片与制程内部。由于原文描述较为简略，并未披露具体的技术发现或性能数据。该分析面向硬件、系统与半导体领域的读者，属于技术深度剖析。

rss · Semianalysis · 9月26日 13:36

**「背景」** Panther Lake 是 Intel 的消费级处理器，采用 Foveros-S 先进封装，把计算 tile、GPU tile 与 I/O tile 堆叠在一片无源基础 tile 之上，两种计算 tile 版本都基于 Intel 18A 制程。Intel 18A 是 Intel 的先进制程节点，其 GAAFET 晶体管、PowerVia 背面供电以及最小金属间距等结构指标常被外界用来评估 Intel 的制造与代工能力，因此对其成品芯片的物理拆解具有参考价值。此次拆解出自 SemiAnalysis 新建的自有芯片拆解实验室，该实验室此前的分析曾把 SMIC 第三代 7nm 的 32.5nm 最小局域金属间距与 Panther Lake 所用 Intel 18A 的 36nm 间距作对比。

**「影响」** 对计划采用 Panther Lake（Core Ultra 300 系列，Intel 首款 18A 产品）的 OEM 与开发者而言，这份拆解提供了独立于厂商宣传的 18A 关键尺寸数据（如 32 纳米 M0 金属间距），可直接用于评估该工艺相对竞品的实际竞争力。由于所给摘要未列出具体测量结果，其结论仍需以拆解全文数据为准。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://newsletter.semianalysis.com/p/intel-panther-lake-teardown">Intel Panther Lake Teardown , 18 A , BSPD, GAAFET, SemiAnalysis ...</a></li>
<li><a href="https://www.neoteo.com/en/semianalysiss-panther-lake-teardown-maps-intel-18as-design">Intel Panther Lake 18 A teardown : what it found | NeoTeo</a></li>
<li><a href="https://www.tomshardware.com/tech-industry/semiconductors/semianalysis-opens-its-own-chip-teardown-lab">Chinese fab SMIC&#x27;s 7nm metal pitch beats Intel 18 A but lags 38% on...</a></li>
<li><a href="https://www.kucoin.com/news/flash/semianalysis-teardown-shows-smic-s-n-3-node-matches-intel-s-18a-in-metal-pitch">SemiAnalysis teardown shows SMIC&#x27;s N+3 node matches Intel&#x27;s 18A in ...</a></li>
<li><a href="https://introl.com/blog/ces-2026-chip-wars-intel-nvidia-amd">CES 2026 Chip Wars: Intel&#x27;s 18A Breakthrough, NVIDIA&#x27;s | Introl Blog</a></li>

</ul>
</details>

**标签**: `#Intel 18A`, `#Panther Lake`, `#semiconductor teardown`, `#process technology`, `#chip architecture`

---

<a id="item-tech-news-2"></a>
### [Reladraw：人机皆可用的相对定位图表语言](https://github.com/reladraw/reladraw) ⭐️ 7.0/10

作者 jpwalsh234 在 Hacker News 上发布 Show HN，介绍开源图表语言 Reladraw。它试图解决现有工具的取舍问题：Mermaid、Graphviz 这类自动布局语言不让用户决定图表外观，而 Draw.io 虽强大却耗时且不利于代理操作。Reladraw 允许用图表语言定义图表，同时保留对元素放置的高度控制，并明确面向人类和 AI 代理两种工作流。GitHub 页面提供无需安装的 playground、简单的 npm 安装方式，以及可配合 Claude 或其他代理使用的 skill。Hacker News 讨论整体积极，认为它处在自动布局与手动控制之间的合适位置，但早期提交也收到具体 bug 报告。

hackernews · jpwalsh234 · 9月26日 17:10 · [社区讨论](https://news.ycombinator.com/item?id=49858513)

**「背景知识」** 图表即代码（diagram-as-code）工具长期分为两类：Mermaid、Graphviz 等语言自动决定元素位置，用户难以控制最终外观；Draw.io 之类软件可以手动摆放，但耗时且不利于 AI 代理操作。Reladraw 试图兼取两者，用文本语言直接描述元素之间的相对位置关系，使排列方式可以从源码中读回，并输出独立的 SVG 而无需运行时依赖。

**「影响」** 对需要精确控制图表布局、又希望 AI 代理能操作的开发者而言，Reladraw 提供了介于 Mermaid/Graphviz 自动布局与 Draw.io 手动绘图之间的开源选择；不过当前版本已出现弯曲箭头渲染的 bug 报告，早期采用需权衡稳定性。

**「社区讨论」** 评论总体正面，认为 Reladraw 在自动布局与手动控制之间找到平衡点，适合 AI 编程时代的人机对齐；有人建议将箭头、分组等拓扑结构与“左/右”等布局关注点解耦，或让它作为 C4 的布局层。质疑集中在代理能否自行创建复杂图表，并有用户报告具体 bug：添加“edge parser -&gt; renderer &quot;test edge&quot; from: left to: right”后，未能智能生成弯曲箭头；同时多位用户表示会尝试将其加入代理可用的图表工具。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/reladraw/reladraw?ref=upstract.com">GitHub - reladraw / reladraw at upstract.com · GitHub</a></li>
<li><a href="https://www.skills.sh/reladraw/reladraw/reladraw">reladraw — reladraw / reladraw</a></li>

</ul>
</details>

**标签**: `#diagram-as-code`, `#developer-tools`, `#AI-agents`, `#open-source`, `#layout-control`

---

<a id="item-tech-news-3"></a>
### [Conversations 退出 Google Play 并转为免费](https://gultsch.de/posts/breaking-up-with-google-play/) ⭐️ 7.0/10

Conversations 是一款开源 XMPP 客户端；其开发者发布文章《Breaking Up with Google Play: Why Conversations Is Now Free》，说明该应用退出 Google Play，并将原本付费的应用改为免费。由于提供的材料没有博文正文，具体退出时间、下架安排、是否改用其他分发渠道等细节尚不清楚。Hacker News 讨论把这一决定放在 Google Play 约 15% 分成、支持与审核反馈质量不佳，以及平台垄断或双寡头格局的背景下审视。对开源 Android 生态和独立开发者来说，此事凸显了应用商店依赖、分发可持续性与平台规则之间的紧张关系。

hackernews · ezst · 9月26日 10:55 · [社区讨论](https://news.ycombinator.com/item?id=49855315)

**「背景」** Conversations 是由 Daniel Gultsch 开发的开源 Jabber/XMPP 安卓客户端，长期以付费应用的形式在 Google Play 上架，面向 Android 6.0 及以上系统提供支持。据作者自述，他与 Google 的关系一直不佳：应用更新曾多次以令人费解的理由被拒绝，Conversations 还两次被从 Play Store 移除。正是在这一背景下，他撰文说明为何与 Google Play 分道扬镳，并将应用改为免费提供。

**「影响」** 对 Conversations 的 Android 用户而言，应用在 Google Play 上架 12 年半后转为免费并撤下付费列表，获取与更新将更依赖 Play 之外的渠道。对独立与开源 Android 开发者而言，这凸显了审核延迟、无解释下架、15% 抽成和开发者验证门槛等分发风险，并展示了资助支持的替代路径。

**「社区讨论」** 评论区普遍不反对支付合理费用，但认为核心问题在于 Google Play 的支持质量：pi-victor 表示若 15% 分成能换来及时反馈和快速版本审核，开发者就不会抱怨，而垄断地位让 Google 无需改进；k1w1 则分享了一年仍无法上架的经历，障碍是 Google 要求验证支持电话号码，却默认开发者是个人或小公司。另有评论者抱怨大公司客服整体恶化、只有社交媒体曝光才有效，并担忧 Google Play 从爱好者的发布平台变成需要企业地址和文件的门槛，以及对 Play Store 之外安装越来越不友好。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://gultsch.de/posts/breaking-up-with-google-play/">Daniel Gultsch | Breaking Up with Google Play : Why Conversations ...</a></li>
<li><a href="https://play.google.com/store/apps/details?id=eu.siacs.conversations&amp;hl=en">Conversations (Jabber / XMPP ) - Apps on Google Play</a></li>
<li><a href="https://conversations.im/">Conversations : the very last word in instant messaging</a></li>
<li><a href="https://daily.dev/posts/breaking-up-with-google-play-why-conversations-is-now-free-vhls7e2nf">Breaking Up with Google Play: Why Conversations Is Now Free</a></li>
<li><a href="https://gultsch.de/posts/breaking-up-with-google-play/">Breaking Up with Google Play: Why Conversations Is Now Free</a></li>

</ul>
</details>

**标签**: `#android`, `#google-play`, `#open-source`, `#app-distribution`, `#developer-platforms`

---

<a id="item-tech-news-4"></a>
### [美上诉法院 2 比 1 维持五角大楼将 Anthropic 列入黑名单](https://www.reuters.com/world/us-appeals-court-declines-block-pentagons-blacklisting-anthropic-2026-09-25/) ⭐️ 7.0/10

据路透社报道，美国华盛顿特区联邦上诉法院于 9 月 25 日以 2 比 1 的裁决，维持五角大楼将 Anthropic 列为国家安全供应链风险、禁止其参与军事合同的决定。多数法官认为，Anthropic 拒绝允许其产品被用于自主武器和大规模监控，五角大楼由此产生的担忧是合理的。Anthropic 表示不同意该裁决，并正考虑请求全体上诉法院复审。此前，一名旧金山联邦法官曾依据另一部法律推翻这一列名，并阻止政府对 Anthropic 实施更广泛的禁令。上述信息来自一则简短的 Telegram 投稿，未提供案件编号、判决书原文或五角大楼与 Anthropic 的进一步回应。

telegram · zaihuapd · 9月26日 05:19

**「背景」** 美国国防部（五角大楼）此前于 3 月将 Anthropic 列为国家安全供应链风险，理由与其拒绝允许产品用于自主武器和大规模监控有关；Anthropic 随后起诉特朗普政府，试图撤销这一列名。华盛顿特区联邦上诉法院此次裁决维持该列名，允许五角大楼继续禁止 Anthropic 参与军事合同；此前旧金山联邦法官曾依据另一部法律推翻相关列名并阻止更广泛的禁令。该案还涉及行政部门将美国企业指定为国家安全风险的权力范围。

**「影响」** 该裁决使 Anthropic 继续被排除在五角大楼军事合同之外，并被维持为国家安全供应链风险，其此前与国防部签署的 2 亿美元合同所涉合作在 2025 年 9 月谈判破裂后仍无法推进。不过 Anthropic 正考虑请求全体上诉法院复审，且此前旧金山联邦法官曾依另一部法律推翻相关列名，因此该列名对其更广泛政府业务的最终影响仍未确定。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/09/25/pentagon-anthropic-ai-risk-appeals-court.html">U.S. appeals court upholds Pentagon designation of Anthropic as supply chain risk</a></li>
<li><a href="https://www.politico.com/news/2026/09/25/anthropic-national-security-risk-pentagon-ruling-01093285">Appeals court allows Pentagon to label Anthropic a national security risk - POLITICO</a></li>
<li><a href="https://thehill.com/policy/technology/6111414-dc-circuit-upholds-anthropic-blacklist/">D.C. appeals court sides with Pentagon on blacklisting Anthropic</a></li>
<li><a href="https://www.reuters.com/world/how-anthropic-pentagon-dispute-over-ai-safeguards-escalated-2026-09-25/">Anthropic&#x27;s Pentagon blacklist upheld in US appeals court ...</a></li>
<li><a href="https://www.cnbc.com/2026/09/25/pentagon-anthropic-ai-risk-appeals-court.html">U.S. appeals court upholds Pentagon designation of Anthropic ...</a></li>

</ul>
</details>

**标签**: `#AI policy`, `#Anthropic`, `#Pentagon`, `#defense contracts`, `#national security`

---

<a id="item-tech-news-5"></a>
### [Excel 首次支持单元格内多值列表与数组](https://techcommunity.microsoft.com/blog/microsoft365insiderblog/put-multiple-values-in-one-cell-with-lists-and-arrays-in-excel/4559395) ⭐️ 7.0/10

微软在 Excel Beta 通道面向 Windows 和 Mac 推出列表、单元格内数组与嵌套数组，这是 Excel 40 年来首次允许在一个单元格中存放多个值。用户可通过 Ctrl+J 或「插入 &gt; 列表」写入以逗号或分号分隔的多个项目，并能按单项筛选与计算。该功能同时新增 FLATTEN、HAS、HASANY、HASALL 四个数组处理函数。这些均为预览功能，正式发布前行为可能调整，官方建议暂不用于重要工作簿。

telegram · zaihuapd · 9月26日 16:26

**「背景」** 在 Excel 约 40 年的历史中，每个单元格只能存放一个值，这是其数据模型长期不变的基本约束。此前 Excel 已引入动态数组函数，可对区域运算并返回多个结果，像 UNIQUE、COUNTA 这类函数还能相互嵌套使用；而在 Excel 2016、2019 等旧版本中，把区域传给某些函数只会返回第一个单元格的单个结果，反映出旧模型对多值处理能力的限制。此次「列表」与「单元格内数组」改变的正是这一底层约束，因此微软同时新增 FLATTEN、HAS、HASANY、HASALL 四个函数，用于处理存放在单个单元格内的多个值。

**「影响」** Windows 与 Mac 的 Beta 通道用户现在可在单个单元格中存放列表、数组乃至嵌套数组，并借助新增的 FLATTEN、HAS、HASANY、HASALL 函数实现更智能的筛选与逐项计算，使此前难以落地的单表内动态统计设计成为可能。但这些功能仍属预览阶段，正式发布前行为可能调整，官方建议暂不用于重要工作簿。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techcommunity.microsoft.com/blog/microsoft365insiderblog/put-multiple-values-in-one-cell-with-lists-and-arrays-in-excel/4559395">Put multiple values in one cell with lists and arrays in Excel | Microsoft Community Hub</a></li>
<li><a href="https://slashdot.org/story/26/09/26/0227226/after-40-years-microsoft-excel-will-add-single-cell-lists-and-arrays">After 40 Years, Microsoft Excel Will Add Single-Cell Lists and Arrays - Slashdot</a></li>
<li><a href="https://www.ablebits.com/office-addins-blog/excel-dynamic-arrays-functions-formulas/">Excel dynamic arrays, functions and formulas</a></li>
<li><a href="https://www.geeky-gadgets.com/multiple-values-one-excel-cell/">Microsoft Excel Beta Lets Single Cells Store Nested Arrays</a></li>
<li><a href="https://www.excelcampus.com/functions/list-arrays-in-cells/">Excel Lists in Cells: HAS, HASALL, HASANY &amp; FLATTEN</a></li>
<li><a href="https://techcommunity.microsoft.com/blog/microsoft365insiderblog/put-multiple-values-in-one-cell-with-lists-and-arrays-in-excel/4559395">Put multiple values in one cell with lists and arrays in Excel | Microsoft Community Hub</a></li>

</ul>
</details>

**标签**: `#Excel`, `#Microsoft 365`, `#电子表格`, `#数组公式`, `#预览功能`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [10 年期美债收益率升至 5.23%，为 2007 年以来最高](https://www.cnbc.com/2026/09/26/10-year-treasury-yield-is-at-its-highest-in-19-years-how-we-got-here.html) ⭐️ 8.0/10

10 年期美国国债收益率周五升至 5.23%，为 2007 年以来最高；本月初该收益率还略低于 4.8%。

rss · CNBC Finance · 9月26日 13:30

**「背景」** 背景是通胀顽固、市场预期美联储进一步加息，以及联邦政府为赤字融资和 AI 相关企业大举发债共同推高债券供给；Macquarie 策略师蒂埃里·维兹曼称，今年发债因素比通胀更重要。

**「影响」** 这一收益率影响房贷利率，并可能通过抬高企业借贷成本、使债券对收益型投资者更具吸引力而压制股票。

**标签**: `#Treasury yields`, `#Federal Reserve`, `#inflation`, `#bond issuance`, `#AI infrastructure`

---

<a id="item-finance-news-2"></a>
### [香港证监会与普华永道香港就恒大审计达成 10 亿港元和解](https://wallstreetcn.com/articles/3782573) ⭐️ 7.0/10

香港证监会与普华永道香港就恒大审计失职达成和解，普华永道不承认责任，但同意支付 10 亿港元，用于补偿受影响的独立小股东。这笔款项来自普华永道香港而非恒大财产，未改变恒大债权人的申索优先次序；恒大清盘人已入禀法院要求撤销该和解，香港高等法院预计 10 月底左右作出判决。

telegram · zaihuapd · 9月26日 07:18

**「背景」** 普华永道香港此前担任中国恒大的审计机构，香港证监会针对其审计失职展开追究并以和解方式结案；恒大现已进入清盘程序，因此由其清盘人而非公司董事会向法院申请撤销该和解。

**「影响」** 若和解最终生效，恒大的合资格独立小股东可从普华永道香港预留的 10 亿港元中获得赔偿，而该笔款项出自普华永道而非恒大财产，因此不改变恒大债权人的申索优先次序；但清盘人已入禀要求撤销和解，赔偿能否实际发放仍取决于法院判决。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.qq.com/rain/a/20260424A01VGD00">普 华 永 道 将支付 10 ...</a></li>
<li><a href="https://www.pai.com.cn/p/01m1gsjd2d032ss55xp9h3m9nx">突发，许家印背后靠山被制裁 - 电商派</a></li>
<li><a href="https://www.163.com/dy/article/KR7Q39DV055616EC.html">刚刚！ 普 华 永 道 为 恒 大 埋单 10 亿 ！行业的遮羞布被彻底撕开</a></li>

</ul>
</details>

**标签**: `#香港证监会`, `#普华永道`, `#恒大`, `#审计和解`, `#清盘人诉讼`

---