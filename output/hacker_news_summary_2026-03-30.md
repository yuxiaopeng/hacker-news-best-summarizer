# Hacker News 热门文章摘要 (2026-03-30)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

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

## 11. Neovim 0.12.0

**原文标题**: Neovim 0.12.0

**原文链接**: [https://github.com/neovim/neovim/releases/tag/v0.12.0](https://github.com/neovim/neovim/releases/tag/v0.12.0)

生成摘要时出错

---

## 12. Philly courts will ban all smart eyeglasses starting next week

**原文标题**: Philly courts will ban all smart eyeglasses starting next week

**原文链接**: [https://www.inquirer.com/news/philadelphia/smart-glasses-ai-meta-courts-20260326.html](https://www.inquirer.com/news/philadelphia/smart-glasses-ai-meta-courts-20260326.html)

生成摘要时出错

---

## 13. My MacBook keyboard is broken and it's insanely expensive to fix

**原文标题**: My MacBook keyboard is broken and it's insanely expensive to fix

**原文链接**: [https://tobiasberg.net/posts/my-macbook-keyboard-is-broken-and-its-insanely-expensive-to-fix/](https://tobiasberg.net/posts/my-macbook-keyboard-is-broken-and-its-insanely-expensive-to-fix/)

生成摘要时出错

---

## 14. How the AI Bubble Bursts

**原文标题**: How the AI Bubble Bursts

**原文链接**: [https://martinvol.pe/blog/2026/03/30/how-the-ai-bubble-bursts/](https://martinvol.pe/blog/2026/03/30/how-the-ai-bubble-bursts/)

生成摘要时出错

---

## 15. Miasma: A tool to trap AI web scrapers in an endless poison pit

**原文标题**: Miasma: A tool to trap AI web scrapers in an endless poison pit

**原文链接**: [https://github.com/austin-weeks/miasma](https://github.com/austin-weeks/miasma)

生成摘要时出错

---

## 16. 1.5M GitHub pull requests have had ads injected into them by Microsoft Copilot

**原文标题**: 1.5M GitHub pull requests have had ads injected into them by Microsoft Copilot

**原文链接**: [https://www.neowin.net/news/microsoft-copilot-is-now-injecting-ads-into-pull-requests-on-github-gitlab/](https://www.neowin.net/news/microsoft-copilot-is-now-injecting-ads-into-pull-requests-on-github-gitlab/)

生成摘要时出错

---

## 17. The curious case of retro demo scene graphics

**原文标题**: The curious case of retro demo scene graphics

**原文链接**: [https://www.datagubbe.se/aipixels/](https://www.datagubbe.se/aipixels/)

生成摘要时出错

---

## 18. C++26 is done: ISO C++ standards meeting Trip Report

**原文标题**: C++26 is done: ISO C++ standards meeting Trip Report

**原文链接**: [https://herbsutter.com/2026/03/29/c26-is-done-trip-report-march-2026-iso-c-standards-meeting-london-croydon-uk/](https://herbsutter.com/2026/03/29/c26-is-done-trip-report-march-2026-iso-c-standards-meeting-london-croydon-uk/)

生成摘要时出错

---

## 19. Full network of clitoral nerves mapped out for first time

**原文标题**: Full network of clitoral nerves mapped out for first time

**原文链接**: [https://www.theguardian.com/society/2026/mar/29/full-network-clitoral-nerves-mapped-out-first-time-women-pelvic-surgery](https://www.theguardian.com/society/2026/mar/29/full-network-clitoral-nerves-mapped-out-first-time-women-pelvic-surgery)

生成摘要时出错

---

## 20. New Apple Silicon M4 and M5 HiDPI Limitation on 4K External Displays

**原文标题**: New Apple Silicon M4 and M5 HiDPI Limitation on 4K External Displays

**原文链接**: [https://smcleod.net/2026/03/new-apple-silicon-m4-m5-hidpi-limitation-on-4k-external-displays/](https://smcleod.net/2026/03/new-apple-silicon-m4-m5-hidpi-limitation-on-4k-external-displays/)

生成摘要时出错

---

## 21. 15 years, one server, 8GB RAM and 500k users – how Webminal refuses to die

**原文标题**: 15 years, one server, 8GB RAM and 500k users – how Webminal refuses to die

**原文链接**: [https://community.webminal.org/t/15-years-one-server-8gb-ram-and-500k-users-how-webminal-refuses-to-die/8803](https://community.webminal.org/t/15-years-one-server-8gb-ram-and-500k-users-how-webminal-refuses-to-die/8803)

生成摘要时出错

---

## 22. Coding agents could make free software matter again

**原文标题**: Coding agents could make free software matter again

**原文链接**: [https://www.gjlondon.com/blog/ai-agents-could-make-free-software-matter-again/](https://www.gjlondon.com/blog/ai-agents-could-make-free-software-matter-again/)

生成摘要时出错

---

## 23. Bird brains (2023)

**原文标题**: Bird brains (2023)

**原文链接**: [https://www.dhanishsemar.com/writing/bird-brains](https://www.dhanishsemar.com/writing/bird-brains)

生成摘要时出错

---

## 24. Claude Code runs Git reset –hard origin/main against project repo every 10 mins

**原文标题**: Claude Code runs Git reset –hard origin/main against project repo every 10 mins

**原文链接**: [https://github.com/anthropics/claude-code/issues/40710](https://github.com/anthropics/claude-code/issues/40710)

生成摘要时出错

---

## 25. I use Excalidraw to manage my diagrams for my blog

**原文标题**: I use Excalidraw to manage my diagrams for my blog

**原文链接**: [https://blog.lysk.tech/excalidraw-frame-export/](https://blog.lysk.tech/excalidraw-frame-export/)

生成摘要时出错

---

## 26. New Washington state law bans noncompete agreements

**原文标题**: New Washington state law bans noncompete agreements

**原文链接**: [https://www.seattletimes.com/business/local-business/new-washington-law-bans-noncompete-agreements/](https://www.seattletimes.com/business/local-business/new-washington-law-bans-noncompete-agreements/)

生成摘要时出错

---

## 27. The bot situation on the internet is worse than you could imagine

**原文标题**: The bot situation on the internet is worse than you could imagine

**原文链接**: [https://gladeart.com/blog/the-bot-situation-on-the-internet-is-actually-worse-than-you-could-imagine-heres-why](https://gladeart.com/blog/the-bot-situation-on-the-internet-is-actually-worse-than-you-could-imagine-heres-why)

生成摘要时出错

---

## 28. Alzheimer's disease mortality among taxi and ambulance drivers (2024)

**原文标题**: Alzheimer's disease mortality among taxi and ambulance drivers (2024)

**原文链接**: [https://www.bmj.com/content/387/bmj-2024-082194](https://www.bmj.com/content/387/bmj-2024-082194)

生成摘要时出错

---

## 29. CodingFont: A game to help you pick a coding font

**原文标题**: CodingFont: A game to help you pick a coding font

**原文链接**: [https://www.codingfont.com/](https://www.codingfont.com/)

生成摘要时出错

---

## 30. Private equity turned vulnerable elderly people into human ATMs

**原文标题**: Private equity turned vulnerable elderly people into human ATMs

**原文链接**: [https://www.theguardian.com/society/2026/mar/28/the-great-care-home-cash-grab-how-private-equity-turned-vulnerable-elderly-people-into-human-atms](https://www.theguardian.com/society/2026/mar/28/the-great-care-home-cash-grab-how-private-equity-turned-vulnerable-elderly-people-into-human-atms)

生成摘要时出错

---

## 31. 72% of the dollar's purchasing power was destroyed in just four episodes

**原文标题**: 72% of the dollar's purchasing power was destroyed in just four episodes

**原文链接**: [https://eco3min.fr/en/us-inflation-is-not-linear/](https://eco3min.fr/en/us-inflation-is-not-linear/)

生成摘要时出错

---

## 32. What if AI doesn't need more RAM but better math?

**原文标题**: What if AI doesn't need more RAM but better math?

**原文链接**: [https://adlrocha.substack.com/p/adlrocha-what-if-ai-doesnt-need-more](https://adlrocha.substack.com/p/adlrocha-what-if-ai-doesnt-need-more)

生成摘要时出错

---

## 33. I am definitely missing the pre-AI writing era

**原文标题**: I am definitely missing the pre-AI writing era

**原文链接**: [https://www.lesswrong.com/posts/BJ4pnropWdnzzgeJc/i-am-definitely-missing-the-pre-ai-writing-era](https://www.lesswrong.com/posts/BJ4pnropWdnzzgeJc/i-am-definitely-missing-the-pre-ai-writing-era)

生成摘要时出错

---

## 34. FTC action against Match and OkCupid for deceiving users, sharing personal data

**原文标题**: FTC action against Match and OkCupid for deceiving users, sharing personal data

**原文链接**: [https://www.ftc.gov/news-events/news/press-releases/2026/03/ftc-takes-action-against-match-okcupid-deceiving-users-sharing-personal-data-third-party](https://www.ftc.gov/news-events/news/press-releases/2026/03/ftc-takes-action-against-match-okcupid-deceiving-users-sharing-personal-data-third-party)

生成摘要时出错

---

## 35. Mathematical methods and human thought in the age of AI

**原文标题**: Mathematical methods and human thought in the age of AI

**原文链接**: [https://arxiv.org/abs/2603.26524](https://arxiv.org/abs/2603.26524)

生成摘要时出错

---

## 36. The road signs that teach travellers about France

**原文标题**: The road signs that teach travellers about France

**原文链接**: [https://www.bbc.com/travel/article/20260327-the-road-signs-that-teach-travellers-about-france](https://www.bbc.com/travel/article/20260327-the-road-signs-that-teach-travellers-about-france)

生成摘要时出错

---

## 37. Android’s new sideload settings will carry over to new devices

**原文标题**: Android’s new sideload settings will carry over to new devices

**原文链接**: [https://www.androidauthority.com/android-sideload-carry-over-3652845/](https://www.androidauthority.com/android-sideload-carry-over-3652845/)

生成摘要时出错

---

## 38. Ghostmoon.app – A Swiss Army Knife for your macOS menu bar

**原文标题**: Ghostmoon.app – A Swiss Army Knife for your macOS menu bar

**原文链接**: [https://www.mgrunwald.com/ghostmoon/](https://www.mgrunwald.com/ghostmoon/)

生成摘要时出错

---

## 39. Midnight train from GA: A view of America from the tracks as airports struggle

**原文标题**: Midnight train from GA: A view of America from the tracks as airports struggle

**原文链接**: [https://apnews.com/article/airports-shutdown-long-lines-train-travel-amtrak-e4d8ea591b3b036142c2bf2dee7dff5a](https://apnews.com/article/airports-shutdown-long-lines-train-travel-amtrak-e4d8ea591b3b036142c2bf2dee7dff5a)

生成摘要时出错

---

## 40. VHDL's Crown Jewel

**原文标题**: VHDL's Crown Jewel

**原文链接**: [https://www.sigasi.com/opinion/jan/vhdls-crown-jewel/](https://www.sigasi.com/opinion/jan/vhdls-crown-jewel/)

生成摘要时出错

---

## 41. Hamilton-Jacobi-Bellman Equation: Reinforcement Learning and Diffusion Models

**原文标题**: Hamilton-Jacobi-Bellman Equation: Reinforcement Learning and Diffusion Models

**原文链接**: [https://dani2442.github.io/posts/continuous-rl/](https://dani2442.github.io/posts/continuous-rl/)

生成摘要时出错

---

## 42. The "Vibe Coding" Wall of Shame

**原文标题**: The "Vibe Coding" Wall of Shame

**原文链接**: [https://crackr.dev/vibe-coding-failures](https://crackr.dev/vibe-coding-failures)

生成摘要时出错

---

## 43. A laser-based process that enables adhesive-free paper packaging

**原文标题**: A laser-based process that enables adhesive-free paper packaging

**原文链接**: [https://www.fraunhofer.de/en/press/research-news/2026/march-2026/sealing-paper-packaging-without-adhesives.html](https://www.fraunhofer.de/en/press/research-news/2026/march-2026/sealing-paper-packaging-without-adhesives.html)

生成摘要时出错

---

## 44. Netscape News Feed Straight Out of the Late 00s

**原文标题**: Netscape News Feed Straight Out of the Late 00s

**原文链接**: [https://isp.netscape.com/](https://isp.netscape.com/)

生成摘要时出错

---

## 45. Take better notes, by hand

**原文标题**: Take better notes, by hand

**原文链接**: [https://brianschrader.com/archive/take-better-notes-by-hand/](https://brianschrader.com/archive/take-better-notes-by-hand/)

生成摘要时出错

---

## 46. TSA lines are so out of control that travelers are hiring line-sitters

**原文标题**: TSA lines are so out of control that travelers are hiring line-sitters

**原文链接**: [https://www.washingtonpost.com/travel/2026/03/28/tsa-line-sitters/](https://www.washingtonpost.com/travel/2026/03/28/tsa-line-sitters/)

生成摘要时出错

---

## 47. “CEO said a thing” journalism

**原文标题**: “CEO said a thing” journalism

**原文链接**: [https://karlbode.com/ceo-said-a-thing-journalism/](https://karlbode.com/ceo-said-a-thing-journalism/)

生成摘要时出错

---

## 48. Do your own writing

**原文标题**: Do your own writing

**原文链接**: [https://alexhwoods.com/dont-let-ai-write-for-you/](https://alexhwoods.com/dont-let-ai-write-for-you/)

生成摘要时出错

---

## 49. Solar is winning the energy race

**原文标题**: Solar is winning the energy race

**原文链接**: [https://www.dw.com/en/solar-is-winning-the-energy-race/a-76517556](https://www.dw.com/en/solar-is-winning-the-energy-race/a-76517556)

生成摘要时出错

---

## 50. Show HN: QuickBEAM – run JavaScript as supervised Erlang/OTP processes

**原文标题**: Show HN: QuickBEAM – run JavaScript as supervised Erlang/OTP processes

**原文链接**: [https://github.com/elixir-volt/quickbeam](https://github.com/elixir-volt/quickbeam)

生成摘要时出错

---

## 51. You are falling behind because you haven't fed the insincerity machine

**原文标题**: You are falling behind because you haven't fed the insincerity machine

**原文链接**: [https://christianheilmann.com/2026/03/28/you-are-falling-behind-because-you-havent-fed-the-insincerity-machine-in-the-last-5-minutes/](https://christianheilmann.com/2026/03/28/you-are-falling-behind-because-you-havent-fed-the-insincerity-machine-in-the-last-5-minutes/)

生成摘要时出错

---

## 52. AyaFlow: A high-performance, eBPF-based network traffic analyzer written in Rust

**原文标题**: AyaFlow: A high-performance, eBPF-based network traffic analyzer written in Rust

**原文链接**: [https://github.com/DavidHavoc/ayaFlow](https://github.com/DavidHavoc/ayaFlow)

生成摘要时出错

---

## 53. The rise and fall of IBM's 4 Pi aerospace computers: an illustrated history

**原文标题**: The rise and fall of IBM's 4 Pi aerospace computers: an illustrated history

**原文链接**: [https://www.righto.com/2026/03/ibm-4-pi-computer-history.html](https://www.righto.com/2026/03/ibm-4-pi-computer-history.html)

生成摘要时出错

---

## 54. There is no spoon – A software engineers primer for demystified ML

**原文标题**: There is no spoon – A software engineers primer for demystified ML

**原文链接**: [https://github.com/dreddnafious/thereisnospoon](https://github.com/dreddnafious/thereisnospoon)

生成摘要时出错

---

## 55. More on Version Control

**原文标题**: More on Version Control

**原文链接**: [https://bramcohen.com/p/more-on-version-control](https://bramcohen.com/p/more-on-version-control)

生成摘要时出错

---

## 56. Kyushu Railway Company Train Varieties

**原文标题**: Kyushu Railway Company Train Varieties

**原文链接**: [https://www.jrkyushu.co.jp/english/train/index.html](https://www.jrkyushu.co.jp/english/train/index.html)

生成摘要时出错

---

## 57. Fedware: Government apps that spy harder than the apps they ban

**原文标题**: Fedware: Government apps that spy harder than the apps they ban

**原文链接**: [https://www.sambent.com/the-white-house-app-has-huawei-spyware-and-an-ice-tip-line/](https://www.sambent.com/the-white-house-app-has-huawei-spyware-and-an-ice-tip-line/)

生成摘要时出错

---

## 58. Sky Wins Irish Court Order to Unmask 300 Pirate IPTV Users via Revolut Bank

**原文标题**: Sky Wins Irish Court Order to Unmask 300 Pirate IPTV Users via Revolut Bank

**原文链接**: [https://torrentfreak.com/sky-wins-irish-court-order-to-unmask-300-pirate-iptv-users-via-revolut-bank/](https://torrentfreak.com/sky-wins-irish-court-order-to-unmask-300-pirate-iptv-users-via-revolut-bank/)

生成摘要时出错

---

## 59. Show HN: BreezePDF – Free, in-browser PDF editor

**原文标题**: Show HN: BreezePDF – Free, in-browser PDF editor

**原文链接**: [https://breezepdf.com/?v=3](https://breezepdf.com/?v=3)

生成摘要时出错

---

## 60. Lat.md: Agent Lattice: a knowledge graph for your codebase, written in Markdown

**原文标题**: Lat.md: Agent Lattice: a knowledge graph for your codebase, written in Markdown

**原文链接**: [https://github.com/1st1/lat.md](https://github.com/1st1/lat.md)

生成摘要时出错

---

## 61. Twice this week, I have come across embarassingly bad data

**原文标题**: Twice this week, I have come across embarassingly bad data

**原文链接**: [https://successfulsoftware.net/2026/03/29/stop-publishing-garbage-data-its-embarrassing/](https://successfulsoftware.net/2026/03/29/stop-publishing-garbage-data-its-embarrassing/)

生成摘要时出错

---

## 62. Build123d: A Python CAD programming library

**原文标题**: Build123d: A Python CAD programming library

**原文链接**: [https://github.com/gumyr/build123d](https://github.com/gumyr/build123d)

生成摘要时出错

---

## 63. First Western Digital, now Sony: The tech giant suspends SD card sales

**原文标题**: First Western Digital, now Sony: The tech giant suspends SD card sales

**原文链接**: [https://mashable.com/article/sony-sd-card-sales-suspended-memory-shortage](https://mashable.com/article/sony-sd-card-sales-suspended-memory-shortage)

生成摘要时出错

---

## 64. Show HN: Sheet Ninja – Google Sheets as a CRUD Back End for Vibe Coders

**原文标题**: Show HN: Sheet Ninja – Google Sheets as a CRUD Back End for Vibe Coders

**原文链接**: [https://sheetninja.io](https://sheetninja.io)

生成摘要时出错

---

## 65. OpenYak – An open-source Cowork that runs any model and owns your filesystem

**原文标题**: OpenYak – An open-source Cowork that runs any model and owns your filesystem

**原文链接**: [https://github.com/openyak/desktop](https://github.com/openyak/desktop)

生成摘要时出错

---

## 66. Spain shuts airspace for US planes involved in Iran war

**原文标题**: Spain shuts airspace for US planes involved in Iran war

**原文链接**: [https://english.aawsat.com/world/5256772-spain-shuts-airspace-us-planes-involved-iran-war](https://english.aawsat.com/world/5256772-spain-shuts-airspace-us-planes-involved-iran-war)

生成摘要时出错

---

## 67. The Strait of Hormuz Oil Shock Is Now Heading West

**原文标题**: The Strait of Hormuz Oil Shock Is Now Heading West

**原文链接**: [https://www.bloomberg.com/graphics/2026-iran-war-hormuz-closure-oil-shock](https://www.bloomberg.com/graphics/2026-iran-war-hormuz-closure-oil-shock)

生成摘要时出错

---

## 68. Goldman Sachs now reckons that oil could take out the 2008 record of $147

**原文标题**: Goldman Sachs now reckons that oil could take out the 2008 record of $147

**原文链接**: [https://www.ft.com/content/360ca227-4d2a-41a4-a05f-41baedc0f7d2](https://www.ft.com/content/360ca227-4d2a-41a4-a05f-41baedc0f7d2)

生成摘要时出错

---

## 69. Sylve – Proxmox Alternative by FreeBSD

**原文标题**: Sylve – Proxmox Alternative by FreeBSD

**原文链接**: [https://sylve.io/](https://sylve.io/)

生成摘要时出错

---

## 70. OCR for construction documents does not work, we fixed it

**原文标题**: OCR for construction documents does not work, we fixed it

**原文链接**: [https://www.getanchorgrid.com/developer/docs/endpoints/drawings-doors](https://www.getanchorgrid.com/developer/docs/endpoints/drawings-doors)

生成摘要时出错

---

## 71. Stripe is down

**原文标题**: Stripe is down

**原文链接**: [https://status.stripe.com/](https://status.stripe.com/)

生成摘要时出错

---

## 72. Show HN: Crazierl – An Erlang Operating System

**原文标题**: Show HN: Crazierl – An Erlang Operating System

**原文链接**: [https://crazierl.org/demo/](https://crazierl.org/demo/)

生成摘要时出错

---

## 73. Why mathematicians are boycotting their biggest conference

**原文标题**: Why mathematicians are boycotting their biggest conference

**原文链接**: [https://www.scientificamerican.com/article/why-mathematicians-are-boycotting-their-biggest-conference/](https://www.scientificamerican.com/article/why-mathematicians-are-boycotting-their-biggest-conference/)

生成摘要时出错

---

## 74. Hardware Image Compression

**原文标题**: Hardware Image Compression

**原文链接**: [https://www.ludicon.com/castano/blog/2026/03/hardware-image-compression/](https://www.ludicon.com/castano/blog/2026/03/hardware-image-compression/)

生成摘要时出错

---

## 75. The road to electric in charts and data

**原文标题**: The road to electric in charts and data

**原文链接**: [https://www.rac.co.uk/drive/electric-cars/choosing/road-to-electric/](https://www.rac.co.uk/drive/electric-cars/choosing/road-to-electric/)

生成摘要时出错

---

## 76. HD Audio Driver for Windows 98SE / Me

**原文标题**: HD Audio Driver for Windows 98SE / Me

**原文链接**: [https://github.com/andrew-hoffman/wdmhda](https://github.com/andrew-hoffman/wdmhda)

生成摘要时出错

---

## 77. Stop picking my Go version for me

**原文标题**: Stop picking my Go version for me

**原文链接**: [https://blog.howardjohn.info/posts/go-mod-version/](https://blog.howardjohn.info/posts/go-mod-version/)

生成摘要时出错

---

## 78. Bitwarden integrates with OneCLI agent vault

**原文标题**: Bitwarden integrates with OneCLI agent vault

**原文链接**: [https://www.onecli.sh/blog/bitwarden-agent-access-sdk-onecli](https://www.onecli.sh/blog/bitwarden-agent-access-sdk-onecli)

生成摘要时出错

---

## 79. DoesItAgeVerify: The age verification status of Open Source Operating Systems

**原文标题**: DoesItAgeVerify: The age verification status of Open Source Operating Systems

**原文链接**: [https://github.com/BryanLunduke/DoesItAgeVerify](https://github.com/BryanLunduke/DoesItAgeVerify)

生成摘要时出错

---

## 80. Shipment of KitKat bars stolen en route from Italy to Poland

**原文标题**: Shipment of KitKat bars stolen en route from Italy to Poland

**原文链接**: [https://apnews.com/article/nestle-switzerland-candy-bar-stolen-kitkat-51073cce27a0e193651aa7f31aaa506e](https://apnews.com/article/nestle-switzerland-candy-bar-stolen-kitkat-51073cce27a0e193651aa7f31aaa506e)

生成摘要时出错

---

## 81. Will the AI data centre boom become a $9T bust?

**原文标题**: Will the AI data centre boom become a $9T bust?

**原文链接**: [https://www.ft.com/content/805f78f3-8da3-4fc0-b860-207a859ac723](https://www.ft.com/content/805f78f3-8da3-4fc0-b860-207a859ac723)

生成摘要时出错

---

## 82. DigitalOcean Seeks $800M in Funding

**原文标题**: DigitalOcean Seeks $800M in Funding

**原文链接**: [https://www.datacenterdynamics.com/en/news/digitalocean-seeks-800m-in-funding/](https://www.datacenterdynamics.com/en/news/digitalocean-seeks-800m-in-funding/)

生成摘要时出错

---

## 83. The sudden fall of Sora

**原文标题**: The sudden fall of Sora

**原文链接**: [https://www.wsj.com/tech/ai/the-sudden-fall-of-openais-most-hyped-product-since-chatgpt-64c730c9](https://www.wsj.com/tech/ai/the-sudden-fall-of-openais-most-hyped-product-since-chatgpt-64c730c9)

生成摘要时出错

---

## 84. AI isn't killing jobs, it's 'unbundling' them into lower-paid chunks

**原文标题**: AI isn't killing jobs, it's 'unbundling' them into lower-paid chunks

**原文链接**: [https://www.theregister.com/2026/03/24/ai_job_unbundling/](https://www.theregister.com/2026/03/24/ai_job_unbundling/)

生成摘要时出错

---

## 85. App that shows real-time lightning on Earth is showing bombings in Middle East

**原文标题**: App that shows real-time lightning on Earth is showing bombings in Middle East

**原文链接**: [https://maps.blitzortung.org/](https://maps.blitzortung.org/)

生成摘要时出错

---

## 86. Wikipedia officially bans AI-generated content

**原文标题**: Wikipedia officially bans AI-generated content

**原文链接**: [https://nypost.com/2026/03/28/tech/wikipedia-officially-bans-ai-generated-encyclopedia-entries/](https://nypost.com/2026/03/28/tech/wikipedia-officially-bans-ai-generated-encyclopedia-entries/)

生成摘要时出错

---

## 87. An NSFW filter for Marginalia search

**原文标题**: An NSFW filter for Marginalia search

**原文链接**: [https://www.marginalia.nu/log/a_134_nsfw/](https://www.marginalia.nu/log/a_134_nsfw/)

生成摘要时出错

---

## 88. Euro-Office Wants to Replace Google Docs and Microsoft Office

**原文标题**: Euro-Office Wants to Replace Google Docs and Microsoft Office

**原文链接**: [https://www.howtogeek.com/this-new-open-source-web-editor-wants-to-replace-google-docs-and-microsoft-office/](https://www.howtogeek.com/this-new-open-source-web-editor-wants-to-replace-google-docs-and-microsoft-office/)

生成摘要时出错

---

## 89. Show HN: Public transit systems as data – lines, stations, railcars, and history

**原文标题**: Show HN: Public transit systems as data – lines, stations, railcars, and history

**原文链接**: [https://publictransit.systems](https://publictransit.systems)

生成摘要时出错

---

