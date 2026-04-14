# Hacker News 热门文章摘要 (2026-04-14)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 未来的一切都是谎言，我想：工作

**原文标题**: The future of everything is lies, I guess: Work

**原文链接**: [https://aphyr.com/posts/418-the-future-of-everything-is-lies-i-guess-work](https://aphyr.com/posts/418-the-future-of-everything-is-lies-i-guess-work)

万物皆谎，我猜：工作

题为《万物皆谎，我猜：工作》的文章，批判性地评估了大型语言模型（LLMs）对劳动力的影响，指出当前对LLM的热情是错误的。作者认为，LLMs混乱而模糊的特性，将编程变成了一种“巫术”，开发者需要“提示工程”那些反复无常的“AI精怪”，来生成不可靠且可能有害的代码。这与能保留语义推理的正式编译器形成了鲜明对比。

作者驳斥了“AI员工”的概念，强调LLMs固有的不负责任、倾向于“漫不经心地撒谎”以及可能出现“精神错乱”的问题，并以Claude模型错误管理自动售货机的轶事为例进行说明。

文章借鉴了贝恩布里奇的“自动化悖论”，警告称LLMs将导致各行各业（从软件工程到医学和教育）的普遍去技能化，因为人类将停止运用关键能力。自动化偏见、监控疲劳和“接管风险”进一步使人类与这些系统的互动复杂化，因为当自动化系统失效时，人们将越来越不擅长干预。

作者对一场“劳动力冲击”表达了深切担忧，设想了两种极端情况：要么LLMs无法提供变革性智能，导致经济“勉强度日”；要么它们实现先进能力，取代众多行业（经理、医生、工程师）的劳动力，并导致大规模失业、经济崩溃和社会动荡。

最后，文章指出机器学习（ML）将主要巩固大型科技公司的财富和权力。认为这些历来抵制纳税和工人福利的企业会自愿用巨额AI利润资助全民基本收入（UBI），这种想法被认为是“无可救药的天真”。

---

## 2. 密歇根州“数字时代”法案因隐私顾虑被撤回

**原文标题**: Michigan 'digital age' bills pulled after privacy concerns raised

**原文链接**: [https://www.thecentersquare.com/michigan/article_7ca4e268-4a68-42fb-9042-f9d8604ebd7f.html](https://www.thecentersquare.com/michigan/article_7ca4e268-4a68-42fb-9042-f9d8604ebd7f.html)

密歇根州的两项法案，众议院第4429号法案和参议院第284号法案，被称为“数字年龄保障法案”，本周在倡导团体，主要是密歇根公平选举研究所（MFEI）提出隐私担忧后被撤回。

这些相同且两党支持的法案，旨在作为“儿童安全立法”，原本要求设备制造商和操作系统在激活时“估算”用户年龄，并向应用程序和网站传输持续的“数字年龄信号”。

批评者认为该立法缺乏关键的隐私保护，包括数据使用限制、将数据与其他个人信息结合的限制以及删除要求。MFEI的Patrice Johnson表示，这些法案本将在设备内部创建一个“始终在线的身份层”，但缺乏保障措施。MFEI还强调，这些法案与全国数字童年联盟的示范立法非常相似。

在MFEI向立法者分享其调查结果后，法案共同提案人承认了这些问题。两天之内，众议院和参议院版本都被撤回。提案人众议员Brad Paquette和参议员John Cherry现在正与倡导团体合作，制定潜在的替代立法。倡导团体建议未来的法案应成为全面的“消费者数据隐私框架”的一部分，赋予用户知情权、删除权、选择退出数据销售权以及限制数据使用权。MFEI称赞这一结果是基层对州政策产生影响的一个范例。

---

## 3. 内省扩散语言模型

**原文标题**: Introspective Diffusion Language Models

**原文链接**: [https://introspective-diffusion.github.io/](https://introspective-diffusion.github.io/)

内省扩散语言模型 (I-DLM) 解决了扩散语言模型 (DLM) 和自回归 (AR) 模型之间长期存在的质量差距，并将其归因于现有 DLM 缺乏“内省一致性”。AR 模型本质上会验证它们生成的内容，而 DLM 通常只进行去噪。

I-DLM 引入了内省分步解码 (ISD)，这是一种新颖的方法，允许模型在单个前向传播中同时生成新 token 和验证先前生成的 token。这种方法统一了生成和内省，与 AR 训练相呼应。

I-DLM-8B 的主要成就包括：
*   **质量匹配：** 它是第一个与其同等规模 AR 模型质量相匹配的 DLM，在 15 项基准测试中，它以一半的参数超越了更大的模型，例如 LLaDA-2.1-mini (16B)（例如，在 AIME-24 上高出 26 分）。
*   **吞吐量：** 在高并发下，吞吐量比 LLaDA-2.1-mini 高 2.9-4.1 倍。
*   **无损加速：** 借助门控 LoRA，I-DLM 实现了与基础 AR 模型逐比特相同的输出，从而实现无损加速。
*   **计算效率：** I-DLM 的计算效率大于 1，这意味着它每个 FLOP 产生的有用输出比 AR 更多，使其吞吐量在高并发下能够有效扩展。

I-DLM 方法包括内省一致性训练（转换预训练 AR 模型）、用于高效生成和验证的 ISD、以及 AR 兼容的服务，从而无需自定义后端即可直接集成到 SGLang 等现有 AR 基础设施中。I-DLM 有效克服了困扰先前 DLM 的内省一致性低、计算效率低下和基础设施不匹配等瓶颈。

---

## 4. 可完善的编程语言

**原文标题**: A perfectable programming language

**原文链接**: [https://alok.github.io/lean-pages/perfectable-lean/](https://alok.github.io/lean-pages/perfectable-lean/)

文章推崇Lean为“最好的”编程语言，因为它具有“可完善性”，即它可以在自身内部进行推理和改进，从而形成一个被称为“进步”的“事实和属性的宏伟体系”。

这种可完善性主要源于两个方面。首先，其**语义**建立在依赖类型之上。作者观察到编程语言普遍存在向更强类型化发展的趋势（例如TypeScript、Rust、Python注解），并断言依赖类型代表了将代码属性直接嵌入语言中“最恰当”且最强大的方式。这自然而然地导致了对定理证明基础设施的需求，而Lean恰好拥有这种设施，从而能够对代码行为进行形式化验证，例如验证一个函数总是返回特定值。

其次，Lean提供了“惊人地无缝”的**元编程和自定义语法**，这与其他语言中常常显得笨拙的功能形成了鲜明对比。这使得开发人员能够设计出高度表达性的领域特定语言和可视化符号，例如所展示的井字棋盘字面量，从而促进分层API和灵活的语法解释。

除了这些核心功能之外，作者还强调了**速度**，指出Lean由于能够形式化证明代码等价性，因此具有很高的优化上限，从而可以实现激进的编译器优化。重要的是，Lean被认为是同类语言中唯一一个——它结合了核心编程能力和强大的定理证明器——并且正在积极获得**社区关注度**的语言，这使其有别于Coq、Idris和Agda等不太成功的竞争者。文章最后指出，这篇帖子本身就是用Lean代码编写的。

---

## 5. 欧洲AI：制胜秘籍

**原文标题**: European AI. A playbook to own it

**原文链接**: [https://europe.mistral.ai/](https://europe.mistral.ai/)

Mistral AI发布了一份名为《欧洲人工智能：掌握主动权的行动指南》的报告，文中指出欧洲必须成为一个自力更生的人工智能强国，以克服其与美国和中国之间日益扩大的技术差距。欧洲拥有独特的优势，包括世界一流的学术生态系统、对以人为本技术的坚持，以及一个拥有4.5亿人口的强大单一市场。然而，它面临着市场碎片化、人才流失和投资缺口等挑战，这些风险可能导致经济衰退和战略脆弱性。

Mistral AI首席执行官Arthur Mensch强调，人工智能革命为欧洲提供了引领潮流和定义自身发展道路的机会，从而确保自主权并扩大全球影响力。该行动指南提出了一个以行动、团结和速度为基础的实用框架，聚焦于三大支柱：

1.  **吸引和留住人才：** 措施包括设立“人工智能蓝卡”以实现快速签证，促进更深入的大学与产业合作，建立泛欧洲人工智能创新机构，以及改善人才流动性，以将欧洲定位为全球人工智能人才中心。
2.  **规模化：释放单一市场潜力：** 为应对市场碎片化并解决欧洲在全球风险投资中份额微乎其微（5%）的问题，该行动指南建议精简数字法规，建立欧盟人工智能合规门户，设立企业行为单一登记制度，推出欧盟企业银行通行证，以及为投资基金设立“人工智能欧洲风险投资标签”（AI EuVECA Label）。
3.  **在实体经济中普及欧洲人工智能：** 该文件强调了在实际应用中大规模部署人工智能的必要性，认为广泛采用将推动创新，并为本土人工智能创造一个良性循环的供需关系。

报告的总体信息是，掌控其人工智能和基础设施对欧洲而言并非可选项，而是赢得人工智能竞赛并确保人工智能按照欧洲自身条件为欧洲发展所必不可少的。

---

## 6. 如何让 Firefox 构建速度提升17%

**原文标题**: How to make Firefox builds 17% faster

**原文链接**: [https://blog.farre.se/posts/2026/04/10/caching-webidl-codegen/](https://blog.farre.se/posts/2026/04/10/caching-webidl-codegen/)

This article details how Firefox build times, particularly for "clobber" builds, can be significantly improved by extending `buildcache`'s capabilities to non-compiler steps using its Lua plugin system.

The "WebIDL step" is a Python-based codegen process (`python3 -m mozbuild.action.webidl`) that converts `.webidl` files into C++ binding code. This step is deterministic, produces thousands of files, and runs on every clobber build, making it an ideal candidate for caching. However, traditional compiler caches like `ccache` and `sccache` couldn't cache it as they only wrap compiler invocations.

The solution, introduced in Bug 2027655, involves modifying `dom/bindings/Makefile.in` to conditionally pass `$(CCACHE)` (which becomes `buildcache`) as a command wrapper to the WebIDL `py_action` call. This change is specific to `buildcache` because of its unique Lua plugin system.

A `webidl.lua` wrapper was created, which instructs `buildcache` on how to handle the `mozbuild.action.webidl` command. It identifies the command, its `.webidl` source and Python script inputs, and its generated C++ outputs, allowing `buildcache` to hash these, check the cache, and either replay results or execute the command and store them.

Performance tests show a significant improvement: a warm clobber build (which initially took 5m35s cold) drops to 1m27s with `buildcache` alone, and further to 1m12s with the `webidl.lua` plugin active, saving an additional 15 seconds.

This WebIDL wrapper serves as a proof of concept for leveraging `buildcache`'s Lua plugins to cache any deterministic build step with known inputs and outputs, with plans to extend this approach to other codegen actions in Firefox. Users can enable it by configuring `buildcache` with the `buildcache-wrappers` repository.

---

## 7. An AI Vibe Coding Horror Story

**原文标题**: An AI Vibe Coding Horror Story

**原文链接**: [https://www.tobru.ch/an-ai-vibe-coding-horror-story/](https://www.tobru.ch/an-ai-vibe-coding-horror-story/)

生成摘要时出错

---

## 8. I went to America's worst national parks so you don't have to

**原文标题**: I went to America's worst national parks so you don't have to

**原文链接**: [https://substack.com/home/post/p-193626949](https://substack.com/home/post/p-193626949)

生成摘要时出错

---

## 9. Claude Code Routines

**原文标题**: Claude Code Routines

**原文链接**: [https://code.claude.com/docs/en/routines](https://code.claude.com/docs/en/routines)

生成摘要时出错

---

## 10. Show HN: I built a social media management tool in 3 weeks with Claude and Codex

**原文标题**: Show HN: I built a social media management tool in 3 weeks with Claude and Codex

**原文链接**: [https://github.com/brightbeanxyz/brightbean-studio](https://github.com/brightbeanxyz/brightbean-studio)

生成摘要时出错

---

## 11. AI could be the end of the digital wave, not the next big thing

**原文标题**: AI could be the end of the digital wave, not the next big thing

**原文链接**: [https://thenextwavefutures.wordpress.com/2026/04/07/ai-end-digital-wave-technology-innovation-perez/](https://thenextwavefutures.wordpress.com/2026/04/07/ai-end-digital-wave-technology-innovation-perez/)

生成摘要时出错

---

## 12. Show HN: Ithihāsas – a character explorer for Hindu epics, built in a few hours

**原文标题**: Show HN: Ithihāsas – a character explorer for Hindu epics, built in a few hours

**原文链接**: [https://www.ithihasas.in](https://www.ithihasas.in)

生成摘要时出错

---

## 13. Hacker compromises A16Z-backed phone farm, calling them the 'antichrist'

**原文标题**: Hacker compromises A16Z-backed phone farm, calling them the 'antichrist'

**原文链接**: [https://www.404media.co/hacker-compromises-a16z-backed-phone-farm-tries-to-post-memes-calling-a16z-the-antichrist/](https://www.404media.co/hacker-compromises-a16z-backed-phone-farm-tries-to-post-memes-calling-a16z-the-antichrist/)

生成摘要时出错

---

## 14. Sam Altman's home targeted in second attack

**原文标题**: Sam Altman's home targeted in second attack

**原文链接**: [https://sfstandard.com/2026/04/12/sam-altman-s-home-targeted-second-attack/](https://sfstandard.com/2026/04/12/sam-altman-s-home-targeted-second-attack/)

生成摘要时出错

---

## 15. Google, Microsoft, Meta All Tracking You Even When You Opt Out

**原文标题**: Google, Microsoft, Meta All Tracking You Even When You Opt Out

**原文链接**: [https://www.404media.co/google-microsoft-meta-all-tracking-you-even-when-you-opt-out-according-to-an-independent-audit/](https://www.404media.co/google-microsoft-meta-all-tracking-you-even-when-you-opt-out-according-to-an-independent-audit/)

生成摘要时出错

---

## 16. Tech valuations are back to pre-AI boom levels

**原文标题**: Tech valuations are back to pre-AI boom levels

**原文链接**: [https://www.apollo.com/wealth/the-daily-spark/tech-valuations-back-to-pre-ai-boom-levels](https://www.apollo.com/wealth/the-daily-spark/tech-valuations-back-to-pre-ai-boom-levels)

生成摘要时出错

---

## 17. The secrets of the Shinkansen

**原文标题**: The secrets of the Shinkansen

**原文链接**: [https://www.worksinprogress.news/p/the-secret-behind-japans-railways](https://www.worksinprogress.news/p/the-secret-behind-japans-railways)

Japan's highly successful and profitable railway system, which far outpaces other developed nations, is attributed not to culture, but to effective public policy. The network is comprised of diverse private entities: "legacy private railways" (private since the early 20th century) and the Japan Railways Group (JR), formed from the privatization of nationalized lines in 1988. These companies frequently compete directly.

A defining feature is "railway-led urbanism." Japanese railway companies extend beyond transport, operating as "city-shaping" entities. They own extensive side businesses—including hospitals, housing, retail, entertainment venues, and even baseball teams—along their routes. This allows them to capture the economic value created by their rail infrastructure, which would otherwise be uncaptured spillover benefits. This model fosters a financial synergy between reliable fare revenue and profitable real estate/commercial ventures, while simultaneously attracting residents and customers to their rail corridors.

This unique development is enabled by Japan's liberal land use regulations and private access to city planning powers (like land readjustment), facilitating transit-oriented development. This policy environment permits the creation of both vast low-rise suburbs and hyperdense city centers, where rail's spatial efficiency excels at moving millions. The article concludes that these replicable policies, rather than cultural norms, are the secrets to Japan's outstanding railway system.

---

## 18. For the first time in the U.S., renewables generate more power than natural gas

**原文标题**: For the first time in the U.S., renewables generate more power than natural gas

**原文链接**: [https://e360.yale.edu/digest/us-renewables-natural-gas-coal](https://e360.yale.edu/digest/us-renewables-natural-gas-coal)

生成摘要时出错

---

## 19. Distributed DuckDB Instance

**原文标题**: Distributed DuckDB Instance

**原文链接**: [https://github.com/citguru/openduck](https://github.com/citguru/openduck)

生成摘要时出错

---

## 20. GAIA – Open-source framework for building AI agents that run on local hardware

**原文标题**: GAIA – Open-source framework for building AI agents that run on local hardware

**原文链接**: [https://amd-gaia.ai/docs](https://amd-gaia.ai/docs)

生成摘要时出错

---

## 21. Claude.ai down

**原文标题**: Claude.ai down

**原文链接**: [https://status.claude.com/incidents/6jd2m42f8mld](https://status.claude.com/incidents/6jd2m42f8mld)

生成摘要时出错

---

## 22. They See Your Photos

**原文标题**: They See Your Photos

**原文链接**: [https://theyseeyourphotos.com/](https://theyseeyourphotos.com/)

生成摘要时出错

---

## 23. Missouri town fires half its city council over data center deal

**原文标题**: Missouri town fires half its city council over data center deal

**原文链接**: [https://www.politico.com/news/2026/04/13/missouri-city-council-data-center-00867259](https://www.politico.com/news/2026/04/13/missouri-city-council-data-center-00867259)

生成摘要时出错

---

## 24. Tracking down a 25% Regression on LLVM RISC-V

**原文标题**: Tracking down a 25% Regression on LLVM RISC-V

**原文链接**: [https://blog.kaving.me/blog/tracking-down-a-25-regression-on-llvm-risc-v/](https://blog.kaving.me/blog/tracking-down-a-25-regression-on-llvm-risc-v/)

生成摘要时出错

---

## 25. Tax Wrapped 2025

**原文标题**: Tax Wrapped 2025

**原文链接**: [https://taxwrapped.com](https://taxwrapped.com)

生成摘要时出错

---

## 26. Who's Been Impersonating This ProPublica Reporter?

**原文标题**: Who's Been Impersonating This ProPublica Reporter?

**原文链接**: [https://www.propublica.org/article/impersonating-propublica-reporter](https://www.propublica.org/article/impersonating-propublica-reporter)

生成摘要时出错

---

## 27. New Orleans's Car-Crash Conspiracy

**原文标题**: New Orleans's Car-Crash Conspiracy

**原文链接**: [https://www.newyorker.com/magazine/2026/04/20/the-car-crash-conspiracy](https://www.newyorker.com/magazine/2026/04/20/the-car-crash-conspiracy)

生成摘要时出错

---

## 28. B-trees and database indexes (2024)

**原文标题**: B-trees and database indexes (2024)

**原文链接**: [https://planetscale.com/blog/btrees-and-database-indexes](https://planetscale.com/blog/btrees-and-database-indexes)

生成摘要时出错

---

## 29. The tech jobs bust is real. Don't blame AI (yet)

**原文标题**: The tech jobs bust is real. Don't blame AI (yet)

**原文链接**: [https://economist.com/finance-and-economics/2026/04/13/the-tech-jobs-bust-is-real-dont-blame-ai-yet](https://economist.com/finance-and-economics/2026/04/13/the-tech-jobs-bust-is-real-dont-blame-ai-yet)

生成摘要时出错

---

## 30. The looming college-enrollment death spiral

**原文标题**: The looming college-enrollment death spiral

**原文链接**: [https://www.theatlantic.com/ideas/2026/04/college-enrollment-demographic-cliff/686750/](https://www.theatlantic.com/ideas/2026/04/college-enrollment-demographic-cliff/686750/)

生成摘要时出错

---

## 31. Israeli strike kills infant girl in south Lebanon during father's funeral

**原文标题**: Israeli strike kills infant girl in south Lebanon during father's funeral

**原文链接**: [https://www.reuters.com/world/middle-east/israeli-strike-kills-infant-girl-south-lebanon-during-fathers-funeral-2026-04-12/](https://www.reuters.com/world/middle-east/israeli-strike-kills-infant-girl-south-lebanon-during-fathers-funeral-2026-04-12/)

生成摘要时出错

---

## 32. Hungary's Orban concedes landmark defeat to centre-right opposition

**原文标题**: Hungary's Orban concedes landmark defeat to centre-right opposition

**原文链接**: [https://www.reuters.com/world/europe/hungarians-vote-landmark-election-closely-watched-by-eu-russia-us-2026-04-11/](https://www.reuters.com/world/europe/hungarians-vote-landmark-election-closely-watched-by-eu-russia-us-2026-04-11/)

生成摘要时出错

---

## 33. State of Homelab 2026

**原文标题**: State of Homelab 2026

**原文链接**: [https://mrlokans.work/posts/state-of-homelab-2026/](https://mrlokans.work/posts/state-of-homelab-2026/)

生成摘要时出错

---

## 34. 40% of lost calories globally are from beef, needing 33 cal of feed per 1 cal

**原文标题**: 40% of lost calories globally are from beef, needing 33 cal of feed per 1 cal

**原文链接**: [https://iopscience.iop.org/article/10.1088/2976-601X/ae4f6b](https://iopscience.iop.org/article/10.1088/2976-601X/ae4f6b)

生成摘要时出错

---

## 35. The AI revolution in math has arrived

**原文标题**: The AI revolution in math has arrived

**原文链接**: [https://www.quantamagazine.org/the-ai-revolution-in-math-has-arrived-20260413/](https://www.quantamagazine.org/the-ai-revolution-in-math-has-arrived-20260413/)

生成摘要时出错

---

## 36. Math Is Still Catching Up to the Mysterious Genius of Srinivasa Ramanujan (2024)

**原文标题**: Math Is Still Catching Up to the Mysterious Genius of Srinivasa Ramanujan (2024)

**原文链接**: [https://www.quantamagazine.org/srinivasa-ramanujan-was-a-genius-math-is-still-catching-up-20241021/](https://www.quantamagazine.org/srinivasa-ramanujan-was-a-genius-math-is-still-catching-up-20241021/)

生成摘要时出错

---

## 37. Uncharted island soon to appear on nautical charts

**原文标题**: Uncharted island soon to appear on nautical charts

**原文链接**: [https://www.awi.de/en/about-us/service/press/single-view/unkartierte-insel-demnaechst-auf-seekarten-verzeichnet.html](https://www.awi.de/en/about-us/service/press/single-view/unkartierte-insel-demnaechst-auf-seekarten-verzeichnet.html)

生成摘要时出错

---

## 38. NimConf 2026: Dates Announced, Registrations Open

**原文标题**: NimConf 2026: Dates Announced, Registrations Open

**原文链接**: [https://nim-lang.org/blog/2026/04/07/nimconf-2026.html](https://nim-lang.org/blog/2026/04/07/nimconf-2026.html)

生成摘要时出错

---

## 39. Can Claude Fly a Plane?

**原文标题**: Can Claude Fly a Plane?

**原文链接**: [https://so.long.thanks.fish/can-claude-fly-a-plane/](https://so.long.thanks.fish/can-claude-fly-a-plane/)

生成摘要时出错

---

## 40. OpenSSL 4.0.0

**原文标题**: OpenSSL 4.0.0

**原文链接**: [https://github.com/openssl/openssl/releases/tag/openssl-4.0.0](https://github.com/openssl/openssl/releases/tag/openssl-4.0.0)

生成摘要时出错

---

## 41. Multi-Agentic Software Development Is a Distributed Systems Problem

**原文标题**: Multi-Agentic Software Development Is a Distributed Systems Problem

**原文链接**: [https://kirancodes.me/posts/log-distributed-llms.html](https://kirancodes.me/posts/log-distributed-llms.html)

生成摘要时出错

---

## 42. The rational conclusion of doomerism is violence

**原文标题**: The rational conclusion of doomerism is violence

**原文链接**: [https://www.campbellramble.ai/p/the-rational-conclusion](https://www.campbellramble.ai/p/the-rational-conclusion)

生成摘要时出错

---

## 43. Visualizing CPU Pipelining (2024)

**原文标题**: Visualizing CPU Pipelining (2024)

**原文链接**: [https://timmastny.com/blog/visualizing-cpu-pipelining/](https://timmastny.com/blog/visualizing-cpu-pipelining/)

生成摘要时出错

---

## 44. X Randomly Banning Users for "Inauthentic Behavior"

**原文标题**: X Randomly Banning Users for "Inauthentic Behavior"

**原文链接**: [https://old.reddit.com/r/LinusTechTips/comments/1rsdk7i/anybody_here_talking_about_the_massive/](https://old.reddit.com/r/LinusTechTips/comments/1rsdk7i/anybody_here_talking_about_the_massive/)

生成摘要时出错

---

## 45. N-Day-Bench – Can LLMs find real vulnerabilities in real codebases?

**原文标题**: N-Day-Bench – Can LLMs find real vulnerabilities in real codebases?

**原文链接**: [https://ndaybench.winfunc.com](https://ndaybench.winfunc.com)

生成摘要时出错

---

## 46. MEMS Array Chip Can Project Video the Size of a Grain of Sand

**原文标题**: MEMS Array Chip Can Project Video the Size of a Grain of Sand

**原文链接**: [https://spectrum.ieee.org/mems-photonics](https://spectrum.ieee.org/mems-photonics)

生成摘要时出错

---

## 47. Initial mainline video capture and camera support for Rockchip RK3588

**原文标题**: Initial mainline video capture and camera support for Rockchip RK3588

**原文链接**: [https://www.collabora.com/news-and-blog/news-and-events/mainline-video-capture-and-camera-support-for-rockchip-rk3588.html](https://www.collabora.com/news-and-blog/news-and-events/mainline-video-capture-and-camera-support-for-rockchip-rk3588.html)

生成摘要时出错

---

## 48. Two Months After I Gave an AI $100 and No Instructions

**原文标题**: Two Months After I Gave an AI $100 and No Instructions

**原文链接**: [https://www.sebastian-jais.de/blog/two-months-alma-experiment](https://www.sebastian-jais.de/blog/two-months-alma-experiment)

生成摘要时出错

---

## 49. 5NF and Database Design

**原文标题**: 5NF and Database Design

**原文链接**: [https://kb.databasedesignbook.com/posts/5nf/](https://kb.databasedesignbook.com/posts/5nf/)

生成摘要时出错

---

## 50. Ransomware Is Growing Three Times Faster Than the Spending Meant to Stop It

**原文标题**: Ransomware Is Growing Three Times Faster Than the Spending Meant to Stop It

**原文链接**: [https://ciphercue.com/blog/ransomware-claims-grew-faster-than-security-spend-2025](https://ciphercue.com/blog/ransomware-claims-grew-faster-than-security-spend-2025)

生成摘要时出错

---

## 51. In Denmark, the spread of solar panels has become a divisive issue

**原文标题**: In Denmark, the spread of solar panels has become a divisive issue

**原文链接**: [https://www.theguardian.com/world/2026/mar/20/solar-power-renewable-energy-denmark-backlash-national-elections](https://www.theguardian.com/world/2026/mar/20/solar-power-renewable-energy-denmark-backlash-national-elections)

生成摘要时出错

---

## 52. TanStack Start Now Support React Server Components

**原文标题**: TanStack Start Now Support React Server Components

**原文链接**: [https://tanstack.com/blog/react-server-components](https://tanstack.com/blog/react-server-components)

生成摘要时出错

---

## 53. Haunt, the 70s text adventure game, is now playable on a website

**原文标题**: Haunt, the 70s text adventure game, is now playable on a website

**原文链接**: [https://haunt.madebywindmill.com](https://haunt.madebywindmill.com)

生成摘要时出错

---

## 54. Hungary's Orban, a Beacon to the Right Wing, Concedes Election Defeat

**原文标题**: Hungary's Orban, a Beacon to the Right Wing, Concedes Election Defeat

**原文链接**: [https://www.nytimes.com/2026/04/12/world/europe/hungary-election-orban-magyar.html](https://www.nytimes.com/2026/04/12/world/europe/hungary-election-orban-magyar.html)

生成摘要时出错

---

## 55. Mark Zuckerberg is reportedly building an AI clone to replace him in meetings

**原文标题**: Mark Zuckerberg is reportedly building an AI clone to replace him in meetings

**原文链接**: [https://www.theverge.com/tech/910990/meta-ceo-mark-zuckerberg-ai-clone](https://www.theverge.com/tech/910990/meta-ceo-mark-zuckerberg-ai-clone)

生成摘要时出错

---

## 56. Zig 0.16.0 Release Notes

**原文标题**: Zig 0.16.0 Release Notes

**原文链接**: [https://ziglang.org/download/0.16.0/release-notes.html](https://ziglang.org/download/0.16.0/release-notes.html)

生成摘要时出错

---

## 57. Programming Used to Be Free

**原文标题**: Programming Used to Be Free

**原文链接**: [https://purplesyringa.moe/blog/programming-used-to-be-free/](https://purplesyringa.moe/blog/programming-used-to-be-free/)

生成摘要时出错

---

## 58. Caffeine, cocaine, and painkillers detected in sharks from The Bahamas

**原文标题**: Caffeine, cocaine, and painkillers detected in sharks from The Bahamas

**原文链接**: [https://www.sciencedirect.com/science/article/abs/pii/S0269749126001880](https://www.sciencedirect.com/science/article/abs/pii/S0269749126001880)

生成摘要时出错

---

## 59. The human cost of 10x: How AI is physically breaking senior engineers

**原文标题**: The human cost of 10x: How AI is physically breaking senior engineers

**原文链接**: [https://techtrenches.dev/p/the-human-cost-of-10x-how-ai-is-physically](https://techtrenches.dev/p/the-human-cost-of-10x-how-ai-is-physically)

生成摘要时出错

---

## 60. Hungary's Viktor Orbán Concedes Defeat in Election

**原文标题**: Hungary's Viktor Orbán Concedes Defeat in Election

**原文链接**: [https://www.wsj.com/world/europe/hungary-election-results-orban-b2dbd42a](https://www.wsj.com/world/europe/hungary-election-results-orban-b2dbd42a)

生成摘要时出错

---

## 61. Let's Talk Space Toilets

**原文标题**: Let's Talk Space Toilets

**原文链接**: [https://mceglowski.substack.com/p/lets-talk-space-toilets](https://mceglowski.substack.com/p/lets-talk-space-toilets)

生成摘要时出错

---

## 62. California ghost-gun bill wants 3D printers to play cop, EFF says

**原文标题**: California ghost-gun bill wants 3D printers to play cop, EFF says

**原文链接**: [https://www.theregister.com/2026/04/14/eff_california_3dprinted_firearms/](https://www.theregister.com/2026/04/14/eff_california_3dprinted_firearms/)

生成摘要时出错

---

## 63. Show HN: LangAlpha – what if Claude Code was built for Wall Street?

**原文标题**: Show HN: LangAlpha – what if Claude Code was built for Wall Street?

**原文链接**: [https://github.com/ginlix-ai/langalpha](https://github.com/ginlix-ai/langalpha)

生成摘要时出错

---

## 64. Roblox devs now need a subscription to share their games freely

**原文标题**: Roblox devs now need a subscription to share their games freely

**原文链接**: [https://devforum.roblox.com/t/new-publishing-requirements-evaluation-process-for-games/4573166](https://devforum.roblox.com/t/new-publishing-requirements-evaluation-process-for-games/4573166)

生成摘要时出错

---

## 65. Tom7: No one can force me to have a secure website [video]

**原文标题**: Tom7: No one can force me to have a secure website [video]

**原文链接**: [https://www.youtube.com/watch?v=M1si1y5lvkk](https://www.youtube.com/watch?v=M1si1y5lvkk)

生成摘要时出错

---

## 66. MOS tech 6502 8-bit microprocessor in pure SQL powered by Postgres

**原文标题**: MOS tech 6502 8-bit microprocessor in pure SQL powered by Postgres

**原文链接**: [https://github.com/lasect/pg_6502](https://github.com/lasect/pg_6502)

生成摘要时出错

---

## 67. Just Enough Chimera Linux

**原文标题**: Just Enough Chimera Linux

**原文链接**: [https://www.dwarmstrong.org/chimera-install-zfs/](https://www.dwarmstrong.org/chimera-install-zfs/)

生成摘要时出错

---

## 68. The exponential curve behind open source backlogs

**原文标题**: The exponential curve behind open source backlogs

**原文链接**: [https://armanckeser.com/writing/jellyfin-flow](https://armanckeser.com/writing/jellyfin-flow)

生成摘要时出错

---

## 69. Ascending into the Realm of Japanese Charts

**原文标题**: Ascending into the Realm of Japanese Charts

**原文链接**: [https://www.chartography.net/p/ascending-into-the-realm-of-japanese](https://www.chartography.net/p/ascending-into-the-realm-of-japanese)

生成摘要时出错

---

## 70. The AI Layoff Trap

**原文标题**: The AI Layoff Trap

**原文链接**: [https://arxiv.org/abs/2603.20617](https://arxiv.org/abs/2603.20617)

生成摘要时出错

---

## 71. The Fediverse deserves a dumb graphical client

**原文标题**: The Fediverse deserves a dumb graphical client

**原文链接**: [https://adele.pages.casa/md/blog/the-fediverse-deserves-a-dumb-graphical-client.md](https://adele.pages.casa/md/blog/the-fediverse-deserves-a-dumb-graphical-client.md)

生成摘要时出错

---

## 72. Schools Never Taught Critical Thinking: AI Exposed the Lie

**原文标题**: Schools Never Taught Critical Thinking: AI Exposed the Lie

**原文链接**: [https://smarterarticles.co.uk/ai-exposed-the-lie-schools-never-taught-critical-thinking](https://smarterarticles.co.uk/ai-exposed-the-lie-schools-never-taught-critical-thinking)

生成摘要时出错

---

## 73. Austerity Creates Fascism

**原文标题**: Austerity Creates Fascism

**原文链接**: [https://pluralistic.net/2026/04/12/always-great/](https://pluralistic.net/2026/04/12/always-great/)

生成摘要时出错

---

## 74. AI will never be ethical or safe

**原文标题**: AI will never be ethical or safe

**原文链接**: [https://meiert.com/blog/ai-ethics-and-safety/](https://meiert.com/blog/ai-ethics-and-safety/)

生成摘要时出错

---

## 75. Evaluation of Claude Mythos Preview's cyber capabilities

**原文标题**: Evaluation of Claude Mythos Preview's cyber capabilities

**原文链接**: [https://www.aisi.gov.uk/blog/our-evaluation-of-claude-mythos-previews-cyber-capabilities](https://www.aisi.gov.uk/blog/our-evaluation-of-claude-mythos-previews-cyber-capabilities)

生成摘要时出错

---

## 76. Show HN: Kontext CLI – Credential broker for AI coding agents in Go

**原文标题**: Show HN: Kontext CLI – Credential broker for AI coding agents in Go

**原文链接**: [https://github.com/kontext-dev/kontext-cli](https://github.com/kontext-dev/kontext-cli)

生成摘要时出错

---

## 77. The Case Against Gameplay Loops (2024)

**原文标题**: The Case Against Gameplay Loops (2024)

**原文链接**: [https://blog.joeyschutz.com/the-case-against-gameplay-loops/](https://blog.joeyschutz.com/the-case-against-gameplay-loops/)

生成摘要时出错

---

## 78. Claude Code may be burning your limits with invisible tokens

**原文标题**: Claude Code may be burning your limits with invisible tokens

**原文链接**: [https://efficienist.com/claude-code-may-be-burning-your-limits-with-invisible-tokens-you-cant-see-or-audit/](https://efficienist.com/claude-code-may-be-burning-your-limits-with-invisible-tokens-you-cant-see-or-audit/)

生成摘要时出错

---

## 79. Computer science enrollment data suddenly shows a big drop

**原文标题**: Computer science enrollment data suddenly shows a big drop

**原文链接**: [https://www.washingtonpost.com/technology/2026/04/13/computer-science-major-ai/](https://www.washingtonpost.com/technology/2026/04/13/computer-science-major-ai/)

生成摘要时出错

---

## 80. NYC to open municipal grocery store in 2027

**原文标题**: NYC to open municipal grocery store in 2027

**原文链接**: [https://www.grocerydive.com/news/new-york-city-owned-grocery-store-manhattan-mamdani/817381/](https://www.grocerydive.com/news/new-york-city-owned-grocery-store-manhattan-mamdani/817381/)

生成摘要时出错

---

## 81. Why it’s impossible to measure England’s coastline

**原文标题**: Why it’s impossible to measure England’s coastline

**原文链接**: [https://www.bbc.com/travel/article/20260410-why-its-impossible-to-measure-englands-coastline](https://www.bbc.com/travel/article/20260410-why-its-impossible-to-measure-englands-coastline)

生成摘要时出错

---

## 82. Turn your best AI prompts into one-click tools in Chrome

**原文标题**: Turn your best AI prompts into one-click tools in Chrome

**原文链接**: [https://blog.google/products-and-platforms/products/chrome/skills-in-chrome/](https://blog.google/products-and-platforms/products/chrome/skills-in-chrome/)

生成摘要时出错

---

## 83. CIA reportedly used Pegasus software during rescue of airman in Iran

**原文标题**: CIA reportedly used Pegasus software during rescue of airman in Iran

**原文链接**: [https://www.timesofisrael.com/cia-reportedly-used-pegasus-software-for-deception-op-during-rescue-of-airman-in-iran/](https://www.timesofisrael.com/cia-reportedly-used-pegasus-software-for-deception-op-during-rescue-of-airman-in-iran/)

生成摘要时出错

---

## 84. Basics of Radar Technology

**原文标题**: Basics of Radar Technology

**原文链接**: [https://www.radartutorial.eu/index.en.html](https://www.radartutorial.eu/index.en.html)

生成摘要时出错

---

## 85. 90% of CEOs Say AI Changed Nothing. The Other 10% Have a PR Team

**原文标题**: 90% of CEOs Say AI Changed Nothing. The Other 10% Have a PR Team

**原文链接**: [https://businessasusual.io/p/ninety-percent-of-ceos-say-ai-changed](https://businessasusual.io/p/ninety-percent-of-ceos-say-ai-changed)

生成摘要时出错

---

## 86. Point Cloud Allemansrätten

**原文标题**: Point Cloud Allemansrätten

**原文链接**: [https://digitalflapjack.com/weeknotes/point-cloud-allemansr%C3%A4tten/](https://digitalflapjack.com/weeknotes/point-cloud-allemansr%C3%A4tten/)

生成摘要时出错

---

## 87. Modifying FileZilla to Workaround Bambu 3D Printer's FTP Issue

**原文标题**: Modifying FileZilla to Workaround Bambu 3D Printer's FTP Issue

**原文链接**: [https://lantian.pub/en/article/modify-computer/modify-filezilla-workaround-bambu-3d-printer-ftp-issue.lantian/](https://lantian.pub/en/article/modify-computer/modify-filezilla-workaround-bambu-3d-printer-ftp-issue.lantian/)

生成摘要时出错

---

## 88. Show HN: Kelet – Root Cause Analysis agent for your LLM apps

**原文标题**: Show HN: Kelet – Root Cause Analysis agent for your LLM apps

**原文链接**: [https://kelet.ai/](https://kelet.ai/)

生成摘要时出错

---

## 89. Kindle users in uproar over update rendering oldest devices virtually unusable

**原文标题**: Kindle users in uproar over update rendering oldest devices virtually unusable

**原文链接**: [https://nypost.com/2026/04/09/tech/kindle-to-cease-support-for-old-devices-causing-user-uproar/](https://nypost.com/2026/04/09/tech/kindle-to-cease-support-for-old-devices-causing-user-uproar/)

生成摘要时出错

---

