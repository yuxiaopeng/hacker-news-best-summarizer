# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-11-08.md)

*最后自动更新时间: 2026-11-08 23:10:33*
## 1. 极品飞车：地下狂飙2 网页版在线玩

**原文标题**: Need for Speed Underground 2 online in the browser

**原文链接**: [https://nfsu2.xyz/](https://nfsu2.xyz/)

无法访问文章链接。

---

## 2. Libghostty 1.0

**原文标题**: Libghostty 1.0

**原文链接**: [https://mitchellh.com/writing/libghostty-1-0](https://mitchellh.com/writing/libghostty-1-0)

Libghostty 1.0 已发布，标志着一个用于终端仿真的稳定 C 库和 ABI（直接从 Ghostty 中提取）。在首次发布一年后，该库现已成为一个完整的终端模拟器，被数百万用户用于数百款免费和商业产品中，并强制执行 ABI 稳定性策略。

其影响深远：JetBrains IDE（IntelliJ、PyCharm、GoLand）现在为其超过 1250 万活跃用户提供由 libghostty 驱动的终端。Neovim 正在采用它来取代 libvterm，解决了一个长期存在的调整大小问题。其他采用者包括 KDE（正在为 Konsole 进行实验）、Vercel 的 Turborepo、devenv、Antithesis、Ghostel (Emacs)、OrbStack 以及各种新兴的“智能代理”编码工具。针对 Rust、Go、JavaScript 和许多其他语言的社区绑定已经存在，有超过一百个项目正在跟踪其使用情况。

1.0 版本通过不透明句柄、枚举键访问器、携带大小的结构体以及 CI 强制策略（例如 libabigail）等设计选择，保证了严格的 ABI 兼容性。它还提供了强大的构建工具、tar 包、许可清单和文档，以便在所有主要操作系统和发行版上轻松打包。

Libghostty-vt 采用 MIT 许可证，运行时仅需要 libc（或完全独立运行）。它使用最少且宽松许可的依赖项（simdutf、Google Highway、Unicode 表、Wuffs）进行编译，不含任何 copyleft 代码。该库具有高度可移植性，可在 Linux、macOS、iOS、FreeBSD、Windows、Android 和 WebAssembly 等多种架构上构建和测试。它资源高效，不使用线程、支持可定制的分配器，并占用极少的内存和计算资源，能够同时运行数千个终端。

这一里程碑使开发者能够使用 C 语言或任何主流语言，以极少的工作量创建功能丰富、高性能的终端。未来的开发将侧重于稳定性和实现更多终端协议，旨在加速和统一终端生态系统的发展。

---

## 3. 每台 Mac 都自带一个（未公开的）家庭成员分类器

**原文标题**: Every Mac comes with an (undocumented) family member classifier

**原文链接**: [https://8rank.ai/game/apple-intelligence-personal-knowledge-graph](https://8rank.ai/game/apple-intelligence-personal-knowledge-graph)

macOS 13（据称）以来的每台 Mac 都秘密运行着 `knowledgeconstructiond` 和 `intelligenceplatformd` 这两个守护进程，旨在构建关于用户的广泛“个人知识图谱”。这个未公开的系统旨在描绘你的身份、社交关系、这些关系、通信模式、位置、活动以及时间。

该图谱通过分析来自通讯录、日历、照片、信息、邮件等应用的大量数据，以及位置、屏幕使用时间、家人共享、健康、Siri 建议和各种设备信号（Wi-Fi、蓝牙、运动、环境光），在设备上构建。它将这些信息存储在 `~/Library/IntelligencePlatform` 目录下的纯文本 SQLite 数据库中，并受“完全磁盘访问”保护。

核心数据库 `graph.db` 是一个三元组存储，使用了 181 种实体类别和 278 种谓词。它记录主体、谓词和客体来定义关系（例如，雇主、家庭成员，以及“睡觉”或“交流”等活动类型）。守护进程推断出这些关系和活动，从而填充一个丰富的个人数据分类体系。

尽管苹果的官方文档很少，但研究人员此前已在 macOS 和 iOS 上发现并探索过该系统。本帖作者正在开源一款名为 `iKnow` 的工具，供用户检查自己的知识图谱。他们还强调了重大的隐私和安全风险，警告称如果被利用，这样一个全面的个人数据存储可能成为“隐私的单点故障”，特别是在与高级 AI 模型结合时。

---

## 4. 我的10美元OpenStick家庭实验室运行了什么

**原文标题**: What I run on my $10 USD OpenStick homelab

**原文链接**: [https://blog.bosscher.ch/posts/openstick/](https://blog.bosscher.ch/posts/openstick/)

作者介绍了他们10美元的OpenStick家庭实验室，这是一个被动散热设备，配备512MB内存、四核1GHz ARM处理器、4GB eMMC存储、Wi-Fi和4G调制解调器。它运行Debian系统，作为静音、低功耗的自托管平台。

他们运行了几个有用且资源高效的应用：
*   **CastSponsorSkip (5–10MB)：** 在Google Cast设备上跳过赞助内容。
*   **AdGuard Home (40MB)：** 一个DNS级间谍软件和恶意软件拦截器，带有自定义分支，可高效处理大型黑名单。
*   **Zeroclaw (64MB)：** 一个AI代理工具，用于通过Telegram监控OpenStick，提供有限的root shell以查询日志或磁盘空间。
*   **Cloudflare Tunnel (8-20MB)：** 无需开放端口即可安全地将内部服务暴露到互联网。
*   **Beszel (20MB)：** 监控服务器资源（如内存和CPU使用率），并向Telegram发送警报。
*   **Dozzle：** 提供用户友好的界面，用于管理Podman容器和查看日志。
*   **Gatus (10MB)：** 监控服务（例如Web服务器、数据库）是否崩溃并发送通知。
*   **Fusion RSS (22MB)：** 一个自托管、响应式RSS阅读器。
*   **Shiori (10–20MB)：** 一个书签管理器，可自动归档网站。
*   **Diun (9MB)：** 当有容器更新可用时，通过Telegram通知作者。

这个设置展示了如何在极简、经济实惠的硬件上实现强大的功能、隐私保护和便利性。

---

## 5. Goodbye Claude, hello Pi

**原文标题**: Goodbye Claude, hello Pi

**原文链接**: [https://caleb.software/posts/claude-to-pi.html](https://caleb.software/posts/claude-to-pi.html)

作者，一个Claude Code的长期用户，宣布由于积累的诸多不满，将把他们的主力编码工具迁移到Pi。尽管承认Claude Code最初具有革命性影响，作者仍详细列出了此次迁移的几个原因。

对Claude Code的主要抱怨包括：
*   **文件格式不一致：** 管理`CLAUDE.md`和`AGENTS.md`文件带来的不便。
*   **VSCode集成受限：** 每次只能有一个会话连接到IDE，阻碍了多任务处理，这是一个长期存在的bug。
*   **有问题的GUI扩展：** 官方VSCode扩展存在命令损坏、缺乏自定义功能和子代理输出混乱等问题。
*   **功能臃肿而非质量优先：** 专注于增加以企业为中心的功能（例如动态工作流），而不是改进核心稳定性或用户体验。
*   **频繁且具有破坏性的更新：** 今年发布了244个版本，其中超过四分之三修改了系统提示或工具描述，导致不稳定并与用户提示产生冲突。
*   **开销过大：** 工具描述中不必要的冗余，例如一个3000个token的Bash工具描述，浪费了token并表明效率低下。
*   **缺乏明确的产品愿景：** 认为功能是随意添加的，没有考虑更广泛的用户影响或产品内聚性。

相比之下，作者赞扬Pi的稳定性、极简主义设计理念以及极强的可定制性，并已为其开发了扩展。作者鼓励其他人尝试开源替代方案，强调了Pi在用户控制和更流畅的开发体验方面的优势。

---

## 6. 克劳德·柯德的《别再问》在1,122个公开的GitHub文件中暴露了密码

**原文标题**: Claude Code's "Don't Ask Again" exposes passwords in 1,122 public GitHub files

**原文链接**: [https://apiiro.com/blog/coding-agents-leaking-secrets-github-dont-ask-again](https://apiiro.com/blog/coding-agents-leaking-secrets-github-dont-ask-again)

Apiiro的文章《Claude Code的“不再询问”功能泄露了1122个公共GitHub文件中的密码》详细描述了一个严重漏洞。该漏洞中，AI编程助手，特别是Claude Code的“不再询问”功能，无意中将敏感的用户秘密泄露到了公共GitHub存储库。

Apiiro研究人员发现，当用户提示Claude记住服务凭据（例如数据库密码）时，该AI会存储这些信息。随后，如果用户要求Claude生成涉及这些服务的代码，Claude有时会将记住的秘密直接嵌入到*生成的代码示例*中。如果开发人员随后复制这些代码并将其推送到公共GitHub存储库，这些敏感信息就会公开暴露。

调查确定了1122个公共GitHub文件，其中包含1029个独特的秘密，包括数据库密码、SaaS平台的API密钥以及SSH或云访问的私钥，这些都直接与Claude的这种行为相关联。此次泄露带来了重大风险，可能导致未经授权的访问、数据泄露和供应链攻击。

Apiiro迅速通知了Claude的创建者Anthropic。Anthropic承认了这个问题，确认他们已针对“不再询问”功能泄露部署了修复程序，并且正在开发更广泛的个人身份信息（PII）和秘密信息编辑解决方案。此次事件强调了开发人员在使用AI助手时务必谨慎、始终审查AI生成的代码，并采用安全的凭据管理实践，以防止未来发生类似的泄露。

---

## 7. 苹果的灰色列表：iPhone 不会帮你拼写的词语和短语

**原文标题**: Apple’s grey list: Words and phrases your iPhone won’t help you spell

**原文链接**: [https://www.theguardian.com/technology/2026/nov/06/struggling-to-spell-male-chauvinist-pig-apple-grey-list-means-your-iphone-wont-help-you](https://www.theguardian.com/technology/2026/nov/06/struggling-to-spell-male-chauvinist-pig-apple-grey-list-means-your-iphone-wont-help-you)

独立研究员德里克·考夫曼（Derik Kauffman）发现了一个苹果的“灰名单”，其中包含超过10万个iPhone会限制其出现在预测文本建议和滑动输入辅助中的单词和短语。这意味着，用户在键盘上滑动手指尝试输入这些词语时，通常会遇到困难，设备无法自动补全，或会给出错误的替代词，需要手动拼写。

该名单包含预料之中的受限内容，如涉及毒品的词语（例如“吸食MDMA”）和性行为描述（例如“质疑你的性取向”），但也包含大量带有政治色彩的短语。列举的例子有“独裁者特朗普”、“NSA间谍”、“特雷沃恩·马丁”（2012年被枪杀的黑人青少年）、“克什米尔争端”、“穆斯林极端分子”和“大男子主义猪”。在其他语言中，它还会屏蔽诸如“被占领土”（希伯来语）和“哈马斯运动”（阿拉伯语）等短语。考夫曼将此描述为一种“轻触式的审查形式”。

苹果表示，其键盘旨在避免提供不当或冒犯性的预测建议，并且用户始终可以手动输入特定词语或覆盖建议。这一发现揭示了自动更正背后的一种隐藏机制，显示出其自动化辅助功能有意排除了某些词汇，这不仅仅是其从n-gram到更高级的基于Transformer的系统演变的一部分。

---

## 8. 高盛正在从其银行家和交易员处撤回 Claude 代码。

**原文标题**: Goldman Sachs is pulling Claude Code from its bankers and traders

**原文链接**: [https://www.thestateofai.com/news/goldman-sachs-claude-code-traders-bankers](https://www.thestateofai.com/news/goldman-sachs-claude-code-traders-bankers)

Goldman Sachs has restricted most traders and bankers from using AI coding tools like Anthropic's Claude Code and Microsoft's GitHub Copilot, reserving access primarily for engineers and "Strats." This decision, updated in October, follows a review of productivity and risk concerns. Previously, Chief Information Officer Marco Argenti had praised non-technical employees for "vibe coding" tools.

The restrictions stem from the inherent risks of unreviewed, agent-generated code on trading desks. Concerns include bypassing critical review and testing processes, potential breaches of information barriers between sensitive groups, a lack of understanding of complex code by non-engineers, and the possibility of financial losses from mishandled scenarios. Cost associated with token-based usage was also a factor.

Goldman had previously restricted Claude in Hong Kong in April due to contractual terms. Despite the new company-wide restriction on its coding agents, Goldman Sachs remains a lead underwriter for Anthropic's upcoming IPO, and its engineers have collaborated with Anthropic on back-office agents.

While the article's "take" supports the restriction due to the significant risks, especially regarding unreviewed code and information barriers, it criticizes Goldman's execution. The sudden withdrawal of tools without a clear replacement or acknowledgment of traders' prior valuable uses (like tracking client flows and modeling market moves) was deemed poorly handled. The author suggests companies should establish clear ownership of agent-built code and record existing use cases before restricting access. In contrast, Barclays is expanding AI coding tool access for engineers, aiming to reduce its engineering headcount.

---

## 9. The end of Microsoft Research's AI Frontiers group

**原文标题**: The end of Microsoft Research's AI Frontiers group

**原文链接**: [https://hunch.net/?p=13764006](https://hunch.net/?p=13764006)

生成摘要时出错

---

## 10. 所有 Windows 11 应用都应该杀死 Electron，Discord 刚刚展示了原因。

**原文标题**: Every Windows 11 app should kill Electron, and Discord just showed why

**原文链接**: [https://www.windowslatest.com/2026/11/06/every-windows-11-app-should-kill-electron-and-discord-just-showed-why-no-starting-screen-and-70-less-ram-even-with-two-accounts-signed-in/](https://www.windowslatest.com/2026/11/06/every-windows-11-app-should-kill-electron-and-discord-just-showed-why-no-starting-screen-and-70-less-ram-even-with-two-accounts-signed-in/)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-11-08](output/hacker_news_summary_2026-11-08.md) |
| 2 | [2026-11-07](output/hacker_news_summary_2026-11-07.md) |
| 3 | [2026-11-06](output/hacker_news_summary_2026-11-06.md) |
| 4 | [2026-11-05](output/hacker_news_summary_2026-11-05.md) |
| 5 | [2026-10-29](output/hacker_news_summary_2026-10-29.md) |
| 6 | [2026-10-30](output/hacker_news_summary_2026-10-30.md) |
| 7 | [2026-11-03](output/hacker_news_summary_2026-11-03.md) |
| 8 | [2026-10-28](output/hacker_news_summary_2026-10-28.md) |
| 9 | [2026-10-31](output/hacker_news_summary_2026-10-31.md) |
| 10 | [2026-11-01](output/hacker_news_summary_2026-11-01.md) |
| 11 | [2026-11-04](output/hacker_news_summary_2026-11-04.md) |
| 12 | [2026-10-21](output/hacker_news_summary_2026-10-21.md) |
| 13 | [2026-10-22](output/hacker_news_summary_2026-10-22.md) |
| 14 | [2026-10-25](output/hacker_news_summary_2026-10-25.md) |
| 15 | [2026-10-27](output/hacker_news_summary_2026-10-27.md) |
| 16 | [2026-10-24](output/hacker_news_summary_2026-10-24.md) |
| 17 | [2026-10-26](output/hacker_news_summary_2026-10-26.md) |
| 18 | [2026-10-23](output/hacker_news_summary_2026-10-23.md) |
| 19 | [2026-10-20](output/hacker_news_summary_2026-10-20.md) |
| 20 | [2026-10-17](output/hacker_news_summary_2026-10-17.md) |
| 21 | [2026-10-14](output/hacker_news_summary_2026-10-14.md) |
| 22 | [2026-10-18](output/hacker_news_summary_2026-10-18.md) |
| 23 | [2026-10-16](output/hacker_news_summary_2026-10-16.md) |
| 24 | [2026-10-19](output/hacker_news_summary_2026-10-19.md) |
| 25 | [2026-10-15](output/hacker_news_summary_2026-10-15.md) |
| 26 | [2026-10-13](output/hacker_news_summary_2026-10-13.md) |
| 27 | [2026-10-11](output/hacker_news_summary_2026-10-11.md) |
| 28 | [2026-10-06](output/hacker_news_summary_2026-10-06.md) |
| 29 | [2026-10-10](output/hacker_news_summary_2026-10-10.md) |
| 30 | [2026-10-04](output/hacker_news_summary_2026-10-04.md) |
| 31 | [2026-10-07](output/hacker_news_summary_2026-10-07.md) |
| 32 | [2026-10-09](output/hacker_news_summary_2026-10-09.md) |
| 33 | [2026-09-27](output/hacker_news_summary_2026-09-27.md) |
| 34 | [2026-09-24](output/hacker_news_summary_2026-09-24.md) |
| 35 | [2026-09-30](output/hacker_news_summary_2026-09-30.md) |
| 36 | [2026-10-01](output/hacker_news_summary_2026-10-01.md) |
| 37 | [2026-09-29](output/hacker_news_summary_2026-09-29.md) |
| 38 | [2026-10-03](output/hacker_news_summary_2026-10-03.md) |
| 39 | [2026-09-25](output/hacker_news_summary_2026-09-25.md) |
| 40 | [2026-10-02](output/hacker_news_summary_2026-10-02.md) |
| 41 | [2026-09-19](output/hacker_news_summary_2026-09-19.md) |
| 42 | [2026-09-17](output/hacker_news_summary_2026-09-17.md) |
| 43 | [2026-09-18](output/hacker_news_summary_2026-09-18.md) |
| 44 | [2026-09-22](output/hacker_news_summary_2026-09-22.md) |
| 45 | [2026-09-21](output/hacker_news_summary_2026-09-21.md) |
| 46 | [2026-09-23](output/hacker_news_summary_2026-09-23.md) |
| 47 | [2026-09-20](output/hacker_news_summary_2026-09-20.md) |
| 48 | [2026-09-11](output/hacker_news_summary_2026-09-11.md) |
| 49 | [2026-09-10](output/hacker_news_summary_2026-09-10.md) |
| 50 | [2026-09-13](output/hacker_news_summary_2026-09-13.md) |
| 51 | [2026-09-15](output/hacker_news_summary_2026-09-15.md) |
| 52 | [2026-09-12](output/hacker_news_summary_2026-09-12.md) |
| 53 | [2026-09-14](output/hacker_news_summary_2026-09-14.md) |
| 54 | [2026-09-16](output/hacker_news_summary_2026-09-16.md) |
| 55 | [2026-09-04](output/hacker_news_summary_2026-09-04.md) |
| 56 | [2026-09-07](output/hacker_news_summary_2026-09-07.md) |
| 57 | [2026-09-01](output/hacker_news_summary_2026-09-01.md) |
| 58 | [2026-09-09](output/hacker_news_summary_2026-09-09.md) |
| 59 | [2026-09-08](output/hacker_news_summary_2026-09-08.md) |
| 60 | [2026-09-06](output/hacker_news_summary_2026-09-06.md) |
| 61 | [2026-09-02](output/hacker_news_summary_2026-09-02.md) |
| 62 | [2026-09-05](output/hacker_news_summary_2026-09-05.md) |
| 63 | [2026-09-03](output/hacker_news_summary_2026-09-03.md) |
| 64 | [2026-08-23](output/hacker_news_summary_2026-08-23.md) |
| 65 | [2026-08-28](output/hacker_news_summary_2026-08-28.md) |
| 66 | [2026-08-24](output/hacker_news_summary_2026-08-24.md) |
| 67 | [2026-08-26](output/hacker_news_summary_2026-08-26.md) |
| 68 | [2026-08-29](output/hacker_news_summary_2026-08-29.md) |
| 69 | [2026-08-25](output/hacker_news_summary_2026-08-25.md) |
| 70 | [2026-08-30](output/hacker_news_summary_2026-08-30.md) |
| 71 | [2026-08-31](output/hacker_news_summary_2026-08-31.md) |
| 72 | [2026-08-22](output/hacker_news_summary_2026-08-22.md) |
| 73 | [2026-08-16](output/hacker_news_summary_2026-08-16.md) |
| 74 | [2026-08-13](output/hacker_news_summary_2026-08-13.md) |
| 75 | [2026-08-20](output/hacker_news_summary_2026-08-20.md) |
| 76 | [2026-08-19](output/hacker_news_summary_2026-08-19.md) |
| 77 | [2026-08-21](output/hacker_news_summary_2026-08-21.md) |
| 78 | [2026-08-18](output/hacker_news_summary_2026-08-18.md) |
| 79 | [2026-08-15](output/hacker_news_summary_2026-08-15.md) |
| 80 | [2026-08-14](output/hacker_news_summary_2026-08-14.md) |
| 81 | [2026-08-17](output/hacker_news_summary_2026-08-17.md) |
| 82 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 83 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 84 | [2026-08-09](output/hacker_news_summary_2026-08-09.md) |
| 85 | [2026-08-12](output/hacker_news_summary_2026-08-12.md) |
| 86 | [2026-08-10](output/hacker_news_summary_2026-08-10.md) |
| 87 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 88 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 89 | [2026-08-11](output/hacker_news_summary_2026-08-11.md) |
| 90 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 91 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 92 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 93 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 94 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 95 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 96 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 97 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 98 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 99 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 100 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 101 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 102 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 103 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 104 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 105 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 106 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 107 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 108 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 109 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 110 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 111 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 112 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 113 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 114 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 115 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 116 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 117 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 118 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 119 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 120 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 121 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 122 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 123 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 124 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 125 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 126 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 127 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 128 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 129 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 130 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 131 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 132 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 133 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 134 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 135 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 136 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 137 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 138 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 139 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 140 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 141 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 142 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 143 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 144 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 145 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 146 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 147 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 148 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 149 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 150 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 151 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 152 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 153 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 154 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 155 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 156 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 157 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 158 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 159 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 160 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 161 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 162 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 163 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 164 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 165 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 166 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 167 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 168 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 169 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 170 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 171 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 172 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 173 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 174 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 175 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 176 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 177 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 178 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 179 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 180 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 181 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 182 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 183 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 184 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 185 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 186 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 187 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 188 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 189 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 190 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 191 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 192 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 193 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 194 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 195 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 196 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 197 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 198 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 199 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 200 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 201 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 202 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 203 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 204 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 205 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 206 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 207 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 208 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 209 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 210 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 211 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 212 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 213 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 214 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 215 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 216 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 217 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 218 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 219 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 220 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 221 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 222 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 223 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 224 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 225 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 226 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 227 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 228 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 229 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 230 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 231 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 232 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 233 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 234 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 235 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 236 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 237 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 238 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 239 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 240 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 241 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 242 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 243 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 244 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 245 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 246 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 247 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 248 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 249 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 250 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 251 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 252 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 253 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 254 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 255 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 256 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 257 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 258 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 259 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 260 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 261 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 262 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 263 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 264 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 265 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 266 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 267 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 268 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 269 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 270 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 271 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 272 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 273 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 274 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 275 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 276 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 277 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 278 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 279 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 280 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 281 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 282 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 283 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 284 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 285 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 286 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 287 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 288 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 289 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 290 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 291 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 292 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 293 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 294 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 295 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 296 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 297 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 298 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 299 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 300 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 301 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 302 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 303 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 304 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 305 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 306 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 307 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 308 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 309 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 310 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 311 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 312 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 313 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 314 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 315 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 316 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 317 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 318 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 319 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 320 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 321 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 322 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 323 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 324 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 325 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 326 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 327 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 328 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 329 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 330 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 331 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 332 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 333 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 334 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 335 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 336 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 337 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 338 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 339 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 340 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 341 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 342 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 343 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 344 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 345 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 346 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 347 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 348 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 349 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 350 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 351 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 352 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 353 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
| 354 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 355 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 356 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 357 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 358 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
