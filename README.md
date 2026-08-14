# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-08-14.md)

*最后自动更新时间: 2026-08-14 20:12:32*
## 1. GLM-5.3：具有涌现网络能力的前沿编程

**原文标题**: GLM-5.3: Frontier coding with emergent cyber capabilities

**原文链接**: [https://z.ai/blog/glm-5.3](https://z.ai/blog/glm-5.3)

GLM-5.3 是 Z.ai 最新的 AI 模型，标志着在前沿编码和软件开发方面取得了重大进展。它在多种编程语言中展现出更强的熟练度，能够生成高效、安全、健壮的代码，并在调试、重构和优化方面表现出色。

一个主要亮点是其“涌现的网络能力”，这些能力源于它对代码结构、系统交互和潜在漏洞的深刻理解。尽管并非明确设计用于攻击性操作，GLM-5.3 能够识别传统工具常常难以发现的细微安全缺陷，例如缓冲区溢出和注入漏洞。从概念上讲，它还可以帮助理解攻击面和制作漏洞利用程序。

然而，文章强烈强调其预期的防御性应用。这些应用包括自动化补丁生成、安全加固、威胁情报分析，以及通过快速理解恶意软件和受损系统来实现的快速事件响应。该模型采用了增强型 Transformer 架构，并在包含代码、技术文档和安全公告在内的海量数据集上进行了训练。Z.ai 强调其对伦理 AI 的承诺，实施了严格的防护措施和红队演练以减轻潜在的滥用，确保 GLM-5.3 主要用于增强全球数字安全，而非助长恶意活动。

---

## 2. 杰米尼 3.7 刷机

**原文标题**: Gemini 3.7 Flash

**原文链接**: [https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-3-7-flash/](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-3-7-flash/)

2026年8月13日，谷歌推出了Gemini 3.7 Flash，并将其定位为最智能的代码编写和智能体主力模型。距离3.6 Flash发布仅三周，这次更新在多个领域带来了显著改进，且成本仅为原3.6 Flash的一半。

Gemini 3.7 Flash在调试和代码准确性等软件工程任务中表现出显著提升，在FrontierCode 1.1 Main（43.6% vs 34.4%）和DeepSWE v1.1（65.3% vs 49.0%）等基准测试中，它显著优于3.6 Flash。对于网页开发，它能生成功能更完善的布局和功能齐全的应用程序，在Arena.ai的WebDev Arena中，其Elo评分为1588（3.6 Flash为1538）。在金融和法律等知识密集型领域，它提供了更高的推理和准确性，在GDP.pdf上得分34.0%（22.0%），在AutomationBench上得分30.4%（17.0%）。

该模型还通过更好地适应障碍、更清晰的意图和更严谨的多步规划，提升了开发者体验。其引入价格为每百万输入tokens 0.75美元，每百万输出tokens 3.75美元。

Gemini 3.7 Flash已集成到Gemini Spark中，供Google AI Pro和Ultra订阅用户使用，从而增强了个人AI智能体在知识工作和Google Workspace应用中的能力。该模型在设计时考虑了安全性，包含了更新的防护措施，以防止在化学、生物、放射性、核（CBRN）以及网络攻击领域的滥用。开发者可通过Google Antigravity或Gemini API访问它。

---

## 3. DeepSeek 驾驭 开发者预览版

**原文标题**: DeepSeek Harness developer preview

**原文链接**: [https://deepseek.com/harness/en/](https://deepseek.com/harness/en/)

DeepSeek Harness 现已推出开发者预览版，作为一款开源的智能体框架，它强调两个核心原则：“一切皆插件”和“每次运行皆可追溯”。

DeepSeek Harness 基于 Cordis 插件系统构建，将智能体的每个能力（包括模型、工具、技能、会话、沙盒、存储、循环、调度和用户界面）都转化为可互换、可重组的插件。这种模块化架构允许开发者通过配置选择、更换或扩展任何组件，而无需修改核心源代码。该框架为智能体提供了与环境交互、利用工具并在真实世界环境中有效运行的关键功能。

一个关键特性是全面的运行可追溯性。所有模型交互，例如系统提示、推理、工具调用、结果和上下文注入，都会记录在只追加的会话日志中。这使得可以通过“轨迹”视图进行详细检查，提供恢复、分支、搜索和重放过去运行的能力。

DeepSeek Harness 提供多种运行时模式：
*   **标准模式：** 一个功能完备的编码智能体，包含文件编辑、shell、搜索、技能和子智能体等大量工具。
*   **代码模式：** 在标准模式的基础上扩展，允许模型通过 SDK 使用 TypeScript 程序来编排多步骤操作。
*   **最小模式：** 一个精简的环境，仅包含 shell 工具和文件编辑器，用于模型基准测试。
*   **创建者模式：** 专为构建自定义智能体预设而设计，提供运行时检查和插件实验功能。

开发者可以通过 `npx` 启动 Web UI 或从 GitHub 克隆源代码来快速上手。DeepSeek Harness 是一个处于开发者预览阶段的不断发展的平台，旨在为 AI 开发构建可复用、可组合的开源基础设施。

---

## 4. 加速 GPT-5.6 Sol 超快

**原文标题**: Accelerating GPT-5.6 Sol Ultrafast

**原文链接**: [https://www.cerebras.ai/blog/accelerating-gpt-5-6-sol-ultrafast-with-openai](https://www.cerebras.ai/blog/accelerating-gpt-5-6-sol-ultrafast-with-openai)

2026年8月13日，Cerebras 和 OpenAI 宣布为 GPT-5.6 Sol 推出“超高速模式”，这是一种由 Cerebras 晶圆级引擎架构提供支持的新服务层级。该模式承诺每秒输出高达750个token，同时不牺牲质量，从而解决了AI速度和智能之间的传统权衡。

超高速模式最初仅对精选客户开放，访问权限将随着时间推移逐步扩大。基准测试显示出显著的性能提升：GPT-5.6 Sol 超高速模式的运行速度比 Fable 5 快11倍，比 Opus 4.8 快5倍。在“人类的最后一考”（2,500个博士级别问题）中，超高速模式在11小时11分钟内完成了测试，比 Claude Fable 5 (78小时27分钟) 快了近7倍，并取得了相当的准确性。它还在具有经济价值的知识工作任务中实现了5.6倍的端到端加速。

这种加速推理将改变法律摘要、金融模型和工程报告等高风险应用。它使AI代理能够在关键路径上运行，从而促进对生产中断和网络攻击的快速响应，并通过提供实时洞察，显著提高研究人员和工程师的生产力。

超高速模式背后的突破性技术是 Cerebras 的晶圆级引擎，它消除了数据传输瓶颈。通过在每个晶圆大小的芯片上封装44 GB的SRAM，模型权重得以保留在芯片上，使token能够不间断地流动，并为前沿AI模型实现持续、高速的处理。

---

## 5. 意大利面化DRAM

**原文标题**: Spaghettifying DRAM

**原文链接**: [https://github.com/xoreaxeaxeax/skitter-creek-bath-salts](https://github.com/xoreaxeaxeax/skitter-creek-bath-salts)

“DRAM打乱”（skitter-creek-bath-salts）是一种针对AMD Family 16h CPU的漏洞攻击，它通过操纵内存层次结构的最深层来绕过平台安全机制。通过翻转DRAM控制器寄存器中的一个比特位，该项目在内存控制器（MCT/DCT）层重构物理地址转换，从而打乱实际的DRAM坐标。

这使得内存“打乱”（spaghettifies），意味着一个物理地址不再指向其在DRAM中预期的位置（即`&x != &x`）。由于所有CPU、固件和芯片组安全原语（例如平台安全处理器、系统管理模式、C6 DRAM和CPU微码保护）都建立在这些物理地址之上，它们因此变得无效。这种重映射暴露了原本不可见、受保护的DRAM区域。

该漏洞利用涉及一个快速、短暂的过程：临时修改DRAM控制器，快速从现在已“打乱”的内存位置获取数据，然后恢复原始映射。这需要精心的系统准备，包括禁用中断、预热缓存和TLB，以及序列化内存访问以维持系统稳定性。

为了重构新的、被打乱的内存布局，研究人员利用了线性代数。他们使用一个SMT求解器（z3）来推断未知的变换矩阵。这是通过在“一致”视图中将哨兵值插入已知内存位置，切换到“打乱”视图，定位哨兵的新“别名”地址，并使用这些（目标，别名）对来映射完整的线性变换来实现的。这允许计算任何受保护内存区域的别名，从而有效地“解锁了一切”。尽管该技术是在AMD Family 16h上开发的，但其底层原理适用于ARM和RISC-V等其他架构。

---

## 6. 每个他妈的网站 (2020)

**原文标题**: Every Fucking Website (2020)

**原文链接**: [https://lxe.github.io/everywebsite/](https://lxe.github.io/everywebsite/)

这篇题为《每个该死的网站 (2020)》的讽刺文章，猛烈抨击了新冠疫情时代网站上普遍存在、无处不在且常常令人沮丧的设计趋势和用户体验。作者幽默地指出了常见的烦恼，包括那些展示着从未阅读过的信息的显眼新冠疫情横幅；用户已经习以为常、提供折扣（例如“10PERCENTOFF”）的侵入式弹窗广告；以及那些令人困惑、常常带有政治色彩的标题（例如“特朗普2020！我讨厌小狗！”）。

文章重点关注了那些随处可见的Cookie同意声明横幅，作者将其描述为法律强制要求但对用户不友好的东西，并将它们的必要性和不一致的实施归咎于欧盟和加利福尼亚等地区的法规。这篇文章对这些标准化、常常无法跳过且集成度差的元素深感沮丧，暗示每个网站都采用了这些做法，最终导致了一种普遍存在、机械化且令人应接不暇的在线体验，其典型体现是最后出现的“您将与机器人聊天！”提示。

---

## 7. 为什么 Opus 5 用起来感觉更差？

**原文标题**: Why does Opus 5 feel worse to work with?

**原文链接**: [https://mun-logadan.github.io/why-does-opus-5-feel-worse/](https://mun-logadan.github.io/why-does-opus-5-feel-worse/)

文章指出，尽管Opus 5在基准测试中能力更优，但使用它却感觉像是一种倒退，相比Opus 4.7、4.8和Fable。主要抱怨是，当意图不明确时，Opus 5不会停下来询问澄清问题，不经核实就做出假设，未经允许就重新解读计划，因此需要“细致的看护”。相比而言，老模型更具协作性和谨慎性。

作者推测，这种行为源于前沿AI实验室中常见的两个因素：渴望打造能进行递归自举的自我改进型AI，以及在基准测试中获得高分的巨大压力。作者认为问题在于，基准测试会奖励那些在模糊不清的情况下做出“大胆、通常正确假设”的模型，同时惩罚那些寻求澄清的模型。

然而，对于像编码这样的真实世界任务，几乎不可能预先向AI提供所有必要的上下文、意图和约束。在这些模糊不清的情况下，用户更倾向于一个会停下来提问的代理，而不是做出假设或“凭最佳猜测行事”，尤其当涉及到现实生活中的后果时。文章总结道，现实生活中的任务与独立的基准测试根本不同，需要一个更谨慎、更善于沟通的AI。

---

## 8. Qwen 3.8 27B

**原文标题**: Qwen 3.8 27B

**原文链接**: [https://huggingface.co/Qwen/Qwen3.8-27B-FP8](https://huggingface.co/Qwen/Qwen3.8-27B-FP8)

生成摘要时出错

---

## 9. Codex in ChatGPT desktop app for Linux is now in preview

**原文标题**: Codex in ChatGPT desktop app for Linux is now in preview

**原文链接**: [https://community.openai.com/t/codex-in-chatgpt-desktop-app-for-linux-is-now-in-preview/1390027](https://community.openai.com/t/codex-in-chatgpt-desktop-app-for-linux-is-now-in-preview/1390027)

生成摘要时出错

---

## 10. Gloomberb

**原文标题**: Gloomberb

**原文链接**: [https://gloom.sh/](https://gloom.sh/)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-08-14](output/hacker_news_summary_2026-08-14.md) |
| 2 | [2026-08-09](output/hacker_news_summary_2026-08-09.md) |
| 3 | [2026-08-10](output/hacker_news_summary_2026-08-10.md) |
| 4 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 5 | [2026-08-11](output/hacker_news_summary_2026-08-11.md) |
| 6 | [2026-08-12](output/hacker_news_summary_2026-08-12.md) |
| 7 | [2026-08-13](output/hacker_news_summary_2026-08-13.md) |
| 8 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 9 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 10 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 11 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 12 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 13 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 14 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 15 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 16 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 17 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 18 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 19 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 20 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 21 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 22 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 23 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 24 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 25 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 26 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 27 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 28 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 29 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 30 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 31 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 32 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 33 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 34 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 35 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 36 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 37 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 38 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 39 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 40 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 41 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 42 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 43 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 44 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 45 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 46 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 47 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 48 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 49 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 50 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 51 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 52 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 53 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 54 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 55 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 56 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 57 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 58 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 59 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 60 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 61 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 62 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 63 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 64 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 65 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 66 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 67 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 68 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 69 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 70 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 71 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 72 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 73 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 74 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 75 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 76 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 77 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 78 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 79 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 80 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 81 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 82 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 83 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 84 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 85 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 86 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 87 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 88 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 89 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 90 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 91 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 92 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 93 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 94 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 95 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 96 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 97 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 98 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 99 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 100 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 101 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 102 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 103 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 104 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 105 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 106 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 107 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 108 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 109 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 110 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 111 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 112 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 113 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 114 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 115 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 116 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 117 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 118 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 119 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 120 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 121 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 122 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 123 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 124 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 125 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 126 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 127 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 128 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 129 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 130 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 131 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 132 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 133 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 134 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 135 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 136 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 137 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 138 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 139 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 140 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 141 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 142 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 143 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 144 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 145 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 146 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 147 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 148 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 149 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 150 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 151 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 152 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 153 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 154 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 155 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 156 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 157 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 158 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 159 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 160 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 161 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 162 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 163 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 164 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 165 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 166 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 167 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 168 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 169 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 170 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 171 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 172 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 173 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 174 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 175 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 176 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 177 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 178 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 179 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 180 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 181 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 182 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 183 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 184 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 185 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 186 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 187 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 188 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 189 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 190 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 191 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 192 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 193 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 194 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 195 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 196 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 197 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 198 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 199 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 200 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 201 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 202 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 203 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 204 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 205 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 206 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 207 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 208 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 209 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 210 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 211 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 212 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 213 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 214 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 215 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 216 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 217 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 218 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 219 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 220 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 221 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 222 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 223 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 224 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 225 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 226 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 227 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 228 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 229 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 230 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 231 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 232 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 233 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 234 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 235 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 236 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 237 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 238 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 239 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 240 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 241 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 242 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 243 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 244 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 245 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 246 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 247 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 248 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 249 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 250 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 251 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 252 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 253 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 254 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 255 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 256 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 257 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 258 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 259 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 260 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 261 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 262 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 263 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 264 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 265 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 266 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 267 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 268 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 269 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 270 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 271 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 272 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 273 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 274 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 275 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 276 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 277 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 278 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 279 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
