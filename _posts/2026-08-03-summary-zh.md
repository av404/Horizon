---
layout: default
title: "Horizon Summary: 2026-08-03 (ZH)"
date: 2026-08-03
lang: zh
---

> 从 32 条内容中筛选出 8 条重要资讯。

---

**科技新闻**
1. [Karpathy 的鹈鹕演示：AI 物理世界理解的新定性基准](#item-tech-news-1) ⭐️ 7.0/10
2. [eBay 骚扰批评者遭 5600 万美元索赔及监禁判决](#item-tech-news-2) ⭐️ 7.0/10
3. [AI 发展公开信：开放权重与安全之争](#item-tech-news-3) ⭐️ 7.0/10
4. [苹果限制漏洞报告提交量，应对 AI 低质量报告激增](#item-tech-news-4) ⭐️ 7.0/10

**财经新闻**
1. [高盛交易业务料创历史最佳年度，股票交易季度收入增 72%至 74.2 亿美元](#item-finance-news-1) ⭐️ 8.0/10
2. [住房公积金条例拟修订：灵活就业者可缴存，装修物业费可提取](#item-finance-news-2) ⭐️ 7.0/10
3. [深圳电动车违法正式纳入征信，宝安已录入 50 人](#item-finance-news-3) ⭐️ 7.0/10
4. [日美联合干预汇市阻止日元跌至近 40 年低点](#item-finance-news-4) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Karpathy 的鹈鹕演示：AI 物理世界理解的新定性基准](https://twitter.com/karpathy/status/2083749667410727319) ⭐️ 7.0/10

Karpathy 展示了一个“鹈鹕”（pelican）演示，被 Hacker News 讨论为一种评估 AI 物理世界理解的新定性基准。该演示不再只是生成图像，而是生成物理场景，社区认为这类基准能更好地暴露模型对物理世界的理解，并可用于衡量未来进展，尽管它属于主观测量。评论还提到，类似“创建弹球游戏”的简单任务仍会难倒前沿大语言模型，而 Opus 5 据称是首个能“一次成功”的模型。有用户尝试让 Opus 5 用威廉·吉布森《神经漫游者》开头做同样的事，但模型因版权问题拒绝逐字引用文本。演示的可复现性受到质疑，因为原始推文没有公开所使用的 prompt。

hackernews · delichon · 8月2日 04:05 · [社区讨论](https://news.ycombinator.com/item?id=49140998)

**「背景」** 这个讨论源于 Andrej Karpathy 的一条推文：他提出，测试 LLM 的传统方式（例如“生成一个骑自行车的鹈鹕 SVG”）正在被更能体现物理世界理解的新形式取代。Karpathy 让 Opus 5 用约 100 万 token 的预算（约合 10 美元）读取《指环王》第一段，并请求生成一个 three.js 渲染；模型运行约两小时后写出了 5500 行程序化渲染代码，结果虽然粗糙，但展示了模型在长程规划和场景编排上的能力。Hacker News 评论者因此讨论是否应把这类生成式物理场景作为新的定性基准，并指出 Karpathy 未公开提示词，导致示例难以复现。

**「影响」** 对 AI 研究者和模型开发者而言，这类物理场景生成演示提供了一种可检验世界理解的新定性基准，并可能促使模型厂商将“可玩且物理合理”的输出作为能力目标；不过由于 prompt 未公开，外部暂时无法直接复现这一特定演示。

**「社区讨论」** 评论者普遍认为成品粗糙正是重点，模型已从生成图像转向更能揭示物理世界理解的新基准，但有人质疑缺少 prompt 导致不可复现；还有用户分享了让 Opus 5 改编《神经漫游者》时因版权被拒的尝试，以及用 LLM 构建《回到未来》德罗宁时光机 3D 动画的实践经验。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://x.com/karpathy/status/2083749667410727319">Andrej Karpathy on X: &quot;We&#x27;re starting to leave the territory where you&#x27;d test an LLM by e.g. &quot;create an svg of pelican on a bicycle&quot;. As one idea to generalize it, I was interested what Opus 5 would do if I gave it the first paragraph of the Lord of the Rings, a 1M token budget (~$10) and asked for three js render of it. Opus went off for ~2 hours and wrote 5500 lines of code that (procedurally) rendered the story. It&#x27;s kind of janky but fun. But it&#x27;s a bit mindboggling that the LLM has to place and orchest</a></li>

</ul>
</details>

**标签**: `#AI`, `#large language models`, `#3D simulation`, `#benchmarks`, `#reproducibility`

---

<a id="item-tech-news-2"></a>
### [eBay 骚扰批评者遭 5600 万美元索赔及监禁判决](https://www.ft.com/content/06ec1b03-d4af-40cf-b12a-4ba5a410f6d2) ⭐️ 7.0/10

美国司法部披露，eBay 前安全团队高层因对批评者夫妇实施骚扰恐吓而被判刑，eBay 已同意支付 5600 万美元和解金。前安全与安保高级总监 Jim Baugh 被判 57 个月监禁，前全球安全团队特别行动高级经理 Brian Gilbert 被判已服刑时间并罚款 2 万美元。该案涉及七名安全团队成员，包括前警长，他们针对 Ina 和 David Steiner 夫妇进行威胁、监控和骚扰。此案凸显大型科技公司安全团队滥用权力、缺乏监督的问题，并带来企业问责与法律后果。

hackernews · JumpCrisscross · 8月2日 19:19 · [社区讨论](https://news.ycombinator.com/item?id=49147435)

**「背景信息」** 这起事件源于 eBay 前全球安全团队高层吉姆·鲍（Jim Baugh）等人，因不满马萨诸塞州夫妇大卫·斯坦纳（David Steiner）与伊娜·斯坦纳（Ina Steiner）运营的电子商务博客对其公司的批评，于 2019 年组织下属实施跟踪、骚扰和恐吓。受害夫妇随后提起诉讼，案件和解一度破裂，直至 2026 年 7 月 28 日，eBay 及三名前高管同意以约 5600 万美元达成和解；此前多名涉案前安全部门成员已在联邦刑事案件中被判刑或认罪。

**「影响」** 此案为科技公司安全部门滥用职权划定了明确的法律红线，可能促使企业加强内部监督，并给其他面临类似行为的企业敲响警钟。

**「社区讨论」** 评论区对案件是否只涉及这一对批评者表示怀疑，认为应彻查 eBay 是否对其他批评者实施过类似行动；也有人借题讨论 eBay 平台收费过高，而另一些人则引用“无人监督时行为会变坏”的观点，强调缺乏监管的危害。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/EBay_stalking_scandal">eBay stalking scandal - Wikipedia</a></li>
<li><a href="https://www.cnn.com/2026/07/28/business/ebay-harrassment-case-hnk">EBay, former executives to pay $56 million to settle couple’s harassment case | CNN Business</a></li>
<li><a href="https://www.bbc.com/news/articles/cj039p238r5o">eBay agrees $56m settlement with bloggers over harassment case</a></li>

</ul>
</details>

**标签**: `#ebay`, `#corporate accountability`, `#security`, `#legal`, `#harassment`

---

<a id="item-tech-news-3"></a>
### [AI 发展公开信：开放权重与安全之争](https://simonwillison.net/2026/Aug/2/open-letters/#atom-everything) ⭐️ 7.0/10

西蒙·威利森总结了近期围绕 AI 发展的多封公开信。微软主导的《开放权重与美国 AI 领导力》于 7 月 24 日发布，已有 235 家 AI 相关公司签署，包括英伟达、亚马逊、Y Combinator、Linux 基金会以及后来加入的 OpenAI。信中主张不应因安全担忧而禁止或限制开放权重模型，认为封闭模型同样可能被攻破或滥用，且会造成少数单点故障并削弱竞争；信中还明确支持蒸馏技术，呼吁政策制定者不要将合法的模型开发技术等同于盗用。Anthropic 未签署该信，并在三天后发布自己的立场，CEO 达里奥·阿莫迪对威权政府构建更强 AI 模型及模型被用于网络或生物攻击表示担忧，同时呼吁打击工业规模的蒸馏活动，但重申 Anthropic 从未倡导禁止开放权重模型。7 月 28 日，《Pacing the Frontier》公开信发布，获得 1324 名前沿 AI 公司员工签署，包括 OpenAI 首席科学家雅库布·帕乔基、伊利亚·苏茨克弗、达里奥·阿莫迪等，他们请求美国政府支持国际合作，开发用于有意调控自动化 AI 发展前沿的技术与治理工具。

rss · Simon Willison · 8月2日 04:16

**「背景」** 2026 年 6 月，美国政府以国家安全为由发布出口管制指令，暂停所有外国国民（包括 Anthropic 自家外籍员工）访问 Anthropic 的 Claude Fable 5 和 Mythos 5 模型，引发业界对开放权重模型可能被限制的担忧。随后，微软于 7 月 24 日主导发布公开信《Open Weights and American AI Leadership》，联合 NVIDIA、亚马逊、Y Combinator 等 235 家公司，主张开放权重模型有助于竞争与安全审查，并反对因“安全”理由禁止或限制开放权重模型。

**「影响」** 这些公开信凸显了美国 AI 政策辩论的关键分歧：以微软为首的阵营主张开放权重并保护蒸馏技术，而 Anthropic 及部分前沿 AI 公司员工则呼吁对蒸馏和自动化 AI 研发加强管控，这可能影响美国政府对开放权重模型及相关技术的监管立场。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.microsoft.com/en-us/corporate-responsibility/topics/open-weight/">Open Weights and American AI Leadership</a></li>
<li><a href="https://www.anthropic.com/news/fable-mythos-access">Statement on the US government directive to suspend access to...</a></li>

</ul>
</details>

**标签**: `#AI policy`, `#open source`, `#open weights`, `#industry news`, `#Simon Willison`

---

<a id="item-tech-news-4"></a>
### [苹果限制漏洞报告提交量，应对 AI 低质量报告激增](https://www.ft.com/content/4532122d-90f2-4433-9df6-ca99d8a141d2?syn-25a6b1a6=1) ⭐️ 7.0/10

苹果承认已于今年 6 月限制安全研究人员可同时提交的漏洞报告数量，并设置 30 天冷却期，以应对借助 AI 模型生成的低质量安全报告激增。意大利安全公司 Bynario 表示，其使用 ChatGPT 在三周内于最新 macOS 中发现 50 多个漏洞，包括可使攻击者完全控制电脑的提权漏洞链，但因提交限额无法向苹果报告。苹果称已联系 Bynario 并审核其提交，同时也在用 AI 加强自身防御，本周安全更新修复数量约为以往的五倍，并致谢 Anthropic 和 OpenAI 的工具协助发现漏洞。此举体现 LLM 对安全研究攻防两端的双重影响。

telegram · zaihuapd · 8月2日 05:50

**「背景」** 漏洞奖励计划通常设定提交限制或配额，以保证厂商能优先处理严重问题。随着 AI 工具能快速生成大量格式规范但质量不一的漏洞报告，安全团队收到的噪音急剧增加，促使苹果采用提交限额与冷却期机制。

**「影响」** 对于依赖 AI 批量发现漏洞的研究者，提交限制和 30 天冷却期可能使其无法及时上报高危发现（如 Bynario 发现的 macOS 提权链），而苹果正在通过 AI 辅助修复将单次安全更新修复量提升到约五倍。

**标签**: `#Apple`, `#vulnerability management`, `#AI security`, `#macOS`, `#LLM`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [高盛交易业务料创历史最佳年度，股票交易季度收入增 72%至 74.2 亿美元](https://www.cnbc.com/2026/08/01/goldman-traders-are-on-pace-for-a-record-year-a-close-up-look-at-how-theyre-doing-it.html) ⭐️ 8.0/10

高盛交易业务正有望创下纪录年度，其股票交易业务第二季度收入同比激增 72%，达 74.2 亿美元的历史新高。

rss · CNBC Finance · 8月2日 13:52

**「背景」** 高盛近年通过全球银行与市场部门的交叉销售策略，把投行、财富管理客户引入股票业务，并在市场波动和 AI 资本开支周期中获益。

**「影响」** 强劲的交易收入可能继续支撑高盛整体业绩，也显示市场波动正在提振华尔街大型银行的交易业务。

**标签**: `#Goldman Sachs`, `#equities trading`, `#investment banking`, `#market volatility`, `#earnings`

---

<a id="item-finance-news-2"></a>
### [住房公积金条例拟修订：灵活就业者可缴存，装修物业费可提取](https://weibo.com/1642634100/RbwfKezfq) ⭐️ 7.0/10

住建部近日就《住房公积金管理条例（修订征求意见稿）》公开征求意见，拟允许个体工商户、外卖员、快递员、网约车司机等灵活就业人员自愿缴存公积金，并将自住住房装修、支付物业费纳入提取范围。此为征求意见稿，尚未正式施行。

telegram · zaihuapd · 8月2日 06:32

**「背景」** 中国的住房公积金制度始于上世纪 90 年代初，借鉴新加坡中央公积金制度而设立，是一项住房保障安排。长期以来，公积金主要由单位及在职职工缴存，资金主要用于购房、租房；此次修订首次允许灵活就业人员自愿缴存，并将装修、物业费等也纳入可提取范围。

**「影响」** 若最终通过，灵活就业人员及新市民、青年人可更灵活使用公积金，装修、物业费等住房消费压力有望缓解；目前仍处征求意见阶段，具体以正式条例为准。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.sciencedirect.com/science/article/abs/pii/S0313592625002553">Effect of the Housing Provident Fund on urban housing prices in China: A dual perspective of spatial heterogeneity and nonlinear linkages - ScienceDirect</a></li>

</ul>
</details>

**标签**: `#housing-policy`, `#china-economy`, `#provident-fund`, `#regulation`, `#consumption`

---

<a id="item-finance-news-3"></a>
### [深圳电动车违法正式纳入征信，宝安已录入 50 人](https://news.qq.com/rain/a/20260801A0BXUV00) ⭐️ 7.0/10

深圳已正式将电动自行车交通违法纳入个人征信，一年内被罚款 5 次以上或一年内 3 次以上违法未处理者，违法信息将被推送至征信机构；目前宝安区已录入 50 名骑行市民的信息。

telegram · zaihuapd · 8月2日 09:02

**「背景」** 依据《深圳经济特区道路交通安全违法行为处罚条例》，深圳交警自 2026 年 7 月起开展“雷霆护航”专项行动，重点查处冲禁令、走机动车道、闯红灯、逆行、违规载人等六类违法，闯红灯罚款 300 元，走机动车道、人行道或逆行罚款 50 元。

**「影响」** 对深圳电动自行车骑行者而言，频繁违章或长期不处理违法将直接影响个人信用记录；宝安区已试点通过“深圳交警”微信公众号在线处理电子监控抓拍的违法。

**标签**: `#personal-credit`, `#policy`, `#shenzhen`, `#traffic-violations`, `#e-bikes`

---

<a id="item-finance-news-4"></a>
### [日美联合干预汇市阻止日元跌至近 40 年低点](https://www.zaobao.com.sg/news/world/story20260802-9457369) ⭐️ 7.0/10

日本财务大臣预计 8 月 3 日宣布，日本与美国已联合干预外汇市场以支撑日元；市场消息称当局近期多次买入日元，美国财长便签显示拟买入 50 亿至 100 亿美元。日元兑美元一度逼近 164，创 1986 年以来最低。

telegram · zaihuapd · 8月3日 01:29

**「背景」** 日元跌至近 40 年低点时，美国罕见参与联合干预，意在提高行动效力、遏制市场做空预期并防范全球金融波动。

**「影响」** 对外汇市场而言，联合干预可能短期内加剧波动；但经济学家普遍认为，仅靠干预难以扭转日元长期贬值趋势，后续仍取决于日本经济基本面与货币政策走向。

**标签**: `#currency intervention`, `#yen exchange rate`, `#forex market`, `#Japan-US coordination`, `#monetary policy`

---