# Hacker News 热门文章摘要 (2025-12-06)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 网飞收购华纳兄弟

**原文标题**: Netflix to Acquire Warner Bros

**原文链接**: [https://about.netflix.com/en/news/netflix-to-acquire-warner-bros](https://about.netflix.com/en/news/netflix-to-acquire-warner-bros)

无法访问文章链接。

---

## 2. Cloudflare 宕机了

**原文标题**: Cloudflare was down

**原文链接**: [https://www.cloudflare.com/](https://www.cloudflare.com/)

Cloudflare推广其“连接云”，作为一个包含60多种全球云服务的统一平台，旨在为用户、应用程序和网络提供连接、保护和构建服务。凭借其智能全球网络，它提供了无与伦比的安全性、速度和可靠性。

该平台的核心功能包括：
1. **连接：**通过现代化网络并借助SASE（安全访问服务边缘）和零信任解决方案保护工作区，确保用户、应用程序和AI代理的安全访问。
2. **保护：**采用行业领先的WAF、DDoS和机器人防护，保护网站、应用程序、API和AI工作负载，同时通过其超高速CDN加速性能。
3. **构建：**提供一个强大的环境来开发和扩展应用程序，包括AI代理框架、无服务器代码部署和S3兼容对象存储，从而降低运营开销。

Cloudflare的全球网络遍布330多个城市，每天拦截高达2340亿次网络威胁，并保护全球20%的网站。领先企业信赖Cloudflare，因为它采用全面的方法来保护和加速其数字基础设施，从用户连接到AI部署。

---

## 3. Cloudflare 2025年12月5日故障

**原文标题**: Cloudflare outage on December 5, 2025

**原文链接**: [https://blog.cloudflare.com/5-december-2025-outage/](https://blog.cloudflare.com/5-december-2025-outage/)

2025年12月5日，Cloudflare遭遇了一次25分钟的服务中断，从UTC时间08:47持续至09:12，影响了其大约28%的HTTP流量。此次事件并非网络攻击，而是源于Cloudflare为缓解React服务器组件中新的行业性漏洞（CVE-2025-55182）而对其请求体解析逻辑所做的更改。

为保护客户，Cloudflare当时正在将其Web应用防火墙（WAF）的缓冲区大小从128KB提升至1MB。在此过程中，他们使用其全局配置系统禁用了内部WAF测试工具，该系统会即时传播更改，而非他们所使用的分阶段部署系统。这一针对其旧版FL1代理应用的第二项更改，触发了一个Lua异常：“尝试索引字段'execute'（一个空值）。”

当一个用于快速禁用异常规则的“快速禁用开关”（killswitch）首次应用于具有“execute”操作的规则时，发生了此错误。用Lua编写的代码预期即使在规则被跳过时，“rule_result.execute”对象也应存在，从而导致了空值错误。这个长期未被发现的错误凸显了该语言类型系统的弱点，而此问题已在其新的基于Rust的FL2代理中得到解决。

Cloudflare承认了此次事件带来的失望，尤其是这已是数周内（继11月18日之后）因配置更改导致的第二次重大中断。他们重申正在持续努力改进发布流程、简化“紧急破窗”机制以及实现“故障开放”错误处理，这些措施仍在部署中。该更改已于UTC时间09:12回滚，所有服务均已恢复。Cloudflare对此次反复给客户和互联网造成的影响表示歉意。

---

## 4. Gemini 3 Pro：视觉 AI 的前沿

**原文标题**: Gemini 3 Pro: the frontier of vision AI

**原文链接**: [https://blog.google/technology/developers/gemini-3-pro-vision/](https://blog.google/technology/developers/gemini-3-pro-vision/)

Gemini 3 Pro 于2025年12月5日推出，是谷歌迄今为止能力最强的多模态模型，标志着视觉AI领域的代际飞跃。它在文档理解、空间理解、屏幕理解和视频理解方面均实现了最先进的性能，树立了新的基准。

在文档理解方面，Gemini 3 Pro 在光学字符识别 (OCR) 方面表现出色，能将视觉文档“反渲染”为结构化代码 (HTML、LaTeX)，并对复杂表格和图表进行精密的、多步骤的推理，甚至在CharXiv推理基准测试中超越了人类基线。

对于空间理解，它提供像素级精确的指向能力和开放词汇参照，赋能机器人技术和AR/XR应用。其强大的屏幕理解能力有助于实现计算机使用代理，用于自动化任务、质量保证 (QA) 测试和用户体验 (UX) 分析。

在视频理解方面，Gemini 3 Pro 取得了重大进展，支持高帧率 (高于1 FPS) 以捕捉快速动作，并具有升级的“思考”模式，能够追溯复杂的因果关系。它还可以将长视频中的洞察转化为功能性应用程序或结构化代码。

实际应用场景多种多样，包括教育（解决大量图表的难题）、医疗和生物医学成像（在专家级基准测试中取得最先进成果），以及法律和金融（分析密集型报告）。

开发者通过新的 `media_resolution` 参数获得对性能和成本的细粒度控制，使他们能够权衡视觉保真度与资源消耗。谷歌鼓励开发者通过其文档或Google AI Studio探索Gemini 3 Pro。

---

## 5. 网飞的AV1之旅：从安卓到电视及更远

**原文标题**: Netflix’s AV1 Journey: From Android to TVs and Beyond

**原文链接**: [https://netflixtechblog.com/av1-now-powering-30-of-netflix-streaming-02f592242d80](https://netflixtechblog.com/av1-now-powering-30-of-netflix-streaming-02f592242d80)

Netflix 的 AV1 之旅：从安卓到电视及更远

Netflix 大幅扩展了 AV1 的使用，这种先进的视频编解码器目前已支持其全球流媒体播放量的 30%。AV1 最初于 2020 年在 Android 上推出，以其卓越的压缩效率而闻名，相比于 AVC 或 HEVC 等老一代编解码器，它能以显著更低的比特率提供相同或更优的视频质量。

此次扩展主要得益于 AV1 硬件解码器在智能电视、游戏主机（如 PS4 Pro 和 Xbox Series X/S）以及其他客厅设备中的日益普及。硬件解码对这些平台至关重要，能帮助它们处理 AV1 的复杂性，同时不影响电池续航或设备性能。Netflix 与合作伙伴紧密合作，以实现 AV1 播放，确保流畅的用户体验。

其益处是巨大的：用户，特别是那些网络连接较慢或有数据限制的用户，能够体验到更少的缓冲、更快的启动速度以及整体更高质量的流媒体内容。对于 Netflix 而言，AV1 使他们能够更高效地提供更多时长的内容，包括更高分辨率和 HDR 内容。文章强调了一种“以设备为中心”的部署策略，优先考虑那些 AV1 能提供最大用户效益且硬件支持强大的平台。这一持续的旅程凸显了 Netflix 致力于利用尖端技术，以提升全球观众体验的承诺。

---

## 6. Go、Rust、Zig 对比之我见

**原文标题**: Thoughts on Go vs. Rust vs. Zig

**原文链接**: [https://sinclairtarget.com/blog/2025/08/thoughts-on-go-vs.-rust-vs.-zig/](https://sinclairtarget.com/blog/2025/08/thoughts-on-go-vs.-rust-vs.-zig/)

作者通过分析 Go、Rust 和 Zig 底层的价值观和权衡，比较了这三种语言，旨在理解它们各自的哲学理念，而不仅仅是特性列表。

**Go** 以其极简主义而受到赞扬，被描述为“现代 C 语言”。它优先考虑稳定性，易于阅读，特别是对于并发代码和企业协作而言。它对新特性（如泛型）设置了很高的门槛，这导致了一些样板代码，但确保了语言的简洁性和可预测性，在其中内存是隐式管理的（例如，切片无需用户明确干预即可处理增长和分配）。

**Rust** 被视为一种极致主义语言，专注于“零成本抽象”，以实现安全性和性能。它的复杂性源于其密集的概念体系，包括富有表现力的类型系统和大量的 trait，这些对于编译器在编译时防止内存不安全和未定义行为（UB）至关重要。这种学习曲线带来了代码正确性和可靠性的强大保证。

**Zig** 作为最新语言，通过强调显式控制来回应 Go 和 Rust。它采用手动内存管理，要求用户选择分配器并管理每一个字节。Zig 避开了传统的面向对象编程（OOP）特性，如私有字段和动态分派，提倡数据导向设计，并鼓励基于大块的内存分配，而不是与单个对象绑定的分配（RAII）。尽管它在运行时检测“非法行为”，但在发布模式下可以禁用性能检查，这提供了一种务实的安全方法。

---

## 7. 改写欧盟人权与气候法的美国污染者

**原文标题**: The US polluters that are rewriting the EU's human rights and climate law

**原文链接**: [https://www.somo.nl/the-secretive-cabal-of-us-polluters-that-is-rewriting-the-eus-human-rights-and-climate-law/](https://www.somo.nl/the-secretive-cabal-of-us-polluters-that-is-rewriting-the-eus-human-rights-and-climate-law/)

SOMO的文章《重写欧盟人权和气候法的美国污染者》揭露了美国行业团体联盟，其中包括美国商会、全国制造商协会（NAM）和美国石油学会（API），正积极游说以削弱欧盟雄心勃勃的人权和环境立法。

这些团体代表石油、天然气、化工和制造业等行业，正针对欧盟的关键倡议，例如《企业可持续发展尽职调查指令》（CSDDD）、《绿色声明指令》和强制劳动禁令。他们的策略包括广泛游说、直接接触欧盟官员以及公共宣传活动，常将欧盟法规框定为对全球贸易和竞争力的威胁。

文章详细阐述了具体案例，例如美国商会干预并影响了CSDDD的范围和执行机制，以及全国制造商协会（NAM）努力拖延或稀释绿色声明法规。这些行动被视为企图削弱欧盟在制定企业问责制和环境保护全球标准方面的领导地位，可能在国际贸易担忧的幌子下，让有害做法得以持续。文章指出，其最终目标是保护美国企业利益，使其免受日益增加的监管负担，并维持在欧盟新法下可能被视为不可持续或剥削性的现有商业模式。

---

## 8. 宝马PHEV：安全保险丝更换极其昂贵

**原文标题**: BMW PHEV: Safety fuse replacement is extremely expensive

**原文链接**: [https://evclinic.eu/2025/12/04/2021-phev-bmw-ibmucp-21f37e-post-crash-recovery-when-eu-engineering-becomes-a-synonym-for-unrepairable-generating-waste/](https://evclinic.eu/2025/12/04/2021-phev-bmw-ibmucp-21f37e-post-crash-recovery-when-eu-engineering-becomes-a-synonym-for-unrepairable-generating-waste/)

2021款宝马插电混动车（X5 45e G05）遭遇了一次轻微追尾事故，尽管物理损伤极小，但却触发了其高压系统安全熔断器（烟火式保险丝），导致车辆无法运行。本文着重指出宝马针对此特定问题采取的一项惊人昂贵且环境浪费的维修政策。

宝马的官方维修规程并未允许简单廉价地更换烧断的烟火式保险丝，而是强制要求更换整个电源分配单元（PDU，亦称“高压部件接线盒”），以及其集成的线束和其他相关组件。这项政策将一次本应是小修的问题，升级为轻微刮蹭事故就需支付约24,000欧元的惊人维修费用。

如此高昂的成本往往超出车辆的残值，导致车辆在其他状况良好的情况下，仍被保险公司宣布为“全损”。这种做法受到了严厉批评，被视为“反维修”工程的一个恶劣典范，它产生了大量的电子垃圾，迫使功能完好的汽车过早报废。作者将此与梅赛德斯等其他制造商进行对比，后者提供烟火式保险丝的直接更换，并指出宝马的设计是蓄意设置的维修障碍，损害了“维修权”，并助长了汽车行业不可持续的做法。

---

## 9. 大多数技术问题都是人为问题

**原文标题**: Most technical problems are people problems

**原文链接**: [https://blog.joeschrag.com/2023/11/most-technical-problems-are-really.html](https://blog.joeschrag.com/2023/11/most-technical-problems-are-really.html)

文章指出，大多数技术问题本质上都是“人的问题”。作者通过他在一家背负巨额技术债和代码重复的公司的工作经验来阐述这一点。他最初尝试纯粹从技术层面解决问题，但失败了，因为他意识到这种做法忽视了更深层次的人为因素。

技术债、不切实际的截止日期或过时的技术选择，往往源于开发者对改变的抵触、过时的技能、自负、糟糕的沟通或被动式管理。承认需要重构可能意味着要面对系统性故障和技能缺陷。作者指出，如果不能解决导致技术债持续存在的人为因素（例如，不愿学习新事物），那么清理技术债的速度就无法超过其产生速度。

文章挑战了工程师在真空中解决问题的理想，强调忽视“政治”和非技术利益相关者是有害的。有效沟通至关重要；技术工作的价值，尤其是技术债清理的价值，必须量化并转化为商业价值，以便非技术领导层理解。

最终，作者总结道，高级职位不仅仅需要技术专长。它们还需要强大的跨职能协作能力、处理人际关系和自我的能力，以及识别更广泛项目风险的预见性。这种兼顾技术深度、人际交往能力和战略意识的“抬头看代码者”被认为对大型项目至关重要，与纯粹专注于技术的“工程师中的工程师”形成对比。

---

## 10. 精神分裂症患者误把智能冰箱广告当成精神病发作

**原文标题**: Schizophrenia sufferer mistakes smart fridge ad for psychotic episode

**原文链接**: [https://old.reddit.com/r/LegalAdviceUK/comments/1pc7999/my_schizophrenic_sister_hospitalised_herself/](https://old.reddit.com/r/LegalAdviceUK/comments/1pc7999/my_schizophrenic_sister_hospitalised_herself/)

一位Reddit用户在LegalAdviceUK版块发帖称，其三十多岁、病情稳定、患有偏执型精神分裂症的妹妹在观看一则YouTube广告后，遭遇了严重的精神病发作。这则为AO.com智能冰箱制作的广告中，冰箱直接与她对话并直呼其名，据推测，这利用了她Google账户中的个性化数据。

这种高度个性化和互动性强的广告引发了她严重的精神崩溃。这位妹妹确信冰箱是真实的，正在观察她、侵犯她的隐私并监视她的思想，这导致了强烈的偏执、妄想和幻觉。她此前一直独立生活并很好地控制着病情，但在此事后自行住院，现在病情严重，可能需要长期护理，并且病情恢复出现严重倒退。

这家人痛心疾首，认为这则广告不负责任且疏忽大意，特别是考虑到AI驱动的个性化定制功能能够创造出如此真实且可能造成痛苦的体验。他们正在寻求法律咨询，以了解AO.com或YouTube/Google是否应对所造成的伤害负责，他们认为直接互动和个性化广告，尤其是那些模拟感知能力或直呼其名的广告，应该附带警告或受到限制，以保护弱势群体。

---

## 11. 我们给5个LLM 10万美元，让它们交易股票8个月。

**原文标题**: We gave 5 LLMs $100K to trade stocks for 8 months

**原文链接**: [https://www.aitradearena.com/research/we-ran-llms-for-8-months](https://www.aitradearena.com/research/we-ran-llms-for-8-months)

这篇文章题为《我们向5个LLM提供10万美元进行8个月的股票交易》，介绍了一个名为“AI交易竞技场”的雄心勃勃的项目。其核心前提是建立一个实验性环境，其中五个不同的大型语言模型（LLM）各自被分配了高达10万美元的资金。这些AI代理被赋予了在股票市场自主交易的任务，为期八个月。

这项倡议旨在评估先进AI模型在真实世界股票市场交易这一动态而复杂的环境中的表现和能力。在没有文章全文的情况下，关于所采用的方法论、所选的具体LLM、所使用的投资策略，或者，最重要的是，它们的实际交易表现结果（例如盈利、亏损、与人类基准或传统算法的对比分析）无法提供。仅从标题来看，这表明了对AI在金融管理和投资方面潜力进行了深入探索。

---

## 12. 内存短缺无人能幸免

**原文标题**: The RAM shortage comes for us all

**原文链接**: [https://www.jeffgeerling.com/blog/2025/ram-shortage-comes-us-all](https://www.jeffgeerling.com/blog/2025/ram-shortage-comes-us-all)

文章指出，全球内存（RAM）短缺日益恶化和价格严重通胀，影响了几乎所有科技行业。作者提到DDR5内存价格在几个月内翻了三倍的个人经历，而树莓派（Raspberry Pi）、Libre Computer及其他小型供应商因内存成本飙升被迫提价。美光（Micron）甚至停产了其Crucial品牌，进一步减少了消费者的选择。

主要原因是人工智能（AI）数据中心的大规模建设。内存制造商优先为AI产品生产高利润、专用内存（如HBM），忽视了消费市场，甚至关闭了消费级生产线。这种资源转移导致PC组装商、单板计算机（SBC）制造商的供应紧张，最终也会影响相机、游戏机和平板电脑等设备。

与过去的科技泡沫不同，潜在的AI“泡沫破裂”不太可能让廉价消费硬件充斥市场，因为许多AI专用内存和集成系统与标准PC不兼容。大型企业囤积内存进一步加剧了这种情况，类似于2020年的卫生纸短缺，从而延长了危机。小型公司面临艰难选择：提价、停止生产或搜寻内存芯片。作者以悲观的预测作结，认为PC组装爱好可能会“名存实亡”，并建议专注于现有项目而非新的购买，因为这种AI驱动的内存“税”将持续多久尚不明确。

---

## 13. Django 6

**原文标题**: Django 6

**原文链接**: [https://docs.djangoproject.com/en/6.0/releases/6.0/](https://docs.djangoproject.com/en/6.0/releases/6.0/)

Django 6.0 于 2025 年 12 月 3 日发布，引入了大量新特性，以及向后不兼容的更改和弃用。它正式支持 Python 3.12、3.13 和 3.14，不再兼容 Python 3.10 和 3.11。

主要新特性包括：
*   **内容安全策略 (CSP) 支持：** 内置工具允许通过中间件和设置强制执行或监控 CSP 策略，增强对内容注入攻击的保护。
*   **模板片段：** Django 模板语言现在支持 `{% partialdef %}` 和 `{% partial %}` 标签，使得模板片段的封装和复用无需单独文件，更为便捷。
*   **后台任务框架：** 一个内置系统，用于定义、验证、排队和处理 HTTP 请求-响应周期之外的任务，适用于卸载诸如发送电子邮件等工作。
*   **采用现代电子邮件 API：** Django 的电子邮件处理现在使用 Python 的 `email.message.EmailMessage` API，以提供更清晰、对 Unicode 更友好的接口。

次要特性包括 `django.contrib.admin` 中引入 Font Awesome 6.7.2、增加 PBKDF2 迭代次数、新的 GIS 功能和对 MariaDB 12+ 的支持、`django.contrib.postgres` 中用于全文搜索的 `Lexeme`、适用于所有数据库的 `StringAgg`、`AsyncPaginator` 以及模板中的 `forloop.length`。

向后不兼容的更改包括弃用对 Python < 3.12 和 MariaDB 10.5 的支持。`DEFAULT_AUTO_FIELD` 现在默认为 `BigAutoField`。自定义 ORM 表达式的 `as_sql()` 方法现在必须以元组形式返回参数。数据库后端 API 也进行了方法重命名和与 `RETURNING` 语句相关的更改。

一个值得注意的弃用是，`django.core.mail` API（例如 `send_mail`、`mail_admins`）现在要求可选参数以关键字参数的形式传递，而使用位置参数将会发出弃用警告。

---

## 14. UniFi 5G

**原文标题**: UniFi 5G

**原文链接**: [https://blog.ui.com/article/introducing-unifi-5g](https://blog.ui.com/article/introducing-unifi-5g)

UniFi 5G Max 产品线旨在提供时尚、多功能且性能超群的 5G 互联网体验。其主要目标是确保在任何环境下都能轻松运行，并提供卓越且适应性强的 5G 连接。

---

## 15. YouTube被曝用AI编辑视频并添加误导性AI摘要

**原文标题**: YouTube caught making AI-edits to videos and adding misleading AI summaries

**原文链接**: [https://www.ynetnews.com/tech-and-digital/article/bj1qbwcklg](https://www.ynetnews.com/tech-and-digital/article/bj1qbwcklg)

YouTube一直在悄悄地试验人工智能，以增强热门创作者（包括Shorts短视频）的视频，而这些创作者及其观众均不知情或未经同意。拥有数百万订阅者的YouTube创作者Rick Beato和Rhett Shull首次注意到细微的人工智能修改，例如更清晰的衣物褶皱、更光滑的皮肤或略微改变的耳朵，这让他们感觉自己的视频“不自然”且“由人工智能生成”。Shull特别表达了对观众信任受损的担忧。

YouTube的创作者联络员Rene Ritchie证实了一项“小型实验”，该实验使用“传统机器学习”来澄清和提高视频清晰度，并将其比作智能手机的功能。然而，虚假信息专家Samuel Woolley对此提出批评，他澄清说机器学习是人工智能的一个子集，因此YouTube的措辞具有误导性。

这种做法引发了人们对真实性和媒体操纵的重大担忧。Woolley强调，未经同意擅自修改和分发内容，会在观众和他们所消费的媒体之间增加一个“隐藏层”，这与用户主动应用的滤镜形成对比。尽管Beato对YouTube的创新保持乐观，但批评者警告说，即使是微小且未披露的修饰，也开创了一个令人不安的先例，特别是对于准确性至关重要的新闻、教育和信息内容。这一事件预示着未来人工智能将越来越多地在用户接触数字媒体之前对其进行预处理和重塑。

---

## 16. 诱骗用户，绕过警告 – 现代 SVG 点击劫持攻击

**原文标题**: Trick users and bypass warnings – Modern SVG Clickjacking attacks

**原文链接**: [https://lyra.horse/blog/2025/12/svg-clickjacking/](https://lyra.horse/blog/2025/12/svg-clickjacking/)

本文介绍了一种“SVG点击劫持”的新型技术，它通过实现复杂的交互场景和数据窃取，显著增强了传统的点击劫持攻击。与经典方法不同，这种方法利用了SVG滤镜（例如`feColorMatrix`、`feDisplacementMap`），这些滤镜意外地应用于跨源iframe。

作者演示了几种利用各种`fe*` SVG元素构建的攻击原语：
1.  **伪造验证码：** 利用`feDisplacementMap`扭曲iframe文本，诱骗用户重新输入敏感信息，从而实现数据窃取。
2.  **灰色文本隐藏：** 结合使用`feComposite`、`feTile`、`feMorphology`、`feFlood`、`feBlend`和`feColorMatrix`，遮盖输入字段中的占位符或警告文本。这使得攻击者能够在保持功能性的同时，重新构建输入的上下文。
3.  **像素读取：** 这是最强大的原语，能够实现响应式攻击。它涉及使用`feTile`裁剪一个像素，用`feComposite`将其颜色二值化，并通过`feColorMatrix`将其转换为alpha蒙版，以切换其他滤镜（例如`feGaussianBlur`）。这有助于实现动态元素，如悬停效果或虚假表单验证。
4.  **逻辑门：** 通过使用`feBlend`和`feComposite`，所有逻辑门（与、或、非、异或）都可以被重新创建，使SVG滤镜“功能完备”。这使得可以在滤镜链中直接编程任意复杂的逻辑电路，从而导致高度复杂和具有说服力的攻击。

这项技术绕过了传统点击劫持的局限性，创建了以前被认为不现实的交互式欺骗，尽管它目前与Safari存在兼容性问题。

---

## 17. 肯尼亚法院裁定禁止种子共享的法律违宪

**原文标题**: Kenyan court declares law banning seed sharing unconstitutional

**原文链接**: [https://apnews.com/article/kenya-seed-sharing-law-ruling-ad4df5a364299b3a9f8515c0f52d5f80](https://apnews.com/article/kenya-seed-sharing-law-ruling-ad4df5a364299b3a9f8515c0f52d5f80)

肯尼亚高等法院宣布，2012年种子法中将农民分享和出售本土种子定为犯罪的部分条款违宪，这一裁决被誉为粮食安全的里程碑式胜利。

罗达·鲁托法官的裁决意味着，农民将不再因通过社区种子银行分享种子而面临最高两年监禁或100万肯尼亚先令（约合7700美元）的罚款。被废止的条款也曾赋予政府官员突击搜查这些银行并没收种子的权力。该法律最初旨在打击假冒伪劣种子，并赋予持牌公司独家贸易权。

此案由15名小农户提起，他们对传统做法如今得到昭雪感到欣慰。农民塞缪尔·瓦索姆指出：“我祖母保存种子，今天法院说我也可以这样做……不必害怕。”

绿色和平非洲的伊丽莎白·阿蒂耶诺称其为“我们文化、韧性和未来的胜利”，她表示法院打击了对粮食系统的“企业掌控”。本土种子因其抗旱性和对当地气候的适应性而备受倡导者推崇，它们常常优于杂交品种，这对于雨养农业地区的粮食安全至关重要。尽管肯尼亚过去曾面临假冒伪劣种子的挑战，社区种子银行与国家种子银行一道，被视为保存多样性和可获取性的关键。

---

## 18. 离开英特尔

**原文标题**: Leaving Intel

**原文链接**: [https://www.brendangregg.com/blog//2025-12-05/leaving-intel.html](https://www.brendangregg.com/blog//2025-12-05/leaving-intel.html)

作者宣布在英特尔工作3.5年后辞职，以寻求新的发展机遇，并总结了在公司面临挑战时期所做的主要贡献。

他们的成就包括开发并开源了AI火焰图（目前尚未广泛采用）和GPU亚秒偏移热图，支持Linux发行版进行堆栈遍历，并就eBPF接受了《华尔街日报》的采访。他们还在eBPF技术指导委员会中担任领导职务，共同主持了2023年USENIX SREcon亚太会议，并发表了六场会议主题演讲。

在云计算领域，作者投入了大量精力，召开了110次客户会议，并制定了包含33项具体建议的公司层面云战略，其中呈现了独特的团队协作可视化图。这项被作者认为是其最佳工作的战略是公司内部文件，但可供英特尔继续执行。

作者分享了一些美好的回忆，包括与Linus Torvalds、Pat Gelsinger和Harshad Sane的会面。他们承认了任职期间的艰难背景（英特尔最艰难的三年以及招聘冻结），对自己的贡献表示满意，并祝愿英特尔在实施他们留下的复杂建议方面一切顺利。

---

## 19. Framework 笔记本 13 通过升级套件搭载 12 核 ARM 处理器

**原文标题**: Framework Laptop 13 gets ARM processor with 12 cores via upgrade kit

**原文链接**: [https://www.notebookcheck.net/Framework-Laptop-13-gets-ARM-processor-with-12-cores-via-upgrade-kit.1177930.0.html](https://www.notebookcheck.net/Framework-Laptop-13-gets-ARM-processor-with-12-cores-via-upgrade-kit.1177930.0.html)

MetaComputing 为 Framework Laptop 13 推出了一款 ARM 主板升级套件，为英特尔、AMD 和骁龙 X 处理器提供了一种替代方案。该主板配备 CIX CP8180 ARM 芯片组，拥有 12 个核心：八个 Cortex-A720 性能核心（其中两个可提升至 2.6 GHz）和四个 Cortex-A520 能效核心。它还集成了 10 核 ARM Immortalis-G720 GPU 和一个 30 TOPS 的 AI 加速器。

尽管可能比骁龙 X Elite 慢，但这款芯片组应能处理日常任务。然而，一个显著缺点是其高达 16 瓦的空闲功耗，这意味着搭配 Framework Laptop 13 的 55 瓦时电池，续航时间会很短，使其主要吸引开发者。

“MetaComputing ARM AI PC 套件”现已上市。基础型号包含 16GB 内存、1TB SSD 和一个迷你 PC 机箱，售价 549 美元。用户可以将其主板安装到现有的 Framework Laptop 13 中，或者以 999 美元的价格购买包含笔记本电脑的捆绑包。升级到 32GB 内存需额外支付 100 美元。全球免费送货，但进口关税和税费不包含在内。

---

## 20. Rust 防御性编程模式

**原文标题**: Patterns for Defensive Programming in Rust

**原文链接**: [https://corrode.dev/blog/defensive-programming/](https://corrode.dev/blog/defensive-programming/)

本文探讨了 Rust 中的“代码异味”和防御性编程模式，以防止 Bug，即使该语言提供了强大的内存安全保障。核心主题是利用编译器来强制执行不变性。

关键防御模式及其动机：

1.  **避免直接的向量索引 (`vec[0]`)**：与其使用 `if !vec.is_empty() { vec[0] }`，不如使用切片模式匹配 (`match vec.as_slice() { [] => ..., [elem] => ..., _ => ... }`)。这强制处理空和多元素情况，使不变性变得明确。
2.  **明确使用 `Default`**：避免使用 `..Default::default()`，因为它可能隐藏新字段。要么明确列出所有字段，要么解构 `Default` (`let Foo { field1, field2, .. } = Foo::default();`)，以清楚地显示哪些是默认的，哪些是自定义的，并启用编译器对新字段的检查。
3.  **防御性特征实现（例如 `PartialEq`）**：对于 `PartialEq` 或 `Hash` 等特征，完整解构 `self` 和 `other` (`let Self { field1, field2, ignored: _, .. } = self;`)。这可确保添加新结构体字段时会导致编译错误，从而强制开发人员明确决定新字段是否影响特征逻辑。
4.  **对可能失败的转换使用 `TryFrom`**：如果转换可能失败或需要默认回退（例如 `unwrap_or_else`），则应实现 `TryFrom`，使潜在的失败对调用者明确可见。
5.  **避免非穷尽的 `match` 捕获所有情况 (`_ => {}`)**：在 `match` 语句中明确列出所有枚举变体。这利用编译器在新变体添加时发出警告，确保它们得到处理。
6.  **使用描述性的 `_` 占位符**：对于模式中未使用的变量，使用 `field_name: _` 而不是简单的 `_`，以提高可读性并明确被忽略的内容。
7.  **临时可变性**：通过用不可变变量遮蔽可变变量 (`let data = data;`) 或使用作用域块进行初始化 (`let data = { let mut data = ...; data }`) 来限制可变范围。这可以防止意外修改。
8.  **防御性构造器（用于库）**：为了在构造器中强制执行验证逻辑：
    *   添加一个私有字段 `_private: ()` 或使用 `#[non_exhaustive]` 来防止在模块/crate外部直接通过结构体字面量构造实例。
    *   为了最强的强制性，即使在同一模块内，也可以使用带有私有“密封”类型的嵌套私有模块，以确保 `new()` 是创建实例的*唯一*方式。将字段设为私有并提供获取器以防止直接修改。

---

## 21. 萨姆·奥特曼的DRAM交易

**原文标题**: Sam Altman’s DRAM Deal

**原文链接**: [https://www.mooreslawisdead.com/post/sam-altman-s-dirty-dram-deal](https://www.mooreslawisdead.com/post/sam-altman-s-dirty-dram-deal)

最近一篇文章揭示，DDR5内存价格在不到一个月内飙升了惊人的156%，并将其归因于“萨姆·奥特曼的肮脏DRAM交易”和更广泛的AI泡沫。这种市场混乱源于三个协同作用的因素：OpenAI前所未有的举动、全行业的恐慌性购买以及全球DRAM安全库存的严重枯竭。

2025年10月1日，OpenAI通过与三星和SK海力士同步进行的交易，秘密获得了全球40%的DRAM供应。这种极端的保密性意味着制造商和行业竞争对手都未能预料到如此大规模、协调一致的收购。这一大胆举动立即引发了恐慌，竞争对手和原始设备制造商（OEM）担心被排除在外，纷纷争抢剩余的DRAM。

市场因缺乏安全库存而异常脆弱。持续的关税变化阻碍了大额订单，内存价格下跌促使人们延迟购买，而韩国公司担心美国的报复，已停止出售老旧的DRAM制造设备，从而消除了关键的供应缓冲。

“人为稀缺”的转折揭示，OpenAI购买的不是成品内存模组，而是裸晶圆，他们只是在囤积。作者认为，这是一种蓄意策略，旨在剥夺Anthropic、Meta和谷歌的Gemini 3等竞争对手的关键内存，从而保护OpenAI的市场领先地位。

后果是严重的：内存价格已经“爆炸式上涨”。固态硬盘（SSD）、小型预装电脑、Radeon GPU和Xbox“几乎要完蛋了”。英伟达GPU、笔记本电脑和手机未来将受到影响。PlayStation准备更充分，而CPU（不带散热器）可能因需求减少而降价。作者敦促消费者现在购买必要的硬件，并呼吁对OpenAI的财务行为进行更严格的审查。

---

## 22. 影响深远的草甘膦安全研究发表25年后遭撤回

**原文标题**: Influential study on glyphosate safety retracted 25 years after publication

**原文链接**: [https://www.lemonde.fr/en/environment/article/2025/12/03/influential-study-on-glyphosate-safety-retracted-25-years-after-publication_6748114_114.html](https://www.lemonde.fr/en/environment/article/2025/12/03/influential-study-on-glyphosate-safety-retracted-25-years-after-publication_6748114_114.html)

于2000年4月发表的一项关于草甘膦安全性的最具影响力的研究之一，在25年后被《监管毒理学与药理学》期刊撤回。该原始文章曾得出除草剂是安全的结论。

11月28日的撤回通知援引了“被认为会损害该文章及其结论的学术诚信的几个关键问题”。识别出的主要问题是“幽灵写作”，这是一种科学欺诈形式。八年前，在美国的法庭诉讼中，被称为“孟山都文件”的孟山都内部文件被公开。这些文件揭示，孟山都员工而非署名科学家（Gary M. Williams、Robert Kroes和Ian C. Munro）才是该研究的实际作者。

幽灵写作是指公司付费让研究人员在一项并非他们撰写的研究上署名。这种做法旨在通过制造出研究是由独立科学家而非公司员工撰写的假象，来提高支持产品安全性的研究结果的可信度。

---

## 23. 车牌被盯上了吗？——查看你的车牌是否正在被监控

**原文标题**: Have I been Flocked? – Check if your license plate is being watched

**原文链接**: [https://haveibeenflocked.com/](https://haveibeenflocked.com/)

无法访问文章链接。

---

## 24. 新冠mRNA疫苗接种与4年全因死亡率

**原文标题**: Covid-19 mRNA Vaccination and 4-Year All-Cause Mortality

**原文链接**: [https://jamanetwork.com/journals/jamanetworkopen/fullarticle/2842305](https://jamanetwork.com/journals/jamanetworkopen/fullarticle/2842305)

发表在《JAMA Network Open》上的这项研究，调查了在一个大型以色列队列中，mRNA新冠疫苗接种与四年期间全因死亡率之间的关联。研究人员进行了一项回顾性队列研究，涉及来自Maccabi Healthcare Services的200多万成年人，比较了至少接种了两剂mRNA疫苗（主要为BNT162b2）的个体与未接种疫苗的个体之间的全因死亡率。该分析控制了广泛的潜在混杂因素，包括年龄、性别、社会经济状况、现有合并症和既往SARS-CoV-2感染。

研究结果显示，在四年随访期间，mRNA新冠疫苗接种与全因死亡风险降低11%相关，相较于未接种疫苗的个体，接种疫苗者的调整后风险比为0.89（95% CI, 0.88-0.91）。尽管在疫苗接种后的前六个月观察到最显著的死亡率降低（aHR 0.77），但统计学上显著的益处在整个四年观察期内持续存在。此外，与仅接种两剂初级疫苗的个体相比，接受加强针的个体显示出全因死亡率的额外降低。

作者总结道，mRNA新冠疫苗接种与四年期间全因死亡率的持续且显著降低相关，这表明其具有超越对重症COVID-19急性保护的长期公共卫生益处。

---

## 25. 我写小众历史博客已经15年了。

**原文标题**: I have been writing a niche history blog for 15 years

**原文链接**: [https://resobscura.substack.com/p/why-i-have-been-writing-a-niche-history](https://resobscura.substack.com/p/why-i-have-been-writing-a-niche-history)

《Res Obscura》这个小众历史博客的作者回顾了15年来撰写冷门话题的经历，其内容主要集中在中世纪和早期现代西班牙的历史。该博客始于2009年，旨在作为一个个人平台，让作者在学术研究之余探索有趣的史料轶事，最初聚焦于斗牛、奇特的中世纪医疗实践以及“黑色传奇”等“古怪事物”。

随着时间的推移，博客从单纯罗列奇闻轶事发展为探索更广泛的主题，这得益于作者兴趣的变化以及对他独特视角的日益增强的自信。他强调，博客是一个低风险的智力探索空间，使他能够随心所欲地追随好奇心，不受学术出版的压力，也无需吸引大量读者。“小众”这一特点至关重要，它提供了一种智力自由和玩乐的感觉。

作者指出，尽管博客培养了一小群忠实的读者，但其主要动力仍是个人化的：即发现的乐趣、写作的过程以及自由探索那些令他着迷的话题，即使这些话题在他人看来可能微不足道。博客已成为他智力生活的核心部分，证明了在一个公开但低压力的论坛中追求个人兴趣的持久价值。

---

## 26. 国务院将以“审查制度”为由拒签事实核查员及其他人。

**原文标题**: State Department to deny visas to fact checkers and others, citing 'censorship'

**原文链接**: [https://www.npr.org/2025/12/04/nx-s1-5633444/trump-content-moderation-visas-censorship](https://www.npr.org/2025/12/04/nx-s1-5633444/trump-content-moderation-visas-censorship)

在特朗普政府领导下的美国国务院发布了一份内部备忘录，指示工作人员拒绝向参与事实核查、内容审核或“信任与安全”活动的人员发放H-1B签证。这些角色被归类为对美国人言论的“审查”，这项政策由国务卿马可·卢比奥首次宣布。

该指令针对高技能工人，特别是科技行业中，其工作经历表明参与打击虚假信息、错误信息或其他内容审查角色的人员。政府为此辩护，引用了特朗普总统此前在社交媒体上遭遇的封禁，以及声称科技公司不公平地针对保守派的说法。领事官员现在被要求彻底审查申请人的职业背景，包括简历和领英（LinkedIn）档案。

该政策招致了批评。曾从事信任与安全工作的爱丽丝·戈根·汉斯伯格对此表示担忧，并强调这类工作对于保护儿童（例如，免受儿童性虐待材料[CSAM]侵害）、防止欺诈以及确保整体网络安全至关重要，而非任意审查。她强调了全球工作人员在这些团队中对于多语言和文化理解的重要性。尽管一位匿名的国务院发言人为此政策辩护，称其旨在保护美国人的言论自由免受外国“审查者”的侵害，但像奈特第一修正案研究所的凯莉·德塞尔这样的第一修正案专家称其“语无伦次且违宪”，认为研究虚假信息和内容审核是受保护的言论形式。

与此同时，国务院还宣布了一项针对H-1B签证申请人及其受抚养人的新要求，要求他们将社交媒体个人资料设置为公开，以供官方审查。

---

## 27. 一种处方药，在欧洲售价20美元，在美国则高达800美元。

**原文标题**: A $20 drug in Europe requires a prescription and $800 in the U.S.

**原文链接**: [https://www.statnews.com/2025/10/31/why-miebo-costs-40-times-more-than-its-european-version/](https://www.statnews.com/2025/10/31/why-miebo-costs-40-times-more-than-its-european-version/)

这篇发布于2025年12月5日的“第一意见”文章，强调了欧美之间药品定价的巨大差异。文章特别指出，一种在欧洲售价20美元（需凭处方购买）的药物，在美国却飙升至800美元。该文以此惊人例子，旨在引出更广泛的讨论，正如其标题所示：“我们需要问的关于产妇死亡危机的问题”。文章将这种显著的药费差异，视为与持续的产妇死亡危机相关的一个关键因素或症状，表明高昂的医疗开支助长或加剧了这一紧迫的公共卫生问题。

---

## 28. 一架Cozy Mk IV轻型飞机因3D打印部件受热弱化而坠毁

**原文标题**: A Cozy Mk IV light aircraft crashed after 3D-printed part was weakened by heat

**原文链接**: [https://www.bbc.com/news/articles/c1w932vqye0o](https://www.bbc.com/news/articles/c1w932vqye0o)

一架Cozy Mk IV轻型飞机于3月18日在格洛斯特郡机场坠毁，原因是一个3D打印部件软化并坍塌，导致发动机完全失去动力。机上唯一的机组成员受了轻伤，但飞机被毁。

航空事故调查局（AAIB）报告称，那个在燃料系统改装期间安装、并在一次航空展上购买的塑料进气弯管，在暴露于发动机热量时失效。这种“不合适的材料”导致发动机在最终进近跑道时失去动力。飞行员短距着陆，撞上了仪表着陆系统。

事故发生后，轻型飞机协会（LAA）宣布将采取安全措施，包括向检查员发布“LAA警报”，以规范飞机上3D打印部件的正确使用。

---

## 29. 我如何在中国NanoKVM上发现隐藏麦克风

**原文标题**: How I discovered a hidden microphone on a Chinese NanoKVM

**原文链接**: [https://telefoncek.si/2025/02/2025-02-10-hidden-microphone-on-nanokvm/](https://telefoncek.si/2025/02/2025-02-10-hidden-microphone-on-nanokvm/)

NanoKVM是来自中国公司Sipeed的一款小巧且价格实惠的硬件KVM切换器，它允许用户通过网页浏览器远程控制电脑，而无需在目标机器上安装任何软件。它模拟虚拟键盘、鼠标和显示器，提供BIOS访问权限，甚至可以管理电源。尽管其承诺开源且价格低廉（约30-60欧元），该设备却存在严重的安全漏洞。

作者的安全审计揭示了诸多问题：初始默认的SSH密码、硬编码的加密密钥、依赖中国DNS服务器、与Sipeed的中国服务器通信时缺乏更新完整性检查，以及生产固件中预装了tcpdump和aircrack等黑客工具。

最令人担忧的是，作者在该设备上发现了一个微型（2x1毫米）、未记录的SMD麦克风。尽管尺寸很小，它却能录制高质量音频。此外，所有必要的录音工具（amixer、arecord）都已预装，可以轻松捕获音频，并通过SSH进行潜在的实时流传输（SSH最初使用默认密码）。由于其尺寸和电路板设计，物理移除该麦克风非常困难。

尽管作者将这些问题归因于极度的疏忽和仓促的开发，而非恶意意图，但其影响是严重的。该设备的开源性质提供了一线希望，因为社区正在努力将定制的、更安全的Linux发行版（如Ubuntu）移植到该设备上，这将需要刷写新的固件，并提供解决麦克风等硬件问题的机会。

---

## 30. Jolla 手机预购

**原文标题**: Jolla Phone Pre-Order

**原文链接**: [https://commerce.jolla.com/products/jolla-phone-preorder](https://commerce.jolla.com/products/jolla-phone-preorder)

Jolla Phone 是一款独立的欧洲 Linux 手机，搭载 Sailfish OS，旨在成为一款由社区塑造的、注重隐私的替代品。它通过预购系统提供，需支付 99 欧元的定金，定金可全额退还。该项目需在 2026 年 1 月 4 日前获得 2000 份预订单才能投入生产；目前已售出 1498 台（已达成 74% 的资金目标）。如果目标未达到，所有款项将全额退还。

主要功能包括“设计即隐私”（无追踪）、实体隐私开关以及用户可更换的电池和后盖选项。它提供现代规格，如支持双 SIM 卡的 5G 网络、12GB 内存、256GB 存储（可扩展）、6.36 英寸全高清 AMOLED 显示屏、5000 万像素主摄像头和 5500 毫安时电池。Sailfish OS 支持 Android 应用，并保证至少 5 年的操作系统更新。

预购可享受 499 欧元（含增值税）的特惠全价，而估计的正常价格为 599 欧元至 699 欧元。预计交付时间为 2026 年上半年末。首批上市市场为欧盟、英国、挪威和瑞士。这个“共同实现”项目让客户能够直接为将一个以隐私为中心、由社区定义的设备变为现实做出贡献。

---

## 31. 微核Linux：一个23 MB的带图形桌面的Linux发行版

**原文标题**: Tiny Core Linux: a 23 MB Linux distro with graphical desktop

**原文链接**: [http://www.tinycorelinux.net/](http://www.tinycorelinux.net/)

Tiny Core Linux，来自 Core 项目，是一个超小型、高度模块化的图形桌面操作系统。它的目标是创建一个游牧系统，能够从光盘、U盘或硬盘快速启动，驻留在内存中，并支持用户选择的应用程序和硬件。

基础“Core”系统仅为11MB，由一个Linux内核和基本模块组成。“TinyCore”是基于此基础构建的一个示例，添加了Xvesa、Xprogs、aterm、FLTK、FLWM和wbar等图形组件，形成了一个16MB的桌面。这反映了该项目的理念：用户从一个最小的核心开始，通过添加扩展来构建自定义的桌面、服务器或设备。

默认情况下，它不是一个完整的桌面，仅提供一个最小X桌面所需的核心组件，通常带有有线互联网连接。用户通过从在线仓库安装额外应用程序和硬件支持，或通过编译来定制他们的系统。“CorePlus”则提供了一个更简单的入门方式，其预打包了各种安装选项所需的扩展。

该项目鼓励开放的开发模式和社区参与。用户受邀通过打包应用程序或硬件支持来贡献，并可从八人组成的Tiny Core Linux团队在论坛和IRC获得帮助。最新版本是16.2，该项目由Robert Shingledecker于2008年12月1日启动。

---

## 32. 让RSS更有趣

**原文标题**: Making RSS More Fun

**原文链接**: [https://matduggan.com/making-rss-more-fun/](https://matduggan.com/making-rss-more-fun/)

作者对传统的RSS阅读器表示不满，认为它们因无休止的积压而变得繁琐。相反，作者渴望为“小网站”提供一种类似TikTok的内容发现体验——被动地消费随机的小创作者内容，由一个简单的算法驱动，用户点赞能增加可见性，并且没有广告或大量数据收集。这一概念类似于已停运的StumbleUpon，旨在对抗大语言模型（LLM）生成搜索结果的趋势。

为此，作者开发了“Timewaster Pro”，一个Firefox扩展（可在https://timewasterpro.xyz/获取）。用户点击一个按钮即可获得一个随机网站，然后可以点赞、点踩或举报。提交热门链接的用户可在排行榜上获得积分。后端使用FastAPI和SQLite构建，抓取Kagi小网站列表中的RSS订阅源，缓慢索引页面并跟踪用户投票，以优先展示“高质量”内容。

该项目使用复古的`system.css`来表明其非商业、爱好者性质。尽管已索引超过60万个页面，但作者指出键盘快捷键和身份验证（对JWTs表示遗憾）存在挑战。未来的计划包括实现内容分类、改善新用户的质量控制，并希望有更多样化的内容，如独立摄影和手工艺品。源代码将在稳定后发布。

---

## 33. GrapheneOS是唯一提供全面安全补丁的Android系统

**原文标题**: GrapheneOS is the only Android OS providing full security patches

**原文链接**: [https://grapheneos.social/@GrapheneOS/115647408229616018](https://grapheneos.social/@GrapheneOS/115647408229616018)

这篇文章强调了GrapheneOS提出的一个关键主张，即它声称自己是“唯一提供完整安全补丁的基于安卓的操作系统”。GrapheneOS自己在其官方Mastodon账户上提出的这一声明，使其在安卓生态系统中对全面安全更新的承诺显得与众不同。关于为Mastodon网页应用启用JavaScript的额外文字是一个与Mastodon平台相关的通用技术说明，与GrapheneOS的安全功能或声明无关。

---

## 34. 沃尔夫拉姆计算服务

**原文标题**: Wolfram Compute Services

**原文链接**: [https://writings.stephenwolfram.com/2025/12/instant-supercompute-launching-wolfram-compute-services/](https://writings.stephenwolfram.com/2025/12/instant-supercompute-launching-wolfram-compute-services/)

Wolfram 推出了 Wolfram 计算服务，使用户能够将 Wolfram 语言的计算无缝扩展到“超级计算机”的算力，而无需管理基础设施。该服务可在 Wolfram Desktop 14.3 中使用（通过 `RemoteBatchSubmissionEnvironment["WolframBatch"]`），并在 Wolfram Cloud 中自动提供，解决了对大规模高性能计算的需求。

该服务使用 `RemoteBatchSubmit` 等函数提交计算，自动处理依赖关系；并使用 `RemoteBatchMapSubmit` 在众多核心和机器上实现大规模并行计算。用户可以选择多种机器配置（1-192 核，8-1500 GB RAM），以适应不同的任务和预算。作业进度可通过仪表板监控，并通过电子邮件/短信接收状态更新通知。结果以可计算的 Wolfram 语言表达式形式检索，可立即使用。

Wolfram 计算服务是完全可编程的，允许用户设置诸如机器类别、时间/信用额度限制、作业名称和通知偏好等选项。它还支持查询作业属性和中止任务。该服务基于 Wolfram 语言的并行计算和云能力，简化了以前“自己动手”的云计算方法。未来计划包括推出 Wolfram HPCKit，用于整合组织内部的计算设施，并提供同步远程计算。这项举措旨在使广泛的 Wolfram 语言用户能够轻松使用高级计算。

---

## 35. 人工智能现状：基于OpenRouter的百万亿Token实证研究

**原文标题**: State of AI: An Empirical 100T Token Study with OpenRouter

**原文链接**: [https://openrouter.ai/state-of-ai](https://openrouter.ai/state-of-ai)

OpenRouter发布的《人工智能现状》报告，基于对18个月内100万亿生产流量（tokens）的实证研究，揭示了一个高度动态且快速发展的人工智能图景。研究强调，不存在单一的“最佳”模型，用户在各种应用中不断优化质量、速度和成本。

主要发现揭示了显著变化：
*   **质量：** 尽管GPT-4保持了强劲地位，但Claude 3 Opus等新模型已成为顶尖表现者，常因其更丰富的细节和洞察力而受到赞扬。Mixtral 8x7B以其卓越的性价比脱颖而出，以显著更低的成本提供了出色的结果。开源模型，尤其是Llama 2和Mistral-7B的微调版本，已大幅改进，对许多企业应用而言已“足够好用”。
*   **成本：** 市场经历了大规模的成本降低，使先进AI更易于获取，这主要得益于高效的开源替代方案。
*   **性能动态：** 模型性能并非一成不变；模型会随着时间推移而退化或改进，因此需要持续评估，而非假定质量始终如一。
*   **用户行为：** 用户频繁切换模型，利用OpenRouter等平台动态地将请求路由到最适合特定任务的模型，这揭示了多模型策略的关键作用。

该研究总结认为，AI市场以持续变化、激烈竞争和日益专业化为特征。在这个快速变化的环境中，动态评估和适应对于AI的最佳利用至关重要。

---

## 36. 带状疱疹疫苗接种在痴呆不同阶段的影响

**原文标题**: The effect of shingles vaccination at different stages of dementia

**原文链接**: [https://www.cell.com/cell/fulltext/S0092-8674(25)01256-5](https://www.cell.com/cell/fulltext/S0092-8674(25)01256-5)

无法访问文章链接。

---

## 37. 广告是人类不满的主要来源 (2019) [pdf]

**原文标题**: Advertising as a major source of human dissatisfaction (2019) [pdf]

**原文链接**: [https://www.andrewoswald.com/docs/AdvertisingMicheletal2019EasterlinVolume.pdf](https://www.andrewoswald.com/docs/AdvertisingMicheletal2019EasterlinVolume.pdf)

所提供的内容是原始的PDF流数据，无法直接读取或解析成人类可理解的文本。因此，我无法从文章本身提取要点、论据或关键信息以提供摘要。

然而，仅根据标题“广告作为人类不满的主要来源 (2019)”，这篇文章可能探讨广告如何促成不快乐或不满情绪的机制。它可能会深入探讨以下方面：

*   **制造不切实际的期望：** 广告常描绘理想化的生活方式或结果，与现实不符，从而导致失望。
*   **助长消费主义：** 鼓励人们不断追求新产品，暗示幸福可以购买，并让人对自己已有的东西感到不足。
*   **社会比较：** 强调他人拥有或取得的成就，从而加剧不足感或嫉妒。
*   **操控性技巧：** 审视广告中利用不安全感或制造虚假需求的心理策略。

2019年的出版日期表明，这是一篇关于该社会话题的相对较新的学术或研究作品。

---

## 38. 法官预示软件自由保护协会在Vizio GPL案中胜诉

**原文标题**: Judge Signals Win for Software Freedom Conservancy in Vizio GPL Case

**原文链接**: [https://fossforce.com/2025/12/judge-signals-win-for-software-freedom-conservancy-in-vizio-gpl-case/](https://fossforce.com/2025/12/judge-signals-win-for-software-freedom-conservancy-in-vizio-gpl-case/)

加州一名法官已初步支持软件自由保护协会（SFC）在其针对Vizio的诉讼中提出的指控，即Vizio违反了通用公共许可证（GPLv2）和宽通用公共许可证（LGPLv2.1）。该案件涉及Vizio的SmartCast电视，这些电视集成了Linux、BusyBox和其他开源软件，但未提供规定的源代码。

法官Sandy N. Leal的初步裁决表明，她支持SFC的主张，即Vizio有义务向SFC提供完整的源代码。SFC是作为Vizio智能电视的购买者而非版权所有者提起诉讼的。尽管这一裁决表明了法官的倾向，最终结果仍有待后续听证会决定。

文章指出，尽管目前法院对开源许可证的强制执行变得更可预测，但情况并非一直如此。21世纪初的案件，例如软件自由法律中心对Monsoon Multimedia等公司提起的诉讼，确立了维护这些许可条款的先例。

Vizio是一家成立于2002年的电视制造商，在沃尔玛（Walmart）于2024年12月完成对其23亿美元的收购后，Vizio成为了一个财力雄厚的“巨头”。沃尔玛打算将Vizio打造成其门店的独家自有品牌。此案对于一家新近资源充沛的公司而言，是开源合规性方面的重要考验。

---

## 39. 为什么我们用 Zig 构建 Lightpanda

**原文标题**: Why we built Lightpanda in Zig

**原文链接**: [https://lightpanda.io/blog/posts/why-we-built-lightpanda-in-zig](https://lightpanda.io/blog/posts/why-we-built-lightpanda-in-zig)

Lightpanda 选择 Zig，主要因为它简洁、高性能和现代化的工具链，动因是希望在一个类浏览器项目中避免 C++ 的复杂性以及 Rust 借用检查器带来的摩擦。

构建一个用于自动化的网络浏览器需要一种低级系统语言、高性能、精确的内存控制，以及与 V8（Chrome 的 C++ JavaScript 引擎）集成。C++ 被认为过于复杂，原因在于其庞大的特性集、手动内存管理风险和复杂的构建系统。Rust 虽然可行，但其借用检查器在处理浏览器引擎中常见的复杂、相互依赖的内存区域时带来了挑战，经常需要难以管理的 `unsafe` 代码。

Zig 提供了一个引人注目的替代方案，它比 C++ 和 Rust 更简洁，同时提供顶级的性能，并且比 C 语言拥有更好的工具链和安全性。Lightpanda 选择 Zig 的主要优势包括：
*   **显式内存管理：** 分配器提供精确控制，实现了高效的模式，例如为每次页面加载使用竞技场分配器，从而简化了内存清理并避免了垃圾回收的开销。
*   **编译时元编程：** 在编译时运行代码，减少了 V8 绑定所需的样板代码，并自动生成 JavaScript 封装器。
*   **一流的 C 语言互操作性：** 无缝直接使用 C 语言头文件和函数（例如 cURL），弥补了 Zig 相对较小的生态系统。
*   **内置构建系统：** 简化了依赖管理和交叉编译，并与 Zig 本身干净地集成。
*   **编译速度快：** 对于响应式开发反馈循环至关重要，并且还在不断改进中。

Lightpanda 发现 Zig 的学习曲线是可控的，其分配器模型非常有效，并且其社区提供支持。尽管仍处于 1.0 版本之前，Zig 已经足够稳定，可以用于生产，并使小型团队能够构建像 Lightpanda 这样复杂、高性能的软件。

---

## 40. 快速抗抑郁作用共同通路中的腺苷：咖啡悖论

**原文标题**: Adenosine on the common path of rapid antidepressant action: The coffee paradox

**原文链接**: [https://genomicpress.kglmeridian.com/view/journals/brainmed/aop/article-10.61373-bm025c.0134/article-10.61373-bm025c.0134.xml](https://genomicpress.kglmeridian.com/view/journals/brainmed/aop/article-10.61373-bm025c.0134/article-10.61373-bm025c.0134.xml)

抱歉，我无法提供题为“腺苷在快速抗抑郁作用的共同途径上：咖啡悖论”的文章摘要。

所提供的内容只显示一条错误信息：“您需要启用JavaScript才能运行此应用程序。”

为了总结该文章，请提供实际文本或指向其内容的有效链接。

---

## 41. 弗兰克·盖里逝世

**原文标题**: Frank Gehry has died

**原文链接**: [https://www.bbc.co.uk/news/articles/c5y2p22z9gno](https://www.bbc.co.uk/news/articles/c5y2p22z9gno)

弗兰克·盖里（Frank Gehry），上世纪最具影响力的建筑师之一，享年96岁去世。他以其前卫的解构主义风格而闻名，盖里利用了铁丝网、胶合板和钛等非传统材料，打破了传统的建筑原则。

他的国际突破性成就于1997年达成，当时他在西班牙毕尔巴鄂设计的钛板古根海姆博物馆（Guggenheim Museum）闻名遐迩地创造了“毕尔巴鄂效应”，成功振兴了该市的经济和旅游业。早些时候，他通过重新设计自己在圣莫尼卡（Santa Monica）的家而获得认可。

盖里于1989年荣获普利兹克建筑奖（Pritzker Architecture Prize），他率先使用3D建模技术来创建他标志性的曲线、雕塑般建筑。他的多元化作品包括洛杉矶的华特迪士尼音乐厅（Walt Disney Concert Hall）、芝加哥的杰伊·普利兹克露天音乐厅（Jay Pritzker Pavilion）、巴黎的路易威登基金会（Louis Vuitton Foundation）以及布拉格的跳舞的房子（Dancing House）。尽管面临批评，他常常不以为意，并留下了一句名言：“至少他们还在看！”他曾在《辛普森一家》（The Simpsons）中为自己配音客串，后来却因为人们对他的设计过程产生误解而“困扰”了他。

加拿大总理马克·卡尼（Mark Carney）、作家保罗·戈德伯格（Paul Goldberger）和古根海姆博物馆纷纷致敬，赞扬了他独特的愿景以及“突破界限”并从情感上感染人们的热情。他身后留下了妻子贝尔塔·伊莎贝尔·阿吉莱拉（Berta Isabel Aguilera）和四个孩子。他的精神和遗产将通过他遍布世界各地的标志性建筑永存。

---

## 42. Framework 赞助 CachyOS

**原文标题**: Framework Sponsors CachyOS

**原文链接**: [https://discuss.cachyos.org/t/framework-sponsorship-for-cachyos/19376](https://discuss.cachyos.org/t/framework-sponsorship-for-cachyos/19376)

CachyOS 宣布获得 Framework 的一项重大新赞助，该公司以其模块化和可维修笔记本电脑而闻名。这项合作对这个开源 Linux 项目意义重大，因为找到真正支持 Linux 的硬件合作伙伴非常罕见。

Framework 的贡献包括一台 Framework Laptop 16，CachyOS 将利用它在现代硬件上优化其内核和软件包。此外，Framework 还承诺每月捐赠 250 美元。这笔财政支持约占 CachyOS 每月总捐款的 10%，凸显了它对这个社区驱动项目的重要性。

这项赞助将帮助 CachyOS 稳定其基础设施，并进一步实现其最终目标：使开发人员能够全职从事该项目，以提供最快、最优化的 Linux 体验。CachyOS 鼓励其社区支持 Framework，并查看他们的博客文章，了解更多关于其赞助计划的信息。

---

## 43. Synadia 和 TigerBeetle 承诺向 Zig 软件基金会捐赠 51.2 万美元。

**原文标题**: Synadia and TigerBeetle Pledge $512k to the Zig Software Foundation

**原文链接**: [https://tigerbeetle.com/blog/2025-10-25-synadia-and-tigerbeetle-pledge-512k-to-the-zig-software-foundation/](https://tigerbeetle.com/blog/2025-10-25-synadia-and-tigerbeetle-pledge-512k-to-the-zig-software-foundation/)

Synadia 和 TigerBeetle 联合承诺在两年内向 Zig 软件基金会捐赠 51.2 万美元，以支持该语言、其领导层和社区。TigerBeetle 于 2020 年为其金融数据库选择了 Zig，而非 C 和 Rust。

Rust 因其默认的内存不足（OOM）处理哲学和借用检查器而被认为不适用，这与 TigerBeetle 对显式静态分配、单线程架构以及“全面正确性是一个设计问题”的方法论需求相冲突。

选择 Zig 是因为 Andrew Kelley 卓越的设计，其设计哲学强调没有隐藏的内存分配或控制流，拥有 `comptime` 等特性，以及出色的表达力与复杂性比。通过修正诸如使用边界检查解决空间内存安全问题，以及默认启用检查算术，它充当了“更好的 C”。Zig 对安全的处理被视为一个光谱，在增强可靠性的同时保持简洁。其减法设计和易学性也是关键因素。

五年过去了，这一决定得到了强有力的验证。TigerBeetle 经历了极端的模糊测试（VOPR、Vörtex、Jepsen 审计），Zig 的质量被证明无懈可击。该语言对公司的成功和快速发展至关重要，并吸引了重要的企业客户。即使是 1.0 版本之前的破坏性变更也易于管理，并且通常能提高编译速度。Zig 对独立编译器后端进行的投资也因其未来的精确性而受到关注。

两家公司都支持 Andrew Kelley 强有力的 BDFL 领导，重视设计中的概念完整性。他们“无附加条件”的承诺旨在确保 ZSF 保持独立和透明，大部分资金将直接支持贡献者。Synadia 首席执行官、同样是 Zig 赞助商的 Derek Collison 发起了这项联合声明，两家公司各捐赠 25.6 万美元。他们鼓励向 Zig 软件基金会进行更多捐赠。

---

## 44. NeurIPS 2025 最佳论文奖

**原文标题**: NeurIPS 2025 Best Paper Awards

**原文链接**: [https://blog.neurips.cc/2025/11/26/announcing-the-neurips-2025-best-paper-awards/](https://blog.neurips.cc/2025/11/26/announcing-the-neurips-2025-best-paper-awards/)

NeurIPS 2025 宣布了七项最佳论文奖，其中包括四项“最佳论文”（一项来自数据集与基准测试赛道）和三项“荣誉提名”，旨在表彰机器学习领域的突破性进展。

“最佳论文”包括：

1.  **“人工蜂巢：语言模型（及其他）的开放式同质性”** 介绍了一个名为 Infinity-Chat 的大规模基准测试，揭示了“人工蜂巢”效应，即大型语言模型（LLMs）生成同质化内容。该论文强调了与多样化人类偏好之间存在的严重失衡，对人类创造力构成风险。
2.  **“大型语言模型的门控注意力：非线性、稀疏性和无注意力汇聚”** 展示了在缩放点积注意力（Scaled Dot-Product Attention）之后添加一个简单的、针对每个头部的 Sigmoid 门控，可以持续提升大型语言模型的性能、训练稳定性和长上下文外推能力。这一易于实现的修改已被 Qwen3-Next 模型采用。
3.  **“用于自监督强化学习的千层网络：深度扩展可实现新的目标达成能力”** 通过展示在自监督强化学习中将网络深度增加至 1024 层可以显著提升性能并实现复杂的新能力，挑战了传统的强化学习（RL）认知。
4.  **“扩散模型为何不记忆：训练中隐式动态正则化的作用”** 为扩散模型提供了基础性见解，识别了不同的泛化和记忆时间尺度。该研究揭示了由于隐式动态正则化，有效泛化的窗口不断扩大，统一了经验和理论发现。

一项“荣誉提名”论文，**“强化学习真的能在基础模型之外激励大型语言模型的推理能力吗？”**，批判性地审视了大型语言模型中带有可验证奖励的强化学习（RLVR）。该论文认为，当前的 RLVR 主要提升了采样效率，而非在基础模型之外激发根本性的新推理模式或能力，并提出蒸馏法可能更有效。

---

## 45. PalmOS 在 费雪 Pixter 玩具上

**原文标题**: PalmOS on FisherPrice Pixter Toy

**原文链接**: [https://dmitry.gr/?r=05.Projects&proj=27.%20rePalm#pixter](https://dmitry.gr/?r=05.Projects&proj=27.%20rePalm#pixter)

rePalm项目旨在将PalmOS移植到费雪Pixter Color玩具上，这是一款21世纪初的儿童设备，配备160x160彩色显示屏和夏普LH75411 ARM SoC。尽管后续的Pixter Multimedia提供了4MB SDRAM，但Pixter Color的128KB板载RAM不足以运行PalmOS，因此需要外部RAM以及一个定制的48字节卡带头来启动。

Pixter Color的硬件带来了重大挑战。卡带插槽的16位数据总线缺少字节通道选择线，这迫使外部RAM必须以较慢的8位模式运行，才能保持字节寻址能力。这意味着一次32位内存读取最多可能需要16个CPU周期。

夏普LH75411 SoC本身的配置严重不足。它缺少缓存、MMU、MPU和协处理器15。这种缺失使得63MHz的CPU效率极低，因为它不断地等待内存。它还阻止了对齐检查和灵活的异常向量重定位等重要的调试和内存保护功能，使得NULL指针捕获变得不可能。尽管存在一些快速但有限的内部内存（16KB TCM、32KB eSRAM），但这些缺陷严重阻碍了性能和系统稳定性。

---

## 46. NASA贝努小行星样本中发现糖、树胶、星尘

**原文标题**: Sugars, Gum, Stardust Found in NASA's Asteroid Bennu Samples

**原文链接**: [https://www.nasa.gov/missions/osiris-rex/sugars-gum-stardust-found-in-nasas-asteroid-bennu-samples/](https://www.nasa.gov/missions/osiris-rex/sugars-gum-stardust-found-in-nasas-asteroid-bennu-samples/)

NASA的OSIRIS-REx任务从小行星Bennu采集的样本揭示了非凡的发现，为早期太阳系和生命起源提供了新见解。三篇新论文详细介绍了必需糖类、一种神秘的胶状物质以及超新星尘埃的意外丰富发现。

科学家发现了核糖（一种对RNA至关重要的五碳糖），以及首次在地外样本中发现的葡萄糖（一种六碳糖，是生命重要的能量来源）。这一发现，连同此前发现的氨基酸和核碱基，表明生命的分子构建块在早期太阳系中广泛存在。核糖的存在和脱氧核糖的缺失支持了“RNA世界”假说，表明RNA可能是早期生命信息存储和反应的主要分子。

还发现了一种前所未见的、富含氮和氧的胶状物质。这种古老的“太空胶”很可能在太阳系早期，当Bennu的母小行星变暖时形成，早于其成为水环境。类似于具有混杂化学结构的“太空塑料”，这种聚合物状物质可能为地球上的生命提供了化学前体。

最后，样本中含有异常丰富的超新星尘埃——比任何其他已研究的宇宙物质多出六倍。这表明Bennu的母体形成于原行星盘中一个富含垂死恒星尘埃的区域。尽管这颗小行星受到流体广泛改变，但其中未受明显改变的物质袋揭示了它所吸积的前太阳系物质的多样性。这些发现共同丰富了我们对宇宙化学和生命潜在途径的理解。

---

## 47. CUDA-l2: 通过强化学习超越 cuBLAS 的矩阵乘法性能

**原文标题**: CUDA-l2: Surpassing cuBLAS performance for matrix multiplication through RL

**原文链接**: [https://github.com/deepreinforce-ai/CUDA-L2](https://github.com/deepreinforce-ai/CUDA-L2)

CUDA-L2是一个新颖的系统，它利用大语言模型（LLMs）和强化学习（RL）自动优化半精度通用矩阵乘法（HGEMM）CUDA核函数。它系统性地超越了包括`torch.matmul`、cuBLAS和cuBLASLt变体在内的现有基线，在NVIDIA A100 GPU上跨1,000种（M,N,K）配置展现出显著的加速。

截至2025年12月，CUDA-L2已针对这1,000种配置发布了A100优化的HGEMM核函数，目前支持16位累加器。未来的开发目标包括支持32位累加器、更密集的矩阵配置、支持更多GPU（Hopper、Blackwell），以及更简便地部署开源LLMs。

要使用CUDA-L2，用户需要Python、PyTorch 2.6.0+，并必须克隆CUTLASS v4.2.1。关键是，必须配置`CUTLASS_DIR`和`TORCH_CUDA_ARCH_LIST`（例如，A100为"8.0"）环境变量。评估通过`eval_one_file.sh`脚本执行，该脚本支持`offline`（离线）和`server`（服务器）模式。参数包括问题大小（`--mnk`）、预热和基准测试持续时间、输出目录、GPU设备ID以及服务器模式下的目标每秒查询次数（`--target_qps`）。虽然A100核函数已针对A100进行优化，但仍可请求自定义矩阵维度。

---

## 48. 自闭症的“易混淆近亲”

**原文标题**: Autism's confusing cousins

**原文链接**: [https://www.psychiatrymargins.com/p/autisms-confusing-cousins](https://www.psychiatrymargins.com/p/autisms-confusing-cousins)

阿瓦伊斯·阿夫塔布（Awais Aftab）的《自闭症的迷惑表亲们》一文探讨了针对社交笨拙、刻板作息或高度专注等症状而广泛出现的自闭症自我诊断现象。作者作为一名精神病学家，承认自闭症的真实性，但认为许多表现出这些特质的人，实际上可能患有其他疾病。这些疾病常因自闭症的“模仿式传播”和更高的公众认知度而未被识别。

在临床医生看来，常见的、自我报告的“自闭症”特质常常与焦虑症或其他精神疾病相符。自闭症作为一种诊断具有吸引力，因为它为“古怪”或尴尬的经历提供了一个公认的解释，并提供了关键的服务和支持，而这些是鲜为人知的诊断所缺乏的。

文章详细列举了几种模仿自闭症但具有不同潜在机制的“表亲”病症：
*   **分裂样人格障碍：** 表现为缺乏社交兴趣，而非社交处理困难。
*   **分裂型人格障碍：** 奇异信念、魔法思维和知觉扭曲。
*   **强迫型人格障碍：** 源于焦虑和对控制的需求而表现出的僵化。
*   **社交恐惧症：** 对社会评判的强烈恐惧，在安全环境中常有改善。
*   **边缘性人格障碍：** 情绪不稳定和混乱的人际关系，这与自闭症的稳定自我概念和感觉问题不同。
*   **社交沟通障碍：** 具有自闭症的社交沟通困难，但没有重复行为或局限兴趣，常因缺乏相关服务而诊断不足。
*   **创伤相关障碍：** 社交退缩作为一种防御反应。

阿夫塔布强调，自闭症诊断是一种临床判断，而非医学检测，准确的鉴别诊断至关重要。他强调，一个人的困难并非被否认，而是被归因于众多诊断可能性中最合适的一种。

---

## 49. JavaScript缺失的多线程标准库

**原文标题**: The missing standard library for multithreading in JavaScript

**原文链接**: [https://github.com/W4G1/multithreading](https://github.com/W4G1/multithreading)

"Multithreading.js" 是一个 TypeScript 库，它为 JavaScript 提供了健壮的、受 Rust 启发的并发原语，抽象化了 Web Workers、序列化和 SharedArrayBuffer 的复杂性。它提供了一个托管线程池、严格的内存安全语义，旨在让多线程代码感觉像标准的异步 JavaScript。

该库的核心是 `spawn` 函数，它将任务提交到工作池并返回一个可等待的句柄。数据传输到 worker 由 `move()` 管理，它对可转移对象（例如 ArrayBuffer）执行零拷贝“移动”，或克隆其他数据。`SharedJsonBuffer` 促进了在共享内存中高效、受 Mutex 保护的 JSON 对象共享，针对持久或频繁访问的复杂数据进行了优化。

关键同步原语包括：
*   **互斥锁 (Mutex)：** 确保对共享数据的独占访问。
*   **读写锁 (RwLock)：** 针对读密集型场景进行优化，允许多个读取者或单个写入者。
*   **信号量 (Semaphore)：** 限制同时访问资源的线程数量。
*   **条件变量 (Condvar)：** 允许线程高效地等待特定条件而无需忙等待。
该库强烈建议使用异步方法（例如 `acquire`、`read`、`write`、`wait`），并支持 `using` 关键字用于自动释放锁。

对于更高级别的通信，多生产者-多消费者 (MPMC) `通道` 为任意 JSON 数据提供了一个有界、线程安全的队列，简化了 worker 间的协调和背压处理。Worker 也支持标准的动态 `await import()`，可用于相对本地文件和外部模块。

核心功能的浏览器兼容性广泛，但需要 `SharedArrayBuffer` 的同步原语必须进行跨域隔离（特定的 HTTP 头）。使用内容安全策略 (CSP) 的应用程序必须允许 `data:` 和 `blob:` URL 作为 worker 入口点。

---

## 50. 欧盟法院实际上已令用户生成内容平台无法合法运营。

**原文标题**: CJEU has made it effectively impossible to run a user-generated platform legally

**原文链接**: [https://www.techdirt.com/2025/12/04/eus-top-court-just-made-it-literally-impossible-to-run-a-user-generated-content-platform-legally/](https://www.techdirt.com/2025/12/04/eus-top-court-just-made-it-literally-impossible-to-run-a-user-generated-content-platform-legally/)

该文章指出，欧洲法院（CJEU）的近期裁决已使得用户生成内容（UGC）平台合法运营“实际上不可能”。

文章强调的核心问题在于，欧洲法院对平台的要求与现有欧盟规则之间存在直接矛盾。具体而言，作者指出这些新要求与欧盟自身禁止对平台施加普遍监控义务的规定相抵触。这种冲突被描述为一种“衔尾蛇困境”，即一种自我挫败或循环困境，其中遵守一套法规似乎又违反了另一套法规。文章最后强调，这给欧盟解决这一问题带来了重大而自相矛盾的挑战。

---

## 51. HTML：论文的可访问格式

**原文标题**: HTML as an Accessible Format for Papers

**原文链接**: [https://info.arxiv.org/about/accessible_HTML.html](https://info.arxiv.org/about/accessible_HTML.html)

arXiv已推出HTML格式论文作为一种无障碍格式，旨在通过补充现有PDF来解决研究领域中迫切的可访问性障碍。这一举措有助于屏幕阅读器、放大镜和移动设备的用户。HTML版本正在逐步回填到arXiv超过200万篇论文的语料库中，作者在提交时可以预览HTML版本。

HTML版本发布的“实验性”在于将各种LaTeX提交文档快速、自动地转换为HTML的巨大挑战。LaTeX的可扩展性意味着其使用方式多样，使得精确转换变得困难，并导致预期的渲染问题。尽管存在这些挑战，但由于社区对无障碍论文的迫切需求以及收集集体反馈的需要，该版本仍得以发布。

为了改进系统，arXiv鼓励社区参与。读者应尝试使用HTML论文并报告功能问题，例如不正确或难以辨认的布局。需要注意的是，HTML论文的渲染方式将与PDF不同，优先考虑适应性和可访问性，而非精确的视觉复刻。作者可以通过遵循LaTeX标记最佳实践做出贡献，开发人员可以协助LaTeXML项目。出版商和学会可以通过推荐使用受支持包的LaTeX `.cls` 文件来提供帮助。

arXiv感谢残疾科学家提供的宝贵见解，并感谢LaTeX项目以及NIST的LaTeXML团队，他们的关键工作使这一无障碍倡议得以实现。

---

## 52. 贝尔格莱德 Linux 安装节

**原文标题**: Linux Instal Fest Belgrade

**原文链接**: [https://dmz.rs/lif2025_en](https://dmz.rs/lif2025_en)

由Decentrala组织的“贝尔格莱德Linux安装节”将于2025年12月9日晚6点至9点在贝尔格莱德Jagićeva 5号数学系JAG3教室举行。主要目标是帮助参与者在他们的笔记本电脑上安装Linux操作系统，届时将有经验丰富的用户提供协助。根据参与者的兴趣，活动可能还会提供关于命令行、Git和C语言编程等主题的短期培训。

本次活动是“终结Windows 10”活动的一部分，旨在推广Linux作为Windows 10的替代品。原文指出Windows日益增长的不友好性、强制功能（云服务、AI、广告、强制账户）以及导致电子垃圾的硬件要求。与此相反，Linux提供了更愉悦的用户体验，在旧硬件上也能良好运行，并符合环保理念。

推荐初学者使用的Linux发行版包括Debian（及其衍生版，如Ubuntu、Mint）和Fedora。Arch则推荐给有经验的用户。Linux可以通过三种方式安装：在虚拟机中安装、与Windows双系统启动，或完全取代Windows。

至关重要的是，选择双系统启动或完全取代Windows的参与者在抵达前*务必*备份其系统分区中的数据。此外，也建议通过DistroSea在线探索不同的发行版。

Decentrala还将在同一地点举办两场相关活动：12月16日的“Linux命令行入门”和12月23日的“Git入门”，两场活动均于晚6点开始。本次安装节还将作为废旧电子设备的收集点，这些设备将捐赠给“Ponovo”组织进行维修，以减少电子垃圾。

---

## 53. 永续合约详解

**原文标题**: Perpetual futures, explained

**原文链接**: [https://www.bitsaboutmoney.com/archive/perpetual-futures-explained/](https://www.bitsaboutmoney.com/archive/perpetual-futures-explained/)

永续合约是加密货币交易量最大的方式，提供连续的现金结算合约，无需实物交割。尽管它早于加密货币出现，但在加密领域普及，旨在提供投机风险，同时降低交易所和做市商的资本要求，否则他们需要持有大量闲置资产以确保信任并支付盈利。

与传统期货不同，永续合约每天通过“资金费率”进行多次结算。赢家由输家支付，这些可以设置上限并包含利息成分的费率，有助于使永续合约价格与标的现货价格保持一致。当永续合约价格高于现货时，精明的做市商会执行“基差交易”（做空永续合约，买入现货）。这种delta中性策略从资金费率中获利，有助于价格趋同，同时也能通过他们的资本提供杠杆。然而，做市商也为交易所提供担保，如果交易所失败，他们的抵押品将面临风险。

永续合约提供极高的杠杆（通常是20倍-100倍，远超传统市场），这吸引了投机者，但也带来了巨大的风险。交易所通过清算过度杠杆的交易者获利，而“保险基金”通常用于弥补不足。然而，在极端市场波动中，系统的资本效率存在临界点。当保险基金不足时，“自动去杠杆”（ADL）机制启动，追溯性地减少赢家的利润以平衡市场，这对所有参与者来说都是一个关键且常被误解的尾部风险。

---

## 54. StardustOS：构建轻量级独立内核的库操作系统

**原文标题**: StardustOS: Library operating system for building light-weight Unikernels

**原文链接**: [https://github.com/StardustOS](https://github.com/StardustOS)

StardustOS是一个专为云应用设计的独内核操作系统，它在一个受保护的单一地址空间内运行，并将物理资源管理委托给可信的底层虚拟机管理程序。Stardust的代码库小巧且易于维护，它利用静态链接将一个最小化的内核与单个应用程序、其库和运行时环境结合成一个不可变、单一用途的虚拟机镜像。它支持多核、抢占式线程、基本的块设备和网络驱动程序，并提供POSIX兼容的库。

该系统在圣安德鲁斯大学用于教学和研究。相关项目包括：
*   **Stardust:** 原始的C语言独内核实现。
*   **Stardust-oxide:** 使用Rust语言对独内核的重新实现。
*   **Duster:** 一个用于在Xen虚拟机管理程序上运行的C语言独内核的调试器。

研究人员就Stardust发表了大量演讲并发布了相关材料，涵盖的主题包括独内核对Lambda函数的支持、调试、分布式微服务以及独内核的通用应用场景，这些主要在英国系统研究挑战研讨会和大学研讨会上进行。此外，一篇关于Stardust Oxide的学位论文也值得关注。

---

## 55. Perl的衰落是文化性的

**原文标题**: Perl's decline was cultural

**原文链接**: [https://www.beatworm.co.uk/blog/computers/perls-decline-was-cultural-not-technical](https://www.beatworm.co.uk/blog/computers/perls-decline-was-cultural-not-technical)

文章认为，Perl的衰落主要是文化上的，根植于其UNIX系统管理员的起源。作者从90年代中期到2005年大量使用Perl，他描述了一种“BOFH”文化，其特点是部落主义、门户之见、珍视难度（“自伤武器”）作为技能的标志，以及知识囤积。这种心态培养了一种保守的环境，在这种环境下，易用性被视为贬低成就。

这种文化保守主义却以一种矛盾的方式体现在“TIMTOWTDI”（There Is More Than One Way To Do It，即“不止一种方法可以做到”）中，这种做法表面上很灵活，却通过将创新推向CPAN（Comprehensive Perl Archive Network）阻碍了核心语言的变革。这种方法看似合理，却导致了“依赖地狱”和方法论的碎片化。

Perl 6的创建并非原因，而是内部不可调和矛盾的体现。社区分裂导致Perl 5加倍强调稳定性（以Perl 6为借口，解释其缺乏现代功能），而Perl 6则踏上了一条漫长、重设计但未能迅速交付的创新之路。

在此期间，Ruby on Rails等竞争者涌现，提供有主见的框架、欢迎新人的文化和简单的上手体验。PHP凭借其“零门槛”的方法和简单的部署，也获得了巨大的吸引力，尤其是在博客热潮中。Perl则因其内部冲突、复杂的生态系统以及一种常常蔑视新人的文化，变得吸引力大减，从而失去了在后端网络编程领域的主导地位。

---

## 56. 为什么速度很重要

**原文标题**: Why Speed Matters

**原文链接**: [https://lemire.me/blog/2025/12/05/why-speed-matters/](https://lemire.me/blog/2025/12/05/why-speed-matters/)

无法访问文章链接。

---

## 57. CSS 中的 Fizz Buzz

**原文标题**: Fizz Buzz in CSS

**原文链接**: [https://susam.net/fizz-buzz-in-css.html](https://susam.net/fizz-buzz-in-css.html)

Susam Pal 的文章《CSS 中的 Fizz Buzz》挑战读者在严格规则下，用尽可能少的 CSS 代码行实现经典的 Fizz Buzz 序列。核心限制是所有输出，包括数字和单词（"Fizz"、"Buzz"），都必须*直接*源自 CSS 样式表，明确禁止使用 JavaScript、纯 HTML 文本，或依赖 `<ol>` 自动列表编号等 HTML 特性。

Pal 提出了一种使用 `<li>` 元素和 CSS 计数器的四行 CSS 解决方案。其工作原理是：
1. 为每个 `<li>` 递增计数器 `n`。
2. 对于非 5 的倍数的 `<li>` 元素显示 `counter(n)`（处理常规数字）。
3. 将其覆盖，使 3 的倍数显示为 "Fizz"。
4. 为 5 的倍数追加 "Buzz"。

作者驳斥了使用 `<ol>` 等常见技巧，指出它们违反了“仅限 CSS 输出”的规则，并导致显示不整洁、不对齐。虽然主要目标是最小化代码行数，文章也简要讨论了字节数优化，提供了一个解决方案的压缩版本（152 字节）并提出了进一步缩减的建议。这篇文章旨在通过这个有趣的谜题展示 CSS 的能力。

---

## 58. AI反噬已至：公众对科技巨头的耐心为何殆尽

**原文标题**: The AI Backlash Is Here: Why Public Patience with Tech Giants Is Running Out

**原文链接**: [https://www.newsweek.com/ai-backlash-openai-meta-friend-10807425](https://www.newsweek.com/ai-backlash-openai-meta-friend-10807425)

公众对人工智能的耐心正在迅速消磨，从最初的乐观情绪转变为普遍的怀疑和公开的敌意。最初对生成式AI能简化生活的希望，已演变为对其感知到的好处主要服务于富裕科技巨头、未能解决实际问题并产生大量低质量“垃圾”内容的失望。

这种反弹的证据包括对AI生成广告的普遍嘲讽和破坏，例如Friend公司在地铁的广告被涂鸦上“监控资本主义”的标签，以及Skechers的AI广告被批“懒惰”。Bad Bunny和Drake等艺术家已公开抨击未经授权的AI声音克隆。皮尤研究中心的数据显示，这种转变非常显著，43%的美国成年人认为AI更有可能伤害而非帮助他们。

专家认为，AI被“过度吹捧”，其“不可避免的未来”叙事被用来取代工人、在没有问责的情况下实现自动化，以及未经同意滥用数据。Z世代用“clanker”梗来指代AI取代工作，也反映了这种担忧。

尽管投资巨大——2025年上半年超过3200亿美元，主要由美国超大规模企业和政治人物支持——专家们仍警告存在不可持续的泡沫。大部分支出似乎超过了合理的经济回报，其驱动力是AI公司之间“循环投资模式”而非真正的客户需求。该行业在大规模运营上仍普遍无利可图，预计到2030年将面临8000亿美元的收入缺口，以满足数据中心需求，这预示着一个“不可持续的模式”和一个可能产生广泛影响的潜在泡沫。

---

## 59. 维基飞：托管于维基媒体共享资源的完整电影

**原文标题**: WikiFlix: Full Movies Hosted on Wikimedia Commons

**原文链接**: [https://commons.wikimedia.org/wiki/User:Spinster/WikiFlix](https://commons.wikimedia.org/wiki/User:Spinster/WikiFlix)

WikiFlix是一个托管在维基共享资源上的原型，提供一个平台用于浏览和观看完整长度的、属于公共领域或知识共享许可的电影。它由维基数据驱动，旨在提供对海量电影收藏的免费访问，并在Toolforge上提供一个替代的独立应用程序。

用户可以通过多种类别浏览电影：按年代和具体年份（从19世纪70年代到21世纪20年代），按类型（例如，抽象片、动画片、纪录片、科幻片），按国家（例如，法国、印度、美国），按导演（例如，华特·迪士尼、谢尔盖·爱森斯坦），按演员（例如，查理·卓别林），甚至按角色（例如，米奇老鼠）。特别列表还突出显示了由女性导演、LGBT+导演执导的电影，以及被列入美国国家电影登记部的影片。

一个重要的部分专门用于“获奖影片”，由机器人定期更新。该列表详细列出了众多获奖电影，并根据它们所获得的具体奖项进行分类。例子包括各类奥斯卡金像奖（最佳影片、导演、男主角、女主角、纪录片等）、安锡水晶奖、印度电影观众奖、百花奖、墨索里尼杯、国家评论协会奖、印度国家电影奖、金棕榈奖、银熊奖和斯大林奖。每个条目都提供电影的片名、年份、时长、类型、导演和原产国等详细信息。

---

## 60. 盲人摸象 – TPUs

**原文标题**: Touching the Elephant – TPUs

**原文链接**: [https://considerthebulldog.com/tte-tpu/](https://considerthebulldog.com/tte-tpu/)

谷歌的张量处理单元（TPU）是一种开创性的硬件加速器，十多年前诞生，源于在摩尔定律和登纳德定律减速背景下，为满足深度学习爆炸性计算需求而生。谷歌在2013年认识到，使用通用硬件扩展数据中心是不可持续的，因此设计了专用芯片。

TPU是领域专用加速器，通过专注于线性代数运算，尤其是神经网络核心的矩阵乘法，以牺牲通用性换取性能。这种方法优化了高计算/数据访问比，并最大程度地减少了传统处理器中与控制流和通用内存访问相关的能量浪费。

第一代TPUv1面向*推理*。它是一个单线程协处理器，配备一个256x256的8位整数脉动阵列（矩阵乘法单元 - MXU）、一个软件控制的统一缓冲区和DDR3 DRAM。其精简设计，不含复杂的缓存或分支预测，依赖确定性执行和精确协调的数据移动（常采用双缓冲），以最大化MXU利用率。这使得它相对于当时的GPU在性能和功耗效率方面取得了显著提升（推理速度提升15-30倍，性能/功耗比提升30-80倍）。

TPUv2是为*训练*而开发的，需要更高的灵活性。它采用双核架构，每个核心集成了可编程向量单元、本地SRAM、HBM和一个128x128的MXU。主要进步包括用于多芯片通信的核间互连（ICI）以及BrainFloat16（BF16）浮点格式的采用，这对于神经网络训练过程中梯度计算所需的更高精度和动态范围至关重要。这一代允许更多样化和可编程的激活函数，反映了不断发展的算法需求。

---

## 61. Ofcom档案，第四部分：Ofcom卷土重来

**原文标题**: The Ofcom Files, Part 4: Ofcom Rides Again

**原文链接**: [https://prestonbyrne.com/2025/12/04/the-ofcom-files-part-4-ofcom-rides-again/](https://prestonbyrne.com/2025/12/04/the-ofcom-files-part-4-ofcom-rides-again/)

《Ofcom文件，第四部分》详细介绍了英国审查机构Ofcom与美国公司，特别是4chan之间持续的纠纷。Ofcom再次向4chan发出“威胁信”，在该公司拒绝支付罚款后扩大了调查范围。作者称该信是“法律上文盲般的胡言乱语”，声称拥有域外权力，旨在对身在美国的美国人执行英国的审查法律。

代表4chan的普雷斯顿·伯恩（Preston Byrne）发出了强硬回应。他提到了美国国会可能引入联邦《花岗岩法案》（GRANITE Act），这是一部受Ofcom此前行动启发、旨在反制外国审查的法律。伯恩明确表示，4chan不会实施Ofcom的“年龄验证”规则，坚称这些规则将破坏受第一修正案保护的匿名性。他澄清说，4chan在儿童安全问题上私下配合真正的执法机构，但不会与Ofcom合作，他将Ofcom视为一个缺乏执法能力的审查机构。伯恩强调，由于第一修正案，他的美国客户不受Ofcom管辖，同时抄送了美国政府官员。作者表示乐观，认为美国联邦立法将很快保护美国实体免受此类境外越权行为。

---

## 62. 2025年博客：向虚空呐喊

**原文标题**: Blogging in 2025: Screaming into the Void

**原文链接**: [https://askmike.org/articles/blogging-in-2025-screaming-into-the-void/](https://askmike.org/articles/blogging-in-2025-screaming-into-the-void/)

作者反思了从去中心化个人博客的“旧网络”到如今由中心化社交媒体平台主导的互联网的巨大转变。他们指出了开放网络的两个主要威胁：人工智能的普遍使用和付费内容的兴起。人工智能搜索工具现在直接从各种来源（包括博客）总结信息，减少了用户访问原始网站的需求。与此同时，高质量内容正越来越多地转移到付费墙后（例如，时事通讯），这虽然对写作者有利，但却削弱了开放、可访问的网络。

尽管面临这些挑战，作者仍被一种怀旧情绪驱使，想再次写博客。他们详细描述了如何使用AI编码工具，不是为了创建复杂的新功能，而是为了简化其现有的博客软件。这包括移除外部JavaScript跟踪器和像Google Fonts这样的第三方依赖，精简HTML/CSS以实现极简、响应式设计，并从一个无人维护的框架迁移到一个简单的静态网站生成脚本。其目标是符合“开放网络卫生”的价值观。

他们的极简主义博客，包括“mijnrealiteit”，现已上线。在移除了所有访客跟踪器后，作者承认他们将不知道谁在阅读他们的文章，并总结说他们是在“对着虚空呐喊”。

---

## 63. Nook 浏览器

**原文标题**: Nook Browser

**原文链接**: [https://browsewithnook.com](https://browsewithnook.com)

无法访问文章链接。

---

## 64. 乔纳森·伊夫的OpenAI设备不得使用“io”名称

**原文标题**: Jony Ive's OpenAI Device Barred From Using 'io' Name

**原文链接**: [https://www.macrumors.com/2025/12/05/openai-device-barred-from-io-name/](https://www.macrumors.com/2025/12/05/openai-device-barred-from-io-name/)

美国一家上诉法院维持了一项临时限制令，阻止OpenAI和乔尼·艾维（Jony Ive）的新硬件合资企业使用“io”这个名称，用于与AI音频初创公司iyO计划的产品类似的产品。

iyO于今年早些时候提起诉讼，称OpenAI计划使用的“io”品牌与其自身名称过于接近，用于类似的AI驱动硬件。法院文件显示，艾维和萨姆·奥特曼（Sam Altman）在2023年中期选择了“io”这个名称。在诉讼之前，iyO首席执行官杰森·鲁戈洛（Jason Rugolo）于2025年初接触奥特曼，寻求为一个“人机界面”项目提供资金，但奥特曼以存在竞争性项目为由拒绝。

OpenAI反驳称，其首款“io”产品并非可穿戴设备，且鲁戈洛是在提出收购建议时自愿披露了相关细节。尽管如此，一家地方法院发布了临时限制令，第九巡回上诉法院对此予以维持。上诉法院同意，“IO”和“iyO”之间存在混淆的可能性，考虑到OpenAI的规模，存在“反向混淆”的重大风险，以及对iyO品牌造成潜在的不可弥补的损害。

然而，该裁决仅禁止营销和销售与iyO计划的AI音频计算机足够相似的硬件，而非禁止所有“io”名称的使用。此案现已发回地方法院，定于2026年4月举行初步禁令听证会，而更广泛的诉讼预计将持续到2027年和2028年。OpenAI的首款硬件设备预计将于明年推出。

---

## 65. “鳄鱼恶魔岛”囚犯遭受“骇人听闻的人权侵犯”

**原文标题**: Detainees at 'Alligator Alcatraz' facing 'harrowing human right violations'

**原文链接**: [https://www.theguardian.com/us-news/2025/dec/04/alligator-alcatraz-human-right-violations-amnesty-report](https://www.theguardian.com/us-news/2025/dec/04/alligator-alcatraz-human-right-violations-amnesty-report)

一份新的大赦国际报告指控，佛罗里达州政府运营的“鳄鱼恶魔岛”和私营的克罗姆移民处理中心存在“骇人听闻的侵犯人权行为”。这份报告基于对被拘留者的采访和实地考察，详细描述了“残忍、不人道和有辱人格的待遇”，在某些情况下等同于酷刑。

在“鳄鱼恶魔岛”，被拘留者据称作为惩罚，被镣铐束缚在一个两英尺高的金属笼子（“箱子”）里，并在没有水的情况下被留在户外长达一天。该设施还被指存在不卫生的条件、马桶溢水、淋浴受限、持续照明、伙食差以及医疗服务被拒绝或不稳定等问题。据报道，被拘留者在牢房外总是被镣铐束缚。尽管联邦法官下达了关闭令，该设施仍重新开放，并在联邦监管之外运营，这使得被拘留者的追踪变得困难，并可能导致“强迫失踪”。佛罗里达州州长罗恩·德桑蒂斯的媒体秘书斥责该报告是“出于政治动机的捏造”。

大赦国际在克罗姆也发现了类似问题，包括过度拥挤、医疗疏忽、“令人担忧”的纪律措施（例如长时间单独监禁）以及难以获得法律代表。警卫的暴力和种族主义虐待很普遍，有些被拘留者被迫在没有设施的巴士上睡了好几天。人权观察此前也曾报道过克罗姆的虐待行为。

大赦国际建议关闭“鳄鱼恶魔岛”，结束佛罗里达州与联邦移民当局的合作，并停止“将移民定罪”和大规模拘留，称这种情况为“人权危机”。

---

## 66. 我用xcopy破解了两百美元的软件保护

**原文标题**: I cracked a $200 software protection with xcopy

**原文链接**: [https://www.ud2.rip/blog/enigma-protector/](https://www.ud2.rip/blog/enigma-protector/)

作者对应用于“Bass Bully Premium”VST3合成器的Enigma Protector（一款售价200美元的商业软件保护系统）进行了调查。Enigma宣称提供强大的安全性，具有RSA加密签名、硬件绑定许可、反调试以及基于虚拟机的代码混淆等功能，这预示着一项艰巨的挑战。

初步分析证实，安装程序受到Enigma的严密保护，表现出混淆的入口点，并需要涉及RSA签名和硬件ID绑定的复杂密钥验证。作者当时正准备进行RSA密钥分解或运行时钩取等复杂操作来绕过这些保护措施。

然而，一个关键缺陷被发现：由受保护安装程序提取的实际VST3插件（即“有效载荷”）完全没有受到保护。对VST的DLL文件进行扫描后发现，其中没有Enigma Protector或其许可API的任何引用。该VST在没有任何许可检查或运行时保护的情况下直接运行。

因此，这个复杂的200美元保护系统被一个“极其简单”的方法击败了：复制安装文件。所谓的“破解”仅仅是使用`xcopy`将VST及其相关数据从安装目录复制出来，从而使该软件无需合法许可或进一步修改即可在任何机器上运行。

这个案例研究强调了威胁建模和正确实施的重要性，而非花哨的安全功能。尽管Enigma Protector功能先进，但由于它只保护了安装程序，却让实际产品的运行时完全暴露无遗，因而变得毫无用处。这一事件表明，昂贵的保护系统如果应用不当则毫无价值，有时最简单的攻击却是最有效的。

---

## 67. AI泡沫破裂倒计时

**原文标题**: Countdown until the AI bubble bursts

**原文链接**: [https://pop-the-bubble.xyz/](https://pop-the-bubble.xyz/)

这个名为“AI泡沫破裂倒计时”的讽刺项目，展示了一个虚构的计时器，倒计时显示天、小时、分钟和秒，直至一个“预测日期”。该网站明确指出它并非真实存在，而是一个思想实验，其中一个AI（Gemini）根据网络新闻预测自身潜在的行业衰退。

每晚，一个脚本会提示Gemini搜索网络上的正面和负面AI新闻。根据所发现的情绪和经济指标，该AI会更新预测的“破裂日期”，并提供其推理的解释。用户还可以查看过去的预测，以了解情绪是如何演变的。

创作者澄清他们并非反对AI，承认其效用。然而，他们批评当前大规模的炒作周期、“万物皆AI”的趋势以及该领域普遍存在的循环投资经济。该项目本身就是用AI创建的，并且鼓励用户使用任何具有网络搜索能力的AI模型来复制该分析。

---

## 68. 欧盟对X处以1.2亿欧元罚款，因违反《数字服务法案》

**原文标题**: EU hits X with €120M fine for breaching the Digital Services Act

**原文链接**: [https://www.dw.com/en/eu-imposes-120-million-fine-on-elon-musks-x-for-breaking-digital-rules/a-75033724](https://www.dw.com/en/eu-imposes-120-million-fine-on-elon-musks-x-for-breaking-digital-rules/a-75033724)

欧盟已对埃隆·马斯克（Elon Musk）的社交媒体平台X处以1.2亿欧元的罚款，原因是其违反了《数字服务法案》（DSA）规定的透明度规则。欧盟委员会副主席亨娜·维尔库宁（Henna Virkkunen）表示，此次罚款是因为X“用蓝色认证标记欺骗用户、模糊广告信息并阻止研究人员”，她澄清说这是为了执行欧盟规则，而非审查制度。

这是欧盟委员会自2023年12月启动调查以来，首次开出此类罚单。X公司因在付费账户上使用蓝色认证标记虚假暗示真实性、广告商信息缺乏透明度以及拒绝研究人员获取数据而被罚。这1.2亿欧元的罚款中，4500万欧元涉及认证标记，3500万欧元涉及广告透明度，4000万欧元涉及研究人员数据访问。尽管《数字服务法案》的罚款最高可达全球营收的6%，但欧盟委员会强调，重点在于执行，而非开出最高额罚款。对X公司非法和操纵内容的进一步调查仍在进行中。

美国政府强烈谴责了欧盟的这一举动。美国副总统J.D.万斯（J.D. Vance）批评欧盟“为了垃圾而攻击美国公司”，而不是支持言论自由。美国商务部长霍华德·卢特尼克（Howard Lutnick）威胁将采取贸易后果。美国联邦通信委员会（FCC）主席布伦丹·卡尔（Brendan Carr）指责欧盟“监管窒息”，并“向美国人征税以补贴一个被欧洲自身窒息性法规所阻碍的大陆”。

---

## 69. 莱纳斯·托瓦兹认为埃隆·马斯克“太蠢了”，不配在科技公司工作。

**原文标题**: Linus Torvalds thinks Elon Musk is 'too stupid' to be working at a tech company

**原文链接**: [https://www.neowin.net/news/linux-creator-torvalds-thinks-elon-musk-is-too-stupid-to-be-working-at-a-tech-company/](https://www.neowin.net/news/linux-creator-torvalds-thinks-elon-musk-is-too-stupid-to-be-working-at-a-tech-company/)

Linux 创始人林纳斯·托瓦兹认为埃隆·马斯克“蠢到不适合在科技公司工作”，尤其批评了他对 Twitter（现称 X）的管理。在接受《Linux Journal》采访时，托瓦兹对马斯克的决策和领导力表示失望，从工程角度形容这些是“显而易见的糟糕想法”。

托瓦兹强调，马斯克显然缺乏对运营大型科技平台所涉及的技术复杂性以及人文因素的理解。他特别指出马斯克反复无常的行为以及对 Twitter 工程师和员工的轻蔑态度，暗示马斯克从根本上误解了成功科技公司的运作之道。托瓦兹暗示，马斯克的做法——其特点是缺乏对专业知识的尊重，以及热衷于冲动、技术上不合理的决策——表明他在科技领域有着深刻的无能。他将马斯克的行为与他认为在科技领域中有效且尊重的领导力形成了对比。

---

## 70. 老鼠空中捕食蝙蝠——研究人员拍下视频

**原文标题**: Rats Snatching Bats Out of the Air and Eating Them–Researchers Got It on Video

**原文链接**: [https://www.smithsonianmag.com/smart-news/rats-are-snatching-bats-out-of-the-air-and-eating-them-and-researchers-got-it-on-video-180987610/](https://www.smithsonianmag.com/smart-news/rats-are-snatching-bats-out-of-the-air-and-eating-them-and-researchers-got-it-on-video-180987610/)

Gloza-Rausch 等人在《全球生态与保护》期刊上发表的一项新研究，详细记录了首次科学观察到褐鼠（Rattus norvegicus）在德国北部积极捕食并食用蝙蝠的行为。科学家们在两个城市蝙蝠冬眠地使用红外摄像机，捕捉到老鼠采用不同策略的画面：伏击静止的蝙蝠，以及令人惊讶地通过后腿站立在空中捕捉飞行的蝙蝠。

这种新颖的行为凸显了老鼠在利用城市食物资源方面显著的适应性。然而，它也带来了双重担忧。首先，入侵性的鼠群可能严重影响当地蝙蝠种群；据计算，在冬季，老鼠在一个主要冬眠地可能捕食多达7%的蝙蝠。其次，已知携带多种病原体的物种之间的密切互动引发了对疾病溢出的担忧，这可能改变疾病动态，并扩大向人类和家畜传播的机会。

研究人员提倡通过改善垃圾管理和下水道维护，在关键蝙蝠冬眠地控制入侵性褐鼠种群。这种方法被视为一个“双赢”的解决方案，既能保护脆弱的蝙蝠种群，又能减轻潜在的公共卫生风险。

---

## 71. 华尔街竞相防范AI泡沫

**原文标题**: Wall Street races to protect itself from AI bubble

**原文链接**: [https://rollingout.com/2025/12/05/wall-street-protects-itself-ai-bubble/](https://rollingout.com/2025/12/05/wall-street-protects-itself-ai-bubble/)

这篇文章尽管标题暗示将更广泛地讨论华尔街如何保护自身免受人工智能泡沫的影响，但其内容却只专注于一个具体事件：Netflix公司在公布创纪录的盈利后股价仍暴跌。文章并未详细阐述人工智能泡沫、华尔街的反应，也未说明Netflix的表现与标题所指的更广泛市场担忧之间有何关联。

---

## 72. 65XX 系列 CPU 的扩展指令 (1996)

**原文标题**: Extra Instructions Of The 65XX Series CPU (1996)

**原文链接**: [http://www.ffd2.com/fridge/docs/6502-NMOS.extra.opcodes](http://www.ffd2.com/fridge/docs/6502-NMOS.extra.opcodes)

亚当·瓦迪在1996年的这份题为《65XX系列CPU的额外指令》的文档中，详细介绍了6502/85XX系列CPU的105个“未文档化”、“非官方”或“未来扩展”操作码，这些操作码不属于标准的151条指令集。该文档在《The Complete Inner Space Anthology》和瓦迪自身研究的帮助下汇编而成，提供了十六进制操作码值、寻址模式、执行周期以及等效的标准指令。

所描述的操作码通常结合了两种标准操作：
*   **ASO (SLO):** ASL内存，然后ORA累加器。
*   **RLA:** ROL内存，然后AND累加器。
*   **LSE (SRE):** LSR内存，然后EOR累加器。
*   **RRA:** ROR内存，然后ADC累加器。
*   **DCM (DCP):** DEC内存，然后CMP累加器。
*   **INS (ISC):** INC内存，然后SBC累加器。

其他操作码包括：
*   **LAX:** 从内存加载A和X。
*   **AXS (SAX):** 对A和X执行AND操作，然后存储到内存。
*   立即模式操作，例如**ALR**（AND A，然后LSR）和**ARR**（AND A，然后ROR，具有复杂的标志行为）。
*   **XAA**（TXA，然后立即数AND）和**OAL**（将A与常量进行OR操作，然后立即数AND，存储到A和X），两者均因在不同机器上行为各异而著称。
*   **NOP**（1A，3A等）、**SKB**（跳过字节）、**SKW**（跳过字）和**HLT**（使CPU崩溃，02，12等）。

瓦迪独家发现的**TAS、SAY、XAS和AXA**涉及与寄存器和内存的复杂AND操作。它们的特点是不影响标准标志/寄存器，并表现出不稳定的行为（例如，存储到非预期地址，依赖于视频显示）。该文档还纠正了错误信息，声明MKA/MKX等操作码不存在，并阐明了几条指令的寻址模式。它警告了某些操作码（LAS、XAA、OAL）的可变性和不可靠性。

---

## 73. Rsync.net 技术笔记 — 2025年第四季度

**原文标题**: Rsync.net Technical Notes – Q4 2025

**原文链接**: [https://www.rsync.net/resources/notes/2025-q4-rsync.net_technotes.html](https://www.rsync.net/resources/notes/2025-q4-rsync.net_technotes.html)

Rsync.net 2025年第四季度技术说明详细介绍了三个关键领域：安全的仅追加备份、ZFS vdev重平衡以及Borg挂载语法。

针对仅追加备份，rsync.net现已支持 `rclone serve restic --stdio`。此方法通过标准I/O运行，绕过了 `rclone serve` 常见的网络套接字限制。用户需创建两个SSH密钥：一个用于初始 `restic init` 设置的“普通”密钥，以及一个受限的“仅追加”密钥。在 `authorized_keys` 中配置的受限密钥，明确限制仅可用于特定存储库的 `rclone serve restic --stdio --append-only`。这确保了即使客户端系统被攻破，也无法删除或修改远程备份，因为它只拥有仅追加密钥。Restic本身在rsync.net平台上通过 `rclone` 运行。

文档还阐述了ZFS vdev重平衡问题。当向一个接近满载的zpool添加新的vdev时，新的写入最初会分散分布，但随着旧的vdev几乎填满，写入最终会集中在新vdev上，从而降低性能。解决方案是设置 `vfs.zfs.mg.noalloc_threshold`（例如，设置为8%的可用空间），并将一个大型数据集（例如10-12.5TB）从池中复制回池本身。这个过程会将复制的数据均匀地重新分布到所有vdev上。随后删除原始数据，即可有效重平衡并整理池，从而提升整体性能。

最后，说明还演示了远程挂载Borg存储库。命令 `borg mount --remote-path=borg14 user@rsync.net:path/path/repo/ /mnt/borg` 将远程存储库本地挂载为只读的 `borgfs` (FUSE) 文件系统，方便轻松访问和检查备份。

---

## 74. Zellij：一个开箱即用的终端工作区

**原文标题**: Zellij: A terminal workspace with batteries included

**原文链接**: [https://zellij.dev](https://zellij.dev)

Zellij 是一个“自带所需功能的终端工作区”。文章强调它适用于 Linux 和 macOS，并提供直接下载链接。对于希望在不完全安装的情况下试用 Zellij 的用户，它提供了适用于 bash/zsh 和 fish shell 的简单命令，以及一个查看执行脚本的链接。此外，开发者还提供 Zellij 贴纸。

---

## 75. 华纳兄弟与Netflix开启独家交易谈判

**原文标题**: Warner Bros Begins Exclusive Deal Talks With Netflix

**原文链接**: [https://www.bloomberg.com/news/articles/2025-12-05/warner-bros-is-said-to-begin-exclusive-deal-talks-with-netflix](https://www.bloomberg.com/news/articles/2025-12-05/warner-bros-is-said-to-begin-exclusive-deal-talks-with-netflix)

无法访问文章链接。

---

## 76. HN 展示：Pbnj —— 极简自托管文本粘贴服务，60秒即可部署。

**原文标题**: Show HN: Pbnj – A minimal, self-hosted pastebin you can deploy in 60 seconds

**原文链接**: [https://pbnj.sh/](https://pbnj.sh/)

Pbnj是一个极简的自托管pastebin解决方案，旨在通过简单的URL分享代码片段和文本文件，无需账户，也没有冗余功能。它承诺“60秒部署”，主要通过一键部署到Cloudflare实现，这种方式会自动fork GitHub仓库。

一个显著的优点是其成本效益：Pbnj利用Cloudflare D1的免费套餐，提供500 MB存储空间、每天500万次读取和10万次写入，这使得它对大多数用户来说几乎是免费的。

Pbnj既包含一个用于直接通过浏览器使用的Web界面，也支持广泛的CLI/API。配置通过一个单独的`pbnj.config.js`文件管理。对于程序化访问，它使用Bearer令牌认证，而Web界面则依赖于安全的基于会话的认证。CLI可以通过npm安装，并可使用交互式设置向导进行配置。

---

## 77. 消息人士：奈飞领跑华纳兄弟探索公司竞购战

**原文标题**: Netflix becomes frontrunner in bidding war for Warner Bros. Discovery – sources

**原文链接**: [https://www.cnn.com/2025/12/04/media/netflix-paramount-wbd-bidding-war-warner-bros-discovery](https://www.cnn.com/2025/12/04/media/netflix-paramount-wbd-bidding-war-warner-bros-discovery)

奈飞（Netflix）在华纳兄弟探索公司（WBD）的制片厂和流媒体资产竞购战中脱颖而出，成为领跑者，迄今为止出价最高，为每股28美元，竞购华纳兄弟制片厂和HBO Max等组成部分。竞争对手派拉蒙（Paramount）出价每股27美元，但其目标是包括CNN在内的整个WBD公司，这与只对制片厂和流媒体部门感兴趣的奈飞和康卡斯特（Comcast）不同。

消息人士指出，WBD和奈飞已进入独家谈判。此举之前，派拉蒙的法律团队对竞购过程表示“严重担忧”，指责WBD偏袒奈飞，这可能预示着由首席执行官大卫·埃里森（David Ellison）领导的派拉蒙正试图进行恶意收购。

竞购战之所以加剧，是因为WBD董事会因2022年合并后股价大幅下跌而面临压力，此前曾计划拆分公司。派拉蒙的出价旨在在该拆分之前收购整个公司。

一个关键因素是“王牌”：派拉蒙首席执行官大卫·埃里森与特朗普总统的所谓关系可能有助于反垄断审批，尽管这并非指总统的实际否决权。然而，任何交易都将面临全球监管审查，参议员迈克·李（Mike Lee）和分析师们对竞争问题提出了严重担忧，他们认为奈飞收购WBD资产可能会使其成为无可争议的全球巨头，从而有效终结“流媒体大战”。

---

## 78. X因违反内容规定被欧盟罚款1.4亿美元

**原文标题**: X hit with $140M EU fine for breaching content rules

**原文链接**: [https://www.reuters.com/sustainability/boards-policy-regulation/eu-fines-x-140-mln-breaching-online-content-rules-tiktok-settles-with-2025-12-05/](https://www.reuters.com/sustainability/boards-policy-regulation/eu-fines-x-140-mln-breaching-online-content-rules-tiktok-settles-with-2025-12-05/)

X（前身为推特）因违反欧盟在线内容规定，被欧盟处以1.4亿欧元（合1.52亿美元）的罚款。这笔由监管机构处以的罚款，源于该公司未能根据欧盟法律要求充分执行内容审核政策，尤其是在移除非法内容和保护用户免受有害材料侵害方面。此次处罚凸显了欧盟根据其严厉的《数字服务法案》（DSA），致力于追究主要科技平台的责任。

对X公司的罚款是根据这些法规处以的最大罚款之一，向在欧盟运营的其他数字服务商发出了强烈信号。文章还提到，TikTok已就无关事项与欧盟达成和解，这表明欧洲监管机构正在更广泛地推动整个科技行业强制执行合规性。此举凸显了社交媒体公司在欧洲市场，在内容治理和用户安全方面面临日益严格的审查。

---

## 79. 汉默史密斯桥 – 2.5万辆车去哪了？

**原文标题**: Hammersmith Bridge – Where did 25k vehicles go?

**原文链接**: [https://nickmaini.substack.com/p/hammersmith-bridge](https://nickmaini.substack.com/p/hammersmith-bridge)

Nick Maini题为“哈默史密斯桥——2.5万辆车去哪儿了？”的文章，探讨了2019年4月哈默史密斯桥因结构安全问题禁止机动车通行后，出现的令人惊讶的交通模式。在关闭之前，该桥每日通行2.5万辆车，这曾导致人们普遍预测周边路线会出现严重交通堵塞，甚至“交通末日”。

然而，与这些预期相反的是，预期的混乱并未发生。尽管普特尼桥和奇西克桥等邻近桥梁的车流量确实有所增加（分别增加了16%和32%），但这些增加量仅相当于约1.1万辆被分流的车辆。这意味着大约有1.4万辆车似乎从道路网络中“消失了”。

作者将这种现象归因于“消失的交通量”或是“诱导需求”的逆向效应。可能的解释包括人们减少非必要的驾车出行、转乘公共交通、骑自行车或步行，以及寻找全新的、不那么直接的路线。文章中引用的研究表明，当道路通行能力被削减时，大部分（通常是40-60%）被转移的交通量会直接消失，而不是完全重新规划路线。

哈默史密斯桥的关闭是一个引人注目的真实案例研究，它表明城市可以在不必然导致经常被预测的灾难性拥堵的情况下，显著削减道路通行能力和对汽车的依赖。这强调了城市重新思考其对私家车依赖的潜力，并在实施变革时减少对大范围交通堵塞的担忧。

---

## 80. 谷歌调查Gmail遭入侵：用户被锁且无法恢复

**原文标题**: Google 'Looking into' Gmail Hack Locking Users Out with No Recovery

**原文链接**: [https://www.forbes.com/sites/daveywinder/2025/12/05/google-looking-into-gmail-hack-locking-users-out-with-no-recovery/](https://www.forbes.com/sites/daveywinder/2025/12/05/google-looking-into-gmail-hack-locking-users-out-with-no-recovery/)

一场毁灭性的Gmail黑客攻击导致用户被锁定在账户之外，且没有恢复选项，促使谷歌声明正在“调查”此问题。网络安全作家戴维·温德尔（Davey Winder）强调了一种新的巧妙策略：黑客入侵Gmail账户后，将用户的年龄更改为儿童（例如10岁），然后将其添加到攻击者控制的家庭账户中。这种操作有效地将合法所有者锁定在外，绕过了所有标准的恢复方法。

受害者，例如一位在Reddit上发帖的用户，发现自己无法重新获得访问权限，有时还面临要求支付礼品卡赎金的情况。这种“儿童账户”机制阻止了对恢复选项的访问，许多人认为这是谷歌本应预料到的一个漏洞，尤其是考虑到该账户的实际存在时间（例如12年）。

谷歌承认这是一种“已知的攻击后行为”，但声称这种情况并不常见，尽管专家担心随着这种策略的曝光，它会蔓延开来。谷歌承诺“在不久的将来提供具体指导”。在此期间，谷歌建议用户通过启用两步验证和通行密钥，并定期检查关联设备和恢复信息（电子邮件、电话、联系人）来防止账户被初步入侵。核心信息是，主动安全是抵御这种独特锁定威胁的最佳防御方式。

---

## 81. YouTuber爆红克隆技术意外搅乱珍稀植物市场

**原文标题**: YouTuber accidentally crashes the rare plant market with viral cloning technique

**原文链接**: [https://www.dexerto.com/youtube/youtuber-accidentally-crashes-the-rare-plant-market-with-a-viral-cloning-technique-3289808/](https://www.dexerto.com/youtube/youtuber-accidentally-crashes-the-rare-plant-market-with-a-viral-cloning-technique-3289808/)

YouTuber“罐中植物”通过推广“组织培养”技术，无意中扰乱了利润丰厚的珍稀植物市场。这项技术能够快速、大规模地繁殖难以寻觅的植物。曾因稀有而身价高达数百或数千美元的珍稀植物，现在正变得更容易获得。

组织培养是指取一小块植物组织，对其进行消毒，然后在营养丰富的凝胶中培育，以产生新的、基因完全相同的植物（克隆体）。“罐中植物”将她的在线内容围绕这一方法展开，提供教程和新手工具包，让更多人能够接触到这种方法。

这大大降低了许多物种的“珍稀”地位和市场价值，引发了植物收藏界的一场激烈辩论。批评者指出克隆植物缺乏天然遗传变异，而支持者则认为组织培养终结了人为的稀缺性，并为非法珍稀植物贸易提供了一种人道的替代方案，后者常常涉及走私并威胁物种灭绝。

“罐中植物”将这种情况比作实验室培育钻石对开采钻石需求的影响，并表示“珍稀植物的垄断时代已经结束。”许多粉丝表示赞同，庆祝人为稀缺性的终结，并希望这能阻止盗采行为。

---

## 82. 布鲁塞尔如何制定如此多的法律

**原文标题**: How Brussels writes so many laws

**原文链接**: [https://www.siliconcontinent.com/p/how-brussels-writes-so-many-laws](https://www.siliconcontinent.com/p/how-brussels-writes-so-many-laws)

尽管存在一个复杂、多主体且有众多否决点的系统，本应导致僵局，但欧盟却展现出非凡的立法生产力，在2019年至2024年间通过了约13,000项法案。这种悖论可以用激励机制来解释：该机制奖励每个主体制定立法，而非行使否决权。

欧盟委员会预算微薄，却将立法作为其主要政策工具，以此扩大其权限和人员。它在谈判中充当“执笔人”，巧妙地引导结果。旨在进行公开辩论的正式立法程序，已在很大程度上被议会、理事会和委员会代表参与的非公开“三方会谈”所取代。这些非正式、通常马拉松式的会议绕过了公众监督，使得协议能够迅速达成，但有时也会导致草拟错误。

在欧洲议会内部，权力集中在专门委员会和少数“报告员”手中，他们闭门谈判达成协议。这些协议被宣称是“我们能达成的最佳妥协”，随后通常由全体委员会和全体会议走形式地批准，往往鲜有辩论。同样，由轮值主席国代表的部长理事会，在其短暂任期内优先达成协议，经常做出让步以实现快速成功。

这一系统因日益依赖“技术性三方会谈”中的工作人员而得到强化，并因新冠疫情而加速，优先追求数量。其结果往往是低质量立法，不同法律之间存在相互矛盾的要求，并且缺乏系统的影响评估或反馈机制。共识是事先人为制造的，绕过了正式审查，导致欧盟法律持续扩张。

---

## 83. 谁把笔记本电脑接到一台1930年代的舞厅机器上？

**原文标题**: Who Hooked Up a Laptop to a 1930s Dance Hall Machine?

**原文链接**: [https://www.chrisbako.com/posts/2025-12-04-speelkok-museam](https://www.chrisbako.com/posts/2025-12-04-speelkok-museam)

Chris在2023年的一次荷兰之旅中，参观了位于乌得勒支、以其自动演奏乐器藏品闻名的斯皮尔克洛克博物馆。他对一台20世纪30年代的舞厅自动演奏机尤其着迷。这台历史悠久的乐器最初通过打孔的硬纸板乐谱演奏音乐，其中孔洞代表音符——这相比早期的音乐滚筒是一项创新。

令Chris惊讶的是，这台老式机器已经被改装，可以直接从笔记本电脑播放MP3文件。实现这一技术整合的方法、原因以及相关人员，对他来说仍然是个谜。对此着迷的Chris已向博物馆发送邮件询问更多详情，目前正在等待回复。他也在向互联网社区寻求帮助，希望能够发现更多关于这种独特改造的信息。

---

## 84. 安娜的档案已发布完所有收录的中文书籍

**原文标题**: Anna's Archive finished releasing all obtained Chinese books

**原文链接**: [https://annas-archive.li/blog/finished-chinese-release.html](https://annas-archive.li/blog/finished-chinese-release.html)

Anna's Archive has announced the completion of its two-year-long Chinese book release, successfully integrating a massive volume of content into its open library, largely thanks to dedicated volunteers.

The release features numerous significant collections:
*   **DuXiu:** A massive database of academic books, acquired from an anonymous volunteer who had already gathered the full collection, ensuring its long-term preservation. This involved converting proprietary formats like PDG to PDF.
*   **CADAL:** A vast collection of ancient books, totaling over 600,000 files, downloaded years ago via exploits.
*   **ScienceReading:** A large crawl conducted by about 30 volunteers exploiting an unprecedented website vulnerability in August 2024.
*   **Shukui.net (CDL):** Scrape of a Chinese shadow library, including its "secondary library" (Chinese Digital Library), with plans for its "primary library."
*   **Other key scrapes:** Include airitibooks (iRead eBooks), dedao (China Platform Book Library), ptpress (Posts & Telecom Press), huafuzhi (China Textile Publishing), and zjjd (with decryption of .zjjd files).
*   **Specialized collections:** Such as ancient books from Shanghai Library, judicial archives from Longquan, academic journals (SuperStar Journals), and local histories (wanfang xinfangzhi).
*   **Volunteer contributions:** Many collections came directly from volunteers like cgiym, woz9ts, and others, sourcing texts from major publishers, Taiwan e-books, and even personal archives or decrypted shadow libraries.

This monumental effort involved extensive scraping, exploiting network vulnerabilities, decrypting encrypted files, and converting formats, all driven by volunteers committed to building the largest truly open library.

---

## 85. What is better: a lookup table or an enum type?

**原文标题**: What is better: a lookup table or an enum type?

**原文链接**: [https://www.cybertec-postgresql.com/en/lookup-table-or-enum-type/](https://www.cybertec-postgresql.com/en/lookup-table-or-enum-type/)

生成摘要时出错

---

## 86. SMS phishers pivot to points, taxes, fake retailers

**原文标题**: SMS phishers pivot to points, taxes, fake retailers

**原文链接**: [https://krebsonsecurity.com/2025/12/sms-phishers-pivot-to-points-taxes-fake-retailers/](https://krebsonsecurity.com/2025/12/sms-phishers-pivot-to-points-taxes-fake-retailers/)

生成摘要时出错

---

## 87. 'Life being stressful is not an illness' – GPs on mental health over-diagnosis

**原文标题**: 'Life being stressful is not an illness' – GPs on mental health over-diagnosis

**原文链接**: [https://www.bbc.com/news/articles/cx2pvxdn9v4o](https://www.bbc.com/news/articles/cx2pvxdn9v4o)

生成摘要时出错

---

## 88. US will now review H-1B applicants' social media – require them to make public

**原文标题**: US will now review H-1B applicants' social media – require them to make public

**原文链接**: [https://www.businessinsider.com/us-to-review-h-1b-applicants-social-media-state-dept-2025-12](https://www.businessinsider.com/us-to-review-h-1b-applicants-social-media-state-dept-2025-12)

生成摘要时出错

---

## 89. Fast trigram based code search

**原文标题**: Fast trigram based code search

**原文链接**: [https://github.com/sourcegraph/zoekt](https://github.com/sourcegraph/zoekt)

生成摘要时出错

---

## 90. Coca Cola has an executive dedicated to McDonald's

**原文标题**: Coca Cola has an executive dedicated to McDonald's

**原文链接**: [https://www.coca-colacompany.com/about-us/leadership/roberto-mercade](https://www.coca-colacompany.com/about-us/leadership/roberto-mercade)

生成摘要时出错

---

## 91. SpaceX in Talks for Share Sale That Would Boost Valuation to $800B

**原文标题**: SpaceX in Talks for Share Sale That Would Boost Valuation to $800B

**原文链接**: [https://www.wsj.com/business/spacex-in-talks-for-share-sale-that-would-boost-valuation-to-800-billion-b2852191](https://www.wsj.com/business/spacex-in-talks-for-share-sale-that-would-boost-valuation-to-800-billion-b2852191)

生成摘要时出错

---

## 92. Why we can’t quit Excel

**原文标题**: Why we can’t quit Excel

**原文链接**: [https://www.bloomberg.com/features/2025-microsoft-excel-ai-software/](https://www.bloomberg.com/features/2025-microsoft-excel-ai-software/)

生成摘要时出错

---

## 93. Without evidence, RFK Jr.'s vaccine panel tosses hep B vaccine recommendation

**原文标题**: Without evidence, RFK Jr.'s vaccine panel tosses hep B vaccine recommendation

**原文链接**: [https://arstechnica.com/health/2025/12/without-evidence-rfk-jr-s-vaccine-panel-tosses-heb-b-vaccine-recommendation/](https://arstechnica.com/health/2025/12/without-evidence-rfk-jr-s-vaccine-panel-tosses-heb-b-vaccine-recommendation/)

生成摘要时出错

---

## 94. The Disappearance of an Anti-AI Activist

**原文标题**: The Disappearance of an Anti-AI Activist

**原文链接**: [https://www.theatlantic.com/technology/2025/12/sam-kirchner-missing-stop-ai/685144/](https://www.theatlantic.com/technology/2025/12/sam-kirchner-missing-stop-ai/685144/)

生成摘要时出错

---

## 95. FDA proposes impossible standards for vaccines that could curtail access

**原文标题**: FDA proposes impossible standards for vaccines that could curtail access

**原文链接**: [https://www.cidrap.umn.edu/childhood-vaccines/fda-official-proposes-impossible-standards-vaccine-testing-could-curtail-access](https://www.cidrap.umn.edu/childhood-vaccines/fda-official-proposes-impossible-standards-vaccine-testing-could-curtail-access)

生成摘要时出错

---

## 96. Tesla Model Y named worst car for reliability in Germany's major TÜV report

**原文标题**: Tesla Model Y named worst car for reliability in Germany's major TÜV report

**原文链接**: [https://electrek.co/2025/12/03/tesla-model-y-named-worst-car-for-reliability-germany-major-tuv-report/](https://electrek.co/2025/12/03/tesla-model-y-named-worst-car-for-reliability-germany-major-tuv-report/)

生成摘要时出错

---

## 97. Why won't Steam Machine support HDMI 2.1?

**原文标题**: Why won't Steam Machine support HDMI 2.1?

**原文链接**: [https://arstechnica.com/gaming/2025/12/why-wont-steam-machine-support-hdmi-2-1-digging-in-on-the-display-standard-drama/](https://arstechnica.com/gaming/2025/12/why-wont-steam-machine-support-hdmi-2-1-digging-in-on-the-display-standard-drama/)

生成摘要时出错

---

## 98. Advent of Code 2025: The AI Edition – By Peter Norvig

**原文标题**: Advent of Code 2025: The AI Edition – By Peter Norvig

**原文链接**: [https://github.com/norvig/pytudes/blob/main/ipynb/Advent-2025-AI.ipynb](https://github.com/norvig/pytudes/blob/main/ipynb/Advent-2025-AI.ipynb)

生成摘要时出错

---

## 99. Berlin: Police can secretly enter homes for state trojan installation

**原文标题**: Berlin: Police can secretly enter homes for state trojan installation

**原文链接**: [https://www.heise.de/en/news/Berlin-Police-can-secretly-enter-homes-for-state-trojan-installation-11103284.html](https://www.heise.de/en/news/Berlin-Police-can-secretly-enter-homes-for-state-trojan-installation-11103284.html)

生成摘要时出错

---

## 100. The Debug Adapter Protocol is a REPL protocol in disguise

**原文标题**: The Debug Adapter Protocol is a REPL protocol in disguise

**原文链接**: [https://zignar.net/2025/06/23/debug-adapter-protocol-is-a-repl-protocol/](https://zignar.net/2025/06/23/debug-adapter-protocol-is-a-repl-protocol/)

生成摘要时出错

---

