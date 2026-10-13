# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-10-13.md)

*最后自动更新时间: 2026-10-13 01:39:03*
## 1. 通行密钥是个陷阱

**原文标题**: Passkeys are a trap

**原文链接**: [https://nonfunctional.substack.com/p/passkeys-are-a-trap-do-not-use-them](https://nonfunctional.substack.com/p/passkeys-are-a-trap-do-not-use-them)

《“通行密钥是个陷阱”》摘要

nonfunctional.substack.com 网站上题为《通行密钥是个陷阱》的文章强烈反对采用通行密钥，认为它们带来的巨大风险远超其宣称的益处。作者认为，通行密钥尽管被吹捧为“密码杀手”，却引入了一系列新的关键问题，主要集中在厂商锁定、账户恢复困难以及可能导致大量账户丢失。

核心批评包括：
1.  **厂商锁定：** 通行密钥通常与特定的操作系统（iOS、安卓、Windows）或浏览器绑定，造成了生态系统依赖。在不同生态系统（例如从iPhone转向安卓）之间迁移时，访问受通行密钥保护的账户会变得困难甚至不可能，迫使用户管理多个互不关联的通行密钥存储。
2.  **恢复困难：** 与可以通过电子邮件或手机重置的密码不同，通行密钥的恢复机制通常与设备备份和云账户（即Apple ID、Google账户）绑定。失去对这些主账户或设备的访问权限，可能导致永久性地丢失对所有关联服务的访问。
3.  **大量账户丢失：** 作者警告说，如果用户的核心云账户（例如Apple ID）遭到泄露，攻击者就可以获得所有关联通行密钥的访问权限，从而导致大量账户同时被盗——这相当于一次“加强版”的大规模网络钓鱼事件。
4.  **互操作性有限：** 尽管存在标准（FIDO联盟），但科技巨头在实施时常会导致专有变体，阻碍了真正的跨平台功能。
5.  **并非网络钓鱼的万能药：** 作者认为，通行密钥并非能从根本上解决所有用户的网络钓鱼问题，因为社会工程学攻击或底层云账户被攻破仍然是重大威胁。

文章最后建议用户避免使用通行密钥，并坚持使用传统的密码管理器和多因素认证（MFA），因为它们提供了更大的控制权和更好的恢复选项。

---

## 2. 指纹是新的Cookie

**原文标题**: Fingerprints are the new cookies

**原文链接**: [https://royfish.dev/fingerprints-are-the-new-cookies](https://royfish.dev/fingerprints-are-the-new-cookies)

文章《指纹是新的Cookie》指出，设备指纹已取代第三方Cookie，成为一种普遍且更持久的在线追踪方法。

文章解释说，指纹识别通过收集浏览器和设备的众多数据点来工作，其中包括网络请求详情（浏览器、操作系统、语言、IP）以及代码环境测量值（GPU、CPU、内存、显示器、音频处理、已安装字体、扩展程序）。单独来看，这些细节可能很常见，但结合起来，它们就创建了一个高度独特的“指纹”，足以识别用户，即便跨越会话、设备变更，或在清除Cookie/使用VPN之后。这类似于“信息熵”，每条信息都缩小了可能的身份池，最终识别出个人。

作者批评谷歌在隐私担忧和反垄断审查之际，表面上摆脱第三方Cookie，却在其广告产品中转而拥抱设备指纹识别。这使得公司能够为用户建立全面的档案，这些档案可以出售给出价最高者，包括政府，从而导致社会进入一种“数字分形状态”，远远超出了简单的广告定位。

虽然禁用JavaScript的用户可以免受某些方法的侵害，但大多数浏览器（Chrome、Edge）几乎不提供任何指纹识别防御。Safari和Firefox提供了一些，但Brave、Tor和Mullvad浏览器被强调为唯一提供强大内置保护的主要浏览器，它们通过“模糊化”（添加噪音）或让所有用户看起来都一样来实现。隐私扩展程序因可能使用户更独特或破坏网站功能而被指出效果不佳。

文章最后详细介绍了在其自身页面上使用的具体指纹识别方法作为例子，例如`OfflineAudioContext`、`WebGL`、`Canvas`、`Intl`（时区/区域设置）和`Navigator`（CPU/内存），所有这些数据都被哈希处理，以生成一个持久的昵称。

---

## 3. 大语言模型能力认知共识的差距正在扩大。

**原文标题**: The gap in shared understanding of LLM capability is widening

**原文链接**: [https://twitter.com/karpathy/status/2109361546505966046](https://twitter.com/karpathy/status/2109361546505966046)

Andrej Karpathy 认为，人们对 LLM 能力的普遍认知正迅速演变成一个“尖锐的漏斗”。

绝大多数人（60 亿）从未接触过 LLM。另有 1-20 亿是随意、免费使用的用户，他们认为 LLM 是“笨笨的”聊天机器人，只能用于搜索或写作等基本任务，作用不大。许多非技术专业人士属于这一类。

一个更小的群体，约 2000 万专业人士（占 0.2%），主要集中在数学和编码领域，他们正在使用前沿 LLM，并体验着复杂的项目。这些项目过去需要数周或数月才能完成，现在却能通过智能体的单个提示词完成——这与一年前的手动编码相比，是一个巨大的转变。

最顶端的极小部分，仅 5000 人（占 0.00006%），他们拥有尖端系统的内部访问权限。他们观察到大量的智能体协同合作，进行“软件巨型项目”——在数周内发现零日漏洞、发动网络攻击，或推动科学和数学进步。这些任务如果由顶尖专家来完成，则需要数年。人类理解能力已经跟不上这种速度了。

这种不断扩大的差距是由三个因素驱动的：1) 影响力随抱负和问题规模而扩大；2) LLM 能力的“参差不齐”，由于强化学习，它在数字化、可验证和具有经济价值的领域表现出色；3) 不同的访问权限（免费、付费、内部）。这创造了一个独特的时刻，即普通大众、大多数专业人士和一小部分精英同时体验着 LLM 能力截然不同的现实。

