# Hacker News 热门文章摘要 (2025-11-22)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. CBP正在监控美国司机并拘留有可疑出行模式的人。

**原文标题**: CBP is monitoring US drivers and detaining those with suspicious travel patterns

**原文链接**: [https://apnews.com/article/immigration-border-patrol-surveillance-drivers-ice-trump-9f5d05469ce8c629d6fecf32d32098cd](https://apnews.com/article/immigration-border-patrol-surveillance-drivers-ice-trump-9f5d05469ce8c629d6fecf32d32098cd)

美国边境巡逻队运作着一项秘密的全国性项目，利用车牌识别器（LPR）监控数百万美国司机。算法会标记出具有“可疑”出行模式（起点、目的地、路线）的车辆，导致联邦或地方执法部门进行拦截，他们常常以轻微交通违规为借口，进行带有侵略性的盘问和搜查。

该系统最初旨在打击与边境相关的犯罪，但在五年内已扩展到美国腹地，其运作方式类似于国内情报行动。它与美国缉毒局（DEA）、私营公司和地方警察合作，利用全国范围的LPR网络，并准备整合人工智能。LPR设备通常隐藏在交通设备中，边境巡逻队对“可疑”的定义非常宽泛（例如，租车、前往边境地区的旅行）。该网络远远超出了边境地区，影响着凤凰城、底特律、芝加哥和休斯顿等主要城市。

法律学者对此提出第四修正案方面的担忧，称其为对普通美国人的“撒网式监控”。例子包括洛伦佐·古铁雷斯·卢戈（Lorenzo Gutierrez Lugo），他因超速（一个借口）被拦截，依据是边境巡逻队的情报，随后被审问并因洗钱指控被捕，但这些指控后来被撤销。类似地，亚历克斯·肖特（Alek Schott）在边境附近过夜旅行后被拦截搜查，但一无所获。这些“耳语”或“情报”拦截掩盖了联邦政府的参与，它们通常通过群聊进行协调，在群聊中，详细的司机信息被非正式地共享。尽管该项目在2017年获得授权用于临时调查，但它已发展成为一个广泛而永久的监控网络。

---

## 2. 助力Valve为Steam设备供电

**原文标题**: Helping Valve to power up Steam devices

**原文链接**: [https://www.igalia.com/2025/11/helpingvalve.html](https://www.igalia.com/2025/11/helpingvalve.html)

Igalia详细阐述了其对Valve新发布的Steam设备的广泛贡献：基于ARM的Steam Frame VR头显、Steam Machine主机和Steam控制器。他们在SteamOS上的工作对这些设备至关重要，特别是对Frame。

对于ARM驱动的Steam Frame，Igalia实施并完善了FEX转译层，通过转换机器码使x86 PC游戏能够在ARM芯片上运行。正如工程师Paulo Matos所解释的，这个极具挑战性的过程通常需要大量的手动调试。

Igalia还显著增强了Mesa3D Turnip，这是一个用于高通Adreno GPU的FOSS Vulkan驱动。他们增加了对Adreno 700系列GPU的支持，以及LRZ等关键优化和众多Vulkan扩展，与专有驱动相比，实现了卓越的正确性和性能。工程师Danylo Piliaiev指出，他们成功确保了D3D11/12/OpenGL游戏能够完美渲染。这项工作，包括对图形编译器的贡献，造福了更广泛的开源社区。

此外，Igalia工程师积极贡献于Khronos Group，开发Vulkan标准、扩展，并通过数百万次一致性测试套件（CTS）测试确保合规性。他们还实施了强大的持续集成测试，以防止渲染退步。

除了图形方面，Igalia的Changwoo Min开发了LAVD，这是一款基于Rust、能效高的CPU调度器，对电池供电的Steam Frame至关重要。Melissa Wen改进了AMD内核显示驱动程序，以增强Steam Deck和Steam Machine上的色彩管理和HDR。

Valve对Mesa3D Turnip和FEX等开源软件的承诺，确保了这些进步造福于整个Linux游戏生态系统，而Igalia将继续推动SteamOS的改进。

---

## 3. HN 展示：Wealthfolio 2.0 — 开源投资追踪器。现已支持移动端和 Docker。

**原文标题**: Show HN: Wealthfolio 2.0- Open source investment tracker. Now Mobile and Docker

**原文链接**: [https://wealthfolio.app/?v=2.0](https://wealthfolio.app/?v=2.0)

Wealthfolio 2.0是一款开源、隐私优先的投资追踪器，旨在帮助个人跨桌面、移动和网络平台管理财富。它强调安全性与透明度，在本地运行，确保用户数据永不离开其设备。该应用程序免费使用，提供可选的一次性付款而非订阅制。

它提供一套全面的功能，包括带有CSV导入功能的账户聚合、清晰的股票、ETF和加密货币持仓概览，以及用于将账户与市场基准进行比较的业绩仪表盘。用户可以追踪股息和利息收入，监控个人账户的长期表现，以及设定并追踪财务目标。

此外，Wealthfolio有助于管理税收优惠账户（如IRA、401(k)、TFSA）的供款限额，以防止超额供款。该平台还具有可扩展性，提供诸如投资费用追踪器、目标进度追踪器和股票交易追踪器等附加组件。它的目标是用一个安全、精美且个性化的财富管理解决方案来取代杂乱的电子表格。

---

## 4. 个人博客回归，小众博客会是下一个热潮吗？

**原文标题**: Personal blogs are back, should niche blogs be next?

**原文链接**: [https://disassociated.com/personal-blogs-back-niche-blogs-next/](https://disassociated.com/personal-blogs-back-niche-blogs-next/)

文章提出，继当前个人博客复兴之后，利基博客的再度崛起应是下一步。这让人回想起博客的“黄金时代”，当时像Darren Rowse的Problogger这类专业网站，是成功、专注内容（常带有商业目的）的典范。利基博客因其能确立作者的专业性并有助于提高搜索引擎可见度而备受重视。

作者承认并非所有成功的博客都需要单一的利基市场，但也指出商业博客建议通常不适用于个人网站。如今，尽管社交媒体占据主导地位，但一场“反弹”以及独立网络/小型网络社区的发展，正在推动个人（大多是非商业性）网站的回归。

作者认为，这种复兴应延伸到高质量、专注于特定主题的利基博客。这被视为对抗社交媒体上日益增长的虚假信息和“AI垃圾内容”的关键对策。这些新型利基博客应由对主题充满热情的作者独立创作，提供可靠、准确的信息。文章强调，在不以侵入性广告损害读者体验的前提下，寻找道德的方式来补偿作者的重要性，并应从过去的盈利策略中吸取经验。最终，恢复可访问且值得信赖的利基信息，被认为是重建充满活力的网络的下一个关键步骤。

---

## 5. 法国法官如何被美国数字切断

**原文标题**: How a French judge was digitally cut off by the USA

**原文链接**: [https://www.heise.de/en/news/How-a-French-judge-was-digitally-cut-off-by-the-USA-11087561.html](https://www.heise.de/en/news/How-a-French-judge-was-digitally-cut-off-by-the-USA-11087561.html)

法国法官戴维·德·帕（David de Pas）在调查法国跨国公司阿尔斯通（Alstom）在亚洲合同中的贿赂指控时，遭遇了美国的严重阻挠，这有效地切断了他获取关键数字证据的途径。在德·帕进行平行调查的同时，美国司法部（DOJ）也对阿尔斯通进行了调查，最终处以7.72亿美元的罚款并监禁了高管。

德·帕迫切需要访问存储在美国微软服务器上的电子邮件和文件，以推进法国的调查。然而，美国国务院介入，明确禁止微软向法国当局提供这些数据。美国援引其主权以及对自身正在进行的调查可能产生的影响，威胁微软称，如果其遵守法国的司法协助请求，将面临法律后果，并使用保密令阻止访问。

此举凸显了美国法律的域外管辖权，阻止了法国调查获取重要证据。甚至在《云法案》（CLOUD Act）出台之前，美国就主张对美国公司持有的数据拥有管辖权，无论其物理位置何处。这一策略有效地削弱了法国对阿尔斯通腐败丑闻中涉案高层人员的调查。本文强调了美国法律框架如何阻碍盟国司法系统的运作，尤其是在现代数字证据和冲突的法律管辖权方面。

---

## 6. 我们都应该使用依赖项冷却时间。

**原文标题**: We should all be using dependency cooldowns

**原文链接**: [https://blog.yossarian.net/2025/11/21/We-should-all-be-using-dependency-cooldowns](https://blog.yossarian.net/2025/11/21/We-should-all-be-using-dependency-cooldowns)

文章强烈主张广泛采用“依赖项冷却期”，认为它是一种免费、简单且高效的策略，能够缓解绝大多数开源供应链攻击。文章指出，尽管供应链安全是一个严重问题，但许多商业解决方案被过度吹嘘。

其核心论点基于这类攻击的典型结构：攻击者入侵一个项目，上传恶意代码，然后在安全供应商和上游注册表检测并解决该漏洞之前，会有一个有限的“机会窗口”（通常是数小时到数天）。

依赖项冷却期是指从依赖项新版本发布到项目认为其适合使用之间的一个指定等待期，例如7天。这种延迟使得安全工具和人工审查能够在恶意更新被自动采用之前识别并报告它们。来自近期攻击（例如xz-utils、Ultralytics、tj-actions）的经验数据表明，大多数攻击的利用窗口期都不到一周；7天的冷却期本可以阻止绝大多数此类攻击触达最终用户。

冷却期实现起来很简单，通常可以使用Dependabot或Renovate等工具，或通过某些包管理器中的功能免费实现。除了其已证实的有效性（可将风险暴露降低80-90%），它们还激励安全供应商专注于快速、有影响力的检测。尽管不是一个完整的解决方案，但冷却期以最小的努力提供了显著的风险降低，作者建议包管理器应直接集成它们。

---

## 7. Olmo 3: 规划模型流程路径，引领开源人工智能

**原文标题**: Olmo 3: Charting a path through the model flow to lead open-source AI

**原文链接**: [https://allenai.org/blog/olmo3](https://allenai.org/blog/olmo3)

Olmo 3 代表着一项重要的开源举措，强调可访问“完整的模型流”——包括每一个阶段、检查点、数据集和依赖项——而不仅仅是最终的模型权重。这种全面的方法旨在培养信任、实现深度定制并加速人工智能研究，通过允许用户在其开发生命周期的任何阶段检查、调整和扩展模型。

Olmo 3 系列包括紧凑、密集型模型（70亿和320亿参数），涵盖了多种专用变体：
*   **Olmo 3-Base：** 一个功能强大的基础模型（70亿、320亿参数），在完全开源模型中提供最先进的性能，并在数学、编程和阅读理解方面与领先的开源权重模型具有竞争力。它支持扩展的上下文长度。
*   **Olmo 3-Think：** 旗舰推理模型（70亿、320亿参数），专为高级实验设计。它支持检查中间推理痕迹，并在推理基准测试中表现出强大的性能，经常达到或超过同类开源权重模型。
*   **Olmo 3-Instruct：** 一个70亿参数模型，针对聊天、指令遵循和工具使用进行了优化，达到或超越了多个开源权重模型。
*   **Olmo 3-RL Zero：** 一个70亿参数模型，为研究和基准测试提供了一个完全开放的强化学习路径。

Olmo 3 利用多阶段训练管道和针对每条路径的特定后训练配方（SFT、DPO、RLVR）。所有组件——包括扩展的高质量训练数据、代码和模型权重——均在宽松的开源许可下发布，以促进完全透明并赋能社区构建自己的人工智能系统。

---

## 8. Arduino发布了更新的条款和条件：不再是开放共享

**原文标题**: Arduino published updated terms and conditions: no longer an open commons

**原文链接**: [https://www.molecularist.com/2025/11/did-qualcomm-kill-arduino-for-good.html](https://www.molecularist.com/2025/11/did-qualcomm-kill-arduino-for-good.html)

高通最近收购Arduino后，更新的条款和条件引起了创客社区的深切关注，预示着Arduino开放共享精神的终结。新条款引入了标准的企业规定，如强制仲裁、与高通生态系统的数据整合、出口管制、AI使用限制，以及关键性的明确声明：使用该平台不授予任何专利许可，并禁止对“该平台”进行逆向工程。

这直接与Arduino的开源IDE（AGPL）和CLI（GPL v3）冲突，给库贡献者和“Arduino兼容”硬件制造商带来了重大的法律不确定性。社区猜测这究竟是律师业务不精、一次试探，还是旨在锁定生态系统的蓄意举动，尤其考虑到“该平台”的模糊定义（是指云服务还是核心工具）。

开放硬件领域的知名领导者Adafruit强调，高通误解了Arduino的真正价值。Arduino不仅仅是一家物联网硬件公司；它是“创客世界的IBM PC”——一个基础标准，也是业余电子领域的通用语言，支持着庞大的库、教程和教育项目生态系统。将限制性企业法律框架应用于这一共享领域，可能会毒害整个创客生态系统，使得数十年的机构知识陷入困境，并让新创客无法接触到电子技术，因为目前没有同样对初学者友好的替代方案。

尽管这可能源于企业法律标准化而非恶意，但这种迟钝的做法已经侵蚀了信任。为挽救局面，高通必须明确澄清限制性条款仅适用于云服务，明确无误地保护其现有许可下的开源IDE、CLI和核心库，理想情况下，还应建立一个基金会或社区治理模式。未来几个月将揭示Arduino是作为开放共享平台幸存下来，还是沦为另一个企业平台。

---

## 9. 过度监管导致成本翻番

**原文标题**: Over-regulation is doubling the cost

**原文链接**: [https://rein.pk/over-regulation-is-doubling-the-cost](https://rein.pk/over-regulation-is-doubling-the-cost)

作者曾是一名软件企业家，现在正在创建“硬科技”公司：Charm Industrial（碳清除）和Revoy（电动卡车运输）。他认为，过度监管和官僚作风使美国的成本翻倍，并扼杀了创新。他断言，监管瓶颈占了他公司一半以上的开支，延迟了气候解决方案，提高了消费者成本，并积极阻碍了环境改善。

Charm Industrial通过注入生物油来去除二氧化碳，仅仅为了确定正确的许可证类型就面临了四年的延迟，导致整个许可过程长达5.5年。这一延迟使Charm损失了9000万美元的运营时间，并因持续污染造成了估计3亿美元的社会医疗负担。

同样，Revoy为半挂卡车设计的电动“转换拖车”，旨在将燃油消耗降低94%，在跨机构分类方面遭遇了数年的延迟。一个州机构要求进行2700万美元的测试，以证明这个旨在“减少”排放的设备并没有“增加”排放——作者认为这笔费用是浪费且适得其反的。

作者将这些问题归因于一个充斥着过度具体、人员不足和对法律挑战的恐惧的监管体系，这导致了一种极度谨慎的文化，对新技术而言，“不”是默认答案。他主张简化法规，赋权并信任监管机构，限制激进主义诉讼，并实施快速审查和“权利许可”，以释放创新，改善环境，并支持美国制造业。

---

## 10. 新系统旨在部分兼容 macOS

**原文标题**: New OS aims to provide (some) compatibility with macOS

**原文链接**: [https://github.com/ravynsoft/ravynos](https://github.com/ravynsoft/ravynos)

ravynOS 是一个全新的开源操作系统项目，旨在 x86-64 和最终 ARM 系统上提供类似 macOS 的体验和兼容性。它基于强大的 FreeBSD 基础构建，旨在实现与 macOS 应用程序的源代码兼容性，使其能够在 ravynOS 上编译和运行。

主要设计目标包括熟悉的 macOS 风格 GUI 和用户体验（例如，顶部菜单栏、文件管理器）、与 macOS 文件夹布局（/Library、/System、/Users）的兼容性，以及对 HFS+ 和 APFS 文件系统的潜在支持，同时全面支持 ZFS。它通过 App Bundles、AppDirs 和 AppImage 文件推广免安装的应用程序体验。ravynOS 还保持与 FreeBSD 基础系统和 X11 的兼容性，提供标准的 Unix 环境，并通过 FreeBSD 内置功能支持 Linux 二进制文件。未来的目标是直接兼容 x86-64/arm64 macOS 二进制文件（Mach-O）和库。该项目优先考虑易用性、安全性、稳定性和高性能。

更多信息、屏幕截图和贡献详情可在 ravynos.com 及其社区渠道获取。其底层 FreeBSD 是一个持续开发的操作系统，拥有超过 30 年的历史，广泛用于服务器、桌面和嵌入式平台，以其先进的网络、安全和存储功能而闻名。

---

## 11. 你可以用 JavaScript 制作 PS2 游戏

**原文标题**: You can make PS2 games in JavaScript

**原文链接**: [https://jslegenddev.substack.com/p/you-can-now-make-ps2-games-in-javascript](https://jslegenddev.substack.com/p/you-can-now-make-ps2-games-in-javascript)

本文介绍了PS2.JS，一个基于JavaScript的引擎，它使网页开发者能够创建模仿PlayStation 2时代独特美学和感觉的游戏。PS2.JS建立在流行的Three.js库之上，其设计目的并非模拟真实的PS2主机，而是重现90年代末和2000年代初主机游戏中常见的视觉特征。

其主要特性包括支持低多边形模型、像素化纹理、固定摄像机视角和特定的光照风格，使开发者能够打造出让人回想起早期3D主机游戏体验的作品。该项目旨在降低JavaScript开发者进行游戏开发的门槛，使他们能够利用现有技能快速原型设计并构建复古风格的游戏。这些游戏直接在网页浏览器中运行，提供了一种独特的方式来探索怀旧游戏设计，而无需复杂的游戏引擎或底层编程。PS2.JS专注于捕捉那个时代的“氛围”和风格限制，为在浏览器环境中进行创意表达提供了一条新途径。

---

## 12. 《超人》创刊号漫画成为史上售价最高的漫画书

**原文标题**: Original Superman comic becomes the highest-priced comic book ever sold

**原文链接**: [https://www.bbc.com/news/articles/c8e9rp0knj6o](https://www.bbc.com/news/articles/c8e9rp0knj6o)

一本1939年6月第一版的《超人 #1》原版漫画，在位于德克萨斯州的传统拍卖行（Heritage Auctions）举办的拍卖会上以912万美元（约合700万英镑）的价格成交，成为有史以来售价最高的漫画书。

这本品相极佳的漫画，经CGC（漫画鉴评公司）评级，在10分制中获得9.0分。去年圣诞节，三兄弟在清理他们已故母亲位于加利福尼亚的阁楼时发现了它。他们在一个旧报纸下面的纸箱里找到了它，同时还有另外五本漫画。他们的母亲在大萧条和第二次世界大战之间收藏了这些漫画，并经常告诉儿子们她拥有珍贵的漫画，尽管从未展示给他们看。凉爽的北加州气候被认为是这本漫画得以非凡保存的关键。

此次售价轻松超越了此前由《动作漫画 #1》（1938年）保持的600万美元纪录，这本首次引入超人的漫画于去年售出。传统拍卖行（Heritage Auctions）称此次拍卖是“漫画收藏的巅峰”。最小的弟弟形容这次发现是“对记忆、家庭以及过去以意想不到的方式回归我们的证明”。

---

## 13. 专家称，百忧解治疗儿童抑郁症“不比安慰剂强”。

**原文标题**: Prozac 'no better than placebo' for treating children with depression, experts

**原文链接**: [https://www.theguardian.com/society/2025/nov/20/prozac-no-better-than-placebo-for-treating-children-with-depression-experts-say](https://www.theguardian.com/society/2025/nov/20/prozac-no-better-than-placebo-for-treating-children-with-depression-experts-say)

奥地利和英国学者进行的一项新的12项试验荟萃分析得出结论，百忧解（氟西汀）在临床上治疗儿童和青少年抑郁症方面不优于安慰剂。这项发表在《临床流行病学杂志》上的研究发现，氟西汀对抑郁症状的任何改善都微乎其微，不具有临床意义。

这一发现促使专家们主张，英国、美国和加拿大当前的临床指南应进行修改，因为这些指南目前推荐百忧解等抗抑郁药用于18岁以下中度至重度抑郁症患者，通常还会伴随心理治疗。作者认为，最初的“新颖性偏倚”可能夸大了早期试验结果，而后续研究未能证实这些效果。

鉴于相对于安慰剂缺乏临床益处，共同作者马克·霍洛维茨等专家指出，让年轻人接触一种已知具有副作用——包括体重增加、睡眠障碍、注意力不集中和自杀意念增加——的药物是不合理的。他们敦促临床医生专注于理解和解决抑郁症的根本原因。

英国国家健康与护理优化研究所（Nice）回应称，强调心理疗法是青少年的一线治疗方法，抗抑郁药仅在专家监督下对中度至重度病例才予以考虑。然而，英国皇家精神科医师学院的艾伦·杨教授建议谨慎解读这项研究，指出指南在制定时会考虑平均效应量之外的多种因素。

---

## 14. 在家教育人数创历史新高

**原文标题**: Homeschooling hits record numbers

**原文链接**: [https://reason.com/2025/11/19/homeschooling-hits-record-numbers/](https://reason.com/2025/11/19/homeschooling-hits-record-numbers/)

美国家庭教育正经历创纪录的增长，2024-2025学年增长率为5.4%，几乎是疫情前2%增长率的三倍。这一趋势最初由COVID-19学校停课和对远程学习的不满所推动，此后持续存在并甚至加速，超过三分之一的州报告其家庭教育人数达到历史新高。约翰霍普金斯大学的安吉拉·沃森等专家指出，这代表着美国教育的“根本性转变”，而不仅仅是“疫情的遗留影响”。目前，全国家庭教育学生总数约占学生总数的6%，是疫情前约3%的两倍。

这一激增是更广泛的趋势的一部分，即从传统的公立学校转向非公立的替代方案。研究表明，如果当前趋势持续下去，到本世纪中叶公立学校可能流失数百万学生。这一转变的主要驱动因素是家长对公立K-12教育日益增长的不满，59%的家长认为公立教育正朝着错误的方向发展——这是十年来最高比例。公立学校的家长满意度始终低于选择私立学校、家庭教育或特许学校的家长。

这种不满的原因包括感知到的僵化、课程的政治化、学习成果的下降，以及对疫情期间政策和远程学习能力的沮丧。家庭教育在所有家长中拥有70%的支持率，提供了一种可定制的替代方案。这一趋势显示出强大的韧性，即使是曾短暂下降的州现在也报告了两位数的增长，这巩固了家庭教育作为一种日益流行和主流教育选择的地位。

---

## 15. 智能体设计仍然很难

**原文标题**: Agent design is still hard

**原文链接**: [https://lucumr.pocoo.org/2025/11/21/agents-are-hard/](https://lucumr.pocoo.org/2025/11/21/agents-are-hard/)

阿明·罗纳赫 (Armin Ronacher) 分享了他对代理设计持续挑战的见解。他建议不要使用 Vercel AI SDK 等高级别 SDK，而是提倡直接使用平台 SDK（例如 Anthropic、OpenAI），以便更好地控制显著的模型差异、工具集成和缓存。Anthropic 采用的显式缓存管理方法因其可预测性和可控性而备受推崇，它支持对话拆分和上下文编辑等策略。代理循环内的强化对于指导代理、提醒其目标、提供失败提示以及传递状态变化至关重要。故障应该被隔离，通常通过在子代理中运行迭代任务，并且只报告成功或总结失败的方法。对于依赖代码执行和生成的代理来说，共享虚拟文件系统至关重要，它能让不同的工具和子代理无缝共享数据，并防止“死胡同”。用于用户通信（例如电子邮件）的专用输出工具面临挑战，因为很难控制其语气，而且为此目的使用子大型语言模型会增加延迟并降低质量。模型选择至关重要：Haiku 和 Sonnet 因其卓越的工具调用能力而受到主代理循环的青睐，而 Gemini 2.5 在总结和图像提取方面表现出色。测试和评估仍然是最困难的方面，它需要进行内嵌检测的测试运行，而不是依赖外部系统。罗纳赫还提到正在试用 Amp，因为它拥有精心设计的子代理交互功能，并且注意到人工智能生成的实用工具正在取代小型开源库的趋势。

---

## 16. 加州DMV批准Waymo无人驾驶运营扩大地图范围

**原文标题**: California DMV approves map increase in Waymo driverless operations

**原文链接**: [https://www.dmv.ca.gov/portal/vehicle-industry-services/autonomous-vehicles/autonomous-vehicle-testing-permit-holders/waymo-approved-areas-of-operation-for-driverless-testing-and-deployment/](https://www.dmv.ca.gov/portal/vehicle-industry-services/autonomous-vehicles/autonomous-vehicle-testing-permit-holders/waymo-approved-areas-of-operation-for-driverless-testing-and-deployment/)

加州机动车辆管理局（DMV）已批准Waymo在加州大幅扩张其无人驾驶测试和部署业务。此授权允许Waymo在全州所有已批准的运营设计域（ODD）内运行全自动驾驶车辆。

Waymo获批用于这些运营的车辆包括捷豹I-Pace（2021年和2024年款）以及极氪RT（2022年和2025年款）。这些车辆获准在全天候、雨雾等各种条件下以及所有速度下运行。

此项批准的核心是Waymo运营地图的大幅扩展。扩展后的运营设计域（ODD）涵盖了加州境内的众多城市和县。这包括在阿拉米达、康特拉科斯塔、洛杉矶、马林、纳帕、奥兰治、河滨、萨克拉门托、圣贝纳迪诺、圣迭戈、旧金山、圣马特奥、圣克拉拉、圣克鲁斯、索拉诺、索诺玛、文图拉和约洛等县的广泛覆盖。这种广泛的地理批准标志着Waymo在加州的自动驾驶汽车服务和发展取得了重大进展。

---

## 17. 惠普和戴尔禁用其笔记本电脑CPU内置的HEVC支持

**原文标题**: HP and Dell disable HEVC support built into their laptops' CPUs

**原文链接**: [https://arstechnica.com/gadgets/2025/11/hp-and-dell-disable-hevc-support-built-into-their-laptops-cpus/](https://arstechnica.com/gadgets/2025/11/hp-and-dell-disable-hevc-support-built-into-their-laptops-cpus/)

惠普和戴尔正在停用其部分笔记本电脑处理器中的HEVC (H.265) 硬件解码功能，尽管自英特尔第六代酷睿和AMD 2015年型号处理器以来，CPU就已集成了此功能。这一决定导致用户无法在网络浏览器中高效播放HEVC内容，迫使他们采取禁用硬件加速等权宜之计，这会降低性能并削弱功能（例如，视频通话中无法进行背景虚化）。

受影响的型号包括惠普ProBook和EliteBook G11系列，其数据表中已注明此停用。对于戴尔，它影响了一些商用笔记本电脑，如戴尔16 Plus二合一；相关信息更难找到，通常出现在一个通用的支持页面上，指出HEVC播放仅支持特定配置，如独立显卡、4K显示器、杜比视界或CyberLink蓝光软件。两家公司都证实了这一变化，建议用户使用第三方软件或“高端”系统来支持HEVC。

可能的原因是HEVC授权费用上涨。授权管理机构Access Advance宣布，自1月起，销量超过100,001台的单位特许权使用费将从每台0.20美元增至0.24美元。这一可能由原始设备制造商（OEM）承担的财务负担，似乎是一个重要因素。其他公司如群晖（Synology）也已缩减了对HEVC的支持。此举正引起用户的不满，特别是对于HEVC常用场景的高端“专业版”笔记本电脑用户。

---

## 18. 全美首创，新墨西哥州推行全民免费托儿服务

**原文标题**: In a U.S. First, New Mexico Opens Doors to Free Child Care for All

**原文链接**: [https://www.wsj.com/us-news/in-a-u-s-first-new-mexico-opens-doors-to-free-child-care-for-all-2dfdea96](https://www.wsj.com/us-news/in-a-u-s-first-new-mexico-opens-doors-to-free-child-care-for-all-2dfdea96)

无法访问文章链接。

---

## 19. 构建振荡器很难

**原文标题**: It's hard to build an oscillator

**原文链接**: [https://lcamtuf.substack.com/p/its-hard-to-build-an-oscillator](https://lcamtuf.substack.com/p/its-hard-to-build-an-oscillator)

Michal Zalewski 的文章“振荡器构建之难”揭示了设计可靠稳定电子振荡器时意想不到的复杂性，尽管它们在理论上很简单。虽然其概念——一个增益级、一个频率相关的相移和一个反馈回路——看似简单，但实际实现却面临诸多实践挑战。

根本困难源于物理元件的非理想性。电阻器、电容器和有源器件并非完美无缺；它们的数值受制于制造公差、温度变化和老化，这使得难以实现稳定振荡所需的精确相移和增益。此外，振荡器极易受到噪声（热噪声、电源噪声、电磁干扰）的影响，这些噪声会轻易干扰其精密的反馈机制。源自电路走线和元件引线的寄生电容和电感，引入了意想不到的影响，显著改变了预期行为，尤其是在高频下。

文章强调了确保振荡器可靠*启动*并随后保持*干净、稳定*的振荡，同时具有一致的频率、幅度和波形纯度的障碍。即使是因其稳定性而备受推崇的晶体振荡器，也需要精心设计的支持电路，以避免杂散模式或启动失败等问题。作者强调了工程中的“最后一公里”问题：创建一个功能原型不同于设计一个在各种条件（温度、电压、元件变化）下都能持续表现稳健的、可投入生产的振荡器。这篇文章强调了模拟物理学与硬件设计中现实世界缺陷之间错综复杂的相互作用。

---

## 20. FAWK: 大语言模型能编写语言解释器

**原文标题**: FAWK: LLMs can write a language interpreter

**原文链接**: [https://martin.janiczek.cz/2025/11/21/fawk-llms-can-write-a-language-interpreter.html](https://martin.janiczek.cz/2025/11/21/fawk-llms-can-write-a-language-interpreter.html)

作者在解决一个Advent of Code问题时，发现传统AWK不足以支持现代函数式编程范式，于是构想了"FAWK"——一个现代化的AWK，它融入了诸如第一类数组和函数、词法作用域、显式全局变量和管道等特性。

作者没有手动实现，而是委托一个大型语言模型（LLM，通过Cursor Agent使用Sonnet 4.5）来生成FAWK的Python解释器。令他们惊讶的是，该LLM不仅提供了一个可工作的解释器，而且出色地处理了闭包、多维数组、I/O重定向乃至GAWK向后兼容性等复杂功能。唯一值得注意的难题是，在没有外部库的情况下，处理任意精度浮点数学计算。

这次经历彻底改变了作者对LLM在复杂软件工程中能力的看法，意识到一门新语言可以在一日之内被“凭感觉编写”（vibe-coded）出来。然而，一个显著的缺点是作者对所生成的代码库完全不熟悉，这引发了关于未来维护以及LLM生成与人类理解之间平衡的问题。作者计划在未来的谜题中“以身试用”（dogfood）FAWK，并探索更多LLM辅助开发的可能性，同时已将该项目发布到GitHub上。

---

## 21. DuckDB 静态数据加密

**原文标题**: Data-at-Rest Encryption in DuckDB

**原文链接**: [https://duckdb.org/2025/11/19/encryption-in-duckdb](https://duckdb.org/2025/11/19/encryption-in-duckdb)

DuckDB v1.4 引入了透明的静态数据加密功能，以满足安全性与合规性需求（如SOC 2）。在PostgreSQL和SQLite等其他数据库中，此功能通常受限或成本高昂。

该系统使用行业标准的对称AES加密，支持AES-GCM-256（推荐用于带标签的数据认证）和AES-CTR-256（速度更快，无认证）。这些密码算法需要明文、初始化向量 (IV/nonce) 和加密密钥。

DuckDB 的实现将主数据库头保持明文，存储必要的元数据，如数据库标识符（盐值）和一个加密的“金丝雀”值，用于验证加密密钥。所有后续的头部、数据块和预写日志 (WAL) 均已加密。用户提供的密钥从不直接使用；相反，系统通过密钥派生函数 (KDF) 派生出安全的密钥，将其存储在安全的内存缓存中，并立即清除原始输入密钥。

加密的数据块具有一个扩展的40字节头部，其中包含 nonce/IV 和一个可选的认证标签，并且校验和本身也经过加密以增强安全性。WAL 条目是单独加密的，包括其长度、nonce、加密校验和以及条目本身，外加GCM的标签。

至关重要的是，用于外部存储操作的临时文件也会自动加密。这些文件利用内部生成的临时密钥，确保即使数据库崩溃，残留的临时文件也是不可恢复的“垃圾”，从而防止数据泄露。

用户可以使用 `ATTACH` 命令，并通过指定 `ENCRYPTION_KEY` 和 `ENCRYPTION_CIPHER` 来启用加密。数据库可以被初始化、加密或重新加密。通过观察高数据熵，使文件内容呈现为随机噪声，即可验证加密是否成功。

---

## 22. 洛杉矶警局含实时运行成本的直升机追踪器

**原文标题**: LAPD helicopter tracker with real-time operating costs

**原文链接**: [https://lapdhelicoptertracker.com/](https://lapdhelicoptertracker.com/)

本文介绍了“洛杉矶警察局直升机追踪器”，这是一套旨在提供警用航空实时监控的创新系统。其主要特点是内置成本计算器，可显示每架在飞的洛杉矶警察局直升机的实时运行费用。该追踪器旨在透明地展示警局空中支援行动的部署和财务影响，让用户能够追踪警务活动并了解其即时成本。

---

## 23. 制作小RPG

**原文标题**: Making a Small RPG

**原文链接**: [https://jslegenddev.substack.com/p/making-a-small-rpg](https://jslegenddev.substack.com/p/making-a-small-rpg)

JSLegendDev的博文《制作小型RPG》为旨在开发可管理RPG而非雄心勃勃的大型项目的开发者提供了实用指导。作者将“小型”定义为范围有限的游戏，建议游戏时长约5-8小时，包含一个主城、一个主地牢和少量支线任务。

文章概述了任何RPG都不可或缺的五个核心支柱：角色发展（属性、技能、装备、升级）、叙事（清晰的故事或目的）、探索（可发现的区域）、战斗/互动（玩家的参与方式）以及战利品/进程（奖励与成长）。对于小型RPG，关键在于专注于这些基础要素，而不使其过于复杂。

保持小规模的策略包括优先考虑必要的RPG功能，创作一个简单但引人入胜的故事，并通过重用现有资源或选择更简单的视觉风格来限制美术资产。文章还建议采用模块化设计方法，将任务分解为可管理的小块，并快速迭代以建立功能性的核心玩法循环。实用建议还包括利用Unity、Godot或RPG Maker等现有游戏引擎，拥抱局限性，保持简洁的文档，并进行持续的玩家测试。其核心信息是通过从小处着手并有效迭代，来构建一个专注且令人愉快的游戏体验。

---

## 24. 警察如何利用Flock的ALPR网络监视抗议者和活动人士

**原文标题**: How Cops Are Using Flock's ALPR Network to Surveil Protesters and Activists

**原文链接**: [https://www.eff.org/deeplinks/2025/11/how-cops-are-using-flock-safetys-alpr-network-surveil-protesters-and-activists](https://www.eff.org/deeplinks/2025/11/how-cops-are-using-flock-safetys-alpr-network-surveil-protesters-and-activists)

对Flock Safety的自动车牌识别（ALPR）网络数据从2024年12月至2025年10月的分析显示，包括美国边境巡逻队在内的50多个联邦、州和地方执法机构进行了数百次与抗议活动相关的搜索。Flock的ALPR系统捕捉并记录每辆车的车牌、特征、时间以及位置，存入一个巨大的、可搜索的全国性数据库中，该数据库在各机构之间共享。

各机构针对了主要的示威活动，例如“无君主”运动（反对政府越权）、“50501抗议活动”，以及与驱逐出境突袭和警察枪击事件相关的集会。警官们经常在搜索的“理由”字段中输入“抗议”或具体的抗议名称等模糊词语，通常没有明确说明实际犯罪行为，这引发了对侵犯第一修正案权利的严重担忧。

美国边境巡逻队广泛使用Flock数据进行移民执法，并监控那些批评其策略的人，即使在其直接访问被暂停后，仍通过地方机构访问该系统。该网络还专门用于监视“直接行动无处不在”（DxE）的动物权利活动家，将搜索与他们的调查和直接行动联系起来，这表明其影响力已超越大型政治示威活动。

尽管一些搜索可能与犯罪有关，但ALPR系统收集了抗议活动附近每个人的数据，这对言论自由造成了“寒蝉效应”。报告建议抗议者考虑乘坐其他交通工具前往示威地点，以保护他们的隐私。报告还敦促地方官员关闭这些监控网络，认为异议权不应导致个人被添加到数据库中。分析表明，鉴于许多搜索使用了“调查”等模糊理由，实际监控程度可能更高。

---

## 25. 法国正在对GrapheneOS采取国家行动？

**原文标题**: France is taking state actions against GrapheneOS?

**原文链接**: [https://grapheneos.social/@GrapheneOS/115584160910016309](https://grapheneos.social/@GrapheneOS/115584160910016309)

这篇文章强调了 GrapheneOS 通过其官方 Mastodon 账户提出的一项主张，称“法国正在对该项目采取国家行动”。该文章的标题将此框定为一个问题：“法国正在对 GrapheneOS 采取国家行动吗？”，表明了报告的性质。所提供的内容直接引用了 GrapheneOS 在 Mastodon 上提出的这一断言，但并未包含其声明的完整背景。文章没有详细阐述这些所谓的政府行动的具体性质或原因。所提供文本中一个单独的、不相关部分是一条关于为 Mastodon 网络应用程序启用 JavaScript 的标准 Mastodon 消息。

---

## 26. 搭载骁龙X Elite SoC的ARM笔记本停产

**原文标题**: Discontinuation of ARM Notebook with Snapdragon X Elite SoC

**原文链接**: [https://www.tuxedocomputers.com/en/Discontinuation-of-ARM-notebooks-with-Snapdragon-X-Elite-SoC.tuxedo](https://www.tuxedocomputers.com/en/Discontinuation-of-ARM-notebooks-with-Snapdragon-X-Elite-SoC.tuxedo)

主要公告是停产搭载骁龙X Elite SoC的ARM笔记本电脑。

与此同时，该供应商也推广了其产品和服务的通用优势：兼容Linux、长达5年保修、即买即用、德国组装、德国数据隐私保护和德国技术支持。此外，用户需启用JavaScript并禁用脚本拦截器才能使用商店。

---

## 27. 余弦解Fizz Buzz

**原文标题**: Solving Fizz Buzz with Cosines

**原文链接**: [https://susam.net/fizz-buzz-with-cosines.html](https://susam.net/fizz-buzz-with-cosines.html)

本文探讨了一种非传统的数学方法来解决经典的Fizz Buzz问题，即用三角函数取代传统的模运算。作者旨在利用离散傅里叶级数，将Fizz Buzz序列的周期性编码成一个单一的闭式表达式。

该解决方案首先定义了四个“符号函数”（`s_0`代表数字，`s_1`代表“Fizz”，`s_2`代表“Buzz”，`s_3`代表“FizzBuzz”）以及一个“索引函数”`f(n)`，它决定了给定`n`时要输出哪个符号。这个`f(n)`最初被构造为一个基于可除性规则的分段函数。

一个关键的简化是使用了“指示函数”`I_m(n)`（如果`m`能整除`n`则为1，否则为0）。文章巧妙地观察到`f(n)`可以表示为`I_3(n) + 2 * I_5(n)`，有效地将`I_5(n)`和`I_3(n)`视为构成`f(n)`的二进制位。文章提供了一个Python程序来演示这种简化逻辑。

文章的核心接着将这些指示函数转换为复指数，并随后利用欧拉公式转换为余弦函数。它表明`I_m(n)`可以写成`(1/m) * sum(e^(2*pi*i*k*n/m))`。应用此方法，`I_3(n)`被表示为`(1/3) + (2/3)cos(2*pi*n/3)`，`I_5(n)`被表示为`(1/5) + (2/5)cos(2*pi*n/5) + (2/5)cos(4*pi*n/5)`。

通过将这些余弦形式代回到`f(n) = I_3(n) + 2 * I_5(n)`中，导出了一个仅使用余弦的`f(n)`的完整闭式表达式。文章提供了一个使用`round()`函数处理此余弦公式的Python实现。文章最后指出，该解决方案是一个有限傅里叶级数，并简要概述了如何通过更“繁琐”的离散傅里叶变换计算获得相同的结果。

---

## 28. XBMC 4.0 初代Xbox版

**原文标题**: XBMC 4.0 for the Original Xbox

**原文链接**: [https://www.xbox-scene.info/articles/announcing-xbmc-40-for-the-original-xbox-r64/](https://www.xbox-scene.info/articles/announcing-xbmc-40-for-the-original-xbox-r64/)

XBMC 4.0 已针对初代 Xbox 发布，标志着一次重大的现代化，也是该主机标志性媒体中心平台自 2016 年以来的首次重大更新。它最初于 2002 年以 XboxMediaPlayer 的身份出现，XBMC 影响了 Kodi 和 Plex 的开发。

这个新版本使软件焕发了生机，带来了由 Estuary 皮肤驱动的现代界面，首次出现在 Kodi v17 中。这需要移植现代的 GUIlib 引擎，使未来的皮肤开发变得更容易。XBMC 4.0 引入了一个完整的游戏库系统，为 Xbox 和模拟游戏提供丰富的元数据支持、艺术作品和描述，类似于其电影和音乐库。

电影和电视的在线元数据抓取器已完全恢复，从而实现全面的媒体库创建。任务调度方面的改进允许在 Xbox 有限的硬件上同时进行后台活动，例如库更新。音乐体验通过支持无损编解码器（FLAC）和可视化工具得到增强。

此版本包含一个易于访问的在线插件库，并继续支持基于 Python 的插件，计划升级到 Python 3.4.10。设置、网络服务（SMB、FTP、UPnP）和系统工具都经过修订，以提高清晰度和控制性。

XBMC 4.0 独立于 XBMC4Gamers，且不隶属于 Kodi 基金会，它正在积极开发中。它欢迎社区贡献，旨在未来多年内扩展初代 Xbox 作为多功能媒体中心的能力。

---

## 29. 柯吉助手

**原文标题**: Kagi Assistants

**原文链接**: [https://blog.kagi.com/kagi-assistants](https://blog.kagi.com/kagi-assistants)

Kagi 于 2025 年 11 月 20 日推出了新的快速助手 (Quick Assistant) 和研究助手 (Research Assistant)，旨在利用人工智能增强而非取代人类的搜索体验。快速助手适用于所有套餐，提供快速、简洁的答案。研究助手面向最高级套餐用户，提供深入、详尽的分析，能够执行多次搜索并将发现结果综合为高质量、带来源的答案。两者均可通过 Kagi 助手网页应用访问，也可以直接在搜索栏中使用 `!quick` 和 `!research` 等命令调用。

2025 年 8 月，Kagi 的研究助手在 SimpleQA 基准测试中取得了 95.5% 的分数，Kagi 称其为“意外之喜”，因为它优先考虑产品实用性而非基准分数。他们解释说，不愿追求 100% 分数的原因包括潜在的过拟合、相互冲突的官方数据、伦理问题（如激进的网络爬虫），以及基准测试创建者固有的偏见。

值得注意的是，Kagi 发现其搜索引擎在 SimpleQA 等基准测试中作为大型语言模型 (LLMs) 的卓越后端，表现优于 Google/Bing，因为它提供了更少噪音和更相关的结果，从而提高了大型语言模型的准确性。助手还可以访问网络搜索之外的先进工具，包括代码执行和特定 API。Kagi 强调为用户构建赋能工具，而不是强推人工智能或追逐人为设定的基准。

---

## 30. 新格伦更新

**原文标题**: New Glenn Update

**原文链接**: [https://www.blueorigin.com/news/new-glenn-upgraded-engines-subcooled-components-drive-enhanced-performance](https://www.blueorigin.com/news/new-glenn-upgraded-engines-subcooled-components-drive-enhanced-performance)

蓝色起源公司宣布对其“新格伦”火箭进行重大升级，旨在提升其未来任务的性能。主要改进包括：将第一级发动机全面换装为七台BE-4发动机，每台推力可达55万磅；以及采用过冷液氧（LOX）和液化天然气（LNG）推进剂。

使用过冷推进剂（即将其冷却至更低温度），能够增加其密度。这使得更多推进剂能够装载到现有储罐体积中，有效提高了火箭的质量分数，并在不重新设计核心结构的情况下，提升了整体性能。此次升级提供了将更重有效载荷送往不同轨道的灵活性，包括地球同步转移轨道（GTO）、近地轨道（LEO）以及月球轨道。

这些增强功能将支持多种任务，涵盖美国宇航局（NASA）的商业月球有效载荷服务（CLPS）计划、NSSL第三阶段合同下的国家安全发射，以及商业卫星部署。升级后的“新格伦”火箭有望在其首次飞行及后续任务中提供更强大的任务多样性和能力。

---

## 31. 浏览器指纹的隐私噩梦

**原文标题**: The privacy nightmare of browser fingerprinting

**原文链接**: [https://kevinboone.me/fingerprinting.html](https://kevinboone.me/fingerprinting.html)

本文《浏览器指纹识别的隐私噩梦》指出，浏览器指纹识别构成了一个重大且日益增长的隐私威胁，其影响超越了传统的追踪Cookie。文章解释说，指纹识别的工作原理是提取用户浏览器和系统中离散信息的独特组合。这包括浏览器版本、操作系统、语言和时区等基本细节，以及已安装字体、浏览器扩展、硬件信息和“画布指纹”（由独特的图形硬件/操作系统交互导致渲染文本的细微像素差异）等更复杂的数据。即使是像窗口大小这样的微小偏好，也有助于形成一个独特的标识符。

对抗指纹识别的尝试充满挑战。禁用JavaScript会使​​用户显得与众不同并破坏网站功能，而伪造用户代理则很容易被检测到。严格的伪造方法可能会留下痕迹或破坏网站功能。

尽管存在这些困难，作者指出，现实世界中的追踪更多是统计性的而非绝对的，并且一个暂时独特的指纹并不能保证长期可追溯性。浏览器开发商也开始整合更强大的反制措施，其中Brave、Mullvad和Librewolf是值得注意的例子。

对于寻求抵制指纹识别的用户，建议包括使用VPN、阻止长期有效的Cookie，并努力做到“不引人注目”——即使用流行浏览器/操作系统、默认配置、最少扩展和默认设置。使用内置抵抗机制的浏览器也被推荐。

然而，这些措施也有缺点：例如强制窗口大小带来的不便、更多的验证码挑战以及潜在的网站功能问题。即使采取了所有预防措施，效果也有限，可能只能将可追溯性降低到50%左右。

浏览器指纹识别的合法性仍不明确，可能违反了GDPR的精神，但在法庭上尚未得到证实，部分原因是其合法用途，例如欺诈检测。作者总结道，最终需要新的立法来解决这种隐形且具有侵扰性的技术，这种技术主要使在线广告行业受益。

---

## 32. 我是如何学习Vulkan并用它编写小型游戏引擎的 (2024)

**原文标题**: How I learned Vulkan and wrote a small game engine with it (2024)

**原文链接**: [https://edw.is/learning-vulkan/](https://edw.is/learning-vulkan/)

在《我是如何学习Vulkan并用它编写一个小型游戏引擎的 (2024)》一文中，一位自学成才的专业程序员讲述了他们为期三个月的旅程，在拥有OpenGL经验的基础上，使用Vulkan构建了一个小型3D游戏引擎EDBR和两个游戏演示。

作者建议先从OpenGL开始学习（推荐learnopengl.com、Anton's Tutorials），以掌握图形学基础知识，然后再应对Vulkan的复杂性。核心建议包括避免“自行车棚效应”——即不要过度设计，从小型游戏入手，先让功能运行起来，之后再进行重构。

由于Vulkan的开源性质和现代功能（不同于已废弃的OpenGL或功能有限的WebGPU），作者选择Vulkan来开发桌面游戏（Windows/Linux），并强调现在Vulkan更易于上手。推荐的主要学习资源包括`vkguide.dev`和维也纳工业大学的Vulkan讲座系列，以及一些高级书籍。`vk-bootstrap`等库因简化了样板代码而受到称赞。

EDBR引擎（1.9万行代码）被描述为专为小型、基于关卡的游戏量身定制。其帧分析涵盖计算蒙皮、级联阴影贴图 (CSM)、基于物理的渲染 (PBR)、深度解析、后处理效果（雾、泛光）和UI渲染。作者的旅程强调了耐心和渐进式学习的重要性，证明了对于专注的自学者来说，使用Vulkan进行开发是可行的。

---

## 33. 降低产品质量，赚钱

**原文标题**: Make product worse, get money

**原文链接**: [https://dynomight.net/worse/](https://dynomight.net/worse/)

本文批判了公司为实现利润最大化而故意将产品质量做差的普遍理论，并以约会应用为例进行了说明。作者认为，“把产品做差赚钱”的观点过于简单且没有帮助，因为它普遍适用于所有业务（例如，披萨、汽车、博客）。尽管生产者天生希望对低成本、劣质商品收取高价，但竞争性市场通常通过迫使公司提供价值来阻止这种情况。

作者指出，真正有趣的问题是：公司 *为什么* 能够通过看似次优的产品来蒙混过关。对此，文章提出了四个主要原因：
1.  **消费者贪图便宜：** 消费者通常优先考虑低价而非高质量（例如，拥挤的飞机座位），这意味着公司提供的是市场所需。
2.  **信息不对称：** 消费者缺乏辨别产品质量的知识，这使得劣质甚至有害的产品（例如，养生骗局、隐藏成分）得以成功。
3.  **消费者品味不佳：** 消费者确实喜欢那些在别人看来可能“糟糕”的产品。
4.  **定价权：** 拥有显著“护城河”（例如，技术壁垒、品牌忠诚度、网络效应）的公司面临的竞争较少，因此改善质量或降低价格的压力也较小。

作者总结道，对于约会应用或任何产品，如果它们确实很差，那么谜团不在于它们的动机，而在于为什么没有更好的竞争对手出现，这暗示着要么是竞争不可能，要么是特定的消费者偏好在起作用。

---

## 34. 皮克斯：早期 前所未见的1996年访谈

**原文标题**: Pixar: The Early Days A never-before-seen 1996 interview

**原文链接**: [https://stevejobsarchive.com/stories/pixar-early-days](https://stevejobsarchive.com/stories/pixar-early-days)

本文介绍了一段史蒂夫·乔布斯（Steve Jobs）1996年的访谈，这段访谈此前从未公开，并将由史蒂夫·乔布斯档案馆（Steve Jobs Archive）于2025年为庆祝《玩具总动员》（Toy Story）上映30周年而发布。该访谈于1996年11月22日进行，正值全球首部完全由电脑制作的动画长片《玩具总动员》首映一年之后。

《玩具总动员》一经推出便大获成功，将皮克斯（Pixar）打造成一家估值15亿美元的上市公司，成为1995年规模最大的首次公开募股（IPO），并荣获一项奥斯卡特别成就奖。访谈进行时，皮克斯正处于快速扩张期：其股价几乎翻了一番，团队规模增长了70%，《虫虫危机》（A Bug’s Life）正在制作中，史蒂夫正利用其影响力重新谈判皮克斯与迪士尼（Disney）的合作关系，为此他关闭了电视广告部门以专注于长片制作。

在访谈中，史蒂夫详细阐述了皮克斯成功背后的“长期策略”（long game）。他讨论了其独特的商业模式，该模式让艺术家和工程师能够在其创作中拥有股份，并分享了从迪士尼那里学到的关于专注和纪律的见解。他还谈到了领导一支颠覆传统层级结构的杰出团队所面临的挑战，留住员工的激励措施，以及他们共同的使命：讲述经久不衰的故事并贡献持久的文化价值。史蒂夫在皮克斯与艾德·卡特姆（Ed Catmull）的紧密合作，尤其关注为人才创造茁壮成长的条件，极大地塑造了他的领导方式。他在皮克斯的经历直接影响了他数周后重返苹果（Apple）担任首席执行官时的愿景，强调要将公司建立在永恒的理念与科技的融合之上。

---

## 35. 繁荣，泡沫，破灭，繁荣。为什么AI会是例外呢？

**原文标题**: Boom, bubble, bust, boom. Why should AI be different?

**原文链接**: [https://crazystupidtech.com/2025/11/21/boom-bubble-bust-boom-why-should-ai-be-different/](https://crazystupidtech.com/2025/11/21/boom-bubble-bust-boom-why-should-ai-be-different/)

文章指出，历时三年的AI革命正在经历一场巨大的科技泡沫，其规模和恐怖程度可能超越1999年的互联网泡沫。作者弗雷德·沃格斯坦和奥姆·马利克借鉴他们互联网泡沫的经验指出，尽管英伟达盈利强劲，但仍存在对快速进展的夸大主张（“AI狗年”），且微软、亚马逊和Meta等主要AI公司的股价近期出现下跌。

他们认为，尽管AI具有深远的长期潜力，但目前的投资与已证实商业模式极不相称。2025年全球AI支出估计（6000亿至1.5万亿美元）远超1999年互联网泡沫的峰值（以2025年美元计算为3600亿美元），且泡沫膨胀所需时间仅为其三分之二。

与1999年公众市场的狂热不同，这次泡沫主要由科技巨头的雄厚财力和私人投资者推动。这种集中、高杠杆以及数据中心面临大规模减记的风险使其“更令人恐惧”。其他担忧包括美国经济不稳定和中国竞争，甚至有行业领袖承认存在“过度投资”。

作者指出了四个主要弱点：支出过高、杠杆过高、疯狂交易和中国。OpenAI被视为一个典型例子：估值5000亿美元（可能达到1万亿美元），每年烧掉数十亿美元（2025年80亿美元，2026年170亿美元），预计在服务器成本达到5000亿美元之后，直到2029年才能实现现金流为正。这种“快速做大”的策略，加上OpenAI的预计支出是亚马逊前五年（调整后）的16倍，预示着一场不可避免的破产，届时输家将多于赢家。

---

## 36. 为什么顶尖公司会解雇优秀员工？

**原文标题**: Why top firms fire good workers

**原文链接**: [https://www.rochester.edu/newscenter/employee-turnover-why-top-firms-churn-good-workers-681832/](https://www.rochester.edu/newscenter/employee-turnover-why-top-firms-churn-good-workers-681832/)

这段文字是罗切斯特大学西蒙商学院的一份宣传声明。它强调该机构致力于采用一种“不折不扣的分析”方法，研究人员和学生将“严谨的分析”应用于“从市场到管理”的各个商业领域。其最终目标是“推进具有现实世界影响力的思想”，并声称他们能促成“更卓越的商业实践”。

值得注意的是，尽管标题提出了“为什么顶尖公司会解雇优秀员工”的问题，但内容本身并未涉及此主题，而是侧重于学院的方法论和使命。

---

## 37. 教育部不将护理学列为“专业”学位

**原文标题**: Nursing excluded as 'professional' degree by Department of Education

**原文链接**: [https://nurse.org/news/nursing-excluded-as-professional-degree-dept-of-ed/](https://nurse.org/news/nursing-excluded-as-professional-degree-dept-of-ed/)

美国教育部(DOE)在针对“有偿就业”(GE)法规的新指南中，将其对“专业学位”的定义中排除护理学位，在护理界引发了争议。尽管医学、法律、牙科乃至兽医学等领域都被明确认定为专业，护理学学士(BSN)、护理学副学士(ADN)和护理学硕士(MSN)课程却明显缺席这一分类。

这一排除带来了重大影响。GE法规旨在保护学生免受那些导致债务过高（相对于其收入潜力）的课程的影响。专业学位通常可免除某些GE报告要求，这意味着护理课程现在可能面临更严格的审查，或被默认为职业而非专业。

包括美国护理学院协会(AACN)、美国护士协会(ANA)、美国护理联盟(NLN)和美国护理领导组织(AONE)在内的主要护理组织，正在强烈抗议这一决定。他们认为，护理是一项高度专业化、以科学为基础的职业，对医疗保健不可或缺，并且这一疏忽贬低了该专业、其严谨的教育及其重要的社会作用。护理界领导者正敦促DOE纠正这一错误，强调BSN是专业实践的入门级要求，并倡导将护理正式认定为一门专业学科。

---

## 38. 在 Proxmox 9.1 中原生运行 Docker 容器 (OCI 镜像)

**原文标题**: Run Docker containers natively in Proxmox 9.1 (OCI images)

**原文链接**: [https://raymii.org/s/tutorials/Finally_run_Docker_containers_natively_in_Proxmox_9.1.html](https://raymii.org/s/tutorials/Finally_run_Docker_containers_natively_in_Proxmox_9.1.html)

Proxmox VE 9.1 引入了一项新功能，允许用户更“原生”地运行 Docker 容器（OCI 镜像），无需单独的虚拟机或易出错的 Docker-in-LXC 配置。Proxmox VE 通过将 OCI 镜像转换为标准 LXC 容器来实现此功能，并利用 `skopeo` 等工具进行转换。

作为一项技术预览功能，它目前存在一些限制：不支持实时迁移或容器编排，并且镜像层在创建时会被扁平化处理，这意味着直接更新（例如 `docker pull`）并不直接，通常需要重新创建容器。尽管容器的控制台可能不总能提供 shell 访问，但可以使用 `pct enter` 进入。环境变量可在创建后配置，但不能在初始化期间配置，并且不支持 `docker-compose` 文件。

该过程主要包括两个步骤：
1.  **下载 OCI 镜像：** 在 Proxmox GUI 中，导航到您的存储，点击“从 OCI 注册表拉取”（Pull from OCI Registry），然后输入完整的镜像 URL（例如 `docker.io/eclipse-mosquitto`）。
2.  **创建容器：** 使用“创建 CT”（Create CT）按钮，选择已下载的 OCI 镜像作为模板，并配置用于持久化数据的卷（类似于 Docker 的 `-v` 选项）以及其他标准 LXC 设置。

Proxmox VE 在容器创建过程中会自动处理转换。尽管存在底层转换和当前的局限性，但此功能显著简化了在 Proxmox VE 上直接运行应用程序容器的过程，从而为用户节省了大量时间。

---

## 39. 新AI意识论文

**原文标题**: The New AI Consciousness Paper

**原文链接**: [https://www.astralcodexten.com/p/the-new-ai-consciousness-paper](https://www.astralcodexten.com/p/the-new-ai-consciousness-paper)

该文章批评了围绕AI意识的讨论普遍质量低下，并重点提到Yoshua Bengio和David Chalmers在《认知科学趋势》上发表的一篇新论文，认为其是罕见的“亮点”。该论文仅限于探讨意识的计算理论，例如循环处理理论（RPT）、全局工作空间理论（GWT）和高阶理论（HOT），这些理论都涉及某种形式的“反馈”。

基于一份相关的技术报告，作者们初步得出结论，尽管当前的AI系统（如大多采用前馈架构的大语言模型）不具备意识，但在技术上“没有明显障碍”来构建满足这些计算指标的未来AI系统（例如MaMBA等架构）。

然而，评论者批评了该论文的哲学贡献。论文正确地区分了“可通达意识”（即一个人能报告或内省的内容）和“现象意识”（即内部体验，其主观感受）。尽管AI可能展现出初步的可通达意识（例如Anthropic的“测谎仪”测试），但关键问题在于现象意识。评论者认为，尽管论文承认了这一区别，但最终却“含糊处理”，将更适合描述可通达意识的计算理论解释为现象意识的指标。这导致了荒谬的结论，例如根据这些标准，一家公司或一个麦克风反馈回路可能被认为是具有现象意识的，揭示了计算指标与内在体验的难以捉摸的本质之间存在根本性的不匹配。

---

## 40. 苔藓太空真空存活9个月

**原文标题**: Moss Survives 9 Months in Space Vacuum

**原文链接**: [https://scienceclock.com/moss-survives-9-months-in-space-vacuum/](https://scienceclock.com/moss-survives-9-months-in-space-vacuum/)

科学家们发现，匍匐土藓 (Physcomitrium patens) 的孢子能在外太空的恶劣环境下存活长达九个月。研究人员将这种小型苔藓的孢子胶囊安装在国际空间站 (ISS) 的外部，使其暴露于太阳直接辐射、真空和极端温度波动之中。

令他们惊讶的是，超过80%的孢子在返回地球后成功发芽，这一存活率远高于预期“几乎为零”的水平。这些孢子仅表现出叶绿素 a 的轻微下降，并且在其他方面生长正常，表明它们在轨道上没有受到重大压力。

这种非凡的韧性归因于苔藓植物（包括苔藓、地钱和角苔）的进化史，它们是大约5亿年前首批在陆地定居的植物之一，进化出了抵抗干燥和阳光直射的保护结构。

这些发现将苔藓孢子与水熊虫和某些微生物等少数已知能耐受直接太空暴露的生物并列。这种顽强性对于理解生命在极端地外环境中的潜力具有重要意义。研究人员认为，苔藓只需少量土壤即可生长，并能从岩石中提取养分，这使其成为在月球或火星上建立早期生态系统的主要候选者，为地外殖民开辟了“新前沿”。该研究发表在《iScience》杂志上。

---

## 41. 矩阵乘法丑陋吗？

**原文标题**: Is Matrix Multiplication Ugly?

**原文链接**: [https://mathenchant.wordpress.com/2025/11/21/is-matrix-multiplication-ugly/](https://mathenchant.wordpress.com/2025/11/21/is-matrix-multiplication-ugly/)

文章反驳了斯蒂芬·威特关于矩阵乘法因其不具备交换律 (AB ≠ BA) 而“很丑”的说法。作者认为威特误解了矩阵，矩阵本质上是关于“变换”的，尤其是像反射这样的几何变换。

矩阵乘法代表了这些变换的复合。作者证明了变换的应用顺序自然会影响结果（例如，先翻转图像再反射与先反射再翻转会得到不同的结果）。因此，AB ≠ BA并非缺陷，而是反映变换本质的内在而优雅的特性。矩阵理论非但不缺乏对称性，反而是理解对称性的重要工具。

作者推测，威特对“丑陋”的看法源于手动矩阵计算的*繁琐*，而非概念本身。他澄清说，威特所引用的数学家G. H. Hardy，不喜欢数学*证明*中的冗长计算，而非数学概念或其实际应用。重复且“令人心力交瘁”的计算工作，与矩阵代数的概念之美和强大功能是截然不同的，矩阵代数现在支撑着人工智能等领域。计算机处理繁琐的计算，从而保留了矩阵的概念之美。

---

## 42. 新的物理学模型有望带来更清晰的核磁共振成像。

**原文标题**: Sharper MRI scans may be on horizon thanks to new physics-based model

**原文链接**: [https://news.rice.edu/news/2025/sharper-mri-scans-may-be-horizon-thanks-new-physics-based-model](https://news.rice.edu/news/2025/sharper-mri-scans-may-be-horizon-thanks-new-physics-based-model)

莱斯大学研究人员开发了一种新的基于物理的模型，有望带来更清晰的核磁共振（MRI）扫描。该模型旨在克服MRI技术的一个根本性局限：图像清晰度与扫描速度之间的权衡。目前，获取高分辨率图像通常需要更长的扫描时间，这使得该过程对患者来说实用性降低，并且更容易受到运动伪影的影响。

由电气与计算机工程师Ashok Veeraraghavan和物理学家Anatoly Kolomensky领导的莱斯大学团队开发了一种算法，可以从现有的低分辨率、有噪声的MRI数据中提取更多信息。他们的模型利用了量子力学原理，具体来说是量子态本质上是稀疏的，并且可以用有限的参数集来描述这一概念。通过将检测到的信号视为量子态，他们的算法即使从稀疏的测量数据中也能重建高保真图像。

这种新方法有潜力显著提高核磁共振扫描的质量，而无需硬件升级或延长扫描时间。它可以带来更清晰的图像，用于诊断癌症和神经系统疾病等病症，同时使扫描过程对患者来说更舒适、更高效。研究人员目前正在致力于将该模型应用于重建3D图像，并探索其在各种医学成像应用中的潜力。

---

## 43. Jmail：Gmail 克隆版，含爱泼斯坦的邮件

**原文标题**: Jmail: Gmail Clone with Epstein's Emails

**原文链接**: [https://jmail.world](https://jmail.world)

所提供的内容模拟了一个名为“Jmail”、类似于Gmail的界面，该界面以“Jeffrey Epstein, [email protected]”的身份登录，并展示了“国会发布的真实电子邮件”。该平台允许用户通过姓名浏览邮件、给邮件加星标、搜索，或随机查看2235条条目。

所展示的电子邮件主要来自2018-2019年，内容混合了新闻阅读和私人通信。许多条目是来自Quora和Flipboard的摘要，涵盖了当前事件，例如穆勒调查、爱泼斯坦被捕后亚历克斯·阿科斯塔的辞职、全球政治（如金正恩-特朗普会晤）以及经济新闻。

值得注意的个人通信对象包括史蒂夫·班农、伊藤穰一和保罗·莫里斯。他们的交流涉及资本市场前景、学术馈赠和政治评论等话题。有几封电子邮件直接与爱泼斯坦的法律背景相关，例如一篇题为“爱泼斯坦案检察官因先前儿童性侵案受指责”的转发文章，以及尼古拉斯·里比斯发来的一条消息，写道“对我们的朋友来说是更多的坏消息”。此外，还有多处提及唐纳德·特朗普，包括关于“特朗普在战争中”和“唐纳德·特朗普的重罪和轻罪”的文章，通常附有爱泼斯坦或班农的简短评论。该界面让人们得以一窥爱泼斯坦在此期间的数字通信以及他所关注的新闻。

---

## 44. 谋智表示终于与Onerep了结了

**原文标题**: Mozilla says it's finally done with Onerep

**原文链接**: [https://krebsonsecurity.com/2025/11/mozilla-says-its-finally-done-with-two-faced-onerep/](https://krebsonsecurity.com/2025/11/mozilla-says-its-finally-done-with-two-faced-onerep/)

Mozilla 在拖延了16个月之后，终于终止了与身份保护服务 Onerep 的合作。该决定源于 KrebsOnSecurity 在2024年3月的一项调查，该调查揭示 Onerep 的创始人 Dimitri Shelest 还创建并运营了众多人员搜索服务，其中包括活跃的数据经纪公司 Nuwber。

尽管 Mozilla 最初在2024年3月宣布将逐步停止合作，但它却继续推广 Onerep。本周，Mozilla 证实该合作将于下个月正式结束。因此，其通过 Onerep 提供自动数据删除的“Monitor Plus”服务将停止。

Mozilla 将继续提供其免费的“Monitor”数据泄露服务，并计划将更多隐私功能（例如其 VPN）直接集成到 Firefox 中。现有的 Monitor Plus 订阅用户将保留全部访问权限直至2025年12月17日，此后将获得按比例退款。Mozilla 表示，维护高标准的供应商以及数据经纪生态系统的复杂性，使其难以持续提供预期的价值和可靠性。Shelest 曾承认他在 Nuwber 持有所有权股份，该公司于2015年与 Onerep 大致同时成立。

---

## 45. 麦当劳正在失去低收入顾客

**原文标题**: McDonald's is losing its low-income customers

**原文链接**: [https://www.latimes.com/business/story/2025-11-16/mcdonalds-is-losing-its-low-income-customers](https://www.latimes.com/business/story/2025-11-16/mcdonalds-is-losing-its-low-income-customers)

快餐价格大幅上涨，导致麦当劳和整个行业失去了其核心的低收入客户群。这些顾客正越来越多地被高收入者取代，麦当劳首席执行官克里斯托弗·肯普钦斯基证实了这一趋势，他指出低收入顾客流量出现了两位数的下降。

从2019年到2024年，麦当劳菜单商品的平均价格上涨了40%。这一涨幅归因于劳动力和牛肉等餐厅必需品成本的飙升（受干旱、关税以及肉类行业涉嫌价格操纵的影响），同时住房、育儿和食品杂货等方面的普遍通胀也加剧了这一情况。

低收入家庭，特别是年收入低于4.5万美元的家庭，受到了严重影响。他们面临信贷违约“同比大幅增长”的情况，并且一半的租房者承受着过高的租金负担，将超过30%的收入用于住房。对于年收入低于3万美元的人来说，用于其他需求的剩余收入已降至每月中位数仅250美元。这凸显了“K型经济”的特点，即富裕消费者保持消费，而低收入个人则削减开支。

历史上，麦当劳在21世纪初通过其“一元菜单”实现了重大转机，特别吸引了精打细算的消费者。然而，由于通货膨胀，这一菜单变得不可持续。麦当劳最近尝试通过5美元套餐和其他超值优惠来吸引手头拮据的顾客，尽管近期销售额略有提升，但结果喜忧参半。

经济学家警告称，经济和政策逆风不成比例地影响着低收入家庭，使得可负担性成为一个紧迫的问题。企业不愿进一步转嫁价格上涨的成本，因为他们认识到，在经历了多年的通货膨胀后，消费者已所剩无几的忍耐度。

---

## 46. 小罗伯特·F·肯尼迪的恶劣修改：疾控中心网站现竟虚假地将疫苗与自闭症联系起来

**原文标题**: RFK Jr.'s loathesome edits: CDC website now falsely links vaccines and autism

**原文链接**: [https://arstechnica.com/health/2025/11/rfk-jr-s-loathesome-edits-cdc-website-now-falsely-links-vaccines-and-autism/](https://arstechnica.com/health/2025/11/rfk-jr-s-loathesome-edits-cdc-website-now-falsely-links-vaccines-and-autism/)

在小罗伯特·F·肯尼迪担任该国最高卫生官员的领导下，疾控中心（CDC）的“自闭症与疫苗”网页突然被修改，错误地暗示疫苗与自闭症之间存在关联。此前，该网站准确指出研究显示“接种疫苗与患上自闭症谱系障碍（ASD）之间没有关联”。现在，它声称“‘疫苗不会导致自闭症’这一说法并非基于证据的主张，因为研究尚未排除婴儿疫苗导致自闭症的可能性。”

预计此举将播下不信任的种子，侵蚀疫苗接种率，并导致更多疾病。卫生与公众服务部（HHS）将这些修改归因于“黄金标准、循证科学”，但据报道，疾控中心的职业科学家并未被征求意见。更新后的页面断章取义地选择边缘研究，歪曲旧数据，并错误地牵连铝佐剂，甚至在不含铝佐剂的疫苗中也如此。它忽视了一项近期针对120万儿童的高质量研究，该研究驳斥了铝的关联性，而肯尼迪曾要求撤回该研究但未成功。

医学专家对此表示震惊和愤怒。美国儿科学会通过其主席苏珊·克雷斯利（Susan Kressly）严厉抨击了这些修改，重申超过40项涉及560万人的高质量研究证实“疫苗与自闭症之间没有关联”。克雷斯利指责那些宣扬这一神话的人“要么被误导，要么是蓄意误导家长”，并敦促疾控中心停止放大虚假主张。

---

## 47. Gmail 可以读取你的电子邮件和附件来训练其人工智能，除非你选择退出。

**原文标题**: Gmail can read your emails and attachments to train its AI, unless you opt out

**原文链接**: [https://www.malwarebytes.com/blog/news/2025/11/gmail-is-reading-your-emails-and-attachments-to-train-its-ai-unless-you-turn-it-off](https://www.malwarebytes.com/blog/news/2025/11/gmail-is-reading-your-emails-and-attachments-to-train-its-ai-unless-you-turn-it-off)

谷歌据报道已开始默认让Gmail用户选择加入，允许其私人邮件和附件用于训练包括Gemini在内的人工智能模型。此举旨在为Gmail的新功能（如智能撰写和AI生成回复）提供支持，意味着用户数据可能被分析以改进谷歌的AI助手。

这一改变正在悄然推出，设置默认开启，用户若不希望自己的邮件被用于AI训练，需要手动选择退出。尽管谷歌承诺采取匿名化等隐私措施，但缺乏明确同意和敏感信息的使用，引发了许多人对隐私的重大担忧，即便这可能带来更智能、更个性化的Gmail功能。

要完全选择退出，用户必须在两个不同的位置调整设置：
1.  **关闭“Gmail、Chat 和 Meet 中的智能功能”**：前往Gmail设置，找到此部分，取消勾选该选项并保存。
2.  **关闭“Google Workspace 智能功能”**：仍在设置中，导航至“管理 Workspace 智能功能设置”，然后关闭“Google Workspace 中的智能功能”和“其他 Google 产品中的智能功能”这两个选项，并保存。

同时禁用这两个选项至关重要，因为一个涵盖Workspace应用（邮件、聊天、会议），另一个则涵盖其他Google产品中的智能功能。用户应核实这两个开关都保持关闭状态。谷歌正在逐步推行此功能，因此虽然并非所有用户的设置都已启用，但建议关注隐私的用户检查一下。

---

## 48. PNG图像中的EXIF方向信息不用于`image-orientation: from-image`。

**原文标题**: EXIF orientation info in PNGs isn't used for image-orientation: from-image

**原文链接**: [https://bugzilla.mozilla.org/show_bug.cgi?id=1627423](https://bugzilla.mozilla.org/show_bug.cgi?id=1627423)

这份题为“PNG中的EXIF方向信息未用于`image-orientation: from-image`”的bug报告，描述了一个问题，即当应用`image-orientation: from-image`时，浏览器（尤其是Firefox）未能根据PNG图像中嵌入的EXIF数据正确地调整其方向。

该报告由Eric Portis于五年前提交，报告者演示了包含相同EXIF“旋转90度顺时针”方向信息的一张JPEG图像和一张PNG图像在浏览器中显示不同。JPEG图像正确旋转，而PNG图像则没有，这与预期相反。

进一步调查显示，尽管PNG规范（PNG-3）为EXIF数据定义了一个`eXIf`数据块，但它在文件中的位置（在图像数据之前或之后）影响了浏览器的解释。当时，Firefox和Chrome完全不遵守PNG中的EXIF方向信息，而Safari只有当EXIF数据出现在图像数据之前时才遵守。`eXIf`数据块被认为是一个有效但不太常见的PNG扩展。

这个bug的状态随着时间而改变，阻塞了其他几个相关问题。它最终在两个月前被标记为“RESOLVED DUPLICATE”（已解决，重复），表明该问题已作为另一个bug（Bug 1682759）的一部分得到处理和修复。这表明，现在预计已实现正确解释PNG中EXIF方向信息的功能。

---

## 49. 脱欧冲击英国经济达官方估算两倍，研究发现

**原文标题**: Brexit Hit to UK Economy Double Official Estimate, Study Finds

**原文链接**: [https://www.bloomberg.com/news/articles/2025-11-21/brexit-hit-to-uk-economy-double-official-estimate-study-finds](https://www.bloomberg.com/news/articles/2025-11-21/brexit-hit-to-uk-economy-double-official-estimate-study-finds)

一项由英格兰银行高级经济学家合著的新研究表明，与官方估计相比，英国脱欧给英国造成的经济损失几乎是官方估计的两倍。

该研究已提交给预算责任办公室（OBR），并计算得出，2016年投票脱离欧盟在过去十年中使英国人均GDP损失了6%至8%。这相当于1800亿英镑（2350亿美元）到2400亿英镑的经济损失。相比之下，预算责任办公室（OBR）——政府的独立预测机构——目前估计损失为GDP的4%。

---

## 50. 注意力缺陷多动障碍 和 单一模式 (2023)

**原文标题**: ADHD and monotropism (2023)

**原文链接**: [https://monotropism.org/adhd/](https://monotropism.org/adhd/)

文章探讨了注意力缺陷多动障碍（ADHD）与单向聚焦理论之间的潜在联系，后者最初是为解释自闭症体验而提出的，即倾向于将注意力集中在少数事物上。尽管诊断标准不同——ADHD侧重于注意力，自闭症侧重于社交，且存在刻板兴趣与冲动性等看似矛盾的特质——许多被诊断为ADHD的人强烈认同单向聚焦理论。

作者弗格斯·默里提出，自闭症和ADHD，或称“动力认知风格（KCS）”，可能共享一个潜在的单向聚焦原因。他认为，ADHD的特质，如冲动性、注意力不集中和多动性，可能源于一种单向聚焦的处理风格。冲动性可能源于注意力转移时意识的丧失，而注意力不集中则源于难以将注意力从当前兴趣中转移开。多动性，无论是需要移动（如刻板行为）还是认知上的“注意力跳跃”，都可以通过将单向聚焦理论与难以进入心流状态、高度寻求新奇或快速的“连续单向聚焦”等因素结合起来加以调和。

文章指出，外在表现严重影响当前的诊断，这可能掩盖了那些发展出应对机制的个体中潜在的单向聚焦认知风格。尽管具有推测性，但单向聚焦理论与ADHD和自闭症之间显著的重叠和强烈相关性，值得未来进行广泛研究，以从内部、认知的角度而非仅仅是表面观察来理解这些神经多样性。

---

## 51. 美国海岸警卫队不再将万字符、绞索认定为仇恨符号

**原文标题**: U.S. Coast Guard will no longer classify swastikas, nooses as hate symbols

**原文链接**: [https://www.washingtonpost.com/national-security/2025/11/20/coast-guard-swastika-noose/](https://www.washingtonpost.com/national-security/2025/11/20/coast-guard-swastika-noose/)

无法访问文章链接

---

## 52. “法国人想救我们”：玻璃制造商杜拉丽获援助如潮

**原文标题**: 'The French people want to save us': help pours in for glassmaker Duralex

**原文链接**: [https://www.theguardian.com/world/2025/nov/22/french-people-want-to-save-us-help-pours-glassmaker-duralex](https://www.theguardian.com/world/2025/nov/22/french-people-want-to-save-us-help-pours-glassmaker-duralex)

法国玻璃制造商杜拉乐士（Duralex）是一个唤起人们深深怀旧情感和民族自豪感的品牌，它获得了惊人的公众支持，仅在5小时40分钟内就筹集到了500万欧元的紧急资金目标。随后的认捐额飙升至逾1900万欧元，但作为一家员工合作社，杜拉乐士只能接受最初的500万欧元。

总经理弗朗索瓦·马西亚诺表示，这一反响“让所有人感到震惊”，他将其归因于“法国人民想拯救我们。他们厌倦了工厂倒闭。”这一成功是在杜拉乐士在二十年内四次面临破产管理之后取得的，马西亚诺在18个月前领导了一次员工收购，使243名员工中的180人成为合作社成员。

这次呼吁引发了“订单海啸”，工厂现在难以跟上生产。杜拉乐士以其高度耐用、可用于微波炉、冰箱和洗碗机的玻璃器皿而闻名，尤其是其标志性的皮卡第（Picardie）玻璃杯，被誉为设计经典。其制造工艺自1945年以来基本未变，包括将原材料加热到1400摄氏度以及严格的质量控制。

尽管筹集到了资金，高昂的天然气和电力成本仍然是一个重大担忧。这500万欧元将用于工厂现代化改造和新产品开发，包括与爱丽舍宫（法国总统府）的合作，并计划通过品脱杯进军英国和美国市场，同时认识到在海外建立品牌知名度的挑战。该公司希望到2027年实现收支平衡，自成为合作社以来，其营业额已增长了22%。

---

## 53. 德国：各州通过操作系统色情过滤器

**原文标题**: Germany: States Pass Porn Filters for Operating Systems

**原文链接**: [https://www.heise.de/en/news/Youth-Protection-States-Pass-Porn-Filters-for-Operating-Systems-11086768.html](https://www.heise.de/en/news/Youth-Protection-States-Pass-Porn-Filters-for-Operating-Systems-11086768.html)

德国各州（Länder）通过了一项法案，要求在德国销售的操作系统必须包含一个预装的“色情过滤器”，作为其青少年保护措施的一部分。该过滤器旨在屏蔽“危害青少年内容”，默认情况下处于非活动状态，需要用户明确激活，这可能涉及年龄验证过程。

该提案遭到了大量批评，特别是来自混沌电脑俱乐部（CCC）和其他数字权利倡导者的批评。批评者认为，此类过滤器在技术上无效，易于规避，并可能制造一种虚假的安全感，同时可能导致审查或监控。他们还对操作系统制造商的技术可行性以及“危害青少年内容”的宽泛定义表示担忧。

尽管存在这些反对意见，但各州的决定反映了其在加强在线青少年保护方面的持续努力。该法案尚未成为法律，在生效前仍需经过进一步的立法阶段，包括获得联邦议院的批准。这场辩论凸显了保护未成年人与维护数字自由及技术现实之间的紧张关系。

---

## 54. 罗布乐思CEO在翻车采访中出洋相

**原文标题**: Roblox CEO Makes a Fool of Himself in Car-Crash Interview

**原文链接**: [https://kotaku.com/roblox-new-york-times-interview-baszucki-2000646174](https://kotaku.com/roblox-new-york-times-interview-baszucki-2000646174)

罗布乐思首席执行官戴维·巴斯祖奇在《纽约时报》的《Hard Fork》播客上接受了一次备受批评的“灾难性”采访，他在日益增加的法律压力和被指控为“恋童癖地狱”的背景下，讨论了儿童安全问题。罗布乐思正在推行新的面部识别技术用于聊天年龄验证，但巴斯祖奇的回应被认为是不合时宜且语无伦次的。

当被问及掠食者的“问题范围”时，巴斯祖奇竟将其称作一个“机会”。他对新的身份验证措施含糊其辞，避开关于在实施基本安全措施方面19年延误的问题，经常以罗布乐思拥有1.5亿用户作为借口。当被追问现有过滤器的无效性时，他变得语无伦次，拒绝评论诉讼，并暗示“老练”的用户或年龄较大的孩子会绕过过滤器。他否认存在掠食者问题，反而将重点放在“创新”上。

后来，当讨论兴登堡研究公司关于安全开支的报告时，巴斯祖奇变得公然带有敌意且不成熟，他要求采访者同意人工智能（现在是罗布乐思安全战略的核心）是优越的，并嘲讽地要求“击掌”。最具争议的是，他表示有兴趣将基于加密骗局的预测市场Polymarket整合到罗布乐思中，让孩子们以“合法”和“教育性”的方式“赌博”，这一提议被主持人公开嘲笑。文章总结称，巴斯祖奇对他平台严重的安全性问题仍然毫无准备且脱节，优先考虑增长和投资者担忧，而非儿童保护。

---

## 55. 我们也在一片死寂的互联网中依然存活。

**原文标题**: We remain alive also in a dead internet

**原文链接**: [https://slavoj.substack.com/p/why-we-remain-alive-also-in-a-dead-954](https://slavoj.substack.com/p/why-we-remain-alive-also-in-a-dead-954)

斯拉沃热·齐泽克的《为何我们仍在“死寂互联网”中生存》深入探讨了流行的“死寂互联网理论”——即互联网如今主要由AI生成内容和机器人占据，从而减少了真实的人类互动。齐泽克并未将其斥为单纯的阴谋论，而是将其作为哲学跳板，通过拉康精神分析的视角进行解读。

他提出互联网并非真正“已死”，而是“不死”，如同僵尸一般。齐泽克认为，这种“不死”的特质映照了拉康的“实在界”（the Real）概念——一个创伤性、无意义、侵入性的存在，它抵抗符号化和想象。大量的AI内容代表了这种实在界的一种新表现，一种持续的“凝视”（gaze），即使我们认识到其人工性，它也悄然塑造着我们的感知和欲望。

齐泽克主张，这个“死寂互联网”并非促使我们简单地拒绝AI或退回到对纯粹人类真实性的追求。相反，它挑战我们去正视即使在人类现实本身中也存在的内在“死寂”或“匮乏”（lack）。他指出，真正的人类自由和生命力在于认识并参与到数字领域和我们自身主体性的这种“不死”维度中，让它重新定义我们对“活着”的理解，并培育新形式的创造力和联结。

---

## 56. 私募股权新业务：青少年体育

**原文标题**: Private Equity's New Venture: Youth Sports

**原文链接**: [https://jacobin.com/2025/11/youth-sports-hockey-private-equity](https://jacobin.com/2025/11/youth-sports-hockey-private-equity)

私募股权公司正日益主导价值400亿美元的青少年体育产业，将其转变为以利润为导向的商业企业，令许多家庭望而却步。一个主要例子是，企业拥有的设施和联盟——尤其是在冰球运动中——日益普遍地禁止家长录制孩子比赛。相反，像最大的冰球场馆所有者兼运营商Black Bear Sports Group这样的公司，强迫家长订阅他们独有的流媒体服务，其费用可能远高于专业体育赛事的订阅费。

康涅狄格州民主党参议员克里斯·墨菲强调了这个问题，他讲述了在一个Black Bear旗下的冰球场馆，他孩子的球队曾因未经授权的直播而面临处罚的威胁。Black Bear还收取额外费用，例如50美元的“注册和保险”费，这进一步增加了青少年体育已经飞涨的成本。现在，普通家庭每年在孩子的主要体育项目上花费超过1000美元，其中冰球平均超过2500美元，这使得低收入家庭难以承担。

其他公司，如Unrivaled Sports和贝恩资本支持的Varsity Brands（啦啦队），也采用类似的策略，整合市场，控制场馆、设备和流媒体版权。Varsity Brands甚至因涉嫌反竞争行为而面临反垄断诉讼。批评者认为，这些私募股权策略将投资者利润置于儿童发展之上，导致服务质量下降，并制造了“可负担性危机”，使青少年体育成为一项奢侈活动。

---

## 57. GitHut — 编程语言与GitHub (2014)

**原文标题**: GitHut – Programming Languages and GitHub (2014)

**原文链接**: [https://githut.info/](https://githut.info/)

GitHut 是 Carlo Zapponi 在2014年发起的一个项目，它是一个可视化工具，旨在探索和理解全球最大代码托管平台 GitHub 上各个代码仓库中使用的编程语言的“宇宙”。其主要目标是揭示语言的流行度、独特特性，以及软件开发中为实现更好的问题解决和协作而进行的历史探索。

GitHut 的定量数据每季度从 GitHub Archive 收集，GitHub Archive 聚合了公开的 GitHub API 数据，可通过 Google BigQuery 访问。为了衡量语言的流行度，GitHut 利用了“活跃度值”，该值被定义为推送到代码仓库的更改次数。选择此指标是因为“创建事件”（新代码仓库创建）通常缺乏指定的语言信息，使其不适合追踪流行语言。编程语言的发布年份则来自维基百科。

GitHut 强调，编程语言不仅仅是工具，更是反映创造力和促进人类协作的媒介。该项目旨在深入探讨语言的使用方式、演变历程以及它们在开源社区中的作用。该作品采用知识共享署名-非商业性使用-相同方式共享（CC BY-NC-SA）许可协议。

---

## 58. Arduino 服务条款和隐私政策更新：以正视听

**原文标题**: Arduino Terms of Service and Privacy Policy update: setting the record straight

**原文链接**: [https://blog.arduino.cc/2025/11/21/the-arduino-terms-of-service-and-privacy-policy-update-setting-the-record-straight/](https://blog.arduino.cc/2025/11/21/the-arduino-terms-of-service-and-privacy-policy-update-setting-the-record-straight/)

Arduino已回应社区对其服务条款和隐私政策近期更新的担忧，重申其20年来对开源原则的坚定承诺。该公司明确表示，高通的收购不会改变用户数据处理或开源实践。

Arduino澄清，所有此前开源的硬件、软件、工具和库仍然保持开源。逆向工程的限制专门适用于其软件即服务（SaaS）云应用程序，而非开源组件。用户也保留其在Arduino平台发布内容的权利。

此次更新旨在提高清晰度、符合法规并支持创新环境。主要变化包括：
*   **增强透明度：** 更精确的数据实践披露。
*   **新产品功能：** 反映了可选AI驱动功能的引入（例如Arduino UNO Q、Arduino App Lab）。
*   **商业条款：** 澄清高级服务的计费、循环付款和退款权利。
*   **法律合规：** 解决美国隐私法、出口管制和全球标准问题。
*   **未成年人数据和隐私：** 加强保护、更新数据保留政策和年龄限制。不活跃账户将在24个月后停用，论坛用户名将保留用于内容归属，除非用户要求完全删除账户。

Arduino鼓励用户阅读完整文件、查阅常见问题解答或联系`privacy@arduino.cc`以获取更多问题解答，并强调其致力于建立一个开放和协作的社区。

---

## 59. OOP 正在领域间转移，并非消失。

**原文标题**: OOP is shifting between domains, not disappearing

**原文链接**: [https://blog.jsbarretto.com/post/actors](https://blog.jsbarretto.com/post/actors)

文章认为，面向对象编程（OOP）并未消亡，而是正在将其核心原则——减少信息流和强制组件间分离——转移到新的领域，作者认为这是一个负面发展。

历史上，OOP的发展是为了管理程序内部的复杂性并促进协作，利用接口、封装、继承和多态来控制组件如何交互。然而，随着分布式系统的兴起以及程序与开发者之间信任的瓦解，隔离的需求从语言层面的结构转向了进程和网络边界。

这种转变在微服务、Docker和Kubernetes等现代范式中显而易见。作者认为，这种分布式对OOP的“替代”，尽管对传统OOP持怀疑态度，却复制了其缺陷，并将其放大了十倍。OpenAPI规范、Docker Compose和Kubernetes等概念实质上是OOP内部机制的外部化版本，但伴随着显著增加的开销。组件间通信现在带来了众多故障模式、缓慢的（反）序列化、内核调度和网络延迟。作者总结道，尽管他们不相信OOP最初的承诺，但对于那些取代OOP的分布式系统所带来的被放大的复杂性和低效率，他们“更难信服”。

---

## 60. 科技理想主义的破灭与北加州无家可归者的崛起

**原文标题**: The death of tech idealism and rise of the homeless in Northern California

**原文链接**: [https://lithub.com/on-the-death-of-tech-idealism-and-rise-of-the-homeless-in-northern-california/](https://lithub.com/on-the-death-of-tech-idealism-and-rise-of-the-homeless-in-northern-california/)

文章《北加州科技理想主义之死（以及无家可归者之增多）》记载了硅谷乌托邦愿景的急剧衰落以及伴随而来的无家可归者数量的激增。作者讲述了他拜访一位前客户，一位风险投资家，此人已从一个富有魅力的进步主义者演变为一个愤世嫉俗的自由意志主义者，满口粗话，并将解决无家可归问题的努力斥为低效和不切实际的理想主义。这位风投认为，“创新者”本能够解决问题，如果不是因为“无能的”公共部门和非营利组织，他坚称只有利润动机才能驱动解决方案。

作者十二年前因加州高昂的住房成本而逃离，他重返故地，发现房地产价格翻了三倍，无家可归现象猖獗，甚至在他曾经的家园圣克鲁斯也是如此。他将这位风投目前的蔑视与硅谷根植于反主流文化理想主义的历史根源进行对比。早期的科技先驱，如史蒂夫·乔布斯和斯图尔特·布兰德（《全球概览》的创始人），将嬉皮士价值观与技术融合，设想计算机是实现个人解放和社区建设的工具，一种“新公社主义梦想”。

然而，这种理想主义，往往掩盖着个人主义，已经变质。像布兰德这样的人物现在为杰夫·贝佐斯等科技巨头打造精心设计的项目，这反映出向智力傲慢的转变。硅谷，这个曾经遍布果园的“心悦谷”，变成了建立在军事工业复合体基础上的科技中心，国防工业的“DNA”根植于当今的巨头企业之中。文章强调了科技乌托邦主张的残酷讽刺，其背景是不平等日益加剧、环境恶化（海湾上空那片“屁云”），以及在企业园区阴影下对无家可归者营地的推土机式拆除。

---

## 61. 阿尔杜伊诺不为人知的历史 (2016)

**原文标题**: The Untold History of Arduino (2016)

**原文链接**: [https://arduinohistory.github.io/](https://arduinohistory.github.io/)

赫尔南多·巴拉甘撰写本文，旨在澄清Wiring和Arduino的历史，纠正错误信息并提供有据可查的事实。他于2003年在伊夫雷亚交互设计学院（IDII）创作了Wiring作为其硕士论文，导师是马西莫·班齐和凯西·里亚斯。其目的是为艺术家和设计师简化电子学，抽象化复杂性，使他们能专注于自己的项目。

Wiring引入了关键要素：一个基于Processing的简单集成开发环境（IDE），一种用于微控制器的用户友好型编程语言（包含`pinMode()`、`digitalWrite()`等命令），开源软件，以及基于Atmel微控制器的硬件设计。巴拉甘详细介绍了设计过程，包括硬件原型——从Javelin Stamp到Atmel ATmega128，其中整合了布赖恩·迪恩的"avrdude"和FTDI用于USB通信。首个Wiring板设计于2004年初问世，有25块板子经过手工焊接和测试。

Wiring获得了显著关注，特别是在2004年末IDII的"Strangely Familiar"项目之后；到2005年，它已在全球范围内使用。

2005年，马西莫·班齐、大卫·梅利斯和大卫·夸蒂列斯分叉（复制）了Wiring的源代码以创建Arduino，并增加了对更便宜的ATmega8微控制器的支持。巴拉甘表示他从未被邀请加入Arduino团队，他觉得这次分叉令人费解，因为他原本计划整合此类开发。吉安卢卡·马蒂诺后来加入Arduino负责制造。尽管分道扬镳，巴拉甘继续了Wiring的开发，而Wiring的许多改进后来被合并到Arduino的代码库中，巴拉甘认为这种情况是多余的。他后来合著了一本书的章节，其中引用了Wiring和Arduino。

---

## 62. 老年人口激增，养老服务难以跟上。

**原文标题**: The senior population is booming. Caregiving is struggling to keep up

**原文链接**: [https://www.cnbc.com/2025/11/21/senior-caregiving-labor.html](https://www.cnbc.com/2025/11/21/senior-caregiving-labor.html)

美国老年人口正在激增，65岁及以上人口比例从2004年的12.4%增至2024年的18%。这一激增主要归因于“婴儿潮”一代的老龄化，对老年护理产生了前所未有的需求，而劳动力市场正努力应对这种需求。贝丝·平斯克（Beth Pinsker）等人的亲身经历凸显了价格飞涨和服务质量下降的趋势。

数据证实了这场危机：老年护理价格的上涨速度快于通货膨胀（年均超过4%），哈佛公共卫生学院预计到2032年将有460万个家庭护理职位空缺。长期护理行业面临的劳动力缺口比任何其他医疗保健领域都更为严重。

专家将这种“关键劳动力短缺”归因于低工资、恶劣的工作条件和有限的职业发展机会。尽管家庭健康助理需要更多培训和繁重工作，但他们的时薪（16.82美元）仅比快餐店员工（15.07美元）略高。人手不足导致居民护理质量受损，例如基本需求等待时间过长以及机构中严重缺乏医护专业人员。

拟议的解决方案包括提高工资、允许更多移民填补职位空缺、建立更清晰的职业晋升阶梯和提供负担得起的培训项目。像Care.com这样的公司正在扩大服务范围，以满足日益增长且往往突发的老年护理需求，并将其视为增长最快的业务板块。这场危机不成比例地影响着“夹心一代”，并对经济增长构成巨大阻碍，凸显了一个紧迫且往往不为人知的社会挑战。

---

## 63. 疾控中心将终止所有猴类研究；逐步取消艾滋病和传染病研究

**原文标题**: CDC to end all monkey research; will phase out HIV, infectious disease studies

**原文链接**: [https://www.science.org/content/article/exclusive-cdc-end-all-monkey-research](https://www.science.org/content/article/exclusive-cdc-end-all-monkey-research)

疾病控制与预防中心（CDC）将停止几乎所有涉及非人灵长类动物的研究，这一决定将逐步淘汰其亚特兰大校区数十年来进行的关于艾滋病及其他传染病的长期研究。这一重大的政策转变是在多年内部审查以及包括善待动物组织（PETA）在内的动物福利团体的压力之后做出的。

CDC证实将不再开展新的猴子研究，而现有涉及其不足100只猕猴及其他灵长类动物的项目也将逐步停止。这些动物将被转移到动物收容所，或从研究中“退役”。一位CDC发言人表示，此举反映了该机构“对动物伦理对待的承诺”，并承认替代研究方法（例如体外和计算模型）的进展。

尽管美国国立卫生研究院（NIH）已于2015年结束了大部分黑猩猩研究，但仍在继续进行大量的猴子研究。CDC的这一决定受到了动物权利倡导者的赞扬，但也引起了一些科学家的担忧，担心其可能对理解复杂的传染病和疫苗开发产生影响，而在这些领域，动物模型仍被部分研究界认为至关重要。

---

## 64. 从零构建最小可行Armv7模拟器

**原文标题**: Building a Minimal Viable Armv7 Emulator from Scratch

**原文链接**: [https://xnacly.me/posts/2025/building-a-minimal-viable-armv7-emulator/](https://xnacly.me/posts/2025/building-a-minimal-viable-armv7-emulator/)

本文详细介绍了 "stinkarm" 的创建，这是一个用 1.3k 行 Rust 代码、零依赖、从零开始构建的最小可行 Armv7 用户空间模拟器。作者的动机源于希望深入理解 ELF 格式、Arm 32 位指令编码和执行流程，这将为一种自定义编程语言的 JIT 编译器提供参考。

`stinkarm` 能够解析并验证 32 位 Arm ELF 二进制文件，映射其段，解码一部分 Arm 指令，转换访客和主机内存交互，并将 Arm Linux 系统调用转发到 x86-64 System V 对应的实现。它成功地在 1.9 毫秒内（其中原始模拟仅需 0.015 毫秒）执行了一个基本的 Armv7 "hello world" 二进制文件，与 QEMU 完成相同任务所需的 12.3 毫秒相比，这是一个显著的提升，尽管仍比原生执行慢 100-1000 倍。

文章概述了开发过程，首先从编写一个最小的 Arm 汇编 "exit" 系统调用开始。使用 Rust 构建脚本 (`bld_exmpl`) 和 Nix flake 在 x86 系统上将 Arm 汇编代码交叉编译成一个 Armv7 ELF 二进制文件。核心关注点是 ELF 解析，特别是 `Elf32_Ehdr` (ELF 头) 和 `Elf32_Phdr` (程序头)。`Ehdr` 被严格验证其是否为 Armv7、32 位、小端架构和静态可执行文件类型，这通过使用 Rust 的 `TryFrom` trait 和自定义的小端字节到整数宏 (`le16!`, `le32!`) 来实现。随后，`Phdr` 被用于提取关键的段信息，以便进行内存映射。

---

## 65. 半衰期2的时空穿梭门bug

**原文标题**: A time-travelling door bug in Half Life 2

**原文链接**: [https://mastodon.gamedev.place/@TomF/115589875974658415](https://mastodon.gamedev.place/@TomF/115589875974658415)

文章重点介绍Tom Forsyth在Gamedev Mastodon上发起的一场关于“游戏中门的危险”的讨论。具体来说，该话题围绕着《半条命2》中遇到的一个独特的“时间旅行门bug”。这表明交互式门可能会给游戏开发者带来复杂且有时不寻常的技术挑战。附带的中文文本是一条关于使用Mastodon网络应用程序需要JavaScript的技术说明，不属于游戏开发讨论本身。

---

## 66. 巴西就重大碳信用欺诈案起诉31人。

**原文标题**: Brazil charges 31 people in major carbon credit fraud investigation

**原文链接**: [https://news.mongabay.com/short-article/2025/11/brazil-charges-31-people-in-major-carbon-credit-fraud-investigation/](https://news.mongabay.com/short-article/2025/11/brazil-charges-31-people-in-major-carbon-credit-fraud-investigation/)

巴西联邦警察在该国历史上已知最大规模的碳信用欺诈调查（代号“洗绿行动”）中，起诉了31名涉嫌欺诈和非法侵占土地的人。该骗局以巴西亚马逊地区为基地，涉及Unitor和Fortaleza Ituxi两个REDD+碳信用项目，这两个项目覆盖亚马逊州拉布雷亚市超过14万公顷的土地。

这项调查由Mongabay的一份报告和气候犯罪分析中心（Center for Climate Crime Analysis）的分析促成，证实这些项目在同时生成碳信用的同时，也被用于洗白来自其他被砍伐区域的非法木材。

有三个相互关联的团伙涉案。其中一个由巴西最大的个人碳信用卖家里卡多·斯托佩·儒尼奥尔（Ricardo Stoppe Júnior）领导，他曾向雀巢（Nestlé）、Spotify和波音（Boeing）等公司出售了数百万碳信用额。另两个团伙则由埃尔西奥·阿帕雷西多·莫索（Élcio Aparecido Moço）和若泽·路易斯·卡佩拉索（José Luiz Capelasso）领导，两人都有与非法木材或林产品证书相关的前科。这起欺诈案由巴西土地改革机构（Incra）、登记处和亚马逊州环境保护研究所（Ipaam）的腐败公职人员提供便利。Incra和Ipaam都已表示支持警方调查。

---

## 67. 维珍航空与澳洲航空将在多起火灾后禁用充电宝

**原文标题**: Virgin and Qantas to ban use of portable power banks after string of fires

**原文链接**: [https://www.abc.net.au/news/2025-11-21/airlines-virgin-australia-qantas-ban-power-banks/106033982](https://www.abc.net.au/news/2025-11-21/airlines-virgin-australia-qantas-ban-power-banks/106033982)

澳大利亚航空公司维珍澳大利亚航空、澳洲航空、澳航快运和捷星航空正在实施新的规定，禁止乘客在航班上使用和为移动电源充电。该规定对维珍澳大利亚航空于12月1日生效，对澳航集团则于12月15日生效。这一决定是在发生一系列涉及锂电池火灾的国际和国内事件之后做出的，其中包括7月维珍澳大利亚航空一架航班上发生的空中火灾。

根据新规定，乘客被禁止在机上使用或为移动电源充电，但其他设备的座位充电仍被允许。每位乘客随身行李中最多可携带两个移动电源。维珍澳大利亚航空要求容量介于100-160瓦时（Wh）的移动电源需经航空公司批准，并禁止携带容量超过160瓦时的设备；而澳洲航空和捷星航空则将单个设备的容量上限设为160瓦时。所有移动电源均严禁托运，必须随身携带并易于取用，不得存放在头顶行李舱中（维珍澳大利亚航空尤其如此）。

这些改变使澳大利亚航空公司符合国际安全标准，因为阿联酋航空和国泰航空等全球航空公司已经禁止使用移动电源。自2016年以来，澳大利亚运输安全局（ATSB）已记录了五起移动电源在澳大利亚飞机上起火的事件。澳大利亚空乘人员协会（FAAA）和澳大利亚竞争和消费者委员会（ACCC）（后者报告称2020年至2022年间锂电池事故增加了92%）均强调了这些设备，特别是存在缺陷的设备，所带来的重大风险。

---

## 68. 命令行

**原文标题**: Command Lines

**原文链接**: [https://www.wreflection.com/p/command-lines-ai-coding](https://www.wreflection.com/p/command-lines-ai-coding)

文章《命令行》认为，AI编程助手正在引领软件开发领域的范式转变，类似于编译器将程序员从机器代码中解放出来的方式。这一快速增长的市场，其中Cursor等初创公司实现了创纪录的收入，谷歌、AWS等巨头也纷纷推出新工具，它允许工程师通过自然语言生成代码，从而专注于更高级别的逻辑。

作者将用户分为三类：“手工编程”（工程师避免使用AI）、“随性编程”（非工程师以最少审查来构建概念原型），以及“架构师+AI编程”（工程师使用AI作为结对程序员来处理日常任务，同时保持控制）。这些用户类型导致了两种市场划分：“不插手”工具，面向非工程师构建原型；以及“亲力亲为”工具，面向将AI集成到生产工作流中的专业工程师，后者是更大的市场部分。

这场竞争中的一个关键因素是模型质量，作者认为这是决定性的。尽管有些公司开发内部模型，但对OpenAI和Anthropic等公司前沿模型的依赖仍然普遍存在。微软的GitHub Copilot等现有企业利用捆绑销售和分发来保持市场领先地位，对新进入者构成挑战。最终，AI工具正在将开发者从样板代码中解放出来，为自主软件生成铺平道路。成功将取决于提供卓越的模型质量、交付可靠的代码、提供深度功能以及实现用户粘性。

---

## 69. 我的个人信息值30美元

**原文标题**: My private information is worth $30

**原文链接**: [https://blog.melashri.net/micro/privacy-price/](https://blog.melashri.net/micro/privacy-price/)

作者对明尼苏达大学就2021年数据泄露事件提出的30美元赔偿金深感愤怒和失望。作为校友，他们的个人信息，包括社会安全号码等敏感数据，遭到泄露。该大学以500万美元和解了一项集体诉讼，但未承认任何不当行为，仅向受影响的个人提供30美元以及两年身份盗窃保护服务。

作者认为，这笔赔偿金额“具有侮辱性”，简直是“一记耳光”，尤其考虑到大学频繁要求捐款，却未能兑现之前诸如终身邮件访问权限等承诺。他们批评大学将声誉和财务底线置于问责制、正式道歉以及受影响个人的信任之上。

作者指出，这种行为并非明尼苏达大学独有，而是反映了一个系统性问题：由于监管不力和法律惩罚不足，无论是公共机构还是商业机构，都逃避对数据泄露的真正责任。作者认为，当前的罚款和和解金过低，无法激励机构改进数据安全措施。

作者拒绝了这笔30美元的和解金，并呼吁制定更严格的法规和更严厉的惩罚，以追究机构在数据泄露方面的责任。他们相信，增加经济后果将迫使大学投入更多资金保护个人信息，而非继续将巨额资金分配给行政开支和高管薪资。

---

## 70. 苹果的人体问题

**原文标题**: Apple's Problem with Bodies

**原文链接**: [https://drobinin.com/posts/apples-problem-with-bodies/](https://drobinin.com/posts/apples-problem-with-bodies/)

苹果的App Store在对与个人亲密关系和身体健康相关的应用进行分类时遇到困难，这是一个源于其基础设计的问题。作者通过他们的应用“Silk”（一款私密的、运行于设备上的亲密关系日记）来说明这一点。尽管“Silk”是一款良性的健康工具，却被评定为16+，这个评级通常适用于赌博或“不受限制的网络访问”应用，这突出表明了一个“灰色地带”，目前没有合适的类别。

这个问题源于App Store的早期，其词汇体系来源于iTunes和电影评级，专为视觉“内容”而非用户生成的个人数据而设计。尽管当前的iOS 26评级矩阵对于暴力或医疗风险的界定极其精确，但它通过应用包内的“内容”而非用户的上下文来定义一切。这导致了像“Silk”这类应用的错误分类，它本身没有令人反感的内容，但因暗示“成人主题”的关键词而被标记。

缺乏针对关系健康的特定类别，影响了应用的搜索可见性，并迫使开发者们在“元数据雷区”中摸索，因为“亲密追踪器”之类的词语会触发更严格的审查。即使是不断扩展的Apple HealthKit，也避免对亲密关系进行建模。该系统由过去的事件和责任担忧驱动的“保守主义”，使其在遇到未定义情况时倾向于过度谨慎。

作者的策略是将App Store视为一个黑盒子，通过试验元数据和屏幕截图来推断其规则。尽管睡眠和经期追踪等新类别最终会出现，但这个过程很缓慢。开发者必须在平台当前的“语言”范围内进行开发，在这个灰色地带中运营，直到苹果的分类体系发展到能够满足用户需求。

---

## 71. 我们的宝宝在“偏颇”的亲职测试后被夺走

**原文标题**: Our babies were taken after 'biased' parenting test

**原文链接**: [https://www.bbc.co.uk/news/articles/c1wlw2qj113o](https://www.bbc.co.uk/news/articles/c1wlw2qj113o)

本文详细介绍了格陵兰家庭在丹麦的痛苦经历，他们的孩子在“带有偏见的”父母能力测试（FKU）后被带走。这些测试现在已被禁止用于格陵兰家庭，但仍用于其他家庭，因其文化偏见、用丹麦语进行以及在预测育儿能力方面缺乏科学有效性而受到严厉批评。

凯拉的女儿扎米在出生仅两小时后就被带走，原因是她的测试结果被认定为不适合抚养孩子。她指出测试中存在文化特定问题，并声称一位心理医生告诉她“表现得像个人样”。同样，约翰娜和乌尔里克在约翰娜的测试被贴上“自恋”和“智力迟钝”的标签后，他们的儿子被收养了。她还声称在罗夏测试的一个答案后被称作“野蛮人”。丹麦政府拒绝审查收养案件，理由是孩子们已经安定下来。

格陵兰父母的孩子被带走的可能性是其他父母的5.6倍。尽管政府承诺审查约300个案件，但目前仅评估了10个，并且没有孩子被送回。像凯拉这样的家庭继续为骨肉团聚而奋斗，感受着深深的心痛和文化异化。而皮林瓜最近与女儿的团聚则带来了一线罕见的希望。

---

## 72. Qtile 窗口管理器：基于 Python 的平铺体验

**原文标题**: The Qtile Window Manager: A Python-Powered Tiling Experience

**原文链接**: [https://tech.stonecharioteer.com/posts/2025/qtile-window-manager/](https://tech.stonecharioteer.com/posts/2025/qtile-window-manager/)

本文详细讲述了作者为了寻求更高效的Linux环境，从XFCE转向Qtile（一个由Python驱动的平铺式窗口管理器）的历程。在对i3wm和xmonad的先前尝试感到失望之后，Qtile基于Python的可配置性使其极具吸引力。

作者强调了一种隔离的安装方法，即通过`deadsnakes` PPA利用虚拟环境，并手动设置`.desktop`入口。一个核心理念是对Python配置进行模块化，分离变量声明，以提高可维护性和错误处理能力。

作者精炼后的Qtile配置具备一致的配色方案和自定义资源。值得注意的特性包括一个用于无缝多显示器导航的“智能鼠标移动”功能（Super + .）、逻辑Vim风格的键位绑定，以及强大的硬件感知小部件。这些小部件动态显示电池状态（仅限笔记本电脑）、当前IP地址，以及与`amdgpu_top`集成的实时AMD GPU VRAM使用情况。该配置还动态适应连接显示器的数量，并利用启动钩子来运行初始和周期性脚本。

所汲取的经验教训强调了Python在复杂逻辑和集成方面的巨大能力、从简单开始并迭代的重要性、硬件感知的必要性以及自定义小部件的性能考量。未来的计划包括开发更多自定义小部件（例如《海贼王》章节通知、Kubernetes上下文）和增强的多显示器支持。Qtile显著改变了作者的Linux桌面体验和生产力。

---

## 73. 非常规花瓶模式3D打印

**原文标题**: 3D printing with unconventional vase mode

**原文链接**: [https://vorpal.se/posts/2025/jun/23/3d-printing-with-unconventional-vase-mode/](https://vorpal.se/posts/2025/jun/23/3d-printing-with-unconventional-vase-mode/)

本文详细介绍了“非常规花瓶模式”的先进3D打印技术，旨在帮助经验丰富的用户节省打印时间和材料。花瓶模式通常打印单层螺旋路径，没有接缝，但缺少内部几何结构、填充或顶层。

第一个技巧是在模型内部创建极薄的“狭缝”（例如0.0001毫米）。切片软件将其解释为向内凹陷的外周边，从而形成内部支撑。关键是，PrusaSlicer的“切片间隙闭合半径”必须设置为0.0，以防止这些狭缝合并。

在此基础上，“双壁”可以实现更坚固的区域，或将内部狭缝牢固地锚定到外壁。这些双壁的宽度必须与切片软件根据当前设置计算出的周边宽度精确匹配。此外，增加“挤出宽度”（可达喷嘴直径的2倍）可以进一步加强花瓶模式打印件。

作者还介绍了“伪花瓶模式”，用户手动配置切片软件设置——例如单层周边、无顶层或填充，并禁用“确保垂直外壳厚度”——以模拟花瓶模式的优点，但没有连续的螺旋路径。这提供了更大的灵活性，允许实现可打印的顶面或特定的内部几何结构，正如打印球体案例研究中所示。作者总结道，虽然狭缝可能可见，“伪花瓶模式”结合“围巾接缝”通常能产生更好的美学和功能效果，提供了真实花瓶模式的大部分优点而没有其局限性。

---

## 74. 移民局误拘高等法院实习生，罗德岛法官介入

**原文标题**: RI judge intervenes after ICE mistakenly detains Superior Court intern

**原文链接**: [https://www.wpri.com/news/local-news/providence/ri-judge-intervenes-after-ice-mistakenly-detains-superior-court-intern/](https://www.wpri.com/news/local-news/providence/ri-judge-intervenes-after-ice-mistakenly-detains-superior-court-intern/)

罗德岛州高等法院实习生路易斯·安赫尔·雷耶斯（Luis Angel Reyes，21岁）在前往法院出庭的途中，被美国移民和海关执法局（ICE）错误拘留。此前，预计针对他的一项轻微家庭暴力指控将在庭上被撤销。雷耶斯是“童年入境者暂缓遣返”计划（DACA）的受益人。他因车尾灯损坏被拦下，此时一张源于2017年家庭暴力指控（他从未因此被定罪）的旧ICE逮捕令浮现。他被拘留了大约24小时。

高等法院首席法官爱丽丝·吉布尼（Alice Gibney）迅速介入，直接联系了美国联邦检察官办公室和ICE。她澄清了雷耶斯作为她的实习生身份及其预定的出庭安排。该家庭暴力指控确如预期被撤销。

该事件引发了人们对联邦移民执法政策的担忧，特别是这些政策如何影响DACA受益人以及司法系统的顺畅运作。雷耶斯的法律团队（来自罗杰威廉姆斯大学法学院移民诊所）目前正致力于永久解除ICE的拘留令。吉布尼法官强调了像雷耶斯这样DACA受益人对社区的宝贵贡献，并强调了此类错误拘留的更广泛影响。雷耶斯此后已被释放。

---

## 75. 更多停机与数值限制的故事

**原文标题**: More tales about outages and numeric limits

**原文链接**: [https://rachelbythebay.com/w/2025/11/18/down/](https://rachelbythebay.com/w/2025/11/18/down/)

Rachel by the Bay 所撰写的文章《故障与数字限制的更多故事》探讨了达到数字限制（特别是整数限制）如何引发重大的系统中断。作者讲述了一个系统故障的案例，原因是一个存储时间戳的32位有符号整数达到了其最大值。这导致某个时间点之后的日期“翻转”，被错误地解读为遥远的过去的值，从而使得服务停止处理新数据。

文章强调，系统中断很少是由单一、明显的错误引起的。相反，它们往往是多种复杂因素相互作用的结果，包括：被忽视的数字限制（例如32位与64位整数的区别，或有符号与无符号的解释差异），未能检测到关键状态的不足的监控，一个故障可能引发连锁反应的复杂系统依赖关系，以及开发者对数据范围或时间表示所做的隐式假设。

在开发过程中，测试这些“遥远的未来”或“过大”的边界情况本质上是困难的。文章强调了主动式系统设计的重要性，即预先考虑到此类限制，实施强大的监控以尽早发现异常，并透彻理解不同组件如何相互作用和依赖。最终，这些“数字限制”故障是导致意外停机的一个反复出现、不易察觉但却威力巨大的原因。

---

## 76. AI泡沫比你想象的要大

**原文标题**: The AI bubble is bigger than you think

**原文链接**: [https://prospect.org/2025/11/19/ai-bubble-bigger-than-you-think/](https://prospect.org/2025/11/19/ai-bubble-bigger-than-you-think/)

这篇文章警告称，一场由巨大AI泡沫驱动、迫在眉睫的金融危机正在逼近，这一泡沫是由硅谷和华尔街通过可疑的信贷交易合作助长的。AI基础设施（如GPU和数据中心）所需的巨额投资——预计到本十年末每年需要2万亿美元的营收——主要由“私募信贷”基金提供资金。这些不受监管的非银行贷款机构，从“影子银行”更名而来，目前管理着1.6万亿美元的资产。

科技巨头公司为了避免资产负债表上出现债务，利用“特殊目的载体”（SPV）来建设数据中心。这些SPV将科技巨头锁定为“主要租户”，然后发行债券，通过科技巨头的支付，隐含地向投资者担保还款。例如，私募信贷基金Blue Owl通过这种SPV为Meta的Hyperion数据中心提供资金，Meta在其中持有少数股权。

然而，诸多危险信号正在显现：AI GPU的寿命非常短（由于快速过时和高强度使用，通常不足两年），但却以远长于实际的期限进行折旧，导致收入虚高。这有可能在数据中心和发电厂造成“搁浅资产”。数据中心贷款的证券化，通过将快速贬值的资产打包，进一步加剧了风险。

关键在于，为当前AI投资提供合理依据的巨大预期收入根本没有实现，像OpenAI这样的主要AI参与者却亏损数十亿美元。该行业云服务提供商补贴AI模型训练的自我强化金融模式，被描述为一个典型的泡沫。作者将这种情况比作21世纪初房地产泡沫的金融工程、20世纪20年代不受监管的贷款以及20世纪90年代科技扩张规模的危险组合。虽然私募信贷是核心，但传统银行、私募股权，甚至普通的401(k)投资者都面临着越来越大的风险敞口。专家和关键参与者正在悄然退出，预示着深层的不稳定性。

---

## 77. Git 3.0 默认分支为 "main"，取代 "master"

**原文标题**: Git 3.0 Defaults to "main" Branch Instead of "master

**原文链接**: [https://www.phoronix.com/news/Git-2.52-Released](https://www.phoronix.com/news/Git-2.52-Released)

Git 2.52 已发布，引入了新功能，并为预计于 2026 年底发布的 Git 3.0 做了重要准备。

Git 3.0 的一项关键变化是采用 "main" 作为默认分支名，取代 "master"。Git 2.52 集成了新的提示来协助用户完成这一过渡，也详细说明了如果需要，如何将分支重命名回 "master"。

Git 3.0 的另一个主要发展是从 SHA1 哈希算法过渡到 SHA256。Git 2.52 通过早期的 SHA1-SHA256 互操作性工作启动了这项努力，旨在 Git 3.0 发布时实现平稳过渡。

除了这些前瞻性准备之外，Git 2.52 本身也带来了一系列增强功能。其中包括对各种 Git 子命令的改进，引入了用于显示仓库特性的新子命令 "git repo"，以及用于显示每个路径最接近的祖先提交的子命令 "git last-modified"。此次发布还包括了通用性能改进、错误修复以及其他增量更新。更多详细信息可在官方发布亮点和 GitHub 博客上查阅。

---

## 78. 特朗普政府废除濒危物种保护措施

**原文标题**: Trump administration eliminates protections for endangered species

**原文链接**: [https://www.cbsnews.com/news/trump-administration-endangered-species-act-rollback/](https://www.cbsnews.com/news/trump-administration-endangered-species-act-rollback/)

特朗普政府提议撤销《濒危物种法案》（ESA）下的保护措施，重新启动此前受阻的修改。主要提案包括取消自动保护受威胁物种的“一揽子规则”，转而要求耗时的特定物种规则。此外，官员在划定关键栖息地时将分析经济影响，并且ESA下“伤害”的定义可能会被修改，以潜在地规避对伐木的保护。

这些修改得到了共和党人以及石油、天然气、采矿和农业等行业的支持，他们认为ESA阻碍了经济增长。内政部长道格·伯格姆表示，这些修订旨在恢复ESA的初衷，提供确定性，并尊重美国人民的生计。

然而，环保人士和科学家警告称，这些改变可能导致保护工作多年的延误，加速帝王蝶和佛罗里达海牛等物种的灭绝。他们认为这些提案削弱了保护，并引用了例如亚罗氏棘蜥的案例，其中经济分析可能延迟受气候威胁物种的关键栖息地划定。ESA历史上被认为拯救了99%的列名物种，包括白头海雕，但由于栖息地丧失和气候变化，全球物种灭绝正在加速。特朗普政府过去对北方斑点猫头鹰等物种的撤销保护措施后来被推翻。

---

## 79. 马云家族多年“消失”后将财富转移至英国

**原文标题**: Jack Ma's family shifted wealth to UK after years-long 'disappearance'

**原文链接**: [https://www.source-material.org/jack-ma-bought-uk-home-after-years-long-disappearance/](https://www.source-material.org/jack-ma-bought-uk-home-after-years-long-disappearance/)

马云的妻子张瑛于2024年10月在伦敦贝尔格莱维亚区购入一处价值1950万英镑的豪宅，标志着该家族首次在英国拥有已知房产。此次收购发生之际，马云在经历数年“消失”和审查之后，正逐步回归公众视野，此前他曾在2020年批评中国的金融体系。

分析人士认为，此次购买是对“政权风险”的“预防性多元化投资”，这是中国富裕家庭日益增长的趋势，他们寻求通过将财富转移到“法治社会”来对冲潜在的敌对政策和资产冻结。张瑛已获得新加坡公民身份，还在新加坡投资了房产，并被曝与持有法国资产的离岸公司有关联。这笔伦敦房产的购买，可能由2023年阿里巴巴股票出售所得资助，据报道是为了赶在英国上调海外买家印花税附加费之前匆忙完成的。

马云于2023年在中国重新露面，此前他据报道被罚款近30亿美元，蚂蚁集团的IPO也被叫停。尽管此后他曾与习近平主席会面，但他的公开言论仍未被官方媒体报道，这表明他可能尚未“完全平反”。还有指控称，中国当局曾利用马云向一名异见商人施压。此次财富转移发生在该家族于2015年在香港和纽约进行国际房地产收购之后。

---

## 80. 密码学家丢失解密密钥后取消选举结果

**原文标题**: Cryptographers cancel election results after losing decryption key

**原文链接**: [https://arstechnica.com/security/2025/11/cryptography-group-cancels-election-results-after-official-loses-secret-key/](https://arstechnica.com/security/2025/11/cryptography-group-cancels-election-results-after-official-loses-secret-key/)

国际密码学研究协会（IACR）取消了其年度领导层选举结果，原因是其中一名理事丢失了关键的解密密钥。本次选举是使用Helios进行的，这是一个开源投票系统，旨在通过先进的密码学技术实现可验证、保密和隐私保护。

Helios对每张选票进行加密，为了确保安全并防止串通，解密密钥材料被分发给了三名独立的选举委员会理事，每人持有三分之一。不幸的是，其中一名理事Moti Yung“不可挽回地丢失了他们的私钥”。这种“真诚但不幸的人为失误”导致在技术上无法完成解密过程并验证选举结果。

因此，IACR取消了此次选举。为了防止类似事件再次发生，该组织将采用一种新的密钥管理机制，未来解密时只需三个密钥分块中的两个即可。Moti Yung已辞职，并由Michel Abdalla接替。

IACR作为一个致力于密码学研究的非营利科学组织，正在举行一次新的选举，该选举已于周五开始并将持续到12月20日。

---

## 81. 如何/为何将异步任务归集到Postgres表中处理

**原文标题**: How/why to sweep async tasks under a Postgres table

**原文链接**: [https://taylor.town/pg-task](https://taylor.town/pg-task)

该文章倡导将异步任务的复杂性收敛到一个PostgreSQL表中，推广“精简愚笨”的服务器，这些服务器优先进行快速、简单的数据库查询以提供流畅的用户体验。文章反对将多个外部系统（如 SQS、Redis、Celery）混合用于任务管理，因为这常常导致分布式状态、痛苦的调试以及“手搓”两阶段提交的“罪恶”。

相反，Postgres 凭借其强大的事务保证，被提议作为中心的“单一事实来源”。它能有效地充当队列、管道和异步数据的统一平台，从而消除了一整类错误。这种方法通过直接在数据库中跟踪未完成或未实现的任务，促进了“待办事项驱动开发”（TODO-Driven Development），并通过让计算机管理复杂的重试，增强了“人为容错性”（Human Fault Tolerance）。

具体实现包括一个 `task` 表（其中 `task_type` 和 `params` 字段为 `jsonb` 类型）以及一个工作进程。这个工作进程在一个事务中，持续地使用 `DELETE ... FOR UPDATE SKIP LOCKED LIMIT 1` 语句获取并删除任务。主要特点包括：任务失败时自动重试（得益于事务回滚）、通过 `SKIP LOCKED` 支持并行工作进程、通过随机任务排序（或优先级队列）增强弹性，以及通过延迟来防止过度频繁的轮询。

---

## 82. 微软AI CEO困惑人们对AI不以为然

**原文标题**: Microsoft AI CEO Puzzled by People Being Unimpressed by AI

**原文链接**: [https://80.lv/articles/microsoft-ai-ceo-puzzled-by-people-being-unimpressed-by-ai](https://80.lv/articles/microsoft-ai-ceo-puzzled-by-people-being-unimpressed-by-ai)

微软人工智能首席执行官穆斯塔法·苏莱曼对公众对人工智能的怀疑态度表示不解，称那些对此“不以为然”的人为“愤世嫉俗者”。他的此番言论，是在微软Windows和设备总裁帕万·达乌鲁里声明Windows正演变为一个集成人工智能的“智能代理操作系统”后，遭遇强烈反对而发表的。

苏莱曼认为，人们竟然对人工智能流畅对话或生成图像和视频的能力不以为然，这“令人难以置信”。然而，用户批评微软优先整合人工智能功能（而许多人并不使用这些功能），却忽视了解决Windows长期存在的问题。评论者认为，他们对此不以为然并非针对技术本身，而是微软为了安抚股东，倾向于将人工智能强制整合到产品中，而不是解决用户关心的问题，例如改进用户界面（类似于Windows 7）、修复安全问题以及提升用户隐私。这凸显了科技巨头一致拥抱人工智能与公众更为批判的态度之间的反差。

---

## 83. 测量延迟 (2015)

**原文标题**: Measuring Latency (2015)

**原文链接**: [https://bravenewgeek.com/everything-you-know-about-latency-is-wrong/](https://bravenewgeek.com/everything-you-know-about-latency-is-wrong/)

本文基于 Gil Tene 的研究指出，常见的延迟测量工具和方法存在根本性缺陷，常常错误地反映系统性能。延迟是单个操作所需的时间，这意味着其行为必须通过其**完整分布**来描述，而非仅仅通过平均值或中位数；对于表现出“打嗝”（例如，GC 暂停）的多模式系统而言，这些平均值或中位数是无用的。

许多工具无法充分捕获数据，专注于“常见情况”，例如第95百分位，这可能与大多数用户无关。对百分位数求平均在数学上是不严谨的，而最大延迟，通常被视为噪声，实则是一个关键信号。第99百分位并不罕见；许多用户会频繁遇到它。由于数据汇总，监控系统通常缺乏足够的精度来捕获关键的“N个9”（例如，99.999百分位）。

最普遍的问题是“协调遗漏”。当负载生成器或监控代码无意中忽略或遗漏了糟糕的延迟事件时，就会发生这种情况。例如，当系统变慢时，负载生成器可能会延迟发送请求，或者监控可能只记录一次长时间操作，从而有效地隐藏了排队延迟。这种遗漏会严重扭曲结果，使有问题系统看起来完美，有时甚至使实际的改进看起来像是性能退化。“CTRL+Z”测试可以揭示这一点。协调遗漏衡量的是服务时间，而非真正的响应时间。

为了准确测量延迟，必须了解整个分布，尤其是尾部延迟，并在空闲到饱和之间的各种负载下进行测试。HdrHistogram 等工具可以捕获高分辨率数据并纠正协调遗漏问题。核心信息是对报告的延迟数据持高度批判态度，认识到它们可能具有误导性。

---

## 84. 微软将预加载 Windows 11 文件资源管理器以解决性能不佳问题

**原文标题**: Microsoft Will Preload Windows 11 File Explorer to Fix Bad Performance

**原文链接**: [https://blogs.windows.com/windows-insider/2025/11/21/announcing-windows-11-insider-preview-build-26100-7271-dev-beta-channels/](https://blogs.windows.com/windows-insider/2025/11/21/announcing-windows-11-insider-preview-build-26100-7271-dev-beta-channels/)

Microsoft has released Windows 11 Insider Preview Build 26220.7271 for both Dev and Beta Channels, based on version 25H2. Insiders currently have a temporary window to switch from the Dev to Beta Channel.

This build introduces several new features and improvements. Key additions include the Xbox full screen experience (FSE) for PC, offering console-style navigation for controller-first gaming. A new point-in-time restore feature allows users to quickly roll back their device to a previous state for easier troubleshooting and reduced downtime. Fluid Dictation has been added to Voice Typing for NPU devices, providing smoother dictation with automatic grammar, punctuation, and filler word corrections.

Improvements include enhanced app continuity, allowing users of specific Android phones (Honor, Huawei, Oppo, Samsung, vivo) to seamlessly resume Spotify tracks, browser activity, and M365 Copilot files from their phone to PC. File Explorer receives context menu refinements for better organization. Crucially, Microsoft is exploring **preloading File Explorer in the background to improve launch performance**, with an option to disable this feature available in Folder Options. The Microsoft Store now also allows uninstalling apps directly from the library page. The update also addresses various bug fixes across the OS and lists several known issues.

---

## 85. Google cracked Apple's AirDrop and is adding it to Pixel phones

**原文标题**: Google cracked Apple's AirDrop and is adding it to Pixel phones

**原文链接**: [https://www.theverge.com/news/825228/iphone-airdrop-android-quick-share-pixel-10](https://www.theverge.com/news/825228/iphone-airdrop-android-quick-share-pixel-10)

生成摘要时出错

---

## 86. A looming 'insect apocalypse' could endanger global food supplies

**原文标题**: A looming 'insect apocalypse' could endanger global food supplies

**原文链接**: [https://www.livescience.com/animals/insects/a-looming-insect-apocalypse-could-endanger-global-food-supplies-can-we-stop-it-before-its-too-late](https://www.livescience.com/animals/insects/a-looming-insect-apocalypse-could-endanger-global-food-supplies-can-we-stop-it-before-its-too-late)

生成摘要时出错

---

## 87. Libpng 1.6.51: Four buffer overflow vulnerabilities fixed

**原文标题**: Libpng 1.6.51: Four buffer overflow vulnerabilities fixed

**原文链接**: [https://www.openwall.com/lists/oss-security/2025/11/22/1](https://www.openwall.com/lists/oss-security/2025/11/22/1)

生成摘要时出错

---

## 88. Google tells employees it must double capacity every 6 months to meet AI demand

**原文标题**: Google tells employees it must double capacity every 6 months to meet AI demand

**原文链接**: [https://arstechnica.com/ai/2025/11/google-tells-employees-it-must-double-capacity-every-6-months-to-meet-ai-demand/](https://arstechnica.com/ai/2025/11/google-tells-employees-it-must-double-capacity-every-6-months-to-meet-ai-demand/)

生成摘要时出错

---

## 89. Streaming platform Twitch added to Australia's teen social media ban

**原文标题**: Streaming platform Twitch added to Australia's teen social media ban

**原文链接**: [https://www.bbc.com/news/articles/cx2n2955g10o](https://www.bbc.com/news/articles/cx2n2955g10o)

生成摘要时出错

---

## 90. Microsoft's head of AI doesn't understand why people don't like AI

**原文标题**: Microsoft's head of AI doesn't understand why people don't like AI

**原文链接**: [https://www.pcgamer.com/software/ai/microsofts-head-of-ai-doesnt-understand-why-people-dont-like-ai-and-i-dont-understand-why-he-doesnt-understand-because-its-pretty-obvious/](https://www.pcgamer.com/software/ai/microsofts-head-of-ai-doesnt-understand-why-people-dont-like-ai-and-i-dont-understand-why-he-doesnt-understand-because-its-pretty-obvious/)

生成摘要时出错

---

## 91. Grok's Elon Musk worship is getting weird

**原文标题**: Grok's Elon Musk worship is getting weird

**原文链接**: [https://www.theverge.com/ai-artificial-intelligence/825675/groks-elon-musk-worship-is-getting-weird](https://www.theverge.com/ai-artificial-intelligence/825675/groks-elon-musk-worship-is-getting-weird)

生成摘要时出错

---

## 92. Lawmakers Are Rolling Back Food Safety Rules

**原文标题**: Lawmakers Are Rolling Back Food Safety Rules

**原文链接**: [https://jacobin.com/2025/11/listeria-food-labeling-shutdown-deal](https://jacobin.com/2025/11/listeria-food-labeling-shutdown-deal)

生成摘要时出错

---

## 93. The FBI spied on a Signal group chat of immigration activists, records reveal

**原文标题**: The FBI spied on a Signal group chat of immigration activists, records reveal

**原文链接**: [https://www.theguardian.com/us-news/2025/nov/21/fbi-signal-group-chat-immigration](https://www.theguardian.com/us-news/2025/nov/21/fbi-signal-group-chat-immigration)

生成摘要时出错

---

## 94. Microsoft admits almost all major Windows 11 core features are broken

**原文标题**: Microsoft admits almost all major Windows 11 core features are broken

**原文链接**: [https://www.neowin.net/news/microsoft-finally-admits-almost-all-major-windows-11-core-features-are-broken/](https://www.neowin.net/news/microsoft-finally-admits-almost-all-major-windows-11-core-features-are-broken/)

生成摘要时出错

---

## 95. Trump accuses 6 Democratic lawmakers of seditious behavior, punishable by death

**原文标题**: Trump accuses 6 Democratic lawmakers of seditious behavior, punishable by death

**原文链接**: [https://rhodeislandcurrent.com/2025/11/20/repub/trump-accuses-6-democratic-lawmakers-of-seditious-behavior-punishable-by-death/](https://rhodeislandcurrent.com/2025/11/20/repub/trump-accuses-6-democratic-lawmakers-of-seditious-behavior-punishable-by-death/)

生成摘要时出错

---

## 96. The Algorithm That Detected a $610B Fraud

**原文标题**: The Algorithm That Detected a $610B Fraud

**原文链接**: [https://substack.com/inbox/post/179453867](https://substack.com/inbox/post/179453867)

生成摘要时出错

---

## 97. While Eyes Are on Takaichi, Taiwan's Lai Is Quietly Redefining the Status Quo

**原文标题**: While Eyes Are on Takaichi, Taiwan's Lai Is Quietly Redefining the Status Quo

**原文链接**: [https://jonathancc.substack.com/p/while-eyes-are-on-takaichi-taiwans](https://jonathancc.substack.com/p/while-eyes-are-on-takaichi-taiwans)

生成摘要时出错

---

## 98. So Long, Firefox, Part One

**原文标题**: So Long, Firefox, Part One

**原文链接**: [https://hackaday.com/2025/11/20/so-long-firefox-part-one/](https://hackaday.com/2025/11/20/so-long-firefox-part-one/)

生成摘要时出错

---

## 99. New Apple Study Shows LLMs Can Tell What You're Doing from Audio and Motion Data

**原文标题**: New Apple Study Shows LLMs Can Tell What You're Doing from Audio and Motion Data

**原文链接**: [https://9to5mac.com/2025/11/21/apple-research-llm-study-audio-motion-activity/](https://9to5mac.com/2025/11/21/apple-research-llm-study-audio-motion-activity/)

生成摘要时出错

---

## 100. China Reaches Energy Milestone by "Breeding" Uranium from Thorium

**原文标题**: China Reaches Energy Milestone by "Breeding" Uranium from Thorium

**原文链接**: [https://humanprogress.org/china-reaches-energy-milestone-by-breeding-uranium-from-thorium/](https://humanprogress.org/china-reaches-energy-milestone-by-breeding-uranium-from-thorium/)

生成摘要时出错

---

