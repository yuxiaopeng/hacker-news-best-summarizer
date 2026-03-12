# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-03-12.md)

*最后自动更新时间: 2026-03-12 20:10:52*
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

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 2 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 3 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 4 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 5 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 6 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 7 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 8 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 9 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 10 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 11 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 12 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 13 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 14 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 15 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 16 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 17 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 18 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 19 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 20 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 21 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 22 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 23 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 24 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 25 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 26 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 27 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 28 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 29 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 30 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 31 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 32 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 33 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 34 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 35 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 36 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 37 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 38 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 39 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 40 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 41 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 42 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 43 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 44 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 45 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 46 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 47 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 48 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 49 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 50 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 51 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 52 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 53 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 54 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 55 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 56 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 57 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 58 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 59 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 60 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 61 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 62 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 63 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 64 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 65 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 66 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 67 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 68 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 69 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 70 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 71 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 72 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 73 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 74 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 75 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 76 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 77 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 78 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 79 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 80 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 81 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 82 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 83 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 84 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 85 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 86 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 87 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 88 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 89 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 90 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 91 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 92 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 93 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 94 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 95 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 96 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 97 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 98 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 99 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 100 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 101 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 102 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 103 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 104 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 105 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 106 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 107 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 108 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 109 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 110 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 111 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 112 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 113 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 114 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 115 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 116 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 117 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 118 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 119 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 120 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 121 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 122 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 123 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 124 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 125 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 126 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
