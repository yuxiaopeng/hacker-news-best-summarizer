# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-05-15.md)

*最后自动更新时间: 2026-05-15 20:35:27*
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

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 2 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 3 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 4 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 5 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 6 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 7 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 8 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 9 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 10 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 11 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 12 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 13 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 14 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 15 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 16 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 17 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 18 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 19 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 20 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 21 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 22 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 23 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 24 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 25 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 26 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 27 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 28 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 29 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 30 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 31 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 32 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 33 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 34 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 35 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 36 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 37 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 38 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 39 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 40 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 41 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 42 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 43 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 44 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 45 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 46 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 47 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 48 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 49 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 50 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 51 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 52 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 53 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 54 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 55 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 56 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 57 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 58 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 59 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 60 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 61 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 62 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 63 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 64 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 65 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 66 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 67 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 68 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 69 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 70 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 71 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 72 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 73 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 74 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 75 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 76 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 77 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 78 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 79 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 80 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 81 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 82 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 83 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 84 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 85 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 86 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 87 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 88 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 89 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 90 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 91 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 92 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 93 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 94 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 95 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 96 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 97 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 98 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 99 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 100 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 101 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 102 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 103 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 104 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 105 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 106 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 107 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 108 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 109 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 110 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 111 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 112 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 113 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 114 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 115 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 116 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 117 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 118 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 119 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 120 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 121 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 122 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 123 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 124 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 125 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 126 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 127 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 128 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 129 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 130 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 131 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 132 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 133 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 134 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 135 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 136 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 137 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 138 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 139 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 140 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 141 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 142 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 143 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 144 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 145 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 146 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 147 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 148 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 149 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 150 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 151 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 152 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 153 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 154 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 155 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 156 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 157 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 158 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 159 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 160 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 161 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 162 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 163 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 164 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 165 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 166 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 167 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 168 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 169 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 170 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 171 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 172 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 173 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 174 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 175 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 176 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 177 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 178 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 179 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 180 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 181 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 182 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 183 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 184 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 185 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 186 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 187 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 188 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 189 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
