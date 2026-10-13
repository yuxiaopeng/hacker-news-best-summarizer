# Hacker News 热门文章摘要 (2026-10-13)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

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

## 11. Nitter: Update Oct 10th seeking funding and legal help

**原文标题**: Nitter: Update Oct 10th seeking funding and legal help

**原文链接**: [https://nitter.net](https://nitter.net)

生成摘要时出错

---

## 12. Codex CLI installs a persistent, self-updating background daemon by default

**原文标题**: Codex CLI installs a persistent, self-updating background daemon by default

**原文链接**: [https://github.com/openai/codex/issues/48195](https://github.com/openai/codex/issues/48195)

生成摘要时出错

---

## 13. LineageOS 24

**原文标题**: LineageOS 24

**原文链接**: [https://lineageos.org/Changelog-32/](https://lineageos.org/Changelog-32/)

生成摘要时出错

---

## 14. Google told to halt work on datacentres in Finland over environmental concerns

**原文标题**: Google told to halt work on datacentres in Finland over environmental concerns

**原文链接**: [https://www.theguardian.com/technology/2026/oct/06/google-datacentres-finland-temporary-halt-environmental-impact-assessment](https://www.theguardian.com/technology/2026/oct/06/google-datacentres-finland-temporary-halt-environmental-impact-assessment)

生成摘要时出错

---

## 15. I'm sorry, but you still have to think

**原文标题**: I'm sorry, but you still have to think

**原文链接**: [https://itsallaboutthebit.com/i-am-sorry-but-you-still-have-to-think/](https://itsallaboutthebit.com/i-am-sorry-but-you-still-have-to-think/)

生成摘要时出错

---

## 16. Hackers activate automatic defrosting in supermarket fridges across Europe

**原文标题**: Hackers activate automatic defrosting in supermarket fridges across Europe

**原文链接**: [https://www.tomshardware.com/tech-industry/cyber-security/unprecedented-cyberattack-cripples-supermarket-fridges-across-europe-as-hackers-activate-automatic-defrosting-delivery-and-store-prices-also-impacted-by-incident](https://www.tomshardware.com/tech-industry/cyber-security/unprecedented-cyberattack-cripples-supermarket-fridges-across-europe-as-hackers-activate-automatic-defrosting-delivery-and-store-prices-also-impacted-by-incident)

生成摘要时出错

---

## 17. GLM-Legal

**原文标题**: GLM-Legal

**原文链接**: [https://z.ai/blog/glm-legal](https://z.ai/blog/glm-legal)

生成摘要时出错

---

## 18. I paid people to try and follow my README

**原文标题**: I paid people to try and follow my README

**原文链接**: [https://shkspr.mobi/blog/2026/10/i-paid-people-to-try-and-follow-my-readme/](https://shkspr.mobi/blog/2026/10/i-paid-people-to-try-and-follow-my-readme/)

生成摘要时出错

---

## 19. IRCv3

**原文标题**: IRCv3

**原文链接**: [https://ircv3.net/](https://ircv3.net/)

生成摘要时出错

---

## 20. Documents add to evidence in climate deception case against ExxonMobil

**原文标题**: Documents add to evidence in climate deception case against ExxonMobil

**原文链接**: [https://insideclimatenews.org/news/07102026/exxonmobil-climate-deception-new-evidence/](https://insideclimatenews.org/news/07102026/exxonmobil-climate-deception-new-evidence/)

生成摘要时出错

---

## 21. A Modern Web App in C

**原文标题**: A Modern Web App in C

**原文链接**: [https://prophitt.me/writing/a-modern-web-app-in-c](https://prophitt.me/writing/a-modern-web-app-in-c)

生成摘要时出错

---

## 22. So, you’d like to sell your print issues of The Onion?

**原文标题**: So, you’d like to sell your print issues of The Onion?

**原文链接**: [https://theonion.com/archivehunt/](https://theonion.com/archivehunt/)

生成摘要时出错

---

## 23. QGIS enacts moratorium on AI contributions

**原文标题**: QGIS enacts moratorium on AI contributions

**原文链接**: [https://github.com/qgis/QGIS-Enhancement-Proposals/pull/387](https://github.com/qgis/QGIS-Enhancement-Proposals/pull/387)

生成摘要时出错

---

## 24. Cartographers of North Korea (2019)

**原文标题**: Cartographers of North Korea (2019)

**原文链接**: [https://cartographers-nk.wonyoung.so/](https://cartographers-nk.wonyoung.so/)

生成摘要时出错

---

## 25. Why aren't AI companies being charged for hacking?

**原文标题**: Why aren't AI companies being charged for hacking?

**原文链接**: [https://mortoray.com/why-arent-ai-companies-being-charged-for-hacking/](https://mortoray.com/why-arent-ai-companies-being-charged-for-hacking/)

生成摘要时出错

---

## 26. AI coding agents generate more code, but not more software

**原文标题**: AI coding agents generate more code, but not more software

**原文链接**: [https://arstechnica.com/ai/2026/10/ai-coding-agents-generate-more-code-but-not-more-software/](https://arstechnica.com/ai/2026/10/ai-coding-agents-generate-more-code-but-not-more-software/)

生成摘要时出错

---

## 27. Show HN: WallHop – 12ft.io is gone, so I built a replacement

**原文标题**: Show HN: WallHop – 12ft.io is gone, so I built a replacement

**原文链接**: [https://wallhop.io/](https://wallhop.io/)

生成摘要时出错

---

## 28. A Remote Employee Refused 160 Webcam Photos a Day. Her Employer Fired Her

**原文标题**: A Remote Employee Refused 160 Webcam Photos a Day. Her Employer Fired Her

**原文链接**: [https://www.inc.com/chloe-rosenberg/a-remote-employee-refused-160-webcam-photos-a-day-her-employer-fired-her/91415963](https://www.inc.com/chloe-rosenberg/a-remote-employee-refused-160-webcam-photos-a-day-her-employer-fired-her/91415963)

生成摘要时出错

---

## 29. Show HN: PS2 games statically recompiled to WebAssembly

**原文标题**: Show HN: PS2 games statically recompiled to WebAssembly

**原文链接**: [https://github.com/snuri00/ps2-web-recomp](https://github.com/snuri00/ps2-web-recomp)

生成摘要时出错

---

## 30. Citroen revives the 2CV for an electric age

**原文标题**: Citroen revives the 2CV for an electric age

**原文链接**: [https://www.bbc.com/news/articles/c620r33plgppo](https://www.bbc.com/news/articles/c620r33plgppo)

生成摘要时出错

---

## 31. Will Linux phones become a viable alternative to the Android/iOS duopoly?

**原文标题**: Will Linux phones become a viable alternative to the Android/iOS duopoly?

**原文链接**: [https://amosbbatto.wordpress.com/2026/10/05/linux-phones-alternative/](https://amosbbatto.wordpress.com/2026/10/05/linux-phones-alternative/)

生成摘要时出错

---

## 32. Turn a WiFi 7 Router into a 320Msps Software Defined Radio Receiver

**原文标题**: Turn a WiFi 7 Router into a 320Msps Software Defined Radio Receiver

**原文链接**: [https://github.com/h0m3us3r/w1700k-sdr](https://github.com/h0m3us3r/w1700k-sdr)

生成摘要时出错

---

## 33. The tilde in your PATH may not be your HOME

**原文标题**: The tilde in your PATH may not be your HOME

**原文链接**: [https://disconnect3d.pl//2026/10/02/dont-put-tilde-in-your-path/](https://disconnect3d.pl//2026/10/02/dont-put-tilde-in-your-path/)

生成摘要时出错

---

## 34. Research Firm Calls Anthropic's IPO 'Unprecedented Test of Investor Gullibity'

**原文标题**: Research Firm Calls Anthropic's IPO 'Unprecedented Test of Investor Gullibity'

**原文链接**: [https://www.cnbc.com/2026/10/07/anthropic-will-be-most-ridiculous-ipo-of-year-analyst-says.html](https://www.cnbc.com/2026/10/07/anthropic-will-be-most-ridiculous-ipo-of-year-analyst-says.html)

生成摘要时出错

---

## 35. Type-safe HTML templating in Zig

**原文标题**: Type-safe HTML templating in Zig

**原文链接**: [https://lalinsky.com/2026/10/11/type-safe-html-templating-in-zig.html](https://lalinsky.com/2026/10/11/type-safe-html-templating-in-zig.html)

生成摘要时出错

---

## 36. Thinking will become a hobby

**原文标题**: Thinking will become a hobby

**原文链接**: [https://www.spinellis.gr/blog/20261008/?li261008](https://www.spinellis.gr/blog/20261008/?li261008)

生成摘要时出错

---

## 37. AI is a tool and using it well takes skill

**原文标题**: AI is a tool and using it well takes skill

**原文链接**: [https://yyhh.org/blog/2026/10/ai-is-a-tool/](https://yyhh.org/blog/2026/10/ai-is-a-tool/)

生成摘要时出错

---

## 38. Yandex bot traffic down 99% after data center attack

**原文标题**: Yandex bot traffic down 99% after data center attack

**原文链接**: [https://radar.cloudflare.com/bots/as13238?dateRange=7d#bot-traffic](https://radar.cloudflare.com/bots/as13238?dateRange=7d#bot-traffic)

生成摘要时出错

---

## 39. Fable Took My Job

**原文标题**: Fable Took My Job

**原文链接**: [https://cendyne.dev/posts/2026-10-11-fable-took-my-jorb.html](https://cendyne.dev/posts/2026-10-11-fable-took-my-jorb.html)

生成摘要时出错

---

## 40. 'AI' Is Not a Tool by Rich Hickey

**原文标题**: 'AI' Is Not a Tool by Rich Hickey

**原文链接**: [https://www.linkedin.com/pulse/ai-tool-rich-hickey-kjl8e](https://www.linkedin.com/pulse/ai-tool-rich-hickey-kjl8e)

生成摘要时出错

---

## 41. 500B tokens later: Letting AI agents decompile a first-person shooter

**原文标题**: 500B tokens later: Letting AI agents decompile a first-person shooter

**原文链接**: [https://momo5502.com/posts/2026-10-09-game-decompilation/](https://momo5502.com/posts/2026-10-09-game-decompilation/)

生成摘要时出错

---

## 42. Doory – Open-Source Canva

**原文标题**: Doory – Open-Source Canva

**原文链接**: [https://github.com/shaongitbd/doory](https://github.com/shaongitbd/doory)

生成摘要时出错

---

## 43. Show HN: BetterWispr – Free, open-source dictation for Mac

**原文标题**: Show HN: BetterWispr – Free, open-source dictation for Mac

**原文链接**: [https://betterwispr.com/](https://betterwispr.com/)

生成摘要时出错

---

## 44. OpenFatigue™ – Open is the new closed

**原文标题**: OpenFatigue™ – Open is the new closed

**原文链接**: [https://openfatigue.ai/](https://openfatigue.ai/)

生成摘要时出错

---

## 45. I Found a $90k Remote Code Execution Vulnerability in Google

**原文标题**: I Found a $90k Remote Code Execution Vulnerability in Google

**原文链接**: [https://simonkoeck.com/writeups/google-devsite-flask-session-pickle-rce](https://simonkoeck.com/writeups/google-devsite-flask-session-pickle-rce)

生成摘要时出错

---

## 46. Zod 4.6.6 compromised by malware?

**原文标题**: Zod 4.6.6 compromised by malware?

**原文链接**: [https://github.com/colinhacks/zod/commit/d821685ea6732436fcdf786a81d076958471e467](https://github.com/colinhacks/zod/commit/d821685ea6732436fcdf786a81d076958471e467)

生成摘要时出错

---

## 47. Valen's Memory Safety: A New Kind of Borrow Checking

**原文标题**: Valen's Memory Safety: A New Kind of Borrow Checking

**原文链接**: [https://verdagon.dev/blog/valen-group-borrowing](https://verdagon.dev/blog/valen-group-borrowing)

生成摘要时出错

---

## 48. Using AI for just 10 minutes erodes your ability to persist at hard things

**原文标题**: Using AI for just 10 minutes erodes your ability to persist at hard things

**原文链接**: [https://vcresearch.berkeley.edu/news/using-ai-just-10-minutes-erodes-your-ability-persist-hard-things](https://vcresearch.berkeley.edu/news/using-ai-just-10-minutes-erodes-your-ability-persist-hard-things)

生成摘要时出错

---

## 49. Postgres isn't slow, your storage is

**原文标题**: Postgres isn't slow, your storage is

**原文链接**: [https://clickhouse.com/blog/posette-talk-recap-postgres-isnt-slow-your-storage-is](https://clickhouse.com/blog/posette-talk-recap-postgres-isnt-slow-your-storage-is)

生成摘要时出错

---

## 50. Whatever became of holography? (2011)

**原文标题**: Whatever became of holography? (2011)

**原文链接**: [https://www.americanscientist.org/article/whatever-became-of-holography](https://www.americanscientist.org/article/whatever-became-of-holography)

生成摘要时出错

---

## 51. How to Build Wealth as a Career Person

**原文标题**: How to Build Wealth as a Career Person

**原文链接**: [https://asheradeniyi.com/2026/04/10/how-to-build-wealth-as-a-career-person/](https://asheradeniyi.com/2026/04/10/how-to-build-wealth-as-a-career-person/)

生成摘要时出错

---

## 52. Just say no to OpenAI and Anthropic

**原文标题**: Just say no to OpenAI and Anthropic

**原文链接**: [https://micahflee.com/just-say-no-to-openai-and-anthropic/](https://micahflee.com/just-say-no-to-openai-and-anthropic/)

生成摘要时出错

---

## 53. French supermarkets suffer fridge shutdown after 'unprecedented' cyberattack

**原文标题**: French supermarkets suffer fridge shutdown after 'unprecedented' cyberattack

**原文链接**: [https://uk.finance.yahoo.com/news/french-supermarket-chains-cyberattack-forced-115141288.html](https://uk.finance.yahoo.com/news/french-supermarket-chains-cyberattack-forced-115141288.html)

生成摘要时出错

---

## 54. Incident with Actions, Pull Requests and Issues

**原文标题**: Incident with Actions, Pull Requests and Issues

**原文链接**: [https://www.githubstatus.com/incidents/93njd414rpbx](https://www.githubstatus.com/incidents/93njd414rpbx)

生成摘要时出错

---

## 55. Feds got warrants to use fake cell towers to hunt down Don Lemon's producer

**原文标题**: Feds got warrants to use fake cell towers to hunt down Don Lemon's producer

**原文链接**: [https://www.wired.com/story/feds-got-warrants-to-use-fake-cell-towers-to-hunt-down-don-lemons-producer/](https://www.wired.com/story/feds-got-warrants-to-use-fake-cell-towers-to-hunt-down-don-lemons-producer/)

生成摘要时出错

---

## 56. GameBoy on E-Paper ESP32 at 30FPS [video]

**原文标题**: GameBoy on E-Paper ESP32 at 30FPS [video]

**原文链接**: [https://www.youtube.com/watch?v=XiZmM6hwwAU](https://www.youtube.com/watch?v=XiZmM6hwwAU)

生成摘要时出错

---

## 57. European Alternatives

**原文标题**: European Alternatives

**原文链接**: [https://buy-european.net/en/alternatives](https://buy-european.net/en/alternatives)

生成摘要时出错

---

## 58. Fridges in French supermarkets hit by cyber attack

**原文标题**: Fridges in French supermarkets hit by cyber attack

**原文链接**: [https://www.bbc.com/news/articles/crq5nzxv9q4yo](https://www.bbc.com/news/articles/crq5nzxv9q4yo)

生成摘要时出错

---

## 59. Chapter 1 of "Ways of Seeing" by John Berger (1972)

**原文标题**: Chapter 1 of "Ways of Seeing" by John Berger (1972)

**原文链接**: [https://www.ways-of-seeing.com/ch1](https://www.ways-of-seeing.com/ch1)

生成摘要时出错

---

## 60. Kevin Kelly's 2016 AI Predictions, 10 Years Later

**原文标题**: Kevin Kelly's 2016 AI Predictions, 10 Years Later

**原文链接**: [https://taylor.town/kk-ai-2026](https://taylor.town/kk-ai-2026)

生成摘要时出错

---

## 61. Recursive self-improvement through collective intelligence

**原文标题**: Recursive self-improvement through collective intelligence

**原文链接**: [https://pub.sakana.ai/mass/](https://pub.sakana.ai/mass/)

生成摘要时出错

---

## 62. PSPi 6 – Raspberry Pi in a PSP

**原文标题**: PSPi 6 – Raspberry Pi in a PSP

**原文链接**: [https://github.com/othermod/PSPi-Version-6](https://github.com/othermod/PSPi-Version-6)

生成摘要时出错

---

## 63. How I reverse engineered a commercial spatial audio effect

**原文标题**: How I reverse engineered a commercial spatial audio effect

**原文链接**: [http://epestr.com/blog/reverse-engineering-a-commercial-spatial-audio-effect/](http://epestr.com/blog/reverse-engineering-a-commercial-spatial-audio-effect/)

生成摘要时出错

---

## 64. RJ Mitte has died

**原文标题**: RJ Mitte has died

**原文链接**: [https://news.sky.com/story/breaking-bad-star-rj-mitte-dies-aged-34-13598332](https://news.sky.com/story/breaking-bad-star-rj-mitte-dies-aged-34-13598332)

生成摘要时出错

---

## 65. Attack of the Vibe Coded Photoshop Clones

**原文标题**: Attack of the Vibe Coded Photoshop Clones

**原文链接**: [https://www.shokunin.studio/blog/2026/10/9/attack-of-the-vibe-coded-photoshop-clones](https://www.shokunin.studio/blog/2026/10/9/attack-of-the-vibe-coded-photoshop-clones)

生成摘要时出错

---

## 66. Local Indexing to reduce tool calling and token usage

**原文标题**: Local Indexing to reduce tool calling and token usage

**原文链接**: [https://tedhaley.ca/pensieve/](https://tedhaley.ca/pensieve/)

生成摘要时出错

---

## 67. Who Is Vfmaddrnd231pd?

**原文标题**: Who Is Vfmaddrnd231pd?

**原文链接**: [https://purplesyringa.moe/blog/who-is-vfmaddrnd231pd/](https://purplesyringa.moe/blog/who-is-vfmaddrnd231pd/)

生成摘要时出错

---

## 68. Publishers Killed the Paperback, Then Blamed Readers

**原文标题**: Publishers Killed the Paperback, Then Blamed Readers

**原文链接**: [https://jacobin.com/2026/10/books-publishing-reading-mass-market-paperback](https://jacobin.com/2026/10/books-publishing-reading-mass-market-paperback)

生成摘要时出错

---

## 69. Solar panels that plug into your wall

**原文标题**: Solar panels that plug into your wall

**原文链接**: [https://www.nationalgeographic.com/environment/article/balcony-plug-in-solar-panels-renewable-energy](https://www.nationalgeographic.com/environment/article/balcony-plug-in-solar-panels-renewable-energy)

生成摘要时出错

---

## 70. Governments are mishandling the affordability crisis

**原文标题**: Governments are mishandling the affordability crisis

**原文链接**: [https://www.economist.com/finance-and-economics/2026/10/08/governments-are-mishandling-the-affordability-crisis](https://www.economist.com/finance-and-economics/2026/10/08/governments-are-mishandling-the-affordability-crisis)

生成摘要时出错

---

## 71. An open-source, clean-room reimplementation of Microsoft Word in pure Rust

**原文标题**: An open-source, clean-room reimplementation of Microsoft Word in pure Rust

**原文链接**: [https://github.com/storytold/wordcraft](https://github.com/storytold/wordcraft)

生成摘要时出错

---

## 72. Illustration Beyond Proof

**原文标题**: Illustration Beyond Proof

**原文链接**: [https://terrytao.wordpress.com/2026/10/11/illustration-beyond-proof/](https://terrytao.wordpress.com/2026/10/11/illustration-beyond-proof/)

生成摘要时出错

---

## 73. Nicolas Cage says he won't work with Amazon again over AI dispute

**原文标题**: Nicolas Cage says he won't work with Amazon again over AI dispute

**原文链接**: [https://www.latimes.com/entertainment-arts/business/story/2026-10-10/nicolas-cage-says-he-wont-work-with-amazon-again-over-ai-dispute](https://www.latimes.com/entertainment-arts/business/story/2026-10-10/nicolas-cage-says-he-wont-work-with-amazon-again-over-ai-dispute)

生成摘要时出错

---

## 74. Google Data Centers around the world

**原文标题**: Google Data Centers around the world

**原文链接**: [https://datacenters.google/locations/](https://datacenters.google/locations/)

生成摘要时出错

---

## 75. Running the unmodified Linux amdgpu driver on an iPad

**原文标题**: Running the unmodified Linux amdgpu driver on an iPad

**原文链接**: [https://github.com/Geramy/LemonSeed-Studio](https://github.com/Geramy/LemonSeed-Studio)

生成摘要时出错

---

## 76. Scandinavia's first farmers slaughtered hunter-gatherer population, DNA suggests

**原文标题**: Scandinavia's first farmers slaughtered hunter-gatherer population, DNA suggests

**原文链接**: [https://phys.org/news/2024-02-scandinavia-farmers-slaughtered-hunter-population.html](https://phys.org/news/2024-02-scandinavia-farmers-slaughtered-hunter-population.html)

生成摘要时出错

---

## 77. Living in the Weimar Era of Ruby

**原文标题**: Living in the Weimar Era of Ruby

**原文链接**: [https://blog.julik.nl/2026/10/the-weimar-of-ruby](https://blog.julik.nl/2026/10/the-weimar-of-ruby)

生成摘要时出错

---

## 78. apsw: Another Python SQLite Wrapper

**原文标题**: apsw: Another Python SQLite Wrapper

**原文链接**: [https://github.com/rogerbinns/apsw](https://github.com/rogerbinns/apsw)

生成摘要时出错

---

## 79. (Post-Quantum) Cryptographic Right Answers

**原文标题**: (Post-Quantum) Cryptographic Right Answers

**原文链接**: [https://words.filippo.io/right-answers/](https://words.filippo.io/right-answers/)

生成摘要时出错

---

## 80. HashiCorp archives the Boundary open source repo

**原文标题**: HashiCorp archives the Boundary open source repo

**原文链接**: [https://github.com/hashicorp/boundary](https://github.com/hashicorp/boundary)

生成摘要时出错

---

## 81. YouTuber builds 'Flock-like' camera to track police vehicles, gets police visit

**原文标题**: YouTuber builds 'Flock-like' camera to track police vehicles, gets police visit

**原文链接**: [https://www.tomshardware.com/tech-industry/cyber-security/canadian-youtuber-builds-flock-like-camera-to-exclusively-track-police-vehicles-officers-visit-his-home-to-express-privacy-concerns](https://www.tomshardware.com/tech-industry/cyber-security/canadian-youtuber-builds-flock-like-camera-to-exclusively-track-police-vehicles-officers-visit-his-home-to-express-privacy-concerns)

生成摘要时出错

---

## 82. I wish you the best in the Offline

**原文标题**: I wish you the best in the Offline

**原文链接**: [https://daverupert.com/2026/09/i-wish-you-the-best-in-the-offline/](https://daverupert.com/2026/09/i-wish-you-the-best-in-the-offline/)

生成摘要时出错

---

## 83. Reverse engineer anything with agents, from app behavior down to native binaries

**原文标题**: Reverse engineer anything with agents, from app behavior down to native binaries

**原文链接**: [https://github.com/morluto/rea](https://github.com/morluto/rea)

生成摘要时出错

---

## 84. British PM says it is 'clear' Russia interfered with Brexit vote

**原文标题**: British PM says it is 'clear' Russia interfered with Brexit vote

**原文链接**: [https://www.bbc.com/news/articles/c6jdm3zggl0ko](https://www.bbc.com/news/articles/c6jdm3zggl0ko)

生成摘要时出错

---

## 85. Programmable pigments: Photochromic nanoparticle inks for rewritable tattoos

**原文标题**: Programmable pigments: Photochromic nanoparticle inks for rewritable tattoos

**原文链接**: [https://www.cell.com/matter-light/fulltext/S3117-5848(26)00119-5](https://www.cell.com/matter-light/fulltext/S3117-5848(26)00119-5)

生成摘要时出错

---

## 86. Making big downloads resumable in Firefox

**原文标题**: Making big downloads resumable in Firefox

**原文链接**: [https://lunarwatcher.codeberg.page/til/firefox/resumable-big-downloads.html](https://lunarwatcher.codeberg.page/til/firefox/resumable-big-downloads.html)

生成摘要时出错

---

## 87. Ledger confirms hidden chip in crypto wallet amid $92M theft claims

**原文标题**: Ledger confirms hidden chip in crypto wallet amid $92M theft claims

**原文链接**: [https://crypto.news/ledger-confirms-hidden-chip-in-crypto-wallet-amid-92m/](https://crypto.news/ledger-confirms-hidden-chip-in-crypto-wallet-amid-92m/)

生成摘要时出错

---

## 88. CIA World Factbook is dead – Here is an attempt at recreation

**原文标题**: CIA World Factbook is dead – Here is an attempt at recreation

**原文链接**: [https://worldfacts.app](https://worldfacts.app)

生成摘要时出错

---

## 89. My Reddit AMA on the Law of Web Scraping

**原文标题**: My Reddit AMA on the Law of Web Scraping

**原文链接**: [https://blog.ericgoldman.org/archives/2026/10/my-reddit-ama-on-the-law-of-web-scraping.htm](https://blog.ericgoldman.org/archives/2026/10/my-reddit-ama-on-the-law-of-web-scraping.htm)

生成摘要时出错

---

## 90. X Is Bad, Though

**原文标题**: X Is Bad, Though

**原文链接**: [https://lexontech.org/x-is-bad-though](https://lexontech.org/x-is-bad-though)

生成摘要时出错

---

## 91. AI models may be capable of self-replicating without access to a datacenter

**原文标题**: AI models may be capable of self-replicating without access to a datacenter

**原文链接**: [https://www.anthropic.com/research/self-replicating-ai](https://www.anthropic.com/research/self-replicating-ai)

生成摘要时出错

---

## 92. Epic Games tells employees to use AI to get Disney game done

**原文标题**: Epic Games tells employees to use AI to get Disney game done

**原文链接**: [https://www.avclub.com/epic-games-disney-ai-delay](https://www.avclub.com/epic-games-disney-ai-delay)

生成摘要时出错

---

## 93. Open-source Microsoft Excel, PowerPoint, and Word replications

**原文标题**: Open-source Microsoft Excel, PowerPoint, and Word replications

**原文链接**: [https://www.tomshardware.com/software/microsoft-office/creator-of-free-adobe-clones-unveils-open-source-microsoft-office-excel-powerpoint-and-word-replications-autodesk-tools-and-other-subscription-based-services-may-come-next](https://www.tomshardware.com/software/microsoft-office/creator-of-free-adobe-clones-unveils-open-source-microsoft-office-excel-powerpoint-and-word-replications-autodesk-tools-and-other-subscription-based-services-may-come-next)

生成摘要时出错

---

## 94. GPT-6 Astra Helped Me Jailbreak My Kindle

**原文标题**: GPT-6 Astra Helped Me Jailbreak My Kindle

**原文链接**: [https://nirajrajgor.com/blog/kindle-photo-frame-with-ai](https://nirajrajgor.com/blog/kindle-photo-frame-with-ai)

生成摘要时出错

---

## 95. Blood cells from 80-year-old donor become stem cells with molecular age under 20

**原文标题**: Blood cells from 80-year-old donor become stem cells with molecular age under 20

**原文链接**: [https://doi.org/10.1111/acel.70751](https://doi.org/10.1111/acel.70751)

生成摘要时出错

---

## 96. Writing a Demoscene Intro for the ZX Spectrum

**原文标题**: Writing a Demoscene Intro for the ZX Spectrum

**原文链接**: [https://www.markround.com/blog/2026/zx-spectrum-intro](https://www.markround.com/blog/2026/zx-spectrum-intro)

生成摘要时出错

---

## 97. The Corporate Happiness Treadmill and the Case for Doing Less

**原文标题**: The Corporate Happiness Treadmill and the Case for Doing Less

**原文链接**: [https://0xff.nu/corp-burnout/](https://0xff.nu/corp-burnout/)

生成摘要时出错

---

## 98. AI is creating a 'human premium' for art created by people

**原文标题**: AI is creating a 'human premium' for art created by people

**原文链接**: [https://www.bbc.com/news/articles/c5vgjm3gk7rzo](https://www.bbc.com/news/articles/c5vgjm3gk7rzo)

生成摘要时出错

---

## 99. We're unlocking the biggest mysteries of the clitoris

**原文标题**: We're unlocking the biggest mysteries of the clitoris

**原文链接**: [https://www.sciencefocus.com/the-human-body/were-finally-unlocking-the-biggest-mysteries-of-the-clitoris-2](https://www.sciencefocus.com/the-human-body/were-finally-unlocking-the-biggest-mysteries-of-the-clitoris-2)

生成摘要时出错

---

## 100. Playgrnd – tiny tools for making weird, beautiful things

**原文标题**: Playgrnd – tiny tools for making weird, beautiful things

**原文链接**: [https://www.playgrnd.tools/](https://www.playgrnd.tools/)

生成摘要时出错

---

