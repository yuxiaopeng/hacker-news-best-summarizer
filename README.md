# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-08-12.md)

*最后自动更新时间: 2026-08-12 20:12:30*
## 1. 英伟达 Nemotron 3.5 闪电 和 NeMo 调车场

**原文标题**: Nvidia Nemotron 3.5 Lightning and NeMo Switchyard

**原文链接**: [https://blogs.nvidia.com/blog/nemotron-lightning-switchyard-rtx-dgx/](https://blogs.nvidia.com/blog/nemotron-lightning-switchyard-rtx-dgx/)

英伟达推出了Nemotron 3.5 Lightning和NeMo Switchyard，旨在增强智能体AI，并强调开放模型和完全部署控制。

Nemotron 3.5 Lightning是一款300亿参数的混合专家模型，专为高效率、长期运行的智能体AI工作负载和专用任务而设计。它能将输出速度提高多达4倍，任务完成速度加快30%，并达到前沿水平的准确性。作为一款开放且可定制的模型，它可以使用英伟达NeMo进行二次训练，以实现领域特定的准确性，这一点已由CrowdStrike（网络安全）和Harvey（法律服务）等合作伙伴证实。它提供灵活的部署方式，可在本地PC、工作站、数据中心或云端运行，确保隐私并利用现有基础设施。英伟达还提供训练数据和技术，包括一个强化学习数据集——Nemotron-RL-Agentic-Terminal-Pivot。

NeMo Switchyard是一个开源库，为AI智能体提供智能模型路由。它根据质量、延迟或成本等特定需求，自动将请求导向最合适、最高效的模型（无论是来自开放、专有还是英伟达的模型），而无需开发者重写应用程序。这提升了“token经济效益”和效率；内部基准测试显示，它在保持前沿水平准确性的同时，显著降低了成本。包括LangChain、LiteLLM和Cognition在内的多家合作伙伴正在集成Switchyard，以实现成本降低和效率提升。

Nemotron 3.5 Lightning和NeMo Switchyard共同赋能企业，使其在AI部署、运营效率以及针对不同硬件上不断演进的智能体系统的定制化方面拥有更大的控制权。这两款产品均已在各种平台上供开发者使用。

---

## 2. 停止扼杀游戏：是时候起诉索尼了，加入我们

**原文标题**: Stop Killing Games: It's time to sue Sony, join us

**原文链接**: [https://www.massaschadeconsument.nl/collectieve-acties/playstation/](https://www.massaschadeconsument.nl/collectieve-acties/playstation/)

Stichting Massaschade & Consument（大规模损害与消费者基金会）已发起“公平PlayStation”倡议，起诉索尼对其PlayStation数字游戏征收所谓的“不公平的索尼税”。核心论点是，索尼利用其作为PlayStation主机唯一数字游戏分销商的垄断地位，人为地抬高PlayStation商店中的价格。

消费者声称，数字游戏通常比实体游戏贵20-25欧元，尽管数字游戏的发行、生产和物流成本更低。他们强调竞争的缺失，并将其与PC平台进行对比，在PC平台上，用户可以在Steam和Epic等各种商店中进行选择。此外，玩家们还对未能真正拥有数字购买物、无法转售以及索尼市场主导地位被认为的剥削感到沮丧，尤其影响到仅拥有数字版PS5的主机用户。

该基金会旨在寻求公平的游戏价格，并为多付费的用户争取赔偿。PlayStation玩家可以无义务地加入集体诉讼；如果成功，参与者可能会获得超额支付款项的退款，且诉讼费用将由部分赔偿金支付。法律诉讼正在荷兰法院进行中，最近已举行口头听证会，预计法院将于2026年10月之后就初步事项作出裁决。

---

## 3. 格罗克 4.6

**原文标题**: Grok 4.6

**原文链接**: [https://x.ai/news/grok-4-6](https://x.ai/news/grok-4-6)

SpaceXAI 于2026年8月12日推出了Grok 4.6，作为Grok 4.5的升级版，尤其侧重于长时间运行的代理以及复杂的交互式和可视化工作。这一新模型擅长处理复杂的、多步骤的任务，从研究分析到开发精良的应用，再到跨代码库工作。

Grok 4.6 达到了前沿智能水平，在人工智能分析指数上与GPT-5.6 Sol持平，并在GDPVal-AA、DeepSWE 1.1、CursorBench 3.2和FrontierCode 1.1等基准测试中表现出色，经常超越Grok 4.5，并与Fable 5 Max展开激烈竞争。

它的训练包括一次更长的补充运行，使用了精选的模型生成数据、高质量的工程数据和一个改进的优化器，随后进行了精细化的SFT和RL阶段。这使得Grok 4.6能够将宽泛的产品构想转化为可用的初版，进行研究，实现核心交互，并执行自测和验证。它还在视觉和交互项目中生成更出色的初步成果。

安全防护措施已得到增强和校准，其中包含了广泛的部署前、部署后以及第三方测试。

Grok 4.6 今日起可在Cursor、Grok Build、通过API以及OpenRouter、Vercel和Cloudflare等合作伙伴处获取。定价为每百万输入令牌2美元，每百万输出令牌6美元，更快的版本价格翻倍。用户在首周内可在Grok Build和Cursor中获得双倍的使用额度。

---

## 4. Show HN：Woxi — 开源的 Mathematica / Wolfram 语言重新实现

**原文标题**: Show HN: Woxi - Open-source Mathematica / Wolfram Language reimplementation

**原文链接**: [https://woxi.ad-si.com](https://woxi.ad-si.com)

Woxi 是一个新宣布的开源项目，它重新实现了 Mathematica/Wolfram 语言。它直接与 Jupyter 生态系统集成，作为一个 Jupyter 内核发布。

用户既可以通过使用 `woxi install-kernel` 在本地安装 Woxi 来访问它，也可以通过其捆绑的 JupyterLite 实例，直接在网络浏览器中运行完整的笔记本体验，且无需在本地进行安装。这使得 Woxi 成为那些寻求计算笔记本开源选项的人们一个易于访问的替代方案。

---

## 5. LLM擅长哪种数学？

**原文标题**: What sort of maths are LLMs good at?

**原文链接**: [https://gowers.wordpress.com/2026/08/12/what-sort-of-maths-are-llms-good-at/](https://gowers.wordpress.com/2026/08/12/what-sort-of-maths-are-llms-good-at/)

本文探讨了大型语言模型（LLM）擅长的数学问题类型，其灵感来源于一个假设的未来：OpenAI已经解决了诸如非索菲群的构造以及多色拉姆齐数新下界等重大问题。

核心问题在于LLM是否特别擅长寻找反例。尽管在这一假设情景下，LLM的许多显著成就都涉及证伪猜想，但作者认为“反例”的定义是复杂的。仅仅否定一个全称量化语句是不够的；例如，维诺格拉多夫定理在逻辑结构上与格鲁斯金关于巴拿赫-马祖尔直径的“例子”相似，但前者是定理，后者是例子。关键区别通常在于哪些变量“有趣”到值得去证明，以及构造本身的内在难度。

作者提出，如果一个对象的存在证伪了一个数学家们“有充分理由相信”的命题，那么它通常被称为“反例”。如果随着时间的推移，由于尝试失败，人们对一个猜想的信念减弱，那么一个证伪该猜想的对象可能更多地被视为“例子”而非“反例”。运用这一观点，非索菲群的构造可能更适合被称为一个“例子”，因为许多专家已经怀疑索菲性猜想。同样，拉姆齐数的结果只有对于那些坚信指数界限的人来说才是一个反例。

最终，LLM似乎擅长生成特定的实例或构造来证伪一般性陈述，但人类先前的信念以及问题的“趣味性”决定了这样一个结果是归类为“定理”、“例子”还是真正的“反例”。

---

## 6. Grok 4.6 在人工智能分析智能指数中得分 61。

**原文标题**: Grok 4.6 scores 61 on the Artificial Analysis Intelligence Index

**原文链接**: [https://artificialanalysis.ai/articles/grok-4-6-benchmarks-and-analysis](https://artificialanalysis.ai/articles/grok-4-6-benchmarks-and-analysis)

SpaceXAI 的 Grok 4.6 在人工分析智能指数上取得了 61 分，使其与 OpenAI 的 GPT-5.6 Sol 并列智能前沿。这比 Grok 4.5 提升了 5 分，仅次于 Anthropic 的 Claude Opus 5 (63 分) 和 Fable 5 (62 分)。

Grok 4.6 在各种基准测试中展现出强大的智能体性能。它在 GDPval-AA v2 上取得了 1753 的 Elo 分数，仅次于 Claude Opus 5。在多轮客户服务方面的 𝜏³-Banking (50.7%) 测试中，它位列前两名；并在软件任务的 Terminal-Bench v2.1 (88.4%) 测试中，表现与领先模型相当。在针对长周期智能体知识工作的私有 AA-Briefcase 基准测试中，它取得了 Fable 5 级别的 1577 Elo 分数。

Grok 4.6 的一个显著优势是其成本效益。其标称价格保持不变，为每百万输入/输出 token 2 美元/6 美元，这使其比 Claude Opus 5 和 GPT-5.6 Sol 便宜超过 60%。这使其处于“智能与每任务成本”的帕累托前沿，每任务成本为 0.84 美元。此外，Grok 4.6 展现出卓越的轮次效率，平均在约 53 个轮次和约 0.5B 输入 token 内完成任务，显著少于 Claude Opus 5，从而为长周期智能体工作节省大量成本。其上下文窗口仍为 50 万 token。

---

## 7. CFTC declares market emergency, orders Kalshi to continue to operate in New York

**原文标题**: CFTC declares market emergency, orders Kalshi to continue to operate in New York

**原文链接**: [https://www.cftc.gov/PressRoom/PressReleases/9281-26](https://www.cftc.gov/PressRoom/PressReleases/9281-26)

The Commodity Futures Trading Commission (CFTC) has declared a market emergency and ordered KalshiEX, LLC to continue operating, exercising its emergency authority under the Commodity Exchange Act. This action was prompted by Kalshi's notification of an emergency after New York Attorney General Letitia James filed a lawsuit seeking to halt all event contracts nationwide and claiming over $36 billion in damages.

The CFTC asserts its legal obligation to provide a uniform national market for derivatives, ensure stability, public confidence, and protect price discovery. Chairman Michael S. Selig stated that Congress did not intend for derivatives exchanges to be regulated by a "patchwork of state gaming laws," arguing that these are interstate financial instruments operating across state lines, connecting residents nationwide, and utilizing a central clearinghouse. He emphasized that New York has no authority to regulate these national financial markets.

The Commission views state attempts to regulate CFTC-supervised entities as major market disruptions. To protect its jurisdiction granted by Congress, the CFTC has a history of challenging such state actions, having filed lawsuits against multiple states (including Arizona, New York, and others) and amicus briefs in various federal courts.

---

## 8. New Bedford police officer accused of using Flock cameras to track ex-partner

**原文标题**: New Bedford police officer accused of using Flock cameras to track ex-partner

**原文链接**: [https://newbedfordlight.org/new-bedford-police-officer-accused-of-using-flock-cameras-to-track-and-follow-ex-romantic-partner/](https://newbedfordlight.org/new-bedford-police-officer-accused-of-using-flock-cameras-to-track-and-follow-ex-romantic-partner/)

生成摘要时出错

---

## 9. Amazon backs power plant that may become top source of US climate pollution

**原文标题**: Amazon backs power plant that may become top source of US climate pollution

**原文链接**: [https://arstechnica.com/tech-policy/2026/08/amazon-funds-biggest-gas-power-plant-in-us-despite-climate-pledge/](https://arstechnica.com/tech-policy/2026/08/amazon-funds-biggest-gas-power-plant-in-us-despite-climate-pledge/)

生成摘要时出错

---

## 10. Company Offering '100% Human-Written, Never AI' Medical Research Is 100% AI

**原文标题**: Company Offering '100% Human-Written, Never AI' Medical Research Is 100% AI

**原文链接**: [https://www.404media.co/company-offering-100-human-written-never-ai-peer-review-is-entirely-ai/](https://www.404media.co/company-offering-100-human-written-never-ai-peer-review-is-entirely-ai/)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-08-12](output/hacker_news_summary_2026-08-12.md) |
| 2 | [2026-08-11](output/hacker_news_summary_2026-08-11.md) |
| 3 | [2026-08-10](output/hacker_news_summary_2026-08-10.md) |
| 4 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 5 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 6 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 7 | [2026-08-09](output/hacker_news_summary_2026-08-09.md) |
| 8 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 9 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 10 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 11 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 12 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 13 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 14 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 15 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 16 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 17 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 18 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 19 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 20 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 21 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 22 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 23 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 24 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 25 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 26 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 27 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 28 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 29 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 30 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 31 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 32 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 33 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 34 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 35 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 36 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 37 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 38 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 39 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 40 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 41 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 42 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 43 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 44 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 45 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 46 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 47 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 48 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 49 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 50 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 51 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 52 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 53 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 54 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 55 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 56 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 57 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 58 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 59 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 60 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 61 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 62 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 63 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 64 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 65 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 66 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 67 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 68 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 69 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 70 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 71 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 72 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 73 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 74 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 75 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 76 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 77 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 78 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 79 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 80 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 81 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 82 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 83 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 84 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 85 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 86 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 87 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 88 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 89 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 90 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 91 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 92 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 93 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 94 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 95 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 96 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 97 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 98 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 99 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 100 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 101 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 102 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 103 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 104 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 105 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 106 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 107 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 108 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 109 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 110 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 111 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 112 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 113 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 114 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 115 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 116 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 117 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 118 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 119 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 120 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 121 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 122 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 123 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 124 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 125 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 126 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 127 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 128 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 129 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 130 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 131 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 132 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 133 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 134 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 135 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 136 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 137 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 138 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 139 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 140 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 141 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 142 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 143 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 144 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 145 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 146 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 147 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 148 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 149 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 150 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 151 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 152 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 153 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 154 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 155 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 156 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 157 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 158 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 159 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 160 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 161 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 162 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 163 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 164 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 165 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 166 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 167 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 168 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 169 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 170 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 171 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 172 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 173 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 174 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 175 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 176 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 177 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 178 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 179 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 180 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 181 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 182 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 183 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 184 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 185 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 186 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 187 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 188 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 189 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 190 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 191 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 192 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 193 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 194 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 195 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 196 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 197 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 198 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 199 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 200 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 201 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 202 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 203 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 204 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 205 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 206 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 207 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 208 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 209 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 210 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 211 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 212 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 213 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 214 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 215 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 216 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 217 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 218 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 219 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 220 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 221 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 222 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 223 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 224 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 225 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 226 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 227 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 228 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 229 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 230 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 231 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 232 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 233 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 234 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 235 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 236 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 237 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 238 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 239 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 240 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 241 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 242 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 243 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 244 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 245 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 246 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 247 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 248 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 249 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 250 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 251 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 252 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 253 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 254 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 255 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 256 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 257 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 258 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 259 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 260 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 261 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 262 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 263 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 264 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 265 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 266 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 267 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 268 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 269 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 270 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 271 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 272 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 273 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 274 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 275 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 276 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 277 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
