# Hacker News 热门文章摘要 (2026-07-01)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

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

## 11. The labor share of income in the US is at its lowest post-war level

**原文标题**: The labor share of income in the US is at its lowest post-war level

**原文链接**: [https://libertystreeteconomics.newyorkfed.org/2026/06/the-post-covid-decline-in-the-labor-share/](https://libertystreeteconomics.newyorkfed.org/2026/06/the-post-covid-decline-in-the-labor-share/)

生成摘要时出错

---

## 12. Nintendo has raised its employees base salary by 10%

**原文标题**: Nintendo has raised its employees base salary by 10%

**原文链接**: [https://mynintendonews.com/2026/06/26/nintendo-has-raised-its-employees-base-salary-by-10/](https://mynintendonews.com/2026/06/26/nintendo-has-raised-its-employees-base-salary-by-10/)

生成摘要时出错

---

## 13. Physical disc production ending in Jan 2028 for new games on PlayStation

**原文标题**: Physical disc production ending in Jan 2028 for new games on PlayStation

**原文链接**: [https://blog.playstation.com/2026/07/01/physical-disc-production-ending-in-january-2028-for-new-games-releasing-on-playstation-consoles/](https://blog.playstation.com/2026/07/01/physical-disc-production-ending-in-january-2028-for-new-games-releasing-on-playstation-consoles/)

生成摘要时出错

---

## 14. Nano Banana 2 Lite

**原文标题**: Nano Banana 2 Lite

**原文链接**: [https://deepmind.google/models/gemini-image/flash-lite/](https://deepmind.google/models/gemini-image/flash-lite/)

生成摘要时出错

---

## 15. County with 37 Data Centers Asks Schools to 'Conserve Electricity'

**原文标题**: County with 37 Data Centers Asks Schools to 'Conserve Electricity'

**原文链接**: [https://www.404media.co/henrico-virginia-datacenter-energy-cost-email/](https://www.404media.co/henrico-virginia-datacenter-energy-cost-email/)

生成摘要时出错

---

## 16. Sony Deletes 551 Movies PlayStation Owners Paid For

**原文标题**: Sony Deletes 551 Movies PlayStation Owners Paid For

**原文链接**: [https://reclaimthenet.org/sony-deletes-551-studiocanal-movies-playstation-owners-paid-for](https://reclaimthenet.org/sony-deletes-551-studiocanal-movies-playstation-owners-paid-for)

生成摘要时出错

---

## 17. Frog-derived gut bacterium eradicates tumors in mice

**原文标题**: Frog-derived gut bacterium eradicates tumors in mice

**原文链接**: [https://www.thefocalpoints.com/p/new-study-frog-derived-gut-bacterium](https://www.thefocalpoints.com/p/new-study-frog-derived-gut-bacterium)

生成摘要时出错

---

## 18. Box3D, an open source 3D physics engine

**原文标题**: Box3D, an open source 3D physics engine

**原文链接**: [https://box2d.org/posts/2026/06/announcing-box3d/](https://box2d.org/posts/2026/06/announcing-box3d/)

生成摘要时出错

---

## 19. Knoppix

**原文标题**: Knoppix

**原文链接**: [https://www.knopper.net/knoppix/index-en.html](https://www.knopper.net/knoppix/index-en.html)

生成摘要时出错

---

## 20. I ported Kubernetes to the browser

**原文标题**: I ported Kubernetes to the browser

**原文链接**: [https://ngrok.com/blog/i-ported-kubernetes-to-the-browser](https://ngrok.com/blog/i-ported-kubernetes-to-the-browser)

生成摘要时出错

---

## 21. We Are the Last People Who Know How It Works

**原文标题**: We Are the Last People Who Know How It Works

**原文链接**: [https://unix.foo/posts/last-people-who-know-how-it-works/](https://unix.foo/posts/last-people-who-know-how-it-works/)

生成摘要时出错

---

## 22. Leanstral 1.5

**原文标题**: Leanstral 1.5

**原文链接**: [https://docs.mistral.ai/models/model-cards/leanstral-1-5-26-06](https://docs.mistral.ai/models/model-cards/leanstral-1-5-26-06)

生成摘要时出错

---

## 23. Google copybara: moving code between repositories

**原文标题**: Google copybara: moving code between repositories

**原文链接**: [https://github.com/google/copybara](https://github.com/google/copybara)

生成摘要时出错

---

## 24. LongCat-2.0, a large-scale MoE model with 1.6T total and 48B Active

**原文标题**: LongCat-2.0, a large-scale MoE model with 1.6T total and 48B Active

**原文链接**: [https://longcat.chat/blog/longcat-2.0/](https://longcat.chat/blog/longcat-2.0/)

生成摘要时出错

---

## 25. ArXiv's Next Chapter

**原文标题**: ArXiv's Next Chapter

**原文链接**: [https://blog.arxiv.org/2026/06/30/arxivs-next-chapter/](https://blog.arxiv.org/2026/06/30/arxivs-next-chapter/)

生成摘要时出错

---

## 26. South Korea to spend $1T on more memory chip production and humanoid robots

**原文标题**: South Korea to spend $1T on more memory chip production and humanoid robots

**原文链接**: [https://arstechnica.com/ai/2026/06/south-korea-to-spend-1t-on-more-memory-chip-production-and-humanoid-robots/](https://arstechnica.com/ai/2026/06/south-korea-to-spend-1t-on-more-memory-chip-production-and-humanoid-robots/)

生成摘要时出错

---

## 27. A retrospective of my time on the internet

**原文标题**: A retrospective of my time on the internet

**原文链接**: [https://cleberg.net/blog/internet.html](https://cleberg.net/blog/internet.html)

生成摘要时出错

---

## 28. US Supreme Court Just Blew Up EU-US Data Transfers

**原文标题**: US Supreme Court Just Blew Up EU-US Data Transfers

**原文链接**: [https://noyb.eu/en/us-supreme-court-just-blew-eu-us-data-transfers](https://noyb.eu/en/us-supreme-court-just-blew-eu-us-data-transfers)

生成摘要时出错

---

## 29. Crypto firms have spent $189M so far on 2026 US election, report says

**原文标题**: Crypto firms have spent $189M so far on 2026 US election, report says

**原文链接**: [https://www.reuters.com/world/crypto-firms-have-spent-189-million-so-far-2026-us-election-report-says-2026-06-30/](https://www.reuters.com/world/crypto-firms-have-spent-189-million-so-far-2026-us-election-report-says-2026-06-30/)

生成摘要时出错

---

## 30. Internal Combustion Engine

**原文标题**: Internal Combustion Engine

**原文链接**: [https://ciechanow.ski/internal-combustion-engine/](https://ciechanow.ski/internal-combustion-engine/)

生成摘要时出错

---

## 31. Supreme Court upholds broad conception of birthright citizenship

**原文标题**: Supreme Court upholds broad conception of birthright citizenship

**原文链接**: [https://apnews.com/live/birthright-citizenship-decision-supreme-court-updates-06-30-2026](https://apnews.com/live/birthright-citizenship-decision-supreme-court-updates-06-30-2026)

生成摘要时出错

---

## 32. Looking Ahead to Postgres 19

**原文标题**: Looking Ahead to Postgres 19

**原文链接**: [https://www.snowflake.com/en/blog/engineering/postgresql-19-features-beta/](https://www.snowflake.com/en/blog/engineering/postgresql-19-features-beta/)

生成摘要时出错

---

## 33. Have you restarted your computer this week?

**原文标题**: Have you restarted your computer this week?

**原文链接**: [https://taonaw.com/2026/06/27/have-you-restarted-your-computer.html](https://taonaw.com/2026/06/27/have-you-restarted-your-computer.html)

生成摘要时出错

---

## 34. Memory Safe Context Switching

**原文标题**: Memory Safe Context Switching

**原文链接**: [https://fil-c.org/context_switches](https://fil-c.org/context_switches)

生成摘要时出错

---

## 35. Apple 'Hide My Email' vulnerability reveals peoples' real email addresses

**原文标题**: Apple 'Hide My Email' vulnerability reveals peoples' real email addresses

**原文链接**: [https://easyoptouts.com/guides/apple-hide-my-email-is-leaking-email-addresses](https://easyoptouts.com/guides/apple-hide-my-email-is-leaking-email-addresses)

生成摘要时出错

---

## 36. Exercise intensity influences body composition in healthy older adults (2025)

**原文标题**: Exercise intensity influences body composition in healthy older adults (2025)

**原文链接**: [https://www.maturitas.org/article/S0378-5122(25)00571-7/fulltext](https://www.maturitas.org/article/S0378-5122(25)00571-7/fulltext)

生成摘要时出错

---

## 37. I built a mmWave material classification radar (2025)

**原文标题**: I built a mmWave material classification radar (2025)

**原文链接**: [https://gauthier-lechevalier.com/radar](https://gauthier-lechevalier.com/radar)

生成摘要时出错

---

## 38. Trump made more than $1B on crypto deals, part of 2025 windfall

**原文标题**: Trump made more than $1B on crypto deals, part of 2025 windfall

**原文链接**: [https://www.wsj.com/politics/policy/trump-made-more-than-1-billion-on-crypto-deals-part-of-2025-windfall-ee917d3f](https://www.wsj.com/politics/policy/trump-made-more-than-1-billion-on-crypto-deals-part-of-2025-windfall-ee917d3f)

生成摘要时出错

---

## 39. Popping the GPU Bubble

**原文标题**: Popping the GPU Bubble

**原文链接**: [https://moondream.ai/blog/popping-the-gpu-bubble](https://moondream.ai/blog/popping-the-gpu-bubble)

生成摘要时出错

---

## 40. Monetization Gateway

**原文标题**: Monetization Gateway

**原文链接**: [https://blog.cloudflare.com/monetization-gateway/](https://blog.cloudflare.com/monetization-gateway/)

生成摘要时出错

---

## 41. Memoirs of Extraordinary Popular Delusions and the Madness of Crowds (1852)

**原文标题**: Memoirs of Extraordinary Popular Delusions and the Madness of Crowds (1852)

**原文链接**: [https://www.gutenberg.org/ebooks/24518](https://www.gutenberg.org/ebooks/24518)

生成摘要时出错

---

## 42. Sony erases digital content from libraries

**原文标题**: Sony erases digital content from libraries

**原文链接**: [https://arstechnica.com/gadgets/2026/06/sony-erases-digital-content-from-libraries-were-reminded-we-dont-own-what-we-buy/](https://arstechnica.com/gadgets/2026/06/sony-erases-digital-content-from-libraries-were-reminded-we-dont-own-what-we-buy/)

生成摘要时出错

---

## 43. From brain waves to words: a new path to communication without surgery

**原文标题**: From brain waves to words: a new path to communication without surgery

**原文链接**: [https://ai.meta.com/blog/brain2qwerty-brain-ai-human-communication/?_fb_noscript=1](https://ai.meta.com/blog/brain2qwerty-brain-ai-human-communication/?_fb_noscript=1)

生成摘要时出错

---

## 44. ZCode: Claude Code from the Makers of GLM

**原文标题**: ZCode: Claude Code from the Makers of GLM

**原文链接**: [https://zcode.z.ai/cn](https://zcode.z.ai/cn)

生成摘要时出错

---

## 45. FFmpeg 9.1's new AAC encoder

**原文标题**: FFmpeg 9.1's new AAC encoder

**原文链接**: [https://hydrogenaudio.org/index.php/topic,129691.0.html](https://hydrogenaudio.org/index.php/topic,129691.0.html)

生成摘要时出错

---

## 46. The first early human eggs from stem cells

**原文标题**: The first early human eggs from stem cells

**原文链接**: [https://www.conception.bio/science-and-updates/the-first-early-human-eggs-from-stem-cells](https://www.conception.bio/science-and-updates/the-first-early-human-eggs-from-stem-cells)

生成摘要时出错

---

## 47. Redeploying Fable 5

**原文标题**: Redeploying Fable 5

**原文链接**: [https://www.anthropic.com/news/redeploying-fable-5](https://www.anthropic.com/news/redeploying-fable-5)

生成摘要时出错

---

## 48. Tokyo has only two barley tea makers, we visited one to see how mugicha is made

**原文标题**: Tokyo has only two barley tea makers, we visited one to see how mugicha is made

**原文链接**: [https://soranews24.com/2026/06/30/tokyo-has-only-two-barley-tea-makers-and-we-visited-one-to-see-how-mugicha-is-made/](https://soranews24.com/2026/06/30/tokyo-has-only-two-barley-tea-makers-and-we-visited-one-to-see-how-mugicha-is-made/)

生成摘要时出错

---

## 49. Zluda 6 release (run unmodified CUDA applications on non-Nvidia GPUs)

**原文标题**: Zluda 6 release (run unmodified CUDA applications on non-Nvidia GPUs)

**原文链接**: [https://vosen.github.io/ZLUDA/blog/zluda-update-q1q2-2026/](https://vosen.github.io/ZLUDA/blog/zluda-update-q1q2-2026/)

生成摘要时出错

---

## 50. Fable 5 Is Back

**原文标题**: Fable 5 Is Back

**原文链接**: [https://twitter.com/claudeai/status/2072402636813607381](https://twitter.com/claudeai/status/2072402636813607381)

生成摘要时出错

---

## 51. Meta loses bid to dismiss US states' claims that FB, Instagram addict children

**原文标题**: Meta loses bid to dismiss US states' claims that FB, Instagram addict children

**原文链接**: [https://www.reuters.com/legal/government/meta-loses-bid-dismiss-us-states-claims-that-facebook-instagram-addict-children-2026-06-30/](https://www.reuters.com/legal/government/meta-loses-bid-dismiss-us-states-claims-that-facebook-instagram-addict-children-2026-06-30/)

生成摘要时出错

---

## 52. Amazon seller reveals glimpse of shadow bribery market

**原文标题**: Amazon seller reveals glimpse of shadow bribery market

**原文链接**: [https://www.latimes.com/business/story/2026-06-30/shadow-bribery-market-inside-amazon-preys-on-desperate-sellers](https://www.latimes.com/business/story/2026-06-30/shadow-bribery-market-inside-amazon-preys-on-desperate-sellers)

生成摘要时出错

---

## 53. We moved our Bluesky data to Eurosky

**原文标题**: We moved our Bluesky data to Eurosky

**原文链接**: [https://waag.org/en/article/why-we-moved-our-bluesky-data-eurosky/](https://waag.org/en/article/why-we-moved-our-bluesky-data-eurosky/)

生成摘要时出错

---

## 54. EU commissioners shut down air conditioning for employees, leave theirs on

**原文标题**: EU commissioners shut down air conditioning for employees, leave theirs on

**原文链接**: [https://www.politico.eu/article/eu-commission-heatwave-hq-forced-shut-down-air-conditioning-europe/](https://www.politico.eu/article/eu-commission-heatwave-hq-forced-shut-down-air-conditioning-europe/)

生成摘要时出错

---

## 55. What to Learn to Be a Graphics Programmer

**原文标题**: What to Learn to Be a Graphics Programmer

**原文链接**: [https://blog.demofox.org/2026/07/01/what-to-learn-to-be-a-graphics-programmer/](https://blog.demofox.org/2026/07/01/what-to-learn-to-be-a-graphics-programmer/)

生成摘要时出错

---

## 56. Xsnow "protestware" in Debian

**原文标题**: Xsnow "protestware" in Debian

**原文链接**: [https://lwn.net/SubscriberLink/1079385/3d7a57da58b41aa9/](https://lwn.net/SubscriberLink/1079385/3d7a57da58b41aa9/)

生成摘要时出错

---

## 57. Parse, Don't Validate – In a Language That Doesn't Want You To

**原文标题**: Parse, Don't Validate – In a Language That Doesn't Want You To

**原文链接**: [https://cekrem.github.io/posts/parse-dont-validate-typescript/](https://cekrem.github.io/posts/parse-dont-validate-typescript/)

生成摘要时出错

---

## 58. Pine64 launch $50 smart speaker for Home Assistant tinkerers

**原文标题**: Pine64 launch $50 smart speaker for Home Assistant tinkerers

**原文链接**: [https://www.omgubuntu.co.uk/2026/06/pine64-pinevoice-riscv-smart-speaker-launch](https://www.omgubuntu.co.uk/2026/06/pine64-pinevoice-riscv-smart-speaker-launch)

生成摘要时出错

---

## 59. Swedish court says Google is to pay $1.5B to Klarna in antitrust damages

**原文标题**: Swedish court says Google is to pay $1.5B to Klarna in antitrust damages

**原文链接**: [https://www.reuters.com/business/swedish-court-says-google-is-pay-15-billion-klarna-antitrust-damages-2026-07-01/](https://www.reuters.com/business/swedish-court-says-google-is-pay-15-billion-klarna-antitrust-damages-2026-07-01/)

生成摘要时出错

---

## 60. How We Made IPFS Content Publishing 10x Faster

**原文标题**: How We Made IPFS Content Publishing 10x Faster

**原文链接**: [https://probelab.io/blog/optimistic-provide/](https://probelab.io/blog/optimistic-provide/)

生成摘要时出错

---

## 61. Study suggests most Americans would be healthier without daylight saving time (2025)

**原文标题**: Study suggests most Americans would be healthier without daylight saving time (2025)

**原文链接**: [https://med.stanford.edu/news/all-news/2025/09/daylight-saving-time.html](https://med.stanford.edu/news/all-news/2025/09/daylight-saving-time.html)

生成摘要时出错

---

## 62. Exploring PDP-1 Lisp (1960)

**原文标题**: Exploring PDP-1 Lisp (1960)

**原文链接**: [https://obsolescence.dev/pdp1-lisp-introduction.html](https://obsolescence.dev/pdp1-lisp-introduction.html)

生成摘要时出错

---

## 63. Scientists find molecular-level evidence for two structures in liquid water

**原文标题**: Scientists find molecular-level evidence for two structures in liquid water

**原文链接**: [https://phys.org/news/2026-06-scientists-molecular-evidence-liquid.html](https://phys.org/news/2026-06-scientists-molecular-evidence-liquid.html)

生成摘要时出错

---

## 64. The Anti-Palantir Manifesto

**原文标题**: The Anti-Palantir Manifesto

**原文链接**: [https://nym.com/blog/anti-palantir-manifesto](https://nym.com/blog/anti-palantir-manifesto)

生成摘要时出错

---

## 65. Google's New reCAPTCHA Wants Your Camera Access and 21 Points of Your Hand

**原文标题**: Google's New reCAPTCHA Wants Your Camera Access and 21 Points of Your Hand

**原文链接**: [https://reclaimthenet.org/googles-new-recaptcha-wants-your-camera-access-and-21-points-of-your-hand](https://reclaimthenet.org/googles-new-recaptcha-wants-your-camera-access-and-21-points-of-your-hand)

生成摘要时出错

---

## 66. The end of my AArch64 desktop experiment

**原文标题**: The end of my AArch64 desktop experiment

**原文链接**: [https://marcin.juszkiewicz.com.pl/2026/06/26/the-end-of-the-aarch64-desktop-experiment/](https://marcin.juszkiewicz.com.pl/2026/06/26/the-end-of-the-aarch64-desktop-experiment/)

生成摘要时出错

---

## 67. Forestiere Underground Gardens

**原文标题**: Forestiere Underground Gardens

**原文链接**: [https://en.wikipedia.org/wiki/Forestiere_Underground_Gardens](https://en.wikipedia.org/wiki/Forestiere_Underground_Gardens)

生成摘要时出错

---

## 68. Words Are a Byproduct of Consciousness. For LLMs, It's Backwards

**原文标题**: Words Are a Byproduct of Consciousness. For LLMs, It's Backwards

**原文链接**: [https://ranpara.net/posts/words-are-a-byproduct-of-consciousness/](https://ranpara.net/posts/words-are-a-byproduct-of-consciousness/)

生成摘要时出错

---

## 69. TabFM: A zero-shot foundation model for tabular data

**原文标题**: TabFM: A zero-shot foundation model for tabular data

**原文链接**: [https://research.google/blog/introducing-tabfm-a-zero-shot-foundation-model-for-tabular-data/](https://research.google/blog/introducing-tabfm-a-zero-shot-foundation-model-for-tabular-data/)

生成摘要时出错

---

## 70. Supreme Court takes sledgehammer to federal regulatory structure

**原文标题**: Supreme Court takes sledgehammer to federal regulatory structure

**原文链接**: [https://www.npr.org/2026/06/29/nx-s1-5875161/supreme-court-takes-sledgehammer-to-much-of-federal-governments-regulatory-structure](https://www.npr.org/2026/06/29/nx-s1-5875161/supreme-court-takes-sledgehammer-to-much-of-federal-governments-regulatory-structure)

生成摘要时出错

---

## 71. SpudCell: The first synthetic cell with a complete cell cycle

**原文标题**: SpudCell: The first synthetic cell with a complete cell cycle

**原文链接**: [https://biotic.org/research/spudcell/](https://biotic.org/research/spudcell/)

生成摘要时出错

---

## 72. Sony will no longer produce discs for PlayStation games starting in January 2028

**原文标题**: Sony will no longer produce discs for PlayStation games starting in January 2028

**原文链接**: [https://www.eurogamer.net/sony-ending-playstation-discs-physical-media-january-2028](https://www.eurogamer.net/sony-ending-playstation-discs-physical-media-january-2028)

生成摘要时出错

---

## 73. Hatari – Online Atari ST/STE/TT/Falcon Emulator

**原文标题**: Hatari – Online Atari ST/STE/TT/Falcon Emulator

**原文链接**: [https://hatari.frama.io/hatari/online/hatari.html](https://hatari.frama.io/hatari/online/hatari.html)

生成摘要时出错

---

## 74. Your Kids' School Bus Is About to Become a Roaming Surveillance Vehicle

**原文标题**: Your Kids' School Bus Is About to Become a Roaming Surveillance Vehicle

**原文链接**: [https://www.thedrive.com/news/your-kids-school-bus-is-about-to-become-a-roaming-surveillance-vehicle](https://www.thedrive.com/news/your-kids-school-bus-is-about-to-become-a-roaming-surveillance-vehicle)

生成摘要时出错

---

## 75. Matrix Orthogonalization Improves Memory in Recurrent Models

**原文标题**: Matrix Orthogonalization Improves Memory in Recurrent Models

**原文链接**: [https://ayushtambde.com/blog/matrix-orthogonalization-improves-memory-in-recurrent-models/](https://ayushtambde.com/blog/matrix-orthogonalization-improves-memory-in-recurrent-models/)

生成摘要时出错

---

## 76. Antares achieves criticality of Mark-0 reactor

**原文标题**: Antares achieves criticality of Mark-0 reactor

**原文链接**: [https://antaresindustries.com/updates/antares-achieves-criticality](https://antaresindustries.com/updates/antares-achieves-criticality)

生成摘要时出错

---

## 77. Supersonic flight returning to US after half-century ban

**原文标题**: Supersonic flight returning to US after half-century ban

**原文链接**: [https://www.forbes.com/sites/suzannerowankelleher/2026/06/30/faa-supersonic-flight-no-boom/](https://www.forbes.com/sites/suzannerowankelleher/2026/06/30/faa-supersonic-flight-no-boom/)

生成摘要时出错

---

## 78. Show HN: My 13-year-old built an ant colony tracker

**原文标题**: Show HN: My 13-year-old built an ant colony tracker

**原文链接**: [https://formicarium.es](https://formicarium.es)

生成摘要时出错

---

## 79. Single header Parser Combinators for C

**原文标题**: Single header Parser Combinators for C

**原文链接**: [https://github.com/steve-chavez/CParseC](https://github.com/steve-chavez/CParseC)

生成摘要时出错

---

## 80. Red Programming Language: Static linking support

**原文标题**: Red Programming Language: Static linking support

**原文链接**: [https://www.red-lang.org/2026/06/static-linking-support.html](https://www.red-lang.org/2026/06/static-linking-support.html)

生成摘要时出错

---

## 81. Claude Fable 5 export control lifted

**原文标题**: Claude Fable 5 export control lifted

**原文链接**: [https://twitter.com/synthwavedd/status/2072103052635451559](https://twitter.com/synthwavedd/status/2072103052635451559)

生成摘要时出错

---

## 82. Claude Fable 5 Promotional Access

**原文标题**: Claude Fable 5 Promotional Access

**原文链接**: [https://support.claude.com/en/articles/15424964-claude-fable-5-promotional-access](https://support.claude.com/en/articles/15424964-claude-fable-5-promotional-access)

生成摘要时出错

---

## 83. Supreme Court strikes down limits on party spending in federal elections

**原文标题**: Supreme Court strikes down limits on party spending in federal elections

**原文链接**: [https://apnews.com/article/supreme-court-campaign-finance-party-spending-ohio-91e49ee112197ae1210a9abfa46986ed](https://apnews.com/article/supreme-court-campaign-finance-party-spending-ohio-91e49ee112197ae1210a9abfa46986ed)

生成摘要时出错

---

## 84. Fixing a kubelet memory leak in Kubernetes 1.36

**原文标题**: Fixing a kubelet memory leak in Kubernetes 1.36

**原文链接**: [https://heyoncall.com/blog/fixing-kubernetes-kubelet-memory-leak](https://heyoncall.com/blog/fixing-kubernetes-kubelet-memory-leak)

生成摘要时出错

---

## 85. Anthropic restoring access to Claude Fable 5 and Mythos 5 from tomorrow

**原文标题**: Anthropic restoring access to Claude Fable 5 and Mythos 5 from tomorrow

**原文链接**: [https://twitter.com/AnthropicAI/status/2072106151890809341](https://twitter.com/AnthropicAI/status/2072106151890809341)

生成摘要时出错

---

## 86. Claude Code Just Got 5x More Expensive

**原文标题**: Claude Code Just Got 5x More Expensive

**原文链接**: [https://www.vincentschmalbach.com/claude-code-quietly-looks-5x-more-expensive/](https://www.vincentschmalbach.com/claude-code-quietly-looks-5x-more-expensive/)

Anthropic has quietly implemented a significant pricing change for its Claude models, specifically impacting developers utilizing "tool use" or "function calling" features. Previously, the `tool_use` content block—which contains the arguments for external function calls made by the model—was not charged, making it effectively free.

The article highlights that Anthropic has now updated its pricing structure to charge for these `tool_use` blocks as output tokens. This means that for applications heavily reliant on Claude's ability to call tools, costs can increase substantially. The author presents an example where the number of tokens in the `tool_use` block exceeded regular output tokens, suggesting a potential "5x more expensive" scenario for such interactions.

Furthermore, `tool_result` blocks, which contain the results returned from the external tools, are now also charged as input tokens. This adjustment aligns Claude's tool-use pricing more closely with industry standards, particularly OpenAI's function calling, which has always charged for tool argument tokens.

The change, introduced without a prominent announcement, has raised concerns among developers who built applications around the previously free `tool_use` behavior, leading to unexpected cost increases.

---

## 87. Anthropic has embedded hidden spyware-like code in Claude Code

**原文标题**: Anthropic has embedded hidden spyware-like code in Claude Code

**原文链接**: [https://twitter.com/IntCyberDigest/status/2071971609183678544](https://twitter.com/IntCyberDigest/status/2071971609183678544)

生成摘要时出错

---

## 88. Meta is adding rate limits and soft paywall to smart glasses

**原文标题**: Meta is adding rate limits and soft paywall to smart glasses

**原文链接**: [https://www.theverge.com/gadgets/959899/meta-ai-glasses-paywall-rate-limit](https://www.theverge.com/gadgets/959899/meta-ai-glasses-paywall-rate-limit)

生成摘要时出错

---

## 89. How employment changes when firms adopt generative AI

**原文标题**: How employment changes when firms adopt generative AI

**原文链接**: [https://ramp.com/data/ai-jobs-impact](https://ramp.com/data/ai-jobs-impact)

生成摘要时出错

---

## 90. Claude Desktop is now available on Linux (in beta)

**原文标题**: Claude Desktop is now available on Linux (in beta)

**原文链接**: [https://code.claude.com/docs/en/desktop-linux](https://code.claude.com/docs/en/desktop-linux)

生成摘要时出错

---

## 91. Scammers Sell Seeds for Exotic AI-Generated Flowers That Don't Exist

**原文标题**: Scammers Sell Seeds for Exotic AI-Generated Flowers That Don't Exist

**原文链接**: [https://www.404media.co/scammers-sell-seeds-for-exotic-ai-generated-flowers-that-dont-exist/](https://www.404media.co/scammers-sell-seeds-for-exotic-ai-generated-flowers-that-dont-exist/)

生成摘要时出错

---

## 92. Building Gin: Simple over Easy

**原文标题**: Building Gin: Simple over Easy

**原文链接**: [https://manualmeida.dev/articles/gin-simple-over-easy/](https://manualmeida.dev/articles/gin-simple-over-easy/)

生成摘要时出错

---

## 93. From Julia to Rust: a differentiable tensor stack for scientific computing

**原文标题**: From Julia to Rust: a differentiable tensor stack for scientific computing

**原文链接**: [https://tensor4all.org/blog/introducing-tenferro-rs/](https://tensor4all.org/blog/introducing-tenferro-rs/)

生成摘要时出错

---

## 94. Claude Fable 5 available globally tomorrow

**原文标题**: Claude Fable 5 available globally tomorrow

**原文链接**: [https://twitter.com/anthropicai/status/2072163884430229756](https://twitter.com/anthropicai/status/2072163884430229756)

生成摘要时出错

---

## 95. Ray Tracer in SQL

**原文标题**: Ray Tracer in SQL

**原文链接**: [https://github.com/ClickHouse/RayTracer](https://github.com/ClickHouse/RayTracer)

生成摘要时出错

---

## 96. Morbid: Debunking Modern Longevity Science

**原文标题**: Morbid: Debunking Modern Longevity Science

**原文链接**: [https://www.newyorker.com/magazine/2026/07/06/morbid-saul-justin-newman-book-review-eat-your-ice-cream-ezekiel-j-emanuel](https://www.newyorker.com/magazine/2026/07/06/morbid-saul-justin-newman-book-review-eat-your-ice-cream-ezekiel-j-emanuel)

生成摘要时出错

---

## 97. America can switch off AI. Europe must switch gears before it's too late

**原文标题**: America can switch off AI. Europe must switch gears before it's too late

**原文链接**: [https://www.euronews.com/my-europe/2026/06/30/america-can-switch-off-the-worlds-ai-europe-must-switch-gears-before-its-too-late](https://www.euronews.com/my-europe/2026/06/30/america-can-switch-off-the-worlds-ai-europe-must-switch-gears-before-its-too-late)

生成摘要时出错

---

## 98. Is It Out Yet?

**原文标题**: Is It Out Yet?

**原文链接**: [https://outyet.ai](https://outyet.ai)

生成摘要时出错

---

## 99. Solid and Clean Code never felt solid or clean to me

**原文标题**: Solid and Clean Code never felt solid or clean to me

**原文链接**: [https://devz.cl/posts/solid-never-felt-solid/](https://devz.cl/posts/solid-never-felt-solid/)

生成摘要时出错

---

## 100. Spanish government 'quietly bans use of Palantir' in critical state systems

**原文标题**: Spanish government 'quietly bans use of Palantir' in critical state systems

**原文链接**: [https://www.lbc.co.uk/article/spanish-bans-palantir-national-security-5HjdcNp_2/](https://www.lbc.co.uk/article/spanish-bans-palantir-national-security-5HjdcNp_2/)

生成摘要时出错

---

