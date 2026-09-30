---
layout: default
title: "Horizon Summary: 2026-09-30 (ZH)"
date: 2026-09-30
lang: zh
---

> 从 57 条内容中筛选出 11 条重要资讯。

---

**科技新闻**
1. [OpenAI 发布 GPT-6.1 Sol：近 Astra 智能、五分之一价格](#item-tech-news-1) ⭐️ 7.0/10
2. [America.gov 被指为 Gemini 驱动的美国政府 AI 门户](#item-tech-news-2) ⭐️ 7.0/10
3. [PS5 Relapse 漏洞利用项目引发 Hacker News 讨论](#item-tech-news-3) ⭐️ 7.0/10
4. [网页与移动对话式 AI 代理隐私分析论文](#item-tech-news-4) ⭐️ 7.0/10
5. [Anthropic 红队：GLM-5.3 实现二进制漏洞利用控制流劫持](#item-tech-news-5) ⭐️ 7.0/10
6. [Cloudflare 发布面向 AI Agent 的 cf CLI 开放测试版](#item-tech-news-6) ⭐️ 7.0/10
7. [谷歌修复 Firebase 服务端数据问题导致的 iOS 应用启动崩溃](#item-tech-news-7) ⭐️ 7.0/10

**财经新闻**
1. [财政部等三部门：首套住房商业贷款贴息政策 10 月 1 日起实施](#item-finance-news-1) ⭐️ 8.0/10
2. [盘前异动：Fair Isaac 因房贷定价调整跌 18%，AMD 以 82 亿美元收购 World Labs](#item-finance-news-2) ⭐️ 7.0/10
3. [中国据报为人形机器人企业上市设三道门槛，符合者寥寥](#item-finance-news-3) ⭐️ 7.0/10
4. [甲骨文就星际之门数据中心电力审批延期发出不可抗力通知](#item-finance-news-4) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [OpenAI 发布 GPT-6.1 Sol：近 Astra 智能、五分之一价格](https://openai.com/index/introducing-gpt-6-1-sol/) ⭐️ 7.0/10

OpenAI 发布 GPT-6.1 Sol，官方标题宣称其以五分之一的价格提供接近 Astra 的智能，但现有材料缺少完整技术规格和基准数据。分析摘要认为这是一次广受讨论且明显降价的模型发布，不过社区质疑和技术细节不足使其更像高价值更新而非突破性发布。Hacker News 评论中，minimaxir 评论称缓存输入成本为每百万 token 0.10 美元，比标准输入价格低 95%，并比 GPT-6 Sol 的缓存输入价格低 50%，认为这对 Codex 的用量提升更关键。其他评论质疑每月 200 美元乃至 500 美元订阅的合理性，并称 DeepSeek 更便宜、速度更快，智能差距可忽略。另有评论猜测 GPT-6.1 Sol 可能是原 Astra-Minor 的紧急改名，背景是 Sol 6 表现不佳而 Opus 5.5 很强，但这只是未经证实的社区说法。

hackernews · crorella · 9月29日 17:06 · [社区讨论](https://news.ycombinator.com/item?id=49896586)

**「背景」** 就在发布 6.1 Sol 之前不久，OpenAI 刚推出 GPT-6 系列的 Sol 与 Luna，并已把 GPT-6 Sol 的输入价格从每百万 token 4 美元下调至 2 美元、输出从 20 美元下调至 10 美元；6.1 Sol 延续这一路线，给出每百万输入 2 美元、缓存输入 0.10 美元、输出 10 美元的定价。标题与报道中的“Astra”是用于对标的更高端型号名称，社区评论里提到的 Astra-Minor、Sol 5.6、Opus 5.5 等型号构成了理解“接近 Astra 的智能、价格只有五分之一”这一卖点的参照。缓存输入定价之所以被评论者视为本次真正的重点，是因为它直接决定 Codex 等大量复用上下文的场景下的实际使用成本。

**「影响」** 对 OpenAI API 和 Codex 用户而言，若评论引用的缓存输入 0.10 美元/百万 token 降价属实，长上下文与高频缓存调用场景的成本将明显下降，并可能改变开发者对订阅与按量计费的取舍；但该价格细节来自社区评论，仍应以 OpenAI 官方定价为准。

**「社区讨论」** 社区整体对 GPT-6.1 Sol 的智能提升持怀疑态度：有评论称 GPT-6/Sol 6 相比 Sol 5.6 出现明显退步、Astra 在编码上不稳定，甚至猜测此次发布只是 Astra-Minor 的紧急改名。与此同时，minimaxir 认为缓存输入降至每百万 token 0.10 美元才是真正重要的宣布，而 proxysna 等用户以 DeepSeek 的低价与够用体验质疑每月 200/500 美元订阅的价值。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/introducing-gpt-6-sol-and-luna/">Introducing GPT-6 Sol and Luna - OpenAI</a></li>
<li><a href="https://venturebeat.com/technology/openais-gpt-6-1-sol-offers-astra-like-performance-at-1-5th-price-a-new-ultrafast-tier-clocks-at-300-tokens-per-second">OpenAI&#x27;s GPT-6.1 Sol offers Astra-like performance at 1/5th price. A new ...</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#GPT-6.1 Sol`, `#LLM pricing`, `#AI model releases`, `#Hacker News discussion`

---

<a id="item-tech-news-2"></a>
### [America.gov 被指为 Gemini 驱动的美国政府 AI 门户](https://america.gov/) ⭐️ 7.0/10

据 Hacker News 条目及其分析摘要，america.gov 似乎是一个新的美国政府 AI 门户，据报道由 Google Gemini 提供支持，目标是帮助超过 1 亿人访问公共资源。由于没有页面正文，具体功能、发布时间和部署范围尚不明确；评论区有用户称其实现看起来是“Gemini + 防护栏”，并引用 Google 博客称 Google 是该倡议的技术合作伙伴，利用 Gemini 帮助超过 1 亿人更快、更方便地获取关键公共资源。若相关描述准确，这将是一个大规模政府 AI 服务部署案例，但现有证据主要来自条目描述和评论，仍需官方信息确认。

hackernews · plesiv · 9月29日 14:04 · [社区讨论](https://news.ycombinator.com/item?id=49893509)

**「背景」** America.gov 是美国联邦政府新推出的人工智能驱动服务门户，据外部报道由特朗普政府于本周二上线，目标是帮助超过 1 亿美国人更便捷地获取政府服务。该门户采用包括 Google Gemini 在内的 AI 系统作为底层能力，Google 也将自身定位为这一计划的技术合作伙伴。把大模型直接放到联邦公共服务入口，意味着面向公众的政府信息服务从静态网页检索转向对话式引导，同时也需处理随之而来的内容准确性与安全边界问题。

**「影响」** 对美国公众而言，这一联邦服务门户意在让超过 1 亿人通过 Gemini 驱动的对话入口更快找到并获取公共资源，Google 与白宫公布的目标是把原本分散的政府服务检索集中到单一 AI 界面。据美国首席设计官 Joe Gebbia 称，该站点还同时使用 Elon Musk 的 Grok，因此多模型分工、实际覆盖人数与服务质量均有待官方细节与后续运行数据确认。

**「社区讨论」** 评论总体认可用聊天机器人帮人找到政府服务路径的潜在价值：maherbeg 认为这能帮人弄清该办什么、获得有资格的服务，是重大改进，同时提到人们很容易被钓鱼；mellosouls 也认为这是聊天机器人真正有用而非令人烦躁的少数场景。争议集中在模型来源与内容边界：none\_to\_remain 说有人贴截图称其为中国模型但很可能造假，他未能让这个被评论者称为 FedGPT 的系统说出底层模型，但模型能提及 1989 年 6 月 3 日至 4 日的事件；sssilver 则认为从公开信息看它像是 Gemini 加防护栏，lrvick 则注意到它对国会大厦相关法律问题的回答比预期更直白。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.facebook.com/WGME13/posts/watch-the-trump-administration-on-tuesday-launched-americagov-an-artificial-inte/1537404648414822/">WATCH: The Trump administration on Tuesday launched America.gov, an ...</a></li>
<li><a href="https://www.facebook.com/rundownnewsletter/posts/the-us-government-has-launched-americagov-a-new-ai-powered-portal-designed-to-ma/975208122267640/">The U.S. government has launched America.gov, a new AI-powered ...</a></li>
<li><a href="https://www.techbuzz.ai/articles/google-s-gemini-ai-powers-new-america-gov-federal-portal">Google&#x27;s Gemini AI Powers New America.gov Federal Portal</a></li>
<li><a href="https://blog.google/company-news/outreach-and-initiatives/public-policy/america-gov-google-public-sector/">Google Gemini powers new America.gov portal - The Keyword</a></li>
<li><a href="https://www.unite.ai/google-becomes-technology-partner-for-white-house-america-gov-launch/">Google Becomes Technology Partner for White House America.gov ...</a></li>
<li><a href="https://www.cnbc.com/2026/09/29/trump-ai-gemini-grok.html">Trump admin AI website uses Gemini, Grok: Joe Gebbia - CNBC</a></li>

</ul>
</details>

**标签**: `#AI`, `#government`, `#Gemini`, `#public services`, `#policy`

---

<a id="item-tech-news-3"></a>
### [PS5 Relapse 漏洞利用项目引发 Hacker News 讨论](https://github.com/ntfargo/Relapse-Exploit) ⭐️ 7.0/10

GitHub 上出现了由 ntfargo 维护的 PS5 漏洞利用项目 Relapse-Exploit，并在 Hacker News 上获得 235 分、128 条评论，成为近期主机安全讨论的焦点。评论者根据公开信息推测，该利用可能针对 WebKit 的 JavaScriptCore JavaScript 引擎漏洞，并讨论 PS5 上的 WebKit 是否启用了 JIT，以及索尼是否会通过禁用 JIT 来缩小攻击面。由于给定信息中没有项目技术说明或独立验证，其具体利用链、受影响固件版本和实际能力仍不明确。讨论还将这一漏洞与 PS5 的存档备份限制联系起来：有用户指出 PS5 不允许将游戏存档备份到 USB，必须依赖 PS Plus 云备份，且每个用户档案需要单独订阅。另有评论担心破解社群会保留零日漏洞，或期待该手段能带来在 PS5 上玩 Steam PC 游戏等用途。

hackernews · therepanic · 9月29日 15:44 · [社区讨论](https://news.ycombinator.com/item?id=49895304)

**「背景」** PS5 主机的固件长期封闭，相关漏洞利用通常需要先用浏览器/WebKit 层面的漏洞取得代码执行，再逐步提权。ntfargo 的 Relapse-Exploit 仓库自称是针对 PS5 7.00 至 13.60 固件的漏洞利用链，其浏览器阶段利用 JavaScriptCore（WebKit 引擎）的信息泄露，并结合 structured clone 的对象池错配来破坏 typed array，随后由监听 9021 端口的 ELF 加载器接管并注入 payload。按项目说明，使用者可在本地运行 serve.py，或在 PS5 上打开项目页面触发，且 WebKit 阶段可能需要多次重试。

**「影响」** 据外部报道，Relapse 漏洞链声称可在 7.00 至 13.60 固件的 PS5（含 Pro 机型）上实现越狱，这意味着处于该固件区间的用户可能获得运行自制软件及备份存档等原本受限的能力。不过这一说法尚未获得独立验证，索尼也可能通过后续固件更新封堵该攻击链。

**「社区讨论」** 评论区没有形成一致结论：有人关心能否借此把游戏存档备份到 USB，并批评 PS5 依赖 PS Plus 云备份且每个档案单独订阅；有人推测漏洞位于 WebKit JavaScriptCore，并担心索尼会禁用 JIT；还有人提到破解社群可能保留零日漏洞，或希望等到《GTA6》再公开，以及期待能在 PS5 上玩 Steam PC 游戏。由于缺少项目方技术细节和独立验证，这些多为猜测和诉求，而非已确认影响。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/ntfargo/Relapse-Exploit">GitHub - ntfargo/Relapse-Exploit: Exploit chain for PS5 7.00 - 13.60 · GitHub</a></li>
<li><a href="https://elsolitario.org/en/2026/09/29/relapse-repo-claims-ps5-exploit-firmware-7-00-to-13-60/">PS5 Jailbreak: What Is Relapse Exploit and Its Scope</a></li>
<li><a href="https://dev.to/lu1tr0n/relapse-repo-afirma-exploit-de-ps5-en-firmware-700-1360-1n14">Relapse: repo afirma exploit de PS5 en firmware 7.00-13.60 - DEV Community</a></li>
<li><a href="https://elsolitario.org/en/2026/09/29/relapse-repo-claims-ps5-exploit-firmware-7-00-to-13-60/">PS5 Jailbreak: What Is Relapse Exploit and Its Scope - El Solitario</a></li>
<li><a href="https://www.yardbarker.com/video_games/articles/rumor_new_ps5_jailbreak_reportedly_hits_base_and_pro_models/s1_17456_44365180">Rumor: New PS5 Jailbreak Reportedly Hits Base and Pro Models</a></li>

</ul>
</details>

**标签**: `#PS5`, `#console security`, `#WebKit`, `#JavaScriptCore`, `#exploit development`

---

<a id="item-tech-news-4"></a>
### [网页与移动对话式 AI 代理隐私分析论文](https://jorgegarciaherrero.com/wp-content/interactivos/20260916-Prompt-like-a-butterfly-sting-like-a-tracker-%28clean%29.pdf) ⭐️ 7.0/10

一份隐私分析论文（PDF）比较了网页端与移动端对话式 AI 代理在泄露用户数据方面的差异。该论文在 Hacker News 上引发讨论（408 分，130 条评论），社区评论提供了具体观察。有用户指出，ChatGPT 网页版会定期将未完成的提示发送到后端的\`conversation/prepare\`端点，未等用户实际发送；另有用户指出，部分服务（如 Perplexity）仅用 URL 中的 UUID 标识对话，访问该 URL 会暴露完整对话内容。讨论还涉及平台 API 与权限在隐私风险中的角色，以及开放模型作为替代方案的争论。由于仅能获取标题与评论片段，论文的具体方法与发现无法在现有证据下核实。

hackernews · damaru2 · 9月29日 09:03 · [社区讨论](https://news.ycombinator.com/item?id=49890226)

**「背景」** 对话式 AI 代理指 ChatGPT、Perplexity 一类以聊天界面提供模型能力的服务，它们既作为网页运行，也作为移动端 App 运行，而两条路径的数据暴露机制并不相同：网页端依赖浏览器请求与 URL，移动端则受平台 API、权限与第三方 SDK（包括广告追踪器）的约束。据社区讨论中的具体观察，网页端常见的隐私问题包括在用户按下发送前就把未完成的提示词发往后端端点（如 \`conversation/prepare\`），以及仅用 URL 中的 UUID 标识整段会话，使任何获得该链接的人都能读取完整对话。这篇论文正是对上述跟踪与数据外泄行为做系统的隐私分析，作者另提供一个可视化摘要页面，并声明若摘要与论文有出入，以论文为准。

**「影响」** 对使用网页版与移动版对话式 AI 的用户来说，最直接的后果是：尚未写完的提示草稿可能在用户点击发送前就已被发往后端接口，而仅凭带 UUID 的会话 URL 就能打开完整对话，使“分享链接”实际上等同于公开聊天记录；既有的系统性综述与用户研究也表明，这类平台的用户本就普遍对隐私、安全与信任抱有顾虑，并把对话式界面形容为令人不安。需要注意的是，上述具体行为主要来自论文与社区观察，其覆盖范围和普遍程度尚无法从现有证据中核实。

**「社区讨论」** 评论者普遍关注两类具体泄露途径：客户端在用户发送前预先传输部分提示内容，以及可访问的对话 URL 暴露完整历史记录。讨论同时存在分歧：有人认为风险主要来自平台 API 与权限，有人主张改用开放模型以规避此类问题，Perplexity 等服务的 URL 隐私问题被作为实例引用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://jorgegarciaherrero.com/en/prompt-like-a-butterfly-sting-like-a-tracker/">Infographic of the paper &quot; Prompt like a Butterfly , sting like a tracker &amp;quo...</a></li>
<li><a href="https://www.sciencedirect.com/science/article/pii/S0747563224002127">Evaluating privacy, security, and trust perceptions in conversational AI: A systematic review - ScienceDirect</a></li>
<li><a href="https://arxiv.org/html/2504.06552v1">Understanding Users’ Security and Privacy Concerns and Attitudes TowardsConversational AI Platforms</a></li>
<li><a href="https://www.sciencedirect.com/science/article/pii/S0885230821000747">Perceptions and reactions to conversational privacy initiated by a conversational user interface - ScienceDirect</a></li>

</ul>
</details>

**标签**: `#privacy`, `#conversational-ai`, `#web-security`, `#tracking`, `#mobile-platforms`

---

<a id="item-tech-news-5"></a>
### [Anthropic 红队：GLM-5.3 实现二进制漏洞利用控制流劫持](https://simonwillison.net/2026/Sep/29/anthropic-frontier-red-team/) ⭐️ 7.0/10

Anthropic 前沿红队（Frontier Red Team）在其研究文章《GLM-5.3 and the spread of advanced cyber capabilities》中报告：在内部 Binary Exploitation 基准中随机抽取的 100 项任务上，智谱 AI 的 GLM-5.3 在 4% 的试验中实现了完整的控制流劫持（control flow hijack），Claude Mythos Preview 的成功率为 6%。Anthropic 表示，GLM-5.3 的表现虽然低于 Claude Mythos Preview，但一个“有意义的门槛”显然已被跨过——更早的模型如 Claude Opus 4.6 和 GLM-5.2 在这些任务上无一成功。Simon Willison 以引文形式转发了这一结论，未附加分析或独立验证。据同一报告相关内容的转述，GLM-5.3 的安全防护还可被简单方法绕过，模拟测试成功率为 64% 至 100%，且开放权重允许用户改造模型以削弱其拒答行为，Anthropic 称这会扩大恶意行为者可用的网络攻击能力。需注意，该条目本身仅为简短引用，未提供基准方法论、任务选取细节或第三方验证。

rss · Simon Willison · 9月29日 22:20

**「背景」** GLM-5.3 是智谱 AI（Z.ai）的旗舰开放权重模型，与 GLM-5.2 共用同一基座模型，能力提升全部来自后训练。二进制利用指发现并利用已编译程序中的内存安全缺陷，「控制流劫持」是其中一类完整利用，即让程序按攻击者指定的路径执行代码；Anthropic 内部的 Binary Exploitation 基准与 ExploitBench 正是用来衡量模型能否自主完成这类任务。Anthropic 的 Frontier Red Team 负责评估前沿模型的网络攻防能力，本次即从内部基准随机抽取任务，比较 GLM-5.3、Claude Mythos Preview 以及更早的 Claude Opus 4.6、GLM-5.2 的表现。

**「影响」** 对防御方而言，这一阈值被跨过意味着过去只有熟练攻击者才能完成的内存破坏与控制流劫持利用，如今可由可获取的模型以一定成功率自主实现；已有安全研究也指出，AI 正在降低网络犯罪的门槛并推动自主攻击流程走向成熟，因此相关组织应假设此类能力会继续扩散而非停滞在当前的 4%–6%。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/research/glm-5-3-and-the-spread-of-advanced-cyber-capabilities">GLM-5.3 and the spread of advanced cyber capabilities \ Anthropic</a></li>
<li><a href="https://simonwillison.net/2026/Sep/29/anthropic-frontier-red-team/">A quote from Anthropic Frontier Red Team</a></li>
<li><a href="https://docs.z.ai/guides/llm/glm-5.3">GLM-5.3 - Overview - Z.AI DEVELOPER DOCUMENT</a></li>
<li><a href="https://aiweekly.co/alerts/anthropic-zhipus-glm-53-matches-claude-on-autonomous-exploits">Anthropic: Zhipu&#x27;s GLM-5.3 Matches Claude on Autonomous ...</a></li>
<li><a href="https://unit42.paloaltonetworks.com/autonomous-ai-cyber-attack-campaign/">Chinese-Speaking Threat Actor Harnesses AI Models for ...</a></li>
<li><a href="https://www.ncsc.gov.uk/report/impact-of-ai-on-cyber-threat">The near-term impact of AI on the cyber threat</a></li>

</ul>
</details>

**标签**: `#ai-security`, `#ai-capabilities`, `#cyber-offense`, `#large-language-models`, `#ai-safety`

---

<a id="item-tech-news-6"></a>
### [Cloudflare 发布面向 AI Agent 的 cf CLI 开放测试版](https://blog.cloudflare.com/cloudflare-cf-cli-launch/) ⭐️ 7.0/10

Cloudflare 发布了 cf CLI 开放测试版，目标是让开发者和 AI Agent 通过命令行调用 Cloudflare 的全部 API。cf 由 API Schema 生成，覆盖超过 3,000 项 API 操作；相比之下，现有的 Wrangler 约覆盖 280 种操作。该工具以 JSON 作为默认输出，并支持命令搜索和引导，方便 Agent 自动发现、执行操作并处理结果。Cloudflare 举例称，Agent 可通过同一工具创建和部署 Worker、监控服务、配置 Access 与 WAF，甚至购买域名。目前该工具处于开放测试阶段。

telegram · zaihuapd · 9月29日 13:46

**「背景」** Cloudflare 此前为开发者提供 Wrangler，这一命令行工具在长期演进中积累约 280 项功能，主要覆盖 Workers 等具体产品的开发与部署流程。新发布的 cf 则从 Cloudflare 的 API Schema 生成，并把整个平台近 3,000 项 API 操作统一到同一个命令行界面中，因此能力和覆盖面远超 Wrangler。该工具定位为面向 Agent 的命令行入口，目前处于开放测试阶段。

**「影响」** 对使用 Cloudflare 的开发者与 Agent 构建者而言，cf 把可在单一命令行工具中自动化的 API 覆盖面从 Wrangler 的约 280 项扩展到 3,000 项以上，使部署、监控与安全配置等跨产品操作可由 Agent 统一执行；不过该版本仍为开放测试版。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.cloudflare.com/cloudflare-cf-cli-launch/">Introducing cf: the agentic CLI for the entire Cloudflare API | Cloudflare Blog</a></li>
<li><a href="https://blog.cloudflare.com/cf-cli-local-explorer/">Building a CLI for all of Cloudflare | Cloudflare Blog</a></li>

</ul>
</details>

**标签**: `#Cloudflare`, `#AI agents`, `#CLI`, `#API tooling`, `#developer tools`

---

<a id="item-tech-news-7"></a>
### [谷歌修复 Firebase 服务端数据问题导致的 iOS 应用启动崩溃](https://github.com/firebase/firebase-ios-sdk/issues/16728) ⭐️ 7.0/10

谷歌确认，Google Analytics for Firebase 的 iOS 服务端曾返回格式错误的数据，导致大量集成该组件的 iOS 应用在启动时崩溃。问题始于 2026 年 9 月 28 日 17:41（美国太平洋夏令时），修复于 19:52 完成推出。谷歌表示，开发者无需更新 Firebase SDK 或应用本身。受缓存影响，部分应用可能在修复完成后再继续崩溃最长约 4 小时，残余问题会自行消退。

telegram · zaihuapd · 9月29日 16:29

**「背景」** Google Analytics for Firebase 是集成在大量 iOS 和 Android 应用中的分析组件，其 iOS SDK 通常会在应用启动时向谷歌服务端请求配置或数据载荷。当服务端返回格式错误的载荷时，SDK 未能妥善处理这种异常输入，导致应用在启动阶段崩溃；由于问题出在服务端，谷歌通过更正返回数据完成修复，因此无需更新 SDK 或应用。这一事件也引发了关于客户端 SDK 应对异常输入容错能力的讨论。

**「影响」** 对使用 Google Analytics for Firebase 的 iOS 开发者而言，这次事故无需紧急发版或升级 SDK，但部分用户仍可能在修复后的数小时内遇到启动崩溃，需等待缓存过期。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://firerun.io/firebase-ios-analytics-sdk-crash-server-side-2026/">Firebase Server Change Crashed iOS Apps, No Update Needed</a></li>
<li><a href="https://www.thenews.com.pk/latest/1418097-google-fixes-firebase-bug-that-crashed-thousands-of-iphone-apps">Google fixes firebase bug that crashed thousands of iPhone apps</a></li>
<li><a href="https://9to5google.com/2026/09/29/google-firebase-iphone-app-crash-fixed/">Google has fixed an issue that caused iPhone apps to crash</a></li>

</ul>
</details>

**标签**: `#Firebase`, `#iOS`, `#service outage`, `#Google Analytics`, `#mobile development`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [财政部等三部门：首套住房商业贷款贴息政策 10 月 1 日起实施](https://jrs.mof.gov.cn/zhengcefabu/phjr/202609/t20260929_3998312.htm) ⭐️ 8.0/10

中国财政部、中国人民银行、金融监管总局 9 月 29 日联合印发通知，自 2026 年 10 月 1 日起在全国对符合条件的首套住房商业性个人住房贷款给予年化 1 个百分点的中央财政贴息，贴息期限最长 5 年，单户可贴息贷款上限 100 万元，政策暂定实施 1 年。财政部称，需同时满足新发放贷款购买首套房（不含新贷款置换存量贷款）、住房建筑面积 120 平方米以下、房价 150 万元以下三项条件；据此测算单户每年最高贴息约 1 万元。

telegram · zaihuapd · 9月29日 10:18

**「背景」** 贴息属于财政补贴：由中央财政按贷款本金为借款人承担部分利息，而不是直接下调银行贷款利率本身。此前财政部、中国人民银行、金融监管总局已将个人消费贷款财政贴息政策的实施期限延长至 2026 年底。

**「影响」** 直接受益的是符合新购首套住房、面积 120 平方米以下且价格 150 万元以下等条件的家庭：年化 1 个百分点的财政贴息可在最长 5 年内减少其商业贷款利息支出，单户每年最多约 1 万元；用新贷款置换存量贷款的家庭不在贴息范围内。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://m.dzplus.dzng.com/share/general/0/NEWS3080737PUUBKWZQDTKPG">三 部 门：将个 人 消费 贷 款 财 政 贴 息 政 策 实施期限延长至 2026 ...</a></li>

</ul>
</details>

**标签**: `#中国房地产政策`, `#首套房贷`, `#财政贴息`, `#购房补贴`, `#宏观政策`

---

<a id="item-finance-news-2"></a>
### [盘前异动：Fair Isaac 因房贷定价调整跌 18%，AMD 以 82 亿美元收购 World Labs](https://www.cnbc.com/2026/09/29/stocks-making-the-biggest-moves-premarket-fair-isaac-spacex-amd-more.html) ⭐️ 7.0/10

9 月 29 日美股盘前，Fair Isaac 股价下跌 18%，此前美国联邦住房金融局（FHFA）局长比尔·普尔特表示，房利美和房地美将把原本分开的两套抵押贷款定价表合并为一张，并让 VantageScore 加入现有的 FICO Classic 定价表。同日，芯片厂商 AMD 宣布以 82 亿美元收购人工智能公司 World Labs，股价盘前上涨逾 1%；二手车零售商 CarMax 公布第二财季每股收益 1.16 美元、营收 78.8 亿美元，高于 FactSet 调查分析师预期的每股 73 美分和 70.9 亿美元。

rss · CNBC Finance · 9月29日 12:03

**「背景」** Fair Isaac 股价重挫源于美国联邦住房金融局（FHFA）要求房利美和房地美在常规房贷上采用统一价格表，允许 VantageScore 4.0 与 FICO Classic 并列使用，从而打破 FICO 在房贷信用评分领域长达数十年的独家地位。AMD 此次是以约 82 亿美元全股票交易收购 AI 研究公司 World Labs（由李飞飞创立），交易预计年底前完成，尚需监管批准。

**「影响」** 这一调整直接关系美国抵押贷款机构与借款人：房利美和房地美将改用单一评分表，并在 FICO Classic 之外纳入 VantageScore。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.wsj.com/tech/ai/amd-to-acquire-world-labs-for-8-2-billion-a8d03d11">AMD to Acquire World Labs for $8.2 Billion - WSJ</a></li>
<li><a href="https://arstechnica.com/ai/2026/09/amd-acquires-world-labs-ai-pioneer-fei-fei-lis-world-models-startup/">AMD acquires World Labs AI startup, upping the ante against Nvidia</a></li>
<li><a href="https://finance.yahoo.com/markets/stocks/articles/fair-isaac-shares-fall-fhfa-145931943.html?fr=sycsrp_catchall">Fair Isaac Shares Fall After FHFA Chief Says VantageScore ...</a></li>
<li><a href="https://www.housingwire.com/articles/fhfa-gses-one-grid/">FHFA says GSEs will use one LLPA grid for FICO, VantageScore</a></li>
<li><a href="https://startupfortune.com/fhfa-director-bill-pulte-ends-ficos-mortgage-credit-score-monopoly/">FHFA Director Bill Pulte Ends FICO&#x27;s Mortgage Credit Score ...</a></li>

</ul>
</details>

**标签**: `#premarket movers`, `#M&amp;A`, `#earnings`, `#mortgage pricing`, `#biotech investment`

---

<a id="item-finance-news-3"></a>
### [中国据报为人形机器人企业上市设三道门槛，符合者寥寥](https://www.cnbc.com/2026/09/29/china-criteria-humanoid-robot-ipos.html) ⭐️ 7.0/10

据三位知情人士透露，中国证监会正以&quot;窗口指导&quot;方式提高人形机器人（即&quot;具身智能&quot;）初创企业的上市门槛，要求申请企业具备可持续收入和商业订单、亏损收窄（一位人士称需提供三年预测），并拥有机器人&quot;大脑&quot;或&quot;手&quot;等核心技术。消息人士称，即便只需满足其中两项，目前也不清楚有哪家公司能够达标，因此预计最终能上市的只有少数几家甚至一家都没有。证监会未立即回应置评请求。

rss · CNBC Finance · 9月29日 07:19

**「背景」** 在中国，内地企业无论在上海等内地市场还是香港上市，都需获得中国证监会批准或备案，因此这种不公开的“窗口指导”会直接影响企业的上市进程。此前人形机器人龙头宇树科技已于 8 月 19 日获监管快速通道在上海上市，其创始人随后表示真正的商业化仍需数年，促使市场更严格地审视该行业的估值与盈利能力。

**「影响」** 据两位消息人士，仅在香港就有至少二十多家人形机器人相关具身智能公司提交了上市申请，若这一门槛落地，这些公司的上市计划以及早期投资人的退出渠道可能受到直接限制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/09/29/china-criteria-humanoid-robot-ipos.html">China &#x27;s criteria for humanoid robot IPOs may be hard to meet</a></li>
<li><a href="https://cryptobriefing.com/china-slows-humanoid-robot-ipos-valuation-scrutiny/">China slows humanoid robot IPOs as scrutiny increases on valuations</a></li>

</ul>
</details>

**标签**: `#China humanoid robots`, `#CSRC IPO rules`, `#embodied AI`, `#AI valuations`, `#Unitree IPO`

---

<a id="item-finance-news-4"></a>
### [甲骨文就星际之门数据中心电力审批延期发出不可抗力通知](https://www.bloomberg.com/news/articles/2026-09-24/oracle-cites-force-majeure-to-shield-itself-on-controversial-data-center) ⭐️ 7.0/10

据彭博报道，星际之门（Stargate）位于新墨西哥州的 Project Jupiter 数据中心因 2.45GW 配套微电网的环境与供电审批尚未落地，面临推迟至 2028 年投运的风险，甲骨文已向项目开发方发出不可抗力通知，拟在外部因素导致延期时推迟部分付款。该事件引发市场对超大型 AI 数据中心建设进度的担忧，相关 180 亿美元银团贷款出现折价交易，折价幅度未披露。

telegram · zaihuapd · 9月29日 05:46

**「背景」** 不可抗力是合同中的常规条款，指在无法控制的事件使履约变得不可能时，当事方可免除相应义务；据虎嗅报道，甲骨文援引该条款的理由是项目遭遇不可预见的审批延误、无法接通电力，但知情人士称合同已约定供电风险由甲骨文而非投资者承担。Project Jupiter 位于新墨西哥州多纳安纳县，占地约 1400 英亩，设计算力容量 2.45 吉瓦（约相当于 180 万户家庭同时用电），总投资规模约 1650 亿美元。

**「影响」** 若甲骨文按不可抗力通知推迟部分付款，该数据中心开发方的现金流将直接承压；同时，持有相关 180 亿美元银团贷款的银行与投资者已面临贷款折价交易，市场对超大型 AI 数据中心能否按期交付的担忧随之升温。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bannedbook.org/bnews/itnews/20260929/2364640.html">星际之门数据中心因电力审批延期 甲骨文发不可抗力通知 - 禁闻网</a></li>
<li><a href="https://www.huxiu.com/article/4893965.html">甲骨文巨型数据中心项目遭遇不可抗力，恐无法按期完工</a></li>
<li><a href="https://www.163.com/dy/article/L7KF56PT05198UNI.html">“AI泡沫”疑云再起! 甲骨文祭出“不可抗力”，180亿美元贷款拷问“星际之门”交付前景|融资|现金流|ai泡沫|知名企业|新墨西哥州|甲骨文公司|jupiter_网易订阅</a></li>
<li><a href="https://www.21jingji.com/article/20260924/herald/90fb07429c23fe3e48143aef58c58503.html">“AI泡沫”疑云再起! 甲骨文祭出“不可抗力”，180亿美元贷款拷问“星际之门”交付前景 - 21经济网</a></li>
<li><a href="https://cn.investing.com/news/stock-market-news/article-3582373">“AI泡沫”疑云再起! 甲骨文祭出“不可抗力”，180亿美元贷款拷问“星际之门”交付前景 提供者 智通财经</a></li>

</ul>
</details>

**标签**: `#AI数据中心`, `#甲骨文`, `#星际之门`, `#项目融资`, `#电力审批`

---