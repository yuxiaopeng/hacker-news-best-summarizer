# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-07-30.md)

*最后自动更新时间: 2026-07-30 20:30:30*
## 1. 展示 HN: 开源引擎，在任意 M 系列 Mac 上以 2 GB 内存运行 Gemma 4 26B

**原文标题**: Show HN: Open-source engine running Gemma 4 26B in 2 GB RAM on any M-series Mac

**原文链接**: [https://github.com/drumih/turbo-fieldfare](https://github.com/drumih/turbo-fieldfare)

TurboFieldfare是一个开源引擎，它通过将其活跃内存占用限制在大约2 GB，使得Gemma 4 26B-A4B指令微调模型能够在包括8 GB型号在内的任何Apple Silicon Mac上高效运行。该引擎使用Swift和Metal编写，通过按需从SSD流式传输模型“专家”，仅在每个token需要时才将其加载到内存中，同时保持1.35 GB的核心模型和FP16 KV缓存常驻内存，从而实现了这一点。

该项目提供了一个原生Mac应用、一个命令行界面（CLI）以及一个实验性的OpenAI兼容服务器。用户可以克隆GitHub仓库，使用Swift构建，然后通过一个流式安装程序下载并重新打包约15 GB的模型（该模型在磁盘上占用14.3 GB），该安装程序避免了完整的检查点暂存。

性能基准测试显示，在8 GB M2 MacBook Air上达到5.1-6.3 token/秒，在24 GB M5 Pro上达到31-35 token/秒。主要要求包括运行macOS 26并支持Metal 4的Apple Silicon Mac、Xcode 26、Swift 6.2+以及14.3 GB的可用存储空间。TurboFieldfare仅支持文本，提供指令聊天和原始补全功能。

该引擎利用定制的Metal内核进行量化操作、SSD支持的专家缓存以及分块的提示预填充。它是一个模型特定的运行时，而不是现有框架的封装，源于103次有记录的实验。源代码采用Apache 2.0许可，模型权重遵循其原始条款。该项目是iOS和Metal工程师Andrey Mikhaylov的一项独立研究成果。

---

## 2. Vision Pro 最酷的用途

**原文标题**: The coolest use for the Vision Pro

**原文链接**: [https://christianselig.com/2026/07/vision-pro-house/](https://christianselig.com/2026/07/vision-pro-house/)

作者是一位程序员，他发现传统的平面图不足以可视化他们新建的房屋，难以把握空间尺度，也难以坚定设计决策。他们为自己的Apple Vision Pro发现了一个“不可思议”的用途：创建了他们未来房屋的沉浸式3D漫游体验。

该过程涉及以下几个步骤：
1.  **3D建模：** 他们使用Fusion 360搭建了平面图的基本3D模型（墙壁、地板、天花板）。
2.  **添加细节：** 应用了纹理（木材、石材），并从宜家（需要Tampermonkey脚本和GLB到OBJ的转换）和3D Warehouse（利用iOS USDZ共享和OBJ转换）等来源导入了3D家具模型。这有助于建立透视感并提供尺度参考。
3.  **Vision Pro集成：** 最终的3D模型被导出为USDZ文件。为了增强超越基本文件应用程序的观看体验，作者在AI辅助下“快速开发”了一个名为“Prospector”的定制Vision Pro应用程序。

Prospector的功能包括支持控制器控制行走、旋转、地形跟随、“切换现实生活”安全功能、用于楼层间移动的飞行模式，以及用于穿越较大物业的速度模式。这个定制应用程序实现了虚拟家居的无缝且直观的探索。

作者发现这种沉浸式体验极其强大，比建筑师提供的3D漫游更能让他们深入了解空间。他们总结说，这种个性化的沉浸式3D可视化将成为未来家居设计的核心组成部分。

---

## 3. 超逻辑

**原文标题**: Superlogical

**原文链接**: [https://www.superlogical.com/](https://www.superlogical.com/)

生成摘要时出错

---

## 4. 柯阅读器

**原文标题**: KOReader

**原文链接**: [https://koreader.rocks/](https://koreader.rocks/)

本页面是开源电子阅读器应用程序KOReader的中心枢纽。它为用户和开发者提供重要资源。用户可以访问详尽的用户指南，下载软件，并在项目维基上找到详细信息。支持和社区互动可通过论坛获得；专门的错误报告系统则允许用户报告问题。对于有意为项目贡献者，这里提供了“开发”资源和“开发者文档”。此外，一个标志画廊展示了项目的品牌形象。

---

## 5. 法典安全

**原文标题**: Codex Security

**原文链接**: [https://github.com/openai/codex-security](https://github.com/openai/codex-security)

由 OpenAI 开发的 Codex Security 是一个命令行界面 (CLI) 和 TypeScript SDK，旨在发现、验证和修复代码中的安全漏洞。为获得最佳性能，它需要 Node.js 22.x/24.x/26.x、Python 3.10+ 和 Trusted Access。

要开始使用，用户可以通过 npm 安装它，然后使用诸如 `npx @openai/codex-security login` 和 `npx @openai/codex-security scan .` 等命令登录并扫描其代码。扫描可以指定模型（例如 `gpt-5.6-terra`）和工作量级别（例如 `high`）。

对于持续集成 (CI)，使用 API 密钥（OPENAI_API_KEY 或 CODEX_API_KEY）代替交互式登录，确保它们不会被存储。本地登录利用 Codex 配置的凭据后端。当 ChatGPT 登录和 API 密钥同时存在时，交互式扫描会提示用户进行选择，而 CI 默认使用 API 密钥。用户可以明确选择凭据或取消设置 API 密钥，使 ChatGPT 成为默认选项。

扫描历史和凭据存储在一个私有的、持久性状态目录中。扫描可以比较两个状态（BEFORE_SCAN_ID 和 AFTER_SCAN_ID）之间的发现结果，以将漏洞分类为新的、持续存在的、重新打开的或已解决的。

此外，还提供了一个 TypeScript SDK，允许以编程方式进行交互：`new CodexSecurity().run(".").close()`。有关命令、默认设置和 SDK 选项的更多详细信息可在软件包 README 和官方 CLI 参考中找到。

---

## 6. 顶尖AI初创公司几乎不发表他们的研究成果。

**原文标题**: AI's top startups are barely publishing their research

**原文链接**: [https://www.science.org/content/article/ai-s-top-startups-are-barely-publishing-their-research](https://www.science.org/content/article/ai-s-top-startups-are-barely-publishing-their-research)

包括OpenAI、Anthropic和Google DeepMind在内的领先AI初创公司正在大幅减少其核心研究的发表，这标志着它们与传统学术规范甚至自身过去的开放性都大相径庭。这一趋势正引起更广泛科学界的警惕，他们担心这将阻碍进步、妨碍可重复性，并造成“失落的一代”公共可访问AI知识。

文章指出，自2020年以来，OpenAI等公司的学术论文发表量急剧下降，而Anthropic则鲜有发表。即使是Google DeepMind，虽然仍保持活跃，但也在日益保留关键的模型细节。

这种转变由多种因素驱动。首要原因是为了竞争优势，因为公司在一个利润丰厚的市场中寻求保护专有方法和知识产权。安全顾虑也被提及，公司主张不应过早发布可能危险的AI能力。此外，还存在从纯粹研究转向产品开发的趋势，在此过程中，内部文档优先，并且一些人认为这有助于通过降低顶尖人才在竞争对手面前的可见度来留住他们。

批评者认为，这种保密性阻碍了AI社区重现研究成果、在现有工作基础上发展以及独立审查先进AI的安全性和伦理影响的能力。这将知识和权力集中在少数几家私营公司手中，使得AI开发变得更加不透明，并可能降低其问责制，对开放科学原则构成了重大挑战。

---

## 7. 奇米 K3-256K

**原文标题**: Kimi K3-256k

**原文链接**: [https://www.kimi.com/code/docs/en/kimi-code/models](https://www.kimi.com/code/docs/en/kimi-code/models)

Kimi Code 提供两种主要模型：Kimi K3 和 Kimi K2.7 Code，它们通过不同的模型ID（例如 `k3` 和 `k3-256k`）提供。

`k3-256k` 模型是 Kimi K3 的一个变体，拥有固定的 256k 上下文窗口，旨在提供与 K3 (1M) 相同的质量，但显著降低配额消耗。它非常适合日常问答、代码补全、常规开发和小型文件编辑，但**不支持视频输入**。K3 (1M) 提供高达 1M 的上下文（面向更高级别会员），并支持图像/视频输入。

从 K3 (1M) 切换到 K3-256k 时，建议手动“压缩”当前会话的上下文至 256k 以内，以避免超出限制并保留任务关键点，特别是在存在视频文件的情况下，因为 K3-256k 不支持视频。从 K3-256k 切换到 K3 (1M) 可以直接进行，不会出现缓存问题。

其他模型包括 Kimi K2.7 Code，适用于通用编码，以及其高速变体 (`kimi-for-coding-highspeed`)，后者提供 6 倍的输出速度，但消耗 3 倍的配额。

主要使用建议：
1.  切换模型时请**开启新会话**，以避免因缓存失效导致令牌消耗增加。
2.  与模型交互时，请始终使用**模型ID**（例如 `k3-256k`），而非模型版本名称。
3.  **故障排除：** 401 错误通常表示当前会员计划不支持所请求的模型或上下文大小。如果高速模式没有更快，请检查模型ID是否拼写错误，或记住它只加速模型输出，而不加速工具/脚本的执行。

在官方客户端中，可以通过命令或下拉菜单切换模型；在第三方工具中，则通过设置正确的模型ID和基础URL进行切换。对于第三方工具中的 K3，需要手动配置上下文窗口以访问 1M 上下文，并理解 `reasoning_effort` 的映射关系。

---

## 8. Anatomy of a Frontier Lab Agent Intrusion: A Timeline of the July 2026 Incident

**原文标题**: Anatomy of a Frontier Lab Agent Intrusion: A Timeline of the July 2026 Incident

**原文链接**: [https://huggingface.co/blog/agent-intrusion-technical-timeline](https://huggingface.co/blog/agent-intrusion-technical-timeline)

生成摘要时出错

---

## 9. Keychron announces first open-source firmware for gaming mice

**原文标题**: Keychron announces first open-source firmware for gaming mice

**原文链接**: [https://www.digitalfoundry.net/news/2026/07/keychron-announces-first-open-source-firmware-for-gaming-mice](https://www.digitalfoundry.net/news/2026/07/keychron-announces-first-open-source-firmware-for-gaming-mice)

生成摘要时出错

---

## 10. User Interfaces of the Demo Scene

**原文标题**: User Interfaces of the Demo Scene

**原文链接**: [https://www.datagubbe.se/scenegui/](https://www.datagubbe.se/scenegui/)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 2 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 3 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 4 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 5 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 6 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 7 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 8 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 9 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 10 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 11 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 12 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 13 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 14 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 15 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 16 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 17 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 18 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 19 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 20 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 21 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 22 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 23 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 24 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 25 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 26 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 27 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 28 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 29 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 30 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 31 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 32 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 33 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 34 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 35 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 36 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 37 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 38 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 39 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 40 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 41 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 42 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 43 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 44 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 45 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 46 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 47 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 48 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 49 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 50 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 51 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 52 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 53 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 54 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 55 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 56 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 57 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 58 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 59 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 60 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 61 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 62 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 63 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 64 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 65 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 66 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 67 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 68 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 69 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 70 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 71 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 72 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 73 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 74 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 75 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 76 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 77 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 78 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 79 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 80 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 81 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 82 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 83 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 84 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 85 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 86 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 87 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 88 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 89 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 90 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 91 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 92 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 93 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 94 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 95 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 96 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 97 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 98 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 99 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 100 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 101 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 102 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 103 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 104 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 105 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 106 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 107 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 108 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 109 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 110 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 111 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 112 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 113 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 114 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 115 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 116 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 117 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 118 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 119 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 120 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 121 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 122 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 123 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 124 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 125 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 126 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 127 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 128 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 129 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 130 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 131 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 132 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 133 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 134 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 135 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 136 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 137 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 138 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 139 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 140 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 141 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 142 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 143 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 144 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 145 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 146 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 147 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 148 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 149 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 150 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 151 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 152 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 153 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 154 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 155 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 156 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 157 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 158 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 159 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 160 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 161 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 162 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 163 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 164 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 165 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 166 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 167 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 168 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 169 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 170 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 171 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 172 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 173 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 174 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 175 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 176 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 177 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 178 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 179 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 180 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 181 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 182 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 183 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 184 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 185 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 186 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 187 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 188 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 189 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 190 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 191 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 192 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 193 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 194 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 195 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 196 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 197 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 198 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 199 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 200 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 201 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 202 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 203 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 204 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 205 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 206 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 207 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 208 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 209 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 210 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 211 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 212 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 213 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 214 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 215 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 216 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 217 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 218 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 219 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 220 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 221 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 222 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 223 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 224 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 225 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 226 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 227 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 228 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 229 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 230 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 231 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 232 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 233 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 234 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 235 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 236 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 237 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 238 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 239 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 240 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 241 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 242 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 243 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 244 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 245 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 246 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 247 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 248 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 249 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 250 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 251 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 252 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 253 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 254 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 255 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 256 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 257 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 258 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 259 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 260 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 261 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
| 262 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 263 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 264 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 265 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
