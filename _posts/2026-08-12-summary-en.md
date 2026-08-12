---
layout: default
title: "Horizon Summary: 2026-08-12 (EN)"
date: 2026-08-12
lang: en
---

> From 44 items, 17 important content pieces were selected

---

**Technology News**
1. [Qwen3.8-2.4T-A95B: Massive Open MoE Model Released](#item-tech-news-1) ⭐️ 9.0/10
2. [DeepSeek V4 Pro 0813: low cost, mixed coding results](#item-tech-news-2) ⭐️ 8.0/10
3. [Tailscale Traces Database Corruption to 16-Year-Old SQLite WAL Bug](#item-tech-news-3) ⭐️ 8.0/10
4. [Adam&\#x27;s Basis-Dependent Scaling Undermines Implicit Low-Rank Bias](#item-tech-news-4) ⭐️ 8.0/10
5. [LTX-2.5 open-source video model runs locally on a single RTX 5090](#item-tech-news-5) ⭐️ 8.0/10
6. [xAI Releases Grok 4.6 for Long-Running Agent Tasks](#item-tech-news-6) ⭐️ 8.0/10
7. [Zed&\#x27;s Delta Brings Multiplayer AI Conversations to the Editor](#item-tech-news-7) ⭐️ 7.0/10
8. [Why tiny JPEGs look different in Chrome](#item-tech-news-8) ⭐️ 7.0/10
9. [AI Is Removing the Middle Class of Software Engineering?](#item-tech-news-9) ⭐️ 7.0/10
10. [AI-Assisted Code Can Leave Teams Unable to Fix Bugs](#item-tech-news-10) ⭐️ 7.0/10
11. [WeChat Unveils WeLM, Resource-Efficient Large Language Model Family](#item-tech-news-11) ⭐️ 7.0/10

**Financial News**
1. [Zhu Rongji, Former Chinese Premier, Dies at 98](#item-finance-news-1) ⭐️ 9.0/10
2. [NYC Council Probes Prediction Market Marketing](#item-finance-news-2) ⭐️ 8.0/10
3. [Tencent Q2 Revenue Beats, Profit Misses as AI Capex Nearly Triples and Free Cash Flow Turns Negative](#item-finance-news-3) ⭐️ 8.0/10
4. [Premarket movers: CoreWeave and Super Micro Computer jump after earnings](#item-finance-news-4) ⭐️ 7.0/10
5. [China&\#x27;s EV market share hits 65.1% as auto sales slide](#item-finance-news-5) ⭐️ 7.0/10
6. [CME Group plans AI compute futures contracts](#item-finance-news-6) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Qwen3.8-2.4T-A95B: Massive Open MoE Model Released](https://huggingface.co/Qwen/Qwen3.8-2.4T-A95B) ⭐️ 9.0/10

Qwen released Qwen3.8-2.4T-A95B on Hugging Face, a Mixture-of-Experts language model with 2.4T total parameters and 95B active parameters, offered initially in BF16 and FP8. It has a native context length of 262,144 tokens, extendable to 1,010,000, and the model card positions its performance between Opus 4.8 and Fable 5, with community commenters treating it as a Kimi k3 rival. The BF16 full model is around 4.9TB, while a 1-bit quantized version from Unsloth is reported at roughly 397GB with 95B active, which commenters say brings Opus 4.5-level performance to hardware a normal person could buy. The open-weights release lacks the vision input, non-thinking support, and default 1M context length of the official Qwen3.8-Max, and its license permits free internal use or use below $50M annual revenue with restrictions above that threshold for serving the model or related services.

hackernews · Philpax · Aug 12, 15:01 · [Discussion](https://news.ycombinator.com/item?id=49273478)

**「Background」** Qwen3.8-2.4T-A95B is a sparse mixture-of-experts \(MoE\) language model from Qwen, with 2.4 trillion total parameters but only about 95 billion active per token, using 512 routed experts \(10 active\) plus one shared expert over a 92-layer hybrid-attention backbone. It is the open-weight variant of the commercial Qwen3.8 Max model, offering similar architecture but without some commercial features such as vision input and extended 1M context support. The model&\#x27;s design aims to deliver high capability at lower inference cost, and its size and quantization options are central to practical deployment discussions.

**「Impact」** The most concrete near-term consequence is that a ~397GB 1-bit quantized build with 95B active parameters makes model performance comparable to Opus 4.5 potentially runnable on consumer-scale hardware rather than multi-TB servers, widening who can deploy this scale of model. However, because Qwen shipped only BF16 and FP8 without QAT on q4, serving it at launch is harder than Kimi k3, and external quantization with substantial calibration data is needed to reach the ~1.3TB q4 size.

**「Community Discussion」** Commenters are excited about the practical quantization path, with one calling the 397GB 1-bit version astonishing because it brings Opus 4.5-level performance to machines a normal person could buy while still achieving usable tokens per second. Others note the open weights miss Qwen3.8-Max features like vision input and non-thinking support, and there is skepticism about serving requirements, exemplified by a joke about running the model on an Intel N100.

<details><summary>References</summary>
<ul>
<li><a href="https://recipes.vllm.ai/Qwen/Qwen3.8-2.4T-A95B">Qwen/Qwen3.8-2.4T-A95B | vLLM Recipes</a></li>
<li><a href="https://openrouter.ai/qwen/qwen3.8-2.4t-a95b">Qwen3.8 2.4T A95B - API Pricing &amp; Providers | OpenRouter</a></li>
<li><a href="https://modelslab.com/models/qwen/qwen-qwen3.8-2.4t-a95b">Qwen: Qwen3.8 2.4T A95B API | Text Generation | ModelsLab</a></li>

</ul>
</details>

**Tags**: `#AI`, `#LLM`, `#Qwen`, `#model release`, `#Mixture of Experts`

---

<a id="item-tech-news-2"></a>
### [DeepSeek V4 Pro 0813: low cost, mixed coding results](https://openrouter.ai/deepseek/deepseek-v4-pro-0813) ⭐️ 8.0/10

DeepSeek V4 Pro 0813 is a newly released major model from DeepSeek, listed on OpenRouter, that has drawn substantial Hacker News attention \(691 points, 241 comments\). The OpenRouter page itself lacks detailed information, but community testing indicates the model offers exceptionally low inference costs compared to competitors—one user&\#x27;s Codex CLI test on the same feature showed DeepSeek V4 Pro working for 12 minutes at $0.12 with a bug, while Grok 4.6 worked for 3 minutes 18 seconds at $1.41 without a bug. The model is part of DeepSeek&\#x27;s rapid update cycle, following a recent Flash update that another user described as surprisingly capable for development tasks at very low cost. The release matters because it highlights the growing cost-performance gap in AI models, making DeepSeek an attractive option for budget-conscious developers, though potentially requiring more verification or debugging effort.

hackernews · explosion-s · Aug 12, 16:04 · [Discussion](https://news.ycombinator.com/item?id=49274600)

**「Background」** DeepSeek V4 Pro 0813 is the flagship model in DeepSeek&\#x27;s V4 family, released on August 12, 2026, as a 1.6-trillion-parameter mixture-of-experts \(MoE\) model with 49 billion activated parameters, hybrid attention, three reasoning modes, and long-context efficiency. Vendor-reported agent benchmarks in the release show it ahead of the earlier V4 Flash 0731 and V4 Pro Preview on every listed agent benchmark. It is accessible through DeepSeek&\#x27;s official API and third-party providers such as OpenRouter, which is where the linked page appears.

**「Impact」** Developers using coding agents can cut costs dramatically by switching to DeepSeek V4 Pro, but should budget extra time for checking and fixing outputs, since an observed test showed it producing a bug where a more expensive model did not.

**「Community Discussion」** Commenters criticized linking to OpenRouter because the page has no useful information, with suggestions to link to the official API docs and benchmark charts instead. A head-to-head test showed DeepSeek V4 Pro was far cheaper but produced a bug, while Grok 4.6 was more expensive but bug-free; another user praised DeepSeek&\#x27;s previous Flash update for handling heavy development tasks at minimal cost, and one commenter noted that for most tasks they prefer cost-effective models like Kimi-K3, GLM-5.2, or MiniMax over more expensive options.

<details><summary>References</summary>
<ul>
<li><a href="https://deepseekv4pro.com/news/deepseek-v4-pro-0813-official-release-opus-fable-benchmarks">DeepSeek V 4 Pro 0813 : Opus 4.8 and Fable 5 Agent Benchmarks</a></li>
<li><a href="https://lmmarketcap.com/model/deepseek-v4-pro-0813">DeepSeek V 4 Pro 0813 - Pricing &amp; Benchmarks 2026 | LM Market Cap</a></li>
<li><a href="https://www.together.ai/models/deepseek-v4-pro-0813">DeepSeek V 4 Pro 0813 API: Pricing, Benchmarks &amp; Docs | Together AI</a></li>

</ul>
</details>

**Tags**: `#deepseek`, `#llm`, `#ai-models`, `#cost-performance`, `#openrouter`

---

<a id="item-tech-news-3"></a>
### [Tailscale Traces Database Corruption to 16-Year-Old SQLite WAL Bug](https://tailscale.com/blog/sqlite-wal-reset-bug) ⭐️ 8.0/10

Tailscale published a detailed root-cause analysis tracing database corruption in its control plane to a 16-year-old SQLite WAL-reset race condition. The bug occurred in a design where a single Go process exclusively accesses the database, which is how SQLite is meant to be used, but the underlying race can only occur under specific multi-connection conditions. Tailscale funded the development of an open-source SQLite VFS shim debugging tool to isolate the race condition, noting it will help track down similar bugs in the future. The write-up has drawn developer appreciation for its technical depth and for Tailscale&\#x27;s willingness to fund open-source debugging infrastructure.

hackernews · ropbear · Aug 12, 14:22 · [Discussion](https://news.ycombinator.com/item?id=49272832)

**「Background」** SQLite&\#x27;s write-ahead logging \(WAL\) mode allows concurrent readers and writers by appending changes to a log file and periodically resetting the log during a checkpoint. Tailscale&\#x27;s control plane database was corrupted by a rare data race in SQLite&\#x27;s source code between a checkpoint and a write transaction, a bug that has existed for about 16 years and can only be triggered when WAL mode is active with multiple database connections open on the same file. To isolate the issue, Tailscale funded the development of an open-source SQLite VFS shim, which added logging that eventually helped the SQLite developers identify and fix the underlying race condition.

**「Community Discussion」** Commenters praised the article and Tailscale&\#x27;s decision to fund a new open-source debugging tool, with one noting the article could have been more direct but still found the bug details satisfying. Another commenter highlighted that the race requires multiple connections, which contrasts with the single-writer design described in the post.

<details><summary>References</summary>
<ul>
<li><a href="https://tailscale.com/blog/sqlite-wal-reset-bug">How Tailscale helped find the SQLite WAL-Reset bug</a></li>
<li><a href="https://www.theregister.com/databases/2026/08/12/tailscale-says-deeply-buried-16-year-old-sqlite-bug-caused-last-years-outages/5287004">Tailscale says deeply buried 16-year-old SQLite bug caused last year&#x27;s outages</a></li>

</ul>
</details>

**Tags**: `#sqlite`, `#database`, `#bug`, `#wal`, `#tailscale`

---

<a id="item-tech-news-4"></a>
### [Adam&\#x27;s Basis-Dependent Scaling Undermines Implicit Low-Rank Bias](https://www.reddit.com/r/MachineLearning/comments/1vmjb3p/the_loss_does_not_see_the_basis_but_adam_does_r/) ⭐️ 8.0/10

A new preprint argues that Adam&\#x27;s per-coordinate second-moment scaling is basis-dependent in factored models W=UV^T, breaking the rotation invariance that gives gradient descent its implicit low-rank bias. In underdetermined matrix sensing at matched training loss, the author found that GD, shared-scalar Adam, Muon, and Shampoo preserve the bias, while Adam, RMSProp, Lion, signum, and Adafactor lose it. A one-parameter interpolation between per-coordinate and shared-scalar denominators improved recovery monotonically, pinpointing anisotropy rather than adaptivity as the cause. Unexpectedly, Muon behaved exactly on truly low-rank targets but degraded fastest as spectral tail energy increased, crossing below GD near 4% tail energy, reconciling conflicting prior reports. A caveat: the reported 43-44% held-out error reduction on hyperspectral data uses a train-only learning-rate rule that gives Adam its worst rate; with per-method tuning the gap shrinks considerably \(Appendix D.6\).

reddit · r/MachineLearning · /u/EtherealGlyph · Aug 12, 16:39

**「Background」** In a factored model W=UV^T, many rotations \(U,V\) -&gt; \(UQ,VQ\) leave the loss unchanged; gradient descent respects this symmetry, while Adam&\#x27;s coordinate-wise adaptive scaling depends on the basis in which U and V are written. In linear underdetermined problems like matrix sensing, optimizers that preserve the symmetry retain a bias toward low-rank solutions, which can improve recovery and generalization.

**「Impact」** For researchers and practitioners training factored or low-rank models with Adam, this suggests per-coordinate adaptivity can sacrifice the implicit low-rank bias; using a shared-scalar denominator variant or accepting Muon&\#x27;s sensitivity to spectral tail energy may restore it.

**Tags**: `#optimization`, `#Adam`, `#low-rank`, `#matrix sensing`, `#machine learning`

---

<a id="item-tech-news-5"></a>
### [LTX-2.5 open-source video model runs locally on a single RTX 5090](https://ltx.io/model/ltx-2-5) ⭐️ 8.0/10

LTX released LTX-2.5, an open-source video generation foundation model with its weights, training code, and inference pipeline fully available, and it can run locally on a single RTX 5090. The announcement states the model supports text-to-video and image-to-video generation, improves multi-shot coherence and prompt following, and uses a new diffusion video decoder plus a Gemma 4 12B text encoder. Commercial use is free for companies with annual revenue under $10 million. In a flaw-evaluation benchmark of 98 prompts, LTX 2.5 Pro ranked first among ten models.

telegram · zaihuapd · Aug 12, 02:15

**「Background」** LTX is the video-generation product line from Lightricks, which maintains the open-source LTX-Video repository supporting full fine-tuning and LoRA fine-tuning for the 2B and 13B model variants. LTX-2.5 continues that open-source approach as a diffusion-transformer-based video generation model, shipping with a pretrained checkpoint for deep fine-tuning.

**「Impact」** AI and ML practitioners can now run and fine-tune a full open-weights video generation model locally on one RTX 5090 and use it commercially without a license fee if their company earns under $10 million annually, enabling private, on-premises video generation without API dependence.

<details><summary>References</summary>
<ul>
<li><a href="https://ltx.io/model/open-source">LTX-2.5 Model Open Source: AI Video Generator</a></li>
<li><a href="https://github.com/Lightricks/LTX-Video">GitHub - Lightricks/LTX-Video: Official repository for LTX-Video</a></li>

</ul>
</details>

**Tags**: `#video generation`, `#open source`, `#diffusion model`, `#LTX`, `#AI model`

---

<a id="item-tech-news-6"></a>
### [xAI Releases Grok 4.6 for Long-Running Agent Tasks](https://x.ai/news/grok-4-6) ⭐️ 8.0/10

xAI released Grok 4.6 on August 12, 2026, building on Grok 4.5 with stronger long-running agent, interaction, and vision capabilities. It matches GPT-5.6 Sol on the Artificial Analysis intelligence index, which aggregates nine benchmarks. Grok 4.6 is available immediately in Cursor, Grok Build, and the API at $2 per million input tokens and $6 per million output tokens, with a fast tier at double the price. During the first week, users get double usage on Grok Build and Cursor.

telegram · zaihuapd · Aug 12, 15:54

**「Background」** Grok 4.5 was xAI&\#x27;s previous flagship model, and Grok 4.6 is positioned as an update focused on sustained agentic workflows rather than a full architectural shift. The Artificial Analysis intelligence index is a composite benchmark score used to compare frontier models across nine tests.

**「Impact」** Developers and Cursor or Grok Build users can immediately adopt Grok 4.6 at the listed API prices and receive double usage for the first week, while the composite benchmark parity suggests it is a viable alternative to GPT-5.6 Sol for agent workloads.

**「Community Discussion」** Commenters are split: some question how several labs reached Fable-level performance within two months, citing benchmarking or distillation concerns, while others call Grok a healthy competitor and report that Grok 4.5 felt faster and more concise than GPT-5.6 Sol or Claude. There are also complaints that the SpaceXAI API adds a default system prompt that can override user instructions and cause refusals to discuss system prompts.

**Tags**: `#Grok 4.6`, `#xAI`, `#AI agents`, `#model release`, `#API pricing`

---

<a id="item-tech-news-7"></a>
### [Zed&\#x27;s Delta Brings Multiplayer AI Conversations to the Editor](https://zed.dev/blog/introducing-delta) ⭐️ 7.0/10

Zed has announced Delta, a new feature that combines AI agents with real-time multi-user collaboration, allowing developers to share and edit AI conversation threads directly in the editor. The feature includes realtime collaborative multiplayer conversations and conversation-as-document, which enables inline commenting within an agent conversation thread. This matters because it expands collaborative coding beyond simple pair programming to include joint oversight of AI-generated changes, potentially helping teams debug and mentor junior developers. However, community reactions are mixed, with some developers questioning the necessity of multiplayer editing and others noting the verbosity of AI summaries. Specific performance data or limitations are not yet available from the announcement.

hackernews · khy · Aug 12, 18:19 · [Discussion](https://news.ycombinator.com/item?id=49276574)

**「Background」** Zed is an open-source, fast code editor that natively supports agentic AI editing, including Git operations and a built-in open-weight model called Zeta2 \(zed.dev\). The editor also supports real-time collaboration so users can share projects while retaining their own keybindings and settings. Delta, announced on Zed’s blog, appears to extend that collaboration to AI agent conversations, with the stated concepts of realtime multiplayer conversations and conversation-as-document inline comments, though the source article itself was not available for direct confirmation.

**「Impact」** For Zed users, Delta introduces a new workflow for collaborative AI-assisted development, particularly useful for mentoring and reviewing AI-generated PRs, though its practical value remains disputed among developers.

**「Community Discussion」** Commenters split on Delta&\#x27;s value: some highlight its utility for jumping into the AI thread behind a PR and mentoring junior engineers, while others argue coding is inherently single-player and AI summaries can miss edge cases or become verbose. Additionally, one commenter criticized the blog post&\#x27;s low-contrast design as hard to read.

<details><summary>References</summary>
<ul>
<li><a href="https://zed.dev/">Zed — Your last next editor</a></li>
<li><a href="https://zed.dev/ai">Zed — The AI Code Editor Built for Speed</a></li>
<li><a href="https://zed.101.dev/tutorials/collaboration.html">Collaboration in Zed - Zed 101</a></li>

</ul>
</details>

**Tags**: `#zed`, `#editor`, `#ai`, `#collaboration`, `#software development`

---

<a id="item-tech-news-8"></a>
### [Why tiny JPEGs look different in Chrome](https://guillaumetech.github.io/posts/jpg-scaling-chrome/) ⭐️ 7.0/10

Chrome&\#x27;s image downscaling behavior makes tiny JPEGs render differently than in Firefox; Chrome produces a blurrier result while Firefox is sharper but with more ringing artifacts. The article traces this to Chrome&\#x27;s &quot;optimization&quot; for downscaling, which also leaked into Electron releases and broke icons in production apps, causing at least one team to postpone an upgrade. Developers are advised to avoid JPEG for icons, use images at an appropriate resolution for display size, and can sometimes control the algorithm via the CSS image-rendering property, though browser behavior varies. Firefox is working on lower-scale decompression \(see Bugzilla 2033250\) to improve such cases.

hackernews · gutechh · Aug 12, 14:00 · [Discussion](https://news.ycombinator.com/item?id=49272549)

**「Background」** Web browsers frequently downscale large images to fit their displayed size, and they use different image scaling algorithms that produce visibly different results. For example, Firefox&\#x27;s high-quality downscaling uses a 3-lobed Lanczos filter, while Chrome and other browsers have historically applied different resampling methods, leading to inconsistencies in sharpness and blur when the same image is rendered at a smaller size. These differences have been an ongoing issue in web development, particularly for icons and images on high-DPI displays.

**「Impact」** Developers of web and Electron apps should verify small images at their displayed size in Chrome, since its downscaling algorithm can visibly blur icons and other UI elements that render sharply in Firefox. CSS image-rendering may help, but behavior varies by browser and DPI.

**「Community discussion」** Commenters confirm the issue also affects PNGs and can break icons in Electron apps, with one team delaying an Electron upgrade as a result. There is broad agreement on using appropriately sized images rather than oversized sources, while some prefer Firefox&\#x27;s sharper scaling over Chrome&\#x27;s blurrier output.

<details><summary>References</summary>
<ul>
<li><a href="https://entropymine.com/resamplescope/notes/browsers/">How web browsers resize images - entropymine.com</a></li>
<li><a href="https://stackoverflow.com/questions/9945363/image-scaling-causes-poor-quality-in-firefox-internet-explorer-but-not-chrome">Image scaling causes poor quality in firefox/internet ... Code sample</a></li>

</ul>
</details>

**Tags**: `#web-development`, `#browser`, `#image-scaling`, `#Chrome`, `#JPEG`

---

<a id="item-tech-news-9"></a>
### [AI Is Removing the Middle Class of Software Engineering?](https://blog.florianherrengt.com/ai-removing-middle-class-software-engineering.html) ⭐️ 7.0/10

In a blog post, Florian Herrengt argues that AI tools are disproportionately displacing mid-level software engineers, even while increasing the leverage of senior engineers and the potential damage caused by ineffective ones. The piece frames this as a structural shift in software engineering careers rather than a purely technical breakthrough, and it has generated substantial community debate. Since no concrete data is presented in the available material, the argument is analytical and forward-looking rather than an account of already-observed job losses.

hackernews · florianherrengt · Aug 12, 13:20 · [Discussion](https://news.ycombinator.com/item?id=49271994)

**「Background」** The article, originating from a blog post by Florian Herrengt, argues that AI coding tools are disproportionately displacing mid-level software engineers—the &\#x27;middle class&\#x27; of the profession—by automating the routine implementation work that has traditionally been handed off from senior engineers. It contends that AI has &\#x27;removed the speed limit&\#x27; on coding, which makes weak engineering cultures fail faster, while senior developers who focus on critical thinking and system design remain harder to replace. This debate sits against a history of tooling improvements that have repeatedly been predicted to replace programmers, with mixed outcomes.

**「Community Discussion」** Commenters broadly agree that AI tools amplify both good and bad engineering, with Syntaf warning that disengaged “bad” engineers can spread poor work across an organization and scronkfinkle describing AI as automating the “Stack Overflow engineer” tier. Others push back on the premise: rootusrootus asks whether there is real evidence of LLM-agent-driven job losses, and eshack94 stresses that engineers must not outsource critical thinking to models.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.florianherrengt.com/ai-removing-middle-class-software-engineering.html">AI is removing the middle class of software engineering</a></li>

</ul>
</details>

**Tags**: `#AI`, `#software engineering`, `#career`, `#LLM`, `#tech industry`

---

<a id="item-tech-news-10"></a>
### [AI-Assisted Code Can Leave Teams Unable to Fix Bugs](https://simonwillison.net/2026/Aug/12/florian-herrengt/) ⭐️ 7.0/10

Simon Willison shared a passage from Florian Herrengt&\#x27;s blog post &\#x27;AI is removing the middle class of software engineering&\#x27; in which Herrengt depicts a team trying to fix a recurring bug in an AI-built feature: the original developer no longer knows where the data comes from, and both he and a coworker watch an endless stream of confident AI output without being able to verify any of it. The excerpt argues that this project has become so convoluted, with so many layers and services, that nobody on the team can understand what is going on. The post is relevant to software engineering practice because it illustrates how AI-assisted development can lead to opaque, unmaintainable code and ongoing debugging challenges, a form of cognitive debt.

rss · Simon Willison · Aug 12, 15:08

**「Background」** Florian Herrengt&\#x27;s essay &\#x27;AI is removing the middle class of software engineering&\#x27; warns that AI-assisted development removes the former speed limit on producing code, allowing projects with weak engineering culture to fail much faster. His quoted scenario describes a team that relies on AI tools like Claude to write and even explain its own features, leaving a codebase so layered and convoluted that no one truly understands it. The commentary ties to the broader concern of &\#x27;cognitive debt,&\#x27; where generated code may work initially but becomes difficult to debug or maintain.

**「Impact」** For developers and teams that rely on generative AI assistants, the scenario highlights a concrete maintenance risk: code produced without a human tracing the data flow can leave teams unable to diagnose persistent bugs, making fixes depend on further AI guesses rather than understanding.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.florianherrengt.com/ai-removing-middle-class-software-engineering.html">AI is removing the middle class of software engineering</a></li>

</ul>
</details>

**Tags**: `#AI`, `#software engineering`, `#code maintainability`, `#AI-assisted development`, `#developer productivity`

---

<a id="item-tech-news-11"></a>
### [WeChat Unveils WeLM, Resource-Efficient Large Language Model Family](https://x.com/Weixin_WeChat/status/2087509298310209718) ⭐️ 7.0/10

WeChat&\#x27;s team has announced WeLM, a family of general-purpose large language models focused on resource efficiency. The deployed WeLM-80B model, which activates 3B parameters, now powers the in-app AI agent Xiaowei \(WeChat Xiaowei\), enabling users to perform dialogue and search, operate native WeChat functions, and call mini-program services. A larger WeLM-617B model with 23B activated parameters is under development using a mixture-of-experts \(MoE\) architecture, targeting stronger general understanding and reasoning at moderate activation scale. It will later be applied to complex WeChat ecosystem tasks such as intelligent mini-program development and generated tools for Xiaowei. The announcement highlights WeChat&\#x27;s push to scale AI capabilities across its massive user base while emphasizing compute efficiency.

telegram · zaihuapd · Aug 12, 13:58

**「Background」** Large language models \(LLMs\) are neural networks with billions of parameters trained on broad text data. Mixture-of-experts \(MoE\) architectures divide the network into specialized expert modules and activate only a subset of them for each input, allowing a very large model to run efficiently at moderate computational cost. Resource-efficient designs like WeLM are intended to reduce deployment costs while preserving strong performance.

**「Impact」** WeChat users with access to the Xiaowei agent may now complete conversations, searches, native operations, and mini-program actions through the WeLM-80B deployment, while developers and WeChat ecosystem partners could later benefit from the planned WeLM-617B-based mini-program generation and intelligent development tools.

**Tags**: `#large language models`, `#AI`, `#WeChat`, `#MoE`, `#NLP`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Zhu Rongji, Former Chinese Premier, Dies at 98](https://www.news.cn/politics/20260812/4c2c72e299ef4561915d2e507393a81f/c.html) ⭐️ 9.0/10

Zhu Rongji, former Chinese premier, died in Beijing on Aug. 12, 2026, at age 98, according to a joint announcement by the Communist Party Central Committee, the National People&\#x27;s Congress Standing Committee, the State Council and the Chinese People&\#x27;s Political Consultative Conference National Committee.

telegram · zaihuapd · Aug 12, 10:11

**「Background」** Zhu joined the Communist Party in 1949 and took office as premier in March 1998. During the Asian financial crisis, he promoted expansionary fiscal policy and prudent monetary policy, insisted on not devaluing the yuan, presided over the completion of China&\#x27;s World Trade Organization accession negotiations, and oversaw major reforms in finance, taxation, state-owned companies, housing and grain distribution.

**Tags**: `#China`, `#economic reform`, `#WTO`, `#fiscal policy`, `#monetary policy`

---

<a id="item-finance-news-2"></a>
### [NYC Council Probes Prediction Market Marketing](https://www.cnbc.com/2026/08/12/new-york-city-council-probes-prediction-markets-marketing-strategies.html) ⭐️ 8.0/10

The New York City Council has opened an investigation into marketing by prediction market platforms Polymarket, Kalshi, Coinbase and Gemini Titan, citing allegations of deceptive advertising and vowing to protect New Yorkers; Speaker Julie Menin said the council plans a hearing and may consider legislation or policy changes.

rss · CNBC Finance · Aug 12, 12:08

**「Background」** The probe follows a Wall Street Journal report that Polymarket made partnered content creators appear to be winning when they were not using their own money, and a related federal CFTC inquiry; New York state is separately suing Kalshi, Coinbase and Gemini over alleged illegal gambling.

**Tags**: `#prediction markets`, `#regulatory probe`, `#New York City Council`, `#consumer protection`, `#Polymarket`

---

<a id="item-finance-news-3"></a>
### [Tencent Q2 Revenue Beats, Profit Misses as AI Capex Nearly Triples and Free Cash Flow Turns Negative](https://wallstreetcn.com/articles/3779275) ⭐️ 8.0/10

Tencent reported Q2 2026 revenue of RMB 204.8 billion, up 11% year over year and slightly above Bloomberg estimates, but net profit rose only 0.7% to RMB 56 billion, missing expectations. Capital expenditure nearly tripled to RMB 52.8 billion, pushing free cash flow to negative RMB 13.8 billion.

telegram · zaihuapd · Aug 12, 10:30

**「Background」** The spending surge is tied to Tencent&\#x27;s AI infrastructure push; the company said that excluding prepayments for AI computing power, free cash flow would have been RMB 37.6 billion.

**Tags**: `#Tencent`, `#Q2 earnings`, `#capital expenditure`, `#AI investment`, `#free cash flow`

---

<a id="item-finance-news-4"></a>
### [Premarket movers: CoreWeave and Super Micro Computer jump after earnings](https://www.cnbc.com/2026/08/12/stocks-making-the-biggest-moves-premarket-crwv-smic-cohr.html) ⭐️ 7.0/10

Several stocks moved sharply in premarket trading after earnings and guidance. CoreWeave rose more than 18.5% after reporting second-quarter revenue of $2.58 billion, up 112% from a year earlier and above the $2.56 billion LSEG consensus, while Super Micro Computer gained about 7.5% after guiding first-quarter adjusted earnings to $1.01-$1.10 per share, above the 76-cent LSEG consensus, and revenue to $14.5 billion-$15.5 billion, above the $11.68 billion consensus.

rss · CNBC Finance · Aug 12, 12:12

**「Background」** Premarket trading occurs before regular U.S. market hours, often reacting to earnings released earlier, and consensus estimates are average analyst forecasts from LSEG or FactSet. CoreWeave, an AI cloud provider using Nvidia hardware, received a $2 billion Nvidia investment in January 2026.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/CoreWeave">CoreWeave - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#premarket movers`, `#earnings guidance`, `#technology stocks`, `#market reaction`, `#consensus estimates`

---

<a id="item-finance-news-5"></a>
### [China&\#x27;s EV market share hits 65.1% as auto sales slide](https://www.cnbc.com/2026/08/12/china-car-sales-data-byd-tesla-geely-vw.html) ⭐️ 7.0/10

New-energy vehicles, including battery-electric and hybrid cars, accounted for 65.1% of new passenger cars sold in China in July, up from 54% a year earlier, according to China Passenger Car Association data. For the year through July, overall passenger car sales fell 20.3% from a year earlier, while new-energy vehicle sales for that period dropped 12.5%.

rss · CNBC Finance · Aug 12, 01:20

**「Background」** China’s passenger-car market has contracted sharply in 2026 — overall sales fell 20.3% in the year through July — even as battery- and hybrid-powered new-energy vehicles made up 65.1% of July sales, up from 54% a year earlier.

**Tags**: `#China auto market`, `#EV sales`, `#BYD`, `#Tesla`, `#Geely`

---

<a id="item-finance-news-6"></a>
### [CME Group plans AI compute futures contracts](https://www.cnbc.com/2026/08/11/ai-computing-power-becomes-a-tradable-asset-class-as-cme-starts-futures.html) ⭐️ 7.0/10

CME Group plans to launch the first futures contracts tied to AI computing capacity on Oct. 5, pending regulatory approval, in partnership with Silicon Data. Each contract will represent a month&\#x27;s rent for an Nvidia H100 GPU and will be based on Silicon Data indexes tracking hourly rental prices for Nvidia H100 and Blackwell B200 chips.

rss · CNBC Finance · Aug 12, 14:14

**「Background」** The launch comes as Wall Street seeks new ways to finance the AI infrastructure buildout, including an effort by Nvidia with large asset managers that could channel as much as $500 billion into AI infrastructure.

**「Impact」** If approved, AI developers and data-center operators could use the contracts to hedge computing costs, while investors could gain exposure to AI capacity prices without owning data centers or chips.

**Tags**: `#AI`, `#CME`, `#Futures`, `#Commodities`, `#Nvidia`

---