---
layout: default
title: "Horizon Summary: 2026-08-13 (EN)"
date: 2026-08-13
lang: en
---

> From 41 items, 16 important content pieces were selected

---

**Technology News**
1. [Gemini 3.7 Flash Launches With New Pricing and Strong Test Results](#item-tech-news-1) ⭐️ 8.0/10
2. [Spaghettifying DRAM: AMD Memory-Controller Exploit Surfaces](#item-tech-news-2) ⭐️ 8.0/10
3. [Choose Boring Technology: Spend Your Innovation Tokens Wisely](#item-tech-news-3) ⭐️ 8.0/10
4. [DeepSeek V4 Pro 0813 Released with Open Weights on Hugging Face](#item-tech-news-4) ⭐️ 8.0/10
5. [DeepMind launches SL2T sign-language-to-text AI on Pixel 11](#item-tech-news-5) ⭐️ 8.0/10
6. [OpenAI Previews Ultrafast Mode, GPT-5.6 Sol Up to 14x Faster](#item-tech-news-6) ⭐️ 8.0/10
7. [DeepSeek Harness developer preview released](#item-tech-news-7) ⭐️ 7.0/10
8. [City2Graph: A Python library for heterogeneous graph neural networks and urban analysis](#item-tech-news-8) ⭐️ 7.0/10
9. [Worldproof tool shows pixel metrics can&\#x27;t rank world models on robot video](#item-tech-news-9) ⭐️ 7.0/10
10. [Trump Memo Lets Private Firms Run US-Backed Overseas Cyber Ops](#item-tech-news-10) ⭐️ 7.0/10

**Financial News**
1. [S&amp;P 500 profit margins hit record high, FactSet says](#item-finance-news-1) ⭐️ 8.0/10
2. [YMTC becomes No. 3 in NAND chip shipments, passing Micron and Kioxia](#item-finance-news-2) ⭐️ 8.0/10
3. [China’s gig jobs rise above 53 million as economy slows, report says](#item-finance-news-3) ⭐️ 8.0/10
4. [CXMT Overtakes Tencent to Become China’s Most Valuable Company](#item-finance-news-4) ⭐️ 8.0/10
5. [Bill Ackman&\#x27;s Pershing Square buys Netflix again, saying it has won streaming](#item-finance-news-5) ⭐️ 7.0/10
6. [EVs now dominate China&\#x27;s new car sales, data show](#item-finance-news-6) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Gemini 3.7 Flash Launches With New Pricing and Strong Test Results](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-3-7-flash/) ⭐️ 8.0/10

Google introduced Gemini 3.7 Flash, an incremental update to its Flash model line now available through the Gemini API. It follows Gemini 3.6 Flash by roughly three weeks, with introductory pricing set to double on December 31, 2026; from January 1, 2027, pricing is listed as $1.50 per million input tokens and $7.50 per million output tokens. Early community tests report strong image-to-HTML and coding results, including solid performance on the DeepSWE 1.1 benchmark, although commenters still rate Anthropic&\#x27;s Opus and OpenAI&\#x27;s Luna as stronger in some tasks. The update matters for developers who want a low-cost, high-volume model for text workflows, but it is not a major version change.

hackernews · thisisauserid · Aug 13, 17:23 · [Discussion](https://news.ycombinator.com/item?id=49289112)

**「Background」** Google’s Gemini Flash series is a line of lower-cost, high-volume AI models designed for coding, agents, and everyday text-based tasks. Gemini 3.7 Flash launched on August 13, 2026, just three weeks after the previous 3.6 Flash release, and is rolling out to the Gemini app&\#x27;s Spark tier for Google AI Pro and Ultra subscribers. At launch, it is priced at $0.75 per million input tokens and $3.75 per million output tokens—half the introductory price of the prior model—with those prices scheduled to double on January 1, 2027.

**「Impact」** For developers, the immediate consequence is a temporary 50% price cut: Gemini 3.7 Flash launched on August 13, 2026 at $0.75 per million input tokens and $3.75 per million output tokens, with pricing scheduled to double on December 31, 2026, making high-volume coding and agent workloads cheaper for the next several months.

**「Community Discussion」** Commenters generally agreed Gemini 3.7 Flash is capable and price-competitive for vision-assisted coding, but several found the doubling introductory pricing odd so soon after 3.6 Flash, and compared it unfavorably with cheaper or stronger rivals such as GPT-5.6 Luna. Some also called for clearer benchmarks against Luna/Terra.

<details><summary>References</summary>
<ul>
<li><a href="https://9to5google.com/2026/08/13/gemini-3-7-flash-launch/">Gemini 3 . 7 Flash launches three weeks after last model</a></li>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-3-7-flash/">Gemini 3 . 7 Flash : our most intelligent workhorse model</a></li>
<li><a href="https://www.studioglobal.ai/discover/answers/search-6a7e4ad110551e202b12954c">Google Gemini 3.7 Flash: Pricing, Benchmarks, and the ...</a></li>
<li><a href="https://www.neowin.net/news/google-joins-the-ai-model-price-war-with-the-new-gemini-37-flash/">Google joins the AI model price war with the new Gemini 3.7 Flash</a></li>

</ul>
</details>

**Tags**: `#gemini`, `#google`, `#machine-learning`, `#llm`, `#ai`

---

<a id="item-tech-news-2"></a>
### [Spaghettifying DRAM: AMD Memory-Controller Exploit Surfaces](https://github.com/xoreaxeaxeax/skitter-creek-bath-salts) ⭐️ 8.0/10

The GitHub project &quot;Spaghettifying DRAM&quot; by security researcher Christopher Domas \(xoreaxeaxeax\) presents an exploitation tool that abuses DRAM and memory-controller behavior, apparently detailed in an upcoming Black Hat talk. Based on the README and community comments, the technique works against the AMD Jaguar architecture from 2013 and is mapped to AMD16h; notes indicate Zen 3 uses a different memory-controller register base address, leaving newer CPU compatibility unclear. The research highlights the growing attack surface in modern DRAM, which now requires proprietary binary blobs and far more complexity than older RAS/CAS interfaces. Community responses emphasize that once ring-0 access is achieved on affected systems, attackers may reach capabilities long considered protected in &quot;negative ring&quot; territory, potentially raising concerns for game-console security. The repository does not yet state which other processor families might be similarly affected.

hackernews · matt\_d · Aug 13, 14:17 · [Discussion](https://news.ycombinator.com/item?id=49286341)

**「Background」** DRAM scrambling is a memory-controller feature in modern CPUs that obscures the mapping between physical addresses and physical DRAM cells, usually presented as a security hardening measure. The &\#x27;skitter-creek-bath-salts&\#x27; project by researcher xoreaxeaxeax \(Christopher Domas\) demonstrates that this scrambling mechanism can instead be exploited to unlock CPU internals that vendors leave undocumented, including PSP, C6, microcode, and SMM. The README documents support for AMD 16h \(Jaguar-era\) parts, with notes that newer architectures such as Zen 3 use a different base address for memory controller registers.

**「Impact」** On AMD Jaguar \(Family 16h\) systems, the proof-of-concept demonstrates that ring-0 code can manipulate DRAM address scrambling registers to bypass hardware security fences and reach protected memory regions, undermining assumptions that DRAM-level protections are opaque to privileged software. The released notes do not establish whether this applies to newer families such as Zen 3.

**「Community Discussion」** Commenters are excited for the accompanying Black Hat talk and praise Domas&\#x27;s prior reverse-engineering work, while also questioning how far the attack extends beyond older AMD parts such as Jaguar and Zen 3. Several speculate that Xbox and PlayStation security teams could be concerned, since ring-0 access on those systems may expose hidden privileges.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/xoreaxeaxeax/skitter-creek-bath-salts">GitHub - xoreaxeaxeax / skitter - creek - bath - salts : Unlocking...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Jaguar_%28microarchitecture%29">Jaguar (microarchitecture) - Wikipedia</a></li>
<li><a href="https://news.linxi.com.au/news/amd-hardware-vulnerability-exposed-by-dram-address-scrambling-research">AMD DRAM Scrambling Exploit Bypasses Security Fences | Linxi News</a></li>

</ul>
</details>

**Tags**: `#security`, `#DRAM`, `#hardware hacking`, `#exploit`, `#reverse engineering`

---

<a id="item-tech-news-3"></a>
### [Choose Boring Technology: Spend Your Innovation Tokens Wisely](https://mcfunley.com/choose-boring-technology) ⭐️ 8.0/10

The 2015 essay &quot;Choose Boring Technology&quot; argues that teams should deliberately pick mature, well-understood tools so they can reserve their limited &quot;innovation tokens&quot; for the few areas where novelty genuinely matters. It frames engineering strategy as a fixed budget: roughly three innovation tokens per company for a long while, so spending them on infrastructure leaves little for user-facing differentiation. The essay is a classic, widely influential technology-choice framework and is now being reapplied to modern AI agent development, where the surrounding stack should stay boring while novelty is concentrated in agent behavior. The guidance is practical: avoid using a slightly better new language or tool when its unfamiliarity and operational risk will outweigh the modest gain.

hackernews · tosh · Aug 13, 17:48 · [Discussion](https://news.ycombinator.com/item?id=49289512)

**「Background」** This item is Dan McKinley&\#x27;s 2015 essay &\#x27;Choose Boring Technology,&\#x27; which argues that software teams should deliberately favor mature, well-understood technologies \(the &\#x27;boring&\#x27; options\) in most areas and reserve their limited &\#x27;innovation tokens&\#x27; for the few problems where novelty genuinely matters. The essay emerged from McKinley&\#x27;s experience as an engineer and engineering leader at companies like Etsy and Stripe, and it has become a widely referenced mental model in software engineering culture for countering technology trend-chasing. A spoken-word version and an expanded slide-based edition were later published on the same site.

**「Impact」** For engineering leaders and product managers, the innovation-tokens concept provides a shared language for justifying technical tradeoffs across all levels, and in current discussions it suggests that teams building AI agents should standardize on boring, in-distribution technology so that their scarce novelty budget goes into the agent layer itself.

**「Community Discussion」** Commenters largely praise the framework, with one calling it one of the most useful concepts they&\#x27;ve had as a PM/eng leader, while others wish for job boards that vet companies for this pragmatic culture. Revisiting it for AI agents, a commenter advises pushing all innovation tokens into agents and using boring tech for the rest, though one pushes back that &quot;innovation tokens&quot; is arbitrary and that novelty should be evaluated by requirements and risk rather than age.

<details><summary>References</summary>
<ul>
<li><a href="https://mcfunley.com/choose-boring-technology">Choose Boring Technology - Dan McKinley</a></li>
<li><a href="https://boringtechnology.club/">Choose Boring Technology</a></li>

</ul>
</details>

**Tags**: `#software-engineering`, `#technology-strategy`, `#engineering-culture`, `#innovation-tokens`, `#boring-technology`

---

<a id="item-tech-news-4"></a>
### [DeepSeek V4 Pro 0813 Released with Open Weights on Hugging Face](https://simonwillison.net/2026/Aug/12/deepseek-v4-pro-0813/) ⭐️ 8.0/10

DeepSeek&\#x27;s V4 Pro 0813 model is now available through API providers such as OpenRouter, and its open weights have been released on Hugging Face as deepseek-ai/DeepSeek-V4-Pro-0813, totaling 1.7T parameters and 893 GB. The model is the latest in DeepSeek&\#x27;s Pro line and follows the April DeepSeek-V4-Pro and July DeepSeek-V4-Flash-0731 releases, which also had open weights. Simon Willison reports that the model produced noticeably different outputs across low, medium, and high reasoning levels, which he had not observed from other models. Benchmark figures appear to have been shared only through unofficial channels, including an official DeepSeek WeChat group and later an ASCII-art table on Hacker News, after a Reddit post was deleted for being low-effort.

rss · Simon Willison · Aug 12, 23:59

**「Background」** DeepSeek is a Chinese AI research lab known for releasing open-weight language models, often at large scale. Previous versions in the V4 family, such as DeepSeek-V4-Pro and DeepSeek-V4-Flash, were also made available as open weights on Hugging Face, allowing developers and researchers to self-host and fine-tune the models. The new V4 Pro 0813 continues this pattern, offering an API-first release alongside downloadable weights.

**「Impact」** Developers and researchers who rely on open-weight models can now access DeepSeek V4 Pro 0813 either via API or by downloading its 893 GB checkpoint, though the model&\#x27;s size will require substantial GPU resources for local deployment. The absence of an official announcement and formal benchmark publication may complicate evaluation for teams planning to adopt the model, but the availability of weights on Hugging Face lowers the barrier for independent testing.

**Tags**: `#deepseek`, `#open-source`, `#language-model`, `#ai`, `#api`

---

<a id="item-tech-news-5"></a>
### [DeepMind launches SL2T sign-language-to-text AI on Pixel 11](https://deepmind.google/blog/putting-sign-language-ai-into-users-hands/) ⭐️ 8.0/10

Google DeepMind unveiled SL2T, a large-scale multilingual sign-language-to-text model, and shipped its first consumer deployment on the Pixel 11: ASL-to-English translation in Gboard and Live Transcribe. The model was trained on over 100,000 hours of sign-language video spanning more than 50 sign languages, and it scores 70 BLEURT zero-shot on the FLEURS-ASL benchmark, well above the prior record. To protect privacy, SL2T operates on hand and body keypoints rather than raw video. Additional devices and languages are planned, but the initial rollout is limited to ASL-to-English on Pixel 11.

telegram · zaihuapd · Aug 13, 08:55

**「Background」** Sign-language-to-text AI translates video of signing into written language, but such systems typically require large datasets and can raise privacy concerns. SL2T addresses both by training on a vast multilingual corpus and using only hand and body keypoints instead of raw video. BLEURT is a learned metric for evaluating text quality, and zero-shot evaluation measures performance without fine-tuning on the target language.

**「Impact」** Pixel 11 owners who use ASL can now convert signing into English text in Gboard and Live Transcribe, a first consumer deployment of DeepMind&\#x27;s sign-language AI. Other devices and languages are planned but not yet available, so the immediate impact is limited to ASL users on Pixel 11.

**Tags**: `#sign language`, `#DeepMind`, `#accessibility`, `#machine translation`, `#consumer AI`

---

<a id="item-tech-news-6"></a>
### [OpenAI Previews Ultrafast Mode, GPT-5.6 Sol Up to 14x Faster](https://openai.com/index/previewing-ultrafast/) ⭐️ 8.0/10

OpenAI has previewed a new Ultrafast mode that runs GPT-5.6 Sol up to 14 times faster than standard processing, with output reaching 750 tokens per second. The service is powered by Cerebras hardware and is initially available through the OpenAI API to a limited set of customers. OpenAI says the faster inference targets time-sensitive applications such as incident response, financial research, customer service, and e-commerce. Access is currently restricted, and OpenAI plans to expand availability as compute capacity grows.

telegram · zaihuapd · Aug 13, 17:04

**「Background」** OpenAI&\#x27;s GPT-5.6 Sol is offered through the OpenAI API, and Ultrafast is a newly previewed service tier that uses Cerebras&\#x27; Wafer-Scale Engine hardware instead of standard processing. This tier targets latency-sensitive workloads such as incident response, financial research, customer support, and e-commerce, promising up to 14x faster generation and up to 750 output tokens per second.

**「Impact」** Affected API customers in the preview can now use GPT-5.6 Sol for latency-critical workloads that were previously impractical, though broader availability remains dependent on compute expansion.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/previewing-ultrafast/">Previewing Ultrafast mode : GPT - 5 . 6 Sol at up to 14 X the... | OpenAI</a></li>
<li><a href="https://www.youtube.com/watch?v=WCwT4gWpHmI">Previewing Ultrafast mode : GPT ‑ 5 . 6 Sol at up to 14 X the... - YouTube</a></li>
<li><a href="https://www.neowin.net/news/openai-introduces-new-ultrafast-mode-for-gpt56-sol-delivering-14x-faster-tokens/">OpenAI introduces new Ultrafast mode for GPT ‑ 5 . 6 Sol ... - Neowin</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#GPT-5.6`, `#Cerebras`, `#AI inference`, `#performance`

---

<a id="item-tech-news-7"></a>
### [DeepSeek Harness developer preview released](https://deepseek.com/harness/en/) ⭐️ 7.0/10

DeepSeek released an early open-source developer preview of its Harness agentic framework under the MIT license, alongside an accompanying paper. The preview emphasizes full traceability, recording everything the model sees in an append-only session log, and a hot-reload plugin system that can dynamically enable, disable, and revert plugin state without restarting. The framework is built on Cordis v4, which has been used for years in the Koishi project, and supports plugin-driven architecture covering UI components and other subsystems. The authors warn it is rough, with compatibility-breaking changes expected, but invite feedback from the community.

hackernews · bjin · Aug 13, 12:58 · [Discussion](https://news.ycombinator.com/item?id=49285244)

**「Background」** An agentic harness is a runtime framework that orchestrates AI agents, managing their context, tool use, subagent scheduling, and execution logs. Plugin systems in such frameworks normally require reloading the process to activate or deactivate components; Cordis addresses this with dynamic hot-reload and state rollback, which DeepSeek Harness applies broadly to its architecture.

**「Impact」** Developers adopting this preview can expect a powerful but unstable foundation, with notable features like full run traceability and plugin hot-reload, though they should plan for frequent breaking changes as the framework matures.

**「Community Discussion」** Commenters highlight the traceability feature as a standout, noting that some US model traces are encrypted or obfuscated, while others express skepticism about the practical utility beyond plugin hot-reload and warn of plugin fatigue from over-architected systems. One author responds that it is an early preview with rough edges and welcomes feedback.

**Tags**: `#deepseek`, `#open-source`, `#agentic-harness`, `#traceability`, `#developer-preview`

---

<a id="item-tech-news-8"></a>
### [City2Graph: A Python library for heterogeneous graph neural networks and urban analysis](https://www.reddit.com/r/MachineLearning/comments/1vn8oya/city2graph_a_python_library_for_heterogeneous/) ⭐️ 7.0/10

City2Graph is a new open-source Python library that converts geospatial urban data into heterogeneous graphs for spatial analysis, network analysis, and Graph Neural Networks. The accompanying paper by Sato, Pietrostefani, Mahabir, and Arribas-Bel was published in Computers, Environment and Urban Systems, volume 130, article 102492, in 2026. The library supports morphological graphs from OpenStreetMap and Overture Maps, GTFS and GBFS transit feeds via DuckDB, OD matrices and flow data, and proximity/contiguity graphs with multiple distance metrics. It also provides conversions between GeoDataFrames, NetworkX, rustworkx, and PyTorch Geometric, preserving geometries and attributes across round trips, and supports heterogeneous node and edge types with metapath-derived edges. The project is hosted on GitHub and welcomes issues and pull requests.

reddit · r/MachineLearning · /u/Tough\_Ad\_6598 · Aug 13, 11:59

**「Background」** Urban data are often stored as tabular geometries—buildings, road segments, or transit stops—that do not naturally express relationships such as adjacency, connectivity, or flow. Graph representations make those relationships explicit, and heterogeneous graphs allow multiple types of nodes \(e.g., buildings and streets\) and edges \(e.g., proximity and transit\) to coexist in one structure. City2Graph bridges this gap by generating such graphs directly from common urban data sources and packaging them for graph neural network frameworks.

**「Impact」** Urban computing and GeoAI researchers can use City2Graph to construct analysis-ready heterogeneous graphs from OpenStreetMap, Overture Maps, GTFS, and GBFS data, reducing the amount of custom code needed to feed such data into PyTorch Geometric models.

**Tags**: `#graph-neural-networks`, `#geospatial`, `#urban-computing`, `#python-library`, `#geoai`

---

<a id="item-tech-news-9"></a>
### [Worldproof tool shows pixel metrics can&\#x27;t rank world models on robot video](https://www.reddit.com/r/MachineLearning/comments/1vnliv7/worldproof_diagnosing_where_worldmodel/) ⭐️ 7.0/10

Worldproof is a new open-source diagnostic tool for world models that predict future frames, and its author reports a striking validation finding: a trivial last-frame baseline achieves near-perfect pixel metrics on real robot video. On a SO-101 arm recording \(30fps, three cameras, 64 rollouts, 6-step horizon, scored only on moving regions\), the baseline got 0.983 SSIM and 53.9 dB PSNR with flat per-step errors, meaning all models tie and the evaluation cannot rank them. On DROID footage \(15fps, 64 rollouts, 48 steps\), the baseline was only separable between roughly steps 8 and 24; before that everything ties, and after step 28 it floors around 0.20 SSIM and 10.3 dB with no trend. The tool is Apache-2.0, installable via &\#x27;pip install worldproof&\#x27;, reads LeRobotDataset v3.0 from parquet and mp4, runs on a laptop without a GPU, and reports horizon curves rather than relying on horizon-averaged scalars, which can be inflated by an easy first step.

reddit · r/MachineLearning · /u/georgia\_bucea · Aug 13, 19:58

**「Background」** World models are predictive models that generate future frames from a starting context and a sequence of actions, and they are typically evaluated with pixel-similarity metrics such as SSIM and PSNR. DROID is a large-scale, in-the-wild robot manipulation dataset containing 76k demonstration trajectories collected across hundreds of scenes, commonly used for benchmarking such models. The post&\#x27;s evaluation also relies on interquartile mean and stratified bootstrap confidence intervals, a statistical approach promoted by the Rliable library to improve reliability in reinforcement learning and related evaluations.

**「Impact」** Developers evaluating video-prediction or world models on similar real-robot data should avoid default pixel-metric comparisons and horizon-averaged scalars, and instead measure the separable horizon window on their own data — for DROID-like footage that window is roughly 8 to 24 steps.

<details><summary>References</summary>
<ul>
<li><a href="https://www.opodab.com/2026/08/deep-rl-benchmarking-iqm-stratified.html">Stop Reporting Mean Scores: The IQM &amp; Rliable Guide That...</a></li>
<li><a href="https://aihub.org/2022/01/19/rliable-towards-reliable-evaluation-and-reporting-in-reinforcement-learning/">RLiable: towards reliable evaluation and reporting in reinforcement...</a></li>
<li><a href="https://giters.com/UltronAI/rliable">UltronAI/rliable - Giters</a></li>
<li><a href="https://droid-dataset.github.io/">DROID: A Large-Scale In-the-Wild Robot Manipulation Dataset</a></li>
<li><a href="https://arxiv.org/abs/2403.12945">[2403.12945] DROID: A Large-Scale In-The-Wild Robot Manipulation Dataset</a></li>
<li><a href="https://arxiv.org/html/2403.12945v2">DROID: A Large-Scale In-The-Wild Robot Manipulation Dataset https://droid-dataset.github.io</a></li>

</ul>
</details>

**Tags**: `#world models`, `#model evaluation`, `#pixel metrics`, `#robotics`, `#open-source tool`

---

<a id="item-tech-news-10"></a>
### [Trump Memo Lets Private Firms Run US-Backed Overseas Cyber Ops](https://www.bloomberg.com/news/articles/2026-08-13/trump-enlists-private-sector-to-boost-cyber-offensive-arsenal) ⭐️ 7.0/10

President Trump signed a memorandum authorizing private companies under direct federal control and supervision to conduct US government-backed overseas surveillance and cyber attacks against foreign transnational cybercrime organizations targeting Americans. The Department of Homeland Security will run the program and coordinate oversight with the Department of Justice. Participating firms must maintain at least $1 million in surety bonds or escrow funds, which will be forfeited if they fail to comply with contract terms. This policy expands the private sector&\#x27;s role in government-supported offensive cyber operations.

telegram · zaihuapd · Aug 13, 05:10

**「Background」** The Trump administration signed a national security presidential memorandum on August 13, 2026, directing federal agencies to leverage private-sector capabilities for offensive cyber operations against overseas criminals. This is reportedly the first time the U.S. government has authorized private companies to conduct offensive cyberattacks, expanding an area previously reserved for government agencies.

**「Impact」** The memorandum immediately expands the commercial offensive-cyber market by letting vetted private companies run US-government-backed overseas surveillance and hacking under DHS/DOJ oversight, a move cybersecurity executives describe as a major shift toward private-sector offensive operations even though it stops short of full &\#x27;hack back&\#x27;; former Cyber Command officials warn it could create a &\#x27;perpetual motion machine for billable threats.&\#x27;

<details><summary>References</summary>
<ul>
<li><a href="https://www.theguardian.com/us-news/2026/aug/13/donald-trump-private-companies-cyber-attack">Donald Trump empowers US private companies to... | The Guardian</a></li>
<li><a href="https://arstechnica.com/security/2026/08/white-house-recruits-security-firms-to-hack-overseas-cybercriminals/">Private security firms will soon be allowed to hack overseas ...</a></li>
<li><a href="https://cyberscoop.com/trump-memo-private-sector-offensive-hacking/">Trump turns to private sector in offensive hacking operations memo | CyberScoop</a></li>
<li><a href="https://www.infosecurity-magazine.com/news/trump-private-offensive-cyber/">Trump Authorizes Private Sector Participation in Offensive Cyber Opera - Infosecurity Magazine</a></li>

</ul>
</details>

**Tags**: `#cybersecurity`, `#surveillance`, `#cyber policy`, `#private sector`, `#offensive cyber operations`

---

## Financial News

<a id="item-finance-news-1"></a>
### [S&amp;P 500 profit margins hit record high, FactSet says](https://www.cnbc.com/2026/08/13/these-charts-show-why-stocks-keep-rallying-profit-margins-are-highest-on-record.html) ⭐️ 8.0/10

S&amp;P 500 companies are estimated to have reached a record-high net profit margin of 16.9% in the second quarter of 2026, up from 14.8% in the first quarter and 12.9% a year earlier, according to FactSet data cited by CNBC.

rss · CNBC Finance · Aug 13, 20:21

**「Background」** Net profit margin is the share of revenue companies keep after paying all expenses; FactSet has tracked the S&amp;P 500 metric since 2009. The latest figure is a blended estimate that partly reflects company reports and partly Wall Street forecasts.

**Tags**: `#S&amp;P 500`, `#profit margins`, `#corporate earnings`, `#stock market`, `#FactSet`

---

<a id="item-finance-news-2"></a>
### [YMTC becomes No. 3 in NAND chip shipments, passing Micron and Kioxia](https://www.cnbc.com/2026/08/13/chinese-firm-tops-micron-kioxia-shipments-nand-memory-chips.html) ⭐️ 8.0/10

Chinese memory maker YMTC became the world’s third-largest shipper of NAND memory chips in Q2 2026, with a 14% share, according to Counterpoint Research, behind Samsung and SK hynix and ahead of Micron and Kioxia.

rss · CNBC Finance · Aug 13, 02:59

**「Background」** NAND chips store data without power but are slower and cheaper than DRAM; YMTC is preparing to list in mainland China after rival CXMT’s recent debut.

**「Impact」** Although YMTC’s shipment share rose, its NAND revenue still trails Micron and Kioxia because it sells more to consumer products than data centers.

**Tags**: `#NAND memory`, `#YMTC`, `#semiconductor market`, `#China tech`, `#competitive dynamics`

---

<a id="item-finance-news-3"></a>
### [China’s gig jobs rise above 53 million as economy slows, report says](https://www.ft.com/content/a3803e70-cb4d-444f-a31e-05be2f2c44f6?accessToken=zwAAAZ_5xcXzkdOjgD5wy01ET9OjHgW-LyxE9g.MEUCIQCWTIny3JTJV8e-PGyK0XL2tg5g_7Ay-rpKkwGZCpp1-AIgbMgJQPlqWgqAsX4s1k4gYaC4b8k0JveZOs35OJQvbZ4&amp;amp;sharetype=gift&amp;amp;token=7e8483bb-395d-429e-afca-2f4ab5ad150b) ⭐️ 8.0/10

The Financial Times reports that China’s economic slowdown pushed the number of delivery and ride-hailing drivers above 53 million as of 2025, an increase of 10 million in two years; even so, oversupply is pushing down incomes and lengthening work hours.

telegram · zaihuapd · Aug 13, 06:40

**「Background」** A property downturn, weak consumer spending, manufacturing and construction contraction, and automation have pushed surplus labor into the gig economy, and Shenzhen declared its ride-hailing market saturated in June.

**「Impact」** Gig workers, especially drivers and couriers, are bearing the immediate effects through lower pay and longer waiting times, with airport taxi queues in Shanghai, Beijing and Chengdu lasting up to 7, 8 and 10 hours respectively.

**Tags**: `#China economy`, `#gig economy`, `#employment`, `#labor market`, `#ride-hailing`

---

<a id="item-finance-news-4"></a>
### [CXMT Overtakes Tencent to Become China’s Most Valuable Company](https://www.bloomberg.com/news/articles/2026-08-13/cxmt-overtakes-tencent-to-become-most-valuable-chinese-company) ⭐️ 8.0/10

Bloomberg reports that Chinese memory-chip maker CXMT overtook Tencent to become the most valuable Chinese company, with a market value of $524 billion compared with Tencent’s $510 billion. CXMT listed in Shanghai last month and surged 467% on its first day of trading.

telegram · zaihuapd · Aug 13, 10:10

**「Background」** ChangXin Memory Technologies \(CXMT\) is a Chinese memory-chip maker that listed on the Shanghai exchange last month after its shares surged 467% on the first day of trading. Tencent, the Hong Kong-listed internet giant, has fallen this year as it steps up AI investment.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tomshardware.com/tech-industry/cxmt-overtakes-tencent-to-become-chinas-most-valuable-company-17-days-after-its-ipo">Memory maker CXMT overtakes Tencent to become China&#x27;s most valuable company 17 days after its IPO — now worth $524 billion | Tom&#x27;s Hardware</a></li>

</ul>
</details>

**Tags**: `#CXMT`, `#Tencent`, `#Chinese equities`, `#semiconductors`, `#IPO`

---

<a id="item-finance-news-5"></a>
### [Bill Ackman&\#x27;s Pershing Square buys Netflix again, saying it has won streaming](https://www.cnbc.com/2026/08/13/ackman-buys-netflix-again-four-years-later-says-it-won-streaming-wars.html) ⭐️ 7.0/10

Bill Ackman&\#x27;s Pershing Square disclosed a new Netflix position in its semiannual report, arguing that Netflix has effectively won the streaming wars. Pershing said Netflix has more than 325 million subscribers and called its valuation attractive at about 21 times forward earnings after a roughly 50% decline from the June 2025 high.

rss · CNBC Finance · Aug 13, 18:04

**「Background」** Ackman previously bought Netflix in early 2022 but sold the entire stake about three months later after Netflix reported its first subscriber decline in more than a decade.

**Tags**: `#Bill Ackman`, `#Netflix`, `#Pershing Square`, `#streaming`, `#investment`

---

<a id="item-finance-news-6"></a>
### [EVs now dominate China&\#x27;s new car sales, data show](https://www.cnbc.com/2026/08/12/china-car-sales-data-byd-tesla-geely-vw.html) ⭐️ 7.0/10

China&\#x27;s latest auto sales data show electric dominance: new energy vehicles—battery and hybrid cars—accounted for 65.1% of new passenger cars sold in July, up from 54% a year earlier, while overall passenger-car sales fell 20.3% for the year through July, according to China Passenger Car Association data. Geely&\#x27;s Xingyuan was the top-selling model in the six months through July, with nearly 197,500 units sold, per Autohome.

rss · CNBC Finance · Aug 13, 01:31

**「Background」** The figures follow a period of intense competition in China&\#x27;s auto market, with EV-focused brands such as BYD, Geely, and Tesla gaining share from traditional gasoline-car makers.

**Tags**: `#China auto sales`, `#electric vehicles`, `#BYD`, `#Tesla`, `#Geely`

---