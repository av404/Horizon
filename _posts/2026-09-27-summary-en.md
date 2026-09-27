---
layout: default
title: "Horizon Summary: 2026-09-27 (EN)"
date: 2026-09-27
lang: en
---

> From 30 items, 7 important content pieces were selected

---

**Technology News**
1. [SemiAnalysis Publishes Free Intel Panther Lake and 18A Teardown](#item-tech-news-1) ⭐️ 8.0/10
2. [Show HN: Reladraw – A Diagram Language With Manual Placement](#item-tech-news-2) ⭐️ 7.0/10
3. [Conversations Developer Leaves Google Play, Makes App Free](#item-tech-news-3) ⭐️ 7.0/10
4. [US Appeals Court Upholds Pentagon Blacklisting of Anthropic](#item-tech-news-4) ⭐️ 7.0/10
5. [Excel Beta lets one cell hold multiple values with new array functions](#item-tech-news-5) ⭐️ 7.0/10

**Financial News**
1. [10-year Treasury yield climbs to 5.23%, highest since 2007](#item-finance-news-1) ⭐️ 8.0/10
2. [Hong Kong Regulator and PwC Reach HK$1 Billion Evergrande Audit Settlement](#item-finance-news-2) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [SemiAnalysis Publishes Free Intel Panther Lake and 18A Teardown](https://newsletter.semianalysis.com/p/intel-panther-lake-teardown) ⭐️ 8.0/10

SemiAnalysis has published a free STEEL teardown examining Intel&\#x27;s Panther Lake processor and the Intel 18A process technology. The article, written by Adith Shankar, looks inside both the chip architecture and the manufacturing process. The item is flagged as highly relevant to hardware, systems, and semiconductor readers, but the supplied description does not specify detailed findings from the teardown.

rss · Semianalysis · Sep 26, 13:36

**「Background」** Intel 18A is Intel&\#x27;s leading-edge process node, and Panther Lake is the consumer processor family built to showcase it, assembling one compute tile, one GPU tile, and one I/O tile atop a passive base tile using Intel&\#x27;s Foveros-S advanced packaging, with both compute tile variants using 18A. SemiAnalysis&\#x27;s teardown, the first from its new in-house lab, examines a Core Ultra 7 365 sample and traces 18A structures including PowerVia backside power routing and tile-level process choices.

**「Impact」** Because Panther Lake \(Core Ultra 300 series\) is Intel&\#x27;s first product built on 18A, this independent teardown gives foundry customers and chip designers the first outside check on Intel&\#x27;s process claims — including the advertised 32 nm M0 metal pitch and the stated ~50% CPU/GPU gain over the previous generation — against measured silicon rather than marketing figures. The supplied excerpt does not disclose the teardown&\#x27;s actual measurements, so those specific conclusions cannot be confirmed here.

<details><summary>References</summary>
<ul>
<li><a href="https://newsletter.semianalysis.com/p/intel-panther-lake-teardown">Intel Panther Lake Teardown , 18 A , BSPD, GAAFET, SemiAnalysis ...</a></li>
<li><a href="https://www.neoteo.com/en/semianalysiss-panther-lake-teardown-maps-intel-18as-design">Intel Panther Lake 18 A teardown : what it found | NeoTeo</a></li>
<li><a href="https://www.kucoin.com/news/flash/semianalysis-teardown-shows-smic-s-n-3-node-matches-intel-s-18a-in-metal-pitch">SemiAnalysis teardown shows SMIC&#x27;s N+3 node matches Intel&#x27;s 18A in ...</a></li>
<li><a href="https://introl.com/blog/ces-2026-chip-wars-intel-nvidia-amd">CES 2026 Chip Wars: Intel&#x27;s 18A Breakthrough, NVIDIA&#x27;s | Introl Blog</a></li>

</ul>
</details>

**Tags**: `#Intel 18A`, `#Panther Lake`, `#semiconductor teardown`, `#process technology`, `#chip architecture`

---

<a id="item-tech-news-2"></a>
### [Show HN: Reladraw – A Diagram Language With Manual Placement](https://github.com/reladraw/reladraw) ⭐️ 7.0/10

Reladraw is a new open-source diagram language, introduced in a Show HN post by jpwalsh234, that lets users define diagrams in code while deciding where elements are placed, aiming to combine the layout control of tools like Draw.io with the declarative workflow of auto-placement languages such as Mermaid and Graphviz. The project provides a GitHub-hosted browser playground that requires no installation, plus an npm install option and an installable skill for Claude or other AI agents, according to the author. The author says the goal is to serve both humans and agents, since auto-placement languages do not let users control appearance and graphical editors are slower and harder for agents to manipulate. Hacker News commenters responded positively, calling the relative-positioning approach a useful sweet spot and a good fit for AI-assisted development, while suggesting decoupling topology from layout and enabling reuse as a layout layer for C4. One commenter reported that the playground seemed buggy: an edge written as \`edge parser -&gt; renderer &quot;test edge&quot; from: left to: right\` did not produce a curved arrow.

hackernews · jpwalsh234 · Sep 26, 17:10 · [Discussion](https://news.ycombinator.com/item?id=49858513)

**「Background」** Diagram-as-code tools such as Mermaid and Graphviz let authors define diagrams in text but rely on automatic layout, so the author surrenders control over how the result looks; conversely, WYSIWYG editors like Draw.io give precise control but are slow for humans and awkward for agents to manipulate. Reladraw is an npm-installable text diagram language that renders standalone SVG with no runtime dependencies and uses relative placement statements — described in its documentation as &quot;a text language for diagrams where you say where things go&quot; — so the arrangement can be read back out of the source. A playground in the GitHub repository allows trying it without installation, and instructions are provided for installing a skill usable with Claude or other agents.

**「Impact」** For developers and teams using AI coding agents, Reladraw offers an open-source, npm-installable way to keep diagrams both code-defined and visually controlled, but its early, lightly documented state and the reported playground edge-rendering bug are adoption caveats.

**「Community Discussion」** Commenters were broadly positive, with Garlef calling the relative-placement approach a sweet spot and suggesting a C4 layout layer plus decoupling topology from layout; HeavyStorm said Mermaid works for fixed layouts like sequence diagrams and Gantts but not flowcharts, and judged relative positioning likely sufficient. apinstein and rodmena focused on agent use, and recroad reported a bug where a left-to-right edge did not render as a curved arrow.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/reladraw/reladraw?ref=upstract.com">GitHub - reladraw / reladraw at upstract.com · GitHub</a></li>
<li><a href="https://www.skills.sh/reladraw/reladraw/reladraw">reladraw — reladraw / reladraw</a></li>
<li><a href="https://news.ycombinator.com/item?id=49858513">Show HN: Reladraw – A diagram language where you... | Hacker News</a></li>

</ul>
</details>

**Tags**: `#diagram-as-code`, `#developer-tools`, `#AI-agents`, `#open-source`, `#layout-control`

---

<a id="item-tech-news-3"></a>
### [Conversations Developer Leaves Google Play, Makes App Free](https://gultsch.de/posts/breaking-up-with-google-play/) ⭐️ 7.0/10

The developer of Conversations, an open-source XMPP client for Android, has announced that the app is leaving Google Play and becoming free. The blog post explains the decision and prompted a large Hacker News discussion about Play Store support, fees, and monopoly dynamics. Commenters focused on Google&\#x27;s 15% commission, poor developer support, slow version reviews, and verification hurdles, including a phone-verification step that can reject support numbers using IVR. The supplied source content did not include the full blog post, so the developer&\#x27;s exact rationale and any specific dates, versions, or migration details remain unavailable.

hackernews · ezst · Sep 26, 10:55 · [Discussion](https://news.ycombinator.com/item?id=49855315)

**「Background」** Conversations is an open-source Jabber/XMPP messaging client for Android 6.0+ maintained by Daniel Gultsch, and it had been sold as a paid app on Google Play. Google Play is the primary Android app marketplace, where developers have long contended with its 15% cut, review and verification requirements, support quality, and restrictions on installing apps outside the store. Gultsch’s post provides the first-hand history behind his decision: updates were repeatedly rejected for unclear reasons, and the app was removed from the Play Store twice.

**「Impact」** Android users who previously had to pay for Conversations through Google Play now get the app for free, though they must obtain it outside the Play Store — a shift that also highlights the review delays, removals, 15% revenue cut, and developer-verification hurdles that other indie Android developers relying on Google Play distribution continue to face.

**「Community Discussion」** Commenters broadly agreed that Google Play&\#x27;s 15% commission is less objectionable than its poor support and slow reviews, with some arguing that monopoly power lets Google act this way. Others shared practical difficulties listing products, including phone-number verification that rejects IVR systems, and warned that Google is making sideloading harder through warnings and potential restrictions.

<details><summary>References</summary>
<ul>
<li><a href="https://gultsch.de/posts/breaking-up-with-google-play/">Daniel Gultsch | Breaking Up with Google Play : Why Conversations ...</a></li>
<li><a href="https://play.google.com/store/apps/details?id=eu.siacs.conversations&amp;hl=en">Conversations (Jabber / XMPP ) - Apps on Google Play</a></li>
<li><a href="https://conversations.im/">Conversations : the very last word in instant messaging</a></li>
<li><a href="https://daily.dev/posts/breaking-up-with-google-play-why-conversations-is-now-free-vhls7e2nf">Breaking Up with Google Play: Why Conversations Is Now Free</a></li>
<li><a href="https://gultsch.de/posts/breaking-up-with-google-play/">Breaking Up with Google Play: Why Conversations Is Now Free</a></li>

</ul>
</details>

**Tags**: `#android`, `#google-play`, `#open-source`, `#app-distribution`, `#developer-platforms`

---

<a id="item-tech-news-4"></a>
### [US Appeals Court Upholds Pentagon Blacklisting of Anthropic](https://www.reuters.com/world/us-appeals-court-declines-block-pentagons-blacklisting-anthropic-2026-09-25/) ⭐️ 7.0/10

On September 25, a divided US Court of Appeals for the District of Columbia Circuit ruled 2-1 to uphold the Pentagon&\#x27;s decision to blacklist Anthropic as a national security supply-chain risk, barring the company from military contracts. The majority found the Pentagon&\#x27;s concerns reasonable because Anthropic refused to allow its products to be used for autonomous weapons and mass surveillance. Anthropic said it disagrees with the ruling and is considering asking the full appeals court to rehear the case. The decision follows an earlier ruling by a federal judge in San Francisco who overturned the listing under a different law and blocked the government from imposing a broader ban on Anthropic. Reuters reported the development.

telegram · zaihuapd · Sep 26, 05:19

**「Background」** Anthropic is a major AI developer that the Pentagon designated a national security supply-chain risk in March 2026, barring it from military contracts; Anthropic sued the Trump administration to challenge that action. The dispute arose after Anthropic declined to permit its products to be used for autonomous weapons and mass surveillance, which the Pentagon deemed a security concern. A federal appeals court in Washington, D.C., has now upheld the designation, while a prior San Francisco federal ruling had overturned the listing under a different law and blocked broader restrictions.

**「Impact」** The ruling keeps Anthropic designated as a national security supply-chain risk and barred from U.S. military contracts, shutting it out of defense work it had entered through a $200 million Pentagon contract signed in July 2025. Anthropic says it disagrees with the decision and is considering asking the full appeals court to rehear the case, so the exclusion could still be revisited.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/09/25/pentagon-anthropic-ai-risk-appeals-court.html">U.S. appeals court upholds Pentagon designation of Anthropic as supply chain risk</a></li>
<li><a href="https://www.politico.com/news/2026/09/25/anthropic-national-security-risk-pentagon-ruling-01093285">Appeals court allows Pentagon to label Anthropic a national security risk - POLITICO</a></li>
<li><a href="https://thehill.com/policy/technology/6111414-dc-circuit-upholds-anthropic-blacklist/">D.C. appeals court sides with Pentagon on blacklisting Anthropic</a></li>
<li><a href="https://www.reuters.com/world/how-anthropic-pentagon-dispute-over-ai-safeguards-escalated-2026-09-25/">Anthropic&#x27;s Pentagon blacklist upheld in US appeals court ...</a></li>
<li><a href="https://www.cnbc.com/2026/09/25/pentagon-anthropic-ai-risk-appeals-court.html">U.S. appeals court upholds Pentagon designation of Anthropic ...</a></li>

</ul>
</details>

**Tags**: `#AI policy`, `#Anthropic`, `#Pentagon`, `#defense contracts`, `#national security`

---

<a id="item-tech-news-5"></a>
### [Excel Beta lets one cell hold multiple values with new array functions](https://techcommunity.microsoft.com/blog/microsoft365insiderblog/put-multiple-values-in-one-cell-with-lists-and-arrays-in-excel/4559395) ⭐️ 7.0/10

Microsoft has introduced lists, in-cell arrays, and nested arrays in Excel, initially available to Beta Channel users on Windows and Mac. According to the Microsoft 365 Insider Blog, this is the first time in Excel&\#x27;s 40-year history that a single cell can store multiple values; users can enter items separated by commas or semicolons using Ctrl+J or Insert &gt; List, and can filter and calculate by individual item. The release also adds four array-handling functions: FLATTEN, HAS, HASANY, and HASALL. All of these are preview features, and Microsoft warns that behavior may change before general release, so they should not be used in important workbooks yet.

telegram · zaihuapd · Sep 26, 16:26

**「Background」** Throughout Excel&\#x27;s roughly 40-year history, each cell has been limited to holding a single value, a constraint that has shaped how spreadsheets are structured, filtered, and calculated. Excel&\#x27;s dynamic array feature, which lets one formula return results that spill across multiple adjacent cells, is a related but distinct capability: it changes where results appear rather than how many values an individual cell can contain. The new lists, in-cell arrays, and nested arrays instead target the cell itself, and the four added functions \(FLATTEN, HAS, HASANY, HASALL\) are again preview features whose behavior may change before general release.

**「Impact」** For Windows and Mac users in Excel&\#x27;s Beta channel, the update enables structured lists, in-cell arrays, and nested arrays plus the FLATTEN, HAS, HASANY, and HASALL functions, allowing filtering and calculations by individual item within a single cell. Because Microsoft labels these as preview features whose behavior may change, the practical impact is limited to experimentation, and the company advises against using them in important workbooks.

<details><summary>References</summary>
<ul>
<li><a href="https://techcommunity.microsoft.com/blog/microsoft365insiderblog/put-multiple-values-in-one-cell-with-lists-and-arrays-in-excel/4559395">Put multiple values in one cell with lists and arrays in Excel | Microsoft Community Hub</a></li>
<li><a href="https://www.ablebits.com/office-addins-blog/excel-dynamic-arrays-functions-formulas/">Excel dynamic arrays, functions and formulas</a></li>
<li><a href="https://www.excelcampus.com/functions/list-arrays-in-cells/">Excel Lists in Cells: HAS, HASALL, HASANY &amp; FLATTEN</a></li>
<li><a href="https://techcommunity.microsoft.com/blog/microsoft365insiderblog/put-multiple-values-in-one-cell-with-lists-and-arrays-in-excel/4559395">Put multiple values in one cell with lists and arrays in Excel | Microsoft Community Hub</a></li>

</ul>
</details>

**Tags**: `#Excel`, `#Microsoft 365`, `#电子表格`, `#数组公式`, `#预览功能`

---

## Financial News

<a id="item-finance-news-1"></a>
### [10-year Treasury yield climbs to 5.23%, highest since 2007](https://www.cnbc.com/2026/09/26/10-year-treasury-yield-is-at-its-highest-in-19-years-how-we-got-here.html) ⭐️ 8.0/10

The 10-year Treasury yield rose to 5.23% on Friday, its highest level since 2007, after trading just below 4.8% earlier in September. Fed funds futures trading shows a 64% likelihood of a Federal Reserve rate hike in October, according to the CME FedWatch tool.

rss · CNBC Finance · Sep 26, 13:30

**「Background」** Bond yields rise when prices fall, and this move reflects stubborn inflation — the University of Michigan&\#x27;s survey put year-ahead inflation expectations at 4.6% in September, up from 4% in August — alongside heavy borrowing by the federal government and by AI-related companies. Thierry Wizman, a rates strategist at Macquarie Group, told CNBC that bond issuance, not inflation, is the bigger driver this year, and Vanguard estimates that Alphabet, Amazon, Meta, Microsoft and Oracle issued about $132 billion of debt through July, against an annual average of roughly $35 billion from 2020 through 2024.

**「Impact」** The 10-year yield is a benchmark for mortgages and other borrowing, so its climb points to higher costs for households and businesses taking on debt, while higher yields can also weigh on stocks by making bonds more attractive to income-seeking investors.

**Tags**: `#Treasury yields`, `#Federal Reserve`, `#inflation`, `#bond issuance`, `#AI infrastructure`

---

<a id="item-finance-news-2"></a>
### [Hong Kong Regulator and PwC Reach HK$1 Billion Evergrande Audit Settlement](https://wallstreetcn.com/articles/3782573) ⭐️ 7.0/10

Hong Kong&\#x27;s Securities and Futures Commission reached a HK$1 billion settlement with PwC Hong Kong over audit failures related to China Evergrande, with the firm not admitting liability and the money going to compensate affected independent minority shareholders rather than Evergrande&\#x27;s estate. Evergrande&\#x27;s liquidators have asked a court to set the settlement aside, and the Hong Kong High Court is expected to rule around the end of October.

telegram · zaihuapd · Sep 26, 07:18

**「Background」** The settlement stems from the Hong Kong Securities and Futures Commission&\#x27;s case over PwC Hong Kong&\#x27;s audits of China Evergrande, which is in liquidation; the payout therefore goes to small outside shareholders rather than to Evergrande&\#x27;s creditors, whose claims are handled separately by the liquidators.

**「Impact」** If upheld, the settlement would use PwC Hong Kong&\#x27;s HK$1 billion to compensate eligible independent minority shareholders of Evergrande without changing creditors&\#x27; claim priority, because the funds come from PwC Hong Kong rather than Evergrande&\#x27;s estate.

<details><summary>References</summary>
<ul>
<li><a href="https://news.qq.com/rain/a/20260424A01VGD00">普 华 永 道 将支付 10 ...</a></li>
<li><a href="https://www.pai.com.cn/p/01m1gsjd2d032ss55xp9h3m9nx">突发，许家印背后靠山被制裁 - 电商派</a></li>

</ul>
</details>

**Tags**: `#香港证监会`, `#普华永道`, `#恒大`, `#审计和解`, `#清盘人诉讼`

---