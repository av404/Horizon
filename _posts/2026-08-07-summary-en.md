---
layout: default
title: "Horizon Summary: 2026-08-07 (EN)"
date: 2026-08-07
lang: en
---

> From 38 items, 19 important content pieces were selected

---

**Technology News**
1. [DeepSeek V4 Flash 0731: Faster, Cheaper, But Tool-Call Loops Reported](#item-tech-news-1) ⭐️ 8.0/10
2. [Rust Engine Makes Postgres Hundreds of Times Faster for Analytics](#item-tech-news-2) ⭐️ 8.0/10
3. [Cloudflare unveils Kitesurf, an agent-first V8-isolate browser](#item-tech-news-3) ⭐️ 8.0/10
4. [Fighting Bots on a 1.5M-Page Site: A Year of Defense](#item-tech-news-4) ⭐️ 8.0/10
5. [US Probes Chinese AI Firms&\#x27; Offshore Access to Nvidia Chips](#item-tech-news-5) ⭐️ 8.0/10
6. [2027 Memory Capacity Reportedly Sold Out Amid AI HBM Demand](#item-tech-news-6) ⭐️ 7.0/10
7. [New Mexico Court Orders Meta to Pay $567M for Children’s Mental Health](#item-tech-news-7) ⭐️ 7.0/10
8. [Moonlight &amp; Mayhem: Codex with GPT-5.6 Sol Ultra Beats Claude Fable 5 on Same Prompt](#item-tech-news-8) ⭐️ 7.0/10
9. [SpaceX 10GW in 2027: $300B ARR and Microsoft as Top Offtaker](#item-tech-news-9) ⭐️ 7.0/10
10. [Gemini Struggles While GCP Gains, Says Analysis](#item-tech-news-10) ⭐️ 7.0/10
11. [sub2api OAuth flaw allows account takeover with only an email](#item-tech-news-11) ⭐️ 7.0/10
12. [AWS Cracks Down on Internal CPU Waste as Agentic AI Raises Demand](#item-tech-news-12) ⭐️ 7.0/10
13. [OpenAI Says Astra May Reach Critical Cyber Capability Threshold, Delays Possible](#item-tech-news-13) ⭐️ 7.0/10

**Financial News**
1. [Fed September rate hike odds tumble after weak July jobs report](#item-finance-news-1) ⭐️ 8.0/10
2. [SEC approves Nasdaq 23-hour trading, starting December 6, 2026](#item-finance-news-2) ⭐️ 8.0/10
3. [Chevrolet Exits China New-Car Market After 21 Years](#item-finance-news-3) ⭐️ 8.0/10
4. [Beijing cuts social-security requirement for homebuyers without Beijing hukou to 1 year](#item-finance-news-4) ⭐️ 8.0/10
5. [Trump signs executive orders targeting birthright citizenship and birth tourism](#item-finance-news-5) ⭐️ 7.0/10
6. [Australia proposes A$31.30/hour minimum pay for food delivery riders](#item-finance-news-6) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [DeepSeek V4 Flash 0731: Faster, Cheaper, But Tool-Call Loops Reported](https://arcprize.org/results/deepseek-v4-flash-0731) ⭐️ 8.0/10

DeepSeek V4 Flash 0731 is an updated model release presented on the ARC Prize results page, with significant speed and capability improvements over the earlier DSv4 Flash preview. Community users report that it is good enough for nearly all coding and document-analysis work and cheap enough that costs are almost irrelevant, with one user spending under $5 per day across 5-6 active sessions on the Oh My Pi platform. Local inference on 2x RTX Pro 6000 Blackwell reportedly reaches about 8k tokens/s prefill and roughly 250 tokens/s on a single generation stream. The same users note that this 07/31 release feels like a whole tier above the previous preview, but some report problematic behaviors such as infinite loops and tool calls not being executed.

hackernews · tosh · Aug 7, 17:56 · [Discussion](https://news.ycombinator.com/item?id=49214008)

**「Background」** DeepSeek V4 Flash is a lightweight, low-cost large language model from DeepSeek, and the 0731 release on July 31, 2026 is an updated version after an earlier preview. The ARC-AGI benchmark suite, run by the ARC Prize Foundation, tests AI systems on novel reasoning tasks that are meant to measure general fluid intelligence rather than memorized knowledge. On this release, DeepSeek reports 89.0% on ARC-AGI-1 Semi-Private and 61.4% on ARC-AGI-2 Semi-Private, at a cost of roughly $0.02 to $0.04 per task across its Max, High, and Low reasoning variants.

**「Impact」** The release gives developers a fast, cheap local model for coding and document-analysis tasks, though agent users on the Pi framework report token-wasting infinite loops and tool-call failures.

**「Community Discussion」** Commenters are broadly enthusiastic about the model&\#x27;s speed, cost, and capability, with one calling it a whole tier up from the preview. However, at least one user reports serious reliability issues in agent mode, including infinite loops and self-dialogue without executing tool calls, wasting significant tokens.

<details><summary>References</summary>
<ul>
<li><a href="https://arcprize.org/results/deepseek-v4-flash-0731">DeepSeek V4 Flash 0731 - ARC-AGI Results</a></li>
<li><a href="https://zeli.app/en/story/49214008">DeepSeek V4 Flash 0731 Hits 89% on ARC-AGI-1, 61.4% on ARC ...</a></li>
<li><a href="https://elsolitario.org/en/2026/08/07/deepseek-v4-flash-arc-agi-results/">DeepSeek V4 Flash: 89% ARC-AGI-1, 61.4% ARC-AGI-2</a></li>

</ul>
</details>

**Tags**: `#deepseek`, `#llm`, `#machine-learning`, `#ai-models`, `#arc-prize`

---

<a id="item-tech-news-2"></a>
### [Rust Engine Makes Postgres Hundreds of Times Faster for Analytics](https://malisper.me/how-we-made-postgres-hundreds-of-times-faster-the-query-engine/) ⭐️ 8.0/10

The article describes pgrust, a Rust-based Postgres query engine that reportedly achieves hundreds-of-times speedups for analytical workloads by using batching, operator fusion, and SIMD. The author states that correctness is the top priority and mentions verifying over 1,000 user-facing functions through formal verification and differential fuzz testing over the past two weeks, with proofs available in a dedicated directory. The project also appears to involve adaptive planning, a feature the author argues has been well-established in other production databases but resisted by the Postgres core team. While performance gains are promising, adoption concerns remain because pgrust is not developed by the trusted Postgres core team.

hackernews · poly2it · Aug 7, 11:00 · [Discussion](https://news.ycombinator.com/item?id=49208535)

**「Background」** Postgres’s original query engine processes rows one at a time, which adds significant overhead for analytical workloads. pgrust is a Rust-based query engine for Postgres that aims to replace this row-by-row execution with batch processing, operator fusion, and SIMD instructions to speed up analytics. Its 0.2 release focused on performance, claiming to be 10 times faster than the previous version and hundreds of times faster than stock Postgres for some queries.

**「Impact」** For Postgres users running analytics workloads, the project demonstrates a credible technical path to dramatic speedups, though broad production adoption is likely to be limited by trust in a non-core-team engine and by the need for continued correctness assurance.

**「Community Discussion」** Commenters welcomed the project&\#x27;s technical direction, especially adaptive planning, but expressed realistic concerns about adoption: some argued users will not choose pgrust over Postgres for trust and longevity reasons, while others asked for more detail on IO scheduling and thread management to address noisy-neighbor problems. A separate comment suggested running Postgres on ramfs/tmpfs as an alternative performance trick.

<details><summary>References</summary>
<ul>
<li><a href="https://malisper.me/how-we-made-postgres-hundreds-of-times-faster-the-query-engine/">Rebuilding Postgres for 300x faster analytics: batching ...</a></li>
<li><a href="https://byteiota.com/pgrust-hits-300x-faster-postgres-analytics-heres-how/">pgrust Hits 300x Faster Postgres Analytics — Here’s How</a></li>
<li><a href="https://newsscore.com/story/181545">Pgrust 0.2 released; query engine rebuild makes Postgres ...</a></li>

</ul>
</details>

**Tags**: `#postgres`, `#query-optimization`, `#simd`, `#rust`, `#database-systems`

---

<a id="item-tech-news-3"></a>
### [Cloudflare unveils Kitesurf, an agent-first V8-isolate browser](https://blog.cloudflare.com/kitesurf/) ⭐️ 8.0/10

Cloudflare has introduced Kitesurf, an agent-first browser that runs in V8 isolates and targets efficient browser automation for AI agents on its edge network. It is built on Blitz, a modular open-source browser engine, and the Blitz maintainer says Cloudflare intends to open-source and upstream its patches. The design aims to reduce the overhead of running full browser instances by using lightweight isolates, though no performance details, benchmarks, or compatibility constraints have been shared. The announcement adds to Cloudflare&\#x27;s broader push toward agent-friendly infrastructure, but concrete availability, pricing, and limitations remain unspecified.

hackernews · m3h · Aug 7, 10:42 · [Discussion](https://news.ycombinator.com/item?id=49208393)

**「Background」** Browser automation for AI agents has conventionally meant driving full browsers such as Chromium, which are optimized for humans and therefore memory- and compute-intensive. Cloudflare Workers execute JavaScript in V8 isolates, lightweight sandboxed execution environments, and Cloudflare is applying that model to browsers: Kitesurf is a stateless browser built on a Rust/Wasm engine, with no Chromium underneath, and is reported to use 3-7x less memory and CPU than Chromium while having slower wall-clock performance. It is designed to run entirely on Workers as part of Cloudflare&\#x27;s Agentic Cloud platform.

**「Community Discussion」** Commenters welcomed the connection to the open-source Blitz engine and the plan to upstream patches, but several questioned Cloudflare&\#x27;s dual role as CDN/security provider and agent-browser operator. They specifically asked whether Kitesurf browser instances would bypass Cloudflare&\#x27;s own anti-bot mechanisms, and one commenter doubted the real-world appeal of browser-based shopping agents. Another user made a lighthearted joke comparing the name to kitesurfing trends.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.cloudflare.com/kitesurf/">Introducing Kitesurf: The agent-first browser that runs in V8 ...</a></li>
<li><a href="https://www.explainx.ai/blog/cloudflare-kitesurf-agent-browser-v8-isolates-august-2026">Cloudflare Kitesurf: The Agent-First Browser Running in V8 ...</a></li>

</ul>
</details>

**Tags**: `#browser`, `#cloudflare`, `#AI agents`, `#browser automation`, `#V8 isolates`

---

<a id="item-tech-news-4"></a>
### [Fighting Bots on a 1.5M-Page Site: A Year of Defense](https://patronview.com/news/99-percent-of-my-website-traffic-is-bots/) ⭐️ 8.0/10

A webmaster published an account of spending a year defending a 1.5-million-page website from scrapers and other bot traffic. The report details the mitigation tools used and the operating costs involved, including a normal monthly bill of around $90 that jumped roughly 500% during one bad spike month. It also discusses how bot defenses can become a bottleneck for humans and raises broader concerns about the open web. The account highlights the practical trade-offs of using third-party bot mitigation services and database choices such as D1.

hackernews · petercooper · Aug 7, 14:51 · [Discussion](https://news.ycombinator.com/item?id=49211386)

**「Background」** Many websites now receive large amounts of automated traffic from search engine crawlers, AI model trainers, and scraper services. Site owners often need to distinguish legitimate visitors from bots, using techniques ranging from proof-of-work challenges to managed reverse-proxy and bot-management services such as Cloudflare. The challenge is that aggressive bot filtering can also block real users and concentrate access decisions in a few large companies.

**「Impact」** For site owners facing high volumes of bot requests, the report’s evidence shows both the financial risk of unexpected bill spikes and the practical appeal of tools like Anubis for sites not behind a major proxy. The concern voiced by readers is that using Cloudflare-style services outsources who can access a site to a single company, which may have hidden consequences for openness.

**「Community Discussion」** Commenters were split on the trade-offs: some praised Anubis as a superb proof-of-work fix for sites not behind Cloudflare, Fastly, or Bunny, while others warned about relying on Cloudflare as a gatekeeper. One operator reported that Claude-searchbot alone fetched about 205,000 pages from their site in 72 hours and sent just one referral, and the author acknowledged the irony that their own site also scrapes public documents.

**Tags**: `#web scraping`, `#bot detection`, `#cloudflare`, `#AI crawlers`, `#open web`

---

<a id="item-tech-news-5"></a>
### [US Probes Chinese AI Firms&\#x27; Offshore Access to Nvidia Chips](https://www.bloomberg.com/news/articles/2026-08-07/us-reviews-china-s-offshore-access-to-nvidia-chips-after-ai-breakthroughs) ⭐️ 8.0/10

The U.S. Commerce Department&\#x27;s Bureau of Industry and Security \(BIS\) is systematically reviewing how Chinese AI companies obtain and use Nvidia chips overseas, including through remote cloud rentals in other countries. The review includes compiling two country lists: locations of black markets suspected of smuggling restricted chips into China, and countries where Chinese firms remotely rent chips. The probe follows the release last month of Moonshot AI&\#x27;s Kimi K3 model, which approached U.S. peers in performance, and a White House official&\#x27;s public accusation that the company illegally obtained Nvidia chips and accessed them remotely via Thailand. BIS enforcement launched its investigation days after that accusation, though remote access itself is not currently illegal and BIS authority over such cloud agreements is uncertain. The House has passed a bipartisan bill to explicitly grant that authority, but it faces expected opposition from Nvidia and other tech companies; Bloomberg also reported that Alibaba, through a Singapore shell company controlled by a Cayman entity, used Nvidia chips in Malaysia via Megaspeed, which is under U.S. investigation.

telegram · zaihuapd · Aug 7, 11:18

**「Background」** U.S. export controls restrict advanced Nvidia AI chips from reaching China, but the rules are less clear for Chinese companies that remotely rent computing power in other countries; export-control lawyers note that remote access to controlled technology can itself be treated as an export. The current investigation examines Singapore-based Megaspeed, a Nvidia customer under police investigation for allegedly helping Chinese firms evade U.S. restrictions, and Moonshot AI, whose Kimi K 3 model the White House has accused of being built with restricted Nvidia chips and of distilling Anthropic&\#x27;s Claude models. Malaysia has since introduced permit requirements for transfers of Nvidia chips as part of broader oversight.

**「Impact」** Chinese AI developers and cloud providers now face heightened risk of export-control enforcement against offshore chip access and intermediary arrangements, which could disrupt their access to advanced Nvidia hardware and reshape international cloud-computing practices.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nytimes.com/2025/10/09/technology/nvidia-chips-china-megaspeed.html">A Mystery C.E.O. and Billions in Sales: Is China Buying Banned Nvidia ...</a></li>
<li><a href="https://www.cryptopolitan.com/nvidia-megaspeed-investigated-in-singapore/">Nvidia client Megaspeed investigated in Singapore for export ...</a></li>
<li><a href="https://distillation.technology/newsroom/white-house-accuses-moonshot">White House accuses Moonshot AI of distilling Anthropic’s</a></li>
<li><a href="https://www.freshfields.com/en/our-thinking/blogs/a-fresh-take/remote-access-or-remote-possibility-rasa-and-the-future-of-cloud-export-controls-102nfbw">Remote Access or Remote Possibility? RASA and the... | Freshfields</a></li>

</ul>
</details>

**Tags**: `#AI`, `#US-China`, `#Nvidia`, `#export-controls`, `#cloud-computing`

---

<a id="item-tech-news-6"></a>
### [2027 Memory Capacity Reportedly Sold Out Amid AI HBM Demand](https://www.ign.com/articles/ramageddon-continues-another-year-as-2027-memory-capacity-is-reportedly-sold-out) ⭐️ 7.0/10

Reports indicate that memory capacity for 2027 is already sold out, driven by surging AI demand for high-bandwidth memory \(HBM\), signaling an extended memory shortage. HBM production imposes a significant wafer trade-off: HBM3E consumes approximately three times the wafer supply of DDR5 to produce a given number of bits at the same technology node, which constrains supply for non-HBM products. This dynamic is expected to keep pressure on memory availability and pricing for both datacenter and consumer markets. The report relies on industry sources, so the exact scale and timing remain uncertain.

hackernews · inigyou · Aug 7, 07:58 · [Discussion](https://news.ycombinator.com/item?id=49207236)

**「Context」** Dynamic random-access memory \(DRAM\) and high-bandwidth memory \(HBM\) are critical components in computers and AI accelerators; HBM is a specialized, high-speed memory stacked vertically for use in AI processors. Industry memory suppliers Samsung, SK hynix, and Micron have reportedly sold out their 2027 DRAM and HBM production capacity, with NAND capacity also tightening, driven by AI demand growing faster than new capacity can be added.

**「Impact」** With 2027 memory capacity reportedly sold out, consumers and enterprises should expect continued tight supply and higher prices for commodity DRAM, laptops, phones, and servers as manufacturers prioritize High-Bandwidth Memory \(HBM\) for AI applications. Industry analyses already point to price hikes and delays for consumer RAM as wafer capacity is reallocated away from standard DRAM to HBM, and the 2027 sellout indicates this pressure will persist well beyond the current cycle.

**「Community Discussion」** Commenters emphasized the wafer capacity trade-off between HBM and conventional DRAM, noting that HBM dies are larger and that ramping HBM production will limit growth in non-HBM memory supply. Several expressed practical concern and frustration, including a microcontroller developer&\#x27;s urge to stockpile RAM, a wish for a universal RAM standard to reuse old sticks, and a buyer who suspected a cancelled DDR4 order was due to the vendor wanting to raise prices.

<details><summary>References</summary>
<ul>
<li><a href="https://www.iclarified.com/101675/global-dram-production-sold-out-through-2027-as-ai-demand-tightens-supply">Global DRAM Production Sold Out Through 2027 as AI Demand ...</a></li>
<li><a href="https://www.tweaktown.com/news/113004/memory-capacity-for-all-of-2027-has-reportedly-been-booked-and-sold-with-no-more-dram-or-hbm-available/index.html">Memory capacity for all of 2027 has reportedly been booked ...</a></li>
<li><a href="https://www.ibselectronics.com/resources/news/memory-supply-tightens-beyond-2027-as-ai-demand-reshapes-dram,-nand-and-hbm-markets/">Memory Supply Tightens Beyond 2027 as AI Demand Reshapes DRAM ...</a></li>
<li><a href="https://www.geeky-gadgets.com/ram-prices-2026/">RAM Shortage 2026: HBM Demand Drives Higher Prices &amp; Delays ...</a></li>
<li><a href="https://bisi.org.uk/reports/global-ram-shortage-and-price-hikes-causes-consequences-and-market-outlook">Global RAM Shortage and Price Hikes: Causes, Consequences ...</a></li>
<li><a href="https://supplyics.com/insights/market-intelligence/2026-hbm-dram-memory-supply-chain-analysis/">2026 HBM and DRAM Supply Chain Analysis: Navigating AI-Driven ...</a></li>

</ul>
</details>

**Tags**: `#memory`, `#hardware`, `#HBM`, `#supply chain`, `#AI`

---

<a id="item-tech-news-7"></a>
### [New Mexico Court Orders Meta to Pay $567M for Children’s Mental Health](https://www.theguardian.com/technology/2026/aug/06/new-mexico-court-meta) ⭐️ 7.0/10

A New Mexico court ordered Meta on August 6, 2026 to pay $567 million and change how it handles underage users after finding the company liable for harming children’s mental health through social media. The decision is based on the state’s public-nuisance law and adds to growing legal scrutiny over teen safety on platforms like Instagram. Coverage of the award varies: most linked reports cite $567 million, while The Wall Street Journal’s headline cites $942 million. Because New Mexico has roughly 2 million residents, the judgment represents a large per-capita penalty even though it is small relative to Meta’s global revenue.

hackernews · boplicity · Aug 7, 00:06 · [Discussion](https://news.ycombinator.com/item?id=49204352)

**「Background」** New Mexico sued Meta, the parent company of Facebook and Instagram, alleging its platforms harmed young users&\#x27; mental health and constituted a public nuisance under state law. In August 2026, a New Mexico state court ordered Meta to pay $567 million into a teen mental health fund and to change how its platforms function for young users. The case relied on New Mexico&\#x27;s public-nuisance statute, which addresses conduct injurious to public health, safety, morals, or welfare.

**「Impact」** The ruling creates concrete state-level financial liability for Meta and pressures the company to redesign safety protections for minors, while also strengthening the use of public-nuisance claims against online platforms for alleged harm to children.

**「Community Discussion」** Commenters generally acknowledged that the sum is a small fraction of Meta’s revenue but stressed that roughly $942 million in a state of about 2 million people is enormous. Several also criticized Instagram Reels and TikTok as addictive, questioned whether any fine would be more than “cost of doing business,” and noted potential stock-price and global-regulatory risks.

<details><summary>References</summary>
<ul>
<li><a href="https://www.theguardian.com/technology/2026/aug/06/new-mexico-court-meta">New Mexico court orders Meta to pay $567m over harms to ...</a></li>
<li><a href="https://www.cbsnews.com/news/meta-instagram-new-mexico-court-kids-mental-health/">New Mexico court orders Meta and Instagram to pay $567M to ...</a></li>
<li><a href="https://www.usnews.com/news/top-news/articles/2026-08-06/new-mexico-court-orders-meta-to-pay-567-million-for-teen-mental-health-fund">New Mexico Court Orders Meta to Pay $567 Million for Teen ...</a></li>

</ul>
</details>

**Tags**: `#Meta`, `#technology regulation`, `#child safety`, `#social media`, `#legal`

---

<a id="item-tech-news-8"></a>
### [Moonlight &amp; Mayhem: Codex with GPT-5.6 Sol Ultra Beats Claude Fable 5 on Same Prompt](https://simonwillison.net/2026/Aug/7/moonlight-mayhem/#atom-everything) ⭐️ 7.0/10

Simon Willison gave Codex Desktop running GPT-5.6 Sol Ultra the identical one-shot prompt he used to build &\#x27;Raccoon Heist&\#x27; with Claude Fable 5, and the resulting game, &\#x27;Moonlight &amp; Mayhem,&\#x27; is, in his words, much better. The premise evolved from a single raccoon collecting coins and fish to a museum heist where the player rescues two raccoon crewmates and stacks them to steal a golden sardine, using textures Codex generated via gpt-image-2. The one-shot version shipped with a bug that gave every raccoon an enormous black eyeball sphere, which Codex missed despite reviewing screenshots; Willison fixed it by asking &\#x27;Why do the raccoons have huge black spheres on them?&\#x27; followed by &\#x27;Fix it.&\#x27; Codex spent 52 minutes on the project, and the full transcript is in the GitHub repository. According to Simon&\#x27;s AgentsView estimate, the same session would have cost about $23.28 in input/output API tokens \($700.7K input, 32.5M cached, 148K output\) if paid at full API prices rather than covered by the Codex subscription.

rss · Simon Willison · Aug 7, 19:18

**「Background」** Codex Desktop is OpenAI&\#x27;s coding-agent environment; in GPT-5.6 Sol Ultra mode the model makes aggressive use of sub-agents to work on a task. Earlier, Willison used Claude Fable 5 to one-shot a full game from a prompt based on a GPT-3 and DALL-E premise he generated four years ago, which became the comparison point for this test. The shared &\#x27;Raccoon Heist&\#x27; premise describes a team of thieving raccoons carrying out heists, but the two models interpreted that premise very differently.

**「Impact」** For developers evaluating coding agents, the comparison is concrete evidence that on an identical game-building prompt, Codex plus GPT-5.6 Sol Ultra can produce a more ambitious and polished result than Claude Fable 5 while generating its own art assets. The unspotted giant-eyeball bug shows that even capable agents can miss visual defects in screenshots, so human review and iterative fix prompts remain necessary.

**Tags**: `#AI code generation`, `#GPT-5.6`, `#Codex`, `#Claude Fable`, `#game development`

---

<a id="item-tech-news-9"></a>
### [SpaceX 10GW in 2027: $300B ARR and Microsoft as Top Offtaker](https://newsletter.semianalysis.com/p/spacex-10gw-in-2027-why-its-real) ⭐️ 7.0/10

SemiAnalysis released an analysis arguing that SpaceX can realistically reach 10GW of compute capacity by 2027, projecting it would generate approximately $300B in annual recurring revenue. The firm positions Microsoft as the largest likely offtaker, tying the capacity to Microsoft&\#x27;s &\#x27;10GW 2026 awakening&\#x27; and triple-digit Azure growth. The analysis cites an inference rate of 100B tokens per GW per year as a key efficiency assumption. No official confirmation or detailed technical evidence was included in the source item, so the projections remain analytic estimates rather than confirmed plans.

rss · Semianalysis · Aug 7, 20:08

**「Background」** SemiAnalysis, a technology research firm, publishes a report arguing that SpaceX is on track to build about 10GW of AI compute capacity by year-end 2027, having evaluated all suitable sites and compiled a quarter-by-quarter list of gas generation equipment from 30+ turbine, engine, and fuel cell suppliers. The report frames this against surging AI inference demand, projecting that Microsoft&\#x27;s Azure could grow triple-digits and that Microsoft would become the largest offtaker of SpaceX&\#x27;s compute capacity. This is part of a broader analysis of AI infrastructure scaling and cloud demand shifts.

**「Impact」** SemiAnalysis projects that Microsoft would become the largest offtaker of SpaceX&\#x27;s 10GW compute, providing the capacity needed to support triple-digit Azure growth if the 2027 targets are met.

<details><summary>References</summary>
<ul>
<li><a href="https://newsletter.semianalysis.com/p/spacex-10gw-in-2027-why-its-real">SpaceX 10GW in 2027 – Why It’s Real, Will Drive $500B ARR for ...</a></li>
<li><a href="https://www.europesays.com/3181060/">SpaceX 10GW in 2027 – Why It’s Real, Will Drive $500B ARR for ...</a></li>

</ul>
</details>

**Tags**: `#AI inference`, `#SpaceX`, `#Microsoft`, `#cloud infrastructure`, `#hardware`

---

<a id="item-tech-news-10"></a>
### [Gemini Struggles While GCP Gains, Says Analysis](https://newsletter.semianalysis.com/p/gemini-is-cooked-but-gcp-is-cooking) ⭐️ 7.0/10

SemiAnalysis&\#x27;s Max Kan argues that Google&\#x27;s Gemini AI models face long-term strategic failure, while Google Cloud Platform \(GCP\) is enjoying short-term gains from the same AI push. The piece frames DeepMind&\#x27;s extended struggles as a counterintuitive benefit to GCP, because AI infrastructure demand and model deployment needs still funnel work to Google&\#x27;s cloud business. The analysis was published in the newsletter &\#x27;Gemini is Cooked but GCP is Cooking&\#x27; and covers the divergence between Google&\#x27;s model-side competitiveness and its cloud-side growth. It suggests GCP&\#x27;s momentum could help offset Gemini&\#x27;s setbacks in the near term, even though the underlying model risk remains unresolved.

rss · Semianalysis · Aug 7, 02:32

**「Background」** Gemini is Google&\#x27;s family of large language models, developed partly by DeepMind, while GCP \(Google Cloud Platform\) is Google&\#x27;s cloud computing business. The analysis argues that although Gemini lost its competitive edge during 2026 after Gemini 3 Pro was widely considered the best model in late 2025, Google&\#x27;s cloud unit is gaining revenue in the short term as AI demand drives GCP growth. This tension underlies the newsletter&\#x27;s claim that DeepMind&\#x27;s long-term struggles are GCP&\#x27;s short-term gain.

**「Impact」** For Google, the analysis implies that near-term GCP revenue growth may partially compensate for Gemini&\#x27;s competitive losses, but the long-term strategic risk from DeepMind&\#x27;s model failures remains an unresolved threat to Google&\#x27;s broader AI leadership.

<details><summary>References</summary>
<ul>
<li><a href="https://newsletter.semianalysis.com/p/gemini-is-cooked-but-gcp-is-cooking">Gemini is Cooked but GCP is Cooking - newsletter.semianalysis.com</a></li>
<li><a href="https://newsletter.semianalysis.com/p/gemini-is-cooked-but-gcp-is-cooking">or why DeepMind&#x27;s long term failure is GCP &#x27;s short term gain</a></li>
<li><a href="https://www.zdnet.com/article/google-cloud-hits-a-10b-annual-revenue-run-rate/">Google Cloud hits a $10B annual revenue run rate | ZDNET</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Google Cloud`, `#Gemini`, `#technology industry`, `#analysis`

---

<a id="item-tech-news-11"></a>
### [sub2api OAuth flaw allows account takeover with only an email](https://github.com/Wei-Shaw/sub2api/issues/5350) ⭐️ 7.0/10

sub2api v0.1.171 and earlier contain a high-severity OAuth account takeover vulnerability rated CVSS 8.8. An attacker who only knows the victim&\#x27;s registered email address can bind their own OAuth identity to the victim&\#x27;s account without a password, verification code, or user interaction. The flaw is in the pending session flow&\#x27;s existingUser branch, which fails to validate the password and verification code before setting the target user ID to the victim and completing OAuth binding. After exploitation, every subsequent OAuth login by the attacker resolves to the victim account, giving full control over API keys, billing balance, and subscription quotas.

telegram · zaihuapd · Aug 7, 14:59

**「Background」** Sub2API is an open-source AI API gateway platform that lets users access AI product subscriptions through a single API key; it handles authentication, billing, load balancing, and request forwarding. The disclosed vulnerability occurs in Sub2API&\#x27;s OAuth identity binding flow, specifically in the pending-session process: the existingUser branch does not verify the user&\#x27;s password or a verification code, so an attacker who knows the victim&\#x27;s registered email can bind their own OAuth identity to the victim&\#x27;s account and take it over.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/Wei-Shaw/sub2api">GitHub - Wei-Shaw/sub2api: Sub2API 一站式开源中转服务，让 Claude...</a></li>

</ul>
</details>

**Tags**: `#security`, `#oauth`, `#vulnerability`, `#sub2api`, `#account takeover`

---

<a id="item-tech-news-12"></a>
### [AWS Cracks Down on Internal CPU Waste as Agentic AI Raises Demand](https://www.tomshardware.com/pc-components/cpus/amazon-cracks-down-on-cpu-waste-among-engineers-as-agentic-ai-crunch-intensifies-cpu-demand-makes-low-utilization-ec2-instances-a-hot-commodity) ⭐️ 7.0/10

Amazon AWS is cracking down on internal CPU waste by engineers as agentic AI workloads drive surging demand for CPU capacity. In May of this year, AWS asked engineers to reduce CPU waste to preserve capacity for customers, pushing internal EC2 instance approval wait times from hours to days, a delay some engineers said they had never experienced in years of work. The shift is driven by agentic AI, which unlike traditional inference relies heavily on CPU-based tool calls and more complex GPU orchestration, moving data center GPU-to-CPU ratios from 8:1 or 4:1 toward 1:1. AMD and Nvidia have both expanded their data center CPU efforts to compete for this growing market.

telegram · zaihuapd · Aug 7, 16:31

**「Background」** AWS provides on-demand virtual servers called EC2 instances, and internal engineering teams have historically used them for development and testing. Traditional AI inference workloads have been dominated by GPUs, with CPUs used mainly for smaller tasks, so data centers were designed with far more GPUs than CPUs. Agentic AI refers to systems that autonomously plan and execute multi-step tasks, frequently invoking tools and coordinating GPU work, which requires substantial CPU resources.

**「Impact」** The crackdown means AWS engineers now face multi-day waits for internal instances, slowing development and testing while AWS prioritizes paying customer capacity. It also signals a broader infrastructure trend: as agentic AI becomes common, cloud providers and chip vendors must rebalance CPU and GPU provisioning, with AMD and Nvidia competing on data center CPUs.

**Tags**: `#AWS`, `#EC2`, `#AI infrastructure`, `#CPU`, `#agentic AI`

---

<a id="item-tech-news-13"></a>
### [OpenAI Says Astra May Reach Critical Cyber Capability Threshold, Delays Possible](https://openai.com/index/responding-next-frontier-critical-cyber-capabilities/) ⭐️ 7.0/10

On August 7, 2026, OpenAI disclosed that its upcoming Astra model showed significant progress in agentic coding and cybersecurity in internal evaluations, with preliminary results strong enough that OpenAI cannot rule out that Astra meets its &\#x27;critical&\#x27; cyber capability threshold. Previously, models such as GPT-5.6-Sol were rated only &\#x27;high&\#x27; on the same evaluation. Under OpenAI&\#x27;s Preparedness Framework, crossing the critical threshold means the model could autonomously discover and exploit zero-day vulnerabilities in hardened real-world systems without human intervention, or plan and execute end-to-end novel cyber attacks from high-level goals alone. In response, OpenAI paused Astra-related internal activities that do not meet enhanced security requirements, introduced isolated testing environments, enhanced encryption and universal monitoring, and will work with government agencies and AI safety organizations on third-party testing. The expanded safety testing may delay Astra&\#x27;s release.

telegram · zaihuapd · Aug 7, 16:44

**「Background」** OpenAI&\#x27;s Preparedness Framework rates frontier models against cyber-capability thresholds such as &\#x27;high&\#x27; and &\#x27;critical.&\#x27; In earlier evaluations, models like GPT-5.6-Sol reached only &\#x27;high&\#x27;; for the upcoming Astra model, preliminary results were strong enough that OpenAI cannot rule out &\#x27;critical&\#x27; cyber capabilities, meaning it could autonomously discover and exploit zero-day vulnerabilities in hardened real-world systems or plan and execute end-to-end novel cyberattacks from high-level goals. As a result, OpenAI paused some Astra-related internal activities that do not meet stricter security requirements and will run third-party testing with government agencies and AI safety organizations.

**「Impact」** OpenAI has paused internal activities with Astra and expanded third-party safety testing because internal evaluations “cannot rule out” critical cyber capabilities, so the model’s release will likely be postponed; the assessment is preliminary and no formal new release date has been announced.

<details><summary>References</summary>
<ul>
<li><a href="https://www.axios.com/2026/08/07/openai-astra-model-delay-cybersecurity-risks">OpenAI slows release of Astra model citing cyber capabilities</a></li>
<li><a href="https://openai.com/index/responding-next-frontier-critical-cyber-capabilities/">Responding to the next frontier of critical cyber capabilities | OpenAI</a></li>
<li><a href="https://www.axios.com/2026/08/07/openai-astra-model-delay-cybersecurity-risks">OpenAI slows release of Astra model citing cyber capabilities</a></li>
<li><a href="https://tech.yahoo.com/cybersecurity/articles/openai-slow-down-astra-model-173331847.html">OpenAI To Slow Down Astra Model Release Over ‘Critical’ Cyber ...</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#AI safety`, `#cybersecurity`, `#frontier models`, `#Astra`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Fed September rate hike odds tumble after weak July jobs report](https://www.cnbc.com/2026/08/07/odds-the-fed-hikes-in-september-tumble-following-big-july-jobs-miss.html) ⭐️ 8.0/10

A weak July jobs report showing the U.S. economy shed jobs has sharply cut investors&\#x27; expectations for a September Federal Reserve rate hike. Kalshi odds of holding rates steady jumped to 65% from roughly 50-50 before the report, while CME&\#x27;s FedWatch put the chance at 60%.

rss · CNBC Finance · Aug 7, 13:34

**「Background」** The Fed held rates steady at its late-July meeting despite three dissents favoring a hike, and the July CPI report due Aug. 12 may still be decisive for September.

**Tags**: `#Federal Reserve`, `#interest rates`, `#jobs report`, `#monetary policy`, `#market expectations`

---

<a id="item-finance-news-2"></a>
### [SEC approves Nasdaq 23-hour trading, starting December 6, 2026](https://finance.sina.com.cn/stock/bxjj/2026-08-07/doc-inimnkup0012339.shtml) ⭐️ 8.0/10

The U.S. Securities and Exchange Commission \(SEC\) has approved Nasdaq’s 23-hour trading schedule, which will begin on Dec. 6, 2026, leaving the market closed only from 8 to 9 p.m. ET each day.

telegram · zaihuapd · Aug 7, 10:03

**「Background」** The approval follows the SEC’s earlier accelerated approval of NYSE Arca’s 22-hour plan and Cboe’s near-24x5 proposal, both targeting December 2026; retail investors already trade overnight through alternative systems such as Blue Ocean ATS and platforms like Robinhood and Charles Schwab.

**「Impact」** The extended schedule will lengthen the U.S. equity trading day, but overnight sessions tend to have thinner liquidity and wider spreads, and the SEC has scheduled a Sept. 17 roundtable on investor protection.

**Tags**: `#Nasdaq`, `#SEC`, `#market structure`, `#trading hours`, `#US equities`

---

<a id="item-finance-news-3"></a>
### [Chevrolet Exits China New-Car Market After 21 Years](https://m.mydrivers.com/newsview/1142126.html) ⭐️ 8.0/10

SAIC-GM has announced that Chevrolet will stop selling new cars in China, ending the brand&\#x27;s 21-year presence and affecting about 7.5 million owners. Chevrolet&\#x27;s China sales fell to 52,000 vehicles in 2025 from a peak above 600,000, and the company says manufacturing will shift to exports while after-sales moves to Buick service channels.

telegram · zaihuapd · Aug 7, 11:12

**「Background」** Chevrolet entered China through the SAIC-GM joint venture in 2005, and hot models like the Cruze and Malibu made it one of the strongest foreign brands before Chinese electric-vehicle makers squeezed sales of joint-venture petrol cars.

**「Impact」** The affected group includes Chevrolet&\#x27;s roughly 7.5 million Chinese owners and its retailer network; many 4S dealerships have already shut, and the company says owner rights remain unchanged through Buick-authorized after-sales support.

**Tags**: `#雪佛兰`, `#上汽通用`, `#中国市场退出`, `#汽车行业`, `#新能源竞争`

---

<a id="item-finance-news-4"></a>
### [Beijing cuts social-security requirement for homebuyers without Beijing hukou to 1 year](https://www.peopleapp.com/column/30052875352-500007640471) ⭐️ 8.0/10

Beijing’s housing authorities announced further easing of homebuying rules: people without Beijing hukou \(household registration\) now need one consecutive year of social-insurance or income-tax payments before buying a home inside the 5th Ring Road, and parents gifting a property to a child no longer triggers a purchase-eligibility check for the child. The city also increased the maximum first-home provident fund loan for couples to 2.4 million yuan, with a possible 1 million yuan top-up for qualifying buyers, and allowed withdrawals of up to 250,000 yuan for home renovation.

telegram · zaihuapd · Aug 7, 13:57

**「Background」** This follows Beijing’s earlier relaxation of purchase restrictions, which had already cut the social-security or income-tax requirement for non-Beijing-hukou buyers to one to two years.

**Tags**: `#房地产政策`, `#北京`, `#公积金`, `#限购`, `#住房市场`

---

<a id="item-finance-news-5"></a>
### [Trump signs executive orders targeting birthright citizenship and birth tourism](https://www.bbc.co.uk/news/articles/cj63966j95yo) ⭐️ 7.0/10

President Donald Trump signed two executive orders on Aug. 6 that aim to restrict birthright citizenship, including one that expands the cases in which children born to non-citizen parents would not automatically gain U.S. citizenship and another that bans so-called birth tourism. The orders face likely legal defeat: the Supreme Court ruled 6–3 on June 30 that Trump’s earlier attempt to end the 150-year-old citizenship guarantee was unconstitutional, and the American Civil Liberties Union said it expects the new orders to lose in court.

telegram · zaihuapd · Aug 7, 07:01

**「Background」** The U.S. Constitution&\#x27;s 14th Amendment grants citizenship to people born in the country, and the Supreme Court in June 2025 struck down Trump&\#x27;s earlier executive order that tried to end birthright citizenship, ruling it unconstitutional. Trump&\#x27;s new orders attempt to narrow that rule by reinterpreting historical exceptions, but legal experts say they face serious constitutional problems.

<details><summary>References</summary>
<ul>
<li><a href="https://www.archives.gov/milestone-documents/14th-amendment">14 th Amendment to the U . S . Constitution: Civil... | National Archives</a></li>

</ul>
</details>

**Tags**: `#US politics`, `#immigration`, `#birthright citizenship`, `#executive order`, `#Supreme Court`

---

<a id="item-finance-news-6"></a>
### [Australia proposes A$31.30/hour minimum pay for food delivery riders](https://www.twu.com.au/press/food-delivery-workers-to-get-world-first-minimum-standards-on-pay-and-conditions-from-august/) ⭐️ 7.0/10

Australia’s Fair Work Commission has proposed a minimum income guarantee of A$31.30 per hour of active delivery time for food delivery riders on platforms such as Uber Eats and DoorDash. If approved, the standard could take effect as early as 17 August 2026, and platforms would have to top up riders’ pay when earnings fall below that rate.

telegram · zaihuapd · Aug 7, 15:44

**「Background」** The proposal follows an application by the Transport Workers’ Union, which later submitted a proposed scheme jointly with two platforms. The union and some media call it a “world first,” but similar minimum-payment rules already exist in New York, Seattle and British Columbia.

**「Impact」** If approved, the rule would affect food delivery riders and gig platforms operating in Australia; the Transport Workers’ Union says 25 gig workers have been killed on the roads since 2017.

**Tags**: `#gig economy`, `#minimum pay`, `#Australia`, `#food delivery`, `#labor regulation`

---