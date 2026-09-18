# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-09-18.md)

*最后自动更新时间: 2026-09-18 21:56:04*
## 1. 微软高管将AI数据爬取称为“人类历史上最大的劳动盗窃”。

**原文标题**: Microsoft exec called AI scraping 'the largest theft of labor in human history'

**原文链接**: [https://techcrunch.com/2026/09/17/microsoft-exec-called-ai-scraping-the-largest-theft-of-labor-in-human-history-new-unredacted-filings-reveal/](https://techcrunch.com/2026/09/17/microsoft-exec-called-ai-scraping-the-largest-theft-of-labor-in-human-history-new-unredacted-filings-reveal/)

《纽约时报》对OpenAI和微软提起的版权诉讼中最新披露的未经修订的信息显示，这些公司内部承认，AI抓取构成“人类历史上最大的劳动窃取”，并对出版业构成“生存威胁”。

微软高管布伦特·赫克特（Brent Hecht）在一份内部备忘录中使用了“最大窃取”这一表述，而OpenAI的领导层则承认，在“擅长新闻”且“在很大程度上可以替代”原创内容的AI模型面前存在“生存威胁”。诉讼文件详细说明了这些公司如何涉嫌绕过付费墙（OpenAI总裁格雷格·布罗克曼（Greg Brockman）在得知一次“破解”后回应“啊，真不错”），构建了庞大的训练数据集，并蓄意去除了版权声明。

这些披露严重削弱了这些公司“合理使用”的辩护。微软首席执行官萨蒂亚·纳德拉（Satya Nadella）作证称，付费墙内容应获得许可，如果他知道存在付费墙抓取行为，他会要求OpenAI重新训练模型。微软自己的数据显示，其Copilot导致《纽约时报》的点击率下降了93%，这说明了直接的市场损害。

复制的规模也得以披露：OpenAI的中期训练数据集包含来自《纽约时报》、《每日新闻》和调查报道中心91,000多份作品的副本，而一个源自Common Crawl的数据集则包含来自nytimes.com的200多万份文档。这些文件还显示，OpenAI和微软通过“出租车项目”（Project Taxi）和“芒果项目”（Mango）等计划进行了广泛的数据共享。原告律师表示，这些证据证明这些公司“明知其行为是错误的”。OpenAI和微软拒绝置评。

---

## 2. 我 不喜欢 通行密钥

**原文标题**: I don't like passkeys

**原文链接**: [https://hawksley.dev/blog/i-dont-like-passkeys](https://hawksley.dev/blog/i-dont-like-passkeys)

本文反对个人用户广泛采用通行密钥，尽管承认其在防止网络钓鱼和增强数据泄露安全性方面的技术优势。作者认为，虽然通行密钥非常适合企业环境，但对个人而言，它们带来了更大的潜在风险，例如永久账户锁定、自动封禁和设备丢失。

强调的关键问题包括硬件密钥的局限性，它们无法备份、价格昂贵、不易扩展、账户容量有限，通常需要多次购买。绑定到苹果或谷歌账户的同步通行密钥，一旦主操作系统账户被封禁，就有可能永久失去对所有第三方账户的访问权限，而且其导出/互操作性功能目前尚不成熟。

使用第三方密码管理器存储通行密钥会导致用户体验碎片化和自动填充不一致。在共享设备上登录很不方便，依赖于不甚理想的解决方案，例如硬件密钥、信任未知的计算机来同步密钥，或者容易出错的混合传输方法。

作者总结道，通行密钥尚未成熟到足以供个人使用。对于大多数个人而言，账户锁定和恢复问题的风险大于其对抗高级网络钓鱼攻击的益处。相反，文章建议结合使用存储在第三方管理器中的随机生成密码和独立的TOTP应用程序。通行密钥只对那些以前重复使用密码的用户而言是实质性的改进；对其他人来说，它们目前代表着一种倒退。

---

## 3. Hister：您的私人搜索引擎，用于检索您访问的网页和保存的文件

**原文标题**: Hister: A private search engine for the pages you visit and the files you keep

**原文链接**: [https://github.com/asciimoo/hister](https://github.com/asciimoo/hister)

Hister是一款私有、自托管的搜索引擎，旨在索引您访问过的网页以及您本地存储的文件内容的全文。它允许用户通过网页界面、终端或通过MCP连接的AI助手轻松检索信息。

Hister强调隐私，不包含遥测或强制性云服务，允许用户在本地或自己的基础设施上运行它。它提供全文索引、强大的查询选项（包括通配符和否定），以及通过用户配置的嵌入端点实现可选的语义搜索。Hister支持通过Firefox或Chrome浏览器扩展自动索引新访问的页面，并允许导入现有的浏览器历史记录、本地目录或单个文件。多用户支持可在共享服务器上保持数据分离。

开始使用只需下载二进制文件，运行`hister listen`，并安装浏览器扩展。其他安装方法包括Homebrew、Docker和Nix。Hister的独特之处在于它创建了一个个人化、可控的搜索索引，确保您的数据保留在您的服务器上，而不依赖第三方搜索提供商。它采用AGPLv3许可证。

---

## 4. 本德——一种通过证明阻止AI错误并支持GPU运行的语言

**原文标题**: Bend – a language that blocks AI mistakes via proof and runs on GPUs

**原文链接**: [https://bend-lang.com/](https://bend-lang.com/)

Bend是一种编程语言，旨在防止人工智能生成的错误，并确保可靠、高性能的应用程序，特别是在后AGI时代。它的主要功能是通过一个基于证明的系统来阻止bug：开发者在`LAWS.bend`中定义关键规则，AI代理在提交任何更改之前，必须通过`PROOF.bend`数学证明其代码符合这些规则。这确保了代码的正确性，并使得合并一个bug在数学上成为不可能。

除了基于证明的安全性，Bend还强调速度和并行性。它编译成原生代码，在单核上提供类C语言的性能，并通过自动利用多个CPU核心或GPU，实现高达100倍的执行速度，而无需手动管理线程或内核。Bend的类型检查器（即证明检查器）速度极快，在数秒内完成验证，使AI代理能够快速迭代更改。

Bend拥有类似Python的语法，集成了C语言的速度、CUDA的并行性以及Lean的证明系统。要开始使用，用户通过一个简单的脚本安装它，并通过在`AGENTS.md`中添加特定指南来指示他们的AI代理使用Bend。它非常适合在Linux和macOS上进行无bug、快速的后端开发。

---

## 5. 阿斯特拉 法律版

**原文标题**: Astra for Law

**原文链接**: [https://openai.com/index/astra-for-law/](https://openai.com/index/astra-for-law/)

2026年9月17日，OpenAI推出了“法律版Astra”，这是一个专为律师事务所和法律科技公司量身定制的新型AI基础系统。该系统将OpenAI最强大的模型GPT-6 Astra与针对专业法律工作的专用设置、工具和上下文相结合。

法律版Astra包含一个强大的法律搜索索引，能够搜索超过2.3亿份美国法律资料，包括判例法、法规和条例，数据来自Free Law Project。这显著增强了法律研究能力，在Vals AI法律研究基准测试中，与仅使用网页搜索的GPT-6 Astra相比，整体正确性相对提高了40%，并检索到更多相关段落。除了研究，它还采用自定义指令进行高级法律分析和写作，改进了识别相关判例和匹配事实模式等任务。

隐私和治理是核心考量，符合条件的律所可以通过“可信访问计划”享受API的零数据保留，并将ChatGPT企业版的使用排除在人工审查之外。OpenAI还与Latham & Watkins（瑞生律师事务所）合作，设计强大的客户保密控制措施。

该平台具有高度可定制性，支持26个新的生态系统插件，可与Relativity、Clio、iManage、Intapp和Thomson Reuters的HighQ等现有法律工具连接。包括Sullivan & Cromwell（苏利文与克伦威尔律师事务所）、Ropes & Gray（礼德律师事务所）和Cooley（科律律师事务所）在内的多家律师事务所已经构建了定制的AI应用程序，用于协议分析、交易尽职调查和IPO准备等任务。适用于法律起草的ChatGPT for Word也已普遍可用。

法律版Astra将首先通过ChatGPT和Codex中的“可信访问”提供，随后通过API提供。OpenAI强调其在法律AI领域的长期投资，推动建立一个开放的生态系统，供律所整合其独特的专业知识和现有解决方案。

---

## 6. Bonsai 2 27B：近无损压缩，占用空间缩小9倍

**原文标题**: Bonsai 2 27B: Near-Lossless Compression in a 9x Smaller Footprint

**原文链接**: [https://prismml.com/news/bonsai-2-27b](https://prismml.com/news/bonsai-2-27b)

PrismML 发布了 Bonsai 2 27B，这是一款开创性的多模态AI模型，以显著减小的占用空间实现了近乎无损压缩。该模型基于 Qwen3.8 27B，提供了增强的推理、编码、视觉和智能体能力。

该模型采用三元 {-1, 0, +1} 权重并结合 FP16 分组缩放，实现了每个权重有效 1.76 比特，总内存占用仅为 5.9GB。这使其比其全精度等效模型小 9 倍以上，同时仍保持了在各种任务中令人印象深刻的 98.2% 综合基准性能。这显著超越了之前 Bonsai 27B 的 95% 能力保持率，使 Bonsai 2 27B 在能力方面几乎“无损”。

Bonsai 2 27B 支持 262K token 的上下文窗口以及多模态文本和图像输入。其高智能密度实现了高效的本地部署，具有卓越的吞吐量（例如，在 NVIDIA RTX 5090 上达到每秒 143 token）和能源效率（比 8B 全精度模型效率高 40%）。这使得复杂的本地应用成为可能，例如编码智能体、计算机使用工作流和私人文档分析。

此次发布在 Apache 2.0 许可下可用，它从根本上改变了 AI 系统的经济性和架构，通过在严格的内存、计算和功耗预算内优化能力，将部署范围从个人设备扩展到大型数据中心。它通过 NVIDIA GPU 上的 CUDA 以及 Apple 设备上的 MLX 运行。

---

## 7. 开源杰夫

**原文标题**: OpenJev

**原文链接**: [https://openjev.com/](https://openjev.com/)

The document "OpenJev" outlines a specific methodology for interpreting model output, emphasizing "direct readoutChoice probabilitiesno decoding." It instructs users to read the model's raw "choice logits" and normalize these values *only* across the options that were explicitly supplied. This approach suggests a focus on straightforward, un-decoded interpretation of model predictions. The mention of "waiting for a run" indicates these instructions are preparatory steps for an impending execution or evaluation within the OpenJev system. The text thus defines a precise, constrained method for output interpretation, likely aimed at specific analysis or evaluation tasks within the OpenJev project.

---

## 8. Cloudflare Quick Tunnels

**原文标题**: Cloudflare Quick Tunnels

**原文链接**: [https://try.cloudflare.com/](https://try.cloudflare.com/)

生成摘要时出错

---

## 9. A heap overflow and SSO misconfiguration to compromise OpenAI internal repos

**原文标题**: A heap overflow and SSO misconfiguration to compromise OpenAI internal repos

**原文链接**: [https://www.hacktron.ai/blog/hacking-openai](https://www.hacktron.ai/blog/hacking-openai)

生成摘要时出错

---

## 10. How GLM built its own inference infrastructure

**原文标题**: How GLM built its own inference infrastructure

**原文链接**: [https://z.ai/blog/glm-built-its-inference-infrastructure](https://z.ai/blog/glm-built-its-inference-infrastructure)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-09-18](output/hacker_news_summary_2026-09-18.md) |
| 2 | [2026-09-17](output/hacker_news_summary_2026-09-17.md) |
| 3 | [2026-09-16](output/hacker_news_summary_2026-09-16.md) |
| 4 | [2026-09-09](output/hacker_news_summary_2026-09-09.md) |
| 5 | [2026-09-10](output/hacker_news_summary_2026-09-10.md) |
| 6 | [2026-09-15](output/hacker_news_summary_2026-09-15.md) |
| 7 | [2026-09-14](output/hacker_news_summary_2026-09-14.md) |
| 8 | [2026-09-11](output/hacker_news_summary_2026-09-11.md) |
| 9 | [2026-09-13](output/hacker_news_summary_2026-09-13.md) |
| 10 | [2026-09-12](output/hacker_news_summary_2026-09-12.md) |
| 11 | [2026-09-04](output/hacker_news_summary_2026-09-04.md) |
| 12 | [2026-09-07](output/hacker_news_summary_2026-09-07.md) |
| 13 | [2026-09-01](output/hacker_news_summary_2026-09-01.md) |
| 14 | [2026-09-08](output/hacker_news_summary_2026-09-08.md) |
| 15 | [2026-09-03](output/hacker_news_summary_2026-09-03.md) |
| 16 | [2026-09-02](output/hacker_news_summary_2026-09-02.md) |
| 17 | [2026-09-05](output/hacker_news_summary_2026-09-05.md) |
| 18 | [2026-09-06](output/hacker_news_summary_2026-09-06.md) |
| 19 | [2026-08-25](output/hacker_news_summary_2026-08-25.md) |
| 20 | [2026-08-26](output/hacker_news_summary_2026-08-26.md) |
| 21 | [2026-08-23](output/hacker_news_summary_2026-08-23.md) |
| 22 | [2026-08-31](output/hacker_news_summary_2026-08-31.md) |
| 23 | [2026-08-28](output/hacker_news_summary_2026-08-28.md) |
| 24 | [2026-08-24](output/hacker_news_summary_2026-08-24.md) |
| 25 | [2026-08-30](output/hacker_news_summary_2026-08-30.md) |
| 26 | [2026-08-29](output/hacker_news_summary_2026-08-29.md) |
| 27 | [2026-08-20](output/hacker_news_summary_2026-08-20.md) |
| 28 | [2026-08-14](output/hacker_news_summary_2026-08-14.md) |
| 29 | [2026-08-18](output/hacker_news_summary_2026-08-18.md) |
| 30 | [2026-08-19](output/hacker_news_summary_2026-08-19.md) |
| 31 | [2026-08-21](output/hacker_news_summary_2026-08-21.md) |
| 32 | [2026-08-17](output/hacker_news_summary_2026-08-17.md) |
| 33 | [2026-08-16](output/hacker_news_summary_2026-08-16.md) |
| 34 | [2026-08-22](output/hacker_news_summary_2026-08-22.md) |
| 35 | [2026-08-15](output/hacker_news_summary_2026-08-15.md) |
| 36 | [2026-08-12](output/hacker_news_summary_2026-08-12.md) |
| 37 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 38 | [2026-08-10](output/hacker_news_summary_2026-08-10.md) |
| 39 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 40 | [2026-08-11](output/hacker_news_summary_2026-08-11.md) |
| 41 | [2026-08-09](output/hacker_news_summary_2026-08-09.md) |
| 42 | [2026-08-13](output/hacker_news_summary_2026-08-13.md) |
| 43 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 44 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 45 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 46 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 47 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 48 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 49 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 50 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 51 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 52 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 53 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 54 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 55 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 56 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 57 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 58 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 59 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 60 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 61 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 62 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 63 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 64 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 65 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 66 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 67 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 68 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 69 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 70 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 71 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 72 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 73 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 74 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 75 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 76 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 77 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 78 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 79 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 80 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 81 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 82 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 83 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 84 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 85 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 86 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 87 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 88 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 89 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 90 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 91 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 92 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 93 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 94 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 95 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 96 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 97 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 98 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 99 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 100 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 101 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 102 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 103 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 104 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 105 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 106 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 107 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 108 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 109 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 110 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 111 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 112 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 113 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 114 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 115 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 116 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 117 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 118 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 119 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 120 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 121 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 122 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 123 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 124 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 125 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 126 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 127 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 128 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 129 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 130 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 131 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 132 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 133 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 134 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 135 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 136 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 137 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 138 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 139 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 140 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 141 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 142 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 143 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 144 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 145 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 146 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 147 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 148 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 149 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 150 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 151 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 152 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 153 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 154 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 155 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 156 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 157 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 158 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 159 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 160 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 161 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 162 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 163 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 164 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 165 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 166 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 167 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 168 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 169 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 170 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 171 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 172 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 173 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 174 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 175 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 176 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 177 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 178 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 179 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 180 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 181 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 182 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 183 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 184 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 185 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 186 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 187 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 188 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 189 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 190 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 191 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 192 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 193 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 194 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 195 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 196 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 197 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 198 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 199 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 200 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 201 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 202 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 203 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 204 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 205 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 206 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 207 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 208 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 209 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 210 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 211 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 212 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 213 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 214 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 215 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 216 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 217 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 218 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 219 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 220 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 221 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 222 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 223 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 224 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 225 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 226 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 227 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 228 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 229 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 230 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 231 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 232 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 233 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 234 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 235 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 236 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 237 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 238 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 239 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 240 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 241 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 242 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 243 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 244 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 245 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 246 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 247 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 248 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 249 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 250 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 251 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 252 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 253 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 254 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 255 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 256 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 257 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 258 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 259 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 260 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 261 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 262 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 263 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 264 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 265 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 266 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 267 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 268 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 269 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 270 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 271 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 272 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 273 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 274 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 275 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 276 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 277 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 278 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 279 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 280 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 281 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 282 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 283 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 284 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 285 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 286 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 287 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 288 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 289 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 290 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 291 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 292 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 293 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 294 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 295 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 296 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 297 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 298 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 299 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 300 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 301 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 302 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 303 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 304 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 305 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 306 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 307 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 308 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 309 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 310 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 311 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 312 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 313 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
