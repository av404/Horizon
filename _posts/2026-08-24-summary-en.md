---
layout: default
title: "Horizon Summary: 2026-08-24 (EN)"
date: 2026-08-24
lang: en
---

> From 44 items, 12 important content pieces were selected

---

**Technology News**
1. [seL4 Security Proofs Completed on AArch64](#item-tech-news-1) ⭐️ 9.0/10
2. [MS Paint and Photos Embed Hidden GUID Watermarks in AI Edits](#item-tech-news-2) ⭐️ 8.0/10
3. [Does NVIDIA&\#x27;s CUDA Moat Hold in Agentic Inference?](#item-tech-news-3) ⭐️ 8.0/10
4. [Xiaomi Unveils Three Xuanjie Chips; O3 SoC to Debut in Xiaomi 18 Fold](#item-tech-news-4) ⭐️ 8.0/10
5. [AI Coding Reliance May Collapse Developer Expertise](#item-tech-news-5) ⭐️ 7.0/10
6. [Executable as a SQLite Database](#item-tech-news-6) ⭐️ 7.0/10
7. [Bart: A 2.82B Vintage LLM Trained on Pre-1931 English Text](#item-tech-news-7) ⭐️ 7.0/10
8. [AI as a spatial software generator for programmable 3D objects](#item-tech-news-8) ⭐️ 7.0/10
9. [Anthropic’s Fable 5 Struggles in Enterprise as Clients Choose Cheaper Rivals](#item-tech-news-9) ⭐️ 7.0/10
10. [Alibaba Cloud Wan3.0 Launches with 30-Second Video Generation API](#item-tech-news-10) ⭐️ 7.0/10

**Financial News**
1. [Alibaba shares plunge after $10.2 billion placement to fund AI](#item-finance-news-1) ⭐️ 8.0/10
2. [Hugging Face reportedly explores sale at up to $13B valuation](#item-finance-news-2) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [seL4 Security Proofs Completed on AArch64](https://proofcraft.systems/news-2026/#2026-08-21) ⭐️ 9.0/10

Proofcraft Systems announced that the formal verification of seL4&\#x27;s security properties is now complete for AArch64 \(ARM 64-bit\), a major milestone in the microkernel&\#x27;s trustworthy computing story. The completed proofs currently cover the non-MCS \(mixed-criticality\) configuration and uniprocessor \(unicore\) systems, meaning mixed-criticality and multicore variants are not yet formally verified. This achievement extends seL4&\#x27;s machine-checked assurance to ARM 64-bit, strengthening its position for embedded, automotive, and military critical systems. Practical adoption still faces caveats, including the need for broader configuration coverage and integration challenges highlighted by community reviewers.

hackernews · snvzz · Aug 24, 11:32 · [Discussion](https://news.ycombinator.com/item?id=49418255)

**「Background」** seL4 is a microkernel designed for safety- and security-critical systems, distinguished by machine-checked formal proofs that verify its correctness rather than relying solely on testing. Proofcraft Systems has now announced the completion of formal security proofs for seL4 on ARM&\#x27;s 64-bit AArch64 architecture, adding a confidentiality guarantee that the kernel prevents unauthorized information flow between components. The proof stack extends down to the binary code, reducing the gap between the verified model and the code actually executed on the processor.

**「Impact」** Developers and organizations building critical systems on ARM 64-bit now have stronger machine-checked assurance for seL4&\#x27;s isolation, integrity, and confidentiality guarantees, though the limitation to non-MCS and unicore configurations means mixed-criticality and multicore deployments lack the same formal coverage.

**「Community Discussion」** Hacker News commenters offered cautious reactions, with some pointing out the fine print around non-MCS and unicore configurations and others suggesting that side-channel timing attacks could undermine the proof result. The thread also shared known seL4 users such as GenodeOS, LionsOS, and a Chinese car maker&\#x27;s hypervisor, while raising concerns that seL4 needs native Linux support to convincingly improve systems security.

<details><summary>References</summary>
<ul>
<li><a href="https://news.linxi.com.au/news/sel4-microkernel-achieves-full-formal-security-verification-on-aarch64">seL4 Microkernel Formal Security Proofs Completed on AArch64 ...</a></li>
<li><a href="https://www.newswarden.com/story/sel4-security-proofs-complete-aarch64">The seL4 Microkernel&#x27;s Security Proofs Are Now Complete on ...</a></li>
<li><a href="https://sel4.systems/Verification/proofs.html">seL4 Proofs | seL4 - sel4.systems</a></li>

</ul>
</details>

**Tags**: `#seL4`, `#formal verification`, `#microkernel`, `#AArch64`, `#security`

---

<a id="item-tech-news-2"></a>
### [MS Paint and Photos Embed Hidden GUID Watermarks in AI Edits](https://xusheng.dev/posts/reversing/mspaint_invisible_watermark/main/) ⭐️ 8.0/10

An analysis reports that Microsoft Paint and Photos silently embed invisible GUID watermarks into images edited with AI features, even when the processing runs locally using a local model. The watermark is added without user notice and cannot be disabled, though a separate visible watermark can be turned off. The findings raise privacy concerns because the unique identifier could potentially be linked to a Microsoft account. The exact scope, such as whether AI-assisted background removal triggers it, remains unclear.

hackernews · ComputerGuru · Aug 24, 15:28 · [Discussion](https://news.ycombinator.com/item?id=49421158)

**「Background」** Microsoft Paint and Windows Photos now add an invisible watermark to AI-generated or AI-edited images, even when processing happens locally. The watermark is a server-issued 16-byte GUID embedded by a component called Watermarker.dll, after Paint or Photos makes a mandatory remote moderation request to a Microsoft Azure Front Door endpoint; if the watermarking step fails, generation is canceled. The GUID is part of an 18-byte payload distributed invisibly across roughly 74% of image pixels, enabling images to be traced back to the Microsoft account that generated them.

**「Impact」** Users of MS Paint and Photos who share AI-edited images may unknowingly expose a unique identifier that could be traced to their Microsoft account, undermining anonymity.

**「Community Discussion」** Commenters largely agree the invisible identifier is a greater concern than the AI watermark itself, citing risks to internet anonymity and potential subpoenas to Microsoft. Others recall Microsoft&\#x27;s previous mishandling of Copilot watermarking in Azure DevOps and report false-positive triggers of the watermark.

<details><summary>References</summary>
<ul>
<li><a href="https://mangodeveloper.com/articles/microsoft-paint-embeds-invisible-guid-watermarks-in-local-ai-images-via-remote-moderation-server">Microsoft Paint Embeds Invisible GUID Watermarks in Local AI ...</a></li>
<li><a href="https://byteiota.com/ms-paint-invisible-server-guid-watermark-ai-image/">MS Paint Embeds Invisible Server GUIDs in Every AI Image</a></li>
<li><a href="https://xusheng.dev/posts/reversing/mspaint_invisible_watermark/main/">Microsoft Paint and Photos Embed Server-Issued GUIDs as ...</a></li>

</ul>
</details>

**Tags**: `#Microsoft`, `#AI watermarking`, `#privacy`, `#reverse engineering`, `#image forensics`

---

<a id="item-tech-news-3"></a>
### [Does NVIDIA&\#x27;s CUDA Moat Hold in Agentic Inference?](https://newsletter.semianalysis.com/p/agentx-inferencexv3-does-cuda-moat) ⭐️ 8.0/10

SemiAnalysis published &\#x27;AgentX - InferenceXv3,&\#x27; an evaluation of whether NVIDIA&\#x27;s CUDA ecosystem retains its advantage in agentic inference workloads. The analysis accompanies the open-sourcing of a $3 million dataset featuring over 1 million tokens of context, multiturn interactions, and sub-agent patterns, with reported 95%+ KV cache hit rates. It compares agentic inference performance across NVIDIA GB300 NVL72 and B200 systems as well as AMD&\#x27;s MI355. The item matters because it examines the durability of NVIDIA&\#x27;s CUDA moat in a workload segment increasingly important for AI infrastructure.

rss · Semianalysis · Aug 24, 00:19

**「Background」** Agentic inference refers to AI workloads where models handle long, multi-turn interactions with sub-agents, requiring high context lengths and efficient key-value cache reuse, unlike fixed-sequence inference. SemiAnalysis, an AI infrastructure research firm, has built an open-source benchmark called AgentX/InferenceXv3 to measure how chips and frameworks perform on this workload, comparing NVIDIA and AMD systems. The benchmark is relevant because NVIDIA&\#x27;s CUDA software ecosystem has long been seen as a moat, and testing whether it holds for agentic workloads helps assess competitive dynamics.

**「Impact」** AI infrastructure teams should expect NVIDIA&\#x27;s rack-scale systems to retain a significant performance lead in high-concurrency MoE and agentic inference—GB200 NVL72 showed up to 28× higher throughput than AMD&\#x27;s MI355X on DeepSeek-R1 workloads, and GB300 NVL72 delivers about 5% more tok/s/GPU than B200 on MiniMax M2.7—but B200&\#x27;s 29% lower cost per token makes it the cheaper choice for cost-sensitive serving. The open-sourced $3M dataset with 1M+ context, multiturn, and sub-agent traces gives developers a concrete way to reproduce these comparisons rather than relying on vendor claims.

<details><summary>References</summary>
<ul>
<li><a href="https://aiweekly.co/alerts/semianalysis-agentx-benchmark-says-cuda-moat-holds-in-agents">SemiAnalysis AgentX benchmark says CUDA moat holds in agents</a></li>
<li><a href="https://inferencex.semianalysis.com/">Open-Source Agentic Inference Benchmark | InferenceX</a></li>
<li><a href="https://inferencex.semianalysis.com/compare/minimax-m27-b200-vs-gb300">B 200 vs GB 300 NVL 72 : MiniMax M2.7 Inference ... | InferenceX</a></li>
<li><a href="https://www.kad8.com/ai/gb200-nvl72-vs-mi355x-why-systems-win-moe-inference/">GB200 NVL 72 vs MI 355 X: Why Systems Win MoE Inference · KAD</a></li>

</ul>
</details>

**Tags**: `#AI inference`, `#CUDA`, `#NVIDIA`, `#hardware`, `#agentic AI`

---

<a id="item-tech-news-4"></a>
### [Xiaomi Unveils Three Xuanjie Chips; O3 SoC to Debut in Xiaomi 18 Fold](https://mp.weixin.qq.com/s/ceIQbNnZrcNQqGywXCiXTQ) ⭐️ 8.0/10

Xiaomi announced three new Xuanjie chips: the O3 AI flagship SoC, the O100 high-bandwidth AI accelerator, and the D100 autonomous-driving AI chip, all of which have completed returned-chip verification and span AI computing needs across phones, vehicles, and smart home devices. The O3 uses a ten-core all-big-core CPU with a multi-core score surpassing 15,000, introduces the G2-Ultra NX GPU with 85% better performance and 64% lower power consumption, and is claimed to be the world&\#x27;s first mobile processor supporting LPDDR6, offering 113.8 GB/s memory bandwidth and 45% improved NPU AI performance. The D100 is described as China&\#x27;s first 3nm high-compute autonomous-driving AI chip, integrating a 20-core CPU, a 16-core NPU, up to 160 GB of unified memory, and enough capacity to locally deploy 200-billion-parameter large models; it is planned for commercial use next year. The O100 is described as the industry&\#x27;s first 6nm wafer-level vertically stacked advanced package using hybrid bonding with 1.4-micron bond pitch, delivering 1.22 TB/s bandwidth—16 times that of traditional flagship phones—and up to 330 TPS edge inference speed. According to the announcement, the O3 SoC will debut in the Xiaomi 18 Fold.

telegram · zaihuapd · Aug 24, 07:18

**「Background」** Xiaomi&\#x27;s Xuanjie \(玄戒\) is the company&\#x27;s self-developed chip family, positioned to cover AI computing across phones, cars, and IoT devices. Announced on August 24, 2026, the three new chips—O3, O100, and D100—have completed validation, with the O3 entering mass production and the other two expected to go commercial next year. The O3 will debut in the Xiaomi 18 Fold and Xiaomi Pad 9 Pro Max in September, while the D100 is noted as China&\#x27;s first 3nm high-compute AI chip for autonomous driving.

**「Impact」** With these chips, Xiaomi extends its in-house silicon to flagship mobile SoCs, edge AI accelerators, and automotive AI, with the O3 slated to appear in the Xiaomi 18 Fold and the D100 expected to bring 200-billion-parameter model deployment to vehicles when it enters commercial use next year.

<details><summary>References</summary>
<ul>
<li><a href="https://www.kucoin.com/news/flash/xuanji-o3-o100-d100-chips-launched-by-xiaomi">Xiaomi Launches Xuanji O3, O100, and D100 Chips - KuCoin</a></li>
<li><a href="https://www.itbear.com/hardware/xiaomi-unveils-three-proprietary-chips-to-build-a-full-ecosystem-ai-computing-foundation/">Xiaomi Unveils Three Proprietary Chips to Build a Full ...</a></li>
<li><a href="https://pandaily.com/xiaomi-unveils-xuanjie-o3-first-flagship-soc-break-5-million-aug2026">Xiaomi Unveils Xuanjie O3, First Flagship SoC to Break 5 ...</a></li>

</ul>
</details>

**Tags**: `#chips`, `#AI`, `#SoC`, `#Xiaomi`, `#hardware`

---

<a id="item-tech-news-5"></a>
### [AI Coding Reliance May Collapse Developer Expertise](https://larsfaye.com/articles/ai-coding-will-prevent-expertise) ⭐️ 7.0/10

In a new essay, Lars Faye argues that reliance on AI coding assistants will prevent software engineers from building deep expertise, predicting an eventual collapse in coding proficiency as developers generate code faster than they can understand and review it. The piece has sparked substantial debate among practitioners, with commenters noting that enterprise mandates now discourage manual coding and push engineers to &\#x27;vibe code&\#x27; through AI. Faye&\#x27;s analysis suggests that while short-term productivity rises, the long-term skill formation that comes from struggling with hard problems is lost when LLMs remove the friction. The article offers a critical counterpoint to current AI-driven development trends but provides no specific data or case studies to support its claims.

hackernews · larsfaye · Aug 24, 15:52 · [Discussion](https://news.ycombinator.com/item?id=49421554)

**「Background」** The article argues that the increasing reliance on AI coding assistants and agentic workflows may erode the hands-on practice that software engineers traditionally needed to build deep expertise. Historically, expertise developed through direct experience with writing, debugging, and designing code, but LLMs can now perform many of those steps, reducing the friction that long-term skill formation depends on. The discussion reflects broader concerns about how anthropic and other AI tools are reshaping developer learning and the future of the profession.

**「Impact」** Developers who rely heavily on AI assistants may find themselves unable to review or maintain the code they produce, as evidenced by enterprise directives that treat manual coding as &\#x27;doing it wrong&\#x27; and by engineers reporting that code is being shipped faster than humans can review it. This can erode code quality and individual expertise even when productivity appears high.

**「Community Discussion」** Commenters are split: some agree that AI reliance is already degrading review and expertise, while others argue that guided coding with AI built into an editor remains enjoyable and high-quality, and that many skilled engineers actively seek friction rather than avoiding it. A notable critique describes the situation as &\#x27;the snake eating its own tail&\#x27; for LLM software development, with the few developers who avoid brain-cooking AI ultimately being rewarded with reviewing terrible AI-generated code.

<details><summary>References</summary>
<ul>
<li><a href="https://larsfaye.com/articles/ai-coding-will-prevent-expertise">AI Coding will Prevent Expertise | Lars Faye</a></li>

</ul>
</details>

**Tags**: `#AI coding`, `#software engineering`, `#expertise`, `#LLM`, `#developer productivity`

---

<a id="item-tech-news-6"></a>
### [Executable as a SQLite Database](https://fzakaria.com/2026/08/23/your-executable-is-a-sqlite-database) ⭐️ 7.0/10

The article &quot;Executable Is a SQLite Database&quot; explores embedding SQLite databases inside executable binaries, allowing programs to be queried as structured data. The central idea treats formats like ELF as already database-like and proposes using SQLite&\#x27;s virtual-table mechanism to expose binary contents, making executables self-describing. The author notes the concept could enable &quot;fat&quot; executables that ship multiple versions of code, such as WebAssembly plus native pieces, or replace AppImages with dynamic SQLite-backed images. In a Hacker News comment, the author says the idea received poor feedback in academic circles despite enthusiasm from the community.

hackernews · setheron · Aug 24, 04:48 · [Discussion](https://news.ycombinator.com/item?id=49415271)

**「Background」** SQLite is a lightweight, serverless SQL database engine typically embedded in applications, and ELF is the standard executable format on many Unix-like systems. The article proposes making an executable file itself a valid SQLite database, so that tools can query its metadata and embedded resources using SQL. The idea builds on SQLite&\#x27;s virtual-table feature, which lets external data sources be exposed as queryable tables; the broader concept has also been discussed as a &\#x27;SQLite database as an executable format&\#x27; on Hacker News.

**「Community Discussion」** Many commenters are enthusiastic: one wants to use the approach for fat executables with WebAssembly and natively compiled variants, while another suggests it could replace AppImages. Another commenter calls SQLite virtual tables mind-blowing, and a counterpoint notes that ELF was already a database in a broad sense.

<details><summary>References</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=49415271">Executable Is a SQLite Database | Hacker News</a></li>

</ul>
</details>

**Tags**: `#SQLite`, `#ELF`, `#executables`, `#databases`, `#software-engineering`

---

<a id="item-tech-news-7"></a>
### [Bart: A 2.82B Vintage LLM Trained on Pre-1931 English Text](https://www.reddit.com/r/MachineLearning/comments/1vx94er/bart_a_vintage_llm_r/) ⭐️ 7.0/10

Unbounded Labs has released Bart, a 2.82B-parameter vintage LLM trained from scratch on 20.1B tokens of English written before 1931, spending about $807 and three months of compute. The model, accessible via a demo, Hugging Face \(jbduran/bartholomew-sft\), and a detailed blog post, explores whether LLMs can independently rediscover past scientific insights, as proposed by Demis Hassabis. The project includes Vintage CORE, the first suite of 20 benchmarks for vintage LLMs, a cleaned corpus derived from Harvard&\#x27;s Institutional Books \(reduced from 242B to 23B tokens\), and the largest vintage SFT dataset the team knows of, with 416k graded Q&amp;A pairs grounded in pre-1930s text. The final model was trained in five days on a single H100 at 60% MFU, and all datasets, methodology, training code, evals, and training runs are open-sourced. The team is seeking compute grants, funding, and mentorship for larger future runs.

reddit · r/MachineLearning · /u/soggydoggy8 · Aug 24, 17:20

**「Background」** Vintage LLMs are language models trained exclusively on historical text, aiming to test whether modern architectures can reach conclusions comparable to those of past scientists and writers without exposure to contemporary knowledge. Training on pre-1931 materials also provides a way to study dataset curation, domain-specific benchmarks, and whether models can generate original ideas rather than regurgitating next tokens from modern corpora.

**「Impact」** For ML researchers studying historical corpora, domain-specific LLMs, and efficient pre-training, Bart provides a fully open-sourced reference point with custom benchmarks and reproducible training runs; however, it is a niche research artifact rather than an industry-scale breakthrough, and its practical applicability beyond the vintage domain remains unproven.

**Tags**: `#LLM`, `#NLP`, `#historical text`, `#research`, `#open source`

---

<a id="item-tech-news-8"></a>
### [AI as a spatial software generator for programmable 3D objects](https://www.reddit.com/r/MachineLearning/comments/1vxcc1h/r_using_ai_as_a_spatial_software_generator_to/) ⭐️ 7.0/10

Researchers, including a co-author posting on Reddit, propose using LLMs as spatial software generators to create 3D objects that are inherently programmable rather than static mesh blobs. The generated objects are composed of logical parts and are animation-ready from inception, with hierarchical structure and hinge/socket articulation set at authoring time. They can also contain logic to render differently depending on compute power, such as mobile versus sophisticated game engines. Visual demonstrations are available at https://nova3d.xyz/ and the work includes a GitHub repository. The approach currently lags behind traditional AI 3D generators on complex organic shapes, but the authors argue that code-based generation will eventually dominate fields like industrial design, game development, simulations, and AR/VR/XR.

reddit · r/MachineLearning · /u/mhb\_11 · Aug 24, 19:10

**「Background」** Most AI 3D generators output monolithic mesh blobs, which are difficult to animate or edit because they lack structure and semantic parts. This research treats 3D as software, using LLMs to write spatial programs that define objects with parts, hierarchy, and articulation, making them more useful for real applications from the moment they are created.

**「Impact」** For developers and designers using AI 3D generation, this approach could significantly reduce post-processing work by producing animation-ready, hierarchy-aware objects, though its current weakness with complex organic shapes means it is not yet a complete replacement for existing generators.

**Tags**: `#3D generation`, `#machine learning`, `#LLM`, `#programmable graphics`, `#procedural modeling`

---

<a id="item-tech-news-9"></a>
### [Anthropic’s Fable 5 Struggles in Enterprise as Clients Choose Cheaper Rivals](https://www.ft.com/content/5ee49718-c258-4f01-aa32-7e5b76ae5245) ⭐️ 7.0/10

Anthropic&\#x27;s flagship model Fable 5 has seen weak enterprise adoption in its first month, according to Ramp data, accounting for about 6% of Anthropic API token usage and roughly 11% of spending. Its pricing, around $10 per million input tokens and $50 per million output, is roughly double Anthropic&\#x27;s other flagship models and higher than OpenAI&\#x27;s GPT-5.6 Sol. Cheaper open-source models and Microsoft&\#x27;s own in-house model are drawing customers away, while Anthropic&\#x27;s requirement to retain user data for 30 days is also dampening demand. Ramp economists say the data suggests corporate willingness to pay for frontier artificial intelligence has hit a ceiling. The trend highlights pricing and data-retention terms as key barriers for high-end AI adoption.

telegram · zaihuapd · Aug 24, 01:22

**「Background」** Anthropic sells its AI models through APIs with usage-based pricing, and enterprise demand is often measured by token volume and API spending. Ramp is a corporate spend platform whose economists track these patterns to gauge willingness to pay for frontier AI.

**「Impact」** Cost-conscious enterprise customers are likely to keep favoring cheaper open-source and Microsoft models over Anthropic&\#x27;s Fable 5, which puts near-term pressure on Anthropic&\#x27;s flagship API revenue unless it adjusts pricing or its 30-day data-retention policy.

**Tags**: `#AI`, `#enterprise`, `#pricing`, `#open-source`, `#Anthropic`

---

<a id="item-tech-news-10"></a>
### [Alibaba Cloud Wan3.0 Launches with 30-Second Video Generation API](https://mp.weixin.qq.com/s/peeeU6cBz4AaROvFe1zqQQ) ⭐️ 7.0/10

Alibaba Cloud officially launched its Wan3.0 video generation model, supporting clips up to 30 seconds and emphasizing realistic human texture, reference consistency, and non-realistic stylization. Users can try it on Alibaba Cloud Bailian, the Wanxiang official website, and the Qwen app. The API is priced per second by resolution: 480P at 0.3 yuan, 720P at 0.6 yuan, and 1080P at 1.2 yuan. From August 24 to September 23, Alibaba Cloud Bailian and the Qwen AI platform offer a limited-time API discount of 30% off, meaning 70% of the list price.

telegram · zaihuapd · Aug 24, 10:14

**「Background」** Wan \(万相\) is Alibaba Cloud&\#x27;s line of generative AI models and a creative platform offering text-to-image, image-to-image, text-to-video, image-to-video, and image editing features. Wan 3.0 was released for public beta on August 6, 2026, according to the company, and can generate up to 30 seconds of video in a single run, supports seamless extension, and accepts document formats such as doc, xls, ppt, pdf, and md as inputs. This release continues Alibaba Cloud&\#x27;s push into AI-driven video generation, positioning Wan 3.0 as a powerful tool for creators.

**「Impact」** Alibaba Cloud has positioned Wan3.0 for AI video developers with per-second API pricing of 0.3/0.6/1.2 yuan for 480P/720P/1080P \(about $0.05/$0.10/$0.20\) and a limited-time 30% discount until September 23, but access is currently gated as a preview or invitation-only offering through Model Studio, so immediate adoption will depend on invitation eligibility and real-world performance validation.

<details><summary>References</summary>
<ul>
<li><a href="https://aihot.virxact.com/story/a99af99d-0dff-4752-a453-37de2d1a0c65">Alibaba Cloud releases Wan 3 . 0 · AI HOT</a></li>
<li><a href="https://wan.video/">Wan AI: Leading AI Video Generation Model</a></li>
<li><a href="https://juejin.cn/post/7670593377075724339">juejin.cn/post/7670593377075724339</a></li>
<li><a href="https://www.ngram.com/blog/wan-3-0-document-to-video-ai-model">Wan 3.0: Alibaba&#x27;s Document-to-Video AI Model Explained | ngram.com</a></li>
<li><a href="https://dataconomy.com/2026/08/24/alibaba-launches-wan30-a-30-second-ai-video-generation-model/">Alibaba Launches Wan3.0, A 30-second AI Video Generation Model - Dataconomy</a></li>
<li><a href="https://www.alibabacloud.com/blog/wan3-0-30-second-ai-video-generation-from-any-input_603452">Wan3.0: 30-Second AI Video Generation from Any Input - Alibaba Cloud Community</a></li>

</ul>
</details>

**Tags**: `#video generation`, `#Alibaba Cloud`, `#generative AI`, `#API pricing`, `#AI models`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Alibaba shares plunge after $10.2 billion placement to fund AI](https://www.cnbc.com/2026/08/24/alibaba-share-placement-drop-ai-hong-kong.html) ⭐️ 8.0/10

Alibaba&\#x27;s Hong Kong shares plunged as much as 10% after the Chinese tech giant priced an HK$80 billion \($10.2 billion\) placement of 710 million new shares to non-U.S. investors at HK$112.70 each, saying all net proceeds will go toward AI infrastructure. Shares were last trading 8.4% lower at HK$112.70, versus Friday&\#x27;s close of HK$123.

rss · CNBC Finance · Aug 24, 08:21

**「Background」** The placement comes days after Alibaba reported a 75% drop in June-quarter profit, with infrastructure spending up 75% to 67.7 billion yuan. It follows the company&\#x27;s earlier plan to invest at least 380 billion yuan in cloud and AI infrastructure over three years.

**Tags**: `#Alibaba`, `#share placement`, `#AI investment`, `#Hong Kong stocks`, `#Chinese tech`

---

<a id="item-finance-news-2"></a>
### [Hugging Face reportedly explores sale at up to $13B valuation](https://www.bloomberg.com/news/articles/2026-08-23/hugging-face-gauging-interest-for-potential-sale-business-insider-says) ⭐️ 7.0/10

Hugging Face, the AI platform, is reportedly exploring a possible sale at a valuation of $13 billion or more, according to Business Insider, citing people familiar with the matter. No deal has been reached.

telegram · zaihuapd · Aug 24, 05:45

**「Background」** The company was valued at $4.5 billion after a $235 million funding round in 2023. It has been working with a bank to gauge buyer interest, the report said.

**Tags**: `#M&amp;A`, `#AI`, `#valuation`, `#startup`, `#tech`

---