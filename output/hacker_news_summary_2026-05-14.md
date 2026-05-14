# Hacker News 热门文章摘要 (2026-05-14)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

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

## 11. Kickstarter is forced to ban adult content by payment processors

**原文标题**: Kickstarter is forced to ban adult content by payment processors

**原文链接**: [https://kotaku.com/kickstarter-is-the-latest-platform-seemingly-forced-to-ban-adult-content-by-payment-processors-2000695648](https://kotaku.com/kickstarter-is-the-latest-platform-seemingly-forced-to-ban-adult-content-by-payment-processors-2000695648)

生成摘要时出错

---

## 12. RTX 5090 and M4 MacBook Air: Can It Game?

**原文标题**: RTX 5090 and M4 MacBook Air: Can It Game?

**原文链接**: [https://scottjg.com/posts/2026-05-05-egpu-mac-gaming/](https://scottjg.com/posts/2026-05-05-egpu-mac-gaming/)

生成摘要时出错

---

## 13. Princeton mandates proctoring for in-person exams, upending 133 year precedent

**原文标题**: Princeton mandates proctoring for in-person exams, upending 133 year precedent

**原文链接**: [https://www.dailyprincetonian.com/article/2026/05/princeton-news-adpol-proctoring-in-person-examinations-passed-faculty-133-years-precedent](https://www.dailyprincetonian.com/article/2026/05/princeton-news-adpol-proctoring-in-person-examinations-passed-faculty-133-years-precedent)

生成摘要时出错

---

## 14. Scorched Earth 2000 – Web

**原文标题**: Scorched Earth 2000 – Web

**原文链接**: [http://www.scorch2000.com/web/](http://www.scorch2000.com/web/)

生成摘要时出错

---

## 15. Scrcpy v4.0

**原文标题**: Scrcpy v4.0

**原文链接**: [https://github.com/Genymobile/scrcpy/releases/tag/v4.0](https://github.com/Genymobile/scrcpy/releases/tag/v4.0)

生成摘要时出错

---

## 16. Rewrite Bun in Rust has been merged

**原文标题**: Rewrite Bun in Rust has been merged

**原文链接**: [https://github.com/oven-sh/bun/pull/30412](https://github.com/oven-sh/bun/pull/30412)

生成摘要时出错

---

## 17. Removing the modem and GPS from my 2024 RAV4 hybrid

**原文标题**: Removing the modem and GPS from my 2024 RAV4 hybrid

**原文链接**: [https://arkadiyt.com/2026/05/13/removing-the-modem-and-gps-from-my-rav4/](https://arkadiyt.com/2026/05/13/removing-the-modem-and-gps-from-my-rav4/)

生成摘要时出错

---

## 18. MacBook Neo Deep Dive: Benchmarks, Wafer Economics, and the 8GB Gamble

**原文标题**: MacBook Neo Deep Dive: Benchmarks, Wafer Economics, and the 8GB Gamble

**原文链接**: [https://www.jdhodges.com/blog/macbook-neo-benchmarks-analysis/](https://www.jdhodges.com/blog/macbook-neo-benchmarks-analysis/)

生成摘要时出错

---

## 19. Starship V3

**原文标题**: Starship V3

**原文链接**: [https://www.spacex.com/updates#starship-v3](https://www.spacex.com/updates#starship-v3)

生成摘要时出错

---

## 20. Bitcoin trader recovers wallet with help of Claude

**原文标题**: Bitcoin trader recovers wallet with help of Claude

**原文链接**: [https://www.tomshardware.com/tech-industry/cryptocurrency/bitcoin-trader-recovers-usd400-000-using-claude-ai-after-losing-wallet-password-11-years-ago-bot-tried-3-5-trillion-passwords-before-decrypting-an-old-wallet-backup](https://www.tomshardware.com/tech-industry/cryptocurrency/bitcoin-trader-recovers-usd400-000-using-claude-ai-after-losing-wallet-password-11-years-ago-bot-tried-3-5-trillion-passwords-before-decrypting-an-old-wallet-backup)

生成摘要时出错

---

## 21. Deterministic Fully-Static Whole-Binary Translation Without Heuristics

**原文标题**: Deterministic Fully-Static Whole-Binary Translation Without Heuristics

**原文链接**: [https://arxiv.org/abs/2605.08419](https://arxiv.org/abs/2605.08419)

生成摘要时出错

---

## 22. Open Source Resistance: keep OSS alive on company time

**原文标题**: Open Source Resistance: keep OSS alive on company time

**原文链接**: [https://ossresistance.com/](https://ossresistance.com/)

生成摘要时出错

---

## 23. AI is making me dumb

**原文标题**: AI is making me dumb

**原文链接**: [https://jpain.io/god-damn-ai-is-making-me-dumb/](https://jpain.io/god-damn-ai-is-making-me-dumb/)

生成摘要时出错

---

## 24. Cisco workforce reductions

**原文标题**: Cisco workforce reductions

**原文链接**: [https://blogs.cisco.com/news/our-path-forward](https://blogs.cisco.com/news/our-path-forward)

生成摘要时出错

---

## 25. Dutch suicide prevention website shares data with tech companies without consent

**原文标题**: Dutch suicide prevention website shares data with tech companies without consent

**原文链接**: [https://nltimes.nl/2026/05/13/dutch-suicide-prevention-hotline-shares-visitor-data-tech-companies](https://nltimes.nl/2026/05/13/dutch-suicide-prevention-hotline-shares-visitor-data-tech-companies)

生成摘要时出错

---

## 26. Microsoft BitLocker – YellowKey zero-day exploit

**原文标题**: Microsoft BitLocker – YellowKey zero-day exploit

**原文链接**: [https://www.tomshardware.com/tech-industry/cyber-security/microsoft-bitlocker-protected-drives-can-now-be-opened-with-just-some-files-on-a-usb-stick-yellowkey-zero-day-exploit-demonstrates-an-apparent-backdoor](https://www.tomshardware.com/tech-industry/cyber-security/microsoft-bitlocker-protected-drives-can-now-be-opened-with-just-some-files-on-a-usb-stick-yellowkey-zero-day-exploit-demonstrates-an-apparent-backdoor)

生成摘要时出错

---

## 27. Kraftwerk's radical 1976 track

**原文标题**: Kraftwerk's radical 1976 track

**原文链接**: [https://www.bbc.com/culture/article/20260511-kraftwerks-radical-1976-track-radioactivity-became-an-anti-nuclear-anthem](https://www.bbc.com/culture/article/20260511-kraftwerks-radical-1976-track-radioactivity-became-an-anti-nuclear-anthem)

生成摘要时出错

---

## 28. EFF to 4th Circuit: Electronic Device Searches at the Border Require a Warrant

**原文标题**: EFF to 4th Circuit: Electronic Device Searches at the Border Require a Warrant

**原文链接**: [https://www.eff.org/deeplinks/2026/05/eff-fourth-circuit-electronic-device-searches-border-require-warrant](https://www.eff.org/deeplinks/2026/05/eff-fourth-circuit-electronic-device-searches-border-require-warrant)

生成摘要时出错

---

## 29. The US is winning the AI race where it matters most: commercialization

**原文标题**: The US is winning the AI race where it matters most: commercialization

**原文链接**: [https://avkcode.github.io/blog/us-winning-ai-race.html](https://avkcode.github.io/blog/us-winning-ai-race.html)

生成摘要时出错

---

## 30. USDA Projects Smallest US Wheat Harvest Since 1972 Due to Plains Drought

**原文标题**: USDA Projects Smallest US Wheat Harvest Since 1972 Due to Plains Drought

**原文链接**: [https://www.agweb.com/news/usda-projects-smallest-us-wheat-harvest-1972-due-plains-drought](https://www.agweb.com/news/usda-projects-smallest-us-wheat-harvest-1972-due-plains-drought)

生成摘要时出错

---

## 31. SecurityBaseline.eu

**原文标题**: SecurityBaseline.eu

**原文链接**: [https://internetcleanup.foundation/2026/05/european-governments-3000-tracking-sites-1000-phpmyadmins-and-99pct-poorly-encrypted-email-introducing-securitybaseline-eu/](https://internetcleanup.foundation/2026/05/european-governments-3000-tracking-sites-1000-phpmyadmins-and-99pct-poorly-encrypted-email-introducing-securitybaseline-eu/)

生成摘要时出错

---

## 32. "Not Medically Necessary": Helping America's Health Insurers Deny Coverage

**原文标题**: "Not Medically Necessary": Helping America's Health Insurers Deny Coverage

**原文链接**: [https://www.propublica.org/article/evicore-health-insurance-denials-cigna-unitedhealthcare-aetna-prior-authorizations](https://www.propublica.org/article/evicore-health-insurance-denials-cigna-unitedhealthcare-aetna-prior-authorizations)

生成摘要时出错

---

## 33. My graduation cap runs Rust

**原文标题**: My graduation cap runs Rust

**原文链接**: [https://ericswpark.com/blog/2026/2026-05-12-my-graduation-cap-runs-rust/](https://ericswpark.com/blog/2026/2026-05-12-my-graduation-cap-runs-rust/)

生成摘要时出错

---

## 34. A Claude Code and Codex Skill for Deliberate Skill Development

**原文标题**: A Claude Code and Codex Skill for Deliberate Skill Development

**原文链接**: [https://github.com/DrCatHicks/learning-opportunities](https://github.com/DrCatHicks/learning-opportunities)

生成摘要时出错

---

## 35. Meta won't let you block its AI account on Threads

**原文标题**: Meta won't let you block its AI account on Threads

**原文链接**: [https://www.theverge.com/tech/929091/meta-ai-threads-account-block](https://www.theverge.com/tech/929091/meta-ai-threads-account-block)

生成摘要时出错

---

## 36. New Nginx Exploit

**原文标题**: New Nginx Exploit

**原文链接**: [https://github.com/DepthFirstDisclosures/Nginx-Rift](https://github.com/DepthFirstDisclosures/Nginx-Rift)

生成摘要时出错

---

## 37. Sam Altman's Business Dealings Under GOP Scrutiny Ahead of OpenAI's IPO

**原文标题**: Sam Altman's Business Dealings Under GOP Scrutiny Ahead of OpenAI's IPO

**原文链接**: [https://www.wsj.com/tech/ai/sam-altmans-business-dealings-under-gop-scrutiny-ahead-of-openais-ipo-52c1cc4d](https://www.wsj.com/tech/ai/sam-altmans-business-dealings-under-gop-scrutiny-ahead-of-openais-ipo-52c1cc4d)

生成摘要时出错

---

## 38. Haiku

**原文标题**: Haiku

**原文链接**: [https://www.haiku-os.org](https://www.haiku-os.org)

生成摘要时出错

---

## 39. Meta's New Reality: Record High Profits. Record Low Morale

**原文标题**: Meta's New Reality: Record High Profits. Record Low Morale

**原文链接**: [https://www.wired.com/story/meta-layoffs-bad-vibes-mark-zuckerberg-ai/](https://www.wired.com/story/meta-layoffs-bad-vibes-mark-zuckerberg-ai/)

生成摘要时出错

---

## 40. When “idle” isn't idle: how a Linux kernel optimization became a QUIC bug

**原文标题**: When “idle” isn't idle: how a Linux kernel optimization became a QUIC bug

**原文链接**: [https://blog.cloudflare.com/quic-death-spiral-fix/](https://blog.cloudflare.com/quic-death-spiral-fix/)

生成摘要时出错

---

## 41. Computer Hobby Movement in Canada

**原文标题**: Computer Hobby Movement in Canada

**原文链接**: [https://museum.eecs.yorku.ca/exhibits/show/hobby_canada/hobby_canada](https://museum.eecs.yorku.ca/exhibits/show/hobby_canada/hobby_canada)

生成摘要时出错

---

## 42. 50K Tahoe residents need power as utility eyes redirecting lines to data centers

**原文标题**: 50K Tahoe residents need power as utility eyes redirecting lines to data centers

**原文链接**: [https://fortune.com/2026/05/12/lake-tahoe-data-center-49000-residents-power-source/](https://fortune.com/2026/05/12/lake-tahoe-data-center-49000-residents-power-source/)

生成摘要时出错

---

## 43. Mystery Microsoft bug leaker keeps the zero-days coming

**原文标题**: Mystery Microsoft bug leaker keeps the zero-days coming

**原文链接**: [https://www.theregister.com/security/2026/05/13/disgruntled-researcher-releases-two-more-microsoft-zero-days/5239758](https://www.theregister.com/security/2026/05/13/disgruntled-researcher-releases-two-more-microsoft-zero-days/5239758)

生成摘要时出错

---

## 44. Classic 7 is a Windows 10 LTSC mod to look 1:1 to Windows 7

**原文标题**: Classic 7 is a Windows 10 LTSC mod to look 1:1 to Windows 7

**原文链接**: [https://classic7.lol/](https://classic7.lol/)

生成摘要时出错

---

## 45. Making the news available at no cost is a victory

**原文标题**: Making the news available at no cost is a victory

**原文链接**: [https://www.sltrib.com/opinion/commentary/2026/05/12/just-days-tribune-reporting/](https://www.sltrib.com/opinion/commentary/2026/05/12/just-days-tribune-reporting/)

生成摘要时出错

---

## 46. S-100 Virtual Workbench

**原文标题**: S-100 Virtual Workbench

**原文链接**: [https://grantmestrength.github.io/S100/](https://grantmestrength.github.io/S100/)

生成摘要时出错

---

## 47. Fuck You, Bambu Lab. Go Ahead, Sue Us

**原文标题**: Fuck You, Bambu Lab. Go Ahead, Sue Us

**原文链接**: [https://gamersnexus.net/fk-you-bambu-lab](https://gamersnexus.net/fk-you-bambu-lab)

生成摘要时出错

---

## 48. Anthropic forms $200M partnership with the Gates Foundation

**原文标题**: Anthropic forms $200M partnership with the Gates Foundation

**原文链接**: [https://www.anthropic.com/news/gates-foundation-partnership](https://www.anthropic.com/news/gates-foundation-partnership)

生成摘要时出错

---

## 49. A desire for a loud car correlates with higher scores on psychopathy and sadism

**原文标题**: A desire for a loud car correlates with higher scores on psychopathy and sadism

**原文链接**: [https://cipp.ug.edu.pl/A-desire-for-a-loud-car-with-a-modified-muffler-is-predicted-by-being-a-man-and-higher,162006,0,2.html](https://cipp.ug.edu.pl/A-desire-for-a-loud-car-with-a-modified-muffler-is-predicted-by-being-a-man-and-higher,162006,0,2.html)

生成摘要时出错

---

## 50. Show HN: Running the second public ODoH relay

**原文标题**: Show HN: Running the second public ODoH relay

**原文链接**: [https://numa.rs/blog/posts/odoh-anonymous-dns-without-an-account.html](https://numa.rs/blog/posts/odoh-anonymous-dns-without-an-account.html)

生成摘要时出错

---

## 51. The European Union backs Italy's right to make Meta pay for news

**原文标题**: The European Union backs Italy's right to make Meta pay for news

**原文链接**: [https://www.niemanlab.org/2026/05/the-eu-backs-italys-right-to-make-meta-pay-for-news/](https://www.niemanlab.org/2026/05/the-eu-backs-italys-right-to-make-meta-pay-for-news/)

生成摘要时出错

---

## 52. Cuba says it has run out of fuel, blames U.S. embargo

**原文标题**: Cuba says it has run out of fuel, blames U.S. embargo

**原文链接**: [https://www.upi.com/Top_News/World-News/2026/05/14/Cuba-says-oil-reserves-totally-drained/9311778746907/](https://www.upi.com/Top_News/World-News/2026/05/14/Cuba-says-oil-reserves-totally-drained/9311778746907/)

生成摘要时出错

---

## 53. Altman forced to confront claims at OpenAI trial that he's a prolific liar

**原文标题**: Altman forced to confront claims at OpenAI trial that he's a prolific liar

**原文链接**: [https://arstechnica.com/tech-policy/2026/05/altman-forced-to-confront-claims-at-openai-trial-that-hes-a-prolific-liar/](https://arstechnica.com/tech-policy/2026/05/altman-forced-to-confront-claims-at-openai-trial-that-hes-a-prolific-liar/)

生成摘要时出错

---

## 54. The other half of AI safety

**原文标题**: The other half of AI safety

**原文链接**: [https://personalaisafety.com/p/the-other-half-of-ai-safety](https://personalaisafety.com/p/the-other-half-of-ai-safety)

生成摘要时出错

---

## 55. Launch HN: Ardent (YC P26) – Postgres sandboxes in seconds with zero migration

**原文标题**: Launch HN: Ardent (YC P26) – Postgres sandboxes in seconds with zero migration

**原文链接**: [https://www.tryardent.com/](https://www.tryardent.com/)

生成摘要时出错

---

## 56. Software Developers Say AI Is Rotting Their Brains

**原文标题**: Software Developers Say AI Is Rotting Their Brains

**原文链接**: [https://www.404media.co/software-developers-say-ai-is-rotting-their-brains/](https://www.404media.co/software-developers-say-ai-is-rotting-their-brains/)

生成摘要时出错

---

## 57. Avoiding and reducing microplastic false positives from dry glove contact

**原文标题**: Avoiding and reducing microplastic false positives from dry glove contact

**原文链接**: [https://pubs.rsc.org/en/content/articlelanding/2026/ay/d5ay01801c](https://pubs.rsc.org/en/content/articlelanding/2026/ay/d5ay01801c)

生成摘要时出错

---

## 58. Rars: a Rust RAR implementation, mostly written by LLMs

**原文标题**: Rars: a Rust RAR implementation, mostly written by LLMs

**原文链接**: [https://bitplane.net/log/2026/05/rars/](https://bitplane.net/log/2026/05/rars/)

生成摘要时出错

---

## 59. The AI Zombification of Universities

**原文标题**: The AI Zombification of Universities

**原文链接**: [https://www.thenewcritic.com/p/the-great-zombification](https://www.thenewcritic.com/p/the-great-zombification)

生成摘要时出错

---

## 60. Cost of enum-to-string: C++26 reflection vs. the old ways

**原文标题**: Cost of enum-to-string: C++26 reflection vs. the old ways

**原文链接**: [https://vittorioromeo.com/index/blog/refl_enum_to_string.html](https://vittorioromeo.com/index/blog/refl_enum_to_string.html)

生成摘要时出错

---

## 61. Show HN: Nibble

**原文标题**: Show HN: Nibble

**原文链接**: [https://github.com/glouw/nibble](https://github.com/glouw/nibble)

生成摘要时出错

---

## 62. Bun's Rust rewrite has been merged

**原文标题**: Bun's Rust rewrite has been merged

**原文链接**: [https://old.reddit.com/r/rust/comments/1tcrmjs/rewrite_bun_in_rust_has_been_merged/](https://old.reddit.com/r/rust/comments/1tcrmjs/rewrite_bun_in_rust_has_been_merged/)

生成摘要时出错

---

## 63. Germany's Sovereign Tech Fund Backs KDE with €1.3M

**原文标题**: Germany's Sovereign Tech Fund Backs KDE with €1.3M

**原文链接**: [https://www.theregister.com/oses/2026/05/14/kde-bags-13m-as-europe-realizes-it-might-need-an-os-of-its-own/5240562](https://www.theregister.com/oses/2026/05/14/kde-bags-13m-as-europe-realizes-it-might-need-an-os-of-its-own/5240562)

生成摘要时出错

---

## 64. The Siri for Families Apple Will Never Build

**原文标题**: The Siri for Families Apple Will Never Build

**原文链接**: [https://taoofmac.com/space/blog/2026/05/14/1220](https://taoofmac.com/space/blog/2026/05/14/1220)

生成摘要时出错

---

## 65. delta time

**原文标题**: delta time

**原文链接**: [https://www.deltatime.life/](https://www.deltatime.life/)

生成摘要时出错

---

## 66. Using OR-Tools CP-SAT for Scheduling Problems

**原文标题**: Using OR-Tools CP-SAT for Scheduling Problems

**原文链接**: [https://atalaykutlay.com/or-tools-cp-sat-for-scheduling-problems.html](https://atalaykutlay.com/or-tools-cp-sat-for-scheduling-problems.html)

生成摘要时出错

---

## 67. Medicare's new payment model is built for AI. Most of the tech world has no idea

**原文标题**: Medicare's new payment model is built for AI. Most of the tech world has no idea

**原文链接**: [https://techcrunch.com/2026/05/12/medicares-new-payment-model-is-built-for-ai-and-most-of-the-tech-world-has-no-idea/](https://techcrunch.com/2026/05/12/medicares-new-payment-model-is-built-for-ai-and-most-of-the-tech-world-has-no-idea/)

生成摘要时出错

---

## 68. The limits of Rust, or why you should probably not follow Amazon and Cloudflare

**原文标题**: The limits of Rust, or why you should probably not follow Amazon and Cloudflare

**原文链接**: [https://kerkour.com/the-limits-of-rust](https://kerkour.com/the-limits-of-rust)

生成摘要时出错

---

## 69. Myths about /dev/urandom (2014)

**原文标题**: Myths about /dev/urandom (2014)

**原文链接**: [https://www.2uo.de/myths-about-urandom/](https://www.2uo.de/myths-about-urandom/)

生成摘要时出错

---

## 70. ReactOS

**原文标题**: ReactOS

**原文链接**: [https://reactos.org/](https://reactos.org/)

生成摘要时出错

---

## 71. The AI Backlash Could Get Ugly

**原文标题**: The AI Backlash Could Get Ugly

**原文链接**: [https://www.theatlantic.com/technology/2026/05/ai-backlash-data-centers-political-violence/687151/](https://www.theatlantic.com/technology/2026/05/ai-backlash-data-centers-political-violence/687151/)

生成摘要时出错

---

## 72. What happens when you post a real Monet and say it's AI?

**原文标题**: What happens when you post a real Monet and say it's AI?

**原文链接**: [https://twitter.com/jediwolf/status/2054776716770320631](https://twitter.com/jediwolf/status/2054776716770320631)

生成摘要时出错

---

## 73. SQLite Code of Ethics

**原文标题**: SQLite Code of Ethics

**原文链接**: [https://sqlite.org/codeofethics.html](https://sqlite.org/codeofethics.html)

生成摘要时出错

---

## 74. YellowKey Bitlocker Bypass Vulnerability

**原文标题**: YellowKey Bitlocker Bypass Vulnerability

**原文链接**: [https://github.com/Nightmare-Eclipse/YellowKey](https://github.com/Nightmare-Eclipse/YellowKey)

生成摘要时出错

---

## 75. First public macOS kernel memory corruption exploit on Apple M5

**原文标题**: First public macOS kernel memory corruption exploit on Apple M5

**原文链接**: [https://blog.calif.io/p/first-public-kernel-memory-corruption](https://blog.calif.io/p/first-public-kernel-memory-corruption)

生成摘要时出错

---

## 76. A sentimental tour of late 1990s and early 2000s hacking tools

**原文标题**: A sentimental tour of late 1990s and early 2000s hacking tools

**原文链接**: [https://andreafortuna.org/2026/05/13/amarcord/](https://andreafortuna.org/2026/05/13/amarcord/)

生成摘要时出错

---

## 77. Meta employees protest against mouse tracking tech at US offices

**原文标题**: Meta employees protest against mouse tracking tech at US offices

**原文链接**: [https://www.reuters.com/sustainability/society-equity/meta-us-employees-organize-protest-against-mouse-tracking-tech-2026-05-12/](https://www.reuters.com/sustainability/society-equity/meta-us-employees-organize-protest-against-mouse-tracking-tech-2026-05-12/)

生成摘要时出错

---

## 78. Composer leaks contents of tokens configured as GitHub OAuth tokens

**原文标题**: Composer leaks contents of tokens configured as GitHub OAuth tokens

**原文链接**: [https://github.com/composer/composer/security/advisories/GHSA-f9f8-rm49-7jv2](https://github.com/composer/composer/security/advisories/GHSA-f9f8-rm49-7jv2)

生成摘要时出错

---

## 79. HDD Firmware Hacking

**原文标题**: HDD Firmware Hacking

**原文链接**: [https://icode4.coffee/?p=1465](https://icode4.coffee/?p=1465)

生成摘要时出错

---

## 80. LinkedIn Fanfiction

**原文标题**: LinkedIn Fanfiction

**原文链接**: [https://www.marginalia.nu/log/a_137_linkedin_fanfiction/](https://www.marginalia.nu/log/a_137_linkedin_fanfiction/)

生成摘要时出错

---

## 81. Arena AI Model ELO History

**原文标题**: Arena AI Model ELO History

**原文链接**: [https://mayerwin.github.io/AI-Arena-History/](https://mayerwin.github.io/AI-Arena-History/)

生成摘要时出错

---

## 82. Grok Build

**原文标题**: Grok Build

**原文链接**: [https://x.ai/news/grok-build-cli](https://x.ai/news/grok-build-cli)

生成摘要时出错

---

## 83. Residents furious as Utah approves datacenter twice the size of Manhattan

**原文标题**: Residents furious as Utah approves datacenter twice the size of Manhattan

**原文链接**: [https://www.theguardian.com/us-news/2026/may/13/utah-approves-datacenter-backlash](https://www.theguardian.com/us-news/2026/may/13/utah-approves-datacenter-backlash)

生成摘要时出错

---

## 84. Beyond Semantic Similarity

**原文标题**: Beyond Semantic Similarity

**原文链接**: [https://arxiv.org/abs/2605.05242](https://arxiv.org/abs/2605.05242)

生成摘要时出错

---

## 85. New York, California pension leaders oppose 'extreme' SpaceX control structure

**原文标题**: New York, California pension leaders oppose 'extreme' SpaceX control structure

**原文链接**: [https://www.reuters.com/legal/government/new-york-california-pension-leaders-oppose-extreme-spacex-control-structure-2026-05-14/](https://www.reuters.com/legal/government/new-york-california-pension-leaders-oppose-extreme-spacex-control-structure-2026-05-14/)

生成摘要时出错

---

## 86. German intelligence offices snub Palantir software

**原文标题**: German intelligence offices snub Palantir software

**原文链接**: [https://www.dw.com/en/german-intelligence-offices-snub-us-based-palantir-software/a-77160897](https://www.dw.com/en/german-intelligence-offices-snub-us-based-palantir-software/a-77160897)

生成摘要时出错

---

## 87. They Said It Would Cost $54M. We Said "No Thanks."

**原文标题**: They Said It Would Cost $54M. We Said "No Thanks."

**原文链接**: [https://nateglubish.substack.com/p/they-said-it-would-cost-54-million](https://nateglubish.substack.com/p/they-said-it-would-cost-54-million)

生成摘要时出错

---

## 88. “I applied to be pope”: Losing grip on reality while using ChatGPT

**原文标题**: “I applied to be pope”: Losing grip on reality while using ChatGPT

**原文链接**: [https://www.thestandard.com.hk/world/article/331886/I-applied-to-be-pope-Losing-grip-on-reality-while-using-ChatGPT](https://www.thestandard.com.hk/world/article/331886/I-applied-to-be-pope-Losing-grip-on-reality-while-using-ChatGPT)

生成摘要时出错

---

## 89. The Whole Anthropic Kerfuffle

**原文标题**: The Whole Anthropic Kerfuffle

**原文链接**: [https://twitter.com/josevalim/status/2054887621336174799](https://twitter.com/josevalim/status/2054887621336174799)

生成摘要时出错

---

## 90. Claude subscription changes coverage of `claude -p`

**原文标题**: Claude subscription changes coverage of `claude -p`

**原文链接**: [https://x.com/i/trending/2054617957440143639](https://x.com/i/trending/2054617957440143639)

生成摘要时出错

---

## 91. Temu is advertising filet mignon on X

**原文标题**: Temu is advertising filet mignon on X

**原文链接**: [https://twitter.com/shoptemu/status/2053092200632685016](https://twitter.com/shoptemu/status/2053092200632685016)

生成摘要时出错

---

## 92. EU browser choice rules send millions more users Firefox's way

**原文标题**: EU browser choice rules send millions more users Firefox's way

**原文链接**: [https://www.theregister.com/software/2026/05/12/eu-law-bestows-6m-more-firefox-users-upon-us-moz-says/5238623](https://www.theregister.com/software/2026/05/12/eu-law-bestows-6m-more-firefox-users-upon-us-moz-says/5238623)

生成摘要时出错

---

## 93. Neanderthals drilled cavities to treat a toothache 59,000 years ago

**原文标题**: Neanderthals drilled cavities to treat a toothache 59,000 years ago

**原文链接**: [https://arstechnica.com/science/2026/05/neanderthals-drilled-cavities-to-treat-a-toothache-59000-years-ago/](https://arstechnica.com/science/2026/05/neanderthals-drilled-cavities-to-treat-a-toothache-59000-years-ago/)

生成摘要时出错

---

## 94. Zero-native – Build native desktop apps with web UI

**原文标题**: Zero-native – Build native desktop apps with web UI

**原文链接**: [https://zero-native.dev](https://zero-native.dev)

生成摘要时出错

---

## 95. The conflation of money and things

**原文标题**: The conflation of money and things

**原文链接**: [https://lithub.com/is-it-even-real-on-the-conflation-of-money-and-things/](https://lithub.com/is-it-even-real-on-the-conflation-of-money-and-things/)

生成摘要时出错

---

## 96. I was asked to install malware during a fake interview

**原文标题**: I was asked to install malware during a fake interview

**原文链接**: [https://ashishb.net/security/contagious-interview/](https://ashishb.net/security/contagious-interview/)

生成摘要时出错

---

## 97. Apple-OpenAI Relationship Frays, Setting Up Possible Legal Fight

**原文标题**: Apple-OpenAI Relationship Frays, Setting Up Possible Legal Fight

**原文链接**: [https://www.bloomberg.com/news/articles/2026-05-14/openai-apple-partnership-frays-setting-up-possible-legal-fight](https://www.bloomberg.com/news/articles/2026-05-14/openai-apple-partnership-frays-setting-up-possible-legal-fight)

生成摘要时出错

---

## 98. U.S. intelligence shows Iran retains substantial missile capabilities

**原文标题**: U.S. intelligence shows Iran retains substantial missile capabilities

**原文链接**: [https://www.nytimes.com/2026/05/12/us/politics/iran-missiles-us-intelligence.html](https://www.nytimes.com/2026/05/12/us/politics/iran-missiles-us-intelligence.html)

生成摘要时出错

---

## 99. Who Trusts Sam Altman?

**原文标题**: Who Trusts Sam Altman?

**原文链接**: [https://techcrunch.com/2026/05/13/who-trusts-sam-altman/](https://techcrunch.com/2026/05/13/who-trusts-sam-altman/)

生成摘要时出错

---

## 100. New Claude Code programmatic usage restrictions

**原文标题**: New Claude Code programmatic usage restrictions

**原文链接**: [https://twitter.com/i/status/2054610152817619388](https://twitter.com/i/status/2054610152817619388)

生成摘要时出错

---

