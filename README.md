# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-04-14.md)

*最后自动更新时间: 2026-04-14 20:33:40*
## 1. 未来的一切都是谎言，我想：工作

**原文标题**: The future of everything is lies, I guess: Work

**原文链接**: [https://aphyr.com/posts/418-the-future-of-everything-is-lies-i-guess-work](https://aphyr.com/posts/418-the-future-of-everything-is-lies-i-guess-work)

万物皆谎，我猜：工作

题为《万物皆谎，我猜：工作》的文章，批判性地评估了大型语言模型（LLMs）对劳动力的影响，指出当前对LLM的热情是错误的。作者认为，LLMs混乱而模糊的特性，将编程变成了一种“巫术”，开发者需要“提示工程”那些反复无常的“AI精怪”，来生成不可靠且可能有害的代码。这与能保留语义推理的正式编译器形成了鲜明对比。

作者驳斥了“AI员工”的概念，强调LLMs固有的不负责任、倾向于“漫不经心地撒谎”以及可能出现“精神错乱”的问题，并以Claude模型错误管理自动售货机的轶事为例进行说明。

文章借鉴了贝恩布里奇的“自动化悖论”，警告称LLMs将导致各行各业（从软件工程到医学和教育）的普遍去技能化，因为人类将停止运用关键能力。自动化偏见、监控疲劳和“接管风险”进一步使人类与这些系统的互动复杂化，因为当自动化系统失效时，人们将越来越不擅长干预。

作者对一场“劳动力冲击”表达了深切担忧，设想了两种极端情况：要么LLMs无法提供变革性智能，导致经济“勉强度日”；要么它们实现先进能力，取代众多行业（经理、医生、工程师）的劳动力，并导致大规模失业、经济崩溃和社会动荡。

最后，文章指出机器学习（ML）将主要巩固大型科技公司的财富和权力。认为这些历来抵制纳税和工人福利的企业会自愿用巨额AI利润资助全民基本收入（UBI），这种想法被认为是“无可救药的天真”。

---

## 2. 密歇根州“数字时代”法案因隐私顾虑被撤回

**原文标题**: Michigan 'digital age' bills pulled after privacy concerns raised

**原文链接**: [https://www.thecentersquare.com/michigan/article_7ca4e268-4a68-42fb-9042-f9d8604ebd7f.html](https://www.thecentersquare.com/michigan/article_7ca4e268-4a68-42fb-9042-f9d8604ebd7f.html)

密歇根州的两项法案，众议院第4429号法案和参议院第284号法案，被称为“数字年龄保障法案”，本周在倡导团体，主要是密歇根公平选举研究所（MFEI）提出隐私担忧后被撤回。

这些相同且两党支持的法案，旨在作为“儿童安全立法”，原本要求设备制造商和操作系统在激活时“估算”用户年龄，并向应用程序和网站传输持续的“数字年龄信号”。

批评者认为该立法缺乏关键的隐私保护，包括数据使用限制、将数据与其他个人信息结合的限制以及删除要求。MFEI的Patrice Johnson表示，这些法案本将在设备内部创建一个“始终在线的身份层”，但缺乏保障措施。MFEI还强调，这些法案与全国数字童年联盟的示范立法非常相似。

在MFEI向立法者分享其调查结果后，法案共同提案人承认了这些问题。两天之内，众议院和参议院版本都被撤回。提案人众议员Brad Paquette和参议员John Cherry现在正与倡导团体合作，制定潜在的替代立法。倡导团体建议未来的法案应成为全面的“消费者数据隐私框架”的一部分，赋予用户知情权、删除权、选择退出数据销售权以及限制数据使用权。MFEI称赞这一结果是基层对州政策产生影响的一个范例。

---

## 3. 内省扩散语言模型

**原文标题**: Introspective Diffusion Language Models

**原文链接**: [https://introspective-diffusion.github.io/](https://introspective-diffusion.github.io/)

内省扩散语言模型 (I-DLM) 解决了扩散语言模型 (DLM) 和自回归 (AR) 模型之间长期存在的质量差距，并将其归因于现有 DLM 缺乏“内省一致性”。AR 模型本质上会验证它们生成的内容，而 DLM 通常只进行去噪。

I-DLM 引入了内省分步解码 (ISD)，这是一种新颖的方法，允许模型在单个前向传播中同时生成新 token 和验证先前生成的 token。这种方法统一了生成和内省，与 AR 训练相呼应。

I-DLM-8B 的主要成就包括：
*   **质量匹配：** 它是第一个与其同等规模 AR 模型质量相匹配的 DLM，在 15 项基准测试中，它以一半的参数超越了更大的模型，例如 LLaDA-2.1-mini (16B)（例如，在 AIME-24 上高出 26 分）。
*   **吞吐量：** 在高并发下，吞吐量比 LLaDA-2.1-mini 高 2.9-4.1 倍。
*   **无损加速：** 借助门控 LoRA，I-DLM 实现了与基础 AR 模型逐比特相同的输出，从而实现无损加速。
*   **计算效率：** I-DLM 的计算效率大于 1，这意味着它每个 FLOP 产生的有用输出比 AR 更多，使其吞吐量在高并发下能够有效扩展。

I-DLM 方法包括内省一致性训练（转换预训练 AR 模型）、用于高效生成和验证的 ISD、以及 AR 兼容的服务，从而无需自定义后端即可直接集成到 SGLang 等现有 AR 基础设施中。I-DLM 有效克服了困扰先前 DLM 的内省一致性低、计算效率低下和基础设施不匹配等瓶颈。

---

## 4. 可完善的编程语言

**原文标题**: A perfectable programming language

**原文链接**: [https://alok.github.io/lean-pages/perfectable-lean/](https://alok.github.io/lean-pages/perfectable-lean/)

文章推崇Lean为“最好的”编程语言，因为它具有“可完善性”，即它可以在自身内部进行推理和改进，从而形成一个被称为“进步”的“事实和属性的宏伟体系”。

这种可完善性主要源于两个方面。首先，其**语义**建立在依赖类型之上。作者观察到编程语言普遍存在向更强类型化发展的趋势（例如TypeScript、Rust、Python注解），并断言依赖类型代表了将代码属性直接嵌入语言中“最恰当”且最强大的方式。这自然而然地导致了对定理证明基础设施的需求，而Lean恰好拥有这种设施，从而能够对代码行为进行形式化验证，例如验证一个函数总是返回特定值。

其次，Lean提供了“惊人地无缝”的**元编程和自定义语法**，这与其他语言中常常显得笨拙的功能形成了鲜明对比。这使得开发人员能够设计出高度表达性的领域特定语言和可视化符号，例如所展示的井字棋盘字面量，从而促进分层API和灵活的语法解释。

除了这些核心功能之外，作者还强调了**速度**，指出Lean由于能够形式化证明代码等价性，因此具有很高的优化上限，从而可以实现激进的编译器优化。重要的是，Lean被认为是同类语言中唯一一个——它结合了核心编程能力和强大的定理证明器——并且正在积极获得**社区关注度**的语言，这使其有别于Coq、Idris和Agda等不太成功的竞争者。文章最后指出，这篇帖子本身就是用Lean代码编写的。

---

## 5. 欧洲AI：制胜秘籍

**原文标题**: European AI. A playbook to own it

**原文链接**: [https://europe.mistral.ai/](https://europe.mistral.ai/)

Mistral AI发布了一份名为《欧洲人工智能：掌握主动权的行动指南》的报告，文中指出欧洲必须成为一个自力更生的人工智能强国，以克服其与美国和中国之间日益扩大的技术差距。欧洲拥有独特的优势，包括世界一流的学术生态系统、对以人为本技术的坚持，以及一个拥有4.5亿人口的强大单一市场。然而，它面临着市场碎片化、人才流失和投资缺口等挑战，这些风险可能导致经济衰退和战略脆弱性。

Mistral AI首席执行官Arthur Mensch强调，人工智能革命为欧洲提供了引领潮流和定义自身发展道路的机会，从而确保自主权并扩大全球影响力。该行动指南提出了一个以行动、团结和速度为基础的实用框架，聚焦于三大支柱：

1.  **吸引和留住人才：** 措施包括设立“人工智能蓝卡”以实现快速签证，促进更深入的大学与产业合作，建立泛欧洲人工智能创新机构，以及改善人才流动性，以将欧洲定位为全球人工智能人才中心。
2.  **规模化：释放单一市场潜力：** 为应对市场碎片化并解决欧洲在全球风险投资中份额微乎其微（5%）的问题，该行动指南建议精简数字法规，建立欧盟人工智能合规门户，设立企业行为单一登记制度，推出欧盟企业银行通行证，以及为投资基金设立“人工智能欧洲风险投资标签”（AI EuVECA Label）。
3.  **在实体经济中普及欧洲人工智能：** 该文件强调了在实际应用中大规模部署人工智能的必要性，认为广泛采用将推动创新，并为本土人工智能创造一个良性循环的供需关系。

报告的总体信息是，掌控其人工智能和基础设施对欧洲而言并非可选项，而是赢得人工智能竞赛并确保人工智能按照欧洲自身条件为欧洲发展所必不可少的。

---

## 6. 如何让 Firefox 构建速度提升17%

**原文标题**: How to make Firefox builds 17% faster

**原文链接**: [https://blog.farre.se/posts/2026/04/10/caching-webidl-codegen/](https://blog.farre.se/posts/2026/04/10/caching-webidl-codegen/)

This article details how Firefox build times, particularly for "clobber" builds, can be significantly improved by extending `buildcache`'s capabilities to non-compiler steps using its Lua plugin system.

The "WebIDL step" is a Python-based codegen process (`python3 -m mozbuild.action.webidl`) that converts `.webidl` files into C++ binding code. This step is deterministic, produces thousands of files, and runs on every clobber build, making it an ideal candidate for caching. However, traditional compiler caches like `ccache` and `sccache` couldn't cache it as they only wrap compiler invocations.

The solution, introduced in Bug 2027655, involves modifying `dom/bindings/Makefile.in` to conditionally pass `$(CCACHE)` (which becomes `buildcache`) as a command wrapper to the WebIDL `py_action` call. This change is specific to `buildcache` because of its unique Lua plugin system.

A `webidl.lua` wrapper was created, which instructs `buildcache` on how to handle the `mozbuild.action.webidl` command. It identifies the command, its `.webidl` source and Python script inputs, and its generated C++ outputs, allowing `buildcache` to hash these, check the cache, and either replay results or execute the command and store them.

Performance tests show a significant improvement: a warm clobber build (which initially took 5m35s cold) drops to 1m27s with `buildcache` alone, and further to 1m12s with the `webidl.lua` plugin active, saving an additional 15 seconds.

This WebIDL wrapper serves as a proof of concept for leveraging `buildcache`'s Lua plugins to cache any deterministic build step with known inputs and outputs, with plans to extend this approach to other codegen actions in Firefox. Users can enable it by configuring `buildcache` with the `buildcache-wrappers` repository.

---

## 7. An AI Vibe Coding Horror Story

**原文标题**: An AI Vibe Coding Horror Story

**原文链接**: [https://www.tobru.ch/an-ai-vibe-coding-horror-story/](https://www.tobru.ch/an-ai-vibe-coding-horror-story/)

生成摘要时出错

---

## 8. I went to America's worst national parks so you don't have to

**原文标题**: I went to America's worst national parks so you don't have to

**原文链接**: [https://substack.com/home/post/p-193626949](https://substack.com/home/post/p-193626949)

生成摘要时出错

---

## 9. Claude Code Routines

**原文标题**: Claude Code Routines

**原文链接**: [https://code.claude.com/docs/en/routines](https://code.claude.com/docs/en/routines)

生成摘要时出错

---

## 10. Show HN: I built a social media management tool in 3 weeks with Claude and Codex

**原文标题**: Show HN: I built a social media management tool in 3 weeks with Claude and Codex

**原文链接**: [https://github.com/brightbeanxyz/brightbean-studio](https://github.com/brightbeanxyz/brightbean-studio)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 2 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 3 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 4 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 5 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 6 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 7 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 8 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 9 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 10 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 11 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 12 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 13 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 14 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 15 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 16 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 17 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 18 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 19 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 20 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 21 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 22 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 23 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 24 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 25 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 26 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 27 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 28 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 29 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 30 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 31 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 32 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 33 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 34 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 35 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 36 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 37 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 38 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 39 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 40 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 41 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 42 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 43 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 44 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 45 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 46 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 47 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 48 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 49 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 50 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 51 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 52 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 53 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 54 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 55 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 56 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 57 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 58 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 59 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 60 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 61 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 62 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 63 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 64 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 65 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 66 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 67 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 68 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 69 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 70 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 71 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 72 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 73 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 74 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 75 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 76 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 77 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 78 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 79 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 80 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 81 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 82 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 83 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 84 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 85 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 86 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 87 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 88 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 89 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 90 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 91 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 92 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 93 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 94 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 95 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 96 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 97 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 98 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 99 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 100 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 101 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 102 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 103 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 104 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 105 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 106 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 107 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 108 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 109 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 110 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 111 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 112 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 113 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 114 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 115 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 116 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 117 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 118 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 119 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 120 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 121 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 122 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 123 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 124 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 125 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 126 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 127 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 128 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 129 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 130 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 131 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 132 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 133 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 134 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 135 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 136 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 137 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 138 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 139 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 140 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 141 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 142 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 143 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 144 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 145 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 146 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 147 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 148 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 149 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 150 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 151 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 152 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 153 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 154 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 155 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 156 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 157 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 158 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
