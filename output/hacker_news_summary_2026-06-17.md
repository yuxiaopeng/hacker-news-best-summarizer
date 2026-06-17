# Hacker News 热门文章摘要 (2026-06-17)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

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

## 11. Wolfram Language and Mathematica version 15

**原文标题**: Wolfram Language and Mathematica version 15

**原文链接**: [https://writings.stephenwolfram.com/2026/06/launching-version-15-of-wolfram-language-mathematica-built-in-useful-ai-lots-of-new-core-functionality/](https://writings.stephenwolfram.com/2026/06/launching-version-15-of-wolfram-language-mathematica-built-in-useful-ai-lots-of-new-core-functionality/)

生成摘要时出错

---

## 12. Qwen-Robot Suite: A Foundation Model Suite for Physical World Intelligence

**原文标题**: Qwen-Robot Suite: A Foundation Model Suite for Physical World Intelligence

**原文链接**: [https://qwen.ai/blog?id=qwen-robotsuite](https://qwen.ai/blog?id=qwen-robotsuite)

生成摘要时出错

---

## 13. Claude: Elevated errors across many models [resolved]

**原文标题**: Claude: Elevated errors across many models [resolved]

**原文链接**: [https://status.claude.com/incidents/xmhsglsz3h3w](https://status.claude.com/incidents/xmhsglsz3h3w)

生成摘要时出错

---

## 14. The founder's playbook: Building an AI-native startup

**原文标题**: The founder's playbook: Building an AI-native startup

**原文链接**: [https://claude.com/blog/the-founders-playbook](https://claude.com/blog/the-founders-playbook)

生成摘要时出错

---

## 15. I've always wondered if anyone used sharing buttons on news sites and blogs

**原文标题**: I've always wondered if anyone used sharing buttons on news sites and blogs

**原文链接**: [https://ankursethi.com/links/nobody-clicks-your-share-buttons/](https://ankursethi.com/links/nobody-clicks-your-share-buttons/)

生成摘要时出错

---

## 16. Commodore Releases Flip Phone

**原文标题**: Commodore Releases Flip Phone

**原文链接**: [https://commodore.net/why-a-flip-phone/](https://commodore.net/why-a-flip-phone/)

生成摘要时出错

---

## 17. Humanity isn't ready for the coming intelligence explosion

**原文标题**: Humanity isn't ready for the coming intelligence explosion

**原文链接**: [https://www.economist.com/by-invitation/2026/06/15/humanity-isnt-ready-for-the-coming-intelligence-explosion](https://www.economist.com/by-invitation/2026/06/15/humanity-isnt-ready-for-the-coming-intelligence-explosion)

生成摘要时出错

---

## 18. 10Gb/s Ethernet: switching to a Broadcom SFP+ module

**原文标题**: 10Gb/s Ethernet: switching to a Broadcom SFP+ module

**原文链接**: [https://www.gilesthomas.com/2026/06/10g-ethernet-switching-to-broadcom-sfp-plus](https://www.gilesthomas.com/2026/06/10g-ethernet-switching-to-broadcom-sfp-plus)

生成摘要时出错

---

## 19. OpenAI Losses Increased Nearly 8X in 2025, with Spending Hitting $34B

**原文标题**: OpenAI Losses Increased Nearly 8X in 2025, with Spending Hitting $34B

**原文链接**: [https://www.wheresyoured.at/exclusive-openai-financials/](https://www.wheresyoured.at/exclusive-openai-financials/)

生成摘要时出错

---

## 20. Show HN: High-Res Neural Cellular Automata

**原文标题**: Show HN: High-Res Neural Cellular Automata

**原文链接**: [https://cells2pixels.github.io/](https://cells2pixels.github.io/)

生成摘要时出错

---

## 21. Anthropic employees accuse Trump administration of targeting them

**原文标题**: Anthropic employees accuse Trump administration of targeting them

**原文链接**: [https://www.nytimes.com/2026/06/17/technology/anthropic-trump-administration-fable.html](https://www.nytimes.com/2026/06/17/technology/anthropic-trump-administration-fable.html)

生成摘要时出错

---

## 22. MicroUI – A tiny, portable, immediate-mode UI library written in ANSI C

**原文标题**: MicroUI – A tiny, portable, immediate-mode UI library written in ANSI C

**原文链接**: [https://github.com/rxi/microui](https://github.com/rxi/microui)

生成摘要时出错

---

## 23. Show HN: An 8-bit live gamecast for baseball

**原文标题**: Show HN: An 8-bit live gamecast for baseball

**原文链接**: [https://ribbie.tv/watch](https://ribbie.tv/watch)

生成摘要时出错

---

## 24. Leak Exposes Members of Peter Thiel's Secretive 'Dialog' Society

**原文标题**: Leak Exposes Members of Peter Thiel's Secretive 'Dialog' Society

**原文链接**: [https://www.wired.com/story/leak-exposes-members-of-peter-thiels-secretive-dialog-society/](https://www.wired.com/story/leak-exposes-members-of-peter-thiels-secretive-dialog-society/)

生成摘要时出错

---

## 25. I Fired Google

**原文标题**: I Fired Google

**原文链接**: [https://www.theartofdoingstuff.com/i-fired-google/](https://www.theartofdoingstuff.com/i-fired-google/)

生成摘要时出错

---

## 26. Microsoft turns to AWS as GitHub faces AI capacity crunch

**原文标题**: Microsoft turns to AWS as GitHub faces AI capacity crunch

**原文链接**: [https://runtimewire.com/article/microsoft-github-aws-ai-capacity-crunch](https://runtimewire.com/article/microsoft-github-aws-ai-capacity-crunch)

生成摘要时出错

---

## 27. Show HN: Garden of Flowers – an archive of pictorial typography before ASCII art

**原文标题**: Show HN: Garden of Flowers – an archive of pictorial typography before ASCII art

**原文链接**: [https://garden-of-flowers.heikkilotvonen.com/](https://garden-of-flowers.heikkilotvonen.com/)

生成摘要时出错

---

## 28. Russian artist and Putin critic shot dead in Poland

**原文标题**: Russian artist and Putin critic shot dead in Poland

**原文链接**: [https://www.bbc.com/news/articles/clyrzd5g6k2o](https://www.bbc.com/news/articles/clyrzd5g6k2o)

生成摘要时出错

---

## 29. NLnet announces funding for 67 more open-source projects

**原文标题**: NLnet announces funding for 67 more open-source projects

**原文链接**: [https://nlnet.nl/news/2026/20260616-67-new-projects.html](https://nlnet.nl/news/2026/20260616-67-new-projects.html)

生成摘要时出错

---

## 30. GLM 5.2 Performance Benchmarks

**原文标题**: GLM 5.2 Performance Benchmarks

**原文链接**: [https://artificialanalysis.ai/models/glm-5-2](https://artificialanalysis.ai/models/glm-5-2)

生成摘要时出错

---

## 31. Google Chrome's Next Update Will Mark the End of Popular Ad Blockers

**原文标题**: Google Chrome's Next Update Will Mark the End of Popular Ad Blockers

**原文链接**: [https://tech.slashdot.org/story/26/06/15/205219/google-chromes-next-update-will-mark-the-end-of-popular-ad-blockers](https://tech.slashdot.org/story/26/06/15/205219/google-chromes-next-update-will-mark-the-end-of-popular-ad-blockers)

生成摘要时出错

---

## 32. The UK's Teen Social Media Ban Is Political Theater, Not Child Safety Policy

**原文标题**: The UK's Teen Social Media Ban Is Political Theater, Not Child Safety Policy

**原文链接**: [https://www.techdirt.com/2026/06/16/the-uks-teen-social-media-ban-is-political-theater-not-child-safety-policy/](https://www.techdirt.com/2026/06/16/the-uks-teen-social-media-ban-is-political-theater-not-child-safety-policy/)

生成摘要时出错

---

## 33. How we run Firecracker VMs inside EC2 and start browsers in less than 1s

**原文标题**: How we run Firecracker VMs inside EC2 and start browsers in less than 1s

**原文链接**: [https://browser-use.com/posts/firecracker-browser-infra](https://browser-use.com/posts/firecracker-browser-infra)

生成摘要时出错

---

## 34. Understanding the rationale behind a rule when trying to circumvent it

**原文标题**: Understanding the rationale behind a rule when trying to circumvent it

**原文链接**: [https://devblogs.microsoft.com/oldnewthing/20260611-00/?p=112415](https://devblogs.microsoft.com/oldnewthing/20260611-00/?p=112415)

生成摘要时出错

---

## 35. SubQ 1.1 Small

**原文标题**: SubQ 1.1 Small

**原文链接**: [https://subq.ai/subq-1-1-small-technical-report](https://subq.ai/subq-1-1-small-technical-report)

生成摘要时出错

---

## 36. French physicist and media star loses doctorate after plagiarism investigation

**原文标题**: French physicist and media star loses doctorate after plagiarism investigation

**原文链接**: [https://www.science.org/content/article/french-physicist-and-media-star-loses-doctorate-after-plagiarism-investigation](https://www.science.org/content/article/french-physicist-and-media-star-loses-doctorate-after-plagiarism-investigation)

生成摘要时出错

---

## 37. Amazon Announces Multibillion-Dollar Data Center in Missouri

**原文标题**: Amazon Announces Multibillion-Dollar Data Center in Missouri

**原文链接**: [https://www.narracomm.com/amazon-announces-multibillion-dollar-data-center-in-missouri/](https://www.narracomm.com/amazon-announces-multibillion-dollar-data-center-in-missouri/)

生成摘要时出错

---

## 38. Why thinking out loud with someone beats thinking alone

**原文标题**: Why thinking out loud with someone beats thinking alone

**原文链接**: [https://www.thesignalist.io/s/the-dialogue-dividend/](https://www.thesignalist.io/s/the-dialogue-dividend/)

生成摘要时出错

---

## 39. ICE Appears to Be Buying Immigrants' Tax Identifiers from a Data Broker

**原文标题**: ICE Appears to Be Buying Immigrants' Tax Identifiers from a Data Broker

**原文链接**: [https://www.404media.co/ice-appears-to-be-buying-immigrants-tax-identifiers-from-a-data-broker/](https://www.404media.co/ice-appears-to-be-buying-immigrants-tax-identifiers-from-a-data-broker/)

生成摘要时出错

---

## 40. Never talk to the police

**原文标题**: Never talk to the police

**原文链接**: [https://www.campolalaw.com/why-you-should-never-talk-to-the-po](https://www.campolalaw.com/why-you-should-never-talk-to-the-po)

生成摘要时出错

---

## 41. Launch HN: Adam (YC W25) – Open-Source AI CAD

**原文标题**: Launch HN: Adam (YC W25) – Open-Source AI CAD

**原文链接**: [https://github.com/Adam-CAD/CADAM](https://github.com/Adam-CAD/CADAM)

生成摘要时出错

---

## 42. Making ast.walk 220x Faster

**原文标题**: Making ast.walk 220x Faster

**原文链接**: [https://reflex.dev/blog/why-ast-walk-when-you-can-ast-sprint/](https://reflex.dev/blog/why-ast-walk-when-you-can-ast-sprint/)

生成摘要时出错

---

## 43. Unicorn – The Ultimate CPU Emulator

**原文标题**: Unicorn – The Ultimate CPU Emulator

**原文链接**: [https://www.unicorn-engine.org/](https://www.unicorn-engine.org/)

生成摘要时出错

---

## 44. Fable ban was never about a jailbreak?

**原文标题**: Fable ban was never about a jailbreak?

**原文链接**: [https://techcrunch.com/2026/06/15/the-us-governments-anthropic-models-ban-was-never-about-an-ai-jailbreak/](https://techcrunch.com/2026/06/15/the-us-governments-anthropic-models-ban-was-never-about-an-ai-jailbreak/)

生成摘要时出错

---

## 45. KDE Plasma 6.7 Released

**原文标题**: KDE Plasma 6.7 Released

**原文链接**: [https://kde.org/announcements/plasma/6/6.7.0/](https://kde.org/announcements/plasma/6/6.7.0/)

生成摘要时出错

---

## 46. After AI takes everything

**原文标题**: After AI takes everything

**原文链接**: [https://ursb.me/en/posts/after-ai-takes-everything/](https://ursb.me/en/posts/after-ai-takes-everything/)

生成摘要时出错

---

## 47. Show HN: cuTile Rust: Safe, data-race-free GPU kernels in Rust

**原文标题**: Show HN: cuTile Rust: Safe, data-race-free GPU kernels in Rust

**原文链接**: [https://github.com/nvlabs/cutile-rs](https://github.com/nvlabs/cutile-rs)

生成摘要时出错

---

## 48. Trinket.io shutting down, so we saved it and hosted it a trinket.strivemath.org

**原文标题**: Trinket.io shutting down, so we saved it and hosted it a trinket.strivemath.org

**原文链接**: [https://trinket.strivemath.org/](https://trinket.strivemath.org/)

生成摘要时出错

---

## 49. NetNewsWire Status

**原文标题**: NetNewsWire Status

**原文链接**: [https://inessential.com/2026/06/15/netnewswire-status.html](https://inessential.com/2026/06/15/netnewswire-status.html)

生成摘要时出错

---

## 50. 'Wow, it really worked ': 70s TV show causing worldwide panic today

**原文标题**: 'Wow, it really worked ': 70s TV show causing worldwide panic today

**原文链接**: [https://www.theguardian.com/tv-and-radio/2026/jun/16/alternative-3-mockumentary-missing-scientists-conspiracy-50-years-later](https://www.theguardian.com/tv-and-radio/2026/jun/16/alternative-3-mockumentary-missing-scientists-conspiracy-50-years-later)

生成摘要时出错

---

## 51. Making espresso with ultrasound

**原文标题**: Making espresso with ultrasound

**原文链接**: [https://www.unsw.edu.au/newsroom/news/2026/06/New-way-making-espresso](https://www.unsw.edu.au/newsroom/news/2026/06/New-way-making-espresso)

生成摘要时出错

---

## 52. Why do commercial spaces sit vacant? (2025)

**原文标题**: Why do commercial spaces sit vacant? (2025)

**原文链接**: [https://www.freerange.city/p/why-do-commercial-spaces-sit-vacant](https://www.freerange.city/p/why-do-commercial-spaces-sit-vacant)

生成摘要时出错

---

## 53. DOJ claims xAI's gas turbines are a matter of 'national and energy security'

**原文标题**: DOJ claims xAI's gas turbines are a matter of 'national and energy security'

**原文链接**: [https://techcrunch.com/2026/06/16/doj-claims-xais-unpermitted-gas-turbines-are-a-matter-of-national-economic-and-energy-security/](https://techcrunch.com/2026/06/16/doj-claims-xais-unpermitted-gas-turbines-are-a-matter-of-national-economic-and-energy-security/)

生成摘要时出错

---

## 54. Vance: Iran can have access to $300B reconstruction fund

**原文标题**: Vance: Iran can have access to $300B reconstruction fund

**原文链接**: [https://thehill.com/homenews/administration/5924963-vance-iran-300b-reconstruction-fund/](https://thehill.com/homenews/administration/5924963-vance-iran-300b-reconstruction-fund/)

生成摘要时出错

---

## 55. Show HN: I built 184 free browser tools – PDF, image, dev, AI tasks, no upload

**原文标题**: Show HN: I built 184 free browser tools – PDF, image, dev, AI tasks, no upload

**原文链接**: [https://brevio.pro](https://brevio.pro)

生成摘要时出错

---

## 56. Reviews have become expensive, rewrites have become cheap

**原文标题**: Reviews have become expensive, rewrites have become cheap

**原文链接**: [http://ishmeetbindra.com/posts/reviews-have-become-expensive-rewrites-have-become-cheap/](http://ishmeetbindra.com/posts/reviews-have-become-expensive-rewrites-have-become-cheap/)

生成摘要时出错

---

## 57. San Francisco Weighs PG&E Takeover Amid Soaring Utility Costs

**原文标题**: San Francisco Weighs PG&E Takeover Amid Soaring Utility Costs

**原文链接**: [https://www.kqed.org/news/12081882/san-francisco-has-been-trying-to-leave-pge-for-100-years-will-this-time-be-different](https://www.kqed.org/news/12081882/san-francisco-has-been-trying-to-leave-pge-for-100-years-will-this-time-be-different)

生成摘要时出错

---

## 58. With Wall Street’s help, you’re about to be forced to buy stock in SpaceX

**原文标题**: With Wall Street’s help, you’re about to be forced to buy stock in SpaceX

**原文链接**: [https://paulkrugman.substack.com/p/elon-musk-human-ponzi-scheme](https://paulkrugman.substack.com/p/elon-musk-human-ponzi-scheme)

生成摘要时出错

---

## 59. Peter Thiel's 'Dialog' network was super-secret. A data leak changed that

**原文标题**: Peter Thiel's 'Dialog' network was super-secret. A data leak changed that

**原文链接**: [https://san.com/cc/peter-thiels-dialog-network-was-super-secret-a-data-leak-changed-that/](https://san.com/cc/peter-thiels-dialog-network-was-super-secret-a-data-leak-changed-that/)

生成摘要时出错

---

## 60. SPECS Augmented Reality Glasses

**原文标题**: SPECS Augmented Reality Glasses

**原文链接**: [https://newsroom.snap.com/introducing-specs-augmented-reality-glasses](https://newsroom.snap.com/introducing-specs-augmented-reality-glasses)

生成摘要时出错

---

