# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-09-17.md)

*最后自动更新时间: 2026-09-17 22:34:03*
## 1. 英伟达宣布Rust原生GPU编程

**原文标题**: Nvidia announces native GPU programming in Rust

**原文链接**: [https://developer.nvidia.com/blog/introducing-cuda-rust-two-tracks-for-writing-gpu-kernels/](https://developer.nvidia.com/blog/introducing-cuda-rust-two-tracks-for-writing-gpu-kernels/)

2026年9月，英伟达（Nvidia）宣布致力于在Rust中进行原生GPU编程，旨在到2027年及以后，发展并成熟其CUDA Rust工具链。此举旨在应对Rust在AI系统层日益增长的采用，重视其编译时安全性和性能。

英伟达正在推出两种不同的路径，用于在Rust中编写GPU内核：

1.  **SIMT轨道 (cuda-oxide)：** 该轨道模仿传统的CUDA C++模型，开发人员在此模型中为单个线程指定操作。它使用自定义的`rustc`代码生成后端，通过Pliron IR和LLVM将Rust的`#[kernel]`函数直接编译为PTX。`cuda-oxide`需要固定的每夜版（nightly）Rust工具链和LLVM。内存安全性在编译时通过使用`DisjointSlice`等类型实现独占访问，并使用启动契约（launch contracts）验证内核配置来强制执行。它目前处于早期alpha阶段。

2.  **Tile轨道 (cutile-rs)：** `cutile-rs`是一种更高级的编程模型，它允许开发人员在“tile”（子张量）上执行计算，由编译器管理线程映射和内存布局。它通过CUDA Tile IR即时编译（JIT-compiles）内核。该轨道运行在稳定版Rust (1.89+)和CUDA 13.3上，要求更宽松。内存安全性通过张量分区和所有权来保证，确保每个tile块的独占写入访问。`cutile-rs`进展更顺利，已发布在crates.io上，并已用于HuggingFace的Grout等项目。

这两个项目都优先考虑编译时内存安全性，以防止常见的别名（aliasing）错误。尽管`cuda-oxide`检查启动调用，但`cutile-rs`通过管理跨启动边界的张量提供了更强的保证。英伟达计划支持CUDA Rust、C++和Python之间的跨语言互操作性。尽管这两个项目都处于早期阶段，尚未达到生产就绪状态，但它们标志着向GPU内核开发引入Rust的安全性与性能优势迈出了重要一步。

---

## 2. 欧盟主席为加拿大成为“准成员”敞开大门

**原文标题**: EU chief opens door for Canada to become 'associate member'

**原文链接**: [https://www.bbc.com/news/articles/cjwyzrr9d3dko](https://www.bbc.com/news/articles/cjwyzrr9d3dko)

欧盟委员会主席乌尔苏拉·冯德莱恩公开支持加拿大成为欧盟首个“联系成员国”的提议，旨在技术、国防和经济安全等关键领域建立更紧密的联系。此举很大程度上是由于加拿大与美国关系恶化（包括贸易争端），以及加拿大总理马克·卡尼希望基于共同的民主价值观和全球视角与欧盟建立“独特联盟”的愿望。

美国前总统唐纳德·特朗普对此反应强烈，扬言如果他认为这种结盟是敌对行为，将对欧洲征收“非常严重的关税”。“联系成员国”对欧盟来说是一个新概念，建立这种地位将是一个漫长的过程，尽管乌克兰和西巴尔干地区的一些国家正在走向更紧密的欧盟一体化。

冯德莱恩还在其盟情咨文中提议组建一个欧洲安全理事会，让加拿大、英国和乌克兰等伙伴参与其中，以加强欧洲大陆的安全，尤其考虑到俄罗斯入侵乌克兰以及此前对北约作用的质疑。该理事会可以补充或“侧翼”北约第四条款。其他提议还包括限制儿童使用社交媒体的措施、简化商业官僚程序，以及建立一个管理大规模移民的新应急工具，该计划已引发人权组织的担忧。

---

## 3. 训练一个4B模型，使其生成的查询计划比Postgres快81%。

**原文标题**: Training a 4B model to produce 81% faster query plans than Postgres

**原文链接**: [https://rohanbansal.com/qorl](https://rohanbansal.com/qorl)

本文探讨了查询优化这一长期存在的挑战，特别是连接顺序这一NP难题，它显著影响查询执行速度。文章指出，像Postgres这样的传统优化器在寻找最优计划时常常面临困难，这是因为各种连接顺序、算法（哈希、合并、嵌套循环）和扫描类型（顺序、索引）创造了巨大的搜索空间。这导致了组合爆炸，一个三表查询可能有数千种潜在计划，对于九表连接，则会激增至百亿亿。

作者进行了实验，旨在探究一个小型、开源权重的4B语言模型是否能通过后训练超越Postgres的默认查询计划。结果“响亮地肯定”了这一点，该模型通过监督微调（SFT）和基于智能体的强化学习（RL），在113个包含大量连接的查询中展示了44.7%的延迟降低，考虑到它最初无法为其中99个查询生成计划，这一成就令人印象深刻。

该实验涉及一个专门的Postgres测量设备、一个用于嘈杂环境的定制GRPO变体，以及一个利用vLLM、训练器和多个Postgres容器的强化学习设置，并辅以从GPT-6 Astra智能体轨迹中进行的离策略蒸馏。通过一个IMDb数据集的例子，文章阐明了核心问题的难度，展示了选择性谓词如何显著改变中间结果的基数，从而使得最优连接顺序对性能至关重要。

---

## 4. 编程小技巧

**原文标题**: Small programming tricks

**原文链接**: [https://will-keleher.com/posts/small-programming-tricks-matter/](https://will-keleher.com/posts/small-programming-tricks-matter/)

文章指出，相当一部分工程生产力来自于“知识碎金”——那些无需大量支持性基础设施的高杠杆技巧。这些可以是特定的语言特性、命令行工具或配置，能够让工作变得稍微轻松一些。

例如，使用`fzf`或`atuin`增强终端历史搜索功能；在SQL中，使用不带`FROM`的`SELECT`语句来测试函数；利用`EXPLAIN ANALYZE`进行数据库查询优化；理解正则表达式的单词边界(`\b`)；在NodeJS中使用`https.Agent`来保持连接打开；或者使用`git log -S`（“pickaxe”模式）通过字符串变更来查找提交。其他有价值的技巧还包括shell通配符（例如，结合`shopt -s globstar`使用的`**/*.md`）以及优先使用`ripgrep` (`rg`) 而非`grep`。

这一概念也延伸到公司内部特有的知识，例如知道遇到问题时该咨询谁、在哪里可以找到文档，或者像滚动重启这样的操作所用的特定命令。作者认为，即使工程师已经掌握了大多数常见技巧，发现一项新技巧也能节省大量时间。鼓励资深工程师与团队分享这些“每日技巧”，以易于理解的方式促进讨论并传播有价值、可操作的知识，从而提升团队整体生产力。

---

## 5. Mistral X Mozilla: Private, Multilingual AI Browsing

**原文标题**: Mistral X Mozilla: Private, Multilingual AI Browsing

**原文链接**: [https://mistral.ai/news/mistral-x-mozilla/](https://mistral.ai/news/mistral-x-mozilla/)

Mistral and Mozilla have partnered to integrate open, private, and multilingual AI into web browsing through Firefox Smart Window (beta), an AI assistant now powered by Mistral models. Available initially in France and North America, then the UK and Germany, Smart Window aids users with complex searches, information recall, and sourcing data from browser tabs.

This collaboration highlights four key principles for the global AI ecosystem:
1.  **Open Technology and Distribution:** Uniting two open-source advocates to demonstrate the potential of open source.
2.  **Locally Optimized AI:** Fine-tuning models on regional languages and dialects to provide culturally nuanced responses.
3.  **User Control and Privacy:** Blending Firefox’s privacy-first legacy with Mistral’s models, ensuring conversations aren't saved on Mozilla's servers by default and Mistral commits to zero data retention.
4.  **Sovereign AI for Everyone:** Extending Mistral’s enterprise-focused technology to end-users worldwide, promoting user control and transparency.

Both companies emphasize preserving an open web where diverse AI providers can compete, preventing a single entity from controlling the AI experience. The partnership aims to deliver privacy, control, and choice to people using AI to browse online, fostering an internet that remains free for exploration and diverse ideas.

---

## 6. Hackers Got Inside a Flock Camera

**原文标题**: Hackers Got Inside a Flock Camera

**原文链接**: [https://www.wired.com/story/hackers-flock-camera-data-shows-how-system-works/](https://www.wired.com/story/hackers-flock-camera-data-shows-how-system-works/)

生成摘要时出错

---

## 7. Xiaomi Mimo 2.6 live post-training dashboard

**原文标题**: Xiaomi Mimo 2.6 live post-training dashboard

**原文链接**: [https://mimo.xiaomi.com/rl/](https://mimo.xiaomi.com/rl/)

生成摘要时出错

---

## 8. Apple Reference Image: A New Approach for Verified Photography

**原文标题**: Apple Reference Image: A New Approach for Verified Photography

**原文链接**: [https://security.apple.com/blog/apple-reference-image/](https://security.apple.com/blog/apple-reference-image/)

生成摘要时出错

---

## 9. AWS says it can't restore some data from mideast facilities struck by Iran

**原文标题**: AWS says it can't restore some data from mideast facilities struck by Iran

**原文链接**: [https://www.wsj.com/world/middle-east/aws-says-it-cant-restore-some-data-from-mideast-facilities-struck-by-iran-ddcb7e5d](https://www.wsj.com/world/middle-east/aws-says-it-cant-restore-some-data-from-mideast-facilities-struck-by-iran-ddcb7e5d)

AWS has informed some customers in its Middle East facilities that they may face irreversible data loss following Iran's missile and drone attacks on Israel in April. The cloud computing giant, a subsidiary of Amazon, acknowledged that the strikes impacted some of its infrastructure, potentially leading to data loss for users whose data was exclusively stored in the directly affected facilities.

AWS emphasized that this situation primarily affects customers who did not follow its recommended best practices for data redundancy. These practices include replicating data across multiple "availability zones" within a region or across different geographical regions for enhanced resilience. While AWS provides durability within a single availability zone, it strongly advises customers to distribute their data to protect against widespread disruptions like physical attacks or power outages.

This incident underscores the shared responsibility model in cloud computing, where providers secure the infrastructure, but customers are accountable for their data's backup, security, and redundancy within the cloud environment. It highlights the critical importance of robust disaster recovery planning and geographical data distribution, particularly for sensitive information stored in regions prone to geopolitical instability.

---

## 10. The Google Play app review process now regularly takes longer than a week

**原文标题**: The Google Play app review process now regularly takes longer than a week

**原文链接**: [https://gultsch.social/@daniel/117280438824908947](https://gultsch.social/@daniel/117280438824908947)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-09-17](output/hacker_news_summary_2026-09-17.md) |
| 2 | [2026-09-16](output/hacker_news_summary_2026-09-16.md) |
| 3 | [2026-09-15](output/hacker_news_summary_2026-09-15.md) |
| 4 | [2026-09-09](output/hacker_news_summary_2026-09-09.md) |
| 5 | [2026-09-07](output/hacker_news_summary_2026-09-07.md) |
| 6 | [2026-09-08](output/hacker_news_summary_2026-09-08.md) |
| 7 | [2026-09-10](output/hacker_news_summary_2026-09-10.md) |
| 8 | [2026-09-06](output/hacker_news_summary_2026-09-06.md) |
| 9 | [2026-09-14](output/hacker_news_summary_2026-09-14.md) |
| 10 | [2026-09-11](output/hacker_news_summary_2026-09-11.md) |
| 11 | [2026-09-13](output/hacker_news_summary_2026-09-13.md) |
| 12 | [2026-09-12](output/hacker_news_summary_2026-09-12.md) |
| 13 | [2026-09-04](output/hacker_news_summary_2026-09-04.md) |
| 14 | [2026-09-01](output/hacker_news_summary_2026-09-01.md) |
| 15 | [2026-09-03](output/hacker_news_summary_2026-09-03.md) |
| 16 | [2026-08-31](output/hacker_news_summary_2026-08-31.md) |
| 17 | [2026-08-28](output/hacker_news_summary_2026-08-28.md) |
| 18 | [2026-09-02](output/hacker_news_summary_2026-09-02.md) |
| 19 | [2026-09-05](output/hacker_news_summary_2026-09-05.md) |
| 20 | [2026-08-30](output/hacker_news_summary_2026-08-30.md) |
| 21 | [2026-08-29](output/hacker_news_summary_2026-08-29.md) |
| 22 | [2026-08-20](output/hacker_news_summary_2026-08-20.md) |
| 23 | [2026-08-25](output/hacker_news_summary_2026-08-25.md) |
| 24 | [2026-08-18](output/hacker_news_summary_2026-08-18.md) |
| 25 | [2026-08-26](output/hacker_news_summary_2026-08-26.md) |
| 26 | [2026-08-19](output/hacker_news_summary_2026-08-19.md) |
| 27 | [2026-08-21](output/hacker_news_summary_2026-08-21.md) |
| 28 | [2026-08-17](output/hacker_news_summary_2026-08-17.md) |
| 29 | [2026-08-23](output/hacker_news_summary_2026-08-23.md) |
| 30 | [2026-08-16](output/hacker_news_summary_2026-08-16.md) |
| 31 | [2026-08-22](output/hacker_news_summary_2026-08-22.md) |
| 32 | [2026-08-24](output/hacker_news_summary_2026-08-24.md) |
| 33 | [2026-08-12](output/hacker_news_summary_2026-08-12.md) |
| 34 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 35 | [2026-08-14](output/hacker_news_summary_2026-08-14.md) |
| 36 | [2026-08-10](output/hacker_news_summary_2026-08-10.md) |
| 37 | [2026-08-11](output/hacker_news_summary_2026-08-11.md) |
| 38 | [2026-08-09](output/hacker_news_summary_2026-08-09.md) |
| 39 | [2026-08-13](output/hacker_news_summary_2026-08-13.md) |
| 40 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 41 | [2026-08-15](output/hacker_news_summary_2026-08-15.md) |
| 42 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 43 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 44 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 45 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 46 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 47 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 48 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 49 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 50 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 51 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 52 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 53 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 54 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 55 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 56 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 57 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 58 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 59 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 60 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 61 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 62 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 63 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 64 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 65 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 66 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 67 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 68 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 69 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 70 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 71 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 72 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 73 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 74 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 75 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 76 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 77 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 78 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 79 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 80 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 81 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 82 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 83 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 84 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 85 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 86 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 87 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 88 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 89 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 90 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 91 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 92 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 93 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 94 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 95 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 96 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 97 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 98 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 99 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 100 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 101 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 102 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 103 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 104 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 105 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 106 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 107 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 108 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 109 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 110 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 111 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 112 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 113 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 114 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 115 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 116 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 117 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 118 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 119 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 120 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 121 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 122 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 123 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 124 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 125 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 126 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 127 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 128 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 129 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 130 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 131 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 132 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 133 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 134 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 135 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 136 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 137 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 138 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 139 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 140 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 141 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 142 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 143 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 144 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 145 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 146 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 147 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 148 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 149 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 150 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 151 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 152 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 153 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 154 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 155 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 156 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 157 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 158 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 159 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 160 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 161 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 162 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 163 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 164 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 165 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 166 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 167 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 168 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 169 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 170 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 171 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 172 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 173 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 174 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 175 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 176 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 177 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 178 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 179 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 180 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 181 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 182 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 183 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 184 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 185 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 186 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 187 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 188 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 189 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 190 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 191 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 192 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 193 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 194 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 195 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 196 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 197 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 198 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 199 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 200 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 201 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 202 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 203 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 204 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 205 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 206 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 207 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 208 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 209 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 210 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 211 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 212 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 213 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 214 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 215 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 216 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 217 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 218 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 219 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 220 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 221 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 222 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 223 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 224 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 225 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 226 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 227 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 228 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 229 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 230 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 231 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 232 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 233 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 234 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 235 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 236 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 237 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 238 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 239 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 240 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 241 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 242 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 243 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 244 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 245 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 246 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 247 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 248 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 249 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 250 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 251 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 252 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 253 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 254 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 255 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 256 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 257 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 258 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 259 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 260 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 261 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 262 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 263 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 264 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 265 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 266 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 267 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 268 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 269 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 270 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 271 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 272 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 273 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 274 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 275 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 276 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 277 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 278 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 279 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 280 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 281 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 282 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 283 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 284 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 285 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 286 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 287 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 288 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 289 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 290 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 291 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 292 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 293 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 294 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 295 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 296 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 297 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 298 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 299 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 300 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 301 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 302 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 303 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 304 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 305 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 306 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 307 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 308 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 309 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 310 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 311 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 312 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
