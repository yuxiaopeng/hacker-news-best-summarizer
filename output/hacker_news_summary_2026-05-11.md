# Hacker News 热门文章摘要 (2026-05-11)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 硬件证明作为垄断的使能者

**原文标题**: Hardware Attestation as Monopoly Enabler

**原文链接**: [https://grapheneos.social/@GrapheneOS/116550899908879585](https://grapheneos.social/@GrapheneOS/116550899908879585)

所提供的内容，题为《硬件认证：垄断助推器》，对主要科技公司日益推行硬件认证的做法提出了批判性观点。

核心信息通过GrapheneOS在Mastodon上发布的一段引言传达，强调“苹果和谷歌正在逐步扩大他们对这项技术的使用”。尽管这段引言不完整，但文章的标题强烈暗示这种扩张指的是硬件认证。

GrapheneOS，一个专注于隐私和安全的安卓操作系统，表示担忧，认为这一趋势尽管常被宣传为一项安全措施，却可能有助于巩固这些公司的垄断地位。硬件认证验证设备软件环境的完整性，而它的日益普及可能会限制用户自由，限制替代操作系统的安装，阻碍应用程序的旁加载，并扼杀数字生态系统内的竞争。

本质上，这篇“文章”是GrapheneOS发出的一个警报，暗示看似是安全功能的特性，实际上可能成为主导者在科技领域施加更大控制并限制开放性的工具。（关于Mastodon的JavaScript附注是访问该平台的技术说明，不属于文章的核心内容。）

---

## 2. 本地AI应成为常态

**原文标题**: Local AI needs to be the norm

**原文链接**: [https://unix.foo/posts/local-ai-needs-to-be-norm/](https://unix.foo/posts/local-ai-needs-to-be-norm/)

文章批评了将云端托管的AI API集成到应用程序中的普遍趋势，认为这种做法导致软件脆弱、侵犯隐私且不必要地复杂。文章指出，现代设备拥有强大的本地芯片，包括神经网络引擎，但在应用程序依赖外部服务器时，这些本地芯片却大部分处于闲置状态，从而导致软件对网络状况、供应商正常运行时间和计费的依赖。

作者倡导本地AI，强调其通过将用户数据保留在设备上，从而在确保隐私、增强可靠性和简化软件堆栈方面的益处。文章认为，本地AI是处理用户自有数据（如总结、提取、分类或规范化）的理想选择，而非充当通用知识引擎。这种方法比冗长的隐私政策更能有效地培养用户信任。

作为一个具体例子，文章详细介绍了iOS应用程序“The Brutalist Report”，该应用使用苹果的本地模型API完全在设备上生成文章摘要。这种方法避免了服务器迂回、数据记录和第三方依赖。作者强调了苹果为实现便捷本地AI开发所提供的工具，特别是能够直接从模型生成结构化、类型化输出（例如Swift结构体）的能力，这相对于解析非结构化文本而言是一项工程改进。

文章承认本地模型在原始智能方面可能无法与云端模型匹敌，但它们被认为是“非常出色”的，足以满足常见的应用功能需求。文章最后敦促开发者仅在严格必要时才使用云端模型，优先将用户数据保留在本地，并将AI作为可靠、结构化的子系统集成，以避免为简单功能构建不必要的分布式系统。

---

## 3. 我要回去手写代码了。

**原文标题**: I'm going back to writing code by hand

**原文链接**: [https://blog.k10s.dev/im-going-back-to-writing-code-by-hand/](https://blog.k10s.dev/im-going-back-to-writing-code-by-hand/)

作者讲述了他使用 Claude AI 凭直觉为 Kubernetes TUI 工具 k10s 编程七个月的经历，最初实现了快速的功能开发。他描述了一种速度的假象，即 AI 快速实现了实时更新、资源视图和 GPU 集群视图等功能，使他以为自己的开发速度是平时的十倍。

然而，这种不受约束的方法导致了一种“上帝对象”架构：一个单一、庞大的 `Model` 结构体累积了所有 UI、状态和客户端逻辑。`Update()` 方法变成了一个包含 110 个 switch/case 分支的庞大 500 行函数，导致状态混乱、键绑定冲突以及复杂且容易出错的清理逻辑（例如，九次手动将变量赋为 `nil` 以防止视图之间的数据泄露）。

作者总结了四个主要教训：
1.  **AI 擅长构建功能，而非架构：** 它擅长处理孤立的任务，但缺乏对更广泛系统设计的认知，导致特殊情况处理和视图隔离的缺失。
2.  **“上帝对象”是 AI 的默认产物：** AI 倾向于采用一个结构体包含所有内容的方法，导致代码紧密耦合，难以推断其行为。
3.  **速度的假象会扩大项目范围：** 感觉上添加功能的容易程度会鼓励范围蔓延，导致项目臃肿，并将其从一个利基工具变成了一个通用工具。
4.  **位置数据是颗定时炸弹：** （作者简要提及）依赖数组索引等位置数据会使系统变得脆弱。

他总结道，人类必须在利用 AI 进行实现*之前*定义架构、接口和范围边界，有效地将 `CLAUDE.md` 指令用作护栏。作者现在正在放弃 AI 生成的代码库，从头重写 k10s，强调人类干预对于有意义的软件开发仍然至关重要。

---

## 4. 事件报告：CVE-2024-YIKES

**原文标题**: Incident Report: CVE-2024-YIKES

**原文链接**: [https://nesbitt.io/2026/02/03/incident-report-cve-2024-yikes.html](https://nesbitt.io/2026/02/03/incident-report-cve-2024-yikes.html)

“CVE-2024-YIKES”事件报告详细描述了一次长达73小时的“灾难性”安全漏洞，该漏洞“意外地”得到了解决。事件链始于流行JavaScript软件包`left-justify`的维护者在YubiKey丢失后（幽默地归因于“Kubernetes这只狗”），通过人工智能生成的链接被钓鱼获取了凭据。

此次入侵导致`left-justify`窃取了凭据，其中包括Rust库`vulpine-lz4`的凭据。随后发布了恶意版本的`vulpine-lz4`，感染了CI（持续集成）管道。这进而导致`snekpack`（一个内含`vulpine-lz4`的Python构建工具）被入侵。`snekpack` 3.7.0版本发布，在大约400万开发人员机器上安装了恶意软件，添加了SSH密钥、一个周二激活的反向Shell，并莫名其妙地将默认Shell更改为`fish`。

该事件被一个不相关的加密货币挖矿蠕虫`cryptobro-9000`意外解决。在传播过程中，该蠕虫意外地将`snekpack`升级到合法的修补版本（3.7.1），并使恶意软件的命令与控制服务器过载，从而阻止了反向Shell在其指定周二被激活。

根本原因包括Npm认证薄弱、AI驱动的网络钓鱼以及未维护的内嵌依赖项。尽管有420万台机器被入侵，但类似数量的机器却被这个“仁慈的”蠕虫“拯救”，导致“令人不安”的净安全态势。报告强调了被忽视的警告和延迟的修复，并以呼吁增加安全团队人手作为结尾。

---

## 5. 路易斯·罗斯曼提出为一名受威胁的OrcaSlicer开发者支付法律费用。

**原文标题**: Louis Rossmann offers to pay legal fees for a threatened OrcaSlicer developer

**原文链接**: [https://www.tomshardware.com/3d-printing/louis-rossmann-tells-3d-printer-maker-bambu-lab-to-go-bleep-yourself-over-its-lawsuit-against-enthusiast-right-to-repair-advocate-offers-to-pay-the-legal-fees-for-a-threatened-orcaslicer-developer](https://www.tomshardware.com/3d-printing/louis-rossmann-tells-3d-printer-maker-bambu-lab-to-go-bleep-yourself-over-its-lawsuit-against-enthusiast-right-to-repair-advocate-offers-to-pay-the-legal-fees-for-a-threatened-orcaslicer-developer)

著名的“维修权”倡导者路易斯·罗斯曼（Louis Rossmann）公开表示，他愿意承担受到3D打印机制造商拓竹（Bambu Lab）威胁的OrcaSlicer开发者所产生的法律费用。

据报道，拓竹向OrcaSlicer的开发者发出了停止侵权通知函。OrcaSlicer是一款流行的开源3D打印切片软件，它从PrusaSlicer分叉而来，并整合了拓竹Studio（拓竹自家的切片软件，同样基于PrusaSlicer）的一些功能。此事件源于OrcaSlicer使用了拓竹的云服务API，以及该开发者被指控逆向工程了拓竹专有的AMS（自动材料系统）协议。

罗斯曼严厉批评了拓竹的行为，称其试图扼杀开源发展和恐吓个人开发者的行为是“愚蠢的”。他强调，一家公司在自己的产品建立在开源基础（PrusaSlicer）之上时，却去威胁一个开源项目，这极具讽刺意味。罗斯曼以其反对反维修行为的坚定立场而闻名，他认为这一事件是对开源社区和用户自由的直接冒犯。他的提议旨在为受威胁的开发者提供法律保护和支持，这标志着他更广泛地致力于捍卫开源项目，以对抗企业的过度干预。

---

## 6. Mythos Finds a Curl Vulnerability

**原文标题**: Mythos Finds a Curl Vulnerability

**原文链接**: [https://daniel.haxx.se/blog/2026/05/11/mythos-finds-a-curl-vulnerability/](https://daniel.haxx.se/blog/2026/05/11/mythos-finds-a-curl-vulnerability/)

这篇文章详细介绍了 `curl` 项目使用 Anthropic 的 Mythos AI 的经验，Mythos AI 是一款因其卓越的安全漏洞检测能力而备受吹捧的 AI 模型。在最初受限访问和延迟之后，`curl` 团队收到了 Mythos 对其 178,000 行 C 代码生成的扫描报告。

`curl` 已经过多个 AI 工具（例如 AISLE、Zeropath、Codex Security、Copilot）和传统分析器的严格扫描，已修复了数百个错误并发布了十多个 CVE。Mythos 报告承认 `curl` 经过了大量审计，在关键领域未发现任何问题。

Mythos 最初标记了五个“已确认的安全漏洞”。然而，`curl` 安全团队的审查将其减少到一个“低严重性 CVE”，其余的则是误报或小错误。报告还识别了大约二十个通用错误，并进行了高度清晰的描述。

作者的结论是，尽管 Mythos “非常好”，但其性能并未显著超越 `curl` 项目使用过的其他 AI 工具。在这种情况下，Mythos 广泛的宣传似乎主要是一种营销手段。它发现的是现有类型的错误，而非新颖的漏洞。

至关重要的是，文章强调 *所有* 现代 AI 驱动的代码分析器都远优于传统分析器。它们能够发现不一致之处，理解第三方 API 和协议，并有效地解释缺陷。任何不使用 AI 分析器的项目都可能留下大量缺陷，供攻击者利用。`curl` 打算继续利用 AI 进行持续的安全扫描。

---

## 7. 拉蒂 – 支持行内 3D 图形的终端模拟器

**原文标题**: Ratty – A terminal emulator with inline 3D graphics

**原文链接**: [https://ratty-term.org/](https://ratty-term.org/)

Ratty是一个独特的终端模拟器，它通过在其界面内直接集成行内3D图形而独树一帜。这一创新功能使其有别于传统终端，提供了显著增强的视觉体验。该项目邀请感兴趣的用户通过一篇专门的博客文章进一步探索其功能，该文章可能详细介绍了它的开发、特性和潜在用例。Ratty可供下载，让用户能够亲身体验其功能，并且其源代码也已提供，这表明了透明度，并可能促进社区贡献或审查。实质上，Ratty旨在重新定义终端模拟器的范围和视觉潜力。

---

## 8. Running local models on an M4 with 24GB memory

**原文标题**: Running local models on an M4 with 24GB memory

**原文链接**: [https://jola.dev/posts/running-local-models-on-m4](https://jola.dev/posts/running-local-models-on-m4)

The author details their successful setup for running local AI models on an M4 Mac with 24GB memory, emphasizing the excitement of offline capabilities and reduced reliance on big tech. They navigated challenges in choosing tools (Ollama, llama.cpp, LM Studio) and models, with Qwen 3.5-9B (4b quant) on LM Studio proving most effective. This setup delivers around 40 tokens per second with a 128K context window, enabling "thinking mode" and successful tool use, despite being prone to distractions or loops compared to SOTA models.

Recommended configurations for Qwen 3.5-9B with "thinking mode" are provided for both Pi and OpenCode frontends. The author stresses that local models require an interactive, step-by-step workflow rather than independent problem-solving. While not a 10x productivity boost, it acts as an engaging research assistant and programming "savant." Simple tasks like suggesting Elixir linter fixes worked well, and it could identify Git conflicts; however, execution of more complex actions, like applying Git conflict resolutions, proved problematic.

Ultimately, the author highlights several benefits of local models: no internet connection, low running costs, reduced environmental impact by using personal hardware, and the enjoyment of tinkering. They advocate for local models as a more sustainable and positive way to interact with AI technology.

---

## 9. Gmail registration now requires scanning a QR code and sending a text message

**原文标题**: Gmail registration now requires scanning a QR code and sending a text message

**原文链接**: [https://discuss.privacyguides.net/t/google-account-registration-now-requires-sending-an-sms-via-phone-instead-of-receiving-an-sms/36082](https://discuss.privacyguides.net/t/google-account-registration-now-requires-sending-an-sms-via-phone-instead-of-receiving-an-sms/36082)

生成摘要时出错

---

## 10. Show HN: Building a web server in assembly to give my life (a lack of) meaning

**原文标题**: Show HN: Building a web server in assembly to give my life (a lack of) meaning

**原文链接**: [https://github.com/imtomt/ymawky](https://github.com/imtomt/ymawky)

生成摘要时出错

---

## 11. Debian must ship reproducible packages

**原文标题**: Debian must ship reproducible packages

**原文链接**: [https://lists.debian.org/debian-devel-announce/2026/05/msg00001.html](https://lists.debian.org/debian-devel-announce/2026/05/msg00001.html)

生成摘要时出错

---

## 12. Obsidian plugin was abused to deploy a remote access trojan

**原文标题**: Obsidian plugin was abused to deploy a remote access trojan

**原文链接**: [https://cyber.netsecops.io/articles/obsidian-plugin-abused-in-campaign-to-deploy-phantom-pulse-rat/](https://cyber.netsecops.io/articles/obsidian-plugin-abused-in-campaign-to-deploy-phantom-pulse-rat/)

生成摘要时出错

---

## 13. Space Cadet Pinball on Linux

**原文标题**: Space Cadet Pinball on Linux

**原文链接**: [https://brennan.io/2026/05/09/pinball-and-escrow/](https://brennan.io/2026/05/09/pinball-and-escrow/)

生成摘要时出错

---

## 14. An AI coding agent, used to write code, needs to reduce your maintenance costs

**原文标题**: An AI coding agent, used to write code, needs to reduce your maintenance costs

**原文链接**: [https://www.jamesshore.com/v2/blog/2026/you-need-ai-that-reduces-your-maintenance-costs](https://www.jamesshore.com/v2/blog/2026/you-need-ai-that-reduces-your-maintenance-costs)

生成摘要时出错

---

## 15. The greatest shot in television: James Burke had one chance to nail this scene (2024)

**原文标题**: The greatest shot in television: James Burke had one chance to nail this scene (2024)

**原文链接**: [https://www.openculture.com/2024/10/the-greatest-shot-in-television.html](https://www.openculture.com/2024/10/the-greatest-shot-in-television.html)

生成摘要时出错

---

## 16. CUDA-oxide: Nvidia's official Rust to CUDA compiler

**原文标题**: CUDA-oxide: Nvidia's official Rust to CUDA compiler

**原文链接**: [https://nvlabs.github.io/cuda-oxide/index.html](https://nvlabs.github.io/cuda-oxide/index.html)

生成摘要时出错

---

## 17. Maryland citizens hit with $2B power grid upgrade for out-of-state AI

**原文标题**: Maryland citizens hit with $2B power grid upgrade for out-of-state AI

**原文链接**: [https://www.tomshardware.com/tech-industry/artificial-intelligence/maryland-citizens-slapped-with-usd2-billion-grid-upgrade-bill-for-out-of-state-ai-data-centers-state-complains-to-federal-energy-regulators-says-additional-cost-breaks-ratepayer-protection-pledge-promises](https://www.tomshardware.com/tech-industry/artificial-intelligence/maryland-citizens-slapped-with-usd2-billion-grid-upgrade-bill-for-out-of-state-ai-data-centers-state-complains-to-federal-energy-regulators-says-additional-cost-breaks-ratepayer-protection-pledge-promises)

生成摘要时出错

---

## 18. France moves to break encrypted messaging

**原文标题**: France moves to break encrypted messaging

**原文链接**: [https://reclaimthenet.org/france-moves-to-break-encrypted-messaging](https://reclaimthenet.org/france-moves-to-break-encrypted-messaging)

生成摘要时出错

---

## 19. Software engineering may no longer be a lifetime career

**原文标题**: Software engineering may no longer be a lifetime career

**原文链接**: [https://www.seangoedecke.com/software-engineering-may-no-longer-be-a-lifetime-career/](https://www.seangoedecke.com/software-engineering-may-no-longer-be-a-lifetime-career/)

生成摘要时出错

---

## 20. YC's Biggest Scandals

**原文标题**: YC's Biggest Scandals

**原文链接**: [https://ycombinator.fyi/](https://ycombinator.fyi/)

生成摘要时出错

---

## 21. Getting arrested in Japan

**原文标题**: Getting arrested in Japan

**原文链接**: [https://sundaicity.com/blogs/getting-arrested-in-japan](https://sundaicity.com/blogs/getting-arrested-in-japan)

生成摘要时出错

---

## 22. Task Paralysis and AI

**原文标题**: Task Paralysis and AI

**原文链接**: [https://g5t.de/articles/20260510-task-paralysis-and-ai/index.html](https://g5t.de/articles/20260510-task-paralysis-and-ai/index.html)

生成摘要时出错

---

## 23. GitHub is sinking

**原文标题**: GitHub is sinking

**原文链接**: [https://dbushell.com/2026/04/29/github-is-sinking/](https://dbushell.com/2026/04/29/github-is-sinking/)

生成摘要时出错

---

## 24. Local privilege escalation via execve()

**原文标题**: Local privilege escalation via execve()

**原文链接**: [https://www.freebsd.org/security/advisories/FreeBSD-SA-26:13.exec.asc](https://www.freebsd.org/security/advisories/FreeBSD-SA-26:13.exec.asc)

生成摘要时出错

---

## 25. Think Linear Algebra (2023)

**原文标题**: Think Linear Algebra (2023)

**原文链接**: [https://allendowney.github.io/ThinkLinearAlgebra/index.html](https://allendowney.github.io/ThinkLinearAlgebra/index.html)

生成摘要时出错

---

## 26. A.I. note takers are making lawyers nervous

**原文标题**: A.I. note takers are making lawyers nervous

**原文链接**: [https://www.nytimes.com/2026/05/09/business/dealbook/ai-notetakers-legal-risk.html](https://www.nytimes.com/2026/05/09/business/dealbook/ai-notetakers-legal-risk.html)

生成摘要时出错

---

## 27. Show HN: Rust but Lisp

**原文标题**: Show HN: Rust but Lisp

**原文链接**: [https://github.com/ThatXliner/rust-but-lisp](https://github.com/ThatXliner/rust-but-lisp)

生成摘要时出错

---

## 28. The locals don't know

**原文标题**: The locals don't know

**原文链接**: [https://www.quarter--mile.com/The-Locals-Dont-Know](https://www.quarter--mile.com/The-Locals-Dont-Know)

生成摘要时出错

---

## 29. Training an LLM in Swift, Part 1: Taking matrix mult from Gflop/s to Tflop/s

**原文标题**: Training an LLM in Swift, Part 1: Taking matrix mult from Gflop/s to Tflop/s

**原文链接**: [https://www.cocoawithlove.com/blog/matrix-multiplications-swift.html](https://www.cocoawithlove.com/blog/matrix-multiplications-swift.html)

生成摘要时出错

---

## 30. Replacing a 3 GB SQLite db with a 10 MB FST (finite state transducer) binary

**原文标题**: Replacing a 3 GB SQLite db with a 10 MB FST (finite state transducer) binary

**原文链接**: [https://til.andrew-quinn.me/posts/replacing-a-3-gb-sqlite-database-with-a-7-mb-fst-finite-state-trandsucer-binary/](https://til.andrew-quinn.me/posts/replacing-a-3-gb-sqlite-database-with-a-7-mb-fst-finite-state-trandsucer-binary/)

生成摘要时出错

---

## 31. Spain has become one of Europe’s cheapest power markets

**原文标题**: Spain has become one of Europe’s cheapest power markets

**原文链接**: [https://janrosenow.substack.com/p/spain-just-became-one-of-europes](https://janrosenow.substack.com/p/spain-just-became-one-of-europes)

生成摘要时出错

---

## 32. PS3 Emulator Devs Politely Ask That People Stop Flooding It with AI PRs

**原文标题**: PS3 Emulator Devs Politely Ask That People Stop Flooding It with AI PRs

**原文链接**: [https://kotaku.com/playstation-3-emulator-devs-politely-ask-that-people-stop-flooding-it-with-ai-code-pull-requests-2000694656](https://kotaku.com/playstation-3-emulator-devs-politely-ask-that-people-stop-flooding-it-with-ai-code-pull-requests-2000694656)

生成摘要时出错

---

## 33. Traces Of Humanity

**原文标题**: Traces Of Humanity

**原文链接**: [https://tracesofhumanity.org/hello-world/](https://tracesofhumanity.org/hello-world/)

生成摘要时出错

---

## 34. What's a mathematician to do? (2010)

**原文标题**: What's a mathematician to do? (2010)

**原文链接**: [https://mathoverflow.net/questions/43690/whats-a-mathematician-to-do](https://mathoverflow.net/questions/43690/whats-a-mathematician-to-do)

生成摘要时出错

---

## 35. Scientists warn Atlantic current at risk of shutting down

**原文标题**: Scientists warn Atlantic current at risk of shutting down

**原文链接**: [https://e360.yale.edu/features/amoc-climate-change](https://e360.yale.edu/features/amoc-climate-change)

生成摘要时出错

---

## 36. Gemini API File Search is now multimodal

**原文标题**: Gemini API File Search is now multimodal

**原文链接**: [https://blog.google/innovation-and-ai/technology/developers-tools/expanded-gemini-api-file-search-multimodal-rag/](https://blog.google/innovation-and-ai/technology/developers-tools/expanded-gemini-api-file-search-multimodal-rag/)

生成摘要时出错

---

## 37. How Fast Does Claude, Acting as a User Space IP Stack, Respond to Pings?

**原文标题**: How Fast Does Claude, Acting as a User Space IP Stack, Respond to Pings?

**原文链接**: [https://dunkels.com/adam/claude-user-space-ip-stack-ping/](https://dunkels.com/adam/claude-user-space-ip-stack-ping/)

生成摘要时出错

---

## 38. Students Boo Commencement Speaker After She Calls AI Next Industrial Revolution

**原文标题**: Students Boo Commencement Speaker After She Calls AI Next Industrial Revolution

**原文链接**: [https://www.404media.co/ucf-ai-commencement-speaker-booed/](https://www.404media.co/ucf-ai-commencement-speaker-booed/)

生成摘要时出错

---

## 39. Show HN: An index of indie web/blog indexes

**原文标题**: Show HN: An index of indie web/blog indexes

**原文链接**: [https://theindex.fyi](https://theindex.fyi)

生成摘要时出错

---

## 40. Can Someone Please Explain Whether Cloudflare Blackmailed Canonical?

**原文标题**: Can Someone Please Explain Whether Cloudflare Blackmailed Canonical?

**原文链接**: [https://www.flyingpenguin.com/can-someone-please-explain-whether-cloudflare-blackmailed-canonical/](https://www.flyingpenguin.com/can-someone-please-explain-whether-cloudflare-blackmailed-canonical/)

生成摘要时出错

---

## 41. Killed by Apple

**原文标题**: Killed by Apple

**原文链接**: [https://killedbyapple.theden.sh/](https://killedbyapple.theden.sh/)

生成摘要时出错

---

## 42. Rotten Dot Com

**原文标题**: Rotten Dot Com

**原文链接**: [https://www.theparisreview.org/blog/2026/05/06/rotten-dot-com/](https://www.theparisreview.org/blog/2026/05/06/rotten-dot-com/)

生成摘要时出错

---

## 43. Chrome's AI features may be hogging 4GB of your computer storage

**原文标题**: Chrome's AI features may be hogging 4GB of your computer storage

**原文链接**: [https://www.theverge.com/tech/924933/google-chrome-4gb-gemini-nano-ai-features](https://www.theverge.com/tech/924933/google-chrome-4gb-gemini-nano-ai-features)

生成摘要时出错

---

## 44. European Money Pours into Palantir

**原文标题**: European Money Pours into Palantir

**原文链接**: [https://english.elpais.com/economy-and-business/branded/2026-04-11/european-money-pours-into-palantir-over-100-asset-managers-and-banks-boost-their-investments-in-the-controversial-tech-company.html](https://english.elpais.com/economy-and-business/branded/2026-04-11/european-money-pours-into-palantir-over-100-asset-managers-and-banks-boost-their-investments-in-the-controversial-tech-company.html)

生成摘要时出错

---

## 45. Microsoft Israel chief leaves amid ethical controversy

**原文标题**: Microsoft Israel chief leaves amid ethical controversy

**原文链接**: [https://en.globes.co.il/en/article-microsoft-israel-chief-leaves-amid-ethical-controversy-1001542602](https://en.globes.co.il/en/article-microsoft-israel-chief-leaves-amid-ethical-controversy-1001542602)

生成摘要时出错

---

## 46. I work in Hollywood. Everyone who used to make TV is now training AI

**原文标题**: I work in Hollywood. Everyone who used to make TV is now training AI

**原文链接**: [https://www.wired.com/story/i-work-in-hollywood-everyone-who-used-to-make-tv-now-training-ai/](https://www.wired.com/story/i-work-in-hollywood-everyone-who-used-to-make-tv-now-training-ai/)

生成摘要时出错

---

## 47. Why modern parents feel more sleep deprived than our ancestors did

**原文标题**: Why modern parents feel more sleep deprived than our ancestors did

**原文链接**: [https://www.bbc.com/future/article/20260508-parents-in-ancient-times-felt-less-sleep-deprived-what-our-ancestors-did-differently-on-baby-sleep](https://www.bbc.com/future/article/20260508-parents-in-ancient-times-felt-less-sleep-deprived-what-our-ancestors-did-differently-on-baby-sleep)

生成摘要时出错

---

## 48. Gen Z Resentment Toward AI Grows as Adoption Stagnates and Workplace Fears Mount

**原文标题**: Gen Z Resentment Toward AI Grows as Adoption Stagnates and Workplace Fears Mount

**原文链接**: [https://www.waltonfamilyfoundation.org/about-us/newsroom/gen-z-resentment-toward-ai-grows-as-adoption-stagnates-and-workplace-fears-mount](https://www.waltonfamilyfoundation.org/about-us/newsroom/gen-z-resentment-toward-ai-grows-as-adoption-stagnates-and-workplace-fears-mount)

生成摘要时出错

---

## 49. 7 lines of code, 3 minutes: Implement a programming language (2010)

**原文标题**: 7 lines of code, 3 minutes: Implement a programming language (2010)

**原文链接**: [https://matt.might.net/articles/implementing-a-programming-language/](https://matt.might.net/articles/implementing-a-programming-language/)

生成摘要时出错

---

## 50. Academic Research Skills for Claude Code

**原文标题**: Academic Research Skills for Claude Code

**原文链接**: [https://github.com/Imbad0202/academic-research-skills](https://github.com/Imbad0202/academic-research-skills)

生成摘要时出错

---

## 51. Show HN: TikTok but for Scientific Papers

**原文标题**: Show HN: TikTok but for Scientific Papers

**原文链接**: [https://andreaturchet.github.io/website/index.html](https://andreaturchet.github.io/website/index.html)

生成摘要时出错

---

## 52. LLMorphism: When humans come to see themselves as language models

**原文标题**: LLMorphism: When humans come to see themselves as language models

**原文链接**: [https://arxiv.org/abs/2605.05419](https://arxiv.org/abs/2605.05419)

生成摘要时出错

---

## 53. Chindogu: Weird and Useless Japanese Inventions

**原文标题**: Chindogu: Weird and Useless Japanese Inventions

**原文链接**: [https://rarehistoricalphotos.com/weird-japanese-inventions/](https://rarehistoricalphotos.com/weird-japanese-inventions/)

生成摘要时出错

---

## 54. ICE to Develop Own Smart Glasses to 'Supplement' Its Facial Recognition App

**原文标题**: ICE to Develop Own Smart Glasses to 'Supplement' Its Facial Recognition App

**原文链接**: [https://www.404media.co/ice-plans-to-develop-own-smart-glasses-to-supplement-its-facial-recognition-app/](https://www.404media.co/ice-plans-to-develop-own-smart-glasses-to-supplement-its-facial-recognition-app/)

生成摘要时出错

---

## 55. Show HN: adamsreview – better multi-agent PR reviews for Claude Code

**原文标题**: Show HN: adamsreview – better multi-agent PR reviews for Claude Code

**原文链接**: [https://github.com/adamjgmiller/adamsreview](https://github.com/adamjgmiller/adamsreview)

生成摘要时出错

---

## 56. Shunting-Yard Animation

**原文标题**: Shunting-Yard Animation

**原文链接**: [https://somethingorotherwhatever.com/shunting-yard-animation/](https://somethingorotherwhatever.com/shunting-yard-animation/)

生成摘要时出错

---

## 57. Interfaze: A new model architecture built for high accuracy at scale

**原文标题**: Interfaze: A new model architecture built for high accuracy at scale

**原文链接**: [https://interfaze.ai/blog/interfaze-a-new-model-architecture-built-for-high-accuracy-at-scale](https://interfaze.ai/blog/interfaze-a-new-model-architecture-built-for-high-accuracy-at-scale)

生成摘要时出错

---

## 58. Show HN: Countries where you can leave your MacBook at a random coffee shop

**原文标题**: Show HN: Countries where you can leave your MacBook at a random coffee shop

**原文链接**: [https://vouchatlas.com](https://vouchatlas.com)

生成摘要时出错

---

## 59. Why we lose our friends as we age (2023)

**原文标题**: Why we lose our friends as we age (2023)

**原文链接**: [https://www.theatlantic.com/newsletters/archive/2023/02/friendship-aging/673026/](https://www.theatlantic.com/newsletters/archive/2023/02/friendship-aging/673026/)

生成摘要时出错

---

## 60. Taxpayers May Be Eligible for Significant Tax Refunds – If They Act by July 10

**原文标题**: Taxpayers May Be Eligible for Significant Tax Refunds – If They Act by July 10

**原文链接**: [https://www.taxpayeradvocate.irs.gov/news/nta-blog/tens-of-millions-of-taxpayers-may-be-eligible-for-significant-tax-refunds/2026/04/](https://www.taxpayeradvocate.irs.gov/news/nta-blog/tens-of-millions-of-taxpayers-may-be-eligible-for-significant-tax-refunds/2026/04/)

生成摘要时出错

---

## 61. SpaceX wants to launch a million satellites

**原文标题**: SpaceX wants to launch a million satellites

**原文链接**: [https://www.cbc.ca/news/science/spacex-data-centre-one-million-satellites-9.7117772](https://www.cbc.ca/news/science/spacex-data-centre-one-million-satellites-9.7117772)

生成摘要时出错

---

## 62. I caught the car

**原文标题**: I caught the car

**原文链接**: [https://undecidability.net/senior/](https://undecidability.net/senior/)

生成摘要时出错

---

## 63. The Adventure Family Tree (2024)

**原文标题**: The Adventure Family Tree (2024)

**原文链接**: [https://mipmip.org/advfamily/advfamily.html](https://mipmip.org/advfamily/advfamily.html)

生成摘要时出错

---

## 64. Plex's price hikes prove I was right to switch to Jellyfin

**原文标题**: Plex's price hikes prove I was right to switch to Jellyfin

**原文链接**: [https://www.androidauthority.com/plex-price-hikes-get-jellyfin-3663600/](https://www.androidauthority.com/plex-price-hikes-get-jellyfin-3663600/)

生成摘要时出错

---

## 65. Oil-price bets ahead of Iran war news totalled $7B, reporting shows

**原文标题**: Oil-price bets ahead of Iran war news totalled $7B, reporting shows

**原文链接**: [https://www.reuters.com/sustainability/boards-policy-regulation/oil-price-bets-ahead-iran-war-news-totalled-7-billion-reporting-shows-2026-05-07/](https://www.reuters.com/sustainability/boards-policy-regulation/oil-price-bets-ahead-iran-war-news-totalled-7-billion-reporting-shows-2026-05-07/)

生成摘要时出错

---

## 66. Israel's AI targeting system: data from a phone become a death sentence

**原文标题**: Israel's AI targeting system: data from a phone become a death sentence

**原文链接**: [https://www.latimes.com/world-nation/story/2026-05-04/inside-israels-ai-targeting-system-how-data-from-phone-become-death-sentence](https://www.latimes.com/world-nation/story/2026-05-04/inside-israels-ai-targeting-system-how-data-from-phone-become-death-sentence)

生成摘要时出错

---

## 67. Scaffold a 1990s Geocities-themed static website

**原文标题**: Scaffold a 1990s Geocities-themed static website

**原文链接**: [https://pypi.org/project/create-geocities-app/](https://pypi.org/project/create-geocities-app/)

生成摘要时出错

---

## 68. "openai.com" was once the personal homepage of a guy named glenn

**原文标题**: "openai.com" was once the personal homepage of a guy named glenn

**原文链接**: [https://bsky.app/profile/annierau.bsky.social/post/3mkzrvrn44c2h](https://bsky.app/profile/annierau.bsky.social/post/3mkzrvrn44c2h)

生成摘要时出错

---

## 69. The Struggle Is Gone

**原文标题**: The Struggle Is Gone

**原文链接**: [https://dogdogfish.com/blog/2026/05/10/the-struggle-is-gone/](https://dogdogfish.com/blog/2026/05/10/the-struggle-is-gone/)

生成摘要时出错

---

## 70. Iran mulls taking control of all 7 cables passing through Strait of Hormuz

**原文标题**: Iran mulls taking control of all 7 cables passing through Strait of Hormuz

**原文链接**: [https://www.wionews.com/world/iran-to-take-full-control-of-all-7-undersea-internet-cables-passing-through-strait-of-hormuz-1778361695047](https://www.wionews.com/world/iran-to-take-full-control-of-all-7-undersea-internet-cables-passing-through-strait-of-hormuz-1778361695047)

生成摘要时出错

---

## 71. Wall Street lawyers aided insider trading ring, say US prosecutors

**原文标题**: Wall Street lawyers aided insider trading ring, say US prosecutors

**原文链接**: [https://www.ft.com/content/d2fbe2c3-103a-4d09-b510-db58c5f8697d](https://www.ft.com/content/d2fbe2c3-103a-4d09-b510-db58c5f8697d)

生成摘要时出错

---

## 72. Sparse Cholesky Elimination Tree

**原文标题**: Sparse Cholesky Elimination Tree

**原文链接**: [https://www.reidatcheson.com/sparse/linear/cholesky/2026/04/09/etree.html](https://www.reidatcheson.com/sparse/linear/cholesky/2026/04/09/etree.html)

生成摘要时出错

---

## 73. Red Hot Chili Peppers ink $300M deal with Warner Music to sell catalog

**原文标题**: Red Hot Chili Peppers ink $300M deal with Warner Music to sell catalog

**原文链接**: [https://www.hollywoodreporter.com/music/music-industry-news/wmg-acquired-red-hot-chili-peppers-catalog-for-350-million-1236589567/](https://www.hollywoodreporter.com/music/music-industry-news/wmg-acquired-red-hot-chili-peppers-catalog-for-350-million-1236589567/)

生成摘要时出错

---

## 74. Should you leave red herrings about yourself online?

**原文标题**: Should you leave red herrings about yourself online?

**原文链接**: [https://blog.alcazarsec.com/posts/should-you-leave-red-herrings-about-yourself-online](https://blog.alcazarsec.com/posts/should-you-leave-red-herrings-about-yourself-online)

生成摘要时出错

---

## 75. I have seen the dystopian future of elderly care

**原文标题**: I have seen the dystopian future of elderly care

**原文链接**: [https://www.telegraph.co.uk/world-news/2026/05/09/testing-the-japanese-airec-robot-for-elderly-care/](https://www.telegraph.co.uk/world-news/2026/05/09/testing-the-japanese-airec-robot-for-elderly-care/)

生成摘要时出错

---

## 76. Data center drains 30M gals of water — until residents complained of pressure

**原文标题**: Data center drains 30M gals of water — until residents complained of pressure

**原文链接**: [https://www.politico.com/news/2026/05/08/georgia-data-centers-water-00909988](https://www.politico.com/news/2026/05/08/georgia-data-centers-water-00909988)

生成摘要时出错

---

## 77. Library for fast mapping of Java records to native memory

**原文标题**: Library for fast mapping of Java records to native memory

**原文链接**: [https://github.com/mamba-studio/TypedMemory](https://github.com/mamba-studio/TypedMemory)

生成摘要时出错

---

## 78. Palantir to be granted "unlimited access" to UK NHS patient data

**原文标题**: Palantir to be granted "unlimited access" to UK NHS patient data

**原文链接**: [https://www.digitalhealth.net/2026/05/palantir-to-be-granted-unlimited-access-to-nhs-patient-data/](https://www.digitalhealth.net/2026/05/palantir-to-be-granted-unlimited-access-to-nhs-patient-data/)

生成摘要时出错

---

## 79. UCLA discovers first stroke rehabilitation drug to repair brain damage (2025)

**原文标题**: UCLA discovers first stroke rehabilitation drug to repair brain damage (2025)

**原文链接**: [https://stemcell.ucla.edu/news/ucla-discovers-first-stroke-rehabilitation-drug-repair-brain-damage](https://stemcell.ucla.edu/news/ucla-discovers-first-stroke-rehabilitation-drug-repair-brain-damage)

生成摘要时出错

---

## 80. The OpenAI Deployment Company

**原文标题**: The OpenAI Deployment Company

**原文链接**: [https://openai.com/index/openai-launches-the-deployment-company/](https://openai.com/index/openai-launches-the-deployment-company/)

生成摘要时出错

---

## 81. Doctors Just Staged the Quietest Coup in American History

**原文标题**: Doctors Just Staged the Quietest Coup in American History

**原文链接**: [https://thegrimhistorian.substack.com/p/36-doctors-just-staged-the-quietest](https://thegrimhistorian.substack.com/p/36-doctors-just-staged-the-quietest)

生成摘要时出错

---

## 82. BLAS, Lapack and OpenMP

**原文标题**: BLAS, Lapack and OpenMP

**原文链接**: [https://pypackaging-native.github.io/key-issues/native-dependencies/blas_openmp/](https://pypackaging-native.github.io/key-issues/native-dependencies/blas_openmp/)

生成摘要时出错

---

## 83. Out with the JavaScript, in with the HTML

**原文标题**: Out with the JavaScript, in with the HTML

**原文链接**: [https://blog.jim-nielsen.com/2026/out-with-js-in-with-html/](https://blog.jim-nielsen.com/2026/out-with-js-in-with-html/)

生成摘要时出错

---

## 84. What's Wrong with AI?

**原文标题**: What's Wrong with AI?

**原文链接**: [https://kurtis.weblog.lol/2026/05/whats-wrong-with-ai](https://kurtis.weblog.lol/2026/05/whats-wrong-with-ai)

生成摘要时出错

---

## 85. I knew my writing students used AI. Their confessions led to a teaching moment

**原文标题**: I knew my writing students used AI. Their confessions led to a teaching moment

**原文链接**: [https://www.theguardian.com/us-news/ng-interactive/2026/may/10/fiction-writing-professor-ai](https://www.theguardian.com/us-news/ng-interactive/2026/may/10/fiction-writing-professor-ai)

生成摘要时出错

---

## 86. Checkmate in Iran

**原文标题**: Checkmate in Iran

**原文链接**: [https://www.theatlantic.com/international/2026/05/iran-war-trump-losing/687094/](https://www.theatlantic.com/international/2026/05/iran-war-trump-losing/687094/)

生成摘要时出错

---

## 87. Energy Prices Are Driving Demand for Solar Panels and Heat Pumps

**原文标题**: Energy Prices Are Driving Demand for Solar Panels and Heat Pumps

**原文链接**: [https://www.nytimes.com/2026/05/08/business/europe-solar-panels-iran-war.html](https://www.nytimes.com/2026/05/08/business/europe-solar-panels-iran-war.html)

生成摘要时出错

---

## 88. Forget the AI job apocalypse. AIs real threat is worker control and surveillance

**原文标题**: Forget the AI job apocalypse. AIs real threat is worker control and surveillance

**原文链接**: [https://www.theguardian.com/technology/2026/may/11/ai-worker-control-surveillance](https://www.theguardian.com/technology/2026/may/11/ai-worker-control-surveillance)

生成摘要时出错

---

## 89. Nuke All Routers

**原文标题**: Nuke All Routers

**原文链接**: [https://github.com/maxbrito500/esp32-c5-deauth](https://github.com/maxbrito500/esp32-c5-deauth)

生成摘要时出错

---

## 90. Canada's unemployment rate rises to 6.9% as economy sheds more jobs

**原文标题**: Canada's unemployment rate rises to 6.9% as economy sheds more jobs

**原文链接**: [https://financialpost.com/news/economy/canada-unemployment-rate-rises-economy-sheds-jobs](https://financialpost.com/news/economy/canada-unemployment-rate-rises-economy-sheds-jobs)

生成摘要时出错

---

## 91. Notes on using GNU Emacs' Tramp system in an unusual shell environment

**原文标题**: Notes on using GNU Emacs' Tramp system in an unusual shell environment

**原文链接**: [https://utcc.utoronto.ca/~cks/space/blog/programming/EmacsTrampNotes](https://utcc.utoronto.ca/~cks/space/blog/programming/EmacsTrampNotes)

生成摘要时出错

---

## 92. Using AI for just 10 minutes might make you lazy and dumb

**原文标题**: Using AI for just 10 minutes might make you lazy and dumb

**原文链接**: [https://www.wired.com/story/using-ai-negative-impact-thinking-problem-solving-study/](https://www.wired.com/story/using-ai-negative-impact-thinking-problem-solving-study/)

生成摘要时出错

---

## 93. Organized Dogmatism Controls the Message about Gender Bias in the Academy

**原文标题**: Organized Dogmatism Controls the Message about Gender Bias in the Academy

**原文链接**: [https://journalofcontroversialideas.org/article/6/1/313](https://journalofcontroversialideas.org/article/6/1/313)

生成摘要时出错

---

## 94. Scouting's Real Crisis Is Not Marketing. It Is Decades of Neglect.

**原文标题**: Scouting's Real Crisis Is Not Marketing. It Is Decades of Neglect.

**原文链接**: [https://www.untendedfire.org/2026/05/09/scoutings-real-crisis-is-not-marketing-it-is-decades-of-neglect/](https://www.untendedfire.org/2026/05/09/scoutings-real-crisis-is-not-marketing-it-is-decades-of-neglect/)

生成摘要时出错

---

## 95. Gibraltar dumping all of its raw sewage into Mediterranean

**原文标题**: Gibraltar dumping all of its raw sewage into Mediterranean

**原文链接**: [https://www.theguardian.com/world/2026/may/06/uk-territory-gibraltar-dumps-raw-sewage-mediterranean](https://www.theguardian.com/world/2026/may/06/uk-territory-gibraltar-dumps-raw-sewage-mediterranean)

生成摘要时出错

---

## 96. 590k buyers paid $59M for Trump's gold phone, but not one has shipped

**原文标题**: 590k buyers paid $59M for Trump's gold phone, but not one has shipped

**原文链接**: [https://finance.yahoo.com/markets/stocks/articles/590-000-buyers-paid-59-223500998.html](https://finance.yahoo.com/markets/stocks/articles/590-000-buyers-paid-59-223500998.html)

生成摘要时出错

---

## 97. Canvas got hacked, provost banned exams, professor responded by assigning Hayek

**原文标题**: Canvas got hacked, provost banned exams, professor responded by assigning Hayek

**原文链接**: [https://old.reddit.com/r/UIUC/comments/1ta8b3o/i_opened_my_email_expecting_exam_postponed_hang/](https://old.reddit.com/r/UIUC/comments/1ta8b3o/i_opened_my_email_expecting_exam_postponed_hang/)

生成摘要时出错

---

## 98. Why do Oregon farms plant red clover every spring?

**原文标题**: Why do Oregon farms plant red clover every spring?

**原文链接**: [https://a.wholelottanothing.org/why-do-oregon-farms-plant-red-clover-every-spring/](https://a.wholelottanothing.org/why-do-oregon-farms-plant-red-clover-every-spring/)

生成摘要时出错

---

## 99. 10 Trillion downloads are crushing open-source repositories

**原文标题**: 10 Trillion downloads are crushing open-source repositories

**原文链接**: [https://www.zdnet.com/article/open-source-repositories-are-being-overwhelmed-but-there-is-an-answer/](https://www.zdnet.com/article/open-source-repositories-are-being-overwhelmed-but-there-is-an-answer/)

生成摘要时出错

---

## 100. What a Japanese cooking principle taught me about overcoming AI fatigue

**原文标题**: What a Japanese cooking principle taught me about overcoming AI fatigue

**原文链接**: [https://www.devas.life/what-a-japanese-cooking-principle-taught-me-about-overcoming-ai-fatigue/](https://www.devas.life/what-a-japanese-cooking-principle-taught-me-about-overcoming-ai-fatigue/)

生成摘要时出错

---

