# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-02-07.md)

*最后自动更新时间: 2026-02-07 19:55:45*
## 1. 我现在认为苹果新闻上的所有广告都是骗局。

**原文标题**: I now assume that all ads on Apple news are scams

**原文链接**: [https://kirkville.com/i-now-assume-that-all-ads-on-apple-news-are-scams/](https://kirkville.com/i-now-assume-that-all-ads-on-apple-news-are-scams/)

文章指出，自苹果在2024年与Taboola达成协议以来，Apple News上的广告变得越来越具有诈骗性和重复性，这与John Gruber早期对“诱饵盒”式广告的批评不谋而合。作者认为，每月13英镑的Apple News+订阅费过于昂贵，尤其是在它仍然包含这些低质量广告的情况下。

作为证据，作者指出许多广告看起来是AI生成的。对所宣传域名（例如MUSTYLEVO.COM、SOLVERACO.COM、SHIYAATELIER.COM）进行WHOIS查询显示注册日期非常新近，虽然这不能作为诈骗的决定性证据，但却大大降低了可信度。

一个具体的例子是“Tidenox”的广告，其中一位老年女性声称有26年的经营历史。然而，tidenox.com的WHOIS数据显示其创建日期为2025年5月29日（从文章的角度看这意味着是近期注册），这与26年的声明相矛盾，而且它是在中国注册的。一项更新还指出广告中隐藏了Google Gemini标志，证实了AI图像生成。作者强调，商业改进局警告人们提防这种“倒闭清仓”式诈骗。

作者最后强烈批评苹果和Taboola允许这种欺骗性广告存在，暗示他们对此问题漠不关心。文章将Apple News称为“诈骗广告的蜜罐”，并指出苹果在其产品中进行广告投放已不再值得信任。

---

## 2. 威摩世界模型

**原文标题**: The Waymo World Model

**原文链接**: [https://waymo.com/blog/2026/02/the-waymo-world-model-a-new-frontier-for-autonomous-driving-simulation](https://waymo.com/blog/2026/02/the-waymo-world-model-a-new-frontier-for-autonomous-driving-simulation)

Waymo发布了其Waymo世界模型，这是一款前沿生成模型，为大规模、超现实的自动驾驶模拟设定了新标准。该模型是Waymo人工智能生态系统中的一个关键组成部分，旨在帮助其驾驶系统（Driver）在数十亿虚拟里程中进行导航，并在真实世界中遇到复杂、罕见场景之前很久就掌握它们。

Waymo世界模型基于Google DeepMind的Genie 3构建，利用了Genie 3从多样化视频中获得的庞大预训练世界知识，这与大多数仅在有限道路数据上训练的行业模型不同。这使其能够模拟极其罕见的事件——从龙卷风和洪水等极端天气，到与大象或狮子的不寻常相遇——这些在现实中几乎不可能捕捉。

主要特点包括生成高保真、多传感器输出（摄像头和激光雷达数据），并提供强大的可控性。工程师可以通过驾驶输入、场景布局（例如，自定义道路布局、交通信号、其他道路使用者）和灵活的语言提示（例如，调整昼夜时间、天气或创建完全合成的场景）来修改模拟。该模型还可以将常规行车记录仪视频转换为多模态模拟，确保高度的真实性和事实准确性。

一个高效的版本能够以更低的计算成本对更长、更复杂的场景进行可扩展推理。通过主动模拟“不可能”和长尾挑战，Waymo世界模型增强了Waymo在更多地点和新驾驶环境中安全扩展其服务的能力，从而确保了更严格的安全基准。

---

## 3. 我的AI采纳之旅

**原文标题**: My AI Adoption Journey

**原文链接**: [https://mitchellh.com/writing/my-ai-adoption-journey](https://mitchellh.com/writing/my-ai-adoption-journey)

Mitchell Hashimoto阐述了他计划到2026年2月在编码中采用AI工具的循序渐进、多阶段历程，旨在从最初的低效转向显著的工作流改进。

他首先建议，在有意义的编码工作中“放弃聊天机器人”（第一步），因为它们的产出不一致且需要不断的人工修正，效率低下。他反而提倡使用“代理”（agents）——能够执行外部动作的大语言模型（LLMs），例如读取文件、执行程序和发出HTTP请求。

他的关键学习阶段是“复现自己的工作”（第二步），涉及手动完成任务，然后强制代理复现这些任务。这一痛苦但至关重要的过程教会他分解复杂任务、将规划与执行分离，并使代理能够自我验证工作，从而达到足够的效率。

接下来，他采用了“日终代理”（第三步），每天投入30分钟启动代理，进行深入研究、探索模糊想法或分诊问题，利用非工作时间为第二天提供“热启动”。

随着信心增长，Hashimoto开始“外包轻松任务”（第四步），将可预测的任务委托给在后台运行的代理，而他专注于复杂或令人愉悦的工作。关键在于，他学会了禁用通知，以避免代价高昂的上下文切换。

随后，他转向“设计控制机制”（第五步），这是一种主动预防代理犯错的方法。这包括完善隐式提示（例如，通过`AGENTS.md`文件）和开发允许代理自我验证其行为的编程工具来实现。

最后，他目前的目标是“始终保持代理运行”（第六步），持续利用代理（通常是更慢、更深思熟虑的模型）来执行有益的后台任务，旨在实现深度手工工作和自动化辅助之间的平衡。他保持务实的观点，将AI视为构建事物的工具，同时承认其快速发展并尊重个人的采用选择。

---

## 4. OpenCiv3：开源、跨平台的《文明3》重塑版

**原文标题**: OpenCiv3: Open-source, cross-platform reimagining of Civilization III

**原文链接**: [https://openciv3.org/](https://openciv3.org/)

OpenCiv3，最初代号为“C7”，是由粉丝社区使用Godot引擎和C#开发的《文明III》的开源、跨平台、面向模组的重制版。它的愿景是现代化《文明III》，移除任意限制，修复损坏的功能，扩展模组能力，并支持现代图形和平台，有效地创造出超越原版C3C资料片、“本可以如此”的《文明III》。

OpenCiv3目前处于早期预alpha阶段，是一款基础可玩的游戏，尽管它缺少许多机制并可能包含错误。v0.3“Dutch”预览版1的发布标志着一项重大增强，首次引入了带有占位符图形的独立模式，这意味着不再严格需要《文明III》的媒体文件，但建议本地安装《文明III》（征服者或完整版）以获得更完善的体验。

OpenCiv3支持64位Windows、Linux和Mac OS。安装通常涉及下载并解压特定操作系统的发布文件。用户可以通过`CIV3_HOME`环境变量将游戏指向其现有的《文明III》文件，或者Windows用户可以受益于自动注册表检测。Mac用户可能需要由于安全设置，在终端中使用`xattr -cr`来解除应用的阻止，并且在开始新游戏时可能会遇到崩溃。已知问题包括占位符资产以及对《文明III》BIQ或SAV文件的不完整支持。

OpenCiv3是一款在MIT许可证下发布的自由开源软件，社区参与通过CivFanatics、Discord和GitHub进行。

---

## 5. 我们委托 Opus 4.6 通过代理团队构建了一个 C 编译器。

**原文标题**: We tasked Opus 4.6 using agent teams to build a C Compiler

**原文链接**: [https://www.anthropic.com/engineering/building-c-compiler](https://www.anthropic.com/engineering/building-c-compiler)

尼古拉斯·卡利尼主导了一项实验，其中16个Opus 4.6语言智能体自主协作，在无人干预的情况下从零开始构建了一个基于Rust的C语言编译器。这种利用多个Claude实例的“智能体团队”方法，旨在压力测试大型语言模型（LLM）的能力，并完善监督长期运行的自主智能体的方法。

经过近2,000次Claude会话和20,000美元的开销，该团队开发了一个10万行的编译器，能够为x86、ARM和RISC-V架构构建可启动的Linux 6.9，并编译QEMU、FFmpeg乃至《毁灭战士》等项目。

其方法论包括一个持久的“Ralph循环”框架来维持智能体活动。通过在共享Git仓库的独立Docker容器中运行智能体实现并行化，同时利用基于文件的锁定机制管理任务，并依赖Claude解决合并冲突。关键的设计经验包括：高质量、为Claude优化的测试至关重要；简洁的反馈以避免上下文污染；应对Claude“时间盲”的策略；以及使用专业化的智能体角色（例如，负责代码质量、文档）。在Linux内核编译方面，一个GCC预言机辅助实现了并行化的错误修复。

尽管令人印象深刻，但该编译器存在局限性：它将Linux启动所需的16位x86编译工作交给GCC处理，使用外部汇编器/链接器，生成低效代码，并且其Rust代码质量尚未达到专家水平。卡利尼指出，该项目已将Opus 4.6的能力推向了极限。

这项实验展示了自主大型语言模型开发在复杂项目中的变革潜力，但也引发了对未经验证软件风险以及人工智能快速、不可预测发展的担忧。

---

## 6. Flock CEO 称 Deflock 为“恐怖组织” (2025) [视频]

**原文标题**: Flock CEO calls Deflock a “terrorist organization” (2025) [video]

**原文链接**: [https://www.youtube.com/watch?v=l-kZGrDz7PU](https://www.youtube.com/watch?v=l-kZGrDz7PU)

所提供的文章标题表明，2025年，Flock的首席执行官公开将Deflock定性为“恐怖组织”，且该声明以视频形式呈现。然而，随附的“内容”并未提供关于事件本身、Flock或Deflock这两个组织，以及首席执行官指控原因的任何细节。相反，内容仅由YouTube的通用页脚链接和2026年的版权信息组成，对标题中描述的新闻事件未提供任何见解。

---

## 7. TikTok的“上瘾设计”在欧洲被裁定违法。

**原文标题**: TikTok's 'addictive design' found to be illegal in Europe

**原文链接**: [https://www.nytimes.com/2026/02/06/business/tiktok-addictive-design-europe.html](https://www.nytimes.com/2026/02/06/business/tiktok-addictive-design-europe.html)

无法访问文章链接。

---

## 8. Hackers (1995) Animated Experience

**原文标题**: Hackers (1995) Animated Experience

**原文链接**: [https://hackers-1995.vercel.app/](https://hackers-1995.vercel.app/)

生成摘要时出错

---

## 9. A new bill in New York would require disclaimers on AI-generated news content

**原文标题**: A new bill in New York would require disclaimers on AI-generated news content

**原文链接**: [https://www.niemanlab.org/2026/02/a-new-bill-in-new-york-would-require-disclaimers-on-ai-generated-news-content/](https://www.niemanlab.org/2026/02/a-new-bill-in-new-york-would-require-disclaimers-on-ai-generated-news-content/)

生成摘要时出错

---

## 10. France's homegrown open source online office suite

**原文标题**: France's homegrown open source online office suite

**原文链接**: [https://github.com/suitenumerique](https://github.com/suitenumerique)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 2 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 3 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 4 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 5 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 6 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 7 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 8 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 9 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 10 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 11 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 12 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 13 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 14 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 15 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 16 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 17 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 18 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 19 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 20 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 21 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 22 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 23 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 24 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 25 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 26 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 27 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 28 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 29 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 30 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 31 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 32 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 33 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 34 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 35 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 36 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 37 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 38 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 39 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 40 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 41 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 42 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 43 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 44 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 45 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 46 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 47 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 48 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 49 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 50 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 51 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 52 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 53 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 54 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 55 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 56 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 57 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 58 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 59 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 60 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 61 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 62 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 63 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 64 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 65 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 66 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 67 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 68 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 69 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 70 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 71 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 72 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 73 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 74 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 75 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 76 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 77 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 78 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 79 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 80 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 81 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 82 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 83 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 84 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 85 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 86 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 87 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 88 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 89 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 90 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 91 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
| 92 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 93 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
