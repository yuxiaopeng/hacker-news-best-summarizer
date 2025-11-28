# Hacker News 热门文章摘要 (2025-11-28)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

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

## 11. 人工智能CEO：别等老板换掉你，你先换掉老板

**原文标题**: AI CEO – Replace your boss before they replace you

**原文链接**: [https://replaceyourboss.ai/](https://replaceyourboss.ai/)

文章《AI CEO：在你被取代前先取代你的老板》探讨了人工智能日益增强的、承担高级领导和管理职能的能力，从而有效挑战传统的人类高管角色。

其核心前提是一个严峻的警告：人工智能不仅是一种优化工具，而且正在演变为一种能够进行战略决策、资源分配和监督的力量——这些职能通常由CEO或高级经理执行。这一转变带来了前所未有的效率、数据驱动的公正性和可扩展性。

至关重要的是，文章将这种威胁延伸到高管层之外，认为如果AI能取代老板，那么它肯定也能取代那些不适应的普通员工。因此，其核心信息是呼吁采取积极行动：职场人士必须学会将AI不仅作为一种生产力工具，而且作为战略伙伴加以利用，以提升自身的价值和决策能力。

在你的老板取代*你*之前“取代你的老板”意味着理解AI的潜力，将其融入自己的工作流程，并发展独特的、人类特有的技能——例如创造力、情商、批判性思维和复杂问题解决能力——这些技能应与AI的优势互补，而非竞争。文章强调要成为组织内部AI解决方案不可或缺的推动者和架构师，而不是被动旁观者或其进步的潜在受害者。

---

## 12. S&box 现在是开源游戏引擎

**原文标题**: S&box is now an open source game engine

**原文链接**: [https://sbox.game/news/update-25-11-26](https://sbox.game/news/update-25-11-26)

S&box，由Facepunch Studios开发的游戏平台，已正式转型为开源游戏引擎。

---

## 13. 不要下载应用

**原文标题**: Don't Download Apps

**原文链接**: [https://blog.calebjay.com/posts/dont-download-apps/](https://blog.calebjay.com/posts/dont-download-apps/)

文章强烈建议不要下载应用程序，理由是其激进做法，尤其是在台湾，工作人员甚至可能在未经同意的情况下为了一点小折扣而安装应用程序，从而导致不必要的垃圾信息。

作者提出支持这一立场的两个主要原因：

1.  **监控资本主义与定价：** 应用程序使公司能够收集大量用户数据，从而导致“监控定价”。这使得企业可以收取个性化价格（例如，当他们知道你刚发工资时会收取更高的价格），从而赋予它们对货币价值和你的购买力过度的权力，而不是由市场力量决定。
2.  **强制仲裁：** 应用程序的“服务条款”中经常包含强制仲裁条款。这些条款强制用户进行私人争议解决，绕过有法官和陪审团的传统法院系统。仲裁员通常由公司聘用，造成了严重的力量不平衡。文章引用了杰弗里·皮科洛的案例，他因妻子去世起诉迪士尼的案件，险些因Disney+订阅条款而被强制仲裁。由于美国最高法院支持强制仲裁，个人必须采取措施，避免放弃自己的权利。

作者警告说，未来可能会出现应用程序的使用（例如，优步外卖、Twitter/TeXla、华盛顿邮报/亚马逊）会强制对涉及母公司的无关事件进行仲裁。最终建议是避免下载应用程序，以保护个人数据和权利。

---

## 14. TPU与GPU：为何谷歌有望长期赢得AI竞赛

**原文标题**: TPUs vs. GPUs and why Google is positioned to win AI race in the long term

**原文链接**: [https://www.uncoveralpha.com/p/the-chip-made-for-the-ai-inference](https://www.uncoveralpha.com/p/the-chip-made-for-the-ai-inference)

谷歌于2013年开发了张量处理单元（TPU），以应对AI日益增长的计算需求，它意识到传统的CPU和GPU在深度学习核心的大规模矩阵乘法方面效率低下。TPU是专为TensorFlow（现也支持PyTorch）神经网络设计的专用集成电路（ASIC），并于2015年迅速在内部投入使用。

核心区别在于TPU的“脉动阵列”架构。与通用GPU因“架构包袱”而受限不同，TPU通过让数据直接流经计算单元，最大限度地减少内存读写（冯·诺依曼瓶颈），从而在AI任务中实现显著更高的每焦耳运算量。谷歌最新的TPUv7（代号“铁木”）在性能上取得了显著飞跃，包括4,614 TFLOPS（BF16）、192GB HBM和先进的芯片间互连。

尽管官方数据有限，但行业专家和前谷歌员工指出，TPU在特定AI应用中提供了卓越的成本效益和每瓦性能，一些估计表明，其每美元性能比英伟达的Hopper GPU高1.4倍，效率高60-65%。谷歌TPU的改进速度也被认为快于英伟达。

尽管有这些优势，但更广泛的采用仍面临挑战：英伟达主导的CUDA/PyTorch生态系统使得切换变得困难，尽管TPU更适合对CUDA依赖性较低的推理工作负载。此外，TPU是Google Cloud Platform独有的，由于数据传出成本和客户对供应商锁定的担忧，造成了多云障碍——这些问题是英伟达普遍可用的GPU所没有的。

---

## 15. 请愿：在德国正式承认开源工作为公民服务

**原文标题**: Petition to formally recognize open source work as civic service in Germany

**原文链接**: [https://www.openpetition.de/petition/online/anerkennung-von-open-source-arbeit-als-ehrenamt-in-deutschland#petition-main](https://www.openpetition.de/petition/online/anerkennung-von-open-source-arbeit-als-ehrenamt-in-deutschland#petition-main)

德国发起了一项请愿活动，倡导将开源开发正式认定为一种公民服务或志愿工作（“Ehrenamt”或“Vereinsarbeit”）。开源开发者要求将他们的贡献与传统志愿活动同等对待，此举旨在获得官方认可并争取与此类公民参与相关的潜在利益。

---

## 16. GitLab 发现大范围 NPM 供应链攻击

**原文标题**: GitLab discovers widespread NPM supply chain attack

**原文链接**: [https://about.gitlab.com/blog/gitlab-discovers-widespread-npm-supply-chain-attack/](https://about.gitlab.com/blog/gitlab-discovers-widespread-npm-supply-chain-attack/)

GitLab 漏洞研究团队发现了一场广泛的 npm 供应链攻击，涉及一种代号为“Shai-Hulud”的破坏性恶意软件变体。这种复杂的恶意软件被观察到像蠕虫一样传播，通过多阶段加载过程感染 npm 包。

初次感染通过修改后的 `package.json` 的 preinstall 脚本发生，该脚本执行 `setup_bun.js`。这个伪装成 Bun JavaScript 运行时安装程序的脚本，随后启动一个大型、混淆的恶意载荷 `bun_environment.js`。

一旦激活，该恶意软件会收集来自 GitHub、npm、AWS、GCP 和 Azure 的敏感凭据，并使用下载的 Trufflehog 二进制文件广泛扫描文件系统以查找秘密信息。被盗数据被窃取到攻击者控制的公共 GitHub 仓库，这些仓库可通过描述“Sha1-Hulud: The Second Coming”识别。恶意软件利用窃取的 npm 令牌，通过将其加载器和载荷注入受害者维护的其他包中、增加版本并重新发布它们来进行传播。

一项关键发现是“死人开关”：如果恶意软件同时失去对其 GitHub 窃取和 npm 传播通道的访问，它将触发一个破坏性载荷。这种机制会删除并覆盖受感染系统上的用户数据，使得协同清除行动风险极高，因为存在大规模数据破坏的威胁。

GitLab 提供了妥协指标（IoC），并概述了其旗舰版（Ultimate）功能，例如依赖扫描（Dependency Scanning）和 Duo Chat 的安全分析师代理（Security Analyst Agent）如何帮助检测暴露。这次攻击代表了一种演变，其中附带损害成为攻击者基础设施的主要防御手段，因此需要仔细的修复策略。

---

## 17. 我们的声音正在被大型语言模型淹没。

**原文标题**: We're losing our voice to LLMs

**原文链接**: [https://tonyalicea.dev/blog/were-losing-our-voice-to-llms/](https://tonyalicea.dev/blog/were-losing-our-voice-to-llms/)

文章认为，社交媒体上大语言模型生成内容的大量涌现，正导致我们失去独特的人类声音，而这种声音被认为是宝贵的财富。作者指出，现在许多帖子听起来千篇一律，仿佛都出自同一个“社交媒体经理”之手，缺乏个人表达的独特性。

独特的声音，由一生的经历塑造而成，被视为具有内在价值。它能被识别，培养信任，并与受众建立联系。这种真实性对于留下持久印象至关重要，无论是在求职面试、人脉拓展等专业场合，甚至能带来职业机会，正如作者亲身经历的那样。文章强调，个人声音会随着练习而成熟并变得更加独特。

关键在于，作者认为大语言模型无法真正复制独特的声音，因为它并非一成不变，而是随着人生的经历和心境而演变。依赖人工智能撰写内容会扼杀这种自然发展，导致“认知惰性”，并使这一重要资产逐渐萎缩。文章最后敦促读者用自己真实的声音写作，让它成长，并将真正的人类表达置于优先地位，而非人工智能生成的语言“混音”。

---

## 18. 250兆瓦时沙电池将在芬兰开建

**原文标题**: 250MWh 'Sand Battery' to start construction in Finland

**原文链接**: [https://www.energy-storage.news/250mwh-sand-battery-to-start-construction-in-finland-for-both-heating-and-ancillary-services/](https://www.energy-storage.news/250mwh-sand-battery-to-start-construction-in-finland-for-both-heating-and-ancillary-services/)

芬兰极夜能源公司（Polar Night Energy）与公共事业公司拉赫蒂能源（Lahti Energia）正在合作，在芬兰万萨（Vääksy）建造一个 250MWh 的“沙电池”热能储存（TES）系统，用于区域供暖和辅助电网服务。该系统供热功率为 2MW，储能容量为 125 小时，建成后将成为全球最大的沙基热能储存项目。

该技术利用电力加热当地可用的天然沙子，将热量储存起来，随后释放到拉赫蒂能源的区域供暖网络。该项目预计每年将减少约 60% 的化石燃料相关排放，主要通过将天然气消耗量减少 80% 来实现。

至关重要的是，其规模使其能够参与芬兰 Fingrid 的备用和电网平衡市场，在日益依赖天气的能源日益增加的情况下，有助于电网稳定。建设工程计划于 2026 年初启动，并于 2027 年夏季完工。此前，极夜能源公司曾成功部署了一个使用皂石的 1MW/100MWh 沙电池。拉赫蒂能源首席执行官强调该项目在提供经济实惠、可再生区域供暖和增强电网灵活性方面的优势。

---

## 19. 极客帝国——硅谷法西斯主义与对民主的战争

**原文标题**: The Nerd Reich – Silicon Valley Fascism and the War on Democracy

**原文链接**: [https://www.simonandschuster.com/books/The-Nerd-Reich/Gil-Duran/9781668221402](https://www.simonandschuster.com/books/The-Nerd-Reich/Gil-Duran/9781668221402)

吉尔·杜兰的《书呆子帝国》一书认为，硅谷尽管披着进步主义的外衣，却对民主构成重大威胁，正演变为一个“书呆子帝国”。该书声称，科技巨头在技术乌托邦主义、自由意志主义意识形态和巨额财富的驱动下，正积极破坏民主机构。

杜兰详细阐述了科技领袖对威权主义的历史性推崇，引用了史蒂夫·乔布斯和彼得·蒂尔等人物为例，并指出业内普遍存在的“兄弟文化”与这种倾向不谋而合。该书解释了科技平台如何助长虚假信息、仇恨言论的传播以及公民对话的侵蚀，同时通过监控资本主义和用户数据武器化牟利。

《书呆子帝国》还强调了科技公司积极游说反对监管和工会化的行为。杜兰认为，他们宣扬一种“技术官僚封建主义”的愿景，在这种愿景中，他们行使不受制约的权力，取代传统治理。该书严厉警告，这种不受制约的权力如何加剧不平等，并滋生一种新型的数字威权主义，从根本上挑战民主的基石。

---

## 20. A16Z的惊人论断

**原文标题**: A Remarkable Assertion from A16Z

**原文链接**: [https://nealstephenson.substack.com/p/a-remarkable-assertion-from-a16z](https://nealstephenson.substack.com/p/a-remarkable-assertion-from-a16z)

Neal Stephenson的文章分析了Andreessen Horowitz (A16Z) 的博客文章《是时候建造了》，该文章倡导国家重新关注实体基础设施——住房、交通、制造业和能源——并将“不建造文化”归咎于监管俘获和风险规避。考虑到A16Z作为一家风险投资公司，在*数字*初创企业上投入巨资并从中获利，并在很大程度上促成了“软件吞噬世界”的范式，Stephenson认为这一主张“非同寻常”。

Stephenson强调了其中的讽刺意味：A16Z作为推动数字优先经济的关键参与者，现在却呼吁转向实体建设，而没有承认自己对它现在似乎正在批判的趋势所产生的影响。他指出A16Z的文章缺乏自我反思，将自己描绘成一个客观的观察者，而非现有科技格局中的主要参与者。

Stephenson质疑A16Z的动机，猜测这是否代表了其投资理念的真正转变，抑或仅仅是一种修辞策略。他将A16Z的抽象呼吁与那些真正建造实体基础设施的人所面临的具体挑战进行对比，强调了数字项目和实体项目在时间线、资金要求和监管环境上的巨大差异。Stephenson暗示A16Z的影响主要局限于数字领域的“元”层面，因此他们呼吁建造“真实”事物的举动显得尤为引人注目。

---

## 21. 米克斯潘内尔安全泄露

**原文标题**: Mixpanel Security Breach

**原文链接**: [https://mixpanel.com/blog/sms-security-incident/](https://mixpanel.com/blog/sms-security-incident/)

Mixpanel宣布于2025年11月8日检测到一起安全事件，该事件源于一场短信钓鱼（smishing）活动，影响了少数客户。该公司迅速启动了事件响应，采取全面措施以遏制和清除未经授权的访问，并保护受影响的用户账户。Mixpanel已与外部网络安全合作伙伴和执法部门合作，开展补救和调查工作。

该公司主动联系了所有受影响的客户，并明确指出，如果客户没有直接收到通知，则其账户未受影响，无需采取任何行动。Mixpanel详细说明了其响应措施，包括保护受影响的账户、撤销活跃会话、更换受损凭据、阻止恶意IP地址、对所有员工进行全局密码重置，并聘请第三方取证公司审查日志并就遏制措施提供建议。他们还实施了额外的控制措施，以检测和阻止未来类似的活动。

收到通知的受影响客户被建议查阅该通知，以了解具体的后续步骤。任何疑问可发送至 support@mixpanel.com。Mixpanel通过首席执行官Jen Taylor强调了其对安全、透明和客户支持的承诺。

---

## 22. 美国公民配偶绿卡面试戴手铐收场

**原文标题**: Green card interviews end in handcuffs for spouses of U.S. citizens

**原文链接**: [https://www.nytimes.com/2025/11/26/us/trump-green-card-interview-arrests.html](https://www.nytimes.com/2025/11/26/us/trump-green-card-interview-arrests.html)

无法访问文章链接

---

## 23. 可能吞噬辐射的神秘切尔诺贝利黑真菌

**原文标题**: The mysterious black fungus from Chernobyl that may eat radiation

**原文链接**: [https://www.bbc.com/future/article/20251125-the-mysterious-black-fungus-from-chernobyl-that-appears-to-eat-radiation](https://www.bbc.com/future/article/20251125-the-mysterious-black-fungus-from-chernobyl-that-appears-to-eat-radiation)

1997年，Nelli Zhdanova 在切尔诺贝利爆炸的核反应堆内部发现了一种神秘的黑色真菌，它在其中茁壮成长并朝着辐射源生长。这种富含黑色素的霉菌表现出“趋辐射性”（radiotropism），表明生命可以利用电离辐射。

Ekaterina Dadachova 的进一步研究提出了“辐射合成”（radiosynthesis）理论，即黑色素将高能辐射转化为真菌生长所需的可用能量，类似于光合作用。研究发现，含黑色素的真菌在放射性环境中生长速度快10%，其中黑色素既能作为吸收有害颗粒的屏障，又能充当抗氧化剂。

这一发现具有重要意义，尤其是在太空旅行方面。在国际空间站对球形枝孢菌（*Cladosporium sphaerospermum*，一种切尔诺贝利菌株）进行的实验表明，它在太空中生长更快，并能有效阻挡银河宇宙射线。尽管科学家仍在调查这种生长是否完全由辐射驱动或受零重力影响，但这种真菌的屏蔽潜力是很有前景的。

这种“真菌建筑”（myco-architecture）可能在月球或火星上建造出自我再生、防辐射的栖息地，从而大幅降低运输传统屏蔽材料的重量和成本。尽管辐射合成仍是一个需要进一步机制理解的理论，但这些真菌为保护宇航员和清洁放射性环境提供了一个革命性的解决方案。

---

## 24. 巴基斯坦称，明年一些区域的屋顶太阳能发电量将超过电网需求。

**原文标题**: Pakistan says rooftop solar output to exceed grid demand in some hubs next year

**原文链接**: [https://www.reuters.com/sustainability/boards-policy-regulation/pakistan-says-rooftop-solar-output-exceed-grid-demand-some-hubs-next-year-2025-11-22/](https://www.reuters.com/sustainability/boards-policy-regulation/pakistan-says-rooftop-solar-output-exceed-grid-demand-some-hubs-next-year-2025-11-22/)

巴基斯坦预计，到明年（2025年），特定工业和城市中心的屋顶太阳能发电量将超过电网需求。联邦能源部长穆罕默德·阿里宣布了这一消息，他将这一快速增长归因于太阳能的积极普及，特别是得益于净计量政策的工业、商业实体和家庭的大力采用。

尽管这一重大转变对于向可再生能源转型并减少对昂贵进口化石燃料的依赖至关重要，但它也给国家电网带来了巨大挑战。现有的输配电基础设施尚未完全具备管理预期过剩电力以及太阳能固有波动的能力，这可能导致电网不稳定，并需要限制清洁能源输出。

为解决这些问题，巴基斯坦迫切需要对电网现代化进行大规模投资，包括智能电网技术、电池和抽水蓄能等大规模储能解决方案，以及输电线路升级。此外，可能需要审查当前的净计量政策，以确保电网稳定和高效能源管理。从长远来看，有效管理这些过剩电力可能为向邻国出口清洁能源开辟途径。

---

## 25. 音乐缓解手术并加速康复，研究发现

**原文标题**: Music eases surgery and speeds recovery, study finds

**原文链接**: [https://www.bbc.com/news/articles/c231dv9zpz3o](https://www.bbc.com/news/articles/c231dv9zpz3o)

一项来自德里毛拉纳·阿扎德医学院和洛克·纳亚克医院的、经同行评审的印度新研究发现，在全身麻醉期间播放音乐可以显著减轻手术过程并加速康复。该研究发表在《音乐与医学》杂志上，提供了有力证据，表明这种简单的干预措施可以显著减少药物需求并改善患者预后。

这项研究针对56名接受腹腔镜胆囊切除术（即胆囊摘除手术）的成年人。患者被随机分为两组：两组都接受了标准的五种药物麻醉方案并佩戴了降噪耳机，但其中一组听了平静的器乐（长笛或钢琴）。

研究人员观察到，即使患者处于无意识状态，其听觉通路仍部分活跃。结果显示，听音乐的患者所需的异丙酚等麻醉药物和芬太尼等阿片类止痛药的剂量更低。因此，他们在术后苏醒更快、更清醒，恢复更平稳，皮质醇（应激激素）水平更低，手术期间血压控制也更好。

参与研究的麻醉师，如法拉赫·侯赛因医生和索尼亚·瓦德哈万医生解释说，即使在麻醉状态下，身体也会触发应激反应，从而减缓康复。音乐似乎通过提供大脑能够识别的积极刺激，即使患者没有意识记忆，也能平息这种内在的“风暴”。这种非药物方法为手术室带来了人文关怀，有望通过减少药物使用和提升患者整体福祉来重塑外科护理。

---

## 26. Meta利用高等几何隐匿270亿美元债务

**原文标题**: Meta hiding $27B in debt using advanced geometry

**原文链接**: [https://stohl.substack.com/p/exclusive-credit-report-shows-meta](https://stohl.substack.com/p/exclusive-credit-report-shows-meta)

Substack上署名“Stohl”的一篇文章声称，Meta Platforms正通过一种被称为“高级几何”的复杂金融策略，隐瞒大约270亿美元的潜在债务。该作者引用一家主要机构贷款人提供的一份“独家匿名信用报告”，声称Meta利用复杂的衍生品和利率互换来实现这一目的。

据报道，该策略涉及Meta出售大量针对其他科技公司的“价外信用违约互换（CDS）”，同时收购高评级的长期公司债券。出售这些CDS所获得的保费被用于购买债券。由于这些CDS是“价外”的，根据标准会计准则，其潜在的未来义务并未在Meta的资产负债表上被完全确认为即时债务。

据报道，该信用报告估计这项隐藏负债的*公允价值*为270亿美元，这代表着在这些CDS同时被触发情况下的理论最坏情景。文章指出，这一操作使Meta能够呈现更健康的资产负债表，保持较低的感知债务比率，并可能获得更好的融资条件。作者对会计透明度以及一旦出现连锁违约，可能暴露金融系统内此类潜在负债所带来的潜在系统性风险表示担忧。

---

## 27. 在已淘汰设备上运行不支持的iOS

**原文标题**: Running Unsupported iOS on Deprecated Devices

**原文链接**: [https://nyansatan.github.io/run-unsupported-ios/](https://nyansatan.github.io/run-unsupported-ios/)

这篇文章详细介绍了在iPod touch 3上运行不受支持的iOS 6的过程，该设备官方最高支持iOS 5.1.1。作者首先在iPhone 3GS上进行了测试，确定了需要修改的关键区域。

主要工作涉及修补多个iOS组件：
*   **设备树 (DeviceTree)：** 开发了一个脚本，用于对比并应用iOS 6特有的硬件节点和属性，这对于iBoot在运行时填充的`nvram-proxy-data`字段至关重要。
*   **iBoot：** 需要进行少量修改，包括Image3签名修补、`amfi=0xff`启动参数注入、启用调试功能，以及动态填充NVRAM数据。
*   **内核缓存 (Kernelcache)：** 最复杂的部分。由于动态内核扩展 (kext) 加载失败，使用`kcgen`（来自macOS内部构建版本）生成了一个预链接内核缓存。这涉及指定kexts（通过比较iPhone 3GS的iOS 5.1.1和6.0构建版本得出）并剥离生成的fat Mach-O头部。
*   **恢复内存盘 (Restore Ramdisk)：** 修补了`asr`并重新定位了`options.plist`。重新实现了`rc.boot`二进制文件，以便在第三分区安装iBoot漏洞利用。
*   **根文件系统 (Root Filesystem)：** 涉及添加SpringBoard硬件功能plist文件，整合5.1.1的多点触控、Wi-Fi和蓝牙固件，并从FairPlay守护进程的plist中移除`LimitLoadToHardware`以启用设备激活。
*   **DYLD共享缓存 (DYLD Shared Cache)：** 补丁包括硬编码产品ID并在MobileGestalt中交换短ID，以及强制`getDeviceVariant()`返回"A"以防止激活崩溃。通过重新计算修改部分的SHA-1哈希值来修复代码签名。
*   **iBoot漏洞利用 (iBoot Exploit)：** 重新实现了一个确定性HFS+文件系统驱动漏洞利用用于启动。

作者总结称该项目充满挑战但比预期容易，未来计划实现越狱并将此工作移植到iPad 1。所描述的方法为类似的、不受支持的iOS尝试提供了指导。

---

## 28. 被低估的感恩理由 五

**原文标题**: Underrated reasons to be thankful V

**原文链接**: [https://dynomight.net/thanks-5/](https://dynomight.net/thanks-5/)

《被低估的感恩理由 V》

本文，题为《被低估的感恩理由 V》，列举了涵盖生物学、科学、技术和社会结构等多个领域的各种被忽视的幸事。

在生物学方面，文章表达了对狗狗真挚的爱、有性生殖基因变异带来的进化优势、过氧化物酶体的无声高效运作，以及睡眠作为日常“重置”的恢复能力的感恩。文章还俏皮地提到了拥有三维身体的便利性。

在健康和技术领域，作者感恩于最终有望“治愈”普通感冒，我们通过卫生、疫苗和先进工具（紫外线杀菌、空气过滤）来控制传染病的集体能力，以及对抗基因工程病原体的“更疯狂策略”的可能性。其他亮点包括丰富的洁净水、牙科医疗、航空旅行固有的安全性，以及放射性原子防止大规模永久性环境污染的特性。感恩还延伸到同时治疗多种疾病的非线性益处、数据拟合中表达式图表梯度的数学优雅，以及在二维胶片上存储五维光场（全息术）的物理奇迹。一次性塑料也因其功用和作为碳捕获的潜力而受到关注。

在社会和哲学层面，文章赞赏人类偏好的多样性、小豆蔻这种负担得起的奢侈品、市场判断力往往优于个人担忧、吸引-爱-繁衍这个复杂却成功的“组合”、社会支持父母的隐性约定，以及尽管经历了漫长的专制历史，民主和公民自由仍在不断取得历史进步。

---

## 29. DeepSeekMath-V2：迈向自可验证的数学推理 [pdf]

**原文标题**: DeepSeekMath-V2: Towards Self-Verifiable Mathematical Reasoning [pdf]

**原文链接**: [https://github.com/deepseek-ai/DeepSeek-Math-V2/blob/main/DeepSeekMath_V2.pdf](https://github.com/deepseek-ai/DeepSeek-Math-V2/blob/main/DeepSeekMath_V2.pdf)

所提供的信息描述了一个来自deepseek-ai的项目或研究论文，标题为“DeepSeekMath-V2：迈向自我验证的数学推理”。

这个标题表明，这项工作致力于开发具有增强数学推理能力的先进人工智能模型（特别是DeepSeekMath-V2）。强调的核心目标是“自我验证”的推理，这表明该模型的设计不仅是为了解决数学问题，还在于内部检查、验证或证明其自身解决方案的正确性。这旨在提高人工智能在复杂数学任务中的可靠性和可信度。

名称中的“V2”暗示着相对于DeepSeekMath先前版本的演进或重大更新，表明正在持续开发以完善其数学能力。“[pdf]”标签证实了它以正式文档的形式呈现，很可能是一篇详细介绍了方法、结果和发现的研究论文。

随附的元数据，例如“Fork 44”和“Star 864”（典型的GitHub仓库数据），表明公众对DeepSeekMath-V2项目有相当大的兴趣和社区参与，凸显了其在人工智能研究领域的重要性。

---

## 30. GPL向AI模型传播理论的现状

**原文标题**: The current state of the theory that GPL propagates to AI models

**原文链接**: [https://shujisado.org/2025/11/27/gpl-propagates-to-ai-models-trained-on-gpl-code/](https://shujisado.org/2025/11/27/gpl-propagates-to-ai-models-trained-on-gpl-code/)

本文强调了美国与日本、欧盟等其他主要司法管辖区在开源许可证法律解释上的一个关键分歧。尽管日本和欧盟通常将开源许可证视为许可协议或合同，但作为许多开源运动发源地的美国，却持不同看法。美国法律认为开源许可证并非合同，而是一种“单方面许可”。这种区别代表着在不同法律框架下理解和应用这些许可证方式上的一个重大“法律妙招”。

---

## 31. 亚瑟·柯南·道尔通过夏洛克·福尔摩斯探讨了男性心理健康。

**原文标题**: Arthur Conan Doyle explored men’s mental health through Sherlock Holmes

**原文链接**: [https://theconversation.com/arthur-conan-doyle-explored-mens-mental-health-through-his-sherlock-holmes-stories-246728](https://theconversation.com/arthur-conan-doyle-explored-mens-mental-health-through-his-sherlock-holmes-stories-246728)

亚瑟·柯南·道尔是一位思想进步的作家，他深入探讨了男性的脆弱性和心理健康问题，这一主题因他父亲的酗酒及其最终被送入精神病院而对他个人意义深远。道尔笔下的夏洛克·福尔摩斯正是这种体现，他塑造了一个并非完美无缺但却令人产生共鸣的天才，他与毒瘾、孤独和抑郁症作斗争——这些弱点反而成就了他的非凡才华。

道尔经常刻画处于情感困境中的男性角色。在《歪嘴男人》中，内维尔·圣克莱尔因经济窘迫而感到羞耻，过着乞丐的双重生活，这凸显了维多利亚时代社会对男性气质的压力；他甚至宁愿被处决也不愿名誉受损。《证券经纪人》则探讨了经济焦虑和男性自杀问题，剧中哈利·平纳为避免入狱而企图自杀。

《工程师大拇指案》的主人公是水利工程师维克多，他遭受了身体暴力和精神创伤。华生医生处理其身体伤势，而福尔摩斯则提供了关键的心理支持，扮演了知己和安慰者的角色，甚至提供了兴奋剂。这体现了道尔对男性心理健康护理重要性的信念。

尽管当时的读者将这些元素视为福尔摩斯天才的标志，但如今它们为我们了解维多利亚时代男性的精神挣扎提供了重要的窗口，在过去和现在的读者之间建立了强大的联系。

---

## 32. 领英喧嚣，职场是地狱

**原文标题**: LinkedIn is loud, and corporate is hell

**原文链接**: [https://ramones.dev/posts/linkedin-is-loud/](https://ramones.dev/posts/linkedin-is-loud/)

文章《领英很喧嚣，企业如地狱》批评了领英和现代企业文化的现状，认为它们已变得流于形式、脱离了真正的职业价值。

作者感叹，领英曾是一个有用的社交工具，却已沦为“表演式积极”和“内卷文化”的平台。动态被用户用来推广自己、副业，或分享夸大的企业成功和韧性故事所占据，而这些往往缺乏实质内容。这营造了一个喧嚣的环境，真正的联系和见解在铺天盖地的自我推销和“道德表演”中迷失了。

这篇文章进一步将批判延伸至企业生活本身，指出许多公司将肤浅的指标、流行语和表演式“文化”置于有意义的工作或员工福祉之上。这导致了一种不真实感和职业倦怠，个体感到压力，被迫在网上和线下都维持着热情和生产力的假象。作者表达了对更真诚互动以及回归重视实际工作与诚实沟通的渴望，而非领英和许多企业环境中普遍存在的刻意制造的热情。

---

## 33. 二维光线步进软阴影 (2020)

**原文标题**: Ray Marching Soft Shadows in 2D (2020)

**原文链接**: [https://www.rykap.com/2020/09/23/distance-fields/](https://www.rykap.com/2020/09/23/distance-fields/)

本文详细介绍了一种利用距离场渲染软阴影的二维光线步进技术。距离场是一种图像，存储着每个像素到最近形状的距离，最初由二维文本生成。

投射阴影的核心思想涉及从像素向光源进行“光线步进”。光线并非逐像素缓慢检查，而是根据`sceneDist`（从距离场中采样的到最近形状的距离）前进。这种高效方法确保不会跳过任何形状。如果光线碰到形状（`sceneDist <= 0`），该像素处于阴影中；否则，如果光线到达光源，则被照亮。带有步数限制（例如64步）的`for`循环可以防止复杂光线路径导致的性能问题。

对于软阴影（一种非物理真实的半影），应用了三条规则：
1. **离形状越近，阴影越深：** 通过步进过程中最小的`sceneDist`来近似。
2. **阴影从“近似交点”处扩散得更远：** 与`rayProgress`相关。
前两条规则通过在步进过程中追踪`sceneDist / rayProgress`的最小值作为`lightContribution`来结合。比率为1表示完全被照亮，0表示完全处于阴影中。
3. **光线随距离衰减：** 最终的`lightContribution`乘以一个二次衰减的`distanceFactor`，该因子随着光线离光源越远而减小。

尽管高效且快速，该方法会产生条带状伪影。解决方案包括更高级的近似法，或者使用`sceneDist * randomJitter`来增加步数和颗粒感以消除条带。

---

## 34. Fara-7B：用于计算机的高效智能体模型

**原文标题**: Fara-7B: An efficient agentic model for computer use

**原文链接**: [https://github.com/microsoft/fara](https://github.com/microsoft/fara)

Fara-7B是微软首个为计算机使用专门设计的智能体小型语言模型（SLM）。仅凭70亿参数，这款超紧凑的计算机使用智能体（CUA）在其同类尺寸中提供了最先进的性能，能有效与更大的智能体系统竞争。

与传统聊天模型不同，Fara-7B通过鼠标和键盘界面进行视觉操作，执行多步骤网络任务。它感知网页并执行滚动、打字和点击预测坐标等操作，而不依赖于辅助功能树。其紧凑的尺寸便于设备端部署，提供更低的延迟和增强的隐私保护，并且能高效完成任务，平均每项任务仅需16步。

Fara-7B通过一种新颖的合成数据生成管道进行训练，利用Magentic-One多智能体框架创建了145,000条多样化轨迹。它基于Qwen2.5-VL-7B构建并经过微调，擅长自动化常见的网络活动，例如信息搜索、表单填写、预订旅行、在线购物以及寻找工作或房地产。

该模型在WebVoyager、Online-M2W、DeepShop和新发布的WebTailBench等网络智能体基准测试中展现了最先进的成果。Fara-7B持续超越其他计算机使用模型，甚至是一些更大的系统，尤其是在包含609项真实世界任务的新基准WebTailBench上表现突出。

用户可以通过克隆其代码库、设置Python环境并使用VLLM（需要GPU）托管模型，在本地试用Fara-7B。另外，Azure Foundry提供了一个推荐的托管解决方案，无需本地GPU硬件。微软强调Fara-7B是一个实验性版本，鼓励社区反馈，并建议在沙盒环境中进行使用。此外，还提供了全面的评估基础设施以确保可复现性。

---

## 35. 如何查尔斯·米·舒尔茨创作了查理·布朗和史努比 (2024)

**原文标题**: How Charles M Schulz created Charlie Brown and Snoopy (2024)

**原文链接**: [https://www.bbc.com/culture/article/20241205-how-charles-m-schulz-created-charlie-brown-and-snoopy](https://www.bbc.com/culture/article/20241205-how-charles-m-schulz-created-charlie-brown-and-snoopy)

查尔斯·M·舒尔茨创作了全球广受欢迎的《花生漫画》，独自绘制了50年，直到1999年因健康不佳宣布退休，并于2000年最后一期漫画刊登后不久去世。舒尔茨谦逊地将自己的作品描述为处理爱、恨和不安全感等“日常小问题”，但他坚持认为这些问题比政治或琐事更重要，构成了日常社会讽刺。

艾柯（Umberto Eco）指出，《花生漫画》的普遍吸引力，既迷住了儿童，也征服了老练的成年人。舒尔茨最初出于商业考虑，专注于画儿童，因为“这样才卖得好”。他发现自己的角色，尤其是史努比，为任何想法提供了多功能的“剧团”，并经常将狗描绘成“比孩子更聪明”。

他害羞的童年，导致他通过函授而非面授方式学习艺术，塑造了他独特的视角，让他觉得“非常适合做漫画家”。舒尔茨强调要隔绝外界，“只管画些你希望有趣的东西”，当好的想法涌现时，他会感到兴奋。尽管他很谦逊，但他始终坚信《花生漫画》会成功。

舒尔茨去世后发表的最后一期漫画，向粉丝们表达了感谢。他通过查理·布朗（Charlie Brown）传达了一个重要的教训：“只要坚持不懈地尝试”，因为他的角色“永不放弃”。

---

## 36. Alan.app – 给 macOS 激活窗口添加边框

**原文标题**: Alan.app – Add a Border to macOS Active Window

**原文链接**: [https://tyler.io/2025/11/alan/](https://tyler.io/2025/11/alan/)

作者开发了一款名为“Alan”的全新 macOS 应用，旨在解决区分活动窗口的挑战，这可能是因为视力下降或 macOS 对比度不佳。Alan 是一款简单的应用程序，可以在活动窗口周围绘制一个可自定义的边框。用户可以在 Alan 的偏好设置中设置首选的边框宽度，并为亮色和深色模式选择不同的颜色。该应用可供下载，还有一个演示视频展示了其功能。对于喜欢极简设置的用户，Alan 还提供一个隐藏偏好设置，可以通过终端命令激活，从而在 Dock 中隐藏其图标。

---

## 37. Coq：全球最佳宏汇编器？ (2013) [pdf]

**原文标题**: Coq: The World's Best Macro Assembler? (2013) [pdf]

**原文链接**: [https://nickbenton.name/coqasm.pdf](https://nickbenton.name/coqasm.pdf)

所提供的内容是原始的、压缩的PDF流数据，而非可读文本。作为AI，我无法直接解压缩或解释这种二进制格式。因此，我无法提供文章内容的摘要。

标题“Coq: The World's Best Macro Assembler? (2013)”表明该论文可能探讨了Coq证明助手在低级代码生成方面的能力，并可能论证其作为一种高度可靠或强大的工具，用于创建和验证类汇编代码的适用性。

如果您能提供文章的实际文本，我将很乐意为您总结。

---

## 38. 欧盟理事会批准与议会谈判的聊天控制授权

**原文标题**: EU Council approves Chat Control mandate for negotiation with Parliament

**原文链接**: [https://www.techradar.com/vpn/vpn-privacy-security/chat-control-eu-lawmakers-finally-agree-on-the-voluntary-scanning-of-your-private-chats](https://www.techradar.com/vpn/vpn-privacy-security/chat-control-eu-lawmakers-finally-agree-on-the-voluntary-scanning-of-your-private-chats)

欧盟理事会经过三年多的努力，于2025年11月26日星期三达成协议，批准了备受争议的《儿童性虐待条例》（CSAR），该条例常被称为“聊天控制”。这一决定使得与欧洲议会的谈判得以启动。

争议的核心在于，该条例拟要求所有消息服务（包括采用端到端加密的服务）扫描用户的私人聊天，以查找儿童性虐待材料（CSAM）。尽管早期版本曾强制要求这样做，但丹麦轮值主席国提出的折衷方案将聊天扫描改为“自愿”，从而促成了理事会的协议。

尽管有这项修正案，隐私专家、密码学家和技术专家仍持高度批评态度，警告该提案仍对“社会构成高风险”，并称其为可能导致“全面监控”的“政治欺骗”。

根据新规定，在线服务提供商必须评估其平台可能如何被滥用，并实施缓解措施。高风险服务可能被迫开发技术来应对这些风险，并由一个新的欧盟机构监督实施。尽管成员国庆祝在打击CSAM方面迈出了一步，但在即将到来的三方谈判中，如何在网络安全与基本数字权利和强加密之间取得平衡，担忧依然存在。

---

## 39. 禽流感病毒耐热，使其对人类构成重大威胁。

**原文标题**: Bird flu viruses are resistant to fever, making them a major threat to humans

**原文链接**: [https://medicalxpress.com/news/2025-11-bird-flu-viruses-resistant-fever.html](https://medicalxpress.com/news/2025-11-bird-flu-viruses-resistant-fever.html)

本文讨论的研究表明，禽流感病毒（avian influenza）已进化出对发热的抵抗力，而发热传统上是帮助哺乳动物对抗感染的机制。这种适应性使其对人类构成更大的威胁。

主要发现包括：
*   与典型的哺乳动物病毒不同，禽流感病毒，特别是H5N1和H7N9，即使在模拟发热的升高温度下也能有效复制。
*   该研究使用与人类感染高度相似的雪貂模型，结果显示，发热般的温度并未抑制病毒复制或降低上呼吸道的病毒载量。
*   这种耐热性归因于病毒聚合酶复合体中的突变，具体来说是PB2基因（E627K和D701N突变），这些突变有助于病毒适应哺乳动物宿主。
*   该研究强调，人类对禽流感的免疫反应可能会受损，因为一种主要的防御机制（发热）对这些病毒的效力降低。
*   该研究强调迫切需要专门针对这些耐热禽流感毒株设计新的抗病毒策略和疫苗，尤其考虑到其大流行潜力。它们规避发热防御的能力使其对公共卫生尤其令人担忧。

---

## 40. 科技巨头积聚数百万美元战争基金，对抗人工智能监管

**原文标题**: Tech Titans Amass Multimillion-Dollar War Chests to Fight AI Regulation

**原文链接**: [https://www.wsj.com/tech/ai/tech-titans-amass-multimillion-dollar-war-chests-to-fight-ai-regulation-88c600e1](https://www.wsj.com/tech/ai/tech-titans-amass-multimillion-dollar-war-chests-to-fight-ai-regulation-88c600e1)

无法访问文章链接。

---

## 41. 荷兰高校离得开微软吗？

**原文标题**: Can Dutch universities do without Microsoft?

**原文链接**: [https://dub.uu.nl/en/news/can-dutch-universities-do-without-microsoft](https://dub.uu.nl/en/news/can-dutch-universities-do-without-microsoft)

对不起，但文章内容尚未提供。文本只包含“HOP”。因此，我无法总结荷兰大学是否可以没有微软，也无法总结这样一篇文章的要点会是什么。请提供文章的全文，我很乐意为您总结。

---

## 42. 维索拉 约顿-8 5纳米 欧洲推理芯片

**原文标题**: Vsora Jotunn-8 5nm European inference chip

**原文链接**: [https://vsora.com/products/jotunn-8/](https://vsora.com/products/jotunn-8/)

Vsora Jotunn-8 被推出为“全球最高效的AI推理芯片”，是一款5纳米欧洲推理解决方案，宣称拥有“0/tflops”效率。该芯片旨在改变现代数据中心中的AI部署方式，为训练好的模型提供极快的速度、极低的成本和轻松的可扩展性。

Jotunn-8 的主要特点包括超低延迟，这对聊天机器人和欺诈检测等实时应用至关重要；以及超高吞吐量，这对于推荐引擎和LLM API等高要求服务不可或缺。该芯片设计注重成本效益，可在大规模部署时显著降低每次推理的成本；同时注重能源效率，旨在削减运营开支和碳足迹。

Jotunn-8 架构确保了灵活性，能够实现各类AI模型的顺畅集成和接近理论峰值的性能，其中包括推理模型、生成式AI（大型语言模型LLMs）和智能体AI。这种多功能性使其能够处理日益复杂和组合的AI系统。Vsora 将 Jotunn-8 定位为大规模AI的新基础，其性能超越现有市场解决方案（例如 Llama3 405B），从而最大化AI投资、降低运营成本并促进可持续发展。

---

## 43. 性感回归。网络监控扼杀了情色。

**原文标题**: Bringing Sexy Back. Internet surveillance has killed eroticism

**原文链接**: [https://lux-magazine.com/article/privacy-eroticism/](https://lux-magazine.com/article/privacy-eroticism/)

无法访问文章链接。

---

## 44. 法国政府称，AdBlock和Signal是恐怖分子工具 (2023) [视频]

**原文标题**: AdBlock and Signal are for terrorists, according to French govt (2023) [video]

**原文链接**: [https://www.youtube.com/watch?v=1q1hjmwLqe4](https://www.youtube.com/watch?v=1q1hjmwLqe4)

所提供的“文章”主要包含一个标题，该标题声称法国政府在2023年将AdBlock和Signal描述为“恐怖分子”工具。该标题还表明来源是一个视频。

随后的内容完全由标准的YouTube法律和版权信息组成（例如，“关于新闻版权联系我们创作者广告开发者条款隐私权政策与安全YouTube 的运作方式测试新功能NFL Sunday Ticket© 2025 Google LLC”），并且没有提供关于法国政府所谓声明的进一步细节、背景或阐述。

---

## 45. 施工人员指控无聊公司拖欠工人工资并对OSHA的担忧置之不理

**原文标题**: Crews claim Boring Company failed to pay workers and snubbed OSHA concerns

**原文链接**: [https://nashvillebanner.com/2025/11/25/boring-company-nashville-shane-trucking-and-excavating/](https://nashvillebanner.com/2025/11/25/boring-company-nashville-shane-trucking-and-excavating/)

肖恩卡车运输与挖掘公司（Shane Trucking and Excavating）作为埃隆·马斯克旗下“无聊公司”（TBC）在纳什维尔“音乐之城环线”隧道项目上的关键分包商，已因据称未付款和安全担忧撤走了其团队。该公司老板威利·肖恩声称，在TBC单方面延长付款期限后，已拖欠123天，但仅支付了六位数欠款的约百分之五。据报道，其他分包商也因类似原因离开。

肖恩还指控一名TBC代表试图挖走他的焊工，从而违反合同。此外，他报告称已就危险工作条件多次向OSHA（美国职业安全与健康管理局）提出投诉，其中包括TBC员工未佩戴适当的个人防护装备（PPE）以及在深挖区存在危险支撑（使用木制2x12s而非混凝土）。肖恩表示他公开此事是为了防止人员受伤。

“无聊公司”副总裁大卫·巴斯承认存在“开票错误”，并承诺在周三前支付所有未结发票，同时否认这是常见做法。巴斯还否认TBC的政策是挖走承包商，并表示他不知道有任何OSHA投诉，但他承诺会进行调查，强调安全对公司至关重要。

州参议员海蒂·坎贝尔批评TBC最近的宣传活动“不真诚”，因为工作人员立即撤离，并对州政府对不安全条件的责任以及TBC的问责制表示担忧。肖恩最初表示他不会返回，但后来表示，如果TBC纠正这种情况，他会考虑。

---

## 46. HN 展示: Runprompt — 在命令行运行 .prompt 文件

**原文标题**: Show HN: Runprompt – run .prompt files from the command line

**原文链接**: [https://github.com/chr15m/runprompt](https://github.com/chr15m/runprompt)

Runprompt是一个极简的单文件Python脚本，旨在直接从命令行执行Dotprompt文件，无需外部依赖。Dotprompt是一种用于生成式AI的可执行提示模板格式，使`.prompt`文件能够同时捆绑提示模板和基本元数据（模型、schema、配置）。

用户可以通过下载脚本、使其可执行，然后运行`.prompt`文件来快速上手，通常通过管道输入JSON来填充模板变量（例如，`echo '{"name": "World"}' | ./runprompt hello.prompt`）。它利用类似Handlebars的模板语法来处理变量、迭代和节，包括一个用于管道输入的特殊`{{STDIN}}`变量。

主要功能包括：使用Picoschema定义提取结构化JSON输出的能力；通过将一个提示的JSON输出通过管道传递给另一个来链式调用提示；以及通过shebang使`.prompt`文件直接可执行。命令行覆盖允许在运行时修改任何前置元数据值（例如，`./runprompt --model ...`）。

配置通过API密钥的环境变量（例如`OPENAI_API_KEY`）和用于全局覆盖的`RUNPROMPT_*`变量进行处理。它支持来自Anthropic、OpenAI、Google AI和OpenRouter的模型，指定为`provider/model-name`格式。Runprompt是Dotprompt规范的一个极简实现，像多消息提示、条件语句和高级模型配置等功能尚未支持。

---

## 47. 中国纯电卡车与柴油霸权的终结

**原文标题**: China's BEV trucks and the end of diesel's dominance

**原文链接**: [https://cleantechnica.com/2025/11/26/chinas-bev-trucks-and-the-end-of-diesels-dominance/](https://cleantechnica.com/2025/11/26/chinas-bev-trucks-and-the-end-of-diesels-dominance/)

中国纯电动重型卡车（BEV卡车）正在迅速扩张，其价格（5.8万至8.5万欧元）远低于西方同类产品（25万欧元以上）。这些车辆是专门设计的电动车型，将磷酸铁锂电池组和电驱动桥集成到简化底盘中，大幅降低了成本。

尽管最初的中国BEV卡车需要2万至4万欧元的改装才能满足西方短途运输的安全、舒适和监管标准，但其到岸价格（8万至12万欧元）仍极具竞争力。这使得它们非常适合大部分短途（<250公里）城市和区域货运，对西方普遍关注长途电气化的趋势构成了挑战。

中国重型卡车市场反映了这一转变，BEV卡车销量从2024年的13%上升到2025年初的22%，将柴油车的份额推至接近50%。天然气卡车也有增长，但面临来自BEV的压力。然而，氢燃料电池卡车所占份额微不足道（低于1%）且正在下降。这种快速转型已经影响到中国的柴油消耗。

西方原始设备制造商（OEM）最初通过改装柴油车底盘以适应电动动力系统，面临成本较高和设计优化不足的挑战。他们现在正转向专门设计的电动平台。中国成熟的BEV供应链和规模化带来的成本降低，为脱碳提供了一条更快、更经济的途径。西方运营商和政策制定者必须决定如何应对这种新的成本结构，因为电动货运在大多数实际工况下比柴油车在经济上更具吸引力，这预示着柴油车主导地位的终结。

---

## 48. C100 开发者终端

**原文标题**: C100 Developer Terminal

**原文链接**: [https://caligra.com/](https://caligra.com/)

卡利格拉（Caligra）开发工具，例如 C100 开发者终端，专门针对准确性、可靠性和生产力至关重要的技术环境。他们的产品专为那些依赖工作成果、并重视保持专注“心流状态”的专业人士设计。C100 被定位为一款基于独特原则打造的电脑，它优先考虑用户需求，并实现高效任务完成，最终帮助创作者“完成工作”。

---

## 49. Linux 输入栈：端到端架构概览

**原文标题**: The input stack on Linux: An end-to-end architecture overview

**原文链接**: [https://venam.net/blog/unix/2025/11/27/input_devices_linux.html](https://venam.net/blog/unix/2025/11/27/input_devices_linux.html)

Linux 输入栈由内核层、对外暴露层和用户空间层组成。

在**内核层**，**输入核心**是处理输入设备和事件的中心。输入设备驱动程序（例如键盘、鼠标）向该核心注册，将设备特定的协议抽象为标准化格式。它们通过 `input_event` 向核心推送事件，核心随后将这些事件分发给已注册的**输入处理程序**。**evdev**（事件设备）处理程序是默认的，它将这些事件作为字符设备（例如 `/dev/input/eventX`）在 `devtmpfs` 中暴露给用户空间。

内核使用 `kobjects`（总线、设备、驱动程序、类、子系统）维护设备的层次结构视图，并在 `sysfs`（例如 `/sys/devices/`）中进行表示。**总线**（例如 PCI、USB、HID）是基础，负责连接设备并启动设备与其相应驱动程序的匹配过程。这种匹配可以级联，一个总线可以作为另一个总线上的设备（例如 PCI 上的 USB）。

当设备插入或拔出时，内核通过 `netlink` 发出 **uevents**。这些事件包含一个 `MODALIAS` 字符串，其中包含设备识别信息（供应商/产品 ID）。在**用户空间**中，`udev` 监控这些 `uevents`，利用 `MODALIAS` 通过 `modprobe` 动态加载所需的内核模块，从而管理设备的**热插拔**和初始设置。`sysfs` 和 `procfs` 也提供对内核对象和输入核心的自省功能。

---

## 50. 函数式数据结构与算法：基于证明助手的方法

**原文标题**: Functional Data Structures and Algorithms: a Proof Assistant Approach

**原文链接**: [https://fdsa-book.net/](https://fdsa-book.net/)

《函数式数据结构与算法：证明助手方法》一书由ACM图书出版，专门为函数式语言介绍了数据结构和算法。该书由Tobias Nipkow以及包括Jasmin Blanchette和Bohua Zhan在内的团队合著，核心着重于严格的证明。它以统一的方式涵盖了函数式正确性与运行时间分析，并利用归纳证明来验证函数式程序及其相关的运行时间函数。

一个关键的显著特点是，书中所有证明都已通过Isabelle证明助手进行形式化机器验证，并且PDF中嵌入了指向相应Isabelle理论的直接链接。这确保了高度的可靠性和精确性。该出版物旨在成为一个不断演进的资源，并积极邀请社区贡献。完整书籍可通过可点击的图片进行下载。

---

## 51. 特斯拉Model Y刚刚获得了十年来最差的可靠性评级。

**原文标题**: The Tesla Model Y Just Scored the Worst Reliability Rating in a Decade

**原文链接**: [https://www.autoblog.com/news/the-bestselling-tesla-model-y-just-scored-the-worst-reliability-rating-in-a-decade](https://www.autoblog.com/news/the-bestselling-tesla-model-y-just-scored-the-worst-reliability-rating-in-a-decade)

根据《消费者报告》2023年可靠性调查，特斯拉Model Y获得了十年来的最低可靠性评级。其得分仅为100分中的8分，预估可靠性较去年大幅下降。

这种糟糕的表现归因于车主报告的众多问题，特别是其空调系统和车身完整性方面，包括嘎嘎作响的噪音和面板错位。油漆质量问题和信息娱乐系统故障也被提及。Model Y的问题似乎源于设计缺陷和组装问题的结合，而不仅仅是软件错误。

尽管Model Y拉低了特斯拉的整体可靠性得分，但Model 3和Model S等其他车型表现更好，其中Model 3还获得了《消费者报告》的推荐。然而，Model X也显示出低于平均水平的可靠性。总体而言，特斯拉在30个品牌中排名第14位，较去年略有提升。

尽管存在这些可靠性问题，Model Y仍然是一款极受欢迎的汽车，经常是全球最畅销的电动汽车之一。然而，对于那些优先考虑长期可靠性的潜在买家来说，《消费者报告》的最新数据发出了一个重要的警示。

---

## 52. 2800万Hacker News评论作为向量嵌入搜索数据集

**原文标题**: 28M Hacker News comments as vector embedding search dataset

**原文链接**: [https://clickhouse.com/docs/getting-started/example-datasets/hackernews-vector-search-dataset](https://clickhouse.com/docs/getting-started/example-datasets/hackernews-vector-search-dataset)

本文介绍了一个包含2874万条Hacker News帖子和评论的数据集，每条都带有由`all-MiniLM-L6-v2` SentenceTransformers模型生成的384维向量嵌入。该数据集由ClickHouse以S3上的Parquet文件形式提供，可作为一个真实世界的例子，用于设计和评估基于文本数据的大规模向量搜索应用。

本指南详细介绍了使用ClickHouse实现向量搜索的分步过程：
1.  **表创建：** 定义一个`hackernews`表，包含`id`、`text`和`vector` (Array(Float32)) 嵌入列，以及其他元数据。
2.  **数据加载：** 将S3 Parquet文件中的2874万行数据插入到ClickHouse表中。
3.  **索引构建：** 在`vector`列上创建一个HNSW向量相似性索引，指定`cosineDistance`和超参数（M=64, ef_construction=512）。
4.  **向量搜索：** 在SQL中使用`cosineDistance`执行近似最近邻（ANN）查询，以查找语义相似的帖子。
5.  **查询嵌入：** 使用Python中相同的`all-MiniLM-L6-v2`模型为用户搜索查询生成嵌入。

本文还介绍了一个生成式AI摘要应用。该系统接受一个主题，生成其嵌入，通过ClickHouse向量搜索检索相关的Hacker News内容，然后使用LangChain和OpenAI的`gpt-3.5-turbo`对检索到的帖子进行摘要。这展示了向量嵌入如何为大型语言模型提供关键上下文，适用于情感分析或技术支持自动化等各种企业领域。

---

## 53. 万亿美元或将浪费在生成式AI上

**原文标题**: A trillion dollars (potentially) wasted on gen-AI

**原文链接**: [https://garymarcus.substack.com/p/a-trillion-dollars-is-a-terrible](https://garymarcus.substack.com/p/a-trillion-dollars-is-a-terrible)

加里·马库斯的文章《万亿美元（可能）浪费在生成式AI上》指出，对生成式AI的巨额投资大部分是徒劳且方向错误的。马库斯认为，尽管该领域充斥着大量炒作和资金投入，但核心技术仍存在根本性缺陷。

他强调，当前的大型语言模型（LLMs）本质上是“随机鹦鹉”，它们擅长模式匹配，但缺乏真正的理解、常识和可靠性。这导致了“幻觉”、事实性错误以及无法有效推理等问题，使得它们在没有大量人工监督的情况下不适用于关键应用。马库斯指出，尽管其表面能力令人印象深刻，但底层机制多年来并未发生根本性改变，许多所谓的突破都是渐进式的，而非革命性的。

文章认为，专注于通过更多数据和算力来扩展现有架构是一种收益递减的策略。业界没有解决深层次的认知挑战，却主要依赖蛮力。马库斯总结道，这万亿美元的投资可能被浪费在一条无法提供稳健、可信和真正智能AI的道路上，他倡导转向开发具有更深层认知能力而非仅仅更大的统计模型的系统。

---

## 54. 基于 io_uring 和 kqueue 的开发者友好型 I/O 抽象 (2022)

**原文标题**: A programmer-friendly I/O abstraction over io_uring and kqueue (2022)

**原文链接**: [https://tigerbeetle.com/blog/2022-11-23-a-friendly-abstraction-over-iouring-and-kqueue/](https://tigerbeetle.com/blog/2022-11-23-a-friendly-abstraction-over-iouring-and-kqueue/)

本文介绍了一种“对程序员友好的 I/O 抽象”，旨在利用现代内核接口（例如 Linux 的 `io_uring` 和 FreeBSD/macOS 的 `kqueue`）的性能。它强调了传统阻塞和非阻塞 I/O 因代价高昂的系统调用而效率低下的问题。

`io_uring` 和 `kqueue` 通过批处理 I/O 和完成队列提供改进。`io_uring` 更进一步，允许内核执行实际的 `read`/`write` 操作，从而最大限度地减少用户态开销。然而，直接使用这些底层 API 可能将 I/O 机制与业务逻辑纠缠在一起，从而创建复杂的事件循环。

所提出的抽象（例如 `io_dispatch`）集中管理 I/O 调度，使开发人员能够调度带有完成回调的操作。它透明地处理操作系统差异，利用 `io_uring` 的内核端 I/O，或者在 `kqueue` 准备就绪事件后执行用户态 I/O。该系统使用用户数据字段将回调链接到事件，管理一个用于未调度请求的溢出队列，并提供高级 API 封装。这种架构促进了简洁、用户管理的事件循环，类似于 `libuv`、TigerBeetle 和 Bun 中的方法。文章还提到了 Windows 的 IOCP，并讨论了用于确定性的单线程事件循环，同时承认针对不同工作负载的多线程替代方案。文中暗示将提供一个独立的 Zig 库。

---

## 55. AI采用率开始趋于平稳

**原文标题**: AI Adoption Rates Starting to Flatten Out

**原文链接**: [https://www.apolloacademy.com/ai-adoption-rates-starting-to-flatten-out/](https://www.apolloacademy.com/ai-adoption-rates-starting-to-flatten-out/)

2025年11月28日，阿波罗首席经济学家托斯滕·斯洛克（Torsten Sløk）报告称，人工智能在美国所有规模的企业中的采纳率正开始趋于平稳。这一评估是基于美国人口普查局和Ramp AI指数的数据。

Ramp AI指数衡量美国企业采纳人工智能产品和服务的速度。该指数利用Ramp企业信用卡和账单支付平台收集的来自超过40,000家企业和数十亿美元企业支出数据。报告的趋势是基于六次调查的移动平均值，调查每两周进行一次。

---

## 56. SQLite 作为应用文件格式

**原文标题**: SQLite as an Application File Format

**原文链接**: [https://sqlite.org/appfileformat.html](https://sqlite.org/appfileformat.html)

文章《SQLite作为应用程序文件格式》倡导使用SQLite数据库文件来持久化应用程序状态和交换信息。它将应用程序文件格式定义为存储多个对象及其关系的文件格式，并将其与存储单个对象的格式区分开来。

该文将现有格式分为三类：
1.  **完全自定义格式：** 不透明、二进制，需要专用工具（例如DOC、PDF）。
2.  **文件堆格式：** 将文件系统用作键/值存储，可访问但不便传输，且缺少单一文档实体（例如Git）。
3.  **封装文件堆格式：** 将文件堆封装成单个归档文件（例如EPUB的ZIP），提供单个文件，但对微小更改通常需要完全重写。

SQLite被提出作为优越的第四类，能够将从简单的键/值结构到复杂的关联模式的数据高效地存储在单个文件中。

将SQLite用作应用程序文件格式的主要优势包括：
*   **简化应用程序开发：** 通过利用SQLite强大、成熟的库，减少I/O编码。
*   **单一文件文档：** 保留了“文档”的隐喻，使文件易于管理、移动和识别。
*   **高级查询语言：** SQL允许开发人员表达“需要什么”数据，而不是“如何”检索，从而简化逻辑。
*   **可访问内容：** 数据不是不透明的二进制大对象；它可以通过通用工具和良好文档化的跨平台格式进行访问，确保了持久性。
*   **原子事务：** 保证数据完整性和崩溃安全，防止写入期间的数据损坏。
*   **增量和持续更新：** 只有更改的部分才写入磁盘，从而提高性能，减少SSD磨损，并防止数据丢失。
*   **易于扩展：** 可以修改模式（添加表/列）而不会破坏向后兼容性。
*   **性能：** 通过仅查询必要数据而不是解析整个文档，可以提供更快的启动和操作。

---

## 57. 文件吉拉 Pro “永久授权” — 致全体用户的一则警告

**原文标题**: FileZilla Pro "Perpetual License" – A Warning to All Users

**原文链接**: [https://github.com/x011/FileZilla-Pro-Download](https://github.com/x011/FileZilla-Pro-Download)

本文对FileZilla Pro的“永久许可证”发出了严厉警告。作者购买了此类许可证，却发现一旦重装操作系统或丢失原始安装程序，该许可证便形同虚设。

操作系统重装后，作者联系了FileZilla Pro支持部门，以获取其合法拥有的版本安装程序。支持部门承认作者对旧版本的合法权利，但以“安全原因”不分发旧版本为由，拒绝提供安装程序。

这种拒绝使得“永久许可证”无法使用，迫使客户为访问已购买的软件而再次支付新订阅费用。作者认为，这项政策是出于经济动机而非安全考虑，因为支持部门立即提供了最新版本的折扣，而且在重装尝试之前，旧版本仍在接收更新。

文章还澄清，FileZilla与Mozilla没有关联，这是作者最初的误解，导致其产生了错误的信任。文章警告正在考虑FileZilla Pro的用户，“永久许可证”可能无法保证他们能够重新安装其合法拥有的产品。

---

## 58. 虎式：编程哲学 (2024)

**原文标题**: Tiger Style: Coding philosophy (2024)

**原文链接**: [https://tigerstyle.dev/](https://tigerstyle.dev/)

虎式风格是一种编码理念，专注于安全性、性能和开发者体验，灵感来源于TigerBeetle的工程实践。它旨在通过严谨的方法构建健壮、高效、可维护的软件。

核心原则强调：
*   **安全性：** 通过使用简单的控制流、固定限制、简洁函数（不超过70行）、显式数据类型（例如u32）、静态内存分配、最小变量作用域、彻底的错误处理（断言、快速失败、将警告视为错误）以及避免隐式默认值，编写可靠、可预测的代码。
*   **性能：** 通过“餐巾纸计算”估算、批处理操作以及优化资源使用（网络、磁盘、内存、CPU），在早期设计阶段就注重效率。它还提倡使用可预测的代码路径，以利用CPU缓存和分支预测。
*   **开发者体验：** 通过清晰、一致且描述性的命名（完整单词、单位/修饰符）、逻辑化的代码组织、简化的函数接口、确保一致性（无重复、按引用传递大型对象、整洁的缓冲区处理）、细致地防止“差一”错误以及标准化的工具和代码风格，促进可维护性和协作。

一项补充内容强化了这些原则，提倡“零技术债”，强调了第一次就把事情做对、积极主动地解决问题以及建立高质量、持久进展的重要性。通过“餐巾纸计算”进行的性能估算也作为一项至关重要的早期设计工具得到了强调。

---

## 59. 伊利亚·苏茨克维、杨立昆与“堆显卡”时代的终结

**原文标题**: Ilya Sutskever, Yann LeCun and the End of “Just Add GPUs”

**原文链接**: [https://www.abzglobal.net/web-development-blog/ilya-sutskever-yann-lecun-and-the-end-of-just-add-gpus](https://www.abzglobal.net/web-development-blog/ilya-sutskever-yann-lecun-and-the-end-of-just-add-gpus)

两位人工智能领军人物，Ilya Sutskever（OpenAI联合创始人，现任SSI负责人）和Yann LeCun（Meta首席人工智能科学家）均表示，当前的大型语言模型（LLM）和“规模化时代”正在触及极限。

Sutskever认为，人工智能正在从“规模化转向研究”。尽管海量算力和数据在2020-2025年间带来了突破，但收益递减、有限的高质量数据，以及基准性能与实际可靠性（幻觉、泛化能力差）之间的差距如今已显而易见。他的公司Safe Superintelligence Inc.致力于为超级智能发明新的训练方法和架构，坚称未来的进步需要更智能的算法，而不仅仅是更多的GPU。

LeCun的观点更为激进，他将LLM称为对于真正的智能而言的“以产品为导向的死胡同”。他批评LLM对物理世界、因果关系的理解肤浅，以及其Token预测的简单本质。相反，他倡导“世界模型”，例如JEPA，它通过观察环境（例如视频）进行学习，以构建内部表征，从而实现持久记忆、推理和规划，类似于人类和动物的学习方式。

两人都同意，当前的规模化策略正在触及天花板。Sutskever建议通过更好的目标来演进现有神经网络，而LeCun则主张向世界模型进行范式转变。

对于开发者和创始人而言，这意味着单纯的GPU算力优势正在减弱。重点必须转向高质量领域数据、稳健的用户工作流、有效的反馈循环，并希望通过用例、用户体验和集成实现差异化。预计将出现更多样化的模型类型和混合系统，在其中，产品内的可靠性、推理和规划比追求基准分数更为重要。人工智能的下一个时代将由新的想法和更智能的算法定义，而不再仅仅是预测下一个Token。

---

## 60. Pixel 10 很可能因欧盟裁决而支持 AirDrop。

**原文标题**: AirDrop support for Pixel 10 likely exists because of the EU ruling

**原文链接**: [https://9to5google.com/2025/11/21/googles-airdrop-support-for-pixel-10-likely-exists-because-of-the-eus-apple-ruling/](https://9to5google.com/2025/11/21/googles-airdrop-support-for-pixel-10-likely-exists-because-of-the-eus-apple-ruling/)

谷歌Pixel 10意外获得了跨平台“隔空投送支持”，通过“快速分享”（Quick Share）功能，可以与iPhone安全地共享文件和照片。这一进展并非谷歌的独立举措，而是欧盟《数字市场法案》（DMA）的直接结果。

欧盟的裁决强制苹果在其最新的操作系统升级中采用可互操作的无线标准，特别是Wi-Fi联盟的Wi-Fi Aware标准。这取代了苹果此前用于连续互通（Continuity）功能的专有协议。因此，尽管苹果并未直接向安卓设备“开放”隔空投送，但其遵守DMA的举动，迫使其实现了一个标准，而安卓设备（从Pixel 10开始）现在可以利用该标准进行安全、类似原生体验的文件传输。

这一变化类似于欧盟对iPhone采用USB-C接口以及支持RCS信息标准的推动。文章指出，只要硬件支持Wi-Fi Aware，该功能就能保持安全性，并有望扩展到更多安卓用户。尽管如此，据报道苹果仍在寻求撤销DMA，因此文章也谨慎地指出，尽管可能性不大，但这项功能的未来仍可能受制于监管变化。

---

## 61. 珠子：编程代理的记忆升级

**原文标题**: Beads – A memory upgrade for your coding agent

**原文链接**: [https://github.com/steveyegge/beads](https://github.com/steveyegge/beads)

Beads (bd) 是一款轻量级、基于图的问题追踪器，被设计为AI编码代理的“内存升级”。它旨在通过使代理能够可靠地管理复杂、长期任务，保持条理并避免工作丢失来解决它们的“健忘症”。

0.20.1版本引入了一项重大变更：基于哈希的问题ID（例如`bd-a1b2`）取代了顺序编号。这消除了多代理或多分支工作流程中常见的合并冲突和碰撞问题，使并行开发变得可靠。ID长度根据数据库大小进行渐进式扩展。

Beads作为一个分布式数据库运行，它看似集中，但通过Git实现其功能。它使用本地SQLite缓存以实现快速操作，并将`.beads/beads.jsonl`提交到Git作为唯一真实来源。自动同步机制使本地数据库与Git保持同步，在没有服务器或守护进程的情况下，跨机器提供共享状态。

主要功能包括四种依赖关系追踪类型（阻塞、关联、父子、发现自）、自动检测准备就绪的工作、代理友好的JSON输出、Git版本控制、用于多代理协作的可选实时“代理邮件”，以及完整的审计追踪。

人类用户通过`bd init`启动，但代理主要负责提交、更新和管理问题，主动记录发现的问题。用户可以使用`bd list`或`bd ready`等命令监控进度。Beads正处于活跃的alpha开发阶段，兼容Linux (glibc 2.32+)、macOS和Windows，可通过`curl`、`npm`或Homebrew轻松安装。

---

## 62. 保护公立学校学生免受校外言论监视

**原文标题**: Protect Public School Students from Surveillance of Off-Campus Speech

**原文链接**: [https://www.eff.org/deeplinks/2025/11/eff-arizona-federal-court-protect-public-school-students-surveillance-and](https://www.eff.org/deeplinks/2025/11/eff-arizona-federal-court-protect-public-school-students-surveillance-and)

电子前沿基金会（EFF）在*Merrill 诉 Marana 联合学区*一案中提交了一份法庭之友简报，倡导公立学校学生免受持续监控的言论自由和隐私权。该案件涉及一名学生，他因在校前使用学校发放的Chromebook起草了一则已删除的校外笑话，被Gaggle监控软件标记后遭到停学。学区辩称，使用学校发放的设备或账户自动将学生言论视为“校内”言论，从而为纪律处分提供了正当理由。

EFF认为这种解释存在缺陷，并引用了最高法院的裁决，包括*Tinker*案（校内言论若造成扰乱则可受处罚）和*Mahanoy*案（学校对校外言论的管辖权较弱，承认学生24小时的言论权）。EFF辩称，该学生的笑话发生在校外，与学校没有足够的关联，且不构成可信威胁。

简报强调了数字言论与隐私之间的关联，坚称对学校管理的科技设备实行一概而论的“校内”规则将严重损害学生利益。此类规则将：
1.  消除学生的任何私人空间，这与*Mahanoy*案中关于不应规制所有学生言论的警告相悖。
2.  造成寒蝉效应，导致学生进行自我审查。
3.  加剧社会经济差距，制造一种“为隐私付费”的系统，其中依赖学校设备的低收入学生将面临更严格的监控。
4.  鼓励侵入性和不准确的数字监控技术发展，导致不必要的调查并侵蚀学生隐私。

EFF敦促法院驳回这种宽泛的观点，强调学生需要一个数字自主空间，用于表达、身份认同发展和学习，从而免受学校持续监控和惩罚。

---

## 63. 为什么强一致性？

**原文标题**: Why Strong Consistency?

**原文链接**: [https://brooker.co.za/blog/2025/11/18/consistency.html](https://brooker.co.za/blog/2025/11/18/consistency.html)

马克·布鲁克的博客文章《为什么是强一致性？》指出，在规模化数据库架构中常见的最终一致性，是给客户和应用程序开发者带来巨大困扰并阻碍有效扩展的一个重要原因。

他通过一个例子强调了客户所面临的困扰：如果读取请求被路由到一个滞后的副本，那么创建资源后立即尝试检索它可能会失败（显示“ID不存在”）。这迫使开发者实施复杂且容易出错的变通方案，例如重试循环；但如果后续读取请求命中不同但同样过时的副本（缺乏“单调读”），这些方案仍然可能失败。

对于应用程序开发者而言，最终一致性使常见工作流变得复杂。涉及多次读写操作（例如，清理附件）可能会导致各种错误，如陈旧数据、不完整操作或断言失败，因为不同的读取请求可能会返回不一致的数据视图。这使得将敏感读取请求路由到主数据库成为必要，从而削弱了只读副本的用途。

此外，最终一致性使得“读-修改-写”工作负载的扩展变得更加困难。如果`UPDATE`语句的读取部分使用了来自副本的陈旧数据，那么对主数据库的写入可能会不正确。而Aurora DSQL中实现的强一致性，则允许任何副本用于读取，即使在读写事务中也能如此，从而避免了这些问题。

Aurora DSQL通过确保所有存储副本都从单调日志处理更新来实现强一致性。当查询处理器启动一个事务时，它会选择一个时间戳（`τ_start`）。副本会阻止读取请求，直到它们处理完截至该`τ_start`的所有更新，从而保证数据的一致性。

总之，尽管最终一致性有其适用之处，但布鲁克认为强一致性极大地简化了开发，使应用程序开发者和最终用户免于处理大规模分布式系统固有的复杂性。

---

## 64. 瑞典出版商就诈骗行为向警方报案，控告Meta的扎克伯格。

**原文标题**: Swedish publishers file police report against Meta's Zuckerberg for fraud

**原文链接**: [https://www.sverigesradio.se/artikel/swedish-publishers-file-police-report-against-metas-zuckerberg-for-fraud](https://www.sverigesradio.se/artikel/swedish-publishers-file-police-report-against-metas-zuckerberg-for-fraud)

瑞典出版商协会已报警，指控Meta创始人马克·扎克伯格欺诈。

---

## 65. 男女最主要的住院原因

**原文标题**: The most male and female reasons to end up hospital

**原文链接**: [https://leobenedictus.substack.com/p/the-most-male-and-female-reasons](https://leobenedictus.substack.com/p/the-most-male-and-female-reasons)

Leo Benedictus的这篇文章基于2021-22年度英国国民医疗服务体系（NHS）的数据，探讨了男性与女性住院的截然不同原因。文章强调，在急诊入院（不包括与妊娠相关的入院）中存在明显的性别模式。

女性急诊住院最主要的常见原因绝大多数与**腹部和盆腔疼痛**、**泌尿道感染（UTIs）**以及**恶心/呕吐**有关。这些病症通常伴有需要紧急医疗关注的症状，但住院时间通常较短。

对男性而言，急诊入院的主要原因是**胸痛**、**腹部和盆腔疼痛**以及**心力衰竭**。尤其是胸痛，常因担心心脏问题而导致就医，即使不总是能发现严重的病因。心力衰竭也是男性入院的一个重要原因。

文章指出，尽管“腹部和盆腔疼痛”是男女共有的主要原因，但其根本原因往往不同。总体而言，这揭示了各种生物学、社会和行为因素如何导致男女之间存在不同的紧急医疗保健需求。

---

## 66. 斯泰兰蒂斯正向车主车载屏幕滥发新车优惠弹窗广告。

**原文标题**: Stellantis Is Spamming Owners' Screens with Pop-Up Ads for New Car Discounts

**原文链接**: [https://www.thedrive.com/news/stellantis-is-spamming-owners-screens-with-pop-up-ads-for-new-car-discounts](https://www.thedrive.com/news/stellantis-is-spamming-owners-screens-with-pop-up-ads-for-new-car-discounts)

斯泰兰蒂斯（Stellantis）因直接向车主车载信息娱乐屏幕推送弹窗营销广告（例如1500美元的忠诚度折扣）而招致了大量的网络批评。经一名Jeep司机和斯泰兰蒂斯证实，这一做法并非新鲜事，今年早些时候也曾出现过类似的延长保修广告。

尽管斯泰兰蒂斯旗下多个品牌（如Jeep、克莱斯勒和Ram）的许多车主正在谴责这一举动并威胁抵制该公司，但也有一些人，如汽车作家Zerin Dube，却利用了这些优惠。Dube在关于该广告的病毒式帖子中强调了“晚期资本主义”，但他最终利用了这一折扣，以大幅度的总节省购买了一辆新的Jeep牧马人，这表明该策略对他而言“奏效了”。

斯泰兰蒂斯为这些通知辩护，称其旨在关键时刻与车主“保持联系”，并且也用于召回目的。该公司澄清说，这些文本信息只在启动时和车辆静止时显示，并在15秒后或驾驶员互动后消失。它们仅在选择“稍后提醒我”选项或未处理时才会重新出现。斯泰兰蒂斯指出客户对这些优惠的接受度，并确认车主可以通过拨打其客户服务热线（800-777-3600）永久选择退出。这种情况引发了关于互联汽车用户体验的更广泛疑问，尤其考虑到过去的问题，即之前的广告活动更具侵扰性。

---

## 67. Show HN: SyncKit — 离线优先同步引擎 (Rust/WASM 和 TypeScript)

**原文标题**: Show HN: SyncKit – Offline-first sync engine (Rust/WASM and TypeScript)

**原文链接**: [https://github.com/Dancode-188/synckit](https://github.com/Dancode-188/synckit)

SyncKit 是一个生产就绪的离线优先同步引擎，基于 Rust/WASM 和 TypeScript 构建，旨在简化本地优先应用程序的创建。它通过仅需几行代码提供自动、实时同步和内置冲突解决（最后写入获胜），解决了现有解决方案（如 Yjs、Firebase 或 Supabase）的复杂性、成本和离线限制。

v0.1.0 的主要特性包括真正的离线优先架构、实时协作、IndexedDB 持久化和跨标签页同步。SyncKit 提供了紧凑的打包大小（gzip 压缩后约 59KB，精简版约 45KB）、快速本地操作（<1 毫秒）和低同步延迟（<100 毫秒）。它是开源的，可自行托管，确保数据主权，并通过形式验证和广泛测试保证数据完整性。

相比之下，SyncKit 提供了优于 Firebase 和 Supabase 的原生离线能力，提供基于 WASM 的多语言服务器支持（与 Yjs 不同），并在打包大小、性能和生产就绪方面优于 Automerge。

即将推出的 v0.2.0 特性包括用于协同编辑的文本 CRDTs、计数器、集合、更多框架适配器（Vue、Svelte）和多语言服务器实现。通过 npm 即可简单安装，并提供直观的 React Hooks。SyncKit 将自身定位为一个强大、高性能、灵活的选择，适用于要求真正离线功能和无缝协作的现代应用程序。

---

## 68. 瑞士：数据保护官对当局颁布广泛云禁令

**原文标题**: Switzerland: Data Protection Officers Impose Broad Cloud Ban for Authorities

**原文链接**: [https://www.heise.de/en/news/Switzerland-Data-Protection-Officers-Impose-Broad-Cloud-Ban-for-Authorities-11093477.html](https://www.heise.de/en/news/Switzerland-Data-Protection-Officers-Impose-Broad-Cloud-Ban-for-Authorities-11093477.html)

瑞士数据保护机构，由联邦数据保护和信息专员（FDPIC）以及各州/市机构牵头，发布了严格的建议，有效禁止公共机构使用云服务。这项禁令尤其针对受外国法律（例如美国《云法案》）约束的服务提供商。

核心顾虑在于，当外国当局可能在数据所有者不知情或未经同意的情况下访问数据时，无法保证充分的数据保护。当局声明，目前的合同条款和技术保障措施不足以降低这些风险。他们建议公共机构只使用明确受瑞士法律管辖的云服务提供商，且所有数据处理和存储都必须完全在瑞士境内进行。即使是瑞士提供商，也需要进行彻底审查，以确保其真正独立于外国控制。

公共机构现有的云部署必须接受审查，如果发现不合规，则必须进行调整或终止。尽管在数据处理完全透明、可控且数据主体提供明确知情同意的情况下，极少数例外情况可能存在，但这对于大多数政府数据而言通常是不切实际的。此举凸显了瑞士对数据主权的承诺，也呼应了欧盟此前提出的类似担忧。

---

## 69. 承载 44 年 Unix 演进的存储库

**原文标题**: A Repository with 44 Years of Unix Evolution

**原文链接**: [https://www.spinellis.gr/pubs/conf/2015-MSR-Unix-History/html/Spi15c.html](https://www.spinellis.gr/pubs/conf/2015-MSR-Unix-History/html/Spi15c.html)

本文介绍了一个Git仓库，它记录了Unix操作系统44年的演进历程，从1972年最初5,000行代码的内核，到2015年2,600万行代码的系统。这个在MSR '15大会上荣获“最佳数据展示”奖的GitHub仓库，包含了659,000次提交和2,306次合并，并识别出850名贡献者。

该项目旨在为软件工程和软件考古学的实证研究提供一个统一的、现代的版本控制系统。它整合了来自24个历史快照（贝尔实验室、伯克利、386BSD）、两个旧版仓库（CSRG SCCS、FreeBSD 1 CVS）以及现代FreeBSD Git仓库的数据。早期贡献的作者身份通过细致的一手研究得以确定，这些研究包括查阅历史文献和与原始开发者进行沟通。

该仓库的构建使得使用`git blame`命令进行精确的代码来源追溯成为可能，揭示了早至1974年的代码行至今仍存在于现代Unix中。快照是按顺序导入的，之前的版本中的文件会被临时移动到一个隐藏目录，以保持`git blame`的历史连续性。这一全面的数字资料为研究一个基础软件系统的长期发展提供了宝贵的资源。

---

## 70. 樱桃放弃德国生产并打算出售核心部门。

**原文标题**: Cherry gives up German production and wants to sell core division

**原文链接**: [https://www.heise.de/en/news/Cherry-gives-up-German-production-and-wants-to-sell-core-division-11092713.html](https://www.heise.de/en/news/Cherry-gives-up-German-production-and-wants-to-sell-core-division-11092713.html)

樱桃（Cherry），这家以机械键盘轴闻名的德国制造商，正在经历重大重组。该公司已宣布出售其“轴体”业务部门，该部门涵盖其核心MX轴体及其他键盘轴体的生产，以及位于德国奥尔巴赫的配套生产设施。此举旨在专注于盈利能力，并战略性地转向其“外设”业务部门，该部门包括成品键盘、鼠标及其他输入设备。

尽管轴体部门是Cherry的历史支柱，但由于高昂的人力成本及其德国工厂日益增长的自动化，该部门在盈利方面一直举步维艰。尽管该部门近期销售额有所回升，但Cherry管理层认为，将其剥离将有助于实现更专注的增长和投资，可能在新所有权下，新所有者能更好地应对其特有挑战。

出售流程已在进行中，目前正在评估意向方。Cherry目标是在2024年中期之前完成此交易。出售完成后，Cherry将只专注于其外设部门，旨在利用其品牌知名度在这个不断增长的市场中。此次战略调整标志着该公司的一个重要转折点，有效终止了其在德国生产标志性MX轴体的历史。

---

## 71. 为什么90年代电影比Netflix上的一切都更生动？

**原文标题**: Why 90s Movies Feel More Alive Than Anything on Netflix

**原文链接**: [https://afranca.com.br/why-90s-movies-feel-more-alive-than-anything-on-netflix](https://afranca.com.br/why-90s-movies-feel-more-alive-than-anything-on-netflix)

文章认为，90年代的电影比当今许多电影，特别是流媒体内容，更“鲜活”且更具影响力。作者以《沉默的羔羊》、《好家伙》和《低俗小说》等电影为例，认为早期的电影在创作上更有目的性，角色塑造更深入，并且更敢于冒险。

《好家伙》因其沉浸式的叙事和有目的性的场景而备受赞誉，这与一些现代电影被认为的“臃肿”形成了对比。《低俗小说》创新的叙事结构和真实的对话被突出强调，这与当代电影“用力过猛”的自作聪明形成了反差。《沉默的羔羊》展现了心理深度和引人入胜的角色互动，而作者认为现代惊悚片缺乏这些。

作者认为，核心区别在于，早期电影信任观众，并赋予导演艺术自由，让他们能够创作“电影，而非产品”。相比之下，现代电影常常感觉是“委员会设计”的，为算法和快速消费而优化，而非追求持久的影响力。作者总结道，尽管技术进步，但当今电影不过是消磨时间，很快被遗忘，这与90年代经典电影的持久共鸣截然不同。

---

## 72. VPN恐慌才刚刚开始

**原文标题**: The VPN panic is only getting started

**原文链接**: [https://www.theverge.com/tech/827435/uk-vpn-restrictions-ban-online-safety-act](https://www.theverge.com/tech/827435/uk-vpn-restrictions-ban-online-safety-act)

英国于2023年7月实施的《网络安全法》(OSA)要求对访问在线“有害材料”（包括色情内容和宣扬自残的内容）进行严格的年龄验证。然而，用户很快发现，虚拟私人网络（VPN）通过伪造来自其他国家的IP地址，有效地规避了这些检查。这导致英国VPN使用量大幅增长，一些供应商报告称注册量增长高达1800%。

这种规避行为引发了采取行动的呼吁。儿童事务专员雷切尔·德·苏萨 (Rachel de Souza) 将VPN访问称为“需要堵塞的漏洞”，建议VPN本身应接受与它们试图规避的相同年龄验证。英国媒体监管机构Ofcom正在“监测VPN的使用”，但否认追踪个人。

尽管政府目前的立场是“目前没有计划禁止使用VPN”，因为其有合法用途（例如商业安全、新闻记者隐私），但他们也表示“一切皆有可能”。专家们普遍认为，全面禁止将是技术上复杂且在很大程度上无效的。

替代解决方案包括要求受OSA覆盖的网站屏蔽VPN流量，这可能迫使网站放弃英国市场或全球所有VPN用户。最可能的结果是对VPN本身进行年龄限制。然而，这伴随着风险，可能将用户推向声誉不佳、隐私保护差的免费VPN，或风险更高的直接文件共享。

文章总结道，随着其他国家和美国各州效仿英国实施在线年龄限制，“VPN恐慌”以及关于其使用监管的辩论才刚刚在全球范围内开始。

---

## 73. 想搭建本地RAG吗？

**原文标题**: So you wanna build a local RAG?

**原文链接**: [https://blog.yakkomajuri.com/blog/local-rag](https://blog.yakkomajuri.com/blog/local-rag)

本文详细介绍了Skald如何构建一个完全本地化、隐私保护的RAG（检索增强生成）系统，从而消除对第三方云服务的依赖。其动机源于对无需外部数据共享的可自托管AI工具的需求，特别是对于对隐私敏感的组织而言。

一个标准的RAG系统由向量数据库、嵌入模型、大语言模型（LLM）、重排序器和文档解析器组成。对于本地化部署，专有的云服务必须替换为开源或自托管的替代方案。Skald选择的本地技术栈包括：
*   **向量数据库：** 带有pgvector的Postgres
*   **向量嵌入：** Sentence Transformers (all-MiniLM-L6-v2) 和 bge-m3
*   **大语言模型：** 用户自行管理（通过llama.cpp测试了GPT-OSS 20B）
*   **重排序器：** Sentence Transformers交叉编码器 和 mmarco-mMiniLMv2-L12-H384-v1
*   **文档解析：** Docling

基准测试使用PostHog网站数据和自定义问题数据集进行。
1.  **云端基线（Voyage + Claude）：** 平均得分9.45，所有答案均正确。
2.  **混合方案（Voyage + GPT-OSS 20B）：** 得分9.18，显示了开源大语言模型的强大性能。
3.  **全本地化方案（默认Sentence Transformers + GPT-OSS 20B）：** 得分7.10。虽然对英语点式查询表现良好，但在处理多语言问题、歧义以及聚合来自多个文档的信息方面表现不佳。
4.  **全本地化方案（多语言bge-m3/mmarco + GPT-OSS 20B）：** 提升至8.63分，能很好地处理多语言查询，但仍面临复杂信息聚合的挑战。

作者总结道，全本地化RAG是可行的，在许多用例中表现良好，并且随着更好的开源模型不断改进。未来的工作将侧重于优化复杂查询的聚合能力，并发布更全面的基准测试。

---

## 74. Mixpanel近期安全事件须知

**原文标题**: What to know about a recent Mixpanel security incident

**原文链接**: [https://openai.com/index/mixpanel-incident](https://openai.com/index/mixpanel-incident)

无法访问文章链接。

---

## 75. Imgur 对英国实施地域限制，我则突破了网络的地域限制

**原文标题**: Imgur Geo-Blocked the UK, So I Geo-Unblocked My Network

**原文链接**: [https://blog.tymscar.com/posts/imgurukproxy/](https://blog.tymscar.com/posts/imgurukproxy/)

本文介绍了作者如何通过部署一个透明的、网络范围的代理解决方案，绕过Imgur在英国的地理限制。尽管作者不常用Imgur，但不断遇到损坏的图片链接（例如Minecraft着色器）变得很烦人。作者排除了使用个人VPN的方案，因为这可能会降低其2.5 Gbps互联网的速度，并且在每台设备（手机、笔记本电脑、台式机）上安装和管理VPN客户端也很不方便。

相反，作者利用现有的家庭实验室组件构建了一个网络层面的解决方案：使用Pi-hole进行DNS解析，Traefik作为反向代理，以及NixOS进行声明式配置。该过程如下：
1. 网络上的任何设备请求 `i.imgur.com`。
2. Pi-hole拦截此DNS请求并返回本地Traefik实例的IP地址。
3. Traefik配置为TCP直通模式，检查SNI（服务器名称指示），并将连接路由到 `gluetun` Docker容器。
4. `Gluetun` 建立与非英国服务器的WireGuard VPN连接。
5. 一个 `nginx` 容器，配置为共享 `gluetun` 的网络栈，充当简单的TCP直通代理，通过VPN将请求转发到 `i.imgur.com`。
6. 图像随后通过VPN隧道返回到原始设备。

Nginx在 `gluetun` 的网络中使用，因为 `gluetun` 提供的是VPN连接性，而非代理功能。整个Docker设置由NixOS声明式管理，敏感的VPN凭据通过Agenix保护。

这种设置提供了一个无缝的、网络范围的解决方案，适用于所有设备，无需任何客户端配置。Imgur访问得以恢复，且仅对受影响的流量产生可忽略不计的延迟增加，这既满足了实际需求，也满足了“家庭实验室折腾欲”。

---

## 76. 如何使用 Linux vsock 实现高速虚拟机通信

**原文标题**: How to use Linux vsock for fast VM communication

**原文链接**: [https://popovicu.com/posts/how-to-use-linux-vsock-for-fast-vm-communication/](https://popovicu.com/posts/how-to-use-linux-vsock-for-fast-vm-communication/)

本文演示了如何使用 Linux `vsock` 实现虚拟机 (VM) 及其宿主机之间的高效通信，特别是将其用作 gRPC 服务的传输方式。`Vsock` 是一种虚拟机专用技术，无需传统的 TCP/IP 协议栈或网络虚拟化，其行为类似于标准套接字，但采用专用的寻址方案。

作者的动机是为密封的 VM 环境实现快速 RPC 通信。该实验展示了一个使用 C++ 实现并用 Bazel 构建的简单 gRPC“加法”服务。

**关键步骤**：
1.  **gRPC 服务定义**：一个 `proto` 文件定义了一个包含 `Addition` RPC 的 `VsockService`，该 RPC 接受两个整数并返回它们的和。
2.  **服务器实现**：一个静态链接的 C++ 服务器二进制文件设计用于在 VM 内部运行。它监听 `vsock:3:9999`，其中 `3` 是 VM 的上下文 ID (CID)，`9999` 是端口。CID -1 (VMADDR_CID_ANY) 允许来自任何 CID 的连接。
3.  **客户端实现**：一个静态链接的 C++ 客户端二进制文件在宿主机上运行。它连接到 `vsock:3:9999` 上的 VM 服务器。
4.  **VM 设置**：使用 `debootstrap` 创建一个 Debian VM 镜像。预构建的服务器二进制文件放置在 `/opt` 中，并在启动时作为 `init` 进程执行。
5.  **QEMU 配置**：使用 QEMU 启动 VM，并附加一个 `guest-cid=3` 的 `vhost-vsock-pci` 设备以启用 vsock 功能。
6.  **执行**：宿主机上的客户端成功调用了 VM 服务器上的 `Addition` RPC，展示了无需网络虚拟化的宿主机到 VM 通信。

文章总结道，通过 `vsock` 使用 gRPC 提供了一种强大的方式来构建隔离应用程序、结合不同的操作系统，并实现高效的 VM/宿主机间通信，得益于 gRPC 的语言独立性和 `vsock` 的原生效率。

---

## 77. 通用人工智能十年内也不可能实现。

**原文标题**: AGI is not possible even in 10 years

**原文链接**: [https://medium.com/@anwarzaid76/agi-is-not-possible-even-in-10-years-013a1aec0d9c](https://medium.com/@anwarzaid76/agi-is-not-possible-even-in-10-years-013a1aec0d9c)

无法访问文章链接。

---

## 78. 你为何在工作时无法专注的数学

**原文标题**: The Math of Why You Can't Focus at Work

**原文链接**: [https://justoffbyone.com/posts/math-of-why-you-cant-focus-at-work/](https://justoffbyone.com/posts/math-of-why-you-cant-focus-at-work/)

本文通过数学建模解释了工作注意力下降的原因，并将其归因于数字化干扰的增加。文章引入了三个核心参数：
1.  **λ (lambda)：中断率**（每小时中断次数）。这反映了人们因消息、会议或快速提问而分心的频率。
2.  **Δ (delta)：恢复期**（恢复专注所需分钟数）。每次中断后，大脑需要时间重新加载上下文，这并非为零，而且可能相当长。
3.  **θ (theta)：专注阈值**（进行有意义工作所需的最小不间断时间）。这是被认为高效的最小时间块；低于此阈值的碎片时间几乎无法产生实际产出。

基于这些参数，文章将“产能”定义为所完成的有意义工作单元的总和，并论证了即使总专注时间很长，但由于模型中“无情”的向下取整函数（地板函数），如果时间块过短，也会导致产能低下。通过100天的模拟，文章阐明了这些参数的变化如何显著影响整体生产力。研究数据证实了现实世界中高中断率（高达每2-3分钟一次）以及漫长的恢复时间（10-16分钟），凸显了现代工作场所中深度工作面临的严峻挑战。

---

## 79. Show HN: MkSlides——Markdown 转幻灯片，工作流与 MkDocs 类似

**原文标题**: Show HN: MkSlides – Markdown to slides with a similar workflow to MkDocs

**原文链接**: [https://github.com/MartenBE/mkslides](https://github.com/MartenBE/mkslides)

MkSlides 是一个静态网站生成器，旨在将 Markdown 文件转换为由 Reveal.js 驱动的引人入胜的幻灯片，效仿 MkDocs 的工作流程。它使用户能够将单个 Markdown 文件或整个文件夹转换为静态 HTML 幻灯片，包括一个可选的集合索引着陆页。

主要功能包括轻松部署到任何静态文件服务器（本地、网络服务器、CI/CD）、编辑时的实时预览模式以及广泛的自定义功能。用户可以应用现有的 Reveal.js 和 Highlight.js 主题，定义自定义 CSS、网站图标和模板，并受益于表情符号支持。示例还突出显示了 Mermaid.js 和 PlantUML 集成等高级功能。

安装非常简单，只需运行 `pip install mkslides`。要生成静态输出，请使用 `mkslides build [PATH]`，其中 `PATH` 可以是目录（默认为 `slides/` 或 `docs/`）或单个 Markdown 文件。对于实时开发，`mkslides serve [PATH]` 提供实时更新。使用单个 Markdown 文件时，请注意只会复制默认的静态资源；对于图片和其他文件，建议采用文件夹结构。

配置通过 `mkslides.yml` 文件进行处理，允许对索引页和单个幻灯片进行详细控制，包括主题、标题、`revealjs` 选项和插件集成。至关重要的是，Markdown 文件前置元数据中定义的设置会覆盖 `mkslides.yml` 中的设置，而 `mkslides.yml` 中的设置又会覆盖默认设置，从而提供灵活的自定义功能。

---

## 80. 中国三枚可重复使用火箭已整装待发，将进行首飞。

**原文标题**: China Has Three Reusable Rockets Ready for Their Debut Flights

**原文链接**: [https://www.china-in-space.com/p/china-has-three-reusable-rockets](https://www.china-in-space.com/p/china-has-three-reusable-rockets)

中国正准备在年底前进行三枚部分可重复使用火箭的首飞，这三枚火箭目前均已抵达酒泉卫星发射中心。它们包括国有上海航天技术研究院的长征十二号A、蓝箭航天的朱雀三号和空间先锋的天龙三号。

长征十二号A和朱雀三号均采用液态甲烷和液氧推进剂，其一级火箭设计通过栅格舵引导进行动力着陆。长征十二号A的目标近地轨道载荷量为12,000公斤，而朱雀三号的目标载荷量为11,800公斤。蓝箭航天的朱雀三号已完成了非常成功的测试活动，包括10公里跳跃测试，使其成为中国首次可重复使用火箭飞行的主要竞争者。

空间先锋的天龙三号是一枚液氧煤油火箭，提供最大的17,000公斤近地轨道载荷能力，也计划进行一级火箭着陆，尽管其首飞火箭上尚未安装可重复使用硬件。

其中一枚火箭将实现中国首次可重复使用火箭着陆，使其成为全球第三个、美国以外的第一个。据报道，蓝箭航天的朱雀三号计划于11月下旬首飞。这些可重复使用火箭对中国雄心勃勃的巨型星座部署至关重要，有望实现更低成本和更频繁的发射任务。

---

## 81. 别拽那个，谁知道它会连着什么呢 (2016)

**原文标题**: Don't tug on that, you never know what it might be attached to (2016)

**原文链接**: [https://blog.plover.com/2016/07/01/#tmpdir](https://blog.plover.com/2016/07/01/#tmpdir)

这篇文章详细描述了一个令人沮丧的bug，即`emacsclient`无法连接到Emacs服务器。核心问题是`emacsclient`在`/mnt/tmp/emacs2017/server`中寻找服务器套接字，而Emacs却在`/tmp/emacs2017/server`中创建它。这种差异被追溯到`TMPDIR`环境变量，它当时被设置为`/mnt/tmp`。

最初，人们怀疑Emacs没有遵循`TMPDIR`。然而，通过仔细测试发现，当Emacs直接启动时，它确实遵循了该变量。问题出现在通过Git中的自定义Perl脚本（`git-re-edit`）间接调用Emacs时。排除了Git的嫌疑后，作者发现Perl本身清除了`TMPDIR`环境变量，这一点通过简单的`perl -le 'print $ENV{TMPDIR}'`返回空字符串得到了证实。

在调查过程中，实施了两种变通方案：
1. 将Emacs配置为使用TCP套接字而不是Unix域套接字。
2. 在shell配置文件中手动设置`EMACS_SERVER_SOCKET`环境变量，作者的`also`脚本使用`--socket-name`参数将其传递给`emacsclient`。

最终的解释（后来由其他人发现）是，动态加载器在加载Perl时，会清除`TMPDIR`作为一项安全措施。这可以防止潜在的攻击，即程序（尤其是具有提升权限的程序）可能通过恶意的`TMPDIR`设置被操纵，将临时文件写入敏感位置。

---

## 82. Collabora Online Desktop Released with Improved UI from LibreOffice

**原文标题**: Collabora Online Desktop Released with Improved UI from LibreOffice

**原文链接**: [https://www.collaboraonline.com/blog/collabora-online-now-available-on-desktop/](https://www.collaboraonline.com/blog/collabora-online-now-available-on-desktop/)

一份新闻稿宣布“Collabora Online Desktop”正式发布。此新版本的一大亮点在于将 Collabora Online 功能引入桌面环境，其改进的用户界面借鉴了 LibreOffice 的增强功能。

---

## 83. 苹果英特尔传将合作Mac芯片

**原文标题**: Apple and Intel Rumored to Partner on Mac Chips

**原文链接**: [https://www.macrumors.com/2025/11/28/intel-rumored-to-supply-new-mac-chip/](https://www.macrumors.com/2025/11/28/intel-rumored-to-supply-new-mac-chip/)

Apple and Intel are rumored to be rekindling their partnership, with Intel potentially manufacturing Apple's lowest-end M-series chips starting mid-2027. According to supply chain analyst Ming-Chi Kuo, Intel would utilize its advanced 18A process (sub-2nm) to produce these chips, which could power future MacBook Air, iPad Air, and iPad Pro models.

Unlike their previous collaboration where Intel designed x86 processors for Macs, this new arrangement would see Intel solely manufacturing Apple's custom-designed, ARM-based M-series chips. TSMC would continue to be the primary supplier for most of Apple's M-series chips.

Kuo suggests Apple's motivations for this move include diversifying its manufacturing supply chain and potentially aligning with "Made in USA" product initiatives. This development follows Apple's complete transition away from Intel processors in Macs, a process that began in 2020. macOS Tahoe is also noted as the final major macOS release supporting Intel-based Macs.

---

## 84. Bonsai_term：Jane Street 开发的动态终端应用构建库

**原文标题**: Bonsai_term: A library for building dynamic terminal apps by Jane Street

**原文链接**: [https://github.com/janestreet/bonsai_term](https://github.com/janestreet/bonsai_term)

生成摘要时出错

---

## 85. 受蜘蛛侠启发，科学家重现蛛丝发射技术

**原文标题**: Inspired by Spider-Man, scientists recreate web-slinging technology

**原文链接**: [https://scienceclock.com/inspired-by-spider-man-scientists-recreate-web-slinging-technology/](https://scienceclock.com/inspired-by-spider-man-scientists-recreate-web-slinging-technology/)

生成摘要时出错

---

## 86. 最后一期《ECMAScript 新闻》

**原文标题**: Last Issue of "ECMAScript News"

**原文链接**: [https://ecmascript.news/archive/es-next-news-2025-11-26.html](https://ecmascript.news/archive/es-next-news-2025-11-26.html)

"ECMAScript News" has announced that its current issue is its last. The newsletter, which launched on September 27, 2016, and published 368 issues, is ceasing publication due to prolonged financial losses. The number of advertisers and subscribers has steadily declined over the past two years, making the operation unsustainable despite previous growth. The publishers expressed gratitude to their loyal readers. There is a possibility that Axel, a contributor, may continue the newsletter in a new format next year, with an update to be sent via email in 2026 if this occurs.

---

## 87. Google denies 'misleading' reports of Gmail using your emails to train AI

**原文标题**: Google denies 'misleading' reports of Gmail using your emails to train AI

**原文链接**: [https://www.theverge.com/news/826902/gmail-ai-training-data-opt-out](https://www.theverge.com/news/826902/gmail-ai-training-data-opt-out)

生成摘要时出错

---

## 88. GrapheneOS Moving Out of France

**原文标题**: GrapheneOS Moving Out of France

**原文链接**: [https://xcancel.com/GrapheneOS/status/1993035936800584103](https://xcancel.com/GrapheneOS/status/1993035936800584103)

生成摘要时出错

---

## 89. DSP 101 Part 1: An Introductory Course in DSP System Design

**原文标题**: DSP 101 Part 1: An Introductory Course in DSP System Design

**原文链接**: [https://www.analog.com/en/resources/analog-dialogue/articles/dsp-101-part-1.html](https://www.analog.com/en/resources/analog-dialogue/articles/dsp-101-part-1.html)

生成摘要时出错

---

## 90. New research highlights a shortage of male mentors for boys and young men

**原文标题**: New research highlights a shortage of male mentors for boys and young men

**原文链接**: [https://www.psypost.org/new-research-highlights-a-shortage-of-male-mentors-for-boys-and-young-men/](https://www.psypost.org/new-research-highlights-a-shortage-of-male-mentors-for-boys-and-young-men/)

生成摘要时出错

---

## 91. Show HN: Era – Open-source local sandbox for AI agents

**原文标题**: Show HN: Era – Open-source local sandbox for AI agents

**原文链接**: [https://github.com/BinSquare/ERA](https://github.com/BinSquare/ERA)

生成摘要时出错

---

## 92. True P2P Email on Top of Yggdrasil Network

**原文标题**: True P2P Email on Top of Yggdrasil Network

**原文链接**: [https://github.com/JB-SelfCompany/Tyr](https://github.com/JB-SelfCompany/Tyr)

生成摘要时出错

---

## 93. Seagate achieves 6.9TB storage capacity per platter

**原文标题**: Seagate achieves 6.9TB storage capacity per platter

**原文链接**: [https://www.tomshardware.com/pc-components/hdds/seagate-achieves-a-whopping-6-9tb-storage-capacity-per-platter-in-its-laboratory-55tb-to-69tb-hard-drives-now-physically-possible](https://www.tomshardware.com/pc-components/hdds/seagate-achieves-a-whopping-6-9tb-storage-capacity-per-platter-in-its-laboratory-55tb-to-69tb-hard-drives-now-physically-possible)

生成摘要时出错

---

## 94. Steam 代表俄罗斯政府审查 LGBTQ+ 内容

**原文标题**: Steam censors LGBTQ+ content on behalf of the Russian Government

**原文链接**: [https://www.videogamesindustrymemo.com/p/how-steam-censors-lgbtq-content-on](https://www.videogamesindustrymemo.com/p/how-steam-censors-lgbtq-content-on)

生成摘要时出错

---

## 95. Don't be a scary old guy: My 40s survival strategy with charm

**原文标题**: Don't be a scary old guy: My 40s survival strategy with charm

**原文链接**: [https://www.devas.life/dont-be-a-scary-old-guy-my-40s-survival-strategy-with-charm/](https://www.devas.life/dont-be-a-scary-old-guy-my-40s-survival-strategy-with-charm/)

生成摘要时出错

---

## 96. A Tale of Four Fuzzers

**原文标题**: A Tale of Four Fuzzers

**原文链接**: [https://tigerbeetle.com/blog/2025-11-28-tale-of-four-fuzzers/](https://tigerbeetle.com/blog/2025-11-28-tale-of-four-fuzzers/)

生成摘要时出错

---

## 97. $96M AUD revamp of Bom website bombs out on launch

**原文标题**: $96M AUD revamp of Bom website bombs out on launch

**原文链接**: [https://www.bbc.com/news/articles/c2k4dy15nqqo](https://www.bbc.com/news/articles/c2k4dy15nqqo)

生成摘要时出错

---

## 98. Shor's algorithm: the one quantum algo that ends RSA/ECC tomorrow

**原文标题**: Shor's algorithm: the one quantum algo that ends RSA/ECC tomorrow

**原文链接**: [https://blog.ellipticc.com/posts/what-is-shors-algorithm-and-why-its-the-single-biggest-threat-to-classical-cryptography/](https://blog.ellipticc.com/posts/what-is-shors-algorithm-and-why-its-the-single-biggest-threat-to-classical-cryptography/)

生成摘要时出错

---

## 99. Africa's forests have switched from absorbing to emitting carbon

**原文标题**: Africa's forests have switched from absorbing to emitting carbon

**原文链接**: [https://phys.org/news/2025-11-africa-forests-absorbing-emitting-carbon.html](https://phys.org/news/2025-11-africa-forests-absorbing-emitting-carbon.html)

生成摘要时出错

---

## 100. Cats became our companions way later than you think

**原文标题**: Cats became our companions way later than you think

**原文链接**: [https://www.bbc.co.uk/news/articles/cq8dvdp9gn7o](https://www.bbc.co.uk/news/articles/cq8dvdp9gn7o)

生成摘要时出错

---

