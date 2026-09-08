---
layout: default
title: "Horizon Summary: 2026-09-08 (EN)"
date: 2026-09-08
lang: en
---

> From 33 items, 5 important content pieces were selected

---

**Technology News**
1. [LLM-guided program evolution improves 10 best-known circle-packing solutions](#item-tech-news-1) ⭐️ 8.0/10
2. [Huawei returns to flagship chips after six years with Kirin 9050 Pro](#item-tech-news-2) ⭐️ 8.0/10
3. [China&\#x27;s Supreme Court Issues AI Interpretation Clarifying Deepfake and Algorithmic Pricing Liability](#item-tech-news-3) ⭐️ 8.0/10
4. [Autonomous Bad Apple generation with a 417k-parameter recurrent dynamical system](#item-tech-news-4) ⭐️ 7.0/10

**Financial News**
1. [China injects $54 billion into state banks and insurers; shares fall on smaller-than-expected package](#item-finance-news-1) ⭐️ 8.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [LLM-guided program evolution improves 10 best-known circle-packing solutions](https://www.reddit.com/r/MachineLearning/comments/1w9xlyi/llmguided_program_evolution_improves_10_bestknown/) ⭐️ 8.0/10

A researcher used an LLM to iteratively evolve an optimization algorithm rather than solving circle packing directly, with the LLM proposing algorithmic changes guided by a scoreboard and history of prior attempts. On the Packomania csqv benchmark, the approach improved best-known sum-of-radii results for 10 values of N between 101 and 114, by 2.4 to 5.4%, over 15 iterations, at a total LLM cost of $27.72. Accepting candidates only after independent verification ensured failures were discarded, and Packomania independently accepted the results. The paper is arxiv.org/abs/2609.05093, with code and solutions in github.com/ucsandman/discovery-loop and the benchmark at packomania.com/csqv/csqv.html.

reddit · r/MachineLearning · /u/SIGH\_I\_CALL · Sep 7, 16:54

**「Background」** Circle packing is a classic optimization problem in which circles must be placed inside a container to maximize the sum of their radii, and Packomania maintains a database of best-known solutions for many variants. The csqv variant used here is a recognized benchmark, so a 2-5% improvement on long-standing best-known objectives is noteworthy. LLM-guided program evolution is a technique that treats the search over solver code itself as the optimization target, using an LLM to propose code changes and an independent verifier to score each candidate.

**「Impact」** The accepted results provide fresh baseline configurations for other researchers working on circle-packing benchmarks and illustrate that LLM-driven evolutionary search can produce concrete scientific improvements at relatively tiny compute cost.

**Tags**: `#LLM`, `#program evolution`, `#optimization`, `#circle packing`, `#machine learning`

---

<a id="item-tech-news-2"></a>
### [Huawei returns to flagship chips after six years with Kirin 9050 Pro](https://www.news.cn/20260907/adf46c5c003240d28cc3cf6de54f9b5f/c.html) ⭐️ 8.0/10

Huawei unveiled the Mate XT 2 triple-folding smartphone in Guangzhou on September 7, powered by the new Kirin 9050 Pro chip, which Huawei says is the first high-performance chip using logic-folding technology. The chip stacks logic layers within a single die, much like upgrading from a single-story layout to a duplex, and adds vertical interconnect channels, likened to elevators, to shorten signal paths, reduce latency, and improve performance. This marks the first new Kirin flagship chip at a Huawei flagship launch in six years, following the global Mate40 release. The announcement is reported by Xinhua, but independent technical analysis and benchmark results are not yet available.

telegram · zaihuapd · Sep 7, 08:20

**「Background」** Huawei&\#x27;s Mate 40 global launch marked its last new flagship Kirin chip until now, leaving a roughly six-year gap in major Kirin introductions. The Kirin 9050 Pro introduces LogicFolding architecture, which stacks logic layers within a single die and adds vertical interconnects to reduce signal path length and latency. Huawei touts density improvements over previous generations without relying on EUV lithography, though independent verification and benchmarks have not yet surfaced.

**「Impact」** Mate XT 2 buyers are the first to receive a Huawei flagship with a newly developed Kirin processor since the Mate40 generation, though the performance and design claims currently come only from Huawei and await independent verification.

<details><summary>References</summary>
<ul>
<li><a href="https://www.archyde.com/huawei-unveils-kirin-9050-pro-chip-with-logicfolding-architecture/">Huawei Unveils Kirin 9050 Pro Chip with LogicFolding Architecture – Archyde</a></li>
<li><a href="https://www.techtimes.com/articles/326836/20260907/huawei-kirin-9050-pro-launches-logicfolding-moves-roadmap-silicon.htm">Huawei Kirin 9050 Pro Launches: LogicFolding Moves From Roadmap to Silicon</a></li>
<li><a href="https://www.digitimes.com/news/a20260907VL215/huawei-kirin-flagship-smartphone-launch-performance.html">Huawei Kirin 9050 Pro revives flagship chip launches with reported LogicFolding architecture in Mate XT 2</a></li>

</ul>
</details>

**Tags**: `#Huawei`, `#Kirin`, `#semiconductors`, `#chip architecture`, `#mobile hardware`

---

<a id="item-tech-news-3"></a>
### [China&\#x27;s Supreme Court Issues AI Interpretation Clarifying Deepfake and Algorithmic Pricing Liability](https://www.cnr.cn/news/20260907/t20260907_527806795.shtml) ⭐️ 8.0/10

China&\#x27;s Supreme People&\#x27;s Court on September 7 released a 24-article judicial interpretation on artificial intelligence disputes, organized into five parts addressing AI face-swapping, algorithmic price discrimination, impersonation endorsements, autonomous driving, and intellectual property. The interpretation clarifies that creating identifiable faces or voices with AI without consent may constitute personality rights infringement, and algorithmic price discrimination that harms consumer rights and interests can trigger legal liability. It also states that when AI impersonation is used to endorse products and induce consumption, courts may support claims for punitive damages. Additionally, the interpretation regulates the use of AI to conduct &\#x27;doxxing&\#x27; and &\#x27;human flesh search&\#x27; activities that violate natural persons&\#x27; privacy. The measure gives Chinese courts a more concrete legal basis for deciding civil disputes involving AI technologies.

telegram · zaihuapd · Sep 7, 09:32

**「Background」** In China, judicial interpretations are binding documents issued by the Supreme People&\#x27;s Court to guide lower courts on how to apply existing statutes. This new interpretation builds on provisions in the Civil Code concerning personality rights, privacy, and consumer protection to address AI-specific harms such as deepfakes, algorithmic differentiation, and unauthorized likeness and voice use.

**「Impact」** AI developers, platforms, and companies operating in China now have clearer exposure to civil liability for deepfake content, algorithmic price bias, and AI impersonation, including potential punitive damages. Future Chinese court rulings on these issues are likely to cite this interpretation as the controlling framework.

**Tags**: `#AI regulation`, `#deepfake`, `#algorithmic pricing`, `#legal liability`, `#China`

---

<a id="item-tech-news-4"></a>
### [Autonomous Bad Apple generation with a 417k-parameter recurrent dynamical system](https://www.reddit.com/r/MachineLearning/comments/1wa8rub/generating_bad_apple_autonomously_from_a_single/) ⭐️ 7.0/10

The author SEBADA321 trained a tiny recurrent dynamical system with 417,129 parameters \(~1.60 MB in FP32\) that autonomously generates the full ~6,500-frame, 384x512 grayscale Bad Apple video from a single initial recurrent state \(h\_0, c\_0\), without receiving any timestamp inputs during inference. The closed-loop model evaluates \(h\_t, c\_t\) through a 4-gate LSTM-style recurrent transition \(ctf, 16,640 parameters\) and a depthwise-separable frame decoder \(fd, 400,361 parameters\), running at over 200 FPS with ~17.2 MB peak active VRAM on an RTX 4080. Unlike earlier SIREN coordinate-based work that mapped \(t, y, x\) to pixels, this system learns the continuous temporal flow in a 64-D latent space and generates the whole sequence from a fixed initial condition. Training used learned latent teacher tables, a rollout horizon curriculum from K=2 to K=512, state perturbation noise \(sigma=0.005\), second-difference acceleration regularization, AdamW for decoder/tables and Muon for recurrent weights, and chunked decoding of 32-frame temporal chunks. The code, weights, rollout scripts, plots, and standalone models are publicly available on GitHub at SEBADA321/BadAppleRNN, and the author notes the decoder still needs optimization.

reddit · r/MachineLearning · /u/SEBADA321 · Sep 8, 00:05

**「Background」** Recent prior work trained a SIREN MLP to implicitly memorize Bad Apple as a coordinate function from timestamp and pixel coordinates to pixel values. The new demonstration instead treats video generation as an autonomous closed-loop dynamical process in latent space, avoiding explicit time input; training such recurrent systems over thousands of frames is difficult because error can compound, gradients can vanish or explode, and short-horizon teacher-forced accuracy does not guarantee long-horizon stability.

**Tags**: `#recurrent-neural-networks`, `#generative-modeling`, `#video-generation`, `#machine-learning`, `#open-source`

---

## Financial News

<a id="item-finance-news-1"></a>
### [China injects $54 billion into state banks and insurers; shares fall on smaller-than-expected package](https://www.cnbc.com/2026/09/07/china-state-banks-lenders-insurers-capital-solvency-bankrupt-nim-.html) ⭐️ 8.0/10

China is injecting 360 billion yuan \($53.6 billion\) into three state-owned banks and five insurers in a recapitalization led by the finance ministry, but Hong Kong-listed shares of the lenders and insurers fell on Monday after Citibank said the package was smaller than expected.

rss · CNBC Finance · Sep 7, 23:23

**「Background」** The move follows a 500 billion yuan injection into four major state banks last year and a March pledge to issue 300 billion yuan in special treasury bonds this year, and it comes as banks&\#x27; net interest margins hit record lows and insurers&\#x27; solvency ratios have weakened.

**「Impact」** Analysts say the capital mainly gives lenders room to fund strategic priorities such as AI and technology and to write off bad loans, but they expect limited near-term effect on the economy because weak credit demand, not capital, constrains lending.

**Tags**: `#China`, `#capital injection`, `#banks`, `#insurers`, `#financial policy`

---