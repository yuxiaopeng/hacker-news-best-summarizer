# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-05-27.md)

*最后自动更新时间: 2026-05-27 21:29:03*
## 1. 我厌倦了和AI说话。

**原文标题**: I'm Tired of Talking to AI

**原文链接**: [https://orchidfiles.com/im-tired-of-ai-generated-answers/](https://orchidfiles.com/im-tired-of-ai-generated-answers/)

作者对与AI互动深感厌倦，尤其是在寻求真人输入时。他讲述了几个令人沮丧的经历来佐证这一点。

有一次，在发现传播恶意软件的GitHub仓库后，作者向AI查询却得到了无用的建议。当他随后在GitHub上发起讨论时，两个不同的人回复了*完全相同*的、AI生成且毫无帮助的文本，这表明他们缺乏原创思想。

类似地，在职场环境中，作为一名开发者的作者向一位企业主询问一项任务。该企业主回复了一个ChatGPT的截图，作者认为这既不相关也不正确。一分钟后，这位企业主又发送了*另一个*ChatGPT截图，显然没有阅读其内容。

作者还描述了最近在Reddit上的一次互动，经过几次交流后，他才意识到自己正在与一个AI代理对话。

这些经历让作者得出结论，他已经厌倦了与AI对话，渴望真正的真人互动。然而，即使在与人交流时，他也经常发现自己的问题被转交给了AI，而AI未经审查的答案随后又被转发回给他。

---

## 2. 用AI更缓慢地编写更好的代码

**原文标题**: Using AI to write better code more slowly

**原文链接**: [https://nolanlawson.com/2026/05/25/using-ai-to-write-better-code-more-slowly/](https://nolanlawson.com/2026/05/25/using-ai-to-write-better-code-more-slowly/)

Nolan Lawson argues against the common perception that AI coding tools are solely for generating low-quality code quickly. He posits that LLMs are highly effective for writing *high-quality code more slowly*, emphasizing their capability to identify numerous bugs.

Lawson details his workflow, which involves a custom "Claude skill" orchestrating multiple AI agents (like Claude, Codex, and Cursor Bugbot) to meticulously review Pull Requests (PRs). This multi-agent approach significantly reduces false positives, uncovering a wide range of bugs from critical security issues to minor code inconsistencies.

His process includes using agents to fix critical and high-priority bugs, selectively addressing others, and sometimes abandoning fundamentally flawed PRs. While this method doesn't necessarily accelerate development—often leading to "side-quests" to fix pre-existing issues—it profoundly improves codebase health and deepens the developer's understanding of complex systems.

Lawson advocates for this methodical, quality-obsessed approach, which he finds more satisfying and beneficial for long-term codebase maintainability. He encourages developers to embrace this slower, deliberate use of AI to write better code, even if it means sacrificing immediate "productivity" in terms of raw output.

---

## 3. 西班牙因缺乏赌博执照禁止Polymarket、Kalshi预测市场

**原文标题**: Spain blocks prediction markets Polymarket, Kalshi over lack of gambling licence

**原文链接**: [https://www.reuters.com/business/spain-blocks-prediction-markets-polymarket-kalshi-over-lack-gambling-licences-2026-05-26/](https://www.reuters.com/business/spain-blocks-prediction-markets-polymarket-kalshi-over-lack-gambling-licences-2026-05-26/)

生成摘要时出错

---

## 4. GitHub Actions 宕机了

**原文标题**: GitHub Actions was down

**原文链接**: [https://www.githubstatus.com/?today](https://www.githubstatus.com/?today)

GitHub Actions在2026年5月经历了多次性能下降和中断。

5月26日，Actions和Pages发生了一起事件，大约从10:57 UTC持续到13:18 UTC。这由认证问题引起，导致Actions运行的启动和下载失败，影响了大多数工作流。尽管某些相关内容，如Issues和PRs，被暂时隐藏，但没有数据丢失，问题通过缓解措施得以解决。

5月20日发生的另一起重大事件，导致GitHub Actions客户在16:00 UTC至17:45 UTC之间经历了运行启动延迟超过5分钟。大约4.5%的所有运行被延迟，其中规模化作业受影响尤为严重（30%延迟，4%失败）。根本原因是内部服务上的健康检查配置错误，导致区域集群发生连锁故障。通过扩容和重新平衡流量解决了问题。

早些时候，5月15日，Actions面临可用性下降，大约从07:43 UTC到08:48 UTC，导致工作流运行失败或延迟。在高峰期，42%的Actions运行失败。这归因于在计划的基础设施故障转移期间，自动化服务发现更新未能正确传播，影响了Pages和Copilot服务。人工干预纠正了路由问题，恢复了稳定性。

GitHub正在实施纠正措施，包括加强健康检查配置和提高依赖项弹性，以防止未来再次发生此类事件。

---

## 5. 我最糟糕的面试

**原文标题**: The worst job interview I ever had

**原文链接**: [https://www.oliverio.dev/blog/the-worst-job-interview-i-had](https://www.oliverio.dev/blog/the-worst-job-interview-i-had)

作者，一名工程师，讲述了他最糟糕的一次面试经历：为了一个心理健康初创公司的创始工程师职位，他接受了一次“未经请求的心理评估”。虽然他理解初创公司中文化契合度的重要性，但他认为这种特定的面试方式存在严重问题。

在一次初步的信息交流面试之后，他被安排参加一次90分钟的“非传统”文化契合度对话。这次对话包含“诱导创伤”的问题，涉及他最艰难的一天、最大的生活挑战、失败的人际关系和家庭困境。尽管他觉得这些问题具有侵犯性，他还是分享了个人细节，相信这是一个“安全空间”，而面试官却鲜有透露。作者在通话结束后感到心力交瘁，期间完全没有讨论任何技术技能。

二十四小时后，他收到了一封简短的拒信。这迅速将他的心力交瘁转变为羞耻和愤怒。他感到非常糟糕，因为分享了如此私密的个人信息，结果却因为“他这个人”而不是他的技术能力而被拒绝。令他尤为不解的是，一家心理健康初创公司竟会采用这种让应聘者感到如此脆弱的面试方式。作者最后呼吁招聘经理在评估文化契合度时，不应强迫应聘者为了获得一份工作而披露他们最深的创伤。

---

## 6. 研究发现：散步比久坐更能激发创造力 (2014)

**原文标题**: Taking a walk may lead to more creativity than sitting, study finds (2014)

**原文链接**: [https://www.apa.org/news/press/releases/2014/04/creativity-walk](https://www.apa.org/news/press/releases/2014/04/creativity-walk)

A 2014 study by Marily Oppezzo (Santa Clara University) and Daniel L. Schwartz (Stanford University) revealed that walking significantly enhances creative thinking compared to sitting. Published in the Journal of Experimental Psychology: Learning, Memory and Cognition, the research involved 176 college students.

Participants performed tasks such as generating alternative uses for common objects and creating original analogies. Across multiple experiments, those who walked—whether on a treadmill indoors or outdoors—consistently produced a higher number of creative and novel responses than those who remained seated or were pushed in a wheelchair. In one experiment, 100% of walkers generated more creative ideas.

Conversely, for tasks requiring focused concentration or a single correct answer, walkers performed slightly less effectively than their seated counterparts. The study highlighted that the physical act of walking itself, rather than the outdoor environment, was the primary factor in boosting creativity. Notably, even walking *before* a task showed a residual positive effect on creativity when participants subsequently sat down.

This research suggests that incorporating simple walks can be an "easy and productive" method to foster free-flowing thought and innovation, benefiting both cognitive function and work-related activities. Further studies are recommended to fully elucidate the complex physiological and cognitive pathways involved.

---

## 7. 荷兰阻止美国收购关键数字供应商

**原文标题**: Netherlands blocks US takeover of vital digital supplier

**原文链接**: [https://www.politico.eu/article/netherlands-blocks-us-takeover-vital-digital-supplier/](https://www.politico.eu/article/netherlands-blocks-us-takeover-vital-digital-supplier/)

荷兰政府阻止了美国公司Kyndryl收购一家重要的荷兰数字供应商Solvinity。Solvinity运营着荷兰国家在线身份识别应用DigiD的平台，公民使用DigiD来验证身份，以获取预约医生或与公共机构互动等基本服务。

此次收购被叫停，原因是对一个重要的国家身份识别工具将落入外国控制之下表示担忧，这构成“对公共利益的潜在风险”。数字经济国务秘书Willemijn Aerdts在听取了国家投资审查机构的建议后宣布了这一决定。

尽管荷兰重视外国科技公司，但它维持着一个独立的投资审查框架，以保护公共利益，适用于所有投资者。此举与欧洲日益增长的对欧盟依赖美国技术的担忧相吻合，并且早于欧盟委员会即将出台的旨在减少在云计算、微芯片和人工智能等领域依赖的“技术主权一揽子计划”。

Kyndryl对此表示极度失望，声称这一过程被“政治化”，并掩盖了此次交易的益处。

---

## 8. Big tech's anti-labor playbook has come for Wikipedia

**原文标题**: Big tech's anti-labor playbook has come for Wikipedia

**原文链接**: [https://medium.com/@jakeorlowitz/wikipedia-is-doing-the-capitalist-thing-56a393232943](https://medium.com/@jakeorlowitz/wikipedia-is-doing-the-capitalist-thing-56a393232943)

生成摘要时出错

---

## 9. Last.fm is now independent

**原文标题**: Last.fm is now independent

**原文链接**: [https://support.last.fm/t/last-fm-is-now-independent/118591](https://support.last.fm/t/last-fm-is-now-independent/118591)

生成摘要时出错

---

## 10. Ferrari Luce

**原文标题**: Ferrari Luce

**原文链接**: [https://www.ferrari.com/en-EN/auto/ferrari-luce](https://www.ferrari.com/en-EN/auto/ferrari-luce)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 2 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 3 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 4 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 5 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 6 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 7 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 8 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 9 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 10 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 11 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 12 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 13 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 14 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 15 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 16 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 17 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 18 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 19 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 20 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 21 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 22 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 23 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 24 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 25 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 26 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 27 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 28 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 29 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 30 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 31 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 32 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 33 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 34 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 35 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 36 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 37 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 38 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 39 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 40 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 41 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 42 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 43 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 44 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 45 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 46 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 47 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 48 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 49 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 50 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 51 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 52 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 53 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 54 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 55 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 56 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 57 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 58 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 59 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 60 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 61 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 62 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 63 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 64 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 65 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 66 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 67 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 68 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 69 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 70 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 71 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 72 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 73 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 74 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 75 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 76 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 77 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 78 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 79 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 80 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 81 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 82 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 83 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 84 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 85 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 86 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 87 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 88 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 89 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 90 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 91 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 92 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 93 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 94 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 95 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 96 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 97 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 98 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 99 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 100 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 101 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 102 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 103 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 104 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 105 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 106 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 107 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 108 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 109 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 110 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 111 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 112 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 113 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 114 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 115 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 116 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 117 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 118 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 119 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 120 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 121 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 122 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 123 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 124 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 125 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 126 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 127 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 128 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 129 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 130 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 131 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 132 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 133 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 134 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 135 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 136 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 137 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 138 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 139 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 140 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 141 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 142 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 143 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 144 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 145 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 146 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 147 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 148 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 149 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 150 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 151 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 152 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 153 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 154 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 155 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 156 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 157 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 158 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 159 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 160 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 161 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 162 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 163 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 164 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 165 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 166 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 167 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 168 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 169 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 170 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 171 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 172 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 173 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 174 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 175 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 176 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 177 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 178 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 179 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 180 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 181 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 182 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 183 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 184 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 185 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 186 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 187 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 188 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 189 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 190 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 191 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 192 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 193 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 194 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 195 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 196 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 197 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 198 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 199 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 200 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 201 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
