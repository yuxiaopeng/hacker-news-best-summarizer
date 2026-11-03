# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-11-03.md)

*最后自动更新时间: 2026-11-03 01:52:35*
## 1. Astra 可以读写权重来改进 Qwen。

**原文标题**: Astra can read and write weights to improve Qwen

**原文链接**: [https://rikiyat.github.io/blog/weight-space-programming/](https://rikiyat.github.io/blog/weight-space-programming/)

本文介绍了“权重空间编程”，这是一种开创性的范式，在其中，前沿大型语言模型（LLM），特别是GPT-6 Astra，能够直接原生读写神经网络权重。这一过程无需传统的优化器、梯度下降或训练循环，而是利用LLM的推理能力来理解和操纵网络组件。

这种能力，无论是对人类还是传统算法来说都出人意料，并在以下三个关键领域有所体现：
1.  **读取权重：** Astra能够根据网络的原始权重准确推断其功能。实验表明，它能识别出网络所训练的游戏（例如，Breakout）、扩散模型生成的形状，或小型语言模型学习的语言，甚至能从孤立的中间层中识别出特定注意力头的作用。
2.  **修正权重：** Astra能够诊断并纠正现有网络中的问题。至关重要的是，它通过编辑Qwen3.5-0.8B仅0.016%的权重来修正推理循环，从而显著提升了其数学性能（MATH-500从7.9%提升到48.1%）和指令遵循能力。它还修正了一个陷入局部最优的“坡道汽车”策略。
3.  **从零开始编写权重：** Astra能够从零开始为新网络生成权重，创建出用于MinAtar游戏的微型游戏网络，这些网络性能超越了通过PPO训练1亿步的策略。

这项研究预示着深度学习领域的一次重大转变，即从Adam等简化的符号优化器，转向能够推理并直接优化神经网络权重的LLM，这对于可解释性和优化都具有深远的影响。

---

## 2. HN展示：HackerBooks — HackerTube，但用于在 HN 上提及的书籍

**原文标题**: Show HN: HackerBooks – HackerTube, but for books mentioned on HN

**原文链接**: [https://hackerbooks.org](https://hackerbooks.org)

HackerBooks 是一个在 Hacker News (Show HN) 上推出的新项目，旨在成为一个专门平台，用于汇集 Hacker News 社区内提及和讨论的书籍。它被描述为“HackerTube，但用于 HN 上提及的书籍”，旨在汇总并组织这些推荐书目。

该服务提供了一个集中式资源，用户可以从中发现其科技达人同行中流行或相关的书籍，这些书籍直接来源于 Hacker News 上自然产生的讨论和分享的链接。本质上，它精选了一个由社区认可的“书籍库”，让 HN 读者更容易探索推荐读物。

---

## 3. 乌班图，搞什么鬼？

**原文标题**: WTF Ubuntu?

**原文链接**: [https://chalmovsky.com/posts/wtf-ubuntu](https://chalmovsky.com/posts/wtf-ubuntu)

作者对 Ubuntu 未能修补一个关键的 Linux 内核 TCP 漏洞 CVE-2026-98432 (CVSS 9.8) 表达了极度不满。这个自2016年就存在的漏洞，允许在几乎所有 Linux 服务器上远程获取 root 权限，据报道，已开发出可用的攻击工具。

Debian 已于10月16日修补了该漏洞，但截至11月2日，Ubuntu 仍未修补，尽管它承诺“及时提供补丁”，并且该漏洞具有高严重性评级和已公开的攻击工具。作者强调了讽刺之处在于，像 Debian、Arch 和 Alpine 这样由志愿者运营的发行版已经发布了修复程序，而销售安全订阅服务的 Canonical 却迟迟未发布。

这种延迟导致作者对 Ubuntu 彻底失去信任，促使他们将所有服务器从该平台迁移走，并由于风险而暂时将现有的 Ubuntu 服务器下线。鉴于此次关键的安全疏漏，作者批评 Ubuntu 的市场营销“空谈”毫无意义。

---

## 4. 挪威景观公路沿途卫生间

**原文标题**: Restrooms along the Norwegian Scenic Routes

**原文链接**: [https://www.visitnorway.com/plan-your-trip/travel-tips-a-z/norwegian-scenic-routes/worlds-best-toilets/](https://www.visitnorway.com/plan-your-trip/travel-tips-a-z/norwegian-scenic-routes/worlds-best-toilets/)

挪威国家旅游路线沿线的洗手间被誉为建筑杰作，其中几乎所有都由挪威知名或新锐建筑事务所设计。著名的例子包括斯诺赫塔（Snøhetta）在罗弗敦（Lofoten）埃格姆（Eggum）的设计，以及雷乌尔夫·拉姆施塔德（Reiulf Ramstad）在哈沃于松（Havøysund）旅游路线沿线的塞尔维卡（Selvika）的作品。

这些独特的建筑巧妙地分布在挪威多样化的地貌中，从北极圈以北、热门峡湾到偏远的山区高原。然而，由于严酷天气导致冬季道路封闭，许多只能在夏季开放。极端恶劣的条件有时需要坚固的结构，例如松恩山道（Sognefjellet）旅游路线沿线奥斯卡肖格（Oscarshaug）的钢筋加固洗手间，它尽管有实用的加固功能，但也拥有独特、几乎像维京头盔般的美学设计。

---

## 5. 联想的“加密”指纹U盘，只不过是一个装在外壳里的未加密SD卡。

**原文标题**: Lenovo's 'encrypted' fingerprint USB is just an unencrypted SD card in a case

**原文链接**: [https://www.reddit.com/r/technology/comments/1xl2pr3/lenovos_encrypted_fingerprint_usb_drive_is_just/](https://www.reddit.com/r/technology/comments/1xl2pr3/lenovos_encrypted_fingerprint_usb_drive_is_just/)

Reddit用户“Gellmar”的一篇帖子揭露了联想“加密”指纹U盘存在的重大设计缺陷和潜在的虚假宣传。Gellmar在拆解一个被宣传为安全外部存储解决方案的此类设备后发现，该U盘的内部组件由一张连接到USB适配器的标准、未加密的闪迪64GB microSD卡组成。

与产品“安全”和“加密”的品牌宣传相反，设备内部的实际存储介质并未采用硬件加密。这意味着，如果绕过外壳——例如，通过简单地取出microSD卡——存储在其中的数据将以明文形式轻易被访问，完全抵消了其宣称的所有安全优势。

这款联想产品中的“加密”似乎是在数据写入未加密的SD卡*之前*，由主机上的软件或一个简单的控制器处理的。这与真正安全的存储设备截然不同，后者直接在闪存控制器上集成了FIPS认证的硬件加密，确保即使存储芯片被物理移除，数据也能保持不可读。

这一发现引发了Reddit社区的担忧和批评，凸显了联想营销宣传与产品实际提供的安全机制之间可能存在差异。用户们表示失望，认为一个被宣传为安全的、指纹保护的U盘，提供的不过是一个装在华丽可上锁外壳里的未加密SD卡。

---

## 6. 占领SaaS

**原文标题**: OccupySaaS

**原文链接**: [https://occupysaas.com/](https://occupysaas.com/)

文章《OccupySaaS》批判了软件即服务（SaaS）中普遍存在的按席位定价模式。作者认为这种模式是一种“增长税”，直接惩罚了扩大员工规模的公司。每增加一名新成员——无论是正式员工、实习生还是承包商——都直接意味着一个额外的费用项和更高的软件使用成本。其核心论点是“基础设施不应按人头收费”，倡导一种不将服务成本与个人用户数量直接挂钩，而是支持而非阻碍组织规模扩大的定价结构。

---

## 7. 警察局长在Flock无视合同终止后拔掉摄像头。

**原文标题**: Police chief unplugs cameras after Flock ignores contract cancellation

**原文链接**: [https://www.thedrive.com/news/my-city-canceled-flocks-contract-flock-ignored-it-so-the-police-chief-unplugged-the-cameras](https://www.thedrive.com/news/my-city-canceled-flocks-contract-flock-ignored-it-so-the-police-chief-unplugged-the-cameras)

普利茅斯市与Flock Safety公司陷入纠纷，此前市议会于一个月前投票决定取消Flock ALPR（自动车牌识别）摄像头的合同。尽管合同已取消，但这些摄像头仍处于安装状态，Flock Safety公司拒绝承认合同终止。

普利茅斯警察局长埃里克·法登证实，在9月22日的市议会投票之后，他们立即暂停了所有用户账户，并正式将该决定通知了Flock Safety公司。然而，Flock公司的企业和法律部门对此保持沉默，仅通过一名当地代表进行沟通。

由于Flock公司不予回应，局长法登采取了直接行动，命令其工作人员断开摄像头的电源线，以确保它们不再运行或录像。作者乔尔·费德尔证实，他检查的多个摄像头确实已断电。

法登表示，这些摄像头是Flock公司的财产，城市仍在努力获取移除它们的时间表，但Flock公司尚未提供。此外，《The Drive》杂志也联系了Flock公司，要求其澄清合同取消流程，但未收到任何回应。

---

## 8. The AI cost of JavaScript frameworks

**原文标题**: The AI cost of JavaScript frameworks

**原文链接**: [https://nolanlawson.com/2026/10/28/the-ai-cost-of-javascript-frameworks/](https://nolanlawson.com/2026/10/28/the-ai-cost-of-javascript-frameworks/)

生成摘要时出错

---

## 9. Patrick Stewart taught us what good men do with power

**原文标题**: Patrick Stewart taught us what good men do with power

**原文链接**: [https://www.vox.com/politics/508526/patrick-stewart-jean-luc-picard-star-trek-liberalism](https://www.vox.com/politics/508526/patrick-stewart-jean-luc-picard-star-trek-liberalism)

生成摘要时出错

---

## 10. If you love a website, back it up

**原文标题**: If you love a website, back it up

**原文链接**: [https://blog.mistys-internet.website/post/2026/10/29/if-you-love-a-website-back-it-up/](https://blog.mistys-internet.website/post/2026/10/29/if-you-love-a-website-back-it-up/)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-11-03](output/hacker_news_summary_2026-11-03.md) |
| 2 | [2026-10-29](output/hacker_news_summary_2026-10-29.md) |
| 3 | [2026-10-25](output/hacker_news_summary_2026-10-25.md) |
| 4 | [2026-10-30](output/hacker_news_summary_2026-10-30.md) |
| 5 | [2026-10-27](output/hacker_news_summary_2026-10-27.md) |
| 6 | [2026-10-24](output/hacker_news_summary_2026-10-24.md) |
| 7 | [2026-10-28](output/hacker_news_summary_2026-10-28.md) |
| 8 | [2026-10-31](output/hacker_news_summary_2026-10-31.md) |
| 9 | [2026-10-26](output/hacker_news_summary_2026-10-26.md) |
| 10 | [2026-11-01](output/hacker_news_summary_2026-11-01.md) |
| 11 | [2026-10-21](output/hacker_news_summary_2026-10-21.md) |
| 12 | [2026-10-22](output/hacker_news_summary_2026-10-22.md) |
| 13 | [2026-10-17](output/hacker_news_summary_2026-10-17.md) |
| 14 | [2026-10-18](output/hacker_news_summary_2026-10-18.md) |
| 15 | [2026-10-16](output/hacker_news_summary_2026-10-16.md) |
| 16 | [2026-10-19](output/hacker_news_summary_2026-10-19.md) |
| 17 | [2026-10-23](output/hacker_news_summary_2026-10-23.md) |
| 18 | [2026-10-20](output/hacker_news_summary_2026-10-20.md) |
| 19 | [2026-10-14](output/hacker_news_summary_2026-10-14.md) |
| 20 | [2026-10-13](output/hacker_news_summary_2026-10-13.md) |
| 21 | [2026-10-11](output/hacker_news_summary_2026-10-11.md) |
| 22 | [2026-10-15](output/hacker_news_summary_2026-10-15.md) |
| 23 | [2026-10-06](output/hacker_news_summary_2026-10-06.md) |
| 24 | [2026-10-10](output/hacker_news_summary_2026-10-10.md) |
| 25 | [2026-10-07](output/hacker_news_summary_2026-10-07.md) |
| 26 | [2026-10-09](output/hacker_news_summary_2026-10-09.md) |
| 27 | [2026-09-27](output/hacker_news_summary_2026-09-27.md) |
| 28 | [2026-09-24](output/hacker_news_summary_2026-09-24.md) |
| 29 | [2026-09-30](output/hacker_news_summary_2026-09-30.md) |
| 30 | [2026-10-01](output/hacker_news_summary_2026-10-01.md) |
| 31 | [2026-09-29](output/hacker_news_summary_2026-09-29.md) |
| 32 | [2026-10-03](output/hacker_news_summary_2026-10-03.md) |
| 33 | [2026-09-25](output/hacker_news_summary_2026-09-25.md) |
| 34 | [2026-10-04](output/hacker_news_summary_2026-10-04.md) |
| 35 | [2026-10-02](output/hacker_news_summary_2026-10-02.md) |
| 36 | [2026-09-19](output/hacker_news_summary_2026-09-19.md) |
| 37 | [2026-09-17](output/hacker_news_summary_2026-09-17.md) |
| 38 | [2026-09-18](output/hacker_news_summary_2026-09-18.md) |
| 39 | [2026-09-22](output/hacker_news_summary_2026-09-22.md) |
| 40 | [2026-09-21](output/hacker_news_summary_2026-09-21.md) |
| 41 | [2026-09-23](output/hacker_news_summary_2026-09-23.md) |
| 42 | [2026-09-20](output/hacker_news_summary_2026-09-20.md) |
| 43 | [2026-09-16](output/hacker_news_summary_2026-09-16.md) |
| 44 | [2026-09-11](output/hacker_news_summary_2026-09-11.md) |
| 45 | [2026-09-07](output/hacker_news_summary_2026-09-07.md) |
| 46 | [2026-09-10](output/hacker_news_summary_2026-09-10.md) |
| 47 | [2026-09-13](output/hacker_news_summary_2026-09-13.md) |
| 48 | [2026-09-15](output/hacker_news_summary_2026-09-15.md) |
| 49 | [2026-09-12](output/hacker_news_summary_2026-09-12.md) |
| 50 | [2026-09-09](output/hacker_news_summary_2026-09-09.md) |
| 51 | [2026-09-08](output/hacker_news_summary_2026-09-08.md) |
| 52 | [2026-09-14](output/hacker_news_summary_2026-09-14.md) |
| 53 | [2026-09-04](output/hacker_news_summary_2026-09-04.md) |
| 54 | [2026-08-28](output/hacker_news_summary_2026-08-28.md) |
| 55 | [2026-09-01](output/hacker_news_summary_2026-09-01.md) |
| 56 | [2026-08-29](output/hacker_news_summary_2026-08-29.md) |
| 57 | [2026-09-06](output/hacker_news_summary_2026-09-06.md) |
| 58 | [2026-09-02](output/hacker_news_summary_2026-09-02.md) |
| 59 | [2026-09-05](output/hacker_news_summary_2026-09-05.md) |
| 60 | [2026-08-30](output/hacker_news_summary_2026-08-30.md) |
| 61 | [2026-08-31](output/hacker_news_summary_2026-08-31.md) |
| 62 | [2026-09-03](output/hacker_news_summary_2026-09-03.md) |
| 63 | [2026-08-23](output/hacker_news_summary_2026-08-23.md) |
| 64 | [2026-08-16](output/hacker_news_summary_2026-08-16.md) |
| 65 | [2026-08-24](output/hacker_news_summary_2026-08-24.md) |
| 66 | [2026-08-26](output/hacker_news_summary_2026-08-26.md) |
| 67 | [2026-08-20](output/hacker_news_summary_2026-08-20.md) |
| 68 | [2026-08-19](output/hacker_news_summary_2026-08-19.md) |
| 69 | [2026-08-25](output/hacker_news_summary_2026-08-25.md) |
| 70 | [2026-08-21](output/hacker_news_summary_2026-08-21.md) |
| 71 | [2026-08-18](output/hacker_news_summary_2026-08-18.md) |
| 72 | [2026-08-15](output/hacker_news_summary_2026-08-15.md) |
| 73 | [2026-08-22](output/hacker_news_summary_2026-08-22.md) |
| 74 | [2026-08-17](output/hacker_news_summary_2026-08-17.md) |
| 75 | [2026-08-13](output/hacker_news_summary_2026-08-13.md) |
| 76 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 77 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 78 | [2026-08-09](output/hacker_news_summary_2026-08-09.md) |
| 79 | [2026-08-12](output/hacker_news_summary_2026-08-12.md) |
| 80 | [2026-08-10](output/hacker_news_summary_2026-08-10.md) |
| 81 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 82 | [2026-08-14](output/hacker_news_summary_2026-08-14.md) |
| 83 | [2026-08-11](output/hacker_news_summary_2026-08-11.md) |
| 84 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 85 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 86 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 87 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 88 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 89 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 90 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 91 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 92 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 93 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 94 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 95 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 96 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 97 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 98 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 99 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 100 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 101 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 102 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 103 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 104 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 105 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 106 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 107 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 108 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 109 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 110 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 111 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 112 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 113 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 114 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 115 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 116 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 117 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 118 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 119 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 120 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 121 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 122 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 123 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 124 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 125 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 126 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 127 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 128 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 129 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 130 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 131 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 132 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 133 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 134 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 135 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 136 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 137 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 138 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 139 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 140 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 141 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 142 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 143 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 144 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 145 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 146 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 147 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 148 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 149 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 150 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 151 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 152 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 153 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 154 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 155 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 156 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 157 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 158 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 159 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 160 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 161 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 162 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 163 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 164 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 165 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 166 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 167 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 168 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 169 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 170 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 171 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 172 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 173 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 174 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 175 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 176 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 177 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 178 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 179 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 180 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 181 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 182 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 183 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 184 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 185 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 186 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 187 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 188 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 189 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 190 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 191 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 192 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 193 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 194 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 195 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 196 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 197 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 198 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 199 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 200 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 201 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 202 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 203 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 204 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 205 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 206 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 207 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 208 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 209 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 210 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 211 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 212 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 213 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 214 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 215 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 216 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 217 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 218 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 219 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 220 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 221 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 222 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 223 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 224 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 225 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 226 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 227 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 228 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 229 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 230 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 231 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 232 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 233 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 234 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 235 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 236 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 237 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 238 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 239 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 240 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 241 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 242 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 243 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 244 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 245 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 246 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 247 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 248 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 249 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 250 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 251 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 252 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 253 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 254 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 255 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 256 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 257 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 258 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 259 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 260 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 261 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 262 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 263 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 264 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 265 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 266 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 267 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 268 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 269 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 270 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 271 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 272 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 273 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 274 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 275 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 276 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 277 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 278 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 279 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 280 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 281 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 282 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 283 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 284 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 285 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 286 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 287 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 288 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 289 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 290 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 291 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 292 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 293 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 294 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 295 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 296 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 297 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 298 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 299 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 300 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 301 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 302 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 303 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 304 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 305 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 306 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 307 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 308 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 309 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 310 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 311 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 312 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 313 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 314 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 315 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 316 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 317 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 318 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 319 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 320 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 321 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 322 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 323 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 324 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 325 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 326 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 327 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 328 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 329 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 330 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 331 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 332 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 333 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 334 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 335 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 336 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 337 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 338 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 339 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 340 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 341 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 342 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 343 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 344 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 345 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 346 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 347 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 348 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 349 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 350 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 351 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 352 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 353 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
