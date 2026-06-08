# Hacker News 热门文章摘要 (2026-06-08)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. LLMs are eroding my software engineering career and I don't know what to do

**原文标题**: LLMs are eroding my software engineering career and I don't know what to do

**原文链接**: [https://human-in-the-loop.bearblog.dev/llms-are-eroding-my-software-engineering-career-and-i-dont-know-what-to-do/](https://human-in-the-loop.bearblog.dev/llms-are-eroding-my-software-engineering-career-and-i-dont-know-what-to-do/)

A 10-year experienced software engineer, specialized in finance and payment systems, describes how LLMs are eroding his career pillars.

He initially focused on becoming a domain expert in finance, but found his specialized knowledge quickly becoming redundant. LLMs, initially used for design docs, soon demonstrated the ability to connect complex domain-specific concepts, like idempotency and payment lifecycles, negating years of accumulated human experience.

Next, his hard-won debugging expertise, especially in distributed systems, was undermined. While LLMs initially aided in coding, advanced models like Claude 4.5+ combined with agentic workflows (MCPs) began "one-shotting" complex bugs, even across distributed systems and undocumented APIs, making his debugging intuition largely promptable. He now feels like an "off-the-shelf" engineer, losing his unique differentiators.

His final pillar, code quality and software architecture (DDD, Clean Architecture), is also eroding. While LLM agents often produce suboptimal code, the industry is increasingly accepting "C or D-grade" codebases, viewing architectural "taste" as less critical when code is primarily read and modified by machines.

The author expresses deep concern for his long-term employability. He notes widespread layoffs and a shift in hiring towards generalist roles, increasing competition. He struggles to identify new areas of expertise that LLMs won't easily master, contemplating radical career shifts like pursuing advanced ML research or even woodworking.

---

## 2. Building from zero after addiction, prison, and a felony

**原文标题**: Building from zero after addiction, prison, and a felony

**原文链接**: [https://gavinray97.github.io/blog/building-from-zero-after-addiction-prison-felony](https://gavinray97.github.io/blog/building-from-zero-after-addiction-prison-felony)

生成摘要时出错

---

## 3. Dopamine Fracking

**原文标题**: Dopamine Fracking

**原文链接**: [https://igerman.cc/blog/dopamine-fracking/](https://igerman.cc/blog/dopamine-fracking/)

生成摘要时出错

---

## 4. Show HN: Performative-UI – a react component library of design tropes

**原文标题**: Show HN: Performative-UI – a react component library of design tropes

**原文链接**: [https://vorpus.github.io/performativeUI/](https://vorpus.github.io/performativeUI/)

生成摘要时出错

---

## 5. 安特罗皮克，请推出官方的克劳德 Linux 桌面版。

**原文标题**: Anthropic, please ship an official Claude Desktop for Linux

**原文链接**: [https://github.com/anthropics/claude-code/issues/65697](https://github.com/anthropics/claude-code/issues/65697)

本文是向Anthropic公司提出的一项功能请求（#65697），要求其推出适用于Linux的官方Claude桌面应用程序，特别是针对Ubuntu LTS和Debian。

核心问题是，尽管Anthropic为macOS和Windows提供了Claude桌面版，但Linux用户没有官方GUI客户端来使用桌面扩展（这对Claude Code插件的开发和测试至关重要）、计算机使用、听写或Cowork等功能。这迫使开发者为了插件工作而切换操作系统，并导致普通Linux用户依赖于非官方、未经审计的第三方Windows Electron构建包，这些打包处理敏感的OAuth令牌和API密钥，构成重大的安全风险。

作者认为，官方Linux构建在结构上是可行的，因为Anthropic已经通过签名仓库分发其他Linux软件（Claude Code CLI），并且Cowork代理在macOS上内部运行Linux虚拟机，这表明产品内部存在现有的Linux执行路径。Linux也是一个重要的开发者平台，其中Ubuntu是27.7%专业开发者的主要操作系统。

提出的解决方案是Anthropic通过其现有的apt仓库基础设施，发布官方签名的.deb格式Linux构建版。如果第一方构建不可行，作者请求发布一份关于路线图的公开声明，认可并推荐一个社区项目，同时提供安全审查和指导。该请求强调了开发者面临的障碍，以及当前对Linux支持“保持沉默”所带来的安全隐患。

---

## 6. Stop the Apple Music app from launching

**原文标题**: Stop the Apple Music app from launching

**原文链接**: [https://lowtechguys.com/musicdecoy/](https://lowtechguys.com/musicdecoy/)

生成摘要时出错

---

## 7. Linear 如何如此之快？技术解析

**原文标题**: How's Linear so fast? A technical breakdown

**原文链接**: [https://performance.dev/how-is-linear-so-fast-a-technical-breakdown](https://performance.dev/how-is-linear-so-fast-a-technical-breakdown)

Linear 实现其近乎即时的速度，主要是通过颠覆传统的 Web 应用关系：其 UI 的主要数据库位于浏览器中 (IndexedDB)。数据变动（mutations）首先在本地应用，更新内存存储（例如 MobX observable），并同步重新渲染 UI，从而有效地消除了依赖网络的加载指示器。一个异步同步引擎随后处理服务器通信和更新广播。这种“乐观更新”原则确保了 UI 的响应速度不依赖于网络延迟。

为了其客户端渲染应用能够快速初始加载，Linear 精心优化了代码交付。他们采用了激进的代码分割、放弃对旧版浏览器的支持，并创建了数百个路由级别的 JavaScript 代码块。关键路径的代码块在 `<head>` 中通过 `modulepreload` 进行预加载以实现并行抓取，而 Service Worker 则缓存剩余资源，以提供离线功能和后续的即时导航。第三方库也被单独分块，以实现高效缓存。字体加载通过可变字体、`font-display: swap` 和正确的 `crossorigin` 预加载进行了优化。最后，内联的应用程序外壳 CSS 确保了即时加载状态，进一步掩盖了网络依赖。

Linear 的速度源于其核心承诺：向用户隐藏所有网络请求、优先提供即时的 UI 反馈，并优化从构建过程到运行时资源交付的每一个细节。

---

## 8. 反社交：如今主宰社交媒体动态的，是潮流而非朋友。

**原文标题**: Anti-social: It's fads, not friends, which now dominate social media feeds

**原文链接**: [https://www.bbc.com/worklife/article/20260520-how-social-media-ceased-to-be-social](https://www.bbc.com/worklife/article/20260520-how-social-media-ceased-to-be-social)

社交媒体平台正迅速从以朋友为中心的交流工具转变为被潮流和专业制作内容主导的娱乐中心。这种转变是由旨在最大化用户参与度和广告收入的算法驱动的。许多用户，像奥雷莉亚一样，现在主要看到的是热门内容和广告，很少是朋友的帖子，这导致他们自己也停止发布内容。

这种趋势在年轻用户中尤为明显，他们宁愿消费不认识的内容创作者的视频，也不愿与朋友互动。这一转变反映在统计数据中，显示法国、英国和美国的活跃发帖量显著下降。临床心理学家瓦内萨·拉洛认为，用户更在意自己的数字足迹和潜在批评，因此将个人分享转移到WhatsApp等更私密的即时通讯应用或Instagram和Snapchat上的封闭群组，以进行真正的社交互动。

社交媒体顾问马特·纳瓦拉强调了一种“分化”：Instagram和TikTok等大型平台正成为娱乐和发现引擎，而WhatsApp则处理真正的社交联系。由TikTok开创并被Meta采用的算法，优先考虑基于预测参与度的内容，而非现有友谊，这使得直接联系在信息流中不再是核心。这种转变迫使小企业成为高水平的内容创作者，以保持可见性。

尽管远离了传统的“社交”互动，但这些平台的核心广告收入商业模式仍在蓬勃发展。人工智能驱动的广告投放，利用海量用户数据，日益高效和精准，为Meta等公司带来了可观的收入增长。虽然用户在社交媒体上花费的总时间已趋于平稳，但用户总数和Z世代（他们将其用于搜索和购物）的参与度依然很高，这表明它们已成功转型为被动、定制化的娱乐体验，尽管存在优先显示朋友内容的工具，但大多数用户并未利用它们。

---

## 9. MiMo-v2.5-Pro-UltraSpeed: 1T model with 1000 tokens per second

**原文标题**: MiMo-v2.5-Pro-UltraSpeed: 1T model with 1000 tokens per second

**原文链接**: [https://mimo.xiaomi.com/blog/mimo-tilert-1000tps](https://mimo.xiaomi.com/blog/mimo-tilert-1000tps)

Xiaomi MiMo-V2.5-Pro-UltraSpeed, in collaboration with TileRT, has achieved a breakthrough 1000 tokens/s (TPS) generation speed for a 1-trillion-parameter (1T) model on commodity GPUs. This unprecedented speed is hailed as a paradigm shift, enabling AI to perform parallel reasoning, drastically boost coding agent productivity, and facilitate real-time decision-making in critical scenarios like high-frequency trading, anti-fraud, and life-saving medical analysis.

This achievement stems from an "extreme model-system codesign." On the model side, MiMo employs selective FP4 quantization for its MoE Experts, dramatically reducing memory footprint and bandwidth. It also leverages DFlash, an innovative block-level masked parallel prediction speculative decoding method that efficiently generates and verifies multiple tokens simultaneously, achieving high acceptance rates, especially in coding.

On the system side, TileRT developed ultra-low-latency inference kernels and a novel execution model. This system eliminates "execution gaps" through a "Persistent Engine Kernel" for continuous prefetching and "Warp Specialization" for heterogeneous pipeline collaboration, maximizing GPU utilization. TileRT's custom compilation engine and kernels are tightly coupled with MiMo's algorithmic innovations.

Access to the UltraSpeed API is available via a limited, application-based trial from June 9-23, 2026, offering 10x speed at 3x the cost, with free chat access for approved users. The MiMo-V2.5-Pro-FP4-DFlash checkpoint has also been open-sourced on HuggingFace.

---

## 10. The 29th International Obfuscated C Code Contest (IOCCC) 2025 Winners

**原文标题**: The 29th International Obfuscated C Code Contest (IOCCC) 2025 Winners

**原文链接**: [https://www.ioccc.org/2025/](https://www.ioccc.org/2025/)

生成摘要时出错

---

## 11. A Farmer Donated Land to Turn into a Park. The City Is Building a Data Center

**原文标题**: A Farmer Donated Land to Turn into a Park. The City Is Building a Data Center

**原文链接**: [https://www.404media.co/a-farmer-donated-land-to-turn-into-a-park-the-city-is-building-a-massive-data-center-instead/](https://www.404media.co/a-farmer-donated-land-to-turn-into-a-park-the-city-is-building-a-massive-data-center-instead/)

生成摘要时出错

---

## 12. DeepSeek V4 Pro beats GPT-5.5 Pro on precision

**原文标题**: DeepSeek V4 Pro beats GPT-5.5 Pro on precision

**原文链接**: [https://runtimewire.com/article/deepseek-v4-pro-beats-gpt-5-5-pro-on-precision](https://runtimewire.com/article/deepseek-v4-pro-beats-gpt-5-5-pro-on-precision)

生成摘要时出错

---

## 13. Show HN: Lathe – Use LLMs to learn a new domain, not skip past it

**原文标题**: Show HN: Lathe – Use LLMs to learn a new domain, not skip past it

**原文链接**: [https://github.com/devenjarvis/lathe](https://github.com/devenjarvis/lathe)

生成摘要时出错

---

## 14. How much of Thermo Fisher's antibody data has been manipulated?

**原文标题**: How much of Thermo Fisher's antibody data has been manipulated?

**原文链接**: [https://reeserichardson.blog/2026/05/28/how-much-of-thermo-fishers-antibody-data-has-been-manipulated/](https://reeserichardson.blog/2026/05/28/how-much-of-thermo-fishers-antibody-data-has-been-manipulated/)

生成摘要时出错

---

## 15. Scientists ejected from diabetes conference for distributing journal reprints

**原文标题**: Scientists ejected from diabetes conference for distributing journal reprints

**原文链接**: [https://arstechnica.com/science/2026/06/scientists-ejected-from-diabetes-conference-for-distributing-journal-reprints/](https://arstechnica.com/science/2026/06/scientists-ejected-from-diabetes-conference-for-distributing-journal-reprints/)

生成摘要时出错

---

## 16. The Cypherpunk Library

**原文标题**: The Cypherpunk Library

**原文链接**: [https://www.cypherpunkbooks.com](https://www.cypherpunkbooks.com)

生成摘要时出错

---

## 17. Making peace with your unlived dreams (2023)

**原文标题**: Making peace with your unlived dreams (2023)

**原文链接**: [https://nik.art/making-peace-with-your-unlived-dreams/](https://nik.art/making-peace-with-your-unlived-dreams/)

生成摘要时出错

---

## 18. I design with Claude more than Figma now

**原文标题**: I design with Claude more than Figma now

**原文链接**: [https://blog.janestreet.com/i-design-with-claude-code-more-than-figma-now-index/](https://blog.janestreet.com/i-design-with-claude-code-more-than-figma-now-index/)

生成摘要时出错

---

## 19. The Smallest Brain You Can Build: A Perceptron in Python

**原文标题**: The Smallest Brain You Can Build: A Perceptron in Python

**原文链接**: [https://ranpara.net/posts/perceptron-explained-from-scratch/](https://ranpara.net/posts/perceptron-explained-from-scratch/)

生成摘要时出错

---

## 20. 1k Data Breaches Later, the Disclosure Lag Is Worse

**原文标题**: 1k Data Breaches Later, the Disclosure Lag Is Worse

**原文链接**: [https://www.troyhunt.com/1000-data-breaches-later-the-disclosure-lag-is-worse-than-ever/](https://www.troyhunt.com/1000-data-breaches-later-the-disclosure-lag-is-worse-than-ever/)

生成摘要时出错

---

## 21. xAI is looking more like a datacentre REIT than a frontier lab

**原文标题**: xAI is looking more like a datacentre REIT than a frontier lab

**原文链接**: [https://martinalderson.com/posts/xais-new-rental-business/](https://martinalderson.com/posts/xais-new-rental-business/)

生成摘要时出错

---

## 22. Major P2P issues in Israel and possibly other Middle East countries

**原文标题**: Major P2P issues in Israel and possibly other Middle East countries

**原文链接**: [https://github.com/ValveSoftware/GameNetworkingSockets/issues/398](https://github.com/ValveSoftware/GameNetworkingSockets/issues/398)

生成摘要时出错

---

## 23. New drug 'functionally cures' many hepatitis B virus infections

**原文标题**: New drug 'functionally cures' many hepatitis B virus infections

**原文链接**: [https://www.science.org/content/article/new-drug-functionally-cures-many-hepatitis-b-virus-infections?user_id=66c4bf745d78644b3aa57b08](https://www.science.org/content/article/new-drug-functionally-cures-many-hepatitis-b-virus-infections?user_id=66c4bf745d78644b3aa57b08)

生成摘要时出错

---

## 24. APC–2 – A professional record cutter for producing original playback discs

**原文标题**: APC–2 – A professional record cutter for producing original playback discs

**原文链接**: [https://teenage.engineering/products/apc-2](https://teenage.engineering/products/apc-2)

生成摘要时出错

---

## 25. Public Domain Image Archive

**原文标题**: Public Domain Image Archive

**原文链接**: [https://pdimagearchive.org/](https://pdimagearchive.org/)

生成摘要时出错

---

## 26. AI is slowing down

**原文标题**: AI is slowing down

**原文链接**: [https://www.wheresyoured.at/ai-is-slowing-down/](https://www.wheresyoured.at/ai-is-slowing-down/)

生成摘要时出错

---

## 27. New U.S. college grads now have higher unemployment than the average worker

**原文标题**: New U.S. college grads now have higher unemployment than the average worker

**原文链接**: [https://www.randalolson.com/2026/06/04/recent-grad-unemployment-flip/](https://www.randalolson.com/2026/06/04/recent-grad-unemployment-flip/)

生成摘要时出错

---

## 28. Siri AI

**原文标题**: Siri AI

**原文链接**: [https://www.apple.com/apple-intelligence/](https://www.apple.com/apple-intelligence/)

生成摘要时出错

---

## 29. Apple WWDC 2026

**原文标题**: Apple WWDC 2026

**原文链接**: [https://www.apple.com/apple-events/event-stream/](https://www.apple.com/apple-events/event-stream/)

生成摘要时出错

---

## 30. Zig by Example

**原文标题**: Zig by Example

**原文链接**: [https://github.com/boringcollege/zig-by-example](https://github.com/boringcollege/zig-by-example)

生成摘要时出错

---

## 31. An Ohio Valley 100k-watt FM signal is severed in broad daylight

**原文标题**: An Ohio Valley 100k-watt FM signal is severed in broad daylight

**原文链接**: [https://www.radioworld.com/news-and-business/headlines/an-ohio-valley-100000-watt-fm-signal-is-severed-in-broad-daylight](https://www.radioworld.com/news-and-business/headlines/an-ohio-valley-100000-watt-fm-signal-is-severed-in-broad-daylight)

生成摘要时出错

---

## 32. How liminalism became the defining aesthetic

**原文标题**: How liminalism became the defining aesthetic

**原文链接**: [https://hyperallergic.com/how-liminalism-became-the-defining-aesthetic-of-our-time/](https://hyperallergic.com/how-liminalism-became-the-defining-aesthetic-of-our-time/)

生成摘要时出错

---

## 33. Vitamin D3 During Pregnancy and Cognitive Performance at 10 Years

**原文标题**: Vitamin D3 During Pregnancy and Cognitive Performance at 10 Years

**原文链接**: [https://jamanetwork.com/journals/jamanetworkopen/fullarticle/2849122](https://jamanetwork.com/journals/jamanetworkopen/fullarticle/2849122)

生成摘要时出错

---

## 34. Age verification tech could put children at greater risk, says think tank

**原文标题**: Age verification tech could put children at greater risk, says think tank

**原文链接**: [https://www.computerweekly.com/news/366643835/Age-verification-tech-could-put-children-at-greater-risk-says-think-tank](https://www.computerweekly.com/news/366643835/Age-verification-tech-could-put-children-at-greater-risk-says-think-tank)

生成摘要时出错

---

## 35. Apple reveals new AI architecture built around Google Gemini models

**原文标题**: Apple reveals new AI architecture built around Google Gemini models

**原文链接**: [https://www.macrumors.com/2026/06/08/apple-reveals-new-ai-architecture/](https://www.macrumors.com/2026/06/08/apple-reveals-new-ai-architecture/)

生成摘要时出错

---

## 36. Tokenomics: Quantifying Where Tokens Are Used in Agentic Software Engineering

**原文标题**: Tokenomics: Quantifying Where Tokens Are Used in Agentic Software Engineering

**原文链接**: [https://arxiv.org/abs/2601.14470](https://arxiv.org/abs/2601.14470)

生成摘要时出错

---

## 37. Field of clones: How horse replicas came to dominate polo

**原文标题**: Field of clones: How horse replicas came to dominate polo

**原文链接**: [https://knowablemagazine.org/content/article/technology/2026/cloned-polo-horses](https://knowablemagazine.org/content/article/technology/2026/cloned-polo-horses)

生成摘要时出错

---

## 38. Massachusetts bans sale of precise location data in new privacy rights bill

**原文标题**: Massachusetts bans sale of precise location data in new privacy rights bill

**原文链接**: [https://techcrunch.com/2026/06/08/massachusetts-votes-to-pass-new-privacy-rights-bill-that-bans-sale-of-precise-location-data/](https://techcrunch.com/2026/06/08/massachusetts-votes-to-pass-new-privacy-rights-bill-that-bans-sale-of-precise-location-data/)

生成摘要时出错

---

## 39. A Matter Wi-Fi Light Bulb in Rust on the Raspberry Pi Pico 2 W

**原文标题**: A Matter Wi-Fi Light Bulb in Rust on the Raspberry Pi Pico 2 W

**原文链接**: [https://github.com/melastmohican/rust-rpico2-embassy-examples](https://github.com/melastmohican/rust-rpico2-embassy-examples)

生成摘要时出错

---

## 40. OneDrive data now has an expiry date

**原文标题**: OneDrive data now has an expiry date

**原文链接**: [https://ms365news.com/blogs/f/your-onedrive-data-now-has-an-expiry-data](https://ms365news.com/blogs/f/your-onedrive-data-now-has-an-expiry-data)

生成摘要时出错

---

## 41. Why are so many young people getting cancer?

**原文标题**: Why are so many young people getting cancer?

**原文链接**: [https://www.nature.com/articles/d41586-026-01780-6](https://www.nature.com/articles/d41586-026-01780-6)

生成摘要时出错

---

## 42. Texas grid flags risks as data centers, crypto sites fail voltage tests

**原文标题**: Texas grid flags risks as data centers, crypto sites fail voltage tests

**原文链接**: [https://www.reuters.com/business/energy/texas-grid-flags-risks-data-centers-crypto-sites-fail-voltage-tests-2026-06-05/](https://www.reuters.com/business/energy/texas-grid-flags-risks-data-centers-crypto-sites-fail-voltage-tests-2026-06-05/)

生成摘要时出错

---

## 43. The gamers taking on the industry to stop it switching off games

**原文标题**: The gamers taking on the industry to stop it switching off games

**原文链接**: [https://www.bbc.com/news/articles/c8e8e7g0r82o](https://www.bbc.com/news/articles/c8e8e7g0r82o)

生成摘要时出错

---

## 44. Algorithmic Monocultures in Hiring

**原文标题**: Algorithmic Monocultures in Hiring

**原文链接**: [https://algorithmichiring.github.io/](https://algorithmichiring.github.io/)

生成摘要时出错

---

## 45. The OnlyFans Economy of American AI

**原文标题**: The OnlyFans Economy of American AI

**原文链接**: [https://leoveanu.com/2026-06-06-qwen3.7max/](https://leoveanu.com/2026-06-06-qwen3.7max/)

生成摘要时出错

---

## 46. The EU Open Source Strategy

**原文标题**: The EU Open Source Strategy

**原文链接**: [https://digital-strategy.ec.europa.eu/en/policies/open-source-strategy](https://digital-strategy.ec.europa.eu/en/policies/open-source-strategy)

生成摘要时出错

---

## 47. Office-open-xml-viewer: Office XML document viewer that renders to HTML Canvas

**原文标题**: Office-open-xml-viewer: Office XML document viewer that renders to HTML Canvas

**原文链接**: [https://github.com/yukiyokotani/office-open-xml-viewer](https://github.com/yukiyokotani/office-open-xml-viewer)

生成摘要时出错

---

## 48. 1worldflag: A blue dot on a transparent background

**原文标题**: 1worldflag: A blue dot on a transparent background

**原文链接**: [https://1worldflag.com/](https://1worldflag.com/)

生成摘要时出错

---

## 49. Switzerland wil have a referendum to cap population at 10M

**原文标题**: Switzerland wil have a referendum to cap population at 10M

**原文链接**: [https://www.admin.ch/en/sustainability-initiative](https://www.admin.ch/en/sustainability-initiative)

生成摘要时出错

---

## 50. Podman 6: machine usability improvements (2025)

**原文标题**: Podman 6: machine usability improvements (2025)

**原文链接**: [https://blog.podman.io/2025/10/podman-6-machine-usability-improvements/](https://blog.podman.io/2025/10/podman-6-machine-usability-improvements/)

生成摘要时出错

---

## 51. EU-banned pesticides found in rice, tea and spices

**原文标题**: EU-banned pesticides found in rice, tea and spices

**原文链接**: [https://www.foodwatch.org/en/eu-banned-pesticides-found-in-rice-tea-and-spices](https://www.foodwatch.org/en/eu-banned-pesticides-found-in-rice-tea-and-spices)

生成摘要时出错

---

## 52. Richard Scolyer Has Died

**原文标题**: Richard Scolyer Has Died

**原文链接**: [https://www.bbc.com/news/articles/c14yz5jg476o](https://www.bbc.com/news/articles/c14yz5jg476o)

生成摘要时出错

---

## 53. Firefox Merges Support for Vulkan Video Decoding

**原文标题**: Firefox Merges Support for Vulkan Video Decoding

**原文链接**: [https://www.phoronix.com/news/Firefox-Vulkan-Video-Merged](https://www.phoronix.com/news/Firefox-Vulkan-Video-Merged)

生成摘要时出错

---

## 54. I replaced Spotify with a homemade FM radio station

**原文标题**: I replaced Spotify with a homemade FM radio station

**原文链接**: [https://old.reddit.com/r/digitalminimalism/comments/1tes8yu/i_replaced_spotify_with_a_homemade_fm_radio/](https://old.reddit.com/r/digitalminimalism/comments/1tes8yu/i_replaced_spotify_with_a_homemade_fm_radio/)

生成摘要时出错

---

## 55. Replies to comments on my "LLMs are eroding my career" post

**原文标题**: Replies to comments on my "LLMs are eroding my career" post

**原文链接**: [https://human-in-the-loop.bearblog.dev/replies-to-comments-on-my-llms-are-eroding-my-career-post/](https://human-in-the-loop.bearblog.dev/replies-to-comments-on-my-llms-are-eroding-my-career-post/)

生成摘要时出错

---

## 56. The circus freaks of open source

**原文标题**: The circus freaks of open source

**原文链接**: [https://drewdevault.com/blog/Circus-freaks-of-FOSS/](https://drewdevault.com/blog/Circus-freaks-of-FOSS/)

生成摘要时出错

---

## 57. Are you expected to run five Python type-checkers now?

**原文标题**: Are you expected to run five Python type-checkers now?

**原文链接**: [https://pyrefly.org/blog/too-many-type-checkers/](https://pyrefly.org/blog/too-many-type-checkers/)

生成摘要时出错

---

## 58. If LLMs Have Human-Like Attributes, Then So Does Age of Empires II

**原文标题**: If LLMs Have Human-Like Attributes, Then So Does Age of Empires II

**原文链接**: [https://arxiv.org/abs/2605.31514](https://arxiv.org/abs/2605.31514)

生成摘要时出错

---

## 59. Full Reverse Engineering of the TI-84 Plus Operating System

**原文标题**: Full Reverse Engineering of the TI-84 Plus Operating System

**原文链接**: [https://siraben.github.io/ti84p-re/](https://siraben.github.io/ti84p-re/)

生成摘要时出错

---

## 60. Spanish traders set the standard for GnuCash database design

**原文标题**: Spanish traders set the standard for GnuCash database design

**原文链接**: [https://handson.money/blog/2026-06-06-horse-arse-and-design/](https://handson.money/blog/2026-06-06-horse-arse-and-design/)

生成摘要时出错

---

## 61. Italy's Bending Spoons, owner of AOL and Vimeo, files for Nasdaq IPO

**原文标题**: Italy's Bending Spoons, owner of AOL and Vimeo, files for Nasdaq IPO

**原文链接**: [https://www.reuters.com/legal/transactional/italys-bending-spoons-files-us-ipo-2026-06-08/](https://www.reuters.com/legal/transactional/italys-bending-spoons-files-us-ipo-2026-06-08/)

生成摘要时出错

---

## 62. 7.8 magnitude earthquake shakes part of southern Philippines. Tsunami possible

**原文标题**: 7.8 magnitude earthquake shakes part of southern Philippines. Tsunami possible

**原文链接**: [https://www.yahoo.com/news/weather-news/articles/as--philippines-earthquake-001322726.html](https://www.yahoo.com/news/weather-news/articles/as--philippines-earthquake-001322726.html)

生成摘要时出错

---

## 63. Launch HN: Intuned (YC S22) – Build and run reliable browser automations as code

**原文标题**: Launch HN: Intuned (YC S22) – Build and run reliable browser automations as code

**原文链接**: [https://intunedhq.com](https://intunedhq.com)

生成摘要时出错

---

## 64. Powering up a module from the IBM 604: an electronic calculator from 1948

**原文标题**: Powering up a module from the IBM 604: an electronic calculator from 1948

**原文链接**: [https://www.righto.com/2026/06/ibm-604-thyraton-tube-module.html](https://www.righto.com/2026/06/ibm-604-thyraton-tube-module.html)

生成摘要时出错

---

## 65. Sam Bankman-Fried applies for a pardon from Trump

**原文标题**: Sam Bankman-Fried applies for a pardon from Trump

**原文链接**: [https://techcrunch.com/2026/06/08/sam-bankman-fried-applies-for-a-pardon-from-trump/](https://techcrunch.com/2026/06/08/sam-bankman-fried-applies-for-a-pardon-from-trump/)

生成摘要时出错

---

## 66. Why isn't the U.S. better at soccer?

**原文标题**: Why isn't the U.S. better at soccer?

**原文链接**: [https://www.natesilver.net/p/why-isnt-the-us-better-at-soccer](https://www.natesilver.net/p/why-isnt-the-us-better-at-soccer)

生成摘要时出错

---

## 67. Wow, if it's this easy in 1998, I bet it'll be even easier in 2026

**原文标题**: Wow, if it's this easy in 1998, I bet it'll be even easier in 2026

**原文链接**: [https://retro.social/@ifixcoinops/116711332505710610](https://retro.social/@ifixcoinops/116711332505710610)

生成摘要时出错

---

## 68. My automated doubt development process

**原文标题**: My automated doubt development process

**原文链接**: [https://www.alexself.dev/blog/automated-doubt](https://www.alexself.dev/blog/automated-doubt)

生成摘要时出错

---

## 69. The iPhone explains 33–52% of fertility decline among women aged 15–44

**原文标题**: The iPhone explains 33–52% of fertility decline among women aged 15–44

**原文链接**: [https://www.nber.org/papers/w35310](https://www.nber.org/papers/w35310)

生成摘要时出错

---

## 70. The architecture of the internet creates risks for democracy

**原文标题**: The architecture of the internet creates risks for democracy

**原文链接**: [https://www.science.org/doi/10.1126/science.aei2409](https://www.science.org/doi/10.1126/science.aei2409)

生成摘要时出错

---

## 71. Flock license plate reader wrongly linked a San Diego man to a violent crime

**原文标题**: Flock license plate reader wrongly linked a San Diego man to a violent crime

**原文链接**: [https://timesofsandiego.com/crime/2026/06/07/a-flock-license-plate-reader-linked-a-san-diego-man-to-a-violent-crime-he-was-five-miles-away/](https://timesofsandiego.com/crime/2026/06/07/a-flock-license-plate-reader-linked-a-san-diego-man-to-a-violent-crime-he-was-five-miles-away/)

生成摘要时出错

---

## 72. Show HN: Kyushu – A self-hostable WASM sandbox for JavaScript workers

**原文标题**: Show HN: Kyushu – A self-hostable WASM sandbox for JavaScript workers

**原文链接**: [https://kyushu.dev/](https://kyushu.dev/)

生成摘要时出错

---

## 73. Surveillance Is Not Safety: A statement on the UK's latest threat to privacy [pdf]

**原文标题**: Surveillance Is Not Safety: A statement on the UK's latest threat to privacy [pdf]

**原文链接**: [https://signal.org/blog/pdfs/2026-06-08-uk-surveillance-is-not-safety.pdf](https://signal.org/blog/pdfs/2026-06-08-uk-surveillance-is-not-safety.pdf)

生成摘要时出错

---

## 74. GitHub Is Down

**原文标题**: GitHub Is Down

**原文链接**: [https://www.githubstatus.com/incidents/m7n7sm0sr1pz](https://www.githubstatus.com/incidents/m7n7sm0sr1pz)

生成摘要时出错

---

## 75. DoD Officially Drops 180 Faiths from Military's Recognized Religion List

**原文标题**: DoD Officially Drops 180 Faiths from Military's Recognized Religion List

**原文链接**: [https://www.military.com/dod-officially-drops-180-faiths-from-militarys-recognized-religion-list](https://www.military.com/dod-officially-drops-180-faiths-from-militarys-recognized-religion-list)

生成摘要时出错

---

## 76. Show HN: Oproxy – inspect and modify network traffic from the browser

**原文标题**: Show HN: Oproxy – inspect and modify network traffic from the browser

**原文链接**: [https://github.com/sauravrao637/oproxy](https://github.com/sauravrao637/oproxy)

生成摘要时出错

---

## 77. Config Files That Run Code: Supply Chain Security Blindspot

**原文标题**: Config Files That Run Code: Supply Chain Security Blindspot

**原文链接**: [https://safedep.io/config-files-that-run-code/](https://safedep.io/config-files-that-run-code/)

生成摘要时出错

---

## 78. Thunderbird Littering My Home

**原文标题**: Thunderbird Littering My Home

**原文链接**: [https://thefoggiest.dev/2026/06/04/thunderbird-littering-my-home](https://thefoggiest.dev/2026/06/04/thunderbird-littering-my-home)

生成摘要时出错

---

## 79. Anthropic/OpenAI may be spending more than $1000 for every $100 you pay them

**原文标题**: Anthropic/OpenAI may be spending more than $1000 for every $100 you pay them

**原文链接**: [https://ea.rna.nl/2026/06/07/anthropic-openai-may-be-spending-more-than-1000-for-every-100-you-pay-them/](https://ea.rna.nl/2026/06/07/anthropic-openai-may-be-spending-more-than-1000-for-every-100-you-pay-them/)

生成摘要时出错

---

## 80. Why are cells small?

**原文标题**: Why are cells small?

**原文链接**: [https://burrito.bio/essays/what-limits-a-cells-size](https://burrito.bio/essays/what-limits-a-cells-size)

生成摘要时出错

---

## 81. The Butlerian Jihad Has Begun

**原文标题**: The Butlerian Jihad Has Begun

**原文链接**: [https://syndekit.substack.com/p/the-butlerian-jihad-has-begun](https://syndekit.substack.com/p/the-butlerian-jihad-has-begun)

生成摘要时出错

---

## 82. Cannibalism

**原文标题**: Cannibalism

**原文链接**: [https://b-ark.ca/2026/06/07/cannibalism.html](https://b-ark.ca/2026/06/07/cannibalism.html)

生成摘要时出错

---

## 83. Doing Nothing at Work

**原文标题**: Doing Nothing at Work

**原文链接**: [https://www.seangoedecke.com/doing-nothing-at-work/](https://www.seangoedecke.com/doing-nothing-at-work/)

生成摘要时出错

---

## 84. Tech sell-off widens as South Korea index plunges

**原文标题**: Tech sell-off widens as South Korea index plunges

**原文链接**: [https://www.ft.com/content/2f0f727b-5315-445c-b8f1-6aa65bd7474c](https://www.ft.com/content/2f0f727b-5315-445c-b8f1-6aa65bd7474c)

生成摘要时出错

---

## 85. Nvidia partners with LG robotics to build humanoid robots in South Korea

**原文标题**: Nvidia partners with LG robotics to build humanoid robots in South Korea

**原文链接**: [https://blogs.nvidia.com/blog/nvidia-and-lg-group-ai-factory/](https://blogs.nvidia.com/blog/nvidia-and-lg-group-ai-factory/)

生成摘要时出错

---

## 86. A CGo-free port of SQLite/SQLite3

**原文标题**: A CGo-free port of SQLite/SQLite3

**原文链接**: [https://gitlab.com/cznic/sqlite](https://gitlab.com/cznic/sqlite)

生成摘要时出错

---

## 87. Iran Severely Damaged US Air Ops Center in Qatar Soon After War Began

**原文标题**: Iran Severely Damaged US Air Ops Center in Qatar Soon After War Began

**原文链接**: [https://www.airandspaceforces.com/us-air-operations-center-qatar-severely-damaged-iran/](https://www.airandspaceforces.com/us-air-operations-center-qatar-severely-damaged-iran/)

生成摘要时出错

---

## 88. Vim Classic 8.3 Released

**原文标题**: Vim Classic 8.3 Released

**原文链接**: [https://vim-classic.org/news/vim-8.3-released.html](https://vim-classic.org/news/vim-8.3-released.html)

生成摘要时出错

---

## 89. The Russian who invented semiconductors 25 years before the USA

**原文标题**: The Russian who invented semiconductors 25 years before the USA

**原文链接**: [https://www.semidoped.com/p/til-the-man-who-invented-the-future](https://www.semidoped.com/p/til-the-man-who-invented-the-future)

生成摘要时出错

---

## 90. Efficient and Training-Free Single-Image Diffusion Models

**原文标题**: Efficient and Training-Free Single-Image Diffusion Models

**原文链接**: [https://arxiv.org/abs/2606.04299](https://arxiv.org/abs/2606.04299)

生成摘要时出错

---

## 91. SDSU Wired Its Dorms with 1,300 AI Cameras Without Telling Students

**原文标题**: SDSU Wired Its Dorms with 1,300 AI Cameras Without Telling Students

**原文链接**: [https://reclaimthenet.org/sdsu-adds-1300-ai-cameras-330-in-student-dorms](https://reclaimthenet.org/sdsu-adds-1300-ai-cameras-330-in-student-dorms)

生成摘要时出错

---

## 92. The best relationships are all-encompassing.

**原文标题**: The best relationships are all-encompassing.

**原文链接**: [https://andys.blog/the-best-relationships/](https://andys.blog/the-best-relationships/)

生成摘要时出错

---

## 93. Do agents.md files help coding agents?

**原文标题**: Do agents.md files help coding agents?

**原文链接**: [https://twitter.com/rasbt/status/2063649136323252397](https://twitter.com/rasbt/status/2063649136323252397)

生成摘要时出错

---

## 94. The curious case of low-protein diets

**原文标题**: The curious case of low-protein diets

**原文链接**: [https://knowablemagazine.org/content/article/living-world/2026/low-protein-diet-animals-live-longer](https://knowablemagazine.org/content/article/living-world/2026/low-protein-diet-animals-live-longer)

生成摘要时出错

---

## 95. Human-Like Neural Nets by Catapulting

**原文标题**: Human-Like Neural Nets by Catapulting

**原文链接**: [https://gwern.net/llm-catapult](https://gwern.net/llm-catapult)

生成摘要时出错

---

## 96. New Referendum Would Flip Brexit Result 10 Years On, Poll Finds

**原文标题**: New Referendum Would Flip Brexit Result 10 Years On, Poll Finds

**原文链接**: [https://www.bloomberg.com/news/articles/2026-06-08/new-referendum-would-flip-brexit-result-10-years-on-poll-finds](https://www.bloomberg.com/news/articles/2026-06-08/new-referendum-would-flip-brexit-result-10-years-on-poll-finds)

生成摘要时出错

---

## 97. SoulsOnly.tff – A font for humans not AI and keyboard firmware to type in it

**原文标题**: SoulsOnly.tff – A font for humans not AI and keyboard firmware to type in it

**原文链接**: [https://github.com/convictional/souls-only](https://github.com/convictional/souls-only)

生成摘要时出错

---

## 98. I am giving up on VM Gaming

**原文标题**: I am giving up on VM Gaming

**原文链接**: [https://deployonfri.day/posts/i-am-giving-up-on-vm-gaming](https://deployonfri.day/posts/i-am-giving-up-on-vm-gaming)

生成摘要时出错

---

## 99. Elfeed 4.0 (Emacs)

**原文标题**: Elfeed 4.0 (Emacs)

**原文链接**: [https://github.com/emacs-elfeed/elfeed/blob/main/NEWS.org](https://github.com/emacs-elfeed/elfeed/blob/main/NEWS.org)

生成摘要时出错

---

## 100. The complete IPv4 address space, mapped

**原文标题**: The complete IPv4 address space, mapped

**原文链接**: [https://worldip.io/](https://worldip.io/)

生成摘要时出错

---

