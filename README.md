# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2025-12-13.md)

*最后自动更新时间: 2025-12-13 19:44:44*
## 1. 苹果已锁定我的Apple ID，我申诉无门。求助

**原文标题**: Apple has locked my Apple ID, and I have no recourse. A plea for help

**原文链接**: [https://hey.paris/posts/appleid/](https://hey.paris/posts/appleid/)

资深苹果用户兼开发者巴黎（Paris）的Apple ID被永久锁定，导致价值超过3万美元的设备形同“砖块”，并失去对数十年数据、已购软件和其专业数字身份的访问权限。此事源于他试图兑换一张购自大型实体零售商的500美元苹果礼品卡，但兑换失败，并被怀疑可能已被盗用。苹果随后以违反“Apple媒体服务条款和条件”为由禁用了其账户。

尽管苹果声称受影响的仅是媒体服务，但巴黎（Paris）因认证错误，已无法使用iMessage、退出iCloud或访问关键的苹果支持服务。数TB的家庭照片和信息历史记录均无法访问，且目前没有实际方法可以恢复。

苹果支持部门态度冷漠，毫无帮助，拒绝提供禁用的具体原因或升级处理该案件。他们甚至建议创建一个新的Apple ID，但巴黎（Paris）认为这是一个技术上灾难性的解决方案，并可能导致进一步的封禁，尤其考虑到他作为苹果开发者以及苹果编程技术书籍作者的专业身份。

作为近30年的忠实用户和苹果开发者社区的知名人物，巴黎（Paris）认为一次自动化的欺诈标记触发了“核打击式”的回应。他正在恳求人工审查他的案件，以恢复他的数字生活，强调了他绝望的处境以及由此造成的巨大个人和职业损失。

---

## 2. 厌倦智能电视？你的最佳选择。

**原文标题**: Sick of smart TVs? Here are your best options

**原文链接**: [https://arstechnica.com/gadgets/2025/12/the-ars-technica-guide-to-dumb-tvs/](https://arstechnica.com/gadgets/2025/12/the-ars-technica-guide-to-dumb-tvs/)

对智能电视的隐私问题、广告和复杂性感到沮丧？本文提供了一些替代方案，以获得更简单的观看体验。首要建议是将智能电视离线，并连接一个Apple TV机顶盒。这种设置用苹果更简洁、无广告的tvOS取代了电视内置的侵入性操作系统，确保了更好的隐私、可靠性和易用性，同时仍可访问先进的显示技术。用户可以通过路由器阻止电视的互联网访问，或者在Google TV上使用“基本电视”模式。

对于那些寻求真正“非智能”显示器的人来说，像Emerson、Westinghouse和Sceptre这样的品牌提供非智能型号，不过这些通常在图像和音质方面有所妥协，缺乏高端功能。在亚马逊上搜索也可以帮助找到这些选项。

替代的显示解决方案包括投影仪，它们提供大屏幕尺寸，但需要昏暗的环境；以及电脑显示器，它们提供详细的规格和高刷新率，尤其适用于小屏幕，但缺乏电视调谐器和通常没有内置扬声器。数字标牌显示器经久耐用，但往往更昂贵，且不适合家庭娱乐优化。

为了驱动这些非智能显示器，用户可以连接笔记本电脑或手机等设备。笔记本电脑提供广泛的自定义选项、广泛的流媒体服务访问（尽管4K/HDR流媒体可能对浏览器/GPU有特定要求）以及多视图功能。从沙发上舒适地控制可能需要蓝牙鼠标/键盘或空中鼠标。手机可以通过适配器连接，但通常面临分辨率限制（例如，iPhone上的Netflix仅支持1080p），并且与某些服务的屏幕镜像存在不一致性。

至关重要的是，任何旨在播放4K或HDR内容的设置，都必须确保显示器和连接设备都符合HDCP 2.2标准。

---

## 3. OpenAI 悄然采用技能，现已登陆 ChatGPT 和 Codex CLI

**原文标题**: OpenAI are quietly adopting skills, now available in ChatGPT and Codex CLI

**原文链接**: [https://simonwillison.net/2025/Dec/12/openai-skills/](https://simonwillison.net/2025/Dec/12/openai-skills/)

2025年12月12日，这篇文章宣布OpenAI正在悄然将“技能（skills）”集成到ChatGPT的Code Interpreter和Codex CLI工具中，此举模仿了Anthropic早期的实现方式。技能的实现方式很简单：一个包含Markdown文件和可选资源的文件夹，旨在让能够进行文件系统导航的LLM轻松采用。

在ChatGPT中，技能位于一个新的`/home/oai/skills`文件夹中，支持电子表格、DOCX和PDF文件。对于文档和PDF文件，OpenAI的方法是将页面转换为PNG图片，然后使用具备视觉能力的GPT模型进行处理，以保留布局和图形细节。一个例子展示了GPT-5.2精心创建了一个PDF摘要，包括对字体兼容性的自我修正。

另外，OpenAI的开源Codex CLI最近增加了对技能的实验性支持。`~/.codex/skills`中的任何文件夹都可以作为一项技能，通过`--enable skills`选项激活。作者成功地使用Codex CLI生成了一个Datasette插件，展示了其实际应用。

作者强调，OpenAI的迅速采纳验证了他此前对技能是一项非常重要的发展的评估，并呼吁对其进行正式的文档编写，最好由Agentic AI Foundation来完成。

---

## 4. macOS 26.2 支持基于雷雳RDMA的快速AI集群

**原文标题**: macOS 26.2 enables fast AI clusters with RDMA over Thunderbolt

**原文链接**: [https://developer.apple.com/documentation/macos-release-notes/macos-26_2-release-notes#RDMA-over-Thunderbolt](https://developer.apple.com/documentation/macos-release-notes/macos-26_2-release-notes#RDMA-over-Thunderbolt)

所提供的内容不包含题为“macOS 26.2 通过雷电上的RDMA实现快速AI集群”的文章。相反，它显示一条消息，指出该页面需要JavaScript且无法查看。

因此，无法总结该预期文章的主要观点和关键信息。该标题表明，文章将详细介绍macOS 26.2（可能代号为“Tahoe”）如何通过在雷电技术上实现远程直接内存访问（RDMA）来促进高速AI集群，这将显著增强AI工作负载的数据传输和处理能力。然而，支持这一点的实际内容却无法获取。

---

## 5. 诺基亚 N900 起死回生

**原文标题**: Nokia N900 Necromancy

**原文链接**: [https://yaky.dev/2025-12-11-nokia-n900-necromancy/](https://yaky.dev/2025-12-11-nokia-n900-necromancy/)

该项目详细介绍了朋友的诺基亚N900“起死回生”的过程，该手机电池已失效，无法启动。作者摒弃了不可靠的替代电池，最初使用超级电容器和电阻器制作了一个原型“假电池”，成功启动了该设备。

后来，这项设计演变为一个定制的3D打印外壳，可容纳十个小型超级电容器（总计0.5F），并能适配电池仓。在测试过程中，电源波动损坏了内部操作系统，这促使作者改为从SD卡启动。

试图通过N900原装micro-USB端口统一供电却适得其反，造成了严重后果。该端口本身已知的脆弱性，再加上意外损坏，导致主板上一个关键的+5V焊盘被毁坏，使得原装USB端口彻底失效。

作者并未气馁，进行了“彻底的改造”。一个小型USB-C端口经过物理改造以适应N900的机身。由于空间限制，仅连接了5V和地线，将充电电流限制在0.5A，仅支持基本的USB-A转USB-C线缆充电。随后设计了一个新的3D打印“电池”，用于容纳一个大电容器、一个二极管以及从报废原装电池中取出的控制模块，通过新的USB-C端口供电。

这种定制的解决方案成功地“复活”了N900，使其能够从SD卡启动，并以网络收音机设备的身份找到了新的用途。

---

## 6. 谷歌取消收录了熊博客，我不知道为什么。

**原文标题**: Google de-indexed Bear Blog and I don't know why

**原文链接**: [https://journal.james-zhan.com/google-de-indexed-my-entire-bear-blog-and-i-dont-know-why/](https://journal.james-zhan.com/google-de-indexed-my-entire-bear-blog-and-i-dont-know-why/)

詹姆斯·詹在blog.james-zhan.com上的Bear Blog，尽管最初成功收录，但由于未知原因，其在Google上被完全取消索引。问题始于10月14日，当时詹不小心为RSS订阅源URL启动了Google Search Console (GSC) 验证。截至10月20日，他除一篇博文外，所有文章都已被取消索引，显示状态为“已抓取 - 当前未编入索引”，最后一篇文章也在11月3日被取消索引。

詹进行了大量的故障排除工作。他通过在另一个子域名 (www.james-zhan.com) 上成功索引另一个Bear Blog，排除了域名问题。内容质量或数量也被排除，因为其他极简主义的Bear博客收录正常。同样，URL结构也不是原因，这已通过使用相同默认设置的其他Bear博客证实。Bear Blog的创始人Herman也确认博客或其CSS代码没有阻止索引的技术问题。关键是，该博客仍被DuckDuckGo、Bing和Brave等其他搜索引擎正常索引，这表明网站本身没有内在的技术缺陷。

詹无法解决这个神秘的取消索引问题，于是将他的博客迁移到一个新的子域名journal.james-zhan.com（当前网站），将域名转发转移到Porkbun，并设置了重定向。对于新博客，他决定不再手动向GSC提交站点地图，希望其能自然索引。詹现在寻求公众的帮助，以了解最初取消索引的原因。

---

## 7. Epic在iOS支付案胜诉后，庆祝“苹果税”的终结。

**原文标题**: Epic celebrates "the end of the Apple Tax" after court win in iOS payments case

**原文链接**: [https://arstechnica.com/tech-policy/2025/12/epic-celebrates-the-end-of-the-apple-tax-after-appeals-court-win-in-ios-payments-case/](https://arstechnica.com/tech-policy/2025/12/epic-celebrates-the-end-of-the-apple-tax-after-appeals-court-win-in-ios-payments-case/)

The Ninth Circuit Court of Appeals has largely upheld a lower court's ruling finding Apple in "willful violation" of a 2021 injunction concerning iOS App Store payments. Epic Games CEO Tim Sweeney hailed the decision as "the end of the Apple Tax" in the USA, anticipating "untaxed competition" on iOS payments worldwide.

The appeals court affirmed that Apple's initial 27 percent fee for external payment options was "prohibitive" and its restrictions on external links were "overly broad." It also agreed that Apple acted in "bad faith" by resisting compliance. However, the appellate court did modify the lower court's blanket ban on fees, suggesting Apple *can* charge a "reasonable fee" based on its "actual costs to ensure user security and privacy." Sweeney believes these should be minimal, covering only app review costs.

Sweeney expects "rapid adoption" of outside payment processors, including Epic Web Shops, predicting web payments will be the norm by next year. He also highlighted a widespread "fear of retaliation" among developers, where Apple allegedly uses "soft power"—like delaying app reviews or burying products—against those using alternative payment methods. Sweeney called this "totally illegal" and urged regulators to address this pervasive fear, stating, "everybody’s afraid of Apple." Apple has not yet commented.

---

## 8. UK House of Lords attempting to ban use of VPNs by anyone under 16

**原文标题**: UK House of Lords attempting to ban use of VPNs by anyone under 16

**原文链接**: [https://alecmuffett.com/article/134925](https://alecmuffett.com/article/134925)

生成摘要时出错

---

## 9. Rats Play DOOM

**原文标题**: Rats Play DOOM

**原文链接**: [https://ratsplaydoom.com/](https://ratsplaydoom.com/)

生成摘要时出错

---

## 10. SQLite JSON at full index speed using generated columns

**原文标题**: SQLite JSON at full index speed using generated columns

**原文链接**: [https://www.dbpro.app/blog/sqlite-json-virtual-columns-indexing](https://www.dbpro.app/blog/sqlite-json-virtual-columns-indexing)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 2 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 3 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 4 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 5 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 6 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 7 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 8 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 9 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 10 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 11 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 12 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 13 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 14 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 15 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 16 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 17 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 18 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 19 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 20 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 21 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 22 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 23 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 24 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 25 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 26 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 27 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 28 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 29 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 30 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 31 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 32 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 33 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 34 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 35 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 36 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 37 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
| 38 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
