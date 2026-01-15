# Hacker News 热门文章摘要 (2026-01-15)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

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

## 11. Apple is fighting for TSMC capacity as Nvidia takes center stage

**原文标题**: Apple is fighting for TSMC capacity as Nvidia takes center stage

**原文链接**: [https://www.culpium.com/p/exclusiveapple-is-fighting-for-tsmc](https://www.culpium.com/p/exclusiveapple-is-fighting-for-tsmc)

生成摘要时出错

---

## 12. 一千张空白白卡

**原文标题**: 1000 Blank White Cards

**原文链接**: [https://en.wikipedia.org/wiki/1000_Blank_White_Cards](https://en.wikipedia.org/wiki/1000_Blank_White_Cards)

生成摘要时出错

---

## 13. So, you’ve hit an age gate. What now?

**原文标题**: So, you’ve hit an age gate. What now?

**原文链接**: [https://www.eff.org/deeplinks/2026/01/so-youve-hit-age-gate-what-now](https://www.eff.org/deeplinks/2026/01/so-youve-hit-age-gate-what-now)

生成摘要时出错

---

## 14. Find a pub that needs you

**原文标题**: Find a pub that needs you

**原文链接**: [https://www.ismypubfucked.com/](https://www.ismypubfucked.com/)

生成摘要时出错

---

## 15. Signal leaders warn agentic AI is an insecure, unreliable surveillance risk

**原文标题**: Signal leaders warn agentic AI is an insecure, unreliable surveillance risk

**原文链接**: [https://coywolf.com/news/productivity/signal-president-and-vp-warn-agentic-ai-is-insecure-unreliable-and-a-surveillance-nightmare/](https://coywolf.com/news/productivity/signal-president-and-vp-warn-agentic-ai-is-insecure-unreliable-and-a-surveillance-nightmare/)

生成摘要时出错

---

## 16. ASCII Clouds

**原文标题**: ASCII Clouds

**原文链接**: [https://caidan.dev/portfolio/ascii_clouds/](https://caidan.dev/portfolio/ascii_clouds/)

生成摘要时出错

---

## 17. Photos Capture the Breathtaking Scale of China's Wind and Solar Buildout

**原文标题**: Photos Capture the Breathtaking Scale of China's Wind and Solar Buildout

**原文链接**: [https://e360.yale.edu/digest/china-renewable-photo-essay](https://e360.yale.edu/digest/china-renewable-photo-essay)

生成摘要时出错

---

## 18. 25 Years of Wikipedia

**原文标题**: 25 Years of Wikipedia

**原文链接**: [https://wikipedia25.org](https://wikipedia25.org)

生成摘要时出错

---

## 19. I’m leaving Redis for SolidQueue

**原文标题**: I’m leaving Redis for SolidQueue

**原文链接**: [https://www.simplethread.com/redis-solidqueue/](https://www.simplethread.com/redis-solidqueue/)

生成摘要时出错

---

## 20. No management needed: anti-patterns in early-stage engineering teams

**原文标题**: No management needed: anti-patterns in early-stage engineering teams

**原文链接**: [https://www.ablg.io/blog/no-management-needed](https://www.ablg.io/blog/no-management-needed)

生成摘要时出错

---

## 21. GitHub should charge everyone $1 more per month to fund open source

**原文标题**: GitHub should charge everyone $1 more per month to fund open source

**原文链接**: [https://blog.greg.technology/2025/11/27/github-should-charge-1-dollar-more-per-month.html](https://blog.greg.technology/2025/11/27/github-should-charge-1-dollar-more-per-month.html)

生成摘要时出错

---

## 22. To those who fired or didn't hire tech writers because of AI

**原文标题**: To those who fired or didn't hire tech writers because of AI

**原文链接**: [https://passo.uno/letter-those-who-fired-tech-writers-ai/](https://passo.uno/letter-those-who-fired-tech-writers-ai/)

生成摘要时出错

---

## 23. Roam 50GB is now Roam 100GB

**原文标题**: Roam 50GB is now Roam 100GB

**原文链接**: [https://starlink.com/support/article/58c9c8b7-474e-246f-7e3c-06db3221d34d](https://starlink.com/support/article/58c9c8b7-474e-246f-7e3c-06db3221d34d)

生成摘要时出错

---

## 24. The Gleam Programming Language

**原文标题**: The Gleam Programming Language

**原文链接**: [https://gleam.run/](https://gleam.run/)

生成摘要时出错

---

## 25. Scaling long-running autonomous coding

**原文标题**: Scaling long-running autonomous coding

**原文链接**: [https://cursor.com/blog/scaling-agents](https://cursor.com/blog/scaling-agents)

生成摘要时出错

---

## 26. The insecure evangelism of LLM maximalists

**原文标题**: The insecure evangelism of LLM maximalists

**原文链接**: [https://lewiscampbell.tech/blog/260114.html](https://lewiscampbell.tech/blog/260114.html)

生成摘要时出错

---

## 27. The Influentists: AI hype without proof

**原文标题**: The Influentists: AI hype without proof

**原文链接**: [https://carette.xyz/posts/influentists/](https://carette.xyz/posts/influentists/)

生成摘要时出错

---

## 28. Every country should set 16 as the minimum age for social media accounts

**原文标题**: Every country should set 16 as the minimum age for social media accounts

**原文链接**: [https://www.afterbabel.com/p/why-every-country-should-set-16](https://www.afterbabel.com/p/why-every-country-should-set-16)

生成摘要时出错

---

## 29. Games Workshop bans staff from using AI

**原文标题**: Games Workshop bans staff from using AI

**原文链接**: [https://www.ign.com/articles/warhammer-maker-games-workshop-bans-its-staff-from-using-ai-in-its-content-or-designs-says-none-of-its-senior-managers-are-currently-excited-about-the-tech](https://www.ign.com/articles/warhammer-maker-games-workshop-bans-its-staff-from-using-ai-in-its-content-or-designs-says-none-of-its-senior-managers-are-currently-excited-about-the-tech)

生成摘要时出错

---

## 30. Raspberry Pi's New AI Hat Adds 8GB of RAM for Local LLMs

**原文标题**: Raspberry Pi's New AI Hat Adds 8GB of RAM for Local LLMs

**原文链接**: [https://www.jeffgeerling.com/blog/2026/raspberry-pi-ai-hat-2/](https://www.jeffgeerling.com/blog/2026/raspberry-pi-ai-hat-2/)

生成摘要时出错

---

## 31. Let's be honest, Generative AI isn't going all that well

**原文标题**: Let's be honest, Generative AI isn't going all that well

**原文链接**: [https://garymarcus.substack.com/p/lets-be-honest-generative-ai-isnt](https://garymarcus.substack.com/p/lets-be-honest-generative-ai-isnt)

生成摘要时出错

---

## 32. Verizon outages reported across U.S.

**原文标题**: Verizon outages reported across U.S.

**原文链接**: [https://www.firstcoastnews.com/article/news/nation-world/verizon-outage-reported/507-ef3cb3d0-f595-432f-9f84-d1690a5085a7](https://www.firstcoastnews.com/article/news/nation-world/verizon-outage-reported/507-ef3cb3d0-f595-432f-9f84-d1690a5085a7)

生成摘要时出错

---

## 33. Crafting Interpreters

**原文标题**: Crafting Interpreters

**原文链接**: [https://craftinginterpreters.com/](https://craftinginterpreters.com/)

生成摘要时出错

---

## 34. Show HN: OSS AI agent that indexes and searches the Epstein files

**原文标题**: Show HN: OSS AI agent that indexes and searches the Epstein files

**原文链接**: [https://epstein.trynia.ai/](https://epstein.trynia.ai/)

生成摘要时出错

---

## 35. Furiosa: 3.5x efficiency over H100s

**原文标题**: Furiosa: 3.5x efficiency over H100s

**原文链接**: [https://furiosa.ai/blog/introducing-rngd-server-efficient-ai-inference-at-data-center-scale](https://furiosa.ai/blog/introducing-rngd-server-efficient-ai-inference-at-data-center-scale)

生成摘要时出错

---

## 36. US freezes visas for 75 nations

**原文标题**: US freezes visas for 75 nations

**原文链接**: [https://english.mathrubhumi.com/news/world/us-visa-ban-public-charge-bjbpzu02](https://english.mathrubhumi.com/news/world/us-visa-ban-public-charge-bjbpzu02)

生成摘要时出错

---

## 37. The State of OpenSSL for pyca/cryptography

**原文标题**: The State of OpenSSL for pyca/cryptography

**原文链接**: [https://cryptography.io/en/latest/statements/state-of-openssl/](https://cryptography.io/en/latest/statements/state-of-openssl/)

生成摘要时出错

---

## 38. How have prices changed in a year? NPR checked 114 items at Walmart

**原文标题**: How have prices changed in a year? NPR checked 114 items at Walmart

**原文链接**: [https://www.npr.org/2026/01/14/nx-s1-5638908/walmart-prices-inflation-affordability-shrinkflation](https://www.npr.org/2026/01/14/nx-s1-5638908/walmart-prices-inflation-affordability-shrinkflation)

生成摘要时出错

---

## 39. Handy – Free open source speech-to-text app

**原文标题**: Handy – Free open source speech-to-text app

**原文链接**: [https://github.com/cjpais/Handy](https://github.com/cjpais/Handy)

生成摘要时出错

---

## 40. Government drops plans for mandatory digital ID to work in UK

**原文标题**: Government drops plans for mandatory digital ID to work in UK

**原文链接**: [https://www.bbc.com/news/articles/c3385zrrx73o](https://www.bbc.com/news/articles/c3385zrrx73o)

生成摘要时出错

---

## 41. Have Taken Up Farming

**原文标题**: Have Taken Up Farming

**原文链接**: [https://dylan.gr/1768295794](https://dylan.gr/1768295794)

生成摘要时出错

---

## 42. Minor says ICE took his iPhone, later found in used-electronics vending machine

**原文标题**: Minor says ICE took his iPhone, later found in used-electronics vending machine

**原文链接**: [https://www.propublica.org/article/videos-ice-dhs-immigration-agents-using-chokeholds-citizens](https://www.propublica.org/article/videos-ice-dhs-immigration-agents-using-chokeholds-citizens)

生成摘要时出错

---

## 43. Wind power slashed 4.6B euros off electricity bills in Spain last year

**原文标题**: Wind power slashed 4.6B euros off electricity bills in Spain last year

**原文链接**: [https://www.surinenglish.com/spain/wind-power-slashes-billion-euros-off-electricity-bills-20251217082020-nt.html](https://www.surinenglish.com/spain/wind-power-slashes-billion-euros-off-electricity-bills-20251217082020-nt.html)

生成摘要时出错

---

## 44. Bubblewrap: A nimble way to prevent agents from accessing your .env files

**原文标题**: Bubblewrap: A nimble way to prevent agents from accessing your .env files

**原文链接**: [https://patrickmccanna.net/a-better-way-to-limit-claude-code-and-other-coding-agents-access-to-secrets/](https://patrickmccanna.net/a-better-way-to-limit-claude-code-and-other-coding-agents-access-to-secrets/)

生成摘要时出错

---

## 45. Servo 2025 Stats

**原文标题**: Servo 2025 Stats

**原文链接**: [https://blogs.igalia.com/mrego/servo-2025-stats/](https://blogs.igalia.com/mrego/servo-2025-stats/)

生成摘要时出错

---

## 46. Anthropic Explicitly Blocking OpenCode

**原文标题**: Anthropic Explicitly Blocking OpenCode

**原文链接**: [https://gist.github.com/R44VC0RP/bd391f6a23185c0fed6c6b5fb2bac50e](https://gist.github.com/R44VC0RP/bd391f6a23185c0fed6c6b5fb2bac50e)

生成摘要时出错

---

## 47. Sun Position Calculator

**原文标题**: Sun Position Calculator

**原文链接**: [https://drajmarsh.bitbucket.io/earthsun.html](https://drajmarsh.bitbucket.io/earthsun.html)

生成摘要时出错

---

## 48. US to suspend immigrant visa processing for 75 nations, State Department says

**原文标题**: US to suspend immigrant visa processing for 75 nations, State Department says

**原文链接**: [https://www.reuters.com/world/us/us-suspend-visa-processing-75-nations-next-week-fox-news-reports-2026-01-14/](https://www.reuters.com/world/us/us-suspend-visa-processing-75-nations-next-week-fox-news-reports-2026-01-14/)

生成摘要时出错

---

## 49. 4k tons of potatoes to be given away for free in Berlin

**原文标题**: 4k tons of potatoes to be given away for free in Berlin

**原文链接**: [https://www.the-berliner.com/english-news-berlin/4000-tons-of-potatoes-to-be-given-away-for-free/](https://www.the-berliner.com/english-news-berlin/4000-tons-of-potatoes-to-be-given-away-for-free/)

生成摘要时出错

---

## 50. A university got itself banned from the Linux kernel (2021)

**原文标题**: A university got itself banned from the Linux kernel (2021)

**原文链接**: [https://www.theverge.com/2021/4/30/22410164/linux-kernel-university-of-minnesota-banned-open-source](https://www.theverge.com/2021/4/30/22410164/linux-kernel-university-of-minnesota-banned-open-source)

生成摘要时出错

---

## 51. Why NUKEMAP isn't on Google Maps anymore (2019)

**原文标题**: Why NUKEMAP isn't on Google Maps anymore (2019)

**原文链接**: [https://blog.nuclearsecrecy.com/2019/12/13/why-nukemap-isnt-on-google-maps-anymore/](https://blog.nuclearsecrecy.com/2019/12/13/why-nukemap-isnt-on-google-maps-anymore/)

生成摘要时出错

---

## 52. Show HN: Tiny FOSS Compass and Navigation App (<2MB)

**原文标题**: Show HN: Tiny FOSS Compass and Navigation App (<2MB)

**原文链接**: [https://github.com/CompassMB/MBCompass](https://github.com/CompassMB/MBCompass)

生成摘要时出错

---

## 53. Show HN: Nogic – VS Code extension that visualizes your codebase as a graph

**原文标题**: Show HN: Nogic – VS Code extension that visualizes your codebase as a graph

**原文链接**: [https://marketplace.visualstudio.com/items?itemName=Nogic.nogic](https://marketplace.visualstudio.com/items?itemName=Nogic.nogic)

生成摘要时出错

---

## 54. Never-before-seen Linux malware is "more advanced than typical"

**原文标题**: Never-before-seen Linux malware is "more advanced than typical"

**原文链接**: [https://arstechnica.com/security/2026/01/never-before-seen-linux-malware-is-far-more-advanced-than-typical/](https://arstechnica.com/security/2026/01/never-before-seen-linux-malware-is-far-more-advanced-than-typical/)

生成摘要时出错

---

## 55. Stop using natural language interfaces

**原文标题**: Stop using natural language interfaces

**原文链接**: [https://tidepool.leaflet.pub/3mcbegnuf2k2i](https://tidepool.leaflet.pub/3mcbegnuf2k2i)

生成摘要时出错

---

## 56. Epic fined €1.1M over manipulating children through in app purchases

**原文标题**: Epic fined €1.1M over manipulating children through in app purchases

**原文链接**: [https://nos.nl/artikel/2598157-maker-fortnite-vangt-bot-bij-rechter-moet-boete-betalen-voor-manipuleren-kinderen](https://nos.nl/artikel/2598157-maker-fortnite-vangt-bot-bij-rechter-moet-boete-betalen-voor-manipuleren-kinderen)

生成摘要时出错

---

## 57. System Programming in Linux: A Hands-On Introduction "Demo" Programs

**原文标题**: System Programming in Linux: A Hands-On Introduction "Demo" Programs

**原文链接**: [https://github.com/stewartweiss/intro-linux-sys-prog](https://github.com/stewartweiss/intro-linux-sys-prog)

生成摘要时出错

---

## 58. Denmark sends military reinforcements to Greenland

**原文标题**: Denmark sends military reinforcements to Greenland

**原文链接**: [https://www.dr.dk/nyheder/indland/groenland/efter-pres-fra-usa-danmark-er-nu-begyndt-sende-militaere-forstaerkninger-til-groenland](https://www.dr.dk/nyheder/indland/groenland/efter-pres-fra-usa-danmark-er-nu-begyndt-sende-militaere-forstaerkninger-til-groenland)

生成摘要时出错

---

## 59. Edge of Emulation: Game Boy Sewing Machines (2020)

**原文标题**: Edge of Emulation: Game Boy Sewing Machines (2020)

**原文链接**: [https://shonumi.github.io/articles/art22.html](https://shonumi.github.io/articles/art22.html)

生成摘要时出错

---

## 60. Show HN: Webctl – Browser automation for agents based on CLI instead of MCP

**原文标题**: Show HN: Webctl – Browser automation for agents based on CLI instead of MCP

**原文链接**: [https://github.com/cosinusalpha/webctl](https://github.com/cosinusalpha/webctl)

生成摘要时出错

---

## 61. OBS Studio 32.1.0 Beta 1 available

**原文标题**: OBS Studio 32.1.0 Beta 1 available

**原文链接**: [https://github.com/obsproject/obs-studio/releases/tag/32.1.0-beta1](https://github.com/obsproject/obs-studio/releases/tag/32.1.0-beta1)

生成摘要时出错

---

## 62. Native ZFS VDEV for Object Storage (OpenZFS Summit)

**原文标题**: Native ZFS VDEV for Object Storage (OpenZFS Summit)

**原文链接**: [https://www.zettalane.com/blog/openzfs-summit-2025-mayanas-objbacker.html](https://www.zettalane.com/blog/openzfs-summit-2025-mayanas-objbacker.html)

生成摘要时出错

---

## 63. How much of my observability data is waste?

**原文标题**: How much of my observability data is waste?

**原文链接**: [https://usetero.com/blog/the-question-your-observability-vendor-wont-answer](https://usetero.com/blog/the-question-your-observability-vendor-wont-answer)

生成摘要时出错

---

## 64. Why we don’t use AI

**原文标题**: Why we don’t use AI

**原文链接**: [https://yarnspinner.dev/blog/why-we-dont-use-ai/](https://yarnspinner.dev/blog/why-we-dont-use-ai/)

生成摘要时出错

---

## 65. New Safari developer tools provide insight into CSS Grid Lanes

**原文标题**: New Safari developer tools provide insight into CSS Grid Lanes

**原文链接**: [https://webkit.org/blog/17746/new-safari-developer-tools-provide-insight-into-css-grid-lanes/](https://webkit.org/blog/17746/new-safari-developer-tools-provide-insight-into-css-grid-lanes/)

生成摘要时出错

---

## 66. 'Elite': The Palantir App ICE Uses to Find Neighborhoods to Raid

**原文标题**: 'Elite': The Palantir App ICE Uses to Find Neighborhoods to Raid

**原文链接**: [https://werd.io/elite-the-palantir-app-ice-uses-to-find-neighborhoods-to-raid/](https://werd.io/elite-the-palantir-app-ice-uses-to-find-neighborhoods-to-raid/)

生成摘要时出错

---

## 67. LLMs are a 400-year-long confidence trick

**原文标题**: LLMs are a 400-year-long confidence trick

**原文链接**: [https://tomrenner.com/posts/400-year-confidence-trick/](https://tomrenner.com/posts/400-year-confidence-trick/)

生成摘要时出错

---

## 68. Show HN: Sparrow-1 – Audio-native model for human-level turn-taking without ASR

**原文标题**: Show HN: Sparrow-1 – Audio-native model for human-level turn-taking without ASR

**原文链接**: [https://www.tavus.io/post/sparrow-1-human-level-conversational-timing-in-real-time-voice](https://www.tavus.io/post/sparrow-1-human-level-conversational-timing-in-real-time-voice)

生成摘要时出错

---

## 69. French Court Orders Popular VPNs to Block More Pirate Sites, Despite Opposition

**原文标题**: French Court Orders Popular VPNs to Block More Pirate Sites, Despite Opposition

**原文链接**: [https://torrentfreak.com/french-court-orders-popular-vpns-to-block-more-pirate-sites-despite-opposition/](https://torrentfreak.com/french-court-orders-popular-vpns-to-block-more-pirate-sites-despite-opposition/)

生成摘要时出错

---

## 70. Instagram AI Influencers Are Defaming Celebrities with Sex Scandals

**原文标题**: Instagram AI Influencers Are Defaming Celebrities with Sex Scandals

**原文链接**: [https://www.404media.co/instagram-ai-influencers-are-defaming-celebrities-with-sex-scandals/](https://www.404media.co/instagram-ai-influencers-are-defaming-celebrities-with-sex-scandals/)

生成摘要时出错

---

## 71. The 3D Software Rendering Technology of 1998's Thief: The Dark Project (2019)

**原文标题**: The 3D Software Rendering Technology of 1998's Thief: The Dark Project (2019)

**原文链接**: [https://nothings.org/gamedev/thief_rendering.html](https://nothings.org/gamedev/thief_rendering.html)

生成摘要时出错

---

## 72. The 500k-ton typo: Why data center copper math doesn't add up

**原文标题**: The 500k-ton typo: Why data center copper math doesn't add up

**原文链接**: [https://investinglive.com/news/the-500000-ton-typo-why-data-center-copper-math-doesnt-add-up-20260113/](https://investinglive.com/news/the-500000-ton-typo-why-data-center-copper-math-doesnt-add-up-20260113/)

生成摘要时出错

---

## 73. Show HN: TinyCity – A tiny city SIM for MicroPython (Thumby micro console)

**原文标题**: Show HN: TinyCity – A tiny city SIM for MicroPython (Thumby micro console)

**原文链接**: [https://github.com/chrisdiana/TinyCity](https://github.com/chrisdiana/TinyCity)

生成摘要时出错

---

## 74. GitHub Incident

**原文标题**: GitHub Incident

**原文链接**: [https://www.githubstatus.com/incidents/q987xpbqjbpl](https://www.githubstatus.com/incidents/q987xpbqjbpl)

生成摘要时出错

---

## 75. Danish Armed Forces expand their presence and continue exercises in Greenland

**原文标题**: Danish Armed Forces expand their presence and continue exercises in Greenland

**原文链接**: [https://www.fmn.dk/en/news/2025/the-danish-armed-forces-expand-their-presence-and-continue-exercises-in-greenland-in-close-cooperation-with-allies/](https://www.fmn.dk/en/news/2025/the-danish-armed-forces-expand-their-presence-and-continue-exercises-in-greenland-in-close-cooperation-with-allies/)

生成摘要时出错

---

## 76. The <Geolocation> HTML Element

**原文标题**: The <Geolocation> HTML Element

**原文链接**: [https://developer.chrome.com/blog/geolocation-html-element](https://developer.chrome.com/blog/geolocation-html-element)

生成摘要时出错

---

## 77. GOG's new owner can't stand Windows either: 'It's such poor-quality software '

**原文标题**: GOG's new owner can't stand Windows either: 'It's such poor-quality software '

**原文链接**: [https://www.pcgamer.com/software/windows/gogs-new-owner-cant-stand-windows-either-its-such-poor-quality-software-i-cant-believe-it/](https://www.pcgamer.com/software/windows/gogs-new-owner-cant-stand-windows-either-its-such-poor-quality-software-i-cant-believe-it/)

生成摘要时出错

---

## 78. EU-US relationship is 'disintegrating,' says Germany's vice chancellor

**原文标题**: EU-US relationship is 'disintegrating,' says Germany's vice chancellor

**原文链接**: [https://www.politico.eu/article/europe-us-germany-vice-chancellor-lars-klingbeil-donald-trump/](https://www.politico.eu/article/europe-us-germany-vice-chancellor-lars-klingbeil-donald-trump/)

生成摘要时出错

---

## 79. US, for first time in 50 years, experienced negative net migration in 2025

**原文标题**: US, for first time in 50 years, experienced negative net migration in 2025

**原文链接**: [https://abcnews.go.com/US/us-1st-time-50-years-experienced-negative-net/story?id=129175522](https://abcnews.go.com/US/us-1st-time-50-years-experienced-negative-net/story?id=129175522)

生成摘要时出错

---

## 80. Open sourcing Dicer: Databricks's auto-sharder

**原文标题**: Open sourcing Dicer: Databricks's auto-sharder

**原文链接**: [https://www.databricks.com/blog/open-sourcing-dicer-databricks-auto-sharder](https://www.databricks.com/blog/open-sourcing-dicer-databricks-auto-sharder)

生成摘要时出错

---

## 81. Project SkyWatch (a.k.a. Wescam at Home)

**原文标题**: Project SkyWatch (a.k.a. Wescam at Home)

**原文链接**: [https://ianservin.com/2026/01/13/project-skywatch-aka-wescam-at-home/](https://ianservin.com/2026/01/13/project-skywatch-aka-wescam-at-home/)

生成摘要时出错

---

## 82. Denmark's struggle to break up with Silicon Valley

**原文标题**: Denmark's struggle to break up with Silicon Valley

**原文链接**: [https://www.politico.eu/article/denmark-declared-war-against-big-tech-digital-sovereignty/](https://www.politico.eu/article/denmark-declared-war-against-big-tech-digital-sovereignty/)

生成摘要时出错

---

## 83. The unbearable frustration of figuring out APIs

**原文标题**: The unbearable frustration of figuring out APIs

**原文链接**: [https://blog.ar-ms.me/thoughts/translation-cli/](https://blog.ar-ms.me/thoughts/translation-cli/)

生成摘要时出错

---

## 84. Python: Tprof, a Targeting Profiler

**原文标题**: Python: Tprof, a Targeting Profiler

**原文链接**: [https://adamj.eu/tech/2026/01/14/python-introducing-tprof/](https://adamj.eu/tech/2026/01/14/python-introducing-tprof/)

生成摘要时出错

---

## 85. CVEs Affecting the Svelte Ecosystem

**原文标题**: CVEs Affecting the Svelte Ecosystem

**原文链接**: [https://svelte.dev/blog/cves-affecting-the-svelte-ecosystem](https://svelte.dev/blog/cves-affecting-the-svelte-ecosystem)

生成摘要时出错

---

## 86. Design and Implementation of Sprites

**原文标题**: Design and Implementation of Sprites

**原文链接**: [https://fly.io/blog/design-and-implementation/](https://fly.io/blog/design-and-implementation/)

生成摘要时出错

---

## 87. Show HN: A 10KiB kernel for cloud apps

**原文标题**: Show HN: A 10KiB kernel for cloud apps

**原文链接**: [https://github.com/ReturnInfinity/BareMetal-Cloud](https://github.com/ReturnInfinity/BareMetal-Cloud)

生成摘要时出错

---

## 88. Running Lean at Scale

**原文标题**: Running Lean at Scale

**原文链接**: [https://harmonic.fun/news#blog-post-lean](https://harmonic.fun/news#blog-post-lean)

生成摘要时出错

---

## 89. Found: Medieval Cargo Ship – Largest Vessel of Its Kind Ever

**原文标题**: Found: Medieval Cargo Ship – Largest Vessel of Its Kind Ever

**原文链接**: [https://www.smithsonianmag.com/smart-news/archaeologists-say-theyve-unearthed-a-massive-medieval-cargo-ship-thats-the-largest-vessel-of-its-kind-ever-found-180987984/](https://www.smithsonianmag.com/smart-news/archaeologists-say-theyve-unearthed-a-massive-medieval-cargo-ship-thats-the-largest-vessel-of-its-kind-ever-found-180987984/)

生成摘要时出错

---

## 90. Starlink activates free internet in Iran

**原文标题**: Starlink activates free internet in Iran

**原文链接**: [https://www.cnn.com/2026/01/13/politics/starlink-access-iran-protests](https://www.cnn.com/2026/01/13/politics/starlink-access-iran-protests)

生成摘要时出错

---

## 91. The housing market isn't for single people

**原文标题**: The housing market isn't for single people

**原文链接**: [https://thewalrus.ca/the-housing-market-isnt-for-single-people/](https://thewalrus.ca/the-housing-market-isnt-for-single-people/)

生成摘要时出错

---

## 92. Inside The Internet Archive's Infrastructure

**原文标题**: Inside The Internet Archive's Infrastructure

**原文链接**: [https://hackernoon.com/the-long-now-of-the-web-inside-the-internet-archives-fight-against-forgetting](https://hackernoon.com/the-long-now-of-the-web-inside-the-internet-archives-fight-against-forgetting)

生成摘要时出错

---

## 93. The string theory hype machine will never die

**原文标题**: The string theory hype machine will never die

**原文链接**: [https://www.math.columbia.edu/~woit/wordpress/?p=15407](https://www.math.columbia.edu/~woit/wordpress/?p=15407)

生成摘要时出错

---

## 94. Choosing learning over autopilot

**原文标题**: Choosing learning over autopilot

**原文链接**: [https://anniecherkaev.com/choosing-learning-over-autopilot](https://anniecherkaev.com/choosing-learning-over-autopilot)

生成摘要时出错

---

## 95. Banning Things for Other People Is Easy

**原文标题**: Banning Things for Other People Is Easy

**原文链接**: [https://dogdogfish.com/blog/2026/01/14/banning-things-for-other-people/](https://dogdogfish.com/blog/2026/01/14/banning-things-for-other-people/)

生成摘要时出错

---

## 96. ChromaDB Explorer

**原文标题**: ChromaDB Explorer

**原文链接**: [https://www.chroma-explorer.com/](https://www.chroma-explorer.com/)

生成摘要时出错

---

## 97. US to suspend immigrant visa processing for 75 nations, State Department says

**原文标题**: US to suspend immigrant visa processing for 75 nations, State Department says

**原文链接**: [https://www.reuters.com/world/us/us-suspend-visa-processing-75-nations-next-week-fox-news-reports-2026-01-14/](https://www.reuters.com/world/us/us-suspend-visa-processing-75-nations-next-week-fox-news-reports-2026-01-14/)

生成摘要时出错

---

## 98. UK Officials could face US entry ban over Twitter policy

**原文标题**: UK Officials could face US entry ban over Twitter policy

**原文链接**: [https://parliamentnews.co.uk/uk-officials-could-face-us-entry-ban-over-x-policy](https://parliamentnews.co.uk/uk-officials-could-face-us-entry-ban-over-x-policy)

生成摘要时出错

---

## 99. Apple: You (Still) Don't Understand the Vision Pro

**原文标题**: Apple: You (Still) Don't Understand the Vision Pro

**原文链接**: [https://stratechery.com/2026/apple-you-still-dont-understand-the-vision-pro/](https://stratechery.com/2026/apple-you-still-dont-understand-the-vision-pro/)

生成摘要时出错

---

## 100. Germany joins European partners with troop deployment to Greenland

**原文标题**: Germany joins European partners with troop deployment to Greenland

**原文链接**: [https://www.reuters.com/world/europe/germany-send-reconnaissance-troops-greenland-government-says-2026-01-14/](https://www.reuters.com/world/europe/germany-send-reconnaissance-troops-greenland-government-says-2026-01-14/)

生成摘要时出错

---

