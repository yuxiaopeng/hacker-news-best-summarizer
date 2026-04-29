# Hacker News 热门文章摘要 (2026-04-29)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 德国弹药产能超越美国

**原文标题**: Germany Overtakes US in Ammunition Production Capacity

**原文链接**: [https://www.newsweek.com/germany-overtakes-us-in-ammunition-production-capacity-11886409](https://www.newsweek.com/germany-overtakes-us-in-ammunition-production-capacity-11886409)

德国国防巨头莱茵金属据报道已在弹药生产能力上超越美国，这标志着欧洲各地正在进行一场大规模的重整军备运动。莱茵金属首席执行官阿明·佩珀格表示，年度炮弹产量已从7万枚激增至110万枚，中口径弹药产量翻了两番。

这一推动主要受美国总统唐纳德·特朗普的警告所影响，他呼吁北约成员国增加国防开支并减少对华盛顿的依赖。美国正将重心转向印太地区，并卷入中东冲突，这使得欧洲不得不加强自身安全。对美国在俄罗斯侵略情况下的承诺以及援乌导致库存耗尽的担忧，进一步加剧了欧洲的努力。

作为回应，北约国家在2025年6月承诺，在十年内将国内生产总值的5%用于军事开支。德国总理弗里德里希·默茨正主导大幅增加德国国防开支，这与二战后的政策背道而驰。国防部长鲍里斯·皮斯托利乌斯的目标是到2039年，使德国拥有“欧洲最强大的常规军队”。

由于乌克兰战争，弹药，尤其是155毫米炮弹，需求旺盛。莱茵金属自2022年以来一直在增产，并于去年八月开设了一家新工厂，该工厂有望成为欧洲最大的弹药工厂。北约秘书长马克·吕特强调了对更多弹药和防空系统的关键需求。

---

## 2. 一份好的 AGENTS.md 是模型升级。一份糟糕的则比完全没有文档更糟。

**原文标题**: A good AGENTS.md is a model upgrade. A bad one is worse than no docs at all

**原文链接**: [https://www.augmentcode.com/blog/how-to-write-good-agents-dot-md-files](https://www.augmentcode.com/blog/how-to-write-good-agents-dot-md-files)

对AGENTS.md文件的研究表明，它们对AI编码代理的性能有着深远而多样的影响，既能显著提升代码质量，也能使输出质量比没有文档时更差。

有效的AGENTS.md模式包括：
1.  **渐进式披露：**主文件简洁（100-150行），详细信息推迟到专注的、按需引用的参考文件中。
2.  **程序化工作流：**针对任务的带编号多步骤指令可显著提高完成率。
3.  **决策表：**解决常见选择的歧义，增强对代码库约定的遵守。
4.  **真实代码示例：**生产代码中短小（3-10行）的片段可提高重用性和模式遵循。
5.  **领域特定规则：**具体的、可强制执行的“易错点”能够改进最佳实践。
6.  **“禁止”与“允许”搭配：**将禁止事项与具体的替代方案配对，可防止过度探索。
7.  **模块化文档：**针对独立的中等规模子模块（约100个核心文件）的AGENTS.md文件能带来最佳收益。

相反，常见的陷阱，如“过度探索”或“上下文腐烂”，会损害性能：
1.  **过多的架构概述：**过于详细会导致代理加载不相关的上下文，从而引发混乱和不完整的解决方案。
2.  **过多的警告/禁止事项：**冗长的禁止事项列表，如果没有“允许”的替代方案，会使代理过度探索并变得过于谨慎。
3.  **过时的文档：**当需要新架构时，AGENTS.md可能会引导代理采用旧模式。

AGENTS.md是最可靠的文档发现位置。迁移时，请精简面向人类的README文件，通过引用重用高质量的现有文档，并解决模块中更广泛的“文档蔓延”问题，因为代理会找到所有相关的文档。优化AGENTS.md的简洁性、任务相关性以及具体的、可操作的指导，以显著提高代理的代码生成能力。

---

## 3. 胡萝卜披露：Forgejo

**原文标题**: Carrot Disclosure: Forgejo

**原文链接**: [https://dustri.org/b/carrot-disclosure-forgejo.html](https://dustri.org/b/carrot-disclosure-forgejo.html)

Fedora迁移到Forgejo的举动促使作者进行了一项安全审查，在一个晚上就发现了许多漏洞。这些漏洞包括SSRF、缺乏CSP/Trusted-Types、加密实践不当、认证机制缺陷、各种拒绝服务攻击、信息泄露以及TOCTOU问题。将其中一些漏洞串联起来，可导致完整的远程代码执行（RCE）、秘密泄露、持久账户访问和OAuth2权限提升。

尽管RCE需要开放注册和非默认配置（尽管在某些实例中存在），但作者决定不采用传统的漏洞披露方式。鉴于“糟糕的代码库状态”（继承自Gitea/Gogs）和系统性问题，他们认为单独的修复是“无止境的打地鼠游戏”。

相反，作者选择了“胡萝卜式披露”：发布经过编辑的关键漏洞利用输出，以激励供应商进行全面的安全审计，否则将面临失去用户的风险。文章通过`chain_alpha.py`的输出来展示了这一点，显示了管理员后门的创建以及通过服务器端Git钩子确认的RCE，在目标上执行了`hostname`和`id`等命令。作者的漏洞利用目录还揭示了更广泛的漏洞集合，包括更多的RCE链和各种DoS漏洞利用。

---

## 4. NPM website was down

**原文标题**: NPM website was down

**原文链接**: [https://status.npmjs.org](https://status.npmjs.org)

NPM状态页显示，截至世界协调时2026年4月29日20:07，“npm网站问题”目前正在调查中。`www.npmjs.com`网站正在经历“性能下降”，并在过去90天内记录了99.92%的正常运行时间。

然而，其他关键服务，例如包安装、包发布、包搜索、安全审计和复制源，在相同的90天内均显示为“正常运行”，并保持100%的正常运行时间。

近期影响npm网站的事件包括：
*   **2026年4月29日：** 查看包和登录npmjs.com时出现性能下降，该问题从世界协调时16:48开始调查，并于19:35解决。
*   **2026年4月28日：** 网站服务性能下降，调查从世界协调时19:55开始，于22:24解决。
*   **2026年4月27日：** npm网站不可用，该问题从世界协调时21:06开始调查，于22:30解决。

该状态页提供选项，用户可以订阅电子邮件或短信通知，在Twitter上关注@npmstatus，或使用Atom/RSS订阅源获取更新。

---

## 5. 威斯奈尔的大衣和我

**原文标题**: Withnail's Coat and I

**原文链接**: [https://ontherow.substack.com/p/withnails-coat-and-i](https://ontherow.substack.com/p/withnails-coat-and-i)

文章《Withnail's Coat and I》深入探讨了作者与电影《Withnail & I》之间深刻而持久的联系，特别是聚焦于片中主角所穿的标志性粗花呢外套。作者描述了一种拥有与威特耐尔（Withnail）外套风格相似的、能体现“没落乡绅”美学的外套的强烈愿望——它沉重、斑驳、结实，略显宽松，而非现代轻薄的粗花呢款式。

寻找这种特定类型外套的过程异常艰难。大量的在线搜索结果都差强人意，很多都过于轻薄、剪裁过于合身，或缺乏那种地道、厚重的感觉。作者想要一件“合适”且耐用、而非仅仅时髦的外套，它能像威特耐尔那身常年不整的装束一样经受风吹雨打。

漫长的寻觅最终在eBay上有所斩获：一件以60英镑购得的复古男士猎装夹克。收到外套后，它的重量和质感立刻给人留下深刻印象。尽管它并非威特耐尔外套的精确复制品，但却具备了作者所寻求的关键特质：厚重、斑驳的粗花呢面料、宽大的衣领，以及一种恰到好处的、略显宽松的剪裁。

最终，作者认定这件复古外套就是“他们的”威特耐尔大衣。它成功地捕捉到了所追求的美学和感觉，实现了作者长久以来的个人愿望。这件外套现在已成为日常生活中珍贵而实用的物品，它体现了作者对这部挚爱电影的深切个人联系，而不仅仅是一件纪念品。

---

## 6. 200名记者赞扬互联网档案馆在保存公共记录方面的作用

**原文标题**: 200 Journalists Applaud the Internet Archive's Role in Preserving Public Record

**原文链接**: [https://www.savethearchive.com/journalists/](https://www.savethearchive.com/journalists/)

超过200名记者公开感谢并赞扬互联网档案馆（IA）及其“回溯机器”，因其在保存新闻和公共记录方面的关键作用。这种集体支持出现之际，主要媒体正在考虑是否允许该档案继续保存新闻内容，部分原因是出于对人工智能的担忧。

记者们称赞IA是不可或缺的“国家宝藏”和“基本服务”。包括雷切尔·马多（Rachel Maddow）在内的许多人每天使用它进行事实核查、验证机构声明，并追踪网站、文档和叙述随时间的变化。记者们强调其作为“取证工具”和“公共账本”的价值，以对抗“记忆删除”（memory-holing）现象——即数字内容可能被修改或删除，从而使问责制变得脆弱。

提供的例子展示了它在揭露被篡改的警方声明、追踪政治团体的消息发布、验证出版时间线以及找回丢失的调查证据方面的实用性。它对于获取稀有的学术书籍、“新闻荒漠”中的旧新闻文章以及对抗“链接失效”（link rot）也至关重要。记者们强调，IA确保了历史准确性和新闻业的诚信，它作为一个类似于国家图书馆的全球资源，对于保存数字文化以及对抗审查制度和强大机构的反复无常、维护一个连贯、知情的集体历史至关重要。

---

## 7. An open-source stethoscope that costs between $2.5 and $5 to produce

**原文标题**: An open-source stethoscope that costs between $2.5 and $5 to produce

**原文链接**: [https://github.com/GliaX/Stethoscope](https://github.com/GliaX/Stethoscope)

This project presents an open-source, research-validated stethoscope designed for low-cost production, targeting $2.50 to $5.00 per unit. Crucially, its performance matches that of the market gold standard, the Littmann Cardiology III, a claim supported by a peer-reviewed publication.

The Bill of Materials includes five 3D-printed components: a stethoscope head, two ear tubes, a Y-piece, a spring, and a ring. These are combined with off-the-shelf parts: translucent silicone rubber tubing (8mm ID/13mm OD and 4mm ID/8mm OD), a 40mm diaphragm cut from approximately 0.35mm plastic report cover material, and large-sized standard earbuds.

Printing instructions are stringent, demanding **100% infill** for all parts, as this is vital for proper acoustic function. PETG or ABS filament is recommended over PLA due to durability and heat deformation concerns. A 0.2mm layer height is specified, with users advised to import a 3MF file into PrusaSlicer 2.0+ and avoid modifying print settings, though minor scaling for fit (e.g., spring or head) is acceptable.

Assembly involves attaching the diaphragm, connecting the silicone tubing to the head and Y-piece, and integrating the spring, ear tubes, and eartips. An instructional video is available. The design files were created using CrystalSCAD and OpenSCAD, with instructions for generating SCAD files provided. The project offers mass manufacturing guidelines, including a serial numbering system and printing multiple units per plate. The work is shared under the TAPR OHL license.

---

## 8. Show HN: Rocky – Rust SQL engine with branches, replay, column lineage

**原文标题**: Show HN: Rocky – Rust SQL engine with branches, replay, column lineage

**原文链接**: [https://github.com/rocky-data/rocky](https://github.com/rocky-data/rocky)

生成摘要时出错

---

## 9. Linux 7.0 Broke PostgreSQL: The Preemption Regression Explained

**原文标题**: Linux 7.0 Broke PostgreSQL: The Preemption Regression Explained

**原文链接**: [https://read.thecoder.cafe/p/linux-broke-postgresql](https://read.thecoder.cafe/p/linux-broke-postgresql)

生成摘要时出错

---

## 10. Integrated by Design

**原文标题**: Integrated by Design

**原文链接**: [https://vivianvoss.net/blog/integrated-by-design-launch](https://vivianvoss.net/blog/integrated-by-design-launch)

生成摘要时出错

---

## 11. Letting AI play my game – building an agentic test harness to help play-testing

**原文标题**: Letting AI play my game – building an agentic test harness to help play-testing

**原文链接**: [https://blog.jeffschomay.com/letting-ai-play-my-game](https://blog.jeffschomay.com/letting-ai-play-my-game)

生成摘要时出错

---

## 12. We decreased our LLM costs with Opus

**原文标题**: We decreased our LLM costs with Opus

**原文链接**: [https://www.mendral.com/blog/frontier-model-lower-costs](https://www.mendral.com/blog/frontier-model-lower-costs)

生成摘要时出错

---

## 13. Laguna XS.2 and M.1

**原文标题**: Laguna XS.2 and M.1

**原文链接**: [https://poolside.ai/blog/laguna-a-deeper-dive](https://poolside.ai/blog/laguna-a-deeper-dive)

生成摘要时出错

---

## 14. Court Rules 2nd Amendment Covers Firearms Parts Good News Those Who Build Guns

**原文标题**: Court Rules 2nd Amendment Covers Firearms Parts Good News Those Who Build Guns

**原文链接**: [https://cowboystatedaily.com/2026/04/28/court-rules-2nd-amendment-covers-firearms-parts-good-news-for-those-who-build-guns/](https://cowboystatedaily.com/2026/04/28/court-rules-2nd-amendment-covers-firearms-parts-good-news-for-those-who-build-guns/)

生成摘要时出错

---

## 15. GitHub – DOS 1.0: Transcription of Tim Paterson's DOS Printouts

**原文标题**: GitHub – DOS 1.0: Transcription of Tim Paterson's DOS Printouts

**原文链接**: [https://github.com/DOS-History/Paterson-Listings](https://github.com/DOS-History/Paterson-Listings)

生成摘要时出错

---

## 16. After Spain's blackout, its shift to renewables and grid evolution power on

**原文标题**: After Spain's blackout, its shift to renewables and grid evolution power on

**原文链接**: [https://www.theguardian.com/world/2026/apr/28/blackout-spain-renewable-energy-grid-solar-wind](https://www.theguardian.com/world/2026/apr/28/blackout-spain-renewable-energy-grid-solar-wind)

生成摘要时出错

---

## 17. L123: A Lotus 1-2-3–style terminal spreadsheet with modern Excel compatibility

**原文标题**: L123: A Lotus 1-2-3–style terminal spreadsheet with modern Excel compatibility

**原文链接**: [https://github.com/duane1024/l123](https://github.com/duane1024/l123)

生成摘要时出错

---

## 18. "People who don't use AI will be left behind"

**原文标题**: "People who don't use AI will be left behind"

**原文链接**: [https://migrainebrain.bearblog.dev/people-who-dont-use-ai-will-be-left-behind/](https://migrainebrain.bearblog.dev/people-who-dont-use-ai-will-be-left-behind/)

生成摘要时出错

---

## 19. U.S. war in Iran has cost $25B so far, says Pentagon official

**原文标题**: U.S. war in Iran has cost $25B so far, says Pentagon official

**原文链接**: [https://www.reuters.com/world/middle-east/us-war-iran-has-cost-25-billion-so-far-says-pentagon-official-2026-04-29/](https://www.reuters.com/world/middle-east/us-war-iran-has-cost-25-billion-so-far-says-pentagon-official-2026-04-29/)

生成摘要时出错

---

## 20. A playable DOOM MCP app

**原文标题**: A playable DOOM MCP app

**原文链接**: [https://chrisnager.com/blog/doom-runs-in-chatgpt-and-claude/](https://chrisnager.com/blog/doom-runs-in-chatgpt-and-claude/)

生成摘要时出错

---

## 21. Coffee with a splash of physics: how to make the most out of your brew

**原文标题**: Coffee with a splash of physics: how to make the most out of your brew

**原文链接**: [https://physicsworld.com/a/coffee-with-a-splash-of-physics-how-to-make-the-most-out-of-your-brew/](https://physicsworld.com/a/coffee-with-a-splash-of-physics-how-to-make-the-most-out-of-your-brew/)

生成摘要时出错

---

## 22. When the Internet Was a Place (2025)

**原文标题**: When the Internet Was a Place (2025)

**原文链接**: [https://www.frontporchrepublic.com/2025/09/when-the-internet-was-a-place/](https://www.frontporchrepublic.com/2025/09/when-the-internet-was-a-place/)

生成摘要时出错

---

## 23. New gas-powered data centers could emit more greenhouse gases than whole nations

**原文标题**: New gas-powered data centers could emit more greenhouse gases than whole nations

**原文链接**: [https://www.wired.com/story/new-gas-powered-data-centers-could-emit-more-greenhouse-gases-than-entire-nations/](https://www.wired.com/story/new-gas-powered-data-centers-could-emit-more-greenhouse-gases-than-entire-nations/)

生成摘要时出错

---

## 24. Apple CMF (Color-Matching Functions) 2026

**原文标题**: Apple CMF (Color-Matching Functions) 2026

**原文链接**: [https://www.lttlabs.com/articles/2026/04/11/apple-studio-display-xdr-display-testing-results](https://www.lttlabs.com/articles/2026/04/11/apple-studio-display-xdr-display-testing-results)

生成摘要时出错

---

## 25. Denuvo has been cracked in all single-player games it previously protected

**原文标题**: Denuvo has been cracked in all single-player games it previously protected

**原文链接**: [https://www.tomshardware.com/video-games/pc-gaming/denuvo-has-been-bypassed-in-all-single-player-games-it-previously-protected-2k-games-and-denuvo-reportedly-retaliate-with-mandatory-14-day-online-checks](https://www.tomshardware.com/video-games/pc-gaming/denuvo-has-been-bypassed-in-all-single-player-games-it-previously-protected-2k-games-and-denuvo-reportedly-retaliate-with-mandatory-14-day-online-checks)

生成摘要时出错

---

## 26. OpenAI Misses Key Revenue, User Targets in High-Stakes Sprint Toward IPO

**原文标题**: OpenAI Misses Key Revenue, User Targets in High-Stakes Sprint Toward IPO

**原文链接**: [https://www.wsj.com/tech/ai/openai-misses-key-revenue-user-targets-in-high-stakes-sprint-toward-ipo-94a95273](https://www.wsj.com/tech/ai/openai-misses-key-revenue-user-targets-in-high-stakes-sprint-toward-ipo-94a95273)

生成摘要时出错

---

## 27. Show HN: Adblock-rust Manager – Firefox extension to enable the Brave ad blocker

**原文标题**: Show HN: Adblock-rust Manager – Firefox extension to enable the Brave ad blocker

**原文链接**: [https://github.com/electricant/adblock-rust-manager](https://github.com/electricant/adblock-rust-manager)

生成摘要时出错

---

## 28. Why Law Is Law-Shaped

**原文标题**: Why Law Is Law-Shaped

**原文链接**: [https://lawvm.org/why-law-is-law-shaped/](https://lawvm.org/why-law-is-law-shaped/)

生成摘要时出错

---

## 29. I quit drinking for a year

**原文标题**: I quit drinking for a year

**原文链接**: [https://dynomight.net/drinking/](https://dynomight.net/drinking/)

生成摘要时出错

---

## 30. Laws of UX

**原文标题**: Laws of UX

**原文链接**: [https://lawsofux.com/](https://lawsofux.com/)

生成摘要时出错

---

