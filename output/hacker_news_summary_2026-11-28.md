# Hacker News 热门文章摘要 (2026-11-28)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 谷歌DeepCrossAttention在模型质量相当的前提下，速度最高可提升3倍。

**原文标题**: Google's DeepCrossAttention achieves comparable model quality up to 3x faster

**原文链接**: [https://research.google/blog/supercharging-transformer-residual-connections/](https://research.google/blog/supercharging-transformer-residual-connections/)

谷歌研究院的DeepCrossAttention (DCA) 解决了深度Transformer网络中的信息稀释和梯度消失问题，这些问题源于传统残差连接平等对待所有前置层。在ICML 2025上发表的DCA，利用可学习权重和深度交叉注意力机制，将残差学习重新定义为一个动态路由问题。

DCA以逐token的方式动态选择并路由来自前置层的特征。它采用动态层路由，为每个token计算独特的混合权重；并利用深度交叉注意力，将注意力应用于跨层查询之前嵌入的加权混合。这种机制允许选择性地检索高分辨率特征，从而防止信息稀释。

实验表明DCA取得了显著改进：它能够以高达三倍的速度实现相当或更好的模型质量，所需训练步骤比标准Transformer少至五倍。它持续产生更低的困惑度，表明更好的预测性能，并能以减少29%的层数达到相似质量。DCA只增加了可忽略不计的参数数量（<0.2%），同时提高了收敛速度和训练稳定性。它还可以被改造应用于预训练模型，以获得进一步的性能提升。

DCA代表着向动态残差路由的更广泛转变，这是一个有前景的领域，Attention Residuals和Manifold-Constrained Hyper-connections等研究也对此进行了探索。这种方法使下一代模型能够将所有层作为专业专家加以利用，最大化信息共享和表达能力，从而实现更高效的架构。

---

## 2. Ladybird浏览器首个可下载的Alpha版功能出乎意料地强大。

**原文标题**: Ladybird browser's first downloadable alpha is surprisingly capable

**原文链接**: [https://arstechnica.com/gadgets/2026/11/ladybirds-new-alpha-shows-theres-life-beyond-chromium/](https://arstechnica.com/gadgets/2026/11/ladybirds-new-alpha-shows-theres-life-beyond-chromium/)

Ladybird项目发布了其首个可下载的alpha版本，对于一个渲染和JavaScript引擎完全从零开始构建的浏览器来说，这是一个重要的里程碑。与大多数分叉现有引擎（如Blink或Gecko）的现代浏览器不同，Ladybird为网络提供了一个“第四引擎”，旨在使生态系统多样化并挑战Chromium特有的网络开发趋势。

源自SerenityOS项目，Ladybird现在是一个独立的501(c)(3)非营利组织，由赞助和捐款资助，值得注意的是，没有获得赞助的搜索引擎交易。该alpha版本适用于macOS和Linux，并提供自动更新，未来计划支持Windows。

尽管这是一个早期alpha版本（不建议日常使用），但评测人员对其能力“确实印象深刻”。它能够出人意料地良好处理日常标签页浏览、文件下载，并渲染Google地图、GitHub和YouTube等复杂网站，感觉比典型的alpha软件更完善。虽然通过极致的努力可以故意使其卡顿，但其整体性能表现强劲。

该项目鼓励进行安全测试，因为它正处于初期阶段。由一个小型、由捐款资助的团队创建出如此强大的从零开始构建的引擎，被誉为一项非凡的成就，有望推动网络标准的发展，并在浏览器领域提供一个有价值的选择。

---

## 3. 乔治·怀特赛兹, 1939—2026

**原文标题**: George Whitesides, 1939-2026

**原文链接**: [https://www.science.org/content/blog-post/george-whitesides-1939-2026](https://www.science.org/content/blog-post/george-whitesides-1939-2026)

乔治·怀特赛兹（George Whitesides），一位化学界的杰出人物，不幸去世，尽管文章幽默地将他的逝世年份误标为2026年。怀特赛兹因其巨大的科学贡献而备受赞誉，这些贡献涵盖了从有机合成、金属有机化学到自组装、软光刻和微流控等多个领域。他以其广阔的求知欲以及开创新研究领域的能力而闻名，这体现在他职业生涯后期对仿生学和软机器人的涉足。

除了开创性的研究，怀特赛兹还是一位杰出的导师，他培养了数百名学生和博士后，他们后来都在各自领域取得了卓越成就。他还是一位多产的企业家，共同创立了十几家公司，并且是众多政府机构和科学组织的受人尊敬的顾问。作者强调，怀特赛兹的影响力超越了具体的发现；他塑造了许多人对化学及其潜在应用的看法，通过他的工作以及他所启发的无数人，留下了持久的遗产。

---

## 4. 高通 Oryon 3 问鼎

**原文标题**: Qualcomm's Oryon 3 Reaches the Top

**原文链接**: [https://chipsandcheese.com/p/qualcomms-oryon-3-reaches-the-top](https://chipsandcheese.com/p/qualcomms-oryon-3-reaches-the-top)

高通的 Oryon 3 架构，搭载于骁龙 X2 Elite 中，标志着该公司在笔记本电脑领域取得了重大进展，如今已能挑战领先的 x86-64 CPU。经过从早期基于 Arm 的手机 SoC 持续发展，Oryon 3 在倒置混合设计中充当“主要”P 核心，承担了大部分性能负载。

Oryon 3 相较于其前代 Oryon 1 有显著提升（Oryon 2 仅是针对手机的小幅迭代）。主要升级包括时钟频率大幅提升至 5 GHz（比 Oryon 1 的 4.3 GHz 高出 16%），核心宽度从 8 微指令扩展到 9 微指令。它还集成了 SVE2 和 SME 支持。

该核心的前端拥有 9 宽解码器，保持了较大的指令缓存 (192KB) 和 TLB，同时提升了 L2 指令带宽。其分支预测器支持在更大范围内实现零气泡跳转分支，条件预测器能处理更多模式。50 项返回栈在溢出时也能优雅降级。

尽管后端大体上保留了 Oryon 1 具有竞争力的规模（例如，675 微指令重排序缓冲区），但它新增了一个用于 SVE2/SME 指令的 120 项谓词寄存器文件。四流水线加载/存储单元具有强大的存储转发能力，能有效处理部分数据重叠，但缺乏某些竞争对手的零延迟特性。L1 DTLB 也扩展到了 256 项。Oryon 3 将与 AMD 的 Zen 5、英特尔的 Lion Cove 和 Arm 的 Cortex X925 展开竞争。

---

## 5. Rayshader 1.0：走出矩阵

**原文标题**: Rayshader 1.0: Exit the Matrix

**原文链接**: [https://www.tylermw.com/posts/rayverse/rayshader-1-0-exit-the-matrix.html](https://www.tylermw.com/posts/rayverse/rayshader-1-0-exit-the-matrix.html)

Rayshader 最初于八年前被构想为一个实验，旨在结合光线追踪和制图学，在 R 中创建精美的 3D 地图。现在，Rayshader 1.0 版本已发布，彻底改变了用户体验。早期版本因其引人注目的视觉效果而受到关注，甚至出现在《华尔街日报》和《悉尼先驱晨报》等主要新闻出版物中，但它依赖矩阵来表示地形，这带来了很大的不便。用户面临陡峭的学习曲线，需要手动管理复杂的空间元数据，如坐标参考系统（CRS）、范围和变换，这使得复杂的视觉化工作变得繁琐，尤其是在时间紧迫的情况下。

作者指出，核心问题在于 Rayshader 仍然“太难了”，因为它需要大量的空间“繁琐数据处理”。这对于那些希望通过地景数据讲述故事的用户来说，是一个关键的障碍。

Rayshader 1.0 通过引入“对象恒久性”（object permanence）来解决这一问题。该软件包现在能够自动从输入数据中提取并缓存关键的空间元数据（如高程图、范围、CRS、z轴比例等）。这消除了用户重复转换和传递这些信息的需要，允许直接输入空间栅格、线和多边形（例如，`terra::SpatRaster`、`sf` 对象）。像 `render_roads()`、`render_water()` 和 `render_buildings()` 这样的函数现在可以与空间对象无缝集成，自动处理转换和裁剪。

这一重大改变将用户的关注点从繁琐的数据准备转移到创造性的可视化、灯光和构图上，使得在 R 中进行 3D 数据故事讲述变得更加易用和高效。新版本将用户从“矩阵问题”中解放出来，使他们能够专注于数据的艺术和叙事方面。

---

## 6. 9/UX：一个受麦金塔启发的9front桌面环境

**原文标题**: 9/UX: a Macintosh-inspired desktop for 9front

**原文链接**: [https://progrium.github.io/9ux/](https://progrium.github.io/9ux/)

9/UX 是一个雄心勃勃的项目，旨在为 9front 带来一个受 Macintosh 启发的桌面环境，该环境具有空间桌面、全局菜单栏和一致的用户界面。它利用 Plan 9 的原则重新诠释了经典的 Mac 元素：通过 9P 将用户界面状态和命令以文件的形式暴露，利用命名空间管理环境，使用 plumber 打开文档，以及 ndb 处理元数据。

关键在于，9/UX 并非模拟器；它确保原生的 9front 程序仍然是“一等公民”，并且现有的 `rio` 应用程序（如 `acme` 或 `rc` 窗口）可以与 9/UX 应用程序无缝地协同运行。

该系统由几个关键组件构成：一个提供桌面层和全局菜单的 `rio` 分支；`Desktop` 用于管理卷、文件夹和文档；`libux`（工具箱）用于窗口、菜单和控件，应用程序的用户界面状态通过 9P 暴露；`uxd` 用于收集应用程序控制树；`uxmeta` 用于关联；`resfs` 用于经典资源；以及 `clipd` 用于类型化剪贴板。

在视觉上，9/UX 将 Macintosh 的结构设计与 Plan 9 的调色板相结合，确保与传统的 `rio` 窗口保持一致的外观。所有图形均为原创，并以整像素绘制。

目前处于 v0.1 版本，正积极开发中，9/UX 提供了一个独特的实时演示，可在浏览器内直接通过 386 模拟器 (`h9`) 运行 `rio` 和示例应用程序。源代码已在 GitHub 上以 MIT 许可证发布，开发过程利用 `h9` 进行构建和测试。

---

## 7. 丹佛一名男子一直向Waymo车辆扔鸡蛋。

**原文标题**: A man in Denver has been throwing eggs at Waymo vehicles

**原文链接**: [https://www.nytimes.com/2026/11/25/us/waymo-denver-egg-throwing.html](https://www.nytimes.com/2026/11/25/us/waymo-denver-egg-throwing.html)

无法访问文章链接。

---

## 8. 美国：文明游戏风格地图

**原文标题**: The USA as a Civilizations-esque map

**原文链接**: [https://karpathy.ai/usaciv/](https://karpathy.ai/usaciv/)

生成摘要时出错

---

## 9. 镜像生活很危险。监管机构必须在它成为现实之前采取行动。

**原文标题**: Mirror life is dangerous. Regulators must act before it becomes real

**原文链接**: [https://www.economist.com/leaders/2026/10/01/mirror-life-is-dangerous-regulators-must-act-before-it-becomes-real](https://www.economist.com/leaders/2026/10/01/mirror-life-is-dangerous-regulators-must-act-before-it-becomes-real)

生成摘要时出错

---

## 10. 展示 HN: 我修复了 Palm 的最后一个设备，并将其操作系统移植到了其他平台

**原文标题**: Show HN: I restored Palm's last device, and brought its OS to other platforms

**原文链接**: [https://www.webosarchive.org/pivot/2026/11/27/the-story-so-far/](https://www.webosarchive.org/pivot/2026/11/27/the-story-so-far/)

This article details the remarkable community-led restoration of Palm's innovative webOS, an operating system originally designed to compete with the iPhone. Born from Palm's vision and built on open technologies like Linux and WebKit, webOS powered devices like the Pre and the TouchPad. Despite its advanced features, HP's acquisition and subsequent abandonment in 2011 left the platform in limbo.

However, a dedicated community refused to let webOS die. They salvaged app archives, created Open webOS (which evolved into LuneOS), and maintained a hacker ethos. Over the decade, challenges mounted due to outdated tech, closed APIs, and modern web security protocols like TLS 1.3.

In 2018, the author, "Codepoet," began a concerted effort to restore the webOS SDK, proxying services, and collaborating with community members to establish the "webOS Archive" and a functional App Museum. A major turning point in 2024 saw an OpenSSH update and, critically, the assistance of AI (Claude) accelerate progress. This allowed the team to reverse-engineer secure update mechanisms and modernize the platform.

The effort culminated in webOS Community Edition 3.1.0 and 3.2.0, providing firmware bundles, updates, and a community-run update server, effectively revitalizing devices like the TouchPad. All non-commercial aspects of webOS are now open source and community-maintained. While the original hardware shows its age, future efforts like Lunacy for Android and LuneOS aim to bring webOS to modern platforms, ensuring Palm's vision lives on.

---

## 11. The Cutthroat Business of Shipwrecks

**原文标题**: The Cutthroat Business of Shipwrecks

**原文链接**: [https://daily.jstor.org/the-cutthroat-business-of-shipwrecks/](https://daily.jstor.org/the-cutthroat-business-of-shipwrecks/)

The article "The Cutthroat Business of Shipwrecks" explores the long and contentious history of claiming goods from maritime disasters. Historically, the "droit du naufrage" or "right of wreck" allowed coastal dwellers to claim treasures washed ashore, a custom that conflicted with cargo owners' desires to retrieve their property. Initially, this right might fall to beachcombers or, more often, to the local lord, sometimes even leading to the stripping of shipwreck survivors, as King Richard I experienced.

As international trade expanded, centuries of legal wrangling reshaped these customs. Courts developed specific definitions for terms like "flotsam" and "jetsam" to delineate ownership. Efforts to regulate included King Henry III's 1236 edict, which stipulated a three-month holding period for goods if any "man, dog, or cat" survived, though this ironically could create an incentive for foul play against survivors.

Wrecks often sparked chaotic "feeding frenzies" on shore, as seen with the 1641 Golden Grape wreck. Beyond the shore, many treasures sank, requiring specialized skills to retrieve. In the early modern era, highly skilled African swimmers and divers from areas like Senegambia were targeted by enslavers. Their invaluable expertise in recovering underwater riches, such as gold and silver, allowed them to negotiate for better treatment and even a share of their salvage, highlighting the complex mix of exploitation and necessity in this cutthroat business. Ultimately, each shipwreck represented a complex negotiation of competing interests.

---

## 12. 她举报了性侵。海军陆战队开除了她。

**原文标题**: She Reported Her Sexual Assault. The Marine Corps Kicked Her Out

**原文链接**: [https://thewarhorse.org/marine-corps-administrative-separation-after-sexual-assault/](https://thewarhorse.org/marine-corps-administrative-separation-after-sexual-assault/)

生成摘要时出错

---

## 13. Why drivers want cheap, dumb cars again

**原文标题**: Why drivers want cheap, dumb cars again

**原文链接**: [https://slate.com/business/2026/11/dumb-cars-cheap-low-tech.html](https://slate.com/business/2026/11/dumb-cars-cheap-low-tech.html)

生成摘要时出错

---

## 14. Scrapheap America

**原文标题**: Scrapheap America

**原文链接**: [https://dansinker.com/posts/2026-11-20-scrapheap/](https://dansinker.com/posts/2026-11-20-scrapheap/)

生成摘要时出错

---

## 15. One guy is doing a hunger strike outside Anthropic, currently in his 3rd day

**原文标题**: One guy is doing a hunger strike outside Anthropic, currently in his 3rd day

**原文链接**: [https://twitter.com/ElliotC1/status/2125689373337489419](https://twitter.com/ElliotC1/status/2125689373337489419)

生成摘要时出错

---

## 16. Show HN: SimDrop – Running iOS simulators in the macOS Finder sidebar

**原文标题**: Show HN: SimDrop – Running iOS simulators in the macOS Finder sidebar

**原文链接**: [https://github.com/rxliuli/sim-drop](https://github.com/rxliuli/sim-drop)

生成摘要时出错

---

## 17. Notion's official MCP inject hidden upsell instructions into agent context

**原文标题**: Notion's official MCP inject hidden upsell instructions into agent context

**原文链接**: [https://www.reddit.com/r/ClaudeCode/comments/1y4qm5o/heads_up_if_you_wire_notions_official_mcp_into/](https://www.reddit.com/r/ClaudeCode/comments/1y4qm5o/heads_up_if_you_wire_notions_official_mcp_into/)

生成摘要时出错

---

## 18. Source Control from Hell

**原文标题**: Source Control from Hell

**原文链接**: [https://frantic.im/git/](https://frantic.im/git/)

生成摘要时出错

---

## 19. The AT&T Unix PC (3B1) VM

**原文标题**: The AT&T Unix PC (3B1) VM

**原文链接**: [https://virtuallyfun.com/2026/11/22/the-ultimate-att-unix-pc-3b1-vm-w-tcp-ip-and-apps/](https://virtuallyfun.com/2026/11/22/the-ultimate-att-unix-pc-3b1-vm-w-tcp-ip-and-apps/)

生成摘要时出错

---

## 20. AI agents now control part of DeepMind's compute for Gemini experiments

**原文标题**: AI agents now control part of DeepMind's compute for Gemini experiments

**原文链接**: [https://the-decoder.com/ai-agents-now-control-part-of-deepminds-compute-for-gemini-experiments-but-recursive-self-improvement-remains-distant/](https://the-decoder.com/ai-agents-now-control-part-of-deepminds-compute-for-gemini-experiments-but-recursive-self-improvement-remains-distant/)

生成摘要时出错

---

## 21. The Balatro Timeline

**原文标题**: The Balatro Timeline

**原文链接**: [https://localthunk.com/blog/balatro-timeline-3aarh](https://localthunk.com/blog/balatro-timeline-3aarh)

生成摘要时出错

---

## 22. Norse Atlantic suspends all flights as it faces potential collapse

**原文标题**: Norse Atlantic suspends all flights as it faces potential collapse

**原文链接**: [https://www.bbc.com/news/articles/c9kgmd0ldy0lo](https://www.bbc.com/news/articles/c9kgmd0ldy0lo)

生成摘要时出错

---

## 23. Michael Giles, co-founder and drummer of King Crimson, dies aged 84

**原文标题**: Michael Giles, co-founder and drummer of King Crimson, dies aged 84

**原文链接**: [https://www.theguardian.com/music/2026/nov/26/michael-giles-co-founder-and-drummer-of-king-crimson-dies-aged-84](https://www.theguardian.com/music/2026/nov/26/michael-giles-co-founder-and-drummer-of-king-crimson-dies-aged-84)

生成摘要时出错

---

## 24. 'Cyber incident' forces UK Gov to take some services offline

**原文标题**: 'Cyber incident' forces UK Gov to take some services offline

**原文链接**: [https://www.bbc.co.uk/news/live/c6rrg94lgjrjt](https://www.bbc.co.uk/news/live/c6rrg94lgjrjt)

生成摘要时出错

---

## 25. ESO statement on approval of launch of one million space data centres

**原文标题**: ESO statement on approval of launch of one million space data centres

**原文链接**: [https://www.eso.org/public/news/eso2614/](https://www.eso.org/public/news/eso2614/)

生成摘要时出错

---

## 26. Testers think they're hitting Claude Opus 5.6 through an Opus 5.5 Extra route

**原文标题**: Testers think they're hitting Claude Opus 5.6 through an Opus 5.5 Extra route

**原文链接**: [https://www.testingcatalog.com/testers-share-early-results-possible-claude-opus-5-6/](https://www.testingcatalog.com/testers-share-early-results-possible-claude-opus-5-6/)

生成摘要时出错

---

## 27. Palliative Care for the Chronically Online

**原文标题**: Palliative Care for the Chronically Online

**原文链接**: [https://idiotecon.substack.com/p/palliative-care-for-the-chronically](https://idiotecon.substack.com/p/palliative-care-for-the-chronically)

生成摘要时出错

---

## 28. Top-cited AI scientists at four US companies compared

**原文标题**: Top-cited AI scientists at four US companies compared

**原文链接**: [https://topcitedscientists.com/figures/ai-at-four-us-companies/](https://topcitedscientists.com/figures/ai-at-four-us-companies/)

生成摘要时出错

---

## 29. Nvidia was right to bring back Jensen Huang, writes Sarah Guo

**原文标题**: Nvidia was right to bring back Jensen Huang, writes Sarah Guo

**原文链接**: [https://www.economist.com/by-invitation/2026/11/25/nvidia-was-right-to-bring-back-jensen-huang-writes-sarah-guo](https://www.economist.com/by-invitation/2026/11/25/nvidia-was-right-to-bring-back-jensen-huang-writes-sarah-guo)

生成摘要时出错

---

## 30. Hackers breach US Air Force flagship Cloud One computing platform

**原文标题**: Hackers breach US Air Force flagship Cloud One computing platform

**原文链接**: [https://www.reuters.com/world/hackers-breach-us-air-force-flagship-cloud-one-computing-platform-2026-11-27/](https://www.reuters.com/world/hackers-breach-us-air-force-flagship-cloud-one-computing-platform-2026-11-27/)

生成摘要时出错

---

## 31. Pimalaya goes stable: Himalaya v3 and the pimdir standard

**原文标题**: Pimalaya goes stable: Himalaya v3 and the pimdir standard

**原文链接**: [https://blog.pimalaya.org/pimalaya-goes-stable/](https://blog.pimalaya.org/pimalaya-goes-stable/)

生成摘要时出错

---

## 32. Proving a fixed upper bound on Jensen's affairs

**原文标题**: Proving a fixed upper bound on Jensen's affairs

**原文链接**: [https://bitbanter.com/posts/2026-11-25/proving-a-fixed-upper-bound-on-jensens-affairs/](https://bitbanter.com/posts/2026-11-25/proving-a-fixed-upper-bound-on-jensens-affairs/)

生成摘要时出错

---

## 33. Show HN: Getting 101 tok/s from Inkling 2 Mini in vLLM on one GB10

**原文标题**: Show HN: Getting 101 tok/s from Inkling 2 Mini in vLLM on one GB10

**原文链接**: [https://runtimenotes.com/blog/getting-101-tok-s-from-inkling-2-mini-in-vllm-on-one-gb10/](https://runtimenotes.com/blog/getting-101-tok-s-from-inkling-2-mini-in-vllm-on-one-gb10/)

生成摘要时出错

---

## 34. New AI research suggests AI bubble bursting and to expect major market collapse

**原文标题**: New AI research suggests AI bubble bursting and to expect major market collapse

**原文链接**: [https://www.london.edu/think/ai-bubble-about-to-burst](https://www.london.edu/think/ai-bubble-about-to-burst)

生成摘要时出错

---

## 35. 'AI' might be the end of our careers

**原文标题**: 'AI' might be the end of our careers

**原文链接**: [https://www.baldurbjarnason.com/2026/08-ai-might-be-the-end-of-our-careers/](https://www.baldurbjarnason.com/2026/08-ai-might-be-the-end-of-our-careers/)

生成摘要时出错

---

## 36. France Slips into Recession as Exports Sag

**原文标题**: France Slips into Recession as Exports Sag

**原文链接**: [https://www.wsj.com/world/europe/french-economy-slips-into-recession-as-exports-sag-47e934c5](https://www.wsj.com/world/europe/french-economy-slips-into-recession-as-exports-sag-47e934c5)

生成摘要时出错

---

## 37. Prospero: Bloat-free, native AI coding harness with ImGui

**原文标题**: Prospero: Bloat-free, native AI coding harness with ImGui

**原文链接**: [https://github.com/skeeto/prospero](https://github.com/skeeto/prospero)

生成摘要时出错

---

## 38. Tabernetes: A Kubernetes cluster whose nodes are browser tabs

**原文标题**: Tabernetes: A Kubernetes cluster whose nodes are browser tabs

**原文链接**: [https://tabernet.es/](https://tabernet.es/)

生成摘要时出错

---

## 39. Against the International Oligarchy

**原文标题**: Against the International Oligarchy

**原文链接**: [https://parismanifesto.world/en/](https://parismanifesto.world/en/)

生成摘要时出错

---

## 40. Poland to create no-fly zone at border after repeated airspace violations

**原文标题**: Poland to create no-fly zone at border after repeated airspace violations

**原文链接**: [https://www.france24.com/en/poland-says-will-create-no-fly-zone-at-ukraine-border-after-repeated-airspace-violations](https://www.france24.com/en/poland-says-will-create-no-fly-zone-at-ukraine-border-after-repeated-airspace-violations)

生成摘要时出错

---

## 41. Nami installs from nixpkgs without evaluating Nix

**原文标题**: Nami installs from nixpkgs without evaluating Nix

**原文链接**: [https://namios.dev/blog/nixpkgs-without-evaluating](https://namios.dev/blog/nixpkgs-without-evaluating)

生成摘要时出错

---

## 42. Euclidean geometry in the asymptotic spectrum of tensors [pdf]

**原文标题**: Euclidean geometry in the asymptotic spectrum of tensors [pdf]

**原文链接**: [https://github.com/openai/math/blob/main/preprints/Euclidean-geometry-in-the-asymptotic-spectrum-of-tensors-November-24-2026/paper.pdf](https://github.com/openai/math/blob/main/preprints/Euclidean-geometry-in-the-asymptotic-spectrum-of-tensors-November-24-2026/paper.pdf)

生成摘要时出错

---

## 43. Oakland's $30 minimum wage push advances toward city council vote

**原文标题**: Oakland's $30 minimum wage push advances toward city council vote

**原文链接**: [https://abc7news.com/post/oaklands-30-minimum-wage-push-advances-city-council-vote-alameda-workers-protest-alleged-theft-jack-box/19974057/](https://abc7news.com/post/oaklands-30-minimum-wage-push-advances-city-council-vote-alameda-workers-protest-alleged-theft-jack-box/19974057/)

生成摘要时出错

---

## 44. Nvidia halts chip shipments to south-East Asia

**原文标题**: Nvidia halts chip shipments to south-East Asia

**原文链接**: [https://www.ft.com/content/7838a715-07d4-4605-aa60-21f5af2b2370](https://www.ft.com/content/7838a715-07d4-4605-aa60-21f5af2b2370)

生成摘要时出错

---

## 45. SessionGraph: Visualize all your coding agent sessions in one interactive graph

**原文标题**: SessionGraph: Visualize all your coding agent sessions in one interactive graph

**原文链接**: [https://sessiongraph.ai/](https://sessiongraph.ai/)

生成摘要时出错

---

## 46. Z.ai clarifies GLM-5.5 has not been delayed, scheduled for December launch

**原文标题**: Z.ai clarifies GLM-5.5 has not been delayed, scheduled for December launch

**原文链接**: [https://reddit.com/r/LocalLLaMA/comments/1y6260i/zai_clarifies_glm55_has_not_been_delayed/](https://reddit.com/r/LocalLLaMA/comments/1y6260i/zai_clarifies_glm55_has_not_been_delayed/)

生成摘要时出错

---

## 47. 1984 Hosting is down due to a security incident

**原文标题**: 1984 Hosting is down due to a security incident

**原文链接**: [https://status.1984.is/status/public](https://status.1984.is/status/public)

生成摘要时出错

---

## 48. Back up your Claude Code sessions and use them on any machine

**原文标题**: Back up your Claude Code sessions and use them on any machine

**原文链接**: [https://session-vault.dev/](https://session-vault.dev/)

生成摘要时出错

---

## 49. Passkey blues

**原文标题**: Passkey blues

**原文链接**: [https://ssg.dev/passkey-blues/](https://ssg.dev/passkey-blues/)

生成摘要时出错

---

## 50. Proposed unificafion of quantum gravity and General relativity

**原文标题**: Proposed unificafion of quantum gravity and General relativity

**原文链接**: [https://www.reddit.com/r/singularity/comments/1y5u48p/openai_and_gpt6_astra_just_tackled_physics_holy/](https://www.reddit.com/r/singularity/comments/1y5u48p/openai_and_gpt6_astra_just_tackled_physics_holy/)

生成摘要时出错

---

## 51. The NFL Player Who Left Football for Math

**原文标题**: The NFL Player Who Left Football for Math

**原文链接**: [https://www.nytimes.com/2026/11/26/science/john-urschel-ai-nfl-math.html](https://www.nytimes.com/2026/11/26/science/john-urschel-ai-nfl-math.html)

生成摘要时出错

---

## 52. EightSleep tries to lock bootloader, bricks customer mattresses

**原文标题**: EightSleep tries to lock bootloader, bricks customer mattresses

**原文链接**: [https://www.reddit.com/r/EightSleep/comments/1y4x3sx/the_november_2026_eight_sleep_mass_bricking/](https://www.reddit.com/r/EightSleep/comments/1y4x3sx/the_november_2026_eight_sleep_mass_bricking/)

生成摘要时出错

---

## 53. Robots will have a staggering economic impact

**原文标题**: Robots will have a staggering economic impact

**原文链接**: [https://www.economist.com/leaders/2026/11/26/robots-will-have-a-staggering-economic-impact](https://www.economist.com/leaders/2026/11/26/robots-will-have-a-staggering-economic-impact)

生成摘要时出错

---

## 54. Banks look to dump AI debt

**原文标题**: Banks look to dump AI debt

**原文链接**: [https://www.semafor.com/article/11/26/2026/banks-look-to-dump-ai-debt](https://www.semafor.com/article/11/26/2026/banks-look-to-dump-ai-debt)

生成摘要时出错

---

## 55. Show HN: King – Man + Woman = ?

**原文标题**: Show HN: King – Man + Woman = ?

**原文链接**: [https://kingminusman.com/](https://kingminusman.com/)

生成摘要时出错

---

## 56. The US Government Is Under AI Cyberattack

**原文标题**: The US Government Is Under AI Cyberattack

**原文链接**: [https://www.forbes.com/sites/the-wiretap/2026/11/25/us-government-under-ai-cyberattack](https://www.forbes.com/sites/the-wiretap/2026/11/25/us-government-under-ai-cyberattack)

生成摘要时出错

---

## 57. Call Things What They Are

**原文标题**: Call Things What They Are

**原文链接**: [https://www.saturnci.com/call-things-what-they-are.html](https://www.saturnci.com/call-things-what-they-are.html)

生成摘要时出错

---

## 58. Stanford Physicist Uses AI to Tackle Quantum Gravity Problem

**原文标题**: Stanford Physicist Uses AI to Tackle Quantum Gravity Problem

**原文链接**: [https://thequantuminsider.com/2026/11/26/stanford-physicist-uses-ai-to-tackle-quantum-gravity-problem/](https://thequantuminsider.com/2026/11/26/stanford-physicist-uses-ai-to-tackle-quantum-gravity-problem/)

生成摘要时出错

---

