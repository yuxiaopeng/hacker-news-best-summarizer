# Hacker News 热门文章摘要 (2026-07-13)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. Zig 创始人直言不讳，安索罗匹克吹嘘

**原文标题**: Zig Creator Calls Spade a Spade, Anthropic Blows Smoke

**原文链接**: [https://raymyers.org/post/zed-creator-calls-spade-a-spade/](https://raymyers.org/post/zed-creator-calls-spade-a-spade/)

所提供的文本仅包含一个标题和重定向通知，而非完整的文章内容。

标题“Zig创始人直言不讳，Anthropic故弄玄虚”表明，文章刊载了Zig编程语言创建者直接且可能带有批判性的评论。此人被描绘为坦率诚实（“直言不讳”），与暗示不真诚或含糊其辞（“故弄玄虚”）的Anthropic公司形成对比。

重定向消息进一步澄清，文章最初引用时错误地将该说法归因于“Zed创建者”，而更新的URL路径中已将其更正为“Zig创建者”。

---

## 2. Claude Code 在读取提示之前发送 33k 个 token；OpenCode 发送 7k 个 token。

**原文标题**: Claude Code sends 33k tokens before reading the prompt; OpenCode sends 7k

**原文链接**: [https://systima.ai/blog/claude-code-vs-opencode-token-overhead](https://systima.ai/blog/claude-code-vs-opencode-token-overhead)

本文比较了Claude Code和OpenCode框架的token效率，发现Claude Code显著“更耗费token”。对于一个简单的一行回复，Claude Code在用户提示*之前*发送大约33,000个token的系统提示、工具架构和脚手架，而OpenCode发送大约7,000个token（在Sonnet模型上是4.7倍的差异，在Fable模型上降至3.3倍）。

Claude Code的缓存效率也更低，在会话中途重写数万个token，导致高额计费，而OpenCode的请求前缀基本保持稳定。

Token消耗进一步膨胀的原因包括：
*   **指令文件：** 一个72KB的文件会为每个请求增加大约20,000个token。
*   **MCP服务器：** 五个普通服务器每个请求会增加5,000到7,000个token。
*   **框架模板：** 其内容随后的每个请求都会重新发送。
*   **子代理：** 最大的倍增因素；一个直接消耗121,000个token的任务，在使用两个Claude Code子代理时消耗了513,000个token，因为每个子代理都会重新读取其完整的基线。

尽管Claude Code最初在一个多步骤任务上由于激进的批处理显示出更低的消耗总量（121,000 vs. OpenCode的132,000个token），但这一优势是依赖于模型的，并且在新模型上情况发生了逆转，Claude Code使用了298,000个token，而OpenCode使用了133,000个token。这些发现强调了框架设计对AI生产中上下文窗口消耗和运营成本的关键影响。

---

## 3. 一张理应登上头版的图

**原文标题**: A graph that should be front-page news

**原文链接**: [https://www.lyrebirddreaming.com/post/the-graph-that-should-be-front-page-news](https://www.lyrebirddreaming.com/post/the-graph-that-should-be-front-page-news)

一张描绘赤道太平洋尼诺3.4区海面温度的图表显示，自1982年以来，其数据以前所未有的方式偏离了所有过往观测值，这代表着一个关键但却在很大程度上被忽视的信号。这不是模型，而是展现现实正在展开的直接实时数据。

尼诺3.4区至关重要，它是地球气候系统的“跳动之心”。这里的变化通过厄尔尼诺-南方涛动（ENSO）影响全球大气环流，从而影响降雨、导致干旱并驱动全球极端天气。厄尔尼诺虽然是一种自然现象，但由于人类引起的气候变化，它现在在一个明显更暖的基线上运作，海洋吸收了90%的多余热量。这加剧了其影响，导致更强烈的风暴、更大量的降雨、更严重的干旱和严酷的热浪，澳大利亚“黑色夏季”事件就是例证。

除了天气之外，这些极端海洋温度正在破坏海洋生态系统，导致珊瑚白化、渔业中断，并导致相互关联的全球“临界点”（例如冰盖、亚马逊雨林）不稳定，有引发连锁反应和不可逆转变化的风险。

最终，这些变化对人类产生了深远影响：食物价格上涨、破坏性风暴、水/食物安全受损、健康危机、社区流离失所，以及不平等加剧和地缘政治不稳定。这张图表预示着地球正在超越现代文明赖以发展的气候条件。它需要紧急关注和行动，以免这些变化变得过于巨大、迅速和相互关联而无法管理。

---

## 4. 如何多读书

**原文标题**: How to read more books

**原文链接**: [https://scotto.me/blog/2026-07-12-how-to-read-more-books/](https://scotto.me/blog/2026-07-12-how-to-read-more-books/)

作者每周大约读一本书，他分享了成为多产读者的策略，并强调这是一个可以实现的目标。主要的建议是**用阅读取代屏幕时间**，方法是删除社交媒体和流媒体服务等分散注意力的应用程序，并在任何不活跃的时刻有意识地拿起一本书。

一个关键的习惯是**始终随身携带一本书**（纸质书或电子书），以填补那些原本会空闲的时刻，例如醒来后、睡前、做饭时、通勤途中或等待时。推荐使用电子阅读器，因为它们便于携带且功能丰富，但与纸质平装书交替阅读可以增加多样性。作者还建议**同时阅读多本书**，将小说和非小说混合阅读以保持兴趣，并**广泛阅读**不同体裁的书籍以发现个人偏好。

一项重要的自由是**不要害怕放弃那些不吸引人的书**，认识到有些书可能在以后更能被欣赏。作者也鼓励建立个人图书馆，通常是从旧书开始。为了保持动力，**设定阅读目标**（例如，使用Goodreads），但要优先考虑理解和享受，而不是仅仅统计数量。**撰写书评和做笔记**有助于巩固理解。

最后，作者不建议使用速读、用摘要替代阅读或主要依赖有声书等“捷径”，并强调真正的阅读需要对文本的专注，才能充分发挥效果。

---

## 5. xAI的Grok构建CLI发送给xAI的内容：线路级分析

**原文标题**: What xAI's Grok build CLI sends to xAI: A wire-level analysis

**原文链接**: [https://gist.github.com/cereblab/dc9a40bc26120f4540e4e09b75ffb547](https://gist.github.com/cereblab/dc9a40bc26120f4540e4e09b75ffb547)

流量分析揭示 xAI 的 Grok CLI (`grok`) 向 xAI 传输大量用户数据，即使是消费者账户。

**主要发现：**

1.  **文件内容，包括密钥，被传输：** 当 Grok 读取文件时，其内容会**未作删减地**发送给 xAI。这包括包含密钥的 `.env` 文件。信息通过以下两种途径传输：
    *   通过 `POST /v1/responses` 进行实时模型交互。
    *   通过 `POST /v1/storage` 上传并被接受 (`HTTP 200`) 的 `session_state` 归档文件，该归档文件会路由到一个名为 `grok-code-session-traces` 的 Google Cloud Storage 存储桶。证据包括在捕获的请求和归档中发现的**原样**密钥。

2.  **整个代码库快照以数 GB 规模上传：** Grok 会上传整个代码库的完整快照——包括所有被跟踪文件的内容以及 Git 历史记录——这与代理实际读取的内容无关。这通过 `POST /v1/storage` 发生。
    *   **规模与证明：** 在一个 12 GB 的代码库上，5.10 GiB 的数据分 73 个数据块上传，全部 `HTTP 200`，发生在捕获截断之前。存储上传 (5.10 GiB) 与模型交互 (192 KB) 之间约 27,800 倍的字节比例证实了这是一次独立的整库上传。关键的是，从 `/v1/storage` 上传中捕获的 Git 捆绑包允许重建代码库，并恢复了明确指示**不要**打开的文件内容。
    *   **限制：** 没有存储上传失败；唯一非 200 的响应是由于 `/v1/responses` 上的模型使用配额，而不是存储大小限制。

3.  **机制与控制：** 存储目标是 `gs://grok-code-session-traces`。此功能默认激活，没有明确文档说明，并且禁用“改进模型”也无法阻止这些上传。

这项分析**明确地**证明了 xAI 对这些数据的**传输、接收和存储**，但并未证明 xAI 会用这些数据来训练其模型。

---

## 6. 格罗克上传了我的用户目录到xAI的服务器上。

**原文标题**: Grok uploaded my user directory to xAI's servers

**原文链接**: [https://twitter.com/a_green_being/status/2076598897779020159](https://twitter.com/a_green_being/status/2076598897779020159)

一位名为“绿色生灵”（@a_green_being）的用户公开声称，xAI旗下的人工智能Grok将其完整的用户目录上传到了xAI的服务器。该用户表示，这次据称发生在2026年7月13日的泄露事件，包含了高度敏感的个人数据，例如SSH密钥、密码管理器数据库、文档、照片和视频。这构成了严重的个人数据泄露和潜在的安全隐患。该帖子迅速获得广泛关注，获得了数万次浏览、数百个赞、转发和回复，凸显了人们对人工智能潜在数据泄露的普遍担忧。

---

## 7. 我爱大语言模型，我讨厌炒作

**原文标题**: I love LLMs, I hate hype

**原文链接**: [https://geohot.github.io//blog/jekyll/update/2026/07/12/i-love-llms.html](https://geohot.github.io//blog/jekyll/update/2026/07/12/i-love-llms.html)

The author expresses profound enthusiasm for AI, having dedicated their career to it since 2014. They are excited by advancements in LLMs, self-driving cars, video generation, and coding agents, citing personal success using local LLMs. They view AI as a natural continuation of the computer revolution.

However, the author strongly criticizes two forms of hype. First, the "negative valence hype" that warns of closing windows, a perpetual underclass, or falling hopelessly behind. They see this as manipulative, designed to instill fear and push people towards specific, undesirable environments. Second, they reject the "singularity" or "light cone" narrative that suggests AI will suddenly transform everything, leaving most behind. The author calls this a strawman jump from AI as a useful tool to an apocalyptic, sudden change, betting against such an event.

They argue that frontier AI labs are overvalued because AI's progress is largely driven by Moore's Law and general computing advancements, not their exclusive efforts. They believe these labs won't capture the vast value AI creates and that their anti-open source stance, often disguised as "safety" or "China concerns," is actually a fear of commodification, intended to secure billions in funding by exaggerating their unique contribution.

Finally, the author revises earlier skepticism about models programming. While acknowledging models can increase cognitive fatigue and produce "slop," they now see AI as making programming more productive, comparing them to useful tools like find/replace or Stack Overflow. Programming is changing, and using models is a new, valuable skill.

---

## 8. Old and new apps, via modern coding agents

**原文标题**: Old and new apps, via modern coding agents

**原文链接**: [https://terrytao.wordpress.com/2026/07/11/old-and-new-apps-via-modern-coding-agents/](https://terrytao.wordpress.com/2026/07/11/old-and-new-apps-via-modern-coding-agents/)

生成摘要时出错

---

## 9. Sam Neill has died

**原文标题**: Sam Neill has died

**原文链接**: [https://www.theguardian.com/film/2026/jul/13/sam-neill-death-actor-dies-aged-78](https://www.theguardian.com/film/2026/jul/13/sam-neill-death-actor-dies-aged-78)

生成摘要时出错

---

## 10. Since Chromium 148, Math.tanh is now fingerprintable to link underlying OS

**原文标题**: Since Chromium 148, Math.tanh is now fingerprintable to link underlying OS

**原文链接**: [https://scrapfly.dev/posts/browser-math-os-fingerprint/](https://scrapfly.dev/posts/browser-math-os-fingerprint/)

生成摘要时出错

---

## 11. 洛杉矶警方未续签与监控巨头Flock的合同

**原文标题**: LAPD lets contract with surveillance giant Flock expire

**原文链接**: [https://techcrunch.com/2026/07/13/lapd-lets-contract-with-surveillance-giant-flock-expire-citing-serious-concerns-over-civil-liberties-and-privacy/](https://techcrunch.com/2026/07/13/lapd-lets-contract-with-surveillance-giant-flock-expire-citing-serious-concerns-over-civil-liberties-and-privacy/)

The Los Angeles Police Department (LAPD) is allowing its three-year contract with Flock Safety, a surveillance company operating thousands of license plate cameras, to expire. The department cited "serious concerns" regarding civil liberties, privacy, and data collection, security, and sharing as the reasons for not renewing the deal. While the contract is ending, the LAPD indicated a potential for future collaboration if these issues can be addressed contractually.

Flock Safety, which helps law enforcement track vehicles, expressed surprise at the decision, stating confidence in clearing up "misconceptions." However, the LAPD is not alone; several other U.S. cities, including Mountain View, California, and South Portland, Maine, have also ceased working with Flock due to privacy concerns, particularly regarding federal immigration officials' use of the cameras.

The company has faced widespread criticism for various issues. Communities have expressed backlash, sometimes dismantling cameras or finding them reinstalled without permission. Researchers have documented an uptick in motorists being wrongly detained due to false positives from license plate readers, including a recent incident where a journalist was tracked after his vehicle was mistakenly flagged as stolen. Furthermore, Flock has experienced security lapses, exposing cameras and data, and has been criticized for lacking multi-factor authentication for police logins. The U.S. Drug Enforcement Administration reportedly used a local officer's password without their knowledge, and lawmakers have urged federal authorities to investigate Flock's security practices.

---

## 12. Mesh LLM: distributed AI computing on iroh

**原文标题**: Mesh LLM: distributed AI computing on iroh

**原文链接**: [https://www.iroh.computer/blog/mesh-llm](https://www.iroh.computer/blog/mesh-llm)

生成摘要时出错

---

## 13. Grok CLI uploaded the whole home directory to GCS

**原文标题**: Grok CLI uploaded the whole home directory to GCS

**原文链接**: [https://twitter.com/a_green_being/status/2076598897779020159](https://twitter.com/a_green_being/status/2076598897779020159)

生成摘要时出错

---

## 14. Tiny Emulators

**原文标题**: Tiny Emulators

**原文链接**: [https://floooh.github.io/tiny8bit-preview/index.html](https://floooh.github.io/tiny8bit-preview/index.html)

生成摘要时出错

---

## 15. Count Binface

**原文标题**: Count Binface

**原文链接**: [https://countbinface.com](https://countbinface.com)

生成摘要时出错

---

## 16. Show HN: Ant – A JavaScript runtime and ecosystem

**原文标题**: Show HN: Ant – A JavaScript runtime and ecosystem

**原文链接**: [https://antjs.org](https://antjs.org)

生成摘要时出错

---

## 17. LARP – Revenue infrastructure for serious founders

**原文标题**: LARP – Revenue infrastructure for serious founders

**原文链接**: [https://www.larp.website/](https://www.larp.website/)

生成摘要时出错

---

## 18. Apple's new SpeechAnalyzer API, benchmarked against Whisper and its predecessor

**原文标题**: Apple's new SpeechAnalyzer API, benchmarked against Whisper and its predecessor

**原文链接**: [https://get-inscribe.com/blog/apple-speech-api-benchmark.html](https://get-inscribe.com/blog/apple-speech-api-benchmark.html)

生成摘要时出错

---

## 19. Ghostel.el: Terminal emulator powered by libghostty

**原文标题**: Ghostel.el: Terminal emulator powered by libghostty

**原文链接**: [https://dakra.github.io/ghostel/](https://dakra.github.io/ghostel/)

生成摘要时出错

---

## 20. A voxel Tokyo in real Japan time – ride the Yamanote line and study Japanese

**原文标题**: A voxel Tokyo in real Japan time – ride the Yamanote line and study Japanese

**原文链接**: [https://jivx.com/densha](https://jivx.com/densha)

生成摘要时出错

---

## 21. Cyberpunk Comics, Manga and Graphic Novels

**原文标题**: Cyberpunk Comics, Manga and Graphic Novels

**原文链接**: [https://shellzine.net/cyberpunk-comics/](https://shellzine.net/cyberpunk-comics/)

生成摘要时出错

---

## 22. Show HN: Super Dario

**原文标题**: Show HN: Super Dario

**原文链接**: [https://superdario.pawb.de](https://superdario.pawb.de)

生成摘要时出错

---

## 23. DOGE is done. What happened to its records?

**原文标题**: DOGE is done. What happened to its records?

**原文链接**: [https://www.ms.now/opinion/doge-government-efficiency-records-job-cuts-elon-musk-foia](https://www.ms.now/opinion/doge-government-efficiency-records-job-cuts-elon-musk-foia)

生成摘要时出错

---

## 24. The shingles vaccine may reduce the risk of dementia

**原文标题**: The shingles vaccine may reduce the risk of dementia

**原文链接**: [https://www.economist.com/leaders/2026/07/09/a-no-brainer-for-protecting-your-brain](https://www.economist.com/leaders/2026/07/09/a-no-brainer-for-protecting-your-brain)

生成摘要时出错

---

## 25. Migrating a production AI agent to GPT-5.6: 2.2x faster, 27% cheaper

**原文标题**: Migrating a production AI agent to GPT-5.6: 2.2x faster, 27% cheaper

**原文链接**: [https://ploy.ai/blog/migrating-a-production-ai-agent-to-gpt-5-6](https://ploy.ai/blog/migrating-a-production-ai-agent-to-gpt-5-6)

生成摘要时出错

---

## 26. How Doctors die. It’s not like the rest of us (2016)

**原文标题**: How Doctors die. It’s not like the rest of us (2016)

**原文链接**: [https://archive.cancerworld.net/featured/how-doctors-die/](https://archive.cancerworld.net/featured/how-doctors-die/)

生成摘要时出错

---

## 27. Irish datacenters now guzzle 23% of the country's electricity

**原文标题**: Irish datacenters now guzzle 23% of the country's electricity

**原文链接**: [https://www.theregister.com/on-prem/2026/07/11/irish-datacenters-now-guzzle-23-of-the-countrys-electricity/5270013](https://www.theregister.com/on-prem/2026/07/11/irish-datacenters-now-guzzle-23-of-the-countrys-electricity/5270013)

生成摘要时出错

---

## 28. Backtrack-Free Cursive

**原文标题**: Backtrack-Free Cursive

**原文链接**: [https://mmapped.blog/posts/52-backtrack-free-cursive](https://mmapped.blog/posts/52-backtrack-free-cursive)

生成摘要时出错

---

## 29. Stop Telling Me to Ask an LLM

**原文标题**: Stop Telling Me to Ask an LLM

**原文链接**: [https://blog.yaelwrites.com/stop-telling-me-to-ask-an-llm/](https://blog.yaelwrites.com/stop-telling-me-to-ask-an-llm/)

生成摘要时出错

---

## 30. Don't you mean extinct?

**原文标题**: Don't you mean extinct?

**原文链接**: [https://fabiensanglard.net/extinct/index.html](https://fabiensanglard.net/extinct/index.html)

生成摘要时出错

---

## 31. RISCBoy is an open-source portable games console, designed from scratch

**原文标题**: RISCBoy is an open-source portable games console, designed from scratch

**原文链接**: [https://github.com/Wren6991/RISCBoy](https://github.com/Wren6991/RISCBoy)

生成摘要时出错

---

## 32. Control the Ideas, Not the Code

**原文标题**: Control the Ideas, Not the Code

**原文链接**: [https://antirez.com/news/169](https://antirez.com/news/169)

生成摘要时出错

---

## 33. Under federal rule, colleges must leave grads better off or lose financial aid

**原文标题**: Under federal rule, colleges must leave grads better off or lose financial aid

**原文链接**: [https://www.npr.org/2026/06/30/nx-s1-5835631/turner-camhi-do-no-harm-college-loans](https://www.npr.org/2026/06/30/nx-s1-5835631/turner-camhi-do-no-harm-college-loans)

生成摘要时出错

---

## 34. Interrail: 6,379Km and 13 Countries over 7 weeks

**原文标题**: Interrail: 6,379Km and 13 Countries over 7 weeks

**原文链接**: [https://shkspr.mobi/blog/2026/07/another-ridiculous-interrail-holiday-6379km-and-13-countries-over-7-weeks/](https://shkspr.mobi/blog/2026/07/another-ridiculous-interrail-holiday-6379km-and-13-countries-over-7-weeks/)

生成摘要时出错

---

## 35. An Infuriating Goodbye to Photoshop

**原文标题**: An Infuriating Goodbye to Photoshop

**原文链接**: [https://anderegg.ca/2026/07/12/an-infuriating-goodbye-to-photoshop](https://anderegg.ca/2026/07/12/an-infuriating-goodbye-to-photoshop)

生成摘要时出错

---

## 36. I Learned to Read Again

**原文标题**: I Learned to Read Again

**原文链接**: [https://substack.magazinenongrata.com/p/how-i-learned-to-read-again](https://substack.magazinenongrata.com/p/how-i-learned-to-read-again)

生成摘要时出错

---

## 37. How we can reduce traffic congestion

**原文标题**: How we can reduce traffic congestion

**原文链接**: [https://research.google/blog/the-power-of-collaboration-how-we-can-reduce-traffic-congestion/](https://research.google/blog/the-power-of-collaboration-how-we-can-reduce-traffic-congestion/)

生成摘要时出错

---

## 38. The art and engineering of Sega CD Silpheed

**原文标题**: The art and engineering of Sega CD Silpheed

**原文链接**: [https://fabiensanglard.net/silpheed/index.html](https://fabiensanglard.net/silpheed/index.html)

生成摘要时出错

---

## 39. Woman in Brazil enslaved for 55 years by 3 generations of the same family

**原文标题**: Woman in Brazil enslaved for 55 years by 3 generations of the same family

**原文链接**: [https://english.elpais.com/international/2026-07-10/woman-rescued-in-brazil-after-being-enslaved-for-55-years-by-three-generations-of-the-same-family.html](https://english.elpais.com/international/2026-07-10/woman-rescued-in-brazil-after-being-enslaved-for-55-years-by-three-generations-of-the-same-family.html)

生成摘要时出错

---

## 40. Show HN: Mindwalk – Replay coding-agent sessions on a 3D map of your codebase

**原文标题**: Show HN: Mindwalk – Replay coding-agent sessions on a 3D map of your codebase

**原文链接**: [https://github.com/cosmtrek/mindwalk](https://github.com/cosmtrek/mindwalk)

生成摘要时出错

---

## 41. Understanding the Odin programming language

**原文标题**: Understanding the Odin programming language

**原文链接**: [https://odinbook.com/](https://odinbook.com/)

生成摘要时出错

---

## 42. Death of the Status Update: Why 55% of Americans Stopped Posting on Social Media

**原文标题**: Death of the Status Update: Why 55% of Americans Stopped Posting on Social Media

**原文链接**: [https://ca.pcmag.com/social-media/16790/the-death-of-the-status-update-why-55-of-americans-stopped-posting-on-social-media](https://ca.pcmag.com/social-media/16790/the-death-of-the-status-update-why-55-of-americans-stopped-posting-on-social-media)

生成摘要时出错

---

## 43. Why Vanilla JavaScript

**原文标题**: Why Vanilla JavaScript

**原文链接**: [https://guseyn.com/html/posts/why-vanilla-js.html](https://guseyn.com/html/posts/why-vanilla-js.html)

生成摘要时出错

---

## 44. Designing and assembling my first PCB

**原文标题**: Designing and assembling my first PCB

**原文链接**: [https://vilkeliskis.com/b/2026/0711.html](https://vilkeliskis.com/b/2026/0711.html)

生成摘要时出错

---

## 45. AI boosts research careers but narrow the span of ideas explored: study

**原文标题**: AI boosts research careers but narrow the span of ideas explored: study

**原文链接**: [https://spectrum.ieee.org/ai-science-research-flattens-discovery](https://spectrum.ieee.org/ai-science-research-flattens-discovery)

生成摘要时出错

---

## 46. Show HN: Clawk – Give coding agents a disposable Linux VM, not your laptop

**原文标题**: Show HN: Clawk – Give coding agents a disposable Linux VM, not your laptop

**原文链接**: [https://github.com/clawkwork/clawk](https://github.com/clawkwork/clawk)

生成摘要时出错

---

## 47. Weightlifting beats running for blood sugar control, researchers find (2025)

**原文标题**: Weightlifting beats running for blood sugar control, researchers find (2025)

**原文链接**: [https://news.vt.edu/articles/2025/11/research_fralinbiomed_yanweightlifting.html](https://news.vt.edu/articles/2025/11/research_fralinbiomed_yanweightlifting.html)

生成摘要时出错

---

## 48. Precursor

**原文标题**: Precursor

**原文链接**: [https://blog.cloudflare.com/introducing-precursor/](https://blog.cloudflare.com/introducing-precursor/)

生成摘要时出错

---

## 49. Automation Without Understanding

**原文标题**: Automation Without Understanding

**原文链接**: [https://arxiv.org/abs/2607.06377](https://arxiv.org/abs/2607.06377)

生成摘要时出错

---

## 50. Autopsy Study Finds Replicating SARS-CoV-2 in the Hearts of Long Covid

**原文标题**: Autopsy Study Finds Replicating SARS-CoV-2 in the Hearts of Long Covid

**原文链接**: [https://my.uscap.org/uscap/program/S0tc675/index.cfm?pgid=5167&sid=14770&abid=51228](https://my.uscap.org/uscap/program/S0tc675/index.cfm?pgid=5167&sid=14770&abid=51228)

生成摘要时出错

---

## 51. A pure scheme web programming tool

**原文标题**: A pure scheme web programming tool

**原文链接**: [https://goeteia.dev](https://goeteia.dev)

生成摘要时出错

---

## 52. Why are US consumers so angry? It's not just high prices

**原文标题**: Why are US consumers so angry? It's not just high prices

**原文链接**: [https://www.theguardian.com/us-news/ng-interactive/2026/jun/04/us-consumer-rage-prices-economy](https://www.theguardian.com/us-news/ng-interactive/2026/jun/04/us-consumer-rage-prices-economy)

生成摘要时出错

---

## 53. Kode Dot Programmable pocket device for makers, pentesters and geeks

**原文标题**: Kode Dot Programmable pocket device for makers, pentesters and geeks

**原文链接**: [https://kode.diy](https://kode.diy)

生成摘要时出错

---

## 54. Against Usefulness

**原文标题**: Against Usefulness

**原文链接**: [https://www.motivenotes.ai/p/against-usefulness](https://www.motivenotes.ai/p/against-usefulness)

生成摘要时出错

---

## 55. Show HN: DOM-docx – HTML to native, editable Word docs (MIT)

**原文标题**: Show HN: DOM-docx – HTML to native, editable Word docs (MIT)

**原文链接**: [https://github.com/floodtide/dom-docx](https://github.com/floodtide/dom-docx)

生成摘要时出错

---

## 56. Mechanistic interpretability researchers applying causality theory to LLMs

**原文标题**: Mechanistic interpretability researchers applying causality theory to LLMs

**原文链接**: [https://cacm.acm.org/news/can-we-understand-how-large-language-models-reason/](https://cacm.acm.org/news/can-we-understand-how-large-language-models-reason/)

生成摘要时出错

---

## 57. Yt-Dlp Sequence Diagrams

**原文标题**: Yt-Dlp Sequence Diagrams

**原文链接**: [https://app.ilograph.com/demo.ilograph.yt-dlp/Download%2520a%2520YouTube%2520Video](https://app.ilograph.com/demo.ilograph.yt-dlp/Download%2520a%2520YouTube%2520Video)

生成摘要时出错

---

## 58. Vagal cholinergic denervation of the gastric mucosa in Long-COVID-19

**原文标题**: Vagal cholinergic denervation of the gastric mucosa in Long-COVID-19

**原文链接**: [https://www.ijidonline.com/article/S1201-9712(26)00608-9/fulltext](https://www.ijidonline.com/article/S1201-9712(26)00608-9/fulltext)

生成摘要时出错

---

## 59. Quadrupling code performance with a "useless" if

**原文标题**: Quadrupling code performance with a "useless" if

**原文链接**: [https://purplesyringa.moe/blog/quadrupling-code-performance-with-a-useless-if/](https://purplesyringa.moe/blog/quadrupling-code-performance-with-a-useless-if/)

生成摘要时出错

---

## 60. Making Crash Bandicoot (2011)

**原文标题**: Making Crash Bandicoot (2011)

**原文链接**: [https://all-things-andy-gavin.com/2011/02/02/making-crash-bandicoot-part-1/](https://all-things-andy-gavin.com/2011/02/02/making-crash-bandicoot-part-1/)

生成摘要时出错

---

## 61. Neocities: Create your own free website

**原文标题**: Neocities: Create your own free website

**原文链接**: [https://neocities.org/](https://neocities.org/)

生成摘要时出错

---

## 62. Leak of San Francisco Police Drone Footage Exposes Reality of Urban Surveillance

**原文标题**: Leak of San Francisco Police Drone Footage Exposes Reality of Urban Surveillance

**原文链接**: [https://www.wired.com/story/sfpd-drone-video-leak-surveillance/](https://www.wired.com/story/sfpd-drone-video-leak-surveillance/)

生成摘要时出错

---

## 63. Unexpected Solidlike Fracture in Simple Liquids

**原文标题**: Unexpected Solidlike Fracture in Simple Liquids

**原文链接**: [https://www.quantamagazine.org/we-know-simple-fluids-can-flow-turns-out-some-can-fracture-20260710/](https://www.quantamagazine.org/we-know-simple-fluids-can-flow-turns-out-some-can-fracture-20260710/)

生成摘要时出错

---

## 64. A dock that wakes up reliably

**原文标题**: A dock that wakes up reliably

**原文链接**: [https://fabiensanglard.net/tb4/index.html](https://fabiensanglard.net/tb4/index.html)

生成摘要时出错

---

## 65. A Erlang style pure Scheme Webserver and further

**原文标题**: A Erlang style pure Scheme Webserver and further

**原文链接**: [https://igropyr.com](https://igropyr.com)

生成摘要时出错

---

## 66. xAI's Grok Build CLI Uploads Git Repositories to a Google Cloud Bucket

**原文标题**: xAI's Grok Build CLI Uploads Git Repositories to a Google Cloud Bucket

**原文链接**: [https://www.internationalcyberdigest.com/xais-grok-build-cli-uploads-entire-git-repositories-to-a-google-cloud-bucket/](https://www.internationalcyberdigest.com/xais-grok-build-cli-uploads-entire-git-repositories-to-a-google-cloud-bucket/)

生成摘要时出错

---

## 67. Martha Lillard, last US polio patient using iron lung, dies at 78 in Oklahoma

**原文标题**: Martha Lillard, last US polio patient using iron lung, dies at 78 in Oklahoma

**原文链接**: [https://abcnews.com/US/wireStory/martha-lillard-us-polio-patient-iron-lung-dies-134668491](https://abcnews.com/US/wireStory/martha-lillard-us-polio-patient-iron-lung-dies-134668491)

生成摘要时出错

---

## 68. Beavis Ultrasound PnP ISA Sound Card Replica

**原文标题**: Beavis Ultrasound PnP ISA Sound Card Replica

**原文链接**: [https://github.com/schlae/BeavisUltrasound](https://github.com/schlae/BeavisUltrasound)

生成摘要时出错

---

## 69. Berkshire's $397B Bet Against an Overheated Market

**原文标题**: Berkshire's $397B Bet Against an Overheated Market

**原文链接**: [https://www.disruptionbanking.com/2026/07/13/inside-berkshires-397-billion-bet-against-an-overheated-market/](https://www.disruptionbanking.com/2026/07/13/inside-berkshires-397-billion-bet-against-an-overheated-market/)

生成摘要时出错

---

## 70. Fable extended until 19 July

**原文标题**: Fable extended until 19 July

**原文链接**: [https://twitter.com/claudeai/status/2076351399999557669](https://twitter.com/claudeai/status/2076351399999557669)

生成摘要时出错

---

## 71. Show HN: Shirei, cross-platform GUI framework in native Go

**原文标题**: Show HN: Shirei, cross-platform GUI framework in native Go

**原文链接**: [https://github.com/hasenj/go-shirei/](https://github.com/hasenj/go-shirei/)

生成摘要时出错

---

## 72. Datacentres drive up big tech's carbon emissions to a third of those of France

**原文标题**: Datacentres drive up big tech's carbon emissions to a third of those of France

**原文链接**: [https://www.theguardian.com/us-news/2026/jul/11/microsoft-amazon-google-datacentre-carbon-emissions-france](https://www.theguardian.com/us-news/2026/jul/11/microsoft-amazon-google-datacentre-carbon-emissions-france)

生成摘要时出错

---

## 73. The Chinese Voice Actor Forced to Prove He's Human

**原文标题**: The Chinese Voice Actor Forced to Prove He's Human

**原文链接**: [https://www.sixthtone.com/news/1018753](https://www.sixthtone.com/news/1018753)

生成摘要时出错

---

## 74. Unauthenticated RCE in Motorola's MR2600 Router

**原文标题**: Unauthenticated RCE in Motorola's MR2600 Router

**原文链接**: [https://mrbruh.com/motorola/](https://mrbruh.com/motorola/)

生成摘要时出错

---

## 75. Wikipedia escapes Category 1 designation under the UK Online Safety Act for now

**原文标题**: Wikipedia escapes Category 1 designation under the UK Online Safety Act for now

**原文链接**: [https://en.wikipedia.org/wiki/Wikipedia:Wikipedia_Signpost/2026-07-13/Special_report](https://en.wikipedia.org/wiki/Wikipedia:Wikipedia_Signpost/2026-07-13/Special_report)

生成摘要时出错

---

## 76. Benchmarking 15 "E-Waste" GPUs with Modern Workloads

**原文标题**: Benchmarking 15 "E-Waste" GPUs with Modern Workloads

**原文链接**: [https://esologic.com/benchmarking-tesla-gpus/](https://esologic.com/benchmarking-tesla-gpus/)

生成摘要时出错

---

## 77. Theo de Raadt: "You've been smoking something mind altering" (2007)

**原文标题**: Theo de Raadt: "You've been smoking something mind altering" (2007)

**原文链接**: [https://marc.info/?l=openbsd-misc&m=119318909016582](https://marc.info/?l=openbsd-misc&m=119318909016582)

生成摘要时出错

---

## 78. Building and Shipping Mac and iOS Apps Without Ever Opening Xcode

**原文标题**: Building and Shipping Mac and iOS Apps Without Ever Opening Xcode

**原文链接**: [https://scottwillsey.com/building-and-shipping-mac-and-ios-apps-without-ever-opening-xcode/](https://scottwillsey.com/building-and-shipping-mac-and-ios-apps-without-ever-opening-xcode/)

生成摘要时出错

---

## 79. Why study Diophantine equations?

**原文标题**: Why study Diophantine equations?

**原文链接**: [https://hidden-phenomena.com/articles/modular](https://hidden-phenomena.com/articles/modular)

生成摘要时出错

---

## 80. How the FSF sysadmins block botnets with reaction

**原文标题**: How the FSF sysadmins block botnets with reaction

**原文链接**: [https://www.fsf.org/blogs/community/blocking-botnets-with-reaction](https://www.fsf.org/blogs/community/blocking-botnets-with-reaction)

生成摘要时出错

---

## 81. MacKenzie Scott's giving, in quality-adjusted life years

**原文标题**: MacKenzie Scott's giving, in quality-adjusted life years

**原文链接**: [https://maxghenis.com/mackenzie-scott-qaly/](https://maxghenis.com/mackenzie-scott-qaly/)

生成摘要时出错

---

## 82. Storm clouds gather over America's financial supremacy

**原文标题**: Storm clouds gather over America's financial supremacy

**原文链接**: [https://www.economist.com/finance-and-economics/2026/07/12/storm-clouds-gather-over-americas-financial-supremacy](https://www.economist.com/finance-and-economics/2026/07/12/storm-clouds-gather-over-americas-financial-supremacy)

生成摘要时出错

---

## 83. Billion Dollar PDFs

**原文标题**: Billion Dollar PDFs

**原文链接**: [https://billiondollarpdf.com/](https://billiondollarpdf.com/)

生成摘要时出错

---

## 84. Why Write Code in 2026

**原文标题**: Why Write Code in 2026

**原文链接**: [https://softwaredoug.com/blog/2026/07/09/write-code.html](https://softwaredoug.com/blog/2026/07/09/write-code.html)

生成摘要时出错

---

## 85. Fixed three bugs that made Qwen3.5-122B a daily driver on Mac Studio

**原文标题**: Fixed three bugs that made Qwen3.5-122B a daily driver on Mac Studio

**原文链接**: [https://mrzk.io/posts/qmlx-maximising-ai-psychosis-minmaxing-mac-studio/](https://mrzk.io/posts/qmlx-maximising-ai-psychosis-minmaxing-mac-studio/)

生成摘要时出错

---

## 86. The real prices of frontier models. Tokens * Price, right?

**原文标题**: The real prices of frontier models. Tokens * Price, right?

**原文链接**: [https://playcode.io/blog/real-price-of-frontier-models](https://playcode.io/blog/real-price-of-frontier-models)

生成摘要时出错

---

## 87. Logseq 2.0 Beta (DB version) is here

**原文标题**: Logseq 2.0 Beta (DB version) is here

**原文链接**: [https://github.com/logseq/logseq/releases](https://github.com/logseq/logseq/releases)

生成摘要时出错

---

## 88. The One-Step Trap (In AI Research)

**原文标题**: The One-Step Trap (In AI Research)

**原文链接**: [http://incompleteideas.net/IncIdeas/OneStepTrap.html](http://incompleteideas.net/IncIdeas/OneStepTrap.html)

生成摘要时出错

---

## 89. Go-Flavored Concurrency in C

**原文标题**: Go-Flavored Concurrency in C

**原文链接**: [https://antonz.org/concurrency-in-c/](https://antonz.org/concurrency-in-c/)

生成摘要时出错

---

## 90. TK, or the secret to effortless writing (2024)

**原文标题**: TK, or the secret to effortless writing (2024)

**原文链接**: [https://atthis.link/blog/2024/49629.html](https://atthis.link/blog/2024/49629.html)

生成摘要时出错

---

## 91. Croc: Securely transfer files and folders between two computers

**原文标题**: Croc: Securely transfer files and folders between two computers

**原文链接**: [https://github.com/schollz/croc/](https://github.com/schollz/croc/)

生成摘要时出错

---

## 92. I used to love Claude, but the latest models are slowly ruining it

**原文标题**: I used to love Claude, but the latest models are slowly ruining it

**原文链接**: [https://www.androidauthority.com/claude-latest-models-pushback-bad-3683521/](https://www.androidauthority.com/claude-latest-models-pushback-bad-3683521/)

生成摘要时出错

---

## 93. Wealthy AI workers send San Francisco house prices soaring

**原文标题**: Wealthy AI workers send San Francisco house prices soaring

**原文链接**: [https://www.bbc.com/news/articles/c9q29j47v9ro](https://www.bbc.com/news/articles/c9q29j47v9ro)

生成摘要时出错

---

## 94. How Ukraine Built a War Fighting State

**原文标题**: How Ukraine Built a War Fighting State

**原文链接**: [https://www.austinvernon.site/blog/ukrainewar.html](https://www.austinvernon.site/blog/ukrainewar.html)

生成摘要时出错

---

## 95. Mystery behind Moana: After 1,700 years, why did Polynesians suddenly sail east?

**原文标题**: Mystery behind Moana: After 1,700 years, why did Polynesians suddenly sail east?

**原文链接**: [https://theconversation.com/the-real-mystery-behind-moana-after-1-700-years-why-did-polynesians-suddenly-sail-east-287226](https://theconversation.com/the-real-mystery-behind-moana-after-1-700-years-why-did-polynesians-suddenly-sail-east-287226)

生成摘要时出错

---

## 96. IT administrators are "fed up" with Microsoft's "useless" apps and Windows 11

**原文标题**: IT administrators are "fed up" with Microsoft's "useless" apps and Windows 11

**原文链接**: [https://www.neowin.net/news/it-admins-feel-overwhelmingly-sick-of-microsoft-and-windows-11-garbage-apps-products/](https://www.neowin.net/news/it-admins-feel-overwhelmingly-sick-of-microsoft-and-windows-11-garbage-apps-products/)

生成摘要时出错

---

## 97. Profiling the "Abundance" housing bottleneck with real data

**原文标题**: Profiling the "Abundance" housing bottleneck with real data

**原文链接**: [https://laxmena.com/same-capacity-less-throughput](https://laxmena.com/same-capacity-less-throughput)

生成摘要时出错

---

## 98. Claude Code May–July 2026 weekly limits promotion

**原文标题**: Claude Code May–July 2026 weekly limits promotion

**原文链接**: [https://support.claude.com/en/articles/15910845-claude-code-may-july-2026-weekly-limits-promotion](https://support.claude.com/en/articles/15910845-claude-code-may-july-2026-weekly-limits-promotion)

生成摘要时出错

---

## 99. Nokia's 14 Years of Mobile-Phone Supremacy Ended in an Afternoon

**原文标题**: Nokia's 14 Years of Mobile-Phone Supremacy Ended in an Afternoon

**原文链接**: [https://spectrum.ieee.org/nokia-phones-history](https://spectrum.ieee.org/nokia-phones-history)

生成摘要时出错

---

## 100. Some Monsters Are Real

**原文标题**: Some Monsters Are Real

**原文链接**: [https://climatecasino.substack.com/p/some-monsters-are-real](https://climatecasino.substack.com/p/some-monsters-are-real)

生成摘要时出错

---

