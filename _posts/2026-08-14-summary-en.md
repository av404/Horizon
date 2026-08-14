---
layout: default
title: "Horizon Summary: 2026-08-14 (EN)"
date: 2026-08-14
lang: en
---

> From 48 items, 22 important content pieces were selected

---

**Technology News**
1. [Spaghettifying DRAM: Hardware Attack Undermines Memory Isolation](#item-tech-news-1) ⭐️ 9.0/10
2. [GLM-5.3: Z.AI&\#x27;s Frontier Coding Model With Emergent Cyber Capabilities](#item-tech-news-2) ⭐️ 8.0/10
3. [Cerebras and OpenAI Claim ~7x Faster GPT-5.6 Sol Ultrafast Reasoning](#item-tech-news-3) ⭐️ 8.0/10
4. [systemd-journald write amplification: 49KB+ per log line on ext4](#item-tech-news-4) ⭐️ 8.0/10
5. [worldproof: Diagnosing World-Model Failures and Pixel-Metric Limits](#item-tech-news-5) ⭐️ 8.0/10
6. [DeepMind SL2T brings sign language-to-text to Pixel 11 keyboard and captions](#item-tech-news-6) ⭐️ 8.0/10
7. [DeepSeek Harness Released; V4-Pro-0813 Weights Open](#item-tech-news-7) ⭐️ 8.0/10
8. [X Opens More of Its Ranking Algorithm and Adds Transparency Check](#item-tech-news-8) ⭐️ 8.0/10
9. [Gemini 3.7 Flash Arrives with Vision Strength and Time-Limited Pricing](#item-tech-news-9) ⭐️ 7.0/10
10. [Bluesky Introduces Jetstream for Easier AT Protocol Development](#item-tech-news-10) ⭐️ 7.0/10
11. [Understanding Is the New Bottleneck in AI-Assisted Coding](#item-tech-news-11) ⭐️ 7.0/10
12. [Choose Boring Technology and Spend Innovation Tokens Wisely](#item-tech-news-12) ⭐️ 7.0/10
13. [NP-hardness Overrated in Practice?](#item-tech-news-13) ⭐️ 7.0/10
14. [Following 657,607 Links Reveals Where the Old Web Went](#item-tech-news-14) ⭐️ 7.0/10
15. [City2Graph: Open-Source Python Library for Urban Heterogeneous Graphs and GNNs](#item-tech-news-15) ⭐️ 7.0/10
16. [AI Robot Labs Test 3M Human Tissue Samples Yearly, Could Replace Animal Testing](#item-tech-news-16) ⭐️ 7.0/10

**Financial News**
1. [Bill Ackman&\#x27;s Pershing Square buys Netflix stake again, saying it has won the streaming wars](#item-finance-news-1) ⭐️ 8.0/10
2. [CXMT Overtakes Tencent as China’s Most Valuable Company](#item-finance-news-2) ⭐️ 8.0/10
3. [Uber and Pony.ai plan 2,000 robotaxis in Europe](#item-finance-news-3) ⭐️ 7.0/10
4. [S&amp;P 500 profit margins hit record 16.9% in Q2, FactSet says](#item-finance-news-4) ⭐️ 7.0/10
5. [U.S. President Announces Drone Tariffs Up to 100% on Some Imports](#item-finance-news-5) ⭐️ 7.0/10
6. [Apple Proposes Up to 15% Commission for Off-App-Store Purchases in the US](#item-finance-news-6) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Spaghettifying DRAM: Hardware Attack Undermines Memory Isolation](https://github.com/xoreaxeaxeax/skitter-creek-bath-salts) ⭐️ 9.0/10

Christopher Domas released a hardware security research project, &\#x27;skitter-creek-bath-salts&\#x27;, demonstrating a DRAM exploitation technique that undermines memory isolation and poses serious security implications. The work, accompanied by a Black Hat talk, exposes a DRAM attack surface that could enable privilege escalation on affected systems. Community discussion notes the README identifies AMD Jaguar \(a 2013 architecture\) as affected, with notes about Zen 3 having a different memory controller register base address; the full scope across newer CPUs remains unclear. The research is significant because it targets hardware-level isolation, potentially exposing negative-ring functionality to ring-0 root on vulnerable machines.

hackernews · matt\_d · Aug 13, 14:17 · [Discussion](https://news.ycombinator.com/item?id=49286341)

**「Background」** DRAM scrambling is a hardware feature that obfuscates the mapping between CPU physical addresses and DRAM cells, making it harder for software to infer the physical layout of memory. Christopher Domas \(@xoreaxeaxeax\) has released a research project, skitter-creek-bath-salts, that demonstrates a technique for reversing or bypassing this scrambling on certain AMD processors—notably the AMD16h \(Jaguar\) family—allowing code with ring-0 privileges to break memory isolation and access data reserved for more privileged layers, such as hypervisors or SMM. The work is associated with an upcoming Black Hat 2026 talk, &\#x27;Spaghettifying DRAM,&\#x27; and notes that newer families like Zen 3 have different base addresses for the memory controller registers, leaving the full scope of affected CPUs unspecified.

**「Impact」** The README identifies AMD Jaguar \(16h\) as an affected family, where the technique lets an already ring-0 attacker bypass memory isolation and access data held in the processor&\#x27;s negative-ring territory; commenters noted that Jaguar-based game consoles could be especially exposed, while newer CPUs remain unconfirmed because only a Zen 3 memory-controller register base address change is noted. No confirmed impact on Intel or newer AMD families has been disclosed in the item.

**「Community Discussion」** Commenters expressed high anticipation for the accompanying Black Hat talk, praising Christopher Domas&\#x27;s past research presentations. Concerns focused on the attack surface of modern DRAM, potential impact on game consoles like Xbox and PlayStation after gaining ring-0, and uncertainty about which newer CPU families beyond AMD Jaguar are affected.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/xoreaxeaxeax/skitter-creek-bath-salts">GitHub - xoreaxeaxeax/skitter-creek-bath-salts: Unlocking _everything_ on the CPU with DRAM scrambling · GitHub</a></li>

</ul>
</details>

**Tags**: `#DRAM`, `#hardware security`, `#exploit`, `#privilege escalation`, `#security research`

---

<a id="item-tech-news-2"></a>
### [GLM-5.3: Z.AI&\#x27;s Frontier Coding Model With Emergent Cyber Capabilities](https://z.ai/blog/glm-5.3) ⭐️ 8.0/10

Z.AI announced GLM-5.3 in a blog post presenting it as a frontier coding model with emergent cyber capabilities, achieved through post-training scaling rather than a new base model. The company positions GLM-5.3 as competitive with leading closed models and highlights open-weight availability, giving developers and researchers a credible alternative to proprietary APIs. The release notes that capability gains are uneven: while coding performance is strong, the largest remaining gaps to closed frontiers appear on benchmarks that sit further up the exploitation chain. This matters because it demonstrates that post-training alone can produce near-frontier results across coding and security-related tasks, potentially reducing reliance on closed providers.

hackernews · pella · Aug 14, 05:19 · [Discussion](https://news.ycombinator.com/item?id=49294997)

**「Background」** GLM is a series of large language models developed by Z.ai \(formerly Zhipu AI\), known for offering open-weight versions that can run locally as well as API access through subscription plans like the GLM Coding Plan. GLM-5.3, announced on August 14, 2026, keeps the same base model as GLM-5.2 and derives all improvements from scaled-up post-training, with a focus on coding and emergent cybersecurity capabilities. This release builds on GLM-5.2&\#x27;s reputation for competitive performance against leading closed models at lower cost.

**「Impact」** For AI engineers, researchers, and security teams, GLM-5.3 offers a near-frontier open-weight model that can be evaluated, adapted, and potentially run locally in quantized form, lowering barriers to high-end coding and cyber-capability research.

**「Community discussion」** Commenters were impressed but measured, noting that GLM-5.3 is only slightly behind leading proprietary models and that the blog post reads like researcher-authored material rather than marketing hype. Some questioned whether the performance jump justifies switching away from existing providers, pointed out that GLM-5.3 is effectively GLM-5.2 plus post-training scaling, and discussed running the model locally in heavily quantized forms once weights are available.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GLM_%28AI%29">GLM (AI) - Wikipedia</a></li>
<li><a href="https://explainx.ai/blog/glm-5-3-launch-cyber-defense-benchmarks-august-2026">GLM-5.3 Launch: Benchmarks, Pricing &amp; Access (Aug 2026) | explainx.ai Blog | explainx.ai</a></li>
<li><a href="https://www.unite.ai/z-ai-launches-glm-5-3-with-frontier-coding-and-a-cyber-capability-that-outgrew-its-training/">Z.ai Launches GLM-5.3 With Frontier Coding and a Cyber Capability That Outgrew Its Training – Unite.AI</a></li>

</ul>
</details>

**Tags**: `#GLM-5.3`, `#artificial intelligence`, `#machine learning`, `#coding`, `#cybersecurity`

---

<a id="item-tech-news-3"></a>
### [Cerebras and OpenAI Claim ~7x Faster GPT-5.6 Sol Ultrafast Reasoning](https://www.cerebras.ai/blog/accelerating-gpt-5-6-sol-ultrafast-with-openai) ⭐️ 8.0/10

OpenAI and Cerebras announced a collaboration delivering &\#x27;Ultrafast&\#x27; inference for GPT-5.6 Sol. In vendor-published HLE evaluations, Ultrafast answered all 2,500 questions in 11 hours and 11 minutes, versus 78 hours and 27 minutes for Claude Fable 5, roughly 7x faster at comparable accuracy. Cerebras also cites external output-speed comparisons suggesting 11x faster than Fable 5 and 5x faster than Opus 4.8 on Fast mode. Neither post states outright that accuracy is exactly identical to regular GPT-5.6 Sol, and pricing details have not been disclosed, so the benchmarks remain vendor claims awaiting independent verification.

hackernews · pr337h4m · Aug 13, 18:10 · [Discussion](https://news.ycombinator.com/item?id=49289844)

**「Background」** Cerebras Systems builds ultra-large wafer-scale AI accelerators designed to deliver extremely high token-generation throughput, and OpenAI has now partnered with Cerebras to offer &quot;Ultrafast mode&quot; for its GPT-5.6 Sol model through the OpenAI API. This mode reportedly achieves up to 750 output tokens per second, targeting frontier-level reasoning tasks such as the HLE \(Humanity&\#x27;s Last Exam\) benchmark, where Cerebras claims the model answered all 2,500 questions in 11 hours and 11 minutes versus 78 hours and 27 minutes for Claude Fable 5. The announcement follows earlier OpenAI previews of Ultrafast technology and broader industry efforts to reduce inference latency, but pricing details have not yet been published.

**「Impact」** For GPT-5.6 Sol users, Ultrafast could make multi-hour frontier reasoning tasks practical within a working day and enable more iterative &\#x27;thinking&\#x27; workflows, but pricing and independent verification are still missing.

**「Community Discussion」** Hacker News commenters were enthusiastic but cautious: some welcomed the speed and its potential for iterative reasoning, while others noted the absence of pricing and that neither Cerebras nor OpenAI explicitly confirmed Ultrafast is performance-identical to regular GPT-5.6 Sol.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cerebras.ai/blog/accelerating-gpt-5-6-sol-ultrafast-with-openai">Accelerating GPT-5.6 Sol Ultrafast with OpenAI</a></li>
<li><a href="https://www.globenewswire.com/news-release/2026/08/13/3344804/0/en/cerebras-powers-ultrafast-mode-for-openai-s-gpt-5-6-sol.html">Cerebras Powers Ultrafast Mode for OpenAI’s GPT-5.6 Sol</a></li>
<li><a href="https://openai.com/index/previewing-ultrafast/">Previewing Ultrafast mode: GPT-5.6 Sol at up to 14X the speed | OpenAI</a></li>

</ul>
</details>

**Tags**: `#AI`, `#hardware`, `#inference acceleration`, `#OpenAI`, `#Cerebras`

---

<a id="item-tech-news-4"></a>
### [systemd-journald write amplification: 49KB+ per log line on ext4](https://github.com/systemd/systemd/issues/40262) ⭐️ 8.0/10

A GitHub issue \(systemd/systemd\#40262\) reports that systemd-journald can cause massive disk write amplification, writing roughly 49KB or more per single log line on ext4 and 110KB or more on btrfs. The report highlights a significant performance and storage-efficiency concern in a core Linux logging component, and it has drawn broad community attention on Hacker News \(199 points and 124 comments\). The exact causes and conditions behind the per-line write sizes remain tied to the issue report, but the measurements indicate journald&\#x27;s persistent storage format can add large overhead compared with the log message itself. This matters for system administrators because journald is widely used as the default logger on many Linux distributions, making storage I/O and wear a practical concern.

hackernews · ValdikSS · Aug 13, 18:41 · [Discussion](https://news.ycombinator.com/item?id=49290215)

**「Background」** systemd-journald is the logging daemon in systemd-based Linux systems, responsible for collecting and storing log entries in a binary journal format. Traditionally, its design emphasizes append-only writes and mmap-based access for robustness and atomicity, but this issue reports that writing a single log line can cause over 49 KB of disk writes on ext4 and over 110 KB on btrfs, highlighting significant write amplification and performance concerns.

**「Impact」** System administrators using persistent journald storage may face considerably higher disk I/O and storage wear than the size of their log messages suggests, especially on btrfs where the reported overhead is larger. Some users already recommend treating journald as a router and forwarding logs to tools such as rsyslog precisely because of this kind of overhead.

**「Community discussion」** Commenters broadly criticize journald&\#x27;s indexing and storage design, calling it slow and lacking practical controls per log identifier or subsystem, with one noting the current behavior seems far from the original append-only design intent. The common recommendation is to avoid persistent journald storage and instead forward logs to external tools for filtering and retention.

<details><summary>References</summary>
<ul>
<li><a href="https://zeli.app/en/story/49290215">systemd - journald writes 49 KB + per log line on ext 4 , 110KB+ on btrfs ...</a></li>

</ul>
</details>

**Tags**: `#systemd`, `#journald`, `#logging`, `#performance`, `#linux`

---

<a id="item-tech-news-5"></a>
### [worldproof: Diagnosing World-Model Failures and Pixel-Metric Limits](https://www.reddit.com/r/MachineLearning/comments/1vnliv7/worldproof_diagnosing_where_worldmodel/) ⭐️ 8.0/10

A new open-source tool, worldproof, diagnoses world-model prediction failures by comparing rollouts against ground truth and physical invariants. Its author found that pixel metrics often cannot rank models on real robot video: a trivial last-frame baseline achieves 0.983 SSIM and 53.9 dB PSNR on a SO-101 arm recording at 30fps, with error that does not grow over a 6-step horizon. On DROID footage, a usable evaluation window exists only around steps 8-24, with dynamic-region SSIM declining monotonically from 0.873 at step 1 to a floor near 0.20 after step 28. The tool is Apache-2.0, installable via pip, runs on a CPU-only laptop, uses n=64 rollouts with interquartile-mean aggregation and bootstrap CIs, and reports LPIPS diverging from other metrics on masked variants for reasons not yet explained.

reddit · r/MachineLearning · /u/georgia\_bucea · Aug 13, 19:58

**「Background」** World models predict future frames from a starting context and an action sequence, and they are commonly evaluated with pixel-level similarity metrics such as SSIM and PSNR. This post introduces a diagnostic tool and demonstrates that on real robot video those metrics can lack discriminative power, making a &\#x27;predict nothing changes&\#x27; baseline competitive with trained models over short horizons.

**「Impact」** For researchers evaluating world models or video predictors on real robot data, this work means pixel metrics like SSIM/PSNR over entire horizons cannot rank models—so evaluations should focus on the separable 8-to-24-step window on DROID-like 15 fps footage \(or an equivalent measured window for their own data\) and should report horizon curves rather than summary scalars, a practice the open-source worldproof tool now supports.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/pdf/1911.01655">High Fidelity Video Prediction with</a></li>

</ul>
</details>

**Tags**: `#world-models`, `#video-prediction`, `#evaluation-metrics`, `#open-source`, `#machine-learning`

---

<a id="item-tech-news-6"></a>
### [DeepMind SL2T brings sign language-to-text to Pixel 11 keyboard and captions](https://deepmind.google/blog/putting-sign-language-ai-into-users-hands/) ⭐️ 8.0/10

Google DeepMind has released SL2T, a large multilingual sign language-to-text model, and integrated it into consumer products for the first time by launching it on the Pixel 11&\#x27;s Gboard keyboard and Live Transcribe real-time captions. The initial deployment supports American Sign Language to English, with plans to expand to more devices and languages. SL2T was trained on over 100,000 hours of data spanning more than 50 sign languages, and it achieves a zero-shot score of 70 BLEURT on the FLEURS-ASL benchmark, far exceeding the previous record. To protect privacy, the model processes only hand and body pose keypoints rather than raw video. This marks the first time DeepMind&\#x27;s sign language AI has been made available directly in consumer devices.

telegram · zaihuapd · Aug 13, 08:55

**「Background」** Sign language translation AI has traditionally struggled with limited data and the need to generalize across many signing styles and languages. DeepMind&\#x27;s new SL2T model is a large-scale multilingual sign-language-to-text model trained on over 100,000 hours of data and 50+ sign languages, using hand and body pose keypoints instead of raw video to protect privacy. It currently supports American Sign Language to English and is debuting in Gboard and Live Transcribe on Pixel 11, with more languages and device support planned.

**「Impact」** Pixel 11 users can now use the first consumer sign language-to-text AI to convert American Sign Language into English through Gboard and Live Transcribe, with privacy preserved because only keypoints are analyzed instead of the original video feed.

<details><summary>References</summary>
<ul>
<li><a href="https://deepmind.google/blog/putting-sign-language-ai-into-users-hands/">Putting sign language AI into users’ hands</a></li>
<li><a href="https://www.cryptopolitan.com/google-deepmind-sign-language-on-pixel-11/">Google DeepMind ships SL2T sign-language model on Pixel 11 - Cryptopolitan</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Sign Language`, `#DeepMind`, `#Accessibility`, `#Machine Learning`

---

<a id="item-tech-news-7"></a>
### [DeepSeek Harness Released; V4-Pro-0813 Weights Open](https://mp.weixin.qq.com/s/mANdGRI4fO_sEbC1ECEoZQ) ⭐️ 8.0/10

DeepSeek released DeepSeek Harness as an MIT-licensed open-source application and opened the DeepSeek-V4-Pro-0813 model weights on Hugging Face. The Harness uses an everything-is-a-plugin architecture driven by Cordis, allowing models, tools, skills, sessions, sandboxes, storage, scheduling, and UI components to be swapped as plugins, and offers four running modes: Standard, PTC, Minimal, and Creative. The GitHub repository and npm package are available, with the GitHub repo initially appearing later in the day. The Hugging Face model page transiently returned a 404 before being restored. The release is described by an author as an early developer preview with expected rough edges and compatibility-breaking changes.

telegram · zaihuapd · Aug 13, 12:39

**「Background」** DeepSeek is an AI research and development organization known for releasing open-weight large language models. Harness applications in this context typically bundle an agent runtime with model access, tools, session management, and user interfaces; DeepSeek Harness extends that by making every component a hot-swappable plugin through the Cordis plugin framework.

**「Impact」** Developers and agent builders can now inspect and customize a complete agent stack under an MIT license, including append-only session logs that record system prompts, reasoning, tool calls, results, subagent scheduling, and context injections. The open weights for DeepSeek-V4-Pro-0813 provide an alternative for users who want full traceability without the encrypted or obfuscated traces typical of US-based model offerings, though the model page&\#x27;s temporary 404 leaves some uncertainty about long-term availability.

**「Community Discussion」** Commenters highlighted the traceability feature as a standout capability that US models do not allow, and explained that Cordis enables hot-loading and unloading of plugins with state rollback. Others expressed caution: the project is an early preview likely to have breaking changes, one reader found the underlying paper only moderately useful, and another voiced fatigue with products built around an everything-is-a-plugin architecture.

**Tags**: `#DeepSeek`, `#open-source`, `#AI model`, `#Hugging Face`, `#LLM`

---

<a id="item-tech-news-8"></a>
### [X Opens More of Its Ranking Algorithm and Adds Transparency Check](https://techcrunch.com/2026/08/13/x-open-sources-its-ranking-algorithm-letting-users-see-if-theyve-been-shadowbanned/) ⭐️ 8.0/10

X announced an expansion of its open-source efforts by publishing the code for its “For You” timeline and core ranking engine on GitHub under the Apache 2.0 license, with the released code roughly 10 to 15 times larger than previous releases. The company also introduced a transparency tool in its settings that lets users who have posted at least 10 times in the past month download a JSON file showing whether their account or posts have been flagged by ranking systems. The tool is initially available only to test users whose accounts have been registered for at least one year. Some Grok systems used to determine rule-violating content were not disclosed as part of this release, so the open-sourced code does not cover all ranking-related components.

telegram · zaihuapd · Aug 14, 01:03

**「Context」** X \(formerly Twitter\) has a history of partially open-sourcing its recommendation system, but this release expands that effort to include the code behind the “For You” feed and core ranking engine, published under the Apache 2.0 license on GitHub at xai-org/x-algorithm. The new transparency tool is designed to address longstanding “shadowbanning” concerns by letting users check whether their account or posts have been downranked or otherwise affected by the platform&\#x27;s ranking systems. This tool gives eligible accounts a downloadable JSON file showing such impacts, complementing the open-source code with user-facing insight.

**「Impact」** Eligible X users can now check whether their content has been affected by ranking flags, while developers gain access to a substantially larger portion of the ranking engine for audit and research. However, because the Grok-based moderation components remain private, the transparency and auditability are still incomplete.

<details><summary>References</summary>
<ul>
<li><a href="https://techcrunch.com/2026/08/13/x-open-sources-its-ranking-algorithm-letting-users-see-if-theyve-been-shadowbanned/">X open sources its ranking algorithm, letting users see if they&#x27;ve been &#x27;shadowbanned&#x27; | TechCrunch</a></li>
<li><a href="https://www.firstpost.com/tech/x-open-sources-its-ranking-algorithm-lets-users-check-account-level-impacts-14038070.html">X open-sources its ranking algorithm, lets users check account-level impacts</a></li>
<li><a href="https://github.com/xai-org/x-algorithm">GitHub - xai-org/x-algorithm: Algorithm powering the For You feed on X · GitHub</a></li>

</ul>
</details>

**Tags**: `#open-source`, `#ranking-algorithm`, `#transparency`, `#social-media`, `#AI`

---

<a id="item-tech-news-9"></a>
### [Gemini 3.7 Flash Arrives with Vision Strength and Time-Limited Pricing](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-3-7-flash/) ⭐️ 7.0/10

Google introduced Gemini 3.7 Flash, a new API model with competitive vision performance and introductory pricing that is scheduled to double on December 31, 2026; starting January 1, 2027, pricing becomes $1.50 per million input tokens and $7.50 per million output tokens. The model arrives only three weeks after Gemini 3.6 Flash, reflecting Google&\#x27;s rapid release cadence. Early community tests show it handles vision tasks such as image-to-HTML well and performs strongly on the DeepSWE 1.1 benchmark, though commenters note it remains more expensive than GPT-5.6 Luna and call for direct benchmarks against Luna and Terra.

hackernews · thisisauserid · Aug 13, 17:23 · [Discussion](https://news.ycombinator.com/item?id=49289112)

**「Background」** Gemini 3.7 Flash is Google&\#x27;s latest low-cost addition to its Flash model line, released on August 13, 2026, with introductory pricing of $0.75 per million input tokens and $3.75 per million output tokens—a 50% discount versus the post-introductory price of the prior 3.6 Flash model. Google positions it against models such as OpenAI&\#x27;s GPT-5.6 Terra and Muse Spark 1.2 on benchmarks, while OpenAI&\#x27;s two-tier GPT-5.6 lineup includes the cheaper, faster Luna tier, which received an 80% price cut and is relevant to comparisons developers have made.

**「Impact」** Developers who use Flash-series models for low-cost, high-volume text and vision workloads will face a doubled API price in 2027, while cheaper alternatives such as GPT-5.6 Luna may reduce Gemini 3.7 Flash&\#x27;s cost-effectiveness for budget-sensitive applications.

**「Community Discussion」** Commenters shared hands-on tests showing Gemini 3.7 Flash performs well on vision and code-related benchmarks, but several questioned the odd introductory pricing, noted that GPT-5.6 Luna remains cheaper and stronger on benchmarks like DeepSWE 1.1, and argued the Flash lineup is undercut by more cost-efficient rivals.

<details><summary>References</summary>
<ul>
<li><a href="https://felloai.com/gemini-3-7-flash/">Gemini 3.7 Flash: Pricing, Benchmarks and What Changed</a></li>
<li><a href="https://officechai.com/ai/gemini-3-7-flash-benchmarks/">Google Releases Gemini 3.7 Flash, Competes With GPT 5.6 Terra &amp; Muse Spark 1.2 On Benchmarks</a></li>
<li><a href="https://muirouter.com/blog/gpt-5-6-price-cut">OpenAI Price Cut: GPT - 5 . 6 Luna &amp; Terra Drop Up to 80% | MuiRouter</a></li>
<li><a href="https://openai.com/index/gpt-5-6/">GPT - 5 . 6 : Frontier intelligence that scales with your ambition | OpenAI</a></li>

</ul>
</details>

**Tags**: `#gemini`, `#google ai`, `#model release`, `#vision`, `#api pricing`

---

<a id="item-tech-news-10"></a>
### [Bluesky Introduces Jetstream for Easier AT Protocol Development](https://atproto.com/blog/introducing-bluesky-protocol-services) ⭐️ 7.0/10

Bluesky has announced new protocol services for the AT Protocol, including Jetstream, a service designed to make it easier to consume the Bluesky firehose. The announcement is aimed at developers building on the decentralized social protocol, providing infrastructure that simplifies real-time data access. Jetstream lowers the barrier to entry by allowing direct consumption in browsers without requiring a server, as demonstrated by a developer who updated their browser-based firehose demo. This move supports the broader ecosystem of third-party developers and open-source tooling around the AT Protocol.

hackernews · danabramov · Aug 14, 00:14 · [Discussion](https://news.ycombinator.com/item?id=49293324)

**「Background」** Bluesky is built on the AT Protocol, whose real-time firehose streams all repository events to consumers \(tool-1-1\). The raw firehose uses CBOR binary encoding, which can be difficult to work with, so Bluesky built Jetstream, an open-source Go server that consumes the firehose and fans out to subscribers as simpler JSON events over a websocket \(tool-1-2, tool-1-3\). Jetstream therefore makes it much easier for developers to consume the firehose and build applications on the protocol.

**「Impact」** Developers building on the AT Protocol can now consume the Bluesky firehose directly in a browser without a server, significantly simplifying the creation of real-time Bluesky clients and demos.

**「Community Discussion」** Developers reacted positively to Jetstream&\#x27;s ease of use, with one noting it can be consumed directly in the browser, while others raised concerns about Bluesky&\#x27;s long-term funding and profitability and one developer complained about the atproto Python library&\#x27;s developer experience.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.bsky.app/docs/advanced-guides/firehose">Firehose | Bluesky</a></li>
<li><a href="https://docs.bsky.app/blog/jetstream">Introducing Jetstream | Bluesky</a></li>
<li><a href="https://getskyscraper.com/blog/bluesky-firehose-streaming-guide">Bluesky Firehose Explained: Real-Time Data Streaming Guide</a></li>

</ul>
</details>

**Tags**: `#bluesky`, `#atproto`, `#decentralized-social`, `#protocol`, `#open-source`

---

<a id="item-tech-news-11"></a>
### [Understanding Is the New Bottleneck in AI-Assisted Coding](https://www.geoffreylitt.com/2026/07/02/understanding-is-the-new-bottleneck) ⭐️ 7.0/10

The essay &\#x27;Understanding is the new bottleneck&\#x27; argues that as LLMs automate code generation, the critical constraint in software development is becoming human understanding of codebases, not writing code. It contends that the ability to review, reason about, and maintain software now matters more than generation speed. The article includes concrete examples and has drawn broad Hacker News discussion, with 160 comments engaging with its implications for engineering practice. The core claim is that developers&\#x27; comprehension is the limiting factor for safely integrating AI-generated code.

hackernews · sebg · Aug 13, 18:47 · [Discussion](https://news.ycombinator.com/item?id=49290299)

**「Background」** The article is a written version of a talk Geoffrey Litt, a design engineer at Notion, gave at the AI Engineer conference in July 2026. It argues that as LLMs automate code generation, the critical bottleneck in software development is shifting from writing code to human understanding of codebases. Litt suggests techniques such as explanations, micro-worlds, and shared spaces to help developers comprehend AI-generated code.

**「Impact」** For software engineers relying on LLM-generated code, the concrete consequence is that production commits now depend on the developer&\#x27;s own review and understanding of the change, since an LLM cannot take responsibility for the outcome.

**「Community Discussion」** Commenters broadly agree that understanding codebases is the real constraint, but they disagree about whether the problem is new or whether LLM-generated summaries are useful. Several note the bottleneck predates LLMs—citing specs and testing in corporate settings—and warn that using LLMs to generate understanding means losing the human check that catches incorrect code.

<details><summary>References</summary>
<ul>
<li><a href="https://www.geoffreylitt.com/2026/07/02/understanding-is-the-new-bottleneck">Understanding is the new bottleneck</a></li>
<li><a href="https://www.startuphub.ai/ai-news/artificial-intelligence/2026/understanding-is-the-new-bottleneck-in-ai">Understanding is the New Bottleneck in AI | StartupHub.ai</a></li>

</ul>
</details>

**Tags**: `#software engineering`, `#LLM`, `#code understanding`, `#developer productivity`, `#AI-assisted development`

---

<a id="item-tech-news-12"></a>
### [Choose Boring Technology and Spend Innovation Tokens Wisely](https://mcfunley.com/choose-boring-technology) ⭐️ 7.0/10

The 2015 essay &\#x27;Choose Boring Technology&\#x27; argues that organizations have a fixed supply of &\#x27;innovation tokens&\#x27;—about three per company—and should spend them only on technologies that differentiate their product, choosing boring, proven tools for everything else. The framework helps teams reserve limited capacity for meaningful innovation instead of chasing novelty. The post remains influential in engineering strategy discussions, including recent debates about applying the idea to AI agents by keeping the stack boring while concentrating innovation on agent capabilities. The Hacker News thread shows both strong endorsement from PM and engineering leaders and criticism that the token model is an arbitrary proxy that can blur real tradeoff analysis.

hackernews · tosh · Aug 13, 17:48 · [Discussion](https://news.ycombinator.com/item?id=49289512)

**「Background」** Dan McKinley&\#x27;s 2015 essay &\#x27;Choose Boring Technology&\#x27; argues that companies have a limited budget for innovation, metaphorically &\#x27;innovation tokens,&\#x27; and should spend them only on novel technologies that provide a competitive edge while adopting proven, &\#x27;boring&\#x27; tools for everything else. The piece emerged from McKinley&\#x27;s experience at Etsy and reflects the era&\#x27;s JavaScript framework churn, advocating for conservative tech choices to preserve capacity for meaningful innovation.

**「Impact」** Practicing engineers and product managers report using the innovation-token model to explain technology tradeoffs to colleagues at all levels, providing a shared vocabulary for defending conservative stack choices.

**「Community Discussion」** Commenters largely praise the innovation-token concept as a practical communication tool for tradeoffs, while some push back that &\#x27;new vs. boring&\#x27; is a weak proxy that oversimplifies engineering decisions. Others extend the idea to AI agents, suggesting that keeping the underlying stack boring maximizes the value of innovating on agent technology.

<details><summary>References</summary>
<ul>
<li><a href="https://mcfunley.com/choose-boring-technology">Dan McKinley :: Choose Boring Technology</a></li>
<li><a href="https://news.ycombinator.com/item?id=49289512">Choose Boring Technology ( 2015 ) | Hacker News</a></li>

</ul>
</details>

**Tags**: `#software-engineering`, `#technology-strategy`, `#engineering-culture`, `#tradeoffs`

---

<a id="item-tech-news-13"></a>
### [NP-hardness Overrated in Practice?](https://gruhn.me/blog/2026-08-13/) ⭐️ 7.0/10

A blog post at gruhn.me/blog/2026-08-13 argues that NP-hardness is overrated for practical algorithmic problem solving. It contends that the exponential worst-case blowups associated with NP-hard problems often depend on adversarial inputs that rarely occur in real applications. The post therefore advocates heuristic solution techniques and careful formulation of problem instances, rather than treating NP-hardness as a reason to give up. The argument is relevant to software engineers and algorithm designers who routinely encounter packing, scheduling, type-checking, and dependency-resolution problems.

hackernews · theanonymousone · Aug 13, 20:14 · [Discussion](https://news.ycombinator.com/item?id=49291268)

**「Background」** Computational complexity theory classifies problems by how quickly algorithms can solve them as input grows. NP-hard problems are among the hardest: no known efficient polynomial-time algorithm exists for them, and exact solutions can require exponential time in the worst case. In practice, many NP-hard instances encountered in software engineering, such as dependency resolution or type checking, may not hit these explosive worst-case configurations, so heuristics and approximate solvers often work well enough.

**「Impact」** For software engineers facing NP-hard problems like dependency resolution or type checking, the post supports the practical tactic of avoiding or eliminating explosive instances instead of attempting a general solution.

**「Community Discussion」** Commenters largely agreed that practical instances usually avoid NP-hard explosions and that heuristics can work, but several pushed back that complexity classes are still important for theoretical understanding and for recognizing when general problems are &\#x27;impossible&\#x27; unless you eliminate hard configurations. Guvante specifically noted that dependency managers and type systems often block or cordon off entire hard problem spaces, while pron drew an analogy to calculus and stressed that NP-complete is actually on the easier end of some much harder classes.

<details><summary>References</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=49291268">NP - Overrated | Hacker News</a></li>

</ul>
</details>

**Tags**: `#algorithms`, `#complexity theory`, `#NP-hard`, `#software engineering`, `#heuristics`

---

<a id="item-tech-news-14"></a>
### [Following 657,607 Links Reveals Where the Old Web Went](https://0.mk/blog/link-rot) ⭐️ 7.0/10

A data-driven investigation tracked 657,607 links to map link rot and the disappearance of older web content. The study examines where old web pages have gone and the patterns behind web decay, offering a quantitative look at internet history and preservation. The analysis is especially relevant to web developers, archivists, and historians of the internet, though it is not a fundamental paradigm shift. The supplied item does not include specific decay rates or concrete breakdowns, so the exact findings remain unverified.

hackernews · tdx · Aug 13, 17:49 · [Discussion](https://news.ycombinator.com/item?id=49289532)

**「Background」** Link rot is the process by which hyperlinks gradually become unusable, typically because the target page is removed or moved without a redirect, leaving a 404 error. Web archives like the Wayback Machine mitigate this by saving periodic snapshots of pages, though they have limitations such as incomplete coverage or missing interactive elements. This study follows 657,607 links to measure how much of the old web has vanished and to identify patterns in link decay.

**「Impact」** By quantifying link rot at this scale, the analysis gives archivists and developers evidence for prioritizing preservation and link-maintenance efforts, although the absence of specific figures in the summary means the practical scale of decay cannot be precisely stated.

**「Community Discussion」** Commenters mainly debate which era counts as the &\#x27;old web,&\#x27; with suggestions ranging from the pre-Google years, the pre-Facebook blogosphere, and 2009–2014. One commenter counters that websites were always ephemeral &\#x27;shopping windows&\#x27; that change or disappear, so permanence was never guaranteed.

<details><summary>References</summary>
<ul>
<li><a href="https://web.archive.org/web/20250214072411/https://en.wikipedia.org/wiki/Wikipedia:Link_rot">Wikipedia: Link rot - Wikipedia</a></li>
<li><a href="https://waybackmachine.org.im/">Wayback Machine Official: Archived Web Pages and Internet History</a></li>
<li><a href="https://hdware.blog/the-legacy-of-old-bom-websites-a-digital-time-capsule/">The Legacy of Old BOM Websites : A Digital Time Capsule - Hdware</a></li>

</ul>
</details>

**Tags**: `#link-rot`, `#web-preservation`, `#internet-history`, `#data-analysis`, `#web-archiving`

---

<a id="item-tech-news-15"></a>
### [City2Graph: Open-Source Python Library for Urban Heterogeneous Graphs and GNNs](https://www.reddit.com/r/MachineLearning/comments/1vn8oya/city2graph_a_python_library_for_heterogeneous/) ⭐️ 7.0/10

City2Graph is a new Python library that converts geospatial data into analysis-ready heterogeneous graphs for spatial analysis, network analysis, and graph neural networks \(GeoAI\). It builds morphological graphs from OpenStreetMap and Overture Maps, transportation graphs from GTFS and GBFS feeds via DuckDB, mobility and OD flow graphs, and proximity or contiguity graphs \(KNN, Delaunay, Gilbert, Waxman, queen/rook\) under Euclidean, Manhattan, or network distances. The library supports multiple node and edge types with metapath-derived edges and provides conversions between GeoDataFrames, NetworkX, rustworkx, and PyTorch Geometric Data/HeteroData while preserving geometries and attributes. A paper describing the library was published in Computers, Environment and Urban Systems \(volume 130, article 102492\). The project aims to fill a gap in GeoAI tooling by treating urban data as heterogeneous graphs rather than flat feature tables.

reddit · r/MachineLearning · /u/Tough\_Ad\_6598 · Aug 13, 11:59

**「Background」** Heterogeneous graphs contain multiple types of nodes and edges, which are useful for modeling urban systems where buildings, streets, transit stops, and flows have different relationships. Graph neural networks operate on such graph structures, but geospatial data is often stored as flat tables or shapefiles, requiring preprocessing to create graph representations. City2Graph provides ready-made construction functions to bridge this gap.

**「Impact」** Researchers and developers in urban analytics and GeoAI can now standardize the conversion of geographic data into heterogeneous graphs for graph neural networks, reducing duplicated effort and improving reproducibility. The published paper provides a citable reference for academic use.

**Tags**: `#graph-neural-networks`, `#geospatial`, `#python`, `#urban-systems`, `#geoai`

---

<a id="item-tech-news-16"></a>
### [AI Robot Labs Test 3M Human Tissue Samples Yearly, Could Replace Animal Testing](https://www.fastcompany.com/91589344/the-worlds-largest-biological-datacenter-could-help-make-animal-testing-obsolete) ⭐️ 7.0/10

Vivodyne operates robot laboratories south of San Francisco that grow human tissues in closet-sized &quot;hive&quot; setups; its 12 hive labs can run more than 3 million controlled human-tissue tests per year, roughly twice the capacity of all U.S. clinical trials combined. The company says AI designs experiments to better predict drug efficacy and safety, addressing the roughly 90% of clinical trials that fail even after animal testing. If validated, this approach could substantially reduce or eventually eliminate reliance on animal testing, though these claims are company-sourced and not yet independently proven.

telegram · zaihuapd · Aug 14, 01:48

**「Background」** Vivodyne is a biotech company that grows lab-grown human tissues and uses robotic labs to run large-scale biological experiments, generating multi-omic data such as imaging, transcriptomics, and proteomics. The company recently raised $40 million to expand its AI-powered human tissue testing platform, which it describes as the world&\#x27;s largest human biological datacenter. This approach aims to replace or reduce reliance on animal testing, which historically fails to predict human drug responses—about 90% of clinical trials fail after animal testing—by creating rich physiological datasets that can train AI models to better predict drug efficacy and safety.

**「Impact」** For pharmaceutical and biotech researchers, scaling AI-driven human-tissue testing offers a potential path to more predictive preclinical screens and reduced reliance on animal models, but real-world impact depends on independent validation and regulatory acceptance.

<details><summary>References</summary>
<ul>
<li><a href="https://www.vivodyne.com/">Vivodyne | Make biology computable</a></li>
<li><a href="https://hlth.com/insights/news/vivodyne-raises-40m-to-transform-drug-development-with-ai-powered-human-tissue-testing-2025-06-03">Vivodyne Raises $40M to Transform Drug Development with...</a></li>
<li><a href="https://www.bastillepost.com/global/article/6076655-vivodyne-launches-the-worlds-largest-human-biological-datacenter-to-train-the-first-world-model-of-human-biology">Vivodyne Launches the World’s Largest Human Biological Datacenter...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#biotech`, `#robotics`, `#drug discovery`, `#lab automation`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Bill Ackman&\#x27;s Pershing Square buys Netflix stake again, saying it has won the streaming wars](https://www.cnbc.com/2026/08/13/ackman-buys-netflix-again-four-years-later-says-it-won-streaming-wars.html) ⭐️ 8.0/10

Bill Ackman&\#x27;s Pershing Square said it has taken a new stake in Netflix, arguing the company has won the streaming wars after its valuation dropped to about 21 times expected future earnings from more than 40 times. Pershing Square disclosed the position in a semiannual report, noting that Netflix&\#x27;s shares are roughly 50% below their June 2025 high of $134.

rss · CNBC Finance · Aug 13, 18:04

**「Background」** Ackman had built a Netflix position in early 2022 but sold the entire stake about three months later after Netflix reported its first subscriber decline in more than a decade.

**Tags**: `#Netflix`, `#Bill Ackman`, `#Pershing Square`, `#Streaming`, `#Valuation`

---

<a id="item-finance-news-2"></a>
### [CXMT Overtakes Tencent as China’s Most Valuable Company](https://www.bloomberg.com/news/articles/2026-08-13/cxmt-overtakes-tencent-to-become-most-valuable-chinese-company) ⭐️ 8.0/10

CXMT, the Chinese memory-chip maker, has overtaken Tencent to become China’s most valuable listed company: its market capitalization was $524 billion after Thursday’s 1.2% decline, versus Tencent’s $510 billion, according to Bloomberg. The milestone follows CXMT’s Shanghai listing last month, when its shares jumped 467% on the first day and another 8% afterward, while Tencent has fallen more than 26% this year as it increases AI spending.

telegram · zaihuapd · Aug 13, 10:10

**「Background」** CXMT is a Chinese maker of DRAM memory chips based in Hefei; it listed on the Shanghai exchange last month, jumping about 466% on its debut and raising $9.8 billion, making it China&\#x27;s largest onshore-listed company.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ChangXin_Memory_Technologies">ChangXin Memory Technologies - Wikipedia</a></li>
<li><a href="https://www.linkedin.com/posts/huiyu-winnie-hsu-wh950316_tech-memory-semiconductor-activity-7487436737384771584-UhzD">CXMT IPO : China&#x27;s Largest Onshore-Listed Company ... | LinkedIn</a></li>

</ul>
</details>

**Tags**: `#CXMT`, `#Tencent`, `#China market cap`, `#semiconductor`, `#IPO`

---

<a id="item-finance-news-3"></a>
### [Uber and Pony.ai plan 2,000 robotaxis in Europe](https://www.cnbc.com/2026/08/14/uber-partners-with-chinas-ponyai-for-2000-robotaxis-in-europe.html) ⭐️ 7.0/10

Uber and Pony.ai announced Friday plans to deploy 2,000 of Pony.ai&\#x27;s self-driving taxis in four additional European cities and expand their robotaxi partnership to the Middle East, building on the Zagreb, Croatia service they launched in late March and describe as Europe&\#x27;s first.

rss · CNBC Finance · Aug 14, 01:02

**「Background」** The companies did not name the other cities or give an exact timeline, and the expansion comes as Alphabet-backed Waymo, with about 5,000 vehicles mostly in the U.S., tests in London and prepares for global operations.

**Tags**: `#Uber`, `#Pony.ai`, `#Robotaxi`, `#Autonomous Vehicles`, `#Europe`

---

<a id="item-finance-news-4"></a>
### [S&amp;P 500 profit margins hit record 16.9% in Q2, FactSet says](https://www.cnbc.com/2026/08/13/these-charts-show-why-stocks-keep-rallying-profit-margins-are-highest-on-record.html) ⭐️ 7.0/10

The S&amp;P 500&\#x27;s estimated net profit margin for the second quarter is 16.9%, up from 12.9% a year earlier and the highest since FactSet began tracking the measure in 2009, according to FactSet data cited by CNBC.

rss · CNBC Finance · Aug 13, 20:21

**「Background」** Net profit margin is the share of sales left after all expenses; Alphabet and Amazon were the biggest contributors, helped partly by large one-time gains, but even excluding them the margin was a record 15%, according to FactSet.

**「Impact」** The gains were broad-based across eight of the 11 S&amp;P 500 sectors, though Vanguard economist Adam Schickling cautions that rising competition in technology could pressure margins in that sector in the future.

**Tags**: `#S&amp;P 500`, `#profit margins`, `#corporate earnings`, `#FactSet data`, `#stock market`

---

<a id="item-finance-news-5"></a>
### [U.S. President Announces Drone Tariffs Up to 100% on Some Imports](https://www.whitehouse.gov/presidential-actions/2026/08/adjusting-imports-of-unmanned-aircraft-systems-and-unmanned-aircraft-systems-components-into-the-united-states/) ⭐️ 7.0/10

The U.S. president signed a proclamation on Aug. 13 imposing tariffs on imported drones and components: from Sept. 3, 2026, drones over 25 kg maximum takeoff weight, drones with thermal imagers, drone base stations, and certain key components will face 100% duties, while drones of 25 kg or less will face 25%. A separate 25% tariff on other drone components will take effect Feb. 9, 2027, with the Commerce secretary authorized to expand coverage.

telegram · zaihuapd · Aug 14, 01:24

**「Background」** The White House said the measures are intended to expand domestic drone production and reduce reliance on foreign sources for critical components, with analysts highlighting China as a key supplier.

**「Impact」** The new tariffs could raise costs for U.S. importers, businesses, and agencies that buy imported drones, especially Chinese-made models already facing combined duties around 170%, potentially pushing up prices and reshaping the U.S. drone market.

<details><summary>References</summary>
<ul>
<li><a href="https://www.aa.com.tr/en/world/trump-imposes-tariffs-of-up-to-100-on-imported-drones-components/4027001">Trump imposes tariffs of up to 100 % on imported drones , components</a></li>
<li><a href="https://www.bloomberg.com/news/articles/2026-08-13/trump-imposes-100-tariffs-on-certain-drones-countering-china">Trump Imposes 100 % Tariffs on Some Drones ... - Bloomberg</a></li>
<li><a href="https://www.datamintelligence.com/news/trump-drone-tariffs-2026-impact-on-global-drone-market-us-china-uav-supply-chain">Trump Drone Tariffs 2026: 100% Duty on Chinese UAV Imports ...</a></li>
<li><a href="https://www.dslrpros.com/blogs/drone-trends/the-impact-of-tariffs-and-geopolitical-challenges-on-the-drone-industry">The Impact of Tariffs and Geopolitical Challenges on the Drone ...</a></li>

</ul>
</details>

**Tags**: `#tariffs`, `#drones`, `#trade policy`, `#United States`, `#import duties`

---

<a id="item-finance-news-6"></a>
### [Apple Proposes Up to 15% Commission for Off-App-Store Purchases in the US](https://9to5mac.com/2026/08/13/apple-proposes-commissions-of-up-to-15-for-off-app-store-purchases-in-the-us/) ⭐️ 7.0/10

Apple has filed a court proposal that would charge US developers commissions of up to 15% for purchases made outside the App Store, with rates of 15% for standard apps, 10% for subscriptions and certain video/news partners, and 5% for small business program apps. This is a proposal subject to court review, not a final policy.

telegram · zaihuapd · Aug 14, 02:33

**「Background」** The proposal was filed in Apple’s ongoing litigation with Epic Games, after the US Supreme Court declined Apple’s request to pause lower-court proceedings on fee rates.

**Tags**: `#Apple`, `#App Store`, `#regulation`, `#Epic Games`, `#commissions`

---