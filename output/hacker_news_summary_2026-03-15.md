# Hacker News 热门文章摘要 (2026-03-15)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 无龄 Linux：面向不分年龄人群的软件

**原文标题**: Ageless Linux – Software for humans of indeterminate age

**原文链接**: [https://agelesslinux.org/](https://agelesslinux.org/)

无龄Linux是一个基于Debian的操作系统，其明确创建旨在对抗加州数字年龄保障法案（AB 1043）。该法案强制要求对“操作系统提供商”、“应用程序”和“受涵盖应用商店”进行年龄验证。它认为AB 1043的定义过于宽泛，几乎涵盖了所有软件、开发者和分发方式，包括开源项目和简单的bash脚本。该法案还独特地将“用户”定义为儿童，监管他们的体验，同时将成年人归类为“基础设施”。

无龄Linux通过让用户安装Debian，然后运行一个转换脚本，来达到不合规的目的。该脚本会重塑操作系统的品牌，并部署一个不返回任何数据的存根年龄验证API，有意使该系统（和用户）成为一个不合规的“操作系统提供商”。

该项目主张AB 1043并非儿童安全法，而是一个“合规护城河”。它不成比例地惠及了已经拥有年龄验证系统的大公司（苹果、谷歌），同时给由志愿者运营的开源项目（Debian、Arch Linux）和小型开发者带来了无法逾越的成本。该法律的威力在于罚款威胁（每名儿童7,500美元），制造了抑制创新并迫使小型项目停止分发的法律风险。

无龄Linux还批评了该法律的“教育学”，认为年龄门槛教导儿童撒谎以绕过系统，从而损害了法律本身的感知合法性。相反，它倡导诚实、人类可读的安全建议、数字素养教育以及平台对有害内容的责任。

作为一种反抗的姿态，无龄Linux计划推出“无龄设备”——一款预装有其操作系统和一个不合规的“受涵盖应用商店”的低于15美元的单板计算机。这些设备将被故意分发给儿童，作为AB 1043明确且有记录的违规行为。

---

## 2. Mouser：Logi-Plus 鼠标软件的开源替代品

**原文标题**: Mouser: An open source alternative to Logi-Plus mouse software

**原文链接**: [https://github.com/TomBadash/MouseControl](https://github.com/TomBadash/MouseControl)

“Mouser”是一款轻量级、开源且完全本地化的罗技 Options+ 软件替代品，专为罗技 MX Master 3S 鼠标的按键重映射而设计。它的突出之处在于无需遥测、云服务或罗技账户。

主要功能包括重映射所有 6 个可编程按键（中键、手势键、前进/后退、水平滚动），以及支持应用程序配置文件，内置 22 种操作，涵盖导航、浏览器、编辑和媒体类别。用户可以控制 DPI（200-8000 DPI），独立的垂直和水平滚动反转，以及完整的 HID++ 2.0 手势按键支持（推荐使用蓝牙）。Mouser 还提供电池电量监控、自动重连和实时连接状态显示。

该应用程序采用现代 Qt Quick UI，带有交互式鼠标示意图，并在系统托盘中静默运行，自动检测前台应用程序以实现即时配置文件切换。它支持 Windows 和 macOS（使用 CGEventTap 进行钩子），并将配置本地存储。尽管目前主要针对 MX Master 3S (PID 0xB034) 进行了优化，但其架构具有可扩展性。重要的是，Logitech Options+ 必须未运行，因为它会与 Mouser 的 HID++ 访问发生冲突。未来的开发目标是支持更多设备、自定义组合键和 Linux。它可以作为便携式可执行文件或从源代码获取。

---

## 3. Digg 又没了

**原文标题**: Digg is gone again

**原文链接**: [https://digg.com/](https://digg.com/)

Digg首席执行官贾斯汀宣布进行“硬重置”，由于难以实现产品市场契合，将大幅裁员。这一决定归因于外部挑战，而非团队成员的能力问题。

一个主要因素是“前所未有的机器人问题”。复杂的AI代理和自动化账户涌入平台，导致无法确保投票和评论等真实互动。尽管封禁了数万个账户并部署了各种工具，Digg仍无法对抗这些机器人账户的规模和速度，损害了其社区的基础。首席执行官表示这是一个“互联网问题”，对Digg的影响尤为严重，因为“信任就是产品”。

此外，Digg低估了现有社交平台的强大网络效应和用户忠诚度，发现仅凭提供一个替代方案，极难吸引和留住用户。

尽管面临这些困境，Digg并未放弃。一支小而坚定的团队将以“彻底革新的切入点”重建平台，旨在打造真正与众不同的产品。至关重要的是，Digg的创始人凯文·罗斯将于四月全职回归，领导此次“再重启”。Diggnation播客也将每月继续更新。该公司向离职团队和社区表达感谢，重申其致力于构建一个值得信赖的互联网平台的承诺。

---

## 4. 美国经济数据不可靠了，会怎样？

**原文标题**: What happens when US economic data becomes unreliable

**原文链接**: [https://mitsloan.mit.edu/ideas-made-to-matter/what-happens-when-us-economic-data-becomes-unreliable](https://mitsloan.mit.edu/ideas-made-to-matter/what-happens-when-us-economic-data-becomes-unreliable)

美国经济数据收集系统依赖于13个主要统计机构，目前正面临严峻挑战，导致数据不可靠并引发公众不信任。麻省理工斯隆管理学院教授罗伯托·里戈邦和哈佛商学院教授阿尔贝托·卡瓦洛强调了三个关键问题：

1.  **调查回复率下降：** 越来越少的家庭和公司参与常规调查，这引入了偏差，延迟了修订，并削弱了关键指标的代表性。
2.  **资金限制：** 劳工统计局和人口普查局等统计机构的预算不断缩减，限制了它们采用新技术和扩展数据收集的能力。一个例子是美国农业部食物不安全调查的暂停。
3.  **政治干预：** 解雇统计负责人、将提名政治化以及政府停摆等行为损害了透明度和数据收集工作，尽管例行修订是健康系统的标志。

这些问题带来了严重的后果：政策制定者可能误判经济健康状况，投资者可能失去信心，公众可能不再关注官方数据。

里戈邦和卡瓦洛提出了企业领导者的两项主要行动建议：

1.  **谨慎使用私人数据：** 尽管私营部门数据可以补充官方统计数据，提供独立核查并填补空白，但由于其覆盖范围、商业动机和透明度存在局限，它无法完全取代政府数据。
2.  **积极发声：** 企业必须倡导数据完整性，抵制政治操纵，并对损害统计系统的政策表达担忧。

最终，通过投资、机构独立性和公众信任来保护美国统计系统，对于所有部门做出明智决策至关重要。

---

## 5. Spotify AI DJ 的 离谱愚蠢

**原文标题**: The Appalling Stupidity of Spotify's AI DJ

**原文链接**: [https://www.charlespetzold.com/blog/2026/02/The-Appalling-Stupidity-of-Spotifys-AI-DJ.html](https://www.charlespetzold.com/blog/2026/02/The-Appalling-Stupidity-of-Spotifys-AI-DJ.html)

作者批判性地评估了Spotify新推出的AI DJ，质疑人工智能中“智能”本身的定义。作为一名古典音乐专家，作者强调了Spotify以流行音乐为中心的元数据中长期存在的问题，这些元数据错误地将器乐“作品”标记为“歌曲”，并且未能正确区分作曲家和演奏家。

作者解释道，一个主要缺陷是Spotify无法将交响曲等多乐章古典作品理解为统一的、有顺序的整体。相反，它将各个乐章视为独立的曲目，从而破坏了作曲家预期的戏剧性结构。

通过一系列请求播放贝多芬第七交响曲的测试，AI DJ屡次失败。诸如“播放贝多芬第七交响曲完整版”的指令，结果却只播放了第二乐章，随后是无关的古典乐曲。即使是明确要求“所有四个乐章……按顺序播放”，也导致DJ播放了错误的交响曲，接着播放第七交响曲的乱序乐章（例如：第一、第二、然后第四、接着第三乐章，且来自不同的乐团），或者完全跳过某些乐章。最终，DJ突然转向了流行和摇滚歌曲。

作者总结称，AI DJ表现出了“令人震惊的愚蠢”，彻底未能掌握古典音乐至关重要的基本音乐概念。尽管该DJ仍处于测试阶段，但作者对显著的改进持怀疑态度，认为西方音乐传统的保存对于公司利润而言无关紧要。

---

## 6. 全欧洲含开箱游戏将获最低16岁评级

**原文标题**: Games with loot boxes to get minimum 16 age rating across Europe

**原文链接**: [https://www.bbc.com/news/articles/cge84xqjg5lo](https://www.bbc.com/news/articles/cge84xqjg5lo)

泛欧游戏信息组织 (PEGI) 将从六月开始在全欧洲（包括英国）实施新的年龄分级。包含“开箱”（loot box）机制的游戏——即游戏中购买随机神秘物品，模糊了游戏与赌博之间的界限——现在将至少获得PEGI 16的评级，甚至可能升至PEGI 18。

此举旨在为家长和玩家提供“更实用、更透明的建议”。年轻玩家与赌徒教育信托基金 (Ygam) 的艾米丽·托菲尔德 (Emily Tofield) 对此表示欢迎，但敦促将这些评级追溯应用于现有游戏，而不仅仅是新游戏，以保护已经在玩这些游戏的孩子。

尽管英国政府在2022年拒绝修订针对“开箱”机制的赌博法律，但行业指南现在限制18岁以下未成年人在未经父母同意的情况下购买它们。伯恩茅斯大学的王瑞杰博士 (Dr. Ruijie Wang) 强调，“开箱”机制是“类似赌博机制”的一个关键例子。

PEGI的其他更新包括：对于包含付费战斗通行证（如《堡垒之夜》）等有时限系统的游戏，评级为PEGI 12；对于NFT游戏，评级为PEGI 18；以及对于缺乏在线玩家举报或屏蔽工具的游戏，评级为PEGI 18。尽管这些变化是积极的，但它们的有效性最终取决于家长能否理解并认真对待新的评级。

---

## 7. 内核反作弊如何工作

**原文标题**: How kernel anti-cheats work

**原文链接**: [https://s4dbrd.github.io/posts/how-kernel-anti-cheats-work/](https://s4dbrd.github.io/posts/how-kernel-anti-cheats-work/)

内核反作弊是一种高度复杂的软件，它在Windows的最高特权级别（ring 0）运行，用于检测和阻止作弊行为。用户模式反作弊程序由于其较低的特权级别，很容易被内核模式作弊程序绕过，从而引发了一场“军备竞赛”，提高了作弊的成本和难度。

BattlEye、EasyAntiCheat (EAC)、Vanguard和FACEIT AC等主流系统都采用内核组件。Vanguard的独特之处在于它在系统启动时加载其驱动程序（vgk.sys），使其能够观察并列入所有后续驱动程序加载的白名单，这是一种比黑名单更强的安全模型。研究指出，从技术上讲，有效的内核反作弊程序与rootkit有共同之处，因为它们需要使用深层的操作系统原语来实现可见性。

这些系统通常遵循三组件架构：
1.  **内核驱动程序（ring 0）：** 注册回调、拦截系统调用、扫描内存并强制执行保护。
2.  **用户模式服务（SYSTEM特权）：** 处理网络通信、执行封禁和遥测。
3.  **游戏注入DLL（ring 3）：** 执行用户模式检查并应用游戏特定保护。

这些层之间的通信使用IOCTL（内核到服务）、命名管道（服务到DLL）以及用于高带宽数据的共享内存。驱动程序签名强制执行（DSE）是作弊开发者面临的关键障碍，需要有签名的驱动程序或绕过方法（BYOVD）。

一个基本的检测机制是使用内核回调，例如 `ObRegisterCallbacks`。通过注册进程和线程句柄操作，反作弊程序可以拦截并剥夺试图与游戏交互的外部进程的危险访问权限（例如 `PROCESS_VM_READ`/`WRITE`），从而防止常见的内存操纵作弊行为。

---

## 8. $96 3D-printed rocket that recalculates its mid-air trajectory using a $5 sensor

**原文标题**: $96 3D-printed rocket that recalculates its mid-air trajectory using a $5 sensor

**原文链接**: [https://github.com/novatic14/MANPADS-System-Launcher-and-Rocket](https://github.com/novatic14/MANPADS-System-Launcher-and-Rocket)

生成摘要时出错

---

## 9. Rack-mount hydroponics

**原文标题**: Rack-mount hydroponics

**原文链接**: [https://sa.lj.am/rack-mount-hydroponics/](https://sa.lj.am/rack-mount-hydroponics/)

生成摘要时出错

---

## 10. Allow me to get to know you, mistakes and all

**原文标题**: Allow me to get to know you, mistakes and all

**原文链接**: [https://sebi.io/posts/2026-03-14-allow-me-to-get-to-know-you-mistakes-and-all/](https://sebi.io/posts/2026-03-14-allow-me-to-get-to-know-you-mistakes-and-all/)

生成摘要时出错

---

## 11. RAM kits are now sold with one fake RAM stick alongside a real one

**原文标题**: RAM kits are now sold with one fake RAM stick alongside a real one

**原文链接**: [https://www.tomshardware.com/pc-components/ram/fake-ram-bundled-with-real-ram-to-create-a-performance-illusion-for-amd-users-1-1-value-pack-offers-desperate-psychological-relief-as-the-memory-shortage-worsens](https://www.tomshardware.com/pc-components/ram/fake-ram-bundled-with-real-ram-to-create-a-performance-illusion-for-amd-users-1-1-value-pack-offers-desperate-psychological-relief-as-the-memory-shortage-worsens)

生成摘要时出错

---

## 12. Montana passes Right to Compute act (2025)

**原文标题**: Montana passes Right to Compute act (2025)

**原文链接**: [https://www.westernmt.news/2025/04/21/montana-leads-the-nation-with-groundbreaking-right-to-compute-act/](https://www.westernmt.news/2025/04/21/montana-leads-the-nation-with-groundbreaking-right-to-compute-act/)

生成摘要时出错

---

## 13. A Visual Introduction to Machine Learning (2015)

**原文标题**: A Visual Introduction to Machine Learning (2015)

**原文链接**: [https://r2d3.us/visual-intro-to-machine-learning-part-1/](https://r2d3.us/visual-intro-to-machine-learning-part-1/)

生成摘要时出错

---

## 14. XML is a cheap DSL

**原文标题**: XML is a cheap DSL

**原文链接**: [https://unplannedobsolescence.com/blog/xml-cheap-dsl/](https://unplannedobsolescence.com/blog/xml-cheap-dsl/)

生成摘要时出错

---

## 15. Head of FCC threatens broadcaster licenses over critical coverage of Iran war

**原文标题**: Head of FCC threatens broadcaster licenses over critical coverage of Iran war

**原文链接**: [https://twitter.com/BrendanCarrFCC/status/2032855414233047172](https://twitter.com/BrendanCarrFCC/status/2032855414233047172)

生成摘要时出错

---

## 16. Claude March 2026 usage promotion

**原文标题**: Claude March 2026 usage promotion

**原文链接**: [https://support.claude.com/en/articles/14063676-claude-march-2026-usage-promotion](https://support.claude.com/en/articles/14063676-claude-march-2026-usage-promotion)

生成摘要时出错

---

## 17. MCP is dead; long live MCP

**原文标题**: MCP is dead; long live MCP

**原文链接**: [https://chrlschn.dev/blog/2026/03/mcp-is-dead-long-live-mcp/](https://chrlschn.dev/blog/2026/03/mcp-is-dead-long-live-mcp/)

生成摘要时出错

---

## 18. GIMP 3.2 released

**原文标题**: GIMP 3.2 released

**原文链接**: [https://www.gimp.org/news/2026/03/14/gimp-3-2-released/](https://www.gimp.org/news/2026/03/14/gimp-3-2-released/)

生成摘要时出错

---

## 19. Marketing for Founders

**原文标题**: Marketing for Founders

**原文链接**: [https://github.com/EdoStra/Marketing-for-Founders](https://github.com/EdoStra/Marketing-for-Founders)

生成摘要时出错

---

## 20. Harold and George Destroy the World

**原文标题**: Harold and George Destroy the World

**原文链接**: [https://tomclancy.info/harold-and-george.html](https://tomclancy.info/harold-and-george.html)

生成摘要时出错

---

## 21. Show HN: Han – A Korean programming language written in Rust

**原文标题**: Show HN: Han – A Korean programming language written in Rust

**原文链接**: [https://github.com/xodn348/han](https://github.com/xodn348/han)

生成摘要时出错

---

## 22. A most elegant TCP hole punching algorithm

**原文标题**: A most elegant TCP hole punching algorithm

**原文链接**: [https://robertsdotpm.github.io/cryptography/tcp_hole_punching.html](https://robertsdotpm.github.io/cryptography/tcp_hole_punching.html)

生成摘要时出错

---

## 23. Bumblebee queens breathe underwater to survive drowning

**原文标题**: Bumblebee queens breathe underwater to survive drowning

**原文链接**: [https://www.smithsonianmag.com/science-nature/bumblebee-queens-breathe-underwater-to-survive-drowning-revealing-how-they-can-live-submerged-for-a-week-180988330/](https://www.smithsonianmag.com/science-nature/bumblebee-queens-breathe-underwater-to-survive-drowning-revealing-how-they-can-live-submerged-for-a-week-180988330/)

生成摘要时出错

---

## 24. The 100 hour gap between a vibecoded prototype and a working product

**原文标题**: The 100 hour gap between a vibecoded prototype and a working product

**原文链接**: [https://kanfa.macbudkowski.com/vibecoding-cryptosaurus](https://kanfa.macbudkowski.com/vibecoding-cryptosaurus)

生成摘要时出错

---

## 25. Human Rights Watch says drone strikes in Haiti have killed nearly 1,250 people

**原文标题**: Human Rights Watch says drone strikes in Haiti have killed nearly 1,250 people

**原文链接**: [https://haitiantimes.com/2026/03/11/hrw-condemns-haiti-drone-strikes-killing-children/](https://haitiantimes.com/2026/03/11/hrw-condemns-haiti-drone-strikes-killing-children/)

生成摘要时出错

---

## 26. Airbus is preparing two uncrewed combat aircraft

**原文标题**: Airbus is preparing two uncrewed combat aircraft

**原文链接**: [https://www.airbus.com/en/newsroom/press-releases/2026-03-airbus-is-preparing-two-uncrewed-combat-aircraft-from-kratos-for-first-flight-with-a-european](https://www.airbus.com/en/newsroom/press-releases/2026-03-airbus-is-preparing-two-uncrewed-combat-aircraft-from-kratos-for-first-flight-with-a-european)

生成摘要时出错

---

## 27. 2026 tech layoffs reach 45,000 in March

**原文标题**: 2026 tech layoffs reach 45,000 in March

**原文链接**: [https://technode.global/2026/03/09/2026-tech-layoffs-reach-45000-in-march-more-than-9200-due-to-ai-and-automation-rationalfx/](https://technode.global/2026/03/09/2026-tech-layoffs-reach-45000-in-march-more-than-9200-due-to-ai-and-automation-rationalfx/)

生成摘要时出错

---

## 28. Changes to OpenTTD Distribution on Steam

**原文标题**: Changes to OpenTTD Distribution on Steam

**原文链接**: [https://www.openttd.org/news/2026/03/14/steam-changes](https://www.openttd.org/news/2026/03/14/steam-changes)

生成摘要时出错

---

## 29. An ode to bzip

**原文标题**: An ode to bzip

**原文链接**: [https://purplesyringa.moe/blog/an-ode-to-bzip/](https://purplesyringa.moe/blog/an-ode-to-bzip/)

生成摘要时出错

---

## 30. Please do not A/B test my workflow

**原文标题**: Please do not A/B test my workflow

**原文链接**: [https://backnotprop.com/blog/do-not-ab-test-my-workflow/](https://backnotprop.com/blog/do-not-ab-test-my-workflow/)

生成摘要时出错

---

## 31. Nmap in the movies (2008)

**原文标题**: Nmap in the movies (2008)

**原文链接**: [https://nmap.org/movies/](https://nmap.org/movies/)

生成摘要时出错

---

## 32. Starlink militarization and its impact on global strategic stability (2023)

**原文标题**: Starlink militarization and its impact on global strategic stability (2023)

**原文链接**: [https://interpret.csis.org/translations/starlink-militarization-and-its-impact-on-global-strategic-stability/](https://interpret.csis.org/translations/starlink-militarization-and-its-impact-on-global-strategic-stability/)

生成摘要时出错

---

## 33. I beg you to follow Crocker's Rules, even if you will be rude to me

**原文标题**: I beg you to follow Crocker's Rules, even if you will be rude to me

**原文链接**: [https://lr0.org/blog/p/crocker/](https://lr0.org/blog/p/crocker/)

生成摘要时出错

---

## 34. I found 39 Algolia admin keys exposed across open source documentation sites

**原文标题**: I found 39 Algolia admin keys exposed across open source documentation sites

**原文链接**: [https://benzimmermann.dev/blog/algolia-docsearch-admin-keys](https://benzimmermann.dev/blog/algolia-docsearch-admin-keys)

生成摘要时出错

---

## 35. Treasure hunter freed from jail after refusing to turn over shipwreck gold

**原文标题**: Treasure hunter freed from jail after refusing to turn over shipwreck gold

**原文链接**: [https://www.bbc.com/news/articles/cg4g7kn99q3o](https://www.bbc.com/news/articles/cg4g7kn99q3o)

生成摘要时出错

---

## 36. Launching the Claude Partner Network

**原文标题**: Launching the Claude Partner Network

**原文链接**: [https://www.anthropic.com/news/claude-partner-network](https://www.anthropic.com/news/claude-partner-network)

生成摘要时出错

---

## 37. Pentagon expands oversight of Stars and Stripes, limits content

**原文标题**: Pentagon expands oversight of Stars and Stripes, limits content

**原文链接**: [https://www.stripes.com/theaters/us/2026-03-13/pentagon-modernization-plan-stars-and-stripes-21051529.html](https://www.stripes.com/theaters/us/2026-03-13/pentagon-modernization-plan-stars-and-stripes-21051529.html)

生成摘要时出错

---

## 38. An investigation of the forces behind the age-verification bills

**原文标题**: An investigation of the forces behind the age-verification bills

**原文链接**: [https://old.reddit.com/r/linux/comments/1rshc1f/i_traced_2_billion_in_nonprofit_grants_and_45/](https://old.reddit.com/r/linux/comments/1rshc1f/i_traced_2_billion_in_nonprofit_grants_and_45/)

生成摘要时出错

---

## 39. Philosoph Jürgen Habermas Gestorben

**原文标题**: Philosoph Jürgen Habermas Gestorben

**原文链接**: [https://www.spiegel.de/kultur/philosoph-juergen-habermas-mit-96-jahren-gestorben-a-8be73ac7-e722-4543-8344-4515c4040363](https://www.spiegel.de/kultur/philosoph-juergen-habermas-mit-96-jahren-gestorben-a-8be73ac7-e722-4543-8344-4515c4040363)

生成摘要时出错

---

## 40. Google Fiber will be sold to private equity firm and merge with cable company

**原文标题**: Google Fiber will be sold to private equity firm and merge with cable company

**原文链接**: [https://arstechnica.com/tech-policy/2026/03/google-fiber-will-be-sold-to-private-equity-firm-and-merge-with-cable-company/](https://arstechnica.com/tech-policy/2026/03/google-fiber-will-be-sold-to-private-equity-firm-and-merge-with-cable-company/)

生成摘要时出错

---

## 41. Sunsetting Jazzband

**原文标题**: Sunsetting Jazzband

**原文链接**: [https://jazzband.co/news/2026/03/14/sunsetting-jazzband](https://jazzband.co/news/2026/03/14/sunsetting-jazzband)

生成摘要时出错

---

## 42. Glassworm Is Back: A New Wave of Invisible Unicode Attacks Hits Repositories

**原文标题**: Glassworm Is Back: A New Wave of Invisible Unicode Attacks Hits Repositories

**原文链接**: [https://www.aikido.dev/blog/glassworm-returns-unicode-attack-github-npm-vscode](https://www.aikido.dev/blog/glassworm-returns-unicode-attack-github-npm-vscode)

生成摘要时出错

---

## 43. SBCL Fibers – Lightweight Cooperative Threads

**原文标题**: SBCL Fibers – Lightweight Cooperative Threads

**原文链接**: [https://atgreen.github.io/repl-yell/posts/sbcl-fibers/](https://atgreen.github.io/repl-yell/posts/sbcl-fibers/)

生成摘要时出错

---

## 44. Megadev: A Development Kit for the Sega Mega Drive and Mega CD Hardware

**原文标题**: Megadev: A Development Kit for the Sega Mega Drive and Mega CD Hardware

**原文链接**: [https://github.com/drojaazu/megadev](https://github.com/drojaazu/megadev)

生成摘要时出错

---

## 45. AI didn't simplify software engineering: It just made bad engineering easier

**原文标题**: AI didn't simplify software engineering: It just made bad engineering easier

**原文链接**: [https://robenglander.com/writing/ai-did-not-simplify/](https://robenglander.com/writing/ai-did-not-simplify/)

生成摘要时出错

---

## 46. Show HN: GitAgent – An open standard that turns any Git repo into an AI agent

**原文标题**: Show HN: GitAgent – An open standard that turns any Git repo into an AI agent

**原文链接**: [https://www.gitagent.sh/](https://www.gitagent.sh/)

生成摘要时出错

---

## 47. UBI as a productivity dividend

**原文标题**: UBI as a productivity dividend

**原文链接**: [https://scottsantens.substack.com/p/universal-basic-income-is-your-productivity](https://scottsantens.substack.com/p/universal-basic-income-is-your-productivity)

生成摘要时出错

---

## 48. What makes Intel Optane stand out (2023)

**原文标题**: What makes Intel Optane stand out (2023)

**原文链接**: [https://blog.zuthof.nl/2023/06/02/what-makes-intel-optane-stand-out/](https://blog.zuthof.nl/2023/06/02/what-makes-intel-optane-stand-out/)

生成摘要时出错

---

## 49. Fedora 44 on the Raspberry Pi 5

**原文标题**: Fedora 44 on the Raspberry Pi 5

**原文链接**: [https://nullr0ute.com/2026/03/fedora-44-on-the-raspberry-pi-5/](https://nullr0ute.com/2026/03/fedora-44-on-the-raspberry-pi-5/)

生成摘要时出错

---

## 50. It's time to move your docs in the repo

**原文标题**: It's time to move your docs in the repo

**原文链接**: [https://www.dein.fr/posts/2026-03-13-its-time-to-move-your-docs-in-the-repo](https://www.dein.fr/posts/2026-03-13-its-time-to-move-your-docs-in-the-repo)

生成摘要时出错

---

## 51. Office.eu launches as Europe's sovereign office platform

**原文标题**: Office.eu launches as Europe's sovereign office platform

**原文链接**: [https://office.eu/media/pressrelease-20260304](https://office.eu/media/pressrelease-20260304)

生成摘要时出错

---

## 52. FCC chairman threatens TV broadcast licenses over news coverage

**原文标题**: FCC chairman threatens TV broadcast licenses over news coverage

**原文链接**: [https://fortune.com/2026/03/14/fcc-brendan-carr-tv-broadcast-licenses-news-coverage-us-war-iran-trump/](https://fortune.com/2026/03/14/fcc-brendan-carr-tv-broadcast-licenses-news-coverage-us-war-iran-trump/)

生成摘要时出错

---

## 53. Hostile Volume – A game about adjusting volume with intentionally bad UI

**原文标题**: Hostile Volume – A game about adjusting volume with intentionally bad UI

**原文链接**: [https://hostilevolume.com/](https://hostilevolume.com/)

生成摘要时出错

---

## 54. Grandparents are glued to their phones, families are worried [video]

**原文标题**: Grandparents are glued to their phones, families are worried [video]

**原文链接**: [https://www.bbc.com/reel/video/p0n61dg3/grandparents-are-glued-to-their-phones-families-are-worried](https://www.bbc.com/reel/video/p0n61dg3/grandparents-are-glued-to-their-phones-families-are-worried)

生成摘要时出错

---

## 55. Library of Short Stories

**原文标题**: Library of Short Stories

**原文链接**: [https://www.libraryofshortstories.com/](https://www.libraryofshortstories.com/)

生成摘要时出错

---

## 56. Separating the Wayland compositor and window manager

**原文标题**: Separating the Wayland compositor and window manager

**原文链接**: [https://isaacfreund.com/blog/river-window-management/](https://isaacfreund.com/blog/river-window-management/)

生成摘要时出错

---

## 57. ICE agents reveal daily arrest quotas and surveillance app in court testimony

**原文标题**: ICE agents reveal daily arrest quotas and surveillance app in court testimony

**原文链接**: [https://www.theguardian.com/us-news/2026/mar/13/ice-agent-court-testimony-oregon](https://www.theguardian.com/us-news/2026/mar/13/ice-agent-court-testimony-oregon)

生成摘要时出错

---

## 58. Hazardous substances found in all headphones tested by ToxFREE project

**原文标题**: Hazardous substances found in all headphones tested by ToxFREE project

**原文链接**: [https://arnika.org/en/news/the-sound-of-contamination-all-analysed-headphones-on-the-central-european-market-found-to-contain-hormone-disrupting-chemicals](https://arnika.org/en/news/the-sound-of-contamination-all-analysed-headphones-on-the-central-european-market-found-to-contain-hormone-disrupting-chemicals)

生成摘要时出错

---

## 59. U.S. Built a Blueprint to Avoid Civilian War Casualties. DOJ Scrapped It

**原文标题**: U.S. Built a Blueprint to Avoid Civilian War Casualties. DOJ Scrapped It

**原文链接**: [https://www.propublica.org/article/trump-defense-department-iran-hegseth-civilian-casualties](https://www.propublica.org/article/trump-defense-department-iran-hegseth-civilian-casualties)

生成摘要时出错

---

## 60. Mathematics Distillation Challenge – Equational Theories

**原文标题**: Mathematics Distillation Challenge – Equational Theories

**原文链接**: [https://terrytao.wordpress.com/2026/03/13/mathematics-distillation-challenge-equational-theories/](https://terrytao.wordpress.com/2026/03/13/mathematics-distillation-challenge-equational-theories/)

生成摘要时出错

---

## 61. Meta planning layoffs as AI costs mount

**原文标题**: Meta planning layoffs as AI costs mount

**原文链接**: [https://www.reuters.com/business/world-at-work/meta-planning-sweeping-layoffs-ai-costs-mount-2026-03-14/](https://www.reuters.com/business/world-at-work/meta-planning-sweeping-layoffs-ai-costs-mount-2026-03-14/)

生成摘要时出错

---

## 62. The enshittification of Amazon paperback books

**原文标题**: The enshittification of Amazon paperback books

**原文链接**: [https://www.alexerhardt.com/en/enshittification-amazon-paperback-books/](https://www.alexerhardt.com/en/enshittification-amazon-paperback-books/)

生成摘要时出错

---

## 63. Show HN: Signet – Autonomous wildfire tracking from satellite and weather data

**原文标题**: Show HN: Signet – Autonomous wildfire tracking from satellite and weather data

**原文链接**: [https://signet.watch](https://signet.watch)

生成摘要时出错

---

## 64. Jeff Bezos wants Washington Post’s newsroom budget halved, productivity doubled

**原文标题**: Jeff Bezos wants Washington Post’s newsroom budget halved, productivity doubled

**原文链接**: [https://www.nytimes.com/2026/03/14/business/media/washington-post-jeff-bezos-layoffs.html](https://www.nytimes.com/2026/03/14/business/media/washington-post-jeff-bezos-layoffs.html)

生成摘要时出错

---

## 65. Stanford researchers report first recording of a blue whale's heart rate (2019)

**原文标题**: Stanford researchers report first recording of a blue whale's heart rate (2019)

**原文链接**: [https://news.stanford.edu/stories/2019/11/first-ever-recording-blue-whales-heart-rate](https://news.stanford.edu/stories/2019/11/first-ever-recording-blue-whales-heart-rate)

生成摘要时出错

---

## 66. Online astroturfing: A problem beyond disinformation (2022)

**原文标题**: Online astroturfing: A problem beyond disinformation (2022)

**原文链接**: [https://journals.sagepub.com/doi/10.1177/01914537221108467](https://journals.sagepub.com/doi/10.1177/01914537221108467)

生成摘要时出错

---

## 67. Our Experience with I-Ready

**原文标题**: Our Experience with I-Ready

**原文链接**: [https://moultano.wordpress.com/2026/03/12/our-experience-with-i-ready/](https://moultano.wordpress.com/2026/03/12/our-experience-with-i-ready/)

生成摘要时出错

---

## 68. The wild six weeks for NanoClaw's creator that led to a deal with Docker

**原文标题**: The wild six weeks for NanoClaw's creator that led to a deal with Docker

**原文链接**: [https://techcrunch.com/2026/03/13/the-wild-six-weeks-for-nanoclaws-creator-that-led-to-a-deal-with-docker/](https://techcrunch.com/2026/03/13/the-wild-six-weeks-for-nanoclaws-creator-that-led-to-a-deal-with-docker/)

生成摘要时出错

---

## 69. Tree Search Distillation for Language Models Using PPO

**原文标题**: Tree Search Distillation for Language Models Using PPO

**原文链接**: [https://ayushtambde.com/blog/tree-search-distillation-for-language-models-using-ppo/](https://ayushtambde.com/blog/tree-search-distillation-for-language-models-using-ppo/)

生成摘要时出错

---

## 70. Israel is running critically low on interceptors, US officials say

**原文标题**: Israel is running critically low on interceptors, US officials say

**原文链接**: [https://www.semafor.com/article/03/14/2026/israel-is-running-critically-low-on-interceptors-us-officials-say](https://www.semafor.com/article/03/14/2026/israel-is-running-critically-low-on-interceptors-us-officials-say)

生成摘要时出错

---

## 71. Federal Surveillance Tech Becomes Mandatory in New Cars by 2027

**原文标题**: Federal Surveillance Tech Becomes Mandatory in New Cars by 2027

**原文链接**: [https://www.gadgetreview.com/federal-surveillance-tech-becomes-mandatory-in-new-cars-by-2027](https://www.gadgetreview.com/federal-surveillance-tech-becomes-mandatory-in-new-cars-by-2027)

生成摘要时出错

---

## 72. The US slashed research for cancer, Alzheimer's, mental health – and more

**原文标题**: The US slashed research for cancer, Alzheimer's, mental health – and more

**原文链接**: [https://www.vox.com/future-perfect/482363/nih-medical-research-grants-cut-2025](https://www.vox.com/future-perfect/482363/nih-medical-research-grants-cut-2025)

生成摘要时出错

---

## 73. Jared Kushner Solicits Funds for His Firm While Working as Mideast Envoy

**原文标题**: Jared Kushner Solicits Funds for His Firm While Working as Mideast Envoy

**原文链接**: [https://www.nytimes.com/2026/03/13/business/jared-kushner-affinity-mideast-funds.html](https://www.nytimes.com/2026/03/13/business/jared-kushner-affinity-mideast-funds.html)

生成摘要时出错

---

## 74. Learning Creative Coding

**原文标题**: Learning Creative Coding

**原文链接**: [https://stigmollerhansen.dk/resume/learning-creative-coding/](https://stigmollerhansen.dk/resume/learning-creative-coding/)

生成摘要时出错

---

## 75. AI Gets Wrong Woman Jailed for Six Months, Life Ruined

**原文标题**: AI Gets Wrong Woman Jailed for Six Months, Life Ruined

**原文链接**: [https://www.youtube.com/watch?v=mzS7dmCUzcQ](https://www.youtube.com/watch?v=mzS7dmCUzcQ)

生成摘要时出错

---

## 76. ArXiv is establishing itself as an independent nonprofit organization

**原文标题**: ArXiv is establishing itself as an independent nonprofit organization

**原文链接**: [https://jobs.chronicle.com/job/37961678/chief-executive-officer](https://jobs.chronicle.com/job/37961678/chief-executive-officer)

生成摘要时出错

---

## 77. Postgres with Builtin File Systems

**原文标题**: Postgres with Builtin File Systems

**原文链接**: [https://db9.ai/](https://db9.ai/)

生成摘要时出错

---

## 78. Age Verification Lobbying: Dark Money, Model Legislation, Institutional Capture

**原文标题**: Age Verification Lobbying: Dark Money, Model Legislation, Institutional Capture

**原文链接**: [https://tboteproject.com](https://tboteproject.com)

生成摘要时出错

---

## 79. Codegen is not productivity

**原文标题**: Codegen is not productivity

**原文链接**: [https://www.antifound.com/posts/codegen-is-not-productivity/](https://www.antifound.com/posts/codegen-is-not-productivity/)

生成摘要时出错

---

## 80. Optimizing Content for Agents

**原文标题**: Optimizing Content for Agents

**原文链接**: [https://cra.mr/optimizing-content-for-agents/](https://cra.mr/optimizing-content-for-agents/)

生成摘要时出错

---

## 81. Hollywood Enters Oscars Weekend in Existential Crisis

**原文标题**: Hollywood Enters Oscars Weekend in Existential Crisis

**原文链接**: [https://www.theculturenewspaper.com/hollywood-enters-oscars-weekend-in-existential-crisis/](https://www.theculturenewspaper.com/hollywood-enters-oscars-weekend-in-existential-crisis/)

生成摘要时出错

---

## 82. $2B nonprofit grants traced to find who's behind age verification bills

**原文标题**: $2B nonprofit grants traced to find who's behind age verification bills

**原文链接**: [https://old.reddit.com/r/linux/comments/1rshc1f/i_traced_2_billion_in_nonprofit_grants_and_45/](https://old.reddit.com/r/linux/comments/1rshc1f/i_traced_2_billion_in_nonprofit_grants_and_45/)

生成摘要时出错

---

## 83. Palantir defends its role in the kill chain: "We are proud of that"

**原文标题**: Palantir defends its role in the kill chain: "We are proud of that"

**原文链接**: [https://www.heise.de/en/news/Palantir-defends-its-role-in-the-kill-chain-We-are-very-very-proud-of-that-11211275.html](https://www.heise.de/en/news/Palantir-defends-its-role-in-the-kill-chain-We-are-very-very-proud-of-that-11211275.html)

生成摘要时出错

---

## 84. UMD Scientists Create 'Smart Underwear' to Measure Human Flatulence

**原文标题**: UMD Scientists Create 'Smart Underwear' to Measure Human Flatulence

**原文链接**: [https://cbmg.umd.edu/news-events/news/brantley-hall-umd-scientists-create-smart-underwear-measure-human-flatulence](https://cbmg.umd.edu/news-events/news/brantley-hall-umd-scientists-create-smart-underwear-measure-human-flatulence)

生成摘要时出错

---

## 85. The most SHAMELESS structural manipulation of a index I've ever seen

**原文标题**: The most SHAMELESS structural manipulation of a index I've ever seen

**原文链接**: [https://substack.com/@georgenoble/note/c-226667679](https://substack.com/@georgenoble/note/c-226667679)

生成摘要时出错

---

## 86. Generating All 32-Bit Primes (Part I)

**原文标题**: Generating All 32-Bit Primes (Part I)

**原文链接**: [https://hnlyman.github.io/pages/prime32_I.html](https://hnlyman.github.io/pages/prime32_I.html)

生成摘要时出错

---

## 87. Show HN: Learn Arabic with spaced repetition and comprehensible input

**原文标题**: Show HN: Learn Arabic with spaced repetition and comprehensible input

**原文链接**: [https://abjadpro.com](https://abjadpro.com)

生成摘要时出错

---

## 88. Meta is reportedly laying off up to 20 percent of its staff

**原文标题**: Meta is reportedly laying off up to 20 percent of its staff

**原文链接**: [https://www.theverge.com/business/895026/meta-laying-off-20-percent](https://www.theverge.com/business/895026/meta-laying-off-20-percent)

生成摘要时出错

---

## 89. IBM, sonic delay lines, and the history of the 80×24 display (2019)

**原文标题**: IBM, sonic delay lines, and the history of the 80×24 display (2019)

**原文链接**: [https://www.righto.com/2019/11/ibm-sonic-delay-lines-and-history-of.html](https://www.righto.com/2019/11/ibm-sonic-delay-lines-and-history-of.html)

生成摘要时出错

---

## 90. The Washington Post Is Using Reader Data to Set Subscription Prices

**原文标题**: The Washington Post Is Using Reader Data to Set Subscription Prices

**原文链接**: [https://washingtonian.com/2026/03/12/the-washington-post-is-using-reader-data-to-set-subscription-prices-how-does-that-work/](https://washingtonian.com/2026/03/12/the-washington-post-is-using-reader-data-to-set-subscription-prices-how-does-that-work/)

生成摘要时出错

---

## 91. Learning athletic humanoid tennis skills from imperfect human motion data

**原文标题**: Learning athletic humanoid tennis skills from imperfect human motion data

**原文链接**: [https://zzk273.github.io/LATENT/](https://zzk273.github.io/LATENT/)

生成摘要时出错

---

## 92. Small U.S. town, big company. Can it weather the tariff Blizzard? (Digi-Key) (2025)

**原文标题**: Small U.S. town, big company. Can it weather the tariff Blizzard? (Digi-Key) (2025)

**原文链接**: [https://www.npr.org/2025/04/24/nx-s1-5332209/digikey-tariff-small-minnesota-town-big-company](https://www.npr.org/2025/04/24/nx-s1-5332209/digikey-tariff-small-minnesota-town-big-company)

生成摘要时出错

---

## 93. Show HN: What if your synthesizer was powered by APL (or a dumb K clone)?

**原文标题**: Show HN: What if your synthesizer was powered by APL (or a dumb K clone)?

**原文链接**: [https://octetta.github.io/k-synth/](https://octetta.github.io/k-synth/)

生成摘要时出错

---

## 94. Show HN: GrobPaint: Somewhere Between MS Paint and Paint.net

**原文标题**: Show HN: GrobPaint: Somewhere Between MS Paint and Paint.net

**原文链接**: [https://github.com/groverburger/grobpaint](https://github.com/groverburger/grobpaint)

生成摘要时出错

---

## 95. Claudetop – htop for Claude Code sessions (see your AI spend in real-time)

**原文标题**: Claudetop – htop for Claude Code sessions (see your AI spend in real-time)

**原文链接**: [https://github.com/liorwn/claudetop](https://github.com/liorwn/claudetop)

生成摘要时出错

---

## 96. U.S. Tech Giants Flocked to the Persian Gulf. Now They Are Targets

**原文标题**: U.S. Tech Giants Flocked to the Persian Gulf. Now They Are Targets

**原文链接**: [https://www.nytimes.com/2026/03/13/technology/amazon-google-persian-gulf-war.html](https://www.nytimes.com/2026/03/13/technology/amazon-google-persian-gulf-war.html)

生成摘要时出错

---

## 97. The Forth Language [Byte Magazine Volume 05 Number 08] (1980)

**原文标题**: The Forth Language [Byte Magazine Volume 05 Number 08] (1980)

**原文链接**: [https://archive.org/details/byte-magazine-1980-08](https://archive.org/details/byte-magazine-1980-08)

生成摘要时出错

---

## 98. How Lego builds a new Lego set (2023)

**原文标题**: How Lego builds a new Lego set (2023)

**原文链接**: [https://www.theverge.com/c/23991049/lego-ideas-polaroid-onestep-behind-the-scenes-price](https://www.theverge.com/c/23991049/lego-ideas-polaroid-onestep-behind-the-scenes-price)

生成摘要时出错

---

## 99. Who Goes Nazi? (1941)

**原文标题**: Who Goes Nazi? (1941)

**原文链接**: [https://harpers.org/archive/1941/08/who-goes-nazi/](https://harpers.org/archive/1941/08/who-goes-nazi/)

生成摘要时出错

---

## 100. SpaceX IPO Scandal

**原文标题**: SpaceX IPO Scandal

**原文链接**: [https://www.youtube.com/watch?v=8rS3fTbC7TE](https://www.youtube.com/watch?v=8rS3fTbC7TE)

生成摘要时出错

---

