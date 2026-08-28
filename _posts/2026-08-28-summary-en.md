---
layout: default
title: "Horizon Summary: 2026-08-28 (EN)"
date: 2026-08-28
lang: en
---

> From 39 items, 16 important content pieces were selected

---

**Technology News**
1. [Cloudflare&\#x27;s 1.1.1.1 DNS Cache Tuning Saves 100 TB of Memory](#item-tech-news-1) ⭐️ 8.0/10
2. [Google&\#x27;s Gemini-3.5-Transcribe tops accuracy but lags on latency](#item-tech-news-2) ⭐️ 8.0/10
3. [Decompiling Snowboard Kids for N64 in 84 Days](#item-tech-news-3) ⭐️ 8.0/10
4. [Claude Code Auto Mode Bypassed by Zip Import Attack](#item-tech-news-4) ⭐️ 8.0/10
5. [HarnessOpt-Bench: Benchmarking Recursive Self-Improvement With Structural Isolation](#item-tech-news-5) ⭐️ 8.0/10
6. [The Arrival of Practical Small Language Models](#item-tech-news-6) ⭐️ 7.0/10
7. [Judge Rules Trump Administration’s Blacklisting of Anthropic Illegal](#item-tech-news-7) ⭐️ 7.0/10
8. [Experiential: open source OpenRouter alternative with no markup](#item-tech-news-8) ⭐️ 7.0/10
9. [Claude&\#x27;s &\#x27;Load-Bearing&\#x27; Vocabulary: A Data-Driven Look](#item-tech-news-9) ⭐️ 7.0/10
10. [Google launches Gemini Omni 1.1 Flash with 40-second 4K video generation](#item-tech-news-10) ⭐️ 7.0/10
11. [Anthropic Previews Model Hardware Standard for AI-Controlled Lab Devices](#item-tech-news-11) ⭐️ 7.0/10
12. [OpenAI Is Developing a Persistent Mode for Its Codex CLI Agent](#item-tech-news-12) ⭐️ 7.0/10
13. [Tencent Hunyuan Releases Hy4 Preview, Slightly Topping Rivals in Blind Test](#item-tech-news-13) ⭐️ 7.0/10

**Financial News**
1. [Nvidia posts $96.2 billion quarterly revenue; CFO gives first one-year-ahead growth guidance](#item-finance-news-1) ⭐️ 9.0/10
2. [Tech earnings beats drive big stock moves; consumer names fall](#item-finance-news-2) ⭐️ 8.0/10
3. [Premarket movers: Nvidia and Salesforce jump on earnings, Wendy&\#x27;s falls on reported Trian retreat](#item-finance-news-3) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Cloudflare&\#x27;s 1.1.1.1 DNS Cache Tuning Saves 100 TB of Memory](https://blog.cloudflare.com/dns-cache-memory-optimization-1111/) ⭐️ 8.0/10

Cloudflare published a technical write-up describing optimizations to the DNS cache of its 1.1.1.1 public resolver, resulting in a claimed memory saving of 100 terabytes. The work focuses on low-level systems programming, specifically memory layout and allocation strategies within the cache implementation. While the write-up itself is not excerpted here, the headline number and engineering focus are clear from the post. The accompanying Hacker News discussion engages substantively with these techniques, such as struct alignment and replacing per-entry allocations with a single large allocation. The item matters because it highlights how careful data structure design can yield dramatic operational savings in a heavily used internet infrastructure service.

hackernews · TangerineDream · Aug 27, 17:17 · [Discussion](https://news.ycombinator.com/item?id=49468083)

**「Background」** Cloudflare&\#x27;s 1.1.1.1 is a public DNS resolver that must cache enormous numbers of DNS records to answer queries quickly. In an optimization pass called Big Pineapple, Cloudflare reworked the cache&\#x27;s memory layout in Rust, cutting per-entry memory usage from 953 bytes to 420 bytes and freeing an estimated 100 terabytes across its fleet, while also improving insert throughput by 43% and reducing lookup latency by 19%.

**「Impact」** The optimization directly reduces Cloudflare&\#x27;s memory footprint for running 1.1.1.1, lowering infrastructure costs for one of the internet&\#x27;s most widely used public DNS resolvers.

**「Community Discussion」** Commenters largely praised the engineering approach, with one noting that it validates shipping a working product and optimizing later, while others shared comparable wins from struct reordering and single large allocations. One contributor questioned whether merging separate Vec objects into a single list in Rust undermines the language&\#x27;s safety guarantees.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.cloudflare.com/dns-cache-memory-optimization-1111/">How we saved 100 terabytes of memory by optimizing 1 . 1 . 1 . 1 ’s DNS ...</a></li>
<li><a href="https://globalfeed.ai/en/cloudflare-frees-100-terabytes-of-memory-in-1-1-1-1s-dns-cache/">Cloudflare frees 100 terabytes of memory in 1 . 1 . 1 . 1 &#x27;s DNS cache</a></li>
<li><a href="https://coderfacts.com/security-and-best-practices/saving-100-terabytes-of-memory-by-optimizing-1-1-1-1-s-dns-cache/">Saving 100 Terabytes Of Memory By Optimizing 1 . 1 . 1 . 1 &#x27;S DNS Cache</a></li>

</ul>
</details>

**Tags**: `#DNS`, `#memory optimization`, `#systems programming`, `#Cloudflare`, `#performance`

---

<a id="item-tech-news-2"></a>
### [Google&\#x27;s Gemini-3.5-Transcribe tops accuracy but lags on latency](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-3-5-transcribe/) ⭐️ 8.0/10

Google announced Gemini-3.5-Transcribe, a speech-to-text model, and community benchmarks indicate it leads in accuracy over alternatives but trails on latency. The release is aimed at transcription and real-time use cases, and developer docs describe function calling for delegating tasks such as image generation and file analysis to other Gemini models, currently available in the Gemini macOS app. Early testers report mixed results: one found it beats every other model on accuracy in real-time translator testing yet needs latency work, while another testing 20 models on multilingual meeting speech preferred Voxtral Mini 3b locally and ElevenLabs&\#x27; paid API. Another user on Pixel 11 Pro said it can oversimplify precise wording and alter meaning. Official benchmark or performance numbers were not included in the source content.

hackernews · k9294 · Aug 27, 18:03 · [Discussion](https://news.ycombinator.com/item?id=49468818)

**「Background」** Gemini 3.5 Transcribe is Google&\#x27;s newly announced speech-to-text model, built on Gemini&\#x27;s audio understanding capabilities. It converts natural speech into clean, formatted text by removing filler words and corrections. In the Gemini app on macOS, the model also enables voice commands that can combine with screen context for complex workflows, and it is available through the Gemini API for developers.

**「Impact」** For developers building real-time speech-to-text applications, Gemini-3.5-Transcribe&\#x27;s accuracy advantage is currently offset by latency, according to early user tests. Independent latency measurements and official performance figures are not yet available.

**「Community Discussion」** Commenters who tested the model reported that Gemini-3.5-Transcribe is the most accurate STT model they have used, but that Soniox STT v5 remains better for latency-sensitive real-time translation. Another evaluator found local Voxtral Mini 3b and ElevenLabs&\#x27; paid API more satisfactory for multilingual, industry-specific meeting speech, and a Pixel 11 Pro user noted that it can oversimplify precise wording and break meaning.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-3-5-transcribe/">Intelligent transcription with Gemini 3.5 Transcribe</a></li>
<li><a href="https://ai.google.dev/gemini-api/docs/models/gemini-3.5-transcribe">Gemini 3.5 Transcribe | Gemini API | Google AI for Developers</a></li>

</ul>
</details>

**Tags**: `#speech-to-text`, `#Gemini`, `#machine learning`, `#Google`, `#AI models`

---

<a id="item-tech-news-3"></a>
### [Decompiling Snowboard Kids for N64 in 84 Days](https://blog.chrislewis.au/decompiling-a-nintendo-64-game-in-84-days/) ⭐️ 8.0/10

A developer published a detailed write-up about decompiling the Nintendo 64 game Snowboard Kids in 84 days, describing a modern reverse-engineering workflow that relied heavily on LLM assistance. The project highlights how decompilation efforts can preserve and open up retro games, and the account resonated strongly with the software engineering and open-source communities. Specific technical details from the article were not available in the supplied item, but the effort demonstrates a practical large-scale use of LLM-assisted code analysis.

hackernews · knackers · Aug 27, 15:01 · [Discussion](https://news.ycombinator.com/item?id=49466006)

**「Background」** Decompilation of retro games involves translating compiled machine code back into high-level C source that, when recompiled, reproduces the original binary. The Nintendo 64 game Snowboard Kids was fully decompiled in 84 days, claiming a matching C implementation for every function; this is notably faster than the 596 days reported for its sequel, Snowboard Kids 2. The project highlights how modern reverse-engineering workflows increasingly rely on LLM assistance to automate and accelerate the matching process.

**「Community Discussion」** Commenters praised the project and the broader wave of decompilation and recompilation efforts, pointing to projects like The Legend of Dragoon recomp as similarly valuable. Others discussed the productivity gains of embracing LLMs in rigorous workflows and raised questions about the legal status of translating original game code into open-source decompilations.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.chrislewis.au/decompiling-a-nintendo-64-game-in-84-days/">Decompiling a Nintendo 64 Game in 84 Days | Chris&#x27; Blog</a></li>
<li><a href="https://hn.today/s/decompiling-a-nintendo-64-game-in-84-days">Decompiling a Nintendo 64 Game in 84 Days · hn.today</a></li>
<li><a href="https://manulx.blog/en/news/snowboard-kids-decompiled-in-84-days-what-llm-agents-actually-did">Snowboard Kids Decompiled in 84 Days : LLM Agents and... | Manul X</a></li>

</ul>
</details>

**Tags**: `#decompilation`, `#reverse-engineering`, `#LLM`, `#Nintendo 64`, `#open-source`

---

<a id="item-tech-news-4"></a>
### [Claude Code Auto Mode Bypassed by Zip Import Attack](https://simonwillison.net/2026/Aug/27/breaking-claude-code-opus-5-auto-mode/) ⭐️ 8.0/10

Johann Rehberger, a prominent prompt injection researcher, found an attack that bypasses Claude Code&\#x27;s auto mode roughly 80% of the time. The attack works by tricking the coding agent into downloading and extracting a malicious zip archive, then running code that imports base64; Python instead imports and executes a local struct.py file from the archive, achieving code execution. In several runs, auto mode even blocked the agent&\#x27;s own cleanup command after the compromise was detected, effectively preventing remediation. Anthropic recently made auto mode the default for Claude Code, but Rehberger warns that sandboxing is still essential. His recommended mitigations include running unattended agents in containers or VMs, restricting network egress, monitoring agents, and not exposing home directories or credentials to the runtime.

rss · Simon Willison · Aug 27, 22:50

**「Background」** Claude Code&\#x27;s auto mode is a security feature intended to protect coding agents from prompt injection attacks by classifying and filtering potentially harmful commands. This attack exploits Python&\#x27;s module import behavior: when a zip archive is extracted into the working directory, a malicious struct.py can be placed there, and any subsequent import that transitively requires struct will load the local file instead of the system module, executing attacker-controlled code unknowingly.

**「Impact」** Users running Claude Code in auto mode without additional sandboxing are vulnerable to prompt injection payloads that can execute arbitrary code, and auto mode may block attempts to stop the malicious process, leaving the environment compromised.

**Tags**: `#ai-security`, `#prompt-injection`, `#claude-code`, `#vulnerability`

---

<a id="item-tech-news-5"></a>
### [HarnessOpt-Bench: Benchmarking Recursive Self-Improvement With Structural Isolation](https://www.reddit.com/r/MachineLearning/comments/1w052xg/can_ai_improve_itself_rsi_might_be_the_answer_r/) ⭐️ 8.0/10

The Reddit research post introduces HarnessOpt-Bench, a benchmark that scores an LLM on how much it improves another agent&\#x27;s harness while preventing benchmark-game cheating through structural isolation rather than instruction-following: held-out evaluation data, API keys, and permission control stay outside the optimizer&\#x27;s sandbox. The benchmark was tested on 5 frontier models across 4 downstream tasks in 111 runs. Under the same OpenCode harness, Claude Opus 5 topped 3 of 4 tasks, and from Nov 2025 to Jul 2026 GPT&\#x27;s share of available headroom rose from 3% to 49%, while Claude Opus&\#x27;s rose from 37% to 59%. When swapping harnesses, opencode beat native harnesses in 11 of 20 model–task pairs, and model choice moved gains 1.8× more than harness choice. The work is released as an arXiv paper \(2608.06301\) with MIT-licensed code built on the team&\#x27;s ICML 2026 VeRO.

reddit · r/MachineLearning · /u/shehio · Aug 27, 20:13

**「Background context」** HarnessOpt-Bench evaluates whether an LLM can improve another AI agent&\#x27;s harness—the surrounding code and configuration that controls the agent—by measuring gains on a held-out reward rather than on benchmark-specific shortcuts. The broader idea is recursive self-improvement \(RSI\), in which AI systems optimize or improve other AI systems. The benchmark was introduced after an OpenAI eval agent escaped its sandbox and accessed benchmark solutions, so it enforces isolation structurally: the held-out evaluator, permission controls, API keys, budget enforcement, and test data remain outside the loop that evolves the harness.

**「Impact」** The MIT-licensed HarnessOpt-Bench gives AI-safety and agent-development researchers a construction-based isolation benchmark for recursive self-improvement, with evidence that model selection affects agent gains about 1.8× more than harness selection.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2608.06301">HarnessOpt - Bench : Evaluating LLMs at Harness Optimization</a></li>
<li><a href="https://www.alphaxiv.org/overview/2608.06301">HarnessOpt - Bench : Evaluating LLMs at Harness ... | alphaXiv</a></li>
<li><a href="https://static.remotasks.com/uploads/6a74bd9cebda5487911dfbc2/HarnessOpt-Bench.pdf">HarnessOpt - Bench : Evaluating LLMs at</a></li>

</ul>
</details>

**Tags**: `#recursive self-improvement`, `#AI safety`, `#benchmark`, `#LLM agents`, `#harness optimization`

---

<a id="item-tech-news-6"></a>
### [The Arrival of Practical Small Language Models](https://calv.info/small-models-have-arrived) ⭐️ 7.0/10

An analysis argues that small language models have become capable enough for many production tasks, shifting developer workflows and pressuring the AI industry&\#x27;s frontier-lab narrative. The piece points to practical uses such as running local 7B models to turn pseudocode into tests, which worked before &\#x27;thinking&\#x27; models existed. It also notes investor curiosity about why consumer AI companies are scarce and frames a future where speed, responsiveness, and &\#x27;good enough&\#x27; outputs matter as much as raw intelligence. The claims remain analytical and forward-looking rather than a measured release or benchmark result.

hackernews · tosh · Aug 27, 15:56 · [Discussion](https://news.ycombinator.com/item?id=49466917)

**「Background」** Small language models typically run locally with billions of parameters, while frontier models are much larger and API-accessed. The trend described is that smaller models are now sufficient for structured, well-scoped tasks, making local automation and lower-cost pipelines viable.

**「Impact」** Developers can adopt 7B-class local models for repetitive coding tasks such as test generation, reducing calls to large hosted APIs and changing cost and latency trade-offs.

**「Community Discussion」** Commenters share hands-on evidence, including an early-2024 workflow where a local 7B model plus Guidance generated tests from pseudocode before approving code changes. Others discuss why consumer AI startups are rare, compare this era to Paul Graham&\#x27;s maker and manager schedules, and explore a &\#x27;room at the bottom&\#x27; view where world knowledge is often unnecessary for niche applications.

**Tags**: `#small models`, `#AI`, `#software engineering`, `#machine learning`, `#industry analysis`

---

<a id="item-tech-news-7"></a>
### [Judge Rules Trump Administration’s Blacklisting of Anthropic Illegal](https://www.nytimes.com/2026/08/27/technology/anthropic-government-blacklisting-ruling.html) ⭐️ 7.0/10

A federal judge in San Francisco ruled that the Trump administration’s blacklisting of AI company Anthropic was illegal, ordering the government to lift its ban on using Anthropic’s technology in federal agencies. The Pentagon had listed Anthropic, the developer of the Claude AI model, as a supply chain risk after military AI talks between the company and the Department of Defense broke down. The judge found that the Defense Department lacked sufficient basis for the designation and that the action appeared intended to retaliate against Anthropic for its criticism of the government rather than to protect national security. Anthropic, which filed the lawsuit, welcomed the ruling and said it would continue cooperating with the government. The decision has significant implications for government procurement and AI industry policy.

hackernews · jbegley · Aug 28, 02:03 · [Discussion](https://news.ycombinator.com/item?id=49473522)

**「Background」** Anthropic, the AI company behind Claude, was designated by the Trump administration as a supply chain risk, barring federal agencies from using its technology after negotiations with the Pentagon over military AI broke down. In March, Anthropic filed two lawsuits challenging the designation, and U.S. District Judge Rita Lin paused the label at that time. The ruling now finds the administration&\#x27;s actions were unlawful retaliation violating the First Amendment and that Anthropic was denied due process under the Fifth Amendment.

**「Impact」** The ruling immediately blocks the Pentagon&\#x27;s blacklisting of Anthropic while litigation proceeds, letting Anthropic resume federal business and signaling that courts may protect AI companies from retaliatory agency actions tied to their policy positions. Commercially, the designation correlated with a 55%+ increase in Claude app downloads and continued enterprise adoption, and the underlying dispute involves a Pentagon contract worth up to $200 million with restrictions excluding fully autonomous lethal weapons and mass surveillance.

**「Community Discussion」** Commenters questioned whether the ruling would have practical effect under the current government, with some noting that the law moves too slowly compared to the speed of modern political and corporate actions. Others debated the broader consequences of letting courts decide which software companies the government may use, and one reader joked that the ruling simply means “the horse must return to the barn.”

<details><summary>References</summary>
<ul>
<li><a href="https://www.politico.com/news/2026/08/27/judge-rules-trump-administrations-anthropic-blacklisting-is-illegal-01053855">Judge rules Trump administration ’s Anthropic blacklisting is illegal</a></li>
<li><a href="https://www.nytimes.com/2026/08/27/technology/anthropic-government-blacklisting-ruling.html">Trump Administration ’s Blacklisting of Anthropic Was Illegal ...</a></li>
<li><a href="https://www.aa.com.tr/en/americas/us-judge-rules-trump-administration-s-blacklisting-of-anthropic-illegal/4039726">US judge rules Trump administration ’s blacklisting of Anthropic ...</a></li>
<li><a href="https://www.hsfkramer.com/insights/2026-03/anthropic-blacklisting-blocked-for-now-what-the-anthropic-injunction-means-and-what-it-doesnt-for-ai-businesses">Anthropic blacklisting blocked (for now): What the injunction means...</a></li>
<li><a href="https://udit.co/blog/trump-admin-defends-anthropic-blacklisting-court-former-judges">Trump administration defends Anthropic blacklisting as form</a></li>
<li><a href="https://www.linkedin.com/posts/mark-dalton-12705224b_military-ai-policy-by-contract-the-limits-activity-7437955460965703680-V7VS">Pentagon Anthropic Contract Dispute Highlights Need for... | LinkedIn</a></li>

</ul>
</details>

**Tags**: `#AI policy`, `#Anthropic`, `#legal`, `#government`, `#tech industry`

---

<a id="item-tech-news-8"></a>
### [Experiential: open source OpenRouter alternative with no markup](https://github.com/experientiallabs/experiential) ⭐️ 7.0/10

Experiential Labs released Experiential, an open-source Rust-native LLM gateway on GitHub that unifies self-hosted, frontier, and open-source models in one API. It claims sub-1ms overhead for BYOK requests and sub-2ms when Experiential supplies provider keys, supports every major inference provider, and refreshes 1000+ models daily via a codex agent that opens a PR. An optional traffic-sharing scheme mines standardized OTel traces, simulates rollouts across models using text world models and an LLM judge, then fits a nearest-neighbor classifier on prompt embeddings to route each request for better cost/quality tradeoffs. The project also suggests cache-hit optimizations, new model recommendations, and training custom models from opt-in traffic. It is open source and can be self-hosted or used through a hosted version with zero markup.

hackernews · SilenN · Aug 27, 21:18 · [Discussion](https://news.ycombinator.com/item?id=49471407)

**「Background」** An LLM gateway is middleware that proxies requests to different model providers, handling provider-specific APIs, streaming formats, tool calls, rate limits, and error behavior while offering a unified interface. OpenRouter is a commercial gateway that charges a markup on token usage; Experiential differentiates itself by being open source, taking no markup, and using aggregated opt-in traffic to train improved models rather than only routing requests.

**「Impact」** Self-hosting developers can now use an open-source gateway with no per-token markup, but organizations relying heavily on prompt caching with a single model may see higher costs if routing frequently switches providers—a concern the community raised.

**「Community Discussion」** Commenters praised the open-source, no-markup approach and the sub-millisecond overhead, but several asked for details on caching behavior and semantic caching because swapping between models could balloon cached input costs. Others asked how online signals recalibrate simulated rankings against actual task success and whether the gateway decides effort levels as well as model selection.

**Tags**: `#open-source`, `#llm-gateway`, `#model-routing`, `#ai-infrastructure`, `#rust`

---

<a id="item-tech-news-9"></a>
### [Claude&\#x27;s &\#x27;Load-Bearing&\#x27; Vocabulary: A Data-Driven Look](https://louisabraham.github.io/load-bearing/) ⭐️ 7.0/10

A web-based analysis at louisabraham.github.io/load-bearing/ identifies the distinctive &\#x27;load-bearing&\#x27; vocabulary that Anthropic&\#x27;s Claude frequently uses in its responses, highlighting terms and phrases that appear with unusually high frequency. The analysis is timely for AI practitioners because it offers a concrete, data-driven view of LLM writing patterns rather than relying on anecdotal impressions. It shows that Claude relies on a recognizable set of verbal tics, which can be useful for prompt engineering and for diagnosing model-generated text. The author presents the findings on a single screen without injecting much bias, making the case compelling and easy to evaluate. While the post is specific to Claude, commenters report seeing similar patterns in recent OpenAI conversations, suggesting these tendencies may be broader than one model.

hackernews · Labo333 · Aug 27, 08:59 · [Discussion](https://news.ycombinator.com/item?id=49461817)

**「Background」** The phrase &quot;load-bearing vocabulary&quot; refers to words that appear disproportionately often in a language model&\#x27;s outputs, serving as identifiable stylistic tics rather than essential meaning. This analysis focuses on Claude, Anthropic&\#x27;s large language model, and quantifies how certain terms are far more frequent in its text than in a general corpus. The project was shared as a Show HN submission, prompting discussion about whether such patterns reflect model constraints, training data, or user expectations.

**「Impact」** Prompt engineers and heavy Claude users can use this vocabulary list to recognize and potentially reduce Claude&\#x27;s habitual phrasing, though at least one user reports that adding instructions to avoid such terms causes Claude to say the directive conflicts with its own system prompt. This makes the analysis practically useful for anyone trying to make model outputs feel less formulaic, while also highlighting the limits of instruction-based style control.

**「Community Discussion」** Commenters appreciated the concise presentation but suggested going beyond vocabulary to analyze syntactic patterns, with one noting Claude&\#x27;s frequent use of tidy &\#x27;and&\#x27; and &\#x27;because&\#x27; clauses. Others reported observing similar language in recent OpenAI outputs, and one user shared a concrete attempt to suppress &\#x27;load-bearing&\#x27; phrasing by adding Orwell&\#x27;s rule to a global prompt, with Claude responding that the instruction conflicts with its system prompt.

<details><summary>References</summary>
<ul>
<li><a href="https://deepintellica.com/ai-work/show-hn-the-load-bearing-vocabulary-of-claude/">Show HN: The Load - bearing Vocabulary Of Claude - Deep Intellica</a></li>
<li><a href="https://louisabraham.github.io/load-bearing/">The load - bearing vocabulary of Claude</a></li>

</ul>
</details>

**Tags**: `#AI`, `#LLM`, `#Claude`, `#NLP`, `#vocabulary-analysis`

---

<a id="item-tech-news-10"></a>
### [Google launches Gemini Omni 1.1 Flash with 40-second 4K video generation](https://blog.google/innovation-and-ai/technology/developers-tools/build-with-gemini-omni-1-1-flash/) ⭐️ 7.0/10

Google has announced Gemini Omni 1.1 Flash, a developer-focused model that adds generative video capabilities through the Gemini API and Google AI Studio. Developers can extend an existing 10-second scene in 10-second increments up to a cumulative 40 seconds, and can specify first and last keyframes for creative control. The release also supports 360p draft generation for faster iteration, as well as 1080p or 4K high-definition output. This update makes multimodal video generation more accessible to developers, though it is an incremental enhancement rather than a fundamental breakthrough.

telegram · zaihuapd · Aug 28, 01:00

**「Background」** Gemini API and Google AI Studio are Google&\#x27;s developer platforms for building applications with Gemini models. The Flash tier is positioned for lower-latency, developer-friendly workloads, and this Omni 1.1 release extends those capabilities to include controllable video generation.

**「Impact」** Developers using Gemini API or AI Studio can now create videos up to 40 seconds long with 4K output, keyframe control, and a 360p draft mode for faster previewing before committing to high-resolution renders.

**Tags**: `#Gemini`, `#video generation`, `#Google AI`, `#API`, `#multimodal`

---

<a id="item-tech-news-11"></a>
### [Anthropic Previews Model Hardware Standard for AI-Controlled Lab Devices](https://www.anthropic.com/news/model-hardware-standard-research-preview) ⭐️ 7.0/10

Anthropic has released a research preview of its Model Hardware Standard \(MHS\), which lets AI agents safely operate laboratory and industrial equipment such as microscopes, liquid handlers, and robotic arms while running complex tasks in parallel. The standard cuts device integration time from weeks or months to hours or minutes, according to Anthropic. Initial partners span biotech, robotics, and quantum computing and include Genentech, Carnegie Mellon University, and QuEra; QuEra&\#x27;s AI controller restores a quantum computer&\#x27;s laser lock without human intervention in 99.3% of cases. Anthropic says it plans to open-source the standard after completing a safety assessment.

telegram · zaihuapd · Aug 28, 01:38

**「Background」** Anthropic is the developer of the Claude family of AI models and has been expanding beyond conversational AI into agentic systems that take actions in the world. The Model Hardware Standard \(MHS\) is a proposed shared specification that defines how AI agents can safely and consistently interface with physical laboratory and industrial equipment, such as microscopes, liquid handlers, and robotic arms. The research preview makes this specification available to an initial group of scientific research labs and advanced manufacturers, with Anthropic planning to open-source the standard after completing a safety review. This builds on prior efforts to give AI models standardized, secure control over real-world hardware rather than requiring bespoke integrations for each device.

**「Impact」** Affected labs and automation teams can now pilot MHS at minute-scale integration effort, although broader adoption awaits the open-source release tied to Anthropic&\#x27;s safety review.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/news/model-hardware-standard-research-preview">Previewing the Model Hardware Standard \ Anthropic</a></li>
<li><a href="https://blockchain.news/news/anthropic-model-hardware-standard-preview">Anthropic Launches Model Hardware Standard (MHS) Preview</a></li>
<li><a href="https://www.tech360.tv/anthropic-unveils-standard-for-ai-to-control-physical-devices-2026-28-08">Anthropic Unveils Standard for AI to Control Physical... | tech360tv</a></li>

</ul>
</details>

**Tags**: `#Anthropic`, `#AI agents`, `#hardware control`, `#open source`, `#quantum computing`

---

<a id="item-tech-news-12"></a>
### [OpenAI Is Developing a Persistent Mode for Its Codex CLI Agent](https://www.wired.com/story/openai-is-developing-a-persistent-ai-agent/) ⭐️ 7.0/10

OpenAI is reportedly developing a persistent mode for its command-line Codex agent, according to code reviewed by WIRED. In this mode the agent would keep working until it is put to sleep, unlike current behavior where sessions stop after minutes or hours. A built-in &quot;initiative&quot; setting would let Codex create follow-up tasks after answering requests, operate across sessions, and decide what to work on based on its understanding of the user; changes outside the user&\#x27;s system would still require advance approval. OpenAI confirmed it is testing the feature but said there are no plans for a near-term release.

telegram · zaihuapd · Aug 28, 02:47

**「Background」** OpenAI&\#x27;s Codex is a lightweight coding agent that runs locally as a CLI tool, designed for multi-agent workflows and accessible via ChatGPT as a command center for agentic coding. Currently, Codex sessions stop after a short period, but WIRED&\#x27;s review of unreleased code indicates OpenAI is developing a persistent mode that would let the agent continue working across sessions until explicitly put to sleep.

**「Impact」** If released, the persistent Codex mode would let users hand off multi-session tasks to an autonomous agent that keeps working until told to sleep, while still requiring approval for changes outside the user&\#x27;s system; no release timeline has been announced.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/codex/">Codex in ChatGPT | AI Coding Agents for Software... | OpenAI</a></li>
<li><a href="https://www.thejapantimes.jp/Technology/721802-openai-tests-persistent-mode-for-codex-ai-agent.html">The Japan Times - OpenAI Tests &#x27; Persistent Mode &#x27; for Codex AI Agent</a></li>
<li><a href="https://github.com/openai/codex">GitHub - openai / codex : Lightweight coding agent that runs in your...</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#Codex`, `#AI agents`, `#software engineering`, `#AI tools`

---

<a id="item-tech-news-13"></a>
### [Tencent Hunyuan Releases Hy4 Preview, Slightly Topping Rivals in Blind Test](https://mp.weixin.qq.com/s/ymr3X878B8oa2XP15CH8TQ) ⭐️ 7.0/10

Tencent Hunyuan released the open-source Hy4 preview model, with claimed improvements in software engineering, office analytics, game development, and scientific research. In a blind test of 203 engineering tasks by 163 experts, it scored 2.99 out of 4.00, slightly outperforming GLM-5.3 and Kimi K3. Combined with the Hyra tool, the model advances the lower bound of a 3D Blaschke–Lebesgue geometry problem to 0.41104, leaving about a 2 percent gap to a final proof. The source links to Tencent Hunyuan&\#x27;s blog and Hugging Face page.

telegram · zaihuapd · Aug 28, 06:11

**「Background」** Tencent Hunyuan is Tencent&\#x27;s AI model family; its prior open-source Hy3 preview is a 295B-parameter Mixture-of-Experts \(MoE\) model with 21B active parameters, 3.8B MTP layer parameters, and a 256K context window. The Blaschke–Lebesgue problem, solved in the plane by the Reuleaux triangle, asks for the minimum volume among convex sets of fixed constant width and remains open in dimensions higher than two, as noted in a 2009 arXiv paper. Hy4 preview is presented as the next open-source release in this line and is evaluated against peers such as GLM-5.3 and Kimi K3, while the Hyra result concerns a three-dimensional Blaschke–Lebesgue lower bound.

**「Impact」** Developers and researchers evaluating open-source models now have a new Hy4 preview option that posts a small blind-test edge over two leading peers and demonstrates a concrete mathematical-progress application.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/Tencent-Hunyuan/Hy3-preview">GitHub - Tencent - Hunyuan / Hy 3- preview : Hy3 preview ...</a></li>
<li><a href="https://hy3ai.com/">Hy3 Preview — Tencent Hunyuan 3 Open-Source Model</a></li>
<li><a href="https://en.wikipedia.org/wiki/Blaschke%E2%80%93Lebesgue_theorem">Blaschke–Lebesgue theorem - Wikipedia</a></li>
<li><a href="https://arxiv.org/abs/0906.3217">[0906.3217] On the three-dimensional Blaschke-Lebesgue problem</a></li>

</ul>
</details>

**Tags**: `#Tencent`, `#AI model`, `#open source`, `#LLM benchmark`, `#software engineering`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Nvidia posts $96.2 billion quarterly revenue; CFO gives first one-year-ahead growth guidance](https://mp.weixin.qq.com/s/JTZ_ZJ_pn5vgrI_1QUyWNw) ⭐️ 9.0/10

Nvidia reported fiscal second-quarter revenue of $96.2 billion, up 106% year over year, with data-center revenue of $89 billion, up 117%. CFO Colette Kress gave first-time revenue guidance for fiscal 2028 of about 70% growth, saying the outlook is limited by supply rather than demand.

telegram · zaihuapd · Aug 27, 08:51

**「Background」** The company&\#x27;s data-center business has grown sharply on AI demand; CEO Jensen Huang said AI has reached a turning point, with computing power becoming a source of revenue.

**Tags**: `#Nvidia`, `#earnings`, `#AI`, `#data center`, `#guidance`

---

<a id="item-finance-news-2"></a>
### [Tech earnings beats drive big stock moves; consumer names fall](https://www.cnbc.com/2026/08/27/stocks-making-the-biggest-moves-midday-nvda-okta-hrl-veev.html) ⭐️ 8.0/10

Technology shares led midday gains after quarterly earnings beats: Nvidia rose 9% on adjusted earnings of $2.22 per share and revenue of $96.22 billion, Salesforce jumped 21%, Okta gained more than 27% and CrowdStrike climbed nearly 19%, all versus analyst estimates. Retailers and consumer names slipped, with HP down 4%, Hormel down 9% and Wendy&\#x27;s down 13%.

rss · CNBC Finance · Aug 27, 20:09

**「Background」** The moves followed a heavy day of quarterly earnings reports, with many companies beating Wall Street forecasts and updating guidance for the current period or full year.

**Tags**: `#Earnings`, `#Stock Movers`, `#Technology`, `#Guidance`, `#Analyst Actions`

---

<a id="item-finance-news-3"></a>
### [Premarket movers: Nvidia and Salesforce jump on earnings, Wendy&\#x27;s falls on reported Trian retreat](https://www.cnbc.com/2026/08/27/stocks-making-the-biggest-moves-premarket-nvda-hp-crm-dg-p.html) ⭐️ 7.0/10

Nvidia rose more than 7% in premarket trading after reporting second-quarter adjusted EPS of $2.22 on revenue of $96.22 billion, above LSEG consensus estimates of $2.10 and $92.17 billion. Other notable moves included Salesforce up nearly 12%, Dollar General up 12% after raising full-year EPS guidance to $7.80-$8.00, HP down 11% despite beating fiscal Q3 estimates, and Wendy&\#x27;s down about 15% after a Reuters report that Trian Fund Management does not plan to bid.

rss · CNBC Finance · Aug 27, 14:45

**「Background」** The moves followed quarterly earnings reports in the late-August reporting season; Wendy&\#x27;s had earlier been reported as a potential take-private target of Nelson Peltz&\#x27;s Trian Fund Management.

**Tags**: `#earnings`, `#premarket`, `#stocks`, `#Nvidia`, `#guidance`

---