# Hacker News 热门文章摘要 (2026-05-25)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

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

## 11. Ruby for Good

**原文标题**: Ruby for Good

**原文链接**: [https://ti.to/codeforgood/rubyforgood](https://ti.to/codeforgood/rubyforgood)

生成摘要时出错

---

## 12. Exit IP VPN servers mitigation rollout

**原文标题**: Exit IP VPN servers mitigation rollout

**原文链接**: [https://mullvad.net/en/help/exit-ip-vpn-servers-mitigation-rollout](https://mullvad.net/en/help/exit-ip-vpn-servers-mitigation-rollout)

生成摘要时出错

---

## 13. Air France and Airbus found guilty of manslaughter over 2009 plane crash

**原文标题**: Air France and Airbus found guilty of manslaughter over 2009 plane crash

**原文链接**: [https://www.bbc.com/news/articles/czd2qmdvmq6o](https://www.bbc.com/news/articles/czd2qmdvmq6o)

生成摘要时出错

---

## 14. My I3-Emacs Integration

**原文标题**: My I3-Emacs Integration

**原文链接**: [https://khz.ac/software/i3-integration.html](https://khz.ac/software/i3-integration.html)

生成摘要时出错

---

## 15. Justice Department scrubs its website of news releases about Jan. 6 defendants

**原文标题**: Justice Department scrubs its website of news releases about Jan. 6 defendants

**原文链接**: [https://apnews.com/article/justice-department-capitol-riot-news-releases-purged-29c580044a9ed27b643c99feac9e2964](https://apnews.com/article/justice-department-capitol-riot-news-releases-purged-29c580044a9ed27b643c99feac9e2964)

生成摘要时出错

---

## 16. Perceptual Image Codec: What Matters in Practical Learned Image Compression

**原文标题**: Perceptual Image Codec: What Matters in Practical Learned Image Compression

**原文链接**: [https://apple.github.io/ml-pico/](https://apple.github.io/ml-pico/)

生成摘要时出错

---

## 17. Rising seas will swallow New Orleans. People need to start relocating now

**原文标题**: Rising seas will swallow New Orleans. People need to start relocating now

**原文链接**: [https://www.cnn.com/2026/05/25/climate/new-orleans-sea-level-rise-relocation](https://www.cnn.com/2026/05/25/climate/new-orleans-sea-level-rise-relocation)

生成摘要时出错

---

## 18. IBM Spins Off the First Pure-Play Quantum Chip Foundry

**原文标题**: IBM Spins Off the First Pure-Play Quantum Chip Foundry

**原文链接**: [https://futurumgroup.com/insights/2-billion-chips-act-investment-in-quantum-bets-on-ibms-300mm-superconducting-silicon/](https://futurumgroup.com/insights/2-billion-chips-act-investment-in-quantum-bets-on-ibms-300mm-superconducting-silicon/)

生成摘要时出错

---

## 19. 'Fuck you, Bambu': How one private message could change the face of 3D printing

**原文标题**: 'Fuck you, Bambu': How one private message could change the face of 3D printing

**原文链接**: [https://www.theverge.com/tech/931532/bambu-agpl-pawel-jarczak-open-source-threat-dmca-github](https://www.theverge.com/tech/931532/bambu-agpl-pawel-jarczak-open-source-threat-dmca-github)

Bambu Lab, a prominent 3D printer company, is facing intense backlash after privately threatening developer Paweł Jarczak. Jarczak created open-source code that enabled users to remote control Bambu printers without proprietary software and support third-party accessories, bypassing Bambu's authentication. Bambu demanded he remove his code, implying legal action under the DMCA and citing security concerns. Jarczak complied but publicly revealed Bambu's aggressive tactics.

This sparked a furious response from the open-source 3D printing community. Influential figures like Louis Rossmann and GamersNexus pledged financial support for Jarczak, announced boycotts, and began "forking" Bambu's code. The Software Freedom Conservancy joined, accusing Bambu of violating the AGPL open-source license, under which Bambu Studio is built. They argue Bambu's proprietary networking plug-in, despite intimate communication with its open-source components, is not being shared as "Corresponding Source" as required by the license.

Bambu defends its actions, stating the networking plug-in is a "separately delivered, optional networking component" not covered by AGPL and citing security threats like DDoS attacks. Legal experts note that the AGPL's application to cloud services and plug-ins is complex and largely untested in court. While Bambu raises valid security points, critics contend the company could implement proper security without suppressing open-source innovation, making Jarczak an unwitting martyr in a larger battle over the future of open hardware and software ecosystems.

---

## 20. C extensions, portability, and alternative compilers

**原文标题**: C extensions, portability, and alternative compilers

**原文链接**: [https://lemon.rip/w/6-c-extensions-compilers/](https://lemon.rip/w/6-c-extensions-compilers/)

生成摘要时出错

---

## 21. The bootstrapper's EU stack for under €10 per month

**原文标题**: The bootstrapper's EU stack for under €10 per month

**原文链接**: [https://eualternative.eu/guides/bootstrapper-free-tier-eu-stack/](https://eualternative.eu/guides/bootstrapper-free-tier-eu-stack/)

生成摘要时出错

---

## 22. FreeBSD Foundation executive director tries daily driving FreeBSD on laptop

**原文标题**: FreeBSD Foundation executive director tries daily driving FreeBSD on laptop

**原文链接**: [https://www.phoronix.com/news/FreeBSD-On-Laptop-Driver](https://www.phoronix.com/news/FreeBSD-On-Laptop-Driver)

生成摘要时出错

---

## 23. Microsoft's 6502 BASIC is now Open Source (2025)

**原文标题**: Microsoft's 6502 BASIC is now Open Source (2025)

**原文链接**: [https://opensource.microsoft.com/blog/2025/09/03/microsoft-open-source-historic-6502-basic/](https://opensource.microsoft.com/blog/2025/09/03/microsoft-open-source-historic-6502-basic/)

生成摘要时出错

---

## 24. A self-powered computer in actual credit-card size (~1mm thick)

**原文标题**: A self-powered computer in actual credit-card size (~1mm thick)

**原文链接**: [https://old.reddit.com/r/electronics/comments/1td7yxl/i_built_a_fully_selfpowered_computer_in_actual/](https://old.reddit.com/r/electronics/comments/1td7yxl/i_built_a_fully_selfpowered_computer_in_actual/)

生成摘要时出错

---

## 25. 2026 HIPAA Security Rule Update

**原文标题**: 2026 HIPAA Security Rule Update

**原文链接**: [https://medcurity.com/hipaa-security-rule-2026-update/](https://medcurity.com/hipaa-security-rule-2026-update/)

生成摘要时出错

---

## 26. GPT Guesses Between 1 and 100

**原文标题**: GPT Guesses Between 1 and 100

**原文链接**: [https://github.com/exmergo/research-chatgpt-guesses-between-1-and-100](https://github.com/exmergo/research-chatgpt-guesses-between-1-and-100)

生成摘要时出错

---

## 27. Data Centers Now Consume 6% of US Electricity–and the Backlash Has Begun

**原文标题**: Data Centers Now Consume 6% of US Electricity–and the Backlash Has Begun

**原文链接**: [https://singularityhub.com/2026/05/22/data-centers-now-consume-6-of-electricity-in-the-us-and-the-backlash-has-begun/](https://singularityhub.com/2026/05/22/data-centers-now-consume-6-of-electricity-in-the-us-and-the-backlash-has-begun/)

生成摘要时出错

---

## 28. When (if ever) it's appropriate to make jokes before the US Supreme Court

**原文标题**: When (if ever) it's appropriate to make jokes before the US Supreme Court

**原文链接**: [https://www.scotusblog.com/2026/05/when-if-ever-its-appropriate-to-make-jokes-take-selfies-or-curse-before-the-court/](https://www.scotusblog.com/2026/05/when-if-ever-its-appropriate-to-make-jokes-take-selfies-or-curse-before-the-court/)

生成摘要时出错

---

## 29. Why Do We Sleep Under Blankets, Even on the Hottest Nights? (2017)

**原文标题**: Why Do We Sleep Under Blankets, Even on the Hottest Nights? (2017)

**原文链接**: [https://www.atlasobscura.com/articles/blankets-summer-hot](https://www.atlasobscura.com/articles/blankets-summer-hot)

生成摘要时出错

---

## 30. D. Trump Jr. and Eric Trump Running Felony Fraud Scheme Prosecutable in New York

**原文标题**: D. Trump Jr. and Eric Trump Running Felony Fraud Scheme Prosecutable in New York

**原文链接**: [https://cmarmitage.substack.com/p/donald-trump-jr-and-eric-trump-are](https://cmarmitage.substack.com/p/donald-trump-jr-and-eric-trump-are)

生成摘要时出错

---

