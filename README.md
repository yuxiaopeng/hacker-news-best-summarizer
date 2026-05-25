# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-05-25.md)

*最后自动更新时间: 2026-05-25 20:48:13*
## 1. CBP 指令 3340-049B：电子设备边境搜查

**原文标题**: CBP Directive 3340-049B: Border Search of Electronic Devices

**原文链接**: [https://www.cbp.gov/document/directives/cbp-directive-no-3340-049b-border-search-electronic-devices](https://www.cbp.gov/document/directives/cbp-directive-no-3340-049b-border-search-electronic-devices)

CBP 指令 3340-049B，题为“电子设备边境搜查”，为美国海关及边境保护局 (CBP) 人员提供了全面的指导和标准操作程序。该指令涉及对存储在各类电子和数字设备中的信息进行搜查、审查、保留和共享。这包括电脑、平板电脑、手机、相机、音乐播放器，以及各种形式的可移动媒体和存储设备。

这些程序适用于由CBP执行的进出境边境搜查。该指令被归类为行政手册和政策指南，与问责制和透明度原则以及《信息自由法案》(FOIA) 相关。该指令本身的日期为2026年1月28日，并附有一份日期为2026年2月2日的分发备忘录。

---

## 2. 用树莓派构建树莓派

**原文标题**: Building Pi with Pi

**原文链接**: [https://lucumr.pocoo.org/2026/5/24/pi-oss/](https://lucumr.pocoo.org/2026/5/24/pi-oss/)

Armin Ronacher反思了使用“Pi”（一个AI代理，或称“笨重机器人”）开发“Pi”软件项目的情况，并指出了对开源项目带来的严峻挑战和深远影响。一个关键问题是“浮泛问题”：AI生成的bug报告常常自信地不准确，不必要地扩大范围，并被其他代理视为证据，从而误导它们。Ronacher倡导简洁的、由人类观察到的问题描述。

这种“浮泛”也延伸到了代码层面，AI模型经常通过添加针对不良状态的局部防御来过度设计解决方案，而不是强制全局不变量或从源头阻止不良数据，从而增加了复杂性。大量低质量的、由LLM（大型语言模型）辅助的贡献带来了巨大的维护负担，使问题追踪器不堪重负，并分散了精力。Ronacher强调，这种“浮泛”的责任在于人类使用者，而非平台。

尽管存在这些问题，“Pi”仍被用于特定任务，例如并行问题复现。自定义指令引导代理独立验证行为并进行分析，明确不信任已存在的“浮泛”内容。

最终，Ronacher认为，AI尽管增加了代码量和项目数量，却分散了开源工作，并鼓励孤立作业，从而破坏了开源的核心价值：人类协作、沟通以及共同解决难题，以构建强大、共享的基础。他强调，主导权在于人类，而非机器。

---

## 3. 以柔术克服Git严谨性疲劳

**原文标题**: Defeating Git Rigour Fatigue with Jujutsu

**原文链接**: [https://ikesau.co/blog/defeating-git-rigour-fatigue-with-jujutsu/](https://ikesau.co/blog/defeating-git-rigour-fatigue-with-jujutsu/)

本文探讨了“Git严谨性疲劳”，即在复杂功能开发过程中，难以维护干净、连续的提交历史（例如，“定义类型”、“添加数据库函数”）的问题。通常，提交会变成修复、测试代码和零散改动的混杂“混乱”，打破了预期的叙述性。尽管Jujutsu提供了`jj absorb`和`jj squash -i`等工具，但它们仍有局限性，例如更改分配不正确或存在合并冲突问题。

作者提出了一种新的Jujutsu技术来解决此问题。该技术首先创建了一个理想的、空的提交历史。然后，将所有实际开发更改合并到一个“所有改动提交”中。最后，开发人员通过交互方式将特定的更改从这个“所有改动提交”合并到预定义的干净提交中，从而有效地将“一堆待洗衣服”分拣到正确的概念箱中，直到“所有改动提交”为空。

这种方法允许进行灵活的、即兴的开发，其中可以包含临时调试代码，并将严格的清理工作推迟到最后。它被认为优于`jj split`，因为它更容易对改动块进行排序，并且避免了增量`jj squash -i`操作可能引起的合并冲突，因为最终的“所有改动提交”状态确保了无冲突的分发。一个主要的缺点是中间提交可能不总是能编译通过。

---

## 4. 教宗良：少数公司掌控的不透明人工智能恐致“新形式非人化”

**原文标题**: Pope Leo: opaque AI run by few firms risks "New Forms of Dehumanization"

**原文链接**: [https://variety.com/2026/biz/global/pope-leo-ai-encyclical-algorithms-threaten-dehumanisation-1236758186/](https://variety.com/2026/biz/global/pope-leo-ai-encyclical-algorithms-threaten-dehumanisation-1236758186/)

教皇利奥发布了一份重要的AI宣言《壮丽的人性》，警告称“少数强大的私人公司”控制的“不透明算法”有导致“新形式的非人化”的风险。教宗采取了不寻常的举动，亲自在梵蒂冈与主要人工智能开发商Anthropic的创始人克里斯托弗·奥拉一起发布了这份通谕。

教皇利奥强调，人工智能绝不能“掌握在少数人手中”，他提到其最近在美国-以色列对伊朗的战争中的应用，并警告不要让技术革命被“对利润的盲目崇拜”所驱动。他阐明，尽管技术本身并非“邪恶”，但它绝不是中立的，它反映了其创造者和使用者的特点。

他呼吁“更积极的政治参与”以减缓快速发展，主张建立“健全的法律框架、独立的监督、知情用户以及一个不推卸责任的政治体系”。这份通谕包含J.R.R.托尔金关于共同责任的一段引文。曾与宗教团体接触的Anthropic公司此前曾拒绝五角大楼无限制使用其人工智能助手Claude的要求。

---

## 5. 籽油恐慌正在伤害我的心脏病患者。

**原文标题**: The seed oil panic is hurting my cardiac patients

**原文链接**: [https://www.statnews.com/2026/05/22/seed-oils-healthy-fats-tallow-fact-check-cardiac-health/](https://www.statnews.com/2026/05/22/seed-oils-healthy-fats-tallow-fact-check-cardiac-health/)

所提供的文本描述了于2026年5月23日发布的“第一观点播客”的一集。该集的主题具体标题为“围绝经期运动如何伤害女性”。

值得注意的是，为本文提供的主标题“籽油恐慌正在伤害我的心脏病患者”与描述这一特定播客剧集的内容不符。所提供的内容专门详细介绍了关于围绝经期的播客剧集。

---

## 6. 精通 Dyalog APL

**原文标题**: Mastering Dyalog APL

**原文链接**: [https://mastering.dyalog.com/README.html](https://mastering.dyalog.com/README.html)

《精通Dyalog APL》一书是学习Dyalog APL的主要资源。该书第一版由Bernard Legrand于2009年11月撰写，但随着Dyalog APL的发展和技术的快速变化，该版本正变得过时。

为解决此问题，目前由Rodrigo Girão Serrão牵头，正在进行一次更新且更现代的修订工作。这个新版本正使用Jupyter Notebooks创建，旨在提供交互式学习体验，目前已有一个静态在线版本可用，并计划推出印刷版。此次修订更新并重写了原版中的散文和示例，同时还增加了新的章节，以涵盖Dyalog APL 12.0（2009年）以来引入的新功能。

在线版本明确声明仍在开发中，存在内容缺失和大幅修订的可能性。我们鼓励读者通过GitHub issues或发送邮件至mdapl@dyalog.com提供反馈、提出修改建议或报告错别字。提供了变更日志，供读者查阅此次修订与原始版本之间的差异。

---

## 7. 微软叫停在喀里多尼亚建设244英亩数据中心的计划 (2025年)

**原文标题**: Microsoft pulls plug on plans for 244-acre data center in Caledonia (2025)

**原文链接**: [https://www.tmj4.com/news/racine-county/microsoft-pulls-plug-on-plans-for-244-acre-data-center-in-caledonia-after-community-pushback](https://www.tmj4.com/news/racine-county/microsoft-pulls-plug-on-plans-for-244-acre-data-center-in-caledonia-after-community-pushback)

微软已正式撤回在威斯康星州卡利多尼亚村建设一个244英亩数据中心的计划，理由是遭到社区的强烈反对。这家科技巨头的决定是由于广泛的反对声浪，其中包括数百名居民表达担忧，以及超过2000人签署请愿书，反对将该地块（位于县界路和32号州道交界处，毗邻住宅和农田）重新规划用途。

尽管放弃了这一特定地点，微软仍重申其继续投资威斯康星州东南部的兴趣。该公司表示，打算与卡利多尼亚和拉辛县的领导人合作，以确定一个既符合社区优先事项又符合其发展目标的替代地点。

普雷斯科特·巴尔奇等居民对这一消息表示欢迎，称这是卡利多尼亚的“伟大一天”，认为他们的论点成功地说服了这家公司。村受托人南希·皮尔斯也尊重微软倾听民众反馈的决定。巴尔奇和皮尔斯都表示，他们未来对与微软合作持开放态度，并建议任何后续提案的关键在于更早、更直接的社区参与。村行政官托德·威利斯指出，村里尚未收到任何正式的撤回文件。

---

## 8. Don't Roll Your Own

**原文标题**: Don't Roll Your Own

**原文链接**: [https://susam.net/do-not-roll-your-own.html](https://susam.net/do-not-roll-your-own.html)

生成摘要时出错

---

## 9. Alexander Grothendieck Revolutionized 20th-Century Mathematics

**原文标题**: Alexander Grothendieck Revolutionized 20th-Century Mathematics

**原文链接**: [https://www.quantamagazine.org/how-alexander-grothendieck-revolutionized-20th-century-mathematics-20260520/](https://www.quantamagazine.org/how-alexander-grothendieck-revolutionized-20th-century-mathematics-20260520/)

生成摘要时出错

---

## 10. The C64 Dead Test Font

**原文标题**: The C64 Dead Test Font

**原文链接**: [https://www.masswerk.at/nowgobang/2026/c64-dead-test-font](https://www.masswerk.at/nowgobang/2026/c64-dead-test-font)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 2 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 3 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 4 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 5 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 6 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 7 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 8 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 9 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 10 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 11 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 12 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 13 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 14 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 15 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 16 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 17 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 18 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 19 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 20 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 21 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 22 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 23 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 24 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 25 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 26 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 27 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 28 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 29 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 30 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 31 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 32 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 33 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 34 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 35 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 36 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 37 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 38 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 39 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 40 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 41 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 42 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 43 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 44 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 45 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 46 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 47 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 48 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 49 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 50 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 51 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 52 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 53 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 54 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 55 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 56 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 57 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 58 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 59 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 60 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 61 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 62 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 63 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 64 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 65 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 66 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 67 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 68 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 69 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 70 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 71 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 72 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 73 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 74 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 75 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 76 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 77 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 78 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 79 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 80 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 81 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 82 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 83 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 84 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 85 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 86 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 87 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 88 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 89 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 90 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 91 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 92 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 93 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 94 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 95 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 96 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 97 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 98 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 99 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 100 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 101 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 102 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 103 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 104 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 105 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 106 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 107 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 108 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 109 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 110 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 111 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 112 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 113 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 114 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 115 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 116 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 117 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 118 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 119 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 120 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 121 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 122 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 123 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 124 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 125 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 126 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 127 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 128 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 129 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 130 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 131 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 132 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 133 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 134 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 135 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 136 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 137 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 138 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 139 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 140 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 141 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 142 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 143 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 144 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 145 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 146 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 147 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 148 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 149 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 150 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 151 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 152 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 153 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 154 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 155 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 156 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 157 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 158 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 159 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 160 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 161 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 162 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 163 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 164 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 165 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 166 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 167 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 168 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 169 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 170 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 171 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 172 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 173 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 174 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 175 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 176 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 177 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 178 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 179 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 180 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 181 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 182 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 183 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 184 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 185 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 186 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 187 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 188 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 189 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 190 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 191 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 192 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 193 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 194 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 195 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 196 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 197 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 198 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 199 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
