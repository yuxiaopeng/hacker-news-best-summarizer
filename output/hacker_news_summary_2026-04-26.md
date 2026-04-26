# Hacker News 热门文章摘要 (2026-04-26)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 西方忘记了如何制造东西，现在它正在忘记如何编程。

**原文标题**: The West forgot how to make things, now it’s forgetting how to code

**原文链接**: [https://techtrenches.dev/p/the-west-forgot-how-to-make-things](https://techtrenches.dev/p/the-west-forgot-how-to-make-things)

文章认为，西方在忘记如何制造必需品之后，如今正因过度依赖人工智能而忽视熟练软件工程师的培养，重蹈覆辙。

作者通过国防工业的困境阐明了这一点。在数十年后重启“毒刺”导弹生产，需要请回退休工程师来教导年轻工人，这暴露了知识流失和设备过时的问题。同样，欧洲未能兑现其生产一百万枚炮弹的承诺，原因在于生产碎片化、工厂关闭以及国内推进剂短缺，这凸显了一个为小批量而非大规模或危机生产优化的行业。“雾堤”（Fogbank）事件——其中关键核材料无法复制，因为其生产知识（包括一种关键的未记录的杂质）已随着最初的工人退休而消失——敲响了严峻的警钟。

这种模式——即建立能力、寻找更廉价的替代品（如“和平红利”）、任由人类专业知识萎缩，然后在危机中面临崩溃——现在正随着人工智能的出现，在软件行业中上演。尽管人工智能能快速生成代码，但人工审查却成了瓶颈；作者指出，大学入学人数下降，初级工程师招聘减少，许多开发者开始依赖“AI中介能力”，而非深入理解。

培养一名合格的资深工程师需要5-10年，这是一个无法通过金钱或人工智能来缩短的时间线。作者警告说，从形成性错误和实践经验中获得的默会知识正在流失。随着当前资深工程师的退休，端到端系统理解和复杂调试所需的关键机构知识将会消失，从而形成一个“代码的雾堤”。西方对人工智能优化的押注，就像其早前对永久和平的押注一样，可能会导致未来软件能力丧失的危机。

---

## 2. ChatGPT助力业余者解决厄尔多斯问题

**原文标题**: Amateur armed with ChatGPT solves an Erdős problem

**原文链接**: [https://www.scientificamerican.com/article/amateur-armed-with-chatgpt-vibe-maths-a-60-year-old-problem/](https://www.scientificamerican.com/article/amateur-armed-with-chatgpt-vibe-maths-a-60-year-old-problem/)

2026年4月24日，23岁的业余爱好者利亚姆·普莱斯在没有受过高等数学训练的情况下，仅通过一次对ChatGPT Pro（GPT-5.4 Pro）的提示，解决了困扰数学界长达60年的埃尔德什问题。这个问题涉及整数的“本原集”（其中集合中任何一个数都不能被另一个数整除）以及与它们相关的“埃尔德什和”。这一特定的猜想几十年来一直困扰着著名的数学家。

洛杉矶加州大学的陶哲轩和斯坦福大学的贾里德·利希特曼等专家证实了该解决方案的有效性，更重要的是，证实了其新颖性。与之前人类尝试总是走错第一步不同，ChatGPT采用了一种全新的方法。它应用了一个来自不同领域的众所周知的数学公式，而没有任何人类曾认为与这类特定问题相关。

尽管人工智能的原始证明最初“相当糟糕”，并需要利希特曼和陶哲轩进行专家提炼，但其核心洞察力——一次“认知飞跃”——被认为是开创性的。这一成就表明，人工智能可以发现真正原创的数学方法，而不仅仅是复制人类的思维。专家们认为，这种“思考大数及其结构的新方式”可能具有更广泛的应用，证实了先前关于这些复杂问题中统一主题的直觉，并预示着人工智能在纯数学领域的一个新前沿。

---

## 3. 新万兆USB网卡：更低温、更小、更便宜

**原文标题**: New 10 GbE USB adapters are cooler, smaller, cheaper

**原文链接**: [https://www.jeffgeerling.com/blog/2026/new-10-gbe-usb-adapters-cooler-smaller-cheaper/](https://www.jeffgeerling.com/blog/2026/new-10-gbe-usb-adapters-cooler-smaller-cheaper/)

基于RTL8159芯片的新型10千兆以太网USB 3.2适配器正在兴起，成为相比传统雷电10千兆以太网适配器更小巧、更凉爽、更便宜的替代品。例如，WisdPi 10G适配器售价80美元，不及雷电型号价格的一半，并且运行温度显著更低（42.5°C），无需大型散热片。

然而，实现完整的10 Gbps速度是一个重要的注意事项。测试表明，只有配备USB 3.2 Gen 2x2（20 Gbps）端口的台式PC才能稳定达到接近10 Gbps的速度。其他系统，如Mac电脑和配备USB 3.1/3.2 Gen 2（10 Gbps）端口的Framework 13笔记本，仅达到6-7 Gbps，凸显了主机USB带宽的影响。复杂的USB命名规范以及Windows系统将USB 3.x连接错误报告为“3.0”的倾向，进一步增加了识别兼容端口的难度。

尽管Mac电脑支持即插即用，Windows系统则需要安装驱动程序。双向测试显示性能各异，Mac电脑能对称处理数据流量，但其他系统则表现出差异。

总的来说，如果你有一个10 Gbps的RJ45网络，并且电脑配备了USB 3.2 Gen 2x2端口，这些适配器物有所值。如果没有高带宽的USB端口，2.5 Gbps或5 Gbps的USB适配器在性能方面提供更好的价值。对于保证实现完整的10 Gbps速度或SFP+支持，雷电适配器仍然是更优越的选择，尽管价格更高。

---

## 4. 朝日 Linux 进展 Linux 7.0

**原文标题**: Asahi Linux Progress Linux 7.0

**原文链接**: [https://asahilinux.org/2026/04/progress-report-7-0/](https://asahilinux.org/2026/04/progress-report-7-0/)

Asahi Linux 在适逢 Linux 7.0 发布之际，发布了一份全面的进展报告，详细介绍了在多个方面取得的重大进展。

沉寂两年后更新至 0.8.0 版本的 Asahi 安装器，现在通过 GitHub 工作流实现了自动化构建过程。这解决了此前因设备树（Devicetrees）过时，导致较新内核无法与纯 UEFI 安装兼容的问题。新的安装器还包括对 Mac Pro 的支持，以及一个精简的固件更新模式，这对未来的升级至关重要。

苹果的 True Tone（环境光传感器 - ALS）支持已通过始终在线处理器（AOP）实现。至关重要的是，安装器现在可以自动从 macOS 中获取并更新必要的校准固件，从而简化了未来的固件管理，并避免了手动修改 EFI 分区。

功耗效率方面取得了重大改进，针对电源管理处理器（PMP）的新驱动，将14英寸M1 Pro MacBook Pro等设备的空闲功耗降低了约20%（0.5W）。将PMP支持扩展到基础M1 SoC的工作正在进行中。

得益于内核对博通（Broadcom）厂商专用主机控制器接口（HCI）扩展的新支持，蓝牙音频中断现已基本消除。这些扩展能更有效地管理 Wi-Fi 和蓝牙共存，优先处理音频流。

最后，开发者发现了适用于外部和内部 ProMotion 显示器的可变刷新率（VRR）功能。尽管显示控制器要求进行模式切换（modeset）才能转换 VRR 状态，这阻止了其完全、标准地暴露给用户空间和合成器，但用户可以通过内核模块参数强制启用它。这一限制正在调查中，特别是在允许此类转换的 HDMI 连接上。

---

## 5. 特朗普解散国家科学基金会监督委员会

**原文标题**: Trump fires NSF's oversight board

**原文链接**: [https://www.science.org/content/article/trump-fires-nsf-s-oversight-board](https://www.science.org/content/article/trump-fires-nsf-s-oversight-board)

2020年11月中旬，特朗普政府史无前例地解雇了国家科学委员会（NSB）的全部24名成员。国家科学委员会（NSB）是国家科学基金会（NSF）的管理机构，负责制定其政策，批准重大研究计划，并就科学和工程事务向总统和国会提供建议。

这个由两党组成的委员会的成员通常任期为交错的六年，他们接到的信函称，他们的解职是“由总统酌情决定”。这次大规模解雇发生在特朗普总统输掉大选后的跛脚鸭时期，招致了科学界的强烈谴责。批评者认为这是一次出于政治动机的行动，破坏了国家科学委员会（NSB）的无党派独立性，并有可能使科学监督政治化。人们对国家科学基金会（NSF）关键职能的中断以及为未来政府设定的先例表示担忧。即将上任的拜登政府面临着立即任命一个全新委员会的任务。

---

## 6. USB 速查表 (2022)

**原文标题**: USB Cheat Sheet (2022)

**原文链接**: [https://fabiensanglard.net/usbcheat/index.html](https://fabiensanglard.net/usbcheat/index.html)

这份USB速查表旨在澄清通用串行总线标准中那些常常令人困惑的术语和规范，这些困惑源于作者个人对误解术语的经历。

该文档追溯了USB的演进，详细说明了“营销名称”及其“也称为”的命名。它展示了从USB 1.1（全速，12 Mbps）和USB 2.0（高速，480 Mbps）到显著更快的SuperSpeed USB变体的进展。例如，“SuperSpeed USB 5Gbps”涵盖了USB 3.0、USB 3.1 Gen 1和USB 3.2 Gen 1，它们都以5000 Mbps（625 MiB/s）运行。随后的版本，如“SuperSpeedPlus USB 10Gbps”（USB 3.1/3.2 Gen 2）和“SuperSpeedPlus USB 20Gbps”（USB 3.2 Gen 2x2），分别将这些速度提高了一倍和四倍，最终达到USB4 40Gbps。

“Gen命名约定”（USB Gen A x B）解释了“A”指代代数，“B”指代所使用的通道数。多通道系统，如Gen 2x2，通过绑定多个通道以实现更高的总信号速度，尽管实际传输速率会因编码开销（例如，8b/10b或128b/132b）而降低。

线缆的线芯数量随着速度的增加而增加：USB 1.1/2.0为4根线，早期SuperSpeed为8根，最高速度（20Gbps和40Gbps）为12根，以支持多数据通道。只有USB Type-C连接器具有足够的引脚（12根线）来支持双通道、电源协商（CC1/CC2）和替代模式。

充电能力也得到了大幅提升，从USB 2.0的2.5W到USB 3.0/3.1的4.5W。借助USB-C和供电（PD）技术，功率输出从15W（非PD）飙升至100W（PD 1/2），使用PD 3.1扩展功率范围（EPR）时最高可达240W。该速查表最后附有1996年至2019年USB规范发布的时间线。

---

## 7. 火狐集成 Brave 广告拦截引擎

**原文标题**: Firefox Has Integrated Brave's Adblock Engine

**原文链接**: [https://itsfoss.com/news/firefox-ships-brave-adblock-engine/](https://itsfoss.com/news/firefox-ships-brave-adblock-engine/)

Firefox 149 于三月发布，悄然集成了 `adblock-rust`，这是 Brave 开源的、基于 Rust 的广告和追踪器拦截引擎。这一重要新增功能在很大程度上未被察觉，直到 Brave 的隐私与安全副总裁 Shivan Kaul Sahib 在一篇博客文章中强调了它，因为它并未被包含在发布说明中。

`adblock-rust` 引擎采用 MPL-2.0 许可证，为 Brave 的原生内容拦截器提供支持。它专为网络请求拦截和美化过滤而设计，并支持与 uBlock Origin 兼容的过滤列表语法。此次集成通过 Bugzilla Bug 2013888 实现，该 Bug 题为“添加一个原型富内容拦截引擎”，并且默认禁用，没有用户界面或预设的过滤列表。Waterfox，一个流行的 Firefox 分支，也采用了此引擎，其实现方式基于 Firefox 的集成。

要测试此实验性功能，建议用户使用一个临时 Firefox 安装。首先，禁用测试网站的增强型追踪保护。接着，在 `about:config` 中，将 `privacy.trackingprotection.content.protection.enabled` 设置为“true”。接下来，编辑 `privacy.trackingprotection.content.protection.test_list_urls` 以添加过滤列表，例如 `https://easylist.to/easylist/easylist.txt|https://easylist.to/easylist/easyprivacy.txt`。访问包含广告的网站时，该引擎应该会拦截广告内容，尽管广告位可能仍会显示。

---

## 8. Why has there been so little progress on Alzheimer's disease?

**原文标题**: Why has there been so little progress on Alzheimer's disease?

**原文链接**: [https://freakonomics.com/podcast/why-has-there-been-so-little-progress-on-alzheimers-disease/](https://freakonomics.com/podcast/why-has-there-been-so-little-progress-on-alzheimers-disease/)

生成摘要时出错

---

## 9. Replace IBM Quantum back end with /dev/urandom

**原文标题**: Replace IBM Quantum back end with /dev/urandom

**原文链接**: [https://github.com/yuvadm/quantumslop/blob/25ad2e76ae58baa96f6219742459407db9dd17f5/URANDOM_DEMO.md](https://github.com/yuvadm/quantumslop/blob/25ad2e76ae58baa96f6219742459407db9dd17f5/URANDOM_DEMO.md)

生成摘要时出错

---

## 10. Using coding assistance tools to revive projects you never were going to finish

**原文标题**: Using coding assistance tools to revive projects you never were going to finish

**原文链接**: [https://blog.matthewbrunelle.com/its-ok-to-use-coding-assistance-tools-to-revive-the-projects-you-never-were-going-to-finish/](https://blog.matthewbrunelle.com/its-ok-to-use-coding-assistance-tools-to-revive-the-projects-you-never-were-going-to-finish/)

生成摘要时出错

---

## 11. My audio interface has SSH enabled by default

**原文标题**: My audio interface has SSH enabled by default

**原文链接**: [https://hhh.hn/rodecaster-duo-fw/](https://hhh.hn/rodecaster-duo-fw/)

生成摘要时出错

---

## 12. EU Age Control: The trojan horse for digital IDs

**原文标题**: EU Age Control: The trojan horse for digital IDs

**原文链接**: [https://juraj.bednar.io/en/blog-en/2026/04/17/eu-age-control-the-trojan-horse-for-digital-ids/](https://juraj.bednar.io/en/blog-en/2026/04/17/eu-age-control-the-trojan-horse-for-digital-ids/)

生成摘要时出错

---

## 13. Plain text has been around for decades and it’s here to stay

**原文标题**: Plain text has been around for decades and it’s here to stay

**原文链接**: [https://unsung.aresluna.org/plain-text-has-been-around-for-decades-and-its-here-to-stay/](https://unsung.aresluna.org/plain-text-has-been-around-for-decades-and-its-here-to-stay/)

生成摘要时出错

---

## 14. The Classic American Diner

**原文标题**: The Classic American Diner

**原文链接**: [https://blogs.loc.gov/picturethis/2026/04/the-classic-american-diner/](https://blogs.loc.gov/picturethis/2026/04/the-classic-american-diner/)

生成摘要时出错

---

## 15. The AI industry is discovering that the public hates it

**原文标题**: The AI industry is discovering that the public hates it

**原文链接**: [https://newrepublic.com/article/209163/ai-industry-discovering-public-backlash](https://newrepublic.com/article/209163/ai-industry-discovering-public-backlash)

生成摘要时出错

---

## 16. GoDaddy Gave a Domain to a Stranger Without Any Documentation

**原文标题**: GoDaddy Gave a Domain to a Stranger Without Any Documentation

**原文链接**: [https://anchor.host/godaddy-gave-a-domain-to-a-stranger-without-any-documentation/](https://anchor.host/godaddy-gave-a-domain-to-a-stranger-without-any-documentation/)

生成摘要时出错

---

## 17. Statecharts: hierarchical state machines

**原文标题**: Statecharts: hierarchical state machines

**原文链接**: [https://statecharts.dev/](https://statecharts.dev/)

生成摘要时出错

---

## 18. Show HN: A Karpathy-style LLM wiki your agents maintain (Markdown and Git)

**原文标题**: Show HN: A Karpathy-style LLM wiki your agents maintain (Markdown and Git)

**原文链接**: [https://github.com/nex-crm/wuphf](https://github.com/nex-crm/wuphf)

生成摘要时出错

---

## 19. Niri 26.04: Scrollable-tiling Wayland compositor

**原文标题**: Niri 26.04: Scrollable-tiling Wayland compositor

**原文链接**: [https://github.com/niri-wm/niri/releases/tag/v26.04](https://github.com/niri-wm/niri/releases/tag/v26.04)

生成摘要时出错

---

## 20. Google to invest up to $40B in Anthropic in cash and compute

**原文标题**: Google to invest up to $40B in Anthropic in cash and compute

**原文链接**: [https://techcrunch.com/2026/04/24/google-to-invest-up-to-40b-in-anthropic-in-cash-and-compute/](https://techcrunch.com/2026/04/24/google-to-invest-up-to-40b-in-anthropic-in-cash-and-compute/)

生成摘要时出错

---

## 21. Turbo Vision 2.0 – a modern port

**原文标题**: Turbo Vision 2.0 – a modern port

**原文链接**: [https://github.com/magiblot/tvision](https://github.com/magiblot/tvision)

生成摘要时出错

---

## 22. GitHub unwanted UX change: issue links now open in a popup

**原文标题**: GitHub unwanted UX change: issue links now open in a popup

**原文链接**: [https://github.com/orgs/community/discussions/192666](https://github.com/orgs/community/discussions/192666)

生成摘要时出错

---

## 23. Simulacrum of Knowledge Work

**原文标题**: Simulacrum of Knowledge Work

**原文链接**: [https://blog.happyfellow.dev/simulacrum-of-knowledge-work/](https://blog.happyfellow.dev/simulacrum-of-knowledge-work/)

生成摘要时出错

---

## 24. Martin Galway's music source files from 1980's Commodore 64 games

**原文标题**: Martin Galway's music source files from 1980's Commodore 64 games

**原文链接**: [https://github.com/MartinGalway/C64_music](https://github.com/MartinGalway/C64_music)

生成摘要时出错

---

## 25. Show HN: I've built a nice home server OS

**原文标题**: Show HN: I've built a nice home server OS

**原文链接**: [https://lightwhale.asklandd.dk/](https://lightwhale.asklandd.dk/)

生成摘要时出错

---

## 26. Open source memory layer so any AI agent can do what Claude.ai and ChatGPT do

**原文标题**: Open source memory layer so any AI agent can do what Claude.ai and ChatGPT do

**原文链接**: [https://alash3al.github.io/stash?_v01](https://alash3al.github.io/stash?_v01)

生成摘要时出错

---

## 27. Why SWE-bench Verified no longer measures frontier coding capabilities

**原文标题**: Why SWE-bench Verified no longer measures frontier coding capabilities

**原文链接**: [https://openai.com/index/why-we-no-longer-evaluate-swe-bench-verified/](https://openai.com/index/why-we-no-longer-evaluate-swe-bench-verified/)

生成摘要时出错

---

## 28. Discret 11, the French TV encryption of the 80s (2020)

**原文标题**: Discret 11, the French TV encryption of the 80s (2020)

**原文链接**: [https://fabiensanglard.net/discret11/](https://fabiensanglard.net/discret11/)

生成摘要时出错

---

## 29. Do I belong in tech anymore?

**原文标题**: Do I belong in tech anymore?

**原文链接**: [https://ky.fyi/posts/ai-burnout](https://ky.fyi/posts/ai-burnout)

生成摘要时出错

---

## 30. Europe to burned American scientists: We'll take you in (2025)

**原文标题**: Europe to burned American scientists: We'll take you in (2025)

**原文链接**: [https://www.politico.eu/article/europe-exploit-dunald-trump-brain-drain-academic-research-progressive-institutions/](https://www.politico.eu/article/europe-exploit-dunald-trump-brain-drain-academic-research-progressive-institutions/)

生成摘要时出错

---

## 31. Trump Fires the National Science Board

**原文标题**: Trump Fires the National Science Board

**原文链接**: [https://www.theverge.com/science/918769/trump-fires-the-entire-national-science-board](https://www.theverge.com/science/918769/trump-fires-the-entire-national-science-board)

生成摘要时出错

---

## 32. AI agents that argue with each other to improve decisions

**原文标题**: AI agents that argue with each other to improve decisions

**原文链接**: [https://github.com/rockcat/HATS](https://github.com/rockcat/HATS)

生成摘要时出错

---

## 33. California Coastal Community Must Reject CBP's AI-Powered Surveillance Tower

**原文标题**: California Coastal Community Must Reject CBP's AI-Powered Surveillance Tower

**原文链接**: [https://www.eff.org/deeplinks/2026/04/california-coastal-community-must-reject-cbps-ai-powered-surveillance-tower](https://www.eff.org/deeplinks/2026/04/california-coastal-community-must-reject-cbps-ai-powered-surveillance-tower)

生成摘要时出错

---

## 34. Show HN: HNswered – watches for replies to your Hacker News posts and comments

**原文标题**: Show HN: HNswered – watches for replies to your Hacker News posts and comments

**原文链接**: [https://github.com/adam-s/HNswered](https://github.com/adam-s/HNswered)

生成摘要时出错

---

## 35. Trump evacuated from White House Correspondents' Dinner after shots fired

**原文标题**: Trump evacuated from White House Correspondents' Dinner after shots fired

**原文链接**: [https://www.abc.net.au/news/2026-04-26/trump-evacuated-white-house-correspondents-dinner-shots-fired/106607720](https://www.abc.net.au/news/2026-04-26/trump-evacuated-white-house-correspondents-dinner-shots-fired/106607720)

生成摘要时出错

---

## 36. The Stanford Freshmen Who Want to Rule the World

**原文标题**: The Stanford Freshmen Who Want to Rule the World

**原文链接**: [https://www.theatlantic.com/ideas/2026/04/stanford-students-power/686920/](https://www.theatlantic.com/ideas/2026/04/stanford-students-power/686920/)

生成摘要时出错

---

## 37. Tip: Web requests should not be measured in Hz [Hertz]

**原文标题**: Tip: Web requests should not be measured in Hz [Hertz]

**原文链接**: [https://mastodon.catgirl.cloud/@sophie/116467789133733136](https://mastodon.catgirl.cloud/@sophie/116467789133733136)

生成摘要时出错

---

## 38. Godot 4.7 Beta with HDR Output, Ray-Tracing Improvements and Editor Enhancements

**原文标题**: Godot 4.7 Beta with HDR Output, Ray-Tracing Improvements and Editor Enhancements

**原文链接**: [https://www.phoronix.com/news/Godot-4.7-Beta](https://www.phoronix.com/news/Godot-4.7-Beta)

生成摘要时出错

---

## 39. Plants can sense the sound of rain, a new study finds

**原文标题**: Plants can sense the sound of rain, a new study finds

**原文链接**: [https://news.mit.edu/2026/plants-can-sense-sound-rain-new-study-finds-0422](https://news.mit.edu/2026/plants-can-sense-sound-rain-new-study-finds-0422)

生成摘要时出错

---

## 40. French tax official sold crypto investors' addresses: kidnappings followed

**原文标题**: French tax official sold crypto investors' addresses: kidnappings followed

**原文链接**: [https://twitter.com/MarioNawfal/status/2047773069607854512](https://twitter.com/MarioNawfal/status/2047773069607854512)

生成摘要时出错

---

## 41. I have officially retired from Emacs

**原文标题**: I have officially retired from Emacs

**原文链接**: [https://nullprogram.com/blog/2026/04/26/](https://nullprogram.com/blog/2026/04/26/)

生成摘要时出错

---

## 42. Google Search to classify 'back button hijacking' as spam

**原文标题**: Google Search to classify 'back button hijacking' as spam

**原文链接**: [https://9to5google.com/2026/04/13/google-search-back-button-hijacking/](https://9to5google.com/2026/04/13/google-search-back-button-hijacking/)

生成摘要时出错

---

## 43. Is Italy the new tax haven for the global rich?

**原文标题**: Is Italy the new tax haven for the global rich?

**原文链接**: [https://www.bbc.com/worklife/article/20260421-is-italy-the-new-tax-haven-for-the-global-rich](https://www.bbc.com/worklife/article/20260421-is-italy-the-new-tax-haven-for-the-global-rich)

生成摘要时出错

---

## 44. GPT-5.5 is generally available for GitHub Copilot

**原文标题**: GPT-5.5 is generally available for GitHub Copilot

**原文链接**: [https://github.blog/changelog/2026-04-24-gpt-5-5-is-generally-available-for-github-copilot/](https://github.blog/changelog/2026-04-24-gpt-5-5-is-generally-available-for-github-copilot/)

生成摘要时出错

---

## 45. TIPSv2: Advancing Vision-Language Pretraining with Enhanced Patch-Text Alignment

**原文标题**: TIPSv2: Advancing Vision-Language Pretraining with Enhanced Patch-Text Alignment

**原文链接**: [https://gdm-tipsv2.github.io/](https://gdm-tipsv2.github.io/)

生成摘要时出错

---

## 46. Microsoft Reportedly Looking at Rebasing Azure Linux on Fedora

**原文标题**: Microsoft Reportedly Looking at Rebasing Azure Linux on Fedora

**原文链接**: [https://www.phoronix.com/news/MS-Azure-Linux-Fedora-Based](https://www.phoronix.com/news/MS-Azure-Linux-Fedora-Based)

生成摘要时出错

---

## 47. US is making Europe pay dearly for its half-hearted electrification

**原文标题**: US is making Europe pay dearly for its half-hearted electrification

**原文链接**: [https://www.programmablemutter.com/cp/195461224](https://www.programmablemutter.com/cp/195461224)

生成摘要时出错

---

## 48. Does internet advertising work? (2020)

**原文标题**: Does internet advertising work? (2020)

**原文链接**: [https://freakonomics.com/podcast/does-advertising-actually-work-part-2-digital-ep-441/](https://freakonomics.com/podcast/does-advertising-actually-work-part-2-digital-ep-441/)

生成摘要时出错

---

## 49. My Homemade PBX (2002)

**原文标题**: My Homemade PBX (2002)

**原文链接**: [https://wandel.ca/homepage/pbx.html](https://wandel.ca/homepage/pbx.html)

生成摘要时出错

---

## 50. FSF Position on "Ethical" AI

**原文标题**: FSF Position on "Ethical" AI

**原文链接**: [https://www.fsf.org/blogs/licensing/rail-are-nonfree-and-unethical](https://www.fsf.org/blogs/licensing/rail-are-nonfree-and-unethical)

生成摘要时出错

---

## 51. Eurosky.social Account

**原文标题**: Eurosky.social Account

**原文链接**: [https://eurosky.tech/accounts/](https://eurosky.tech/accounts/)

生成摘要时出错

---

## 52. The Knight Programming Language

**原文标题**: The Knight Programming Language

**原文链接**: [https://github.com/knight-lang/knight-lang/tree/master](https://github.com/knight-lang/knight-lang/tree/master)

生成摘要时出错

---

## 53. Show HN: Browse GitHub repos in Emacs without cloning

**原文标题**: Show HN: Browse GitHub repos in Emacs without cloning

**原文链接**: [https://github.com/agzam/remoto.el](https://github.com/agzam/remoto.el)

生成摘要时出错

---

## 54. The U.K. Smoking Ban Is Illiberal

**原文标题**: The U.K. Smoking Ban Is Illiberal

**原文链接**: [https://www.theatlantic.com/ideas/2026/04/case-against-uk-smoking-ban/686949/](https://www.theatlantic.com/ideas/2026/04/case-against-uk-smoking-ban/686949/)

生成摘要时出错

---

## 55. Nicholas Carlini – Black-hat LLMs [video]

**原文标题**: Nicholas Carlini – Black-hat LLMs [video]

**原文链接**: [https://www.youtube.com/watch?v=1sd26pWhfmg](https://www.youtube.com/watch?v=1sd26pWhfmg)

生成摘要时出错

---

## 56. YC as a Service

**原文标题**: YC as a Service

**原文链接**: [https://ycaas.lol](https://ycaas.lol)

生成摘要时出错

---

## 57. MenteDB – open-source memory database for AI agents (Rust)

**原文标题**: MenteDB – open-source memory database for AI agents (Rust)

**原文链接**: [https://github.com/nambok/mentedb](https://github.com/nambok/mentedb)

生成摘要时出错

---

## 58. Show HN: I remade my blog into a Windows 3.1 environment

**原文标题**: Show HN: I remade my blog into a Windows 3.1 environment

**原文链接**: [https://passo.uno/](https://passo.uno/)

生成摘要时出错

---

## 59. Trump ousts National Science Board members

**原文标题**: Trump ousts National Science Board members

**原文链接**: [https://www.washingtonpost.com/science/2026/04/25/national-science-board-members-dismissed/](https://www.washingtonpost.com/science/2026/04/25/national-science-board-members-dismissed/)

生成摘要时出错

---

