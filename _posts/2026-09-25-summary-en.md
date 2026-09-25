---
layout: default
title: "Horizon Summary: 2026-09-25 (EN)"
date: 2026-09-25
lang: en
---

> From 41 items, 12 important content pieces were selected

---

**Technology News**
1. [F-Droid 2.0 Redesign Arrives With Privileged Extension Phase-Out](#item-tech-news-1) ⭐️ 8.0/10
2. [Apple Disables Advanced Data Protection in UK, Creating Two-Tier iCloud Encryption](#item-tech-news-2) ⭐️ 8.0/10
3. [arXiv secures $17.2M to support independent nonprofit launch](#item-tech-news-3) ⭐️ 7.0/10
4. [Claude Code cloud sessions launch with up to $250 credits](#item-tech-news-4) ⭐️ 7.0/10
5. [OpenAI Releases MentalHealthBench for Mental-Health AI Evaluation](#item-tech-news-5) ⭐️ 7.0/10

**Financial News**
1. [China confirms first AI talks with U.S., discusses tariff cuts and trade truce extension](#item-finance-news-1) ⭐️ 8.0/10
2. [Beijing Requires Topped-Out Structure Before Pre-Sale for New Land Plots](#item-finance-news-2) ⭐️ 8.0/10
3. [Philadelphia Fed&\#x27;s Paulson Says Modest Further Tightening May Be Needed](#item-finance-news-3) ⭐️ 7.0/10
4. [U.S.-China trade truce extended two months to Jan. 10 as Xi begins state visit](#item-finance-news-4) ⭐️ 7.0/10
5. [Ahead of Trump-Xi meeting, China&\#x27;s self-sufficiency reshapes trade calculus](#item-finance-news-5) ⭐️ 7.0/10
6. [DeepSeek Reported at $1B Annualized Revenue as It Plans RMB 50B Round and Shanghai Listing](#item-finance-news-6) ⭐️ 7.0/10
7. [China&\#x27;s three major telecom carriers suspend installment phone financing, including &quot;0 yuan phone&quot; offers](#item-finance-news-7) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [F-Droid 2.0 Redesign Arrives With Privileged Extension Phase-Out](https://f-droid.org/2026/09/24/f-droid-2.0-a-new-chapter-for-android-freedom.html) ⭐️ 8.0/10

F-Droid 2.0 was released on September 24, 2026 as the official app&\#x27;s biggest update in ten years, following 14 test releases, and it is rolling out over the coming weeks. The release redesigns both the interface and underlying code, simplifying navigation into Discover, Search, and My Apps. It improves app discovery, categories, search and filtering, including searching app descriptions, categories, and translated content, with stronger Chinese, Japanese, and Korean text search. F-Droid also adds smoother install and update flows and background update checks. The F-Droid Privileged Extension is not supported in this release, and Android 6 support has been dropped.

hackernews · daveoc64 · Sep 24, 15:26 · [Discussion](https://news.ycombinator.com/item?id=49831968)

**「Background」** F-Droid is a community-run, free and open-source Android app repository and client, serving as an alternative to proprietary app stores. Its Privileged Extension is an optional companion component that allows the client to install and update apps with elevated system permissions, often requiring special configuration on custom Android distributions. F-Droid 2.0, released on September 24, 2026 after 14 test releases, is the project&\#x27;s largest update in a decade; it rebuilds the interface and underlying code while dropping support for Android 6 and temporarily does not support the F-Droid Privileged Extension.

**「Impact」** Users who depended on the F-Droid Privileged Extension for unattended background installs, and any devices still on Android 6, lose that capability in 2.0 because the extension is not yet supported and the older OS version is dropped entirely. The release also arrives as Google&\#x27;s 2026 developer registration requirements loom over sideloaded apps, reinforcing F-Droid&\#x27;s role as an alternative marketplace, though the phased rollout over the coming weeks makes the extent of its effect uncertain.

**「Community Discussion」** Commenters were divided on the redesign: one criticized the lack of visual separation between sections, tappable affordances, and scroll indicators, while another welcomed the overhaul after finding the old F-Droid UI terrible and the Privileged Extension painful to configure on GrapheneOS and LineageOS. Discussion also noted a text-wrapping defect in a screenshot, questioned F-Droid&\#x27;s future amid an expected Google lockdown next year, and included an unrelated request for a user-friendly FOSS ebook reader.

<details><summary>References</summary>
<ul>
<li><a href="https://trashbox.ru/link/f-droid-android">Скачать F - Droid 2 . 0 -rc1 для Android</a></li>
<li><a href="https://www.theregister.com/applications/2026/09/24/f-droid-app-store-thumbs-its-nose-at-googles-dev-crackdown/5298974">F - Droid app store thumbs its nose at Google &#x27;s dev crackdown</a></li>
<li><a href="https://factually.co/fact-checks/technology/android-developer-registration-fdroid-sideloading-availability-6fefe0">If Android Requires Developer Registration, Can Users ..</a></li>

</ul>
</details>

**Tags**: `#Android`, `#F-Droid`, `#open-source`, `#app-distribution`, `#UI-redesign`

---

<a id="item-tech-news-2"></a>
### [Apple Disables Advanced Data Protection in UK, Creating Two-Tier iCloud Encryption](https://macanorak.com/two-tier-encryption-in-the-uk/) ⭐️ 8.0/10

A Hacker News item examines the UK’s two-tier encryption landscape after Apple disabled Advanced Data Protection \(ADP\) for UK users, raising questions about iCloud security and lawful access. According to discussion, withdrawing ADP did not affect the 14 iCloud categories already end-to-end encrypted by default, such as iCloud Keychain and Health, but ADP had extended that protection to 23 categories; for UK users without ADP, categories including iCloud Backup, Photos, Notes, and iCloud Drive revert to Standard Data Protection, where Apple holds the keys. The item frames this as Apple’s response to a legal order that would have required changing ADP’s security architecture, leading Apple to stop offering the feature rather than build a lawful-access mechanism. Community members debate whether even the baseline encrypted categories remain fully protected in practice and warn about precedent, government secrecy, and the broader erosion of end-to-end encryption.

hackernews · ReturnoftheHack · Sep 24, 10:39 · [Discussion](https://news.ycombinator.com/item?id=49828731)

**「Background」** Advanced Data Protection \(ADP\) is Apple’s optional iCloud setting that extends end-to-end encryption to additional data categories; after the UK issued a secret Technical Capability Notice in January 2025 seeking lawful access, Apple disabled ADP for UK users rather than alter its security architecture, according to reports \(tool-1-1, tool-1-2\). Apple’s withdrawal did not fully satisfy the UK order, and the dispute has since moved into court over government secrecy, with critics challenging the nondisclosure of such surveillance demands \(tool-1-2, tool-1-3\).

**「Impact」** UK iCloud users lose end-to-end encryption on the nine additional categories that ADP covered — including iCloud Backup, Photos, Notes and iCloud Drive — which revert to Standard Data Protection, where Apple holds the keys and can decrypt and disclose data in response to lawful process, leaving that data more exposed to breaches and government access. Apple has reportedly launched a legal challenge against the underlying UK data-access demand, so the durability of this two-tier arrangement remains contested.

**「Community Discussion」** Commenters disagree on the implications: some argue Apple has retreated from its 2015 resistance to government demands and point to age-verification or KYC prompts as evidence of weakening resolve, while others focus on the technical distinction between the 14 default end-to-end encrypted iCloud categories and the additional categories lost when ADP is withdrawn. Concerns about secret legal orders, an effective ban on end-to-end encryption, and whether Apple should exit the UK market or refuse services to UK government entities also feature prominently.

<details><summary>References</summary>
<ul>
<li><a href="https://www.kucoin.com/news/flash/apple-challenges-uk-s-demand-for-icloud-encryption-backdoor">Apple Challenges UK &#x27;s Demand for iCloud Encryption ... | KuCoin</a></li>
<li><a href="https://petapixel.com/2025/02/21/apple-removes-icloud-encryption-in-uk-after-secret-government-order/">Apple Removes iCloud Encryption in UK After Secret... | PetaPixel</a></li>
<li><a href="https://www.gadgetreview.com/uk-court-apple-icloud-backdoor-secrecy-called-farcical">UK Court: Apple iCloud Backdoor Secrecy Called... - Gadget Review</a></li>
<li><a href="https://www.theguardian.com/technology/2026/aug/03/apple-legal-challenge-uk-government-data-access">Apple launches legal challenge against UK government demand to access data | Apple | The Guardian</a></li>
<li><a href="https://androidexperto.com/apple-forced-to-kill-popular-security-feature-in-the-uk-heres-whats-happening/">Apple forced to kill popular security feature in the UK — he</a></li>
<li><a href="https://macdailynews.com/2026/08/03/apple-launches-legal-challenge-to-uk-demand-for-access-to-encrypted-user-data/">Apple launches legal challenge to UK demand for access to encrypted user data</a></li>

</ul>
</details>

**Tags**: `#encryption`, `#apple`, `#uk-policy`, `#privacy`, `#icloud`

---

<a id="item-tech-news-3"></a>
### [arXiv secures $17.2M to support independent nonprofit launch](https://www.reddit.com/r/MachineLearning/comments/1wox8kt/arxiv_receives_multiyear_philanthropic/) ⭐️ 7.0/10

arXiv has received $17.2 million in multiyear philanthropic commitments to support its launch as an independent nonprofit. The investment comes from Simons Foundation International, XTX Markets, and Siegel Family Endowment and spans three to five years. arXiv is a central preprint server for physics, mathematics, computer science, and machine learning research, making the funding significant for the broader research community. The Reddit submission provides only headline-level details and links to the primary arXiv blog post, and no community comments are available.

reddit · r/MachineLearning · /u/Nunki08 · Sep 24, 09:43

**「Background」** arXiv is a preprint archive founded by Paul Ginsparg that has long operated under Cornell University, where from 2010 onward it broadened its funding by asking institutions to make annual voluntary contributions based on download usage, with each member institution pledging a five-year funding commitment. That sustainable funding model combines major philanthropic and institutional support with a membership program, sponsors, affiliates, and individual donors. The newly announced $17.2 million in commitments is intended to support arXiv&\#x27;s transition by strengthening its technical infrastructure, supporting ongoing operations, and improving services for researchers worldwide as it moves to operate as an independent nonprofit.

**「Impact」** For the researchers who rely on arXiv&\#x27;s free preprint service, the $17.2 million commitment gives the platform a multiyear financial base for its launch as an independent nonprofit, a structure arXiv says will let it pursue a more diverse and sustainable funding model, faster technological development, and expanded partnerships without changing its mission or free access. The source item reports only headline-level figures, so how the three-to-five-year funding translates into specific operational capacity has not yet been detailed.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.arxiv.org/2026/09/23/arxiv-receives-multiyear-investment/">arXiv receives Multiyear Philanthropic Commitments to Support Its Launch as an Independent Nonprofit</a></li>
<li><a href="https://en.wikipedia.org/wiki/ArXiv">arXiv - Wikipedia</a></li>
<li><a href="https://runtimewire.com/article/arxiv-17-2m-nonprofit-transition">arXiv secures $17.2M in multiyear support for nonprofit ...</a></li>
<li><a href="https://blog.arxiv.org/2026/09/23/arxiv-receives-multiyear-investment/">arXiv receives 17.2 million multiyear investment</a></li>
<li><a href="https://info.arxiv.org/about/spinout_faq.html">arXiv is now an independent nonprofit - arXiv info</a></li>
<li><a href="https://blog.arxiv.org/2026/04/02/arxiv-is-becoming-an-independent-nonprofit/">arXiv is becoming an independent nonprofit – News from arXiv</a></li>

</ul>
</details>

**Tags**: `#arXiv`, `#open science`, `#research infrastructure`, `#nonprofit funding`, `#machine learning`

---

<a id="item-tech-news-4"></a>
### [Claude Code cloud sessions launch with up to $250 credits](https://code.claude.com/docs/en/claude-code-on-the-web) ⭐️ 7.0/10

Anthropic has launched Claude Code cloud sessions, moving the feature out of research preview for Pro, Max, Team, and Enterprise users. The cloud sessions let tasks continue running after users close their laptops, and users can view or take over the work from a browser, phone, desktop app, or terminal. Existing subscribers can claim one-time cloud session credits: $100 for Pro and $250 for Max, usable only for Cloud sessions, by logging in on the official claim page or running /claim-credit in Claude Code. The claim deadline is October 7 at 11:59 PM Pacific Time, and credits remain valid until November 4 at 11:59 PM; eligibility is determined after login according to account and terms, so not all users qualify. Anthropic&\#x27;s supported region list currently excludes mainland China, Hong Kong, and Macau.

telegram · zaihuapd · Sep 24, 02:45

**「Background」** Claude Code is Anthropic’s AI coding agent, and cloud sessions let a coding task continue running after the user closes their laptop, with the session viewable and controllable from a browser, phone, desktop app, or terminal. The capability was previously a research preview and is now generally available for Pro, Max, Team, and Enterprise users, with one-time cloud-session credits of $100 for Pro and $250 for Max users. The trial credits must be claimed by October 7 and expire November 4, eligibility depends on account and terms after login, and Anthropic’s supported-regions list currently excludes mainland China, Hong Kong, and Macau; explainx.ai also notes a GitHub requirement for the trial.

**「Impact」** Developers on Pro, Max, Team, and Enterprise plans can now keep Claude Code tasks running in the cloud and pick them up from browser, mobile, desktop, or terminal, with one-time credits of $100 \(Pro\) or $250 \(Max\) that must be claimed by 11:59 p.m. PT on October 7 and expire at 11:59 p.m. on November 4. Eligibility is determined per account and subject to terms, and Anthropic&\#x27;s supported-region list still excludes mainland China, Hong Kong, and Macau, so not all subscribers can claim the credits or use the feature.

<details><summary>References</summary>
<ul>
<li><a href="https://alphasignal.ai/news/anthropic-ships-claude-code-cloud-sessions-so-developers-can-code-without-a">Anthropic Ships Claude Code Cloud Sessions so Developers Can Code Without a Laptop | AlphaSignal</a></li>
<li><a href="https://explainx.ai/blog/claude-code-cloud-sessions-ga-100-250-credit-claim-credit-2026">Claude Code Cloud Sessions GA: Claim $100/$250 Credit | explainx.ai Blog | explainx.ai</a></li>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent , Terminal, IDE</a></li>

</ul>
</details>

**Tags**: `#Claude Code`, `#Anthropic`, `#AI coding agents`, `#cloud sessions`, `#developer tools`

---

<a id="item-tech-news-5"></a>
### [OpenAI Releases MentalHealthBench for Mental-Health AI Evaluation](https://openai.com/zh-Hans-CN/index/introducing-mentalhealthbench/) ⭐️ 7.0/10

OpenAI released MentalHealthBench, an open benchmark for evaluating how AI responds in real mental-health conversations. The benchmark was developed with more than 80 licensed mental-health experts across 22 countries. It measures behaviors including safety, gathering context, maintaining user autonomy, and providing actionable advice. MentalHealthBench covers scenarios involving adults, adolescents, caregivers, and clinical staff. OpenAI said the results show steady progress in how AI handles mental-health issues, but cautioned that ChatGPT cannot replace professional treatment.

telegram · zaihuapd · Sep 24, 06:00

**「Background」** Evaluation of AI in mental-health contexts has historically centered on crisis detection, leaving everyday stress, context-gathering, and ongoing support largely unmeasured. MentalHealthBench was co-created with more than 80 licensed mental health experts from 22 countries, who authored weighted rubrics spanning scenarios from ordinary stress to emergencies. It is presented as an open, expert-informed benchmark intended to fill the gap left by crisis-only evaluations.

**「Impact」** Developers, product teams, and mental-health organizations building conversational AI gain a shared open benchmark, authored by more than 80 licensed experts across 22 countries, for scoring responses in realistic mental-health scenarios on safety, context gathering, user autonomy, and actionable advice. Because the release offers limited methodology detail and no independent validation yet, its results should be treated as guidance rather than evidence that such systems can replace professional care.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/introducing-mentalhealthbench/">Introducing MentalHealthBench | OpenAI</a></li>
<li><a href="https://contentbuffer.com/news/openai-mentalhealthbench-80-clinicians-grade-ai-replies-e6b8dffb">OpenAI MentalHealthBench : 80 + Clinicians... — ContentBuffer News</a></li>
<li><a href="https://www.techbooky.com/openai-mentalhealthbench-ai-chat-safety/">OpenAI MentalHealthBench Tests Mental Health AI</a></li>
<li><a href="https://ybuild.ai/en/blog/mentalhealthbench-sensitive-conversation-launch-gate-founders">MentalHealthBench Changes How Founders Should Test Sensitive AI ...</a></li>
<li><a href="https://openai.com/index/introducing-mentalhealthbench/">Introducing MentalHealthBench | OpenAI</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#LLM evaluation`, `#mental health`, `#benchmark`, `#OpenAI`

---

## Financial News

<a id="item-finance-news-1"></a>
### [China confirms first AI talks with U.S., discusses tariff cuts and trade truce extension](https://www.cnbc.com/2026/09/24/china-confirms-first-ai-talks-with-us-have-taken-place-hints-at-trade-truce-extension.html) ⭐️ 8.0/10

China&\#x27;s Commerce Ministry confirmed Thursday that U.S. and Chinese trade negotiators held their first talks on artificial intelligence, and said the two sides discussed reducing tariffs and extending the trade arrangements agreed in Kuala Lumpur in October 2025. Treasury Secretary Scott Bessent said the two countries agreed to extend the trade truce to January; that truce kept tariffs lower and limited China&\#x27;s export controls on rare earths—minerals used in semiconductors and many other products.

rss · CNBC Finance · Sep 24, 14:16

**「Background」** The talks preceded a Washington state visit meeting between U.S. President Donald Trump and Chinese President Xi Jinping, after Chinese Vice Premier He Lifeng met Bessent in New York.

**「Impact」** The reported extension would keep tariffs lower and continue limits on China&\#x27;s rare-earth export controls through January, directly affecting manufacturers that depend on rare earths for semiconductors and other goods.

**Tags**: `#US-China trade`, `#Artificial intelligence`, `#Tariffs`, `#Rare earths`, `#Trade truce`

---

<a id="item-finance-news-2"></a>
### [Beijing Requires Topped-Out Structure Before Pre-Sale for New Land Plots](https://mp.weixin.qq.com/s/g-nwBAIGMCfuhENgs6o9-g) ⭐️ 8.0/10

On Sept. 24, Beijing issued implementation rules for reforming commercial housing sales: for projects on land sold after Aug. 28, developers must have the main structure topped out before applying for pre-sale, and completed-home sales are to be prioritized, with full, whole-process supervision of pre-sale funds. Land fees for such plots may be paid in installments, with a first payment of at least 50% of the total and the remainder interest-free and cleared within two years; banks may release individual mortgage loans only after the project passes completion filing.

telegram · zaihuapd · Sep 24, 11:10

**「Background」** Under China&\#x27;s long-standing pre-sale system, developers sell homes before they are built and use buyers&\#x27; payments to finance construction, which has left buyers exposed when projects stall. Beijing&\#x27;s new rules, covering land sold after Aug. 28, require the main structure to be topped out — the frame finished — before a pre-sale application, and channel all pre-sale proceeds into a supervised account at the city&\#x27;s housing fund management centre.

**「Impact」** Developers with Beijing projects on land sold after Aug. 28 must carry construction costs for years before collecting sale proceeds; a CICC estimate cited by Chinese media puts their free-cash-flow breakeven at 2.5–3 years after land purchase instead of within one year. The full escrow of pre-sale funds and the release of mortgages only after completion filing also shift prepayment risk away from homebuyers toward developers and their lenders.

<details><summary>References</summary>
<ul>
<li><a href="https://www.163.com/dy/article/L7KFNHKI0512D3VJ.html?clickfrom=w_house">163.com/dy/article/L7KFNHKI0512D3VJ.html?clickfrom=w_house</a></li>
<li><a href="https://m.21jingji.com/article/20260924/herald/689862331695d9635934bdf8b5b35515.html">北 京 ： 商 品 房 预 售 需 封 顶 优先选择 现 房 销 售 - 21财经</a></li>
<li><a href="https://www.163.com/dy/article/L7K8CGJN0519AFSG.html">封顶才准卖房，余款两年免息：北京新政很温柔|期房|预售|开发商|购房者|北京市|商品住房_网易订阅</a></li>
<li><a href="https://www.163.com/dy/article/L7KCJBLQ0535GP8A.html">重磅！北京现房销售细则落地，有什么利好什么利空？|期房|预售证|开发商|北京市|全年二手房均价_网易订阅</a></li>

</ul>
</details>

**Tags**: `#China property policy`, `#Beijing real estate`, `#housing pre-sale reform`, `#developer cash flow`, `#mortgage lending`

---

<a id="item-finance-news-3"></a>
### [Philadelphia Fed&\#x27;s Paulson Says Modest Further Tightening May Be Needed](https://www.cnbc.com/2026/09/24/philadelphia-feds-anna-paulson-says-modest-rate-moves-likely-ahead-to-tame-inflation.html) ⭐️ 7.0/10

Philadelphia Fed President Anna Paulson said Thursday that some &quot;modest further tightening&quot; may be warranted to return inflation to the Fed&\#x27;s 2% target, after the FOMC raised its benchmark rate by a quarter point a week earlier to a 3.75%-4% target range. She said underlying inflation is still running around 2.5%-3%, well above that target.

rss · CNBC Finance · Sep 24, 17:12

**「Background」** The Fed&\#x27;s rate-setting Federal Open Market Committee \(FOMC\) uses the benchmark rate as its main tool to steer inflation toward a 2% goal; Paulson&\#x27;s remarks are guidance rather than a policy decision.

**「Impact」** Investors are already pricing more tightening: longer-duration Treasury yields have risen to highs not seen since 2004, and traders see a 64% chance the FOMC raises rates again in October, according to CME Group&\#x27;s FedWatch tool.

**Tags**: `#Monetary Policy`, `#Federal Reserve`, `#Inflation`, `#Interest Rates`, `#Treasury Yields`

---

<a id="item-finance-news-4"></a>
### [U.S.-China trade truce extended two months to Jan. 10 as Xi begins state visit](https://www.cnbc.com/2026/09/24/us-china-trade-truce-bessent-trump-xi.html) ⭐️ 7.0/10

The U.S. and China have extended their trade truce by two months to Jan. 10, keeping tariffs lower and rare earths flowing, U.S. Treasury Secretary Scott Bessent said, as President Xi Jinping began a state visit to Washington.

rss · CNBC Finance · Sep 24, 04:55

**「Background」** The truce stems from a one-year agreement between Trump and Xi at a meeting in South Korea last October, and it had been set to expire in November.

**「Impact」** For companies, the two-month extension leaves current lower tariffs and rare earth flows in place only until Jan. 10; the European Chamber of Commerce in China&\#x27;s president said it does not address the lack of a standardized rare earth export licensing process.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nytimes.com/2026/09/23/us/politics/china-trade-truce-tariffs.html">U . S . and China Agree to Extend Trade Truce by 2 Months, Bessent ...</a></li>

</ul>
</details>

**Tags**: `#US-China trade`, `#tariffs`, `#rare earths`, `#trade policy`, `#diplomacy`

---

<a id="item-finance-news-5"></a>
### [Ahead of Trump-Xi meeting, China&\#x27;s self-sufficiency reshapes trade calculus](https://www.cnbc.com/2026/09/23/trump-xi-meeting-why-chinas-self-sufficiency-changes-the-calculus.html) ⭐️ 7.0/10

U.S. President Donald Trump and Chinese President Xi Jinping are expected to meet this week, with businesses hoping for at best an extension of the trade truce reached last fall. The U.S. trade deficit with China rose again this year after briefly falling to its lowest level since 2017 in April, as demand for AI-related parts offset the effect of tariffs, according to China Customs data accessed through Wind Information.

rss · CNBC Finance · Sep 24, 01:44

**「Background」** China&\#x27;s push for self-sufficiency and export dominance has reduced its exposure to outside trade pressure: the country reached 40% of global container exports this summer, a milestone European Chamber of Commerce in China president Jens Eskelund had expected only in 2030, while Asia still supplies more than 60% of U.S. imports.

**「Impact」** Foreign competitors are feeling the strain: the American Chamber of Commerce in Shanghai said this month that three-quarters of surveyed members saw Chinese rivals as more advanced, and that domestic competition overtook geopolitical tensions as their top challenge for the first time since 2022.

**Tags**: `#US-China trade`, `#Trump-Xi meeting`, `#China economy`, `#tariffs`, `#AI supply chain`

---

<a id="item-finance-news-6"></a>
### [DeepSeek Reported at $1B Annualized Revenue as It Plans RMB 50B Round and Shanghai Listing](https://weibo.com/1642634100/RjAoNli86) ⭐️ 7.0/10

DeepSeek&\#x27;s annualized revenue run rate has reached $1 billion, up from under $500 million a few months earlier, CEO Liang Wenfeng reportedly told investors, attributing the growth to higher API prices and continued demand; the company is also preparing a second funding round targeting RMB 50 billion \(about $7.5 billion\) at a RMB 500 billion valuation, with plans to list on the Shanghai Stock Exchange. These figures come from unnamed sources and are not officially confirmed.

telegram · zaihuapd · Sep 24, 07:56

**「Background」** DeepSeek is a Chinese AI model developer; an annualized revenue run rate projects recent revenue over a full year rather than reporting a completed fiscal-year total, and the company is pursuing a second funding round at a 500 billion yuan valuation ahead of a planned Shanghai listing, according to reports citing unnamed sources.

**「Who is affected」** The price increase applies to developers and businesses paying for DeepSeek&\#x27;s API, while its free web and app chat services for ordinary users are reported to be unaffected — so API-reliant companies face higher operating costs.

<details><summary>References</summary>
<ul>
<li><a href="https://m.cnmo.com/news/819333.html">曝 DeepSeek 完成75 亿 美 元 融 资 年 化 营 收 达 10 亿 美 元 _CNMO</a></li>
<li><a href="https://wallstreetcn.com/articles/3782443">报道： DeepSeek 年 化 营 收 突破 10 亿 美 元 ，计划在 10 ...</a></li>
<li><a href="https://wenku.baidu.com/view/e150f5452679168884868762caaedd3383c4b5b7.html">DeepSeek API调价确认！2026年8月涨价公告解读与应对指南</a></li>
<li><a href="https://www.tmtpost.com/8094414.html">DeepSeek预告API涨价，AI低价红利落幕-钛媒体官方网站</a></li>

</ul>
</details>

**Tags**: `#DeepSeek`, `#AI financing`, `#IPO`, `#revenue growth`, `#API pricing`

---

<a id="item-finance-news-7"></a>
### [China&\#x27;s three major telecom carriers suspend installment phone financing, including &quot;0 yuan phone&quot; offers](https://finance.sina.com.cn/jjxw/2026-09-24/doc-inisxhnx5270778.shtml) ⭐️ 7.0/10

China Mobile, China Telecom and China Unicom suspended new sign-ups for their financial installment phone-purchase plans — including &quot;0 yuan phone&quot; offers such as Hebao credit purchase, Chengfenqi and Wofenqi — from September 24, 2026, according to the report, with existing installment contracts still in force. Carrier customer service has confirmed the suspension, the report said, while no official statement has been issued; staff mostly described it as a product upgrade and gave no restart date.

telegram · zaihuapd · Sep 24, 08:46

**「Background」** Such offers were previously marketed as &quot;free phones&quot; but in practice signed customers up for installment loans, making them a frequent source of consumer complaints. The operators&\#x27; customer service lines have confirmed the suspension, while no formal explanation has been issued; some responses cited a product upgrade, with no restart date given.

**「Impact」** The suspension is expected to weigh on the three operators&\#x27; offline business halls, which had used installment offers as a sales channel, according to tech outlet Phoenix \(tool-2-1\); existing installment contracts continue, so current users are unaffected for now.

<details><summary>References</summary>
<ul>
<li><a href="https://tech.ifeng.com/c/8wgLAZcg33a">“0元 购 机”凉了！ 移动电 信 联通三大运营商 分 期 业务全面 暂 停 _凤凰网</a></li>

</ul>
</details>

**Tags**: `#China telecom`, `#consumer finance`, `#installment sales`, `#mobile phones`, `#product suspension`

---