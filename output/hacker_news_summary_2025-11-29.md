# Hacker News 热门文章摘要 (2025-11-29)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 口袋基地：单文件的开源实时后端

**原文标题**: Pocketbase – open-source realtime back end in 1 file

**原文链接**: [https://pocketbase.io/](https://pocketbase.io/)

Pocketbase 是一款开源的实时后端解决方案，其“单文件”打包的特性尤为突出。这一特性凸显了其极致的简洁性、易于设置和可移植性。作为一款实时后端，它想必提供了数据库、API和用户认证等核心功能，所有这些都旨在实现快速应用开发。文章鼓励用户通过体验实时演示来立即参与，并通过查阅详尽的文档来深入了解其功能。总之，Pocketbase 旨在为开发者提供一个轻量、高效且快速部署的后端。

---

## 2. 欧盟理事会通过新“聊天控制”授权 推动大规模监控

**原文标题**: EU Council Approves New "Chat Control" Mandate Pushing Mass Surveillance

**原文链接**: [https://reclaimthenet.org/eu-council-approves-new-chat-control-mandate-pushing-mass-surveillance](https://reclaimthenet.org/eu-council-approves-new-chat-control-mandate-pushing-mass-surveillance)

欧盟理事会已临时批准一项备受争议的“聊天控制”指令，其官方名称为CSAM（儿童性虐待材料）条例。该妥协文本旨在通过强制通信服务提供商扫描私人消息和内容来打击CSAM。

该提案的核心要素是“上传审核”或客户端扫描（CSS），即在内容加密*之前*在用户设备上进行扫描。尽管当前的妥协方案基于风险评估将其称为提供商的“自愿”行为，但批评人士认为，这实际上是在迫使他们部署可能破坏端到端加密（E2EE）并引入重大安全漏洞的技术。

隐私倡导者、安全专家和科技公司普遍谴责该指令，认为它是一种侵犯基本权利的大规模监控形式。担忧还包括人工智能检测系统产生高误报的可能性，以及该条例对大多数通信服务的广泛适用性。

此次批准确立了理事会的谈判立场。该提案现在将与欧洲议会进行“三方对话”谈判，欧洲议会历来对客户端扫描措施持更抵制态度。这些讨论的结果将决定该立法的最终形式。

---

## 3. 请愿在德国正式承认开源工作为公民服务

**原文标题**: Petition to formally recognize open source work as civic service in Germany

**原文链接**: [https://www.openpetition.de/petition/online/anerkennung-von-open-source-arbeit-als-ehrenamt-in-deutschland#petition-main](https://www.openpetition.de/petition/online/anerkennung-von-open-source-arbeit-als-ehrenamt-in-deutschland#petition-main)

德国一项请愿正在倡导正式承认开源工作为公益服务（即“Ehrenamt”）。该倡议旨在通过赋予开发者与从事传统志愿或社团活动（即“Vereinsarbeit”）的人同等的地位，从而加强开源贡献。新闻报道指出，这种官方认可的呼声日益高涨，突显了开源工作对社会的价值，并旨在提升其在德国公民体系中的地位。

---

## 4. HN 展示：识别带摄像头智能眼镜的眼镜

**原文标题**: Show HN: Glasses to detect smart-glasses that have cameras

**原文链接**: [https://github.com/NullPxl/banrays](https://github.com/NullPxl/banrays)

“禁光”项目正在开发一种眼镜，用于检测带有摄像头的智能眼镜，特别是Meta Ray-Ban眼镜，这与过去针对早期拍照手机的努力有异曲同工之处。开发者正在探索两种主要的检测方法：光学和网络。

**光学**方法试图通过检测“猫眼效应”来识别摄像头，即CMOS传感器会逆向反射红外光。该系统利用红外LED和光电二极管，旨在对反射光进行分类。尽管原理可行，但对Meta Ray-Ban眼镜的初步测试产生了微弱且不一致的信号，在不依赖摄像头或复杂机器学习（这正是项目想要避免的）的情况下，很难可靠地将其与其他反光表面区分开。该领域的未来工作包括测试不同的红外波长、扫描模式和准直。

主要利用低功耗蓝牙 (BLE) 的**网络**方法已显示出更大的前景。该系统通过检测Meta Ray-Ban眼镜在开机、配对或从眼镜盒中取出时的独特制造商ID (0x01AB) 和服务UUID (0xFD5F)，成功识别其特征，从而触发声音警报。这目前被认为是最简单、最可靠的方法。然而，在主动使用期间（当与已配对手机通信时）检测眼镜是困难的，因为这涉及定向BLE流量，需要跟踪跳频信道，而当前硬件尚未为此配置。未来的计划包括探索nRF模块和主动探测。

---

## 5. Imgur地理封锁了英国，所以我解除了我网络的地理封锁。

**原文标题**: Imgur geo-blocked the UK, so I geo-unblocked my network

**原文链接**: [https://blog.tymscar.com/posts/imgurukproxy/](https://blog.tymscar.com/posts/imgurukproxy/)

作者面临Imgur对英国用户实施地域限制的问题，导致旧网站、论坛和文档中无数嵌入图片无法访问。作者排除了客户端VPN方案，原因是其2.5 Gbps互联网的速度顾虑以及每台设备单独设置的不便。他们利用自己的家庭实验室，设计了一个网络范围的解决方案。

该系统的工作原理如下：
1. **Pi-hole** 拦截对 `i.imgur.com` 的DNS请求，将其重定向到本地的 **Traefik** 反向代理。
2. **Traefik** 使用带TLS直通的TCP路由，将这些请求转发给一个 **Gluetun** 容器。
3. **Gluetun** 建立VPN连接，提供一个非英国的出口点。
4. 一个在Gluetun网络命名空间内运行的 **Nginx** 代理，通过VPN隧道对真实的 `i.imgur.com` 执行TCP直通。
5. 整个Docker Compose堆栈（Gluetun和Nginx）由 **NixOS** 作为systemd服务进行声明式管理，VPN凭据则使用 **Agenix** 进行保护。

这种设置使得网络上的每台设备都能自动、透明地访问Imgur图片，无需任何客户端配置。延迟增加微乎其微，且仅影响Imgur流量，保留了所有其他互联网使用的全速。作者承认这可能有些“过度设计”，但他们珍视这种干净、低维护、高效且能无缝融入其家庭实验室的解决方案。

---

## 6. 空客A320：强烈太阳辐射可能破坏飞行关键数据

**原文标题**: Airbus A320 – intense solar radiation may corrupt data critical for flight

**原文链接**: [https://www.airbus.com/en/newsroom/press-releases/2025-11-airbus-update-on-a320-family-precautionary-fleet-action](https://www.airbus.com/en/newsroom/press-releases/2025-11-airbus-update-on-a320-family-precautionary-fleet-action)

空中客车公司于2025年11月28日宣布，强烈的太阳辐射可能会损坏其A320系列飞机中对飞行控制至关重要的数据。在对近期一起事件进行分析后，发现了这个问题。大量在役的A320系列飞机可能受到影响。

为此，空中客车公司已主动与航空当局合作，向运营商发布了《警示运营商通告》（AOT）。该AOT要求立即采取预防措施，包括实施可用的软件和/或硬件保护，以确保机队的持续安全。欧洲航空安全局（EASA）随后将发布一份《紧急适航指令》（EAD），以反映这些建议。

空中客车公司承认，这些必要的措施将给乘客和客户带来运营中断，并为此表示歉意。该公司表示将与运营商紧密合作，将安全作为其首要任务。

---

## 7. AI CEO — 取代你的老板，趁他们还没取代你。

**原文标题**: AI CEO – Replace your boss before they replace you

**原文链接**: [https://replaceyourboss.ai/](https://replaceyourboss.ai/)

文章《AI CEO——在他们取代你之前，先取代你的老板》提出了一个快速临近的未来，在这个未来中，人工智能(AI)不再仅仅是一个辅助工具，而是一种可行且可能更优越的人类领导替代方案，即使在最高执行层面也是如此。

核心前提提出了双重挑战和机遇：
1.  **拥抱AI以提升自身地位：** 鼓励个人积极学习并将AI工具和策略融入到工作中。通过利用AI自动化、优化和创新传统上由上级执行的任务，员工可以有效地“取代”老板角色中的职能部分，展示出更高的价值和战略远见。
2.  **立即行动以避免被淘汰：** “在他们取代你之前”这一紧急警告强调了AI的颠覆性力量。如果员工未能适应、提升技能并驾驭AI，他们将面临被淘汰的风险——这可能是由拥抱新技术的精通AI的管理者造成的，或者直接由能够更高效、更有效地完成他们工作（甚至老板工作）的AI系统造成的。

本文实质上是对职业转型发出的严厉号召。它认为，成功驾驭AI驱动的未来需要个人成为积极的创新者，将AI作为战略杠杆来巩固和发展自己的职业生涯，而不是被动等待其不可避免的颠覆所影响。

---

## 8. 泄露消息证实，OpenAI 正准备在 ChatGPT 上推出广告，面向公众。

**原文标题**: Leak confirms OpenAI is preparing ads on ChatGPT for public roll out

**原文链接**: [https://www.bleepingcomputer.com/news/artificial-intelligence/leak-confirms-openai-is-preparing-ads-on-chatgpt-for-public-roll-out/](https://www.bleepingcomputer.com/news/artificial-intelligence/leak-confirms-openai-is-preparing-ads-on-chatgpt-for-public-roll-out/)

最近泄露的消息证实，OpenAI正在ChatGPT安卓应用（版本1.2025.329测试版）内部测试一项“广告功能”，这标志着该平台正朝着商业化方向迈出重要一步。据Tibor在X上发现，该应用的代码包含“bazaar内容”、“搜索广告”和“搜索广告轮播”等引用。

此举旨在复制谷歌搜索的广告模式，可能扰乱网络经济。与目前无广告的用户体验（付费方案除外）不同，ChatGPT计划整合广告。专家认为，由于OpenAI对用户有深入了解，这些广告可能具有高度个性化和有效性，甚至可能“悄悄地”嵌入到搜索结果中。

最初，广告预计将仅限于搜索体验，尽管这可能会扩大。ChatGPT庞大且快速增长的用户群，使其成为成功投放广告的理想选择。该平台目前拥有约8亿周活跃用户（2023年11月时为1亿），每天处理约25亿次提示，印度是其最大的单一用户群体。这种巨大的用户参与度为成功推出广告奠定了坚实基础。

---

## 9. 2800万条Hacker News评论：向量嵌入搜索数据集

**原文标题**: 28M Hacker News comments as vector embedding search dataset

**原文链接**: [https://clickhouse.com/docs/getting-started/example-datasets/hackernews-vector-search-dataset](https://clickhouse.com/docs/getting-started/example-datasets/hackernews-vector-search-dataset)

本文阐述了如何使用 ClickHouse 中的 2874 万条 Hacker News 评论构建一个大规模向量嵌入搜索和摘要应用。

该数据集包含 2874 万条 Hacker News 帖子及其 384 维向量嵌入，这些嵌入由 SentenceTransformers 的 `all-MiniLM-L6-v2` 模型生成。本指南详细介绍了在 ClickHouse 中设置 `hackernews` 表、从 S3 Parquet 文件加载数据，以及在 `vector` 列上使用 `cosineDistance` 构建 HNSW 向量相似性索引以实现高效的近似最近邻 (ANN) 搜索的步骤。

为了执行搜索，用户将了解到如何使用相同的 `all-MiniLM-L6-v2` 模型在 Python 中生成查询嵌入，然后通过在 ClickHouse 中执行 SQL 查询来检索语义相似的帖子。

此外，本文还介绍了一个生成式 AI 摘要应用。该基于 Python 的工具接收用户定义的主题，执行向量相似性搜索以检索相关的 Hacker News 帖子，然后利用 LangChain 和 OpenAI 的 `gpt-3.5-turbo` API 对检索到的内容进行摘要。这展示了一个强大的用例，即向量搜索为大型语言模型提供了上下文，适用于客户情感分析或技术支持自动化等各种企业领域。

---

## 10. 信用报告显示，Meta通过先进的几何学将270亿美元不计入其账目。

**原文标题**: Credit report shows Meta keeping $27B off its books through advanced geometry

**原文链接**: [https://stohl.substack.com/p/exclusive-credit-report-shows-meta](https://stohl.substack.com/p/exclusive-credit-report-shows-meta)

这篇以一份来自“Equiplex”的“泄露”信用报告为基础的独家报道声称，Meta正在利用先进的几何技术，使其270亿美元不计入账目。该报告指出，Meta正在使用“闵可夫斯基和”和“双曲密铺”在其财务记录中创建非欧几里得空间。

作者，一位前几何学教师，解释说闵可夫斯基和允许“将金融实体融合到一个单一但几何上扩展的会计空间中”，有效地隐藏了价值。双曲密铺通过在有限的账本空间内创建“无限的子账户”进一步使其复杂化，使得资产的真实规模难以确定。

文章强调了一个可疑的“负空间权益”条目，作者将其解读为Meta正在利用其财务维度中“非存在”的内在价值。“Equiplex”的分析师在Meta的“资产-负债关联图”中注意到“令人眼花缭乱的多面体结构”，这暗示了一种故意的混淆策略。结论是，Meta利用这些抽象的几何原理并非用于技术创新，而是用于“宇宙级逃税”，通过维持一个“在数学上严谨，但在财务上隐形”的帝国。作者认为这种做法可能预示着一个“几何会计”新时代的到来。

---

## 11. 莫莉：Signal改进版

**原文标题**: Molly: An Improved Signal App

**原文链接**: [https://molly.im/](https://molly.im/)

Molly是Signal安卓应用的一个独立分支，旨在成为一个具有增强功能和隐私保护的改进版本。与Signal不同，Molly是完全的FOSS（自由及开源软件），不含任何专有二进制文件。

主要特点和改进包括：
*   **增强安全性**：通过密码加密保护数据库，敏感数据进行内存粉碎（RAM Shredding），以及不活动时自动锁定。
*   **多设备支持**：能够将多个设备配对到一个账户。
*   **注重隐私的通知**：集成UnifiedPush，实现非谷歌的通知系统。
*   **Tor支持**：通过SOCKS代理和Orbot提供Tor连接。
*   **美学定制**：包含一个遵循设备调色板的Material You主题。

Molly被定位为一个不断发展的应用程序，并计划推出更多新功能。它可在GitHub上下载，并鼓励用户捐赠以支持其开发。

---

## 12. 性感回归。网络监控扼杀了情色。

**原文标题**: Bringing Sexy Back. Internet surveillance has killed eroticism

**原文链接**: [https://lux-magazine.com/article/privacy-eroticism/](https://lux-magazine.com/article/privacy-eroticism/)

文章《重拾性感：互联网监控扼杀了情色》认为，由企业和国家行为者共同推动的无处不在的互联网监控，从根本上扼杀了情色繁荣所必需的条件。作者杰西卡·菲耶尔德提出，情色不仅仅是性，它还包含风险、脆弱、亲密以及未知带来的刺激——这些要素都需要一个私密的、未受观察的空间。

监控通过确保几乎所有数字和许多物理互动都受到持续监控和记录，从而侵蚀了这一至关重要的隐私。这种无处不在的凝视造成了一种寒蝉效应，导致个人出于对曝光、数据泄露或个人信息武器化的恐惧而进行自我审查。隐私的丧失扼杀了自发性和真实的脆弱性，而这些正是情色连接的核心。此外，欲望的算法商业化预测并包装了偏好，用商品化的解决方案取代了有机的、个性化的发现。这净化并剥离了对情色至关重要的不可预测的、“禁忌”的方面。

从历史上看，情色总是在自由和部分隐秘的空间中繁荣，远离权威的审视。该文章总结认为，重新获得隐私并积极抵制无处不在的监控是重振情色的关键步骤，使脆弱、风险和未知能够再次蓬勃发展，不受持续观察和算法控制。

---

## 13. 大公司里，好工程师如何写出烂代码

**原文标题**: How good engineers write bad code at big companies

**原文链接**: [https://www.seangoedecke.com/bad-code-at-big-companies/](https://www.seangoedecke.com/bad-code-at-big-companies/)

本文探讨了大型科技公司中，有能力的工程师却产出令人惊讶的糟糕代码这一悖论。主要原因是工程师频繁的流动和内部调动；由于薪酬结构，工程师往往只在公司停留1-2年，而频繁的组织重构又让他们在不同团队和代码库间辗转。这意味着许多代码修改是由不熟悉特定系统甚至编程语言的“新手”完成的，而这些代码库却往往已有十年甚至更久的历史。

尽管“老手”（拥有深厚系统知识的资深工程师）可以协助代码审查，但他们的支持往往是非正式的，且通常工作量过大，无法在不牺牲自身产出的情况下发现所有问题。“普通高效工程师”能力很强，但通常对当前代码库不熟悉，或者需要同时处理大量截止日期，这导致他们写出的临时性解决方案在快速审查后便被发布。

作者认为，这是大型科技公司有意识的权衡。公司优先考虑的是“内部可理解性”——即能够将工程师视为可互换的资源，并迅速调动他们去解决眼前的问题（例如，人工智能转型）——而非培养深厚的长期专业知识和代码质量。这种系统性选择迫使工程师从事“不纯粹的工程”，在压力下处理不熟悉的项目，使得不尽如人意的代码成为必然结果。

最终，文章总结道，将问题归咎于单个工程师是错误的。根本原因是组织动态，这种动态迫使即使是高技能专业人士也持续在不熟悉的代码库中工作，从而创造了一个“糟糕”代码是系统性而非个人失败的环境。

---

## 14. 你是不是想搭建本地 RAG？

**原文标题**: So you wanna build a local RAG?

**原文链接**: [https://blog.yakkomajuri.com/blog/local-rag](https://blog.yakkomajuri.com/blog/local-rag)

本文详细介绍了Skald在构建一个完全可自托管、保护隐私的RAG（检索增强生成）系统方面的努力，该系统无需将数据发送给第三方即可运行。这包括用本地开源替代方案取代RAG核心组件——向量数据库、嵌入模型、大型语言模型（LLM）、重排序器和文档解析——的专有SaaS解决方案。

Skald当前的本地技术栈使用带有pgvector的Postgres作为向量数据库，可配置的Sentence Transformers（例如all-MiniLM-L6-v2、bge-m3）用于生成嵌入，用户自行管理的开源LLM（已使用GPT-OSS 20B进行测试），可配置的Sentence Transformers交叉编码器（例如ms-marco-MiniLM-L6-v2、mmarco-mMiniLMv2-L12-H384-v1）用于重排序，以及Docling用于文档解析。

针对PostHog网站数据集进行的基准测试显示：
1. **Voyage AI + Claude Sonnet 3.7（专有）：** 性能卓越，得分9.45。
2. **Voyage AI + GPT-OSS 20B（混合）：** 非常出色，得分9.18，展示了强大的开源LLM能力。
3. **完全本地化（默认Sentence Transformers）：** 对于英语点查询表现尚可（7.10），但在非英语查询和聚合任务上失败。
4. **完全本地化（多语言bge-m3嵌入 + mmarco-mMiniLMv2-L12-H384-v1重排序器）：** 非常出色（8.63），能够处理多语言查询，但仍难以聚合多个文档中的信息。

作者总结认为，完全本地化的RAG是可行的，在许多用例中表现良好，并且正在持续改进。Skald计划进一步完善并进行更具说服力的基准测试。

---

## 15. A16Z的重磅论断

**原文标题**: A Remarkable Assertion from A16Z

**原文链接**: [https://nealstephenson.substack.com/p/a-remarkable-assertion-from-a16z](https://nealstephenson.substack.com/p/a-remarkable-assertion-from-a16z)

Neal Stephenson的文章讨论了Andreessen Horowitz (A16Z) 的合伙人Scott Kupor关于建立“全栈AI”公司可行性所做出的“一个显著论断”。Kupor的论断在a16z的一份通讯中被强调，他认为在AI领域有效整合硬件和软件具有挑战性，这导致难以创建具有防御性的全栈公司。他认为，现成硬件的成本效益和快速演进使其成为AI公司主要专注于软件的更好策略。

Stephenson结合他在物理工程方面的经验以及他的小说《终结冲击》，发现这一论断与直觉相悖，并可能令人担忧。他指出，纵观历史，基础性的技术变革，如蒸汽机或计算，往往需要硬件和软件（或其等价物）的深度整合，才能实现突破性性能和竞争优势。他暗示，A16Z作为一家主要的风险投资公司，可能淡化这种整合的重要性，这可能反映了风险投资界与AI领域真正、长期创新所必需的基础工程挑战之间存在脱节，尤其是在考虑物理世界时。他认为，这种观点可能忽视了源于“深层软硬件协同设计”的真正技术突破的潜力。

---

## 16. 芬兰将开建250兆瓦时“沙电池”

**原文标题**: 250MWh 'Sand Battery' to start construction in Finland

**原文链接**: [https://www.energy-storage.news/250mwh-sand-battery-to-start-construction-in-finland-for-both-heating-and-ancillary-services/](https://www.energy-storage.news/250mwh-sand-battery-to-start-construction-in-finland-for-both-heating-and-ancillary-services/)

极夜能源公司与芬兰拉赫蒂能源公司正在合作，在芬兰瓦克斯建造一座250兆瓦时（MWh）的“沙子电池”热能储存（TES）系统。该项目将成为全球最大的沙基热储能项目，拥有2兆瓦的供热功率和125小时的储存容量。

建设工作计划于2026年初开始，预计于2027年夏季完工。“沙子电池”将主要向拉赫蒂能源公司的区域供热网络供热，每年可大幅减少约60%的化石燃料排放（减少80%的天然气使用）。其相当大的规模也使其能够参与芬兰电网公司Fingrid的备用和电网平衡市场，提供重要的辅助服务。

该技术包括用电加热当地采购的天然沙，储存热量，然后将其释放用于供热。此前，极夜能源公司已于今年早些时候为另一家能源公司成功部署了一台使用皂石的1兆瓦/100兆瓦时沙子电池。拉赫蒂能源公司为此项目获得了芬兰商业局的资助，旨在提供负担得起的、可再生的区域供热并支持电网稳定。

---

## 17. 软件开发者的忏悔录：不再自我审查

**原文标题**: Confessions of a Software Developer: No More Self-Censorship

**原文链接**: [https://kerrick.blog/articles/2025/confessions-of-a-software-developer-no-more-self-censorship/](https://kerrick.blog/articles/2025/confessions-of-a-software-developer-no-more-self-censorship/)

Kerrick Staley 的文章《一个软件开发者的自白：不再自我审查》是作者一份个人声明，旨在放弃在职业和公共交流中的自我审查。Staley 反思了他长期以来过滤思想、观点和经验的习惯，尤其是那些可能被视为有争议、非传统或仅仅是不够完善的内容。

他将这种自我设限归因于多种因素，包括渴望显得能干、避免批评或遵从被普遍认同的职业规范。然而，他现在认为这种习惯是有害的，导致了真实性的丧失、创造力的扼杀以及错失了建立真正联系和进行更深入讨论的机会。

Staley 声明他打算更开放地分享自己的观点，即使这些观点尚未成熟、不尽完美，或者挑战现状。这包括表达挫折、讨论非传统方法以及揭示软件开发中凌乱的现实。他的目标是促进更真诚的对话、更有效地学习，并最终为建立一个更透明、更以人为本的科技社区做出贡献。这篇文章既是作者的个人承诺，也是邀请他人拥抱类似真诚的呼吁。

---

## 18. 荷兰大学能否摆脱微软？

**原文标题**: Can Dutch universities do without Microsoft?

**原文链接**: [https://dub.uu.nl/en/news/can-dutch-universities-do-without-microsoft](https://dub.uu.nl/en/news/can-dutch-universities-do-without-microsoft)

我很抱歉，但是文章内容缺失了。您提供的文本只写着“HOP”。请提供完整的文章，以便我为您总结。

---

## 19. 系统 7 在 Mac mini G4 上原生启动。

**原文标题**: System 7 natively boots on the Mac mini G4

**原文链接**: [https://macos9lives.com/smforum/index.php?topic=7711.0](https://macos9lives.com/smforum/index.php?topic=7711.0)

“Mac OS 9 Lives”论坛上的一篇帖子宣布了一项重大成就：System 7 已成功在 Mac mini G4 上原生启动。这篇题为“System 7 在 Mac mini G4 上原生启动！”的帖子由用户 RonsCompVids 于2025年11月29日在“非官方硬件上的 Mac OS 9”板块发布。

这一进展彰显了社区持续努力，旨在非官方支持的硬件上运行经典 Mac 操作系统。该帖子已获得巨大关注，浏览量达 49,381 次。这似乎是之前讨论的延续或相关内容，例如2025年11月27日的“Mac OS 9 在 Mac mini G4 上启动：详细帖子”，表明了社区正齐心协力，将经典 Mac OS 的兼容性扩展到 Mac mini 等更晚期的 G4 时代机器上。

---

## 20. 艾尔隆 – 3D 飞行追踪器

**原文标题**: Airloom – 3D Flight Tracker

**原文链接**: [https://objectiveunclear.com/airloom.html](https://objectiveunclear.com/airloom.html)

Airloom是一款三维飞行追踪应用程序，旨在三维环境中可视化飞行路径。用户可以通过搜索机场、使用当前位置或定义搜索半径来定位航班，并能查看实时飞机数量。

界面提供广泛的导航功能，包括沉浸式“飞行模式”（WASD控制），用于在三维空间中移动、重置视图以及清除飞行轨迹。“航班追踪”允许用户追踪特定飞机，并配有便于选择的“浏览模式”。显示设置高度可定制，包括轨迹长度、粗细、颜色（按速度或高度）以及机场/城市标签的可见性。

提供多种地图图层，从卫星图、线框图到三维视图，并可选择显示边界、GPS海拔以及具有可调不透明度的详细空域分类（B、C、D类）。数据设置包括可定制的更新速率和强大的飞机过滤器，可根据呼号、类型和高度进行筛选。

一个关键功能是“录制与回放”系统，用户可以通过时间轴和可变速度来启动、保存、加载和回放飞行数据。高级设置提供对高度比例、雾距离、地图亮度、线框密度和配色方案的精细控制，确保高度个性化和交互式的飞行追踪体验。

---

## 21. 可能吞噬辐射的切尔诺贝利神秘黑真菌

**原文标题**: The mysterious black fungus from Chernobyl that may eat radiation

**原文链接**: [https://www.bbc.com/future/article/20251125-the-mysterious-black-fungus-from-chernobyl-that-appears-to-eat-radiation](https://www.bbc.com/future/article/20251125-the-mysterious-black-fungus-from-chernobyl-that-appears-to-eat-radiation)

Nelli Zhdanova在切尔诺贝利核废墟中发现了一种神秘的黑色真菌，它表现出一种独特的趋向电离辐射生长的能力，这种现象被称为“趋辐射性”。这些真菌富含黑色素，这种色素最初被认为可以保护它们免受有害辐射。

Ekaterina Dadachova的进一步研究提出，这些含黑色素的真菌不仅保护自身，还能主动将辐射能转化为可用于生长的能量，这一过程被称为“辐射合成”。她的研究表明，含黑色素的真菌在放射性环境中生长更快，这暗示了一种潜在的新的生命基础。

同样的真菌菌株——*球形枝孢菌*（*Cladosporium sphaerospermum*），后来被送往国际空间站，在那里它在银河宇宙射线的存在下生长得更快，并展现出显著的辐射阻挡能力。这为太空探索开辟了激动人心的可能性。科学家设想利用这些真菌为未来的月球和火星基地建造自我再生的“真菌建筑”，为宇航员提供轻质、耐用的宇宙射线防护罩，从而无需从地球运输笨重的传统屏蔽材料。

---

## 22. 冰岛将洋流不稳定列为国家安全风险

**原文标题**: Iceland declares ocean-current instability a national security risk

**原文链接**: [https://edition.cnn.com/2025/11/15/climate/iceland-warming-current-amoc-collapse-threat](https://edition.cnn.com/2025/11/15/climate/iceland-warming-current-amoc-collapse-threat)

冰岛做出了前所未有的举动，将大西洋经向翻转环流（AMOC）——一个重要的洋流系统——的潜在崩溃定性为国家安全风险。这一决定源于越来越多的证据表明，AMOC（它将暖水输送到北方并维持冰岛相对温和的气候）正因全球变暖而减缓。

科学家们认为AMOC崩溃是“最可怕的潜在气候影响”之一。对于冰岛而言，AMOC的停止将意味着严重的区域降温、更频繁的暴风雨以及周围海冰的增加，这将对基础设施、交通以及渔业等重要产业造成毁灭性打击。约翰·帕尔·约翰逊部长称其为对国家气候、经济和安全的“生存威胁”。

在最近的研究强调了对AMOC稳定性的“严重担忧”之后，冰岛国家安全委员会于9月正式做出了这一认定。这引发了高层、协调一致的政府应对措施，以了解并减轻这一威胁。虽然崩溃的确切时间尚不确定，但一些研究预测它可能发生在本世纪，专家们表示这不再是低可能性风险。

科学家们赞扬冰岛的积极立场，敦促其他国家效仿，因为AMOC崩溃的全球影响将是灾难性的，包括海平面上升、季风紊乱以及欧洲范围内的严冬。冰岛的决定标志着一个重大转变，认识到这种剧烈的气候变化可能导致无法适应，使其成为“国家生存和安全的问题”。

---

## 23. 被低估的感恩理由 V

**原文标题**: Underrated reasons to be thankful V

**原文链接**: [https://dynomight.net/thanks-5/](https://dynomight.net/thanks-5/)

文章《被低估的感恩理由 V》罗列了在生物学、技术、社会和物理学等领域中常被忽视的种种福分。

理由包括狗的真挚爱意、有性生殖在促进复杂生命基因变异方面的演化成功，以及最终治愈普通感冒的潜力。文章对传染病控制方面的进展表示感谢，指出尽管城市化进程加快，但凭借卫生设施、疫苗和新兴对策，病原体仍得到了有效管理。充足的清洁水、现代牙科，乃至舌头的简单功用等基本便利也备受赞扬。

放射性原子独特的、其环境影响大多是自我限制的特性，以及经证实旨在治愈重大疾病、有望带来非线性预期寿命增长的努力，都得到了提及。过氧化物酶等生物学奇迹，以及提供重要“重置”功能的睡眠的恢复力也受到了认可。

社会层面的感恩涵盖了航空旅行的安全性、金融市场通常更为可靠的乐观情绪，以及社会支持父母的功能性共识。民主和公民自由在历史上罕见但日益普及，这带来了希望。一些抽象概念，例如个人偏好促进幸福，以及将五维光场存储在二维胶片上（全息术）背后的深奥物理学，也都是值得赞赏的理由。甚至一次性塑料，若管理得当，其便利性和碳固存潜力也得到了认可。最后，生活在三维空间中的基本福祉，避免了进食时身体分裂的情况。

---

## 24. 空客要求改装6000架飞机 航班面临中断预警

**原文标题**: Flight disruption warning as Airbus requests modifications to 6k planes

**原文链接**: [https://www.bbc.com/news/live/cvg4y6g74ert](https://www.bbc.com/news/live/cvg4y6g74ert)

空客已发布警告称，因强制要求超过6000架飞机（主要为空客A320机型）立即进行软件更新，航班可能中断。问题的根源在于发现飞机计算机易受强烈太阳辐射的干扰，这可能损坏控制飞机高度的数据。去年10月，一架捷蓝航空飞机经历“高度骤降”后，这一脆弱性才浮出水面，该事件现已被归因于太阳辐射。所需的修改导致大量航班取消，尤其是在一个主要的假日周末期间影响了美国。美国航空、达美航空、捷蓝航空和联合航空这四家美国主要的A320运营公司都在受影响之列。虽然全球各地都有航班取消的报告，但迄今为止，英国机场的航班中断相对有限。

---

## 25. 笨蛋，永远是过程。

**原文标题**: It's Always the Process, Stupid

**原文链接**: [https://its.promp.td/its-always-the-process-stupid/](https://its.promp.td/its-always-the-process-stupid/)

文章指出，人工智能并非解决企业低效问题的“灵丹妙药”；相反，它只是加速了现有流程，无论好坏。不存在所谓的“AI战略”，只有业务流程优化（BPO）。人工智能，如同过去的科技变革一样，主要让任务变得*更快*，而非本质上更智能，自动化一个有缺陷的流程只会加速“垃圾”的产生。

人工智能的独特能力在于处理非结构化数据（如电子邮件、PDF文件），这是过去由人类管理的领域。然而，依赖此类数据的流程本身往往是无结构且未被记录的。为了使人工智能有效，这些“隐藏”的工作流必须首先被揭示出来，并通过明确定义触发器、转换（AI提取什么）和结构化输出进行设计和构建。

尽管人工智能擅长快速模式匹配，但人类智能和治理对于真正的理解和背景仍然至关重要。企业应优先绘制并优化其价值链，特别是那些混乱的、以人为中心的流程。只有在建立了精简、逻辑化的流程之后，才能应用人工智能来加速它们，因为“关键始终在于流程本身”。企业人工智能采纳的困境，部分源于AI工具在开发时并未秉持这种“业务流程优化优先”的理念。

---

## 26. DeepSeekMath-V2: 迈向自验证数学推理 [pdf]

**原文标题**: DeepSeekMath-V2: Towards Self-Verifiable Mathematical Reasoning [pdf]

**原文链接**: [https://github.com/deepseek-ai/DeepSeek-Math-V2/blob/main/DeepSeekMath_V2.pdf](https://github.com/deepseek-ai/DeepSeek-Math-V2/blob/main/DeepSeekMath_V2.pdf)

本文介绍了DeepSeek AI的一个项目DeepSeekMath-V2，该项目专注于提升人工智能的数学推理能力。正如其名称“迈向自验证数学推理”所暗示的，它的显著特点在于它不仅能解决数学问题，还能自主验证其解决方案的正确性。这旨在提升人工智能生成的数学输出的可靠性和可信度，解决了该领域的一个关键挑战。

这项工作的详细内容已在一篇研究论文中发表（标记为“[pdf]”）。该项目以 `deepseek-ai/DeepSeek-Math-V2` 的形式托管在GitHub上，是公开的，并吸引了社区的广泛关注，获得了1k星标和53个分支。这表明它在开发用于复杂数学任务的更强大、更可靠的人工智能系统方面做出了显著贡献。

---

## 27. 每个数学家都只有那几招 (2020)

**原文标题**: Every mathematician has only a few tricks (2020)

**原文链接**: [https://mathoverflow.net/questions/363119/every-mathematician-has-only-a-few-tricks](https://mathoverflow.net/questions/363119/every-mathematician-has-only-a-few-tricks)

Gian-Carlo Rota断言“每个数学家都只有少数几个技巧”，这引发了一场关于这些反复出现的技巧可能是什么的社区讨论。尽管一些用户争论Rota的观点指的是普遍适用的方法还是高度个性化的方法，仍有几个共同的“技巧”被识别出来。

一个常被引用的技巧是**交换求和或积分的顺序**，这通常被视为Fubini定理或Gelfand更广义的重新索引版本的强大应用。另一个关键策略是**修改问题**：要么通过简化问题来证明一个更易于理解的版本（归因于Polya和Hilbert），要么通过添加参数来推广问题以揭示更深层的结构（例如Macdonald多项式）。

其他被强调的技巧包括：
*   **不等式**的基本应用，例如三角不等式。
*   **分部积分法**的多功能性，以其在分析学中的深远影响而闻名。
*   **抽屉原理**，或其实数等价形式（最大值至少等于平均值）。
*   Erdős所倡导的**概率方法**，包括“尝试一个随机对象”来证明存在性。
*   利用**莫比乌斯 $\mu$ 函数**作为容斥原理的更优雅替代。
*   在**连通域上的连续、取整数值的函数必定是常数**的原理。

讨论表明，尽管数学家拥有渊博的知识，但他们最有效的解决问题方法往往源于一套简洁、适应性强的核心技巧。

---

## 28. 领英很喧嚣，职场是地狱

**原文标题**: LinkedIn is loud, and corporate is hell

**原文链接**: [https://ramones.dev/posts/linkedin-is-loud/](https://ramones.dev/posts/linkedin-is-loud/)

文章《领英喧嚣，职场如狱》批判领英是一个“表演性地狱”，也是现代职场虚伪的缩影。作者将该平台描述为一个个人“表演工作”而非真正投入工作的场所，充斥着持续不断的凡尔赛式炫耀、职场黑话、遮掩不住的广告，以及一种无处不在的压力，要求人们保持“永远在线”的专业人设。

该文认为，领英充分体现了当代职场文化的肤浅与虚伪。它突出强调了姿态性盟友关系的例子，比如企业采纳社会正义议题，却不进行实质性内部改革；以及普遍要求员工展现出虚假的激情和生产力形象。这种在“个人品牌”和肤浅社交驱动下的环境，迫使个人持续处于表演状态，导致筋疲力尽，并让人感觉自己像个“职场傀儡”。

最终，作者对领英无法培养真诚的人际关系或提供超越肤浅求职与社交的真正价值表达了深刻的幻灭。它只优先考虑外在表现，而非实质性的专业投入。这是对职场表演性那种令人筋疲力尽、往往毫无意义的本质的尖锐批判。

---

## 29. 科技巨头储备数百万美元“战争基金”对抗AI监管

**原文标题**: Tech Titans Amass Multimillion-Dollar War Chests to Fight AI Regulation

**原文链接**: [https://www.wsj.com/tech/ai/tech-titans-amass-multimillion-dollar-war-chests-to-fight-ai-regulation-88c600e1](https://www.wsj.com/tech/ai/tech-titans-amass-multimillion-dollar-war-chests-to-fight-ai-regulation-88c600e1)

无法访问文章链接。

---

## 30. AI采纳率开始趋于平稳

**原文标题**: AI Adoption Rates Starting to Flatten Out

**原文链接**: [https://www.apolloacademy.com/ai-adoption-rates-starting-to-flatten-out/](https://www.apolloacademy.com/ai-adoption-rates-starting-to-flatten-out/)

2025年11月28日，阿波罗首席经济学家托斯滕·斯洛克报告称，各种规模企业的人工智能采用率开始趋于平稳。这一趋势是基于美国人口普查局和Ramp AI指数的数据。

Ramp AI指数衡量美国企业对人工智能产品和服务的采用率。它通过Ramp的企业卡和账单支付平台，收集了来自超过40,000家美国企业的数据以及数十亿美元的企业支出信息。所报告的数据代表六次调查的移动平均值，这些调查是每两周进行一次的。这表明企业整合人工智能技术的速度可能达到了一个平台期。

---

## 31. 斯泰兰蒂斯用新车折扣弹窗广告刷爆车主屏幕。

**原文标题**: Stellantis Is Spamming Owners' Screens with Pop-Up Ads for New Car Discounts

**原文链接**: [https://www.thedrive.com/news/stellantis-is-spamming-owners-screens-with-pop-up-ads-for-new-car-discounts](https://www.thedrive.com/news/stellantis-is-spamming-owners-screens-with-pop-up-ads-for-new-car-discounts)

Stellantis因在车主车载屏幕上直接显示推广新车折扣的弹窗广告而受到大量批评。吉普车主Zerin Dube和Stellantis公司本身都证实了这一做法，在网上引发了众怒，用户称之为“令人厌恶”和“晚期资本主义”。吉普、Ram和克莱斯勒车车主报告收到了这些广告，许多人发誓再也不会购买这些品牌的汽车。这不是第一次发生此类事件，Stellantis此前曾使用类似的弹窗广告推广延长保修服务，同样引来了不满。

Stellantis为目前的1500美元忠诚奖金优惠辩护，称其是“在关键时刻与车主保持联系”的一种方式，并指出该系统还会发送重要的召回和健康警报。他们声称营销信息被设计成侵扰性最小：只在启动时和车辆静止时显示，当车辆移动、15秒后或用户解除时便会消失。它们只在选择“稍后提醒”或被忽略时才会再次出现。

尽管遭到强烈反对，但这些广告可能有效；最初发帖抱怨弹窗广告的Zerin Dube最终购买了一辆享受大幅折扣的新款吉普牧马人，其中包括1500美元的忠诚奖金。Stellantis证实，车主可以通过联系其客户服务热线永久选择退出车载信息推送。这种做法凸显了广告与网联汽车技术日益融合的趋势，尤其是在Stellantis旨在竞争中提高销量之际。

---

## 32. 查尔斯·M·舒尔茨如何创作查理·布朗和史努比 (2024)

**原文标题**: How Charles M Schulz created Charlie Brown and Snoopy (2024)

**原文链接**: [https://www.bbc.com/culture/article/20241205-how-charles-m-schulz-created-charlie-brown-and-snoopy](https://www.bbc.com/culture/article/20241205-how-charles-m-schulz-created-charlie-brown-and-snoopy)

查尔斯·M·舒尔茨，标志性漫画《花生漫画》（以查理·布朗和史努比为主角）的创作者，50年来亲自绘制了每一幅漫画，直到1999年末因病退休，不久后于2000年2月去世。尽管建立了一个全球数十亿美元的帝国，舒尔茨却谦逊地将自己的作品描述为处理“日常小问题”，例如能力不足感，而非宏大的社会议题。然而，他强调，这些看似渺小的主题——爱、恨、不信任、恐惧和不安全感——却具有深远的意义。

《花生漫画》在全球引起共鸣，通过可产生共鸣的“永恒的失败者”查理·布朗，传达了普遍的情感。翁贝托·埃科指出它既能吸引儿童，也能征服阅历丰富的成年人。舒尔茨承认，他最初关注儿童是出于商业考量，因为编辑们更喜欢儿童题材，而且他从狗和孩子之间的互动中找到了灵感，这为他的想法提供了一个多功能的“剧团”。

舒尔茨性格内向，通过函授学习艺术，认为自己的背景非常适合漫画创作。他始终专注于画“一些有趣的东西”，不断创作漫画，当灵感涌现时，他常常感到兴奋。舒尔茨始终坚信《花生漫画》会成功。

1999年12月14日，他宣布因癌症退休，他创作的最后一篇日报漫画于2000年1月3日刊登，而他最后一篇周日漫画则在他去世后的第二天发布。舒尔茨的遗产包括一份感恩的信息，以及通过查理·布朗传达的“坚持不懈，永不放弃”的持久教训。

---

## 33. 禽流感病毒耐热，使其对人类构成重大威胁。

**原文标题**: Bird flu viruses are resistant to fever, making them a major threat to humans

**原文链接**: [https://medicalxpress.com/news/2025-11-bird-flu-viruses-resistant-fever.html](https://medicalxpress.com/news/2025-11-bird-flu-viruses-resistant-fever.html)

无法访问文章链接。

---

## 34. 比利时警方被曝利用僵尸网络操纵欧盟数据法影响评估

**原文标题**: Belgian Police exposed using botnets to manipulate EU data law impact assessment

**原文链接**: [https://old.reddit.com/r/europe/comments/1p9kxhm/belgian_federal_police_forgot_to_turn_their_vpn/](https://old.reddit.com/r/europe/comments/1p9kxhm/belgian_federal_police_forgot_to_turn_their_vpn/)

2013年10月的一篇Reddit帖子，标题为“比利时联邦警察被曝使用僵尸网络操纵欧盟数据法影响评估”，详细描述了对比利时联邦警察（BFP）的指控。BFP被指控在一次关于数据保留政策的欧盟公众咨询中搞“伪草根运动”。

该帖子称，BFP向欧盟委员会关于数据保留的影响评估提交了多条评论。这些评论被包装成来自不同“公民”的意见，一致主张强制数据保留并反对端到端加密。据报道，当与这些评论相关的IP地址被追溯到比利时联邦警察使用的一家VPN服务商时，这一欺骗行为才被发现。作者声称，警方“忘记关闭他们的VPN”，尽管试图掩盖评论来源，但仍有效地暴露了其机构起源。

该事件被定性为比利时国家通过欺骗性手段操纵公众舆论并影响欧盟数据保护立法的一次尝试，类似于“国家资助的宣传”。作者使用“僵尸网络”等词语来描述这些协调一致、数量众多的提交，暗示这是一种系统性的努力，旨在为其在数据保留问题上的立场制造虚假的基层支持。

---

## 35. Yggdrasil网络上的真P2P邮件

**原文标题**: True P2P Email on Top of Yggdrasil Network

**原文链接**: [https://github.com/JB-SelfCompany/Tyr](https://github.com/JB-SelfCompany/Tyr)

Tyr是一款安卓应用，通过利用Yggdrasil网络提供真正的点对点（P2P）电子邮件服务。它挑战了传统的基于服务器的电子邮件模式，该模式容易遭受监视、审查和元数据泄露。Tyr通过实现设备间的直接通信来规避这些问题，而无需中心化邮件服务器、独立的加密层（因为Yggdrasil提供网络层加密）或复杂的NAT穿透设置。

该应用直接在安卓设备上运行一个完整的SMTP/IMAP服务器，使其兼容标准电子邮件客户端。它与DeltaChat和ArcaneChat等去中心化即时通讯工具无缝集成，这些工具被推荐用于获得最佳P2P消息体验。每次Tyr安装都会生成一个唯一的Ed25519加密密钥，形成一个可验证的`<64-十六进制字符>@yggmail`地址，从而防止身份欺骗。

主要功能包括聊天应用的自动配置、加密备份、精密的电源管理和自动启动功能。安全性内置其中，利用安卓密钥库、Yggdrasil的网络加密以及邮件端口的仅限本地访问。Tyr倡导规避审查、设计层面隐私（无元数据或服务器日志）和真正的去中心化，提供了一个弹性且私密的电子邮件解决方案。

---

## 36. SQLite 作为应用程序文件格式

**原文标题**: SQLite as an Application File Format

**原文链接**: [https://sqlite.org/appfileformat.html](https://sqlite.org/appfileformat.html)

文章《将 SQLite 用作应用程序文件格式》倡导使用 SQLite 数据库文件来存储应用程序状态，并将其视为传统应用程序文件格式的更优替代方案。文章首先将“应用程序文件格式”定义为存储多个对象及其关系（例如 EPUB、DOC）的格式，以区别于存储单个对象（例如 JPEG）的更简单的“文件格式”。

现有应用程序文件格式分为：
1.  **全定制格式：** 二进制、不透明（例如 PDF），需要专门工具。
2.  **文件堆格式：** 使用文件系统作为键/值存储（例如 Git），可访问但移动不便。
3.  **封装文件堆格式：** 将文件堆封装在单个归档文件（如 ZIP）中（例如 EPUB、ODT），是可访问性和单文件便利性之间的折衷。

文章提出将 SQLite 作为“第四类”格式，提供以下引人注目的优势：
*   **简化应用程序开发：** 减少代码量，利用健壮且经过验证的库。
*   **单文件文档：** 保留“文档隐喻”，易于管理和共享。
*   **高级查询语言 (SQL)：** 简化数据访问，侧重于“需要什么”信息。
*   **可访问内容：** 不是不透明的二进制数据块；内容可通过常见的开源工具读取，确保长期可用性。
*   **跨平台：** 跨不同系统和架构可移植。
*   **原子事务：** 确保数据在崩溃和断电情况下的完整性。
*   **增量和连续更新：** 仅写入更改的数据，提高性能并防止数据丢失。
*   **易于扩展：** 可以通过修改模式添加新功能，而不会破坏向后兼容性。
*   **性能：** 通常比其他格式更快，尤其是通过选择性加载数据来加速应用程序启动。

因此，SQLite 为应用程序数据提供了一个多功能、结构化且可靠的容器，超越了其他方法的性能和便利性。

---

## 37. 你工作时无法专注的数学

**原文标题**: The Math of Why You Can't Focus at Work

**原文链接**: [https://justoffbyone.com/posts/math-of-why-you-cant-focus-at-work/](https://justoffbyone.com/posts/math-of-why-you-cant-focus-at-work/)

这篇题为《你为何无法在工作中专注的数学原理》的文章，提出了一个数学模型，旨在解释工作场所普遍存在的专注力下降现象，超越了轶事性的观察。它识别出决定日常生产力的三个关键参数：

1.  **λ (lambda)：** 中断率（每小时中断次数），被建模为泊松过程，指示员工专注力被打断的频率。
2.  **Δ (delta)：** 恢复时间（分钟），即每次中断后重新集中精力所需的时间，在此期间实际生产力为零。
3.  **θ (theta)：** 专注阈值（分钟），即进行有意义的深度工作所需的最小不间断时间块。

这“三个旋钮”的相互作用决定了一天进行实际工作的“容量”，计算公式为`C(θ) = Σ⌊di/θ⌋`。该公式中的向下取整函数（`⌊x⌋`）揭示了，即使零碎的工作时间块总计很长时间，如果它们低于`θ`阈值，仍会大幅降低实际生产力产出。

文章通过可视化方式展示了典型的“浪费日”与“高效日”，并模拟了λ、Δ和θ在不同条件下的数百个工作日，以阐明它们对深度工作时间块的影响。该模型以现实世界的研究为基础，引用了显示现代工作中惊人高中断率（例如，对于高频合作者来说，每2-3分钟一次）和大量恢复时间（10-16分钟）的研究。其目的是提供一个可量化的框架，以理解并解决保持专注力的挑战。

---

## 38. 维索拉约顿-8 5纳米欧洲推理芯片

**原文标题**: Vsora Jotunn-8 5nm European inference chip

**原文链接**: [https://vsora.com/products/jotunn-8/](https://vsora.com/products/jotunn-8/)

Vsora Jotunn-8是一款5纳米欧洲推理芯片，被誉为“终极AI芯片”和“全球最高效AI推理芯片”，旨在实现突破性效率（以“0 /tflops”为佐证）。它专为现代数据中心设计，专注于以闪电般的速度、最低的成本和轻松的可扩展性部署训练好的AI模型。

主要特性和优势包括：
*   **超低延迟**：对聊天机器人、欺诈检测和搜索等实时应用至关重要。
*   **超高吞吐量**：对推荐引擎和大型语言模型API等高需求服务必不可少。
*   **高成本效益**：显著降低每次推理的成本，这对于规模化业务的生存能力至关重要。
*   **高能效**：最大限度地降低运营开支和环境影响。

Jotunn-8还强调性能、内存和灵活性，并致力于可持续性。它声称性能超越市场同类产品，特别提到了Llama3 405B。一个显著优势是其架构能够无缝集成不同类型的AI模型——推理模型、生成式AI（大型语言模型）和智能体AI——为构建更强大、更可靠的系统提供接近理论的性能。这将Jotunn-8定位为规模化AI的新基石，使AI投资发挥最大效益，同时降低运营成本。

---

## 39. 高空气污染可能使运动益处减半——研究

**原文标题**: High air pollution could diminish exercise benefits by half – study

**原文链接**: [https://scienceclock.com/exercise-may-protect-less-when-air-pollution-is-high-study-finds/](https://scienceclock.com/exercise-may-protect-less-when-air-pollution-is-high-study-finds/)

一项由伦敦大学学院共同主导的最新国际研究，分析了来自多个国家超过150万成年人的健康数据，揭示了高空气污染显著削弱运动对健康的益处。

研究人员关注细颗粒物（PM2.5），它可能在体内引起炎症和长期损害。虽然每周至少进行2.5小时的中等到剧烈运动通常可将死亡风险降低30%，但在年平均PM2.5超过25 μg/m³的地区，这种保护作用降至12–15%。在污染更严重的地区（PM2.5高于35 μg/m³，全球36%的人口居住在此类地区），这些益处进一步减弱，尤其是在降低癌症死亡率方面。

首席研究员顾博文教授强调，即使在污染环境中，运动仍然有益，但改善空气质量可以显著增强这些益处。合著者安德鲁·斯蒂普托教授强调，有毒空气会阻碍但不会消除运动益处，并强调控制污染对健康老龄化的必要性。

这项发表在《BMC医学》杂志上的研究指出，其数据主要来自高收入国家，这表明在低收入地区，影响可能更为严重。研究人员建议，与其劝阻户外运动，不如在污染日检查空气质量、选择更清洁的路线或降低运动强度。研究结果强调，清洁空气和定期运动对健康都至关重要，因此污染控制对我们的福祉至关重要。

---

## 40. 加菲尔德的勾股定理证明

**原文标题**: Garfield's Proof of the Pythagorean Theorem

**原文链接**: [https://en.wikipedia.org/wiki/Garfield%27s_proof_of_the_Pythagorean_theorem](https://en.wikipedia.org/wiki/Garfield%27s_proof_of_the_Pythagorean_theorem)

第20任美国总统詹姆斯·A·加菲尔德因其对勾股定理的原创证明而闻名，该证明于1876年他担任国会议员期间发表。他是唯一一位对原创数学做出贡献的美国总统，这一殊荣独一无二。他的证明发表在《新英格兰教育杂志》上，被历史学家誉为“非常巧妙”，并在收录了370种不同证明的《勾股定理命题》一书中被确认为第231个证明。

加菲尔德的证明利用了一个由三个直角三角形构成的梯形。从一个直角三角形ABC（边长为a、b，斜边为c）开始，他构造了第二个全等三角形BDE，使B点共享，且AB垂直于BD。连接点A和点D形成第三个三角形ABD。这三个三角形组合起来形成了梯形ACED。

该证明通过两种方式计算这个梯形的面积。首先，利用梯形面积公式（高 × 平行边平均值），面积被确定为 1/2 * (a + b) * (a + b)，其中CE = a+b 是高，AC = a 和 DE = b 是平行边。

其次，梯形的面积被计算为三个组成三角形的面积之和：三角形ACB (1/2 * ab)，三角形BDE (1/2 * ab)，以及三角形ABD (1/2 * c * c，因为它是一个等腰直角三角形，两条直角边均为c)。

将这两种面积表达式等同起来：1/2 * (a + b)^2 = 1/2 * ab + 1/2 * c^2 + 1/2 * ab。简化此方程得到 a^2 + 2ab + b^2 = 2ab + c^2，这进一步简化为勾股定理：a^2 + b^2 = c^2。

---

## 41. Django 新后台任务初探

**原文标题**: A first look at Django's new background tasks

**原文链接**: [https://roam.be/notes/2025/a-first-look-at-djangos-new-background-tasks/](https://roam.be/notes/2025/a-first-look-at-djangos-new-background-tasks/)

Django 6.0 引入了 `django.tasks`，一个内置的后台任务框架。其主要目的是为任务队列实现提供一个*通用API*，因为它*不包含用于任务执行的工作机制*，需要外部基础设施。任务使用 `@task` 装饰器定义，并且必须通过 `.enqueue()` 调用，以防止意外的进程内执行。该框架是极简主义的，缺少内置的重试或指数退避机制，但可以实现自定义逻辑。

本文详细介绍了如何构建一个自定义的数据库支持的任务后端和一个工作进程，因为 Django 6.0 仅提供 `ImmediateBackend`（立即执行）和 `DummyBackend`（不执行任何操作）。

自定义后端使用 `Task`、`Attempt` 和 `Error` 模型来存储任务元数据、执行尝试和异常。`Task` 模型通过 `available_after`（用于管理带退避的重试）、`attempt_count` 和 `worker_id`（用于任务认领）等字段进行了完善。`DatabaseBackend` 负责任务入队（创建 `Task` 记录）和结果检索。它支持每个队列可配置的 `max_attempts` 和 `backoff_factor`。

一个自定义的 `Worker` 持续轮询待处理的任务。它使用原子事务来 `claim_first_available` 任务，确保唯一性。后端随后通过执行可调用对象、记录尝试、捕获任何错误，并更新任务状态和 `available_after` 以进行后续重试来 `process_task`。这种设置展示了一个基于 `django.tasks` 构建的完整自定义后台任务解决方案。

---

## 42. 别拽那个，谁知道它连着什么呢？(2016)

**原文标题**: Don't tug on that, you never know what it might be attached to (2016)

**原文链接**: [https://blog.plover.com/2016/07/01/#tmpdir](https://blog.plover.com/2016/07/01/#tmpdir)

作者详细描述了一次调试经历，当时 `emacsclient` 突然停止工作，并报告“找不到套接字”。核心问题是一个不匹配：`emacsclient` 在 `/mnt/tmp/emacs2017/server` 中查找 Unix 域套接字，而 Emacs 则在 `/tmp/emacs2017/server` 中创建它。

调查显示，一个系统脚本将 `TMPDIR` 环境变量设置为 `/mnt/tmp` 是导致问题的原因。`emacsclient` 遵循此设置，但 Emacs 在直接启动时*也*遵循 `TMPDIR`，这导致了混淆。这种差异只在 Emacs 通过一个自定义 Perl 脚本（`git-re-edit`）间接启动时发生。

进一步的排查证明 Perl 本身从其进程中剥离了 `TMPDIR` 环境变量，这种行为在其他变量或不同系统上并未出现。文章最后指出，这并非一个 bug，而是动态加载器采取的一种微妙的安全措施，旨在防止 `TMPDIR` 被操纵以诱骗特权进程写入非预期位置的攻击。

实施了两种变通方案：配置 Emacs 使用 TCP 套接字，或者显式设置 `EMACS_SERVER_SOCKET` 环境变量并修改 `also` 脚本，以便将正确的 Unix 域套接字路径传递给 `emacsclient`。

---

## 43. 大型人工智能会议充斥着由AI撰写的同行评审

**原文标题**: Major AI conference flooded with peer reviews written by AI

**原文链接**: [https://www.nature.com/articles/d41586-025-03506-6](https://www.nature.com/articles/d41586-025-03506-6)

Pangram Labs公司最近的一项分析显示，2026年国际学习表征会议（ICLR）的同行评审过程中存在大量AI生成内容。最初，学术界人士（包括Graham Neubig在内）对此表示担忧，Graham Neubig曾收到“非常冗长”且模糊、带有虚构引用的反馈，这促使他寻求检测AI使用的工具。

Max Spero旗下的Pangram Labs随后扫描了所有19,490份提交的研究论文和75,800份同行评审。他们的发现令人震惊：大约21%的ICLR同行评审完全由AI生成，超过一半的评审报告包含AI使用迹象。该分析还发现1%（199篇）的稿件完全由AI生成，另有9%的稿件包含超过50%的AI生成文本。

这些结果证实了许多研究人员的怀疑，例如Desmond Elliott的论文就收到了一份完全由AI生成的评审报告的低分，该报告误解了内容并引用了错误的数值数据，这给他带来了极大的沮丧。ICLR高级项目主席Bharath Hariharan指出，这是该会议首次遇到如此大规模的AI使用情况。作为回应，组织者计划实施自动化工具，以强制执行投稿和评审中禁止使用AI的政策，旨在恢复对评估过程的信任。

---

## 44. 中国纯电动卡车和柴油主导地位的终结

**原文标题**: China's BEV trucks and the end of diesel's dominance

**原文链接**: [https://cleantechnica.com/2025/11/26/chinas-bev-trucks-and-the-end-of-diesels-dominance/](https://cleantechnica.com/2025/11/26/chinas-bev-trucks-and-the-end-of-diesels-dominance/)

中国电动重卡（BEV）正迅速崛起，成为全球货运业的一股颠覆性力量，其价格显著更低，且采用专用设计。在中国，配备400-600千瓦时电池的车型售价为5.8万至8.5万欧元。尽管它们需要约2万至4万欧元的升级以符合西方认证和驾驶员舒适度要求，但其短途运输到岸价为8万至12万欧元，远低于通常起价约25万欧元的西方电动重卡。

这种成本优势至关重要，因为欧洲的大部分货运（250公里以下）都是短途运输，而这些经济实惠的中国电动重卡非常适合这一细分市场。中国的重卡市场已发生剧变：电动重卡在新车销售中的占比从2024年的13%攀升至2025年初的22%，而柴油车的份额则暴跌至接近50%。相反，氢燃料电池卡车的占比仍低于1%，并因成本和运营挑战而呈下降趋势。

西方原始设备制造商（OEM）面临巨大压力，其中许多企业最初只是将柴油车底盘改装用于电动化。他们的传统设计和成本结构难以与中国批量生产的专用电动平台竞争。文章警告称，在更便宜的电动重卡所带来的经济逻辑推动下，货运脱碳转型正以超出预期的速度加速。对西方运营商和政策制定者而言，挑战在于适应这种新的成本曲线，并整合或应对中国已建立的电动卡车生态系统。

---

## 45. 内角和为零的三角形

**原文标题**: A triangle whose interior angles sum to zero

**原文链接**: [https://www.johndcook.com/blog/2025/11/28/tricusp-triangle/](https://www.johndcook.com/blog/2025/11/28/tricusp-triangle/)

文章对比了球面几何和双曲几何中的三角形性质。

在**球面几何**中，三角形的内角和总是大于π (180°)。在半径为1的球体上，这种三角形的面积是其“过量”(E)，定义为内角和减去π。一个例子是具有三个直角的三角形。

在**双曲几何**中，三角形的内角和总是小于π。在曲率为-1的空间中，其面积是其“亏格”(D)，计算方法是π减去内角和。两种几何都是局部欧几里得的，这意味着在这两种空间中，小三角形的内角和都接近于π。

文章随后描述了一个独特的双曲三角形，其内角和为零。这个“非正常”三角形，由三条双曲线（半圆）在实轴上的理想点相交形成，其最大可能面积为π。尽管其周长是无限的，但面积是有限的。构成该三角形的半圆半径不会改变其面积。虽然它严格来说位于双曲平面之外，但可以在双曲平面内任意接近它。

---

## 46. 最初的ABC语言，Python 的前身 (1991年)

**原文标题**: The original ABC language, Python's predecessor (1991)

**原文链接**: [https://github.com/gvanrossum/abc-unix](https://github.com/gvanrossum/abc-unix)

本文详细介绍了ABC编程语言，该语言被认为是Python最直接的前身。Python的创建者Guido van Rossum于1983年至1986年期间参与了ABC的开发工作，并被列为其作者之一。

ABC的源代码，大部分源于1991年，从cwi.nl（abc-unix tarball）获取，也存放在Luciano Ramalho的GitHub上，希望能统一这两个版本。目前编译该语言需要32位系统，未来计划将其更新以兼容64位系统。

ABC没有明确的开源许可证，但它带有Stichting Mathematisch Centrum（1988-2011）的版权。Guido van Rossum打算与Steven Pemberton协商获取MIT许可证。主要作者包括Eddy Boeve、Lambert Meertens、Steven Pemberton和Guido van Rossum。参考文献包括《The ABC Programmer's Handbook》（1990年）以及Steven Pemberton和Lambert Meertens探讨ABC设计及其起源的文章。

---

## 47. 苹果英特尔据传将合作Mac芯片

**原文标题**: Apple and Intel Rumored to Partner on Mac Chips

**原文链接**: [https://www.macrumors.com/2025/11/28/intel-rumored-to-supply-new-mac-chip/](https://www.macrumors.com/2025/11/28/intel-rumored-to-supply-new-mac-chip/)

供应链分析师郭明錤表示，据传苹果将与英特尔重燃合作，但合作模式将是全新的且有限的。尽管目前所有Mac都使用苹果定制设计的M系列芯片，但英特尔预计最早将于2027年中期开始生产苹果的最低端M系列芯片（可能是M6或M7）。

英特尔将利用其18A工艺（一种在北美制造的、低于2纳米的先进节点），为未来的MacBook Air、iPad Air和iPad Pro型号生产这些芯片。这与他们之前的合作模式有显著不同，因为英特尔将只协助生产苹果设计的基于Arm架构的芯片，而非设计x86芯片。

台积电仍将是苹果大部分M系列芯片的主要供应商。郭明錤认为，此举将有助于苹果分散其供应链，并与“美国制造”倡议保持一致，他提到了特朗普政府的偏好。

苹果于2020年开始在Mac上逐步淘汰英特尔处理器，其M系列芯片提供了行业领先的每瓦性能。macOS Tahoe被认为是支持基于英特尔Mac的最后一个主要版本。

---

## 48. 瑞典出版商对Meta扎克伯格报案，指控其欺诈。

**原文标题**: Swedish publishers file police report against Meta's Zuckerberg for fraud

**原文链接**: [https://www.sverigesradio.se/artikel/swedish-publishers-file-police-report-against-metas-zuckerberg-for-fraud](https://www.sverigesradio.se/artikel/swedish-publishers-file-police-report-against-metas-zuckerberg-for-fraud)

瑞典出版商协会已向警方报案，指控Meta创始人马克·扎克伯格犯有欺诈罪。

---

## 49. 万亿美元或将浪费在生成式AI上

**原文标题**: A trillion dollars (potentially) wasted on gen-AI

**原文链接**: [https://garymarcus.substack.com/p/a-trillion-dollars-is-a-terrible](https://garymarcus.substack.com/p/a-trillion-dollars-is-a-terrible)

在Gary Marcus的文章《一万亿美元（可能）浪费在生成式AI上》中，他认为在过去一年半中，投入到生成式AI领域的巨额投资，可能超过一万亿美元，但由于当前AI模型的基本局限性，这些投资可能大半付诸东流。

Marcus指出，虽然大型语言模型（LLMs）在生成文本和代码方面表现出色，但它们缺乏真正的理解、常识和可靠的推理能力。他强调了几个关键问题：
*   **事实性和幻觉：**LLMs经常“幻觉”出错误信息，使其在需要准确性的任务中不可靠。
*   **脆弱的推理能力：**它们难以进行复杂的推理，在人类看来微不足道的基本逻辑或算术问题上常常出错。
*   **缺乏因果理解：**当前模型是模式匹配器，而非因果推理器，这限制了它们真正理解世界或做出明智决策的能力。
*   **成本和可扩展性：**训练和运行这些模型的成本极其高昂，而持续的规模扩展主要带来更流畅的语言，不一定带来更高的智能或可靠性。

Marcus认为，该行业陷入了一个炒作周期，将巨额资金投入到一项在其当前形式下如同“纸牌屋”的技术中。他倡导研究重点的转变，转向构建混合AI系统，将符号推理和因果理解与神经网络相结合，以实现更强大、更可靠、真正智能的AI。他警告说，如果没有这种根本性的转变，大部分投资资本将产生递减回报，无法兑现真正变革性AI的承诺。

---

## 50. 语言主要是交流工具而非思想 (2024) [pdf]

**原文标题**: Language is primarily a tool for communication rather than thought (2024) [pdf]

**原文链接**: [https://gwern.net/doc/psychology/linguistics/2024-fedorenko.pdf](https://gwern.net/doc/psychology/linguistics/2024-fedorenko.pdf)

所提供的内容是原始的PDF二进制数据，无法直接读取或以文本形式进行总结。因此，无法对文章的内部要点进行概述。

然而，根据标题“语言主要是一种交流工具而非思维工具 (2024)”，这篇文章将探讨语言的根本目的。它可能会论证，语言的主要功能是促进个体间的互动、信息交流和社会凝聚，强调其外部的、交际性的作用。这种观点将与认为语言主要是内部认知过程、推理或思想形成的媒介的看法形成对比。该文于2024年发表，将对这一长期存在的哲学和语言学辩论提供一次当代审视。

---

## 51. Electron 对比 Tauri

**原文标题**: Electron vs. Tauri

**原文链接**: [https://www.dolthub.com/blog/2025-11-13-electron-vs-tauri/](https://www.dolthub.com/blog/2025-11-13-electron-vs-tauri/)

Dolt Workbench是一个开源的SQL工作台，最初是使用Electron构建的。Electron是一个流行的框架，用于将Web应用转换为桌面应用，它利用了Next.js前端和GraphQL层。然而，Electron的缺点促使团队探索Tauri，一个更新的Web转桌面替代方案。

一个关键区别在于对Next.js的支持。由于服务器端特性，Electron与Next.js的集成具有挑战性，它依赖于现在已不再维护的Nextron项目。相比之下，Tauri通过利用Next.js的静态站点生成功能，提供了更简单的集成。

最显著的区别在于网页视图（webview）。Electron捆绑了完整的Chromium浏览器引擎，这确保了UI的一致性，但导致了相当大的臃肿（例如，简单应用就达到150MB）。Tauri通过WRY库使用系统的原生网页视图，使得应用程序轻量得多，兼容性问题也鲜少出现。

对于后端“主”进程，Electron利用Node.js，这对Web开发者很有吸引力。然而，Tauri使用Rust。虽然初始上手难度较高，但Tauri提供了强大的JavaScript API，用于与Rust层交互，并且其IPC（进程间通信）抽象被认为更简洁。

Electron捆绑的Node.js运行时也简化了运行Node.js“边车”（sidecar），例如Workbench的GraphQL服务器。Tauri则需要将这些边车编译成二进制文件，尽管它为此常见用例提供了指导。Electron完整的Node.js运行时也导致了它比Tauri更大的应用体积。

尽管Tauri在减少臃肿和自然集成方面有优势，但全面迁移目前已暂停。限制包括Tauri不支持Windows .appx和.msix捆绑包，以及macOS通用二进制文件代码签名问题。这些是“烦恼”，而非硬性阻碍，意味着团队将在这些问题解决后，或者当Electron的问题变得更严重时，重新考虑迁移。总的来说，Tauri因其轻量级特性和集成能力而令人印象深刻。

---

## 52. 虎式：编程理念 (2024)

**原文标题**: Tiger Style: Coding philosophy (2024)

**原文链接**: [https://tigerstyle.dev/](https://tigerstyle.dev/)

"虎式风格" (版本 0.1-dev) 是一种受 TigerBeetle 启发的编程哲学，侧重于**安全性**、**性能**和**开发者体验**，旨在通过严谨的工程实践，构建健壮、高效且可维护的软件。

**安全性**是基础，通过可预测的执行确保代码的可靠性。其实践包括简单、显式的控制流（例如，短函数（不超过70行）、固定限制、集中式逻辑）、精确的内存/类型处理（例如，`u32`、静态分配、最小变量作用域），以及严格的错误管理（断言、快速失败、处理所有错误、将编译器警告视为错误、避免隐式默认值）。

**性能**应尽早解决，采用“餐巾纸计算”进行估算、批量操作，并优化资源使用（网络 > 磁盘 > 内存 > CPU）。它强调编写可预测的代码，以实现高效的CPU缓存，并减少对编译器优化的过度依赖。

**开发者体验**旨在构建可维护且协作友好的代码库。主要实践包括清晰、一致的命名（描述性、完整单词、带单位/修饰符）、记录设计原理、逻辑化的代码组织（简单接口、最小变量作用域、原地对象构造），以及严格的一致性（避免重复、通过引用传递大对象、整洁的缓冲区分配）。它还强调避免“差一错误”、一致的格式（缩进、行限制、清晰的代码块），并最小化/标准化外部依赖和工具。

一则**附录**强调了“零技术债”策略，主张一开始就把事情做好，并主动解决问题，以确保可持续的进展和质量。“餐巾纸计算”被再次强调，以提供早期性能洞察。

---

## 53. io_uring 和 kqueue 之上的程序员友好型 I/O 抽象 (2022)

**原文标题**: A programmer-friendly I/O abstraction over io_uring and kqueue (2022)

**原文链接**: [https://tigerbeetle.com/blog/2022-11-23-a-friendly-abstraction-over-iouring-and-kqueue/](https://tigerbeetle.com/blog/2022-11-23-a-friendly-abstraction-over-iouring-and-kqueue/)

本文探讨了如何在Linux的`io_uring`和macOS/FreeBSD的`kqueue`等高性能异步API之上构建一个程序员友好的I/O抽象层。文章首先指出，在硬件速度不断提升的背景下，传统的阻塞和非阻塞I/O中频繁的系统调用和上下文切换成为瓶颈。

`io_uring`和`kqueue`通过允许批量处理I/O请求并提供完成事件来解决这一问题，从而减少系统调用开销。`io_uring`的独特之处在于它允许内核直接使用用户提供的缓冲区执行I/O，相比`kqueue`的就绪模型，进一步分摊了系统调用成本。

直接实现，例如所提供的`io_uring` TCP回显服务器，会将I/O和业务逻辑交织在一起，在大型应用程序中变得难以管理。提出的解决方案是一个“中央I/O调度”抽象。该层通过提供高级API来调度I/O并附加回调函数，抽象化操作系统特定的差异并批量处理请求，从而统一了`io_uring`和`kqueue`。

它使用`flush`和`run_for_ns`函数构建了一个传统的事件循环，利用内核的`user_data`字段将完成事件与其各自的回调函数关联起来。一个内部溢出队列处理超出内核批处理大小的请求。该模型类似于`libuv` (Node.js)，并且是TigerBeetle的I/O库（被Bun采用）的基础。文章对比了`io_uring`的内核驱动I/O与`kqueue`的就绪模型，后者需要用户态I/O调用。它简要提到了Windows的`IOCP`，并探讨了单线程事件循环（有利于确定性，如TigerBeetle中）与多线程架构在不同工作负载下的应用。作者建议开源他们基于Zig的跨平台I/O库。

---

## 54. 长期运行智能体的高效框架

**原文标题**: Effective harnesses for long-running agents

**原文链接**: [https://www.anthropic.com/engineering/effective-harnesses-for-long-running-agents](https://www.anthropic.com/engineering/effective-harnesses-for-long-running-agents)

长期运行的AI智能体由于内存限制，在跨离散上下文窗口保持持续进展方面面临一个核心挑战。这导致智能体一次性尝试过多，留下半成品工作，过早宣布任务完成，以及测试不足。

Anthropic为Claude Agent SDK提供的解决方案包含一个双重机制：一个**初始化智能体**和一个**编码智能体**。初始化智能体负责设置初始环境，创建一个详细的`feature_list.json`文件，该文件概述了所有需求（初始标记为“失败”），以防止“一蹴而就”的尝试和过早完成。它还建立了一个用于服务器管理的`init.sh`脚本和一个初始Git提交。

**编码智能体**随后进行增量式进展，每次会话集中精力于一个特性。对其成功至关重要的是留下清晰的工件：将代码提交到Git并附带描述性消息，并维护一个`claude-progress.txt`文件。这使得后续智能体能够快速了解项目状态。通过提示智能体使用浏览器自动化工具（例如Puppeteer）以像人类用户一样验证功能，从而强制执行强大的端到端测试。

每次编码会话都从“定位”步骤开始——阅读Git日志、进度文件和特性列表，并通过`init.sh`运行基本的端到端测试，以确保在实现新特性之前有一个稳定的环境。这种结构化方法确保了代码库的整洁和可验证性，从而实现持续、增量的进展。未来的工作旨在探索多智能体架构，并将这些发现推广到网络开发之外的其他领域。

---

## 55. FileZilla Pro “永久许可证” – 致所有用户的警告

**原文标题**: FileZilla Pro "Perpetual License" – A Warning to All Users

**原文链接**: [https://github.com/x011/FileZilla-Pro-Download](https://github.com/x011/FileZilla-Pro-Download)

本文旨在对FileZilla Pro的“永久许可”发出严厉警告。作者曾为特定版本购买终身许可，但在重装操作系统后无法重新安装该软件。

FileZilla Pro支持部门承认作者有权合法使用其购买的版本，但明确拒绝提供安装程序，理由是出于“安全原因”不提供旧版本。作者认为，这种拒绝实际上使“永久许可”变得毫无价值，导致用户必须购买新许可（很可能是在其当前的订阅模式下）才能访问其合法拥有的软件。这意味着如果用户重装操作系统或丢失原始安装程序，他们就会失去访问权限。

作者强调，FileZilla清楚客户合法拥有这些旧版本，然而他们却故意不提供必要的安装程序。潜在买家应注意，他们面临着无法重新安装其合法拥有产品的风险。

文章还澄清，FileZilla与Mozilla没有关联，这是一个常见的误解。作者认为FileZilla的拒绝是出于经济动机而非安全考虑，并指出支持部门立即提供新版本折扣作为证据。

---

## 56. 空客 A320 飞行中电传操纵系统受辐射损坏

**原文标题**: Airbus A320 Fly by wire corrupted by radiation in flight

**原文链接**: [https://viewfromthewing.com/airbus-a320s-could-be-temporarily-grounded-worldwide-for-software-update-after-faulty-jetblue-computer-triggered-sudden-uncommanded-descent/](https://viewfromthewing.com/airbus-a320s-could-be-temporarily-grounded-worldwide-for-software-update-after-faulty-jetblue-computer-triggered-sudden-uncommanded-descent/)

航空博主JonNYC最初报道称空客A320系列飞机可能在全球范围内停飞或强制进行软件更新，这一说法后来得到空客证实。这一进展源于10月30日一架捷蓝航空A320航班，该航班在从坎昆飞往纽瓦克的途中“在没有飞行员输入的情况下意外俯冲”，导致10-15名乘客住院，并被迫改道飞往坦帕。

美国国家运输安全委员会（NTSB）将泰雷兹ELAC 2计算机的故障认定为可能原因，该计算机负责解释飞行员的指令以控制飞行，故障发生在ELAC开关转换期间。至关重要的是，飞机冗余的ELAC系统，本应在一个单元失效时无缝接管，但并未按预期运行。

JonNYC证实解决方案是为ELAC单元进行强制性软件更新，预计每架飞机需要几个小时。空客随后发布了“运营商警示通告”（AOT），指出“强烈的太阳辐射可能会损坏对飞行控制功能至关重要的数据”。他们敦促运营商通过软件和/或硬件保护实施“立即预防措施”，并承认这些措施将导致“运营中断”。

这个问题影响全球约10,000架A320系列飞机，此前美国联邦航空管理局（FAA）曾于2018年就迎角问题发布了关于ELAC单元升级的指令。尽管预计会有航班取消，但这些取消预计将错峰进行，以最大程度地减少对乘客的影响。具体的时间细节尚未公布。

---

## 57. 珠子 — 你的编程智能体的记忆升级

**原文标题**: Beads – A memory upgrade for your coding agent

**原文链接**: [https://github.com/steveyegge/beads](https://github.com/steveyegge/beads)

Beads (bd) 是一种轻量级、基于图的问题追踪器，旨在为AI编程代理提供“记忆升级”，解决它们的健忘症，并增强它们处理长期、复杂任务的能力。代理使用Beads来提交、管理和链接问题，确保任务的正确排序，并防止工作丢失或计划混乱。

v0.20.1版本中的一个关键更新是引入了基于哈希的ID（例如bd-a1b2）来取代顺序数字。这消除了合并冲突和碰撞问题，实现了可靠的多工作者、多分支和多代理工作流，这对协作开发至关重要。

Beads作为一个独特的分布式数据库运行，利用Git作为其后端。问题数据存储在Git版本化的JSONL文件（`.beads/beads.jsonl`）中，而每台机器都维护一个快速的本地SQLite缓存。这种设计允许不同机器上的代理查询和更新一个看似共享的数据库，而无需中央服务器或复杂的配置。

人类使用`bd init`初始化Beads并指示其代理使用该工具，但代理主要管理问题追踪过程。其功能包括依赖追踪（四种类型）、自动就绪工作检测、代理友好的JSON输出、完整的审计追踪以及针对旧问题的“记忆衰减”。“隐身模式”允许个体开发者私下使用Beads，而无需修改主仓库。尽管Beads正处于积极开发阶段（alpha状态），但它旨在为代理提供前所未有的长期规划能力和改进的项目可审计性。

---

## 58. ‘标普493’揭示不同的美国经济

**原文标题**: The 'S&P 493' reveals a different U.S. economy

**原文链接**: [https://www.msn.com/en-us/money/markets/the-s-p-493-reveals-a-very-different-us-economy/ar-AA1R1VUJ](https://www.msn.com/en-us/money/markets/the-s-p-493-reveals-a-very-different-us-economy/ar-AA1R1VUJ)

抱歉，我无法为您总结MSN上题为“‘标普493’揭示了不一样的美国经济”的文章。您没有提供该文章的内容。

为了有效地总结一篇文章，我需要获取其全文，以理解其主要观点、关键论证、数据和结论。

如果您能提供文章的全文，我将很乐意在您指定的字数限制内为您总结。

然而，仅凭标题来看，它强烈暗示了一项分析，旨在区分更广泛的美国经济（由493家公司代表）的表现和健康状况与少数几家大公司（标普500指数中剩余的7家）的巨大影响力之间的差异。这样的文章可能会探讨诸如市场集中度、经济增长的分布、中小型或更传统行业的表现，以及对投资者或政策制定者可能产生的影响等主题。

---

## 59. DNS LOC 记录 (2014)

**原文标题**: DNS LOC Record (2014)

**原文链接**: [https://blog.cloudflare.com/the-weird-and-wonderful-world-of-dns-loc-records/](https://blog.cloudflare.com/the-weird-and-wonderful-world-of-dns-loc-records/)

CloudFlare 利用其定制的基于 Go 语言的 DNS 服务器 RRDNS，发现了一个与鲜为人知的 DNS LOC（位置）记录类型相关的错误。尽管处理着数百万条 DNS 记录，其中只有 743 条是 LOC 记录，但有一位客户报告说他们的 LOC 记录未能被正确解析。

调查显示，RRDNS 具备接收和响应 LOC 数据的基础设施，但缺少一个关键组件：将人类可读的文本 LOC 记录格式（例如，“33 40 31 N 106 28 29 W 10m”）解析成其内部二进制“线上传输”格式的代码。

这两种格式都在 RFC 1876 (1996) 中有详细说明。文本格式规定了纬度、经度、高度以及可选的大小/精度，对省略的值有默认设定。二进制格式是一个固定的 16 字节结构。纬度、经度、高度是 32 位无符号整数，表示弧秒的千分之一或从基准高度算起的厘米数。独特之处在于，8 位的尺寸和精度值采用“底数和十的幂”编码（例如，0x15 = 1e5），使得从 1 厘米到 90,000 公里的广泛值范围能够以紧凑且易读的十六进制形式表示。

作者为文本 LOC 记录实现了一个解析器，从而修复了这个错误。RRDNS 现在能够正确解析 LOC 记录，确保所有指定的地理位置数据在 DNS 系统中正确传播。

---

## 60. 我的自制操作系统上的C++ Web服务器

**原文标题**: C++ Web Server on my custom hobby OS

**原文链接**: [https://oshub.org/projects/retros-32/posts/getting-a-webserver-running](https://oshub.org/projects/retros-32/posts/getting-a-webserver-running)

joexbayer成功实现了一个重要里程碑：在其自定义的业余操作系统RetrOS-32上运行了一个C++ Web服务器。经过一段时间的沉寂，广泛的调试修复了关键问题，包括损坏的终端缓冲区和E1000网卡驱动程序错误，最终使基本的TCP协议栈完全正常工作。随后，通过处理突发数据包和正确处理浏览器生成的RST数据包，性能得到了提升。

该Web服务器的架构由几个自定义构建的组件组成。一个HTTP引擎，改编自作者的`c-web-modules`项目，负责处理请求解析。它被集成到一个Web引擎中，该引擎提供了现代C++路由功能，允许将路径和方法映射到lambda函数处理程序。随后添加了一个文件仓库（FileRepository）来提供带缓存的静态HTML文件。

系统的堆栈从浏览器流向用户空间的Web服务器（包含WebEngine、HTTPEngine和FileRepository），该服务器依赖于内核健壮的网络协议栈（TCP/UDP、IP、ARP、DHCP、DNS和E1000以太网驱动程序）。该项目未来的计划包括实现优雅的服务器关闭和在操作系统内部开发一个Web浏览器。该项目强调使用C++从头开始实现。

---

## 61. 龙虾采访

**原文标题**: Lobsters Interview

**原文链接**: [https://susam.net/my-lobsters-interview.html](https://susam.net/my-lobsters-interview.html)

Susam Pal的《Lobsters访谈》全面深入地探讨了他的计算哲学、工具和兴趣。这篇访谈由Lobsters社区的Alex编辑和重新整理，凸显了Pal对技术和数学的深度投入。

Pal广泛使用Common Lisp进行个人项目，并使用Emacs Lisp自动化任务，同时还涉猎Python、Go、Rust以及单文件HTML/JavaScript工具。他的计算之旅始于童年时期的Logo语言，2007年发现了Lisp（当时是CLISP，现在是SBCL），之后通过SLIME接触到Emacs。数学是他一生的热情，例如，他对数论的兴趣便是由研究RSA密码系统所激发的。

他将“娱乐性计算”定义为探索、提问“会发生什么”，并分享结果，这在他的`devil-mode`或小型游戏等项目中显而易见。他多样的兴趣往往相互关联；MathB、TeXMe和Muboard等工具都是源于分享数学笔记的愿望而演变出来的。除此之外，他还探索IRC客户端、光线追踪和趣味编程。

对Pal而言，“计算”广义上包括编程、使用、理解系统（甚至构建CPU），以及深入研究抽象的数学基础，他将计算机科学视为离散数学的实际应用。他优先考虑问题领域而非特定工具，为特定任务选择最合适的语言或框架。他创建新Emacs功能的频率自然有所下降，他将此归因于拥有一个稳定且令人满意的设置，以及较少的时间进行持续的修修补补。

---

## 62. 44年Unix演进存储库

**原文标题**: A Repository with 44 Years of Unix Evolution

**原文链接**: [https://www.spinellis.gr/pubs/conf/2015-MSR-Unix-History/html/Spi15c.html](https://www.spinellis.gr/pubs/conf/2015-MSR-Unix-History/html/Spi15c.html)

迪奥米迪斯·斯皮内利斯（Diomidis Spinellis）创建了一个综合性的Git存储库，记录了Unix操作系统44年的演进历程，从其1972年作为一个拥有5,000行代码的内核诞生，到2015年发展成为一个拥有2,600万行代码的系统。该存储库托管于GitHub上，容量为1GB，包含了659,000次提交和2,306次合并，并识别出850位来自贝尔实验室、伯克利和FreeBSD项目的贡献者。

该存储库是利用定制软件合成的，整合了24个历史快照（包括Research Unix、BSD、386BSD）、两个旧版版本控制系统（CSRG SCCS、FreeBSD 1 CVS）以及现代的FreeBSD Git存储库。大量的原始研究被用于归属作者身份，并建立这些不同来源之间的合并关系。

一项关键创新在于精心保留了跨快照的提交历史，使得`git blame`工具能够准确追溯贯穿整个44年的代码来源。这使得研究人员能够识别代码行的起源，揭示出现代的FreeBSD版本仍然包含相当一部分代码，这些代码来自早期的版本，如BSD 4.3，甚至追溯到1979年的第七版Unix。

这一独特的数据集为软件工程、信息系统和软件考古学领域的实证研究提供了宝贵的资源，为理解这一最具影响力的操作系统之一的演进提供了前所未有的深入见解。

---

## 63. 瑞士：数据保护官员对当局实施全面的云服务禁令

**原文标题**: Switzerland: Data Protection Officers Impose Broad Cloud Ban for Authorities

**原文链接**: [https://www.heise.de/en/news/Switzerland-Data-Protection-Officers-Impose-Broad-Cloud-Ban-for-Authorities-11093477.html](https://www.heise.de/en/news/Switzerland-Data-Protection-Officers-Impose-Broad-Cloud-Ban-for-Authorities-11093477.html)

瑞士数据保护官（DPOs）发布了一项全面建议，建议联邦、州和市镇当局停止使用来自被认为“数据保护不足”国家的服务提供商的云服务。这项重要指令主要针对美国的云服务提供商，其驱动因素是对外国情报机构可能获取数据的深切担忧，例如通过美国《云法案》，即使数据实际存储在瑞士。

联邦数据保护和信息专员（FDPIC）联同州和市镇的数据保护官强调，瑞士当局作为数据控制者，对个人数据的保护负有全权责任。他们声称，目前没有充分的法律依据来保证公共机构在使用此类云服务时的数据保护。这项广泛建议扩展了此前的警告，包括FDPIC在2021年对Microsoft 365的立场。

这项禁令影响了广泛的公共服务，从学校、医疗保健到关键基础设施。当局被敦促审查其当前的云服务使用情况，停止从不合规提供商处引入新服务，并将现有数据迁移到安全的替代方案。数据保护官们倡导采用完全符合瑞士数据保护法律的本地、欧洲或瑞士云解决方案，以促进数字主权。受影响的公共实体预计将在2025年底前实施这些更改并完成数据迁移。

---

## 64. Hachi: 图片搜索引擎

**原文标题**: Hachi: An Image Search Engine

**原文链接**: [https://eagledot.xyz/hachi.md.html](https://eagledot.xyz/hachi.md.html)

Hachi 是一个雄心勃勃的项目，旨在构建一个完全自托管、端到端的图像搜索引擎，未来计划支持视频、文本和音频。它旨在解决个人不断增长且分布式的个人数据搜索难题，并批判现有搜索引擎的单向信息流、对部分查询处理不佳以及侵犯隐私的特性。

该项目旨在提供一个以用户为中心的界面，通过公开多个数据属性来实现递归式查询优化。其核心理念包括极简主义（最少的外部依赖）、可修改性（易于使用 Python/Nim 进行修改）和实验性（融合确定性元数据与语义机器学习属性）。Hachi 优先考虑速度并避免数据重复，而是采用一个元数据索引引擎（用 Nim 编写），并结合向量搜索能力来实现语义查询。

目前 Hachi 专注于图像，实现了强大的面部识别功能，生成嵌入向量用于最近邻搜索。基于 Nim 的元索引是一个单线程、面向列的数据库。未来的目标包括改进字符串查询、添加 SIMD 优化、动态模式更新以及在低功耗设备集群上实现分布式查询，同时保持其原则性、高性能的方法。

---

## 65. JSON Schema 揭秘：方言、词汇与元模式

**原文标题**: JSON Schema Demystified: Dialects, Vocabularies and Metaschemas

**原文链接**: [https://www.iankduncan.com/engineering/2025-11-24-json-schema-demystified/](https://www.iankduncan.com/engineering/2025-11-24-json-schema-demystified/)

JSON Schema描述了JSON数据的结构和约束。其核心是，**schema**（模式）是一个JSON文档，它使用“type”和“properties”等关键字为其他JSON文档定义规则。

这些schema的结构本身由一个**metaschema**（元模式）描述。metaschema实际上是“schema的schema”，它定义了允许使用哪些关键字、它们的取值以及它们如何起作用。它确保你的schema格式良好，并为工具提供正式规范。这种关系是：数据由schema验证，而schema由metaschema验证。

随着JSON Schema的演进，出现了不同的版本。**dialect**（方言）是JSON Schema的一个特定版本或“风味”（例如，Draft 2020-12），通过`$schema`关键字中的URI进行标识。每个方言都有其自己的定义metaschema和一套行为。

从Draft 2019-09开始，JSON Schema引入了**vocabularies**（词汇表）。vocabulary是相关关键字的命名、模块化集合（例如，核心、验证、应用器、元数据）。方言不再由单一的metaschema构成，而是由各种vocabulary组合而成。这种模块化实现了强大的可扩展性：开发人员可以定义自己的vocabulary，包含自定义关键字（例如在OpenAPI中或用于领域特定的注解），这些关键字可以被兼容工具明确声明和理解。

总而言之，你的数据由你的schema验证。你的schema遵循一个方言，该方言由metaschema定义，并使用组织成vocabulary的关键字。这个系统实现了清晰性、演进性和强大的可扩展性。

---

## 66. 如何使用 Linux vsock 实现虚拟机快速通信

**原文标题**: How to use Linux vsock for fast VM communication

**原文链接**: [https://popovicu.com/posts/how-to-use-linux-vsock-for-fast-vm-communication/](https://popovicu.com/posts/how-to-use-linux-vsock-for-fast-vm-communication/)

本文演示了如何使用 Linux `vsock` 在虚拟机 (VM) 及其宿主机之间实现高效通信，绕过传统的 TCP/IP 网络。`vsock` 提供了一个类似套接字的 API，但它采用了一种基于上下文 ID (CID) 和端口号的专门寻址方案，专为虚拟环境设计。

作者通过实现一个用于整数加法的 gRPC 服务来阐释这一点。服务器运行在通过 QEMU 启动的 Debian 虚拟机内，而客户端则运行在宿主机上。该项目使用 Bazel 构建，为客户端和服务器生成了静态链接的 C++ 二进制文件。

设置的关键是 `vsock` 地址格式：`vsock:CID:PORT`。在实验中，虚拟机服务器监听 `vsock:3:9999`，其中 `3` 是访客虚拟机的上下文 ID。宿主机客户端随后连接到相同的 `vsock:3:9999` 以发送 RPC 请求。

QEMU 虚拟机配置了 `-device vhost-vsock-pci,guest-cid=3`，这会将带有指定 CID 的 `vsock` 网络硬件暴露给访客。在将服务器二进制文件作为 `init` 进程启动虚拟机后，宿主机客户端成功调用了加法 RPC，证实了直接通信。

这种方法使得在隔离的虚拟机环境中实现结构化 RPC 成为可能，支持多种操作系统和 gRPC 的多语言能力。主要优点是由于消除了网络虚拟化开销而提高了效率。

---

## 67. CRDT 词典：无冲突复制数据类型实战指南

**原文标题**: The CRDT Dictionary: A Field Guide to Conflict-Free Replicated Data Types

**原文链接**: [https://www.iankduncan.com/engineering/2025-11-27-crdt-dictionary/](https://www.iankduncan.com/engineering/2025-11-27-crdt-dictionary/)

本文作为无冲突复制数据类型（CRDTs）的实战指南，源于作者对CRDTs在分布式系统应用中重新燃起的好奇心。CRDTs提供了一种在没有协调或数据丢失的情况下处理并发写入的解决方案，这对于前Riak数据库或离线优先应用等系统至关重要，它不同于基于共识的方法（Paxos/Raft）可能在分区时阻塞，也不同于最后写入胜出（Last-Write-Wins）可能导致数据丢失。

CRDTs的核心“诀窍”在于其合并操作是可交换的、结合的、幂等的，这确保了无论状态合并的顺序或次数如何，副本之间都能确定性地收敛。这个概念通常与格（lattices）相关联，其中数据状态形成偏序，并且更新只“向上”移动。

CRDTs大致分为基于状态的（CvRDTs，发送完整状态）和基于操作的（CmRDTs，发送操作）。本指南侧重于基于状态的示例：
*   **G-Counter：** 一种只增计数器，每个副本跟踪自己的计数，通过取每个组件的最大值进行合并。无法递减。
*   **PN-Counter：** 在G-Counter的基础上扩展，为正增量和负增量分别使用独立的G-Counter，从而允许两种操作。
*   **G-Set：** 一种只增集合，使用集合“并集”进行合并。无法移除元素。
*   **2P-Set：** 一种两阶段集合，由“已添加”和“已移除”两个G-Set组成。允许移除，但防止重新添加已移除的元素。
*   **LWW-Element-Set：** 使用时间戳来确定添加和移除的“最后写入”，如果元素的添加时间戳比移除时间戳新，则允许重新添加该元素。

这些示例说明了CRDTs是如何设计来保证最终一致性和数据完整性，而无需复杂的分布式协调。

---

## 68. VPN恐慌才刚刚开始

**原文标题**: The VPN panic is only getting started

**原文链接**: [https://www.theverge.com/tech/827435/uk-vpn-restrictions-ban-online-safety-act](https://www.theverge.com/tech/827435/uk-vpn-restrictions-ban-online-safety-act)

英国的《网络安全法》（OSA）原计划于2025年7月引入严格的在线年龄验证，以限制用户访问“有害内容”，但该法案正因VPN（虚拟私人网络）的广泛使用而受到严重破坏。这些VPN允许用户通过伪造IP地址绕过年龄验证，导致英国居民的VPN注册量大幅飙升。

当局对此日益担忧，儿童事务专员雷切尔·德·苏扎将VPN称为“需要堵塞的漏洞”，并主张对该软件进行年龄门槛限制。尽管政府坚称鉴于VPN对企业、记者和个人隐私的合法用途，目前“没有计划禁止”VPN，但一位部长表示“一切皆有可能”。据报道，英国媒体监管机构Ofcom正在“监测VPN的使用情况”。

全面禁止VPN被认为技术上极具挑战性，政治上也可能性不大。要求网站屏蔽VPN流量同样存在问题，因为这将迫使网站要么放弃英国市场，要么屏蔽所有VPN用户。最可能的结果是对VPN服务本身进行年龄限制，从而扩大《网络安全法》的适用范围。

专家警告称，此类限制可能将用户推向风险更高、信誉较差的免费VPN或直接文件共享，从而产生新的隐私和安全漏洞。这种“VPN恐慌”并非英国独有；随着越来越多的国家实施在线年龄限制而VPN仍是有效的规避方法，类似的讨论和拟议限制正在全球范围内出现，例如澳大利亚、欧盟和美国各州。

---

## 69. HN发布：Pulse 2.0 – 实时共听房间，人人都能当DJ

**原文标题**: Show HN: Pulse 2.0 – Live co-listening rooms where anyone can be a DJ

**原文链接**: [https://473999.net/pulse](https://473999.net/pulse)

Pulse 2.0是一个通过“Show HN”公告推出的新平台，旨在创建实时、互动式的共同聆听房间。其主要功能是赋能用户充当DJ，实时为他人策划并广播音乐。此举使DJ体验民主化，允许任何人主持房间并分享他们的音乐品味，从而营造一个动态且具有社区感的音频环境。Pulse 2.0旨在促进音乐爱好者之间的共同发现和联系，超越静态播放列表，演变为用户既是听众又是积极参与者的实时、引人入胜的声景。

---

## 70. 太空数据中心是个馊主意。

**原文标题**: Datacenters in space are a terrible, horrible, no good idea

**原文链接**: [https://taranis.ie/datacenters-in-space-are-a-terrible-horrible-no-good-idea/](https://taranis.ie/datacenters-in-space-are-a-terrible-horrible-no-good-idea/)

一位前NASA和谷歌云工程师强烈指出，太空数据中心，尤其是用于处理使用GPU和TPU的AI工作负载的数据中心，是一个极其糟糕的主意，因为它们与太空环境存在根本性的不兼容。

**供电：** 太空电力充足是一个误解。国际空间站 (ISS) 巨大的2500平方米太阳能电池阵列能产生200千瓦 (kW) 的电力，仅够约200块NVIDIA H200 GPU使用。为一个拥有10万块GPU的数据中心供电，将需要500颗国际空间站大小的卫星，而每颗卫星仅能支持相当于三个地面服务器机架的设备。核放射性同位素热电发电机 (RTG) 功率过低 (50-150瓦)，甚至无法运行一块GPU。

**热量管理：** 太空环境不易散热。真空阻止了对流，热量必须通过巨大的散热器散发。国际空间站的活动式热管理系统使用一个42.5平方米的散热器，处理16千瓦 (用于约16块H200 GPU) 的热量。将热处理能力扩展到200千瓦，将需要一个巨大的531平方米的散热器，如此巨大的散热器会使卫星本身相形见绌，而其所能提供的容量却微乎其微。

**抗辐射能力：** 太空辐射会导致单粒子翻转 (位翻转)、破坏性的单粒子锁定以及长期的性能下降。现代GPU/TPU由于其微小、密集的晶体管和大的芯片面积，极易受到影响。由于质量限制，有效的屏蔽是不切实际的。经过抗辐射加固的太空处理器提供的性能仅相当于20年前的技术，与当前的AI硬件不可同日而语。

**通信：** 可靠的星地数据链路通常限制在1Gbps左右，与地面数据中心100Gbps以上的互连带宽相比，这是一个显著的瓶颈。

总之，作者指出太空数据中心将极其困难、成本极其高昂、性能平庸，并且是一个“灾难性糟糕的主意”。

---

## 71. 我知道AI是泡沫，因为没人要我。

**原文标题**: I Know We're in an AI Bubble Because Nobody Wants Me

**原文链接**: [https://petewarden.com/2025/11/29/i-know-were-in-an-ai-bubble-because-nobody-wants-me-%f0%9f%98%ad/](https://petewarden.com/2025/11/29/i-know-were-in-an-ai-bubble-because-nobody-wants-me-%f0%9f%98%ad/)

佩特·沃登，一位自2012年以来便是深度学习领域的资深人士和效率倡导者，认为当前的人工智能热潮是一个因资源分配不合理而不可持续的泡沫。他观察到数百亿资金投入到AI硬件（GPU、数据中心）中，但在机器学习基础设施工程师和软件优化方面的投资却明显不足，这与他自己的创业公司尽管专注于效率却难以获得资金的情况形成了对比。

沃登认为这在经济上是不理性的。公司每月花费数十亿购买通常利用率不足（低于50%）的GPU，从理性的角度来看，应该投资数亿进行软件优化，以大幅削减成本、提高性能并减少对环境的影响。他强调，有动力的工程师可以超越标准库的性能，而且许多推理任务可以在更便宜的CPU上运行。

他将这种不平衡归因于“信号效应”。像OpenAI这样的初创公司将大规模购买GPU作为“护城河”，以展示其主导地位并吸引投资。投资者发现支持这些大型硬件投资更容易、更安全，而大型科技公司从硬件发布中获得的积极新闻和股价提振，比从雇佣效率优化人员中获得的更多。硬件项目也被认为比复杂的软件优化更容易管理。

沃登将这比作互联网泡沫时期对昂贵的Sun工作站的依赖，谷歌当时通过廉价PC和开源软件打破了这种局面。他预测人工智能领域也将出现类似的情况，届时，聊天机器人初创公司将利用价格实惠的PC和开源CPU模型，强调当前硬件优先方法的不可持续性。

---

## 72. 财富如何消亡

**原文标题**: How wealth dies

**原文链接**: [https://surplusenergyeconomics.wordpress.com/2025/11/02/314-how-wealth-dies/](https://surplusenergyeconomics.wordpress.com/2025/11/02/314-how-wealth-dies/)

文章《财富如何消亡》强调了一个关键的失衡：金融财富总量持续增长，而“实体”物质经济却在萎缩。这种明显的悖论解释为，旨在阻止物质经济衰退的货币干预措施，反而讽刺地推高了以金融方式衡量的财富，而这些财富中的大部分是“名义上的”，无法转化为物质价值。

实体经济是由能源将自然资源转化为商品和服务所驱动的，但这一过程受到不断上升的能源获取成本（ECoE）和资源枯竭的阻碍。因此，几十年来物质繁荣几乎没有增长，预计将出现显著下降，使“生活成本危机”成为永久性趋势。货币本身没有内在价值；它仅仅是对有限物质商品的“可执行债权”。政府可以创造无限的货币，但不能创造无限的资源。

名义财富的大规模增长，特别是自20世纪70年代以来，一直由央行干预措施推动（例如1987年股灾和2008年危机后的“美联储看跌期权”）。这种“兜底”行为制造了道德风险，鼓励投资者预期获得救助，从而进行过度冒险。

核心问题在于，所有报告的财富总量从根本上都是“虚假的”且无法变现的。它们的“价值”来源于边际交易价格，错误地暗示整个市场或资产类别可以按其标示的价值出售。该系统注定会“死于富有”，拥有创纪录的账面财富，但随着货币体系在其未能兑现的物质债权重压下崩溃，这些财富将变得毫无意义。

---

## 73. 我们正在了解更多维生素D对人体的影响。

**原文标题**: We're learning more about what Vitamin D does to our bodies

**原文链接**: [https://www.technologyreview.com/2025/11/21/1128206/vitamin-d-bodies-bone-health-immune/](https://www.technologyreview.com/2025/11/21/1128206/vitamin-d-bodies-bone-health-immune/)

本文探讨了维生素D（常被称为“阳光维生素”）普遍缺乏的问题，尤其是在冬季的英国等地区。尽管其主要已确立的作用在于骨骼健康——帮助钙吸收并预防佝偻病——近期研究正在揭示它对其他身体系统的潜在影响。

科学家们正在调查维生素D水平与免疫功能、心脏健康（包括血压和心血管事件）、心理健康、妊娠结局，甚至癌症存活率之间的联系。然而，在这些新领域中，关于补充剂益处的证据大多混杂且常常尚无定论；例如，虽然低维生素D水平与普通感冒有关，但补充剂尚未被持续证明能预防急性呼吸道感染。

研究的复杂性在于，大部分维生素D来自阳光照射，而膳食来源有限。关于“理想”的血液水平没有普遍共识，个人对紫外线的反应差异很大（例如，由于黑色素）。尽管存在这些复杂性，全球在婴儿补充维生素D以预防佝偻病方面达成了共识。英国政府建议成年人在秋冬季服用10微克的补充剂。目前的重点仍然是预防维生素D缺乏症（血液水平低于每升30纳摩尔），同时我们正等待对其全面影响有更明确的认识。

---

## 74. 使用大模型时的反模式

**原文标题**: Anti-patterns while working with LLMs

**原文链接**: [https://instavm.io/blog/llm-anti-patterns](https://instavm.io/blog/llm-anti-patterns)

本文基于15个月的经验，总结了使用LLM时应避免的五种反模式。

1.  **冗余上下文：** 避免在同一会话中重复发送相同信息。上下文是一种宝贵的资源；只提供新的或显著改变的信息，而不是重复的数据（例如几乎相同的截图），以节省资源并提高效率。

2.  **任务分配不当：** 不要让LLM执行它们不擅长的任务。例如，直接、精确的计数或带有特定文本约束的复杂图像生成可能很困难。相反，应利用它们的优势，例如生成用于精确计数的代码，或在图像任务中合并预先存在的视觉元素，这些是它们通常擅长的。

3.  **上下文过载：** LLM在上下文窗口未接近满载时表现最佳。在接近token限制（例如128k token）的长时间会话中，LLM可能会“淹没”，它们会不可预测地压缩或丢弃数据，从而忘记关键细节或产生不准确的信息。请注意这种准确性下降。

4.  **冷门主题：** 由于训练数据不足，LLM难以处理小众主题或其训练截止日期之后出现的话题。对于这些领域，请预期较低的准确性并规划其他验证方法。

5.  **盲目信任：** 避免成为一个“凭感觉行事”的开发者，忽视LLM的输出。彻底审查生成的代码和响应至关重要，以发现细微错误或安全漏洞（例如无意中暴露敏感用户数据），从而防止潜在风险。

---

## 75. 四模糊器记

**原文标题**: A Tale of Four Fuzzers

**原文链接**: [https://tigerbeetle.com/blog/2025-11-28-tale-of-four-fuzzers/](https://tigerbeetle.com/blog/2025-11-28-tale-of-four-fuzzers/)

TigerBeetle 最近重构了其复制路由算法（自适应复制路由，ARR），以应对不断变化的网络拓扑，这成为了一个实用生成测试的案例研究。文章强调，有效的模糊测试不仅需要一个，而是多个、多样化的模糊测试器，尤其关键的是，一种以“最小化接口”为核心的设计理念。

复制对于数据持久性至关重要。最初的方法，如广播（带宽密集型）和静态环形拓扑（易受网络变化和“冷代码”错误影响），都被证明不足。ARR 通过将主节点置于动态环的中间来解决这个问题，允许冗余（即使一个消息丢失，消息也仍会被复制），并使集群能够根据实时延迟测量（格蕾丝·霍珀风格）动态地重新排序副本，而不是依赖可能产生误导的模型。

为了有效地对 ARR 进行模糊测试，全系统模拟（VOPR）被认为不足以用于深层和特定断言。子系统模糊测试的普遍原则是将连接抽象到最小化接口之后。文章指出，这种接口最小化应该发生在架构的“草图”阶段，而不是在实现之后。

`Routing` 组件的接口是这方面的例证：它传递简单的整数（`Instant` 用 `u64`，副本 ID 用 `u8`），并维护 `view` 号的私有副本，这有意简化了依赖，以提高模糊测试效率，尽管偶尔会偏离“最佳实践”。引入的第一个模糊测试器利用这一点，通过将路由的序列化和反序列化作为基于属性的测试进行测试，从而确保编码过程中的数据完整性。

---

## 76. 谷歌否认Gmail用你的邮件训练AI的‘误导性’报道

**原文标题**: Google denies 'misleading' reports of Gmail using your emails to train AI

**原文链接**: [https://www.theverge.com/news/826902/gmail-ai-training-data-opt-out](https://www.theverge.com/news/826902/gmail-ai-training-data-opt-out)

Google 正在驳斥社交媒体上疯传的帖子和文章，这些帖子和文章错误地声称 Gmail 使用用户的电子邮件和附件来训练 Gemini 等人工智能模型，并且必须选择退出“智能功能”才能阻止这种情况发生。

Google 发言人珍妮·汤姆森（Jenny Thomson）表示，这些报道是“误导性的”，她强调 Google 并未更改任何人的设置，Gmail 的智能功能已存在多年，并且该公司“不会使用您的 Gmail 内容来训练我们的 Gemini AI 模型。”

疯传的说法建议用户需要禁用拼写检查等“智能功能”以避免 AI 训练。尽管 Google 否认使用电子邮件内容进行 AI 训练，但文章指出用户可能仍需检查其“智能功能”设置。这是因为一位 Verge 工作人员发现他们之前选择退出后又被重新加入了这些功能。今年一月，Google 更新了其设置，允许用户独立控制 Google Workspace 和其他 Google 产品（如地图和钱包）的智能功能。

在 Workspace 中启用智能功能，Google 可以使用“Workspace 内容和活动来个性化您在 Workspace 中的体验”，例如拼写检查、订单跟踪以及将航班添加到日历，但 Google 澄清这不涉及使用电子邮件内容进行 AI 训练。

---

## 77. GrapheneOS 退出法国

**原文标题**: GrapheneOS Moving Out of France

**原文链接**: [https://xcancel.com/GrapheneOS/status/1993035936800584103](https://xcancel.com/GrapheneOS/status/1993035936800584103)

GrapheneOS 正在将所有活跃服务器迁出法国，并中止与 OVH 的合作关系，原因是担忧法国执法部门在加密和隐私问题上的立场。该组织指出，法国“对开源隐私项目来说不是一个安全的国家”，并指责法国当局期望加密和设备访问中存在后门、散布虚假信息以及进行直接威胁。

作为迁移的一部分，GrapheneOS 正在轮换 TLS、Let's Encrypt 和潜在的 DNSSEC 密钥。目前，备份仍加密存储在 OVH 上。目前托管在加拿大五个 OVH 服务器上的关键服务，如电子邮件、Matrix、讨论论坛、Mastodon 和证明服务，短期内将迁移到 Netcup 根服务器或类似提供商，长期计划是在多伦多建立托管服务器。

更新镜像目前位于美国的赞助服务器 (ReliableSite) 和伦敦的临时服务器 (Tempest) 上，未来计划增加更多。他们的任播 DNS 网络（ns1 位于 Vultr，ns2 位于 BuyVM）支持 BGP，主网站/操作系统连接服务器正迁移到 Vultr 和 BuyVM 的混合地点。

GrapheneOS 强调其强大的安全措施，包括为其应用商店和系统更新程序提供加密签名验证和降级保护，这得益于 Android 的包管理器、update_engine 和验证启动。他们强调，绕过基于安全元件的暴力破解保护（据称法国执法部门希望如此）在技术上是不可能的。

此次迁移正在扰乱开发工作，包括实验性的 Pixel 10 支持。GrapheneOS 报告称，针对其团队的诽谤、骚扰和聊天室突袭事件正在加剧。尽管服务器进行了搬迁，GrapheneOS 仍确认其服务，包括连接性检查、网络时间以及更新，将通过德国和瑞士等其他国家的服务器，完全面向法国用户开放。他们还对在丹麦和英国的运营表示担忧，因为这些国家在加密方面存在类似的法律压力。

---

## 78. 大降容

**原文标题**: The Great Downzoning

**原文链接**: [https://worksinprogress.co/issue/the-great-downzoning/](https://worksinprogress.co/issue/the-great-downzoning/)

这篇文章介绍了“大降级分区”，这是1890-1940年间西方城市从高度宽松的建筑法规（例如，没有高度限制）转变为限制性分区的一次深刻转变。作者认为，这一过程是当代住房短缺的主要原因，对健康、家庭、环境和经济增长造成严重后果，可能使美国GDP减少25%。

与认为反密度意识形态是唯一驱动因素的假设相反，作者提出，降级分区主要是受利益驱动的。它通过阻止“不受欢迎的”开发，成功提升了现有郊区的房产价值，但在降低土地价值的地方（例如在绿地地区）则面临阻力。

历史上，早期郊区通常是未经规划的，且用途混合的。从18世纪起，有规划的、低密度的郊区开始出现，最初采用私人“契约”（一种“原始降级分区”）以对密度、用途甚至最低价格施加限制，从而保护社区特色和价值。然而，这些契约因法律模糊性、无法适应不断变化的条件（如通货膨胀）以及高昂的执行成本而失效。这些局限性为公共的、由政府主导的降级分区铺平了道路。

如今，尽管降级分区仍使一些业主受益，但在大城市，它造成的住房短缺现在反而*降低*了房产价值，这促成了新的利益联盟的形成，这些联盟最终可能逆转“大降级分区”的局面。

---

## 79. 俐拓扫地机器人将停止工作

**原文标题**: Neato vacuum robots to stop working

**原文链接**: [https://support.neatorobotics.com/support/solutions/articles/204000073686-announcement-6th-oct-2025](https://support.neatorobotics.com/support/solutions/articles/204000073686-announcement-6th-oct-2025)

诺拓机器人于2025年10月6日宣布，将逐步停止其云服务。此决定是在作为福维克集团旗下公司的诺拓机器人已于2023年停止运营之后做出的。

最初，福维克曾承诺提供五年云服务，以确保客户能够继续顺畅使用他们的机器人，履行此前的承诺。然而，由于自2023年以来网络安全标准、合规义务和监管框架的重大进展，现有的云基础设施已无法可靠地维护或更新以满足当前的质量和可持续性期望。从技术角度来看，对其进行更新已无任何意义。

尽管云服务将被逐步终止，但以下几个重要方面保持不变：
*   制造商的保修承诺仍然有效。
*   诺拓机器人将继续支持手动操作；按下按钮一次即可启动全屋清扫。
*   在neatorobotics.com网站上仍可获得在线支持和实用帮助。

此决定仅影响诺拓机器人产品，福维克集团的其他产品和服务不受影响。福维克强调，这不是一项出于便利的决定，而是在技术和监管环境发生根本性变化的情况下，为保护用户隐私、数据和安全所必需的步骤。

---

## 80. DMT诱导的临界性转变与自我瓦解相关联。

**原文标题**: DMT-induced shifts in criticality correlate with self-dissolution

**原文链接**: [https://www.jneurosci.org/content/early/2025/10/24/JNEUROSCI.0344-25.2025](https://www.jneurosci.org/content/early/2025/10/24/JNEUROSCI.0344-25.2025)

本研究探讨了迷幻物质DMT对人脑振荡临界性的影响及其与主观体验（尤其是自我消解）的相关性。近临界脑动力学对健康功能至关重要。

研究发现，DMT使α波及邻近频段的脑振荡动力学偏离临界状态，转向亚临界状态。这种转变导致脑活动熵增加但复杂性降低。至关重要的是，在α波和θ波频段观察到的这些临界性转变与所报告的自我消解强度（一种标志性的迷幻体验）直接相关。

本质上，DMT将通常占主导地位的α波振荡转化为一种更安静、亚临界的状态。这些发现对理解迷幻物质的神经学机制以及人脑中意识改变状态的基础具有重要意义。

---

## 81. 秀尔算法：明日终结RSA/ECC的唯一量子算法

**原文标题**: Shor's algorithm: the one quantum algo that ends RSA/ECC tomorrow

**原文链接**: [https://blog.ellipticc.com/posts/what-is-shors-algorithm-and-why-its-the-single-biggest-threat-to-classical-cryptography/](https://blog.ellipticc.com/posts/what-is-shors-algorithm-and-why-its-the-single-biggest-threat-to-classical-cryptography/)

Shor算法是一种量子算法，能够高效地找到大数的质因数，这对于经典计算机来说是计算上不可行的任务。这种能力对现代公钥密码学构成了最大的威胁，尤其是对RSA和ECC算法。

RSA依赖于大数分解的困难性，而ECC依赖于解决离散对数问题的困难性——这两种难题Shor算法都能高效破解。如果建造出足够强大的量子计算机，Shor算法几乎能够解密所有受这些密码方案保护的互联网通信、金融交易和安全数据。

该算法利用量子力学，特别是叠加和纠缠特性，同时探索多种可能性，并找到与被分解数相关的函数的周期。这使得它能够远远优于经典的分解算法。

尽管实用、容错的量子计算机仍需数年才能问世，但这一威胁已经足够重大，值得立即采取行动。专家们预计会出现“先收集，后解密”的情景，即今天收集加密数据，待强大的量子计算机可用时再进行解密。这推动了“后量子密码学”（PQC）的发展——这是一类旨在抵抗量子计算机攻击的新密码算法，NIST正在进行标准化工作。文章强调了组织机构通过过渡到PQC来准备应对这一量子威胁的紧迫性。

---

## 82. 测试显示汽车破窗器无法击碎现代汽车玻璃

**原文标题**: Testing Shows Automotive Glassbreakers Can't Break Modern Automotive Glass

**原文链接**: [https://www.core77.com/posts/138925/Testing-Shows-Automotive-Glassbreakers-Cant-Break-Modern-Automotive-Glass](https://www.core77.com/posts/138925/Testing-Shows-Automotive-Glassbreakers-Cant-Break-Modern-Automotive-Glass)

文章《测试表明汽车破窗器无法打破现代汽车玻璃》指出，常见的汽车逃生工具，特别是破窗器，对现代汽车基本无效。蓬勃发展的“汽车逃生工具市场”主要由基于恐惧的营销推动，这些营销围绕着汽车起火或沉没等罕见场景，以及安全带卡死等统计上微不足道的事件。

这些工具的关键缺陷在于，它们被设计用来打破钢化玻璃，而大多数汽车侧窗*过去*常使用钢化玻璃。然而，现代安全法规（FMVSS 226，2013）已促使大多数汽车制造商——包括几乎所有主要品牌——将侧窗玻璃改为夹层玻璃。夹层玻璃，已经在挡风玻璃中使用，明显更坚韧，旨在防止乘员被甩出车外。

一份AAA研究报告测试了六种常见的破窗器，结果发现没有一个能打破夹层玻璃，其中两个甚至连钢化玻璃都无法打破。尽管安全带切割器对于急救人员解救昏迷的受害者确实有用，但这些工具的破窗功能对现代汽车而言已基本过时，使其仅对老爷车可能有用。

---

## 83. 织物项目

**原文标题**: Fabric Project

**原文链接**: [https://github.com/Fabric-Project/Fabric](https://github.com/Fabric-Project/Fabric)

Fabric是一个创意编程和快速原型开发环境，专为交互式视觉效果、图像/视频处理和3D内容创作而设计。它受Apple的Quartz Composer启发，具有直观的视觉节点式界面，并提供用于内容加载和通过插件创建自定义节点的SDK。

它是一个工具，适用于需要少量编程的创意程序员、创建可嵌入第三方应用程序的可复用文档的专业用户，以及使用其底层Satin引擎构建高保真视觉效果的开发者。Fabric支持创建交互式3D图形、图像效果、音频响应场景和视频分析管道。

主要功能包括物理渲染（PBR）、场景图、光照/阴影、实时着色器编辑、GPU计算、基于图像的光照、3D模型加载和基于机器学习的分割。它集成了Satin 3D引擎（由@Reza Ali开发）和Lygia着色器库的Metal移植版本（由@Patricio Gonzalez Vivo开发）。

目前处于早期alpha阶段，且“正在大规模开发中”，Fabric需要macOS 14及更高版本和Xcode 15及更高版本。为开发者提供了架构文档、教程和示例以作指导。Fabric是专为Apple平台使用Metal、Swift和SwiftUI而构建的，暂无跨平台兼容性计划。其创建者Anton Marini正在积极建立社区，寻求重视其相较于其他节点式工具独特方法的贡献者。

---

## 84. 猫远比你想象的要晚才成为我们的伙伴。

**原文标题**: Cats became our companions way later than you think

**原文链接**: [https://www.bbc.co.uk/news/articles/cq8dvdp9gn7o](https://www.bbc.co.uk/news/articles/cq8dvdp9gn7o)

新科学证据表明，猫成为人类伙伴的时间比之前认为的晚得多，地点也不同。与“驯化始于10000年前的黎凡特地区”这一观点相反，一项对古代猫骨骼DNA的研究指出，猫与人类的联系仅在3500至4000年前的北非，很可能是埃及开始。所有现代家猫都源自非洲野猫。

这一修正后的时间线与古埃及人对猫的崇敬相符。猫因被视为害虫防治者和船只伴侣而受到重视，随后在全球传播开来，约2000年前随罗马人抵达欧洲，随后经丝绸之路东传至中国。

一个意想不到的发现是，科学家们发现，另一种物种——豹猫，在中国与人类共生了约3500年，比家猫的到来还要早。这些豹猫作为天然的啮齿动物捕食者，从人类定居点中受益，但它们从未被驯化，在亚洲各地仍保持野性。值得注意的是，它们最近与家猫杂交，培育出了孟加拉猫。这项研究挑战了既定的猫驯化时间线。

---

## 85. Africa's forests have switched from absorbing to emitting carbon

**原文标题**: Africa's forests have switched from absorbing to emitting carbon

**原文链接**: [https://phys.org/news/2025-11-africa-forests-absorbing-emitting-carbon.html](https://phys.org/news/2025-11-africa-forests-absorbing-emitting-carbon.html)

生成摘要时出错

---

## 86. Copenhagenize Index 2025: The Global Ranking of Bicycle-Friendly Cities

**原文标题**: Copenhagenize Index 2025: The Global Ranking of Bicycle-Friendly Cities

**原文链接**: [https://copenhagenizeindex.eu/](https://copenhagenizeindex.eu/)

生成摘要时出错

---

## 87. Jedi Blue

**原文标题**: Jedi Blue

**原文链接**: [https://en.wikipedia.org/wiki/Jedi_Blue](https://en.wikipedia.org/wiki/Jedi_Blue)

生成摘要时出错

---

## 88. Chainalysis Successful Deanonymization Attack on Monero

**原文标题**: Chainalysis Successful Deanonymization Attack on Monero

**原文链接**: [https://darkwebinformer.com/chainalysis-successful-deanonymization-attack-on-monero-2/](https://darkwebinformer.com/chainalysis-successful-deanonymization-attack-on-monero-2/)

生成摘要时出错

---

## 89. Show HN: An LLM-Powered Tool to Catch PCB Schematic Mistakes

**原文标题**: Show HN: An LLM-Powered Tool to Catch PCB Schematic Mistakes

**原文链接**: [https://netlist.io/](https://netlist.io/)

生成摘要时出错

---

## 90. Migrating to Positron, a next-generation data science IDE for Python and R

**原文标题**: Migrating to Positron, a next-generation data science IDE for Python and R

**原文链接**: [https://posit.co/blog/positron-migration-guides](https://posit.co/blog/positron-migration-guides)

生成摘要时出错

---

## 91. KDE going all-in on a Wayland future

**原文标题**: KDE going all-in on a Wayland future

**原文链接**: [https://blogs.kde.org/2025/11/26/going-all-in-on-a-wayland-future/](https://blogs.kde.org/2025/11/26/going-all-in-on-a-wayland-future/)

生成摘要时出错

---

## 92. Writing Builds Resilience in Everyday Challenges by Changing Your Brain

**原文标题**: Writing Builds Resilience in Everyday Challenges by Changing Your Brain

**原文链接**: [https://scienceclock.com/writing-builds-resilience-in-everyday-challenges-by-changing-your-brain/](https://scienceclock.com/writing-builds-resilience-in-everyday-challenges-by-changing-your-brain/)

生成摘要时出错

---

## 93. OpenAI won't make money by 2030 and needs another $207B, HSBC estimates

**原文标题**: OpenAI won't make money by 2030 and needs another $207B, HSBC estimates

**原文链接**: [https://fortune.com/2025/11/26/is-openai-profitable-forecast-data-center-200-billion-shortfall-hsbc/](https://fortune.com/2025/11/26/is-openai-profitable-forecast-data-center-200-billion-shortfall-hsbc/)

生成摘要时出错

---

## 94. Users brutually reject Microsoft's "Copilot for work" in Edge and Windows 11

**原文标题**: Users brutually reject Microsoft's "Copilot for work" in Edge and Windows 11

**原文链接**: [https://www.windowslatest.com/2025/11/28/you-heard-wrong-users-brutually-reject-microsofts-copilot-for-work-in-edge-and-windows-11/](https://www.windowslatest.com/2025/11/28/you-heard-wrong-users-brutually-reject-microsofts-copilot-for-work-in-edge-and-windows-11/)

生成摘要时出错

---

## 95. ML-KEM Mythbusting

**原文标题**: ML-KEM Mythbusting

**原文链接**: [https://keymaterial.net/2025/11/27/ml-kem-mythbusting/](https://keymaterial.net/2025/11/27/ml-kem-mythbusting/)

生成摘要时出错

---

## 96. Show HN: I built Magiclip – an all-in-one AI studio

**原文标题**: Show HN: I built Magiclip – an all-in-one AI studio

**原文链接**: [https://magiclip.io/](https://magiclip.io/)

生成摘要时出错

---

## 97. How to Short the Bubbliest Firms

**原文标题**: How to Short the Bubbliest Firms

**原文链接**: [https://www.economist.com/finance-and-economics/2025/11/26/how-to-short-the-bubbliest-firms](https://www.economist.com/finance-and-economics/2025/11/26/how-to-short-the-bubbliest-firms)

生成摘要时出错

---

## 98. Rock Paper Scissors Solitaire

**原文标题**: Rock Paper Scissors Solitaire

**原文链接**: [https://klezlab.it/rock-paper-scissors-solitaire.html](https://klezlab.it/rock-paper-scissors-solitaire.html)

生成摘要时出错

---

## 99. Louvre to hike ticket prices for most non-EU tourists by 45%

**原文标题**: Louvre to hike ticket prices for most non-EU tourists by 45%

**原文链接**: [https://www.bbc.com/news/articles/clyd4llgrego](https://www.bbc.com/news/articles/clyd4llgrego)

生成摘要时出错

---

## 100. Codex, Opus, Gemini Try to Build Counter Strike

**原文标题**: Codex, Opus, Gemini Try to Build Counter Strike

**原文链接**: [https://www.instantdb.com/essays/agents_building_counterstrike](https://www.instantdb.com/essays/agents_building_counterstrike)

生成摘要时出错

---

