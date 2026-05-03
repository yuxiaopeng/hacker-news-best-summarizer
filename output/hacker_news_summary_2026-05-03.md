# Hacker News 热门文章摘要 (2026-05-03)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. VS Code 无论是否使用，都会在提交中插入 'Co-Authored-by Copilot'

**原文标题**: VS Code inserting 'Co-Authored-by Copilot' into commits regardless of usage

**原文链接**: [https://github.com/microsoft/vscode/pull/310226](https://github.com/microsoft/vscode/pull/310226)

一个于2026年4月16日合并到VS Code的Git扩展中的拉取请求（PR），将`git.addAICoAuthor`设置的默认值从“off”更改为“all”。这一修改自动启用了AI合著署名，导致“Co-Authored-by: Copilot <copilot@github.com>”默认被插入到Git提交信息中。

这一改变在用户中引发了广泛的愤怒，他们报告称，即使在未曾使用Copilot或明确禁用了AI功能的情况下，合著标签也出现在了他们的提交中。用户谴责此举“不可接受”、“荒谬”、“蓄意破坏”、“疯狂”，甚至近乎“欺诈”，并猜测这是企图人为夸大Copilot使用量指标。许多人威胁要改用其他IDE。该问题还在Hacker News上获得了广泛关注。

2026年5月2日，参与合并原始PR的微软贡献者dmitrivMS为此“退步”表示歉意。他承认，当AI功能被禁用时，该功能不应被启用，也不应将非AI所做的更改归因于AI。他承诺将在1.119版本中修复此问题，并创建了一个后续PR（#313931）。紧随此次道歉之后，微软以存在垃圾信息为由锁定了该对话。

---

## 2. 为什么黑色风扇版本发布要这么久？

**原文标题**: Why does it take so long to release black fan versions?

**原文链接**: [https://www.noctua.at/en/expertise/blog/how-can-it-take-so-long-to-release-black-fan-versions](https://www.noctua.at/en/expertise/blog/how-can-it-take-so-long-to-release-black-fan-versions)

猫头鹰（Noctua）的文章解释说，推出黑色版风扇需要很长时间，因为这涉及复杂的广泛研发和质量控制过程，远不止是简单的颜色改变。

核心原因是风扇的颜色，特别是所使用的颜料，会对其材料特性和制造工艺产生重大影响。即使是微小的变化也会影响扇叶和框架的刚度、强度和重量，从而改变其空气动力学性能，并可能引入不必要的噪音或振动。

猫头鹰必须一丝不苟地测试每一个组件。这包括：
1.  **材料和颜料研究：** 寻找合适的黑色颜料，且这些颜料不能损害塑料的机械性能。
2.  **注塑成型调整：** 不同的塑料和颜料需要对注塑成型过程（温度、压力、循环时间）进行精确调整，以确保质量一致性并防止翘曲或薄弱点。
3.  **空气动力学性能测试：** 每个原型都必须在他们的消音室中进行严格测试，以确保其符合原始风扇严格的噪音和气流标准。
4.  **长期耐久性测试：** 风扇会进行加速老化测试，以保证黑色版本保持相同的寿命和可靠性。

此外，生产新版本需要为每个组件创建新的注塑模具，这既昂贵又耗时。文章强调，猫头鹰将性能、声学和寿命置于一切之上，这使得他们不愿仓促推出产品，如果这会损害他们既定的质量标准。正是这种对每一个黑色变体进行的彻底验证过程，导致它们可能需要数年才能上市。

---

## 3. Ti-84 进化版

**原文标题**: Ti-84 Evo

**原文链接**: [https://education.ti.com/en/products/calculators/graphing-calculators/ti-84-evo](https://education.ti.com/en/products/calculators/graphing-calculators/ti-84-evo)

TI-84 Evo 是一款全新进化的图形计算器，旨在让所有功能表现更出色。该发布强调了其显著改进，并邀请用户探索其新功能。

---

## 4. 达维二维

**原文标题**: Dav2d

**原文链接**: [https://code.videolan.org/videolan/dav2d](https://code.videolan.org/videolan/dav2d)

此加载界面是一个机器人验证挑战，由网站管理员使用“Anubis”激活以保护服务器。Anubis旨在阻止人工智能公司进行大规模抓取，这可能导致网站崩溃并扰乱合法用户的访问。

Anubis是一种临时的折衷方案，采用类似于Hashcash的工作量证明（PoW）机制。该系统对单个用户造成的计算负担可忽略不计，但显著增加了大规模爬虫的累计成本，使大规模抓取在经济上变得不可行。

长期目标是超越工作量证明（PoW）挑战，通过开发先进的指纹识别和无头浏览器检测技术（例如，通过字体渲染）来识别机器人，同时不给合法用户带来不便。

至关重要的是，Anubis要求使用现代JavaScript功能。用户必须为此域名启用JavaScript并禁用JShelter等干扰性插件才能通过验证。采取这项措施被认为是必要的，因为人工智能公司已经改变了网络托管的“社会契约”。目前正在开发不需要JavaScript的解决方案。

---

## 5. 网络骇客 5.0.0

**原文标题**: NetHack 5.0.0

**原文链接**: [https://nethack.org/v500/release.html](https://nethack.org/v500/release.html)

NetHack 5.0.0于2026年5月2日发布，是这款经典地下城探索游戏的增强版本。作为一个.0版本，其中可能存在一些错误，开发团队欢迎用户提供反馈和bug报告。

此版本引入了重大的架构改进：源代码现在符合C99标准，并且移除了交叉编译的障碍，使得在各种平台上构建变得更加容易。以前基于“yacc和lex”的关卡和地下城编译器，以及任务文本处理，已被在游戏过程中加载的Lua文本替代方案取代。

此版本包含超过3100项修复和更改，详细记录在`doc/fixes5-0-0.txt`文件中。对玩家而言一个重要的注意事项是：**现有的存档文件和骨骸文件与NetHack 5.0.0不兼容。** 用户可以使用提供的SHA256校验和验证下载的二进制文件，并利用`nethack --showpaths`命令确认文件位置。开发团队鼓励用户通过其问题报告表提交bug，并请用户首先查阅“已知bug”列表。

---

## 6. 请勿追踪

**原文标题**: Do_not_track

**原文链接**: [https://donottrack.sh/](https://donottrack.sh/)

文章指出一个显著问题：众多 CLI 工具、SDK 和框架默认收集遥测数据，每个都需通过不同且通常是独有的方法来选择退出（例如 `DOTNET_CLI_TELEMETRY_OPTOUT=1`、`SAM_CLI_TELEMETRY=0`）。这种缺乏标准化的做法对于希望禁用数据收集的用户来说既不方便又令人沮丧。

为了解决这个问题，该提议建议引入一个单一的通用环境变量：`DO_NOT_TRACK=1`。这个变量将明确表达用户希望选择退出所有形式的数据收集，包括广告跟踪、使用情况报告（无论是否匿名）、遥测、崩溃报告以及发送给软件创建者或第三方的任何非必要网络请求。目标是确保软件在本地运行，而无需不必要的数据传输。

用户可以通过在其 shell 配置文件（例如 `~/.bashrc` 或 `~/.zshrc`）中添加 `export DO_NOT_TRACK=1` 来实现这一点；对于 Fish shell，使用 `set -x DO_NOT_TRACK 1`；对于 PowerShell，使用 `$env:DO_NOT_TRACK = "1"`；对于 Windows CMD，使用 `setx DO_NOT_TRACK 1`。

强烈建议软件作者尊重此变量：如果 `DO_NOT_TRACK` 被设置为 `1`，他们应该禁用所有跟踪，同时仍保留现有的选择退出机制。文章还鼓励作者考虑将遥测功能默认设置为选择加入（opt-in），而非默认选择退出（opt-out），参照像 `NO_COLOR` 这样用于禁用颜色输出的标准化工作。

---

## 7. Ladybird 本月 – 2026年4月

**原文标题**: This Month in Ladybird – April 2026

**原文链接**: [https://ladybird.org/newsletter/2026-04-30/](https://ladybird.org/newsletter/2026-04-30/)

Ladybird 在 2026 年 4 月发布了更新，汇集了 35 位贡献者的 333 个 PR，在性能、功能和架构方面带来了显著进步。新增赞助包括人权基金会提供的 50,000 美元。

核心面向用户的功能现在包括一个内置 PDF 查看器（由 pdf.js 提供支持）以及一个功能丰富、支持历史记录的地址栏自动补全功能。全新的 GTK4/libadwaita Linux 前端已发布，同时还推出了功能全面的书签管理功能，包括专用用户界面、导入/导出和拖放功能。完整的 Cache 和 CacheStorage API 也已实现。

性能方面有了显著提升：HTML 解析现在支持增量和推测性解析，从而更有效地预加载资源。JavaScript 引擎得益于离线程字节码编译、更快的 JS-to-JS 调用、O(1) 寄存器分配器、缓存的 `for-in` 迭代（提升了 Speedometer 分数）以及零拷贝字符串优化等诸多改进。渲染现在支持在单独线程上进行每个 Navigable（iframe）的栅格化，并改进了使用 `dmabuf` 的 Linux GPU 绘制。网络的 `getaddrinfo` 已实现异步化，并且响应数据排空也得到了优化。

CSS 新增了 `image-set()`、`position-anchor`、增强的颜色插值，并更好地处理演示提示和 RTL 列表标记。在样式失效方面的大量工作显著减少了复杂页面上的重新计算。该项目还采用了 `mimalloc` 作为主要分配器，从而改善了 JS 基准测试性能，并强制构建使用 Rust。

这些改变使得在 Reddit（图片画廊、无限滚动）和 YouTube 上的性能显著提升，同时还修复了许多其他网站的问题。Ladybird 的 Web 平台测试分数增加了超过 63,000 个子测试，其中包括新集成的 test262 JavaScript 一致性测试套件达到了 97.8% 的通过率。

---

## 8. Mercedes-Benz commits to bringing back physical buttons

**原文标题**: Mercedes-Benz commits to bringing back physical buttons

**原文链接**: [https://www.drive.com.au/news/mercedes-benz-commits-to-bringing-back-phycial-buttons/](https://www.drive.com.au/news/mercedes-benz-commits-to-bringing-back-phycial-buttons/)

生成摘要时出错

---

## 9. Ask.com has closed

**原文标题**: Ask.com has closed

**原文链接**: [https://www.ask.com/](https://www.ask.com/)

生成摘要时出错

---

## 10. Six years perfecting maps on watchOS

**原文标题**: Six years perfecting maps on watchOS

**原文链接**: [https://www.david-smith.org/blog/2026/04/29/maps-on-watchos/](https://www.david-smith.org/blog/2026/04/29/maps-on-watchos/)

生成摘要时出错

---

## 11. A couple million lines of Haskell: Production engineering at Mercury

**原文标题**: A couple million lines of Haskell: Production engineering at Mercury

**原文链接**: [https://blog.haskell.org/a-couple-million-lines-of-haskell/](https://blog.haskell.org/a-couple-million-lines-of-haskell/)

Ian Duncan discusses how Mercury, a fast-growing fintech company serving over 300,000 businesses with a $248 billion transaction volume, successfully runs a 2-million-line Haskell codebase, largely maintained by engineers new to the language. He argues that Haskell's value in production comes from its ability to enforce operational rigor and encode institutional knowledge, rather than just its elegance or theoretical purity.

Mercury's reliability philosophy emphasizes "adaptive capacity": a system's ability to absorb variation, degrade gracefully, and be understandable. This is vital in a company with high engineering turnover. The type system functions as an "operational aid," preserving critical knowledge by encoding it directly into interfaces, making it more reliable than mutable documentation.

Key principles include:
1.  **Purity as a Boundary:** Haskell's strength isn't inherent purity but its ability to enforce purity at interfaces. Dangerous or mutable operations are acceptable if strictly contained and narrowly exposed through types, preventing misuse.
2.  **Make the Right Thing Easy:** Haskell allows encoding operational "incantations" (e.g., transactional event publishing) into types. This makes the correct procedure the *only* available path, preventing errors that stem from forgotten tribal knowledge and ensuring consistent, safe operations as teams evolve.

The compiler, in this context, becomes a superior custodian of operational lore, enforcing design choices that ensure system stability and adaptability at scale.

---

## 12. Kimi K2.6 just beat Claude, GPT-5.5, and Gemini in a coding challenge

**原文标题**: Kimi K2.6 just beat Claude, GPT-5.5, and Gemini in a coding challenge

**原文链接**: [https://thinkpol.ca/2026/04/30/an-open-weights-chinese-model-just-beat-claude-gpt-5-5-and-gemini-in-a-programming-challenge/](https://thinkpol.ca/2026/04/30/an-open-weights-chinese-model-just-beat-claude-gpt-5-5-and-gemini-in-a-programming-challenge/)

生成摘要时出错

---

## 13. AI Self-preferencing in Algorithmic Hiring: Empirical Evidence and Insights

**原文标题**: AI Self-preferencing in Algorithmic Hiring: Empirical Evidence and Insights

**原文链接**: [https://arxiv.org/abs/2509.00462](https://arxiv.org/abs/2509.00462)

生成摘要时出错

---

## 14. California to begin ticketing driverless cars that violate traffic laws

**原文标题**: California to begin ticketing driverless cars that violate traffic laws

**原文链接**: [https://www.bbc.com/news/articles/clypjx3rg2go](https://www.bbc.com/news/articles/clypjx3rg2go)

生成摘要时出错

---

## 15. Neanderthals ran 'fat factories' 125k years ago (2025)

**原文标题**: Neanderthals ran 'fat factories' 125k years ago (2025)

**原文链接**: [https://www.universiteitleiden.nl/en/news/2025/07/neanderthals-ran-fat-factories-125000-years-ago](https://www.universiteitleiden.nl/en/news/2025/07/neanderthals-ran-fat-factories-125000-years-ago)

生成摘要时出错

---

## 16. How fast is a macOS VM, and how small could it be?

**原文标题**: How fast is a macOS VM, and how small could it be?

**原文链接**: [https://eclecticlight.co/2026/05/02/how-fast-is-a-macos-vm-and-how-small-could-it-be/](https://eclecticlight.co/2026/05/02/how-fast-is-a-macos-vm-and-how-small-could-it-be/)

生成摘要时出错

---

## 17. Tesla owner won $10k in court for Tesla's FSD lies. Tesla is still fighting him

**原文标题**: Tesla owner won $10k in court for Tesla's FSD lies. Tesla is still fighting him

**原文链接**: [https://electrek.co/2026/05/02/this-tesla-owner-won-10k-in-court-for-teslas-fsd-lies-tesla-is-still-fighting-him/](https://electrek.co/2026/05/02/this-tesla-owner-won-10k-in-court-for-teslas-fsd-lies-tesla-is-still-fighting-him/)

生成摘要时出错

---

## 18. America's Expanding Domestic Surveillance

**原文标题**: America's Expanding Domestic Surveillance

**原文链接**: [https://www.wsj.com/articles/americas-expanding-domestic-surveillance-08b73187](https://www.wsj.com/articles/americas-expanding-domestic-surveillance-08b73187)

生成摘要时出错

---

## 19. Russia Poisons Wikipedia

**原文标题**: Russia Poisons Wikipedia

**原文链接**: [https://www.bettedangerous.com/p/russia-poisons-wikipedia](https://www.bettedangerous.com/p/russia-poisons-wikipedia)

生成摘要时出错

---

## 20. Specsmaxxing – On overcoming AI psychosis, and why I write specs in YAML

**原文标题**: Specsmaxxing – On overcoming AI psychosis, and why I write specs in YAML

**原文链接**: [https://acai.sh/blog/specsmaxxing](https://acai.sh/blog/specsmaxxing)

生成摘要时出错

---

## 21. Roblox shares plummet 18% as child safety measures weigh on bookings

**原文标题**: Roblox shares plummet 18% as child safety measures weigh on bookings

**原文链接**: [https://www.cnbc.com/2026/05/01/roblox-rblx-stock-child-safety-earnings.html](https://www.cnbc.com/2026/05/01/roblox-rblx-stock-child-safety-earnings.html)

生成摘要时出错

---

## 22. Credit cards are vulnerable to brute force kind attacks

**原文标题**: Credit cards are vulnerable to brute force kind attacks

**原文链接**: [https://metin.nextc.org/posts/Credit_Cards_Are_Vulnerable_To_Brute_Force_Kind_Attacks.html](https://metin.nextc.org/posts/Credit_Cards_Are_Vulnerable_To_Brute_Force_Kind_Attacks.html)

生成摘要时出错

---

## 23. Job Postings for Software Engineers Are Rapidly Rising

**原文标题**: Job Postings for Software Engineers Are Rapidly Rising

**原文链接**: [https://www.citadelsecurities.com/news-and-insights/2026-global-intelligence-crisis/](https://www.citadelsecurities.com/news-and-insights/2026-global-intelligence-crisis/)

生成摘要时出错

---

## 24. Maryland to ban A.I.-driven price increases in grocery stores

**原文标题**: Maryland to ban A.I.-driven price increases in grocery stores

**原文链接**: [https://www.nytimes.com/2026/05/01/business/surveillance-pricing-groceries-maryland.html](https://www.nytimes.com/2026/05/01/business/surveillance-pricing-groceries-maryland.html)

生成摘要时出错

---

## 25. Open Design: Use Your Coding Agent as a Design Engine

**原文标题**: Open Design: Use Your Coding Agent as a Design Engine

**原文链接**: [https://github.com/nexu-io/open-design](https://github.com/nexu-io/open-design)

生成摘要时出错

---

## 26. Why are there both TMP and TEMP environment variables? (2015)

**原文标题**: Why are there both TMP and TEMP environment variables? (2015)

**原文链接**: [https://devblogs.microsoft.com/oldnewthing/20150417-00/?p=44213](https://devblogs.microsoft.com/oldnewthing/20150417-00/?p=44213)

生成摘要时出错

---

## 27. Utah to hold websites liable for users who mask their location with VPNs

**原文标题**: Utah to hold websites liable for users who mask their location with VPNs

**原文链接**: [https://www.tomshardware.com/software/vpn/utah-becomes-first-us-state-to-target-vpn-use-with-age-verification-law](https://www.tomshardware.com/software/vpn/utah-becomes-first-us-state-to-target-vpn-use-with-age-verification-law)

生成摘要时出错

---

## 28. Lib0xc: A set of C standard library-adjacent APIs for safer systems programming

**原文标题**: Lib0xc: A set of C standard library-adjacent APIs for safer systems programming

**原文链接**: [https://github.com/microsoft/lib0xc](https://github.com/microsoft/lib0xc)

生成摘要时出错

---

## 29. For thirty years I programmed with Phish on, every day

**原文标题**: For thirty years I programmed with Phish on, every day

**原文链接**: [https://christophermeiklejohn.com/ai/personal/phish/flow/agents/2026/05/03/rift.html](https://christophermeiklejohn.com/ai/personal/phish/flow/agents/2026/05/03/rift.html)

生成摘要时出错

---

## 30. Open source does not imply open community

**原文标题**: Open source does not imply open community

**原文链接**: [https://blog.feld.me/posts/2026/04/open-source-does-not-imply-open-community/](https://blog.feld.me/posts/2026/04/open-source-does-not-imply-open-community/)

生成摘要时出错

---

## 31. A network smuggling Starlink tech into Iran to beat internet blackout

**原文标题**: A network smuggling Starlink tech into Iran to beat internet blackout

**原文链接**: [https://www.bbc.com/news/articles/cvgzk91leweo](https://www.bbc.com/news/articles/cvgzk91leweo)

生成摘要时出错

---

## 32. The agent harness belongs outside the sandbox

**原文标题**: The agent harness belongs outside the sandbox

**原文链接**: [https://www.mendral.com/blog/agent-harness-belongs-outside-sandbox](https://www.mendral.com/blog/agent-harness-belongs-outside-sandbox)

生成摘要时出错

---

## 33. Windows quality update: Progress we've made since March

**原文标题**: Windows quality update: Progress we've made since March

**原文链接**: [https://blogs.windows.com/windows-insider/2026/05/01/windows-quality-update-progress-weve-made-since-march/](https://blogs.windows.com/windows-insider/2026/05/01/windows-quality-update-progress-weve-made-since-march/)

生成摘要时出错

---

## 34. Show HN: State of the Art of Coding Models, According to Hacker News Commenters

**原文标题**: Show HN: State of the Art of Coding Models, According to Hacker News Commenters

**原文链接**: [https://hnup.date/hn-sota](https://hnup.date/hn-sota)

生成摘要时出错

---

## 35. Show HN: Apple's SHARP running in the browser via ONNX runtime web

**原文标题**: Show HN: Apple's SHARP running in the browser via ONNX runtime web

**原文链接**: [https://github.com/bring-shrubbery/ml-sharp-web](https://github.com/bring-shrubbery/ml-sharp-web)

生成摘要时出错

---

## 36. Uber wants to turn its drivers into a sensor grid for self-driving companies

**原文标题**: Uber wants to turn its drivers into a sensor grid for self-driving companies

**原文链接**: [https://techcrunch.com/2026/05/01/uber-wants-to-turn-its-millions-of-drivers-into-a-sensor-grid-for-self-driving-companies/](https://techcrunch.com/2026/05/01/uber-wants-to-turn-its-millions-of-drivers-into-a-sensor-grid-for-self-driving-companies/)

生成摘要时出错

---

## 37. A report on burnout in open source software communities (2025) [pdf]

**原文标题**: A report on burnout in open source software communities (2025) [pdf]

**原文链接**: [https://mirandaheath.website/static/oss_burnout_report_mh_25.pdf](https://mirandaheath.website/static/oss_burnout_report_mh_25.pdf)

生成摘要时出错

---

## 38. Clojurists Together – Q2 2026 Open Source Funding Announcement

**原文标题**: Clojurists Together – Q2 2026 Open Source Funding Announcement

**原文链接**: [https://www.clojuriststogether.org/news/q2-2026-funding-announcement/](https://www.clojuriststogether.org/news/q2-2026-funding-announcement/)

生成摘要时出错

---

## 39. Good developers learn to program. Most courses teach a language

**原文标题**: Good developers learn to program. Most courses teach a language

**原文链接**: [https://evilgeniuslabs.ca/blog/good-developers-learn-to-program-not-a-language](https://evilgeniuslabs.ca/blog/good-developers-learn-to-program-not-a-language)

生成摘要时出错

---

## 40. Ubuntu servers taken offline by "sustained, cross-border attack"

**原文标题**: Ubuntu servers taken offline by "sustained, cross-border attack"

**原文链接**: [https://arstechnica.com/security/2026/05/ubuntu-infrastructure-has-been-down-for-more-than-a-day/](https://arstechnica.com/security/2026/05/ubuntu-infrastructure-has-been-down-for-more-than-a-day/)

生成摘要时出错

---

## 41. Metal Gear Solid 2's source code has been leaked on 4chan

**原文标题**: Metal Gear Solid 2's source code has been leaked on 4chan

**原文链接**: [https://www.thegamer.com/mgs2-hd-edition-source-code-massive-leak/](https://www.thegamer.com/mgs2-hd-edition-source-code-massive-leak/)

生成摘要时出错

---

## 42. How far behind is each major Chromium browser?

**原文标题**: How far behind is each major Chromium browser?

**原文链接**: [https://chromium-drift.pages.dev/](https://chromium-drift.pages.dev/)

生成摘要时出错

---

## 43. Investors pile into clean energy as Iran war drives push for energy security

**原文标题**: Investors pile into clean energy as Iran war drives push for energy security

**原文链接**: [https://www.ft.com/content/9921f2b5-c910-4cec-a50f-cad453935a1a](https://www.ft.com/content/9921f2b5-c910-4cec-a50f-cad453935a1a)

生成摘要时出错

---

## 44. Refusal in Language Models Is Mediated by a Single Direction

**原文标题**: Refusal in Language Models Is Mediated by a Single Direction

**原文链接**: [https://arxiv.org/abs/2406.11717](https://arxiv.org/abs/2406.11717)

生成摘要时出错

---

## 45. Zugzwang

**原文标题**: Zugzwang

**原文链接**: [https://en.wikipedia.org/wiki/Zugzwang](https://en.wikipedia.org/wiki/Zugzwang)

生成摘要时出错

---

## 46. A physics engine with incremental rollback for multiplayer games

**原文标题**: A physics engine with incremental rollback for multiplayer games

**原文链接**: [https://easel.games/blog/2026-rollback-physics](https://easel.games/blog/2026-rollback-physics)

生成摘要时出错

---

## 47. K3k: Kubernetes in Kubernetes

**原文标题**: K3k: Kubernetes in Kubernetes

**原文链接**: [https://github.com/rancher/k3k](https://github.com/rancher/k3k)

生成摘要时出错

---

## 48. A desktop made for one

**原文标题**: A desktop made for one

**原文链接**: [https://isene.org/2026/05/Audience-of-One.html](https://isene.org/2026/05/Audience-of-One.html)

生成摘要时出错

---

## 49. An unknown Sega Saturn project has come to light after 29 years

**原文标题**: An unknown Sega Saturn project has come to light after 29 years

**原文链接**: [https://32bits.substack.com/p/under-the-microscope-pyramid-unreleased](https://32bits.substack.com/p/under-the-microscope-pyramid-unreleased)

生成摘要时出错

---

## 50. Whimsical Animations Course Open House

**原文标题**: Whimsical Animations Course Open House

**原文链接**: [https://courses.joshwcomeau.com/wham/open-house/00-introduction](https://courses.joshwcomeau.com/wham/open-house/00-introduction)

生成摘要时出错

---

## 51. Unsigned sizes: A five year mistake

**原文标题**: Unsigned sizes: A five year mistake

**原文链接**: [https://c3-lang.org/blog/unsigned-sizes-a-five-year-mistake/](https://c3-lang.org/blog/unsigned-sizes-a-five-year-mistake/)

生成摘要时出错

---

## 52. Southwest Headquarters Tour

**原文标题**: Southwest Headquarters Tour

**原文链接**: [https://katherinemichel.github.io/blog/travel/southwest-headquarters-tour-2026.html](https://katherinemichel.github.io/blog/travel/southwest-headquarters-tour-2026.html)

生成摘要时出错

---

## 53. Flue is a TypeScript framework for building the next generation of agents

**原文标题**: Flue is a TypeScript framework for building the next generation of agents

**原文链接**: [https://flueframework.com/](https://flueframework.com/)

生成摘要时出错

---

## 54. Care homes and hotels in Japan shut as expansion strategy unravels

**原文标题**: Care homes and hotels in Japan shut as expansion strategy unravels

**原文链接**: [https://www.newsonjapan.com/article/149075.php](https://www.newsonjapan.com/article/149075.php)

生成摘要时出错

---

## 55. Windows API is Successful Cross-Platform API (2024)

**原文标题**: Windows API is Successful Cross-Platform API (2024)

**原文链接**: [https://retrocoding.net/windows-api-is-successful-cross-platform-api](https://retrocoding.net/windows-api-is-successful-cross-platform-api)

生成摘要时出错

---

## 56. Show HN: Agent-desktop – Native desktop automation CLI for AI agents

**原文标题**: Show HN: Agent-desktop – Native desktop automation CLI for AI agents

**原文链接**: [https://github.com/lahfir/agent-desktop](https://github.com/lahfir/agent-desktop)

生成摘要时出错

---

## 57. Porsche will contest Laguna Seca in historic colors of the Apple Computer livery

**原文标题**: Porsche will contest Laguna Seca in historic colors of the Apple Computer livery

**原文链接**: [https://newsroom.porsche.com/en_US/2026/motorsport/porsche-will-contest-laguna-seca-in-historic-colors-of-the-apple-computer-livery.html](https://newsroom.porsche.com/en_US/2026/motorsport/porsche-will-contest-laguna-seca-in-historic-colors-of-the-apple-computer-livery.html)

生成摘要时出错

---

## 58. BYOMesh – New LoRa mesh radio offers 100x the bandwidth

**原文标题**: BYOMesh – New LoRa mesh radio offers 100x the bandwidth

**原文链接**: [https://partyon.xyz/@nullagent/116499715071759135](https://partyon.xyz/@nullagent/116499715071759135)

生成摘要时出错

---

## 59. Modern C++ Programming: Busato

**原文标题**: Modern C++ Programming: Busato

**原文链接**: [https://github.com/federico-busato/Modern-CPP-Programming](https://github.com/federico-busato/Modern-CPP-Programming)

生成摘要时出错

---

## 60. Nuclear receptor 4A1 linked to health effects of coffee: study

**原文标题**: Nuclear receptor 4A1 linked to health effects of coffee: study

**原文链接**: [https://sciencex.com/news/2026-04-coffee-doesnt-key-biological-pathway.html](https://sciencex.com/news/2026-04-coffee-doesnt-key-biological-pathway.html)

生成摘要时出错

---

## 61. OpenAI's o1 correctly diagnosed 67% of ER patients vs. 50-55% by triage doctors

**原文标题**: OpenAI's o1 correctly diagnosed 67% of ER patients vs. 50-55% by triage doctors

**原文链接**: [https://www.theguardian.com/technology/2026/apr/30/ai-outperforms-doctors-in-harvard-trial-of-emergency-triage-diagnoses](https://www.theguardian.com/technology/2026/apr/30/ai-outperforms-doctors-in-harvard-trial-of-emergency-triage-diagnoses)

生成摘要时出错

---

## 62. Waymo Drives Off with South Bay Man's Luggage

**原文标题**: Waymo Drives Off with South Bay Man's Luggage

**原文链接**: [https://sfist.com/2026/05/01/waymo-drives-off-with-south-bay-mans-luggage-after-trunk-fails-to-open/](https://sfist.com/2026/05/01/waymo-drives-off-with-south-bay-mans-luggage-after-trunk-fails-to-open/)

生成摘要时出错

---

## 63. Spirit Airlines canceled all flights and is going out of business

**原文标题**: Spirit Airlines canceled all flights and is going out of business

**原文链接**: [https://www.cnn.com/2026/05/02/business/spirit-to-halt-all-flights](https://www.cnn.com/2026/05/02/business/spirit-to-halt-all-flights)

生成摘要时出错

---

## 64. GameStop Preparing Offer for eBay

**原文标题**: GameStop Preparing Offer for eBay

**原文链接**: [https://www.wsj.com/business/deals/gamestop-preparing-offer-for-ebay-1678e6de](https://www.wsj.com/business/deals/gamestop-preparing-offer-for-ebay-1678e6de)

生成摘要时出错

---

## 65. Alert-driven monitoring

**原文标题**: Alert-driven monitoring

**原文链接**: [https://simpleobservability.com/docs/alert-driven-monitoring](https://simpleobservability.com/docs/alert-driven-monitoring)

生成摘要时出错

---

## 66. Voice-AI-for-Beginners – A curated learning path for developers

**原文标题**: Voice-AI-for-Beginners – A curated learning path for developers

**原文链接**: [https://github.com/mahimairaja/voiceai](https://github.com/mahimairaja/voiceai)

生成摘要时出错

---

## 67. Systemd-manager-TUI: A TUI application for managing systemd services

**原文标题**: Systemd-manager-TUI: A TUI application for managing systemd services

**原文链接**: [https://github.com/Matheus-git/systemd-manager-tui](https://github.com/Matheus-git/systemd-manager-tui)

生成摘要时出错

---

## 68. The Claude Delusion: Richard Dawkins believes his AI chatbot is conscious

**原文标题**: The Claude Delusion: Richard Dawkins believes his AI chatbot is conscious

**原文链接**: [https://www.dailygrail.com/2026/05/the-claude-delusion-richard-dawkins-believes-his-female-ai-chatbot-is-conscious/](https://www.dailygrail.com/2026/05/the-claude-delusion-richard-dawkins-believes-his-female-ai-chatbot-is-conscious/)

生成摘要时出错

---

## 69. Why TUIs Are Back

**原文标题**: Why TUIs Are Back

**原文链接**: [https://wiki.alcidesfonseca.com/blog/why-tuis-are-back/](https://wiki.alcidesfonseca.com/blog/why-tuis-are-back/)

生成摘要时出错

---

## 70. Welcome to Hell Developer

**原文标题**: Welcome to Hell Developer

**原文链接**: [https://noahclements.com/Wahoo-Bolt-Hidden-Debug-Mode/](https://noahclements.com/Wahoo-Bolt-Hidden-Debug-Mode/)

生成摘要时出错

---

## 71. AI, Intimacy, and the Data You Never Meant to Share

**原文标题**: AI, Intimacy, and the Data You Never Meant to Share

**原文链接**: [https://fshot.org/techzone/the-algorithm-knows.php](https://fshot.org/techzone/the-algorithm-knows.php)

生成摘要时出错

---

## 72. Spirit Airlines Is Winding Down All Operations

**原文标题**: Spirit Airlines Is Winding Down All Operations

**原文链接**: [https://www.spiritrestructuring.com/](https://www.spiritrestructuring.com/)

生成摘要时出错

---

## 73. Security through obscurity is not bad

**原文标题**: Security through obscurity is not bad

**原文链接**: [https://mobeigi.com/blog/security/security-through-obscurity-is-not-bad/](https://mobeigi.com/blog/security/security-through-obscurity-is-not-bad/)

生成摘要时出错

---

## 74. Show HN: Mljar Studio – local AI data analyst that saves analysis as notebooks

**原文标题**: Show HN: Mljar Studio – local AI data analyst that saves analysis as notebooks

**原文链接**: [https://mljar.com/](https://mljar.com/)

生成摘要时出错

---

## 75. Canonical Under Attack

**原文标题**: Canonical Under Attack

**原文链接**: [https://status.canonical.com](https://status.canonical.com)

生成摘要时出错

---

## 76. Am I the only one who hates delivery robots?

**原文标题**: Am I the only one who hates delivery robots?

**原文链接**: [https://www.latimes.com/entertainment-arts/story/2026-04-14/delivery-robots-creating-problems-glendale-ban](https://www.latimes.com/entertainment-arts/story/2026-04-14/delivery-robots-creating-problems-glendale-ban)

生成摘要时出错

---

## 77. Show HN: Piruetas – A self-hosted diary app I built for my girlfriend

**原文标题**: Show HN: Piruetas – A self-hosted diary app I built for my girlfriend

**原文链接**: [https://piruet.app](https://piruet.app)

生成摘要时出错

---

## 78. Pushed by Trump policies, top U.S. battery scientist is moving to Singapore

**原文标题**: Pushed by Trump policies, top U.S. battery scientist is moving to Singapore

**原文链接**: [https://www.science.org/content/article/pushed-trump-policies-top-u-s-battery-scientist-moving-singapore](https://www.science.org/content/article/pushed-trump-policies-top-u-s-battery-scientist-moving-singapore)

生成摘要时出错

---

## 79. New US phone network for Christians to block porn and gender-related content

**原文标题**: New US phone network for Christians to block porn and gender-related content

**原文链接**: [https://www.technologyreview.com/2026/05/01/1136739/a-new-t-mobile-network-for-christians-aims-to-block-porn-and-gender-related-content/](https://www.technologyreview.com/2026/05/01/1136739/a-new-t-mobile-network-for-christians-aims-to-block-porn-and-gender-related-content/)

生成摘要时出错

---

## 80. Breaking up with WordPress after two decades

**原文标题**: Breaking up with WordPress after two decades

**原文链接**: [https://yusufaytas.com/breaking-up-with-wordpress-after-two-decades](https://yusufaytas.com/breaking-up-with-wordpress-after-two-decades)

生成摘要时出错

---

## 81. U.S. to Withdraw 5k Troops from Germany, Pentagon Says

**原文标题**: U.S. to Withdraw 5k Troops from Germany, Pentagon Says

**原文链接**: [https://www.nytimes.com/2026/05/01/us/politics/us-troops-germany.html](https://www.nytimes.com/2026/05/01/us/politics/us-troops-germany.html)

生成摘要时出错

---

## 82. The Oscars just banned AI from winning acting and writing awards

**原文标题**: The Oscars just banned AI from winning acting and writing awards

**原文链接**: [https://gizmodo.com/the-oscars-just-banned-ai-from-winning-acting-and-writing-awards-2000753740](https://gizmodo.com/the-oscars-just-banned-ai-from-winning-acting-and-writing-awards-2000753740)

生成摘要时出错

---

## 83. Becoming a father shrinks your cerebrum (2022)

**原文标题**: Becoming a father shrinks your cerebrum (2022)

**原文链接**: [https://www.economist.com/science-and-technology/2022/10/21/becoming-a-father-shrinks-your-cerebrum](https://www.economist.com/science-and-technology/2022/10/21/becoming-a-father-shrinks-your-cerebrum)

生成摘要时出错

---

## 84. What did you love about VB6?

**原文标题**: What did you love about VB6?

**原文链接**: [https://evilgeniuslabs.ca/blog/vb6-modern-dotnet-question](https://evilgeniuslabs.ca/blog/vb6-modern-dotnet-question)

生成摘要时出错

---

## 85. Craig Venter of Human Genome Project Dies at 79

**原文标题**: Craig Venter of Human Genome Project Dies at 79

**原文链接**: [https://www.economist.com/obituary/2026/05/01/craig-venter-raced-to-decode-the-human-genome](https://www.economist.com/obituary/2026/05/01/craig-venter-raced-to-decode-the-human-genome)

生成摘要时出错

---

## 86. I Do Not Recommend Bitwarden

**原文标题**: I Do Not Recommend Bitwarden

**原文链接**: [https://xn--gckvb8fzb.com/i-do-not-recommend-bitwarden/](https://xn--gckvb8fzb.com/i-do-not-recommend-bitwarden/)

生成摘要时出错

---

## 87. Oil tanker hijacked off Yemen, steers toward Somalia

**原文标题**: Oil tanker hijacked off Yemen, steers toward Somalia

**原文链接**: [https://www.yahoo.com/news/articles/yemen-says-oil-tanker-hijacked-121710980.html](https://www.yahoo.com/news/articles/yemen-says-oil-tanker-hijacked-121710980.html)

生成摘要时出错

---

## 88. Uncle Bob: It's Over

**原文标题**: Uncle Bob: It's Over

**原文链接**: [https://old.reddit.com/r/vibecoding/comments/1srfqm0/uncle_bob_its_over/](https://old.reddit.com/r/vibecoding/comments/1srfqm0/uncle_bob_its_over/)

生成摘要时出错

---

## 89. Business Owners Are Worst Clients

**原文标题**: Business Owners Are Worst Clients

**原文链接**: [https://zencapital.substack.com/p/business-owners-are-worst-clients](https://zencapital.substack.com/p/business-owners-are-worst-clients)

生成摘要时出错

---

## 90. Show HN: Filling PDF forms with AI using client-side tool calling

**原文标题**: Show HN: Filling PDF forms with AI using client-side tool calling

**原文链接**: [https://copilot.simplepdf.com/?share=a7d00ad073c75a75d493228e6ff7b11eb3f2d945b6175913e87898ec96ca8076&form=w9&lang=en](https://copilot.simplepdf.com/?share=a7d00ad073c75a75d493228e6ff7b11eb3f2d945b6175913e87898ec96ca8076&form=w9&lang=en)

生成摘要时出错

---

## 91. The feed doesn't know you, and YouTube refuses to let you browse

**原文标题**: The feed doesn't know you, and YouTube refuses to let you browse

**原文链接**: [https://evilgeniuslabs.ca/blog/the-feed-doesnt-know-you](https://evilgeniuslabs.ca/blog/the-feed-doesnt-know-you)

生成摘要时出错

---

## 92. Meta's Pyrefly sabotages competing Python extensions without telling you

**原文标题**: Meta's Pyrefly sabotages competing Python extensions without telling you

**原文链接**: [https://github.com/facebook/pyrefly/issues/3292](https://github.com/facebook/pyrefly/issues/3292)

生成摘要时出错

---

## 93. Show HN: Large Scale Article Extract of Newspapers 1730s-1960s

**原文标题**: Show HN: Large Scale Article Extract of Newspapers 1730s-1960s

**原文链接**: [https://snewpapers.com/](https://snewpapers.com/)

生成摘要时出错

---

## 94. Palantir Workers Are Finally Noticing the Skulls on Their Caps

**原文标题**: Palantir Workers Are Finally Noticing the Skulls on Their Caps

**原文链接**: [https://www.techdirt.com/2026/04/30/palantir-workers-are-finally-noticing-the-skulls-on-their-caps/](https://www.techdirt.com/2026/04/30/palantir-workers-are-finally-noticing-the-skulls-on-their-caps/)

生成摘要时出错

---

## 95. Notes on a non-profit indicted for bank fraud

**原文标题**: Notes on a non-profit indicted for bank fraud

**原文链接**: [https://www.bitsaboutmoney.com/archive/nonprofit-indicted-bank-fraud/](https://www.bitsaboutmoney.com/archive/nonprofit-indicted-bank-fraud/)

生成摘要时出错

---

## 96. Show HN: Destiny – Claude Code's fortune Teller skill

**原文标题**: Show HN: Destiny – Claude Code's fortune Teller skill

**原文链接**: [https://github.com/xodn348/destiny](https://github.com/xodn348/destiny)

生成摘要时出错

---

## 97. Redistricting and the Supreme Court have cut voters out of US House races

**原文标题**: Redistricting and the Supreme Court have cut voters out of US House races

**原文链接**: [https://www.reuters.com/legal/government/how-redistricting-supreme-court-have-cut-voters-out-us-house-races-2026-05-03/](https://www.reuters.com/legal/government/how-redistricting-supreme-court-have-cut-voters-out-us-house-races-2026-05-03/)

生成摘要时出错

---

## 98. Santa Cruz restaurant changes logo after flurry of negative reviews for AI art

**原文标题**: Santa Cruz restaurant changes logo after flurry of negative reviews for AI art

**原文链接**: [https://www.sfgate.com/food/article/santa-cruz-restaurant-ai-21955920.php](https://www.sfgate.com/food/article/santa-cruz-restaurant-ai-21955920.php)

生成摘要时出错

---

## 99. Show HN: Browser-based light pollution simulator using real photometric data

**原文标题**: Show HN: Browser-based light pollution simulator using real photometric data

**原文链接**: [https://iesna.eu/?wasm=skyglow_demo](https://iesna.eu/?wasm=skyglow_demo)

生成摘要时出错

---

## 100. Bad Connection: Global telecom exploitation by covert surveillance actors

**原文标题**: Bad Connection: Global telecom exploitation by covert surveillance actors

**原文链接**: [https://citizenlab.ca/research/uncovering-global-telecom-exploitation-by-covert-surveillance-actors/](https://citizenlab.ca/research/uncovering-global-telecom-exploitation-by-covert-surveillance-actors/)

生成摘要时出错

---

