# Hacker News 热门文章摘要 (2026-01-12)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 在 macOS Tahoe 上调整窗口大小的挣扎

**原文标题**: The struggle of resizing windows on macOS Tahoe

**原文链接**: [https://noheger.at/blog/2026/01/11/the-struggle-of-resizing-windows-on-macos-tahoe/](https://noheger.at/blog/2026/01/11/the-struggle-of-resizing-windows-on-macos-tahoe/)

文章批评macOS Tahoe“大得离谱”的窗口圆角半径，认为其不仅在美学上令人不悦，更重要的是损害了可用性。作为一名资深电脑用户，作者指出自升级以来，调整窗口大小变得异常困难。

这种困难源于macOS窗口期望调整大小的点击发生在角落附近一个19x19像素的目标区域内。在之前具有尖角的macOS版本中，该区域的62%都位于可见窗口内部。然而，由于Tahoe版本显著的圆角设计，这个关键目标区域的75%现在位于可见窗口边界*之外*。

用户本能地试图在窗口可见形状*内部*抓取其角落，这是一个与人们物理抓取物体方式相符的自然动作。然而，在Tahoe中，这些直观的点击点却经常落在被接受的调整大小区域之外，导致尝试失败。矛盾的是，在Tahoe中调整窗口大小最可靠的方法是点击并拖动可见角落*之外*的区域。这种所需的操作手势令人感觉不自然、反直觉，并且最终容易出错，由于这一设计选择，将一个基本的计算任务变成了一种令人沮丧的体验。

---

## 2. 别陷入反AI炒作

**原文标题**: Don't fall into the anti-AI hype

**原文链接**: [https://antirez.com/news/158](https://antirez.com/news/158)

别陷入反AI炒作

---

## 3. 我抛弃了 Windows 11 转投 Linux，你也应该。

**原文标题**: I dumped Windows 11 for Linux, and you should too

**原文链接**: [https://www.notebookcheck.net/I-dumped-Windows-11-for-Linux-and-you-should-too.1190961.0.html](https://www.notebookcheck.net/I-dumped-Windows-11-for-Linux-and-you-should-too.1190961.0.html)

生成摘要时出错

---

## 4. 杰罗姆·鲍威尔声明

**原文标题**: Statement from Jerome Powell

**原文链接**: [https://www.federalreserve.gov/newsevents/speech/powell20260111a.htm](https://www.federalreserve.gov/newsevents/speech/powell20260111a.htm)

2026年1月11日，美联储主席杰罗姆·H·鲍威尔宣布，司法部已向他发出大陪审团传票，威胁对其进行刑事起诉。此次行动的公开理由与他去年六月在参议院银行委员会前的证词有关，该证词涉及美联储办公大楼的一项翻修项目。

鲍威尔在申明他尊重法治的同时，将此描述为“前所未有的行动”，并将其置于本届政府威胁和施压的更广泛背景下看待。他明确指出，刑事指控的威胁并非真正与他的证词或翻修工程有关，他认为这些都是“借口”。

相反，鲍威尔认为此举是美联储根据经济证据和公共服务独立设定利率，而非遵循总统偏好所导致的结果。他将此局面视为对美联储在不受政治压力或恐吓的情况下执行货币政策能力的一项严峻挑战。

鲍威尔曾在多届政府任职，他重申将秉持职责，不惧政治影响，不偏不倚，只专注于美联储物价稳定和最大就业的双重使命。他誓言，尽管面临威胁，仍将诚信地继续为美国人民服务。

---

## 5. CLI agents make self-hosting on a home server easier and fun

**原文标题**: CLI agents make self-hosting on a home server easier and fun

**原文链接**: [https://fulghum.io/self-hosting](https://fulghum.io/self-hosting)

Jordan Fulghum declares 2026 the "Year of Self-hosting," citing how CLI agents like Claude Code, combined with cheap mini PCs and Tailscale, have made it dramatically easier and fun. Previously deterred by complex configurations, the author now recommends self-hosting to software-literate individuals who don't want to become sysadmins.

The transformation stems from installing Claude Code directly on a low-power Linux box (e.g., Beelink Mini N150). Instead of manual Docker, Compose, or reverse proxy setups, the author simply describes desired outcomes to Claude Code, which then automates tasks like Docker installation, service deployment (Vaultwarden, Plex, Immich, Uptime Kuma, Readeck, Home Assistant), Caddy configuration, data persistence, updates, security, and automatic restarts.

This setup replaced core services with self-hosted alternatives, offering control and peace of mind. For example, Vaultwarden replaced Bitwarden, Immich served as a Google Photos alternative, and Readeck filled a "read-it-later" void. The system also includes a custom monitoring dashboard and automated backups to local drives and AWS S3 Glacier.

The author emphasizes the powerful feeling of ownership and independence, enabling time spent *using* and *learning* software rather than stressing over maintenance. This approach is ideal for those comfortable with a terminal, currently paying for SaaS tools, and curious about how things work, but who wish to avoid becoming infra experts. For the first time, self-hosting is presented as not just viable, but genuinely fun.

---

## 6. 发现并修复 Ghostty 的最大内存泄漏

**原文标题**: Finding and fixing Ghostty's largest memory leak

**原文链接**: [https://mitchellh.com/writing/ghostty-memory-leak-fix](https://mitchellh.com/writing/ghostty-memory-leak-fix)

Ghostty，一个终端模拟器，正遭受严重的内存泄漏问题，有用户报告内存占用高达37 GB。这个自Ghostty 1.0版本以来就存在的漏洞，最近由于Claude Code等应用程序生成特定的输出模式而变得突出。

核心问题在于Ghostty的`PageList`内存管理。它使用一个内存页的双向链表，对标准大小的页采用内存池，而对更大的“非标准”页则使用`mmap`。一个关键的优化是当达到历史记录限制时，重用最旧的回滚页，以避免昂贵的重新分配。

这个漏洞发生在一个通过`mmap`直接分配的非标准页在回滚修剪期间被重用时。虽然页面的元数据被重置为标准大小，但底层的`mmap`分配并未调整大小。因此，当该页面随后被“释放”时，Ghostty的逻辑错误地认为它是一个标准池化页面，未能调用`munmap`，从而导致内存泄漏。Claude Code的命令行界面通过频繁生成多代码点字素输出加剧了这一问题，在高回滚场景中强制常规使用非标准页。

修复方案在概念上很简单：非标准页在回滚修剪期间不再被重用。相反，它们被正确地`munmap`，并从池中分配一个新的标准大小的页面。

在macOS上添加虚拟内存标签有助于诊断此泄漏，从而能够专门识别和监控PageList内存。尽管Ghostty具有各种泄漏检测机制（例如，泄漏检测分配器、Valgrind、Instruments），但这个特定的漏洞由于其非常具体的触发条件而避开了这些机制，现在这些条件已被新的测试覆盖。这是Ghostty报告过的最大内存泄漏，其解决凸显了真实世界复现场景对于诊断的重要性。

---

## 7. iCloud 照片下载器

**原文标题**: iCloud Photos Downloader

**原文链接**: [https://github.com/icloud-photos-downloader/icloud_photos_downloader](https://github.com/icloud-photos-downloader/icloud_photos_downloader)

iCloud照片下载器是一个跨平台命令行工具，用于下载所有iCloud照片，兼容Linux、Windows、macOS和NAS设备。它可以通过直接可执行文件获取，或通过Docker、PyPI、AUR和npm等包管理器进行安装。该项目由志愿者维护，正在积极寻找新的维护者，并目标是每周发布新版本。

为确保功能正常运行，用户必须配置其iCloud账户，启用“在网页上访问iCloud数据”并禁用“高级数据保护”，以避免出现`ACCESS_DENIED`错误。

该工具提供三种操作模式：“复制”（默认）模式，用于下载新照片；“同步”模式，用于下载新照片并移除iCloud中已删除的本地文件；以及“移动”模式，用于下载新照片然后将其从iCloud中删除。主要功能包括支持Live Photos和RAW图像、自动去重、一次性或持续监控选项，以及照片元数据（EXIF）更新。

安装方法包括下载预构建的可执行文件、使用包管理器或从源代码构建。示例用法包括使用`icloudpd --directory /data --username my@email.address --watch-with-interval 3600`进行持续同步，以及使用`--auth-only`进行独立会话认证。实验模式允许抢先体验新功能。欢迎贡献。

---

## 8. 软盘竟然是孩子们最棒的电视遥控器。

**原文标题**: Floppy disks turn out to be the greatest TV remote for kids

**原文链接**: [https://blog.smartere.dk/2026/01/floppy-disks-the-best-tv-remote-for-kids/](https://blog.smartere.dk/2026/01/floppy-disks-the-best-tv-remote-for-kids/)

生成摘要时出错

---

## 9. 美联储主席杰罗姆·F·鲍威尔声明 [视频]

**原文标题**: Statement by Federal Reserve Chair Jerome F. Powell [video]

**原文链接**: [https://www.youtube.com/watch?v=KckGHaBLSn4](https://www.youtube.com/watch?v=KckGHaBLSn4)

生成摘要时出错

---

## 10. Apple picks Google's Gemini to power Siri

**原文标题**: Apple picks Google's Gemini to power Siri

**原文链接**: [https://www.cnbc.com/2026/01/12/apple-google-ai-siri-gemini.html](https://www.cnbc.com/2026/01/12/apple-google-ai-siri-gemini.html)

Apple has officially partnered with Google, selecting its Gemini models and cloud technology to power a major AI-driven upgrade for Siri, expected later this year. This multiyear collaboration will also support Apple's future foundational models. Apple stated that Google's technology provides the "most capable foundation" for its AI initiatives.

The move signifies Apple's more aggressive entry into the AI landscape, having mostly stayed out of the recent "AI frenzy." This partnership aims to deliver an impressive Siri upgrade, addressing previous delays. While specific financial terms were not disclosed, earlier reports suggested Apple could pay Google around $1 billion annually.

This deal reinforces growing trust in Google's accelerating AI agenda and its comeback against competitors like OpenAI. Google already pays Apple billions annually for its search engine default status on iPhones and recently surpassed Apple in market capitalization.

The partnership's effect on Apple's existing integration of OpenAI's ChatGPT for complex Siri queries is currently unclear, though Apple stated it isn't making immediate changes to that agreement. Shares initially rose following the news before pulling back, with Google briefly touching a $4 trillion market value.

---

## 11. Gentoo Linux 2025 Review

**原文标题**: Gentoo Linux 2025 Review

**原文链接**: [https://www.gentoo.org/news/2026/01/05/new-year.html](https://www.gentoo.org/news/2026/01/05/new-year.html)

生成摘要时出错

---

## 12. Anthropic: Developing a Claude Code competitor using Claude Code is banned

**原文标题**: Anthropic: Developing a Claude Code competitor using Claude Code is banned

**原文链接**: [https://twitter.com/SIGKITTEN/status/2009697031422652461](https://twitter.com/SIGKITTEN/status/2009697031422652461)

生成摘要时出错

---

## 13. Private equity firms acquired more than 500 autism centers in past decade: study

**原文标题**: Private equity firms acquired more than 500 autism centers in past decade: study

**原文链接**: [https://www.brown.edu/news/2026-01-07/private-equity-autism-centers](https://www.brown.edu/news/2026-01-07/private-equity-autism-centers)

生成摘要时出错

---

## 14. Ozempic reduced grocery spending by an average of 5.3% in the US

**原文标题**: Ozempic reduced grocery spending by an average of 5.3% in the US

**原文链接**: [https://news.cornell.edu/stories/2025/12/ozempic-changing-foods-americans-buy](https://news.cornell.edu/stories/2025/12/ozempic-changing-foods-americans-buy)

生成摘要时出错

---

## 15. TimeCapsuleLLM: LLM trained only on data from 1800-1875

**原文标题**: TimeCapsuleLLM: LLM trained only on data from 1800-1875

**原文链接**: [https://github.com/haykgrigo3/TimeCapsuleLLM](https://github.com/haykgrigo3/TimeCapsuleLLM)

生成摘要时出错

---

## 16. Xfce is great

**原文标题**: Xfce is great

**原文链接**: [https://rubenerd.com/xfce-is-great/](https://rubenerd.com/xfce-is-great/)

生成摘要时出错

---

## 17. This game is a single 13 KiB file that runs on Windows, Linux and in the Browser

**原文标题**: This game is a single 13 KiB file that runs on Windows, Linux and in the Browser

**原文链接**: [https://iczelia.net/posts/snake-polyglot/](https://iczelia.net/posts/snake-polyglot/)

生成摘要时出错

---

## 18. The next two years of software engineering

**原文标题**: The next two years of software engineering

**原文链接**: [https://addyosmani.com/blog/next-two-years/](https://addyosmani.com/blog/next-two-years/)

生成摘要时出错

---

## 19. Meta announces nuclear energy projects

**原文标题**: Meta announces nuclear energy projects

**原文链接**: [https://about.fb.com/news/2026/01/meta-nuclear-energy-projects-power-american-ai-leadership/](https://about.fb.com/news/2026/01/meta-nuclear-energy-projects-power-american-ai-leadership/)

生成摘要时出错

---

## 20. My Home Fibre Network Disintegrated

**原文标题**: My Home Fibre Network Disintegrated

**原文链接**: [https://alienchow.dev/post/fibre_disintegration/](https://alienchow.dev/post/fibre_disintegration/)

生成摘要时出错

---

## 21. Show HN: Ferrite – Markdown editor in Rust with native Mermaid diagram rendering

**原文标题**: Show HN: Ferrite – Markdown editor in Rust with native Mermaid diagram rendering

**原文链接**: [https://github.com/OlaProeis/Ferrite](https://github.com/OlaProeis/Ferrite)

生成摘要时出错

---

## 22. Poison Fountain

**原文标题**: Poison Fountain

**原文链接**: [https://rnsaffn.com/poison3/](https://rnsaffn.com/poison3/)

生成摘要时出错

---

## 23. The Concise TypeScript Book

**原文标题**: The Concise TypeScript Book

**原文链接**: [https://github.com/gibbok/typescript-book](https://github.com/gibbok/typescript-book)

生成摘要时出错

---

## 24. BYD's cheapest electric cars to have Lidar self-driving tech

**原文标题**: BYD's cheapest electric cars to have Lidar self-driving tech

**原文链接**: [https://thedriven.io/2026/01/11/byds-cheapest-electric-cars-to-have-lidar-self-driving-tech/](https://thedriven.io/2026/01/11/byds-cheapest-electric-cars-to-have-lidar-self-driving-tech/)

生成摘要时出错

---

## 25. Overdose deaths are falling in America because of a 'supply shock': study

**原文标题**: Overdose deaths are falling in America because of a 'supply shock': study

**原文链接**: [https://www.economist.com/united-states/2026/01/08/why-overdose-deaths-are-falling-in-america](https://www.economist.com/united-states/2026/01/08/why-overdose-deaths-are-falling-in-america)

生成摘要时出错

---

## 26. Instagram data breach reportedly exposed the personal info of 17.5M users

**原文标题**: Instagram data breach reportedly exposed the personal info of 17.5M users

**原文链接**: [https://www.engadget.com/cybersecurity/an-instagram-data-breach-reportedly-exposed-the-personal-info-of-175-million-users-192105616.html](https://www.engadget.com/cybersecurity/an-instagram-data-breach-reportedly-exposed-the-personal-info-of-175-million-users-192105616.html)

生成摘要时出错

---

## 27. FUSE is All You Need – Giving agents access to anything via filesystems

**原文标题**: FUSE is All You Need – Giving agents access to anything via filesystems

**原文链接**: [https://jakobemmerling.de/posts/fuse-is-all-you-need/](https://jakobemmerling.de/posts/fuse-is-all-you-need/)

生成摘要时出错

---

## 28. LLVM: The bad parts

**原文标题**: LLVM: The bad parts

**原文链接**: [https://www.npopov.com/2026/01/11/LLVM-The-bad-parts.html](https://www.npopov.com/2026/01/11/LLVM-The-bad-parts.html)

生成摘要时出错

---

## 29. Sampling at negative temperature

**原文标题**: Sampling at negative temperature

**原文链接**: [https://cavendishlabs.org/blog/negative-temperature/](https://cavendishlabs.org/blog/negative-temperature/)

生成摘要时出错

---

## 30. A battle over Canada’s mystery brain disease

**原文标题**: A battle over Canada’s mystery brain disease

**原文链接**: [https://www.bbc.com/news/articles/c623r47d67lo](https://www.bbc.com/news/articles/c623r47d67lo)

生成摘要时出错

---

## 31. Iran shuts down Starlink internet for first time

**原文标题**: Iran shuts down Starlink internet for first time

**原文链接**: [https://www.forbes.com/sites/zakdoffman/2026/01/11/kill-switch-iran-shuts-down-starlink-internet-for-first-time/](https://www.forbes.com/sites/zakdoffman/2026/01/11/kill-switch-iran-shuts-down-starlink-internet-for-first-time/)

生成摘要时出错

---

## 32. Date is out, Temporal is in

**原文标题**: Date is out, Temporal is in

**原文链接**: [https://piccalil.li/blog/date-is-out-and-temporal-is-in/](https://piccalil.li/blog/date-is-out-and-temporal-is-in/)

生成摘要时出错

---

## 33. Workers at Redmond SpaceX lab exposed to toxic chemicals

**原文标题**: Workers at Redmond SpaceX lab exposed to toxic chemicals

**原文链接**: [https://www.fox13seattle.com/video/fmc-w1ga4pk97gxq0hj5](https://www.fox13seattle.com/video/fmc-w1ga4pk97gxq0hj5)

生成摘要时出错

---

## 34. I'd tell you a UDP joke…

**原文标题**: I'd tell you a UDP joke…

**原文链接**: [https://www.codepuns.com/post/805294580859879424/i-would-tell-you-a-udp-joke-but-you-might-not-get](https://www.codepuns.com/post/805294580859879424/i-would-tell-you-a-udp-joke-but-you-might-not-get)

生成摘要时出错

---

## 35. Max Payne – two decades later – Graphics Critique (2021)

**原文标题**: Max Payne – two decades later – Graphics Critique (2021)

**原文链接**: [https://darkcephas.blogspot.com/2021/07/max-payne-two-decades-later-graphics.html](https://darkcephas.blogspot.com/2021/07/max-payne-two-decades-later-graphics.html)

生成摘要时出错

---

## 36. Lightpanda migrate DOM implementation to Zig

**原文标题**: Lightpanda migrate DOM implementation to Zig

**原文链接**: [https://lightpanda.io/blog/posts/migrating-our-dom-to-zig](https://lightpanda.io/blog/posts/migrating-our-dom-to-zig)

生成摘要时出错

---

## 37. Statement from Federal Reserve Chair

**原文标题**: Statement from Federal Reserve Chair

**原文链接**: [https://www.federalreserve.gov/newsevents/speech/powell20260111a.htm?mod=ANLink](https://www.federalreserve.gov/newsevents/speech/powell20260111a.htm?mod=ANLink)

生成摘要时出错

---

## 38. Uncrossy

**原文标题**: Uncrossy

**原文链接**: [https://uncrossy.com/](https://uncrossy.com/)

生成摘要时出错

---

## 39. Show HN: Play poker with LLMs, or watch them play against each other

**原文标题**: Show HN: Play poker with LLMs, or watch them play against each other

**原文链接**: [https://llmholdem.com/](https://llmholdem.com/)

生成摘要时出错

---

## 40. Himalayas bare and rocky after reduced winter snowfall, scientists warn

**原文标题**: Himalayas bare and rocky after reduced winter snowfall, scientists warn

**原文链接**: [https://www.bbc.com/news/articles/clyndv7zd20o](https://www.bbc.com/news/articles/clyndv7zd20o)

生成摘要时出错

---

## 41. Windows 8 Desktop Environment for Linux

**原文标题**: Windows 8 Desktop Environment for Linux

**原文链接**: [https://github.com/er-bharat/Win8DE](https://github.com/er-bharat/Win8DE)

生成摘要时出错

---

## 42. Bob Weir has died

**原文标题**: Bob Weir has died

**原文链接**: [https://www.rollingstone.com/music/music-news/bob-weir-grateful-dead-dead-obituary-1234810106/](https://www.rollingstone.com/music/music-news/bob-weir-grateful-dead-dead-obituary-1234810106/)

生成摘要时出错

---

## 43. Ai, Japanese chimpanzee who counted and painted dies at 49

**原文标题**: Ai, Japanese chimpanzee who counted and painted dies at 49

**原文链接**: [https://www.bbc.com/news/articles/cj9r3zl2ywyo](https://www.bbc.com/news/articles/cj9r3zl2ywyo)

生成摘要时出错

---

## 44. Code is cheap now, but software isn't

**原文标题**: Code is cheap now, but software isn't

**原文链接**: [https://www.chrisgregori.dev/opinion/code-is-cheap-now-software-isnt](https://www.chrisgregori.dev/opinion/code-is-cheap-now-software-isnt)

生成摘要时出错

---

## 45. Anthropic made a mistake in cutting off third-party clients

**原文标题**: Anthropic made a mistake in cutting off third-party clients

**原文链接**: [https://archaeologist.dev/artifacts/anthropic](https://archaeologist.dev/artifacts/anthropic)

生成摘要时出错

---

## 46. China applies to put 200K satellites in space after calling Starlink crash risk

**原文标题**: China applies to put 200K satellites in space after calling Starlink crash risk

**原文链接**: [https://www.scmp.com/news/china/science/article/3339493/china-applies-put-200000-satellites-space-after-calling-starlink-crash-risk](https://www.scmp.com/news/china/science/article/3339493/china-applies-put-200000-satellites-space-after-calling-starlink-crash-risk)

生成摘要时出错

---

## 47. Iran is likely jamming Starlink

**原文标题**: Iran is likely jamming Starlink

**原文链接**: [https://www.timesofisrael.com/iran-appears-to-jam-starlink-after-shutting-down-comms-networks/](https://www.timesofisrael.com/iran-appears-to-jam-starlink-after-shutting-down-comms-networks/)

生成摘要时出错

---

## 48. UK Orders Ofcom to Explore Encryption Backdoors

**原文标题**: UK Orders Ofcom to Explore Encryption Backdoors

**原文链接**: [https://reclaimthenet.org/uk-orders-ofcom-to-explore-encryption-backdoors](https://reclaimthenet.org/uk-orders-ofcom-to-explore-encryption-backdoors)

生成摘要时出错

---

## 49. ‘Fuck you, make me’ without saying the words

**原文标题**: ‘Fuck you, make me’ without saying the words

**原文链接**: [https://daringfireball.net/2026/01/fuck_you_make_me_without_saying_the_words](https://daringfireball.net/2026/01/fuck_you_make_me_without_saying_the_words)

生成摘要时出错

---

## 50. Iran has now been offline for 96 hours

**原文标题**: Iran has now been offline for 96 hours

**原文链接**: [https://twitter.com/netblocks/status/2010750871274160361](https://twitter.com/netblocks/status/2010750871274160361)

生成摘要时出错

---

## 51. Zen-C: Write like a high-level language, run like C

**原文标题**: Zen-C: Write like a high-level language, run like C

**原文链接**: [https://github.com/z-libs/Zen-C](https://github.com/z-libs/Zen-C)

生成摘要时出错

---

## 52. Erich von Däniken has died

**原文标题**: Erich von Däniken has died

**原文链接**: [https://daniken.com/en/startseite-english/](https://daniken.com/en/startseite-english/)

生成摘要时出错

---

## 53. Worst of breed software

**原文标题**: Worst of breed software

**原文链接**: [https://worstofbreed.net/](https://worstofbreed.net/)

生成摘要时出错

---

## 54. Which programming languages are most token-efficient?

**原文标题**: Which programming languages are most token-efficient?

**原文链接**: [https://martinalderson.com/posts/which-programming-languages-are-most-token-efficient/](https://martinalderson.com/posts/which-programming-languages-are-most-token-efficient/)

生成摘要时出错

---

## 55. DHS restricts congressional visits to ICE facilities in Minneapolis

**原文标题**: DHS restricts congressional visits to ICE facilities in Minneapolis

**原文链接**: [https://www.npr.org/2026/01/11/nx-s1-5673949/dhs-restricts-congressional-visits-to-ice-facilities-in-minneapolis-with-new-policy](https://www.npr.org/2026/01/11/nx-s1-5673949/dhs-restricts-congressional-visits-to-ice-facilities-in-minneapolis-with-new-policy)

生成摘要时出错

---

## 56. Ireland fast tracks Bill to criminalise harmful voice or image misuse

**原文标题**: Ireland fast tracks Bill to criminalise harmful voice or image misuse

**原文链接**: [https://www.irishtimes.com/ireland/2026/01/07/call-to-fast-track-bill-targeting-ai-deepfakes-and-identity-hijacking/](https://www.irishtimes.com/ireland/2026/01/07/call-to-fast-track-bill-targeting-ai-deepfakes-and-identity-hijacking/)

生成摘要时出错

---

## 57. Think of Pavlov

**原文标题**: Think of Pavlov

**原文链接**: [https://boz.com/articles/think-pavlov](https://boz.com/articles/think-pavlov)

生成摘要时出错

---

## 58. Launch a Debugging Terminal into GitHub Actions

**原文标题**: Launch a Debugging Terminal into GitHub Actions

**原文链接**: [https://blog.gripdev.xyz/2026/01/10/actions-terminal-on-failure-for-debugging/](https://blog.gripdev.xyz/2026/01/10/actions-terminal-on-failure-for-debugging/)

生成摘要时出错

---

## 59. HTML-only conditional lazy loading (via preload and media)

**原文标题**: HTML-only conditional lazy loading (via preload and media)

**原文链接**: [https://orga.cat/blog/html-conditional-lazy-loading/](https://orga.cat/blog/html-conditional-lazy-loading/)

生成摘要时出错

---

## 60. guys why does armenian completely break Claude

**原文标题**: guys why does armenian completely break Claude

**原文链接**: [https://twitter.com/dyushag/status/1993143599286886525](https://twitter.com/dyushag/status/1993143599286886525)

生成摘要时出错

---

## 61. A Year of Work on the Arch Linux Package Management (ALPM) Project

**原文标题**: A Year of Work on the Arch Linux Package Management (ALPM) Project

**原文链接**: [https://devblog.archlinux.page/2026/a-year-of-work-on-the-alpm-project/](https://devblog.archlinux.page/2026/a-year-of-work-on-the-alpm-project/)

生成摘要时出错

---

## 62. Fossil versus Git

**原文标题**: Fossil versus Git

**原文链接**: [https://fossil-scm.org/home/doc/trunk/www/fossil-v-git.wiki](https://fossil-scm.org/home/doc/trunk/www/fossil-v-git.wiki)

生成摘要时出错

---

## 63. American Dialect Society 2025 Word of the Year Is "Slop"

**原文标题**: American Dialect Society 2025 Word of the Year Is "Slop"

**原文链接**: [https://americandialect.org/2025-word-of-the-year-is-slop/](https://americandialect.org/2025-word-of-the-year-is-slop/)

生成摘要时出错

---

## 64. Code Is Clay

**原文标题**: Code Is Clay

**原文链接**: [https://campedersen.com/code-is-clay](https://campedersen.com/code-is-clay)

生成摘要时出错

---

## 65. Rats caught on camera hunting flying bats (2025)

**原文标题**: Rats caught on camera hunting flying bats (2025)

**原文链接**: [https://scienceclock.com/rats-caught-on-camera-hunting-flying-bats-for-the-first-time/](https://scienceclock.com/rats-caught-on-camera-hunting-flying-bats-for-the-first-time/)

生成摘要时出错

---

## 66. BasiliskII Macintosh 68k Emulator Ported to ESP32-P4 / M5Stack Tab5

**原文标题**: BasiliskII Macintosh 68k Emulator Ported to ESP32-P4 / M5Stack Tab5

**原文链接**: [https://github.com/amcchord/M5Tab-Macintosh](https://github.com/amcchord/M5Tab-Macintosh)

生成摘要时出错

---

## 67. More than one hundred years of Film Sizes

**原文标题**: More than one hundred years of Film Sizes

**原文链接**: [https://wichm.home.xs4all.nl/filmsize.html](https://wichm.home.xs4all.nl/filmsize.html)

生成摘要时出错

---

## 68. Postal Arbitrage

**原文标题**: Postal Arbitrage

**原文链接**: [https://walzr.com/postal-arbitrage](https://walzr.com/postal-arbitrage)

生成摘要时出错

---

## 69. Reproducing DeepSeek's MHC: When Residual Connections Explode

**原文标题**: Reproducing DeepSeek's MHC: When Residual Connections Explode

**原文链接**: [https://taylorkolasinski.com/notes/mhc-reproduction/](https://taylorkolasinski.com/notes/mhc-reproduction/)

生成摘要时出错

---

## 70. Google: Don't make "bite-sized" content for LLMs

**原文标题**: Google: Don't make "bite-sized" content for LLMs

**原文链接**: [https://arstechnica.com/google/2026/01/google-dont-make-bite-sized-content-for-llms-if-you-care-about-search-rank/](https://arstechnica.com/google/2026/01/google-dont-make-bite-sized-content-for-llms-if-you-care-about-search-rank/)

生成摘要时出错

---

## 71. Keychron's Nape Pro turns your keyboard into a laptop‑style trackball rig

**原文标题**: Keychron's Nape Pro turns your keyboard into a laptop‑style trackball rig

**原文链接**: [https://www.yankodesign.com/2026/01/08/keychrons-nape-pro-turns-your-mechanical-keyboard-into-a-laptop-style-trackball-rig-hands-on-at-ces-2026/](https://www.yankodesign.com/2026/01/08/keychrons-nape-pro-turns-your-mechanical-keyboard-into-a-laptop-style-trackball-rig-hands-on-at-ces-2026/)

生成摘要时出错

---

## 72. Linus Torvalds Uses Google Antigravity

**原文标题**: Linus Torvalds Uses Google Antigravity

**原文链接**: [https://github.com/torvalds/AudioNoise/blob/main/README.md](https://github.com/torvalds/AudioNoise/blob/main/README.md)

生成摘要时出错

---

## 73. Gadget Exposed a Spy Camera [video]

**原文标题**: Gadget Exposed a Spy Camera [video]

**原文链接**: [https://www.youtube.com/watch?v=1reman2waLs](https://www.youtube.com/watch?v=1reman2waLs)

生成摘要时出错

---

## 74. Happy 50th Birthday KIM-1

**原文标题**: Happy 50th Birthday KIM-1

**原文链接**: [https://github.com/netzherpes/KIM1-Demo](https://github.com/netzherpes/KIM1-Demo)

生成摘要时出错

---

## 75. YouTube has removed the ability to search by upload date

**原文标题**: YouTube has removed the ability to search by upload date

**原文链接**: [https://twitter.com/TeamYouTube/status/2009744367834022320](https://twitter.com/TeamYouTube/status/2009744367834022320)

生成摘要时出错

---

## 76. Replace the Retiring Windows XP with Linux (2014)

**原文标题**: Replace the Retiring Windows XP with Linux (2014)

**原文链接**: [https://www.linux.com/training-tutorials/replace-retiring-windows-xp-linux/](https://www.linux.com/training-tutorials/replace-retiring-windows-xp-linux/)

生成摘要时出错

---

## 77. Quake 1 Single-Player Map Design Theories (2001)

**原文标题**: Quake 1 Single-Player Map Design Theories (2001)

**原文链接**: [https://www.quaddicted.com/webarchive//teamshambler.planetquake.gamespy.com/theories1.html](https://www.quaddicted.com/webarchive//teamshambler.planetquake.gamespy.com/theories1.html)

生成摘要时出错

---

## 78. Extracting books from production language models (2026)

**原文标题**: Extracting books from production language models (2026)

**原文链接**: [https://arxiv.org/abs/2601.02671](https://arxiv.org/abs/2601.02671)

生成摘要时出错

---

## 79. Bichon: A lightweight, high-performance Rust email archiver with WebUI

**原文标题**: Bichon: A lightweight, high-performance Rust email archiver with WebUI

**原文链接**: [https://github.com/rustmailer/bichon](https://github.com/rustmailer/bichon)

生成摘要时出错

---

## 80. "Scholars Will Call It Nonsense": The Structure of von Däniken's Argument (1987)

**原文标题**: "Scholars Will Call It Nonsense": The Structure of von Däniken's Argument (1987)

**原文链接**: [https://www.penn.museum/sites/expedition/scholars-will-call-it-nonsense/](https://www.penn.museum/sites/expedition/scholars-will-call-it-nonsense/)

生成摘要时出错

---

## 81. Linus is vibe coding

**原文标题**: Linus is vibe coding

**原文链接**: [https://github.com/torvalds/AudioNoise](https://github.com/torvalds/AudioNoise)

生成摘要时出错

---

## 82. US prosecutors launch criminal investigation into Federal Reserve chair

**原文标题**: US prosecutors launch criminal investigation into Federal Reserve chair

**原文链接**: [https://www.theguardian.com/business/live/2026/jan/12/us-prosecutors-criminal-investigation-federal-reserve-chair-jerome-powell-dollar-stock-market-gold-bitcoin-business-live-news-updates](https://www.theguardian.com/business/live/2026/jan/12/us-prosecutors-criminal-investigation-federal-reserve-chair-jerome-powell-dollar-stock-market-gold-bitcoin-business-live-news-updates)

生成摘要时出错

---

## 83. Tesla's Germany Sales Down 72% from Their Peak

**原文标题**: Tesla's Germany Sales Down 72% from Their Peak

**原文链接**: [https://cleantechnica.com/2026/01/08/teslas-germany-sales-down-72-from-their-peak/](https://cleantechnica.com/2026/01/08/teslas-germany-sales-down-72-from-their-peak/)

生成摘要时出错

---

## 84. Show HN: Epstein IM – Talk to Epstein clone in iMessage

**原文标题**: Show HN: Epstein IM – Talk to Epstein clone in iMessage

**原文链接**: [https://epstein.im/](https://epstein.im/)

生成摘要时出错

---

## 85. Tux Paint

**原文标题**: Tux Paint

**原文链接**: [https://tuxpaint.org/](https://tuxpaint.org/)

生成摘要时出错

---

## 86. Show HN: AI in SolidWorks

**原文标题**: Show HN: AI in SolidWorks

**原文链接**: [https://www.trylad.com](https://www.trylad.com)

生成摘要时出错

---

## 87. Open-Meteo is a free and open-source weather API for non-commercial use

**原文标题**: Open-Meteo is a free and open-source weather API for non-commercial use

**原文链接**: [https://open-meteo.com/](https://open-meteo.com/)

生成摘要时出错

---

## 88. OpenAI is reportedly asking contractors to upload real work from past jobs

**原文标题**: OpenAI is reportedly asking contractors to upload real work from past jobs

**原文链接**: [https://techcrunch.com/2026/01/10/openai-is-reportedly-asking-contractors-to-upload-real-work-from-past-jobs/](https://techcrunch.com/2026/01/10/openai-is-reportedly-asking-contractors-to-upload-real-work-from-past-jobs/)

生成摘要时出错

---

## 89. Sisyphus Now Lives in Oh My Claude

**原文标题**: Sisyphus Now Lives in Oh My Claude

**原文链接**: [https://github.com/Yeachan-Heo/oh-my-claude-sisyphus](https://github.com/Yeachan-Heo/oh-my-claude-sisyphus)

生成摘要时出错

---

## 90. 2025 marked a record-breaking year for Apple services

**原文标题**: 2025 marked a record-breaking year for Apple services

**原文链接**: [https://www.apple.com/newsroom/2026/01/2025-marked-a-record-breaking-year-for-apple-services/](https://www.apple.com/newsroom/2026/01/2025-marked-a-record-breaking-year-for-apple-services/)

生成摘要时出错

---

## 91. Unauthenticated remote code execution in OpenCode

**原文标题**: Unauthenticated remote code execution in OpenCode

**原文链接**: [https://cy.md/opencode-rce/](https://cy.md/opencode-rce/)

生成摘要时出错

---

## 92. KaraDAV – Lightweight Nextcloud compatible WebDAV server

**原文标题**: KaraDAV – Lightweight Nextcloud compatible WebDAV server

**原文链接**: [https://github.com/kd2org/karadav](https://github.com/kd2org/karadav)

生成摘要时出错

---

## 93. Show HN: An LLM-optimized programming language

**原文标题**: Show HN: An LLM-optimized programming language

**原文链接**: [https://github.com/ImJasonH/ImJasonH/blob/main/articles/llm-programming-language.md](https://github.com/ImJasonH/ImJasonH/blob/main/articles/llm-programming-language.md)

生成摘要时出错

---

## 94. Ripple: The Elegant TypeScript UI Framework

**原文标题**: Ripple: The Elegant TypeScript UI Framework

**原文链接**: [https://jsdev.space/meet-ripple/](https://jsdev.space/meet-ripple/)

生成摘要时出错

---

## 95. Are We ... Yet?

**原文标题**: Are We ... Yet?

**原文链接**: [https://wiki.mozilla.org/Areweyet](https://wiki.mozilla.org/Areweyet)

生成摘要时出错

---

## 96. Show HN: VAM Seek – 2D video navigation grid, 15KB, zero server load

**原文标题**: Show HN: VAM Seek – 2D video navigation grid, 15KB, zero server load

**原文链接**: [https://github.com/unhaya/vam-seek](https://github.com/unhaya/vam-seek)

生成摘要时出错

---

## 97. Building a 25 Gbit/s workstation for the SCION Association

**原文标题**: Building a 25 Gbit/s workstation for the SCION Association

**原文链接**: [https://github.com/scionassociation/blog-25gbit-workstation](https://github.com/scionassociation/blog-25gbit-workstation)

生成摘要时出错

---

## 98. Why Ontario Digital Service couldn't procure '98% safe' LLMs (15M Canadians)

**原文标题**: Why Ontario Digital Service couldn't procure '98% safe' LLMs (15M Canadians)

**原文链接**: [https://rosetta-labs-erb.github.io/authority-boundary-ledger/](https://rosetta-labs-erb.github.io/authority-boundary-ledger/)

生成摘要时出错

---

## 99. Court rejects NVIDIAs attempt to seal email chain with Annas Archive [pdf]

**原文标题**: Court rejects NVIDIAs attempt to seal email chain with Annas Archive [pdf]

**原文链接**: [https://storage.courtlistener.com/recap/gov.uscourts.cand.426191/gov.uscourts.cand.426191.222.0.pdf](https://storage.courtlistener.com/recap/gov.uscourts.cand.426191/gov.uscourts.cand.426191.222.0.pdf)

生成摘要时出错

---

## 100. Message Queues: A Simple Guide with Analogies

**原文标题**: Message Queues: A Simple Guide with Analogies

**原文链接**: [https://www.cloudamqp.com/blog/message-queues-exaplined-with-analogies.html](https://www.cloudamqp.com/blog/message-queues-exaplined-with-analogies.html)

生成摘要时出错

---

