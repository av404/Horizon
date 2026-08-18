---
layout: default
title: "Horizon Summary: 2026-08-18 (EN)"
date: 2026-08-18
lang: en
---

> From 37 items, 14 important content pieces were selected

---

**Technology News**
1. [Mojo Is Now Open Source Under Apache 2](#item-tech-news-1) ⭐️ 8.0/10
2. [Qwen 3.8 27B Matches GPT-5.6 Luna on AI Index](#item-tech-news-2) ⭐️ 8.0/10
3. [Chinese Domestic AI Chips to Approach 90% Market Share by 2026](#item-tech-news-3) ⭐️ 8.0/10
4. [Turbovec brings Google&\#x27;s TurboQuant to Rust for efficient vector search](#item-tech-news-4) ⭐️ 7.0/10
5. [Linux 7.3 VRAM Overcommit Performance Gains Discussed](#item-tech-news-5) ⭐️ 7.0/10
6. [Data Center Waste Heat Raises Downwind Phoenix Temperatures 0.8°C](#item-tech-news-6) ⭐️ 7.0/10
7. [Two-Page Polars Cheatsheet Based on Definitive Guide](#item-tech-news-7) ⭐️ 7.0/10
8. [macOS 26.7 Code Reveals Apple Intelligence Content-Safety Filtering for Mainland China](#item-tech-news-8) ⭐️ 7.0/10
9. [China pulls custom Windows 10 from agencies months early](#item-tech-news-9) ⭐️ 7.0/10

**Financial News**
1. [Rising Treasury yields lift mortgage and diesel costs for households](#item-finance-news-1) ⭐️ 7.0/10
2. [Kalshi seeks CFTC approval for equity-index perpetual futures](#item-finance-news-2) ⭐️ 7.0/10
3. [US &\#x27;Buy Now, Pay Later&\#x27; Borrowing Hit $160 Billion in 2025](#item-finance-news-3) ⭐️ 7.0/10
4. [HSBC asks some mainland Chinese investment clients to declare fund sources by Sep 12 or risk losing service](#item-finance-news-4) ⭐️ 7.0/10
5. [Apple&\#x27;s US App Store revenue falls amid regulatory changes](#item-finance-news-5) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Mojo Is Now Open Source Under Apache 2](https://simonwillison.net/2026/Aug/18/mojo-is-now-open-source/) ⭐️ 8.0/10

Modular has open-sourced the Mojo programming language compiler and toolchain under the Apache 2 license, following Mojo 1.0&\#x27;s release last week. Previously promised since May 2023, the move fulfills an original open-source commitment even as Mojo&\#x27;s long-term Python-superset plan has been revised since August 2025 to allow the language to evolve independently. Mojo is now positioned as a Python-inspired language optimized for GPU programming rather than a fully compatible Python superset. The Apache 2 license permits broad use and modification, marking a major milestone for the AI/ML language ecosystem.

rss · Simon Willison · Aug 18, 21:39

**「Background」** Mojo launched in May 2023 as a proposed superset of Python, intended to help existing Python code bootstrap its ecosystem. In August 2025, Modular revised that vision, saying Mojo may or may not become a full Python superset and noting AI-assisted migration tooling could ease the transition. The Apache 2 license is a permissive open-source license allowing users to use, modify, and distribute the software.

**「Impact」** Developers can now inspect, modify, and build on Mojo&\#x27;s compiler and toolchain under Apache 2&\#x27;s permissive terms, removing a key barrier to broader adoption of the language for GPU and AI workloads.

**Tags**: `#mojo`, `#open-source`, `#programming-language`, `#ai`, `#compiler`

---

<a id="item-tech-news-2"></a>
### [Qwen 3.8 27B Matches GPT-5.6 Luna on AI Index](https://simonwillison.net/2026/Aug/17/qwen-38-27b-scores-52/) ⭐️ 8.0/10

Qwen 3.8 27B scored 52 on the Artificial Analysis Intelligence Index, matching GPT-5.6 Luna \(max\) and landing just one point behind GLM-5.2 \(max\), a 753B-parameter model, and DeepSeek V4 Pro 0813 \(max\), a 1.7T-parameter model. Luna&\#x27;s parameter count is not publicly known but is presumed to be far larger than 27B, making Qwen 3.8 27B&\#x27;s parity a striking efficiency milestone. Simon Willison, who reported the result on August 17, 2026, described the model as truly astonishing. The score suggests that a relatively compact open-weights model can approach the performance of much larger frontier systems on this benchmark.

rss · Simon Willison · Aug 17, 23:58

**「Background」** Artificial Analysis is an independent benchmark aggregator that publishes an Intelligence Index scoring language models on reasoning and problem-solving tasks; according to the index, Qwen3.8 27B&\#x27;s score of 52 is far above the median of 9 among open-weight models of similar size. The model is a 27-billion-parameter release from Alibaba&\#x27;s Qwen team, and this common scale is what makes direct comparisons to much larger models like GPT-5.6 Luna, GLM-5.2, and DeepSeek V4 Pro meaningful.

**「Impact」** For developers, this result implies a 27B-parameter model can deliver frontier-adjacent benchmark performance at far lower compute and deployment cost than models that are dozens or hundreds of times larger.

<details><summary>References</summary>
<ul>
<li><a href="https://artificialanalysis.ai/models/qwen3-8-27b">Qwen3.8 27B - Intelligence, Performance &amp; Price Analysis</a></li>
<li><a href="https://simonwillison.net/2026/Aug/17/qwen-38-27b-scores-52/">Qwen 3.8 27B scores 52 on the Artificial Analysis Intelligence Index</a></li>

</ul>
</details>

**Tags**: `#qwen`, `#artificial-analysis`, `#llms`, `#benchmarks`, `#ai`

---

<a id="item-tech-news-3"></a>
### [Chinese Domestic AI Chips to Approach 90% Market Share by 2026](https://www.tomshardware.com/tech-industry/artificial-intelligence/chinas-homegrown-ai-accelerators-to-supply-90-percent-of-the-countrys-domestic-market-analysts-suggest-cambricon-and-huawei-expected-to-be-the-biggest-winners-in-the-shift-away-from-nvidia-and-amd) ⭐️ 8.0/10

TrendForce predicts that Chinese domestic AI accelerators will supply nearly 90% of China&\#x27;s domestic market by 2026, a significant jump from 45% last year, with Huawei and Cambricon expected to be the biggest beneficiaries. In 2025, Nvidia held a 55% market share with 2.2 million units shipped, while Huawei shipped 812,000 units for a 20.3% share. To meet the forecast, China would need to increase its high-end AI chip production by 2.2 times to about 1.96 million units within a year, though whether production capacity can keep pace remains uncertain. This shift represents a major realignment of the AI accelerator supply chain away from Nvidia and AMD toward domestic alternatives.

telegram · zaihuapd · Aug 18, 13:03

**「Background」** The forecast reflects ongoing U.S. export controls that restrict Nvidia and AMD from selling advanced AI accelerators to China, prompting Chinese chipmakers to develop domestic alternatives. Huawei and Cambricon have emerged as leading domestic suppliers, with their products increasingly adopted by Chinese data centers and AI firms seeking to reduce reliance on foreign technology.

**「Impact」** Chinese AI companies and data centers will face a substantial supply shift toward Huawei and Cambricon accelerators, potentially affecting performance, software compatibility, and procurement strategies as Nvidia and AMD&\#x27;s market share declines. The feasibility of this transition depends on whether domestic production can scale up fast enough to meet the projected 1.96 million units demand.

**Tags**: `#AI accelerators`, `#China semiconductor`, `#Huawei`, `#Cambricon`, `#AI hardware`

---

<a id="item-tech-news-4"></a>
### [Turbovec brings Google&\#x27;s TurboQuant to Rust for efficient vector search](https://github.com/RyanCodrai/turbovec) ⭐️ 7.0/10

Turbovec is a new Rust library that implements Google&\#x27;s TurboQuant quantization technique for efficient vector search, targeting local and privacy-focused applications. Its core advantage is a greatly reduced memory footprint—commenters suggest roughly 4 GB for 10 million documents—which could make large-scale reverse index construction faster and debugging/performance testing smoother. SQLite bindings are reportedly in progress, and developers are exploring compiling it to WASM for browser extensions. It enters a landscape where FAISS is no longer considered state-of-the-art and Qdrant has already been integrating TurboQuant.

hackernews · fittingopposite · Aug 18, 18:07 · [Discussion](https://news.ycombinator.com/item?id=49349898)

**「Background」** Vector search finds similar items by comparing embeddings, but storing and scanning large numbers of high-dimensional vectors can become memory-intensive and slow. Google&\#x27;s TurboQuant is a compression technique that combines vector normalization with a random rotation before quantization, dramatically reducing the memory footprint of vector indexes while preserving search accuracy. Turbovec is a Rust implementation of this technique, making it possible to build compact vector indexes that can run locally or in privacy-focused applications.

**「Community Discussion」** Reactions are positive overall, with users highlighting memory efficiency and the potential for faster index building, while several ask for a more human-readable README. One user asks whether the Rust code can compile to WASM for in-browser extension use, and another points out that Qdrant has been integrating TurboQuant for months, suggesting an existing alternative.

<details><summary>References</summary>
<ul>
<li><a href="https://research.google/blog/turboquant-redefining-ai-efficiency-with-extreme-compression/">TurboQuant : Redefining AI efficiency with extreme compression</a></li>
<li><a href="https://medium.com/data-science-in-your-pocket/turbovec-googles-turboquant-makes-vector-search-smaller-faster-and-simpler-fdea72674aad">turbovec : Google ’s TurboQuant Makes Vector Search ... | Medium</a></li>

</ul>
</details>

**Tags**: `#rust`, `#vector-search`, `#quantization`, `#ai`, `#library`

---

<a id="item-tech-news-5"></a>
### [Linux 7.3 VRAM Overcommit Performance Gains Discussed](https://pixelcluster.dev/VRAM-Overcommit/) ⭐️ 7.0/10

An article on pixelcluster.dev describes performance improvements in Linux 7.3 for running out of video RAM \(VRAM\), focusing on better handling of VRAM overcommit scenarios. The piece suggests that the kernel should rely on applications to inform it about desired VRAM stickiness, arguing that applications are best positioned to make those allocation decisions rather than relying on kernel guesses. It also raises ideas around virtual memory fragmentation, possibly including in-place defragmentation despite potential hitches. The article is speculative and lacks full verifiable technical details, but the discussion has drawn strong community interest on Hacker News with 492 points and 258 comments. The topic is relevant to kernel design, memory management, and GPU performance optimization.

hackernews · flaburgan · Aug 18, 07:51 · [Discussion](https://news.ycombinator.com/item?id=49342719)

**「Background」** VRAM is a GPU&\#x27;s dedicated memory; when workloads exceed it, the kernel must either reject allocations or use overcommit and paging, which historically has been poorly supported on Linux. The PixelCluster blog posts describe kernel work to improve VRAM handling specifically for out-of-memory situations, and according to Phoronix the patch series has been merged upstream and queued for Linux 7.3, with the code already shipping in Valve&\#x27;s SteamOS kernel.

**「Impact」** The Linux 7.3 VRAM-overcommit improvements should reduce the performance hit for AMD GPU users when VRAM is exhausted, while Nvidia users are unlikely to benefit because Nvidia does not support paging, and Linux can also be configured to disable memory overcommit entirely.

**「Community Discussion」** Commenters are largely enthusiastic about the proposed Linux 7.3 improvements, praising the article as well-written and informative, and expressing eagerness for future kernel releases. Some commenters raise practical concerns, such as Nvidia&\#x27;s lack of VRAM paging support and the desire for better handling when system RAM is full without freezing, while others share the author&\#x27;s hunch that application-informed memory allocation is the right direction.

<details><summary>References</summary>
<ul>
<li><a href="https://www.phoronix.com/news/Linux-7.3-Improving-vRAM-Mgmt">Linux 7.3 To Land Initial Code Improving vRAM Management, More Improvements Coming - Phoronix</a></li>
<li><a href="https://pixelcluster.dev/VRAM-Overcommit/">VRAM Management Part 2: Beyond the Limits of Physical VRAM | pixelcluster&#x27;s GPU blog</a></li>
<li><a href="https://pixelcluster.dev/VRAM-Overcommit/">VRAM Management Part 2: Beyond the Limits... | pixelcluster&#x27;s GPU blog</a></li>
<li><a href="https://news.ycombinator.com/item?id=49342719">Linux 7.3 improves performance when running out of vRAM</a></li>

</ul>
</details>

**Tags**: `#linux`, `#vram`, `#memory-management`, `#gpu`, `#kernel`

---

<a id="item-tech-news-6"></a>
### [Data Center Waste Heat Raises Downwind Phoenix Temperatures 0.8°C](https://asmedigitalcollection.asme.org/sustainablebuildings/article/7/2/024501/1233035/Data-Center-Waste-Heat-as-an-Emerging-Urban) ⭐️ 7.0/10

A field study in Phoenix measured the neighborhood-scale air temperature impact of data center waste heat and found that downwind areas near a data center campus were about 0.8°C warmer than upwind areas, with the observed temperature difference extending roughly 500 meters downwind. The study provides concrete empirical evidence that data center heat emissions can affect local urban temperatures, even though the average effect is much smaller than some headlines suggest. These findings are relevant to data center siting, urban heat management, and infrastructure planning, particularly in hot climates where additional heat can worsen outdoor conditions. The study was published in the ASME Journal of Sustainable Buildings under the title &\#x27;Data Center Waste Heat as an Emerging Urban Microclimate Phenomenon&\#x27; or similar, though the exact full title should be verified from the original source.

hackernews · cwwc · Aug 18, 17:24 · [Discussion](https://news.ycombinator.com/item?id=49349147)

**「Background」** Data centers consume large amounts of electricity and generate substantial waste heat as a byproduct of their computing and cooling operations; in hot climates like Phoenix, Arizona, this heat can be carried downwind and raise local air temperatures. A field study by researchers at Arizona State University measured temperature increases in downwind neighborhoods, finding increases of up to 4 degrees Fahrenheit \(about 2 degrees Celsius\) and noting that a single data center&\#x27;s waste heat can exceed that of 40,000 U.S. households.

**「Impact」** Neighborhoods downwind of large data centers in Phoenix may experience measurable but modest additional heat exposure, which could affect outdoor comfort and heat-health risks during extreme heat events. This evidence can inform urban planners and data center operators considering heat mitigation and site placement.

**「Community Discussion」** Commenters disagreed about whether concerns over data center heat and pollution are exaggerated, with some suggesting that anti-data-center sentiment may be driven by political or NIMBY motives and others pointing to more significant pollution sources like oil refineries. Several commenters highlighted that the measured 0.8°C average increase is much smaller than the 4°C figure in some headlines, and one commenter lamented that the discussion felt dominated by ideology and inauthentic accounts rather than objective data.

<details><summary>References</summary>
<ul>
<li><a href="https://www.rediff.com/news/report/data-centers-heat-impact-on-downwind-localities/20260519.htm">Data Centre Waste Heat : Impact On Neighbourhood Temperatures</a></li>
<li><a href="https://techxplore.com/news/2026-05-centers-nearby-temperatures-degrees-phoenix.html">Data centers raise nearby temperatures by up to 4 degrees in Phoenix</a></li>

</ul>
</details>

**Tags**: `#data centers`, `#environmental impact`, `#urban heat`, `#sustainability`, `#field measurements`

---

<a id="item-tech-news-7"></a>
### [Two-Page Polars Cheatsheet Based on Definitive Guide](https://opensource.posit.co/resources/cheatsheets/polars/) ⭐️ 7.0/10

jeroenjanssens and colleagues released a two-page Python Polars cheatsheet derived from their O&\#x27;Reilly book, Python Polars: The Definitive Guide, compressing nearly 500 pages into a practical reference for common dataframe operations. The cheatsheet is available as both a PDF and an accessible HTML version on the Posit Open Source site. It intentionally omits depth, described by the authors as &\#x27;highly lossy compression,&\#x27; and aims to capture the most useful Polars operations. The release prompted discussion about Polars compared with R&\#x27;s dplyr/data.table and DuckDB, as well as feedback about Polars&\#x27; column-expression syntax \(pl.col\(...\)\).

hackernews · jeroenjanssens · Aug 18, 13:38 · [Discussion](https://news.ycombinator.com/item?id=49345476)

**「Background」** Polars is a relatively new, high-performance DataFrame library for Python, often positioned as a faster and more expressive alternative to Pandas. The cheatsheet is based on the O&\#x27;Reilly book &\#x27;Python Polars: The Definitive Guide&\#x27; by Jeroen Janssens and Thijs Nieuwdorp, and was published via Posit Open Source. It condenses the nearly 500-page book into a two-page reference for common dataframe operations, available as PDF and HTML.

**「Impact」** The cheatsheet gives current and prospective Polars users a concise, book-derived reference for common dataframe operations, potentially easing adoption for developers coming from pandas or R.

**「Community Discussion」** Commenters compared the cheatsheet to R&\#x27;s dplyr/data.table and DuckDB, with some saying it makes Polars worth trying despite prior pandas frustrations. Others noted that Polars&\#x27; pl.col\(&\#x27;...&\#x27;\) syntax adds ceremony, and one user said they moved from Polars to DuckDB and have not looked back.

<details><summary>References</summary>
<ul>
<li><a href="https://opensource.posit.co/resources/cheatsheets/polars/">Python Polars: The Definitive Cheatsheet :: Posit Open Source</a></li>

</ul>
</details>

**Tags**: `#polars`, `#python`, `#dataframes`, `#cheatsheet`, `#data-analysis`

---

<a id="item-tech-news-8"></a>
### [macOS 26.7 Code Reveals Apple Intelligence Content-Safety Filtering for Mainland China](https://www.macrumors.com/2026/08/17/macos-26-7-unreleased-apple-devices/) ⭐️ 7.0/10

According to a MacRumors report cited in a Telegram post, code in macOS 26.7 indicates that Apple&\#x27;s Writing Tools will include a content-safety mechanism when it arrives in mainland China. The code strings show that after multiple security alerts, the Writing Tools feature will be temporarily restricted, and for content that Apple Intelligence cannot edit, the system will display a prompt suggesting the user send the text to another handler. Users will also be required to install a content-safety update before using Writing Tools on iPhone. The finding suggests that Apple is preparing an independent content-filtering, interception, and penalty system for its AI features in mainland China, with rules potentially delivered remotely via cloud control. This matters because it gives a concrete look at how Apple&\#x27;s on-device AI writing features may be moderated under Chinese content requirements.

telegram · zaihuapd · Aug 18, 02:16

**「Background」** macOS Tahoe 26.7 is the current release candidate for Apple&\#x27;s next-generation desktop operating system, seeded to developers on August 17, 2026. The build&\#x27;s code includes references to unreleased products and indicates that Apple Intelligence features, including a localized &\#x27;Writing Tools&\#x27; implementation, are being prepared for mainland China. The leaks describe content-safety mechanics: after repeated security alerts, the tool can be temporarily restricted, and unsupported text can be routed to a third-party app.

**「Impact」** Users in mainland China who use Apple&\#x27;s Writing Tools may have the feature temporarily restricted after repeated security alerts, and certain text that cannot be safely edited will be blocked from processing, with the system suggesting they send it to another app such as %1$@ or %2$@. Apple has also confirmed that previously purchased devices supporting Apple Intelligence will be able to activate and use it in that region when the features become available.

<details><summary>References</summary>
<ul>
<li><a href="https://www.macrumors.com/2026/08/17/macos-26-7-unreleased-apple-devices/">macOS Tahoe 26 . 7 is Full of References to Unreleased... - MacRumors</a></li>
<li><a href="https://www.macworld.com/article/3214949/upcoming-apple-products-revealed-in-macos-26-7-release-candidate.html">Upcoming Apple products revealed in the macOS 26 . 7 release...</a></li>
<li><a href="https://support.apple.com/en-us/121115">How to get Apple Intelligence - Apple Support</a></li>

</ul>
</details>

**Tags**: `#Apple`, `#AI censorship`, `#content moderation`, `#macOS`

---

<a id="item-tech-news-9"></a>
### [China pulls custom Windows 10 from agencies months early](https://www.bloomberg.com/news/articles/2026-08-18/china-axing-microsoft-windows-from-state-agencies-ahead-of-plan) ⭐️ 7.0/10

China&\#x27;s national security ministry has ordered some government agencies to uninstall a customized version of Windows 10, moving the previously planned phase-out, originally set for February 2027, months earlier. The directive stems from data security concerns, according to people familiar with the matter, though no specific vulnerability was disclosed. Microsoft said it has not found any security incidents affecting the product and that the customized Windows 10 continues to receive regular security updates. The move signals accelerated government action against the customized OS and could affect Microsoft&\#x27;s presence in Chinese state-affiliated institutions.

telegram · zaihuapd · Aug 18, 06:22

**「Background」** Microsoft developed a customized version of Windows 10, known as Windows 10 China Government Edition, based on Windows 10 Enterprise but modified for Chinese government use, after negotiations involving CEO Satya Nadella and Chinese finance officials. The Chinese government had planned to phase out this system by February 2027, but the national security ministry is now requiring some agencies to uninstall it months ahead of that schedule, reflecting broader efforts to reduce reliance on foreign technology.

**「Impact」** Affected Chinese government agencies must uninstall the customized Windows 10 build months ahead of the originally planned February 2027 retirement, accelerating their migration and adding pressure on Microsoft&\#x27;s China government business.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bloomberg.com/news/articles/2026-08-18/china-axing-microsoft-windows-from-state-agencies-ahead-of-plan">China Removes Microsoft Windows at State Users Ahead of Plan</a></li>
<li><a href="https://www.techspot.com/news/113529-china-finally-pulling-windows-10-government-machines-ahead.html">China pulls the plug on Windows 10 for government ... | TechSpot</a></li>
<li><a href="https://www.tomshardware.com/software/operating-systems/china-reportedly-orders-state-agencies-to-uninstall-its-government-only-edition-of-windows-10">China reportedly orders state agencies to uninstall its government-only edition of Windows 10 — Beijing accelerates planned retirement over data security concerns | Tom&#x27;s Hardware</a></li>
<li><a href="https://www.tradingkey.com/analysis/stocks/us-stocks/262114664-win10-government-removal-microsoft-china-headwinds-tradingkey">Win10 Government Edition Phased Out Early as Microsoft&#x27;s China Business Faces New Headwinds</a></li>

</ul>
</details>

**Tags**: `#Windows 10`, `#China`, `#government policy`, `#data security`, `#Microsoft`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Rising Treasury yields lift mortgage and diesel costs for households](https://www.cnbc.com/2026/08/18/bond-market-treasury-yields-warsh-main-street.html) ⭐️ 7.0/10

A recent sell-off in U.S. government bonds has pushed the 10-year Treasury yield above 4.7%, lifting the average 30-year mortgage rate to 6.75% and raising the price of diesel to $5.46 a gallon, up 48% from a year earlier.

rss · CNBC Finance · Aug 18, 16:48

**「Background」** Long-term Treasury yields reflect investor expectations for growth and inflation, while the Federal Reserve controls short-term rates. The U.S. budget deficit is projected to hit $2.1 trillion, around 6.4% of GDP, for the fiscal year through September, and new Fed Chair Kevin Warsh has seemed to welcome the rise in yields.

**「Impact」** These moves hit households directly through higher mortgage and fuel costs, while Wall Street remains better insulated because stock gains have been concentrated among the wealthiest Americans.

**Tags**: `#bond yields`, `#Treasury market`, `#consumer debt`, `#fiscal policy`, `#inflation`

---

<a id="item-finance-news-2"></a>
### [Kalshi seeks CFTC approval for equity-index perpetual futures](https://www.cnbc.com/2026/08/18/kalshi-wants-to-launch-perps-tied-to-equity-indexes.html) ⭐️ 7.0/10

Kalshi has filed with the CFTC to launch perpetual futures tied to equity indexes, including a &\#x27;US500&\#x27; contract that tracks the MerQube U.S. Large Cap Index. The proposal is pending approval; Kalshi said perpetual futures had over $90 trillion in global volume in 2025.

rss · CNBC Finance · Aug 18, 16:49

**「Background」** Perpetual futures are no-expiration, futures-style contracts that track an asset&\#x27;s price using funding payments. Until Kalshi received CFTC approval for cryptocurrency perps a few months ago, the asset class was mostly offshore, and CME has sued the CFTC over that approval.

**Tags**: `#Kalshi`, `#perpetual futures`, `#CFTC`, `#equity indexes`, `#exchange competition`

---

<a id="item-finance-news-3"></a>
### [US &\#x27;Buy Now, Pay Later&\#x27; Borrowing Hit $160 Billion in 2025](https://www.nytimes.com/2026/08/17/business/buy-now-pay-later.html) ⭐️ 7.0/10

Americans borrowed $160 billion through &\#x27;buy now, pay later&\#x27; loans in 2025, nearly double the 2023 level, as lenders expanded into everyday bills like rent and utilities, raising concerns about overdraft fees and debt traps.

telegram · zaihuapd · Aug 18, 01:41

**「Background」** Buy now, pay later \(BNPL\) is a short-term installment credit product that originally appeared mainly at online checkout but has expanded to cover everyday bills such as rent, utilities, insurance and medical costs. Federal Reserve data estimate BNPL providers originated close to $160 billion in consumer credit in 2025, with about half in traditional “pay in 4” plans and the rest in other short- and longer-term installment loans.

**「Impact」** Consumers who rely on BNPL for rent and utility payments may face overdraft fees from automatic debits and can accumulate debt that is not reported to major credit bureaus, leaving their true financial exposure invisible to lenders; Richmond Fed research also notes that BNPL users generally carry higher debt than nonusers.

<details><summary>References</summary>
<ul>
<li><a href="https://www.federalreserve.gov/econres/notes/feds-notes/buy-now-pay-later-beyond-pay-in-4-a-comprehensive-product-overview-20260605.html">The Fed - “Buy Now, Pay Later” Beyond “Pay in 4”, A Comprehensive Product Overview</a></li>
<li><a href="https://www.nytimes.com/2026/08/17/business/buy-now-pay-later.html">‘Buy Now, Pay Later’ Lenders Pitch Loans for Needs Like Electricity and Rent - The New York Times</a></li>
<li><a href="https://files.consumerfinance.gov/f/documents/cfpb_BNPL_Report_2025_01.pdf">CONSUMER FINANCIAL PROTECTION BUREAU | JANUARY 2025 Consumer Use of Buy</a></li>
<li><a href="https://www.richmondfed.org/publications/research/economic_brief/2026/eb_26-05">Buy Now, Pay Later: Recent Developments and Implications | Richmond Fed</a></li>

</ul>
</details>

**Tags**: `#buy-now-pay-later`, `#consumer-credit`, `#household-debt`, `#fintech`, `#financial-regulation`

---

<a id="item-finance-news-4"></a>
### [HSBC asks some mainland Chinese investment clients to declare fund sources by Sep 12 or risk losing service](https://36kr.com/newsflashes/3944605562797192) ⭐️ 7.0/10

HSBC Hong Kong has begun asking some mainland Chinese investment clients to submit a source-of-funds declaration, warning that investment services may be suspended if it is not filed by Aug 20 and may be terminated if it is not filed by Sep 12. The bank says the requirement applies only to investment-service clients and is part of keeping its know-your-client information up to date.

telegram · zaihuapd · Aug 18, 07:30

**「Background」** Banks in Hong Kong are required to follow anti-money-laundering rules, including verifying that clients&\#x27; investment funds have legitimate sources and keeping customer information up to date. HSBC says the declaration request applies only to its investment services clients.

<details><summary>References</summary>
<ul>
<li><a href="https://www.163.com/dy/article/L4KAO89P0512B07B.html">163.com/dy/article/L4KAO89P0512B07B.html</a></li>
<li><a href="https://m.nbd.com.cn/articles/2026-08-18/4545030.html">m.nbd.com.cn/articles/2026-08-18/4545030.html</a></li>
<li><a href="https://cj.sina.com.cn/articles/view/1649173367/m624c637703301ijyq?finpagefr=p_104">cj.sina.com.cn/articles/view/1649173367/m624c637703301ijyq?...</a></li>

</ul>
</details>

**Tags**: `#HSBC`, `#compliance`, `#KYC`, `#cross-border investment`, `#regulatory`

---

<a id="item-finance-news-5"></a>
### [Apple&\#x27;s US App Store revenue falls amid regulatory changes](https://www.macrumors.com/2026/08/18/apple-app-store-revenue-falling/) ⭐️ 7.0/10

Apple&\#x27;s US App Store commission revenue has fallen 18% since early 2026, and US user spending in the second quarter dropped 6% year over year after growing 9% the year before, according to Appfigures and Sensor Tower. Apple says regulatory changes have weighed on its services business growth.

telegram · zaihuapd · Aug 18, 12:17

**「Background」** The declines follow changes to App Store payment and commission rules in the US and other markets, including Brazil and Japan, where revenue has also slipped since new rules took effect.

**Tags**: `#Apple`, `#App Store`, `#regulatory impact`, `#services revenue`, `#consumer spending`

---