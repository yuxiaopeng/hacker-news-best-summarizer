# Hacker News 热门文章摘要 (2026-02-22)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 我验证了我的领英身份。这是我提供的。

**原文标题**: I verified my LinkedIn identity. Here's what I handed over

**原文链接**: [https://thelocalstack.eu/posts/linkedin-identity-verification-privacy/](https://thelocalstack.eu/posts/linkedin-identity-verification-privacy/)

LinkedIn上进行“蓝勾”身份验证时，用户会被重定向到一家美国公司Persona Identities, Inc.，而非直接通过LinkedIn验证。作者发现Persona收集了大量个人数据，包括全名、护照信息、自拍照、面部几何数据（生物识别数据）、NFC芯片数据、国民身份号码，甚至行为生物识别数据，例如犹豫检测。

Persona还会将这些信息与众多第三方来源（包括政府数据库和信用机构）进行交叉比对，实质上是在进行背景调查。令人担忧的是，Persona利用上传的身份文件和自拍照来训练其AI，声称是出于“合法利益”，而非获得明确同意。

尽管LinkedIn仅接收有限的模糊身份信息，但Persona却与17家分包处理商（其中16家位于美国，包括Anthropic和OpenAI等AI公司）共享完整数据。这给欧洲用户带来了重大的隐私担忧，因为Persona作为一家美国公司，受美国《云法案》（US CLOUD Act）的约束。该法案允许美国执法部门要求获取数据，即使数据存储在欧洲，并且可能附带“封口令”，从而凌驾于《欧美数据隐私框架》之上。

文章强调了生物识别数据的风险，这类数据独一无二且无法更改。尽管Persona声称会在六个月内删除生物识别数据，但美国法律程序可能强制其无限期保留。此外，Persona的条款将数据泄露的责任上限设为区区50美元，并强制要求在美国进行仲裁。

作者建议所有已验证身份的用户请求获取其数据、要求删除数据，并联系Persona的数据保护官，敦促用户充分了解为获得一个“装饰性徽章”所付出的巨大数据代价。

---

## 2. 我发现了一个漏洞。他们找到了一个律师。

**原文标题**: I found a vulnerability. they found a lawyer

**原文链接**: [https://dixken.de/blog/i-found-a-vulnerability-they-found-a-lawyer](https://dixken.de/blog/i-found-a-vulnerability-they-found-a-lawyer)

作者（一名潜水教练兼平台工程师）在一家主要潜水保险公司的会员门户网站中发现了一个严重漏洞。该系统为新账户（包括未成年人账户）分配了连续的数字用户ID和静态默认密码。这使得未经任何速率限制、账户锁定或多因素认证，即可轻松访问敏感个人数据（姓名、地址、出生日期、联系方式）。

作者于2025年4月28日负责任地向马耳他计算机安全事件响应小组（CSIRT Malta）和该组织披露了这一缺陷，并提供了30天的禁发期。该组织的律师事务所作出回应，承认漏洞已修复，但批评了涉及当局的做法，并威胁如果公开披露将采取法律行动。他们要求作者在当天结束前签署一份广泛的保密协议（NDA）。

作者拒绝签署保密协议，认为透明度至关重要，尤其是在GDPR合规性和未成年人数据暴露方面。他还指出，让马耳他计算机安全事件响应小组（CSIRT Malta）介入是负责任披露的一部分。该组织随后升级了应对措施，援引马耳他刑法（计算机滥用），并重申威胁，禁止公开提及此事件。他们甚至指责用户没有更改默认密码。

尽管漏洞已修复，但作者尚未收到受影响用户已被通知的确认，这对于高风险数据泄露是GDPR的要求。他总结认为，这种“寒蝉效应”式的回应（即组织威胁研究人员而非合作）将声誉置于数据保护之上。他倡导制定协同漏洞披露政策，感谢研究人员，并建议研究人员与国家计算机安全事件响应小组（CSIRT）合作，记录一切，并拒绝签署旨在消音的保密协议。

---

## 3. 我如何使用 Claude 代码：规划与执行分离

**原文标题**: How I use Claude Code: Separation of planning and execution

**原文链接**: [https://boristane.com/blog/how-i-use-claude-code/](https://boristane.com/blog/how-i-use-claude-code/)

作者描述了一种严格的Claude代码工作流程，强调规划与执行的严格分离，这与典型的AI编码工具使用方式截然不同。其核心原则是，在书面计划经过审查和批准之前，绝不让Claude编写代码，从而避免浪费精力，保持架构控制，并产生卓越的成果。

该工作流程包含几个不同的阶段：
1.  **研究：** Claude深入阅读相关的代码库部分，并将发现写入一个持久化的`research.md`文件。这使得作者能够在任何规划之前验证理解并纠正错误。
2.  **规划：** Claude生成一个详细的`plan.md`文档，概述实现方法、代码片段和文件更改。
3.  **注释循环：** 这是最独特的阶段。作者在编辑器中审查`plan.md`，添加内联注释（纠正假设、增加约束、注入领域知识），然后将其发回给Claude更新文档。这个循环重复1-6次，并带有明确的“尚未实现”防护，确保人类判断彻底塑造了计划。`plan.md`充当共享可变状态。
4.  **待办事项列表：** 在实施之前，会将详细的任务分解添加到`plan.md`中，用于跟踪进度。
5.  **实施：** 一个单一的、全面的提示指示Claude执行整个计划，标记任务完成，保持严格类型，并持续运行类型检查。到此阶段，执行是机械性的，因为所有创造性决策都已完成。
6.  **反馈：** 在实施过程中，作者充当监督者，提供简洁的更正，引用现有代码，或在需要时回滚和重新确定范围。作者通过评估Claude的建议、削减范围和覆盖技术选择来保持控制。

整个过程，从研究到实施，通常在长时间的单次会话中进行，而持久化的计划文档则保留了上下文。这种严格的方法，没有“神奇提示”，确保了知情、受控和有效的AI辅助开发。

---

## 4. 关闭 Dependabot

**原文标题**: Turn Dependabot off

**原文链接**: [https://words.filippo.io/dependabot/](https://words.filippo.io/dependabot/)

作者主张关闭Dependabot，称其为“噪音机器”，会造成警报疲劳，尤其是在Go语言安全警报方面。他们引用了一个案例研究，其中Dependabot针对`filippo.io/edwards25519`漏洞生成了数千个不相关的PR和误报的安全警报，即使是对于未使用受影响代码路径甚至未使用该漏洞包的存储库也是如此。这浪费了时间，通过使正确的分类变得不切实际而降低了安全性，并加重了开源维护者的负担。

相反，作者推荐了两个定时运行的GitHub Actions。对于安全性，用`govulncheck`取代Dependabot。该工具由Go漏洞数据库提供支持，利用静态分析仅识别*可达的*易受攻击符号，与Dependabot宽泛的包级别警报相比，大大减少了误报。这确保了通知针对的是实际的、有影响力的漏洞。

对于一般的依赖更新，不应自动打开PR，而应通过一个独立的GitHub Action每天运行`go get -u -t ./...`（或其他生态系统中的类似命令）。这可以在不提交更改的情况下，针对*最新*的依赖版本测试项目，从而实现早期发现破坏性更改，并减少未来安全修复的“补丁差异”。这种方法将依赖更新决策与发布周期分离，提供了更大的控制权并防止了持续中断，同时通过在生产环境前在CI中测试更新来减轻供应链攻击风险。

---

## 5. 维基百科弃用Archive.today，开始移除存档链接

**原文标题**: Wikipedia deprecates Archive.today, starts removing archive links

**原文链接**: [https://arstechnica.com/tech-policy/2026/02/wikipedia-bans-archive-today-after-site-executed-ddos-and-altered-web-captures/](https://arstechnica.com/tech-policy/2026/02/wikipedia-bans-archive-today-after-site-executed-ddos-and-altered-web-captures/)

维基百科英文版正在将Archive.today列入黑名单并移除其链接，此前该网站被用于发起分布式拒绝服务（DDoS）攻击，并被发现恶意篡改了存档内容。

这次DDoS攻击的目标是Jani Patokallio的Gyrovague博客，通过Archive.today上的恶意验证码（CAPTCHA）代码发起，此前Patokallio发布了讨论该存档网站维护者身份的帖子。在随后的讨论中，维基百科编辑人员发现Archive.today蓄意修改了存档网页快照，将Patokallio的名字插入到内容和评论中，似乎是出于个人恩怨。这种篡改行为严重损害了Archive.today的可靠性和可验证性。

维基百科目前正要求编辑人员移除遍布40万个页面的超过69.5万个指向Archive.today的链接。指导方针规定，将这些链接替换为其他存档服务，例如互联网档案馆（Archive.org）、Ghostarchive或Megalodon，或者如果原始来源仍然有效则直接删除。强调指出互联网档案馆是独立且未涉事的。

Patokallio对维基百科的决定表示欢迎，并指出Archive.today的维护者（“Nora”）也曾向他发出人身威胁。编辑人员认为内容篡改是严重的信任违背行为，维基媒体基金会也因安全问题考虑介入。

---

## 6. 安全许可表格上不该写什么 (1988)

**原文标题**: What not to write on your security clearance form (1988)

**原文链接**: [https://milk.com/wall-o-shame/security_clearance.html](https://milk.com/wall-o-shame/security_clearance.html)

1988年，莱斯·厄内斯特讲述了一件离奇的童年往事，这件事后来给他的安全许可带来了麻烦。他12岁时，和一位朋友读了一本密码学书籍后，创建了一套秘密代码。莱斯把他的密码钥匙藏在眼镜盒里。1943年，他在一辆有轨电车上弄丢了眼镜盒。一位爱国公民找到了它，在二战的偏执气氛下，误将密码钥匙当作日本间谍材料，并将其交给了联邦调查局。

联邦调查局随即展开了一项范围广泛、优先级很高的调查。六周后，一名特工拜访了莱斯的母亲，失望地发现这名可疑的间谍竟然只有12岁。特工归还了眼镜，但保留了密码钥匙，并强调此案耗费了数千美元和最高优先级的资源。

多年后，当莱斯申请海军安全许可时，他如实回答了“你是否曾被联邦调查局调查过？”这一问题，选择了“是”，并解释说他“曾被怀疑是日本间谍”。安全官员勃然大怒，撕毁了表格，并警告莱斯重新填写，不许提及此事，否则他将确保莱斯永远无法获得许可。莱斯照办了，获得了许可，并随后在所有未来的安全表格上都隐瞒了此事。

---

## 7. 全美各地，人们正在拆除并破坏Flock监控摄像头。

**原文标题**: Across the US, people are dismantling and destroying Flock surveillance cameras

**原文链接**: [https://www.bloodinthemachine.com/p/across-the-us-people-are-dismantling](https://www.bloodinthemachine.com/p/across-the-us-people-are-dismantling)

在美国各地，人们正在积极拆除和销毁Flock监控摄像头，这股浪潮源于人们对这些摄像头与ICE（美国移民及海关执法局）的关联、普遍的隐私侵犯以及地方政府无视民意的愤怒。破坏事件，包括摄像头被砸毁和电线杆被切断，已在至少五个州（从加利福尼亚州到弗吉尼亚州）被报道。其中，一名男子因破坏13台设备被捕，并被人们誉为英雄。

估价75亿美元的Flock摄像头使用自动车牌识别器收集车辆识别数据，这些数据无需搜查令即可获取，并例行与ICE共享，引发了人们对违反第四修正案以及其被用于追踪个人（例如跨州寻求堕胎者）的担忧。尽管圣克鲁斯和尤金等一些城市已取消了合同，但公众的愤怒常常导致针对这些设备的直接行动，这些破坏行为在网上获得了广泛支持。

在相关新闻中，一名俄克拉荷马州男子在反对一个当地数据中心项目时，因超出其分配的公众评论时间几秒而被捕。此外，一万名优步和Lyft司机向加州劳工委员会请愿，要求追回22号提案（Prop 22）生效前被克扣的数十亿美元工资。最后，根据特斯拉自己的数据显示，该公司在奥斯汀的新型“机器人出租车”（RoboTaxis）的事故发生率据报道是人类驾驶员的四倍。

---

## 8. Why is Claude an Electron app?

**原文标题**: Why is Claude an Electron app?

**原文链接**: [https://www.dbreunig.com/2026/02/21/why-is-claude-an-electron-app.html](https://www.dbreunig.com/2026/02/21/why-is-claude-an-electron-app.html)

生成摘要时出错

---

## 9. Attention Media ≠ Social Networks

**原文标题**: Attention Media ≠ Social Networks

**原文链接**: [https://susam.net/attention-media-vs-social-networks.html](https://susam.net/attention-media-vs-social-networks.html)

Susam Pal argues that web-based social networks, once genuinely social and hopeful in the early 2000s, devolved into "attention media" between 2012 and 2016. Initially, platforms like early Twitter fostered genuine connections, offering relevant updates from chosen contacts and meaningful notifications. This era, part of Web 2.0, emphasized user participation and interaction.

However, the introduction of infinite scroll and bogus, manipulative notifications marked a turning point. Notifications ceased to serve users, instead becoming arbitrary prompts designed to capture attention. Timelines increasingly filled with content from strangers rather than friends, making the services feel overwhelming and unsocial. Pal describes this shift as platforms prioritizing attention capture and monetization over genuine social interaction, leading him to abandon them due to the irrelevant and unsubstantial content.

In contrast, Pal highlights Mastodon as a return to original social networking principles. It allows users to follow a select group of genuinely interesting individuals, receiving only their updates without manipulative algorithms or bogus notifications. This creates a calm, predictable timeline based on user choices, reminiscent of the early, user-centric days of social media, a model Pal hopes Mastodon maintains.

---

## 10. Claws are now a new layer on top of LLM agents

**原文标题**: Claws are now a new layer on top of LLM agents

**原文链接**: [https://twitter.com/karpathy/status/2024987174077432126](https://twitter.com/karpathy/status/2024987174077432126)

生成摘要时出错

---

## 11. How Taalas “prints” LLM onto a chip?

**原文标题**: How Taalas “prints” LLM onto a chip?

**原文链接**: [https://www.anuragk.com/blog/posts/Taalas.html](https://www.anuragk.com/blog/posts/Taalas.html)

生成摘要时出错

---

## 12. Show HN: Llama 3.1 70B on a single RTX 3090 via NVMe-to-GPU bypassing the CPU

**原文标题**: Show HN: Llama 3.1 70B on a single RTX 3090 via NVMe-to-GPU bypassing the CPU

**原文链接**: [https://github.com/xaskasdf/ntransformer](https://github.com/xaskasdf/ntransformer)

生成摘要时出错

---

## 13. Be wary of Bluesky

**原文标题**: Be wary of Bluesky

**原文链接**: [https://kevinak.se/blog/be-wary-of-bluesky](https://kevinak.se/blog/be-wary-of-bluesky)

生成摘要时出错

---

## 14. Every company building your AI assistant is now an ad company

**原文标题**: Every company building your AI assistant is now an ad company

**原文链接**: [https://juno-labs.com/blogs/every-company-building-your-ai-assistant-is-an-ad-company](https://juno-labs.com/blogs/every-company-building-your-ai-assistant-is-an-ad-company)

生成摘要时出错

---

## 15. Andrej Karpathy talks about "Claws"

**原文标题**: Andrej Karpathy talks about "Claws"

**原文链接**: [https://simonwillison.net/2026/Feb/21/claws/](https://simonwillison.net/2026/Feb/21/claws/)

生成摘要时出错

---

## 16. Gamedate – A site to revive dead multiplayer games

**原文标题**: Gamedate – A site to revive dead multiplayer games

**原文链接**: [https://gamedate.org/](https://gamedate.org/)

生成摘要时出错

---

## 17. AI uBlock Blacklist

**原文标题**: AI uBlock Blacklist

**原文链接**: [https://github.com/alvi-se/ai-ublock-blacklist](https://github.com/alvi-se/ai-ublock-blacklist)

生成摘要时出错

---

## 18. Iran students stage first large anti-government protests since deadly crackdown

**原文标题**: Iran students stage first large anti-government protests since deadly crackdown

**原文链接**: [https://www.bbc.com/news/articles/c5yj2kzkrj0o](https://www.bbc.com/news/articles/c5yj2kzkrj0o)

生成摘要时出错

---

## 19. CXMT has been offering DDR4 chips at about half the prevailing market rate

**原文标题**: CXMT has been offering DDR4 chips at about half the prevailing market rate

**原文链接**: [https://www.koreaherald.com/article/10679206](https://www.koreaherald.com/article/10679206)

生成摘要时出错

---

## 20. zclaw: personal AI assistant in under 888 KB, running on an ESP32

**原文标题**: zclaw: personal AI assistant in under 888 KB, running on an ESP32

**原文链接**: [https://github.com/tnm/zclaw](https://github.com/tnm/zclaw)

生成摘要时出错

---

## 21. CERN rebuilt the original browser from 1989 (2019)

**原文标题**: CERN rebuilt the original browser from 1989 (2019)

**原文链接**: [https://worldwideweb.cern.ch](https://worldwideweb.cern.ch)

生成摘要时出错

---

## 22. Parse, Don't Validate and Type-Driven Design in Rust

**原文标题**: Parse, Don't Validate and Type-Driven Design in Rust

**原文链接**: [https://www.harudagondi.space/blog/parse-dont-validate-and-type-driven-design-in-rust/](https://www.harudagondi.space/blog/parse-dont-validate-and-type-driven-design-in-rust/)

生成摘要时出错

---

## 23. Acme Weather

**原文标题**: Acme Weather

**原文链接**: [https://acmeweather.com/blog/introducing-acme-weather](https://acmeweather.com/blog/introducing-acme-weather)

生成摘要时出错

---

## 24. Personal Statement of a CIA Analyst

**原文标题**: Personal Statement of a CIA Analyst

**原文链接**: [https://antipolygraph.org/statements/statement-038.shtml](https://antipolygraph.org/statements/statement-038.shtml)

生成摘要时出错

---

## 25. EU mandates replaceable batteries by 2027 (2023)

**原文标题**: EU mandates replaceable batteries by 2027 (2023)

**原文链接**: [https://environment.ec.europa.eu/news/new-law-more-sustainable-circular-and-safe-batteries-enters-force-2023-08-17_en](https://environment.ec.europa.eu/news/new-law-more-sustainable-circular-and-safe-batteries-enters-force-2023-08-17_en)

生成摘要时出错

---

## 26. OpenScan

**原文标题**: OpenScan

**原文链接**: [https://openscan.eu/pages/scan-gallery](https://openscan.eu/pages/scan-gallery)

生成摘要时出错

---

## 27. What Is OAuth?

**原文标题**: What Is OAuth?

**原文链接**: [https://leaflet.pub/p/did:plc:3vdrgzr2zybocs45yfhcr6ur/3mfd2oxx5v22b](https://leaflet.pub/p/did:plc:3vdrgzr2zybocs45yfhcr6ur/3mfd2oxx5v22b)

生成摘要时出错

---

## 28. macOS's Little-Known Command-Line Sandboxing Tool (2025)

**原文标题**: macOS's Little-Known Command-Line Sandboxing Tool (2025)

**原文链接**: [https://igorstechnoclub.com/sandbox-exec/](https://igorstechnoclub.com/sandbox-exec/)

生成摘要时出错

---

## 29. EDuke32 – Duke Nukem 3D (Open-Source)

**原文标题**: EDuke32 – Duke Nukem 3D (Open-Source)

**原文链接**: [https://www.eduke32.com/](https://www.eduke32.com/)

生成摘要时出错

---

## 30. Evidence of the bouba-kiki effect in naïve baby chicks

**原文标题**: Evidence of the bouba-kiki effect in naïve baby chicks

**原文链接**: [https://www.science.org/doi/10.1126/science.adq7188](https://www.science.org/doi/10.1126/science.adq7188)

生成摘要时出错

---

## 31. Cloudflare outage on February 20, 2026

**原文标题**: Cloudflare outage on February 20, 2026

**原文链接**: [https://blog.cloudflare.com/cloudflare-outage-february-20-2026/](https://blog.cloudflare.com/cloudflare-outage-february-20-2026/)

生成摘要时出错

---

## 32. A16z partner says that the theory that we’ll vibe code everything is wrong

**原文标题**: A16z partner says that the theory that we’ll vibe code everything is wrong

**原文链接**: [https://www.aol.com/articles/a16z-partner-says-theory-well-050150534.html](https://www.aol.com/articles/a16z-partner-says-theory-well-050150534.html)

生成摘要时出错

---

## 33. Japanese Woodblock Print Search

**原文标题**: Japanese Woodblock Print Search

**原文链接**: [https://ukiyo-e.org/](https://ukiyo-e.org/)

生成摘要时出错

---

## 34. Back to FreeBSD: Part 1

**原文标题**: Back to FreeBSD: Part 1

**原文链接**: [https://hypha.pub/back-to-freebsd-part-1](https://hypha.pub/back-to-freebsd-part-1)

生成摘要时出错

---

## 35. Don't create .gitkeep files, use .gitignore instead (2023)

**原文标题**: Don't create .gitkeep files, use .gitignore instead (2023)

**原文链接**: [https://adamj.eu/tech/2023/09/18/git-dont-create-gitkeep/](https://adamj.eu/tech/2023/09/18/git-dont-create-gitkeep/)

生成摘要时出错

---

## 36. Toyota’s hydrogen-powered Mirai has experienced rapid depreciation

**原文标题**: Toyota’s hydrogen-powered Mirai has experienced rapid depreciation

**原文链接**: [https://carbuzz.com/toyota-mirai-massive-depreciation-one-year/](https://carbuzz.com/toyota-mirai-massive-depreciation-one-year/)

生成摘要时出错

---

## 37. What Is a Database Transaction?

**原文标题**: What Is a Database Transaction?

**原文链接**: [https://planetscale.com/blog/database-transactions](https://planetscale.com/blog/database-transactions)

生成摘要时出错

---

## 38. We hid backdoors in ~40MB binaries and asked AI + Ghidra to find them

**原文标题**: We hid backdoors in ~40MB binaries and asked AI + Ghidra to find them

**原文链接**: [https://quesma.com/blog/introducing-binaryaudit/](https://quesma.com/blog/introducing-binaryaudit/)

生成摘要时出错

---

## 39. Cord: Coordinating Trees of AI Agents

**原文标题**: Cord: Coordinating Trees of AI Agents

**原文链接**: [https://www.june.kim/cord](https://www.june.kim/cord)

生成摘要时出错

---

## 40. Meta Deployed AI and It Is Killing Our Agency

**原文标题**: Meta Deployed AI and It Is Killing Our Agency

**原文链接**: [https://mojodojo.io/blog/meta-is-systematically-killing-our-agency/](https://mojodojo.io/blog/meta-is-systematically-killing-our-agency/)

生成摘要时出错

---

## 41. A Botnet Accidentally Destroyed I2P

**原文标题**: A Botnet Accidentally Destroyed I2P

**原文链接**: [https://www.sambent.com/a-botnet-accidentally-destroyed-i2p-the-full-story/](https://www.sambent.com/a-botnet-accidentally-destroyed-i2p-the-full-story/)

生成摘要时出错

---

## 42. LibreOffice blasts OnlyOffice for working with Microsoft to lock users in

**原文标题**: LibreOffice blasts OnlyOffice for working with Microsoft to lock users in

**原文链接**: [https://www.neowin.net/news/libreoffice-blasts-fake-open-source-onlyoffice-for-working-with-microsoft-to-lock-users-in/](https://www.neowin.net/news/libreoffice-blasts-fake-open-source-onlyoffice-for-working-with-microsoft-to-lock-users-in/)

生成摘要时出错

---

## 43. Man accidentally gains control of 7k robot vacuums

**原文标题**: Man accidentally gains control of 7k robot vacuums

**原文链接**: [https://www.popsci.com/technology/robot-vacuum-army/](https://www.popsci.com/technology/robot-vacuum-army/)

生成摘要时出错

---

## 44. Over 80% of 16 to 24-year-olds would vote to rejoin the EU

**原文标题**: Over 80% of 16 to 24-year-olds would vote to rejoin the EU

**原文链接**: [https://www.itv.com/news/2026-02-19/over-80-of-16-to-24-year-olds-would-vote-to-rejoin-the-eu-itv-poll-finds](https://www.itv.com/news/2026-02-19/over-80-of-16-to-24-year-olds-would-vote-to-rejoin-the-eu-itv-poll-finds)

生成摘要时出错

---

## 45. FCC asks stations for "pro-America" programming, like daily Pledge of Allegiance

**原文标题**: FCC asks stations for "pro-America" programming, like daily Pledge of Allegiance

**原文链接**: [https://arstechnica.com/tech-policy/2026/02/fcc-asks-stations-for-pro-america-programming-like-daily-pledge-of-allegiance/](https://arstechnica.com/tech-policy/2026/02/fcc-asks-stations-for-pro-america-programming-like-daily-pledge-of-allegiance/)

生成摘要时出错

---

## 46. Coccinelle: Source-to-source transformation tool

**原文标题**: Coccinelle: Source-to-source transformation tool

**原文链接**: [https://github.com/coccinelle/coccinelle](https://github.com/coccinelle/coccinelle)

生成摘要时出错

---

## 47. 24 Hour Fitness won't let you unsubscribe from marketing spam, so I fixed it

**原文标题**: 24 Hour Fitness won't let you unsubscribe from marketing spam, so I fixed it

**原文链接**: [https://ahmedkaddoura.com/projects/24hf-unsubscribe](https://ahmedkaddoura.com/projects/24hf-unsubscribe)

生成摘要时出错

---

## 48. Canvas_ity: A tiny, single-header <canvas>-like 2D rasterizer for C++

**原文标题**: Canvas_ity: A tiny, single-header <canvas>-like 2D rasterizer for C++

**原文链接**: [https://github.com/a-e-k/canvas_ity](https://github.com/a-e-k/canvas_ity)

生成摘要时出错

---

## 49. Fix Your Tools

**原文标题**: Fix Your Tools

**原文链接**: [https://ochagavia.nl/blog/fix-your-tools/](https://ochagavia.nl/blog/fix-your-tools/)

生成摘要时出错

---

## 50. Inputlag.science – Repository of knowledge about input lag in gaming

**原文标题**: Inputlag.science – Repository of knowledge about input lag in gaming

**原文链接**: [https://inputlag.science](https://inputlag.science)

生成摘要时出错

---

## 51. Show HN: Mines.fyi – all the mines in the US in a leaflet visualization

**原文标题**: Show HN: Mines.fyi – all the mines in the US in a leaflet visualization

**原文链接**: [https://mines.fyi/](https://mines.fyi/)

生成摘要时出错

---

## 52. Phil Spencer is exiting Microsoft as AI executive takes over Xbox

**原文标题**: Phil Spencer is exiting Microsoft as AI executive takes over Xbox

**原文链接**: [https://www.neowin.net/news/phil-spencer-is-exiting-microsoft-as-ai-executive-takes-over-xbox/](https://www.neowin.net/news/phil-spencer-is-exiting-microsoft-as-ai-executive-takes-over-xbox/)

生成摘要时出错

---

## 53. Minions: Stripe’s one-shot, end-to-end coding agents

**原文标题**: Minions: Stripe’s one-shot, end-to-end coding agents

**原文链接**: [https://stripe.dev/blog/minions-stripes-one-shot-end-to-end-coding-agents](https://stripe.dev/blog/minions-stripes-one-shot-end-to-end-coding-agents)

生成摘要时出错

---

## 54. Loon: A functional lang with invisible types, safe ownership, and alg. effects

**原文标题**: Loon: A functional lang with invisible types, safe ownership, and alg. effects

**原文链接**: [https://loonlang.com](https://loonlang.com)

生成摘要时出错

---

## 55. Xweather Live – Interactive global vector weather map

**原文标题**: Xweather Live – Interactive global vector weather map

**原文链接**: [https://live.xweather.com/](https://live.xweather.com/)

生成摘要时出错

---

## 56. Password managers less secure than promised

**原文标题**: Password managers less secure than promised

**原文链接**: [https://ethz.ch/en/news-and-events/eth-news/news/2026/02/password-managers-less-secure-than-promised.html](https://ethz.ch/en/news-and-events/eth-news/news/2026/02/password-managers-less-secure-than-promised.html)

生成摘要时出错

---

## 57. Palantir's secret weapon isn't AI – it's Ontology. An open-source deep dive

**原文标题**: Palantir's secret weapon isn't AI – it's Ontology. An open-source deep dive

**原文链接**: [https://github.com/Leading-AI-IO/palantir-ontology-strategy](https://github.com/Leading-AI-IO/palantir-ontology-strategy)

生成摘要时出错

---

## 58. Show HN: Iron-Wolf – Wolfenstein 3D source port in Rust

**原文标题**: Show HN: Iron-Wolf – Wolfenstein 3D source port in Rust

**原文链接**: [https://github.com/Ragnaroek/iron-wolf](https://github.com/Ragnaroek/iron-wolf)

生成摘要时出错

---

## 59. Iranian Students Protest as Anger Grows

**原文标题**: Iranian Students Protest as Anger Grows

**原文链接**: [https://www.wsj.com/world/middle-east/iranian-students-protest-as-anger-grows-89a6a44e](https://www.wsj.com/world/middle-east/iranian-students-protest-as-anger-grows-89a6a44e)

生成摘要时出错

---

## 60. I hate AI side projects

**原文标题**: I hate AI side projects

**原文链接**: [https://dylancastillo.co/posts/ai-side-projects.html](https://dylancastillo.co/posts/ai-side-projects.html)

生成摘要时出错

---

## 61. DialUp95 – A 90s inspired nostalgia hit

**原文标题**: DialUp95 – A 90s inspired nostalgia hit

**原文链接**: [https://dialup95.com/](https://dialup95.com/)

生成摘要时出错

---

## 62. Trunk Based Development

**原文标题**: Trunk Based Development

**原文链接**: [https://trunkbaseddevelopment.com/](https://trunkbaseddevelopment.com/)

生成摘要时出错

---

## 63. How an inference provider can prove they're not serving a quantized model

**原文标题**: How an inference provider can prove they're not serving a quantized model

**原文链接**: [https://tinfoil.sh/blog/2026-02-03-proving-model-identity](https://tinfoil.sh/blog/2026-02-03-proving-model-identity)

生成摘要时出错

---

## 64. U.S. Cannot Legally Impose Tariffs Using Section 122 of the Trade Act of 1974

**原文标题**: U.S. Cannot Legally Impose Tariffs Using Section 122 of the Trade Act of 1974

**原文链接**: [https://ielp.worldtradelaw.net/2026/01/guest-post-president-trump-cannot-legally-impose-tariffs-using-section-122-of-the-trade-act-of-1974/](https://ielp.worldtradelaw.net/2026/01/guest-post-president-trump-cannot-legally-impose-tariffs-using-section-122-of-the-trade-act-of-1974/)

生成摘要时出错

---

## 65. People Loved the Dot-Com Boom. The A.I. Boom, Not So Much

**原文标题**: People Loved the Dot-Com Boom. The A.I. Boom, Not So Much

**原文链接**: [https://www.nytimes.com/2026/02/21/technology/ai-boom-backlash.html](https://www.nytimes.com/2026/02/21/technology/ai-boom-backlash.html)

生成摘要时出错

---

## 66. The dance floor is disappearing in a sea of phones

**原文标题**: The dance floor is disappearing in a sea of phones

**原文链接**: [https://www.bloomberg.com/news/features/2026-02-20/a-boom-in-electronic-dance-music-is-changing-club-culture](https://www.bloomberg.com/news/features/2026-02-20/a-boom-in-electronic-dance-music-is-changing-club-culture)

生成摘要时出错

---

## 67. The Software Development Lifecycle Is Dead

**原文标题**: The Software Development Lifecycle Is Dead

**原文链接**: [https://boristane.com/blog/the-software-development-lifecycle-is-dead/](https://boristane.com/blog/the-software-development-lifecycle-is-dead/)

生成摘要时出错

---

## 68. The Nekonomicon – Nekochan.net Archive, Updated

**原文标题**: The Nekonomicon – Nekochan.net Archive, Updated

**原文链接**: [http://nekonomicon.irixnet.org/](http://nekonomicon.irixnet.org/)

生成摘要时出错

---

## 69. Excessive token usage in Claude Code

**原文标题**: Excessive token usage in Claude Code

**原文链接**: [https://github.com/anthropics/claude-code/issues/16856](https://github.com/anthropics/claude-code/issues/16856)

生成摘要时出错

---

## 70. Palantir Captured the UK Ministry of Defence

**原文标题**: Palantir Captured the UK Ministry of Defence

**原文链接**: [https://www.ft.com/content/5207928a-13e8-4832-8c6f-2e78740c16c9](https://www.ft.com/content/5207928a-13e8-4832-8c6f-2e78740c16c9)

生成摘要时出错

---

## 71. 'A Big Fuck You to Big Tech': New Jersey Residents Defeat AI Data Center

**原文标题**: 'A Big Fuck You to Big Tech': New Jersey Residents Defeat AI Data Center

**原文链接**: [https://www.commondreams.org/news/new-brunswick-ai-data-center](https://www.commondreams.org/news/new-brunswick-ai-data-center)

生成摘要时出错

---

## 72. Colorado proposal moves age checks from websites to operating systems

**原文标题**: Colorado proposal moves age checks from websites to operating systems

**原文链接**: [https://www.biometricupdate.com/202602/colorado-moves-age-checks-from-websites-to-operating-systems](https://www.biometricupdate.com/202602/colorado-moves-age-checks-from-websites-to-operating-systems)

生成摘要时出错

---

## 73. What's the best way to learn a new language?

**原文标题**: What's the best way to learn a new language?

**原文链接**: [https://www.bbc.com/future/article/20260220-whats-the-best-way-to-learn-a-new-language](https://www.bbc.com/future/article/20260220-whats-the-best-way-to-learn-a-new-language)

生成摘要时出错

---

## 74. Judge scolds Zuckerberg's team for wearing Meta glasses to social media trial

**原文标题**: Judge scolds Zuckerberg's team for wearing Meta glasses to social media trial

**原文链接**: [https://www.cbsnews.com/news/meta-trial-mark-zuckerberg-ai-glasses/](https://www.cbsnews.com/news/meta-trial-mark-zuckerberg-ai-glasses/)

生成摘要时出错

---

## 75. Git's Magic Files

**原文标题**: Git's Magic Files

**原文链接**: [https://nesbitt.io/2026/02/05/git-magic-files.html](https://nesbitt.io/2026/02/05/git-magic-files.html)

生成摘要时出错

---

## 76. Show HN: 3D Mahjong, Built in CSS

**原文标题**: Show HN: 3D Mahjong, Built in CSS

**原文链接**: [https://voxjong.com](https://voxjong.com)

生成摘要时出错

---

## 77. I put New Zealand behind a $1 paywall

**原文标题**: I put New Zealand behind a $1 paywall

**原文链接**: [https://rename.world/](https://rename.world/)

生成摘要时出错

---

## 78. From 'buy America' to 'bye America', Wall Street exodus gathers pace

**原文标题**: From 'buy America' to 'bye America', Wall Street exodus gathers pace

**原文链接**: [https://www.reuters.com/business/buy-america-bye-america-wall-street-exodus-gathers-pace-2026-02-20/](https://www.reuters.com/business/buy-america-bye-america-wall-street-exodus-gathers-pace-2026-02-20/)

生成摘要时出错

---

## 79. The Four-Color Theorem 1852–1976

**原文标题**: The Four-Color Theorem 1852–1976

**原文链接**: [https://www.ams.org/journals/notices/202603/noti3305/noti3305.html](https://www.ams.org/journals/notices/202603/noti3305/noti3305.html)

生成摘要时出错

---

## 80. Red Robin Died by Spreadsheet. Don't Make the Same Mistake

**原文标题**: Red Robin Died by Spreadsheet. Don't Make the Same Mistake

**原文链接**: [https://garryslist.org/posts/red-robin-died-by-spreadsheet-don-t-make-the-same-mistake](https://garryslist.org/posts/red-robin-died-by-spreadsheet-don-t-make-the-same-mistake)

生成摘要时出错

---

## 81. When etcd crashes, check your disks first

**原文标题**: When etcd crashes, check your disks first

**原文链接**: [https://nubificus.co.uk/blog/etcd/](https://nubificus.co.uk/blog/etcd/)

生成摘要时出错

---

## 82. Postgres Is Your Friend. ORM Is Not

**原文标题**: Postgres Is Your Friend. ORM Is Not

**原文链接**: [https://hypha.pub/postgres-is-your-friend-orm-is-not](https://hypha.pub/postgres-is-your-friend-orm-is-not)

生成摘要时出错

---

## 83. Are compilers deterministic?

**原文标题**: Are compilers deterministic?

**原文链接**: [https://blog.onepatchdown.net/2026/02/22/are-compilers-deterministic-nerd-version/](https://blog.onepatchdown.net/2026/02/22/are-compilers-deterministic-nerd-version/)

生成摘要时出错

---

## 84. Greenland ice melt surges unprecedentedly amid warming

**原文标题**: Greenland ice melt surges unprecedentedly amid warming

**原文链接**: [https://phys.org/news/2026-02-greenland-ice-surges-unprecedentedly.html](https://phys.org/news/2026-02-greenland-ice-surges-unprecedentedly.html)

生成摘要时出错

---

## 85. Trump raises tariffs to 15% day after Supreme Court ruling

**原文标题**: Trump raises tariffs to 15% day after Supreme Court ruling

**原文链接**: [https://www.bbc.co.uk/news/articles/cn8z48xwqn3o](https://www.bbc.co.uk/news/articles/cn8z48xwqn3o)

生成摘要时出错

---

## 86. OpenAI employees raised alarms about Canada shooting suspect months ago

**原文标题**: OpenAI employees raised alarms about Canada shooting suspect months ago

**原文链接**: [https://www.wsj.com/us-news/law/openai-employees-raised-alarms-about-canada-shooting-suspect-months-ago-b585df62](https://www.wsj.com/us-news/law/openai-employees-raised-alarms-about-canada-shooting-suspect-months-ago-b585df62)

生成摘要时出错

---

## 87. DHS pausing TSA PreCheck, Global Entry programs amid funding lapse

**原文标题**: DHS pausing TSA PreCheck, Global Entry programs amid funding lapse

**原文链接**: [https://www.nbcnews.com/news/us-news/dhs-pausing-tsa-precheck-global-entry-programs-funding-lapse-rcna260114](https://www.nbcnews.com/news/us-news/dhs-pausing-tsa-precheck-global-entry-programs-funding-lapse-rcna260114)

生成摘要时出错

---

## 88. Turns Out There Was Voter Fraud in Georgia – By Elon Musk

**原文标题**: Turns Out There Was Voter Fraud in Georgia – By Elon Musk

**原文链接**: [https://newrepublic.com/post/206857/georgia-voter-fraud-elon-musk](https://newrepublic.com/post/206857/georgia-voter-fraud-elon-musk)

生成摘要时出错

---

## 89. Large Language Model Reasoning Failures

**原文标题**: Large Language Model Reasoning Failures

**原文链接**: [https://arxiv.org/abs/2602.06176](https://arxiv.org/abs/2602.06176)

生成摘要时出错

---

## 90. Hackers Expose Age-Verification Software Powering Surveillance Web

**原文标题**: Hackers Expose Age-Verification Software Powering Surveillance Web

**原文链接**: [https://www.therage.co/persona-age-verification/](https://www.therage.co/persona-age-verification/)

生成摘要时出错

---

## 91. Chris Lattner: Claude C Compiler

**原文标题**: Chris Lattner: Claude C Compiler

**原文链接**: [https://www.modular.com/blog/the-claude-c-compiler-what-it-reveals-about-the-future-of-software](https://www.modular.com/blog/the-claude-c-compiler-what-it-reveals-about-the-future-of-software)

生成摘要时出错

---

## 92. I'm #1 on Google thanks to AI bullshit [video]

**原文标题**: I'm #1 on Google thanks to AI bullshit [video]

**原文链接**: [https://www.youtube.com/watch?v=6uKZ84zwJI0](https://www.youtube.com/watch?v=6uKZ84zwJI0)

生成摘要时出错

---

## 93. Altman on AI energy: it also takes 20 years of eating food to train a human

**原文标题**: Altman on AI energy: it also takes 20 years of eating food to train a human

**原文链接**: [https://old.reddit.com/r/singularity/comments/1rb2pzf/sam_altman_people_talk_about_how_much_energy_it/](https://old.reddit.com/r/singularity/comments/1rb2pzf/sam_altman_people_talk_about_how_much_energy_it/)

生成摘要时出错

---

## 94. Fungicide vinclozin causes disease via germline for 20 generations in rats

**原文标题**: Fungicide vinclozin causes disease via germline for 20 generations in rats

**原文链接**: [https://pnas.org/doi/10.1073/pnas.2523071123](https://pnas.org/doi/10.1073/pnas.2523071123)

生成摘要时出错

---

## 95. Volatility: The volatile memory forensic extraction framework

**原文标题**: Volatility: The volatile memory forensic extraction framework

**原文链接**: [https://github.com/volatilityfoundation/volatility3](https://github.com/volatilityfoundation/volatility3)

生成摘要时出错

---

## 96. Instant AI Response

**原文标题**: Instant AI Response

**原文链接**: [https://chatjimmy.ai/](https://chatjimmy.ai/)

生成摘要时出错

---

## 97. The UK tourist with a valid visa detained by ICE for six weeks

**原文标题**: The UK tourist with a valid visa detained by ICE for six weeks

**原文链接**: [https://www.theguardian.com/us-news/2026/feb/21/karen-newton-valid-visa-detained-ice](https://www.theguardian.com/us-news/2026/feb/21/karen-newton-valid-visa-detained-ice)

生成摘要时出错

---

## 98. Online Pebble Development

**原文标题**: Online Pebble Development

**原文链接**: [https://cloudpebble.repebble.com/](https://cloudpebble.repebble.com/)

生成摘要时出错

---

## 99. MeshTNC is a tool for turning consumer grade LoRa radios into KISS TNC compatib

**原文标题**: MeshTNC is a tool for turning consumer grade LoRa radios into KISS TNC compatib

**原文链接**: [https://github.com/datapartyjs/MeshTNC](https://github.com/datapartyjs/MeshTNC)

生成摘要时出错

---

## 100. Claude Code's compaction discards data that's still on disk

**原文标题**: Claude Code's compaction discards data that's still on disk

**原文链接**: [https://github.com/anthropics/claude-code/issues/26771](https://github.com/anthropics/claude-code/issues/26771)

生成摘要时出错

---

