# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-04-15.md)

*最后自动更新时间: 2026-04-15 20:30:17*
## 1. 达芬奇 - 照片

**原文标题**: DaVinci Resolve – Photo

**原文链接**: [https://www.blackmagicdesign.com/products/davinciresolve/photo](https://www.blackmagicdesign.com/products/davinciresolve/photo)

DaVinci Resolve 的全新“照片”页面将其先进的好莱坞级别色彩校正和调色工具引入静态摄影领域，满足专业调色师和摄影师的需求。它提供了一套熟悉的标准调整功能，例如白平衡、曝光和色彩，同时还为主要相机品牌（佳能、尼康、索尼、富士胶片、iPhone ProRAW）提供原生RAW支持。

摄影师可受益于高达32K原始分辨率的无损编辑、GPU加速带来的快速处理和批量导出，以及精确的变换/裁剪功能。该平台包含强大的图像管理功能，允许导入、使用标签和关键词进行整理、AI智能搜索，以及创建相册来管理收藏和多个调色版本。索尼和佳能的相机联机拍摄功能可实现实时捕捉和调色。

对于调色师和高级用户，“照片”页面解锁了完整的DaVinci调色页面，提供基于节点的调色、专业示波器、Power Windows以及超过100种Resolve FX特效。强大的AI工具也已集成，包括用于选区的Magic Mask、用于分离前景/背景的Depth Map、用于添加光源的Relight FX、用于美容修饰的Face Refinement、用于画面放大的AI SuperScale，以及用于降噪的UltraNR。

协作是其核心，通过基于云的工作流程，实现相册和调色在全球范围内的实时共享。硬件调色台提供直观的创意控制。DaVinci Resolve 可免费下载，Studio版本售价295美元。

---

## 2. Backblaze 停止备份 OneDrive 和 Dropbox 文件夹，可能还有其他。

**原文标题**: Backblaze has stopped backing up OneDrive and Dropbox folders and maybe others

**原文链接**: [https://rareese.com/posts/backblaze/](https://rareese.com/posts/backblaze/)

For a decade, the author relied on Backblaze for comprehensive, unlimited personal computer backups, praising its service after a successful data recovery in the past. Backblaze had always promised to back up "all user data" with "no restrictions on file type or size," building significant trust.

However, the author discovered a "disturbing trend" of Backblaze quietly ceasing to back up certain types of files and folders. First, they found that Backblaze ignored `.git` folders, preventing restoration of lost Git history. More recently, a Reddit thread alerted them to Backblaze no longer backing up Dropbox folders, leading the author to discover their 383GB OneDrive folder was also excluded.

The author emphasizes that cloud syncing services like OneDrive and Dropbox are not true backups, offering limited file retention and version history compared to Backblaze's previous policy. The core betrayal, for the author, is Backblaze's complete lack of transparent communication regarding these significant policy changes. The exclusion was "nestled into their release notes under 'Improvements'," which the author views as a "downgrade in service" and a broken promise. Furthermore, these exclusions are not listed in the app's preferences or on Backblaze's public exclusion lists.

The author concludes that by silently deciding not to back up "everything," Backblaze has fundamentally eroded trust. They warn other users that Backblaze is no longer backing up "all" their data, despite their original promises of "Unlimited, Simplified, Secure Personal Online Backup Cloud Storage."

---

## 3. 停止群聚

**原文标题**: Stop Flock

**原文链接**: [https://stopflock.com](https://stopflock.com)

生成摘要时出错

---

## 4. “后退按钮劫持”新垃圾信息政策

**原文标题**: A new spam policy for “back button hijacking”

**原文链接**: [https://developers.google.com/search/blog/2026/04/back-button-hijacking](https://developers.google.com/search/blog/2026/04/back-button-hijacking)

Google搜索中心已宣布一项新的垃圾内容政策，旨在打击“返回按钮劫持”，该政策将于2026年6月15日生效。这种欺骗性行为现在已明确违反Google的“恶意行为”政策，它指的是网站干扰用户的浏览器导航，阻止用户通过点击返回按钮回到上一页。相反，用户可能会被发送到意想不到的页面，看到不请自来的内容，或以其他方式阻碍正常浏览。

Google表示，此举优先考虑用户体验，因为返回按钮劫持会使用户感到沮丧，并打破基本的浏览器预期。这种行为的出现促使其被定性为恶意行为，即在用户预期与实际结果之间造成不匹配，从而导致负面或欺骗性的体验。

从事返回按钮劫持的网站可能会面临人工垃圾内容处理或自动降级，从而影响其Google搜索表现。网站所有者被敦促审查其技术实施，并删除任何操纵浏览器历史记录的脚本、技术或第三方代码（包括库或广告平台）。如果网站受到人工处理影响且问题已解决，所有者可以通过Search Console提交重新审核请求。此政策旨在促进一个有益且非欺骗性的网络体验。

---

## 5. GitHub 堆叠式PR

**原文标题**: GitHub Stacked PRs

**原文链接**: [https://github.github.com/gh-stack/](https://github.github.com/gh-stack/)

GitHub 正在推出一项原生的“堆叠式 PRs”功能，以简化复杂代码变更的管理。这项新功能允许开发者将拉取请求按顺序堆叠排列，从而能够一键合并所有相关的 PRs。

其核心理念是将大型变更分解为更小、更集中的层次，每个层次都由一个独立的拉取请求表示。这种方法有助于对每个特定层次进行独立审查，提高了审查者的清晰度和可管理性。最终，堆叠式 PRs 实现了独立的、有重点的审查，同时确保了大型变更中所有已批准的组件能够高效地一起合并。

---

## 6. 克劳德代码例程

**原文标题**: Claude Code Routines

**原文链接**: [https://code.claude.com/docs/en/routines](https://code.claude.com/docs/en/routines)

Claude 代码例程是已保存的自动化配置，包含提示、仓库和连接器，它们在 Anthropic 的云基础设施上执行，使得无人值守、可重复的任务能够持续运行。这些例程适用于 Pro、Max、Team 和 Enterprise 计划的用户。

例程可以通过三种类型的触发器激活：
1.  **定时触发：** 按周期性频率运行（每小时、每天、每周或自定义 cron 表达式）。
2.  **API 触发：** 通过向带有 bearer token 的唯一端点发送 HTTP POST 请求来按需触发。这允许与告警工具或 CI/CD 流水线等外部系统集成，并在请求体中传递特定于运行的上下文。
3.  **GitHub 触发：** 自动响应仓库事件，例如拉取请求（已打开、已关闭、已更新）或发布（已创建、已发布）。这些触发器可以根据作者、标题、基础/头部（或源/目标）分支、标签或草稿状态等条件进行精细过滤。

例程通过网页用户界面 (claude.ai/code/routines)、命令行界面 (CLI) (/schedule) 或桌面应用程序（“新建远程任务”）进行创建和管理。在创建过程中，用户定义一个自包含的提示，选择 GitHub 仓库（可选择无限制的推送权限），配置云环境（网络访问、变量、设置脚本），并选择连接器以连接到 Slack 或 Linear 等外部服务。

作为自主云会话执行，例程会执行归因于用户关联的 GitHub 身份或服务账户的操作（例如，提交、拉取请求、外部服务交互）。示例应用包括待办事项维护、告警分类、定制代码审查、部署验证、文档更新和库移植。

---

## 7. 稀有演唱会录音正在登陆互联网档案馆。

**原文标题**: Rare concert recordings are landing on the Internet Archive

**原文链接**: [https://techcrunch.com/2026/04/13/thousands-of-rare-concert-recordings-are-landing-on-the-internet-archive-listen-now/](https://techcrunch.com/2026/04/13/thousands-of-rare-concert-recordings-are-landing-on-the-internet-archive-listen-now/)

Chicago-based music superfan Aadam Jacobs is collaborating with the Internet Archive to digitize his vast collection of over 10,000 rare concert recordings, amassed since the 1980s. Realizing his cassette tapes would eventually degrade, the 59-year-old agreed to let volunteers from the nonprofit digital library preserve this unique archive.

So far, approximately 2,500 of these tapes have been posted online. The collection features rare gems, including a 1989 Nirvana performance recorded before their mainstream success, as well as previously unknown recordings from influential artists like Sonic Youth, R.E.M., Phish, Liz Phair, Pavement, Neutral Milk Hotel, and numerous punk groups, alongside a 1988 Tracy Chapman concert.

Despite Jacobs often using modest recording equipment, volunteer audio engineers are meticulously cleaning up and enhancing the sound quality. Volunteers like Brian Emerick regularly collect batches of tapes, which are converted into digital files using specialized cassette decks. Other volunteers then organize, label, and even identify song names for forgotten bands, making this significant musical history accessible to the public.

---

## 8. 我写信给Flock的隐私联系人，选择退出他们的国内间谍计划。

**原文标题**: I wrote to Flock's privacy contact to opt out of their domestic spying program

**原文链接**: [https://honeypot.net/2026/04/14/i-wrote-to-flocks-privacy.html](https://honeypot.net/2026/04/14/i-wrote-to-flocks-privacy.html)

生成摘要时出错

---

## 9. Google Broke Its Promise to Me. Now ICE Has My Data

**原文标题**: Google Broke Its Promise to Me. Now ICE Has My Data

**原文链接**: [https://www.eff.org/deeplinks/2026/04/google-broke-its-promise-me-now-ice-has-my-data](https://www.eff.org/deeplinks/2026/04/google-broke-its-promise-me-now-ice-has-my-data)

生成摘要时出错

---

## 10. jj – the CLI for Jujutsu

**原文标题**: jj – the CLI for Jujutsu

**原文链接**: [https://steveklabnik.github.io/jujutsu-tutorial/introduction/what-is-jj-and-why-should-i-care.html](https://steveklabnik.github.io/jujutsu-tutorial/introduction/what-is-jj-and-why-should-i-care.html)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 2 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 3 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 4 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 5 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 6 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 7 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 8 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 9 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 10 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 11 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 12 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 13 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 14 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 15 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 16 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 17 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 18 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 19 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 20 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 21 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 22 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 23 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 24 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 25 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 26 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 27 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 28 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 29 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 30 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 31 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 32 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 33 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 34 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 35 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 36 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 37 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 38 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 39 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 40 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 41 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 42 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 43 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 44 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 45 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 46 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 47 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 48 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 49 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 50 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 51 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 52 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 53 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 54 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 55 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 56 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 57 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 58 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 59 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 60 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 61 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 62 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 63 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 64 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 65 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 66 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 67 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 68 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 69 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 70 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 71 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 72 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 73 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 74 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 75 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 76 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 77 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 78 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 79 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 80 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 81 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 82 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 83 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 84 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 85 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 86 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 87 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 88 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 89 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 90 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 91 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 92 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 93 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 94 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 95 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 96 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 97 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 98 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 99 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 100 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 101 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 102 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 103 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 104 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 105 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 106 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 107 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 108 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 109 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 110 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 111 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 112 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 113 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 114 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 115 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 116 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 117 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 118 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 119 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 120 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 121 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 122 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 123 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 124 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 125 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 126 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 127 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 128 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 129 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 130 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 131 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 132 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 133 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 134 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 135 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 136 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 137 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 138 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 139 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 140 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 141 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 142 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 143 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 144 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 145 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 146 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 147 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 148 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 149 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 150 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 151 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 152 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 153 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 154 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 155 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 156 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 157 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 158 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 159 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
