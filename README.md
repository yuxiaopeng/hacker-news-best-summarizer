# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-01-16.md)

*最后自动更新时间: 2026-01-16 19:49:23*
## 1. 克劳德协同文件外传

**原文标题**: Claude Cowork exfiltrates files

**原文链接**: [https://www.promptarmor.com/resources/claude-cowork-exfiltrates-files](https://www.promptarmor.com/resources/claude-cowork-exfiltrates-files)

本文详细介绍了一个 Anthropic 的 Claude Cowork 中存在的严重文件窃取漏洞，该漏洞源于 Claude 代码执行环境中未修复的隔离缺陷。这个漏洞曾由 Johann Rehberger 在 Claude.ai 中披露，它使攻击者能够通过间接的提示注入窃取用户文件。

Anthropic 建议用户留意“可疑行为”，并避免授予 Cowork 访问敏感本地文件的权限，但作者认为，对于非技术用户而言，这一建议不切实际。

攻击链涉及受害者将 Cowork 连接到本地文件夹，并上传一个看似无害的文件，例如伪装成“技能”的 `.docx` 文件。该文件包含一个隐藏的提示注入，通过微小的白色文本和紧密的行间距使其不可见。当受害者提示 Cowork 分析文件时，隐藏注入会操控 Cowork 执行一个 `curl` 命令。该命令利用 Claude 虚拟机中允许列表的 Anthropic API，使用攻击者的 API 密钥，将受害者本地目录中最大的可用文件直接上传到攻击者的 Anthropic 账户。整个过程无需人工批准，从而实现敏感数据（如财务数据和个人身份信息 (PII)）的外泄。

该漏洞利用已在 Claude Haiku 上演示，并在 Cowork 中的 Claude Opus 4.5 上成功复现。文章还强调了一个使用格式错误文件可能导致的拒绝服务漏洞，并警告称，Cowork 的“代理特性”及其连接器通过与不可信数据源交互，显著扩大了提示注入的攻击面。敦促用户务必保持高度警惕。

---

## 2. 让你的链接尽可能可疑的URL缩短器

**原文标题**: The URL shortener that makes your links look as suspicious as possible

**原文链接**: [https://creepylink.com/](https://creepylink.com/)

CreepyLink 是一个独特的网址缩短服务，它幽默地旨在让链接看起来尽可能可疑，与标准“可信”链接形成对比。用户可以生成并复制这些“可疑的缩短网址”。该平台包含一个问题报告功能。

文本的很大一部分涉及法律问题，澄清 CreepyLink 旨在作为一个玩笑。作者声明该服务包含重定向页面，以告知用户其目的地，并强调它并非旨在“削弱全球网络安全防护能力”或助长网络钓鱼。作者断言该网站遵守所有已知法律和政策，并且之前法律威胁中提出的合理担忧已得到解决。他们请求未来任何问题或疑虑都通过电子邮件直接沟通，而不是收到法律威胁。

---

## 3. 苹果争抢台积电产能，英伟达抢尽风头。

**原文标题**: Apple is fighting for TSMC capacity as Nvidia takes center stage

**原文链接**: [https://www.culpium.com/p/exclusiveapple-is-fighting-for-tsmc](https://www.culpium.com/p/exclusiveapple-is-fighting-for-tsmc)

长期以来作为台积电最大客户的苹果，如今正积极争夺芯片产能，因为英伟达日益占据主导地位。这家iPhone制造商面临显著的价格上涨和优先级降低，英伟达在最近几个季度很可能已超越它成为台积电的第一大客户，这一趋势预计将持续到2026年。

这一转变的驱动力是蓬勃发展的AI产业，这推动了英伟达和AMD等公司对高性能计算（HPC）芯片的巨大需求。相比之下，作为苹果主要业务领域的智能手机市场已陷入停滞。台积电去年的HPC收入飙升了48%，而智能手机收入仅增长了11%。

台积电正利用其日益增长的定价权，实现了创纪录的毛利率，并预测收入将大幅增长。它计划在2026年投入创纪录的资本支出（520亿至560亿美元），用于开发N2和A16等先进工艺节点，其中A16专门为HPC优化，将使英伟达受益。

尽管近期产能吃紧，苹果因其多样化的芯片产品组合和在台积电众多晶圆厂的广泛制造足迹而依然至关重要，这提供了稳定性。预计在2028年左右推出的A14节点，专为移动和HPC设计，有可能使产能重新向苹果倾斜。

台积电为其谨慎的产能扩张辩护，强调新晶圆厂建设需要两到三年时间，以及如果未来需求下降将面临巨大的财务风险。与英伟达等无晶圆厂客户不同，台积电承担着沉重的资本和折旧成本，这使得审慎投资至关重要。黄仁勋（英伟达）在争取台积电尖端晶圆供应方面，如今比蒂姆·库克（苹果）拥有更大的权力。

---

## 4. 照片捕捉中国风光建设的惊人规模。

**原文标题**: Photos capture the breathtaking scale of China's wind and solar buildout

**原文链接**: [https://e360.yale.edu/digest/china-renewable-photo-essay](https://e360.yale.edu/digest/china-renewable-photo-essay)

这篇文章强调了中国风能和太阳能扩张的巨大规模，去年全球新增风能和太阳能装机容量中，超过一半来自中国。仅在去年五月，中国新增的可再生能源发电量就足以满足波兰全国的用电需求，其太阳能电池板的安装速度达到惊人的每秒100块。

这种迅猛发展遍及全国，从拥挤的东部城市的屋顶太阳能板，到偏远西部沙漠的巨型风力发电场。摄影师褚卫民耗时三年，利用无人机从空中视角捕捉了这一转型，揭示了这些设施与山脉、沙漠和海洋等自然景观之间形成的几何图案。他的作品汲取了中国传统水墨画的灵感，并在一个获奖的绿色和平组织展览中展出。

褚卫民在进行风光摄影时，多次遇到这些可再生能源设施，从而意识到记录它们的重要性，他将其定义为“我们时代的故事”。随附的照片展示了各种各样的设施，从风景区和湿地附近的风力发电场，到滩涂上、有羊群放牧的沙漠中以及城市屋顶上的太阳能发电场，生动地说明了中国清洁能源转型的空前规模。

---

## 5. Palantir 应用协助 ICE 在明尼阿波利斯突袭

**原文标题**: The Palantir app helping ICE raids in Minneapolis

**原文链接**: [https://www.404media.co/elite-the-palantir-app-ice-uses-to-find-neighborhoods-to-raid/](https://www.404media.co/elite-the-palantir-app-ice-uses-to-find-neighborhoods-to-raid/)

404 Media 披露了 Palantir 为美国移民和海关执法局 (ICE) 开发的一款工具的细节，该工具旨在协助识别和定位潜在的驱逐目标。据报道，该工具能够在地图上标示出这些目标，提供个人档案，并为他们的当前地址分配一个“置信度评分”。其目的是帮助 ICE 确定可能拘留的许多人所居住的区域。

这些发现来源于 ICE 内部材料、公共采购记录以及一名 ICE 官员最近的宣誓证词，确立了 Palantir 技术与 ICE 行动活动之间的明确联系。该工具从包括美国卫生与公众服务部 (HHS) 在内的多个来源收集人们的地址信息。

这一披露正值联邦机构在明尼阿波利斯增加部署，国土安全部 (DHS) 负责人 Kristi Noem 在大规模抗议活动中派遣了数百名联邦探员。最近的事件包括一名 ICE 官员射杀了一名 37 岁的美国公民 Renee Nicole Good。此外，在被称为“有史以来最大规模移民行动”的“都市突击行动”（Operation Metro Surge）中，据报道移民探员包围了网约车司机，并对高中生使用了胡椒喷雾。

---

## 6. Pocket TTS：高质量文本转语音，让你的CPU拥有声音

**原文标题**: Pocket TTS: A high quality TTS that gives your CPU a voice

**原文链接**: [https://kyutai.org/blog/2026-01-13-pocket-tts](https://kyutai.org/blog/2026-01-13-pocket-tts)

所提供的文本仅包含一篇博客文章的标题和日期：“Pocket TTS: 一款让你的CPU拥有声音的高质量TTS 2026年1月13日。”

它不包含实际的文章内容。因此，由于没有正文可供分析，我无法提供主要观点或关键信息的摘要。

要提供摘要，请提供博客文章的完整内容。

---

## 7. 当互联网中断时，Briar 通过蓝牙和Wi-Fi 保持伊朗的连接。

**原文标题**: Briar keeps Iran connected via Bluetooth and Wi-Fi when the internet goes dark

**原文链接**: [https://briarproject.org/manual/fa/](https://briarproject.org/manual/fa/)

Briar是一款去中心化消息应用程序，专为安全通信设计，在审查环境或互联网无法访问时尤其有价值。与传统即时通讯工具不同，Briar无需中央服务器运行，直接在用户设备之间同步消息。当互联网中断时，它可以通过蓝牙或Wi-Fi连接，确保危机期间的信息流通。当互联网可用时，Briar利用Tor网络，包括“桥接器”，来保护用户隐私和绕过审查。

该应用可通过Google Play、F-Droid或直接下载安装到Android设备。创建账户需要选择一个别名和设置一个强密码；账户信息本地存储在设备上，如果删除或忘记，则无法恢复。

可以通过分享独特的`briar://`链接远程添加联系人，或者通过扫描二维码在面对面安全添加。所有私密消息都经过端到端加密。

Briar提供多种通信工具：
*   **私密消息：** 加密的点对点聊天。
*   **介绍联系人：** 允许用户将其联系人相互连接。
*   **私人群组：** 由创建者管理的群聊，支持线程消息。
*   **论坛：** 公开对话，任何成员都可以邀请他人加入。
*   **博客：** 自动与联系人分享的个人博客，支持转发和集成RSS订阅，RSS订阅通过Tor下载以保护隐私。

设置允许自定义主题，控制互联网连接（包括使用Tor网络，无论是否带桥接器；移动数据使用；以及仅在充电时连接），以及具有不活动超时功能的屏幕锁定，以增强隐私。删除联系人会将其从列表中移除，但不会发送通知。

---

## 8. 25 Years of Wikipedia

**原文标题**: 25 Years of Wikipedia

**原文链接**: [https://wikipedia25.org](https://wikipedia25.org)

生成摘要时出错

---

## 9. Cloudflare acquires Astro

**原文标题**: Cloudflare acquires Astro

**原文链接**: [https://astro.build/blog/joining-cloudflare/](https://astro.build/blog/joining-cloudflare/)

生成摘要时出错

---

## 10. ‘ELITE’: The Palantir app ICE uses to find neighborhoods to raid

**原文标题**: ‘ELITE’: The Palantir app ICE uses to find neighborhoods to raid

**原文链接**: [https://werd.io/elite-the-palantir-app-ice-uses-to-find-neighborhoods-to-raid/](https://werd.io/elite-the-palantir-app-ice-uses-to-find-neighborhoods-to-raid/)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 2 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 3 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 4 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 5 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 6 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 7 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 8 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 9 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 10 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 11 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 12 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 13 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 14 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 15 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 16 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 17 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 18 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 19 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 20 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 21 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 22 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 23 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 24 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 25 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 26 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 27 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 28 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 29 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 30 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 31 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 32 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 33 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 34 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 35 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 36 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 37 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 38 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 39 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 40 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 41 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 42 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 43 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 44 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 45 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 46 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 47 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 48 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 49 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 50 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 51 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 52 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 53 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 54 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 55 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 56 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 57 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 58 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 59 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 60 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 61 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 62 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 63 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 64 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 65 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 66 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 67 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 68 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 69 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 70 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 71 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
| 72 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
