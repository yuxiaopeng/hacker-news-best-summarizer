# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-07-06.md)

*最后自动更新时间: 2026-07-06 21:05:49*
## 1. 每百万token的价格毫无意义

**原文标题**: Price per 1M tokens is meaningless

**原文链接**: [https://janilowski.pl/en/blog/2026/price-per-m-tokens/](https://janilowski.pl/en/blog/2026/price-per-m-tokens/)

文章认为，仅以“每百万token $X”来比较AI模型的成本毫无意义且具有误导性，因为它未能反映真实的支出。

这一主张主要基于两个原因：
1.  **不可比较的分词器**：不同的AI实验室，甚至同一供应商内部的不同模型，都采用专有的分词器。这些分词器将相同的文本分割成不同的token数量（例如，GPT-4o对一段文本使用160个token，而GPT-4使用200个）。对分词器的调整，例如Anthropic最近的修改导致相同文本的token数量增加30%，这可能等同于隐性涨价。
2.  **token效率的巨大差异**：除了原始的token价格之外，每个token所产生的“价值”或“成果”也大相径庭。在复杂任务中，很大一部分token消耗用于“思考”或“思维链”过程，而这些消耗与输出token以相同的费率计费。这种隐性消耗可能是主要的成本驱动因素，并且在不同模型之间差异巨大。

一项包含多个模型（例如Claude、GPT、GLM、DeepSeek）对比表格的实证分析证明了这一点。尽管GPT-5.5名义上每百万token比Claude Opus 4.8更昂贵，但它完成基准任务的成本几乎只有后者的一半，这表明其token效率更高。相反，GLM-5.2每token便宜得多，但其每任务成本并没有成比例地降低。尽管DeepSeek V4 Pro的智能得分较低，但其每任务成本极低，使其成为成本效率方面的一个显著例外。

文章总结道，“每百万token $X”并非一个有意义的成本指标。为了做出明智的模型选择决策，并避免为较差的性能支付更高的价格，用户必须关注“实际每任务成本”。

---

## 2. OfficeCLI：供AI代理读写Microsoft Office文件的办公套件

**原文标题**: OfficeCLI: Office suite for AI agents to read and edit Microsoft Office files

**原文链接**: [https://github.com/iOfficeAI/OfficeCLI](https://github.com/iOfficeAI/OfficeCLI)

OfficeCLI 被引入，成为全球首个也是最佳的专为AI代理设计的Office套件，使它们能够通过一行代码完全控制Microsoft Word、Excel和PowerPoint文件。它是一个开源工具，以自包含的单一二进制文件形式分发，无需安装Office或任何外部依赖，并可在所有平台上运行。

其核心创新是内置的高保真HTML渲染引擎，它能够将.docx、.xlsx和.pptx文件渲染成HTML或PNG，使AI代理能够“看到”文档。这一功能有助于实现“渲染→查看→修正”的循环，这对于在无头环境中提供视觉反馈和迭代生成文档至关重要。

OfficeCLI 极大地简化了Office自动化，将传统代码中数十行的工作量替换为单个CLI命令，用于创建、读取、修改和格式化文档等任务。它支持所有三种Office格式的全面功能，包括Word的完全国际化、Excel的公式和数据透视表引擎（自动评估350多个函数和原生数据透视表），以及PowerPoint的丰富形状/图表操作等高级功能。

关键原语包括用于数据填充的模板`merge`函数；一个`dump`命令，用于将现有文档或子树序列化为可重放的JSON，以便学习和复制；以及用于高效多步工作流的`resident`和`batch`模式。AI代理的安装只需一个简单的`curl`命令，而人类用户可以使用AionUi GUI或CLI，开发者可以快速设置实时预览。该工具以包含嵌入式.NET运行时的单一二进制文件形式发布，确保了轻松部署和自动更新。

---

## 3. 牛津大学比阿兹特克帝国历史更悠久，以及其他历史事实 (2013)

**原文标题**: University of Oxford Is Older Than the Aztec Empire and Other Facts of History (2013)

**原文链接**: [https://www.smithsonianmag.com/smart-news/university-oxford-older-than-aztec-empire-other-facts-will-change-your-perspective-history-1529607/](https://www.smithsonianmag.com/smart-news/university-oxford-older-than-aztec-empire-other-facts-will-change-your-perspective-history-1529607/)

牛津大学比阿兹特克帝国更古老，以及其他历史事实

这篇文章，“牛津大学比阿兹特克帝国更古老，以及其他历史事实”，挑战了人们对历史时间线的普遍误解。文章指出，牛津大学的教学活动始于大约1096年，比阿兹特克首都特诺奇蒂特兰（Tenochtitlán）于1325年建立早了229年。阿兹特克帝国从1325年持续到1521年，存在时间不足一个世纪，这意味着白宫（1792年奠基）矗立的时间比阿兹特克人统治其首都的时间还要长。

尽管牛津大学是英语世界中最古老的大学，但文章指出，卡鲁因大学（University of al-Qarawiyyin，建于859年）是世界上持续运作时间最长的高等教育机构，而博洛尼亚大学（University of Bologna，建于1088年）则是西方世界同类大学中最古老的。

这篇文章的重点是，我们对历史的理解常常是“扭曲的”，时间线被歪曲和压缩。为此，文章解释说，埃及艳后克利奥帕特拉统治古埃及时，正值其长达3000年历史的末期，她所处的时代更接近2024年，而不是金字塔建造的时代。文章还指出，安妮·弗兰克和马丁·路德·金等看似迥异的人物都出生于同一年（1929年），而阿提拉和先知穆罕默德等常被一同提及的人物却相隔数百年。文章总结说，将历史事件置于语境中理解对于更清晰地认识过去至关重要。

---

## 4. 鸡蛋摄入与阿尔茨海默病呈负相关

**原文标题**: Egg consumption inversely correlated with Alzheimer's

**原文链接**: [https://pubmed.ncbi.nlm.nih.gov/42002260/](https://pubmed.ncbi.nlm.nih.gov/42002260/)

发表在《食品与功能》杂志上的一项系统评价和荟萃分析，调查了鸡蛋摄入与阿尔茨海默病（AD）风险之间的关联。该研究分析了来自12项观察性研究（包括7项病例对照研究和5项队列研究）的数据，共涉及26,122名参与者。

汇总结果显示，鸡蛋摄入与AD风险之间存在显著的负相关，表明摄入鸡蛋的个体患AD的风险较低（汇总RR = 0.81；95% CI：0.70-0.93）。相比病例对照研究，这种负相关在队列研究中更为明显（RR = 0.75）。

基于摄入频率的进一步分析显示，适度鸡蛋摄入（定义为每周3-6个鸡蛋）与AD风险显著降低相关（RR = 0.76）。然而，大量鸡蛋摄入（每周7个或更多鸡蛋）未显示与AD风险有统计学上的显著关联（RR = 0.96）。

该研究结果具有稳健性，荟萃回归和敏感性分析证实，这种负相关不受发表年份、研究设计或地理区域等因素的影响。作者认为，将适量鸡蛋纳入饮食可能是降低AD风险的一种潜在策略，尽管他们强调需要进一步的前瞻性研究来证实这些发现并阐明其潜在的生物学机制。

---

## 5. HN 展示：普尔佩——网络清理模型

**原文标题**: Show HN: Pulpie – Models for Cleaning the Web

**原文链接**: [https://usefeyn.com/blog/pulpie-pareto-optimal-models-for-cleaning-the-web/](https://usefeyn.com/blog/pulpie-pareto-optimal-models-for-cleaning-the-web/)

由Feyn Labs开发的Pulpie推出了一系列帕累托最优模型，用于从HTML页面中提取主要内容，以二十分之一的成本和显著更高的速度提供接近最先进（SOTA）的质量。这一创新解决了对干净网络数据的关键需求，因为样板内容通常占HTML页面的70%，阻碍了语言模型的预训练和推理质量。

Pulpie高效的关键在于其编码器架构，该架构在一个前向传播中将每个HTML块标记为内容或样板。这种设计使其受计算限制而非内存带宽限制，这与Dripper等基于解码器的提取器不同。

最小的模型`pulpie-orange-small`（2.1亿参数）在WebMainBench上获得了0.862的ROUGE-5 F1分数，与Dripper的0.864 F1分数非常接近，尽管其大小仅为Dripper（6亿参数）的三分之一。性能基准令人瞩目：在NVIDIA L4 GPU上，`pulpie-orange-small`每秒处理13.7页，比Dripper每秒0.68页的速度快20倍。这意味着使用Pulpie清理十亿页只需7,900美元，而使用Dripper则需159,000美元。

Pulpie的训练涉及创建一个新颖的14,959页块级标记数据集，使用DeepSeek V3.2和Dripper进行交叉验证。然后，一个21亿参数的教师模型（EuroBERT）被微调并蒸馏，成为更小、更高效的`orange-small`和`orange-base`模型。

这些模型已在Hugging Face上开源，其中`pulpie-orange-small`因其在质量、速度和成本之间的最佳平衡而被推荐，使大规模高质量网络提取——此前不可能实现——现在可用于LLM开发。

---

## 6. 千字：征文比赛

**原文标题**: 1k Words: A Writing Contest

**原文链接**: [https://writingclub.world/1picture1000words](https://writingclub.world/1picture1000words)

“千字：写作比赛”挑战参赛者，要求他们以一张特定但尚未公开的图片为灵感，撰写恰好1000字的作品。比赛不限文体，无论是创意非虚构、科幻小说、一个笑话，还是其他任何形式的作品，只要与提供的图片相关即可。

提交截止日期是2026年8月31日。作品被评为“最佳”的作者将赢得1000美元的奖金。

本次比赛由Jordan和Carter的项目Quarter Mile组织，他们此前曾举办过“DEAR ALIENS”和“The Next Tiramisu”等比赛。有任何疑问者可通过电子邮件联系他们。文中还提到，对于那些不参赛但希望关注结果的人，也提供了相关选项。

---

## 7. 欧足联抨击国际足联“前所未有、毫无道理”的巴洛贡决定

**原文标题**: UEFA slams FIFA's 'unprecedented, unjustifiable' Balogun decision

**原文链接**: [https://www.reuters.com/sports/soccer/uefa-slams-fifas-unprecedented-incomprehensible-unjustifiable-balogun-decision-2026-07-06/](https://www.reuters.com/sports/soccer/uefa-slams-fifas-unprecedented-incomprehensible-unjustifiable-balogun-decision-2026-07-06/)

生成摘要时出错

---

## 8. sqlite-utils 4.0rc2, mostly written by Claude Fable (for about $149.25)

**原文标题**: sqlite-utils 4.0rc2, mostly written by Claude Fable (for about $149.25)

**原文链接**: [https://simonwillison.net/2026/Jul/5/sqlite-utils-fable/](https://simonwillison.net/2026/Jul/5/sqlite-utils-fable/)

生成摘要时出错

---

## 9. Linux on the Atari Jaguar. No, really.

**原文标题**: Linux on the Atari Jaguar. No, really.

**原文链接**: [https://cakehonolulu.github.io/linux-for-jaguar/](https://cakehonolulu.github.io/linux-for-jaguar/)

生成摘要时出错

---

## 10. Android is almost dead – OSnews

**原文标题**: Android is almost dead – OSnews

**原文链接**: [https://www.osnews.com/story/145415/android-is-almost-dead/](https://www.osnews.com/story/145415/android-is-almost-dead/)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 2 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 3 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 4 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 5 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 6 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 7 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 8 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 9 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 10 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 11 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 12 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 13 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 14 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 15 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 16 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 17 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 18 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 19 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 20 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 21 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 22 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 23 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 24 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 25 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 26 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 27 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 28 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 29 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 30 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 31 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 32 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 33 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 34 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 35 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 36 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 37 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 38 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 39 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 40 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 41 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 42 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 43 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 44 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 45 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 46 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 47 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 48 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 49 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 50 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 51 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 52 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 53 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 54 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 55 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 56 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 57 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 58 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 59 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 60 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 61 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 62 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 63 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 64 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 65 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 66 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 67 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 68 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 69 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 70 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 71 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 72 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 73 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 74 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 75 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 76 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 77 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 78 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 79 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 80 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 81 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 82 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 83 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 84 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 85 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 86 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 87 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 88 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 89 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 90 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 91 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 92 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 93 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 94 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 95 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 96 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 97 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 98 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 99 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 100 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 101 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 102 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 103 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 104 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 105 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 106 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 107 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 108 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 109 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 110 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 111 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 112 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 113 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 114 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 115 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 116 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 117 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 118 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 119 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 120 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 121 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 122 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 123 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 124 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 125 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 126 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 127 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 128 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 129 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 130 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 131 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 132 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 133 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 134 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 135 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 136 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 137 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 138 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 139 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 140 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 141 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 142 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 143 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 144 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 145 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 146 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 147 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 148 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 149 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 150 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 151 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 152 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 153 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 154 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 155 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 156 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 157 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 158 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 159 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 160 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 161 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 162 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 163 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 164 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 165 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 166 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 167 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 168 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 169 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 170 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 171 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 172 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 173 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 174 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 175 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 176 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 177 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 178 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 179 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 180 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 181 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 182 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 183 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 184 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 185 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 186 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 187 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 188 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 189 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 190 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 191 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 192 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 193 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 194 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 195 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 196 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 197 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 198 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 199 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 200 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 201 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 202 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 203 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 204 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 205 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 206 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 207 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 208 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 209 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 210 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 211 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 212 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 213 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 214 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 215 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 216 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 217 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 218 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 219 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 220 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 221 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 222 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 223 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 224 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 225 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 226 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 227 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 228 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 229 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 230 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 231 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 232 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 233 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 234 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 235 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 236 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 237 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 238 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 239 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 240 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 241 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
