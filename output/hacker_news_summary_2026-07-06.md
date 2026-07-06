# Hacker News 热门文章摘要 (2026-07-06)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

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

## 11. Pi squared is nearly 10

**原文标题**: Pi squared is nearly 10

**原文链接**: [https://mihai.page/pi-square-is-10/](https://mihai.page/pi-square-is-10/)

生成摘要时出错

---

## 12. 'There Is No Going Back': The Inside Story of Europe's Rupture with America

**原文标题**: 'There Is No Going Back': The Inside Story of Europe's Rupture with America

**原文链接**: [https://www.wsj.com/world/europe/european-rupture-with-america-e3a9bb3c](https://www.wsj.com/world/europe/european-rupture-with-america-e3a9bb3c)

生成摘要时出错

---

## 13. Falling fertility on the left as key driver of US birth decline

**原文标题**: Falling fertility on the left as key driver of US birth decline

**原文链接**: [https://www.nature.com/articles/s41598-026-57582-3](https://www.nature.com/articles/s41598-026-57582-3)

生成摘要时出错

---

## 14. Electric anti-aircraft interceptor drone breaks world air speed record at 434mph

**原文标题**: Electric anti-aircraft interceptor drone breaks world air speed record at 434mph

**原文链接**: [https://www.tomshardware.com/tech-industry/drones/electric-drone-breaks-world-air-speed-record-at-434-mph-designed-for-anti-aircraft-interceptor-roles-german-firm-convincingly-smashed-the-official-409-mph-record-hopes-to-get-stamp-of-approval-from-guinness-soon](https://www.tomshardware.com/tech-industry/drones/electric-drone-breaks-world-air-speed-record-at-434-mph-designed-for-anti-aircraft-interceptor-roles-german-firm-convincingly-smashed-the-official-409-mph-record-hopes-to-get-stamp-of-approval-from-guinness-soon)

生成摘要时出错

---

## 15. Show HN: Osint tool that finds exposed files on domains

**原文标题**: Show HN: Osint tool that finds exposed files on domains

**原文链接**: [https://search.cerast-intelligence.com/](https://search.cerast-intelligence.com/)

生成摘要时出错

---

## 16. Why DMARC's new "NP" tag can fail with DNSSEC

**原文标题**: Why DMARC's new "NP" tag can fail with DNSSEC

**原文链接**: [https://dmarcwise.io/blog/dmarc-np-incompatibility-with-dnssec](https://dmarcwise.io/blog/dmarc-np-incompatibility-with-dnssec)

生成摘要时出错

---

## 17. Dependencies should be fetched directly from VCS

**原文标题**: Dependencies should be fetched directly from VCS

**原文链接**: [https://www.arp242.net/deps-vcs.html](https://www.arp242.net/deps-vcs.html)

生成摘要时出错

---

## 18. The AI Superforecasters Are Here

**原文标题**: The AI Superforecasters Are Here

**原文链接**: [https://www.astralcodexten.com/p/the-ai-superforecasters-are-here](https://www.astralcodexten.com/p/the-ai-superforecasters-are-here)

生成摘要时出错

---

## 19. Egg companies made $1.22B in profit off $6 carton

**原文标题**: Egg companies made $1.22B in profit off $6 carton

**原文链接**: [https://fortune.com/2026/07/02/egg-price-fixing-crisis-cover-cash-and-eggs/](https://fortune.com/2026/07/02/egg-price-fixing-crisis-cover-cash-and-eggs/)

生成摘要时出错

---

## 20. Is The Economist Always Wrong?

**原文标题**: Is The Economist Always Wrong?

**原文链接**: [https://economist.com/interactive/finance-and-economics/2026/07/02/is-the-economist-always-wrong](https://economist.com/interactive/finance-and-economics/2026/07/02/is-the-economist-always-wrong)

生成摘要时出错

---

## 21. Januscape: Guest-to-Host Escape in KVM/x86 [CVE-2026-53359]

**原文标题**: Januscape: Guest-to-Host Escape in KVM/x86 [CVE-2026-53359]

**原文链接**: [https://github.com/V4bel/Januscape](https://github.com/V4bel/Januscape)

生成摘要时出错

---

## 22. New Microsoft 365 pricing live, some products up by 42% due to AI

**原文标题**: New Microsoft 365 pricing live, some products up by 42% due to AI

**原文链接**: [https://www.windowslatest.com/2026/07/05/microsoft-365-just-got-a-price-hike-over-continuous-innovation-but-copilot-is-the-ai-tax-on-businesses/](https://www.windowslatest.com/2026/07/05/microsoft-365-just-got-a-price-hike-over-continuous-innovation-but-copilot-is-the-ai-tax-on-businesses/)

生成摘要时出错

---

## 23. What does Jeff Bezos think is going to happen?

**原文标题**: What does Jeff Bezos think is going to happen?

**原文链接**: [https://reprog.wordpress.com/2026/07/05/what-does-jeff-bezos-think-is-going-to-happen/](https://reprog.wordpress.com/2026/07/05/what-does-jeff-bezos-think-is-going-to-happen/)

生成摘要时出错

---

## 24. How the U.S. Engineered Its Sovereignty

**原文标题**: How the U.S. Engineered Its Sovereignty

**原文链接**: [https://spectrum.ieee.org/us-engineered-sovereignty](https://spectrum.ieee.org/us-engineered-sovereignty)

生成摘要时出错

---

## 25. Reflections on the Guillotine (1957)

**原文标题**: Reflections on the Guillotine (1957)

**原文链接**: [https://theanarchistlibrary.org/library/albert-camus-reflections-on-the-guillotine](https://theanarchistlibrary.org/library/albert-camus-reflections-on-the-guillotine)

生成摘要时出错

---

## 26. Multilingual experience linked to delayed aging

**原文标题**: Multilingual experience linked to delayed aging

**原文链接**: [https://fens2026.abstractserver.com/program/#/details/presentations/5474](https://fens2026.abstractserver.com/program/#/details/presentations/5474)

生成摘要时出错

---

## 27. Bryan Johnson: I have an autoimmune disease. My stomach is eating itself

**原文标题**: Bryan Johnson: I have an autoimmune disease. My stomach is eating itself

**原文链接**: [https://twitter.com/bryan_johnson/status/2072069730517860385](https://twitter.com/bryan_johnson/status/2072069730517860385)

生成摘要时出错

---

## 28. "Software Engineering" Is Not Engineering (2005)

**原文标题**: "Software Engineering" Is Not Engineering (2005)

**原文链接**: [https://web.archive.org/web/20050615235108/http://www.geocities.com/tablizer/science.htm](https://web.archive.org/web/20050615235108/http://www.geocities.com/tablizer/science.htm)

生成摘要时出错

---

## 29. Generate parametric, manufacturable 3D models in seconds

**原文标题**: Generate parametric, manufacturable 3D models in seconds

**原文链接**: [https://kyrall.com/](https://kyrall.com/)

生成摘要时出错

---

## 30. Connections in Math: the two kinds of random

**原文标题**: Connections in Math: the two kinds of random

**原文链接**: [https://stillthinking.net/posts/connections-in-math-two-kinds-of-random/](https://stillthinking.net/posts/connections-in-math-two-kinds-of-random/)

生成摘要时出错

---

