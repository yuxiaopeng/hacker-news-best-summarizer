# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2025-12-14.md)

*最后自动更新时间: 2025-12-14 19:45:22*
## 1. 我的Apple ID被苹果锁定了，我束手无策。求助。

**原文标题**: Apple has locked my Apple ID, and I have no recourse. A plea for help

**原文链接**: [https://hey.paris/posts/appleid/](https://hey.paris/posts/appleid/)

忠实的苹果用户兼专业开发者帕里斯报告称，他拥有25年之久的Apple ID已被永久锁定，这事实上已使他的数字生活陷入瘫痪，并导致其价值超过3万美元的苹果硬件形同废铁。该问题源于他尝试兑换一张价值500美元的苹果礼品卡，这张卡购自一家大型实体零售店，但据苹果公司称，该卡被标记为已被盗用。

此举已导致他的iPhone、iPad、Mac电脑和Apple Watch基本无法使用，并阻止了他访问数TB的家庭照片、消息历史记录以及数千美元的已购软件和媒体内容。他无法退出iCloud、无法使用iMessage、无法下载他的数据，也无法访问许多需要活跃Apple ID的苹果支持系统。

苹果支持部门没有提供任何关于此次封禁的解释，拒绝升级处理，并且不屑一顾地建议他“创建一个新的Apple账户”。这一建议是灾难性的，存在硬件被标记、因规避安全措施而导致账户进一步被禁用，以及他作为一名苹果开发者可能被列入黑名单的风险。

作为苹果编程语言技术书籍的作者和大型开发者活动的组织者，帕里斯强调了他长期以来对苹果生态系统的投入。他认为，是自动欺诈标记错误地触发了这种“核打击”，他恳求对他的案件进行人工审查，以恢复他的数字身份和访问权限。

---

## 2. OpenAI正在悄悄采用技能，现已在ChatGPT和Codex CLI中可用

**原文标题**: OpenAI are quietly adopting skills, now available in ChatGPT and Codex CLI

**原文链接**: [https://simonwillison.net/2025/Dec/12/openai-skills/](https://simonwillison.net/2025/Dec/12/openai-skills/)

OpenAI正在悄然整合一套类似于Anthropic的“技能”机制，到ChatGPT的Code Interpreter（代码解释器）和其Codex CLI工具中，截至2025年12月。这一采用验证了作者之前将技能视为AI重大发展的评估。

技能被构造成文件夹，包含一个Markdown文件（`skill.md`）和可选的资源/脚本，使大型语言模型（LLM）易于实现。

在**ChatGPT**中，技能可以通过`/home/oai/skills`文件夹在Code Interpreter（代码解释器）内部访问。当前技能涵盖电子表格、DOCX和PDF。值得注意的是，对于PDF和文档，OpenAI将页面转换为PNG，利用支持视觉的GPT模型来保留布局和图形，而不仅仅是提取文本。一个示例展示了GPT-5.2精心创建了一份关于新西兰红松（rimu trees）和鸮鹦鹉（kakapo）的PDF，甚至能自我纠正长音符号（macrons）的字体问题。

对于**Codex CLI**，两周前引入了技能的实验性支持。用户可以将技能安装到`~/.codex/skills`中，并通过`--enable skills`选项激活它们。一个示例展示了使用自定义技能完美生成了一个Datasette插件。

文章强调，OpenAI迅速采纳这种“轻量级规范”进一步证实了技能概念的强大。作者建议，对技能规范进行正式文档化将大有裨益，这可能由Agentic AI Foundation牵头。

---

## 3. 欧洲健康数据售予前以色列间谍掌管的美国公司

**原文标题**: Europeans' health data sold to US firm run by ex-Israeli spies

**原文链接**: [https://www.ftm.eu/articles/europe-health-data-us-firm-israel-spies](https://www.ftm.eu/articles/europe-health-data-us-firm-israel-spies)

欧洲通讯服务Zivver，被欧盟和英国政府、医院及法院用于机密通讯，现已被出售给一家与以色列情报机构有密切联系的美国公司Kiteworks，这引发了严重关切。

荷兰公司Zivver，经调查发现，尽管声称“零访问”，但其能够读取客户的“加密”内容。这意味着包括医疗和政府通讯在内的敏感欧洲数据，Zivver本身就已经可能访问。

Kiteworks的此次收购带来了两个主要问题：
1.  **美国司法管辖权：** 这些数据现在受制于侵入性的美国法律，这意味着无论数据存储在哪里，美国政府都可以要求访问。
2.  **与以色列情报机构的联系：** Kiteworks的首席执行官乔纳森·亚伦（Jonathan Yaron）和几位高级管理人员都曾是以色列精英军事情报8200部队的成员，该部队以窃听闻名。专家警告称，以色列情报机构与科技行业之间存在“旋转门”现象，这造成了一个漏洞，Zivver的敏感数据“金矿”可能被外国情报机构利用。

荷兰当局未能阻止或适当评估此次收购，将Zivver归类为非关键基础设施——专家称这一决定是“巨大失误”。批评人士强调，欧洲对其数字基础设施缺乏战略控制，呼吁加强监管，以保护重要的通讯服务免受外国影响和潜在的数据滥用。

---

## 4. macOS 26.2 通过 Thunderbolt RDMA 实现快速 AI 集群

**原文标题**: macOS 26.2 enables fast AI clusters with RDMA over Thunderbolt

**原文链接**: [https://developer.apple.com/documentation/macos-release-notes/macos-26_2-release-notes#RDMA-over-Thunderbolt](https://developer.apple.com/documentation/macos-release-notes/macos-26_2-release-notes#RDMA-over-Thunderbolt)

标题为“macOS 26.2 enables fast AI clusters with RDMA over Thunderbolt”的文章内容无法访问。页面没有显示文章，而是显示了一条错误消息，表明需要JavaScript才能查看其内容。

因此，无法提供关于macOS 26.2、其实现快速AI集群的能力以及通过Thunderbolt使用RDMA的实际文章内容的摘要。根据输入，文章本身的要点和关键信息均无法获取。

---

## 5. VPN宣称的位置与实际流量出口不符

**原文标题**: VPN location claims don't match real traffic exits

**原文链接**: [https://ipinfo.io/blog/vpn-location-mismatch-report](https://ipinfo.io/blog/vpn-location-mismatch-report)

IPinfo 的研究显示，在 20 个热门 VPN 中，有 17 个谎报了其流量出口位置。通过分析 137 个国家/地区的 15 万个出口 IP，他们发现许多提供商声称支持超过 100 个国家/地区，但实际上却通过少数几个物理数据中心（主要位于美国或欧洲）路由流量。其中有 38 个声称的国家/地区是“纯虚拟”的，意味着没有实际流量从这些地方出口。只有 Mullvad、IVPN 和 Windscribe 展现了完全可验证的位置。

当 VPN 应用甚至 IP 注册数据声称是“国家 X”，但活跃网络测量却显示流量从“国家 Y”出口时，就会出现虚拟位置，两者通常相隔数千公里（例如，巴哈马的流量从美国出口，索马里的流量从法国/英国出口）。传统的 IP 数据提供商常常依赖于自报数据，从而延续了这些错误，其位置中位数误差高达 3100 公里。

尽管虚拟位置存在技术原因（风险、成本），但缺乏透明度和大规模的不匹配现象造成了严重的信任问题，影响了用户、记者和反欺诈系统。IPinfo 通过“测量优先”的方法来解决这个问题，利用其 ProbeNet（1200 多个全球 PoP）进行主动 RTT 测量，以验证真实的物理位置。用户应对过长的国家列表持怀疑态度，并寻找透明标注虚拟位置的提供商。

---

## 6. 老鼠玩毁灭战士

**原文标题**: Rats Play DOOM

**原文链接**: [https://ratsplaydoom.com/](https://ratsplaydoom.com/)

《老鼠玩DOOM》一文详细介绍了一种专门为老鼠设计用于玩电子游戏的头戴设备，强调其独特的视觉界面和集成的感官功能。该头显能牢固地环绕老鼠的头部，集成一个可折叠的AMOLED屏幕，提供全高清分辨率以实现最大沉浸感，同时确保老鼠的胡须不受阻碍。

除了显示屏，该头显还集成了几个关键的感官组件。它在左右胡须附近设有两个小型气嘴，能够提供定向气流，以提示游戏内事件，例如撞墙。框架还为奖励系统的分配管提供了一个牢固的安装点，将其方便地定位在老鼠嘴巴附近。此外，该设计还在每只耳朵附近预留了微型立体声扬声器的安装位置，表明未来有集成音频提示的计划。该描述还辅以对视觉辅助材料的引用，例如“头显特写”和“3D模型：头显”。

---

## 7. GNU 统一字体

**原文标题**: GNU Unifont

**原文链接**: [https://unifoundry.com/unifont/index.html](https://unifoundry.com/unifont/index.html)

GNU Unifont 是一个 GNU 项目字体，提供对可打印 Unicode 码点的全面覆盖，主要涵盖基本多文种平面 (BMP)，并日益支持辅助多文种平面 (SMP) 和 ConScript Unicode 注册表 (CSUR)。

它采用双重许可，即附带 GNU 字体嵌入例外条款的 GNU GPLv2+ 许可和 SIL 开放字体许可 1.1。此许可明确允许商业使用，确保派生字体保持自由，并鸣谢志愿者贡献者。

Unifont 提供 OpenType、PCF、BDF、PSF 和 HEX 等多种格式下载，并提供针对日文、更高 Unicode 平面和 CSUR 字形的专门版本。Windows 和 Mac OS X 用户可以将未压缩的字体文件安装到其系统的“字体”文件夹中。在 Mac 终端上，为了实现正确显示，可能需要启用抗锯齿功能。

Unifont 的一个显著局限是每个码点只存储一个字形。这使其不太适合需要上下文塑形、连字或浮动元音标记才能准确显示的复杂文字系统（如印度语系或阿拉伯语系文字）。对于这些文字系统，它通常作为“最后的备用字体”使用。

开发工作持续进行，众多贡献者在所有 Unicode 平面添加和修改字形。近期发布的版本（例如 17.0、16.0）详细说明了广泛的更新，包括对中文、阿拉伯文、格鲁吉亚文、古突厥文和表情符号字形的改进，以及新增的文字和符号。鼓励希望贡献新字形的志愿者提前联系项目组协调工作，需注意受中华人民共和国版权保护的 CJK 字形不能包含在该自由字体中。

---

## 8. I tried Gleam for Advent of Code

**原文标题**: I tried Gleam for Advent of Code

**原文链接**: [https://blog.tymscar.com/posts/gleamaoc2025/](https://blog.tymscar.com/posts/gleamaoc2025/)

生成摘要时出错

---

## 9. Linux Sandboxes and Fil-C

**原文标题**: Linux Sandboxes and Fil-C

**原文链接**: [https://fil-c.org/seccomp](https://fil-c.org/seccomp)

生成摘要时出错

---

## 10. Recovering Anthony Bourdain's Li.st's

**原文标题**: Recovering Anthony Bourdain's Li.st's

**原文链接**: [https://sandyuraz.com/blogs/bourdain/](https://sandyuraz.com/blogs/bourdain/)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 2 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 3 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 4 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 5 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 6 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 7 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 8 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 9 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 10 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 11 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 12 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 13 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 14 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 15 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 16 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 17 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 18 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 19 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 20 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 21 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 22 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 23 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 24 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 25 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 26 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 27 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 28 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 29 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 30 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 31 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 32 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 33 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 34 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
| 35 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 36 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 37 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 38 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 39 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
