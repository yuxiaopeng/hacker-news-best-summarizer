# Hacker News 热门文章摘要 (2026-09-09)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

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

## 11. We accidentally built a synthetic cell factory

**原文标题**: We accidentally built a synthetic cell factory

**原文链接**: [https://bnext.bio/post/we-accidentally-built-a-synthetic-cell-factory](https://bnext.bio/post/we-accidentally-built-a-synthetic-cell-factory)

生成摘要时出错

---

## 12. OUI-1: world's first model for Generative UI

**原文标题**: OUI-1: world's first model for Generative UI

**原文链接**: [https://www.openui.com/blog/oui-1](https://www.openui.com/blog/oui-1)

生成摘要时出错

---

## 13. I Rewrote My Back End in Go in 72 Hours and Cut My AWS Bill by 94%

**原文标题**: I Rewrote My Back End in Go in 72 Hours and Cut My AWS Bill by 94%

**原文链接**: [https://www.bajura.online/2026/09/i-rewrote-my-backend-in-go-in-72-hours.html](https://www.bajura.online/2026/09/i-rewrote-my-backend-in-go-in-72-hours.html)

生成摘要时出错

---

## 14. Apple Watch Ultra 4

**原文标题**: Apple Watch Ultra 4

**原文链接**: [https://www.apple.com/apple-watch-ultra-4/](https://www.apple.com/apple-watch-ultra-4/)

生成摘要时出错

---

## 15. Defining AI Psychosis. Part 2: "Prolific AI Psychosis"

**原文标题**: Defining AI Psychosis. Part 2: "Prolific AI Psychosis"

**原文链接**: [https://jeffs.blog/p/defining-ai-psychosis-part-2-prolific](https://jeffs.blog/p/defining-ai-psychosis-part-2-prolific)

生成摘要时出错

---

## 16. I haven't lost a customer service fight in seven months

**原文标题**: I haven't lost a customer service fight in seven months

**原文链接**: [https://www.sudomoin.com/p/consumer-claims](https://www.sudomoin.com/p/consumer-claims)

生成摘要时出错

---

## 17. Microsoft/TracerAI withdraws copyright takedown against Luanti

**原文标题**: Microsoft/TracerAI withdraws copyright takedown against Luanti

**原文链接**: [https://blog.luanti.org/2026/09/08/dmca-rescinded/](https://blog.luanti.org/2026/09/08/dmca-rescinded/)

生成摘要时出错

---

## 18. Canada's counter-tariffs take effect on various US goods

**原文标题**: Canada's counter-tariffs take effect on various US goods

**原文链接**: [https://www.france24.com/en/live-news/20260908-canada-s-counter-tariffs-take-effect-on-various-us-goods](https://www.france24.com/en/live-news/20260908-canada-s-counter-tariffs-take-effect-on-various-us-goods)

Canada's counter-tariffs on various US goods officially took effect, responding to the US decision to reinstate tariffs on Canadian aluminum. This move, announced by Deputy Prime Minister Chrystia Freeland, applies reciprocal tariffs on US aluminum products, including certain sheets and coils, and extends to other items like washing machines and specific sporting equipment.

The tariffs are valued at $2.7 billion (CAD), matching the amount of US tariffs on Canadian aluminum. Freeland emphasized that these measures are proportionate, fully reciprocal, and designed to avoid escalating the trade dispute while making it clear Canada will defend its industry. She also reiterated that Canada is prepared to adjust the tariffs if the US withdraws its duties on Canadian aluminum. The initial US tariffs on Canadian aluminum had been imposed and then lifted in 2018 during fraught negotiations for the USMCA trade agreement, only to be reimposed by President Donald Trump's administration, citing national security concerns.

---

## 19. DOJ Blocked ICE Agent Shooting Charge over Federal Prosecutor's Objections

**原文标题**: DOJ Blocked ICE Agent Shooting Charge over Federal Prosecutor's Objections

**原文链接**: [https://www.propublica.org/article/doj-blocks-charges-ice-agent-minneapolis-julio-cesar-sosa-celis](https://www.propublica.org/article/doj-blocks-charges-ice-agent-minneapolis-julio-cesar-sosa-celis)

生成摘要时出错

---

## 20. Playing whack-a-mole is losing

**原文标题**: Playing whack-a-mole is losing

**原文链接**: [https://dadrian.io/blog/posts/whack-a-mole-is-losing/](https://dadrian.io/blog/posts/whack-a-mole-is-losing/)

生成摘要时出错

---

## 21. The far right's win in Germany is sending a chill through Europe's establishment

**原文标题**: The far right's win in Germany is sending a chill through Europe's establishment

**原文链接**: [https://www.cnn.com/2026/09/08/europe/germany-far-right-afd-election-europe-intl](https://www.cnn.com/2026/09/08/europe/germany-far-right-afd-election-europe-intl)

生成摘要时出错

---

## 22. So you want to use OpenRouter?

**原文标题**: So you want to use OpenRouter?

**原文链接**: [https://mmoustafa.com/blog/so-you-want-to-use-openrouter/](https://mmoustafa.com/blog/so-you-want-to-use-openrouter/)

生成摘要时出错

---

## 23. GrapheneOS on AI Usage

**原文标题**: GrapheneOS on AI Usage

**原文链接**: [https://grapheneos.social/@GrapheneOS/117236529351603001](https://grapheneos.social/@GrapheneOS/117236529351603001)

生成摘要时出错

---

## 24. My business partner sent a 5K vibe-coded PR that he didn't even test

**原文标题**: My business partner sent a 5K vibe-coded PR that he didn't even test

**原文链接**: [https://ycj.bearblog.dev/ai-again/](https://ycj.bearblog.dev/ai-again/)

生成摘要时出错

---

## 25. I resigned from Anthropic today (Jacob Coxon)

**原文标题**: I resigned from Anthropic today (Jacob Coxon)

**原文链接**: [https://xcancel.com/hilbertspaess/status/2097476196791709843?s=20](https://xcancel.com/hilbertspaess/status/2097476196791709843?s=20)

生成摘要时出错

---

## 26. Flock worker calls police on investigator filming public camera installation

**原文标题**: Flock worker calls police on investigator filming public camera installation

**原文链接**: [https://www.atlantanewsfirst.com/2026/09/08/flock-worker-calls-police-anf-chief-investigator-filming-public-camera-installation/](https://www.atlantanewsfirst.com/2026/09/08/flock-worker-calls-police-anf-chief-investigator-filming-public-camera-installation/)

生成摘要时出错

---

## 27. How Climate Resilient Are the Largest Cities?

**原文标题**: How Climate Resilient Are the Largest Cities?

**原文链接**: [https://alphageo.ai/how-climate-resilient-are-the-worlds-largest-cities/](https://alphageo.ai/how-climate-resilient-are-the-worlds-largest-cities/)

生成摘要时出错

---

