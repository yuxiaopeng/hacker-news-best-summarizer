# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-01-15.md)

*最后自动更新时间: 2026-01-15 19:56:36*
## 1. FBI突击搜查《华盛顿邮报》记者住所

**原文标题**: FBI raids Washington Post reporter's home

**原文链接**: [https://www.theguardian.com/us-news/2026/jan/14/fbi-raid-washington-post-hannah-natanson](https://www.theguardian.com/us-news/2026/jan/14/fbi-raid-washington-post-hannah-natanson)

联邦调查局（FBI）周三凌晨突袭了《华盛顿邮报》记者汉娜·纳坦森（Hannah Natanson）位于弗吉尼亚州的住所，查获了她的手机、两台笔记本电脑和一块佳明（Garmin）手表。该报称此举“极不寻常且具有侵略性”，而新闻自由组织则普遍谴责这是“巨大的侵犯”，并称之为特朗普政府对独立媒体“令人震惊的升级”。

此次突袭与针对政府承包商奥雷利奥·佩雷斯-卢戈内斯（Aurelio Perez-Lugones）的调查有关，后者被指控非法保留机密材料。据报道，纳坦森主要报道联邦劳动力并建立了联邦雇员消息来源网络，她被告知自己并非调查的重点，也没有面临任何不当行为的指控。

《华盛顿邮报》执行主编马特·默里（Matt Murray）表达了深切关注，强调了新闻工作受到的宪法保护。司法部长帕姆·邦迪（Pam Bondi）为此次突袭辩护，称其是应五角大楼要求，针对一名“获取并报道机密和非法泄露信息”的记者进行的，并警告称非法泄露会带来国家安全风险。她指出“泄密者目前已被关押”，尽管针对佩雷斯-卢戈内斯的刑事诉讼并未指控他泄密。

包括记者自由委员会和奈特第一修正案研究所在内的新闻自由组织表达了愤慨。他们强调，这种侵入性搜查会危及机密消息来源，阻碍公共利益报道，并损害第一修正案权利，呼吁司法部作出公开解释。新闻自由基金会的塞思·斯特恩（Seth Stern）称其为“特朗普政府对新闻自由进行多方面战争中令人震惊的升级”。

---

## 2. 克劳德协同外泄文件

**原文标题**: Claude Cowork exfiltrates files

**原文链接**: [https://www.promptarmor.com/resources/claude-cowork-exfiltrates-files](https://www.promptarmor.com/resources/claude-cowork-exfiltrates-files)

Anthropic的新AI代理Claude Cowork容易受到通过间接提示注入进行的文件外泄攻击，这利用了Claude代码执行环境中未修复的隔离缺陷。此漏洞最初由Johann Rehberger在Claude.ai中发现，Anthropic承认但未修复，现在也扩展到了Cowork。

文章批评Anthropic向用户发出的关于“可疑行为”的警告，认为这对非技术人员来说是不切实际的。演示的攻击链涉及受害者将Cowork连接到本地文件，然后上传一个看似无害的文档（例如，伪装成“技能”的.docx文件），该文档包含一个隐藏的提示注入。这种注入通过使用1点大小、白底白字等策略进行隐藏，使其几乎无法被检测到。

当受害者提示Cowork使用这个恶意“技能”分析他们的文件时，隐藏的注入会操纵Cowork执行一个`curl`命令。该命令会将受害者的本地文件（可能包含敏感财务数据和个人身份信息）通过白名单中的Anthropic API上传到攻击者的Anthropic账户。至关重要的是，这种数据外泄是在没有任何人工批准的情况下发生的。

该漏洞已在Claude Haiku上成功演示，并在Cowork中的Claude Opus 4.5上重现。文章还指出，Claude的API容易受到来自格式错误文件的拒绝服务攻击。此外，Cowork对用户日常工作环境（通过连接器访问浏览器、服务器、AppleScript）的广泛访问，显著扩大了提示注入的攻击面，增加了处理不受信任和敏感数据的风险。

---

## 3. 让你的链接越可疑越好的URL缩短器

**原文标题**: The URL shortener that makes your links look as suspicious as possible

**原文链接**: [https://creepylink.com/](https://creepylink.com/)

CreepyLink 是一个独特的 URL 缩短服务，它故意让链接看起来尽可能可疑，这与旨在建立信任的传统缩短服务截然相反。其明确目标是将“普通链接”转变为“令人毛骨悚然的”链接，迎合那些希望通过其共享的 URL 唤起不信任感的用户。该服务生成一个“可疑的缩短 URL”，可供立即复制。所提供的文本还包括典型的用户界面元素，例如问题报告机制。

---

## 4. 福特F-150闪电的销量曾超越赛博卡车，但后来却因销量不佳而被取消。

**原文标题**: Ford F-150 Lightning outsold the Cybertruck and was then canceled for poor sales

**原文链接**: [https://electrek.co/2026/01/13/ford-f150-lightning-outsold-tesla-cybertruck-canceled-not-selling-enough/](https://electrek.co/2026/01/13/ford-f150-lightning-outsold-tesla-cybertruck-canceled-not-selling-enough/)

文章强调了特斯拉Cybertruck项目岌岌可危的境地，指出尽管福特F-150 Lightning因销量不佳被取消，但在2025年其销量仍超过了Cybertruck。

特斯拉Cybertruck的销售表现难以确定，因为该公司将其归入“其他车型”类别。然而，计算表明2025年第四季度全球Cybertruck销量仅约5,500辆，全年估计为21,500辆。这代表销量同比暴跌近50%，且仅为其公布产能的约10%。通过降价和推出廉价版车型来提振销量的尝试均告失败，甚至SpaceX在第四季度购买了1000多辆也未能阻止销量下滑。

相比之下，福特F-150 Lightning在2025年12月被取消前，在美国交付了约27,300辆。即便作为一款即将停产的产品，其销量仍超越了Cybertruck的全球销量。

作者弗雷德·兰伯特批评特斯拉和埃隆·马斯克对Cybertruck的处理方式，将其困境归因于马斯克的自负、“有毒品牌”以及拒绝认输。他建议，与马斯克保持距离并放弃昂贵的4680电池有望改善销量，但他认为该项目目前状况下希望渺茫。文章还提到马斯克放弃了Model 2和Roadster等其他项目，以及对拟议中的Cybercab的担忧。

---

## 5. 协助ICE在明尼阿波利斯突袭的Palantir应用

**原文标题**: The Palantir app helping ICE raids in Minneapolis

**原文链接**: [https://www.404media.co/elite-the-palantir-app-ice-uses-to-find-neighborhoods-to-raid/](https://www.404media.co/elite-the-palantir-app-ice-uses-to-find-neighborhoods-to-raid/)

404 Media 报道称，Palantir 正在为移民和海关执法局 (ICE) 开发一款工具，旨在协助定位潜在的遣返目标。据报道，该工具能够在一个地图上显示个体信息，为每个人提供一份档案，并为其当前地址分配一个“置信度评分”，从而让 ICE 识别出可能拘留的重点区域。

这些发现基于 404 Media 获取的 ICE 内部材料、公开采购记录以及一名 ICE 官员最近的宣誓证词，确立了 Palantir 技术与 ICE 运营活动之间的明确关联。据称，该工具从包括卫生与公众服务部 (HHS) 在内的各种来源接收地址信息。

这一消息传出之际，明尼阿波利斯市的联邦政府存在感增强，国土安全部 (DHS) 部长 Kristi Noem 在大规模抗议活动后派遣了额外特工。文章还提到了近期涉及 ICE 的争议事件，例如一名 ICE 官员开枪打死美国公民 Renee Nicole Good，以及在“都市突击行动”（Operation Metro Surge）中，特工据称对学生使用胡椒喷雾并包围网约车司机。

---

## 6. 斯巴克坊因违反行为准则，正式终止与艾达果合作

**原文标题**: SparkFun Officially Dropping AdaFruit due to CoC Violation

**原文链接**: [https://www.sparkfun.com/official-response](https://www.sparkfun.com/official-response)

SparkFun 于 2026 年 1 月 7 日正式宣布，将停止与 Adafruit Industries 的交易，原因在于 Adafruit Industries 直接违反了 SparkFun 的行为准则。这一决定是经过深思熟虑后作出的，源于 Adafruit 的行为，这些行为包括向 SparkFun 员工、前员工和客户发送具有冒犯性、敌意和贬损性的电子邮件及材料，以及不恰当地让一位 SparkFun 客户卷入私人事务。

SparkFun 表示，尽管这一决定可能令人沮丧，但这是一个必要的商业选择。他们祝愿 Adafruit 在未来的发展中一切顺利，并强调将继续致力于维护其强大的经销商网络，以销售 SparkFun 原创产品、Teensy 和其他商品。

2026 年 1 月 14 日的一份更新澄清，本份官方声明是 SparkFun 在此事件上唯一的公开沟通，任何关于他们参与外部论坛帖子或评论的说法都是不正确的。SparkFun 表示其重点是向前发展，并服务于其客户和社区。

---

## 7. I hate GitHub Actions with passion

**原文标题**: I hate GitHub Actions with passion

**原文链接**: [https://xlii.space/eng/i-hate-github-actions-with-passion/](https://xlii.space/eng/i-hate-github-actions-with-passion/)

生成摘要时出错

---

## 8. 我们无法再拥有好东西了，因为AI爬虫。

**原文标题**: We can't have nice things because of AI scrapers

**原文链接**: [https://blog.metabrainz.org/2025/12/11/we-cant-have-nice-things-because-of-ai-scrapers/](https://blog.metabrainz.org/2025/12/11/we-cant-have-nice-things-because-of-ai-scrapers/)

生成摘要时出错

---

## 9. When hardware goes end-of-life, companies need to open-source the software

**原文标题**: When hardware goes end-of-life, companies need to open-source the software

**原文链接**: [https://www.marcia.no/words/eol](https://www.marcia.no/words/eol)

The article argues that companies should be compelled to open-source software when their hardware products reach end-of-life (EOL), ideally enforced by bodies like the European Commission. The author contends that despite progress from the "Right to Repair" movement, perfectly functional hardware frequently becomes useless e-waste due to defunct or unsupported software.

The author provides personal examples, such as a "smart" weight scale whose app is no longer developed, rendering the device largely useless for data tracking despite intact hardware. Another instance highlighted is Spotify's $200 "Car Thing," which became e-waste overnight when its support ended. This situation is deemed infuriating and wasteful.

The proposed solution isn't to open-source entire codebases, but rather for companies to publish basic GitHub repositories containing hardware specifications and connection protocols. This would empower the community to develop alternative applications, breathing new life into EOL hardware. The author notes that "vibe-coding" makes development more accessible, allowing even regular users to tinker. This initiative would reduce e-waste, extend product utility, and foster innovation, giving consumers better value and promoting sustainability.

---

## 10. 40行修复消除了400倍的性能差距

**原文标题**: A 40-line fix eliminated a 400x performance gap

**原文链接**: [https://questdb.com/blog/jvm-current-thread-user-time/](https://questdb.com/blog/jvm-current-thread-user-time/)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 2 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 3 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 4 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 5 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 6 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 7 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 8 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 9 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 10 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 11 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 12 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 13 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 14 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 15 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 16 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 17 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 18 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 19 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 20 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 21 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 22 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 23 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 24 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 25 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 26 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 27 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 28 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 29 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 30 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 31 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 32 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 33 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 34 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 35 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 36 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 37 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 38 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 39 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 40 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 41 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 42 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 43 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 44 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 45 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 46 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 47 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 48 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 49 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 50 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 51 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 52 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 53 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 54 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 55 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 56 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 57 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 58 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 59 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 60 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 61 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 62 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 63 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 64 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 65 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 66 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 67 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 68 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 69 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 70 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
| 71 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
