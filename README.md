# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2025-12-04.md)

*最后自动更新时间: 2025-12-04 20:12:35*
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

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 2 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 3 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 4 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 5 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 6 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 7 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 8 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 9 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 10 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 11 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 12 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 13 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 14 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 15 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 16 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 17 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 18 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 19 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 20 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 21 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 22 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 23 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 24 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 25 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 26 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 27 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
| 28 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 29 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
