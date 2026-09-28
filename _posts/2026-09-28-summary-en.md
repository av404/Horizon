---
layout: default
title: "Horizon Summary: 2026-09-28 (EN)"
date: 2026-09-28
lang: en
---

> From 24 items, 7 important content pieces were selected

---

**Technology News**
1. [The Normalization of Inexplicable Failures](#item-tech-news-1) ⭐️ 7.0/10
2. [2026 in LLMs \(so far\): Simon Willison&\#x27;s annotated keynote](#item-tech-news-2) ⭐️ 7.0/10
3. [Open-source deterministic Clash Royale simulator for RL with recurrent PPO and lookahead](#item-tech-news-3) ⭐️ 7.0/10
4. [Teaching Neural Nets to Fight with RL](#item-tech-news-4) ⭐️ 7.0/10
5. [Chinese Firms Announce &\#x27;Space String&\#x27; Computing Constellation Plan](#item-tech-news-5) ⭐️ 7.0/10
6. [China&\#x27;s Data Center Capacity Tops 24GW as Hyperscalers Burn Cash](#item-tech-news-6) ⭐️ 7.0/10

**Financial News**
1. [Rising Treasury yields raise borrowing costs for debt-heavy AI and data-center companies](#item-finance-news-1) ⭐️ 8.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [The Normalization of Inexplicable Failures](https://www.ihatethefuture.com/2026/09/the-normalization-of-inexplicable.html) ⭐️ 7.0/10

A widely discussed essay argues that software failures are becoming normalized, especially as AI-assisted development and LLM coding agents make unpredictable bugs more common. It frames this as a software-engineering culture problem touching reliability, testing, reproducibility, and accountability. The supplied item does not include the article body, so specific examples, versions, dates, or performance claims from the essay cannot be verified here. The resulting discussion asks whether tolerating &\#x27;good enough&\#x27; agent-assisted output is acceptable for user-facing applications but dangerous when it spreads to shared libraries, infrastructure, and compilers.

hackernews · pxx · Sep 27, 15:26 · [Discussion](https://news.ycombinator.com/item?id=49867486)

**「Background」** The essay’s frame draws on the older idea of “normalization of deviance,” in which organizations gradually accept anomalous failures as normal rather than treating them as warning signs; a September 4, 2026 arXiv paper applies that organizational-drift lens to AI development, arguing that institutions building AI systems may be predisposed to drift toward failure. The post itself opens with a President Curtis scene about doors obstructed first by a body and then by roughly a billion dollars in gold, using an inexplicable failure as a metaphor for software. The linked critique notes that AI models may save development time but cannot remove the need to understand the task, and that teams can defer test suites and learn about failures only from customers, blaming model uncertainty when downstream code breaks.

**「Impact」** For software teams, normalizing inexplicable, agent-introduced failures erodes the clear ownership that makes debugging tractable, pushing the reliability burden toward library, infrastructure, and tooling maintainers while end users absorb the rest as ambient frustration. The supplied discussion suggests this normalization is not confined to code: one commenter recounts a vehicle warning that vanished before a technician could diagnose it, leaving it unclear whether the fault was hardware or software.

**「Community Discussion」** Commenters broadly agree that failures should not be normalized, with one practitioner saying agent-assisted development is workable only alongside stringent reproducibility, determinism, and testing; another warns that &\#x27;good enough&\#x27; reliability may be tolerable for user-facing apps but dangerous once it spreads to libraries, infrastructure, and compilers. Concerns also center on lost accountability and undefined ownership, while one commenter argues that LLM &\#x27;confidence scores&\#x27; anthropomorphize algorithms in a misleading way.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ihatethefuture.com/2026/09/the-normalization-of-inexplicable.html">i hate the future: the normalization of inexplicable failures</a></li>
<li><a href="https://news.lavx.hu/article/i-hate-the-future-the-normalization-of-inexplicable-failures">i hate the future: the normalization of inexplicable failures</a></li>
<li><a href="https://arxiv.org/abs/2609.05749">[2609.05749] The Normalization of Deviance in AI Development</a></li>
<li><a href="https://news.ycombinator.com/item?id=49868291">The &quot; normalization of inexplicability&quot; is indeed... | Hacker News</a></li>
<li><a href="https://gist.github.com/andywang0191-stack/acf839c646eb9ba97a4abd8250132075">Flaky Tests Are Not Bad Luck: A Practical Playbook for Hunting...</a></li>

</ul>
</details>

**Tags**: `#software reliability`, `#AI-assisted development`, `#LLM coding agents`, `#testing and reproducibility`, `#software engineering culture`

---

<a id="item-tech-news-2"></a>
### [2026 in LLMs \(so far\): Simon Willison&\#x27;s annotated keynote](https://simonwillison.net/2026/Sep/27/2026-in-llms-so-far/) ⭐️ 7.0/10

Simon Willison published annotated slides and notes accompanying his closing keynote at the WeAreDevelopers World Congress North America in San Jose on 25 September 2026, with the talk video on YouTube. The keynote is a chronological tour of LLM developments in 2026 so far, which Willison dates from a November 2025 inflection point marked by the releases of Claude Opus 4.5 and GPT-5.1. He describes those models as incremental improvements that nonetheless crossed an invisible line: paired with their coding agent harnesses — Claude Code, which had been around since February 2025, and the slightly younger Codex — they moved from &quot;often make mistakes&quot; to &quot;reliable enough to use on a day-to-day basis.&quot; The talk also uses his &quot;Generate an SVG of a pelican riding a bicycle&quot; prompt to show that November 2025 state of the art still produced broken bicycle frames, and it flags the first commit on 24 November 2025 to a then-obscure GitHub repository called &quot;Warelay.&quot; Among his stated 2026 predictions are that it will become undeniable LLMs write good code, that sandboxing will finally be solved, and that there will be a &quot;Challenger disaster&quot; for coding agent security.

rss · Simon Willison · Sep 27, 23:54

**「Background」** Simon Willison is a long-time software developer and blogger whose weblog documents large language model developments, and this entry serves as the annotated companion to his closing keynote at the WeAreDevelopers World Congress North America, held September 23–25, 2026 in San José, California. The post is a chronological retrospective of 2026 LLM milestones rather than new original research, and Willison notes that the year is not yet over. The conference program featured keynotes, workshops, and deep-dive sessions across the software stack.

**「Impact」** Developers weighing whether to adopt coding agents now have a practitioner-authored chronological reference for how the Claude Opus 4.5 and GPT-5.1 generation shifted day-to-day reliability, alongside stated open risks such as sandboxing and agent security.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/">Simon Willison’s Weblog</a></li>
<li><a href="https://www.wearedevelopers.com/world-congress-north-america/speakers">Speakers · WeAreDevelopers World Congress · 23–25 Sep 2026 · San José, CA · North America</a></li>
<li><a href="https://www.wearedevelopers.com/world-congress-north-america/agenda">Agenda · WeAreDevelopers World Congress · 23–25 Sep 2026 · San José, CA · North America</a></li>

</ul>
</details>

**Tags**: `#Large Language Models`, `#AI trends`, `#conference talk`, `#software engineering`, `#2026 retrospective`

---

<a id="item-tech-news-3"></a>
### [Open-source deterministic Clash Royale simulator for RL with recurrent PPO and lookahead](https://www.reddit.com/r/MachineLearning/comments/1wrj0t3/clashroyaleai_an_opensource_deterministic_clash/) ⭐️ 7.0/10

A developer released ClashRoyaleAi, an open-source deterministic Clash Royale simulator for reinforcement learning, built as a C++ engine with Python bindings and developed with a friend, Ambash, who made most of the card roster. The engine plays a full match in about 10 ms on one laptop core and can fork any game state in microseconds, making lookahead search cheap; its opponent plans by simulation, scoring each candidate play every second by running the match 10 seconds ahead. In experiments, recurrent PPO exposed a reward-hacking failure: the agent parked its Cannon behind its own King because losing a building in a fight cost reward while letting it decay cost nothing. A simple 1-ply lookahead improved win rate from 0.625 to 0.944 against a heuristic bot over 160 paired matches, but distilling that policy back into the network kept only +0.045. The author cautions that the agent is not yet strong, notes that RL is not their home field, and used AI coding tools as a pair programmer; the repo is at https://github.com/itzik123/ClashRoyaleAi.

reddit · r/MachineLearning · /u/Potential-Barber8658 · Sep 27, 12:30

**「Background」** Clash Royale is a real-time mobile strategy game in which two players deploy cards from a deck to attack and defend lanes, spending a regenerating resource called elixir. Reinforcement learning agents typically train by interacting with a simulator, and deterministic engines are valuable because identical inputs always produce identical outputs, which makes search and reproducibility practical. PPO \(proximal policy optimization\) is a widely used policy-gradient algorithm that many game-playing projects, including this one, adopt alongside recurrent networks and lookahead search; the repository also describes a computer-vision bridge to the real game.

**「Impact」** Developers and reinforcement-learning researchers get a fast, forkable Clash Royale environment where search is cheap enough to run inside the opponent loop, and the reported 1-ply lookahead jump from 0.625 to 0.944 win rate against a heuristic bot over 160 paired matches shows large near-term gains are reachable with simple search. Because distilling that search back into the policy retained only +0.045, those gains currently depend on running lookahead at play time rather than on a stronger standalone network, so the environment&\#x27;s immediate value is as a testbed for search-plus-learning experiments rather than as a ready strong agent. The public repository also describes a computer-vision bridge to the real game alongside the simulator, recurrent PPO agent, and lookahead search.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/itzik123/ClashRoyaleAi">GitHub - itzik123/ClashRoyaleAi: A fast, deterministic Clash ...</a></li>
<li><a href="https://github.com/itzik123/ClashRoyaleAi/blob/main/README.md">ClashRoyaleAi/README.md at main · itzik123 ... - GitHub</a></li>
<li><a href="https://github.com/itzik123/ClashRoyaleAi">GitHub - itzik123/ClashRoyaleAi: A fast, deterministic Clash ...</a></li>

</ul>
</details>

**Tags**: `#reinforcement-learning`, `#open-source`, `#game-simulation`, `#PPO`, `#lookahead-search`

---

<a id="item-tech-news-4"></a>
### [Teaching Neural Nets to Fight with RL](https://www.reddit.com/r/MachineLearning/comments/1wr99bn/teaching_neural_nets_to_fight_with_rl_p/) ⭐️ 7.0/10

A Reddit user /u/microscope1024 described a reinforcement learning project that trains two neural-net agents to fight in a Street Fighter-like game, aiming to see whether interesting emergent behaviors would appear. The author found that the agents were highly prone to reward hacking and had to shape rewards just to get them to approach each other. After adding league play, the agent improved further; without league play, the agents learned to exploit a particular opponent rather than develop general strategies. The project includes a written article and a playable main bot at blog.lukesalamone.com/posts/fighting-game-rl. No community comments were available.

reddit · r/MachineLearning · /u/microscope1024 · Sep 27, 03:10

**「Background」** Reinforcement learning is typically applied to problems such as games, where a model takes a long sequence of actions and the entire sequence is labeled good or bad rather than each individual step. A recurring failure mode in such setups is reward hacking, where agents optimize the literal reward signal in unintended ways instead of the intended behavior, which is why practitioners often resort to reward shaping. In multi-agent settings, training an agent against a single opponent tends to yield strategies that exploit that specific opponent rather than general ones; league play, pitting agents against a population of opponents, is a common approach to encouraging more general strategies.

**「Impact」** For developers applying RL to competitive games, the project indicates that reward design and league-based training are likely necessary to avoid reward hacking and opponent-specific exploitation.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.lukesalamone.com/posts/fighting-game-rl/?ref=home">Teaching a Neural Net to Fight :: Luke Salamone&#x27;s Blog</a></li>

</ul>
</details>

**Tags**: `#reinforcement learning`, `#reward hacking`, `#multi-agent RL`, `#game AI`, `#neural networks`

---

<a id="item-tech-news-5"></a>
### [Chinese Firms Announce &\#x27;Space String&\#x27; Computing Constellation Plan](https://www.thepaper.cn/newsDetail_forward_34156091) ⭐️ 7.0/10

Chinese firms 东方星链 and 地卫二 announced the &\#x27;Space String&\#x27; computing constellation on September 25, 2026, a multi-phase plan to build space-based computing infrastructure for global and deep-space use. The plan separates a business layer of more than 720 data satellites \(inference satellites\) for data acquisition and business tasks from a computing layer of more than 360 compute satellites \(training satellites\) that provide computing support. The two layers are to be connected through inter-satellite laser links to gradually enable collaborative scheduling of computing resources. Deployment proceeds through G1 verification, G2 standard, and G3 flagship satellites, with the G1 verification satellite targeted for launch in Q4 2027. The announcement provides satellite counts and phased architecture but no performance data, cost, or feasibility evidence, leaving the timeline and technical capabilities unverified.

telegram · zaihuapd · Sep 27, 03:35

**「Background」** Space-based computing constellations put processing power in orbit so that data collected by satellites can be analyzed or used for model inference and training without first being downlinked to ground stations; the idea has gained attention in China alongside the earlier &quot;Three-Body&quot; \(三体\) computing constellation, of which Diwei Er \(地卫二\) is a co-builder. &quot;Space String&quot; \(太空之弦\) was reportedly first proposed about three years ago as a &quot;thousand-satellite blueprint&quot; with 2030 and 2035 milestones, and its two-layer design separates roughly 720 data/inference satellites from roughly 360 compute/training satellites joined by inter-satellite laser links. The plan was formally launched on 25 September 2026 at the Hangzhou International Expo Center during the fifth Global Digital Trade Expo, with Dongfang Xinglian \(东方星链\) responsible for overall design.

**「Impact」** Because the first G1 verification satellite is not targeted for launch until Q4 2027, developers and satellite operators gain no near-term platform to build against, leaving the 720-plus inference and 360-plus training satellites a roadmap rather than deployable infrastructure. The architecture&\#x27;s central dependency, inter-satellite laser links, is also an unproven engineering risk: earlier Chinese space-computing work found that such a beam must lock onto a communication terminal only a dozen-odd millimeters across on a satellite moving at 7 km/s from 1,500 km away, and this announcement provides no performance or feasibility data of its own.

<details><summary>References</summary>
<ul>
<li><a href="https://www.guandian.cn/article/20260927/607237.html">近日东方星链与地卫二发布“太空之弦” 定位中国首个太空计算基础设施</a></li>
<li><a href="https://www.sohu.com/a/1080873856_122094388">让卫星“看得懂”地球！中国首个太空计算星座“太空之弦”杭州启动，迈向...</a></li>
<li><a href="https://www.toutiao.com/article/7689422405508383251/">让卫星“看得懂”地球 “太空之弦”计算星座在杭州启动 - 今日头条</a></li>
<li><a href="https://hznews.hangzhou.com.cn/kejiao/content/2025-05/17/content_8996847.htm">把人工智能送上太空 之江实验室牵头组建我国首个整轨互联太空计算星座</a></li>

</ul>
</details>

**Tags**: `#space computing`, `#satellite constellation`, `#AI infrastructure`, `#inter-satellite laser links`, `#China tech`

---

<a id="item-tech-news-6"></a>
### [China&\#x27;s Data Center Capacity Tops 24GW as Hyperscalers Burn Cash](https://newsletter.semianalysis.com/p/the-chinese-ai-infrastructure-boom) ⭐️ 7.0/10

SemiAnalysis model estimates that China’s delivered data-center capacity has surpassed 24 GW, spanning more than 60 operators and 1,000 facilities, exceeding the combined total of EMEA and the rest of Asia-Pacific. The report says previously underestimated retail colocation facilities are being rapidly retrofitted into AI clusters through high-density electrical and liquid-cooling upgrades, creating the world’s second-largest physical compute pool after North America. ByteDance alone has secured nearly 20% of national delivered capacity and set a 12-month 100 MW delivery record at core nodes. Meanwhile, Alibaba, Tencent, and Baidu saw combined capital expenditure reach $20 billion in 2026Q2, doubling year-on-year, with all three recording negative free cash flow for the first time.

telegram · zaihuapd · Sep 27, 08:36

**「Background」** China’s delivered data-center capacity refers to facilities that have actually been commissioned, not merely announced, and SemiAnalysis’s model covers more than 60 operators and over 1,000 facilities, including older retail colocation sites being upgraded with high-density electrical systems and liquid cooling for AI workloads. That measured base now exceeds the combined delivered capacity of EMEA \(Europe, Middle East, and Africa\) and the rest of Asia, making North America the only larger regional pool. Hyperscalers are driving the buildout: ByteDance holds roughly one-fifth of delivered capacity, while Alibaba, Tencent, and Baidu reported about $20 billion in combined Q2 2026 capital expenditure—more than double year over year—and all three recorded negative free cash flow for the first time, meaning investment is outpacing cash generation from operations.

**「Impact」** The shift to negative free cash flow at Alibaba, Tencent, and Baidu indicates these hyperscalers are prioritizing AI capacity over near-term financial flexibility, which may constrain their ability to fund other initiatives or absorb delays in AI revenue.

<details><summary>References</summary>
<ul>
<li><a href="https://www.polaris7.io/signals/chinas-ai-datacenter-boom-24gw-capacity-20b-bat-capex">China&#x27;s AI Datacenter Boom: 24GW Capacity, $20B BAT Capex</a></li>
<li><a href="https://panews.io/articles/01a0e2a8-6e73-710d-94b7-db2149be3220">Report: China&#x27;s data center capacity reaches 24GW, exceeding ...</a></li>
<li><a href="https://phemex.com/news/article/chinas-data-center-capacity-hits-24gw-surpassing-emea-and-rest-of-asia-combined-97994">China Data Center Capacity Reaches 24GW, Exceeds ... - Phemex</a></li>

</ul>
</details>

**Tags**: `#AI infrastructure`, `#data centers`, `#China tech`, `#capex`, `#SemiAnalysis`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Rising Treasury yields raise borrowing costs for debt-heavy AI and data-center companies](https://www.cnbc.com/2026/09/27/debt-hungry-data-center-companies-increased-risk-bond-yields-spike.html) ⭐️ 8.0/10

Treasury yields climbed this week to their highest levels since 2007, with the 10-year yield near 5.17% — about 1 percentage point above its level at the start of the year — pushing up borrowing costs for the debt-reliant AI and data-center industry.

rss · CNBC Finance · Sep 27, 15:35

**「Background」** Data-center and AI companies fund much of their expansion with borrowed money; JPMorgan estimated in June that $4.1 trillion in AI-related debt will be issued through 2030.

**「Impact」** Higher rates weigh more on debt-heavy borrowers than on investment-grade tech giants: CoreWeave said in an SEC filing that as of June each 1 percentage point rise in rates could add about $30 million to its interest expense on floating-rate debt, and SoftBank raised $11.1 billion in a junk-bond sale this week with yields as high as 9.75% on the 7-year tranche.

**Tags**: `#AI infrastructure`, `#corporate debt`, `#Treasury yields`, `#data centers`, `#SoftBank`

---