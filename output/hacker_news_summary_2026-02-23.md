# Hacker News 热门文章摘要 (2026-02-23)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 我搭建了Timeframe，我们的家庭电子纸仪表盘

**原文标题**: I built Timeframe, our family e-paper dashboard

**原文链接**: [https://hawksley.org/2026/02/17/timeframe.html](https://hawksley.org/2026/02/17/timeframe.html)

Joel Hawksley 用十多年时间打造了 Timeframe，这是一个家庭电子纸仪表盘，旨在无需传统背光屏幕的情况下提供日历、天气和智能家居数据等基本信息。早期原型包括一个“魔镜”（亮度过高）和越狱的 Kindle 设备（验证了电子纸的概念，但不可靠，通过 Ruby on Rails 应用每30分钟更新一次）。

他转而使用更可靠的 Visionect 电子纸显示屏，实现了5分钟更新。然而，一项市场测试显示成本过高（一个13英寸屏幕1000美元，外加月费）。马歇尔大火摧毁他家后，一个关键时刻随之而来，这恰逢 Boox 25.3英寸 Mira Pro 发布。这款通过 HDMI 驱动的高分辨率、实时更新的电子纸显示屏，被证明是颠覆性的，并被整合到他的新家设计中。

这种实时性要求促使后端进行了彻底的改造。Hawksley 将大部分数据抓取迁移到 Home Assistant (HA) 进行日历、天气和智能家居集成，通过取消数据库和 Redis 大幅简化了代码库。Timeframe 现在充当实时状态指示器，仅显示开着的门或洗衣完成等关键信息；空白屏幕则表示“健康”的房子。

未来的计划包括强化系统以实现更广泛的部署，实现与 Home Assistant 应用的完全集成，并解决高昂的硬件成本（例如，Boox Mira Pro 售价2000美元），从而使 Timeframe 能被更广阔的市场接受。该项目仍然是一项充满热情的事业，它显著改善了他家庭的日常生活。

---

## 2. 我如何使用 Claude 代码：规划与执行分离

**原文标题**: How I use Claude Code: Separation of planning and execution

**原文链接**: [https://boristane.com/blog/how-i-use-claude-code/](https://boristane.com/blog/how-i-use-claude-code/)

作者为Claude代码提出了一种独特的“规划与执行分离”工作流，强调代码只有在详细且经用户批准的计划之后才能编写。这种方法可以避免徒劳的工作，保持架构控制，并产生卓越的成果。

工作流包括以下几个不同的阶段：
1.  **研究：** Claude对代码库进行深入阅读，并将发现记录在一个持久化的`research.md`文件中。这通过确保预先彻底理解来防止误解和昂贵的架构错误。
2.  **规划：** Claude起草一份详细的`plan.md`文档，概述实现方法、代码片段和文件更改。作者经常提供参考代码以提供更好的上下文。
3.  **批注循环：** 这是工作流的核心。用户在其编辑器中审查`plan.md`，添加内联注释以纠正假设、增加约束或注入领域知识。Claude随后根据这些注释更新计划。这个迭代过程重复1-6次，并带有一个明确的“暂不实现”守卫，利用markdown文件作为“共享可变状态”来精确地完善计划。
4.  **待办事项列表：** 将详细的任务分解添加到计划中，在实现过程中作为进度跟踪器。
5.  **实现：** 一个单一、标准化的提示启动执行，指示Claude实现所有内容，将任务标记为完成，保持严格的类型，并持续运行类型检查。实现变得机械化，所有创造性决策都在规划阶段完成。
6.  **反馈：** 在实现过程中，如果某个方法出错，用户会提供简洁的纠正，引用现有代码，或者进行回滚并重新确定范围。
7.  **主导权：** 用户始终保持控制权，精心挑选提案，缩减范围，并根据更广泛的项目背景和产品优先级推翻技术选择。

作者在单个、长时间的会话中执行这些阶段，相信Claude的理解会随着时间的推移而加深。这种严谨的流程将用户判断与AI执行分离，从而实现更健壮和受控的开发。

---

## 3. 瓢虫浏览器采用 Rust

**原文标题**: Ladybird Browser adopts Rust

**原文链接**: [https://ladybird.org/posts/adopting-rust/](https://ladybird.org/posts/adopting-rust/)

Andreas Kling于2026年2月23日宣布，Ladybird浏览器正在采用Rust，并借助AI辅助，以取代C++，从而提升内存安全性。在考虑了Swift之后（Swift缺乏强大的C++互操作性和跨平台支持），最终选择了Rust，因为它拥有成熟的系统编程生态系统和安全保障，这与Firefox和Chromium所展现的趋势一致。

尽管Rust在2024年曾因与C++ 20世纪90年代风格的面向对象编程（深度继承、垃圾回收）不兼容而被最初拒绝，但对安全性及强大生态系统的务实需求使Rust成为了首选。

首次移植的主要组件是Ladybird的JavaScript引擎LibJS，具体包括其词法分析器、解析器、抽象语法树（AST）和字节码生成器。此次转换涉及了人类指导的AI（Claude Code和Codex），使用了数百个小提示并进行了对抗性代码审查。

结果令人印象深刻：大约25,000行Rust代码在短短两周内被移植完成（手动完成这项任务预计需要数月）。新的Rust代码在抽象语法树和字节码方面，与C++管道相比，产生了逐字节相同的输出，确保在test262和Ladybird自身测试等广泛的测试套件中没有出现任何退化，且对性能没有影响。

转换后的Rust代码特意模仿了C++的模式以确保兼容性，这意味着它尚不完全是地道的Rust代码，但未来计划进行清理。此次Rust迁移将是一项长期且受控的工作，与C++的持续开发并行，核心团队将协调所有的移植工作。Kling认为这是Ladybird未来发展中一个有争议但必要的步骤。

---

## 4. 年龄验证陷阱：验证年龄损害所有人的数据保护

**原文标题**: The Age Verification Trap: Verifying age undermines everyone's data protection

**原文链接**: [https://spectrum.ieee.org/age-verification](https://spectrum.ieee.org/age-verification)

提供的文本是一篇文章的导言，而非文章全文。它包含了标题、作者姓名、作者资历和出版详情，但*缺少文章的主体内容*。

因此，我无法总结文章的要点和关键信息，因为文章内容缺失。我只能重申已提供的信息：

**所提供文本（仅导言）的摘要：**

这篇题为“年龄验证陷阱：验证年龄损害了所有人的数据保护”的文章，是电信领域内的一篇评论文章。作者是Waydell D. Carvalho，一位专注于人工智能治理、监管设计和社会技术风险的独立研究员和系统架构师。文章认为，年龄验证实践对普遍数据保护有害。预计阅读时长为10分钟。

---

## 5. 谷歌限制Google AI Pro/Ultra订阅用户使用OpenClaw

**原文标题**: Google restricting Google AI Pro/Ultra subscribers for using OpenClaw

**原文链接**: [https://discuss.ai.google.dev/t/account-restricted-without-warning-google-ai-ultra-oauth-via-openclaw/122778](https://discuss.ai.google.dev/t/account-restricted-without-warning-google-ai-ultra-oauth-via-openclaw/122778)

生成摘要时出错

---

## 6. 注意力媒体不等于社交网络

**原文标题**: Attention Media ≠ Social Networks

**原文链接**: [https://susam.net/attention-media-vs-social-networks.html](https://susam.net/attention-media-vs-social-networks.html)

Susam Pal认为，近二十年前始于“真正的社交网络”的东西，已经退化为“注意力媒体”。最初，平台带来了Web 2.0的乐观情绪，将用户与他们认识的人联系起来，提供有意义的更新和真实的通知。

然而，在2012年至2016年间，情况发生了变化。无限滚动的引入带来了不安，通知也从相关的信号演变为旨在服务平台而非用户的操控性提示。随着时间的推移，时间线被来自陌生人而非朋友的内容淹没，使得体验感觉像是一场铺天盖地、无关紧要的广播。Pal指出，这些服务不再是社交性的，转而专注于捕获和变现用户注意力。

相比之下，作者发现Mastodon回归了真正的社交网络。它允许用户关注少量精选个体，只接收他们相关的更新，没有虚假通知或算法操纵。这种用户控制的环境带来平静、可预测的时间线，反映的是个人选择，而非旨在利用注意力的系统。Pal希望Mastodon能保留这种最初的、以用户为中心的社交互动模式。

---

## 7. Loops is a federated, open-source TikTok

**原文标题**: Loops is a federated, open-source TikTok

**原文链接**: [https://joinloops.org/](https://joinloops.org/)

Loops is introduced as a federated, open-source short-video platform, designed as an ethical alternative to corporate giants like TikTok. Now in Open Beta, it empowers creators and communities by offering "Your community. Your rules," free from corporate control, invasive tracking, and ads.

Built on the ActivityPub protocol, Loops integrates with the fediverse, allowing videos to reach users on platforms like Mastodon and Pixelfed while maintaining user control over their home server. Key features include a creator-first camera, chronological "Following" and fediverse-tuned "For You" feeds (powered by engagement, not ads), rich comment threads, and engagement metrics (likes, shares) that travel across the fediverse. Users can also control notifications and discover content via hashtags and search.

Loops' mission is to "reclaim short-video sharing for humanity," prioritizing privacy, ethical design (no dark patterns), global accessibility, community ownership, and sustainable growth. The project operates with radical transparency and encourages community governance, with all features designed for user experience rather than advertising revenue. Development is supported through sponsorships and donations, ensuring Loops remains independent and ad-free.

---

## 8. 教宗敦促神父们运用大脑而非人工智能撰写讲道词。

**原文标题**: Pope tells priests to use their brains, not AI, to write homilies

**原文链接**: [https://www.ewtnnews.com/vatican/pope-leo-xiv-tells-priests-to-use-their-brains-not-ai-to-write-homilies](https://www.ewtnnews.com/vatican/pope-leo-xiv-tells-priests-to-use-their-brains-not-ai-to-write-homilies)

Pope Francis urged priests and seminarians to avoid using artificial intelligence to write their homilies, stressing that sermons must be a "mediation that comes from the heart." Speaking to seminarians at the Vatican on June 10, the Pope emphasized the need for priests to personally "think about homilies" through prayer, study of the Word of God, and deep reflection.

He explained that a homily is not merely a conference or a lecture, but "a different service" that requires the preacher to "put his heart into it" and deliver a message born from personal spiritual engagement. Pope Francis also reiterated his frequent advice that homilies should be concise, ideally lasting no more than eight minutes, to ensure the congregation's attention and prevent boredom.

This caution against AI in spiritual guidance reflects Pope Francis's broader interest in the ethical implications of technology. While acknowledging AI's potential for good, he has previously called for its responsible and ethical development, underscoring the irreplaceable human element in matters of faith and spiritual proclamation. His message highlights the profound personal and spiritual responsibility inherent in delivering God's Word.

---

## 9. Show HN: CIA World Factbook Archive (1990–2025), searchable and exportable

**原文标题**: Show HN: CIA World Factbook Archive (1990–2025), searchable and exportable

**原文链接**: [https://cia-factbook-archive.fly.dev/](https://cia-factbook-archive.fly.dev/)

生成摘要时出错

---

## 10. Elsevier shuts down its finance journal citation cartel

**原文标题**: Elsevier shuts down its finance journal citation cartel

**原文链接**: [https://www.chrisbrunet.com/p/elsevier-shuts-down-its-finance-journal](https://www.chrisbrunet.com/p/elsevier-shuts-down-its-finance-journal)

生成摘要时出错

---

## 11. Why is Claude an Electron app?

**原文标题**: Why is Claude an Electron app?

**原文链接**: [https://www.dbreunig.com/2026/02/21/why-is-claude-an-electron-app.html](https://www.dbreunig.com/2026/02/21/why-is-claude-an-electron-app.html)

生成摘要时出错

---

## 12. How Taalas “prints” LLM onto a chip?

**原文标题**: How Taalas “prints” LLM onto a chip?

**原文链接**: [https://www.anuragk.com/blog/posts/Taalas.html](https://www.anuragk.com/blog/posts/Taalas.html)

生成摘要时出错

---

## 13. Hetzner (European hosting provider) to increase prices by up to 38%

**原文标题**: Hetzner (European hosting provider) to increase prices by up to 38%

**原文链接**: [https://old.reddit.com/r/BuyFromEU/comments/1rce0lf/hetzner_european_hosting_provider_to_increase/](https://old.reddit.com/r/BuyFromEU/comments/1rce0lf/hetzner_european_hosting_provider_to_increase/)

生成摘要时出错

---

## 14. Man accidentally gains control of 7k robot vacuums

**原文标题**: Man accidentally gains control of 7k robot vacuums

**原文链接**: [https://www.popsci.com/technology/robot-vacuum-army/](https://www.popsci.com/technology/robot-vacuum-army/)

生成摘要时出错

---

## 15. Show HN: Llama 3.1 70B on a single RTX 3090 via NVMe-to-GPU bypassing the CPU

**原文标题**: Show HN: Llama 3.1 70B on a single RTX 3090 via NVMe-to-GPU bypassing the CPU

**原文链接**: [https://github.com/xaskasdf/ntransformer](https://github.com/xaskasdf/ntransformer)

生成摘要时出错

---

## 16. Six Math Essentials

**原文标题**: Six Math Essentials

**原文链接**: [https://terrytao.wordpress.com/2026/02/16/six-math-essentials/](https://terrytao.wordpress.com/2026/02/16/six-math-essentials/)

生成摘要时出错

---

## 17. Iran students stage first large anti-government protests since deadly crackdown

**原文标题**: Iran students stage first large anti-government protests since deadly crackdown

**原文链接**: [https://www.bbc.com/news/articles/c5yj2kzkrj0o](https://www.bbc.com/news/articles/c5yj2kzkrj0o)

生成摘要时出错

---

## 18. Magical Mushroom – Europe's first industrial-scale mycelium packaging producer

**原文标题**: Magical Mushroom – Europe's first industrial-scale mycelium packaging producer

**原文链接**: [https://magicalmushroom.com/index](https://magicalmushroom.com/index)

生成摘要时出错

---

## 19. Fix your tools

**原文标题**: Fix your tools

**原文链接**: [https://ochagavia.nl/blog/fix-your-tools/](https://ochagavia.nl/blog/fix-your-tools/)

生成摘要时出错

---

## 20. Parse, Don't Validate and Type-Driven Design in Rust

**原文标题**: Parse, Don't Validate and Type-Driven Design in Rust

**原文链接**: [https://www.harudagondi.space/blog/parse-dont-validate-and-type-driven-design-in-rust/](https://www.harudagondi.space/blog/parse-dont-validate-and-type-driven-design-in-rust/)

生成摘要时出错

---

## 21. Freemediaheckyeah – A collection of free stuff on the internet

**原文标题**: Freemediaheckyeah – A collection of free stuff on the internet

**原文链接**: [https://fmhy.net/](https://fmhy.net/)

生成摘要时出错

---

## 22. What is a database transaction?

**原文标题**: What is a database transaction?

**原文链接**: [https://planetscale.com/blog/database-transactions](https://planetscale.com/blog/database-transactions)

生成摘要时出错

---

## 23. The JavaScript Oxidation Compiler

**原文标题**: The JavaScript Oxidation Compiler

**原文链接**: [https://oxc.rs/](https://oxc.rs/)

生成摘要时出错

---

## 24. We hid backdoors in ~40MB binaries and asked AI + Ghidra to find them

**原文标题**: We hid backdoors in ~40MB binaries and asked AI + Ghidra to find them

**原文链接**: [https://quesma.com/blog/introducing-binaryaudit/](https://quesma.com/blog/introducing-binaryaudit/)

Researchers conducted an experiment challenging AI agents, supported by tools like Ghidra, to find hidden backdoors in ~40MB binary executables of open-source projects like lighttpd and dnsmasq. The binaries were stripped of source code and debug symbols, simulating real-world malware analysis.

Motivated by rising supply chain attacks and firmware tampering, the study aimed to assess AI's capability in reverse engineering low-level machine code, a task traditionally requiring human expertise.

The findings were mixed. AI agents surprisingly demonstrated some specialized reverse engineering capabilities; for example, Claude Opus 4.5 successfully detected a `popen()`-based backdoor in lighttpd by analyzing imported functions and decompiled code.

However, the approach is "not ready for production." Even the top model, Claude Opus 4.6, only found backdoors 49% of the time. A significant limitation was the high false positive rate, with models flagging clean binaries 28% of the time, rendering them impractical for security. A notable failure occurred when Claude rationalized an obvious `execl("/bin/sh", ...)` backdoor in dnsmasq as legitimate script execution, failing to trace the command's origin.

The authors conclude that current AI agents lack the "high-level intuition" needed for effective binary analysis. They often struggle with the "needle-in-haystack" problem, getting distracted by legitimate code or random functions rather than strategically prioritizing high-risk areas. Despite glimmers of promise, substantial advancements are required before AI can reliably perform practical binary malware detection.

---

## 25. $30B for laptops yielded a generation less cognitively capable than parents

**原文标题**: $30B for laptops yielded a generation less cognitively capable than parents

**原文链接**: [https://www.yahoo.com/news/articles/u-spent-30-billion-ditch-110200869.html](https://www.yahoo.com/news/articles/u-spent-30-billion-ditch-110200869.html)

生成摘要时出错

---

## 26. Back to FreeBSD: Part 1

**原文标题**: Back to FreeBSD: Part 1

**原文链接**: [https://hypha.pub/back-to-freebsd-part-1](https://hypha.pub/back-to-freebsd-part-1)

生成摘要时出错

---

## 27. EDuke32 – Duke Nukem 3D (Open-Source)

**原文标题**: EDuke32 – Duke Nukem 3D (Open-Source)

**原文链接**: [https://www.eduke32.com/](https://www.eduke32.com/)

生成摘要时出错

---

## 28. Spain’s LaLiga has blocked access to freedom.gov

**原文标题**: Spain’s LaLiga has blocked access to freedom.gov

**原文链接**: [https://twitter.com/Pirat_Nation/status/2025643188321714642](https://twitter.com/Pirat_Nation/status/2025643188321714642)

生成摘要时出错

---

## 29. Show HN: Local-First Linux MicroVMs for macOS

**原文标题**: Show HN: Local-First Linux MicroVMs for macOS

**原文链接**: [https://shuru.run](https://shuru.run)

生成摘要时出错

---

## 30. Japanese Woodblock Print Search

**原文标题**: Japanese Woodblock Print Search

**原文链接**: [https://ukiyo-e.org/](https://ukiyo-e.org/)

生成摘要时出错

---

## 31. Evidence of the bouba-kiki effect in naïve baby chicks

**原文标题**: Evidence of the bouba-kiki effect in naïve baby chicks

**原文链接**: [https://www.science.org/doi/10.1126/science.adq7188](https://www.science.org/doi/10.1126/science.adq7188)

生成摘要时出错

---

## 32. Cloudflare outage on February 20, 2026

**原文标题**: Cloudflare outage on February 20, 2026

**原文链接**: [https://blog.cloudflare.com/cloudflare-outage-february-20-2026/](https://blog.cloudflare.com/cloudflare-outage-february-20-2026/)

生成摘要时出错

---

## 33. Hacker News.love – 22 projects Hacker News didn't love

**原文标题**: Hacker News.love – 22 projects Hacker News didn't love

**原文链接**: [https://hackernews.love/](https://hackernews.love/)

生成摘要时出错

---

## 34. The peculiar case of Japanese web design (2022)

**原文标题**: The peculiar case of Japanese web design (2022)

**原文链接**: [https://sabrinas.space](https://sabrinas.space)

生成摘要时出错

---

## 35. Global Intelligence Crisis

**原文标题**: Global Intelligence Crisis

**原文链接**: [https://www.citriniresearch.com/p/2028gic](https://www.citriniresearch.com/p/2028gic)

生成摘要时出错

---

## 36. Git's Magic Files

**原文标题**: Git's Magic Files

**原文链接**: [https://nesbitt.io/2026/02/05/git-magic-files.html](https://nesbitt.io/2026/02/05/git-magic-files.html)

生成摘要时出错

---

## 37. Xweather Live – Interactive global vector weather map

**原文标题**: Xweather Live – Interactive global vector weather map

**原文链接**: [https://live.xweather.com/](https://live.xweather.com/)

生成摘要时出错

---

## 38. NanoClaw moved from Apple Containers to Docker

**原文标题**: NanoClaw moved from Apple Containers to Docker

**原文链接**: [https://twitter.com/Gavriel_Cohen/status/2025603982769410356](https://twitter.com/Gavriel_Cohen/status/2025603982769410356)

生成摘要时出错

---

## 39. Hetzner Prices increase 30-40%

**原文标题**: Hetzner Prices increase 30-40%

**原文链接**: [https://docs.hetzner.com/general/infrastructure-and-availability/price-adjustment/](https://docs.hetzner.com/general/infrastructure-and-availability/price-adjustment/)

生成摘要时出错

---

## 40. A Botnet Accidentally Destroyed I2P

**原文标题**: A Botnet Accidentally Destroyed I2P

**原文链接**: [https://www.sambent.com/a-botnet-accidentally-destroyed-i2p-the-full-story/](https://www.sambent.com/a-botnet-accidentally-destroyed-i2p-the-full-story/)

生成摘要时出错

---

## 41. Hello Worg, the Org-Mode Community

**原文标题**: Hello Worg, the Org-Mode Community

**原文链接**: [https://orgmode.org/worg/](https://orgmode.org/worg/)

生成摘要时出错

---

## 42. Emulated Windows 3.11 in the Browser

**原文标题**: Emulated Windows 3.11 in the Browser

**原文链接**: [https://pieter.com/](https://pieter.com/)

生成摘要时出错

---

## 43. Crawling a billion web pages in just over 24 hours, in 2025

**原文标题**: Crawling a billion web pages in just over 24 hours, in 2025

**原文链接**: [https://andrewkchan.dev/posts/crawler.html](https://andrewkchan.dev/posts/crawler.html)

生成摘要时出错

---

## 44. Linuxulator on FreeBSD Feels Like Magic

**原文标题**: Linuxulator on FreeBSD Feels Like Magic

**原文链接**: [https://hayzam.com/blog/02-linuxulator-is-awesome/](https://hayzam.com/blog/02-linuxulator-is-awesome/)

生成摘要时出错

---

## 45. Show HN: WARN Firehose – Every US layoff notice in one searchable database

**原文标题**: Show HN: WARN Firehose – Every US layoff notice in one searchable database

**原文链接**: [https://warnfirehose.com](https://warnfirehose.com)

生成摘要时出错

---

## 46. Show HN: 3D Mahjong, Built in CSS

**原文标题**: Show HN: 3D Mahjong, Built in CSS

**原文链接**: [https://voxjong.com](https://voxjong.com)

生成摘要时出错

---

## 47. A simple web we own

**原文标题**: A simple web we own

**原文链接**: [https://rsdoiel.github.io/blog/2026/02/21/a_simple_web_we_own.html](https://rsdoiel.github.io/blog/2026/02/21/a_simple_web_we_own.html)

生成摘要时出错

---

## 48. Inputlag.science – Repository of knowledge about input lag in gaming

**原文标题**: Inputlag.science – Repository of knowledge about input lag in gaming

**原文链接**: [https://inputlag.science](https://inputlag.science)

生成摘要时出错

---

## 49. Large US company came after me for releasing a free open-source alternative

**原文标题**: Large US company came after me for releasing a free open-source alternative

**原文链接**: [https://old.reddit.com/r/selfhosted/comments/1rbkx5e/large_us_company_came_after_me_for_releasing_a/](https://old.reddit.com/r/selfhosted/comments/1rbkx5e/large_us_company_came_after_me_for_releasing_a/)

生成摘要时出错

---

## 50. Using the new bridges of FreeBSD 15

**原文标题**: Using the new bridges of FreeBSD 15

**原文链接**: [https://blog.feld.me/posts/2026/02/using-new-bridges-freebsd-15/](https://blog.feld.me/posts/2026/02/using-new-bridges-freebsd-15/)

FreeBSD 15 introduces a new, optimized bridging implementation with native VLAN support, soft-deprecating Layer 3 addresses on bridge members to achieve hardware switch-like behavior. This allows for a single bridge managing all traffic, improving performance and simplifying configuration.

The previous method required a separate bridge and VLAN interface for each VLAN, resulting in cumbersome `rc.conf` setups. The new design dramatically simplifies this, enabling a single bridge with the `vlanfilter` flag to directly specify tagged or untagged VLANs for its members (e.g., `ifconfig bridge0 "vlanfilter addm ix1 tagged 2,3,128"`).

For VNET jails, existing `jib` scripts are outdated. While `epair(4)` now natively generates stable MAC addresses, the author provides a custom script (`/scripts/vnetif`) to create and name `epair` devices, attaching them to the bridge with untagged VLANs and the required `-vlanhwfilter` flag. Jail `exec.poststop` commands are also no longer necessary.

Bhyve VMs currently lack direct `vm-bhyve` tooling support for the new bridging. The author's workaround involves manually creating `tap` interfaces in `/etc/rc.local`, adding them to the bridge with specific untagged VLANs, and then configuring `vm-bhyve` to use these pre-created devices. Stable MAC addresses for VMs must be set when creating the `tap` interface. This new bridging is a significant improvement, despite current tooling requiring manual adjustments.

---

## 51. VTT Test Donut Lab Battery Reaches 80% Charge in Under 10 Minutes [pdf]

**原文标题**: VTT Test Donut Lab Battery Reaches 80% Charge in Under 10 Minutes [pdf]

**原文链接**: [https://pub-fee113bb711e441db5c353d2d31abbb3.r2.dev/VTT_CR_00092_26.pdf](https://pub-fee113bb711e441db5c353d2d31abbb3.r2.dev/VTT_CR_00092_26.pdf)

生成摘要时出错

---

## 52. What's the best way to learn a new language?

**原文标题**: What's the best way to learn a new language?

**原文链接**: [https://www.bbc.com/future/article/20260220-whats-the-best-way-to-learn-a-new-language](https://www.bbc.com/future/article/20260220-whats-the-best-way-to-learn-a-new-language)

生成摘要时出错

---

## 53. Fresh File Explorer – VS Code extension for navigating recent work

**原文标题**: Fresh File Explorer – VS Code extension for navigating recent work

**原文链接**: [https://github.com/FreHu/vscode-fresh-file-explorer](https://github.com/FreHu/vscode-fresh-file-explorer)

生成摘要时出错

---

## 54. An Unbothered Jimmy Wales Calls Grokipedia a 'Cartoon Imitation' of Wikipedia

**原文标题**: An Unbothered Jimmy Wales Calls Grokipedia a 'Cartoon Imitation' of Wikipedia

**原文链接**: [https://gizmodo.com/an-unbothered-jimmy-wales-calls-grokipedia-a-cartoon-imitation-of-wikipedia-2000725070](https://gizmodo.com/an-unbothered-jimmy-wales-calls-grokipedia-a-cartoon-imitation-of-wikipedia-2000725070)

生成摘要时出错

---

## 55. Algolia Hacker News Search GitHub Project Archived

**原文标题**: Algolia Hacker News Search GitHub Project Archived

**原文链接**: [https://github.com/algolia/hn-search](https://github.com/algolia/hn-search)

生成摘要时出错

---

## 56. Show HN: PgDog – Scale Postgres without changing the app

**原文标题**: Show HN: PgDog – Scale Postgres without changing the app

**原文链接**: [https://github.com/pgdogdev/pgdog](https://github.com/pgdogdev/pgdog)

生成摘要时出错

---

## 57. Minions: Stripe’s one-shot, end-to-end coding agents

**原文标题**: Minions: Stripe’s one-shot, end-to-end coding agents

**原文链接**: [https://stripe.dev/blog/minions-stripes-one-shot-end-to-end-coding-agents](https://stripe.dev/blog/minions-stripes-one-shot-end-to-end-coding-agents)

生成摘要时出错

---

## 58. Mexican Forces Kill Nation's Most-Wanted Cartel Boss

**原文标题**: Mexican Forces Kill Nation's Most-Wanted Cartel Boss

**原文链接**: [https://www.nytimes.com/2026/02/22/world/americas/jalisco-new-generation-cartel-leader-killed.html](https://www.nytimes.com/2026/02/22/world/americas/jalisco-new-generation-cartel-leader-killed.html)

生成摘要时出错

---

## 59. Show HN: AI Timeline – 171 LLMs from Transformer (2017) to GPT-5.3 (2026)

**原文标题**: Show HN: AI Timeline – 171 LLMs from Transformer (2017) to GPT-5.3 (2026)

**原文链接**: [https://llm-timeline.com/](https://llm-timeline.com/)

生成摘要时出错

---

## 60. femtolisp: A lightweight, robust, scheme-like Lisp implementation

**原文标题**: femtolisp: A lightweight, robust, scheme-like Lisp implementation

**原文链接**: [https://github.com/JeffBezanson/femtolisp](https://github.com/JeffBezanson/femtolisp)

生成摘要时出错

---

## 61. Palantir's secret weapon isn't AI – it's Ontology. An open-source deep dive

**原文标题**: Palantir's secret weapon isn't AI – it's Ontology. An open-source deep dive

**原文链接**: [https://github.com/Leading-AI-IO/palantir-ontology-strategy](https://github.com/Leading-AI-IO/palantir-ontology-strategy)

生成摘要时出错

---

## 62. Facebook's Fascination with My Robots.txt

**原文标题**: Facebook's Fascination with My Robots.txt

**原文链接**: [https://blog.nytsoi.net/2026/02/23/facebook-robots-txt](https://blog.nytsoi.net/2026/02/23/facebook-robots-txt)

生成摘要时出错

---

## 63. Password managers less secure than promised

**原文标题**: Password managers less secure than promised

**原文链接**: [https://ethz.ch/en/news-and-events/eth-news/news/2026/02/password-managers-less-secure-than-promised.html](https://ethz.ch/en/news-and-events/eth-news/news/2026/02/password-managers-less-secure-than-promised.html)

生成摘要时出错

---

## 64. Iranian Students Protest as Anger Grows

**原文标题**: Iranian Students Protest as Anger Grows

**原文链接**: [https://www.wsj.com/world/middle-east/iranian-students-protest-as-anger-grows-89a6a44e](https://www.wsj.com/world/middle-east/iranian-students-protest-as-anger-grows-89a6a44e)

生成摘要时出错

---

## 65. Anthropic announces proof of distillation at scale by MiniMax, DeepSeek,Moonshot

**原文标题**: Anthropic announces proof of distillation at scale by MiniMax, DeepSeek,Moonshot

**原文链接**: [https://twitter.com/anthropicai/status/2025997928242811253](https://twitter.com/anthropicai/status/2025997928242811253)

生成摘要时出错

---

## 66. The Tears of Donald Knuth (2015)

**原文标题**: The Tears of Donald Knuth (2015)

**原文链接**: [https://cacm.acm.org/opinion/the-tears-of-donald-knuth/](https://cacm.acm.org/opinion/the-tears-of-donald-knuth/)

生成摘要时出错

---

## 67. I put New Zealand behind a $1 paywall

**原文标题**: I put New Zealand behind a $1 paywall

**原文链接**: [https://rename.world/](https://rename.world/)

生成摘要时出错

---

## 68. ASML unveils EUV light source advance that could yield 50% more chips by 2030

**原文标题**: ASML unveils EUV light source advance that could yield 50% more chips by 2030

**原文链接**: [https://www.reuters.com/world/china/asml-unveils-euv-light-source-advance-that-could-yield-50-more-chips-by-2030-2026-02-23/](https://www.reuters.com/world/china/asml-unveils-euv-light-source-advance-that-could-yield-50-more-chips-by-2030-2026-02-23/)

生成摘要时出错

---

## 69. U.S. Cannot Legally Impose Tariffs Using Section 122 of the Trade Act of 1974

**原文标题**: U.S. Cannot Legally Impose Tariffs Using Section 122 of the Trade Act of 1974

**原文链接**: [https://ielp.worldtradelaw.net/2026/01/guest-post-president-trump-cannot-legally-impose-tariffs-using-section-122-of-the-trade-act-of-1974/](https://ielp.worldtradelaw.net/2026/01/guest-post-president-trump-cannot-legally-impose-tariffs-using-section-122-of-the-trade-act-of-1974/)

生成摘要时出错

---

## 70. People Loved the Dot-Com Boom. The A.I. Boom, Not So Much

**原文标题**: People Loved the Dot-Com Boom. The A.I. Boom, Not So Much

**原文链接**: [https://www.nytimes.com/2026/02/21/technology/ai-boom-backlash.html](https://www.nytimes.com/2026/02/21/technology/ai-boom-backlash.html)

生成摘要时出错

---

## 71. AIs can generate near-verbatim copies of novels from training data

**原文标题**: AIs can generate near-verbatim copies of novels from training data

**原文链接**: [https://arstechnica.com/ai/2026/02/ais-can-generate-near-verbatim-copies-of-novels-from-training-data/](https://arstechnica.com/ai/2026/02/ais-can-generate-near-verbatim-copies-of-novels-from-training-data/)

生成摘要时出错

---

## 72. The dance floor is disappearing in a sea of phones

**原文标题**: The dance floor is disappearing in a sea of phones

**原文链接**: [https://www.bloomberg.com/news/features/2026-02-20/a-boom-in-electronic-dance-music-is-changing-club-culture](https://www.bloomberg.com/news/features/2026-02-20/a-boom-in-electronic-dance-music-is-changing-club-culture)

生成摘要时出错

---

## 73. Large study finds link between cannabis use in teens and psychosis later

**原文标题**: Large study finds link between cannabis use in teens and psychosis later

**原文链接**: [https://text.npr.org/nx-s1-5719338](https://text.npr.org/nx-s1-5719338)

生成摘要时出错

---

## 74. Zuckerberg's "fix" for child safety could end anonymous internet access for all

**原文标题**: Zuckerberg's "fix" for child safety could end anonymous internet access for all

**原文链接**: [https://reclaimthenet.org/zuckerberg-instagram-age-verification-trial](https://reclaimthenet.org/zuckerberg-instagram-age-verification-trial)

生成摘要时出错

---

## 75. Show HN: C99 implementation of new O(m log^(2/3) n) shortest path algorithm

**原文标题**: Show HN: C99 implementation of new O(m log^(2/3) n) shortest path algorithm

**原文链接**: [https://github.com/danalec/DMMSY-SSSP](https://github.com/danalec/DMMSY-SSSP)

生成摘要时出错

---

## 76. Pinterest is drowning in a sea of AI slop and auto-moderation

**原文标题**: Pinterest is drowning in a sea of AI slop and auto-moderation

**原文链接**: [https://www.404media.co/pinterest-is-drowning-in-a-sea-of-ai-slop-and-auto-moderation/](https://www.404media.co/pinterest-is-drowning-in-a-sea-of-ai-slop-and-auto-moderation/)

生成摘要时出错

---

## 77. What I learned designing a barebones UI engine

**原文标题**: What I learned designing a barebones UI engine

**原文链接**: [https://madebymohammed.com/miniui](https://madebymohammed.com/miniui)

生成摘要时出错

---

## 78. SETI@home: Data Acquisition and Front-End Processing (2025)

**原文标题**: SETI@home: Data Acquisition and Front-End Processing (2025)

**原文链接**: [https://iopscience.iop.org/article/10.3847/1538-3881/ade5a7](https://iopscience.iop.org/article/10.3847/1538-3881/ade5a7)

生成摘要时出错

---

## 79. What it means that Ubuntu is using Rust

**原文标题**: What it means that Ubuntu is using Rust

**原文链接**: [https://smallcultfollowing.com/babysteps/blog/2026/02/23/ubuntu-rustnation/](https://smallcultfollowing.com/babysteps/blog/2026/02/23/ubuntu-rustnation/)

生成摘要时出错

---

## 80. Aqua: A CLI message tool for AI agents

**原文标题**: Aqua: A CLI message tool for AI agents

**原文链接**: [https://github.com/quailyquaily/aqua](https://github.com/quailyquaily/aqua)

生成摘要时出错

---

## 81. In world without BlackBerry, physical keyboards on phones are making a comeback

**原文标题**: In world without BlackBerry, physical keyboards on phones are making a comeback

**原文链接**: [https://www.cnet.com/tech/mobile/in-a-world-without-blackberry-physical-keyboards-on-phones-are-making-a-comeback/](https://www.cnet.com/tech/mobile/in-a-world-without-blackberry-physical-keyboards-on-phones-are-making-a-comeback/)

生成摘要时出错

---

## 82. Writing code is cheap now

**原文标题**: Writing code is cheap now

**原文链接**: [https://simonwillison.net/guides/agentic-engineering-patterns/code-is-cheap/](https://simonwillison.net/guides/agentic-engineering-patterns/code-is-cheap/)

生成摘要时出错

---

## 83. Agentic Software Engineering Book

**原文标题**: Agentic Software Engineering Book

**原文链接**: [https://agenticse-book.github.io/](https://agenticse-book.github.io/)

生成摘要时出错

---

## 84. Binance Fired Employees Who Found $1.7B in Crypto Was Sent to Iran

**原文标题**: Binance Fired Employees Who Found $1.7B in Crypto Was Sent to Iran

**原文链接**: [https://www.nytimes.com/2026/02/23/technology/binance-employees-iran-firings.html](https://www.nytimes.com/2026/02/23/technology/binance-employees-iran-firings.html)

生成摘要时出错

---

## 85. How close are we to a vision for 2010?

**原文标题**: How close are we to a vision for 2010?

**原文链接**: [https://shkspr.mobi/blog/2026/02/how-close-are-we-to-a-vision-for-2010/](https://shkspr.mobi/blog/2026/02/how-close-are-we-to-a-vision-for-2010/)

生成摘要时出错

---

## 86. Tesla loses bid to overturn $243M Autopilot verdict

**原文标题**: Tesla loses bid to overturn $243M Autopilot verdict

**原文链接**: [https://techcrunch.com/2026/02/20/tesla-loses-bid-to-overturn-243m-autopilot-verdict/](https://techcrunch.com/2026/02/20/tesla-loses-bid-to-overturn-243m-autopilot-verdict/)

On February 20, 2026, a judge denied Tesla's attempt to overturn a $243 million jury verdict that held the automaker partially responsible for a fatal crash involving its Autopilot system.

Hon. Judge Beth Bloom rejected Tesla's request, stating that the company's arguments for relief had already been considered and rejected during trial and summary judgment. She noted that Tesla failed to present new arguments or controlling law to persuade the court to alter its earlier decisions or the jury verdict.

The original verdict, delivered last August, awarded $243 million against Tesla for its culpability in a 2019 fatal crash in Florida. The incident killed Naibel Benavides and critically injured Dillon Angulo. The jury assigned two-thirds of the blame to the driver and one-third to Tesla, notably assessing punitive damages solely against Tesla. Tesla's lawyers had argued that the blame rested entirely with the driver.

---

## 87. Silicon Valley can't import talent like before. So it's exporting jobs

**原文标题**: Silicon Valley can't import talent like before. So it's exporting jobs

**原文链接**: [https://restofworld.org/2026/h1b-visa-impact-india-tech-hiring-faamng/](https://restofworld.org/2026/h1b-visa-impact-india-tech-hiring-faamng/)

生成摘要时出错

---

## 88. Show HN: Sowbot – open-hardware agricultural robot (ROS2, RTK GPS)

**原文标题**: Show HN: Sowbot – open-hardware agricultural robot (ROS2, RTK GPS)

**原文链接**: [https://sowbot.co.uk/](https://sowbot.co.uk/)

生成摘要时出错

---

## 89. Music Discovery

**原文标题**: Music Discovery

**原文链接**: [https://www.secondtrack.co/](https://www.secondtrack.co/)

生成摘要时出错

---

## 90. US Gov Deploys Grok as Nutrition Bot, It Advises for Rectal Use of Vegetables

**原文标题**: US Gov Deploys Grok as Nutrition Bot, It Advises for Rectal Use of Vegetables

**原文链接**: [https://futurism.com/artificial-intelligence/us-government-grok-nutrition](https://futurism.com/artificial-intelligence/us-government-grok-nutrition)

生成摘要时出错

---

## 91. AI is destroying open source, and it's not even good yet [video]

**原文标题**: AI is destroying open source, and it's not even good yet [video]

**原文链接**: [https://www.youtube.com/watch?v=bZJ7A1QoUEI](https://www.youtube.com/watch?v=bZJ7A1QoUEI)

生成摘要时出错

---

## 92. Red Robin Died by Spreadsheet. Don't Make the Same Mistake

**原文标题**: Red Robin Died by Spreadsheet. Don't Make the Same Mistake

**原文链接**: [https://garryslist.org/posts/red-robin-died-by-spreadsheet-don-t-make-the-same-mistake](https://garryslist.org/posts/red-robin-died-by-spreadsheet-don-t-make-the-same-mistake)

生成摘要时出错

---

## 93. Postgres Is Your Friend. ORM Is Not

**原文标题**: Postgres Is Your Friend. ORM Is Not

**原文链接**: [https://hypha.pub/postgres-is-your-friend-orm-is-not](https://hypha.pub/postgres-is-your-friend-orm-is-not)

生成摘要时出错

---

## 94. DHS pausing TSA PreCheck, Global Entry programs amid funding lapse

**原文标题**: DHS pausing TSA PreCheck, Global Entry programs amid funding lapse

**原文链接**: [https://www.nbcnews.com/news/us-news/dhs-pausing-tsa-precheck-global-entry-programs-funding-lapse-rcna260114](https://www.nbcnews.com/news/us-news/dhs-pausing-tsa-precheck-global-entry-programs-funding-lapse-rcna260114)

生成摘要时出错

---

## 95. Americans are destroying Flock surveillance cameras

**原文标题**: Americans are destroying Flock surveillance cameras

**原文链接**: [https://techcrunch.com/2026/02/23/americans-are-destroying-flock-surveillance-cameras/](https://techcrunch.com/2026/02/23/americans-are-destroying-flock-surveillance-cameras/)

生成摘要时出错

---

## 96. The power of daily rituals (2021)

**原文标题**: The power of daily rituals (2021)

**原文链接**: [https://www.bbc.com/future/article/20210914-how-rituals-help-us-to-deal-with-uncertainty-and-stress](https://www.bbc.com/future/article/20210914-how-rituals-help-us-to-deal-with-uncertainty-and-stress)

生成摘要时出错

---

## 97. Altman on AI energy: it also takes 20 years of eating food to train a human

**原文标题**: Altman on AI energy: it also takes 20 years of eating food to train a human

**原文链接**: [https://old.reddit.com/r/singularity/comments/1rb2pzf/sam_altman_people_talk_about_how_much_energy_it/](https://old.reddit.com/r/singularity/comments/1rb2pzf/sam_altman_people_talk_about_how_much_energy_it/)

生成摘要时出错

---

## 98. Yet Another Fix Coming for Older AMD GPUs on Linux – Thanks to Valve Developer

**原文标题**: Yet Another Fix Coming for Older AMD GPUs on Linux – Thanks to Valve Developer

**原文链接**: [https://www.phoronix.com/news/Hawaii-Macs-AMDGPU-DC-Fix](https://www.phoronix.com/news/Hawaii-Macs-AMDGPU-DC-Fix)

生成摘要时出错

---

## 99. Anthropic Education the AI Fluency Index

**原文标题**: Anthropic Education the AI Fluency Index

**原文链接**: [https://www.anthropic.com/research/AI-fluency-index](https://www.anthropic.com/research/AI-fluency-index)

生成摘要时出错

---

## 100. The Geometry of Tostitos Scoops

**原文标题**: The Geometry of Tostitos Scoops

**原文链接**: [https://chip-tech-rob.zocomputer.io/](https://chip-tech-rob.zocomputer.io/)

生成摘要时出错

---

