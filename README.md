# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-08-09.md)

*最后自动更新时间: 2026-08-09 19:51:03*
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

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-08-09](output/hacker_news_summary_2026-08-09.md) |
| 2 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 3 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 4 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 5 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 6 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 7 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 8 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 9 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 10 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 11 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 12 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 13 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 14 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 15 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 16 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 17 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 18 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 19 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 20 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 21 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 22 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 23 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 24 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 25 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 26 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 27 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 28 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 29 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 30 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 31 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 32 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 33 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 34 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 35 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 36 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 37 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 38 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 39 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 40 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 41 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 42 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 43 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 44 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 45 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 46 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 47 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 48 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 49 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 50 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 51 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 52 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 53 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 54 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 55 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 56 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 57 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 58 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 59 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 60 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 61 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 62 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 63 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 64 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 65 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 66 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 67 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 68 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 69 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 70 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 71 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 72 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 73 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 74 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 75 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 76 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 77 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 78 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 79 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 80 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 81 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 82 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 83 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 84 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 85 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 86 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 87 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 88 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 89 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 90 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 91 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 92 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 93 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 94 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 95 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 96 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 97 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 98 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 99 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 100 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 101 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 102 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 103 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 104 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 105 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 106 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 107 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 108 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 109 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 110 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 111 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 112 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 113 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 114 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 115 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 116 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 117 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 118 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 119 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 120 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 121 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 122 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 123 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 124 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 125 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 126 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 127 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 128 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 129 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 130 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 131 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 132 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 133 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 134 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 135 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 136 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 137 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 138 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 139 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 140 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 141 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 142 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 143 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 144 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 145 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 146 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 147 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 148 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 149 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 150 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 151 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 152 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 153 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 154 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 155 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 156 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 157 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 158 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 159 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 160 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 161 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 162 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 163 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 164 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 165 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 166 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 167 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 168 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 169 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 170 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 171 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 172 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 173 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 174 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 175 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 176 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 177 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 178 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 179 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 180 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 181 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 182 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 183 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 184 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 185 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 186 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 187 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 188 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 189 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 190 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 191 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 192 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 193 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 194 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 195 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 196 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 197 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 198 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 199 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 200 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 201 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 202 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 203 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 204 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 205 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 206 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 207 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 208 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 209 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 210 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 211 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 212 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 213 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 214 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 215 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 216 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 217 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 218 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 219 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 220 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 221 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 222 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 223 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 224 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 225 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 226 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 227 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 228 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 229 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 230 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 231 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 232 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 233 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 234 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 235 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 236 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 237 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 238 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 239 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 240 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 241 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 242 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 243 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 244 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 245 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 246 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 247 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 248 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 249 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 250 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 251 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 252 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 253 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 254 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 255 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 256 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 257 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 258 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 259 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 260 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 261 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 262 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 263 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 264 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 265 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 266 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 267 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 268 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 269 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 270 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 271 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 272 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 273 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 274 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
