# Hacker News 热门文章摘要 (2026-11-23)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

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

## 11. Data Processing Incidents on Inference Providers

**原文标题**: Data Processing Incidents on Inference Providers

**原文链接**: [https://openrouter.ai/blog/announcements/data-processing-incidents-on-inference-providers/](https://openrouter.ai/blog/announcements/data-processing-incidents-on-inference-providers/)

生成摘要时出错

---

## 12. GnuPG Security Advisory for GPGME

**原文标题**: GnuPG Security Advisory for GPGME

**原文链接**: [https://lists.gnupg.org/pipermail/gnupg-announce/2026q4/000517.html](https://lists.gnupg.org/pipermail/gnupg-announce/2026q4/000517.html)

生成摘要时出错

---

## 13. Show HN: I built a game where you are an LLM's subagent

**原文标题**: Show HN: I built a game where you are an LLM's subagent

**原文链接**: [https://github.com/gulivan/worker755](https://github.com/gulivan/worker755)

生成摘要时出错

---

## 14. Advice for the next 100 Rust GUIs

**原文标题**: Advice for the next 100 Rust GUIs

**原文链接**: [https://linebender.org/blog/next-100-guis/](https://linebender.org/blog/next-100-guis/)

生成摘要时出错

---

## 15. Backblaze Notice at Collection and Privacy Policy

**原文标题**: Backblaze Notice at Collection and Privacy Policy

**原文链接**: [https://www.backblaze.com/company/policy/privacy](https://www.backblaze.com/company/policy/privacy)

生成摘要时出错

---

## 16. Re: Riemann

**原文标题**: Re: Riemann

**原文链接**: [https://borretti.me/article/re-riemann](https://borretti.me/article/re-riemann)

The author describes learning about the Riemann Hypothesis being proven by "Claude," an AI, noting the human collaborator's announcement which emphasized Claude's exceptional performance and outstripping of human efforts. He contrasts this deferential tone with human-centric celebrations of achievement, like Ayn Rand's exultation over Apollo 11 or Diego Rivera's "Man, Controller of the Universe" mural, both of which laud "Man's greatness" and his triumph over nature and the unknown.

For the author, the Riemann announcement signifies a shift where "humanity is not at the center. Claude is at the center," reducing humans to "passive recipients." He interprets this trend as a "betrayal and a surrender," arguing that the vision of AI companies and proponents like those in effective altruism suggests humans should abdicate their drive to explore, invent, and strive for self-improvement. The article concludes by questioning the purpose of human struggle and aspiration if AI fulfills all grand endeavors, suggesting a passive surrender rather than a drive to "become divine."

---

## 17. Leonida – PC Recompilation of the Xbox Version of GTA 6

**原文标题**: Leonida – PC Recompilation of the Xbox Version of GTA 6

**原文链接**: [https://github.com/ItsNotRexed/Leonida](https://github.com/ItsNotRexed/Leonida)

生成摘要时出错

---

## 18. Open Social Web Alliance

**原文标题**: Open Social Web Alliance

**原文链接**: [https://osw-alliance.net/en/](https://osw-alliance.net/en/)

生成摘要时出错

---

## 19. Clojure will affect the way you think about programming (2017)

**原文标题**: Clojure will affect the way you think about programming (2017)

**原文链接**: [https://eli.thegreenplace.net/2017/clojure-the-perfect-language-to-expand-your-brain/](https://eli.thegreenplace.net/2017/clojure-the-perfect-language-to-expand-your-brain/)

生成摘要时出错

---

## 20. FBI reportedly investigating apparent hack of its criminal database

**原文标题**: FBI reportedly investigating apparent hack of its criminal database

**原文链接**: [https://www.bbc.com/news/articles/cvze7de86pk3o](https://www.bbc.com/news/articles/cvze7de86pk3o)

生成摘要时出错

---

## 21. Astra 6.2 and Sol 6.2 flop at Simple Bench

**原文标题**: Astra 6.2 and Sol 6.2 flop at Simple Bench

**原文链接**: [https://simple-bench.com/](https://simple-bench.com/)

A new multiple-choice text benchmark called SimpleBench has been introduced to evaluate large language models (LLMs). Comprising over 200 questions, SimpleBench assesses spatio-temporal reasoning, social intelligence, and "linguistic adversarial robustness" (trick questions).

Crucially, SimpleBench reveals a unique performance gap: individuals with unspecialized (high school) knowledge outperform state-of-the-art LLMs. A small sample of nine human participants achieved an average score of 83.7%, surpassing all tested LLMs, including Claude Fable, which scored 81.9%. This contrasts with most text-based benchmarks where LLMs typically exceed human performance.

The results suggest that the memorized knowledge and approximate reasoning capabilities prevalent in frontier LLMs are not always sufficient for answering the "basic questions" presented in SimpleBench. For more details on the findings and methodology, a full technical report is available, and users can test models on the Simple Bench app via LMcouncil.ai.

---

## 22. Fast-Anything: Don't rewrite it in Rust. Rewrite the 5% that's slow

**原文标题**: Fast-Anything: Don't rewrite it in Rust. Rewrite the 5% that's slow

**原文链接**: [https://github.com/EL4CTEO/fast-anything](https://github.com/EL4CTEO/fast-anything)

生成摘要时出错

---

## 23. Show HN: Zero C# – C# without a runtime or GC

**原文标题**: Show HN: Zero C# – C# without a runtime or GC

**原文链接**: [https://onurgumus.github.io/zero-csharp/index.html](https://onurgumus.github.io/zero-csharp/index.html)

生成摘要时出错

---

## 24. Sir Brian May adds new dimension to Hera asteroid

**原文标题**: Sir Brian May adds new dimension to Hera asteroid

**原文链接**: [https://www.esa.int/articles/about-us/directorates/operations/space-safety/hera/sir-brian-may-adds-new-dimension-to-hera-asteroid](https://www.esa.int/articles/about-us/directorates/operations/space-safety/hera/sir-brian-may-adds-new-dimension-to-hera-asteroid)

生成摘要时出错

---

## 25. Jensen Huang's fall is bad news for Silicon Valley's accelerationists

**原文标题**: Jensen Huang's fall is bad news for Silicon Valley's accelerationists

**原文链接**: [https://www.economist.com/business/2026/11/19/jensen-huangs-fall-is-bad-news-for-silicon-valleys-accelerationists](https://www.economist.com/business/2026/11/19/jensen-huangs-fall-is-bad-news-for-silicon-valleys-accelerationists)

生成摘要时出错

---

## 26. ClawDOS – An AI coding agent for DOS

**原文标题**: ClawDOS – An AI coding agent for DOS

**原文链接**: [http://ricapar.net/ClawDOS/](http://ricapar.net/ClawDOS/)

ClawDOS is an AI chat and coding agent designed to run on a vintage IBM PC XT (8088 at 4.77 MHz, 640K RAM, CGA). This project merges old and new technology, with 100% of its codebase, except for the introductory text, generated by Claude AI.

The core component, HARNESS.EXE, is a 176 KB DOS program that directly interacts with the Claude Messages API. It functions as a complete coding environment, allowing the AI to read/edit files, write, compile (using tools like Turbo C), and execute programs, and even capture screenshots of the output. A "bridge" PC handles TLS encryption, offloading this burden from the 8088 processor.

Key capabilities include:
*   **Code Generation:** From simple prime number programs to complex "WarGames" demos with vector graphics and sound, ClawDOS can write, compile, and run C code.
*   **Screen Perception:** It captures CGA video memory as PNG images, allowing Claude to "see" and interpret the output of programs.
*   **Persistent Memory:** It remembers past conversations, projects, and custom code ("memories" in C:\MEMORY) and utilizes built-in "skills" for development tools and CGA effects.
*   **Extensive Toolset:** ClawDOS features 18 tools for file operations, system information, memory/port manipulation, PC speaker music, and text art.
*   **User Interface:** A CGA-optimized chat screen, persistent conversations, safe mode for file changes, and flexible AI model switching enhance usability.

The system runs on FreeDOS with mTCP for networking, built with Open Watcom. It can be deployed on real IBM PC XT hardware (often with a PicoMEM card for modern I/O) or emulated environments like 86Box, offering a unique blend of historical computing and cutting-edge AI.

---

## 27. Surprisingly Adorable Insect Portraits

**原文标题**: Surprisingly Adorable Insect Portraits

**原文链接**: [https://amateurphotographer.com/latest/these-astonishing-insect-portraits-reveal-a-hidden-world-you-never-knew-existed/](https://amateurphotographer.com/latest/these-astonishing-insect-portraits-reveal-a-hidden-world-you-never-knew-existed/)

生成摘要时出错

---

## 28. PostgreSQL Extensions in Go

**原文标题**: PostgreSQL Extensions in Go

**原文链接**: [https://jespino.github.io/gopgext/](https://jespino.github.io/gopgext/)

生成摘要时出错

---

## 29. The Mythology of Conscious AI

**原文标题**: The Mythology of Conscious AI

**原文链接**: [https://www.noemamag.com/the-mythology-of-conscious-ai/](https://www.noemamag.com/the-mythology-of-conscious-ai/)

生成摘要时出错

---

## 30. PcapAnalyzer – self-hosted pcap analyzer with 27 problem detectors

**原文标题**: PcapAnalyzer – self-hosted pcap analyzer with 27 problem detectors

**原文链接**: [https://github.com/sebaandrada-cell/PcapAnalyzer](https://github.com/sebaandrada-cell/PcapAnalyzer)

生成摘要时出错

---

## 31. Upload2Shell (CVE-2026-125396)

**原文标题**: Upload2Shell (CVE-2026-125396)

**原文链接**: [https://pwn.ai/upload2shell](https://pwn.ai/upload2shell)

生成摘要时出错

---

## 32. Serious cyberattack thought backed by wealthy operators

**原文标题**: Serious cyberattack thought backed by wealthy operators

**原文链接**: [https://www.ruv.is/english/2026-11-20-serious-cyberattack-thought-backed-by-wealthy-operators-493411](https://www.ruv.is/english/2026-11-20-serious-cyberattack-thought-backed-by-wealthy-operators-493411)

生成摘要时出错

---

## 33. Europe weakens chemical rules as science links them to 'lifestyle diseases'

**原文标题**: Europe weakens chemical rules as science links them to 'lifestyle diseases'

**原文链接**: [https://www.lemonde.fr/en/opinion/article/2026/11/22/as-science-increasingly-shows-the-role-chemical-substances-play-in-lifestyle-diseases-europe-weakens-its-regulations_6786595_23.html](https://www.lemonde.fr/en/opinion/article/2026/11/22/as-science-increasingly-shows-the-role-chemical-substances-play-in-lifestyle-diseases-europe-weakens-its-regulations_6786595_23.html)

生成摘要时出错

---

## 34. A Beginner's Guide to Local AI with Inkling, Qwen, and Unsloth

**原文标题**: A Beginner's Guide to Local AI with Inkling, Qwen, and Unsloth

**原文链接**: [https://www.gpupartner.com/blog/beginners-guide-local-ai-inkling-qwen-unsloth](https://www.gpupartner.com/blog/beginners-guide-local-ai-inkling-qwen-unsloth)

生成摘要时出错

---

## 35. Backblaze customers worried of personal data sale/sharing after policy update

**原文标题**: Backblaze customers worried of personal data sale/sharing after policy update

**原文链接**: [https://www.neowin.net/news/backblaze-customers-worried-of-personal-data-salesharing-after-policy-update/](https://www.neowin.net/news/backblaze-customers-worried-of-personal-data-salesharing-after-policy-update/)

生成摘要时出错

---

## 36. Pandex – Official European Law for AI Agents, over MCP

**原文标题**: Pandex – Official European Law for AI Agents, over MCP

**原文链接**: [https://www.pandex.io](https://www.pandex.io)

生成摘要时出错

---

## 37. Verification files for the Lean proof of the Riemann Hypothesis

**原文标题**: Verification files for the Lean proof of the Riemann Hypothesis

**原文链接**: [https://math.mit.edu/~drew/grh/](https://math.mit.edu/~drew/grh/)

生成摘要时出错

---

## 38. I joined the NTP Pool, but not with my Stratum 1 Pi

**原文标题**: I joined the NTP Pool, but not with my Stratum 1 Pi

**原文链接**: [https://www.jeffgeerling.com/blog/2026/i-joined-the-ntp-pool/](https://www.jeffgeerling.com/blog/2026/i-joined-the-ntp-pool/)

生成摘要时出错

---

## 39. Canada recommits to federal funding for news

**原文标题**: Canada recommits to federal funding for news

**原文链接**: [https://www.niemanlab.org/2026/11/a-government-that-gets-it-canada-recommits-to-federal-funding-for-news/](https://www.niemanlab.org/2026/11/a-government-that-gets-it-canada-recommits-to-federal-funding-for-news/)

生成摘要时出错

---

## 40. A Better Vocabulary for Testing

**原文标题**: A Better Vocabulary for Testing

**原文链接**: [https://alperenkeles.com/posts/vocab-for-testing/](https://alperenkeles.com/posts/vocab-for-testing/)

生成摘要时出错

---

## 41. A miniature San Francisco with live buses, planes and boats

**原文标题**: A miniature San Francisco with live buses, planes and boats

**原文链接**: [https://smallsf.com/](https://smallsf.com/)

生成摘要时出错

---

## 42. U.N. Climate Talks Collapse in a Bitter Clash over Fossil Fuels

**原文标题**: U.N. Climate Talks Collapse in a Bitter Clash over Fossil Fuels

**原文链接**: [https://www.nytimes.com/2026/11/22/climate/cop31-climate-summit-ends-climate.html](https://www.nytimes.com/2026/11/22/climate/cop31-climate-summit-ends-climate.html)

生成摘要时出错

---

## 43. AI Supply Chain Security: What Canary Tokens Found

**原文标题**: AI Supply Chain Security: What Canary Tokens Found

**原文链接**: [https://www.dragos.com/blog/ai-supply-chain-security-canary-tokens](https://www.dragos.com/blog/ai-supply-chain-security-canary-tokens)

生成摘要时出错

---

## 44. AI is becoming a disaster for the climate

**原文标题**: AI is becoming a disaster for the climate

**原文链接**: [https://www.bloodinthemachine.com/p/ai-is-becoming-a-disaster-for-the](https://www.bloodinthemachine.com/p/ai-is-becoming-a-disaster-for-the)

生成摘要时出错

---

## 45. Notes on the discrete Fourier transform (DFT)

**原文标题**: Notes on the discrete Fourier transform (DFT)

**原文链接**: [https://eli.thegreenplace.net/2026/notes-on-the-discrete-fourier-transform-dft/](https://eli.thegreenplace.net/2026/notes-on-the-discrete-fourier-transform-dft/)

生成摘要时出错

---

## 46. Adult-only households accounted for 55% of toy sales in the first half of 2026

**原文标题**: Adult-only households accounted for 55% of toy sales in the first half of 2026

**原文链接**: [https://www.bloomberg.com/news/articles/2026-11-18/jellycats-squishmallows-and-lego-sets-for-adults-drive-holiday-traffic](https://www.bloomberg.com/news/articles/2026-11-18/jellycats-squishmallows-and-lego-sets-for-adults-drive-holiday-traffic)

生成摘要时出错

---

## 47. Harsher on Male? Evaluating LLMs on Gender-Asymmetric Moral Framing in Conflicts

**原文标题**: Harsher on Male? Evaluating LLMs on Gender-Asymmetric Moral Framing in Conflicts

**原文链接**: [https://arxiv.org/abs/2606.14068](https://arxiv.org/abs/2606.14068)

生成摘要时出错

---

## 48. All Delta Flights Through Atlanta Delayed as Automated System Falters

**原文标题**: All Delta Flights Through Atlanta Delayed as Automated System Falters

**原文链接**: [https://www.nytimes.com/2026/11/22/us/delta-flight-delays-system-outage.html](https://www.nytimes.com/2026/11/22/us/delta-flight-delays-system-outage.html)

生成摘要时出错

---

## 49. Progress map for the Lean formalization of Alessandro Masullo's manuscript

**原文标题**: Progress map for the Lean formalization of Alessandro Masullo's manuscript

**原文链接**: [https://claude.ai/artifact/CtQyX8qfYAF822bgHJHHE3](https://claude.ai/artifact/CtQyX8qfYAF822bgHJHHE3)

生成摘要时出错

---

## 50. Show HN: The Riemann Proof Handbook

**原文标题**: Show HN: The Riemann Proof Handbook

**原文链接**: [https://github.com/tamnd/riemann-handbook](https://github.com/tamnd/riemann-handbook)

生成摘要时出错

---

## 51. Nyx, the Oldest Internet Service Provider

**原文标题**: Nyx, the Oldest Internet Service Provider

**原文链接**: [https://nyx.net/](https://nyx.net/)

生成摘要时出错

---

## 52. Muru – AI-assisted Rust server for Python apps by mod_WSGI's creator

**原文标题**: Muru – AI-assisted Rust server for Python apps by mod_WSGI's creator

**原文链接**: [https://simonwillison.net/2026/Nov/21/muru/](https://simonwillison.net/2026/Nov/21/muru/)

生成摘要时出错

---

## 53. Agent swarm trying to solve P vs. NP

**原文标题**: Agent swarm trying to solve P vs. NP

**原文链接**: [https://pequalnp.com/](https://pequalnp.com/)

生成摘要时出错

---

## 54. Testing Terraform with AWS Emulator

**原文标题**: Testing Terraform with AWS Emulator

**原文链接**: [https://notes.hatedabamboo.me/terraform-tests-with-aws-emulator/](https://notes.hatedabamboo.me/terraform-tests-with-aws-emulator/)

生成摘要时出错

---

## 55. Uncontacted Indigenous people emerge from Amazon forest to ask for food

**原文标题**: Uncontacted Indigenous people emerge from Amazon forest to ask for food

**原文链接**: [https://www.washingtonpost.com/world/2026/11/19/uncontacted-indigenous-people-emerge-amazon-forest-ask-food/](https://www.washingtonpost.com/world/2026/11/19/uncontacted-indigenous-people-emerge-amazon-forest-ask-food/)

生成摘要时出错

---

## 56. Fascism and Monopoly (2020)

**原文标题**: Fascism and Monopoly (2020)

**原文链接**: [https://repository.law.umich.edu/mlr/vol118/iss7/2/](https://repository.law.umich.edu/mlr/vol118/iss7/2/)

生成摘要时出错

---

## 57. C++26 is done (again): November 2026 ISO C++ meeting trip report

**原文标题**: C++26 is done (again): November 2026 ISO C++ meeting trip report

**原文链接**: [https://herbsutter.com/2026/11/21/c26-is-done-again-trip-report-november-2026-iso-c-standards-meeting-buzios-brazil/](https://herbsutter.com/2026/11/21/c26-is-done-again-trip-report-november-2026-iso-c-standards-meeting-buzios-brazil/)

生成摘要时出错

---

## 58. Help github just deleted me

**原文标题**: Help github just deleted me

**原文链接**: [https://nate.mecca1.net/posts/2026-11-20_help/](https://nate.mecca1.net/posts/2026-11-20_help/)

生成摘要时出错

---

