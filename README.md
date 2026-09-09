# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-09-09.md)

*最后自动更新时间: 2026-09-09 21:46:20*
## 1. Bevy动画：宏观视图

**原文标题**: Animation in Bevy: The Big Picture

**原文链接**: [https://glocq.com/en/blog/20260827/](https://glocq.com/en/blog/20260827/)

本文旨在阐明 Bevy 中 3D 模型动画制作这一通常复杂的流程，旨在为初学者建立清晰的思维模型。尽管简单的 `model.play_animation()` 很直观，但 Bevy 的方法涉及几个不同的组件。

首先，一个 3D 模型通常是作为一个实体层级结构生成的，而非单个实体。为了控制其动画，Bevy 使用 `AnimationPlayer` 组件，该组件会自动插入到该层级结构中的 *某个* 实体中。

动画本身存储并组合在一个 `AnimationGraph` 中。要引用某个特定的动画，你需要同时拥有一个指向 `AnimationGraph` 的引用（即 `Handle`）以及一个 `NodeIndex`，用于指定它在该图中的位置。

要播放动画，你必须：
1. 获取一个 `AnimationGraph`（例如，使用 `AnimationGraph::from_clip` 从 `.glb` 文件中获取）及其对应的 `NodeIndex`。
2. 生成你的 3D 模型场景。
3. 在已生成的模型层级结构中，**定位拥有** `AnimationPlayer` **组件的实体**（通常需要遍历其后代实体，例如使用 `iter_descendants`）。
4. **将** `AnimationGraphHandle` **作为组件插入到** *持有 `AnimationPlayer` 的同一实体上*。
5. 最后，在 `AnimationPlayer` 实例上调用 `player.play(node_index)`，并可选择添加 `.repeat()`。

这个过程通过一个共享实体将 `AnimationPlayer` 及其 `AnimationGraph` 连接起来，从而使播放器能够找到并执行指定的动画。

---

## 2. LG电视被曝扫描局域网，搜寻第三方手机等设备

**原文标题**: LG TV shown scanning LAN for third-party phones and other devices

**原文链接**: [https://arstechnica.com/gadgets/2026/09/lg-tv-shown-capable-of-tracking-user-activity-even-when-offline/](https://arstechnica.com/gadgets/2026/09/lg-tv-shown-capable-of-tracking-user-activity-even-when-offline/)

YouTube 频道 Gamers Nexus 和 Level1Techs 与安全研究人员合作进行的一项最新调查，揭示了LG电视存在的严重隐私问题。分析显示，LG电视（包括高端OLED型号）会主动扫描本地局域网（LAN），以查找其他设备，如智能手表和手机，即便这些设备与电视无关或未连接到电视。

研究人员使用Wireshark观察到，LG电视会识别网络上其他设备的IP地址、地理位置、附近的Wi-Fi网络详情以及内部IP地址。Gamers Nexus 的主编 Steve Burke 指出，这项“原生功能”发现了“数十个不相关的设备”。LG的广告业务LG Ad Solutions此前曾提及触达“可寻址的辅助设备”。LG回应称，这是“智能电视普遍提供的标准功能”，旨在实现设备连接和智能家居集成等特性。

调查还表明，LG电视即使在未连接网络的情况下，也能录制麦克风音频，并将其以纯文本形式本地存储。LG澄清说，这种“监听”只有在开启了“远场语音”（Far-Field）功能以监测唤醒词时才会发生。如果未检测到唤醒词，音频会在本地处理，并立即删除，不会传输到LG服务器；仅当用户有意激活语音功能时，才会进行收集。

这些发现凸显了智能电视普遍存在的隐私问题，因为许多用户，尤其是在设备看似“关闭”或离线时，并不了解此类追踪。这项审查挑战了LG此前在用户追踪和广告方面少于廉价品牌的声誉，并强调了制造商监控用户活动的更广泛担忧。

---

## 3. “美国湖”明确了一点：我们不能信任美国科技公司

**原文标题**: 'Lake America' makes one thing clear: We can't trust U.S. tech companies

**原文链接**: [https://www.tvo.org/article/analysis-lake-america-makes-one-thing-clear-we-cant-trust-us-tech-companies](https://www.tvo.org/article/analysis-lake-america-makes-one-thing-clear-we-cant-trust-us-tech-companies)

我无法提供题为《“美利坚湖”清楚地表明了一点：我们不能信任美国科技公司》的文章摘要，因为所提供的内容并非文章本身。

所提供的文本，“TVO Today | Current Affairs Journalism, Documentaries and Podcasts 您需要启用JavaScript才能运行此应用程序”，似乎是一个通用的网站信息，表明实际内容无法加载或显示。

仅根据标题来看，这篇文章可能主张不信任美国科技公司，可能会从一个被称为“美利坚湖”的概念或实体中获取证据或批判性视角。然而，如果没有文章的实际文本，无法提取或总结更多细节。

---

## 4. 美国将于9月29日禁止加拿大乳制品、酒类和机动车进口。

**原文标题**: US to ban Canadian dairy, alcohol, motor vehicle imports on September 29

**原文链接**: [https://www.reuters.com/business/us-ban-canadian-dairy-alcohol-motor-vehicle-imports-september-29-2026-09-08/](https://www.reuters.com/business/us-ban-canadian-dairy-alcohol-motor-vehicle-imports-september-29-2026-09-08/)

无法访问文章链接。

---

## 5. Disappointed Optimists

**原文标题**: Disappointed Optimists

**原文链接**: [https://cwodtke.com/disappointed-optimists/](https://cwodtke.com/disappointed-optimists/)

生成摘要时出错

---

## 6. 苹果手表 Ultra 4

**原文标题**: Apple Watch Ultra 4

**原文链接**: [https://www.apple.com/newsroom/2026/09/apple-unveils-apple-watch-ultra-4/](https://www.apple.com/newsroom/2026/09/apple-unveils-apple-watch-ultra-4/)

苹果公司于2026年9月9日发布了Apple Watch Ultra 4，将其定位为终极运动与探险手表，在健康、健身和电池续航方面取得了显著进步。

此次更新的核心是全新的健康感应系统，由S11芯片驱动，提供可穿戴设备中最精准的心率感应，以及更高频率的心率和心率变异性（HRV）测量。这带来了一个全新的“准备度”评分，提供每日评估（0-10分）和可操作的建议（恢复、放慢节奏、准备就绪、全力以赴），以指导用户的活动水平。S11芯片还驱动“音频智能”功能，用于记录关键时刻和声音提醒，而Apple Intelligence则通过个人情境，增强了watchOS 27上的Siri功能。

电池续航大幅提升，日常使用可达50小时，低功耗模式下84小时，连续GPS追踪的“极限户外训练”模式下最长可达45小时。充电速度也更快。Ultra 4现在拥有所有智能手表中最精准的步数追踪功能。

一款重新设计的iPhone健康App将于今年晚些时候推出，引入了带有“健康年龄”指标的“长寿”标签页，一个提供及时健康信息的“洞察”标签页，以及新的运动评估功能。用户还可以通过App直接预约Quest Diagnostics的实验室检测。

Apple Watch Ultra 4提供原色和黑色钛金属版本，现已开放预订，并将于9月18日开始发售。

---

## 7. 开源三维解剖探索器：2,234个可选的BodyParts3D网格

**原文标题**: Open-source 3D anatomy explorer: 2,234 selectable BodyParts3D meshes

**原文链接**: [https://github.com/ashemag/human-atlas](https://github.com/ashemag/human-atlas)

本文介绍了一个开源的“人体图谱”，这是一个使用 React、Three.js 和 shadcn/ui 开发的交互式3D解剖探索器。它允许用户探索 BodyParts3D 4.0 成年男性参考模型，该模型包含2,234个可单独选择的网格、15个人体解剖系统和3,432个命名概念。

主要功能包括环绕旋转、缩放、直接选择结构、切换系统（或使用预设）、所有可见部分的“爆炸图”视图、搜索解剖名称以及隔离选定结构以查看详细信息。该探索器设计有紧凑的控件和详细信息面板，适用于移动设备。

该应用程序可以在本地运行，使用 Node.js 22.13+ 版本，且无需 API 密钥。它对网格缓冲区、布局、搜索和交互处理进行了严格验证。解剖数据采用 CC BY 4.0 许可，是一个成年男性参考模型，为提升浏览器性能已简化至约33 MB（220万个三角形）。它明确是一个教育工具，不用于诊断或手术用途。从技术角度看，几何体被合并成批次，并利用 GPU 纹理高效控制平移、可见性和选择。

应用程序代码根据 MIT 许可证发布，而解剖数据则保持其 CC BY 4.0 许可。欢迎提交问题和拉取请求。

---

## 8. AI有发现问题

**原文标题**: AI Has a Discovery Problem

**原文链接**: [https://mhacevedo.com/posts/the-discovery-problem](https://mhacevedo.com/posts/the-discovery-problem)

文章指出，“发现问题”是人工智能普及的主要瓶颈：用户不知道人工智能能为他们做什么，因为其庞大的功能被隐藏在一个空白文本框后面。用户只有尝试后才能发现可能性，但他们却不知道该尝试什么。

模板和情境建议等部分解决方案提供了一些帮助，提供初始提示或相关想法，但它们效果不佳，因为模板通常缺乏个人相关性，而建议也未能充分展现系统的潜力。

作者引用了艾伦·凯的比喻：大峡谷中的蚂蚁只能看到一线天空，而站在峡谷边缘的人却能看到整个平面。这说明了熟练的人工智能用户（他们能立即发现大量的自动化和创新机会）与普通用户（他们面对空白提示，无法利用现有智能）之间的差距。

核心论点是，发现人工智能潜力的负担过于沉重地落在了用户身上，而非系统。文章总结道，高级人工智能界面应主动、渐进、情境化地展现其能力，并以直接匹配用户实际工作的方式，有效地“向你展示可能性之空”。

---

## 9. One woman's Tesla was remotely controlled by an abusive ex-partner

**原文标题**: One woman's Tesla was remotely controlled by an abusive ex-partner

**原文链接**: [https://www.theguardian.com/australia-news/2026/sep/09/how-one-womans-tesla-was-remotely-controlled-and-harass-by-her-abusive-ex-partner-ntwnfb](https://www.theguardian.com/australia-news/2026/sep/09/how-one-womans-tesla-was-remotely-controlled-and-harass-by-her-abusive-ex-partner-ntwnfb)

A woman, identified as Stacey (name changed), endured years of domestic abuse from her ex-partner, Enrico Pucci, who remotely controlled her Tesla car to harass and endanger her. Pucci was recently convicted of 30 domestic violence-related charges, including using the Tesla app to stalk and harass Stacey, and sentenced to two years and three months in prison.

Stacey had registered the Tesla in Pucci's name for "assistance" with its technology. After their relationship ended, Pucci exploited this access. Between November 6 and 12, 2025, he remotely activated "Valet Mode" to limit the car's speed to 40km/h, creating significant safety issues. He also manipulated the car's temperature, locks, and curfew settings, and attempted to disconnect it from charging multiple times, taunting Stacey with phrases like "I am in your car." Stacey had no control over her vehicle and feared for her safety.

This tech-enabled harassment was part of a four-year pattern of coercive control. Previous abuses included common assault where he threatened her son and left her stranded, and a strangulation incident that caused her to black out. Pucci's history also includes exploiting vulnerable workers through his cleaning firm and corporate disqualification by ASIC for failed companies. He is appealing his sentence.

---

## 10. The Education of a Doomer

**原文标题**: The Education of a Doomer

**原文链接**: [https://borretti.me/article/the-education-of-a-doomer](https://borretti.me/article/the-education-of-a-doomer)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-09-09](output/hacker_news_summary_2026-09-09.md) |
| 2 | [2026-09-08](output/hacker_news_summary_2026-09-08.md) |
| 3 | [2026-09-04](output/hacker_news_summary_2026-09-04.md) |
| 4 | [2026-09-07](output/hacker_news_summary_2026-09-07.md) |
| 5 | [2026-09-03](output/hacker_news_summary_2026-09-03.md) |
| 6 | [2026-09-02](output/hacker_news_summary_2026-09-02.md) |
| 7 | [2026-09-05](output/hacker_news_summary_2026-09-05.md) |
| 8 | [2026-09-06](output/hacker_news_summary_2026-09-06.md) |
| 9 | [2026-08-25](output/hacker_news_summary_2026-08-25.md) |
| 10 | [2026-08-26](output/hacker_news_summary_2026-08-26.md) |
| 11 | [2026-09-01](output/hacker_news_summary_2026-09-01.md) |
| 12 | [2026-08-31](output/hacker_news_summary_2026-08-31.md) |
| 13 | [2026-08-28](output/hacker_news_summary_2026-08-28.md) |
| 14 | [2026-08-30](output/hacker_news_summary_2026-08-30.md) |
| 15 | [2026-08-29](output/hacker_news_summary_2026-08-29.md) |
| 16 | [2026-08-20](output/hacker_news_summary_2026-08-20.md) |
| 17 | [2026-08-18](output/hacker_news_summary_2026-08-18.md) |
| 18 | [2026-08-19](output/hacker_news_summary_2026-08-19.md) |
| 19 | [2026-08-21](output/hacker_news_summary_2026-08-21.md) |
| 20 | [2026-08-17](output/hacker_news_summary_2026-08-17.md) |
| 21 | [2026-08-23](output/hacker_news_summary_2026-08-23.md) |
| 22 | [2026-08-22](output/hacker_news_summary_2026-08-22.md) |
| 23 | [2026-08-24](output/hacker_news_summary_2026-08-24.md) |
| 24 | [2026-08-12](output/hacker_news_summary_2026-08-12.md) |
| 25 | [2026-08-14](output/hacker_news_summary_2026-08-14.md) |
| 26 | [2026-08-10](output/hacker_news_summary_2026-08-10.md) |
| 27 | [2026-08-11](output/hacker_news_summary_2026-08-11.md) |
| 28 | [2026-08-16](output/hacker_news_summary_2026-08-16.md) |
| 29 | [2026-08-09](output/hacker_news_summary_2026-08-09.md) |
| 30 | [2026-08-13](output/hacker_news_summary_2026-08-13.md) |
| 31 | [2026-08-15](output/hacker_news_summary_2026-08-15.md) |
| 32 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 33 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 34 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 35 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 36 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 37 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 38 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 39 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 40 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 41 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 42 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 43 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 44 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 45 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 46 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 47 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 48 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 49 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 50 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 51 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 52 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 53 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 54 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 55 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 56 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 57 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 58 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 59 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 60 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 61 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 62 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 63 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 64 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 65 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 66 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 67 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 68 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 69 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 70 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 71 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 72 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 73 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 74 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 75 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 76 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 77 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 78 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 79 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 80 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 81 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 82 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 83 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 84 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 85 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 86 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 87 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 88 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 89 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 90 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 91 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 92 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 93 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 94 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 95 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 96 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 97 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 98 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 99 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 100 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 101 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 102 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 103 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 104 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 105 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 106 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 107 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 108 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 109 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 110 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 111 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 112 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 113 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 114 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 115 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 116 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 117 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 118 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 119 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 120 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 121 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 122 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 123 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 124 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 125 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 126 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 127 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 128 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 129 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 130 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 131 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 132 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 133 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 134 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 135 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 136 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 137 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 138 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 139 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 140 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 141 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 142 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 143 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 144 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 145 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 146 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 147 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 148 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 149 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 150 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 151 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 152 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 153 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 154 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 155 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 156 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 157 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 158 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 159 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 160 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 161 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 162 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 163 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 164 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 165 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 166 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 167 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 168 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 169 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 170 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 171 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 172 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 173 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 174 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 175 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 176 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 177 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 178 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 179 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 180 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 181 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 182 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 183 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 184 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 185 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 186 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 187 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 188 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 189 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 190 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 191 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 192 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 193 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 194 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 195 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 196 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 197 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 198 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 199 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 200 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 201 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 202 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 203 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 204 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 205 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 206 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 207 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 208 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 209 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 210 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 211 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 212 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 213 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 214 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 215 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 216 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 217 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 218 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 219 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 220 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 221 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 222 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 223 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 224 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 225 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 226 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 227 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 228 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 229 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 230 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 231 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 232 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 233 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 234 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 235 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 236 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 237 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 238 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 239 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 240 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 241 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 242 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 243 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 244 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 245 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 246 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 247 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 248 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 249 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 250 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 251 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 252 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 253 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 254 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 255 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 256 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 257 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 258 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 259 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 260 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 261 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 262 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 263 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 264 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 265 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 266 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 267 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 268 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 269 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 270 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 271 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 272 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 273 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 274 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 275 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 276 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 277 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 278 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 279 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 280 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 281 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 282 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 283 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 284 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 285 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 286 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 287 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 288 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 289 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 290 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 291 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 292 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 293 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 294 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 295 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 296 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 297 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 298 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 299 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 300 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 301 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 302 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 303 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 304 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
