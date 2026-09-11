---
layout: default
title: "Horizon Summary: 2026-09-11 (EN)"
date: 2026-09-11
lang: en
---

> From 41 items, 10 important content pieces were selected

---

**Technology News**
1. [Shopify moves from React Native back to Swift and Kotlin](#item-tech-news-1) ⭐️ 8.0/10
2. [Microsoft Designates Rust as a Tier-1 Language](#item-tech-news-2) ⭐️ 8.0/10
3. [trynix.dev boots any Nix package in the browser](#item-tech-news-3) ⭐️ 8.0/10
4. [Debate over trusting OpenAI with unpublished math](#item-tech-news-4) ⭐️ 7.0/10
5. [Fly connectome Pong attempt fails, yielding synapse-level audit](#item-tech-news-5) ⭐️ 7.0/10
6. [Ant International, Visa, Mastercard to develop common AI-agent payment standard](#item-tech-news-6) ⭐️ 7.0/10
7. [DeepSeek V4.1 Flash Reportedly Launches as 552B Multimodal API Model](#item-tech-news-7) ⭐️ 7.0/10
8. [Tencent Hunyuan open-sources AuK audio editing model](#item-tech-news-8) ⭐️ 7.0/10

**Financial News**
1. [Kalshi launches CFTC-approved gold and silver perpetual futures](#item-finance-news-1) ⭐️ 7.0/10
2. [Chinese AI chipmakers raise prices as HBM shortage bites](#item-finance-news-2) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Shopify moves from React Native back to Swift and Kotlin](https://shopify.engineering/back-to-native) ⭐️ 8.0/10

Shopify Engineering is moving from React Native back to native Swift and Kotlin, according to the company&\#x27;s engineering post. The item is framed as a notable industry case study for mobile and software engineering readers weighing shared cross-platform codebases against platform-native development. Because no article text was supplied, specifics such as the migration scope, timeline, compatibility constraints, and performance rationale are not available in the provided material. The accompanying Hacker News discussion focused on React Native versus native tradeoffs, the value of shared codebases, and whether AI-assisted migration changes the economics of such rewrites.

hackernews · fnthawar2 · Sep 10, 14:09 · [Discussion](https://news.ycombinator.com/item?id=49643982)

**「Background」** React Native is a cross-platform mobile framework that allows developers to build iOS and Android apps from a shared JavaScript and React codebase. Shopify adopted React Native in 2020 to unify its mobile development, but has now decided to migrate back to native Swift for iOS and Kotlin for Android. According to the author, the rise of large language models changed a core assumption behind the 2020 decision, prompting a reevaluation of the shared-codebase approach.

**「Impact」** For Shopify&\#x27;s mobile engineers, the move ends a single shared React Native codebase in favor of separate Swift and Kotlin codebases, a shift the company attributes to AI coding agents changing the cost assumptions behind its original 2020 decision to adopt React Native.

**「Community Discussion」** Commenters broadly welcomed moving off React Native, with one iOS engineer saying the decision validated a career-long argument against shared codebases, while others shared migration experiences ranging from an overnight, Codex-assisted rewrite of a 15–20-screen app to a larger Swift/Kotlin migration completed mostly without LLM code assistance before January 2026. A key disagreement was whether AI made the migration viable: some treated LLMs as the enabling factor, but one commenter argued the migration was already feasible without them, and the post author said Shopify reevaluated its 2020 React Native decision because LLMs changed a core assumption.

<details><summary>References</summary>
<ul>
<li><a href="https://shopify.engineering/back-to-native">Native is now the future of mobile at Shopify (2026) - Shopify</a></li>
<li><a href="https://news.ycombinator.com/item?id=49643982">Shopify moves back to Native from React Native | Hacker News</a></li>
<li><a href="https://shopify.engineering/back-to-native">Native is now the future of mobile at Shopify (2026) - Shopify</a></li>

</ul>
</details>

**Tags**: `#React Native`, `#Mobile Engineering`, `#Swift`, `#Kotlin`, `#AI-assisted Migration`

---

<a id="item-tech-news-2"></a>
### [Microsoft Designates Rust as a Tier-1 Language](https://rustfoundation.org/media/guest-post-rust-is-tier-1-language-at-microsoft/) ⭐️ 8.0/10

A Rust Foundation guest post states that Microsoft has designated Rust as a tier-1 language, making it a first-class supported option for systems and application development at the company. The designation is a significant industry endorsement for Rust, which has been gaining adoption as a memory-safe alternative to C and C++ in infrastructure and large codebases. Specifics about exact support commitments, product areas, and timelines were not provided in the available material. Community discussion framed the move as confirmation of Rust&\#x27;s maturity and as part of a broader diversification of systems-programming languages among major OS vendors.

hackernews · mmastrac · Sep 10, 13:39 · [Discussion](https://news.ycombinator.com/item?id=49643546)

**「Background」** Microsoft&\#x27;s &quot;tier-1 language&quot; label is an internal engineering designation meaning a language receives a paved path from local development to production, including secure toolchain builds, productive developer tooling, quality workflows, deep platform integration, and compliance support. Rust is a memory-safe systems programming language that has been gaining adoption at large infrastructure organizations, and the classification is being described as a notable shift in Microsoft&\#x27;s language strategy, though official details remain limited.

**「Impact」** Developers targeting Windows are the most concretely affected: Microsoft&\#x27;s own Rust setup guidance already requires the Microsoft C++ build tools as a prerequisite and relies on VS Code&\#x27;s rust-analyzer extension for completion, diagnostics, go-to-definition and debugging, so treating Rust as tier-1 points toward continued first-party tooling investment rather than a break from the existing MSVC-linked toolchain. The community discussion treats MSVC integration as publicly signaled but still unconfirmed in the details.

**「Community Discussion」** Commenters broadly welcomed the announcement as evidence that Rust is now a mature, serious competitor to C++ and C\#, with one long-time professional Rust developer saying they would use it exclusively for backends and frontends if WebAssembly and native UI support were better. Others highlighted Microsoft&\#x27;s reported goal to convert 1 billion lines of code to Rust by 2030 with automated tooling, DARPA work on automating C-to-Rust conversion, and the strategic value of Rust&\#x27;s memory safety for reducing CVEs in Microsoft&\#x27;s portfolio; one noted that all major OS vendors with C and C++ tooling now have diversified systems-language options.

<details><summary>References</summary>
<ul>
<li><a href="https://rustfoundation.org/media/guest-post-rust-is-tier-1-language-at-microsoft/">Guest Post: Rust Is Tier-1 Language at Microsoft</a></li>
<li><a href="https://qatrial.com/developer-open-source/rust-is-tier-1-language-at-microsoft/">Rust Is Tier-1 Language At Microsoft - QAtrial</a></li>
<li><a href="https://bestcadpapers.com/art-and-society/rust-is-tier-1-language-at-microsoft/">Rust Is Tier-1 Language At Microsoft - Best CAD papers</a></li>
<li><a href="https://learn.microsoft.com/ru-ru/windows/dev-environment/rust/setup">Настройка среды разработки в Windows для Rust | Microsoft Learn</a></li>

</ul>
</details>

**Tags**: `#Rust`, `#Microsoft`, `#programming languages`, `#systems programming`, `#open source`

---

<a id="item-tech-news-3"></a>
### [trynix.dev boots any Nix package in the browser](https://simonwillison.net/2026/Sep/10/trynix/) ⭐️ 8.0/10

Farid Zakaria has launched trynix.dev, which he describes as his &quot;magnum opus&quot; of Nix work, providing a qemu-wasm-powered x86\_64 Linux virtual machine that runs entirely in the browser through WebAssembly. The VM can be booted with any Nix package from the past 13 years, and packages are URL-addressable: navigating to https://trynix.dev/?pkg=python3%403.6.2 and clicking &quot;Load&quot; yields an interactive shell against a virtual machine running Python 3.6.2 from 2017. Zakaria is building further tooling on top of this, including the trynix-preview GitHub Action, which comments a link on a pull request so the PR&\#x27;s build can be booted in the browser, with no servers involved. Simon Willison highlighted the project, framing it as a notable and practically useful demonstration of browser-based virtualization and reproducible Nix environments.

rss · Simon Willison · Sep 10, 23:44

**「Background」** Nix is a package manager built around reproducible builds, and nixpkgs is its package collection; trynix indexes the full history of nixpkgs, covering 13 years and more than 310,083 package versions. Running an old package traditionally meant fetching and building a matching environment locally, but trynix relies on qemu-wasm — QEMU compiled to WebAssembly with a wasm TCG JIT and a virtio-9p port that exposes the Nix store to the guest — to boot an x86\_64 Linux VM entirely inside a browser tab with no server involved. The result is a serial-console shell rather than a graphical environment, addressable by URL so a specific package version can be shared as a link.

**「Impact」** For Nix users and maintainers, the trynix-preview action means a pull request&\#x27;s build can be inspected interactively from a browser link rather than by provisioning server infrastructure, though the source does not describe performance, package-size limits, or other constraints of the in-browser VM.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/fzakaria/trynix">fzakaria/ trynix : Boot anything nixpkgs ever shipped, in your browser .</a></li>
<li><a href="https://fzakaria.com/2026/09/04/any-nix-package-live-in-your-browser">Any Nix package, live in your browser | Farid Zakaria ’s Blog</a></li>
<li><a href="https://trynix.dev/">trynix</a></li>

</ul>
</details>

**Tags**: `#Nix`, `#WebAssembly`, `#qemu-wasm`, `#browser-based virtualization`, `#reproducible builds`

---

<a id="item-tech-news-4"></a>
### [Debate over trusting OpenAI with unpublished math](https://mathstodon.xyz/@andreasthom/117240535270608201) ⭐️ 7.0/10

A Mathstodon thread by @andreasthom, linking to additional posts plus an X thread by ValerioCapraro and a Bluesky post, raises questions about whether researchers can trust OpenAI with unpublished mathematics. The item itself is link-only, and the central claims remain unverified. It drew a large Hacker News discussion of 631 points and 613 comments debating attribution, training-data provenance, and whether model progress on open problems is genuine. One commenter cited reports that OpenAI&\#x27;s internal models solve open problems at a surprisingly fast rate, while others noted that researchers using such models on open problems may be feeding fresh training data back to the company. Several commenters argued both effects can hold at once: chats may sharpen a model&\#x27;s latent intuition while reinforcement learning on verifiable math with massive compute yields results that owe little to any specific chat.

hackernews · pred\_ · Sep 10, 06:49 · [Discussion](https://news.ycombinator.com/item?id=49639408)

**「Background」** The dispute follows earlier allegations by mathematicians Levent Alpöge and Tristan Buckmaster that OpenAI used their unpublished work, and it now includes Andreas Thom, who says he spent months discussing the expander matching problem with ChatGPT before OpenAI announced a model result constructing the first non-sofic group. Thom reportedly emailed OpenAI researchers Mark Sellke and Sébastien Bubeck about the overlap. At issue is training-data provenance and attribution: whether private chats or unpublished mathematical ideas that researchers share with AI systems can later appear in models or in company-announced results without credit.

**「Impact」** Researchers weighing whether to run unpublished mathematics through OpenAI&\#x27;s models now face a concrete disincentive: the chats and problem ideas they supply could be absorbed into internal models or precede a rival credited result, pushing sensitive work away from commercial AI systems. The underlying accusations remain unverified, and no evidence has been presented that OpenAI trained on or used any specific collaborator&\#x27;s unpublished mathematics.

**「Community discussion」** Commenters largely agreed that researchers feeding unpublished work into OpenAI models may be supplying valuable training data, but disagreed on whether that explains the models&\#x27; reported success on open problems. One analogy compared OpenAI to a human collaborator who publishes on a shared idea without attribution—behavior called highly unethical for a human researcher—while another argued that RL on verifiable math could produce superhuman results largely independent of any specific chat, and a third framed the issue more broadly as misplaced trust in companies to safeguard user data.

<details><summary>References</summary>
<ul>
<li><a href="https://lemmy.world/post/51743560">OpenAI might have stolen another major math proof - Lemmy.World</a></li>
<li><a href="https://officechai.com/ai/mathematician-andreas-thom-questions-if-openai-used-his-chatgpt-chat-data-for-its-non-sofic-groups-proof/">Mathematician Andreas Thom Questions If OpenAI Used His...</a></li>
<li><a href="https://ai-tldr.dev/releases/andreas-thom-openai-math-data/">Andreas Thom — a second mathematician questions OpenAI on his...</a></li>
<li><a href="https://theconversation.com/openai-claims-another-huge-mathematical-result-amid-fights-over-credit-ethics-and-privacy-291575">OpenAI claims another huge mathematical result amid fights over...</a></li>
<li><a href="https://news.ycombinator.com/item?id=49639408">More questions about whether researchers can trust OpenAI with...</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#AI research ethics`, `#training data provenance`, `#mathematics`, `#LLM attribution`

---

<a id="item-tech-news-5"></a>
### [Fly connectome Pong attempt fails, yielding synapse-level audit](https://www.reddit.com/r/MachineLearning/comments/1wc67ci/i_tried_to_make_a_real_fly_connectome_learn_to/) ⭐️ 7.0/10

A Reddit post by /u/oPeraza2007 describes an attempt to train a small real subgraph of the new MaleCNS v1.0 fly connectome — 166k neurons from a real EM reconstruction — to play Pong using dopamine-style plasticity, and it did not learn. The author says diagnosing the failure was more informative than a successful demo: fixing a neuPrint regex bug that silently zeroed out two neuron populations, discovering the original neuron selection had no photoreceptor-to-anything path because real photoreceptors do not synapse directly onto motion detectors and an intermediate layer was missing, and finding learning-on vs learning-off produced bit-for-bit identical results across multiple seeds even though weights verifiably changed. That was traced to half of the 4 available motor neurons having zero synapses from any sensory pathway in the model; they had been assigned to the “paddle down” group by array index and could never fire. A rebuilt circuit based on a courtship-pursuit visual-target-tracking hypothesis was refuted by the data, but led to a different descending neuron that connected end to end, after which learning-on vs learning-off finally diverged—though the effect looked like the learning rule quieting the system rather than skill improvement, since misses outnumber hits and punishment dominates. The post also argues that viral fly-brain game projects had not solved these issues: the Doom project’s repo says it failed its own validation gates after six iterations, the Minecraft mod’s limitations section admits the real motion-detection pathway stays silent and escape/foraging behaviors are hand-injected or reflex-layer fallbacks, and the Beat Saber creator’s replies admit overfitting to one track with replay data mixed into the input; a full writeup is linked.

reddit · r/MachineLearning · /u/oPeraza2007 · Sep 10, 02:28

**「Background」** A Drosophila connectome is a list of the neurons in the fruit fly nervous system and the chemical synapses between them, spanning both the brain and the ventral nerve cord, which differ considerably between males and females. MaleCNS v1.0 is Janelia&\#x27;s electron-microscopy reconstruction of the complete central nervous system of a single male fruit fly, covering roughly 166,000 neurons and the millions of connections between them, and such datasets are typically queried through tools like neuPrint. neuPrint&\#x27;s search semantics distinguish whole-field regular-expression matching from partial substring matching, a distinction that matters because NeuronCriteria and related APIs behave differently depending on whether a query is treated as a fixed string or a regex.

**「Impact」** For researchers and developers evaluating MaleCNS v1.0 connectome demos, the audit indicates that the viral Doom, Minecraft, and Beat Saber clips should not be treated as evidence of emergent sensorimotor learning, since the projects&\#x27; own documentation reportedly concedes failed validation gates, a silent real motion-detection pathway with hand-injected behaviors, and overfitting to a single track. The author&\#x27;s inability to produce learning even after fixing the connectivity and regex bugs suggests that simulating the central complex and steering circuits, rather than routing around them, is the more defensible next step for anyone building on this connectome.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Drosophila_connectome">Drosophila connectome - Wikipedia</a></li>
<li><a href="https://male-cns.janelia.org/">Male CNS Connectome - MaleCNS connectome</a></li>
<li><a href="https://www.janelia.org/project-team/flyem/male-cns-connectome">Male CNS Connectome | Janelia Research Campus</a></li>
<li><a href="https://connectome-neuprint.github.io/neuprint-python/docs/neuroncriteria.html">NeuronCriteria — neuprint-python 0.6.2 documentation</a></li>
<li><a href="http://natverse.org/neuprintr/reference/neuprint_search.html">Search for body IDs based on a given name — neuprint_search • neuprintr</a></li>
<li><a href="https://hothardware.com/news/google-mapped-a-fruit-fly-brain-so-engineers-taught-it-to-play-doom">Google Mapped A Fruit Fly Brain, So Engineers Taught It To Play Doom</a></li>
<li><a href="https://www.pcgamer.com/hardware/after-google-mapped-an-adult-male-fruit-flys-brain-software-engineers-made-it-play-doom-mario64-and-beat-saber/">After Google mapped an adult male fruit fly&#x27;s brain, software engineers made it play Doom, Mario64, and Beat Saber | PC Gamer</a></li>

</ul>
</details>

**Tags**: `#connectome`, `#computational neuroscience`, `#plasticity`, `#machine learning`, `#negative results`

---

<a id="item-tech-news-6"></a>
### [Ant International, Visa, Mastercard to develop common AI-agent payment standard](https://www.cnbc.com/2026/09/10/ant-international-visa-mastercard-ai-agent-payment-standard.html) ⭐️ 7.0/10

Ant International announced a collaboration with Visa and Mastercard to develop a common standard for AI-agent payments, under which the three parties would establish a &quot;Know Your Agent&quot; mechanism that links agents to valid entities, assesses their behavior and monitors risk. The stated goal is to improve interoperability and security across different payment systems. The companies cited a McKinsey forecast that AI agents could handle between $3 trillion and $5 trillion of global consumer commerce transactions by 2030. The announcement is an early-stage partnership: no technical specification, implementation timeline, governance model, or pilot details were disclosed, and the account is a secondary summary citing CNBC, which limits independent verification.

telegram · zaihuapd · Sep 10, 03:00

**「Background」** AI-agent payments, sometimes called agentic commerce, refer to transactions initiated and completed by autonomous software agents on a user&\#x27;s behalf, which require ways to verify the agent&\#x27;s identity and authority. The proposed &quot;Know Your Agent&quot; \(KYA\) framework is intended to link an agent to a legitimate entity, assess its behavior, and monitor risk across different payment systems, similar in spirit to Know Your Customer checks. Ant International, Visa, and Mastercard announced the collaboration on September 10, 2026, but independent coverage described it as a high-level interoperability commitment among competing payment protocols without technical specifications, governance, or a timeline.

**「Impact」** For merchants, issuers, and developers building AI shopping agents, the Ant International, Visa, and Mastercard collaboration points toward a shared agent-identification and verification framework that could reduce friction in cross-network AI-initiated payments. Because this is an early-stage partnership announcement without a published specification, timeline, or implementation details, no concrete integration or compliance requirements have been established yet.

<details><summary>References</summary>
<ul>
<li><a href="https://www.unite.ai/ant-international-visa-mastercard-align-on-ai-agent-verification-rules/">Ant International, Visa, Mastercard Align on AI Agent ...</a></li>
<li><a href="https://forkast.news/ant-international-visa-and-mastercard-agree-on-agent-identity-standard-now-comes-the-hard-part/">Ant International, Visa, and Mastercard Agree on Agent ...</a></li>
<li><a href="https://www.cnbc.com/2026/09/10/ant-international-visa-mastercard-ai-agent-payment-standard.html">Ant International, Visa and Mastercard team up on AI payment ...</a></li>
<li><a href="https://mitsloanindia.com/article/visa-mastercard-ant-push-common-standards-for-ai-agents-making-payments/">Visa , Mastercard , Ant Push Common Standards for AI Agents ...</a></li>
<li><a href="https://www.hokanews.com/2026/09/visa-and-mastercard-back-ant.html">Visa and Mastercard Back Ant International’s ‘Know Your Agent ...</a></li>

</ul>
</details>

**Tags**: `#AI agents`, `#payments`, `#standards`, `#fintech`, `#interoperability`

---

<a id="item-tech-news-7"></a>
### [DeepSeek V4.1 Flash Reportedly Launches as 552B Multimodal API Model](https://mp.weixin.qq.com/s/qg0NU3NNUbp1co2PdkAPAg) ⭐️ 7.0/10

DeepSeek has reportedly released V4.1 Flash, described as the smallest model in a new architecture series, built on a 552B-parameter Causal-Encoder-Decoder structure with 8B input and 16B output activations and native support for multimodal visual understanding. The model is said to be live on the DeepSeek API under the name deepseek-flash. According to the report, new pricing takes effect on 2026年9月10日 12:00, and after 2026年9月14日 12:00 requests to deepseek-v4-pro will be routed to V4.1 Flash and billed at its rates. The information comes from a Telegram aggregator post and includes no benchmarks, technical evaluation, or official confirmation, so the release, specifications, dates, and pricing changes remain unverified.

telegram · zaihuapd · Sep 10, 05:54

**「Background」** DeepSeek has been rolling out a new architecture family in which V4.1-Flash is described as the smallest member, positioned for greater capability, faster inference, higher throughput, and cheaper scaling to larger models. The Causal Encoder–Decoder design splits a 40-layer Transformer into a 20-layer causal encoder and a 20-layer decoder, so input-heavy agentic workloads such as processing large documents, codebases, or long conversation histories stay cheap while output generation uses a larger active parameter set. DeepSeek published a model card for the release on Hugging Face under an MIT license, consistent with its recent practice, though the aggregator post itself provides no benchmarks or independent evaluation.

**「Impact」** Developers and organizations sending production traffic to deepseek-v4-pro must prepare for their requests to be automatically routed to deepseek-flash from September 14, 2026 12:00 and billed at the Flash model&\#x27;s rates, which means prior acceptance tests and quality assumptions tied to V4 Pro no longer describe what the endpoint returns. Because the release has no accompanying benchmarks or official confirmation in the supplied material, teams should validate outputs against their own workloads before the routing switch rather than assume equivalent behavior.

<details><summary>References</summary>
<ul>
<li><a href="https://www.deepseek.com/en/news/deepseek-v4-1-flash/">DeepSeek | Introducing DeepSeek-V4.1-Flash: smarter, faster ...</a></li>
<li><a href="https://www.gate.com/news/detail/deepseek-releases-v41-flash-ai-model-with-552b-parameters-24165404">DeepSeek Releases V4.1-Flash AI Model With 552B Parameters</a></li>
<li><a href="https://aiweekly.co/alerts/deepseek-posts-v41-flash-552b-moe-8b-active-1m-context">DeepSeek posts V4.1-Flash: 552B MoE, 8B active, 1M context</a></li>
<li><a href="https://benchlm.ai/deepseek/api-pricing">DeepSeek API Pricing (September 2026): $0.30–$1.20 per 1M ...</a></li>

</ul>
</details>

**Tags**: `#DeepSeek`, `#LLM release`, `#multimodal AI`, `#API pricing`, `#AI news`

---

<a id="item-tech-news-8"></a>
### [Tencent Hunyuan open-sources AuK audio editing model](https://x.com/TencentHunyuan/status/2097996926876795197) ⭐️ 7.0/10

Tencent Hunyuan announced the official release of AuK, an open-source audio editing model that unifies speech generation and editing through natural-language instructions and reference audio. According to the announcement, AuK supports zero-shot text-to-speech, timbre/style/emotion editing, accent removal, and multi-speaker voice separation. Tencent Hunyuan also released AuK-Flash, a variant that uses 4-step inference and is claimed to be about 4.5x faster under matching conditions. Code, model weights, and demos are said to be available. The available recap does not include benchmarks, a paper, model size, licensing details, or independent verification, and the speedup claim is conditional and unverified.

telegram · zaihuapd · Sep 10, 11:56

**「Background」** Speech and audio models have traditionally been task-specific, with separate systems for text-to-speech, voice conversion, denoising, and source separation. Recent work has moved toward unified foundation models that handle both generation and editing through a single interface, typically taking a reference audio clip plus a natural-language instruction; AuK is presented in external coverage as such a model, described as a 1.5B-parameter system released under the MIT license. Few-step variants such as AuK-Flash follow a broader trend of cutting the number of iterative sampling steps in diffusion- and flow-based audio generators to reduce inference latency, which is the context for its 4-step operation and speed claim.

**「Impact」** Speech and audio developers gain a self-hostable, open-weight option that unifies zero-shot text-to-speech with instruction- and reference-audio-based editing, reducing the need to stitch together separate generation and editing pipelines, while AuK-Flash&\#x27;s 4-step inference lowers the latency floor for deployment. That 4.5x figure is reported under matched conditions and is characterized as a sampler speedup rather than an end-to-end one, so real-world gains may differ.

<details><summary>References</summary>
<ul>
<li><a href="https://mmlong818.github.io/ai-pulse/articles/tencent-auk-audio-model.html">Tencent Hunyuan Open - Sources AuK for Speech and Audio Editing ...</a></li>
<li><a href="https://www.orcarouter.ai/blog/auk-flash-open-source-release">AuK -Flash &amp; AuK : Tencent &#x27;s Quiet Open - Source Speech Model</a></li>
<li><a href="https://alphasignal.ai/news/tencent-s-auk-replaces-16-speech-tools-with-one-open-source-model">Tencent &#x27;s AuK Replaces 16 Speech Tools With One Open - Source ...</a></li>
<li><a href="https://www.orcarouter.ai/blog/auk-vs-auk-flash">AuK vs AuK - Flash : 4 Sampling Steps vs 32, and Who Wins</a></li>
<li><a href="https://arxiv.org/pdf/2609.08936">AuK Technical Report: An Open-Source Foundational Model for...</a></li>

</ul>
</details>

**Tags**: `#open-source-models`, `#audio-editing`, `#text-to-speech`, `#generative-ai`, `#Tencent-Hunyuan`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Kalshi launches CFTC-approved gold and silver perpetual futures](https://www.cnbc.com/2026/09/10/kalshi-launches-perps-for-gold-and-silver-following-cftc-approval-expanding-futures-offerings.html) ⭐️ 7.0/10

Kalshi launched perpetual futures tied to gold and silver on Thursday after the Commodity Futures Trading Commission approved the listing this week, the first non-crypto perpetuals it has been cleared to offer in the U.S. Kalshi&\#x27;s crypto perpetuals, approved in late May, have since recorded $44 billion in notional volume, according to the platform&\#x27;s website.

rss · CNBC Finance · Sep 10, 14:00

**「Background」** Perpetual futures \(&quot;perps&quot;\) are contracts that track an asset&\#x27;s price without an expiry date and without requiring the buyer to own the asset. Kalshi first listed crypto-linked perps in late May, and this week&\#x27;s CFTC approval makes gold and silver the first non-crypto perpetual futures cleared in the U.S.

**「Who is affected」** Established futures exchanges such as CME Group, Cboe, ICE and Nasdaq face the prospect of losing trading volume to Kalshi&\#x27;s listed perpetuals; their shares fell after Kalshi&\#x27;s earlier crypto-perp approval, and CME has sued the CFTC alleging the agency improperly approved the contracts.

<details><summary>References</summary>
<ul>
<li><a href="https://finance.yahoo.com/markets/commodities/articles/kalshi-launches-gold-silver-perpetual-175449558.html?fr=sycsrp_catchall">Kalshi launches gold and silver perpetual futures with CFTC ...</a></li>
<li><a href="https://www.kucoin.com/news/flash/kalshi-launches-gold-and-silver-perpetual-futures-with-cftc-approval">Kalshi Launches Gold and Silver Perpetual Futures with CFTC ...</a></li>
<li><a href="https://finance.yahoo.com/markets/stocks/articles/cboe-cme-ice-ndaq-stocks-183845986.html?fr=sycsrp_catchall">CBOE, CME, ICE, NDAQ Stocks Take A Hit After Kalshi&#x27;s Bitcoin ...</a></li>
<li><a href="https://scanx.trade/stock-market-news/equity-markets/cme-sues-cftc-over-kalshi-perpetual-futures-approval/43780384">CME sues CFTC over Kalshi perpetual futures approval</a></li>
<li><a href="https://fenado.ai/articles/cboe-shares-drop-76-as-cme-group-sues-cftc-over-perpetual-futures-approval">Cboe Shares Drop 7.6% as CME Group Sues CFTC Over Perpetual ...</a></li>

</ul>
</details>

**Tags**: `#CFTC`, `#perpetual futures`, `#Kalshi`, `#gold and silver`, `#market structure`

---

<a id="item-finance-news-2"></a>
### [Chinese AI chipmakers raise prices as HBM shortage bites](https://www.reuters.com/world/asia-pacific/chinas-ai-chipmakers-raise-prices-high-bandwidth-memory-shortage-bites-2026-09-10/) ⭐️ 7.0/10

Chinese AI chipmakers including Huawei and Cambricon are raising prices as a global shortage of high-bandwidth memory \(HBM\) tightens supply. Reuters reported Huawei&\#x27;s Ascend 950DT quotes are about 20%-50% higher than two months earlier and some older chips rose about 30%, while Cambricon&\#x27;s next-generation Siyuan 690 is expected to rise about 20%-30%.

telegram · zaihuapd · Sep 10, 09:29

**「Background」** HBM, a type of memory designed to feed AI processors, is mainly supplied by SK Hynix, Samsung, and Micron; U.S. export restrictions have further tightened its availability in China, making HBM a bottleneck as domestic AI-computing demand grows.

**「Impact」** The HBM shortage is becoming a bottleneck that constrains the expansion of China&\#x27;s domestic AI chip industry.

**Tags**: `#HBM shortage`, `#AI chips`, `#China semiconductor industry`, `#price increases`, `#export controls`

---