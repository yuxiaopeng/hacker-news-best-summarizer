# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2025-11-28.md)

*最后自动更新时间: 2025-11-28 20:08:35*
## 1. Zig 主仓库从 GitHub 迁移到 Codeberg

**原文标题**: Migrating the main Zig repository from GitHub to Codeberg

**原文链接**: [https://ziglang.org/news/migrating-from-github-to-codeberg/](https://ziglang.org/news/migrating-from-github-to-codeberg/)

Zig 项目正在将其主代码库从 GitHub 迁移到 Codeberg，立即生效，并使 GitHub 代码库变为只读。此举归因于 GitHub 自七年前被微软收购以来工程质量的下降，具体问题包括界面臃肿、漏洞百出、性能迟缓，以及被忽视且不可靠的 GitHub Actions 扰乱 CI。此次迁移还旨在防止违反 Zig 严格的“禁止大型语言模型/禁止人工智能”政策，因为 GitHub 的 Copilot 功能侵犯了这一政策。

尽管 GitHub Sponsors 对 Zig 的资金支持至关重要，但由于其关键负责人离职后产品质量下降，现在它被视为一种负担。Zig 软件基金会请求捐助者将定期捐款从 GitHub Sponsors 切换到非营利组织 Every.org，因为现有福利将在此处停止并重新提供。

迁移计划包括保留现有的 GitHub issues 和 pull requests，使其保持开放且不进行迁移，并将其视为“写时复制”。Codeberg 上的新 issues 将从 30000 开始编号，以确保编号的唯一性。除非需要编辑，否则用户无需迁移其 GitHub 内容，因为现有的 GitHub PRs 和 issues 仍将接受审查。作者 Andrew 强调了非营利组织在保护公共资源免受平台资本主义侵害方面的重要性。

---

## 2. 让浴室门回归酒店

**原文标题**: Bring bathroom doors back to hotels

**原文链接**: [https://bringbackdoors.com/](https://bringbackdoors.com/)

作者对酒店拆除浴室门深感不满，认为这是出于“美观”或节约成本的考虑而对隐私和尊严做出的不可接受的牺牲。他们认为浴室门应该像床一样是标配，为此，他们建立了一个名为“Bring Back Doors”（恢复房门）的网站来解决这个问题。

该网站主要有两大用途：
1. **寻找带门的酒店：** 它汇集了一份酒店名单，这些酒店保证拥有能够完全关闭且非玻璃材质的浴室门。这些信息通过直接向数百家酒店发送电子邮件，并根据价格范围和城市对它们的肯定答复进行整理。
2. **查询并举报无门酒店：** 客人可以在网站上快速搜索，查看他们正在考虑的酒店是否已被举报为缺少浴室门。该项目还依赖公众参与，鼓励客人们通过电子邮件 (bringbackdoors@gmail.com) 或 Instagram 私信（附带照片）提交没有合适浴室门的酒店，以便公开曝光。

最终目标是“点名批评”这些酒店，通过提供这些易于获取的信息来保护未来旅客的尊严和隐私。

---

## 3. Penpot：开源版Figma

**原文标题**: Penpot: The Open-Source Figma

**原文链接**: [https://github.com/penpot/penpot](https://github.com/penpot/penpot)

Penpot 常被称为“开源版 Figma”，是首个旨在实现设计与代码无缝协作的开源设计工具。它允许设计师创建设计稿、原型和设计系统，而开发人员则可获取现成的代码，从而简化工作流程并消除交接问题。

Penpot 采用 SVG、CSS、HTML 和 JSON 等开放标准运行，免费提供，既可在浏览器中使用，也可自行托管。近期重大更新，包括 2.0 版本的发布，引入了原生设计令牌（design tokens）以增强协作、突破性的 CSS 网格布局、完整的 UI 重新设计以及改进的组件系统。

主要功能包括用于即时访问代码的检查模式、灵活的插件系统，以及通过 Webhook 和 API 进行集成。Penpot 利用原生的设计令牌、组件和变体，协助构建强大的设计系统以保持一致性。用户可以将其部署为 SaaS 服务，或使用 Docker 或 Kubernetes 进行自行托管。

该平台得益于其开源社区的蓬勃发展，鼓励通过分享库、报告错误、翻译或直接贡献代码来参与贡献。行为准则有助于营造积极的环境。提供了文档和教程等资源，Penpot 遵循 Mozilla 公共许可证 v2.0，每年举办的 Penpot Fest 将社区成员聚集在一起。

---

## 4. 欧盟迫使苹果采用新的Wi-Fi标准，现在安卓可以支持隔空投送了。

**原文标题**: The EU made Apple adopt new Wi-Fi standards, and now Android can support AirDrop

**原文链接**: [https://arstechnica.com/gadgets/2025/11/the-eu-made-apple-adopt-new-wi-fi-standards-and-now-android-can-support-airdrop/](https://arstechnica.com/gadgets/2025/11/the-eu-made-apple-adopt-new-wi-fi-standards-and-now-android-can-support-airdrop/)

谷歌已更新安卓的“快速分享”功能，以支持苹果的隔空投送，从而实现安卓和iPhone设备之间的直接文件共享。这使得安卓手机可以出现在隔空投送的“所有人（10分钟）”模式中，反之亦然，尽管目前尚不支持“仅限联系人”模式。初期，此功能将仅在Pixel 10系列上可用，谷歌表示有兴趣将其扩展到更多安卓设备。谷歌强调了这些直接点对点传输的安全性，将其归功于内存安全的Rust编程语言。

这种新发现的互操作性是欧盟《数字市场法案》（DMA）的直接成果。历史上，苹果的隔空投送使用一种名为Apple无线直连（AWDL）的专有协议。然而，DMA强制苹果采用可互操作的Wi-Fi Aware标准，该标准苹果曾参与开发，但在其产品中实施缓慢。随着Wi-Fi Aware现已集成到iOS 26和iPadOS 26中（支持iPhone 12及更高版本，以及近期发布的iPad），其他设备如安卓现在也可以连接了。

谷歌自安卓8.0版本以来就支持Wi-Fi Aware，这预示着未来可能会有更广泛的安卓设备兼容性。值得注意的是，macOS的隔空投送不受DMA管辖，因此无法与安卓设备互通。谷歌的声明刻意避免提及DMA，这可能是由于该公司对该法案的广泛批评以及可能面临的罚款。

---

## 5. Linux 内核探索器

**原文标题**: Linux Kernel Explorer

**原文链接**: [https://reverser.dev/linux-kernel-explorer](https://reverser.dev/linux-kernel-explorer)

“Linux内核探索器”是一个交互式学习平台，旨在帮助用户理解Linux内核源代码，其设计基于Moon Hee Lee的《心智中的内核》。它具备文件浏览器、跨多章节的结构化指南、学习文件和知识检测。

第一章，“编写代码前理解Linux内核”，确立了以下基础概念：
*   内核不是进程；它是连接硬件和软件的基础系统权限。
*   它通过协调系统调用、中断和调度来服务用户进程。
*   内核通过一个分层系统运行，这些层被描述为虚拟的、映射的、隔离的、受控的。

该指南提供了具体学习文件，例如`init/main.c`、`kernel/fork.c`和`include/linux/sched.h`，以阐明这些要点。知识检测有助于巩固对内核本质、其对进程的服务以及其分层结构的理解。

未来章节将涵盖系统基础、内存与隔离、引导与进入、进入内核、执行上下文、通信、调度、输入/输出、虚拟化以及总结性见解，对Linux内核的内部工作原理提供全面探索。

---

## 6. Pocketbase – 开源实时后端，单文件

**原文标题**: Pocketbase – open-source realtime back end in 1 file

**原文链接**: [https://pocketbase.io/](https://pocketbase.io/)

本文介绍了 **Pocketbase**，它被描述为一个开源、实时的后端解决方案，方便地打包成一个单一文件。对于有兴趣探索其功能的用户，文章提供了其 **实时演示** 和全面的 **文档** 的直接链接。

---

## 7. 欧盟理事会通过新的“聊天控制”授权，推动大规模监控

**原文标题**: EU Council Approves New "Chat Control" Mandate Pushing Mass Surveillance

**原文链接**: [https://reclaimthenet.org/eu-council-approves-new-chat-control-mandate-pushing-mass-surveillance](https://reclaimthenet.org/eu-council-approves-new-chat-control-mandate-pushing-mass-surveillance)

欧盟理事会已批准一项新的“聊天控制”授权，其官方名称为《预防和打击儿童性虐待（CSAM）规定》。这项备受争议的提案要求私人消息服务，包括那些采用端到端加密的服务，实施“上传审核”或“客户端扫描”。这意味着所有用户通信，例如私人聊天和电子邮件，都将在加密*之前*直接在用户设备上进行扫描，以检测CSAM内容。

批评者和隐私倡导者强烈谴责这项授权，称其为一种大规模监控形式，从根本上侵蚀了隐私和数字安全。他们认为，这必然会削弱加密技术并制造不安全的后门，从而使所有用户都容易受到数据泄露和政府过度干预的侵害。担忧还包括较高的误报可能性，以及该系统可能被扩大到扫描CSAM之外其他类型内容的风险。尽管支持者将其辩解为打击儿童剥削的关键工具，但反对者则认为它是在监视全体民众，而非专注于可疑的犯罪分子，此举侵犯了基本权利，且无法保证其有效性。

在理事会批准之后，这项授权现在将进入与欧洲议会的“三方对话”谈判，欧洲议会历来对此类广泛的监控措施表示出更大的怀疑。

---

## 8. 骁龙8 Elite 第五代当日上游Linux支持

**原文标题**: Same-day upstream Linux support for Snapdragon 8 Elite Gen 5

**原文链接**: [https://www.qualcomm.com/developer/blog/2025/10/same-day-snapdragon-8-elite-gen-5-upstream-linux-support](https://www.qualcomm.com/developer/blog/2025/10/same-day-snapdragon-8-elite-gen-5-upstream-linux-support)

本文宣布，全新骁龙 8 Elite Gen 5 处理器已获得立即提供的 Linux 上游支持。其主要亮点在于这种支持的“同步发布”特性，这意味着所需的代码和驱动程序在芯片发布或公布时或之后不久，便已集成到官方 Linux 内核代码库中。这种“上游”集成至关重要，因为它确保了采用骁龙 8 Elite Gen 5 的 Linux 系统具备强大的长期兼容性、稳定性以及更简便的开发，从而造福更广泛的开源社区，并加速了新硬件上的采用。

---

## 9. DIY NAS：2026 版

**原文标题**: DIY NAS: 2026 Edition

**原文链接**: [https://blog.briancmoses.com/2025/11/diy-nas-2026-edition.html](https://blog.briancmoses.com/2025/11/diy-nas-2026-edition.html)

这篇文章详细介绍了作者的“DIY NAS：2026版”，这是他每年搭建网络附加存储服务器的传统延续。该构建遵循以下标准：小巧外形、至少六个硬盘位、集成低功耗CPU（用于24/7运行），以及作为家庭实验室支持虚拟机/容器的潜力。

作者指出当前经济形势严峻，硬盘、固态硬盘、内存、CPU和主板价格上涨，使当前成为一个艰难的搭建时期。尽管如此，该项目仍然继续进行。

选用的关键组件包括：
*   **主板/CPU：** Topton N22，搭载Intel Core 3 N355处理器，具有8个SATA接口、2个M.2 NVMe接口和10Gbps网卡，增强了家庭实验室功能。
*   **机箱：** 乔思伯（JONSBO）N4，因其性价比和可容纳六个3.5英寸和两个2.5英寸硬盘的能力而入选。
*   **风扇：** 猫头鹰（Noctua）NF-A12x25 PWM风扇取代了原装噪音较大的机箱风扇。
*   **内存：** 使用了一根32GB DDR5 4800MHz SODIMM内存条（作者特别指出当前价格昂贵）。
*   **存储：** 两块128GB的Silicon Power A55 SATA固态硬盘作为启动盘，两块1TB的Silicon Power NVMe M.2固态硬盘用于应用程序/虚拟机（受限于PCIe 3.0 x1通道）。大容量存储使用了退役硬盘，并提供了智能购买硬盘的建议。
*   **电源：** 银欣（SilverStone）SX500-G SFX电源。
*   **线缆：** SFF-8643转4个SATA分线缆，以实现高效布线。

作者一贯选择TrueNAS Community Edition，因为它具备企业级的可靠性和用户友好性。本次搭建的估计总成本（不包括新的大容量存储）为989.36美元。组装过程基本顺利，只进行了少量的线缆管理调整。

---

## 10. 展示 HN: 检测带摄像头智能眼镜的眼镜

**原文标题**: Show HN: Glasses to detect smart-glasses that have cameras

**原文链接**: [https://github.com/NullPxl/banrays](https://github.com/NullPxl/banrays)

“Ban-Rays”项目旨在开发能够检测配备摄像头的智能眼镜的眼镜，探索两种主要方法：光学和网络。

光学方法利用红外（IR）光来利用“猫眼效应”，即摄像头镜头会逆向反射光线。尽管这一概念有历史先例，但目前的实验表明，Meta Raybans发出的信号微弱且不稳定，使得现有硬件难以与其他反射表面进行可靠区分。开发者正在试验特定的红外扫描模式并结合不同波长，同时刻意避免使用机载摄像头进行检测。

网络方法侧重于低功耗蓝牙（BLE）和Wi-Fi分析。目前，通过BLE广播对Meta Raybans进行指纹识别是最有前景和可靠的方法。系统在Meta Raybans开机、配对或从眼镜盒中取出时，能成功检测到Meta特有的制造商ID（0x01AB）和服务UUID（0xFD5F）。然而，在持续使用（当眼镜连接到手机时）期间检测定向BLE流量具有挑战性，并且需要比当前ESP32配置更先进的硬件。传统蓝牙检测也被指出是硬件密集型的。

总体而言，BLE指纹识别提供了一种初步的检测能力，但两种方法在活跃使用期间实现一致、实时的摄像头检测都面临重大的技术障碍。

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 2 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 3 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 4 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 5 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 6 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 7 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 8 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 9 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 10 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 11 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 12 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 13 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 14 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 15 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 16 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 17 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 18 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 19 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 20 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 21 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
| 22 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 23 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
