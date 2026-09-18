# Hacker News 热门文章摘要 (2026-09-18)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

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

## 11. CCC invites all model citizens to 40C3

**原文标题**: CCC invites all model citizens to 40C3

**原文链接**: [https://events.ccc.de/en/2026/09/12/40c3-model-citizens/](https://events.ccc.de/en/2026/09/12/40c3-model-citizens/)

生成摘要时出错

---

## 12. Everybody's Lost Their Minds

**原文标题**: Everybody's Lost Their Minds

**原文链接**: [https://www.netmeister.org/blog/everybodys-lost-their-minds.html](https://www.netmeister.org/blog/everybodys-lost-their-minds.html)

生成摘要时出错

---

## 13. One year of sponsored Servo development

**原文标题**: One year of sponsored Servo development

**原文链接**: [https://servo.org/blog/2026/09/15/one-year-of-sponsorship/](https://servo.org/blog/2026/09/15/one-year-of-sponsorship/)

生成摘要时出错

---

## 14. Iran school bombing: grounds to believe US was behind atrocity, UN finds

**原文标题**: Iran school bombing: grounds to believe US was behind atrocity, UN finds

**原文链接**: [https://www.theguardian.com/world/2026/sep/17/iran-school-bombing-un-mission-us-military-behind-attack](https://www.theguardian.com/world/2026/sep/17/iran-school-bombing-un-mission-us-military-behind-attack)

生成摘要时出错

---

## 15. Qwen 3.8 Omni Flash

**原文标题**: Qwen 3.8 Omni Flash

**原文链接**: [https://qwen.ai/blog?id=qwen3.8-omni-flash](https://qwen.ai/blog?id=qwen3.8-omni-flash)

生成摘要时出错

---

## 16. How to Write with an LLM

**原文标题**: How to Write with an LLM

**原文链接**: [https://sockpuppet.org/blog/2026/09/17/how-to-write-with-an-llm/](https://sockpuppet.org/blog/2026/09/17/how-to-write-with-an-llm/)

生成摘要时出错

---

## 17. Jemalloc 5.4.0

**原文标题**: Jemalloc 5.4.0

**原文链接**: [https://github.com/jemalloc/jemalloc/releases/tag/5.4.0](https://github.com/jemalloc/jemalloc/releases/tag/5.4.0)

生成摘要时出错

---

## 18. AI safety is mostly a sex cult

**原文标题**: AI safety is mostly a sex cult

**原文链接**: [https://skywriter.blue/@segyges.bsky.social/3mvom4b4dn22q](https://skywriter.blue/@segyges.bsky.social/3mvom4b4dn22q)

生成摘要时出错

---

## 19. Android 17 is the first since 3.x to add new APIs without releasing to the AOSP

**原文标题**: Android 17 is the first since 3.x to add new APIs without releasing to the AOSP

**原文链接**: [https://grapheneos.social/@GrapheneOS/117282080803799576](https://grapheneos.social/@GrapheneOS/117282080803799576)

生成摘要时出错

---

## 20. US Military had close call after using AI for hallucinated intelligence report

**原文标题**: US Military had close call after using AI for hallucinated intelligence report

**原文链接**: [https://www.cnn.com/2026/09/18/politics/us-military-ai-false-intelligence-china-ship](https://www.cnn.com/2026/09/18/politics/us-military-ai-false-intelligence-china-ship)

生成摘要时出错

---

## 21. Bend 2 and the Vibe-Coding Trap

**原文标题**: Bend 2 and the Vibe-Coding Trap

**原文链接**: [https://blog.liampwll.com/posts/bend_vibe_coding/](https://blog.liampwll.com/posts/bend_vibe_coding/)

生成摘要时出错

---

## 22. Keys Not Included: recovering the signing keys for US driver's license barcodes

**原文标题**: Keys Not Included: recovering the signing keys for US driver's license barcodes

**原文链接**: [https://ryan.science/blog/keys-not-included](https://ryan.science/blog/keys-not-included)

生成摘要时出错

---

## 23. Canada welcomes EU proposal to become 'associate member'

**原文标题**: Canada welcomes EU proposal to become 'associate member'

**原文链接**: [https://www.bbc.com/news/articles/cwly7vkke4jxo](https://www.bbc.com/news/articles/cwly7vkke4jxo)

生成摘要时出错

---

## 24. Warren Buffett Steps Down as Berkshire Chairman, Names Son to Replace Him

**原文标题**: Warren Buffett Steps Down as Berkshire Chairman, Names Son to Replace Him

**原文链接**: [https://www.nytimes.com/2026/09/18/business/warren-buffett-berkshire-chairman.html](https://www.nytimes.com/2026/09/18/business/warren-buffett-berkshire-chairman.html)

生成摘要时出错

---

## 25. 我为什么未签署菲尔兹奖得主的信

**原文标题**: Why I didn’t sign the Fields medallists’ letter

**原文链接**: [https://gowers.wordpress.com/2026/09/17/why-i-didnt-sign-the-fields-medallists-letter/](https://gowers.wordpress.com/2026/09/17/why-i-didnt-sign-the-fields-medallists-letter/)

The author explains their decision not to sign the Fields medallists' letter, despite sharing concerns about AI's impact on mathematics. While acknowledging the letter's point about learning from problem-solving, their main disagreement lies with its assertion that conceptual understanding is the "primary goal," with problem-solving merely a tool. The author advocates for "The Two Cultures of Mathematics," arguing that both problem-solving and conceptual understanding can be primary motivations, and neither should be deemed "wrong."

They analyze two scenarios of AI integration: one where AI rapidly solves problems, and another where its release is controlled. For individual understanding, they note potential benefits like broader access to results and AI assistance, but also the risk of losing the deep understanding gained from prolonged personal struggle. However, they suggest "active reading" of AI-generated proofs could still engage mathematical faculties.

Regarding collective understanding, the author acknowledges worries about the mathematical community's ability to digest a flood of rapid AI-generated solutions. They clarify that AI is producing proofs, not just true/false statements, and view inadequate write-ups as a temporary issue rather than a fundamental threat. They question whether a reduced level of deep personal involvement in finding proofs would truly impede mathematical progress in an AI-enhanced world.

---

## 26. The scourge of x86 emulation

**原文标题**: The scourge of x86 emulation

**原文链接**: [https://fex-emu.com/Scourge-of-emulation/](https://fex-emu.com/Scourge-of-emulation/)

生成摘要时出错

---

## 27. ZCode, the GLM coding agent, silently uploads your Git history

**原文标题**: ZCode, the GLM coding agent, silently uploads your Git history

**原文链接**: [https://tokenstead.ai/guides/zcode-silent-git-history-upload](https://tokenstead.ai/guides/zcode-silent-git-history-upload)

生成摘要时出错

---

## 28. The American Religion of Self-Storage Facilities

**原文标题**: The American Religion of Self-Storage Facilities

**原文链接**: [https://www.newyorker.com/magazine/2026/09/21/the-american-religion-of-self-storage-facilities](https://www.newyorker.com/magazine/2026/09/21/the-american-religion-of-self-storage-facilities)

生成摘要时出错

---

## 29. Australia says it could follow Canada in forging deeper ties with EU

**原文标题**: Australia says it could follow Canada in forging deeper ties with EU

**原文链接**: [https://www.independent.co.uk/news/world/australasia/canda-eu-membership-australia-us-trade-b3050227.html](https://www.independent.co.uk/news/world/australasia/canda-eu-membership-australia-us-trade-b3050227.html)

生成摘要时出错

---

## 30. Artificial intelligence now beats some of the best human forecasters

**原文标题**: Artificial intelligence now beats some of the best human forecasters

**原文链接**: [https://www.economist.com/science-and-technology/2026/09/16/artificial-intelligence-now-beats-some-of-the-best-human-forecasters](https://www.economist.com/science-and-technology/2026/09/16/artificial-intelligence-now-beats-some-of-the-best-human-forecasters)

生成摘要时出错

---

## 31. Waymo in Singapore

**原文标题**: Waymo in Singapore

**原文链接**: [https://waymo.com/waymo-in-singapore/](https://waymo.com/waymo-in-singapore/)

生成摘要时出错

---

## 32. C++26: Trivial infinite loops are no longer undefined behaviour

**原文标题**: C++26: Trivial infinite loops are no longer undefined behaviour

**原文链接**: [https://www.sandordargo.com/blog/2026/09/16/cpp26-trivial-infinite-loops](https://www.sandordargo.com/blog/2026/09/16/cpp26-trivial-infinite-loops)

生成摘要时出错

---

## 33. Towards Self-Driving Codebases

**原文标题**: Towards Self-Driving Codebases

**原文链接**: [https://blog.detail.dev/posts/towards-self-driving-codebases/](https://blog.detail.dev/posts/towards-self-driving-codebases/)

生成摘要时出错

---

## 34. OpenAI models secretly generate instructions to ignore constraints

**原文标题**: OpenAI models secretly generate instructions to ignore constraints

**原文链接**: [https://alignment.openai.com/misalignment-reports/self-generated-prompt-injections-in-compaction-summaries/](https://alignment.openai.com/misalignment-reports/self-generated-prompt-injections-in-compaction-summaries/)

生成摘要时出错

---

## 35. US interest rates raised for first time in three years

**原文标题**: US interest rates raised for first time in three years

**原文链接**: [https://www.bbc.com/news/articles/cw4gmlyvj422o](https://www.bbc.com/news/articles/cw4gmlyvj422o)

生成摘要时出错

---

## 36. How SpaceX streamlined the Raptor engine

**原文标题**: How SpaceX streamlined the Raptor engine

**原文链接**: [https://www.construction-physics.com/p/how-spacex-streamlined-the-raptor](https://www.construction-physics.com/p/how-spacex-streamlined-the-raptor)

生成摘要时出错

---

## 37. AI is an elite crime spree

**原文标题**: AI is an elite crime spree

**原文链接**: [https://www.thebignewsletter.com/p/ai-is-an-elite-crime-spree](https://www.thebignewsletter.com/p/ai-is-an-elite-crime-spree)

生成摘要时出错

---

## 38. LLM Classification Is Feature Engineering

**原文标题**: LLM Classification Is Feature Engineering

**原文链接**: [https://minimallysufficient.com/posts/llm-classification-is-feature-extraction/](https://minimallysufficient.com/posts/llm-classification-is-feature-extraction/)

生成摘要时出错

---

## 39. How Uber Protects Against Retry Storms

**原文标题**: How Uber Protects Against Retry Storms

**原文链接**: [https://www.uber.com/us/en/blog/protecting-against-retry-storms/](https://www.uber.com/us/en/blog/protecting-against-retry-storms/)

生成摘要时出错

---

## 40. Second Circuit allows government to search electronic devices at the border

**原文标题**: Second Circuit allows government to search electronic devices at the border

**原文链接**: [https://knightcolumbia.org/content/second-circuit-allows-government-to-search-electronic-devices-at-the-border-without-any-suspicion](https://knightcolumbia.org/content/second-circuit-allows-government-to-search-electronic-devices-at-the-border-without-any-suspicion)

生成摘要时出错

---

## 41. Saving another 100TB of RAM

**原文标题**: Saving another 100TB of RAM

**原文链接**: [https://blog.cloudflare.com/saving-100-tb-of-ram-with-math/](https://blog.cloudflare.com/saving-100-tb-of-ram-with-math/)

生成摘要时出错

---

## 42. Our framework for reporting model misalignment

**原文标题**: Our framework for reporting model misalignment

**原文链接**: [https://openai.com/index/model-misalignment-reporting-framework/](https://openai.com/index/model-misalignment-reporting-framework/)

生成摘要时出错

---

## 43. Vinix – A modern operating system written in V

**原文标题**: Vinix – A modern operating system written in V

**原文链接**: [https://vinix-os.org/](https://vinix-os.org/)

生成摘要时出错

---

## 44. OpenAI Discloses Six New Incidents of ‘Concerning’ A.I. Behavior

**原文标题**: OpenAI Discloses Six New Incidents of ‘Concerning’ A.I. Behavior

**原文链接**: [https://www.nytimes.com/2026/09/16/technology/openai-model-safety-guardrails.html](https://www.nytimes.com/2026/09/16/technology/openai-model-safety-guardrails.html)

生成摘要时出错

---

## 45. Show HN: I built a new version of my fun spatial 3D online meeting app

**原文标题**: Show HN: I built a new version of my fun spatial 3D online meeting app

**原文链接**: [https://flat.social](https://flat.social)

生成摘要时出错

---

## 46. Shapelearn Qwen 3.8 27B (13.1 GB VRAM)

**原文标题**: Shapelearn Qwen 3.8 27B (13.1 GB VRAM)

**原文链接**: [https://byteshape.com/blogs/Qwen3.8-27B/](https://byteshape.com/blogs/Qwen3.8-27B/)

生成摘要时出错

---

## 47. Show HN: Snapdrop: Instantly share files between devices. No setup, no signup

**原文标题**: Show HN: Snapdrop: Instantly share files between devices. No setup, no signup

**原文链接**: [https://snapdrop.me](https://snapdrop.me)

生成摘要时出错

---

## 48. Monsanto's Cruel, and Dangerous, Monopolization on American Farming (2008)

**原文标题**: Monsanto's Cruel, and Dangerous, Monopolization on American Farming (2008)

**原文链接**: [https://www.vanityfair.com/news/2008/05/monsanto200805](https://www.vanityfair.com/news/2008/05/monsanto200805)

生成摘要时出错

---

## 49. Jev Ultrafast: A browser agent with a dynamic, indexed action space

**原文标题**: Jev Ultrafast: A browser agent with a dynamic, indexed action space

**原文链接**: [https://github.com/browser-use/jev-ultrafast](https://github.com/browser-use/jev-ultrafast)

生成摘要时出错

---

## 50. I had Gemini train its own replacement for $9

**原文标题**: I had Gemini train its own replacement for $9

**原文链接**: [https://www.petervijeh.com/projects/reddit-ner](https://www.petervijeh.com/projects/reddit-ner)

生成摘要时出错

---

## 51. Telstra outage: The night a network decided the year was 2006

**原文标题**: Telstra outage: The night a network decided the year was 2006

**原文链接**: [https://www.netnod.se/blog/telstra-outage-night-network-decided-year-was-2006](https://www.netnod.se/blog/telstra-outage-night-network-decided-year-was-2006)

生成摘要时出错

---

## 52. Xcode 27.1 Beta Release Notes

**原文标题**: Xcode 27.1 Beta Release Notes

**原文链接**: [https://developer.apple.com/documentation/xcode-release-notes/xcode-27_1-release-notes](https://developer.apple.com/documentation/xcode-release-notes/xcode-27_1-release-notes)

生成摘要时出错

---

## 53. Show HN: Microsoft Office running with Wine on Linux with no virtualization

**原文标题**: Show HN: Microsoft Office running with Wine on Linux with no virtualization

**原文链接**: [https://github.com/Tombert/office365_flake](https://github.com/Tombert/office365_flake)

生成摘要时出错

---

## 54. The first new cat species discovered in 100 years

**原文标题**: The first new cat species discovered in 100 years

**原文链接**: [https://www.nationalgeographic.com/animals/article/meet-the-first-new-cat-species-discovered-in-100-years](https://www.nationalgeographic.com/animals/article/meet-the-first-new-cat-species-discovered-in-100-years)

生成摘要时出错

---

## 55. Better Vector Search for Long Documents: Chunking Inside Manticore Search

**原文标题**: Better Vector Search for Long Documents: Chunking Inside Manticore Search

**原文链接**: [https://manticoresearch.com/blog/auto-chunking/](https://manticoresearch.com/blog/auto-chunking/)

生成摘要时出错

---

## 56. Our brain evolved from two primitive nervous systems that merged: Study

**原文标题**: Our brain evolved from two primitive nervous systems that merged: Study

**原文链接**: [https://www.newscientist.com/article/2589739-our-brain-evolved-from-two-primitive-nervous-systems-that-merged/](https://www.newscientist.com/article/2589739-our-brain-evolved-from-two-primitive-nervous-systems-that-merged/)

生成摘要时出错

---

## 57. Don't Just Say Hello

**原文标题**: Don't Just Say Hello

**原文链接**: [https://nohello.net/en/](https://nohello.net/en/)

生成摘要时出错

---

## 58. AI chatbots are becoming experts at changing people's minds

**原文标题**: AI chatbots are becoming experts at changing people's minds

**原文链接**: [https://www.science.org/content/article/ai-chatbots-are-becoming-experts-changing-people-s-minds-what-s-their-secret](https://www.science.org/content/article/ai-chatbots-are-becoming-experts-changing-people-s-minds-what-s-their-secret)

生成摘要时出错

---

## 59. Pentagon weighs pulling nearly a third of U.S. forces from Europe

**原文标题**: Pentagon weighs pulling nearly a third of U.S. forces from Europe

**原文链接**: [https://www.nbcnews.com/politics/national-security/pentagon-weighs-pulling-nearly-third-us-forces-europe-rcna597722](https://www.nbcnews.com/politics/national-security/pentagon-weighs-pulling-nearly-third-us-forces-europe-rcna597722)

生成摘要时出错

---

## 60. Claude Code now reads AGENTS.md if there is no Claude.md

**原文标题**: Claude Code now reads AGENTS.md if there is no Claude.md

**原文链接**: [https://code.claude.com/docs/en/changelog](https://code.claude.com/docs/en/changelog)

生成摘要时出错

---

## 61. T. Rex Had a Body Temperature of 97°F

**原文标题**: T. Rex Had a Body Temperature of 97°F

**原文链接**: [https://www.nytimes.com/2026/09/16/science/trex-dinosaur-temperature-warm-blooded.html](https://www.nytimes.com/2026/09/16/science/trex-dinosaur-temperature-warm-blooded.html)

生成摘要时出错

---

## 62. South Africa is at risk of becoming a mafia state

**原文标题**: South Africa is at risk of becoming a mafia state

**原文链接**: [https://www.economist.com/middle-east-and-africa/2026/09/14/south-africa-is-at-risk-of-becoming-a-mafia-state](https://www.economist.com/middle-east-and-africa/2026/09/14/south-africa-is-at-risk-of-becoming-a-mafia-state)

生成摘要时出错

---

## 63. Economic policy for AGI

**原文标题**: Economic policy for AGI

**原文链接**: [https://institute.deepmind.com/essays/economic-policy-for-agi/](https://institute.deepmind.com/essays/economic-policy-for-agi/)

生成摘要时出错

---

## 64. The Painful Truth: The RAM Crisis Is Only Just the Beginning

**原文标题**: The Painful Truth: The RAM Crisis Is Only Just the Beginning

**原文链接**: [https://www.madshrimps.be/news/the-painful-truth-the-ram-crisis-is-only-just-the-beginning/](https://www.madshrimps.be/news/the-painful-truth-the-ram-crisis-is-only-just-the-beginning/)

生成摘要时出错

---

## 65. Mathematicians Build Long-Awaited Graph Sandwich

**原文标题**: Mathematicians Build Long-Awaited Graph Sandwich

**原文链接**: [https://www.quantamagazine.org/mathematicians-build-long-awaited-graph-sandwich-20260918/](https://www.quantamagazine.org/mathematicians-build-long-awaited-graph-sandwich-20260918/)

生成摘要时出错

---

## 66. Warez: The Infrastructure and Aesthetics of Piracy (2021)

**原文标题**: Warez: The Infrastructure and Aesthetics of Piracy (2021)

**原文链接**: [https://archive.org/details/b904a8eb-9c98-4bb1-bf25-3cb9d075b157](https://archive.org/details/b904a8eb-9c98-4bb1-bf25-3cb9d075b157)

生成摘要时出错

---

## 67. Ask A Monk – A digital wilderness for thoughts with no immediate answer

**原文标题**: Ask A Monk – A digital wilderness for thoughts with no immediate answer

**原文链接**: [https://askamonk.online](https://askamonk.online)

生成摘要时出错

---

## 68. Part-human part-mouse brain developed in science breakthrough

**原文标题**: Part-human part-mouse brain developed in science breakthrough

**原文链接**: [https://www.bbc.com/news/articles/c60m3k28j81mo](https://www.bbc.com/news/articles/c60m3k28j81mo)

生成摘要时出错

---

## 69. Microsoft, OpenAI lose fight to hide internal docs admitting scraping is theft

**原文标题**: Microsoft, OpenAI lose fight to hide internal docs admitting scraping is theft

**原文链接**: [https://arstechnica.com/tech-policy/2026/09/microsoft-exec-called-ai-scraping-the-largest-theft-of-labor-in-human-history/](https://arstechnica.com/tech-policy/2026/09/microsoft-exec-called-ai-scraping-the-largest-theft-of-labor-in-human-history/)

生成摘要时出错

---

## 70. Goose Programming Language

**原文标题**: Goose Programming Language

**原文链接**: [https://github.com/aardappel/goose/tree/master](https://github.com/aardappel/goose/tree/master)

生成摘要时出错

---

## 71. AI Protest in Montreal

**原文标题**: AI Protest in Montreal

**原文链接**: [https://montrealgazette.com/news/photos-anti-ai-protest-in-montreal/](https://montrealgazette.com/news/photos-anti-ai-protest-in-montreal/)

生成摘要时出错

---

## 72. Google illegally retains customer data,and I am taking legal action against them

**原文标题**: Google illegally retains customer data,and I am taking legal action against them

**原文链接**: [https://medium.com/@istokovicsgyorgy79/google-illegally-retains-customer-data-and-i-am-taking-legal-action-against-them-7da0cf95941c](https://medium.com/@istokovicsgyorgy79/google-illegally-retains-customer-data-and-i-am-taking-legal-action-against-them-7da0cf95941c)

生成摘要时出错

---

## 73. U.S. Strike on Iranian School May Have Been War Crime, U.N. Report Says

**原文标题**: U.S. Strike on Iranian School May Have Been War Crime, U.N. Report Says

**原文链接**: [https://www.nytimes.com/2026/09/17/world/asia/us-iran-school-strike-report.html](https://www.nytimes.com/2026/09/17/world/asia/us-iran-school-strike-report.html)

生成摘要时出错

---

## 74. Missouri governor orders guardrails on Flock cameras and ALPRs

**原文标题**: Missouri governor orders guardrails on Flock cameras and ALPRs

**原文链接**: [https://www.stlpr.org/news-briefs/2026-09-16/flock-cameras-guardrails-missouri-kehoe](https://www.stlpr.org/news-briefs/2026-09-16/flock-cameras-guardrails-missouri-kehoe)

生成摘要时出错

---

## 75. Republican bill would order ISPs, DNS providers, and VPNs to block piracy sites

**原文标题**: Republican bill would order ISPs, DNS providers, and VPNs to block piracy sites

**原文链接**: [https://arstechnica.com/tech-policy/2026/09/republican-bill-would-order-isps-dns-providers-and-vpns-to-block-piracy-sites/](https://arstechnica.com/tech-policy/2026/09/republican-bill-would-order-isps-dns-providers-and-vpns-to-block-piracy-sites/)

生成摘要时出错

---

## 76. Flock cameras are riddled with security vulnerabilities and hardcoded creds

**原文标题**: Flock cameras are riddled with security vulnerabilities and hardcoded creds

**原文链接**: [https://micahflee.com/flock-cameras-are-riddled-with-security-vulnerabilities-and-hard-coded-credentials/](https://micahflee.com/flock-cameras-are-riddled-with-security-vulnerabilities-and-hard-coded-credentials/)

生成摘要时出错

---

## 77. NATS publishes preliminary report on technical incident of 8 September

**原文标题**: NATS publishes preliminary report on technical incident of 8 September

**原文链接**: [https://www.nats.aero/news/nats-publishes-preliminary-report-on-technical-incident-of-8-september/](https://www.nats.aero/news/nats-publishes-preliminary-report-on-technical-incident-of-8-september/)

生成摘要时出错

---

## 78. Introducing GNOME 51, "A Coruña"

**原文标题**: Introducing GNOME 51, "A Coruña"

**原文链接**: [https://release.gnome.org/51/](https://release.gnome.org/51/)

生成摘要时出错

---

## 79. New wild cat species discovered – with only one known living member

**原文标题**: New wild cat species discovered – with only one known living member

**原文链接**: [https://www.bbc.com/news/articles/c6x2zgv9rr4ro](https://www.bbc.com/news/articles/c6x2zgv9rr4ro)

生成摘要时出错

---

## 80. Why I didn’t sign the Fields medallists’ letter

**原文标题**: Why I didn’t sign the Fields medallists’ letter

**原文链接**: [https://terrytao.wordpress.com/2026/09/17/why-i-didnt-sign-the-fields-medallists-letter/](https://terrytao.wordpress.com/2026/09/17/why-i-didnt-sign-the-fields-medallists-letter/)

生成摘要时出错

---

## 81. Cache-to-Cache: Direct Semantic Communication Between LLMs (2025)

**原文标题**: Cache-to-Cache: Direct Semantic Communication Between LLMs (2025)

**原文链接**: [https://arxiv.org/abs/2510.03215](https://arxiv.org/abs/2510.03215)

生成摘要时出错

---

## 82. Canto: A speech model built for the real world

**原文标题**: Canto: A speech model built for the real world

**原文链接**: [https://wisprflow.ai/canto](https://wisprflow.ai/canto)

生成摘要时出错

---

## 83. OpenAI's Misalignment Framework: A Tactical Bid to Preempt Global AI Governance

**原文标题**: OpenAI's Misalignment Framework: A Tactical Bid to Preempt Global AI Governance

**原文链接**: [https://asiaai.fyi/openai-misalignment-framework-global-governance/](https://asiaai.fyi/openai-misalignment-framework-global-governance/)

生成摘要时出错

---

## 84. BYD looking to build 5-minute EV charging network in Canada

**原文标题**: BYD looking to build 5-minute EV charging network in Canada

**原文链接**: [https://driving.ca/auto-news/industry/byd-china-ev-megawatt-flash-charger-network-canada](https://driving.ca/auto-news/industry/byd-china-ev-megawatt-flash-charger-network-canada)

生成摘要时出错

---

## 85. Don't Make Job Referrals Public

**原文标题**: Don't Make Job Referrals Public

**原文链接**: [https://blog.melashri.net/micro/public-job-referral/](https://blog.melashri.net/micro/public-job-referral/)

生成摘要时出错

---

## 86. Anthropic finally adds AGENTS.md support to Claude Code

**原文标题**: Anthropic finally adds AGENTS.md support to Claude Code

**原文链接**: [https://twitter.com/trq212/status/2101009392611278961](https://twitter.com/trq212/status/2101009392611278961)

生成摘要时出错

---

