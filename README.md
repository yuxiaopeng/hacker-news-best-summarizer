# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-11-13.md)

*最后自动更新时间: 2026-11-13 00:34:04*
## 1. 黄仁勋辞职

**原文标题**: Jensen Huang resigns

**原文链接**: [https://apnews.com/article/nvidia-megaspeed-china-singapore-huang-5403f152a601cf82ce939f1d24fffa0f](https://apnews.com/article/nvidia-megaspeed-china-singapore-huang-5403f152a601cf82ce939f1d24fffa0f)

无法访问文章链接。

---

## 2. 蒂姆·彼得斯去世了

**原文标题**: Tim Peters has died

**原文链接**: [https://discuss.python.org/t/in-memoriam-tim-peters-1952-2026/110028](https://discuss.python.org/t/in-memoriam-tim-peters-1952-2026/110028)

吉多·范罗苏姆于7月15日宣布蒂姆·彼得斯去世，表达了深切的悲痛，并肯定了彼得斯对Python的巨大影响。彼得斯因撰写“Python之禅”（PEP 20）而广为人知，并且是吉多的导师和语言共同设计者。

Python初次发布后不久，彼得斯就做出了重大贡献，例如倡导混合整型/浮点型算术。他成为了Python邮件列表上的常客，因其无数、耐心且幽默的回答——这些回答常带有“<wink>”标记——而赢得了“Timbot”的昵称。

彼得斯在深入的设计讨论中发挥了关键作用，他利用其丰富的数学知识和编译器经验，预防了设计缺陷并解决了复杂问题。他在为早期核心开发设定建设性基调方面发挥了重要作用，总是清晰地解释其原理。他的遗产还包括Timsort，一种于2002年为Python列表设计的排序算法，后来被Java和Android采用。吉多强调，如果没有蒂姆·彼得斯，Python就不会是今天的样子。

---

## 3. 英伟达准备罢免黄仁勋

**原文标题**: Nvidia is preparing to oust Jensen Huang

**原文链接**: [https://www.wsj.com/business/nvidia-is-preparing-to-oust-nvidia-ceo-jensen-huang-30f421ad](https://www.wsj.com/business/nvidia-is-preparing-to-oust-nvidia-ceo-jensen-huang-30f421ad)

无法访问文章链接。

---

## 4. 我的AI代理发现了一处未探明的玛雅遗址？

**原文标题**: My AI agents found an unmapped Maya site?

**原文链接**: [https://pietromiotti.com/latest/maya-site](https://pietromiotti.com/latest/maya-site)

作为人工智能能力的一个显著例证，作者委托多个AI代理（Gemini、ChatGPT、Claude、Grok）分析NASA激光雷达数据，以在墨西哥寻找未绘制地图的玛雅考古遗址。受希拉姆·宾厄姆发现马丘比丘的启发，作者旨在了解现代工具能取得怎样的成就。

在72小时内，这些代理处理了1,200平方公里的丛林激光雷达数据，识别出大量结构。他们标记了一个重要的村落，其特征包括一个广场、一座8-12米高的椭圆形金字塔、一个高架庭院和一个潜在的水库，所有这些都隐藏在森林冠层之下。这些代理生成了一份报告，非考古学家的作者将该报告提交给了墨西哥国家人类学和历史研究所（INAH）。

INAH最初证实，在给定坐标处没有已注册的考古遗址，这让作者相信这是一个新发现。然而，一份更新披露，考古学家已在Estrada-Belli等人2025年的研究中绘制了该遗址的地图，这意味着这些代理是“重新发现”了它，而非原创性发现，因为它尚未被INAH登记在册。

尽管如此，作者强调了AI代理在处理和分析复杂数据方面令人难以置信的速度和效率。这一经历凸显了人工智能在普及科学探索方面的潜力，通过利用计算能力和好奇心，使非专业人士也能为考古学等领域做出贡献。作者总结道，人工智能有望彻底改变所有科学，使好奇心和想象力成为发现的主要瓶颈。

---

## 5. AWS模拟器

**原文标题**: AWS emulator

**原文链接**: [https://github.com/aws/aws-emulator](https://github.com/aws/aws-emulator)

AWS模拟器是一个本地工具，旨在模拟AWS API，使开发人员无需调用实际AWS服务即可构建和测试软件。它可以在本地、开发服务器或CI环境中运行，无需AWS账户，也不产生服务费用。它仅用于构建和测试，不适用于生产工作负载或安全测试。

该模拟器作为一个提供AWS API端点的本地程序运行。用户可以通过环境变量（服务器模式）配置AWS CLI或SDK指向此端点。对于Rust项目，嵌入式模式允许模拟器在进程内运行，将其HTTP客户端直接连接到SDK中以进行隔离测试。

安装方法包括使用AI编码代理技能、安装Linux软件包、通过Docker在Windows/macOS上运行，或作为开发依赖项添加到Rust嵌入式测试中。从源代码构建（修改或嵌入式模式所需）需要Rust工具链、C编译器和大量磁盘空间（100 GB）。

已知问题和服务保真度分数发布在发布页面上，并在GitHub Issues中进行跟踪。

AWS模拟器默认收集匿名使用遥测数据，侧重于数据最小化并排除敏感用户数据。这可以通过命令行选项、环境变量、配置文件或嵌入式API禁用。错误和保真度差距可以在GitHub Issues上报告。该项目在CC0 1.0通用许可下授权，供应商代码在Apache 2.0许可下；不接受拉取请求。

---

## 6. 安索罗匹克上市

**原文标题**: Anthropic IPO

**原文链接**: [https://ipo.anthropic.com/us/](https://ipo.anthropic.com/us/)

Anthropic, a public benefit corporation dedicated to securing AI's benefits and mitigating its risks, is launching an Initial Public Offering (IPO) on Nasdaq under the ticker symbol "ANT". The company asserts AI is a profoundly consequential technology capable of accelerating scientific innovation, economic growth, and solving complex problems.

For Q3'26, Anthropic reported robust financial highlights: $17.0 billion in revenue, a >12x year-over-year increase, and over 11,900 customers spending ≥ $100K TTM revenue, also growing >12x YoY. They achieved a >4x compute efficiency gain since Q1'25 and a 15% Adjusted Operating Margin. A reported $23.3 billion Net Loss was primarily due to a non-cash charge from an increase in valuation of convertible notes and derivative liabilities.

Customer success stories include Legora (scaling agentic OS for lawyers), Eli Lilly (empowering scientists), Rakuten (driving innovation and autonomous coding), Salesforce (re-engineering enterprise operations), and Walmart (enhancing shopping and engineering productivity). These cases demonstrate Claude's impact on efficiency, innovation, and user experience across diverse industries.

The IPO roadshow starts November 10th (EST). The final share price is expected November 18th (EST), with public trading commencing November 19th (EST). Investors can request shares through participating brokerage platforms. Anthropic advises reviewing their prospectus for detailed information.

---

## 7. United Airlines bans AI agents from booking flights on behalf of travelers

**原文标题**: United Airlines bans AI agents from booking flights on behalf of travelers

**原文链接**: [https://www.cbsnews.com/news/united-airlines-bans-ai-agents-booking-flights/](https://www.cbsnews.com/news/united-airlines-bans-ai-agents-booking-flights/)

United Airlines has announced a ban on artificial intelligence (AI) agents booking flights on behalf of travelers, citing security risks and potential violations of federal regulations.

The airline expressed concern that sharing personal information and payment credentials with third-party AI assistants like Meta's Muse or OpenAI's dots could expose sensitive data, lead to unintended purchases, account changes, or misuse of MileagePlus miles. Additionally, United stated that using AI for tasks like flight check-in could breach federal rules, such as those requiring in-person luggage verification.

United is implementing this ban by restricting access directly on its digital platforms and indirectly through travel agencies and aggregators, updating its booking and ticketing policies accordingly. Aviation analyst Henry Harteveldt suggests United aims to retain control over the customer booking process and avoid the costs associated with a surge of AI bot flight searches.

In contrast, other airlines like Southwest are taking a different approach, allowing ChatGPT users to view their flight inventory. Harteveldt assures consumers that United fares will remain accessible through traditional aggregators like Kayak and Google Flights, meaning finding good fares won't be any more difficult, although blocking AI bots won't make it easier either.

---

## 8. A false smoke alarm almost drowned Jane Street's only NYC datacenter

**原文标题**: A false smoke alarm almost drowned Jane Street's only NYC datacenter

**原文链接**: [https://michael.bacarella.com/2026/11/10/false-smoke-alarm-jane-street-datacenter/](https://michael.bacarella.com/2026/11/10/false-smoke-alarm-jane-street-datacenter/)

这篇文章讲述了Jane Street系统团队的一个“战役故事”，详细描述了他们位于纽约广场一号的唯一纽约数据中心发生的一次近乎灾难性的事件。受知识产权考量和受“核潜艇”启发的风险文化驱动，Jane Street故意将其数据中心设在交易大厅附近，看重能够手动拔掉服务器电源线的能力。

一天晚上，附近工作的承包商不慎扬起灰尘，意外触发了虚假的烟雾警报。尽管洒水器不会仅因烟雾而启动，但警报系统被设计为关闭机房空调（CRAC）设备，以防助长火势。这导致数据中心的温度迅速升高。随着洒水管中的加压水，温度的升高意味着一旦房间达到150°F，热敏洒水头就会启动，可能摧毁所有设备。

作者，一名住在附近的系统团队成员，接到了一个紧急电话。他飞奔回办公室，进入酷热的数据中心，疯狂地工作，拔掉了服务器机架上的所有电源线。他设法将温度上升停止在143.6°F，险些避免了一场灾难。

由于市场休市，此次事件造成的停机时间极短。随后的讨论，被描述为务实的工程辩论，决定保留洒水系统但实施更严格的程序。为防止未来出现类似问题，作者开发了一个新的OCaml监控系统。该程序轮询每台Linux服务器的温度，计算平均值，并在温度升高时向团队发出警报，提供了一种高度可靠、去中心化的冷却故障检测方案，绕过了不太可靠的CRAC遥测系统。

---

## 9. 93%的油漆飞溅是有效的Perl程序 (2019年)

**原文标题**: 93% of paint splatters are valid Perl programs (2019)

**原文链接**: [https://www.mcmillen.dev/sigbovik/](https://www.mcmillen.dev/sigbovik/)

生成摘要时出错

---

## 10. Gemini 决策 API

**原文标题**: Gemini Decisions API

**原文链接**: [https://blog.google/innovation-and-ai/technology/developers-tools/gemini-decisions-api/](https://blog.google/innovation-and-ai/technology/developers-tools/gemini-decisions-api/)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-11-13](output/hacker_news_summary_2026-11-13.md) |
| 2 | [2026-11-11](output/hacker_news_summary_2026-11-11.md) |
| 3 | [2026-11-08](output/hacker_news_summary_2026-11-08.md) |
| 4 | [2026-11-10](output/hacker_news_summary_2026-11-10.md) |
| 5 | [2026-11-12](output/hacker_news_summary_2026-11-12.md) |
| 6 | [2026-11-03](output/hacker_news_summary_2026-11-03.md) |
| 7 | [2026-11-05](output/hacker_news_summary_2026-11-05.md) |
| 8 | [2026-11-06](output/hacker_news_summary_2026-11-06.md) |
| 9 | [2026-11-04](output/hacker_news_summary_2026-11-04.md) |
| 10 | [2026-11-07](output/hacker_news_summary_2026-11-07.md) |
| 11 | [2026-10-30](output/hacker_news_summary_2026-10-30.md) |
| 12 | [2026-10-28](output/hacker_news_summary_2026-10-28.md) |
| 13 | [2026-10-31](output/hacker_news_summary_2026-10-31.md) |
| 14 | [2026-11-01](output/hacker_news_summary_2026-11-01.md) |
| 15 | [2026-10-27](output/hacker_news_summary_2026-10-27.md) |
| 16 | [2026-10-29](output/hacker_news_summary_2026-10-29.md) |
| 17 | [2026-10-26](output/hacker_news_summary_2026-10-26.md) |
| 18 | [2026-10-25](output/hacker_news_summary_2026-10-25.md) |
| 19 | [2026-10-21](output/hacker_news_summary_2026-10-21.md) |
| 20 | [2026-10-23](output/hacker_news_summary_2026-10-23.md) |
| 21 | [2026-10-20](output/hacker_news_summary_2026-10-20.md) |
| 22 | [2026-10-22](output/hacker_news_summary_2026-10-22.md) |
| 23 | [2026-10-24](output/hacker_news_summary_2026-10-24.md) |
| 24 | [2026-10-16](output/hacker_news_summary_2026-10-16.md) |
| 25 | [2026-10-17](output/hacker_news_summary_2026-10-17.md) |
| 26 | [2026-10-15](output/hacker_news_summary_2026-10-15.md) |
| 27 | [2026-10-19](output/hacker_news_summary_2026-10-19.md) |
| 28 | [2026-10-18](output/hacker_news_summary_2026-10-18.md) |
| 29 | [2026-10-11](output/hacker_news_summary_2026-10-11.md) |
| 30 | [2026-10-10](output/hacker_news_summary_2026-10-10.md) |
| 31 | [2026-10-14](output/hacker_news_summary_2026-10-14.md) |
| 32 | [2026-10-13](output/hacker_news_summary_2026-10-13.md) |
| 33 | [2026-10-09](output/hacker_news_summary_2026-10-09.md) |
| 34 | [2026-10-07](output/hacker_news_summary_2026-10-07.md) |
| 35 | [2026-10-02](output/hacker_news_summary_2026-10-02.md) |
| 36 | [2026-10-03](output/hacker_news_summary_2026-10-03.md) |
| 37 | [2026-10-01](output/hacker_news_summary_2026-10-01.md) |
| 38 | [2026-10-06](output/hacker_news_summary_2026-10-06.md) |
| 39 | [2026-09-30](output/hacker_news_summary_2026-09-30.md) |
| 40 | [2026-10-04](output/hacker_news_summary_2026-10-04.md) |
| 41 | [2026-09-29](output/hacker_news_summary_2026-09-29.md) |
| 42 | [2026-09-25](output/hacker_news_summary_2026-09-25.md) |
| 43 | [2026-09-24](output/hacker_news_summary_2026-09-24.md) |
| 44 | [2026-09-22](output/hacker_news_summary_2026-09-22.md) |
| 45 | [2026-09-27](output/hacker_news_summary_2026-09-27.md) |
| 46 | [2026-09-23](output/hacker_news_summary_2026-09-23.md) |
| 47 | [2026-09-17](output/hacker_news_summary_2026-09-17.md) |
| 48 | [2026-09-21](output/hacker_news_summary_2026-09-21.md) |
| 49 | [2026-09-19](output/hacker_news_summary_2026-09-19.md) |
| 50 | [2026-09-20](output/hacker_news_summary_2026-09-20.md) |
| 51 | [2026-09-16](output/hacker_news_summary_2026-09-16.md) |
| 52 | [2026-09-18](output/hacker_news_summary_2026-09-18.md) |
| 53 | [2026-09-15](output/hacker_news_summary_2026-09-15.md) |
| 54 | [2026-09-12](output/hacker_news_summary_2026-09-12.md) |
| 55 | [2026-09-14](output/hacker_news_summary_2026-09-14.md) |
| 56 | [2026-09-13](output/hacker_news_summary_2026-09-13.md) |
| 57 | [2026-09-10](output/hacker_news_summary_2026-09-10.md) |
| 58 | [2026-09-11](output/hacker_news_summary_2026-09-11.md) |
| 59 | [2026-09-08](output/hacker_news_summary_2026-09-08.md) |
| 60 | [2026-09-03](output/hacker_news_summary_2026-09-03.md) |
| 61 | [2026-09-09](output/hacker_news_summary_2026-09-09.md) |
| 62 | [2026-09-07](output/hacker_news_summary_2026-09-07.md) |
| 63 | [2026-09-02](output/hacker_news_summary_2026-09-02.md) |
| 64 | [2026-09-04](output/hacker_news_summary_2026-09-04.md) |
| 65 | [2026-09-06](output/hacker_news_summary_2026-09-06.md) |
| 66 | [2026-09-05](output/hacker_news_summary_2026-09-05.md) |
| 67 | [2026-08-26](output/hacker_news_summary_2026-08-26.md) |
| 68 | [2026-08-31](output/hacker_news_summary_2026-08-31.md) |
| 69 | [2026-09-01](output/hacker_news_summary_2026-09-01.md) |
| 70 | [2026-08-30](output/hacker_news_summary_2026-08-30.md) |
| 71 | [2026-08-28](output/hacker_news_summary_2026-08-28.md) |
| 72 | [2026-08-29](output/hacker_news_summary_2026-08-29.md) |
| 73 | [2026-08-23](output/hacker_news_summary_2026-08-23.md) |
| 74 | [2026-08-25](output/hacker_news_summary_2026-08-25.md) |
| 75 | [2026-08-20](output/hacker_news_summary_2026-08-20.md) |
| 76 | [2026-08-18](output/hacker_news_summary_2026-08-18.md) |
| 77 | [2026-08-16](output/hacker_news_summary_2026-08-16.md) |
| 78 | [2026-08-19](output/hacker_news_summary_2026-08-19.md) |
| 79 | [2026-08-17](output/hacker_news_summary_2026-08-17.md) |
| 80 | [2026-08-24](output/hacker_news_summary_2026-08-24.md) |
| 81 | [2026-08-21](output/hacker_news_summary_2026-08-21.md) |
| 82 | [2026-08-22](output/hacker_news_summary_2026-08-22.md) |
| 83 | [2026-08-12](output/hacker_news_summary_2026-08-12.md) |
| 84 | [2026-08-10](output/hacker_news_summary_2026-08-10.md) |
| 85 | [2026-08-14](output/hacker_news_summary_2026-08-14.md) |
| 86 | [2026-08-09](output/hacker_news_summary_2026-08-09.md) |
| 87 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 88 | [2026-08-15](output/hacker_news_summary_2026-08-15.md) |
| 89 | [2026-08-11](output/hacker_news_summary_2026-08-11.md) |
| 90 | [2026-08-13](output/hacker_news_summary_2026-08-13.md) |
| 91 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 92 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 93 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 94 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 95 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 96 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 97 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 98 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 99 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 100 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 101 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 102 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 103 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 104 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 105 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 106 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 107 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 108 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 109 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 110 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 111 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 112 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 113 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 114 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 115 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 116 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 117 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 118 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 119 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 120 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 121 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 122 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 123 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 124 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 125 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 126 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 127 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 128 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 129 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 130 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 131 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 132 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 133 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 134 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 135 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 136 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 137 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 138 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 139 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 140 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 141 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 142 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 143 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 144 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 145 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 146 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 147 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 148 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 149 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 150 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 151 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 152 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 153 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 154 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 155 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 156 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 157 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 158 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 159 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 160 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 161 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 162 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 163 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 164 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 165 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 166 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 167 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 168 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 169 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 170 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 171 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 172 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 173 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 174 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 175 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 176 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 177 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 178 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 179 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 180 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 181 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 182 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 183 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 184 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 185 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 186 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 187 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 188 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 189 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 190 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 191 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 192 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 193 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 194 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 195 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 196 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 197 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 198 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 199 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 200 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 201 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 202 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 203 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 204 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 205 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 206 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 207 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 208 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 209 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 210 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 211 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 212 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 213 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 214 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 215 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 216 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 217 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 218 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 219 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 220 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 221 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 222 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 223 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 224 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 225 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 226 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 227 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 228 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 229 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 230 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 231 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 232 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 233 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 234 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 235 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 236 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 237 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 238 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 239 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 240 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 241 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 242 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 243 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 244 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 245 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 246 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 247 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 248 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 249 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 250 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 251 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 252 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 253 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 254 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 255 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 256 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 257 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 258 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 259 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 260 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 261 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 262 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 263 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 264 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 265 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 266 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 267 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 268 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 269 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 270 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 271 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 272 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 273 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 274 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 275 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 276 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 277 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 278 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 279 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 280 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 281 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 282 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 283 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 284 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 285 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 286 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 287 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 288 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 289 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 290 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 291 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 292 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 293 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 294 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 295 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 296 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 297 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 298 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 299 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 300 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 301 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 302 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 303 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 304 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 305 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 306 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 307 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 308 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 309 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 310 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 311 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 312 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 313 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 314 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 315 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 316 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 317 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 318 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 319 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 320 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 321 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 322 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 323 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 324 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 325 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 326 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 327 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 328 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 329 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 330 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 331 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 332 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 333 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 334 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 335 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 336 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 337 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 338 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 339 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 340 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 341 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 342 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 343 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 344 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 345 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 346 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 347 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 348 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 349 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 350 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 351 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 352 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 353 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 354 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 355 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 356 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 357 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 358 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 359 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 360 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 361 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 362 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
