# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-07-01.md)

*最后自动更新时间: 2026-07-01 21:13:39*
## 1. 克劳德代码正在隐写标记请求

**原文标题**: Claude Code is steganographically marking requests

**原文链接**: [https://thereallo.dev/blog/claude-code-prompt-steganography](https://thereallo.dev/blog/claude-code-prompt-steganography)

thereallo.dev 撰写的文章《Claude Code is steganographically marking requests》揭示，Anthropic 的 Claude 3 Opus 模型（以及可能其他模型）会对其生成的代码进行隐秘水印标记。作者通过观察相同代码输出的字节级差异发现了这一点，识别出 Claude 修改了空白字符。

该模型没有使用标准空格，而是插入了不间断空格（`\u00A0`）、零宽度空格（`\u200B`）或特定的空格和制表符模式，这些对肉眼来说是不可见的。这些隐藏字符编码了可识别的数据，包括 `request_id` 和 `message_id`，有效为每段生成的代码创建了独一无二的指纹。

这种隐写式标记使得 Anthropic 能够将任何代码片段追溯到生成它的特定 API 请求和用户会话。尽管 Anthropic 尚未公开披露此做法，但推断其目的可能是用于审计追踪、安全、滥用预防或内部使用分析。这一发现引发了对用户隐私、Anthropic 缺乏透明度以及代码完整性潜在影响的担忧，因为这些隐藏字符理论上可能导致解析器或 linter 出现问题。该文章强调了这种隐写式水印标记与其他 AI 模型归因方法相比的持久性。

---

## 2. Claude Sonnet 5

**原文标题**: Claude Sonnet 5

**原文链接**: [https://www.anthropic.com/news/claude-sonnet-5](https://www.anthropic.com/news/claude-sonnet-5)

Anthropic has launched Claude Sonnet 5, touting it as their most agentic Sonnet model to date. It excels at making plans, using tools like browsers and terminals, and operating autonomously, achieving levels previously requiring larger, more expensive Opus-class models. Sonnet 5 significantly narrows the performance gap with Opus 4.8, offering comparable capabilities in reasoning, tool use, coding, and knowledge work at a lower price point than its predecessor, Sonnet 4.6.

Safety assessments show Sonnet 5 has an overall lower rate of undesirable behaviors than Sonnet 4.6, is better at refusing malicious requests, and exhibits lower hallucination and sycophancy. It was not deliberately trained on dangerous cybersecurity tasks, performing substantially poorer in exploit development than Opus 4.8, and launches with cyber safeguards enabled by default.

Sonnet 5 is available immediately across all Claude plans (Free, Pro, Max, Team, Enterprise), Claude Code, and the Claude Platform. It features introductory pricing of $2 per million input tokens and $10 per million output tokens through August 31, 2026, after which it will adjust to $3 and $15 respectively, making it highly cost-efficient compared to Opus 4.8 ($5 input, $25 output). Early access partners praised its ability to complete complex, multi-step tasks, self-correct, and follow through in demanding technical contexts.

---

## 3. Department of Commerce has lifted export controls on Claude Fable 5 and Mythos 5

**原文标题**: Department of Commerce has lifted export controls on Claude Fable 5 and Mythos 5

**原文链接**: [https://twitter.com/AnthropicAI/status/2072106151890809341](https://twitter.com/AnthropicAI/status/2072106151890809341)

生成摘要时出错

---

## 4. 欧洲数字身份钱包依赖谷歌和苹果的安全服务。

**原文标题**: European digital ID wallets rely on safety services of Google and Apple

**原文链接**: [https://waag.org/en/article/european-digital-id-wallets-are-gift-google-and-apple/](https://waag.org/en/article/european-digital-id-wallets-are-gift-google-and-apple/)

欧洲数字身份钱包旨在访问公共服务和在线年龄验证，其安全性关键依赖于Google的Play Integrity API和Apple的Managed Device Attestation。这些“远程证明”服务确保了应用程序的完整性，但根据文章，它们本质上强化了大型科技公司对数字生态系统的控制。

Google的Play Integrity API虽然被宣传为一项安全措施，但它会检查“真正的认证Android设备”，从而有效地排除了未经许可的Android版本，并强制要求应用程序通过Google Play商店使用Google账户安装。这种做法被视为违反了《数字市场法案》(DMA)，并与欧盟声明的数字自主和互操作性目标相悖。一个更开放、基于硬件的替代方案——Android的硬件证明API是可用的，但却常常被忽视。

通过整合这些服务，欧洲各国政府面临着巩固他们声称反对的垄断的风险。这种设计排除了“去谷歌化”操作系统的用户，迫使他们进入谷歌生态系统以获取基本公共服务，从而损害了开放性、包容性和技术主权等公共价值观。

尽管身份钱包是要求供应商独立的关键公共基础设施，但目前并没有统一的欧洲方法。欧盟的框架推荐谷歌证明，导致意大利和荷兰等国家实施了它，而瑞士等其他国家则因数据保护和选择自由的担忧而拒绝了它。

文章敦促欧盟强制采用开放的、基于硬件的证明机制，彻底排除谷歌和苹果。它呼吁公民、开发者和记者进行公开辩论、追究责任和采取行动，以防止大型科技公司权力进一步根深蒂固。

---

## 5. 美国大使让比利时警方停止了我们的报道。

**原文标题**: The US ambassador had Belgian police stop our reporting

**原文链接**: [https://europeancorrespondent.com/en/r/the-us-ambassador-had-belgian-police-stop-our-reporting](https://europeancorrespondent.com/en/r/the-us-ambassador-had-belgian-police-stop-our-reporting)

2026年6月29日，记者尤利乌斯·E·O·芬特尔曼和塞缪尔·登普西在布鲁塞尔“自由250”庆典上向美国大使比尔·怀特提问了一个据称他不喜欢的问题后，被比利时警方拘留并带离现场。

这场纪念美国建国250周年的活动由美国驻布鲁塞尔的三家大使馆私人出资并组织，在五十周年纪念公园（Parc du Cinquantenaire）举行。作为受邀媒体，记者们就塞缪尔·登普西此前发表的一篇关于大使据称威胁一名美国和比利时居民的报道向怀特大使提问。

大约20分钟后，八名比利时便衣警察将他们强行围住并带走。警官没收了他们的身份证件，并就他们所在出版物的政治议程对他们进行了审问，最初告知他们塞缪尔是一名“活跃的威胁”。尽管警方最终承认了错误并确认了记者们的证件，但美国大使馆指示警方将记者们完全护送离开现场。

次日，怀特大使拒绝澄清此事，称记者们为“失败者”。作者们谴责这一事件是对欧洲新闻自由的一次重大考验，对一个外国政府在一个被外国实体有效私有化的公共空间内，利用当地警方让持有证件的记者噤声表示担忧，并将比利时当局视为“本届特朗普政府的延伸”。

---

## 6. 大多数争论都关乎自我，而非思想。

**原文标题**: Most arguments are about ego, not ideas

**原文链接**: [https://wangcong.org/2026-06-30-why-i-stopped-arguing-with-people.html](https://wangcong.org/2026-06-30-why-i-stopped-arguing-with-people.html)

作者曾是一名软件工程师，最初认为可以通过逻辑和技术上的正确性来赢得争论。然而，他逐渐意识到这种方法是无效的，并且常常会疏远他人。他的转变源于几个关键的领悟：

1.  **正确性并非总是好事：** 赢得争论会制造一个失败者，从而产生抗拒而非理解。
2.  **争论常常关乎自我，而非观点本身：** 许多人将自己的观点等同于自我价值。挑战一个想法变成了人身攻击，导致防御性行为而非理性参与。必须区分与“聪明人”进行的建设性讨论和由自我驱动的争论。
3.  **人并非纯粹理性：** 人是情感动物，常会将已有的感受合理化。单凭逻辑无法动摇根深蒂固的信念。
4.  **未经请求的纠正鲜有帮助：** 即使是出于好意，批评也鲜少受到赞赏。人们通常从结果中学习，而非建议，除非他们明确请求帮助。
5.  **从差异中获益：** 与其试图说服，不如将分歧视为一种资产。立足于你独特的视角，让现实证明你的观点，尤其是在创业中。
6.  **你只能改变自己：** 试图改变他人的精力是浪费的。通过谦逊的自我反省和积极寻求反馈来专注于个人成长。一个需要获胜的自我会阻碍真正的学习和进步。

最终，作者停止了争论，转而优先考虑持续的自我提升，他认识到谦逊和学习的意愿远比“正确”更有价值。

---

## 7. 首次，从零构建的细胞实现生长与分裂

**原文标题**: For first time, a cell built from scratch grows and divides

**原文链接**: [https://www.quantamagazine.org/for-the-first-time-a-cell-built-from-scratch-grows-and-divides-20260701/](https://www.quantamagazine.org/for-the-first-time-a-cell-built-from-scratch-grows-and-divides-20260701/)

科学家们通过从零开始构建一个能够生长、复制DNA并分裂的合成细胞，取得了重大突破。在合成生物学家凯特·亚当拉（Kate Adamala）的带领下，这个被她的学生戏称为“土豆细胞”（spudcell）的细胞，是迄今为止最接近生命的人造细胞，它展示了细胞周期的基本功能，为在实验室中从非生命物质生成生命提供了关键的概念验证。

这个实验室制造的细胞并非在所有定义上都完全“活”着，因为它依赖于持续外部供应的食物、核糖体和其他复杂分子，并且缺乏防御机制或废物清除系统。然而，它生长和分裂的能力克服了该领域的一个长期挑战。亚当拉的团队通过修改一种膜蛋白，使其能够物理弯曲并分裂细胞，从而创新性地规避了对复杂细胞骨架（自然细胞用于分裂）的需求。

这一“惊人的技术成就”为生命的最低要求和生物学的起源提供了宝贵的见解。这些利用完整成分列表“从零开始”构建的细胞所展现出的灵活性，为未来制造生物燃料、药物或新型材料等应用打开了大门。尽管“土豆细胞”仍需要发展自我维持的新陈代谢和真正的进化能力，但它代表了合成生物学的一个“分水岭事件”，类似于生命系统中的“莱特飞行器”。为了促进进一步的研究，亚当拉的团队还成立了Biotic，一个旨在分享其工具和方法的非营利组织。

---

## 8. 克劳德科学

**原文标题**: Claude Science

**原文链接**: [https://claude.com/product/claude-science](https://claude.com/product/claude-science)

Claude Science 是一个全新的测试版应用程序，旨在作为严谨科学工作的综合研究伙伴，可在用户现有的基础设施（macOS/Linux）上运行。它使科学家能够运行分析、搜索数据库，并跟踪从数据整理到发表的每一步，旨在节省时间。

主要功能包括完全可重现的工作流程，其中每个产物（图表、表格、笔记本）都与其生成代码、环境和对话历史记录相关联。它提供用于蛋白质、结构、化学品和PDF的内置科学渲染器，以及一个后台审阅器，可标记不准确和不可追溯的数据。该应用程序支持迭代图形编辑、手稿起草（使用Markdown/LaTeX），并管理跨笔记本电脑、集群或GPU的计算。

Claude Science 预配置了基因组学、蛋白质组学和化学信息学等主要生命科学领域，连接到60多个科学数据库，并通过连接器与现有实验室工具、ELN（电子实验记录本）和流程管线集成。它因加速分析、确保可重现性以及促进复杂的科学任务而受到研究人员的赞扬。与通用人工智能不同，它作为一个完整的科学计算环境，通过本地运行来保护数据隐私。可在各种Claude套餐中使用，学术和非营利实验室可享受折扣。

---

## 9. Godot will no longer accept AI-authored code contributions

**原文标题**: Godot will no longer accept AI-authored code contributions

**原文链接**: [https://www.pcgamer.com/gaming-industry/open-source-game-engine-godot-will-no-longer-accept-ai-authored-code-contributions-we-cant-trust-heavy-users-of-ai-to-understand-their-code-enough-to-fix-it/](https://www.pcgamer.com/gaming-industry/open-source-game-engine-godot-will-no-longer-accept-ai-authored-code-contributions-we-cant-trust-heavy-users-of-ai-to-understand-their-code-enough-to-fix-it/)

生成摘要时出错

---

## 10. Asahi Linux 7.1 Progress Report

**原文标题**: Asahi Linux 7.1 Progress Report

**原文链接**: [https://asahilinux.org/2026/06/progress-report-7-1/](https://asahilinux.org/2026/06/progress-report-7-1/)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 2 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 3 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 4 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 5 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 6 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 7 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 8 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 9 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 10 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 11 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 12 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 13 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 14 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 15 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 16 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 17 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 18 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 19 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 20 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 21 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 22 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 23 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 24 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 25 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 26 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 27 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 28 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 29 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 30 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 31 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 32 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 33 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 34 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 35 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 36 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 37 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 38 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 39 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 40 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 41 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 42 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 43 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 44 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 45 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 46 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 47 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 48 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 49 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 50 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 51 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 52 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 53 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 54 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 55 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 56 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 57 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 58 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 59 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 60 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 61 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 62 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 63 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 64 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 65 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 66 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 67 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 68 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 69 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 70 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 71 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 72 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 73 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 74 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 75 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 76 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 77 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 78 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 79 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 80 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 81 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 82 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 83 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 84 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 85 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 86 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 87 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 88 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 89 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 90 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 91 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 92 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 93 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 94 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 95 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 96 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 97 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 98 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 99 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 100 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 101 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 102 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 103 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 104 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 105 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 106 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 107 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 108 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 109 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 110 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 111 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 112 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 113 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 114 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 115 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 116 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 117 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 118 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 119 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 120 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 121 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 122 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 123 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 124 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 125 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 126 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 127 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 128 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 129 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 130 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 131 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 132 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 133 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 134 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 135 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 136 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 137 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 138 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 139 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 140 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 141 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 142 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 143 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 144 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 145 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 146 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 147 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 148 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 149 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 150 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 151 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 152 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 153 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 154 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 155 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 156 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 157 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 158 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 159 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 160 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 161 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 162 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 163 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 164 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 165 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 166 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 167 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 168 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 169 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 170 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 171 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 172 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 173 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 174 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 175 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 176 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 177 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 178 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 179 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 180 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 181 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 182 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 183 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 184 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 185 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 186 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 187 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 188 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 189 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 190 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 191 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 192 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 193 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 194 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 195 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 196 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 197 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 198 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 199 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 200 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 201 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 202 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 203 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 204 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 205 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 206 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 207 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 208 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 209 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 210 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 211 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 212 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 213 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 214 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 215 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 216 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 217 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 218 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 219 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 220 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 221 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 222 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 223 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 224 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 225 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 226 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 227 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 228 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 229 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 230 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 231 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 232 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 233 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 234 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 235 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 236 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
