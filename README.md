# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-08-31.md)

*最后自动更新时间: 2026-08-31 23:33:27*
## 1. 我只是斟酌用词。

**原文标题**: “I just chose words carefully”

**原文链接**: [https://unsung.aresluna.org/i-just-chose-words-carefully/](https://unsung.aresluna.org/i-just-chose-words-carefully/)

本文讨论了等宽字体排版的固有难度，尤其是在居中和两端对齐方面。它解释说，由于缺乏半角空格，居中排版很棘手；而两端对齐则会导致难看、过大且不均匀的空格。连字符，在其他语境中常见的解决方案，在等宽字体中也显得问题重重，它会过度吸引对连字符的注意力，并破坏复制粘贴功能，因此在文本文件中很少使用。

文章随后提出了一种卓越的替代方案：精心重写文本，选择恰好填满每行长度的词语，从而避免任何双空格并实现完美的右对齐。这项惊人的壮举由“rs1n”在1990年代末为他那17,000字的《超级银河战士》攻略指南所完成，其中每一行都完美地以一个字母结尾，没有任何双空格。在一次常见问题解答中，rs1n证实他没有使用任何特殊程序，仅仅是一个ASCII编辑器和细致的词语选择。

作者将此作为一个引人入胜的奇闻轶事分享，并将这种极致的专注与开发者或设计师在密集界面中，将UI字符串或工具提示精心调整以适应特定宽度限制的亲身体验进行类比。

---

## 2. 加州议员一致通过豁免Linux免受年龄验证法约束。

**原文标题**: California lawmakers unanimously pass Linux exemption from age-verification law

**原文链接**: [https://www.tomshardware.com/software/linux/california-lawmakers-unanimously-pass-linux-exemption-from-age-verification-law-software-distributed-under-the-gpl-mit-bsd-and-apache-licenses-are-exempt](https://www.tomshardware.com/software/linux/california-lawmakers-unanimously-pass-linux-exemption-from-age-verification-law-software-distributed-under-the-gpl-mit-bsd-and-apache-licenses-are-exempt)

加州立法者一致通过了AB 1856法案，为开源操作系统设立了豁免，使其免受该州定于2027年1月1日生效的《数字年龄保障法案》的约束。原始法案曾要求操作系统提供商在账户设置期间进行年龄验证。

AB 1856重新定义了“操作系统提供商”，将根据GPL、MIT、BSD和Apache等开源许可证分发软件的实体排除在外。这一关键性修改使Debian、Fedora、Ubuntu、Arch、BSD家族和GrapheneOS等流行的Linux发行版免除了年龄验证的要求。

进一步的修订澄清，未通过受监管的应用商店作为独立应用程序提供的软件组件被排除在外，这解决了软件包管理器的问题。仅在宿主应用程序（如浏览器扩展）中运行的扩展商店也获得了豁免。

该法案还纠正了原始法案中存在问题的措辞，删除了将所有加州居民错误地归类为儿童的“用户”定义。现在，除非法律要求，否则它禁止向操作系统提供商或应用商店请求年龄信号，从而防止滥用年龄API。此外，平台和开发者获得“善意避风港”，免除因错误的年龄信号而承担的责任。

尽管Windows、macOS、iOS和Android仍然完全在法案范围内，但这一豁免解决了开源社区近一年的不确定性。众议员Buffy Wicks在收到Linux开发者和电子前沿基金会的批评后提出了这项修正案。该法案目前正等待州长加文·纽森的签署。

---

## 3. 奥马奇：任何用户进程均可提权至Root

**原文标题**: Omarchy: Any User Process Can Escalate to Root

**原文链接**: [https://0xcc.io/posts/omarchy-root-creds/](https://0xcc.io/posts/omarchy-root-creds/)

Omarchy 4.0.1之前的版本在其默认Docker配置中存在一个严重的安全漏洞。操作系统自动将默认用户添加到Linux的`docker`组，这实际上授予了root级别的权限。这是因为`docker`组成员可以直接与root用户拥有的Docker守护进程通信。

任何可以访问Docker套接字的进程都可以命令守护进程以root身份启动容器、挂载主机文件系统的任意部分，并以root权限执行代码。这意味着在用户桌面会话中运行的几乎所有应用程序——包括网络浏览器、IDE和开发工具——都可以在没有密码或权限提示的情况下升级为root权限，从而将用户级别的入侵转化为对整个机器的完全入侵。

该漏洞是一个默认“选择退出”的配置，意味着在用户未明确同意或未获得清晰解释的情况下，系统为其做出了安全权衡。此外，Omarchy的文档错误地建议使用“非root”配置，暗示了一种无root设置，但这是不准确的。

鉴于此问题已得到修复，我们敦促Omarchy用户立即更新到4.0.1版本。文章强调了在以开发者为中心的发行版中，健壮的安全默认设置至关重要，因为开发者是高价值目标。它还推荐Podman作为Docker更安全的无守护进程替代方案，用于运行容器而无需root权限。

---

## 4. OpenShot 4.0 – 开源视频编辑器

**原文标题**: OpenShot 4.0 – Open-source video editor

**原文链接**: [https://www.openshot.org/blog/2026/08/30/openshot-40-record-edit-color-like-never-before/](https://www.openshot.org/blog/2026/08/30/openshot-40-record-edit-color-like-never-before/)

OpenShot 4.0 为这款开源视频编辑器带来了重大的创作工作流程升级。其中一项突出功能是**新的颜色视图**，提供全面的色彩校正和调色功能，包括色轮、曲线、LUTs 以及专业的视频示波器（亮度波形、直方图、RGB分量显示、矢量示波器），所有这些都集成到新的、可关键帧的“色彩分级”效果中。

**新的录制视图**允许将屏幕、网络摄像头、麦克风和系统音频直接捕获到项目中，并使每个源文件保持独立，以便进行灵活编辑。OpenShot 4.0 还新增了**10种效果**，包括用于动画图形的“音频可视化”、用于音频响应式色彩的“节拍同步”、“胶片颗粒”、“图像降噪”、“阴影”、“辉光”和“计时器”。

一项重要创新是**本地AI驱动的遮罩**，它使“对象遮罩”效果能够使用免费、可下载的机器学习模型来选择和跟踪主体，这些模型完全在用户计算机上运行，无需云服务或订阅。对象检测功能也得到了改进。

**时间轴**已被重新设计为更简洁、原生的Qt界面，具有更流畅的缩放、更简单的关键帧、可编辑的时间码和改进的片段交互。性能增强包括显著加快模糊和锐化效果，以及时间轴渲染、视频示波器和色彩分级方面的普遍改进。重新组织的菜单和扩展的Qt 6支持进一步增强了可用性和未来的兼容性，使OpenShot 4.0 成为一个更快、更完善、更具创造性的编辑工具。

---

## 5. 欧盟委员会在 ProtectEU 战略中重启推动加密后门

**原文标题**: European Commission Revives Push for Encryption Backdoors in ProtectEU Strategy

**原文链接**: [https://reclaimthenet.org/eu-protecteu-strategy-encryption-backdoor-law-enforcement](https://reclaimthenet.org/eu-protecteu-strategy-encryption-backdoor-law-enforcement)

欧盟委员会的新“ProtectEU”战略正在重新推动强制要求加密后门的努力，将其包装成执法部门的“合法访问”。该战略被宣布为一项多年期的“愿景和工作计划”，其理由是援引了敌对国家、犯罪集团、恐怖分子和日益猖獗的网络犯罪带来的日益增长的威胁。其六个关键领域之一侧重于开发“更有效的执法工具”，直接瞄准端到端加密。

该战略采用委婉的说法，例如制定“合法有效获取数据”的路线图，以及寻求“访问加密数据的技术解决方案”，并提出一个技术路线图来寻找这些解决方案。然而，这些举措无一例外地遭到科技公司和民权倡导者的强烈反对。他们警告说，加密后门从根本上损害了整体安全和基本权利，使其可供所有行为者访问，包括欧盟声称要防范的敌对实体，尽管委员会承诺维护网络安全。

除了加密之外，“ProtectEU”还概述了成员国之间以及与该集团的单一情报分析能力（SIAC）之间加强情报共享的计划。此外，它旨在赋予欧洲刑警组织（EUROPOL）更多行动权力，以进行跨境和大规模调查，旨在将其转变为一个“真正具有行动力的警察机构”，以加强对成员国的支持。

---

## 6. Playa Phone

**原文标题**: Playa Phone

**原文链接**: [https://playaphone.com/](https://playaphone.com/)

"Playa Phone"是火人节（Burning Man）上的一部免费电话亭，具体位于3:30和Ceiba街交叉口，飞天面条怪兽神庙（Temple of the Flying Spaghetti Monster）前。它允许火人节参与者（Burners）拨打免费的5分钟电话，几乎可以打到世界任何地方，与朋友或挚爱通话。

另外，任何人都可以拨打 +1 (775) 557-4848 这个号码呼叫电话亭，可能会有路过的随机参与者接听。拨打者应预料到可能会遇到占线或响铃六声后无人接听的情况，并且可能需要反复拨打。

如果你接到这个号码的来电，这意味着火人节现场的某个人——可能是朋友、挚爱，也可能是陌生人——拨打了你的号码。建议将“Playa Phone”添加为联系人，以防止未来的来电被静音。

该电话亭通过改造后的内部结构运作，从而实现基于互联网的通话，无需付费。更多信息可查阅一篇SFGATE报道和一份Reddit公告。

---

## 7. Lawmakers added $1 to car insurance policies. That money paid for Flock cameras

**原文标题**: Lawmakers added $1 to car insurance policies. That money paid for Flock cameras

**原文链接**: [https://www.texastribune.org/2026/08/28/texas-flock-cameras-auto-insurance-fee-mvcpa-grants/](https://www.texastribune.org/2026/08/28/texas-flock-cameras-auto-insurance-fee-mvcpa-grants/)

生成摘要时出错

---

## 8. Bug Blindness

**原文标题**: Bug Blindness

**原文链接**: [https://danluu.com/bug-blind/](https://danluu.com/bug-blind/)

生成摘要时出错

---

## 9. A 12TB Steam “teraleak” spills more than a decade of lost PC gaming history

**原文标题**: A 12TB Steam “teraleak” spills more than a decade of lost PC gaming history

**原文链接**: [https://arstechnica.com/gaming/2026/08/a-12tb-steam-teraleak-spills-more-than-a-decade-of-lost-pc-gaming-history/](https://arstechnica.com/gaming/2026/08/a-12tb-steam-teraleak-spills-more-than-a-decade-of-lost-pc-gaming-history/)

生成摘要时出错

---

## 10. Haiku R1/beta6 has been released

**原文标题**: Haiku R1/beta6 has been released

**原文链接**: [https://www.haiku-os.org/news/2026-08-26_haiku_r1_beta6](https://www.haiku-os.org/news/2026-08-26_haiku_r1_beta6)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-08-31](output/hacker_news_summary_2026-08-31.md) |
| 2 | [2026-08-29](output/hacker_news_summary_2026-08-29.md) |
| 3 | [2026-08-30](output/hacker_news_summary_2026-08-30.md) |
| 4 | [2026-08-21](output/hacker_news_summary_2026-08-21.md) |
| 5 | [2026-08-19](output/hacker_news_summary_2026-08-19.md) |
| 6 | [2026-08-25](output/hacker_news_summary_2026-08-25.md) |
| 7 | [2026-08-20](output/hacker_news_summary_2026-08-20.md) |
| 8 | [2026-08-26](output/hacker_news_summary_2026-08-26.md) |
| 9 | [2026-08-24](output/hacker_news_summary_2026-08-24.md) |
| 10 | [2026-08-28](output/hacker_news_summary_2026-08-28.md) |
| 11 | [2026-08-23](output/hacker_news_summary_2026-08-23.md) |
| 12 | [2026-08-22](output/hacker_news_summary_2026-08-22.md) |
| 13 | [2026-08-18](output/hacker_news_summary_2026-08-18.md) |
| 14 | [2026-08-09](output/hacker_news_summary_2026-08-09.md) |
| 15 | [2026-08-10](output/hacker_news_summary_2026-08-10.md) |
| 16 | [2026-08-15](output/hacker_news_summary_2026-08-15.md) |
| 17 | [2026-08-11](output/hacker_news_summary_2026-08-11.md) |
| 18 | [2026-08-12](output/hacker_news_summary_2026-08-12.md) |
| 19 | [2026-08-13](output/hacker_news_summary_2026-08-13.md) |
| 20 | [2026-08-14](output/hacker_news_summary_2026-08-14.md) |
| 21 | [2026-08-17](output/hacker_news_summary_2026-08-17.md) |
| 22 | [2026-08-16](output/hacker_news_summary_2026-08-16.md) |
| 23 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 24 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 25 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 26 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 27 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 28 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 29 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 30 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 31 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 32 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 33 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 34 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 35 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 36 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 37 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 38 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 39 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 40 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 41 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 42 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 43 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 44 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 45 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 46 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 47 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 48 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 49 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 50 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 51 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 52 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 53 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 54 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 55 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 56 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 57 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 58 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 59 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 60 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 61 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 62 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 63 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 64 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 65 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 66 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 67 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 68 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 69 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 70 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 71 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 72 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 73 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 74 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 75 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 76 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 77 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 78 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 79 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 80 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 81 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 82 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 83 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 84 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 85 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 86 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 87 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 88 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 89 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 90 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 91 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 92 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 93 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 94 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 95 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 96 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 97 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 98 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 99 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 100 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 101 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 102 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 103 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 104 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 105 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 106 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 107 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 108 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 109 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 110 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 111 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 112 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 113 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 114 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 115 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 116 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 117 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 118 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 119 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 120 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 121 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 122 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 123 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 124 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 125 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 126 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 127 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 128 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 129 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 130 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 131 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 132 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 133 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 134 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 135 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 136 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 137 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 138 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 139 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 140 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 141 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 142 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 143 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 144 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 145 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 146 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 147 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 148 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 149 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 150 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 151 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 152 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 153 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 154 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 155 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 156 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 157 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 158 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 159 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 160 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 161 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 162 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 163 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 164 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 165 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 166 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 167 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 168 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 169 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 170 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 171 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 172 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 173 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 174 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 175 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 176 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 177 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 178 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 179 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 180 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 181 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 182 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 183 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 184 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 185 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 186 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 187 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 188 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 189 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 190 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 191 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 192 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 193 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 194 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 195 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 196 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 197 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 198 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 199 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 200 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 201 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 202 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 203 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 204 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 205 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 206 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 207 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 208 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 209 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 210 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 211 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 212 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 213 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 214 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 215 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 216 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 217 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 218 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 219 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 220 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 221 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 222 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 223 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 224 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 225 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 226 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 227 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 228 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 229 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 230 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 231 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 232 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 233 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 234 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 235 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 236 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 237 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 238 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 239 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 240 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 241 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 242 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 243 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 244 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 245 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 246 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 247 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 248 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 249 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 250 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 251 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 252 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 253 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 254 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 255 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 256 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 257 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 258 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 259 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 260 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 261 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 262 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 263 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 264 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 265 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 266 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 267 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 268 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 269 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 270 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 271 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 272 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 273 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 274 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 275 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 276 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 277 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 278 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 279 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 280 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 281 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 282 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 283 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 284 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 285 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 286 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 287 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 288 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 289 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 290 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 291 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 292 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 293 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 294 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 295 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
