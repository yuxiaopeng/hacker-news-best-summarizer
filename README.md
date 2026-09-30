# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-09-30.md)

*最后自动更新时间: 2026-09-30 23:19:48*
## 1. GPT 6.1 Sol：准Astra级智能，五分之一价格

**原文标题**: GPT 6.1 Sol: Near-Astra intelligence for a fifth of the price

**原文链接**: [https://openai.com/index/introducing-gpt-6-1-sol/](https://openai.com/index/introducing-gpt-6-1-sol/)

OpenAI 已推出 GPT-6.1 Sol，这是 GPT-6 Sol 的一次强大升级，旨在提供接近 GPT-6 Astra 的智能，而标准输入和输出 token 价格仅为 Astra 的五分之一。缓存输入成本惊人的低，每百万 token 仅需 0.10 美元，这大大降低了开发者的成本。

GPT-6.1 Sol 在各项任务中均展现出显著改进：
*   **编码：** 在复杂软件工程任务 (DeepSWE v1.1) 上达到 GPT-6 Astra 的水平，成本仅为其五分之一，并显著优于 GPT-6 Sol。
*   **专业工作：** 在复杂 PDF 理解 (GDP.pdf) 上接近 Astra 的表现，并在多步骤业务工作流 (AutomationBench) 中超越 Opus 5.5，所有这些都以极低的成本实现。
*   **计算机使用：** 在高要求计算机使用工作流 (OSWorld 2.0) 上取得显著进展，优于 GPT-6 Sol，并以七分之一的成本接近 Astra 的得分。
*   **科学研究：** 在科学工作流 (Terminal-Bench Science 0.1) 中，GPT-6.1 Sol 的得分是 GPT-6 Sol 的两倍以上，且成本不到其一半，提供了强大的能力，成本比 Astra 或 Opus 5.5 低75%以上，尽管 Astra 在最困难的任务上仍保持优势。
*   **事实性：** 在低推理难度下，相比 GPT-6 Sol，事实错误率降低约32%，以显著更低的成本，与 Astra 的准确性不相上下。

安全与对齐评估显示，GPT-6.1 Sol 有了显著改进，更接近 Astra，在尊重用户意图和安全限制方面具有更高的透明度和可靠性。

GPT-6.1 Sol 立即面向 ChatGPT Work 和 Codex 中的 Plus、Pro、Business、Enterprise 和 Edu 用户，以及通过 OpenAI API 提供。一个提供高达8倍 token 生成速度的“超快”版本也将很快发布。

---

## 2. Livenerf: Opus 5.5 被削弱了没有？

**原文标题**: Livenerf: Has Opus 5.5 been nerfed yet?

**原文链接**: [https://github.com/ninjahawk/livenerf](https://github.com/ninjahawk/livenerf)

Livenerf是一个开源的、确定性的基准测试，旨在检测前沿AI模型（例如Claude Opus 5.5）在发布后是否会悄然退化或“削弱”（nerf）。它旨在提供一个干净的零日基线，以反驳关于模型性能变化的猜测性报告。

该系统通过无头Claude代码在Claude Max订阅上运行，确保所有其他变量固定：固定的提示、锁定的CLI、精确的评分器和原始日志。它通过数千个样本衡量统计漂移，利用Inspect（英国AI安全研究所的评估框架）和Anthropic自己的误差棒方法。主要指标是每个项目的配对分数与基线之间的差异，输出token数量作为关键的次要指标，因为工作量减少通常会首先在那里体现出来。

对于Opus 5.5，该基准测试于2026年9月24日启动，每日运行30天（前10天用于建立基线）。其测试集包含78个来自GPQA Diamond和MMLU-Pro等高风险基准测试的“有时正确”问题，以最大化信息价值。一个使用Opus 5的对照组同时运行，以区分模型变化和平台变化。

Livenerf可以检测到每10天窗口大约7.5点的准确率变化。虽然在发现显著的工作量下降（例如，token减少62%导致准确率下降8.3%）方面很有效，但以目前的样本量，它目前无法可靠地区分Opus 5和5.5。结果（包括改进和退步）将以滚动10天表格的形式发布。仅当满足预先设定的规则时才宣布发生变化：两个连续10天窗口的99%置信区间不包含零，效果至少为3点，且对照组没有显示出类似的变化。

---

## 3. 大家都回家了。没人来。

**原文标题**: Everybody’s home. No one’s coming over

**原文链接**: [https://www.derekthompson.org/p/the-death-of-the-american-host](https://www.derekthompson.org/p/the-death-of-the-american-host)

文章《人人都在家，无人再来访》强调了美国人招待宾客和面对面社交的急剧减少，称之为“招待文化的消亡”。自1975年以来，定期在家招待亲友的美国人比例下降了70%，从42%降至2026年的12%。这一趋势并非因为人们转向餐馆或新的集体活动；相反，整体面对面社交活动减少，居家时间显著增加。

作者为此“大规模停止邀约”现象提出了四个主要解释：

1.  **忙碌的休闲阶层/双职工家庭：** 随着社会变得更富裕，以及更多女性进入劳动力市场，人们感到更加忙碌。招待宾客需要大量的后勤工作，对于忙碌的双职工家庭来说，这变成了不讨喜的“无偿派对策划”，因为男性并未承担起社交活动的重担。
2.  **密集型育儿：** 现代父母在更少的孩子身上投入了更多时间。曾经用于成人社交的夜晚，如今被育儿事务占据。
3.  **友谊网络萎缩：** 亲密友谊的平均数量正在减少，尤其是在受教育程度较低和未婚人群中。这使得招待宾客变得不那么可行，使其成为一种“奢侈品”。
4.  **独自在家也乐趣无穷：** 个性化的家庭娱乐（屏幕、流媒体）让独自待在家里变得极其舒适、便捷和引人入胜，从而降低了人们对社交互动的感知需求。

最终，文章认为，技术使得他人在休闲时变得“不那么必要”。这种“协调失败”意味着方便的、独自进行的活动取代了社交聚会所需的努力，导致人们的社交生活日益萎缩。

---

## 4. 双子座4号 氩

**原文标题**: Gemini 4 Argon

**原文链接**: [https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-argon/](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-argon/)

谷歌宣布推出Gemini 4 Argon，这是一款新的前沿AI模型，旨在针对复杂、长周期专业任务进行深度推理。Argon最初通过“顺风计划”（Fairwind Program）向值得信赖的网络防御者推出，在实际软件工程、企业知识工作（法律、金融）和网络安全防御方面表现卓越。

其一项突出特点是业界领先的100万个token限制，实现了深刻的多步骤问题解决能力。在内部，谷歌利用Argon优化量子算法，自主提升数据中心的内存效率（释放数百TiB），并将关键系统的庞大代码库从C/C++迁移到Rust。

Argon设定了新的基准，在软件工程领域的DeepSWE v1.1上达到最先进水平（77.9%），并在衡量金融、编码、法律和税务经济影响的Vals指数上处于领先地位。它还在Zapier的AutomationBench上排名第一（51.3%），并展示了先进的长视频理解能力（LVBench 91.7%）。

至关重要的是，Argon在网络安全防御方面能力极强，能够自主发现、验证和修补关键软件漏洞。像Wiz这样的可信防御者已经在使用它来发现严重风险，它在CWE-bench v1（68%）的漏洞修复方面并列第一。

谷歌强调分阶段发布，通过严格测试优先确保安全，并加强防范滥用（网络、CBRN攻击）、提示注入和模型失调的保障措施。Argon将以每百万输入token 2美元的介绍价提供，在收集早期测试者的反馈后，计划向开发者、企业和消费者提供更广泛的访问权限。

---

## 5. 点：始终在线智能体

**原文标题**: Dots: Always-on agents

**原文链接**: [https://openai.com/index/introducing-dots/](https://openai.com/index/introducing-dots/)

OpenAI 于2026年9月29日推出了“Dots”，它们是功能卓越、始终在线的AI智能体，由GPT-6 Astra提供支持。Dots 旨在学习用户偏好，持续为个人工作，自动化任务并节省时间。它们在自己的云计算机上运行，通过反馈学习，并通过插件连接到4,000多个应用程序。

用户可以通过ChatGPT、Slack、Teams或语音通话与他们的Dot进行交互，智能体可以在不同平台之间传递上下文。Dots 主动预测需求并执行工作，例如开发者接收经过测试的代码修复，产品负责人修改发布材料，或内容创作者起草社交帖子。

Dots 内置了强大的安全和隐私保护措施，使用独立的云计算机，用户可以控制应用权限，设置自定义操作规则，并对敏感任务进行审批。它们还通过对连接应用进行只读访问来开展“主动研究”。来自商业版、企业版和教育版工作空间的用户数据默认不用于模型改进。

Dots 将面向Pro、Business Premium和Enterprise计划推出，第一个Dot已包含在现有订阅中。OpenAI 设想Dots团队协同工作，并正在试点用于组织职责的专业Dots，计划将其整合到Microsoft Agent 365中。

---

## 6. America.gov

**原文标题**: America.gov

**原文链接**: [https://america.gov/](https://america.gov/)

生成摘要时出错

---

## 7. You said no MCP

**原文标题**: You said no MCP

**原文链接**: [https://earendil.com/posts/you-said-no-mcp/](https://earendil.com/posts/you-said-no-mcp/)

生成摘要时出错

---

## 8. How Delhi cut electricity loss from 50 to 5 percent

**原文标题**: How Delhi cut electricity loss from 50 to 5 percent

**原文链接**: [https://spectrum.ieee.org/delhi-electricity-loss](https://spectrum.ieee.org/delhi-electricity-loss)

生成摘要时出错

---

## 9. DraftKings is using AI to behaviorally target chronic gamblers

**原文标题**: DraftKings is using AI to behaviorally target chronic gamblers

**原文链接**: [https://www.eff.org/deeplinks/2026/09/draftkings-using-ai-supercharge-harms-online-behavioral-advertising](https://www.eff.org/deeplinks/2026/09/draftkings-using-ai-supercharge-harms-online-behavioral-advertising)

生成摘要时出错

---

## 10. 500k facial scans at UK stations yield no arrests, 1 false positive

**原文标题**: 500k facial scans at UK stations yield no arrests, 1 false positive

**原文链接**: [https://www.theguardian.com/technology/2026/sep/29/trial-live-facial-recognition-cameras-london-stations-false-positive](https://www.theguardian.com/technology/2026/sep/29/trial-live-facial-recognition-cameras-london-stations-false-positive)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-09-30](output/hacker_news_summary_2026-09-30.md) |
| 2 | [2026-09-24](output/hacker_news_summary_2026-09-24.md) |
| 3 | [2026-09-29](output/hacker_news_summary_2026-09-29.md) |
| 4 | [2026-09-23](output/hacker_news_summary_2026-09-23.md) |
| 5 | [2026-09-27](output/hacker_news_summary_2026-09-27.md) |
| 6 | [2026-09-22](output/hacker_news_summary_2026-09-22.md) |
| 7 | [2026-09-25](output/hacker_news_summary_2026-09-25.md) |
| 8 | [2026-09-21](output/hacker_news_summary_2026-09-21.md) |
| 9 | [2026-09-20](output/hacker_news_summary_2026-09-20.md) |
| 10 | [2026-09-17](output/hacker_news_summary_2026-09-17.md) |
| 11 | [2026-09-19](output/hacker_news_summary_2026-09-19.md) |
| 12 | [2026-09-18](output/hacker_news_summary_2026-09-18.md) |
| 13 | [2026-09-10](output/hacker_news_summary_2026-09-10.md) |
| 14 | [2026-09-13](output/hacker_news_summary_2026-09-13.md) |
| 15 | [2026-09-16](output/hacker_news_summary_2026-09-16.md) |
| 16 | [2026-09-14](output/hacker_news_summary_2026-09-14.md) |
| 17 | [2026-09-11](output/hacker_news_summary_2026-09-11.md) |
| 18 | [2026-09-12](output/hacker_news_summary_2026-09-12.md) |
| 19 | [2026-09-15](output/hacker_news_summary_2026-09-15.md) |
| 20 | [2026-09-03](output/hacker_news_summary_2026-09-03.md) |
| 21 | [2026-09-09](output/hacker_news_summary_2026-09-09.md) |
| 22 | [2026-09-04](output/hacker_news_summary_2026-09-04.md) |
| 23 | [2026-09-08](output/hacker_news_summary_2026-09-08.md) |
| 24 | [2026-09-05](output/hacker_news_summary_2026-09-05.md) |
| 25 | [2026-09-07](output/hacker_news_summary_2026-09-07.md) |
| 26 | [2026-09-06](output/hacker_news_summary_2026-09-06.md) |
| 27 | [2026-09-02](output/hacker_news_summary_2026-09-02.md) |
| 28 | [2026-08-31](output/hacker_news_summary_2026-08-31.md) |
| 29 | [2026-08-28](output/hacker_news_summary_2026-08-28.md) |
| 30 | [2026-09-01](output/hacker_news_summary_2026-09-01.md) |
| 31 | [2026-08-29](output/hacker_news_summary_2026-08-29.md) |
| 32 | [2026-08-30](output/hacker_news_summary_2026-08-30.md) |
| 33 | [2026-08-22](output/hacker_news_summary_2026-08-22.md) |
| 34 | [2026-08-25](output/hacker_news_summary_2026-08-25.md) |
| 35 | [2026-08-19](output/hacker_news_summary_2026-08-19.md) |
| 36 | [2026-08-20](output/hacker_news_summary_2026-08-20.md) |
| 37 | [2026-08-23](output/hacker_news_summary_2026-08-23.md) |
| 38 | [2026-08-21](output/hacker_news_summary_2026-08-21.md) |
| 39 | [2026-08-24](output/hacker_news_summary_2026-08-24.md) |
| 40 | [2026-08-26](output/hacker_news_summary_2026-08-26.md) |
| 41 | [2026-08-12](output/hacker_news_summary_2026-08-12.md) |
| 42 | [2026-08-14](output/hacker_news_summary_2026-08-14.md) |
| 43 | [2026-08-16](output/hacker_news_summary_2026-08-16.md) |
| 44 | [2026-08-17](output/hacker_news_summary_2026-08-17.md) |
| 45 | [2026-08-18](output/hacker_news_summary_2026-08-18.md) |
| 46 | [2026-08-15](output/hacker_news_summary_2026-08-15.md) |
| 47 | [2026-08-13](output/hacker_news_summary_2026-08-13.md) |
| 48 | [2026-08-11](output/hacker_news_summary_2026-08-11.md) |
| 49 | [2026-08-10](output/hacker_news_summary_2026-08-10.md) |
| 50 | [2026-08-09](output/hacker_news_summary_2026-08-09.md) |
| 51 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 52 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 53 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 54 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 55 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 56 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 57 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 58 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 59 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 60 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 61 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 62 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 63 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 64 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 65 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 66 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 67 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 68 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 69 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 70 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 71 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 72 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 73 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 74 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 75 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 76 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 77 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 78 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 79 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 80 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 81 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 82 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 83 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 84 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 85 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 86 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 87 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 88 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 89 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 90 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 91 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 92 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 93 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 94 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 95 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 96 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 97 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 98 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 99 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 100 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 101 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 102 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 103 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 104 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 105 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 106 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 107 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 108 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 109 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 110 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 111 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 112 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 113 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 114 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 115 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 116 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 117 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 118 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 119 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 120 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 121 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 122 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 123 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 124 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 125 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 126 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 127 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 128 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 129 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 130 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 131 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 132 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 133 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 134 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 135 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 136 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 137 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 138 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 139 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 140 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 141 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 142 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 143 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 144 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 145 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 146 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 147 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 148 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 149 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 150 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 151 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 152 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 153 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 154 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 155 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 156 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 157 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 158 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 159 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 160 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 161 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 162 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 163 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 164 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 165 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 166 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 167 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 168 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 169 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 170 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 171 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 172 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 173 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 174 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 175 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 176 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 177 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 178 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 179 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 180 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 181 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 182 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 183 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 184 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 185 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 186 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 187 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 188 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 189 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 190 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 191 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 192 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 193 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 194 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 195 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 196 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 197 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 198 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 199 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 200 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 201 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 202 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 203 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 204 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 205 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 206 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 207 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 208 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 209 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 210 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 211 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 212 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 213 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 214 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 215 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 216 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 217 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 218 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 219 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 220 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 221 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 222 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 223 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 224 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 225 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 226 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 227 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 228 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 229 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 230 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 231 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 232 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 233 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 234 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 235 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 236 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 237 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 238 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 239 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 240 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 241 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 242 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 243 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 244 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 245 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 246 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 247 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 248 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 249 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 250 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 251 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 252 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 253 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 254 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 255 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 256 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 257 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 258 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 259 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 260 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 261 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 262 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 263 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 264 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 265 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 266 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 267 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 268 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 269 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 270 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 271 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 272 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 273 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 274 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 275 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 276 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 277 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 278 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 279 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 280 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 281 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 282 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 283 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 284 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 285 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 286 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 287 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 288 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 289 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 290 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 291 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 292 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 293 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 294 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 295 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 296 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 297 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 298 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 299 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 300 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 301 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 302 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 303 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 304 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 305 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 306 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 307 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 308 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 309 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 310 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 311 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 312 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 313 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 314 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 315 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 316 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 317 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 318 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 319 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 320 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 321 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 322 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 323 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
