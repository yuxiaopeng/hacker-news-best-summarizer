# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-10-20.md)

*最后自动更新时间: 2026-10-20 22:36:47*
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

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-10-20](output/hacker_news_summary_2026-10-20.md) |
| 2 | [2026-10-17](output/hacker_news_summary_2026-10-17.md) |
| 3 | [2026-10-18](output/hacker_news_summary_2026-10-18.md) |
| 4 | [2026-10-19](output/hacker_news_summary_2026-10-19.md) |
| 5 | [2026-10-13](output/hacker_news_summary_2026-10-13.md) |
| 6 | [2026-10-15](output/hacker_news_summary_2026-10-15.md) |
| 7 | [2026-10-14](output/hacker_news_summary_2026-10-14.md) |
| 8 | [2026-10-16](output/hacker_news_summary_2026-10-16.md) |
| 9 | [2026-10-10](output/hacker_news_summary_2026-10-10.md) |
| 10 | [2026-10-11](output/hacker_news_summary_2026-10-11.md) |
| 11 | [2026-10-07](output/hacker_news_summary_2026-10-07.md) |
| 12 | [2026-10-06](output/hacker_news_summary_2026-10-06.md) |
| 13 | [2026-10-04](output/hacker_news_summary_2026-10-04.md) |
| 14 | [2026-10-02](output/hacker_news_summary_2026-10-02.md) |
| 15 | [2026-10-03](output/hacker_news_summary_2026-10-03.md) |
| 16 | [2026-10-09](output/hacker_news_summary_2026-10-09.md) |
| 17 | [2026-09-24](output/hacker_news_summary_2026-09-24.md) |
| 18 | [2026-10-01](output/hacker_news_summary_2026-10-01.md) |
| 19 | [2026-09-29](output/hacker_news_summary_2026-09-29.md) |
| 20 | [2026-09-30](output/hacker_news_summary_2026-09-30.md) |
| 21 | [2026-09-27](output/hacker_news_summary_2026-09-27.md) |
| 22 | [2026-09-25](output/hacker_news_summary_2026-09-25.md) |
| 23 | [2026-09-21](output/hacker_news_summary_2026-09-21.md) |
| 24 | [2026-09-23](output/hacker_news_summary_2026-09-23.md) |
| 25 | [2026-09-20](output/hacker_news_summary_2026-09-20.md) |
| 26 | [2026-09-22](output/hacker_news_summary_2026-09-22.md) |
| 27 | [2026-09-19](output/hacker_news_summary_2026-09-19.md) |
| 28 | [2026-09-18](output/hacker_news_summary_2026-09-18.md) |
| 29 | [2026-09-13](output/hacker_news_summary_2026-09-13.md) |
| 30 | [2026-09-16](output/hacker_news_summary_2026-09-16.md) |
| 31 | [2026-09-14](output/hacker_news_summary_2026-09-14.md) |
| 32 | [2026-09-17](output/hacker_news_summary_2026-09-17.md) |
| 33 | [2026-09-15](output/hacker_news_summary_2026-09-15.md) |
| 34 | [2026-09-09](output/hacker_news_summary_2026-09-09.md) |
| 35 | [2026-09-10](output/hacker_news_summary_2026-09-10.md) |
| 36 | [2026-09-08](output/hacker_news_summary_2026-09-08.md) |
| 37 | [2026-09-05](output/hacker_news_summary_2026-09-05.md) |
| 38 | [2026-09-07](output/hacker_news_summary_2026-09-07.md) |
| 39 | [2026-09-06](output/hacker_news_summary_2026-09-06.md) |
| 40 | [2026-09-11](output/hacker_news_summary_2026-09-11.md) |
| 41 | [2026-09-12](output/hacker_news_summary_2026-09-12.md) |
| 42 | [2026-09-03](output/hacker_news_summary_2026-09-03.md) |
| 43 | [2026-09-02](output/hacker_news_summary_2026-09-02.md) |
| 44 | [2026-08-31](output/hacker_news_summary_2026-08-31.md) |
| 45 | [2026-09-04](output/hacker_news_summary_2026-09-04.md) |
| 46 | [2026-09-01](output/hacker_news_summary_2026-09-01.md) |
| 47 | [2026-08-29](output/hacker_news_summary_2026-08-29.md) |
| 48 | [2026-08-30](output/hacker_news_summary_2026-08-30.md) |
| 49 | [2026-08-22](output/hacker_news_summary_2026-08-22.md) |
| 50 | [2026-08-25](output/hacker_news_summary_2026-08-25.md) |
| 51 | [2026-08-20](output/hacker_news_summary_2026-08-20.md) |
| 52 | [2026-08-28](output/hacker_news_summary_2026-08-28.md) |
| 53 | [2026-08-23](output/hacker_news_summary_2026-08-23.md) |
| 54 | [2026-08-21](output/hacker_news_summary_2026-08-21.md) |
| 55 | [2026-08-24](output/hacker_news_summary_2026-08-24.md) |
| 56 | [2026-08-26](output/hacker_news_summary_2026-08-26.md) |
| 57 | [2026-08-12](output/hacker_news_summary_2026-08-12.md) |
| 58 | [2026-08-14](output/hacker_news_summary_2026-08-14.md) |
| 59 | [2026-08-19](output/hacker_news_summary_2026-08-19.md) |
| 60 | [2026-08-16](output/hacker_news_summary_2026-08-16.md) |
| 61 | [2026-08-17](output/hacker_news_summary_2026-08-17.md) |
| 62 | [2026-08-18](output/hacker_news_summary_2026-08-18.md) |
| 63 | [2026-08-15](output/hacker_news_summary_2026-08-15.md) |
| 64 | [2026-08-13](output/hacker_news_summary_2026-08-13.md) |
| 65 | [2026-08-11](output/hacker_news_summary_2026-08-11.md) |
| 66 | [2026-08-10](output/hacker_news_summary_2026-08-10.md) |
| 67 | [2026-08-09](output/hacker_news_summary_2026-08-09.md) |
| 68 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 69 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 70 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 71 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 72 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 73 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 74 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 75 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 76 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 77 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 78 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 79 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 80 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 81 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 82 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 83 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 84 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 85 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 86 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 87 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 88 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 89 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 90 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 91 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 92 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 93 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 94 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 95 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 96 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 97 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 98 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 99 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 100 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 101 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 102 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 103 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 104 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 105 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 106 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 107 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 108 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 109 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 110 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 111 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 112 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 113 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 114 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 115 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 116 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 117 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 118 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 119 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 120 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 121 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 122 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 123 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 124 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 125 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 126 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 127 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 128 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 129 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 130 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 131 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 132 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 133 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 134 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 135 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 136 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 137 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 138 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 139 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 140 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 141 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 142 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 143 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 144 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 145 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 146 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 147 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 148 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 149 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 150 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 151 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 152 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 153 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 154 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 155 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 156 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 157 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 158 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 159 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 160 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 161 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 162 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 163 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 164 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 165 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 166 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 167 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 168 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 169 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 170 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 171 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 172 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 173 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 174 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 175 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 176 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 177 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 178 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 179 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 180 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 181 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 182 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 183 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 184 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 185 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 186 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 187 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 188 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 189 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 190 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 191 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 192 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 193 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 194 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 195 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 196 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 197 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 198 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 199 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 200 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 201 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 202 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 203 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 204 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 205 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 206 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 207 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 208 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 209 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 210 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 211 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 212 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 213 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 214 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 215 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 216 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 217 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 218 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 219 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 220 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 221 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 222 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 223 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 224 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 225 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 226 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 227 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 228 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 229 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 230 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 231 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 232 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 233 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 234 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 235 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 236 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 237 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 238 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 239 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 240 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 241 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 242 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 243 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 244 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 245 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 246 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 247 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 248 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 249 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 250 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 251 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 252 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 253 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 254 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 255 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 256 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 257 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 258 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 259 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 260 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 261 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 262 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 263 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 264 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 265 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 266 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 267 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 268 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 269 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 270 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 271 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 272 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 273 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 274 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 275 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 276 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 277 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 278 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 279 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 280 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 281 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 282 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 283 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 284 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 285 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 286 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 287 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 288 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 289 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 290 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 291 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 292 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 293 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 294 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 295 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 296 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 297 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 298 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 299 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 300 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 301 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 302 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 303 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 304 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 305 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 306 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 307 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 308 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 309 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 310 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 311 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 312 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 313 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 314 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 315 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 316 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 317 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 318 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 319 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 320 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 321 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 322 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 323 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 324 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 325 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 326 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 327 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 328 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 329 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 330 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 331 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 332 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 333 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 334 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 335 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 336 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 337 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 338 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 339 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 340 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
