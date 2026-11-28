# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-11-28.md)

*最后自动更新时间: 2026-11-28 02:10:50*
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

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-11-28](output/hacker_news_summary_2026-11-28.md) |
| 2 | [2026-11-24](output/hacker_news_summary_2026-11-24.md) |
| 3 | [2026-11-25](output/hacker_news_summary_2026-11-25.md) |
| 4 | [2026-11-26](output/hacker_news_summary_2026-11-26.md) |
| 5 | [2026-11-27](output/hacker_news_summary_2026-11-27.md) |
| 6 | [2026-11-23](output/hacker_news_summary_2026-11-23.md) |
| 7 | [2026-11-19](output/hacker_news_summary_2026-11-19.md) |
| 8 | [2026-11-22](output/hacker_news_summary_2026-11-22.md) |
| 9 | [2026-11-21](output/hacker_news_summary_2026-11-21.md) |
| 10 | [2026-11-18](output/hacker_news_summary_2026-11-18.md) |
| 11 | [2026-11-20](output/hacker_news_summary_2026-11-20.md) |
| 12 | [2026-11-14](output/hacker_news_summary_2026-11-14.md) |
| 13 | [2026-11-15](output/hacker_news_summary_2026-11-15.md) |
| 14 | [2026-11-12](output/hacker_news_summary_2026-11-12.md) |
| 15 | [2026-11-13](output/hacker_news_summary_2026-11-13.md) |
| 16 | [2026-11-17](output/hacker_news_summary_2026-11-17.md) |
| 17 | [2026-11-07](output/hacker_news_summary_2026-11-07.md) |
| 18 | [2026-11-06](output/hacker_news_summary_2026-11-06.md) |
| 19 | [2026-11-11](output/hacker_news_summary_2026-11-11.md) |
| 20 | [2026-11-08](output/hacker_news_summary_2026-11-08.md) |
| 21 | [2026-11-10](output/hacker_news_summary_2026-11-10.md) |
| 22 | [2026-11-01](output/hacker_news_summary_2026-11-01.md) |
| 23 | [2026-11-03](output/hacker_news_summary_2026-11-03.md) |
| 24 | [2026-11-05](output/hacker_news_summary_2026-11-05.md) |
| 25 | [2026-10-31](output/hacker_news_summary_2026-10-31.md) |
| 26 | [2026-10-30](output/hacker_news_summary_2026-10-30.md) |
| 27 | [2026-11-04](output/hacker_news_summary_2026-11-04.md) |
| 28 | [2026-10-24](output/hacker_news_summary_2026-10-24.md) |
| 29 | [2026-10-25](output/hacker_news_summary_2026-10-25.md) |
| 30 | [2026-10-27](output/hacker_news_summary_2026-10-27.md) |
| 31 | [2026-10-28](output/hacker_news_summary_2026-10-28.md) |
| 32 | [2026-10-26](output/hacker_news_summary_2026-10-26.md) |
| 33 | [2026-10-29](output/hacker_news_summary_2026-10-29.md) |
| 34 | [2026-10-19](output/hacker_news_summary_2026-10-19.md) |
| 35 | [2026-10-18](output/hacker_news_summary_2026-10-18.md) |
| 36 | [2026-10-23](output/hacker_news_summary_2026-10-23.md) |
| 37 | [2026-10-21](output/hacker_news_summary_2026-10-21.md) |
| 38 | [2026-10-22](output/hacker_news_summary_2026-10-22.md) |
| 39 | [2026-10-20](output/hacker_news_summary_2026-10-20.md) |
| 40 | [2026-10-17](output/hacker_news_summary_2026-10-17.md) |
| 41 | [2026-10-13](output/hacker_news_summary_2026-10-13.md) |
| 42 | [2026-10-15](output/hacker_news_summary_2026-10-15.md) |
| 43 | [2026-10-14](output/hacker_news_summary_2026-10-14.md) |
| 44 | [2026-10-16](output/hacker_news_summary_2026-10-16.md) |
| 45 | [2026-10-09](output/hacker_news_summary_2026-10-09.md) |
| 46 | [2026-10-11](output/hacker_news_summary_2026-10-11.md) |
| 47 | [2026-10-07](output/hacker_news_summary_2026-10-07.md) |
| 48 | [2026-10-10](output/hacker_news_summary_2026-10-10.md) |
| 49 | [2026-10-06](output/hacker_news_summary_2026-10-06.md) |
| 50 | [2026-10-04](output/hacker_news_summary_2026-10-04.md) |
| 51 | [2026-10-03](output/hacker_news_summary_2026-10-03.md) |
| 52 | [2026-10-02](output/hacker_news_summary_2026-10-02.md) |
| 53 | [2026-09-29](output/hacker_news_summary_2026-09-29.md) |
| 54 | [2026-09-30](output/hacker_news_summary_2026-09-30.md) |
| 55 | [2026-09-27](output/hacker_news_summary_2026-09-27.md) |
| 56 | [2026-10-01](output/hacker_news_summary_2026-10-01.md) |
| 57 | [2026-09-24](output/hacker_news_summary_2026-09-24.md) |
| 58 | [2026-09-21](output/hacker_news_summary_2026-09-21.md) |
| 59 | [2026-09-23](output/hacker_news_summary_2026-09-23.md) |
| 60 | [2026-09-25](output/hacker_news_summary_2026-09-25.md) |
| 61 | [2026-09-22](output/hacker_news_summary_2026-09-22.md) |
| 62 | [2026-09-18](output/hacker_news_summary_2026-09-18.md) |
| 63 | [2026-09-20](output/hacker_news_summary_2026-09-20.md) |
| 64 | [2026-09-19](output/hacker_news_summary_2026-09-19.md) |
| 65 | [2026-09-17](output/hacker_news_summary_2026-09-17.md) |
| 66 | [2026-09-16](output/hacker_news_summary_2026-09-16.md) |
| 67 | [2026-09-15](output/hacker_news_summary_2026-09-15.md) |
| 68 | [2026-09-12](output/hacker_news_summary_2026-09-12.md) |
| 69 | [2026-09-13](output/hacker_news_summary_2026-09-13.md) |
| 70 | [2026-09-11](output/hacker_news_summary_2026-09-11.md) |
| 71 | [2026-09-14](output/hacker_news_summary_2026-09-14.md) |
| 72 | [2026-09-09](output/hacker_news_summary_2026-09-09.md) |
| 73 | [2026-09-10](output/hacker_news_summary_2026-09-10.md) |
| 74 | [2026-09-05](output/hacker_news_summary_2026-09-05.md) |
| 75 | [2026-09-02](output/hacker_news_summary_2026-09-02.md) |
| 76 | [2026-09-06](output/hacker_news_summary_2026-09-06.md) |
| 77 | [2026-09-03](output/hacker_news_summary_2026-09-03.md) |
| 78 | [2026-09-08](output/hacker_news_summary_2026-09-08.md) |
| 79 | [2026-09-07](output/hacker_news_summary_2026-09-07.md) |
| 80 | [2026-09-04](output/hacker_news_summary_2026-09-04.md) |
| 81 | [2026-08-29](output/hacker_news_summary_2026-08-29.md) |
| 82 | [2026-09-01](output/hacker_news_summary_2026-09-01.md) |
| 83 | [2026-08-25](output/hacker_news_summary_2026-08-25.md) |
| 84 | [2026-08-30](output/hacker_news_summary_2026-08-30.md) |
| 85 | [2026-08-26](output/hacker_news_summary_2026-08-26.md) |
| 86 | [2026-08-31](output/hacker_news_summary_2026-08-31.md) |
| 87 | [2026-08-28](output/hacker_news_summary_2026-08-28.md) |
| 88 | [2026-08-20](output/hacker_news_summary_2026-08-20.md) |
| 89 | [2026-08-16](output/hacker_news_summary_2026-08-16.md) |
| 90 | [2026-08-22](output/hacker_news_summary_2026-08-22.md) |
| 91 | [2026-08-24](output/hacker_news_summary_2026-08-24.md) |
| 92 | [2026-08-18](output/hacker_news_summary_2026-08-18.md) |
| 93 | [2026-08-17](output/hacker_news_summary_2026-08-17.md) |
| 94 | [2026-08-21](output/hacker_news_summary_2026-08-21.md) |
| 95 | [2026-08-23](output/hacker_news_summary_2026-08-23.md) |
| 96 | [2026-08-19](output/hacker_news_summary_2026-08-19.md) |
| 97 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 98 | [2026-08-11](output/hacker_news_summary_2026-08-11.md) |
| 99 | [2026-08-10](output/hacker_news_summary_2026-08-10.md) |
| 100 | [2026-08-15](output/hacker_news_summary_2026-08-15.md) |
| 101 | [2026-08-12](output/hacker_news_summary_2026-08-12.md) |
| 102 | [2026-08-14](output/hacker_news_summary_2026-08-14.md) |
| 103 | [2026-08-09](output/hacker_news_summary_2026-08-09.md) |
| 104 | [2026-08-13](output/hacker_news_summary_2026-08-13.md) |
| 105 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 106 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 107 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 108 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 109 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 110 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 111 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 112 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 113 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 114 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 115 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 116 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 117 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 118 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 119 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 120 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 121 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 122 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 123 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 124 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 125 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 126 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 127 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 128 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 129 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 130 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 131 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 132 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 133 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 134 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 135 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 136 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 137 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 138 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 139 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 140 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 141 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 142 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 143 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 144 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 145 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 146 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 147 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 148 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 149 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 150 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 151 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 152 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 153 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 154 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 155 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 156 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 157 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 158 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 159 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 160 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 161 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 162 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 163 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 164 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 165 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 166 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 167 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 168 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 169 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 170 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 171 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 172 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 173 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 174 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 175 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 176 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 177 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 178 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 179 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 180 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 181 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 182 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 183 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 184 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 185 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 186 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 187 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 188 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 189 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 190 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 191 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 192 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 193 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 194 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 195 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 196 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 197 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 198 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 199 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 200 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 201 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 202 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 203 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 204 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 205 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 206 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 207 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 208 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 209 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 210 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 211 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 212 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 213 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 214 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 215 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 216 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 217 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 218 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 219 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 220 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 221 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 222 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 223 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 224 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 225 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 226 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 227 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 228 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 229 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 230 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 231 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 232 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 233 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 234 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 235 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 236 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 237 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 238 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 239 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 240 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 241 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 242 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 243 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 244 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 245 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 246 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 247 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 248 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 249 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 250 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 251 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 252 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 253 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 254 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 255 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 256 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 257 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 258 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 259 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 260 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 261 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 262 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 263 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 264 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 265 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 266 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 267 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 268 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 269 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 270 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 271 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 272 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 273 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 274 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 275 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 276 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 277 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 278 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 279 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 280 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 281 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 282 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 283 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 284 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 285 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 286 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 287 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 288 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 289 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 290 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 291 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 292 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 293 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 294 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 295 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 296 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 297 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 298 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 299 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 300 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 301 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 302 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 303 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 304 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 305 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 306 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 307 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 308 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 309 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 310 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 311 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 312 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 313 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 314 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 315 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 316 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 317 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 318 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 319 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 320 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 321 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 322 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 323 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 324 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 325 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 326 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 327 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 328 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 329 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 330 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 331 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 332 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 333 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 334 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 335 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 336 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 337 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 338 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 339 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 340 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 341 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 342 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 343 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 344 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 345 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 346 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 347 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 348 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 349 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 350 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 351 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 352 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 353 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 354 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 355 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 356 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 357 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 358 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 359 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 360 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 361 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 362 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 363 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 364 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 365 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 366 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 367 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 368 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 369 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 370 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 371 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 372 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 373 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 374 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 375 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 376 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
