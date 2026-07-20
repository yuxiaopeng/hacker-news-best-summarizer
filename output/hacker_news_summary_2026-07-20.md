# Hacker News 热门文章摘要 (2026-07-20)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

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

## 11. DeKalb deputy charged with Flock camera misuse; more Georgia officers fired

**原文标题**: DeKalb deputy charged with Flock camera misuse; more Georgia officers fired

**原文链接**: [https://www.ajc.com/news/2026/07/3-more-georgia-police-officers-fired-over-alleged-flock-camera-misuse/](https://www.ajc.com/news/2026/07/3-more-georgia-police-officers-fired-over-alleged-flock-camera-misuse/)

生成摘要时出错

---

## 12. The Anti-Palantir Manifesto

**原文标题**: The Anti-Palantir Manifesto

**原文链接**: [https://nonogra.ph/the-anti-palantir-manifesto-07-20-2026](https://nonogra.ph/the-anti-palantir-manifesto-07-20-2026)

生成摘要时出错

---

## 13. Natural experiments prove phytoplankton carbon removal works

**原文标题**: Natural experiments prove phytoplankton carbon removal works

**原文链接**: [https://www.onepercentbrighter.com/p/natural-experiments-prove-feeding](https://www.onepercentbrighter.com/p/natural-experiments-prove-feeding)

生成摘要时出错

---

## 14. The Trump administration's Threat to Scientific Research

**原文标题**: The Trump administration's Threat to Scientific Research

**原文链接**: [https://marginalrevolution.com/marginalrevolution/2026/07/the-trump-administrations-threat-to-scientific-research.html](https://marginalrevolution.com/marginalrevolution/2026/07/the-trump-administrations-threat-to-scientific-research.html)

生成摘要时出错

---

## 15. Judge a book by its first pages

**原文标题**: Judge a book by its first pages

**原文链接**: [https://uncovered.ink](https://uncovered.ink)

生成摘要时出错

---

## 16. How to Abandon Your Climate Commitments and Get Away with It

**原文标题**: How to Abandon Your Climate Commitments and Get Away with It

**原文链接**: [https://www.nytimes.com/2026/07/17/climate/company-climate-change-commitments-renege.html](https://www.nytimes.com/2026/07/17/climate/company-climate-change-commitments-renege.html)

生成摘要时出错

---

## 17. Firefox 153.0 Beta

**原文标题**: Firefox 153.0 Beta

**原文链接**: [https://www.firefox.com/en-US/firefox/153.0beta/releasenotes/](https://www.firefox.com/en-US/firefox/153.0beta/releasenotes/)

生成摘要时出错

---

## 18. Scrying the AMD GFX1250 LLVM Tea Leaves

**原文标题**: Scrying the AMD GFX1250 LLVM Tea Leaves

**原文链接**: [https://chipsandcheese.com/p/scrying-the-amd-gfx1250-llvm-tea](https://chipsandcheese.com/p/scrying-the-amd-gfx1250-llvm-tea)

生成摘要时出错

---

## 19. Real-Time LuaTeX: Recompiling Large Documents in 1ms [pdf]

**原文标题**: Real-Time LuaTeX: Recompiling Large Documents in 1ms [pdf]

**原文链接**: [https://www.tug.org/tug2026/preprints/lode-realtime.pdf](https://www.tug.org/tug2026/preprints/lode-realtime.pdf)

生成摘要时出错

---

## 20. US gas prices hit an average of $4 a gallon again

**原文标题**: US gas prices hit an average of $4 a gallon again

**原文链接**: [https://apnews.com/article/gas-prices-iran-war-4-gallon-4b82825734ec3ded192351e53a4be69e](https://apnews.com/article/gas-prices-iran-war-4-gallon-4b82825734ec3ded192351e53a4be69e)

生成摘要时出错

---

## 21. I'm Done with Mullvad

**原文标题**: I'm Done with Mullvad

**原文链接**: [https://moonwriting.blog/i-m-done-with-mullvad](https://moonwriting.blog/i-m-done-with-mullvad)

生成摘要时出错

---

## 22. Codex is wearing out our devices

**原文标题**: Codex is wearing out our devices

**原文链接**: [https://old.reddit.com/r/codex/comments/1v0m3lt/codex_is_wearing_out_our_devices/](https://old.reddit.com/r/codex/comments/1v0m3lt/codex_is_wearing_out_our_devices/)

生成摘要时出错

---

## 23. Big tech is now targeting Native American land for data centers

**原文标题**: Big tech is now targeting Native American land for data centers

**原文链接**: [https://www.nytimes.com/2026/07/09/us/data-centers-native-american-tribes.html](https://www.nytimes.com/2026/07/09/us/data-centers-native-american-tribes.html)

生成摘要时出错

---

## 24. Nativ: Run frontier open models locally on your Mac

**原文标题**: Nativ: Run frontier open models locally on your Mac

**原文链接**: [https://blaizzy.github.io/nativ/](https://blaizzy.github.io/nativ/)

生成摘要时出错

---

## 25. Show HN: 一个基于画布的笔记和整理应用

**原文标题**: Show HN: A canvas-based note taking and organizer app

**原文链接**: [https://www.passinote.app/](https://www.passinote.app/)

生成摘要时出错

---

## 26. Deepsec

**原文标题**: Deepsec

**原文链接**: [https://github.com/vercel-labs/deepsec](https://github.com/vercel-labs/deepsec)

生成摘要时出错

---

## 27. Valve say there's no end in sight to the memory crisis, prices going to increase

**原文标题**: Valve say there's no end in sight to the memory crisis, prices going to increase

**原文链接**: [https://www.pcgamer.com/hardware/steam-machines/valve-says-theres-no-end-in-sight-to-the-memory-crisis-and-prices-are-only-going-to-increase-honestly-its-still-getting-worse/](https://www.pcgamer.com/hardware/steam-machines/valve-says-theres-no-end-in-sight-to-the-memory-crisis-and-prices-are-only-going-to-increase-honestly-its-still-getting-worse/)

生成摘要时出错

---

## 28. Google Is Censoring Reviews of ICE Detention Centers

**原文标题**: Google Is Censoring Reviews of ICE Detention Centers

**原文链接**: [https://theintercept.com/2026/07/20/google-maps-reviews-ice-detention-centers/](https://theintercept.com/2026/07/20/google-maps-reviews-ice-detention-centers/)

生成摘要时出错

---

## 29. Perforce charges $500 for training training videos.. and it's AI narrated

**原文标题**: Perforce charges $500 for training training videos.. and it's AI narrated

**原文链接**: [https://training.perforce.com/learn/courses/535/p4-helix-core-user-basic](https://training.perforce.com/learn/courses/535/p4-helix-core-user-basic)

生成摘要时出错

---

