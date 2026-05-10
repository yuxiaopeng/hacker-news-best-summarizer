# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-05-10.md)

*最后自动更新时间: 2026-05-10 20:10:06*
## 1. 人们讨厌AI艺术

**原文标题**: People Hate AI Art

**原文链接**: [https://mccue.dev/pages/5-8-26-ai-art](https://mccue.dev/pages/5-8-26-ai-art)

Ethan McCue 坚决主张“人们讨厌AI艺术”，并认为使用AI艺术标志着“较低的社会素养”，会引起普遍的负面反应，例如“啊”或翻白眼。他认为任何没有负面反应的人都是个例外。

根据McCue的说法，“博弈论”的结论很明确：最好的情况是观众不介意AI艺术，但通常情况下，他们会因此看轻你，因为没有人会对那些“提示词的努力”留下深刻印象。

他提出了几个替代方案，所有这些方案都比AI艺术更受欢迎：
1.  **粗糙的Photoshop编辑：** 即使是拙劣的手动编辑也显示出更多的努力，并且更容易被接受。
2.  **涂鸦：** 自己画一些东西，甚至让孩子画，都能显著提升观感。
3.  **委托艺术作品：** 对于专业人士来说，付费委托艺术家创作作品能正面反映其品味，并支持创意社区。
4.  **做一个骗子：** 这种讽刺的替代方案表明，AI艺术仅有助于筛选掉批判性思考者，吸引适合诈骗的轻信之人，并将其标记为“摇钱树”。

总而言之，McCue断言，使用AI艺术会损害个人形象，除非其明确意图是吸引和剥削那些缺乏辨别力的受众。

---

## 2. 将一个 3 GB 的 SQLite 数据库替换为一个 10 MB 的 FST (有限状态转换器) 二进制文件

**原文标题**: Replacing a 3 GB SQLite db with a 10 MB FST (finite state transducer) binary

**原文链接**: [https://til.andrew-quinn.me/posts/replacing-a-3-gb-sqlite-database-with-a-7-mb-fst-finite-state-trandsucer-binary/](https://til.andrew-quinn.me/posts/replacing-a-3-gb-sqlite-database-with-a-7-mb-fst-finite-state-trandsucer-binary/)

作者详细介绍了芬兰语-英语增量搜索词典“Taskusanakirja”（tsk）实现300倍内存缩减的过程。挑战在于如何高效处理粘着语芬兰语中海量的屈折形式，因为其词根可以有多达上百种词尾。

最初，tsk (v1，基于Go语言) 使用Trie树存储词根（约50 MB）。然而，用Trie树扩展到处理4000万至6000万个屈折形式是不可行的。临时解决方案是一个独立的3 GB SQLite数据库，带有屈折形式的全文搜索功能，尽管功能上可行，但这需要大量下载，与设计一个小型、便携的“袖珍词典”的目标相悖。

九个月后，受BurntSushi关于紧凑字符串表示研究的启发，作者重新审视了这个问题，并使用有限状态换能器（FST）在Rust中重写了屈折形式的处理。这一过程将3 GB的SQLite数据库转化为了一个仅10 MB的FST二进制文件。FST被证明特别适合芬兰语，因为它们能够压缩前缀和后缀，而这在粘着语中是高度重复的。

这种优化意味着整个tsk v2应用程序预计约为20 MB，使其显著更小且更易获取。作者反思，从“糟糕的简易方案”（SQLite）开始至关重要，这使得低成本实验成为可能，并最终带来了卓越的FST解决方案，这倡导了迭代解决问题和“重新发明一些轮子”的价值。

---

## 3. 科学家警告大西洋洋流恐将停摆

**原文标题**: Scientists warn Atlantic current at risk of shutting down

**原文链接**: [https://e360.yale.edu/features/amoc-climate-change](https://e360.yale.edu/features/amoc-climate-change)

生成摘要时出错

---

## 4. Let’s Encrypt：因潜在事故暂停签发 — 已解决

**原文标题**: Let’s Encrypt: Stopping Issuance for Potential Incident – Resolved

**原文链接**: [https://letsencrypt.status.io/pages/incident/55957a99e800baa4470002da/69fe2d6698ca07050eb4b1b3](https://letsencrypt.status.io/pages/incident/55957a99e800baa4470002da/69fe2d6698ca07050eb4b1b3)

2026年5月8日，Let's Encrypt因一起潜在事件暂时停止了所有证书签发，并于世界协调时18:37（UTC）启动了关停。

此次事件是由于一张旨在从其“X代”根证书过渡到新的“Y代”根证书的交叉签名证书出现了问题。这个问题特别影响了他们的“tlsserver”和“shortlived”ACME证书配置文件。

截至世界协调时21:03（UTC），Let's Encrypt已解决该问题并恢复了全部签发。解决方案包括将所有签发切换回其现有的“X代”根证书，以绕过交叉签名证书的问题。服务现已恢复正常运行。

---

## 5. Gemini API File Search is now multimodal

**原文标题**: Gemini API File Search is now multimodal

**原文链接**: [https://blog.google/innovation-and-ai/technology/developers-tools/expanded-gemini-api-file-search-multimodal-rag/](https://blog.google/innovation-and-ai/technology/developers-tools/expanded-gemini-api-file-search-multimodal-rag/)

The Gemini API File Search tool has received three significant updates, making it multimodal and enhancing its capabilities for building efficient, verifiable Retrieval-Augmented Generation (RAG) systems. Announced on May 05, 2026, these features help developers structure unstructured data.

Firstly, **multimodal support** enables the tool to process images and text together. Powered by the Gemini Embedding 2 model, it allows applications to search for visual assets based on emotional tone or style described in natural language, not just keywords, giving agents contextual awareness.

Secondly, **custom metadata** allows users to attach key-value labels (e.g., "department: Legal") to data. This enables filtering at query time, significantly reducing irrelevant information, which boosts the speed and accuracy of RAG workflows.

Finally, **page-level citations** introduce greater transparency and trust. When the model provides an answer, it now ties the response directly to the original source by capturing the page number. This granularity allows users to verify information directly, facilitating rigorous fact-checking.

These updates aim to simplify the storage and retrieval of diverse data, allowing developers to focus on product innovation by handling heavy infrastructure.

---

## 6. 任务瘫痪与人工智能

**原文标题**: Task Paralysis and AI

**原文链接**: [https://g5t.de/articles/20260510-task-paralysis-and-ai/index.html](https://g5t.de/articles/20260510-task-paralysis-and-ai/index.html)

作者探讨了他们与“任务麻痹”的斗争，这与“分析麻痹”有所不同。尽管尚未被正式确诊，但作者表现出一些迹象，例如难以完成看似简单的任务、对新鲜事物有强烈需求（每2-3年更换一次职业角色），以及尽管规划成功却无法执行策略，对迈出第一步感到不知所措。

关于人工智能，作者持有喜忧参半的看法。他们承认其负面影响，如工作岗位流失和艺术盗用，并避免将其用于艺术创作。然而，他们发现人工智能对个人使用而言是无价的，尤其是在克服他们的“任务麻痹”方面。人工智能（如Claude）通过快速处理他们想法和策略的实施阶段（尤其是在编码方面）提供帮助，使他们能够专注于构思而非耗时的执行。

“症结”在于人工智能的成瘾潜力。从“想法”到“结果”的快速循环提供了强烈的多巴胺快感，作者称其令人非常满足。这种快速反馈循环产生了更强的渴望，导致在人工智能代币和订阅上过度消费——作者将其比作“瘾君子奔向他们的毒贩”。作者承认自己已陷入这个陷阱，大量投入API积分和更高阶套餐以追逐这种多巴胺刺激。

---

## 7. 日交易额达数十亿美金的生产工程 [视频]

**原文标题**: Production engineering when trading billions of dollars a day [video]

**原文链接**: [https://www.youtube.com/watch?v=zR9PpXWsKFQ](https://www.youtube.com/watch?v=zR9PpXWsKFQ)

所提供的内容，尽管标题名为「每日交易数十亿美元的生产工程 [视频]」，但并未讨论指定主题。

相反，这些文字由一个标准的YouTube页脚区块组成。该区块包含与平台运营和政策相关的链接及信息，例如「关于」、「新闻」、「版权」、「联系我们」、「创作者」、「广告商」、「开发者」、「条款」、「隐私政策与安全」、「YouTube 的运作方式」、「试用新功能」，以及关于「NFL Sunday Ticket© 2026 Google LLC。」的版权声明。

因此，仅基于所提供的文本，无法总结出任何关于生产工程或大宗金融交易的信息。

---

## 8. cPanel的黑色一周：4.4万台服务器遭攻击后，3个新漏洞被修复

**原文标题**: CPanel's Black Week: 3 New Vulnerabilities Patched After Attack on 44k Servers

**原文链接**: [https://www.copahost.com/blog/cpanels-black-week-three-new-vulnerabilities-patched-after-ransomware-attack-on-44000-servers/](https://www.copahost.com/blog/cpanels-black-week-three-new-vulnerabilities-patched-after-ransomware-attack-on-44000-servers/)

生成摘要时出错

---

## 9. Forking the Web

**原文标题**: Forking the Web

**原文链接**: [https://dillo-browser.org/lab/web-fork/](https://dillo-browser.org/lab/web-fork/)

Rodrigo Arias Mallo proposes "Forking the Web" by developing an alternative specification to address the current Web's drawbacks, such as its overwhelming complexity, constant evolution, and vulnerability to standard capture. The initiative focuses on an HTML-like document format with several driving goals.

A core principle is **simplicity**, aiming for a short, byte-limited specification (e.g., 1.44 MiB compressed) to foster diverse client implementations. It mandates **semantic versioning (1.2.3)**, ensuring published standards are immutable and stable, allowing authors to target specific, reliably rendered versions. The specification will employ a **strict, non-ambiguous formal grammar**, meaning non-compliant pages will be rejected by clients. This approach simplifies parsers and encourages authors to use simpler, more forgiving languages like Markdown.

The project prioritizes **text first** as the most versatile information medium, designed to adapt to various screen sizes. Critically, it advocates for **no scripting**, eliminating client-side programming. Instead, interactivity would rely on standardized protocols (like Geo links) that launch native applications, offering optimized, device-specific experiences. The overall objective is to resist standard capture and enable efficient information exchange without requiring complex virtual machines.

---

## 10. Think Linear Algebra (2023)

**原文标题**: Think Linear Algebra (2023)

**原文链接**: [https://allendowney.github.io/ThinkLinearAlgebra/index.html](https://allendowney.github.io/ThinkLinearAlgebra/index.html)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 2 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 3 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 4 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 5 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 6 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 7 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 8 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 9 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 10 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 11 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 12 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 13 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 14 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 15 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 16 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 17 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 18 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 19 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 20 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 21 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 22 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 23 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 24 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 25 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 26 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 27 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 28 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 29 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 30 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 31 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 32 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 33 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 34 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 35 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 36 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 37 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 38 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 39 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 40 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 41 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 42 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 43 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 44 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 45 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 46 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 47 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 48 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 49 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 50 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 51 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 52 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 53 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 54 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 55 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 56 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 57 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 58 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 59 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 60 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 61 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 62 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 63 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 64 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 65 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 66 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 67 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 68 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 69 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 70 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 71 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 72 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 73 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 74 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 75 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 76 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 77 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 78 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 79 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 80 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 81 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 82 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 83 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 84 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 85 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 86 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 87 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 88 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 89 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 90 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 91 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 92 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 93 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 94 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 95 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 96 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 97 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 98 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 99 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 100 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 101 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 102 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 103 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 104 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 105 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 106 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 107 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 108 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 109 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 110 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 111 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 112 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 113 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 114 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 115 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 116 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 117 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 118 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 119 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 120 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 121 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 122 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 123 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 124 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 125 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 126 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 127 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 128 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 129 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 130 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 131 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 132 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 133 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 134 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 135 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 136 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 137 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 138 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 139 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 140 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 141 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 142 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 143 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 144 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 145 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 146 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 147 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 148 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 149 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 150 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 151 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 152 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 153 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 154 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 155 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 156 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 157 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 158 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 159 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 160 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 161 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 162 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 163 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 164 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 165 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 166 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 167 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 168 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 169 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 170 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 171 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 172 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 173 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 174 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 175 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 176 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 177 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 178 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 179 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 180 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 181 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 182 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 183 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 184 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
