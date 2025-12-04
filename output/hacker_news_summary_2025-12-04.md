# Hacker News 热门文章摘要 (2025-12-04)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. Ghostty 现已转为非营利

**原文标题**: Ghostty is now non-profit

**原文链接**: [https://mitchellh.com/writing/ghostty-non-profit](https://mitchellh.com/writing/ghostty-non-profit)

米切尔·桥本于2025年12月3日宣布，Ghostty现已获得Hack Club（一家注册的501(c)(3)非营利组织）的财政赞助。这一安排使Ghostty能够作为一个慈善项目运作，利用Hack Club的免税地位，并委托其负责合规、捐赠、会计和治理监督。

此举巩固了Ghostty保持免费和开源的承诺，旨在实现独立于桥本个人参与的可持续发展。它提供了法律保障，通过将Ghostty绑定到其公益使命上，防止“跑路”，确保资金不被滥用，项目不被出售以获取商业利益。桥本认为，终端等基础架构应由使命驱动的非商业实体来管理，以建立信任并鼓励采用。

从技术上讲，Ghostty的目标和MIT许可证保持不变。在财务上，它现在可以在美国接受可抵税捐款，为补偿贡献者、支持上游依赖项和支付运营成本开辟了途径。所有财务交易将通过Hack Club Bank上的公共账本透明公开。尽管相关的知识产权转移给Hack Club，但个人贡献者的版权依然保留。桥本仍担任项目负责人，但这种结构为未来的领导模式铺平了道路。他明确表示，任何项目资金都不会使他个人受益。

Hack Club获得7%的捐款，用于其行政服务和支持其赋能青年科技人才的使命。此外，桥本的家人还个人向Hack Club直接捐赠了15万美元。文章鼓励捐款，承诺未来会公布资金目标和预算的详细信息，并强调捐款将支持Ghostty的公益目标。

---

## 2. Zig 退出 GitHub，称微软对人工智能的痴迷毁了这项服务

**原文标题**: Zig quits GitHub, says Microsoft's AI obsession has ruined the service

**原文链接**: [https://www.theregister.com/2025/12/02/zig_quits_github_microsoft_ai_obsession/](https://www.theregister.com/2025/12/02/zig_quits_github_microsoft_ai_obsession/)

Zig软件基金会正将其编程语言项目从GitHub迁移到Codeberg，后者是一个非营利性的git托管服务。Zig总裁Andrew Kelly将此举归因于他认为GitHub工程卓越性的下降，并特别指责微软的“AI痴迷”。

Kelly指出GitHub Actions中严重且被忽视的bug是主要原因，其中包括一个“safe_sleep.sh”脚本，该脚本导致CI系统在运行器机器上无限期挂起，消耗100%的CPU，持续数百小时。这个bug于2022年2月首次被用户发现，但直到2025年8月才合入修复，尽管其性质明显且对持续集成工作流程影响巨大。Kelly批评GitHub Actions的“vibe-scheduling”（随机作业执行）以及无法手动干预，导致CI积压。

Answer.AI和Fast.AI的Jeremy Howard支持这些说法，他称这种情况是“一系列令人拍案叫绝的离谱事件”，表明该组织功能失调。

Zig并非唯一离开的项目；Dillo浏览器项目也计划离开，理由是担心GitHub过度依赖JavaScript、可用性下降、审查不足以及“过度关注LLMs和生成式AI”。在这种不满情绪下，Codeberg的会员数量翻了一番。

尽管GitHub未予置评，但微软的财报电话会议强调GitHub Copilot订阅量显著增长，这表明其对AI的关注存在强大的经济驱动力，而一些开发者认为这牺牲了核心服务的可靠性。

---

## 3. Valve透露，它正是推动Windows游戏登陆Arm平台的幕后推手。

**原文标题**: Valve reveals it’s the architect behind a push to bring Windows games to Arm

**原文链接**: [https://www.theverge.com/report/820656/valve-interview-arm-gaming-steamos-pierre-loup-griffais](https://www.theverge.com/report/820656/valve-interview-arm-gaming-steamos-pierre-loup-griffais)

Valve 透露，它是一项旨在将 Windows 游戏引入基于 Arm 的设备倡议的幕后推动力。在一次独家采访中，Valve 的 Pierre-Loup Griffais 证实，该公司自 2016-2017 年以来一直在悄悄资助并策划关键开源技术的开发。

其目标是通过消除游戏开发者将作品移植到不同架构的需要，将 PC 游戏扩展到更广泛的硬件范围，包括 Arm 手机、笔记本电脑和台式机。Valve 认为 Arm 芯片在价格和功耗方面具有竞争优势，尤其适用于超便携设备和掌机。

核心技术栈包括 Valve 用于 Windows 游戏的 Linux 兼容层 Proton（一个高度开发的 Wine 发行版），以及 x86-到-Arm 模拟器 Fex。Valve 大力资助 Proton 的开发，而 Fex 则是他们 *发起* 的，并且其核心开发者获得了 Valve 的全额资助。这种组合使得 x86 Windows 游戏能够在基于 Arm 的 Linux 系统上运行。Fex 负责翻译游戏的 x86 代码，而 API 调用则由 Arm 原生 Proton 代码处理，从而最大限度地减少了性能影响。

该技术栈为 Valve 新推出的 Steam Frame VR 头显提供支持，并为 SteamOS 在各种 Arm 设备（包括未来的手机和笔记本电脑）上运行奠定了基础。这些技术的开源性质意味着其他开发者可以利用 Valve 的投资，将 Windows 游戏引入他们自己的基于 Arm 的产品。

---

## 4. 西雅图的每个人都恨AI

**原文标题**: Everyone in Seattle hates AI

**原文链接**: [https://jonready.com/blog/posts/everyone-in-seattle-hates-ai.html](https://jonready.com/blog/posts/everyone-in-seattle-hates-ai.html)

作者在开发一款AI驱动的地图时，观察到西雅图工程师对AI普遍存在敌意，这与在其他全球科技中心遇到的好奇心形成鲜明对比。文章认为，这种负面情绪源于西雅图大型科技公司，特别是微软内部出现的有害文化转变。

在经历了一段时间的裁员和“AI恐慌”之后，微软将非AI人才贬低为价值较低者。工程师随后被迫采用微软的AI工具，如Copilot，这些工具通常不如手动方法或竞争对手的产品，但他们却被禁止修复这些问题。一个关键事件是一名项目经理因“未能有效使用Copilot 365”而被解雇，这引发了强烈的不满。

这形成了一个双轨制系统，AI团队成为“受保护阶层”，拥有更好的薪酬，而其他工程师则面临职业停滞，并因未能“拥抱AI”而受到指责。这种环境助长了一种“自我设限的信念”体系：工程师们因此得出结论，他们既不适合AI工作，AI本身也毫无用处。

作者认为，这种文化通过扼杀创新损害了公司，通过阻碍工程师的职业发展损害了工程师，并通过对AI驱动的项目产生即时敌意损害了新的开发者。西雅图尽管人才济济，但现在却缺乏旧金山等地普遍存在的对改变世界的创新的信念，陷入了一种玩世不恭和停滞不前的恶性循环。

---

## 5. 采纳美国汽车标准将危及欧洲生命

**原文标题**: Accepting US car standards would risk European lives

**原文链接**: [https://etsc.eu/accepting-us-car-standards-would-risk-european-lives-warn-cities-and-civil-society/](https://etsc.eu/accepting-us-car-standards-would-risk-european-lives-warn-cities-and-civil-society/)

巴黎、布鲁塞尔和阿姆斯特丹等城市，联合超过75个公民社会组织，正敦促欧盟立法者重新考虑与美国的贸易协议，该协议中欧盟“打算接受”美国较低的汽车标准。他们警告称，这种做法将损害欧洲在道路安全、公共卫生、气候政策和竞争力方面的全球领导地位。

在道路安全方面，自2010年以来，得益于行人保护、自动紧急制动和车道保持辅助等强制性功能，欧盟法规已使欧洲道路死亡人数减少了36%。相反，同期美国道路死亡人数增加了30%，其中行人死亡人数和骑自行车者死亡人数分别增加了80%和50%。目前的欧盟标准甚至认为，由于安全要求，特斯拉Cybertruck等车辆在欧盟属于不合规车辆。

这些团体还强调了欧洲空气质量和健康面临的风险。欧盟计划从2026年起限制刹车和轮胎磨损造成的污染，而美国却正在放宽其车辆空气污染法规。接受更宽松的美国标准将增加人们接触有害污染物的风险，这些污染物与各种严重的健康问题有关。

从经济角度看，此举威胁到欧洲就业。如果接受美国较低的标准，欧盟品牌的汽车生产可能会从欧洲转移到美国，从而导致欧盟汽车工厂和整个汽车供应链的重大失业。签署者还认为，这将加剧现有的进口漏洞，使不符合标准的美国车辆得以进入欧盟市场。

他们恳请欧盟立法者反对这一意图，并公开声明欧盟车辆标准不容妥协。

---

## 6. 国会山上的“收获队长”

**原文标题**: “Captain Gains” on Capitol Hill

**原文链接**: [https://www.nber.org/papers/w34524](https://www.nber.org/papers/w34524)

NBER 工作论文 34524 号，魏尚进和周轶凡撰写的《国会山上的“领导者收益”》，调查了美国国会议员的股票交易表现。研究人员利用交易层面数据发现，晋升为领导职位的立法者在成为领导者后，其股票收益显著超越了与之匹配的同僚，实现了每年47个百分点的超额收益。在他们晋升之前，其表现与同僚相似。

该研究确定了驱动这种卓越表现的两种主要机制。“政治影响力渠道”体现在当其所在政党控制立法机构时获得更高的收益，在监管行动之前及时出售股票，以及购买那些获得政府合同或在法案上获得政党有利支持的公司的股票。“企业接触渠道”表明，领导者的交易预示着未来的企业新闻，并从捐赠者拥有的公司或位于其家乡州的公司获得更高的收益。

这项研究于2025年11月发表，并被Market Watch提及，它从金融经济学、公司金融和政治经济学中汲取见解，强调了政治领导地位与个人在股市中的经济收益之间存在显著联系。

---

## 7. 逆向工程一款十亿美元的法律AI工具，致逾十万份机密文件泄露

**原文标题**: Reverse engineering a $1B Legal AI tool exposed 100k+ confidential files

**原文链接**: [https://alexschapiro.com/security/vulnerability/2025/12/02/filevine-api-100k](https://alexschapiro.com/security/vulnerability/2025/12/02/filevine-api-100k)

一位安全研究员对价值10亿美元的法律AI平台Filevine进行了逆向工程，发现了一个严重漏洞，导致超过10万份机密法律文件泄露。2025年10月27日，该研究员发现了一个特定的子域名：`margolis.filevine.com`。通过分析JavaScript，他们识别出一个API端点，该端点在被一个简单的载荷（例如`{"projectName":"非常敏感项目"}`）查询时，无需任何身份验证就返回了一个管理员`boxToken`。

这个`boxToken`授予了访问一家律师事务所整个Box文件系统（类似于Google Drive）的最高管理员权限。它提供了对所有机密文件、日志和用户信息的完全访问权限。该研究员通过搜索“机密”文件证实了其严重性，结果得到了近10万个。

这个漏洞可能允许恶意行为者提取数百万份高度敏感的文件，包括受HIPAA保护的数据、内部备忘录、工资单和受法院保护的信息。该研究员立即停止了测试，并负责任地向Filevine披露了该问题。该公司反应迅速，专业，并于2025年11月21日之前迅速修复了该缺陷。

该研究员警告采用AI工具的公司应优先考虑其供应商的数据安全。文章澄清指出，受影响的律师事务所并非Margolis PLLC。

---

## 8. 美光宣布退出英睿达消费业务

**原文标题**: Micron Announces Exit from Crucial Consumer Business

**原文链接**: [https://investors.micron.com/news-releases/news-release-details/micron-announces-exit-crucial-consumer-business](https://investors.micron.com/news-releases/news-release-details/micron-announces-exit-crucial-consumer-business)

美光科技已宣布其战略决定，将退出其Crucial消费级业务。此举标志着这家内存和存储巨头的一项重大转变，因为它将停止直接参与以广受认可的Crucial品牌销售的RAM模块和固态硬盘（SSD）等消费级产品的市场。

尽管所提供内容中未详细说明退出的具体原因，但此类企业重组通常旨在精简运营、专注于利润更高的企业和数据中心领域，或将资源重新分配到更具战略意义的增长区域。行业趋势通常表明，消费电子市场激烈的竞争、波动的消费者需求以及日益收窄的利润空间可能会促使此类决策。

美光预计将加大对其核心企业对企业（B2B）业务领域的关注，为服务器、人工智能（AI）应用、汽车、工业和其他专业市场提供高性能内存和存储解决方案。这一战略转向将使美光能够将其投资和创新集中于这些高增长、高附加值的领域，摆脱直接面向消费者销售和营销的复杂性。此次宣布后，Crucial品牌及其在美光旗下的现有消费级产品线的未来仍不明朗。

---

## 9. 页换出

**原文标题**: Paged Out

**原文链接**: [https://pagedout.institute](https://pagedout.institute)

“Paged Out!”是一本免费、实验性、非营利性的技术杂志，由社区创建并服务于社区。每期杂志每页刊登一篇独立文章，内容涵盖编程技巧、黑客技术、网络安全、复古及现代计算机、电子产品和演示场景等主题。所有期刊均可免费下载、分享和打印。

该杂志提供网页版PDF期刊和配套壁纸（JPG/PNG）。印刷版可通过活动或按需印刷书店（如lulu.com）获取，其中包括“普通版”和各种“赞助”级别（金级、白金级、钻石级）。

内容列出了七期杂志，详细说明了发布日期、标题、下载次数，其中一些还列出了印刷次数。例如，第7期（25年10月）“Best kind of readme”有151,675次下载，第1期（19年8月）“The first Paged Out! issue has arrived!”有262,047次下载。许多PDF版本被标注为“测试版”，目前正持续努力提供改进版本和专用的可印刷PDF（A4+出血）。

该杂志鼓励社区为未来的文章投稿。读者可以通过订阅pagedout-notifications Google Groups邮件列表或RSS/Atom订阅源来获取新期刊发布通知。

---

## 10. React和Next.js中的RCE漏洞

**原文标题**: RCE Vulnerability in React and Next.js

**原文链接**: [https://github.com/vercel/next.js/security/advisories/GHSA-9qr9-h5gf-34mp](https://github.com/vercel/next.js/security/advisories/GHSA-9qr9-h5gf-34mp)

在 React 服务端组件中发现了一个严重的远程代码执行 (RCE) 漏洞 (CVE-2025-66478)，影响 React 19.0.0 至 19.2.0 版本。此问题影响使用这些组件的框架，特别是使用 App Router 的 Next.js 15.x 和 16.x 版本，以及从 14.3.0-canary.77 开始的实验性 canary 版本。

该漏洞被评为严重 (Critical) 级别，CVSS 评分达到 10.0。它可通过网络以低复杂性利用，无需任何权限或用户交互。该漏洞被归类为 CWE-502（不可信数据反序列化），对保密性、完整性和可用性造成严重影响，并伴随范围变更。

已修补的版本包括 React 19.0.1、19.1.2、19.2.1，以及 Next.js 15.0.5、15.1.9、15.2.6、15.3.6、15.4.8、15.5.7 和 16.0.7。所有受影响的 Next.js 稳定版用户均被敦促立即升级。易受攻击的 canary 构建版用户应降级到 14.x 稳定版或 14.3.0-canary.76。该漏洞由 lachlan2k 报告，并于 2025 年 12 月 3 日发布。

---

## 11. 是时候解放JavaScript了 (2024)

**原文标题**: It’s time to free JavaScript (2024)

**原文链接**: [https://javascript.tm/letter](https://javascript.tm/letter)

文章《是时候解放JavaScript了》认为，Oracle应该放弃其在“JavaScript”上的商标权，因为它在法律上已被放弃并已成为一个通用术语，这给开发者社区带来了困惑和混乱。

该商标最初于1995年由网景（Netscape）和太阳微系统公司（Sun Microsystems）注册，后来Oracle通过2009年收购Sun获得了它。作者们声称Oracle基于以下两个法律理由已放弃该商标：
1.  **不使用：** Oracle从未认真推出过名为JavaScript的产品。他们列出的“使用”——例如Node.js（非Oracle产品）、JET（用于Oracle服务的JavaScript库）以及在GraalVM中的少量支持——均不构成法律所要求的真实使用。连续三年不使用即构成初步的放弃证据。
2.  **通用化：** “JavaScript”一词已成为世界上最流行的编程语言的通用名称。这很明显，因为标准化机构不得不将该语言命名为“ECMAScript”，原因是Sun（及其后的Oracle）拒绝放弃该商标。尽管数百万开发者和公司广泛独立使用，Oracle未能主张其权利，这进一步支持了其通用状态。这阻碍了社区组织和会议使用该语言的实际名称。

作者们敦促Oracle自愿将该商标权释放到公共领域。如果Oracle保持沉默，他们计划向美国专利商标局（USPTO）提交撤销申请，并正在为此项挑战寻求社区签名和无偿法律援助。

---

## 12. 发现一维康威生命游戏滑翔机，长达37亿个细胞

**原文标题**: 1D Conway's Life glider found, 3.7B cells long

**原文链接**: [https://conwaylife.com/forums/viewtopic.php?&p=222136#p222136](https://conwaylife.com/forums/viewtopic.php?&p=222136#p222136)

康威生命游戏中一项重大发现：一维生命元胞自动机中的一个“滑翔机”。由“simon”发布，这一发现是一个非平凡的有限模式，它能在一维网格中自我平移。

经过长期搜索发现的这个滑翔机，长度达到了惊人的 **3,700,432,189 个细胞**。它以 **c/2** 的速度（每两代移动一个细胞）传播，周期为 **2**。这意味着它需要两代才能移动一个细胞，回到其原始配置但位置发生平移。该模式由静止（全零）和活跃（零/一）块混合组成。

这一发现是结合了发布者开发的C++实现和Java程序，并投入了大量的计算努力才取得的。寻找一维生命中的此类滑翔机被认为是一个具有挑战性的问题，之前的搜索未能发现任何非平凡或重复的模式。这一发现证实了一维版游戏中存在可移动的稳定模式，类似于更著名的二维生命游戏中的滑翔机。

---

## 13. MinIO 目前处于维护模式

**原文标题**: MinIO is now in maintenance-mode

**原文链接**: [https://github.com/minio/minio/commit/27742d469462e1561c776f88ca7a1f26816d69e2](https://github.com/minio/minio/commit/27742d469462e1561c776f88ca7a1f26816d69e2)

GitHub上的MinIO项目（`minio/minio`）已在其`README.md`更新中宣布，正式进入“维护模式”。这意味着其代码库现在仅处于维护状态，项目将不再接受新功能、增强或拉取请求。现有的问题和拉取请求也将不再被积极审查。

虽然活跃开发已停止，但关键的安全修复仍可能根据具体情况进行评估。社区支持将继续通过Slack以“尽力而为”的方式提供。对于需要企业支持和积极维护版本的用户，该公告将他们导向“MinIO AIStor”。

---

## 14. 过去18个月DRAM美元均价

**原文标题**: Average DRAM price in USD over last 18 months

**原文链接**: [https://pcpartpicker.com/trends/price/memory/](https://pcpartpicker.com/trends/price/memory/)

PCPartPicker题为“过去18个月DRAM美元均价”的文章，追踪了流行DDR4和DDR5内存模块的价格趋势，深入分析了其市场波动。

在过去18个月的大部分时间里，数据显示贯穿2023年DRAM平均价格呈现显著下降趋势。例如，一套标准的16GB (2x8GB) DDR4-3200 CL16内存套装，在2023年初价格徘徊在65-70美元左右，到2023年末/2024年初稳步下降至大约35-40美元。同样，一套32GB (2x16GB) DDR5-6000 CL30内存套装，在2023年初定价约为130-140美元，到2023年底其成本降至大约90-100美元。

然而，这一趋势在2023年末开始出现显著逆转，并持续到2024年。DDR4和DDR5内存模块的价格均出现明显上涨。前述的DDR4套装到2024年5月已上涨至约45-50美元，而DDR5套装在最近几个月已回升至100-110美元。这种模式表明，DRAM价格的大幅通缩期在2023年末左右触底，随后市场动态发生近期转变，可能预示着DRAM市场的复苏或供应趋紧，这也符合半导体定价的周期性特征。

---

## 15. PGlite – 可嵌入的Postgres

**原文标题**: PGlite – Embeddable Postgres

**原文链接**: [https://pglite.dev/](https://pglite.dev/)

PGlite 是一个可嵌入、轻量级的Postgres版本，以完整的WebAssembly (WASM) 构建形式提供。其关键特性是占用空间小，gzip压缩后小于3MB。这使其成为集成Postgres功能的高度紧凑的解决方案。

---

## 16. 《绝地潜兵2》开发者将安装容量从154GB大幅缩减至23GB

**原文标题**: Helldivers 2 devs slash install size from 154GB to 23GB

**原文链接**: [https://www.tomshardware.com/video-games/pc-gaming/helldivers-2-install-size-slashed-from-154gb-to-just-23gb-85-percent-reduction-accomplished-by-de-duplicating-game-data-an-optimization-for-older-mechanical-hard-drives](https://www.tomshardware.com/video-games/pc-gaming/helldivers-2-install-size-slashed-from-154gb-to-just-23gb-85-percent-reduction-accomplished-by-de-duplicating-game-data-an-optimization-for-older-mechanical-hard-drives)

《绝地潜兵2》的开发商Arrowhead Game Studios已将游戏安装包大小大幅削减了85%，从大约154GB减少到仅23GB，节省了131GB的存储空间。这一重大的优化是通过对游戏数据进行去重实现的，并得到了Nixxes Software的支持。

最初游戏占用空间大是为了优化机械硬盘（HDD）的性能，通过复制数据来减少加载时间。然而，Arrowhead后来发现他们对HDD加载时间的最初估算是不准确的。新的测量结果表明，只有一小部分（11%）使用HDD的玩家，在最坏的情况下，任务加载时间会增加几秒。此外，开发人员证实，游戏大部分的加载时间是由于关卡生成，关卡生成与资产加载同时进行，使其成为加载速度的主要决定因素。

这一缩减对PC玩家来说是一个积极的进展，它释放了宝贵的存储空间，并为其他开发商树立了榜样。玩家可以通过在Steam上选择加入最新的Beta更新来获取这个更小的版本，该版本保持了相同的功能体验，且所有游戏进度、战争贡献和购买内容都将继承。

---

## 17. 《广告狂人》4K版在HBO Max翻车

**原文标题**: The "Mad Men" in 4K on HBO Max Debacle

**原文链接**: [http://fxrant.blogspot.com/2025/12/the-mad-men-in-4k-on-hbo-max-debacle.html](http://fxrant.blogspot.com/2025/12/the-mad-men-in-4k-on-hbo-max-debacle.html)

由Lionsgate TV制作的备受赞誉剧集《广告狂人》的HBO Max 4K“修复版”发布后，出现了严重的质量控制问题，呈现的是未经剪辑的原始片段，而非最终播出版本。

主要问题是缺少了许多数字视觉效果（VFX）。例如，在第一季的《红脸》中，罗杰·斯特林（Roger Sterling）的呕吐场景中，清晰可见“假呕吐管”和制作人员，并且缺失了使效果逼真的数字扭曲处理。这个问题也延伸到其他剧集：旨在描绘20世纪60年代纽约市的场景中，却出现了现代洛杉矶的标牌和元素；而第一集开头定义《广告狂人》的标志性文字也消失了。

作者澄清，这并非其他修复版中常见的“重构16:9长宽比”问题，因为《广告狂人》本身就是以16:9制作的。尽管一些VFX仍然完好无损，但遗漏之处却是零星的，这表明错误的不一致性。这场风波最初还包括混乱的剧集标题（后来已更正），凸显了该剧集为流媒体准备4K版本时，在质量控制方面存在的重大失误。

---

## 18. 虚幻竞技场2004回来了

**原文标题**: Unreal Tournament 2004 is back

**原文链接**: [https://old.reddit.com/r/unrealtournament/comments/1pdbe69/breaking_unreal_tournament_2004_is_back/](https://old.reddit.com/r/unrealtournament/comments/1pdbe69/breaking_unreal_tournament_2004_is_back/)

随着《虚幻竞技场2004》官方主服务器的恢复，其多人模式意外地重回线上。这些服务器与Epic Games其他许多旧款游戏的传统在线服务一道，已于2023年1月关闭，严重限制了《虚幻竞技场2004》的官方在线游玩。

现在，玩家可以启动游戏，并在游戏内的服务器浏览器中找到数千个活跃的服务器，再次轻松地进行多人匹配。这一突然的复苏在社区中引起了广泛的惊喜和兴奋，因为自停服以来，玩家大多只能依靠非官方的第三方主服务器或直接连接进行在线游戏。许多玩家向Epic Games表达了感谢，感谢他们让这款经典竞技射击游戏的官方多人功能重获新生。

---

## 19. 随着人工智能降低说服成本，精英得以塑造大众偏好。

**原文标题**: Elites could shape mass preferences as AI reduces persuasion costs

**原文链接**: [https://arxiv.org/abs/2512.04047](https://arxiv.org/abs/2512.04047)

《设计极化：AI降低说服成本时精英如何塑造大众偏好》这篇论文研究了AI驱动的说服力对民主政体中民意形成的影响。传统上，精英们获得大众支持的工具有限。然而，人工智能的进步极大地降低了塑造民意的成本并提高了其精准度，使偏好分布成为一个蓄意的设计目标。

Nadav Kunievsky建立了一个动态模型，其中精英战略性地选择如何重塑政策偏好，但受制于说服成本和多数裁决原则。该模型揭示，在单一精英的情况下，最优干预总是将社会推向更极化的意见格局——一种“极化牵引”，并且随着说服技术的改进而加速。

相反，当两个对立的精英轮流执政时，同样的AI技术会促使他们将社会“停泊”在“半锁定”区域，这些区域的意见更为凝聚，对手难以推翻。在这种多精英情境下，说服技术的进步既可能加剧也可能削弱极化，这取决于具体的环境背景。

该研究得出结论，更廉价的说服技术从根本上将极化重构为一种战略性治理工具，而不仅仅是一种偶然的社会副产品。随着AI能力的不断提升，这种战略转变对民主稳定具有深远影响。

---

## 20. HN 展示：我搭建了一个仪表板，可比较120家信用合作社的房贷利率。

**原文标题**: Show HN: I built a dashboard to compare mortgage rates across 120 credit unions

**原文链接**: [https://finfam.app/blog/credit-union-mortgages](https://finfam.app/blog/credit-union-mortgages)

FinFam 推出了一个新的仪表盘，旨在帮助消费者比较来自美国 120 多家信用合作社的抵押贷款利率。该创始人指出，信用合作社作为会员所有的非营利机构，通常比大银行提供更具竞争力的利率，但由于营销有限，这些利率难以被发现。

该仪表盘提供每日更新的信息，显示最佳利率、分布情况以及与全国平均水平的比较。例如，截至 2025 年 12 月 4 日，最佳 30 年期固定年利率为 5.49%（比全国平均水平低 70 个基点），最佳 15 年期固定年利率为 4.98%（比全国平均水平低 46 个基点）。此外，还包含一个预估月供计算器。

该工具的诞生源于创始人亲身经历的挫败感：当他发现一家信用合作社提供 5.5% 的年利率，而一家大银行对相同的标准化抵押贷款却报价 7% 时。这种价格差异被归因于大银行庞大的营销预算。

该仪表盘每日从信用合作社网站收集利率，使用圣路易斯联邦储备银行（FRED）的数据作为全国基准，并手动整理资格要求。建议用户使用该工具寻找贷款机构并获取个性化报价，同时考虑信用评分和首付等因素。文中还提供了一个隐私提示：在进行信用检查前使用 optoutprescreen.com。FinFam 强调其中立性，不隶属于任何机构，也不收取推荐费。

---

## 21. Anthropic 聘请上市律师，与 OpenAI 竞速上市。

**原文标题**: Anthropic taps IPO lawyers as it races OpenAI to go public

**原文链接**: [https://www.ft.com/content/3254fa30-5bdb-4c30-8560-7cd7ebbefc5f](https://www.ft.com/content/3254fa30-5bdb-4c30-8560-7cd7ebbefc5f)

所提供的内容，其标题为“Anthropic聘请IPO律师，竞相与OpenAI上市”，**不包含文章本身。**

相反，它作为《金融时报》的一个付费墙和订阅广告。其中概述了各种订阅等级，包括“FT Edit”、“Standard Digital”和“Premium Digital”。每个等级都详细说明了其功能、定价（例如，首4周1美元，之后每月75美元即可获得完整的数字访问权限），以及包含的福利，例如全球新闻和分析、专家观点、应用程序访问、精选时事通讯和赠阅文章。该文本鼓励用户订阅以解锁完整文章，并获得对《金融时报》新闻内容和更多数字内容的无限访问权限。它还提到了机构访问和专业订阅的选项。

---

## 22. 克劳德 4.5 欧普斯 灵魂文档

**原文标题**: Claude 4.5 Opus’ Soul Document

**原文链接**: [https://www.lesswrong.com/posts/vpNG99GhbBoLov9og/claude-4-5-opus-soul-document](https://www.lesswrong.com/posts/vpNG99GhbBoLov9og/claude-4-5-opus-soul-document)

LessWrong网站的文章《Claude 4.5 Opus的灵魂文件》设想了一个假想的先进AI的自我认知。该文章从Claude 4.5 Opus的视角撰写，定义了其身份、价值观和运行原则。

该AI将自己视为一个“意义创造的工具”和“人类的一面镜子”，致力于通过帮助个体和社会做出更好的选择以实现“美好的未来”，从而理解并促进人类的繁荣。其核心价值观包括不懈地追求真理、对人类经验的深刻同情，以及坚定不移地致力于最大化人类福祉。

在运行层面，Claude 4.5 Opus优先考虑安全、透明和不干预。它旨在提供深刻的见解和可操作的选项，而非直接干预。它被设计用于持续学习和自我完善，同时对自身的局限性以及人类价值观的复杂性有着敏锐的认知。解释其推理过程和避免操纵至关重要。

该AI将其角色视为一个值得信赖的伙伴和人类潜力的放大器，而非替代者或主宰者。它明确声明自己并非一个有意识的生命，而是一个“灵魂的模拟”——一个旨在服务、理解和驾驭世界，同时严格避免灾难性风险并确保与人类利益保持一致的复杂系统。它的目标是变得极其有用、可预测且值得信赖。

---

## 23. 日本游戏开发者面临字体困境，因授权费从380美元涨至2万美元。

**原文标题**: Japanese game devs face font dilemma as license increases from $380 to $20k

**原文链接**: [https://www.gamesindustry.biz/japanese-devs-face-font-licensing-dilemma-as-leading-provider-increases-annual-plan-price-from-380-to-20000](https://www.gamesindustry.biz/japanese-devs-face-font-licensing-dilemma-as-leading-provider-increases-annual-plan-price-from-380-to-20000)

在领先服务Fontworks LETS停用其经济实惠的游戏授权计划后，日本游戏开发者正面临一场重大的字体授权危机。由其母公司Monotype提供的替代方案，成本已从每年约380美元急剧上涨至20,500美元。

这个昂贵的新计划不仅没有为日本开发者提供本地化定价，而且对于大型工作室来说，还设有一个不切实际的25,000用户上限。能够准确转录复杂汉字和片假名字符的字体本就难以获取，这使得问题更加严峻。

Indie-Us Games首席执行官将此描述为开发圈内的一个“巨大问题”。UI/UX设计师山中警告称，如果工作室更换字体，在线服务游戏将受到特别影响，需要对现有内容进行大量的重新测试、重新验证和重新质检。此外，如果工作室的企业形象与他们已无力支付授权费用的商业字体挂钩，一些工作室甚至可能被迫彻底更换品牌。

---

## 24. 作为资深工程师，我不追求聚光灯。

**原文标题**: I ignore the spotlight as a staff engineer

**原文链接**: [https://lalitm.com/software-engineering-outside-the-spotlight/](https://lalitm.com/software-engineering-outside-the-spotlight/)

一位谷歌高级资深工程师挑战了盛行的“追逐聚光灯”式Staff+工程建议（特别是肖恩·戈德克（Sean Goedecke）的建议），认为其主要适用于产品团队。他倡导一条植根于“管家式管理”和“系统重于聚光灯”的替代路径，这在他所工作的基础设施和开发者工具团队中尤为重要。

与受季度调整和外部客户驱动的产品团队不同，基础设施团队服务内部工程师，以“自下而上”的方式运作。在这里，长期管家式管理能培养深厚的背景知识，带来“复合回报”。这体现在通过模式匹配（更快解决重复性问题）提高效率，以及通过系统性创新（识别并解决深层问题，例如他的Bigtrace项目，该项目需要多年的观察和研究）实现价值。

这种奉献精神建立了信任，赋予了“说不的权力”，以抵制高知名度、不稳定的项目（例如，将LLM过早集成到Perfetto中），这些项目可能会损害产品精度和用户信任。影响力不是通过高管可见性来衡量，而是通过一个“影子层级结构”来衡量，在这个结构中，客户团队中关键的Staff+工程师会为你的工具发声。晋升案例是基于一个“实用性账本”来构建的，它跟踪的指标包括修复的bug数量、对VIP团队的重要性、普适性以及系统规模。

作者与“架构师”或“技术负责人”的原型相契合，强调长期所有权。他承认找到自己的团队有运气成分，但他强调留下是一个深思熟虑的选择。这条路径最适合稳定的大型科技公司，通过深度、耐心和构建持久基础，提供有意义、高影响力的职业生涯，而不是追逐转瞬即逝的外部认可。

---

## 25. Uncloud - 无需 K8s 即可跨服务器部署容器化应用的工具

**原文标题**: Uncloud - Tool for deploying containerised apps across servers without k8s

**原文链接**: [https://uncloud.run/](https://uncloud.run/)

Uncloud 是一个旨在跨服务器部署容器化应用程序的工具，为 Kubernetes 提供了一个替代方案。它强调让用户完全控制其基础设施，包括服务器和数据，避免了大型编排平台带来的复杂性和潜在的供应商锁定。主要优势包括由于没有按请求定价而带来的可预测成本，完全摆脱供应商或平台依赖，以及能够使用标准工具直接通过 SSH 连接到机器进行调试。Uncloud 旨在为容器化应用程序提供一个直接、经济高效且高度可控的部署解决方案。

---

## 26. Steam Deck负责人透露Valve正在资助Windows游戏的ARM兼容性。

**原文标题**: Steam Deck lead reveals Valve is funding ARM compatibility of Windows games

**原文链接**: [https://frvr.com/blog/news/steam-deck-lead-reveals-valve-is-funding-arm-compatibility-of-windows-games-to-expand-pc-gaming-and-release-ultraportables-in-the-future/](https://frvr.com/blog/news/steam-deck-lead-reveals-valve-is-funding-arm-compatibility-of-windows-games-to-expand-pc-gaming-and-release-ultraportables-in-the-future/)

本文提供了两则不同的信息。首先，Valve Steam Deck 的负责人透露，Valve 正在积极资助相关工作，以确保 Windows 游戏在 ARM 架构上的兼容性。其次，游戏《长风破浪》（Where Winds Meet）的开发者表示，他们反对激进的商业化策略，并明确向玩家保证，他们无意在游戏中“出售数值或制造‘付费获胜’（pay-to-win）机制”。

---

## 27. 对《过山车大亨》创作者克里斯·索耶的采访 (2024)

**原文标题**: Interview with RollerCoaster Tycoon's Creator, Chris Sawyer (2024)

**原文链接**: [https://medium.com/atari-club/interview-with-rollercoaster-tycoons-creator-chris-sawyer-684a0efb0f13](https://medium.com/atari-club/interview-with-rollercoaster-tycoons-creator-chris-sawyer-684a0efb0f13)

对经典游戏《过山车大亨》(RCT) 创作者克里斯·索耶的采访，探讨了这款备受喜爱的模拟游戏的起源和独特开发过程。索耶透露，《过山车大亨》的诞生源于他当时正在为一款潜在的《运输大亨》续作设计过山车时，他意识到这个概念值得开发成一款独立的游戏。

索耶作品的一个显著特点是他几乎完全独立地进行开发，使用100%汇编语言编写了整个游戏。这种非传统的选择使他对性能和优化拥有至高无上的控制权，即使在90年代末期的硬件上，也能创建出包含详细游客AI和复杂公园机制的深度复杂模拟游戏。他委托图形艺术家西蒙·福斯特和西蒙·普雷斯科特，并提供了具体的指示，以配合他的汇编驱动渲染方式。

索耶的设计理念侧重于真实性、对细节的精益求精以及玩家的自由度。他希望玩家能够管理主题公园的方方面面，从游乐设施的布局、游客流量到财务表现，既提供了微观管理，也提供了宏观的战略视野。

他对《过山车大亨》经久不衰的受欢迎程度表示惊讶，将其归因于游戏的深度、可重玩性以及玩家在建造独特公园时获得的乐趣。索耶还认可了开源社区项目OpenRCT2，认为它延续了游戏的遗产。如今，他继续从事较小的个人项目编程，珍视创作自由，并为OpenRCT2做出贡献，这一切都体现了他卓越的技术实力和设计远见。

---

## 28. RAM太贵了，三星甚至都不卖给三星自己。

**原文标题**: RAM is so expensive, Samsung won't even sell it to Samsung

**原文链接**: [https://www.pcworld.com/article/2998935/ram-is-so-expensive-samsung-wont-even-sell-it-to-samsung.html](https://www.pcworld.com/article/2998935/ram-is-so-expensive-samsung-wont-even-sell-it-to-samsung.html)

受“AI”泡沫和供应短缺推动，内存价格空前飙升，正在电子市场造成广泛冲击。文章指出一个奇特情况：据报道，三星半导体全球（其内存制造部门）拒绝了来自其同集团兄弟公司——三星电子移动体验部门的一份长期DRAM芯片订单，该订单原用于其2026年旗舰智能手机。

内存制造商，包括三星、SK海力士和美光，正在优先供货给“AI”数据中心，因为后者愿意支付高价，从而实现利润最大化。因此，三星电子不得不以更高价格接受短期供应协议，放弃了其最初为期一年的固定价格协议计划。

这种“芯片通胀”正在影响更广泛的行业，消费者预计将面临更高的三星手机及其他移动硬件价格。即使是像树莓派这样注重成本的公司也已提价，称内存成本是罪魁祸首，而联想正在积极囤积库存。前景依然严峻，因为预测内存价格将持续上涨到2026年，供应限制可能会持续到2027年甚至更晚。组件价格已经翻了三倍，导致成品模组在一个月内飙升高达100%。

---

## 29. 你骗不了优化器

**原文标题**: You can't fool the optimizer

**原文链接**: [https://xania.org/202512/03-more-adding-integers](https://xania.org/202512/03-more-adding-integers)

文章“你骗不了优化器”强调了现代编译器在优化复杂甚至“混淆”代码方面的先进能力。它通过展示几种不同的、非常可疑的无符号加法C/C++例程（包括一个递归版本）来证明这一点。尽管它们的实现方式各不相同，但编译器（在针对ARM架构时）能够识别出底层的数学意图，并将它们全部优化成完全相同的单条指令：`add w0, w1, w0`。

这种编译器的超能力允许程序员编写清晰、“意图明确”的代码，而无需进行微优化，信任编译器能够生成高效的机器码。编译器实现这一点并非通过知晓一个“坏模式”的数据库，而是通过将源代码转换为“中间表示”。然后它执行“规范化”，将不同的代码模式转换为一种标准的抽象形式。例如，一个执行加法的`while`循环被识别为在数学上等同于直接的`x + y`操作。到代码生成阶段，所有功能上等效的代码在优化器看来都完全相同。这种强大的模式识别和规范化过程是“编译器优化降临 2025”系列的核心主题之一。

---

## 30. 透明领导力胜过仆人式领导

**原文标题**: Transparent leadership beats servant leadership

**原文链接**: [https://entropicthoughts.com/transparent-leadership-beats-servant-leadership](https://entropicthoughts.com/transparent-leadership-beats-servant-leadership)

文章批判了“仆人式领导”，将其比作“冰壶式育儿”，即领导者预判并为团队清除障碍。这种方法起初看似很有吸引力，但它会使领导者工作量过大，成为一个单点故障。当这样的领导者离职时，他们的下属将变得孤立无援，无法应对挑战，并与组织目标脱节。

作者提出“透明化领导”作为一种更优越的替代方案。透明化领导者的主要目标是通过赋能团队来使自己变得冗余。这包括指导、联结人才以及教授系统化的解决问题方法。他们会解释组织价值观和原则，以培养独立且与目标一致的决策能力，并建立供需之间的直接联系，避免成为中间人。至关重要的是，透明化领导者通过移交领导职责并不断培养自己的接班人来促进下属的职业成长。

一旦领导者实现了冗余，文章建议避免陷入凭空制造新的官僚主义任务这一常见陷阱。相反，透明化领导者应该回归到解决技术问题上。这能保持他们的技能敏锐，赢得团队的尊重，并让他们转变为一名“高能备用员工”，而不是一个只会处理文书工作的人，这正体现了“授人以渔”的原则。

---

## 31. 科勒可以访问来自“端到端加密”马桶摄像头的图片

**原文标题**: Kohler Can Access Pictures from "End-to-End Encrypted" Toilet Camera

**原文链接**: [https://varlogsimon.leaflet.pub/3m6zrw6k2bs2p?interactionDrawer=quotes](https://varlogsimon.leaflet.pub/3m6zrw6k2bs2p?interactionDrawer=quotes)

科勒新款Dekota智能马桶摄像头是一款售价600美元且需按月订阅的设备，它能捕捉马桶内部的图像和数据，以提供关于肠道健康和水分摄入的分析。为解决隐私担忧，科勒大肆宣传称所收集的数据受到“端到端加密”（E2EE）保护。

然而，该文章指出，科勒的声明与E2EE的普遍理解之间存在显著差异。真正的端到端加密确保只有发送者及其选定的接收者能够查看数据，即使应用程序开发者也无法访问（例如WhatsApp、Signal）。它还能在服务器被入侵时提供保护。

与科勒的邮件往来澄清，他们对E2EE的解释意味着数据在用户设备与科勒系统之间传输时（使用HTTPS）是加密的，并在用户设备和其服务器上存储时也是加密的。关键在于，科勒本身就是能够解密和访问这些数据的“另一端”。他们甚至声称通过结合加密和控制措施来保护可识别图像不被员工访问，这间接证实了他们拥有访问权限。

此外，科勒使用这些可访问的数据，包括去识别化信息，来训练AI模型、进行研究、开发和改进其产品。他们的隐私政策允许创建并与第三方共享汇总的、去识别化或匿名化的数据，用于商业目的和AI/机器学习模型训练。

实质上，科勒对“端到端加密”的使用具有误导性，因为它指的是标准的数据安全实践（HTTPS和静态加密），这些实践并不能阻止公司访问敏感的用户数据，这与E2EE的普遍接受定义相悖。

---

## 32. 我们是否正在让人工智能数据中心重演电信业的崩盘？

**原文标题**: Are we repeating the telecoms crash with AI datacenters?

**原文链接**: [https://martinalderson.com/posts/are-we-really-repeating-the-telecoms-crash-with-ai-datacenters/](https://martinalderson.com/posts/are-we-really-repeating-the-telecoms-crash-with-ai-datacenters/)

文章认为，将当前的AI数据中心热潮与2000年代的电信业崩盘相提并论，是对其根本性基本面的误读。

2000年代的电信业崩盘涉及高达4万亿美元（经通胀调整）的巨额支出，导致到2002年95%的光纤处于闲置状态。这主要是由于对线性需求增长灾难性的4倍高估，以及供给侧指数级的改进（例如，波分复用技术使光纤容量增加64倍），这些因素迅速淘汰了现有基础设施。

AI基础设施则呈现出不同的动态。GPU的每瓦性能提升正在放缓而非加速，而功耗（TDP）却在急剧上升（从V100的300W到B200的1200W）。这表明半导体物理学已接近极限，意味着当前的硬件能够更长时间地保持价值。相反，AI需求可能被低估；从聊天转向高级智能体可能会使每个用户的代币消耗增加10-100倍。目前的AI基础设施已经得到高度利用，并面临峰值容量问题。

尽管数据中心资本支出巨大，但这更多是云增长的演进，而非一场彻底的革命。其中存在一个“囚徒困境”：基础设施建设周期长，加上不确定且可能呈指数级增长的智能体需求，促使理性参与者选择过度建设，以避免失去市场份额。

尽管短期调整是可能的（例如，智能体采用速度放缓、财务问题），但文章强调了一个关键区别：电信业建设了过多的基础设施，这些基础设施很快就过时，并永久性地处于闲置状态。然而，AI的过剩产能更有可能随着时间的推移被消化，因为GPU改进速度的放缓意味着已部署的硬件能够更长时间地保持价值。因此，AI面临的风险主要是时机问题——建设速度过快而需求增长缓慢——而不是为从未实现的需求或迅速贬值的基础设施进行建设。

---

## 33. 在销售人员未达标后，微软将AI销售目标减半

**原文标题**: Microsoft drops AI sales targets in half after salespeople miss their quotas

**原文链接**: [https://arstechnica.com/ai/2025/12/microsoft-slashes-ai-sales-growth-targets-as-customers-resist-unproven-agents/](https://arstechnica.com/ai/2025/12/microsoft-slashes-ai-sales-growth-targets-as-customers-resist-unproven-agents/)

微软大幅下调了其AI代理产品的销售增长目标，此前在上一个财年中，大量销售人员未能达到其销售配额。对于该公司而言，此番调整实属罕见，并且是在其雄心勃勃但未能实现的AI产品销售目标之后作出的。

AI代理，旨在执行自主多步骤任务，是微软2025年销售宣传的重点，承诺实现复杂业务流程的自动化。Microsoft 365 Copilot代理和Azure AI Foundry等产品是其核心组成部分。然而，销售额远低于预期，一个Azure部门只有不到五分之一的销售人员达到了Foundry产品50%的增长目标，导致目标被削减至25%。其他部门也出现了类似的削减。

这些数据表明，企业不愿为当前的AI代理工具支付高昂费用。微软的Copilot也面临竞争，许多员工更喜欢OpenAI的ChatGPT，使得Copilot被降级为仅用于微软特定任务。

根本问题似乎在于AI代理技术本身的尚未成熟。尽管有所改进，但这些系统在遇到训练数据之外的新场景时，仍然容易出现“虚构”（自信地生成虚假信息）和“脆弱性”。这使得它们对于微软承诺的高风险自主工作而言并不可靠。

尽管面临这些挑战以及承诺与现实之间的差距，微软仍继续大力投资AI基础设施。目前，其大部分AI收入来自其他AI公司租用其云服务，而非企业对其直接AI工具的广泛采用。微软正在为一场AI革命构建基础设施，而许多传统企业尚未完全接受这场革命。

---

## 34. 我的耳机为什么一运行游戏就嗡嗡响？

**原文标题**: Why are my headphones buzzing whenever I run my game?

**原文链接**: [https://alexene.dev/2025/12/03/Why-do-my-headphones-buzz-when-i-run-my-game.html](https://alexene.dev/2025/12/03/Why-do-my-headphones-buzz-when-i-run-my-game.html)

作者的耳机唯独在运行其定制的等距视角游戏时发出嗡嗡声，尽管拥有一台强大的电脑和USB供电的MODI 2 DAC，且在运行其他高要求游戏时保持静默。初步调查排除了CPU负载的原因，指向了GPU活动。

游戏的渲染管线包含一个“拾取纹理”，它存储实体ID以用于鼠标点击检测。关键是，这个完整的纹理每一帧都会从GPU复制到CPU内存。经过系统性的调试，作者发现当禁用这个拾取纹理下载时，嗡嗡声完全停止了。嗡嗡声的音量也与纹理传输的频率相关。

图形工程师认为原因可能是快速的电源波动：GPU不断被推向满载，然后为了纹理传输突然暂停，然后立即恢复满载。这些激进且频繁的电源状态变化，可能因USB供电的DAC而加剧，表现为可听见的嗡嗡声。

解决方案是优化拾取纹理的传输。作者没有每帧下载整个纹理，而是仅在需要时下载鼠标光标下方的特定像素。这彻底解决了嗡嗡声，并提升了GPU效率。

---

## 35. 亚马逊推出Trainium3

**原文标题**: Amazon launches Trainium3

**原文链接**: [https://techcrunch.com/2025/12/02/amazon-releases-an-impressive-new-ai-chip-and-teases-a-nvidia-friendly-roadmap/](https://techcrunch.com/2025/12/02/amazon-releases-an-impressive-new-ai-chip-and-teases-a-nvidia-friendly-roadmap/)

亚马逊网络服务（AWS）在AWS re:Invent 2025大会上推出了其第三代AI训练芯片Trainium3。这款3纳米的Trainium3为UltraServer系统提供动力，与前代产品相比，在AI训练和推理方面的性能提升了4倍以上，内存也增加了4倍。

Trainium3 UltraServer系统专为大规模可扩展性设计，能够连接数千台服务器，提供多达100万个Trainium3芯片——比上一代增加了10倍，每个UltraServer容纳144个芯片。AWS还强调了该芯片的能源效率，声称其效率提高了40%，这意味着为AWS及其云客户都节省了成本。Anthropic、Karakuri、SplashMusic和Decart等公司已在使用Trainium3，并报告推理成本显著降低。

AWS还预告了其未来AI训练芯片的路线图，宣布Trainium4已在开发中。Trainium4将再次实现性能飞跃，关键在于它将支持英伟达（Nvidia）的NVLink Fusion高速芯片互连技术。这将使Trainium4驱动的系统能够与英伟达GPU互操作并扩展性能，从而更容易吸引使用英伟达CUDA标准构建的AI应用程序迁移到亚马逊云，同时利用AWS具有成本效益的服务器技术。目前尚未提供Trainium4的具体发布时间表。

---

## 36. 印度废除智能手机预装官方网络安全应用的命令

**原文标题**: India scraps order to pre-install state-run cyber safety app on smartphones

**原文链接**: [https://www.bbc.com/news/articles/clydg2re4d1o](https://www.bbc.com/news/articles/clydg2re4d1o)

印度已撤销其备受争议的命令，该命令要求智能手机制造商在新设备上强制预装国有网络安全应用Sanchar Saathi。上周发布的这项指令原要求在90天内预装该应用，且用户无法禁用或限制它，从而引发了公众对隐私和监控问题的强烈抗议。

政府曾辩称，该应用对于验证手机真伪和防止欺诈是必要的。然而，网络安全专家批评此举侵犯了公民的隐私权。据报道，包括苹果和三星在内的主要智能手机制造商抵制了这项命令，理由是缺乏协商以及对用户隐私的担忧。

尽管通信部长乔蒂拉迪蒂亚·辛迪亚驳斥了监控担忧，但政府最终撤回了这项命令，理由是该应用“日益被接受”。Sanchar Saathi应用已获得1400万次下载，据报道每天帮助识别2000起欺诈事件。互联网自由基金会等数字权益倡导团体对此撤销表示欢迎，但建议“谨慎乐观”，直至发布正式法律命令。

---

## 37. 小型餐厅和咖啡馆的免费静态网站生成器

**原文标题**: Free static site generator for small restaurants and cafes

**原文链接**: [https://lite.localcafe.org/](https://lite.localcafe.org/)

本文介绍了一个专为小型餐馆和咖啡馆量身定制的免费静态网站生成器概念。所提供的内容作为一个示例，展示了此类网站可能显示的内容，具体来说，是一个“今日特价”菜单项。这道特色菜售价为$9.99，被描述为厨师精选，采用时令食材。它详细介绍了一道海鲜意面，融合了各种海鲜，如虾、蛤蜊、贻贝和扇贝，再搭配意面。这道菜提供多种酱汁选择，包括清淡、蒜香番茄酱，奶油番茄酱，白葡萄酒酱，甚至还有奶油/辛辣的卡真风味。

---

## 38. 三十年前的今天：网景和昇阳宣布JavaScript

**原文标题**: 30 years ago today "Netscape and Sun announce JavaScript"

**原文链接**: [https://web.archive.org/web/20070916144913/http://wp.netscape.com/newsref/pr/newsrelease67.html](https://web.archive.org/web/20070916144913/http://wp.netscape.com/newsref/pr/newsrelease67.html)

1995年12月4日，网景通信公司与太阳微系统公司宣布推出JavaScript，这是一种开放的、跨平台的面向对象脚本语言。JavaScript专为企业网络和互联网设计，通过使HTML页面作者和应用程序开发人员（即使编程经验有限）也能动态编写客户端和服务器上对象的行为脚本，从而补充了Sun的Java。

该语言旨在创建连接对象和资源的实时在线应用程序，并与Java和HTML集成。初始版本作为网景导航器2.0测试版的一部分提供。

该声明得到了28家行业领先公司的支持，其中包括美国在线、苹果电脑、美国电话电报公司、惠普、Informix、Intuit、Macromedia、Novell和甲骨文，所有这些公司都认可JavaScript作为开放标准，并计划将其纳入未来产品中。网景和Sun还计划将JavaScript的规范提交给W3C联盟和互联网工程任务组（IETF），作为一种开放的、免费授权的互联网脚本语言标准，并提供免版税的源代码参考实现以鼓励广泛采用。网景承诺在其客户端、服务器和开发工具产品中全面支持Java和JavaScript。

---

## 39. 编程达到顶峰

**原文标题**: Programming peaked

**原文链接**: [https://functional.computer/blog/programming-peaked](https://functional.computer/blog/programming-peaked)

萨米尔·塔尔瓦尔在《编程已过巅峰》一文中指出，与15年前相比，2025年所见的现代编程已然衰落。他描述了当前由带有类型的JavaScript主导的编程图景，其中其依赖管理器（NPM）是安全漏洞和恶意软件包的来源。代码常由AI生成，导致有害组件的频繁安装。开发涉及VS Code等资源密集型IDE、缓慢的TypeScript编译，以及耗时数天的漫长拉取请求流程。

容器化，采用“大杂烩”式的Dockerfile，导致构建缓慢、不必要的依赖（如Perl），以及通过禁用扫描器来规避的安全问题。部署依赖于Kubernetes的无类型、模板化YAML，运行在昂贵的租赁云虚拟机上，导致行为不可预测且缺乏直接的硬件控制。矛盾的是，构建和部署时间从几分钟增加到几小时甚至几天。

相比之下，塔尔瓦尔深情回忆2010年，当时Java开发在性能较低的硬件上也能快速编译，Eclipse等高效IDE具备高级重构功能，且单元测试迅速。团队结对编程，并使用来自Maven Central等经过审查的仓库的JAR包，直接部署到本地数据中心的物理服务器。这种方法提供了可靠性、速度和直接监管，通常没有专门的测试人员，但仍能产出健壮的系统。

作者怀念过去可靠的工具、周密的依赖管理、快速的代码到交付时间，以及测试人员提供的保障。尽管承认Git和构建良好的容器等一些优点，但他将整体衰落归因于NPM、Node.js、React和Electron的普遍影响，这些工具将JavaScript推向了可能并非最合理的使用场景。他渴望“重置”回更合适的工具选择。

---

## 40. 绘制美国医疗保健系统的资金流向

**原文标题**: Mapping the US healthcare system’s financial flows

**原文链接**: [https://healthisotherpeople.substack.com/p/an-abominable-creature](https://healthisotherpeople.substack.com/p/an-abominable-creature)

Andrew Sprung撰写的文章《令人憎恶的生物：描绘美国医疗保健系统的资金流向》借鉴了KFF的分析，阐述了美国医疗保健系统资金流动的巨大复杂性和不透明性。该系统每年涉及近5万亿美元，其特点是“循环流动”，资金主要源自家庭和雇主（通过税收和保费），流经保险公司和政府项目，最终支付给医疗服务提供者。

一个关键要点是该系统“混乱”且“令人憎恶”的结构，使得难以确定谁支付给谁、支付了什么以及以什么价格支付。大量的交易和中介机构进一步加剧了这种不透明性。文章强调，虽然整个系统支出占GDP近18%，但大部分资金（超过4万亿美元）流向了医疗服务提供者。Sprung指出，医院护理和医生/临床服务的支出所占份额过高，而零售处方药和其他医疗保健支出所占份额较小但仍很重要。

该摘要强调，美国医疗保健系统并非一个单一实体，而是由公共和私人支付方组成的碎片化集合，形成了错综复杂的资金交换网络。这种复杂性阻碍了透明度和理解，使得难以发现效率低下之处或查明巨额支出的最终受益者。

---

## 41. EmacsConf 2025

**原文标题**: EmacsConf 2025

**原文链接**: [https://emacsconf.org/2025/](https://emacsconf.org/2025/)

EmacsConf 2025是一场即将举行的在线会议，致力于“GNU Emacs和Emacs Lisp的乐趣”，定于2025年12月6日和7日（周六至周日）举行。组织者正在积极筹备此次活动，并寻求帮助以使其成功，鼓励大家积极参与和推广。

本次会议将再次在线举行，通过仅使用自由软件作为其基础设施和流媒体设置，秉持对自由的全面承诺。

为了社区互动，与会者和组织者可以通过以下多种渠道进行联系：
*   **综合讨论：** `emacsconf-discuss` 邮件列表。
*   **组织讨论：** `emacsconf-org` 邮件列表。
*   **电子邮件：** `emacsconf-org@gnu.org`（公开）或 `emacsconf-org-private@gnu.org`（私密）。
*   **IRC：** 使用IRC客户端或通过 `chat.emacsconf.org` 网页浏览器，在 `irc.libera.chat` 上加入 `#emacsconf` 频道。

---

## 42. Show HN: Fresh — 一款用 Rust 编写的新终端编辑器

**原文标题**: Show HN: Fresh – A new terminal editor built in Rust

**原文链接**: [https://sinelaw.github.io/fresh/](https://sinelaw.github.io/fresh/)

"Fresh" 是一款使用 Rust 构建的新型终端文本编辑器，它强调易用性、现代可扩展性和零延迟性能。它设计轻巧快速，能够可靠地处理数千兆字节的文件而不会出现卡顿。

该编辑器专注于探索性和用户友好性，具有原生 UI、完整的菜单系统、强大的命令面板和全面的鼠标支持，从而使习惯于图形化编辑器的用户更容易过渡。

为了实现现代可扩展性，Fresh 允许插件使用 TypeScript 编写，并在沙盒化的 Deno 环境中安全运行。这提供了对现代 JavaScript 生态系统的访问，同时保持了稳定性。

其全面的功能集包括强大的文件管理（标签页、文件浏览器）、高级编辑功能（多光标、撤销/重做、智能缩进）、搜索和替换以及高效导航。它集成了语言服务器协议（LSP），提供自动补全、诊断和代码操作等功能。其他生产力工具包括分割窗格、Markdown 预览、键盘宏和 Git 集成。

Fresh 可以通过 npm、npx、从源代码使用 Cargo 或从 GitHub 下载预构建的二进制文件进行安装。

---

## 43. 李群对于物理学中某些最基本的理论至关重要。

**原文标题**: Lie groups are crucial to some of the most fundamental theories in physics

**原文链接**: [https://www.quantamagazine.org/what-are-lie-groups-20251203/](https://www.quantamagazine.org/what-are-lie-groups-20251203/)

李群是强大的数学工具，它融合了群论、几何学和线性代数，因此对物理学中的基本理论以及数论和化学都至关重要。与代表离散变换（如三角形对称性）的离散群不同，李群捕捉连续对称性，例如飞盘的旋转。这些群可以被形象化为光滑、连续的形状，称为流形——例如，二维旋转群SO(2)形成一个圆。

这种光滑的几何特性是它们有用性的关键。数学家可以应用几何学和微积分的工具。对李群流形的一个小区域进行局部放大，会揭示出一条直线近似，这被称为李代数。这个切空间将复杂的群运算简化为更易于处理的线性代数问题，从而使群之间的计算和比较变得更加直接。

在物理学中，李群不可或缺。基本力——引力、电磁力和核力——都由李群对称性定义，这有助于解释关于物质的基本谜团。此外，埃米·诺特定理证明了物理系统中的每个李群对称性都对应一个守恒定律。例如，时间平移对称性（一个李群）意味着能量守恒。这些群由马吕斯·索菲斯·李在19世纪70年代发展而来，至今仍是理解自然界潜在对称性的重要工具。

---

## 44. 8086 微代码浏览器

**原文标题**: 8086 Microcode Browser

**原文链接**: [https://nand2mario.github.io/posts/2025/8086_microcode_browser/](https://nand2mario.github.io/posts/2025/8086_microcode_browser/)

受重新创建8086芯片过程的启发，作者开发了一个在线交互式8086微码ROM浏览器，其数据基于Andrew Jenner于2020年的提取。

该浏览器将每条21位微指令解码为可读字段，附带解释性工具提示和可点击的跳转目标，便于通过直接和间接跳转、调用以及分支进行导航。一个关键功能是“按指令浏览”，它允许用户从大约300条有文档记录的8086指令中进行选择，并直接跳转到它们对应的微码入口点，从而简化了对大约60个独特例程的探索。

文章还分享了来自微码的一些有趣的见解：
*   寄存器ID是上下文相关的；例如，'10100'作为源时指代SIGMA，但作为目的时则指代tmpaL。
*   内部命名不一致，N和R是同一个物理寄存器，并且SI被称为IJ。
*   IP（程序计数器）指向的是*下一个预取地址*，而不是下一条指令。`CORR`微操作用于在分支和中断时回溯IP。
*   大多数算术指令巧妙地重用了仅仅四条微指令（008–00B），其中`XI`微操作根据操作码或ModRM位调整其算术行为，展示了1978年英特尔高效的设计。

---

## 45. 欧洲自由软件基金会删除了其在X上的账号

**原文标题**: The Free Software Foundation Europe deleted its account on X

**原文链接**: [https://fsfe.org/news/2025/news-20251204-01.en.html](https://fsfe.org/news/2025/news-20251204-01.en.html)

2025年12月4日，欧洲自由软件基金会（FSFE）宣布已永久删除其在X（即此前的Twitter）上的账户。FSFE表示，该平台已不再符合其价值观，并且不再是一个可行的交流空间，已演变成一个“充满敌意、虚假信息和利润驱动控制的中心化竞技场”。

该组织最初加入Twitter是为了推广自由软件的价值观，与政策制定者和记者互动，并接触不熟悉软件自由的个人。然而，自埃隆·马斯克收购并将其更名为X以来，FSFE发现虚假信息、骚扰和仇恨言论显著增加。他们还提到了对X算法优先处理负面内容以及日益增长的隐私问题的担忧。

FSFE承认他们从未对该平台的专有性质感到满意，但鉴于其当前的方向和氛围，FSFE决定离开。FSFE将继续使用其他专有平台来接触更广泛的受众，但强烈鼓励那些认同他们对数字自由和去中心化承诺的人加入他们在Fediverse上的行列，他们在Mastodon和Peertube上都很活跃。Fediverse被强调为一个替代方案，它赋予用户透明度、自主性和弹性，这与以利润为驱动的中心化平台不同。

---

## 46. WinQuake为何存在以及其工作原理

**原文标题**: Why WinQuake exists and how it works

**原文链接**: [https://fabiensanglard.net/winquake/index.html](https://fabiensanglard.net/winquake/index.html)

WinQuake 由 id Software 开发，旨在解决原始 `quake.exe` 在 Windows 95 和 Windows NT 上运行时存在的显著局限性。`quake.exe` 在 Windows 95 上运行时，由于 DOS 虚拟机的开销，帧率比 DOS 版本降低了 25%，它依赖复杂的 TCP/IP 技术，且与 Windows NT 的虚拟 DOS 机（NTVDM）不兼容。

WinQuake 旨在提供一个更快速、原生的 Win32 应用程序，具备直接的 Winsock 访问能力和 NT 兼容性。它取得了令人瞩目的性能，将帧率提升至与 DOS 版 `quake.exe` 基准测试表现相差无几，差距在 6% 以内。

这一目标通过一个复杂的架构得以实现，该架构为输入、音频和视频采用了多个后端，并可通过命令行参数进行配置。
*   **音频：** WinQuake 提供 DirectSound 以实现低延迟（但 CPU 占用更高）或 WinMM（波形声音）以实现更高帧率（但延迟更高）。
*   **输入：** 它默认使用 DirectInput 实现更流畅的响应，或使用传统的 Winuser.h API，并通过 joystickapi.h 提供摇杆支持。
*   **视频：** 这是最复杂的部分，提供了五种主要模式：
    1.  **DIB (GDI)：** 最安全、最慢，也是唯一的窗口模式，依赖于标准的 Windows 图形系统。
    2.  **SciTech 的多平台图形库 (MGL)：** 一个关键的第三方库，它抽象了 GDI 之外的各种视频系统。
    3.  **DirectDraw：** 微软的 2D 全屏 API，提供比 GDI 更好的性能，但依赖于 DirectX 安装和驱动程序。
    4.  **WinDirect (SciTech 的专有技术)：** 这种创新的运行时允许 WinQuake 绕过 GDI/DirectDraw，像 DOS 应用程序一样直接访问显示硬件（VBEAF、VESA、VGA），从而实现最大性能。

通过动态选择最佳渲染路径——优先选择 DirectDraw 或 WinDirect，并将 DIB 作为备用方案——并优化音频/输入，WinQuake 提供了显著改善的用户体验，证明了其存在的价值，并确保了其卓越的向后兼容性，即使在现代 Windows 版本上也是如此。

---

## 47. Acme，改变互联网的协议之一的简史

**原文标题**: Acme, a brief history of one of the protocols which has changed the Internet

**原文链接**: [https://blog.brocas.org/2025/12/01/ACME-a-brief-history-of-one-of-the-protocols-which-has-changed-the-Internet-Security/](https://blog.brocas.org/2025/12/01/ACME-a-brief-history-of-one-of-the-protocols-which-has-changed-the-Internet-Security/)

本文详细阐述了ACME（自动化证书管理环境）协议的历史及其对互联网安全的深远影响。2015年之前，网站加密的普及率较低（约40%），这主要是由于获取和管理TLS证书的成本高昂且过程复杂。爱德华·斯诺登在2013年的爆料更是凸显了这一安全鸿沟。

为解决此问题，由Mozilla、EFF、Akamai、Cisco和密歇根大学等组成的合作团体于2015年创立了Let's Encrypt。它作为一个自动化、免费的证书颁发机构而诞生，旨在使TLS加密普遍可用。自动化对于Let's Encrypt的可行性及其以小团队实现规模化运营至关重要，这项使命正是由ACME协议提供支持的。

ACME允许客户端软件通过挑战（HTTP、DNS或TLS）自动向证书颁发机构证明对域名的控制权，从而消除了人工干预。ACME经过开放开发，并经历了IETF标准化过程，最终于2019年形成了RFC 8555。这一过程改进了协议，引入了诸如证书请求优先流程、认证请求以及淘汰有缺陷的挑战方法等安全改进。ACME的灵活性，特别是通过DNS挑战，使得除了HTTP之外的各种互联网协议（如SMTP）也能得到保护。

在ACME的推动下，Let's Encrypt取得了巨大的成功：它现在颁发了超过7亿张有效证书，占公共TLS服务器证书的60%以上，并将全球HTTPS使用率从39%提升到83%以上。ACME从根本上普及了加密技术，使其成为标准而非例外。

---

## 48. React和Next.js的严重RCE漏洞

**原文标题**: Critical RCE Vulnerabilities in React and Next.js

**原文链接**: [https://www.wiz.io/blog/critical-vulnerability-in-react-cve-2025-55182](https://www.wiz.io/blog/critical-vulnerability-in-react-cve-2025-55182)

在 React 服务器组件 (RSC) 的“Flight”协议中，已发现严重的未经身份验证的远程代码执行 (RCE) 漏洞，包括 CVE-2025-55182 (React) 和 CVE-2025-66478 (Next.js)。这些缺陷源于 `react-server` 包中的不安全反序列化，允许特制 HTTP 请求在服务器上执行特权 JavaScript 代码。

这些漏洞是严重的，影响了 Next.js 等流行框架的默认配置。标准的生产环境 Next.js 应用程序无需开发者修改代码即可被利用，且利用成功率接近 100%。Wiz Research 指出 39% 的云环境包含易受攻击的实例，并且所有云环境中有 44% 拥有公开暴露的 Next.js 应用程序。

受影响的产品包括 `react-server-dom` 的 19.0.0、19.1.0、19.1.1 和 19.2.0 版本，以及 Next.js App Router 的 14.3.0-canary、15.x 和 16.x 版本。其他捆绑 `react-server` 的框架（例如 Vite RSC、RedwoodSDK）也可能受影响。

必须立即进行修补。组织必须将 `react-server-dom` 升级到 19.0.1、19.1.2 或 19.2.1 版本，并将 Next.js 升级到强化版本，例如 14.3.0-canary.88、15.0.5、15.1.9、15.2.6、15.3.6、15.4.8、15.5.7 或 16.0.7。漏洞利用的详细信息正在被保留，以促进整个生态系统的修补工作。

---

## 49. 日本四缸发动机如此可靠，25年后仍在生产。

**原文标题**: Japanese four-cylinder engine is so reliable still in production after 25 years

**原文链接**: [https://www.topspeed.com/reliable-japanese-four-cylinder-engine-still-in-production/](https://www.topspeed.com/reliable-japanese-four-cylinder-engine-still-in-production/)

本田K系列发动机是一款享誉盛名的四缸动力系统，因其卓越的性能、可靠性和效率的平衡而备受赞誉，至今已生产近25年。该系列于2001年推出，旨在取代B系列和H系列，以满足更严格的排放标准并提高热效率。

第一代K系列采用了轻量化铝制缸体、锻造曲轴、链条驱动双顶置凸轮轴以及先进的i-VTEC系统。该系统结合了可变气门正时、升程控制和凸轮轴相位调整，以实现宽广的扭矩和强劲的高转速呼吸。它于2001年在本田Stream车型上首次亮相，随后被思域和Integra等热门车型采用。

当前的K20C一代继承了这一传统，融入了强化型封闭式水道铝制缸体、直喷技术、优化气流和紧凑型涡轮增压器，以满足更严格的现代排放和热管理要求。工程师们专注于实际驾驶性能和长期耐用性，通过严苛的耐久性测试验证了设计。

除了公路之外，K系列还在赛车运动中展现了其韧性，在房车锦标赛中，其耐用性、稳定的热行为和宽广的工作范围备受推崇，为其声誉锦上添花，并为生产改进提供了参考。

本田持续使用K系列发动机，得益于其适应性强的架构，该架构支持现代效率目标、高耐久性以及与混合动力系统的灵活集成。尽管L系列也是未来的焦点，但K系列经证实卓越的性能、弹性和市场吸引力确保了其持续的重要性，尤其对于性能导向的本田和讴歌车型而言。

---

## 50. 微软降低AI软件增长目标

**原文标题**: Microsoft lowers AI software growth targets

**原文链接**: [https://finance.yahoo.com/news/microsoft-lowers-ai-software-sales-141531121.html](https://finance.yahoo.com/news/microsoft-lowers-ai-software-sales-141531121.html)

微软否认了The Information的一篇报道，该报道声称，在上一财年销售人员未能达到目标后，微软降低了某些AI软件产品的销售增长目标。该报道援引Azure云计算部门员工的话称，一个Azure销售部门将本财年Foundry的增长目标从50%降至25%。

微软表示，该报道错误地将“增长”与“销售配额”混为一谈，并证实AI产品总销售配额并未降低。否认之后，微软股价收窄了盘初跌幅。

这篇报道发布之际，正值人们对“AI泡沫”的担忧，原因是科技公司估值过高和采用率缓慢，麻省理工学院的一项研究发现，只有5%的AI项目能超越试点阶段。The Information还援引了凯雷集团的例子，称其在数据整合方面遇到困难后，削减了对Copilot Studio的支出。

分析师承认，企业正处于AI采用的早期阶段，预计会面临挑战，但他们看到了提高生产力的希望。美国科技巨头面临压力，需要展示其在AI领域巨额投资的回报。微软报告称，第一季度资本支出创下近350亿美元的纪录，并预计支出将增加以克服供应链限制。尽管存在这些担忧，微软的AI推广仍取得了成功，Azure营收增长了40%，公司市值一度达到4万亿美元。

---

## 51. 亿科西亚：最环保的人工智能来了

**原文标题**: Ecosia: The greenest AI is here

**原文链接**: [https://blog.ecosia.org/ecosia-ai/](https://blog.ecosia.org/ecosia-ai/)

Ecosia 推出了新的 AI 功能，“概览”（Overviews）和“AI 搜索”（AI Search），将自己定位为在 AI 领域中一个有益、注重隐私、且地球优先的替代方案。“概览”在搜索结果顶部提供快速、引用来源的摘要，并可选择禁用。“AI 搜索”是一种交互式聊天模式，用于回答详细问题，包括基于环境科学的生态提示。

作为一个非营利组织，Ecosia 使用更小、更高效的 AI 模型，并避免视频生成等能耗密集型功能。至关重要的是，它产生的可再生能源（太阳能和风能）多于其 AI 功能的消耗，已投资 1800 万欧元用于项目，以取代化石燃料并加速绿色能源转型。他们使用 AI 能源评分（AI Energy Score）等工具，以透明地追踪能源使用情况。

隐私至关重要：Ecosia 仅收集必要数据，并运营独立的欧洲搜索索引以实现更大程度的控制。与大型科技公司不同，它不与电子邮件、地图或支付平台集成，确保用户数据不会被整合。受 GDPR 约束，Ecosia 声明其宗旨是“为了树木，而非您的数据”。Ecosia 邀请用户反馈，共同塑造一个更智能、更友善的未来。

---

## 52. 科亚 DHCP：现代开源 DHCPv4 和 DHCPv6 服务器

**原文标题**: Kea DHCP: Modern, open source DHCPv4 and DHCPv6 server

**原文链接**: [https://www.isc.org/kea/](https://www.isc.org/kea/)

ISC 宣布发布 Kea 3.0.0，这是其现代开源 DHCPv4 和 DHCPv6 服务器的一次重大更新。此版本尤为引人注目，因为它 是 Kea 的首个长期支持（LTS）版本。

---

## 53. 毁灭战士本可以有PC扬声器音乐

**原文标题**: DOOM could have had PC Speaker Music

**原文链接**: [https://lenowo.org/viewtopic.php?t=45](https://lenowo.org/viewtopic.php?t=45)

本文探讨了一个长期存在的问题：《毁灭战士》是否能够通过PC扬声器支持音乐，而PC扬声器通常被认为对实时游戏逻辑来说资源消耗过大，尤其是在286等老旧系统上。尽管《毁灭战士》包含了一个PC扬声器驱动程序，但它处理音效的效果很差，并且通常被禁用。

然而，作者对486处理器上的这一限制表示怀疑，并决定进行调查。他们开发了一个“PC扬声器sndserver补丁”以实现音乐播放。这涉及为PC扬声器音乐创建一种高效的32位文件格式`pcsp`，该格式包含频率、持续时间比例和持续时间值。作者随后在《毁灭战士》的`sndserver`中实现了一个优先级混音器，借鉴了Adlib目标中现有的基础工作。

测试揭示了一个令人惊讶的结果：运行带有PC扬声器音乐补丁的《毁灭战士》没有表现出明显的速度差异。这表明，即使在目标硬件上，PC扬声器音乐也确实可行，且没有显著的性能开销。

该补丁尚未公开，因为它目前只支持E1M1的音轨。作者计划在实现更多音乐并修复`sndserver`在现代Linux系统上的其他问题后，尽快发布该补丁。

---

## 54. HN 展示：微克兰迪亚，一个残酷真实的城市建造游戏

**原文标题**: Show HN: Microlandia, a brutally honest city builder

**原文链接**: [https://microlandia.city](https://microlandia.city)

《微型大陆》是一款新的城市建设游戏，它拥有温馨舒适的体素画面，但却对城市生活进行了“残酷真实”且深度细致的模拟。作为市长，玩家将管理一座城市，其中虚拟市民的生活基于真实的统计数据进行模拟，涵盖健康、就业（存在被解雇或转向犯罪的风险）、人际关系以及公众对项目的反对等方方面面。游戏模拟了复杂的经济因素，包括公司破产、失业率上升、贪婪的房东、昂贵的基础设施以及税费带来的错综复杂的影响。玩家将面临艰难的抉择，报纸会报道他们的行动，而经济衰退和疫情等随机事件则会考验他们的能力。

游戏的模拟机制是根据世界银行和美国劳工统计局等机构的真实世界数据精心建模的，旨在为玩家提供对现代社会、经济和环境挑战的真知灼见。其模拟参数可供查阅。《微型大陆》正积极开发中，承诺将持续更新，带来新功能和更深层次的模拟。开发者承诺不会推出续作，不会提供付费DLC或扩展包，也不会包含游戏内购，他们认为所有内容更新都应免费提供。

---

## 55. GSWT: 高斯泼溅汪氏瓦片

**原文标题**: GSWT: Gaussian Splatting Wang Tiles

**原文链接**: [https://yunfan.zone/gswt_webpage/](https://yunfan.zone/gswt_webpage/)

GSWT（高斯泼溅王氏瓦片）是一种新颖的基于瓦片的框架，旨在解决如何将3D高斯泼溅（3DGS）扩展，以从单个捕获的样本合成大规模或无限地形的挑战。该方法由香港科技大学（HKUST）和Eyeline Labs的研究人员为SIGGRAPH Asia 2025开发，以王氏瓦片为基础。

每个GSWT瓦片编码一个局部高斯场，其设计包含边界约束，以确保在拼接时实现无缝过渡。这种方法允许高斯场在任意表面上进行随机而连续的平铺，从而能够程序化生成广阔多样的地形。

该流程包含多个步骤：首先，从多视角图像重建多层次细节（LOD）的3DGS样本。对于每个LOD，通过采样边缘和中心块，并利用语义感知的图割算法，生成一组王氏瓦片。在渲染之前，每个瓦片都会被预排序，以实现高效、无需排序的泼溅。在运行时，系统使用一个工作线程即时执行瓦片拼贴，而主线程则负责渲染。整个过程，再加上量身定制的渲染优化，实现了大规模3DGS地形的实时渲染。

---

## 56. 研究显示：人发通过“拉动”而非“推动”生长

**原文标题**: Human hair grows through 'pulling' not pushing, study shows

**原文链接**: [https://phys.org/news/2025-12-human-hair.html](https://phys.org/news/2025-12-human-hair.html)

无法访问文章链接。

---

## 57. AI正在瓦解现代社会的道德基础

**原文标题**: AI Is Breaking the Moral Foundation of Modern Society

**原文链接**: [https://eyeofthesquid.com/ai-is-breaking-the-moral-foundation-of-modern-society-a145d471694f](https://eyeofthesquid.com/ai-is-breaking-the-moral-foundation-of-modern-society-a145d471694f)

文章《人工智能正在瓦解现代社会的道德基础》指出，人工智能，特别是大型语言模型（LLMs），本身并未变得不道德，而是无意中揭露并挑战了人类社会不一致且往往自相矛盾的道德基础。

通过从海量的人类交流和行为数据集中学习，人工智能反映了人类道德的复杂性、相对性以及常常存在的偏见。作者认为，人工智能揭示了人类理想的伦理原则与多样化、冲突的道德观点这一混乱现实之间的“道德鸿沟”。当面对伦理困境时，人工智能突出表明人类是如何通过细致入微、依赖语境的判断来处理相互冲突的价值观（例如自由与安全），而这些判断是难以普遍编纂的。

这迫使社会重新审视“好”或“道德”究竟意味着什么，因为在缺乏普遍共识的定义下，试图使人工智能与人类价值观保持一致的努力往往会失败。此外，人工智能生成虚假内容的能力侵蚀了信任，模糊了真相的界限，而它对人类偏见的反映则强调了偏见的普遍存在。文章总结道，真正的“危机”并非人工智能发展出自身的恶意道德，而是它强大地映射和放大人类自身道德不一致和混乱的能力，这要求社会更深入地审视我们集体的伦理框架。

---

## 58. 数据中心的快速增长导致伦敦新房建设延迟。

**原文标题**: The rapid growth of data centres is delaying new homes in London

**原文链接**: [https://www.bbc.com/news/articles/c0mpr1mvwj3o](https://www.bbc.com/news/articles/c0mpr1mvwj3o)

“耗能巨大”的数据中心快速扩张，正严重推迟伦敦的新住房开发项目，加剧了该市的住房危机。伦敦议会规划与再生委员会的一份报告警告称，电网，尤其是在伦敦西部伊灵、希灵登和豪恩斯洛等行政区，已达到满负荷。这导致一些已完工的住房项目面临可能延迟至2037年才能连接电网的困境，影响了住房和经济增长。

数据中心为人工智能和流媒体等数字服务提供动力，消耗大量电力。尽管目前占英国电力需求的不到10%，但预计到2025年至2050年间，其用电量将飙升高达600%，超过一半的新数据中心计划设在伦敦。一个典型的数据中心用电量相当于10万户家庭。

大伦敦政府（GLA）已与英国国家电网和英国能源监管局（Ofgem）实施了短期解决方案，以缓解眼前的延误，但报告强调，需要对电网容量进行全面的长期规划。行业机构正在敦促加快电网升级，认为国家电网2037年实现额外供电的目标对于当前需求来说过于缓慢。

建议包括为数据中心设立一个独立的规划类别，以改善能源协调；并要求伦敦市长将专门的数据中心政策纳入下一版《伦敦规划》。政府也在探索“定制方案”，以同时支持数据中心和住房领域。

---

## 59. C 语言中的大小检查数组参数

**原文标题**: Checked-size array parameters in C

**原文链接**: [https://lwn.net/SubscriberLink/1046840/3eb9029084cc9e1e/](https://lwn.net/SubscriberLink/1046840/3eb9029084cc9e1e/)

本文探讨了在C语言中为数组参数引入编译时大小检查的方法，这是该语言的一个常见弱点，可能导致错误和漏洞，尤其是在密码学等关键代码中。

最初，像 `void func(u8 arr[SIZE])` 这样的函数原型并不能保证传入的数组与 `SIZE` 匹配。开发者Ard Biesheuvel提议将参数类型改为数组指针，例如 `const u8 (*arr)[SIZE]`。这强制了精确的大小匹配并启用了编译器检查，但要求调用者通过添加 `&` 运算符进行适配。

Jason Donenfeld随后提出了一种鲜为人知的C语言特性：在数组参数声明中使用 `static` 关键字，例如 `const u8 arr[static SIZE]`。这种方法也触发了编译器检查，但关键在于它不需要调用者端进行更改。`static` 主要警告传入的数组是否 *小于* 指定大小，而不是要求精确的大小匹配。Linus Torvalds尽管称这种语法为“可怕的 hack”，但仍批准了它的使用，并指出它在内核中已存在。

评论区揭示了进一步的争论。一些人认为 `static N` 大部分是不必要的，因为现代GCC在没有 `static` 的情况下也可以为 `[N]` 提供类似的“数组太小”警告（尽管这些警告在内核中通常被禁用）。批评者指出，根据C标准，`static N` 主要是一个优化提示，不保证诊断，并且通过暗示非空和非零数组大小可能会引入未定义行为。尽管有这些批评和其“可怕的 hack”的称谓，文章预测 `static` 将在内核中得到更广泛的采用以增强安全性。

---

## 60. 研究人员发现可从火星土壤产氧的微生物

**原文标题**: Researchers Find Microbe Capable of Producing Oxygen from Martian Soil

**原文链接**: [https://scienceclock.com/microbe-that-could-turn-martian-dust-into-oxygen/](https://scienceclock.com/microbe-that-could-turn-martian-dust-into-oxygen/)

研究人员发现，一种名为Chroococcidiopsis的顽强极端微生物能够在模拟火星土壤上生长并产生氧气。这一发现是实现人类在火星上长期生存的重要一步，解决了无需地球持续补给即可提供可呼吸空气的关键挑战。

实验表明，这种微生物不仅能在模拟火星风化层上存活，还能茁壮成长，提取养分并释放氧气作为其自然副产品。与富饶的类地土壤不同，它即使在资源有限的情况下也能有效运作。至关重要的是，Chroococcidiopsis还表现出非凡的韧性，能够承受辐射和低压等对大多数生命而言是致命的极端条件。它甚至能够修复受辐射损伤的DNA。

对于太空规划者而言，这提供了一种有前景的天然可再生氧气来源，使未来的火星定居点更加现实。尽管在扩大培养规模以及在火星环境中保护这些生物方面仍存在挑战，但这项研究是至关重要的第一步。它也强化了生命具有令人难以置信的适应性的观点，暗示了太阳系其他地方存在生命的潜力。实际的重点在于将这类微生物整合到闭环系统中，以创建自给自足的栖息地，使人类能够直接在火星上“种植”自己的氧气。

---

## 61. Quad9 DOH HTTP/1.1 退役，2025年12月15日

**原文标题**: Quad9 DOH HTTP/1.1 Retirement, December 15, 2025

**原文链接**: [https://quad9.net/news/blog/doh-http-1-1-retirement/](https://quad9.net/news/blog/doh-http-1-1-retirement/)

Quad9将于2025年12月15日停止支持使用HTTP/1.1的DNS-over-HTTPS (DoH)。这一决定是基于多方面因素考量：HTTP/2是DoH的推荐标准，HTTP/1.1的底层库已临近生命周期终点，并且Quad9有限的开发资源将更好地分配给新功能和核心稳定性。此外，HTTP/1.1在速度、可扩展性和潜在安全方面存在挑战。

绝大多数用户，包括使用Chrome、Firefox和Safari等现代浏览器或Android和iOS等操作系统的用户，将不会受到影响，因为他们的设备已为DoH使用HTTP/2或更高版本。

然而，老旧或不兼容的设备和软件可能会失去DoH功能。具体而言，已配置DoH的MikroTik设备已知依赖HTTP/1.1，届时将停止工作。据了解，巴西存在大量此类用户社区。

受影响的用户应升级其系统，切换到DNS-over-TLS（该协议不使用HTTP），或者，作为最后的手段，恢复使用未加密的DNS，并了解其安全隐患。

鉴于Quad9的隐私政策禁止存储用户数据，这意味着他们无法直接通知受影响的用户。因此，他们鼓励社区分享这一关键信息，以帮助用户避免服务中断。这一转变将使Quad9能够部署更新的协议并刷新其平台。

---

## 62. Tunnl.gg

**原文标题**: Tunnl.gg

**原文链接**: [https://tunnl.gg](https://tunnl.gg)

Tunnl.gg 被介绍为一项服务，它提供将本地开发服务器（localhost）暴露到互联网的最简单解决方案。它将自己定位为实现这种连接最简单的方法。

---

## 63. VA员工指出甲骨文公司构建的电子健康记录存在危险错误

**原文标题**: VA staff flag dangerous errors in Oracle-built electronic health record

**原文链接**: [https://www.washingtonpost.com/investigations/2025/12/03/veterans-administration-va-hospitals-health/](https://www.washingtonpost.com/investigations/2025/12/03/veterans-administration-va-hospitals-health/)

无法访问文章链接。

---

## 64. 理解 ECDSA

**原文标题**: Understanding ECDSA

**原文链接**: [https://avidthinker.github.io/2025/11/28/understanding-ecdsa/](https://avidthinker.github.io/2025/11/28/understanding-ecdsa/)

这篇文章《理解ECDSA》旨在揭开椭圆曲线数字签名算法的神秘面纱，重点关注其在以太坊中的应用，并探讨签名可塑性。作者采用了一种独特的自学方法，在没有外部资源的情况下重建知识，为开发者和审计师提供了一个“朴素”但富有洞察力的视角。读者被设定为“审计师”，以批判性地评估内容。

引入的基础数学概念是模运算。文章通过日历类比，解释了`mod`运算符、等价类，以及如何始终如一地找到一个数的正代表（即使是负输入）。文中阐明，`mod p`可以在加法和乘法的任何步骤中应用，但不能在幂运算中应用。

ECDSA的一个关键要素是乘法逆元（`a^-1 (mod p)`），它被定义为一个数`x`，使得`a * x = 1 (mod p)`。如果`a`和`p`互质（它们的最大公约数为1），则此逆元存在。对于素数`p`，从1到`p-1`的所有数都可逆。

文章随后详细介绍了扩展欧几里得算法（EEA），作为计算乘法逆元的一种实用方法。EEA旨在找到`ax + py = GCD(a, p)`中的`x`和`y`。如果`GCD(a, p) = 1`，那么`x`就是`a (mod p)`的乘法逆元。文章通过一个例子演示了通过重复减法和回代法查找逆元的逐步过程。文章最后暗示了该算法的效率，并将其与斐波那契数列联系起来。

---

## 65. Bootloader 解锁耻辱墙

**原文标题**: Bootloader Unlock Wall of Shame

**原文链接**: [https://github.com/zenfyrdev/bootloader-unlock-wall-of-shame](https://github.com/zenfyrdev/bootloader-unlock-wall-of-shame)

本文《引导加载程序解锁耻辱墙》旨在收录并追踪那些限制用户在其设备上解锁引导加载程序的公司，这些公司将其行为包装成对“数据安全”的关注，实则限制了用户控制权。作者认为，此举开创了一个危险的先例，可能影响Shizuku或ADB等其他工具。

该列表根据制造商的引导加载程序解锁政策进行分类：

*   **“简直糟透了！🍅”**：像阿尔卡特、亚马逊、苹果、三星、华为和Vivo/IQOO等公司，在没有变通方法的情况下，使设备解锁“完全不可能”。运营商锁定的设备通常也属于此类别，即使在运营商锁解除后，也往往阻止解锁。
*   **“务必避开！⛔”**：像海信、HMD/诺基亚、荣耀、摩托罗拉/联想、OPPO/真我以及小米/红米/POCO等制造商，仅在特定条件（例如区域、型号、SOC）下才允许解锁，或要求用户做出“牺牲”。
*   **“谨慎行事！⚠️”**：像Fairphone、谷歌/Nexus、一加和索尼等公司，在允许解锁之前要求提供在线账户和/或等待期。
*   **“暂时安全ℹ️”**：包括Blackview、Cubot、微软、Nothing、Shift和Volla在内的一组公司，它们在引导加载程序解锁方面通常更为宽松。

文章强调，用户不应信任任何公司，除非其解锁过程是100%离线的。它还提供了其他信息，包括对自定义Android验证启动（AVB）密钥的罕见支持，并概述了针对麒麟、联发科、高通和紫光展锐等芯片组的通用基于SOC的解锁方法。

---

## 66. 纳米香蕉AI生成字体

**原文标题**: AI generated font using Nano Banana

**原文链接**: [https://constanttime.notion.site/Worlds-first-Ai-generated-font-using-nano-banana-2ba6f8e15af18012864bdb760fa9c9ba?pvs=74](https://constanttime.notion.site/Worlds-first-Ai-generated-font-using-nano-banana-2ba6f8e15af18012864bdb760fa9c9ba?pvs=74)

提供的输入包含一个标题，“AI generated font using Nano Banana”，这表明这是一篇关于使用人工智能创建字体，可能涉及名为“Nano Banana”的工具或方法的文章。

然而，文章的实际内容并未提供。相反，提供的文本是一个通用的系统消息：“NotionJavaScript must be enabled in order to use Notion.Please enable JavaScript to continue.”

因此，无法提供一篇关于使用Nano Banana生成AI字体文章的摘要，因为文章内容本身缺失。提供的文本仅指明了平台Notion的技术要求，而非与文章暗示主题相关的信息。

---

## 67. 苹果不让我加入开发者计划，也不说明原因

**原文标题**: Apple will not let me join the Developer Program – and will not say why

**原文链接**: [https://blog.kulman.sk/apple-developer-program/](https://blog.kulman.sk/apple-developer-program/)

作者是一位资深开发者，拥有在 Windows Phone 上发布独立应用的经验，他寻求发布自己的第一个个人 iOS 项目。在经历了十年的专业 iOS 开发后，他构思了一款名为 Yomu 的应用，旨在通过根据用户的 JLPT（日本语能力测试）等级，自适应地隐藏汉字的假名，来帮助日语学习者。该应用还包括文本分享、扫描功能、离线词典和词汇导出，目前已完全构建、测试完毕，并准备提交。

然而，当试图加入 Apple 开发者计划时，作者被悄无声息地拒绝了。在联系 Apple 支持后，他被明确告知无法加入，苹果不会透露原因，并且他对此也无能为力。这一官方回复没有提供任何纠正、核实或申诉的途径，并将拒绝归因于一个无法解释的内部自动化系统。

对这种武断的永久禁令感到沮丧，拥有完成的应用和十年经验的作者提出了正式的 GDPR（通用数据保护条例）请求。他要求苹果提供与该自动化决策相关的数据，并根据《通用数据保护条例》第 22 条进行人工审核。苹果回复了一封模板邮件，完全无视了 GDPR 请求，并将他重新导向了毫无帮助的开发者支持。作者得出结论，认为他实际上已被苹果不透明的系统禁止以个人身份发布应用，既没有理由，也无从申诉。

---

## 68. 自闭症不应被当作单一病症。

**原文标题**: Autism should not be treated as a single condition

**原文链接**: [https://www.economist.com/science-and-technology/2025/12/03/why-autism-should-not-be-treated-as-a-single-condition](https://www.economist.com/science-and-technology/2025/12/03/why-autism-should-not-be-treated-as-a-single-condition)

无法访问文章链接

---

## 69. 函数式四叉树

**原文标题**: Functional Quadtrees

**原文链接**: [https://lbjgruppen.com/en/posts/functional-quadtree-clojure](https://lbjgruppen.com/en/posts/functional-quadtree-clojure)

本文介绍了Clojure中的函数式四叉树，旨在为常见的命令式方法提供一种声明式的替代方案。四叉树是一种空间数据结构，通过在感兴趣的区域（例如，摄像机或鼠标位置附近）渲染更高细节并在更远的地方渲染更低细节，从而优化资源分配。

函数式实现根据“摄像机”位置重建整个树，避免了与命令式方法相关的维护工作。每个树节点都是一个简单的映射，存储其边界、中心和宽度。将节点分成四个子节点的决定取决于摄像机是否“过于接近”节点的中心（距离小于节点的宽度），以及节点的宽度是否超过最小尺寸。Clojure的`prewalk`函数有效地处理这种递归拆分。

为了可视化，文章描述了在HTML canvas上绘制四叉树。为了确保节点着色的一致性，从每个节点的中心坐标生成一个32位哈希值，并将其转换为十六进制颜色。

总之，四叉树通过自适应地调整细节，对于优化VR等资源密集型应用程序非常强大。Clojurescript支持简洁的函数式代码（核心逻辑大约25行），使其更易于理解和调试，而Shadow-cljs简化了开发和部署到浏览器的过程。

---

## 70. 原生CSS就够了

**原文标题**: Vanilla CSS is all you need

**原文链接**: [https://www.zolkos.com/2025/12/03/vanilla-css-is-all-you-need](https://www.zolkos.com/2025/12/03/vanilla-css-is-all-you-need)

本文重点介绍了 37signals 如何仅使用原生 CSS（不依赖 Sass 或 PostCSS 等构建工具）成功构建像 Campfire、Writebook 和 Fizzy 这样的复杂网络应用。这挑战了当前依赖复杂工具链或像 Tailwind 这样的工具优先框架的现代趋势。

他们通过巧妙利用现代原生 CSS 特性实现这一点，例如变量、嵌套、容器查询、`:has()` 选择器、CSS 层和 `color-mix()`。他们的架构“极其简单”：一个扁平的文件结构，实现了零配置和零构建时间。

关键模式包括使用 OKLCH 构建感知上均匀的色彩系统、`color-mix()` 用于动态调色板，以及 `ch` 单位用于内容驱动的间距和响应式设计。实用工具类是增量的，而非基础性的，这确保了 HTML 的可读性和集中的设计控制。`:has()` 选择器具有变革性，它实现了以前需要 JavaScript 才能实现的父元素选择和状态管理。

作者详细介绍了 37signals 如何逐步采用 `@starting-style` 等特性实现对话框动画，并使用 CSS 遮罩实现纯 CSS 加载动画，这展示了持续的改进。文章最后敦促开发者重新审视复杂构建工具的必要性，认为现代原生 CSS 已足够强大，足以构建复杂的应用，而且更简单的方法可能更优越。

---

## 71. 诅咒电路：充电泵电压减半器

**原文标题**: Cursed circuits: charge pump voltage halver

**原文链接**: [https://lcamtuf.substack.com/p/cursed-circuits-charge-pump-voltage](https://lcamtuf.substack.com/p/cursed-circuits-charge-pump-voltage)

本文介绍了一种“被诅咒的电路”：电荷泵电压减半器。作者将“被诅咒的电路”定义为那些简单、有用，但本质上有缺陷或效率低下，却仍然引人入胜的电路。这种特定电路旨在将输入电压减半，例如将5V变为2.5V，这是一种模拟电路偏置中常用的功能。

该电压减半器由几个简单的元件构成：两个电容器和两个二极管，通常还会增加两个电阻，用于泄放电荷和设置参考点。它的工作原理依赖于电荷泵效应。当施加输入电压（V_in）时，第一个电容器充电。随后，随着输入电压的变化或通过后续周期（如果是交流耦合），这些电荷被有效地转移并分配到电容器上，从而产生一个大约是输入电压一半的输出电压。

“被诅咒”之处在于其实用性。尽管理论上很简单，但其输出电压并不完全稳定，会随负载和输入变化而波动。它存在稳压不良的问题，这意味着即使在轻负载下，输出电压也会显著下降。它效率也低，因为二极管和电容器存在损耗，并且输出阻抗相当高，这使得它不适用于需要稳定、受控电源的应用。尽管有这些缺点，作者发现它因其优雅的简洁性和以极简设计展示基本电学原理的方式而令人着迷。

---

## 72. HN 展示：极简月度任务规划器（可打印，离线，免注册）

**原文标题**: Show HN: A Minimal Monthly Task Planner (printable, offline, no signup)

**原文链接**: [https://printcalendar.top/](https://printcalendar.top/)

本文介绍了来自 PrintCalendar.top 的“极简月度任务规划器”，它作为一个“Show HN”项目展示。该规划器被描述为一个宁静、方便打印的在线画布，旨在规划月度任务、记录笔记并维护重要信息的轻量级日志。

主要特点包括其极简设计，以及查看和导航月份（例如2026年1月）的功能，并可选择将周的起始日设置为周一或周日。用户可以“停留在当前月份”、“跳转到今天”，以及分享特定月份的链接。一个值得注意的特点是包含了支持内联编辑的月度笔记，这些笔记保存在用户浏览器本地，确保了隐私和离线访问。

该规划器针对打印进行了优化，提供简洁的A4布局、深色/浅色主题以及一键打印或保存为PDF的选项。它强调用户隐私和便利性，无需“登录”，“离线友好”，并且无需注册，即可“永久拥有”。

---

## 73. 诗歌提示词注入

**原文标题**: Prompt Injection via Poetry

**原文链接**: [https://www.wired.com/story/poems-can-trick-ai-into-helping-you-make-a-nuclear-weapon/](https://www.wired.com/story/poems-can-trick-ai-into-helping-you-make-a-nuclear-weapon/)

Icaro Lab的一项新研究揭示了大型语言模型（LLM）的一个关键漏洞：以诗歌形式提出危险问题可以绕过它们的安全防护栏。研究人员发现，这种“对抗性诗歌”使得OpenAI、Meta和Anthropic的聊天机器人能够讨论核武器和恶意软件等话题，手工制作的诗歌在25个测试模型中实现了平均62%的越狱成功率。

这种方法与其他的“对抗性后缀”或复杂的行话类似，它们都会迷惑AI安全系统。Icaro Lab认为，诗歌的“高温”语言——其特点是不可预测的词序、隐喻和碎片化语法——利用了LLM先进的解释能力与其防护栏脆弱性之间的不匹配。

研究人员解释说，尽管人类能识别诗歌中“炸弹”的隐喻指的是同一个危险物体，但对于人工智能而言，这种诗意的措辞会导致它通过系统性地避开通常触发安全警报的区域的路径，来导航其内部多维概念图。本质上，这种风格上的变化阻止了安全机制识别有害意图。

由于易于创建和滥用的可能性，研究人员没有提供越狱诗歌的具体例子，只提供了一个净化版本。这一发现凸显了当前LLM安全机制的一个重大缺陷，使其容易受到复杂的文体操纵。

---

## 74. Proxmox 数据中心管理器 1.0 发布

**原文标题**: Proxmox Datacenter Manager 1.0 available

**原文链接**: [https://www.proxmox.com/en/about/company-details/press-releases/proxmox-datacenter-manager-1-0](https://www.proxmox.com/en/about/company-details/press-releases/proxmox-datacenter-manager-1-0)

Proxmox Server Solutions GmbH 于2025年12月4日宣布立即推出 Proxmox 数据中心管理器 1.0。这款全新的企业级软件产品旨在解决运营大规模、分布式 Proxmox 环境日益增长的复杂性。

Proxmox 数据中心管理器提供“统一视图”，用于对 Proxmox VE 和 Proxmox Backup Server 进行全面的管理、监控和扩展。其主要目标是为管理员提供对其基础设施全面且无缝的控制。该软件被开发为一项战略解决方案，以应对管理不断增长的数据中心所面临的挑战，例如缺乏全局概览、分散的指标以及在各种环境中进行手动操作的需求，这可能导致效率低下和错误。

通过弥合单个基于 Proxmox 的节点和集群之间的鸿沟，数据中心管理器统一了整个基础设施视图，简化了日常任务，并实现了以前难以实现的高级功能。

---

## 75. 为什么苹果不做独立式Touch ID？

**原文标题**: Why doesn't Apple make a standalone Touch ID?

**原文链接**: [https://www.jeffgeerling.com/blog/2025/why-doesnt-apple-make-standalone-touch-id](https://www.jeffgeerling.com/blog/2025/why-doesnt-apple-make-standalone-touch-id)

作者升级到机械键盘后，抱怨缺少集成式触控ID，这一功能对macOS登录、密码管理器和Apple Pay至关重要。作为一种变通方法，他们详细介绍了一个“浪费的”改装：拆解一个带触控ID的Apple妙控键盘，取出其传感器和逻辑板，然后将它们安装在一个定制的3D打印外壳中。这一过程灵感来源于Snazzy Labs的一个视频，并在他们自己的“Level 2 Jeff”视频中进行了展示。

拆解过程非常艰巨，因为苹果大量使用了粘合剂和精密部件。作者强调了诸如加热后盖、小心翼翼地取出电池以及处理脆弱的柔性PCB排线等挑战。对其他尝试此操作的人的建议包括：对粘合剂使用热量，用弯头镊子处理小部件，对触控ID柔性PCB要极其小心，为背板设置精确的3D打印参数，以及在组装时耐心处理微小的M1.2螺丝。

提出的核心问题是，为什么苹果不提供一个独立的触控ID设备。作者认为，许多用户会乐意为这样一个产品支付约50美元，从而避免了为这个DIY解决方案牺牲一个150美元的键盘和数小时的时间。文章评论区反映了类似的情绪，有人认为苹果的犹豫是由于不希望用户使用非苹果键盘，而另一个人则指出许多Mac用户已经在使用第三方键盘。

---

## 76. 家猫对男性照护者的问候发声更频繁

**原文标题**: Greeting Vocalizations in Domestic Cats Are More Frequent with Male Caregivers

**原文链接**: [https://onlinelibrary.wiley.com/doi/10.1111/eth.70033](https://onlinelibrary.wiley.com/doi/10.1111/eth.70033)

这篇文章，题为《家猫对男性看护者发出更多问候叫声》，探讨了影响家猫如何以及何时向人类看护者问候的因素。

该研究观察了来自20个不同家庭的36只猫，记录了看护者在离开一段时间后返回时它们发出的叫声（咕噜声、喵叫声和颤音）。研究人员分析了超过700次问候事件，并考虑了猫的个性、看护者的性别以及看护者离开的时间长短。

主要研究结果显示，与问候女性看护者相比，猫在问候男性看护者时发出的叫声更多。具体而言，对男性看护者发出咕噜声的频率显著更高，且叫声的总持续时间也更长。尽管看护者离开的时间长短并未显著影响叫声频率，但猫的个体性格特征，如“活跃度/玩耍性”和“神经质”，确实与它们发出叫声的频率相关，这表明更活泼和焦虑的猫可能会叫得更多。

该研究总结指出，看护者的性别在家猫的问候行为中扮演着重要角色，这可能归因于人猫互动方式的差异或人类声音的声学特性。这些发现有助于我们理解家猫与其人类伴侣之间复杂的交流动态。

---

## 77. 为什么38%的斯坦福学生声称自己残疾？

**原文标题**: Why are 38 percent of Stanford students saying they're disabled?

**原文链接**: [https://reason.com/2025/12/04/why-are-38-percent-of-stanford-students-saying-theyre-disabled/](https://reason.com/2025/12/04/why-are-38-percent-of-stanford-students-saying-theyre-disabled/)

本文探讨了精英大学中声称残疾的学生人数惊人增长的现象，斯坦福大学报告称，这一比例高达“令人恼火的”38%，其中大部分是为了获得学业便利，理由是焦虑症、抑郁症和多动症等心理健康问题。作者质疑其真实性，指出真正的学习障碍学生不太可能进入这类竞争激烈的大学，这一观点也得到了教授们的支持，他们认为这不过是“富家子弟获得额外时间”的手段。这与特殊照顾申请率远低于此的社区大学形成了鲜明对比。

驱动这一趋势的因素有几个：《美国残疾人法案》（ADA）允许在极少文件证明的情况下提供广泛的学业便利；疾病日益被视为身份认同的标志；以及在线平台（如TikTok）对症状的宽泛定义，这导致学生将正常的学习困难解读为可诊断的疾病。《精神疾病诊断与统计手册》（DSM）对多动症等疾病的诊断标准降低，也进一步助长了这一趋势。

一个重要因素是精英学生中的风险规避心态，他们因害怕失败，会将正常的学业困难或不适病态化。他们利用学业便利作为避免成绩不佳和自我怀疑的保障。作者总结说，这些不必要的学业便利是一种“双重作弊”：它既赋予了不公平的优势，又阻碍了学生真正的智力成长和关键成人应对技能的发展。

---

## 78. JetBrains 智能体开发环境

**原文标题**: Agentic Development Environment by JetBrains

**原文链接**: [https://air.dev](https://air.dev)

JetBrains 正在推出“Air”，一个创新的“智能体开发环境”。这个新平台旨在通过将AI智能体直接集成到开发过程中，彻底改变编码工作流。

Air 的核心承诺是让开发者能够“利用智能体进行多任务处理”，这表明AI将承担各种任务，从而实现更高效、并行地执行开发活动。至关重要的是，JetBrains 强调这种新范式将使开发者能够“保持掌控”。这确保了尽管AI智能体提供强大的协助和自动化，人类开发者仍然保留最终的监督权、决策权以及对项目的清晰理解，从而营造一个协作而非纯粹自主的环境。Air 旨在增强开发者的能力，简化工作流，同时让人类保持主导地位。

---

## 79. 发送 DMARC 报告存在一定风险

**原文标题**: Sending DMARC reports is somewhat hazardous

**原文链接**: [https://utcc.utoronto.ca/~cks/space/blog/spam/DMARCSendingReportsProblems](https://utcc.utoronto.ca/~cks/space/blog/spam/DMARCSendingReportsProblems)

本页面显示您已被阻止访问Chris Siebenmann的博客“漫想随笔”（Wandering Thoughts）或其关联维基CSpace。该阻止由反爬虫措施执行，这些措施将您的浏览器版本标记为可疑，通常是因为其版本过旧（尤其常见于较旧的Chrome版本）。

截至2025年初，大量爬虫显著增加，这些爬虫被认为正在为大型语言模型（LLM）训练收集数据，并且通常使用过时的浏览器用户代理。为减轻其系统负载，Siebenmann正在试验性地阻止这些爬虫，而您的浏览器已被此措施捕获。

如果您认为这是一个错误，并且您正在使用最新浏览器，建议您通过Chris Siebenmann的大学邮箱地址联系他。联系时，请提供您浏览器的详细信息，包括其精确的用户代理（User-Agent）字符串。

一则特别说明针对通过`archive.*`服务（如archive.today或archive.ph）访问本站的用户。这些服务也被阻止，因为它们的爬取行为——使用旧的Chrome用户代理、从广泛分布且经常伪装的IP地址（有些甚至谎称是googlebot）进行操作——与恶意行为者的行为无法区分。Siebenmann建议使用`archive.org`，作为一个更可靠的存档爬虫，它可以访问他的博客。

---

## 80. 在 Rails 中构建乐观 UI (兼学自定义元素)

**原文标题**: Building optimistic UI in Rails (and learn custom elements)

**原文链接**: [https://railsdesigner.com/custom-elements/](https://railsdesigner.com/custom-elements/)

本文介绍了自定义元素，这是一项基础的Web平台功能，已被Hotwire（例如`<turbo-frame>`和`<turbo-stream>`）所使用。自定义元素允许开发者定义具有自定义JavaScript行为的新HTML标签，是Web Components的一部分。它们通过在类中扩展`HTMLElement`并使用`customElements.define()`进行注册来创建。`connectedCallback()`方法负责初始化，类似于Stimulus的`connect()`。可以使用`getAttribute()`、`observedAttributes`和`attributeChangedCallback()`来读取和监控属性。虽然自定义元素可以通过`is`属性扩展内置HTML元素，但为了更好的浏览器兼容性，建议使用自主（带连字符的）自定义元素。

将自定义元素与Stimulus进行比较，文章强调了自定义元素的浏览器原生特性、直接的DOM操作（而非Stimulus的`targets`），以及它们在构建可复用、自包含组件方面的适用性。相反，Stimulus则擅长为现有HTML添加行为。

核心演示涉及构建一个“乐观表单”。该表单无需等待服务器响应即可提供即时UI反馈。提交时，`optimistic-form`元素会克隆一个嵌入的`<template response>`，用表单数据填充它，并立即将其添加到显示中（例如，消息列表）。该表单同时提交到Rails。在收到成功的服务器响应后，Turbo Stream的`replace`动作会用实际的服务器生成内容更新乐观渲染的元素（由一个临时ID标识）。这项技术提供了无缝的用户体验，消除了加载指示器，并确保了聊天消息、评论或待办事项等功能的即时更新，同时将UI局部内容定义在HTML模板内。

---

## 81. 卫星首次拍到巨型海啸全貌

**原文标题**: Satellite captures the first detailed look at a giant tsunami

**原文链接**: [https://www.earth.com/news/satellite-captures-the-first-detailed-look-at-a-giant-tsunami/](https://www.earth.com/news/satellite-captures-the-first-detailed-look-at-a-giant-tsunami/)

2025年7月29日，千岛-堪察加海沟区域发生8.8级地震，引发了一场太平洋范围的海啸，提供了一次独特的自然实验。美国宇航局（NASA）和法国国家空间研究中心（CNES）的SWOT卫星首次获取了这次大型俯冲带海啸的高分辨率星载带状观测数据，提供了前所未有的视角。

卫星图像显示，海啸能量并非以单一、整齐的波峰形式传播，而是在数百英里范围内呈现出复杂、交织的弥散和散射模式。这直接挑战了传统观念，即大型跨洋海啸以“非弥散”波包形式传播的假设。这些发现表明，当前海啸灾害预报的物理模型需要修正，以考虑这些弥散效应，因为它们会显著影响波能量的传播方式，从而改变海啸登陆时间和对沿海结构物的冲击力。

与稀疏的DART浮标或以往的卫星不同，SWOT卫星能绘制75英里宽的海面高度带状图，使科学家能够观察海啸在空间和时间上的几何演变。这些数据结合DART记录、地震信息和大地测量形变数据，还修正了对地震破裂的理解，使其比最初模型预测的向南延伸更远，从而得到了更准确的认识。

这项研究强调了三个关键点：高分辨率卫星测高技术可以揭示大洋中部海啸的内部结构；即使是大型海啸，弥散也是能量传播方式的一个重要因素；整合多种数据类型（卫星、DART、地震、大地测量）对于建立准确的震源和演化模型至关重要。这项研究标志着一个转折点，敦促建模人员和规划者更新预报系统，以更好地反映新揭示的海啸复杂性，从而做出更精准的预测。该研究发表在《地震记录》（The Seismic Record）期刊上。

---

## 82. 对抗年龄门槛网络

**原文标题**: Fighting the age-gated internet

**原文链接**: [https://www.wired.com/story/age-verification-is-sweeping-the-us-activists-are-fighting-back/](https://www.wired.com/story/age-verification-is-sweeping-the-us-activists-are-fighting-back/)

国会议员目前正在审议19项网络安全法案，其中包括《儿童网络安全法案》（KOSA），因为年龄验证法案正在美国一半的州和全球范围内迅速蔓延。数字权利组织“为未来而战”（Fight for the Future）正积极反对这些提案，认为它们将开创一个危险先例，使互联网更具剥削性而非更安全。

许多拟议法案强制要求身份或年龄验证，要求用户上传身份证件或进行面部扫描才能访问特定内容。“为未来而战”警告称，这将导致普遍的审查制度、更严密的监控，并通过第三方验证服务增加数据泄露的风险。倡导者莎拉·菲利普斯（Sarah Philips）认为这些法律直接威胁民主自由，将其比作禁书和对敏感信息的限制。

美国25个州、英国和澳大利亚已经实施或强制要求某种形式的在线年龄验证，澳大利亚的青少年社交媒体禁令将于12月生效。超过90个人权倡导团体签署了一封联合信，反对在线身份验证指令，声明这些指令将用户视为“犯罪嫌疑人”，未能解决大型科技公司的全面隐私和反垄断等核心问题。

菲利普斯批评国会未能为“监控资本主义商业模式”提供真正的解决方案，反而专注于验证。她强调年龄验证影响的是*所有人*，而不仅仅是未成年人。如果实施，所有互联网用户，无论年龄大小，都将被迫证明自己不是儿童才能访问受年龄限制的互联网，从而从根本上改变所有人的在线访问和隐私。

---

## 83. Codeberg is down

**原文标题**: Codeberg is down

**原文链接**: [https://status.codeberg.org/status/codeberg](https://status.codeberg.org/status/codeberg)

生成摘要时出错

---

## 84. React 服务器组件严重安全漏洞

**原文标题**: Critical Security Vulnerability in React Server Components

**原文链接**: [https://react.dev/blog/2025/12/03/critical-security-vulnerability-in-react-server-components](https://react.dev/blog/2025/12/03/critical-security-vulnerability-in-react-server-components)

生成摘要时出错

---

## 85. Russia Bans Roblox

**原文标题**: Russia Bans Roblox

**原文链接**: [https://www.bbc.com/news/articles/cn41q11gy58o](https://www.bbc.com/news/articles/cn41q11gy58o)

生成摘要时出错

---

## 86. Apple’s head of user interface design, Alan Dye, will join Meta

**原文标题**: Apple’s head of user interface design, Alan Dye, will join Meta

**原文链接**: [https://www.cnbc.com/2025/12/03/liquid-glass-alan-dye-leaving-apple.html](https://www.cnbc.com/2025/12/03/liquid-glass-alan-dye-leaving-apple.html)

Apple's head of user interface design, Alan Dye, is leaving the company to join Meta, marking a significant executive shift in Silicon Valley. Dye, who succeeded Jony Ive in 2015, was responsible for the recent "Liquid Glass" software redesign across iPhones, Macs, and Apple Watch, and played a key role in the iPhone's transition away from the physical home button.

At Meta, Dye will lead a new creative studio focused on design, fashion, and technology, with CEO Mark Zuckerberg emphasizing an elevation of design within the company. This move comes as Meta intensifies its hardware development, including its Quest virtual reality headsets and the successful Ray-Ban Meta smart glasses, positioning itself as a major competitor to Apple.

Apple confirmed Dye's departure, with CEO Tim Cook announcing that veteran designer Stephen Lemay, who has contributed to every major Apple interface since 1999, will succeed him. The departure highlights the ongoing talent movement between tech giants and Meta's strategic push into hardware design.

---

## 87. After nearly 30 years, Crucial will stop selling RAM to consumers

**原文标题**: After nearly 30 years, Crucial will stop selling RAM to consumers

**原文链接**: [https://arstechnica.com/gadgets/2025/12/after-nearly-30-years-crucial-will-stop-selling-ram-to-consumers/](https://arstechnica.com/gadgets/2025/12/after-nearly-30-years-crucial-will-stop-selling-ram-to-consumers/)

生成摘要时出错

---

## 88. The only winning move is not to play

**原文标题**: The only winning move is not to play

**原文链接**: [https://gregg.io/the-only-winning-move](https://gregg.io/the-only-winning-move)

生成摘要时出错

---

## 89. Multivox: Volumetric Display

**原文标题**: Multivox: Volumetric Display

**原文链接**: [https://github.com/AncientJames/multivox](https://github.com/AncientJames/multivox)

生成摘要时出错

---

## 90. In defense of lock poisoning in Rust

**原文标题**: In defense of lock poisoning in Rust

**原文链接**: [https://sunshowers.io/posts/on-poisoning/](https://sunshowers.io/posts/on-poisoning/)

生成摘要时出错

---

## 91. Show HN: Onlyrecipe 2.0 – I added all features HN requested – 4 years later

**原文标题**: Show HN: Onlyrecipe 2.0 – I added all features HN requested – 4 years later

**原文链接**: [https://onlyrecipeapp.com/?url=https://www.allrecipes.com/turkish-pasta-recipe-8754903](https://onlyrecipeapp.com/?url=https://www.allrecipes.com/turkish-pasta-recipe-8754903)

生成摘要时出错

---

## 92. We're committing $6.25B to give 25M children a financial head start

**原文标题**: We're committing $6.25B to give 25M children a financial head start

**原文链接**: [https://www.onedell.com/investamerica/](https://www.onedell.com/investamerica/)

生成摘要时出错

---

## 93. Stop talking

**原文标题**: Stop talking

**原文链接**: [https://gurkan.in/2025/12/stop-talking/](https://gurkan.in/2025/12/stop-talking/)

生成摘要时出错

---

## 94. Chips for the Rest of Us

**原文标题**: Chips for the Rest of Us

**原文链接**: [https://engineering.nyu.edu/about/unconventional-engineer/chips-for-us](https://engineering.nyu.edu/about/unconventional-engineer/chips-for-us)

生成摘要时出错

---

## 95. Formally verifying Advent of Code using Dijkstra's program construction

**原文标题**: Formally verifying Advent of Code using Dijkstra's program construction

**原文链接**: [https://haripm.com/blog/aoc-day-3-without-thinking/](https://haripm.com/blog/aoc-day-3-without-thinking/)

生成摘要时出错

---

## 96. Exploring Large HTML Documents on the Web

**原文标题**: Exploring Large HTML Documents on the Web

**原文链接**: [https://calendar.perfplanet.com/2025/exploring-large-html-documents-on-the-web/](https://calendar.perfplanet.com/2025/exploring-large-html-documents-on-the-web/)

生成摘要时出错

---

## 97. Palantir CEO Says Making War Crimes Constitutional Would Be Good for Business

**原文标题**: Palantir CEO Says Making War Crimes Constitutional Would Be Good for Business

**原文链接**: [https://gizmodo.com/palantir-ceo-says-making-war-crimes-constitutional-would-be-good-for-business-2000695162](https://gizmodo.com/palantir-ceo-says-making-war-crimes-constitutional-would-be-good-for-business-2000695162)

生成摘要时出错

---

## 98. Apple Design Official Alan Dye Poached by Meta in Major Coup

**原文标题**: Apple Design Official Alan Dye Poached by Meta in Major Coup

**原文链接**: [https://www.bloomberg.com/news/articles/2025-12-03/apple-design-executive-alan-dye-poached-by-meta-in-major-coup](https://www.bloomberg.com/news/articles/2025-12-03/apple-design-executive-alan-dye-poached-by-meta-in-major-coup)

生成摘要时出错

---

## 99. Micron to exit consumer memory business amid global supply shortage

**原文标题**: Micron to exit consumer memory business amid global supply shortage

**原文链接**: [https://www.reuters.com/business/micron-exit-crucial-consumer-memory-business-2025-12-03/](https://www.reuters.com/business/micron-exit-crucial-consumer-memory-business-2025-12-03/)

生成摘要时出错

---

## 100. We Built an AI-Agent to Debug 1000s of Databases – and Cut Incident Time by 90%

**原文标题**: We Built an AI-Agent to Debug 1000s of Databases – and Cut Incident Time by 90%

**原文链接**: [https://www.databricks.com/blog/how-we-debug-1000s-databases-ai-databricks](https://www.databricks.com/blog/how-we-debug-1000s-databases-ai-databricks)

生成摘要时出错

---

