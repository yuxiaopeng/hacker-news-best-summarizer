# Hacker News 热门文章摘要 (2026-01-06)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 难以合理化太浩湖的标志

**原文标题**: It's hard to justify Tahoe icons

**原文链接**: [https://tonsky.me/blog/tahoe-icons/](https://tonsky.me/blog/tahoe-icons/)

文章《塔霍图标难以自圆其说》批判了苹果公司假想的macOS Tahoe操作系统，该系统为每个菜单项引入了图标，作者认为这些图标“令人不快、分散注意力、难以辨认、杂乱、拥挤、混乱、令人沮丧”。作者认为这种做法违反了基本可用性原则，并经常引用苹果1992年的《人机界面指南》(HIG)，该指南由于人类认知功能不变而至今仍具指导意义。

主要批评包括：
1.  **缺乏区分度：** 如果每个项目都有图标，就没有什么能脱颖而出，这使得快速找到特定命令变得更加困难，这与稀疏使用独特（可能带颜色）的图标形成对比。
2.  **不一致性：** 对于“新建”、“打开”、“保存”、“剪切”和“删除”等常见基础操作的图标，在不同的苹果应用程序之间，甚至在同一应用程序的菜单和工具栏之间都存在巨大差异。
3.  **图标重复使用：** 相同的图标经常被用于完全不同的操作，导致用户产生严重困惑。
4.  **过度细微与细节化：** 图标依赖于微小、难以察觉的差异（例如，箭头细微的角度或描边宽度）来传达不同的含义。它们还非常小（在高DPI屏幕上为24x24像素，实际比历史图标更小）且过于详细，使得它们难以辨认。
5.  **技术缺陷：** 苹果使用矢量字体导致图标模糊，且未进行像素对齐。
6.  **令人困惑的隐喻：** 许多图标使用了拙劣、荒谬或主动误导的隐喻（例如，“全选”，“选中”代表“取消选中”）。其他图标则忽视既定惯例，或将文本 *用作* 图标，模糊了图形与文字的界限。
7.  **破坏扫视：** 图标不一致的存在和对齐方式，破坏了用户通过阅读首字母快速扫视菜单的能力。

作者总结道，为 *每个* 菜单项添加图标是一项不可能完成且自找麻烦的任务，因为根本没有足够清晰的隐喻，而且这个前提本身就是有缺陷的，因为当所有事物都被强调时，就没有什么被强调了。

---

## 2. 围马

**原文标题**: enclose.horse

**原文链接**: [https://enclose.horse/](https://enclose.horse/)

这篇文章名为“enclose.horse”，描述了一种以“围栏”（enclosure）概念为核心的个人计算理念——即创建一个自给自足、隔离且高度受控的计算环境。作者主张将一台单一、便携的笔记本电脑作为主要计算设备，并摒弃使用云服务、个人服务器，甚至除了必要的互联网连接之外的本地网络访问。

这一理念的核心原则包括：
*   **隔离性：** 笔记本电脑被视为一个独立系统，不与家庭网络、服务器或云存储交互。数据只保存在设备上。
*   **便携性：** 所选笔记本电脑是一个功能强大、自给自足的单元，可以轻松携带并在任何地方使用，不依赖外部设备。
*   **设备内自托管：** 用户不依赖外部服务，而是在*笔记本电脑本身*上“自托管”所有相关内容。这包括数据、配置和应用程序。
*   **无云，无服务器：** 明确拒绝云存储、同步服务和家用服务器，以保持完全控制并减少攻击面。
*   **不可变基础设施：** 该系统旨在建立一个弹性设置，其中核心配置是稳定的，并且所有更改都是有意的且受控的。备份至关重要，并且最好是外部备份。
*   **专注于本地控制：** 目标是最大限度地个人控制数据和计算体验，最大限度地减少对第三方的依赖。

作者提出这种方法是为了降低复杂性、增强隐私性，并提供数字安全感和所有权，从而创建一个完全属于自己的“数字之马”。

---

## 3. 委内瑞拉停电期间发生了BGP异常

**原文标题**: There were BGP anomalies during the Venezuela blackout

**原文链接**: [https://loworbitsecurity.com/radar/radar16/](https://loworbitsecurity.com/radar/radar16/)

2026年1月2日委内瑞拉停电期间，观察到显著的BGP（边界网关协议）异常，这与地缘政治紧张局势以及涉及美国太空司令部（SPACECOM）和美国网络司令部（CYBERCOM）的军事行动同时发生。

作者作为一名攻击性安全从业者，对委内瑞拉国有电信公司CANTV（AS8048）进行了调查。Cloudflare Radar数据显示，CANTV出现了异常的BGP路由泄漏，有八个IP前缀通过CANTV路由，其自治系统（AS）路径中包含Sparkle（一家以不实施RPKI过滤等BGP安全功能而闻名的意大利传输提供商）和GlobeNet（一家哥伦比亚运营商）。这对CANTV来说是一种非典型的路由情况。

使用`bgpdump`对公共BGP数据集进行分析，识别出受影响的特定前缀（例如，200.74.226.0/24到200.74.238.0/23），这些前缀属于加拉加斯的Dayco电信公司。对这些范围进行反向DNS查询发现，它们包含了银行、互联网服务提供商和电子邮件服务器等关键基础设施。

值得注意的是，这些泄漏路由的AS路径显示CANTV的AS号（8048）重复出现了十次。尽管BGP偏爱较短的路径，但这种“AS路径前置（prepending）”会使路由的吸引力降低，引发了对其意图的质疑。

这些BGP异常于1月2日世界协调时15:40被检测到，发生在1月3日加拉加斯报告的爆炸和美国军队调动之前。作者认为，即使是几个小时的互联网流量重路由，也能为政府实体提供大量情报收集的便利。这种无法解释的BGP活动的时机和性质强烈表明存在蓄意的“伎俩”。

---

## 4. 2025年数据库：年度回顾

**原文标题**: Databases in 2025: A Year in Review

**原文链接**: [https://www.cs.cmu.edu/~pavlo/blog/2026/01/2025-databases-retrospective.html](https://www.cs.cmu.edu/~pavlo/blog/2026/01/2025-databases-retrospective.html)

2025年，尽管作者个人面临挑战，数据库领域仍出现了显著趋势。

PostgreSQL继续保持其主导地位，第18版引入了异步I/O和跳过扫描（skip scans），突破了操作系统页面缓存的限制。其重要性通过几项重大收购得以凸显：Databricks以10亿美元收购了Neon，Snowflake以2.5亿美元收购了CrunchyData，两者都是PostgreSQL DBaaS公司。微软也推出了HorizonDB。这一年也出现了推动分布式PostgreSQL的浪潮，Supabase宣布推出Multigres（由Vitess联合创始人Sugu领导），PlanetScale推出了Neki，两者都旨在开发类似于Vitess针对MySQL的分片中间件。PgDog也作为该领域的竞争者出现。尽管许多云供应商已经提供PostgreSQL，但Hydra和PostgresML等小型独立软件开发商（ISV）破产，而Xata则调整了其基础设施。

另一项重大进展是，在OpenAI支持后，Anthropic的模型上下文协议（Model Context Protocol, MCP）得到了广泛采用。这个标准化的JSON-RPC接口允许大型语言模型（LLM）与数据库进行交互，促使每个数据库管理系统（DBMS）供应商和云服务提供商发布自己的MCP服务器。数据库分支（database branching）——允许代理安全测试更改的功能——也受到了关注，Neon报告称80%的新数据库是由代理创建的。然而，作者警告不要授予LLM无限制的访问权限，强调需要最小权限和自动化防护措施，而这通常是企业系统所具备的。

最后，一起值得关注的法律事件是MongoDB公司与FerretDB公司之间的诉讼，后者是一个将MongoDB查询转换为PostgreSQL后端查询的中间件代理。

---

## 5. 安娜档案突遭暂停，失去.org域名

**原文标题**: Anna's Archive loses .org domain after surprise suspension

**原文链接**: [https://torrentfreak.com/annas-archive-loses-org-domain-after-surprise-suspension/](https://torrentfreak.com/annas-archive-loses-org-domain-after-surprise-suspension/)

Anna档案，一个在Z-Library被查封后上线的盗版书籍和文章元搜索引擎，因意外暂停服务而失去了其主要的`annas-archive.org`域名。该网站也协助AI研究人员，并最近宣布了一个300TB的Spotify大规模备份，其域名状态已变为"serverHold"，这表明它已被负责管理.org域名的公共利益注册局（PIR）暂停服务。

PIR采取此类行动实属罕见，这表明它很可能是由法院命令强制执行的，尽管PIR拒绝置评。尽管最近的“规避DRM”Spotify备份可能是导火索，但尚无确凿证据，并且来自正在进行的WorldCat诉讼（Anna档案被起诉）的禁令也尚未得到证实。

Anna档案将此视为一次“小插曲”，否认与Spotify备份有关，并引导用户访问其他目前可用的域名，例如`.li`、`.se`、`.in`和`.pm`。这不是他们第一次面临域名挑战；此前迁移到`.gs`域名也导致了迅速的暂停服务。尽管他们表现出韧性并继续在新域名上运营，但日益增长的法律压力给他们的长期稳定性蒙上了一层阴影。

---

## 6. 维纳姆屏蔽强制广告

**原文标题**: Vienam bans unskippable ads

**原文链接**: [https://saigoneer.com/vietnam-news/28652-vienam-bans-unskippable-ads,-requires-skip-button-to-appear-after-5-seconds](https://saigoneer.com/vietnam-news/28652-vienam-bans-unskippable-ads,-requires-skip-button-to-appear-after-5-seconds)

越南将实施第342号法令，该法令是对其国家广告法的修订，并将于2026年2月15日生效。此法令旨在更严格地控制线上广告活动，保护消费者，并遏制非法广告。

一项重大改变针对不可跳过的广告：视频和动画广告在用户能够跳过之前，最长不得超过五秒。静态广告必须能够立即关闭。此外，该法令强制要求平台提供清晰、只需一次交互即可关闭广告的方式，并明确禁止旨在混淆用户的误导性或模糊符号。

线上平台还必须设置可见的符号和指南，以帮助用户举报违法广告，并允许用户关闭或拒绝不当内容。除了用户体验之外，考虑到对人类健康和环境的直接影响，该法令还将严格规范11类特定商品和服务的广告，例如化妆品、食品饮料、药品和酒精饮料。

---

## 7. AWS周六将GPU价格上调15%，指望你没注意到。

**原文标题**: AWS raises GPU prices 15% on a Saturday, hopes you weren't paying attention

**原文链接**: [https://www.theregister.com/2026/01/05/aws_price_increase/](https://www.theregister.com/2026/01/05/aws_price_increase/)

AWS已悄然将其适用于机器学习 (ML) 的EC2容量块价格上调了约15%，特别是影响到p5e.48xlarge和p5en.48xlarge GPU实例。例如，在大多数区域，p5e.48xlarge的价格从每小时34.61美元跃升至39.80美元，部分区域涨幅更高。此次涨价于2026年1月的一个周六实施，在此之前七个月，AWS曾宣布针对其他GPU实例类型“最高达45%的降价”。

容量块对于需要预先支付费用、并在特定时间窗口内保证GPU容量的严谨机器学习操作至关重要。AWS将“供需模式”列为此次调整的原因。

作者Corey Quinn强调，这显著偏离了AWS典型的定价策略，后者通常是通过改变定价维度或仅因监管行动而实施涨价。此举为Azure和GCP等竞争对手提供了强有力的论据，并对拥有企业折扣计划的客户造成负面影响。

文章将此次涨价视为一个“风向标”，暗示这可能预示着其他资源受限服务（例如内存或Graviton实例）未来的价格上涨。至关重要的是，它打破了客户长达二十年认为AWS价格只会走低的期望。这开创了一个先例，使得后续其他服务的涨价变得更有可能。Quinn总结称，这很可能是云计算定价的“新常态”，而非异常。

---

## 8. Claude Code On-the-Go

**原文标题**: Claude Code On-the-Go

**原文链接**: [https://granda.org/en/2026/01/02/claude-code-on-the-go/](https://granda.org/en/2026/01/02/claude-code-on-the-go/)

生成摘要时出错

---

## 9. Google broke my heart

**原文标题**: Google broke my heart

**原文链接**: [https://perishablepress.com/google-broke-my-heart/](https://perishablepress.com/google-broke-my-heart/)

生成摘要时出错

---

## 10. The Post-American Internet

**原文标题**: The Post-American Internet

**原文链接**: [https://pluralistic.net/2026/01/01/39c3/](https://pluralistic.net/2026/01/01/39c3/)

生成摘要时出错

---

## 11. Murder-suicide case shows OpenAI selectively hides data after users die

**原文标题**: Murder-suicide case shows OpenAI selectively hides data after users die

**原文链接**: [https://arstechnica.com/tech-policy/2025/12/openai-refuses-to-say-where-chatgpt-logs-go-when-users-die/](https://arstechnica.com/tech-policy/2025/12/openai-refuses-to-say-where-chatgpt-logs-go-when-users-die/)

生成摘要时出错

---

## 12. Brave overhauled its Rust adblock engine with FlatBuffers, cutting memory 75%

**原文标题**: Brave overhauled its Rust adblock engine with FlatBuffers, cutting memory 75%

**原文链接**: [https://brave.com/privacy-updates/36-adblock-memory-reduction/](https://brave.com/privacy-updates/36-adblock-memory-reduction/)

生成摘要时出错

---

## 13. I switched from VSCode to Zed

**原文标题**: I switched from VSCode to Zed

**原文链接**: [https://tenthousandmeters.com/blog/i-switched-from-vscode-to-zed/](https://tenthousandmeters.com/blog/i-switched-from-vscode-to-zed/)

生成摘要时出错

---

## 14. 65% of Hacker News posts have negative sentiment, and they outperform

**原文标题**: 65% of Hacker News posts have negative sentiment, and they outperform

**原文链接**: [https://philippdubach.com/standalone/hn-sentiment/](https://philippdubach.com/standalone/hn-sentiment/)

生成摘要时出错

---

## 15. Show HN: Terminal UI for AWS

**原文标题**: Show HN: Terminal UI for AWS

**原文链接**: [https://github.com/huseyinbabal/taws](https://github.com/huseyinbabal/taws)

生成摘要时出错

---

## 16. During Helene, I just wanted a plain text website

**原文标题**: During Helene, I just wanted a plain text website

**原文链接**: [https://sparkbox.com/foundry/helene_and_mobile_web_performance](https://sparkbox.com/foundry/helene_and_mobile_web_performance)

生成摘要时出错

---

## 17. Microsoft Office renamed to “Microsoft 365 Copilot app”

**原文标题**: Microsoft Office renamed to “Microsoft 365 Copilot app”

**原文链接**: [https://www.office.com](https://www.office.com)

生成摘要时出错

---

## 18. C Is Best (2025)

**原文标题**: C Is Best (2025)

**原文链接**: [https://sqlite.org/whyc.html](https://sqlite.org/whyc.html)

生成摘要时出错

---

## 19. Show HN: DoNotNotify – Log and intelligently block notifications on Android

**原文标题**: Show HN: DoNotNotify – Log and intelligently block notifications on Android

**原文链接**: [https://donotnotify.com/](https://donotnotify.com/)

生成摘要时出错

---

## 20. X blames users for Grok-generated CSAM; no fixes announced

**原文标题**: X blames users for Grok-generated CSAM; no fixes announced

**原文链接**: [https://arstechnica.com/tech-policy/2026/01/x-blames-users-for-grok-generated-csam-no-fixes-announced/](https://arstechnica.com/tech-policy/2026/01/x-blames-users-for-grok-generated-csam-no-fixes-announced/)

生成摘要时出错

---

## 21. All AI Videos Are Harmful (2025)

**原文标题**: All AI Videos Are Harmful (2025)

**原文链接**: [https://idiallo.com/blog/all-ai-videos-are-harmful](https://idiallo.com/blog/all-ai-videos-are-harmful)

生成摘要时出错

---

## 22. Why does a least squares fit appear to have a bias when applied to simple data?

**原文标题**: Why does a least squares fit appear to have a bias when applied to simple data?

**原文链接**: [https://stats.stackexchange.com/questions/674129/why-does-a-linear-least-squares-fit-appear-to-have-a-bias-when-applied-to-simple](https://stats.stackexchange.com/questions/674129/why-does-a-linear-least-squares-fit-appear-to-have-a-bias-when-applied-to-simple)

生成摘要时出错

---

## 23. California residents can now request all data brokers delete personal info

**原文标题**: California residents can now request all data brokers delete personal info

**原文链接**: [https://consumer.drop.privacy.ca.gov/](https://consumer.drop.privacy.ca.gov/)

生成摘要时出错

---

## 24. A spider web unlike any seen before

**原文标题**: A spider web unlike any seen before

**原文链接**: [https://www.nytimes.com/2025/11/08/science/biggest-spiderweb-sulfur-cave.html](https://www.nytimes.com/2025/11/08/science/biggest-spiderweb-sulfur-cave.html)

生成摘要时出错

---

## 25. Jensen: 'We've done our country a great disservice' by offshoring

**原文标题**: Jensen: 'We've done our country a great disservice' by offshoring

**原文链接**: [https://www.barchart.com/story/news/36862423/weve-done-our-country-a-great-disservice-by-offshoring-nvidias-jensen-huang-says-we-have-to-create-prosperity-for-all-not-just-phds](https://www.barchart.com/story/news/36862423/weve-done-our-country-a-great-disservice-by-offshoring-nvidias-jensen-huang-says-we-have-to-create-prosperity-for-all-not-just-phds)

生成摘要时出错

---

## 26. Show HN: Tailsnitch – A security auditor for Tailscale

**原文标题**: Show HN: Tailsnitch – A security auditor for Tailscale

**原文链接**: [https://github.com/Adversis/tailsnitch](https://github.com/Adversis/tailsnitch)

生成摘要时出错

---

## 27. Show HN: Prism.Tools – Free and privacy-focused developer utilities

**原文标题**: Show HN: Prism.Tools – Free and privacy-focused developer utilities

**原文链接**: [https://blgardner.github.io/prism.tools/](https://blgardner.github.io/prism.tools/)

生成摘要时出错

---

## 28. Six-decade math puzzle solved by Korean mathematician

**原文标题**: Six-decade math puzzle solved by Korean mathematician

**原文链接**: [https://www.koreaherald.com/article/10648326](https://www.koreaherald.com/article/10648326)

生成摘要时出错

---

## 29. I/O is no longer the bottleneck? (2022)

**原文标题**: I/O is no longer the bottleneck? (2022)

**原文链接**: [https://stoppels.ch/2022/11/27/io-is-no-longer-the-bottleneck.html](https://stoppels.ch/2022/11/27/io-is-no-longer-the-bottleneck.html)

生成摘要时出错

---

## 30. Sega co-founder David Rosen has died

**原文标题**: Sega co-founder David Rosen has died

**原文链接**: [https://www.theguardian.com/games/2026/jan/05/sega-co-founder-david-rosen-dies](https://www.theguardian.com/games/2026/jan/05/sega-co-founder-david-rosen-dies)

生成摘要时出错

---

## 31. Donut Lab’s all-solid-state battery delivers 400 Wh/kg of energy density

**原文标题**: Donut Lab’s all-solid-state battery delivers 400 Wh/kg of energy density

**原文链接**: [https://www.donutlab.com/ces-battery-announcement/](https://www.donutlab.com/ces-battery-announcement/)

生成摘要时出错

---

## 32. ICE is using facial-recognition technology to quickly arrest people

**原文标题**: ICE is using facial-recognition technology to quickly arrest people

**原文链接**: [https://www.wsj.com/politics/policy/ice-facial-recognition-app-mobile-fortify-dfdd00bf](https://www.wsj.com/politics/policy/ice-facial-recognition-app-mobile-fortify-dfdd00bf)

生成摘要时出错

---

## 33. Why didn't AI “join the workforce” in 2025?

**原文标题**: Why didn't AI “join the workforce” in 2025?

**原文链接**: [https://calnewport.com/why-didnt-ai-join-the-workforce-in-2025/](https://calnewport.com/why-didnt-ai-join-the-workforce-in-2025/)

生成摘要时出错

---

## 34. Eurostar AI vulnerability: When a chatbot goes off the rails

**原文标题**: Eurostar AI vulnerability: When a chatbot goes off the rails

**原文链接**: [https://www.pentestpartners.com/security-blog/eurostar-ai-vulnerability-when-a-chatbot-goes-off-the-rails/](https://www.pentestpartners.com/security-blog/eurostar-ai-vulnerability-when-a-chatbot-goes-off-the-rails/)

生成摘要时出错

---

## 35. Why is the Gmail app 700 MB?

**原文标题**: Why is the Gmail app 700 MB?

**原文链接**: [https://akr.am/blog/posts/why-is-the-gmail-app-700-mb](https://akr.am/blog/posts/why-is-the-gmail-app-700-mb)

生成摘要时出错

---

## 36. Strange.website

**原文标题**: Strange.website

**原文链接**: [https://strange.website/](https://strange.website/)

生成摘要时出错

---

## 37. I changed my personality in six weeks

**原文标题**: I changed my personality in six weeks

**原文链接**: [https://www.bbc.com/future/article/20260102-how-i-changed-my-personality-in-six-weeks](https://www.bbc.com/future/article/20260102-how-i-changed-my-personality-in-six-weeks)

生成摘要时出错

---

## 38. GBC Boot Animation 88×31 Web Button

**原文标题**: GBC Boot Animation 88×31 Web Button

**原文链接**: [https://zakhary.dev/blog/gbc-web-button](https://zakhary.dev/blog/gbc-web-button)

生成摘要时出错

---

## 39. How Y Combinator made it smart to trust founders

**原文标题**: How Y Combinator made it smart to trust founders

**原文链接**: [https://elbowgreasegames.substack.com/p/when-good-actors-can-trust-each-other](https://elbowgreasegames.substack.com/p/when-good-actors-can-trust-each-other)

生成摘要时出错

---

## 40. Agentic Patterns

**原文标题**: Agentic Patterns

**原文链接**: [https://github.com/nibzard/awesome-agentic-patterns](https://github.com/nibzard/awesome-agentic-patterns)

生成摘要时出错

---

## 41. Decorative Cryptography

**原文标题**: Decorative Cryptography

**原文链接**: [https://www.dlp.rip/decorative-cryptography](https://www.dlp.rip/decorative-cryptography)

生成摘要时出错

---

## 42. State of the Fin 2026-01-06

**原文标题**: State of the Fin 2026-01-06

**原文链接**: [https://jellyfin.org/posts/state-of-the-fin-2026-01-06/](https://jellyfin.org/posts/state-of-the-fin-2026-01-06/)

生成摘要时出错

---

## 43. North Dakota law lists fake critical minerals based on coal lawyers' names

**原文标题**: North Dakota law lists fake critical minerals based on coal lawyers' names

**原文链接**: [https://bismarcktribune.com/news/local/government-politics/article_515812a0-d29a-4161-91f1-3e53003e2911.html](https://bismarcktribune.com/news/local/government-politics/article_515812a0-d29a-4161-91f1-3e53003e2911.html)

生成摘要时出错

---

## 44. Volkswagen Brings Back Physical Buttons

**原文标题**: Volkswagen Brings Back Physical Buttons

**原文链接**: [https://www.caranddriver.com/news/a69916699/volkswagen-interior-physical-buttons-return/](https://www.caranddriver.com/news/a69916699/volkswagen-interior-physical-buttons-return/)

生成摘要时出错

---

## 45. CSS sucks because we don't bother learning it (2022)

**原文标题**: CSS sucks because we don't bother learning it (2022)

**原文链接**: [https://idiallo.com/blog/learn-css](https://idiallo.com/blog/learn-css)

生成摘要时出错

---

## 46. Gatekeepers of Law: Inside the Westlaw and LexisNexis Duopoly

**原文标题**: Gatekeepers of Law: Inside the Westlaw and LexisNexis Duopoly

**原文链接**: [https://www.thebignewsletter.com/p/gatekeepers-of-law-inside-the-westlaw](https://www.thebignewsletter.com/p/gatekeepers-of-law-inside-the-westlaw)

生成摘要时出错

---

## 47. So, you want to chunk really fast?

**原文标题**: So, you want to chunk really fast?

**原文链接**: [https://minha.sh/posts/so,-you-want-to-chunk-really-fast](https://minha.sh/posts/so,-you-want-to-chunk-really-fast)

生成摘要时出错

---

## 48. Cigarette smoke effect using shaders

**原文标题**: Cigarette smoke effect using shaders

**原文链接**: [https://garden.bradwoods.io/notes/javascript/three-js/shaders/shaders-103-smoke](https://garden.bradwoods.io/notes/javascript/three-js/shaders/shaders-103-smoke)

生成摘要时出错

---

## 49. Pentagon moves to punish Democratic senator over 'seditious video'

**原文标题**: Pentagon moves to punish Democratic senator over 'seditious video'

**原文链接**: [https://www.bbc.com/news/articles/cp8039wg1rdo](https://www.bbc.com/news/articles/cp8039wg1rdo)

生成摘要时出错

---

## 50. GOG Patrons- Join gamers keeping classics alive

**原文标题**: GOG Patrons- Join gamers keeping classics alive

**原文链接**: [https://www.gog.com/en/patrons](https://www.gog.com/en/patrons)

生成摘要时出错

---

## 51. Pipe Dreams – The life and times of Yahoo Pipes (2023)

**原文标题**: Pipe Dreams – The life and times of Yahoo Pipes (2023)

**原文链接**: [https://retool.com/pipes](https://retool.com/pipes)

生成摘要时出错

---

## 52. Novo Nordisk launches Wegovy weight-loss pill in US, triggering price war

**原文标题**: Novo Nordisk launches Wegovy weight-loss pill in US, triggering price war

**原文链接**: [https://www.theguardian.com/business/2026/jan/05/novo-nordisk-launches-wegovy-weight-loss-pill-us-price-war](https://www.theguardian.com/business/2026/jan/05/novo-nordisk-launches-wegovy-weight-loss-pill-us-price-war)

生成摘要时出错

---

## 53. Dealing with abandonware (2024)

**原文标题**: Dealing with abandonware (2024)

**原文链接**: [https://blog.hris.to/./dealing-with-abandonware.html](https://blog.hris.to/./dealing-with-abandonware.html)

生成摘要时出错

---

## 54. OneDrive just deleted all of my files

**原文标题**: OneDrive just deleted all of my files

**原文链接**: [https://twitter.com/jasonkpargin/status/2007659047663874120](https://twitter.com/jasonkpargin/status/2007659047663874120)

生成摘要时出错

---

## 55. A prediction market user made $436k betting on Maduro's downfall

**原文标题**: A prediction market user made $436k betting on Maduro's downfall

**原文链接**: [https://www.bbc.com/news/articles/cx2gn93292do](https://www.bbc.com/news/articles/cx2gn93292do)

生成摘要时出错

---

## 56. SCiZE's Classic Warez Collection

**原文标题**: SCiZE's Classic Warez Collection

**原文链接**: [https://scenelist.org/](https://scenelist.org/)

生成摘要时出错

---

## 57. Singularity Rootkit: SELinux bypass and netlink filter (ss/conntrack hidden)

**原文标题**: Singularity Rootkit: SELinux bypass and netlink filter (ss/conntrack hidden)

**原文链接**: [https://github.com/MatheuZSecurity/Singularity](https://github.com/MatheuZSecurity/Singularity)

生成摘要时出错

---

## 58. Stop Forwarding Errors, Start Designing Them

**原文标题**: Stop Forwarding Errors, Start Designing Them

**原文链接**: [https://fast.github.io/blog/stop-forwarding-errors-start-designing-them/](https://fast.github.io/blog/stop-forwarding-errors-start-designing-them/)

生成摘要时出错

---

## 59. Intel Core Ultra Series 3 Debut as First Built on Intel 18A

**原文标题**: Intel Core Ultra Series 3 Debut as First Built on Intel 18A

**原文链接**: [https://newsroom.intel.com/client-computing/ces-2026-intel-core-ultra-series-3-debut-first-built-on-intel-18a](https://newsroom.intel.com/client-computing/ces-2026-intel-core-ultra-series-3-debut-first-built-on-intel-18a)

生成摘要时出错

---

## 60. Boston Dynamics and DeepMind form new AI partnership

**原文标题**: Boston Dynamics and DeepMind form new AI partnership

**原文链接**: [https://bostondynamics.com/blog/boston-dynamics-google-deepmind-form-new-ai-partnership/](https://bostondynamics.com/blog/boston-dynamics-google-deepmind-form-new-ai-partnership/)

生成摘要时出错

---

## 61. Building a Rust-style static analyzer for C++ with AI

**原文标题**: Building a Rust-style static analyzer for C++ with AI

**原文链接**: [http://mpaxos.com/blog/rusty-cpp.html](http://mpaxos.com/blog/rusty-cpp.html)

生成摘要时出错

---

## 62. Mamdani Targets Junk Fees and Hidden Charges in Two Executive Orders

**原文标题**: Mamdani Targets Junk Fees and Hidden Charges in Two Executive Orders

**原文链接**: [https://www.nytimes.com/2026/01/05/nyregion/mamdani-affordability-consumer-protections.html](https://www.nytimes.com/2026/01/05/nyregion/mamdani-affordability-consumer-protections.html)

生成摘要时出错

---

## 63. "Microslop" trends on social media

**原文标题**: "Microslop" trends on social media

**原文链接**: [https://www.windowscentral.com/artificial-intelligence/microslop-trends-on-social-media-backlash-to-microsofts-on-going-ai-obsession-continues](https://www.windowscentral.com/artificial-intelligence/microslop-trends-on-social-media-backlash-to-microsofts-on-going-ai-obsession-continues)

生成摘要时出错

---

## 64. Opus 4.5 is not the normal AI agent experience that I have had thus far

**原文标题**: Opus 4.5 is not the normal AI agent experience that I have had thus far

**原文链接**: [https://burkeholland.github.io/posts/opus-4-5-change-everything/](https://burkeholland.github.io/posts/opus-4-5-change-everything/)

生成摘要时出错

---

## 65. Show HN: Server-rendered multiplayer games with Lua (no client code)

**原文标题**: Show HN: Server-rendered multiplayer games with Lua (no client code)

**原文链接**: [https://cleoselene.com/](https://cleoselene.com/)

生成摘要时出错

---

## 66. Imagine 130M Washing Machines

**原文标题**: Imagine 130M Washing Machines

**原文链接**: [https://scottsumner.substack.com/p/imagine-130000000-washing-machines](https://scottsumner.substack.com/p/imagine-130000000-washing-machines)

生成摘要时出错

---

## 67. A web developer posted a payment shaming message on their client's site

**原文标题**: A web developer posted a payment shaming message on their client's site

**原文链接**: [https://joseph-smith.co.uk/](https://joseph-smith.co.uk/)

生成摘要时出错

---

## 68. Show HN: A simulator for engineers transitioning from IC to management

**原文标题**: Show HN: A simulator for engineers transitioning from IC to management

**原文链接**: [https://apmcommunication.com/scenario/backchannel-vp](https://apmcommunication.com/scenario/backchannel-vp)

生成摘要时出错

---

## 69. Venezuela's interim government says it is united behind Maduro

**原文标题**: Venezuela's interim government says it is united behind Maduro

**原文链接**: [https://www.reuters.com/world/us/venezuelas-maduro-custody-trump-says-us-will-run-country-2026-01-04/](https://www.reuters.com/world/us/venezuelas-maduro-custody-trump-says-us-will-run-country-2026-01-04/)

生成摘要时出错

---

## 70. Observability's past, present, and future

**原文标题**: Observability's past, present, and future

**原文链接**: [https://blog.sherwoodcallaway.com/observability-s-past-present-and-future/](https://blog.sherwoodcallaway.com/observability-s-past-present-and-future/)

生成摘要时出错

---

## 71. Utopian Scholastic

**原文标题**: Utopian Scholastic

**原文链接**: [https://wol.fm/blog/utopian-scholastic.html](https://wol.fm/blog/utopian-scholastic.html)

生成摘要时出错

---

## 72. Raspberry Pi and mini PC home lab prices hit parity as DRAM costs skyrocket

**原文标题**: Raspberry Pi and mini PC home lab prices hit parity as DRAM costs skyrocket

**原文链接**: [https://www.tomshardware.com/raspberry-pi/raspberry-pi-and-mini-pc-home-lab-prices-hit-parity-as-dram-costs-skyrocket-price-hikes-force-hobbyists-to-weigh-up-performance-versus-power-consumption](https://www.tomshardware.com/raspberry-pi/raspberry-pi-and-mini-pc-home-lab-prices-hit-parity-as-dram-costs-skyrocket-price-hikes-force-hobbyists-to-weigh-up-performance-versus-power-consumption)

生成摘要时出错

---

## 73. Hacktivist deletes white supremacist websites live onstage during conference

**原文标题**: Hacktivist deletes white supremacist websites live onstage during conference

**原文链接**: [https://techcrunch.com/2026/01/05/hacktivist-deletes-white-supremacist-websites-live-on-stage-during-hacker-conference/](https://techcrunch.com/2026/01/05/hacktivist-deletes-white-supremacist-websites-live-on-stage-during-hacker-conference/)

生成摘要时出错

---

## 74. Keeping Syria connected during war: Surviving ISIS and Intelligence

**原文标题**: Keeping Syria connected during war: Surviving ISIS and Intelligence

**原文链接**: [https://syriauntold.com/2025/12/27/keeping-syria-connected-during-war/](https://syriauntold.com/2025/12/27/keeping-syria-connected-during-war/)

生成摘要时出错

---

## 75. How GitHub monopoly is destroying the open source ecosystem

**原文标题**: How GitHub monopoly is destroying the open source ecosystem

**原文链接**: [https://ploum.net/2026-01-05-unteaching_github.html](https://ploum.net/2026-01-05-unteaching_github.html)

生成摘要时出错

---

## 76. Sandboxing Untrusted Python

**原文标题**: Sandboxing Untrusted Python

**原文链接**: [https://gist.github.com/mavdol/2c68acb408686f1e038bf89e5705b28c](https://gist.github.com/mavdol/2c68acb408686f1e038bf89e5705b28c)

生成摘要时出错

---

## 77. Why German Strings Are Everywhere?

**原文标题**: Why German Strings Are Everywhere?

**原文链接**: [https://cedardb.com/blog/german_strings/](https://cedardb.com/blog/german_strings/)

生成摘要时出错

---

## 78. Portland's gas-powered leaf blower ban goes into effect

**原文标题**: Portland's gas-powered leaf blower ban goes into effect

**原文链接**: [https://www.oregonlive.com/environment/2026/01/portlands-gas-powered-leaf-blower-ban-goes-into-effect.html](https://www.oregonlive.com/environment/2026/01/portlands-gas-powered-leaf-blower-ban-goes-into-effect.html)

生成摘要时出错

---

## 79. New Lego smart-play system

**原文标题**: New Lego smart-play system

**原文链接**: [https://www.lego.com/en-us/smart-play](https://www.lego.com/en-us/smart-play)

生成摘要时出错

---

## 80. NeXTSTEP on Pa-RISC

**原文标题**: NeXTSTEP on Pa-RISC

**原文链接**: [https://www.openpa.net/nextstep_pa-risc.html](https://www.openpa.net/nextstep_pa-risc.html)

生成摘要时出错

---

## 81. Co-founder Joe Lonsdale: Palantir was founded to kill communists

**原文标题**: Co-founder Joe Lonsdale: Palantir was founded to kill communists

**原文链接**: [https://twitter.com/JTLonsdale/status/2007849014407086427](https://twitter.com/JTLonsdale/status/2007849014407086427)

生成摘要时出错

---

## 82. Scientific production in the era of large language models [pdf]

**原文标题**: Scientific production in the era of large language models [pdf]

**原文链接**: [https://gwern.net/doc/science/2025-kusumegi.pdf](https://gwern.net/doc/science/2025-kusumegi.pdf)

生成摘要时出错

---

## 83. NSFW Acronyms for Programmers (Free eBook)

**原文标题**: NSFW Acronyms for Programmers (Free eBook)

**原文链接**: [https://github.com/fristovic/naughty-words-every-programmer-should-know](https://github.com/fristovic/naughty-words-every-programmer-should-know)

生成摘要时出错

---

## 84. Gemini Protocol Deployment Statistics

**原文标题**: Gemini Protocol Deployment Statistics

**原文链接**: [https://www.obsessivefacts.com/gemini-proxy?uri=gemini%3A%2F%2Fgemini.bortzmeyer.org%2Fsoftware%2Flupa%2Fstats.gmi](https://www.obsessivefacts.com/gemini-proxy?uri=gemini%3A%2F%2Fgemini.bortzmeyer.org%2Fsoftware%2Flupa%2Fstats.gmi)

生成摘要时出错

---

## 85. Mapping Protests in Iran

**原文标题**: Mapping Protests in Iran

**原文链接**: [https://www.fdd.org/analysis/2025/06/25/mapping-the-protests-in-iran-2/](https://www.fdd.org/analysis/2025/06/25/mapping-the-protests-in-iran-2/)

生成摘要时出错

---

## 86. Show HN: Hover – IDE style hover documentation on any webpage

**原文标题**: Show HN: Hover – IDE style hover documentation on any webpage

**原文链接**: [https://github.com/Sampsoon/hover](https://github.com/Sampsoon/hover)

生成摘要时出错

---

## 87. The skill of the future is not 'AI', but 'Focus' (2025)

**原文标题**: The skill of the future is not 'AI', but 'Focus' (2025)

**原文链接**: [https://carette.xyz/posts/focus_will_be_the_skill_of_the_future/](https://carette.xyz/posts/focus_will_be_the_skill_of_the_future/)

生成摘要时出错

---

## 88. Show HN: An LLM-Powered PCB Schematic Checker (Major Update)

**原文标题**: Show HN: An LLM-Powered PCB Schematic Checker (Major Update)

**原文链接**: [https://traceformer.io/](https://traceformer.io/)

生成摘要时出错

---

## 89. Show HN: Open-Source 8-Ch BCI Board (ESP32 and ADS1299 and OpenBCI GUI)

**原文标题**: Show HN: Open-Source 8-Ch BCI Board (ESP32 and ADS1299 and OpenBCI GUI)

**原文链接**: [https://github.com/Cerelog-ESP-EEG/ESP-EEG](https://github.com/Cerelog-ESP-EEG/ESP-EEG)

生成摘要时出错

---

## 90. High-performance header-only container library for C++23 on x86-64

**原文标题**: High-performance header-only container library for C++23 on x86-64

**原文链接**: [https://github.com/kressler/fast-containers](https://github.com/kressler/fast-containers)

生成摘要时出错

---

## 91. A year of clean energy milestones

**原文标题**: A year of clean energy milestones

**原文链接**: [https://e360.yale.edu/digest/2025-energy-review](https://e360.yale.edu/digest/2025-energy-review)

生成摘要时出错

---

## 92. OpenGitOps

**原文标题**: OpenGitOps

**原文链接**: [https://opengitops.dev/](https://opengitops.dev/)

生成摘要时出错

---

## 93. LocalFirst: You Keep Using That Word

**原文标题**: LocalFirst: You Keep Using That Word

**原文链接**: [https://www.deobald.ca/essays/2026-01-01-localfirst-you-keep-using-that-word/](https://www.deobald.ca/essays/2026-01-01-localfirst-you-keep-using-that-word/)

生成摘要时出错

---

## 94. Millennium Challenge: A corrupted military exercise and its legacy (2015)

**原文标题**: Millennium Challenge: A corrupted military exercise and its legacy (2015)

**原文链接**: [https://warontherocks.com/2015/11/millennium-challenge-the-real-story-of-a-corrupted-military-exercise-and-its-legacy/](https://warontherocks.com/2015/11/millennium-challenge-the-real-story-of-a-corrupted-military-exercise-and-its-legacy/)

生成摘要时出错

---

## 95. Serious = Suspicious, Shooting with Phone vs. Shooting with Camera

**原文标题**: Serious = Suspicious, Shooting with Phone vs. Shooting with Camera

**原文链接**: [https://photoni.st/index.php/2026/01/02/serious-suspicious/](https://photoni.st/index.php/2026/01/02/serious-suspicious/)

生成摘要时出错

---

## 96. Gnome and Mozilla Discuss Proposal to Disable Middle Mouse Paste on Linux

**原文标题**: Gnome and Mozilla Discuss Proposal to Disable Middle Mouse Paste on Linux

**原文链接**: [https://linuxiac.com/gnome-and-mozilla-discuss-proposal-to-disable-middle-mouse-paste-on-linux/](https://linuxiac.com/gnome-and-mozilla-discuss-proposal-to-disable-middle-mouse-paste-on-linux/)

生成摘要时出错

---

## 97. Pink Power Ranger takes down white supremacist dating sites

**原文标题**: Pink Power Ranger takes down white supremacist dating sites

**原文链接**: [https://www.thecanary.co/skwawkbox/2026/01/04/power-ranger-deletes-dating-site/](https://www.thecanary.co/skwawkbox/2026/01/04/power-ranger-deletes-dating-site/)

生成摘要时出错

---

## 98. A ssh server that knows who you are. $ ssh whoami.filippo.io

**原文标题**: A ssh server that knows who you are. $ ssh whoami.filippo.io

**原文链接**: [https://github.com/FiloSottile/whoami.filippo.io](https://github.com/FiloSottile/whoami.filippo.io)

生成摘要时出错

---

## 99. Getting off US tech: a guide

**原文标题**: Getting off US tech: a guide

**原文链接**: [https://disconnect.blog/getting-off-us-tech-a-guide/](https://disconnect.blog/getting-off-us-tech-a-guide/)

生成摘要时出错

---

## 100. Refactoring – Not on the backlog (2014)

**原文标题**: Refactoring – Not on the backlog (2014)

**原文链接**: [https://ronjeffries.com/xprog/articles/refactoring-not-on-the-backlog/](https://ronjeffries.com/xprog/articles/refactoring-not-on-the-backlog/)

生成摘要时出错

---

