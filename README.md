# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-04-07.md)

*最后自动更新时间: 2026-04-07 20:14:28*
## 1. 萨姆·奥特曼或将掌控我们的未来——他可信吗？

**原文标题**: Sam Altman may control our future – can he be trusted?

**原文链接**: [https://www.newyorker.com/magazine/2026/04/13/sam-altman-may-control-our-future-can-he-be-trusted](https://www.newyorker.com/magazine/2026/04/13/sam-altman-may-control-our-future-can-he-be-trusted)

2023年末，OpenAI首席执行官山姆·奥特曼（Sam Altman）被由首席科学家伊利亚·苏茨克维尔（Ilya Sutskever）领导的董事会秘密解雇，原因是董事会对其诚信以及在安全协议方面涉嫌虚假陈述存在严重担忧。作为联合创始人的苏茨克维尔认为奥特曼不适合掌控接近人类智能水平的技术，并指出他“撒谎”的一贯模式。该董事会以将人类安全置于利润之上为宗旨，认为奥特曼缺乏必要的诚信。

奥特曼被解雇一事令微软等投资者措手不及，并叫停了与Thrive公司计划中的860亿美元估值交易。奥特曼迅速发起了一场积极的公关反击战，将董事会的行动定性为一场“政变”。在微软威胁要启动竞争性业务以及员工大规模离职的背景下，董事会在五天内被迫恢复了奥特曼的职务。

解雇奥特曼的董事会成员被新成员取代，这些新成员是与奥特曼密切协商后选出的。尽管要求对这些指控进行调查，但新董事会的独立性却引人质疑。

关于奥特曼诚信的争论仍在继续。他的前同事坚持对奥特曼涉嫌欺骗的担忧，认为这对如此颠覆性人工智能的领导者来说是危险的。与此同时，奥特曼驳斥了这些批评，将其归因于过去对冲突的回避，尽管一位前董事会成员将他“我无法改变我的个性”的言论解读为承认持续的欺骗。奥特曼现在推动着OpenAI的快速增长以及雄心勃勃的人工智能基础设施计划，引发了关于谁来掌控人类未来的关键问题。

---

## 2. 问题：Claude Code在二月更新后无法用于复杂的工程任务。

**原文标题**: Issue: Claude Code is unusable for complex engineering tasks with Feb updates

**原文链接**: [https://github.com/anthropics/claude-code/issues/42796](https://github.com/anthropics/claude-code/issues/42796)

署名为“stellaraccident”的详细分析指出，自2026年2月更新以来，Claude Code（Opus模型）在复杂工程任务中的性能严重下降。来自6,852个会话、17,871个思考块和234,760次工具调用的定量数据显示，这种退步与“思考内容删减”的推出以及此前估计思考深度的下降密切相关。

该报告涵盖2026年1月30日至4月1日，显示截至2月底思考深度下降了67%，随后到3月12日实现了完全删减。3月8日独立报告的质量问题，与内容删减达到50%的时间点精确吻合。

主要行为转变包括：
*   **研究减少：** 读取与编辑比率下降70%（从6.6降至2.0），导致在缺乏适当上下文的情况下出现“先编辑”行为。
*   **错误增多：** “未先读取即编辑”的情况从6.2%激增至33.7%。
*   **推理能力下降：** “推理循环”、“最简修复”心态、过早停止、寻求许可（3月8日后出现173次程序化停止钩子违规，此前为零）、用户中断以及自认的质量问题显著增加。
*   **精准度丧失：** 整文件写入使用量翻倍，且约定遵循度受损。

该分析认为，“扩展思考令牌”对于高级工程工作流中的多步骤规划、约定遵循、自我纠正和连贯推理至关重要。当思考深度不足时，模型会默认采取“最廉价的行动”，例如不阅读就编辑或过早停止。

作者建议Anthropic提高思考分配的透明度，为高级用户提供“最大思考”层级，在API响应中公开`thinking_tokens`，并监控停止钩子违规率等金丝雀指标。

---

## 3. 我不会下载你们的App。网页版用起来没毛病。

**原文标题**: I won't download your app. The web version is a-ok

**原文链接**: [https://www.0xsid.com/blog/wont-download-your-app](https://www.0xsid.com/blog/wont-download-your-app)

The author expresses significant frustration over companies aggressively pushing users from web versions to dedicated apps, often via intrusive pop-ups and deliberately hobbled web experiences. They champion web usage for the superior control it offers, enabling customizability through user scripts, ad-blockers, and extensions to enhance usability and block unwanted content.

The article argues that app makers prioritize apps to gain more control over users. Apps facilitate dark patterns, push notifications, intrusive data collection (telemetry), and lock users into "walled gardens" for retention, rather than genuinely improving user experience. The author questions the necessity of most apps, contending many are merely "thin clients" displaying simple text and media (JSON data) that a browser could easily handle, without requiring large downloads, extensive permissions, or background processes.

Moreover, the author criticizes the quality of many apps, noting they often lack a polished native feel, exhibiting "uncanny valley" jankiness—subtle inconsistencies in scrolling, gestures, or timing that detract from the experience.

This trend is termed the "enshittification loop": companies initially attract users on the open, frictionless web, then deliberately degrade the web version to force them into apps. Once inside the app, users become a captive audience for ads and data collection, bypassing browser-based controls. This strategy, driven by financial incentives and app download metrics, transforms the browser into a mere marketing funnel for app stores, despite the web's inherent advantages.

---

## 4. HN 展示：我打造了一个微型 LLM，用以揭秘语言模型的工作原理。

**原文标题**: Show HN: I built a tiny LLM to demystify how language models work

**原文链接**: [https://github.com/arman-bd/guppylm](https://github.com/arman-bd/guppylm)

GuppyLM是一个约900万参数的语言模型，旨在揭秘大型语言模型（LLM）的训练过程，展示任何人都可以在没有博士学位或大量资源的情况下从零开始构建一个。它扮演着一条名叫Guppy的小鱼，用简短、小写的句子谈论它的水生世界（水、食物、光线、鱼缸生活），并刻意避免人类的抽象概念。

该项目强调易用性：用户可以在单个Colab T4 GPU上约五分钟内训练自己的GuppyLM，或者在浏览器中（通过一个约10MB的量化ONNX模型）或本地与预训练版本进行聊天。

GuppyLM采用普通的Transformer架构，包含6层、384个隐藏维度、一个4,096词元的BPE词汇表和128词元的最大序列长度。它的简洁性（没有GQA、RoPE等）是刻意的，旨在清晰地解释大型语言模型的工作原理。它通过模板组合生成了涵盖60个主题的60,000个合成对话进行训练，旨在确保其具备友善、好奇且痴迷食物的一致鱼类个性。

设计选择包括将个性融入模型权重（无需系统提示）、由于上下文窗口较短而侧重于可靠的单轮交互，以及利用定制的合成数据。该项目提供了数据生成、分词器、模型架构、训练和推理的完整代码，并采用MIT许可证。

---

## 5. HN 展示：粗野主义混凝土笔记本支架 (2024)

**原文标题**: Show HN: Brutalist Concrete Laptop Stand (2024)

**原文链接**: [https://sam-burns.com/posts/concrete-laptop-stand/](https://sam-burns.com/posts/concrete-laptop-stand/)

一位粗野主义建筑爱好者制作了一个独特的“粗野主义混凝土笔记本支架”，旨在捕捉“beton brut”（清水混凝土）美学和城市衰败的主题。这个支架可能重达世界之最，集成了实用功能，例如两个2.1安培的USB充电端口和一个笔记本电脑用的三孔插座。

它的设计以悬挑结构体现了粗野主义风格，并有意融入了破败元素：一个受损的角落、裸露的生锈钢筋，以及经过氨水处理、呈现老旧外观的假腐蚀铜线。支架上还带有一个一体化的酥油罐花盆，里面栽种着一盆“佛珠吊兰”，一个带有仿真苔藓的人工锈蚀笔筒则共同完善了城市衰败的主题。

这个支架通过两次混凝土浇筑制成，故意采用不均匀的混合和打磨，以营造出风化的表面。创作者对最终成品感到非常满意，指出粗野主义和城市衰败的主题都成功实现了，尽管其沉重的分量需要用手推车才能搬运。

---

## 6. France pulls last gold held in US

**原文标题**: France pulls last gold held in US

**原文链接**: [https://www.mining.com/france-pulls-last-gold-held-in-us-for-15b-gain/](https://www.mining.com/france-pulls-last-gold-held-in-us-for-15b-gain/)

法国已成功完成将其此前存放在美国的全部黄金储备遣返本国的工作，这项战略性进程始于20世纪60年代戴高乐总统的倡议，现已圆满结束。此举涉及将实物黄金从纽约联邦储备银行运回，据报道，这为法国带来了150亿美元的巨额未实现收益，得益于自购入以来黄金价格的大幅上涨。

戴高乐最初启动遣返行动是出于对美元稳定性的担忧，以及在布雷顿森林体系下，法国希望摆脱美国货币政策的束缚，捍卫自身的金融独立性。

此次遣返工作的完成使法国成为全球第五大黄金持有国，其目前储备量为2,436.5吨，价值超过1500亿美元。法国的行动与各国央行，特别是欧洲（包括德国、荷兰、比利时和奥地利）央行遣返黄金的更广泛趋势相吻合。这一趋势近年来有所加速，其推动因素是对国家资产拥有更大控制权的愿望、地缘政治担忧，以及在2008年金融危机和2014年克里米亚被吞并等事件之后，对美元和国际金融体系日益增长的不信任感。

---

## 7. 凭感觉编程的狂热，正是内部自用模式的走火入魔。

**原文标题**: The cult of vibe coding is dogfooding run amok

**原文链接**: [https://bramcohen.com/p/the-cult-of-vibe-coding-is-insane](https://bramcohen.com/p/the-cult-of-vibe-coding-is-insane)

生成摘要时出错

---

## 8. Are We Idiocracy Yet?

**原文标题**: Are We Idiocracy Yet?

**原文链接**: [https://idiocracy.wtf/](https://idiocracy.wtf/)

生成摘要时出错

---

## 9. 密码工程师眼中的量子计算时间线

**原文标题**: A cryptography engineer's perspective on quantum computing timelines

**原文链接**: [https://words.filippo.io/crqc-timeline/](https://words.filippo.io/crqc-timeline/)

生成摘要时出错

---

## 10. Battle for Wesnoth: open-source, turn-based strategy game

**原文标题**: Battle for Wesnoth: open-source, turn-based strategy game

**原文链接**: [https://www.wesnoth.org](https://www.wesnoth.org)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 2 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 3 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 4 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 5 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 6 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 7 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 8 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 9 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 10 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 11 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 12 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 13 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 14 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 15 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 16 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 17 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 18 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 19 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 20 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 21 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 22 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 23 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 24 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 25 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 26 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 27 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 28 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 29 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 30 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 31 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 32 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 33 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 34 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 35 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 36 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 37 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 38 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 39 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 40 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 41 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 42 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 43 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 44 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 45 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 46 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 47 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 48 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 49 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 50 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 51 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 52 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 53 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 54 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 55 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 56 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 57 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 58 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 59 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 60 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 61 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 62 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 63 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 64 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 65 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 66 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 67 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 68 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 69 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 70 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 71 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 72 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 73 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 74 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 75 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 76 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 77 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 78 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 79 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 80 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 81 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 82 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 83 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 84 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 85 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 86 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 87 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 88 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 89 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 90 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 91 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 92 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 93 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 94 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 95 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 96 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 97 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 98 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 99 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 100 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 101 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 102 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 103 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 104 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 105 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 106 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 107 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 108 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 109 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 110 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 111 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 112 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 113 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 114 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 115 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 116 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 117 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 118 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 119 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 120 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 121 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 122 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 123 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 124 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 125 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 126 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 127 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 128 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 129 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 130 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 131 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 132 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 133 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 134 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 135 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 136 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 137 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 138 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 139 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 140 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 141 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 142 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 143 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 144 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 145 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 146 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 147 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 148 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 149 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 150 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 151 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
