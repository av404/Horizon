---
layout: default
title: "Horizon Summary: 2026-09-08 (ZH)"
date: 2026-09-08
lang: zh
---

> 从 33 条内容中筛选出 5 条重要资讯。

---

**科技新闻**
1. [LLM 引导程序演化刷新 Packomania 十项圆堆积纪录](#item-tech-news-1) ⭐️ 8.0/10
2. [华为时隔六年发布逻辑折叠芯片麒麟 9050 Pro](#item-tech-news-2) ⭐️ 8.0/10
3. [最高法发布 AI 纠纷司法解释：换脸与算法杀熟责任明确](#item-tech-news-3) ⭐️ 8.0/10
4. [417K 参数循环系统从单初始状态自主生成 Bad Apple 全片](#item-tech-news-4) ⭐️ 7.0/10

**财经新闻**
1. [中国向国有银行和保险公司注资 3600 亿元，规模低于预期](#item-finance-news-1) ⭐️ 8.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [LLM 引导程序演化刷新 Packomania 十项圆堆积纪录](https://www.reddit.com/r/MachineLearning/comments/1w9xlyi/llmguided_program_evolution_improves_10_bestknown/) ⭐️ 8.0/10

一项新研究使用 LLM 迭代演化优化算法，而不是直接求解圆堆积问题，在 Packomania csqv 基准上把 N=101 到 114 中 10 个数值的已知最优半径和纪录提高了 2.4%至 5.4%，整个过程仅用 15 次迭代，总 LLM 成本为 27.72 美元。研究者从简单种子求解器出发，让 LLM 根据结果记分板和先前尝试历史提出算法修改，再由独立验证器评分，保留改进而丢弃失败。Packomania 官方已独立接受这些结果。论文见 arxiv.org/abs/2609.05093，代码与优化解见 github.com/ucsandman/discovery-loop。

reddit · r/MachineLearning · /u/SIGH\_I\_CALL · 9月7日 16:54

**「背景」** Packomania csqv 是一个几何优化基准，要求排列指定数量 N 的圆并最大化所有圆的半径之和，其榜单记录长期用于衡量优化算法能力。LLM 引导的程序演化是一种将语言模型作为搜索算子的方法：模型基于历史方案和评分结果不断提出算法层面的改动，替代直接针对具体实例进行人工设计或暴力搜索。

**「影响」** 让 Packomania csqv 榜单上的 10 项纪录被 AI 演化程序刷新，并以约 28 美元的低成本展示了 LLM 程序搜索改进数值优化的可行性；相关代码和解已开源，研究者可直接复现并尝试把该循环应用于其他优化基准。

**标签**: `#LLM`, `#program evolution`, `#optimization`, `#circle packing`, `#machine learning`

---

<a id="item-tech-news-2"></a>
### [华为时隔六年发布逻辑折叠芯片麒麟 9050 Pro](https://www.news.cn/20260907/adf46c5c003240d28cc3cf6de54f9b5f/c.html) ⭐️ 8.0/10

据新华社报道，华为 7 日在广州发布 Mate XT 2 三折叠手机，搭载麒麟 9050 Pro 芯片。这是华为继 Mate40 全球发布会后，时隔六年在旗舰发布会上推出全新麒麟芯片。麒麟 9050 Pro 据称是首款采用逻辑折叠技术的高性能芯片，它将逻辑单元在单芯片内分层排布，并增设垂直互联通道，使信号传输路径更短、时延更低、性能更好。报道未提供独立测试数据，其实际性能增益仍有待验证。

telegram · zaihuapd · 9月7日 08:20

**「背景」** 麒麟 9050 Pro 是华为自 2020 年 Mate40 系列发布以来，时隔约六年再次在旗舰发布会上推出的全新麒麟芯片，搭载于 Mate XT 2 三折叠手机。该芯片采用华为所称的 LogicFolding（逻辑折叠）架构，在单芯片内将逻辑单元立体分层堆叠，并加入垂直互联通道，以缩短信号传输路径、降低时延并提升性能。外部报道称，这类 3D 堆叠工艺可以在不使用 EUV 光刻的情况下将晶体管密度较前代提升约 55%，但这些数字尚缺乏独立测试验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.archyde.com/huawei-unveils-kirin-9050-pro-chip-with-logicfolding-architecture/">Huawei Unveils Kirin 9050 Pro Chip with LogicFolding Architecture – Archyde</a></li>
<li><a href="https://www.techtimes.com/articles/326836/20260907/huawei-kirin-9050-pro-launches-logicfolding-moves-roadmap-silicon.htm">Huawei Kirin 9050 Pro Launches: LogicFolding Moves From Roadmap to Silicon</a></li>
<li><a href="https://www.digitimes.com/news/a20260907VL215/huawei-kirin-flagship-smartphone-launch-performance.html">Huawei Kirin 9050 Pro revives flagship chip launches with reported LogicFolding architecture in Mate XT 2</a></li>

</ul>
</details>

**标签**: `#Huawei`, `#Kirin`, `#semiconductors`, `#chip architecture`, `#mobile hardware`

---

<a id="item-tech-news-3"></a>
### [最高法发布 AI 纠纷司法解释：换脸与算法杀熟责任明确](https://www.cnr.cn/news/20260907/t20260907_527806795.shtml) ⭐️ 8.0/10

最高人民法院 9 月 7 日发布人工智能纠纷案件司法解释，全文共 5 部分 24 条，聚焦 AI 换脸、算法杀熟、冒充他人代言、自动驾驶和知识产权等问题。解释明确，未经同意用 AI 制作可识别的人脸、声音等可能构成人格权侵权；算法价格歧视侵害消费者权益的，相关主体应承担侵权责任；AI 冒充他人代言诱导消费的，可依法支持惩罚性赔偿请求。意见还依法规制利用人工智能实施“网络开盒”“人肉搜索”等侵害自然人隐私权的行为。这一司法解释为 AI 从业者、平台运营者和科技企业提供了更具体的司法裁判规则，直接影响相关产品合规与纠纷处理。

telegram · zaihuapd · 9月7日 09:32

**「背景」** 中国此前主要通过《民法典》人格权编以及《生成式人工智能服务管理暂行办法》《互联网信息服务算法推荐管理规定》等部门规章来规范 AI 应用，但在民事司法层面缺少针对 AI 纠纷的系统性裁判细则。该司法解释将相关法律原则转化为具体的侵权责任认定和赔偿规则，覆盖从深度合成到算法定价等常见的 AI 纠纷类型。

**「影响」** 在中国运营的 AI 应用开发者、平台和商家需重新评估换脸、声音合成、算法差异化定价、AI 代言等业务的法律风险，并相应调整技术合规措施，否则可能面临人格权侵权、惩罚性赔偿等责任。具体影响程度仍有待各级法院在个案中适用该解释时进一步明确。

**标签**: `#AI regulation`, `#deepfake`, `#algorithmic pricing`, `#legal liability`, `#China`

---

<a id="item-tech-news-4"></a>
### [417K 参数循环系统从单初始状态自主生成 Bad Apple 全片](https://www.reddit.com/r/MachineLearning/comments/1wa8rub/generating_bad_apple_autonomously_from_a_single/) ⭐️ 7.0/10

作者受 SIREN 式“将 Bad Apple 记忆为\(t,y,x\)像素坐标函数”的启发，训练了一个仅 417,129 个参数、约 1.60 MB\(FP32\)的小型循环动力系统，在推理时不接受任何时间戳输入，而是从单一初始状态\(h\_0,c\_0\)闭环滚动，自主生成整个约 6,573 帧、384×512 灰度 Bad Apple 视频。该系统由 4 门 LSTM 风格循环转移\(16,640 参数\)和 4 级双线性上采样与深度可分离卷积帧解码器\(400,361 参数\)组成，隐状态 h 和内部记忆 c 均为 64 维；在 RTX 4080 上可实现高于 200 FPS 的解码，峰值活动显存约 17.2 MB。训练采用可丢弃的 latent teacher tables、从 K=2 到 512 逐级翻倍的长度课程、sigma=0.005 状态扰动噪声、二阶差分加速度正则化，以及 AdamW/Muon 优化器，使模型能稳定展开超过训练最大视界\(512 帧\)的 6,500 多帧序列。作者已开源代码、权重和滚动/分析工具，并坦言训练过程并非严格消融、解码器仍有改进空间。

reddit · r/MachineLearning · /u/SEBADA321 · 9月8日 00:05

**「背景」** Bad Apple 是常用于测试视频生成的经典黑白动画素材。此前相关工作用 SIREN 等坐标网络把视频建模为 f\(t,y,x\)=像素的隐式函数，因此需要给定时间 t；而本文改为让一组循环隐藏状态表示连续时间流，用当前状态预测下一状态并由状态解码出当前帧，从而在生成时完全摆脱外部时钟输入。

**标签**: `#recurrent-neural-networks`, `#generative-modeling`, `#video-generation`, `#machine-learning`, `#open-source`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [中国向国有银行和保险公司注资 3600 亿元，规模低于预期](https://www.cnbc.com/2026/09/07/china-state-banks-lenders-insurers-capital-solvency-bankrupt-nim-.html) ⭐️ 8.0/10

中国财政部牵头国家机构，向三家国有银行和五家保险公司注资 3600 亿元人民币（约 540 亿美元），规模小于市场预期。相关银行和保险公司的港股周一普遍下跌，农业银行和工商银行分别下跌 2.7%和 2.3%，中国太平跌近 4%。

rss · CNBC Finance · 9月7日 23:23

**「背景」** 这是中国政府首次将此类资本补充扩大到保险公司，此前中国已向四家大型国有银行注资 5000 亿元，并承诺今年发行 3000 亿元特别国债补充大型银行资本。当前银行净息差（放贷收益与存款成本之差）处于历史低位，保险业偿付能力充足率也降至 180.6%。

**「影响」** 麦格理首席中国经济学家 Larry Hu 认为，注资短期内对经济的拉动可能有限，因为制约贷款增长的主要因素是信贷需求疲软，而非银行资本不足。

**标签**: `#China`, `#capital injection`, `#banks`, `#insurers`, `#financial policy`

---