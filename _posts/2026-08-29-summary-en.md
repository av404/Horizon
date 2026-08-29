---
layout: default
title: "Horizon Summary: 2026-08-29 (EN)"
date: 2026-08-29
lang: en
---

> From 35 items, 14 important content pieces were selected

---

**Technology News**
1. [Z.ai Releases Open-Weight GLM-5.3 with Strong Benchmarks](#item-tech-news-1) ⭐️ 9.0/10
2. [Triton 3.8.0 adds aggregate types, tl.topk descending, backend improvements](#item-tech-news-2) ⭐️ 8.0/10
3. [Htmx 4.0 Released with Alpine.js Compatibility](#item-tech-news-3) ⭐️ 8.0/10
4. [Just a rumour of a bug is enough to find a security exploit these days](#item-tech-news-4) ⭐️ 8.0/10
5. [U.S. Sanctions Italian Hosting Provider Autistici/Inventati](#item-tech-news-5) ⭐️ 7.0/10
6. [Tiny Latent Flow Transformer Generates Faces on RP2350 MCU](#item-tech-news-6) ⭐️ 7.0/10
7. [Tencent Open-Sources Hy4 Preview, Slightly Beats GLM-5.3 and Kimi K3 on Blind Tests](#item-tech-news-7) ⭐️ 7.0/10
8. [FTC Probes YouTube Over Content Policies and Account Bans](#item-tech-news-8) ⭐️ 7.0/10
9. [OpenAI Ends Cursor Model Supply After SpaceX Acquisition](#item-tech-news-9) ⭐️ 7.0/10

**Financial News**
1. [Corn and Wheat Futures Jump to Multi-Year Highs on Supply Concerns](#item-finance-news-1) ⭐️ 8.0/10
2. [Appeals court rules against prediction markets in fight over sports event contracts](#item-finance-news-2) ⭐️ 8.0/10
3. [China Extends Maximum Mortgage Term From 30 to 40 Years](#item-finance-news-3) ⭐️ 8.0/10
4. [Warsh Speech Puts September Fed Rate Hike Odds Near 50%](#item-finance-news-4) ⭐️ 7.0/10
5. [Premarket movers: PayPal slides on buyout report; Affirm, Gap jump on earnings](#item-finance-news-5) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Z.ai Releases Open-Weight GLM-5.3 with Strong Benchmarks](https://huggingface.co/zai-org/GLM-5.3) ⭐️ 9.0/10

Z.ai has released GLM-5.3 as an open-weight model on Hugging Face \(zai-org/GLM-5.3\), with weights available for download, running, and customization. The company says the model shares its base with GLM-5.2 and that all improvements come from post-training, targeting agentic coding and cyber-defense workloads. Reported benchmark gains include Terminal Bench 2.1 score of 88.2 and DeepSWE score of 66.9, both well ahead of GLM-5.2. A custom GLM-5.3 License allows individuals and SMBs to use, fine-tune, and commercialize the model, though it includes an additional restriction for companies exceeding $10B in trailing 12-month revenue.

hackernews · jeudesprits · Aug 28, 15:20 · [Discussion](https://news.ycombinator.com/item?id=49479878)

**「Background」** GLM-5.3 is the latest open-weight model in Z.ai&\#x27;s GLM series of large language models, released on 14 August 2026 with its weights available for download and customization. It shares the same base model as GLM-5.2, with improvements coming from post-training, and is distributed under a custom GLM-5.3 License that permits free use, fine-tuning, and commercial use for individuals and small-to-medium businesses while restricting large enterprises once they exceed revenue thresholds. The GLM family is known as a self-hostable alternative to proprietary models, and prior versions have been deployed in contexts where American proprietary models were blocked by safety guardrails.

**「Impact」** For developers and organizations that self-host open models, GLM-5.3 offers a strong new option with benchmark-leading agentic coding and long-horizon task performance under a permissive custom license for individuals and SMBs.

**「Community Discussion」** Commenters were broadly positive, calling GLM-5.3 a &quot;sweet spot&quot; open-weights model with strong reasoning and one saying it &quot;feels like Opus 4.8&quot;; tests reportedly handled hard problems that DeepSeek Flash lacked intuition for. A recurring caveat was that earlier GLM/Qwen models overthink on complex data tasks, generating 3-4x more tokens than Opus/GPT, though the token-vs-accuracy ratio in GLM-5.3 was viewed as promising.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GLM_%28AI%29">GLM (AI) - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#open-source`, `#LLM`, `#GLM`, `#AI`, `#HuggingFace`

---

<a id="item-tech-news-2"></a>
### [Triton 3.8.0 adds aggregate types, tl.topk descending, backend improvements](https://github.com/triton-lang/triton/releases/tag/v3.8.0) ⭐️ 8.0/10

Triton 3.8.0 has been released, introducing public aggregate types through \`@triton.aggregate\` and \`@gluon.aggregate\` with inherited fields, default values, immutable instances, and \`aggregate\_replace\(\)\`. \`tl.topk\` now accepts a \`descending\` argument to return the smallest values, tensor descriptors may appear in tuple-valued kernel arguments, and the interpreter supports \`tl.dot\_scaled\`. The compiler backend adds generic multi-CTA support, an autotuning listener, deterministic JIT cache keys, and new sanitizers \(FpSan, GSan, ConSan\) with expanded coverage for NVIDIA and AMD gfx942/gfx950/gfx1250 targets. AMD/HIP gains gfx1250/CDNA5 improvements such as scaled WMMA variants and buffer atomics, while the pinned LLVM revision includes correctness fixes for GFX950 and SLP-vectorizer issues. The release notes also document breaking changes and contributor acknowledgments.

github · warrendeng · Aug 28, 18:25

**「Background」** Triton is an open-source, Python-based language and compiler for writing custom GPU kernels, especially for deep-learning primitives, and is designed to offer higher productivity than CUDA while retaining high performance. It originated from OpenAI&\#x27;s release of Triton 1.0 in 2021 and has since become a widely used tool in the AI/ML ecosystem, with development continuing in the triton-lang/triton repository. The v3.8.0 release builds on this foundation by adding new frontend APIs such as aggregate types and enhanced tl.topk, along with backend improvements for AMD and NVIDIA GPUs.

**「Impact」** Kernel authors can now use \`@triton.aggregate\` and \`tl.topk\(descending=False\)\` as public APIs, while developers targeting AMD gfx1250/CDNA5 gain scaled WMMA, buffer atomics, and expanded tensor data movement support.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/triton-lang/triton">GitHub - triton-lang/triton: Development repository for the ...</a></li>
<li><a href="https://openai.com/index/triton/">Introducing Triton: Open-source GPU programming for neural ...</a></li>

</ul>
</details>

**Tags**: `#Triton`, `#GPU`, `#compiler`, `#AI/ML`, `#release`

---

<a id="item-tech-news-3"></a>
### [Htmx 4.0 Released with Alpine.js Compatibility](https://four.htmx.org/announcements/2026-08-28-htmx-4.0.0-is-released) ⭐️ 8.0/10

Htmx 4.0.0 was released on August 28, 2026, as a major version of the hypermedia-oriented web UI library. The release includes \`hx-alpine-compat\`, an attribute that smooths over compatibility issues between htmx and Alpine.js, and has drawn substantial community attention. The update matters because it renews htmx&\#x27;s position as a lightweight alternative to complex JavaScript front-end stacks for hypermedia-driven applications.

hackernews · rmsaksida · Aug 28, 13:28 · [Discussion](https://news.ycombinator.com/item?id=49478178)

**「Background」** htmx is an open-source JavaScript library that lets developers build dynamic web interfaces using hypermedia attributes in HTML, avoiding heavy client-side JavaScript frameworks. The 4.0.0 release is a major update that rebuilds htmx&\#x27;s internals based on lessons from fixi.js and over five years of supporting htmx, with a key change being a migration to the Fetch API \(sometimes called &quot;the fetch\(\)ening&quot;\). It also introduces new features such as \`hx-alpine-compat\` to smooth compatibility with Alpine.js, and provides an upgrade guide for migrating from htmx 2.x to 4.x. The official announcement notes that htmx 2.x remains the latest npm tag until early 2027, while htmx 4.0 moves toward a stable release.

**「Community Discussion」** Commenters were generally enthusiastic, with the htmx CEO saying he cannot wait to try the new version and a developer describing the Go + htmx + SQLite stack as simple and fast. One contrarian comment noted that htmx made things harder for developers used to .NET API backends with Angular frontends because it moves presentation concerns into backend-generated UI, and another suggested Alpine Ajax as a smaller alternative.

<details><summary>References</summary>
<ul>
<li><a href="https://four.htmx.org/announcements/2026-08-28-htmx-4.0.0-is-released">htmx 4 . 0 . 0 has been released ! ~ htmx</a></li>
<li><a href="https://medium.com/django-journal/htmx-4-0-alpha-in-django-fetch-api-superpowers-for-real-time-uis-early-benchmarks-vs-htmx-2-x-2b68407a22cc">HTMX 4 . 0 Alpha in Django: Fetch API Superpowers for... | Medium</a></li>
<li><a href="https://web.archive.org/web/20251103222343/https://htmx.org/essays/the-fetchening/">htmx ~ The fetch() ening</a></li>

</ul>
</details>

**Tags**: `#htmx`, `#web development`, `#open source`, `#javascript`, `#hypermedia`

---

<a id="item-tech-news-4"></a>
### [Just a rumour of a bug is enough to find a security exploit these days](https://simonwillison.net/2026/Aug/28/just-a-rumour-of-a-bug/) ⭐️ 8.0/10

Anil Madhavapeddy, a Cambridge professor and core maintainer of the OCaml compiler, reports that OCaml projects now see attempted exploit probes within minutes of security patches being shared for discussion; his website fielded probes for percent-encoded traversal sequences about ten minutes after posting. He attributes this to modern coding agents that can turn a hint about a bug into an exploit, and says he demonstrated it with his own agents, using DeepSeek V4 Pro when Claude Fable refused the task. He argues the speed is incompatible with existing open source embargo practices, so communities need new processes for handling issues safely. rclone maintainer Nick Craig-Wood confirmed the problem in Hacker News comments, saying rclone received about 20 GitHub security disclosures in its first 10 years but over 40 in the last month, with roughly 75% containing something worth investigating. Craig-Wood also reported GitHub CVE assignment has slowed from 2-3 days to 3-4 weeks, forcing point releases with CVE-PENDING entries in changelogs.

rss · Simon Willison · Aug 28, 22:12

**「Background」** Open source security practice typically relies on coordinated disclosure: maintainers prepare a fix privately under an embargo and release it before exploit details become public. AI coding agents that watch public repositories and inspect patches and commit messages can reconstruct the underlying flaw from the smallest hint, shrinking that window from days to minutes. This post documents automated watchers scanning repositories as soon as a patch is shared for discussion.

**「Impact」** Affected open source maintainers now face a flood of security disclosures—rclone went from about 20 in a decade to over 40 in one month—and exploit probes before official releases, while delayed CVE assignment forces them to ship with CVE-PENDING entries.

**「Community discussion」** Commenters largely agreed the dynamic is real but split on what it means: bri3d argued that building exploits from patch hints predates LLMs, which have instead scaled the practice to mass exploitation of low-value targets, while godelski said the bigger problem is a lack of will to fix bugs. stephbook countered that deployment and update lag are the real bottleneck, and rndhouse described building a tool that monitors commits to detect silent bug fixes using GPT-5.5-class models.

**Tags**: `#security`, `#AI agents`, `#open source`, `#vulnerability exploitation`, `#OCaml`

---

<a id="item-tech-news-5"></a>
### [U.S. Sanctions Italian Hosting Provider Autistici/Inventati](https://www.inventati.org/) ⭐️ 7.0/10

The U.S. government has imposed sanctions on the Italian hosting provider Autistici/Inventati \(A/I Collective\), designating the organization and its noblogs.org platform as affiliated with global terrorism. The action targets internet infrastructure rather than specific individuals, raising unprecedented concerns about the chilling effect on privacy tools, open-source projects, and providers that host content for radical groups. Commenters note that the designation could set a precedent for treating users and developers of anonymizing or privacy-focused systems such as I2P, Monero, Veilid, Tox, and Signal as terrorist-affiliated. The move follows earlier sanctions-related discussion on Hacker News and has reportedly caused outages or dysfunction on some A/I services.

hackernews · exiguus · Aug 28, 12:58 · [Discussion](https://news.ycombinator.com/item?id=49477854)

**「Background」** Autistici/Inventati \(A/I Collective\) is an Italy-based collective that operates privacy-focused digital services, including encrypted email accounts and the Noblogs blogging platform. The U.S. State Department and Treasury recently designated the collective as a Specially Designated Global Terrorist, alleging that it builds and operates digital infrastructure for violent far-left militants and Antifa cells. The designation is notable because it targets a hosting and privacy service provider, which has raised alarm about the broader chilling effect on privacy tools and open-source projects.

**「Impact」** The Aug. 26 U.S. Treasury/State designation of Autistici/Inventati as a Specially Designated Global Terrorist immediately blocks the collective’s U.S.-connected property and interests, and puts pressure on the banks, hosts, and infrastructure providers that keep its privacy-focused email, chat, hosting, and Noblogs services online, threatening disruption for the independent and open-source projects that rely on them.

**「Community Discussion」** Commenters largely view the designation as unprecedented and dangerous, warning that infrastructure providers for radical groups could be treated as terrorists, with broad implications for privacy and open-source communities. Others debate the historical context and dispute whether Autistici/Inventati has directly supported the PKK, with some noting difficulty verifying links because of service outages.

<details><summary>References</summary>
<ul>
<li><a href="https://www.state.gov/releases/office-of-the-spokesperson/2026/08/designation-of-autistici-inventati-as-a-specially-designated-global-terrorist/">Designation of Autistici/Inventati as a Specially Designated ...</a></li>
<li><a href="https://home.treasury.gov/news/press-releases/sb0616/">Treasury Takes Action Against Violent Far-Left Terrorist ...</a></li>
<li><a href="https://techandbusiness.org/newswire/IfCKeYYCbu4DC4Tb4R0aWk">US sanctions Italian digital-services provider Autistici ...</a></li>
<li><a href="https://www.state.gov/releases/office-of-the-spokesperson/2026/08/designation-of-autistici-inventati-as-a-specially-designated-global-terrorist/">Designation of Autistici/Inventati as a Specially Designated ...</a></li>
<li><a href="https://news.lavx.hu/article/u-s-sanctions-put-autistici-inventati-s-resilient-network-under-pressure">U.S. sanctions put Autistici/Inventati’s resilient network ...</a></li>

</ul>
</details>

**Tags**: `#sanctions`, `#internet infrastructure`, `#privacy`, `#hosting`, `#open source`

---

<a id="item-tech-news-6"></a>
### [Tiny Latent Flow Transformer Generates Faces on RP2350 MCU](https://www.reddit.com/r/MachineLearning/comments/1w10tax/i_implemented_a_very_tiny_image_generation_model/) ⭐️ 7.0/10

A developer \(/u/cpldcpu\) implemented a 2.4–4 million parameter latent flow transformer on an RP2350 microcontroller that generates 128×128 face images in about 20 seconds. The 12-layer model uses AdaLN-Zero conditioning and classifier-free guidance \(CFG\) to improve image quality, and int8 quantization with ReLU² activation to exploit sparsity. The inference engine streams weights from flash via DMA while the previous layer computes, enabling full on-device execution. The generated image is displayed on a monitor or transferred over USB. The project demonstrates that a very small parameter count can still produce capable image generation, with a repository link provided.

reddit · r/MachineLearning · /u/cpldcpu · Aug 28, 19:48

**「Background」** The RP2350 is a low-cost microcontroller from Raspberry Pi, introduced in August 2024 with dual Arm Cortex-M33 cores running at 150 MHz and hardware floating-point support, commonly used on boards like the Raspberry Pi Pico 2. Latent Flow Transformers \(LFTs\) are a neural architecture that compresses stacks of discrete transformer layers into continuous flow-matching transport operators, often operating in a low-dimensional latent space for efficient generative modeling of images and other data. This context helps explain the technical significance of running a quantized 2.4-4M parameter LFT image generation model directly on such a microcontroller.

**「Impact」** This demonstration shows that sub-5M-parameter latent flow transformers with sparsity-aware inference can run generative image models on inexpensive microcontrollers, opening up fully offline edge inference for low-power embedded devices.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/RP2350">RP2350 - Wikipedia</a></li>
<li><a href="https://www.raspberrypi.com/products/rp2350/">Buy an RP2350 – Raspberry Pi</a></li>
<li><a href="https://arxiv.org/abs/2505.14513">[2505.14513] Latent Flow Transformer - arXiv.org Latent Flow Transformer - arXiv.org Latent Flow Transformers (LFT) - emergentmind.com Latent Flow Transformer (LFT) - emergentmind.com GitHub - itz-sayak/Latent-Flow-Transformer Paper page - Latent Flow Transformer - Hugging Face Latent Flow Transformer - catalyzex.com</a></li>

</ul>
</details>

**Tags**: `#embedded-ml`, `#microcontrollers`, `#transformers`, `#image-generation`, `#edge-inference`

---

<a id="item-tech-news-7"></a>
### [Tencent Open-Sources Hy4 Preview, Slightly Beats GLM-5.3 and Kimi K3 on Blind Tests](https://mp.weixin.qq.com/s/ymr3X878B8oa2XP15CH8TQ) ⭐️ 7.0/10

On August 28, 2026, Tencent released the open-source Hy4 preview, describing it as its strongest open model. The Mixture-of-Experts model has 770B total parameters with 49B active, supports a 1M-token context window, and targets long-cycle software engineering, document/office work, and scientific research. In a blind evaluation across 203 engineering tasks, it scored 2.99, slightly ahead of GLM 5.3&\#x27;s 2.92 and Kimi K3&\#x27;s 2.94. It is available on Tencent Cloud, GitHub, HuggingFace, ModelScope, AtomGit, and OpenRouter. API pricing is $0.834 per million input tokens and $2.501 per million output tokens.

telegram · zaihuapd · Aug 28, 06:11

**「Background」** Tencent&\#x27;s Hy4 preview is a Mixture-of-Experts \(MoE\) large language model, a design that keeps a very large total parameter count while activating only a small subset per token—here 770B total with 49B active. This sparse-activation approach balances model capacity with inference cost, and the model&\#x27;s 1M-token context window supports long-document and software-engineering workloads. The release continues Tencent&\#x27;s pattern of open-sourcing its Hunyuan LLM family, following broader industry trends toward larger MoE models and longer context windows.

**「Impact」** Developers and organizations seeking open-weight long-context models for engineering and documentation work now have Hy4 preview, which offers incremental blind-test gains over GLM-5.3 and Kimi K3 while introducing a paid API with a $2.501 per million output token price.

<details><summary>References</summary>
<ul>
<li><a href="https://www.aibase.com/news/30694">Tencent Hunyuan launches open - source flagship model Hy 4 preview ...</a></li>
<li><a href="https://www.kucoin.com/news/flash/tencent-hunyuan-releases-and-opens-source-hy4-preview-with-770b-total-parameters">Tencent HunYuan releases and open - sources the Hy 4 preview with...</a></li>
<li><a href="https://www.brocker.org/tencent-hy4-preview-open-source-770b-parameters-1m-context">Tencent open - sources Hy 4 preview 770 B MoE model</a></li>

</ul>
</details>

**Tags**: `#tencent`, `#hunyuan`, `#large language model`, `#open-source`, `#AI`

---

<a id="item-tech-news-8"></a>
### [FTC Probes YouTube Over Content Policies and Account Bans](https://www.bloomberg.com/news/articles/2026-08-27/us-ftc-probing-youtube-over-social-media-policies) ⭐️ 7.0/10

The US Federal Trade Commission is investigating Alphabet&\#x27;s YouTube over whether its account bans and content-moderation practices violate consumer protection law. According to people familiar with the matter, the probe began last year and has reached its final stage before a possible lawsuit. Investigators are focusing on whether YouTube violates its own user policies when it bans or demotes content, and whether users are misled into thinking certain posts are allowed before removal or account bans. YouTube and the FTC declined to comment, and the company has not been accused of wrongdoing.

telegram · zaihuapd · Aug 28, 07:48

**「Background」** The FTC is the US agency that enforces consumer-protection statutes prohibiting unfair or deceptive business practices, including how companies describe their own policies. This investigation treats YouTube&\#x27;s content rules and enforcement as a potential consumer disclosure issue: if users are led to believe certain content is allowed and then it is removed, that may be considered misleading.

**「Impact」** If the investigation results in a lawsuit, YouTube could face FTC enforcement action and increased pressure to align its published content policies with how its moderation systems actually operate.

**Tags**: `#YouTube`, `#FTC`, `#content moderation`, `#regulation`, `#Alphabet`

---

<a id="item-tech-news-9"></a>
### [OpenAI Ends Cursor Model Supply After SpaceX Acquisition](https://openai.com/index/our-decision-on-cursor-following-its-acquisition-by-spacex/) ⭐️ 7.0/10

OpenAI announced it will terminate the contract that supplies OpenAI models through Cursor because SpaceX has acquired the AI coding tool company, setting a recommended cutoff date of November 12, 2026, and using the maximum notice period the agreement permits. OpenAI said it cannot be confident SpaceX will honor the service terms, citing a pattern of violations by Elon Musk&\#x27;s companies, including a contract breach after the Twitter acquisition and xAI&\#x27;s sworn admission earlier this year that it had violated OpenAI&\#x27;s service terms. The arrangement was a custom agreement allowing OpenAI to end cooperation within a limited time after a change of control, and the two companies had worked together for nearly four years. The decision affects users of Cursor&\#x27;s OpenAI-powered features, giving them just over a year to prepare for the change.

telegram · zaihuapd · Aug 29, 02:24

**「Background」** Cursor is an AI-powered code editor that has relied on OpenAI&\#x27;s models for close to four years, and OpenAI&\#x27;s custom contract let it cancel cooperation after a change of control. SpaceX&\#x27;s acquisition of Cursor triggered that clause, and OpenAI is exercising it because it does not trust SpaceX or related Musk-owned companies to comply with its usage terms.

**「Impact」** By November 12, 2026, Cursor users will lose access to OpenAI models unless a replacement provider or new agreement is put in place, forcing developers to plan for migration or alternative AI coding tools.

**Tags**: `#OpenAI`, `#Cursor`, `#SpaceX`, `#AI tools`, `#industry`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Corn and Wheat Futures Jump to Multi-Year Highs on Supply Concerns](https://www.cnbc.com/2026/08/28/corn-and-wheat-prices-jump-to-highest-prices-in-more-than-three-years.html) ⭐️ 8.0/10

Corn and wheat futures jumped to their highest levels in more than three years, with wheat settling at 784 cents per bushel \(up 12.1% on the week\) and corn at 536.5 cents per bushel \(up 5.5% on the week\) amid Black Sea export disruptions and tighter U.S. supply expectations.

rss · CNBC Finance · Aug 28, 20:00

**「Background」** Wheat’s rally is tied mainly to disruptions to Black Sea grain exports from Russia and Ukraine, which together account for more than a quarter of global wheat exports; corn’s rally reflects lower U.S. crop estimates and constrained Ukrainian exports.

**「Impact」** According to AgMarket.Net’s Jim McCormick, Europe’s drought-hit corn crop may lead the region to substitute wheat for animal feed, adding further pressure to wheat supplies.

**Tags**: `#corn`, `#wheat`, `#commodity prices`, `#supply disruptions`, `#agriculture`

---

<a id="item-finance-news-2"></a>
### [Appeals court rules against prediction markets in fight over sports event contracts](https://www.cnbc.com/2026/08/28/appeals-court-rules-against-prediction-markets-tees-up-scotus-fight.html) ⭐️ 8.0/10

The 9th U.S. Circuit Court of Appeals rejected requests by Kalshi, Crypto.com and Robinhood to stop Nevada and other states from treating sports event contracts as gambling, ruling that such contracts are not federally regulated swaps and setting up a likely Supreme Court fight.

rss · CNBC Finance · Aug 29, 02:23

**「Background」** The decision conflicts with a 3rd Circuit ruling from April, creating a circuit split over whether sports-related event contracts fall under the Commodity Futures Trading Commission&\#x27;s exclusive swap authority or state gambling law. The platforms and the CFTC argued all event contracts are swaps, while 44 states said they are sports betting.

**Tags**: `#prediction markets`, `#CFTC`, `#sports betting`, `#regulation`, `#Supreme Court`

---

<a id="item-finance-news-3"></a>
### [China Extends Maximum Mortgage Term From 30 to 40 Years](https://news.ifeng.com/c/8vxm6huJOMR) ⭐️ 8.0/10

China&\#x27;s central bank and financial regulator announced on Oct. 28 that the maximum term for personal housing loans will be extended from 30 years to 40 years, with the exact term to be agreed between the borrower and the commercial bank.

telegram · zaihuapd · Aug 28, 12:16

**「Background」** The policy is part of a joint guideline on reforming real estate credit management to support a new real estate development model, giving lenders and borrowers more flexibility in setting loan terms.

**Tags**: `#中国房地产`, `#住房贷款`, `#信贷政策`, `#央行`, `#金融监管`

---

<a id="item-finance-news-4"></a>
### [Warsh Speech Puts September Fed Rate Hike Odds Near 50%](https://www.cnbc.com/2026/08/28/-september-fed-decision-now-a-coin-flip-as-rate-hike-odds-increase.html) ⭐️ 7.0/10

After Fed Chair Kevin Warsh said at Jackson Hole that he is committed to fighting inflation, traders on Kalshi, CME FedWatch and Polymarket now put roughly 48-56% odds on a quarter-point rate hike at the Federal Reserve&\#x27;s Sept. 16 meeting, up from nearly 70% odds that the Fed would hold before the speech. No rate decision has been made.

rss · CNBC Finance · Aug 28, 15:22

**「Background」** The Fed left rates steady in July, but three members of its rate-setting committee dissented in favor of a hike; expectations for September cooled after a weak July jobs report and cooler inflation, which Warsh said were not enough to show underlying trends had improved.

**Tags**: `#Federal Reserve`, `#monetary policy`, `#interest rates`, `#inflation`, `#market expectations`

---

<a id="item-finance-news-5"></a>
### [Premarket movers: PayPal slides on buyout report; Affirm, Gap jump on earnings](https://www.cnbc.com/2026/08/28/stocks-making-the-biggest-moves-premarket-pypl-afrm-gap-mrvl.html) ⭐️ 7.0/10

PayPal dropped nearly 16% premarket after Bloomberg reported, citing people familiar with the matter, that Advent and Stripe had decided not to pursue a buyout of PayPal. Affirm rose 13% after reporting $1.17 billion in fiscal fourth-quarter revenue, above the $1.11 billion estimate from LSEG, Gap gained 15% after beating adjusted earnings estimates and naming a new Old Navy CEO, and Elastic jumped over 17% on stronger full-year guidance; Marvell, Rubrik and Autodesk slipped after some forecasts or margins missed estimates.

rss · CNBC Finance · Aug 28, 11:43

**「Background」** Premarket moves reflect trading before U.S. markets open, driven by company news and earnings. The reported PayPal deal would have been one of the largest leveraged buyouts, a purchase financed mostly with debt.

**Tags**: `#earnings`, `#mergers and acquisitions`, `#premarket movers`, `#technology stocks`, `#retail`

---