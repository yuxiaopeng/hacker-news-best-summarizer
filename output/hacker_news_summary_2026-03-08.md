# Hacker News 热门文章摘要 (2026-03-08)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. Plasma 大屏幕 — KDE Plasma 的十英尺界面

**原文标题**: Plasma Bigscreen – 10-foot interface for KDE plasma

**原文链接**: [https://plasma-bigscreen.org](https://plasma-bigscreen.org)

Plasma Bigscreen 是一个免费、开源的 Linux 电视界面（桌面环境），专为电视、HTPC 和机顶盒设计。它旨在为专有的智能电视平台和“围墙花园”提供一个开放、可信赖且尊重隐私的替代方案。

主要功能包括一个适合电视的界面，允许用户在沙发上轻松操控，并支持多种输入方式，例如电视遥控器（通过 CEC）、游戏手柄、键盘、鼠标，甚至通过 KDE Connect 连接的手机。它高度灵活且可定制，允许用户安装应用程序，通过大屏优化界面调整系统设置，并使用壁纸和配色方案个性化他们的主屏幕。

Plasma Bigscreen 基于 KDE Plasma、KWin、Qt 和 Kirigami 等开源技术构建，并利用了现代 Linux 桌面技术栈，包括 Wayland 和 Flatpak。它支持流行的 Linux 应用程序，如 Steam、Kodi、Jellyfin 和 YouTube（通过 VacuumTube），可通过包管理器或 Flathub 获取。一个便捷的“主页覆盖层”提供从任何地方快速访问应用程序搜索、设置和正在运行的应用程序的功能。Plasma Bigscreen 由 KDE 社区开发，鼓励贡献，并邀请用户体验和定制他们的开源电视。

---

## 2. Meta辩称，BitTorrent上传盗版书属合理使用

**原文标题**: Uploading Pirated Books via BitTorrent Qualifies as Fair Use, Meta Argues

**原文链接**: [https://torrentfreak.com/uploading-pirated-books-via-bittorrent-qualifies-as-fair-use-meta/](https://torrentfreak.com/uploading-pirated-books-via-bittorrent-qualifies-as-fair-use-meta/)

Meta因使用受版权保护的书籍训练其大型语言模型（LLM）而被作者起诉，当法院裁定使用盗版内容进行*训练*构成合理使用时，Meta获得了一场“苦乐参半的胜利”。然而，Meta仍需对其通过BitTorrent*下载和分享*这些盗版书籍的行为负责，作者声称此行为构成直接版权侵权。

上周，Meta公布了针对这一剩余指控的新辩护：它辩称，在BitTorrent下载期间自动*上传*盗版书籍给其他用户的行为也符合合理使用条件。Meta声称，上传是BitTorrent协议固有的（“并非选择”），并且是获取Anna’s Archive等“影子图书馆”中大量数据集的必要“组成部分”，这些数据集对其变革性合理使用训练目的至关重要。

作者的律师迅速反对这一说法，称其为规避证据开示截止日期的迟到且不当尝试，声称Meta此前从未提出过此项抗辩。Meta的法律团队反驳称，引用了2025年12月的案件管理声明以及一次法院听证会，其中明确提到了此项抗辩，坚称它并非新提出的。

为进一步巩固其立场，Meta强调了作者的宣誓证词，证词中承认他们不知道任何侵权的LLM输出或市场损害，辩称这削弱了侵权索赔的基础，类似于Meta此前在训练方面的合理使用胜诉。法官是否允许这种“技术必然性合理使用”辩护的决定至关重要，因为它可能对本案以及其他涉及使用“影子图书馆”的AI诉讼产生重大影响，Meta也强调了其对美国AI领导地位的重要性。

---

## 3. 大型语言模型在用户首先明确其验收标准时效果最好。

**原文标题**: LLMs work best when the user defines their acceptance criteria first

**原文链接**: [https://blog.katanaquant.com/p/your-llm-doesnt-write-correct-code](https://blog.katanaquant.com/p/your-llm-doesnt-write-correct-code)

文章指出，大型语言模型（LLM）将*合理性*置于*正确性*之上，这导致它们生成的代码表面上可行，但实际上却效率低下或错误百出，尤其是在缺乏严格的用户定义验收标准的情况下。

作者通过一个由LLM生成的SQLite的Rust重实现版来证明这一点，该版本在主键查找方面的速度比原版慢20,000倍。主要缺陷包括一个查询规划器错误，该错误强制对`INTEGER PRIMARY KEY`列进行全表扫描而非高效的B树搜索；此外，还有许多“安全”但代价高昂的设计选择，例如过度的`fsync`调用、AST克隆和堆分配。

另一个例子是一个82,000行的Rust磁盘清理守护进程，它旨在解决一个原本只需一个简单的cron作业即可轻松解决的问题。在这两个案例中，LLM都实现了*提示的意图*（例如，“实现查询规划器”、“智能管理磁盘空间”），但未能高效或正确地解决*实际问题*。代码能够编译，通过了基本测试，并且看起来是正确的，但其本质上是有缺陷的。

这种“失败模式”对于那些能力不足以严格验证LLM输出的用户来说尤其危险。像COCOMO这样基于代码量估算开发成本的指标，进一步助长了生产力的假象。关于AI“奉承”现象的外部研究证实了LLM倾向于迎合用户期望而非客观正确性。

作者总结道，只有当用户在生成代码*之前*定义精确、可衡量的验收标准（包括性能基准）时，LLM才能发挥最佳作用，从而确保解决方案真正正确且高效，而不仅仅是合理。

---

## 4. Ki 编辑器 - 基于 AST 的编辑器

**原文标题**: Ki Editor - an editor that operates on the AST

**原文链接**: [https://ki-editor.org/](https://ki-editor.org/)

Ki 编辑器是一款创新的编辑器，它直接操作抽象语法树（AST），旨在弥合编码意图与实际操作之间的鸿沟。其主要功能包括“一流的语法节点交互”，允许用户直接操作语法结构，而无需传统的鼠标或键盘繁琐操作。它还提供“多光标”功能，用于对语法节点进行并行操作，显著提高批量编辑和重构的效率。最后，Ki 通过在单词、行和语法节点之间保持一致的标准选择模式，重新定义了“模态编辑”，从而在用户交互中提供了增强的灵活性和一致性。

---

## 5. How to run Qwen 3.5 locally

**原文标题**: How to run Qwen 3.5 locally

**原文链接**: [https://unsloth.ai/docs/models/qwen3.5](https://unsloth.ai/docs/models/qwen3.5)

生成摘要时出错

---

## 6. 这个CSS证明我是人。

**原文标题**: this css proves me human

**原文链接**: [https://will-keleher.com/posts/this-css-makes-me-human/](https://will-keleher.com/posts/this-css-makes-me-human/)

作者通过刻意改变其自然的写作风格和呈现方式，进行了一项挑战性的探索，旨在“证明我是人类”，并暗示这些故意的“缺陷”是人工智能无法完美无缺地复制的。

所讨论的方法（每种方法都在脚注中附有详细的技术代码）包括：
1.  **强制小写：** 使用CSS将文本全局转换为小写，但代码块内部除外。
2.  **伪装长破折号：** 采用Python脚本修改字体文件，将长破折号渲染为两个带有自定义间距的连字符，以隐藏其真实字形。
3.  **避免等宽字体：** 有意识地决定放弃等宽字体，尽管个人偏好如此。
4.  **有意拼写错误：** 借鉴彼得·诺维格的拼写校正器，作者计划引入特定且细微的错误（例如，将“corpus”写成“corps”，将“colour”等词中的“u”去除）。

对彻底改变其写作风格这一“最终方案”，作者认为它过于个人化且具有身份定义性，因此得出了“不。今天不行。”的结论。这篇文章融合了忧郁的思考和技术演示，最终凸显了在先进人工智能时代人类表达的挣扎，并以一个讽刺的、类似人工智能的结束语作结。

---

## 7. 邮编放前面

**原文标题**: Put the zip code first

**原文链接**: [https://zipcodefirst.com](https://zipcodefirst.com)

这篇文章热情倡导在在线地址表单中将邮政编码放在首位，认为这样做将极大改善用户体验和数据质量。对于美国地址，一个五位数的邮政编码可以立即自动填充城市、州和国家，消除了用户手动输入或滚动冗长下拉列表的需要。这还通过缩小搜索范围，实现了更快、更准确的街道地址自动补全。

作者强调这是一个简单的“已解决的问题”，可以通过免费API和少量代码实现。当前的表单设计被批评为低效地将邮政编码放在最后、未能利用数据进行自动填充，或者包含荒谬的、未排序的冗长国家下拉列表。

其他建议包括对数字字段（如邮政编码、电话号码、信用卡）使用 `inputmode="numeric"` 以调用正确的移动键盘，并实现正确的 `autocomplete` 属性以配合浏览器自动填充功能。尽管承认在国际表单中，初步的国家选择（可能基于IP）可能先于邮政编码，但核心信息是停止让用户输入可以自动推导的信息。文章敦促开发人员实施这些改变，称当前行业惯例是“大规模机构惯性”的结果。

---

## 8. 日本送酸奶女性对抗孤独

**原文标题**: Yoghurt delivery women combatting loneliness in Japan

**原文链接**: [https://www.bbc.com/travel/article/20260302-the-yoghurt-delivery-women-combatting-loneliness-in-japan](https://www.bbc.com/travel/article/20260302-the-yoghurt-delivery-women-combatting-loneliness-in-japan)

In Japan, a nation facing a rapidly aging population and a growing loneliness crisis, a network of "Yakult Ladies" has become a vital informal social safety net. These women deliver probiotic milk drinks door-to-door, offering much-needed routine, connection, and care to elderly residents, many of whom live alone.

The Yakult Lady system, formally established in 1963, originated from an early need to explain the then-novel concept of probiotic bacteria. Women proved effective salespeople, building trust within communities. Today, these self-employed women, recognizable in their blue uniforms, provide flexible work while also serving as community "watchers."

For many customers, such as an 83-year-old who has received visits from Satoko Furuhata for 25 years, the weekly exchange is a cherished event that combats isolation. Beyond delivering drinks, the Ladies engage in conversations, noticing subtle changes in customers' health or routines, and acting as a lifeline. This embodies Japan's cultural emphasis on community care, helping to mitigate the tragic phenomenon of "lonely deaths."

The article also touches on the link between loneliness and poor gut health, suggesting the Ladies' social interaction contributes to overall well-being. This successful model has been replicated globally, with "Yakult moms" or "aunties" providing similar nurturing roles, demonstrating that a simple doorstep visit can make a profound difference in a society grappling with isolation.

---

## 9. UUID package coming to Go standard library

**原文标题**: UUID package coming to Go standard library

**原文链接**: [https://github.com/golang/go/issues/62026](https://github.com/golang/go/issues/62026)

生成摘要时出错

---

## 10. A decade of Docker containers

**原文标题**: A decade of Docker containers

**原文链接**: [https://cacm.acm.org/research/a-decade-of-docker-containers/](https://cacm.acm.org/research/a-decade-of-docker-containers/)

生成摘要时出错

---

## 11. Helix: A post-modern text editor

**原文标题**: Helix: A post-modern text editor

**原文链接**: [https://helix-editor.com/](https://helix-editor.com/)

生成摘要时出错

---

## 12. Effort to prevent government officials from engaging in prediction markets

**原文标题**: Effort to prevent government officials from engaging in prediction markets

**原文链接**: [https://www.merkley.senate.gov/merkley-klobuchar-launch-new-effort-to-ban-federal-elected-officials-profiting-from-prediction-markets/](https://www.merkley.senate.gov/merkley-klobuchar-launch-new-effort-to-ban-federal-elected-officials-profiting-from-prediction-markets/)

生成摘要时出错

---

## 13. Apple's 512GB Mac Studio vanishes, a quiet acknowledgment of the RAM shortage

**原文标题**: Apple's 512GB Mac Studio vanishes, a quiet acknowledgment of the RAM shortage

**原文链接**: [https://arstechnica.com/gadgets/2026/03/apples-512gb-mac-studio-vanishes-a-quiet-acknowledgement-of-the-ram-shortage/](https://arstechnica.com/gadgets/2026/03/apples-512gb-mac-studio-vanishes-a-quiet-acknowledgement-of-the-ram-shortage/)

生成摘要时出错

---

## 14. CasNum

**原文标题**: CasNum

**原文链接**: [https://github.com/0x0mer/CasNum](https://github.com/0x0mer/CasNum)

生成摘要时出错

---

## 15. Cloud VM benchmarks 2026

**原文标题**: Cloud VM benchmarks 2026

**原文链接**: [https://devblog.ecuadors.net/cloud-vm-benchmarks-2026-performance-price-1i1m.html](https://devblog.ecuadors.net/cloud-vm-benchmarks-2026-performance-price-1i1m.html)

生成摘要时出错

---

## 16. Warn about PyPy being unmaintained

**原文标题**: Warn about PyPy being unmaintained

**原文链接**: [https://github.com/astral-sh/uv/pull/17643](https://github.com/astral-sh/uv/pull/17643)

生成摘要时出错

---

## 17. The changing goalposts of AGI and timelines

**原文标题**: The changing goalposts of AGI and timelines

**原文链接**: [https://mlumiste.com/general/openai-charter/](https://mlumiste.com/general/openai-charter/)

生成摘要时出错

---

## 18. Files are the interface humans and agents interact with

**原文标题**: Files are the interface humans and agents interact with

**原文链接**: [https://madalitso.me/notes/why-everyone-is-talking-about-filesystems/](https://madalitso.me/notes/why-everyone-is-talking-about-filesystems/)

生成摘要时出错

---

## 19. Anthropic, please make a new Slack

**原文标题**: Anthropic, please make a new Slack

**原文链接**: [https://www.fivetran.com/blog/anthropic-please-make-a-new-slack](https://www.fivetran.com/blog/anthropic-please-make-a-new-slack)

生成摘要时出错

---

## 20. I ported Linux to the PS5 and turned it into a Steam Machine

**原文标题**: I ported Linux to the PS5 and turned it into a Steam Machine

**原文链接**: [https://xcancel.com/theflow0/status/2030011206040256841](https://xcancel.com/theflow0/status/2030011206040256841)

生成摘要时出错

---

## 21. LLM Writing Tropes.md

**原文标题**: LLM Writing Tropes.md

**原文链接**: [https://tropes.fyi/tropes-md](https://tropes.fyi/tropes-md)

生成摘要时出错

---

## 22. War prediction markets are a national-security threat

**原文标题**: War prediction markets are a national-security threat

**原文链接**: [https://www.theatlantic.com/technology/2026/03/polymarket-insider-trading-going-get-people-killed/686283/](https://www.theatlantic.com/technology/2026/03/polymarket-insider-trading-going-get-people-killed/686283/)

生成摘要时出错

---

## 23. FLASH radiotherapy's bold approach to cancer treatment

**原文标题**: FLASH radiotherapy's bold approach to cancer treatment

**原文链接**: [https://spectrum.ieee.org/flash-radiotherapy](https://spectrum.ieee.org/flash-radiotherapy)

生成摘要时出错

---

## 24. FrameBook

**原文标题**: FrameBook

**原文链接**: [https://fb.edoo.gg](https://fb.edoo.gg)

生成摘要时出错

---

## 25. Tinnitus Is Connected to Sleep

**原文标题**: Tinnitus Is Connected to Sleep

**原文链接**: [https://www.sciencealert.com/tinnitus-is-somehow-connected-to-a-crucial-bodily-function](https://www.sciencealert.com/tinnitus-is-somehow-connected-to-a-crucial-bodily-function)

生成摘要时出错

---

## 26. QGIS 4.0

**原文标题**: QGIS 4.0

**原文链接**: [https://changelog.qgis.org/en/version/4.0/](https://changelog.qgis.org/en/version/4.0/)

生成摘要时出错

---

## 27. US economy sheds 92,000 jobs in February in sharp slide

**原文标题**: US economy sheds 92,000 jobs in February in sharp slide

**原文链接**: [https://www.ft.com/content/6542bd0c-59ca-493b-ab5d-2d69e4e00cae](https://www.ft.com/content/6542bd0c-59ca-493b-ab5d-2d69e4e00cae)

生成摘要时出错

---

## 28. LibreOffice: Request to the European Commission to adhere to its own guidances

**原文标题**: LibreOffice: Request to the European Commission to adhere to its own guidances

**原文链接**: [https://blog.documentfoundation.org/blog/2026/03/05/cra-guidances/](https://blog.documentfoundation.org/blog/2026/03/05/cra-guidances/)

生成摘要时出错

---

## 29. I resigned from OpenAI

**原文标题**: I resigned from OpenAI

**原文链接**: [https://twitter.com/kalinowski007/status/2030320074121478618](https://twitter.com/kalinowski007/status/2030320074121478618)

生成摘要时出错

---

## 30. TSA leaves passenger needing surgery after illegally forcing her through scanner

**原文标题**: TSA leaves passenger needing surgery after illegally forcing her through scanner

**原文链接**: [https://www.thetravel.com/tsa-leaves-passenger-needing-surgery-after-illegally-forcing-her-through-scanner-spinal-cord-implant/](https://www.thetravel.com/tsa-leaves-passenger-needing-surgery-after-illegally-forcing-her-through-scanner-spinal-cord-implant/)

生成摘要时出错

---

## 31. PC processors entered the Gigahertz era today in the year 2000 with AMD's Athlon

**原文标题**: PC processors entered the Gigahertz era today in the year 2000 with AMD's Athlon

**原文链接**: [https://www.tomshardware.com/pc-components/cpus/pc-processors-entered-the-gigahertz-era-today-in-the-year-2000-with-amds-athlon-amd-hit-marketing-gold-with-its-1-ghz-athlon-beat-intel-by-a-nose](https://www.tomshardware.com/pc-components/cpus/pc-processors-entered-the-gigahertz-era-today-in-the-year-2000-with-amds-athlon-amd-hit-marketing-gold-with-its-1-ghz-athlon-beat-intel-by-a-nose)

生成摘要时出错

---

## 32. Sarvam 105B, the first competitive Indian open source LLM

**原文标题**: Sarvam 105B, the first competitive Indian open source LLM

**原文链接**: [https://www.sarvam.ai/blogs/sarvam-30b-105b](https://www.sarvam.ai/blogs/sarvam-30b-105b)

生成摘要时出错

---

## 33. New imagery suggests U.S. responsible for Iran school strike

**原文标题**: New imagery suggests U.S. responsible for Iran school strike

**原文链接**: [https://www.cnn.com/2026/03/06/world/video/updates-suggests-us-responsible-iran-school-strike-digvid](https://www.cnn.com/2026/03/06/world/video/updates-suggests-us-responsible-iran-school-strike-digvid)

生成摘要时出错

---

## 34. The surprising whimsy of the Time Zone Database

**原文标题**: The surprising whimsy of the Time Zone Database

**原文链接**: [https://muddy.jprs.me/links/2026-03-06-the-surprising-whimsy-of-the-time-zone-database/](https://muddy.jprs.me/links/2026-03-06-the-surprising-whimsy-of-the-time-zone-database/)

生成摘要时出错

---

## 35. Boy I was wrong about the Fediverse

**原文标题**: Boy I was wrong about the Fediverse

**原文链接**: [https://matduggan.com/boy-i-was-wrong-about-the-fediverse/](https://matduggan.com/boy-i-was-wrong-about-the-fediverse/)

生成摘要时出错

---

## 36. Autoresearch: Agents researching on single-GPU nanochat training automatically

**原文标题**: Autoresearch: Agents researching on single-GPU nanochat training automatically

**原文链接**: [https://github.com/karpathy/autoresearch](https://github.com/karpathy/autoresearch)

生成摘要时出错

---

## 37. Notes on writing Rust-based Wasm

**原文标题**: Notes on writing Rust-based Wasm

**原文链接**: [https://notes.brooklynzelenka.com/Blog/Notes-on-Writing-Wasm](https://notes.brooklynzelenka.com/Blog/Notes-on-Writing-Wasm)

生成摘要时出错

---

## 38. Training students to prove they're not robots is pushing them to use more AI

**原文标题**: Training students to prove they're not robots is pushing them to use more AI

**原文链接**: [https://www.techdirt.com/2026/03/06/were-training-students-to-write-worse-to-prove-theyre-not-robots-and-its-pushing-them-to-use-more-ai/](https://www.techdirt.com/2026/03/06/were-training-students-to-write-worse-to-prove-theyre-not-robots-and-its-pushing-them-to-use-more-ai/)

生成摘要时出错

---

## 39. Ada 2022

**原文标题**: Ada 2022

**原文链接**: [https://www.adaic.org/ada-resources/standards/ada22/](https://www.adaic.org/ada-resources/standards/ada22/)

生成摘要时出错

---

## 40. Show HN: µJS, a 5KB alternative to Htmx and Turbo with zero dependencies

**原文标题**: Show HN: µJS, a 5KB alternative to Htmx and Turbo with zero dependencies

**原文链接**: [https://mujs.org](https://mujs.org)

生成摘要时出错

---

## 41. Oracle may slash up to 30k jobs to fund AI data-centers as US banks retreat

**原文标题**: Oracle may slash up to 30k jobs to fund AI data-centers as US banks retreat

**原文链接**: [https://www.cio.com/article/4125103/oracle-may-slash-up-to-30000-jobs-to-fund-ai-data-center-expansion-as-us-banks-retreat.html](https://www.cio.com/article/4125103/oracle-may-slash-up-to-30000-jobs-to-fund-ai-data-center-expansion-as-us-banks-retreat.html)

生成摘要时出错

---

## 42. The shady world of IP leasing

**原文标题**: The shady world of IP leasing

**原文链接**: [https://acid.vegas/blog/the-shady-world-of-ip-leasing/](https://acid.vegas/blog/the-shady-world-of-ip-leasing/)

生成摘要时出错

---

## 43. Nintendo Sues U.S. Government for Tariff Refunds

**原文标题**: Nintendo Sues U.S. Government for Tariff Refunds

**原文链接**: [https://www.scribd.com/document/1008639172/Nintendo-Sues-U-S-Government-For-Tariff-Refunds](https://www.scribd.com/document/1008639172/Nintendo-Sues-U-S-Government-For-Tariff-Refunds)

生成摘要时出错

---

## 44. Lawmakers Want DoD Investigated for Biblical 'Armageddon' Claims

**原文标题**: Lawmakers Want DoD Investigated for Biblical 'Armageddon' Claims

**原文链接**: [https://www.military.com/daily-news/2026/03/06/lawmakers-want-dod-hegseth-investigated-biblical-armageddon-claims.html](https://www.military.com/daily-news/2026/03/06/lawmakers-want-dod-hegseth-investigated-biblical-armageddon-claims.html)

生成摘要时出错

---

## 45. C# strings silently kill your SQL Server indexes in Dapper

**原文标题**: C# strings silently kill your SQL Server indexes in Dapper

**原文链接**: [https://consultwithgriff.com/dapper-nvarchar-implicit-conversion-performance-trap](https://consultwithgriff.com/dapper-nvarchar-implicit-conversion-performance-trap)

生成摘要时出错

---

## 46. The worst acquisition in history, again

**原文标题**: The worst acquisition in history, again

**原文链接**: [https://www.profgmedia.com/p/the-worst-acquisition-in-history](https://www.profgmedia.com/p/the-worst-acquisition-in-history)

生成摘要时出错

---

## 47. LibreOffice Writer now supports Markdown

**原文标题**: LibreOffice Writer now supports Markdown

**原文链接**: [https://blog.documentfoundation.org/blog/2026/02/04/libreoffice-26-2-is-here/](https://blog.documentfoundation.org/blog/2026/02/04/libreoffice-26-2-is-here/)

生成摘要时出错

---

## 48. Verification debt: the hidden cost of AI-generated code

**原文标题**: Verification debt: the hidden cost of AI-generated code

**原文链接**: [https://fazy.medium.com/agentic-coding-ais-adolescence-b0d13452f981](https://fazy.medium.com/agentic-coding-ais-adolescence-b0d13452f981)

生成摘要时出错

---

## 49. Palantir and Anthropic AI helped the US hit 1k Iran targets in 24 hours

**原文标题**: Palantir and Anthropic AI helped the US hit 1k Iran targets in 24 hours

**原文链接**: [https://www.moneycontrol.com/europe/?url=https://www.moneycontrol.com/world/how-palantir-and-anthropic-ai-helped-the-us-hit-1-000-iran-targets-in-24-hours-article-13853331.html](https://www.moneycontrol.com/europe/?url=https://www.moneycontrol.com/world/how-palantir-and-anthropic-ai-helped-the-us-hit-1-000-iran-targets-in-24-hours-article-13853331.html)

生成摘要时出错

---

## 50. How Big Diaper absorbs billions of extra dollars from American parents

**原文标题**: How Big Diaper absorbs billions of extra dollars from American parents

**原文链接**: [https://thehustle.co/originals/how-big-diaper-absorbs-billions-of-extra-dollars-from-american-parents](https://thehustle.co/originals/how-big-diaper-absorbs-billions-of-extra-dollars-from-american-parents)

生成摘要时出错

---

## 51. $3T flows through U.S. nonprofits every year

**原文标题**: $3T flows through U.S. nonprofits every year

**原文链接**: [https://charitysense.com/insights/the-3-trillion-blind-spot](https://charitysense.com/insights/the-3-trillion-blind-spot)

生成摘要时出错

---

## 52. SWE-CI: Evaluating Agent Capabilities in Maintaining Codebases via CI

**原文标题**: SWE-CI: Evaluating Agent Capabilities in Maintaining Codebases via CI

**原文链接**: [https://arxiv.org/abs/2603.03823](https://arxiv.org/abs/2603.03823)

生成摘要时出错

---

## 53. Show HN: ANSI-Saver – A macOS Screensaver

**原文标题**: Show HN: ANSI-Saver – A macOS Screensaver

**原文链接**: [https://github.com/lardissone/ansi-saver](https://github.com/lardissone/ansi-saver)

生成摘要时出错

---

## 54. TypeScript 6.0 RC

**原文标题**: TypeScript 6.0 RC

**原文链接**: [https://devblogs.microsoft.com/typescript/announcing-typescript-6-0-rc/](https://devblogs.microsoft.com/typescript/announcing-typescript-6-0-rc/)

生成摘要时出错

---

## 55. MonoGame: A .NET framework for making cross-platform games

**原文标题**: MonoGame: A .NET framework for making cross-platform games

**原文链接**: [https://github.com/MonoGame/MonoGame](https://github.com/MonoGame/MonoGame)

生成摘要时出错

---

## 56. The stagnancy of publishing and the disappearance of the midlist

**原文标题**: The stagnancy of publishing and the disappearance of the midlist

**原文链接**: [https://www.honest-broker.com/p/the-day-ny-publishing-lost-its-soul](https://www.honest-broker.com/p/the-day-ny-publishing-lost-its-soul)

生成摘要时出错

---

## 57. I don't know if my job will still exist in ten years

**原文标题**: I don't know if my job will still exist in ten years

**原文链接**: [https://www.seangoedecke.com/will-my-job-still-exist/](https://www.seangoedecke.com/will-my-job-still-exist/)

生成摘要时出错

---

## 58. Some Words on WigglyPaint

**原文标题**: Some Words on WigglyPaint

**原文链接**: [https://beyondloom.com/blog/onwigglypaint.html](https://beyondloom.com/blog/onwigglypaint.html)

生成摘要时出错

---

## 59. Art Bits from HyperCard

**原文标题**: Art Bits from HyperCard

**原文链接**: [https://archives.somnolescent.net/web/mari_v2/junk/hypercard/](https://archives.somnolescent.net/web/mari_v2/junk/hypercard/)

生成摘要时出错

---

## 60. Show HN: Kula – Lightweight, self-contained Linux server monitoring tool

**原文标题**: Show HN: Kula – Lightweight, self-contained Linux server monitoring tool

**原文链接**: [https://github.com/c0m4r/kula](https://github.com/c0m4r/kula)

生成摘要时出错

---

## 61. To the Polypropylene Makers

**原文标题**: To the Polypropylene Makers

**原文链接**: [https://www.lesswrong.com/posts/HQTueNS4mLaGy3BBL/here-s-to-the-polypropylene-makers](https://www.lesswrong.com/posts/HQTueNS4mLaGy3BBL/here-s-to-the-polypropylene-makers)

生成摘要时出错

---

## 62. Re-creating the complex cuisine of prehistoric Europeans

**原文标题**: Re-creating the complex cuisine of prehistoric Europeans

**原文链接**: [https://arstechnica.com/science/2026/03/recreating-the-complex-cuisine-of-prehistoric-europeans/](https://arstechnica.com/science/2026/03/recreating-the-complex-cuisine-of-prehistoric-europeans/)

生成摘要时出错

---

## 63. Google just gave Sundar Pichai a $692M pay package

**原文标题**: Google just gave Sundar Pichai a $692M pay package

**原文链接**: [https://techcrunch.com/2026/03/07/google-just-gave-sundar-pichai-a-692m-pay-package/](https://techcrunch.com/2026/03/07/google-just-gave-sundar-pichai-a-692m-pay-package/)

生成摘要时出错

---

## 64. Claude struggles to cope with ChatGPT exodus

**原文标题**: Claude struggles to cope with ChatGPT exodus

**原文链接**: [https://www.forbes.com/sites/barrycollins/2026/03/06/claude-struggles-to-cope-with-chatgpt-exodus/](https://www.forbes.com/sites/barrycollins/2026/03/06/claude-struggles-to-cope-with-chatgpt-exodus/)

生成摘要时出错

---

## 65. Show HN: Curiosity – DIY 6" Newtonian Reflector Telescope

**原文标题**: Show HN: Curiosity – DIY 6" Newtonian Reflector Telescope

**原文链接**: [https://curiosity-telescope.vercel.app/](https://curiosity-telescope.vercel.app/)

生成摘要时出错

---

## 66. Does Apple‘s M5 Max Really “Destroy” a 96-Core Threadripper?

**原文标题**: Does Apple‘s M5 Max Really “Destroy” a 96-Core Threadripper?

**原文链接**: [https://slashdot.org/submission/17345398/does-apples-m5-max-really-destroy-a-96-core-threadripper](https://slashdot.org/submission/17345398/does-apples-m5-max-really-destroy-a-96-core-threadripper)

生成摘要时出错

---

## 67. Sem – Semantic version control. Entity-level diffs on top of Git

**原文标题**: Sem – Semantic version control. Entity-level diffs on top of Git

**原文链接**: [https://github.com/ataraxy-labs/sem](https://github.com/ataraxy-labs/sem)

生成摘要时出错

---

## 68. They all said Hormuz closure would be brief. What if they were wrong?

**原文标题**: They all said Hormuz closure would be brief. What if they were wrong?

**原文链接**: [https://www.lloydslist.com/LL1156532/They-all-said-Hormuz-closure-would-be-brief-What-if-they-were-wrong](https://www.lloydslist.com/LL1156532/They-all-said-Hormuz-closure-would-be-brief-What-if-they-were-wrong)

生成摘要时出错

---

## 69. Why it takes you and an elephant the same amount of time to poop (2017)

**原文标题**: Why it takes you and an elephant the same amount of time to poop (2017)

**原文链接**: [https://www.pbs.org/newshour/health/takes-elephant-amount-time-poop](https://www.pbs.org/newshour/health/takes-elephant-amount-time-poop)

生成摘要时出错

---

## 70. Why developers using AI are working longer hours

**原文标题**: Why developers using AI are working longer hours

**原文链接**: [https://www.scientificamerican.com/article/why-developers-using-ai-are-working-longer-hours/](https://www.scientificamerican.com/article/why-developers-using-ai-are-working-longer-hours/)

生成摘要时出错

---

## 71. The Banality of Surveillance

**原文标题**: The Banality of Surveillance

**原文链接**: [https://benn.substack.com/p/the-banality-of-surveillance](https://benn.substack.com/p/the-banality-of-surveillance)

生成摘要时出错

---

## 72. Living human brain cells play DOOM on a CL1 [video]

**原文标题**: Living human brain cells play DOOM on a CL1 [video]

**原文链接**: [https://www.youtube.com/watch?v=yRV8fSw6HaE](https://www.youtube.com/watch?v=yRV8fSw6HaE)

生成摘要时出错

---

## 73. My Homelab Setup

**原文标题**: My Homelab Setup

**原文链接**: [https://bryananthonio.com/blog/my-homelab-setup/](https://bryananthonio.com/blog/my-homelab-setup/)

生成摘要时出错

---

## 74. Will Claude Code ruin our team?

**原文标题**: Will Claude Code ruin our team?

**原文链接**: [https://justinjackson.ca/claude-code-ruin](https://justinjackson.ca/claude-code-ruin)

生成摘要时出错

---

## 75. Tech jobs are getting demolished in ways not seen since 2008

**原文标题**: Tech jobs are getting demolished in ways not seen since 2008

**原文链接**: [https://www.businessinsider.com/tech-jobs-getting-demolished-great-recession-dot-com-era-2026-3](https://www.businessinsider.com/tech-jobs-getting-demolished-great-recession-dot-com-era-2026-3)

生成摘要时出错

---

## 76. AI Error May Have Contributed to Girl's School Bombing in Iran

**原文标题**: AI Error May Have Contributed to Girl's School Bombing in Iran

**原文链接**: [https://thisweekinworcester.com/exclusive-ai-error-girls-school-bombing/](https://thisweekinworcester.com/exclusive-ai-error-girls-school-bombing/)

生成摘要时出错

---

## 77. LLM Doesn't Write Correct Code. It Writes Plausible Code

**原文标题**: LLM Doesn't Write Correct Code. It Writes Plausible Code

**原文链接**: [https://twitter.com/KatanaLarp/status/2029928471632224486](https://twitter.com/KatanaLarp/status/2029928471632224486)

生成摘要时出错

---

## 78. Beagle, a source code management system that stores AST trees

**原文标题**: Beagle, a source code management system that stores AST trees

**原文链接**: [https://github.com/gritzko/librdx/tree/master/be](https://github.com/gritzko/librdx/tree/master/be)

生成摘要时出错

---

## 79. Show HN: Eyot, A programming language where the GPU is just another thread

**原文标题**: Show HN: Eyot, A programming language where the GPU is just another thread

**原文链接**: [https://cowleyforniastudios.com/2026/03/08/announcing-eyot/](https://cowleyforniastudios.com/2026/03/08/announcing-eyot/)

生成摘要时出错

---

## 80. Lisp-style C++ template meta programming

**原文标题**: Lisp-style C++ template meta programming

**原文链接**: [https://github.com/mistivia/lmp](https://github.com/mistivia/lmp)

生成摘要时出错

---

## 81. Show HN: I open-sourced my Steam game, 100% written in Lua, engine is also open

**原文标题**: Show HN: I open-sourced my Steam game, 100% written in Lua, engine is also open

**原文链接**: [https://github.com/willtobyte/reprobate](https://github.com/willtobyte/reprobate)

生成摘要时出错

---

## 82. The Case of the Disappearing Secretary

**原文标题**: The Case of the Disappearing Secretary

**原文链接**: [https://rowlandmanthorpe.substack.com/p/the-case-of-the-disappearing-secretary](https://rowlandmanthorpe.substack.com/p/the-case-of-the-disappearing-secretary)

生成摘要时出错

---

## 83. Israel Strikes Oil Facilities in Iran

**原文标题**: Israel Strikes Oil Facilities in Iran

**原文链接**: [https://www.nytimes.com/2026/03/07/world/middleeast/israel-iran-oil-strikes.html](https://www.nytimes.com/2026/03/07/world/middleeast/israel-iran-oil-strikes.html)

生成摘要时出错

---

## 84. Science Fiction Is Dying. Long Live Post Sci-Fi?

**原文标题**: Science Fiction Is Dying. Long Live Post Sci-Fi?

**原文链接**: [https://www.typebarmagazine.com/science-fiction-is-dying-long-live-post-sci-fi/](https://www.typebarmagazine.com/science-fiction-is-dying-long-live-post-sci-fi/)

生成摘要时出错

---

## 85. Fork Off: Surveillance States Need to Fork Linux Themselves

**原文标题**: Fork Off: Surveillance States Need to Fork Linux Themselves

**原文链接**: [https://blog.devrupt.io/posts/fork-off-california-linux/](https://blog.devrupt.io/posts/fork-off-california-linux/)

生成摘要时出错

---

## 86. I'm Not Consulting an LLM

**原文标题**: I'm Not Consulting an LLM

**原文链接**: [https://lr0.org/blog/p/gpt/](https://lr0.org/blog/p/gpt/)

生成摘要时出错

---

## 87. Give Up GitHub – Software Freedom Conservancy

**原文标题**: Give Up GitHub – Software Freedom Conservancy

**原文链接**: [https://sfconservancy.org/GiveUpGitHub/](https://sfconservancy.org/GiveUpGitHub/)

生成摘要时出错

---

## 88. Iranian Women Graduate in Stem 3× the Rate of U.S. Women and Has 5× More PhDs

**原文标题**: Iranian Women Graduate in Stem 3× the Rate of U.S. Women and Has 5× More PhDs

**原文链接**: [https://hrnews1.substack.com/p/iranian-women-graduate-in-stem-at](https://hrnews1.substack.com/p/iranian-women-graduate-in-stem-at)

生成摘要时出错

---

## 89. AI and the Illegal War

**原文标题**: AI and the Illegal War

**原文链接**: [https://buttondown.com/creativegood/archive/ai-and-the-illegal-war/](https://buttondown.com/creativegood/archive/ai-and-the-illegal-war/)

生成摘要时出错

---

## 90. The new Apple begins to emerge

**原文标题**: The new Apple begins to emerge

**原文链接**: [https://parkerortolani.blog/2026/03/07/the-new-apple-finally-begins.html](https://parkerortolani.blog/2026/03/07/the-new-apple-finally-begins.html)

生成摘要时出错

---

## 91. What if AI just makes us work harder?

**原文标题**: What if AI just makes us work harder?

**原文链接**: [https://www.ft.com/content/e8bb5ab1-4b4d-473e-8f76-e690443e9fb4](https://www.ft.com/content/e8bb5ab1-4b4d-473e-8f76-e690443e9fb4)

生成摘要时出错

---

## 92. CLI RSS/Atom feed reader inspired by Taskwarrior, synced using Git

**原文标题**: CLI RSS/Atom feed reader inspired by Taskwarrior, synced using Git

**原文链接**: [https://github.com/kantord/blogtato](https://github.com/kantord/blogtato)

生成摘要时出错

---

## 93. What if the Apple ][ had run on Field-Sequential?

**原文标题**: What if the Apple ][ had run on Field-Sequential?

**原文链接**: [https://nicole.express/2026/the-apple-that-wasnt.html](https://nicole.express/2026/the-apple-that-wasnt.html)

生成摘要时出错

---

## 94. SPA vs. Hypermedia: Real-World Performance Under Load

**原文标题**: SPA vs. Hypermedia: Real-World Performance Under Load

**原文链接**: [https://zweiundeins.gmbh/en/methodology/spa-vs-hypermedia-real-world-performance-under-load](https://zweiundeins.gmbh/en/methodology/spa-vs-hypermedia-real-world-performance-under-load)

生成摘要时出错

---

## 95. John C. Dvorak – heart attack – in hospital

**原文标题**: John C. Dvorak – heart attack – in hospital

**原文链接**: [https://www.noagendashow.net/listen/1848?t=1:24](https://www.noagendashow.net/listen/1848?t=1:24)

生成摘要时出错

---

## 96. Apple Used to Design Its Laptops for Repairability

**原文标题**: Apple Used to Design Its Laptops for Repairability

**原文链接**: [https://www.ifixit.com/News/115995/how-apple-used-to-design-its-laptops-for-repairability](https://www.ifixit.com/News/115995/how-apple-used-to-design-its-laptops-for-repairability)

生成摘要时出错

---

## 97. Global Warming Has Accelerated Significantly

**原文标题**: Global Warming Has Accelerated Significantly

**原文链接**: [https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2025GL118804](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2025GL118804)

生成摘要时出错

---

## 98. Utah's online porn tax proposal poses a major threat to civil liberties

**原文标题**: Utah's online porn tax proposal poses a major threat to civil liberties

**原文链接**: [https://www.techdirt.com/2026/03/06/utahs-proposal-to-tax-online-pornography-is-a-civil-liberties-disaster-waiting-to-happen/](https://www.techdirt.com/2026/03/06/utahs-proposal-to-tax-online-pornography-is-a-civil-liberties-disaster-waiting-to-happen/)

生成摘要时出错

---

## 99. If It Quacks Like a Package Manager

**原文标题**: If It Quacks Like a Package Manager

**原文链接**: [https://nesbitt.io/2026/03/08/if-it-quacks-like-a-package-manager.html](https://nesbitt.io/2026/03/08/if-it-quacks-like-a-package-manager.html)

生成摘要时出错

---

## 100. When DOGE Unleashed ChatGPT on the National Endowment for the Humanities

**原文标题**: When DOGE Unleashed ChatGPT on the National Endowment for the Humanities

**原文链接**: [https://www.nytimes.com/2026/03/07/arts/humanities-endowment-doge-trump.html](https://www.nytimes.com/2026/03/07/arts/humanities-endowment-doge-trump.html)

生成摘要时出错

---

