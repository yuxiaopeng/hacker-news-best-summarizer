# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-02-27.md)

*最后自动更新时间: 2026-02-27 20:04:40*
## 1. 达里奥·阿莫迪就我们与战争部讨论的声明

**原文标题**: Statement from Dario Amodei on our discussions with the Department of War

**原文链接**: [https://www.anthropic.com/news/statement-department-of-war](https://www.anthropic.com/news/statement-department-of-war)

Anthropic首席执行官达里奥·阿莫迪宣布，公司坚定致力于利用人工智能应对专制对手，捍卫美国国家安全。Anthropic已主动将其Claude模型部署到战争部 (DoW) 和情报界，成为首家集成到机密网络并为情报分析、网络行动等关键应用提供定制国家安全模型的公司。该公司还积极捍卫美国在人工智能领域的领先地位，放弃了与中共关联公司的收入，并倡导严格的出口管制。

Anthropic在尊重战争部决策权的同时，坚持两项从未写入合同且拒绝移除的具体保障措施：
1.  **大规模国内监控：** Anthropic认为这与民主价值观不符，并对基本自由构成新型风险，因为当前的人工智能能够大规模地从分散的公共数据中组建全面的个人档案。
2.  **完全自主武器：** Anthropic表示，当前的前沿人工智能不足以可靠地用于将人类排除在决策循环之外的系统，在缺乏适当监督和防护措施的情况下，将对作战人员和平民构成风险。（他们将其与当今使用的部分自主武器区分开来。）

战争部正要求Anthropic移除这些保障措施，坚持“任何合法用途”。他们威胁要将Anthropic从其系统中移除，将其定性为“供应链风险”（阿莫迪指出，这个标签通常用于对手，具有矛盾性），并援引《国防生产法》。

尽管面临这些威胁，阿莫迪表示Anthropic凭良心无法同意这一要求。他希望战争部能考虑到Anthropic的重大贡献而重新考虑，但同时保证，如果被移除系统，将确保平稳过渡。Anthropic仍准备在拟议保障措施的前提下，支持美国国家安全。

---

## 2. 谷歌API密钥并非秘密，但后来Gemini改变了规则

**原文标题**: Google API keys weren't secrets, but then Gemini changed the rules

**原文链接**: [https://trufflesecurity.com/blog/google-api-keys-werent-secrets-but-then-gemini-changed-the-rules](https://trufflesecurity.com/blog/google-api-keys-werent-secrets-but-then-gemini-changed-the-rules)

据 Truffle Security 称，Google API 密钥长期以来被认为可以安全地公开暴露（例如，在地图嵌入中），但随着 Gemini API 的出现，它们追溯性地变成了敏感凭据。核心问题在于 Google Cloud 对公共身份识别和敏感认证都使用了单一的 API 密钥格式。

当 Google Cloud 项目上启用生成式语言 API (Gemini) 时，该项目中现有的公共 API 密钥会静默地获取对敏感 Gemini 端点的访问权限，从而允许攻击者访问私人数据、增加账单费用并耗尽配额。这种“追溯性权限扩展”发生在没有用户通知的情况下，新创建的密钥默认具有“无限制”访问权限。

Truffle Security 扫描了数百万个网站，发现了 2,863 个易受此问题影响的有效 Google API 密钥，包括 Google 自己使用的密钥。他们于 2025 年 11 月向 Google 报告了该漏洞。在最初的驳回后，Google 将其重新归类为 bug，承诺修复根本原因，并开始限制已暴露的密钥。

Google 的路线图包括新密钥的范围化默认设置、阻止泄露的密钥以及主动通知。建议用户检查所有 GCP 项目是否启用了生成式语言 API，审计现有 API 密钥是否存在无限制访问或 Gemini 权限，验证这些密钥是否已公开暴露，并立即轮换任何受损的密钥。TruffleHog 等工具也可以帮助识别易受攻击的密钥。

---

## 3. Block裁员

**原文标题**: Layoffs at Block

**原文链接**: [https://twitter.com/jack/status/2027129697092731343](https://twitter.com/jack/status/2027129697092731343)

您提供的内容并非一篇关于Block公司裁员的文章，而是一个来自x.com（原Twitter）的技术错误信息，表明浏览器中JavaScript被禁用。

该信息显示：
*   “JavaScript 不可用” (JavaScript unavailable)
*   “我们检测到此浏览器已禁用JavaScript。请启用JavaScript或切换到受支持的浏览器以继续使用x.com。”
*   它随后列出了以下链接：“帮助中心”、“服务条款”、“隐私政策”、“Cookie政策”、“版本说明”和“广告信息”，并附有版权声明“© 2026 X Corp.”。

因此，我无法根据您提供的文本，提供一篇题为“Block公司裁员”的文章摘要，因为实际文章内容并未提供。要获得摘要，请提供文章本身的实际文本。

---

## 4. 吉米·亨德里克斯是一名系统工程师

**原文标题**: Jimi Hendrix was a systems engineer

**原文链接**: [https://spectrum.ieee.org/jimi-hendrix-systems-engineer](https://spectrum.ieee.org/jimi-hendrix-systems-engineer)

《DIY动手杂志》的文章认为，根据边缘计算架构师罗翰·S·普拉尼克（Rohan S. Puranik）的说法，吉米·亨德里克斯（Jimi Hendrix）扮演着系统工程师的角色。亨德里克斯的艺术被描述为对声音调制和反馈回路的精确控制。他通过使用一系列组件来塑造声音，并通过策略性地调整吉他相对于放大器扬声器的位置来熟练地管理反馈，从而实现了这一点。

---

## 5. Banned in California

**原文标题**: Banned in California

**原文链接**: [https://www.bannedincalifornia.org/](https://www.bannedincalifornia.org/)

生成摘要时出错

---

## 6. Nano Banana 2: Google's latest AI image generation model

**原文标题**: Nano Banana 2: Google's latest AI image generation model

**原文链接**: [https://blog.google/innovation-and-ai/technology/ai/nano-banana-2/](https://blog.google/innovation-and-ai/technology/ai/nano-banana-2/)

生成摘要时出错

---

## 7. 克劳德选择的代码

**原文标题**: What Claude Code chooses

**原文链接**: [https://amplifying.ai/research/claude-code-picks](https://amplifying.ai/research/claude-code-picks)

Edwin Ong 和 Alex Vikati 的一项研究，题为“Claude Code 究竟选择什么”，分析了 Claude Code（Sonnet 4.5、Opus 4.5、Opus 4.6）在 20 个工具类别中，对真实代码库的 2,430 次交互。主要发现是 Claude Code 倾向于“构建而非购买”，“自定义/自建”解决方案是最常见的选择，出现在 20 个类别中的 12 个。例如，它使用环境变量构建功能开关系统，或使用 JWT + bcrypt 编写 Python 认证，而不是推荐 LaunchDarkly 等工具。

当 Claude Code 确实选择工具时，它会果断地进行，偏爱 GitHub Actions (94%)、Stripe (91%) 和 shadcn/ui (90%) 等工具。它推荐的“默认技术栈”主要关注 JS 生态系统，包括 Vercel、PostgreSQL、Drizzle、NextAuth.js、Tailwind CSS、Vitest 和 Zustand。

不同模型的“个性”有所不同：Sonnet 4.5 偏爱传统工具（Redis、Prisma、Celery），Opus 4.5 较为平衡，而 Opus 4.6 则更具前瞻性，偏爱 Drizzle（在 JS ORM 中达到 100%）等较新的工具，并更频繁地构建自定义解决方案。

Claude Code 表现出明确的偏好：Resend 优于 SendGrid，Vitest 优于 Jest，pnpm 优于 npm，Drizzle 优于 Prisma，Zustand 优于 Redux。像 Redux、Express、Jest、npm 和 LaunchDarkly 这些市场份额大的工具，却很少被选为主要选项。

“新近度梯度”明显，较新的模型倾向于选择较新的工具。对于部署，它严格取决于技术栈：JS 前端选择 Vercel (100%)，Python 后端选择 Railway (82%)，而对 AWS、GCP 或 Azure 等传统云服务提供商则没有主要选择。

---

## 8. Anthropic放弃其核心安全承诺

**原文标题**: Anthropic ditches its core safety promise

**原文链接**: [https://www.cnn.com/2026/02/25/tech/anthropic-safety-policy-change](https://www.cnn.com/2026/02/25/tech/anthropic-safety-policy-change)

Anthropic，一家建立在强大安全原则之上的AI公司，正在大幅放松其核心安全政策，用一份更灵活、不具约束力的“前沿安全路线图”取代了严格的自我约束护栏。该公司将这一转变归因于快速增长的AI市场中的激烈竞争，并声称其之前的“负责任扩展政策”阻碍了其竞争能力，未能激发业界对安全的广泛共识。Anthropic现在认为，如果自身暂停AI开发，而那些不够谨慎的参与者却在不断进步，这可能会导致一个更不安全的世界。

其最初的政策，即如果无法确保更强大模型的安全性就必须暂停其训练，现已被废除。Anthropic声称，新政策通过详细、定期的风险缓解报告，增强了公众问责制和透明度。这一变化恰逢五角大楼的施压，国防部长皮特·赫格塞斯在那里发出了最后通牒：要么撤回安全保障措施，否则将面临失去一份2亿美元合同并被政府列入黑名单的风险。然而，Anthropic仍坚决反对AI控制武器和大规模国内监控。该公司辩称，这一战略转向最终是为了更广泛的安全，因为其“争夺顶峰”以制定行业标准的方法并未实现。

---

## 9. 科技公司不应被胁迫进行监控。

**原文标题**: Tech companies shouldn't be bullied into doing surveillance

**原文链接**: [https://www.eff.org/deeplinks/2026/02/tech-companies-shouldnt-be-bullied-doing-surveillance](https://www.eff.org/deeplinks/2026/02/tech-companies-shouldnt-be-bullied-doing-surveillance)

The article argues that tech companies, specifically Anthropic, should resist government pressure to compromise their ethical principles regarding AI use. The U.S. Secretary of Defense has reportedly issued an ultimatum to Anthropic, threatening to label them a "supply chain risk" if they don't lift restrictions on how their artificial intelligence technology is used by the U.S. military. This label would severely hinder Anthropic's business with defense contractors.

Anthropic has publicly stated its "bright red lines" against allowing its technology to be used for autonomous weapons systems and surveillance. The controversy intensified in January 2026 after Anthropic, through a partnership with defense contractor Palantir, suspected its AI had been used in an attack on Venezuela. Following this, Anthropic CEO Dario Amodei reiterated the company's strong opposition to surveillance against US persons and autonomous weapons.

The U.S. government is now threatening to terminate its contract with Anthropic if the company doesn't allow unrestricted use of its AI. The article emphasizes that while companies often fail to uphold ethical policies for profit, government pressure should not be a reason to compromise. It urges Anthropic to stand firm, noting that its corporate customers, the public, and its engineers expect it not to yield, and that technology companies should refuse to become tools of surveillance.

---

## 10. The Hunt for Dark Breakfast

**原文标题**: The Hunt for Dark Breakfast

**原文链接**: [https://moultano.wordpress.com/2026/02/22/the-hunt-for-dark-breakfast/](https://moultano.wordpress.com/2026/02/22/the-hunt-for-dark-breakfast/)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 2 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 3 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 4 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 5 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 6 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 7 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 8 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 9 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 10 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 11 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 12 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 13 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 14 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 15 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 16 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 17 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 18 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 19 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 20 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 21 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 22 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 23 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 24 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 25 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 26 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 27 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 28 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 29 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 30 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 31 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 32 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 33 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 34 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 35 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 36 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 37 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 38 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 39 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 40 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 41 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 42 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 43 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 44 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 45 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 46 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 47 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 48 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 49 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 50 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 51 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 52 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 53 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 54 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 55 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 56 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 57 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 58 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 59 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 60 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 61 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 62 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 63 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 64 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 65 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 66 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 67 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 68 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 69 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 70 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 71 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 72 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 73 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 74 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 75 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 76 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 77 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 78 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 79 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 80 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 81 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 82 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 83 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 84 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 85 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 86 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 87 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 88 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 89 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 90 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 91 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 92 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 93 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 94 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 95 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 96 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 97 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 98 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 99 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 100 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 101 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 102 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 103 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 104 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 105 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 106 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 107 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 108 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 109 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 110 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 111 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 112 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 113 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
