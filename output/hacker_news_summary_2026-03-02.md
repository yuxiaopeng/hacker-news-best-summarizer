# Hacker News 热门文章摘要 (2026-03-02)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 微GPT

**原文标题**: Microgpt

**原文链接**: [http://karpathy.github.io/2026/02/12/microgpt/](http://karpathy.github.io/2026/02/12/microgpt/)

Microgpt是一个开创性的艺术项目：一个仅200行、无依赖的Python文件，能够完整地训练和推理一个GPT模型。它封装了完整的算法内容，包括数据集、分词器、自动梯度引擎、类GPT-2神经网络架构、Adam优化器以及训练/推理循环。其创建者Andrej Karpathy将其描述为他十年来致力于将大型语言模型（LLMs）简化到最基本要素的执念的巅峰之作。

该项目可在GitHub、Karpathy的网站以及Google Colab笔记本上获取。

它使用包含32,000个名字的数据集来学习统计模式，并生成新的、听起来可信的名字。一个简单的字符级分词器将文本转换为整数ID，其中包括一个特殊的序列开始（BOS）词元，从而形成27个词元的词汇表。

关键是，Microgpt使用一个`Value`类实现了自己的自动梯度引擎，该类跟踪计算并通过链式法则计算梯度。这使得模型参数的迭代优化成为可能，它模仿了PyTorch的功能，但实现于基础的标量级别。

该模型的“知识”由4,192个随机初始化的参数组成，这些参数被组织成嵌入表、注意力层和多层感知器（MLP）的权重。其架构是简化的GPT-2，它利用辅助函数进行线性变换，使用softmax进行概率分布，并采用RMSNorm进行稳定训练，这些共同构成了其多头注意力块的基础。

---

## 2. 摩托罗拉宣布与 GrapheneOS 基金会建立合作关系

**原文标题**: Motorola announces a partnership with GrapheneOS Foundation

**原文链接**: [https://motorolanews.com/motorola-three-new-b2b-solutions-at-mwc-2026/](https://motorolanews.com/motorola-three-new-b2b-solutions-at-mwc-2026/)

联想旗下摩托罗拉公司于 2026 年 3 月 2 日在世界移动通信大会上宣布与 GrapheneOS 基金会建立具有里程碑意义的合作关系，开启了智能手机安全的新纪元。这项长期合作旨在将 GrapheneOS 经过强化的、注重隐私的操作系统整合到未来的摩托罗拉设备中，为全球用户带来尖端安全。GrapheneOS 的一位发言人表达了热情，强调此次合作是推动移动安全发展和扩大 GrapheneOS 影响力的重要一步。该联盟将结合 GrapheneOS 的开创性工程技术、摩托罗拉的安全专长以及联想的 ThinkShield 解决方案，重点关注联合研究、软件增强和新的安全功能。

与此同时，摩托罗拉通过推出两项关键产品，扩展了其企业产品组合：
1.  **Moto Analytics**：一个企业级平台，为 IT 管理员提供对其设备群组的实时性能可见性，提供深入的运营洞察，以实现高效故障排除和提高生产力。
2.  **私密图像数据**：Moto Secure 平台内的一项新功能，可自动从新的相机图像中删除敏感元数据（例如位置信息），从而增强用户隐私。

这些发布强调了摩托罗拉致力于为消费者和企业提供智能、高性能且安全性增强的技术，并通过专为严苛企业环境打造的解决方案，扩展其 B2B 生态系统。

---

## 3. 微软在其Discord上禁用“Microslop”一词，随后锁定该服务器。

**原文标题**: Microsoft bans the word "Microslop" on its Discord, then locks the server

**原文链接**: [https://www.windowslatest.com/2026/03/02/microsoft-gets-tired-of-microslop-bans-the-word-on-its-discord-then-locks-the-server-after-backlash/](https://www.windowslatest.com/2026/03/02/microsoft-gets-tired-of-microslop-bans-the-word-on-its-discord-then-locks-the-server-after-backlash/)

微软最近封锁了其官方Copilot Discord服务器，原因在于用户普遍使用并规避了对贬义词“Microslop”的禁令。这一绰号的流行是对微软将人工智能强行整合到Windows 11中的一种批评，许多用户认为这种整合的优先级高于操作系统的稳定性。

Windows Latest最初报道称，包含“Microslop”一词的消息会自动被过滤并标记为不当内容。然而，用户很快找到了变通方法，使用“Microsl0p”等变体来规避审查。这种“猫捉老鼠”的游戏不断升级，导致一些账号被封禁，随后微软限制了服务器访问，隐藏了消息历史记录，并禁用了许多用户的发帖权限。

此次事件被认为进一步损害了微软的品牌形象，尤其是在其AI领导地位面临日益激烈的竞争之际。尽管Copilot Discord服务器于2024年12月上线时获得了用户的积极参与，但当前的情绪反映出对微软AI战略的普遍不满。尽管存在争议，文章承认Copilot确实提供了一些真正有用的功能，例如用于Google通讯录等服务的数据连接器。此次事件引发了关于微软AI推广未来及其与用户社区关系的问题。

---

## 4. Ghostty - 终端模拟器

**原文标题**: Ghostty – Terminal Emulator

**原文链接**: [https://ghostty.org/docs](https://ghostty.org/docs)

Ghostty是一款快速、功能丰富且跨平台的终端模拟器，它利用平台原生的UI和GPU加速来实现最佳性能。它旨在易于使用，无需任何配置即可上手。

安装简单，macOS提供即用型二进制文件，Linux则有软件包或从源代码构建的选项。Ghostty提供广泛的自定义选项，包括灵活的自定义按键绑定以及数百种支持亮色和暗色模式的内置颜色主题。用户可以通过众多配置选项来定制其外观和行为。此外，它还提供一份终端API (VT) 参考，可作为终端应用程序开发者的宝贵资源。

---

## 5. We do not think Anthropic should be designated as a supply chain risk

**原文标题**: We do not think Anthropic should be designated as a supply chain risk

**原文链接**: [https://twitter.com/OpenAI/status/2027846016423321831](https://twitter.com/OpenAI/status/2027846016423321831)

The provided text does not contain an article arguing against designating Anthropic as a supply chain risk. Instead, it is an error message from x.com (formerly Twitter) stating that JavaScript is disabled in the user's browser. The message instructs the user to enable JavaScript or switch to a supported browser to continue accessing the site. Therefore, no content is available to summarize regarding Anthropic or supply chain risks.

---

## 6. /e/OS 是一个完整的、彻底“去谷歌化”的移动生态系统

**原文标题**: /e/OS is a complete, fully “deGoogled” mobile ecosystem

**原文链接**: [https://e.foundation/e-os/](https://e.foundation/e-os/)

/e/OS 是一个完整、开源、"去谷歌化"且专注于隐私的移动生态系统。它是一个基于安卓的操作系统，用 Murena Find 和 microG 等尊重隐私的替代方案取代了谷歌的搜索、连接性检查和地理定位等服务。该操作系统可审计，确保其隐私声明的透明性。

除了核心操作系统之外，/e/OS 还提供了一套精心策划的开源应用程序，以及一个"App Lounge"，该中心提供隐私评级，详细列出每个应用的跟踪器和权限。主要功能包括用于隐藏 IP 地址和地理位置的"高级隐私"小部件，以及内置广告拦截器。

Murena Workspace 账户是核心，提供免费的 @murena.io 电子邮件、1GB 云存储、在线办公文档工具以及用于端到端加密存储的 Murena Vault，可作为主流服务的隐私友好替代方案。家长控制功能已集成，提供内容过滤、屏幕时间限制和"查找我的设备"功能。账户管理器允许同步来自不同提供商的数据，将其本地存储并尊重用户隐私。

用户可以通过购买预装了 /e/OS 的 Murena 智能手机、使用基于网络的 /e/OS 安装器，或者对于有经验的用户手动下载来获取 /e/OS。支持可通过完善的用户文档、社区论坛、专门的 Telegram 聊天以及 GitLab 上的开发者资源获得。还为企业提供专业服务。

---

## 7. 切换到 Claude 无需从头开始

**原文标题**: Switch to Claude without starting over

**原文链接**: [https://claude.com/import-memory](https://claude.com/import-memory)

本文概述了用户如何从其他AI提供商无缝切换到Claude，而不丢失他们积累的偏好和上下文。该过程被称为“一键复制粘贴”法，它让Claude能够更新其记忆，并接续对话，仿佛对话一直在进行。

为了导入上下文，用户只需将一个提供的提示复制到他们现有AI提供商的聊天中。该AI的输出结果随后被粘贴到Claude的记忆设置中，这个快速过程耗时不到一分钟。这确保了用户的“第一次对话感觉就像他们的第一百次对话一样”。

Claude的记忆系统旨在理解跨对话的用户偏好，保持项目上下文的独立性，并允许用户查看和编辑其记忆内容。这项“记忆”功能在所有付费计划中均可用。该服务旨在让Claude“从第一天起就了解你”，鼓励用户启动专业版（Pro）计划以体验这种顺畅的过渡。

---

## 8. 我做了一个演示，展示AI聊天在“免费”且由广告支持时会是什么样子。

**原文标题**: I built a demo of what AI chat will look like when it's “free” and ad-supported

**原文链接**: [https://99helpers.com/tools/ad-supported-chat](https://99helpers.com/tools/ad-supported-chat)

This article introduces "AdBot AI," a satirical yet functional demo illustrating what ad-supported AI chat could look like in a future where AI becomes "free." Built as an educational tool, it aims to show how companies might monetize AI services to cover significant compute costs, akin to free websites or streaming platforms. The demo presents various monetization patterns, prompting discussions on the future of AI.

It showcases a full spectrum of ad types: pre-chat interstitial videos, classic banner and sidebar ads, sponsored responses subtly weaving product recommendations into AI answers, contextual text ads matched to conversation topics, and rich media intent-based product cards. Additionally, it features freemium gating (requiring an ad view or upgrade after 5 messages), retargeting and geo-targeted ads, and sponsored quick-reply suggestions.

The article contrasts ad-supported and subscription AI models: Ad-supported offers a free (but ad-filled) experience with potential privacy trade-offs and ad-optimized responses. Subscriptions offer an ad-free, private, and user-value-optimized experience for a monthly fee.

This demo is valuable for a wide audience, including product managers, marketers, developers, UX designers, founders, investors, and journalists, to understand AI monetization, ethics, and potential user experiences. The demo's ads are fictional, though the AI responses are real. The article concludes by promoting 99helpers' ad-free chatbot builder as an alternative.

---

## 9. Decision trees – the unreasonable power of nested decision rules

**原文标题**: Decision trees – the unreasonable power of nested decision rules

**原文链接**: [https://mlu-explain.github.io/decision-tree/](https://mlu-explain.github.io/decision-tree/)

生成摘要时出错

---

## 10. Iran's Ayatollah Ali Khamenei is killed in Israeli strike, ending 36-year rule

**原文标题**: Iran's Ayatollah Ali Khamenei is killed in Israeli strike, ending 36-year rule

**原文链接**: [https://www.npr.org/2026/02/28/1123499337/iran-israel-ayatollah-ali-khamenei-killed](https://www.npr.org/2026/02/28/1123499337/iran-israel-ayatollah-ali-khamenei-killed)

生成摘要时出错

---

## 11. Qwen3.5 122B and 35B models offer Sonnet 4.5 performance on local computers

**原文标题**: Qwen3.5 122B and 35B models offer Sonnet 4.5 performance on local computers

**原文链接**: [https://venturebeat.com/technology/alibabas-new-open-source-qwen3-5-medium-models-offer-sonnet-4-5-performance](https://venturebeat.com/technology/alibabas-new-open-source-qwen3-5-medium-models-offer-sonnet-4-5-performance)

生成摘要时出错

---

## 12. If AI writes code, should the session be part of the commit?

**原文标题**: If AI writes code, should the session be part of the commit?

**原文链接**: [https://github.com/mandel-macaque/memento](https://github.com/mandel-macaque/memento)

生成摘要时出错

---

## 13. How to talk to anyone and why you should

**原文标题**: How to talk to anyone and why you should

**原文链接**: [https://www.theguardian.com/lifeandstyle/2026/feb/24/stranger-secret-how-to-talk-to-anyone-why-you-should](https://www.theguardian.com/lifeandstyle/2026/feb/24/stranger-secret-how-to-talk-to-anyone-why-you-should)

生成摘要时出错

---

## 14. Everett shuts down Flock camera network after judge rules footage public record

**原文标题**: Everett shuts down Flock camera network after judge rules footage public record

**原文链接**: [https://www.wltx.com/article/news/nation-world/281-53d8693e-77a4-42ad-86e4-3426a30d25ae](https://www.wltx.com/article/news/nation-world/281-53d8693e-77a4-42ad-86e4-3426a30d25ae)

生成摘要时出错

---

## 15. When does MCP make sense vs CLI?

**原文标题**: When does MCP make sense vs CLI?

**原文链接**: [https://ejholmes.github.io/2026/02/28/mcp-is-dead-long-live-the-cli.html](https://ejholmes.github.io/2026/02/28/mcp-is-dead-long-live-the-cli.html)

生成摘要时出错

---

## 16. Jolla phone – a full-stack European alternative

**原文标题**: Jolla phone – a full-stack European alternative

**原文链接**: [https://commerce.jolla.com/products/jolla-phone-sept-26](https://commerce.jolla.com/products/jolla-phone-sept-26)

生成摘要时出错

---

## 17. AI让写代码更简单，却让工程师更难当。

**原文标题**: AI Made Writing Code Easier. It Made Being an Engineer Harder

**原文链接**: [https://www.ivanturkovic.com/2026/02/25/ai-made-writing-code-easier-engineering-harder/](https://www.ivanturkovic.com/2026/02/25/ai-made-writing-code-easier-engineering-harder/)

生成摘要时出错

---

## 18. 我们与战争部的协议

**原文标题**: Our Agreement with the Department of War

**原文链接**: [https://openai.com/index/our-agreement-with-the-department-of-war](https://openai.com/index/our-agreement-with-the-department-of-war)

生成摘要时出错

---

## 19. The Windows 95 user interface: A case study in usability engineering (1996)

**原文标题**: The Windows 95 user interface: A case study in usability engineering (1996)

**原文链接**: [https://dl.acm.org/doi/fullHtml/10.1145/238386.238611](https://dl.acm.org/doi/fullHtml/10.1145/238386.238611)

生成摘要时出错

---

## 20. WebMCP is available for early preview

**原文标题**: WebMCP is available for early preview

**原文链接**: [https://developer.chrome.com/blog/webmcp-epp](https://developer.chrome.com/blog/webmcp-epp)

生成摘要时出错

---

## 21. Anthropic Cowork feature creates 10GB VM bundle on macOS without warning

**原文标题**: Anthropic Cowork feature creates 10GB VM bundle on macOS without warning

**原文链接**: [https://github.com/anthropics/claude-code/issues/22543](https://github.com/anthropics/claude-code/issues/22543)

生成摘要时出错

---

## 22. U.S. science agency moves to restrict foreign scientists from its labs

**原文标题**: U.S. science agency moves to restrict foreign scientists from its labs

**原文链接**: [https://www.science.org/content/article/nist-moves-restrict-foreign-scientists-its-labs](https://www.science.org/content/article/nist-moves-restrict-foreign-scientists-its-labs)

生成摘要时出错

---

## 23. Block the “Upgrade to Tahoe” alerts

**原文标题**: Block the “Upgrade to Tahoe” alerts

**原文链接**: [https://robservatory.com/block-the-upgrade-to-tahoe-alerts-and-system-settings-indicator/](https://robservatory.com/block-the-upgrade-to-tahoe-alerts-and-system-settings-indicator/)

生成摘要时出错

---

## 24. New iron nanomaterial wipes out cancer cells without harming healthy tissue

**原文标题**: New iron nanomaterial wipes out cancer cells without harming healthy tissue

**原文链接**: [https://www.sciencedaily.com/releases/2026/02/260228093456.htm](https://www.sciencedaily.com/releases/2026/02/260228093456.htm)

生成摘要时出错

---

## 25. Techno‑feudal elite are attempting to build a twenty‑first‑century fascist state

**原文标题**: Techno‑feudal elite are attempting to build a twenty‑first‑century fascist state

**原文链接**: [https://collapseofindustrialcivilization.com/2026/02/16/americas-oligarchic-techno-feudal-elite-are-attempting-to-build-a-twenty-first-century-fascist-state/](https://collapseofindustrialcivilization.com/2026/02/16/americas-oligarchic-techno-feudal-elite-are-attempting-to-build-a-twenty-first-century-fascist-state/)

生成摘要时出错

---

## 26. Microgpt explained interactively

**原文标题**: Microgpt explained interactively

**原文链接**: [https://growingswe.com/blog/microgpt](https://growingswe.com/blog/microgpt)

生成摘要时出错

---

## 27. Claude becomes number one app on the U.S. App Store

**原文标题**: Claude becomes number one app on the U.S. App Store

**原文链接**: [https://apps.apple.com/us/iphone/charts](https://apps.apple.com/us/iphone/charts)

生成摘要时出错

---

## 28. 10-202: Introduction to Modern AI (CMU)

**原文标题**: 10-202: Introduction to Modern AI (CMU)

**原文链接**: [https://modernaicourse.org](https://modernaicourse.org)

生成摘要时出错

---

## 29. Right-sizes LLM models to your system's RAM, CPU, and GPU

**原文标题**: Right-sizes LLM models to your system's RAM, CPU, and GPU

**原文链接**: [https://github.com/AlexsJones/llmfit](https://github.com/AlexsJones/llmfit)

生成摘要时出错

---

## 30. Flightradar24 for Ships

**原文标题**: Flightradar24 for Ships

**原文链接**: [https://atlas.flexport.com/](https://atlas.flexport.com/)

生成摘要时出错

---

## 31. Operational issue – Multiple services (UAE)

**原文标题**: Operational issue – Multiple services (UAE)

**原文链接**: [https://health.aws.amazon.com/health/status](https://health.aws.amazon.com/health/status)

生成摘要时出错

---

## 32. Why XML tags are so fundamental to Claude

**原文标题**: Why XML tags are so fundamental to Claude

**原文链接**: [https://glthr.com/XML-fundamental-to-Claude](https://glthr.com/XML-fundamental-to-Claude)

生成摘要时出错

---

## 33. MinIO Is Dead, Long Live MinIO

**原文标题**: MinIO Is Dead, Long Live MinIO

**原文链接**: [https://blog.vonng.com/en/db/minio-resurrect/](https://blog.vonng.com/en/db/minio-resurrect/)

生成摘要时出错

---

## 34. OpenClaw surpasses React to become the most-starred software project on GitHub

**原文标题**: OpenClaw surpasses React to become the most-starred software project on GitHub

**原文链接**: [https://www.star-history.com/blog/openclaw-surpasses-react-most-starred-software](https://www.star-history.com/blog/openclaw-surpasses-react-most-starred-software)

生成摘要时出错

---

## 35. AI is making junior devs useless

**原文标题**: AI is making junior devs useless

**原文链接**: [https://beabetterdev.com/2026/03/01/ai-is-making-junior-devs-useless/](https://beabetterdev.com/2026/03/01/ai-is-making-junior-devs-useless/)

生成摘要时出错

---

## 36. Microslop Manifesto

**原文标题**: Microslop Manifesto

**原文链接**: [http://microslop.com/](http://microslop.com/)

生成摘要时出错

---

## 37. New iPad Air, powered by M4

**原文标题**: New iPad Air, powered by M4

**原文链接**: [https://www.apple.com/newsroom/2026/03/apple-introduces-the-new-ipad-air-powered-by-m4/](https://www.apple.com/newsroom/2026/03/apple-introduces-the-new-ipad-air-powered-by-m4/)

生成摘要时出错

---

## 38. Ape Coding [fiction]

**原文标题**: Ape Coding [fiction]

**原文链接**: [https://rsaksida.com/blog/ape-coding/](https://rsaksida.com/blog/ape-coding/)

生成摘要时出错

---

## 39. Show HN: Timber – Ollama for classical ML models, 336x faster than Python

**原文标题**: Show HN: Timber – Ollama for classical ML models, 336x faster than Python

**原文链接**: [https://github.com/kossisoroyce/timber](https://github.com/kossisoroyce/timber)

生成摘要时出错

---

## 40. Samsung Galaxy update removes Android recovery menu tools, including sideloading

**原文标题**: Samsung Galaxy update removes Android recovery menu tools, including sideloading

**原文链接**: [https://9to5google.com/2026/02/27/samsung-galaxy-update-android-recovery-menu-removed/](https://9to5google.com/2026/02/27/samsung-galaxy-update-android-recovery-menu-removed/)

生成摘要时出错

---

## 41. Inside the M4 Apple Neural Engine, Part 1: Reverse Engineering

**原文标题**: Inside the M4 Apple Neural Engine, Part 1: Reverse Engineering

**原文链接**: [https://maderix.substack.com/p/inside-the-m4-apple-neural-engine](https://maderix.substack.com/p/inside-the-m4-apple-neural-engine)

生成摘要时出错

---

## 42. You don't have to

**原文标题**: You don't have to

**原文链接**: [https://www.scottsmitelli.com/articles/you-dont-have-to/](https://www.scottsmitelli.com/articles/you-dont-have-to/)

生成摘要时出错

---

## 43. "Cancel ChatGPT" movement goes mainstream after OpenAI closes deal with U.S. Dow

**原文标题**: "Cancel ChatGPT" movement goes mainstream after OpenAI closes deal with U.S. Dow

**原文链接**: [https://www.windowscentral.com/artificial-intelligence/cancel-chatgpt-movement-goes-mainstream-after-openai-closes-deal-with-u-s-department-of-war-as-anthropic-refuses-to-surveil-american-citizens](https://www.windowscentral.com/artificial-intelligence/cancel-chatgpt-movement-goes-mainstream-after-openai-closes-deal-with-u-s-department-of-war-as-anthropic-refuses-to-surveil-american-citizens)

生成摘要时出错

---

## 44. Little Free Library

**原文标题**: Little Free Library

**原文链接**: [https://littlefreelibrary.org/](https://littlefreelibrary.org/)

生成摘要时出错

---

## 45. First-ever in-utero stem cell therapy for fetal spina bifida repair is safe

**原文标题**: First-ever in-utero stem cell therapy for fetal spina bifida repair is safe

**原文链接**: [https://health.ucdavis.edu/news/headlines/first-ever-in-utero-stem-cell-therapy-for-fetal-spina-bifida-repair-is-safe-study-finds/2026/02](https://health.ucdavis.edu/news/headlines/first-ever-in-utero-stem-cell-therapy-for-fetal-spina-bifida-repair-is-safe-study-finds/2026/02)

生成摘要时出错

---

## 46. Judge finalizes order for Greenpeace to pay $345M in ND oil pipeline case

**原文标题**: Judge finalizes order for Greenpeace to pay $345M in ND oil pipeline case

**原文链接**: [https://northdakotamonitor.com/2026/02/27/judge-finalizes-order-for-greenpeace-to-pay-345-million-in-north-dakota-oil-pipeline-case/](https://northdakotamonitor.com/2026/02/27/judge-finalizes-order-for-greenpeace-to-pay-345-million-in-north-dakota-oil-pipeline-case/)

生成摘要时出错

---

## 47. Why does C have the best file API

**原文标题**: Why does C have the best file API

**原文链接**: [https://maurycyz.com/misc/c_files/](https://maurycyz.com/misc/c_files/)

生成摘要时出错

---

## 48. A new Polymarket account made over $500k betting on the U.S. strike against Iran

**原文标题**: A new Polymarket account made over $500k betting on the U.S. strike against Iran

**原文链接**: [https://twitter.com/cabsav456/status/2027937130995921119](https://twitter.com/cabsav456/status/2027937130995921119)

生成摘要时出错

---

## 49. Pentagon chief blocks officers from Ivy League schools and top universities

**原文标题**: Pentagon chief blocks officers from Ivy League schools and top universities

**原文链接**: [https://fortune.com/2026/02/28/pentagon-officer-education-ivy-league-schools-universities-partners-ai-space/](https://fortune.com/2026/02/28/pentagon-officer-education-ivy-league-schools-universities-partners-ai-space/)

生成摘要时出错

---

## 50. Computer-generated dream world: Virtual reality for a 286 processor

**原文标题**: Computer-generated dream world: Virtual reality for a 286 processor

**原文链接**: [https://deadlime.hu/en/2026/02/22/computer-generated-dream-world/](https://deadlime.hu/en/2026/02/22/computer-generated-dream-world/)

生成摘要时出错

---

## 51. How to record and retrieve anything you've ever had to look up twice

**原文标题**: How to record and retrieve anything you've ever had to look up twice

**原文链接**: [https://ellanew.com/2026/03/02/ptpl-197-record-retrieve-from-a-personal-knowledgebase](https://ellanew.com/2026/03/02/ptpl-197-record-retrieve-from-a-personal-knowledgebase)

生成摘要时出错

---

## 52. Show HN: Omni – Open-source workplace search and chat, built on Postgres

**原文标题**: Show HN: Omni – Open-source workplace search and chat, built on Postgres

**原文链接**: [https://github.com/getomnico/omni](https://github.com/getomnico/omni)

生成摘要时出错

---

## 53. Claude dethrones ChatGPT as top U.S. app after Pentagon saga

**原文标题**: Claude dethrones ChatGPT as top U.S. app after Pentagon saga

**原文链接**: [https://www.axios.com/2026/03/01/anthropic-claude-chatgpt-app-downloads-pentagon](https://www.axios.com/2026/03/01/anthropic-claude-chatgpt-app-downloads-pentagon)

生成摘要时出错

---

## 54. Why is the first C++ (m)allocation always 72 KB?

**原文标题**: Why is the first C++ (m)allocation always 72 KB?

**原文链接**: [https://joelsiks.com/posts/cpp-emergency-pool-72kb-allocation/](https://joelsiks.com/posts/cpp-emergency-pool-72kb-allocation/)

生成摘要时出错

---

## 55. Waymo blocking ambulance during deadly Austin shooting

**原文标题**: Waymo blocking ambulance during deadly Austin shooting

**原文链接**: [https://www.mysanantonio.com/news/austin/article/waymo-austin-shooting-21948947.php](https://www.mysanantonio.com/news/austin/article/waymo-austin-shooting-21948947.php)

生成摘要时出错

---

## 56. An interactive intro to Elliptic Curve Cryptography

**原文标题**: An interactive intro to Elliptic Curve Cryptography

**原文链接**: [https://growingswe.com/blog/elliptic-curve-cryptography](https://growingswe.com/blog/elliptic-curve-cryptography)

生成摘要时出错

---

## 57. How the Government Deceived Congress in the Debate over Surveillance Powers (2013)

**原文标题**: How the Government Deceived Congress in the Debate over Surveillance Powers (2013)

**原文链接**: [https://www.eff.org/deeplinks/2013/06/director-national-intelligences-word-games-explained-how-government-deceived](https://www.eff.org/deeplinks/2013/06/director-national-intelligences-word-games-explained-how-government-deceived)

生成摘要时出错

---

## 58. Claude hits #1 on the App Store as users rally behind Anthropic

**原文标题**: Claude hits #1 on the App Store as users rally behind Anthropic

**原文链接**: [https://9to5mac.com/2026/03/01/claude-hits-1-on-the-app-store-as-users-rally-behind-anthropics-government-standoff/](https://9to5mac.com/2026/03/01/claude-hits-1-on-the-app-store-as-users-rally-behind-anthropics-government-standoff/)

生成摘要时出错

---

## 59. Just two days of oatmeal cut bad cholesterol by 10%

**原文标题**: Just two days of oatmeal cut bad cholesterol by 10%

**原文链接**: [https://www.sciencedaily.com/releases/2026/02/260225081217.htm](https://www.sciencedaily.com/releases/2026/02/260225081217.htm)

生成摘要时出错

---

## 60. Allegations of insider trading over prediction-market bets tied to Iran conflict

**原文标题**: Allegations of insider trading over prediction-market bets tied to Iran conflict

**原文链接**: [https://www.morningstar.com/news/marketwatch/20260301140/allegations-of-insider-trading-over-prediction-market-bets-tied-to-iran-conflict](https://www.morningstar.com/news/marketwatch/20260301140/allegations-of-insider-trading-over-prediction-market-bets-tied-to-iran-conflict)

生成摘要时出错

---

## 61. Felix "fx" Lindner has died

**原文标题**: Felix "fx" Lindner has died

**原文链接**: [https://blog.recurity-labs.com/2026-03-02/Farewell_Felix](https://blog.recurity-labs.com/2026-03-02/Farewell_Felix)

生成摘要时出错

---

## 62. This system can go fuck itself and burn in hell

**原文标题**: This system can go fuck itself and burn in hell

**原文链接**: [https://shawnfromportland.substack.com/p/this-system-can-go-fuck-itself-and](https://shawnfromportland.substack.com/p/this-system-can-go-fuck-itself-and)

生成摘要时出错

---

## 63. Are the Mysteries of Quantum Mechanics Beginning to Dissolve?

**原文标题**: Are the Mysteries of Quantum Mechanics Beginning to Dissolve?

**原文链接**: [https://www.quantamagazine.org/are-the-mysteries-of-quantum-mechanics-beginning-to-dissolve-20260213/](https://www.quantamagazine.org/are-the-mysteries-of-quantum-mechanics-beginning-to-dissolve-20260213/)

生成摘要时出错

---

## 64. Process-Based Concurrency: Why Beam and OTP Keep Being Right

**原文标题**: Process-Based Concurrency: Why Beam and OTP Keep Being Right

**原文链接**: [https://variantsystems.io/blog/beam-otp-process-concurrency](https://variantsystems.io/blog/beam-otp-process-concurrency)

生成摘要时出错

---

## 65. Khamenei Dead

**原文标题**: Khamenei Dead

**原文链接**: [https://twitter.com/BarakRavid/status/2027830773328302396](https://twitter.com/BarakRavid/status/2027830773328302396)

生成摘要时出错

---

## 66. AMD Am386 released March 2, 1991

**原文标题**: AMD Am386 released March 2, 1991

**原文链接**: [https://dfarq.homeip.net/amd-am386-released-march-2-1991/](https://dfarq.homeip.net/amd-am386-released-march-2-1991/)

生成摘要时出错

---

## 67. A plastic made from milk that vanishes in 13 weeks

**原文标题**: A plastic made from milk that vanishes in 13 weeks

**原文链接**: [https://www.sciencedaily.com/releases/2026/02/260227071922.htm](https://www.sciencedaily.com/releases/2026/02/260227071922.htm)

生成摘要时出错

---

## 68. South Korean Police Lose Seized Crypto by Posting Password Online

**原文标题**: South Korean Police Lose Seized Crypto by Posting Password Online

**原文链接**: [https://gizmodo.com/south-korean-police-lose-seized-crypto-by-posting-password-online-2000728191](https://gizmodo.com/south-korean-police-lose-seized-crypto-by-posting-password-online-2000728191)

生成摘要时出错

---

## 69. Claude Code LSP

**原文标题**: Claude Code LSP

**原文链接**: [https://karanbansal.in/blog/claude-code-lsp/](https://karanbansal.in/blog/claude-code-lsp/)

生成摘要时出错

---

## 70. Running a One Trillion-Parameter LLM Locally on AMD Ryzen AI Max+ Cluster

**原文标题**: Running a One Trillion-Parameter LLM Locally on AMD Ryzen AI Max+ Cluster

**原文链接**: [https://www.amd.com/en/developer/resources/technical-articles/2026/how-to-run-a-one-trillion-parameter-llm-locally-an-amd.html](https://www.amd.com/en/developer/resources/technical-articles/2026/how-to-run-a-one-trillion-parameter-llm-locally-an-amd.html)

生成摘要时出错

---

## 71. iPhone 17e

**原文标题**: iPhone 17e

**原文链接**: [https://www.apple.com/newsroom/2026/03/apple-introduces-iphone-17e/](https://www.apple.com/newsroom/2026/03/apple-introduces-iphone-17e/)

生成摘要时出错

---

## 72. Building a Minimal Transformer for 10-digit Addition

**原文标题**: Building a Minimal Transformer for 10-digit Addition

**原文链接**: [https://alexlitzenberger.com/blog/post.html?post=/building_a_minimal_transformer_for_10_digit_addition](https://alexlitzenberger.com/blog/post.html?post=/building_a_minimal_transformer_for_10_digit_addition)

生成摘要时出错

---

## 73. Parallel coding agents with tmux and Markdown specs

**原文标题**: Parallel coding agents with tmux and Markdown specs

**原文链接**: [https://schipper.ai/posts/parallel-coding-agents/](https://schipper.ai/posts/parallel-coding-agents/)

生成摘要时出错

---

## 74. Show HN: I built a zero-browser, pure-JS typesetting engine for bit-perfect PDFs

**原文标题**: Show HN: I built a zero-browser, pure-JS typesetting engine for bit-perfect PDFs

**原文链接**: [https://github.com/cosmiciron/vmprint](https://github.com/cosmiciron/vmprint)

生成摘要时出错

---

## 75. Apple AI servers unused in warehouses due to low Apple Intelligence usage

**原文标题**: Apple AI servers unused in warehouses due to low Apple Intelligence usage

**原文链接**: [https://9to5mac.com/2026/03/02/some-apple-ai-servers-are-reportedly-sitting-unused-on-warehouse-shelves-due-to-low-apple-intelligence-usage/](https://9to5mac.com/2026/03/02/some-apple-ai-servers-are-reportedly-sitting-unused-on-warehouse-shelves-due-to-low-apple-intelligence-usage/)

生成摘要时出错

---

## 76. An Interesting Find: STM32 RDP1 Decryptor

**原文标题**: An Interesting Find: STM32 RDP1 Decryptor

**原文链接**: [https://carlossless.io/stm32-rdp1-decryptor/](https://carlossless.io/stm32-rdp1-decryptor/)

生成摘要时出错

---

## 77. Show HN: Govbase – Follow a bill from source text to news bias to social posts

**原文标题**: Show HN: Govbase – Follow a bill from source text to news bias to social posts

**原文链接**: [https://govbase.com](https://govbase.com)

生成摘要时出错

---

## 78. U.S. Races to Accomplish Iran Mission Before Munitions Run Out

**原文标题**: U.S. Races to Accomplish Iran Mission Before Munitions Run Out

**原文链接**: [https://www.wsj.com/world/middle-east/u-s-races-to-accomplish-iran-mission-before-munitions-run-out-c014acbc](https://www.wsj.com/world/middle-east/u-s-races-to-accomplish-iran-mission-before-munitions-run-out-c014acbc)

生成摘要时出错

---

## 79. Show HN: Xmloxide – an agent-made Rust replacement for libxml2

**原文标题**: Show HN: Xmloxide – an agent-made Rust replacement for libxml2

**原文链接**: [https://github.com/jonwiggins/xmloxide](https://github.com/jonwiggins/xmloxide)

生成摘要时出错

---

## 80. Evil in the West Bank

**原文标题**: Evil in the West Bank

**原文链接**: [https://www.nybooks.com/articles/2026/03/12/evil-in-the-west-bank-david-shulman/](https://www.nybooks.com/articles/2026/03/12/evil-in-the-west-bank-david-shulman/)

生成摘要时出错

---

## 81. January in Servo: preloads, better forms, details styling, and more

**原文标题**: January in Servo: preloads, better forms, details styling, and more

**原文链接**: [https://servo.org/blog/2026/02/28/january-in-servo/](https://servo.org/blog/2026/02/28/january-in-servo/)

生成摘要时出错

---

## 82. 4,500 Physicians Agree (About Bacon)

**原文标题**: 4,500 Physicians Agree (About Bacon)

**原文链接**: [https://machielreyneke.com/blog/persuasion/](https://machielreyneke.com/blog/persuasion/)

生成摘要时出错

---

## 83. Show HN: Audio Toolkit for Agents

**原文标题**: Show HN: Audio Toolkit for Agents

**原文链接**: [https://github.com/shiehn/sas-audio-processor](https://github.com/shiehn/sas-audio-processor)

生成摘要时出错

---

## 84. US Military says 3 service members have been killed

**原文标题**: US Military says 3 service members have been killed

**原文链接**: [https://apnews.com/live/us-israel-strikes-iran-khamenei-03-01-2026](https://apnews.com/live/us-israel-strikes-iran-khamenei-03-01-2026)

生成摘要时出错

---

## 85. A case for Go as the best language for AI agents

**原文标题**: A case for Go as the best language for AI agents

**原文链接**: [https://getbruin.com/blog/go-is-the-best-language-for-agents/](https://getbruin.com/blog/go-is-the-best-language-for-agents/)

生成摘要时出错

---

## 86. Bars close and hundreds lose jobs as US firm buys Brewdog in £33M deal

**原文标题**: Bars close and hundreds lose jobs as US firm buys Brewdog in £33M deal

**原文链接**: [https://www.bbc.com/news/articles/c05v0p1d0peo](https://www.bbc.com/news/articles/c05v0p1d0peo)

生成摘要时出错

---

## 87. Why Go Can't Try

**原文标题**: Why Go Can't Try

**原文链接**: [https://niketpatel.com/essays/why-go-cant-try](https://niketpatel.com/essays/why-go-cant-try)

生成摘要时出错

---

## 88. Big Breakfast Alters Appetite, Gut Health

**原文标题**: Big Breakfast Alters Appetite, Gut Health

**原文链接**: [https://www.cambridge.org/core/journals/british-journal-of-nutrition/article/big-breakfast-diet-composition-impacts-on-appetite-control-and-gut-health-a-randomized-weight-loss-trial-in-adults-with-overweight-or-obesity/69D4E150EAE7D9632D33904D7A4AE5FA](https://www.cambridge.org/core/journals/british-journal-of-nutrition/article/big-breakfast-diet-composition-impacts-on-appetite-control-and-gut-health-a-randomized-weight-loss-trial-in-adults-with-overweight-or-obesity/69D4E150EAE7D9632D33904D7A4AE5FA)

生成摘要时出错

---

## 89. The Science of Detecting LLM-Generated Text (2024)

**原文标题**: The Science of Detecting LLM-Generated Text (2024)

**原文链接**: [https://dl.acm.org/doi/10.1145/3624725](https://dl.acm.org/doi/10.1145/3624725)

生成摘要时出错

---

## 90. Packaging a Gleam app into a single executable

**原文标题**: Packaging a Gleam app into a single executable

**原文链接**: [https://www.dhzdhd.dev/blog/gleam-executable](https://www.dhzdhd.dev/blog/gleam-executable)

生成摘要时出错

---

## 91. Show HN: Web Audio Studio – A Visual Debugger for Web Audio API Graphs

**原文标题**: Show HN: Web Audio Studio – A Visual Debugger for Web Audio API Graphs

**原文链接**: [https://webaudio.studio/](https://webaudio.studio/)

生成摘要时出错

---

## 92. Libxml2 Enterprise Edition (AGPL, from the previous maintainer)

**原文标题**: Libxml2 Enterprise Edition (AGPL, from the previous maintainer)

**原文链接**: [https://codeberg.org/nwellnhof/libxml2-ee](https://codeberg.org/nwellnhof/libxml2-ee)

生成摘要时出错

---

## 93. "All Lawful Use": More Than You Wanted to Know

**原文标题**: "All Lawful Use": More Than You Wanted to Know

**原文链接**: [https://www.astralcodexten.com/p/all-lawful-use-much-more-than-you](https://www.astralcodexten.com/p/all-lawful-use-much-more-than-you)

生成摘要时出错

---

## 94. Pentagon Adopts Incel-Speak

**原文标题**: Pentagon Adopts Incel-Speak

**原文链接**: [https://www.theguardian.com/science/2026/mar/01/incel-slang-mainstream-government-media](https://www.theguardian.com/science/2026/mar/01/incel-slang-mainstream-government-media)

生成摘要时出错

---

## 95. Can Europe break free of Visa and Mastercard? MEPs stall digital euro

**原文标题**: Can Europe break free of Visa and Mastercard? MEPs stall digital euro

**原文链接**: [https://www.euronews.com/my-europe/2026/02/27/can-europe-break-free-of-visa-and-mastercard-meps-stall-digital-euro](https://www.euronews.com/my-europe/2026/02/27/can-europe-break-free-of-visa-and-mastercard-meps-stall-digital-euro)

生成摘要时出错

---

## 96. I Built a Scheme Compiler with AI in 4 Days

**原文标题**: I Built a Scheme Compiler with AI in 4 Days

**原文链接**: [https://matthewphillips.info/programming/posts/i-built-a-scheme-compiler-with-ai/](https://matthewphillips.info/programming/posts/i-built-a-scheme-compiler-with-ai/)

生成摘要时出错

---

## 97. Lil' Fun Langs' Guts

**原文标题**: Lil' Fun Langs' Guts

**原文链接**: [https://taylor.town/scrapscript-001](https://taylor.town/scrapscript-001)

生成摘要时出错

---

## 98. Anthropic's Claude rises to No. 2 in the App Store following Pentagon dispute

**原文标题**: Anthropic's Claude rises to No. 2 in the App Store following Pentagon dispute

**原文链接**: [https://techcrunch.com/2026/02/28/anthropics-claude-rises-to-no-2-in-the-app-store-following-pentagon-dispute/](https://techcrunch.com/2026/02/28/anthropics-claude-rises-to-no-2-in-the-app-store-following-pentagon-dispute/)

生成摘要时出错

---

## 99. The inner workings of TCP zero-copy

**原文标题**: The inner workings of TCP zero-copy

**原文链接**: [https://blog.tohojo.dk/2026/02/the-inner-workings-of-tcp-zero-copy.html](https://blog.tohojo.dk/2026/02/the-inner-workings-of-tcp-zero-copy.html)

生成摘要时出错

---

## 100. 390TB video game archive being taken offline due to skyrocketing RAM, SSD

**原文标题**: 390TB video game archive being taken offline due to skyrocketing RAM, SSD

**原文链接**: [https://www.tomshardware.com/video-games/390tb-video-game-archive-being-taken-offline-due-to-skyrocketing-ram-ssd-and-hard-drive-prices-ai-driven-supply-squeeze-results-in-closure-of-one-of-the-largest-online-video-game-archives](https://www.tomshardware.com/video-games/390tb-video-game-archive-being-taken-offline-due-to-skyrocketing-ram-ssd-and-hard-drive-prices-ai-driven-supply-squeeze-results-in-closure-of-one-of-the-largest-online-video-game-archives)

生成摘要时出错

---

