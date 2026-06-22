# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-06-22.md)

*最后自动更新时间: 2026-06-22 21:42:48*
## 1. 可销售软件的最小可行单元

**原文标题**: The minimum viable unit of saleable software

**原文链接**: [https://brandur.org/minimum-viable-unit](https://brandur.org/minimum-viable-unit)

在《可销售软件的最小可行单元》一文中，作者Brandur探讨了在人工智能时代构建软件业务的可行性，特别是针对强大的大型语言模型（LLM）出现后“购买与自建”的权衡。

他认为，尽管LLM大大降低了软件的开发成本，但“便宜不等于免费”。LLM生成的代码仍需要人工进行提示、优化和维护，这其中包含显著的成本。他举例说明：将每月400美元的Jira订阅替换为内部通过LLM构建的追踪器，他计算出其工程小时成本（初始构建加持续维护）将远高于直接支付Jira费用。

然而，对于价格非常高的SaaS产品（例如，50个席位每月2.5万美元的Salesforce），自建内部替代方案确实变得更经济可行。这使他提出了可销售软件的“可行性区域”，该区域由两个条件定义：
1.  **足够的独特性：** 软件必须足够复杂，以至于通过LLM驱动的重建并非微不足道，并且需要持续维护。
2.  **合理的定价：** 价格不能高得离谱，以至于强烈促使用户选择自建。

“可销售软件的最小可行单元”位于一个临界点：购买第三方解决方案的成本小于或等于内部重建（即使有LLM辅助）所需付出的努力和成本。

作者将此框架应用于他的个人项目River，一个用于Go和Postgres的作业队列。他相信River Pro，通过提供高级功能和非线性扩展的定价模型（小型团队每月125美元），正处于这个可行性区域内，使其尽管在人工智能进步的背景下，仍然是一项可行的业务。

---

## 2. Show HN: 教孩子绝对音感

**原文标题**: Show HN: Teach your kids perfect pitch

**原文链接**: [https://github.com/paytonjjones/bsharp](https://github.com/paytonjjones/bsharp)

BSharp 是一款移动应用程序，旨在帮助幼童习得绝对音高（即完美音高），它利用了在六岁左右关闭的关键发育窗口期。该应用可在Play商店下载，它采用了江口（Eguchi）的和弦识别方法，教导儿童将钢琴和弦与不同颜色关联起来。

学习过程从两个和弦（红色和黄色）开始，随着孩子以100%的准确率掌握每个级别，逐步引入更多和弦。建议的练习时间表是每天五次练习，每次持续2-3分钟（20-25次识别）。新和弦的引入时间间隔不早于两周。BSharp 会跟踪准确性，使用自适应加权算法更频繁地呈现难度更高的和弦，并支持多个用户配置文件。

该应用会逐步学习9个初始白键和弦（例如，黄色代表F/C，蓝色代表G/B），随后是5个黑键和弦。BSharp 基于 Paul Ganssle 的开源 CIM 训练器，并采用 Apache 许可证 2.0。开发需要 Node.js。

---

## 3. 微调Qwen 3:0.6B等本地LLM用于问题分类，效果良好。

**原文标题**: Good results fine tuning a local LLM like Qwen 3:0.6B to categorize questions

**原文链接**: [https://www.teachmecoolstuff.com/viewarticle/fine-tuning-a-local-llm-to-categorize-questions](https://www.teachmecoolstuff.com/viewarticle/fine-tuning-a-local-llm-to-categorize-questions)

Torgeir Helgevold 开展了一个个人项目，旨在开发一个家用聊天机器人，用于对用户问题进行分类，以改进向量数据库中的RAG搜索效果。其核心假设是，一个非常小的本地大型语言模型，特别是Qwen 3:0.6B，能否通过微调可靠地将问题分类到预定义的元数据类别中（例如，游泳池、汽车、暖通空调）。

最初，仅通过提示词直接使用Qwen 0.6B模型，效果很差，在一个包含131个问题的测试集上，准确率仅为10%。该模型经常将问题误分类到宽泛的类别中，或者凭空创造出新的类别。

首次微调尝试中，利用Unsloth和QLora在一个包含约850个家庭问题的数据集上进行训练，准确率显著提升至79%。然而，模型仍然存在问题，有时会输出类别的片段（例如，“ac”而非“hvac”），或者混淆语义相似的类别，如“喷泉”、“热水器”和“游泳池”。

第二次微调实验引入了一个关键的调整：即不再要求模型输出完整的类别名称，而是提示它返回固定的两位字符不透明代码（例如，“KK”代表“hvac”）。这一简单的改变将准确率大幅提升至92%。尽管一些“与水相关”的混淆（例如，热水器被错误分类为游泳池）仍然存在，但微调后的LLM被证明是一个普遍可靠的预测器，使其适用于聊天机器人的预处理步骤。作者计划进一步完善训练数据，以解决剩余的歧义。一项更新还提到，正在探索使用逻辑回归作为替代分类方法。

---

## 4. 数位板品牌为何不合作开发 Linux 开源驱动？

**原文标题**: Why Drawing Tablet Brands Won't Collaborate on Linux Floss Drivers

**原文链接**: [https://www.davidrevoy.com/article1154/why-drawing-tablet-brands-wont-collaborate-on-linux-floss-drivers](https://www.davidrevoy.com/article1154/why-drawing-tablet-brands-wont-collaborate-on-linux-floss-drivers)

The author, a tech reviewer, tests drawing tablets on GNU/Linux using Free/Libre and Open Source (FLOSS) software and drivers. Historically, they've extracted tablet specifications and reported them to Red Hat developers, Peter Hutterer and Benjamin Tissoire, who then create FLOSS drivers via `udev-hid-bpf`.

Finding this process exhaustive, the author recently attempted a new strategy: direct collaboration with brands like Gaomon, XpPen, and Huion to share their device specifications. After extensive outreach, they successfully connected with a technical contact at Huion, who appeared to manage drivers for several brands. The author shared details of the existing FLOSS driver projects.

However, the initiative was politely rejected by Gaomon. Their technical team cited concerns that the current Linux FLOSS driver infrastructure (e.g., `libwacom`, `wacom-hid-descriptors`) is "Wacom-led" and branded after their largest competitor. They worried about sharing their device specifications directly with a Wacom-branded project and perceived limited impact for Gaomon if their devices were still associated with Wacom branding.

The author identifies this historical "Wacom branding" within the open-source infrastructure as a major barrier preventing other brands from collaborating. Despite the setback, the author will revert to their previous method of individually reviewing tablets and documenting their specifications, relying on the Red Hat developers' efforts. They hope this highlights the need for funding to rebrand and evolve the FLOSS driver repositories to foster broader industry collaboration.

---

## 5. 构建可靠的智能体AI系统

**原文标题**: Building reliable agentic AI systems

**原文链接**: [https://martinfowler.com/articles/reliable-llm-bayer.html](https://martinfowler.com/articles/reliable-llm-bayer.html)

本文详细介绍了PRINCE（临床前信息中心）的开发，该平台由拜耳公司和Thoughtworks共同打造，是一个云端平台，旨在通过解决访问海量临床前数据面临的挑战，彻底改变药物开发。PRINCE最初是一个基于关键词的搜索工具，后来发展成为一个智能研究助手，利用智能体检索增强生成（RAG）和Text-to-SQL技术，整合了数十年的安全性研究报告。

PRINCE的演进分为三个阶段：“搜索”（整合结构化元数据）、“提问”（利用AI驱动的RAG对非结构化PDF进行自然语言查询）和“执行”（一个多智能体系统，执行起草监管文件等复杂任务）。该系统的架构由LangGraph编排，采用专门的智能体（澄清用户意图、研究员、反思、撰写者），并强调“上下文工程”以优化信息流，以及“驾驭工程”以实现强大的编排、恢复和可观测性。

关键设计原则包括通过透明度、可解释性和人机协作整合来优先建立信任。该系统具备LLM回退、重试和错误上下文等弹性机制，并辅以广泛的监控（Langfuse、Cloudwatch）和评估（RAGAS框架）。PRINCE显著提升了制药领域的数据可访问性和研究效率，确保了治理和合规性，同时展示了AI的变革潜力。

---

## 6. 人工智能的十万个为什么

**原文标题**: The 100k whys of AI

**原文链接**: [https://lcamtuf.substack.com/p/the-100000-whys-of-ai](https://lcamtuf.substack.com/p/the-100000-whys-of-ai)

lcamtuf的文章《人工智能的十万个为什么》批判性地审视了人工智能（特别是大型语言模型LLM）的现状和局限性，通过质疑它们的真正理解能力和泛化能力。作者认为，尽管LLM擅长模式匹配和生成看似合理的文本，但它们根本缺乏对世界的因果理解。

核心论点是LLM并不理解事物“为什么”是真的，而仅仅知道“什么”词序列通常跟在其他词之后。这种对统计相关性的依赖使得它们在遇到训练数据之外的情景或需要真正推理时，变得脆弱并容易产生“幻觉”或逻辑错误。作者区分了“浅层”学习（系统识别模式）和“深层”理解（涉及因果关系和真正的泛化）。

文章指出，当前的人工智能进展类似于复杂的统计学鹦鹉，它们在模仿方面令人印象深刻，但缺乏真正的智能或常识。它警告不要夸大AI的能力，并强调需要取得突破，超越单纯的相关性，构建能够理解因果关系和上下文的模型，就像人类从极少量数据中学习一样。对“十万个为什么”的追求意味着寻求深刻的因果理解，而不仅仅是庞大的统计数据库。

---

## 7. 如何编写 Lisp 解释器 (Python 版) (2010)

**原文标题**: (How to Write a (Lisp) Interpreter (In Python)) (2010)

**原文链接**: [https://norvig.com/lispy.html](https://norvig.com/lispy.html)

本文题为《如何用Python编写Lisp解释器》，于2010年发表，是一篇教学性文章。其主要目的，正如标题所示，是指导读者逐步实践，构建一个Lisp编程语言的解释器。这篇指南的一个关键方面是它选择了Python作为实现语言。因此，文章很可能详细阐述了使用Python作为开发工具来构建Lisp解释器所需的流程、技术和代码示例。2010年的发表年份将内容置于当时特定的技术和教学背景之下。

---

## 8. Ask for no, don't ask for yes (2022)

**原文标题**: Ask for no, don't ask for yes (2022)

**原文链接**: [https://www.mooreds.com/wordpress/archives/3518](https://www.mooreds.com/wordpress/archives/3518)

生成摘要时出错

---

## 9. Moebius: 0.2B image inpainting model with 10B-level performance

**原文标题**: Moebius: 0.2B image inpainting model with 10B-level performance

**原文链接**: [https://hustvl.github.io/Moebius/](https://hustvl.github.io/Moebius/)

生成摘要时出错

---

## 10. Alan Greenspan has died

**原文标题**: Alan Greenspan has died

**原文链接**: [https://www.washingtonpost.com/obituaries/2026/06/22/alan-greenspan-most-powerful-central-banker-modern-times-dies-100/](https://www.washingtonpost.com/obituaries/2026/06/22/alan-greenspan-most-powerful-central-banker-modern-times-dies-100/)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 2 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 3 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 4 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 5 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 6 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 7 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 8 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 9 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 10 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 11 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 12 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 13 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 14 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 15 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 16 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 17 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 18 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 19 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 20 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 21 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 22 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 23 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 24 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 25 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 26 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 27 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 28 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 29 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 30 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 31 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 32 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 33 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 34 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 35 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 36 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 37 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 38 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 39 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 40 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 41 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 42 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 43 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 44 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 45 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 46 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 47 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 48 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 49 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 50 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 51 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 52 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 53 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 54 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 55 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 56 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 57 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 58 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 59 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 60 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 61 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 62 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 63 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 64 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 65 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 66 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 67 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 68 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 69 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 70 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 71 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 72 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 73 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 74 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 75 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 76 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 77 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 78 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 79 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 80 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 81 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 82 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 83 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 84 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 85 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 86 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 87 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 88 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 89 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 90 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 91 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 92 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 93 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 94 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 95 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 96 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 97 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 98 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 99 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 100 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 101 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 102 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 103 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 104 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 105 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 106 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 107 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 108 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 109 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 110 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 111 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 112 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 113 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 114 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 115 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 116 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 117 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 118 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 119 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 120 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 121 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 122 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 123 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 124 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 125 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 126 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 127 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 128 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 129 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 130 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 131 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 132 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 133 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 134 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 135 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 136 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 137 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 138 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 139 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 140 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 141 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 142 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 143 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 144 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 145 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 146 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 147 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 148 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 149 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 150 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 151 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 152 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 153 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 154 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 155 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 156 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 157 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 158 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 159 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 160 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 161 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 162 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 163 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 164 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 165 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 166 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 167 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 168 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 169 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 170 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 171 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 172 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 173 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 174 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 175 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 176 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 177 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 178 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 179 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 180 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 181 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 182 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 183 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 184 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 185 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 186 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 187 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 188 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 189 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 190 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 191 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 192 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 193 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 194 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 195 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 196 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 197 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 198 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 199 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 200 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 201 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 202 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 203 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 204 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 205 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 206 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 207 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 208 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 209 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 210 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 211 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 212 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 213 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 214 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 215 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 216 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 217 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 218 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 219 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 220 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 221 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 222 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 223 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 224 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 225 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 226 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 227 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
