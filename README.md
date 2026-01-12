# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-01-12.md)

*最后自动更新时间: 2026-01-12 19:50:50*
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

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 2 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 3 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 4 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 5 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 6 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 7 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 8 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 9 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 10 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 11 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 12 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 13 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 14 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 15 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 16 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 17 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 18 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 19 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 20 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 21 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 22 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 23 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 24 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 25 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 26 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 27 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 28 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 29 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 30 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 31 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 32 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 33 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 34 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 35 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 36 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 37 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 38 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 39 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 40 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 41 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 42 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 43 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 44 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 45 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 46 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 47 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 48 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 49 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 50 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 51 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 52 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 53 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 54 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 55 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 56 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 57 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 58 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 59 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 60 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 61 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 62 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 63 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 64 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
| 65 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 66 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 67 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 68 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
