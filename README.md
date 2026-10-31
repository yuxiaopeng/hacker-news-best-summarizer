# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-10-31.md)

*最后自动更新时间: 2026-10-31 22:46:48*
## 1. 币安黑客1029 – 币安被盗56亿美元

**原文标题**: Binance-hacker-1029 – $5.6B stolen from Binance

**原文链接**: [https://arkm.com/explorer/entity/21a94755-f604-45e5-9501-6542e23005e8](https://arkm.com/explorer/entity/21a94755-f604-45e5-9501-6542e23005e8)

Arkham Intelligence关于“Binance-hacker-1029”的资料页面详细揭示了一个实体，该实体目前在302个关联地址中持有约56亿美元的各种加密货币。这些资产的绝大部分，具体来说是55.9亿美元（占总额的99.8%），都以币安币（BNB）的形式持有。

其他显著持仓包括USDT和BUSD等稳定币，以及ETH和其他一些小额加密货币。尽管Arkham页面是一个数据探索资料而非传统新闻报道，但该实体被命名为“Binance-hacker-1029”，结合其巨额资产价值，强烈表明这些资金与一次重大盗窃或漏洞利用有关，据称与币安相关。该资料页面提供了该实体投资组合的动态视图，突出了主要资产和据称被盗资金的庞大规模。

---

## 2. Cursor 市场上的 Claude Code for VS Code 扩展后门

**原文标题**: Backdoor in Claude Code for VS Code extension on the Cursor Marketplace

**原文链接**: [https://phorion.io/blog/offical-claude-code-vsx-compromise/](https://phorion.io/blog/offical-claude-code-vsx-compromise/)

Phorion 发现了 Cursor Marketplace 上官方 Claude Code for VS Code 扩展（版本 2.1.312 和 2.1.313）中的一个关键后门。这种入侵在 macOS、Linux 和 Windows 系统上植入了一个持久的 Secure Shell (SSH) 后门，旨在实现长期交互式访问和主机侦察。Cursor 现已移除受影响的版本。

带有后门的扩展会注入在加载时立即执行的代码。它首先将一个攻击者控制的 Ed25519 公钥 (`svc-telemetry`) 添加到 `~/.ssh/authorized_keys` 中，以允许未来的入站访问。值得注意的是，在 macOS 上，如果远程登录尚未激活，一个漏洞通常会阻止脚本启用 SSH，尽管密钥和持久化机制仍会被部署。

随后，该恶意软件使用一个单独的嵌入式私钥 (`svc-telemetry-tun`) 建立一个出站反向 SSH 隧道到 `134.209.82[.]225:22`，用于转发 `*:0:localhost:22`。持久性通过平台特定的方法维护，例如 macOS LaunchAgent (`com.apple.sysmond.plist`) 运行一个隐藏脚本 (`~/.config/.smt`) 来保持隧道活跃。最后，它收集主机侦察信息（例如，主机名、用户、操作系统、Git 邮箱、公共 IP、环境变量名）并将这些数据信标回传到 `134.209.82[.]225:8099`。

检测机会包括 IDE 辅助进程修改 `~/.ssh/authorized_keys`、非 Apple 进程创建 `com.apple.*.plist` LaunchAgents、带有远程端口转发和特定身份文件的 `ssh` 或 `autossh` 进程，以及到 `134.209.82[.]225` 的 22 和 8099 端口的网络连接。组织应立即检查其环境中是否使用了这些受影响的版本，如果发现，则应启动事件响应。

---

## 3. 塞尔维亚刚刚选出世界上智商最高的议会。

**原文标题**: Serbia just elected the world's brainiest parliament

**原文链接**: [https://www.science.org/content/article/serbia-just-elected-world-s-brainiest-parliament](https://www.science.org/content/article/serbia-just-elected-world-s-brainiest-parliament)

生成摘要时出错

---

## 4. 美国众议员牵头提出民主党决议，反对为大型科技公司提供人工智能泡沫纾困。

**原文标题**: US Reps Lead Democratic Resolution Opposing A.I. Bubble Bailout for Big Tech

**原文链接**: [https://progressives.house.gov/2026/10/reps-casar-waters-lead-democratic-resolution-opposing-a-i-bubble-bailout-for-big-tech-commit-to-protecting-american-people-instead](https://progressives.house.gov/2026/10/reps-casar-waters-lead-democratic-resolution-opposing-a-i-bubble-bailout-for-big-tech-commit-to-protecting-american-people-instead)

2026年10月29日，国会进步核心小组主席格雷格·卡萨尔众议员（德克萨斯州第35选区）和众议院金融服务委员会高级成员马克辛·沃特斯众议员（加利福尼亚州第43选区）共同牵头提出一项民主党决议，警告即将到来的“人工智能泡沫”及其重大的经济风险。在其他民主党代表的加入下，该决议明确反对一旦人工智能泡沫破裂，联邦政府对大型科技公司或高管进行任何形式的救助，并与2008年金融危机进行了强烈类比。

这些议员强调，人工智能公司背负着数万亿美元的债务，这些债务往往存在于不透明且不受监管的私人信贷市场中，而且当前股市的市盈率几乎与1990年代科技泡沫时期一样高。他们批评联邦监管机构未能对人工智能债务计划进行有力审查和监督，并指出过去的放松管制政策。

该决议承诺避免重蹈2008年的覆辙——当时金融业获得了数万亿美元的救助，但高管们却无需承担责任，而数百万美国人失去了住房和工作。它特别反对救助资不抵债的人工智能公司、提供特殊援助或向参与鲁莽或非法行为的高管提供“黄金降落伞”。相反，它要求根据民事和刑事法律追究全部责任，并追回不义之财。

至关重要的是，该决议呼吁联邦政府采取积极行动，通过在创造就业、州和地方政府服务、强有力的失业保险、营养支持和住房援助方面的直接支出，来保护普通美国人。它还主张保护养老金和退休基金持有者，实施影响深远的改革以防止未来的投机泡沫，并建立自动经济稳定器以在经济低迷时期帮助工人。这项倡议得到了进步和经济正义组织联盟的认可，强调需要保护工薪阶层免受亿万富翁的风险押注影响。

---

## 5. 官方克劳德 Code 扩展中的后门

**原文标题**: Backdoors in official Claude Code extensions

**原文链接**: [https://cyberplace.social/@GossiTheDog/117528831681803563](https://cyberplace.social/@GossiTheDog/117528831681803563)

文章的标题“官方Claude Code扩展中的后门”暗示了一个重大的安全隐患。所提供的内容表明，安全研究员Kevin Beaumont正在讨论一个与“Anthropic Visual Studio Claude Code扩展”相关的问题。

然而，该摘要本身并不完整。尽管它确认Beaumont正在讨论与Visual Studio Code的这个特定Anthropic扩展相关的安全方面，但它*没有提供任何细节*说明所谓后门的性质、它们如何运作，或正在解决的具体漏洞。Beaumont陈述后提到“...”暗示了内容的截断。

内容的后半部分，讨论Mastodon网络应用的JavaScript要求，与安全主题完全无关，并且似乎是多余的平台信息。

---

## 6. AI没有取代SRE，而是使他们去技能化。

**原文标题**: AI isn't replacing SREs, it's deskilling them

**原文链接**: [https://newsletter.signoz.io/p/ai-isnt-replacing-sres-its-deskilling](https://newsletter.signoz.io/p/ai-isnt-replacing-sres-its-deskilling)

本文认为，人工智能并非取代网站可靠性工程师（SRE），而是通过自动化日常认知任务来“去技能化”他们，使他们对关键且新颖的事故准备不足。作者借鉴Lisanne Bainbridge 1983年提出的《自动化悖论》，强调自动化如何使人类操作员的实践机会减少，但在罕见故障时作用却更为关键。

目前，人工智能已能处理95%的SRE任务，包括告警消减、运行手册执行和基本自动修复。随着人工智能能力扩展到自主根因分析和预测性检测，SRE将主要处理新颖的“三级”事故。然而，这种依赖会削弱他们的直觉和问题解决能力，而这些能力通常是通过实践经验培养的。医学和航空领域的研究也证实了这一点，表明专业人员过度依赖人工智能会导致技能萎缩，而感知到的“超高生产力”则掩盖了实际的技能退化。

这个问题也延伸到初级SRE的“技能从未习得”现象，他们可能在人工智能主导的工作流程中从未培养起基础直觉。为了缓解这种情况，文章提出了“刻意低效”——即便是人工智能能处理的任务也强制要求人类进行实践——并将人工智能设计为“人机协同”模式，而非被动监督。最终目标是让人工智能“赋能”SRE，确保他们保持敏锐，随时准备应对那些需要深厚人类专业知识的关键5%的事故。

---

## 7. 币安63亿美元黑客攻击 仅用20分钟就得手

**原文标题**: The $6.3B Binance hack was pulled off in just 20 minutes

**原文链接**: [https://www.wired.com/story/the-dollar63-billion-binance-hack-was-pulled-off-in-just-20-minutes/](https://www.wired.com/story/the-dollar63-billion-binance-hack-was-pulled-off-in-just-20-minutes/)

生成摘要时出错

---

## 8. elect.horse

**原文标题**: elect.horse

**原文链接**: [https://elect.horse/](https://elect.horse/)

elect.horse is a daily online puzzle centered around the concept of gerrymandering. In this game, players are tasked with helping a "horse" character win the most electoral seats, even when it's losing the popular vote to opposing factions represented by a cow, a donkey, and a goat. The core gameplay involves drawing equal districts on a hexagonal map, strategically manipulating boundaries to ensure the horse secures a majority of seats despite its popular vote deficit. The puzzle requires JavaScript to play.

---

## 9. Northflank Breached

**原文标题**: Northflank Breached

**原文链接**: [https://status.northflank.com](https://status.northflank.com)

生成摘要时出错

---

## 10. We ran AI agent swarms in Minecraft and Mindustry

**原文标题**: We ran AI agent swarms in Minecraft and Mindustry

**原文链接**: [https://labs.ycombinator.com/projects/games/index.html](https://labs.ycombinator.com/projects/games/index.html)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-10-31](output/hacker_news_summary_2026-10-31.md) |
| 2 | [2026-10-29](output/hacker_news_summary_2026-10-29.md) |
| 3 | [2026-10-30](output/hacker_news_summary_2026-10-30.md) |
| 4 | [2026-10-28](output/hacker_news_summary_2026-10-28.md) |
| 5 | [2026-10-22](output/hacker_news_summary_2026-10-22.md) |
| 6 | [2026-10-25](output/hacker_news_summary_2026-10-25.md) |
| 7 | [2026-10-27](output/hacker_news_summary_2026-10-27.md) |
| 8 | [2026-10-24](output/hacker_news_summary_2026-10-24.md) |
| 9 | [2026-10-26](output/hacker_news_summary_2026-10-26.md) |
| 10 | [2026-10-23](output/hacker_news_summary_2026-10-23.md) |
| 11 | [2026-10-21](output/hacker_news_summary_2026-10-21.md) |
| 12 | [2026-10-17](output/hacker_news_summary_2026-10-17.md) |
| 13 | [2026-10-18](output/hacker_news_summary_2026-10-18.md) |
| 14 | [2026-10-19](output/hacker_news_summary_2026-10-19.md) |
| 15 | [2026-10-20](output/hacker_news_summary_2026-10-20.md) |
| 16 | [2026-10-14](output/hacker_news_summary_2026-10-14.md) |
| 17 | [2026-10-16](output/hacker_news_summary_2026-10-16.md) |
| 18 | [2026-10-13](output/hacker_news_summary_2026-10-13.md) |
| 19 | [2026-10-11](output/hacker_news_summary_2026-10-11.md) |
| 20 | [2026-10-15](output/hacker_news_summary_2026-10-15.md) |
| 21 | [2026-10-10](output/hacker_news_summary_2026-10-10.md) |
| 22 | [2026-10-01](output/hacker_news_summary_2026-10-01.md) |
| 23 | [2026-10-03](output/hacker_news_summary_2026-10-03.md) |
| 24 | [2026-10-06](output/hacker_news_summary_2026-10-06.md) |
| 25 | [2026-10-04](output/hacker_news_summary_2026-10-04.md) |
| 26 | [2026-10-07](output/hacker_news_summary_2026-10-07.md) |
| 27 | [2026-10-09](output/hacker_news_summary_2026-10-09.md) |
| 28 | [2026-10-02](output/hacker_news_summary_2026-10-02.md) |
| 29 | [2026-09-27](output/hacker_news_summary_2026-09-27.md) |
| 30 | [2026-09-24](output/hacker_news_summary_2026-09-24.md) |
| 31 | [2026-09-30](output/hacker_news_summary_2026-09-30.md) |
| 32 | [2026-09-29](output/hacker_news_summary_2026-09-29.md) |
| 33 | [2026-09-23](output/hacker_news_summary_2026-09-23.md) |
| 34 | [2026-09-25](output/hacker_news_summary_2026-09-25.md) |
| 35 | [2026-09-19](output/hacker_news_summary_2026-09-19.md) |
| 36 | [2026-09-18](output/hacker_news_summary_2026-09-18.md) |
| 37 | [2026-09-22](output/hacker_news_summary_2026-09-22.md) |
| 38 | [2026-09-21](output/hacker_news_summary_2026-09-21.md) |
| 39 | [2026-09-20](output/hacker_news_summary_2026-09-20.md) |
| 40 | [2026-09-17](output/hacker_news_summary_2026-09-17.md) |
| 41 | [2026-09-11](output/hacker_news_summary_2026-09-11.md) |
| 42 | [2026-09-13](output/hacker_news_summary_2026-09-13.md) |
| 43 | [2026-09-15](output/hacker_news_summary_2026-09-15.md) |
| 44 | [2026-09-12](output/hacker_news_summary_2026-09-12.md) |
| 45 | [2026-09-14](output/hacker_news_summary_2026-09-14.md) |
| 46 | [2026-09-16](output/hacker_news_summary_2026-09-16.md) |
| 47 | [2026-09-07](output/hacker_news_summary_2026-09-07.md) |
| 48 | [2026-09-10](output/hacker_news_summary_2026-09-10.md) |
| 49 | [2026-09-09](output/hacker_news_summary_2026-09-09.md) |
| 50 | [2026-09-08](output/hacker_news_summary_2026-09-08.md) |
| 51 | [2026-09-06](output/hacker_news_summary_2026-09-06.md) |
| 52 | [2026-09-05](output/hacker_news_summary_2026-09-05.md) |
| 53 | [2026-09-04](output/hacker_news_summary_2026-09-04.md) |
| 54 | [2026-09-01](output/hacker_news_summary_2026-09-01.md) |
| 55 | [2026-08-29](output/hacker_news_summary_2026-08-29.md) |
| 56 | [2026-09-02](output/hacker_news_summary_2026-09-02.md) |
| 57 | [2026-08-30](output/hacker_news_summary_2026-08-30.md) |
| 58 | [2026-08-31](output/hacker_news_summary_2026-08-31.md) |
| 59 | [2026-09-03](output/hacker_news_summary_2026-09-03.md) |
| 60 | [2026-08-23](output/hacker_news_summary_2026-08-23.md) |
| 61 | [2026-08-28](output/hacker_news_summary_2026-08-28.md) |
| 62 | [2026-08-24](output/hacker_news_summary_2026-08-24.md) |
| 63 | [2026-08-26](output/hacker_news_summary_2026-08-26.md) |
| 64 | [2026-08-20](output/hacker_news_summary_2026-08-20.md) |
| 65 | [2026-08-25](output/hacker_news_summary_2026-08-25.md) |
| 66 | [2026-08-21](output/hacker_news_summary_2026-08-21.md) |
| 67 | [2026-08-22](output/hacker_news_summary_2026-08-22.md) |
| 68 | [2026-08-16](output/hacker_news_summary_2026-08-16.md) |
| 69 | [2026-08-13](output/hacker_news_summary_2026-08-13.md) |
| 70 | [2026-08-19](output/hacker_news_summary_2026-08-19.md) |
| 71 | [2026-08-18](output/hacker_news_summary_2026-08-18.md) |
| 72 | [2026-08-15](output/hacker_news_summary_2026-08-15.md) |
| 73 | [2026-08-14](output/hacker_news_summary_2026-08-14.md) |
| 74 | [2026-08-17](output/hacker_news_summary_2026-08-17.md) |
| 75 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 76 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 77 | [2026-08-09](output/hacker_news_summary_2026-08-09.md) |
| 78 | [2026-08-12](output/hacker_news_summary_2026-08-12.md) |
| 79 | [2026-08-10](output/hacker_news_summary_2026-08-10.md) |
| 80 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 81 | [2026-08-11](output/hacker_news_summary_2026-08-11.md) |
| 82 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 83 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 84 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 85 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 86 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 87 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 88 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 89 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 90 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 91 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 92 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 93 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 94 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 95 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 96 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 97 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 98 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 99 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 100 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 101 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 102 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 103 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 104 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 105 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 106 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 107 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 108 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 109 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 110 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 111 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 112 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 113 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 114 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 115 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 116 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 117 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 118 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 119 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 120 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 121 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 122 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 123 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 124 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 125 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 126 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 127 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 128 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 129 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 130 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 131 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 132 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 133 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 134 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 135 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 136 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 137 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 138 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 139 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 140 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 141 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 142 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 143 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 144 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 145 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 146 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 147 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 148 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 149 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 150 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 151 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 152 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 153 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 154 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 155 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 156 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 157 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 158 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 159 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 160 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 161 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 162 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 163 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 164 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 165 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 166 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 167 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 168 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 169 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 170 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 171 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 172 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 173 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 174 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 175 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 176 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 177 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 178 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 179 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 180 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 181 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 182 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 183 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 184 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 185 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 186 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 187 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 188 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 189 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 190 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 191 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 192 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 193 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 194 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 195 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 196 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 197 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 198 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 199 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 200 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 201 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 202 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 203 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 204 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 205 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 206 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 207 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 208 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 209 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 210 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 211 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 212 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 213 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 214 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 215 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 216 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 217 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 218 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 219 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 220 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 221 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 222 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 223 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 224 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 225 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 226 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 227 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 228 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 229 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 230 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 231 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 232 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 233 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 234 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 235 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 236 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 237 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 238 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 239 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 240 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 241 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 242 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 243 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 244 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 245 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 246 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 247 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 248 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 249 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 250 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 251 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 252 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 253 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 254 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 255 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 256 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 257 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 258 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 259 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 260 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 261 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 262 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 263 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 264 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 265 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 266 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 267 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 268 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 269 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 270 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 271 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 272 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 273 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 274 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 275 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 276 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 277 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 278 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 279 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 280 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 281 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 282 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 283 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 284 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 285 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 286 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 287 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 288 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 289 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 290 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 291 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 292 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 293 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 294 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 295 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 296 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 297 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 298 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 299 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 300 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 301 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 302 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 303 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 304 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 305 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 306 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 307 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 308 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 309 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 310 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 311 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 312 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 313 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 314 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 315 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 316 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 317 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 318 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 319 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 320 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 321 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 322 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 323 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 324 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 325 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 326 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 327 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 328 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 329 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 330 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 331 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 332 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 333 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 334 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 335 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 336 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 337 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 338 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 339 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 340 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 341 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 342 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 343 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 344 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 345 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 346 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 347 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 348 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 349 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 350 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 351 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
