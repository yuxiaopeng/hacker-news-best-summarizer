# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-02-25.md)

*最后自动更新时间: 2026-02-25 20:16:13*
## 1. 以色列国防军在2025年大屠杀中近距离射杀加沙援助人员：报告

**原文标题**: IDF killed Gaza aid workers at point blank range in 2025 massacre: Report

**原文链接**: [https://www.dropsitenews.com/p/israeli-soldiers-tel-sultan-gaza-red-crescent-civil-defense-massacre-report-forensic-architecture-earshot](https://www.dropsitenews.com/p/israeli-soldiers-tel-sultan-gaza-red-crescent-civil-defense-massacre-report-forensic-architecture-earshot)

Earshot和Forensic Architecture的一项联合调查报告称，2025年3月23日，在加沙南部的Tel al-Sultan，以色列士兵“近距离射击”杀害了15名巴勒斯坦援助人员。该报告基于目击者证词、音视频分析和卫星图像，重建了一场“大屠杀”：士兵们向清晰标记的应急车辆和工作人员发射了900多发子弹，其中至少八发子弹的射击距离近至一米。

这起事件造成巴勒斯坦红新月会（PRCS）的八名工作人员、巴勒斯坦民防部门的六名工作人员以及一名联合国救援机构工作人员死亡。报告详细描述了士兵如何伏击援助车队，从高处持续射击了两个多小时，随后推进并处决了工作人员。音频分析证实至少有五名枪手同时开火。两名幸存者证实现场有12至30名士兵。

以色列军方最初几次改变其说法，最终进行了一项内部调查，称没有证据支持处决指控，并建议不采取任何刑事行动，称这些指控为“血腥诽谤”。袭击发生后，据报道以色列军队压碎并试图掩埋车辆，并进行了大规模的土方工程，随后在该地区修建了“莫拉格走廊”安全区。几天后，穿着制服的援助人员的尸体在一个乱葬坑中被发现。

---

## 2. 我在帮我家狗凭感觉编游戏。

**原文标题**: I'm helping my dog vibe code games

**原文链接**: [https://www.calebleak.com/posts/dog-game/](https://www.calebleak.com/posts/dog-game/)

作者开发了一套独特的系统，让他9磅重的卡瓦犬Momo能够使用Claude Code AI“氛围编程”视频游戏。这个项目是作者在被裁员后启动的，灵感来源于Momo之前意外打字到他键盘上的一次事件。

该设置包括Momo在蓝牙键盘上打字，键击通过树莓派5路由到一个名为DogKeyboard的Rust应用程序。这个应用程序会过滤特殊按键，并将输入转发给Claude Code。当Momo输入足够字符时，智能宠物喂食器会分发零食，一声提示音则表示Claude已准备好接收更多输入。游戏使用Godot 4.6和C#开发。

一个关键方面是提示工程：Claude Code被指示扮演一个“杰出的人工智能游戏开发者”，负责从一个“古怪的游戏设计师”那里，即使是从无意义的输入中，解读“神秘的谜语”。强大的护栏机制和最低游戏要求清单（例如，声音、玩家角色、控制）显著改善了结果。

为了扩展系统，强大的验证工具至关重要。作者让Claude能够启动游戏、截取屏幕截图，并发送输入序列（例如“向左3秒，开火”），有效地将AI变成了它自己的质量保证测试员。这使得Claude能够识别并修复诸如用户界面损坏或控制无响应等问题。针对Godot场景和着色器的额外linter，加上一个输入动作映射器，进一步完善了这一过程。

Momo的训练大约持续了两周，最初是在键盘上放置高价值零食以建立关联，然后逐渐通过宠物喂食器自动奖励打字行为。该项目展示了惊人的良好结果，随着工具和Claude能力的演进，游戏质量也随之提高。一个关键发现是在新游戏开始前清除Claude持久化的`MEMORY.md`文件，以防止它强制执行特定的“标志性风格”。Momo创造了各种可玩的游戏，从节奏挑战到解谜游戏和放牧模拟。

---

## 3. 美国人破坏 Flock 监控摄像头

**原文标题**: Americans are destroying Flock surveillance cameras

**原文链接**: [https://techcrunch.com/2026/02/23/americans-are-destroying-flock-surveillance-cameras/](https://techcrunch.com/2026/02/23/americans-are-destroying-flock-surveillance-cameras/)

美国人正在全国范围内日益拆除和破坏Flock监控摄像头，原因是公众对这些车牌识别器协助美国移民局（ICE）进行驱逐出境感到愤怒，以及对隐私的担忧。Flock是一家总部位于亚特兰大的初创公司，生产这些通过拍摄车牌来跟踪车辆移动的摄像头。

尽管Flock声称不直接与ICE共享数据，但据报道，当地警察部门允许联邦当局访问他们的Flock摄像头和数据库。这种间接访问被视为助长了特朗普政府的移民打击行动。

布莱恩·默钱特报告了多起破坏事件，其中包括加利福尼亚州拉梅萨的摄像头被损坏，此事发生在该市议会不顾公众反对投票决定继续部署这些摄像头之后。类似的事件也发生在加利福尼亚州、康涅狄格州、伊利诺伊州和弗吉尼亚州等多个州。在俄勒冈州，六个摄像头被切断并喷漆，并留下了表达强烈反监控情绪的纸条。

根据DeFlock（一个绘制这些设备地图的项目）的数据，美国各地有近8万个摄像头。为了回应争议，数十个城市拒绝了Flock的摄像头，一些警察部门也阻止了联邦当局访问其资源。Flock发言人没有评论该公司是否追踪被毁摄像头的数量。这股破坏浪潮反映了人们对被视为侵犯隐私和有争议的政府政策工具的监控技术日益增长的抵制。

---

## 4. 丹麦政府机构将弃用微软软件 (2025年)

**原文标题**: Danish government agency to ditch Microsoft software (2025)

**原文链接**: [https://therecord.media/denmark-digital-agency-microsoft-digital-independence](https://therecord.media/denmark-digital-agency-microsoft-digital-independence)

丹麦数字化部将用开源替代品取代微软软件，目标是实现“数字独立”并减少对美国科技公司的依赖。数字化部长卡罗琳·斯塔奇·奥尔森证实，该部一半以上的员工将于下月从Microsoft Office转向LibreOffice，并将在年底前全面过渡到开源软件。

此举受多方面因素驱动，包括避免管理过时Windows 10系统的开销、成本考量、微软的市场主导地位以及美国与丹麦之间过去存在的政治紧张关系。LibreOffice由总部位于柏林的非营利组织The Document Foundation开发，提供免费的开源办公套件。斯塔奇指出，如果此次过渡过于复杂，该部可能会恢复使用微软产品。

这一决定反映了欧洲范围内走向数字主权的更广泛趋势。丹麦最大的两个城市哥本哈根和奥胡斯此前也宣布了类似的计划。此外，德国石勒苏益格-荷尔斯泰因州正在放弃Microsoft Office工具，转用LibreOffice和Open-Xchange，并计划迁移到Linux操作系统，这凸显了整个欧洲大陆对独立、安全和可持续IT工作场所日益增长的推动。

---

## 5. 亚马逊被控在全经济范围大范围哄抬物价。

**原文标题**: Amazon accused of widespread scheme to inflate prices across the economy

**原文链接**: [https://www.thebignewsletter.com/p/amazon-busted-for-widespread-price](https://www.thebignewsletter.com/p/amazon-busted-for-widespread-price)

联邦贸易委员会（FTC）和17个州的检察长已对亚马逊提起一项里程碑式的反垄断诉讼，指控这家电子商务巨头运营一项非法且广泛的计划，以在整个经济中抬高物价并抑制竞争。

该诉讼指控亚马逊使用了两种主要的******竞争策略。首先，它实施了反折扣政策，常被称为“公平定价”政策，如果第三方卖家在竞争对手的在线平台上以更低的价格销售商品，就会对其进行惩罚。通过算法强制执行以及威胁将其从亚马逊关键的“购买按钮”中移除，卖家被迫在其他网站上保持更高的价格，否则就有可能被有效排除在亚马逊市场之外。据称，这种做法消除了价格竞争，迫使消费者在整个互联网上支付更多费用。

其次，该诉讼针对亚马逊的“亚马逊物流”（FBA）服务。FTC声称，亚马逊对这项类似强制性物流服务收取过高费用，有效地迫使卖家使用它，进一步抬高了他们的成本，这些成本最终转嫁给了消费者。诉讼认为，这些做法使亚马逊能够人为地抬高价格，扼杀创新，损害竞争对手的零售商，最终通过使产品比在竞争市场中更昂贵来损害消费者。该诉讼旨在结束亚马逊被指控的******竞争行为并恢复竞争。

---

## 6. OpenAI、美国政府和佩尔索纳打造了一个身份监控系统。

**原文标题**: OpenAI, the US government and Persona built an identity surveillance machine

**原文链接**: [https://vmfunc.re/blog/persona/](https://vmfunc.re/blog/persona/)

一份调查报告声称，OpenAI、美国政府和身份验证服务Persona已合作构建了一台“身份监控机器”。研究人员通过对公共资源的被动侦察发现了这一点，识别出一个自2023年11月起活跃的专用Google Cloud实例（`openai-watchlistdb.withpersona.com`）。这比OpenAI公开宣布其身份验证服务早了18个月。

据报道，这个独立于Persona通用网络的隔离基础设施被用于“观察名单”筛选。在一个政府端点上发现的未经认证的源映射暴露了代码，揭示了人脸识别功能、针对14类“负面媒体”（包括恐怖主义和间谍活动）的筛选，以及向FinCEN提交可疑活动报告（SARs）。Persona的公共API文档证实了其收集广泛的用户数据，包括法定姓名、出生详情、国籍、地址、政府文件信息以及生物识别数据（身份证照片、自拍和视频）。

进一步调查发现了`withpersona-gov.com`，这是一个位于Google Cloud数据中心、专门针对政府的并行部署，并于2025年10月获得了FedRAMP授权状态。其Content-Security-Policy标头显示其连接到OpenAI的API，并与第三方服务集成，用于浏览器指纹识别、文档扫描、错误跟踪、用户分析、实时用户监控和财务数据。一个新子域名`onyx.withpersona-gov.com`于2026年2月出现，作者将其与ICE（美国移民和海关执法局）的AI监控项目联系起来。作者强调，所有发现均来自公共可访问数据，构成受保护的新闻报道和安全研究。

---

## 7. Mac mini 将在休斯顿的一处新设施生产。

**原文标题**: Mac mini will be made at a new facility in Houston

**原文链接**: [https://www.apple.com/newsroom/2026/02/apple-accelerates-us-manufacturing-with-mac-mini-production/](https://www.apple.com/newsroom/2026/02/apple-accelerates-us-manufacturing-with-mac-mini-production/)

Apple announced a significant expansion of its U.S. manufacturing operations, bringing Mac mini production to a new facility in Houston, Texas, for the first time, starting later this year (2026). The Houston site will also expand its advanced AI server manufacturing, which began in 2025 and is currently ahead of schedule, supplying Apple's U.S. data centers.

Complementing these production efforts, Apple will open a 20,000-square-foot Advanced Manufacturing Center in Houston later this year. This center will provide hands-on training in advanced manufacturing techniques to students, supplier employees, and American businesses, fostering skills development and creating thousands of jobs.

CEO Tim Cook emphasized Apple's deep commitment to American manufacturing. This Houston expansion is part of Apple's broader $600 billion U.S. manufacturing program, which has achieved several milestones. These include sourcing over 20 billion U.S.-made chips, GlobalWafers starting bare silicon wafer production in Sherman, Texas, and Amkor breaking ground on a $7 billion semiconductor facility in Arizona with Apple as its first customer. Furthermore, Corning's Kentucky facility is now 100% dedicated to iPhone and Apple Watch cover glass, and Apple plans to significantly increase chip purchases from TSMC's Arizona facility in 2026. The company also launched the Apple Manufacturing Academy in Detroit to support American manufacturers with training in AI and automation.

---

## 8. Anthropic Drops Flagship Safety Pledge

**原文标题**: Anthropic Drops Flagship Safety Pledge

**原文链接**: [https://time.com/7380854/exclusive-anthropic-drops-flagship-safety-pledge/](https://time.com/7380854/exclusive-anthropic-drops-flagship-safety-pledge/)

生成摘要时出错

---

## 9. Never buy a .online domain

**原文标题**: Never buy a .online domain

**原文链接**: [https://www.0xsid.com/blog/online-tld-is-pain](https://www.0xsid.com/blog/online-tld-is-pain)

生成摘要时出错

---

## 10. Pi – A minimal terminal coding harness

**原文标题**: Pi – A minimal terminal coding harness

**原文链接**: [https://pi.dev](https://pi.dev)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 2 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 3 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 4 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 5 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 6 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 7 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 8 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 9 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 10 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 11 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 12 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 13 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 14 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 15 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 16 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 17 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 18 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 19 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 20 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 21 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 22 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 23 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 24 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 25 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 26 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 27 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 28 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 29 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 30 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 31 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 32 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 33 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 34 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 35 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 36 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 37 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 38 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 39 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 40 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 41 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 42 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 43 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 44 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 45 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 46 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 47 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 48 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 49 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 50 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 51 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 52 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 53 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 54 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 55 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 56 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 57 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 58 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 59 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 60 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 61 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 62 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 63 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 64 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 65 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 66 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 67 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 68 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 69 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 70 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 71 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 72 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 73 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 74 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 75 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 76 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 77 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 78 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 79 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 80 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 81 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 82 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 83 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 84 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 85 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 86 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 87 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 88 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 89 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 90 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 91 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 92 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 93 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 94 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 95 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 96 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 97 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 98 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 99 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 100 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 101 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 102 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 103 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 104 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 105 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 106 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 107 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 108 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 109 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 110 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
| 111 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
