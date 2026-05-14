# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-05-14.md)

*最后自动更新时间: 2026-05-14 21:03:47*
## 1. 我把我的数字栈搬到了欧洲。

**原文标题**: I moved my digital stack to Europe

**原文链接**: [https://monokai.com/articles/how-i-moved-my-digital-stack-to-europe/](https://monokai.com/articles/how-i-moved-my-digital-stack-to-europe/)

作者详细介绍了他们如何出于对数字主权的承诺，刻意将个人和商业数字技术栈迁移到欧洲基础设施。对美国服务的不满源于对数据控制、不确定的司法管辖权以及激励机制错位的担忧，促使他们寻求符合个人价值观并遵守GDPR的基础设施。

主要的迁移包括：将Google Analytics切换为自托管的Matomo；将Google Workspace和1Password切换为瑞士的Proton Mail和Proton Pass；将DigitalOcean/AWS的计算和对象存储服务切换为Scaleway。异地备份从Backblaze迁移到OVHcloud；事务性邮件从SendGrid迁移到Lettermint；错误跟踪从Sentry迁移到自托管的Bugsink；AI API集成从OpenAI迁移到Mistral。

然而，有些服务保持不变。Cloudflare因其强大的功能和数据固有的公共性质，被保留用于面向公众的CDN服务。Stripe（支付）因集成复杂性而被推迟，尽管Mollie被确定为一个欧洲替代方案。在AI代码辅助方面，作者从OpenAI转向了美国公司Anthropic的Claude Code，优先考虑其质量和价值观，同时也注意到像Qwen这样有能力的本地模型的崛起。GitHub因其强大的网络效应，仍用于面向公众的开源项目。

尽管最初遇到了一些磨合和研究，但这些迁移在两个月内顺利完成，未发生任何事故，总体上是可控且成功的。作者总结道，主要依靠欧洲基础设施运行一个可靠、专业的数字技术栈是完全可行的，并强调将对数据和基础设施的自主控制作为核心原则。

---

## 2. 恢复对 Bambu Lab 打印机的完整 BambuNetwork 支持

**原文标题**: Restore full BambuNetwork support for Bambu Lab printers

**原文链接**: [https://github.com/FULU-Foundation/OrcaSlicer-bambulab](https://github.com/FULU-Foundation/OrcaSlicer-bambulab)

本次 OrcaSlicer 发布重新为 Bambu Lab 打印机启用了完整的 BambuNetwork 支持，允许用户像以前一样通过互联网全面地打印和管理他们的设备。它不再仅限于局域网操作。

安装说明：
*   **Windows:** 需要 WSL 2。首次启动前，用户必须在管理员权限的命令提示符或 PowerShell 中运行两条 `dism.exe` 命令，以启用 `Microsoft-Windows-Subsystem-Linux` 和 `VirtualMachinePlatform` 功能，然后在打开 Orca Studio 前重启 Windows。
*   **Linux:** 标准安装过程即可。
*   **macOS:** 目前正在开发支持中。

作者还建议使用 BMCU 固件，该固件可在其存储库中找到。

---

## 3. 离开 GitHub 转向 Forgejo

**原文标题**: Leaving GitHub for Forgejo

**原文链接**: [https://jorijn.com/en/blog/leaving-github-for-forgejo/](https://jorijn.com/en/blog/leaving-github-for-forgejo/)

作者出于对数字自主权和所有权的担忧，将其代码从GitHub迁移到了自托管的Forgejo实例`code.jorijn.com`，此举也得到了荷兰政府的响应。

离开GitHub的决定源于以下几个因素：
1.  **缺乏独立领导层：** GitHub于2025年8月被并入微软的CoreAI部门，失去了其首席执行官和独立领导权，使其成为微软人工智能组织的一个单位。
2.  **AI训练数据默认设置：** 自2026年4月24日起，Copilot Free、Pro和Pro+的用户交互数据成为默认用于AI训练，用户需选择退出，且没有仓库级别的控制权，这意味着无论代码库的许可如何，都可能成为训练材料。
3.  **美国管辖权风险：** 作为一家美国公司，GitHub无论数据驻留何处，都受美国法律（《外国情报监视法》第702条、CLOUD法案）的管辖，使数据面临美国政府潜在的秘密访问风险。尽管频繁发生服务中断，但这些被视为GitHub激进AI战略的征兆。

荷兰内政部也为`code.overheid.nl`选择了Forgejo，因为它是一个完全开源的项目，没有开放核心（open-core）拆分，并提供了数字自主所需的自由，这与他们的“开放，除非”（Open, tenzij）政策相符。

作者选择Forgejo而非GitLab，是因为Forgejo采用GPLv3+ copyleft许可证，并在Codeberg e.V.的非营利组织治理下，这确保了社区的控制权并抵制了商业侵占。

作者的设置是在一台Intel NUC上运行Forgejo v15 LTS。一个关键的安全重点是执行不受信任代码的Forgejo Actions runner。它采用了多层防御机制：KVM隔离的虚拟机、使用gVisor作为Docker运行时、每周从全新的基础镜像进行破坏性重建，以及`nftables`出站过滤器，以确保隔离和安全。

---

## 4. 设置免费的 *.city.state.us 地方域名 (2025年)

**原文标题**: Setting up a free *.city.state.us locality domain (2025)

**原文链接**: [https://fredchan.org/blog/locality-domains-guide/](https://fredchan.org/blog/locality-domains-guide/)

本文详细介绍了如何在美国获取免费的`*.city.state.us`地方域名。这些域名于1992年首次创建，要求申请人必须是美国公民/居民或美国境内的组织。

这个过程包含五个主要步骤：

1.  **选择一个地方域名：** 查阅已授权子域名的旧列表，以找到管理您所需`city.state.us`域名（例如`seattle.wa.us`）的注册商的电子邮件地址。您可能需要寻找更新的联系方式。如果您的特定地方域名未被授权，您可以尝试`gen.your-state.us`。未授权的域名通常保留给政府机构。
2.  **获取名称服务器：** 由于您在注册前需要名称服务器，请使用Amazon Lightsail的免费DNS区域功能。创建一个AWS账户，导航到Lightsail，为您打算使用的域名创建一个DNS区域，并记下提供的名称服务器地址。
3.  **填写 .US 临时域名模板 v2.0：** 请用您选择的域名、个人地址（如果用于个人用途）、用途描述、您作为管理联系人和技术联系人的详细联系方式，以及Lightsail的名称服务器（包括通过DNS查找获得的IP地址）填写此表格。对于美国连接要求（US Nexus），请选择“personal use”（个人用途）和“Natural person who is a United States Citizen”（美国公民自然人）。
4.  **发送表格并等待：** 将填好的表格通过电子邮件发送给在步骤1中确定的注册商。注册是手动完成的，可能需要数天或数周。
5.  **在Lightsail中完成DNS设置：** 注册成功后，返回您的Lightsail DNS区域，创建DNS记录（A、CNAME等），将您的新域名指向您的网络主机或其他服务器。

值得注意的是，这些域名的WHOIS查询不会显示个人地址，只会显示注册商信息。文章还指出，所选区域内的地理居住地要求可能不会被严格执行。

---

## 5. 科恩布鲁斯校长关于资金与人才输送的致辞

**原文标题**: A message from President Kornbluth about funding and the talent pipeline

**原文链接**: [https://president.mit.edu/writing-speeches/video-transcript-message-president-kornbluth-about-funding-and-talent-pipeline](https://president.mit.edu/writing-speeches/video-transcript-message-president-kornbluth-about-funding-and-talent-pipeline)

麻省理工学院院长萨莉·科恩布鲁斯发布了一份关于学院面临的关键挑战的最新报告：资金和人才储备。

一年多来，麻省理工学院一直在应对因其捐赠基金被征收8%税款而加剧的预算压力。尽管进行了内部削减，财政前景依然严峻。联邦拨款虽然国会部分恢复，但未能如预期般拨付给麻省理工学院。与去年相比，联邦校园研究活动和新获资助项目均下降了20%以上。因此，麻省理工学院的联邦和非联邦来源的总资助研究活动比一年前减少了10%——这对学院来说是一个重大损失。

人才储备也受到了影响。政策变化正在阻碍国际学生，而联邦资金的不确定性使得各系对招收新的研究生持谨慎态度。今年研究生入学人数有所下降，预计明年将下降近20%（斯隆管理学院之外约500名学生）。这对麻省理工学院来说，意味着“创新才华”的严重流失，也意味着国家未来科学家数量的减少。

为解决这些问题，麻省理工学院正积极寻求新的途径。教职员工正在为新兴的联邦机会（例如，为美国能源部“创世纪任务”提交了176份提案）制定方案。学院正在寻求新的产业资金，探索通过教育产品创收，并加大慈善募捐力度。至关重要的是，麻省理工学院正在华盛顿加大游说力度，反对征收捐赠基金税，并倡导好奇心驱动的科学所带来的变革性影响，科恩布鲁斯院长频繁会见各界领袖，以宣传麻省理工学院的价值。

---

## 6. 小型企业克劳德

**原文标题**: Claude for Small Business

**原文链接**: [https://www.anthropic.com/news/claude-for-small-business](https://www.anthropic.com/news/claude-for-small-business)

Anthropic于2026年5月13日推出了“Claude小企业版”，这是一项新产品，旨在通过将Claude直接整合到现有工具中，帮助小企业利用AI。尽管小企业对美国经济做出了重大贡献，但这项举措旨在解决它们在AI采用方面滞后的问题。

该套餐为Intuit QuickBooks、PayPal、HubSpot、Canva、Docusign、Google Workspace和Microsoft 365等常用平台提供连接器和即时可用的工作流。用户可以“切换安装”Claude，以自动化规划薪资、月度结算、开展销售活动和催收发票等任务。它在Claude Cowork中运行，提供跨财务、运营、销售、营销、人力资源和客户服务的15个代理工作流和15项技能，用户在执行前批准所有操作。

针对主要关注点，“Claude小企业版”优先考虑信任和数据安全。用户保持控制，启动所有任务并批准计划。系统尊重现有权限，并且在团队和企业计划中，默认情况下用户数据不会用于训练。

为了提升AI素养，Anthropic与PayPal合作，提供免费在线课程“小企业AI流畅度”。他们还将推出“Claude SMB巡演”，在各个城市提供免费的半天培训研讨会。此外，Anthropic正在投资与LISC和Workday基金会等非营利组织和社区发展金融机构（CDFIs）建立合作关系，以赋能个体创业者，并帮助CDFIs利用AI为小企业扩大融资机会。

---

## 7. 如何让你的文字看起来有未来感 (2016)

**原文标题**: How to make your text look futuristic (2016)

**原文链接**: [https://typesetinthefuture.com/2016/02/18/futuristic/](https://typesetinthefuture.com/2016/02/18/futuristic/)

Dave Addey 在他2016年的文章中，提出了六条让文字看起来具有未来感的“简易规则”，这些规则建立在 Eurostile Bold 等字体有效性的基础上。他通过逐步改造一个简单的无衬线字体单词来演示这些规则。

这些规则是：
1.  **增加斜体倾斜：** 旨在暗示向未来的运动。
2.  **融入曲线和角度：** 混合字体风格以营造现代感。
3.  **使用“完美的V形”：** 对字母进行特定的风格化添加。
4.  **组合字母（字距调整）：** 通过合并笔画来应对“字距大战”。
5.  **删除任意笔画：** 删除字母的部分，如横线。
6.  **应用纹理和效果：** 添加噪点、拉丝金属、忧郁的蓝色灯光、浮雕效果和星场。

Addey 阐释了这些规则的综合效果，最终呈现出一种引人注目的未来主义美学。他接着展示了这些原则的各种排列组合如何应用于众多电影和电视剧中，以确立未来时间背景。例子包括《银翼杀手》、《太空堡垒卡拉狄加》、《变形金刚》、《银河护卫队》、《机械战警》、《星球大战》、《回到未来》和《星际迷航：下一代》等标志性片名，凸显了这些设计元素在表示未来方面的广泛而持续的应用。

---

## 8. Twin brothers wipe 96 government databases minutes after being fired

**原文标题**: Twin brothers wipe 96 government databases minutes after being fired

**原文链接**: [https://arstechnica.com/tech-policy/2026/05/drop-database-what-not-to-do-after-losing-an-it-job/](https://arstechnica.com/tech-policy/2026/05/drop-database-what-not-to-do-after-losing-an-it-job/)

生成摘要时出错

---

## 9. Tell NYT, Atlantic, USA Today to keep Wayback Machine

**原文标题**: Tell NYT, Atlantic, USA Today to keep Wayback Machine

**原文链接**: [https://www.savethearchive.com/newsleaders/](https://www.savethearchive.com/newsleaders/)

生成摘要时出错

---

## 10. The Emacsification of Software

**原文标题**: The Emacsification of Software

**原文链接**: [https://sockpuppet.org/blog/2026/05/12/emacsification/](https://sockpuppet.org/blog/2026/05/12/emacsification/)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 2 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 3 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 4 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 5 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 6 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 7 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 8 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 9 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 10 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 11 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 12 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 13 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 14 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 15 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 16 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 17 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 18 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 19 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 20 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 21 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 22 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 23 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 24 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 25 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 26 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 27 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 28 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 29 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 30 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 31 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 32 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 33 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 34 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 35 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 36 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 37 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 38 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 39 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 40 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 41 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 42 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 43 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 44 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 45 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 46 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 47 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 48 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 49 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 50 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 51 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 52 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 53 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 54 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 55 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 56 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 57 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 58 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 59 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 60 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 61 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 62 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 63 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 64 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 65 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 66 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 67 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 68 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 69 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 70 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 71 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 72 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 73 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 74 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 75 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 76 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 77 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 78 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 79 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 80 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 81 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 82 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 83 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 84 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 85 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 86 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 87 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 88 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 89 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 90 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 91 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 92 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 93 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 94 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 95 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 96 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 97 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 98 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 99 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 100 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 101 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 102 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 103 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 104 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 105 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 106 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 107 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 108 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 109 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 110 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 111 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 112 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 113 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 114 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 115 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 116 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 117 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 118 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 119 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 120 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 121 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 122 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 123 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 124 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 125 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 126 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 127 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 128 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 129 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 130 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 131 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 132 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 133 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 134 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 135 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 136 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 137 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 138 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 139 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 140 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 141 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 142 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 143 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 144 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 145 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 146 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 147 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 148 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 149 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 150 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 151 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 152 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 153 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 154 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 155 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 156 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 157 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 158 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 159 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 160 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 161 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 162 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 163 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 164 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 165 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 166 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 167 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 168 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 169 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 170 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 171 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 172 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 173 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 174 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 175 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 176 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 177 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 178 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 179 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 180 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 181 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 182 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 183 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 184 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 185 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 186 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 187 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 188 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
