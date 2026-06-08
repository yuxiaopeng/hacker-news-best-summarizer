# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-06-08.md)

*最后自动更新时间: 2026-06-08 21:37:11*
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

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 2 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 3 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 4 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 5 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 6 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 7 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 8 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 9 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 10 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 11 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 12 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 13 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 14 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 15 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 16 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 17 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 18 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 19 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 20 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 21 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 22 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 23 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 24 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 25 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 26 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 27 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 28 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 29 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 30 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 31 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 32 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 33 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 34 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 35 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 36 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 37 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 38 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 39 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 40 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 41 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 42 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 43 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 44 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 45 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 46 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 47 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 48 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 49 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 50 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 51 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 52 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 53 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 54 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 55 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 56 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 57 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 58 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 59 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 60 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 61 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 62 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 63 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 64 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 65 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 66 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 67 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 68 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 69 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 70 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 71 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 72 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 73 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 74 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 75 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 76 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 77 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 78 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 79 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 80 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 81 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 82 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 83 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 84 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 85 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 86 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 87 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 88 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 89 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 90 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 91 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 92 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 93 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 94 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 95 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 96 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 97 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 98 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 99 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 100 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 101 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 102 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 103 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 104 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 105 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 106 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 107 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 108 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 109 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 110 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 111 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 112 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 113 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 114 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 115 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 116 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 117 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 118 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 119 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 120 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 121 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 122 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 123 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 124 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 125 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 126 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 127 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 128 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 129 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 130 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 131 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 132 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 133 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 134 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 135 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 136 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 137 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 138 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 139 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 140 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 141 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 142 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 143 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 144 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 145 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 146 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 147 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 148 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 149 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 150 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 151 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 152 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 153 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 154 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 155 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 156 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 157 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 158 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 159 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 160 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 161 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 162 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 163 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 164 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 165 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 166 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 167 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 168 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 169 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 170 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 171 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 172 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 173 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 174 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 175 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 176 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 177 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 178 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 179 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 180 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 181 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 182 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 183 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 184 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 185 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 186 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 187 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 188 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 189 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 190 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 191 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 192 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 193 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 194 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 195 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 196 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 197 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 198 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 199 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 200 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 201 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 202 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 203 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 204 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 205 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 206 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 207 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 208 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 209 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 210 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 211 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 212 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 213 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
