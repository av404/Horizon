---
layout: default
title: "Horizon Summary: 2026-09-25 (ZH)"
date: 2026-09-25
lang: zh
---

> 从 41 条内容中筛选出 12 条重要资讯。

---

**科技新闻**
1. [F-Droid 2.0 发布：十年来最大更新](#item-tech-news-1) ⭐️ 8.0/10
2. [英国双层加密与 Apple 停用 ADP](#item-tech-news-2) ⭐️ 8.0/10
3. [arXiv 获 1720 万美元多年期慈善资助，启动独立非营利运作](#item-tech-news-3) ⭐️ 7.0/10
4. [Claude Code 云会话正式上线，Pro/Max 可领最高 250 美元额度](#item-tech-news-4) ⭐️ 7.0/10
5. [OpenAI 发布心理健康基准 MentalHealthBench](#item-tech-news-5) ⭐️ 7.0/10

**财经新闻**
1. [中国确认美中首次 AI 会谈 提及延长贸易休战](#item-finance-news-1) ⭐️ 8.0/10
2. [北京发布商品房预售新政：封顶方可预售](#item-finance-news-2) ⭐️ 8.0/10
3. [费城联储保尔森：为压低通胀，未来或需“小幅”加息](#item-finance-news-3) ⭐️ 7.0/10
4. [中美贸易休战延长两个月至 1 月 10 日](#item-finance-news-4) ⭐️ 7.0/10
5. [特朗普与习近平会晤前瞻：中国自给自足如何改变贸易盘算](#item-finance-news-5) ⭐️ 7.0/10
6. [DeepSeek 年化营收据称破 10 亿美元，同步推进 500 亿元融资与上市筹备](#item-finance-news-6) ⭐️ 7.0/10
7. [三大运营商暂停金融分期购机新业务](#item-finance-news-7) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [F-Droid 2.0 发布：十年来最大更新](https://f-droid.org/2026/09/24/f-droid-2.0-a-new-chapter-for-android-freedom.html) ⭐️ 8.0/10

F-Droid 于 2026 年 9 月 24 日发布 2.0 版本，官方称这是其十年来最大的一次更新，界面与底层代码均被重做。新版把界面简化为“发现、搜索、我的应用”三大区域，改进应用发现、分类、搜索与筛选，支持检索应用描述、分类及翻译内容，并加强中日韩文字搜索，同时带来更顺畅的安装更新流程和后台检查更新。该版本将在未来数周陆续推送，此前已经过 14 次测试发布。新版暂不支持 F-Droid 特权扩展（FPE），并放弃对 Android 6 的支持。

hackernews · daveoc64 · 9月24日 15:26 · [社区讨论](https://news.ycombinator.com/item?id=49831968)

**「背景」** F-Droid 是 Android 平台上的自由与开源软件（FOSS）应用仓库及官方客户端，用户可通过它从多个独立仓库浏览、安装和更新开源应用，其分发方式独立于 Google Play。F-Droid Privileged Extension 是一个需要系统级权限（通常配合定制 ROM 或 root 使用）的扩展组件，用于让 F-Droid 无需用户逐次确认即可静默安装和更新应用，但配置与稳定运行一直较为麻烦。据此次发布信息，F-Droid 2.0 是该官方应用约十年来最大的一次更新。

**「影响」** 对现有用户而言，最直接的后果是：Android 6 及更早版本的设备将不再获得支持，而依赖 F-Droid Privileged Extension 实现免确认后台安装与更新的用户需暂时回到手动确认安装的方式，直至该扩展重新适配。与此同时，Google 计划于 2026 年推进的开发者注册与侧载限制，使 F-Droid 这类第三方应用商店未来能否继续正常分发应用存在不确定性，社区因此呼吁更多人安装并反馈意见。

**「社区讨论」** 评论中既有欢迎也有批评：有用户表示自己多年因 F-Droid 界面糟糕、特权扩展难以配置而转用 GrapheneOS 上的 Droid-ify，对这次大改以及 FPE 被淘汰表示欢迎。也有人批评新设计未在界面各区块之间画出明确分界，缺乏可点击性提示，并指出首张截图中 “Syncthing-For k” 的换行错误；另有评论者追问在 Google 明年收紧生态限制后 F-Droid 的前景如何。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://factually.co/fact-checks/technology/android-developer-registration-fdroid-sideloading-availability-6fefe0">If Android Requires Developer Registration, Can Users ..</a></li>
<li><a href="https://keepandroidopen.org/cta/">Advocating for Android as a free, open platform for everyone to build...</a></li>

</ul>
</details>

**标签**: `#Android`, `#F-Droid`, `#open-source`, `#app-distribution`, `#UI-redesign`

---

<a id="item-tech-news-2"></a>
### [英国双层加密与 Apple 停用 ADP](https://macanorak.com/two-tier-encryption-in-the-uk/) ⭐️ 8.0/10

一篇 Hacker News 文章讨论英国 iCloud 的“双层加密”现状：Apple 为应对英国法律要求而停止向英国用户提供高级数据保护（ADP）。评论引述文章称，英国撤回 ADP 并未影响原本默认端到端加密的 14 个 iCloud 类别，如 iCloud 钥匙串和健康数据；ADP 会把端到端加密类别从 14 个增加到 23 个。对没有 ADP 的英国用户，iCloud 备份、照片、备忘录、iCloud Drive 等额外类别回落到标准数据保护，Apple 持有密钥，可回应合法法律程序，只有基线类别仍保持端到端加密。文章称 Apple 面对要求其改变 ADP 所依赖安全架构的法律命令，选择停止提供该功能，从而在满足法律要求的同时避免构建后门。讨论关注这是否等于变相禁止端到端加密，以及 Apple 当前是否还愿意像 2015 年那样对抗政府要求。

hackernews · ReturnoftheHack · 9月24日 10:39 · [社区讨论](https://news.ycombinator.com/item?id=49828731)

**「背景」** 英国政府于 2025 年 1 月向苹果发出技术能力通知（TCN），要求其协助访问受端到端加密保护的 iCloud 数据。苹果没有按该命令构建加密后门，而是对英国用户停用“高级数据保护”（ADP），使这部分 iCloud 数据回退到由苹果持有密钥的标准数据保护。此举并未完全满足英方要求，而围绕该命令保密性的争议也已提交英国调查权力法庭（IPT）审理。

**「影响」** 对英国 iCloud 用户而言，被停用的 ADP 使备份、照片、笔记、iCloud Drive 等原本可端到端加密的类别退回标准数据保护，由苹果持有密钥并可在合法程序下提供数据，苹果称这会让用户更易遭受恶意攻击者的数据泄露。苹果已于 2026 年 8 月就该要求提起法律挑战，因此最终影响仍取决于诉讼结果。

**「社区讨论」** 评论区分歧集中在 Apple 是否仍有能力或意愿抵抗政府要求：有人批评其从 2015 年的强硬立场后退，并提到强制年龄确认和 KYC；也有人认为在不得披露的法律命令下，停用 ADP 是无奈但现实的选择，另有用户呼吁 Apple 退出英国市场或停止向英国政府提供服务。整体担忧是，这类秘密法律命令和英国加密政策正让端到端加密的实际保护范围收窄。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.kucoin.com/news/flash/apple-challenges-uk-s-demand-for-icloud-encryption-backdoor">Apple Challenges UK &#x27;s Demand for iCloud Encryption ... | KuCoin</a></li>
<li><a href="https://petapixel.com/2025/02/21/apple-removes-icloud-encryption-in-uk-after-secret-government-order/">Apple Removes iCloud Encryption in UK After Secret... | PetaPixel</a></li>
<li><a href="https://www.gadgetreview.com/uk-court-apple-icloud-backdoor-secrecy-called-farcical">UK Court: Apple iCloud Backdoor Secrecy Called... - Gadget Review</a></li>
<li><a href="https://www.theguardian.com/technology/2026/aug/03/apple-legal-challenge-uk-government-data-access">Apple launches legal challenge against UK government demand to access data | Apple | The Guardian</a></li>
<li><a href="https://androidexperto.com/apple-forced-to-kill-popular-security-feature-in-the-uk-heres-whats-happening/">Apple forced to kill popular security feature in the UK — he</a></li>
<li><a href="https://macdailynews.com/2026/08/03/apple-launches-legal-challenge-to-uk-demand-for-access-to-encrypted-user-data/">Apple launches legal challenge to UK demand for access to encrypted user data</a></li>

</ul>
</details>

**标签**: `#encryption`, `#apple`, `#uk-policy`, `#privacy`, `#icloud`

---

<a id="item-tech-news-3"></a>
### [arXiv 获 1720 万美元多年期慈善资助，启动独立非营利运作](https://www.reddit.com/r/MachineLearning/comments/1wox8kt/arxiv_receives_multiyear_philanthropic/) ⭐️ 7.0/10

arXiv 获得总额 1720 万美元的多年期慈善资助承诺，用于支持其作为独立非营利组织正式启动运作。这笔资金由 Simons Foundation International、XTX Markets 和 Siegel Family Endowment 提供，资助周期跨度为三到五年。相关消息由 arXiv 官方博客于 2026 年 9 月 23 日发布，Reddit 机器学习社区亦转发了该消息。arXiv 是机器学习与人工智能等领域研究者广泛依赖的预印本平台，此次转向独立非营利身份意味着其运营经费将从多年期机构捐赠中获得更稳定的支撑。目前公开信息仅为公告层面，未披露资金的具体用途分配、治理架构调整细节或长期筹款目标。

reddit · r/MachineLearning · /u/Nunki08 · 9月24日 09:43

**「背景」** arXiv 是由 Paul Ginsparg 创立的预印本论文存档平台，长期以来依托康奈尔大学运营；2010 年起它通过要求机构按下载量缴纳年度自愿会费、并承诺五年资助的模式拓宽资金来源，同时辅以会员计划、赞助商、附属机构和个人捐赠来维持可持续运营。此次出资方之一的 Simons Foundation 是由 Marilyn 与 Jim Simons 于 1994 年创立的美国私人基金会，2022 年资产规模超过 50 亿美元，宗旨是推动科学前沿。这一 1720 万美元的多年期承诺将用于强化技术基础设施、支持日常运营并改善面向全球研究者的服务，同时支撑 arXiv 向独立非营利机构过渡。

**「影响」** 对依赖 arXiv 的研究者而言，这笔 1720 万美元的多年期资助为其独立非营利转型提供了资金基础，使其能更灵活地筹资、加快技术开发并扩大合作，以应对持续增长的投稿压力（包括 AI 生成的低质投稿）。不过资金按三至五年分期投入，能否彻底缓解投稿洪水仍待观察。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Simons_Foundation">Simons Foundation - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/ArXiv">arXiv - Wikipedia</a></li>
<li><a href="https://runtimewire.com/article/arxiv-17-2m-nonprofit-transition">arXiv secures $17.2M in multiyear support for nonprofit ...</a></li>
<li><a href="https://blog.arxiv.org/2026/09/23/arxiv-receives-multiyear-investment/">arXiv receives 17.2 million multiyear investment</a></li>
<li><a href="https://www.reddit.com/r/MachineLearning/comments/1rzp5ph/n_arxiv_the_pioneering_preprint_server_declares/">r/MachineLearning on Reddit: [N] ArXiv, the pioneering preprint server, declares independence from Cornell | Science | As an independent nonprofit, it hopes to raise funds to cope with exploding submissions and “AI slop”</a></li>
<li><a href="https://info.arxiv.org/about/spinout_faq.html">arXiv is now an independent nonprofit - arXiv info</a></li>
<li><a href="https://blog.arxiv.org/2026/04/02/arxiv-is-becoming-an-independent-nonprofit/">arXiv is becoming an independent nonprofit – News from arXiv</a></li>

</ul>
</details>

**标签**: `#arXiv`, `#open science`, `#research infrastructure`, `#nonprofit funding`, `#machine learning`

---

<a id="item-tech-news-4"></a>
### [Claude Code 云会话正式上线，Pro/Max 可领最高 250 美元额度](https://code.claude.com/docs/en/claude-code-on-the-web) ⭐️ 7.0/10

Anthropic 的 Claude Code 云会话结束研究预览正式发布，面向 Pro、Max、Team 及 Enterprise 用户开放。用户合上笔记本后，任务仍可在云端继续运行，并可随时从浏览器、手机、桌面应用或终端查看和接管。现有订阅用户可领取一次性云会话体验额度：Pro 用户 100 美元、Max 用户 250 美元，额度仅限 Cloud sessions 使用，可在官方领取页登录领取，或在 Claude Code 中执行 /claim-credit。领取截止时间为太平洋时间 10 月 7 日 23:59，额度有效至 11 月 4 日 23:59；资格需登录后按账号及条款判定，并非所有用户均可领取，且 Anthropic 支持地区名单目前不含中国大陆、香港和澳门。

telegram · zaihuapd · 9月24日 02:45

**「背景」** Claude Code 是 Anthropic 面向开发者的 AI 编程工具，用户可以让它在终端等环境中代写、修改和运行代码，而云会话让同一任务在云端持续运行，并可从浏览器、手机、桌面应用或终端随时接管。该云会话能力此前以研究预览形式存在，本次转为正式可用（GA），成为 Pro、Max、Team 与 Enterprise 订阅的一项能力。作为上线配套，Anthropic 向现有订阅用户发放一次性云会话额度（Pro 100 美元、Max 250 美元）；外部报道显示该额度领取截止到 10 月 7 日，且试用期结束后的计费方式尚不明确。

**「影响」** 对 Pro、Max、Team 和 Enterprise 订阅用户而言，Claude Code 任务可在合上笔记本后继续在云端运行，并可从浏览器、手机、桌面应用或终端随时查看和接管，同时可领取一次性云端额度（Pro 100 美元、Max 250 美元）。但资格受地区与条款限制：Anthropic 支持地区名单目前不含中国大陆、香港和澳门，额度领取与有效期分别截至太平洋时间 10 月 7 日 23:59 和 11 月 4 日 23:59，是否符合条件需登录后按账号及条款判定。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://alphasignal.ai/news/anthropic-ships-claude-code-cloud-sessions-so-developers-can-code-without-a">Anthropic Ships Claude Code Cloud Sessions so Developers Can Code Without a Laptop | AlphaSignal</a></li>
<li><a href="https://explainx.ai/blog/claude-code-cloud-sessions-ga-100-250-credit-claim-credit-2026">Claude Code Cloud Sessions GA: Claim $100/$250 Credit | explainx.ai Blog | explainx.ai</a></li>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent , Terminal, IDE</a></li>

</ul>
</details>

**标签**: `#Claude Code`, `#Anthropic`, `#AI coding agents`, `#cloud sessions`, `#developer tools`

---

<a id="item-tech-news-5"></a>
### [OpenAI 发布心理健康基准 MentalHealthBench](https://openai.com/zh-Hans-CN/index/introducing-mentalhealthbench/) ⭐️ 7.0/10

OpenAI 发布了开放基准 MentalHealthBench，用于评估 AI 在真实心理健康对话中的回应。该基准由来自 22 个国家/地区的 80 多名持证心理健康专家共同制定，衡量 AI 在安全、收集背景信息、维护用户自主权和提供可行建议等方面的表现。其覆盖场景包括成人、青少年、照护者和临床人员。结果显示 AI 在应对心理健康问题方面取得稳步进展，但 OpenAI 强调 ChatGPT 不能替代专业治疗。

telegram · zaihuapd · 9月24日 06:00

**「背景」** MentalHealthBench 是 OpenAI 与来自 22 个国家的 80 多名持证心理健康专家共同制定的开放基准，用于评估 AI 在真实心理健康对话中的回应。它通过加权评分标准覆盖从日常压力到紧急情况的多种场景，填补了以往只关注危机干预评估的空白。这类基准的意义在于为 AI 在心理健康场景中的安全性、背景信息收集、用户自主权和可行建议等行为提供可比较的衡量方式。

**「影响」** 对开发心理健康相关 AI 产品的团队与机构而言，MentalHealthBench 提供了一个由 22 个国家 80 多名持证专家参与制定评分标准的开放基准，可用于在上线前评测模型在安全、背景信息收集、用户自主权和可行建议等方面的表现。由于该基准由 OpenAI 主导发布，目前尚缺独立验证与完整方法学细节，其评测结果宜作为参考依据而非专业治疗或合规的证明。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/introducing-mentalhealthbench/">Introducing MentalHealthBench | OpenAI</a></li>
<li><a href="https://contentbuffer.com/news/openai-mentalhealthbench-80-clinicians-grade-ai-replies-e6b8dffb">OpenAI MentalHealthBench : 80 + Clinicians... — ContentBuffer News</a></li>
<li><a href="https://www.techbooky.com/openai-mentalhealthbench-ai-chat-safety/">OpenAI MentalHealthBench Tests Mental Health AI</a></li>
<li><a href="https://ybuild.ai/en/blog/mentalhealthbench-sensitive-conversation-launch-gate-founders">MentalHealthBench Changes How Founders Should Test Sensitive AI ...</a></li>
<li><a href="https://openai.com/index/introducing-mentalhealthbench/">Introducing MentalHealthBench | OpenAI</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#LLM evaluation`, `#mental health`, `#benchmark`, `#OpenAI`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [中国确认美中首次 AI 会谈 提及延长贸易休战](https://www.cnbc.com/2026/09/24/china-confirms-first-ai-talks-with-us-have-taken-place-hints-at-trade-truce-extension.html) ⭐️ 8.0/10

中国商务部周四确认，美中高级贸易谈判代表首次就人工智能举行会谈，双方还讨论了削减关税以及延长去年 10 月在吉隆坡达成的贸易安排。美国财长贝森特称，两国已同意把贸易休战延长至 1 月，但具体条款尚未公布。

rss · CNBC Finance · 9月24日 14:16

**「背景」** 这项休战于 2025 年 10 月达成，原本降低了部分关税并限制了中国对稀土的出口管制；稀土是半导体、家电和国防产品的重要原料。此次确认发生在特朗普与习近平于华盛顿会晤前数小时，双方此前还讨论了建立 AI 对话和风险通报机制。

**「影响」** 按贝森特的说法，休战延长至 1 月意味着依赖较低关税和稀土稳定供应的半导体、家电及国防相关企业可暂时避免关税上调和出口管制收紧。

**标签**: `#US-China trade`, `#Artificial intelligence`, `#Tariffs`, `#Rare earths`, `#Trade truce`

---

<a id="item-finance-news-2"></a>
### [北京发布商品房预售新政：封顶方可预售](https://mp.weixin.qq.com/s/g-nwBAIGMCfuhENgs6o9-g) ⭐️ 8.0/10

9 月 24 日，北京发布落实商品住房销售制度改革的实施意见，规定 8 月 28 日后新出让地块的商品住房项目须主体结构封顶方可申请预售，并优先实行现房销售、预售资金全额全过程监管；新出让住宅用地出让价款可分期缴纳，首付款不低于总价 50%，余款两年内缴清且不计利息，银行须待项目竣工备案后才可发放个人住房按揭贷款。

telegram · zaihuapd · 9月24日 11:10

**「背景」** 中国商品房长期实行预售制，即购房者在项目尚未竣工时就先付款，开发商借此提前回笼资金，但也容易产生交付风险。北京此次把预售门槛提高到主体结构封顶，并优先推动现房销售，收紧的正是这一提前销售的通道（据新华社报道）。

**「影响」** 购房者的期房资金占用与烂尾风险敞口明显缩小，风险更多转向开发商和银行；对开发商而言回款周期被拉长，据媒体报道引用的中金公司测算，其自由现金流回正时间将从拿地后 1 年内延长至 2.5 到 3 年。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://m.21jingji.com/article/20260924/herald/689862331695d9635934bdf8b5b35515.html">北 京 ： 商 品 房 预 售 需 封 顶 优先选择 现 房 销 售 - 21财经</a></li>
<li><a href="https://www.163.com/dy/article/L7K8CGJN0519AFSG.html">封顶才准卖房，余款两年免息：北京新政很温柔|期房|预售|开发商|购房者|北京市|商品住房_网易订阅</a></li>
<li><a href="https://www.163.com/dy/article/L7KCJBLQ0535GP8A.html">重磅！北京现房销售细则落地，有什么利好什么利空？|期房|预售证|开发商|北京市|全年二手房均价_网易订阅</a></li>

</ul>
</details>

**标签**: `#China property policy`, `#Beijing real estate`, `#housing pre-sale reform`, `#developer cash flow`, `#mortgage lending`

---

<a id="item-finance-news-3"></a>
### [费城联储保尔森：为压低通胀，未来或需“小幅”加息](https://www.cnbc.com/2026/09/24/philadelphia-feds-anna-paulson-says-modest-rate-moves-likely-ahead-to-tame-inflation.html) ⭐️ 7.0/10

费城联储主席安娜·保尔森表示，如果情况按她的预期发展，可能需要“小幅”进一步收紧货币政策，才能把通胀拉回 2%的目标；一周前，美联储联邦公开市场委员会已将基准利率上调 0.25 个百分点，至 3.75%-4%的目标区间。

rss · CNBC Finance · 9月24日 17:12

**「背景」** 保尔森在 fintech 会议的讲稿中说，剔除能源和关税冲击后的基础通胀仍运行在约 2.5%-3%，“远高于”2%的目标，她对今年基础通胀“最好的评价是没有变得更糟”。

**「影响」** 与此同时，市场对进一步加息的预期明显升温：据芝商所 FedWatch 工具，交易员认为 10 月再次加息的概率为 64%，利率期货隐含 2027 年底利率约 4.8%，长端美国国债收益率升至 2004 年以来未见的高位，这对利率敏感的借款人和债券投资者构成压力。

**标签**: `#Monetary Policy`, `#Federal Reserve`, `#Inflation`, `#Interest Rates`, `#Treasury Yields`

---

<a id="item-finance-news-4"></a>
### [中美贸易休战延长两个月至 1 月 10 日](https://www.cnbc.com/2026/09/24/us-china-trade-truce-bessent-trump-xi.html) ⭐️ 7.0/10

美国财政部长贝森特表示，美中将贸易休战再延长两个月、至 1 月 10 日，其间继续维持较低关税并让稀土保持流通；该休战原定 11 月到期，是两位领导人在去年 10 月韩国会晤时达成的为期一年的安排。贝森特是在中国国家主席习近平抵达华盛顿开始国事访问之际、通过福克斯新闻作出上述表示的。

rss · CNBC Finance · 9月24日 04:55

**「背景」** 美中此前于去年 10 月在韩国举行的会晤中达成一项为期一年的贸易休战安排，双方同意降低部分关税并保持稀土供应，该安排原定于今年 11 月到期。据《纽约时报》和 The Money Centre 报道，此次将到期日延长至明年 1 月 10 日，即在原期限基础上再延长两个月。

**「影响」** 中国欧盟商会会长彦辞指出，仅延长休战并未解决企业面临的难题，包括稀土出口许可申请缺乏统一标准，这意味着在华欧洲企业等依赖稀土的厂商仍要面对许可流程上的不确定性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://themoneycentre.net/2026/09/24/u-s-china-trade-truce-extended-two-months-during-xis-visit/">U . S .- China Trade Truce Extended Two Months During Xi ’s Visit</a></li>
<li><a href="https://www.nytimes.com/2026/09/23/us/politics/china-trade-truce-tariffs.html">U . S . and China Agree to Extend Trade Truce by 2 Months, Bessent ...</a></li>

</ul>
</details>

**标签**: `#US-China trade`, `#tariffs`, `#rare earths`, `#trade policy`, `#diplomacy`

---

<a id="item-finance-news-5"></a>
### [特朗普与习近平会晤前瞻：中国自给自足如何改变贸易盘算](https://www.cnbc.com/2026/09/23/trump-xi-meeting-why-chinas-self-sufficiency-changes-the-calculus.html) ⭐️ 7.0/10

美国总统特朗普与中国国家主席习近平预计本周举行今年第二次面对面峰会，但商界对成果的预期仅限于延长去年秋天达成的贸易休战。据中国海关数据（经 Wind 资讯获取），4 月贸易紧张升级曾短暂将美国对华贸易逆差压至 2017 年以来最低，随后 AI 相关零部件需求又推动逆差今年重新扩大。

rss · CNBC Finance · 9月24日 01:44

**「背景」** 中国近年推动自给自足以降低外部贸易变化对国内市场的冲击，而 2022 年房地产下行后企业加速全球扩张和出口，全球对中国制成品的依赖不降反升。

**「影响」** 欧盟对华贸易逆差为全球最大，并正跟随美国加强对中国来源出口的审查，欧盟贸易专员要求中方 10 月前取得“切实成果”并预计下月访京，中国出口商可能面临更严的欧洲贸易措施。

**标签**: `#US-China trade`, `#Trump-Xi meeting`, `#China economy`, `#tariffs`, `#AI supply chain`

---

<a id="item-finance-news-6"></a>
### [DeepSeek 年化营收据称破 10 亿美元，同步推进 500 亿元融资与上市筹备](https://weibo.com/1642634100/RjAoNli86) ⭐️ 7.0/10

知情人士称，DeepSeek 的年化营收运行率已达 10 亿美元，数月前还不足 5 亿美元，增长主要来自上调 API 定价及大模型持续热捧，CEO 梁文锋在近期投资者会议上披露了这一数据。同一消息称，公司正推进第二轮融资，计划 10 月底前完成、目标募资 500 亿元人民币（约合 75 亿美元），估值目标 5000 亿元，并筹备在上海证券交易所上市，梁文锋表示调价未造成客户流失。上述数字与计划均来自未具名知情人士，尚未获公司官方确认。

telegram · zaihuapd · 9月24日 07:56

**「背景」** 年化营收运行率是把近期收入按全年速度折算的估算指标，DeepSeek 的这一数字数月前还不足 5 亿美元。公司在完成上一轮融资后正推进第二轮募资，目标募资 500 亿元人民币（约合 75 亿美元）、估值目标 5000 亿元人民币，并计划 10 月底前完成。

**「影响」** 使用 DeepSeek API 的开发者和企业用户将面临 API 调用成本上升；官方公告称调价仅针对 API 接口，官网网页端和 App 的免费聊天等服务不受影响，完整调价细则和生效时间尚未公布。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://m.cnmo.com/news/819333.html">曝 DeepSeek 完成75 亿 美 元 融 资 年 化 营 收 达 10 亿 美 元 _CNMO</a></li>
<li><a href="https://wallstreetcn.com/articles/3782443">报道： DeepSeek 年 化 营 收 突破 10 亿 美 元 ，计划在 10 ...</a></li>
<li><a href="https://m.163.com/dy/article/L7K0CTIK051180F7.html">DeepSeek 被曝冲刺 5000 亿 元 估 值 ！ 年 化 营 收 达67 亿 _手机网易网</a></li>
<li><a href="https://wenku.baidu.com/view/e150f5452679168884868762caaedd3383c4b5b7.html">DeepSeek API调价确认！2026年8月涨价公告解读与应对指南</a></li>
<li><a href="https://www.tmtpost.com/8094414.html">DeepSeek预告API涨价，AI低价红利落幕-钛媒体官方网站</a></li>

</ul>
</details>

**标签**: `#DeepSeek`, `#AI financing`, `#IPO`, `#revenue growth`, `#API pricing`

---

<a id="item-finance-news-7"></a>
### [三大运营商暂停金融分期购机新业务](https://finance.sina.com.cn/jjxw/2026-09-24/doc-inisxhnx5270778.shtml) ⭐️ 7.0/10

自 2026 年 9 月 24 日起，中国移动、中国电信、中国联通暂停金融分期购机业务的新受理，和包信用购、橙分期、沃分期等“0 元购机”业务全面停办，已办理老用户的分期合约继续生效。三大运营商客服已确认暂停，官方暂无正式回应，多称系产品升级，恢复时间未定。

telegram · zaihuapd · 9月24日 08:46

**「背景」** 此类“0 元购机”此前常被包装成“免费领手机”，实际是替用户办理分期贷款，因而长期是消费者投诉集中的领域。三家运营商客服已确认暂停新受理，但官方尚无正式回应，多称系产品升级，恢复时间未定。

**「影响」** 据凤凰网报道，分期业务暂停预计将对运营商线下营业厅的业绩造成一定影响；已办理分期购机合约的老用户不受影响，合约继续生效。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://linux.do/t/topic/2947089">三 大 运 营 商 暂 停 金 融 分 期 业务，“0 元 购 机 ”全面 停 办 - 前沿快讯 - LINUX...</a></li>
<li><a href="https://tech.ifeng.com/c/8wgLAZcg33a">“0元 购 机”凉了！ 移动电 信 联通三大运营商 分 期 业务全面 暂 停 _凤凰网</a></li>

</ul>
</details>

**标签**: `#China telecom`, `#consumer finance`, `#installment sales`, `#mobile phones`, `#product suspension`

---