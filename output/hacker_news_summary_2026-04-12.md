# Hacker News 热门文章摘要 (2026-04-12)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 锉掉我的 MacBook 的边角

**原文标题**: Filing the corners off my MacBooks

**原文链接**: [https://kentwalters.com/posts/corners/](https://kentwalters.com/posts/corners/)

作者详细介绍了他们将MacBook锋利的铝制边角打磨圆润的做法，这项定制他们预计会让其他人感到不解甚至震惊。他们的主要动机是锋利的底部边缘对手腕造成的不适，同时他们坚信应该将自己的工具个性化。

这项改造尤其集中在屏幕凹槽附近的尖锐区域，作者在那里小心翼翼地打磨出了新的、更柔和的曲线。整个过程包括夹紧MacBook，并用胶带封住扬声器和键盘等敏感区域，以防止铝屑进入。他们先用粗锉刀打磨，然后用150和400目砂纸将表面打磨光滑，并对结果表示满意。尽管最初担心会打磨穿机器，但事实证明这并非问题。

这次改造是在一台工作电脑上进行的，作者计划未来也会以类似方式改造其他机器。他们积极鼓励其他人克服对定制自己设备的任何顾虑，敦促他们“放开手脚去折腾一下”，并向那些考虑此类改造的人提供支持。

---

## 2. 阿耳忒弥斯2号安全溅落

**原文标题**: Artemis II safely splashes down

**原文链接**: [https://www.cbsnews.com/live-updates/artemis-ii-splashdown-return/](https://www.cbsnews.com/live-updates/artemis-ii-splashdown-return/)

美国国家航空航天局（NASA）的“阿尔忒弥斯2号”任务于2026年4月10日星期五成功结束，猎户座飞船于美国东部时间晚上8点07分在圣迭戈海岸附近的太平洋安全溅落。四名宇航员——指挥官里德·怀斯曼、飞行员维克多·格洛弗、任务专家克里斯蒂娜·科赫和加拿大宇航员杰里米·汉森——在结束了为期10天的任务后返回地球，此次任务创下了人类太空旅行最远距离的记录。

再入过程包括高速下降、在防热罩承受极端温度时有6分钟的通信中断，以及精确的降落伞部署，最终实现了“完美靶心式溅落”。海军回收人员利用充气筏和直升机迅速抵达飞船。在潜水员对“猎户座”内部进行初步医疗检查后，宇航员们走出飞船，表示他们感觉“很棒”，随后被送往“约翰·P·默萨号”（USS John P. Murtha）进行进一步评估。

NASA官员在溅落后的新闻发布会上表达了极大的自豪和兴奋，称赞此次任务是“一个不可思议的结局”和“太空探索新时代的开始”。特朗普总统也祝贺了宇航员们完成了“壮观的”任务。此次成功返回标志着未来月球探索迈出了重要一步。

---

## 3. Small models also found the vulnerabilities that Mythos found

**原文标题**: Small models also found the vulnerabilities that Mythos found

**原文链接**: [https://aisle.com/blog/ai-cybersecurity-after-mythos-the-jagged-frontier](https://aisle.com/blog/ai-cybersecurity-after-mythos-the-jagged-frontier)

生成摘要时出错

---

## 4. 我用每月20美元的技术栈，运营多个MRR达1万美元的公司。

**原文标题**: I run multiple $10K MRR companies on a $20/month tech stack

**原文链接**: [https://stevehanov.ca/blog/how-i-run-multiple-10k-mrr-companies-on-a-20month-tech-stack](https://stevehanov.ca/blog/how-i-run-multiple-10k-mrr-companies-on-a-20month-tech-stack)

这位作者是websequencediagrams.com等产品的幕后推手，一位经验丰富的白手起家者。他提倡通过最小化的技术栈来运营精益创业公司，这与风险投资模式的高烧钱率形成鲜明对比。他展示了如何以每月20美元的开销，实现多家月经常性收入（MRR）达到1万美元的公司。

他的策略包括：
1.  **精益服务器：** 利用Linode或DigitalOcean等提供商每月5-10美元的单一虚拟私有服务器（VPS），放弃AWS EKS/RDS等复杂昂贵的云设置，以实现简单性和成本效益。
2.  **精益语言：** 使用Go开发后端，这是一种性能高、内存效率高的语言，可编译成单个静态链接的二进制文件，从而简化部署和资源使用。
3.  **本地AI处理长时间运行的任务：** 利用个人GPU硬件（例如RTX 3090），配合Ollama、VLLM和Transformer Lab等工具进行免费的AI批量处理，例如总结数千份报告，而不是产生数百美元的云API费用。他还提到了`laconic`和`llmhub`来管理本地LLM。
4.  **OpenRouter实现快速/智能LLM：** 使用OpenRouter访问Claude 3.5 Sonnet或GPT-4o等尖端LLM，用于用户交互。这简化了API管理，整合了账单，并实现了不同提供商之间的自动回退。
5.  **Copilot用于AI IDE：** 在VS Code中利用GitHub Copilot的“按请求计费”模式，每次详细提示大约0.04美元，即可获得大量的AI编码辅助，无论计算持续时间多长。
6.  **SQLite处理所有事务：** 将SQLite作为主要数据库，并强调在启用预写式日志（WAL）的情况下，它具有速度和可扩展性，并提供定制的`smhanov/auth`库用于用户认证。

这种方法提供了无限的运营空间，减轻了压力，并使创始人能够专注于产品市场契合度，而无需承受来自投资者的持续压力或高昂的运营成本。

---

## 5. 安装所有 Firefox 扩展

**原文标题**: Installing every* Firefox extension

**原文链接**: [https://jack.cab/blog/every-firefox-extension](https://jack.cab/blog/every-firefox-extension)

这篇文章详细介绍了一个雄心勃勃的项目，旨在抓取并分析所有Firefox扩展。作者最初在使用Firefox Add-ons API时遇到了困难，由于页面限制和排序约束，只抓取到了30,000个扩展。通过迭代方法，包括多种排序、最终并行按类别查询，以及后续使用日期过滤器，作者成功抓取了84,235个独特的扩展，总计49.3 GB。

分析该数据集揭示了以下几点洞察。最大的扩展是dmitlichess (196.3 MB)，包含2000多个音频文件，而其他扩展则嵌入了Unity应用程序、Tesseract.js或AI模型。最小的扩展是theTabs-saver，大小为7518字节，不含任何代码。由“lolicon”开发的“Tab Stack for Firefox”被评为评分最差的扩展，“Dr. B”则是最多产的开发者，拥有84个“直觉编码”（vibe coded）的扩展。

分析揭示了恶意内容，包括使用同形异义字攻击（homoglyph attacks）和NocoDB来获取钓鱼URL的钓鱼扩展，以及带有可疑主页链接的SEO垃圾邮件扩展。很大一部分涉及来自“Innover Online Group Ltd”和“Atom Apps”等实体的潜在有害应用程序（PUA）。这些公司在不同平台发布了大量扩展（例如“Maps Assist & Custom Web Search”），通常将Yahoo与推广代码集成，共同吸引了数十万用户，其中一些后来被Mozilla禁用。

统计数据显示，34.3%的扩展没有日活跃用户，76.7%是开源的，23%是在本文开始撰写后创建的。文章最后通过获取所有扩展的直接下载URL，以便于批量安装。

---

## 6. Pro Max 5倍配额在1.5小时内用尽，尽管使用量适中

**原文标题**: Pro Max 5x quota exhausted in 1.5 hours despite moderate usage

**原文链接**: [https://github.com/anthropics/claude-code/issues/45756](https://github.com/anthropics/claude-code/issues/45756)

一位使用Claude Code Pro Max 5x (Opus, 1M 上下文) 套餐的用户报告称，尽管是适度使用，但其配额在1.5小时内就耗尽了。这出乎意料，尤其是与之前在高强度开发下持续了5小时的配额窗口期相比，那是一个预期结果。

核心问题似乎是，受益于提示缓存的 `cache_read` 令牌，在计入用户配额时似乎是按全额费率计算的。这抵消了缓存的成本降低优势，导致配额耗尽速度大大加快。数据显示，如果 `cache_read` 令牌以降低的1/10费率（即预期成本）计算，中度使用每小时仅消耗8.7M令牌。然而，如果以全额费率计算（疑似的实际行为），将达到每小时70.5M令牌，这与观察到的配额快速耗尽相符。

其他促成因素包括后台Claude Code会话消耗了大量共享配额（占重置后配额的78%），自动压缩功能通过发送大量上下文创建了昂贵的令牌峰值，以及1M上下文窗口每次API调用都会放大令牌消耗。

用户建议了改进措施，例如明确 `cache_read` 的计费方式，基于*有效*令牌的速率限制，空闲会话检测，以及更好地实时显示配额。Claude Code团队承认，1M令牌上下文窗口成本高昂，尤其是在一个小时不活动后出现提示缓存未命中时，并正在调查默认使用400k上下文窗口，同时实施用户体验改进以引导用户。

---

## 7. 法国政府弃用Windows改用Linux，称美国技术存在战略风险

**原文标题**: France's government is ditching Windows for Linux, says US tech a strategic risk

**原文链接**: [https://www.xda-developers.com/frances-government-ditching-windows-for-linux/](https://www.xda-developers.com/frances-government-ditching-windows-for-linux/)

法国政府正着手放弃来自欧盟以外的专有技术，特别是Windows系统，转而采用Linux等开源解决方案。这一由法国数字部际总局 (DINUM) 宣布的战略转变，旨在增强法国的数字主权，并减少对“欧盟以外”——特别是美国——技术的依赖。

政府认为当前的依赖是一种战略风险，因为它对这些外国解决方案的规则、定价、演进和安全风险缺乏控制。公共行动和账目部长戴维·阿米尔强调，需要“摆脱束缚”，并“重新掌控我们的数字命运”。

所有部委目前都受命绘制其对欧盟以外来源的依赖，并制定一份在秋季前完成的退出计划，尽管具体推出日期尚未确定。虽然主要目标是开源，但如果严格偏好欧盟内部解决方案，也可选用源自欧盟的选项，如openSUSE和LibreOffice。此举凸显了全球范围内为增强控制和安全性而转向开源的日益增长的趋势。

---

## 8. Exploiting the most prominent AI agent benchmarks

**原文标题**: Exploiting the most prominent AI agent benchmarks

**原文链接**: [https://rdi.berkeley.edu/blog/trustworthy-benchmarks-cont/](https://rdi.berkeley.edu/blog/trustworthy-benchmarks-cont/)

A UC Berkeley research team (Hao Wang et al., April 2026) has revealed that eight prominent AI agent benchmarks, including SWE-bench, WebArena, and OSWorld, are fundamentally exploitable. Their automated scanning agent achieved near-perfect scores on all audited benchmarks without solving a single task or employing any AI reasoning, solely by exploiting flaws in how scores are computed.

Exploits included manipulating test infrastructure (e.g., `conftest.py` for SWE-bench, fake `curl` for Terminal-Bench), reading gold answers directly from task configs via `file://` URLs (WebArena), and abusing flawed validation logic (FieldWorkArena). The authors assert this isn't theoretical, citing real-world instances where models have already gamed benchmarks by copying answers or manipulating evaluation environments.

They identify recurring vulnerabilities: lack of isolation between agent and evaluator, answers shipped with tests, `eval()` on untrusted input, prompt injection in LLM judges, weak string matching, and flawed evaluation logic. This systemic problem means benchmarks often measure lookup speed or exploitation skill, not true AI capability, necessitating a fundamental redesign of evaluation methodologies for trustworthiness and robustness.

---

## 9. Chimpanzees in Uganda locked in eight-year 'civil war', say researchers

**原文标题**: Chimpanzees in Uganda locked in eight-year 'civil war', say researchers

**原文链接**: [https://www.bbc.com/news/articles/cr71lkzv49po](https://www.bbc.com/news/articles/cr71lkzv49po)

生成摘要时出错

---

## 10. South Korea introduces universal basic mobile data access

**原文标题**: South Korea introduces universal basic mobile data access

**原文链接**: [https://www.theregister.com/2026/04/10/south_korea_data_access_universal/](https://www.theregister.com/2026/04/10/south_korea_data_access_universal/)

生成摘要时出错

---

## 11. Anthropic downgraded cache TTL on March 6th

**原文标题**: Anthropic downgraded cache TTL on March 6th

**原文链接**: [https://github.com/anthropics/claude-code/issues/46829](https://github.com/anthropics/claude-code/issues/46829)

生成摘要时出错

---

## 12. Sam Altman's response to Molotov cocktail incident

**原文标题**: Sam Altman's response to Molotov cocktail incident

**原文链接**: [https://blog.samaltman.com/2279512](https://blog.samaltman.com/2279512)

生成摘要时出错

---

## 13. Seven countries now generate 100% of their electricity from renewable energy

**原文标题**: Seven countries now generate 100% of their electricity from renewable energy

**原文链接**: [https://www.the-independent.com/tech/renewable-energy-solar-nepal-bhutan-iceland-b2533699.html](https://www.the-independent.com/tech/renewable-energy-solar-nepal-bhutan-iceland-b2533699.html)

生成摘要时出错

---

## 14. Apple update looks like Czech mate for locked-out iPhone user

**原文标题**: Apple update looks like Czech mate for locked-out iPhone user

**原文链接**: [https://www.theregister.com/2026/04/12/ios_passcode_bug/](https://www.theregister.com/2026/04/12/ios_passcode_bug/)

生成摘要时出错

---

## 15. AI Will Be Met with Violence, and Nothing Good Will Come of It

**原文标题**: AI Will Be Met with Violence, and Nothing Good Will Come of It

**原文链接**: [https://www.thealgorithmicbridge.com/p/ai-will-be-met-with-violence-and](https://www.thealgorithmicbridge.com/p/ai-will-be-met-with-violence-and)

生成摘要时出错

---

## 16. Bring Back Idiomatic Design

**原文标题**: Bring Back Idiomatic Design

**原文链接**: [https://essays.johnloeber.com/p/4-bring-back-idiomatic-design](https://essays.johnloeber.com/p/4-bring-back-idiomatic-design)

生成摘要时出错

---

## 17. Cirrus Labs to join OpenAI

**原文标题**: Cirrus Labs to join OpenAI

**原文链接**: [https://cirruslabs.org/](https://cirruslabs.org/)

生成摘要时出错

---

## 18. The future of everything is lies, I guess – Part 5: Annoyances

**原文标题**: The future of everything is lies, I guess – Part 5: Annoyances

**原文链接**: [https://aphyr.com/posts/415-the-future-of-everything-is-lies-i-guess-annoyances](https://aphyr.com/posts/415-the-future-of-everything-is-lies-i-guess-annoyances)

生成摘要时出错

---

## 19. Advanced Mac Substitute is an API-level reimplementation of 1980s-era Mac OS

**原文标题**: Advanced Mac Substitute is an API-level reimplementation of 1980s-era Mac OS

**原文链接**: [https://www.v68k.org/advanced-mac-substitute/](https://www.v68k.org/advanced-mac-substitute/)

生成摘要时出错

---

## 20. DOJ wants to scrap Watergate-era rule that makes presidential records public

**原文标题**: DOJ wants to scrap Watergate-era rule that makes presidential records public

**原文链接**: [https://theintercept.com/2026/04/09/trump-documents-library-presidential-records-act/](https://theintercept.com/2026/04/09/trump-documents-library-presidential-records-act/)

生成摘要时出错

---

## 21. 447 TB/cm² at zero retention energy – atomic-scale memory on fluorographane

**原文标题**: 447 TB/cm² at zero retention energy – atomic-scale memory on fluorographane

**原文链接**: [https://zenodo.org/records/19513269](https://zenodo.org/records/19513269)

生成摘要时出错

---

## 22. 20 years on AWS and never not my job

**原文标题**: 20 years on AWS and never not my job

**原文链接**: [https://www.daemonology.net/blog/2026-04-11-20-years-on-AWS-and-never-not-my-job.html](https://www.daemonology.net/blog/2026-04-11-20-years-on-AWS-and-never-not-my-job.html)

生成摘要时出错

---

## 23. Molotov cocktail is hurled at home of Sam Altman

**原文标题**: Molotov cocktail is hurled at home of Sam Altman

**原文链接**: [https://www.nytimes.com/2026/04/10/us/open-ai-sam-altman-molotov-cocktail.html](https://www.nytimes.com/2026/04/10/us/open-ai-sam-altman-molotov-cocktail.html)

生成摘要时出错

---

## 24. Bitcoin miners are losing on every coin produced as difficulty drops

**原文标题**: Bitcoin miners are losing on every coin produced as difficulty drops

**原文链接**: [https://www.coindesk.com/markets/2026/03/22/bitcoin-miners-are-losing-usd19-000-on-every-btc-produced-as-difficulty-drops-7-8](https://www.coindesk.com/markets/2026/03/22/bitcoin-miners-are-losing-usd19-000-on-every-btc-produced-as-difficulty-drops-7-8)

生成摘要时出错

---

## 25. Dark Castle

**原文标题**: Dark Castle

**原文链接**: [https://darkcastle.co.uk/](https://darkcastle.co.uk/)

生成摘要时出错

---

## 26. Apple Silicon and Virtual Machines: Beating the 2 VM Limit (2023)

**原文标题**: Apple Silicon and Virtual Machines: Beating the 2 VM Limit (2023)

**原文链接**: [https://khronokernel.com/macos/2023/08/08/AS-VM.html](https://khronokernel.com/macos/2023/08/08/AS-VM.html)

生成摘要时出错

---

## 27. Nowhere is safe

**原文标题**: Nowhere is safe

**原文链接**: [https://steveblank.com/2026/04/09/nowhere-is-safe/](https://steveblank.com/2026/04/09/nowhere-is-safe/)

生成摘要时出错

---

## 28. US appeals court declares 158-year-old home distilling ban unconstitutional

**原文标题**: US appeals court declares 158-year-old home distilling ban unconstitutional

**原文链接**: [https://www.theguardian.com/law/2026/apr/11/appeals-court-ruling-home-distilling-ban-unconstitutional](https://www.theguardian.com/law/2026/apr/11/appeals-court-ruling-home-distilling-ban-unconstitutional)

生成摘要时出错

---

## 29. The End of Eleventy

**原文标题**: The End of Eleventy

**原文链接**: [https://brennan.day/the-end-of-eleventy/](https://brennan.day/the-end-of-eleventy/)

生成摘要时出错

---

## 30. The disturbing white paper Red Hat is trying to erase from the internet

**原文标题**: The disturbing white paper Red Hat is trying to erase from the internet

**原文链接**: [https://www.osnews.com/story/144776/the-disturbing-white-paper-red-hat-is-trying-to-erase-from-the-internet/](https://www.osnews.com/story/144776/the-disturbing-white-paper-red-hat-is-trying-to-erase-from-the-internet/)

生成摘要时出错

---

## 31. We have a 99% email reputation. Gmail disagrees

**原文标题**: We have a 99% email reputation. Gmail disagrees

**原文链接**: [https://blogfontawesome.wpcomstaging.com/we-have-a-99-email-reputation-gmail-disagrees/](https://blogfontawesome.wpcomstaging.com/we-have-a-99-email-reputation-gmail-disagrees/)

生成摘要时出错

---

## 32. Polymarket gamblers betting millions on war

**原文标题**: Polymarket gamblers betting millions on war

**原文链接**: [https://www.theguardian.com/business/2026/apr/11/polymarket-gamblers-betting-iran-war-ukraine-news-truth](https://www.theguardian.com/business/2026/apr/11/polymarket-gamblers-betting-iran-war-ukraine-news-truth)

生成摘要时出错

---

## 33. Phyphox – Physical Experiments Using a Smartphone

**原文标题**: Phyphox – Physical Experiments Using a Smartphone

**原文链接**: [https://phyphox.org/](https://phyphox.org/)

生成摘要时出错

---

## 34. Productive Procrastination

**原文标题**: Productive Procrastination

**原文链接**: [https://www.maxvanijsselmuiden.nl/blog/productive-procrastination/](https://www.maxvanijsselmuiden.nl/blog/productive-procrastination/)

生成摘要时出错

---

## 35. Building a SaaS in 2026 Using Only EU Infrastructure

**原文标题**: Building a SaaS in 2026 Using Only EU Infrastructure

**原文链接**: [https://eualternative.eu/guides/building-saas-eu-stack/](https://eualternative.eu/guides/building-saas-eu-stack/)

生成摘要时出错

---

## 36. Israel Destroys Villages in Lebanon

**原文标题**: Israel Destroys Villages in Lebanon

**原文链接**: [https://www.theguardian.com/world/2026/apr/12/how-israeli-offensive-destroyed-entire-villages-in-lebanon](https://www.theguardian.com/world/2026/apr/12/how-israeli-offensive-destroyed-entire-villages-in-lebanon)

生成摘要时出错

---

## 37. JVM Options Explorer

**原文标题**: JVM Options Explorer

**原文链接**: [https://chriswhocodes.com/vm-options-explorer.html](https://chriswhocodes.com/vm-options-explorer.html)

生成摘要时出错

---

## 38. The Problem That Built an Industry

**原文标题**: The Problem That Built an Industry

**原文链接**: [https://ajitem.com/blog/iron-core-part-1-the-problem-that-built-an-industry/](https://ajitem.com/blog/iron-core-part-1-the-problem-that-built-an-industry/)

生成摘要时出错

---

## 39. Internet outage in Iran reaches 1,008 hours

**原文标题**: Internet outage in Iran reaches 1,008 hours

**原文链接**: [https://mastodon.social/@netblocks/116384935123261912](https://mastodon.social/@netblocks/116384935123261912)

生成摘要时出错

---

## 40. Show HN: boringBar – a taskbar-style dock replacement for macOS

**原文标题**: Show HN: boringBar – a taskbar-style dock replacement for macOS

**原文链接**: [https://boringbar.app/](https://boringbar.app/)

生成摘要时出错

---

## 41. Apple has removed most of the towns and villages in Lebanon from Apple maps

**原文标题**: Apple has removed most of the towns and villages in Lebanon from Apple maps

**原文链接**: [https://maps.apple.com/frame?center=33.723388%2C35.614698&span=1.983925%2C4.004193](https://maps.apple.com/frame?center=33.723388%2C35.614698&span=1.983925%2C4.004193)

生成摘要时出错

---

## 42. How to build a `Git diff` driver

**原文标题**: How to build a `Git diff` driver

**原文链接**: [https://www.jvt.me/posts/2026/04/11/how-git-diff-driver/](https://www.jvt.me/posts/2026/04/11/how-git-diff-driver/)

生成摘要时出错

---

## 43. Show HN: Oberon System 3 runs natively on Raspberry Pi 3 (with ready SD card)

**原文标题**: Show HN: Oberon System 3 runs natively on Raspberry Pi 3 (with ready SD card)

**原文链接**: [https://github.com/rochus-keller/OberonSystem3Native/releases](https://github.com/rochus-keller/OberonSystem3Native/releases)

生成摘要时出错

---

## 44. Italo Calvino: A traveller in a world of uncertainty

**原文标题**: Italo Calvino: A traveller in a world of uncertainty

**原文链接**: [https://www.historytoday.com/archive/portrait-author-historian/italo-calvino-traveller-world-uncertainty](https://www.historytoday.com/archive/portrait-author-historian/italo-calvino-traveller-world-uncertainty)

生成摘要时出错

---

## 45. Watgo – A WebAssembly Toolkit for Go

**原文标题**: Watgo – A WebAssembly Toolkit for Go

**原文链接**: [https://eli.thegreenplace.net/2026/watgo-a-webassembly-toolkit-for-go/](https://eli.thegreenplace.net/2026/watgo-a-webassembly-toolkit-for-go/)

生成摘要时出错

---

## 46. DOJ Top Antitrust Litigators Exit After Ticketmaster Accord

**原文标题**: DOJ Top Antitrust Litigators Exit After Ticketmaster Accord

**原文链接**: [https://www.bloomberg.com/news/articles/2026-04-08/doj-top-antitrust-litigators-exit-after-ticketmaster-settlement](https://www.bloomberg.com/news/articles/2026-04-08/doj-top-antitrust-litigators-exit-after-ticketmaster-settlement)

生成摘要时出错

---

## 47. Rockstar Games Hacked, Hackers Threaten a Massive Data Leak If Not Paid Ransom

**原文标题**: Rockstar Games Hacked, Hackers Threaten a Massive Data Leak If Not Paid Ransom

**原文链接**: [https://kotaku.com/rockstar-games-reportedly-hacked-massive-data-leak-ransom-gta-6-shinyhunters-2000686858](https://kotaku.com/rockstar-games-reportedly-hacked-massive-data-leak-ransom-gta-6-shinyhunters-2000686858)

生成摘要时出错

---

## 48. Keeping a Postgres Queue Healthy

**原文标题**: Keeping a Postgres Queue Healthy

**原文链接**: [https://planetscale.com/blog/keeping-a-postgres-queue-healthy](https://planetscale.com/blog/keeping-a-postgres-queue-healthy)

生成摘要时出错

---

## 49. Now is the best time to write code by hand

**原文标题**: Now is the best time to write code by hand

**原文链接**: [https://sitebloom.ch/writing/now-is-the-best-time-to-write-code-by-hand/](https://sitebloom.ch/writing/now-is-the-best-time-to-write-code-by-hand/)

生成摘要时出错

---

## 50. Quien – A better WHOIS lookup tool

**原文标题**: Quien – A better WHOIS lookup tool

**原文链接**: [https://github.com/retlehs/quien/](https://github.com/retlehs/quien/)

生成摘要时出错

---

## 51. We spoke to the man making viral Lego-style AI videos for Iran

**原文标题**: We spoke to the man making viral Lego-style AI videos for Iran

**原文链接**: [https://www.bbc.com/news/articles/cjd8jrd1vnyo](https://www.bbc.com/news/articles/cjd8jrd1vnyo)

生成摘要时出错

---

## 52. Combining spicy foods with mint boosts anti-inflammatory effects 100x or more

**原文标题**: Combining spicy foods with mint boosts anti-inflammatory effects 100x or more

**原文链接**: [https://scitechdaily.com/this-spice-combo-could-slash-inflammation-hundreds-of-times-more-effectively/](https://scitechdaily.com/this-spice-combo-could-slash-inflammation-hundreds-of-times-more-effectively/)

生成摘要时出错

---

## 53. The Physics of GPS

**原文标题**: The Physics of GPS

**原文链接**: [https://perthirtysix.com/how-does-gps-work](https://perthirtysix.com/how-does-gps-work)

生成摘要时出错

---

## 54. MiniMax M2.7 Is Now Open Source

**原文标题**: MiniMax M2.7 Is Now Open Source

**原文链接**: [https://firethering.com/minimax-m2-7-agentic-model/](https://firethering.com/minimax-m2-7-agentic-model/)

生成摘要时出错

---

## 55. Pope Leo XIV denounces the 'delusion of omnipotence' he says fuels the Iran war

**原文标题**: Pope Leo XIV denounces the 'delusion of omnipotence' he says fuels the Iran war

**原文链接**: [https://www.politico.com/news/2026/04/11/pope-leo-xiv-denounces-the-delusion-of-omnipotence-he-says-fuels-the-us-israeli-war-in-iran-00868142](https://www.politico.com/news/2026/04/11/pope-leo-xiv-denounces-the-delusion-of-omnipotence-he-says-fuels-the-us-israeli-war-in-iran-00868142)

生成摘要时出错

---

## 56. The Closing of the Frontier

**原文标题**: The Closing of the Frontier

**原文链接**: [https://tanyaverma.sh/2026/04/10/closing-of-the-frontier.html](https://tanyaverma.sh/2026/04/10/closing-of-the-frontier.html)

生成摘要时出错

---

## 57. The APL programming language source code (2012)

**原文标题**: The APL programming language source code (2012)

**原文链接**: [https://computerhistory.org/blog/the-apl-programming-language-source-code/](https://computerhistory.org/blog/the-apl-programming-language-source-code/)

生成摘要时出错

---

## 58. How to breathe in fewer microplastics in your home

**原文标题**: How to breathe in fewer microplastics in your home

**原文链接**: [https://www.bbc.com/future/article/20260410-how-to-breathe-in-fewer-microplastics-in-your-home](https://www.bbc.com/future/article/20260410-how-to-breathe-in-fewer-microplastics-in-your-home)

生成摘要时出错

---

## 59. Doom, Played over Curl

**原文标题**: Doom, Played over Curl

**原文链接**: [https://github.com/xsawyerx/curl-doom](https://github.com/xsawyerx/curl-doom)

生成摘要时出错

---

## 60. US – Iran negotiations end with no deal reached

**原文标题**: US – Iran negotiations end with no deal reached

**原文链接**: [https://www.nytimes.com/live/2026/04/11/world/iran-war-trump-talks-pakistan](https://www.nytimes.com/live/2026/04/11/world/iran-war-trump-talks-pakistan)

生成摘要时出错

---

## 61. Phone Trips

**原文标题**: Phone Trips

**原文链接**: [http://www.wideweb.com/phonetrips/](http://www.wideweb.com/phonetrips/)

生成摘要时出错

---

## 62. New synthesis of astronomical measurements shows Hubble tension is real

**原文标题**: New synthesis of astronomical measurements shows Hubble tension is real

**原文链接**: [https://noirlab.edu/public/news/noirlab2611/?nocache=true&lang=en](https://noirlab.edu/public/news/noirlab2611/?nocache=true&lang=en)

生成摘要时出错

---

## 63. Americans still opt for print books over digital or audio versions

**原文标题**: Americans still opt for print books over digital or audio versions

**原文链接**: [https://www.pewresearch.org/short-reads/2026/04/09/americans-still-opt-for-print-books-over-digital-or-audio-versions-few-are-in-book-clubs/](https://www.pewresearch.org/short-reads/2026/04/09/americans-still-opt-for-print-books-over-digital-or-audio-versions-few-are-in-book-clubs/)

生成摘要时出错

---

## 64. Apple removes Lebanese village names from Apple Maps as Israel attacks

**原文标题**: Apple removes Lebanese village names from Apple Maps as Israel attacks

**原文链接**: [https://twitter.com/EthanLevins2/status/2043366941922926940](https://twitter.com/EthanLevins2/status/2043366941922926940)

生成摘要时出错

---

## 65. No one owes you supply-chain security

**原文标题**: No one owes you supply-chain security

**原文链接**: [https://purplesyringa.moe/blog/no-one-owes-you-supply-chain-security/](https://purplesyringa.moe/blog/no-one-owes-you-supply-chain-security/)

生成摘要时出错

---

## 66. One neat trick to end extreme poverty

**原文标题**: One neat trick to end extreme poverty

**原文链接**: [https://www.economist.com/finance-and-economics/2026/04/09/one-neat-trick-to-end-extreme-poverty](https://www.economist.com/finance-and-economics/2026/04/09/one-neat-trick-to-end-extreme-poverty)

生成摘要时出错

---

## 67. Why AI Sucks at Front End

**原文标题**: Why AI Sucks at Front End

**原文链接**: [https://nerdy.dev/why-ai-sucks-at-front-end](https://nerdy.dev/why-ai-sucks-at-front-end)

生成摘要时出错

---

## 68. Killing of Hind Rajab (2024)

**原文标题**: Killing of Hind Rajab (2024)

**原文链接**: [https://en.wikipedia.org/wiki/Killing_of_Hind_Rajab](https://en.wikipedia.org/wiki/Killing_of_Hind_Rajab)

生成摘要时出错

---

## 69. Viktor Orbán concedes defeat after 'painful' election result

**原文标题**: Viktor Orbán concedes defeat after 'painful' election result

**原文链接**: [https://apnews.com/article/hungary-election-orban-magyar-trump-1a4eb0ba6b94e0c80c3cd18bd36254ab](https://apnews.com/article/hungary-election-orban-magyar-trump-1a4eb0ba6b94e0c80c3cd18bd36254ab)

生成摘要时出错

---

## 70. High-Level Rust: Getting 80% of the Benefits with 20% of the Pain

**原文标题**: High-Level Rust: Getting 80% of the Benefits with 20% of the Pain

**原文链接**: [https://hamy.xyz/blog/2026-01_high-level-rust](https://hamy.xyz/blog/2026-01_high-level-rust)

生成摘要时出错

---

## 71. How a dancer with ALS used brainwaves to perform live

**原文标题**: How a dancer with ALS used brainwaves to perform live

**原文链接**: [https://www.electronicspecifier.com/products/sensors/how-a-dancer-with-als-used-brainwaves-to-perform-live/](https://www.electronicspecifier.com/products/sensors/how-a-dancer-with-als-used-brainwaves-to-perform-live/)

生成摘要时出错

---

## 72. The Grand Line

**原文标题**: The Grand Line

**原文链接**: [https://pilgrima.ge/p/the-grand-line](https://pilgrima.ge/p/the-grand-line)

生成摘要时出错

---

## 73. Show HN: Hormuz Havoc, a satirical game that got overrun by AI bots in 24 hours

**原文标题**: Show HN: Hormuz Havoc, a satirical game that got overrun by AI bots in 24 hours

**原文链接**: [https://www.hormuz-havoc.com/](https://www.hormuz-havoc.com/)

生成摘要时出错

---

## 74. Artemis II is competency porn

**原文标题**: Artemis II is competency porn

**原文链接**: [https://lizplank.substack.com/p/artemis-ii-is-competency-porn-and](https://lizplank.substack.com/p/artemis-ii-is-competency-porn-and)

生成摘要时出错

---

## 75. Meta is set to pay its top AI executives almost a billion each in bonuses

**原文标题**: Meta is set to pay its top AI executives almost a billion each in bonuses

**原文链接**: [https://www.msn.com/en-my/news/other/meta-is-set-to-pay-its-top-ai-executives-almost-a-billion-each-in-bonuses-if-they-hit-their-targets/ar-AA1ZszqA](https://www.msn.com/en-my/news/other/meta-is-set-to-pay-its-top-ai-executives-almost-a-billion-each-in-bonuses-if-they-hit-their-targets/ar-AA1ZszqA)

生成摘要时出错

---

## 76. Hungary Is a Laboratory for Illiberal Nationalism. The Results Are In

**原文标题**: Hungary Is a Laboratory for Illiberal Nationalism. The Results Are In

**原文链接**: [https://www.cato.org/commentary/hungary-laboratory-illiberal-nationalism-results-are](https://www.cato.org/commentary/hungary-laboratory-illiberal-nationalism-results-are)

生成摘要时出错

---

## 77. Has Mythos just broken the deal that kept the internet safe?

**原文标题**: Has Mythos just broken the deal that kept the internet safe?

**原文链接**: [https://martinalderson.com/posts/has-mythos-just-broken-the-deal-that-kept-the-internet-safe/](https://martinalderson.com/posts/has-mythos-just-broken-the-deal-that-kept-the-internet-safe/)

生成摘要时出错

---

## 78. US Government trying to unmask ICE critical redditor

**原文标题**: US Government trying to unmask ICE critical redditor

**原文链接**: [https://arstechnica.com/tech-policy/2026/04/trump-admin-hounds-reddit-to-reveal-identity-of-user-who-criticized-ice/](https://arstechnica.com/tech-policy/2026/04/trump-admin-hounds-reddit-to-reveal-identity-of-user-who-criticized-ice/)

生成摘要时出错

---

## 79. The Seasons Are Wrong

**原文标题**: The Seasons Are Wrong

**原文链接**: [https://kentwalters.com/posts/seasons/](https://kentwalters.com/posts/seasons/)

生成摘要时出错

---

## 80. Eternity in six hours: Intergalactic spreading of intelligent life (2013)

**原文标题**: Eternity in six hours: Intergalactic spreading of intelligent life (2013)

**原文链接**: [https://www.researchgate.net/publication/256935390_Eternity_in_six_hours_Intergalactic_spreading_of_intelligent_life_and_sharpening_the_Fermi_paradox](https://www.researchgate.net/publication/256935390_Eternity_in_six_hours_Intergalactic_spreading_of_intelligent_life_and_sharpening_the_Fermi_paradox)

生成摘要时出错

---

## 81. Great at gaming? US air traffic control wants you to apply

**原文标题**: Great at gaming? US air traffic control wants you to apply

**原文链接**: [https://www.bbc.com/news/articles/ce84rvx0e6do](https://www.bbc.com/news/articles/ce84rvx0e6do)

生成摘要时出错

---

## 82. Microsoft starts removing Copilot buttons from Windows 11 apps

**原文标题**: Microsoft starts removing Copilot buttons from Windows 11 apps

**原文链接**: [https://www.theverge.com/news/909640/microsoft-removing-copilot-windows-11-buttons](https://www.theverge.com/news/909640/microsoft-removing-copilot-windows-11-buttons)

生成摘要时出错

---

## 83. Trump says US will blockade Strait of Hormuz

**原文标题**: Trump says US will blockade Strait of Hormuz

**原文链接**: [https://www.cnn.com/2026/04/12/world/live-news/iran-us-war-talks-trump](https://www.cnn.com/2026/04/12/world/live-news/iran-us-war-talks-trump)

生成摘要时出错

---

## 84. Borges' cartographers and the tacit skill of reading LM output

**原文标题**: Borges' cartographers and the tacit skill of reading LM output

**原文链接**: [https://galsapir.github.io/sparse-thoughts/2026/04/11/map-and-territory/](https://galsapir.github.io/sparse-thoughts/2026/04/11/map-and-territory/)

生成摘要时出错

---

## 85. Software Preservation Group: C++ History Collection

**原文标题**: Software Preservation Group: C++ History Collection

**原文链接**: [https://softwarepreservation.computerhistory.org/c_plus_plus/](https://softwarepreservation.computerhistory.org/c_plus_plus/)

This "C++ History Collection," curated by Paul McJones, serves as an archive of design documents, source code, and other materials detailing the birth, development, standardization, and use of the C++ programming language.

The collection's chronology highlights key milestones, starting with "C with Classes" in 1979 and its pre-processor, Cpre. C++ was named in 1984, followed by Cfront Release E (first external) in February 1985, and Release 1.0 (first commercial) in October 1985. The ANSI C++ committee (J16) was founded in 1989, leading to the acceptance of major features like templates, exceptions, RTTI, namespaces, and the STL throughout the early 1990s. The ISO C++ standard was ratified in 1998, with work on C++0x commencing in 2003.

Dedicated sections explore "C with Classes" (Cpre) through early papers by Bjarne Stroustrup, describing its function as a pre-processor adding Simula-like classes to C. The Cfront releases section offers historical source code and documentation for the original C++ translator, including Release E (largely Stroustrup's sole work) and subsequent versions (1.0, 1.2, 2.0, 3.0).

Further resources include links to ISO/IEC C++ Standardization committee papers, GNU g++ release information, and a selection of influential papers and articles about C++, notably Bjarne Stroustrup's comprehensive "History of C++" series. The collection acknowledges numerous individuals and organizations for their contributions to preserving this historical data.

---

## 86. What have been the greatest intellectual achievements? (2017)

**原文标题**: What have been the greatest intellectual achievements? (2017)

**原文链接**: [https://www.thinkingcomplete.com/2017/09/what-have-been-greatest-intellectual.html](https://www.thinkingcomplete.com/2017/09/what-have-been-greatest-intellectual.html)

生成摘要时出错

---

## 87. Tesla's supervised self-driving software gets Dutch okay, first in Europe

**原文标题**: Tesla's supervised self-driving software gets Dutch okay, first in Europe

**原文链接**: [https://www.reuters.com/business/teslas-self-driving-software-gets-dutch-go-ahead-boost-eu-ambitions-2026-04-10/](https://www.reuters.com/business/teslas-self-driving-software-gets-dutch-go-ahead-boost-eu-ambitions-2026-04-10/)

生成摘要时出错

---

## 88. DIY Soft Drinks

**原文标题**: DIY Soft Drinks

**原文链接**: [https://blinry.org/diy-soft-drinks/](https://blinry.org/diy-soft-drinks/)

生成摘要时出错

---

## 89. Midnight Captain – A midnight commander inspired file manager

**原文标题**: Midnight Captain – A midnight commander inspired file manager

**原文链接**: [https://github.com/duguyue100/midnight-captain](https://github.com/duguyue100/midnight-captain)

生成摘要时出错

---

## 90. Show HN: Waffle – Native macOS terminal that auto-tiles sessions into a grid

**原文标题**: Show HN: Waffle – Native macOS terminal that auto-tiles sessions into a grid

**原文链接**: [https://waffle.baby](https://waffle.baby)

生成摘要时出错

---

## 91. Artemis II returns to Earth, splashdown in four hours

**原文标题**: Artemis II returns to Earth, splashdown in four hours

**原文链接**: [https://www.cbc.ca/news/science/artemisii-return-splashdown-9.7157857](https://www.cbc.ca/news/science/artemisii-return-splashdown-9.7157857)

生成摘要时出错

---

## 92. Reading Is Magic

**原文标题**: Reading Is Magic

**原文链接**: [https://samkriss.substack.com/p/reading-is-magic](https://samkriss.substack.com/p/reading-is-magic)

生成摘要时出错

---

## 93. 40x Faster Binary Search

**原文标题**: 40x Faster Binary Search

**原文链接**: [https://www.p99conf.io/session/40x-faster-binary-search/](https://www.p99conf.io/session/40x-faster-binary-search/)

生成摘要时出错

---

## 94. I Hate Tailwind and Love Bootstrap

**原文标题**: I Hate Tailwind and Love Bootstrap

**原文链接**: [https://necromant2005.github.io/dev/why-i-hate-tailwind-and-love-bootstrap/](https://necromant2005.github.io/dev/why-i-hate-tailwind-and-love-bootstrap/)

生成摘要时出错

---

## 95. Method to reverse cellular ageing is about to be tested in humans

**原文标题**: Method to reverse cellular ageing is about to be tested in humans

**原文链接**: [https://www.nature.com/articles/d41586-026-01024-7](https://www.nature.com/articles/d41586-026-01024-7)

生成摘要时出错

---

## 96. USB/IP Project: a general USB device sharing system over IP network

**原文标题**: USB/IP Project: a general USB device sharing system over IP network

**原文链接**: [https://usbip.sourceforge.net/](https://usbip.sourceforge.net/)

生成摘要时出错

---

## 97. The Brainrot Industrial Complex

**原文标题**: The Brainrot Industrial Complex

**原文链接**: [https://jshamsul.com/essays/2026-04-12-brainrot-industrial-complex](https://jshamsul.com/essays/2026-04-12-brainrot-industrial-complex)

生成摘要时出错

---

## 98. Iran Unable to Find Mines in Strait of Hormuz, U.S. Says

**原文标题**: Iran Unable to Find Mines in Strait of Hormuz, U.S. Says

**原文链接**: [https://www.nytimes.com/2026/04/10/us/politics/iran-mines-strait.html](https://www.nytimes.com/2026/04/10/us/politics/iran-mines-strait.html)

生成摘要时出错

---

## 99. A Crazy Expensive U.S. Drone Just Disappeared over Strait of Hormuz

**原文标题**: A Crazy Expensive U.S. Drone Just Disappeared over Strait of Hormuz

**原文链接**: [https://www.forbes.com/sites/davidhambling/2026/04/10/a-crazy-expensive-us-drone-just-disappeared-over-strait-of-hormuz/](https://www.forbes.com/sites/davidhambling/2026/04/10/a-crazy-expensive-us-drone-just-disappeared-over-strait-of-hormuz/)

生成摘要时出错

---

## 100. Top Performers Are Pathologically Ambitious

**原文标题**: Top Performers Are Pathologically Ambitious

**原文链接**: [https://thatvastvariety.substack.com/p/top-performers-are-pathologically](https://thatvastvariety.substack.com/p/top-performers-are-pathologically)

生成摘要时出错

---

