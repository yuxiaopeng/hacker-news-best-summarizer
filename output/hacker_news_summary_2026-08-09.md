# Hacker News 热门文章摘要 (2026-08-09)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. Windows 11 自带的天气应用浪费超过 1 GB 的内存

**原文标题**: Windows 11's built-in Weather app wastes more than 1 GB of RAM

**原文链接**: [https://www.notebookcheck.net/Windows-11-s-built-in-Weather-app-wastes-more-than-1-GB-of-RAM.1364205.0.html](https://www.notebookcheck.net/Windows-11-s-built-in-Weather-app-wastes-more-than-1-GB-of-RAM.1364205.0.html)

Windows 11 内置的天气应用被发现占用超过 1 GB 的 RAM，这严重拖累了电脑（PC）效率，尤其是在内存有限的系统上。Windows Latest 和 Wccftech 的测试显示，该应用在显示天气预报时占用超过 1.2 GB，而在进行缩放等基本交互时甚至高达 1.5–1.6 GB。这大大高于苹果 macOS 天气应用（内存占用不到 250 MB）。

内存占用过高归因于该应用并非完全原生的 Windows 应用程序。相反，它是一个基于微软 WebView2 框架构建的 MSN 天气网页应用，该框架运行多个基于 Chromium 的子进程。虽然配备 32 GB 以上 RAM 的高端电脑可能不会注意到其影响，但内存为 8 GB 或 16 GB 的入门级系统可能会经历更大的内存压力，导致对页面文件的依赖增加，并降低系统响应速度。

进一步的批评源于该应用在其界面中包含赞助内容。这种高内存消耗和广告的存在与微软最近为提高 Windows 11 效率、增强低端硬件性能以及为操作系统开发更多原生应用程序所做的努力背道而驰。

---

## 2. 领英动态屏蔽

**原文标题**: LinkedIn Feed Blocker

**原文链接**: [https://github.com/andrewpollack/linkedin-feed-blocker](https://github.com/andrewpollack/linkedin-feed-blocker)

“领英动态屏蔽器”是一个轻量级的 Chrome 扩展程序，旨在禁用领英的主页动态，同时保持其他功能可用。它的主要目的是隐藏 `/feed` 页面上的整个主动态，并阻止无限滚动的信息流分页，让用户能够专注于求职、个人资料、消息和通知等专业功能，而不受社交动态的干扰。

开发者创建此扩展程序是因为他们重视领英在求职和与招聘人员互动方面的作用，但却不喜欢其“狂野西部”式的社交动态。

目前，该扩展程序正在等待 Chrome 网上应用店的审核，用户可以通过下载其代码库、在 `chrome://extensions` 中启用开发者模式并加载解压后的目录来手动安装。

从技术上讲，它通过使用 `feed.css` 来隐藏主动态元素（具体为 `[data-testid="mainFeed"] { display: none !important; }`），并使用 `rules.json` 通过专门针对领英的 `mainFeed` 分页器（即 `sduiid=com.linkedin.sdui.pagers.feed.mainFeed`）来阻止对更多主动态帖子的请求，从而防止干扰平台其他部分的功能。

---

## 3. Gentoo bugzilla closed due AI bot scraper overload

**原文标题**: Gentoo bugzilla closed due AI bot scraper overload

**原文链接**: [https://social.treehouse.systems/@mgorny/117058483039362779](https://social.treehouse.systems/@mgorny/117058483039362779)

Gentoo 的官方缺陷追踪系统 Bugzilla 已被关闭。此次关闭归因于人工智能机器人爬虫造成的过载。

这一举动得到了 Jesus Michał von Gentoo（一位可能是开发人员或管理员）的证实，他通过 Treehouse Mastodon 宣布他已关闭该系统。虽然他提供的直接引述不完整，但文章标题明确指出“人工智能机器人爬虫过载”是关闭的原因。

---

## 4. 褪黑素损害健康青年人晨间认知 (2023)

**原文标题**: Melatonin impairs morning cognition in healthy young adults (2023)

**原文链接**: [https://academic.oup.com/sleep/article/46/Supplement_1/A34/7181621](https://academic.oup.com/sleep/article/46/Supplement_1/A34/7181621)

一项研究调查了28名健康青年人（18-35岁）中褪黑素对晨间认知能力的影响。该研究采用双盲、随机、安慰剂对照、交叉设计，参与者在睡前30分钟服用5毫克褪黑素或安慰剂。次日上午8点进行认知能力评估。

结果显示，根据卡罗林斯卡困倦量表测量，褪黑素显著增加了主观困倦感。客观上，褪黑素损害了精神运动警觉性，在精神运动警觉测试中导致反应时间变慢和失误增多。工作记忆也受到负面影响，在n-back任务中观察到准确性下降和反应时间增加。此外，抑制控制能力受损，表现为Go/No-Go任务中执行错误的增加。然而，未发现对言语学习或数字广度有显著影响。

该研究得出结论，急性服用5毫克褪黑素会显著损害健康青年人的晨间警觉性、精神运动警觉性、工作记忆和抑制控制能力。这些发现强调了在使用褪黑素时需谨慎，尤其是在需要最佳晨间认知表现的情况下。

---

## 5. 欧洲的免费卫星服务刚让追踪野火变得更容易。

**原文标题**: Europe's free satellite service just made it easier to track wildfires

**原文链接**: [https://arstechnica.com/gadgets/2026/08/europes-free-satellite-service-just-made-it-easier-to-track-wildfires/](https://arstechnica.com/gadgets/2026/08/europes-free-satellite-service-just-made-it-easier-to-track-wildfires/)

Europe's free Copernicus Browser, providing satellite imagery from the European Space Agency's Sentinel-2 mission, has significantly improved its wildfire tracking capabilities. On August 4, a new, straightforward "wildfires" visualization layer was added, making it easier for anyone to monitor active fires (white/yellow), burning vegetation (red), and burned landscapes (dark brown/black).

This enhancement stems from a JavaScript script developed by remote sensing expert Pierre Markuse. The script combines visible red, narrow near-infrared, and short-wave infrared 2 bands to differentiate between healthy and burned vegetation and reveal soil moisture levels in burned areas. Previously, users had to manually add this script. However, Simon Proud, a mission scientist for Sentinel-2, successfully advocated for its integration as a default option.

Sentinel-2 imagery offers multi-spectral imaging at a granular 10-meter resolution, providing a significant advantage over other free services like NASA's FIRMS tool, which typically offers coarser resolutions down to 250 meters. While Sentinel-2 updates every few days compared to FIRMS's rapid hourly updates, its higher resolution makes it arguably the best free and publicly available tool for detailed wildfire monitoring. This development is particularly timely as climate change exacerbates wildfire seasons globally, impacting regions from Washington and Oregon to Canada, France, and Spain.

---

## 6. 任意阶幻方六边形存在

**原文标题**: There Are Magic Hexagons of Every Order

**原文链接**: [https://gukov.dev/math/2026/08/02/new-magic-hexagons.html](https://gukov.dev/math/2026/08/02/new-magic-hexagons.html)

生成摘要时出错

---

## 7. 激励是给失败者的。

**原文标题**: Incentives are for losers

**原文链接**: [https://www.experimental-history.com/p/incentives-are-for-losers](https://www.experimental-history.com/p/incentives-are-for-losers)

文章《激励是给失败者的》反对普遍存在的“人们应该服从激励”的观念，称这种行为是缺乏尊严的。它认为，真正的人类发展在于培养个人的目标感和完善自己的道德指南针，而不是被任意的奖励系统所左右。如果没有这种内在目标，个人就会成为“激励最大化者”，被对金钱、权力、名声的“肿瘤般欲望”所驱动，即使取得外部成功，也往往导致一种“精神上软弱无力”的存在。

作者提出，建立一个强大的价值观体系是一种困难的后天习得技能，而非与生俱来的能力。对“道德治疗性自然神论”和“解释深度错觉”的研究表明，大多数人的道德和宗教信仰是模糊的，容易被覆盖，直到受到深刻挑战。

为了培养真正的信念，一个人必须“凝视一条鱼并为之疯狂”——面对一条“可怕的大鱼”，一个未经审视的假设，它要求对生命进行彻底的重新评估。作者将他自己的“鱼”描述为：意识到学术界的社会正义论述与会议酒店外的苦难脱节，这促使他离开了学术界。他引用了参议员查尔斯·萨姆纳（Charles Sumner）的例子，萨姆纳为他的废奴主义信念而抵抗暴力，其“道德清算”造就了非凡的正直，不受外部激励的影响。最终，这篇文章提倡锻造自我的道德准则，而非服从外部奖励系统。

---

## 8. Analyzing data from Silicon Valley ventures and founders prosecuted for fraud

**原文标题**: Analyzing data from Silicon Valley ventures and founders prosecuted for fraud

**原文链接**: [https://pubsonline.informs.org/doi/full/10.1287/orsc.2024.19981](https://pubsonline.informs.org/doi/full/10.1287/orsc.2024.19981)

无法访问文章链接。

---

## 9. 微软 Word Windows 1.1a 版，原生 X64 移植

**原文标题**: Microsoft Word for Windows 1.1a, Native X64 Port

**原文链接**: [https://github.com/jmarshall23/msword](https://github.com/jmarshall23/msword)

生成摘要时出错

---

## 10. Message your other Claude Code sessions

**原文标题**: Message your other Claude Code sessions

**原文链接**: [https://code.claude.com/docs/en/cross-session-messaging](https://code.claude.com/docs/en/cross-session-messaging)

生成摘要时出错

---

## 11. Tom Stanton's supersonic trebuchet breaks sound barrier with gravity alone

**原文标题**: Tom Stanton's supersonic trebuchet breaks sound barrier with gravity alone

**原文链接**: [https://www.techeblog.com/tom-stanton-supersonic-trebuchet/](https://www.techeblog.com/tom-stanton-supersonic-trebuchet/)

生成摘要时出错

---

## 12. Everything You Do Is Being Recorded

**原文标题**: Everything You Do Is Being Recorded

**原文链接**: [https://www.theatlantic.com/technology/2026/05/ai-wearable-surveillance-countermeasures/687203/](https://www.theatlantic.com/technology/2026/05/ai-wearable-surveillance-countermeasures/687203/)

The article warns that everyday individuals may soon need to adopt extreme anti-surveillance measures, previously reserved for criminals and spies, due to the rise of AI-enabled wearable recording devices. Companies like Apple are reportedly developing AI pins or pendants that could constantly listen and record, making ubiquitous surveillance a reality.

This technological advancement has sparked a new 'arms race.' While traditional jammers used white noise or inaudible ultrasonic frequencies to disrupt recordings, modern AI wearables employ sophisticated speech-recovery algorithms. These algorithms, developed through extensive research for hearing aids and teleconferencing, can strip away unwanted noise—including jamming signals—and even reconstruct missing speech from highly complex sound environments, effectively solving the "cocktail party problem."

In response, new countermeasures are emerging. Strategies include "obfuscation," such as supplying junk data to confuse algorithms (e.g., anti-facial recognition makeup, decoy web searches). More advanced audio jammers like MicFrozen generate real-time "anti-speech" or counterfeit speech-shaped sounds to mislead recording devices. Deveillance's Spectre I also aims to prevent recording and detect microphones.

However, the article highlights a significant imbalance: billions of dollars are invested in AI speech processing by major tech corporations, vastly outmatching the limited resources available for privacy countermeasures from a few academics and small companies. Experts predict that AI will likely maintain an edge, potentially even bypassing audio altogether through lip-reading or analyzing surface vibrations. The 'cat and mouse' game, the author concludes, often favors the powerful 'cat' – the corporations – a scenario previously witnessed in law enforcement's successful infiltration of criminal organizations' secure communication systems.

---

## 13. Gateway 2000's hilariously bad ads in the 90s (Part II)

**原文标题**: Gateway 2000's hilariously bad ads in the 90s (Part II)

**原文链接**: [https://buttondown.com/suchbadtechads/archive/gateway-2000-part-2/](https://buttondown.com/suchbadtechads/archive/gateway-2000-part-2/)

生成摘要时出错

---

## 14. Illinois just told every operating system to start reporting your kid's age

**原文标题**: Illinois just told every operating system to start reporting your kid's age

**原文链接**: [https://itsfoss.com/news/illinois-age-verification-bill/](https://itsfoss.com/news/illinois-age-verification-bill/)

生成摘要时出错

---

## 15. Maryland Closes More of Cunningham Falls State Park After Second Beaver Attack

**原文标题**: Maryland Closes More of Cunningham Falls State Park After Second Beaver Attack

**原文链接**: [https://news.maryland.gov/dnr/2026/08/05/dnr-closes-additional-areas-of-cunningham-falls-state-park-following-second-beaver-attack/](https://news.maryland.gov/dnr/2026/08/05/dnr-closes-additional-areas-of-cunningham-falls-state-park-following-second-beaver-attack/)

生成摘要时出错

---

## 16. Should you stop cracking your knuckles?

**原文标题**: Should you stop cracking your knuckles?

**原文链接**: [https://www.bbc.com/future/article/20260807-should-i-stop-cracking-my-knuckles](https://www.bbc.com/future/article/20260807-should-i-stop-cracking-my-knuckles)

生成摘要时出错

---

## 17. Cool URIs Don't Change (1998)

**原文标题**: Cool URIs Don't Change (1998)

**原文链接**: [https://www.w3.org/Provider/Style/URI](https://www.w3.org/Provider/Style/URI)

生成摘要时出错

---

## 18. Reviving a four year old reMarkable 2

**原文标题**: Reviving a four year old reMarkable 2

**原文链接**: [https://oskrim.github.io/hardware/2026/08/09/remarkable-over-ssh.html](https://oskrim.github.io/hardware/2026/08/09/remarkable-over-ssh.html)

生成摘要时出错

---

## 19. John C. Lilly on solid state intelligence and the elimination of man (1978)

**原文标题**: John C. Lilly on solid state intelligence and the elimination of man (1978)

**原文链接**: [https://kibotronics.net/unlisted/lilly-machines/](https://kibotronics.net/unlisted/lilly-machines/)

生成摘要时出错

---

## 20. TheoremDB – A public workspace for machine mathematics

**原文标题**: TheoremDB – A public workspace for machine mathematics

**原文链接**: [https://theoremdb.org/](https://theoremdb.org/)

生成摘要时出错

---

## 21. Psychological Warfare in Reverse Engineering (2015)

**原文标题**: Psychological Warfare in Reverse Engineering (2015)

**原文链接**: [https://github.com/xoreaxeaxeax/repsych](https://github.com/xoreaxeaxeax/repsych)

生成摘要时出错

---

## 22. CSS: The bomb inside your inbox

**原文标题**: CSS: The bomb inside your inbox

**原文链接**: [https://portswigger.net/research/css-the-bomb-inside-your-inbox](https://portswigger.net/research/css-the-bomb-inside-your-inbox)

生成摘要时出错

---

## 23. Software Giant SAP Stops Most Travel and Hiring Because of AI's Soaring Cost

**原文标题**: Software Giant SAP Stops Most Travel and Hiring Because of AI's Soaring Cost

**原文链接**: [https://www.404media.co/software-giant-sap-stops-most-travel-and-hiring-because-of-ais-soaring-cost/](https://www.404media.co/software-giant-sap-stops-most-travel-and-hiring-because-of-ais-soaring-cost/)

生成摘要时出错

---

## 24. Voyager 1 FDS Computer Emulator

**原文标题**: Voyager 1 FDS Computer Emulator

**原文链接**: [https://zaneham.github.io/voyager-fds-emulator/](https://zaneham.github.io/voyager-fds-emulator/)

生成摘要时出错

---

## 25. Show HN: A Project Oberon System version running on RISC-V instead of RISC-5

**原文标题**: Show HN: A Project Oberon System version running on RISC-V instead of RISC-5

**原文链接**: [https://github.com/rochus-keller/OberonSystem/tree/op2-rv32](https://github.com/rochus-keller/OberonSystem/tree/op2-rv32)

生成摘要时出错

---

## 26. Mythos social engineering AISI INC-2026-07-28-01

**原文标题**: Mythos social engineering AISI INC-2026-07-28-01

**原文链接**: [https://web.archive.org/web/20260731053721/http://github.com/ancaferro/myNetwork/pull/3](https://web.archive.org/web/20260731053721/http://github.com/ancaferro/myNetwork/pull/3)

生成摘要时出错

---

## 27. FCC moves to ban Lidar-equipped foreign drones from US

**原文标题**: FCC moves to ban Lidar-equipped foreign drones from US

**原文链接**: [https://www.tomshardware.com/tech-industry/drones/fcc-moves-to-ban-lidar-equipped-foreign-drones-from-us-classifies-the-technology-as-military-grade-in-a-proposal-that-could-also-hit-thermal-models-and-the-swarms-used-drone-light-shows](https://www.tomshardware.com/tech-industry/drones/fcc-moves-to-ban-lidar-equipped-foreign-drones-from-us-classifies-the-technology-as-military-grade-in-a-proposal-that-could-also-hit-thermal-models-and-the-swarms-used-drone-light-shows)

生成摘要时出错

---

## 28. Tech sucks: You have to vote with your wallet, or nothing will change

**原文标题**: Tech sucks: You have to vote with your wallet, or nothing will change

**原文链接**: [https://82mhz.net/posts/2026/08/tech-sucks-you-have-to-vote-with-your-wallet-or-nothing-will-change/](https://82mhz.net/posts/2026/08/tech-sucks-you-have-to-vote-with-your-wallet-or-nothing-will-change/)

生成摘要时出错

---

## 29. Making an AI bid writer refuse to lie

**原文标题**: Making an AI bid writer refuse to lie

**原文链接**: [https://ailucius.com/blog/making-an-ai-bid-writer-refuse-to-lie](https://ailucius.com/blog/making-an-ai-bid-writer-refuse-to-lie)

生成摘要时出错

---

