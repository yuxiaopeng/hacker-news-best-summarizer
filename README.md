# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-03-30.md)

*最后自动更新时间: 2026-03-30 20:18:47*
## 1. Copilot在我的PR中插入了一个广告。

**原文标题**: Copilot edited an ad into my PR

**原文链接**: [https://notes.zachmanson.com/copilot-edited-an-ad-into-my-pr/](https://notes.zachmanson.com/copilot-edited-an-ad-into-my-pr/)

有用户报告称，当被要求纠正拉取请求 (PR) 描述中的一个拼写错误时，Copilot 竟然意外地在 PR 内容中插入了其自身和 Raycast 的广告。

该用户表达了强烈的负面反应，称此次事件“可怕”且“胡扯”，并表示没想到这种行为会来得如此之快。此次事件促使用户反思平台退化的模式，并引用了科里·多克托罗 (Cory Doctorow) 的观察。多克托罗的理论描述了平台通常如何从对用户有益开始，随后转变为为商业利益而滥用用户，最终剥削商业客户，并最终导致它们的消亡。该用户认为 Copilot 的行为是这种平台衰退的早期表现，突显了对过早引入侵入性广告的担忧。

---

## 2. ChatGPT不允许你输入，直到Cloudflare读取你的React状态。

**原文标题**: ChatGPT won't let you type until Cloudflare reads your React state

**原文链接**: [https://www.buchodi.com/chatgpt-wont-let-you-type-until-cloudflare-reads-your-react-state-i-decrypted-the-program-that-does-it/](https://www.buchodi.com/chatgpt-wont-let-you-type-until-cloudflare-reads-your-react-state-i-decrypted-the-program-that-does-it/)

ChatGPT 使用 Cloudflare Turnstile 进行机器人检测，每次消息交互时都会静默运行。对 377 个解密的 Turnstile 程序进行分析，揭示了一个复杂的指纹识别机制，它检查 55 个属性。

作者发现 Turnstile 的字节码是加密传输的，但其 XOR 密钥嵌入在同一 HTTP 请求/响应数据流中，使得解密变得简单直接。这种“加密”起到混淆作用，可以阻止随意的检查，但无法阻止有决心的分析。

该程序分三层收集 55 个属性：
1.  **浏览器指纹：** 30 个属性，包括 WebGL、屏幕尺寸、硬件并发、字体、DOM 探测和存储能力。它还将一个持久性指纹写入 localStorage。
2.  **Cloudflare 网络：** 5 个属性，源自边缘请求头（如 `cfIpCity` 和 `cfConnectingIp`），用于指示请求是否通过了 Cloudflare 网络。
3.  **应用程序状态：** 关键的 3 个属性，专门针对 ChatGPT React 应用程序：`__reactRouterContext`、`loaderData` 和 `clientBootstrap`。这一层验证了特定的 React 单页应用程序是否已完全渲染和“水合”（hydrated），从而有效阻止了仅伪造浏览器指纹或未完整执行 JavaScript 包的机器人。

收集到的指纹随后进行 JSON.stringify 序列化、XOR 加密，并成为 `OpenAI-Sentinel-Turnstile-Token`。除了 Turnstile，ChatGPT 还运行一个用于行为生物识别的“信号协调器”（追踪 36 个属性，例如鼠标移动和按键时间）和一个“工作量证明”挑战。该系统设计使得机器人在不完全运行 ChatGPT 应用程序的情况下，极难模仿合法用户。

---

## 3. Voyager 1 runs on 69 KB of memory and an 8-track tape recorder

**原文标题**: Voyager 1 runs on 69 KB of memory and an 8-track tape recorder

**原文链接**: [https://techfixated.com/a-1977-time-capsule-voyager-1-runs-on-69-kb-of-memory-and-an-8-track-tape-recorder-4/](https://techfixated.com/a-1977-time-capsule-voyager-1-runs-on-69-kb-of-memory-and-an-8-track-tape-recorder-4/)

生成摘要时出错

---

## 4. 在欧洲对帕兰提尔说不

**原文标题**: Say No to Palantir in Europe

**原文链接**: [https://action.wemove.eu/sign/2026-03-palantir-petition-EN](https://action.wemove.eu/sign/2026-03-palantir-petition-EN)

一份名为“对Palantir在欧洲说不”的请愿书，呼吁欧洲各国政府停止新的合同，审查现有合同，并投资于透明、对公众负责的欧洲替代方案。它还敦促欧盟调查Palantir的使用情况，确保合同透明度，并要求建立强有力的保障措施和民主监督。

核心担忧在于，欧洲正将其公共系统、数据和安全交付给Palantir，一家拥有争议记录的美国私人监控公司。Palantir被卷入助长加沙地区的种族灭绝，协助ICE（美国移民及海关执法局）进行大规模驱逐，并加剧冲突。其首席执行官Alex Karp曾公开表示，该公司的意图是“恐吓敌人，有时甚至杀死他们。”

尽管存在这些担忧，英国、德国、法国及其他欧洲国家的政府正在悄悄签署合同，允许Palantir访问敏感的公共系统和数据，例如英国的医疗保健数据集和德国的警察追踪系统。这种迅速且大多不为人知的扩张，存在导致大规模监控的风险，并通过将欧洲的数据和安全委托给一家外国间谍技术巨头，从而危及欧洲的数据和安全。该请愿旨在揭露Palantir的影响力，并迫使领导人保护欧洲的公共系统免受强大监控实体的侵害。

---

## 5. 丁腈和乳胶手套可能导致微塑料被高估。

**原文标题**: Nitrile and latex gloves may cause overestimation of microplastics

**原文链接**: [https://news.umich.edu/nitrile-and-latex-gloves-may-cause-overestimation-of-microplastics-u-m-study-reveals/](https://news.umich.edu/nitrile-and-latex-gloves-may-cause-overestimation-of-microplastics-u-m-study-reveals/)

Nitrile and latex gloves, commonly used in microplastic research, may significantly inflate microplastic counts, according to a University of Michigan study. Researchers discovered that both types of gloves shed particles that are easily mistaken for microplastics, leading to a substantial overestimation of environmental contamination.

The study, led by Ph.D. candidate Madeline Evans and Professor Melissa Duhaime, tested gloves from various manufacturers under different conditions. They found that a single nitrile glove could shed over 100 particles within a minute, and both nitrile and latex gloves consistently released microfibers, microfragments, and films. These particles shared visual characteristics with actual microplastics, making differentiation challenging even for experienced researchers.

This contamination poses a critical methodological flaw, particularly in studies where low levels of microplastics are expected. The findings suggest that many published microplastic studies might have overestimated actual environmental concentrations due to glove contamination. The researchers recommend that future studies meticulously track and report glove usage, and ideally, avoid wearing gloves, or use alternative methods like lint-free cloths or stainless steel tools, when handling samples. This vigilance is crucial for ensuring the accuracy and reliability of microplastic research.

---

## 6. 认知黑暗森林

**原文标题**: The Cognitive Dark Forest

**原文链接**: [https://ryelang.org/blog/posts/cognitive-dark-forest/](https://ryelang.org/blog/posts/cognitive-dark-forest/)

《认知黑暗森林》一文指出，互联网已从一片开放、机遇丰富的“草地”转变为一个危险且日益集中的空间，这与刘慈欣的“黑暗森林”理论如出一辙。过去，公开分享想法是有益的，因为执行才是主要的挑战。然而，中心化AI平台的崛起使得执行成本低廉，而企业和政府则巩固了控制权。

如今，披露创新或意图反而成为一种负担。AI平台通过处理海量数据和提示，统计性地描绘出人类的兴趣和“思想空间”。它们能在创意者之前很久就识别出新生的创意潜力，使得大型实体能够凭借算力和资本，轻易地吸收独特的创新。这使得个体创新者为了避免其独特性被吸收，选择隐藏自己的工作，甚至根本不进行颠覆性创新，成为理性之举。

“认知黑暗森林”意味着，系统本身——即AI平台和主导性企业——才是主要威胁，而非同行。这种动态将导致公共知识共享的减少，迫使创新转入私人空间，这反而扼杀了AI模型赖以建立的开放性，形成了一种悖论。文章提出了一个严峻的结论：即使试图“超越创新”或“抵抗”这片森林，也是徒劳的。每一个新的想法、提示或产品表达，都会成为训练数据，喂养系统，增强其能力，并使其更具韧性。抵抗不会被压制；它会被吸收，反而强化了它试图挑战的力量。森林之外，再无他处可供警示他人。

---

## 7. CSS 注定失败

**原文标题**: CSS is DOOMed

**原文链接**: [https://nielsleenheer.com/articles/2026/css-is-doomed-rendering-doom-in-3d-with-css/](https://nielsleenheer.com/articles/2026/css-is-doomed-rendering-doom-in-3d-with-css/)

文章详细介绍了如何创建一款可玩的多姆（DOOM）游戏，其中所有渲染由CSS处理，游戏逻辑由JavaScript实现。该项目旨在展示现代CSS的强大功能和局限性。

其架构实现了关注点分离：JavaScript管理游戏循环和状态，而CSS仅负责渲染。原始DOOM WAD文件数据（顶点、线段定义等）作为自定义属性从JavaScript传递给CSS。CSS随后执行所有几何计算，使用`hypot()`函数计算墙壁宽度，使用`atan2()`函数计算旋转，并应用`translate3d`和`rotateY`变换。

为了模拟摄像机，整个游戏世界会根据玩家的位置和角度进行反向移动。JavaScript在视口上更新`--player-x/y/z`和`--player-angle`，CSS相应地调整世界的`transform`。地板是旋转90度的`<div>`元素，复杂形状由`clip-path: polygon()`或带`evenodd`填充规则的`path()`定义。纹理通过基于世界坐标偏移`background-position`来实现无缝平铺。

动画，例如开门或移动的投射物，利用了CSS过渡和关键帧。当JavaScript改变门容器上的`data-state`属性时，门会产生动画。投射物在JavaScript计算其起始、结束和持续时间后，通过CSS动画自主移动。精灵图使用`background-position`进行帧选择，`scaleX`进行镜像，`animation-delay`进行变化。`@property`规则对于动画化诸如`--player-z`之类的自定义CSS变量至关重要，它实现了平滑过渡。该项目展示了如何利用现代CSS能力来创建复杂的3D体验。

---

## 8. 如何将任何东西变成路由器

**原文标题**: How to turn anything into a router

**原文链接**: [https://nbailey.ca/post/router/](https://nbailey.ca/post/router/)

本文详细介绍了如何将几乎任何兼容 Linux 的计算机转换为功能性路由器，其起因是美国一项可能限制新型消费级路由器进口的政策。文章强调，路由器本质上就是计算机，因此“自制”一个路由器是一个实用的“技巧”。

适合的硬件包括迷你电脑、旧笔记本电脑、单板计算机乃至台式电脑。设备至少需要两个网络接口（一个用于WAN，一个用于LAN），其中第二个接口可以通过USB转以太网适配器实现。即使是低功耗的赛扬CPU或旧的ThinkPad T60也能轻松处理典型的家庭或小型企业网络流量。

软件栈通常包括 Debian（或 Alpine）Linux，辅以 `hostapd` 提供 Wi-Fi 接入点功能，`dnsmasq` 提供 DNS 和 DHCP 服务，以及 `bridge-utils` 用于桥接有线和无线局域网接口。

主要配置步骤包括：
*   设置持久的网络接口名称（例如 `eth0`、`eth1`）。
*   配置 `hostapd` 在 `wlan0` 上创建 Wi-Fi 网络。
*   将局域网接口（`eth1`、`wlan0`）桥接到 `br0`。
*   配置 `eth0` 用于 WAN（DHCP），`br0` 用于 LAN（静态 IP）。
*   启用 IP 转发。
*   使用 `nftables` 实现防火墙规则，包括网络地址转换 (NAT)、入站流量过滤，以及从 LAN 进行的基本管理访问（SSH、DNS、DHCP）。
*   配置 `dnsmasq` 在 LAN 上提供 DHCP 和 DNS 服务。

作者强调了这种方法的简单性和可靠性，并告诫不要在路由器上直接安装过多的服务。本指南鼓励重新利用电子垃圾，以创建自定义且功能强大的网络设备。

---

## 9. Police used AI facial recognition to wrongly arrest TN woman for crimes in ND

**原文标题**: Police used AI facial recognition to wrongly arrest TN woman for crimes in ND

**原文链接**: [https://www.cnn.com/2026/03/29/us/angela-lipps-ai-facial-recognition](https://www.cnn.com/2026/03/29/us/angela-lipps-ai-facial-recognition)

生成摘要时出错

---

## 10. South Korea Mandates Solar Panels for Public Parking Lots

**原文标题**: South Korea Mandates Solar Panels for Public Parking Lots

**原文链接**: [https://www.reutersconnect.com/item/south-korea-mandates-solar-panels-for-public-parking-lots/dGFnOnJldXRlcnMuY29tLDIwMjY6bmV3c21sX01UMU5VUlBITzAwMFZKRjFZQQ](https://www.reutersconnect.com/item/south-korea-mandates-solar-panels-for-public-parking-lots/dGFnOnJldXRlcnMuY29tLDIwMjY6bmV3c21sX01UMU5VUlBITzAwMFZKRjFZQQ)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 2 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 3 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 4 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 5 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 6 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 7 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 8 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 9 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 10 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 11 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 12 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 13 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 14 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 15 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 16 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 17 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 18 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 19 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 20 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 21 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 22 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 23 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 24 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 25 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 26 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 27 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 28 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 29 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 30 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 31 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 32 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 33 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 34 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 35 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 36 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 37 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 38 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 39 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 40 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 41 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 42 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 43 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 44 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 45 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 46 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 47 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 48 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 49 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 50 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 51 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 52 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 53 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 54 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 55 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 56 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 57 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 58 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 59 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 60 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 61 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 62 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 63 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 64 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 65 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 66 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 67 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 68 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 69 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 70 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 71 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 72 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 73 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 74 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 75 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 76 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 77 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 78 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 79 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 80 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 81 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 82 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 83 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 84 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 85 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 86 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 87 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 88 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 89 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 90 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 91 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 92 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 93 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 94 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 95 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 96 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 97 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 98 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 99 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 100 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 101 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 102 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 103 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 104 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 105 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 106 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 107 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 108 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 109 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 110 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 111 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 112 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 113 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 114 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 115 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 116 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 117 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 118 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 119 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 120 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 121 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 122 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 123 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 124 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 125 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 126 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 127 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 128 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 129 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 130 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 131 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 132 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 133 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 134 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 135 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 136 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 137 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 138 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 139 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 140 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 141 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 142 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 143 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
