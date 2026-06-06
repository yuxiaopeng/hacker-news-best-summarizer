# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-06-06.md)

*最后自动更新时间: 2026-06-06 20:38:00*
## 1. 宝可梦 绿宝石 移植到 WebAssembly (10万 FPS)

**原文标题**: Pokemon Emerald Ported to WebAssembly (100k FPS)

**原文链接**: [https://pokeemerald.com/](https://pokeemerald.com/)

本文宣布经典游戏《宝可梦 绿宝石》已成功移植到WebAssembly，并展示了令人印象深刻的性能，达到每秒10万帧（FPS）。随附内容展示了该移植版本的交互式网页界面。界面开始时显示“loading wasm…”指示器，随后是屏幕上的游戏控制按钮，包括方向键（↑、←、→、↓）和动作按钮（B、A、SELECT、START）。界面还显示当前游戏速度设置为“1x”。重要的是，它提供了清晰的键盘操作映射：方向键控制移动，'Z'键作为'A'按钮，'X'键作为'B'按钮，'Enter'键作为'Start'，'Shift'键作为'Select'。这种设置突显了这款深受喜爱的Game Boy Advance游戏的高度优化且用户友好的网络版再现。

---

## 2. 消息人士称，五角大楼将以色列对美间谍威胁级别升至最高。

**原文标题**: Pentagon raised threat of Israeli spying on U.S. to highest level, sources say

**原文链接**: [https://www.nbcnews.com/politics/national-security/pentagon-raised-threat-israeli-spying-us-highest-level-sources-say-rcna348565](https://www.nbcnews.com/politics/national-security/pentagon-raised-threat-israeli-spying-us-highest-level-sources-say-rcna348565)

五角大楼已将以色列对美国间谍活动的反情报威胁级别提升至“危急”，美国官员表示，这是最高级别。美国国防情报局（DIA）发布了这一评估，此前有担忧指出，以色列正在大幅增加对美国高级官员的监视。其目的据报是收集有关特朗普政府在中东冲突，特别是与伊朗的战争方面的内部审议和决策信息。

国防情报局的评估在一份七页的详细文件中指出具体事件，并将以色列的人力和技术情报收集能力评定为“危急”。这一举动发生之际，特朗普总统与以色列总理本雅明·内塔尼亚胡在对伊战争方向问题上的紧张关系日益加剧，特朗普寻求外交协议，而内塔尼亚胡则主张恢复军事行动。

以色列驻华盛顿大使馆强烈否认这些指控，声明以色列不刺探美国，只针对其敌人。一位白宫官员也驳斥这一说法“不实”。

虽然盟友之间存在间谍活动并非罕见，但美国官员认为以色列目前的行动超出了寻常水平。历史上，以色列以对美国进行咄咄逼人的情报收集而闻名，乔纳森·波拉德案便是例证。实际影响是，美国官员在与以色列同行互动或赴以色列时将格外谨慎，尽管与伊朗战争相关的关键情报共享似乎仍未受影响。这一局面存在侵蚀这两个亲密盟友之间信任的风险。

---

## 3. 超越 fork() + exec()

**原文标题**: Moving beyond fork() + exec()

**原文链接**: [https://lwn.net/SubscriberLink/1076018/16f01bbbb8e0d1f0/](https://lwn.net/SubscriberLink/1076018/16f01bbbb8e0d1f0/)

文章指出了Unix/Linux中 `fork()` + `exec()` 进程创建模型长期存在的低效问题。`fork()` 开销很大，它会复制父进程的整个状态，而 `exec()` 却往往立即丢弃这些内存。

陈立提出了“spawn模板”来优化这一问题，其思路是允许应用程序在重复启动*相同*的可执行文件时，通过 `spawn_template_create()` 创建一个模板。这会缓存可执行文件信息，使得后续的 `spawn_template_spawn()` 调用（这些调用指定参数、环境变量和文件描述符操作）变得更快。基准测试显示性能约有2%的提升，分摊了 `exec()` 部分的设置成本。

然而，内核开发者，特别是Mateusz Guzik，批评陈立的提议未能解决主要开销：`fork()`。Guzik主张直接“创建一个纯净的进程”。Christian Brauner同意这一目标，但建议基于 `pidfd` 构建一个更健壮的API。他的设想是使用 `pidfd_open()` 创建一个空进程，随后通过 `pidfd_config()` 调用设置其环境变量、可执行映像及其他属性。这个新接口的一个关键目标将是在用户空间支持一个原生的、高效的 `posix_spawn()` 实现，从而避免当前 `posix_spawn()` 实现中隐藏的 `fork()` + `exec()` 调用。

陈立接受了Brauner的方向。因此，“spawn模板”将不会被合入。相反，未来的工作将集中于开发一个基于 `pidfd` 的API，以提供一个适当的、优化的 `posix_spawn()` 实现，最终超越存在问题的 `fork()` + `exec()` 范式。

---

## 4. Fine-tuning an LLM to write docs like it's 1995

**原文标题**: Fine-tuning an LLM to write docs like it's 1995

**原文链接**: [https://passo.uno/fine-tuning-docs-llm/](https://passo.uno/fine-tuning-docs-llm/)

The author experimented with fine-tuning an LLM to emulate 1990s software technical writing style, a step towards potential future local, specialized LLMs. For training data, they utilized Bitsavers' Microsoft collection of old manuals (1977-2005), cleaning 37 million words down to 192,456 JSONL examples with Python and `gemma-4-26b` for intelligibility.

Instead of training from scratch, QLoRA fine-tuning was chosen for style transfer, not factual retrieval, using Runpod for GPU access (costing around $50). The experiment involved Llama 3.1 8B Instruct, Qwen 2.5 7B Instruct, and a Llama base model. Various parameters were tested, including training data volume, epochs, and QLoRA rank.

Results showed significant style transfer. For documenting `malloc()`, fine-tuned models adopted period-correct structures (Synopsis, Return Value). For a fictitious `ConnectWifi()` function, the 3-epoch Qwen model best maintained the 90s fiction. Most remarkably, Qwen fine-tunes, especially `msft-qwen-192k`, excelled at explaining a modern `REST API` in a convincing, anachronistic 90s-Microsoft style chapter opening. Llama Instruct, due to heavy RLHF, produced bland marketing prose, while the base model failed entirely. Smaller QLoRA ranks (e.g., rank 8) with fewer epochs committed more strongly to the impersonation.

The author concludes that fine-tuned models are effective, relatively cheap style impersonators, useful for augmenting tech writers in tasks like style review or drafting. However, they demand high-quality data, careful model and parameter selection, and still lack human judgment, necessitating significant steering.

---

## 5. Programmers will document for Claude, but not for each other

**原文标题**: Programmers will document for Claude, but not for each other

**原文链接**: [https://blog.plover.com/2026/03/09/#documentation-wins-2](https://blog.plover.com/2026/03/09/#documentation-wins-2)

生成摘要时出错

---

## 6. 量子纠缠构建时空。现在，“神奇”赋予其引力。

**原文标题**: Entanglement Builds Space-Time. Now "Magic" Gives It Gravity

**原文链接**: [https://www.quantamagazine.org/entanglement-builds-space-time-now-magic-gives-it-gravity-20260603/](https://www.quantamagazine.org/entanglement-builds-space-time-now-magic-gives-it-gravity-20260603/)

物理学家在理解引力如何从量子力学中涌现方面迈出了重要一步，解决了约翰·阿奇博尔德·惠勒提出的“物质告诉时空如何弯曲”的挑战。在全息理论中，时空被视为量子粒子集合。此前，这些粒子间的纠缠被证明能构建时空结构，使得空间能够告诉物质如何运动。然而，这些模型产生的时空是“惰性的”，不会响应物质而弯曲。

查尔斯·曹（Charles Cao）领导的新研究将一种名为“魔性”（magic）的量子特性确定为缺失的要素。魔性是量子纠错码中由“非克利福德门”（non-Clifford gates）引入的一种量子性度量，它使时空变得可弯曲。与此前完美分离空间和物质的“稳定器码”（stabilizer codes）不同，新的魔性码允许与空间和物质相关的纠缠相互作用。这种相互作用赋予了空间以灵活性，并将其与引力联系起来。

这一发现表明空间本身是深刻的量子性的，引力则源于量子编码的不完美性。尽管目前仍处于概念验证阶段，但这一框架为发展完整的量子引力理论以及未来在量子计算机上模拟引力现象提供了关键方向。

---

## 7. The Smart TV in Your LivingRoom Is a Node in the AIScraping Economy

**原文标题**: The Smart TV in Your LivingRoom Is a Node in the AIScraping Economy

**原文链接**: [https://blog.includesecurity.com/2026/06/the-smart-tv-in-your-livingroom-is-a-node-in-the-aiscraping-economy/](https://blog.includesecurity.com/2026/06/the-smart-tv-in-your-livingroom-is-a-node-in-the-aiscraping-economy/)

生成摘要时出错

---

## 8. Hacker News, Sans AI

**原文标题**: Hacker News, Sans AI

**原文链接**: [https://elijahpotter.dev/articles/hacker-news-sans-AI](https://elijahpotter.dev/articles/hacker-news-sans-AI)

生成摘要时出错

---

## 9. WSL 2 正在获得更快的 Windows 文件系统访问

**原文标题**: WSL 2 is getting faster Windows file system access

**原文链接**: [https://www.boxofcables.dev/wsl2-per-device-swiotlb-pools-for-virtiofs-and-virtioproxy/](https://www.boxofcables.dev/wsl2-per-device-swiotlb-pools-for-virtiofs-and-virtioproxy/)

WSL 2 is significantly improving cross-OS file system access, crucial for workflows spanning Windows and Linux. WSL 1 initially provided fast Windows drive access via DrvFs. WSL 2, with its Hyper-V VM architecture, shifted to Plan 9 (9P) over Hyper-V sockets, which incurred protocol overhead.

Around 2021, virtiofs was introduced as an experimental opt-in, using VirtIO transport for shared-memory access to reduce serialization overhead compared to 9P. The latest major enhancement, merged in May 2026, addresses a critical bottleneck in the DMA layer. Previously, all virtio devices (like virtiofs mounts and network adapters) shared a single global DMA pool (SWIOTLB), causing contention during heavy I/O. PR #40654 now allocates a dedicated DMA pool for each virtio device, eliminating this shared queue contention.

This fix dramatically benefits file-heavy cross-OS workloads, such as building projects located on a Windows drive within Linux (e.g., `npm install` on `/mnt/c`). VirtioProxy networking also benefits.

To utilize these improvements, users must enable `virtiofs=true` in their `.wslconfig`, update to the latest pre-release WSL kernel (Microsoft.WSL.Kernel 6.18.26.3-1), and ensure their WSL 2 session has over 1 GB of RAM. While virtiofs remains opt-in (9P is still the default), these ongoing efforts are continuously narrowing the performance gap for cross-OS file operations.

---

## 10. Nvidia is proposing a beast of a CPU system for Windows PCs

**原文标题**: Nvidia is proposing a beast of a CPU system for Windows PCs

**原文链接**: [https://twitter.com/lemire/status/2062880075117113739](https://twitter.com/lemire/status/2062880075117113739)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 2 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 3 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 4 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 5 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 6 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 7 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 8 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 9 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 10 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 11 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 12 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 13 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 14 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 15 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 16 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 17 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 18 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 19 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 20 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 21 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 22 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 23 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 24 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 25 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 26 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 27 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 28 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 29 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 30 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 31 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 32 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 33 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 34 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 35 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 36 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 37 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 38 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 39 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 40 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 41 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 42 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 43 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 44 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 45 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 46 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 47 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 48 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 49 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 50 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 51 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 52 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 53 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 54 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 55 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 56 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 57 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 58 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 59 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 60 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 61 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 62 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 63 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 64 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 65 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 66 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 67 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 68 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 69 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 70 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 71 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 72 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 73 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 74 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 75 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 76 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 77 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 78 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 79 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 80 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 81 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 82 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 83 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 84 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 85 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 86 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 87 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 88 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 89 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 90 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 91 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 92 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 93 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 94 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 95 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 96 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 97 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 98 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 99 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 100 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 101 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 102 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 103 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 104 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 105 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 106 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 107 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 108 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 109 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 110 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 111 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 112 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 113 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 114 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 115 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 116 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 117 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 118 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 119 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 120 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 121 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 122 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 123 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 124 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 125 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 126 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 127 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 128 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 129 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 130 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 131 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 132 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 133 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 134 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 135 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 136 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 137 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 138 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 139 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 140 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 141 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 142 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 143 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 144 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 145 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 146 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 147 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 148 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 149 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 150 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 151 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 152 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 153 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 154 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 155 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 156 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 157 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 158 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 159 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 160 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 161 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 162 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 163 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 164 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 165 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 166 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 167 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 168 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 169 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 170 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 171 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 172 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 173 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 174 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 175 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 176 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 177 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 178 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 179 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 180 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 181 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 182 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 183 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 184 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 185 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 186 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 187 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 188 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 189 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 190 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 191 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 192 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 193 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 194 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 195 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 196 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 197 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 198 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 199 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 200 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 201 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 202 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 203 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 204 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 205 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 206 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 207 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 208 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 209 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 210 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 211 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
