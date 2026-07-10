# Hacker News 热门文章摘要 (2026-07-10)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

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

## 11. Ways to think about token pricing

**原文标题**: Ways to think about token pricing

**原文链接**: [https://www.ben-evans.com/benedictevans/2026/7/9/ways-to-think-about-token-pricing](https://www.ben-evans.com/benedictevans/2026/7/9/ways-to-think-about-token-pricing)

生成摘要时出错

---

## 12. Show HN: Runloom – Go-style coroutines for Python free-threaded

**原文标题**: Show HN: Runloom – Go-style coroutines for Python free-threaded

**原文链接**: [https://github.com/robertsdotpm/runloom](https://github.com/robertsdotpm/runloom)

生成摘要时出错

---

## 13. Creatine doesn't just build muscle. It may also help fight cancer

**原文标题**: Creatine doesn't just build muscle. It may also help fight cancer

**原文链接**: [https://www.sciencedaily.com/releases/2026/07/260701015237.htm](https://www.sciencedaily.com/releases/2026/07/260701015237.htm)

生成摘要时出错

---

## 14. The internet does not want readers. It wants livestock

**原文标题**: The internet does not want readers. It wants livestock

**原文链接**: [https://grumpywelshman.com/the-internet-doesnt-want-readers-it-wants-livestock/](https://grumpywelshman.com/the-internet-doesnt-want-readers-it-wants-livestock/)

生成摘要时出错

---

## 15. Just Pay the Subscription

**原文标题**: Just Pay the Subscription

**原文链接**: [https://www.uncommonapps.nyc/p/just-pay-the-subscription](https://www.uncommonapps.nyc/p/just-pay-the-subscription)

生成摘要时出错

---

## 16. You're Not a Better Engineer Because You Type Git Commands by Hand

**原文标题**: You're Not a Better Engineer Because You Type Git Commands by Hand

**原文链接**: [https://www.minid.net/2026/7/10/ai-works-for-me](https://www.minid.net/2026/7/10/ai-works-for-me)

生成摘要时出错

---

## 17. A Roomba recorded a woman on the toilet. How did screenshots end up on Facebook? (2022)

**原文标题**: A Roomba recorded a woman on the toilet. How did screenshots end up on Facebook? (2022)

**原文链接**: [https://www.technologyreview.com/2022/12/19/1065306/roomba-irobot-robot-vacuums-artificial-intelligence-training-data-privacy/](https://www.technologyreview.com/2022/12/19/1065306/roomba-irobot-robot-vacuums-artificial-intelligence-training-data-privacy/)

生成摘要时出错

---

## 18. Iran, Not Trump, Is in Control of This War

**原文标题**: Iran, Not Trump, Is in Control of This War

**原文链接**: [https://www.theatlantic.com/ideas/2026/07/iran-controls-war-trump/687848/](https://www.theatlantic.com/ideas/2026/07/iran-controls-war-trump/687848/)

生成摘要时出错

---

## 19. China may restrict foreign access to Chinese open-source AI models

**原文标题**: China may restrict foreign access to Chinese open-source AI models

**原文链接**: [https://www.reuters.com/technology/artificial-intelligence/china-weighs-silicon-curtain-around-sought-after-ai-models-2026-07-08/](https://www.reuters.com/technology/artificial-intelligence/china-weighs-silicon-curtain-around-sought-after-ai-models-2026-07-08/)

生成摘要时出错

---

## 20. Star Just Ate a Planet, and It's Not Done Yet

**原文标题**: Star Just Ate a Planet, and It's Not Done Yet

**原文链接**: [https://www.nytimes.com/2026/07/09/science/space/planetary-engulfment-hungry-star.html](https://www.nytimes.com/2026/07/09/science/space/planetary-engulfment-hungry-star.html)

生成摘要时出错

---

## 21. Show HN: Reviving my 2001 college band with AI

**原文标题**: Show HN: Reviving my 2001 college band with AI

**原文链接**: [https://www.fadingmaize.com](https://www.fadingmaize.com)

生成摘要时出错

---

## 22. Madison Sq Garden database tracks hundreds. Labels "LGBTQIA," & low/high "risk."

**原文标题**: Madison Sq Garden database tracks hundreds. Labels "LGBTQIA," & low/high "risk."

**原文链接**: [https://www.wired.com/story/madison-square-garden-celebrity-database-surveillance/](https://www.wired.com/story/madison-square-garden-celebrity-database-surveillance/)

生成摘要时出错

---

## 23. Samsung chip division's 1-year profit beat past 40 years of profits, combined

**原文标题**: Samsung chip division's 1-year profit beat past 40 years of profits, combined

**原文链接**: [https://www.tomshardware.com/tech-industry/samsungs-chip-division-expects-to-out-earn-its-entire-40-year-history-in-2026](https://www.tomshardware.com/tech-industry/samsungs-chip-division-expects-to-out-earn-its-entire-40-year-history-in-2026)

生成摘要时出错

---

## 24. Show HN: Devthropology – Better Insights for GitHub Repos

**原文标题**: Show HN: Devthropology – Better Insights for GitHub Repos

**原文链接**: [https://devthropology.com/demo](https://devthropology.com/demo)

生成摘要时出错

---

## 25. You paid me, a long-time Linux user, to use Windows 11 exclusively for a month

**原文标题**: You paid me, a long-time Linux user, to use Windows 11 exclusively for a month

**原文链接**: [https://www.osnews.com/story/145459/you-paid-me-a-long-time-linux-user-to-use-windows-11-exclusively-for-a-month-heres-how-it-went/](https://www.osnews.com/story/145459/you-paid-me-a-long-time-linux-user-to-use-windows-11-exclusively-for-a-month-heres-how-it-went/)

生成摘要时出错

---

## 26. NASA SpaceWASM – A flight-compliant WebAssembly interpreter

**原文标题**: NASA SpaceWASM – A flight-compliant WebAssembly interpreter

**原文链接**: [https://github.com/nasa/spacewasm](https://github.com/nasa/spacewasm)

生成摘要时出错

---

## 27. 45% of Enthusiasts 'Seriously Considering' Leaving Sony for PC

**原文标题**: 45% of Enthusiasts 'Seriously Considering' Leaving Sony for PC

**原文链接**: [https://www.pushsquare.com/news/2026/07/ps5-has-put-a-dampener-on-gaming-45percent-of-enthusiasts-seriously-considering-leaving-sony-for-pc](https://www.pushsquare.com/news/2026/07/ps5-has-put-a-dampener-on-gaming-45percent-of-enthusiasts-seriously-considering-leaving-sony-for-pc)

生成摘要时出错

---

## 28. Proton AG Services is currently experiencing some issues

**原文标题**: Proton AG Services is currently experiencing some issues

**原文链接**: [https://status.proton.me/incidents/01lxtcq155lc](https://status.proton.me/incidents/01lxtcq155lc)

生成摘要时出错

---

## 29. Open Source Barware: free, local-first bar inventory software (GPLv3)

**原文标题**: Open Source Barware: free, local-first bar inventory software (GPLv3)

**原文链接**: [https://opensourcebarware.com](https://opensourcebarware.com)

生成摘要时出错

---

