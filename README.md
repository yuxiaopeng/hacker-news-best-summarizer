# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-07-16.md)

*最后自动更新时间: 2026-07-16 20:22:08*
## 1. TS-2026-009: Tailscale SSH 不安全的参数处理导致 root 权限访问

**原文标题**: TS-2026-009: Insecure argument handling in Tailscale SSH permitted root access

**原文链接**: [https://tailscale.com/security-bulletins](https://tailscale.com/security-bulletins)

Tailscale 解决了两个严重漏洞，均已在 1.98.9 版本中修复，并由 Anthropic 和 Ada Logics 报告。

第一个漏洞 TS-2026-009 影响了 Linux 上的 Tailscale SSH。不安全的参数处理允许以连字符（例如 `-i`）开头的用户名被 `getent(1)` 解释为标志。具体来说，`-i` 导致 `getent` 打印整个 `passwd` 文件，进而使 Tailscale 打开一个交互式 root 会话，绕过 ACLs。这意味着任何对 Linux 节点拥有 SSH 访问权限的用户都可以获取 root 权限。Tailscale SSH 现在拒绝使用以连字符开头的用户名。

第二个漏洞影响了 Tailscale Serve 和 Funnel。单个格式错误的 HTTP 请求，如果包含非绝对路径（不是以 '/' 开头），可能会在路径解析期间触发无限循环，永久占用一个 CPU 核心并导致拒绝服务。对于 Tailscale Serve，任何 tailnet 对等节点都可以利用此漏洞，而对于 Funnel，任何未经身份验证的互联网主机都可以利用。Tailscale 现在会终止非绝对路径的路径遍历。

强烈建议依赖 `autogroup:nonroot` 限制的 Linux 主机上的 Tailscale SSH 用户，或者运行 Tailscale Serve 或 Funnel 的用户，立即升级到 1.98.9 或更高版本。

---

## 2. 迈向无所不能的线束

**原文标题**: Towards a harness that can do anything

**原文链接**: [https://eardatasci.github.io/c/ambiance/index.html](https://eardatasci.github.io/c/ambiance/index.html)

本文提出了一种名为“Ambiance”的新型LLM框架，旨在通过利用模型对Unix/Linux环境的固有知识，将它们从聊天界面中解放出来。作者指出了一个优秀框架的关键属性：对代理的直观性、便于自我开发和审计的透明性、精简性、灵活性以及强大的错误恢复能力，同时最大程度地降低基于token的认知负荷。

其核心理念是利用LLM在编程和系统管理方面的大量训练。该假设认为，一个经过修改的Unix/Linux环境可以作为理想的代理框架。Ambiance借鉴了Unix哲学，倡导模块化、透明化的工具，这些工具各司其职、协同工作，并主要处理文本流。因此，“一切皆文件”，这简化了数据交互，并利用了LLM处理纯文本的优势。

Ambiance使用文件系统层次标准（FHS）来组织数据，允许代理导航熟悉的文件结构（例如，日志位于`/var`，工作区位于`/home`）。一个中央“内核”充当事件总线，监视文件系统的变化并调用LLM，确保不遗漏任何通知，并验证代理操作的安全性。该系统包含不同的“用户”，如`root`（系统级任务）、`pai`（面向人类的交互）和`librarian`（记录性能），所有用户都通过事件总线进行通信。

Ambiance背后的基本思想是，围绕模型已知的概念——文件、用户、日志、文档——构建框架是最有效且最具成本效益的方法。Ambiance是一个正在进行中的项目，可供公众测试。

---

## 3. Dependabot 版本更新推出默认包冷却期

**原文标题**: Dependabot version updates introduce default package cooldown

**原文链接**: [https://github.blog/changelog/2026-07-14-dependabot-version-updates-introduce-default-package-cooldown/](https://github.blog/changelog/2026-07-14-dependabot-version-updates-introduce-default-package-cooldown/)

Dependabot 为版本更新引入了一个新的默认“冷却期”。现在，在新版本在其注册表中可用之后，它将等待三天，然后才会打开一个版本更新的拉取请求。

这一新默认设置旨在防止供应链攻击，以及意外合并损坏或受损的新版本。这三天的延迟为维护者和社区提供了时间，来识别并指出新版本存在的任何问题，从而降低了用户在新版本发布后立即采用问题代码的风险。

值得注意的是，这一冷却期**仅适用于版本更新**。安全更新仍会立即打开，以确保关键修复能够及时应用。用户保留完全控制权，可以通过在其 `.github/dependabot.yml` 配置文件中使用 `cooldown` 选项，来自定义冷却期或完全禁用此功能。

此功能正在 github.com 上的所有受支持生态系统中推出，并将包含在 GitHub Enterprise Server (GHES) 3.23 中。更多详细信息可在 Dependabot 冷却期文档中查阅。

---

## 4. 电报无服务器

**原文标题**: Telegram Serverless

**原文链接**: [https://core.telegram.org/bots/serverless](https://core.telegram.org/bots/serverless)

Telegram 无服务器允许开发者直接在 Telegram 的基础设施上运行 Telegram 机器人和迷你应用的后端代码，完全消除了服务器配置、维护和扩展的需求。开发者编写纯 JavaScript 模块，并通过单个命令进行部署，受益于快速、隔离的 V8 沙箱、直接访问 Bot API 以及内置的由 SQLite 支持的数据库。

主要优势包括零基础设施管理、自动扩展以及 Bot API 和 HTTP 请求等“开箱即用”的功能。开发工作流程涉及使用 `tgcloud` CLI 将本地 JavaScript 文件（用于更新处理器、共享代码和数据库模式）同步到云端。像 `push` 这样的命令用于部署代码，而 `migrate` 则用于应用数据库模式更改。开发者可以在部署前使用 `npx tgcloud run` 在本地测试处理器。

项目结构将代码组织到 `handlers/`（不同更新类型的入口点）、`lib/`（可重用模块）和 `schema.js`（数据库表定义）中。Telegram 无服务器适用于对话式 AI 机器人、迷你应用后端、游戏和集成。它还通过 `AGENTS.md` 和 `docs/tgcloud-sdk.md` 文件提供对 AI 编码助手的集成支持，并允许直接通过移动设备上的 @BotFather 进行全面的项目管理。

---

## 5. 微软已发布软件更新，修补了至少570个安全漏洞。

**原文标题**: Microsoft has released software updates to plug at least 570 security holes

**原文链接**: [https://krebsonsecurity.com/2026/07/microsoft-patches-a-record-570-security-flaws/](https://krebsonsecurity.com/2026/07/microsoft-patches-a-record-570-security-flaws/)

微软发布了一项创纪录的软件更新，修补了其Windows操作系统及其他软件中至少570个安全漏洞，几乎是上个月更新量的三倍。此次显著增长归因于人工智能辅助漏洞发现。

此次更新包括近60个允许远程控制的“关键”漏洞，以及三个零日漏洞，其中两个正被积极利用。值得注意的修复解决了Active Directory联合身份验证服务 (CVE-2026-56155) 和Microsoft SharePoint (CVE-2026-56164) 中的权限提升问题，一个BitLocker安全绕过漏洞 (CVE-2026-50661)，以及Microsoft Copilot中一个高危远程代码执行漏洞 (CVE-2026-48561)。

虽然AI加速了漏洞发现，但Tenable公司的Satnam Narang等专家认为，它也让攻击者更容易快速设计出攻击手段。Narang批评微软的“可利用性指数”以人为中心，未能跟上AI驱动的攻击生成速度，他指出最初被评为“可能性较低”的漏洞也能被迅速利用。

这一趋势是行业性的，Adobe、思科、Mozilla、甲骨文和谷歌也增加了补丁发布频率，通常引用AI的影响。鉴于前所未有的补丁数量，建议用户备份系统并考虑在几天后应用更新，因为大量的补丁有时可能会引入稳定性问题。

---

## 6. 恩特 – 公开账目

**原文标题**: Ente – Opening Our Books

**原文链接**: [https://ente.com/open/](https://ente.com/open/)

Ente已公开披露其业务指标，对其业绩提供了全面的透明度。这篇题为“Ente – 公开账簿”的公告，来自Vishnu的博客，揭示了收入、付费客户和总注册账户的关键数据。

此次公开的数据包括2026年1月的具体（示例性）指标以及预计的年度总计。在活跃订阅收入方面，Ente报告称2026年1月为780,996美元，预计年收入为1,178,724美元。在用户基础方面，该公司在2026年1月拥有12,018名活跃订阅付费客户，预计全年将达到18,455名。此外，Ente在2026年1月注册了290,703个账户，预计全年注册账户总数将达到439,046个。这些指标通过折线图等可视化辅助工具呈现，使公司的财务和用户增长信息对公众透明可及。

---

## 7. 数据中心已将公众电价推高了230亿美元。

**原文标题**: Data centers have hiked electricity prices on the public by $23B

**原文链接**: [https://fortune.com/2026/07/14/data-centers-23-billion-electricity-bills/](https://fortune.com/2026/07/14/data-centers-23-billion-electricity-bills/)

Data centers are significantly driving up electricity demand, raising concerns about escalating costs for the public. A PJM market report estimates a $23 billion increase in customer electricity prices by 2028, primarily due to data center demand.

Electricity rates are determined by state utility commissions, who allocate the costs of infrastructure investments—such as power plants and transmission lines—among residential, commercial, and industrial customers. While costs are ideally borne by those who cause them, shared grid upgrades necessitated by data centers often result in costs being spread across all users.

A major concern is a potential loophole in "coincident peak demand" pricing. Data centers can finely tune their electricity consumption, potentially reducing usage precisely during system-wide peak loads. This strategic reduction could allow them to avoid paying costs allocated based on peak demand, despite their substantial overall energy consumption, a tactic already observed with cryptocurrency mining.

Residential customers also face a lack of effective representation in these rate-setting processes. While utility companies, large industries, and data centers employ experts to advocate for lower cost allocations to themselves, state consumer advocate offices are often legally barred from taking positions that favor one customer group over another. This leaves average households without dedicated advocacy on crucial cost allocation decisions.

Additional risks include "stranded costs" if planned data centers fail to materialize or become obsolete, leaving existing ratepayers to cover the initial infrastructure investments. The article emphasizes the importance of consumers understanding cost allocation and participating in public hearings to ensure their interests are represented.

---

## 8. Decoy Font

**原文标题**: Decoy Font

**原文链接**: [https://www.mixfont.com/experiments/decoy-font](https://www.mixfont.com/experiments/decoy-font)

生成摘要时出错

---

## 9. Guerrilla London bus ads mock Kylie Jenner’s Meta glasses campaign

**原文标题**: Guerrilla London bus ads mock Kylie Jenner’s Meta glasses campaign

**原文链接**: [https://hyperallergic.com/guerrilla-london-bus-ads-mock-kylie-jenners-meta-glasses-campaign/](https://hyperallergic.com/guerrilla-london-bus-ads-mock-kylie-jenners-meta-glasses-campaign/)

生成摘要时出错

---

## 10. My midlife crisis Corolla is fast, furious, and modded

**原文标题**: My midlife crisis Corolla is fast, furious, and modded

**原文链接**: [https://www.zocalopublicsquare.org/my-midlife-crisis-corolla-fast-furious-fully-modded/](https://www.zocalopublicsquare.org/my-midlife-crisis-corolla-fast-furious-fully-modded/)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 2 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 3 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 4 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 5 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 6 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 7 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 8 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 9 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 10 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 11 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 12 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 13 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 14 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 15 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 16 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 17 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 18 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 19 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 20 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 21 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 22 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 23 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 24 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 25 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 26 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 27 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 28 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 29 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 30 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 31 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 32 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 33 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 34 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 35 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 36 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 37 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 38 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 39 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 40 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 41 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 42 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 43 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 44 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 45 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 46 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 47 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 48 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 49 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 50 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 51 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 52 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 53 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 54 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 55 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 56 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 57 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 58 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 59 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 60 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 61 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 62 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 63 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 64 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 65 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 66 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 67 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 68 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 69 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 70 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 71 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 72 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 73 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 74 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 75 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 76 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 77 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 78 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 79 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 80 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 81 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 82 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 83 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 84 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 85 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 86 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 87 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 88 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 89 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 90 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 91 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 92 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 93 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 94 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 95 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 96 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 97 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 98 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 99 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 100 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 101 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 102 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 103 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 104 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 105 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 106 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 107 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 108 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 109 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 110 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 111 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 112 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 113 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 114 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 115 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 116 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 117 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 118 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 119 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 120 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 121 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 122 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 123 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 124 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 125 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 126 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 127 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 128 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 129 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 130 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 131 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 132 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 133 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 134 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 135 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 136 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 137 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 138 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 139 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 140 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 141 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 142 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 143 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 144 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 145 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 146 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 147 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 148 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 149 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 150 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 151 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 152 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 153 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 154 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 155 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 156 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 157 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 158 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 159 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 160 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 161 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 162 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 163 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 164 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 165 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 166 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 167 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 168 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 169 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 170 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 171 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 172 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 173 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 174 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 175 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 176 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 177 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 178 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 179 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 180 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 181 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 182 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 183 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 184 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 185 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 186 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 187 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 188 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 189 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 190 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 191 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 192 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 193 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 194 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 195 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 196 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 197 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 198 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 199 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 200 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 201 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 202 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 203 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 204 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 205 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 206 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 207 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 208 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 209 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 210 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 211 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 212 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 213 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 214 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 215 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 216 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 217 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 218 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 219 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 220 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 221 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 222 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 223 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 224 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 225 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 226 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 227 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 228 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 229 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 230 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 231 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 232 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 233 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 234 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 235 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 236 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 237 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 238 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 239 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 240 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 241 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 242 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 243 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 244 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 245 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 246 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 247 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 248 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 249 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 250 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 251 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
