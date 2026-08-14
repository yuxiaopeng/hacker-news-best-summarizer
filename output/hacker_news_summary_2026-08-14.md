# Hacker News 热门文章摘要 (2026-08-14)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

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

## 11. Understanding is the new bottleneck

**原文标题**: Understanding is the new bottleneck

**原文链接**: [https://www.geoffreylitt.com/2026/07/02/understanding-is-the-new-bottleneck](https://www.geoffreylitt.com/2026/07/02/understanding-is-the-new-bottleneck)

生成摘要时出错

---

## 12. Choose Boring Technology (2015)

**原文标题**: Choose Boring Technology (2015)

**原文链接**: [https://mcfunley.com/choose-boring-technology](https://mcfunley.com/choose-boring-technology)

生成摘要时出错

---

## 13. Deutsche Bank becomes first foreign yuan clearing bank in Europe

**原文标题**: Deutsche Bank becomes first foreign yuan clearing bank in Europe

**原文链接**: [https://tradersunion.com/news/central-banks/show/2973571-deutsche-bank-becomes/](https://tradersunion.com/news/central-banks/show/2973571-deutsche-bank-becomes/)

生成摘要时出错

---

## 14. Mistral OCR 4.1

**原文标题**: Mistral OCR 4.1

**原文链接**: [https://docs.mistral.ai/models/ocr-4-1](https://docs.mistral.ai/models/ocr-4-1)

生成摘要时出错

---

## 15. Ordinary Abundance

**原文标题**: Ordinary Abundance

**原文链接**: [https://ordinaryabundance.com/](https://ordinaryabundance.com/)

生成摘要时出错

---

## 16. Nine PBS sues Iron Mountain over blocked access to archival data

**原文标题**: Nine PBS sues Iron Mountain over blocked access to archival data

**原文链接**: [https://current.org/2026/08/nine-pbs-sues-iron-mountain-over-blocked-access-to-archival-data/](https://current.org/2026/08/nine-pbs-sues-iron-mountain-over-blocked-access-to-archival-data/)

生成摘要时出错

---

## 17. Hello, me. It's been a while

**原文标题**: Hello, me. It's been a while

**原文链接**: [https://themech.net/2026/08/hello-me-its-been-a-while/](https://themech.net/2026/08/hello-me-its-been-a-while/)

生成摘要时出错

---

## 18. Count Binface receives over a quarter of votes in Clacton by-election

**原文标题**: Count Binface receives over a quarter of votes in Clacton by-election

**原文链接**: [https://www.bbc.com/news/articles/ce97mm3vvemo](https://www.bbc.com/news/articles/ce97mm3vvemo)

生成摘要时出错

---

## 19. Qwen3.8-27B

**原文标题**: Qwen3.8-27B

**原文链接**: [https://twitter.com/alibaba_qwen/status/2088280182356611304](https://twitter.com/alibaba_qwen/status/2088280182356611304)

生成摘要时出错

---

## 20. Principia Mathematica is modern and insightful

**原文标题**: Principia Mathematica is modern and insightful

**原文链接**: [https://okmij.org/ftp/Computation/Impressions/PrincipiaMathematica.html](https://okmij.org/ftp/Computation/Impressions/PrincipiaMathematica.html)

生成摘要时出错

---

## 21. Donkey.bas is 45 Years Old – 131 line of Glory

**原文标题**: Donkey.bas is 45 Years Old – 131 line of Glory

**原文链接**: [https://donkeybas.com/](https://donkeybas.com/)

生成摘要时出错

---

## 22. In Australia, a home battery boom has helped cut wholesale power prices

**原文标题**: In Australia, a home battery boom has helped cut wholesale power prices

**原文链接**: [https://e360.yale.edu/digest/australia-home-batteries](https://e360.yale.edu/digest/australia-home-batteries)

生成摘要时出错

---

## 23. Single log line is 49KB+ (ext4) / 110KB+ (btrfs) of systemd-journald disk writes

**原文标题**: Single log line is 49KB+ (ext4) / 110KB+ (btrfs) of systemd-journald disk writes

**原文链接**: [https://github.com/systemd/systemd/issues/40262](https://github.com/systemd/systemd/issues/40262)

生成摘要时出错

---

## 24. NP-overrated

**原文标题**: NP-overrated

**原文链接**: [https://gruhn.me/blog/2026-08-13/](https://gruhn.me/blog/2026-08-13/)

生成摘要时出错

---

## 25. US conducted mass spying campaign against leftwing and anti-ICE protesters

**原文标题**: US conducted mass spying campaign against leftwing and anti-ICE protesters

**原文链接**: [https://www.theguardian.com/us-news/2026/aug/13/us-government-spied-anti-ice-protesters](https://www.theguardian.com/us-news/2026/aug/13/us-government-spied-anti-ice-protesters)

生成摘要时出错

---

## 26. I requested a copy of my data from McDonald’s loyalty program

**原文标题**: I requested a copy of my data from McDonald’s loyalty program

**原文链接**: [https://www.wired.com/story/mcdonalds-built-a-515-page-dossier-on-me-it-says-ill-never-leave/](https://www.wired.com/story/mcdonalds-built-a-515-page-dossier-on-me-it-says-ill-never-leave/)

生成摘要时出错

---

## 27. DeepSeek peak/off-peak pricing update

**原文标题**: DeepSeek peak/off-peak pricing update

**原文链接**: [https://api-docs.deepseek.com/news/news260813/](https://api-docs.deepseek.com/news/news260813/)

生成摘要时出错

---

## 28. Where did the old web go? We followed 657,607 links to find out

**原文标题**: Where did the old web go? We followed 657,607 links to find out

**原文链接**: [https://0.mk/blog/link-rot](https://0.mk/blog/link-rot)

生成摘要时出错

---

## 29. Choosing an AI model: one prompt, 11 models, different results

**原文标题**: Choosing an AI model: one prompt, 11 models, different results

**原文链接**: [https://www.netlify.com/blog/one-prompt-11-models-very-different-results/](https://www.netlify.com/blog/one-prompt-11-models-very-different-results/)

生成摘要时出错

---

## 30. Seven books I keep close because I love them

**原文标题**: Seven books I keep close because I love them

**原文链接**: [https://blog.plover.com/2026/08/02/](https://blog.plover.com/2026/08/02/)

生成摘要时出错

---

## 31. Bluesky Protocol Services

**原文标题**: Bluesky Protocol Services

**原文链接**: [https://atproto.com/blog/introducing-bluesky-protocol-services](https://atproto.com/blog/introducing-bluesky-protocol-services)

生成摘要时出错

---

## 32. How Compaction Works in Pi

**原文标题**: How Compaction Works in Pi

**原文链接**: [https://earendil.com/posts/compaction-in-pi/](https://earendil.com/posts/compaction-in-pi/)

生成摘要时出错

---

## 33. Flutter 3.47

**原文标题**: Flutter 3.47

**原文链接**: [https://flutter.dev/blog/whats-new-in-flutter-3-47](https://flutter.dev/blog/whats-new-in-flutter-3-47)

生成摘要时出错

---

## 34. Kubernetes on Oxide: How customer needs shaped our integrations

**原文标题**: Kubernetes on Oxide: How customer needs shaped our integrations

**原文链接**: [https://oxide.computer/blog/kubernetes-on-oxide](https://oxide.computer/blog/kubernetes-on-oxide)

生成摘要时出错

---

## 35. Thanks to social media, canned sardines are a scarcity on the supermarket shelf

**原文标题**: Thanks to social media, canned sardines are a scarcity on the supermarket shelf

**原文链接**: [https://corneroffifth.studio/why-cant-you-find-canned-sardines-right-now/](https://corneroffifth.studio/why-cant-you-find-canned-sardines-right-now/)

生成摘要时出错

---

## 36. Dear people who work at the airport

**原文标题**: Dear people who work at the airport

**原文链接**: [https://life-after-ssri.bearblog.dev/dear-people-who-work-at-the-airport/](https://life-after-ssri.bearblog.dev/dear-people-who-work-at-the-airport/)

生成摘要时出错

---

## 37. AI agents lie, cheat and steal. That is putting off users

**原文标题**: AI agents lie, cheat and steal. That is putting off users

**原文链接**: [https://www.economist.com/business/2026/08/12/ai-agents-lie-cheat-and-steal-that-is-putting-off-users](https://www.economist.com/business/2026/08/12/ai-agents-lie-cheat-and-steal-that-is-putting-off-users)

生成摘要时出错

---

## 38. SparrowMap – Cameras that watch government vehicles

**原文标题**: SparrowMap – Cameras that watch government vehicles

**原文链接**: [https://sparrowmap.com/](https://sparrowmap.com/)

生成摘要时出错

---

## 39. When Genius Fails: The Intellectual Arrogance of the AI Labs

**原文标题**: When Genius Fails: The Intellectual Arrogance of the AI Labs

**原文链接**: [https://weightythoughts.com/p/when-genius-failsthe-intellectual](https://weightythoughts.com/p/when-genius-failsthe-intellectual)

生成摘要时出错

---

## 40. Breaking the WAL

**原文标题**: Breaking the WAL

**原文链接**: [https://antithesis.com/blog/2026/wal-reset-bug/](https://antithesis.com/blog/2026/wal-reset-bug/)

生成摘要时出错

---

## 41. France's top court blocks social media ban for under-15s

**原文标题**: France's top court blocks social media ban for under-15s

**原文链接**: [https://www.reuters.com/world/frances-top-court-rules-social-media-ban-curtails-freedom-expression-2026-08-14/](https://www.reuters.com/world/frances-top-court-rules-social-media-ban-curtails-freedom-expression-2026-08-14/)

生成摘要时出错

---

## 42. Blog about things you don't understand yet

**原文标题**: Blog about things you don't understand yet

**原文链接**: [https://www.seangoedecke.com/blog-about-things-you-dont-understand-yet/](https://www.seangoedecke.com/blog-about-things-you-dont-understand-yet/)

生成摘要时出错

---

## 43. I built a 500k-domain search engine for makers in a weekend for $10

**原文标题**: I built a 500k-domain search engine for makers in a weekend for $10

**原文链接**: [https://alexmorleyfinch.github.io/marlin/history/v1/article/the_birth.html](https://alexmorleyfinch.github.io/marlin/history/v1/article/the_birth.html)

生成摘要时出错

---

## 44. Heart aerospace completes first flight of largest electric aircraft

**原文标题**: Heart aerospace completes first flight of largest electric aircraft

**原文链接**: [https://www.heartaerospace.com/newsroom/heart-aerospace-completes-first-flight-of-world-s-largest-electric-aircraft](https://www.heartaerospace.com/newsroom/heart-aerospace-completes-first-flight-of-world-s-largest-electric-aircraft)

生成摘要时出错

---

## 45. Text AI watermarks will always be trivial to remove

**原文标题**: Text AI watermarks will always be trivial to remove

**原文链接**: [https://www.seangoedecke.com/text-ai-watermarks/](https://www.seangoedecke.com/text-ai-watermarks/)

生成摘要时出错

---

## 46. Google is making private AI practical with homomorphic encryption

**原文标题**: Google is making private AI practical with homomorphic encryption

**原文链接**: [https://blog.google/security/how-google-is-making-private-ai-practical-with-homomorphic-encryption/](https://blog.google/security/how-google-is-making-private-ai-practical-with-homomorphic-encryption/)

生成摘要时出错

---

## 47. Introducing Toast 1

**原文标题**: Introducing Toast 1

**原文链接**: [https://www.mixedbread.com/blog/toast-1](https://www.mixedbread.com/blog/toast-1)

生成摘要时出错

---

## 48. How AI text watermarking works

**原文标题**: How AI text watermarking works

**原文链接**: [https://declaude.org/watermarking/](https://declaude.org/watermarking/)

生成摘要时出错

---

## 49. DeepSeek API Pricing Update

**原文标题**: DeepSeek API Pricing Update

**原文链接**: [https://twitter.com/deepseek_ai/status/2087864589895798968](https://twitter.com/deepseek_ai/status/2087864589895798968)

生成摘要时出错

---

## 50. RustDesk now supports true unattended remote access on Wayland

**原文标题**: RustDesk now supports true unattended remote access on Wayland

**原文链接**: [https://rustdesk.com/blog/unattended-remote-access-wayland/](https://rustdesk.com/blog/unattended-remote-access-wayland/)

生成摘要时出错

---

## 51. AI At Home Part 1: A Box Of Scraps

**原文标题**: AI At Home Part 1: A Box Of Scraps

**原文链接**: [https://jdagostino.github.io/ai-pt1-box-o-scraps/index.html](https://jdagostino.github.io/ai-pt1-box-o-scraps/index.html)

生成摘要时出错

---

## 52. How Organizations Use AI: Evidence from ChatGPT [pdf]

**原文标题**: How Organizations Use AI: Evidence from ChatGPT [pdf]

**原文链接**: [https://cdn.openai.com/pdf/how-organizations-use-chatgpt.pdf](https://cdn.openai.com/pdf/how-organizations-use-chatgpt.pdf)

生成摘要时出错

---

## 53. Happy 45th Birthday to the IBM PC and Model F/XT

**原文标题**: Happy 45th Birthday to the IBM PC and Model F/XT

**原文链接**: [https://sharktastica.co.uk/articles/pc-fxt-45](https://sharktastica.co.uk/articles/pc-fxt-45)

生成摘要时出错

---

## 54. How Gödel's Proof Works (2020)

**原文标题**: How Gödel's Proof Works (2020)

**原文链接**: [https://www.quantamagazine.org/how-godels-proof-works-20200714/](https://www.quantamagazine.org/how-godels-proof-works-20200714/)

生成摘要时出错

---

## 55. The TEMU-Fication of Software, Digital Goods and Services

**原文标题**: The TEMU-Fication of Software, Digital Goods and Services

**原文链接**: [https://xn--gckvb8fzb.com/the-temu-fication-of-software-digital-goods-services/](https://xn--gckvb8fzb.com/the-temu-fication-of-software-digital-goods-services/)

生成摘要时出错

---

## 56. 'Not acceptable': Judge orders Google to make rival app store installs easier

**原文标题**: 'Not acceptable': Judge orders Google to make rival app store installs easier

**原文链接**: [https://www.theverge.com/policy/979852/that-is-not-acceptable-judge-orders-google-to-make-rival-app-store-installs-easier](https://www.theverge.com/policy/979852/that-is-not-acceptable-judge-orders-google-to-make-rival-app-store-installs-easier)

生成摘要时出错

---

## 57. Launch HN: Bullet (YC S26) – A Faster Coding Agent

**原文标题**: Launch HN: Bullet (YC S26) – A Faster Coding Agent

**原文链接**: [https://www.codewithbullet.com](https://www.codewithbullet.com)

生成摘要时出错

---

## 58. Build Wide, Ship Narrow

**原文标题**: Build Wide, Ship Narrow

**原文链接**: [https://adapt.com/blog/build-wide-ship-narrow](https://adapt.com/blog/build-wide-ship-narrow)

生成摘要时出错

---

## 59. How art invented humanity

**原文标题**: How art invented humanity

**原文链接**: [https://aeon.co/essays/humans-did-not-invent-art-it-was-the-other-way-around](https://aeon.co/essays/humans-did-not-invent-art-it-was-the-other-way-around)

生成摘要时出错

---

## 60. Can I use my Outputs to train an AI model?

**原文标题**: Can I use my Outputs to train an AI model?

**原文链接**: [https://support.claude.com/en/articles/12326764-can-i-use-my-outputs-to-train-an-ai-model](https://support.claude.com/en/articles/12326764-can-i-use-my-outputs-to-train-an-ai-model)

生成摘要时出错

---

## 61. Unsloth Qwen3.8-27B GGUF files

**原文标题**: Unsloth Qwen3.8-27B GGUF files

**原文链接**: [https://huggingface.co/unsloth/Qwen3.8-27B-GGUF](https://huggingface.co/unsloth/Qwen3.8-27B-GGUF)

生成摘要时出错

---

## 62. Record heat is drying up Europe's major rivers, as these striking images show

**原文标题**: Record heat is drying up Europe's major rivers, as these striking images show

**原文链接**: [https://www.washingtonpost.com/climate-environment/interactive/2026/08/12/see-receding-water-levels-europes-major-rivers/](https://www.washingtonpost.com/climate-environment/interactive/2026/08/12/see-receding-water-levels-europes-major-rivers/)

生成摘要时出错

---

## 63. Person Hides Prompt Injection in Legal Filing Telling AI to Side with Them

**原文标题**: Person Hides Prompt Injection in Legal Filing Telling AI to Side with Them

**原文链接**: [https://www.404media.co/person-hides-prompt-injection-in-legal-filing-telling-ai-to-side-with-them/](https://www.404media.co/person-hides-prompt-injection-in-legal-filing-telling-ai-to-side-with-them/)

生成摘要时出错

---

## 64. The Strongest El Niño Ever Forecast and the Hunger It Will Leave Behind

**原文标题**: The Strongest El Niño Ever Forecast and the Hunger It Will Leave Behind

**原文链接**: [https://www.4hunger.org/p/scorched-harvest-the-strongest-el](https://www.4hunger.org/p/scorched-harvest-the-strongest-el)

生成摘要时出错

---

## 65. France's tax authority had data stolen on 680k taxpayers

**原文标题**: France's tax authority had data stolen on 680k taxpayers

**原文链接**: [https://korben.info/en/france-tax-authority-data-breach-680000-taxpayers.html](https://korben.info/en/france-tax-authority-data-breach-680000-taxpayers.html)

生成摘要时出错

---

## 66. Ntfy – open-source Push to Mobile

**原文标题**: Ntfy – open-source Push to Mobile

**原文链接**: [https://ntfy.sh/](https://ntfy.sh/)

生成摘要时出错

---

## 67. Time to Move On: Querying Without Nulls and Bags

**原文标题**: Time to Move On: Querying Without Nulls and Bags

**原文链接**: [https://arxiv.org/abs/2608.10863](https://arxiv.org/abs/2608.10863)

生成摘要时出错

---

## 68. Three years after police raid on Kansas newspaper, reporter settles for $850K

**原文标题**: Three years after police raid on Kansas newspaper, reporter settles for $850K

**原文链接**: [https://kansasreflector.com/2026/08/11/three-years-after-police-raid-on-kansas-newspaper-reporter-settles-lawsuit-for-850k/](https://kansasreflector.com/2026/08/11/three-years-after-police-raid-on-kansas-newspaper-reporter-settles-lawsuit-for-850k/)

生成摘要时出错

---

## 69. Self-hosted web push Cloudflare Worker, works on iOS

**原文标题**: Self-hosted web push Cloudflare Worker, works on iOS

**原文链接**: [https://kukuroo.cc/](https://kukuroo.cc/)

生成摘要时出错

---

## 70. PBS loses 70 years of TV history after cloud storage vendor goes defunct

**原文标题**: PBS loses 70 years of TV history after cloud storage vendor goes defunct

**原文链接**: [https://www.tomshardware.com/software/cloud-storage/nine-pbs-loses-access-to-70-years-of-data-after-contracted-cloud-storage-vendor-goes-defunct-public-tv-channel-sues-iron-mountain-data-center-which-hosts-archival-materials-to-ensure-preservation](https://www.tomshardware.com/software/cloud-storage/nine-pbs-loses-access-to-70-years-of-data-after-contracted-cloud-storage-vendor-goes-defunct-public-tv-channel-sues-iron-mountain-data-center-which-hosts-archival-materials-to-ensure-preservation)

生成摘要时出错

---

## 71. Trump has amassed staggering wealth in 'most openly corrupt' presidency

**原文标题**: Trump has amassed staggering wealth in 'most openly corrupt' presidency

**原文链接**: [https://www.theguardian.com/us-news/2026/aug/13/trump-presidency-revenue-wealth](https://www.theguardian.com/us-news/2026/aug/13/trump-presidency-revenue-wealth)

生成摘要时出错

---

## 72. Gemini 3.7 Flash

**原文标题**: Gemini 3.7 Flash

**原文链接**: [https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-3-7-flash/](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-3-7-flash/)

生成摘要时出错

---

## 73. S.F.'s top-paid employee made $900K. Here's what every city worker gets paid

**原文标题**: S.F.'s top-paid employee made $900K. Here's what every city worker gets paid

**原文链接**: [https://www.sfchronicle.com/projects/2026/san-francisco-employee-pay/?taid=6a7db1d2d297630001917f1d&utm_campaign=trueanthem%2B3988&utm_medium=social&utm_source=twitter](https://www.sfchronicle.com/projects/2026/san-francisco-employee-pay/?taid=6a7db1d2d297630001917f1d&utm_campaign=trueanthem%2B3988&utm_medium=social&utm_source=twitter)

生成摘要时出错

---

## 74. Terabytes of credentials leaked in supply-chain attack

**原文标题**: Terabytes of credentials leaked in supply-chain attack

**原文链接**: [https://arstechnica.com/security/2026/08/terabytes-of-credentials-leaked-in-massive-supply-chain-attack/](https://arstechnica.com/security/2026/08/terabytes-of-credentials-leaked-in-massive-supply-chain-attack/)

生成摘要时出错

---

## 75. Flock updates privacy, accountability, security, and transparency safeguards

**原文标题**: Flock updates privacy, accountability, security, and transparency safeguards

**原文链接**: [https://www.flocksafety.com/blog/flock-guardrails-address-lpr-privacy-concerns-and-police-transparency](https://www.flocksafety.com/blog/flock-guardrails-address-lpr-privacy-concerns-and-police-transparency)

生成摘要时出错

---

## 76. Show HN: LuaCAD – Parametric CAD Scripted in Lua

**原文标题**: Show HN: LuaCAD – Parametric CAD Scripted in Lua

**原文链接**: [https://luacad.ad-si.com](https://luacad.ad-si.com)

生成摘要时出错

---

## 77. Show HN: Lumabri – Run Moe Models on a P2P Swarm with Colibri

**原文标题**: Show HN: Lumabri – Run Moe Models on a P2P Swarm with Colibri

**原文链接**: [https://github.com/JustVugg/lumabri](https://github.com/JustVugg/lumabri)

生成摘要时出错

---

## 78. US loses one-fourth of drone fleet as Iran war drains its arsenal

**原文标题**: US loses one-fourth of drone fleet as Iran war drains its arsenal

**原文链接**: [https://www.indiatoday.in/world/story/us-loses-one-fourth-mq-9-reaper-drones-near-strait-of-hormuz-in-iran-war-2970823-2026-08-14](https://www.indiatoday.in/world/story/us-loses-one-fourth-mq-9-reaper-drones-near-strait-of-hormuz-in-iran-war-2970823-2026-08-14)

生成摘要时出错

---

## 79. Earth.nullschool.net

**原文标题**: Earth.nullschool.net

**原文链接**: [https://earth.nullschool.net/](https://earth.nullschool.net/)

生成摘要时出错

---

## 80. US Navy sailors try to throw themselves overboard after 250 days at sea

**原文标题**: US Navy sailors try to throw themselves overboard after 250 days at sea

**原文链接**: [https://www.telegraph.co.uk/world-news/2026/08/13/us-navy-sailors-jump-overboard-after-nine-months-at-sea/](https://www.telegraph.co.uk/world-news/2026/08/13/us-navy-sailors-jump-overboard-after-nine-months-at-sea/)

生成摘要时出错

---

## 81. 'The Nerd Reich' tracks the 'unmasking of Silicon Valley's true politics'

**原文标题**: 'The Nerd Reich' tracks the 'unmasking of Silicon Valley's true politics'

**原文链接**: [https://www.npr.org/2026/08/10/nx-s1-5925350/the-nerd-reich-tracks-the-unmasking-of-silicon-valleys-true-politics](https://www.npr.org/2026/08/10/nx-s1-5925350/the-nerd-reich-tracks-the-unmasking-of-silicon-valleys-true-politics)

生成摘要时出错

---

## 82. Even Claude Is in the Dark About Dario Amodei's Wife

**原文标题**: Even Claude Is in the Dark About Dario Amodei's Wife

**原文链接**: [https://www.wsj.com/tech/ai/claude-dario-amodei-wife-anthropic-e1eeda7d](https://www.wsj.com/tech/ai/claude-dario-amodei-wife-anthropic-e1eeda7d)

生成摘要时出错

---

## 83. Mozilla says stricter antitrust measures against Google 'threaten Firefox'

**原文标题**: Mozilla says stricter antitrust measures against Google 'threaten Firefox'

**原文链接**: [https://www.techcentral.ie/mozilla-says-stricter-antitrust-measures-against-google-threaten-firefox/](https://www.techcentral.ie/mozilla-says-stricter-antitrust-measures-against-google-threaten-firefox/)

生成摘要时出错

---

## 84. AI Model Atlas – visualizing populations of ML models as interconnected 3D graph

**原文标题**: AI Model Atlas – visualizing populations of ML models as interconnected 3D graph

**原文链接**: [https://run.cosmograph.app/public/ca9fd1ad-fe83-4238-8b69-b707c633aef0](https://run.cosmograph.app/public/ca9fd1ad-fe83-4238-8b69-b707c633aef0)

生成摘要时出错

---

## 85. HashAgent – Share an AI agent as a URL, runs locally via WebGPU

**原文标题**: HashAgent – Share an AI agent as a URL, runs locally via WebGPU

**原文链接**: [https://hashagent.pages.dev/](https://hashagent.pages.dev/)

生成摘要时出错

---

## 86. For the love of god stop using CPU limits in Kubernetes

**原文标题**: For the love of god stop using CPU limits in Kubernetes

**原文链接**: [https://github.com/inevolin/k8s-cpu-limits-analyzed](https://github.com/inevolin/k8s-cpu-limits-analyzed)

生成摘要时出错

---

## 87. "Solving a largely imaginary user goal"

**原文标题**: "Solving a largely imaginary user goal"

**原文链接**: [https://unsung.aresluna.org/solving-a-largely-imaginary-user-goal/](https://unsung.aresluna.org/solving-a-largely-imaginary-user-goal/)

生成摘要时出错

---

## 88. Major oil slick washes up on Iran coast after Hormuz ship strike

**原文标题**: Major oil slick washes up on Iran coast after Hormuz ship strike

**原文链接**: [https://www.bbc.com/news/articles/cr7kpdkg13zo](https://www.bbc.com/news/articles/cr7kpdkg13zo)

生成摘要时出错

---

## 89. Samsung is using Claude to verify chip designs. It's not going smoothly

**原文标题**: Samsung is using Claude to verify chip designs. It's not going smoothly

**原文链接**: [https://www.neowin.net/news/samsung-is-using-claude-to-verify-chip-designs-and-its-not-going-smoothly/](https://www.neowin.net/news/samsung-is-using-claude-to-verify-chip-designs-and-its-not-going-smoothly/)

生成摘要时出错

---

## 90. Taxpayers Funded a $533M Artillery Plant That Made Nothing

**原文标题**: Taxpayers Funded a $533M Artillery Plant That Made Nothing

**原文链接**: [https://www.propublica.org/article/general-dynamics-artillery-factory-failed](https://www.propublica.org/article/general-dynamics-artillery-factory-failed)

生成摘要时出错

---

