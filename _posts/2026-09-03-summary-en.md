---
layout: default
title: "Horizon Summary: 2026-09-03 (EN)"
date: 2026-09-03
lang: en
---

> From 42 items, 11 important content pieces were selected

---

**Technology News**
1. [Meta Releases Muse Spark 1.3, a Low-Cost Near-SOTA Model](#item-tech-news-1) ⭐️ 8.0/10
2. [Google&\#x27;s Gemini 3.8 Flash and Flash Cyber are fast, cheap and strong in early tests](#item-tech-news-2) ⭐️ 8.0/10
3. [Investigation: 215k AI-generated &\#x27;best software&\#x27; pages drive Perplexity citations](#item-tech-news-3) ⭐️ 8.0/10
4. [Jasper Research releases open text-to-image training cookbook and dataset](#item-tech-news-4) ⭐️ 8.0/10
5. [FBI Probing Nexus Dark Web Service Selling 153M Driver&\#x27;s License Scans](#item-tech-news-5) ⭐️ 8.0/10
6. [Google defeats U.S. bid to force ad tech breakup](#item-tech-news-6) ⭐️ 7.0/10
7. [Claude’s revised prompts restrict song lyrics and copyrighted characters](#item-tech-news-7) ⭐️ 7.0/10
8. [Paint.NET&\#x27;s Claude-written Direct2D rewrite powers experimental WINE/Linux support](#item-tech-news-8) ⭐️ 7.0/10
9. [Open-source AI detectors largely fail at 0.5% false-positive rate](#item-tech-news-9) ⭐️ 7.0/10

**Financial News**
1. [Nepal’s tourism industry faces hard hit after Himalayan glacial floods](#item-finance-news-1) ⭐️ 8.0/10
2. [Premarket Movers: Dell Jumps, MongoDB Slips, Vertiv Announces Acquisition](#item-finance-news-2) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Meta Releases Muse Spark 1.3, a Low-Cost Near-SOTA Model](https://developer.meta.com/ai/models/muse-spark/) ⭐️ 8.0/10

Meta has released Muse Spark 1.3, a low-cost AI model that approaches state-of-the-art performance, according to the linked Meta research blog post and community reports. Commenters report a DeepSWE benchmark score of 75.4, described as the best so far and ahead of Google&\#x27;s Gemini 3.8 Flash, while the model remains very cheap to run. In a practical test, one developer generated an SVG via the llm CLI for 4.2266 cents in 38 seconds, with visibly better output than version 1.2. Meta also offers a contributor variant with explicit training-on-data pricing, which commenters praised for transparency.

hackernews · bvaldivielso · Sep 2, 19:35 · [Discussion](https://news.ycombinator.com/item?id=49541256)

**「Background」** Muse Spark is Meta&\#x27;s family of large language models developed by Meta Superintelligence Labs, first introduced in April 2026 and launched as Muse Spark 1.1 in July 2026. Muse Spark 1.3, the latest release, is designed for multimodal reasoning, coding, and agentic tasks, with enhancements like improved long-horizon collaboration and tool use. Meta also offers a separate pricing tier that explicitly allows training on user data, which has drawn attention to how much model providers value access to user tokens.

**「Impact」** Developers who accept Meta&\#x27;s data-training terms gain access to a very low-cost, near-state-of-the-art model for coding and agent tasks, and the reported DeepSWE score suggests Muse Spark 1.3 is materially more capable than the already popular 1.2.

**「Community Discussion」** Commenters were largely enthusiastic about price-performance: a practical SVG test showed clear quality gains from 1.2 to 1.3, the strong DeepSWE result and low cost were highlighted, and the explicit contributor-pricing model was praised as transparent. Some also noted broader context around Meta&\#x27;s policies and practices, but the model&\#x27;s capability and value drew the most attention.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Muse_Spark">Muse Spark - Wikipedia</a></li>
<li><a href="https://research.meta.ai/blog/introducing-muse-spark-1-3">Introducing Muse Spark 1.3 | Meta AI Research</a></li>
<li><a href="https://developer.meta.com/ai/models/muse-spark/">Muse Spark 1.3 | Meta</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Meta`, `#Muse Spark`, `#benchmarks`, `#machine learning`

---

<a id="item-tech-news-2"></a>
### [Google&\#x27;s Gemini 3.8 Flash and Flash Cyber are fast, cheap and strong in early tests](https://blog.google/innovation-and-ai/models-and-research/gemini-models/3-8-flash-and-3-8-flash-cyber/) ⭐️ 8.0/10

Google has released the Gemini 3.8 Flash and 3.8 Flash Cyber model pair, announced on the official blog with a DeepMind model card. Early community testing emphasizes speed and cost: one commenter produced a working HTML/JavaScript demo in 13 seconds for 1.8 cents, and a high-effort testing run was about 8.97 cents. The model tops the DeepSwe leaderboard ahead of Opus 5 and matches Opus 5 medium on Artificial Analysis&\#x27; intelligence score of 59, suggesting strong quality for a Flash-tier model. Because the Gemini family also accepts audio and video input, while OpenAI and Anthropic flagship models remain image-only, Flash models are positioned as a cheap route to multimodal media analysis.

hackernews · bratao · Sep 2, 15:12 · [Discussion](https://news.ycombinator.com/item?id=49537553)

**「Background」** The Gemini Flash line consists of smaller, cost-efficient versions of Google&\#x27;s Gemini models, aimed at developers who need low-latency outputs for coding and agentic workloads; Gemini 3.7 Flash is the direct predecessor with the same output pricing as the new 3.8 Flash. The 3.8 Flash Cyber variant is a specialized release aimed at cybersecurity use, with Google initially restricting it to trusted defenders through its Fairwind Program and highlighting capabilities such as autonomous vulnerability discovery.

**「Impact」** Developers building fast web-prototype or multimodal analysis flows can now use Gemini 3.8 Flash at low cost with benchmark results rivaling more expensive models. Anyone relying on low thinking-effort outputs on earlier Gemini Flash releases should re-test on 3.8, since one commenter reported a possible regression.

**「Community discussion」** Community response is enthusiastic but not unanimous, with praise focusing on speed, cost, benchmark position and the differentiator of audio/video input. One hands-on comparison also suggested that low thinking-effort quality may have regressed in 3.8 relative to 3.7.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/3-8-flash-and-3-8-flash-cyber/">Introducing Gemini 3 . 8 Flash and 3 . 8 Flash Cyber</a></li>
<li><a href="https://www.datacamp.com/blog/gemini-3-8-flash-cyber">Gemini 3 . 8 Flash : Features, Benchmarks, and Pricing | DataCamp</a></li>

</ul>
</details>

**Tags**: `#Gemini`, `#AI models`, `#Google`, `#LLMs`, `#machine learning`

---

<a id="item-tech-news-3"></a>
### [Investigation: 215k AI-generated &\#x27;best software&\#x27; pages drive Perplexity citations](https://trellner.com/reports/manufactured-sources-behind-ai-recommendations/) ⭐️ 8.0/10

A report from trellner.com identifies three websites that generated 215,128 AI-authored &quot;best software&quot; pages and shows that Perplexity&\#x27;s AI answers frequently cite these manufactured sources. The investigation exposes how AI-generated SEO content can influence the references that AI assistants rely on for software recommendations. It describes a concrete failure mode in AI-assisted software discovery, where spam sites appear to be treated as authoritative enough to shape search results and model outputs. The findings also raise broader concerns about LLMs training on or favoring AI-generated text, which can degrade trust in AI systems and search reliability.

hackernews · jakobgreenfeld · Sep 2, 13:59 · [Discussion](https://news.ycombinator.com/item?id=49536375)

**「Background」** The investigation by Trellner Research examined software-category recommendation queries answered by AI assistants, measuring which websites supplied the cited sources. It found that across 380 software categories, 59.8% of the sources behind grounded AI recommendations come from outside the 100,000 most-visited websites, and several of the most-cited sites appear designed to be read by AI models rather than by people. The full dataset and scripts behind the report are publicly available, providing evidence for claims about AI-generated spam pages influencing AI responses.

**「Impact」** Perplexity’s retrieval system has no mechanism to down-rank AI-generated pages, meaning its answers can cite AI-produced &\#x27;best software&\#x27; spam and expose users to inaccurate or fabricated recommendations.

**「Community Discussion」** Commenters shared related evidence: one said Claude consistently prefers its own generated code over human refactoring, and both Claude and Codex routinely cite generated websites. Another described LLMs confidently recommending a nonexistent &quot;Foobar square&quot; for street food, while a Perplexity user said the service seems to have optimized for speed at the cost of reference quality.

<details><summary>References</summary>
<ul>
<li><a href="https://trellner.com/reports/manufactured-sources-behind-ai-recommendations/">Three sites made 215,128 &quot;best software&quot; pages for AI. Perplexity cites them | Trellner Research</a></li>
<li><a href="https://trellner.com/">Trellner Research | Independent brand and market research</a></li>
<li><a href="https://futurism.com/the-byte/perplexity-citing-ai-generated-spam">Perplexity Is Already &quot;Citing&quot; Error-Filled AI-Generated Spam</a></li>
<li><a href="https://www.forbes.com/sites/rashishrivastava/2024/06/26/search-startup-perplexity-increasingly-cites-ai-generated-sources/">Garbage In, Garbage Out: Perplexity Spreads Misinformation From Spammy AI Blog Posts</a></li>
<li><a href="https://www.aiqnahub.com/perplexity-fake-citations-how-to-fix-them-in-2026/">Perplexity Fake Citations: How to Fix Them in 2026 - AI Q&amp;A Hub</a></li>

</ul>
</details>

**Tags**: `#AI-generated content`, `#Perplexity`, `#search quality`, `#spam`, `#LLM reliability`

---

<a id="item-tech-news-4"></a>
### [Jasper Research releases open text-to-image training cookbook and dataset](https://www.reddit.com/r/MachineLearning/comments/1w5c9rd/detailed_explanation_of_how_to_create_a/) ⭐️ 8.0/10

Jasper Research released a cookbook, dataset, and codebase for training text-to-image models from scratch. The cookbook shares the full reasoning and intermediate results, aiming to show how frontier labs build such systems. It includes the Monet Dataset of 100M image-text pairs and a tiny trainable model in the nano-t2i codebase, so engineers can train a text-to-image model from scratch. The resource is intended for deep-dive learners and those curious about production-oriented text-to-image pipelines.

reddit · r/MachineLearning · /u/dh7net · Sep 2, 14:40

**「Background」** Text-to-image models typically require massive curated datasets and substantial compute, which makes end-to-end training difficult to reproduce. This release lowers that barrier by packaging a 100M-image dataset, a compact codebase, and concrete explanations of architecture and training decisions.

**「Impact」** ML practitioners can now follow a complete, open recipe to train and evaluate a small text-to-image model from scratch, reusing the provided dataset and code rather than assembling components from separate sources.

**Tags**: `#text-to-image`, `#deep learning`, `#open source`, `#training dataset`, `#AI education`

---

<a id="item-tech-news-5"></a>
### [FBI Probing Nexus Dark Web Service Selling 153M Driver&\#x27;s License Scans](https://krebsonsecurity.com/2026/09/fbi-probes-service-selling-153m-drivers-licenses/) ⭐️ 8.0/10

KrebsOnSecurity reports that the FBI is investigating Nexus, a dark web identity-data service claiming to hold and sell more than 153 million digital scans of U.S. and Canadian driver&\#x27;s licenses. The scans include sensitive details such as names, addresses, and birth dates, making them valuable for identity theft. Nexus may have obtained the files from older breaches at car dealerships and insurance companies, but officials have not yet confirmed the specific source or the number of affected people. If the service&\#x27;s claims are accurate, the exposed population could be substantial, though the full impact remains unverified.

telegram · zaihuapd · Sep 2, 09:31

**「Background」** Driver&\#x27;s license scans are high-value identity documents because they combine a person&\#x27;s name, address, date of birth, and often other identifying details into one verified credential. Dark web marketplaces frequently sell such records after breaches, enabling account takeover, loan fraud, and synthetic identity creation.

**「Impact」** If Nexus&\#x27;s inventory is real, tens of millions of U.S. and Canadian motorists could face increased risk of identity theft and fraud, though the breach&\#x27;s origin and the exact list of affected residents have not been officially confirmed.

**Tags**: `#cybersecurity`, `#data breach`, `#privacy`, `#identity theft`, `#dark web`

---

<a id="item-tech-news-6"></a>
### [Google defeats U.S. bid to force ad tech breakup](https://www.nytimes.com/2026/09/02/technology/google-ad-tech-remedies.html) ⭐️ 7.0/10

Google has defeated the U.S. government&\#x27;s antitrust suit seeking to force a sale of its ad tech business, avoiding a court-ordered breakup. The decision, reported on Sept. 2, 2026, ends the government&\#x27;s bid to make Google divest that business through a monopolization case. Google&\#x27;s ad tech business brought in about $30 billion last year, or roughly 8 percent of Alphabet&\#x27;s revenue, but its ad tech revenue has declined for 16 straight quarters and analysts estimate it accounts for less than 1 percent of Alphabet&\#x27;s profit. The outcome spares Google from a breakup while leaving broader regulatory debates about tech monopolies unresolved.

hackernews · donohoe · Sep 2, 14:46 · [Discussion](https://news.ycombinator.com/item?id=49537131)

**「Background」** Google’s ad tech business includes its Ad Manager platform for programmatic advertising, which accounted for about 4.1% of Google’s overall revenue and 1.5% of its operating profit in 2020, though more recent figures were redacted from court documents. The U.S. Department of Justice had sued over that business, arguing that Google monopolized ad technology markets and sought to force a sale. A federal court sided with Google in September 2026, rejecting the government’s request for a breakup.

**「Impact」** The ruling means Google avoids a court-ordered sale or breakup of its ad tech business and can keep operating the ad exchange and related tools that connect publishers with marketers, preserving a central part of the digital media economy. This is a major win for Google that removes the immediate threat of forced divestiture of its ad tech operations.

**「Community Discussion」** Commenters were skeptical of the outcome, with some questioning the narrow definition of &quot;ad tech&quot; and why a business with such a small profit share drew a major suit, while others proposed alternatives such as progressive monopoly taxes. Several argued that corporate mergers and breakups are enforced asymmetrically, making it far harder to undo a merger than to complete one, and that large tech companies reliably preempt major antitrust remedies.

<details><summary>References</summary>
<ul>
<li><a href="https://money.usnews.com/investing/news/articles/2026-09-02/google-defeats-us-bid-to-force-ad-tech-sale">Google Defeats US Bid to Force Ad Tech Sale</a></li>
<li><a href="https://gokhshtein.com/news/2026-09-02-google-defeats-us-bid-to-force-ad-tech-sale">Google Wins Ad Tech Antitrust Battle; GOOGL Reprices... | Gokhshtein</a></li>
<li><a href="https://nypost.com/2026/09/02/business/google-escapes-bid-to-force-sale-of-ad-tech-business-in-doj-defeat/">Google escapes bid to force sale of ad tech business in DOJ defeat</a></li>
<li><a href="https://www.thewrap.com/industry-news/public-policy-legal/google-ad-tech-breakup-antitrust-ruling/">Google Avoids Breakup of Ad Tech Business in Antitrust Ruling - TheWrap</a></li>

</ul>
</details>

**Tags**: `#antitrust`, `#google`, `#ad-tech`, `#regulation`, `#technology-industry`

---

<a id="item-tech-news-7"></a>
### [Claude’s revised prompts restrict song lyrics and copyrighted characters](https://simonwillison.net/2026/Sep/2/claudes-new-system-prompt/) ⭐️ 7.0/10

Anthropic has reorganized the system prompts it publishes for Claude consumer apps—Claude.ai and the mobile apps, but not Claude Cowork or Claude Code—into an index page and per-model pages, and those docs pages can now be retrieved as Markdown by appending .md. A notable new policy section forbids Claude from reproducing song lyrics, poems, or passages from books and articles in whole or in part, including refraining from providing closing lines, choruses, melodies, or lines pasted one at a time; after declining once, Claude continues declining narrower or reworded versions for the rest of the conversation and offers to describe or analyze the work instead, while works first published before 1929 may be allowed only when Claude reliably knows the date. The related visual guidance forbids generating copyrighted artworks, logos, characters, mascots, or brand figures using generated code such as SVG, canvas, CSS, HTML mockups, plotting scripts, or ASCII art, with an explicitly worked Sonic-the-hedgehog refusal example. Simon Willison highlights the lyric restriction as appearing days after reports that Sony Music Publishing and Warner Chappell are suing Anthropic over training on databases of song lyrics, and demonstrates how the reorganized documentation makes the Fable 5.1 prompt changes easy to diff.

rss · Simon Willison · Sep 2, 14:16

**「Background」** Anthropic publishes the system prompts used by its Claude consumer applications, sharing both current and historical versions so observers can track how the model&\#x27;s instructions evolve. The platform documentation site is designed for LLM use, and adding .md to a page URL returns its content as Markdown, which enables direct comparison of prompt changes across model versions such as Fable 5.1 and Haiku 4.5.

**「Impact」** Developers and practitioners can now easily diff historical system-prompt changes through Anthropic&\#x27;s Markdown endpoints, while Claude.ai and mobile users making lyric or copyrighted-character requests can expect explicit refusals followed by offers to describe or analyze the work or to produce an original alternative.

**Tags**: `#Anthropic`, `#Claude`, `#system prompts`, `#AI policy`, `#copyright`

---

<a id="item-tech-news-8"></a>
### [Paint.NET&\#x27;s Claude-written Direct2D rewrite powers experimental WINE/Linux support](https://simonwillison.net/2026/Sep/2/rick-brewster/) ⭐️ 7.0/10

Rick Brewster, author of Paint.NET, announced that the application now includes an internal, from-scratch, clean-room reverse-engineered rewrite of Microsoft&\#x27;s Direct2D API to enable extremely experimental WINE/Linux support. The rewrite, written by Anthropic&\#x27;s Claude and living in PaintDotNet.Windows.Direct2D1.Managed.dll, is triggered by launching Paint.NET with the /wine argument. Brewster says Direct2D was always the biggest hurdle for Paint.NET on WINE and cannot simply be disabled. The new code totals about 180,000 lines, compared with roughly 700,000 lines for the rest of Paint.NET accumulated over more than 20 years, and much of it was &quot;vibe coded&quot; and not thoroughly reviewed. Claude needed significant babysitting around COM reference counting, at one point omitting AddRef equivalents, but also performed clever reverse engineering to figure out formulas for Direct2D&\#x27;s built-in effects library.

rss · Simon Willison · Sep 2, 05:50

**「Background」** Direct2D is a Windows graphics API used heavily by Paint.NET for hardware-accelerated rendering, and WINE&\#x27;s incomplete Direct2D implementation has long prevented Paint.NET from working on Linux/WINE. A clean-room rewrite means the code was independently written to be functionally compatible without copying Microsoft&\#x27;s proprietary implementation, in this case using an AI coding agent to generate the large managed-code shim that calls through to native Direct2D behavior.

**「Impact」** Paint.NET users on Linux can now experiment with running the application under WINE via the /wine switch, but the support is explicitly preliminary and the un-reviewed, AI-written codebase carries real stability risks. Developers and users should treat this as an experimental showcase of large-scale AI-generated code rather than a production-ready compatibility solution.

**Tags**: `#AI-generated code`, `#Reverse engineering`, `#WINE`, `#Direct2D`, `#Software engineering`

---

<a id="item-tech-news-9"></a>
### [Open-source AI detectors largely fail at 0.5% false-positive rate](https://www.reddit.com/r/MachineLearning/comments/1w58erw/most_opensource_ai_detectors_cant_hold_a_05/) ⭐️ 7.0/10

A Reddit-published benchmark of six notable open-source AI text detectors found that most cannot operate at a 0.5% false-positive rate when thresholds are calibrated on a shared set of 6,930 human documents. Using public datasets \(Jabarian &amp; Imas 2025 NBER, Liang 2023 TOEFL essays, 5,000 pre-LLM FineWeb pages, and a 1,060-text frontier set from GPT-5.x, Claude Opus 5, and Gemini 3.x\), recall on raw AI text ranged widely, from 93.2% for tropa-mini down to 0.0% for the old OpenAI RoBERTa detector. Four of the six models effectively could not reach the target FPR: MAGE assigned scores above 0.9999 to 26% of ordinary human web text, while the OpenAI RoBERTa detector had AUC 0.31, worse than chance on modern generators. Performance collapsed on humanizer-paraphrased AI text, with the best detector catching only 42%, and all models flagged non-native English essays more heavily than native essays. The post discloses that one evaluated model is the author&\#x27;s open-weights Apache-2.0 detector and links to public rerunnable data.

reddit · r/MachineLearning · /u/grumpyp2 · Sep 2, 12:04

**「Background」** AI-text detectors are classifiers that try to distinguish human writing from LLM-generated text; their threshold determines the false-positive rate \(FPR\), or how often human text is wrongly flagged. Public datasets have been used to expose long-standing bias: Liang et al. \(2023\) found detectors falsely flagged over 61% of non-native TOEFL essays, while Jabarian and Imas \(2025\) studied artificial writing and automated detection more broadly. This benchmark applies a strict 0.5% FPR across open-source detectors using pre-LLM human web pages, modern frontier AI outputs, and humanizer-paraphrased text to test whether these tools are reliable at that operating point.

**「Impact」** This implies current open-source detectors are not reliable for low-tolerance screening tasks such as academic integrity reviews, because hitting a 0.5% false-positive target would miss most paraphrased AI and disproportionately flag non-native writers.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nber.org/papers/w34223">Artificial Writing and Automated Detection | NBER</a></li>
<li><a href="https://gradpilot.com/news/ai-detector-false-positive-rates-compared">AI Detector False Positive Rates Compared (2026) - GradPilot</a></li>

</ul>
</details>

**Tags**: `#AI detection`, `#LLM benchmarks`, `#open source`, `#model evaluation`, `#text classification`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Nepal’s tourism industry faces hard hit after Himalayan glacial floods](https://www.cnbc.com/2026/09/02/nepal-tibet-floods-adventure-tourism-economy.html) ⭐️ 8.0/10

A glacial flood that began in Nepal&\#x27;s Himalayas on Aug. 26 has killed 987 people according to authorities, with nearly 4,250 missing, and is disrupting bookings just before Nepal&\#x27;s main tourism season; Nepal has reportedly estimated rebuilding costs at $4 billion to $5 billion, roughly one-tenth of its economy.

rss · CNBC Finance · Sep 2, 09:23

**「Background」** The disaster came from a glacial collapse that sent ice, rock and meltwater through valleys, damaging roads, bridges and hydropower facilities; local officials say warming is making Himalayan glaciers less stable, and Nepal now needs to redesign tourism infrastructure for extreme weather.

**「Impact」** Tourism businesses in Nepal are seeing cancellations, mainly from European visitors, as the peak season from Sept. 15 to Nov. 15 begins; one Kathmandu hostel owner expects occupancy to fall to 60% from 100% last year.

**Tags**: `#Nepal`, `#tourism`, `#natural disaster`, `#climate change`, `#economic impact`

---

<a id="item-finance-news-2"></a>
### [Premarket Movers: Dell Jumps, MongoDB Slips, Vertiv Announces Acquisition](https://www.cnbc.com/2026/09/02/stocks-making-the-biggest-moves-premarket-vrt-siri-dell-mdb.html) ⭐️ 7.0/10

Premarket trading is sharply mixed after company news: Dell Technologies jumped about 8% after beating Wall Street expectations and lifting its fiscal 2027 forecast, while MongoDB fell about 13% even though its second-quarter earnings and revenue beat analyst forecasts. Vertiv slipped less than 1% after announcing it will buy UtilityInnovation Group for $1.45 billion, plus up to $1.15 billion tied to EBITDA targets.

rss · CNBC Finance · Sep 2, 11:40

**「Background」** Premarket refers to orders placed before the regular US market session, so investors often react overnight to earnings reports, guidance, analyst actions, and deals. Dell credited strength in its artificial intelligence services business for its raised outlook, while MongoDB&\#x27;s decline showed that beating estimates alone does not always satisfy investors.

**Tags**: `#earnings`, `#premarket movers`, `#acquisitions`, `#Dell Technologies`, `#MongoDB`

---