---
layout: default
title: "Horizon Summary: 2026-08-05 (ZH)"
date: 2026-08-05
lang: zh
---

> 从 46 条内容中筛选出 17 条重要资讯。

---

**科技新闻**
1. [Keyv 等 npm 包遭 Shai-Hulud 供应链攻击](#item-tech-news-1) ⭐️ 8.0/10
2. [中国发布首部 L3/L4 自动驾驶强制性国标，2027 年 7 月实施](#item-tech-news-2) ⭐️ 8.0/10
3. [Mistral 发布 3B 开源多模态审核模型 Shieldstral](#item-tech-news-3) ⭐️ 7.0/10
4. [Waymo 在达拉斯全面开放无人驾驶出租车服务](#item-tech-news-4) ⭐️ 7.0/10
5. [单块 AMD MI300X 运行 DeepSeek V4 Flash：以上下文换单卡](#item-tech-news-5) ⭐️ 7.0/10
6. [感谢联邦快递：我们为何不断被钓鱼](#item-tech-news-6) ⭐️ 7.0/10
7. [Oxide Computer 提交 SEC 表格 D，融资 4.45 亿美元](#item-tech-news-7) ⭐️ 7.0/10
8. [MiniMax-H3 MLX 移植版在 Apple Silicon 上本地生成 15 秒视频](#item-tech-news-8) ⭐️ 7.0/10
9. [三大 PC 厂开始采用长鑫存储芯片](#item-tech-news-9) ⭐️ 7.0/10
10. [Cloudflare 以每月 58 美元 AI 处理漏洞赏金](#item-tech-news-10) ⭐️ 7.0/10
11. [美拟禁中国光模块进口](#item-tech-news-11) ⭐️ 7.0/10

**财经新闻**
1. [Polymarket 洽谈超 200 亿美元估值融资](#item-finance-news-1) ⭐️ 8.0/10
2. [高盛交易员有望创年度纪录：第二季度股票业务收入激增 72%](#item-finance-news-2) ⭐️ 8.0/10
3. [谷歌被曝为 Anthropic 搭建约 2000 亿美元 AI 芯片融资架构](#item-finance-news-3) ⭐️ 8.0/10
4. [财报引发美股盘后个股大幅波动](#item-finance-news-4) ⭐️ 7.0/10
5. [财报驱动美股盘前异动：Palantir 大涨 15%，卡特彼勒超预期](#item-finance-news-5) ⭐️ 7.0/10
6. [白宫开源 AI 监管立场反复，拟推发布前网络安全审查](#item-finance-news-6) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Keyv 等 npm 包遭 Shai-Hulud 供应链攻击](https://www.aikido.dev/blog/keyv-and-friends-compromised-in-npm-supply-chain-attack) ⭐️ 8.0/10

一场名为 Shai-Hulud 的活跃供应链攻击已入侵 Keyv 及相关 npm 包，攻击者通过被篡改的依赖或安装钩子在安装时执行恶意代码，可能窃取凭据、植入后门，并作为蠕虫继续扩散。由于 Keyv 是广泛使用的缓存库，影响波及大量依赖它的 JavaScript 和 Node.js 项目。开发者应立即审查依赖锁定文件、检查新增的 install 脚本，并在确认安全前暂停升级或使用隔离环境。社区强调需对新增的 pre-install/post-install hooks 保持高度警惕，并考虑限制此类安装时脚本机制。

hackernews · cimi\_ · 8月4日 11:01 · [社区讨论](https://news.ycombinator.com/item?id=49166874)

**「背景」** Keyv 是一个在 npm 上每周被下载约 1.27 亿次的流行键值存储库，其维护者的 GitHub 账户在 2026 年 8 月 4 日遭到入侵，攻击者借此向 Keyv 及其八个相关 npm 包注入了名为“Shai-Hulud”的恶意代码。该恶意软件能够从受影响的 Node.js 应用程序中窃取环境变量和密钥等敏感信息。这类供应链攻击之所以危险，是因为开发者往往在安装依赖时自动执行安装前或安装后脚本，而恶意包正是利用这些钩子（hooks）在用户不知情的情况下运行恶意负载。

**「影响」** 使用 Keyv 及其受影响依赖的 npm 项目在安装或更新包时可能已被植入恶意代码，开发者应尽快审计依赖树和安装脚本，并留意 GitHub 等平台上的可疑数据外传仓库。

**「社区讨论」** 评论中有人推荐使用 Packj 等静态和动态行为分析工具来检测供应链攻击，也有人呼吁暂停或禁止新增安装钩子，并建议开发者采用 devcontainers 等隔离环境降低风险；同时有观点指出当前依赖系统本身非常脆弱，即使原始问题被清理，后续仍可能面临大量二次利用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.aikido.dev/blog/keyv-and-friends-compromised-in-npm-supply-chain-attack">Keyv and friends compromised in npm supply chain attack</a></li>
<li><a href="https://dev.to/onsen/keyv-supply-chain-attack-what-you-need-to-know-now-1466">Keyv Supply Chain Attack : What You Need to... - DEV Community</a></li>
<li><a href="https://cybersecuritynews.com/keyv-npm-package-compromised/">Keyv npm Package With 127 Million Weekly Downloads...</a></li>

</ul>
</details>

**标签**: `#security`, `#npm`, `#supply-chain`, `#javascript`, `#open-source`

---

<a id="item-tech-news-2"></a>
### [中国发布首部 L3/L4 自动驾驶强制性国标，2027 年 7 月实施](https://wap.miit.gov.cn/jgsj/zbys/qcgy/art/2026/art_a1d2072374884287b67048a77560014e.html) ⭐️ 8.0/10

工业和信息化部组织制定的《智能网联汽车 自动驾驶系统安全要求》（GB 44721—2026）强制性国家标准已获批发布，将于 2027 年 7 月 1 日起实施。这是我国首部针对 L3 级有条件自动驾驶和 L4 级高度自动驾驶系统的强制性国标，适用于搭载 L3/L4 系统的 M 类载客车辆和 N 类载货车辆，但不适用于自动泊车系统。该标准将 2024 年推荐性国标升级为强制性，从企业全生命周期安全保障、系统动态驾驶能力、人机交互与用户告知、多维度检验检测四个维度构建安全要求体系，并要求自动驾驶系统安全水平至少达到合格且专注驾驶人的水平。这标志着中国自动驾驶监管从推荐性走向强制性，为产业规模化部署明确了底线安全要求。

telegram · zaihuapd · 8月4日 13:06

**「背景」** L3 级有条件自动驾驶和 L4 级高度自动驾驶是国际自动机工程师学会（SAE）定义的驾驶自动化分级；L3 在特定条件下由系统执行全部动态驾驶任务但驾驶员需随时接管，L4 在限定场景内无需驾驶员接管。此前中国仅有 2024 年发布的推荐性国标，汽车企业可自愿参照，此次转为强制性国标，意味着满足安全要求成为在中国市场生产和上市相关车辆的前置条件。

**「影响」** 对计划在中国生产或进口 L3/L4 级载客与载货车辆的企业而言，该标准将使其自动驾驶系统的设计、测试和量产必须满足强制性安全基线，包括达到合格且专注驾驶人的驾驶水平；至 2027 年实施前，企业需完成标准差距分析和产品适配。

**标签**: `#autonomous-driving`, `#regulation`, `#China`, `#AI-safety`, `#standards`

---

<a id="item-tech-news-3"></a>
### [Mistral 发布 3B 开源多模态审核模型 Shieldstral](https://mistral.ai/news/shieldstral/) ⭐️ 7.0/10

Mistral 发布了 Shieldstral，一个 3B 参数、开放权重的多模态内容审核模型，专门面向 AI 安全与内容审核场景。该模型采用微调路线，主打低成本和高效率，适合部署在社交平台或图像分享等需要审核的内容链路中。由于权重开放，开发者可以自托管使用，将其作为审核的第一道防线，再配合人工复核处理敏感判断。此举延续了 Mistral 聚焦较小、更垂直模型的新策略，为内容审核基础设施提供了更可控的选项。

hackernews · riadsila · 8月4日 16:36 · [社区讨论](https://news.ycombinator.com/item?id=49171268)

**「背景」** Shieldstral 是 Mistral AI 于 2026 年 8 月 4 日发布的一个 3B 参数开放权重多模态安全分类器，用于对文本和图像进行内容审核。它的关键特点是“策略自适应”：审核策略可以用自然语言描述，并在推理时动态传入，无需重新训练即可调整审核规则。这类模型通常用于替代传统的内容审核 API 或大型专有护栏模型，一个 3B 模型即可在消费级 GPU 上运行，同时宣称在文本安全任务上可媲美比它大 7 倍的模型，并在多模态审核上达到新的最优水平。

**「影响」** 对于希望自建或自托管内容审核能力的开发者和社区平台，Shieldstral 提供了一个无需依赖大型专有 API 的 3B 开放权重方案；不过由于非确定性模型特性，通常仍需人工复核或与确定性规则配合。

**「社区讨论」** 评论中有人询问它能否按任意规则集灵活校准，还是仅复刻现有大平台的一种审核风格；也有人肯定 Mistral 转向更小、更垂直微调模型的做法，并认为这类开放模型有助于降低内容审核成本，但需注意不能完全依赖非确定性输出，应保留人工审核。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mistral.ai/news/shieldstral/">Introducing Shieldstral. | Mistral AI</a></li>
<li><a href="https://aiweekly.co/alerts/mistral-open-sources-shieldstral-a-3b-multimodal-safety-guard">Mistral open-sources Shieldstral, a 3B multimodal safety ...</a></li>
<li><a href="https://www.unite.ai/mistrals-shieldstral-packs-policy-adaptive-safety-screening-into-3b-parameters/">Mistral’s Shieldstral Packs Policy-Adaptive Safety Screening ...</a></li>

</ul>
</details>

**标签**: `#Mistral`, `#content moderation`, `#open-weights`, `#AI safety`, `#multimodal`

---

<a id="item-tech-news-4"></a>
### [Waymo 在达拉斯全面开放无人驾驶出租车服务](https://waymo.com/blog/shorts/dallas-open-to-all/) ⭐️ 7.0/10

Waymo 宣布其无人驾驶出租车服务在达拉斯正式向所有用户开放，标志着这家公司在商业机器人出租车领域的又一次大规模扩张。达拉斯是典型的高扩散、低密度、汽车依赖型大都市，此前 Waymo 已在多个美国城市开展类似服务。此次开放的具体车队规模、服务区域和运营细节尚未公布，但社区反应多持欢迎态度，也有讨论关注其经济影响。这一部署是自动驾驶技术从试点走向日常商业运营的又一重要里程碑。

hackernews · xnx · 8月4日 18:29 · [社区讨论](https://news.ycombinator.com/item?id=49172836)

**「背景」** Waymo 是 Alphabet 旗下的自动驾驶公司，此前已在多个美国城市运营无人驾驶出租车服务，并逐步扩大商业化运营范围。Waymo 于 2025 年 7 月宣布将进入达拉斯，并与汽车租赁公司 Avis Budget Group 建立多年合作，由后者负责车队维护和停车基础设施等运营工作。该服务最初在 2026 年 2 月向等候名单用户开放，自那以来已服务近 15 万名乘客，如今正式向所有达拉斯居民和游客开放。

**「影响」** Waymo 于 2026 年 8 月 4 日向达拉斯所有人开放其无人驾驶出租车服务，取消了此前自今年 2 月商业上线以来实行的邀请制等待名单；自开放以来已有近 15 万名乘客通过兴趣名单体验过该服务，现在任何达拉斯用户都可直接下载 Waymo 应用叫车，这标志着该自动驾驶出行服务在达拉斯这一低密度、高扩张、以汽车为核心的大都会区进入全面商业化运营。

**「社区讨论」** 评论者普遍对 Waymo 车辆的道路表现表示认可，认为其比人类驾驶更可预测、事故更少。但也有观点担心 Waymo 把收入抽离本地经济，另有人将其视为达拉斯缺乏公共交通的城市的积极补充。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://waymo.com/blog/2025/07/our-next-city-dallas/">Introducing our next city: Dallas - waymo.com</a></li>
<li><a href="https://waymo.com/blog/shorts/dallas-open-to-all/">August 4, 2026 - From the road - Waymo</a></li>
<li><a href="https://tech.yahoo.com/transportation/articles/waymo-launch-autonomous-ride-hailing-224642342.html">Waymo to launch autonomous ride-hailing in Dallas next year</a></li>
<li><a href="https://techcrunch.com/2026/08/04/waymo-opens-up-robotaxi-service-in-dallas-to-everyone/">Waymo opens up robotaxi service in Dallas to everyone</a></li>
<li><a href="https://www.unite.ai/waymo-drops-the-dallas-waitlist-as-freeway-and-airport-testing-looms/">Waymo Drops the Dallas Waitlist as Freeway and Airport ...</a></li>

</ul>
</details>

**标签**: `#autonomous vehicles`, `#Waymo`, `#AI`, `#transportation`, `#industry expansion`

---

<a id="item-tech-news-5"></a>
### [单块 AMD MI300X 运行 DeepSeek V4 Flash：以上下文换单卡](https://github.com/ryanzhou/deepseek-v4-flash-mi300x) ⭐️ 7.0/10

GitHub 项目“DeepSeek V4 Flash on a Single AMD MI300X”展示了如何在单块 AMD MI300X（OAM 模块）上运行 DeepSeek V4 Flash。该项目通过缩短上下文长度来适配单卡显存，以换取单块 OAM 模块即可部署的能力。这种取舍属于实用工程优化而非重大突破，但为 MoE 大模型在 AMD 硬件上的推理提供了一份有价值的参考资料。需要指出的是，MI300X 是 OAM 模块，通常以 8 卡整机形式销售（成本约 25 万欧元），不能简单单独购买。

hackernews · zhoutong · 8月4日 10:00 · [社区讨论](https://news.ycombinator.com/item?id=49166386)

**「背景」** DeepSeek V4 Flash 是一个大型混合专家（MoE）模型，其 256 个专家权重原生采用 MXFP4 量化，因而内存需求相对可控。AMD MI300X 是高带宽内存加速器，通常以 8 卡 OAM 机箱形式提供，单块 OAM 模块的容量有限。该项目通过将上下文长度从 1M 压缩至 256k，成功在单个 MI300X 上运行该模型，并实现约 168.6 token/s 的单流解码速度。

**「影响」** 对希望用单块 AMD MI300X 做 DeepSeek V4 Flash 推理的工程师，该仓库提供了一条省去整机投入的可行路径，但必须接受上下文窗口缩短等限制。

**「社区讨论」** 评论区对项目整体持积极态度，但也提出几点保留：有用户质疑单块 MI300X 并不单独出售（通常是 8 卡整机），并推荐了显存 144GB 的 PCIe 形态 MI350P；还有用户指出同类方案 DwarfStar 未被列入先前工作。多数评论认为这种用上下文长度换显存的做法很实用，且推理速度可达 150 tokens/s 以上。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/ryanzhou/deepseek-v4-flash-mi300x">GitHub - ryanzhou/ deepseek - v 4 - flash - mi 300 x · GitHub</a></li>

</ul>
</details>

**标签**: `#deepseek-v4`, `#AMD-MI300X`, `#inference`, `#quantization`, `#hardware`

---

<a id="item-tech-news-6"></a>
### [感谢联邦快递：我们为何不断被钓鱼](https://www.troyhunt.com/thanks-fedex-this-is-why-we-keep-getting-phished/) ⭐️ 7.0/10

Troy Hunt 剖析了一封看似合法的 FedEx 钓鱼邮件，指出用户之所以反复上当，是因为发件人身份验证机制失效、域名使用混乱，让普通用户难以辨别真假。他强调仅靠安全意识教育无法解决这类系统性问题，企业在邮件认证和域名选择上的不规范做法直接助长了钓鱼攻击。文中还提到可信品牌与攻击者使用相同的基础设施和通知方式，进一步削弱了用户的鉴别能力。该分析来自安全领域知名专家，对关注邮件安全与可用性的工程师有警示价值。

hackernews · stymaar · 8月4日 21:09 · [社区讨论](https://news.ycombinator.com/item?id=49175192)

**「背景」** Troy Hunt 是安全网站 Have I Been Pwned 的创办人，长期研究数据泄露与钓鱼攻击。他在 2024 年的一篇文章中指出，FedEx 发出的多条短信和邮件在形式和域名上几乎与钓鱼消息无异，连他都只能通过 FedEx 官网上的客服电话来核实真伪。这折射出钓鱼难以防范的根本背景：合法企业可能使用可疑域名、发件验证不一致，用户很难仅凭邮件外观判断真假。后来在 2025 年，Hunt 本人也因钓鱼攻击泄露了约 1.6 万个邮件地址，进一步说明这类攻击的迷惑性。

**「影响」** 对普通用户和接收 FedEx、Google 等品牌邮件的用户来说，合法通知与钓鱼邮件在技术上难以区分，导致即使警惕性高的人也可能会点击恶意链接或提交个人信息。

**「社区讨论」** 评论区用户分享了类似经历：有人收到 FedEx 客服个人邮箱发来的真实海关通知，有人发现 Google 官方链接使用的 c.gle 域名无法通过常规 whois 查询验证；还有人指出新通用顶级域泛滥和 IRS 电话语音系统与诈骗电话相同，让非技术用户更难识别诈骗。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.troyhunt.com/thanks-fedex-this-is-why-we-keep-getting-phished/">Troy Hunt: Thanks FedEx, This is Why we Keep Getting Phished</a></li>
<li><a href="https://www.techlicious.com/blog/how-troy-hunt-got-phished-and-why-2fa-did-not-save-him/">How Security Expert Troy Hunt Got Phished—and Why 2FA Didn’t Save Him - Techlicious</a></li>

</ul>
</details>

**标签**: `#phishing`, `#security`, `#email`, `#usability`, `#FedEx`

---

<a id="item-tech-news-7"></a>
### [Oxide Computer 提交 SEC 表格 D，融资 4.45 亿美元](https://www.sec.gov/Archives/edgar/data/1795071/000179507126000002/xslFormDX01/primary_doc.xml) ⭐️ 7.0/10

Oxide Computer 根据美国证券交易委员会的 Form D 文件披露了新一笔大规模融资，金额为 4.45 亿美元。该公司是开发机架级（rack-scale）计算系统的硬件创业公司，文件本身没有提供技术细节或产品进展。社区评论将这笔融资称为 D 轮，并列出其此前融资：2023 年 A 轮 4400 万美元、2025 年 B 轮 1 亿美元、2026 年 C 轮 2 亿美元。此轮融资额远超以往各轮，表明资本市场对机架级硬件方向保持高度兴趣，但 SEC 文件并未说明具体用途、估值或客户情况。

hackernews · depr · 8月4日 20:13 · [社区讨论](https://news.ycombinator.com/item?id=49174407)

**「背景」** Oxide Computer 是一家成立于 2019 年的公司，由前 Joyent 和 Sun Microsystems 工程师创立，总部位于加利福尼亚州埃默里维尔，主要销售机架规模的集成硬件和开源软件，将其定位为本地云替代方案。该公司此前已获得多轮融资：2023 年 A 轮 4400 万美元，2025 年 B 轮 1 亿美元，2026 年 2 月完成由 Thomas Tull 的 USIT 领投的 2 亿美元 C 轮融资。最新 SEC Form D 文件显示，Oxide 已披露一笔 4.45 亿美元的新融资，金额是其 C 轮的两倍多。

**「社区讨论」** 评论区情绪复杂：有人对 Oxide 及 Oxide and Friends 播客表示兴奋，也有人质疑公司是否真正出货硬件；一位自称工程副总裁的用户称去年提交销售表单后未获回应，目前每年在 AWS 花费约 90 万美元。另有评论表达对 Jessie Frazelle 参与项目的信任。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://aiweekly.co/alerts/oxide-computer-discloses-445m-funding-round-in-sec-form-d">Oxide Computer discloses $445M funding round in SEC Form D</a></li>
<li><a href="https://assets.theregister.com/2026/02/13/whats_next_for_oxide_computer/">Oxide plans new rack attack with Zen 5 CPUs, DDR5</a></li>

</ul>
</details>

**标签**: `#funding`, `#hardware`, `#Oxide Computer`, `#rack-scale`, `#tech industry`

---

<a id="item-tech-news-8"></a>
### [MiniMax-H3 MLX 移植版在 Apple Silicon 上本地生成 15 秒视频](https://simonwillison.net/2026/Aug/4/minimax-h3-mlx/#atom-everything) ⭐️ 7.0/10

MiniMax 于两天前发布了 MiniMax-H3，这是一个接受文本、图像、音频和视频输入的通用全模态生成系统，可生成最长 15 秒、带音频的视频片段。开源项目 PipeNetwork/minimax-h3-mlx 将该模型移植到 MLX，使其能在 Apple Silicon 上本地运行。Simon Willison 在 M5 Max MacBook Pro 上成功运行，下载了约 115 GB 模型文件，生成一个视频片段耗时近 45 分钟。他测试的提示词“a rainbow colored skunk leaps over a mossy log in a supermarket”生成的视频令人印象深刻，但由于未参考官方提示词指南，音频部分只是奇怪的类似语音的噪声。官方提供的视频提示词编写指南包含如何获得更好音频效果的大量说明。

rss · Simon Willison · 8月4日 19:10

**「背景」** MiniMax-H3 是一个“通用全模态生成系统”，这意味着它能统一处理文本、图像、音频和视频，并根据这些输入生成带音频的视频内容。MLX 是 Apple 的机器学习框架，允许在 Apple Silicon 芯片上高效运行模型；PipeNetwork 的移植让开发者无需专用服务器即可在本地 Mac 上体验这一视频生成能力，但代价是巨大的存储和计算资源开销。

**「影响」** 对于使用 Apple Silicon 的开发者与研究者，这个 MLX 移植提供了本地运行 MiniMax-H3 的可操作路径，但需要约 115 GB 存储和近 45 分钟的单次生成时间，因此实际使用时需评估资源成本。音频生成质量对提示词引导敏感，若未按官方指南编写提示词，可能得到不可用的音频结果。

**标签**: `#MiniMax-H3`, `#MLX`, `#Apple Silicon`, `#video generation`, `#omni-modal`

---

<a id="item-tech-news-9"></a>
### [三大 PC 厂开始采用长鑫存储芯片](https://asia.nikkei.com/business/china-tech/hp-asus-and-acer-begin-using-cxmt-chips-amid-memory-shortage) ⭐️ 7.0/10

在全球 AI 基础设施需求引发 DRAM 严重短缺的背景下，惠普、华硕和宏碁已开始少量采用中国长鑫存储的 DRAM 芯片，主要用于面向非美国市场的低端笔记本。知情人士称，三家厂商今年年中完成认证，但长鑫优先将大部分产能留给华为等中国客户，因此初期采用规模有限。PC 厂商刻意保持低调，以避免得罪合计占据全球九成以上份额的美光、三星和 SK 海力士；长鑫仍在五角大楼涉军企业名单上，使美国公司采购较为敏感。长鑫存储 7 月 27 日登陆科创板，首日大涨逾 465%，市值超 3.5 万亿元并超越英特尔；IDC 估计今年全球 PC 出货量或因存储短缺下滑超 11%。

telegram · zaihuapd · 8月4日 07:12

**「背景」** DRAM 即动态随机存取存储器，是个人电脑和服务器主要的短期存储芯片。全球市场长期由美光、三星和 SK 海力士把持，合计份额超过九成；长鑫存储是中国最主要的 DRAM 制造商，并被视为国产替代的关键企业。在美中科技竞争加剧和内存短缺的当下，主流 PC 厂商开始认证和采用其产品，标志着供应格局出现边际变化。

**「影响」** 最直接的后果是长鑫存储开始进入惠普、华硕、宏碁的非美国低端笔记本供应链，但初期采用有限；IDC 预计今年全球 PC 出货量或因存储短缺下滑超 11%，表明供应紧张对行业的冲击仍大于这批替代订单的缓解作用。

**标签**: `#DRAM`, `#semiconductors`, `#supply chain`, `#China tech`, `#PC industry`

---

<a id="item-tech-news-10"></a>
### [Cloudflare 以每月 58 美元 AI 处理漏洞赏金](https://www.theregister.com/security/2026/08/04/cloudflare-has-mostly-ditched-third-party-security-tools-suggests-not-trying-that-at-home/5282600) ⭐️ 7.0/10

据 The Register 报道，Cloudflare 首席安全官 Grant Bourzikas 在悉尼表示，公司已用 Anthropic 的 Claude Sonnet 模型自动化漏洞赏金报告的去重和评估，费用约每月 58 美元；若改用安全专用模型 Mythos，相同工作约需 20 万美元。该公司还构建了 200 多个自主安全代理，几乎弃用全部第三方安全工具，转而使用部分由 AI 辅助编写的自研应用。Bourzikas 同时建议其他企业不要效仿，称并非每家银行都应自行开发所有安全软件。首席战略官 Stephanie Cohen 称 AI 将根本改变厂商与客户的合作模式，并将公司此前裁员 1100 人归因于 AI 带来的自动化变革；她还透露 Cloudflare 正计划充当 AI 公司与出版商之间的中介，通过微支付让 AI 公司为内容付费。

telegram · zaihuapd · 8月4日 09:24

**「背景」** 漏洞赏金计划是安全厂商通过悬赏鼓励外部研究人员提交漏洞，再由内部团队验证、去重并评估严重性的机制。传统上，该流程依赖人工和多种第三方安全工具；Cloudflare 的做法是用通用大模型替代部分人工与工具，并转向自研安全应用。

**「影响」** 对于依赖大量第三方安全工具的企业，这一案例表明通用大模型可能显著降低漏洞初审成本，但 Cloudflare 高管也明确警告，其自研能力和规模并不适合普遍照搬。

**标签**: `#AI security`, `#Cloudflare`, `#bug bounty`, `#LLM automation`, `#security operations`

---

<a id="item-tech-news-11"></a>
### [美拟禁中国光模块进口](https://www.reuters.com/world/trump-administration-drafting-ban-chinese-data-center-devices-sources-say-2026-08-04/) ⭐️ 7.0/10

特朗普政府据知情人士透露正在起草一项禁令，拟禁止进口新型中国数据中心组件，重点针对光模块，以保护支撑 AI 热潮的关键基础设施。美国联邦通信委员会（FCC）正推进该措施，官员希望今年内发布并生效，但目前禁令仍可能修改或搁置。此举旨在防止中方窃取数据、植入恶意软件或中断服务，中国驻美使馆则回应称将对损害中国利益的行为采取一切必要措施。若禁令实施，将冲击全球光模块龙头中际旭创，该公司占据市场份额约 27%。此前 FCC 已陆续对中国无人机、路由器、机器人和逆变器实施类似进口限制。

telegram · zaihuapd · 8月4日 11:29

**「背景」** 光模块是数据中心内实现高速光信号传输的关键组件，尤其为人工智能训练和推理所需的算力集群提供内部互联。此前美国联邦通信委员会（FCC）已陆续对中国无人机、路由器、机器人和逆变器实施进口限制；此次拟议的禁令将限制范围扩展至新型数据中心组件，重点针对中国光模块。全球光模块龙头中际旭创占据约 27%市场份额，因此该政策若落地，可能显著影响 AI 基础设施供应链。

**「影响」** 若禁令最终落地，将直接影响占全球数据中心光模块约 60%收入的中国厂商（如中际旭创、新易盛、光迅科技等），迫使美国超大规模云厂商重新调整 AI 基础设施供应链，并为 Coherent、Lumentum 等西方竞争者创造替代机会；但该措施尚未最终敲定，仍可能修改或搁置。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.theguardian.com/technology/2026/aug/04/fcc-ban-china-datacenter-devices">Trump administration reportedly drafting ban on Chinese datacenter components | Technology | The Guardian</a></li>
<li><a href="https://www.newsnationnow.com/business/tech/fcc-ban-chinese-data-center-components/">Report: FCC considering ban on Chinese data center components</a></li>
<li><a href="https://www.dailymail.com/news/article-16028817/trump-fcc-ban-chinese-data-center-parts.html">The terrifying truth behind Trump&#x27;s ban on Chinese data center parts spreading across the US | Daily Mail Online</a></li>
<li><a href="https://www.emsnow.com/fcc-proposed-import-ban-on-chinese-optical-transceivers-implications-for-us-hyperscalers-chinese-suppliers-and-global-ai-infrastructure">FCC Proposed Import Ban on Chinese Optical Transceivers: Implications for US Hyperscalers, Chinese Suppliers, and Global AI Infrastructure · EMSNow</a></li>
<li><a href="https://finance.yahoo.com/markets/stocks/articles/optical-component-stocks-rally-proposed-113406255.html">Optical component stocks rally on proposed U.S. ban on Chinese tech</a></li>

</ul>
</details>

**标签**: `#US-China tech policy`, `#optical modules`, `#AI infrastructure`, `#supply chain`, `#regulation`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [Polymarket 洽谈超 200 亿美元估值融资](https://www.cnbc.com/2026/08/04/polymarket-seeks-fundraising-round-at-more-than-20-billion-valuation.html) ⭐️ 8.0/10

预测市场平台 Polymarket 正在洽谈以超过 200 亿美元的估值进行新一轮融资，知情人士向 CNBC 证实了相关谈判；该公司 6 月底表示年化营收远高于 10 亿美元，此前 4 月一轮融资估值为 150 亿美元。

rss · CNBC Finance · 8月4日 13:31

**「背景」** Polymarket 是预测市场平台，今年 5 月推出了受监管的美国交易所；其主要竞争对手 Kalshi 今年 5 月完成融资，估值为 220 亿美元。

**标签**: `#Polymarket`, `#fundraising`, `#valuation`, `#prediction markets`, `#private markets`

---

<a id="item-finance-news-2"></a>
### [高盛交易员有望创年度纪录：第二季度股票业务收入激增 72%](https://www.cnbc.com/2026/08/01/goldman-traders-are-on-pace-for-a-record-year-a-close-up-look-at-how-theyre-doing-it.html) ⭐️ 8.0/10

高盛交易部门有望创下年度交易收入纪录，其第二季度股票业务收入较上年同期增长 72%，达到创纪录的 74.2 亿美元；同期投行业务收入增长 55%至 34 亿美元。

rss · CNBC Finance · 8月4日 19:38

**「背景」** 高盛近年来持续投入并调整其全球银行与市场部门策略，希望借助投行和财富管理业务吸引客户使用其股票交易服务；该部门第二季度收入为 155 亿美元，占全行总收入的 75%以上。

**标签**: `#Goldman Sachs`, `#equities trading`, `#Q2 earnings`, `#capital markets`, `#trading revenue`

---

<a id="item-finance-news-3"></a>
### [谷歌被曝为 Anthropic 搭建约 2000 亿美元 AI 芯片融资架构](https://www.ft.com/content/549f2e23-5aa2-49c7-9ea6-a9784ab7087c) ⭐️ 8.0/10

《金融时报》调查报道，谷歌为人工智能公司 Anthropic 搭建了总额约 2000 亿美元的华尔街融资架构，其中约八成与 AI 芯片直接挂钩；今年 6 月，一个为这次融资专设的特殊目的载体已完成约 350 亿美元的首批硬件交易。

telegram · zaihuapd · 8月4日 10:52

**「背景」** 据《金融时报》调查，谷歌正与博通、阿波罗、黑石、摩根士丹利等机构搭建约 2000 亿美元的融资架构，以向 Anthropic 交付超过 1500 亿美元的 AI 芯片。由于 Anthropic 没有信用评级，各方通过特殊目的载体分担风险，并将购入的硬件回租给 Anthropic。

**「影响」** 报道称，这种安排借鉴波音和 GE 的厂商融资模式，让谷歌、博通、阿波罗、黑石等参与方不必把数百亿美元 AI 硬件压在资产负债表上，也使没有信用评级的 Anthropic 仍能大规模获得算力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://the-decoder.com/google-moves-billions-in-anthropic-chip-risk-off-its-balance-sheet/">Google moves billions in Anthropic chip risk off its balance sheet</a></li>

</ul>
</details>

**标签**: `#AI`, `#financing`, `#Google`, `#Anthropic`, `#infrastructure`

---

<a id="item-finance-news-4"></a>
### [财报引发美股盘后个股大幅波动](https://www.cnbc.com/2026/08/04/stocks-making-the-biggest-moves-after-the-bell-spcx-amd-pins-anet-wynn.html) ⭐️ 7.0/10

美股盘后，多家公司因最新财报和业绩指引大幅波动：Arista Networks 经调整每股收益 1.02 美元、营收 30.4 亿美元，均高于市场预期，股价上涨 11%；AMD 经调整每股收益 1.66 美元、营收 115.4 亿美元，略超预期但投资者仍失望，股价下跌 8%。SpaceX 上市后首份季度报告显示二季度营收 78.1 亿美元、高于预期，但资本开支达 183.7 亿美元、同比增 550%，股价下跌 7%；Pinterest 因三季度收入指引处于预期区间而下跌 8%。

rss · CNBC Finance · 8月4日 22:25

**「背景」** 这些波动发生在财报季盘后交易中，投资者将公司实际业绩与分析师共识预期（如 LSEG、FactSet）对比后调整仓位，业绩和指引是短期股价变动的主要驱动因素。

**标签**: `#earnings`, `#after-hours trading`, `#stock movers`, `#technology`, `#guidance`

---

<a id="item-finance-news-5"></a>
### [财报驱动美股盘前异动：Palantir 大涨 15%，卡特彼勒超预期](https://www.cnbc.com/2026/08/04/stocks-making-the-biggest-moves-premarket-mcd-cat-pltr-mrk.html) ⭐️ 7.0/10

美股盘前，多只股票因财报大幅波动：Palantir 二季度美国商业收入激增近 150%，股价大涨 15%；卡特彼勒调整后每股收益 8.17 美元，远超分析师预期的 6.20 美元，股价上涨 8%。

rss · CNBC Finance · 8月4日 11:42

**「背景」** 这是财报季常见的盘前行情，公司发布季度业绩和全年指引后，投资者通过交易即时消化消息；调整后每股收益通常剔除一次性项目，以便与分析师预期直接比较。

**标签**: `#Earnings`, `#Premarket Movers`, `#Pharmaceuticals`, `#Semiconductors`, `#Industrial Sector`

---

<a id="item-finance-news-6"></a>
### [白宫开源 AI 监管立场反复，拟推发布前网络安全审查](https://www.nytimes.com/2026/08/04/technology/ai-washington-regulation-whiplash.html) ⭐️ 7.0/10

白宫对开源 AI 监管出现政策摇摆。据知情人士称，白宫曾考虑制裁中国开源 AI 模型，后在硅谷反对下转向提升美国 AI 竞争力；8 月 4 日邀科技公司商议新框架，拟在模型发布前审查网络安全。

telegram · zaihuapd · 8月4日 15:22

**「背景」** 导火索是中国开源模型 Kimi 部分性能比肩 OpenAI 顶级模型；硅谷企业立场分裂，OpenAI 与 Anthropic 以国家安全为由推动限制中国对手，Nvidia、Meta 等支持开放生态。

**「影响」** 若该框架落地，发布开源大模型的企业可能需要先通过网络安全审查才能发布模型。

**标签**: `#AI监管`, `#开源AI`, `#白宫政策`, `#硅谷`, `#网络安全`

---