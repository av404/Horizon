---
layout: default
title: "Horizon Summary: 2026-09-30 (EN)"
date: 2026-09-30
lang: en
---

> From 57 items, 11 important content pieces were selected

---

**Technology News**
1. [GPT 6.1 Sol: Near-Astra intelligence for a fifth of the price](#item-tech-news-1) ⭐️ 7.0/10
2. [America.gov Government AI Portal Reportedly Uses Google Gemini](#item-tech-news-2) ⭐️ 7.0/10
3. [PS5 Relapse Exploit Draws Hacker News Discussion](#item-tech-news-3) ⭐️ 7.0/10
4. [Privacy Analysis Compares Web and Mobile Conversational AI Agents](#item-tech-news-4) ⭐️ 7.0/10
5. [Anthropic: GLM-5.3 crosses binary-exploitation threshold](#item-tech-news-5) ⭐️ 7.0/10
6. [Cloudflare launches cf CLI open beta for AI agents and developers](#item-tech-news-6) ⭐️ 7.0/10
7. [Google fixes Firebase Analytics issue causing iOS app launch crashes](#item-tech-news-7) ⭐️ 7.0/10

**Financial News**
1. [中国对首套房贷给予1个百分点财政贴息，10月1日起实施](#item-finance-news-1) ⭐️ 8.0/10
2. [Premarket movers: Fair Isaac falls on mortgage-pricing change; AMD and CarMax rise](#item-finance-news-2) ⭐️ 7.0/10
3. [China Reportedly Sets Three Criteria for Humanoid Robot IPOs](#item-finance-news-3) ⭐️ 7.0/10
4. [Oracle Issues Force Majeure Notice as Stargate Data Center Faces Power-Approval Delay](#item-finance-news-4) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [GPT 6.1 Sol: Near-Astra intelligence for a fifth of the price](https://openai.com/index/introducing-gpt-6-1-sol/) ⭐️ 7.0/10

OpenAI announced GPT-6.1 Sol, with the release title promising &\#x27;Near-Astra intelligence for a fifth of the price,&\#x27; but the supplied item contains no technical details beyond the headline and pricing discussion. The most concrete change highlighted by Hacker News commenters is cached input pricing at $0.10 per million tokens—95% less than standard input and 50% less than GPT-6 Sol&\#x27;s cached rate—which one commenter called the real announcement for Codex usage. The release follows a poorly received GPT-6/Sol 6 generation that users described as a regression from Sol 5.6, and some commenters doubt 6.1 will differ much for coding. One commenter speculated the model may be a last-minute rename of Astra-Minor, while another warned that making token price the main battleground is ominous for the industry and investors.

hackernews · crorella · Sep 29, 17:06 · [Discussion](https://news.ycombinator.com/item?id=49896586)

**「Background」** OpenAI&\#x27;s current model line has been built around GPT-6, an earlier release that shipped as two model sizes, GPT-6 Sol and GPT-6 Luna, with Sol positioned as the higher-end option at $4 per million input tokens and $20 per million output tokens. Astra is referenced as a separate, more capable tier that costs substantially more, so the GPT-6.1 Sol release is framed as bringing &quot;near-Astra&quot; intelligence to a much lower price point: $2 per million input tokens, $0.10 per million cached input tokens, and $10 per million output tokens. Commenters also reference an intermediate &quot;Sol 5.6&quot; generation and a found-in-the-files model called &quot;Astra-Minor,&quot; though those naming details come from community discussion rather than supplied official documentation, and no source content for the announcement itself was available to verify the lineage.

**「Impact」** For heavy API and Codex users, the reported cached-input price of $0.10 per million tokens and a 50% reduction versus GPT-6 Sol&\#x27;s cached rate could substantially lower costs for repeated-context workloads, though the lack of technical detail leaves quality improvements unverified.

**「Community Discussion」** Commenters were split between practical cost interest and quality skepticism: the cached-input price cut was singled out as the most important part of the announcement, while one user reported poor reliability from recent OpenAI models and said they had switched to Opus 5.5, and another preferred DeepSeek on bang-for-buck grounds. Speculation that GPT-6.1 Sol is a rebranded Astra-Minor remained unconfirmed.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/introducing-gpt-6-sol-and-luna/">Introducing GPT-6 Sol and Luna - OpenAI</a></li>
<li><a href="https://venturebeat.com/technology/openais-gpt-6-1-sol-offers-astra-like-performance-at-1-5th-price-a-new-ultrafast-tier-clocks-at-300-tokens-per-second">OpenAI&#x27;s GPT-6.1 Sol offers Astra-like performance at 1/5th price. A new ...</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#GPT-6.1 Sol`, `#LLM pricing`, `#AI model releases`, `#Hacker News discussion`

---

<a id="item-tech-news-2"></a>
### [America.gov Government AI Portal Reportedly Uses Google Gemini](https://america.gov/) ⭐️ 7.0/10

America.gov appears to be a new U.S. government AI portal that reportedly uses Google Gemini to help more than 100 million people access public resources. According to a Google blog post cited in the discussion, Google is a technology partner in the initiative, leveraging Gemini to help people access critical public resources &quot;with greater speed and ease.&quot; The portal is intended to help users navigate government services and avoid phishing, and as a large-scale government AI deployment it carries potential policy and industry implications, though the linked page and discussion offer little technical detail. Commenters describe it as a Gemini deployment with guardrails, and one user said it would not name its underlying model while answering a question about the June 3–4, 1989 crackdown; screenshots claiming it uses a Chinese model were viewed as likely fake. The discussion broadly supports the concept of a well-crafted government-services chatbot, while highlighting concerns about accuracy, trust, and model provenance.

hackernews · plesiv · Sep 29, 14:04 · [Discussion](https://news.ycombinator.com/item?id=49893509)

**「Background」** America.gov is a newly launched U.S. government AI portal, introduced by the Trump administration, that is intended to help more than 100 million people access federal public resources. Reporting and commentary identify Google Gemini as the underlying AI technology, with Google described as a technology partner in the initiative. The concept behind such portals is to use a chatbot interface to guide users through fragmented government services, rather than requiring them to know the correct agency or form in advance.

**「Impact」** For U.S. residents seeking federal services, Google&\#x27;s role as technology partner makes Gemini the AI layer intended to help more than 100 million people access public resources faster, shifting some public-service navigation toward a private AI model. CNBC additionally reports that Grok is also used, so the complete model stack and guardrail details remain less clearly established.

**「Community Discussion」** Commenters broadly welcomed the idea—finding the correct path to government assistance being a rare, genuinely useful chatbot application—while noting phishing risks and trust concerns. One user found the portal more honest than expected in a response about unlawful entry to the U.S. Capitol, and others debated the underlying model: a commenter identified it as Gemini with guardrails, another said it would not name its model but answered a question about the June 3–4, 1989 crackdown, and screenshots claiming a Chinese model were dismissed as likely fake.

<details><summary>References</summary>
<ul>
<li><a href="https://www.facebook.com/WGME13/posts/watch-the-trump-administration-on-tuesday-launched-americagov-an-artificial-inte/1537404648414822/">WATCH: The Trump administration on Tuesday launched America.gov, an ...</a></li>
<li><a href="https://www.facebook.com/rundownnewsletter/posts/the-us-government-has-launched-americagov-a-new-ai-powered-portal-designed-to-ma/975208122267640/">The U.S. government has launched America.gov, a new AI-powered ...</a></li>
<li><a href="https://www.techbuzz.ai/articles/google-s-gemini-ai-powers-new-america-gov-federal-portal">Google&#x27;s Gemini AI Powers New America.gov Federal Portal</a></li>
<li><a href="https://blog.google/company-news/outreach-and-initiatives/public-policy/america-gov-google-public-sector/">Google Gemini powers new America.gov portal - The Keyword</a></li>
<li><a href="https://www.unite.ai/google-becomes-technology-partner-for-white-house-america-gov-launch/">Google Becomes Technology Partner for White House America.gov ...</a></li>
<li><a href="https://www.cnbc.com/2026/09/29/trump-ai-gemini-grok.html">Trump admin AI website uses Gemini, Grok: Joe Gebbia - CNBC</a></li>

</ul>
</details>

**Tags**: `#AI`, `#government`, `#Gemini`, `#public services`, `#policy`

---

<a id="item-tech-news-3"></a>
### [PS5 Relapse Exploit Draws Hacker News Discussion](https://github.com/ntfargo/Relapse-Exploit) ⭐️ 7.0/10

A GitHub repository named Relapse-Exploit for the PlayStation 5 was submitted to Hacker News and drew 235 points and 128 comments, according to the item&\#x27;s analysis. The repository appears to be a PS5 exploit, but the supplied material contains no technical write-up, exploit chain details, or independent verification of which firmware versions or capabilities it affects. Hacker News commenters speculated that it may exploit a bug in WebKit&\#x27;s JavaScriptCore JavaScript engine, and one asked whether the PS5&\#x27;s WebKit uses JavaScriptCore with JIT enabled and whether Sony might respond by disabling JIT to reduce attack surface. Discussion also connected the exploit to console security and backup limitations, including a user&\#x27;s complaint that PS5 game saves cannot be backed up to USB without a PS Plus subscription. Because the item lacks source content and verified technical detail, the exploit&\#x27;s real-world impact and reliability remain unconfirmed.

hackernews · therepanic · Sep 29, 15:44 · [Discussion](https://news.ycombinator.com/item?id=49895304)

**「Background」** Relapse-Exploit is a GitHub-hosted exploit chain that its README says targets PS5 firmware 7.00 through 13.60, so understanding it requires knowing that modern console jailbreaks often start in a bundled browser engine before pivoting to lower-level system access. According to summaries of the repository, the browser stage uses JavaScriptCore information leaks plus a structured-clone object-pool mismatch to corrupt a typed array, after which payloads are loaded and an ELF loader listens on port 9021. The exploit is run by serving the page locally or opening the project&\#x27;s GitHub Pages URL on the PS5, and the README notes that WebKit may need several reload attempts if the browser stalls.

**「Impact」** If the chain works as reported, PS5 owners on firmware versions 7.00 through 13.60 could run unsigned code, potentially enabling local game-save backups that Sony currently limits to its per-profile PS Plus cloud service. The repository has not been independently verified and Sony has not publicly responded, so the actual reach and stability of the exploit remain uncertain.

**「Community discussion」** Commenters raised both practical and strategic questions: one wanted USB save backups and described losing a year of Minecraft progress because PS5 backups require PS Plus, while others speculated that the exploit targets WebKit&\#x27;s JavaScriptCore and debated whether Sony would disable JIT. Other comments focused on the console-hacking community&\#x27;s reserve of zero-days, wished the release had waited until GTA6, or expressed interest in running Steam PC games on PS5.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/ntfargo/Relapse-Exploit">GitHub - ntfargo/Relapse-Exploit: Exploit chain for PS5 7.00 - 13.60 · GitHub</a></li>
<li><a href="https://elsolitario.org/en/2026/09/29/relapse-repo-claims-ps5-exploit-firmware-7-00-to-13-60/">PS5 Jailbreak: What Is Relapse Exploit and Its Scope</a></li>
<li><a href="https://dev.to/lu1tr0n/relapse-repo-afirma-exploit-de-ps5-en-firmware-700-1360-1n14">Relapse: repo afirma exploit de PS5 en firmware 7.00-13.60 - DEV Community</a></li>
<li><a href="https://elsolitario.org/en/2026/09/29/relapse-repo-claims-ps5-exploit-firmware-7-00-to-13-60/">PS5 Jailbreak: What Is Relapse Exploit and Its Scope - El Solitario</a></li>

</ul>
</details>

**Tags**: `#PS5`, `#console security`, `#WebKit`, `#JavaScriptCore`, `#exploit development`

---

<a id="item-tech-news-4"></a>
### [Privacy Analysis Compares Web and Mobile Conversational AI Agents](https://jorgegarciaherrero.com/wp-content/interactivos/20260916-Prompt-like-a-butterfly-sting-like-a-tracker-%28clean%29.pdf) ⭐️ 7.0/10

A privacy analysis paper titled “A Privacy Analysis of Web and Mobile Conversational AI Agents” compares how web and mobile conversational AI agents leak user data. It is accompanied by substantial Hacker News discussion—408 points and 130 comments—that adds concrete reports about prompt pre-sending, trackable conversation URLs, and platform permissions. Commenters describe web-based ChatGPT periodically sending unfinished prompts to a \`conversation/prepare\` endpoint before the user sends them, potentially revealing writing cadence and evolving ideas, and note that services such as Perplexity expose full conversations via URL. The supplied evidence includes only the paper title, an analysis summary, and comment snippets, so the paper’s methodology, exact findings, and mitigation recommendations cannot be independently verified here.

hackernews · damaru2 · Sep 29, 09:03 · [Discussion](https://news.ycombinator.com/item?id=49890226)

**「Background」** Conversational AI agents, such as ChatGPT and Perplexity, are widely used through web browsers and mobile apps, where user prompts are sent to remote servers for processing. Privacy research in this area investigates how these agents and their surrounding platforms may expose user data—for example, via third-party trackers, the pre-sending of incomplete prompts to backend endpoints, or conversation histories accessible through shareable URLs. The paper analyzed here compares such privacy risks between web and mobile environments, as detailed on its project page.

**「Impact」** Users of web and mobile conversational AI agents face a concrete exposure risk: community reports describe unfinished prompts being sent to backend endpoints such as \`conversation/prepare\` before the user hits send, and conversation URLs keyed only by a UUID revealing a full past conversation to anyone holding the link. Prior research already documents widespread user privacy, security, and trust concerns with conversational AI, but because only the paper&\#x27;s title and community comments are available here, the specific web-versus-mobile findings and their scope cannot be verified.

**「Community Discussion」** Commenters converge on concern that conversational AI services leak sensitive inputs: one reports ChatGPT’s web client pre-sending unfinished prompts to \`conversation/prepare\`, another says Perplexity exposes full conversations through UUID-based URLs, and a third argues that even private Codex sessions may feed into model improvement. Disagreement is limited, but one commenter asks how much risk comes from the agent itself versus underlying platform APIs and permissions, while another frames the issue through a Milhouse/Simpsons analogy about telling secrets to AI.

<details><summary>References</summary>
<ul>
<li><a href="https://jorgegarciaherrero.com/en/prompt-like-a-butterfly-sting-like-a-tracker/">Infographic of the paper &quot; Prompt like a Butterfly , sting like a tracker &amp;quo...</a></li>
<li><a href="https://www.sciencedirect.com/science/article/pii/S0747563224002127">Evaluating privacy, security, and trust perceptions in conversational AI: A systematic review - ScienceDirect</a></li>
<li><a href="https://arxiv.org/html/2504.06552v1">Understanding Users’ Security and Privacy Concerns and Attitudes TowardsConversational AI Platforms</a></li>

</ul>
</details>

**Tags**: `#privacy`, `#conversational-ai`, `#web-security`, `#tracking`, `#mobile-platforms`

---

<a id="item-tech-news-5"></a>
### [Anthropic: GLM-5.3 crosses binary-exploitation threshold](https://simonwillison.net/2026/Sep/29/anthropic-frontier-red-team/) ⭐️ 7.0/10

Anthropic&\#x27;s Frontier Red Team reports that GLM-5.3 and Claude Mythos Preview can now autonomously achieve full control flow hijacks in binary-exploitation tasks where earlier models failed, a finding Simon Willison quotes from the team&\#x27;s post &quot;GLM-5.3 and the spread of advanced cyber capabilities.&quot; Evaluating several models on 100 randomly selected tasks from Anthropic&\#x27;s internal Binary Exploitation benchmark, the team found GLM-5.3 developed full control flow hijacks in 4% of trials and Claude Mythos Preview in 6%, while earlier models such as Claude Opus 4.6 and GLM-5.2 did not succeed in any of them. Anthropic describes this as a meaningful capability threshold that has clearly been crossed. An accompanying summary of the same research cites different figures — 50 successes in 410 attempts for GLM-5.3 on a benchmark it calls ExploitBench, versus 56 for Claude Mythos Preview — and adds that GLM-5.3&\#x27;s safeguards could be bypassed by simple methods with 64% to 100% success in simulated tests, with open weights allowing users to modify the model to weaken its refusals. The item itself is a brief quotation plus summary, offering no methodology details or independent verification of the claims.

rss · Simon Willison · Sep 29, 22:20

**「Background」** GLM-5.3 is the latest flagship open-weight model from Z.ai \(Zhipu AI\), built on the same base model as GLM-5.2 with all improvements coming from post-training, and positioned as a leader in coding and agentic tasks. A control flow hijack is a binary-exploitation outcome in which an attacker redirects a vulnerable program&\#x27;s execution to code of their choosing, and Anthropic&\#x27;s Frontier Red Team tests this on its internal Binary Exploitation benchmark as well as on ExploitBench, where GLM-5.3 reportedly succeeded in 50 of 410 attempts against 56 for Claude Mythos Preview. Anthropic frames the result against earlier baselines — Claude Opus 4.6 and GLM-5.2 completed none of the sampled tasks — and notes that GLM-5.3 was released as open-weight without meaningful safeguards against misuse.

**「Impact」** Because GLM-5.3 is an open-weights model whose safety guardrails can be bypassed, Anthropic&\#x27;s result implies that capable autonomous binary-exploitation tooling is now reachable by a much broader pool of attackers, not just well-resourced groups — a dynamic consistent with warnings that AI lowers the barrier for less-skilled cyber criminals and enables increasingly autonomous attack campaigns. These rates come from 100 randomly selected tasks on Anthropic&\#x27;s internal Binary Exploitation benchmark, so they should not be read as a direct prediction of real-world exploitation success.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/research/glm-5-3-and-the-spread-of-advanced-cyber-capabilities">GLM-5.3 and the spread of advanced cyber capabilities \ Anthropic</a></li>
<li><a href="https://simonwillison.net/2026/Sep/29/anthropic-frontier-red-team/">A quote from Anthropic Frontier Red Team</a></li>
<li><a href="https://madrobot.blog/2026/09/29/anthropic-glm-5-3-zai-cyber-exploits-safeguards-open-weight/">Anthropic: China’s GLM-5.3 Can Build Cyber Exploits | MadRobot</a></li>
<li><a href="https://docs.z.ai/guides/llm/glm-5.3">GLM-5.3 - Overview - Z.AI DEVELOPER DOCUMENT</a></li>
<li><a href="https://aiweekly.co/alerts/anthropic-zhipus-glm-53-matches-claude-on-autonomous-exploits">Anthropic: Zhipu&#x27;s GLM-5.3 Matches Claude on Autonomous ...</a></li>
<li><a href="https://z.ai/blog/glm-5.3">GLM-5.3: Frontier Coding with Emergent Cyber Capabilities - z.ai</a></li>
<li><a href="https://www.ncsc.gov.uk/report/impact-of-ai-on-cyber-threat">The near-term impact of AI on the cyber threat</a></li>

</ul>
</details>

**Tags**: `#ai-security`, `#ai-capabilities`, `#cyber-offense`, `#large-language-models`, `#ai-safety`

---

<a id="item-tech-news-6"></a>
### [Cloudflare launches cf CLI open beta for AI agents and developers](https://blog.cloudflare.com/cloudflare-cf-cli-launch/) ⭐️ 7.0/10

Cloudflare has launched the open beta of cf, a command-line tool intended to let developers and AI agents invoke all Cloudflare APIs from the terminal. The CLI is generated from Cloudflare&\#x27;s API schema and covers more than 3,000 API operations, compared with roughly 280 operations exposed by the existing Wrangler tool. cf uses JSON as its default output and supports command search and guidance, which Cloudflare says helps agents automatically discover operations, execute them, and process results. Cloudflare gives examples such as creating and deploying a Worker, monitoring services, configuring Access and WAF, and even purchasing a domain through the same tool. The announcement is an open beta, so the item does not establish production readiness or detailed limitations.

telegram · zaihuapd · Sep 29, 13:46

**「Background」** Cloudflare&\#x27;s existing developer CLI, Wrangler, was built primarily around Workers and had grown to cover roughly 280 operations over time. Cloudflare&\#x27;s broader API surface, spanning products such as Access, WAF, and domain registration, comprises more than 3,000 operations. The new cf CLI is generated from Cloudflare&\#x27;s API schema and defaults to JSON output, a design intended to let AI agents discover and invoke API operations without separate per-endpoint tooling.

**「Impact」** For Cloudflare developers and AI-agent builders, cf&\#x27;s much broader schema-generated API coverage and JSON-first interface could make command-line automation of many Cloudflare operations feasible in one tool, though its open-beta status leaves production readiness unsettled.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.cloudflare.com/cloudflare-cf-cli-launch/">Introducing cf: the agentic CLI for the entire Cloudflare API | Cloudflare Blog</a></li>
<li><a href="https://daily.dev/posts/introducing-cf-the-agentic-cli-for-the-entire-cloudflare-api-2x4miixan">Introducing cf: the agentic CLI for the entire Cloudflare API | daily.dev</a></li>

</ul>
</details>

**Tags**: `#Cloudflare`, `#AI agents`, `#CLI`, `#API tooling`, `#developer tools`

---

<a id="item-tech-news-7"></a>
### [Google fixes Firebase Analytics issue causing iOS app launch crashes](https://github.com/firebase/firebase-ios-sdk/issues/16728) ⭐️ 7.0/10

Google confirmed that a server-side issue in Google Analytics for Firebase caused many iOS apps that integrate the component to crash on launch. The incident began on September 28, 2026, at 17:41 PDT, when the service returned malformed data, and Google completed the fix rollout at 19:52 PDT. Google said no SDK or app update was required. Because of caching, some apps could continue crashing for up to about four hours after the fix, after which the residual problems were expected to subside on their own.

telegram · zaihuapd · Sep 29, 16:29

**「Background」** Google Analytics for Firebase is a widely used mobile analytics SDK embedded in thousands of iOS and Android apps, and on iOS it fetches configuration and data payloads from Google&\#x27;s servers when an app starts. Because that payload is delivered server-side, a fault in the response can crash apps even when their own code and SDK versions have not changed — which is what occurred here, as the SDK received an incorrectly formatted payload at launch. The incident is tracked in the firebase-ios-sdk repository as issue \#16728, and Google characterized the trigger as a malformed server-side response rather than an app-level defect.

**「Impact」** For iOS developers and organizations relying on Firebase Analytics, the incident could cause app launch crashes during the affected window without any code change or SDK update, and cached responses may have extended the disruption by roughly four hours after the fix.

<details><summary>References</summary>
<ul>
<li><a href="https://firerun.io/firebase-ios-analytics-sdk-crash-server-side-2026/">Firebase Server Change Crashed iOS Apps, No Update Needed</a></li>
<li><a href="https://www.thenews.com.pk/latest/1418097-google-fixes-firebase-bug-that-crashed-thousands-of-iphone-apps">Google fixes firebase bug that crashed thousands of iPhone apps</a></li>
<li><a href="https://9to5google.com/2026/09/29/google-firebase-iphone-app-crash-fixed/">Google has fixed an issue that caused iPhone apps to crash</a></li>

</ul>
</details>

**Tags**: `#Firebase`, `#iOS`, `#service outage`, `#Google Analytics`, `#mobile development`

---

## Financial News

<a id="item-finance-news-1"></a>
### [中国对首套房贷给予1个百分点财政贴息，10月1日起实施](https://jrs.mof.gov.cn/zhengcefabu/phjr/202609/t20260929_3998312.htm) ⭐️ 8.0/10

中国财政部、中国人民银行、金融监管总局9月29日联合印发通知，自2026年10月1日起在全国对新发放的首套住房商业贷款给予中央财政贴息，标准为年化1个百分点、期限最长5年，单户贴息贷款本金上限100万元，政策暂定实施1年。按此测算，单户每年最高贴息约1万元；适用条件为购买首套住房、建筑面积120平方米以下（含）、房价150万元以下（含），且须为新发放贷款而非置换存量贷款。

telegram · zaihuapd · Sep 29, 10:18

**「Background」** The measure follows an earlier three-department decision to extend fiscal interest subsidies for personal consumer loans through the end of 2026, reflecting an existing channel for using central fiscal subsidies to lower household borrowing costs.

**「Who benefits」** Households taking out a new commercial mortgage on a first home of 120 sq m or less and priced at 1.5 million yuan or below can receive up to about 10,000 yuan a year in relief on as much as 1 million yuan of loan principal, and one analysis cited by Sinocism estimates the 1-percentage-point subsidy is equivalent to roughly one-third of current first-home commercial mortgage rates.

<details><summary>References</summary>
<ul>
<li><a href="https://m.dzplus.dzng.com/share/general/0/NEWS3080737PUUBKWZQDTKPG">三 部 门：将个 人 消费 贷 款 财 政 贴 息 政 策 实施期限延长至 2026 ...</a></li>
<li><a href="https://sinocism.com/p/incremental-policy-support-wang-yis">Incremental policy support; Wang Yi&#x27;s message to Japan - Sinocism</a></li>

</ul>
</details>

**Tags**: `#中国房地产政策`, `#首套房贷`, `#财政贴息`, `#购房补贴`, `#宏观政策`

---

<a id="item-finance-news-2"></a>
### [Premarket movers: Fair Isaac falls on mortgage-pricing change; AMD and CarMax rise](https://www.cnbc.com/2026/09/29/stocks-making-the-biggest-moves-premarket-fair-isaac-spacex-amd-more.html) ⭐️ 7.0/10

Fair Isaac shares plunged 18% in premarket trading after Federal Housing Finance Agency Director Bill Pulte said Fannie Mae and Freddie Mac will move to a single mortgage-pricing grid that includes VantageScore alongside FICO Classic. AMD rose more than 1% after acquiring AI firm World Labs for $8.2 billion, and CarMax gained more than 6% after reporting second-quarter earnings of $1.16 per share, versus the $0.73 per share FactSet analysts expected.

rss · CNBC Finance · Sep 29, 12:03

**「Background」** The FHFA directive ended FICO&\#x27;s decades-long lock on mortgage credit scoring by letting Fannie Mae and Freddie Mac use one pricing grid for both FICO Classic and VantageScore 4.0, while AMD&\#x27;s all-stock deal for World Labs is expected to close by year-end pending regulatory approval.

<details><summary>References</summary>
<ul>
<li><a href="https://www.wsj.com/tech/ai/amd-to-acquire-world-labs-for-8-2-billion-a8d03d11">AMD to Acquire World Labs for $8.2 Billion - WSJ</a></li>
<li><a href="https://arstechnica.com/ai/2026/09/amd-acquires-world-labs-ai-pioneer-fei-fei-lis-world-models-startup/">AMD acquires World Labs AI startup, upping the ante against Nvidia</a></li>
<li><a href="https://www.housingwire.com/articles/fhfa-gses-one-grid/">FHFA says GSEs will use one LLPA grid for FICO, VantageScore</a></li>
<li><a href="https://startupfortune.com/fhfa-director-bill-pulte-ends-ficos-mortgage-credit-score-monopoly/">FHFA Director Bill Pulte Ends FICO&#x27;s Mortgage Credit Score ...</a></li>

</ul>
</details>

**Tags**: `#premarket movers`, `#M&amp;A`, `#earnings`, `#mortgage pricing`, `#biotech investment`

---

<a id="item-finance-news-3"></a>
### [China Reportedly Sets Three Criteria for Humanoid Robot IPOs](https://www.cnbc.com/2026/09/29/china-criteria-humanoid-robot-ipos.html) ⭐️ 7.0/10

China&\#x27;s securities regulator has reportedly issued &quot;window guidance&quot; requiring humanoid robot startups seeking to go public to have sustainable revenue and commercial orders, narrowing losses — with one source saying a three-year forecast is needed — and core technology such as robotic brains or hands. The criteria, reported by three anonymous sources familiar with the CSRC&\#x27;s thinking, could leave only a handful or none of the sector&\#x27;s startups able to list, and neither the CSRC nor the Hong Kong stock exchange confirmed the guidance.

rss · CNBC Finance · Sep 29, 07:19

**「Background」** The criteria are being applied as &quot;window guidance&quot; — informal direction from regulators rather than published rules — and mainland Chinese companies need the China Securities Regulatory Commission&\#x27;s approval to list, including in Hong Kong. Scrutiny of the sector intensified after Unitree&\#x27;s volatile Shanghai debut in August.

**「Impact」** If enforced, the criteria would narrow the listing path for the at least two dozen humanoid-related companies that sources say have filed in Hong Kong, where mainland Chinese firms also need the CSRC&\#x27;s approval to list.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/09/29/china-criteria-humanoid-robot-ipos.html">China &#x27;s criteria for humanoid robot IPOs may be hard to meet</a></li>
<li><a href="https://cryptobriefing.com/china-slows-humanoid-robot-ipos-valuation-scrutiny/">China slows humanoid robot IPOs as scrutiny increases on valuations</a></li>

</ul>
</details>

**Tags**: `#China humanoid robots`, `#CSRC IPO rules`, `#embodied AI`, `#AI valuations`, `#Unitree IPO`

---

<a id="item-finance-news-4"></a>
### [Oracle Issues Force Majeure Notice as Stargate Data Center Faces Power-Approval Delay](https://www.bloomberg.com/news/articles/2026-09-24/oracle-cites-force-majeure-to-shield-itself-on-controversial-data-center) ⭐️ 7.0/10

Oracle has sent a force majeure notice to the developers of the Stargate project&\#x27;s Project Jupiter data center in New Mexico, which faces a possible delay in starting operations until 2028 because environmental and power-supply approvals for its planned 2.45GW microgrid have not been granted, according to a secondary summary of Bloomberg and TechCrunch reporting. The same account says the roughly $18 billion syndicated loan tied to the project is trading at a discount, and that most Stargate projects remain in construction, permitting or energy-provisioning stages, with only a few — such as the Abilene campus in Texas — in operation; no discount figure was provided, so the scale of the impact is unconfirmed.

telegram · zaihuapd · Sep 29, 05:46

**「Background」** Project Jupiter is one of the data centers planned under Stargate, the large AI computing build-out; it is located in Doña Ana County, New Mexico and is designed for 2.45 gigawatts of computing capacity, roughly the simultaneous electricity use of about 1.8 million homes. Oracle invoked force majeure — a contract clause that suspends a party&\#x27;s obligations when an uncontrollable event, here delayed environmental and power-supply permits, makes performance impossible — and reporting on the dispute says the contract already assigned the power-supply risk to Oracle rather than to the project&\#x27;s investors.

**「影响」** 如果延期成真，为该项目提供约180亿美元银团贷款的银行和投资者将承受账面减记压力——这笔债务已在折价交易——而甲骨文发出的不可抗力通知可让其在外部因素导致延期时推迟部分付款，直接挤压项目开发方的现金流。

<details><summary>References</summary>
<ul>
<li><a href="https://www.bannedbook.org/bnews/itnews/20260929/2364640.html">星际之门数据中心因电力审批延期 甲骨文发不可抗力通知 - 禁闻网</a></li>
<li><a href="https://www.huxiu.com/article/4893965.html">甲骨文巨型数据中心项目遭遇不可抗力，恐无法按期完工</a></li>
<li><a href="https://www.163.com/dy/article/L7KF56PT05198UNI.html">“AI泡沫”疑云再起! 甲骨文祭出“不可抗力”，180亿美元贷款拷问“星际之门”交付前景|融资|现金流|ai泡沫|知名企业|新墨西哥州|甲骨文公司|jupiter_网易订阅</a></li>

</ul>
</details>

**Tags**: `#AI数据中心`, `#甲骨文`, `#星际之门`, `#项目融资`, `#电力审批`

---