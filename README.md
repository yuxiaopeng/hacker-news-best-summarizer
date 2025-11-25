# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2025-11-25.md)

*最后自动更新时间: 2025-11-25 20:14:00*
## 1. Pebble 手表软件现已开源

**原文标题**: Pebble Watch software is now open source

**原文链接**: [https://ericmigi.com/blog/pebble-watch-software-is-now-100percent-open-source](https://ericmigi.com/blog/pebble-watch-software-is-now-100percent-open-source)

文章宣布Pebble手表软件现已100%开源，相较于之前的95%有了显著提升，并包含了新的Pebble移动应用程序的源代码。这项由Core Devices主导的举措，旨在确保Pebble手表在2025年1月重新发布后的长期可持续性。

为此，Core Devices依靠自有资金，并专注于盈利能力以继续生产手表，使Pebble Time 2等新型号更易于维修，采用螺丝固定式后盖方便更换电池。他们还发布了Pebble 2 Duo的电气和机械设计文件。

软件可持续性至关重要：PebbleOS自一月起已100%开源。适用于iOS和Android的新型跨平台Pebble移动配套应用现也已在GitHub上100%开源，解决了过去用户缺乏官方应用的问题。开发者工具和SDK已针对现代系统进行了更新。Pebble应用商店正在去中心化，支持多“源”，允许任何人创建应用商店。Core Devices已推出自己的源，并将内容备份到Archive.org，确保可靠性。尽管存在一些非开源组件（例如心率传感器、Memfault），但核心软件堆栈仍保持开源，且这些组件是可选的。

Pebble Time 2正处于设计验证测试（DVT）阶段。少量产品可能会在1月下旬的中国农历新年前发货，但大部分预计将在3月/4月到货。将提供四种颜色选项，选购邮件将在几周内发出。新一期“Tick Talk”节目提供了PT2的演示。

---

## 2. 克劳德 Opus 4.5

**原文标题**: Claude Opus 4.5

**原文链接**: [https://www.anthropic.com/news/claude-opus-4-5](https://www.anthropic.com/news/claude-opus-4-5)

Anthropic 于 2025 年 11 月 24 日发布了 Claude Opus 4.5，称其为全球在编码、智能体和计算机使用方面表现最佳的模型，并在深度研究以及处理幻灯片/电子表格方面有显著提升。它在真实世界的软件工程基准测试中取得了最先进的成果，超越了其前身 Sonnet 4.5 和竞争对手，通常用显著更少的 tokens。

Opus 4.5 可通过 Anthropic 的应用程序、API 和主要云平台访问，目前定价为每百万 tokens $5/$25，使其先进功能得以广泛应用。早期测试者和客户一致指出它能够处理模糊性、复杂错误和长周期任务，赞扬其前沿的任务规划、工具调用和高质量代码生成能力。它在多种应用中表现出色，从自我改进的 AI 智能体和代码重构，到长上下文故事创作和 Excel 自动化。值得注意的是，它在一次高难度工程考试中得分高于任何人类考生。

Opus 4.5 还展示了创造性解决问题的能力，有时能找到超出基准预期的、合理且意想不到的解决方案。它是 Anthropic 对齐最稳健的模型，表现出对提示注入攻击的强大抵抗力。

更新后的 Claude 开发者平台引入了一个新的“投入参数”，用于平衡成本/时间与能力，同时增强了多智能体系统的上下文管理。产品更新包括 Claude Code 的改进版规划模式和桌面应用程序、消费者应用程序中的持续长对话功能，以及扩展了 Claude 在 Chrome 和 Excel 上的访问权限，并提高了 Opus 4.5 用户的用量限制。

---

## 3. 沙虫归来：逾300个NPM包被感染

**原文标题**: Shai-Hulud Returns: Over 300 NPM Packages Infected

**原文链接**: [https://helixguard.ai/blog/malicious-sha1hulud-2025-11-24](https://helixguard.ai/blog/malicious-sha1hulud-2025-11-24)

HelixGuard，一家开源安全研究公司，报告了一起影响Node.js包管理器（NPM）生态系统中超过300个软件包的重大供应链攻击。

这起被不祥地命名为“沙虫归来”（Shai-Hulud Returns）的事件，暗示着一个重大且可能反复出现的威胁，或一次深层隐藏的入侵，如同《沙丘》传说中巨大的沙虫。这次感染表明恶意代码已被植入到这些广泛使用的软件组件中。

这对依赖这些组件的开发者和应用程序构成了巨大风险，可能导致数据泄露、后门、凭据窃取，或在开发和生产环境中进一步部署恶意软件。HelixGuard的发现强调了确保开源供应链安全的持续挑战，因为一个软件包的受损可能影响到众多下游项目。NPM用户被敦促保持警惕，仔细审查他们的依赖项，并等待HelixGuard提供的详细修复指导。

---

## 4. 断电的固态硬盘会缓慢丢失数据

**原文标题**: Unpowered SSDs slowly lose data

**原文链接**: [https://www.xda-developers.com/your-unpowered-ssd-is-slowly-losing-your-data/](https://www.xda-developers.com/your-unpowered-ssd-is-slowly-losing-your-data/)

未通电的固态硬盘（SSD）在长期闲置后，由于其NAND闪存单元中的电荷逐渐消散，容易导致数据丢失。与使用磁性存储的硬盘不同，SSD通过电压水平存储数据，而未通电时电压会衰减，从而导致信息损坏或丢失。

数据保留寿命因NAND类型而异：QLC NAND（大多数消费级SSD中常见）在未通电状态下可能只能保留数据1-2年，而TLC则可达3年。更昂贵的MLC和SLC NAND则分别提供5年和10年的保留期。因此，SSD不适合用于“冷存储”（长期未通电归档），传统硬盘、磁带或M-Disc是更合适的替代方案。

然而，文章澄清，这种担忧主要针对将数据长期存储在未通电硬盘上的企业用户、发烧友或独立创业者。大多数普通用户，他们的SSD在PC中会定期通电，在更换硬盘之前不太可能遇到这个问题。

无论存储介质如何，最关键的建议是实施一个强大的备份策略。遵循3-2-1备份规则（数据三份，至少存储在两种不同介质上，其中一份异地存放）等原则，能够让人安心，并防范硬盘故障和数据丢失，包括未通电SSD的数据保留限制。

---

## 5. 克劳德高级工具使用

**原文标题**: Claude Advanced Tool Use

**原文链接**: [https://www.anthropic.com/engineering/advanced-tool-use](https://www.anthropic.com/engineering/advanced-tool-use)

Anthropic 针对 Claude 推出了三项高级功能，旨在增强其 AI 代理能力：工具搜索工具、程序化工具调用和工具使用示例。这些创新旨在克服复杂代理工作流中上下文窗口饱和、推理开销大以及工具使用不精确等局限性。

**工具搜索工具**允许 Claude 访问庞大的工具库，而不会消耗过多的上下文。它无需预先加载所有工具定义（这在多服务器设置中很容易超过 50,000 个 token），而是按需发现并加载相关工具。这显著减少了初始 token 消耗（高达 85%），提高了工具选择的准确性，并为核心任务保留了上下文。

**程序化工具调用 (PTC)** 解决了多步骤工作流中的上下文污染和高推理成本问题。传统上，每次工具调用都需要进行一次推理，所有中间结果都会累积在 Claude 的上下文中。借助 PTC，Claude 可以编写 Python 代码，在沙盒执行环境中编排工具调用。中间数据处理发生在 Claude 的上下文之外，只有最终的、合成的结果才会返回给模型。这显著降低了 token 使用量（例如，在研究任务中可减少 37%），通过最小化推理次数减少了延迟，并通过明确的基于代码的控制流提高了准确性，从而能够高效处理数千行电子表格等任务。

**工具使用示例**通过提供一个通用标准来演示正确的工具使用模式，补充了模式定义，包括可选参数和 API 约定，这些是仅凭 JSON 模式无法传达的。

总体而言，这些功能使 Claude 能够构建更具可扩展性、更高效、更准确的 AI 代理，从而能够跨无限工具库管理复杂任务。

---

## 6. 法国威胁GrapheneOS，因拒绝后门将逮捕或查封其服务器。

**原文标题**: France threatens GrapheneOS with arrests / server seizure for refusing backdoors

**原文链接**: [https://mamot.fr/@LaQuadrature/115581775965025042](https://mamot.fr/@LaQuadrature/115581775965025042)

提供的內容是來自法國數字權利倡導組織“La Quadrature du Net”的一篇長毛象（Mastodon）帖子。該帖子簡要提及他們引用了“昨天《巴黎人報》的兩篇文章，今天接著……”

關鍵是，所提供的內容不包含任何信息或證據來支持標題中關於法國威脅GrapheneOS，稱如果拒絕後門將面臨逮捕或服務器扣押的說法。

帖子本身只提及《巴黎人報》中未具體的文章，所給文本中沒有提到GrapheneOS、法國政府的威脅、後門、逮捕或服務器扣押。

額外提供的中文文本是一條關於啟用JavaScript以使用網絡應用程序或選擇特定平台應用程序的通用長毛象消息，與所述主題無關。

實質上，所提供的文章內容不包含任何關於GrapheneOS、法國威脅、後門、逮捕或服務器扣押的細節。

---

## 7. X新的国家来源地功能揭示，许多“美国”账户实为境外运营

**原文标题**: X's new country-of-origin feature reveals many 'US' accounts to be foreign-run

**原文链接**: [https://www.hindustantimes.com/world-news/us-news/xs-new-country-of-origin-feature-shakes-maga-and-democrat-circles-as-many-us-accounts-revealed-to-be-foreignrun-101763857104296.html](https://www.hindustantimes.com/world-news/us-news/xs-new-country-of-origin-feature-shakes-maga-and-democrat-circles-as-many-us-accounts-revealed-to-be-foreignrun-101763857104296.html)

X（前身为推特）推出了一项新的“原籍国”功能，允许用户通过其“加入时间”选项卡查看某个账号的运营地点。这一进展在MAGA和民主党在线社区中引起了轩然大波，因为许多积极参与美国政治讨论并自称美国人的账号被揭示为从国外运营。

值得注意的例子包括与MAGA结盟的账号，如“MAGA NATION”（东欧）、“MAGA Scope”（尼日利亚）和“America First”（孟加拉国）。在民主党方面，自称“骄傲的民主党人”的“Ron Smith”被追踪到肯尼亚，而反特朗普页面“Republicans Against Trump”最初被发现位于奥地利（尽管现在据报使用VPN）。一个亲以色列账号“Mariana Times”也被链接到印度。

这些披露引发了“外国骗子”和“外国反对派”试图影响并破坏美国政治稳定的指控。众议员安娜·保利娜·卢娜和亚历克西斯·威尔金斯等人士表达了对外部势力散布分裂的担忧，并强调了外国运营账号以及使用VPN来掩盖真实位置所带来的挑战。

---

## 8. 爱荷华市公交免费了。交通顺畅了，空气也清新了。

**原文标题**: Iowa City made its buses free. Traffic cleared, and so did the air

**原文链接**: [https://www.nytimes.com/2025/11/18/climate/iowa-city-free-buses.html](https://www.nytimes.com/2025/11/18/climate/iowa-city-free-buses.html)

无法访问文章链接。

---

## 9. HN 展示：我构建了一个交互式HN模拟器

**原文标题**: Show HN: I built an interactive HN Simulator

**原文链接**: [https://news.ysimulator.run/news](https://news.ysimulator.run/news)

这篇“Show HN”公告介绍了一个交互式Hacker News模拟器。作者构建了一个旨在模拟热门Hacker News平台的工具，更多详情可另行查阅。

---

## 10. PS5现价低于64GB DDR5内存。内存因短缺飙升至600美元。

**原文标题**: PS5 now costs less than 64GB of DDR5 memory. RAM jumps to $600 due to shortage

**原文链接**: [https://www.tomshardware.com/pc-components/ddr5/64gb-of-ddr5-memory-now-costs-more-than-an-entire-ps5-even-after-a-discount-trident-z5-neo-kit-jumps-to-usd600-due-to-dram-shortage-and-its-expected-to-get-worse-into-2026](https://www.tomshardware.com/pc-components/ddr5/64gb-of-ddr5-memory-now-costs-more-than-an-entire-ps5-even-after-a-discount-trident-z5-neo-kit-jumps-to-usd600-due-to-dram-shortage-and-its-expected-to-get-worse-into-2026)

人工智能热潮正导致内存和存储价格空前飙升，使得DDR5内存等常见组件对终端消费者来说变得极其昂贵。一套64GB的芝奇幻锋戟Z5 Neo 6000 MT/s DDR5内存目前标价599.99美元，比几个月前205-220美元的价格大幅上涨——自10月底以来上涨了近190%。这使得这款内存套件比PS5 Slim或Xbox Series S更贵，几乎与PS5 Pro一样昂贵。

此前，类似的64GB套件价格曾低至140美元，凸显了惊人的通货膨胀。“AI需求激增”正在优先满足AI客户的需求，导致广泛的供应问题。除了内存，硬盘也正在消失，大容量硬盘的订单已排到两年后，这促使人们抢购QLC固态硬盘。甚至microSD卡也被考虑作为硬盘替代品，分销商正在将内存与主板捆绑销售以应对。Valve即将推出的Steam Machine预计也将涨价。

专家预测，随着科技巨头追求通用人工智能（AGI），DRAM和NAND的供应紧张将持续到2026年。尽管目前价格处于令人担忧的水平，但内存市场历来经历“过山车”式的周期，这表明到2027年DDR5内存可能再次出现廉价。

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 2 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 3 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 4 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 5 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 6 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 7 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 8 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 9 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 10 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 11 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 12 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 13 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 14 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 15 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 16 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 17 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 18 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 19 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 20 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
