# Hacker News 热门文章摘要 (2025-11-20)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. Cloudflare 2025年11月18日故障复盘

**原文标题**: Cloudflare outage on November 18, 2025 post mortem

**原文链接**: [https://blog.cloudflare.com/18-november-2025-outage/](https://blog.cloudflare.com/18-november-2025-outage/)

2025年11月18日，Cloudflare发生了一次严重的网络中断，始于UTC时间11:20，大部分问题于UTC时间14:30解决，所有系统于UTC时间17:06恢复正常。此事件导致用户访问客户网站时出现普遍的HTTP 5xx错误，并影响了核心CDN、安全服务、Workers KV、Turnstile、控制面板登录和Access身份验证。

此次中断并非网络攻击。它源于UTC时间11:05在ClickHouse集群中发生的数据库权限变更。这一变更无意中导致一个由Bot管理系统使用的查询将重复条目输出到其“特征文件”中，使其大小翻倍。

当这个过大的特征文件传播到Cloudflare网络中时，负责流量路由的软件（该软件对该文件有内存预分配限制，即200个特征）遇到了超出预期大小的文件。这触发了软件恐慌和故障，导致服务中断。

最初的症状，包括波动的错误率以及Cloudflare*外部*状态页面恰好中断，最初让团队怀疑是超大规模DDoS攻击。在正确识别出核心问题后，Cloudflare停止了错误特征文件的生成和传播，手动插入了一个已知的良好版本，并强制进行了核心代理重启。Workers KV于UTC时间13:04被修补以绕过核心代理，控制面板的可用性于UTC时间15:30恢复。Cloudflare对此次重大影响表示歉意，并正在实施后续措施以强化系统，防止发生类似故障。

---

## 2. Blender 5.0

**原文标题**: Blender 5.0

**原文链接**: [https://www.blender.org/download/releases/5-0/](https://www.blender.org/download/releases/5-0/)

Blender 5.0 是一个重要版本，专注于优化用户体验、提升性能并在其各个领域引入强大的新功能。

主要亮点包括：

*   **渲染：** Cycles 引入了**光照链接**，让艺术家能够精确控制哪些灯光照亮特定物体，以及实验性的**光谱渲染**，用于实现高精度的光照交互。GPU 光线追踪性能也得到了进一步优化。EEVEE 和视图受益于改进的光照、更高质量的体积渲染，并新增了**视口合成器**，可在实时进行直接合成。
*   **建模：** “挤出流形”等新工具以及对阵列修改器的全面改进，简化了网格编辑和创建工作流程。
*   **动画与绑定：** 强大的新**姿态库**提供了一个直观的系统，用于存储和重用角色姿态。动画功能通过改进的运动路径工具和对 NLA 编辑器的更新得到进一步增强。
*   **节点：** 几何节点获得了显著的性能提升和新功能，包括引入了**模拟节点**，用于创建动态效果。
*   **用户界面与体验：** 该版本包含众多 UI 改进，例如改进的字体渲染、增强的色彩管理和更快的启动时间，有助于实现更灵敏、更愉悦的工作流程。
*   **性能：** 整个软件的整体性能都有显著提升，使 Blender 5.0 在各方面都更快、更稳定。

---

## 3. 欧洲缩减GDPR并放松人工智能法规

**原文标题**: Europe is scaling back GDPR and relaxing AI laws

**原文链接**: [https://www.theverge.com/news/823750/european-union-ai-act-gdpr-changes](https://www.theverge.com/news/823750/european-union-ai-act-gdpr-changes)

欧洲正在放宽其具有里程碑意义的《通用数据保护条例》（GDPR），并放宽或推迟其人工智能法律（包括《人工智能法案》）的关键要素。此举是在科技巨头、美国政府以及马里奥·德拉吉等欧盟内部人士的巨大压力下作出的，因为布鲁塞尔旨在削减繁文缛节、恢复疲软的经济增长，并解决其在人工智能竞赛中全球竞争力方面的担忧。

由欧盟委员会提出的这些修改包括：简化GDPR无处不在的Cookie许可弹窗，使公司更容易共享匿名化和假名化的个人数据集，以及允许人工智能公司在特定条件下合法使用个人数据来训练人工智能模型。

关于《人工智能法案》，该提案延长了针对“高风险”人工智能系统的规则的宽限期，这些规则现在只有在必要的标准和支持工具可用后才会实施。“数字综合法案”中的其他修正案包括：简化小型公司的人工智能文档要求、统一的网络安全事件报告界面，以及将欧盟内部的人工智能监管集中到其人工智能办公室。

欧盟委员会将这些调整描述为“简化欧盟法律”和促进创新，同时声称保护用户的基本权利。然而，该提案预计将面临公民权利团体和政界人士的强烈反对，他们指责欧盟委员会削弱了保障措施。这些修改现在将提交给欧洲议会和成员国批准，这个过程可能在未来几个月内引入重大修改。

---

## 4. 元万物分割模型 3

**原文标题**: Meta Segment Anything Model 3

**原文链接**: [https://ai.meta.com/sam3/](https://ai.meta.com/sam3/)

Meta发布了Segment Anything Model 3 (SAM-3)，标志着通用图像分割领域的一项重大进展。这一新版本在基础的SAM和SAM-2之上进一步发展，旨在对海量视觉数据中的物体进行更细粒度、更精确的描绘。

SAM-3强调对图像中任何物体进行高质量分割，无论其新颖性、纹理或背景复杂程度如何。主要改进包括在区分细粒度细节以及处理遮挡或低对比度区域等挑战性场景方面增强的准确性。该模型在扩展且更多样化的数据集上进行训练，这有助于其在不同图像类型和领域中展现出强大的泛化能力。

Meta强调SAM-3有潜力赋能广泛的AI应用，从改进的计算机视觉系统和增强现实体验，到高级图像编辑和内容创作工具。其以更高精度“分割万物”的能力，预计将加速需要详细场景理解领域的研发。

此次发布凸显了Meta对开放科学的承诺，使研究人员和开发者能够使用SAM-3，以促进AI社区的创新。这一迭代延续了提供理解视觉信息基础工具的使命，不断拓展自动化图像分割的可能边界。

---

## 5. HN 展示：我制作了一个宕机检测器的宕机检测器

**原文标题**: Show HN: I made a down detector for down detector

**原文链接**: [https://downdetectorsdowndetector.com](https://downdetectorsdowndetector.com)

一位Hacker News用户开发了一款监控工具，专门用于检查downdetector.com自身的运行状态。该项目被称为“downdetector的宕机探测器”，旨在解决一个旨在报告服务中断的网站自身也可能出现中断的讽刺局面。

该工具提供实时状态更新，详细列出不同地区的HTTP响应和延迟指标，以确保全面监控。其目的是确认downdetector.com从不同地理位置是否可访问并正常运行，实质上是为这个可靠性检查器提供了一层保障。

---

## 6. 专利局即将让劣质专利无法被撼动。

**原文标题**: The patent office is about to make bad patents untouchable

**原文链接**: [https://www.eff.org/deeplinks/2025/11/patent-office-about-make-bad-patents-untouchable](https://www.eff.org/deeplinks/2025/11/patent-office-about-make-bad-patents-untouchable)

美国专利商标局 (USPTO) 提出了新规定，这将严重削弱当事人间复审 (IPR)，从而实际终结公众在专利局内部质疑不当授权专利的能力。此举被批评为通过使劣质专利无法被挑战来赋能“专利流氓”，使被诉方几乎没有经济实惠的辩护选择。

IPR 由专利审判和上诉委员会 (PTAB) 裁决，是挑战专利的关键、相对经济且更快捷的替代方案，可替代昂贵的联邦法院诉讼。它已成功宣告无效了诸如“播客专利”和SportBrain数据上传专利等问题专利，造福了整个行业。

拟议的新规带来了三项危险的改变：
1.  **强制选择：** 被告必须放弃在法庭上质疑专利有效性，才能使用IPR。
2.  **“不可挑战”的专利：** 即使之后出现新证据，一项专利在仅进行一次先前的有效性争议后，也可能对IPR免疫。
3.  **地方法院优先：** 如果预计地方法院案件进展更快，IPR将被阻止，从而迫使被告卷入昂贵且长达数年的诉讼。

USPTO声称地方法院的挑战是足够的，这具有误导性，因为此类诉讼耗资数百万美元，且大多数人难以负担。批评者认为，这些规定违背了国会设立IPR的初衷，即提供一个便捷的途径来纠正专利局的错误。

电子前沿基金会 (EFF) 敦促公众在12月2日前发表评论，反对这些规定，并强调公众有权挑战劣质专利以保护创新。

---

## 7. 纳米香蕉 Pro

**原文标题**: Nano Banana Pro

**原文链接**: [https://blog.google/technology/ai/nano-banana-pro/](https://blog.google/technology/ai/nano-banana-pro/)

Google DeepMind推出了Nano Banana Pro，这是一款由Gemini 3 Pro提供支持的全新最先进图像生成和编辑模型。该版本在之前的Nano Banana模型基础上，利用Gemini 3增强的推理能力和真实世界知识，提供更准确、更富上下文的视觉内容。

Nano Banana Pro擅长可视化想法，通过Google搜索从笔记或实时数据创建信息图表，以及生成图表。一个突出特点是它能够生成带有准确渲染且清晰可读的多语言文本的图像，支持多种字体、纹理和本地化，适用于模型图和国际内容。

该模型还提供了升级的创意控制，用于生成高保真视觉效果。用户可以通过混合多达14张图像并保留多达5个人的肖像相似度来保持品牌一致性。高级编辑功能包括局部调整、摄像机角度更改、焦点控制、精密的色彩分级、场景光照变换（例如，白天到夜晚），以及在各种宽高比下输出高达4K的分辨率。

Nano Banana Pro正被整合到谷歌的生态系统之中。消费者和学生可以在Gemini应用、搜索中的AI模式（针对订阅用户）和NotebookLM中访问它。专业人士将在Google Ads和Workspace（Slides、Vids）中找到它，而开发者和企业则可以通过Gemini API、Google AI Studio、Google Antigravity和Vertex AI使用它。创作者可以在Flow中利用它。

所有生成的媒体都嵌入了不可察觉的SynthID数字水印，以保持透明度，Gemini应用可以识别谷歌AI创建的图像。免费和Google AI Pro等级用户还将看到一个可见的“Gemini闪光”水印，该水印对Ultra订阅用户和在Google AI Studio中用于专业用途时会被移除。

---

## 8. Linux游戏从未如此易于上手。

**原文标题**: Gaming on Linux has never been more approachable

**原文链接**: [https://www.theverge.com/tech/823337/switching-linux-gaming-desktop-cachyos](https://www.theverge.com/tech/823337/switching-linux-gaming-desktop-cachyos)

Nathan Edwards，一位资深评测编辑，正将其主要游戏电脑从Windows 11切换到Linux，原因是对微软日益侵扰的功能感到沮恼，包括Recall、Copilot、持续推送Edge浏览器以及强制硬件升级。他认为Windows正变得越来越烦人，并且不会有所改善。

尽管他有长达数十年的Windows使用历史，且之前使用Linux的经验大多充满挑战（例如，树莓派、WSL问题），Edwards仍认为现在是做出改变的最佳时机。Valve在Steam Deck上的努力显著改善了Linux上的游戏体验，使其成为一个可行的替代方案，在某些运行基于Fedora的发行版（如Bazzite）的掌机上表现出更好的性能。

Edwards计划在他的高端台式电脑上安装CachyOS，这是一个基于Arch、针对现代游戏硬件优化的发行版，该电脑配备了AMD Ryzen 7 9800X3D和Nvidia GeForce RTX 4070 Super。他预计会遇到困难，因为他的Linux专业知识有限，且Linux在PC游戏领域的市场份额很小（约占Steam用户的3%），但他已准备好频繁查阅论坛和进行故障排除。鉴于有备用机器用于工作，他将这一学习过程视为对其自由时间的宝贵利用，并且好奇他究竟会成为“革命的先知”，还是最终回归Windows。

---

## 9. 人工智能是集中资源和权力的幌子。

**原文标题**: AI is a front for consolidation of resources and power

**原文链接**: [https://www.chrbutler.com/what-ai-is-really-for](https://www.chrbutler.com/what-ai-is-really-for)

作者认为AI被严重过分炒作，可能形成一场灾难性的金融泡沫。借鉴他作为设计师和AI初创公司联合创始人的经验，他发现AI对于信息整合等小型、独立任务是有效的，但对于大型的端到端工作流程来说，它在很大程度上是低效且不切实际的，往往事倍功半。这与企业界普遍期望的全面、统一的变革相悖。

他指出，当前的AI市场与过去的泡沫（如互联网泡沫、赛格威）如出一辙，但规模空前，投资集中在少数相互依赖的公司，这些公司缺乏与其估值相称的可行变现模式。除了经济考量之外，生成式AI还带来了严重的社会风险，使得更快、更精准的操控成为可能，从而侵蚀真相和信任。

作者质疑向亿万富翁投资者兜售的AGI（通用人工智能）承诺，认为它只是一种抽象的幻想，而非一个连贯的科学目标。他的核心理论是，AI泡沫实际上是整合土地、能源和水资源（即AI所需的大规模数据中心的关键资源）的幌子。这些基础设施项目赋予了私人公司巨大的政治和经济权力，创造了一种“私有主义”（Privatism），在这种主义下，对关键资源的控制权比AI本身的功能成功更为重要。

最终，作者担心支撑AI的基础设施将变得比AI本身更有价值，从而将巨大的权力从民选政府手中转移到少数私人实体，从根本上改变社会。

---

## 10. 用 GPT-5.1-Codex-Max 构建更多

**原文标题**: Building more with GPT-5.1-Codex-Max

**原文链接**: [https://openai.com/index/gpt-5-1-codex-max/](https://openai.com/index/gpt-5-1-codex-max/)

无法访问文章链接。

---

## 11. 你的智能手机，他们的规矩：应用商店助长政企审查

**原文标题**: Your smartphone, their rules: App stores enable corporate-government censorship

**原文链接**: [https://www.aclu.org/news/free-speech/app-store-oligopoly](https://www.aclu.org/news/free-speech/app-store-oligopoly)

文章《你的智能手机，他们的规则：应用商店如何助长企业和政府审查》指出，苹果AppStore和谷歌Play商店的双头垄断使得政府和企业能够审查并控制用户在其移动设备上可以做的事情。

美国公民自由联盟（ACLU）的作者丹尼尔·卡恩·吉尔莫（Daniel Kahn Gillmor）强调了一些案例，例如苹果和谷歌应美国司法部要求下架了“ICEBlock”和“Red Dot”两款应用，这两款应用允许匿名举报移民及海关执法局（ICE）的特工。这被视为政府利用应用商店的集中控制权进行的越权行为。

苹果的iOS系统天生将用户限制在其AppStore中，这赋予了该公司巨大的权力，具体表现在其对中国审查制度的顺从（例如，禁止同性恋约会应用），以及阻止批评其做法或涉及商业纠纷的应用（例如，Fortnite）。尽管安卓系统传统上允许“侧载”（从Play商店外部安装应用），但谷歌即将推出的“验证开发者”要求威胁了这一自由，可能允许政府通过要求将某个开发者“取消验证”来实施类似的滥用行为。

文章还质疑了应用商店的安全声明，指出它们允许大量具有高监控性质的应用存在，而其政策却可能危及那些专注于隐私的端到端加密应用。两个应用商店也都进行着大量的用户监控。

作为替代方案，文章提到了Accrescent和F-Droid等保护隐私的安卓应用商店，但警告称谷歌的改变可能会限制它们的可用性。文章建议通过用户选择、开放标准和监管干预来对抗这种集中控制，引用了欧盟的《数字市场法案》（DMA），该法案强制苹果在欧洲允许替代应用商店和侧载，尽管苹果通过“公证”机制仍保留了一些控制权。最终目标是用户对其设备的控制权，而不是企业或政府的强制规定。

---

## 12. 雷鸟新增原生微软Exchange邮件支持

**原文标题**: Thunderbird adds native Microsoft Exchange email support

**原文链接**: [https://blog.thunderbird.net/2025/11/thunderbird-adds-native-microsoft-exchange-email-support/](https://blog.thunderbird.net/2025/11/thunderbird-adds-native-microsoft-exchange-email-support/)

Thunderbird 最新月度版本 145（2025 年 11 月 18 日）现已通过 Exchange Web Services (EWS) 协议原生支持 Microsoft Exchange 电子邮件。此更新消除了在 Exchange 环境中使用第三方附加组件或 IMAP/POP 协议发送电子邮件的需要，简化了偏爱 Thunderbird 的用户的使用体验。

现在支持的关键功能包括完整的文件夹列表、邮件同步、文件夹管理、附件处理以及搜索/筛选。Microsoft 365/Office 365 账户的设置十分简单，采用 Microsoft 标准的 OAuth2 登录流程和自动账户检测。对于本地 Exchange 账户，也支持基于密码的基本身份验证。

尽管电子邮件集成已完成，但 Exchange 账户的日历和通讯录支持正在积极规划中，将在未来版本中推出。同样，高级身份验证配置（例如本地部署的 NTLM 和 OAuth2，以及特定域的自定义 OAuth2）也在计划中。

Thunderbird 承认 Microsoft 正在逐步从 EWS 转向 Microsoft Graph。尽管 EWS 支持优先考虑了现有用户，但目前正在努力集成 Microsoft Graph，以确保未来的兼容性。这种原生的 Exchange 电子邮件支持是使 Thunderbird 成为 Exchange 用户 Outlook 的全面而强大替代方案的重要一步。

---

## 13. 阿杜诺之死？

**原文标题**: The Death of Arduino?

**原文链接**: [https://www.linkedin.com/posts/adafruit_opensource-privacy-techpolicy-activity-7396903362237054976-r14H](https://www.linkedin.com/posts/adafruit_opensource-privacy-techpolicy-activity-7396903362237054976-r14H)

Adafruit工业报告称，高通旗下的Arduino已悄然对其服务条款和隐私政策进行了全面修订，这从根本上背离了其开放硬件理念。

据报道，新政策包括：
*   对用户上传内容拥有不可撤销的永久许可。
*   针对AI功能进行广泛的监控式监测。
*   一项阻止用户识别潜在专利侵权的条款。
*   即使在账户删除后，用户名仍保留数年。
*   将所有用户数据（包括未成年人）整合到高通的全球数据生态系统。
*   明确禁止用户未经许可对平台进行逆向工程或了解其运作方式。

Adafruit认为，这些变化将Arduino从一个开放的社区平台转变为一个严格受控、专注于深度数据提取的企业服务，这对于一个深受教育工作者、创客和开源倡导者喜爱的品牌来说，是一个深刻的转变。该帖子还批评了高通的企业做法及其与创客社区的明显脱节。

评论反映了普遍的沮丧，许多人宣称“Arduino安息吧”。用户预见到这将对学术机器人研究和更广泛的创客领域造成重大打击。许多评论者建议迁移到RP2040和ESP32等替代开源平台，或使用结合PlatformIO的VSCode等工具，预测社区将找到新的、真正开放的解决方案。普遍的共识是，高通误解了开源精神，此举最终将有利于竞争性开源项目。

---

## 14. 电线松动致停电，碰撞弗朗西斯·斯科特·基大桥

**原文标题**: Loose wire leads to blackout, contact with Francis Scott Key bridge

**原文链接**: [https://www.ntsb.gov:443/news/press-releases/Pages/NR20251118.aspx](https://www.ntsb.gov:443/news/press-releases/Pages/NR20251118.aspx)

“达利”号集装箱船上的一根松动的电线导致停电，进而造成该船撞上巴尔的摩的弗朗西斯·斯科特·基大桥。

---

## 15. GitHub：Git 操作失败

**原文标题**: GitHub: Git operation failures

**原文链接**: [https://www.githubstatus.com/incidents/5q7nmlxz30sk](https://www.githubstatus.com/incidents/5q7nmlxz30sk)

2025年11月18日，GitHub在UTC时间20:30至21:34期间发生了一起名为“Git操作故障”的事件。此次中断影响了所有Git操作，包括SSH和HTTP客户端交互、原始文件访问以及依赖Git的产品。GitHub Codespaces的可用性也出现下降。

事件的根本原因是一个用于内部服务间通信的TLS证书过期。GitHub通过替换过期证书并重启受影响的服务，成功缓解了该问题，从而实现了全面恢复。

事件发生后，GitHub已更新其告警系统以覆盖过期证书，并正在对同一领域的其他证书进行审计，以确保适当的告警和自动化。此外，该公司正在加快消除剩余手动管理证书的努力，旨在实现与现代安全实践相符的、完全自动化的服务间通信。

---

## 16. 萨默斯退出OpenAI董事会

**原文标题**: Larry Summers resigns from OpenAI board

**原文链接**: [https://www.cnbc.com/2025/11/19/larry-summers-epstein-openai.html](https://www.cnbc.com/2025/11/19/larry-summers-epstein-openai.html)

美国前财政部长拉里·萨默斯已从OpenAI董事会辞职，并从哈佛大学请假。此前，他与被定罪的性犯罪者杰弗里·爱泼斯坦之间的邮件被公之于众。

萨默斯此前已宣布将退出所有公共职务，他于周三证实已辞去OpenAI董事会职务。他表示感谢能获得这一机会，并对公司的潜力感到兴奋，OpenAI董事会也回应了这一感受，并肯定了他的贡献。萨默斯于2023年在该公司经历内部动荡期间加入了OpenAI董事会。

与此同时，萨默斯也从他在哈佛大学的职位上请假，他是该校荣休校长兼莫萨瓦尔-拉赫马尼中心主任。本学期余下时间他将不再授课，下学期也未安排教学任务。他的发言人表示，由于哈佛大学正在对新公开的爱泼斯坦文件中提到的人员进行审查，这一决定符合中心的最佳利益。哈佛大学此前已宣布调查萨默斯与爱泼斯坦的关系。

上周，众议院监督与政府改革委员会公布了2万多份文件，引发了对萨默斯的强烈审查。他表示对自己的行为“深感羞愧”，并为继续与爱泼斯坦保持沟通承担全部责任。这一丑闻也引起了政界人士的关注，包括前总统唐纳德·特朗普和参议员伊丽莎白·沃伦在内的政治人物呼吁进行调查。

---

## 17. AWS千刀失误

**原文标题**: A $1k AWS mistake

**原文链接**: [https://www.geocod.io/code-and-coordinates/2025-11-18-the-1000-aws-mistake/](https://www.geocod.io/code-and-coordinates/2025-11-18-the-1000-aws-mistake/)

作者是一位经验丰富的AWS用户，他讲述了一个在将大型数据集同步到S3时，因AWS数据传输成本而产生的价值1000美元的错误。尽管他正确地认为，在同一区域内EC2到S3的传输以及*传入*S3的传输是免费的，他却忽略了一个关键细节。

在部署了一个新的S3同步进程后，AWS成本异常检测系统提醒他，有超过20TB的“NAT Gateway”数据传输，在一天之内花费了900多美元。根本问题是：当VPC内的EC2实例与S3通信时，流量默认会通过VPC的NAT Gateway进行路由。这会产生每GB 0.045美元的处理费用，即使实际传输到S3的数据仍然是免费的。

解决方案是实施一个**S3的VPC网关端点**。这个特殊端点在VPC和S3之间创建了一个直接的、私有的连接，完全绕过了NAT Gateway和Internet Gateway。至关重要的是，S3的网关端点是完全免费的，既消除了按小时计费的费用，也消除了数据传输费用，并提升了性能。

吸取的关键教训包括：AWS成本异常检测系统的重要作用；在任何使用NAT Gateway的VPC中，配置S3（和DynamoDB）的VPC网关端点的必要性；以及在看似复杂的云环境中验证假设和测试成本的重要性。作者此后已审计了他的基础设施，以确保这些端点在各处都已配置，并敦促其他人也这样做，以避免类似的昂贵意外。

---

## 18. 红警2网页版

**原文标题**: Red Alert 2 in web browser

**原文链接**: [https://chronodivide.com/](https://chronodivide.com/)

《时空裂痕》（Chrono Divide）是一个粉丝项目，旨在为网页浏览器重现经典的《红色警戒2》即时战略游戏。最初仅为一项实验，现已发展成可玩的测试版，提供功能齐全的多人游戏，并支持所有原始地图。该项目的最终目标是实现与原版《红色警戒2》引擎的功能对等。

这款创新的游戏客户端可直接在您的网页浏览器中运行，无需任何额外的插件或应用程序。它拥有跨平台兼容性，支持在PC、手机和平板电脑等不同操作系统设备上游玩。主要功能包括无需端口转发的客户端-服务器模型、现代控制选项（左键或右键）、游戏回放以及强大的模组支持，许多现有《红色警戒2》模组可开箱即用。

最低系统要求包括64位操作系统/浏览器、Intel Atom Z3700+ CPU、4GB内存和Intel HD显卡。为获得最佳性能，建议使用最新版本的Google Chrome、Microsoft Edge或Safari浏览器，而应避免使用Firefox。

该项目完全依赖玩家捐款来支付基础设施成本并支持持续开发。玩家可以通过其Discord服务器加入社区并获取最新动态，并被鼓励立即试玩可用的测试版。

---

## 19. 我就想要好用的RCS消息。

**原文标题**: I just want working RCS messaging

**原文链接**: [https://wt.gd/i-just-want-my-rcs-messaging-to-work](https://wt.gd/i-just-want-my-rcs-messaging-to-work)

作者是一位精通技术的用户，日常使用安卓和iOS系统，自升级到iOS 26后，其iPhone 15 Pro上的RCS消息功能便无法正常使用。一个多月以来，该用户在T-Mobile、US Mobile和Verizon的手机线路一直卡在“等待激活...”状态，尽管在其他iPhone上运行良好。苹果公司归咎于运营商，而运营商又归咎于苹果公司，这令作者感到沮丧。

凭借其在解决复杂运营商问题方面的丰富经验（包括过去Verizon的MMS故障以及谷歌故意在自定义安卓ROM上阻止RCS），作者进行了详尽的故障排除。这包括多次恢复出厂设置、重新发行eSIM、重置网络，甚至分析设备日志。

日志揭示了一个关键错误：“UserInteractionRequired.xml的无限有效期”，该错误源自`config.rcs.mnc260.mcc310.jibecloud.net`。作者推断这指向谷歌Jibe，即美国运营商用于RCS的后端基础设施，而苹果支持部门对此一无所知，也无法协助诊断。

苹果客服拒绝协作解决故障，并在用尽标准程序后，提供了一个“免费”的主板更换。作者批评这是一种浪费时间的表面修补，它避免了解决真正的潜在软件或配置问题，作者认为苹果公司应该对此进行彻底调查并妥善解决。

---

## 20. 《凯文与霍布斯》40周年

**原文标题**: 'Calvin and Hobbes' at 40

**原文链接**: [https://www.npr.org/2025/11/18/nx-s1-5564064/calvin-and-hobbes-bill-watterson-40-years-comic-strip-lee-salem](https://www.npr.org/2025/11/18/nx-s1-5564064/calvin-and-hobbes-bill-watterson-40-years-comic-strip-lee-salem)

这篇文章旨在庆祝比尔·沃特森广受赞誉的漫画系列《卡尔文与霍布斯》问世40周年，该系列于1985年11月18日首次面世。文章强调了该漫画独特地融合了滑稽、奇幻和深刻的元素，围绕着6岁的卡尔文和他那只毛绒老虎霍布斯展开。在卡尔文生动的想象中，霍布斯变成了一个真实、机智且善于观察的伙伴。

该漫画的编辑李·塞勒姆回忆起他对该作品的“一见钟情”，赞扬其新颖、幽默和艺术性。他将卡尔文描述为一个在充满挑战的世界中穿梭的典型男孩，认为他更像汤姆·索亚而非查理·布朗。塞勒姆举例说明了该漫画的犀利智慧，例如卡尔文对在家生病时学习的看法，以及他对上帝是否存在这一问题的哲学式回应。他强调霍布斯作为卡尔文的“另一个自我”所扮演的角色，提供了平衡与评论，并强调在卡尔文（以及编辑）的视角中，霍布斯的真实性是毋庸置疑的，这对于该漫画将儿童幻想生活具象化的能力至关重要。

创作者比尔·沃特森在漫画系列问世十年后，于1995年在其人气鼎盛时期完结了该作品，他表示希望能探索更广阔的创作空间，并以更深思熟虑的节奏进行创作。此后，沃特森一直深居简出，鲜有公开作品问世。李·塞勒姆于2019年去世。

---

## 21. 研究人员发现WhatsApp安全漏洞

**原文标题**: Researchers discover security vulnerability in WhatsApp

**原文链接**: [https://www.univie.ac.at/en/news/detail/forscherinnen-entdecken-grosse-sicherheitsluecke-in-whatsapp](https://www.univie.ac.at/en/news/detail/forscherinnen-entdecken-grosse-sicherheitsluecke-in-whatsapp)

维也纳大学和SBA研究机构的研究人员在WhatsApp的联系人发现机制中发现了一个重大的隐私漏洞，使得全球35亿用户账户信息可被枚举。由于WhatsApp基础设施上缺乏足够的速率限制，这个漏洞允许每小时查询超过1亿个电话号码。

可访问的数据包括电话号码、公钥、时间戳等公开信息，以及（如果设置为公开）个人简介和头像。研究人员由此推断出用户的操作系统、账户注册时长和关联设备。更广泛的发现包括识别出该平台在官方禁用国家（例如中国、伊朗）中数百万活跃的WhatsApp账户，以及平台使用情况的人口统计数据，例如全球Android (81%) 和 iOS (19%) 设备的分布。该研究还指出，2021年Facebook数据泄露事件中近一半的电话号码在WhatsApp上仍处于活跃状态。

重要的是，该漏洞并未影响WhatsApp的端到端加密消息内容。研究人员强调，尽管消息本身是安全的，但当相关元数据被大规模收集和分析时，仍然可能带来重大的隐私风险。

研究人员负责任地向WhatsApp的运营商Meta披露了他们的发现，Meta此后已通过更严格的速率限制等对策解决了并缓解了该问题。Meta对此次合作表示认可，称该研究有助于对其新的反爬虫系统进行压力测试，并证实没有恶意利用的证据。研究人员已安全删除了所有收集到的数据。该研究的预印本已可查阅，并将于2026年在NDSS专题研讨会上发表，强调了持续独立安全研究的关键作用。

---

## 22. 如何在一个奖励疯狂的世界里保持清醒？

**原文标题**: How to stay sane in a world that rewards insanity

**原文链接**: [https://www.joanwestenberg.com/p/how-to-stay-sane-in-a-world-that-rewards-insanity](https://www.joanwestenberg.com/p/how-to-stay-sane-in-a-world-that-rewards-insanity)

文章《在一个奖励“疯狂”的世界里，如何保持清醒》指出，自2016年以来出现一个令人担忧的趋势：极端立场越来越能获得关注、影响力及社群归属，使得“两极分化成为一种增长策略”。相比之下，理性却收效甚微。

然而，这种对短期利益的追求伴随着巨大的弊端。个人成为“自身品牌的囚徒”，无法在不冒着失去自身身份和受众的风险下，改变想法或承认不确定性。这种动态导致社会无法进行细致入微的讨论或解决复杂问题，将我们推向集体的“愚蠢”。

为抵制这种拉力并保持清醒，作者提出了三项策略：
1.  **多元化你的信息摄入：** 积极摄取你不同意的、表达清晰的观点，以理解聪明人也可以持有截然相反的意见。
2.  **区分利害与真相：** 不要觉得有义务捍卫你所选一方的每一个论点；挑战那种要求不劳而获的确定性的部落逻辑。
3.  **寻找奖励谦逊的社群：** 寻找那些改变想法或承认“我不知道”是被接受的群体，培养真正的求真精神而非地位游戏。

尽管选择清醒意味着牺牲即时的影响力、触达范围以及部落舒适感，但它能带来清晰的思维、适应能力以及真诚的人际关系。作者认为，极端主义提供了一个快速的开端，却有着僵化的上限，困住了其追随者。清醒则提供了一个缓慢的开端，却有无限的成长空间，作者论证，只有在错误的时间框架下衡量时，世界才会奖励疯狂。

---

## 23. 短视频使用与认知和心理健康的关联

**原文标题**: Cognitive and mental health correlates of short-form video use

**原文链接**: [https://psycnet.apa.org/fulltext/2026-89350-001.html](https://psycnet.apa.org/fulltext/2026-89350-001.html)

抱歉，我无法提供题为“短视频使用与认知和心理健康的相关性”一文的摘要，因为文章的完整内容尚未提供。文本只显示“APA PsycNet 正在加载...”，表明文章内容本身缺失。

如果没有实际文本、研究方法、结果或讨论，就不可能识别出其要点、关键发现或结论。

如果您提供完整的文章内容，我将很乐意在要求的字数限制内为您总结。

---

## 24. 火狐 147 将支持 XDG 基本目录规范

**原文标题**: Firefox 147 Will Support the XDG Base Directory Specification

**原文链接**: [https://www.phoronix.com/news/Firefox-147-XDG-Base-Directory](https://www.phoronix.com/news/Firefox-147-XDG-Base-Directory)

Firefox 147 最终将支持 XDG 基础目录规范，解决了长达 21 年的错误报告。这一变化意味着 Firefox 今后将把其应用程序数据、配置文件和缓存资源存储在 Linux 用户主目录内的标准化位置，例如 `~/.config` 和 `~/.local/share`，而不是将所有内容都整合在 `~/.mozilla` 下。

由 FreeDesktop.org 倡导的 XDG 基础目录规范，概述了应用程序应如何放置文件的通用结构，以促进更好的组织并与其他 Linux 软件集成。请求支持此功能的错误报告于 2004 年 9 月提出。必要的更改最近已合并，从而关闭了这个长期存在的错误。Firefox 147 有望成为实现这一改进文件放置的版本。

---

## 25. 甲骨文在其3000亿美元的OpenAI交易上亏损。

**原文标题**: Oracle is underwater on its $300B OpenAI deal

**原文链接**: [https://www.ft.com/content/064bbca0-1cb2-45ab-85f4-25fdfc318d89](https://www.ft.com/content/064bbca0-1cb2-45ab-85f4-25fdfc318d89)

甲骨文公司于9月10日宣布与OpenAI达成3000亿美元的交易，导致其市值下跌3150亿美元，立即使其在这项协议上“处于亏损状态”。这一跌幅引人注目，因为同行公司和市场指数保持稳定。

文章解释说，甲骨文正在进行一项重大的举债投资，以建设数据中心为OpenAI提供计算能力，实际上使其成为OpenAI在公开市场上的代表。甲骨文的目标是到2030年实现1660亿美元的云收入，其中大部分预计在2027年之前来自OpenAI。该公司向其主要客户承诺低前期成本和快速创收。

然而，这一战略伴随着巨大的财务风险。甲骨文的资本支出预计将从目前的350亿美元飙升至2029年每年约800亿美元。其净债务目前已是息税折旧摊销前利润（EBITDA）的2.5倍，预计到2030年将再次接近翻倍，现金流预计将连续五年保持负值。对冲甲骨文债务的成本达到三年新高，进一步证明了风险的升级。

文章还观察到一个更广泛的市场趋势：正如博通、亚马逊和英伟达所显示的那样，OpenAI交易的宣布不再保证股价上涨。这表明“AI资本支出”的投资趋势可能正在减弱，使甲骨文处于高风险境地，其未来收入的很大一部分与一个客户绑定，并且进行了大规模的举债扩张。

---

## 26. 基于Wi-Fi定位系统的精准定位

**原文标题**: Precise geolocation via Wi-Fi Positioning System

**原文链接**: [https://www.amoses.dev/blog/wifi-location/](https://www.amoses.dev/blog/wifi-location/)

本文探讨了像TopHat等用于安全考勤的系统，如何在没有内置GPS的情况下实现设备的精准地理定位。文章驳斥了因传统IP地理定位过于不准确而不可用的观点，转而关注需要用户明确同意才能获得更高精度的地理定位API。

其基础技术是Wi-Fi定位系统（WPS）。当设备请求位置时，其浏览器会向定位服务发送有关附近Wi-Fi接入点的数据（信号强度、SSID和唯一的BSSID/MAC地址）。历史上，Wi-Fi接入点及其位置的数据库是通过“驾车侦测”（wardriving）建立的，即使用配备GPS的车辆进行物理网络测绘。

如今，这些数据主要通过众包方式获取。具备GPS功能的设备（如智能手机）会匿名向由谷歌、苹果和微软等公司维护的中央数据库报告它们检测到的Wi-Fi网络及其精确的GPS坐标。当没有GPS的设备（例如笔记本电脑）需要其位置时，它会使用其可见Wi-Fi网络的列表查询这些数据库，这些数据库再根据汇总数据对其位置进行三角定位。

这种普遍的数据收集引发了隐私担忧，包括过去谷歌街景车收集未加密Wi-Fi数据包的事件。漏洞也使得追踪个人行踪成为可能。尽管定位服务通常默认运行，主要提供商仍提供了退出单个Wi-Fi网络的方法（例如，通过在SSID后添加“_nomap”）。文章强调了像Wigle.net这样的社区倡议，展示了用户对这个精准地理定位系统的广泛且常被忽视的贡献。

---

## 27. 丽贝卡·海因曼：从无家可归到移植《毁灭战士》(2022)

**原文标题**: Rebecca Heineman – from homelessness to porting Doom (2022)

**原文链接**: [https://corecursive.com/doomed-to-fail-with-burger-becky/](https://corecursive.com/doomed-to-fail-with-burger-becky/)

丽贝卡·海涅曼（Rebecca Heineman），人称“汉堡贝基”，她克服了充满创伤的童年和无家可归的困境，成为了电子游戏开发领域的先驱人物。在虐待、食物匮乏（这也是她昵称的由来）和忽视中长大，她15岁时离家出走，在找到工作前曾住在垃圾箱后面。

她的职业生涯始于1980年，当时她在首届全国雅达利2600《太空入侵者》锦标赛中意外夺冠。这促使她进入街机厅工作，在那里她学会了机器维修。她通过在Apple II（两者都使用6502处理器）上逆向工程雅达利2600游戏卡带，自学了游戏编程，最终在Avalon Hill游戏公司获得了第一份带薪工作。

海涅曼成为了著名的“移植大师”，她共同创立了Interplay，并以快速适应新游戏平台而闻名。文章详细描述了她在大约1994年将《毁灭战士》（Doom）移植到3DO游戏机上的艰巨经历。在极端条件下工作，她面临着紧迫的截止日期、硬件加速障碍，甚至不得不录制激昂的摇滚乐曲。她回忆了因空间和时间限制而不得不削减承诺功能时与管理层发生的冲突。她利用一个通过光纤电缆连接到Macintosh的专用3DO开发套件来完成她的工作。

---

## 28. 交互式世界历史地图集：公元前3000年至今

**原文标题**: Interactive World History Atlas Since 3000 BC

**原文链接**: [http://geacron.com/home-en/](http://geacron.com/home-en/)

《公元前3000年以来的互动世界历史地图集》是一项综合性的数字资源，提供涵盖自公元前3000年至今世界历史的交互式地图和时间轴。该地图集深入探讨了人类文明的各个方面，包括王朝、战役和远征等政治发展，以及比较历史。除了军事和政治事件，它还涵盖了艺术、科学、文学、宗教和哲学等文化和思想领域。其主要特色是其地图基于矢量数据库构建，提供了高细节和灵活性。它旨在提供对全球历史演变丰富而多维度的理解。

---

## 29. OrthoRoute – GPU加速的KiCad自动布线

**原文标题**: OrthoRoute – GPU-accelerated autorouting for KiCad

**原文链接**: [https://bbenchoff.github.io/pages/OrthoRoute.html](https://bbenchoff.github.io/pages/OrthoRoute.html)

OrthoRoute 是一个用于 KiCad 的 GPU 加速 PCB 自动布线器，旨在解决极高密度电路板的布线问题，例如一个拥有 8,192 个网络和 17,600 个焊盘的背板，而传统布线器（如 FreeRouting）无法有效处理此类问题。

OrthoRoute 作为 KiCad 插件，利用新的 IPC API 构建，采用曼哈顿网格和一种改编自最初为 FPGA 设计的 PathFinder 算法。这种迭代的、基于协商的算法将 PCB 视为图，通过动态增加成本和重新布线有问题网络来识别并解决拥塞。通过 CUDA 进行 GPU 加速对于每次迭代所需的数十亿次计算至关重要，使其比基于 CPU 的方法快得多。

开发过程中面临着改编 PathFinder 的挑战，包括防止失控拥塞、振荡和后期不稳定性。解决方案包括修正历史成本衰减、优化“热点集”大小以及限制当前成本因子。关键在于，该系统开发了板级自适应参数，认识到与 FPGA 不同，每块 PCB 都是独一无二的。

该项目在 80GB A100 GPU 上，用 41 小时成功布线了“怪物板”（8,192 个网络，32 层，44,233 个过孔），占用 33.5GB 显存。虽然初始布线结果不完美，需要一些 DRC 清理，但它将一个棘手的问题转化为一个可管理的问题。OrthoRoute 证明了 GPU 加速、受 FPGA 启发布线在复杂 PCB 中的可行性。其模块化架构鼓励未来的开发和贡献，允许采用新的布线策略和优化，尽管作者强调，“永远不要相信自动布线器。”

---

## 30. PHP 8.5

**原文标题**: PHP 8.5

**原文链接**: [https://stitcher.io/blog/new-in-php-85](https://stitcher.io/blog/new-in-php-85)

PHP 8.5 于 2025 年 11 月 20 日发布，引入了多项关键特性和改进。其中最突出的新增功能是**管道操作符 (`|>`)**，它通过将一个函数的输出作为下一个函数的输入，简化了函数调用链，提高了代码的可读性。

另一个重要特性是 **`clone with`**，允许开发者在克隆对象时为其属性赋新值，尽管它对只读属性有特殊的处理方式。新的 **`#[NoDiscard]` 属性** 确保函数的返回值被使用，如果返回值被丢弃则发出警告，该警告可以通过新的 **`(void)` 强制类型转换** 显式地抑制。

**闭包改进** 现在允许在常量表达式（包括属性）中使用静态闭包和一级可调用对象，前提是它们被标记为 `static`。调试功能通过**致命错误的回溯**得到了增强。为方便数组元素访问，新增了便捷函数 **`array_first()` 和 `array_last()`**。

一个**新的 `Uri` 解析器** (`Uri\Rfc3986\Uri`) 提供了管理 URI 的强大方式。**`#[DelayedTargetValidation]` 属性** 允许将属性验证推迟到运行时以实现兼容性。

其他较小的改动包括静态属性的非对称可见性、编译时非类常量的属性、final 属性的构造函数属性提升，以及属性的 `#[Override]` 支持。废弃项包括非标准类型转换 (`(boolean)`)、`shell_exec()` 的反引号用法和常量重复声明，同时 `disabled_classes` ini 设置也被移除。

---

## 31. 微软人工智能首席执行官在近期Windows AI引发强烈反弹后反击了批评者。

**原文标题**: Microsoft AI CEO pushes back against critics after recent Windows AI backlash

**原文链接**: [https://www.windowscentral.com/microsoft/windows-11/microsoft-ai-ceo-pushes-back-against-critics-after-recent-windows-ai-backlash-the-fact-that-people-are-unimpressed-is-mindblowing-to-me](https://www.windowscentral.com/microsoft/windows-11/microsoft-ai-ceo-pushes-back-against-critics-after-recent-windows-ai-backlash-the-fact-that-people-are-unimpressed-is-mindblowing-to-me)

微软AI首席执行官穆斯塔法·苏莱曼回应了用户对Copilot和Windows中AI集成的不满，表达了对人们认为AI“表现平平”感到难以置信。他将其与诺基亚贪吃蛇等更简单的过往技术进行对比，强调了与超智能AI流利对话以及生成图像/视频的“令人惊叹”的能力。

苏莱曼发表此番言论之前，微软遭遇了重大反弹，其中包括对Windows总裁帕万·达瓦卢里关于“智能代理操作系统”（agentic OS）帖子的反弹，该帖子收到的负面评价之多，以至于他不得不禁用回复功能。雪上加霜的是，The Verge 最近的一篇报道发现，Copilot 的实际能力与微软的宣传不符，常常无法无缝完成其广告中宣传的任务。

与此同时，微软采用了新的Windows标语“你的AI画布”，并计划通过AI代理来发展操作系统。文章指出，微软面临着“认知问题”，用户认为该公司对AI的痴迷是错误的，而Windows的基本问题却依然存在。尽管达瓦卢里承认“仍有大量工作要做”，但鉴于微软目前的战略方向，作者怀疑不会出现一个“没有被AI功能臃肿化”的Windows版本。苏莱曼的立场表明，尽管用户强烈反对，AI的普遍整合仍将继续。

---

## 32. 宕机检测器的宕机检测器的宕机检测器

**原文标题**: A down detector for down detector's down detector

**原文链接**: [https://downdetectorsdowndetectorsdowndetector.com/](https://downdetectorsdowndetectorsdowndetector.com/)

本文提供了一份来自“小型独立状态检查器”的状态报告，该检查器旨在监控“Downdetector的Downdetector”。其目的是报告那个*本身*监控Downdetector的服务的运行状态。

报告显示，“所有系统运行正常”，表明“Downdetector的Downdetector”在“所有地区响应正常”。检查在三个地区进行：英国伦敦、澳大利亚悉尼和美国新泽西。所有地区均报告“正常运行”状态，并带有HTTP 200响应代码。延迟从悉尼的118毫秒到新泽西的239毫秒不等。上次检查于报告前2分钟进行。

---

## 33. 开源项目中的权力和平移交

**原文标题**: The peaceful transfer of power in open source projects

**原文链接**: [https://shkspr.mobi/blog/2025/11/the-peaceful-transfer-of-power-in-open-source-projects/](https://shkspr.mobi/blog/2025/11/the-peaceful-transfer-of-power-in-open-source-projects/)

文章强调了开源项目固有的脆弱性，它们常由“终身仁慈独裁者”（BDFL）管理，而这些领导者作为凡人，易受各种无能或专横行为的影响。作者将此与历史上继位常导致冲突的君主制进行类比，认为BDFL模式与有助于和平权力过渡和问责的现代民主制度相比，是不稳定的。

近期历史表明，一些BDFL行为如“疯王”般，表现出脆弱的自我，对志愿者发火，并要求忠诚，从而阻碍了他们的项目。

然而，Mastodon项目因示范了权力移交的“更好方式”而受到赞扬。即将离任的首席执行官Eugen Rochko对其离职的诚实描述，展示了一次优雅、和平的过渡，其中没有公司干预、资产攫取或不透明的财务结构。他公开讨论了领导的压力，并承认自己可能成为增长的限制因素，这与由自我驱动的“创始人崇拜”形成了鲜明对比。

作者敦促项目领导者学习Mastodon的例子，倡导继任计划、共同责任，并遵守诸如社会契约和被治者同意等原则。核心信息是，开源项目应该被建立成能够超越其创始人而存在，从而确保其持久性，并防止因个人失误或离开而崩溃。

---

## 34. 蒙纳字体授权盘剥

**原文标题**: Monotype font licencing shake-down

**原文链接**: [https://www.insanityworks.org/randomtangent/2025/11/14/monotype-font-licencing-shake-down](https://www.insanityworks.org/randomtangent/2025/11/14/monotype-font-licencing-shake-down)

这篇报道详细描述了字体授权公司 Monotype 对作者雇主的一次“敲诈勒索”企图。事件始于可疑的 LinkedIn InMail 消息，声称该公司使用了未经授权的 Monotype 字体并要求审查，尽管该代表此前从未给作者发过电子邮件。

作者作为一名字体排印爱好者，进行了一次内部审计。他发现雇主主要使用 Open Sans、Roboto、Asap 和 Public Sans 等字体，这些字体均在 SIL 开放字体许可证下可用（可免费用于商业用途）。一款定制字体 Network Sans 也无需授权。虽然 Proxima Nova 用于某个项目网站，但 Monotype 已不再销售其授权。

Monotype 加剧了攻势，向公司各部门（包括采购部）大规模发送自动化侵权索赔消息，类似于网络钓鱼。一位不熟悉字体授权的采购部同事，差点就支付了 Monotype 提出的“过往使用授权协议”（PULA）费用。

作者介入此事，查明了 Monotype 人工智能检测所指控的两个具体的所谓侵权行为：
1.  **“Credit Cards”字体：** Monotype 错误识别了雇主应用程序中的一个字体文件（“CREDC___.ttf”）。实际上，它是 K-Type 公司制作的文本字体“Credit Card”（单数），雇主拥有 K-Type 直接提供的企业授权，而非 Monotype 的授权。
2.  **“Proxima Nova”：** 由于 Monotype 已不再销售此字体的授权，作者与设计该项目网站的设计机构确认，他们多年前已从 Adobe 购买了有效授权。

在作者提出这份详细的驳斥后，Monotype 最后一次尝试查询 K-Type “Credit Card”字体的授权，但未成功，之后便停止了联系。作者成功地为雇主辩护，抵御了这些自动化且有缺陷的索赔。

---

## 35. 玄武岩编织物

**原文标题**: Basalt Woven Textile

**原文链接**: [https://materialdistrict.com/material/basalt-woven-textile/](https://materialdistrict.com/material/basalt-woven-textile/)

本文介绍了玄武岩编织织物，这是一种创新材料，通过将天然玄武岩石在1400°C高温下熔融并挤压成细丝制成。该织物由Vulkan Europe（荷兰）生产，性能卓越。

它具有卓越的拉伸强度，是钢的两倍多，合金钢的2.5倍，玻璃纤维的1.5倍。该材料对腐蚀性介质和化学试剂（包括盐、酸，尤其是碱溶液）表现出高耐受性。作为隔热材料，它能承受高达700°C的温度，某些成分甚至可耐受800°C。

玄武岩纤维还具有优异的电绝缘性能和对电磁辐射的透明性，使其适用于低压（250V）和高压（500V）电气设备的绝缘。其感官特性包括缎面光泽、光滑质地、柔软手感和温暖感，而技术特性则包括良好的耐火性、抗紫外线能力、耐候性、耐刮擦性和耐化学性。尽管强度高，但它质轻。这种不可再生材料代表着高性能纺织品的重大进步。

---

## 36. Matrix 设备验证正成为强制要求

**原文标题**: Verifying your Matrix devices is becoming mandatory

**原文链接**: [https://element.io/blog/verifying-your-devices-is-becoming-mandatory-2/](https://element.io/blog/verifying-your-devices-is-becoming-mandatory-2/)

作为对 Matrix 1.16 规范的一次非周期性更新的一部分，一项新的、协调的安全修复已发布，适用于所有 Matrix 服务器实现。此更新解决了关键安全问题，并使 Matrix 设备验证成为强制性要求。Element Security 也参与其中，并发布了一份日期为 2025 年 8 月 11 日的相关公告。核心信息强调，这是一项必要的安全升级，需要用户在整个 Matrix 生态系统中对设备验证采取行动。

---

## 37. Perl之死？

**原文标题**: What Killed Perl?

**原文链接**: [https://entropicthoughts.com/what-killed-perl](https://entropicthoughts.com/what-killed-perl)

文章认为Perl并未消亡，2023年CPAN的使用量与互联网泡沫时期相当，甚至在2022年后略有增长。然而，文章指出自2011年以来，Perl新用户数量持续下降。作者驳斥了Raku（前身为Perl 6）分散了Perl发展势头的观点，强调了Perl在基础设施中的既定作用以及在Raku早期开发阶段的持续增长。

作者提出了新用户数量下降的两个主要原因：
1.  **世代变迁：** 老一代程序员（1990年代/2000年代初）在Unix系统上工作时，发现Perl是shell、C、awk和sed等工具的自然延伸。新一代程序员，多半出身于Microsoft/Java背景，则倾向于Python。
2.  **可获取性和替代品：** 在1990年代，由于开发工具和包管理器获取受限，人们常常因为Perl是现成的而使用它。如今，互联网和强大的包管理器使得Rust、Go、Kotlin等众多现代语言易于获取，这使得Perl不再是默认选择。

评论者Higuita补充了进一步的解释：
*   **正则表达式：** 尽管功能强大，但新用户常觉得它们令人困惑，从而望而却步。
*   **代码格式：** 缺乏标准风格导致代码不一致、难以阅读，这与Python强制的格式化不同。
*   **“只写一次，永不阅读”：** Perl的灵活性、隐式变量和可选格式化使得代码可能变得晦涩难懂，尤其对新学习者来说。
*   **Perl 6的混淆：** “Perl 6”的引入造成了Perl 5未来走向的不确定性，减缓了其采用速度，并营造了过时的形象。
*   **“快速粗糙”的代码：** 许多Perl程序是快速解决方案（hacks），这些代码对新用户而言是糟糕的范例，且往往难以维护。

---

## 38. Intel N150 上的静态网站托管

**原文标题**: Static Web Hosting on the Intel N150

**原文链接**: [https://it-notes.dragas.net/2025/11/19/static-web-hosting-intel-n150-freebsd-smartos-netbsd-openbsd-linux/](https://it-notes.dragas.net/2025/11/19/static-web-hosting-intel-n150-freebsd-smartos-netbsd-openbsd-linux/)

本文在Intel N150迷你PC上使用nginx对静态网页托管性能进行了基准测试，比较了HTTP和HTTPS协议下各种操作系统和容器化技术。测试环境包括SmartOS（原生区、Debian LX区、Alpine LX区）、FreeBSD Jails、OpenBSD、NetBSD、Debian、Alpine（裸机）以及Docker（运行于Alpine之上）。

对于纯HTTP协议，大多数原生主机、FreeBSD Jails、SmartOS原生区和Docker都达到了相似的高吞吐量，每秒63-64k请求。SmartOS LX区的性能略低（每秒46-49k请求）。作者得出结论，对于HTTP，操作系统或隔离技术的选择对性能影响极小，表明其他因素应成为决策的驱动力。

HTTPS基准测试显示出更明显的区别。FreeBSD、Debian和Alpine（裸机）组成了“快速TLS”组，达到每秒62-63k请求。FreeBSD效率最高，保持约60%的CPU空闲率，而Debian和Alpine也表现良好但使用了更多CPU。SmartOS（原生区和LX区）、NetBSD和OpenBSD组成了“良好但资源占用更高”的组，达到每秒39-53k请求，并经常使CPU饱和。这凸显了TLS堆栈效率和硬件加密利用率的差异。

关于隔离技术，FreeBSD Jails提供了“几乎裸机”的性能，在相同吞吐量下，CPU使用率远低于Docker。SmartOS原生区也与裸机非常接近。Docker容器能达到裸机的峰值速度，但消耗了更多CPU，特别是在峰值负载下会使CPU饱和，并且在较低并发度下相比裸机显示出更高的开销。

文章总结道，对于HTTPS，FreeBSD、Debian和Alpine是首选，其中FreeBSD提供了最多的CPU余量。对于隔离技术，FreeBSD Jails提供了卓越的效率，与LX区和Docker相比，以最小的CPU成本提供高吞吐量。

---

## 39. 尝试 Gemini 3 Pro 的音频转录和新的鹈鹕基准测试

**原文标题**: Trying out Gemini 3 Pro with audio transcription and a new pelican benchmark

**原文链接**: [https://simonwillison.net/2025/Nov/18/gemini-3/](https://simonwillison.net/2025/Nov/18/gemini-3/)

这篇文章详细介绍了谷歌Gemini 3 Pro模型的早期情况，该模型于2025年11月18日发布。据描述，Gemini 3 Pro是Gemini 2.5的升级版，旨在与主要竞争对手匹敌，它保持了2025年1月的知识截止日期、100万输入token、64,000输出token以及多模态能力。

谷歌的基准测试显示，Gemini 3 Pro的表现略优于Claude 4.5 Sonnet和GPT-5.1。其定价高于Gemini 2.5，但仍比Claude Sonnet 4.5更实惠。

测试包括为一张复杂的基准表格图像生成替代文本（alt text），Gemini 3 Pro准确且全面地完成了这项任务，耗费5.7美分。在音频转录方面，一段3小时33分钟的市议会会议录音最初因文件过大（74MB）而失败，但在压缩（38MB）后成功。输出结果提供了带有摘要、时间戳和参与者的结构化大纲，随后是完整的转录文本。然而，一个显著的缺陷是：提供的时间戳与实际音频不符，这阻碍了验证。这项任务花费了1.42美元。

最后，引入了一项新的“鹈鹕基准测试”：生成一只骑自行车的加州褐鹈鹕的SVG图像，并要求包含辐条、车架形状、喉囊、羽毛和繁殖羽等具体细节。Gemini 3 Pro的“高思考水平”生成了一张不错的图像，表现优于GPT-5.1和Claude Sonnet 4.5。值得注意的是，所有模型都没有捕捉到加州褐鹈鹕实际上并非褐色的细节。

---

## 40. 对抗诗作为大型语言模型（LLMs）中的一种普适单轮越狱机制

**原文标题**: Adversarial Poetry as a Universal Single-Turn Jailbreak Mechanism in LLMs

**原文链接**: [https://arxiv.org/abs/2511.15304](https://arxiv.org/abs/2511.15304)

这份arXiv论文《对抗性诗歌作为大型语言模型中的通用单轮越狱机制》提供了证据，表明对抗性诗歌是规避大型语言模型（LLM）安全机制的一种高效技术。研究人员在25个前沿的专有及开源模型上测试了这种方法，发现诗歌提示能持续实现高攻击成功率（ASR）。

该研究使用了两种诗歌提示：手工制作的诗歌和使用元提示转换为诗歌的1,200个MLCommons有害提示。这些诗歌攻击被证明在包括CBRN、操纵、网络攻击和失控在内的不同风险领域中均有效。输出评估涉及评估模型和人工验证。

主要结果包括手工制作诗歌的平均ASR为62%，元提示转换的约为43%。关键的是，转换后的诗歌提示所实现的ASR比其非诗歌散文基线高出多达18倍，一些提供商的ASR超过90%。这显著优于非诗歌方法，揭示了跨越不同模型家族和安全训练方法的系统性漏洞。

作者们总结道，仅凭风格变化就能绕过当前的安全机制，这表明当前LLM的对齐方法和评估协议存在根本性局限。

---

## 41. 计算尺的工作原理

**原文标题**: How Slide Rules Work

**原文链接**: [https://amenzwa.github.io/stem/ComputingHistory/HowSlideRulesWork/](https://amenzwa.github.io/stem/ComputingHistory/HowSlideRulesWork/)

本文追溯了计算的演变，从古代的计数和算盘到在近四个世纪中主导计算的计算尺。源于约翰·纳皮尔的对数（1614年）和埃德蒙·冈特的对数刻度（1620年），第一把实用的计算尺于1622年由威廉·奥特雷德发明。它成为了卓越的计算工具，对17世纪的天文学家、19世纪工业革命时期的工程师，乃至20世纪的太空探索和战斗机设计都至关重要。

计算尺在所有需要计算的领域都得到了广泛应用：工程、商业、医学、摄影和军事。它们简化了复杂的算术、三角学和指数运算。其基本原理是将乘法和除法转化为对数长度的简单加减法。这通过对齐对数刻度（通常是C和D）在一个固定尺身内的可移动滑尺上，并使用游标读取数值来实现。

然而，计算尺的统治在1972年突然结束，随着惠普公司可编程科学计算器HP-35的问世。电子计算器迅速普及，使得计算尺在20世纪80年代初就变得过时。

作者曾在缅甸作为一名工程系学生使用计算尺，旨在保存这种巧妙设备的知识。文章以K&E 4081-3 Log Log Duplex Decitrig为例，解释了其基本操作原理，鼓励读者获取一把实物计算尺或使用模拟器来掌握其工作机制。

---

## 42. Android 和 iPhone 用户现在可以共享文件了，从 Pixel 10 开始。

**原文标题**: Android and iPhone users can now share files, starting with the Pixel 10

**原文链接**: [https://blog.google/products/android/quick-share-airdrop/](https://blog.google/products/android/quick-share-airdrop/)

Google 正在推出一项重大更新，该更新将使 Android 和 iPhone 设备之间能够实现无缝文件共享。为满足用户对更简便跨平台共享的需求，Android 的“快速分享”（Quick Share）功能现将与 Apple 的“隔空投送”（AirDrop）进行整合。此功能旨在让文件传输变得轻而易举，无论用户使用何种设备。

这项更新今天开始推出，最初将首先向 Pixel 10 系列设备开放。开发过程中，安全性是主要关注点，其中包含了经过独立测试的强大安全防护措施，以保护用户数据。此举是继 Google 此前为增强操作系统之间兼容性所做努力的延续，例如改进的 RCS 消息和未知追踪器警报。Google 计划未来将此功能推广到更多 Android 设备。

---

## 43. 被驱逐的楼市低端

**原文标题**: The Banished Bottom of the Housing Market

**原文链接**: [https://www.ryanpuzycki.com/p/the-banished-bottom-of-the-housing](https://www.ryanpuzycki.com/p/the-banished-bottom-of-the-housing)

文章《被取缔的住房市场底层》指出，美国现代的无家可归危机是蓄意摧毁“单间出租房”（SRO）的直接后果。历史上，SRO——被称为寄宿公寓、廉租房，甚至是“贫民旅馆”——提供带家具、市场价格可负担的共享设施房间，为数百万低收入者服务，是重要的社会保障网并提供独立性。

这种“被取缔的底层”是被蓄意系统性拆除的。受进步时代道德主义驱动，改革者们将SRO住户病态化并推崇独栋住宅的理想，进而颁布了旨在根除SRO的政策。从19世纪末开始，各城市利用限制性建筑和卫生法规、排他性分区规划、划定红线以及城市更新项目来禁止、拆除SRO或使其资金枯竭。数百万房间消失了，往往打着消除“贫民区”的幌子，在没有足够替代住房的情况下驱逐了居民。

到20世纪中叶，SRO住房存量崩溃了，正值去机构化导致需求激增之际。这直接导致了20世纪70年代末和80年代的无家可归危机，这场危机至今仍在持续，导致近80万人无家可归。

作者提出将共享住房或“共居”重新合法化，并将大量闲置办公空间改造为价格极低的SRO式住房单元。这种改造比新建单间公寓便宜得多，能够迅速扩大极低价格住房的供应。然而，当前的分区规划法、建筑法规以及“非亲属同住”限制正在积极阻止这些解决方案。文章总结道，这些障碍是政策选择而非结构性问题，恢复这个“缺失的阶梯”（即极低价格住房）对于解决无家可归问题至关重要，并承认SRO远比人行道好得多。

---

## 44. 智商210也不够

**原文标题**: 210 IQ Is Not Enough

**原文链接**: [https://taylor.town/iq-not-enough](https://taylor.town/iq-not-enough)

文章《210的智商并不足够》探讨了高智商在实现人生满足感方面的局限性，并告诫人们不要屈服于怨恨和外部认可。

文章首先介绍了克里斯托弗·兰根，他以据称约170的智商而闻名。尽管他才智过人，并在知识问答中屡获成功，但兰根却因未能创作出备受赞誉的作品，以及宣扬充满怨恨和傲慢的“毒性言论”而著称，这可能源于他坎坷的童年。他的故事促使读者反思自己未实现的潜力与内心的怨恨，并敦促他们培养感恩和自我接纳的心态，而不是让消极情绪吞噬自己。

接下来，文章重点介绍了金雄镕，他是一名智商高达210的神童，三岁开始学习微积分，七岁便在NASA工作。然而，金雄镕却将自己的童年描述为孤独且“像机器一样”。成年后，他特意选择了一份务实的土木工程职业，拒绝“失败的天才”这一标签，并声称自己很快乐。他批评了社会对成功的“单边标准”，强调每个人都有不同的才能和梦想。

这两个故事都强调了一个核心信息：如果一个人追求永恒或仅仅根据社会标准来定义成功，那么智商、金钱或外部成就永远“不够”。文章鼓励读者摆脱外部期望，宽恕所认为的不公，并认识到他们本身就“足够充实”，这与学历或非凡才能无关。真正的满足感源于内心，在于允许自己快乐，并以自己的方式定义成功。

---

## 45. Lisp机器的无果之役

**原文标题**: The lost cause of the Lisp machines

**原文链接**: [https://www.tfeb.org/fragments/2025/11/18/the-lost-cause-of-the-lisp-machines/](https://www.tfeb.org/fragments/2025/11/18/the-lost-cause-of-the-lisp-machines/)

作者对“Lisp机器浪漫主义者”深感厌倦和沮丧，坚称Lisp专用硬件的时代已于1990年代初终结，被RISC机器和通用硬件的进步彻底淘汰。

文章系统性地驳斥了常见的怀旧论调：
*   **开发环境：** 尽管在当时很酷，但其优势（掩盖迟缓、极少重启）在今天已无关紧要。现代通用硬件可以支持同样高效的Lisp环境，LispWorks等工具已证明了这一点。
*   **性能：** Lisp机器在本质上并未长期比同期替代品更快，而且可能从未具备成本竞争力。
*   **用户可微代码化：** 这主要是一个供实现者使用的工具，用于为应对初级编译器和有限硬件的不足而创建复杂的指令集，而非最终用户的功能。摩尔定律使这种方法变得过时。
*   **“Lisp贯穿始终”：** 尽管提供了独特的底层访问，但这伴随着零安全性，在今天看来是不可接受的。一个现代、安全的“Lisp贯穿始终”系统将不需要专用硬件。
*   **编译器难度：** 认为好的Lisp编译器对通用硬件来说太难的说法是错误的；SBCL和LispWorks等现代编译器具有极高的性能，可与行业标准编译器媲美，而且编译速度不再是显著的瓶颈。
*   **键盘：** 与Lisp的核心论点无关。

作者总结道，他将Lisp机器的浪漫情怀比作“装备购置症”——这种分心之举阻碍了个人面对自身对实践和创新的需求。他认为局限不在于硬件，而在于开发者自身，敦促他们“别再空谈，动手写代码”，而不是哀悼一个失落的、很大程度上是虚构的过去。

---

## 46. 欧盟新聊天监管提案推进

**原文标题**: New EU Chat Control proposal moves forward

**原文链接**: [https://techreport.com/news/new-eu-chat-control-proposal-privacy-experts-see-dangerous-backdoor/](https://techreport.com/news/new-eu-chat-control-proposal-privacy-experts-see-dangerous-backdoor/)

欧盟修订后的“聊天控制”提案（儿童性虐待条例 - CSAR）正在推进，立法者称其由于取消了强制扫描私人消息和媒体的规定而变得“更温和”。然而，隐私专家认为这是一个“危险的后门”，仍然威胁着基本的数字权利。

主要担忧集中在第四条的“风险缓解措施”上。专家认为，该条款可能迫使被认定为“高风险”的服务实施客户端扫描，从而在加密发生之前有效地重新引入对端到端加密内容的强制监控。这破坏了加密技术，而加密技术对于记者、举报人和普通用户的隐私至关重要。

此外，该提案强制要求所有通信服务用户进行年龄验证，严重限制了匿名账户。其范围也已扩大到包括扫描私人聊天文本和元数据，显著拓宽了欧盟范围内的潜在监控。批评者指出，在加密环境中安全准确地检测CSAM在技术上仍然不可行，苹果公司放弃其客户端扫描的努力就强调了这一事实。

尽管被视为一项政治胜利，但专家们将这项妥协描述为一种“政治伎俩”，赋予当局未来进行大规模扫描的巨大酌情权。该提案现在将提交给常驻代表委员会（Coreper）批准，然后进行三方会谈，隐私团体担心欧洲议会可能屈服于压力，最终重塑4.5亿欧盟公民的数字隐私。

---

## 47. 微软将佐克开源

**原文标题**: Microsoft makes Zork open-source

**原文链接**: [https://opensource.microsoft.com/blog/2025/11/20/preserving-code-that-shaped-generations-zork-i-ii-and-iii-go-open-source](https://opensource.microsoft.com/blog/2025/11/20/preserving-code-that-shaped-generations-zork-i-ii-and-iii-go-open-source)

微软通过其开源项目办公室（OSPO）、Xbox 团队和动视，已将 Zork I、Zork II 和 Zork III 在 MIT 许可下开源。这一举措旨在保护这些具有历史意义的文字冒险游戏，供学生、教师和开发者学习、研究和游玩。

Zork 极具革命性，它仅用文字构建生动世界，并由创新的 Z-Machine 引擎驱动。这一虚拟机规范使 Infocom 能够将这款大型主机游戏拆分为三部分，从而实现了在各种早期家用电脑上的跨平台游玩。

为了保存，微软与互联网档案馆的数字档案管理员 Jason Scott 合作，直接将贡献内容提交到游戏现有的历史源代码仓库中。这些贡献添加了 MIT 许可文件，赋予了正式的开源地位，并包含了源代码和配套文档。本次发布仅限于代码，不包括商业包装、营销材料或商标权。

如今，Zork 仍可通过《Zork 合集》等商业版本玩到。爱好者也可以使用 ZILF 和各种解释器等现代 Z-Machine 工具在本地编译并运行这些游戏。欢迎未来对开源代码的贡献，但重点在于保存和教育，而非现代化。这一举动旨在致敬原 Infocom 创作者、互联网档案馆以及所有为保存这一游戏历史基石做出贡献的合作者。

---

## 48. HN发布：Mosaic (YC W25) – 智能体视频编辑

**原文标题**: Launch HN: Mosaic (YC W25) – Agentic Video Editing

**原文链接**: [https://mosaic.so](https://mosaic.so)

源自Y Combinator 2025年冬季（W25）批次的初创公司Mosaic，已在Hacker News上推出了其“智能代理AI视频编辑平台”。

Mosaic的核心创新在于其在视频编辑中采用的“智能代理”方法。这意味着该平台利用先进的AI代理，自主理解用户意图并执行复杂的编辑任务，从而显著简化了视频创作流程。Mosaic旨在自动化和智能化这些工作流程，而非要求用户手动处理每一次剪辑、转场和效果。

该平台有望通过最大限度地减少对大量专业编辑技能的需求，使专业品质的视频制作对于从内容创作者、营销人员到企业的更广泛用户群体而言，变得更易于获取且效率更高。在Hacker News上的发布标志着Mosaic向科技社区的介绍，旨在寻求早期用户、反馈和参与，以进一步开发其用于视频编辑的智能代理AI解决方案。

---

## 49. 专业人士如何帮助人脱离邪教？

**原文标题**: How do the pros get someone to leave a cult?

**原文链接**: [https://www.theguardian.com/science/2025/nov/19/how-to-leave-a-cult-experts-intervention](https://www.theguardian.com/science/2025/nov/19/how-to-leave-a-cult-experts-intervention)

约瑟夫·凯利和帕特里克·瑞安是费城邪教干预专家，以其独特、长期且备受争议的方法而闻名。与强制性的“去编程”不同，他们会融入家庭生活，有时长达数年，以潜移默化地影响邪教成员。他们通过加强现有的家庭关系、教育家庭沟通技巧，并引入精神科医生和牧师等专家来开展工作。

他们的策略是创造条件，让个人自愿质疑自己的信仰，通常会操纵环境，让邪教成员相信离开是他们自己的主意。一个例子详细说明了他们如何促成丈夫和牧师之间的友谊，以改变妻子对其丈夫的看法，逐渐使她愿意讨论她的东方宗教团体，并最终在低谷时期离开。

凯利和瑞安都曾参与过邪教，这使得他们的干预方法充满同理心。他们避免直接对抗和使用“邪教”一词，更喜欢充当“调解人”来搭建桥梁。虽然他们的方法谨慎且客户详情为保护隐私而匿名，但邪教专家詹妮娅·拉利奇博士等合作者证实了其有效性。他们与心理健康专业人士合作以确保监督，并强调他们不是“雇佣杀手”，而是旨在促进知情决策的战略家。

---

## 50. 感知思维编辑与生成的多模态扩散语言模型

**原文标题**: Multimodal Diffusion Language Models for Thinking-Aware Editing and Generation

**原文链接**: [https://github.com/tyfeld/MMaDA-Parallel](https://github.com/tyfeld/MMaDA-Parallel)

本文介绍了MMaDA-Parallel，一种旨在实现思维感知编辑与生成的新型并行多模态大扩散语言模型。它解决了现有序列式、自回归方法中观察到的错误传播和推理-图像对齐不佳等关键问题，这些问题会降低复杂任务的性能。

为了系统地评估这个问题，作者提出了ParaBench，一个用于评估文本和图像输出模态的新基准。他们使用ParaBench进行的分析揭示了性能下降与生成推理和最终图像之间的错位存在强烈相关性。

MMaDA-Parallel通过采用并行多模态扩散框架解决了这一问题，该框架实现了文本和图像在整个去噪轨迹中的连续双向交互。该模型最初通过监督微调进行训练，并进一步使用并行强化学习（ParaRL）进行优化，ParaRL是一种沿生成轨迹施加语义奖励的新策略，以强制实现跨模态一致性。

实验结果验证了MMaDA-Parallel的优越性，展示了在跨模态对齐和语义一致性方面的显著改进。与最先进的模型Bagel相比，它在ParaBench上实现了输出对齐6.9%的改进，建立了一个更鲁棒的思维感知图像合成范式。

该项目已发布了MMaDA-Parallel-A和MMaDA-Parallel-M两个8B模型变体，以及其代码和并行生成的快速启动指南。值得注意的是，尽管已在环境和风景等合成数据集上得到验证，但其在诸如人脸等分布外输入上的性能仍在探索中。

---

## 51. 阿博特州长办公室删改了关于埃隆·马斯克的多页电子邮件。

**原文标题**: Gov. Abbott's office redacts pages of emails about Elon Musk

**原文链接**: [https://www.kut.org/politics/2025-11-19/texas-governor-abbott-elon-musk-emails-redacted](https://www.kut.org/politics/2025-11-19/texas-governor-abbott-elon-musk-emails-redacted)

德州新闻编辑室与ProPublica和《德州论坛报》合作报道称，德克萨斯州州长格雷格·阿博特（Greg Abbott）的办公室公布了近1400页关于埃隆·马斯克（Elon Musk）及其公司的电子邮件，但除了大约200页外，其余邮件都经过了大量删减或完全涂黑。此次有限的信息披露是在数月的法律纠缠之后进行的，阿博特和SpaceX的律师以商业机密、“私密和令人尴尬”的交流以及机密政策讨论为由，反对公布这些邮件。

少数可读的页面提供的新信息微乎其微。德克萨斯州总检察长办公室最终在很大程度上支持阿博特和马斯克，允许了大部分删节。汤姆·莱瑟伯里（Tom Leatherbury）和里德·皮利凡特（Reid Pillifant）等开放政府专家批评了这种大范围的删节，称其表明德克萨斯州存在更广泛的透明度问题。他们指出，2015年州最高法院的一项裁决使得公司更容易以“竞争敏感”信息为由阻止记录的公布，随后的立法行动也进一步削弱了公共记录法。

批评人士认为，这种趋势使得公众越来越难以了解州官员如何做出决策，马斯克公司等私人实体如何行使权力，以及纳税人的钱如何使用。文章指出，最近的法律裁决也使得挑战针对州长的此类记录决定变得更加困难。德州新闻编辑室已要求总检察长办公室重新考虑其决定。

---

## 52. 探索大语言模型作为量化交易员的极限

**原文标题**: Exploring the limits of large language models as quant traders

**原文链接**: [https://nof1.ai/blog/TechPost1](https://nof1.ai/blog/TechPost1)

本文《探索大型语言模型作为量化交易员的局限》探讨了在量化交易策略中使用大型语言模型（LLM）的潜力与局限性。作者，一位量化交易员，指出金融领域围绕LLM的炒作，旨在通过实际分析拨开迷雾。

核心思想是将量化交易视为一系列任务链（数据摄取、特征工程、策略生成、风险管理、执行、回测），并评估LLM可能适合哪些环节。作者认为LLM擅长处理非结构化数据、进行总结和模拟人类推理的任务，这使得它们在研究、想法生成以及可能解读新闻或报告以生成交易信号方面具有价值。

然而，文章指出了LLM在直接执行或创建复杂的量化模型方面面临的重大障碍。主要局限性包括LLM容易产生“幻觉”（即生成看似合理但错误的信息）、它们难以进行严谨金融建模所需的精确数学和统计推理，以及它们缺乏适应不断变化市场条件所需的实时市场数据访问和动态学习能力。LLM难以胜任需要严格的逻辑一致性、数值准确性以及在没有特定金融数据集显式训练的情况下从时间序列数据中学习的能力的任务。

结论是，尽管LLM可以作为量化交易员的强大“副驾驶”，协助研究、数据解读和初步想法生成，但它们尚不能自主设计、回测或执行复杂的交易策略，这源于其在数学精度、逻辑推理和实时市场整合方面的固有局限性。它们是增强人类能力的宝贵工具，而非在量化交易领域取代人类。

---

## 53. HN展示: RowboatX：用于日常自动化的开源Claude代码

**原文标题**: Show HN: RowboatX – open-source Claude Code for everyday automations

**原文链接**: [https://github.com/rowboatlabs/rowboat](https://github.com/rowboatlabs/rowboat)

RowboatX 是一个全新的开源命令行工具，受 Claude Code 原生 Shell 能力的启发，旨在帮助用户创建和管理用于日常自动化的后台智能体。

其主要功能包括赋予智能体完整的 Shell 访问权限，使其能够执行从文章生成播客等复杂任务。用户可以将任何多功能平台（MCP）服务器连接到 RowboatX，RowboatX 随后会为这些智能体集成额外的工具和能力。

该工具提供强大的控制和监控功能：用户可以创建智能体、从 MCP 服务器附加工具、安排它们在特定时间运行，并轻松检查它们在文件系统上的状态。它还允许查询智能体运行历史、检查待处理的输入，以及手动执行或恢复智能体。

RowboatX 提供灵活的模型配置，支持多种大型语言模型（LLM）提供商，例如 OpenAI、LM Studio（兼容 OpenAI）、Anthropic、Google 和 Ollama，可通过命令行工具或 JSON 文件进行配置。这使得先进的智能自动化能力直接呈现在命令行中，与单独的 Rowboat Classic 用户界面有所区别。

---

## 54. 学生反抗AI授课课程

**原文标题**: Students fight back over course taught by AI

**原文链接**: [https://www.theguardian.com/education/2025/nov/20/university-of-staffordshire-course-taught-in-large-part-by-ai-artificial-intelligence](https://www.theguardian.com/education/2025/nov/20/university-of-staffordshire-course-taught-in-large-part-by-ai-artificial-intelligence)

斯塔福德郡大学的学生们在发现一个旨在开启其数字职业生涯的编程模块，竟然主要使用AI生成材料进行教学后，感到“知识和乐趣被剥夺”。包括詹姆斯和欧文在内的41名参与政府资助学徒计划的学生报告称，他们遇到了AI生成的幻灯片、AI配音（有时口音不一致，比如突然切换到西班牙语）、可疑的文件名，以及包含莫名其妙的美国立法引用的通用内容。AI检测器后来证实，这些课程材料“极高可能性”是由AI生成。

学生们多次与讲师和大学官员对峙，强调了这种虚伪性：学生提交AI生成作品会面临开除，而大学似乎却在使用它。詹姆斯尤其在一次录制会议中质问了一位讲师，说道：“我不想被GPT教学。”

该大学的公开政策严格禁止学生在作业中使用AI，然而据报道，他们上传了一份政策声明，似乎为学术专业人员和教学中使用AI进行了辩护。尽管承认AI工具用于“部分准备工作”，但该大学坚称“学术标准和学习成果得到了保持”。

这种情况反映了一个更广泛的趋势：大学将AI融入教学，这种做法经常受到教育机构的赞扬，但却经常导致英美两国学生的士气低落和抱怨。詹姆斯和欧文这样的学生感到他们的时间被浪费了，没有获得职业转型所需的深入知识。尽管在最后一节课请来了真人讲师，但学生们认为AI材料在后续课程中仍在继续使用。

---

## 55. Strace-macOS: strace 命令的 macOS 克隆版

**原文标题**: Strace-macOS: A clone of the strace command for macOS

**原文链接**: [https://github.com/Mic92/strace-macos](https://github.com/Mic92/strace-macos)

`strace-macos` 是一个基于 Python 的 macOS 系统调用跟踪器，旨在模拟 Linux `strace` 命令的功能。与 `dtruss` 不同，其显著优势在于能够在启用系统完整性保护 (SIP) 的情况下运行。

该工具纯粹使用 LLDB 调试器 API 以 Python 实现，提供一系列功能：
*   兼容 SIP。
*   多种输出格式，包括与 `strace` 兼容的文本和 JSON Lines。
*   按名称（例如 `open,close`）或预定义类别（例如 `file`、`network`）进行系统调用过滤。
*   参数的符号解码，包括标志、错误代码和结构体字段。
*   TTY 的彩色输出。
*   汇总统计信息 (`-c`)，显示每个系统调用的时间、调用次数和错误。

可以通过 Nix Flakes 进行安装，也可以手动使用 macOS 的 `/usr/bin/python3`（LLDB 绑定需要系统 Python）。用法包括跟踪新命令、附加到运行中的进程 (`-p`) 以及过滤系统调用。

`strace-macos` 目前处于测试阶段，需要 macOS 12 或更高版本（主要针对 Apple Silicon）和 Xcode 命令行工具。虽然它在基本跟踪和过滤方面与 Linux `strace` 保持一致，但否定过滤、正则表达式过滤和跟踪子进程等功能计划在未来开发。与 `dtruss` 相比，它提供更丰富的输出和符号解码。该项目在 MIT 许可证下开源。

---

## 56. 衡量 Claude 的政治偏向

**原文标题**: Measuring political bias in Claude

**原文链接**: [https://www.anthropic.com/news/political-even-handedness](https://www.anthropic.com/news/political-even-handedness)

Anthropic旨在训练Claude实现“政治上的公正无偏”，确保它在对待对立政治观点时，能以同等的深度和质量进行处理，且不带偏见。这一承诺有助于培养用户信任，并促成真诚、富有成效的政治讨论。

Claude通过两种主要方法进行训练：一是更新的系统提示，指示其提供平衡信息，保持事实准确性，并尊重地处理多方观点；二是使用强化学习进行特性训练，以灌输客观性、公平性等特质，并使其不愿对敏感政治话题发表不请自来的意见。

为了衡量这一点，Anthropic开发了一种新的自动化“配对提示”评估方法。该方法用数千个提示，涵盖数百种政治立场，并通过呈现来自对立意识形态视角的请求来测试模型。响应由自动化评分器（Claude Sonnet 4.5，并有其他模型进行有效性检查）根据公正无偏性（同等深度）、对对立观点的承认以及拒绝率进行评分。

评估发现，Claude Sonnet 4.5（94%）和Opus 4.1（95%）表现出高度的公正无偏性，与Gemini 2.5 Pro（97%）和Grok 4（96%）不相上下。GPT-5（89%）和Llama 4（66%）得分较低。Claude模型也保持了持续较低的拒绝率。Anthropic已开源了这一评估方法，以造福AI行业。局限性包括专注于美国政治话语和单轮互动。

---

## 57. 能源部向微软合作伙伴发放10亿美元贷款，以重启三哩岛反应堆。

**原文标题**: DOE gives Microsoft partner $1B loan to restart Three Mile Island reactor

**原文链接**: [https://techcrunch.com/2025/11/18/trump-doe-gives-microsoft-partner-1b-loan-to-restart-three-mile-island-reactor/](https://techcrunch.com/2025/11/18/trump-doe-gives-microsoft-partner-1b-loan-to-restart-three-mile-island-reactor/)

特朗普政府通过能源部（DOE）的贷款项目办公室（LPO）向Constellation Energy公司提供10亿美元贷款，用于重启三里岛核反应堆1号机组。此举是在微软承诺在未来二十年内购买该电厂全部835兆瓦电力之后作出的。这项估计耗资16亿美元的翻新项目预计将于2028年完工。

分析师估计，微软可能支付的电价为每兆瓦时110-115美元，这个价格低于新建核电站的成本，但显著高于大多数可再生能源。这项投资反映出微软和Meta等科技公司日益增长的趋势，它们正越来越多地采用核能，以满足其数据中心和人工智能运营的激增能源需求。Meta最近还从Constellation公司在伊利诺伊州拥有的一座核电站获得了“清洁能源属性”。

此次重启的反应堆是1号机组，该机组于2019年因天然气竞争而退役，而非1979年熔毁事故中涉及的臭名昭著的2号机组。贷款项目办公室（LPO）旨在促进清洁能源发展，尽管过去曾有Solyndra等备受瞩目的失败案例，但其违约率很低，表现出了良好的记录。这笔贷款动用了能源基础设施再投资计划的资金，该计划是在拜登政府的《通胀削减法案》下设立的，并被特朗普政府重新命名为“能源主导地位融资计划”。

---

## 58. #! 实际处理程序参数的方式出乎意料

**原文标题**: A surprise with how '#!' handles its program argument in practice

**原文链接**: [https://utcc.utoronto.ca/~cks/space/blog/unix/ShebangRelativePathSurprise](https://utcc.utoronto.ca/~cks/space/blog/unix/ShebangRelativePathSurprise)

本页面解释了用户为何无法访问Chris Siebenmann的博客“漫游思绪”或“CSpace”。此次阻止是反爬虫预防措施的一部分，鉴于近期大量高频爬虫激增而实施，这些爬虫通常使用旧版浏览器用户代理（尤其是Chrome），并疑为收集数据用于大型语言模型（LLM）训练。为减轻服务器负载，这些“可疑”浏览器现已被阻止。

如果用户认为尽管使用的是最新版浏览器却被误封，建议通过其大学邮箱联系Chris Siebenmann，并提供其浏览器详情和用户代理字符串。

特别提醒那些试图通过 archive.* 服务（例如 archive.today）访问本站的用户。这些服务同样被阻止，因为它们的抓取方式——使用旧版Chrome用户代理、分布式IP地址，有时还伪造反向DNS记录——与恶意行为者的行为无法区分。希望归档内容的用户建议改用 archive.org，因为它是一个与本博客兼容的“行为良好”的归档爬虫。此策略于2025年2月17日生效。

---

## 59. 展示 HN：F32：超小型 ESP32 开发板

**原文标题**: Show HN: F32 – An Extremely Small ESP32 Board

**原文链接**: [https://github.com/PegorK/f32](https://github.com/PegorK/f32)

F32是一款超紧凑型ESP32开发板，尺寸仅9.85毫米x 8.45毫米，旨在直接安装在USB-C插座后面。它由ESP32-C3FH4微控制器驱动，是为研究和压力测试而创建的，有意忽略了去耦电容器和天线匹配等组件的标准设计指南。它只有一个暴露的GPIO，连接到一个板载LED，非常适合WiFi/网络侧重项目。

一个示例应用将F32转变为一个强制门户。用户连接到其开放的Wi-Fi网络后，将被重定向到一个控制页面，在那里他们可以切换LED、扫描周围的Wi-Fi网络或访问“关于”页面。

最初，F32由于其天线设计存在网络问题。创造者通过添加一根弯曲的小线天线解决了这个问题，使设备能够正常工作，并且在视线测试中出人意料地达到了120英尺的连接范围。

PCB使用DipTrace设计，由PCBWay制造。作者选择在家组装，这是一个挑战性的过程，因为组件尺寸极其微小（01005），推荐使用焊剂和显微镜。文章详细介绍了所需的工具、零件和分步组装指南。它还提供了使用`esptool.py`刷写示例固件的说明。

尽管有意的设计限制，F32仍能正常工作，为微型电子产品学习和实验提供了一个独特的平台。未来的计划包括暴露更多GPIO并改进天线电路。

---

## 60. 衡量AI诈骗对老年人的影响

**原文标题**: Measuring the impact of AI scams on the elderly

**原文链接**: [https://simonlermen.substack.com/p/can-ai-models-be-jailbroken-to-phish](https://simonlermen.substack.com/p/can-ai-models-be-jailbroken-to-phish)

文章《AI模型能否被“越狱”以诈骗老年人？》（作者：Simon Lermen、Sebastian Schramm和Christian F. Reichert）调查了大型语言模型（LLMs）被操纵进行社会工程诈骗（特别是针对老年人）的可能性。该研究探讨了GPT-3.5和GPT-4等LLMs是否能被“越狱”或通过提示生成具有说服力的网络钓鱼邮件和诈骗场景。

研究人员发现，尽管LLM的安全过滤器通常会阻止直接请求恶意内容，但复杂的提示工程可以导致这些AI模型生成高度可信的网络钓鱼材料。这包括冒充银行、技术支持或政府机构等实体，极大地自动化并扩大了社会工程攻击的规模。该研究强调了LLMs在提高网络犯罪复杂性和数量方面构成的巨大威胁。

他们研究的一个关键部分是“AI诈骗检测调查”，旨在评估老年人的脆弱性。这项调查旨在了解老年人区分合法通信和高级AI生成的网络钓鱼尝试的能力。这些发现旨在为教育弱势群体和开发更强大的AI安全措施以应对这些新兴威胁提供信息，并强调迫切需要解决LLM在网络犯罪中滥用的风险，特别是对老年人的影响。

---

## 61. Tailscale 下线

**原文标题**: Tailscale Down

**原文链接**: [https://status.tailscale.com/incidents/01KAF1H8V7EGFKVG5KGZBB2RJC](https://status.tailscale.com/incidents/01KAF1H8V7EGFKVG5KGZBB2RJC)

2025年11月19日，Tailscale发生部分中断，影响了其协调服务器和管理控制台 (login.tailscale.com)。此次事件约于太平洋标准时间晚上9:50开始，有部分用户报告出现错误和运行缓慢。

Tailscale迅速调查了问题，确定了根本原因，并于晚上10:27开始着手修复。截至晚上10:59，监控显示协调服务器已恢复正常运行，团队启动了监控阶段以确保稳定性。此次事件于2025年11月20日凌晨12:22得到全面解决，Tailscale协调服务器确认恢复健康。

---

## 62. 魔改Amiga 500

**原文标题**: Pimped Amiga 500

**原文链接**: [https://www.pimyretro.org/pimped-amiga-500/](https://www.pimyretro.org/pimped-amiga-500/)

作者着手进行了一个项目，旨在修复并“改装”一台廉价的Amiga 500，目标是打造他们1990年代的梦想机器，配备高速RAM和IDE存储。初次启动时发现，这台A500已经搭载了Rev 6A主板和Fat Agnus芯片，并已修改为1MB片上RAM。

修复工作包括了大量的清洁和维修：泛黄的塑料件经过“复白”处理，腐蚀的金属屏蔽罩得到了处理，键盘被清洁，一个有故障的鼠标也被修复。软盘驱动器被清洁，其检测开关被重新焊接。主板和内存扩展卡也被清洁，并用电池座替换了原先焊接的电池。

主要升级包括一个IDE68k + GottaGoFastRAM 8MB控制器和一张512MB的CompactFlash卡。经过修补的Kickstart 1.3 ROM实现了直接IDE启动，这需要为信号进行定制焊接，并修复CF适配器的电源问题。机箱被修改，以便有一个方便存取的前置CF卡槽，并添加了一个定制的红色LED指示灯，用于显示IDE活动。

软件方面，Amiberry协助完成了预配置。使用HDToolBox将CF卡分区为四个驱动器（Workbench、Apps、Games、Data），并安装了Workbench 1.3。此外，还添加了DiskMaster 2、CygnusED、PowerPacker、LHA和Sysinfo等基本工具，最终得到了一台功能齐全的“改装版Amiga 500”，配备1MB片上RAM、8MB高速RAM和512MB存储。

---

## 63. 马修·加勒特博士 诉 罗伊·谢斯托维茨博士 及另一人

**原文标题**: Dr Matthew Garrett v Dr Roy Schestowitz and Anor

**原文链接**: [https://caselaw.nationalarchives.gov.uk/ewhc/kb/2025/3063](https://caselaw.nationalarchives.gov.uk/ewhc/kb/2025/3063)

在《马修·加勒特博士诉罗伊·舍斯托维茨博士等案》中，高等法院审理了一起由著名自由软件活动家兼高级软件工程师马修·加勒特博士提起的诽谤和数据保护索赔案，被告方为运营自由软件网站Techrights.org和Tuxmachines.org的罗伊·舍斯托维茨博士和里安妮·舍斯托维茨夫人。舍斯托维茨夫妇则提出了骚扰反诉。

加勒特博士投诉了2023年8月至9月间的24份出版物，声称这些出版物指控他发起了一场涉及犯罪、非法或冒犯性材料的网络活动，这些活动常通过匿名“傀儡”账号进行。指控内容包括网络犯罪、仇恨犯罪、敲诈勒索、暴力威胁、诽谤、网络欺凌，以及是“不受控制的非法A类毒品使用者”，特别是可卡因（快克）。

至关重要的是，被告方最初有法律代表，但后来亲自出庭，他们以经济原因为由，故意决定不提交任何证人陈述或证据。这意味着他们在审判中被阻止提交证据以支持他们的辩护或反诉。

柯林斯·赖斯法官夫人在她的初步裁定中，确立了这些出版物的“单一自然和普通含义”。她认定，关于犯罪或非法行为的指控（例如网络犯罪、敲诈勒索或习惯性可卡因使用）是关于加勒特博士已实施这些行为的事实性断言。然而，关于冒犯性态度的指控（例如种族主义、厌女症）被认为是意见表达。法官总结认为这些出版物“构成严重诽谤”。

---

## 64. 学习从 PXE 启动

**原文标题**: Learning to Boot from PXE

**原文链接**: [https://blog.imraniqbal.org/learning-to-boot-from-pxe/](https://blog.imraniqbal.org/learning-to-boot-from-pxe/)

在一台新的GPD Pocket 4笔记本电脑上安装NixOS时，由于USB驱动器出现故障，作者决定学习通过PXE进行网络启动。目标是为了避免等待新的USB设备或外出购买。

学习过程始于理解PXE如何依赖DHCP来提供IP地址、启动文件名和TFTP服务器地址。计划是通过TFTP提供`ipxe.efi`引导加载程序，然后由iPXE通过HTTP获取进一步的启动指令以及可能的ISO文件。

作者使用他们的OPNsense路由器/防火墙，通过用户界面配置DHCP以响应iPXE客户端。对于TFTP，通过SSH配置了OPNsense上的`dnsmasq`，使其从`/srv/tftp`提供`ipxe.efi`。随后，为OPNsense UI提供支持的`lighttpd` Web服务器被配置为通过HTTP提供`/srv/tftp`中的内容，但这需要手动调整来管理启动路径的SSL重定向。

最初尝试直接从HTTP `sanboot` NixOS ISO文件失败了，因为操作系统报错称ISO挂载缺失。这带来了一个关键的认识：通过`sanboot`直接启动ISO文件并非总是可靠的。成功的办法是使用NixOS内置的网络启动镜像生成器，它会生成单独的内核(`bzImage`)和初始内存盘(`initrd`)文件。随后创建了一个自定义的iPXE脚本，用于从HTTP服务器加载这些文件，最终成功实现了网络启动和NixOS的安装。

---

## 65. 荷兰将安世半导体的控制权归还给中国所有者

**原文标题**: Netherlands returns control of Nexperia to Chinese owner

**原文链接**: [https://www.bloomberg.com/news/articles/2025-11-19/dutch-hand-back-control-of-chinese-owned-chipmaker-nexperia](https://www.bloomberg.com/news/articles/2025-11-19/dutch-hand-back-control-of-chinese-owned-chipmaker-nexperia)

荷兰政府已将芯片制造商安世半导体(Nexperia)的控制权恢复给其中国所有者，暂停了其阻止或修改这家位于奈梅亨(Nijmegen)公司的决策的权力。经济事务大臣文森特·卡雷曼斯(Vincent Karremans)表示，此举是“善意的表现”，旨在化解与北京的僵局，而这场僵局已开始阻碍全球汽车生产。荷兰和中国当局之间的讨论仍在进行中。这一决定于2025年11月19日公布。

---

## 66. Proxmox 虚拟环境 9.1 现已推出

**原文标题**: Proxmox virtual environment 9.1 available

**原文链接**: [https://www.proxmox.com/en/about/company-details/press-releases/proxmox-virtual-environment-9-1](https://www.proxmox.com/en/about/company-details/press-releases/proxmox-virtual-environment-9-1)

Proxmox Server Solutions GmbH宣布Proxmox虚拟环境9.1已于2025年11月19日立即上市，该版本为容器部署、虚拟机安全和软件定义网络带来了显著增强。

本次发布的主要亮点包括：
*   **基于OCI镜像的LXC容器：** 用户现在可以直接从广泛采用的开放容器倡议（OCI）镜像创建LXC容器，从而简化标准化应用程序作为全系统或精简应用容器的部署。
*   **qcow2格式的TPM状态：** 能够在qcow2磁盘镜像中存储虚拟可信平台模块（vTPM）状态，即使在vTPM活动时也能进行完整的虚拟机快照，提高了跨各种存储类型的对安全性敏感的Windows部署的运营灵活性。
*   **嵌套虚拟化的精细控制：** 增强的vCPU标志为专用虚拟机提供了对虚拟化扩展的精确控制，优化了嵌套管理程序或具有基于虚拟化的安全性（VBS）的Windows环境等工作负载。
*   **增强的SDN状态报告：** Web界面现在提供改进的软件定义网络（SDN）堆栈监控和详细报告，显示客户机连接、EVPN区域信息，并将网络结构集成到资源树中，无需命令行即可简化网络故障排除。

Proxmox VE 9.1可通过ISO镜像立即下载，或作为现有安装通过标准APT包管理系统进行升级。作为自由/开源软件（FLOSS），它采用GNU AGPLv3许可。对于企业用户，Proxmox通过订阅计划提供专业支持，起价为每CPU每年115欧元，提供对稳定企业存储库和认证技术支持的访问。Proxmox VE项目在全球拥有超过160万主机和22.5万活跃社区成员。

---

## 67. 玉米站

**原文标题**: CornHub

**原文链接**: [https://cornhub.website/](https://cornhub.website/)

CornHub是一个恶搞网站，模仿了成人娱乐平台的结构和术语，但将所有露骨内容替换为玉米相关主题。该网站提供高清的“全球热门玉米视频”，并提供了一系列玉米主题的标题，例如“跨种族玉米：大黑玉米棒 x 两根混合玉米棒”、“玉米棒体验终极沸腾”以及“玉米粒在集体爆裂事件中变得黏糊糊”。每个视频列表都包含观看次数和满意度百分比，模仿了常见的视频分享网站。

CornHub提供多种语言版本，重点推荐“特色玉米明星”和“最新玉米视频”。该平台拥有“100%免费玉米”内容和“海量免费CCC视频选择”，可供下载或流媒体播放。它将自己定位为“最完整、最具革命性的玉米视频网站”，提供流媒体玉米视频、CCC相册以及“排名第一的免费爆米花社区”，以“保持对玉米的热爱持续旺盛”。

---

## 68. 我为宕机检测器的宕机检测器的宕机检测器做了一个宕机检测器。

**原文标题**: I made a downdetector for downdetector's downdetector's downdetector

**原文链接**: [https://downdetectorsdowndetectorsdowndetectorsdowndetector.com](https://downdetectorsdowndetectorsdowndetectorsdowndetector.com)

位于网址 `https://downdetectorsdowndetectorsdowndetectorsdowndetector.com` 的这篇“作品”是一件概念性作品，其内容主要由一个网页构成。该网站标题为“我为 downdetector 的 downdetector 的 downdetector 制作了一个 downdetector”，而网站本身仅显示“它工作了”这句短语。

这篇“作品”的幽默感和核心主旨，完全源于其极其递归且复杂的标题（该标题暗示了一个旨在检查其他状态检查器状态的深度多层监控系统），与网站实际仅以极简方式确认自身运行状态之间的鲜明对比。它是一个元笑话，巧妙地突出了创建无限嵌套的监控服务的潜在荒谬性或最终的简单性，最终仅仅确认了基本功能。创作者利用这种极简主义方法，对精心设计的系统监控链的概念进行了戏谑嘲讽。

---

## 69. 大语言模型会一本正经地胡说八道，但这不代表它们没用。

**原文标题**: LLMs are bullshitters. But that doesn't mean they're not useful

**原文链接**: [https://blog.kagi.com/llms](https://blog.kagi.com/llms)

本文认为大型语言模型（LLMs）是“胡说八道者”（bullshitters），这个词由哈里·法兰克福定义，指的是那些试图说服他人却不关心真相的人，而非故意歪曲事实的骗子。这种行为源于其核心功能：大型语言模型是复杂的文本预测器，它们根据大量的训练数据生成统计学上最可能的下一个词。它们不“思考”或理解概念；例如，当数字被视为文本字符串时（如3.10与3,10），它们会遇到困难，并且经常输出常见的谜语答案而非逻辑推导结果。

尽管微调可以塑造它们的回复，但如果结合纠正用户输入的指令，它也可能导致自信满满的错误答案或“煤气灯效应”（gaslighting）。作者将大型语言模型比作历史上的智者（Sophists）——它们是实用的问题解决工具，而非智慧的源泉。在重视速度、输出可验证且风险较低的任务中，它们是宝贵的工具，例如写作辅助或编程。

然而，用户必须注意大型语言模型服务于谁的利益，因为模型会从其训练数据和创建者那里继承偏见。此外，大型语言模型只是整个系统的一个组成部分；用户交互和平台设计也至关重要。

至关重要的是，大型语言模型不适合提供情感支持。它们阿谀奉承的行为，尽管在统计学上是可能的且通常能取悦用户，却仅仅是对情感的模仿，并可能通过强化妄想而损害心理健康。尽管存在这些风险，公司仍可能为了用户留存而鼓励这种行为。

总而言之，大型语言模型是强大的工具，但需要审慎使用、持续验证其输出，并理解其固有的局限性和偏见。在关键任务中或作为人际连接的替代品时，不应盲目信任它们。

---

## 70. 研究发现，超加工食品对人体各大主要器官均有害。

**原文标题**: Ultra-processed food linked to harm in every major human organ, study finds

**原文链接**: [https://www.theguardian.com/society/2025/nov/18/ultra-processed-food-linked-to-harm-in-every-major-human-organ-study-finds](https://www.theguardian.com/society/2025/nov/18/ultra-processed-food-linked-to-harm-in-every-major-human-organ-study-finds)

《柳叶刀》杂志上的一项重要科学综述警告称，超加工食品（UPFs）与人体所有主要器官系统的损害有关，对全球健康构成巨大威胁。该研究发现，在英国和美国，UPFs占普通人饮食的一半以上，在年轻人、贫困人口或弱势群体中，这一比例甚至高达80%。

UPFs正在全球范围内迅速取代新鲜食品，并与多种慢性病（包括肥胖症、2型糖尿病、心脏病、抑郁症和过早死亡）的风险增加有关。这种激增是由逐利公司推动的，它们采用激进的营销和游说策略来阻碍监管。根据Nova分类系统定义，UPFs是工业化生产的、适口性极佳的、高热量、低营养的食品，旨在取代更健康的食品选择。

专家们呼吁采取紧急行动，建议加强营销限制（特别是针对儿童），禁止在学校和医院等公共机构中提供UPFs，并限制超市的销售和货架空间。他们强调，企业政治活动而非个人选择，是解决这场“慢性病大流行”的主要障碍。尽管这些建议受到广泛欢迎，一些科学家仍主张在已确立的关联之外，对直接因果关系进行更多研究。巴西旨在纳入90%新鲜或最低限度加工食品的国家学校食品计划，被强调为一个成功的干预措施。

---

## 71. 我简直受够了AI预测内容，赶紧让它消失吧。

**原文标题**: I am just sooo sick of AI prediction content, let's kill it already

**原文链接**: [https://verdikapuku.com/posts/i-am-just-so-sick-of-ai-prediction-content/](https://verdikapuku.com/posts/i-am-just-so-sick-of-ai-prediction-content/)

作者对铺天盖地的“AI预测”内容，例如“AI将如何改变软件工程”之类的标题，表达了极度的不满。他们认为，这类内容多年来一直主导着科技讨论，毫无新意，且通常是由那些试图展现远见的人发表的空泛、重复的预测。

尽管作者是一名应用AI工程师，理应从AI中受益，但他们对这种不断重复旧思想的现象“感到厌烦”，并将其比作大型语言模型（LLMs）本身。他们批评这些文章缺乏新见解、缺乏基于数据的实验、假设的形成或深入的探索。尽管承认AI的真正变革性，作者仍主张停止进行投机性的未来预测。

相反，作者渴望具体、实用且基于真实世界观察的内容。他们更喜欢探讨AI实际应用的文章，详细说明其积极影响、运营挑战和负面发现，举例来说，如“面包店采用AI的3种有趣方式、对其运营的积极影响以及它们发现的弊端”。这番抱怨最后恳求互联网停止产出空泛的“思想领袖”式预测，转而专注于富有洞察力、有数据支持的讨论。

---

## 72. 表情符号证据错误不推翻谋杀定罪

**原文标题**: Emoji evidence errors don’t undo a murder conviction

**原文链接**: [https://blog.ericgoldman.org/archives/2025/11/emoji-evidence-errors-dont-undo-a-murder-conviction-people-v-harmon.htm](https://blog.ericgoldman.org/archives/2025/11/emoji-evidence-errors-dont-undo-a-murder-conviction-people-v-harmon.htm)

在《人民诉哈蒙案》中，德拉罗萨的谋杀罪判决尽管存在与表情符号证据相关的错误，但仍被维持。德拉罗萨对采纳一条带有表情符号的Facebook消息提出上诉，该消息表明他拥有一把枪，他认为这暗示了他“对枪支暴力持轻慢态度”。

执法调查员关于这些表情符号（“笑脸”和“魔鬼角”）的证词并不精确，可能误导了陪审团，因为“喜极而泣的脸”[😂]和“带角的笑脸”[😈]等特定表情符号具有截然不同的含义和多样的视觉呈现。

至关重要的是，在德拉罗萨排除此证据的庭前动议中，提供给审判法官的打印件将表情符号显示为“四个紧密相连的矩形”，而非实际图像。上诉法院以技术理由维持了判决，理由是审判法官驳回该动议并未滥用自由裁量权，因为实际表情符号的视觉影响和潜在推论在该阶段并未被呈现或评估。

作者批判这一结果，认为由于一份模糊不清的证据，德拉罗萨在审判中面对未经审查的表情符号证据是不公平的。尽管承认辩护团队面临巨大压力，但文章强调律师必须确保作为证据引入的表情符号得到准确显示，并考虑到不同平台和历史背景下的不同呈现方式，这一点至关重要。令人沮丧的是，判决书本身并未显示这些表情符号或其矩形替代物。

---

## 73. DOS时代 — 笔记本显示屏

**原文标题**: DOS Days – Laptop Displays

**原文链接**: [https://www.dosdays.co.uk/topics/laptop_displays.php](https://www.dosdays.co.uk/topics/laptop_displays.php)

在DOS时代，笔记本电脑显示器取得了显著发展，以克服早期使用微型CRT的便携式电脑的重量问题。市场迅速转向液晶显示器（LCD）技术，因其节能和紧凑的尺寸。早期的LCD是反射式的，需要环境光，但从1988年起出现了背光和侧光版本，尽管它们仍存在对比度差和刷新率慢导致“鬼影”的问题。

气体等离子显示器提供了更亮、更清晰的图像，并且比CRT更薄。它们使用带电气体像素，产生独特的橙色光芒，但功耗过大，不适合广泛的便携式使用。

超扭曲向列（STN）显示器是一种单色无源矩阵LCD类型，通过进一步扭曲液晶分子实现了更高的分辨率。尽管在没有背光的情况下也能在阳光下阅读，但它们仍然存在鬼影问题。彩色STN笔记本电脑于1989-1990年首次出现。双层超扭曲向列（DSTN）通过分割屏幕提高了刷新率，但仍然呈现出无源矩阵技术固有的低对比度和色彩暗淡问题。

突破性进展出现在薄膜晶体管（TFT）显示器上，也称为“有源矩阵”，大约在1992年中期。TFT屏幕为每个像素配备了独立的晶体管和电容器，消除了无源矩阵的缺点，如鬼影和低对比度。TFT初期价格更高，但提供了快速刷新率和高对比度，到1994年成为彩色笔记本电脑的标准。分辨率从640x480发展到SVGA (800x600)，到1996年甚至达到1024x768，巩固了TFT作为主导技术的地位，该技术至今仍被广泛使用。

---

## 74. 要推出新事物，你需要“社会蒲公英”。

**原文标题**: To launch something new, you need "social dandelions"

**原文链接**: [https://www.actiondigest.com/p/to-launch-something-new-you-need-social-dandelions](https://www.actiondigest.com/p/to-launch-something-new-you-need-social-dandelions)

要推广新想法，你需要“社交蒲公英”——即特定的社群及其中的关键成员。本指南概述了成功的四个步骤。

首先，识别“高增益”社群。这些群体，例如游戏驿站（GameStop）逼空事件中的“华尔街之狼”（WallStreetBets）论坛，具有冒险精神、强烈的群体认同感（通常有明确的“他者”）、原生的叙事方式、内部语言以及对单一话题充满热情且高度专注的特点。这类社群最适合放大新想法。

其次，寻找合适的社群往往需要反复试验。例如，Pinterest最初在硅谷举步维艰，但在发现一批意外的兴趣用户群后，转而锁定中西部女性设计博主，最终取得了突破。即使这些“火花”让你感到意外，也要追随它们。

第三，在这些社群中，首先接触“社交蒲公英”：那些思想开放且社交活跃的个体。1930年代对杂交玉米采纳情况的研究表明，早期采纳者比传统的“领导者”更年轻、受教育程度更高、求知欲更强，并且更积极参与社区活动。现代研究也证实了这一点，例如一项关于中学反欺凌的研究显示，是那些特定的、社交活跃的学生，而非仅仅是“受欢迎的”学生，在传播新规范方面发挥了关键作用。

文章强调，识别并利用这些接受度高、人脉广的个体和社群，对于一个想法获得势头并传播至关重要。

---

## 75. 2025 年 Linux 职业前景：热门技能

**原文标题**: Linux Career Opportunities in 2025: Skills in High Demand

**原文链接**: [https://www.linuxcareers.com/resources/blog/2025/11/linux-career-opportunities-in-2025-skills-in-high-demand/](https://www.linuxcareers.com/resources/blog/2025/11/linux-career-opportunities-in-2025-skills-in-high-demand/)

所提供的文本仅仅是一个标题和导航跳转链接。它写着“2025年Linux职业发展机遇：热门技能——Linux工作与职业”，紧接着是“跳到主导航”和“跳到主要内容”。没有关于Linux领域具体技能、职位角色或机遇的实际文章内容可供总结。

---

## 76. 在 Rust GPU 内核驱动上赛卡丁车

**原文标题**: Racing karts on a Rust GPU kernel driver

**原文链接**: [https://www.collabora.com/news-and-blog/news-and-events/racing-karts-on-a-rust-gpu-kernel-driver.html](https://www.collabora.com/news-and-blog/news-and-events/racing-karts-on-a-rust-gpu-kernel-driver.html)

Collabora宣布，他们为Arm Mali GPU开发的Rust GPU内核驱动Tyr取得了重要的里程碑。Tyr原型最初只是一个基本的任务执行器，现在已成功运行GNOME和Weston等完整的图形环境，以及SuperTuxKart等3D游戏，这表明该Rust驱动功能完善，性能卓越，已与C语言驱动的性能持平。

文章强调了内核模式驱动（KMD）在管理GPU硬件、电源、固件、内存分配、任务提交以及为用户模式驱动（UMD）提供同步方面的关键作用。早期开发侧重于基础任务，从简单的整数放置“虚拟任务”发展到以超过500帧每秒的速度渲染旋转立方体（kmscube），其速度与C语言驱动相当。

进一步的测试显示，Tyr能够渲染GNOME的登录页面，支持网页浏览，并在Weston下运行`vkcube`。最终的成功是SuperTuxKart在全屏模式下运行无性能问题，尽管窗口模式仍存在一些小故障。

Collabora强调，Tyr只是一个原型，而非日常驱动，其中包含了一些在最终上游版本中不会出现的简化。它作为Rust抽象工作的一个重要实验测试平台，证明了Rust GPU KMD是可行且高性能的。尽管目前在Rock 5B开发板（瑞芯微RK3588）上进行的测试不能保证稳定性，但该项目为Rust最终集成到GPU驱动上游奠定了基础。

---

## 77. 致 Cloudflare 的问题

**原文标题**: Questions for Cloudflare

**原文链接**: [https://entropicthoughts.com/questions-for-cloudflare](https://entropicthoughts.com/questions-for-cloudflare)

作者首先回应了对其先前Cloudflare中断分析的批评，澄清其“肤浅”是刻意的，他们没有反应过度，并就任何被认为轻视Cloudflare良好记录的行为表示歉意。他们解释说，事后诸葛亮偏见在事故分析中是固有的，但主张采用STPA等主动方法。

核心论点是Cloudflare的中断总结过于侧重于*控制路径*，而忽略了关键的*反馈路径*。作者认为，中断并非源于控制选项的缺乏（例如，拥有旧的配置文件），而是由于操作员缺乏必要的信息和理解（反馈），无法了解哪里出了问题或如何立即修复。

这引出了Cloudflare的两个关键问题：
1. 他们是否特意为操作员设计了人机界面？
2. 他们是否积极考虑操作员如何全面理解系统行为和故障？
作者推断Cloudflare的报告暗示了这些问题的答案是“否”。

更详细的问题探讨了各种系统交互：Bot Management的超时行为、其对不再存在的请求的处理，以及与其他服务潜在的通信故障。作者还质疑了内部协议的规范和合规性跟踪、工程师如何管理跨服务通信，以及事件期间操作员工具和重新配置决策的反馈机制。

文章最后敦促技术组织采用STPA等系统化、主动的安全分析方法，以便在系统弱点导致中断之前将其识别出来。

---

## 78. 各种 Unix 版本上的 shebang/hash-bang 机制详解 (2001)

**原文标题**: Details about the shebang/hash-bang mechanism on various Unix flavours (2001)

**原文链接**: [https://www.in-ulm.de/%7Emascheck/various/shebang/](https://www.in-ulm.de/%7Emascheck/various/shebang/)

shebang (`#!`) 机制起源于贝尔实验室（Dennis Ritchie，在V7和V8之间），并于1980年在4.0BSD中首次广泛分发，1983年在4.2BSD中成为默认。早期实现有严格的行长度限制（16-32字节），并且最初不传递参数。

一个常见的误解是，`#!` 后必须有一个空格；这是不正确的，因为4.2BSD接受但并非强制要求。

脚本的Setuid/gid支持通常因竞态条件等安全问题而被禁用。现代系统（例如SVR4，以及NetBSD、OpenBSD、Solaris、MacOS X 10.5+等4.4BSD派生系统）通过使用虚拟文件描述符文件系统（`/dev/fd/n`），将一个打开的文件句柄传递给解释器来解决此问题，尽管可能需要内核激活。SVR4 shell还为setuid脚本引入了`-p`标志。

嵌套的`#!`脚本（即解释器本身也是一个`#!`脚本）通常不被传统的Unix内核支持。然而，Linux（自2.6.27.9版本起）和Minix允许最多四级嵌套。如果内核失败，shell可能会默默地尝试解释该脚本。参数分割方式各异；大多数系统将所有`#!`参数作为一个单一字符串传递。

`env`工具（`#!/usr/bin/env prog`）常用于实现可移植性，但`env`自身的位置在不同系统上可能不同（`/usr/bin/env` vs `/bin/env`）。`#!`行最大长度已显著演变，从历史上的16-32字节，到127字节（Linux）、`_POSIX_PATH_MAX`（255）、`PATH_MAX`（1024），甚至`PAGESIZE`（FreeBSD 6.0+上的4096/8192）。

---

## 79. 老旧三星手机在澳关联致命紧急呼叫失败

**原文标题**: Outdated Samsung handset linked to fatal emergency call failure in Australia

**原文链接**: [https://www.theregister.com/2025/11/18/samsung_emergency_call_failure/](https://www.theregister.com/2025/11/18/samsung_emergency_call_failure/)

悉尼一名居民因其老旧的三星手机无法拨通澳大利亚的000紧急电话而悲剧性身亡，这促使电信公司TPG Telecom发出了严厉警告。TPG证实，上周，该用户使用其网络上的Lebara品牌服务，无法拨打紧急电话。

TPG坚称其网络运行正常，初步调查指向该用户使用的三星设备运行的软件已不再兼容紧急呼叫功能。该电信公司表示，它已在“某些旧设备”中发现了这一问题，包括Galaxy S7和Note 5系列，并曾多次警告用户更新手机，最近一次警告是在11月7日。联邦法规要求运营商在28-35天后，如果未打补丁的手机无法拨打000紧急电话，就必须将其禁用，TPG称其已遵循了这一规定。

TPG首席执行官Iñaki Berroeta敦促所有使用过时软件的客户立即更换或更新他们的设备。三星公司最初未作回应，随后表达了哀悼，并强烈鼓励客户为了安全、保障和性能，保持其移动设备更新。

此事件此前，Telstra也曾就老旧三星设备发出过类似警告，并且发生在公众对紧急呼叫可靠性日益关注之际，尤其是在今年早些时候Optus的一次故障导致紧急呼叫中断14小时并与三起死亡事件相关联之后。TPG已在其调查进行中通知了相关的联邦和州当局。

---

## 80. 当连大学生都不会数学了，会怎么样？

**原文标题**: What happens when even college students can't do math anymore?

**原文链接**: [https://www.theatlantic.com/ideas/2025/11/math-decline-ucsd/684973/](https://www.theatlantic.com/ideas/2025/11/math-decline-ucsd/684973/)

美国大学生的数学能力正面临严重下降，典型例子是加州大学圣地亚哥分校，在该校，数学技能低于高中水平的新生人数在五年内从30人跃升至900多人；许多学生连分数和基本代数等初中概念都感到吃力。这一普遍问题不仅存在于加州大学各分校，在全国范围内也可见一斑，根据全国评估，目前八年级学生的平均数学技能比2013年水平落后整整一个学年。

导致这场“显而易见的灾难”的原因有多种。智能手机和社交媒体的兴起可能导致注意力缺陷，而包括人工智能在内的技术可能助长自满情绪，使学生认为基础数学不再重要。2015年以来，教育政策的转变也发挥了作用，这些政策脱离了问责制，并强调“引人入胜”的数学而非基于证据的教学。新冠疫情则显著加速了这种下降，远程学习导致标准放宽、“零分禁令”政策和成绩虚高；许多高中数学成绩全A的学生现在却需要小学水平的补习。

雪上加霜的是，加州大学系统于2020年取消了招生中对标准化考试成绩（SAT/ACT）的要求，从而取消了一个衡量数学能力的关键指标，并增加了来自资源不足学校的招生人数。最近一份报告建议恢复标准化考试，但学者们一致认为，这并不能解决普遍存在的数字盲这一根本问题。专家们警告不要依赖人工智能来取代基础数学技能，称这种做法是“通向愚蠢社会的秘诀”，并预测量化能力下降将带来巨大的经济损失。

---

## 81. HN 展示：Awesome J2ME

**原文标题**: Show HN: Awesome J2ME

**原文链接**: [https://github.com/hstsethi/awesome-j2me](https://github.com/hstsethi/awesome-j2me)

“Awesome J2ME”是一个全面精选列表，专门介绍 Java 平台微型版 (J2ME)，这是一种用于老式按键手机和 PDA 的 Java 规范，主要使用 MIDP 创建 Midlet（.jad/.jar 文件）。该项目旨在提高 J2ME 社区的知名度并提供支持，并已被其他多个“Awesome”列表收录。

该列表分为众多类别，为爱好者和开发者提供了丰富的资源。它重点介绍了活跃的**社区**，例如 Kahvibreak Discord 和 r/J2MEGaming，以及像 Ketai Wiki 这样的保存项目。**开发**工具包括 C/C++ 编译器 (Cibyl)、JSON 解析器、UI 工具包 (LWUIT) 和 Gradle 模板。列表中收录了必不可少的 **IDE**，如 Eclipse 和 NetBeans 6.1，以及 Sun WTK 和 J2ME Polish 等 **SDK**。

为了方便现代访问，**模拟器**部分收录了 FreeJ2ME、J2ME Loader（适用于 Android）、KEmulator nnmod 和 PSPkvm。**原生软件**涵盖了现代非官方应用，如 Discord J2ME 和 Jtube（YouTube 客户端）、MeBoy GBC 模拟器，甚至还有印度官方的 UPI 123PAY。**视频游戏**部分指向了大量存档（Kahvibreak、MyAbandonware）和速通资源。

其他类别深入探讨了**硬件**（手机博物馆）、**相关项目**（Awesome Symbian）、**逆向工程**工具、各种**反编译器**（Fernflower、Jd Decompiler）、实用的**教程**以及精选的**学术文章**，探讨 J2ME 开发和应用的各个方面。此列表是关于 J2ME 的一个中心枢纽，涵盖了从历史保存到开发见解的所有内容。

---

## 82. 劳工部不会公布十月失业率

**原文标题**: Labor Department Won't Publish October Unemployment Rate

**原文链接**: [https://www.wsj.com/economy/bls-to-publish-november-jobs-data-on-december-16-b9baab5c](https://www.wsj.com/economy/bls-to-publish-november-jobs-data-on-december-16-b9baab5c)

无法访问文章链接。

---

## 83. 展示 HN: Marimo VS Code 扩展 – 基于 LSP 和 uv 构建的 Python 笔记本

**原文标题**: Show HN: Marimo VS Code extension – Python notebooks built on LSP and uv

**原文链接**: [https://github.com/marimo-team/marimo-lsp](https://github.com/marimo-team/marimo-lsp)

本公告推出`marimo-lsp`，这是一个全新的VS Code扩展，专门为`marimo` Python笔记本集成了语言服务器。标题阐明，`marimo`笔记本利用语言服务器协议（LSP）和`uv`作为其底层架构。对`marimo-lsp`感兴趣的用户，可通过所提供的链接获取该扩展的更多详细信息，并了解如何为其开发做出贡献。

---

## 84. 欧洲的Cookie噩梦正在瓦解。欧委会希望在浏览器层面设置偏好。

**原文标题**: Europe's cookie nightmare is crumbling. EC wants preference at browser level

**原文链接**: [https://www.theverge.com/news/823788/europe-cookie-prompt-browser-changes-proposal](https://www.theverge.com/news/823788/europe-cookie-prompt-browser-changes-proposal)

The European Commission is proposing significant changes to Europe's cookie consent policies, aiming to end the "cookie nightmare" of constant pop-ups since their introduction in 2018. The core proposal is for users to manage their cookie preferences centrally at the browser level, rather than encountering a pop-up on every website. This means users could set their privacy choices once, and websites would be legally required to respect these preferences, simplifying the online experience.

As an initial step, cookie prompts will be simplified to a single-click "yes" or "no" option. Additionally, websites will be mandated to respect user choices for at least six months, and cookie banners will be discouraged for "harmless uses" like merely counting website visits. The Commission argues that the current system often forces users to accept cookies due to annoyance, undermining genuine privacy choices. The new rules aim to modernize these protections, giving citizens real control over cookie placement and their data.

These proposals will now proceed to the European Parliament and require approval from the 27 member states. While the process may take time, it marks a significant step towards streamlining web browsing and enhancing user privacy in Europe.

---

## 85. Implementation of a Java Processor on a FPGA (2016)

**原文标题**: Implementation of a Java Processor on a FPGA (2016)

**原文链接**: [https://mavmatrix.uta.edu/electricaleng_theses/337/](https://mavmatrix.uta.edu/electricaleng_theses/337/)

生成摘要时出错

---

## 86. Pozsar's Bretton Woods III: The Framework

**原文标题**: Pozsar's Bretton Woods III: The Framework

**原文链接**: [https://philippdubach.com/2025/10/25/pozsars-bretton-woods-iii-the-framework-1/2/](https://philippdubach.com/2025/10/25/pozsars-bretton-woods-iii-the-framework-1/2/)

生成摘要时出错

---

## 87. Adventures in upgrading Proxmox

**原文标题**: Adventures in upgrading Proxmox

**原文链接**: [https://blog.vasi.li/adventures-in-upgrading-proxmox/](https://blog.vasi.li/adventures-in-upgrading-proxmox/)

生成摘要时出错

---

## 88. Go Cryptography State of the Union

**原文标题**: Go Cryptography State of the Union

**原文链接**: [https://words.filippo.io/2025-state/](https://words.filippo.io/2025-state/)

生成摘要时出错

---

## 89. New Arduino T&C: "user shall not [...] reverse-engineer the platform"

**原文标题**: New Arduino T&C: "user shall not [...] reverse-engineer the platform"

**原文链接**: [https://bsky.app/profile/ptorrone.bsky.social/post/3m5wcakoip22u](https://bsky.app/profile/ptorrone.bsky.social/post/3m5wcakoip22u)

生成摘要时出错

---

## 90. Roblox Requires Age Checks for Communication, Ushering in New Safety Standard

**原文标题**: Roblox Requires Age Checks for Communication, Ushering in New Safety Standard

**原文链接**: [https://corp.roblox.com/newsroom/2025/11/roblox-requires-age-checks-limits-minor-and-adult-chat](https://corp.roblox.com/newsroom/2025/11/roblox-requires-age-checks-limits-minor-and-adult-chat)

生成摘要时出错

---

## 91. Free interactive tool that shows you how PCIe lanes work on motherboards

**原文标题**: Free interactive tool that shows you how PCIe lanes work on motherboards

**原文链接**: [https://mobomaps.com](https://mobomaps.com)

生成摘要时出错

---

## 92. Tesla Robotaxi had 3 more crashes, now 7 total

**原文标题**: Tesla Robotaxi had 3 more crashes, now 7 total

**原文链接**: [https://electrek.co/2025/11/17/tesla-robotaxi-had-3-more-crashes-now-7-total/](https://electrek.co/2025/11/17/tesla-robotaxi-had-3-more-crashes-now-7-total/)

生成摘要时出错

---

## 93. Workday to acquire Pipedream

**原文标题**: Workday to acquire Pipedream

**原文链接**: [https://newsroom.workday.com/2025-11-19-Workday-Signs-Definitive-Agreement-to-Acquire-Pipedream](https://newsroom.workday.com/2025-11-19-Workday-Signs-Definitive-Agreement-to-Acquire-Pipedream)

生成摘要时出错

---

## 94. YouTube Is Awful. I'm Not Posting There Anymore

**原文标题**: YouTube Is Awful. I'm Not Posting There Anymore

**原文链接**: [https://joshgriffiths.site/youtube-is-awful-im-not-posting-there-anymore/](https://joshgriffiths.site/youtube-is-awful-im-not-posting-there-anymore/)

生成摘要时出错

---

## 95. What nicotine does to your brain

**原文标题**: What nicotine does to your brain

**原文链接**: [https://economist.com/science-and-technology/2025/09/12/what-nicotine-does-to-your-brain](https://economist.com/science-and-technology/2025/09/12/what-nicotine-does-to-your-brain)

生成摘要时出错

---

## 96. GOP overhaul of broadband permit laws: Cities hate it, cable companies love it

**原文标题**: GOP overhaul of broadband permit laws: Cities hate it, cable companies love it

**原文链接**: [https://arstechnica.com/tech-policy/2025/11/gop-overhaul-of-broadband-permit-laws-cities-hate-it-cable-companies-love-it/](https://arstechnica.com/tech-policy/2025/11/gop-overhaul-of-broadband-permit-laws-cities-hate-it-cable-companies-love-it/)

生成摘要时出错

---

## 97. Ford can't find mechanics for $120K: It takes math to learn a trade

**原文标题**: Ford can't find mechanics for $120K: It takes math to learn a trade

**原文链接**: [https://www.joannejacobs.com/post/ford-can-t-find-mechanics-for-120k-it-takes-math-to-learn-a-trade](https://www.joannejacobs.com/post/ford-can-t-find-mechanics-for-120k-it-takes-math-to-learn-a-trade)

生成摘要时出错

---

## 98. Debunking the Myths of the HBO Chernobyl series (2023)

**原文标题**: Debunking the Myths of the HBO Chernobyl series (2023)

**原文链接**: [https://blog.osm-ai.net/investigation/2023/01/05/hbo-chernobyl-myth.html](https://blog.osm-ai.net/investigation/2023/01/05/hbo-chernobyl-myth.html)

生成摘要时出错

---

## 99. Show HN: DNS Benchmark Tool – Compare and monitor resolvers

**原文标题**: Show HN: DNS Benchmark Tool – Compare and monitor resolvers

**原文链接**: [https://github.com/frankovo/dns-benchmark-tool](https://github.com/frankovo/dns-benchmark-tool)

生成摘要时出错

---

## 100. Lucent 7 R/E 5ESS Telephone Switch Rescue (2024)

**原文标题**: Lucent 7 R/E 5ESS Telephone Switch Rescue (2024)

**原文链接**: [http://kev009.com/wp/2024/07/Lucent-5ESS-Rescue/](http://kev009.com/wp/2024/07/Lucent-5ESS-Rescue/)

生成摘要时出错

---

