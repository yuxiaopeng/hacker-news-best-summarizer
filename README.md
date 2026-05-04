# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-05-04.md)

*最后自动更新时间: 2026-05-04 20:53:33*
## 1. 三十年来，我每天都听着Phish编程。

**原文标题**: For thirty years I programmed with Phish on, every day

**原文链接**: [https://christophermeiklejohn.com/ai/personal/phish/flow/agents/2026/05/03/rift.html](https://christophermeiklejohn.com/ai/personal/phish/flow/agents/2026/05/03/rift.html)

三十年来，作者每天听着Phish乐队的音乐编程，并在该乐队的音乐与编程的“心流状态”之间建立了一种深刻、几乎密不可分的联系。这种独特的习惯养成使他们在复杂的科技工作中表现出色，从15岁的第一份专业工作，到撰写博士论文和开发生产软件。Phish乐队漫长、渐次展开的即兴演奏，与分布式系统等高要求任务所需的持续专注力完美契合，让他们的工作感觉像一种融合的激情。

这种共生关系培养了巨大的自豪感和创造力，使作者能够完成重要而复杂的项目。Phish始终相伴，如此根深蒂固，以至于作者能一音不差地唱出乐队的独奏。他们感到无比幸运，能用三十年时间做着自己热爱的事情。

然而，最近一次职业转变——转为管理“代理人”（agents），一个以持续的任务切换和短促间断的任务为特征的角色——彻底打破了这种联系。尽管作者仍然热爱Phish，但发现乐队的音乐与新的工作节奏“脱节”；即兴演奏的连贯乐章已无法与他们碎片化的注意力相匹配。

这种变化带来了深深的悲伤，以及失去了定义其职业生涯的创造性心流状态。那种成就感、创造力以及“沉浸其中”的感觉都已不复存在。作者将自己比作一个曾经幸福地沉浸其中、如今却在旁观的人，正在努力思索如何在新的“代理人世界”中找回心流。

---

## 2. 伟大抽象的隐藏成本

**原文标题**: The 'Hidden' Costs of Great Abstractions

**原文链接**: [https://jdgr.net/the-hidden-costs-of-great-abstractions](https://jdgr.net/the-hidden-costs-of-great-abstractions)

文章《伟大抽象的“隐性”成本》认为，虽然抽象简化了计算，但它常常削弱理解，导致软件质量下降。从历史上看，深入了解机器的复杂性至关重要。然而，随着计算能力的增长和进入门槛的降低，开发人员越来越依赖外部库而缺乏完全的理解，这导致了更慢、错误更多的软件的泛滥。

作者认为，大型语言模型（LLMs）的出现进一步降低了这一门槛，使几乎任何人都能生成功能性但质量可能低下的代码。从仅仅够用的解决方案中辨别出真正优秀的解决方案需要专业知识，这好比区分黄金和黄铁矿。尽管“足够”有时可以接受（就像奇迹面包），但它往往缺乏真正工艺的品质。

作者透露了他们撰写这篇评论的个人动机：自2025年7月以来深感沮丧和失业，身体受伤使其无法从事体力劳动，这加剧了他们的困境。尽管对底层计算有着终身的热情，并在求职、技能适应和人脉建设方面付出了巨大努力，他们仍形容自己的职业生涯枯竭了。文章最后以寻求联系和机会的呼吁作结。

---

## 3. 恶意连接：全球电信遭秘密监控者滥用

**原文标题**: Bad Connection: Global telecom exploitation by covert surveillance actors

**原文链接**: [https://citizenlab.ca/research/uncovering-global-telecom-exploitation-by-covert-surveillance-actors/](https://citizenlab.ca/research/uncovering-global-telecom-exploitation-by-covert-surveillance-actors/)

本报告题为《恶意连接》，揭露了秘密监控者如何利用全球电信网络中的系统性漏洞进行间谍活动。公民实验室（Citizen Lab）于2024年末发起的一项调查，揭露了两起独立的商业监控供应商（CSV）行动，旨在针对包括一名“特级贵宾”（VVIP）高管在内的知名人士，并利用了Cellusys提供的情报。

关键发现揭示了多向量监控技术，它结合了3G和4G信令协议，并通过恶意短信直接利用设备漏洞。其中一项行动通过发送隐藏的SIM卡命令来提取位置数据，有效地将设备变成了一个跟踪信标。这些老练的攻击者利用定制工具来伪造运营商身份、操纵信令协议，并通过包括英国、以色列和中国在内的众多国家的网络在全球范围内路由流量。持续的行动活动，以及多年来重复使用的运营商标识符，凸显了他们的先进能力。运营商间提供商薄弱的运行安全，允许监控消息通过受信任的网络路径传输，从而助长了这些攻击。

该报告强调，这些漏洞并非错误，而是SS7（3G）和Diameter（4G/5G）协议固有的设计缺陷，它们缺乏认证和加密等基本安全机制。尽管Diameter的设计更为强大，但运营商常常未能实施这些保护措施，而是依赖于过时的信任模型。攻击者还通过第三方提供商获得间接访问权限，并利用“组合附着”（combined attach）功能在3G和4G网络之间枢转攻击。这种复杂的环境使得资源充足的与国家相关的间谍服务机构和商业监控供应商（CSV）能够将电信网络武器化，用于全球监控。

---

## 4. PyInfra 3.8.0

**原文标题**: PyInfra 3.8.0

**原文链接**: [https://github.com/pyinfra-dev/pyinfra/releases/tag/v3.8.0](https://github.com/pyinfra-dev/pyinfra/releases/tag/v3.8.0)

PyInfra 3.8.0 是一个重要版本，标志着全面转向语义化版本控制，并带来了大量的修复和改进。

主要亮点包括：

*   **核心API：** 与Click解耦，增强了灵活性，并修复了字符串格式化问题。
*   **安全性：** 扩大了在操作和连接器中用户输入的引用范围，以防止命令注入，并在命令构建中引用了不可信的值。
*   **新增 Facts：** 引入了关于监听`Ports`、`AuthorizedKeys`的详细信息，完整的`Crontab`环境变量、`GpgKeyrings`、`Server.Processes`，全面的`Docker`详细信息（版本、容器、镜像、网络）、`ZfsDatasets`，以及`AptSources`的deb822格式支持。
*   **新增操作：** 增加了`files.unarchive`、`git.repo`的深度支持、`files.download`的限速、`server.kill`、`gpg`操作，以及广泛的`docker`支持，包括自定义命令、`login/logout`、`compose`和`build`操作。`apt.packages`现在支持`purge`选项。
*   **连接器：** SSH改进包括更好的配置文件解析，通过`ProxyJump`遵守`ConnectTimeout`，支持`IdentityAgent`指令，以及更清晰的`askpass`生成错误。
*   **底层改进：** 支持Paramiko v4、`uv`集成、事实和操作模块的懒加载、使用`dzdo`进行权限提升，以及`config.INHERIT_ENV`选项以传递本地环境变量。

此版本侧重于稳定性、安全性以及显著扩展的功能，并得到了众多开发者的贡献。

---

## 5. 隐匿安全并非不好

**原文标题**: Security through obscurity is not bad

**原文链接**: [https://mobeigi.com/blog/security/security-through-obscurity-is-not-bad/](https://mobeigi.com/blog/security/security-through-obscurity-is-not-bad/)

本文挑战了“通过模糊实现安全是糟糕的”这一普遍观念，转而认为“*仅仅*通过模糊实现安全是糟糕的”，但“作为额外层面的通过模糊实现安全是好的”。作者认为，模糊性（指使应用程序内部工作原理不那么可见）是深度防御策略中一个有价值的组成部分。

将其比作将备用钥匙藏在门垫下，作者解释说，模糊性增加了恶意行为者的成本和时间，使他们更有可能放弃。以下几个现实世界的例子说明了这一点：
1.  **WordPress表前缀：** 更改默认前缀使作者的网站免受已知SQL注入漏洞的影响，因为标准查询会失败。
2.  **CSGO调试符号：** Valve有意从游戏二进制文件中去除调试符号，以阻碍作弊程序的开发，这表明了其在提高逆向工程门槛方面的有效性。
3.  **混淆代码：** 恶意软件、Google reCAPTCHA、Netflix DRM和Riot Vanguard都使用代码混淆来保护敏感逻辑，并使人类和自动化工具更难分析。

针对“AI使模糊性过时”的论点，作者承认AI的能力，但强调去混淆仍然是一个缓慢、昂贵且常常不确定的过程，特别是对于复杂系统而言。一个关于LLM花费300美元和4.5小时解决一个CTF挑战的个人轶事，突出了模糊性在增加攻击者开销方面的持续价值。

总之，文章倡导一种细致入微的理解：通过模糊实现安全可以有效地作为一个有益的额外层面，使攻击变得更昂贵、更耗时，而不是其本身存在缺陷。

---

## 6. 开源不意味着开放社区

**原文标题**: Open source does not imply open community

**原文链接**: [https://blog.feld.me/posts/2026/04/open-source-does-not-imply-open-community/](https://blog.feld.me/posts/2026/04/open-source-does-not-imply-open-community/)

文章认为，现代对开源的解读，深受GitHub等平台的影响，已将其从一个简单的代码共享模式，转变为维护者的“无偿工作”。

历史上，开源涉及通过FTP服务器、电子邮件，可能还有邮件列表来共享代码，而“社区”开销、政治或正式管理结构极少。然而，作者认为，GitHub的兴起引入了类似企业的责任，例如管理问题、拉取请求、路线图、利益相关者，甚至“办公室政治”和行为准则，而所有这些都没有报酬。这种转变带来了巨大的压力，导致维护者精疲力尽，因为他们要对一个要求苛刻的“社区”负责，而这个社区往往缺乏耐心或不尊重他们的时间和方向。

作者提倡回归旧模式，特别是对于个人或小型团队项目。他们建议禁用问题追踪器和拉取请求，使用裸Git服务器，并与少数几个值得信赖的人（或独自一人）合作，以保持控制，防止“陌生人入侵你的空间”。核心信息是，开源并不意味着必须进行开放开发或管理一个苛刻的社区；它关乎按照自己的意愿编写和共享代码，摆脱被视为“科技孵化器和日托”运作的负担。

---

## 7. 各主要 Chromium 浏览器落后多远？

**原文标题**: How far behind is each major Chromium browser?

**原文链接**: [https://chromium-drift.pages.dev/](https://chromium-drift.pages.dev/)

本文解释了为什么浏览器Chromium版本滞后意义重大。首先，这使用户面临已在较新Chromium版本中修复的已知安全漏洞，从而使他们成为攻击者主动利用的目标。此外，用户会错过最新的Web API和功能，这可能导致网站兼容性问题。文章最后鼓励用户检查自己浏览器的Chromium版本。

---

## 8. Microsoft Edge stores all passwords in memory in clear text, even when unused

**原文标题**: Microsoft Edge stores all passwords in memory in clear text, even when unused

**原文链接**: [https://twitter.com/L1v1ng0ffTh3L4N/status/2051308329880719730](https://twitter.com/L1v1ng0ffTh3L4N/status/2051308329880719730)

The provided content does not contain an article discussing Microsoft Edge's password storage or any related security vulnerabilities. Instead, the content is a standard error message from x.com (formerly Twitter) indicating that JavaScript is disabled in the user's browser. It prompts the user to enable JavaScript or switch to a supported browser to continue using the platform, followed by links to various policy pages and a copyright notice. Therefore, it is not possible to summarize an article about Microsoft Edge's password handling based on the text provided.

---

## 9. How Monero's proof of work works

**原文标题**: How Monero's proof of work works

**原文链接**: [https://blog.alcazarsec.com/tech/posts/how-moneros-proof-of-work-works](https://blog.alcazarsec.com/tech/posts/how-moneros-proof-of-work-works)

生成摘要时出错

---

## 10. A network smuggling Starlink tech into Iran to beat internet blackout

**原文标题**: A network smuggling Starlink tech into Iran to beat internet blackout

**原文链接**: [https://www.bbc.com/news/articles/cvgzk91leweo](https://www.bbc.com/news/articles/cvgzk91leweo)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 2 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 3 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 4 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 5 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 6 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 7 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 8 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 9 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 10 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 11 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 12 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 13 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 14 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 15 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 16 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 17 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 18 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 19 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 20 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 21 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 22 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 23 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 24 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 25 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 26 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 27 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 28 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 29 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 30 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 31 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 32 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 33 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 34 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 35 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 36 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 37 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 38 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 39 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 40 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 41 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 42 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 43 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 44 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 45 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 46 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 47 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 48 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 49 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 50 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 51 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 52 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 53 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 54 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 55 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 56 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 57 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 58 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 59 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 60 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 61 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 62 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 63 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 64 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 65 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 66 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 67 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 68 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 69 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 70 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 71 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 72 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 73 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 74 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 75 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 76 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 77 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 78 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 79 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 80 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 81 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 82 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 83 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 84 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 85 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 86 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 87 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 88 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 89 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 90 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 91 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 92 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 93 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 94 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 95 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 96 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 97 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 98 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 99 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 100 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 101 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 102 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 103 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 104 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 105 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 106 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 107 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 108 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 109 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 110 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 111 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 112 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 113 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 114 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 115 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 116 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 117 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 118 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 119 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 120 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 121 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 122 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 123 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 124 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 125 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 126 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 127 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 128 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 129 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 130 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 131 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 132 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 133 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 134 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 135 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 136 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 137 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 138 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 139 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 140 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 141 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 142 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 143 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 144 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 145 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 146 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 147 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 148 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 149 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 150 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 151 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 152 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 153 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 154 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 155 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 156 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 157 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 158 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 159 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 160 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 161 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 162 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 163 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 164 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 165 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 166 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 167 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 168 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 169 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 170 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 171 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 172 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 173 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 174 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 175 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 176 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 177 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 178 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
