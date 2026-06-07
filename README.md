# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-06-07.md)

*最后自动更新时间: 2026-06-07 20:42:12*
## 1. 语义：代码理解的新原语——并非LSP，而是基于Git构建的实体

**原文标题**: Sem: New primitive for code understanding – not LSPs, but entities on top of Git

**原文链接**: [https://ataraxy-labs.github.io/sem/](https://ataraxy-labs.github.io/sem/)

Sem是一个新的命令行工具，旨在为代码变更带来语义理解，超越传统的基于行的`git diff`。它直接在Git仓库上运行，专注于函数、类和方法等“实体”。

主要功能包括：
*   **`sem diff`**：显示实体级别的变更（新增、修改、删除的函数），具备重命名检测和结构哈希功能，相比原始的行级差异提高了清晰度。
*   **`sem blame`**：识别最后一次修改每个特定实体的提交。
*   **`sem impact`**：生成跨文件依赖图，揭示哪些实体依赖于给定函数以及哪些测试受到影响。
*   **`sem log`**：提供单个实体的Git历史记录，显示所有修改过它的提交。
*   **`sem entities`**：列出路径中所有识别的实体（函数、类等）及其行范围。
*   **`sem context`**：为AI创建带有令牌预算的上下文窗口，包括目标实体、其依赖项和被依赖项，旨在适应LLM提示。

`sem` 处理其输出时，能显著提高AI代理的准确性（2.3倍）。它支持26种编程语言和5种数据格式，无需配置或插件，可在任何Git仓库中运行。安装简单，并且可以配置为全局替换`git diff`，为代码演进和影响提供了强大、语义化的视角。

---

## 2. 代币经济学：量化代币在智能体软件工程中的应用

**原文标题**: Tokenomics: Quantifying Where Tokens Are Used in Agentic Software Engineering

**原文链接**: [https://arxiv.org/abs/2601.14470](https://arxiv.org/abs/2601.14470)

本文题为《令牌经济学：量化智能体软件工程中令牌的使用情况》，探讨了自动化软件工程中基于大型语言模型的多智能体 (LLM-MA) 系统关键但却鲜为人知的运行效率和资源消耗问题。不可预测的成本和环境影响阻碍了这些系统在代码生成和测试等任务中的实际应用。

Mohamad Salim及其合著者研究了软件开发生命周期 (SDLC) 中的令牌消耗模式。他们分析了由ChatDev框架使用GPT-5推理模型执行的30个软件开发任务的执行轨迹。他们的方法将ChatDev的内部阶段映射到标准化的SDLC阶段——设计、编码、代码补全、代码审查、测试和文档——以量化和比较这些阶段中输入、输出和推理令牌的分布。

初步研究结果揭示了显著的令牌使用模式。迭代的代码审查阶段占令牌消耗的大部分，平均为59.4%。此外，输入令牌始终占据消耗的最大份额，平均为53.9%。这些结果表明，智能体软件工程中的主要成本并非源于初始代码生成，而是来自自动化优化和验证过程，突出了智能体协作中潜在的低效率。作者们提出，他们的新颖方法可以帮助从业者预测开销、优化工作流程，并指导未来研究开发更具令牌效率的智能体协作协议。

---

## 3. 阈限主义如何成为我们这个时代的标志性美学

**原文标题**: How Liminalism Became the Defining Aesthetic of Our Time

**原文链接**: [https://hyperallergic.com/how-liminalism-became-the-defining-aesthetic-of-our-time/](https://hyperallergic.com/how-liminalism-became-the-defining-aesthetic-of-our-time/)

阈限主义（Liminalism）是一种流行的网络美学，其核心是探索那些既诡异、令人不安又似曾相识的“介于两者之间”的空间，这些空间通常空无一人。这项自下而上、由大众策展的运动，以废弃商场或空荡走廊的照片为例，唤起一种忧郁的不适感——一种不安与怀旧的混合体。

其近期兴起源于2019年“后室”（Backrooms）恐怖故事和Javier 2021年发布的关于废弃地点的TikTok视频等网络现象，COVID-19封锁和数字隔离更是推波助澜。一个显著特征是人的缺席，培养出一种个人化的、近乎末世般的孤独感。阈限主义作为一种民主的数字现成品艺术而存在，明确禁止人工智能内容，并标志着艺术话语脱离传统机构的趋势。

历史上，阈限主义通过空间迷失感和空旷的风景，与乔治·德·基里科（Giorgio de Chirico）和雷内·马格里特（René Magritte）等超现实主义者相关联。更直接地说，它追随了格兰特·伍德（Grant Wood）等美国战后艺术家，最重要的是爱德华·霍珀（Edward Hopper），他的作品，如《周日清晨》（Early Sunday Morning）和《空屋中的阳光》（Sun in an Empty Room），有力地描绘了人类的缺席和异化。

这种美学深刻地反映了我们这个时代，体现了“制图焦虑”和“空间混乱”。它诠释了无地性、匿名性、异化和焦虑，描绘了一个“非场所”（no-places）暗示着模拟的超现实当下。它通过匿名论坛和社交媒体进行的数字化传播，对其情感影响至关重要，作为对反乌托邦晚期资本主义和我们原子化存在的“内在死亡”的视觉评论。

---

## 4. 英格兰和威尔士警方被告知暂停在法庭陈述中使用人工智能。

**原文标题**: Police in England and Wales told to halt AI use in court statements

**原文链接**: [https://www.ft.com/content/229e5949-3ebc-4151-8a86-a01b5e259241](https://www.ft.com/content/229e5949-3ebc-4151-8a86-a01b5e259241)

所提供的“文章内容”完全是付费墙，导致文章全文无法访问。

因此，无法提供一份详细阐述实际文章中提及的原因、影响或具体指令的全面概述。

仅根据标题，关键信息是：**英格兰和威尔士的警方已被指示停止在准备法庭陈述时使用人工智能 (AI)。**

---

## 5. 《C++: The Language》的封底引发了封面无法解答的疑问

**原文标题**: The back cover of C++: The Language raises questions not answered by front cover

**原文链接**: [https://devblogs.microsoft.com/oldnewthing/20260605-01/?p=112391](https://devblogs.microsoft.com/oldnewthing/20260605-01/?p=112391)

文章批评了《C++：编程语言》一书的封底宣传语，认为其内容空泛且缺乏特异性。像“其中包含的主题至关重要”和“必将为学生提供令人难以置信的见解”这样的表述过于模糊，几乎可以用来描述任何一本教科书，这促使作者将其比作学生未曾阅读就写的读书报告。

为支持这一论点，作者在其他几本不相关的书籍（包括《铸造手册》、《食品工业：工艺与技术》、《营养与代谢：过程与技术》以及《材料科学与工程》）的宣传语中发现了几乎相同的语句。包括这本C++书籍在内的所有这些出版物的共同点是，它们都由Larson and Keller出版。文章总结道，该出版商可能为其所有书籍使用一个通用的宣传语模板，而非为每本书量身定制独特的描述，这与此前对该C++书籍封面显示JavaScript代码而非C++代码的批评如出一辙。

---

## 6. 克隆马的天下：它们如何称霸马球

**原文标题**: Field of clones: How horse replicas came to dominate polo

**原文链接**: [https://knowablemagazine.org/content/article/technology/2026/cloned-polo-horses](https://knowablemagazine.org/content/article/technology/2026/cloned-polo-horses)

文章《克隆领域：克隆马匹如何主宰马球运动》描述了马匹克隆如何成为一个成熟但备受伦理争议的产业，尤其是在阿根廷。马球传奇人物Adolfo Cambiaso于2006年开创了这一趋势，他在他的母马Aiken Cura受伤后，意识到保存优秀基因的潜力。他的La Dolfina队现在使用超过150匹克隆马，建立了前所未有的统治地位。

克隆过程，即体细胞核移植（SCNT），涉及将体细胞核转移到去核卵细胞中。尽管技术上具有挑战性且昂贵，但诸如使用干细胞和改进卵母细胞来源等进步，已提高了成功率。然而，其效率仍然低下，只有3-10%的移植胚胎能存活出生，且各个阶段都有大量损失，这导致了高昂的成本。克隆马虽然共享核DNA，但在线粒体DNA和表观遗传模式上有所不同，这可能导致健康问题。

阿根廷生物技术专家Gabriel Vichera的公司Kheiron Biotech在标准化这一过程方面发挥了关键作用，已生产了一千匹克隆马。他们甚至通过使用CRISPR-Cas9基因编辑克隆马驹，实现了全球首次，预示着未来基因组修饰将超越单纯的复制。阿根廷现在在马匹克隆领域处于世界领先地位。

尽管取得了技术上的成功，但在动物福利、公平竞争以及体育运动中的基因操纵方面，伦理困境依然存在。尽管如此，克隆技术继续推动着马球运动中对获胜基因的追求，代表着顶级竞争者的一项奢侈产业。

---

## 7. 你可以跑

**原文标题**: You Can Run

**原文链接**: [https://magazine.atavist.com/2026/mccann-cocaine-fugitives](https://magazine.atavist.com/2026/mccann-cocaine-fugitives)

《你能逃脱》（You Can Run）讲述了姐妹艾琳和梅雷迪思·麦肯的故事，她们的田园诗般的童年被父母莉亚和约翰打破，父母最初声称是由于税务局（IRS）的麻烦，迫使她们过上逃亡生活。多年后，她们才发现父亲犯罪历史的全部真相。

文章开头，已是律师的成年艾琳匆匆赶往母亲家。莉亚多年来一直保持沉默，却突然透露她已将两箱与她们过去相关的关键政府文件当作垃圾扔掉了，艾琳心急如焚地想要找回它们。

叙事闪回到1984年，当时13岁的艾琳和10岁的梅雷迪思在匹兹堡的福克斯教堂过着优渥的生活。她们的父亲约翰·H·麦肯三世魅力十足却控制欲强；母亲莉亚则优雅得体。在与几名西装男士偶遇后，莉亚迅速带走了姐妹俩，最终在安大略省温莎透露，她们正在放弃自己的生活和身份以躲避政府。

在一年半的时间里，这家人用着各种化名，辗转于马略卡岛、伦敦和不列颠哥伦比亚等多个地方。姐妹俩编造着背景故事，不断适应着新生活，却从未真正了解她们流亡的真实原因。

文章详细描述了约翰的过往：他出身工人阶级，却自我改造，谎报教育和成就，过着奢华的生活。他的职业生涯包括担任市长和法官（最终以丑闻告终），从一家煤炭企业中掏空资金，以及涉嫌与有组织犯罪勾结以获取回扣。随后，他开始推销“可疑的避税方案”，这暗示了导致她们失踪的更大规模犯罪活动。莉亚虽然知道他的欺骗行为，但最初为了他提供的奢华生活而接受了这一切。艾琳希望这些箱子最终能揭示她们破碎过去背后的全部真相。

---

## 8. Benchmarks in Leipzig

**原文标题**: Benchmarks in Leipzig

**原文链接**: [https://arxiv.org/abs/2606.05818](https://arxiv.org/abs/2606.05818)

The paper "Benchmarks in Leipzig," authored by Andrei Balakin and 47 collaborators, details a project where 49 mathematicians compiled a unique dataset of 100 research-level mathematics questions with known answers. This extensive effort took place between April 1 and May 15, 2026, largely during a 3-day workshop with 35 participants at the Max Planck Institute for Mathematics in the Sciences in Leipzig, Germany.

The primary objective was to evaluate the mathematical reasoning capabilities of state-of-the-art Large Language Models (LLMs) using this new benchmark. The evaluation proceeded in three stages:
1.  A single attempt by five LLMs left 41 questions completely unsolved.
2.  A subsequent stage involved 20 runs per model with three of the initial LLMs, reducing the unsolved count to 16.
3.  Finally, two "heavy-thinking" models made a 3-run attempt, successfully solving all but 2 of the remaining questions.

This significant progress, from 41 initially unsolved to only 2 by the end, compellingly demonstrates that the mathematical reasoning capabilities of LLMs are becoming remarkably impressive. The paper includes detailed benchmark statistics and the full set of 100 questions.

---

## 9. US House lawmakers release draft bill to prohibit state AI rules

**原文标题**: US House lawmakers release draft bill to prohibit state AI rules

**原文链接**: [https://www.reuters.com/business/us-house-lawmakers-release-draft-bill-regulate-ai-2026-06-04/](https://www.reuters.com/business/us-house-lawmakers-release-draft-bill-regulate-ai-2026-06-04/)

生成摘要时出错

---

## 10. The OnlyFans Economy of American AI

**原文标题**: The OnlyFans Economy of American AI

**原文链接**: [https://leoveanu.com/2026-06-06-qwen3.7max/](https://leoveanu.com/2026-06-06-qwen3.7max/)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 2 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 3 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 4 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 5 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 6 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 7 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 8 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 9 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 10 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 11 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 12 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 13 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 14 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 15 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 16 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 17 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 18 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 19 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 20 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 21 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 22 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 23 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 24 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 25 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 26 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 27 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 28 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 29 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 30 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 31 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 32 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 33 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 34 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 35 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 36 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 37 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 38 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 39 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 40 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 41 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 42 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 43 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 44 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 45 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 46 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 47 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 48 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 49 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 50 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 51 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 52 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 53 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 54 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 55 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 56 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 57 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 58 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 59 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 60 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 61 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 62 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 63 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 64 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 65 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 66 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 67 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 68 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 69 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 70 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 71 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 72 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 73 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 74 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 75 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 76 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 77 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 78 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 79 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 80 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 81 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 82 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 83 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 84 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 85 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 86 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 87 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 88 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 89 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 90 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 91 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 92 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 93 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 94 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 95 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 96 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 97 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 98 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 99 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 100 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 101 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 102 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 103 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 104 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 105 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 106 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 107 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 108 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 109 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 110 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 111 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 112 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 113 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 114 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 115 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 116 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 117 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 118 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 119 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 120 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 121 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 122 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 123 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 124 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 125 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 126 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 127 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 128 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 129 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 130 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 131 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 132 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 133 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 134 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 135 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 136 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 137 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 138 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 139 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 140 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 141 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 142 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 143 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 144 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 145 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 146 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 147 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 148 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 149 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 150 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 151 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 152 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 153 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 154 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 155 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 156 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 157 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 158 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 159 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 160 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 161 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 162 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 163 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 164 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 165 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 166 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 167 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 168 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 169 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 170 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 171 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 172 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 173 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 174 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 175 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 176 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 177 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 178 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 179 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 180 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 181 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 182 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 183 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 184 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 185 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 186 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 187 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 188 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 189 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 190 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 191 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 192 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 193 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 194 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 195 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 196 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 197 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 198 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 199 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 200 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 201 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 202 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 203 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 204 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 205 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 206 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 207 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 208 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 209 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 210 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 211 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 212 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
