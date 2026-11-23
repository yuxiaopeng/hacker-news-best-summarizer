# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-11-23.md)

*最后自动更新时间: 2026-11-23 00:26:30*
## 1. Lean形式化黎曼假设

**原文标题**: Lean verification of the Riemann Hypothesis

**原文链接**: [https://leanprover-community.github.io/blog/posts/riemann-hypothesis/](https://leanprover-community.github.io/blog/posts/riemann-hypothesis/)

2026年11月20日，Levent Alpöge发布了一个包含1700万行代码的Lean库，其中包含黎曼猜想的证明。Lean和Mathlib社区在Lean FRO和Mathlib Initiative的支持下，经过一天的验证过程后，联合声明对该证明的正确性充满信心。

他们的理由基于以下四项已满足的标准：
1.  **正确的陈述：** 黎曼猜想的陈述（作为Mathlib的一部分）已经过专家审查。
2.  **正确编译：** Alpöge庞大的代码库编译无错误，并经数十人验证。
3.  **证明了正确的陈述：** 独立工具确认，Alpöge证明的定理与Mathlib中黎曼猜想的陈述精确匹配。
4.  **有效证明：** 导出的证明经过多个证明检查器严格检查，包括Lean的官方内核以及con-leche和con-ron等几个第三方工具。值得注意的是，con-leche和con-ron都有形式化证明，表明它们无法接受虚假证明，这解决了对Lean自身逻辑可能存在缺陷的担忧。这些检查是在一个静态导出文件上进行的，以防止恶意代码。

社区向贡献者表示感谢，并期待数学界能够探索和解释该证明中的新思想。

---

## 2. 丰田、日产、本田将标准化零部件以降低成本

**原文标题**: Toyota, Nissan, and Honda to standardize parts to lower costs

**原文链接**: [https://www.caranddriver.com/news/a74490092/toyota-nissan-honda-standardize-parts-lower-costs/](https://www.caranddriver.com/news/a74490092/toyota-nissan-honda-standardize-parts-lower-costs/)

丰田、日产和本田计划标准化多种汽车零部件，以大幅降低生产成本。日本汽车工业协会会长佐藤浩二宣布，这项举措旨在将节省下来的资金投入新创新，以应对来自中国汽车制造商日益激烈的竞争。

标准化工作最初将集中于三个关键领域：统一的钢铁质量标准、塑料和树脂的统一规范，以及线束的通用颜色编码方案。选择这些组件是因为它们通常不被消费者察觉，从而保持了各个品牌的品牌识别度，但却占用了大量的生产成本，确保能立即对成本产生影响。

目前正在与日本国内的汽车零部件供应商展开讨论，国际供应商将在稍后被纳入。首批标准化工作计划于明年生效。从长远来看，日本汽车工业协会计划标准化更广泛的汽车零部件。此举反映出包括马自达、斯巴鲁、三菱和铃木等日本汽车制造商之间存在“强烈的危机感”，促使它们精简运营并提高竞争力。

---

## 3. 到2028年，Anthropic的能源87%将来自天然气，11%将来自煤炭。

**原文标题**: 87% of the Anthropic power will come from gas and 11% from coal in 2028

**原文链接**: [https://betterdatacenterproject.com/2026/11/16/how-ai-is-powered-a-breakdown-of-byop-and-grid-power/](https://betterdatacenterproject.com/2026/11/16/how-ai-is-powered-a-breakdown-of-byop-and-grid-power/)

文章揭示，尽管Anthropic声称对可再生能源感兴趣，但到2028年，其在美国的AI计算能力中，87%将来自天然气，11%将来自煤炭。该公司未做出任何直接的美国可再生能源承诺，反而大量投资于天然气发电机。

到2028年，Anthropic已签约的15 GW计算能力（其中5.9-9.6 GW与特定数据中心相关）将主要由新的现场天然气、新的电网天然气以及现有化石燃料来源供电。这预计将导致巨大的环境后果：
*   **排放量：** 到2028年，每年因电力使用产生的二氧化碳排放量可能达到1700万至3800万吨二氧化碳当量（中值：3200万吨），这可能超过加利福尼亚州2024年全年发电排放总量，以及Meta、微软和谷歌2025年范围2排放量的总和。这还将使美国数据中心行业的排放量增加16-36%。
*   **碳强度：** 估计Anthropic的电力碳强度将比美国电网平均水平高出35%，这主要归因于数据中心选址在煤炭/天然气资源丰富的地区。
*   **低效率与污染：** 其2.5 GW现场天然气发电能力中，80%使用低效率的简单循环涡轮机，每年产生超过13,000吨氮氧化物和2,000吨细颗粒物。这种空气污染可能每年造成20亿至30亿美元的健康损害。
*   **可疑做法：** Anthropic使用的设施包括SpaceX的Colossus 2（依赖临时、未经许可且不受控制的涡轮机）以及Nscale的Monarch（由低效率、高排放的发动机供电）。

---

## 4. 引爆一堆叠氮化铅

**原文标题**: Detonating a pile of lead azide

**原文链接**: [https://www.science.org/content/blog-post/detonating-huge-pile-lead-azide-really](https://www.science.org/content/blog-post/detonating-huge-pile-lead-azide-really)

Science.org 的“In the Pipeline”博客文章中，一篇题为《引爆一堆叠氮化铅》的文章，纠正了关于叠氮化铅历史用途及其感知危险的普遍误解，尤其是在大量存在的情况下。文章作者是一位药物化学家，驳斥了虚构作品中经常描绘的、由掉落一桶叠氮化铅而引发巨大爆炸的夸大情景。

叠氮化铅确实是一种敏感而强大的初级炸药，主要用作雷管中的起爆药。然而，作者强调，由于其对冲击、摩擦和静电的极度敏感性，它*绝不会*以“堆”或“桶”的形式进行处理。处理通常涉及非常小的、严格控制的少量，通常用水润湿以在运输和储存过程中降低敏感性。

该博文指出，尽管危险，但其敏感性使其不适合大规模储存或随意引爆。流行文化中描绘的“爆炸”常常夸大了其数量和引发此类灾难的容易程度，尤其是在高度受控的工业环境之外，在这些环境中，它被制造并小心地加工成极小装药量的雷管。核心信息是，尽管它威力强大，但叠氮化铅的实际处理和实用性远不如通常想象的那样耸人听闻。

---

## 5. 我的显示器使我的下载速度降低了75%。

**原文标题**: My monitor was cutting my download speed by 75%

**原文链接**: [https://blog.tymscar.com/posts/studiodisplayethernet/](https://blog.tymscar.com/posts/studiodisplayethernet/)

Oscar Molnar 发现，当他的绿联 (UGREEN) 2.5G USB-C 以太网适配器连接到 Apple Studio Display XDR 时，他 2.5 Gbps 的互联网下载速度下降了 75%（降至 600 Mbps），而上传速度则未受影响。将适配器直接连接到他的 MacBook Pro M3 Pro 后，速度恢复正常，这表明显示器是瓶颈所在。

初步故障排除措施包括安装 Realtek 针对 RTL8156B 芯片的专用驱动程序，将速度提升至 1.1 Gbps；并在他的 UniFi 路由器上启用流量控制，达到 2 Gbps。然而，由于潜在的延迟问题，流量控制是一个不理想的权宜之计。

通过 UDP 流量的进一步调查显示，当原始适配器通过显示器连接时，在速度超过约 2 Gbps 时开始显著丢包。核心问题是显示器内部的 USB 集线器及其处理 USB 3 设备通信的方式。RTL8156B 适配器每次突发传输只发送 4KB（4 个数据包），然后需要 Mac 发出“继续”信号。发送这些数据包并等待 Mac 回复的总时间导致数据从适配器到 Mac 的有效数据引流速率仅约为 2 Gbps。当传入数据为 2.5 Gbps 时，适配器的缓冲区会溢出，导致丢包和速度下降。上传未受影响，因为瓶颈在于数据从适配器传输到 Mac。

解决方案是使用一个新的绿联 (UGREEN) 5G USB-C 以太网适配器（RTL8157 芯片），它每次突发传输 8KB（8 个数据包）。这与更快的链路相结合，将有效引流速率提高到 4.5 Gbps，从而防止了缓冲区溢出并实现了完整的 2.5 Gbps 下载速度。作者强调，传输速度受复杂因素影响，不仅仅是链路速度，还包括数据包突发大小和主机回复时间。

---

## 6. Inkling-2-Mini 在 5.4 GB 内存中

**原文标题**: Inkling-2-Mini in 5.4 GB Memory

**原文链接**: [https://github.com/ShinMegamiBoson/lookatmyquant](https://github.com/ShinMegamiBoson/lookatmyquant)

LookAtMyQuant是一个量化编译器，旨在显著减少大型语言模型的内存占用，同时最大限度地减少性能下降。它通过根据模型参数的影响选择性地压缩这些参数来实现这一点，采用格码、费雪信息和蒸馏等技术。

主要成就包括：
*   **Qwen3.5-4B：** 压缩至1.23 GB（每权重2.3比特），解决了540道数学题中的330道，与原始模型的KL散度为0.45 nats。
*   **Qwen3.8-27B：** 从53.7 GB减少到7.2 GB（每权重2.1比特），匹配原始模型的数学性能（540道题中答对401道），并在HumanEval、MMLU和GSM8K上超越其他GGUF模型。

本文重点介绍了**Inkling-2-Mini**，一个26.4B物理 / 5.4B活跃的MoE模型。LookAtMyQuant将其18.89 GB的BF16文本权重压缩为多个Apple Silicon MLX版本。具体而言，**5.4 GB（1.65 bpp）版本（使用SQYFR v2）**在GSM8K（200）上达到87.0%，在HumanEval（164）上达到71.3%，三项任务平均值为89.0%。其他版本包括从匹配教师模型性能的12.8 GB版本到适用于8 GB iPhone的3.9 GB（1.18 bpp）版本。

这些模型在Apple Silicon MLX上借助专用的Metal内核高效运行，通常与DSpark草稿器配合使用以提高解码速度。例如，5.4 GB模型实现了75.3 tok/s的串行解码速度和124.4 tok/s的草稿解码中位数速度。LookAtMyQuant还通过CUDA支持NVIDIA GPU。该编译器的代码采用MIT许可证，安装方式为`pip install git+https://github.com/ShinMegamiBoson/lookatmyquant.git`，提供命令行工具、Python集成以及一个兼容OpenAI的服务器。

---

## 7. Sandwich Simulator

**原文标题**: Sandwich Simulator

**原文链接**: [https://stulle.app/](https://stulle.app/)

本文介绍了一个“三明治模拟器”(Stullensimulator)，这是一个运行需要JavaScript的在线工具。文本显示这是一种互动体验，并伴有“三明治加载中”的提示信息。提及的关键功能或自定义类别包括“Foto”（照片）、“Aufstriche”（涂抹酱）和“Mehr Beläge”（更多配料），表明用户可以虚拟地制作和定制自己的三明治。

---

## 8. Perplexity and Intelligence

**原文标题**: Perplexity and Intelligence

**原文链接**: [https://openai.com/index/perplexity-and-intelligence/](https://openai.com/index/perplexity-and-intelligence/)

Jakub Pachocki, OpenAI's Chief Scientist, argues that AI progress hinges on training "compressors" (predictors) on large datasets, and **perplexity** (or cross-entropy loss) is the key metric for tracking this advancement and the emergence of general intelligence. He proposes establishing perplexity as a shared industry benchmark to inform safety standards, with OpenAI sharing its internal measurements as a first step.

The article highlights how decreasing log-perplexity correlates with significant emergent capabilities in OpenAI models: GPT-2 for coherent text, GPT-3 for in-context learning, GPT-3.5 for fluent conversation, and GPT-4 for chain-of-thought reasoning. Reaching log-losses below 0.8 has yielded transformative capabilities in fields like cybersecurity and mathematics. Pachocki expects further breakthroughs as perplexity drops to ~0.68-0.7.

A potential "step change" in AI development may come from AI's own participation in algorithmic pretraining research, accelerating progress akin to recent mathematical breakthroughs. Given this rapid advance and the hard-to-predict emergent capabilities, he urges frontier model developers to jointly establish evaluation norms, red-team safety cases, and shared transparency standards. He proposes common perplexity-based limits that developers commit not to cross until AI understanding and monitoring capabilities reach concrete milestones.

While acknowledging challenges like cross-lab comparison and perplexity's detachment from specific tasks, Pachocki asserts its enduring value in consistently indicating gains in general intelligence and standardizing discussions on AI progress.

---

## 9. 硅谷怎么了？

**原文标题**: What Happened to Silicon Valley?

**原文链接**: [https://www.oreilly.com/radar/what-happened-to-silicon-valley/](https://www.oreilly.com/radar/what-happened-to-silicon-valley/)

生成摘要时出错

---

## 10. The Birds of GTA 6: A Field Guide to Vice City and Leonida's Wildlife

**原文标题**: The Birds of GTA 6: A Field Guide to Vice City and Leonida's Wildlife

**原文链接**: [https://www.audubon.org/magazine/birds-of-gta-6-field-guide-vice-city-wildlife](https://www.audubon.org/magazine/birds-of-gta-6-field-guide-vice-city-wildlife)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-11-23](output/hacker_news_summary_2026-11-23.md) |
| 2 | [2026-11-22](output/hacker_news_summary_2026-11-22.md) |
| 3 | [2026-11-21](output/hacker_news_summary_2026-11-21.md) |
| 4 | [2026-11-20](output/hacker_news_summary_2026-11-20.md) |
| 5 | [2026-11-19](output/hacker_news_summary_2026-11-19.md) |
| 6 | [2026-11-14](output/hacker_news_summary_2026-11-14.md) |
| 7 | [2026-11-15](output/hacker_news_summary_2026-11-15.md) |
| 8 | [2026-11-18](output/hacker_news_summary_2026-11-18.md) |
| 9 | [2026-11-13](output/hacker_news_summary_2026-11-13.md) |
| 10 | [2026-11-17](output/hacker_news_summary_2026-11-17.md) |
| 11 | [2026-11-07](output/hacker_news_summary_2026-11-07.md) |
| 12 | [2026-11-06](output/hacker_news_summary_2026-11-06.md) |
| 13 | [2026-11-11](output/hacker_news_summary_2026-11-11.md) |
| 14 | [2026-11-08](output/hacker_news_summary_2026-11-08.md) |
| 15 | [2026-11-05](output/hacker_news_summary_2026-11-05.md) |
| 16 | [2026-11-12](output/hacker_news_summary_2026-11-12.md) |
| 17 | [2026-11-10](output/hacker_news_summary_2026-11-10.md) |
| 18 | [2026-11-01](output/hacker_news_summary_2026-11-01.md) |
| 19 | [2026-11-03](output/hacker_news_summary_2026-11-03.md) |
| 20 | [2026-10-28](output/hacker_news_summary_2026-10-28.md) |
| 21 | [2026-10-29](output/hacker_news_summary_2026-10-29.md) |
| 22 | [2026-10-31](output/hacker_news_summary_2026-10-31.md) |
| 23 | [2026-10-30](output/hacker_news_summary_2026-10-30.md) |
| 24 | [2026-11-04](output/hacker_news_summary_2026-11-04.md) |
| 25 | [2026-10-24](output/hacker_news_summary_2026-10-24.md) |
| 26 | [2026-10-23](output/hacker_news_summary_2026-10-23.md) |
| 27 | [2026-10-25](output/hacker_news_summary_2026-10-25.md) |
| 28 | [2026-10-27](output/hacker_news_summary_2026-10-27.md) |
| 29 | [2026-10-21](output/hacker_news_summary_2026-10-21.md) |
| 30 | [2026-10-22](output/hacker_news_summary_2026-10-22.md) |
| 31 | [2026-10-20](output/hacker_news_summary_2026-10-20.md) |
| 32 | [2026-10-26](output/hacker_news_summary_2026-10-26.md) |
| 33 | [2026-10-19](output/hacker_news_summary_2026-10-19.md) |
| 34 | [2026-10-18](output/hacker_news_summary_2026-10-18.md) |
| 35 | [2026-10-17](output/hacker_news_summary_2026-10-17.md) |
| 36 | [2026-10-16](output/hacker_news_summary_2026-10-16.md) |
| 37 | [2026-10-13](output/hacker_news_summary_2026-10-13.md) |
| 38 | [2026-10-09](output/hacker_news_summary_2026-10-09.md) |
| 39 | [2026-10-11](output/hacker_news_summary_2026-10-11.md) |
| 40 | [2026-10-15](output/hacker_news_summary_2026-10-15.md) |
| 41 | [2026-10-14](output/hacker_news_summary_2026-10-14.md) |
| 42 | [2026-10-07](output/hacker_news_summary_2026-10-07.md) |
| 43 | [2026-10-10](output/hacker_news_summary_2026-10-10.md) |
| 44 | [2026-10-03](output/hacker_news_summary_2026-10-03.md) |
| 45 | [2026-10-02](output/hacker_news_summary_2026-10-02.md) |
| 46 | [2026-09-29](output/hacker_news_summary_2026-09-29.md) |
| 47 | [2026-09-30](output/hacker_news_summary_2026-09-30.md) |
| 48 | [2026-09-27](output/hacker_news_summary_2026-09-27.md) |
| 49 | [2026-10-01](output/hacker_news_summary_2026-10-01.md) |
| 50 | [2026-10-06](output/hacker_news_summary_2026-10-06.md) |
| 51 | [2026-10-04](output/hacker_news_summary_2026-10-04.md) |
| 52 | [2026-09-24](output/hacker_news_summary_2026-09-24.md) |
| 53 | [2026-09-21](output/hacker_news_summary_2026-09-21.md) |
| 54 | [2026-09-23](output/hacker_news_summary_2026-09-23.md) |
| 55 | [2026-09-20](output/hacker_news_summary_2026-09-20.md) |
| 56 | [2026-09-19](output/hacker_news_summary_2026-09-19.md) |
| 57 | [2026-09-25](output/hacker_news_summary_2026-09-25.md) |
| 58 | [2026-09-22](output/hacker_news_summary_2026-09-22.md) |
| 59 | [2026-09-18](output/hacker_news_summary_2026-09-18.md) |
| 60 | [2026-09-13](output/hacker_news_summary_2026-09-13.md) |
| 61 | [2026-09-14](output/hacker_news_summary_2026-09-14.md) |
| 62 | [2026-09-17](output/hacker_news_summary_2026-09-17.md) |
| 63 | [2026-09-16](output/hacker_news_summary_2026-09-16.md) |
| 64 | [2026-09-15](output/hacker_news_summary_2026-09-15.md) |
| 65 | [2026-09-05](output/hacker_news_summary_2026-09-05.md) |
| 66 | [2026-09-12](output/hacker_news_summary_2026-09-12.md) |
| 67 | [2026-09-06](output/hacker_news_summary_2026-09-06.md) |
| 68 | [2026-09-03](output/hacker_news_summary_2026-09-03.md) |
| 69 | [2026-09-08](output/hacker_news_summary_2026-09-08.md) |
| 70 | [2026-09-07](output/hacker_news_summary_2026-09-07.md) |
| 71 | [2026-09-11](output/hacker_news_summary_2026-09-11.md) |
| 72 | [2026-09-04](output/hacker_news_summary_2026-09-04.md) |
| 73 | [2026-09-09](output/hacker_news_summary_2026-09-09.md) |
| 74 | [2026-09-10](output/hacker_news_summary_2026-09-10.md) |
| 75 | [2026-08-29](output/hacker_news_summary_2026-08-29.md) |
| 76 | [2026-09-01](output/hacker_news_summary_2026-09-01.md) |
| 77 | [2026-09-02](output/hacker_news_summary_2026-09-02.md) |
| 78 | [2026-08-30](output/hacker_news_summary_2026-08-30.md) |
| 79 | [2026-08-26](output/hacker_news_summary_2026-08-26.md) |
| 80 | [2026-08-31](output/hacker_news_summary_2026-08-31.md) |
| 81 | [2026-08-28](output/hacker_news_summary_2026-08-28.md) |
| 82 | [2026-08-20](output/hacker_news_summary_2026-08-20.md) |
| 83 | [2026-08-16](output/hacker_news_summary_2026-08-16.md) |
| 84 | [2026-08-22](output/hacker_news_summary_2026-08-22.md) |
| 85 | [2026-08-24](output/hacker_news_summary_2026-08-24.md) |
| 86 | [2026-08-18](output/hacker_news_summary_2026-08-18.md) |
| 87 | [2026-08-25](output/hacker_news_summary_2026-08-25.md) |
| 88 | [2026-08-17](output/hacker_news_summary_2026-08-17.md) |
| 89 | [2026-08-15](output/hacker_news_summary_2026-08-15.md) |
| 90 | [2026-08-21](output/hacker_news_summary_2026-08-21.md) |
| 91 | [2026-08-23](output/hacker_news_summary_2026-08-23.md) |
| 92 | [2026-08-19](output/hacker_news_summary_2026-08-19.md) |
| 93 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 94 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 95 | [2026-08-11](output/hacker_news_summary_2026-08-11.md) |
| 96 | [2026-08-10](output/hacker_news_summary_2026-08-10.md) |
| 97 | [2026-08-12](output/hacker_news_summary_2026-08-12.md) |
| 98 | [2026-08-14](output/hacker_news_summary_2026-08-14.md) |
| 99 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 100 | [2026-08-09](output/hacker_news_summary_2026-08-09.md) |
| 101 | [2026-08-13](output/hacker_news_summary_2026-08-13.md) |
| 102 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 103 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 104 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 105 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 106 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 107 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 108 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 109 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 110 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 111 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 112 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 113 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 114 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 115 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 116 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 117 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 118 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 119 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 120 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 121 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 122 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 123 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 124 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 125 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 126 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 127 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 128 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 129 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 130 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 131 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 132 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 133 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 134 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 135 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 136 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 137 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 138 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 139 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 140 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 141 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 142 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 143 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 144 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 145 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 146 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 147 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 148 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 149 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 150 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 151 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 152 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 153 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 154 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 155 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 156 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 157 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 158 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 159 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 160 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 161 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 162 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 163 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 164 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 165 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 166 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 167 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 168 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 169 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 170 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 171 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 172 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 173 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 174 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 175 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 176 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 177 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 178 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 179 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 180 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 181 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 182 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 183 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 184 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 185 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 186 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 187 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 188 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 189 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 190 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 191 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 192 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 193 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 194 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 195 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 196 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 197 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 198 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 199 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 200 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 201 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 202 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 203 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 204 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 205 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 206 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 207 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 208 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 209 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 210 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 211 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 212 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 213 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 214 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 215 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 216 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 217 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 218 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 219 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 220 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 221 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 222 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 223 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 224 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 225 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 226 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 227 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 228 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 229 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 230 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 231 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 232 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 233 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 234 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 235 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 236 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 237 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 238 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 239 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 240 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 241 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 242 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 243 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 244 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 245 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 246 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 247 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 248 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 249 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 250 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 251 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 252 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 253 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 254 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 255 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 256 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 257 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 258 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 259 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 260 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 261 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 262 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 263 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 264 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 265 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 266 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 267 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 268 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 269 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 270 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 271 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 272 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 273 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 274 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 275 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 276 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 277 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 278 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 279 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 280 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 281 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 282 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 283 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 284 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 285 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 286 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 287 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 288 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 289 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 290 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 291 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 292 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 293 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 294 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 295 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 296 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 297 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 298 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 299 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 300 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 301 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 302 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 303 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 304 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 305 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 306 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 307 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 308 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 309 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 310 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 311 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 312 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 313 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 314 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 315 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 316 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 317 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 318 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 319 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 320 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 321 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 322 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 323 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 324 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 325 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 326 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 327 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 328 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 329 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 330 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 331 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 332 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 333 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 334 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 335 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 336 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 337 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 338 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 339 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 340 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 341 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 342 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 343 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 344 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 345 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 346 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 347 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 348 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 349 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 350 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 351 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 352 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 353 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 354 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 355 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 356 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 357 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 358 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 359 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 360 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 361 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 362 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 363 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 364 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 365 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 366 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 367 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 368 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 369 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 370 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 371 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
