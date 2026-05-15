# Hacker News 热门文章摘要 (2026-05-15)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 2024款RAV4混动版移除调制解调器和GPS

**原文标题**: Removing the modem and GPS from my 2024 RAV4 hybrid

**原文链接**: [https://arkadiyt.com/2026/05/13/removing-the-modem-and-gps-from-my-rav4/](https://arkadiyt.com/2026/05/13/removing-the-modem-and-gps-from-my-rav4/)

本文详细介绍了一个DIY项目，旨在通过物理移除2024款RAV4混动车型的调制解调器（数据通信模块，简称DCM）和内置GPS来增强隐私。作者强调，现代汽车大量收集并向制造商和第三方数据经纪人传输敏感的遥测数据——包括位置、速度、燃油水平、驾驶行为，甚至摄像头录像——这构成了重大的隐私和安全风险。

该项目旨在从源头阻止这种数据传输。移除DCM会禁用云服务、OTA更新、SOS功能和自动碰撞通知。通过DCM路由的车载麦克风则使用特定的DCM旁路套件进行恢复。此外，还断开了汽车内置的GPS，以防止一个已知的CarPlay错误，即汽车中错误的定位数据可能会干扰手机导航。作者指出，虽然这可能会使部分与远程信息处理相关的保修失效，但根据《马格努森-莫斯保修法案》，它不会使整个汽车保修失效。

一个关键点是，通过蓝牙连接手机会允许汽车利用手机的互联网传输数据，因此作者建议使用有线USB连接CarPlay或蓝牙转USB适配器。

这个被认为是中等难度且需要几个小时的过程，涉及拆卸中控台和信息娱乐区域，以接触并拆下DCM，安装旁路套件，然后从主机断开GPS天线。成功确认的标志包括信息娱乐屏幕上出现“无连接”图标、SOS指示灯不亮以及麦克风功能正常。作者对此表示满意，但承认由于汽车集成度日益提高和反“维修权”的努力，未来可能面临挑战，并倡导制定更强的联邦隐私法。

---

## 2. Bun 的 Rust 重写已合并

**原文标题**: Rewrite Bun in Rust has been merged

**原文链接**: [https://github.com/oven-sh/bun/pull/30412](https://github.com/oven-sh/bun/pull/30412)

Jarred-Sumner 于 2026 年 5 月 8 日宣布，使用 Rust 重写的 Bun 已成功合并。这次重大更新将 Bun 的核心逻辑用 Rust 重新实现，同时基本保留了其现有架构和数据结构，并且没有引入异步 Rust 或许多新的第三方库。

这次合并带来了几项关键改进：
*   **稳定性：** 它通过了 Bun 在所有平台上现有的测试套件，解决了多项内存泄漏和不稳定的测试。
*   **性能：** 基准测试显示结果从持平到更快不等。
*   **效率：** 二进制文件大小缩减了 3 MB 到 8 MB。
*   **开发者体验：** 至关重要的是，转向 Rust 提供了编译器辅助工具来捕获和防止内存错误，这些错误在过去耗费了大量的开发和调试时间。

用户可以通过运行 `bun upgrade --canary` 来试用新的 Rust 驱动的 Bun，并鼓励他们提交遇到的任何问题。在更新发布到非 Canary 版本之前，还计划进行进一步的优化工作和代码清理。

---

## 3. RTX 5090 和 M4 MacBook Air：能玩游戏吗？

**原文标题**: RTX 5090 and M4 MacBook Air: Can It Game?

**原文链接**: [https://scottjg.com/posts/2026-05-05-egpu-mac-gaming/](https://scottjg.com/posts/2026-05-05-egpu-mac-gaming/)

本文详细介绍了一个雄心勃勃的项目，旨在让 NVIDIA RTX 5090 eGPU 在 M4 MacBook Air 上用于游戏和AI推理。鉴于 macOS 缺少适用于 Apple Silicon 的原生 NVIDIA 驱动程序，该方法涉及在 MacBook Air 上运行一个 Linux ARM64 虚拟机，并利用 PCI 直通技术赋予虚拟机直接访问通过 Thunderbolt 连接的 GPU 的权限。

这需要在 macOS 上实现 PCI 直通技术时克服重大的技术挑战。第一个障碍是映射 PCI 基地址寄存器 (BAR)，这最初导致了宿主内核崩溃。解决方法是发现 Apple 的 Hypervisor.framework 中用于设备内存映射的 `HV_MEMORY_EXEC` 标志存在问题；改用只读写标志则避免了崩溃。然而，这会带来性能损失，由于更严格的内存类型处理，BAR 写入速度比最佳状态慢约 10 倍。

第二个主要挑战是直接内存访问 (DMA)。Apple Silicon 的 DART 单元（一个 IOMMU 等效组件）负责处理设备的内存转换。然而，DART 在虚拟机直通方面存在关键限制：总映射限制约为 1.5GB（不足以满足现代 GPU 的需求），单个缓冲区映射上限约为 64KB，并且无法控制分配的地址或对齐方式。这些限制严重复杂化了在 Linux 虚拟机中可靠启用 GPU DMA 的过程。

---

## 4. 科恩布鲁斯校长关于资金与人才输送管道的致辞

**原文标题**: A message from President Kornbluth about funding and the talent pipeline

**原文链接**: [https://president.mit.edu/writing-speeches/video-transcript-message-president-kornbluth-about-funding-and-talent-pipeline](https://president.mit.edu/writing-speeches/video-transcript-message-president-kornbluth-about-funding-and-talent-pipeline)

2026年5月14日，麻省理工学院校长萨莉·科恩布鲁斯向全体教职员工和学生通报了学院在资金和人才储备方面面临的严峻挑战。学院一年多来一直面临预算压力，其捐赠基金被征收8%的税收使其雪上加霜，导致不得不进行艰难的削减。

尽管联邦拨款得到部分恢复，但资金流向麻省理工学院的情况不如从前，一些机构在考量时将地域因素置于科学价值之上。这导致校园研究活动和新获得的联邦研究资助与去年相比均下降了20%以上。虽然非联邦资金有所增长，但不足以弥补缺口，导致赞助研究活动总体减少了10%。

人才储备也受到了影响。政策变化阻碍了国际学生的入学，而联邦资金的不确定性使得首席研究员（PIs）在招收新研究生时变得谨慎。这导致今年的研究生入学人数下降，预计将持续下去，可能导致研究生人数（斯隆管理学院除外）减少500名。这种损失威胁到麻省理工学院的研究使命，削弱了对本科生的指导，并剥夺了有才华的个人接受麻省理工学院教育的机会。

科恩布鲁斯强调，这不仅仅是“勒紧裤腰带”，而是研究活动的实际下降，可能损害国家创新能力。尽管前景“严峻”，麻省理工学院仍在积极应对：教职员工正在寻求新的联邦机会（例如，为美国能源部“创世纪任务”提交了176份提案），积极争取产业资金，探索新的教育收入来源，加强慈善募捐工作，并在华盛顿游说，反对征收捐赠基金税，并倡导好奇心驱动的科学研究的价值。麻省理工学院正在利用其社区的活力来应对这些挑战。

---

## 5. arXiv 新政策：虚构参考文献，禁投一年

**原文标题**: New arXiv policy: 1-year ban for hallucinated references

**原文链接**: [https://twitter.com/tdietterich/status/2055000956144935055](https://twitter.com/tdietterich/status/2055000956144935055)

所提供的内容是一条错误消息，提示“JavaScript 已禁用”并附带了启用它或切换浏览器的说明，而非文章本身。

因此，我无法总结标题为“arXiv新政策：因虚构参考文献而禁言一年”的文章，因为其文本不可用。请提供文章的实际内容，以便我进行总结。

---

## 6. 穆瓦瓦德出口IP的识别性令人惊讶。

**原文标题**: Mullvad exit IPs are surprisingly identifying

**原文链接**: [https://tmctmt.com/posts/mullvad-exit-ips-as-a-fingerprinting-vector/](https://tmctmt.com/posts/mullvad-exit-ips-as-a-fingerprinting-vector/)

最新分析显示，Mullvad VPN 的出口 IP 分配尽管表面上多样，却因其确定性而具有惊人的识别性。Mullvad 根据用户的 WireGuard 密钥分配出口 IP，而该密钥每 1-30 天才轮换一次，对于第三方客户端则永不轮换。

一个针对 9 台服务器测试了 3650 个公钥的脚本发现，尽管理论上存在数万亿个 IP 组合，实际却只分配了 284 个独特的组合。发生这种情况是因为 IP 选择算法对于给定的公钥，始终选择一个落在每个服务器总 IP 池中“相同百分位”的出口 IP。

这种行为归因于一个常见的编程误解：Mullvad 可能使用一个以公钥作为种子的随机数生成器来选择一个 IP“索引”。在 Rust 等语言中，这种随机数生成器产生的内部浮点数值无论提供的“边界”（池大小）如何都保持一致，导致从不同的服务器 IP 范围中选择了相同的相对位置。

这极大地损害了用户的匿名性。特定 IP 组合可以将用户范围缩小到几百人（例如，占 Mullvad 用户群的 0.34%，或约 340 名用户）。这使得高度准确的关联攻击成为可能：如果来自两个不同连接（即使连接到不同的 Mullvad 服务器）的 IP 日志显示出重叠的“浮点范围”，那么他们属于同一人的可能性超过 99%。这种去匿名化风险适用于数据泄露或合法获取的 IP 日志。

为保护自身安全，用户应避免在不轮换公钥的情况下切换服务器，并且可以通过退出 Mullvad 应用程序来强制进行公钥轮换。

---

## 7. 克劳德小型企业版

**原文标题**: Claude for Small Business

**原文链接**: [https://www.anthropic.com/news/claude-for-small-business](https://www.anthropic.com/news/claude-for-small-business)

2026年5月13日，Anthropic推出了“Claude中小企业版”，旨在帮助小型企业主在其现有工具中利用人工智能并实现任务自动化。鉴于小型企业因缺乏量身定制的解决方案而在人工智能采纳方面常落后于大型企业，该产品旨在弥合这一差距。

Claude中小企业版直接集成到Intuit QuickBooks、PayPal、HubSpot、Canva、Docusign、Google Workspace和Microsoft 365等流行平台中。它以“一键安装”的形式运行，提供15个即用型工作流程和15项技能，涵盖财务、运营、销售和营销等各种业务职能。功能包括规划薪资、月度结账、开展销售活动、催收发票、生成营销素材和提供业务洞察。

该系统允许用户在Claude Cowork中选择一项工作；Claude随后执行该工作，所有操作在最终确定前均需用户批准。信任和安全是首要考量，确保任务由用户发起、维护现有工具权限，并且在团队版和企业版计划中，用户数据默认不用于模型训练。

为支持有效采纳，Anthropic与PayPal合作，提供名为“小型企业AI流畅度”的免费在线课程。此外，“Claude中小企业巡展”在多个城市提供免费的实践培训研讨会。作为其公共利益使命的一部分，Anthropic还与Workday基金会/LISC等组织合作，支持个体创业者和社区发展金融机构（CDFIs），以帮助小型企业通过人工智能工具获取资金。

---

## 8. AI is making me dumb

**原文标题**: AI is making me dumb

**原文链接**: [https://jpain.io/god-damn-ai-is-making-me-dumb/](https://jpain.io/god-damn-ai-is-making-me-dumb/)

生成摘要时出错

---

## 9. UK government replaces Palantir software with internally-built refugee system

**原文标题**: UK government replaces Palantir software with internally-built refugee system

**原文链接**: [https://www.bbc.com/news/articles/c2l2j1lxdk5o](https://www.bbc.com/news/articles/c2l2j1lxdk5o)

生成摘要时出错

---

## 10. Project Gutenberg – keeps getting better

**原文标题**: Project Gutenberg – keeps getting better

**原文链接**: [https://www.gutenberg.org/](https://www.gutenberg.org/)

生成摘要时出错

---

## 11. Codex is now in the ChatGPT mobile app

**原文标题**: Codex is now in the ChatGPT mobile app

**原文链接**: [https://openai.com/index/work-with-codex-from-anywhere/](https://openai.com/index/work-with-codex-from-anywhere/)

生成摘要时出错

---

## 12. First public macOS kernel memory corruption exploit on Apple M5

**原文标题**: First public macOS kernel memory corruption exploit on Apple M5

**原文链接**: [https://blog.calif.io/p/first-public-kernel-memory-corruption](https://blog.calif.io/p/first-public-kernel-memory-corruption)

生成摘要时出错

---

## 13. Explore Wikipedia Like a Windows XP Desktop

**原文标题**: Explore Wikipedia Like a Windows XP Desktop

**原文链接**: [https://explorer.samismith.com/](https://explorer.samismith.com/)

生成摘要时出错

---

## 14. New Nginx Exploit

**原文标题**: New Nginx Exploit

**原文链接**: [https://github.com/DepthFirstDisclosures/Nginx-Rift](https://github.com/DepthFirstDisclosures/Nginx-Rift)

生成摘要时出错

---

## 15. A few words on DS4

**原文标题**: A few words on DS4

**原文链接**: [https://antirez.com/news/165](https://antirez.com/news/165)

生成摘要时出错

---

## 16. Princeton mandates proctoring for in-person exams, upending 133 year precedent

**原文标题**: Princeton mandates proctoring for in-person exams, upending 133 year precedent

**原文链接**: [https://www.dailyprincetonian.com/article/2026/05/princeton-news-adpol-proctoring-in-person-examinations-passed-faculty-133-years-precedent](https://www.dailyprincetonian.com/article/2026/05/princeton-news-adpol-proctoring-in-person-examinations-passed-faculty-133-years-precedent)

生成摘要时出错

---

## 17. Scorched Earth 2000 – Web

**原文标题**: Scorched Earth 2000 – Web

**原文链接**: [http://www.scorch2000.com/web/](http://www.scorch2000.com/web/)

生成摘要时出错

---

## 18. We are retiring our bug bounty program

**原文标题**: We are retiring our bug bounty program

**原文链接**: [https://turso.tech/blog/the-wonders-of-ai](https://turso.tech/blog/the-wonders-of-ai)

生成摘要时出错

---

## 19. Bitcoin trader recovers wallet with help of Claude

**原文标题**: Bitcoin trader recovers wallet with help of Claude

**原文链接**: [https://www.tomshardware.com/tech-industry/cryptocurrency/bitcoin-trader-recovers-usd400-000-using-claude-ai-after-losing-wallet-password-11-years-ago-bot-tried-3-5-trillion-passwords-before-decrypting-an-old-wallet-backup](https://www.tomshardware.com/tech-industry/cryptocurrency/bitcoin-trader-recovers-usd400-000-using-claude-ai-after-losing-wallet-password-11-years-ago-bot-tried-3-5-trillion-passwords-before-decrypting-an-old-wallet-backup)

生成摘要时出错

---

## 20. Ontario auditors find doctors' AI note takers routinely blow basic facts

**原文标题**: Ontario auditors find doctors' AI note takers routinely blow basic facts

**原文链接**: [https://www.theregister.com/ai-ml/2026/05/14/ontario-auditors-find-doctors-ai-note-takers-routinely-blow-basic-facts/5240771](https://www.theregister.com/ai-ml/2026/05/14/ontario-auditors-find-doctors-ai-note-takers-routinely-blow-basic-facts/5240771)

生成摘要时出错

---

## 21. Bun Rust rewrite: "codebase fails basic miri checks, allows for UB in safe rust"

**原文标题**: Bun Rust rewrite: "codebase fails basic miri checks, allows for UB in safe rust"

**原文链接**: [https://github.com/oven-sh/bun/issues/30719](https://github.com/oven-sh/bun/issues/30719)

生成摘要时出错

---

## 22. Show HN: Find the best local LLM for your hardware, ranked by benchmarks

**原文标题**: Show HN: Find the best local LLM for your hardware, ranked by benchmarks

**原文链接**: [https://github.com/Andyyyy64/whichllm](https://github.com/Andyyyy64/whichllm)

生成摘要时出错

---

## 23. Cisco workforce reductions

**原文标题**: Cisco workforce reductions

**原文链接**: [https://blogs.cisco.com/news/our-path-forward](https://blogs.cisco.com/news/our-path-forward)

生成摘要时出错

---

## 24. Amazon workers under pressure to up their AI usage are making up tasks

**原文标题**: Amazon workers under pressure to up their AI usage are making up tasks

**原文链接**: [https://www.fastcompany.com/91541586/amazon-workers-pressured-to-up-ai-use-extraneous-tasks](https://www.fastcompany.com/91541586/amazon-workers-pressured-to-up-ai-use-extraneous-tasks)

生成摘要时出错

---

## 25. A 0-click exploit chain for the Pixel 10

**原文标题**: A 0-click exploit chain for the Pixel 10

**原文链接**: [https://projectzero.google/2026/05/pixel-10-exploit.html](https://projectzero.google/2026/05/pixel-10-exploit.html)

生成摘要时出错

---

## 26. Microsoft BitLocker – YellowKey zero-day exploit

**原文标题**: Microsoft BitLocker – YellowKey zero-day exploit

**原文链接**: [https://www.tomshardware.com/tech-industry/cyber-security/microsoft-bitlocker-protected-drives-can-now-be-opened-with-just-some-files-on-a-usb-stick-yellowkey-zero-day-exploit-demonstrates-an-apparent-backdoor](https://www.tomshardware.com/tech-industry/cyber-security/microsoft-bitlocker-protected-drives-can-now-be-opened-with-just-some-files-on-a-usb-stick-yellowkey-zero-day-exploit-demonstrates-an-apparent-backdoor)

生成摘要时出错

---

## 27. USDA Projects Smallest US Wheat Harvest Since 1972 Due to Plains Drought

**原文标题**: USDA Projects Smallest US Wheat Harvest Since 1972 Due to Plains Drought

**原文链接**: [https://www.agweb.com/news/usda-projects-smallest-us-wheat-harvest-1972-due-plains-drought](https://www.agweb.com/news/usda-projects-smallest-us-wheat-harvest-1972-due-plains-drought)

生成摘要时出错

---

## 28. Details of the Daring Airdrop at Tristan Da Cunha

**原文标题**: Details of the Daring Airdrop at Tristan Da Cunha

**原文链接**: [https://www.tristandc.com/government/news-2026-05-11-airdrop.php](https://www.tristandc.com/government/news-2026-05-11-airdrop.php)

生成摘要时出错

---

## 29. A Claude Code and Codex Skill for Deliberate Skill Development

**原文标题**: A Claude Code and Codex Skill for Deliberate Skill Development

**原文链接**: [https://github.com/DrCatHicks/learning-opportunities](https://github.com/DrCatHicks/learning-opportunities)

生成摘要时出错

---

## 30. We don't know why Malawi is poor

**原文标题**: We don't know why Malawi is poor

**原文链接**: [https://newsletter.deenamousa.com/p/we-dont-know-why-malawi-is-poor](https://newsletter.deenamousa.com/p/we-dont-know-why-malawi-is-poor)

生成摘要时出错

---

## 31. German intelligence offices snub Palantir software

**原文标题**: German intelligence offices snub Palantir software

**原文链接**: [https://www.dw.com/en/german-intelligence-offices-snub-us-based-palantir-software/a-77160897](https://www.dw.com/en/german-intelligence-offices-snub-us-based-palantir-software/a-77160897)

生成摘要时出错

---

## 32. Image-blaster: Creates 3D environments, SFX, and meshes from a single image

**原文标题**: Image-blaster: Creates 3D environments, SFX, and meshes from a single image

**原文链接**: [https://github.com/neilsonnn/image-blaster](https://github.com/neilsonnn/image-blaster)

生成摘要时出错

---

## 33. The conflation of money and things

**原文标题**: The conflation of money and things

**原文链接**: [https://lithub.com/is-it-even-real-on-the-conflation-of-money-and-things/](https://lithub.com/is-it-even-real-on-the-conflation-of-money-and-things/)

生成摘要时出错

---

## 34. LinkedIn Fanfiction

**原文标题**: LinkedIn Fanfiction

**原文链接**: [https://www.marginalia.nu/log/a_137_linkedin_fanfiction/](https://www.marginalia.nu/log/a_137_linkedin_fanfiction/)

生成摘要时出错

---

## 35. New York, California pension leaders oppose 'extreme' SpaceX control structure

**原文标题**: New York, California pension leaders oppose 'extreme' SpaceX control structure

**原文链接**: [https://www.reuters.com/legal/government/new-york-california-pension-leaders-oppose-extreme-spacex-control-structure-2026-05-14/](https://www.reuters.com/legal/government/new-york-california-pension-leaders-oppose-extreme-spacex-control-structure-2026-05-14/)

生成摘要时出错

---

## 36. High dimensional geometry is transforming the MRI industry (2017) [pdf]

**原文标题**: High dimensional geometry is transforming the MRI industry (2017) [pdf]

**原文链接**: [https://www.ams.org/government/DonohoPresentation06-28-17Final.pdf](https://www.ams.org/government/DonohoPresentation06-28-17Final.pdf)

生成摘要时出错

---

## 37. 7 in 10 Americans oppose data centers being built in their communities

**原文标题**: 7 in 10 Americans oppose data centers being built in their communities

**原文链接**: [https://www.washingtonpost.com/nation/2026/05/13/7-10-americans-oppose-data-centers-being-built-their-communities/](https://www.washingtonpost.com/nation/2026/05/13/7-10-americans-oppose-data-centers-being-built-their-communities/)

生成摘要时出错

---

## 38. Arena AI Model ELO History

**原文标题**: Arena AI Model ELO History

**原文链接**: [https://mayerwin.github.io/AI-Arena-History/](https://mayerwin.github.io/AI-Arena-History/)

生成摘要时出错

---

## 39. Have a Coherent AI Policy

**原文标题**: Have a Coherent AI Policy

**原文链接**: [https://brianmeeker.me/2026/05/14/have-a-coherent-ai-policy/](https://brianmeeker.me/2026/05/14/have-a-coherent-ai-policy/)

生成摘要时出错

---

## 40. ABC News has taken all FiveThirtyEight articles offline

**原文标题**: ABC News has taken all FiveThirtyEight articles offline

**原文链接**: [https://twitter.com/baseballot/status/2055309076209492208](https://twitter.com/baseballot/status/2055309076209492208)

生成摘要时出错

---

## 41. Waymo recalls 3,800 robotaxis after they drive into flood waters

**原文标题**: Waymo recalls 3,800 robotaxis after they drive into flood waters

**原文链接**: [https://www.cnbc.com/2026/05/12/waymo-recalls-3800-robotaxis-after-able-drive-into-standing-water.html](https://www.cnbc.com/2026/05/12/waymo-recalls-3800-robotaxis-after-able-drive-into-standing-water.html)

生成摘要时出错

---

## 42. What the Hell Was Going on with Cigarette Ads in the 70s? (2024)

**原文标题**: What the Hell Was Going on with Cigarette Ads in the 70s? (2024)

**原文链接**: [https://tohippo.com/what-the-hell-was-going-on-with-cigarette-ads-in-the-70s/](https://tohippo.com/what-the-hell-was-going-on-with-cigarette-ads-in-the-70s/)

生成摘要时出错

---

## 43. OpenAI is connecting ChatGPT to bank accounts via Plaid

**原文标题**: OpenAI is connecting ChatGPT to bank accounts via Plaid

**原文链接**: [https://firethering.com/chatgpt-bank-account-plaid-openai/](https://firethering.com/chatgpt-bank-account-plaid-openai/)

生成摘要时出错

---

## 44. Apple-OpenAI Relationship Frays, Setting Up Possible Legal Fight

**原文标题**: Apple-OpenAI Relationship Frays, Setting Up Possible Legal Fight

**原文链接**: [https://www.bloomberg.com/news/articles/2026-05-14/openai-apple-partnership-frays-setting-up-possible-legal-fight](https://www.bloomberg.com/news/articles/2026-05-14/openai-apple-partnership-frays-setting-up-possible-legal-fight)

生成摘要时出错

---

## 45. They Said It Would Cost $54M. We Said "No Thanks."

**原文标题**: They Said It Would Cost $54M. We Said "No Thanks."

**原文链接**: [https://nateglubish.substack.com/p/they-said-it-would-cost-54-million](https://nateglubish.substack.com/p/they-said-it-would-cost-54-million)

生成摘要时出错

---

## 46. Check Your Fucking Sources, People

**原文标题**: Check Your Fucking Sources, People

**原文链接**: [https://brodzinski.com/2026/05/check-fcking-sources.html](https://brodzinski.com/2026/05/check-fcking-sources.html)

生成摘要时出错

---

## 47. Safari and Firefox change how big sites render based on the domain

**原文标题**: Safari and Firefox change how big sites render based on the domain

**原文链接**: [https://denodell.com/blog/browsers-treat-big-sites-differently](https://denodell.com/blog/browsers-treat-big-sites-differently)

生成摘要时出错

---

## 48. The Whole Anthropic Kerfuffle

**原文标题**: The Whole Anthropic Kerfuffle

**原文链接**: [https://twitter.com/josevalim/status/2054887621336174799](https://twitter.com/josevalim/status/2054887621336174799)

生成摘要时出错

---

## 49. Show HN: GlycemicGPT – Open-source AI-powered diabetes management

**原文标题**: Show HN: GlycemicGPT – Open-source AI-powered diabetes management

**原文链接**: [https://github.com/GlycemicGPT/GlycemicGPT](https://github.com/GlycemicGPT/GlycemicGPT)

生成摘要时出错

---

## 50. Claude subscription changes coverage of `claude -p`

**原文标题**: Claude subscription changes coverage of `claude -p`

**原文链接**: [https://x.com/i/trending/2054617957440143639](https://x.com/i/trending/2054617957440143639)

生成摘要时出错

---

## 51. Elevated error rates on Opus 4.7

**原文标题**: Elevated error rates on Opus 4.7

**原文链接**: [https://status.claude.com/incidents/8z7l5zcy0v3b](https://status.claude.com/incidents/8z7l5zcy0v3b)

生成摘要时出错

---

## 52. Show HN: Race to the Bottom

**原文标题**: Show HN: Race to the Bottom

**原文链接**: [https://race-to-the-bottom.onrender.com](https://race-to-the-bottom.onrender.com)

生成摘要时出错

---

## 53. The sigmoids won't save you

**原文标题**: The sigmoids won't save you

**原文链接**: [https://www.astralcodexten.com/p/the-sigmoids-wont-save-you](https://www.astralcodexten.com/p/the-sigmoids-wont-save-you)

生成摘要时出错

---

## 54. I built Zenith: a live local-first fixed viewport planetarium

**原文标题**: I built Zenith: a live local-first fixed viewport planetarium

**原文链接**: [https://smorgasb.org/zenith-tech/](https://smorgasb.org/zenith-tech/)

生成摘要时出错

---

## 55. I was asked to install malware during a fake interview

**原文标题**: I was asked to install malware during a fake interview

**原文链接**: [https://ashishb.net/security/contagious-interview/](https://ashishb.net/security/contagious-interview/)

生成摘要时出错

---

## 56. Where's Ed: Anthropic Told Court $5B but Public $19B

**原文标题**: Where's Ed: Anthropic Told Court $5B but Public $19B

**原文链接**: [https://www.flyingpenguin.com/wheres-ed-anthropic-told-court-5-billion-but-public-19-billion/](https://www.flyingpenguin.com/wheres-ed-anthropic-told-court-5-billion-but-public-19-billion/)

生成摘要时出错

---

## 57. Overseas fakers using AI videos to push a narrative of UK decline, BBC finds

**原文标题**: Overseas fakers using AI videos to push a narrative of UK decline, BBC finds

**原文链接**: [https://www.bbc.co.uk/news/articles/ckgpyn30dp3o](https://www.bbc.co.uk/news/articles/ckgpyn30dp3o)

生成摘要时出错

---

## 58. Show HN: GridTravel – A community based travel app for users to share routes

**原文标题**: Show HN: GridTravel – A community based travel app for users to share routes

**原文链接**: [https://www.gridtravel.app](https://www.gridtravel.app)

生成摘要时出错

---

