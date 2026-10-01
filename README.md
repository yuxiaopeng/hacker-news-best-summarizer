# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-10-01.md)

*最后自动更新时间: 2026-10-01 23:28:18*
## 1. 双子星4号 氩

**原文标题**: Gemini 4 Argon

**原文链接**: [https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-argon/](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-argon/)

Google 推出了 Gemini 4 Argon，这是一款旨在为复杂、长期专业任务提供高级推理能力的新型前沿AI模型。Argon 最初通过 Fairwind 项目向受信任的网络安全防御者推出，其具有业界领先的100万个token限制，能够实现深度、多步骤的问题解决。

该模型在实际软件工程、企业知识工作（如法律和金融）以及网络安全防御方面展现了前沿性能。在内部，Google 将 Argon 用于量子算法优化、数据中心自主内存优化（预计节省 500 TiB 至 1 PiB）以及将大规模代码库从 C/C++ 迁移到 Rust。它在 DeepSWE v1.1 软件工程基准测试中创造了新的最先进水平，在经济影响方面领先 Vals 指数，在 AutomationBench 上排名第一，并在多模态视觉理解方面表现出色，在 LVBench 上取得了最先进的分数。

一个关键焦点是网络安全防御，Argon 可以在该领域自主发现、验证和修补关键漏洞。它已被 Wiz 等合作伙伴用于保护公共基础设施，并已发现之前模型遗漏的严重风险。Argon 在 CWE-bench v1 和内部渗透测试基准测试中表现强劲。

Google 正在采用分阶段发布方法，优先考虑安全性，实施了强大的防护措施以防止滥用（包括网络/CBRN 攻击）、提示注入攻击（在 Gray Swan IPI 上处于领先地位）和不对齐。它还配备了强化的沙盒环境以进行安全测试。Argon 最终将向开发者、企业和消费者开放，入门价为每百万输入 token 2 美元，每百万输出 token 10 美元。

---

## 2. Livenerf: Has Opus 5.5 been nerfed yet?

**原文标题**: Livenerf: Has Opus 5.5 been nerfed yet?

