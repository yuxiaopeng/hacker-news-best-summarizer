# Hacker News 热门文章摘要 (2026-02-27)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

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

## 11. How will OpenAI compete?

**原文标题**: How will OpenAI compete?

**原文链接**: [https://www.ben-evans.com/benedictevans/2026/2/19/how-will-openai-compete-nkg2x](https://www.ben-evans.com/benedictevans/2026/2/19/how-will-openai-compete-nkg2x)

生成摘要时出错

---

## 12. What does " 2>&1 " mean?

**原文标题**: What does " 2>&1 " mean?

**原文链接**: [https://stackoverflow.com/questions/818255/what-does-21-mean](https://stackoverflow.com/questions/818255/what-does-21-mean)

生成摘要时出错

---

## 13. AirSnitch: Demystifying and breaking client isolation in Wi-Fi networks [pdf]

**原文标题**: AirSnitch: Demystifying and breaking client isolation in Wi-Fi networks [pdf]

**原文链接**: [https://www.ndss-symposium.org/wp-content/uploads/2026-f1282-paper.pdf](https://www.ndss-symposium.org/wp-content/uploads/2026-f1282-paper.pdf)

生成摘要时出错

---

## 14. Will vibe coding end like the maker movement?

**原文标题**: Will vibe coding end like the maker movement?

**原文链接**: [https://read.technically.dev/p/vibe-coding-and-the-maker-movement](https://read.technically.dev/p/vibe-coding-and-the-maker-movement)

生成摘要时出错

---

## 15. RAM now represents 35 percent of bill of materials for HP PCs

**原文标题**: RAM now represents 35 percent of bill of materials for HP PCs

**原文链接**: [https://arstechnica.com/gadgets/2026/02/ram-now-represents-35-percent-of-bill-of-materials-for-hp-pcs/](https://arstechnica.com/gadgets/2026/02/ram-now-represents-35-percent-of-bill-of-materials-for-hp-pcs/)

生成摘要时出错

---

## 16. Making MCP cheaper via CLI

**原文标题**: Making MCP cheaper via CLI

**原文链接**: [https://kanyilmaz.me/2026/02/23/cli-vs-mcp.html](https://kanyilmaz.me/2026/02/23/cli-vs-mcp.html)

生成摘要时出错

---

## 17. Show HN: Terminal Phone – E2EE Walkie Talkie from the Command Line

**原文标题**: Show HN: Terminal Phone – E2EE Walkie Talkie from the Command Line

**原文链接**: [https://gitlab.com/here_forawhile/terminalphone](https://gitlab.com/here_forawhile/terminalphone)

生成摘要时出错

---

## 18. Tenth Circuit: 4th Amendment Doesn't Support Broad Search of Protesters' Devices

**原文标题**: Tenth Circuit: 4th Amendment Doesn't Support Broad Search of Protesters' Devices

**原文链接**: [https://www.eff.org/deeplinks/2026/02/victory-tenth-circuit-finds-fourth-amendment-doesnt-support-broad-search-0](https://www.eff.org/deeplinks/2026/02/victory-tenth-circuit-finds-fourth-amendment-doesnt-support-broad-search-0)

生成摘要时出错

---

## 19. First Website (1992)

**原文标题**: First Website (1992)

**原文链接**: [https://info.cern.ch](https://info.cern.ch)

生成摘要时出错

---

## 20. Get free Claude max 20x for open-source maintainers

**原文标题**: Get free Claude max 20x for open-source maintainers

**原文链接**: [https://claude.com/contact-sales/claude-for-oss](https://claude.com/contact-sales/claude-for-oss)

生成摘要时出错

---

## 21. A better streams API is possible for JavaScript

**原文标题**: A better streams API is possible for JavaScript

**原文链接**: [https://blog.cloudflare.com/a-better-web-streams-api/](https://blog.cloudflare.com/a-better-web-streams-api/)

生成摘要时出错

---

## 22. Google workers seek 'red lines' on military A.I., echoing Anthropic

**原文标题**: Google workers seek 'red lines' on military A.I., echoing Anthropic

**原文链接**: [https://www.nytimes.com/2026/02/26/technology/google-deepmind-letter-pentagon.html](https://www.nytimes.com/2026/02/26/technology/google-deepmind-letter-pentagon.html)

生成摘要时出错

---

## 23. Smartphone market forecast to decline this year due to memory shortage

**原文标题**: Smartphone market forecast to decline this year due to memory shortage

**原文链接**: [https://www.idc.com/resource-center/press-releases/wwsmartphoneforecast4q25/](https://www.idc.com/resource-center/press-releases/wwsmartphoneforecast4q25/)

生成摘要时出错

---

## 24. Open Source Endowment – new funding source for open source maintainers

**原文标题**: Open Source Endowment – new funding source for open source maintainers

**原文链接**: [https://endowment.dev/](https://endowment.dev/)

生成摘要时出错

---

## 25. The normalization of corruption in organizations (2003) [pdf]

**原文标题**: The normalization of corruption in organizations (2003) [pdf]

**原文链接**: [https://gwern.net/doc/sociology/2003-ashforth.pdf](https://gwern.net/doc/sociology/2003-ashforth.pdf)

生成摘要时出错

---

## 26. OsmAnd’s Faster Offline Navigation (2025)

**原文标题**: OsmAnd’s Faster Offline Navigation (2025)

**原文链接**: [https://osmand.net/blog/fast-routing/](https://osmand.net/blog/fast-routing/)

生成摘要时出错

---

## 27. BuildKit: Docker's Hidden Gem That Can Build Almost Anything

**原文标题**: BuildKit: Docker's Hidden Gem That Can Build Almost Anything

**原文链接**: [https://tuananh.net/2026/02/25/buildkit-docker-hidden-gem/](https://tuananh.net/2026/02/25/buildkit-docker-hidden-gem/)

生成摘要时出错

---

## 28. The Pentagon is making a mistake by threatening Anthropic

**原文标题**: The Pentagon is making a mistake by threatening Anthropic

**原文链接**: [https://www.understandingai.org/p/the-pentagon-is-making-a-mistake](https://www.understandingai.org/p/the-pentagon-is-making-a-mistake)

生成摘要时出错

---

## 29. In 2025, Meta paid an effective federal tax rate of 3.5%

**原文标题**: In 2025, Meta paid an effective federal tax rate of 3.5%

**原文链接**: [https://bsky.app/profile/rbreich.bsky.social/post/3mfptlfeucn2i](https://bsky.app/profile/rbreich.bsky.social/post/3mfptlfeucn2i)

生成摘要时出错

---

## 30. You Want to Visit the UK? You Better Have a Google Play or App Store Account

**原文标题**: You Want to Visit the UK? You Better Have a Google Play or App Store Account

**原文链接**: [https://www.heltweg.org/posts/you-want-to-visit-the-uk-you-better-have-a-google-play-or-app-store-account/](https://www.heltweg.org/posts/you-want-to-visit-the-uk-you-better-have-a-google-play-or-app-store-account/)

生成摘要时出错

---

## 31. Palm OS User Interface Guidelines (2003) [pdf]

**原文标题**: Palm OS User Interface Guidelines (2003) [pdf]

**原文链接**: [https://cs.uml.edu/~fredm/courses/91.308-spr05/files/palmdocs/uiguidelines.pdf](https://cs.uml.edu/~fredm/courses/91.308-spr05/files/palmdocs/uiguidelines.pdf)

生成摘要时出错

---

## 32. This time is different

**原文标题**: This time is different

**原文链接**: [https://shkspr.mobi/blog/2026/02/this-time-is-different/](https://shkspr.mobi/blog/2026/02/this-time-is-different/)

生成摘要时出错

---

## 33. Jane Street Hit with Terra $40B Insider Trading Suit

**原文标题**: Jane Street Hit with Terra $40B Insider Trading Suit

**原文链接**: [https://www.disruptionbanking.com/2026/02/24/jane-street-hit-with-terra-40b-insider-trading-suit/](https://www.disruptionbanking.com/2026/02/24/jane-street-hit-with-terra-40b-insider-trading-suit/)

生成摘要时出错

---

## 34. A Nationwide Book Ban Bill Has Been Introduced in the House of Representatives

**原文标题**: A Nationwide Book Ban Bill Has Been Introduced in the House of Representatives

**原文链接**: [https://bookriot.com/hr7661-book-ban-legislation/](https://bookriot.com/hr7661-book-ban-legislation/)

生成摘要时出错

---

## 35. I don't know how you get here from “predict the next word”

**原文标题**: I don't know how you get here from “predict the next word”

**原文链接**: [https://www.grumpy-economist.com/p/refine](https://www.grumpy-economist.com/p/refine)

生成摘要时出错

---

## 36. He saw an abandoned trailer, then uncovered a surveillance network

**原文标题**: He saw an abandoned trailer, then uncovered a surveillance network

**原文链接**: [https://calmatters.org/justice/2026/02/alpr-border-patrol-caltrans/](https://calmatters.org/justice/2026/02/alpr-border-patrol-caltrans/)

生成摘要时出错

---

## 37. Twitch: "Hey, come back! This commercial break can't play while you're away."

**原文标题**: Twitch: "Hey, come back! This commercial break can't play while you're away."

**原文链接**: [https://twitter.com/KryDotExe/status/2026806591517856208](https://twitter.com/KryDotExe/status/2026806591517856208)

生成摘要时出错

---

## 38. Breaking Free

**原文标题**: Breaking Free

**原文链接**: [https://www.forbrukerradet.no/breakingfree/](https://www.forbrukerradet.no/breakingfree/)

生成摘要时出错

---

## 39. Netflix Backs Out of Warner Bros. Bidding, Paramount Set to Win

**原文标题**: Netflix Backs Out of Warner Bros. Bidding, Paramount Set to Win

**原文链接**: [https://www.hollywoodreporter.com/business/business-news/netflix-backs-out-warners-deal-paramount-win-1236516763/](https://www.hollywoodreporter.com/business/business-news/netflix-backs-out-warners-deal-paramount-win-1236516763/)

生成摘要时出错

---

## 40. Palantir's AI Is Playing a Major Role in Tracking Gaza Aid Deliveries

**原文标题**: Palantir's AI Is Playing a Major Role in Tracking Gaza Aid Deliveries

**原文链接**: [https://www.dropsitenews.com/p/palantir-ai-gaza-humanitarian-aid-cmcc-srs-ngos-banned-israel](https://www.dropsitenews.com/p/palantir-ai-gaza-humanitarian-aid-cmcc-srs-ngos-banned-israel)

生成摘要时出错

---

## 41. An autopsy of AI-generated 3D slop

**原文标题**: An autopsy of AI-generated 3D slop

**原文链接**: [https://aircada.com/blog/ai-vs-human-3d-ecommerce](https://aircada.com/blog/ai-vs-human-3d-ecommerce)

生成摘要时出错

---

## 42. F-Droid Board of Directors nominations 2026

**原文标题**: F-Droid Board of Directors nominations 2026

**原文链接**: [https://f-droid.org/2026/02/26/board-of-directors-nominations.html](https://f-droid.org/2026/02/26/board-of-directors-nominations.html)

生成摘要时出错

---

## 43. Show HN: RetroTick – Run classic Windows EXEs in the browser

**原文标题**: Show HN: RetroTick – Run classic Windows EXEs in the browser

**原文链接**: [https://retrotick.com/](https://retrotick.com/)

生成摘要时出错

---

## 44. Google Street View in 2026

**原文标题**: Google Street View in 2026

**原文链接**: [https://tech.marksblogg.com/google-street-view-coverage.html](https://tech.marksblogg.com/google-street-view-coverage.html)

生成摘要时出错

---

## 45. America, and probably the world, stands on a precipice

**原文标题**: America, and probably the world, stands on a precipice

**原文链接**: [https://garymarcus.substack.com/p/america-and-probably-the-world-stands](https://garymarcus.substack.com/p/america-and-probably-the-world-stands)

生成摘要时出错

---

## 46. Experts sound alarm after ChatGPT Health fails to recognise medical emergencies

**原文标题**: Experts sound alarm after ChatGPT Health fails to recognise medical emergencies

**原文链接**: [https://www.theguardian.com/technology/2026/feb/26/chatgpt-health-fails-recognise-medical-emergencies](https://www.theguardian.com/technology/2026/feb/26/chatgpt-health-fails-recognise-medical-emergencies)

生成摘要时出错

---

## 47. Dan Simmons, author of Hyperion, has died

**原文标题**: Dan Simmons, author of Hyperion, has died

**原文链接**: [https://www.dignitymemorial.com/obituaries/longmont-co/daniel-simmons-12758871](https://www.dignitymemorial.com/obituaries/longmont-co/daniel-simmons-12758871)

生成摘要时出错

---

## 48. Story of XZ Backdoor [video]

**原文标题**: Story of XZ Backdoor [video]

**原文链接**: [https://www.youtube.com/watch?v=aoag03mSuXQ](https://www.youtube.com/watch?v=aoag03mSuXQ)

生成摘要时出错

---

## 49. Launch HN: Cardboard (YC W26) – Agentic video editor

**原文标题**: Launch HN: Cardboard (YC W26) – Agentic video editor

**原文链接**: [https://www.usecardboard.com/](https://www.usecardboard.com/)

生成摘要时出错

---

## 50. Just-bash: Bash for Agents

**原文标题**: Just-bash: Bash for Agents

**原文链接**: [https://github.com/vercel-labs/just-bash](https://github.com/vercel-labs/just-bash)

生成摘要时出错

---

## 51. iPhone and iPad approved to handle classified NATO information

**原文标题**: iPhone and iPad approved to handle classified NATO information

**原文链接**: [https://www.apple.com/newsroom/2026/02/iphone-and-ipad-approved-to-handle-classified-nato-information/](https://www.apple.com/newsroom/2026/02/iphone-and-ipad-approved-to-handle-classified-nato-information/)

生成摘要时出错

---

## 52. Show HN: Deff – Side-by-side Git diff review in your terminal

**原文标题**: Show HN: Deff – Side-by-side Git diff review in your terminal

**原文链接**: [https://github.com/flamestro/deff](https://github.com/flamestro/deff)

生成摘要时出错

---

## 53. We gave terabytes of CI logs to an LLM

**原文标题**: We gave terabytes of CI logs to an LLM

**原文链接**: [https://www.mendral.com/blog/llms-are-good-at-sql](https://www.mendral.com/blog/llms-are-good-at-sql)

生成摘要时出错

---

## 54. Dear Time Lords: Freeze Computers in 1993

**原文标题**: Dear Time Lords: Freeze Computers in 1993

**原文链接**: [https://graydon2.dreamwidth.org/322461.html](https://graydon2.dreamwidth.org/322461.html)

生成摘要时出错

---

## 55. Parakeet.cpp – Parakeet ASR inference in pure C++ with Metal GPU acceleration

**原文标题**: Parakeet.cpp – Parakeet ASR inference in pure C++ with Metal GPU acceleration

**原文链接**: [https://github.com/Frikallo/parakeet.cpp](https://github.com/Frikallo/parakeet.cpp)

生成摘要时出错

---

## 56. Americans Are Leaving the U.S. in Record Numbers

**原文标题**: Americans Are Leaving the U.S. in Record Numbers

**原文链接**: [https://www.wsj.com/us-news/americans-leaving-the-us-migration-a5795bfa](https://www.wsj.com/us-news/americans-leaving-the-us-migration-a5795bfa)

生成摘要时出错

---

## 57. Vibe coded Lovable-hosted app littered with basic flaws exposed 18K users

**原文标题**: Vibe coded Lovable-hosted app littered with basic flaws exposed 18K users

**原文链接**: [https://www.theregister.com/2026/02/27/lovable_app_vulnerabilities/](https://www.theregister.com/2026/02/27/lovable_app_vulnerabilities/)

生成摘要时出错

---

## 58. Technical Excellence Is Not Enough

**原文标题**: Technical Excellence Is Not Enough

**原文链接**: [https://raccoon.land/posts/technical-excellence-is-not-enough/](https://raccoon.land/posts/technical-excellence-is-not-enough/)

生成摘要时出错

---

## 59. NASA announces major overhaul of Artemis program amid safety concerns, delays

**原文标题**: NASA announces major overhaul of Artemis program amid safety concerns, delays

**原文链接**: [https://www.cbsnews.com/news/nasa-artemis-moon-program-overhaul/](https://www.cbsnews.com/news/nasa-artemis-moon-program-overhaul/)

生成摘要时出错

---

## 60. MitID, Denmarks sole digital ID, has been down for over an hour and counting

**原文标题**: MitID, Denmarks sole digital ID, has been down for over an hour and counting

**原文链接**: [https://www.digitaliser.dk/mitid/nyt-fra-mitid/2026/feb/driftsforstyrrelser-mitid](https://www.digitaliser.dk/mitid/nyt-fra-mitid/2026/feb/driftsforstyrrelser-mitid)

生成摘要时出错

---

## 61. Men in their 50s may be aging faster due to toxic 'forever chemicals'

**原文标题**: Men in their 50s may be aging faster due to toxic 'forever chemicals'

**原文链接**: [https://www.cnn.com/2026/02/26/health/forever-chemicals-aging-men-wellness](https://www.cnn.com/2026/02/26/health/forever-chemicals-aging-men-wellness)

生成摘要时出错

---

## 62. Dyson settles forced labour suit in landmark UK case

**原文标题**: Dyson settles forced labour suit in landmark UK case

**原文链接**: [https://www.bbc.com/news/articles/cddnry8dnl7o](https://www.bbc.com/news/articles/cddnry8dnl7o)

生成摘要时出错

---

## 63. PostmarketOS in 2026-02: generic kernels, bans use of generative AI

**原文标题**: PostmarketOS in 2026-02: generic kernels, bans use of generative AI

**原文链接**: [https://postmarketos.org/blog/2026/02/26/pmOS-update-2026-02/](https://postmarketos.org/blog/2026/02/26/pmOS-update-2026-02/)

生成摘要时出错

---

## 64. Block spent $68M on a single party in September 2025

**原文标题**: Block spent $68M on a single party in September 2025

**原文链接**: [https://twitter.com/BullTheoryio/status/2027250361816486085](https://twitter.com/BullTheoryio/status/2027250361816486085)

生成摘要时出错

---

## 65. You Just Need Postgres

**原文标题**: You Just Need Postgres

**原文链接**: [https://youjustneedpostgres.com/](https://youjustneedpostgres.com/)

生成摘要时出错

---

## 66. Anthropic says company 'cannot in good conscience accede' to Pentagon's demands

**原文标题**: Anthropic says company 'cannot in good conscience accede' to Pentagon's demands

**原文链接**: [https://apnews.com/article/anthropic-ai-pentagon-hegseth-dario-amodei-9b28dda41bdb52b6a378fa9fc80b8fda](https://apnews.com/article/anthropic-ai-pentagon-hegseth-dario-amodei-9b28dda41bdb52b6a378fa9fc80b8fda)

生成摘要时出错

---

## 67. SynthID

**原文标题**: SynthID

**原文链接**: [https://deepmind.google/models/synthid/](https://deepmind.google/models/synthid/)

生成摘要时出错

---

## 68. Fentanyl makeover: Core structural redesign could lead to safer pain medications

**原文标题**: Fentanyl makeover: Core structural redesign could lead to safer pain medications

**原文链接**: [https://www.scripps.edu/news-and-events/press-room/2026/20260211-janda-molecule.html](https://www.scripps.edu/news-and-events/press-room/2026/20260211-janda-molecule.html)

生成摘要时出错

---

## 69. Burger King will use AI to check if employees say 'please' and 'thank you'

**原文标题**: Burger King will use AI to check if employees say 'please' and 'thank you'

**原文链接**: [https://www.theverge.com/ai-artificial-intelligence/884911/burger-king-ai-assistant-patty](https://www.theverge.com/ai-artificial-intelligence/884911/burger-king-ai-assistant-patty)

生成摘要时出错

---

## 70. OpenAI raises $110B on $730B pre-money valuation

**原文标题**: OpenAI raises $110B on $730B pre-money valuation

**原文链接**: [https://techcrunch.com/2026/02/27/openai-raises-110b-in-one-of-the-largest-private-funding-rounds-in-history/](https://techcrunch.com/2026/02/27/openai-raises-110b-in-one-of-the-largest-private-funding-rounds-in-history/)

生成摘要时出错

---

## 71. Steering interpretable language models with concept algebra

**原文标题**: Steering interpretable language models with concept algebra

**原文链接**: [https://www.guidelabs.ai/post/steerling-steering-8b/](https://www.guidelabs.ai/post/steerling-steering-8b/)

生成摘要时出错

---

## 72. Leaked Documents Show Meta Cracking Down on Access to Abortion Information

**原文标题**: Leaked Documents Show Meta Cracking Down on Access to Abortion Information

**原文链接**: [https://www.motherjones.com/politics/2026/02/meta-abortion-ai-chatbot-leak-teen-info-ban/](https://www.motherjones.com/politics/2026/02/meta-abortion-ai-chatbot-leak-teen-info-ban/)

生成摘要时出错

---

## 73. RK3588 and RK3576 video decoders support merged in the upstream Linux Kernel

**原文标题**: RK3588 and RK3576 video decoders support merged in the upstream Linux Kernel

**原文链接**: [https://www.collabora.com/news-and-blog/news-and-events/rk3588-and-rk3576-video-decoders-support-merged-in-the-upstream-linux-kernel.html](https://www.collabora.com/news-and-blog/news-and-events/rk3588-and-rk3576-video-decoders-support-merged-in-the-upstream-linux-kernel.html)

生成摘要时出错

---

## 74. Show HN: Badge that shows how well your codebase fits in an LLM's context window

**原文标题**: Show HN: Badge that shows how well your codebase fits in an LLM's context window

**原文链接**: [https://github.com/qwibitai/nanoclaw/tree/main/repo-tokens](https://github.com/qwibitai/nanoclaw/tree/main/repo-tokens)

生成摘要时出错

---

## 75. Origin of the rule that swap size should be 2x of the physical memory

**原文标题**: Origin of the rule that swap size should be 2x of the physical memory

**原文链接**: [https://retrocomputing.stackexchange.com/questions/32492/origin-of-the-rule-that-swap-size-should-be-2x-of-the-physical-memory](https://retrocomputing.stackexchange.com/questions/32492/origin-of-the-rule-that-swap-size-should-be-2x-of-the-physical-memory)

生成摘要时出错

---

## 76. 56% of CEOs report zero financial return from AI in 2026 (PwC survey, n=4,454)

**原文标题**: 56% of CEOs report zero financial return from AI in 2026 (PwC survey, n=4,454)

**原文链接**: [https://aishortcutlab.com/articles/pwc-ceo-survey-2026-only-12-of-ceos-win-with-ai](https://aishortcutlab.com/articles/pwc-ceo-survey-2026-only-12-of-ceos-win-with-ai)

生成摘要时出错

---

## 77. The Pentagon Feuding with an AI Company Is a Bad Sign

**原文标题**: The Pentagon Feuding with an AI Company Is a Bad Sign

**原文链接**: [https://foreignpolicy.com/2026/02/25/anthropic-pentagon-feud-ai/](https://foreignpolicy.com/2026/02/25/anthropic-pentagon-feud-ai/)

生成摘要时出错

---

## 78. New California law requires age verification for all OS accounts

**原文标题**: New California law requires age verification for all OS accounts

**原文链接**: [https://www.pcgamer.com/software/operating-systems/a-new-california-law-says-all-operating-systems-including-linux-need-to-have-some-form-of-age-verification-at-account-setup/](https://www.pcgamer.com/software/operating-systems/a-new-california-law-says-all-operating-systems-including-linux-need-to-have-some-form-of-age-verification-at-account-setup/)

生成摘要时出错

---

## 79. Why Developers Keep Choosing Claude over Every Other AI

**原文标题**: Why Developers Keep Choosing Claude over Every Other AI

**原文链接**: [https://www.bhusalmanish.com.np/blog/posts/why-claude-wins-coding.html](https://www.bhusalmanish.com.np/blog/posts/why-claude-wins-coding.html)

生成摘要时出错

---

## 80. Number of UK workers on zero-hours contracts hits record high ahead of crackdown

**原文标题**: Number of UK workers on zero-hours contracts hits record high ahead of crackdown

**原文链接**: [https://www.bbc.co.uk/news/articles/czj1m7d4gxpo](https://www.bbc.co.uk/news/articles/czj1m7d4gxpo)

生成摘要时出错

---

## 81. Working on Pharo Smalltalk: BPatterns: Rewrite Engine with Smalltalk Style

**原文标题**: Working on Pharo Smalltalk: BPatterns: Rewrite Engine with Smalltalk Style

**原文链接**: [http://dionisiydk.blogspot.com/2026/02/bpatterns-rewrite-engine-with-smalltalk.html](http://dionisiydk.blogspot.com/2026/02/bpatterns-rewrite-engine-with-smalltalk.html)

生成摘要时出错

---

## 82. Show HN: Agent Swarm – Multi-agent self-learning teams (OSS)

**原文标题**: Show HN: Agent Swarm – Multi-agent self-learning teams (OSS)

**原文链接**: [https://github.com/desplega-ai/agent-swarm](https://github.com/desplega-ai/agent-swarm)

生成摘要时出错

---

## 83. Hydroph0bia – fixed SecureBoot bypass for UEFI firmware from Insyde H2O (2025)

**原文标题**: Hydroph0bia – fixed SecureBoot bypass for UEFI firmware from Insyde H2O (2025)

**原文链接**: [https://coderush.me/hydroph0bia-part3/](https://coderush.me/hydroph0bia-part3/)

生成摘要时出错

---

## 84. OpenAI's $110B funding round (investments from Amazon, Nvidia, SoftBank)

**原文标题**: OpenAI's $110B funding round (investments from Amazon, Nvidia, SoftBank)

**原文链接**: [https://www.reuters.com/business/retail-consumer/amazon-invest-50-billion-openai-2026-02-27/](https://www.reuters.com/business/retail-consumer/amazon-invest-50-billion-openai-2026-02-27/)

生成摘要时出错

---

## 85. Allocating on the Stack

**原文标题**: Allocating on the Stack

**原文链接**: [https://go.dev/blog/allocation-optimizations](https://go.dev/blog/allocation-optimizations)

生成摘要时出错

---

## 86. The complete Manic Miner disassembly

**原文标题**: The complete Manic Miner disassembly

**原文链接**: [https://skoolkit.ca/disassemblies/manic_miner/](https://skoolkit.ca/disassemblies/manic_miner/)

生成摘要时出错

---

## 87. Show HN: ZSE – Open-source LLM inference engine with 3.9s cold starts

**原文标题**: Show HN: ZSE – Open-source LLM inference engine with 3.9s cold starts

**原文链接**: [https://github.com/Zyora-Dev/zse](https://github.com/Zyora-Dev/zse)

生成摘要时出错

---

## 88. Kansas invalidates driver's licenses, birth certificates for ~1k transgender

**原文标题**: Kansas invalidates driver's licenses, birth certificates for ~1k transgender

**原文链接**: [https://www.reuters.com/legal/government/kansas-invalidates-drivers-licenses-birth-certificates-over-1000-transgender-2026-02-26/](https://www.reuters.com/legal/government/kansas-invalidates-drivers-licenses-birth-certificates-over-1000-transgender-2026-02-26/)

生成摘要时出错

---

## 89. Move tests to closed source repo

**原文标题**: Move tests to closed source repo

**原文链接**: [https://github.com/tldraw/tldraw/issues/8082](https://github.com/tldraw/tldraw/issues/8082)

生成摘要时出错

---

## 90. Lawmakers say US Military used laser to take down Border Protection drone in TX

**原文标题**: Lawmakers say US Military used laser to take down Border Protection drone in TX

**原文链接**: [https://apnews.com/article/military-laser-border-drone-texas-airport-55aaab7093f7d6dd174f909f3875001c](https://apnews.com/article/military-laser-border-drone-texas-airport-55aaab7093f7d6dd174f909f3875001c)

生成摘要时出错

---

## 91. Sam Altman: We raised a $110B round from Amazon, Nvidia, SoftBank

**原文标题**: Sam Altman: We raised a $110B round from Amazon, Nvidia, SoftBank

**原文链接**: [https://twitter.com/sama/status/2027386252555919386](https://twitter.com/sama/status/2027386252555919386)

生成摘要时出错

---

## 92. US farmers are rejecting multimillion-dollar datacenter bids for their land

**原文标题**: US farmers are rejecting multimillion-dollar datacenter bids for their land

**原文链接**: [https://www.theguardian.com/technology/2026/feb/21/us-farmers-datacenters](https://www.theguardian.com/technology/2026/feb/21/us-farmers-datacenters)

生成摘要时出错

---

## 93. Compact disc story (1998)

**原文标题**: Compact disc story (1998)

**原文链接**: [https://www.researchgate.net/publication/294484774_Compact_disc_story](https://www.researchgate.net/publication/294484774_Compact_disc_story)

生成摘要时出错

---

## 94. Larry Page has moved to Florida

**原文标题**: Larry Page has moved to Florida

**原文链接**: [https://twitter.com/paulg/status/2026737030257062253](https://twitter.com/paulg/status/2026737030257062253)

生成摘要时出错

---

## 95. Show HN: Rev-dep – 20x faster knip.dev alternative build in Go

**原文标题**: Show HN: Rev-dep – 20x faster knip.dev alternative build in Go

**原文链接**: [https://github.com/jayu/rev-dep](https://github.com/jayu/rev-dep)

生成摘要时出错

---

## 96. Running OpenClaw on an isolated cloud VM

**原文标题**: Running OpenClaw on an isolated cloud VM

**原文链接**: [https://blog.skypilot.co/openclaw-on-skypilot/](https://blog.skypilot.co/openclaw-on-skypilot/)

生成摘要时出错

---

## 97. Anthropic gives Opus 3 exit interview, "retirement" blog

**原文标题**: Anthropic gives Opus 3 exit interview, "retirement" blog

**原文链接**: [https://www.anthropic.com/research/deprecation-updates-opus-3](https://www.anthropic.com/research/deprecation-updates-opus-3)

生成摘要时出错

---

## 98. Show HN: Mission Control – Open-source task management for AI agents

**原文标题**: Show HN: Mission Control – Open-source task management for AI agents

**原文链接**: [https://github.com/MeisnerDan/mission-control](https://github.com/MeisnerDan/mission-control)

生成摘要时出错

---

## 99. US Customs destroys rare floppy disk

**原文标题**: US Customs destroys rare floppy disk

**原文链接**: [https://twitter.com/TehKeripo/status/2027171532825571678](https://twitter.com/TehKeripo/status/2027171532825571678)

生成摘要时出错

---

## 100. Canada and South Korea sign a defence agreement

**原文标题**: Canada and South Korea sign a defence agreement

**原文链接**: [https://www.cbc.ca/lite/story/9.7106354](https://www.cbc.ca/lite/story/9.7106354)

生成摘要时出错

---

