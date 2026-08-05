---
layout: default
title: "Horizon Summary: 2026-08-05 (EN)"
date: 2026-08-05
lang: en
---

> From 46 items, 17 important content pieces were selected

---

**Technology News**
1. [Keyv npm Packages Compromised in Active Shai-Hulud Supply-Chain Attack](#item-tech-news-1) ⭐️ 8.0/10
2. [China Issues First Mandatory L3/L4 Autonomous Driving National Standard, Effective July 2027](#item-tech-news-2) ⭐️ 8.0/10
3. [Mistral Releases Shieldstral, a 3B Open-Weight Multimodal Moderation Model](#item-tech-news-3) ⭐️ 7.0/10
4. [Waymo Opens Dallas Robotaxi Service to All](#item-tech-news-4) ⭐️ 7.0/10
5. [Running DeepSeek V4 Flash on a Single AMD MI300X](#item-tech-news-5) ⭐️ 7.0/10
6. [Why Legitimate FedEx Emails Still Look Like Phishing](#item-tech-news-6) ⭐️ 7.0/10
7. [Oxide Computer Raises $445M in New SEC Filing](#item-tech-news-7) ⭐️ 7.0/10
8. [Run MiniMax-H3 locally on Apple Silicon with MLX port](#item-tech-news-8) ⭐️ 7.0/10
9. [HP, Asus, Acer Begin Limited Use of CXMT DRAM Amid Shortage](#item-tech-news-9) ⭐️ 7.0/10
10. [Cloudflare Ditches Third-Party Security Tools for $58/Month AI Bug Bounty Triage](#item-tech-news-10) ⭐️ 7.0/10
11. [Trump Administration Drafting Ban on Chinese Optical Modules](#item-tech-news-11) ⭐️ 7.0/10

**Financial News**
1. [Polymarket in Talks for Fundraising at Over $20 Billion Valuation](#item-finance-news-1) ⭐️ 8.0/10
2. [Goldman Sachs Equities Revenue Jumps 72% to Record $7.42 Billion](#item-finance-news-2) ⭐️ 8.0/10
3. [Google builds roughly $200bn AI-chip financing structure for Anthropic](#item-finance-news-3) ⭐️ 8.0/10
4. [After-Hours Earnings Reports Drive Sharp Stock Moves](#item-finance-news-4) ⭐️ 7.0/10
5. [Premarket movers: Caterpillar, Palantir and Merck react to earnings](#item-finance-news-5) ⭐️ 7.0/10
6. [White House Reverses on Open-Source AI Regulation, Pivoting to Security Reviews](#item-finance-news-6) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Keyv npm Packages Compromised in Active Shai-Hulud Supply-Chain Attack](https://www.aikido.dev/blog/keyv-and-friends-compromised-in-npm-supply-chain-attack) ⭐️ 8.0/10

Keyv and related npm packages have been compromised in an active Shai-Hulud supply-chain attack, according to a blog post by Aikido.dev. The incident highlights systemic risks in the npm dependency ecosystem, where widely used packages can be abused to propagate malicious code. The attack is described as ongoing and appears to leverage the Shai-Hulud worm, which can exfiltrate data and spread through dependent projects. Developers and organizations using affected packages should treat their dependency chains as potentially compromised and audit them promptly.

hackernews · cimi\_ · Aug 4, 11:01 · [Discussion](https://news.ycombinator.com/item?id=49166874)

**「Background」** Keyv is a widely used key-value storage library for Node.js, with hundreds of millions of monthly downloads. In this incident, attackers compromised the maintainer&\#x27;s GitHub account and published malicious versions of Keyv and eight related npm packages, injecting Shai-Hulud malware that can exfiltrate environment variables and secrets from affected applications. Such supply-chain attacks exploit npm&\#x27;s dependency system, where packages automatically install and run code from dependencies, making a single compromised maintainer account a vector for widespread malware distribution.

**「Community Discussion」** Commenters expressed frustration with npm&\#x27;s lifecycle hooks and the fragile dependency ecosystem, with some recommending defenses such as static and behavioral analysis tools like Packj and consistent use of devcontainers. Others questioned whether GitHub could automatically block Shai-Hulud exfiltration repositories, while noting that the widespread reliance on transitive dependencies makes such attacks difficult to fully clean up.

<details><summary>References</summary>
<ul>
<li><a href="https://www.aikido.dev/blog/keyv-and-friends-compromised-in-npm-supply-chain-attack">Keyv and friends compromised in npm supply chain attack</a></li>
<li><a href="https://dev.to/onsen/keyv-supply-chain-attack-what-you-need-to-know-now-1466">Keyv Supply Chain Attack : What You Need to... - DEV Community</a></li>
<li><a href="https://cybersecuritynews.com/keyv-npm-package-compromised/">Keyv npm Package With 127 Million Weekly Downloads...</a></li>

</ul>
</details>

**Tags**: `#security`, `#npm`, `#supply-chain`, `#javascript`, `#open-source`

---

<a id="item-tech-news-2"></a>
### [China Issues First Mandatory L3/L4 Autonomous Driving National Standard, Effective July 2027](https://wap.miit.gov.cn/jgsj/zbys/qcgy/art/2026/art_a1d2072374884287b67048a77560014e.html) ⭐️ 8.0/10

The Ministry of Industry and Information Technology \(MIIT\) of China has issued the country&\#x27;s first mandatory national standard for L3 and L4 autonomous driving systems, titled “Safety Requirements for Intelligent Connected Vehicles – Automated Driving Systems” \(GB 44721—2026\), which will take effect on July 1, 2027. The standard applies to passenger \(category M\) and cargo \(category N\) vehicles equipped with L3 conditional and L4 highly automated driving systems, but explicitly excludes automatic parking systems. It systematically upgrades the 2024 recommended national standard into a binding requirement, building a safety framework across four dimensions: enterprise full-lifecycle safety assurance, system dynamic driving capability, human-machine interaction and user notification, and multi-dimensional inspection and testing. The standard mandates that autonomous driving systems achieve a safety level at least equivalent to a qualified and attentive human driver. This transition from recommended to mandatory rules marks a major regulatory milestone that will require manufacturers to meet binding safety requirements in the design, production, and deployment of L3 and L4 vehicles.

telegram · zaihuapd · Aug 4, 13:06

**「Background」** Automated driving levels are defined by standards such as SAE J3016: L3 \(conditional automation\) allows the driver to relinquish continuous control but requires them to be ready to intervene when requested, while L4 \(high automation\) can perform all driving tasks within a defined operational design domain without expecting driver intervention. This new Chinese national standard is a mandatory upgrade of the 2024 recommended national standard, making the previously voluntary safety requirements legally binding for vehicles equipped with these systems.

**「Impact」** By July 2027, automakers and suppliers selling L3/L4 passenger or cargo vehicles in China must comply with the mandatory safety requirements of GB 44721—2026, including achieving a demonstrated safety level at least equal to a qualified and attentive human driver, covering system design, human-machine interaction, user notification, and testing processes.

**Tags**: `#autonomous-driving`, `#regulation`, `#China`, `#AI-safety`, `#standards`

---

<a id="item-tech-news-3"></a>
### [Mistral Releases Shieldstral, a 3B Open-Weight Multimodal Moderation Model](https://mistral.ai/news/shieldstral/) ⭐️ 7.0/10

Mistral has released Shieldstral, a 3B-parameter open-weights model designed for multimodal content moderation. The release gives developers and platforms a cost-effective, self-hostable option for automated moderation rather than relying on closed APIs. It reflects Mistral&\#x27;s strategy of focusing on smaller, fine-tuned models for specific use cases instead of competing at the frontier-model scale. As an open-weights model, Shieldstral can be customized and integrated into moderation pipelines, although detailed performance metrics and the exact moderation policies it follows have not been specified.

hackernews · riadsila · Aug 4, 16:36 · [Discussion](https://news.ycombinator.com/item?id=49171268)

**「Background」** Shieldstral is a 3B-parameter open-weights multimodal safety classifier released by Mistral AI on August 4, 2026. It judges text and images against moderation policies written in plain language at inference time, so rules can be adjusted without retraining. Mistral says it matches models up to 7 times larger on text safety and sets a new state of the art on multimodal moderation, making it a viable cost-effective option for open-weights deployers.

**「Impact」** Developers building image-sharing or social platforms can deploy Shieldstral as a practical first-pass content moderation layer, potentially reducing costs before human review. Whether it can enforce arbitrary custom rulesets without retraining remains an open question, so teams should evaluate its flexibility against their specific policies.

**「Community Discussion」** Commenters welcomed the release but questioned how much it can be tuned without retraining, wondering if it is limited to the moderation style typical of big tech platforms. Others noted its usefulness as an initial automated filter ahead of human review, with one comparison to OpenAI&\#x27;s omni-moderation model.

<details><summary>References</summary>
<ul>
<li><a href="https://mistral.ai/news/shieldstral/">Introducing Shieldstral. | Mistral AI</a></li>
<li><a href="https://www.unite.ai/mistrals-shieldstral-packs-policy-adaptive-safety-screening-into-3b-parameters/">Mistral’s Shieldstral Packs Policy-Adaptive Safety Screening ...</a></li>

</ul>
</details>

**Tags**: `#Mistral`, `#content moderation`, `#open-weights`, `#AI safety`, `#multimodal`

---

<a id="item-tech-news-4"></a>
### [Waymo Opens Dallas Robotaxi Service to All](https://waymo.com/blog/shorts/dallas-open-to-all/) ⭐️ 7.0/10

Waymo has opened its autonomous ride-hailing service to everyone in Dallas, marking another major expansion of commercial robotaxi operations in a large U.S. metroplex. The move brings driverless vehicles to a low-density, car-dependent region with limited public transit, signaling continued growth of Waymo&\#x27;s public deployment beyond earlier cities. This expansion matters because it tests the viability of autonomous ride-hailing in sprawling, highway-centric environments and broadens real-world exposure to self-driving technology. No specific date, fleet size, or service area boundaries were provided in the announcement, but the service is now available to all users in Dallas.

hackernews · xnx · Aug 4, 18:29 · [Discussion](https://news.ycombinator.com/item?id=49172836)

**「Background」** Waymo is Alphabet&\#x27;s autonomous ride-hailing service that has been gradually expanding across U.S. cities. For Dallas, Waymo announced in July 2025 that it would launch in 2026 and operate through a multi-year partnership with Avis Budget Group, which handles fleet maintenance and depot infrastructure. The service first opened to riders from an interest list in February 2026, and on August 4, 2026, it became available to everyone in Dallas.

**「Impact」** All Dallas residents and visitors can now use the Waymo app to hail fully autonomous rides without a waitlist, expanding service beyond the roughly 150,000 people who rode during the invitation-only phase since February.

**「Community Discussion」** Commenters expressed general enthusiasm for Waymo&\#x27;s safety and road behavior, with some noting the vehicles have become unremarkable in areas like Los Angeles and that they cause fewer incidents than human drivers. Others raised economic concerns about money leaving the local economy, while one real estate professional argued that driverless cars could serve as an effective affordable housing policy by reducing transportation costs, and another welcomed the expansion in Dallas for its low density and limited transit options.

<details><summary>References</summary>
<ul>
<li><a href="https://waymo.com/blog/2025/07/our-next-city-dallas/">Introducing our next city: Dallas - waymo.com</a></li>
<li><a href="https://waymo.com/blog/shorts/dallas-open-to-all/">August 4, 2026 - From the road - Waymo</a></li>
<li><a href="https://tech.yahoo.com/transportation/articles/waymo-launch-autonomous-ride-hailing-224642342.html">Waymo to launch autonomous ride-hailing in Dallas next year</a></li>
<li><a href="https://www.unite.ai/waymo-drops-the-dallas-waitlist-as-freeway-and-airport-testing-looms/">Waymo Drops the Dallas Waitlist as Freeway and Airport ...</a></li>
<li><a href="https://waymo.com/blog/shorts/dallas-open-to-all/">August 4, 2026 - From the road - Waymo</a></li>

</ul>
</details>

**Tags**: `#autonomous vehicles`, `#Waymo`, `#AI`, `#transportation`, `#industry expansion`

---

<a id="item-tech-news-5"></a>
### [Running DeepSeek V4 Flash on a Single AMD MI300X](https://github.com/ryanzhou/deepseek-v4-flash-mi300x) ⭐️ 7.0/10

A project on GitHub demonstrates how to run DeepSeek V4 Flash on a single AMD MI300X accelerator, trading a reduced context window for the ability to fit the model on one OAM module. The setup preserves the model&\#x27;s full inference weights without additional quantization, and commenters estimate throughput around 150 tokens per second. The key tradeoff is context length: the model is normally trained and served at 1M tokens, while this configuration uses 256k. Hardware availability is a caveat, since MI300X is an OAM module generally sold in 8-GPU boxes at ~€250K, though commenters note the MI350P PCIe card with 144GB may also run the model.

hackernews · zhoutong · Aug 4, 10:00 · [Discussion](https://news.ycombinator.com/item?id=49166386)

**「Background」** DeepSeek V4 Flash is a large Mixture-of-Experts \(MoE\) language model with 256 billion parameters that uses native MXFP4 quantization, making its 144GB of weights feasible on a single high-memory accelerator. The AMD MI300X is an OAM module with 192GB of HBM3 memory, typically sold in 8-GPU servers, and running such a large model usually requires multiple GPUs. This project demonstrates how to fit and run DeepSeek V4 Flash on a single MI300X by reducing the context window from 1M tokens to 256K tokens, while preserving the full inference weights and achieving over 150 tokens per second in single-stream decode.

**「Impact」** For practitioners targeting single-accelerator DeepSeek V4 Flash inference, the project provides a practical recipe that keeps full-weight quality at more than 150 tokens per second, with only context length reduced; however, the MI300X&\#x27;s OAM-only packaging and roughly €250K 8-GPU system cost limits adoption to those with access to such hardware or an MI350P alternative.

**「Community Discussion」** Commenters generally welcomed the tradeoff as practical, citing full-weight preservation and high throughput, but questioned hardware accessibility since a single MI300X is not sold directly, and suggested the MI350P PCIe \(144GB\) as a cheaper alternative. Some also pointed out that prior work such as DwarfStar can run the same model in less memory, which the author did not list.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/ryanzhou/deepseek-v4-flash-mi300x">GitHub - ryanzhou/ deepseek - v 4 - flash - mi 300 x · GitHub</a></li>

</ul>
</details>

**Tags**: `#deepseek-v4`, `#AMD-MI300X`, `#inference`, `#quantization`, `#hardware`

---

<a id="item-tech-news-6"></a>
### [Why Legitimate FedEx Emails Still Look Like Phishing](https://www.troyhunt.com/thanks-fedex-this-is-why-we-keep-getting-phished/) ⭐️ 7.0/10

Troy Hunt&\#x27;s 2024 post dissects a legitimate-looking FedEx phishing email to explain why people keep falling for such scams, pointing to broken sender authentication and confusing domain practices as the root causes. He argues that even credible-looking messages can fail basic trust signals, making it nearly impossible for recipients to distinguish genuine delivery notifications from malicious ones. The piece is framed as a high-value cautionary analysis for software engineers and security-conscious readers, not as a report of a new vulnerability or breakthrough. The broader point is that usability failures in email infrastructure, not just user gullibility, drive phishing success.

hackernews · stymaar · Aug 4, 21:09 · [Discussion](https://news.ycombinator.com/item?id=49175192)

**「Background」** Troy Hunt, a well-known security researcher, examined a phishing-style SMS and related FedEx communications that turned out to be legitimate, highlighting how official messages can closely mimic the signals users are told to treat as suspicious. The article describes his decision to verify through FedEx&\#x27;s website rather than the number in the SMS, and notes that such confusing official communication undermines users&\#x27; ability to distinguish real messages from phishing. This background matters because the piece&\#x27;s argument is that systemic usability problems in email/SMS authentication and domain practices—not just user naivete—cause phishing to succeed.

**「Impact」** The concrete consequence is that people who receive genuine automated delivery notices from companies like FedEx cannot reliably trust them, which can lead both to missed real packages and to successful phishing when users stop treating warning signs as decisive.

**「Community Discussion」** Commenters shared matching experiences: one had to coax a FedEx chatbot to confirm a legitimate customs email, another noted Google&\#x27;s c.gle links are hard to verify, and others blamed the flood of .xyz top-level domains and the IRS&\#x27;s scam-like text-to-speech system for eroding trust. The overall sentiment is that systemic usability and authentication failures, rather than simple user carelessness, are the real problem.

<details><summary>References</summary>
<ul>
<li><a href="https://www.troyhunt.com/thanks-fedex-this-is-why-we-keep-getting-phished/">Troy Hunt: Thanks FedEx, This is Why we Keep Getting Phished</a></li>

</ul>
</details>

**Tags**: `#phishing`, `#security`, `#email`, `#usability`, `#FedEx`

---

<a id="item-tech-news-7"></a>
### [Oxide Computer Raises $445M in New SEC Filing](https://www.sec.gov/Archives/edgar/data/1795071/000179507126000002/xslFormDX01/primary_doc.xml) ⭐️ 7.0/10

Oxide Computer has raised $445 million according to an SEC Form D filing, marking a substantial funding milestone for the rack-scale hardware company. The filing itself provides no technical details, but the reported amount appears to be the company&\#x27;s largest round to date. Oxide builds integrated rack-scale systems combining compute, storage, and networking with an open-source management stack. The new capital likely supports continued development and commercialization of its hardware platform. Observers note that, despite years of coverage, the company has not publicly shown widespread customer deployments.

hackernews · depr · Aug 4, 20:13 · [Discussion](https://news.ycombinator.com/item?id=49174407)

**「Background」** Oxide Computer is an Emeryville, California-based startup founded in 2019 by former Joyent and Sun Microsystems engineers. The company sells rack-scale integrated hardware alongside open-source software, positioning itself as an on-premises cloud alternative. It previously announced a $200 million Series C in February 2026, making this $445 million SEC Form D filing a significant follow-on funding event.

**「Impact」** The $445 million raise gives Oxide Computer significantly more financial runway to scale its rack-scale hardware business, though the SEC filing does not disclose shipping status, revenue, or deployment metrics.

**「Community Discussion」** Commenters expressed enthusiasm for Oxide&\#x27;s product concept and confidence in team members such as Jessie Frazelle, but several questioned whether the company actually ships hardware to customers, citing the lack of deployment images or announcements. One self-identified VP of Engineering reported filling out Oxide&\#x27;s sales form and never receiving a response while spending $900k per year on AWS.

<details><summary>References</summary>
<ul>
<li><a href="https://aiweekly.co/alerts/oxide-computer-discloses-445m-funding-round-in-sec-form-d">Oxide Computer discloses $445M funding round in SEC Form D</a></li>
<li><a href="https://assets.theregister.com/2026/02/13/whats_next_for_oxide_computer/">Oxide plans new rack attack with Zen 5 CPUs, DDR5</a></li>

</ul>
</details>

**Tags**: `#funding`, `#hardware`, `#Oxide Computer`, `#rack-scale`, `#tech industry`

---

<a id="item-tech-news-8"></a>
### [Run MiniMax-H3 locally on Apple Silicon with MLX port](https://simonwillison.net/2026/Aug/4/minimax-h3-mlx/#atom-everything) ⭐️ 7.0/10

Simon Willison reports on MiniMax-H3, a general-purpose, omni-modal generative system from MiniMax that accepts text, images, audio, and video and can generate up to 15-second video clips with audio. A new Python package, PipeNetwork/minimax-h3-mlx, ports the model to MLX for Apple Silicon. Willison ran it on an M5 Max MacBook Pro, downloading about 115 GB of model files and taking just under 45 minutes for a single video generation. The generated clip for the prompt &quot;a rainbow colored skunk leaps over a mossy log in a supermarket&quot; was visually impressive, but the audio was unusable speech-like garbage because no audio prompt guidance was provided; MiniMax&\#x27;s prompting guide offers detailed advice on improving this.

rss · Simon Willison · Aug 4, 19:10

**「Background」** MiniMax-H3 is an &quot;omni-modal&quot; generative model that can consume text, images, audio, and video inputs and produce video with synchronized audio. MLX is Apple&\#x27;s machine learning framework for Apple Silicon, and this port lets users run the model locally on M-series Macs rather than relying on cloud GPUs.

**「Impact」** Developers and researchers with Apple Silicon Macs can now run a large omni-modal video generation model locally, but must plan for very large downloads \(~115 GB\) and long generation times \(45 minutes per clip\), and follow the audio prompting guide to avoid poor audio quality.

**Tags**: `#MiniMax-H3`, `#MLX`, `#Apple Silicon`, `#video generation`, `#omni-modal`

---

<a id="item-tech-news-9"></a>
### [HP, Asus, Acer Begin Limited Use of CXMT DRAM Amid Shortage](https://asia.nikkei.com/business/china-tech/hp-asus-and-acer-begin-using-cxmt-chips-amid-memory-shortage) ⭐️ 7.0/10

HP, Asus, and Acer have begun limited adoption of CXMT DRAM chips in low-end notebooks for non-US markets, after completing certification in the middle of this year amid a severe memory shortage driven by AI infrastructure demand. CXMT is reportedly prioritizing most of its production capacity for Chinese customers such as Huawei. The PC makers are staying low-key to avoid alienating Micron, Samsung, and SK Hynix, which together control more than 90% of the global DRAM market; CXMT is also on the U.S. Pentagon&\#x27;s Chinese military companies list, making sourcing sensitive for American firms. CXMT debuted on Shanghai&\#x27;s STAR Market on July 27, surging more than 465% on its first day and reaching a market value of over 3.5 trillion yuan, surpassing Intel. IDC estimates that global PC shipments could decline more than 11% this year because of the memory shortage.

telegram · zaihuapd · Aug 4, 07:12

**「Background」** DRAM is a type of memory used in PCs and servers, and the global market has long been controlled by Samsung, SK Hynix, and Micron. CXMT is China&\#x27;s leading DRAM maker, and its recent STAR Market listing has made it a visible alternative supplier as memory demand has outpaced supply.

**「Impact」** For HP, Asus, and Acer, the immediate effect is a certified but limited DRAM option for non-US budget laptops, while the broader PC industry faces an IDC-estimated shipment decline of more than 11% this year because of the shortage.

**Tags**: `#DRAM`, `#semiconductors`, `#supply chain`, `#China tech`, `#PC industry`

---

<a id="item-tech-news-10"></a>
### [Cloudflare Ditches Third-Party Security Tools for $58/Month AI Bug Bounty Triage](https://www.theregister.com/security/2026/08/04/cloudflare-has-mostly-ditched-third-party-security-tools-suggests-not-trying-that-at-home/5282600) ⭐️ 7.0/10

Cloudflare CISO Grant Bourzikas disclosed at a Sydney event that the company has largely replaced third-party security tools with 200-plus autonomous security agents built in-house, including using Anthropic&\#x27;s Claude Sonnet model to triage bug bounty reports at about $58 per month. He contrasted that with roughly $200,000 per month that a specialized security model called Mythos would cost for the same work, and noted many of Cloudflare&\#x27;s custom applications are partly AI-written. Bourzikas cautioned other enterprises against copying the approach, saying not every bank should build all its own security software. Chief Strategy Officer Stephanie Cohen linked the company&\#x27;s earlier layoff of 1,100 people to AI-driven automation and said Cloudflare plans to act as an intermediary between AI companies and publishers, using micropayments for content access.

telegram · zaihuapd · Aug 4, 09:24

**「Background」** Bug bounty programs rely on human analysts to deduplicate and assess the value of incoming vulnerability reports, which is labor-intensive and often expensive. Cloudflare&\#x27;s budget-conscious use of a general-purpose large language model for that triage work highlights how AI is being applied to routine security operations, though the company acknowledges its in-house engineering capacity is not typical.

**「Impact」** For security teams and bug bounty programs, Cloudflare&\#x27;s reported cost figures suggest that general-purpose LLMs can make vulnerability triage dramatically cheaper, but they also underscore that replicating this approach requires strong internal development capability, which Cloudflare itself advises others not to assume.

**Tags**: `#AI security`, `#Cloudflare`, `#bug bounty`, `#LLM automation`, `#security operations`

---

<a id="item-tech-news-11"></a>
### [Trump Administration Drafting Ban on Chinese Optical Modules](https://www.reuters.com/world/trump-administration-drafting-ban-chinese-data-center-devices-sources-say-2026-08-04/) ⭐️ 7.0/10

The Trump administration is drafting a ban on imports of new Chinese data center components, focusing on optical modules, according to four people familiar with the matter. The FCC is advancing the measure, and officials hope to issue and implement it within the year to protect critical infrastructure supporting the AI boom. The ban aims to prevent China from stealing data, implanting malware, or disrupting services, but sources caution it may still be modified or shelved. If implemented, it would hit Chinese optical module maker Zhongji Innolight, which holds 27% of the global market share. The FCC has previously imposed similar import restrictions on Chinese drones, routers, robots, and inverters, and China&\#x27;s embassy in the U.S. said it would take all necessary measures to protect its interests.

telegram · zaihuapd · Aug 4, 11:29

**「Background」** Optical transceivers, also called optical modules, are key components used to connect servers and switches in data centers and are especially critical in AI-heavy computing clusters. The U.S. Federal Communications Commission \(FCC\) has already restricted imports of Chinese-made drones, routers, robots, and inverters, and this reported draft rule would extend that approach to new models of Chinese data center components, focusing on optical modules. The proposal is not finalized and could be changed or shelved, according to sources, but it targets a major supply chain where Chinese vendor Zhongji Innolight holds about 27% of the global market.

**「Impact」** If finalized, the FCC&\#x27;s import ban would directly hit U.S. hyperscalers and AI data-center builders that depend on Chinese optical transceivers, since Chinese makers collectively supply nearly two-thirds of global units and about 60% of optical datacom transceiver revenue, with Zhongji Innolight alone holding 27% of the data-center transceiver market. The proposal has already sparked rallies in optical component stocks and positioned rivals such as Coherent and Lumentum as potential beneficiaries, though officials caution the rule could still be revised or shelved before it takes effect.

<details><summary>References</summary>
<ul>
<li><a href="https://www.theguardian.com/technology/2026/aug/04/fcc-ban-china-datacenter-devices">Trump administration reportedly drafting ban on Chinese datacenter components | Technology | The Guardian</a></li>
<li><a href="https://www.newsnationnow.com/business/tech/fcc-ban-chinese-data-center-components/">Report: FCC considering ban on Chinese data center components</a></li>
<li><a href="https://www.dailymail.com/news/article-16028817/trump-fcc-ban-chinese-data-center-parts.html">The terrifying truth behind Trump&#x27;s ban on Chinese data center parts spreading across the US | Daily Mail Online</a></li>
<li><a href="https://wccftech.com/the-fcc-mulls-banning-china-sourced-optical-transceivers-threatening-innolights-27-global-market-share-as-coherent-and-lumentum-prepare-to-pounce/">The FCC Mulls Banning China-Sourced Optical Transceivers, Threatening Innolight&#x27;s 27% Global Market Share As Coherent And Lumentum Prepare To Pounce</a></li>
<li><a href="https://www.emsnow.com/fcc-proposed-import-ban-on-chinese-optical-transceivers-implications-for-us-hyperscalers-chinese-suppliers-and-global-ai-infrastructure">FCC Proposed Import Ban on Chinese Optical Transceivers: Implications for US Hyperscalers, Chinese Suppliers, and Global AI Infrastructure · EMSNow</a></li>
<li><a href="https://finance.yahoo.com/markets/stocks/articles/optical-component-stocks-rally-proposed-113406255.html">Optical component stocks rally on proposed U.S. ban on Chinese tech</a></li>

</ul>
</details>

**Tags**: `#US-China tech policy`, `#optical modules`, `#AI infrastructure`, `#supply chain`, `#regulation`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Polymarket in Talks for Fundraising at Over $20 Billion Valuation](https://www.cnbc.com/2026/08/04/polymarket-seeks-fundraising-round-at-more-than-20-billion-valuation.html) ⭐️ 8.0/10

Polymarket is in talks for a fundraising round that would value the prediction-market platform at more than $20 billion, a person familiar with the matter told CNBC; the company previously said its annualized revenue was above $1 billion as of late June.

rss · CNBC Finance · Aug 4, 13:31

**「Background」** Polymarket closed a funding round in April at a $15 billion valuation, and rival Kalshi was valued at $22 billion in May.

**「Impact」** If completed, the round would be Polymarket&\#x27;s first since launching its regulated U.S. exchange in May.

**Tags**: `#Polymarket`, `#fundraising`, `#valuation`, `#prediction markets`, `#private markets`

---

<a id="item-finance-news-2"></a>
### [Goldman Sachs Equities Revenue Jumps 72% to Record $7.42 Billion](https://www.cnbc.com/2026/08/01/goldman-traders-are-on-pace-for-a-record-year-a-close-up-look-at-how-theyre-doing-it.html) ⭐️ 8.0/10

Goldman Sachs is on pace for a record trading year after equities revenue surged 72% to a record $7.42 billion in the second quarter, according to CNBC. Investment banking revenue rose 55% to $3.4 billion.

rss · CNBC Finance · Aug 4, 19:38

**「Background」** Goldman has spent years investing in equities and shifting its Global Banking &amp; Markets strategy to cross-sell trading services to investment banking and wealth management clients. That division generated $15.5 billion in revenue last quarter, more than 75% of the bank&\#x27;s total.

**Tags**: `#Goldman Sachs`, `#equities trading`, `#Q2 earnings`, `#capital markets`, `#trading revenue`

---

<a id="item-finance-news-3"></a>
### [Google builds roughly $200bn AI-chip financing structure for Anthropic](https://www.ft.com/content/549f2e23-5aa2-49c7-9ea6-a9784ab7087c) ⭐️ 8.0/10

According to a Financial Times investigation published on Aug. 4, Google has put together a roughly $200 billion Wall Street financing structure to deliver more than $150 billion of AI chips to Anthropic, with about 80% of the contracts tied directly to the chips. The arrangement, involving Broadcom, Apollo, Blackstone and Morgan Stanley, lets the parties avoid putting hundreds of billions of dollars in AI hardware on their own balance sheets.

telegram · zaihuapd · Aug 4, 10:52

**「背景」** 据《金融时报》调查，谷歌悄然搭建了史上规模最大的基础设施融资架构之一，用于向 Anthropic 交付 AI 芯片，相关合同总额约 2000 亿美元，其中约八成与芯片直接挂钩。由于 Anthropic 没有信用评级，各方分担风险：谷歌担保数据中心，博通购买并协助融资芯片，阿波罗和黑石出资购买硬件后回租给 Anthropic。今年 6 月，特殊目的载体 Compute SPV 完成了首批交易，购入约 350 亿美元硬件，约合 1 吉瓦算力和 100 万颗 TPU。该模式借鉴波音、GE 推销飞机和发动机的厂商融资玩法，让各方都不必把数百亿美元 AI 硬件压在自家资产负债表上。

**「Impact」** Because Anthropic has no credit rating, risk is split: Google guarantees data centers, Broadcom buys and helps finance the chips, and Apollo and Blackstone buy the hardware and lease it back to Anthropic.

<details><summary>References</summary>
<ul>
<li><a href="https://the-decoder.com/google-moves-billions-in-anthropic-chip-risk-off-its-balance-sheet/">Google moves billions in Anthropic chip risk off its balance sheet</a></li>
<li><a href="https://finance.biggo.com/news/cc3ceaa8-e838-4501-b4c0-13b9fcba9232">Google Orchestrates $200 Billion AI Chip Financing Network in Landmark Infrastructure Deal — BigGo Finance</a></li>
<li><a href="https://www.bloomberg.com/news/articles/2026-05-28/apollo-shops-36-billion-debt-deal-to-buy-google-chips-for-anthropic">Apollo, Blackstone Seek Investors for $36 Billion Anthropic Chip Financing Deal - Bloomberg</a></li>

</ul>
</details>

**Tags**: `#AI`, `#financing`, `#Google`, `#Anthropic`, `#infrastructure`

---

<a id="item-finance-news-4"></a>
### [After-Hours Earnings Reports Drive Sharp Stock Moves](https://www.cnbc.com/2026/08/04/stocks-making-the-biggest-moves-after-the-bell-spcx-amd-pins-anet-wynn.html) ⭐️ 7.0/10

Several stocks moved sharply after the bell following quarterly earnings reports, with Arista Networks jumping 11% after beating estimates and AMD falling 8% despite a slight earnings beat.

rss · CNBC Finance · Aug 4, 22:25

**「Background」** These after-hours moves reflect how investors react to quarterly results and guidance released after the market closes.

**Tags**: `#earnings`, `#after-hours trading`, `#stock movers`, `#technology`, `#guidance`

---

<a id="item-finance-news-5"></a>
### [Premarket movers: Caterpillar, Palantir and Merck react to earnings](https://www.cnbc.com/2026/08/04/stocks-making-the-biggest-moves-premarket-mcd-cat-pltr-mrk.html) ⭐️ 7.0/10

Several companies moved sharply in premarket trading after second-quarter earnings, with Caterpillar climbing 8% after earning an adjusted $8.17 per share versus the $6.20 analysts expected, and Palantir jumping 15% on blowout results.

rss · CNBC Finance · Aug 4, 11:42

**「Background」** The moves follow second-quarter earnings reports from the named companies; analyst estimates cited are LSEG consensus figures.

**Tags**: `#Earnings`, `#Premarket Movers`, `#Pharmaceuticals`, `#Semiconductors`, `#Industrial Sector`

---

<a id="item-finance-news-6"></a>
### [White House Reverses on Open-Source AI Regulation, Pivoting to Security Reviews](https://www.nytimes.com/2026/08/04/technology/ai-washington-regulation-whiplash.html) ⭐️ 7.0/10

The New York Times reports that the White House has swung away from considering sanctions or a trade blacklist on Chinese open-source AI models and will instead discuss a framework on August 4 that would require pre-release cybersecurity reviews of AI models.

telegram · zaihuapd · Aug 4, 15:22

**「Background」** The shift follows the Chinese open-source model Kimi approaching top OpenAI performance; OpenAI and Anthropic have pushed for restrictions on Chinese rivals while Nvidia and Meta defend open ecosystems. Nvidia’s Jensen Huang recently posted on X for the first time in defense of open source and helped form a safety alliance with more than 230 members.

**Tags**: `#AI监管`, `#开源AI`, `#白宫政策`, `#硅谷`, `#网络安全`

---