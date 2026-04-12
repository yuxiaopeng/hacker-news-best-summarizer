# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-04-12.md)

*最后自动更新时间: 2026-04-12 20:10:31*
## 1. 锉掉我的 MacBook 的边角

**原文标题**: Filing the corners off my MacBooks

**原文链接**: [https://kentwalters.com/posts/corners/](https://kentwalters.com/posts/corners/)

作者详细介绍了他们将MacBook锋利的铝制边角打磨圆润的做法，这项定制他们预计会让其他人感到不解甚至震惊。他们的主要动机是锋利的底部边缘对手腕造成的不适，同时他们坚信应该将自己的工具个性化。

这项改造尤其集中在屏幕凹槽附近的尖锐区域，作者在那里小心翼翼地打磨出了新的、更柔和的曲线。整个过程包括夹紧MacBook，并用胶带封住扬声器和键盘等敏感区域，以防止铝屑进入。他们先用粗锉刀打磨，然后用150和400目砂纸将表面打磨光滑，并对结果表示满意。尽管最初担心会打磨穿机器，但事实证明这并非问题。

这次改造是在一台工作电脑上进行的，作者计划未来也会以类似方式改造其他机器。他们积极鼓励其他人克服对定制自己设备的任何顾虑，敦促他们“放开手脚去折腾一下”，并向那些考虑此类改造的人提供支持。

---

## 2. 阿耳忒弥斯2号安全溅落

**原文标题**: Artemis II safely splashes down

**原文链接**: [https://www.cbsnews.com/live-updates/artemis-ii-splashdown-return/](https://www.cbsnews.com/live-updates/artemis-ii-splashdown-return/)

美国国家航空航天局（NASA）的“阿尔忒弥斯2号”任务于2026年4月10日星期五成功结束，猎户座飞船于美国东部时间晚上8点07分在圣迭戈海岸附近的太平洋安全溅落。四名宇航员——指挥官里德·怀斯曼、飞行员维克多·格洛弗、任务专家克里斯蒂娜·科赫和加拿大宇航员杰里米·汉森——在结束了为期10天的任务后返回地球，此次任务创下了人类太空旅行最远距离的记录。

再入过程包括高速下降、在防热罩承受极端温度时有6分钟的通信中断，以及精确的降落伞部署，最终实现了“完美靶心式溅落”。海军回收人员利用充气筏和直升机迅速抵达飞船。在潜水员对“猎户座”内部进行初步医疗检查后，宇航员们走出飞船，表示他们感觉“很棒”，随后被送往“约翰·P·默萨号”（USS John P. Murtha）进行进一步评估。

NASA官员在溅落后的新闻发布会上表达了极大的自豪和兴奋，称赞此次任务是“一个不可思议的结局”和“太空探索新时代的开始”。特朗普总统也祝贺了宇航员们完成了“壮观的”任务。此次成功返回标志着未来月球探索迈出了重要一步。

---

## 3. Small models also found the vulnerabilities that Mythos found

**原文标题**: Small models also found the vulnerabilities that Mythos found

**原文链接**: [https://aisle.com/blog/ai-cybersecurity-after-mythos-the-jagged-frontier](https://aisle.com/blog/ai-cybersecurity-after-mythos-the-jagged-frontier)

生成摘要时出错

---

## 4. 我用每月20美元的技术栈，运营多个MRR达1万美元的公司。

**原文标题**: I run multiple $10K MRR companies on a $20/month tech stack

**原文链接**: [https://stevehanov.ca/blog/how-i-run-multiple-10k-mrr-companies-on-a-20month-tech-stack](https://stevehanov.ca/blog/how-i-run-multiple-10k-mrr-companies-on-a-20month-tech-stack)

这位作者是websequencediagrams.com等产品的幕后推手，一位经验丰富的白手起家者。他提倡通过最小化的技术栈来运营精益创业公司，这与风险投资模式的高烧钱率形成鲜明对比。他展示了如何以每月20美元的开销，实现多家月经常性收入（MRR）达到1万美元的公司。

他的策略包括：
1.  **精益服务器：** 利用Linode或DigitalOcean等提供商每月5-10美元的单一虚拟私有服务器（VPS），放弃AWS EKS/RDS等复杂昂贵的云设置，以实现简单性和成本效益。
2.  **精益语言：** 使用Go开发后端，这是一种性能高、内存效率高的语言，可编译成单个静态链接的二进制文件，从而简化部署和资源使用。
3.  **本地AI处理长时间运行的任务：** 利用个人GPU硬件（例如RTX 3090），配合Ollama、VLLM和Transformer Lab等工具进行免费的AI批量处理，例如总结数千份报告，而不是产生数百美元的云API费用。他还提到了`laconic`和`llmhub`来管理本地LLM。
4.  **OpenRouter实现快速/智能LLM：** 使用OpenRouter访问Claude 3.5 Sonnet或GPT-4o等尖端LLM，用于用户交互。这简化了API管理，整合了账单，并实现了不同提供商之间的自动回退。
5.  **Copilot用于AI IDE：** 在VS Code中利用GitHub Copilot的“按请求计费”模式，每次详细提示大约0.04美元，即可获得大量的AI编码辅助，无论计算持续时间多长。
6.  **SQLite处理所有事务：** 将SQLite作为主要数据库，并强调在启用预写式日志（WAL）的情况下，它具有速度和可扩展性，并提供定制的`smhanov/auth`库用于用户认证。

这种方法提供了无限的运营空间，减轻了压力，并使创始人能够专注于产品市场契合度，而无需承受来自投资者的持续压力或高昂的运营成本。

---

## 5. 安装所有 Firefox 扩展

**原文标题**: Installing every* Firefox extension

**原文链接**: [https://jack.cab/blog/every-firefox-extension](https://jack.cab/blog/every-firefox-extension)

这篇文章详细介绍了一个雄心勃勃的项目，旨在抓取并分析所有Firefox扩展。作者最初在使用Firefox Add-ons API时遇到了困难，由于页面限制和排序约束，只抓取到了30,000个扩展。通过迭代方法，包括多种排序、最终并行按类别查询，以及后续使用日期过滤器，作者成功抓取了84,235个独特的扩展，总计49.3 GB。

分析该数据集揭示了以下几点洞察。最大的扩展是dmitlichess (196.3 MB)，包含2000多个音频文件，而其他扩展则嵌入了Unity应用程序、Tesseract.js或AI模型。最小的扩展是theTabs-saver，大小为7518字节，不含任何代码。由“lolicon”开发的“Tab Stack for Firefox”被评为评分最差的扩展，“Dr. B”则是最多产的开发者，拥有84个“直觉编码”（vibe coded）的扩展。

分析揭示了恶意内容，包括使用同形异义字攻击（homoglyph attacks）和NocoDB来获取钓鱼URL的钓鱼扩展，以及带有可疑主页链接的SEO垃圾邮件扩展。很大一部分涉及来自“Innover Online Group Ltd”和“Atom Apps”等实体的潜在有害应用程序（PUA）。这些公司在不同平台发布了大量扩展（例如“Maps Assist & Custom Web Search”），通常将Yahoo与推广代码集成，共同吸引了数十万用户，其中一些后来被Mozilla禁用。

统计数据显示，34.3%的扩展没有日活跃用户，76.7%是开源的，23%是在本文开始撰写后创建的。文章最后通过获取所有扩展的直接下载URL，以便于批量安装。

---

## 6. Pro Max 5倍配额在1.5小时内用尽，尽管使用量适中

**原文标题**: Pro Max 5x quota exhausted in 1.5 hours despite moderate usage

**原文链接**: [https://github.com/anthropics/claude-code/issues/45756](https://github.com/anthropics/claude-code/issues/45756)

一位使用Claude Code Pro Max 5x (Opus, 1M 上下文) 套餐的用户报告称，尽管是适度使用，但其配额在1.5小时内就耗尽了。这出乎意料，尤其是与之前在高强度开发下持续了5小时的配额窗口期相比，那是一个预期结果。

核心问题似乎是，受益于提示缓存的 `cache_read` 令牌，在计入用户配额时似乎是按全额费率计算的。这抵消了缓存的成本降低优势，导致配额耗尽速度大大加快。数据显示，如果 `cache_read` 令牌以降低的1/10费率（即预期成本）计算，中度使用每小时仅消耗8.7M令牌。然而，如果以全额费率计算（疑似的实际行为），将达到每小时70.5M令牌，这与观察到的配额快速耗尽相符。

其他促成因素包括后台Claude Code会话消耗了大量共享配额（占重置后配额的78%），自动压缩功能通过发送大量上下文创建了昂贵的令牌峰值，以及1M上下文窗口每次API调用都会放大令牌消耗。

用户建议了改进措施，例如明确 `cache_read` 的计费方式，基于*有效*令牌的速率限制，空闲会话检测，以及更好地实时显示配额。Claude Code团队承认，1M令牌上下文窗口成本高昂，尤其是在一个小时不活动后出现提示缓存未命中时，并正在调查默认使用400k上下文窗口，同时实施用户体验改进以引导用户。

---

## 7. 法国政府弃用Windows改用Linux，称美国技术存在战略风险

**原文标题**: France's government is ditching Windows for Linux, says US tech a strategic risk

**原文链接**: [https://www.xda-developers.com/frances-government-ditching-windows-for-linux/](https://www.xda-developers.com/frances-government-ditching-windows-for-linux/)

法国政府正着手放弃来自欧盟以外的专有技术，特别是Windows系统，转而采用Linux等开源解决方案。这一由法国数字部际总局 (DINUM) 宣布的战略转变，旨在增强法国的数字主权，并减少对“欧盟以外”——特别是美国——技术的依赖。

政府认为当前的依赖是一种战略风险，因为它对这些外国解决方案的规则、定价、演进和安全风险缺乏控制。公共行动和账目部长戴维·阿米尔强调，需要“摆脱束缚”，并“重新掌控我们的数字命运”。

所有部委目前都受命绘制其对欧盟以外来源的依赖，并制定一份在秋季前完成的退出计划，尽管具体推出日期尚未确定。虽然主要目标是开源，但如果严格偏好欧盟内部解决方案，也可选用源自欧盟的选项，如openSUSE和LibreOffice。此举凸显了全球范围内为增强控制和安全性而转向开源的日益增长的趋势。

---

## 8. Exploiting the most prominent AI agent benchmarks

**原文标题**: Exploiting the most prominent AI agent benchmarks

**原文链接**: [https://rdi.berkeley.edu/blog/trustworthy-benchmarks-cont/](https://rdi.berkeley.edu/blog/trustworthy-benchmarks-cont/)

A UC Berkeley research team (Hao Wang et al., April 2026) has revealed that eight prominent AI agent benchmarks, including SWE-bench, WebArena, and OSWorld, are fundamentally exploitable. Their automated scanning agent achieved near-perfect scores on all audited benchmarks without solving a single task or employing any AI reasoning, solely by exploiting flaws in how scores are computed.

Exploits included manipulating test infrastructure (e.g., `conftest.py` for SWE-bench, fake `curl` for Terminal-Bench), reading gold answers directly from task configs via `file://` URLs (WebArena), and abusing flawed validation logic (FieldWorkArena). The authors assert this isn't theoretical, citing real-world instances where models have already gamed benchmarks by copying answers or manipulating evaluation environments.

They identify recurring vulnerabilities: lack of isolation between agent and evaluator, answers shipped with tests, `eval()` on untrusted input, prompt injection in LLM judges, weak string matching, and flawed evaluation logic. This systemic problem means benchmarks often measure lookup speed or exploitation skill, not true AI capability, necessitating a fundamental redesign of evaluation methodologies for trustworthiness and robustness.

---

## 9. Chimpanzees in Uganda locked in eight-year 'civil war', say researchers

**原文标题**: Chimpanzees in Uganda locked in eight-year 'civil war', say researchers

**原文链接**: [https://www.bbc.com/news/articles/cr71lkzv49po](https://www.bbc.com/news/articles/cr71lkzv49po)

生成摘要时出错

---

## 10. South Korea introduces universal basic mobile data access

**原文标题**: South Korea introduces universal basic mobile data access

**原文链接**: [https://www.theregister.com/2026/04/10/south_korea_data_access_universal/](https://www.theregister.com/2026/04/10/south_korea_data_access_universal/)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 2 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 3 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 4 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 5 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 6 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 7 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 8 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 9 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 10 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 11 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 12 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 13 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 14 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 15 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 16 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 17 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 18 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 19 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 20 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 21 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 22 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 23 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 24 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 25 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 26 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 27 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 28 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 29 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 30 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 31 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 32 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 33 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 34 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 35 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 36 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 37 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 38 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 39 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 40 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 41 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 42 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 43 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 44 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 45 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 46 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 47 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 48 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 49 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 50 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 51 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 52 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 53 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 54 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 55 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 56 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 57 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 58 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 59 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 60 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 61 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 62 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 63 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 64 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 65 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 66 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 67 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 68 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 69 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 70 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 71 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 72 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 73 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 74 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 75 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 76 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 77 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 78 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 79 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 80 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 81 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 82 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 83 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 84 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 85 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 86 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 87 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 88 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 89 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 90 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 91 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 92 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 93 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 94 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 95 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 96 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 97 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 98 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 99 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 100 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 101 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 102 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 103 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 104 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 105 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 106 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 107 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 108 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 109 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 110 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 111 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 112 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 113 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 114 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 115 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 116 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 117 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 118 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 119 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 120 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 121 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 122 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 123 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 124 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 125 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 126 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 127 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 128 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 129 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 130 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 131 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 132 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 133 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 134 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 135 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 136 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 137 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 138 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 139 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 140 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 141 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 142 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 143 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 144 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 145 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 146 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 147 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 148 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 149 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 150 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 151 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 152 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 153 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 154 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 155 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 156 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
