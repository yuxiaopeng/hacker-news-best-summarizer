# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-06-13.md)

*最后自动更新时间: 2026-06-13 20:31:46*
## 1. HN 展示：用于从网页界面批量删除 Claude 聊天的脚本

**原文标题**: Show HN: Script to bulk delete Claude chats from the web UI

**原文链接**: [https://github.com/MatteoLeonesi/bulk-delete-claude-chat](https://github.com/MatteoLeonesi/bulk-delete-claude-chat)

本文介绍了一个JavaScript脚本，旨在从Claude.ai批量删除对话，解决了原生用户界面（UI）中“全选”按钮只能选择可见聊天记录的局限性。

该脚本`delete-all.js`利用了通过浏览器网络请求推断出的Claude.ai网络应用程序内部的、未公开的端点。提醒用户，这些端点随时可能更改或停止工作，且该脚本与Anthropic公司无关。它仅限在用户自己的Claude账户上使用。

使用脚本：
1. 访问`https://claude.ai/recents`。
2. 打开浏览器开发者控制台（F12）。
3. 粘贴脚本内容并按回车键。
4. 确认所有弹窗（每个组织一个）。
5. 请耐心等待；对话将在几分钟内缓慢消失。
6. 保持`claude.ai`标签页打开，直到控制台显示“Finished”，以确保过程完成。

该脚本采用MIT许可证。

---

## 2. 上诉法院维持FTX联合创始人山姆·班克曼-弗里德的欺诈罪定罪

**原文标题**: Appeals court upholds FTX co-founder Sam Bankman-Fried's fraud conviction

**原文链接**: [https://apnews.com/article/sam-bankman-fried-ftx-cryptocurrency-appeal-e709df4a152e9b3b52a266dd81eb44cc](https://apnews.com/article/sam-bankman-fried-ftx-cryptocurrency-appeal-e709df4a152e9b3b52a266dd81eb44cc)

联邦上诉法院维持了FTX联合创始人萨姆·班克曼-弗里德的诈骗定罪和25年监禁。位于曼哈顿的美国第二巡回上诉法院周五裁定，政府的证据“确凿有力”，2023年的审判“并无不公”。

班克曼-弗里德被陪审团裁定诈骗客户和投资者数十亿美元。上诉法院确认他将FTX用作其“个人存钱罐”，挪用客户资金用于房地产、政治捐款和投资。他同时向客户保证其资金安全，同时伪造商业记录以隐瞒这些交易。

法院驳回了辩方关于审判因法官限制证据的裁决而不公的主张。34岁的班克曼-弗里德在FTX于2022年11月崩溃后，于2023年被定罪。此次崩溃导致客户损失约80亿美元，投资者损失17亿美元，贷方损失13亿美元，总损失超过110亿美元。他的庭审证词曾被刘易斯·A·卡普兰法官批评为伪证和闪烁其词。

---

## 3. You can power on a Mac remotely

**原文标题**: You can power on a Mac remotely

**原文链接**: [https://www.jeffgeerling.com/blog/2026/power-on-your-mac-remotely/](https://www.jeffgeerling.com/blog/2026/power-on-your-mac-remotely/)

生成摘要时出错

---

## 4. 如何用计算机视觉自动化Instagram互动（以及被封号）

**原文标题**: How to automate Instagram engagements with computer vision (and get banned)

**原文链接**: [https://blog.florianherrengt.com/how-to-automate-instagram-engagements.html](https://blog.florianherrengt.com/how-to-automate-instagram-engagements.html)

本文详细介绍了一项利用计算机视觉自动化Instagram互动的实验，并明确指出此类活动会导致账号封禁。传统的自动化方法之所以失败，是因为Instagram的DOM（文档对象模型）高度动态且经过混淆。作者通过专注于用户界面的视觉一致性来绕过这一点，因为该界面必须保持对人类可导航。

核心思想是截取屏幕截图，利用计算机视觉在视觉上定位UI元素（例如心形图标），然后在其坐标处模拟鼠标点击。初步尝试面临的困难是移动的元素以及在搜索整个屏幕时出现过多的误报。

解决方案涉及一个精炼的流程：
1.  **缩小搜索空间**：识别稳定的“地标”（例如三点菜单、操作栏），以动态定义一个小的、相关的裁剪区域，预期目标图标（如心形）会出现在此处。这适应了各种帖子布局。
2.  **滑动窗口模板匹配**：在这个缩小区域内应用宽松的模板匹配，以找到潜在的心形图标。
3.  **垂直对齐过滤器**：由于实际的心形图标出现在一个一致的垂直列中，因此过滤掉那些与最常见的X坐标不一致的检测结果，从而消除大部分误报。

尽管包含了模拟人类的光标移动和随机化计时，实验账户仍在几天内被封禁，这证明了Instagram复杂的机器人检测机制。作者强调了这项“对抗性”实验的价值，即在于理解机器人检测策略以及正常用户行为与自动化用户行为之间的区别。

---

## 5. 英特尔8087浮点芯片的核心加法器

**原文标题**: The adder at the heart of Intel's 8087 floating-point chip

**原文链接**: [https://www.righto.com/2026/06/intel-8087-adder-reverse-engineered.html](https://www.righto.com/2026/06/intel-8087-adder-reverse-engineered.html)

1980年发布的Intel 8087浮点协处理器，凭借其核心的69位加法器，在数学运算中取得了显著的速度提升。本文将解释其精密的内部设计，该设计解决了多位数据快速进位传播的挑战。

8087的加法器采用了两种主要优化：
1.  **4位块：** 将加法分解成4位块，从而减少了总体的进位步骤数。
2.  **曼彻斯特进位链：** 在每个块内，使用优化的曼彻斯特进位链。这项基于“生成”、“传播”和“删除”信号的技术，允许进位值通过并行开关快速流动，避免了逻辑门造成的延迟。如果所有位都处于“传播”状态，一个“进位跳跃”电路还会允许进位绕过内部块计算，进一步提高了速度。

在电气层面，8087的NMOS晶体管在将信号拉低时速度更快。因此，进位线被预充电到5V（表示无进位），如果需要进位，则将其拉低。在预充电期间，传播信号被强制置高，以连接所有进位线。

该加法器的69位输入包含了三个舍入位（保护位、舍入位、粘滞位）、B寄存器中数值可能加倍的情况，以及用于减法的二补数求反。它产生一个70位的输出。周围电路，如尾数总线、B寄存器、和寄存器以及移位器（跳过和求和），协同执行乘法、除法和平方根运算，加法器是这些迭代过程的核心。

8087的加法器，凭借其曼彻斯特进位链和进位跳跃机制，是平衡复杂性和性能的关键组件，使芯片能够在两个时钟周期内完成加法运算。

---

## 6. 卡吉魔法

**原文标题**: Kagi Magic

**原文链接**: [https://kagi.com/magic](https://kagi.com/magic)

文章《Kagi魔力》批判了当前搜索引擎的现状，哀叹它们已从信息查找工具转变为优先展示AI概览、充斥广告、付费排名和无处不在的监控。文章认为，现代搜索对用户而言已变得大体上无关紧要且令人沮丧。

Kagi搜索被提出作为解决这些问题的一种替代方案。与传统的“免费”搜索引擎不同，Kagi采用用户付费订阅模式，确保其忠诚度完全面向用户。这种模式使Kagi能够提供一个干净、私密、无广告的体验，摆脱了侵入性AI总结或数据利用。用户可以通过提升可信来源、屏蔽不需要的内容以及根据特定需求调整结果来完全定制他们的搜索体验。

像Cory Doctorow和Gizmodo的Matthew Gault这样的用户评价将Kagi描述为“魔力”和“颠覆性”的，声称它超越了鼎盛时期的谷歌。用户普遍反映，在体验了Kagi准确、可定制和以用户为中心的结果后，他们无法再回到其他搜索引擎。文章最后邀请怀疑论者尝试Kagi，并断言，尽管是付费的，但这种卓越、以用户为中心的网络体验最终是值得投资的。

---

## 7. 发布 HN: BitBoard (YC P25) — 智能体分析工作区

**原文标题**: Launch HN: BitBoard (YC P25) – Analytics Workspace for Agents

**原文链接**: [https://bitboard.work/](https://bitboard.work/)

BitBoard，一家YC P25初创公司，已正式推出一个专门为代理（agents）设计的分析工作空间。该平台允许用户利用他们偏爱的AI聊天或编码工具来生成仪表盘并进行数据分析。BitBoard的一个关键创新在于它能够将这些AI生成的分析从短暂的一次性聊天线程转化为相互关联、持久的资产。这意味着从AI代理获得的洞察可以被保存、整理和在此基础上进行构建，防止它们在短暂的对话中丢失。本质上，BitBoard旨在为AI驱动的数据探索和可视化提供一个持久的家园。

---

## 8. 专访英特尔基拉·博伊科：至强6产品总监

**原文标题**: An Interview with Intel's Kira Boyko: Xeon 6's Product Director

**原文链接**: [https://chipsandcheese.com/p/an-interview-with-intels-kira-boyko](https://chipsandcheese.com/p/an-interview-with-intels-kira-boyko)

在2026年的台北国际电脑展(Computex)的一次采访中，英特尔Xeon 6+产品总监Kira Boyko详细介绍了她广泛的职责以及这款新推出的处理器。Boyko负责定义产品规格、确定目标市场细分、设定性能关键绩效指标(KPI)，并监督从概念到交付的整个执行过程。她深入参与SKU规划，平衡客户需求与制造能力，并对Xeon 6+精简的路线图感到自豪。她对产品的参与早在产品发布前几年就开始了。

Xeon 6+的一个突出特性是英特尔应用能耗遥测(AET)，这是一项将在未来所有Xeon处理器上推出的全新硬件级功能。AET能够以核心级别精确跟踪工作负载的能耗，从单个核心到整个封装。这使得客户能够优化工作负载编排以降低能耗，提供透明的能源成本分摊，或提供使用激励。Boyko强调了AET相对于基于软件的解决方案的优势，因为它直接集成了硬件，这降低了开销并减少了潜在的误用。AET在所有Xeon 6+ SKU上均可用，并可即开即用。

Boyko还强调了英特尔服务器和客户端部门之间显著的“交叉授粉”效应，促进了技术和知识的共享。值得注意的是，Xeon 6+是首款18A制程的Xeon处理器。采访最后以轻松愉快的关于喜爱奶酪的交流收尾，其中Boyko表达了她对蓝纹奶酪的喜爱。

---

## 9. Elon Musk Becomes First Trillionaire as SpaceX Starts Trading

**原文标题**: Elon Musk Becomes First Trillionaire as SpaceX Starts Trading

**原文链接**: [https://www.nytimes.com/live/2026/06/12/business/spacex-ipo-elon-musk/heres-the-latest](https://www.nytimes.com/live/2026/06/12/business/spacex-ipo-elon-musk/heres-the-latest)

生成摘要时出错

---

## 10. SkillSpector

**原文标题**: SkillSpector

**原文链接**: [https://github.com/NVIDIA/SkillSpector](https://github.com/NVIDIA/SkillSpector)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 2 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 3 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 4 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 5 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 6 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 7 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 8 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 9 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 10 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 11 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 12 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 13 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 14 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 15 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 16 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 17 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 18 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 19 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 20 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 21 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 22 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 23 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 24 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 25 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 26 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 27 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 28 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 29 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 30 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 31 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 32 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 33 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 34 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 35 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 36 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 37 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 38 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 39 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 40 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 41 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 42 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 43 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 44 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 45 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 46 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 47 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 48 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 49 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 50 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 51 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 52 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 53 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 54 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 55 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 56 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 57 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 58 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 59 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 60 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 61 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 62 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 63 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 64 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 65 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 66 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 67 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 68 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 69 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 70 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 71 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 72 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 73 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 74 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 75 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 76 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 77 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 78 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 79 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 80 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 81 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 82 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 83 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 84 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 85 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 86 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 87 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 88 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 89 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 90 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 91 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 92 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 93 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 94 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 95 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 96 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 97 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 98 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 99 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 100 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 101 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 102 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 103 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 104 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 105 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 106 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 107 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 108 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 109 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 110 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 111 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 112 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 113 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 114 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 115 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 116 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 117 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 118 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 119 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 120 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 121 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 122 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 123 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 124 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 125 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 126 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 127 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 128 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 129 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 130 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 131 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 132 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 133 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 134 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 135 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 136 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 137 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 138 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 139 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 140 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 141 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 142 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 143 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 144 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 145 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 146 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 147 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 148 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 149 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 150 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 151 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 152 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 153 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 154 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 155 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 156 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 157 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 158 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 159 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 160 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 161 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 162 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 163 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 164 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 165 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 166 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 167 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 168 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 169 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 170 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 171 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 172 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 173 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 174 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 175 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 176 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 177 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 178 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 179 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 180 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 181 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 182 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 183 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 184 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 185 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 186 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 187 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 188 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 189 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 190 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 191 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 192 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 193 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 194 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 195 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 196 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 197 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 198 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 199 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 200 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 201 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 202 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 203 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 204 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 205 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 206 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 207 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 208 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 209 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 210 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 211 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 212 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 213 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 214 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 215 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 216 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 217 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 218 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