---

## 4. 横扫千军，为现代电脑重制

**原文标题**: Total Annihilation, rebuilt for modern computers

**原文链接**: [https://nanolathe.gg](https://nanolathe.gg)

本文宣布，经典即时战略游戏《横扫千军》将进行现代化重制，专为当代计算机系统设计。一个主要的改进是显著提升的视觉保真度和镜头控制，让玩家能够近距离放大观察自己的单位和战场行动。这使得玩家能够更深入地欣赏熟悉的战场，以一个全新且更精细的规模将其呈现。

---

## 5. Yandex机器人流量

**原文标题**: Bot traffic from Yandex

**原文链接**: [https://radar.cloudflare.com/bots/as13238?dateRange=7d](https://radar.cloudflare.com/bots/as13238?dateRange=7d)

Cloudflare Radar针对AS13238（Yandex LLC）的页面提供了过去七天内源自Yandex基础设施的网络流量的详细概览。数据显示，AS13238的绝大部分流量被归类为机器人流量，显著超过了人类生成的流量。

具体而言，“按类别划分的机器人流量”细分数据显示，合法的搜索引擎机器人构成了这种自动化流量的绝大多数，通常占比超过95%。这一高比例是预料之中，并与Yandex作为主要搜索引擎的角色相符，其索引服务需要广泛的网络抓取。

尽管搜索引擎机器人占据主导地位，但分析也识别出其他机器人类别的少量贡献，包括内容聚合器、订阅源抓取器以及各种类型的抓取器。攻击机器人也存在，但仅占源自AS13238的总机器人流量的极小部分。过去七天的数据趋势显示出一致的高机器人流量模式，主要由Yandex合法的搜索引擎操作驱动。

---

## 6. 扬戴克斯云第三数据中心遭打击

**原文标题**: 3rd Yandex Cloud Data Center Was Hit

**原文链接**: [https://status.yandex.cloud/en/incidents/2136](https://status.yandex.cloud/en/incidents/2136)

2024年3月27日，Yandex Cloud 发生了一起编号为 2136 的“某独立可用区网络分段连接问题”事件，严重影响了其 `ru-central1-c` 可用区。此次中断始于世界协调时间 (UTC) 10:48，并于世界协调时间 12:47 完全解决。

该事件由 `ru-central1-c` 可用区内某个特定网络分段的多个网络设备并发故障引发，导致路由问题。这造成在该可用区托管的多种 Yandex Cloud 服务（包括 Managed Databases、Compute Cloud、Managed Service for Kubernetes、Object Storage 等）出现连接问题和不可用。用户报告难以连接到虚拟机 (VM) 和数据库集群、API 错误以及操作失败。

Yandex Cloud 通过逐步将流量从受影响的网络分段重新路由并修复故障设备，解决了该问题。尽管所有服务最终都已恢复，该公司仍对造成的不便表示歉意。

展望未来，Yandex Cloud 计划实施额外的故障隔离和更快的流量重新路由机制，以增强抵御类似设备故障的弹性。他们还重申了对用户的建议，即应将工作负载分布在多个可用区和区域，以防止单可用区中断。

---

## 7. 纽约市的“点击取消”规定现已生效。

**原文标题**: NYC's "Click to Cancel" rule is now in effect

**原文链接**: [https://www.nyc.gov/main/click-to-cancel](https://www.nyc.gov/main/click-to-cancel)

NYC's "Click to Cancel" rule, effective October 1, 2026, aims to protect consumers from difficult subscription cancellations. Mayor Zohran Mamdani states the core principle: if you can sign up with a click, you must be able to cancel with one.

Enforced by the Department of Consumer and Worker Protection (DCWP), the rule combats "subscription traps" by mandating that businesses provide clear terms, disclose consumer rights, and offer a straightforward cancellation process matching the sign-up method. Companies also cannot require payment or return shipping for items initially given for free. Violators face civil penalties starting at $525 and potential consumer refunds.

Consumers can file complaints online or via mail/fax if they experience issues such as unclear terms, forced complex cancellation methods (e.g., online sign-up, phone cancellation), delayed cancellations, or unsolicited products. The DCWP reviews complaints, may request additional information, and can assign a mediator to facilitate a resolution between the consumer and the business. Complaint forms are available in multiple languages.

---

## 8. Deloitte falsified documents to evade tax on Abramovich's wealth

**原文标题**: Deloitte falsified documents to evade tax on Abramovich's wealth

**原文链接**: [https://www.bbc.com/news/articles/c64g1l5389kvo](https://www.bbc.com/news/articles/c64g1l5389kvo)

英国广播公司《广角镜》栏目和调查记者局根据泄露的“塞浦路斯机密”文件联合调查发现，全球最大的会计师事务所德勤被指控伪造文件，帮助罗曼·阿布拉莫维奇（Roman Abramovich）逃避对其数十亿美元财富的纳税。律师安德鲁·米切尔（Andrew Mitchell）御用大律师将这些被揭露的方案描述为“赤裸裸的逃税”。

调查显示，德勤塞浦路斯于2006年批准了阿布拉莫维奇旗下公司Amiscan Investments的账目，使得价值6.72亿美元的资产——包括超级游艇、豪宅和私人飞机——凭空消失。这是通过将这些资产的转移日期追溯到三年前，转移给一家英属维尔京群岛（BVI）的母公司来实现的，以规避新的塞浦路斯透明度法律。尽管明知这些文件具有误导性，德勤仍审查并批准了这些回溯日期的文件。

进一步证据表明，德勤还为阿布拉莫维奇的另一家持有近20亿美元资产的公司Kravin Investments提供了一项方案。为逃避利息税，文件被回溯日期，虚假地显示Kravin只是为一家英属维尔京群岛母公司代持资金，使其在塞浦路斯看起来无需纳税。MeritServus（德勤曾拥有并持续合作的公司）的电子邮件明确讨论了在与德勤会面后更改财务报表。

MeritServus还为Electus Investments回溯了文件日期，使价值100亿美元的财富看起来属于一家同名的英属维尔京群岛公司，从而将其保密。

阿布拉莫维奇的律师否认逃税，称他未参与日常运营，并合法地依赖专业建议。德勤塞浦路斯表示其“遵守适用法律”，但无法就涉及20多年前文件的指控发表评论。

---

## 9. Terence Tao: Math 2.0 [pdf]

**原文标题**: Terence Tao: Math 2.0 [pdf]

**原文链接**: [https://teorth.github.io/tao-web/slides/math-2-0-caltech-2026.pdf](https://teorth.github.io/tao-web/slides/math-2-0-caltech-2026.pdf)

生成摘要时出错

---

## 10. Muse Wonder

**原文标题**: Muse Wonder

**原文链接**: [https://research.meta.ai/blog/muse-wonder](https://research.meta.ai/blog/muse-wonder)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-10-13](output/hacker_news_summary_2026-10-13.md) |
| 2 | [2026-10-10](output/hacker_news_summary_2026-10-10.md) |
| 3 | [2026-10-11](output/hacker_news_summary_2026-10-11.md) |
| 4 | [2026-10-07](output/hacker_news_summary_2026-10-07.md) |
| 5 | [2026-10-01](output/hacker_news_summary_2026-10-01.md) |
| 6 | [2026-10-06](output/hacker_news_summary_2026-10-06.md) |
| 7 | [2026-10-04](output/hacker_news_summary_2026-10-04.md) |
| 8 | [2026-10-02](output/hacker_news_summary_2026-10-02.md) |
| 9 | [2026-10-03](output/hacker_news_summary_2026-10-03.md) |
| 10 | [2026-10-09](output/hacker_news_summary_2026-10-09.md) |
| 11 | [2026-09-24](output/hacker_news_summary_2026-09-24.md) |
| 12 | [2026-09-21](output/hacker_news_summary_2026-09-21.md) |
| 13 | [2026-09-29](output/hacker_news_summary_2026-09-29.md) |
| 14 | [2026-09-23](output/hacker_news_summary_2026-09-23.md) |
| 15 | [2026-09-30](output/hacker_news_summary_2026-09-30.md) |
| 16 | [2026-09-27](output/hacker_news_summary_2026-09-27.md) |
| 17 | [2026-09-22](output/hacker_news_summary_2026-09-22.md) |
| 18 | [2026-09-25](output/hacker_news_summary_2026-09-25.md) |
| 19 | [2026-09-20](output/hacker_news_summary_2026-09-20.md) |
| 20 | [2026-09-16](output/hacker_news_summary_2026-09-16.md) |
| 21 | [2026-09-17](output/hacker_news_summary_2026-09-17.md) |
| 22 | [2026-09-19](output/hacker_news_summary_2026-09-19.md) |
| 23 | [2026-09-18](output/hacker_news_summary_2026-09-18.md) |
| 24 | [2026-09-15](output/hacker_news_summary_2026-09-15.md) |
| 25 | [2026-09-09](output/hacker_news_summary_2026-09-09.md) |
| 26 | [2026-09-10](output/hacker_news_summary_2026-09-10.md) |
| 27 | [2026-09-13](output/hacker_news_summary_2026-09-13.md) |
| 28 | [2026-09-08](output/hacker_news_summary_2026-09-08.md) |
| 29 | [2026-09-14](output/hacker_news_summary_2026-09-14.md) |
| 30 | [2026-09-07](output/hacker_news_summary_2026-09-07.md) |
| 31 | [2026-09-06](output/hacker_news_summary_2026-09-06.md) |
| 32 | [2026-09-11](output/hacker_news_summary_2026-09-11.md) |
| 33 | [2026-09-12](output/hacker_news_summary_2026-09-12.md) |
| 34 | [2026-09-03](output/hacker_news_summary_2026-09-03.md) |
| 35 | [2026-09-02](output/hacker_news_summary_2026-09-02.md) |
| 36 | [2026-08-31](output/hacker_news_summary_2026-08-31.md) |
| 37 | [2026-09-04](output/hacker_news_summary_2026-09-04.md) |
| 38 | [2026-09-05](output/hacker_news_summary_2026-09-05.md) |
| 39 | [2026-09-01](output/hacker_news_summary_2026-09-01.md) |
| 40 | [2026-08-29](output/hacker_news_summary_2026-08-29.md) |
| 41 | [2026-08-30](output/hacker_news_summary_2026-08-30.md) |
| 42 | [2026-08-22](output/hacker_news_summary_2026-08-22.md) |
| 43 | [2026-08-25](output/hacker_news_summary_2026-08-25.md) |
| 44 | [2026-08-19](output/hacker_news_summary_2026-08-19.md) |
| 45 | [2026-08-20](output/hacker_news_summary_2026-08-20.md) |
| 46 | [2026-08-17](output/hacker_news_summary_2026-08-17.md) |
| 47 | [2026-08-28](output/hacker_news_summary_2026-08-28.md) |
| 48 | [2026-08-23](output/hacker_news_summary_2026-08-23.md) |
| 49 | [2026-08-18](output/hacker_news_summary_2026-08-18.md) |
| 50 | [2026-08-21](output/hacker_news_summary_2026-08-21.md) |
| 51 | [2026-08-24](output/hacker_news_summary_2026-08-24.md) |
| 52 | [2026-08-26](output/hacker_news_summary_2026-08-26.md) |
| 53 | [2026-08-12](output/hacker_news_summary_2026-08-12.md) |
| 54 | [2026-08-11](output/hacker_news_summary_2026-08-11.md) |
| 55 | [2026-08-14](output/hacker_news_summary_2026-08-14.md) |
| 56 | [2026-08-16](output/hacker_news_summary_2026-08-16.md) |
| 57 | [2026-08-10](output/hacker_news_summary_2026-08-10.md) |
| 58 | [2026-08-09](output/hacker_news_summary_2026-08-09.md) |
| 59 | [2026-08-15](output/hacker_news_summary_2026-08-15.md) |
| 60 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 61 | [2026-08-13](output/hacker_news_summary_2026-08-13.md) |
| 62 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 63 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 64 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 65 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 66 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 67 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 68 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 69 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 70 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 71 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 72 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 73 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 74 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 75 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 76 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 77 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 78 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 79 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 80 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 81 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 82 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 83 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 84 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 85 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 86 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 87 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 88 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 89 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 90 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 91 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 92 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 93 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 94 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 95 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 96 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 97 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 98 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 99 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 100 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 101 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 102 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 103 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 104 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 105 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 106 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 107 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 108 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 109 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 110 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 111 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 112 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 113 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 114 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 115 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 116 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 117 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 118 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 119 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 120 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 121 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 122 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 123 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 124 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 125 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 126 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 127 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 128 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 129 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 130 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 131 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 132 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 133 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 134 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 135 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 136 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 137 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 138 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 139 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 140 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 141 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 142 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 143 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 144 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 145 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 146 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 147 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 148 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 149 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 150 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 151 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 152 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 153 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 154 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 155 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 156 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 157 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 158 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 159 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 160 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 161 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 162 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 163 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 164 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 165 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 166 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 167 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 168 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 169 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 170 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 171 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 172 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 173 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 174 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 175 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 176 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 177 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 178 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 179 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 180 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 181 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 182 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 183 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 184 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 185 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 186 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 187 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 188 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 189 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 190 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 191 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 192 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 193 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 194 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 195 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 196 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 197 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 198 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 199 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 200 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 201 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 202 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 203 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 204 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 205 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 206 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 207 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 208 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 209 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 210 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 211 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 212 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 213 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 214 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 215 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 216 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 217 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 218 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 219 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 220 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 221 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 222 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 223 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 224 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 225 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 226 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 227 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 228 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 229 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 230 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 231 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 232 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 233 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 234 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 235 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 236 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 237 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 238 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 239 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 240 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 241 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 242 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 243 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 244 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 245 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 246 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 247 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 248 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 249 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 250 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 251 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 252 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 253 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 254 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 255 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 256 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 257 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 258 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 259 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 260 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 261 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 262 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 263 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 264 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 265 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 266 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 267 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 268 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 269 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 270 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 271 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 272 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 273 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 274 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 275 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 276 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 277 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 278 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 279 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 280 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 281 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 282 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 283 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 284 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 285 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 286 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 287 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 288 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 289 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 290 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 291 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 292 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 293 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 294 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 295 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 296 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 297 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 298 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 299 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 300 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 301 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 302 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 303 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 304 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 305 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 306 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 307 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 308 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 309 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 310 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 311 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 312 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 313 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 314 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 315 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 316 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 317 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 318 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 319 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 320 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 321 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 322 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 323 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 324 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 325 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 326 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 327 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 328 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 329 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 330 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 331 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 332 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 333 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
