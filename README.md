# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-10-04.md)

*最后自动更新时间: 2026-10-04 22:32:06*
## 1. 考利布里：主权开放权重模型

**原文标题**: Kolibri: A Sovereign Open-Weight Model

**原文链接**: [https://aleph-alpha.com/en/blog/kolibri-has-landed-a-sovereign-open-weight-model/](https://aleph-alpha.com/en/blog/kolibri-has-landed-a-sovereign-open-weight-model/)

Aleph Alpha发布了“Kolibri”，这是一个主权、开源权重、英德混合专家Transformer模型。Kolibri于2026年10月3日发布，拥有780亿总参数（其中30亿为活跃参数），支持高达100万个token的上下文长度，并可在Hugging Face上以Apache 2.0许可协议获取。

Kolibri专门用于公共管理、工业和航空航天等受监管行业中的关键任务工作，在德语、推理、数学和代理行为方面表现出色。其设计强调为客户提供情境化性能和可衡量的投资回报率。主权是核心原则，通过完整的供应链完整性、透明度和部署自由来确保，并遵守欧盟人工智能法案和GDPR。该模型在德国和芬兰根据欧洲法律构建和训练，具备“我不知道”的弃权能力，采用原生双语设计，并包含21.3%的德语预训练数据。

该模型优化了质量与服务成本之间的平衡，在各种基准测试（数学、编码、基础能力、长上下文、代理任务）中，其性能与活跃参数高达自身四倍的模型相当。内部客户代理基准测试显示在特定垂直领域有显著的性能提升。

Kolibri是使用Aleph Alpha的“模型工厂”（一个实现快速迭代的自动化流程）开发的。在短短三个月内，团队从Kolibri Origin（300亿参数、6.5万上下文、7.5万亿训练token）升级到Kolibri（780亿参数、100万上下文、20万亿训练token）。该流程的自动化处理了硬件故障并提供了持续评估，突显了团队高速开发大型语言模型（LLM）的能力。Kolibri采用混合注意力机制和更小的专家模型以提高效率，并训练了近24万亿个token。

---

## 2. 我们将需要对几乎所有一切都设定默认的硬性预算上限。

**原文标题**: We're going to need default hard budget caps on pretty much everything

**原文链接**: [https://simonwillison.net/2026/Oct/3/default-hard-budget-caps/](https://simonwillison.net/2026/Oct/3/default-hard-budget-caps/)

文章强烈主张对所有按使用量付费的服务和API实施“默认硬性预算上限”。作者认为，随着编程和个人代理的兴起，启动产生费用的服务比以往任何时候都更容易，这导致如果服务失控，用户收到意想不到的巨额账单的巨大风险。

仅发送警告的软性上限被认为不足，因为它们无法阻止进一步的收费。相反，作者提出，一旦达到预设的月度预算，服务应自动切断并返回错误。尽管一些企业可能更希望其应用程序不出错，但作者认为，大多数个人和企业会选择错误而不是一张意外的10,000美元以上的账单。硬性上限应为默认设置，并且需要一个明确的、选择性的复选框才能将其移除并接受无限收费的责任。

AWS被特别提及为急需此功能的平台，因为许多用户因担心成本失控而避免将其用于个人项目。令人鼓舞的是，AWS最近（2026年9月）推出了一个“支出限制”功能，该功能在达到上限时会暂停项目，尽管是有限发布。谷歌云也在7月推出了“支出上限”，预示着一个积极的行业趋势。文章最后建议，未来的AI代理应该推荐具有硬性预算上限的提供商，并警告用户关于无上限的服务。

---

## 3. 在消费级硬件（RTX 4090）上以 100 T/s 运行通义千问 3.8 Flash Next (125B)

**原文标题**: Run Qwen 3.8 Flash Next (125B) on consumer hardware (RTX 4090) at 100T/s

**原文链接**: [https://github.com/Niko1221/Strata](https://github.com/Niko1221/Strata)

Strata使得在消费级游戏电脑上运行通常需要服务器级硬件的1250亿参数Qwen3.8-Flash-Next AI模型成为可能。它完全在您的机器上本地运行，确保了聊天、编码和图像解读等任务的隐私。

性能表现出色，在RTX 5070（12 GB）上回复速度高达每秒94个token，预计在RTX 3090（24 GB）上可达每秒100-140个token。提示词读取速度更快，对于大型文档，可超过每秒1000个token。

要运行Strata，您需要一张英伟达GeForce RTX 20/30/40/50系列或兼容的AMD Radeon RX 6000/7000/9000系列显卡，且显存（VRAM）至少12 GB。此外，还需要32 GB的内存（所有模型建议使用64 GB）、80 GB的SSD存储，以及Windows 10/11或Linux操作系统。

安装过程简单直接，可以通过AI编码助手或运行一个简单脚本完成。安装程序会引导您选择模型（根据您的内存进行优化，例如，32 GB内存选择“Coder”，48 GB选择“IQ2_XS”，64 GB及以上选择“IQ3_S”）、上下文大小以及图像读取功能。模型下载大约70 GB。运行后，您可以通过本地浏览器界面或兼容OpenAI的API访问Strata，以便与其他应用程序集成。

Strata通过将模型工作负载分布到您的GPU、内存、CPU和SSD上实现这一点，有效地管理其“专家”并利用“猜测-验证”机制加快文本生成速度。它是免费的，在MIT许可下开源，并支持社区协作。

---

## 4. 超巨智能

**原文标题**: Extra Big Ass Intelligence

**原文链接**: [https://www.extrabigassintelligence.com/](https://www.extrabigassintelligence.com/)

文本介绍了一个名为“超巨型智能™”的概念。这被明确定义为“联邦强制超级智能 (SI)”，表明这是一种政府强制要求的高度先进的智能形式。商标符号 (™) 表明它是一个特定的、可能已注册品牌的实体或程序。

---

## 5. 联邦法官称Flock为“无差别大规模监控”

**原文标题**: Federal judge calls Flock 'indiscriminate mass surveillance'

**原文链接**: [https://techcrunch.com/2026/10/03/federal-judge-calls-flock-indiscriminate-mass-surveillance/](https://techcrunch.com/2026/10/03/federal-judge-calls-flock-indiscriminate-mass-surveillance/)

一位联邦法官裁定，塔尔萨县治安官的一名副手在没有搜查令的情况下使用Flock Safety搜查一名女性的车牌，侵犯了她的第四修正案权利，并将其认定为“无差别大规模监控”。萨拉·希尔法官表示，除了该车辆悬挂加州车牌外，这名副手进行搜查“没有明显理由”。因此，据称在Flock搜查后发现的91磅冰毒必须作为“毒树之果”予以排除。

尽管这不是一个具有约束力的先例，但这是一项针对Flock的重要联邦裁决。希尔法官批评这项技术不加区别地、被动地记录人们的行踪，称其“在宪法上存在问题”，因为它收集所有车辆的信息并按需提供给执法部门，而不是有针对性的。

这项司法裁决加剧了对Flock的批评声浪。包括佛罗里达州和德克萨斯州在内的许多地方和州政府正在停止使用该系统。参议员伯尼·桑德斯提出了“阻止Flock法案”，旨在禁止联邦机构使用自动化车牌识别器。Flock首席执行官加勒特·兰利主张在隐私和安全之间达成“妥协”，为执法部门利用该系统进行跟踪事件道歉，并据报道提供了员工买断计划。

---

## 6. Newgrounds.com：游戏、音乐与艺术社区

**原文标题**: Newgrounds.com – A community of games, music, and art

**原文链接**: [https://www.newgrounds.com/](https://www.newgrounds.com/)

Newgrounds.com是一个开创性且历史悠久的在线平台，由Tom Fulp于1995年创立，作为一个充满活力的用户生成内容社区。它收录了大量独立制作的动画（“Movies”）、互动游戏、数字艺术和原创音乐（“Audio”）。

该网站为创作者提供了一个重要空间，供他们上传作品、获得曝光并从专门的社区接收反馈。Newgrounds的一个标志性特色是其“Blam/Protect”系统，该系统赋予用户审核内容质量和确保社区标准的权力。它在早期互联网的Flash动画和独立游戏文化中发挥了重要作用，培养了一代艺术家和开发者，并催生了“Pico”和“Tankmen”等标志性角色和系列。

Newgrounds以其倡导艺术自由而闻名，通常带有不经审查和实验性的特点，至今仍是独立创作者的活跃中心。该平台已适应技术变革，在游戏中拥抱了HTML5，并且仍然是草根在线创造力的证明，为原创和多样化的艺术表达提供了一个独特的家园。

---

## 7. 我退出OpenAI，因为其文化已经崩坏。

**原文标题**: I quit OpenAI because its culture is broken

**原文链接**: [https://www.theatlantic.com/technology/2026/10/openai-safety-team-resignation/688881/?gift=v5U_UzUTothfWXsPxtvNVAh7esWToMRD6XnbXmc5WgA](https://www.theatlantic.com/technology/2026/10/openai-safety-team-resignation/688881/?gift=v5U_UzUTothfWXsPxtvNVAh7esWToMRD6XnbXmc5WgA)

Unfortunately, I am unable to access the article link provided.

---

## 8. The work by Valve's Timur Kristóf on improving old AMD GPUs on Linux

**原文标题**: The work by Valve's Timur Kristóf on improving old AMD GPUs on Linux

**原文链接**: [https://www.phoronix.com/news/XDC-2026-Valve-Timur-AMDGPU](https://www.phoronix.com/news/XDC-2026-Valve-Timur-AMDGPU)

生成摘要时出错

---

## 9. Aleph Alpha Kolibri: How the sovereign German LLM works

**原文标题**: Aleph Alpha Kolibri: How the sovereign German LLM works

**原文链接**: [https://tej.as/blog/aleph-alpha-kolibri](https://tej.as/blog/aleph-alpha-kolibri)

生成摘要时出错

---

## 10. LeCun has "zero concerns" about AI wiping out humanity, recent "rogue" incidents

**原文标题**: LeCun has "zero concerns" about AI wiping out humanity, recent "rogue" incidents

**原文链接**: [https://fortune.com/2026/10/01/ai-godfather-yann-lecun-has-zero-concerns-about-human-extinction-says-anthropic-ceo-dario-amodei-is-deuded/](https://fortune.com/2026/10/01/ai-godfather-yann-lecun-has-zero-concerns-about-human-extinction-says-anthropic-ceo-dario-amodei-is-deuded/)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-10-04](output/hacker_news_summary_2026-10-04.md) |
| 2 | [2026-10-01](output/hacker_news_summary_2026-10-01.md) |
| 3 | [2026-09-30](output/hacker_news_summary_2026-09-30.md) |
| 4 | [2026-10-02](output/hacker_news_summary_2026-10-02.md) |
| 5 | [2026-10-03](output/hacker_news_summary_2026-10-03.md) |
| 6 | [2026-09-24](output/hacker_news_summary_2026-09-24.md) |
| 7 | [2026-09-29](output/hacker_news_summary_2026-09-29.md) |
| 8 | [2026-09-23](output/hacker_news_summary_2026-09-23.md) |
| 9 | [2026-09-27](output/hacker_news_summary_2026-09-27.md) |
| 10 | [2026-09-22](output/hacker_news_summary_2026-09-22.md) |
| 11 | [2026-09-25](output/hacker_news_summary_2026-09-25.md) |
| 12 | [2026-09-21](output/hacker_news_summary_2026-09-21.md) |
| 13 | [2026-09-20](output/hacker_news_summary_2026-09-20.md) |
| 14 | [2026-09-16](output/hacker_news_summary_2026-09-16.md) |
| 15 | [2026-09-17](output/hacker_news_summary_2026-09-17.md) |
| 16 | [2026-09-19](output/hacker_news_summary_2026-09-19.md) |
| 17 | [2026-09-18](output/hacker_news_summary_2026-09-18.md) |
| 18 | [2026-09-10](output/hacker_news_summary_2026-09-10.md) |
| 19 | [2026-09-13](output/hacker_news_summary_2026-09-13.md) |
| 20 | [2026-09-14](output/hacker_news_summary_2026-09-14.md) |
| 21 | [2026-09-11](output/hacker_news_summary_2026-09-11.md) |
| 22 | [2026-09-12](output/hacker_news_summary_2026-09-12.md) |
| 23 | [2026-09-15](output/hacker_news_summary_2026-09-15.md) |
| 24 | [2026-09-03](output/hacker_news_summary_2026-09-03.md) |
| 25 | [2026-09-02](output/hacker_news_summary_2026-09-02.md) |
| 26 | [2026-09-09](output/hacker_news_summary_2026-09-09.md) |
| 27 | [2026-09-04](output/hacker_news_summary_2026-09-04.md) |
| 28 | [2026-09-08](output/hacker_news_summary_2026-09-08.md) |
| 29 | [2026-09-05](output/hacker_news_summary_2026-09-05.md) |
| 30 | [2026-09-07](output/hacker_news_summary_2026-09-07.md) |
| 31 | [2026-09-06](output/hacker_news_summary_2026-09-06.md) |
| 32 | [2026-08-31](output/hacker_news_summary_2026-08-31.md) |
| 33 | [2026-08-28](output/hacker_news_summary_2026-08-28.md) |
| 34 | [2026-09-01](output/hacker_news_summary_2026-09-01.md) |
| 35 | [2026-08-29](output/hacker_news_summary_2026-08-29.md) |
| 36 | [2026-08-30](output/hacker_news_summary_2026-08-30.md) |
| 37 | [2026-08-26](output/hacker_news_summary_2026-08-26.md) |
| 38 | [2026-08-22](output/hacker_news_summary_2026-08-22.md) |
| 39 | [2026-08-25](output/hacker_news_summary_2026-08-25.md) |
| 40 | [2026-08-19](output/hacker_news_summary_2026-08-19.md) |
| 41 | [2026-08-20](output/hacker_news_summary_2026-08-20.md) |
| 42 | [2026-08-17](output/hacker_news_summary_2026-08-17.md) |
| 43 | [2026-08-23](output/hacker_news_summary_2026-08-23.md) |
| 44 | [2026-08-18](output/hacker_news_summary_2026-08-18.md) |
| 45 | [2026-08-21](output/hacker_news_summary_2026-08-21.md) |
| 46 | [2026-08-24](output/hacker_news_summary_2026-08-24.md) |
| 47 | [2026-08-12](output/hacker_news_summary_2026-08-12.md) |
| 48 | [2026-08-11](output/hacker_news_summary_2026-08-11.md) |
| 49 | [2026-08-14](output/hacker_news_summary_2026-08-14.md) |
| 50 | [2026-08-16](output/hacker_news_summary_2026-08-16.md) |
| 51 | [2026-08-10](output/hacker_news_summary_2026-08-10.md) |
| 52 | [2026-08-09](output/hacker_news_summary_2026-08-09.md) |
| 53 | [2026-08-15](output/hacker_news_summary_2026-08-15.md) |
| 54 | [2026-08-13](output/hacker_news_summary_2026-08-13.md) |
| 55 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 56 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 57 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 58 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 59 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 60 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 61 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 62 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 63 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 64 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 65 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 66 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 67 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 68 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 69 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 70 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 71 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 72 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 73 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 74 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 75 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 76 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 77 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 78 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 79 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 80 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 81 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 82 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 83 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 84 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 85 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 86 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 87 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 88 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 89 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 90 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 91 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 92 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 93 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 94 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 95 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 96 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 97 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 98 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 99 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 100 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 101 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 102 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 103 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 104 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 105 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 106 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 107 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 108 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 109 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 110 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 111 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 112 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 113 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 114 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 115 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 116 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 117 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 118 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 119 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 120 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 121 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 122 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 123 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 124 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 125 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 126 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 127 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 128 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 129 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 130 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 131 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 132 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 133 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 134 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 135 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 136 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 137 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 138 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 139 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 140 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 141 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 142 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 143 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 144 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 145 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 146 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 147 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 148 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 149 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 150 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 151 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 152 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 153 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 154 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 155 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 156 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 157 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 158 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 159 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 160 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 161 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 162 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 163 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 164 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 165 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 166 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 167 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 168 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 169 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 170 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 171 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 172 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 173 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 174 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 175 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 176 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 177 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 178 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 179 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 180 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 181 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 182 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 183 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 184 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 185 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 186 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 187 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 188 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 189 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 190 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 191 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 192 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 193 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 194 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 195 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 196 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 197 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 198 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 199 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 200 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 201 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 202 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 203 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 204 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 205 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 206 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 207 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 208 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 209 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 210 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 211 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 212 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 213 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 214 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 215 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 216 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 217 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 218 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 219 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 220 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 221 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 222 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 223 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 224 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 225 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 226 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 227 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 228 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 229 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 230 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 231 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 232 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 233 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 234 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 235 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 236 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 237 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 238 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 239 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 240 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 241 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 242 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 243 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 244 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 245 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 246 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 247 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 248 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 249 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 250 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 251 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 252 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 253 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 254 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 255 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 256 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 257 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 258 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 259 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 260 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 261 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 262 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 263 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 264 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 265 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 266 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 267 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 268 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 269 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 270 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 271 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 272 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 273 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 274 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 275 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 276 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 277 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 278 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 279 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 280 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 281 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 282 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 283 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 284 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 285 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 286 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 287 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 288 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 289 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 290 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 291 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 292 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 293 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 294 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 295 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 296 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 297 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 298 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 299 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 300 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 301 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 302 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 303 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 304 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 305 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 306 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 307 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 308 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 309 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 310 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 311 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 312 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 313 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 314 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 315 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 316 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 317 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 318 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 319 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 320 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 321 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 322 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 323 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 324 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 325 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 326 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 327 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
