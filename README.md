# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2025-11-19.md)

*最后自动更新时间: 2025-11-19 20:09:54*
## 1. Cloudflare 全球网络发生故障

**原文标题**: Cloudflare Global Network experiencing issues

**原文链接**: [https://www.cloudflarestatus.com/incidents/8gmgl950y3h7](https://www.cloudflarestatus.com/incidents/8gmgl950y3h7)

2025年11月18日，Cloudflare的全球网络经历了一次严重中断，影响了包括Access、Bot Management、CDN/Cache、Dashboard、Firewall、Network、WARP和Workers在内的众多服务。该事件始于世界标准时间11:48左右，当时出现内部服务性能下降。

当天，Cloudflare工程师们致力于识别并解决该问题。最初的影响包括间歇性服务中断，以及暂时禁用了伦敦地区的WARP访问。到世界标准时间13:09，根本问题被确定，并启动了修复。

服务恢复是渐进的：Cloudflare Access和WARP在世界标准时间13:13恢复，Dashboard服务在世界标准时间14:34恢复。尽管有所改善，但随着团队在全球网络中清除了剩余问题，间歇性错误、延迟升高以及对机器人评分的影响持续了数小时。

到世界标准时间17:44，Cloudflare确认服务已正常运行，错误和延迟已恢复到事件发生前的水平。该事件于世界标准时间19:28正式解决。Cloudflare目前正在进行更深入的事件后调查，并很快将提供一份完整的报告，建议用户可以安全地重新启用任何暂时禁用的服务。

---

## 2. 双子星3号

**原文标题**: Gemini 3

**原文链接**: [https://blog.google/products/gemini/gemini-3/](https://blog.google/products/gemini/gemini-3/)

谷歌发布了Gemini 3，并将其誉为其最智能的AI模型，标志着“智能新时代”的开启。现已推出的Gemini 3 Pro版本在推理、多模态理解和智能体能力方面取得了显著进步，在LMArena、人类的期末考试、GPQA Diamond以及各种编码和多模态测试等主要AI基准测试中，其性能均超越了2.5 Pro等之前的模型。

Gemini 3旨在实现深度和细微理解，更有效地洞察用户意图，并提供更丰富的可视化效果和交互式体验。它致力于赋能用户“学习、构建和规划任何事物”。其应用涵盖解读手写食谱、分析运动表现，到生成复杂的网页用户界面，并通过在Google Antigravity（一个新型智能体开发平台）等平台上进行“氛围编码”来促进自主软件开发。它还在多步骤任务的长期规划方面表现出更强的能力。

一种增强的推理模式Gemini 3 Deep Think，进一步拓展了智能的边界，并将在额外的安全评估后，很快向Google AI Ultra订阅者开放。Gemini 3正立即在谷歌产品中全面推出，包括Gemini应用、搜索中的AI模式、AI Studio和Vertex AI。谷歌强调了Gemini 3的全面安全评估，将其定位为迄今为止最安全的模型。此次发布标志着Gemini 3时代的开启，预计未来还将推出更多模型。

---

## 3. Cloudflare 2025年11月18日故障复盘

**原文标题**: Cloudflare outage on November 18, 2025 post mortem

**原文链接**: [https://blog.cloudflare.com/18-november-2025-outage/](https://blog.cloudflare.com/18-november-2025-outage/)

2025年11月18日，Cloudflare遭遇了一次大范围中断，从协调世界时11:20开始，导致其网络出现重大故障和HTTP 5xx错误。此次事件并非网络攻击，而是源于ClickHouse数据库系统权限的一次内部更改。

这次权限更新导致一个用于为Cloudflare的机器人管理系统生成“特征文件”的查询返回了重复条目。结果，该特征文件大小翻倍。当这个过大的文件在网络中传播时，对该文件有预分配内存限制的核心代理软件（FL2）遇到了一个未处理的错误并崩溃，从而触发了5xx错误。

最初的诊断因错误率波动以及Cloudflare外部状态页面的巧合性中断而受阻，导致一些人最初怀疑是DDoS攻击。此次中断影响了核心CDN和安全服务、Turnstile、Workers KV、Dashboard登录功能以及Cloudflare Access认证。

工程师们确定了根本原因，停止了问题特征文件的传播，手动插入了一个已知正常版本，并重启了核心代理。核心流量在协调世界时14:30前基本恢复，所有系统于协调世界时17:06恢复正常运行。Cloudflare对此次影响表示歉意，并承诺加强内部生成的配置文件摄取流程，以防止未来再次发生此类事件。

---

## 4. 谷歌反重力

**原文标题**: Google Antigravity

**原文链接**: [https://antigravity.google/](https://antigravity.google/)

“Google反重力”页面（antigravity.google）是一个幽默且富有想象力的“即将推出”公告，旨在介绍一个概念性的谷歌项目，该项目专注于反重力技术。

该网站的主要信息是一个醒目的“即将推出”，旁边伴随着俏皮的声明：“重力，我们有麻烦了。”一个交互式搜索栏进一步强化了该页面的讽刺性质，因为尝试使用它时会显示信息：“抱歉，我们还没到那一步……”

该页面没有提供任何具体信息、技术细节或实际产品的时间表，而是以轻松愉快的方式探讨了一个革命性的概念。它邀请用户“了解Project ZeroG”，这会重定向到一个关于“零重力”的标准谷歌搜索；并邀请用户通过电子邮件注册表单“获取更新”。总体基调强烈暗示，“Google反重力”页面是一个讽刺性的或概念性的作品，一个互联网彩蛋，或一个非常长期、推测性的品牌参与，而不是一个严肃的产品或技术公告。它以谷歌特有的幽默感，凸显了这种壮举的不可能。

---

## 5. Blender 5.0

**原文标题**: Blender 5.0

**原文链接**: [https://www.blender.org/download/releases/5-0/](https://www.blender.org/download/releases/5-0/)

Blender 5.0 引入了重大进展，专注于艺术控制、行业标准工作流程和性能。一个主要亮点是**光照链接（Light Linking）**，使艺术家能够精确控制哪些灯光照亮特定物体，在场景照明中提供前所未有的创作自由。

**色彩管理系统进行了全面改革**，采用 OpenColorIO (OCIO) 并以 ACES 作为默认配置。这使 Blender 与专业生产流程保持一致，确保色彩呈现的一致性和准确性。

动画工作流程通过**动画系统改革**得到了显著增强，包括新的关键帧集、改进的曲线编辑器性能，以及专用的动画播放器，以实现更流畅的播放。**视口合成器（Viewport Compositor）性能显著提升**，允许更快的实时合成。

渲染方面的改进包括 **Eevee 和 Cycles 的优化**，其中 Eevee 的毛发渲染得到改善，整体性能也有所提升。**几何节点（Geometry Nodes）获得新功能**，具有更灵活的节点工具。此版本还包括**新的Relax雕刻笔刷**、众多用户界面优化以及**各个领域的整体性能改进**，使 Blender 5.0 成为 3D 艺术家更强大、更高效的工具。

---

## 6. 丽贝卡·海涅曼去世

**原文标题**: Rebecca Heineman has died

**原文链接**: [https://www.pcgamer.com/gaming-industry/legendary-game-designer-programmer-space-invaders-champion-and-lgbtq-trailblazer-rebecca-heineman-has-died/](https://www.pcgamer.com/gaming-industry/legendary-game-designer-programmer-space-invaders-champion-and-lgbtq-trailblazer-rebecca-heineman-has-died/)

知名游戏开发者丽贝卡·海涅曼（Rebecca Heineman）逝世，享年62岁。此前，她在上个月被诊断出患有侵袭性癌症后，健康状况迅速恶化。她的死讯由一位朋友在Bluesky上证实，并在她的GoFundMe页面上发布了最后一条消息。该页面将继续保持活跃，以支持她的家人处理后事。

海涅曼是业界真正的先驱。1980年，她通过赢得全国性的《太空入侵者》（Space Invaders）锦标赛，成为美国首位获得官方认可的电子游戏冠军，从而在业界崭露头角。1983年，她共同创立了Interplay，这家举足轻重的开发商和发行商推出了《废土》（Wasteland）、《辐射》（Fallout）和《博德之门》（Baldur's Gate）等奠基性的PC游戏。在Interplay，她设计并编程了许多游戏，其中最著名的当属《吟游诗人故事3：命运盗贼》（The Bard's Tale 3: Thief of Fate）。后来，她因在数周内独自完成了《毁灭战士》（Doom）的3DO移植版编程而获得了传奇地位。

在21世纪初公开以跨性别者身份亮相的海涅曼，其伴侣是同样的游戏界传奇人物珍内尔·雅奎斯（Jennell Jaquays），雅奎斯已于2024年1月去世。海涅曼因其对LGBTQ+包容性和多样性的倡导，被授予Gayming 2025年度Gayming标志性人物奖。包括Interplay联合创始人布莱恩·法戈（Brian Fargo）在内的朋友和同事纷纷致敬，称赞她是其中一位最杰出的程序员，一个善良、鼓舞人心，并给游戏界留下不可磨灭印记的灵魂。

---

## 7. 几乎所有英国司机都表示车头灯太亮了

**原文标题**: Nearly all UK drivers say headlights are too bright

**原文链接**: [https://www.bbc.com/news/articles/c1j8ewy1p86o](https://www.bbc.com/news/articles/c1j8ewy1p86o)

英国交通部（DfT）委托进行的一项最新研究显示，几乎所有英国司机（97%）经常或偶尔会被迎面而来的车灯分散注意力，其中96%的司机认为车灯太亮。这项由交通研究实验室（TRL）进行的研究提供了“令人信服的证据”，表明车灯眩光是“英国司机面临的一个真正问题”。

该研究将这一问题与LED和更白的头灯联系起来，这些头灯更亮、更集中，并发出更多的蓝光，使人眼在夜间更难适应。这种眩光严重影响了驾驶习惯；33%的受访司机已停止或减少夜间驾驶，而22%的司机希望如此，但别无选择。

作为回应，政府宣布将审查汽车和头灯设计，并将新措施纳入其即将发布的《道路安全战略》中。RAC（英国皇家汽车俱乐部）对研究结果表示欢迎，主张在有效照明和防止司机炫目之间取得平衡。英国验光师学院敦促英国交通部立即采取行动，并委托进行进一步研究，以修订头灯法规。

---

## 8. Windows 11 新增后台运行并可访问个人文件夹的 AI 代理。

**原文标题**: Windows 11 adds AI agent that runs in background with access to personal folders

**原文链接**: [https://www.windowslatest.com/2025/11/18/windows-11-to-add-an-ai-agent-that-runs-in-background-with-access-to-personal-folders-warns-of-security-risk/](https://www.windowslatest.com/2025/11/18/windows-11-to-add-an-ai-agent-that-runs-in-background-with-access-to-personal-folders-warns-of-security-risk/)

微软正在将一项实验性的“Agent Workspace”功能整合到 Windows 11 中，尽管遭到用户反对，但这标志着向“AI原生”操作系统迈出了重要一步。此功能允许 AI 代理在后台运行，拥有自己的运行时、桌面和用户账户。

一旦 Windows 预览体验成员（开发版/Beta 版频道）通过“实验性代理功能”启用此功能，Agent Workspace 将授予 AI 代理对桌面、音乐、图片和视频等重要个人文件夹以及已安装应用程序的读写访问权限。这些代理旨在模仿人类交互，通过操作应用程序和文件，代表用户执行任务。

与提供完全隔离并在关闭时删除所有活动的 Windows 沙盒不同，Agent Workspace 虽然也是隔离且可审计的，但它明确允许代理访问和修改用户文件。微软声称该功能比完整的虚拟机更高效，并强调正在持续改进其透明度、安全性和用户控制。每个代理都可以有预定义的访问规则，并且该功能是可选的，默认不启用。

鉴于对个人数据的广泛访问权限以及代理在后台持续运行可能带来的性能影响，安全担忧依然存在。尽管用户群体对这种“代理式”转变提出了批评，微软领导层仍致力于在 Windows 11 中深入投资 AI，这表明以 AI 为中心的操作系统是其未来的发展方向。

---

## 9. 核心设备老是窃取我们的成果。

**原文标题**: Core Devices keeps stealing our work

**原文链接**: [https://rebble.io/2025/11/17/core-devices-keeps-stealing-our-work.html](https://rebble.io/2025/11/17/core-devices-keeps-stealing-our-work.html)

Rebble是一个在过去九年里致力于维护Pebble智能手表生态系统的社区组织，指控Eric Migicovsky的新公司Core Devices试图窃取他们的工作成果和知识产权。Rebble声称，在Pebble Technology Corporation倒闭后，他们投入数十万美元和巨大精力，独自挽救并重建了Pebble应用商店及其他关键服务。Rebble表示，Core Devices目前提供的“Pebble应用商店”完全是他们的心血结晶。

Rebble声称Core Devices要求无限制地访问他们过去十年的所有工作成果和数据。尽管最初达成了合作协议，但据报道，Core拒绝提供书面承诺，保证他们不会利用Rebble的数据来构建一个专有的“围墙花园”式应用商店，从而将社区和Rebble本身边缘化。Core还被指控违反协议抓取Rebble的应用商店数据，在未合并回贡献的情况下分叉了Rebble资助的开源固件（PebbleOS），并以更严格的许可使用Rebble的移动应用组件。

Rebble的“红线”是为其社区驱动平台确保一个有保障的未来。他们倾向于Core能与Rebble合作，共同利用Rebble的服务。面对僵局，Rebble现在正在征求社区的意见，是在法律上保护他们的工作，还是允许Core无限制使用。他们强调，他们偏好的结果是Core做出明确的法律承诺，以合作伙伴身份进行合作。Rebble正在积极征集社区关于如何继续的反馈。

---

## 10. 我将卸任 Mastodon 首席执行官

**原文标题**: I am stepping down as the CEO of Mastodon

**原文链接**: [https://blog.joinmastodon.org/2025/11/my-next-chapter-with-mastodon/](https://blog.joinmastodon.org/2025/11/my-next-chapter-with-mastodon/)

Mastodon首席执行官在近10年后卸任，将商标和资产的所有权转让给Mastodon非营利组织。这一决定旨在维护项目的价值观和社区，防止潜在的创始人驱动的陷阱，并与其技术的去中心化性质保持一致。

即将离任的首席执行官以个人原因为由离职，强调了领导社交媒体项目的巨大压力，以及其性格不适合面对公众审视。他们描述了不切实际的期望、与没有相应资源的富有科技亿万富翁进行比较的负担，以及微小批评所造成的消耗。去年夏天一次特别负面的用户互动成为催化剂，促使他们意识到需要与项目建立更健康的关系。

回顾自己的成就，这位首席执行官强调了坚持说“不”以保持专注的关键作用，并承认不喜公开露面可能让他们错失了宣传机会。尽管如此，他们对Mastodon从一个“简陋的项目”发展成为一个蓬勃发展的、以社区为中心的平台感到无比自豪。

出于对Mastodon和“联邦宇宙”（被视为“日益反乌托邦的资本主义地狱中的一座孤岛”）的深厚热情，这位前首席执行官将以不那么公开的顾问身份继续参与其中，相信这代表着通往更美好未来的重要途径。

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 2 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 3 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 4 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 5 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 6 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 7 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 8 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 9 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 10 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 11 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 12 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 13 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
| 14 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
