# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-05-03.md)

*最后自动更新时间: 2026-05-03 20:19:35*
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

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 2 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 3 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 4 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 5 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 6 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 7 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 8 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 9 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 10 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 11 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 12 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 13 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 14 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 15 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 16 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 17 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 18 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 19 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 20 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 21 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 22 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 23 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 24 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 25 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 26 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 27 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 28 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 29 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 30 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 31 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 32 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 33 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 34 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 35 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 36 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 37 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 38 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 39 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 40 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 41 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 42 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 43 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 44 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 45 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 46 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 47 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 48 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 49 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 50 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 51 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 52 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 53 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 54 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 55 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 56 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 57 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 58 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 59 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 60 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 61 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 62 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 63 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 64 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 65 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 66 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 67 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 68 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 69 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 70 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 71 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 72 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 73 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 74 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 75 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 76 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 77 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 78 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 79 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 80 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 81 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 82 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 83 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 84 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 85 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 86 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 87 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 88 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 89 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 90 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 91 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 92 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 93 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 94 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 95 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 96 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 97 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 98 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 99 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 100 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 101 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 102 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 103 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 104 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 105 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 106 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 107 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 108 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 109 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 110 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 111 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 112 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 113 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 114 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 115 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 116 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 117 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 118 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 119 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 120 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 121 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 122 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 123 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 124 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 125 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 126 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 127 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 128 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 129 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 130 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 131 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 132 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 133 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 134 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 135 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 136 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 137 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 138 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 139 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 140 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 141 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 142 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 143 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 144 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 145 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 146 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 147 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 148 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 149 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 150 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 151 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 152 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 153 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 154 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 155 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 156 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 157 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 158 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 159 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 160 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 161 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 162 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 163 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 164 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 165 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 166 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 167 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 168 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 169 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 170 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 171 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 172 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 173 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 174 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 175 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 176 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 177 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
