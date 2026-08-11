---
layout: default
title: "Horizon Summary: 2026-08-11 (EN)"
date: 2026-08-11
lang: en
---

> From 45 items, 17 important content pieces were selected

---

**Technology News**
1. [Extracting Hidden Reasoning Traces from Proprietary LLM APIs](#item-tech-news-1) ⭐️ 8.0/10
2. [Meta&\#x27;s Muse Glimmer: 30B Open Apache 2.0 Agentic Model](#item-tech-news-2) ⭐️ 8.0/10
3. [Nvidia Debuts Nemotron 3.5 Lightning and NeMo Switchyard for Efficient AI Routing](#item-tech-news-3) ⭐️ 7.0/10
4. [Mojo 1.0 Released: Python Superset for AI Performance](#item-tech-news-4) ⭐️ 7.0/10
5. [Stratechery Analysis: Nvidia Faces Risk in AI Compute Demand](#item-tech-news-5) ⭐️ 7.0/10
6. [London Underground Begins Facial Recognition Scanning](#item-tech-news-6) ⭐️ 7.0/10
7. [Decoupled Descent Uses AMP Onsager Corrections to Match Train and Test Errors](#item-tech-news-7) ⭐️ 7.0/10
8. [HyperSAE applies hyperbolic geometry to sparse autoencoders, cutting MSE by 9.8%](#item-tech-news-8) ⭐️ 7.0/10
9. [Anthropic to Add AI Watermarks to Claude Content](#item-tech-news-9) ⭐️ 7.0/10
10. [Graphene-Based Soft Lens Tunes Focus With Electric Field](#item-tech-news-10) ⭐️ 7.0/10
11. [Manus Splits from Meta; Some User Data Will Be Deleted](#item-tech-news-11) ⭐️ 7.0/10

**Financial News**
1. [Stocks making big after-hours moves: Super Micro, CoreWeave, H&amp;R Block](#item-finance-news-1) ⭐️ 8.0/10
2. [Nvidia&\#x27;s $500 billion AI financing plan faces a major China risk](#item-finance-news-2) ⭐️ 8.0/10
3. [SK Hynix Restarts Dalian NAND Fab Expansion, China Output to Rise About 50%](#item-finance-news-3) ⭐️ 8.0/10
4. [State election-betting bans create legal uncertainty for prediction markets](#item-finance-news-4) ⭐️ 7.0/10
5. [Amkor Reportedly Explores Stake Sale in China Unit Valued at Up to $1.5 Billion](#item-finance-news-5) ⭐️ 7.0/10
6. [Hang Seng Tech Index Proposes Major Reform, Expanding from 30 to 50 Constituents](#item-finance-news-6) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Extracting Hidden Reasoning Traces from Proprietary LLM APIs](https://stolen-thoughts.com/) ⭐️ 8.0/10

A new article at stolen-thoughts.com, shared on Hacker News, presents techniques for extracting hidden chain-of-thought reasoning traces from proprietary LLM APIs instead of receiving only final answers. One approach involves replaying a trace produced by a frontier model into a weaker sibling model and jailbreaking the weaker model to reveal the internal reasoning. Another commenter reports using a two-sentence developer prompt injected around Codex&\#x27;s encrypted compaction to make models output the encrypted data in plaintext, while another method disables thinking and supplies a &\#x27;deep\_think&\#x27; tool that returns internal CoT reasoning. The discussion matters because it challenges API providers&\#x27; attempts to hide reasoning traces and raises unresolved questions about model output ownership, transparency, and whether vendors will further restrict access. Some participants argue the extraction is legitimate because users pay for tokens and model outputs are trained on the sum of human knowledge.

hackernews · quantumgarbage · Aug 11, 13:22 · [Discussion](https://news.ycombinator.com/item?id=49257876)

**「Background」** Leading large language model providers now conceal their models’ step-by-step reasoning, or chain-of-thought, to protect intellectual property and limit information leakage. Rather than storing these traces server-side, providers return them to the client as blocks of encrypted text, which the client passes back with each subsequent request. Building on prior research, the paper identifies techniques for extracting these hidden reasoning traces from proprietary LLM APIs, including replaying a trace produced by a frontier model into a weaker sibling model and jailbreaking that weaker model.

**「Impact」** Developers using APIs like Codex can currently extract internal reasoning traces through targeted prompt manipulation, which may push proprietary LLM vendors to strengthen protections or limit hidden reasoning output.

**「Community Discussion」** Commenters disagree on whether the technique is ethically problematic: one argues that users already paid for the tokens and that training on other model outputs is normal, while another expects future models to withhold reasoning unless users pay for enterprise APIs. Practical reports include prompting Codex to output encrypted compaction data in plaintext and using a &\#x27;deep\_think&\#x27; tool to reveal internal CoT reasoning.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2608.09867">Stealing Reasoning Traces from Proprietary LLM APIs</a></li>
<li><a href="https://stolen-thoughts.com/paper.pdf">Stealing Reasoning Traces from Proprietary LLM APIs</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#AI security`, `#chain-of-thought`, `#proprietary APIs`, `#jailbreak`

---

<a id="item-tech-news-2"></a>
### [Meta&\#x27;s Muse Glimmer: 30B Open Apache 2.0 Agentic Model](https://simonwillison.net/2026/Aug/10/introducing-muse-glimmer/#atom-everything) ⭐️ 8.0/10

Meta released Muse Glimmer, a new 30B open-weights model under the Apache 2.0 license, aimed at end-to-end agentic task completion, reliable tool use, and multi-step reasoning. The model claims strong results on benchmarks such as DeepSearch QA, MCP-Atlas, tau-Bench, and SWE-Bench, and it is a vision model capable of describing images. Simon Willison tested a quantized 18.16 GB version in LM Studio, generated a pelican image, and used it with his llm-coding-agent plugin against a Datasette checkout to explore code auth behavior. He notes that a 32 GB+ RAM machine can run the model while leaving room for other applications, and the Apache 2.0 license is a departure from Meta&\#x27;s earlier Llama license restrictions.

rss · Simon Willison · Aug 10, 23:56

**「Background」** Meta has introduced Muse Glimmer, a 30-billion-parameter dense model released under the Apache 2.0 license and available now. It is distilled from Meta&\#x27;s Muse Spark model and optimized for local agentic workflows such as tool use, multi-step reasoning, and end-to-end task completion, designed to run on consumer hardware with a single GPU \(around 24GB VRAM in one configuration\). The release marks a notable return to more permissive open weights for Meta, whose earlier open-weight Llama models used more restrictive licenses.

**「Impact」** Developers can now run Muse Glimmer locally for commercial agentic coding and tool-use tasks without the licensing constraints of Meta&\#x27;s earlier Llama releases, provided they have 32 GB or more of RAM.

<details><summary>References</summary>
<ul>
<li><a href="https://research.meta.ai/blog/introducing-muse-glimmer-open-agentic-model">Introducing Muse Glimmer: An Open Agentic Model That Runs on Your Device | Meta AI Research</a></li>
<li><a href="https://venturebeat.com/technology/meta-returns-to-open-source-with-muse-glimmer-an-apache-2-0-licensed-30b-parameter-ai-model-optimized-for-agents-available-now">Meta returns to open source with Muse Glimmer, an Apache 2.0 licensed 30B parameter AI model optimized for agents — available now | VentureBeat</a></li>
<li><a href="https://explainx.ai/blog/meta-muse-glimmer-open-weight-30b-agentic-model-2026">Muse Glimmer: Meta&#x27;s 30B Open Model Runs on 24GB VRAM | explainx.ai Blog | explainx.ai</a></li>

</ul>
</details>

**Tags**: `#Meta`, `#open source`, `#AI`, `#agentic`, `#large language model`

---

<a id="item-tech-news-3"></a>
### [Nvidia Debuts Nemotron 3.5 Lightning and NeMo Switchyard for Efficient AI Routing](https://blogs.nvidia.com/blog/nemotron-lightning-switchyard-rtx-dgx/) ⭐️ 7.0/10

Nvidia announced Nemotron 3.5 Lightning, a family of small language models, alongside NeMo Switchyard, an open-source library that routes each request to the most capable and suitable model. The release reflects a broader push toward smaller, more efficient models as an alternative to multi-trillion-parameter systems. Nemotron 3.5 Lightning models are designed to run on local hardware, including Apple Silicon via MLX; a 30B variant is available and one user reported running it with OpenCode on an older Mac, albeit slowly. NeMo Switchyard targets deployment efficiency by intelligently directing requests, though practical questions remain about prompt caching and session consistency. The announcement positions Nvidia around lightweight deployment and routing rather than ever-larger models.

hackernews · droidjj · Aug 11, 19:35 · [Discussion](https://news.ycombinator.com/item?id=49263340)

**「Background」** Nemotron 3.5 Lightning is a 30-billion-parameter mixture-of-experts model that NVIDIA designed for specialized tasks within larger multi-agent systems, aiming to provide faster and more efficient agentic AI. NeMo Switchyard is the accompanying open-source library that directs each request to the most suitable model in a system, letting developers connect Lightning or other models without rewriting their agent stack. This release fits a broader trend toward smaller, more efficient models, partly driven by memory and cost pressures from very large trillion-parameter systems.

**「Impact」** For developers deploying AI on constrained hardware, Nemotron 3.5 Lightning and NeMo Switchyard provide an open-source way to mix smaller specialized models and reduce reliance on large serving stacks, with early community experience showing the 30B model works on Apple Silicon via MLX but runs slowly.

**「Community Discussion」** Commenters generally welcomed the focus on small efficient models, arguing that multi-trillion-parameter models may be missing fundamental insights and that efficiency-driven work will produce structural gains. Others raised implementation concerns about how the router handles prompt caching, whether sessions remain sticky to a single model, and benchmark graphs that omit most Qwen models.

<details><summary>References</summary>
<ul>
<li><a href="https://blogs.nvidia.com/blog/nemotron-lightning-switchyard-rtx-dgx/">NVIDIA Nemotron 3 . 5 Lightning and NeMo Switchyard Deliver...</a></li>
<li><a href="https://cobusgreyling.medium.com/nvidia-nemotron-3-5-lightning-5c38fbeacc0b">NVIDIA Nemotron 3 . 5 Lightning . The Execution Engine for... | Medium</a></li>
<li><a href="https://news.google.com/stories/CAAqNggKIjBDQklTSGpvSmMzUnZjbmt0TXpZd1NoRUtEd2lFLTkzZ0VSRzRRV09uVFdBRWt5Z0FQAQ?hl=en-US&amp;gl=US&amp;ceid=US:en">Google News - Nvidia Nemotron 3 . 5 Lightning - Overview</a></li>

</ul>
</details>

**Tags**: `#nvidia`, `#nemotron`, `#small-language-models`, `#model-routing`, `#open-source`

---

<a id="item-tech-news-4"></a>
### [Mojo 1.0 Released: Python Superset for AI Performance](https://www.modular.com/blog/modular-26-5-mojo-1-0-is-here) ⭐️ 7.0/10

Modular released Mojo 1.0, a key milestone for its Python-superset language designed for high-performance AI, with a commitment to open-source the compiler and toolchain in 2026. The release includes components built with Mojo in MAX, and the team says it will continue progressively open-sourcing language components. However, community discussion reveals unresolved concerns about the value of a closed-source compiler, the project&\#x27;s shifting stance on being a full Python superset, and its positioning versus other languages. The source item did not include detailed feature or performance information, so concrete performance data remains unavailable.

hackernews · dayanruben · Aug 11, 16:56 · [Discussion](https://news.ycombinator.com/item?id=49261128)

**「Background」** Mojo is a programming language developed by Modular Inc., which was founded by Chris Lattner \(creator of Swift and LLVM\) and Tim Davis. It is designed to combine Python&\#x27;s ease of use with the high performance needed for AI applications, targeting CPUs, GPUs, and other accelerators. Originally pitched as a potential superset of Python, the official roadmap now says Mojo may or may not evolve into a full superset. The compiler is currently closed-source, but Modular has committed to open-sourcing the Mojo compiler and toolchain in 2026.

**「Impact」** AI/ML developers considering a high-performance Python superset now have a versioned Mojo 1.0 to evaluate, but the closed-source compiler and uncertain superset direction may discourage adoption until the 2026 open-sourcing.

**「Community discussion」** Commenters asked for a one-page overview to clarify Mojo&\#x27;s problem statement, questioned the value of a closed-source compiler when Python can already offload to Rust libraries, and noted that the roadmap says Mojo &\#x27;may or may not&\#x27; become a full Python superset. Some expressed hope for Mojo while others criticized waiting until 2026 for source availability.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mojo_%28programming_language%29">Mojo (programming language) - Wikipedia</a></li>
<li><a href="https://www.modular.com/blog/the-path-to-mojo-1-0">Modular: The path to Mojo 1.0</a></li>

</ul>
</details>

**Tags**: `#mojo`, `#programming-language`, `#ai`, `#python`, `#release`

---

<a id="item-tech-news-5"></a>
### [Stratechery Analysis: Nvidia Faces Risk in AI Compute Demand](https://stratechery.com/2026/nvidias-risky-business/) ⭐️ 7.0/10

Stratechery published an analysis dated 2026, &quot;Nvidia&\#x27;s Risky Business,&quot; examining Nvidia&\#x27;s business risks and strategic position in AI hardware and software. The piece reportedly evaluates the company&\#x27;s competitive moat, including the role of its software ecosystem and the sustainability of compute demand growth assumptions. It is significant because it questions whether Nvidia&\#x27;s high market expectations are justified and offers a critical perspective for investors and industry watchers. No further article details were available in the supplied metadata.

hackernews · jonbaer · Aug 11, 10:02 · [Discussion](https://news.ycombinator.com/item?id=49255710)

**「Background」** Stratechery is a technology industry analysis publication by Ben Thompson. This article, published August 11, 2026, examines risks in Nvidia&\#x27;s AI-centric strategy, including its dominant hardware and software position and the sustainability of demand for compute. The discussion around the piece highlights Nvidia&\#x27;s entrenched CUDA software ecosystem and questions about how accurately forecasts of continued demand growth reflect reality.

**「Community Discussion」** Commenters generally agreed that Nvidia&\#x27;s strongest moat is its software ecosystem&\#x27;s deep entrenchment in ML research, though one developer described CUDA as one of the worst software development ecosystems imaginable. Others highlighted risks in second-order demand growth assumptions, Nvidia&\#x27;s pivot toward robotics, and its strong but not absolute position in the West relative to China, with one skeptically comparing AI&\#x27;s current capabilities to biological systems.

<details><summary>References</summary>
<ul>
<li><a href="https://stratechery.com/2026/nvidias-risky-business/">Nvidia ’ s Risky Business – Stratechery by Ben Thompson</a></li>
<li><a href="https://news.ycombinator.com/item?id=49255710">Nvidia &#x27; s Risky Business | Hacker News</a></li>

</ul>
</details>

**Tags**: `#Nvidia`, `#AI hardware`, `#business strategy`, `#software ecosystem`, `#industry analysis`

---

<a id="item-tech-news-6"></a>
### [London Underground Begins Facial Recognition Scanning](https://www.btp.police.uk/news/btp/news/england/btp-expands-live-facial-recognition-lfr-trial-into-london-underground-stations/) ⭐️ 7.0/10

British Transport Police has begun expanding a live facial recognition \(LFR\) trial into London Underground stations, according to the force&\#x27;s announcement. The trial reportedly scans passengers&\#x27; faces and matches them against watchlists in real time, marking a notable expansion of police biometric surveillance within a major public transport network. No specific station names, trial dates, or arrest figures were provided in the available announcement. The move intensifies ongoing concerns about privacy and civil liberties, especially since commenters note that anonymous travel on the Underground was already undermined by the widespread use of bank cards and contactless payments at barriers.

hackernews · BlueBerry2001 · Aug 11, 09:40 · [Discussion](https://news.ycombinator.com/item?id=49255496)

**「Background」** Live Facial Recognition \(LFR\) technology uses cameras to scan faces in real time and compare them against watchlists, typically to identify wanted individuals. The British Transport Police \(BTP\) has been trialling LFR on the rail network, deploying it 18 times between February and July at major London train stations and scanning over 530,000 faces. It now plans to expand the trial into Transport for London \(TfL\) Underground stations, moving the technology into a new transport environment to assess its effectiveness and refine its use.

**「Impact」** Passengers using London Underground stations included in the trial may now have their faces scanned and checked against police watchlists in real time. This adds a new layer of surveillance to a transport system where travel is already linked to payment data, while doing little to address commenters&\#x27; concerns about the trial&\#x27;s reversibility or its potential use beyond immediate arrests.

**「Community Discussion」** Commenters are broadly critical, arguing that the trial will likely be expanded rather than reversed and that it could be used to identify, infiltrate, and disrupt movements rather than simply catch criminals. Several also note that the loss of anonymous travel began with contactless payment adoption, with one commenter calling Britain an &\#x27;original Orwellian society&\#x27; and another sarcastically questioning whether the technology will actually solve street crime.

<details><summary>References</summary>
<ul>
<li><a href="https://www.btp.police.uk/news/btp/news/england/btp-expands-live-facial-recognition-lfr-trial-into-london-underground-stations/">BTP expands Live Facial Recognition (LFR) trial into London Underground stations | British Transport Police</a></li>
<li><a href="https://www.bbc.co.uk/news/articles/c07r0gvgjxyo">Facial recognition cameras to be trialled at London Tube stations - BBC News</a></li>
<li><a href="https://www.itv.com/news/london/2026-08-11/live-facial-recognition-technology-to-be-deployed-at-tube-stations">Live facial recognition technology to be deployed at Tube stations | ITV News London</a></li>

</ul>
</details>

**Tags**: `#facial recognition`, `#privacy`, `#surveillance`, `#AI ethics`, `#London`

---

<a id="item-tech-news-7"></a>
### [Decoupled Descent Uses AMP Onsager Corrections to Match Train and Test Errors](https://www.reddit.com/r/MachineLearning/comments/1vlu1se/decoupled_descent_enforcing_exact_traintest_error/) ⭐️ 7.0/10

A researcher has released &\#x27;Decoupled Descent&\#x27; \(DD\), a training method designed to enforce exact train–test error tracking in neural networks by applying approximate message passing \(AMP\) Onsager corrections at each parameter iterate. The work, presented as a theory paper on arXiv \(2604.27883\), frames generalization failure in full-batch gradient descent as a result of data reuse bias and demonstrates DD on stylized Gaussian mixture models and a high-dimensional XOR model with a bespoke two-layer network over 100 simulations. The author reports that DD provides a certificate that training error asymptotically equals testing error, which could support optimal stopping and hyperparameter tuning. The paper is explicitly preliminary for large models, and the author plans a future PyTorch-compatible package.

reddit · r/MachineLearning · /u/mlovik1 · Aug 11, 21:06

**「Background」** In supervised learning, gradient-based training can exhibit a generalization gap: the training error drops toward zero while the test error plateaus or even increases, a phenomenon often attributed to the reuse of training data. Approximate message passing \(AMP\) is a high-dimensional statistical framework that uses an Onsager correction term to track how errors propagate across iterative updates, enabling exact asymptotic predictions for certain stylized models. Decoupled Descent builds on this theory by introducing a train-test identity that enforces the training error to asymptotically match the test error at each parameter iterate, initially for Gaussian mixture models.

**「Impact」** For researchers studying generalization and training dynamics, DD offers a theoretical proof-of-concept that AMP-style corrections can make training and test error track each other, potentially enabling principled early stopping and hyperparameter selection, though practical scaling to large models remains unvalidated.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2604.27883v1">Decoupled Descent: Exact Test Error Tracking Via Approximate Message Passing</a></li>
<li><a href="https://arxiv.org/abs/2604.27883">[2604.27883] Decoupled Descent: Exact Test Error Tracking Via Approximate Message Passing</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#generalization`, `#optimization`, `#approximate message passing`, `#neural networks`

---

<a id="item-tech-news-8"></a>
### [HyperSAE applies hyperbolic geometry to sparse autoencoders, cutting MSE by 9.8%](https://www.reddit.com/r/MachineLearning/comments/1vlpyh2/hypersae_decoupled_poincar%C3%A9_geometry_for_sparse/) ⭐️ 7.0/10

HyperSAE, a PyTorch library for mechanistic interpretability, applies decoupled Poincaré hyperbolic geometry to sparse autoencoders \(SAEs\) while keeping the forward pass entirely Euclidean and causal steering as a single vector addition. On Gemma-2-2B Layer 13 trained on 20M tokens of FineWeb-Edu on an NVIDIA L4, it reduced reconstruction MSE by 9.8% \(4.5724 to 4.1232\), raised CE loss recovery from 75.5% to 78.9%, and cut dead latents from 3.8% to 0.2% versus a FlatSAE baseline. The design projects dictionary weights into the Poincaré ball during training and adds an entailment cone loss that places parent concepts near the origin and child concepts near the boundary. The library, paper, and pip install are available on GitHub.

reddit · r/MachineLearning · /u/visha1v · Aug 11, 18:37 · [Discussion](https://www.reddit.com/r/MachineLearning/comments/1vlpyh2/hypersae_decoupled_poincar%C3%A9_geometry_for_sparse/)

**「Background」** Standard sparse autoencoders \(SAEs\) embed dictionary atoms in Euclidean space, whose volume grows polynomially, but LLM concepts form branching hierarchies whose possible combinations grow exponentially, producing collisions, dead latents, and degraded reconstruction at large dictionary sizes. HyperSAE addresses this by making the training geometry hyperbolic \(Poincaré ball\) while keeping inference Euclidean, plus an entailment cone loss.

**「Impact」** For researchers using SAEs in mechanistic interpretability, HyperSAE provides an evidence-supported way to reduce dead latents and reconstruction error on large models while keeping inference Euclidean, which is especially useful when training large dictionaries.

**Tags**: `#sparse autoencoders`, `#mechanistic interpretability`, `#hyperbolic geometry`, `#PyTorch`, `#LLM interpretability`

---

<a id="item-tech-news-9"></a>
### [Anthropic to Add AI Watermarks to Claude Content](https://support.claude.com/en/articles/16266773-how-claude-marks-ai-generated-content) ⭐️ 7.0/10

Anthropic announced it will embed machine-readable watermarks and digital signature provenance metadata in Claude outputs, aligning with the EU AI Act Article 50\(2\) transparency code of practice. New Claude models released in the EU on or after August 2, 2026 will include the markers from launch, covering Claude&\#x27;s API, Claude, Claude Code, Claude Cowork, and Claude Tag products across global use. Text watermarks are invisible, and supported files will use the C2PA provenance standard. Anthropic is also adding markers to older models released before that date and plans to publish detection technical details. The company notes that detecting a marker only indicates content may have been processed by Claude, and its absence does not prove content was not AI-generated.

telegram · zaihuapd · Aug 11, 03:06

**「Background」** The EU AI Act sets transparency obligations for AI-generated content, requiring providers to mark outputs so users can recognize when they interact with artificial intelligence. Article 50\(2\) specifically addresses generative AI systems, prompting signatories like Anthropic to adopt technical measures such as machine-readable watermarks and provenance metadata like C2PA.

**「Impact」** Developers and enterprises using Claude products will need to handle new metadata and C2PA provenance in outputs, while users can verify potential AI origin through the planned detection tools, though the markers are not foolproof.

**Tags**: `#AI transparency`, `#Anthropic`, `#Claude`, `#watermarking`, `#EU AI Act`

---

<a id="item-tech-news-10"></a>
### [Graphene-Based Soft Lens Tunes Focus With Electric Field](https://www.qmul.ac.uk/news/latest-news/2026/science-and-engineering/se/new-graphene-powered-soft-lens-could-pave-the-way-for-smarter-glasses-cameras-and-medical-devices.html) ⭐️ 7.0/10

Researchers at Queen Mary University of London, led by James Busfield, have built a transparent soft lens from reduced graphene oxide that changes focal length when a small electric field is applied, avoiding the bulky moving parts used in traditional lenses. The work is published in Advanced Functional Materials. The prototype mimics the human eye: the electric field stretches a soft membrane to reshape the lens and focus on objects at different distances. The team integrated ultrathin transparent graphene electrodes directly into the actuator layer beneath the lens, overcoming the previous limitation that opaque electrodes had to be placed only at the lens edge, and significantly shrinking the device. They say the technology could eventually be used in autofocus cameras, wearable displays, VR/AR headsets, and miniature medical imaging devices, though electrode transparency and performance still need improvement.

telegram · zaihuapd · Aug 11, 12:27

**「Background」** Conventional autofocus lenses typically rely on moving glass elements driven by motors, which add bulk and complexity; alternative liquid lenses use fluids but often also require pumps or mechanical housings. Graphene and reduced graphene oxide are attractive for this application because they combine electrical conductivity with optical transparency, allowing electrodes to be placed in the optical path without blocking light. This work builds on those properties to make a compact, electrically tunable soft lens.

**「Impact」** For researchers and developers in optics and materials science, the validated integration of transparent graphene electrodes into a soft lens offers a concrete path toward compact electrically tunable optics, though commercial devices are not yet available.

**Tags**: `#graphene`, `#optics`, `#AR/VR`, `#medical-imaging`, `#materials-science`

---

<a id="item-tech-news-11"></a>
### [Manus Splits from Meta; Some User Data Will Be Deleted](https://manus.im/zh-tw/blog/a-note-to-our-users) ⭐️ 7.0/10

AI assistant Manus is separating from Meta and returning to independent operations. As part of the split, data generated by some users on or after December 29, 2025 \(the day Meta acquired Manus\) will be deleted between August 23, 2026 08:00 and August 24, 2026 \(Singapore time\). Affected users can export data via backup tools before August 23, 2026 07:59 and regain access from August 25, 2026 08:00. Manus says the deletion is required to comply with regulatory requirements in certain jurisdictions during the separation. Affected paid users will not be charged during the backup period and will receive return rewards after restoration; unaffected users need no action.

telegram · zaihuapd · Aug 11, 14:14

**「Context」** Manus is an AI assistant startup that was acquired by Meta Platforms in a $2 billion deal. In April, Chinese regulators demanded that Meta unwind the acquisition, prompting Manus to announce it will resume operating as an independent company. The company is now executing the separation, including deleting user data generated on or after the acquisition date to comply with regulatory requirements in certain jurisdictions.

**「Impact」** Users who generated data with Manus on or after the Meta acquisition date must export before August 23, 2026 07:59 or lose that data, while affected paid users avoid charges during the backup period and receive return rewards after restoration.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/08/11/manus-china-meta-acquisition.html">Manus to return as independent company after China forced Meta to unwind $2 billion deal</a></li>
<li><a href="https://www.theinformation.com/briefings/manus-return-independent-company-meta-deal-unwinds">Manus to Return as an Independent Company as Meta Deal Unwinds — The Information</a></li>
<li><a href="https://qz.com/manus-independent-meta-acquisition-china-unwind-081126?.tsrc=rss">Manus returns to independence after China blocks Meta acquisition</a></li>

</ul>
</details>

**Tags**: `#AI`, `#data governance`, `#Meta`, `#startup`, `#industry news`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Stocks making big after-hours moves: Super Micro, CoreWeave, H&amp;R Block](https://www.cnbc.com/2026/08/11/stocks-making-the-biggest-moves-after-hours-smci-crwv-hrb.html) ⭐️ 8.0/10

Several stocks moved after hours following earnings and forecasts: Super Micro Computer rose more than 8% after beating fourth-quarter estimates and guiding first-quarter adjusted earnings to $1.01-$1.10 per share, above the 76-cent consensus; CoreWeave gained 14% after second-quarter revenue jumped 112% to $2.58 billion, ahead of the $2.56 billion expected; H&amp;R Block surged 15% after forecasting fiscal 2027 adjusted earnings of $6.04-$6.24 per share, above the $5.86 consensus.

rss · CNBC Finance · Aug 11, 21:18

**「Background」** The moves came after companies released their latest quarterly results after the market close; Super Micro and CoreWeave are closely tied to AI infrastructure spending.

**Tags**: `#Earnings`, `#Guidance`, `#Artificial Intelligence`, `#After-Hours Movers`, `#Super Micro Computer`

---

<a id="item-finance-news-2"></a>
### [Nvidia&\#x27;s $500 billion AI financing plan faces a major China risk](https://www.cnbc.com/2026/08/11/nvidia-ai-funding-jensen-huang-china-risk.html) ⭐️ 8.0/10

Nvidia announced a plan with six large asset managers—BlackRock, Blackstone, Apollo, KKR, Brookfield and Goldman Sachs—to build a $500 billion financing pipeline for AI data centers and GPU clusters, betting that Nvidia chips will hold value like infrastructure assets. The biggest risk, according to structured-finance expert Ben Emons, is a Chinese price war that could rapidly erode GPU collateral values and leave investors exposed to losses.

rss · CNBC Finance · Aug 11, 21:01

**「Background」** The plan treats GPUs as collateral that can be repossessed and resold if borrowers default, similar to buildings or ships, but chips depreciate faster than real estate; Nvidia argues its CUDA software keeps older chips productive longer.

**「Impact」** If used-chip prices fall faster than expected, lenders and investors in GPU-backed loans could face losses, and high-risk borrowers such as AI startups and neoclouds may be most exposed.

**Tags**: `#Nvidia`, `#AI infrastructure`, `#financing`, `#GPU depreciation`, `#China risk`

---

<a id="item-finance-news-3"></a>
### [SK Hynix Restarts Dalian NAND Fab Expansion, China Output to Rise About 50%](https://en.sedaily.com/finance/2026/08/11/sk-hynix-to-boost-china-nand-output-50-percent-with-dalian) ⭐️ 8.0/10

SK Hynix is restarting construction of its second NAND flash fab in Dalian, China, a move expected to raise its local output by about 50%, according to Seoul Economic Daily. The new line is planned at roughly 50,000 wafers per month, with equipment move-in scheduled for late this year and mass production in the first half of next year, as AI data-center demand for enterprise SSDs has helped push NAND prices up nearly tenfold over the past year.

telegram · zaihuapd · Aug 11, 16:21

**「Background」** The Dalian site is SK hynix&\#x27;s NAND flash base, operated by its Solidigm subsidiary after the 2021 acquisition of Intel&\#x27;s NAND business, and the second fab there broke ground four years ago before work was paused during a memory downcycle.

<details><summary>References</summary>
<ul>
<li><a href="https://en.sedaily.com/finance/2026/08/11/sk-hynix-to-boost-china-nand-output-50-percent-with-dalian">SK hynix to Boost China NAND Output 50% With Dalian Plant ...</a></li>

</ul>
</details>

**Tags**: `#SK Hynix`, `#NAND`, `#capacity expansion`, `#AI datacenter`, `#memory market`

---

<a id="item-finance-news-4"></a>
### [State election-betting bans create legal uncertainty for prediction markets](https://www.cnbc.com/2026/08/11/do-state-election-betting-bans-apply-to-prediction-markets.html) ⭐️ 7.0/10

Wisconsin’s election commission said last month that betting on elections, including trades on prediction-market exchanges, is illegal under a state law more than 175 years old, and violators lose the right to vote in that election. Twenty-three states have similar election-betting bans, according to Pew Research Center, but officials in many states are unsure whether those laws apply to prediction-market trades.

rss · CNBC Finance · Aug 11, 18:44

**「Background」** The Commodity Futures Trading Commission treats event contracts as federally regulated swaps, while states argue they can regulate betting on elections under their constitutional power over election management. A 2024 federal appeals court allowed platforms to list election contracts, but it did not rule on whether state betting bans apply.

**「Impact」** Platforms like Kalshi and Polymarket face state penalties and shutdowns, and bettors in states such as Wisconsin or New York could be fined, jailed, or barred from voting in the affected election while the legal uncertainty persists.

**Tags**: `#prediction markets`, `#election betting`, `#regulation`, `#legal uncertainty`, `#CFTC`

---

<a id="item-finance-news-5"></a>
### [Amkor Reportedly Explores Stake Sale in China Unit Valued at Up to $1.5 Billion](https://www.bloomberg.com/news/articles/2026-08-11/amkor-is-said-to-explore-stake-sale-in-1-5-billion-china-unit) ⭐️ 7.0/10

Bloomberg, citing people familiar with the matter, reports that Amkor Technology is exploring selling a stake in its China business, with the unit potentially valued at $1 billion to $1.5 billion; the talks are preliminary and Amkor may keep a minority stake. A company representative declined to comment.

telegram · zaihuapd · Aug 11, 07:21

**「Background」** Amkor is the world&\#x27;s second-largest outsourced semiconductor packaging and testing company; it opened its Shanghai packaging plant in 2001 and announced a separate $1.5 billion multi-year agreement with Nvidia in July 2026 to develop next-generation AI chip packaging technology.

**Tags**: `#Amkor`, `#semiconductor`, `#China`, `#M&amp;A`, `#divestiture`

---

<a id="item-finance-news-6"></a>
### [Hang Seng Tech Index Proposes Major Reform, Expanding from 30 to 50 Constituents](https://www.stcn.com/article/detail/4068889.html) ⭐️ 7.0/10

Hang Seng Index Company has proposed a major overhaul of the Hang Seng Tech Index, expanding the number of constituents from 30 to 50 and introducing a two-track selection system in which 40 stocks are chosen by market cap and 10 by revenue growth over the past 12 months. The changes are still under consultation and are expected to be announced by the end of September 2026 and take effect in December 2026.

telegram · zaihuapd · Aug 11, 09:06

**「Background」** Launched in 2020, the index has been heavily concentrated in internet platforms—earning it the nickname &\#x27;takeout delivery index&\#x27;—and has fallen more than 24% from its October high even after rebounding over 14% from late-June lows; the reform aims to bring in more advanced hardware and AI companies.

**「Impact」** If finalized, the revision would affect investors in index-tracking funds, which would gain exposure to a broader set of Hong Kong-listed tech firms.

**Tags**: `#Hang Seng Tech Index`, `#index reform`, `#Hong Kong market`, `#ETFs`, `#technology stocks`

---