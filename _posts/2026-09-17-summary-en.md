---
layout: default
title: "Horizon Summary: 2026-09-17 (EN)"
date: 2026-09-17
lang: en
---

> From 42 items, 15 important content pieces were selected

---

**Technology News**
1. [Nvidia announces native Rust GPU kernel programming for CUDA](#item-tech-news-1) ⭐️ 8.0/10
2. [Micron Shows 512 GB DDR5 RDIMM, Targets 2027 Production](#item-tech-news-2) ⭐️ 8.0/10
3. [4B Model Claims 81% Faster Query Plans Than Postgres](#item-tech-news-3) ⭐️ 7.0/10
4. [Xiaomi MiMo 2.6 live post-training dashboard draws Hacker News attention](#item-tech-news-4) ⭐️ 7.0/10
5. [Mistral and Mozilla announce private, multilingual AI browsing collaboration](#item-tech-news-5) ⭐️ 7.0/10
6. [Hackers Accessed Flock Camera, Exposing Hardcoded Credentials](#item-tech-news-6) ⭐️ 7.0/10
7. [Anthropic merges Claude Cowork and chat into one Claude](#item-tech-news-7) ⭐️ 7.0/10
8. [TMLR quizzes authors of 10 papers slated for desk rejection](#item-tech-news-8) ⭐️ 7.0/10
9. [GoBench benchmarks LLMs on 9x9 Go against KataGo](#item-tech-news-9) ⭐️ 7.0/10
10. [Cloudflare adds per-domain setting to block AI training while keeping search indexing](#item-tech-news-10) ⭐️ 7.0/10
11. [Chinese-language casino sites hide APT malware C2 infrastructure](#item-tech-news-11) ⭐️ 7.0/10
12. [Sina Cloud SAE Shutdown Threatens 420 TB of Early Bilibili Video Data](#item-tech-news-12) ⭐️ 7.0/10

**Financial News**
1. [Fed raises rates for the first time in over three years, signals another hike possible this year](#item-finance-news-1) ⭐️ 9.0/10
2. [Hong Kong announces 11 measures to encourage childbirth](#item-finance-news-2) ⭐️ 7.0/10
3. [China Opens Pinglu Canal, a New Southwest-to-ASEAN Shipping Route](#item-finance-news-3) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Nvidia announces native Rust GPU kernel programming for CUDA](https://developer.nvidia.com/blog/introducing-cuda-rust-two-tracks-for-writing-gpu-kernels/) ⭐️ 8.0/10

Nvidia has announced native GPU programming in Rust through an official developer blog post introducing CUDA Rust with two tracks for writing GPU kernels. The move extends CUDA tooling to Rust developers and is especially relevant to systems, GPU, and AI infrastructure programmers who want to write kernels in Rust. The announcement drew significant technical discussion, with commenters debating Rust&\#x27;s safety benefits, CUDA vendor lock-in, and the quality of the article itself. Because the supplied item does not include the full blog text, the concrete APIs, toolchain requirements, hardware support, and compatibility constraints are not specified here.

hackernews · nonmaskable · Sep 16, 11:15 · [Discussion](https://news.ycombinator.com/item?id=49724881)

**「Background」** CUDA has traditionally meant writing GPU kernels in CUDA C++ or using wrappers around other languages, while Rust support largely came through bindings rather than native kernel code. Nvidia&\#x27;s CUDA Rust aims to close that gap by letting kernels be written in Rust and compiled natively to PTX, with two tracks that mirror CUDA&\#x27;s own programming models: the SIMT model via the open-source cuda-oxide project and the newer Tile model via cutile-rs. Both are early-stage NVlabs projects, and they use Rust&\#x27;s ownership rules to reject aliasing bugs at compile time.

**「Impact」** Rust developers targeting Nvidia GPUs gain an officially supported path for kernel programming, though the provided evidence does not establish whether it reduces CUDA vendor lock-in or replaces existing C++ workflows.

**「Community Discussion」** Commenters broadly welcomed Rust&\#x27;s safety promise for GPU kernels, but disagreement centered on CUDA&\#x27;s proprietary nature and vendor lock-in, with one critic preferring separate kernel files and manual launches as in Metal, OpenCL, and D3D12. Others framed the release as a useful step toward native Rust kernels and, for at least one commenter, a rare opportunity to learn Rust that large language models have not yet been trained on.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.nvidia.com/blog/introducing-cuda-rust-two-tracks-for-writing-gpu-kernels/">Introducing CUDA Rust : Two Tracks for Writing GPU Kernels</a></li>
<li><a href="https://blockchain.news/news/nvidia-cuda-rust-gpu-kernels">NVIDIA Launches CUDA Rust for GPU Kernels... - Blockchain.News</a></li>
<li><a href="https://www.marktechpost.com/2026/09/08/nvidia-announces-cuda-rust-with-cuda-oxide-simt-and-cutile-rs-tile-for-compile-time-safe-gpu-kernels/">NVIDIA Announces CUDA Rust with cuda -oxide... - MarkTechPost</a></li>

</ul>
</details>

**Tags**: `#Rust`, `#CUDA`, `#GPU programming`, `#Nvidia`, `#systems programming`

---

<a id="item-tech-news-2"></a>
### [Micron Shows 512 GB DDR5 RDIMM, Targets 2027 Production](https://videocardz.com/newz/micron-says-worlds-first-512gb-ddr5-module-will-be-production-ready-for-2027) ⭐️ 8.0/10

Micron says it has shown the world&\#x27;s first 512 GB DDR5 RDIMM for servers, with speeds up to 9200 MT/s and expected production readiness in 2027. The module uses 3D-stacked DRAM and can form 12 TB of memory across 24 modules, according to Micron. Micron says a single module consumes 16 W, more than 60% less than the 44.2 W of four 128 GB modules. AMD and Intel are validating it for future server platforms, but the item remains a demonstration and validation-stage product rather than a shipping one.

telegram · zaihuapd · Sep 16, 16:15

**「Background」** DDR5 RDIMMs are registered server memory modules that place a register between the memory controller and the DRAM chips, a design long used in data centers to keep signals stable as module capacity and module counts grow. To reach 512 GB in a single module, Micron uses advanced packaging that stacks multiple DRAM dies vertically and connects them with through-silicon vias \(TSVs\), rather than relying only on conventional die scaling. Server memory capacity and power draw have become pressing constraints as AI and data-center workloads push demand for more memory per system while energy budgets stay fixed.

**「Impact」** For server and AI platform operators, the claimed capacity and power figures could make 512 GB modules attractive for dense 12 TB configurations if AMD and Intel validation and the 2027 production timeline hold.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tomshardware.com/pc-components/dram/micron-announces-512gb-ddr5-9200-memory-modules-with-16w-power-draw-up-to-12tb-per-server-claims-60-percent-less-energy-intensive-than-four-128gb-modules">Micron announces 512 GB DDR 5 -9200 memory ... | Tom&#x27;s Hardware</a></li>
<li><a href="https://www.guru3d.com/story/micron-builds-worlds-first-512gb-ddr5-rdimm-with-9200mt-s-transfer-rate/">Micron Builds Worlds First 512 GB DDR 5 RDIMM With...</a></li>

</ul>
</details>

**Tags**: `#DDR5`, `#服务器内存`, `#美光`, `#3D堆叠DRAM`, `#硬件`

---

<a id="item-tech-news-3"></a>
### [4B Model Claims 81% Faster Query Plans Than Postgres](https://rohanbansal.com/qorl) ⭐️ 7.0/10

A Hacker News-discussed blog post at rohanbansal.com/qorl describes training a 4B-parameter model to generate SQL query plans, with the headline claim that its plans are 81% faster than Postgres on a narrow benchmark. The benchmark conditions reported in discussion include an 8 GB dataset that fits entirely in memory, shared\_buffers constrained below that size, warmed queries, and read-only SELECTs. Commenters also note that tables had no secondary indexes beyond the primary key and no additional statistics, and that correlated columns could affect planning. The Hacker News item drew 380 points and 80 comments, with much of the discussion focused on whether the result generalizes. The supplied evidence does not establish that the 81% figure transfers to larger, write-heavy, or index-rich production workloads.

hackernews · polyphilz · Sep 16, 18:50 · [Discussion](https://news.ycombinator.com/item?id=49731285)

**「Background」** Postgres translates SQL queries into execution plans using table statistics and deterministic transforms, as discussed in the linked Hacker News thread \[tool-1-2\]. The project in question trains a 4B-parameter model to generate query plans, with the reported 81% faster result measured on a narrow in-memory benchmark \[tool-1-1\]. Commenters have questioned whether such a learned planner generalizes beyond that benchmark&\#x27;s specific conditions.

**「Impact」** Database engineers and users evaluating the claim should treat the 81% advantage as benchmark-specific rather than evidence that a 4B model can replace Postgres&\#x27;s planner in production. No supplied evidence shows it generalizes to OLTP, larger datasets, secondary indexes, or richer statistics.

**「Community Discussion」** Commenters broadly questioned overfitting and generalization, pointing to the in-memory 8 GB dataset, constrained shared\_buffers, warmed read-only SELECTs, missing secondary indexes and extra statistics, and correlated columns as reasons the result may not transfer. Some also raised reliability concerns, such as an LLM planner hallucinating and missing an index, while others argued query planning is math- and algorithm-heavy and that an LLM may be a blunt tool compared with neural heuristics or fixing statistics and hints.

<details><summary>References</summary>
<ul>
<li><a href="https://rohanbansal.com/qorl">Training a 4 B model to produce 81 % faster query ... - Rohan Bansal</a></li>
<li><a href="https://news.ycombinator.com/item?id=49731285">Training a 4 B model to produce 81 % faster query plans than ...</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#query optimization`, `#databases`, `#machine learning`, `#benchmarking`

---

<a id="item-tech-news-4"></a>
### [Xiaomi MiMo 2.6 live post-training dashboard draws Hacker News attention](https://mimo.xiaomi.com/rl/) ⭐️ 7.0/10

Xiaomi has published a live post-training dashboard for MiMo 2.6, according to the item, and it drew Hacker News attention for offering unusual transparency into model RL/post-training. The source item provides no additional technical details about the dashboard itself and offers limited technical detail overall. Commenters shared practical experiences with MiMo models: one software engineer praised MiMo-V2.5 for very high ROI, low cost, and quality comparable to Anthropic models they had used in late last year or early this year, while noting occasional hallucination loops that were resolved by stopping and continuing. A commenter cited an unverified benchmark result that MiMo-v2.5-Pro scored 19% on DeepSWE 1.1, versus higher scores for other models, and another said they had spent a week trying Xiaomi&\#x27;s next model, describing it as capable but forgetful and not great at multitasking. Another commenter asked why other model providers do not offer similar dashboards, framing the transparency as notable.

hackernews · krackers · Sep 16, 20:09 · [Discussion](https://news.ycombinator.com/item?id=49732270)

**「Background」** Xiaomi&\#x27;s MiMo family is an AI model line whose post-training stage adapts a pretrained model to downstream tasks, and the new dashboard exposes live reinforcement-learning training metrics for the mimo-v2.6-pro and mimo-v2.6-flash runs directly from the trainer&\#x27;s logs. Post-training can involve scaling across a broad range of agent tasks, so such runs are typically kept internal; publishing them live is what makes this dashboard notable.

**「Impact」** For developers weighing MiMo-v2.6, the dashboard publishes live training metrics from the MiMo-v2.6-pro and MiMo-v2.6-flash reinforcement-learning runs, offering unusually direct visibility into post-training progress; those models are also positioned for use in third-party agents including Cursor, Cline, and Zed. Whether that transparency corresponds to measurable capability gains remains unverified, since the benchmark comparisons raised in the discussion lack confirmation.

**「Community discussion」** Commenters were broadly positive about MiMo models&\#x27; cost and capability, with one engineer calling MiMo-V2.5 very high ROI and another describing Xiaomi&\#x27;s next model as generally capable but forgetful and weak at multitasking. The thread also highlighted unverified benchmark comparisons for MiMo-v2.5-Pro and raised the question of why other model providers do not publish similar live post-training dashboards.

<details><summary>References</summary>
<ul>
<li><a href="https://mimo.xiaomi.com/rl/">mimo-v2.6 RL</a></li>
<li><a href="https://mimo.xiaomi.com/mimo-v2-pro">MiMo-V2-Pro | Xiaomi</a></li>
<li><a href="https://mimo.xiaomi.com/rl/">mimo -v 2 . 6 RL</a></li>
<li><a href="https://github.com/XiaomiMiMo/MiMo-Code">GitHub - XiaomiMiMo/ MiMo -Code: MiMo Code: Where Models and...</a></li>

</ul>
</details>

**Tags**: `#AI models`, `#post-training`, `#open-source AI`, `#Xiaomi MiMo`, `#RL training`

---

<a id="item-tech-news-5"></a>
### [Mistral and Mozilla announce private, multilingual AI browsing collaboration](https://mistral.ai/news/mistral-x-mozilla/) ⭐️ 7.0/10

Mistral and Mozilla announced a collaboration to bring private, multilingual AI features to browsing, according to Mistral&\#x27;s news page. The supplied item does not include the full announcement text, so specific models, deployment details, supported languages, and privacy architecture cannot be verified from the available material. The announcement drew substantial Hacker News attention \(532 points and 186 comments\), with discussion focused on whether inference runs locally or in the cloud, what users must consent to, and how such features could help with non-English developer documentation. Commenters also compared the effort with existing browser AI integrations, including Chrome&\#x27;s built-in Gemini Nano model, while questioning how much trust users can place in cloud-based privacy claims.

hackernews · vertigoruntime · Sep 16, 08:08 · [Discussion](https://news.ycombinator.com/item?id=49723408)

**「Background」** Mozilla and Mistral announced a partnership to bring what they describe as open, private, and multilingual AI to the web browser. Under the arrangement, Mozilla&\#x27;s Firefox Smart Window beta, an AI browsing assistant, is now powered by Mistral models and can help users search, work with information across tabs, and find pages they have visited. The announcement frames the effort around privacy, control, and choice for people using AI while browsing online.

**「Impact」** For Firefox users, this puts Mistral-powered, multilingual AI browsing inside the browser under an explicit privacy-and-choice framing, giving Mozilla an independent-model alternative to rivals that bundle their own AI. Commenters on the announcement, however, note that the marketing materials do not clearly distinguish on-device from cloud inference, so users opting in still cannot tell from these pages alone where their browsing context is processed.

**「Community Discussion」** Commenters were divided: some welcomed private multilingual AI for reading non-English developer docs, while others criticized a cloud-upload model for browsing history and said marketing pages do not clearly distinguish local from cloud inference or consent. Others suggested lightweight local models for query generation and compared the approach to Chrome&\#x27;s built-in Gemini Nano, while noting that privacy-focused cloud inference still requires trust that users cannot easily verify.

<details><summary>References</summary>
<ul>
<li><a href="https://mistral.ai/news/mistral-x-mozilla/">Mistral x Mozilla : Private , Multilingual AI Browsing</a></li>
<li><a href="https://digg.com/tech/a90064fc-f0ba-40a2-97f1-ac972efc5192">Mozilla taps Mistral to power Firefox Smart Window · Digg</a></li>
<li><a href="https://upstract.com/x/a1d4820c4e4f178e">Mistral X Mozilla : Private , Multilingual AI Browsing</a></li>
<li><a href="https://mistral.ai/news/mistral-x-mozilla/">Mistral x Mozilla: Private, Multilingual AI Browsing</a></li>
<li><a href="https://blog.mozilla.org/en/firefox/mozilla-mistral-partnership/">Mozilla and Mistral partner to expand AI competition, user choice | The Mozilla Blog</a></li>
<li><a href="https://news.ycombinator.com/item?id=49723408">Mistral X Mozilla: Private, Multilingual AI Browsing | Hacker News</a></li>

</ul>
</details>

**Tags**: `#AI browsers`, `#privacy`, `#local inference`, `#Mozilla Firefox`, `#Mistral AI`

---

<a id="item-tech-news-6"></a>
### [Hackers Accessed Flock Camera, Exposing Hardcoded Credentials](https://www.wired.com/story/hackers-flock-camera-data-shows-how-system-works/) ⭐️ 7.0/10

A Wired report and a linked technical write-up say hackers gained access to a Flock surveillance camera, exposing hardcoded credentials and broader security weaknesses in the system. The analysis describes a hardcoded API key that could be used to request credentials stored in plaintext, potentially granting access to Flock&\#x27;s servers, though the exact privileges available to an authenticated camera are unclear. The reporting was produced in collaboration with 404 Media, and Distributed Denial of Secrets has published partition images from the device. The episode highlights how hardcoded secrets in Internet-of-Things and public-space surveillance hardware can create security risks.

hackernews · driverdan · Sep 16, 13:18 · [Discussion](https://news.ycombinator.com/item?id=49726586)

**「Background」** Flock Safety is one of the largest vendors of automated license plate reader \(ALPR\) cameras in the United States, with devices installed for police departments, businesses, and homeowners associations. ALPR cameras capture and log vehicle plate data and movements, which is why their security posture matters beyond the individual device. Hardcoded credentials are authentication secrets embedded in firmware that cannot be changed or rotated per unit, so anyone who extracts them can potentially reuse them across an entire fleet; in this case the reporting notes that a hardcoded API key appears usable to obtain credentials for any Flock camera based on its MAC address.

**「Impact」** For agencies and organizations that deploy Flock ALPR cameras in public spaces, the reported hardcoded credentials and extracted software and stored data mean that physical access to a roadside device can expose system credentials and captured data, undermining the security assumptions of those deployments. Reporting does not quantify how many cameras or agencies are affected or what level of backend access such credentials would grant.

**「Community Discussion」** Commenters largely condemned the hardcoded credentials and physical-access threat model, with one calling it a sign of total incompetence and another attributing it to reduced time to market, while noting uncertainty about what a compromised camera could actually do. They also criticized Flock&\#x27;s vulnerability disclosure policy as discouraging real research through carveouts against interacting with devices or downloading data, and warned that the camera&\#x27;s data was accessible and not suitably encrypted.

<details><summary>References</summary>
<ul>
<li><a href="https://micahflee.com/flock-cameras-are-riddled-with-security-vulnerabilities-and-hard-coded-credentials/">Flock cameras are riddled with security vulnerabilities and...</a></li>
<li><a href="https://deflock.org/">Find Nearby ALPRs | DeFlock</a></li>
<li><a href="https://clashreport.com/world/articles/hackers-expose-how-flock-mass-surveillance-works-05q58b65rsj">Hackers Expose How Flock Mass Surveillance Works · Clash Report</a></li>

</ul>
</details>

**Tags**: `#security`, `#IoT`, `#surveillance`, `#embedded systems`, `#vulnerability disclosure`

---

<a id="item-tech-news-7"></a>
### [Anthropic merges Claude Cowork and chat into one Claude](https://simonwillison.net/2026/Sep/16/one-claude/) ⭐️ 7.0/10

Anthropic is merging Claude Cowork and Claude chat into a single Claude, according to the company&\#x27;s announcement that &quot;Claude Cowork and chat are now merging into one Claude.&quot; Anthropic says the combined product is intended to handle both a quick question and a handed-over task such as a report due at noon, continuing the work even after the user has closed their laptop. The change is rolling out to Pro and Max plans first, in the Claude app on web, desktop, and mobile, over the coming weeks for both existing and new users on those plans. Commentator Simon Willison framed the move as Claude becoming a general agent in its own right, noting it echoes OpenAI renaming its Codex desktop app to ChatGPT a few weeks earlier. Willison added that while the consolidation saves him from writing a planned follow-up on the boundaries between Cowork and regular Claude, working out what the change means for features and surfaces will still take considerable effort.

rss · Simon Willison · Sep 16, 18:09

**「Background」** Anthropic had split its assistant into separate surfaces: Claude chat for conversational use, Claude Cowork for longer delegated agentic work, and Claude Code for software development. Merging Cowork into chat leaves Claude with two modes, Chat and Code, and coincides with new in-conversation artifacts such as Claude Docs and Claude Slides. The consolidation mirrors a broader industry pattern of folding specialized agent apps back into general assistants, as OpenAI did by renaming its Codex desktop app to ChatGPT.

**「Impact」** For Pro and Max subscribers on web, desktop, and mobile, the separate Cowork and chat surfaces collapse into one product over the coming weeks, so existing habits and documentation built around distinguishing the two will need to be re-mapped. Anthropic&\#x27;s announcement does not detail how individual features and surfaces will be divided within the merged product.

<details><summary>References</summary>
<ul>
<li><a href="https://claude.com/blog/cowork-is-now-claude">Claude Cowork and chat are now one Claude | Claude by Anthropic</a></li>
<li><a href="https://9to5mac.com/2026/09/16/anthropic-merging-claude-cowork-with-chat/">Anthropic merging Claude Cowork with chat - 9to5Mac</a></li>
<li><a href="https://www.zdnet.com/innovation/claude-chat-absorbs-cowork-anthropic/">Anthropic merges Claude chat and Cowork into one - ZDNET</a></li>

</ul>
</details>

**Tags**: `#AI agents`, `#Anthropic`, `#Claude`, `#product strategy`, `#AI assistants`

---

<a id="item-tech-news-8"></a>
### [TMLR quizzes authors of 10 papers slated for desk rejection](https://www.reddit.com/r/MachineLearning/comments/1wid67h/tmlr_reached_out_to_the_authors_of_10_papers/) ⭐️ 7.0/10

TMLR reached out to the authors of 10 papers slated for desk rejection to ask them to explain the papers they submitted, according to a Reddit r/MachineLearning post summarizing a Medium article by TmlrOrg. The reported outcomes were: one submission was withdrawn; one author said they were unavailable due to other commitments; one scheduled a meeting but did not show up; three were unable to answer basic questions about the paper; three could answer high-level questions but struggled with technical details; and one answered all questions, though the interviewer, the Co-EiC, identified a major flaw in that paper. The episode matters because it raises concerns about peer review, authorship, and possible LLM-generated or paper-mill submissions in machine learning. The Reddit post is a community discussion summarizing the Medium account rather than a primary technical analysis.

reddit · r/MachineLearning · /u/hihey54 · Sep 16, 23:20

**「Background」** TMLR \(Transactions on Machine Learning Research\) is a machine-learning journal that uses OpenReview for submissions and reviewing. It has adopted annual author submission quotas, as many conferences, journals, and funding agencies have done, and its 2025 review cycle accepted 70.6% of reviewed submissions \(46.3% when withdrawals and desk rejections are counted\). The Reddit discussion concerns TMLR&\#x27;s Co-EiC contacting authors of 10 papers that were slated for desk rejection—rejection before full peer review—to ask them to explain their own submissions, amid broader concerns about LLM-generated or paper-mill work.

**「Impact」** The reported outcomes raise concerns for TMLR and the broader ML research community about peer review and authorship integrity, particularly when authors cannot adequately explain their own submissions.

<details><summary>References</summary>
<ul>
<li><a href="https://medium.com/@TmlrOrg/annual-author-submission-quotas-for-tmlr-1db785e51548">Annual Author Submission Quotas for TMLR | by Transactions on Machine Learning Research | Medium</a></li>
<li><a href="https://phdflow.ai/guides/tmlr-explained">TMLR explained: a differently shaped bar, not a lower one</a></li>
<li><a href="https://openreview.net/group?id=TMLR">TMLR | OpenReview</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#peer review`, `#academic integrity`, `#TMLR`, `#LLM-generated papers`

---

<a id="item-tech-news-9"></a>
### [GoBench benchmarks LLMs on 9x9 Go against KataGo](https://www.reddit.com/r/MachineLearning/comments/1wi68jg/gobench_evaluating_llms_on_the_game_of_go_r/) ⭐️ 7.0/10

GoBench is a new open benchmark and leaderboard that evaluates large language models on 9x9 Go games against a ladder of KataGo opponents ranging from random play to superhuman strength. The author reports that GoBench measures general reasoning ability, correlates strongly with ARC-AGI 2 at r=0.83, and remains highly unsaturated. Reported results place GPT-6 Astra max at 2500 Elo, well below the best KataGo at 4400 Elo, while Codex with Astra reaches 3560 Elo when given coding tools and two hours of preparation before evaluation. The author states that the leaderboard will be kept updated as long as it is not saturated, and provides links to the leaderboard, a GitHub code repository, a paper, and a social media post. The results are self-posted and have not been independently verified.

reddit · r/MachineLearning · /u/Roland31415 · Sep 16, 18:54

**「Background」** KataGo is an open-source, self-play-trained Go engine that achieves superhuman play, making it a reference opponent for evaluating Go-playing systems. ARC-AGI is a benchmark introduced by François Chollet in 2019 to measure abstraction and reasoning, so a correlation with ARC-AGI 2 indicates how well Go performance tracks general reasoning ability. GoBench uses an opponent ladder from random to superhuman and reports Elo ratings to express relative playing strength.

**「Impact」** Researchers seeking reasoning evaluations that resist saturation gain a Go-based benchmark reporting a 0.83 correlation with ARC-AGI 2, but the Elo figures and correlation are self-reported in a Reddit post and should be treated as unverified until reproduced.

<details><summary>References</summary>
<ul>
<li><a href="https://arcprize.org/arc-agi">ARC Prize - The only AI benchmark that measures AGI progress.</a></li>
<li><a href="https://www.stork.ai/en/katago">KataGo Review (2026): Pricing &amp; Alternatives | Stork. AI</a></li>

</ul>
</details>

**Tags**: `#LLM evaluation`, `#Go`, `#reasoning benchmarks`, `#KataGo`, `#AI research`

---

<a id="item-tech-news-10"></a>
### [Cloudflare adds per-domain setting to block AI training while keeping search indexing](https://blog.cloudflare.com/accountable-mixed-use-ai-crawlers/) ⭐️ 7.0/10

Cloudflare announced on September 15 a new &quot;block AI training&quot; setting that lets websites remain indexed by search engines while blocking training crawlers that do not meet its requirements. Apple, Google, and Microsoft have either complied or committed to comply with those requirements. The setting is configured per domain; choosing &quot;block&quot; blocks all crawlers, including mixed crawlers, which also affects search indexing. Cloudflare plans early next year to let sites control the proportion of their content that can be referenced in AI summaries.

telegram · zaihuapd · Sep 16, 05:46

**「Background」** Cloudflare is a widely used content delivery network, DNS provider, and reverse proxy, so its crawler policies can affect how bots reach a large share of websites. Sites have traditionally relied on robots.txt and user-agent rules to separate search crawlers from other bots, but AI training crawlers—and mixed crawlers that also serve search indexing—are harder to distinguish; Google-Extended is an existing Google control for opting out of AI training while keeping search inclusion. The new setting is an attempt to give site owners a domain-level way to block non-compliant AI training crawlers while allowing accountable or search-related crawlers to continue.

**「Impact」** For site operators on Cloudflare, the per-domain &quot;block AI training&quot; setting allows blocking non-compliant training crawlers while keeping search indexing, but selecting &quot;block&quot; also intercepts mixed crawlers that combine search and training, which affects search inclusion as well. Cloudflare says it plans to let sites control the share of their content cited in AI summaries starting early next year, so the practical effect on AI-referred traffic is not yet demonstrated.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bannedbook.org/bnews/itnews/20260916/2360152.html">Cloudflare 推出设置：可保留搜索收录并禁止 AI 训练 - 禁闻网</a></li>
<li><a href="https://k.sina.cn/article_1826017320_6cd6d02802001wxju.html">Cloudflare推出新设置：可允许搜索引擎爬取，同时拒绝AI训练|rain|it之家|爬虫|谷歌|微软_新浪新闻</a></li>
<li><a href="https://www.ithome.com/1/003/108.htm">Cloudflare 推出新设置：可允许搜索引擎爬取，同时拒绝 AI 训练 - IT之家</a></li>
<li><a href="https://blog.cloudflare.com/content-independence-day-ai-options/">Your site, your rules: new AI traffic options for all customers | Cloudflare Blog</a></li>
<li><a href="https://www.cloudflare.com/press/press-releases/2025/cloudflare-just-changed-how-ai-crawlers-scrape-the-internet-at-large/">Cloudflare Just Changed How AI Crawlers Scrape the Internet-at-Large; Permission-Based Approach Makes Way for A New Business Model | Cloudflare</a></li>

</ul>
</details>

**Tags**: `#Cloudflare`, `#AI爬虫`, `#搜索收录`, `#AI训练数据`, `#网络基础设施`

---

<a id="item-tech-news-11"></a>
### [Chinese-language casino sites hide APT malware C2 infrastructure](https://www.theregister.com/security/2026/09/15/low-quality-casino-sites-conceal-highly-dangerous-threat-actors/5296652) ⭐️ 7.0/10

A security report says many low-quality Chinese-language gambling and adult websites are being used as covert cyberattack infrastructure rather than ordinary entertainment sites. The company tracked roughly 1.7 million Chinese casino websites, some of which were used for malware distribution and espionage. Since 2023, a China-linked APT group has used a framework called &quot;PeckBirdy&quot; to hide malware command-and-control domains inside these low-quality gambling sites and to trick users into downloading malicious programs through fake software updates. Because the sites closely resemble ordinary gambling sites, security staff can easily mistake related traffic for employee policy violations and overlook it.

telegram · zaihuapd · Sep 16, 07:31

**「Background」** China-aligned advanced persistent threat \(APT\) groups have used low-quality Chinese-language casino and adult sites to conceal command-and-control \(C2\) infrastructure linked to the PeckBirdy malware framework \(tool-1-1\). PeckBirdy is a JScript-based C2 framework used by China-aligned APT actors since 2023 and designed to execute across multiple environments, making deployment flexible \(tool-1-2, tool-1-3\). Security researchers at Infoblox warned that roughly 1.7 million illegal gambling pages serve as cover for espionage and malware attacks \(tool-2-3\), while a subset of casino sites also offers scam gambling, or &quot;scambling,&quot; in which visitors place bets but cannot withdraw winnings if they win \(tool-2-1\).

**「Impact」** For security teams monitoring employee traffic, the finding means malicious command-and-control activity can be misclassified as policy violations, potentially delaying detection and response.

<details><summary>References</summary>
<ul>
<li><a href="https://cyberpress.org/peckbirdy-hides-in-casinos/">PeckBirdy Malware Uses Chinese Casino and Adult Websites to Hide...</a></li>
<li><a href="https://www.trendaisecurity.com/en-gb/resources-insights/trendai-security-blog/peckbirdy-script-framework">PeckBirdy : A Versatile Script Framework for LOLBins Exploitation...</a></li>
<li><a href="https://thehackernews.com/2026/01/china-linked-hackers-have-used.html">China -Linked Hackers Have Used the PeckBirdy JavaScript...</a></li>
<li><a href="https://www.theregister.com/security/2026/09/15/low-quality-casino-sites-conceal-highly-dangerous-threat-actors/5296652">Low - quality casino sites conceal highly dangerous threat actors</a></li>
<li><a href="https://lustich.de/news/low-quality-casino-sites-conceal-highly-dangerous-threat-actors">Gefährliche Schadsoftware hinter illegalen Casino -Webseiten entdeckt</a></li>

</ul>
</details>

**Tags**: `#cybersecurity`, `#APT`, `#malware C2`, `#threat intelligence`, `#Chinese-language gambling sites`

---

<a id="item-tech-news-12"></a>
### [Sina Cloud SAE Shutdown Threatens 420 TB of Early Bilibili Video Data](https://tracker.archiveteam.org/sinavideo/#show-all) ⭐️ 7.0/10

Sina Cloud SAE, described as China&\#x27;s first PaaS cloud platform, is reported to be permanently shutting down with all user data deleted; the source says the deadline is 24:00 on September 16, 2026, and frames it as imminent. Launched in 2009, SAE became popular with developers for its low cost and maintenance-free operation. Early Bilibili depended on Sina Cloud to store large volumes of video source files, and about 420 TB of historical data reportedly remains in Sina Cloud S3 buckets. Archive Team&\#x27;s distributed archiving project has cumulatively rescued about 680 TB of data and reports 96.26% completion, according to the tracker. The shutdown therefore threatens the remaining early Bilibili source material while the archiving effort continues.

telegram · zaihuapd · Sep 16, 15:00

**「Background」** Sina Cloud SAE \(Sina App Engine\) launched in 2009 and was described as China&\#x27;s first PaaS cloud-computing platform, offering distributed web application hosting and runtime services. Early Bilibili relied on SAE to store its video source files, leaving roughly 420 TB of historical data in SAE S3 buckets. Archive Team, the volunteer digital-preservation group behind the current rescue, runs distributed archiving projects to save at-risk online data.

**「Impact」** Developers holding data on Sina Cloud SAE face permanent loss of all user data once the platform&\#x27;s scheduled shutdown completes on 16 September 2026, and roughly 420 TB of early Bilibili video source files still sitting in Sina Cloud S3 buckets remain at risk unless the current archiving push closes the remaining gap — the Archive Team tracker reports 96.26% completion after about 680 TB recovered. These figures come from a Telegram-aggregated report and the Archive Team tracker rather than primary technical documentation, so the final preservation outcome is not yet confirmed.

<details><summary>References</summary>
<ul>
<li><a href="https://www.sinacloud.com/sae.html">云 应用 SAE - 云 服务 - 云 托管</a></li>

</ul>
</details>

**Tags**: `#cloud computing`, `#data preservation`, `#Archive Team`, `#Sina Cloud SAE`, `#Bilibili`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Fed raises rates for the first time in over three years, signals another hike possible this year](https://www.cnbc.com/2026/09/16/fed-rate-decision-september-2026.html) ⭐️ 9.0/10

The Federal Reserve raised its key interest rate by 25 basis points \(a quarter percentage point\) to a target range of 3.75%–4%, its first increase since July 2023, in a unanimous 12-0 vote. Updated Fed projections indicated that 16 of 18 officials expected at least one more increase later this year, with four of those seeing two more, while the Fed also nudged up its 2026 inflation forecasts to 3.7% for headline PCE prices and 3.4% for core prices.

rss · CNBC Finance · Sep 16, 21:07

**「Background」** The Fed had held its benchmark federal funds rate — the overnight rate banks charge each other, which feeds into other borrowing costs — at 3.50%–3.75% all year, and its previous increase was in July 2023; it aims for 2% annual inflation, as measured by the personal consumption expenditures price index. Kevin Warsh, who became Fed chair in 2026, has chosen not to submit a rate projection at meetings, though 16 of the other 18 participants expected another increase.

**「Who feels it」** Higher rates feed directly into borrowing costs that are tied to the Fed&\#x27;s benchmark, so households taking out mortgages or carrying credit-card and auto debt, and businesses rolling over loans, face pricier financing — housing analysts noted mortgage rates were already at their highest level in more than a year before the decision, per Fitch Ratings.

<details><summary>References</summary>
<ul>
<li><a href="https://simple.wikipedia.org/wiki/Kevin_Warsh">Kevin Warsh - Simple English Wikipedia, the free encyclopedia</a></li>
<li><a href="https://edition.cnn.com/2026/09/16/business/live-news/federal-reserve-interest-rate-september">Fed raises interest rates for the first time since 2023 | CNN Business</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#Interest Rates`, `#Monetary Policy`, `#Inflation`, `#FOMC`

---

<a id="item-finance-news-2"></a>
### [Hong Kong announces 11 measures to encourage childbirth](https://www.info.gov.hk/gia/general/202609/16/P2026091600265.htm) ⭐️ 7.0/10

Hong Kong&\#x27;s Chief Executive John Lee announced 11 measures in his new Policy Address to encourage childbirth, saying the government is shifting from a non-interventionist stance to a pro-natal one. The package extends the HK$20,000 newborn baby bonus for three years and raises it to HK$30,000 for a second or later child born from today, while the tax allowance for second and subsequent children rises to HK$160,000 from HK$140,000 starting in the 2026/27 tax year.

telegram · zaihuapd · Sep 16, 08:01

**「Background」** The measures came in Hong Kong&\#x27;s 2026 Policy Address, delivered by Chief Executive John Lee on 16 September; the government said it was changing its past non-interventionist stance, and the HK$20,000 newborn bonus it extended had been due to expire on 24 October.

**「Impact」** Families planning a second or later child, and subsidised-housing applicants with a newborn, are the main beneficiaries, since the higher baby bonus, stamp duty relief and raised mortgage ceiling lower upfront costs; commentary cited alongside the coverage argues financial incentives alone may not change childbearing decisions in a city it describes as having one of the world&\#x27;s lowest birth rates.

<details><summary>References</summary>
<ul>
<li><a href="https://news.ifeng.com/c/8wT4qi5kBpU">2万港元新生婴儿奖励金计划延续3年……香港推11项鼓励生育措施_凤凰网</a></li>
<li><a href="https://www.zaobao.com.sg/news/china/story20260916-9684664">香港施政报告加码催生 | 联合早报</a></li>
<li><a href="https://h5.ifeng.com/c/vivoArticle/v002leYk281--pBRDxcsIcLUjR0tndmXHLMihreMj8jqIehQ__?isNews=1&amp;showComments=0">家庭月入三万不敢 生 娃？ 香 港 生 育 率 全球最低</a></li>

</ul>
</details>

**Tags**: `#Hong Kong`, `#fertility policy`, `#fiscal incentives`, `#tax allowances`, `#housing policy`

---

<a id="item-finance-news-3"></a>
### [China Opens Pinglu Canal, a New Southwest-to-ASEAN Shipping Route](https://www.news.cn/politics/20260916/4d3b671357d14c8db202cbf6120f2c43/c.html) ⭐️ 7.0/10

The Pinglu Canal, a 134.2-kilometre waterway built for more than 70 billion yuan and able to handle 5,000-tonne vessels, has opened to navigation, according to Xinhua, with two direct river-sea services beginning on the same day: Nanning Port to Vietnam&\#x27;s Can Tho Port and Nanning Port to Yangpu Port. Xinhua reports that cargo from southwest China now travels more than 560 kilometres less than on traditional routes, cutting logistics costs by 18% to 30%.

telegram · zaihuapd · Sep 16, 09:10

**「Background」** The canal is a backbone project of China&\#x27;s New International Land-Sea Trade Corridor, an effort to give the landlocked southwest a shorter water route to Southeast Asian markets. Construction began in August 2022, and state media describe it as the country&\#x27;s first &quot;river-to-sea&quot; canal since the founding of the People&\#x27;s Republic — meaning ships can travel directly between inland river ports and the sea without unloading.

**「Who stands to gain」** Businesses moving bulk and container freight between southwest China and Southeast Asia are the immediate beneficiaries: the chairman of Hunan Huaihua International Land Port, Yang Fanglai, says bulk-cargo logistics costs are expected to fall 18%–30% and container unit costs 18%–22%, and one estimate cited by China News Service puts annual savings to the wider economy at more than 5 billion yuan \(50亿元人民币\).

<details><summary>References</summary>
<ul>
<li><a href="https://news.cyol.com/gb/articles/2026-06/04/content_BbNGmOTlYQ.html">通 江达 海 西 部 陆 海 新 通 道 跑出高水 平 对外开放“加速度”</a></li>
<li><a href="https://www.ddgx.cn/show/59283.html">当代广 西 网 -- 读懂 平 陆 运 河 的重大 战 略 意 义</a></li>
<li><a href="https://www.chinanews.com.cn/aseaninfo/2026/09-16/10697442.shtml">一河通江海 平陆运河铺就中国—东盟经贸合作“水上高速路”-中新网</a></li>
<li><a href="https://www.sohu.com/a/1076477959_121443915">东西问丨余虹：平陆运河通航将如何重构中国—东盟经贸格局？_广西_产业链_物流</a></li>

</ul>
</details>

**Tags**: `#平陆运河`, `#基础设施投资`, `#中国-东盟贸易`, `#物流成本`, `#区域经济`

---