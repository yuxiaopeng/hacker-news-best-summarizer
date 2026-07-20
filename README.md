# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-07-20.md)

*最后自动更新时间: 2026-07-20 20:45:32*
## 1. 美国人对数据中心感到愤怒。政治家们感受到了压力。

**原文标题**: Americans are angry about data centers. Politicians are feeling the pressure

**原文链接**: [https://www.reuters.com/world/us/americans-are-angry-about-data-centers-politicians-are-feeling-pressure-2026-07-16/](https://www.reuters.com/world/us/americans-are-angry-about-data-centers-politicians-are-feeling-pressure-2026-07-16/)

无法访问文章链接。

---

## 2. HMD 触控 4G

**原文标题**: HMD Touch 4G

**原文链接**: [https://www.hmd.com/en_int/hmd-touch-4g](https://www.hmd.com/en_int/hmd-touch-4g)

HMD Touch 4G 的亮点在于其炫彩触摸屏，该屏幕还提供流畅的滚动功能。

---

## 3. Co-evolution of self-replication and function in a digital primordial soup

**原文标题**: Co-evolution of self-replication and function in a digital primordial soup

**原文链接**: [https://arxiv.org/abs/2607.09211](https://arxiv.org/abs/2607.09211)

生成摘要时出错

---

## 4. 那个帖子根本不存在。别听那个东西。

**原文标题**: That post never existed. Stop listening to that thing

**原文链接**: [https://rachelbythebay.com/w/2026/05/05/404/](https://rachelbythebay.com/w/2026/05/05/404/)

所提供URL的文章，标题为“那篇文章从未存在过。别再听信那个东西了。”，是对一个404错误页面的巧妙元评论。与传统博文不同，该页面的内容明确指出：“这篇文章不存在。”作者Rachel by the Bay对内容缺失的原因给出了一些常见而幽默的解释，包括用户可能打错字了、文章已被移动或作者已将其删除。本质上，这篇文章本身 *就是* 一个404错误信息，它利用自己的标题和URL结构（其中包含“404”），以玩味的方式探讨内容的不存在性，而不是提供内容。它通过声明信息从未存在过，颠覆了人们寻找信息的预期，从而创造了一个关于互联网上缺失页面的自我指涉的笑话。

---

## 5. Hyprland 0.55 宣布将配置文件改为 Lua。

**原文标题**: Hyprland 0.55 announced the switch to Lua for its config files

**原文链接**: [https://hypr.land/news/update55/](https://hypr.land/news/update55/)

Hyprland 0.55 已发布，标志着一次大规模更新，带来了重大变化和新功能。最突出的亮点是配置文件的*官方切换到Lua*。虽然现有的hyprlang配置在未来几个版本中仍将可用，但建议用户进行迁移，Hyprland维基已更新以反映新的Lua语法。

利用Lua的特性，此次更新引入了*布局API*，使用户能够直接在配置文件中定义自定义布局，这些布局可以全局应用、按工作区应用或按显示器应用。

主要改进还包括：
*   *滚动增强*：原生支持tape模式下的全屏窗口，并通过Lua中的`scroll_move`实现新的触控板手势。
*   *ICC配置文件*：用户现在可以为每个输出加载ICC配置文件，以提高色彩准确性。
*   *渲染器和色彩管理 (CM) 改进*：Hyprland现在默认使用FP16精度和增强的CM管道，从而提升色彩准确性和屏幕共享能力。

一些*破坏性变更*包括移除或重新定位了部分配置选项，例如`dwindle:pseudotile`和`decoration:shadow:ignore_window`。此次发布还包含众多小幅新增功能和修复，例如新的滚动选项、设备标签、`confine_pointer`规则、群组管理功能、实时捏合光标缩放手势、新的发光窗口装饰，以及无数的bug修复。

---

## 6. C64 Basic 地牢探索游戏：哥布林袭击 (C64 Basic 第8部分)

**原文标题**: C64 Basic Dungeon Crawler: Goblin Attack (C64 Basic Part 8)

**原文链接**: [https://retrogamecoders.com/c64-basic-dungeon-part8/](https://retrogamecoders.com/c64-basic-dungeon-part8/)

C64 Basic 地牢探索系列游戏的第八期主要关注如何将战斗遭遇集成到游戏中，特别是“哥布林袭击”。

文章详细介绍了每当玩家移动时，遭遇是如何随机触发的（10% 的几率）。如果发生遭遇，程序会调用一个专门的战斗子程序（代码行 2000-2999）。该子程序会初始化怪物的属性，例如它的名字（“哥布林”）、生命值（`MH`）、攻击力（`MA`），以及击败它后获得的经验值（`EX`）。

战斗以回合制进行。玩家会获得选项：按 'A' 进行攻击或按 'R' 进行逃跑。攻击会根据玩家的等级计算随机伤害，并减少怪物的生命值。如果怪物的生命值降至零，玩家获胜，获得经验值，并返回地牢。如果玩家选择逃跑，有 50% 的成功几率，让他们返回地牢。逃跑失败会导致怪物获得一次自由攻击。

在玩家的回合之后，如果怪物仍然活着，它会进行攻击，对玩家造成随机伤害。如果玩家的生命值降至零，游戏将以“GAME OVER”（游戏结束）的消息告终。文章提供了实现这些机制的 C64 Basic 代码，将战斗系统无缝集成到现有的地牢探索中。

---

## 7. 科学与工程中的洞察力艺术 – 驾驭复杂性 (2014) [pdf]

**原文标题**: The Art of Insight in Science and Engineering – Mastering Complexity(2014) [pdf]

**原文链接**: [https://ocw.mit.edu/courses/res-6-011-the-art-of-insight-in-science-and-engineering-mastering-complexity-fall-2014/3bca850386a3005c22134fa62fb3bad5_MITRES_6-011F14_art_insfin.pdf](https://ocw.mit.edu/courses/res-6-011-the-art-of-insight-in-science-and-engineering-mastering-complexity-fall-2014/3bca850386a3005c22134fa62fb3bad5_MITRES_6-011F14_art_insfin.pdf)

现有内容由原始PDF元数据和压缩数据流组成，无法直接提取文章的可读文本。因此，本摘要仅依据文章标题：《科学与工程中的洞察力之艺术——驾驭复杂性》(2014)。

基于此标题，这篇发表于2014年的文章可能深入探讨了在科学和工程学科中发展和应用“洞察力”所需的方法论、认知过程和战略方法。它似乎侧重于这些领域的专业人士如何有效地解决和克服复杂问题。其中心主题表明，该文旨在探索高级问题解决技术，培养创新思维，以及培养能够带来突破的深刻理解。它将洞察力的产生定位为一种可以被磨练和掌握的“艺术”，而非偶然事件，旨在应对科学发现和工程设计中固有的复杂挑战，最终旨在为读者提供“驾驭复杂性”的工具。

---

## 8. 最大的概率计算机化噪声为答案

**原文标题**: Biggest Probabilistic Computer Turns Noise into Answers

**原文链接**: [https://spectrum.ieee.org/biggest-probabilistic-computer](https://spectrum.ieee.org/biggest-probabilistic-computer)

《计算新闻》报道了迄今为止最大的概率计算机的研制成功，该计算机拥有前所未有的100万个概率比特（p-bit）。据Charles Q. Choi详细介绍，这款新机器是通过将18个现场可编程门阵列（FPGA）连接起来制造而成的。在Navid Anjum Aadit和张秀琪等研究人员的带领下，这一技术进步有望解决目前传统数字计算机力所不及的极其困难的优化问题。这项创新标志着计算领域的重大进展，并有可能将固有的噪声转化为应对复杂挑战的计算答案。

---

## 9. A new Intel Itanium (IA-64) emulator that boots Windows

**原文标题**: A new Intel Itanium (IA-64) emulator that boots Windows

**原文链接**: [https://raymii.org/s/blog/Intel_Itanium_IA-64-Emulator_that_boots_Windows.html](https://raymii.org/s/blog/Intel_Itanium_IA-64-Emulator_that_boots_Windows.html)

生成摘要时出错

---

## 10. Harness Engineering

**原文标题**: Harness Engineering

**原文链接**: [https://github.com/lopopolo/harness-engineering](https://github.com/lopopolo/harness-engineering)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 2 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 3 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 4 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 5 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 6 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 7 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 8 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 9 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 10 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 11 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 12 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 13 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 14 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 15 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 16 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 17 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 18 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 19 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 20 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 21 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 22 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 23 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 24 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 25 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 26 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 27 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 28 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 29 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 30 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 31 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 32 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 33 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 34 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 35 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 36 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 37 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 38 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 39 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 40 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 41 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 42 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 43 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 44 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 45 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 46 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 47 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 48 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 49 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 50 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 51 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 52 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 53 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 54 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 55 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 56 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 57 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 58 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 59 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 60 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 61 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 62 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 63 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 64 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 65 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 66 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 67 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 68 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 69 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 70 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 71 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 72 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 73 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 74 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 75 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 76 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 77 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 78 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 79 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 80 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 81 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 82 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 83 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 84 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 85 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 86 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 87 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 88 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 89 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 90 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 91 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 92 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 93 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 94 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 95 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 96 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 97 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 98 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 99 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 100 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 101 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 102 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 103 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 104 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 105 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 106 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 107 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 108 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 109 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 110 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 111 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 112 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 113 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 114 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 115 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 116 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 117 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 118 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 119 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 120 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 121 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 122 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 123 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 124 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 125 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 126 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 127 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 128 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 129 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 130 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 131 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 132 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 133 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 134 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 135 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 136 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 137 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 138 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 139 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 140 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 141 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 142 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 143 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 144 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 145 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 146 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 147 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 148 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 149 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 150 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 151 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 152 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 153 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 154 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 155 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 156 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 157 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 158 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 159 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 160 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 161 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 162 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 163 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 164 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 165 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 166 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 167 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 168 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 169 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 170 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 171 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 172 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 173 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 174 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 175 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 176 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 177 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 178 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 179 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 180 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 181 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 182 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 183 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 184 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 185 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 186 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 187 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 188 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 189 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 190 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 191 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 192 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 193 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 194 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 195 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 196 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 197 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 198 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 199 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 200 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 201 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 202 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 203 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 204 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 205 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 206 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 207 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 208 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 209 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 210 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 211 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 212 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 213 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 214 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 215 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 216 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 217 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 218 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 219 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 220 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 221 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 222 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 223 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 224 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 225 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 226 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 227 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 228 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 229 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 230 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 231 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 232 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 233 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 234 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 235 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 236 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 237 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 238 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 239 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 240 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 241 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 242 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 243 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 244 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 245 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 246 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 247 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 248 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 249 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 250 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 251 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 252 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 253 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 254 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 255 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
