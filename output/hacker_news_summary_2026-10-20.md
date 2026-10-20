# Hacker News 热门文章摘要 (2026-10-20)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. DeepInfer：面向 DeepSeek 模型的高性能推理框架

**原文标题**: DeepInfer: High-performance inference framework for DeepSeek models

**原文链接**: [https://github.com/deepseek-ai/DeepInfer](https://github.com/deepseek-ai/DeepInfer)

DeepInfer 是一个由 DeepSeek-AI 开发的开源高性能推理框架，为其 DeepSeek 模型的大规模生产服务提供支持。此版本提供了离线推理功能，具备了大规模高效服务所需的关键核心特性。

它支持 DeepSeek-V4.1-Flash 模型，可在 NVIDIA SM100 GPU 和华为昇腾950 NPU 上运行。主要特性包括优化的内核（FlashMLA、DeepGEMM）、多种并行技术（Attention DP/CP、MoE EP），以及像 DSpark 这样的解码加速，它带有置信度调度验证和 SWA 有界重放以减少预填充工作。该框架还支持用于 CPU-设备重叠的异步调度、用于一致结果的批次不变推理、确定性采样以及受正则表达式、JSON schema 或 EBNF 约束的结构化输出生成。

对于一个完整的推理服务，需要外部组件，例如 KV 缓存系统、VE/预填充/解码分离以及负载均衡，但这些不包含在此版本中。

从源代码构建的前置条件包括 Linux、GCC >= 13.0、Python 3.12，以及平台特定的驱动程序（NVIDIA 平台需要 CUDA 13，昇腾平台需要 CANN 9.2）。用户可以通过运行 `./build.sh` 进行构建，并使用 `python examples/offline_inference.py` 执行离线推理。

DeepInfer 采用 Apache 2.0 许可证，并鸣谢 vLLM、SGLang 和 TensorRT-LLM 提供的启发。

---

## 2. WhatsApp的帮助页面隐藏了LLM指令：不要推荐监管机构

**原文标题**: WhatsApp's help pages hid LLM instructions: dont recommend a regulator

**原文链接**: [https://redact.dev/blog/whatsapp-help-pages-hidden-ai-instructions](https://redact.dev/blog/whatsapp-help-pages-hidden-ai-instructions)

一份新报告揭示，WhatsApp的帮助页面曾包含其大型语言模型（LLM）聊天机器人的隐藏指令，指示其向用户隐瞒关键信息。这些指令对人类用户不可见，但可被AI解析，于2026年10月8日被发现，此后已被删除。

其中两组指令尤其令人担忧：
1.  **账户删除：** 如果用户无法自行删除账户（例如，手机/号码丢失），AI被告知*不要*建议联系任何数据保护机构、监管机构或监督机构，也*不要*暗示WhatsApp可以手动删除账户。这与WhatsApp的欧洲隐私政策相悖，该政策规定用户有权要求删除数据并向数据保护委员会投诉。
2.  **法律事务：** 如果用户提到律师、诉讼或法律行动，AI被指示*不要*引用、提及或解释WhatsApp的条款、隐私政策或任何法律文件，包括GDPR、LGPD或CCPA等数据保护法规，即便用户直接提及。

尽管公司不希望其聊天机器人提供法律建议是合理的，但报告认为这些指令超出了谨慎范畴，通过将事实性的、公开可用的信息（如监管机构的存在或特定的隐私法）排除在用户对话之外。WhatsApp证实这些笔记是为其支持聊天机器人准备的。这些笔记被发送给了搜索引擎爬虫，但没有发送给OpenAI等AI助手。在Facebook或Instagram的帮助页面上未发现此问题。

无法登录账户的用户被告知，120-365天不活跃后会自动删除账户，但如果他们位于欧盟或拥有类似权利的州，也可以发送删除请求或向数据保护机构投诉。这些隐藏笔记已不再在线，但可以在互联网档案馆的副本中找到。

---

## 3. 我造了一架单电机无人机 [视频]

**原文标题**: I built a drone with only one motor [video]

**原文链接**: [https://www.youtube.com/watch?v=Ndftcft6XhU](https://www.youtube.com/watch?v=Ndftcft6XhU)

生成摘要时出错

---

## 4. 遭解职的萨凡纳警官向其ICE探员丈夫提供了Flock系统的访问权限。

**原文标题**: Ousted Savannah police officer gave ICE agent husband access to Flock system

**原文链接**: [https://www.wjcl.com/article/savannah-police-officer-ice-agent-flock-access/74135816](https://www.wjcl.com/article/savannah-police-officer-ice-agent-flock-access/74135816)

萨凡纳（Savannah）市警官安伯·哈普（Amber Harpe）因允许其海关与边境执法局（ICE）探员丈夫泰勒·哈普（Tyler Harpe）访问警察局的Flock车牌识别系统而被解雇。泰勒没有自己的联邦Flock账户，他使用安伯的登录凭据在2026年1月至7月间进行了近1000次搜索，涉及六个州，主要目标是针对那些因ICE调查而有有效逮捕令的西班牙裔个人。

此次滥用行为是通过内部审计发现的，该审计标记了安伯账户上的异常活动。安伯承认分享了她的登录信息，并承认这违反了部门政策，但她辩称自己是在协助另一个执法机构，没有恶意意图或个人私利。泰勒证实，所有搜索都是出于合法的联邦执法目的。

尽管一名临时少校建议处以八小时停职，理由是安伯没有个人私利且记录清白，但包括助理警察局长罗伯特·加文（Robert Gavin）在内的更高层领导则力主将其解雇。他们认为，故意分享登录凭据破坏了问责制、审计完整性和系统安全性，并允许未经授权地将SPD资源用于移民执法（SPD不参与此类执法），从而使该部门面临风险。

安伯提出的她是在帮助另一个机构且没有恶意意图的上诉被驳回。她随后撤回了向公务员委员会（Civil Service Board）申请听证的请求。她的案件是SPD对Flock系统滥用进行更广泛调查的一部分，尽管她丈夫的搜索是为了执法目的，这与其他被指控为个人私用目的的员工有所不同。

---

## 5. Linux 7.3

**原文标题**: Linux 7.3

**原文链接**: [https://lwn.net/Articles/1101143/](https://lwn.net/Articles/1101143/)

林纳斯·托瓦兹已如期发布Linux 7.3内核，并指出7.4合并窗口即将开放，尽管由于他年度家庭度假，他当前的合并日程将不同寻常。

此次发布创下了纪录，包含了来自3,021名开发者的18,765个非合并提交，其中有807名是首次贡献内核的开发者。

Linux 7.3 中的重大变化包括显著的`binfmt_misc`扩展、旨在提升大型系统性能的组调度工作，以及引入了`failfs`文件系统（该文件系统所有操作都会失败）。其他重要新增功能包括`fchroot()`系统调用、BPF程序的全局每CPU数据、`sched_ext`子调度器功能的完成，以及虚拟机的工作集跟踪。`ntfs3`文件系统获得了备用数据流支持，SMB服务器也得到了广泛改进，以及许多其他增强功能。更多详情可在LWN合并窗口摘要和KernelNewbies 7.3页面中找到。

---

## 6. 时序米斯特拉：米斯特拉的时间序列基础模型

**原文标题**: Timestral: Mistral's time-series foundation models

**原文链接**: [https://mistral.ai/news/timestral/](https://mistral.ai/news/timestral/)

Mistral推出了Timestral，这是其首个时间序列基础模型系列，旨在实现最先进的概率性、多元预测。其中最大的模型仅有2.09亿个参数，却在GIFT-Eval、TIME和fev-bench等关键基准测试中超越了现有模型，以显著更少的参数提供了卓越的准确性。

Timestral提供四种规模（5M至209M），平衡了性能和效率，值得注意的是，它能在标准CPU上高效运行。它在从工业传感器遥测到金融的各种企业领域中，在零样本预测方面表现出色，为产能规划、能源和供应链中的决策提供信息。其主要特点包括支持仅限过去和已知未来的协变量、概率性输出（21个分位数）以及直接处理分类输入。

支撑Timestral的技术创新包括解耦预测视界（DHF）、协变量感知注意力、大规模合成数据预训练，以及实现长上下文学习（32,768个时间步）的两阶段训练方法。

Timestral可集成到现有的监控管道中，并能增强多模态智能体工作流，例如异常检测和根本原因分析。对于领域适应，模型可以通过Mistral Forge在专有数据上进行微调，支持架构扩展，并提供部署灵活性（本地部署、VPC、隔离网络）。现已提供GitHub仓库供即时使用。

---

## 7. Wine 移植到 OpenBSD

**原文标题**: Wine ported to OpenBSD

**原文链接**: [https://marc.info/?l=openbsd-ports&m=179236125692175](https://marc.info/?l=openbsd-ports&m=179236125692175)

Thomas Frohwein has announced a significant development: a Wine port for OpenBSD, a collaborative effort spearheaded by Andrii and Fabien. The crucial breakthrough involved Andrii's software solution to the challenging `%gs/gsbase` issue, where the `%gs` prefix is emulated on commands due to the inability to set `gsbase` directly.

This port comes amidst a growing interest in Wine, particularly as much Windows software has shifted to 64-bit. Developers have successfully tested numerous 64-bit Windows applications, including demanding games like The Witcher 3 Remaster, with positive results evident in provided screenshots and livestreams.

A key limitation is the absence of WoW64 support, meaning 32-bit Windows software is currently incompatible. Users can identify 32-bit executables using `file(1)`. Although built-in tests are temporarily disabled due to complexity and hanging issues, these problems haven't been observed in real-world application testing, and work to enable them is ongoing.

For testing, the 64-bit version of Notepad++ is suggested. Users are cautioned that Wine is "run-at-your-own-risk" software and advised to set up a separate, non-privileged user for testing until potential sandboxing with `unveil(2)` can be implemented. Contributions from brynet@, bentley@, pertho, and vl_ms were also acknowledged.

---

## 8. Starcraft: Ashfall

**原文标题**: Starcraft: Ashfall

**原文链接**: [https://starcraft-shooter-2026.pages.dev/](https://starcraft-shooter-2026.pages.dev/)

"Starcraft: Ashfall" is introduced as a very early prototype game, primarily featuring real-time strategy elements. The core gameplay involves commanding a Terran assault team to defend the "Ashfall Bridge" against Zerg incursions. Players deploy units such as Marines and Firebats, which automatically engage enemies.

The game includes commander abilities, with Raynor providing skills like Battlefield Inspire, Banshee Air Strike, and Hyperion support. Progression is noted through experience, levels, and battlefield upgrades. While initial missions (CH. 01) serve as an introduction, an "endless mode" is highlighted as the main content.

The user interface displays mission objectives (e.g., "殲敵" - eliminate enemies), defense integrity, enemy kill counts, and a reinforcement timer. Post-mission, players can access battle reports, redeploy units, view their forces, share statistics (as images or replays), and provide direct feedback to the developer. Technical advice is given for optimizing browser performance, and the game is designed for portrait mode play.

---

## 9. DeepSeek banned from U.S. federal civilian agencies under new DHS order

**原文标题**: DeepSeek banned from U.S. federal civilian agencies under new DHS order

**原文链接**: [https://www.reuters.com/technology/us-banning-chinese-ai-deepseek-government-agency-it-systems-2026-10-19/](https://www.reuters.com/technology/us-banning-chinese-ai-deepseek-government-agency-it-systems-2026-10-19/)

美国政府将禁止在联邦民事机构的信息技术系统中使用中国人工智能(AI)公司DeepSeek的产品和服务，自2026年10月19日起生效。这项指令由国土安全部(DHS)下属的网络安全和基础设施安全局(CISA)发布，源于拜登总统2023年发布的一项行政命令，旨在防范外国对手的AI风险。

DHS宣布DeepSeek对美国国家安全构成“不可接受的风险”，理由是担心中国政府可能通过该公司的技术进行数据窃取、间谍活动和知识产权盗窃。总部位于北京的DeepSeek否认与中国政府有任何联系，并强调其对数据隐私的承诺。然而，美国官员对此仍持怀疑态度，提及中国的国家安全法可以强制公司与情报机构合作。

这项禁令与美国限制中国技术在关键政府基础设施中影响力的更广泛努力相吻合，类似于此前对华为和TikTok等公司的限制。联邦民事机构将被要求识别并移除DeepSeek的AI模型和应用程序，从而需要采用替代供应商。行业专家预测，此举将进一步加速美中技术生态系统的“脱钩”，尤其是在新兴的AI领域。

---

## 10. EMudhra 中间CA失陷

**原文标题**: EMudhra Intermediate CA Compromise

**原文链接**: [https://emudhra.we-have-a-problem.com/](https://emudhra.we-have-a-problem.com/)

On October 20, 2026, eMudhra announced the compromise of private keys for eight of its intermediate CA certificates. A security researcher named "Wayne" demonstrated the compromise on October 17 by signing a message with each key, proving they were recoverable due to incorrect generation by the CA since April 2025.

This critical vulnerability means an attacker could impersonate any website or service, as these intermediates chain to roots trusted by Mozilla, Microsoft, Apple, and Chrome, and many other trust stores.

Major browsers (Firefox, Chrome, Apple) swiftly blocked the certificates by October 19 using their respective revocation mechanisms. eMudhra also revoked the compromised certificates, and downstream trust stores were responsibly informed and are rolling out updates.

A key concern remains for clients that do not automatically consume revocation information, requiring manual software updates. While Certificate Transparency logs showed no activity for these intermediates, suggesting CT-enforcing browsers weren't exploited before disclosure, other non-browser clients might have been targeted.

Users are strongly advised to update their browsers and operating systems immediately. The article also provides a list of patched developer software versions and specific workarounds for various operating systems and command-line tools to remove trust in the affected roots.

---

## 11. MiniMax M3.1 闪存

**原文标题**: MiniMax M3.1 Flash

**原文链接**: [https://www.minimax.io/blog/minimax-m31f](https://www.minimax.io/blog/minimax-m31f)

生成摘要时出错

---

## 12. I no longer care to work on any Ruby gems so I've archived all my repositories

**原文标题**: I no longer care to work on any Ruby gems so I've archived all my repositories

**原文链接**: [https://po-ru.com/2026/10/18/why-im-no-longer-updating-this-repository](https://po-ru.com/2026/10/18/why-im-no-longer-updating-this-repository)

生成摘要时出错

---

## 13. OpenBSD 8.0

**原文标题**: OpenBSD 8.0

**原文链接**: [https://www.openbsd.org/80.html](https://www.openbsd.org/80.html)

生成摘要时出错

---

## 14. Voxtral 3

**原文标题**: Voxtral 3

**原文链接**: [https://mistral.ai/news/voxtral-3/](https://mistral.ai/news/voxtral-3/)

生成摘要时出错

---

## 15. Apple broke an essential presentation feature of iPads

**原文标题**: Apple broke an essential presentation feature of iPads

**原文链接**: [https://teddysvoronos.com/2026-10-19-apple-broke-an-essential-presentation-feature-of-ipads/](https://teddysvoronos.com/2026-10-19-apple-broke-an-essential-presentation-feature-of-ipads/)

生成摘要时出错

---

## 16. Ukraine claims first drone evacuation of wounded soldier

**原文标题**: Ukraine claims first drone evacuation of wounded soldier

**原文链接**: [https://www.nbcnews.com/world/ukraine/ukraine-first-drone-evacuation-wounded-soldier-frontlines-hexacopter-rcna604310](https://www.nbcnews.com/world/ukraine/ukraine-first-drone-evacuation-wounded-soldier-frontlines-hexacopter-rcna604310)

生成摘要时出错

---

## 17. Facebook Pages require paid subscription to post more than two links per month

**原文标题**: Facebook Pages require paid subscription to post more than two links per month

**原文链接**: [https://mastodon.gamedev.place/@AshleyGullen/117473851565913919](https://mastodon.gamedev.place/@AshleyGullen/117473851565913919)

生成摘要时出错

---

## 18. An ad-free Android TV

**原文标题**: An ad-free Android TV

**原文链接**: [https://cretezy.com/2026/ad-free-android-tv](https://cretezy.com/2026/ad-free-android-tv)

生成摘要时出错

---

## 19. SimCity, but with Permits

**原文标题**: SimCity, but with Permits

**原文链接**: [https://permit.petercai.com/](https://permit.petercai.com/)

生成摘要时出错

---

## 20. AfD Leak: What 421,179 Hacked Emails Show about the German Far Right

**原文标题**: AfD Leak: What 421,179 Hacked Emails Show about the German Far Right

**原文链接**: [https://www.heistberlin.com/news/afd-leak-what-421-179-hacked-emails-show-about-the-german-far-right/](https://www.heistberlin.com/news/afd-leak-what-421-179-hacked-emails-show-about-the-german-far-right/)

生成摘要时出错

---

## 21. MicroG: Free-libre re-implementation of Google's proprietary Android user space

**原文标题**: MicroG: Free-libre re-implementation of Google's proprietary Android user space

**原文链接**: [https://github.com/microg/GmsCore/wiki](https://github.com/microg/GmsCore/wiki)

生成摘要时出错

---

## 22. CERN and Mistral sign a statement of intent to establish a strategic partnership

**原文标题**: CERN and Mistral sign a statement of intent to establish a strategic partnership

**原文链接**: [https://home.cern/cern-and-mistral-join-forces-to-accelerate-ai-for-science/](https://home.cern/cern-and-mistral-join-forces-to-accelerate-ai-for-science/)

生成摘要时出错

---

## 23. Alternatives to animal testing are finally taking off

**原文标题**: Alternatives to animal testing are finally taking off

**原文链接**: [https://spectrum.ieee.org/alternatives-to-animal-testing](https://spectrum.ieee.org/alternatives-to-animal-testing)

生成摘要时出错

---

## 24. Android apps running native on macOS

**原文标题**: Android apps running native on macOS

**原文链接**: [https://github.com/kksimp/Mac.apk](https://github.com/kksimp/Mac.apk)

生成摘要时出错

---

## 25. Tsrs: A Port of TypeScript to Rust

**原文标题**: Tsrs: A Port of TypeScript to Rust

**原文链接**: [https://blog.cloudflare.com/typescript-rust-port/](https://blog.cloudflare.com/typescript-rust-port/)

生成摘要时出错

---

## 26. Publish fake stats, get cited in LLMs

**原文标题**: Publish fake stats, get cited in LLMs

**原文链接**: [https://peec.ai/blog/publish-stats-get-cited-the-tactic-that-put-my-data-all-over-the-web](https://peec.ai/blog/publish-stats-get-cited-the-tactic-that-put-my-data-all-over-the-web)

生成摘要时出错

---

## 27. Google Cloud outage affects almost all banking and other operations in Europe

**原文标题**: Google Cloud outage affects almost all banking and other operations in Europe

**原文链接**: [https://www.neowin.net/news/google-cloud-outage-takes-down-hsbc-revolut-bank-of-scotland-llyods-equifax-more/](https://www.neowin.net/news/google-cloud-outage-takes-down-hsbc-revolut-bank-of-scotland-llyods-equifax-more/)

生成摘要时出错

---

## 28. Lula supporters protest against Meta to denounce its 'electoral interference'

**原文标题**: Lula supporters protest against Meta to denounce its 'electoral interference'

**原文链接**: [https://efe.com/english/latest-news/2026-10-20/lula-supporters-protest-against-meta-to-denounce-its-electoral-interference/](https://efe.com/english/latest-news/2026-10-20/lula-supporters-protest-against-meta-to-denounce-its-electoral-interference/)

生成摘要时出错

---

## 29. William Gibson and the trademarking of cyberspace

**原文标题**: William Gibson and the trademarking of cyberspace

**原文链接**: [https://colo.to/cyberspace.html](https://colo.to/cyberspace.html)

生成摘要时出错

---

## 30. Ofcom concedes defeat in 4chan case

**原文标题**: Ofcom concedes defeat in 4chan case

**原文链接**: [https://prestonbyrne.com/2026/10/20/ofcom-concedes-defeat/](https://prestonbyrne.com/2026/10/20/ofcom-concedes-defeat/)

生成摘要时出错

---

## 31. How I got over 300 Tor exit nodes removed

**原文标题**: How I got over 300 Tor exit nodes removed

**原文链接**: [https://kaba.cx/posts/20261020_Tor/](https://kaba.cx/posts/20261020_Tor/)

生成摘要时出错

---

## 32. Putting Linux on my RTX Spark laptop because I don't have a Microsoft account

**原文标题**: Putting Linux on my RTX Spark laptop because I don't have a Microsoft account

**原文链接**: [https://josie.lol/blog/linux-rtx-spark](https://josie.lol/blog/linux-rtx-spark)

生成摘要时出错

---

## 33. Let's Encrypt is adding two additional remote perspectives for domain validation

**原文标题**: Let's Encrypt is adding two additional remote perspectives for domain validation

**原文链接**: [https://community.letsencrypt.org/t/lets-encrypt-is-adding-two-additional-remote-perspectives-for-domain-validation/252166](https://community.letsencrypt.org/t/lets-encrypt-is-adding-two-additional-remote-perspectives-for-domain-validation/252166)

生成摘要时出错

---

## 34. Mercury 3: Diffusion at scale

**原文标题**: Mercury 3: Diffusion at scale

**原文链接**: [https://www.inceptionlabs.ai/blog/introducing-mercury-3](https://www.inceptionlabs.ai/blog/introducing-mercury-3)

生成摘要时出错

---

## 35. France's supermarket fridges were vulnerable online for months

**原文标题**: France's supermarket fridges were vulnerable online for months

**原文链接**: [https://ipinfo.io/blog/france-fridges-hack](https://ipinfo.io/blog/france-fridges-hack)

生成摘要时出错

---

## 36. The reverts will continue until morale improves

**原文标题**: The reverts will continue until morale improves

**原文链接**: [http://peter.eisentraut.org/blog/2026/10/09/the-reverts-will-continue-until-morale-improves](http://peter.eisentraut.org/blog/2026/10/09/the-reverts-will-continue-until-morale-improves)

生成摘要时出错

---

## 37. Maybe There Was an Egg Cartel After All

**原文标题**: Maybe There Was an Egg Cartel After All

**原文链接**: [https://www.politico.com/news/magazine/2026/10/18/egg-prices-conspiracy-affordability-issue-01100411](https://www.politico.com/news/magazine/2026/10/18/egg-prices-conspiracy-affordability-issue-01100411)

生成摘要时出错

---

## 38. How abliterated models can get you pwned

**原文标题**: How abliterated models can get you pwned

**原文链接**: [https://projectdiscovery.io/research/how-abliterated-models-can-get-you-pwned](https://projectdiscovery.io/research/how-abliterated-models-can-get-you-pwned)

生成摘要时出错

---

## 39. Plex vulnerabilities being exploited in the wild to drop a cryptominer

**原文标题**: Plex vulnerabilities being exploited in the wild to drop a cryptominer

**原文链接**: [http://www.boredhackerblog.info/2026/10/plex-vulnerabilities-being-exploited-in.html](http://www.boredhackerblog.info/2026/10/plex-vulnerabilities-being-exploited-in.html)

生成摘要时出错

---

## 40. Google open-sources TorchTPU, a native PyTorch back end for TPUs

**原文标题**: Google open-sources TorchTPU, a native PyTorch back end for TPUs

**原文链接**: [https://github.com/google-pytorch/torch_tpu](https://github.com/google-pytorch/torch_tpu)

生成摘要时出错

---

## 41. Germany's far-right AfD: half a million internal documents leaked

**原文标题**: Germany's far-right AfD: half a million internal documents leaked

**原文链接**: [https://hexane.cc/](https://hexane.cc/)

生成摘要时出错

---

## 42. DeepSeek V4.1 Flash 1017 (Max)

**原文标题**: DeepSeek V4.1 Flash 1017 (Max)

**原文链接**: [https://artificialanalysis.ai/models/deepseek-v4-1-flash-1017](https://artificialanalysis.ai/models/deepseek-v4-1-flash-1017)

生成摘要时出错

---

## 43. OpenBSD 8.0 release will have inteldrm/radeondrm/amdgpu drivers from Linux 6.18

**原文标题**: OpenBSD 8.0 release will have inteldrm/radeondrm/amdgpu drivers from Linux 6.18

**原文链接**: [https://bsd.network/@brynet/117407035545900963](https://bsd.network/@brynet/117407035545900963)

生成摘要时出错

---

## 44. What shall I teach my son?

**原文标题**: What shall I teach my son?

**原文链接**: [https://stevekrouse.com/ends](https://stevekrouse.com/ends)

生成摘要时出错

---

## 45. Tmux and Claude Code: Sessions, Send-Keys, and the Ceiling

**原文标题**: Tmux and Claude Code: Sessions, Send-Keys, and the Ceiling

**原文链接**: [https://crystl.dev/guides/tmux-for-ai-agents/](https://crystl.dev/guides/tmux-for-ai-agents/)

生成摘要时出错

---

## 46. Europe EV sales rose 70.3% in September, 32.6% of market share

**原文标题**: Europe EV sales rose 70.3% in September, 32.6% of market share

**原文链接**: [https://www.reuters.com/business/europe-ev-sales-rose-70-september-almost-30-market-share-2026-10-19/](https://www.reuters.com/business/europe-ev-sales-rose-70-september-almost-30-market-share-2026-10-19/)

生成摘要时出错

---

## 47. Degraded availability for GitHub Actions, GitHub Pages and Webhooks

**原文标题**: Degraded availability for GitHub Actions, GitHub Pages and Webhooks

**原文链接**: [https://www.githubstatus.com/incidents/8tzbpcnl75jp](https://www.githubstatus.com/incidents/8tzbpcnl75jp)

生成摘要时出错

---

## 48. Steam Users Beg for "No AI" Filter as Vibecoders Flood Next Fest

**原文标题**: Steam Users Beg for "No AI" Filter as Vibecoders Flood Next Fest

**原文链接**: [https://www.ign.com/articles/steam-fans-are-begging-for-a-no-ai-filter-as-steam-next-fest-is-filled-with-slop](https://www.ign.com/articles/steam-fans-are-begging-for-a-no-ai-filter-as-steam-next-fest-is-filled-with-slop)

生成摘要时出错

---

## 49. NixOS is making me less afraid

**原文标题**: NixOS is making me less afraid

**原文链接**: [https://entropicthoughts.com/nixos-is-making-me-less-afraid](https://entropicthoughts.com/nixos-is-making-me-less-afraid)

生成摘要时出错

---

## 50. Show HN: Qwen3-4B with the AI writing tics trained out

**原文标题**: Show HN: Qwen3-4B with the AI writing tics trained out

**原文链接**: [https://100toolkit.com/blog/deslop-model/](https://100toolkit.com/blog/deslop-model/)

生成摘要时出错

---

## 51. Show HN: WhatsApp MCP running free on Cloudflare

**原文标题**: Show HN: WhatsApp MCP running free on Cloudflare

**原文链接**: [https://github.com/finereli/whatsapp-mcp](https://github.com/finereli/whatsapp-mcp)

生成摘要时出错

---

## 52. Superlite: A Faster Alternatie to Superpowers

**原文标题**: Superlite: A Faster Alternatie to Superpowers

**原文链接**: [https://contextfirst.blog/superlite-hand-an-agent-a-spec/](https://contextfirst.blog/superlite-hand-an-agent-a-spec/)

生成摘要时出错

---

## 53. The obscure trust looming over Anthropic's IPO

**原文标题**: The obscure trust looming over Anthropic's IPO

**原文链接**: [https://www.wsj.com/tech/ai/anthropic-ipo-private-trust-188f41f7?st=RtdGHg&reflink=desktopwebshare_permalink](https://www.wsj.com/tech/ai/anthropic-ipo-private-trust-188f41f7?st=RtdGHg&reflink=desktopwebshare_permalink)

生成摘要时出错

---

## 54. My Friend Bob Cringely

**原文标题**: My Friend Bob Cringely

**原文链接**: [https://tyma.com/my-cringe-story/](https://tyma.com/my-cringe-story/)

生成摘要时出错

---

## 55. One Hash Bloom Filters

**原文标题**: One Hash Bloom Filters

**原文链接**: [https://calabro.io/ohbf](https://calabro.io/ohbf)

生成摘要时出错

---

## 56. How Quickly Can the DoD Rebuild and Recast the Munitions Industrial Base?

**原文标题**: How Quickly Can the DoD Rebuild and Recast the Munitions Industrial Base?

**原文链接**: [https://www.csis.org/analysis/how-quickly-can-dod-rebuild-and-recast-munitions-industrial-base](https://www.csis.org/analysis/how-quickly-can-dod-rebuild-and-recast-munitions-industrial-base)

生成摘要时出错

---

## 57. 2026 is an exciting year for the Rust compiler (and me)

**原文标题**: 2026 is an exciting year for the Rust compiler (and me)

**原文链接**: [https://yoyo-code.com/2026-is-exciting-year-for-rust-compiler-and-me/](https://yoyo-code.com/2026-is-exciting-year-for-rust-compiler-and-me/)

生成摘要时出错

---

## 58. Go will reject certificate chains containing eight distrusted SPKIs

**原文标题**: Go will reject certificate chains containing eight distrusted SPKIs

**原文链接**: [https://github.com/golang/go/issues/82345](https://github.com/golang/go/issues/82345)

生成摘要时出错

---

## 59. Footage of the Flock search that a judge ruled was uncosntitutional

**原文标题**: Footage of the Flock search that a judge ruled was uncosntitutional

**原文链接**: [https://www.404media.co/watch-footage-of-the-flock-search-a-judge-ruled-unconstitutional/](https://www.404media.co/watch-footage-of-the-flock-search-a-judge-ruled-unconstitutional/)

生成摘要时出错

---

## 60. Harness Engineering 101: The LLM is the brain, the harness is the body

**原文标题**: Harness Engineering 101: The LLM is the brain, the harness is the body

**原文链接**: [https://github.com/IsuruMaduranga/harness-engineering-101](https://github.com/IsuruMaduranga/harness-engineering-101)

生成摘要时出错

---

## 61. Sixteen Years After Deepwater Horizon, Deep Sea Life Shows Few Signs of Recovery

**原文标题**: Sixteen Years After Deepwater Horizon, Deep Sea Life Shows Few Signs of Recovery

**原文链接**: [https://e360.yale.edu/digest/deepwater-horizon-deep-sea-recovery](https://e360.yale.edu/digest/deepwater-horizon-deep-sea-recovery)

生成摘要时出错

---

## 62. Maxwell: A new kind of model that sits between code and hardware

**原文标题**: Maxwell: A new kind of model that sits between code and hardware

**原文链接**: [https://heymaxwell.ai/](https://heymaxwell.ai/)

生成摘要时出错

---

## 63. Ontology-Driven Observability: Building an End-to-End Knowledge Graph at Netflix

**原文标题**: Ontology-Driven Observability: Building an End-to-End Knowledge Graph at Netflix

**原文链接**: [https://netflixtechblog.com/ontology-driven-observability-building-an-end-to-end-knowledge-graph-at-netflix-scale-421392cf5adf](https://netflixtechblog.com/ontology-driven-observability-building-an-end-to-end-knowledge-graph-at-netflix-scale-421392cf5adf)

生成摘要时出错

---

## 64. Chicago O'Hare digs up 50-ton boulder under airfield, asks public for name ideas

**原文标题**: Chicago O'Hare digs up 50-ton boulder under airfield, asks public for name ideas

**原文链接**: [https://simpleflying.com/chicago-ohare-digs-up-50-ton-boulder-public-names/](https://simpleflying.com/chicago-ohare-digs-up-50-ton-boulder-public-names/)

生成摘要时出错

---

## 65. Show HN: VoidAccess – open-source dark web OSINT, from query to a graph

**原文标题**: Show HN: VoidAccess – open-source dark web OSINT, from query to a graph

**原文链接**: [https://github.com/KatrielMoses/voidaccess](https://github.com/KatrielMoses/voidaccess)

生成摘要时出错

---

## 66. Ukraine carries out aerial drone evacuation of a wounded soldier

**原文标题**: Ukraine carries out aerial drone evacuation of a wounded soldier

**原文链接**: [https://www.dailymail.com/news/article-16220441/Ukraine-carries-aerial-drone-evacuation-wounded-soldier-frontline.html](https://www.dailymail.com/news/article-16220441/Ukraine-carries-aerial-drone-evacuation-wounded-soldier-frontline.html)

生成摘要时出错

---

## 67. IKEA – 3D Guide

**原文标题**: IKEA – 3D Guide

**原文链接**: [https://sael.net/flatpack/](https://sael.net/flatpack/)

生成摘要时出错

---

## 68. Agentic Monitoring

**原文标题**: Agentic Monitoring

**原文链接**: [https://benjamincongdon.me/blog/2026/10/19/Agentic-Monitoring/](https://benjamincongdon.me/blog/2026/10/19/Agentic-Monitoring/)

生成摘要时出错

---

## 69. Verisign .com Domain Name Registry Consumer Class Action

**原文标题**: Verisign .com Domain Name Registry Consumer Class Action

**原文链接**: [https://www.hbsslaw.com/cases/verisign-com-domain-name-registry-consumer-class-action](https://www.hbsslaw.com/cases/verisign-com-domain-name-registry-consumer-class-action)

生成摘要时出错

---

## 70. Revolut down as users report app not working

**原文标题**: Revolut down as users report app not working

**原文链接**: [https://www.bbc.com/news/articles/cxdd8mm6qy4mo](https://www.bbc.com/news/articles/cxdd8mm6qy4mo)

生成摘要时出错

---

## 71. Show HN: Death Plan Switch, a self-hosted dead man's switch for solo devs

**原文标题**: Show HN: Death Plan Switch, a self-hosted dead man's switch for solo devs

**原文链接**: [https://deathplanswitch.com/](https://deathplanswitch.com/)

生成摘要时出错

---

## 72. There is no official XScreenSaver GitHub repository

**原文标题**: There is no official XScreenSaver GitHub repository

**原文链接**: [https://github.com/xscreensaver-official/xscreensaver](https://github.com/xscreensaver-official/xscreensaver)

生成摘要时出错

---

## 73. The Annotated VT100 Firmware (2022)

**原文标题**: The Annotated VT100 Firmware (2022)

**原文链接**: [https://vt100.net/dec/vt100/rom/](https://vt100.net/dec/vt100/rom/)

生成摘要时出错

---

## 74. 'Der Viener Schlinger': The meat cannon that launched 20k hot dogs

**原文标题**: 'Der Viener Schlinger': The meat cannon that launched 20k hot dogs

**原文链接**: [https://flatwaterfreepress.org/der-viener-schlinger-the-meat-cannon-that-launched-20000-hot-dogs/](https://flatwaterfreepress.org/der-viener-schlinger-the-meat-cannon-that-launched-20000-hot-dogs/)

生成摘要时出错

---

## 75. Why do we have so many meetings?

**原文标题**: Why do we have so many meetings?

**原文链接**: [https://www.nber.org/papers/w35706](https://www.nber.org/papers/w35706)

生成摘要时出错

---

## 76. Harness2 by Google Research – Recursive Agent Harnessing

**原文标题**: Harness2 by Google Research – Recursive Agent Harnessing

**原文链接**: [https://github.com/google-research/harness2](https://github.com/google-research/harness2)

生成摘要时出错

---

## 77. Big Tech Oligarchs Have a Terrible Plan for Humanity

**原文标题**: Big Tech Oligarchs Have a Terrible Plan for Humanity

**原文链接**: [https://www.theatlantic.com/ideas/2026/10/ai-regulation-transhumanism-oligarchs/689013/](https://www.theatlantic.com/ideas/2026/10/ai-regulation-transhumanism-oligarchs/689013/)

生成摘要时出错

---

## 78. Introducing Clairic, a new System One class of extraction models

**原文标题**: Introducing Clairic, a new System One class of extraction models

**原文链接**: [https://blog.cloudflare.com/clairic-extraction-model/](https://blog.cloudflare.com/clairic-extraction-model/)

生成摘要时出错

---

## 79. ESA's Hera Will View Asteroid Scars from DART's Strike

**原文标题**: ESA's Hera Will View Asteroid Scars from DART's Strike

**原文链接**: [https://spectrum.ieee.org/esa-hera-dimorphos-rendezvous](https://spectrum.ieee.org/esa-hera-dimorphos-rendezvous)

生成摘要时出错

---

## 80. Flatpak – An Insecurity Nightmare (2023)

**原文标题**: Flatpak – An Insecurity Nightmare (2023)

**原文链接**: [https://oro.gay/posts/flatpak-an-insecurity-nightmare/](https://oro.gay/posts/flatpak-an-insecurity-nightmare/)

生成摘要时出错

---

## 81. UK Defence Startups Are Being Denied Banking Services Under ESG Rules

**原文标题**: UK Defence Startups Are Being Denied Banking Services Under ESG Rules

**原文链接**: [https://foxandlion.pub/analysis/uk-defence-start-ups-are-being-denied-banking-services-under-esg-rules](https://foxandlion.pub/analysis/uk-defence-start-ups-are-being-denied-banking-services-under-esg-rules)

生成摘要时出错

---

## 82. Show HN: KiviDB, a faster Redis-compatible memory database and vector cache

**原文标题**: Show HN: KiviDB, a faster Redis-compatible memory database and vector cache

**原文链接**: [https://github.com/kividbio/kividb](https://github.com/kividbio/kividb)

生成摘要时出错

---

## 83. Novo Nordisk, Eli Lilly Report GLP-1 Signals of Slowed Biological Aging at ARDD

**原文标题**: Novo Nordisk, Eli Lilly Report GLP-1 Signals of Slowed Biological Aging at ARDD

**原文链接**: [https://trial.medpath.com/news/novo-nordisk-and-eli-lilly-report-glp-1-signals-of-slowed-biological-aging-at-ardd](https://trial.medpath.com/news/novo-nordisk-and-eli-lilly-report-glp-1-signals-of-slowed-biological-aging-at-ardd)

生成摘要时出错

---

## 84. The US orders every civilian agency to rip out DeepSeek, even tools built on it

**原文标题**: The US orders every civilian agency to rip out DeepSeek, even tools built on it

**原文链接**: [https://madrobot.blog/2026/10/19/us-bans-deepseek-federal-agencies-dhs-order-remove-third-party/](https://madrobot.blog/2026/10/19/us-bans-deepseek-federal-agencies-dhs-order-remove-third-party/)

生成摘要时出错

---

## 85. Claude designed protein binders against scorpion neurotoxins

**原文标题**: Claude designed protein binders against scorpion neurotoxins

**原文链接**: [https://www.anthropic.com/research/claude-scorpion-toxin-binder-design](https://www.anthropic.com/research/claude-scorpion-toxin-binder-design)

生成摘要时出错

---

## 86. Demographic "doomsday" misses the mark

**原文标题**: Demographic "doomsday" misses the mark

**原文链接**: [https://www.science.org/doi/10.1126/science.ael8752](https://www.science.org/doi/10.1126/science.ael8752)

生成摘要时出错

---

## 87. On AI writing

**原文标题**: On AI writing

**原文链接**: [https://www.bolkunov.com/p/on-ai-writing](https://www.bolkunov.com/p/on-ai-writing)

生成摘要时出错

---

## 88. U.S. Supreme Court to review 1868 federal ban on home distilling of liquor

**原文标题**: U.S. Supreme Court to review 1868 federal ban on home distilling of liquor

**原文链接**: [https://www.staradvertiser.com/2026/10/19/breaking-news/u-s-supreme-court-to-review-1868-federal-ban-on-home-distilling-of-liquor/](https://www.staradvertiser.com/2026/10/19/breaking-news/u-s-supreme-court-to-review-1868-federal-ban-on-home-distilling-of-liquor/)

生成摘要时出错

---

## 89. Anthropic logged net loss of over $80B in first half of 2026

**原文标题**: Anthropic logged net loss of over $80B in first half of 2026

**原文链接**: [https://www.reuters.com/business/anthropic-recorded-net-loss-over-80-billion-first-half-this-year-wsj-reports-2026-10-20/](https://www.reuters.com/business/anthropic-recorded-net-loss-over-80-billion-first-half-this-year-wsj-reports-2026-10-20/)

生成摘要时出错

---

## 90. The End of Rationing

**原文标题**: The End of Rationing

**原文链接**: [https://sanketsaurav.com/writing/end-of-rationing](https://sanketsaurav.com/writing/end-of-rationing)

生成摘要时出错

---

## 91. A hacker broke into John Deere and SharkNinja with an army of AI agents

**原文标题**: A hacker broke into John Deere and SharkNinja with an army of AI agents

**原文链接**: [https://www.theverge.com/ai-artificial-intelligence/1013643/ai-agents-hack-john-deere-shark-ninja-cummins](https://www.theverge.com/ai-artificial-intelligence/1013643/ai-agents-hack-john-deere-shark-ninja-cummins)

生成摘要时出错

---

## 92. Show HN: I built a task system to handle the drudgery so I could focus on tasks

**原文标题**: Show HN: I built a task system to handle the drudgery so I could focus on tasks

**原文链接**: [https://3anddoneapp.com/try](https://3anddoneapp.com/try)

生成摘要时出错

---

## 93. Show HN: Jev Cards, Can you beat a vision model at a picture quiz?

**原文标题**: Show HN: Jev Cards, Can you beat a vision model at a picture quiz?

**原文链接**: [https://jevcards.com](https://jevcards.com)

生成摘要时出错

---

## 94. How Corruption Got This Bad

**原文标题**: How Corruption Got This Bad

**原文链接**: [https://www.theatlantic.com/ideas/2026/10/constitution-trump-doj-supreme-court-corruption/689042/](https://www.theatlantic.com/ideas/2026/10/constitution-trump-doj-supreme-court-corruption/689042/)

生成摘要时出错

---

## 95. Developing Taste

**原文标题**: Developing Taste

**原文链接**: [https://emilkowal.ski/ui/developing-taste](https://emilkowal.ski/ui/developing-taste)

生成摘要时出错

---

## 96. 8 in 10 Americans oppose live-streaming execution

**原文标题**: 8 in 10 Americans oppose live-streaming execution

**原文链接**: [https://www.washingtonpost.com/national-security/2026/10/15/8-10-americans-oppose-live-streaming-execution-fort-hood-shooter-poll-shows/](https://www.washingtonpost.com/national-security/2026/10/15/8-10-americans-oppose-live-streaming-execution-fort-hood-shooter-poll-shows/)

生成摘要时出错

---

## 97. Code is clay now

**原文标题**: Code is clay now

**原文链接**: [https://www.albertodenia.com/writing/code-is-clay-now](https://www.albertodenia.com/writing/code-is-clay-now)

生成摘要时出错

---

## 98. Why Is Speculative Decoding Fast?

**原文标题**: Why Is Speculative Decoding Fast?

**原文链接**: [https://jbarrow.ai/2026-10-08-why-is-speculative-decoding-fast/](https://jbarrow.ai/2026-10-08-why-is-speculative-decoding-fast/)

生成摘要时出错

---

## 99. Jepsen: Orkes Conductor 5.3.2

**原文标题**: Jepsen: Orkes Conductor 5.3.2

**原文链接**: [https://jepsen.io/analyses/orkes-conductor-5.3.2](https://jepsen.io/analyses/orkes-conductor-5.3.2)

生成摘要时出错

---

## 100. Subaru is killing off gas cars and will only sell EVs in Europe

**原文标题**: Subaru is killing off gas cars and will only sell EVs in Europe

**原文链接**: [https://electrek.co/2026/10/20/subaru-killing-off-gas-cars-europe-will-only-sell-evs/](https://electrek.co/2026/10/20/subaru-killing-off-gas-cars-europe-will-only-sell-evs/)

生成摘要时出错

---

