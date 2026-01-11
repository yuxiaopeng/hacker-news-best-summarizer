# Hacker News 热门文章摘要 (2026-01-11)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 让我介绍一下，雪铁龙 C15

**原文标题**: Allow me to introduce, the Citroen C15

**原文链接**: [https://eupolicy.social/@jmaris/115860595238097654](https://eupolicy.social/@jmaris/115860595238097654)

所提供的内容，标题为“请允许我介绍，雪铁龙C15”，实际上并未介绍或讨论雪铁龙C15。相反，它呈现的是一条来自Mastodon的支离破碎的社交媒体帖子。

这条帖子由用户Jordan Maris发布，标识为🇪🇺 🇺🇦 #NAFO，并来自“EUpolicy.social——一个服务于欧盟圈（EU bubble）的Mastodon服务器”。Maris帖子中可见的内容是一段不完整的引文：“我经常听到美国人和富有的英国人为购买……辩解”。该声明的其余部分及其语境和含义均已缺失。

此外，文本中还包含一条中文信息，指出使用Mastodon网页应用程序需要JavaScript，或者建议使用特定平台的Mastodon应用程序。

---

## 2. 我把 Windows 换成了 Linux，一切都很顺利。

**原文标题**: I replaced Windows with Linux and everything's going great

**原文链接**: [https://www.theverge.com/tech/858910/linux-diary-gaming-desktop](https://www.theverge.com/tech/858910/linux-diary-gaming-desktop)

高级测评编辑内森·爱德华兹（Nathan Edwards）讲述了他因对Windows日益沮丧，转而将Linux作为主桌面操作系统后最初一周的经历。他的目标是确定Linux是否可以成为一个“可行的替代品”，而无需进行大量的技术“折腾”。

他选择了CachyOS，一个基于Arch的发行版，以其对现代硬件的优化和游戏便利性而闻名。安装过程包括选择一个引导加载程序（Limine），分区他的硬盘（最初100GB根目录，后来扩展），并选择一个桌面环境（KDE）。他最直接且幽默的挑战是他那老旧的游戏鼠标，鼠标指针可以移动，但在桌面上无法注册点击，然而在游戏中却能完美运行。

尽管如此，他的大部分硬件，包括GPU驱动、显示器、扬声器、网络摄像头和打印机，都“即插即用”，无需任何努力。使用各种Linux应用仓库安装流行的应用程序，如Chromium、Discord、Slack和Audacity，都非常简单。游戏也变得简单：CachyOS的一键游戏包让《天外世界》（The Outer Worlds）通过Proton完美运行，并支持云存档同步。

小问题包括缺少他偏爱的Arc浏览器，以及Airtable和Spotify等服务的官方应用（尽管浏览器版本可以运行）。主要的烦恼是让《我的世界：基岩版》（Minecraft: Bedrock Edition）运行起来，这对于和孩子们一起玩至关重要。

爱德华兹承认这只是一个“蜜月期”，但他报告说“后悔程度：无”。他发现这次过渡“比预期容易得多”，并且相比Windows的烦扰，他很欣赏这种“更安静的体验”。尽管他的工作不允许他完全使用Linux，但他第一周的经历预示着他的Linux之旅前景乐观。

---

## 3. “Erdos problem #728 was solved more or less autonomously by AI”

**原文标题**: “Erdos problem #728 was solved more or less autonomously by AI”

**原文链接**: [https://mathstodon.xyz/@tao/115855840223258103](https://mathstodon.xyz/@tao/115855840223258103)

生成摘要时出错

---

## 4. 发现并修复Ghostty最大的内存泄漏

**原文标题**: Finding and fixing Ghostty's largest memory leak

**原文链接**: [https://mitchellh.com/writing/ghostty-memory-leak-fix](https://mitchellh.com/writing/ghostty-memory-leak-fix)

Ghostty用户报告了一个离谱的内存泄漏，某个实例在10天内达到了37 GB。修复方案已经找到并合并，将在未来的版本中提供。

该泄漏源于Ghostty使用`PageList`（一个内存页的双向链表）管理终端内存的方式。大多数页面是标准大小的，从内存池中获取。然而，对于包含大量表情符号或超链接等内容，更大的“非标准”页面则通过`mmap`直接分配。标准页面在释放时会返回内存池，而非标准页面则需要`munmap`。

Ghostty还通过在达到回滚限制时将最旧的页面重用为最新页面来优化回滚历史的修剪，从而避免了重新分配。

当一个非标准页面通过这种回滚优化被重用时，bug就出现了。它的*元数据*被重置以指示其为标准大小，但底层的、通过`mmap`分配的大块内存实际上从未被重新调整大小。后来，当系统尝试释放此页面时，它看到了“标准大小”的元数据，认为这是一个池化页面，因此*从未*调用`munmap`。这导致了通过`mmap`分配的大块内存泄漏。

最初，非标准页面很少见，因此自Ghostty 1.0以来，此泄漏一直未被发现。然而，最近CLI应用程序（如Claude Code）的兴起，它们经常生成复杂的多码点字素，在大量回滚操作下开始生成大量的非标准页面，从而大规模触发了泄漏。

修复方案在概念上很简单：在回滚修剪期间不再重用非标准页面。相反，它们会被正确地`munmap`，并从内存池中分配一个新的标准大小页面。

为了帮助诊断，macOS上实现了虚拟内存标签，使得Ghostty的`PageList`内存可以在调试工具中被专门识别，从而确认了泄漏并验证了修复。现有的泄漏预防措施由于其独特的触发条件而未能发现这个特定的bug；一个新的测试现在可以防止此问题再次出现。

---

## 5. 我弃用 Windows 11 投奔 Linux，你也该如此。

**原文标题**: I dumped Windows 11 for Linux, and you should too

**原文链接**: [https://www.notebookcheck.net/I-dumped-Windows-11-for-Linux-and-you-should-too.1190961.0.html](https://www.notebookcheck.net/I-dumped-Windows-11-for-Linux-and-you-should-too.1190961.0.html)

The author, frustrated with Windows 11's pervasive telemetry (like Copilot and Recall) and severe instability (frequent crashes, buggy updates, disjointed settings), migrated fully to Linux after a Windows update deleted his dual-boot partition. He initially considered macOS but found it restrictive and sluggish on older hardware.

His journey through various Linux distributions led him to Artix Linux for its control and lightweight nature, reserving Mint for a family media PC. Challenges included installing wireless drivers on an older MacBook Air (requiring an Ethernet connection) and resolving graphical glitches and network manager issues after trying different desktop environments. He also noted some game compatibility issues (e.g., Civilization III) and the absence of specific Windows-only software.

However, the benefits significantly outweighed the hurdles. He found smartphone management surprisingly excellent, especially for iPhones using the Dolphin file manager, bypassing iTunes entirely. The biggest gain was "joy": Linux resurrected his enthusiasm for computing, offering endless customization and learning opportunities. His systems became significantly more stable (zero crashes) and faster than on Windows. While demanding some technical know-how, Linux's flexibility allows users to choose distros ranging from beginner-friendly to highly customizable. Ultimately, for the author, Linux wasn't just a fix; it transformed his computing experience, offering a sense of accomplishment in problem-solving that Windows never provided.

---

## 6. HN 展示: 我使用克劳德代码发现了100本书之间的关联

**原文标题**: Show HN: I used Claude Code to discover connections between 100 books

**原文链接**: [https://trails.pieterma.es/](https://trails.pieterma.es/)

这篇 Show HN 帖子详细介绍了一个项目，作者在该项目中利用AI工具“Claude Code”对一百本书籍的语料库进行分析，以发现其中的联系。

核心发现围绕着普遍存在的**自我欺骗**概念。分析表明，自我欺骗不仅仅是一个缺陷，还可以作为一种策略机制，并观察到“最善于撒谎的人会相信自己的谎言”。这一主题通过“有益的谎言”（useful lies）和“善意的谎言”（blue lies）等概念进行探讨，这些谎言通常指为了他人或团体的利益而使用的欺骗行为。这些行为的根本框架归因于**进化心理学**，表明这种形式的自我欺骗和策略性谎言可能具有适应性优势。

---

## 7. 暗空挽歌：数据可视化杰作 (2023)

**原文标题**: Eulogy for Dark Sky, a data visualization masterpiece (2023)

**原文链接**: [https://nightingaledvs.com/dark-sky-weather-data-viz/](https://nightingaledvs.com/dark-sky-weather-data-viz/)

提供的文本是一个不完整的摘录，似乎与其给定的标题不符。

虽然标题暗示着“对数据可视化杰作Dark Sky的悼词（2023年）”，但实际内容却聚焦于数据可视化刊物“Nightingale”。它宣布庆祝“Nightingale社区成立五周年！”，该社区自2019年7月启动。Nightingale由其编辑创立，旨在填补数据可视化领域的一个特定空白。

因此，无法根据现有内容提供“对Dark Sky的悼词”的摘要，因为文本描述的是Nightingale刊物的历史和周年纪念。

---

## 8. 代码共生共荣

**原文标题**: Code and Let Live

**原文链接**: [https://fly.io/blog/code-and-let-live/](https://fly.io/blog/code-and-let-live/)

Kurt Mackey 认为，瞬时只读的沙盒对于 AI 智能体来说已经过时，他提出 Fly.io 新推出的“Sprites”是一个更优越的替代方案。Sprites 是持久的、可在 1-2 秒内即时创建的 Linux 微虚拟机，提供带有 100GB 存储的 root shell。它们在不同会话之间保留状态和已安装的软件，即使长时间不活动也是如此，并具有快速、随意的检查点/恢复功能（大约 1 秒），这类似于 Git 对整个系统的操作。

Sprites 的设计旨在经济实惠，在空闲时停止计费，并与 Fly.io 的 Anycast 网络集成以实现 HTTPS 访问，使用户能够轻松管理数百个 Sprites。Mackey 认为，AI 智能体（如“Claude”）需要具有持久存储和持久性的真正“计算机”，而不是无状态容器。当前的沙盒迫使智能体采用低效的变通方法，例如反复重建环境、依赖外部状态存储或将状态编码到“计划文件”中，这限制了它们的能力，使其只能执行短期任务。

作者设想了一个未来，个人可以利用 Sprites 等持久机器上的智能体来构建和拥有解决特定问题的应用程序，从而模糊了开发与生产之间的界限（“开发即生产，生产即开发”）。他认为沙盒正在阻碍这一演进，而 Sprites 提供的“一次性云计算机”范式标志着瞬时沙盒时代的终结。

---

## 9. Open Chaos: A self-evolving open-source project

**原文标题**: Open Chaos: A self-evolving open-source project

**原文链接**: [https://www.openchaos.dev/](https://www.openchaos.dev/)

生成摘要时出错

---

## 10. Exercise can be nearly as effective as therapy for depression

**原文标题**: Exercise can be nearly as effective as therapy for depression

**原文链接**: [https://www.sciencedaily.com/releases/2026/01/260107225516.htm](https://www.sciencedaily.com/releases/2026/01/260107225516.htm)

生成摘要时出错

---

## 11. Don't fall into the anti-AI hype

**原文标题**: Don't fall into the anti-AI hype

**原文链接**: [https://antirez.com/news/158](https://antirez.com/news/158)

生成摘要时出错

---

## 12. JavaScript Demos in 140 Characters

**原文标题**: JavaScript Demos in 140 Characters

**原文链接**: [https://beta.dwitter.net](https://beta.dwitter.net)

生成摘要时出错

---

## 13. Microsoft May Have Created the Slowest Windows in 25 Years with Windows 11

**原文标题**: Microsoft May Have Created the Slowest Windows in 25 Years with Windows 11

**原文链接**: [https://www.eteknix.com/microsoft-may-have-created-the-slowest-windows-in-25-years-with-windows-11/](https://www.eteknix.com/microsoft-may-have-created-the-slowest-windows-in-25-years-with-windows-11/)

生成摘要时出错

---

## 14. Oh My Zsh adds bloat

**原文标题**: Oh My Zsh adds bloat

**原文链接**: [https://rushter.com/blog/zsh-shell/](https://rushter.com/blog/zsh-shell/)

生成摘要时出错

---

## 15. AI is a business model stress test

**原文标题**: AI is a business model stress test

**原文链接**: [https://dri.es/ai-is-a-business-model-stress-test](https://dri.es/ai-is-a-business-model-stress-test)

生成摘要时出错

---

## 16. New information extracted from Snowden PDFs through metadata version analysis

**原文标题**: New information extracted from Snowden PDFs through metadata version analysis

**原文链接**: [https://libroot.org/posts/going-through-snowden-documents-part-4/](https://libroot.org/posts/going-through-snowden-documents-part-4/)

生成摘要时出错

---

## 17. UK government exempting itself from cyber law inspires little confidence

**原文标题**: UK government exempting itself from cyber law inspires little confidence

**原文链接**: [https://www.theregister.com/2026/01/10/csr_bill_analysis/](https://www.theregister.com/2026/01/10/csr_bill_analysis/)

生成摘要时出错

---

## 18. Private equity firms acquired more than 500 autism centers in past decade: study

**原文标题**: Private equity firms acquired more than 500 autism centers in past decade: study

**原文链接**: [https://www.brown.edu/news/2026-01-07/private-equity-autism-centers](https://www.brown.edu/news/2026-01-07/private-equity-autism-centers)

生成摘要时出错

---

## 19. RTX 5090 and Raspberry Pi: Can it game?

**原文标题**: RTX 5090 and Raspberry Pi: Can it game?

**原文链接**: [https://scottjg.com/posts/2026-01-08-crappy-computer-showdown/](https://scottjg.com/posts/2026-01-08-crappy-computer-showdown/)

生成摘要时出错

---

## 20. Start your meetings at 5 minutes past

**原文标题**: Start your meetings at 5 minutes past

**原文链接**: [https://philipotoole.com/start-your-meetings-at-5-minutes-past/](https://philipotoole.com/start-your-meetings-at-5-minutes-past/)

生成摘要时出错

---

## 21. Org Mode Syntax Is One of the Most Reasonable Markup Languages for Text (2017)

**原文标题**: Org Mode Syntax Is One of the Most Reasonable Markup Languages for Text (2017)

**原文链接**: [https://karl-voit.at/2017/09/23/orgmode-as-markup-only/](https://karl-voit.at/2017/09/23/orgmode-as-markup-only/)

生成摘要时出错

---

## 22. Gentoo Linux 2025 Review

**原文标题**: Gentoo Linux 2025 Review

**原文链接**: [https://www.gentoo.org/news/2026/01/05/new-year.html](https://www.gentoo.org/news/2026/01/05/new-year.html)

生成摘要时出错

---

## 23. My Home Fibre Network Disintegrated

**原文标题**: My Home Fibre Network Disintegrated

**原文链接**: [https://alienchow.dev/post/fibre_disintegration/](https://alienchow.dev/post/fibre_disintegration/)

生成摘要时出错

---

## 24. Show HN: Ferrite – Markdown editor in Rust with native Mermaid diagram rendering

**原文标题**: Show HN: Ferrite – Markdown editor in Rust with native Mermaid diagram rendering

**原文链接**: [https://github.com/OlaProeis/Ferrite](https://github.com/OlaProeis/Ferrite)

生成摘要时出错

---

## 25. Video filmed by ICE agent who shot Minneapolis woman emerges

**原文标题**: Video filmed by ICE agent who shot Minneapolis woman emerges

**原文链接**: [https://www.bbc.com/news/articles/cz7yv4524gqo](https://www.bbc.com/news/articles/cz7yv4524gqo)

生成摘要时出错

---

## 26. Overdose deaths are falling in America because of a 'supply shock': study

**原文标题**: Overdose deaths are falling in America because of a 'supply shock': study

**原文链接**: [https://www.economist.com/united-states/2026/01/08/why-overdose-deaths-are-falling-in-america](https://www.economist.com/united-states/2026/01/08/why-overdose-deaths-are-falling-in-america)

生成摘要时出错

---

## 27. The Concise TypeScript Book

**原文标题**: The Concise TypeScript Book

**原文链接**: [https://github.com/gibbok/typescript-book](https://github.com/gibbok/typescript-book)

生成摘要时出错

---

## 28. A battle over Canada’s mystery brain disease

**原文标题**: A battle over Canada’s mystery brain disease

**原文链接**: [https://www.bbc.com/news/articles/c623r47d67lo](https://www.bbc.com/news/articles/c623r47d67lo)

生成摘要时出错

---

## 29. Drones that recharge directly on transmission lines

**原文标题**: Drones that recharge directly on transmission lines

**原文链接**: [https://www.ycombinator.com/companies/voltair](https://www.ycombinator.com/companies/voltair)

生成摘要时出错

---

## 30. Iran Shuts Down Starlink Internet for First Time

**原文标题**: Iran Shuts Down Starlink Internet for First Time

**原文链接**: [https://www.forbes.com/sites/zakdoffman/2026/01/11/kill-switch-iran-shuts-down-starlink-internet-for-first-time/](https://www.forbes.com/sites/zakdoffman/2026/01/11/kill-switch-iran-shuts-down-starlink-internet-for-first-time/)

生成摘要时出错

---

## 31. OLED, Not for Me

**原文标题**: OLED, Not for Me

**原文链接**: [https://nuxx.net/blog/2026/01/09/oled-not-for-me/](https://nuxx.net/blog/2026/01/09/oled-not-for-me/)

生成摘要时出错

---

## 32. Workers at Redmond SpaceX lab exposed to toxic chemicals

**原文标题**: Workers at Redmond SpaceX lab exposed to toxic chemicals

**原文链接**: [https://www.fox13seattle.com/video/fmc-w1ga4pk97gxq0hj5](https://www.fox13seattle.com/video/fmc-w1ga4pk97gxq0hj5)

生成摘要时出错

---

## 33. Show HN: Rocket Launch and Orbit Simulator

**原文标题**: Show HN: Rocket Launch and Orbit Simulator

**原文链接**: [https://www.donutthejedi.com/](https://www.donutthejedi.com/)

生成摘要时出错

---

## 34. Show HN: Play poker with LLMs, or watch them play against each other

**原文标题**: Show HN: Play poker with LLMs, or watch them play against each other

**原文链接**: [https://llmholdem.com/](https://llmholdem.com/)

生成摘要时出错

---

## 35. Instagram data breach reportedly exposed the personal info of 17.5M users

**原文标题**: Instagram data breach reportedly exposed the personal info of 17.5M users

**原文链接**: [https://www.engadget.com/cybersecurity/an-instagram-data-breach-reportedly-exposed-the-personal-info-of-175-million-users-192105616.html](https://www.engadget.com/cybersecurity/an-instagram-data-breach-reportedly-exposed-the-personal-info-of-175-million-users-192105616.html)

生成摘要时出错

---

## 36. Max Payne – two decades later – Graphics Critique (2021)

**原文标题**: Max Payne – two decades later – Graphics Critique (2021)

**原文链接**: [https://darkcephas.blogspot.com/2021/07/max-payne-two-decades-later-graphics.html](https://darkcephas.blogspot.com/2021/07/max-payne-two-decades-later-graphics.html)

生成摘要时出错

---

## 37. Bob Weir has died

**原文标题**: Bob Weir has died

**原文链接**: [https://www.rollingstone.com/music/music-news/bob-weir-grateful-dead-dead-obituary-1234810106/](https://www.rollingstone.com/music/music-news/bob-weir-grateful-dead-dead-obituary-1234810106/)

生成摘要时出错

---

## 38. NASA announces unprecedented return of sick ISS astronaut and crew

**原文标题**: NASA announces unprecedented return of sick ISS astronaut and crew

**原文链接**: [https://www.livescience.com/space/space-exploration/nasa-cancels-spacewalk-and-considers-early-crew-return-from-iss-due-to-medical-issues](https://www.livescience.com/space/space-exploration/nasa-cancels-spacewalk-and-considers-early-crew-return-from-iss-due-to-medical-issues)

生成摘要时出错

---

## 39. UK Orders Ofcom to Explore Encryption Backdoors

**原文标题**: UK Orders Ofcom to Explore Encryption Backdoors

**原文链接**: [https://reclaimthenet.org/uk-orders-ofcom-to-explore-encryption-backdoors](https://reclaimthenet.org/uk-orders-ofcom-to-explore-encryption-backdoors)

生成摘要时出错

---

## 40. You are not required to close your <p>, <li>, <img>, or <br> tags in HTML

**原文标题**: You are not required to close your <p>, <li>, <img>, or <br> tags in HTML

**原文链接**: [https://blog.novalistic.com/archives/2017/08/optional-end-tags-in-html/](https://blog.novalistic.com/archives/2017/08/optional-end-tags-in-html/)

生成摘要时出错

---

## 41. Why Is Greenland Part of the Kingdom of Denmark? A Short History

**原文标题**: Why Is Greenland Part of the Kingdom of Denmark? A Short History

**原文链接**: [https://www.diis.dk/en/research/why-is-greenland-part-of-the-kingdom-of-denmark-a-short-history](https://www.diis.dk/en/research/why-is-greenland-part-of-the-kingdom-of-denmark-a-short-history)

生成摘要时出错

---

## 42. Worst of breed software

**原文标题**: Worst of breed software

**原文链接**: [https://worstofbreed.net/](https://worstofbreed.net/)

生成摘要时出错

---

## 43. CDC staff 'blindsided' as child vaccine schedule unilaterally overhauled

**原文标题**: CDC staff 'blindsided' as child vaccine schedule unilaterally overhauled

**原文链接**: [https://www.unmc.edu/healthsecurity/transmission/2026/01/07/cdc-staff-blindsided-as-child-vaccine-schedule-unilaterally-overhauled/](https://www.unmc.edu/healthsecurity/transmission/2026/01/07/cdc-staff-blindsided-as-child-vaccine-schedule-unilaterally-overhauled/)

生成摘要时出错

---

## 44. Poison Fountain

**原文标题**: Poison Fountain

**原文链接**: [https://rnsaffn.com/poison3/](https://rnsaffn.com/poison3/)

生成摘要时出错

---

## 45. A Year of Work on the Arch Linux Package Management (ALPM) Project

**原文标题**: A Year of Work on the Arch Linux Package Management (ALPM) Project

**原文链接**: [https://devblog.archlinux.page/2026/a-year-of-work-on-the-alpm-project/](https://devblog.archlinux.page/2026/a-year-of-work-on-the-alpm-project/)

生成摘要时出错

---

## 46. I got paid minimum wage to solve an impossible problem

**原文标题**: I got paid minimum wage to solve an impossible problem

**原文链接**: [https://tiespetersen.substack.com/p/i-got-paid-minimum-wage-to-solve](https://tiespetersen.substack.com/p/i-got-paid-minimum-wage-to-solve)

生成摘要时出错

---

## 47. All my new code will be closed-source from now on

**原文标题**: All my new code will be closed-source from now on

**原文链接**: [https://twitter.com/MarcJSchmidt/status/2009688028931875156](https://twitter.com/MarcJSchmidt/status/2009688028931875156)

生成摘要时出错

---

## 48. Think of Pavlov

**原文标题**: Think of Pavlov

**原文链接**: [https://boz.com/articles/think-pavlov](https://boz.com/articles/think-pavlov)

生成摘要时出错

---

## 49. Rats caught on camera hunting flying bats (2025)

**原文标题**: Rats caught on camera hunting flying bats (2025)

**原文链接**: [https://scienceclock.com/rats-caught-on-camera-hunting-flying-bats-for-the-first-time/](https://scienceclock.com/rats-caught-on-camera-hunting-flying-bats-for-the-first-time/)

生成摘要时出错

---

## 50. Code Is Clay

**原文标题**: Code Is Clay

**原文链接**: [https://campedersen.com/code-is-clay](https://campedersen.com/code-is-clay)

生成摘要时出错

---

## 51. Turn a single image into a navigable 3D Gaussian Splat with depth

**原文标题**: Turn a single image into a navigable 3D Gaussian Splat with depth

**原文链接**: [https://lab.revelium.studio/ml-sharp](https://lab.revelium.studio/ml-sharp)

生成摘要时出错

---

## 52. Circumcision classed as possible child abuse in draft CPS document

**原文标题**: Circumcision classed as possible child abuse in draft CPS document

**原文链接**: [https://www.theguardian.com/society/2026/jan/10/circumcision-classed-as-possible-child-abuse-in-draft-cps-document](https://www.theguardian.com/society/2026/jan/10/circumcision-classed-as-possible-child-abuse-in-draft-cps-document)

生成摘要时出错

---

## 53. More than one hundred years of Film Sizes

**原文标题**: More than one hundred years of Film Sizes

**原文链接**: [https://wichm.home.xs4all.nl/filmsize.html](https://wichm.home.xs4all.nl/filmsize.html)

生成摘要时出错

---

## 54. Washington National Opera Is Leaving the Kennedy Center

**原文标题**: Washington National Opera Is Leaving the Kennedy Center

**原文链接**: [https://www.nytimes.com/2026/01/09/arts/music/washington-national-opera-kennedy-center.html](https://www.nytimes.com/2026/01/09/arts/music/washington-national-opera-kennedy-center.html)

生成摘要时出错

---

## 55. Iran's internet shutdown is chillingly precise and may last some time

**原文标题**: Iran's internet shutdown is chillingly precise and may last some time

**原文链接**: [https://www.theguardian.com/world/2026/jan/10/irans-internet-shutdown-is-strikingly-sophisticated-and-may-last-some-time](https://www.theguardian.com/world/2026/jan/10/irans-internet-shutdown-is-strikingly-sophisticated-and-may-last-some-time)

生成摘要时出错

---

## 56. Datadog, thank you for blocking us

**原文标题**: Datadog, thank you for blocking us

**原文链接**: [https://www.deductive.ai/blogs/datadog-thank-you-for-blocking-us](https://www.deductive.ai/blogs/datadog-thank-you-for-blocking-us)

生成摘要时出错

---

## 57. Deno has made its PyPI distribution official

**原文标题**: Deno has made its PyPI distribution official

**原文链接**: [https://github.com/denoland/deno/issues/31254](https://github.com/denoland/deno/issues/31254)

生成摘要时出错

---

## 58. Show HN: EuConform – Offline-first EU AI Act compliance tool (open source)

**原文标题**: Show HN: EuConform – Offline-first EU AI Act compliance tool (open source)

**原文链接**: [https://github.com/Hiepler/EuConform](https://github.com/Hiepler/EuConform)

生成摘要时出错

---

## 59. HTML-only conditional lazy loading (via preload and media)

**原文标题**: HTML-only conditional lazy loading (via preload and media)

**原文链接**: [https://orga.cat/blog/html-conditional-lazy-loading/](https://orga.cat/blog/html-conditional-lazy-loading/)

生成摘要时出错

---

## 60. HTML-only conditional lazy loading (via preload and media)

**原文标题**: HTML-only conditional lazy loading (via preload and media)

**原文链接**: [https://orga.cat/blog/html-conditional-lazy-loading/](https://orga.cat/blog/html-conditional-lazy-loading/)

生成摘要时出错

---

## 61. Caltrain shows why every region should be moving toward regional rail

**原文标题**: Caltrain shows why every region should be moving toward regional rail

**原文链接**: [https://www.hsrail.org/blog/caltrain-shows-why-every-region-should-be-moving-toward-regional-rail/](https://www.hsrail.org/blog/caltrain-shows-why-every-region-should-be-moving-toward-regional-rail/)

生成摘要时出错

---

## 62. Iranian regime tries to shut down Starlink

**原文标题**: Iranian regime tries to shut down Starlink

**原文链接**: [https://www.timesofisrael.com/iran-appears-to-jam-starlink-after-shutting-down-comms-networks/](https://www.timesofisrael.com/iran-appears-to-jam-starlink-after-shutting-down-comms-networks/)

生成摘要时出错

---

## 63. Landlords are using automated services to monitor tenant promotions

**原文标题**: Landlords are using automated services to monitor tenant promotions

**原文链接**: [https://old.reddit.com/r/shitrentals/comments/1q38sh4/if_you_get_promoted_at_work_keep_it_a_secret_from/](https://old.reddit.com/r/shitrentals/comments/1q38sh4/if_you_get_promoted_at_work_keep_it_a_secret_from/)

生成摘要时出错

---

## 64. Google: Don't make "bite-sized" content for LLMs

**原文标题**: Google: Don't make "bite-sized" content for LLMs

**原文链接**: [https://arstechnica.com/google/2026/01/google-dont-make-bite-sized-content-for-llms-if-you-care-about-search-rank/](https://arstechnica.com/google/2026/01/google-dont-make-bite-sized-content-for-llms-if-you-care-about-search-rank/)

生成摘要时出错

---

## 65. BasiliskII Macintosh 68k Emulator Ported to ESP32-P4 / M5Stack Tab5

**原文标题**: BasiliskII Macintosh 68k Emulator Ported to ESP32-P4 / M5Stack Tab5

**原文链接**: [https://github.com/amcchord/M5Tab-Macintosh](https://github.com/amcchord/M5Tab-Macintosh)

生成摘要时出错

---

## 66. Extracting books from production language models (2026)

**原文标题**: Extracting books from production language models (2026)

**原文链接**: [https://arxiv.org/abs/2601.02671](https://arxiv.org/abs/2601.02671)

生成摘要时出错

---

## 67. My mouse stopped working because Logitech's servers went down

**原文标题**: My mouse stopped working because Logitech's servers went down

**原文链接**: [https://old.reddit.com/r/logitech/comments/1q621k6/logi_options_is_down/](https://old.reddit.com/r/logitech/comments/1q621k6/logi_options_is_down/)

生成摘要时出错

---

## 68. Iran's complete Internet shutdown reaches 24 hours

**原文标题**: Iran's complete Internet shutdown reaches 24 hours

**原文链接**: [https://mastodon.social/@netblocks/115866066884567356](https://mastodon.social/@netblocks/115866066884567356)

生成摘要时出错

---

## 69. Linus Torvalds Uses Google Antigravity

**原文标题**: Linus Torvalds Uses Google Antigravity

**原文链接**: [https://github.com/torvalds/AudioNoise/blob/main/README.md](https://github.com/torvalds/AudioNoise/blob/main/README.md)

生成摘要时出错

---

## 70. Replace the Retiring Windows XP with Linux (2014)

**原文标题**: Replace the Retiring Windows XP with Linux (2014)

**原文链接**: [https://www.linux.com/training-tutorials/replace-retiring-windows-xp-linux/](https://www.linux.com/training-tutorials/replace-retiring-windows-xp-linux/)

生成摘要时出错

---

## 71. YouTube has removed the ability to search by upload date

**原文标题**: YouTube has removed the ability to search by upload date

**原文链接**: [https://twitter.com/TeamYouTube/status/2009744367834022320](https://twitter.com/TeamYouTube/status/2009744367834022320)

生成摘要时出错

---

## 72. Bichon: A lightweight, high-performance Rust email archiver with WebUI

**原文标题**: Bichon: A lightweight, high-performance Rust email archiver with WebUI

**原文链接**: [https://github.com/rustmailer/bichon](https://github.com/rustmailer/bichon)

生成摘要时出错

---

## 73. Former Google CEO Eric Schmidt accused of rape, surveillance by ex-mistress

**原文标题**: Former Google CEO Eric Schmidt accused of rape, surveillance by ex-mistress

**原文链接**: [https://www.news.com.au/world/north-america/former-google-ceo-eric-schmidt-accused-of-rape-surveillance-by-exmistress/news-story/cc5947d2828ec3dc7a343ebec5a33151](https://www.news.com.au/world/north-america/former-google-ceo-eric-schmidt-accused-of-rape-surveillance-by-exmistress/news-story/cc5947d2828ec3dc7a343ebec5a33151)

生成摘要时出错

---

## 74. Tim Cook and Sundar Pichai are cowards

**原文标题**: Tim Cook and Sundar Pichai are cowards

**原文链接**: [https://www.theverge.com/policy/859902/apple-google-run-by-cowards](https://www.theverge.com/policy/859902/apple-google-run-by-cowards)

生成摘要时出错

---

## 75. US oil giant ExxonMobil says Venezuela is 'uninvestable'

**原文标题**: US oil giant ExxonMobil says Venezuela is 'uninvestable'

**原文链接**: [https://www.ft.com/content/4c21c031-443e-4834-a7a6-3dd59672b54e](https://www.ft.com/content/4c21c031-443e-4834-a7a6-3dd59672b54e)

生成摘要时出错

---

## 76. Tesla's Germany Sales Down 72% from Their Peak

**原文标题**: Tesla's Germany Sales Down 72% from Their Peak

**原文链接**: [https://cleantechnica.com/2026/01/08/teslas-germany-sales-down-72-from-their-peak/](https://cleantechnica.com/2026/01/08/teslas-germany-sales-down-72-from-their-peak/)

生成摘要时出错

---

## 77. See it with your lying ears

**原文标题**: See it with your lying ears

**原文链接**: [https://lcamtuf.substack.com/p/see-it-with-your-lying-ears](https://lcamtuf.substack.com/p/see-it-with-your-lying-ears)

生成摘要时出错

---

## 78. Happy 50th Birthday KIM-1

**原文标题**: Happy 50th Birthday KIM-1

**原文链接**: [https://github.com/netzherpes/KIM1-Demo](https://github.com/netzherpes/KIM1-Demo)

生成摘要时出错

---

## 79. Linus is vibe coding

**原文标题**: Linus is vibe coding

**原文链接**: [https://github.com/torvalds/AudioNoise](https://github.com/torvalds/AudioNoise)

生成摘要时出错

---

## 80. Tux Paint

**原文标题**: Tux Paint

**原文链接**: [https://tuxpaint.org/](https://tuxpaint.org/)

生成摘要时出错

---

## 81. OpenAI is reportedly asking contractors to upload real work from past jobs

**原文标题**: OpenAI is reportedly asking contractors to upload real work from past jobs

**原文链接**: [https://techcrunch.com/2026/01/10/openai-is-reportedly-asking-contractors-to-upload-real-work-from-past-jobs/](https://techcrunch.com/2026/01/10/openai-is-reportedly-asking-contractors-to-upload-real-work-from-past-jobs/)

生成摘要时出错

---

## 82. "We write to ask that you enforce your app stores' terms of service against X" [pdf]

**原文标题**: "We write to ask that you enforce your app stores' terms of service against X" [pdf]

**原文链接**: [https://www.wyden.senate.gov/imo/media/doc/letter_to_apple_and_google_on_removing_x_and_grok_from_app_store_192026pdf.pdf](https://www.wyden.senate.gov/imo/media/doc/letter_to_apple_and_google_on_removing_x_and_grok_from_app_store_192026pdf.pdf)

生成摘要时出错

---

## 83. USDA suspends federal financial awards to Minnesota and Minneapolis

**原文标题**: USDA suspends federal financial awards to Minnesota and Minneapolis

**原文链接**: [https://turnto10.com/news/nation-world/enough-is-enough-usda-suspends-federal-financial-awards-to-minnesota-and-minneapolis-fraud-scheme-investigation-governor-tim-walz-mayor-jacob-frey-nick-shirley-feeding-our-children-food-programs](https://turnto10.com/news/nation-world/enough-is-enough-usda-suspends-federal-financial-awards-to-minnesota-and-minneapolis-fraud-scheme-investigation-governor-tim-walz-mayor-jacob-frey-nick-shirley-feeding-our-children-food-programs)

生成摘要时出错

---

## 84. QtNat – Open you port with Qt UPnP

**原文标题**: QtNat – Open you port with Qt UPnP

**原文链接**: [http://renaudguezennec.eu/index.php/2026/01/09/qtnat-open-you-port-with-qt/](http://renaudguezennec.eu/index.php/2026/01/09/qtnat-open-you-port-with-qt/)

生成摘要时出错

---

## 85. Sisyphus Now Lives in Oh My Claude

**原文标题**: Sisyphus Now Lives in Oh My Claude

**原文链接**: [https://github.com/Yeachan-Heo/oh-my-claude-sisyphus](https://github.com/Yeachan-Heo/oh-my-claude-sisyphus)

生成摘要时出错

---

## 86. Sigmund Freud's Begonia

**原文标题**: Sigmund Freud's Begonia

**原文链接**: [https://observer.co.uk/news/first-person/article/emma-freud-sigmund-freuds-begonia](https://observer.co.uk/news/first-person/article/emma-freud-sigmund-freuds-begonia)

生成摘要时出错

---

## 87. 'F*ck You, Make Me' Without Saying the Words

**原文标题**: 'F*ck You, Make Me' Without Saying the Words

**原文链接**: [https://daringfireball.net/2026/01/fuck_you_make_me_without_saying_the_words](https://daringfireball.net/2026/01/fuck_you_make_me_without_saying_the_words)

生成摘要时出错

---

## 88. Why Are Federal Agents Using GoPros, Smart Glasses, and Phones to Record Us?

**原文标题**: Why Are Federal Agents Using GoPros, Smart Glasses, and Phones to Record Us?

**原文链接**: [https://gizmodo.com/why-are-federal-agents-using-gopros-smart-glasses-and-phones-to-record-us-2000707835](https://gizmodo.com/why-are-federal-agents-using-gopros-smart-glasses-and-phones-to-record-us-2000707835)

生成摘要时出错

---

## 89. Ripple: The Elegant TypeScript UI Framework

**原文标题**: Ripple: The Elegant TypeScript UI Framework

**原文链接**: [https://jsdev.space/meet-ripple/](https://jsdev.space/meet-ripple/)

生成摘要时出错

---

## 90. Show HN: VAM Seek – 2D video navigation grid, 15KB, zero server load

**原文标题**: Show HN: VAM Seek – 2D video navigation grid, 15KB, zero server load

**原文链接**: [https://github.com/unhaya/vam-seek](https://github.com/unhaya/vam-seek)

生成摘要时出错

---

## 91. LLMs have burned Billions but couldn't build another Tailwind

**原文标题**: LLMs have burned Billions but couldn't build another Tailwind

**原文链接**: [https://omarabid.com/tailwind-ai](https://omarabid.com/tailwind-ai)

生成摘要时出错

---

## 92. Many small queries are efficient in SQLite

**原文标题**: Many small queries are efficient in SQLite

**原文链接**: [https://sqlite.org/np1queryprob.html](https://sqlite.org/np1queryprob.html)

生成摘要时出错

---

## 93. FFmpeg 8.0

**原文标题**: FFmpeg 8.0

**原文链接**: [https://ayosec.github.io/ffmpeg-filters-docs/](https://ayosec.github.io/ffmpeg-filters-docs/)

生成摘要时出错

---

## 94. Microsoft revealed as company behind controversial data center proposal in MI

**原文标题**: Microsoft revealed as company behind controversial data center proposal in MI

**原文链接**: [https://www.cnbc.com/2026/01/07/microsoft-behind-controversial-data-center-in-michigan-township.html](https://www.cnbc.com/2026/01/07/microsoft-behind-controversial-data-center-in-michigan-township.html)

生成摘要时出错

---

## 95. Collection and Use of Biometrics by U.S. Citizenship and Immigration Services

**原文标题**: Collection and Use of Biometrics by U.S. Citizenship and Immigration Services

**原文链接**: [https://www.federalregister.gov/documents/2025/11/03/2025-19747/collection-and-use-of-biometrics-by-us-citizenship-and-immigration-services](https://www.federalregister.gov/documents/2025/11/03/2025-19747/collection-and-use-of-biometrics-by-us-citizenship-and-immigration-services)

生成摘要时出错

---

## 96. Datadog, thank you for blocking us

**原文标题**: Datadog, thank you for blocking us

**原文链接**: [https://www.deductive.ai/blogs/datadog-thank-you-for-blocking-us](https://www.deductive.ai/blogs/datadog-thank-you-for-blocking-us)

生成摘要时出错

---

## 97. Sinclair C5

**原文标题**: Sinclair C5

**原文链接**: [https://en.wikipedia.org/wiki/Sinclair_C5](https://en.wikipedia.org/wiki/Sinclair_C5)

生成摘要时出错

---

## 98. What Claude Code Sends to the Cloud

**原文标题**: What Claude Code Sends to the Cloud

**原文链接**: [https://rastrigin.systems/blog/claude-code-part-1-requests/](https://rastrigin.systems/blog/claude-code-part-1-requests/)

生成摘要时出错

---

## 99. Looking for flagged discussions on HN? See what's active

**原文标题**: Looking for flagged discussions on HN? See what's active

**原文链接**: [https://news.ycombinator.com/active](https://news.ycombinator.com/active)

生成摘要时出错

---

## 100. Court rejects NVIDIAs attempt to seal email chain with Annas Archive [pdf]

**原文标题**: Court rejects NVIDIAs attempt to seal email chain with Annas Archive [pdf]

**原文链接**: [https://storage.courtlistener.com/recap/gov.uscourts.cand.426191/gov.uscourts.cand.426191.222.0.pdf](https://storage.courtlistener.com/recap/gov.uscourts.cand.426191/gov.uscourts.cand.426191.222.0.pdf)

生成摘要时出错

---

