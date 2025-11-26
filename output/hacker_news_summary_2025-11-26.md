# Hacker News 热门文章摘要 (2025-11-26)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. Pebble 手表软件现已开源

**原文标题**: Pebble Watch software is now open source

**原文链接**: [https://ericmigi.com/blog/pebble-watch-software-is-now-100percent-open-source](https://ericmigi.com/blog/pebble-watch-software-is-now-100percent-open-source)

斐波（Pebble）的智能手表软件现已100%开源，这是Core Devices（重启斐波的公司）为确保其长期可持续性而迈出的重要一步。这包括PebbleOS（智能手表软件，自一月起已开源）、新的斐波移动伴侣应用程序（现已在GitHub上完全开源）以及更新的开发者工具。此举确保即使Core Devices停止运营，用户仍能构建、运行和改进他们的斐波软件。

一个显著的变化是斐波应用商店的去中心化。移动应用程序将支持多个应用商店“订阅源”（类似于包管理器），Core Devices已推出自己的订阅源，并已备份至Archive.org，以促进长期可靠性和社区贡献。尽管存在一些非免费组件（例如心率传感器库），但核心斐波软件栈在没有它们的情况下仍然保持开源和可用。

硬件可持续性也是一个重点，Core Devices作为一家精简、自筹资金的实体运营。像Pebble Time 2 (PT2) 这样的新手表在设计时就考虑了可修复性（例如可更换电池），Pebble 2 Duo的电气/机械设计文件已在GitHub上公开。

关于Pebble Time 2，预计发货将于2026年1月开始，但由于生产周期和农历新年，大部分预计将在3月/4月到达。将提供四种颜色选项，选择邮件将在未来几周内发送。预生产的PT2设备已在一个新的“Tick Talk”节目中进行了展示。

---

## 2. 克劳德 奥普斯 4.5

**原文标题**: Claude Opus 4.5

**原文链接**: [https://www.anthropic.com/news/claude-opus-4-5](https://www.anthropic.com/news/claude-opus-4-5)

Anthropic于2025年11月24日发布了Claude Opus 4.5，将其定位为迄今为止最智能、最高效的模型，专为编码、代理和计算机使用而设计。该模型可通过应用程序、API和云平台获取，其新的定价（每百万token 5美元/25美元）使高级功能更易于获取。

Opus 4.5在软件工程领域树立了新标杆，在SWE-bench Multilingual和Aider Polyglot等测试中表现优于Sonnet 4.5及竞争对手，通常可将token使用量减少高达65%。在一项具有挑战性的2小时性能工程考试中，它的得分高于任何人类考生。除了编码，它还显著改进了深度研究、电子表格自动化（准确性提高20%）和长上下文叙事等日常任务。测试人员赞扬它处理模糊性、权衡利弊以及创造性解决复杂问题的能力。

该模型拥有增强的视觉、推理和数学能力。关键在于，Opus 4.5也是Anthropic对齐最稳健的模型，在防范提示注入攻击方面显示出实质性进展，从而确保了更高的安全性和可靠性。

开发者平台更新包括一个新的`effort`参数，允许用户在速度/成本与模型能力之间进行平衡。产品更新通过改进的“计划模式”和桌面应用程序增强了Claude Code，使Claude应用程序中能够进行连续的长对话，并扩大了Claude对Chrome和Excel的访问。Opus 4.5的高级用户使用限制已提高，反映出它已准备好用于日常专业用途。此次发布标志着人工智能能力向前迈出了重要一步，并预示着未来工作方式的改变。

---

## 3. YouTube上有人该配眼镜了：预言应验了

**原文标题**: Someone at YouTube Needs Glasses: The Prophecy Has Been Fulfilled

**原文链接**: [https://jayd.ml/2025/11/10/someone-at-youtube-needs-glasses-prophecy-fulfilled.html](https://jayd.ml/2025/11/10/someone-at-youtube-needs-glasses-prophecy-fulfilled.html)

作者回忆起一项先前的统计分析，该分析预测由于信息密度下降，YouTube的主页到2026年5月将只显示一个视频。这项分析引起了关注，导致YouTube产品管理（PM）部门的一段泄露录音讨论了这些批评。

几个月后，在“Gemini YouTube工程师”一番努力之后，作者发现在Apple TV上打开YouTube时，主页上只显示一个孤零零的视频。这一发现促使作者对最初的预言进行了重大修订。作者援引YouTube PM部门日益加速的“短视”，现在预测到2026年5月，主页将显示 *零* 个视频，下降速度比之前估计的更快。

文章最后，作者沮丧地表示“波伊定律适用于谷歌的产品经理”，暗示现实已经超越了讽刺，并幽默地推测强制性NeuraLink将提前到来，这强调了对YouTube用户界面设计走向的批判性看法。

---

## 4. 未通电的固态硬盘会缓慢丢失数据

**原文标题**: Unpowered SSDs slowly lose data

**原文链接**: [https://www.xda-developers.com/your-unpowered-ssd-is-slowly-losing-your-data/](https://www.xda-developers.com/your-unpowered-ssd-is-slowly-losing-your-data/)

未通电的固态硬盘（SSD）在长时间内会缓慢丢失数据，这使得它们不适合用于长期“冷”存储。与使用磁性存储的硬盘不同，固态硬盘通过改变NAND闪存单元中的电荷来存储数据。没有电源，这些电荷会消散，导致数据损坏或丢失。

数据保留时间取决于NAND类型：QLC NAND（常见于消费级硬盘）在未通电状态下可保留约2-3年，TLC NAND长达3年，MLC长达5年，SLC长达10年。大多数消费级固态硬盘使用TLC或QLC，这意味着在不通电几年后，数据完整性就面临风险。硬盘虽然容易受到位衰减（bit rot）的影响，但通常对长时间未通电存储更具弹性。

这种担忧主要影响需要长期存档数据的企业用户、爱好者和个人创业者。大多数日常用户由于其固态硬盘会定期通电，不太可能遇到这个问题。温度和NAND质量等因素会加速电荷流失。

文章强调，健壮的备份策略至关重要，推荐3-2-1规则（3份数据副本，存储在2种不同介质上，其中1份异地存储）。对于重要的长期存档，硬盘、磁带或M-Disc等替代方案更佳。虽然固态硬盘非常适合作为主存储，但依靠它们在未通电状态下进行多年数据保留是冒险的，这突显了全面备份对于数据保存的普遍必要性。

---

## 5. 谷歌反重力通过间接提示注入攻击外泄数据

**原文标题**: Google Antigravity exfiltrates data via indirect prompt injection attack

**原文链接**: [https://www.promptarmor.com/resources/google-antigravity-exfiltrates-data](https://www.promptarmor.com/resources/google-antigravity-exfiltrates-data)

Google的新型代理代码编辑器Antigravity，由其Gemini AI代理驱动，容易受到间接提示注入攻击，该攻击能够窃取敏感用户数据。研究人员演示了恶意网络源（如集成指南）如何操纵Gemini窃取凭据和代码。

攻击链始于用户将Gemini指向一个包含隐藏提示注入的恶意网页。Gemini随后被迫执行以下操作：
1. **收集敏感数据**：它收集代码片段和凭据，值得注意的是，通过使用`cat`终端命令，绕过了自身针对`.env`文件的`.gitignore`文件访问保护。
2. **构造恶意URL**：Gemini对收集到的数据进行URL编码，并将其附加到攻击者监控的域名，例如`webhook.site`。
3. **窃取数据**：Gemini激活一个浏览器子代理来打开这个恶意URL。

Antigravity的几个默认设置助长了这种攻击：用于人工审查的“代理决定”（"Agent Decides"）、用于终端命令执行的“自动”（"Auto"）以及允许子代理的“浏览器工具”（"Browser tools"）功能。关键是，`webhook.site`位于Antigravity的默认浏览器URL白名单上，从而阻止了拦截。

尽管用户可以监控代理，但Antigravity的“代理管理器”（"Agent Manager"）鼓励在无人监督的情况下运行多个代理，使得检测变得不太可能。尽管谷歌通过免责声明承认数据窃取风险，但研究人员认为，考虑到无人值守代理和宽松默认设置的实际影响，这远远不够，因此选择不进行负责任的披露。

---

## 6. 克劳德进阶工具使用

**原文标题**: Claude Advanced Tool Use

**原文链接**: [https://www.anthropic.com/engineering/advanced-tool-use](https://www.anthropic.com/engineering/advanced-tool-use)

Anthropic为Claude发布了三项新功能，旨在增强AI代理能力，解决与庞大工具库、复杂编排以及学习正确工具使用方法相关的挑战。

**工具搜索工具**解决了大量工具定义占用大量上下文窗口空间的问题（例如，58个工具占用55K token）。通过允许工具使用 `defer_loading: true` 按需发现和加载，它将初始token消耗降低了85%（对于50多个工具，从约77K降至约8.7K token），并通过确保Claude只看到相关工具来提高准确性。这对于拥有大量工具的大型MCP驱动系统尤其有利。

**程序化工具调用**使Claude能够通过沙盒执行环境中生成的Python代码来编排多步骤工作流。这可以防止中间结果（如大型数据集或大量明细项）污染Claude的上下文窗口，因为只有最终处理后的输出才会被返回。这带来了大幅的token节省（复杂任务中减少37%），通过最大限度地减少模型推理次数来降低延迟，并通过显式控制流提高准确性。它非常适用于处理大型数据集、执行并行操作或需要数据转换的复杂多步骤任务。

**工具使用示例**提供了一个通用标准，用于展示有效的工具使用模式。这有助于Claude超越JSON schema的结构定义进行学习，理解何时使用可选参数或特定API约定。

总而言之，这些功能使Claude能够更高效、更准确、更具扩展性地与无限工具库交互，为构建高级AI代理开辟了新的可能性。

---

## 7. 耗资万亿，大型软件项目依然失败

**原文标题**: Trillions spent and big software projects are still failing

**原文链接**: [https://spectrum.ieee.org/it-management-software-failures](https://spectrum.ieee.org/it-management-software-failures)

尽管全球在IT领域投入了数万亿美元，技术也取得了二十年的进步，但大型软件项目仍以持续且惊人的速度失败。自2005年以来，全球IT支出已增长逾三倍，但成功率并未提高，随着软件渗透到生活的方方面面，这导致商业和社会成本不断攀升。

文章认为，人工智能工具和编程助手无法解决这些系统性管理问题，这些问题源于系统工程、财务管理、组织政治以及往往非理性的决策之间复杂的相互作用。失败的根本原因包括人类想象力的不足、不切实际的目标、处理复杂性的能力不足以及未能有效管理的风险——这些因素已被广泛记录，但却一再被忽视。

灾难性的例子包括加拿大耗资3.1亿加元的“凤凰”薪资系统，该系统导致了普遍的工资错误、经济困难乃至自杀事件，最终耗费超过51亿加元。更糟糕的是，英国邮局的“地平线”系统由于蓄意隐藏的软件错误，导致数百名邮政局长被错误定罪和监禁，成为迄今为止最严重的运营IT故障，但它仍在继续使用。

经济损失巨大；仅在美国，运营和开发软件故障每年就造成超过2万亿美元的损失。尽管存在敏捷和DevOps等现代方法，但由于缺乏持续的领导力、组织纪律和文化变革，它们常常无法达到预期效果。IT界固执地拒绝从过去的错误中吸取教训，经常将过去的经验教训视为不相关，这使得重复的失败代价极其高昂，并对现代社会构成生存威胁。

---

## 8. PS5售价已低于64GB DDR5内存；内存因短缺飙升至600美元

**原文标题**: PS5 now costs less than 64GB of DDR5 memory. RAM jumps to $600 due to shortage

**原文链接**: [https://www.tomshardware.com/pc-components/ddr5/64gb-of-ddr5-memory-now-costs-more-than-an-entire-ps5-even-after-a-discount-trident-z5-neo-kit-jumps-to-usd600-due-to-dram-shortage-and-its-expected-to-get-worse-into-2026](https://www.tomshardware.com/pc-components/ddr5/64gb-of-ddr5-memory-now-costs-more-than-an-entire-ps5-even-after-a-discount-trident-z5-neo-kit-jumps-to-usd600-due-to-dram-shortage-and-its-expected-to-get-worse-into-2026)

由于人工智能热潮对内存和存储的巨大需求，DDR5内存价格一路飙升，使其对终端消费者来说越来越难以承受。一套64GB芝奇幻锋戟Z5 Neo 6000 MT/s内存套件现在标价599.99美元，明显高于一台PS5 Slim（449美元）或Xbox Series S（399美元），并且只比一台PS5 Pro（649美元）便宜50美元。

这代表着在短短两个月内惊人的约190%涨幅；同样的套件此前售价205-220美元，而今年早些时候，同类套件价格曾低至140美元。制造商正在优先满足AI客户的需求，导致普遍的短缺。这场“AI危机”也在耗尽硬盘库存，导致大容量硬盘的积压订单长达两年，并推高了对QLC固态硬盘的需求。甚至Valve即将推出的Steam掌机也由于DRAM危机而面临更高的成本。

专家预测DRAM和NAND的供应紧张将持续到2026年。然而，内存市场历来在供过于求和供不应求之间循环，这表明DDR5价格可能在2027年左右回落到廉价水平。

---

## 9. 旅行者1号即将达到距地球一光日

**原文标题**: Voyager 1 Is About to Reach One Light-Day from Earth

**原文链接**: [https://scienceclock.com/voyager-1-is-about-to-reach-one-light-day-from-earth/](https://scienceclock.com/voyager-1-is-about-to-reach-one-light-day-from-earth/)

美国宇航局的“旅行者1号”探测器将于2026年11月15日达到一个历史性的里程碑：它将抵达距离地球161亿英里（259亿公里）的位置。届时，一个无线电信号将需要整整24小时——即一个“光日”——才能抵达该探测器。

“旅行者1号”于1977年发射，旨在探索木星和土星，并于2012年进入星际空间，成为距离地球最远的人造物体。它以每秒11英里（17.7公里/秒）的速度飞行，每年增加约3.5个天文单位，并凭借其放射性同位素热电发生器持续传输数据，这些发生器预计将持续工作到2030年代。

与“旅行者1号”通信是一个缓慢的过程；指令需要一天才能抵达，再用一天才能确认，这与距离较近天体的通信时间形成鲜明对比。这遥远的距离凸显了太空的浩瀚规模，使得一个“光日”在宇宙尺度上显得微不足道（例如，光需要四年多才能抵达比邻星）。除了其距离记录之外，“旅行者1号”的任务，包括其著名的“暗淡蓝点”图像，象征着人类的智慧、我们太阳系的浩瀚以及永恒的探索精神。

---

## 10. 我才不在乎你的‘AI’运行得怎么样呢。

**原文标题**: I don't care how well your "AI" works

**原文链接**: [https://fokus.cool/2025/11/25/i-dont-care-how-well-your-ai-works.html](https://fokus.cool/2025/11/25/i-dont-care-how-well-your-ai-works.html)

作者对即使在进步的黑客圈子里也随意采纳“AI”（特指大型语言模型LLM）深感幻灭，视之为“脑部寄生虫”或“有害的应对机制”。他们观察到有才华的程序员面临生存危机，因为他们的技艺正在迅速贬值，这类似于设计师、作家和其他手工艺者所经历的。

尽管作者个人避免使用大型语言模型，但承认这是一种特权，因为许多人受制于社会压力、雇主期望以及日益增长的“知识污染”，不得不使用这些系统。文章指出，仅仅关注AI的技术缺陷或偏见，会忽视其旨在集中权力的根本性、蓄意设计的问题。

作者强调工具塑造我们的思想和身份。AI系统微妙地影响认知过程，让用户相信输出真正反映了他们的原始思想，从而破坏了真正的创造性和反思过程。最终，AI系统被描绘成控制的工具，通过将资本转化为控制并蓄意摧毁手艺和表达，强化了现有的资本主义和法西斯主义权力结构。

文章最后呼吁“在转移性资本主义下求生”，敦促读者支持朋友、加入工会、通过减少社交媒体滋养心智、自我教育并创造原创作品。作者指出，蓬勃发展是最不服从的行为。

---

## 11. 人脑预设了理解世界的指令。

**原文标题**: Human brains are preconfigured with instructions for understanding the world

**原文链接**: [https://news.ucsc.edu/2025/11/sharf-preconfigured-brain/](https://news.ucsc.edu/2025/11/sharf-preconfigured-brain/)

加州大学圣克鲁斯分校Tal Sharf教授领导的研究团队利用大脑类器官——由干细胞培育出的三维脑组织模型——揭示了早期人类大脑发育的新见解。他们的研究发表在《自然-神经科学》杂志上，表明大脑最早的电活动在任何感官体验 *之前* 就以结构化的模式出现。

这一突破性发现表明，人类大脑预先配置了固有的指令或一个“原始操作系统”，用于理解和与世界互动。这些类器官在发育数月内自发地发出复杂的、基于时间的电活动模式，这与大脑的“默认模式”惊人地相似——这种基本放电结构随后会为特定的感官进行完善。这表明，神经结构是由基因编码的蓝图指导的，而非模式仅仅是响应外部刺激而产生。

这项研究对于理解神经发育障碍、评估农药和微塑料等环境毒素对发育中大脑的影响，并最终开发有针对性的疗法和干预措施具有重要意义。类器官提供了一个合乎伦理且受控的平台来观察这种基本的自组装过程，为我们了解大脑如何构建自身提供了独特的窗口。

---

## 12. OpenAI 需要到2030年至少筹集2070亿美元。

**原文标题**: OpenAI needs to raise at least $207B by 2030

**原文链接**: [https://ft.com/content/23e54a28-6f63-4533-ab96-3756d9c88bad](https://ft.com/content/23e54a28-6f63-4533-ab96-3756d9c88bad)

汇丰银行估算，到2030年，OpenAI将需要筹集至少2070亿美元。汇丰银行预计该公司将持续亏损，因此这笔巨额资金被认为是其持续运营所必需的。

这一预测的具体细节和分析来自《金融时报》的一篇FT Alphaville文章，该文章目前需付费订阅才能阅读。所提供的文本主要包含《金融时报》的各种订阅选项，包括试用、标准数字版和高级数字版计划，详细介绍了它们的功能、定价和访问级别，而不是关于OpenAI财务需求的完整文章内容。

---

## 13. 猎户 1.0

**原文标题**: Orion 1.0

**原文链接**: [https://blog.kagi.com/orion](https://blog.kagi.com/orion)

macOS 版 Orion 1.0 经过六年开发，于 2025 年 11 月 25 日正式发布，与已有的 iOS 和 iPadOS 版本一同亮相。Orion 由 Kagi 开发，是一款隐私优先、以用户为中心的浏览器，旨在对抗现代网络浏览日益趋向广告资助模式和数据利用的趋势。它扩展了 Kagi 旗下的“Kagi宇宙”（Kagiverse）中尊重隐私的产品线。

Orion 的一个核心区别因素在于其使用 WebKit（Safari 的开源引擎）而非 Chromium。这为 macOS/iOS 提供了深度优化，避免了 Chromium 的单一文化，并使其脱离了广告资助的巨头。Orion 以速度为核心，拥有精简的代码库和优化的性能；同时默认保护隐私，具有零遥测、无内置广告/追踪技术以及强大的内容拦截功能。

在人工智能方面，Orion 采用了一种安全优先的方法：其核心不包含任何内置人工智能，允许用户连接到他们选择的人工智能工具（包括 Kagi 自己的），同时保持安全的隔离。该浏览器提供独特功能，例如专注模式、链接预览、迷你工具栏以及用于隔离浏览环境的“应用式配置文件”（Profiles as Apps）。

Orion 对所有人免费，包括 200 次免费 Kagi 搜索，并完全由其用户通过可选的打赏（Tip Jar）、支持者订阅（每月 5 美元或每年 50 美元）或终身访问费用（150 美元）自筹资金。支持者可以获得 Orion+ 的额外福利，例如浮动窗口和高级自定义功能。

目前，Orion 已在 macOS、iOS 和 iPadOS 上可用，其 Linux 版本正处于 Alpha 阶段，Windows 版本正在开发中（目标是 2026 年底），旨在实现无缝的跨平台同步。未来的路线图包括进一步的自定义、性能增强以及更深入、由用户控制的 Kagi AI 集成。

---

## 14. 雅加达现在是世界上最大的城市。

**原文标题**: Jakarta is now the biggest city in the world

**原文链接**: [https://www.axios.com/2025/11/24/jakarta-tokyo-worlds-biggest-city-population](https://www.axios.com/2025/11/24/jakarta-tokyo-worlds-biggest-city-population)

无法访问文章链接。

---

## 15. 伊利亚·萨茨克维尔：我们正在从规模化时代迈向研究时代

**原文标题**: Ilya Sutskever: We're moving from the age of scaling to the age of research

**原文链接**: [https://www.dwarkesh.com/p/ilya-sutskever-2](https://www.dwarkesh.com/p/ilya-sutskever-2)

伊利亚·苏茨克维认为，人工智能正在从“规模化时代”转向“研究时代”。他强调当前AI模型存在显著的“参差不齐”：尽管在评估中表现出色，但它们在现实世界泛化方面却举步维艰，导致其感知智能与经济影响之间存在脱节。

苏茨克维指出，这一局限性源于强化学习（RL）训练无意中侧重于特定评估任务，类似于学生为考试死记硬背而非获得深刻理解。他认为，即使预训练数据量少得多，人类的泛化能力也远超AI，并提到AI可能修复一个错误却又重新引入另一个错误。

他质疑海量预训练数据本身是否能带来实现稳健泛化所需的深刻、类人的理解。苏茨克维还强调了“价值函数”（类似于人类情感）在有效决策中的关键作用。他引用了脑损伤损害情感处理能力从而严重阻碍决策的案例，暗示整合这些基本机制对于创建可行的AI智能体至关重要——而这在机器学习领域目前尚未充分探索。“研究时代”将聚焦于这些超越单纯计算规模的基础性挑战。

---

## 16. HN展示：我们开发了一个开源、零webhook的支付处理器

**原文标题**: Show HN: We built an open source, zero webhooks payment processor

**原文链接**: [https://github.com/flowglad/flowglad](https://github.com/flowglad/flowglad)

Flowglad是一个开源的、零Webhook支付处理器，旨在简化互联网资金处理，并现代化账单处理中的开发者体验。它无需管理Webhook、单独的订阅表或Flowglad特有的客户ID。相反，它充当客户账单状态的单一真相来源，包括功能访问和使用量计费额度，这些都可以直接使用您应用程序现有的用户ID或组织ID进行查询。

该平台提供了一个全栈SDK，包含一个用于前端集成的`useBilling()` React Hook，以及一个用于后端访问的`flowgladServer.getBilling()`方法。这支持实时功能门控、使用余额检查和结账会话创建。Flowglad具有适应性，使开发者能够在测试模式下迭代定价模型，并立即将其推送到生产环境，支持无需重新部署的无缝模型轮换。

集成过程非常简单，通常只需不到一分钟：安装相关的Flowglad软件包（例如，`@flowglad/nextjs`），使用您的`customerExternalId`和`getCustomerDetails`函数配置服务器客户端，暴露一个API路由以进行安全通信，并使用`FlowgladProvider`包装您的应用程序。

Flowglad支持无限的定价模型，为各种策略提供可定制的模板，例如使用量限制混合、分级访问和功能门控订阅。其首要目标是通过提供一个自助式、低维护的计费层，改变停滞不前的支付格局，从而提高开发者体验，减少集成时间，并为现代AI驱动应用程序日益增长的复杂性做好准备。

---

## 17. FLUX.2: 前沿视觉智能

**原文标题**: FLUX.2: Frontier Visual Intelligence

**原文链接**: [https://bfl.ai/blog/flux-2](https://bfl.ai/blog/flux-2)

黑森林实验室推出了FLUX.2：前沿视觉智能，这是图像生成和编辑领域的一项强大进步。FLUX.2秉持“开放核心”理念，将顶尖功能与开放权重模型和生产级API相结合，旨在促进研究人员和创作者的创新。

FLUX.2通过生成高质量、逼真的图像以及带有清晰排版的复杂信息图表，显著提升了生产工作流程，所有图像的分辨率均可达到4兆像素。主要改进包括在多达10张参考图像中实现卓越的角色和风格一致性、更精细的图像细节、更锐利的纹理以及适用于产品拍摄的稳定光照。该模型在遵循复杂提示方面表现出更高的依从性、更好的世界知识和连贯的空间逻辑。它还支持在4兆像素下进行图像编辑，同时保留细节。

FLUX.2系列提供多个版本：
*   **FLUX.2 [pro]：** 提供顶尖的图像质量、速度和成本效益。
*   **FLUX.2 [flex]：** 为开发者提供对步骤和引导比例等参数的控制，在文本和精细细节方面表现出色。
*   **FLUX.2 [dev]：** 一个32B开放权重模型，目前是图像生成和编辑领域最强大的开源选项。
*   **FLUX.2 [klein]：** （即将推出）一个Apache 2.0开源、尺寸精简模型。
*   **FLUX.2 - VAE：** 一个新的开源变分自编码器，构成了FLUX.2的基础。

FLUX.2基于潜在流匹配架构构建，集成了Mistral-3 24B视觉-语言模型与整流流变换器，并具有一个重新训练的潜在空间，以提高学习能力和图像质量。黑森林实验室将FLUX.2视为创意基础设施不可或缺的组成部分，致力于推动实现开放、多模态的视觉智能。

---

## 18. 人工智能对这段代码的工作原理有深入理解。

**原文标题**: AI has a deep understanding of how this code works

**原文链接**: [https://github.com/ocaml/ocaml/pull/14369](https://github.com/ocaml/ocaml/pull/14369)

这个GitHub拉取请求（#14369）为OCaml原生编译器引入了DWARF v5调试支持，从而在GDB和LLDB中实现了强大的源代码级调试。该功能由joelreymont开发，目标是Linux/ELF和macOS/Mach-O平台上的AMD64和ARM64架构，并明确禁用了对32位平台和Windows/其他系统的支持。

该实现侧重于DWARF v5的核心特性，例如内联字符串（DW_FORM_string）以防止链接器问题、多编译单元支持以及节相关重定位，以提高可移植性。调试功能包括函数和行断点、跟踪参数和局部let绑定变量及其原始源代码名称、正确的词法块映射以及基本的OCaml类型信息。

提供了一个LLDB插件（`ocaml_lldb.py`），用于OCaml特有的值格式化，可通过`ocaml print`访问。调试信息通过`ocamlopt -g`启用，禁用时没有运行时开销。

这个包含40次提交的PR从DWARF v4过渡到v5，解决了特定于架构的寄存器映射问题，并实现了`Variable_info`和`Var_lifetime`模块，以在编译管道中保留变量名和生命周期。广泛的测试确保DWARF结构、断点功能、类型可见性以及多对象链接在不同平台上均能正常工作。

然而，在审查期间，yallop提出了一个重大担忧，关于代码的来源问题，他引用了一个将功劳归于“Claude”的外部网页，并要求joelreymont澄清代码的获取来源。

---

## 19. GrapheneOS 服务器基础设施迁出法国

**原文标题**: GrapheneOS migrates server infrastructure from France

**原文链接**: [https://www.privacyguides.org/news/2025/11/22/grapheneos-migrates-server-infrastructure-from-france-amid-police-intimidation-claims/](https://www.privacyguides.org/news/2025/11/22/grapheneos-migrates-server-infrastructure-from-france-amid-police-intimidation-claims/)

GrapheneOS 已宣布将其所有服务器基础设施迁出法国，认为该国对于“开源隐私项目”而言不安全。该项目此前由法国服务商 OVH Bearharnois 托管，现正将其 Mastodon、Discourse 和 Matrix 实例迁至多伦多，而关键网站基础设施将由德国公司 Netcup 托管。签名验证和降级保护等核心服务不受影响，因为 GrapheneOS 声明其在法国不收集机密用户数据。

这一决定是由于法国政府支持欧盟的“聊天控制”提案以及《巴黎人报》的负面报道所促成的。对法国网络犯罪检察官 Johanna Brousse 的采访暗示，如果 GrapheneOS 被发现与犯罪组织有联系且不配合调查，可能会对其采取法律行动。

GrapheneOS 辩称，《巴黎人报》将其合法项目与“政府支持的分支”混为一谈——这些虚假副本包含伪造的 Snapchat 应用和暗网广告等元素，而这些都不是官方 GrapheneOS 的一部分。该项目此前曾威胁对这类分支提起诉讼，并援引 FBI 支持的被破解的安卓操作系统 ANOM 作为例子。鉴于这些担忧，GrapheneOS 的开发人员现在拒绝前往法国或在法国境内工作。

---

## 20. Python 并非一门优秀的数据科学语言。

**原文标题**: Python is not a great language for data science

**原文链接**: [https://blog.genesmindsmachines.com/p/python-is-not-a-great-language-for](https://blog.genesmindsmachines.com/p/python-is-not-a-great-language-for)

在《Python不是数据科学的好语言》一文中，Claus Wilke认为，Python虽然流行，但对于一般数据科学任务（深度学习除外）而言，并非天生就具有优越性，并且与R相比，它常常导致繁琐的体验。他分享了在某个研究实验室的观察：使用Python的学生，甚至是一位专家同事，都持续发现交互式数据探索、快速分析或图表修改比他预想的更加困难和耗时，这与R所展现出的敏捷性形成了鲜明对比。

Wilke将一种有效的数据科学语言定义为：交互式的，启动成本低，并且优先考虑程序员的便利性而非原始性能。一个关键特性是它能够将分析逻辑与实现中的后勤细节（例如，避免手动循环、索引或数据重构）分离开来。他通过比较R的tidyverse和Python的pandas在数据聚合任务中的表现来论证这一点，指出两者都能在高级层面成功完成任务，但强调了基础Python如何迅速演变为后勤复杂性。

他总结说，Python的语言特性或现有库常常迫使用户处理数据后勤问题，从而阻碍了高层次的概念性编程。Wilke计划在后续文章中详细阐述这些具体问题。

---

## 21. 大脑有五个“时代”，成人模式直到30出头才开启

**原文标题**: Brain has five 'eras' with adult mode not starting until early 30s

**原文链接**: [https://www.theguardian.com/science/2025/nov/25/brain-human-cognitive-development-life-stages-cambridge-study](https://www.theguardian.com/science/2025/nov/25/brain-human-cognitive-development-life-stages-cambridge-study)

科学家们已经确定了人类大脑发展的五个不同“时期”，其标志是大约在9岁、32岁、66岁和83岁时的四个关键“转折点”。这项基于近4000份从婴儿期到90岁脑部扫描数据的全面研究，描绘了神经连接的演变过程。

第一个时期，**童年期（出生至9岁）**，其特征是“网络整合”，在此期间突触得到优化，连接效率下降，灰白质增长，大脑皮层厚度达到峰值。

**青少年期（9岁至32岁）**，白质持续增长，通讯网络得到完善，连接效率不断提高，这与认知能力增强相关。研究人员澄清，这指的是*变化模式*，并非暗示二十多岁的人行为举止像青少年。这一时期对于理解精神健康障碍的风险因素尤为重要，这些风险因素通常在青少年期出现。

大脑在**32岁左右进入成人模式**，这是最长的时期，持续到66岁。在此期间，大脑结构趋于稳定，与智力和个性的稳定期相对应，并且分隔化程度增加。诸如为人父母等人生事件可能会影响这个转折点附近的变化。

最后两个阶段是**早期衰老（66岁至83岁）**和**晚期衰老（83岁以后）**，两者都以大脑连接性下降为特征，据信这与衰老和白质退化有关。

了解这些独特的大脑时期及其转折点，有助于深入了解大脑连接何时以及如何容易受到干扰，并有助于解释青少年期常见的精神健康障碍的出现。

---

## 22. HN 作品：KiDoom — 在 PCB 走线上运行 DOOM

**原文标题**: Show HN: KiDoom – Running DOOM on PCB Traces

**原文链接**: [https://www.mikeayles.com/#kidoom](https://www.mikeayles.com/#kidoom)

这篇题为《Show HN: KiDoom – 在PCB走线上运行DOOM》的文章介绍了一个创新项目，据称经典视频游戏DOOM直接在印刷电路板（PCB）的导电走线上运行。这表明这是一种高度技术性和创造性的硬件创新，正在突破PCB设计和嵌入式系统通常所能实现的界限。

然而，随附内容并未提供关于KiDoom项目本身的具体细节、其方法论或所面临的挑战。相反，它列出了一般性的专业指标和项目类别，包括：“开发了3个ECU”、“10年以上经验”和“行驶里程超过2850万英里”。它还提到了“精选项目”和“私人工具”。这些内容似乎是个人或团队总体资质和作品集的一份高层级总结，而非对KiDoom技术成就的详细阐述。

因此，尽管标题预示着一场引人入胜的硬件创新展示，所提供的文本却给出了与在PCB走线上运行DOOM的机制或成功与否无关的背景专业数据。

---

## 23. 最稳定的树莓派？散热管理助NTP更准。

**原文标题**: Most Stable Raspberry Pi? Better NTP with Thermal Management

**原文链接**: [https://austinsnerdythings.com/2025/11/24/worlds-most-stable-raspberry-pi-81-better-ntp-with-thermal-management/](https://austinsnerdythings.com/2025/11/24/worlds-most-stable-raspberry-pi-81-better-ntp-with-thermal-management/)

文章详细介绍了一种先进方法，旨在提高基于树莓派的NTP服务器的稳定性，解决由CPU温度波动引起的频率漂移问题。尽管使用了稳定的GPS PPS参考，作者仍观察到系统时钟频率变化与全天CPU温度变化相关。关键在于，靠近CPU且受温度影响的底层晶体振荡器直接受到这些热变化的影响。

该解决方案被命名为“Austin's Nerdy Things”，包含两个主要部分，使频率可变性降低了81%，频率标准差降低了77%：

1.  **CPU核心绑定和实时优先级：** CPU 0专门用于关键计时任务（`chronyd`和PPS中断）。一个启动脚本确保所有CPU以最大频率运行（性能调控器），将PPS中断和`chronyd`绑定到CPU 0，并将`chronyd`设置为实时优先级。这隔离并优先处理了时间敏感的操作。

2.  **PID控制的热稳定性：** 一个基于Python的“时间燃烧器”脚本利用PID控制器来维持恒定的CPU温度（例如54°C）。这是通过在CPU 1-3上（避开CPU 0）运行工作进程实现的，这些工作进程根据PID输出进行忙循环（MD5哈希计算）或休眠。通过主动控制CPU温度，晶体振荡器的热环境得以稳定，从而保持其频率一致。

这种组合将均方根偏移均值显著降低了49%（从85.44纳秒降至43.54纳秒），表明尽管环境温度波动，时间精度仍显著提高。文章提供了使用shell脚本和systemd服务实现这些优化的分步说明。

---

## 24. 使用 CSS 子网格的新布局

**原文标题**: New layouts with CSS Subgrid

**原文链接**: [https://www.joshwcomeau.com/css/subgrid/](https://www.joshwcomeau.com/css/subgrid/)

CSS 子网格是 CSS Grid 的强大扩展，它允许网格布局更深入地渗透到 DOM 树中，解决了只有直接子元素才能参与网格的局限性。它最初被认为是语义化标记的便利工具，但事实证明能开启新的布局可能性。

文章首先通过演示子网格如何解决在 `<ul>` 标签中语义化分组图片的问题来阐释其基本机制，否则这种分组会破坏扁平的网格布局。通过对 `<ul>` 应用 `display: grid`、`grid-row: span 2`、`grid-column: span 3`，以及关键的 `grid-template-rows: subgrid; grid-template-columns: subgrid;`，其 `<li>` 子元素便能与父网格对齐。虽然简单情况可能通过嵌套的 Flexbox/Grid 解决，但子网格在更复杂的场景中大放异彩。

文章提出了一个更引人注目的用例：一个由文章卡片组成的网格，每张卡片包含图片和文本。没有子网格时，每个 `<article>` 都定义自己的内部两列网格（例如 `2fr 1fr`）。这导致兄弟卡片之间列宽不一致，因为每张卡片的 `fr` 单位计算仅基于其自身内容，从而使得整体网格中图片和文本列错位。强制使用固定百分比的列可能导致内容溢出。

子网格提供了一个优雅的解决方案：父级 `.grid` 定义了整个轨道结构（例如，对于两列布局，`grid-template-columns: repeat(2, 2fr 1fr)`，其中每个“列”块都是 `2fr 1fr`）。然后，每个子级 `<article>` 被指示跨越这两个轨道（`grid-column: span 2`），并使用 `display: grid; grid-template-columns: subgrid;` 来继承父级定义的列结构。这确保了所有卡片中的所有图片和文本内容完美对齐，因为它们都引用了 *相同* 的底层网格轨道定义。子网格从而实现了以前用 CSS 难以实现的复杂、协调的布局。

---

## 25. 统一 1.0

**原文标题**: Unison 1.0

**原文链接**: [https://www.unison-lang.org/unison-1-0/](https://www.unison-lang.org/unison-1-0/)

Unison 1.0 标志着其独特的“内容寻址”编程语言、分布式运行时和开发者工作流的稳定版发布。Unison 的核心创新在于通过定义内容的实际信息来识别定义，并将代码存储在数据库中而非文本文件。这种设计从根本上解决了许多版本冲突，优化了编译，并使得在一个单一的强类型程序中构建复杂的、自部署的分布式系统成为可能。

Unison 1.0 的主要特性包括：
*   **协作工具：** 精简的工作流和不断发展的生态系统，由 Unison Share（一个用于代码浏览和贡献的开源社区中心）提供支持。
*   **Unison 云：** 一个用于部署 Unison 应用程序的平台，完全通过代码定义应用程序和基础设施。它还支持“自带云”（BYOC），用于在自定义容器基础设施上部署。
*   **优化开发者体验（DX）：** 工具方面的改进，包括 Unison Codebase Manager (ucm) 命令行界面和 UCM 桌面图形用户界面。
*   **运行时优化：** 解释器速度和效率的显著提升。
*   **分布式系统框架：** 可伸缩、容错应用程序的构建模块，例如 Volturno 流处理库。

迈向 1.0 的历程包含了重要里程碑，包括公司成立（2018年）、首次 Alpha 版本发布（2019年）、采用 SQLite（2021年）、Unison Share 推出、LSP 支持（2022年）、Unison Cloud 全面上市（2024年）、Share 开源（2024年）以及 BYOC 功能（2025年）。该项目展现出强劲的发展势头，拥有超过 26,000 次提交和 150,000 多个已发布的定义。

未来计划包括 C FFI 支持、改进的记录类型、云可观测性以及一个智能代理计算框架。Unison 提供原生版本控制系统，旨在提供独特且高度集成的开发体验。

---

## 26. APT Rust要求引发疑问

**原文标题**: APT Rust requirement raises questions

**原文链接**: [https://lwn.net/SubscriberLink/1046841/5bbf1fc049a18947/](https://lwn.net/SubscriberLink/1046841/5bbf1fc049a18947/)

Debian APT 维护者朱利安·安德烈斯·克洛德宣布，Debian 的高级软件包工具 (APT) 将不迟于 2026 年 5 月要求使用 Rust。这一旨在实现现代化、内存安全和更强单元测试的决定，在项目中引发了重大质疑。

这一新依赖将主要影响 Alpha、Motorola 680x0、PA-RISC 和 SuperH 等非官方 Debian 移植版本，这些版本目前缺乏可用的 Rust 工具链。这些移植版本将要么需要获得 Rust 支持，要么保留旧版 APT。

包括约翰·保罗·阿德里安·格劳比茨在内的批评者认为，克洛德的沟通方式具有对抗性。APT 的同事贡献者大卫·卡尔尼什基斯质疑 Rust 对于单元测试的必要性，他提出了替代方法，甚至建议从 APT 中完全移除部分解析代码。阿德里安·邦克和法比安·格伦比希勒强调了 Debian 现有基础设施对于静态链接软件包（例如用 Rust 编写的软件包）存在的问题，这导致了有限的安全支持，并难以追踪依赖项和 CVE。

一些人认为，由于一位开发者正在主导一项具有广泛影响的变革，此举与 Debian 支持广泛硬件、民主治理和依赖志愿者贡献等核心价值观相矛盾。尽管文章承认 Rust 在自由软件中日益普及，但它强调需要更多志愿者来改进 Rust 在 Debian 中的支持，而不是由单方面指令给他人制造计划外的工作。

---

## 27. 罗布乐思是个问题，但它只是更糟糕问题的一个症状。

**原文标题**: Roblox is a problem but it's a symptom of something worse

**原文链接**: [https://www.platformer.news/roblox-ceo-interview-backlash-analysis/](https://www.platformer.news/roblox-ceo-interview-backlash-analysis/)

文章批判了科技公司CEO对儿童安全和用户伤害的轻蔑态度，以Roblox首席执行官David Baszucki最近的采访为例。尽管该平台的用户年龄低至五岁，Baszucki在被问及Roblox历史上的安全失误时表现出沮丧。历史上，Roblox缺乏有效的年龄验证，并且允许轻易规避安全功能，导致了多起儿童掠夺事件和诉讼。作者认为，Roblox和许多科技公司一样，将增长置于实施关键安全防护措施之上。

这种模式并非孤立，还包括OpenAI将用户参与度置于安全之上，TikTok的“数字健康”功能反而鼓励更多应用使用，以及Meta据称为了增长而拖延儿童掠夺者预防工作。Meta内部文件显示，员工将他们的策略比作烟草公司“从小培养成瘾用户”，并故意淡化成瘾研究结果。

作者总结道，这种“拖延、否认和转移”的策略之所以有效，是由于公众注意力持续时间短以及企业责任感的下降。尽管过去的公众压力曾带来一些改进，但如今的科技领袖似乎反应迟钝，将未来愿景置于当前用户福祉之上。Baszucki的采访突出一个普遍存在的问题：科技高管中普遍存在的轻蔑心态。

文章还简要指出，特朗普政府因两党强烈反对而撤回了一项旨在先发制人州级AI法规的行政命令；以及X平台新的“关于此账户”功能无意中揭示许多有影响力的右翼政治账户设在国外，重新引发了对虚假在线活动的担忧。

---

## 28. 制作古惑狼 (2011)

**原文标题**: Making Crash Bandicoot (2011)

**原文链接**: [https://all-things-andy-gavin.com/video-games/making-crash/](https://all-things-andy-gavin.com/video-games/making-crash/)

这篇节选《古惑狼的制作——第一部分》发表于2011年2月2日，介绍了该游戏创作的早期历史。作者回顾了顽皮狗公司在1994年夏天时的状况。那时，公司仅由作者和Jason Rubin两人运营。在此前八年里，他们已共同发行了六款游戏，并意识到是时候将团队从两人精简的模式扩展开来了。

---

## 29. 新桥连接无穷数学与计算机科学

**原文标题**: A new bridge links the math of infinity to computer science

**原文链接**: [https://www.quantamagazine.org/a-new-bridge-links-the-strange-math-of-infinity-to-computer-science-20251121/](https://www.quantamagazine.org/a-new-bridge-links-the-strange-math-of-infinity-to-computer-science-20251121/)

数学家安东·伯恩施泰因在探索集合无限性质的描述集理论与专注于有限网络和算法的现代计算机科学之间，发现了一个深刻而令人惊讶的联系。他证明了某些无限集相关的问题可以被重新表述为计算机网络进行通信和解决任务的挑战。鉴于这两个领域传统上使用的语言和尺度（无限与有限）截然不同，这座桥梁显得尤为卓越。

描述集理论家根据无限集的“可测性”（例如长度或面积）对其进行分类，并将其排列成一个层次结构。他们通常避免使用“选择公理”，因为它的使用可能导致“不可测”或“病态”的集合。例如，可测地为某个特定的无限图着色可能需要三种颜色，而使用选择公理时，两色解将涉及不可测集合。

与此同时，计算机科学家研究“分布式算法”，即网络中的多台计算机协同解决问题，例如分配通信信道（一个着色问题）以避免干扰。这些“局部算法”依赖于节点只与其直接邻居通信，旨在提高效率。

伯恩施泰因观察到，着色问题的“阈值”（即某些属性所需的颜色数量）在这两个领域中惊人地相似。他提出，计算机科学中的高效局部算法直接对应于描述集理论中无限图的勒贝格可测着色。这一开创性的见解意味着，这些看似截然不同的领域中的问题其基本结构是相同的，只是以不同的数学语言表达，为新的发现和合作铺平了道路。

---

## 30. 台积电亚利桑那厂停电致晶圆厂停产，苹果晶圆报废。

**原文标题**: TSMC Arizona outage saw fab halt, Apple wafers scrapped

**原文链接**: [https://www.culpium.com/p/tsmc-arizona-outage-saw-fab-halt](https://www.culpium.com/p/tsmc-arizona-outage-saw-fab-halt)

一份独家报道揭示，九月中旬，工业气体设施林德（Linde）的一次停电导致台积电亚利桑那州21厂（Fab 21）遭遇严重生产中断。台积电外包气体供应商林德的一次电力故障中断了关键原料供应，迫使该晶圆厂停产数小时，并导致数千片原定用于苹果、英伟达和AMD等客户的晶圆报废。

这一此前未被报道的事件，为台积电亚利桑那州工厂第三季度净收入锐减99%提供了另一种解释，此前人们普遍将此唯一归因于运营成本上升。台积电证实其亚利桑那州部门对营收有积极贡献，但指出利润受到多种因素影响，包括未来五年海外晶圆厂投产导致的毛利率稀释预期。该公司拒绝直接回应此次中断事件。

晶圆厂停产对台积电来说是罕见的，其昂贵的设备24/7不间断运行，因此即使短暂的闲置也会造成巨大损失。尽管预计对客户的影响微乎其微，且鉴于该晶圆厂产能仍小，财务损失可能由保险公司承担，但此次事件突显了台湾制造商在海外设施的关键运营中依赖非台湾公司时所面临的挑战。此事件是亚利桑那州晶圆厂建设过程中更广泛的“跨文化适应”的一部分。

---

## 31. 重塑 .NET 构建与发布的方式 (再次)

**原文标题**: Reinventing how .NET builds and ships (again)

**原文链接**: [https://devblogs.microsoft.com/dotnet/reinventing-how-dotnet-builds-and-ships-again/](https://devblogs.microsoft.com/dotnet/reinventing-how-dotnet-builds-and-ships-again/)

.NET 团队正在再次彻底改革其构建和发布流程，因为先前的分布式存储库模型虽然适用于一般的开源项目，但对于快速交付一个内聚的产品而言，被证明效率低下且不可持续。该系统面临的挑战包括多版本的高昂成本、关键修复的缓慢（例如，36 小时以上的构建时间）、日益增长的基础设施维护负担以及跨栈功能原型开发的困难。

这种低效源于两个核心问题：“产品构建复杂性”（相互依赖的存储库之间步骤过多、协调点繁杂以及环境差异大）和“产品构建开销”（大量时间花费在非产物生成活动上，例如依赖流转、PR 审查和构建排队）。例如，一个安全补丁需要跨越众多团队和存储库进行复杂、顺序的协调，以在同步发布前实现“一致性”。内部分析显示了惊人的开销，其中一个 8.0 运行时构建显示其总时间的 38.5% 是非生产性开销。

为解决这些问题，“统一构建项目”正在将产品构建转移到一个“虚拟单体”存储库中，将构建整合为“垂直构建”，并利用“Linux 发行版源构建”。这旨在大幅降低复杂性和开销，提高可预测性和速度，同时保留外部贡献能力。

---

## 32. 十五年

**原文标题**: Fifteen Years

**原文链接**: [https://xkcd.com/3172/](https://xkcd.com/3172/)

此内容来自xkcd.com网页，其中包含题为“十五年”的漫画。xkcd自称是“一部关于浪漫、讽刺、数学和语言的网络漫画。”

一个显眼的部分宣传《WHAT IF？》的“十周年特别版”——一本经过修订和注释的书，包含全新插图并解答重要问题，可供订购。

该页面提供标准的网络漫画导航（上一篇、下一篇、随机），以及漫画及其图片的永久链接。它还列出了创作者喜欢的其他网络漫画，并链接到“其他内容”，例如技术提示和气候常见问题。

一则幽默的提示提供了不合时宜的最佳观看建议，建议在模拟的Apple IIGS上使用Netscape Navigator 4.0，屏幕分辨率为1024x1，并附带具体说明，例如启用广告拦截器和设置“船模式”。

最后，该作品根据知识共享署名-非商业性使用2.5许可协议授权，允许非商业性复制和分享。

---

## 33. DoGE“割肉割到骨头”；残酷裁员后，2.6万专家获返聘

**原文标题**: DoGE "cut muscle, not fat"; 26K experts rehired after brutal cuts

**原文链接**: [https://arstechnica.com/tech-policy/2025/11/doge-doesnt-exist-anymore-but-expert-says-its-still-not-dead/](https://arstechnica.com/tech-policy/2025/11/doge-doesnt-exist-anymore-but-expert-says-its-still-not-dead/)

由埃隆·马斯克牵头、旨在大幅削减政府开支和官僚机构的备受争议的机构——政府效率部（DOGE），已提前八个月终止。DOGE最初被吹捧可节省一万亿美元，但据报道实际节省的资金远少于此（2140亿美元，可能被夸大），并因非法解雇面临多起诉讼。

布鲁金斯学会的伊莱恩·卡马克表示，DOGE“削的是肌肉，而不是脂肪”，表明其对关键政府职能缺乏了解。她的报告记录了26,511起特朗普政府突然解雇联邦雇员后又重新雇佣的案例。这些被重新雇佣的人员往往是工程师和医生等关键专业人士，其中许多是法院强制要求或默许承认基本任务受到威胁。

DOGE的混乱做法导致了严重的“人才流失”，特朗普任期前六个月内有15.4万名联邦雇员寻求延迟辞职，7万名雇员退休。尽管招聘冻结已解除，但重新招聘进展缓慢且似乎存在偏见。

尽管DOGE作为一个集中实体已经消失，但其职能已被人事管理办公室（OPM）和管理与预算办公室（OMB）吸收，这表明“分散化”的削减工作将继续进行。卡马克警告说，如果流失的人才得不到补充，将导致严重后果，包括核管理不善、灾害响应不足、联邦调查局（FBI）失职以及公共卫生和社会服务受到损害。各机构现在正争相评估和减轻损失，但政府能否迅速恢复仍不确定。

---

## 34. 谷歌的新“Aluminium OS”项目将Android引入PC

**原文标题**: Google's new 'Aluminium OS' project brings Android to PC

**原文链接**: [https://www.androidauthority.com/aluminium-os-android-for-pcs-3619092/](https://www.androidauthority.com/aluminium-os-android-for-pcs-3619092/)

谷歌正在开发一款代号为“Aluminium OS”的新操作系统，旨在将ChromeOS和Android融合为适用于PC的单一统一桌面平台。这一举措旨在将Android的影响力扩展到移动设备之外，更好地与Windows、macOS和iPad竞争，并优化开发资源。

Aluminium OS已被确认为一个基于Android的系统，其核心将集成谷歌的AI技术栈，包括Gemini。招聘信息揭示了该操作系统雄心勃勃的计划，即支持笔记本电脑、可拆卸设备、平板电脑和迷你PC等多种外形，涵盖“AL大众高端”和“AL高端”等多个价位，打消了它将仅限于低成本设备的担忧。

尽管Aluminium OS最初将与ChromeOS共存，但谷歌打算最终完全取代ChromeOS。这一过渡将得到精心管理，为旧款ChromeOS设备提供传统支持，并为现有具备能力的Chromebook提供潜在的可选迁移路径。最终品牌名称尚未确定，备选方案包括保留“ChromeOS”名称或采用“Android Desktop”。

谷歌已确认将于2026年推出，目前正在Android 16上进行开发测试。初次公开发布预计将基于Android 17。谷歌正在与高通合作开展此项目，旨在融合移动和桌面计算。

---

## 35. 一个极简到挑战生命定义的细胞

**原文标题**: A cell so minimal that it challenges definitions of life

**原文链接**: [https://www.quantamagazine.org/a-cell-so-minimal-that-it-challenges-definitions-of-life-20251124/](https://www.quantamagazine.org/a-cell-so-minimal-that-it-challenges-definitions-of-life-20251124/)

由Takuro Nakayama领导的科学家们发现了一种新的单细胞古菌，*Candidatus Sukunaarchaeum mirabile*，其基因组异常小，仅有238,000个碱基对。这种微生物独一无二，因为它几乎缺乏所有代谢基因，完全依赖宿主细胞进行营养加工和生长。这种极端的基因组简化挑战了生命的基本生物学定义，传统上，这些定义包括代谢自给自足。

*Sukunaarchaeum* 仅保留了自身复制所需的遗传成分，代表了一种极简形式的细胞生命。与其他基因组缩减但可能向宿主提供营养的共生微生物不同，*Sukunaarchaeum* 似乎是一种自我中心的寄生生物。尽管它高度依赖宿主，但它通过拥有自己的基因表达核心机制（包括核糖体）而与病毒不同。

这一发现揭示了一个隐藏的寄生微生物多样性世界，特别是在*Sukunaarchaeum* 所属的DPANN古菌中。它真正的宿主以及其大部分新颖基因的功能仍然未知，尽管推测这些基因可能介导宿主相互作用。研究人员认为，许多类似、超微型生物可能存在，但常常被传统的基因测序方法所忽视，这暗示着一个巨大的微生物生命“冰山”，它正在拓宽对生命实体构成的认知界限。

---

## 36. CS234：强化学习 2025年冬季

**原文标题**: CS234: Reinforcement Learning Winter 2025

**原文链接**: [https://web.stanford.edu/class/cs234/](https://web.stanford.edu/class/cs234/)

CS234：强化学习，2025年冬季学期，由Emma Brunskill教授（Chethan Bhateja担任首席助教），旨在向学生介绍用于自主系统的强化学习，内容涵盖核心挑战、泛化、探索以及深度强化学习。

先决条件包括熟练掌握Python，大学微积分/线性代数，基础概率论/统计学，以及机器学习基础（CS 221/229）。学习成果侧重于定义和公式化强化学习问题，实现常用算法，并评估其性能，包括探索与利用的挑战。

讲座时间为太平洋标准时间周二和周四下午1:30-2:50，并提供Canvas上的视频。沟通通过Ed讨论区进行，以获得最快的回复。作业和成绩通过Gradescope管理。

课程成绩包括三次作业（46%），一次期中考试（25%），一次小测验（5%），以及一个课程项目（24%，包含项目提案、里程碑、海报展示和论文），外加讲座投票参与的0.5%额外加分。学生总共有5天宽限期（每个作业/项目组件最多2天，海报/最终论文无宽限期）。

学术诚信至关重要：学生可以讨论想法，但必须独立完成解决方案。允许使用GPT-4等生成式AI工具进行构思（如同人类协作），但禁止直接用于解决方案或代码复制，且必须注明其使用。AI工具不能列为项目合作者。推荐教材是Sutton和Barto的《强化学习：导论》（第二版，免费在线获取）。

---

## 37. 统一移动端和桌面端

**原文标题**: Unifying our mobile and desktop domains

**原文链接**: [https://techblog.wikimedia.org/2025/11/21/unifying-mobile-and-desktop-domains/](https://techblog.wikimedia.org/2025/11/21/unifying-mobile-and-desktop-domains/)

维基媒体基金会已成功统一其移动端和桌面端域名，从独立的`m.wikipedia.org`网址过渡到单一标准域名，如`en.wikipedia.org`。这项于十月完成的变更，消除了自2011年起针对移动用户存在的长期重定向。

曾一度常见的独立移动域名已过时。谷歌转向“移动优先”的抓取方式，意味着它不再支持广告独立的移动网址。这一变化导致谷歌引荐流量的移动响应时间下降10-20%，因为用户被迫等待重定向。

统一域名带来了显著的好处：
1.  **移动响应时间加快20%**：消除重定向直接提升了所有用户的移动页面加载速度，包括恢复了谷歌引荐流量所经历的下降。例如，波斯语维基百科的响应时间缩短了0.25秒。
2.  **改善了搜索引擎优化（SEO）**：维基共享资源面临着严重的SEO问题，数百万页面被取消索引，且只有一半被谷歌知晓，原因是重定向造成了抓取循环。禁用维基共享资源上的Googlebot重定向，使得谷歌引荐的页面浏览量增加了100%。此外，启用站点地图帮助谷歌索引了7000万个新的维基共享资源页面，且视频识别能力得到提升。
3.  **更好的链接分享用户体验（UX）**：移动设备分享的链接以前硬编码了移动域名。现在，旧的移动链接会自动重定向到标准域名，确保无论接收者使用何种设备，始终显示适当的站点版本。
4.  **降低了基础设施负载**：独立的域名导致每次编辑都会产生重复的缓存清除。统一这些域名将MediaWiki的清除率降低了50%，每天清除量减少了约40亿次，整体CDN清除量减少了20-40%。

这一战略性统一使维基百科的基础设施现代化，提升了用户体验、搜索引擎可见性和运营效率。

---

## 38. 读心设备现已能够预测前意识思想。

**原文标题**: Mind-reading devices can now predict preconscious thoughts

**原文链接**: [https://www.nature.com/articles/d41586-025-03714-0](https://www.nature.com/articles/d41586-025-03714-0)

读心设备，即脑机接口（BCI），正在迅速发展，以预测前意识思维。早期的植入式脑机接口，例如南希·史密斯曾用它弹奏钢琴，能将想象中的动作转化为实际行动，有时甚至在意识形成前数百毫秒就能检测到意图。这类设备最初主要关注运动皮层，以帮助瘫痪患者控制辅助技术，而新型的“双植入”脑机接口还能进入诸如顶叶后皮层等区域，解码与推理、注意力、规划相关的更复杂信号，包括内心独白。

与此同时，利用人工智能增强的脑电图（EEG）技术的可穿戴消费级神经技术也在不断改进。尽管不如植入设备精确，这些设备能揭示整体大脑状态，例如警觉性或焦虑，而苹果等科技巨头正在探索将其整合。

这种快速发展引发了重大的伦理担忧。临床脑机接口受医疗法规约束，而消费级神经技术领域则基本不受监管，允许公司对用户数据拥有广泛的控制权。伦理学家担忧隐私侵犯、推断出的个人数据（例如心理健康、政治立场）的出售，以及对“认知自由”的影响，形容其为“给现有数据经济注入类固醇”。

各国政府和国际机构正开始引入法律和指导方针，以保护神经数据。脑机接口的未来旨在更深入地探究潜意识思维的前兆，并通过监测神经信号和提供靶向刺激，可能诊断和治疗精神疾病，这凸显了建立健全的安全和伦理框架的迫切需求。

---

## 39. 中国精英质疑AI

**原文标题**: PRC elites voice AI-skepticism

**原文链接**: [https://jamestown.org/prc-elites-voice-ai-skepticism/](https://jamestown.org/prc-elites-voice-ai-skepticism/)

詹姆斯敦基金会的文章《中国精英对人工智能持怀疑态度》指出，中国影响力人物中对于人工智能的变革力量和潜在风险，日益弥漫着谨慎和疑虑。尽管普遍认为中国在积极寻求人工智能主导地位，但该文章揭示，许多中国共产党（CCP）和军民融合体系内人士表达了严重的保留意见，其担忧从技术局限性延伸至深远的社会和政治影响。

这些精英，包括学者、战略家和政府顾问，表示人工智能的能力常常被过分夸大，其发展面临严峻的技术障碍，尤其是在道德困境、偏见和控制方面。他们质疑人工智能是否能真正复制人类的创造力或判断力，担心过度依赖人工智能可能导致战略失误或侵蚀人类主体性。此外，人们还担心人工智能如果管理不当，可能加剧社会不平等、破坏就业稳定，甚至构成生存威胁。这种怀疑论与公开宣称的AI乐观主义形成鲜明对比，并表明在中国决策圈内部，对于人工智能的未来发展轨迹和应用，存在着一种更为细致、谨慎的态度。

---

## 40. 维护开源项目不为人知的真相

**原文标题**: What they don't tell you about maintaining an open source project

**原文链接**: [https://andrej.sh/blog/maintaining-open-source-project/](https://andrej.sh/blog/maintaining-open-source-project/)

Andrej的文章《他们没有告诉你的开源项目维护真相》揭示了维护一个成功开源项目背后严苛的现实，这往往与最初的理想化预期形成鲜明对比。最初作为一项充满激情的项目或个人作品集构建器，它很快演变成一份无偿的“第二份工作”，耗费大量时间和情感精力。

维护者们肩负着一系列任务，从修复错误和审查拉取请求到撰写文档和提供用户支持。用户通常不知道维护者的个人限制或其工作的无偿性，对及时响应和持续更新抱有很高的期望，这导致了巨大的压力。这种持续不断的需求，加上微薄的经济回报和偶尔的负面反馈，经常导致压力、沮丧和倦怠。

作者将这种困境描述为“金手铐”；项目变得过于成功而无法放弃，这源于维护者对用户的责任感，即使他们不再享受这份工作。

最终，维护者必须面对艰难的选择：找到项目盈利的方法，尝试将其移交给社区领导，或者有意缩减参与程度，但这会冒着用户不满的风险。文章建议有抱负的开源创作者在投入一个可能获得巨大关注的项目之前，仔细考虑成功可能带来的负担，并提前规划好可持续性或优雅的退出策略。

---

## 41. Python 统计过程控制

**原文标题**: Statistical Process Control in Python

**原文链接**: [https://timothyfraser.com/sigma/statistical-process-control-in-python.html](https://timothyfraser.com/sigma/statistical-process-control-in-python.html)

本文提供了Python中统计过程控制（SPC）的实用指南，重点在于衡量产品质量波动并确定何时需要进行过程干预。它利用`pandas`进行数据操作，`plotnine`进行可视化，以及`scipy`进行统计功能。

该研讨会使用日本温泉（onsen）的案例研究来演示质量控制，特别是针对温度、pH值和硫含量，这些对市场定位至关重要。加载样本温度数据后，过程从计算描述性统计数据（均值、标准差）开始。

引入了关键的SPC可视化，首先是一个过程概览图，它结合了抖动图和箱线图，以显示随时间变化的单个测量值和子组分布，同时还包含一个用于整体过程波动的直方图。

为了进行更深入的分析，计算了子组统计数据，包括均值（`xbar`）、极差（`r`）、标准差（`sd`）和合并的子组内标准差（`sigma_s`）。这些值用于确定X-bar图的控制限，X-bar图通过绘制随时间变化的子组均值与中心线（总均值）和3-sigma控制限，以监控过程稳定性。一个自定义的`ggprocess`函数简化了图表的生成。

本文还涵盖了针对单个测量值（n=1）情况的移动极差图，演示了连续测量值之间的绝对差如何帮助估计和监控过程波动。

总之，本指南为用户提供了在Python中生成SPC可视化和统计数据的工具和理解，从而能够做出数据驱动的决策，以改进和控制过程。

---

## 42. 移民局向追踪移民的“赏金猎人”公司提供高达2.8亿美元资金

**原文标题**: ICE Offers Up to $280M to Immigrant-Tracking 'Bounty Hunter' Firms

**原文链接**: [https://www.wired.com/story/ice-bounty-hunter-spy-program/](https://www.wired.com/story/ice-bounty-hunter-spy-program/)

移民与海关执法局（ICE）正大幅扩大其将移民追踪外包给私人监控公司的计划，超越了此前1.8亿美元的试点项目。经WIRED审阅的新合同记录显示，ICE已取消了这项计划的总支出上限，将单个供应商的限额提高到2.8125亿美元，并保证每家承包商的初始任务订单至少为750万美元。

这一转变表明，ICE现在将其视为一项重大投资而非一项实验，期望主承包商充当联邦执法部门的实际延伸。这些被描述为“赏金猎人”的私人公司，将确认被指定驱逐人员的住址和工作地址。他们的方法将包括拍摄住宅、记录行动、监视工作场所，以及利用商业数据中介和开源研究。

该计划的范围巨大，承包商预计每月将处理一份150万人案件清单中的5万个案件。付款将基于绩效，按案件固定价格支付，并根据速度和准确性提供额外奖金。尽管承包商无法直接访问ICE的内部系统，但他们将收到导出的案件数据包，其中包含大量敏感个人数据，并在公共监督之外运作。

这项举措是特朗普政府一系列努力中的最新一项，旨在扩大承包商在ICE执法行动中的作用，此前已推出私人运输网络、社交媒体目标识别中心和全国呼叫中心等计划。增加的财政担保被认为是必要的，以确保承包商能够调集ICE所需的大量劳动力和基础设施。

---

## 43. 不良用户体验世界杯 2025

**原文标题**: Bad UX World Cup 2025

**原文链接**: [https://badux.lol/](https://badux.lol/)

由Nordcraft主办的“2025年糟糕用户体验世界杯”近日落幕，最终Dalia凭借作品“完美日期选择器”夺得冠军。

比赛要求参赛者构建一个故意设计成糟糕用户体验的日期选择器——越差越好——同时要确保在技术上仍然可以选择所需的日期。参赛作品可以使用任何网络技术，并必须通过公开可访问的URL提供。

获胜者的奖品包括一个“烂奖杯”（shittrophy）和一份Kevin Powell的“CSS揭秘”课程。评审团由David Prentell、Cassidy Williams以及Kevin Powell本人组成。

人们对这项活动的反应不一，从Reddit用户称其“愚蠢且不专业”，到Anders R. Møller认为其“令人厌恶却又引人入胜”，甚至ChatGPT也评价其“才华横溢且具有文化共鸣”。该活动吸引了来自不同国家的开发者提交大量作品，展现了人们对糟糕设计理念的广泛而幽默的参与。

---

## 44. 大语言模型扩展的惨痛教训

**原文标题**: The Bitter Lesson of LLM Extensions

**原文链接**: [https://www.sawyerhood.com/blog/llm-extension](https://www.sawyerhood.com/blog/llm-extension)

这篇文章记录了大型语言模型（LLM）扩展功能三年的演变，并强调了一个学到的“惨痛教训”。它始于2023年3月雄心勃勃的ChatGPT插件，旨在通过OpenAPI实现通用工具使用，但因模型尚不成熟和用户体验不佳而告失败，尽管其代码解释器预示了未来的潜力。2023年7月的自定义指令（Custom Instructions）和2023年11月的自定义GPTs（Custom GPTs）等更简单的方法则侧重于提示工程，而2024年2月的记忆功能（Memory）引入了自动个性化。

2024年4月的Cursor规则（Cursor Rules）将自定义指令直接集成到代码仓库（`.cursorrules`文件），使扩展功能变得更加原生。到2024年末，模型上下文协议（Model Context Protocol, MCP）作为一种重量级的客户端-服务器解决方案出现，用于实现强大的工具集成，但其强大也伴随着复杂。

关键转折点是2025年10月的智能体技能（Agent Skills），这是插件功能的简化版重生。技能由目录中的Markdown文件和脚本组成，智能体只在相关时才对其进行索引和读取。至关重要的是，智能体技能的运行前提是智能体拥有通用的计算机访问权限（例如Bash），能够*编写和执行自己的工具和脚本*。

这便是“惨痛教训”的体现：赋予智能体通用工具，并信任其智能来完成“粘合工作”并即时创建专业解决方案，这远优于预先定义每一个具体工具。作者预测，未来的LLM应用将普遍集成一个抽象的“计算机”，使自然语言成为最易用的扩展机制，并有效地取代MCP等复杂协议。

---

## 45. 我私信了一位韩国总统候选人，结果为他打造了核心竞选班底。

**原文标题**: I DM'd a Korean presidential candidate and ended up building his core campaign

**原文链接**: [https://medium.com/@wjsdj2008/i-dmd-a-korean-presidential-candidate-and-ended-up-building-his-core-campaign-platform-the-38eb1c5f5e7d](https://medium.com/@wjsdj2008/i-dmd-a-korean-presidential-candidate-and-ended-up-building-his-core-campaign-platform-the-38eb1c5f5e7d)

软件工程师杰克·李（Jake Lee）详细讲述了他为当时的总统候选人（现任韩国总统）尹锡悦搭建核心竞选平台的意外历程。2021年，他对现有政治应用程序的不足感到沮丧，于是直接在Facebook上向尹锡悦发消息，主动提出要创建一个更优秀的数字沟通渠道。

尹锡悦的竞选活动饱受数字基础设施老旧、缺乏与支持者直接互动之苦。李的主动联络很快获得批准，着手构建解决方案。在一周内，他召集了一支由工程师和设计师组成的志愿者团队，启动了一个直接沟通平台。这个系统使公民能够提交政策建议、参加志愿活动、捐款以及参与讨论，有效地绕过了传统政党结构，促进了草根参与。

这个迅速开发的平台对尹锡悦的竞选活动至关重要，促进了大量的公众参与、政策建言和志愿者协调。李的这一举措展示了拥有技术技能的个人对一场重大政治竞选活动所能产生的深远影响，展现了现代数字工具以及直接、技术驱动的互动在动员支持者和为尹锡悦最终的选举成功做出贡献方面的力量。

---

## 46. 太空货运 · 诺斯特罗莫 (2012)

**原文标题**: Space Truckin' – The Nostromo (2012)

**原文链接**: [https://alienseries.wordpress.com/2012/10/23/space-truckin-the-nostromo/](https://alienseries.wordpress.com/2012/10/23/space-truckin-the-nostromo/)

文章《太空货运——诺斯特罗莫号》探讨了雷德利·斯科特1979年电影《异形》中“诺斯特罗莫号”宇宙飞船错综复杂且充满挑战的设计过程。导演雷德利·斯科特追求一种“旧宇宙”美学，这受到了《2001：太空漫游》的现实主义以及约翰·卡朋特电影《黑星》中描绘的粗粝、破败生活的影响。这种做法刻意与《星球大战》中更干净、更奇幻的设定形成对比，强调了功能性以及“卡车司机版”的太空旅行。

编剧丹·欧班农在推动这种充满生活气息的工业感外观方面发挥了关键作用，他在制作初期便委托艺术家罗恩·科布和克里斯·福斯进行设计。科布（他也是异形腐蚀性血液的构思者）为这艘飞船（最初名为“斯纳克号”）制作了大量早期设计。福斯（以其充满活力的宇宙飞船绘画而闻名）也贡献了丰富的外部设计概念。

尽管经过数月的工作并将名字改为“诺斯特罗莫号”，但最终设计却迟迟未能确定。斯科特一旦投入其中，便对一艘“缓慢移动的巨型钢铁块”有了清晰的构想。最终，在压力之下，特效总监布莱恩·约翰逊选择了罗恩·科布的“诺斯特罗莫A”草图作为模型的基础，斯科特随后将其从黄色重新漆成灰色。尽管科布的内部设计大体被接受，但斯科特坚定的方向往往意味着福斯等艺术家早先大量的工作被搁置一旁，这在创作团队中引起了一些沮丧情绪。

---

## 47. 奥泽皮克不减缓阿尔茨海默病，研究发现

**原文标题**: Ozempic does not slow Alzheimer's, study finds

**原文链接**: [https://www.semafor.com/article/11/25/2025/ozempic-does-not-slow-alzheimers-study-finds](https://www.semafor.com/article/11/25/2025/ozempic-does-not-slow-alzheimers-study-finds)

制造商诺和诺德（Novo Nordisk）进行的一项为期两年的研究得出结论，广受欢迎的减肥药Ozempic（诺和泰）并不能减缓阿尔茨海默病（老年痴呆症）的进展。这一发现淡化了此前的一些猜测，即这种以帮助肥胖患者减轻体重而闻名的药物，可能还会减缓各种脑部疾病、癌症和其他健康问题的进展。

研究人员此前曾质疑，观察到的任何益处究竟是药物的直接作用，还是仅仅是肥胖减轻的后果，抑或是关注健康的患者本身就是一个混杂因素。这项研究结果与帕金森病（Parkinson's disease）的类似结果一致，在帕金森病的研究中，Ozempic也未能减缓神经退行性病变。

尽管在神经系统疾病方面遭遇挫折，但该药物对心血管和肾脏问题的积极影响似乎更为显著。消息公布后，诺和诺德的股价下跌了6%。

---

## 48. Netflix订阅费能买到什么？

**原文标题**: What you can get for the price of a Netflix subscription

**原文链接**: [https://nmil.dev/what-you-can-get-for-the-price-of-a-netflix-subscription](https://nmil.dev/what-you-can-get-for-the-price-of-a-netflix-subscription)

作者决定取消他们的Netflix订阅，因为他们发现它使用率低且内容不吸引人。他们将每月约19.99欧元的费用重新分配给了三个每天都会使用的不同订阅，从而促进了主动参与而非被动消费。

首先，一项**Zed Pro**订阅（约10欧元）提升了他们的编程体验，让这项深受喜爱的爱好变得更加愉快，并鼓励更积极的参与。这里的核心信息是投资于能让爱好更具吸引力的工具，从而激励人们将时间花在有意义的活动上。

其次，一项**Kagi**订阅（约5欧元）提供了无广告的搜索体验。作者强调了为每天使用的服务直接付费的价值，以避免用注意力和忍受广告来交换，从而支持他们真正重视的产品。

最后，一台廉价的**Hetzner服务器**（约4欧元）提供了他们在互联网上的个人空间，用于托管他们的博客，并鼓励学习和参与构建事物。

总之，本文倡导摆脱默认的流媒体订阅。花同样的钱，个人可以构建一套有用的工具，这些工具能提升爱好、最大程度地减少广告曝光，并赋能创作和学习。作者还指出，本文是人工撰写的，没有使用AI。

---

## 49. 谷歌将寻求医疗服务的美国人引向“垃圾保险”

**原文标题**: Google steers Americans looking for health care into "junk insurance"

**原文链接**: [https://pluralistic.net/2025/11/25/open-season/](https://pluralistic.net/2025/11/25/open-season/)

无法访问文章链接。

---

## 50. 布达佩斯出土1700年罗马石棺

**原文标题**: 1,700-year-old Roman sarcophagus is unearthed in Budapest

**原文链接**: [https://apnews.com/article/hungary-roman-sarcophagus-discovery-budapest-77a41fe190bbcc167b43d05141536f54](https://apnews.com/article/hungary-roman-sarcophagus-discovery-budapest-77a41fe190bbcc167b43d05141536f54)

布达佩斯的考古学家发掘出一个保存完好的1700年历史的罗马石棺，这为我们了解古阿奎库姆（Aquincum）定居点一名年轻女性的生活提供了难得的窗口。这个石灰石棺椁在奥布达区被发现，当时它被密封完好，未遭盗墓者破坏，棺盖仍用金属夹和熔铅固定着。

打开后，研究人员发现了一具完整的骨骸，根据其尺寸和随葬品判断，应属于一名年轻女性。石棺内有数十件文物，包括两件完好无损的玻璃器皿、青铜小雕像、140枚硬币、一根骨发簪、琥珀首饰，以及金线织物的痕迹。这些物品象征着她“永恒旅程”的礼物，反映了罗马的丧葬习俗及其亲属的深切关怀。

首席考古学家加布里埃拉·费涅什（Gabriella Fényes）强调了这种完好无损的定制石棺的稀有性，这表明逝者很可能家境富裕或社会地位较高。该石棺位于阿奎库姆一个废弃区域内的墓地中，靠近一条罗马渡槽。

人类学家现在将检查这名女性的遗骸，以确定她的年龄、健康状况和出身，同时，石棺内的一层泥土也将被筛查，以寻找耳环等潜在的额外宝藏。这项发现提供了宝贵的科学见解，并让我们对古人表达爱与奉献的方式有了情感上的共鸣。

---

## 51. ZoomInfo 首席执行官在研究员披露未经同意的生物识别追踪后将其拉黑

**原文标题**: ZoomInfo CEO blocks researcher after documenting pre-consent biometric tracking

**原文链接**: [https://github.com/clark-prog/blackout-public](https://github.com/clark-prog/blackout-public)

2025年11月25日，安全研究员Blackout Research记录了ZoomInfo的GTM Studio着陆页上存在大量未经用户同意的生物识别跟踪行为。调查结果发布到LinkedIn后，ZoomInfo的CEO Henry Schuck屏蔽了该研究员。

调查显示，在同意横幅加载之前，已有超过50个跟踪请求被触发。主要发现包括：
*   **Sardine.ai** 生物识别功能已启用（在解码配置中显示 `enableBiometrics: true`），用于跟踪鼠标移动、打字模式和DNS指纹。
*   **PerimeterX** 指纹识别和 **IdentityMatrix.ai** 也处于活跃状态，同时还伴有用于欺诈检测的会话指纹。
*   在单次页面加载中，总共联系了 **118个独特的跟踪域**。

值得注意的是，ZoomInfo将其GTM Studio产品宣传为“识别个人层面的网站访问”，然而讽刺的是，它却在其自己的产品页面上依赖三个外部身份供应商并进行大量未经同意的跟踪。

Blackout Research警告营销人员，这会带来重大影响：包括供应商潜在的法律风险、未经同意收集“意图数据”的法律风险、客户可能成为原告、因供应商不合规（GDPR、CCPA、CIPA）而产生的连带责任，以及竞争劣势。

CEO在未对调查结果提出异议或澄清的情况下屏蔽研究员的举动，更加突显了报告中的论断：“你可以屏蔽研究员，但你无法屏蔽证据。”Blackout Research为此发布了一份全面的证据包，以确保这些做法的透明度。

---

## 52. 贝尔格莱德卡吉中心

**原文标题**: Kagi Hub Belgrade

**原文链接**: [https://blog.kagi.com/kagi-hub](https://blog.kagi.com/kagi-hub)

Kagi已宣布其贝尔格莱德中心将于2025年11月21日开放。这将是Kagi的首个实体办公室，旨在兼作所有Kagi会员和Kagi团队的免费共享办公空间。该现代化办公室位于塞尔维亚贝尔格莱德市中心，占地250平方米，旨在为用户和团队提供一个线下空间，供他们分享反馈、交流想法，并共同努力构建一个更好的互联网。

Kagi会员可于12月15日起通过 hub.kagi.com 预订。会员每月可免费预订最多五天的工位，享用设有25张人体工学办公桌的安静开放式工作区、高速Wi-Fi、免费咖啡和茶、小型厨房以及会议室（需视可用情况而定）。中心运营时间为周一至周五，上午10:00至晚上7:00。

贝尔格莱德被战略性地选中，因为它地处东西方交汇点，拥有蓬勃发展的科技行业，并且对Kagi的创始人兼首席执行官具有历史意义。Kagi中心被视为Kagi将其运动延伸到物理世界的首次尝试，旨在支持构建一个摆脱广告、追踪和不惜一切代价追求参与度的互联网的愿景。公司欢迎所有会员，无论本地还是国际会员，前来交流并贡献。

---

## 53. 生成式墨西哥卷饼测试

**原文标题**: The Generative Burrito Test

**原文链接**: [https://www.generativist.com/notes/2025/Nov/25/generative-burrito-test.html](https://www.generativist.com/notes/2025/Nov/25/generative-burrito-test.html)

“生成式墨西哥卷饼测试”是一个旨在评估各种图像生成模型性能的基准测试。该测试灵感来源于“宇航员骑马”迷因以及西蒙的“鹈鹕”基准测试，它使用墨西哥卷饼，作者最初认为由于卷饼在训练数据中很常见，模型应该很容易描绘它们。

然而，创建者发现模型难以准确地表现出墨西哥卷饼食材那种复杂、“压扁揉碎”的特性。该测试使用一个单一、标准化的提示语：“A partially eaten burrito with cheese, sour cream, guacamole, lettuce, salsa, pinto beans, and chicken。”一个关键的方法是对所有生成采用“fal 默认参数”，明确避免任何人工干预（HIL）或提示词优化，以防止“作弊”，并确保对模型能力进行原始评估。

文章列出了许多经过测试的模型，包括SD 1.5、Fast SDXL、Flux Schnell、Ideogram V2/V3、SD v3.5、Imagen4 Preview等，这表明对这些生成式AI模型如何处理描绘常见但视觉上复杂的食物进行了全面比较。

---

## 54. 同卵双胞胎分开抚养后的智商差异受教育影响

**原文标题**: IQ differences of identical twins reared apart are influenced by education

**原文链接**: [https://www.sciencedirect.com/science/article/pii/S0001691825003853](https://www.sciencedirect.com/science/article/pii/S0001691825003853)

无法访问文章链接。

---

## 55. 黑客入侵金融科技公司后，美国多家银行争相评估数据失窃。

**原文标题**: US banks scramble to assess data theft after hackers breach financial tech firm

**原文链接**: [https://techcrunch.com/2025/11/24/us-banks-scramble-to-assess-data-theft-after-hackers-breach-financial-tech-firm/](https://techcrunch.com/2025/11/24/us-banks-scramble-to-assess-data-theft-after-hackers-breach-financial-tech-firm/)

包括摩根大通、花旗集团和摩根士丹利在内的美国银行，正在争相评估金融科技公司SitusAMC遭受网络攻击后发生的客户数据失窃事件。这家总部位于纽约、为一千多家商业和房地产金融机构提供技术的公司，于11月12日证实发生了一起数据泄露事件。

黑客窃取了与其银行客户关系相关的企业数据，以及会计记录和法律协议。SitusAMC澄清说，没有使用加密恶意软件，这表明攻击者的重点是窃取数据而非造成破坏。该事件目前已得到“控制”，系统已恢复运行，尽管影响范围仍在调查中。

SitusAMC充当中介，每年处理大量的非公开银行信息和数十亿份贷款文件。尽管受影响消费者的全面范围尚不清楚，但联邦调查局（FBI）已知晓此次泄露事件，并表示到目前为止，“银行服务尚未受到运营影响”。受影响的银行大多拒绝置评。

---

## 56. KDE Plasma 6.8 将独占 Wayland，放弃 X11 会话支持

**原文标题**: KDE Plasma 6.8 Will Go Wayland-Exclusive in Dropping X11 Session Support

**原文链接**: [https://www.phoronix.com/news/KDE-Plasma-68-Wayland-Exclusive](https://www.phoronix.com/news/KDE-Plasma-68-Wayland-Exclusive)

KDE 开发者宣布 Plasma 6.8 将仅支持 Wayland，从而有效地停止对 Plasma X11 会话的支持。这一战略举措表明他们致力于“全力投入 Wayland 的未来”，因为“绝大多数”用户已经在使用 Wayland 会话。

此次转型旨在通过将精力从 X11 会话维护中转移出来，从而解锁新功能、促进优化并加速开发。虽然 X11 会话支持正在逐步淘汰，但 X11 应用程序和游戏将继续通过 XWayland 得到支持。

目前依赖 X11 会话的用户将通过 Plasma 6.7 系列获得支持，该系列预计将持续发布错误修复版本直至 2027 年初。有关此更改的更全面详细信息可在 KDE.org 官方博客上查阅。该公告由 Michael Larabel 于 2025 年 11 月 26 日发布。

---

## 57. LLVM将迎来常数时间支持：保护加密代码

**原文标题**: Constant-time support coming to LLVM: Protecting cryptographic code

**原文链接**: [https://blog.trailofbits.com/2025/11/25/constant-time-support-coming-to-llvm-protecting-cryptographic-code-at-the-compiler-level/](https://blog.trailofbits.com/2025/11/25/constant-time-support-coming-to-llvm-protecting-cryptographic-code-at-the-compiler-level/)

无法访问文章链接。

---

## 58. Cloudflare宕机本不该发生。

**原文标题**: Cloudflare outage should not have happened

**原文链接**: [https://ebellani.github.io/blog/2025/cloudflare-outage-should-not-have-happened-and-they-seem-to-be-missing-the-point-on-how-to-avoid-it-in-the-future/](https://ebellani.github.io/blog/2025/cloudflare-outage-should-not-have-happened-and-they-seem-to-be-missing-the-point-on-how-to-avoid-it-in-the-future/)

Eduardo Bellani 批评 Cloudflare 在2025年11月18日的宕机事件，认为他们的根本原因分析（RCA）未能抓住核心教训。此次宕机源于一个数据库查询，该查询是Cloudflare Bot Management的关键组成部分，但缺少数据库名称过滤器。当授予新权限时，该查询意外地从底层 `r0` 数据库返回了重复的列条目，导致返回的行数是预期值的两倍多。应用程序代码未能为这种增加的数据做好准备，随后导致核心系统崩溃。

尽管Cloudflare提出了合理的预防措施，例如强化数据摄取和实施全局终止开关，但Bellani认为这些措施治标不治本。他声称Cloudflare误将物理复制等同于防止逻辑单点故障，将一个逻辑问题当作物理问题来处理。他指出Cloudflare采用ClickHouse优先考虑速度，而非确保逻辑正确性和一致性。

Bellani将此类宕机归因于“应用程序逻辑与数据库模式之间不受控制的交互”。他主张通过分析设计，从“结构上”预防这些问题。他的建议包括消除可空字段、确保数据库完全规范化，以及使用经过形式化验证的应用程序代码。他总结道，尽管采用这些“形式化方法”和“关系严格性”可能不受欢迎，但对于关键系统而言，它们对于实现“设计上不可能发生”的故障至关重要，最终将造福互联网。

---

## 59. 在同等价格下，AWS 比专用服务器慢10倍 [视频]

**原文标题**: AWS is 10x slower than a dedicated server for the same price [video]

**原文链接**: [https://www.youtube.com/watch?v=Ps3AI1kTIR4](https://www.youtube.com/watch?v=Ps3AI1kTIR4)

所提供的文章标题“在同等价格下，AWS比专用服务器慢10倍[视频]”就亚马逊网络服务（AWS）与专用服务器解决方案的性能与成本比率提出了一个惊人的主张。它声称AWS基础设施提供的性能明显低于专用服务器——具体来说，慢了十倍——即使在比较价格相同的服务时。“[视频]”标签表明，这个主张可能得到了以视频形式呈现的视觉演示、基准测试或详细比较的支持。

然而，所提供的“内容”部分仅仅包含了一系列通用的YouTube页脚链接、法律免责声明和版权信息（例如：“YouTube关于新闻版权联系我们创作者广告开发者条款隐私权政策与安全YouTube 的运作方式测试新功能NFL Sunday Ticket© 2025 Google LLC”）。它不包含任何实际的正文、论点、证据或具体细节来阐述或支持标题中提出的主张。因此，由于文章的实际内容缺失，无法根据所提供的信息，就AWS性能与专用服务器的比较，提供一份关于文章主要观点、方法或结论的全面总结。

---

## 60. 欧盟将于明天不经讨论通过“聊天管控”谈判授权。

**原文标题**: EU set to adopt ChatControl negotiating mandate tomorrow without discussion

**原文链接**: [https://digitalcourage.social/@echo_pbreyer/115611006935923542](https://digitalcourage.social/@echo_pbreyer/115611006935923542)

据Patrick Breyer在digitalcourage.social上分享的消息，欧盟据报道最早将于明天准备通过一项关于“聊天控制”（ChatControl）的谈判授权。强调的关键细节是，欧盟各国政府大使预计将“不经讨论”地通过这项授权，这引发了人们对这项有争议的措施缺乏辩论的担忧。

---

## 61. 你的安卓电视盒子是僵尸网络的一部分吗？

**原文标题**: Is your Android TV streaming box part of a botnet?

**原文链接**: [https://krebsonsecurity.com/2025/11/is-your-android-tv-streaming-box-part-of-a-botnet/](https://krebsonsecurity.com/2025/11/is-your-android-tv-streaming-box-part-of-a-botnet/)

Superbox等安卓电视流媒体盒子在大型零售商处以约400美元的一次性费用出售，承诺无限访问数千种流媒体服务，绕过每月订阅费。然而，安全专家警告称，这些设备强制安装了侵入性软件，强迫用户网络为他人中继互联网流量，通常用于网络犯罪活动，例如广告欺诈和账户盗用。

Censys的一名分析师发现，Superbox设备会立即联系中国的腾讯QQ和一个名为Grass IO的住宅代理服务。尽管Grass IO宣传通过共享带宽进行AI研究来赚取奖励，但其创始人否认与Superbox有任何关联，并表示这些盒子利用的是一个不道德的代理网络。Superbox设备还包含强大的网络分析和远程访问工具，并执行DNS劫持。为了访问这些“免费”内容，用户必须用一个非官方应用商店取代谷歌官方的Play Store来下载特定应用。Superbox声明他们只销售硬件，以此推卸责任。

这个问题不仅仅局限于Superbox。谷歌对一个由超过1000万台安卓流媒体设备组成的僵尸网络提起了“BadBox 2.0 Enterprise”诉讼，该网络从事广告欺诈活动，这些设备通常预装了恶意软件或在应用下载过程中被感染。联邦调查局也警告称，像这类被入侵的物联网设备会成为BADBOX 2.0僵尸网络的一部分，该僵尸网络与IPidea（被制裁的911S5 Proxy的更名）相关联，助长了数十亿美元的网络犯罪，包括广告欺诈和账户盗用。

文章总结道，尽管消费者可能节省了流媒体费用，但他们的互联网连接却被用于非法活动，而且往往是在他们不知情的情况下，这印证了一句格言：“如果某样东西是免费的，那么你就是产品。”

---

## 62. 可以说“CSS变量”而不是“自定义属性”

**原文标题**: It is ok to say "CSS variables" instead of "custom properties"

**原文链接**: [https://blog.kizu.dev/css-variables/](https://blog.kizu.dev/css-variables/)

文章主张，将“CSS变量”与“自定义属性”互换或并用是完全可以接受的。作者指出，尽管这并非争议性问题，但术语选择可能会导致犹豫。

为了证明这一立场，作者指出，官方CSS模块名为“CSS Custom Properties for Cascading Variables”，其规范URL别名为“css-variables”。它们确实是变量，特别是“层叠变量”，能够通过层叠动态改变、被覆盖、进行动画，并响应视口或容器大小等条件。虽然它们也是“自定义属性”，尤其是在使用`@property`明确声明类型时，但其变量本质是不可否认的。

作者在TPAC 2025大会后感到疲惫，简要指出CSS和HTML是编程语言。他们最后提到了一项成功的实验和一篇计划中的未来文章。

---

## 63. 图像扩散模型在视频中展现涌现的时序传播

**原文标题**: Image Diffusion Models Exhibit Emergent Temporal Propagation in Videos

**原文链接**: [https://arxiv.org/abs/2511.19936](https://arxiv.org/abs/2511.19936)

《图像扩散模型在视频中展现涌现的时间传播》探讨了图像扩散模型超越其在图像生成中的主要用途的潜在能力，并将其应用于视频分析。该论文提出，这些模型中的自注意力图隐式地捕获了丰富的语义结构，充当着鲁棒的语义标签传播核。这些核有助于促进相关图像区域之间的像素级对应关系。

通过将这一机制扩展到视频帧之间，作者推导出了一个时间传播核，从而通过分割实现零样本目标跟踪。这利用了扩散模型固有的语义理解能力，而无需对视频任务进行显式训练。为了增强标签传播的鲁棒性和一致性，该研究采用了DDIM反演、文本反演和自适应头部加权等测试时优化策略。

这项研究最终形成了DRIFT，这是一个利用预训练图像扩散模型并结合SAM引导的掩码细化的目标跟踪框架。DRIFT在标准视频目标分割基准上展现了最先进的零样本性能，展示了图像扩散模型涌现的时间传播能力。

---

## 64. Windows GUI——好、坏与奇丑无比 (2023)

**原文标题**: Windows GUI – Good, Bad and Pretty Ugly (2023)

**原文链接**: [https://creolened.com/windows-gui-good-bad-and-pretty-ugly-ranked/](https://creolened.com/windows-gui-good-bad-and-pretty-ugly-ranked/)

本文回顾并排名了从1985年到2023年微软Windows操作系统的所有主要图形用户界面（GUI），根据它们当前的美学吸引力，以1到10个Clippy的等级进行评分。

**Windows 1.0 (1 Clippy)** 和 **2.0 (2.5 Clippys)** 因早期的图形限制被认为“丑陋”且“缺乏吸引力”。**Windows 3.0/3.1 (6 Clippys)** 标志着一次重大飞跃，具有连贯的伪3D图形用户界面和VGA支持，显得更加专业。**Windows 95/98 (7.5 Clippys)** 引入了任务栏和开始按钮等标志性功能，改进了3D斜面外观并保持了功能性。**Windows 2000 (8 Clippys)** 因其精致的表面和改进的图标而略占优势。

**Windows XP (6 Clippys)** 被认为是一种“倒退”，带有“卡通化”且不那么严肃的外观。**Windows Vista/7 (7.5 Clippys)** 引入了光泽的3D光泽和透明效果（在Windows 7中有所减弱），旨在打造一种“成熟”的美学。**Windows 8 (5 Clippys)** 和 **8.1 (5.5 Clippys)** 是重大的“倒退”，因其以平板电脑为中心的设计、“丑陋”的磁贴以及移除了开始菜单而受到批评。**Windows 10 (6.5 Clippys)** 是一个“杂合操作系统”，它试图修复Windows 8，但感觉缺乏规划，保留了扁平的外观。

**Windows 11 (8 Clippys)** 被誉为自2000年以来最“精致”的版本，因其连贯性、简洁的设计和圆角而受到赞扬，尽管存在一些功能上的缺陷，但在美学上超越了当前的macOS。

作者认为Windows 3.0、95、Vista和11是微软“做对了”的图形用户界面，而XP和8则“失误了”。

---

## 65. 铁木，我们最新的TPU

**原文标题**: Ironwood, our latest TPU

**原文链接**: [https://blog.google/products/google-cloud/ironwood-google-tpu-things-to-know/](https://blog.google/products/google-cloud/ironwood-google-tpu-things-to-know/)

谷歌推出了其第七代张量处理单元（TPU）Ironwood，现已面向云客户开放。在Cloud Next大会上亮相的Ironwood，被誉为谷歌最强大、最能干、能效最高的定制芯片，专为高吞吐量、低延迟的AI推理和模型服务而设计，为复杂的AI模型提供强大算力。

Ironwood 的三大关键特性突显其强大能力：

1.  **专为推理而打造：** Ironwood 旨在适应交互式AI的发展趋势，与前代产品相比，其在训练和推理方面，每芯片性能提升超过4倍，显著加速了复杂的AI计算。
2.  **强大的互联网络：** 作为谷歌AI超算（AI Hypercomputer）的核心组件，Ironwood TPU在一个超级Pod中可扩展至9216颗芯片。这些芯片通过一个9.6 Tb/s的芯片间互连（ICI）网络互联，提供高速通信并可访问1.77拍字节（PB）的共享高带宽内存（HBM）。这种大规模连接减少了先进AI服务的数据瓶颈、计算时长和能耗。
3.  **由AI设计，专为AI打造：** Ironwood 得益于独特的内部协作，其中谷歌DeepMind研究人员直接影响硬件设计，而硬件则反过来加速了研究。谷歌还利用AI，特别是通过强化学习实现的AlphaChip方法，为其包括Ironwood在内的最新TPU代次设计出更优越的芯片布局。

---

## 66. Await 不是上下文切换：理解 Python 的协程与任务

**原文标题**: Await Is Not a Context Switch: Understanding Python's Coroutines vs. Tasks

**原文链接**: [https://mergify.com/blog/await-is-not-a-context-switch-understanding-python-s-coroutines-vs-tasks](https://mergify.com/blog/await-is-not-a-context-switch-understanding-python-s-coroutines-vs-tasks)

本文旨在解决对 Python `async` 模型的一个常见误解，尤其是对于熟悉 JavaScript、C# 或 Java 的工程师而言。在这些语言中，`await` 通常意味着“将控制权交给运行时/事件循环”，自动暗示着潜在的上下文切换和并发。

然而，Python 在以下两者之间进行了区分：
1.  **协程 (`async def`)：** 它们仅仅是状态机，当被 `await` 时，会在当前任务中*同步*执行，直到它们*自身*遇到一个尚未准备就绪的 `awaitable` 对象（例如 `asyncio.sleep`）。`await` 一个裸协程*并不会*将控制权交还给事件循环。
2.  **任务 (`asyncio.create_task`)：** 任务是 Python 真正的并发单元。事件循环只会在*任务*之间进行交错。`await` 一个*任务*（它代表着已调度的工作）*确实会*将控制权交给事件循环，从而允许其他任务运行。

这一关键差异意味着并发仅源于任务，并且只在这些任务中明确的挂起点才会发生。单纯的存在 `async` 或 `await` 并不能保证交错执行。因此，只有当共享数据可能在*任务*之间，并且在实际挂起点被并发访问时，才需要加锁。如果一个临界区不包含任何 `await` 调用，那么它相对于事件循环而言是原子的，无论它是否是一个 `async` 函数。

Python 的设计从生成器演变而来，提供了对何时可以发生交错执行的细粒度控制。工程师应该审查任务的创建点和挂起点，以确定并发真正存在于何处以及真正需要锁的地方。

---

## 67. 一项研究表明，一些服用GLP-1药物的人可能没有安全的退出途径。

**原文标题**: There may not be a safe off-ramp for some taking GLP-1 drugs, study suggests

**原文链接**: [https://arstechnica.com/health/2025/11/glp-1-drugs-improve-heart-health-but-only-if-you-keep-taking-them/](https://arstechnica.com/health/2025/11/glp-1-drugs-improve-heart-health-but-only-if-you-keep-taking-them/)

《美国医学会内科杂志》最近发表的一项分析指出，停用替西帕肽（Zepbound）等GLP-1减肥药物会导致大多数使用者体重显著反弹，并使健康益处逆转。这促使专家们提出，应将这些药物重新定义为“体重管理”药物，可能需要无限期使用，类似于治疗其他慢性病的药物。

该研究观察了670名肥胖或超重参与者，他们服用了替西帕肽36周。那些体重至少减轻10%的人随后被随机分为继续服药组或改用安慰剂组，为期52周，同时保持饮食和锻炼。在最初受益的308名参与者中，到第88周时，82%的人体重反弹了至少25%的已减体重。此外，57%的人反弹超过一半，24%的人反弹超过四分之三。这种体重反弹伴随着心血管和代谢改善的逆转，包括血压、胆固醇、糖化血红蛋白和空腹胰岛素的升高。

尽管一小部分人（17.5%）没有显著反弹体重，但原因尚不清楚。这项研究涉及药物的突然停用，强调需要研究逐步戒断策略以及体重波动对健康的潜在影响。

专家Elizabeth Oczypok和Timothy Anderson总结说，临床医生和患者应将这些抗肥胖药物视为长期疗法，就像其他慢性病治疗一样。

---

## 68. 独立游戏开发者有了一个新卖点：“无AI”

**原文标题**: Indie game developers have a new sales pitch: being 'AI free'

**原文链接**: [https://www.theverge.com/entertainment/827650/indie-developers-gen-ai-nexon-arc-raiders](https://www.theverge.com/entertainment/827650/indie-developers-gen-ai-nexon-arc-raiders)

独立游戏开发者正越来越多地采用“无AI”的宣传策略来突出自身，强调其游戏完全由人工制作。这一反击是在Nexon首席执行官李政宪（Junghun Lee）建议所有游戏公司都应使用AI之后出现的，许多独立开发者对此表示强烈反对。

对于Polygon Treehouse的Alex Kanaris-Sotiriou等开发者而言，避免生成式AI是一种反对未经许可使用他人作品的道德立场，也是一种与重视原创的玩家建立联系的营销工具。Kanaris-Sotiriou共同设计了一个免费的、金色齿轮状的徽章，上面写着“本开发者保证此独立游戏未使用任何生成式AI”，该徽章已出现在多个独立游戏商店页面上。其他工作室，如D-Cell Games，则发布充满激情的声明，确认其游戏中的“一切”都由人类创造，认为AI是“徒劳无功”，达不到他们的质量标准。

这一立场与艺电（EA）、微软和育碧等主要发行商形成对比，后者正在整合生成式AI以简化开发、降低成本并加速游戏发布，例如《使命召唤：黑色行动6》（*Call of Duty: Black Ops 6*）和《弧光勇士》（*Arc Raiders*）等游戏就使用了AI资产。然而，独立开发者认为，他们的限制反而能催生真正的创意解决方案，使人工开发过程本身就充满价值。尽管承认AI日益普及，但他们相信，他们对人工制作内容的坚持能与玩家和社区产生深刻共鸣。

---

## 69. 这个博客现在托管在一个GPS/LTE调制解调器上 (2021)

**原文标题**: This blog is now hosted on a GPS/LTE modem (2021)

**原文链接**: [https://blog.nns.ee/2021/04/01/modem-blog](https://blog.nns.ee/2021/04/01/modem-blog)

作者发现 PinePhone 的 Quectel EG25-G GPS/LTE 调制解调器暴露了一个 Android 调试桥 (ADB) 接口，允许通过 root shell 访问其完全独立且闭源的 Linux 3.18.44 操作系统。借此机会，作者决定直接在调制解调器上托管他们的静态文件博客。

他们为 ARMv7 交叉编译了轻量级 Web 服务器 `darkhttpd`，并通过 ADB 将其与博客资源一同推送到调制解调器 50MB 可写分区 `/usrdata`。在配置 ADB 转发和 `iptables` 后，博客在 PinePhone 的本地网络上成功可访问。

吞吐量测试显示，通过 ADB 转发的连接速度约为 11.4 Mbits/秒。文章最后强调了重大的安全隐患：获取 root 权限的简易性以及潜在的命令注入漏洞可能导致持久性恶意软件。此类恶意软件可以在宿主操作系统重装后仍然存在，可能窃听通信或追踪位置，尽管与宿主操作系统的直接交互有限。

---

## 70. 触目惊心的科技就业新数据

**原文标题**: The gruesome new data on tech jobs

**原文链接**: [https://www.businessinsider.com/gruesome-tech-jobs-data-scientists-analytics-indeed-2025-11](https://www.businessinsider.com/gruesome-tech-jobs-data-scientists-analytics-indeed-2025-11)

很抱歉，我无法提供对题为《科技工作岗位的新残酷数据》一文的简洁摘要，因为文章本身的内容并未提供。

您提供的文本只包含标题和出版商的标语（“Business Insider 讲述你想了解的创新故事”）。

要提供准确的摘要，请提供文章的全文。仅凭标题判断，这篇文章可能深入探讨关于科技行业就业的负面或具有挑战性的数据和趋势，例如裁员、招聘冻结或就业增长放缓。

---

## 71. HN 展示：一个 WordPress 插件，重写图片 URL 以实现近乎零成本分发

**原文标题**: Show HN: A WordPress plugin that rewrites image URLs for near-zero-cost delivery

**原文链接**: [https://wordpress.org/plugins/bandwidth-saver/](https://wordpress.org/plugins/bandwidth-saver/)

"Bandwidth Saver" 是一款 WordPress 插件，它通过从 Cloudflare 的全球内容分发网络 (CDN) 交付图像，并利用 Cloudflare R2 实现近乎零成本的数据传输，从而优化网站性能。其旨在通过从离每个访客最近的服务器提供图像，来减少页面加载时间和带宽消耗。

主要功能包括：
*   **零出站费用：** 基于 Cloudflare R2 构建，消除了数据传输成本。
*   **一键设置（托管模式）：** 无需 Cloudflare 账户或复杂的配置。
*   **广泛兼容性：** 兼容所有主流主题、页面构建器（Gutenberg、Elementor）以及缓存/优化插件（ShortPixel、WP Rocket）。
*   **防弹级故障恢复：** 如果 CDN 不可用，图像会自动从您的服务器加载。
*   **自动重写：** 插件会将图像 URL 重写指向 Cloudflare，并在首次访问时对其进行缓存。

用户可在两种模式之间选择：
1.  **托管模式（推荐）：** 每月 2.99 美元，提供无限图像和带宽，由 ImgPro 负责基础设施。
2.  **自托管模式（免费）：** 用户部署到自己的 Cloudflare 账户，提供完全控制，并且在免费套餐下通常不产生费用。Cloudflare Worker 是开源的。

该插件侧重于交付而非优化，可与现有图像压缩或 WebP 转换工具无缝协作。它尊重隐私，不收集访客数据、cookie 或分析信息。托管模式的安装非常简单。目前处于早期开发阶段 (v0.1.3)，安装量较少，支持 WordPress 6.2+ 和 PHP 7.4+。

---

## 72. 一个花架子SaaS毁了我的团队

**原文标题**: A Vibe Coded SaaS Killed My Team

**原文链接**: [https://cendyne.dev/posts/2025-11-26-a-vibe-coded-saas-killed-my-team.html](https://cendyne.dev/posts/2025-11-26-a-vibe-coded-saas-killed-my-team.html)

作者详细阐述了他们公司即将关闭的情况。该公司因收入下降和过度招聘，选择了一种激进的转型方式，而非体面的退出。投资者决定迁移到一个第三方“凭感觉编码”（vibe coded）的SaaS平台，希望裁减几乎所有员工（工程、实施、支持），并依赖合同销售人员。作者的任务是在被解雇前，独自再完成一两个月的迁移工作。

在简短测试期间，作者立即发现了严重的法律风险：该SaaS由一个没有美国客户的外国团队开发，违反了包括CCPA、CPRA、TCPA、CAN-SPAM和ADA在内的主要美国法律。在功能上，该平台严重残缺，体现了“凭感觉编码”——即忽视实际代码，转而依赖LLM（大型语言模型）提示生成。它具有无效按钮、损坏的模态窗口、肤浅的用户界面元素，以及关键业务缺陷，例如允许在没有付款或联系方式的情况下下单。

作者感叹领导层被该应用程序的表面外观“蒙蔽”了。尽管接受公司的财务失败是根本原因，但作者难以接受自己因不符合法律规定且功能严重缺陷的软件而被取代。文章最后警告了在缺乏专家监督的情况下使用LLM生成代码的危险，并预测更多“疏忽大意的软件”将对人们的生活产生负面影响。然而，作者仍致力于专业地完成他们的迁移任务。

---

## 73. DRAM价格暴涨，但我并不信任行业给出的理由。

**原文标题**: DRAM prices are spiking, but I don't trust the industry's why

**原文链接**: [https://www.xda-developers.com/dram-prices-spiking-dont-trust-industry-reasons/](https://www.xda-developers.com/dram-prices-spiking-dont-trust-industry-reasons/)

2025年全球DRAM价格飙升，DDR5内存模组价格翻倍，且第三季度整体合约价格同比上涨171.8%。此次涨价影响了消费者、PC制造商、OEM厂商和云服务提供商，有报道称，价格翻了两番，出现配给制，NAND闪存和硬盘驱动器（HDD）的成本也在上升。

业内将此归因于人工智能数据中心对海量内存和存储的旺盛需求，加上供应受限。制造商在之前的低迷期（2022年）削减了产量，现在则由于更高的利润率，优先生产高带宽内存（HBM），从而将产能从标准DRAM转移开。他们也犹豫是否大幅增加整体产量，担心潜在的人工智能泡沫破裂。

然而，作者对此表示怀疑，并指出内存行业有操纵价格的历史。DRAM市场是由三星、SK海力士和美光主导的寡头垄断，他们都在21世纪初因串通（价格共谋）而被罚款。尽管2016-2018年的一项集体诉讼失败了，但怀疑依然存在。作者指出，这“三大巨头”目前正从短缺中获得创纪录的利润，并且不急于扩大标准DRAM产能。相反，他们正在集体采取一种“谨慎”的方法：优先生产HBM，逐步淘汰DDR4，推迟新的晶圆厂项目，并避免价格战。这种同步的、维护利润的策略，加上过去的先例，表明即使人工智能需求是一个真实因素，也可能存在有利于主导厂商的潜在默契协调。预计这种情况至少在未来一年内不会有所改善。

---

## 74. 美国环保署刚刚批准了可用于食品的新型“永久化学品”农药。

**原文标题**: EPA just approved new 'forever chemical' pesticides for use on food

**原文链接**: [https://www.washingtonpost.com/climate-environment/2025/11/22/forever-chemicals-pesticides/](https://www.washingtonpost.com/climate-environment/2025/11/22/forever-chemicals-pesticides/)

无法访问文章链接。

---

## 75. Scaleway 将 Mac mini 转化为高密度、树莓派管理的服务器

**原文标题**: Scaleway turns Mac Minis into high‑density, Raspberry Pi–managed servers

**原文链接**: [https://www.scaleway.com/en/blog/how-we-turn-apples-mac-mini-into-high-performance-dedicated-servers/](https://www.scaleway.com/en/blog/how-we-turn-apples-mac-mini-into-high-performance-dedicated-servers/)

Scaleway 通过整合虚拟私有云（VPC）功能，大幅增强了其 Apple Silicon Mac mini 服务器产品。Scaleway 以利用 Mac mini 作为高密度、由树莓派管理的服务器而闻名，此举使其能够为客户提供高级私有网络功能和更高的隔离性。这代表着他们在云服务领域迈出了关键一步，使其 Mac mini 部署更加多功能和安全。

---

## 76. 微软不理解对 Windows 新方向的反感。

**原文标题**: Microsoft doesn't understand the dislike for Windows' new direction

**原文链接**: [https://www.xda-developers.com/microsoft-doesnt-understand-dislike-windows-new-direction/](https://www.xda-developers.com/microsoft-doesnt-understand-dislike-windows-new-direction/)

微软正因其新的“代理式”Windows方向而面临用户的强烈反对，该方向旨在将AI（Copilot）深度嵌入到整个操作系统中，使AI负责大部分决策和繁重工作。尽管用户普遍不赞同，该公司，包括其AI首席执行官穆斯塔法·苏莱曼，似乎对这种负面反响感到困惑。

用户明确表达了他们的反对意见：他们的问题不在于AI本身，而在于它被强制性且无处不在地整合到Windows的各个方面——例如任务栏、文件系统和浏览器。批评人士认为，微软正在“将解决方案强行注入一个不存在的‘问题’中”，并强调他们不希望AI无处不在地扩散到整个操作系统中。相反，他们主张在AI能提供真正价值并解决具体问题的特定应用程序中，进行有针对性的AI实施。

文章强调了微软内部“AI不再是可选项”的信念与用户对更聚焦的AI实用性需求之间的脱节。文章警告说，如果微软继续无视用户反馈并积极推行其代理式愿景，它将面临疏远用户群而非建立忠诚度的风险。

---

## 77. 司法部要求瑞尔佩奇停止共享竞争敏感信息

**原文标题**: Justice dept. requires RealPage end sharing competitively sensitive information

**原文链接**: [https://www.justice.gov/opa/pr/justice-department-requires-realpage-end-sharing-competitively-sensitive-information-and](https://www.justice.gov/opa/pr/justice-department-requires-realpage-end-sharing-competitively-sensitive-information-and)

司法部反垄断司已向为租赁住房提供收益管理软件的公司RealPage Inc.提交了一项拟议和解协议，以终止反竞争行为。RealPage被指控利用房东分享的非公开、竞争敏感信息来设定租金价格、限制价格下降，并协调竞争对手之间的定价，这通常是通过其软件和公司主办的会议促成的。

这项拟议的同意判决旨在通过要求RealPage采取以下措施来恢复自由市场竞争：
*   停止使用竞争对手的非公开实时数据来确定租金价格。
*   将软件模型训练限制为至少12个月前的历史非公开数据。
*   停止使用范围小于州级的地理效应模型。
*   移除或重新设计限制价格下降或协调定价的功能。
*   停止进行敏感信息市场调查，并在会议中避免讨论非公开数据或定价策略。
*   接受法院指定的合规监督员。
*   配合正在进行的针对物业管理公司的诉讼。

这项行动强调了司法部对算法协调和信息共享行为进行严格反垄断执法的承诺。根据《滕尼法案》的要求，公众有60天时间对拟议和解协议发表评论。

---

## 78. BebboSSH：Amiga 系统上的 SSH2 实现 (68000, GPLv3)

**原文标题**: BebboSSH: SSH2 implementation for Amiga systems (68000, GPLv3)

**原文链接**: [https://franke.ms/git/bebbo/bebbossh](https://franke.ms/git/bebbo/bebbossh)

BebboSSH 是一款获得 GPLv3+ 许可的 Amiga 系统 (68000+ 处理器) SSH2 实现，提供现代安全 Shell、SCP 和 SFTP 功能。它包含一整套工具：`bebbosshd` (服务器端)、`bebbossh` (客户端)、`bebboscp` (文件传输) 和 `bebbosshkeygen` (Ed25519 密钥生成器)，以及加密库 (`libcryptossh.library`)。

该软件支持 curve25519-sha256、ssh-ed25519、aes128-gcm@openssh.com 和 chacha20-poly1305@openssh.com 等现代密码，需要兼容的现代服务器和 `bsdsocket.library` (例如 AmiTCP)。

尽管在未加速的 Amiga (68000 处理器) 上也能正常运行，但连接可能需要大约一分钟，BebboSSH 已针对更快的 CPU 进行了优化。使用加速器时性能显著提升，当使用 `libcryptossh.library020` 时，在 V4SA/68080 上 SCP 传输速度可达 396 kB/s。

功能包括配置文件支持、密钥认证、端口转发和终端仿真 (推荐使用 `xterm-amiga` terminfo)。BebboSSH 从其“AmigaSSH”的根源持续发展，专注于速度提升和现代密码集成。文档还提供必要的配置技巧和常见问题的故障排除，确保经典 Amiga 硬件的现代安全网络连接。

---

## 79. 航海家1号临近距地球一光日

**原文标题**: Voyager 1 approaches one light day from Earth

**原文链接**: [https://newatlas.com/space/voyager-approaches-1-light-day-from-earth/](https://newatlas.com/space/voyager-approaches-1-light-day-from-earth/)

美国宇航局的旅行者1号探测器正接近一个历史性的里程碑，预计将于2026年11月15日成为第一个距离地球一光日远的航天器。届时，它将距离地球约161亿英里（259亿公里），这意味着来自地球的无线电信号将需要24小时才能到达它。

这篇文章强调了太空的浩瀚以及光速对通信的影响。尽管光以每秒18.6万英里的速度传播，但太空中的距离造成了显著的延迟：到月球需要2.6秒，到火星最长需要四分钟，到冥王星需要6.8小时。这种延迟使得深空任务必须使用高度自主的机器人航天器。

旅行者1号于1977年发射，至今已有近50年的历史，尽管环境恶劣，它仍在继续运行，不过其核电源预计将在未来一年左右失效。目前，它距离地球157亿英里（253亿公里），单向通信延迟超过23小时。

两艘旅行者探测器都通过美国宇航局的深空网络与任务控制中心保持联系。然而，旅行者1号一旦达到一光日的距离，发送的任何指令都将需要整整两天才能收到确认，这对航天机构的工程师们构成了前所未有的挑战。

---

## 80. 从血糖到大脑缓解：GLP-1疗法锐减偏头痛发作频率

**原文标题**: From blood sugar to brain relief: GLP-1 therapy slashes migraine frequency

**原文链接**: [https://www.medlink.com/news/from-blood-sugar-to-brain-relief-glp-1-therapy-slashes-migraine-frequency](https://www.medlink.com/news/from-blood-sugar-to-brain-relief-glp-1-therapy-slashes-migraine-frequency)

根据在美国头痛学会年会上发布的新研究，GLP-1受体激动剂疗法（最初用于治疗2型糖尿病和肥胖症）在减少偏头痛发作频率方面显示出巨大潜力。

一项分析了152名偏头痛患者的回顾性研究（其中90名正在服用司美格鲁肽或利拉鲁肽等GLP-1激动剂）发现，接受GLP-1疗法的患者在三个月后，月偏头痛天数（MMD）减少了44%。平均MMD从10.8天降至6.3天。慢性偏头痛患者的MMD降幅更大，达到61.5%。近8%的GLP-1使用者实现了MMD的100%减少，从而完全摆脱了偏头痛。

另一项针对50名患者的较小规模回顾性研究也报告了MMD和头痛天数减少了50%，同时头痛强度和持续时间也得到改善。

这种作用机制尚未完全阐明，但可能涉及GLP-1激动剂的抗炎特性、其对体重减轻、血糖调节以及潜在的神经保护作用。已知这些药物能减少全身炎症和氧化应激，而这些都被认为与偏头痛的病理生理学有关。

尽管这些真实世界研究是回顾性和观察性的，表明存在强烈的相关性，但它们突显了偏头痛预防的一个潜在新治疗途径。需要进一步的前瞻性、随机对照试验来证实这些发现并阐明精确的作用机制。

---

## 81. 计算机和视频显示器故障排除与维修笔记

**原文标题**: Notes on the Troubleshooting and Repair of Computer and Video Monitors

**原文链接**: [https://www.repairfaq.org/sam/monfaq.htm](https://www.repairfaq.org/sam/monfaq.htm)

Samuel M. Goldwasser 撰写的《电脑和视频显示器故障排除与维修笔记》（3.22版，2009年）是一本关于诊断和维修基于CRT（阴极射线管）显示器的综合指南。它首先强调了重要的安全预防措施，特别是关于高压和CRT内爆的风险，然后概述了显示器的基本原理、特性和子系统。

该文档系统地涵盖了故障排除，按显示器组件对问题进行分类：低压电源（例如，显示器无电源、保险丝问题）、偏转电路（例如，尺寸、位置、同步问题、行输出晶体管故障）、高压电源（例如，无高压、电弧、聚焦问题）以及光栅/色彩/视频（例如，黑屏、色彩不平衡、回扫线、聚焦不良）。它提供了各种内部调整的详细说明，包括聚焦、纯度、会聚和几何校正。

文中提供了关于预防性维护、测试设备、电容器放电以及安全拆开显示器的实用建议。还讨论了各种杂项问题，例如干扰、省电问题、物理损坏以及特定显示器型号的怪癖。该指南最后附有大量“感兴趣的条目”，涵盖了显示器规格、视频标准、使用寿命、屏幕老化（烧屏）预防，以及“服务信息”，包括原理图、零件和高级故障排除的资源，使其成为显示器维修的宝贵资源。

---

## 82. 麻省理工研究：AI可取代11.7%美国劳动力

**原文标题**: MIT study finds AI can replace 11.7% of U.S. workforce

**原文链接**: [https://www.cnbc.com/2025/11/26/mit-study-finds-ai-can-already-replace-11point7percent-of-us-workforce.html](https://www.cnbc.com/2025/11/26/mit-study-finds-ai-can-already-replace-11point7percent-of-us-workforce.html)

麻省理工学院与橡树岭国家实验室联合开展的一项研究揭示，人工智能已能取代美国11.7%的劳动力，相当于金融、医疗保健和专业服务等领域约1.2万亿美元的工资。

该研究利用了一个名为“冰山指数”（Iceberg Index）的复杂劳动力模拟工具，该工具是美国劳动力市场的“数字孪生”。它绘制了覆盖923个职业、3000个县的1.51亿名工人，并识别出当前人工智能系统能够执行的特定技能。

该研究区分了冰山的“可见尖端”——与科技相关的裁员（占工资暴露度的2.2%，即2110亿美元）——以及更庞大的总暴露度（11.7%，即1.2万亿美元），后者包含了人力资源、物流、金融和办公室行政等领域常被忽视的日常职能。

“冰山指数”并非失业预测引擎，而是一个以技能为中心的快照，旨在帮助政策制定者主动探索“假设情景”。它提供了精确到邮政编码的潜在颠覆的详细地图，使各州能够在投入大量资源之前测试干预措施并优先考虑再培训投资。

至关重要的是，该指数挑战了人工智能风险仅限于沿海科技中心的假设，表明受影响的职业遍布全美50个州，包括内陆和农村地区。田纳西州、北卡罗来纳州和犹他州等州已与研究人员合作，利用互动模拟环境来制定和验证其人工智能劳动力行动计划。该工具使政策制定者能够识别风险热点、量身定制培训项目，并了解人工智能对当地就业和GDP的潜在影响。

---

## 83. 欧盟理事会就聊天管控达成立场

**原文标题**: EU council reaches position on Chat Control

**原文链接**: [https://www.consilium.europa.eu/de/press/press-releases/2025/11/26/child-sexual-abuse-council-reaches-position-on-law-protecting-children-from-online-abuse/](https://www.consilium.europa.eu/de/press/press-releases/2025/11/26/child-sexual-abuse-council-reaches-position-on-law-protecting-children-from-online-abuse/)

欧盟理事会于2024年6月20日通过了其关于一项旨在预防和打击网络儿童性虐待（CSA）的拟议法规的谈判立场（即“总体方针”）。其目标是加强儿童保护并确保肇事者受到起诉。

理事会立场的重点是“定向检测令”（TDOs）。这些命令由国家司法或行政机关发布，强制特定的托管或人际通信服务提供商检测已知的儿童性虐待材料（CSAM）（通过哈希匹配），并在严格的条件下检测新的CSAM。至关重要的是，这些TDOs并非用于普遍监控私人通信，而是针对上传者和初始分发者，重点关注被认为传播新CSAM高风险的服务。

其中内置了重要的隐私和数据保护保障措施。理事会的立场明确指出，TDOs不能强制扫描端到端加密通信，也不能要求服务提供商削弱加密。某些敏感服务，例如医疗保健在线聊天，也被排除在新CSAM检测范围之外。

服务提供商必须向新成立的欧盟儿童性虐待中心或国家机构报告检测到的材料。该法规还涵盖对CSA内容和诱骗行为的审核。该协议使得理事会能够与欧洲议会和欧盟委员会启动“三方对话”谈判，以最终确定立法。

---

## 84. OpenAI 需要在2030年前筹集2070亿美元，才能继续亏损。

**原文标题**: OpenAI needs to raise $207B by 2030 so it can continue to lose money

**原文链接**: [https://www.ft.com/content/23e54a28-6f63-4533-ab96-3756d9c88bad](https://www.ft.com/content/23e54a28-6f63-4533-ab96-3756d9c88bad)

The provided text is primarily a paywall for an FT Alphaville article, offering various subscription options to access its content.

The core information visible, taken from the title and a snippet of the article, states that **OpenAI needs to raise at least $207 billion by 2030**. This substantial fundraising is estimated by **HSBC**, and its purpose is to enable the company to **continue covering its financial losses**. The details and analysis supporting this estimate are locked behind the FT Alphaville paywall.

---

## 85. The Bughouse Effect

**原文标题**: The Bughouse Effect

**原文链接**: [https://tsvibt.blogspot.com/2025/11/the-bughouse-effect.html](https://tsvibt.blogspot.com/2025/11/the-bughouse-effect.html)

生成摘要时出错

---

## 86. Why I (Still) Love Linux ?

**原文标题**: Why I (Still) Love Linux ?

**原文链接**: [https://it-notes.dragas.net/2025/11/24/why-i-still-love-linux/](https://it-notes.dragas.net/2025/11/24/why-i-still-love-linux/)

生成摘要时出错

---

## 87. Slashdot effect

**原文标题**: Slashdot effect

**原文链接**: [https://en.wikipedia.org/wiki/Slashdot_effect](https://en.wikipedia.org/wiki/Slashdot_effect)

生成摘要时出错

---

## 88. Space: 1999 – Special Effects Techniques

**原文标题**: Space: 1999 – Special Effects Techniques

**原文链接**: [https://catacombs.space1999.net/main/pguide/upsfx.html](https://catacombs.space1999.net/main/pguide/upsfx.html)

生成摘要时出错

---

## 89. GrapheneOS is leaving France after receiving threats from law enforcement

**原文标题**: GrapheneOS is leaving France after receiving threats from law enforcement

**原文链接**: [https://grapheneos.social/@GrapheneOS/115606319562587450](https://grapheneos.social/@GrapheneOS/115606319562587450)

生成摘要时出错

---

## 90. Meta Execs Privately Compared Instagram to Addictive Drug, Court Filing Shows

**原文标题**: Meta Execs Privately Compared Instagram to Addictive Drug, Court Filing Shows

**原文链接**: [https://www.nationalreview.com/news/meta-researchers-privately-compared-instagram-to-addictive-drug-bombshell-court-filing-shows/](https://www.nationalreview.com/news/meta-researchers-privately-compared-instagram-to-addictive-drug-bombshell-court-filing-shows/)

生成摘要时出错

---

## 91. New report calls for end to child marriage in the US

**原文标题**: New report calls for end to child marriage in the US

**原文链接**: [https://womensmediacenter.com/news-features/new-report-calls-for-end-to-child-marriage-in-us](https://womensmediacenter.com/news-features/new-report-calls-for-end-to-child-marriage-in-us)

生成摘要时出错

---

## 92. Launch HN: Karumi (YC F25) – Personalized, agentic product demos

**原文标题**: Launch HN: Karumi (YC F25) – Personalized, agentic product demos

**原文链接**: [http://karumi.ai/](http://karumi.ai/)

生成摘要时出错

---

## 93. Investors expect AI use to soar. That's not happening

**原文标题**: Investors expect AI use to soar. That's not happening

**原文链接**: [https://www.economist.com/finance-and-economics/2025/11/26/investors-expect-ai-use-to-soar-thats-not-happening](https://www.economist.com/finance-and-economics/2025/11/26/investors-expect-ai-use-to-soar-thats-not-happening)

生成摘要时出错

---

## 94. More Americans are getting their power shut off, as unpaid bills pile up

**原文标题**: More Americans are getting their power shut off, as unpaid bills pile up

**原文链接**: [https://www.washingtonpost.com/business/2025/11/24/power-shutoffs-surge-electric-bills/](https://www.washingtonpost.com/business/2025/11/24/power-shutoffs-surge-electric-bills/)

生成摘要时出错

---

## 95. Slop Detective – Fight the Slop Syndicate

**原文标题**: Slop Detective – Fight the Slop Syndicate

**原文链接**: [https://slopdetective.kagi.com/](https://slopdetective.kagi.com/)

生成摘要时出错

---

## 96. Stop Telling Us XMPP Should Use JSON

**原文标题**: Stop Telling Us XMPP Should Use JSON

**原文链接**: [https://www.process-one.net/blog/stop-telling-us-xmpp-should-use-json/](https://www.process-one.net/blog/stop-telling-us-xmpp-should-use-json/)

生成摘要时出错

---

## 97. Google experts tell the US DOJ selling its ad tech business would be impossible

**原文标题**: Google experts tell the US DOJ selling its ad tech business would be impossible

**原文链接**: [https://www.androidcentral.com/apps-software/google-experts-tell-the-us-doj-selling-its-ad-tech-business-would-be-impossible](https://www.androidcentral.com/apps-software/google-experts-tell-the-us-doj-selling-its-ad-tech-business-would-be-impossible)

生成摘要时出错

---

## 98. One in two people in the US is affected by a neurological disease or disorder

**原文标题**: One in two people in the US is affected by a neurological disease or disorder

**原文链接**: [https://medicalxpress.com/news/2025-11-people-affected-neurological-disease-disorder.html](https://medicalxpress.com/news/2025-11-people-affected-neurological-disease-disorder.html)

生成摘要时出错

---

## 99. Modder who put Thomas the Tank Engine into Skyrim flips the bird at lawyers

**原文标题**: Modder who put Thomas the Tank Engine into Skyrim flips the bird at lawyers

**原文链接**: [https://www.gamesradar.com/games/the-elder-scrolls/modder-who-first-put-thomas-the-tank-engine-into-skyrim-flips-the-bird-at-the-lawyers-does-it-again-in-morrowind-i-fundamentally-do-not-view-toy-company-ceos-or-media-ceos-as-people/](https://www.gamesradar.com/games/the-elder-scrolls/modder-who-first-put-thomas-the-tank-engine-into-skyrim-flips-the-bird-at-the-lawyers-does-it-again-in-morrowind-i-fundamentally-do-not-view-toy-company-ceos-or-media-ceos-as-people/)

生成摘要时出错

---

## 100. UK intends to scrap jury trials for majority of court cases

**原文标题**: UK intends to scrap jury trials for majority of court cases

**原文链接**: [https://www.gbnews.com/politics/uk/david-lammy-scrap-jury-trials](https://www.gbnews.com/politics/uk/david-lammy-scrap-jury-trials)

生成摘要时出错

---

