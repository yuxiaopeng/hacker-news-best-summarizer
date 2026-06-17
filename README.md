# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-06-17.md)

*最后自动更新时间: 2026-06-17 21:33:00*
## 1. AI 对工程纪律的要求更高，而非更低。

**原文标题**: AI demands more engineering discipline. Not less

**原文链接**: [https://charitydotwtf.substack.com/p/ai-demands-more-engineering-discipline](https://charitydotwtf.substack.com/p/ai-demands-more-engineering-discipline)

文章《AI需要更多的工程规范，而非更少》论证了，随着AI系统从研究实验室走向关键生产环境，它们对传统软件开发中严格的工程规范要求只会更高，而非更低。作者认为，当前AI开发中普遍存在的“快速行动，打破常规”的心态，考虑到AI日益增长的影响力，是不可持续且危险的。

核心论点是AI引入了独特的挑战——例如非确定性、复杂的故障模式、伦理影响和数据依赖性——这些挑战更突显了对健全工程实践的需求。这些实践包括对数据完整性、模型性能和偏差进行全面测试；在生产环境中对模型行为进行强有力的可观测性；复杂的可靠性工程以处理漂移和操作故障；以及为提高透明度和可维护性而进行的详尽文档编写。

文章强调，忽视这些规范会导致重大风险，包括安全漏洞、运行崩溃、伦理违规和可扩展性问题。它主张AI/ML工程应超越其实验阶段，采纳已有的软件工程原则，如架构设计、依赖管理和安全内建，以构建安全、可靠、值得信赖的AI系统。作者总结道，AI的未来取决于对工程卓越的这一承诺。

---

## 2. 谷歌浏览器更新将堵死广告拦截器

**原文标题**: Google Chrome update will close the door on ad blockers

**原文链接**: [https://9to5google.com/2026/06/15/google-chromes-next-update-will-mark-the-end-of-popular-ad-blockers/](https://9to5google.com/2026/06/15/google-chromes-next-update-will-mark-the-end-of-popular-ad-blockers/)

Google Chrome 正在最终确定其扩展程序向 Manifest V3 的过渡，此举将有效终止对许多流行广告拦截器（包括 uBlock Origin）的支持。这一期待已久的改变堵住了 Manifest V2 扩展程序的最后一个漏洞。

关键一步是移除 Chromium 中的 "kExtensionManifestV2Disabled" 标志，该标志曾允许部分 V2 广告拦截器继续运行。尽管用户批评此举对广告拦截器造成影响，谷歌仍以维护 V2 支持所带来的复杂性、技术债务和安全风险为由为其辩护。

预计于 2026 年 6 月 30 日发布的 Chrome 150 将移除这一主要的临时技术方案。随后，2026 年 7 月发布的 Chrome 151 将彻底清除所有剩余的 Manifest V2 相关标志。

尽管微软 Edge 和 Opera 等其他基于 Chromium 的浏览器很可能会效仿，但谷歌指出它们可以选择继续支持 Manifest V2。此次更新标志着浏览器扩展生态系统的一次重大转变，尤其是在广告拦截功能方面。

---

## 3. 无人经济？技术上并非不可能。

**原文标题**: Peopleless economy? Not technically impossible

**原文链接**: [https://gmalandrakis.com/writings/ad-economicum.html](https://gmalandrakis.com/writings/ad-economicum.html)

G. M. A. Landrakis 的文章《无人经济？技术上并非不可能》探讨了在很大程度上不再需要人类劳动作为生产投入的经济体的技术可行性。尽管看似反乌托邦，作者认为人工智能和机器人技术的进步使得这样的未来变得可信。

核心思想是，自主系统可以执行体力劳动和认知任务，从制造和物流到复杂的决策和创造性过程。这并非意味着人类的完全消失，而是他们在生产角色上的大幅减少。在这样的经济体中，挑战将从“生产”转向“分配”。如果劳动不再是主要的收入来源，社会将需要新的财富分配模式，例如全民基本收入，以确保人们能够消费。

该文章强调的是“技术”可能性，而非即时的必然性或可取性。它提出了关于人类目的、意义以及如果自动化生产资料的所有权高度集中可能导致的不平等问题，这些都是深刻的社会和哲学问题。尽管这一转变将是渐进的，但这一前景要求我们重新思考经济结构、社会保障网络，以及在一个人类劳动可能在很大程度上变为可选的世界中，工作的定义本身。

---

## 4. RFC 10008：新的HTTP查询方法

**原文标题**: RFC 10008: The new HTTP Query Method

**原文链接**: [https://www.rfc-editor.org/info/rfc10008/](https://www.rfc-editor.org/info/rfc10008/)

RFC 10008 引入了 HTTP QUERY 方法，这是一份于 2026 年 6 月发布的新互联网标准跟踪文档，旨在解决使用 GET 和 POST 进行复杂数据检索时面临的不足。

尽管 GET 方法是安全且幂等的，但它对 URI 查询字符串的依赖限制了查询大小，导致表达某些数据类型效率低下，并因日志记录引发隐私问题。POST 方法可以在请求体中携带大量查询数据，但它通常既不安全也不幂等，这阻碍了自动重试、缓存以及在没有预先服务器知识情况下的清晰语义理解。

QUERY 方法弥补了这一空白，它允许客户端在请求体中发送复杂的查询参数，这与 POST 类似。关键是，QUERY 请求被明确定义为**安全**且**幂等**的。这确保了处理这些请求不会改变目标资源的状态，并且可以重复执行而无需担心意外的副作用。这些特性促进了关键的 HTTP 功能，例如缓存、自动重试和可预测的客户端行为。

QUERY 方法的关键方面包括：
*   使用请求内容及其媒体类型来定义查询。
*   支持请求（例如 `Content-Type`）和响应（例如 `Accept`）的内容协商。
*   允许服务器返回代表查询结果的 URI 的 `Content-Location`，或代表查询操作本身的 URI 的 `Location`，后者可以通过 GET 方法检索。
*   对 QUERY 请求的响应是可缓存的，缓存键包含请求内容和元数据。
*   引入 `Accept-Query` 头字段，供服务器通告支持的查询媒体类型。

QUERY 方法在 HTTP 框架内提供了一种语义清晰、健壮且功能丰富的高级数据检索机制。

---

## 5. GPT-NL：荷兰主权语言模型

**原文标题**: GPT‑NL: a sovereign language model for the Netherlands

**原文链接**: [https://www.tno.nl/en/digital/artificial-intelligence/gpt-nl/](https://www.tno.nl/en/digital/artificial-intelligence/gpt-nl/)

GPT-NL是TNO、SURF和荷兰法医研究所（NFI）合作的一个项目，旨在开发一个主权荷兰语语言模型和生态系统，目标是增强荷兰和欧洲的数字自主权。该项目解决了围绕人工智能技术控制、数据使用以及隐私、版权和透明度等公共价值观维护的关键问题。

该倡议建立在四个核心价值观之上：
1.  **主权的**：在荷兰/欧洲境内开发，确保对模型、数据和选择的完全控制，从而避免对非欧洲提供商的依赖，并符合国家法律和社会目标。
2.  **开放透明的**：特点是数据收集和训练选择有清晰的文档，代码开源，提供详细的数据集洞察，以及在受控许可证下提供模型权重以确保问责制。
3.  **可信赖的**：完全从零开始训练，以防止继承现有模型的问题。数据收集遵守严格标准，包括保护知识产权、匿名化个人数据以及排除机密或有害内容。
4.  **互惠的**：通过内容委员会与数据提供商和权利持有人合作，确保公平协议，提供对未来发展的投入，并与创作者分享收益。

此外，GPT-NL优先考虑高效利用资源，优化能源和水消耗。该项目由荷兰企业管理局公共资助1350万欧元，彰显了其在国家层面的重要性，旨在证明强大的AI可以负责任地开发，同时维护公共价值观。产品经理Saskia Lensink和研发经理Frank Brinkkemper是该项目的关键人物。

---

## 6. 美国电池制造产量持续创新高

**原文标题**: US battery manufacturing output continues to break records

**原文链接**: [https://fred.stlouisfed.org/series/IPG33591S](https://fred.stlouisfed.org/series/IPG33591S)

提供的网址（`https://fred.stlouisfed.org/series/IPG33591S`）链接到一个名为“工业生产：制造业：非金属矿物制品制造”（指数2017=100，经季节性调整）的FRED数据系列，而非一篇专门关于“美国电池制造业产出”的文章。

分析这一非金属矿物制品制造数据系列，揭示出产出的显著增长趋势。继2020年初急剧下滑之后，该部门（包括水泥、玻璃和陶瓷等材料）的生产强劲反弹并持续达到高位。工业生产指数在2020年初跌破90后，稳步攀升，到2022年末和2023年初已超过110，这比疫情前的水平有了大幅增长。尽管存在轻微的月度波动，但总体趋势表明持续而强劲的增长，这表明非金属矿物制品制造部门的产出近期确实已达到或接近历史新高，并在最新可用数据中保持了这些强劲水平。

---

## 7. 美国暂缓将DeepSeek和逾百家被视为安全风险的公司列入黑名单

**原文标题**: US holds off blacklisting DeepSeek, more than 100 firms deemed security risks

**原文链接**: [https://www.reuters.com/world/china/us-holds-off-blacklisting-chinas-deepseek-more-than-100-firms-deemed-security-2026-06-17/](https://www.reuters.com/world/china/us-holds-off-blacklisting-chinas-deepseek-more-than-100-firms-deemed-security-2026-06-17/)

无法访问文章链接。

---

## 8. Why I email complete strangers

**原文标题**: Why I email complete strangers

**原文链接**: [https://www.goodinternetmagazine.com/why-i-email-complete-strangers/](https://www.goodinternetmagazine.com/why-i-email-complete-strangers/)

生成摘要时出错

---

## 9. 'Ghost jobs' could soon be illegal in New York

**原文标题**: 'Ghost jobs' could soon be illegal in New York

**原文链接**: [https://www.fastcompany.com/91558427/ghost-jobs-could-soon-be-illegal-in-new-york](https://www.fastcompany.com/91558427/ghost-jobs-could-soon-be-illegal-in-new-york)

生成摘要时出错

---

## 10. Leaked OpenAI financials show $38.5B loss and compute burn

**原文标题**: Leaked OpenAI financials show $38.5B loss and compute burn

**原文链接**: [https://runtimewire.com/article/openai-leaked-financials-altman-compute-burn](https://runtimewire.com/article/openai-leaked-financials-altman-compute-burn)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 2 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 3 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 4 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 5 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 6 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 7 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 8 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 9 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 10 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 11 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 12 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 13 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 14 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 15 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 16 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 17 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 18 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 19 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 20 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 21 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 22 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 23 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 24 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 25 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 26 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 27 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 28 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 29 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 30 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 31 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 32 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 33 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 34 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 35 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 36 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 37 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 38 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 39 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 40 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 41 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 42 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 43 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 44 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 45 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 46 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 47 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 48 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 49 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 50 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 51 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 52 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 53 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 54 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 55 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 56 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 57 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 58 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 59 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 60 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 61 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 62 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 63 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 64 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 65 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 66 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 67 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 68 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 69 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 70 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 71 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 72 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 73 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 74 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 75 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 76 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 77 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 78 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 79 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 80 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 81 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 82 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 83 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 84 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 85 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 86 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 87 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 88 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 89 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 90 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 91 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 92 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 93 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 94 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 95 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 96 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 97 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 98 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 99 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 100 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 101 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 102 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 103 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 104 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 105 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 106 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 107 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 108 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 109 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 110 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 111 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 112 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 113 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 114 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 115 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 116 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 117 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 118 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 119 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 120 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 121 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 122 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 123 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 124 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 125 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 126 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 127 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 128 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 129 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 130 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 131 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 132 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 133 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 134 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 135 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 136 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 137 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 138 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 139 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 140 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 141 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 142 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 143 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 144 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 145 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 146 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 147 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 148 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 149 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 150 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 151 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 152 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 153 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 154 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 155 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 156 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 157 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 158 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 159 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 160 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 161 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 162 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 163 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 164 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 165 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 166 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 167 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 168 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 169 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 170 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 171 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 172 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 173 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 174 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 175 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 176 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 177 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 178 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 179 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 180 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 181 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 182 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 183 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 184 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 185 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 186 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 187 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 188 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 189 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 190 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 191 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 192 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 193 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 194 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 195 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 196 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 197 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 198 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 199 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 200 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 201 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 202 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 203 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 204 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 205 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 206 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 207 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 208 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 209 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 210 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 211 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 212 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 213 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 214 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 215 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 216 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 217 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 218 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 219 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 220 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 221 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 222 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
