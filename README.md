# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-02-26.md)

*最后自动更新时间: 2026-02-26 20:12:13*
## 1. 谷歌 API 密钥原本不是秘密，但 Gemini 改变了规则

**原文标题**: Google API keys weren't secrets, but then Gemini changed the rules

**原文链接**: [https://trufflesecurity.com/blog/google-api-keys-werent-secrets-but-then-gemini-changed-the-rules](https://trufflesecurity.com/blog/google-api-keys-werent-secrets-but-then-gemini-changed-the-rules)

Truffle Security 发现了一个重大漏洞：过去被认为可以安全地公开嵌入在地图和 Firebase 等服务中的 Google API 密钥，现在却能提供对 Gemini AI API 的敏感访问。十多年来，Google 一直告知开发者，这些密钥并非秘密，主要作为项目标识符用于计费，且功能受限。

然而，当 Google Cloud 项目中启用了 Gemini API（即生成式语言 API）时，该项目内现有的 API 密钥，即使是那些已公开暴露的，也会悄无声息地获得对 Gemini 端点的完全访问权限。这种“追溯性权限扩展”意味着一个旧的、公开的地图密钥可能突然变成访问上传文件、缓存数据并产生巨额 AI 计费的凭据。新的 API 密钥也默认为“无限制”，一旦启用，它们会立即对 Gemini 生效。

Truffle Security 扫描了数百万个网站，发现了 2,863 个此类易受攻击的 Google API 密钥，其中一些甚至被 Google 自己使用。攻击者可以轻易地从公共网页抓取这些密钥，无需触及受害者的基础设施，即可访问私人数据或耗尽配额。

Google 最初驳回了该报告，但在收到包括来自 Google 自身基础设施的示例在内的具体证据后，将其重新归类为 bug。Google 现在正在实施变革，例如为新密钥设置作用域默认值、阻止泄露的密钥以及主动发送通知，以解决此问题。建议用户检查其 GCP 项目是否启用了生成式语言 API，审计密钥是否存在无限制或 Gemini 访问权限，验证此类密钥是否未公开，并立即轮换任何已暴露的凭据。

---

## 2. 丹麦政府机构将弃用微软软件 (2025)

**原文标题**: Danish government agency to ditch Microsoft software (2025)

**原文链接**: [https://therecord.media/denmark-digital-agency-microsoft-digital-independence](https://therecord.media/denmark-digital-agency-microsoft-digital-independence)

丹麦数字化部计划用包括LibreOffice在内的开源软件替代微软软件，以实现数字独立并减少对美国科技公司的依赖。丹麦数字化大臣卡罗琳·施塔格·奥尔森证实，该部一半以上的员工将于下月从Microsoft Office转向LibreOffice，预计年底前完成全面过渡。此举也旨在避免管理将于10月失去官方支持的过时Windows 10系统所产生的费用。

这一决定是出于对“数字主权”的追求、成本考量、微软的市场主导地位以及过去与华盛顿在数据保护方面的政治紧张关系。虽然如果过渡过于复杂，该部可能会恢复原状，但这一转变与丹麦最大城市哥本哈根和奥胡斯的类似计划不谋而合。这也反映了更广泛的欧洲趋势，德国石勒苏益格-荷尔斯泰因州同样正在转向LibreOffice和Open-Xchange，并计划迁移到Linux操作系统，以建立一个“数字主权IT工作场所”。

---

## 3. Never buy a .online domain

**原文标题**: Never buy a .online domain

**原文链接**: [https://www.0xsid.com/blog/online-tld-is-pain](https://www.0xsid.com/blog/online-tld-is-pain)

生成摘要时出错

---

## 4. HN上的新用户更可能使用破折号。

**原文标题**: New accounts on HN more likely to use em-dashes

**原文链接**: [https://www.marginalia.nu/weird-ai-crap/hn/](https://www.marginalia.nu/weird-ai-crap/hn/)

作者对近期Hacker News (HN) 上机器人数量激增表示担忧，并指出评论明显出现异常以及讨论质量普遍下降，表现为平庸或离题的言论。

为了调查，他们分别从`/newcomments`（最新评论）和`/noobcomments`（新注册账户的最新评论）中抓取了大约700条评论。分析揭示了两个重要发现：

1.  **符号使用：** 新注册账户的评论使用破折号、箭头及其他符号的可能性高出近10倍（在评论中占比17.47% 对 1.83%；p = 7e-20）。
2.  **提及AI/LLM：** 新账户提及AI和LLM的可能性也更高（在评论中占比18.67% 对 11.8%；p = 0.0018）。

尽管样本量适中，作者仍强调这些是“相当大的差异”，尤其是符号使用率高出10倍这一点，他们认为这难以用合法的真人用户行为来解释，并将其解读为机器人活动增加的有力证据。

---

## 5. 安特罗匹克放弃旗舰安全承诺

**原文标题**: Anthropic Drops Flagship Safety Pledge

**原文链接**: [https://time.com/7380854/exclusive-anthropic-drops-flagship-safety-pledge/](https://time.com/7380854/exclusive-anthropic-drops-flagship-safety-pledge/)

Anthropic, an AI company that positioned itself as the most safety-conscious, has dropped a central pledge from its 2023 Responsible Scaling Policy (RSP). Previously, Anthropic committed to never training an AI system without guaranteeing adequate safety measures in advance, a promise touted as resisting market pressures.

The revamped RSP eliminates this "guarantee in advance" stipulation. Instead, Anthropic now pledges greater transparency on AI risks, aims to match or exceed competitors' safety efforts, and will only "delay" AI development if it's both leading the AI race and believes catastrophic risks are significant.

Chief Science Officer Jared Kaplan explained the shift, citing the lack of similar commitments from rivals, the failure of national/international regulations to materialize, and the increasing complexity of AI safety evaluations. He stressed that stopping development while competitors advanced would render Anthropic irrelevant for safety research. The company argues that to understand and mitigate frontier risks, it must build frontier models.

This policy change coincides with Anthropic's recent commercial and technological successes, including a $30 billion investment. While Kaplan denies capitulating to market incentives, framing it as a pragmatic response to emerging realities, critics like Chris Painter of METR view it as a "bearish signal" that society is unprepared for potential AI catastrophes, warning of a "frog-boiling" effect without clear safety thresholds.

Anthropic maintains the new policy reinforces its commitment to safety by promising regular "Frontier Safety Roadmaps" and "Risk Reports" to drive transparency and prioritize safety research.

---

## 6. 亚马逊被控普遍哄抬物价，波及整个经济。

**原文标题**: Amazon accused of widespread scheme to inflate prices across the economy

**原文链接**: [https://www.thebignewsletter.com/p/amazon-busted-for-widespread-price](https://www.thebignewsletter.com/p/amazon-busted-for-widespread-price)

由联邦贸易委员会（FTC）和17个州检察长提起的一项诉讼，指控亚马逊实施一项旨在在整个经济领域内普遍抬高物价的计划，损害了消费者和竞争企业双方的利益。诉状声称，亚马逊利用其垄断权力，强迫第三方卖家签订反竞争协议，阻止他们在竞争性电商平台上提供更低的价格。

一项关键指控集中在亚马逊的“公平定价政策”上，诉讼称其为一项欺骗性的价格均等条款。根据这项政策，亚马逊据称会惩罚那些在沃尔玛或eBay等竞争网站上以更低价格列出商品的卖家。惩罚包括降低商品可见度、移除备受追捧的“购买按钮”，甚至完全下架商品，从而有效切断卖家与亚马逊庞大客户群的联系。这种压力迫使卖家在其他平台上提高价格，以避免亚马逊的制裁，导致整个互联网上的价格被人为抬高。

诉讼进一步详细说明了亚马逊如何利用算法检测其他地方的更低价格，并随后提高自身价格，有时在热门商品上涨幅高达16%。FTC认为这些做法扼杀竞争、抑制创新，并每年从消费者那里攫取数十亿美元。这项法律行动旨在制止亚马逊涉嫌的反竞争行为，处以金钱罚款，并可能强制进行结构性改革，以恢复电商市场的竞争。

---

## 7. 吉米·亨德里克斯是一名系统工程师

**原文标题**: Jimi Hendrix was a systems engineer

**原文链接**: [https://spectrum.ieee.org/jimi-hendrix-systems-engineer](https://spectrum.ieee.org/jimi-hendrix-systems-engineer)

在《DIY动手杂志》的一篇文章中，边缘计算架构师Rohan S. Puranik提出，吉米·亨德里克斯（Jimi Hendrix）实际上是一名系统工程师。Puranik认为，亨德里克斯通过一系列组件精确控制了声音调制和反馈回路。他“工程学”的一个关键方面在于通过策略性地调整吉他相对于放大器扬声器的位置来操纵反馈。

---

## 8. Mac mini will be made at a new facility in Houston

**原文标题**: Mac mini will be made at a new facility in Houston

**原文链接**: [https://www.apple.com/newsroom/2026/02/apple-accelerates-us-manufacturing-with-mac-mini-production/](https://www.apple.com/newsroom/2026/02/apple-accelerates-us-manufacturing-with-mac-mini-production/)

生成摘要时出错

---

## 9. Pi — 极简终端编程套件

**原文标题**: Pi – A minimal terminal coding harness

**原文链接**: [https://pi.dev](https://pi.dev)

Pi 是一个极简的终端编码框架，旨在实现最大程度的适应性和可扩展性。它不强制规定工作流程，而是提供一个灵活的核心，用户可以使用 TypeScript 扩展、技能、提示模板和主题进行扩展，所有这些都可以作为 npm 或 Git 包共享。

它支持超过 15 个 AI 提供商和数百种模型（例如 Anthropic、OpenAI、Google），并允许在会话中途切换模型。Pi 具有树状结构、可共享的会话历史记录，支持导航、分支、导出为 HTML 或作为 GitHub gist 共享。它对上下文工程的重视，通过 `AGENTS.md`、`SYSTEM.md` 和可自定义的压缩功能，提供了对提示和上下文窗口的精确控制。

Pi 以四种模式运行：交互式 TUI、用于脚本的打印/JSON、用于非 Node 集成的 RPC 和用于嵌入的 SDK。它的理念是提供“原语，而非功能”；其他代理中常见的功能——例如子代理、计划模式或权限门控——都留给用户通过扩展自行构建，或从社区包中安装。这种方法确保了核心的极简性，同时允许用户根据自身特定需求完全塑造 Pi。社区互动通过 GitHub、Discord 和全面的文档进行。

---

## 10. Anthropic ditches its core safety promise

**原文标题**: Anthropic ditches its core safety promise

**原文链接**: [https://www.cnn.com/2026/02/25/tech/anthropic-safety-policy-change](https://www.cnn.com/2026/02/25/tech/anthropic-safety-policy-change)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 2 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 3 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 4 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 5 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 6 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 7 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 8 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 9 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 10 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 11 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 12 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 13 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 14 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 15 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 16 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 17 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 18 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 19 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 20 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 21 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 22 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 23 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 24 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 25 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 26 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 27 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 28 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 29 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 30 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 31 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 32 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 33 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 34 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 35 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 36 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 37 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 38 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 39 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 40 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 41 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 42 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 43 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 44 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 45 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 46 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 47 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 48 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 49 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 50 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 51 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 52 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 53 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 54 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 55 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 56 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 57 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 58 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 59 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 60 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 61 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 62 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 63 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 64 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 65 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 66 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 67 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 68 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 69 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 70 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 71 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 72 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 73 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 74 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 75 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 76 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 77 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 78 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 79 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 80 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 81 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 82 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 83 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 84 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 85 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 86 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 87 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 88 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 89 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 90 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 91 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 92 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 93 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 94 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 95 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 96 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 97 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 98 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 99 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 100 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 101 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 102 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 103 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 104 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 105 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 106 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 107 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 108 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
| 109 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 110 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 111 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 112 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
