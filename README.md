# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-07-10.md)

*最后自动更新时间: 2026-07-10 20:47:25*
## 1. 我的一次性邮箱黑名单把我屏蔽了。

**原文标题**: My burner email blocklist blocked me

**原文链接**: [https://benjamin.piouffle.com/blog/burner-email-blocklists/](https://benjamin.piouffle.com/blog/burner-email-blocklists/)

作者在2018年创建了旨在阻止“阅后即焚”邮件域名的Burnex Elixir包。然而，他最近在使用Proton Mail别名时，却发现自己也被类似的系统拦截了。这一经历，加上不断发展的隐私工具，促使他撤回了此前的建议：他不再主张在注册时系统性地阻止增强隐私的邮件服务。

他强调了“阅后即焚邮箱”（如yopmail.fr等公共的、短时存在的收件箱）和“邮件别名”（如Proton Mail、Firefox Relay或Apple Hide My Email等服务提供的永久、可控的转发地址）之间的关键区别。阅后即焚邮箱用于一次性验证，而邮件别名是限制跨站追踪、减少垃圾邮件和帮助用户识别数据泄露的隐私工具。阻止别名会惩罚那些注重隐私的用户。

文章指出，阻止列表对那些有决心的滥用者无效，他们可以轻易地通过Gmail别名、自定义域名或专用工具绕过这些列表。此类列表仅能减缓低成本机器人的速度，却不公平地拒绝了合法用户。一般来说，邮件验证只证明一个地址能够接收邮件，而不能证明账户的真实性。

作者现在建议改进阻止列表：它们可以作为更广泛信任评分的信号，但必须区分真正的公共共享收件箱和个人别名提供商。他已向广泛使用的`wesbos/burner-email-providers`列表提出了这种区分建议，以鼓励更好的文档和实践。他自己的Burnex项目已于2026年弃用，所有权也已转让。

---

## 2. 瑞安航空乘客空中引擎故障后被吸向破窗

**原文标题**: Ryanair Passenger Sucked Toward Broken Window After Midair Engine Failure

**原文链接**: [https://simpleflying.com/ryanair-thessaloniki-diversion-window-damage/](https://simpleflying.com/ryanair-thessaloniki-diversion-window-damage/)

瑞安航空一架波音737-800客机（由马耳他航空运营，注册号9H-QEU），执飞从塞萨洛尼基（SKG）飞往梅明根（FMM）的FR1879航班，在一个周五起飞后不久遭遇了严重的发动机故障。发动机碎片击碎了一扇客舱窗户，据报道导致一名男性乘客颈部受伤，其头部和肩膀部分被吸出破裂的窗外。

该飞机当时已爬升至约16,000英尺（约4877米）的高度，飞行员宣布紧急状态后，安全返回塞萨洛尼基。在耗尽多余燃油着陆后，紧急服务人员已在现场待命，客舱内的氧气面罩也已全部弹出。

受伤乘客立即得到了医疗救治，有关部门已对此次事件展开调查。瑞安航空证实了这一事件，并安排了备用飞机，导致前往梅明根的乘客以及返程航班的乘客行程延误约四小时。

文章指出此类事件的罕见性，并提及了过去的类似事故，例如2018年西南航空1380航班的致命客舱窗户破裂事故，以及1990年英国航空一架飞机机长部分被吸出驾驶舱但幸存的事件。

---

## 3. HN作品：LastShelf – 家庭文件、账单及联系方式应急地图

**原文标题**: Show HN: LastShelf – an emergency map of your family's documents bills& contacts

**原文链接**: [https://www.lastshelf.ai/](https://www.lastshelf.ai/)

LastShelf 被推出为一款“应急地图”，旨在集中管理并方便获取一个家庭的重要文件、账单和联系人。该服务旨在通过连接各种来源，发现重要的账单和账户详情。此外，LastShelf 还会引导用户整理个人文件、联系人以及个人独有的具体指示，确保这些关键信息得到妥善组织和随时可取用，尤其是在紧急情况下。

---

## 4. 还有其他人收到模糊的 GitHub 勒索通知吗？

**原文标题**: Anyone else get a vague GitHub shakedown notice?

**原文链接**: [https://lists.osgeo.org/pipermail/qgis-developer/2026-July/068430.html](https://lists.osgeo.org/pipermail/qgis-developer/2026-July/068430.html)

Greg Troxel 收到了一封他称之为“模糊的 GitHub 收费威胁通知”的电子邮件，该邮件似乎是合法的（来自 GitHub 经由 Sendgrid 发送，并有 DKIM 签名）。邮件威胁要开始向他收取 GitHub “代码质量”服务的费用，该服务将于2026年7月20日全面推出。

该通知详细说明了一种定价模式，包括基本订阅费加上按使用量计费：每位活跃提交者每月10美元的企业版访问许可证，用于AI驱动功能（如Copilot代码审查）的按使用量计费的AI点数，以及用于确定性分析的GitHub Actions分钟数。通知建议收件人在7月20日前评估仓库覆盖范围并禁用仓库上的代码质量功能，以避免产生费用。

Troxel 从未注册过付费的GitHub服务，也从未提供过账单信息，因此他感到困惑，因为邮件还错误地声称他收到此邮件是因为他是“GitHub 赞助者”的一部分，但他否认了这一点。他最近离开了与他GitHub账户关联的其他已解散的组织。

他质疑QGIS是否正在使用“代码质量”服务，以及他与该项目的关联（例如克隆仓库、提交问题）是否导致他收到了此通知。Troxel 询问其他QGIS开发者是否收到了类似的邮件，寻求澄清此通知是否混乱或“暗藏玄机”，并表达了对潜在意外账单的担忧。

---

## 5. JEPA 注释版

**原文标题**: The Annotated JEPA

**原文链接**: [https://elonlit.com/scrivings/the-annotated-jepa/](https://elonlit.com/scrivings/the-annotated-jepa/)

JEPA详解：本文介绍了Yann LeCun提出的自监督学习范式——联合嵌入预测架构（JEPA），旨在无需标签即可构建世界模型，避免模型崩溃，并忽略无关细节。其核心原则是*在表征空间进行预测*，通过要求上下文编码预测目标表征，迫使模型学习语义和结构特征。

JEPA由一个上下文编码器（$f_\theta$）、一个目标编码器（$f_{\bar\theta}$）和一个预测器（$g_\phi$）组成，旨在最小化预测误差$D(\widehat{s}_y, s_y)$。预测表征而非像素可以防止模型将容量浪费在高熵噪声上，从而专注于有意义的信息。

“崩溃”到平凡解是一个关键挑战，I-JEPA（图像实例化）通过非对称设计解决了这一问题。上下文编码器和预测器通过梯度下降更新，而目标编码器的权重是上下文编码器权重的指数移动平均（EMA）。这种滞后防止了协同适应，迫使上下文编码器学习真正的预测特征。

对于I-JEPA，图像被分解为补丁标记。上下文是一个大的可见块，而目标是其他位置的几个较小的、被遮蔽的块。关键在于，目标编码器处理*完整图像*，并且遮蔽发生在其*输出表征*上，这确保了高语义质量。该架构对两个编码器（其中教师编码器通过EMA更新）使用视觉Transformer，并对预测器使用一个较小的Transformer。损失函数是预测的目标补丁嵌入与实际目标补丁嵌入之间的均方误差。

---

## 6. 德州ICE杀人案疑云密布：议员称目击者被逼“自愿遣返”

**原文标题**: Texas ICE Killing Darkens: Rep Says Witnesses Were Pressured to Self-Deport

**原文链接**: [https://newrepublic.com/article/212900/texas-ice-killing-darkens-rep-says-witnesses-pressured-self-deport](https://newrepublic.com/article/212900/texas-ice-killing-darkens-rep-says-witnesses-pressured-self-deport)

在休斯顿的一次交通截停中，一名联邦特工开枪射杀了洛伦佐·萨尔加多·阿拉乌霍 (Lorenzo Salgado Araujo)，他是一名无证墨西哥裔男子。尽管国土安全部 (DHS) 声称萨尔加多·阿拉乌霍“将车辆武器化”并试图撞击一名警官，但迄今未提供任何证据或视频录像来支持这一说法。

至关重要的是，另外三名男子——萨尔加多·阿拉乌霍的兄弟和两名雇员——当时也在车内，随后被移民和海关执法局 (ICE) 拘留。LULAC 首席执行官兼这些家属的代表胡安·普罗阿尼奥 (Juan Proaño) 指控，这三名关键目击者目前正受到移民官员的施压，要求他们同意“自行递解出境”。普罗阿尼奥和刑事司法改革专家拉德利·巴尔科 (Radley Balko) 认为，这是国土安全部企图压制他们的证词并阻止真相浮出水面，并将其与 ICE 此前压制证人的案例相提并论。

52岁的萨尔加多·阿拉乌霍已在美国居住了35年，拥有一家建筑企业，抚养着美国公民的儿子，并且正在积极寻求法律保护，这与官方将其描述为暴力抵抗的说法相悖。他的家人甚至为他准备了一旦被捕就服从的计划。

文章批评ICE缺乏透明度，指出他们尚未说明这些目击者的状况。文章最后强调迫切需要全面公开目击者的证词，并表示担忧，随着ICE递解出境人数的增加和准军事力量使用的升级，事件的全部真相可能被刻意隐瞒。

---

## 7. 政府想吓阻美国人分享新闻。

**原文标题**: The government wants to scare Americans out of sharing the news

**原文链接**: [https://freedom.press/issues/the-government-wants-to-scare-americans-out-of-sharing-the-news/](https://freedom.press/issues/the-government-wants-to-scare-americans-out-of-sharing-the-news/)

该文章声称，美国政府正在采取一项“令人不安的新举措”来压制新闻：通过调查美国公民在社交媒体上分享新闻报道中的信息，旨在恐吓公众并限制新闻业的影响力，同时避免直接审查新闻编辑室。

一个主要例子是Paigelynne Gonyea，她因一篇Instagram帖子指明了移民及海关执法局（ICE）探员Jonathan Ross的身份而遭到联邦探员的盘问。该帖子援引了《明尼苏达星论坛报》指认Ross为Renee Good枪手的报道。探员要求Gonyea删除该帖子，并签署一份承认可能因威胁联邦官员而面临刑事起诉的文件。尽管国土安全部（DHS）声称Gonyea发布了Ross的家庭住址，她对此予以否认，而且探员向她展示的帖子中也并未包含该地址。

新闻自由基金会（FPF）已提交了一项《信息自由法》（FOIA）请求，以调查这些调查是否仅仅针对那些转发新闻内容的个人。文章强调，联邦政府声称指认或批评官员是非法的说法，与《第一修正案》对发布真实、合法获取信息的明确保护相矛盾。

这种策略使政府能够阻止公众讨论，损害新闻业，并避免与更有能力通过法律手段反击的媒体机构直接对抗。文章还令人担忧，政府可能正在悄悄地胁迫科技平台删除提及新闻报道的帖子，从而使这种形式的审查在很大程度上隐形。

作者总结道，这些策略，无论是直接的还是间接的，都从根本上威胁着新闻自由，并指出如果人们不敢分享和讨论追究权力责任的新闻，那么新闻自由就毫无意义。

---

## 8. Reframing smart glasses as 'pervert glasses'

**原文标题**: Reframing smart glasses as 'pervert glasses'

**原文链接**: [https://this.weekinsecurity.com/reframing-smart-glasses-as-pervert-glasses/](https://this.weekinsecurity.com/reframing-smart-glasses-as-pervert-glasses/)

生成摘要时出错

---

## 9. A new way to reflect on how you use Claude

**原文标题**: A new way to reflect on how you use Claude

**原文链接**: [https://www.anthropic.com/news/reflect-with-claude](https://www.anthropic.com/news/reflect-with-claude)

Anthropic is launching a new beta feature on July 9, 2026, designed to help Claude users reflect on and refine their AI usage. This "reflection" tool aims to answer questions about effective AI integration into daily life, such as how often and for what tasks AI is best suited.

Accessible through a dashboard in Claude's web and desktop app settings, the feature summarizes usage patterns, key topics, and task types over periods up to 12 months. It visualizes peak usage times and activities, with future updates to include time spent. The tool also prompts users with periodic reflective questions and allows them to set quiet hours or schedule breaks from Claude.

It integrates the "4D AI Fluency Framework" (Delegation, Description, Discernment, Diligence) to help users build AI skills, offering insights into their collaboration style and practical suggestions like using Projects for ongoing work. Privacy is a core focus; the tool excludes incognito chats, underlying files from connected tools, and all conversations related to health integrations. Sensitive topics appear only at a high level, and insights remain private, not used for other purposes.

The reflection feature is available in beta for Free, Pro, and Max users who have Claude's Memory turned on, with future support for Cowork conversations.

---

## 10. Computation as a universal and fundamental concept

**原文标题**: Computation as a universal and fundamental concept

**原文链接**: [https://ergo.org/courses/computation-as-a-universal-and-fundamental-concept](https://ergo.org/courses/computation-as-a-universal-and-fundamental-concept)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 2 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 3 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 4 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 5 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 6 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 7 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 8 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 9 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 10 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 11 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 12 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 13 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 14 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 15 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 16 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 17 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 18 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 19 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 20 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 21 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 22 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 23 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 24 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 25 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 26 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 27 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 28 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 29 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 30 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 31 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 32 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 33 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 34 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 35 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 36 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 37 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 38 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 39 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 40 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 41 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 42 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 43 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 44 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 45 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 46 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 47 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 48 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 49 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 50 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 51 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 52 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 53 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 54 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 55 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 56 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 57 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 58 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 59 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 60 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 61 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 62 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 63 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 64 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 65 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 66 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 67 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 68 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 69 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 70 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 71 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 72 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 73 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 74 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 75 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 76 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 77 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 78 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 79 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 80 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 81 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 82 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 83 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 84 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 85 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 86 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 87 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 88 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 89 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 90 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 91 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 92 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 93 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 94 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 95 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 96 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 97 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 98 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 99 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 100 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 101 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 102 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 103 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 104 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 105 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 106 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 107 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 108 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 109 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 110 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 111 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 112 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 113 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 114 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 115 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 116 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 117 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 118 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 119 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 120 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 121 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 122 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 123 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 124 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 125 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 126 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 127 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 128 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 129 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 130 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 131 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 132 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 133 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 134 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 135 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 136 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 137 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 138 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 139 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 140 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 141 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 142 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 143 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 144 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 145 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 146 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 147 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 148 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 149 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 150 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 151 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 152 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 153 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 154 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 155 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 156 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 157 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 158 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 159 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 160 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 161 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 162 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 163 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 164 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 165 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 166 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 167 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 168 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 169 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 170 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 171 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 172 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 173 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 174 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 175 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 176 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 177 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 178 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 179 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 180 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 181 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 182 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 183 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 184 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 185 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 186 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 187 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 188 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 189 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 190 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 191 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 192 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 193 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 194 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 195 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 196 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 197 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 198 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 199 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 200 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 201 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 202 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 203 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 204 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 205 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 206 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 207 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 208 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 209 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 210 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 211 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 212 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 213 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 214 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 215 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 216 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 217 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 218 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 219 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 220 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 221 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 222 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 223 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 224 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 225 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 226 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 227 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 228 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 229 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 230 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 231 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 232 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 233 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 234 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 235 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 236 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 237 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 238 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 239 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 240 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 241 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 242 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 243 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 244 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 245 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
