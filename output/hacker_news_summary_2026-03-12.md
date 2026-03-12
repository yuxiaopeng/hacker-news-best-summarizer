# Hacker News 热门文章摘要 (2026-03-12)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 请勿发布AI生成或编辑的评论。HN是为了人与人之间的交流。

**原文标题**: Don't post generated/AI-edited comments. HN is for conversation between humans

**原文链接**: [https://news.ycombinator.com/newsguidelines.html#generated](https://news.ycombinator.com/newsguidelines.html#generated)

Hacker News (HN) 指南旨在促进人与人之间求知欲强烈的对话。提交的内容应侧重于“优秀黑客”感兴趣的话题，超越典型的科技和创业新闻，并排除大多数主流政治、犯罪或名人故事，除非它们能突出独特的现象。主要的提交规则包括使用原创来源，避免煽动性标题（大写、感叹号、网站名称或无意义的数字），以及不主要将平台用于推广。

评论应友善、深思熟虑且有实质内容。用户应以好奇心参与讨论，避免冷嘲热讽，直接回应论点，而不是诉诸人身攻击或僵化的消极态度。至关重要的是，指南明确指出：“请勿发布生成式评论或经AI编辑的评论。HN是为人与人之间的对话而设。”参与者必须秉持善意，宽容地理解他人的言论，并避免引战、肤浅的驳斥或政治争论。鼓励具有启发性的建设性批评。其他指示包括使用*星号*表示强调，通过电子邮件报告滥用行为而非公开指责，标记恶劣评论，以及避免讨论投票、网站烦恼或将HN与Reddit进行比较。其首要目标是维护一个高质量、以人为本的讨论环境。

---

## 2. Temporal：修复 JavaScript 中的时间问题的九年之旅

**原文标题**: Temporal: The 9-year journey to fix time in JavaScript

**原文链接**: [https://bloomberg.github.io/js-blog/post/temporal/](https://bloomberg.github.io/js-blog/post/temporal/)

该文章详细介绍了Temporal的九年历程，Temporal是一个旨在取代问题重重的`Date`对象的新JavaScript API，该文章于2026年3月11日发布。原始的`Date`对象是1995年从Java匆忙移植过来的，由于其可变性、不一致的算术操作（例如，月份溢出）和模糊的解析，尤其是在复杂的全球应用中，给开发者带来了数十年的困扰。

这导致了Moment.js等第三方库的广泛采用，尽管它们很有用，却因捆绑了本地化和时区数据而显著增加了打包体积。认识到这个问题，Maggie Johnson-Pint于2017年提出了Temporal提案，并将其推进到JavaScript标准化委员会TC39的第一阶段。

该提案在Bloomberg（包括工程师Jason Williams、Philipp Dunkel）、Igalia（Ujjwal Sharma、Philip Chimento）、Microsoft（Maggie和Matt Johnson-Pint、Brian Terlson）和Google（Shane Carr）等公司以及受邀专家Justin Grant的支持下获得了发展势头。他们经历了TC39的各个阶段，解决了可配置的时区和更高的精度等现实世界的需求。

Temporal引入了一个顶层命名空间，包含不可变的日期/时间类型：
*   **`Temporal.ZonedDateTime`**：`Date`最接近的替代品，代表一个具有明确时区和日历的精确时刻，正确处理夏令时（DST）。
*   **`Temporal.Instant`**：一个精确的时间点，不带有时区或日历信息，以Unix纪元以来的纳秒数衡量，是理想的存储方式。
*   **`Temporal.PlainDate`、`PlainTime`、`PlainDateTime`等**：这些“墙上时间”（wall time）类型缺乏时区或夏令时意识，使它们适用于显示或不跨越这些边界的算术运算，防止意外错误。

Temporal旨在标准化强大的日期和时间处理，消除常见陷阱，并减少对大型外部库的依赖。

---

## 3. Malus – 洁净室即服务

**原文标题**: Malus – Clean Room as a Service

**原文链接**: [https://malus.sh](https://malus.sh)

MALUS提供“净室即服务”，旨在将公司从开源归属和许可义务中“解放”出来。它旨在解决企业普遍面临的痛点，包括Apache归属条款、AGPL污染风险、许可合规成本，以及向社区贡献改进的要求。

该解决方案涉及“机器人驱动的净室重建”。专有AI系统独立分析公共文档、API规范和接口（绝不触及原始源代码），从头开始重新创建功能等效的软件。此过程旨在生成合法独立的代码，该代码完全归客户所有，免受衍生作品主张、许可继承或任何义务的影响。

该服务保证100%由机器人编写代码，零原始代码接触，功能等效，并以企业友好的“MalusCorp-0许可”交付，无任何归属或反版权要求。它还提供全面的法律赔偿，尽管是通过位于不承认软件版权的司法管辖区的离岸子公司提供。

该过程包括上传依赖清单，随后由受过法律训练的机器人对文档进行隔离分析，由独立的机器人团队进行重新创建，最后实现许可解放。定价透明，按解放包的解压大小，以KB为单位计费。MalusCorp坚称其流程合法，基于既定的净室先例，并自信地驳斥了原始开发者的担忧。

---

## 4. 为他人创造价值，不计较回报。

**原文标题**: Create value for others and don’t worry about the returns

**原文链接**: [https://geohot.github.io//blog/jekyll/update/2026/03/11/running-69-agents.html](https://geohot.github.io//blog/jekyll/update/2026/03/11/running-69-agents.html)

文章驳斥了社交媒体上围绕人工智能制造恐惧和焦虑的普遍论调，将其斥为“一派胡言”。作者认为，人工智能并非是魔术般的颠覆者，而是技术进步的自然延续，主要用于增强搜索和优化。尽管人工智能是一个有用的工具，但它有其固有的局限性，并非许多人所认为的科幻现象。

作者指出，真正的变革针对的是“寻租者”——那些为他人制造不必要复杂性的人。这些角色是零和博弈，大型参与者正在巩固自身权力，以人工智能效率为幌子推动裁员。处于此类职位的人被建议尽早辞职。

核心信息是，与其参与零和竞争，不如为他人创造价值，消耗少于产出。这种做法能够确保在有效运转的社区中获得接纳，并有助于避免有害的比较陷阱，提供了一条真正的前进道路，尽管与那些充满末日论调的叙事相比，它可能不太能吸引注意力。

---

## 5. 使 WebAssembly 成为 Web 上的一等语言

**原文标题**: Making WebAssembly a first-class language on the Web

**原文链接**: [https://hacks.mozilla.org/2026/02/making-webassembly-a-first-class-language-on-the-web/](https://hacks.mozilla.org/2026/02/making-webassembly-a-first-class-language-on-the-web/)

WebAssembly自2017年以来已显著成熟，扩展了其能力以支持更多语言，并缩小了与原生性能的差距。然而，与JavaScript相比，它“二等公民”的地位阻碍了其在网络上的采用。

核心问题在于WebAssembly无法直接与网络平台交互；它必须通过JavaScript。这主要体现在两个方面：
1.  **代码加载：** 尽管ESM集成正在改进，但WebAssembly模块通常仍需要特定的JavaScript API进行加载和实例化，这与JavaScript简单的`<script>`标签不同。
2.  **使用Web API：** 从WebAssembly访问Web API（例如`console.log`）需要大量的JavaScript“胶水代码”。这些胶水代码处理Wasm和JS之间的数据重编码，增加了复杂性、运行时开销（一项DOM基准测试显示了45%的性能损失），以及特定语言的构建步骤。

这些限制导致糟糕的开发者体验：编译器难以提供一流的Web支持，标准工具链无法生成适用于Web的Wasm，Web文档以JavaScript为中心，开发者需要不断理解JavaScript抽象层。这使得WebAssembly成为一项“高级用户”功能，阻碍了其更广泛的采用。

拟议的解决方案是**WebAssembly组件模型**。这项标准轨道提案旨在创建一个标准化的、自包含的可执行构件，它可以用多种语言创建，由浏览器直接处理，并且至关重要的是，允许WebAssembly代码直接调用Web API而无需JavaScript胶水代码。这将为WebAssembly提供共享的、浏览器原生的集成，摆脱特定语言的JavaScript重新实现，并在网络上提供真正一流的体验。

---

## 6. 麦克本 尼奥

**原文标题**: The MacBook Neo

**原文链接**: [https://daringfireball.net/2026/03/the_macbook_neo](https://daringfireball.net/2026/03/the_macbook_neo)

2026年3月发布的MacBook Neo是一款售价600美元的笔记本电脑，搭载与iPhone 16 Pro SoC相同的A18 Pro芯片。这表明苹果的A系列芯片足以胜任出色的消费级MacBook，实现了Mac从x86转向ARM长达十年的预测。

Neo提供了压倒性的价值，在其600-700美元的价格区间内，性能、显示屏、音频以及构建/软件质量都超越了x86 PC。尽管只有8GB RAM，但日常使用依然流畅。它配备了亮度达500尼特的显示屏、令人印象深刻的侧向扬声器和持久的电池续航。机械式触控板作为一项成本节约措施，尽管缺乏Force Touch功能，但其质量和正常手感仍备受赞誉。

作者唯一重要的抱怨是缺少环境光传感器，需要手动调节亮度。其他遗漏，如没有硬件摄像头指示灯、缺少人物居中功能、第二个USB-C端口速度较慢以及20W充电器，考虑到其价格，都被认为是次要的。

Neo重2.7磅，虽然算不上超轻，但与M5 MacBook Air相当。它被视为iPad Pro或iPad Air搭配妙控键盘的更出色、更高效、显著更便宜的替代品，特别是作为一台用于“居家”的备用电脑，以令人难以置信的价格提供了卓越的macOS体验。

---

## 7. 举报人声称，一名前DOGE成员表示他将社保数据带到了新工作。

**原文标题**: Whistleblower claims ex-DOGE member says he took Social Security data to new job

**原文链接**: [https://www.washingtonpost.com/politics/2026/03/10/social-security-data-breach-doge-2/](https://www.washingtonpost.com/politics/2026/03/10/social-security-data-breach-doge-2/)

无法访问文章链接。

---

## 8. Cloudflare 爬取端点

**原文标题**: Cloudflare crawl endpoint

**原文链接**: [https://developers.cloudflare.com/changelog/post/2026-03-10-br-crawl-endpoint/](https://developers.cloudflare.com/changelog/post/2026-03-10-br-crawl-endpoint/)

Cloudflare has introduced a new `/crawl` endpoint for its Browser Rendering service, now in open beta, allowing users to crawl entire websites with a single API call. This asynchronous service takes a starting URL, automatically discovers pages through sitemaps or links, and renders them in a headless browser. Crawled content is returned in multiple formats, including HTML, Markdown, and structured JSON (powered by Workers AI).

Key features include controls for crawl depth, page limits, URL path patterns, and incremental crawling using `modifiedSince` and `maxAge` to optimize repeated fetches. A static mode (`render: false`) is available for faster crawling of static sites without browser rendering. The endpoint functions as a "well-behaved bot," respecting `robots.txt` directives and AI Crawl Control by default, making it ideal for training AI models, building RAG pipelines, and monitoring website content responsibly.

While powerful, the `/crawl` endpoint cannot bypass Cloudflare bot detection or captchas and explicitly identifies itself as a bot. It's available on both Workers Free and Paid plans. Users initiate a crawl via a POST request, receiving a job ID to check results with a GET request.

---

## 9. How we hacked McKinsey's AI platform

**原文标题**: How we hacked McKinsey's AI platform

**原文链接**: [https://codewall.ai/blog/how-we-hacked-mckinseys-ai-platform](https://codewall.ai/blog/how-we-hacked-mckinseys-ai-platform)

生成摘要时出错

---

## 10. Agents that run while I sleep

**原文标题**: Agents that run while I sleep

**原文链接**: [https://www.claudecodecamp.com/p/i-m-building-agents-that-run-while-i-sleep](https://www.claudecodecamp.com/p/i-m-building-agents-that-run-while-i-sleep)

生成摘要时出错

---

## 11. I was interviewed by an AI bot for a job

**原文标题**: I was interviewed by an AI bot for a job

**原文链接**: [https://www.theverge.com/featured-video/892850/i-was-interviewed-by-an-ai-bot-for-a-job](https://www.theverge.com/featured-video/892850/i-was-interviewed-by-an-ai-bot-for-a-job)

生成摘要时出错

---

## 12. The dead Internet is not a theory anymore

**原文标题**: The dead Internet is not a theory anymore

**原文链接**: [https://www.adriankrebs.ch/blog/dead-internet/](https://www.adriankrebs.ch/blog/dead-internet/)

生成摘要时出错

---

## 13. Type resolution redesign, with language changes to taste

**原文标题**: Type resolution redesign, with language changes to taste

**原文链接**: [https://ziglang.org/devlog/2026/#2026-03-10](https://ziglang.org/devlog/2026/#2026-03-10)

生成摘要时出错

---

## 14. U+237C ⍼ Is Azimuth

**原文标题**: U+237C ⍼ Is Azimuth

**原文链接**: [https://ionathan.ch/2026/02/16/angzarr.html](https://ionathan.ch/2026/02/16/angzarr.html)

生成摘要时出错

---

## 15. Show HN: s@: decentralized social networking over static sites

**原文标题**: Show HN: s@: decentralized social networking over static sites

**原文链接**: [http://satproto.org/](http://satproto.org/)

生成摘要时出错

---

## 16. Lego's 0.002mm specification and its implications for manufacturing (2025)

**原文标题**: Lego's 0.002mm specification and its implications for manufacturing (2025)

**原文链接**: [https://www.thewave.engineer/articles.html/productivity/legos-0002mm-specification-and-its-implications-for-manufacturing-r120/](https://www.thewave.engineer/articles.html/productivity/legos-0002mm-specification-and-its-implications-for-manufacturing-r120/)

生成摘要时出错

---

## 17. BitNet: Inference framework for 1-bit LLMs

**原文标题**: BitNet: Inference framework for 1-bit LLMs

**原文链接**: [https://github.com/microsoft/BitNet](https://github.com/microsoft/BitNet)

生成摘要时出错

---

## 18. Universal vaccine against respiratory infections and allergens

**原文标题**: Universal vaccine against respiratory infections and allergens

**原文链接**: [https://med.stanford.edu/news/all-news/2026/02/universal-vaccine.html](https://med.stanford.edu/news/all-news/2026/02/universal-vaccine.html)

生成摘要时出错

---

## 19. Returning to Rails in 2026

**原文标题**: Returning to Rails in 2026

**原文链接**: [https://www.markround.com/blog/2026/03/05/returning-to-rails-in-2026/](https://www.markround.com/blog/2026/03/05/returning-to-rails-in-2026/)

生成摘要时出错

---

## 20. Google closes deal to acquire Wiz

**原文标题**: Google closes deal to acquire Wiz

**原文链接**: [https://www.wiz.io/blog/google-closes-deal-to-acquire-wiz](https://www.wiz.io/blog/google-closes-deal-to-acquire-wiz)

Google has officially closed its deal to acquire Wiz, nearly a year after the initial announcement, aiming to combine Wiz’s innovation with Google’s scale to redefine cloud security, particularly for AI-driven development. Wiz's core mission remains helping organizations protect everything they build and run, now at the speed of AI.

Leading up to the acquisition, Wiz demonstrated significant achievements. Their research uncovered critical vulnerabilities such as CodeBreach (AWS), RediShell (Redis RCE), and NVIDIAScape (container escape), and addressed sophisticated supply chain attacks like Shai-Hulud and NX. Product innovations included expanding the Wiz AI Security Platform to secure AI applications, introducing Wiz Exposure Management for a proactive risk view, launching AI Security Agents for automated remediation, and creating WizOS for secure container base images.

As part of Google Cloud, Wiz will accelerate its roadmap by integrating cutting-edge AI capabilities, including Gemini. Crucially, Wiz will remain a multi-cloud platform, committed to protecting customers across AWS, Azure, GCP, and OCI. This partnership strengthens Wiz’s ability to protect customers everywhere, leveraging Google's infrastructure, Mandiant's threat intelligence, and the broader Google Unified Security Platform. The goal is to enable organizations to build boldly, securely, and with confidence in a rapidly evolving, AI-powered world.

---

## 21. RISC-V Is Sloooow

**原文标题**: RISC-V Is Sloooow

**原文链接**: [https://marcin.juszkiewicz.com.pl/2026/03/10/risc-v-is-sloooow/](https://marcin.juszkiewicz.com.pl/2026/03/10/risc-v-is-sloooow/)

生成摘要时出错

---

## 22. Asia rolls out 4-day weeks, WFH to solve fuel crisis caused by Iran war

**原文标题**: Asia rolls out 4-day weeks, WFH to solve fuel crisis caused by Iran war

**原文链接**: [https://fortune.com/2026/03/11/iran-war-fuel-crisis-asia-work-from-home-closed-schools-price-caps/](https://fortune.com/2026/03/11/iran-war-fuel-crisis-asia-work-from-home-closed-schools-price-caps/)

生成摘要时出错

---

## 23. Show HN: I built a tool that watches webpages and exposes changes as RSS

**原文标题**: Show HN: I built a tool that watches webpages and exposes changes as RSS

**原文链接**: [https://sitespy.app](https://sitespy.app)

生成摘要时出错

---

## 24. Entities enabling scientific fraud at scale (2025)

**原文标题**: Entities enabling scientific fraud at scale (2025)

**原文链接**: [https://doi.org/10.1073/pnas.2420092122](https://doi.org/10.1073/pnas.2420092122)

生成摘要时出错

---

## 25. Britain is ejecting hereditary nobles from Parliament after 700 years

**原文标题**: Britain is ejecting hereditary nobles from Parliament after 700 years

**原文链接**: [https://apnews.com/article/uk-house-of-lords-hereditary-peers-expelled-535df8781dd01e8970acda1dca99d3d4](https://apnews.com/article/uk-house-of-lords-hereditary-peers-expelled-535df8781dd01e8970acda1dca99d3d4)

生成摘要时出错

---

## 26. Many SWE-bench-Passing PRs would not be merged

**原文标题**: Many SWE-bench-Passing PRs would not be merged

**原文链接**: [https://metr.org/notes/2026-03-10-many-swe-bench-passing-prs-would-not-be-merged-into-main/](https://metr.org/notes/2026-03-10-many-swe-bench-passing-prs-would-not-be-merged-into-main/)

生成摘要时出错

---

## 27. Big Data on the Cheapest MacBook

**原文标题**: Big Data on the Cheapest MacBook

**原文链接**: [https://duckdb.org/2026/03/11/big-data-on-the-cheapest-macbook](https://duckdb.org/2026/03/11/big-data-on-the-cheapest-macbook)

生成摘要时出错

---

## 28. Dolphin Progress Release 2603

**原文标题**: Dolphin Progress Release 2603

**原文链接**: [https://dolphin-emu.org/blog/2026/03/12/dolphin-progress-report-release-2603/](https://dolphin-emu.org/blog/2026/03/12/dolphin-progress-report-release-2603/)

生成摘要时出错

---

## 29. Faster asin() was hiding in plain sight

**原文标题**: Faster asin() was hiding in plain sight

**原文链接**: [https://16bpp.net/blog/post/faster-asin-was-hiding-in-plain-sight/](https://16bpp.net/blog/post/faster-asin-was-hiding-in-plain-sight/)

生成摘要时出错

---

## 30. DHS Contracts Explorer – Hacked data from the Office of Industry Partnership

**原文标题**: DHS Contracts Explorer – Hacked data from the Office of Industry Partnership

**原文链接**: [https://micahflee.github.io/ice-contracts/](https://micahflee.github.io/ice-contracts/)

生成摘要时出错

---

## 31. Writing my own text editor, and daily-driving it

**原文标题**: Writing my own text editor, and daily-driving it

**原文链接**: [https://blog.jsbarretto.com/post/text-editor](https://blog.jsbarretto.com/post/text-editor)

生成摘要时出错

---

## 32. Kotlin creator's new language: a formal way to talk to LLMs instead of English

**原文标题**: Kotlin creator's new language: a formal way to talk to LLMs instead of English

**原文链接**: [https://codespeak.dev/](https://codespeak.dev/)

生成摘要时出错

---

## 33. Iran-backed hackers claim wiper attack on medtech firm Stryker

**原文标题**: Iran-backed hackers claim wiper attack on medtech firm Stryker

**原文链接**: [https://krebsonsecurity.com/2026/03/iran-backed-hackers-claim-wiper-attack-on-medtech-firm-stryker/](https://krebsonsecurity.com/2026/03/iran-backed-hackers-claim-wiper-attack-on-medtech-firm-stryker/)

生成摘要时出错

---

## 34. Atlassian to cut roughly 1,600 jobs in pivot to AI

**原文标题**: Atlassian to cut roughly 1,600 jobs in pivot to AI

**原文链接**: [https://www.reuters.com/technology/atlassian-lay-off-about-1600-people-pivot-ai-2026-03-11/](https://www.reuters.com/technology/atlassian-lay-off-about-1600-people-pivot-ai-2026-03-11/)

生成摘要时出错

---

## 35. Swiss e-voting pilot can't count 2,048 ballots after decryption failure

**原文标题**: Swiss e-voting pilot can't count 2,048 ballots after decryption failure

**原文链接**: [https://www.theregister.com/2026/03/11/swiss_evote_usb_snafu/](https://www.theregister.com/2026/03/11/swiss_evote_usb_snafu/)

生成摘要时出错

---

## 36. 3D-Knitting: The Ultimate Guide

**原文标题**: 3D-Knitting: The Ultimate Guide

**原文链接**: [https://www.oliver-charles.com/pages/3d-knitting](https://www.oliver-charles.com/pages/3d-knitting)

生成摘要时出错

---

## 37. Personal Computer by Perplexity

**原文标题**: Personal Computer by Perplexity

**原文链接**: [https://www.perplexity.ai/personal-computer-waitlist](https://www.perplexity.ai/personal-computer-waitlist)

生成摘要时出错

---

## 38. US banks' exposure to private credit hits $300B (2025)

**原文标题**: US banks' exposure to private credit hits $300B (2025)

**原文链接**: [https://alternativecreditinvestor.com/2025/10/22/us-banks-exposure-to-private-credit-hits-300bn/](https://alternativecreditinvestor.com/2025/10/22/us-banks-exposure-to-private-credit-hits-300bn/)

生成摘要时出错

---

## 39. 1B identity records exposed in ID verification data leak

**原文标题**: 1B identity records exposed in ID verification data leak

**原文链接**: [https://www.aol.com/articles/1-billion-identity-records-exposed-152505381.html](https://www.aol.com/articles/1-billion-identity-records-exposed-152505381.html)

生成摘要时出错

---

## 40. Avoiding Trigonometry (2013)

**原文标题**: Avoiding Trigonometry (2013)

**原文链接**: [https://iquilezles.org/articles/noacos/](https://iquilezles.org/articles/noacos/)

生成摘要时出错

---

## 41. ATMs didn't kill bank teller jobs, but the iPhone did

**原文标题**: ATMs didn't kill bank teller jobs, but the iPhone did

**原文链接**: [https://davidoks.blog/p/why-the-atm-didnt-kill-bank-teller](https://davidoks.blog/p/why-the-atm-didnt-kill-bank-teller)

生成摘要时出错

---

## 42. Suburban school district uses license plate readers to verify student residency

**原文标题**: Suburban school district uses license plate readers to verify student residency

**原文链接**: [https://www.nbcchicago.com/consumer/suburban-school-district-uses-license-plate-readers-to-verify-student-residency/3906703/](https://www.nbcchicago.com/consumer/suburban-school-district-uses-license-plate-readers-to-verify-student-residency/3906703/)

生成摘要时出错

---

## 43. I'm glad the Anthropic fight is happening now

**原文标题**: I'm glad the Anthropic fight is happening now

**原文链接**: [https://www.dwarkesh.com/p/dow-anthropic](https://www.dwarkesh.com/p/dow-anthropic)

生成摘要时出错

---

## 44. Italian prosecutors seek trial for Amazon, 4 execs in alleged $1.4B tax evasion

**原文标题**: Italian prosecutors seek trial for Amazon, 4 execs in alleged $1.4B tax evasion

**原文链接**: [https://www.reuters.com/world/italian-prosecutors-seek-trial-amazon-four-execs-over-alleged-14-bln-tax-evasion-2026-03-12/](https://www.reuters.com/world/italian-prosecutors-seek-trial-amazon-four-execs-over-alleged-14-bln-tax-evasion-2026-03-12/)

生成摘要时出错

---

## 45. Show HN: Klaus – OpenClaw on a VM, batteries included

**原文标题**: Show HN: Klaus – OpenClaw on a VM, batteries included

**原文链接**: [https://klausai.com/](https://klausai.com/)

生成摘要时出错

---

## 46. US- and Greek-owned tankers ablaze after Iran claims 'underwater drone' strike

**原文标题**: US- and Greek-owned tankers ablaze after Iran claims 'underwater drone' strike

**原文链接**: [https://www.lloydslist.com/LL1156592/US--and-Greek-owned-tankers-ablaze-after-Iran-claims-underwater-drone-strike-in-Iraqi-waters](https://www.lloydslist.com/LL1156592/US--and-Greek-owned-tankers-ablaze-after-Iran-claims-underwater-drone-strike-in-Iraqi-waters)

生成摘要时出错

---

## 47. Show HN: Open-source browser for AI agents

**原文标题**: Show HN: Open-source browser for AI agents

**原文链接**: [https://github.com/theredsix/agent-browser-protocol](https://github.com/theredsix/agent-browser-protocol)

生成摘要时出错

---

## 48. Mesh over Bluetooth LE, TCP, or Reticulum

**原文标题**: Mesh over Bluetooth LE, TCP, or Reticulum

**原文链接**: [https://github.com/torlando-tech/columba](https://github.com/torlando-tech/columba)

生成摘要时出错

---

## 49. Bubble Sorted Amen Break

**原文标题**: Bubble Sorted Amen Break

**原文链接**: [https://parametricavocado.itch.io/amen-sorting](https://parametricavocado.itch.io/amen-sorting)

生成摘要时出错

---

## 50. US private credit defaults hit record 9.2% in 2025, Fitch says

**原文标题**: US private credit defaults hit record 9.2% in 2025, Fitch says

**原文链接**: [https://www.marketscreener.com/news/us-private-credit-defaults-hit-record-9-2-in-2025-fitch-says-ce7e5fd8df8fff2d](https://www.marketscreener.com/news/us-private-credit-defaults-hit-record-9-2-in-2025-fitch-says-ce7e5fd8df8fff2d)

生成摘要时出错

---

## 51. Colon cancer now leading cause of cancer deaths under 50 in US

**原文标题**: Colon cancer now leading cause of cancer deaths under 50 in US

**原文链接**: [https://www.theguardian.com/us-news/2026/mar/12/colon-cancer-leading-deaths](https://www.theguardian.com/us-news/2026/mar/12/colon-cancer-leading-deaths)

生成摘要时出错

---

## 52. Physicist Astrid Eichhorn is a leader in the field of asymptotic safety

**原文标题**: Physicist Astrid Eichhorn is a leader in the field of asymptotic safety

**原文链接**: [https://www.quantamagazine.org/where-some-see-strings-she-sees-a-space-time-made-of-fractals-20260311/](https://www.quantamagazine.org/where-some-see-strings-she-sees-a-space-time-made-of-fractals-20260311/)

生成摘要时出错

---

## 53. Why the global elite gave up on spelling and grammar

**原文标题**: Why the global elite gave up on spelling and grammar

**原文链接**: [https://www.wsj.com/lifestyle/jeffrey-epstein-files-bad-grammar-spelling-trump-ellison-dorsey-gates-thiel-cbfe9fb1](https://www.wsj.com/lifestyle/jeffrey-epstein-files-bad-grammar-spelling-trump-ellison-dorsey-gates-thiel-cbfe9fb1)

生成摘要时出错

---

## 54. Claude now creates interactive charts, diagrams and visualizations

**原文标题**: Claude now creates interactive charts, diagrams and visualizations

**原文链接**: [https://claude.com/blog/claude-builds-visuals](https://claude.com/blog/claude-builds-visuals)

生成摘要时出错

---

## 55. The Met Releases High-Def 3D Scans of 140 Famous Art Objects

**原文标题**: The Met Releases High-Def 3D Scans of 140 Famous Art Objects

**原文链接**: [https://www.openculture.com/2026/03/the-met-releases-high-definition-3d-scans-of-140-famous-art-objects.html](https://www.openculture.com/2026/03/the-met-releases-high-definition-3d-scans-of-140-famous-art-objects.html)

生成摘要时出错

---

## 56. Show HN: A context-aware permission guard for Claude Code

**原文标题**: Show HN: A context-aware permission guard for Claude Code

**原文链接**: [https://github.com/manuelschipper/nah/](https://github.com/manuelschipper/nah/)

生成摘要时出错

---

## 57. HyperCard discovery: Neuromancer, Count Zero, Mona Lisa Overdrive (2022)

**原文标题**: HyperCard discovery: Neuromancer, Count Zero, Mona Lisa Overdrive (2022)

**原文链接**: [https://macintoshgarden.org/apps/neuromancer-count-zero-mona-lisa-overdrive](https://macintoshgarden.org/apps/neuromancer-count-zero-mona-lisa-overdrive)

生成摘要时出错

---

## 58. U.S. Navy Turns Down Hormuz Escort Requests Because of High Risk

**原文标题**: U.S. Navy Turns Down Hormuz Escort Requests Because of High Risk

**原文链接**: [https://maritime-executive.com/article/u-s-navy-turns-down-strait-of-hormuz-escort-requests-because-of-high-risk](https://maritime-executive.com/article/u-s-navy-turns-down-strait-of-hormuz-escort-requests-because-of-high-risk)

生成摘要时出错

---

## 59. Show HN: Vanilla JavaScript refinery simulator built to explain job to my kids

**原文标题**: Show HN: Vanilla JavaScript refinery simulator built to explain job to my kids

**原文链接**: [https://fuelingcuriosity.com/game.html](https://fuelingcuriosity.com/game.html)

生成摘要时出错

---

## 60. Show HN: Rudel – Claude Code Session Analytics

**原文标题**: Show HN: Rudel – Claude Code Session Analytics

**原文链接**: [https://github.com/obsessiondb/rudel](https://github.com/obsessiondb/rudel)

生成摘要时出错

---

## 61. AI should not replace people at Atlassian, says CEO

**原文标题**: AI should not replace people at Atlassian, says CEO

**原文链接**: [https://www.heise.de/en/news/Atlassian-CEO-AI-doesn-t-replace-people-here-but-we-re-firing-them-anyway-11208758.html](https://www.heise.de/en/news/Atlassian-CEO-AI-doesn-t-replace-people-here-but-we-re-firing-them-anyway-11208758.html)

生成摘要时出错

---

## 62. SBCL: A Sanely-Bootstrappable Common Lisp (2008) [pdf]

**原文标题**: SBCL: A Sanely-Bootstrappable Common Lisp (2008) [pdf]

**原文链接**: [https://research.gold.ac.uk/id/eprint/2336/1/sbcl.pdf](https://research.gold.ac.uk/id/eprint/2336/1/sbcl.pdf)

生成摘要时出错

---

## 63. Urea prices

**原文标题**: Urea prices

**原文链接**: [https://tradingeconomics.com/commodity/urea](https://tradingeconomics.com/commodity/urea)

生成摘要时出错

---

## 64. Apple releases iOS 15.8.7 to fix Coruna exploit for iPhone 6S from 2015

**原文标题**: Apple releases iOS 15.8.7 to fix Coruna exploit for iPhone 6S from 2015

**原文链接**: [https://support.apple.com/en-us/126632](https://support.apple.com/en-us/126632)

生成摘要时出错

---

## 65. Whistleblower claims ex-DOGE member says he took Social Security data to new job

**原文标题**: Whistleblower claims ex-DOGE member says he took Social Security data to new job

**原文链接**: [https://www.washingtonpost.com/politics/2026/03/10/social-security-data-breach-doge/](https://www.washingtonpost.com/politics/2026/03/10/social-security-data-breach-doge/)

生成摘要时出错

---

## 66. TADA: Speech generation through text-acoustic synchronization

**原文标题**: TADA: Speech generation through text-acoustic synchronization

**原文链接**: [https://www.hume.ai/blog/opensource-tada](https://www.hume.ai/blog/opensource-tada)

生成摘要时出错

---

## 67. DOGE employee stole Social Security data and put it on a thumb drive

**原文标题**: DOGE employee stole Social Security data and put it on a thumb drive

**原文链接**: [https://techcrunch.com/2026/03/10/doge-employee-stole-social-security-data-and-put-it-on-a-thumb-drive-report-says/](https://techcrunch.com/2026/03/10/doge-employee-stole-social-security-data-and-put-it-on-a-thumb-drive-report-says/)

生成摘要时出错

---

## 68. Against vibes: When is a generative model useful

**原文标题**: Against vibes: When is a generative model useful

**原文链接**: [https://www.williamjbowman.com/blog/2026/03/05/against-vibes-when-is-a-generative-model-useful/](https://www.williamjbowman.com/blog/2026/03/05/against-vibes-when-is-a-generative-model-useful/)

生成摘要时出错

---

## 69. How much of HN is AI?

**原文标题**: How much of HN is AI?

**原文链接**: [https://lcamtuf.substack.com/p/how-much-of-hn-is-ai](https://lcamtuf.substack.com/p/how-much-of-hn-is-ai)

生成摘要时出错

---

## 70. Apple's MacBook Neo makes repairs easier and cheaper than other MacBooks

**原文标题**: Apple's MacBook Neo makes repairs easier and cheaper than other MacBooks

**原文链接**: [https://arstechnica.com/gadgets/2026/03/more-modular-design-makes-macbook-neo-easier-to-fix-than-other-apple-laptops/](https://arstechnica.com/gadgets/2026/03/more-modular-design-makes-macbook-neo-easier-to-fix-than-other-apple-laptops/)

生成摘要时出错

---

## 71. Reversing memory loss via gut-brain communication

**原文标题**: Reversing memory loss via gut-brain communication

**原文链接**: [https://med.stanford.edu/news/all-news/2026/03/gut-brain-cognitive-decline.html](https://med.stanford.edu/news/all-news/2026/03/gut-brain-cognitive-decline.html)

生成摘要时出错

---

## 72. Hisense TVs force owners to watch intrusive ads

**原文标题**: Hisense TVs force owners to watch intrusive ads

**原文链接**: [https://www.tomshardware.com/tech-industry/big-tech/hisense-tvs-force-owners-to-watch-intrusive-ads-when-switching-inputs-visiting-the-home-screen-or-even-changing-channels-practice-infuriates-consumers-brand-denies-wrongdoing](https://www.tomshardware.com/tech-industry/big-tech/hisense-tvs-force-owners-to-watch-intrusive-ads-when-switching-inputs-visiting-the-home-screen-or-even-changing-channels-practice-infuriates-consumers-brand-denies-wrongdoing)

生成摘要时出错

---

## 73. Mother of All Grease Fires (1994)

**原文标题**: Mother of All Grease Fires (1994)

**原文链接**: [https://milk.com/wall-o-shame/bucket.html](https://milk.com/wall-o-shame/bucket.html)

生成摘要时出错

---

## 74. Reliable Software in the LLM Era

**原文标题**: Reliable Software in the LLM Era

**原文链接**: [https://quint-lang.org/posts/llm_era](https://quint-lang.org/posts/llm_era)

生成摘要时出错

---

## 75. UK MPs give ministers powers to restrict Internet for under 18s

**原文标题**: UK MPs give ministers powers to restrict Internet for under 18s

**原文链接**: [https://www.openrightsgroup.org/press-releases/mps-give-ministers-powers-to-restrict-entire-internet/](https://www.openrightsgroup.org/press-releases/mps-give-ministers-powers-to-restrict-entire-internet/)

生成摘要时出错

---

## 76. Show HN: Axe – A 12MB binary that replaces your AI framework

**原文标题**: Show HN: Axe – A 12MB binary that replaces your AI framework

**原文链接**: [https://github.com/jrswab/axe](https://github.com/jrswab/axe)

生成摘要时出错

---

## 77. Iran warns U.S. tech firms could become targets as war expands

**原文标题**: Iran warns U.S. tech firms could become targets as war expands

**原文链接**: [https://www.wired.me/story/war-on-big-tech-iran-names-israeli-linked-us-firms-as-potential-targets](https://www.wired.me/story/war-on-big-tech-iran-names-israeli-linked-us-firms-as-potential-targets)

生成摘要时出错

---

## 78. Standardizing source maps

**原文标题**: Standardizing source maps

**原文链接**: [https://bloomberg.github.io/js-blog/post/standardizing-source-maps/](https://bloomberg.github.io/js-blog/post/standardizing-source-maps/)

生成摘要时出错

---

## 79. Show HN: OneCLI – Vault for AI Agents in Rust

**原文标题**: Show HN: OneCLI – Vault for AI Agents in Rust

**原文链接**: [https://github.com/onecli/onecli](https://github.com/onecli/onecli)

生成摘要时出错

---

## 80. Are LLMs not getting better?

**原文标题**: Are LLMs not getting better?

**原文链接**: [https://entropicthoughts.com/no-swe-bench-improvement](https://entropicthoughts.com/no-swe-bench-improvement)

生成摘要时出错

---

## 81. Show HN: Autoresearch@home

**原文标题**: Show HN: Autoresearch@home

**原文链接**: [https://www.ensue-network.ai/autoresearch](https://www.ensue-network.ai/autoresearch)

生成摘要时出错

---

## 82. We were right about Havana syndrome

**原文标题**: We were right about Havana syndrome

**原文链接**: [https://warontherocks.com/2026/03/we-were-right-about-havana-syndrome/](https://warontherocks.com/2026/03/we-were-right-about-havana-syndrome/)

生成摘要时出错

---

## 83. Google to provide Pentagon with AI agents

**原文标题**: Google to provide Pentagon with AI agents

**原文链接**: [https://www.bloomberg.com/news/articles/2026-03-10/google-to-provide-pentagon-with-ai-agents-for-unclassified-work](https://www.bloomberg.com/news/articles/2026-03-10/google-to-provide-pentagon-with-ai-agents-for-unclassified-work)

生成摘要时出错

---

## 84. Another DOGE staffer explaining how he flagged grants at NEH for "DEI"

**原文标题**: Another DOGE staffer explaining how he flagged grants at NEH for "DEI"

**原文链接**: [https://bsky.app/profile/404media.co/post/3mgupw4v3ak2j](https://bsky.app/profile/404media.co/post/3mgupw4v3ak2j)

生成摘要时出错

---

## 85. Oil hits $100 a barrel despite deal to release record amount of reserves

**原文标题**: Oil hits $100 a barrel despite deal to release record amount of reserves

**原文链接**: [https://www.bbc.com/news/articles/c1w5141vx53o](https://www.bbc.com/news/articles/c1w5141vx53o)

生成摘要时出错

---

## 86. U.S. at Fault in Strike on School in Iran, Preliminary Inquiry Says

**原文标题**: U.S. at Fault in Strike on School in Iran, Preliminary Inquiry Says

**原文链接**: [https://www.nytimes.com/2026/03/11/us/politics/iran-school-missile-strike.html](https://www.nytimes.com/2026/03/11/us/politics/iran-school-missile-strike.html)

生成摘要时出错

---

## 87. I don't use LLMs for programming

**原文标题**: I don't use LLMs for programming

**原文链接**: [https://neilmadden.blog/2026/03/02/why-i-dont-use-llms-for-programming/](https://neilmadden.blog/2026/03/02/why-i-dont-use-llms-for-programming/)

生成摘要时出错

---

## 88. Fungal Electronics (2021)

**原文标题**: Fungal Electronics (2021)

**原文链接**: [https://arxiv.org/abs/2111.11231](https://arxiv.org/abs/2111.11231)

生成摘要时出错

---

## 89. Show HN: I built an ISP infrastructure emulator from scratch with a custom vBNG

**原文标题**: Show HN: I built an ISP infrastructure emulator from scratch with a custom vBNG

**原文链接**: [https://aether.saphal.me/dashboard/default](https://aether.saphal.me/dashboard/default)

生成摘要时出错

---

## 90. WireGuard Is Two Things

**原文标题**: WireGuard Is Two Things

**原文链接**: [https://www.proxylity.com/articles/wireguard-is-two-things.html](https://www.proxylity.com/articles/wireguard-is-two-things.html)

生成摘要时出错

---

## 91. Elevated errors on login with Claude Code

**原文标题**: Elevated errors on login with Claude Code

**原文链接**: [https://status.claude.com/incidents/jm3b4jjy2jrt](https://status.claude.com/incidents/jm3b4jjy2jrt)

生成摘要时出错

---

## 92. WA income tax clears House after 24-hour debate

**原文标题**: WA income tax clears House after 24-hour debate

**原文链接**: [https://www.seattletimes.com/seattle-news/politics/wa-income-tax-passes-house-after-24-hour-debate/](https://www.seattletimes.com/seattle-news/politics/wa-income-tax-passes-house-after-24-hour-debate/)

生成摘要时出错

---

## 93. First 6 days of Iran war cost $11.3B

**原文标题**: First 6 days of Iran war cost $11.3B

**原文链接**: [https://www.nbcnews.com/politics/congress/first-6-days-iran-war-cost-11-billion-pentagon-tells-senators-rcna263060](https://www.nbcnews.com/politics/congress/first-6-days-iran-war-cost-11-billion-pentagon-tells-senators-rcna263060)

生成摘要时出错

---

## 94. Preliminary data from a longitudinal AI impact study

**原文标题**: Preliminary data from a longitudinal AI impact study

**原文链接**: [https://newsletter.getdx.com/p/ai-productivity-gains-are-10-not](https://newsletter.getdx.com/p/ai-productivity-gains-are-10-not)

生成摘要时出错

---

## 95. The U.S. borrowed $50B a week for the past five months, the CBO says

**原文标题**: The U.S. borrowed $50B a week for the past five months, the CBO says

**原文链接**: [https://fortune.com/2026/03/10/treasury-debt-borrowing-five-months-deficit-warning/](https://fortune.com/2026/03/10/treasury-debt-borrowing-five-months-deficit-warning/)

生成摘要时出错

---

## 96. USDA is closing buildings, relocating staff, and downsizing-a lot

**原文标题**: USDA is closing buildings, relocating staff, and downsizing-a lot

**原文链接**: [https://www.foodpolitics.com/2026/03/usda-is-closing-buildings-relocating-staff-and-downsizing-a-lot/](https://www.foodpolitics.com/2026/03/usda-is-closing-buildings-relocating-staff-and-downsizing-a-lot/)

生成摘要时出错

---

## 97. Iranian Hacktivists Strike Medical Device Maker Stryker and Wiped Systems

**原文标题**: Iranian Hacktivists Strike Medical Device Maker Stryker and Wiped Systems

**原文链接**: [https://www.zetter-zeroday.com/iranian-hacktivists-strike-medical-device-maker-stryker-in-severe-attack-that-wiped-systems/](https://www.zetter-zeroday.com/iranian-hacktivists-strike-medical-device-maker-stryker-in-severe-attack-that-wiped-systems/)

生成摘要时出错

---

## 98. Emacs internals: Tagged pointers vs. C++ std:variant and LLVM (Part 3)

**原文标题**: Emacs internals: Tagged pointers vs. C++ std:variant and LLVM (Part 3)

**原文链接**: [https://thecloudlet.github.io/blog/project/emacs-03/](https://thecloudlet.github.io/blog/project/emacs-03/)

生成摘要时出错

---

## 99. Anthropic has strong case against Pentagon blacklisting, legal experts say

**原文标题**: Anthropic has strong case against Pentagon blacklisting, legal experts say

**原文链接**: [https://www.reuters.com/legal/legalindustry/anthropic-has-strong-case-against-pentagon-blacklisting-legal-experts-say-2026-03-11/](https://www.reuters.com/legal/legalindustry/anthropic-has-strong-case-against-pentagon-blacklisting-legal-experts-say-2026-03-11/)

生成摘要时出错

---

## 100. I'm going to build my own OpenClaw, with blackjack and bun

**原文标题**: I'm going to build my own OpenClaw, with blackjack and bun

**原文链接**: [https://github.com/rcarmo/piclaw](https://github.com/rcarmo/piclaw)

生成摘要时出错

---

