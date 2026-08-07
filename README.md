# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-08-07.md)

*最后自动更新时间: 2026-08-07 20:17:44*
## 1. 马里奥遇帕累托

**原文标题**: Mario Meets Pareto

**原文链接**: [https://www.mayerowitz.io/blog/mario-meets-pareto](https://www.mayerowitz.io/blog/mario-meets-pareto)

Antoine Mayerowitz 的文章《马力欧邂逅帕累托》探讨了如何利用帕累托效率优化《马力欧卡丁车8豪华版》中的角色和载具部件选择。玩家选择车手、车身、轮胎和滑翔翼，每个部件都会影响速度、加速、操控等多种统计数据，从而产生数千种可能的组合。

挑战在于在这些统计数据之间进行权衡。经济学家维尔弗雷多·帕累托提出的解决方案有助于识别“高效”的选择。许多选项是“被支配的”，意味着存在另一个选项在所有相关统计数据上都优于或等于它（例如，库巴比猫咪桃花公主或奇诺比奥奇诺比姬更差）。“帕累托前沿”包含所有未被任何其他选项支配的“高效”选项。这一客观标准筛选掉了次优选择。

尽管帕累托前沿不会揭示单一的“最佳”配置——因为最终决定取决于玩家的个人偏好和游戏风格（他们的“效用函数”）——但它提供了一系列客观最优的权衡方案。这使得玩家可以尝试最有效的组合，而无需在明显低劣的组合上浪费时间。

文章将这一概念扩展到各种现实世界的多目标优化问题，例如平衡餐食的成本和质量、工作的薪水和成就感，或投资的风险和回报。当不同目标的精确权重未知或不确定时，帕累托效率的价值无法估量，它能引导决策者找到一系列最优的、非支配性选择。

---

## 2. AMD 收购 Taalas，旨在通过在硅片中刻蚀模型来提升推理性能。

**原文标题**: AMD acquires Taalas to boost inference performance by etching models in silicon

**原文链接**: [https://www.theregister.com/systems/2026/08/06/amd-acquires-ai-chip-startup-taalas-to-boost-inference-performance-by-etching-models-into-silicon/5284344](https://www.theregister.com/systems/2026/08/06/amd-acquires-ai-chip-startup-taalas-to-boost-inference-performance-by-etching-models-into-silicon/5284344)

AMD已收购AI芯片初创公司泰拉斯，旨在通过将AI模型权重直接蚀刻到硅中，创建模型专用集成电路（MSIC），从而显著提升推理性能。这种方法绕过了高带宽内存（HBM）进行权重存储，带来了显著的性能提升。

泰拉斯的HC1测试芯片采用台积电6纳米工艺制造，在发布时展示了以每秒16,960个令牌的惊人速度服务Meta的Llama 3.1 8B模型，比英伟达GPU快48倍。他们即将推出的HC2芯片旨在每个芯片支持200亿参数，只需50个加速器即可支持万亿参数模型，有望比现有GPU或LPU解决方案实现更高的效率。这些芯片包含一个用于权重的掩模ROM回忆结构，以及用于KV缓存和微调适配器的SRAM。

AMD打算将泰拉斯的技术与其基于Instinct的Helios机架整合，可能采用一种解耦架构，其中GPU处理提示，而泰拉斯加速器管理令牌生成。目前还在考虑为模型部署采用“滴答”节奏。

主要限制是模型不可变性；重大修改需要芯片“重制”。然而，泰拉斯声称这仅涉及修改两个金属层，比完全重新设计成本更低、耗时更少。这项技术可能最吸引那些对其模型选择充满信心的AI模型开发者和推理服务提供商，尤其是在蚀刻模型的成本据报道比训练前沿模型便宜100倍的情况下。它还有望通过降低每令牌成本和提升输出速度，通过扩展“测试时缩放”来提高模型精度。该交易预计将在第四季度完成，尚待监管部门批准。

---

## 3. 美国达成12亿美元交易，支付德国公司以叫停海上风电项目。

**原文标题**: US strikes $1.2B deal to pay German firm to halt offshore wind projects

**原文链接**: [https://www.bbc.com/news/articles/c1e1vg0gjl5o](https://www.bbc.com/news/articles/c1e1vg0gjl5o)

生成摘要时出错

---

## 4. 犯罪致富，植物学不济

**原文标题**: Crime Pays but Botany Doesn't

**原文链接**: [https://www.crimepaysbutbotanydoesnt.com/reading-list](https://www.crimepaysbutbotanydoesnt.com/reading-list)

《犯罪有钱赚，植物学没钱赚》一书为自学植物学提供了一份直接而热情的指南。作者鼓励初学者不要被复杂的术语吓倒，建议积极利用互联网查阅不熟悉的词汇和概念。

一个关键点是拉丁语术语的重要性，它被誉为一套通用的、精确的系统（由林奈创立），能够避免俗名造成的混淆。文章强调了正确的科学命名法——属名首字母大写，种加词小写，两者均斜体。分类学被描述为一种“非常酷”的方法，通过进化关系对植物进行分组，从而能够根据共同特征和进化历史来识别新物种。

对于严肃的学习，迈克尔·辛普森（Michael Simpson）的《植物系统学》（*Plant Systematics*）被推荐为一本开创性的教材，用于通过共有衍征理解植物进化、形态和识别。《雷文植物生物学》（*Raven's Biology of Plants*）则被建议用于学习基础植物生物学、进化概念和引人入胜的例子。

考虑到教材的高昂费用，作者提倡使用www.libgen.is和www.sci-hub.se等资源，并建议在经济实惠的电子阅读器上阅读PDF文件。此外，还提供了一份全面的额外文本列表，涵盖从分子系统发育学和植物进化到生态学和专业区域研究等多个不同领域，强调即使是针对特定地理区域的书籍也能提供广泛适用的生态学 M。

---

## 5. 新墨西哥州法院判决Meta因损害儿童心理健康赔偿5.67亿美元。

**原文标题**: New Mexico court orders Meta to pay $567m over harms to children’s mental health

**原文链接**: [https://www.theguardian.com/technology/2026/aug/06/new-mexico-court-meta](https://www.theguardian.com/technology/2026/aug/06/new-mexico-court-meta)

新墨西哥州一家法院已命令Meta额外支付5.67亿美元，用于设立一个基金，以解决其平台对儿童造成的负面心理健康影响，使Meta在该州的总负债达到9.42亿美元。此前，在今年3月的一项里程碑式审判中，陪审团裁定Meta故意损害儿童心理健康并隐瞒儿童性剥削行为，最初判处其3.75亿美元罚款。新增加的资金将主要用于新墨西哥州青少年在五年内的治疗服务（4.2亿美元）、宣传、预防和筛查工作。

除了金钱判决外，法院还强制要求Meta做出多项改变。Meta必须改善其在新墨西哥州的年龄验证工具，包括使用AI预测用户年龄，并在两年内开发专门的“13岁以下用户预测模型”。它必须要求疑似未成年用户提供年龄证明，在验证完成前将其视为13岁以下或18岁以下用户，并与学校合作建立举报门户。其他命令还包括创建关于保护功能的信息屏幕、开展教育宣传活动，以及删除从13岁以下用户收集的个人数据。

新墨西哥州总检察长劳尔·托雷斯（Raúl Torrez）称赞这一裁决是儿童的胜利。Meta表示不同意该裁决，计划提起上诉，并对其安全工作充满信心。此案是Meta首次因其平台造成的损害被判承担责任，也是美国其他州日益增多的诉讼浪潮的一部分，这表明了更广泛地规范社交媒体公司对青少年心理健康影响的努力。

---

## 6. 只余余味

**原文标题**: Taste Is All That's Left

**原文链接**: [https://notashelf.dev/posts/taste-is-all-thats-left](https://notashelf.dev/posts/taste-is-all-thats-left)

文章《品味是唯一所剩》指出，人工智能和大型语言模型的出现，从根本上重塑了创意和技术工作，尤其是软件开发。历史上，主要的挑战在于*让*事物存在，生产的“摩擦”（编码、调试）充当了质量的过滤器和学习的熔炉。这种努力培养了“品味”——一种通过经验和错误发展起来的、即时而无言的质量判断。

人工智能现在已基本消除了这种摩擦，缩短了“从构思到成品”的距离。虽然这使得快速生成“看似合理”的产出成为可能，但却剥夺了培养品味所必需的学徒式学习过程。市场看重速度和可量化的产出，却未能认识到辨别真正品质这种缓慢、无法量化的行为。这导致了大量“还行”但最终“平庸”的产出，作者将其比作“AI糟粕”。

作者认为，尽管现在产出丰富，“品味”仍然是人类独有且稀缺的技能。它是一种对仅仅“看似合理”的解决方案说“不，重来”的能力，努力追求“正确”之物。这种通过经验培养的鉴别力，如今是至高无上的技艺。文章最后倡导，在这个充满无限生成内容的世界里，拥抱这种无法衡量、无法自动化的判断行为——即“删除”和批判性精炼——将其视为人类关怀和技能的最后证据。一篇事后补充回应了读者对文章自身写作风格与AI产出相似的担忧，作者否认文章由大型语言模型创作。

---

## 7. Qwen3.8 Max 现已被智能体指数评为最佳综合模型

**原文标题**: Qwen3.8 Max now ranked as the best overall model by agentic index

**原文链接**: [https://artificialanalysis.ai/?intelligence=agentic-index](https://artificialanalysis.ai/?intelligence=agentic-index)

人工分析公司宣布，其智能体指数已将通义千问3.8 Max评为最佳综合模型。该指数是衡量智能体工作流程（如工具使用、规划、自主性和复杂问题解决）性能的关键指标。此次更新伴随着智能指数v4.1.1的推出，旨在帮助用户驾驭人工智能格局，并根据智能、速度和成本效益来选择模型。

v4.1.1智能指数整合了九项评估，包括GDPval-AA v2、𝜏³-银行（现v1.0.1）、Terminal-Bench v2.1、SciCode、人类的最终考试、GPQA Diamond、CritPt、AA-全知和AA-LCR。其中几项评估（包括HLE、AA-LCR和AA-全知）的评分器已升级为GPT-5.6 Luna。

人工分析公司还推出了端点准确性指数，以评估由提供商提供的模型质量。该平台提供详细指标，涵盖每秒输出token数、每任务加权平均成本，以及各种专业基准，如编码智能体指数、图像与视频、语音，以及行业特定能力指数（例如金融、法律、工程）。针对每任务成本的方法学也进行了近期更新。总体目标是提供个性化的模型推荐。

---

## 8. GitHub Actions and Pages are experiencing degraded availability

**原文标题**: GitHub Actions and Pages are experiencing degraded availability

**原文链接**: [https://www.githubstatus.com/incidents/qcvjkzcs7j74](https://www.githubstatus.com/incidents/qcvjkzcs7j74)

GitHub experienced an incident affecting Actions and Pages, starting around 15:22 UTC on August 6, 2026, and resolving by 02:04 UTC on August 7, 2026.

The disruption caused degraded availability for GitHub Actions and Pages, leading to workflow failures, significant delays in job processing, and queued jobs timing out. The incident also impacted Actions API requests, webhook deliveries (which were throttled), Copilot code review, Copilot coding agent, and migrations using GitHub Enterprise Importer (which were paused as a precaution). Both GitHub-hosted and self-hosted runners were affected, with issues such as runners being assigned invalid jobs and some becoming stuck.

GitHub engineers actively worked on the issue, deploying multiple fixes, clearing system-wide queues, and incrementally restoring throughput for affected services. By early August 7, most services, including Actions workflows and GitHub Pages, showed signs of recovery, with engineers monitoring for sustained stability.

Upon resolution, GitHub advised users that some Actions Runner Controller (ARC) runner pods might remain stuck, requiring manual deletion or redeployment. Additionally, certain workflow-triggering events (like pushes and pull requests) that occurred during the incident were not automatically replayed, necessitating users to repeat the triggering action. Future releases of Actions Runner and Controller are planned to include automatic recovery mechanisms for these issues. A detailed root cause analysis will be shared when available.

---

## 9. I'm switching my phone from Android to Linux

**原文标题**: I'm switching my phone from Android to Linux

**原文链接**: [https://runarcn.no/android-to-linux/](https://runarcn.no/android-to-linux/)

生成摘要时出错

---

## 10. The title cards in Blade Runner are amazing

**原文标题**: The title cards in Blade Runner are amazing

**原文链接**: [https://randsinrepose.com/archives/blade-runner-title-cards/](https://randsinrepose.com/archives/blade-runner-title-cards/)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 2 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 3 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 4 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 5 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 6 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 7 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 8 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 9 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 10 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 11 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 12 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 13 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 14 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 15 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 16 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 17 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 18 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 19 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 20 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 21 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 22 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 23 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 24 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 25 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 26 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 27 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 28 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 29 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 30 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 31 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 32 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 33 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 34 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 35 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 36 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 37 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 38 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 39 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 40 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 41 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 42 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 43 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 44 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 45 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 46 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 47 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 48 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 49 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 50 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 51 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 52 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 53 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 54 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 55 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 56 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 57 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 58 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 59 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 60 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 61 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 62 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 63 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 64 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 65 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 66 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 67 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 68 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 69 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 70 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 71 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 72 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 73 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 74 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 75 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 76 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 77 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 78 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 79 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 80 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 81 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 82 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 83 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 84 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 85 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 86 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 87 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 88 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 89 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 90 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 91 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 92 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 93 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 94 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 95 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 96 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 97 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 98 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 99 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 100 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 101 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 102 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 103 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 104 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 105 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 106 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 107 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 108 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 109 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 110 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 111 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 112 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 113 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 114 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 115 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 116 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 117 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 118 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 119 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 120 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 121 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 122 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 123 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 124 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 125 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 126 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 127 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 128 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 129 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 130 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 131 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 132 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 133 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 134 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 135 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 136 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 137 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 138 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 139 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 140 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 141 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 142 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 143 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 144 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 145 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 146 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 147 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 148 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 149 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 150 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 151 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 152 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 153 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 154 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 155 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 156 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 157 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 158 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 159 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 160 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 161 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 162 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 163 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 164 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 165 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 166 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 167 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 168 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 169 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 170 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 171 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 172 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 173 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 174 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 175 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 176 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 177 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 178 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 179 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 180 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 181 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 182 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 183 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 184 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 185 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 186 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 187 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 188 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 189 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 190 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 191 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 192 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 193 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 194 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 195 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 196 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 197 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 198 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 199 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 200 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 201 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 202 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 203 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 204 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 205 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 206 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 207 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 208 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 209 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 210 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 211 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 212 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 213 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 214 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 215 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 216 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 217 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 218 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 219 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 220 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 221 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 222 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 223 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 224 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 225 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 226 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 227 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 228 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 229 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 230 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 231 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 232 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 233 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 234 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 235 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 236 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 237 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 238 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 239 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 240 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 241 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 242 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 243 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 244 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 245 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 246 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 247 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 248 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 249 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 250 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 251 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 252 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 253 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 254 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 255 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 256 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 257 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 258 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 259 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 260 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 261 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 262 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 263 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 264 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 265 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 266 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 267 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 268 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
| 269 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 270 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 271 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 272 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
