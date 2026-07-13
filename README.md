# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-07-13.md)

*最后自动更新时间: 2026-07-13 20:43:49*
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

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 2 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 3 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 4 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 5 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 6 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 7 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 8 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 9 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 10 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 11 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 12 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 13 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 14 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 15 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 16 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 17 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 18 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 19 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 20 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 21 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 22 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 23 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 24 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 25 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 26 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 27 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 28 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 29 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 30 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 31 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 32 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 33 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 34 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 35 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 36 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 37 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 38 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 39 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 40 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 41 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 42 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 43 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 44 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 45 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 46 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 47 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 48 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 49 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 50 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 51 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 52 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 53 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 54 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 55 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 56 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 57 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 58 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 59 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 60 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 61 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 62 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 63 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 64 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 65 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 66 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 67 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 68 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 69 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 70 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 71 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 72 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 73 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 74 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 75 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 76 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 77 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 78 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 79 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 80 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 81 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 82 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 83 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 84 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 85 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 86 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 87 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 88 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 89 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 90 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 91 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 92 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 93 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 94 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 95 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 96 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 97 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 98 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 99 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 100 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 101 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 102 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 103 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 104 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 105 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 106 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 107 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 108 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 109 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 110 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 111 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 112 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 113 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 114 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 115 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 116 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 117 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 118 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 119 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 120 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 121 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 122 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 123 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 124 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 125 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 126 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 127 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 128 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 129 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 130 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 131 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 132 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 133 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 134 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 135 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 136 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 137 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 138 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 139 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 140 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 141 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 142 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 143 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 144 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 145 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 146 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 147 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 148 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 149 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 150 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 151 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 152 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 153 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 154 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 155 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 156 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 157 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 158 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 159 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 160 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 161 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 162 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 163 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 164 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 165 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 166 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 167 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 168 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 169 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 170 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 171 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 172 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 173 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 174 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 175 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 176 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 177 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 178 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 179 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 180 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 181 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 182 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 183 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 184 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 185 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 186 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 187 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 188 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 189 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 190 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 191 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 192 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 193 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 194 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 195 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 196 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 197 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 198 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 199 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 200 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 201 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 202 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 203 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 204 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 205 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 206 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 207 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 208 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 209 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 210 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 211 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 212 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 213 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 214 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 215 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 216 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 217 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 218 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 219 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 220 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 221 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 222 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 223 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 224 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 225 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 226 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 227 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 228 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 229 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 230 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 231 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 232 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 233 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 234 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 235 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 236 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 237 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 238 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 239 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 240 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 241 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 242 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 243 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 244 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 245 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 246 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 247 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 248 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