**原文链接**: [https://github.com/ninjahawk/livenerf](https://github.com/ninjahawk/livenerf)

Livenerf is a deterministic benchmark designed to detect if frontier models, specifically Anthropic's Claude Opus 5.5, are quietly "nerfed" (degraded) after launch. Launched on 2026-09-22, Livenerf began tracking Opus 5.5's performance on 2026-09-24 to establish a day-0 baseline, aiming to provide empirical data against speculative "nerf" reports.

The benchmark employs a highly controlled methodology: frozen prompts, pinned CLI versions, and exact graders ensure determinism everywhere except the model's stochastic output. It measures statistical drift over thousands of samples, built on the Inspect framework and using Anthropic's own error bar statistics. To maximize informational value, Livenerf focuses on 78 questions from datasets like GPQA and MMLU-Pro that Opus 5.5 only "sometimes" gets right.

Crucially, Livenerf measures Opus 5.5 as served through a Claude Max subscription via Claude Code, reflecting the path where "nerf" reports are most common. It tracks both accuracy and output token count, with the latter serving as an early indicator of "lower effort." A control arm, running Claude Opus 5, helps differentiate model changes from harness or platform issues.

The project operates under a pre-registered protocol for item selection, validation, and decision rules. A performance change is declared only if a 99% confidence interval excludes zero in two consecutive 10-day windows, the effect is at least 3 points, and the control arm shows no similar movement. As of 2026-10-01, 8 of the 30 baseline days have been collected. Livenerf will publish a running 10-day table showing Opus 5.5's performance relative to its launch-week baseline, reporting both improvements and regressions.

---

## 3. 你说没有MCP

**原文标题**: You said no MCP

**原文链接**: [https://earendil.com/posts/you-said-no-mcp/](https://earendil.com/posts/you-said-no-mcp/)

生成摘要时出错

---

## 4. 派 1.0

**原文标题**: Pi 1.0

**原文链接**: [https://earendil.com/posts/pi-1-0/](https://earendil.com/posts/pi-1-0/)

2026年10月1日，厄伦迪尔宣布发布 Pi 1.0，标志着其强化、极简且可扩展的代理框架迎来了重大演进。Pi 1.0 汇集了用户反馈，并致力于只采用经过验证的稳定功能，在保持其核心特性的同时增强了功能。

Pi 1.0 的主要新增功能包括对 Codemode 的原生支持（整合了 MCP、Jev 和图像模型）、对虚拟模型的扩展支持、延迟工具加载、Anthropic 模型的缓存预热，以及用于动态提示和工具更改的会话中系统消息。此次更新还带来了全新的 TUI 主题和默认全屏模式。

除了 Pi 1.0，厄伦迪尔还推出了 Pi Durable，一个实验性软件包，旨在构建长期运行的代理应用程序。Pi Durable 扩展了 Pi 的极简主义和超可塑性原则，为超越传统编码代理和终端使用的任务提供更强的持久性和控制力。

Pi 1.0 和 Pi Durable 均采用 MIT 许可证。Pi 1.0 可通过 `curl` 或 `powershell` 脚本获取，而 Pi Durable 可通过 `npm` 安装。厄伦迪尔强调其使命是通过开放软件和协议赋能人类能动性。文档可在 pi.dev 查阅，代码托管在 GitHub 上。

---

## 5. September 2026: The world today, as seen by one Polish guy

**原文标题**: September 2026: The world today, as seen by one Polish guy

**原文链接**: [https://tomwojcik.com/posts/2026-09-21/september-2026-the-world-today/](https://tomwojcik.com/posts/2026-09-21/september-2026-the-world-today/)

生成摘要时出错

---

## 6. StreetComplete iOS 版现已推出公开测试版

**原文标题**: StreetComplete on iOS is now in public beta

**原文链接**: [https://github.com/streetcomplete/StreetComplete/issues/5421](https://github.com/streetcomplete/StreetComplete/issues/5421)

StreetComplete，一款流行的OpenStreetMap编辑器，现已推出iOS公开测试版，标志着其跨平台开发迈出了重要一步。这项在“iOS - Testing! :-D #5421”下追踪的工作，旨在通过多平台方法将该应用引入苹果设备。

该项目利用Kotlin Multiplatform，将应用现有的100% Kotlin代码库进行转译。对于用户界面，正在使用Compose Multiplatform（目前处于iOS的alpha/beta测试阶段），它是Jetpack Compose的扩展。这一策略使得开发团队能够维护单一代码库，相比于将应用用Dart重写用于Flutter等替代方案，大幅减少了未来的维护开销。用户界面最初是Android XML，现在正逐步迁移到Compose Multiplatform。

开发工作于2023年12月启动，取代了早期的研究工单。目前迁移工作已完成约50%，预计还需要一人年的工作量才能完全移植。由于项目范围庞大，它严重依赖社区贡献。鼓励用户通过处理项目看板上的任务、熟悉Jetpack Compose/Compose Multiplatform、赞助开发或协助日常维护和问题分类来提供帮助。

---

## 7. 新加坡政府约会应用采用盖尔-沙普利稳定婚姻算法

**原文标题**: Singapore govt dating app uses Gale-Shapley stable marriage algorithm

**原文链接**: [https://twitter.com/tuakdotsol/status/2105105417760391258](https://twitter.com/tuakdotsol/status/2105105417760391258)

新加坡政府为年龄介于21至35岁的公务员推出了一款名为“FirstDate”的试点约会应用。这款应用旨在通过促成成功的配对来帮助用户“脱单”，从而独特地让用户不再需要使用该平台，这与商业约会应用形成了鲜明对比。

FirstDate采用了1962年提出的盖尔-沙普利稳定匹配算法，该算法曾荣获诺贝尔经济学奖（2012年），并被应用于医院实习生匹配和肾脏交换等领域。这种算法确保了数学上的稳定配对：用户创建偏好排名列表，提议者向他们的首选发出提议，接收者则保留他们收到的最佳提议，直到达成一个稳定的结果。这使得任何两个人都不可能互相喜欢却最终被分配给非彼此的对象。

该应用的用户体验特点包括：每个周期只提供一个匹配对象、没有无限滚动、72小时的决策窗口，以及只有在双方互相接受后才会显示联系方式。Singpass验证确保了用户身份的真实性。尽管盖尔-沙普利算法会产生对提议者最优的结果（提议者获得他们最佳的稳定匹配，而接收者获得他们最差的稳定匹配），但这种由国家支持、博弈论驱动的方法旨在挑战约会应用的自由市场模式。

---

## 8. The AI Race Just Got Awkward

**原文标题**: The AI Race Just Got Awkward

**原文链接**: [https://insufferable.dev/posts/the-ai-race-just-got-awkward/](https://insufferable.dev/posts/the-ai-race-just-got-awkward/)

The article challenges the prevailing narrative of Chinese labs merely "distilling" Western AI models, arguing that the dynamic has shifted. It suggests Western companies are now "adopting" significant advances from Chinese labs, who are openly sharing their "recipes."

A prime example is DeepSeek's "mind-blowing" KV cache optimizations. Driven by constraints on advanced GPUs, Chinese labs prioritized performance, developing innovations like DeepSeek-V4.1-Flash, which drastically reduced KV cache memory footprint—by approximately 437x for certain long-context use cases, achieving 890 bytes per token. This is critical for serving long-context models, as VRAM for caching is a major cost.

The author claims that Western AI giants, including Anthropic (with Claude Opus 5.5) and OpenAI (with GPT-6.1 Sol), have silently released new models incorporating these breakthroughs. The quiet nature of these releases hints at embarrassment, but the impact is clear: stellar user reviews and sharp reductions in cache-read pricing (Opus 5.5 cut 60% versus Opus 5; GPT-6.1 Sol cut 80% versus GPT-5.6 Sol). These advancements have significantly improved inference margins for Western labs, essentially acting as a "lifeline" from Chinese research, though the author is puzzled by the Chinese labs' decision to freely share such valuable innovations.

---

## 9. Clef: Open-source decision models, and new RL fine-tuning platform

**原文标题**: Clef: Open-source decision models, and new RL fine-tuning platform

**原文链接**: [https://blog.cloudflare.com/clef-decision-models/](https://blog.cloudflare.com/clef-decision-models/)

生成摘要时出错

---

## 10. A brief history of the Bloomberg terminal

**原文标题**: A brief history of the Bloomberg terminal

**原文链接**: [https://spectrum.ieee.org/bloomberg-terminal](https://spectrum.ieee.org/bloomberg-terminal)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-10-01](output/hacker_news_summary_2026-10-01.md) |
| 2 | [2026-09-24](output/hacker_news_summary_2026-09-24.md) |
| 3 | [2026-09-29](output/hacker_news_summary_2026-09-29.md) |
| 4 | [2026-09-30](output/hacker_news_summary_2026-09-30.md) |
| 5 | [2026-09-27](output/hacker_news_summary_2026-09-27.md) |
| 6 | [2026-09-25](output/hacker_news_summary_2026-09-25.md) |
| 7 | [2026-09-21](output/hacker_news_summary_2026-09-21.md) |
| 8 | [2026-09-23](output/hacker_news_summary_2026-09-23.md) |
| 9 | [2026-09-20](output/hacker_news_summary_2026-09-20.md) |
| 10 | [2026-09-22](output/hacker_news_summary_2026-09-22.md) |
| 11 | [2026-09-19](output/hacker_news_summary_2026-09-19.md) |
| 12 | [2026-09-18](output/hacker_news_summary_2026-09-18.md) |
| 13 | [2026-09-13](output/hacker_news_summary_2026-09-13.md) |
| 14 | [2026-09-16](output/hacker_news_summary_2026-09-16.md) |
| 15 | [2026-09-14](output/hacker_news_summary_2026-09-14.md) |
| 16 | [2026-09-17](output/hacker_news_summary_2026-09-17.md) |
| 17 | [2026-09-15](output/hacker_news_summary_2026-09-15.md) |
| 18 | [2026-09-09](output/hacker_news_summary_2026-09-09.md) |
| 19 | [2026-09-10](output/hacker_news_summary_2026-09-10.md) |
| 20 | [2026-09-08](output/hacker_news_summary_2026-09-08.md) |
| 21 | [2026-09-07](output/hacker_news_summary_2026-09-07.md) |
| 22 | [2026-09-06](output/hacker_news_summary_2026-09-06.md) |
| 23 | [2026-09-11](output/hacker_news_summary_2026-09-11.md) |
| 24 | [2026-09-12](output/hacker_news_summary_2026-09-12.md) |
| 25 | [2026-09-03](output/hacker_news_summary_2026-09-03.md) |
| 26 | [2026-09-02](output/hacker_news_summary_2026-09-02.md) |
| 27 | [2026-08-31](output/hacker_news_summary_2026-08-31.md) |
| 28 | [2026-09-04](output/hacker_news_summary_2026-09-04.md) |
| 29 | [2026-09-05](output/hacker_news_summary_2026-09-05.md) |
| 30 | [2026-09-01](output/hacker_news_summary_2026-09-01.md) |
| 31 | [2026-08-29](output/hacker_news_summary_2026-08-29.md) |
| 32 | [2026-08-30](output/hacker_news_summary_2026-08-30.md) |
| 33 | [2026-08-22](output/hacker_news_summary_2026-08-22.md) |
| 34 | [2026-08-25](output/hacker_news_summary_2026-08-25.md) |
| 35 | [2026-08-20](output/hacker_news_summary_2026-08-20.md) |
| 36 | [2026-08-28](output/hacker_news_summary_2026-08-28.md) |
| 37 | [2026-08-23](output/hacker_news_summary_2026-08-23.md) |
| 38 | [2026-08-21](output/hacker_news_summary_2026-08-21.md) |
| 39 | [2026-08-24](output/hacker_news_summary_2026-08-24.md) |
| 40 | [2026-08-26](output/hacker_news_summary_2026-08-26.md) |
| 41 | [2026-08-14](output/hacker_news_summary_2026-08-14.md) |
| 42 | [2026-08-19](output/hacker_news_summary_2026-08-19.md) |
| 43 | [2026-08-16](output/hacker_news_summary_2026-08-16.md) |
| 44 | [2026-08-17](output/hacker_news_summary_2026-08-17.md) |
| 45 | [2026-08-18](output/hacker_news_summary_2026-08-18.md) |
| 46 | [2026-08-15](output/hacker_news_summary_2026-08-15.md) |
| 47 | [2026-08-13](output/hacker_news_summary_2026-08-13.md) |
| 48 | [2026-08-12](output/hacker_news_summary_2026-08-12.md) |
| 49 | [2026-08-11](output/hacker_news_summary_2026-08-11.md) |
| 50 | [2026-08-10](output/hacker_news_summary_2026-08-10.md) |
| 51 | [2026-08-09](output/hacker_news_summary_2026-08-09.md) |
| 52 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 53 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 54 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 55 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 56 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 57 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 58 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 59 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 60 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 61 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 62 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 63 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 64 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 65 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 66 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 67 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 68 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 69 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 70 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 71 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 72 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 73 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 74 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 75 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 76 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 77 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 78 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 79 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 80 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 81 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 82 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 83 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 84 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 85 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 86 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 87 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 88 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 89 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 90 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 91 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 92 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 93 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 94 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 95 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 96 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 97 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 98 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 99 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 100 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 101 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 102 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 103 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 104 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 105 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 106 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 107 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 108 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 109 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 110 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 111 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 112 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 113 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 114 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 115 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 116 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 117 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 118 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 119 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 120 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 121 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 122 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 123 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 124 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 125 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 126 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 127 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 128 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 129 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 130 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 131 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 132 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 133 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 134 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 135 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 136 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 137 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 138 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 139 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 140 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 141 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 142 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 143 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 144 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 145 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 146 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 147 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 148 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 149 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 150 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 151 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 152 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 153 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 154 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 155 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 156 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 157 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 158 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 159 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 160 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 161 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 162 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 163 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 164 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 165 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 166 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 167 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 168 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 169 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 170 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 171 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 172 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 173 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 174 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 175 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 176 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 177 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 178 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 179 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 180 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 181 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 182 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 183 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 184 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 185 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 186 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 187 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 188 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 189 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 190 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 191 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 192 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 193 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 194 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 195 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 196 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 197 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 198 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 199 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 200 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 201 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 202 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 203 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 204 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 205 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 206 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 207 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 208 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 209 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 210 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 211 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 212 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 213 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 214 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 215 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 216 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 217 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 218 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 219 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 220 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 221 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 222 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 223 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 224 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 225 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 226 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 227 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 228 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 229 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 230 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 231 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 232 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 233 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 234 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 235 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 236 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 237 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 238 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 239 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 240 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 241 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 242 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 243 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 244 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 245 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 246 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 247 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 248 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 249 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 250 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 251 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 252 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 253 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 254 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 255 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 256 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 257 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 258 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 259 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 260 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 261 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 262 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 263 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 264 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 265 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 266 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 267 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 268 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 269 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 270 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 271 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 272 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 273 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 274 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 275 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 276 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 277 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 278 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 279 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 280 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 281 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 282 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 283 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 284 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 285 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 286 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 287 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 288 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 289 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 290 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 291 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 292 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 293 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 294 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 295 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 296 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 297 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 298 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 299 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 300 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 301 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 302 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 303 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 304 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 305 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 306 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 307 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 308 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 309 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 310 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 311 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 312 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 313 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 314 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 315 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 316 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 317 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 318 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 319 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 320 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 321 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 322 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 323 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 324 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
