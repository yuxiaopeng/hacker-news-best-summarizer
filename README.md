# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-11-22.md)

*最后自动更新时间: 2026-11-22 00:08:00*
## 1. 莱文特·阿尔珀热声称证明了广义黎曼猜想。

**原文标题**: Levent Alpöge claims proof of the Generalized Riemann Hypothesis [pdf]

**原文链接**: [https://alpo.ge/remark.pdf](https://alpo.ge/remark.pdf)

所提供的“内容”是来自PDF文件的原始压缩数据，并非人类可读的文本。因此，无法阅读或总结其内容。

标题“Levent Alpöge claims proof of the Generalized Riemann Hypothesis [pdf]”表明该文档可能讨论了Levent Alpöge声称的广义黎曼假设的证明。然而，如果无法访问PDF的解码和渲染文本，就无法提取或总结有关该证明、其方法论或文档中提出的主张的任何细节。

---

## 2. 紧急通知：亚历山德罗·马苏洛 GRH

**原文标题**: Hurried Announcement: Alessandro Masullo GRH

**原文链接**: [https://math216.wordpress.com/2026/11/20/hurried-announcement-alessandro-masullo-grh/](https://math216.wordpress.com/2026/11/20/hurried-announcement-alessandro-masullo-grh/)

2026年11月20日，ravivakil就Alessandro Maria Masullo提出的广义黎曼猜想（GRH）证明，发表了一份“仓促的公告”。作者当时正出席美国数学学会会议，他感到有必要立即发布当前草稿，这偏离了原定一年协作完善的计划。数学家Brian Conrad数月来一直在密切审查Masullo这份由人工生成的证明，提供了大量反馈，并认为它“看起来不错”。作者对Conrad的评估表示强烈信心，并敦促数学界迅速审查、将其形式化，并解决证明中的任何潜在不足。

然而，大约八小时后的一份更新披露，有数人报告了所提出的证明存在问题，这些问题是在各种AI模型的协助下发现的。作者澄清，按照惯例，所有问题都必须得到社区的满意解决，证明才能被接受。作者还声明，他们不对该证明策略的正确性作任何断言。原始帖子中附带了一个名为“The Music Of The PrimesDownload”的文件。

---

## 3. Inkling 2 Mini

**原文标题**: Inkling 2 Mini

**原文链接**: [https://thinkingmachines.ai/news/inkling-2-mini/](https://thinkingmachines.ai/news/inkling-2-mini/)

Inkling 2 Mini 是一款新发布、快速且强大的AI模型，旨在消费级笔记本电脑上高效运行。其核心创新是一种“循环Transformer”架构，该架构中模型的中间层每处理一个token就会被处理三次。这提升了推理质量，尤其是在智能体编码任务中，并通过允许更深层次的推理而无需冗长的思维链，从而提高了可监控性。

Inkling 2 Mini 总参数量为264亿（活跃参数34亿），在DeepSWE v1.1 (48.2%) 和 Vals Index v2.2 (46.5%) 等基准测试中，领先参数量低于千亿的开源模型，在速度上常超越同等规模的模型。其小巧的内存占用（约20GB）使其能够在MacBook Pro等设备上离线运行，这已通过构建飞行模拟器和驱动20个智能体城镇模拟得到验证。

该模型擅长长期智能体工作、编码以及工具增强知识任务（例如BrowseComp, DeepSearchQA），它通过有效利用搜索来弥补事实性知识空白，而非仅仅依赖增加参数数量。其效率通过0.703的高“每焦耳智能”分数得以体现。

Inkling 2 Mini 已在Tinker平台上提供开源权重，用于推理和定制。尽管它在推理和智能体任务方面表现出色，但在多轮聊天或高度受限的指令方面，它仍落后于某些模型。

---

## 4. 我再也不会买 Framework 硬件了。

**原文标题**: I'll never buy Framework hardware again

**原文链接**: [https://poolp.org/posts/2026-11-20/ill-never-buy-framework-hardware-again/](https://poolp.org/posts/2026-11-20/ill-never-buy-framework-hardware-again/)

这篇文章，标题为“我再也不会购买Framework硬件了”，表达了作者对Framework的强烈不满。作者无意过度损害该公司，但要求Framework解决其支持问题，并为客户提供能正常工作的笔记本电脑，这暗示他们收到了有缺陷的设备。该文章在Hacker News上被推荐后获得了广泛关注。

值得注意的是，所提供的文章极少具体说明Framework硬件或其支持方面遇到的问题。相反，文章的很大一部分是作者呼吁读者支持的内容——鼓励在社交网络上分享，并通过GitHub Sponsors或Patreon寻求资金捐助，以资助新的文章和项目。作者还通过aljuna.tech推广其咨询服务（架构审查、技术尽职调查和邮件基础设施）。

---

## 5. 黎曼猜想的 Lean 形式化验证

**原文标题**: Lean verification of the Riemann Hypothesis

**原文链接**: [https://leanprover-community.github.io/blog/posts/riemann-hypothesis/](https://leanprover-community.github.io/blog/posts/riemann-hypothesis/)

2026年11月20日，Levent Alpöge 发布了一个包含黎曼猜想证明的1700万行Lean代码库。得到Lean FRO和Mathlib Initiative认可的Lean和Mathlib社区，已联合验证并对该证明的正确性表示完全确信。

验证过程满足了四个严格标准。首先，作为Mathlib现有部分的黎曼猜想陈述，被确认为正确并经过专家审查。其次，Alpöge的代码库在多人编译时均成功通过且无错误，并始终生成相同的原始证明导出文件。第三，独立的比较工具证实，Alpöge证明的定理与Mathlib官方审查通过的黎曼猜想陈述精确匹配。最后，Lean证明的有效性受到了多个证明检查器的严格检验，其中包括Lean的官方内核、经过形式化证明正确的con-leche和con-ron检查器，以及多个独立的第三方工具。这些检查是在证明的惰性导出文件上进行的，以确保鲁棒性。

随着所有标准均已满足，各社区证明了该陈述和证明的正确性。向贡献者表达了感谢，并期待数学界能够探索这项重大成就中的新思想。

---

## 6. 如果你无法简单地解释一件事，就说明你还没有真正理解它。(2017)

**原文标题**: If you can't explain something in simple terms, you don't understand it (2017)

**原文链接**: [https://kottke.org/17/06/if-you-cant-explain-something-in-simple-terms-you-dont-understand-it](https://kottke.org/17/06/if-you-cant-explain-something-in-simple-terms-you-dont-understand-it)

文章《如果你无法用简单的语言解释某事，那你就不懂它》围绕着物理学家理查德·费曼的一个深刻信念展开：真正理解的标志在于能够将复杂思想简化的能力。一个关键的轶事描述了费曼曾试图为新生讲座简化解释为何自旋为半整数的粒子遵循费米-狄拉克统计。他最终失败了，并总结道：“这意味着我们并没有真正理解它。”

这种哲学超越了物理学范畴。约翰·格鲁伯指出，苹果公司也同样期望工程师们能简单地解释复杂技术，这不仅是为了高管，更是作为他们透彻理解的证明。费曼因其对火或磁铁等概念通俗易懂的解释而备受赞誉。关键的是，他对自己的知识局限也保持谦逊，承认无法用更简单的语言解释磁力，因为他自己也不以那种方式理解它。尽管他因解释量子力学而获得了诺贝尔奖，但他却有名地宣称：“没有人真正理解量子力学。”他毕生对深刻理解的追求体现在他最后的黑板笔记上：“我不能创造的，我就不理解。”

---

## 7. 霜咬：一种新型CPU架构，由AI发现、设计并验证

**原文标题**: Frostbite: A new CPU architecture discovered, designed and verified by AI

**原文链接**: [https://architectlabs.com/blog/frostbite](https://architectlabs.com/blog/frostbite)

Frostbite是一种新颖的通用CPU架构，完全由AI系统设计和验证，相较于现代超标量CPU，实现了4.59倍的每瓦性能提升。它解决了CPU性能停滞不前以及传统架构的局限性，后者在处理隐藏依赖、共享可变状态和复杂缓存一致性方面面临挑战。

Frostbite的基石是交互网，这是一种计算模型，其中程序是图，计算是局部重写，且每个值只有一个所有者。这种方法提供了固有的并行性，消除了对复杂多线程机制的需求，并使数据能够驻留在小型本地内存中，从而减少了大型缓存子系统在功耗和面积上的开销。

AI系统自主迭代了整个设计堆栈：编译器、指令集架构（ISA）、架构、微架构、寄存器传输级（RTL）、验证以及版图数据（GDS）。它们采用了一种新的形式化规约语言ASL和代理群，用于快速探索、跨堆栈优化和形式化验证。这一过程带来了新颖的架构原语和运行时特性的发现，包括用于并行网络交互的动态操作，以及在独立处理单元之间一种优雅的分布式工作窃取机制。

Frostbite展示了AI推动根本性架构变革的能力，证明了在每瓦性能和每面积性能上的显著提升，对未来所有类别的芯片设计具有广泛的影响。

---

## 8. 史洛普斯特拉普 – 让你的网站看起来像是仓促随性编写的

**原文标题**: Slopstrap – Make your site look hastily vibecoded

**原文链接**: [https://slopstrap.mikelacher.com/](https://slopstrap.mikelacher.com/)

文章介绍了 Slopstrap，一个旨在让网站呈现出“仓促编程”风格的工具。它概述了该服务的周末运营时间，并指出周六的开放时间为上午8点至下午4点。此外，Slopstrap 为紧急关停请求提供24小时支持。

---

## 9. 我们没有通知他们，就将开发者晋升为架构师。

**原文标题**: We promoted developers into architects without informing them

**原文链接**: [https://manidoraisamy.com/developer-to-architect.html](https://manidoraisamy.com/developer-to-architect.html)

生成摘要时出错

---

## 10. Restricting AI agents in mobile operating systems platforms from capturing data

**原文标题**: Restricting AI agents in mobile operating systems platforms from capturing data

**原文链接**: [https://signal.org/blog/protecting-your-privacy/](https://signal.org/blog/protecting-your-privacy/)

Signal is taking stringent measures to protect user privacy from AI agents integrated into mobile operating systems, following a similar move against Microsoft Recall on Windows. With Google and Apple integrating "agentic capabilities" like Gemini Intelligence and Siri AI deep into iOS 27 and Android, these systems can "scan" screens, capturing sensitive Signal data and making it available to their local or remote servers.

Signal states this undermines their long-standing privacy guarantees and poses an "existential threat" to their mission. To counter this, Signal is blocking screen capture by preventing screenshots on iOS 27 and automatically enabling "Screen security" on Android when AI assistants attempt to access the screen. While users can disable this protection, doing so risks exposing their conversations to AI agents.

The company highlights significant challenges: a lack of robust tools for developers to prevent AI data access without impacting user experience, and insufficient documentation from OS providers on how these AI agents function. Signal is calling on Apple, Google, and Microsoft to provide:
1.  Easy, well-documented methods for apps to opt out of AI data access (screen reading, filesystem, APIs).
2.  Clear technical specifications and documentation on AI agent functionality and data processing.

Signal warns that without these remedies, the current integration of AI agents represents an existential threat to application-layer privacy, affecting the entire ecosystem. They are engaging with OS providers, hopeful for standardized approaches to protect privacy.

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-11-22](output/hacker_news_summary_2026-11-22.md) |
| 2 | [2026-11-21](output/hacker_news_summary_2026-11-21.md) |
| 3 | [2026-11-20](output/hacker_news_summary_2026-11-20.md) |
| 4 | [2026-11-19](output/hacker_news_summary_2026-11-19.md) |
| 5 | [2026-11-14](output/hacker_news_summary_2026-11-14.md) |
| 6 | [2026-11-15](output/hacker_news_summary_2026-11-15.md) |
| 7 | [2026-11-18](output/hacker_news_summary_2026-11-18.md) |
| 8 | [2026-11-13](output/hacker_news_summary_2026-11-13.md) |
| 9 | [2026-11-17](output/hacker_news_summary_2026-11-17.md) |
| 10 | [2026-11-07](output/hacker_news_summary_2026-11-07.md) |
| 11 | [2026-11-06](output/hacker_news_summary_2026-11-06.md) |
| 12 | [2026-11-11](output/hacker_news_summary_2026-11-11.md) |
| 13 | [2026-11-08](output/hacker_news_summary_2026-11-08.md) |
| 14 | [2026-11-05](output/hacker_news_summary_2026-11-05.md) |
| 15 | [2026-11-12](output/hacker_news_summary_2026-11-12.md) |
| 16 | [2026-11-10](output/hacker_news_summary_2026-11-10.md) |
| 17 | [2026-11-01](output/hacker_news_summary_2026-11-01.md) |
| 18 | [2026-10-27](output/hacker_news_summary_2026-10-27.md) |
| 19 | [2026-11-03](output/hacker_news_summary_2026-11-03.md) |
| 20 | [2026-10-28](output/hacker_news_summary_2026-10-28.md) |
| 21 | [2026-10-29](output/hacker_news_summary_2026-10-29.md) |
| 22 | [2026-10-31](output/hacker_news_summary_2026-10-31.md) |
| 23 | [2026-10-30](output/hacker_news_summary_2026-10-30.md) |
| 24 | [2026-11-04](output/hacker_news_summary_2026-11-04.md) |
| 25 | [2026-10-24](output/hacker_news_summary_2026-10-24.md) |
| 26 | [2026-10-23](output/hacker_news_summary_2026-10-23.md) |
| 27 | [2026-10-25](output/hacker_news_summary_2026-10-25.md) |
| 28 | [2026-10-21](output/hacker_news_summary_2026-10-21.md) |
| 29 | [2026-10-22](output/hacker_news_summary_2026-10-22.md) |
| 30 | [2026-10-20](output/hacker_news_summary_2026-10-20.md) |
| 31 | [2026-10-26](output/hacker_news_summary_2026-10-26.md) |
| 32 | [2026-10-19](output/hacker_news_summary_2026-10-19.md) |
| 33 | [2026-10-18](output/hacker_news_summary_2026-10-18.md) |
| 34 | [2026-10-17](output/hacker_news_summary_2026-10-17.md) |
| 35 | [2026-10-15](output/hacker_news_summary_2026-10-15.md) |
| 36 | [2026-10-14](output/hacker_news_summary_2026-10-14.md) |
| 37 | [2026-10-16](output/hacker_news_summary_2026-10-16.md) |
| 38 | [2026-10-13](output/hacker_news_summary_2026-10-13.md) |
| 39 | [2026-10-09](output/hacker_news_summary_2026-10-09.md) |
| 40 | [2026-10-11](output/hacker_news_summary_2026-10-11.md) |
| 41 | [2026-10-07](output/hacker_news_summary_2026-10-07.md) |
| 42 | [2026-10-10](output/hacker_news_summary_2026-10-10.md) |
| 43 | [2026-10-06](output/hacker_news_summary_2026-10-06.md) |
| 44 | [2026-10-04](output/hacker_news_summary_2026-10-04.md) |
| 45 | [2026-10-03](output/hacker_news_summary_2026-10-03.md) |
| 46 | [2026-10-02](output/hacker_news_summary_2026-10-02.md) |
| 47 | [2026-09-29](output/hacker_news_summary_2026-09-29.md) |
| 48 | [2026-09-30](output/hacker_news_summary_2026-09-30.md) |
| 49 | [2026-09-25](output/hacker_news_summary_2026-09-25.md) |
| 50 | [2026-09-27](output/hacker_news_summary_2026-09-27.md) |
| 51 | [2026-10-01](output/hacker_news_summary_2026-10-01.md) |
| 52 | [2026-09-24](output/hacker_news_summary_2026-09-24.md) |
| 53 | [2026-09-21](output/hacker_news_summary_2026-09-21.md) |
| 54 | [2026-09-18](output/hacker_news_summary_2026-09-18.md) |
| 55 | [2026-09-23](output/hacker_news_summary_2026-09-23.md) |
| 56 | [2026-09-20](output/hacker_news_summary_2026-09-20.md) |
| 57 | [2026-09-19](output/hacker_news_summary_2026-09-19.md) |
| 58 | [2026-09-22](output/hacker_news_summary_2026-09-22.md) |
| 59 | [2026-09-12](output/hacker_news_summary_2026-09-12.md) |
| 60 | [2026-09-13](output/hacker_news_summary_2026-09-13.md) |
| 61 | [2026-09-11](output/hacker_news_summary_2026-09-11.md) |
| 62 | [2026-09-14](output/hacker_news_summary_2026-09-14.md) |
| 63 | [2026-09-17](output/hacker_news_summary_2026-09-17.md) |
| 64 | [2026-09-16](output/hacker_news_summary_2026-09-16.md) |
| 65 | [2026-09-15](output/hacker_news_summary_2026-09-15.md) |
| 66 | [2026-09-05](output/hacker_news_summary_2026-09-05.md) |
| 67 | [2026-09-02](output/hacker_news_summary_2026-09-02.md) |
| 68 | [2026-09-06](output/hacker_news_summary_2026-09-06.md) |
| 69 | [2026-09-03](output/hacker_news_summary_2026-09-03.md) |
| 70 | [2026-09-08](output/hacker_news_summary_2026-09-08.md) |
| 71 | [2026-09-07](output/hacker_news_summary_2026-09-07.md) |
| 72 | [2026-09-04](output/hacker_news_summary_2026-09-04.md) |
| 73 | [2026-09-09](output/hacker_news_summary_2026-09-09.md) |
| 74 | [2026-09-10](output/hacker_news_summary_2026-09-10.md) |
| 75 | [2026-08-29](output/hacker_news_summary_2026-08-29.md) |
| 76 | [2026-09-01](output/hacker_news_summary_2026-09-01.md) |
| 77 | [2026-08-25](output/hacker_news_summary_2026-08-25.md) |
| 78 | [2026-08-30](output/hacker_news_summary_2026-08-30.md) |
| 79 | [2026-08-26](output/hacker_news_summary_2026-08-26.md) |
| 80 | [2026-08-31](output/hacker_news_summary_2026-08-31.md) |
| 81 | [2026-08-28](output/hacker_news_summary_2026-08-28.md) |
| 82 | [2026-08-20](output/hacker_news_summary_2026-08-20.md) |
| 83 | [2026-08-16](output/hacker_news_summary_2026-08-16.md) |
| 84 | [2026-08-22](output/hacker_news_summary_2026-08-22.md) |
| 85 | [2026-08-24](output/hacker_news_summary_2026-08-24.md) |
| 86 | [2026-08-18](output/hacker_news_summary_2026-08-18.md) |
| 87 | [2026-08-17](output/hacker_news_summary_2026-08-17.md) |
| 88 | [2026-08-15](output/hacker_news_summary_2026-08-15.md) |
| 89 | [2026-08-21](output/hacker_news_summary_2026-08-21.md) |
| 90 | [2026-08-23](output/hacker_news_summary_2026-08-23.md) |
| 91 | [2026-08-14](output/hacker_news_summary_2026-08-14.md) |
| 92 | [2026-08-19](output/hacker_news_summary_2026-08-19.md) |
| 93 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 94 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 95 | [2026-08-11](output/hacker_news_summary_2026-08-11.md) |
| 96 | [2026-08-10](output/hacker_news_summary_2026-08-10.md) |
| 97 | [2026-08-12](output/hacker_news_summary_2026-08-12.md) |
| 98 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 99 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 100 | [2026-08-09](output/hacker_news_summary_2026-08-09.md) |
| 101 | [2026-08-13](output/hacker_news_summary_2026-08-13.md) |
| 102 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 103 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 104 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 105 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 106 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 107 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 108 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 109 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 110 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 111 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 112 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 113 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 114 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 115 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 116 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 117 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 118 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 119 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 120 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 121 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 122 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 123 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 124 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 125 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 126 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 127 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 128 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 129 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 130 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 131 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 132 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 133 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 134 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 135 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 136 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 137 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 138 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 139 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 140 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 141 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 142 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 143 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 144 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 145 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 146 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 147 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 148 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 149 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 150 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 151 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 152 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 153 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 154 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 155 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 156 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 157 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 158 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 159 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 160 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 161 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 162 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 163 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 164 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 165 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 166 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 167 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 168 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 169 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 170 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 171 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 172 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 173 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 174 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 175 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 176 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 177 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 178 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 179 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 180 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 181 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 182 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 183 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 184 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 185 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 186 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 187 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 188 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 189 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 190 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 191 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 192 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 193 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 194 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 195 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 196 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 197 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 198 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 199 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 200 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 201 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 202 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 203 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 204 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 205 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 206 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 207 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 208 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 209 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 210 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 211 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 212 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 213 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 214 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 215 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 216 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 217 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 218 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 219 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 220 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 221 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 222 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 223 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 224 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 225 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 226 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 227 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 228 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 229 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 230 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 231 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 232 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 233 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 234 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 235 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 236 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 237 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 238 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 239 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 240 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 241 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 242 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 243 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 244 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 245 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 246 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 247 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 248 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 249 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 250 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 251 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 252 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 253 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 254 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 255 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 256 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 257 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 258 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 259 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 260 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 261 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 262 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 263 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 264 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 265 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 266 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 267 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 268 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 269 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 270 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 271 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 272 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 273 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 274 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 275 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 276 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 277 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 278 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 279 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 280 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 281 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 282 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 283 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 284 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 285 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 286 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 287 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 288 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 289 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 290 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 291 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 292 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 293 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 294 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 295 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 296 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 297 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 298 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 299 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 300 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 301 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 302 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 303 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 304 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 305 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 306 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 307 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 308 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 309 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 310 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 311 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 312 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 313 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 314 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 315 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 316 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 317 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 318 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 319 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 320 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 321 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 322 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 323 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 324 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 325 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 326 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 327 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 328 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 329 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 330 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 331 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 332 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 333 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 334 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 335 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 336 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 337 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 338 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 339 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 340 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 341 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 342 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 343 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 344 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 345 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 346 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 347 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 348 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 349 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 350 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 351 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 352 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 353 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 354 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 355 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 356 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 357 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 358 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 359 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 360 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 361 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 362 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 363 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 364 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 365 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
| 366 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 367 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 368 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 369 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 370 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
