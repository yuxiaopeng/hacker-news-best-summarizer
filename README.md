# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-05-11.md)

*最后自动更新时间: 2026-05-11 21:13:32*
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

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 2 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 3 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 4 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 5 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 6 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 7 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 8 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 9 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 10 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 11 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 12 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 13 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 14 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 15 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 16 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 17 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 18 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 19 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 20 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 21 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 22 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 23 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 24 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 25 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 26 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 27 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 28 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 29 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 30 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 31 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 32 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 33 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 34 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 35 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 36 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 37 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 38 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 39 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 40 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 41 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 42 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 43 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 44 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 45 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 46 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 47 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 48 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 49 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 50 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 51 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 52 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 53 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 54 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 55 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 56 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 57 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 58 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 59 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 60 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 61 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 62 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 63 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 64 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 65 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 66 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 67 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 68 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 69 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 70 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 71 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 72 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 73 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 74 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 75 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 76 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 77 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 78 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 79 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 80 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 81 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 82 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 83 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 84 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 85 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 86 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 87 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 88 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 89 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 90 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 91 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 92 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 93 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 94 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 95 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 96 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 97 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 98 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 99 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 100 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 101 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 102 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 103 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 104 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 105 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 106 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 107 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 108 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 109 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 110 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 111 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 112 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 113 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 114 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 115 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 116 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 117 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 118 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 119 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 120 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 121 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 122 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 123 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 124 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 125 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 126 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 127 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 128 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 129 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 130 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 131 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 132 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 133 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 134 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 135 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 136 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 137 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 138 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 139 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 140 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 141 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 142 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 143 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 144 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 145 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 146 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 147 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 148 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 149 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 150 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 151 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 152 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 153 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 154 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 155 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 156 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 157 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 158 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 159 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 160 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 161 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 162 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 163 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 164 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 165 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 166 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 167 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 168 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 169 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 170 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 171 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 172 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 173 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 174 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 175 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 176 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 177 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 178 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 179 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 180 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 181 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 182 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 183 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 184 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 185 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
