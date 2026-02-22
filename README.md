# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-02-22.md)

*最后自动更新时间: 2026-02-22 19:57:05*
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

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 2 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 3 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 4 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 5 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 6 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 7 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 8 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 9 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 10 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 11 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 12 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 13 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 14 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 15 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 16 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 17 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 18 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 19 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 20 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 21 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 22 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 23 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 24 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 25 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 26 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 27 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 28 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 29 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 30 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 31 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 32 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 33 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 34 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 35 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 36 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 37 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 38 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 39 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 40 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 41 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 42 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 43 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 44 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 45 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 46 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 47 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 48 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 49 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 50 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 51 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 52 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 53 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 54 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 55 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 56 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 57 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 58 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 59 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 60 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 61 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 62 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 63 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 64 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 65 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 66 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 67 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 68 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 69 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 70 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 71 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 72 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 73 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 74 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 75 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 76 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 77 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 78 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 79 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 80 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 81 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 82 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 83 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 84 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 85 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 86 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 87 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 88 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 89 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 90 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 91 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 92 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 93 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 94 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 95 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 96 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 97 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 98 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 99 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 100 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 101 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 102 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 103 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 104 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
| 105 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 106 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 107 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 108 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
