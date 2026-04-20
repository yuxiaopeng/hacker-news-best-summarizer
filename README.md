# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-04-20.md)

*最后自动更新时间: 2026-04-20 20:27:40*
## 1. Vercel April 2026 security incident

**原文标题**: Vercel April 2026 security incident

**原文链接**: [https://www.bleepingcomputer.com/news/security/vercel-confirms-breach-as-hackers-claim-to-be-selling-stolen-data/](https://www.bleepingcomputer.com/news/security/vercel-confirms-breach-as-hackers-claim-to-be-selling-stolen-data/)

Vercel 于 2026 年 4 月 19 日证实发生了一起安全事件，此前自称“ShinyHunters”的威胁行为者在一个黑客论坛上宣布，他们已攻破该平台并正在出售被盗数据。

此次泄露源于 Vercel 某员工的 Google Workspace 账户被入侵，而该入侵是因第三方 AI 平台 Context.ai 发生的安全事件，特别是涉及到一个 Google Workspace OAuth 应用程序所致。攻击者利用此访问权限渗透进入 Vercel 环境。

据 Vercel 首席执行官 Guillermo Rauch 称，攻击者在枚举出“非敏感”环境变量后，利用这些未进行静态加密的变量获得了进一步的访问权限。虽然 Vercel 会加密所有客户环境变量，但一项特定功能允许某些变量被指定为非敏感。

Vercel 表示，一小部分客户受到影响，但其服务并未受到冲击。他们已聘请事件响应专家，通知了执法部门，并保证 Next.js 等核心系统和开源项目仍然安全。

该黑客声称正在出售访问密钥、源代码、数据库数据、内部部署以及 API 密钥，其中包括 NPM 和 GitHub 令牌。他们还分享了一份包含 580 条 Vercel 员工记录的列表，以及一张据称是内部仪表板的截图。据称，赎金要求高达 200 万美元。

Vercel 已推出仪表板更新，以改进环境变量管理，并强烈建议客户检查其环境变量中是否存在敏感信息，启用“敏感变量”功能进行静态加密，并在必要时轮换密钥。

---

## 2. 2027年起，欧盟销售手机须配备可更换电池。

**原文标题**: All phones sold in the EU to have replaceable batteries from 2027

**原文链接**: [https://www.theolivepress.es/spain-news/2026/04/20/eu-to-force-replaceable-batteries-in-phones-and-tablets-from-2027/](https://www.theolivepress.es/spain-news/2026/04/20/eu-to-force-replaceable-batteries-in-phones-and-tablets-from-2027/)

欧盟颁布了一项新法规，要求到2027年，在欧盟境内销售的所有便携式设备，包括智能手机和平板电脑，必须配备用户可更换的电池。这项里程碑式的立法，经欧洲议会和理事会初步达成一致并随后由理事会通过，旨在大幅减少电子垃圾，并促进电池的循环经济。

该法规规定，消费者必须能够在无需专业工具或知识的情况下，轻松地从其设备中取出并更换电池。这项举措预计将延长电子产品的使用寿命，减少消费，并减轻与不可维修设备以及内置电池处理相关的环境影响。

除了消费电子产品，新规还适用于广泛的便携式电池，包括电动自行车和电动滑板车等轻型交通工具使用的电池，以及电动汽车电池、工业电池和启动电池。这项全面的立法还设定了废弃物收集、材料回收（例如锂、钴、镍和铅）的雄心勃勃的目标，并要求对某些类型的电池进行碳足迹声明。这种整体方法强调了欧盟致力于在从生产到回收的整个电池生命周期中实现可持续发展。

---

## 3. GitHub的虚假星标经济

**原文标题**: GitHub's Fake Star Economy

**原文链接**: [https://awesomeagents.ai/news/github-fake-stars-investigation/](https://awesomeagents.ai/news/github-fake-stars-investigation/)

CMU最近的一项研究 (ICSE 2026) 揭示了600万个虚假GitHub星标，涉及18,617个代码库，由301,000个账户生成。这个问题在2024年急剧增加，AI/LLM项目是被针对的最大非恶意类别。这些星标在众多网站、Fiverr和Telegram上公开出售，每个价格从0.03美元到0.85美元不等，卖家提供不同质量的账户和保证。

风险投资家明确将星标数量作为重要的项目来源信号，运行自动化爬虫来识别快速增长的项目。Redpoint Ventures发现种子轮项目的星标中位数为2,850个，这使得购买星标的投资回报率巨大（例如，花费85-285美元购买2,850个星标，就能获得数百万美元的种子轮融资）。

我们对20个代码库的独立分析揭示了明显的操纵痕迹：36-76%的星标用户关注者/代码库为零，高“僵尸账户”比例，以及极低的fork与star比率（例如，比自然基线低10倍）。例如，Union Labs，一个在风险投资指数中排名靠前的项目，也显示出明显的虚假星标迹象。fork与star比率（对于拥有1万+星标的代码库低于0.05）是一个强有力的检测启发式指标。

这种虚假人气延伸到npm下载量、VS Code扩展和X等社交媒体平台，通常通过互动群组放大。从法律角度看，FTC的2024年规定禁止出售/购买“社交媒体影响力虚假指标”，每项违规行为可处以53,088美元的罚款。美国证交会（SEC）也曾起诉初创公司创始人在融资期间虚报增长指标，这表明欺骗投资者并非“假装成功直到成功”的一部分。这形成了一个成熟的、专业化的、公然运作的影子经济。

---

## 4. At long last, InfoWars is ours

**原文标题**: At long last, InfoWars is ours

**原文链接**: [https://theonion.com/at-long-last-infowars-is-ours/](https://theonion.com/at-long-last-infowars-is-ours/)

On April 20, 2026, Bryce P. Tetraeder, CEO of Global Tetrahedron, announced the successful acquisition of InfoWars.com, calling it the fulfillment of a childhood "night terror" dream. Tetraeder outlines an ambitious, "cruel" vision for the platform, aligning it with market data.

He envisions the new InfoWars as an "infinite virtual surface" teeming with ads, scams, and "free radical misinformation," designed for "psychological torture" and the disintegration of visitors' minds. Comparing the project to the Manhattan Project, but for a website, he describes it as a place welcoming "brutal and sadistic ideas" from all, even "the very stupidest among us."

Tetraeder anticipates InfoWars becoming a "swirling vortex of content about content," where media mergers process human artistry into an "endlessly digestible slurry"—a "dank, sunless place" where panic and capital feed each other, reflecting what he calls "modern-day America." He believes this can be achieved by combining amateur inquiry, corporate profit, and the clarity gained from "mind- and body-altering chemicals."

Concluding with a cynical welcome to "warriors," Tetraeder acknowledges the future will be "long" and "bad," emphasizing the power they now wield by controlling a website.

---

## 5. NIST scientists create 'any wavelength' lasers

**原文标题**: NIST scientists create 'any wavelength' lasers

**原文链接**: [https://www.nist.gov/news-events/news/2026/04/any-color-you-nist-scientists-create-any-wavelength-lasers-tiny-circuits](https://www.nist.gov/news-events/news/2026/04/any-color-you-nist-scientists-create-any-wavelength-lasers-tiny-circuits)

生成摘要时出错

---

## 6. Kimi K2.6: Advancing open-source coding

**原文标题**: Kimi K2.6: Advancing open-source coding

**原文链接**: [https://www.kimi.com/blog/kimi-k2-6](https://www.kimi.com/blog/kimi-k2-6)

Kimi has open-sourced its latest model, Kimi K2.6, featuring state-of-the-art coding, long-horizon execution, and advanced agent swarm capabilities. Available via Kimi.com, the Kimi App, API, and Kimi Code, K2.6 marks a significant advancement for open-source models.

The model demonstrates strong improvements in **long-horizon coding**, generalizing reliably across languages like Rust, Go, and Python, and tasks such as front-end development, devops, and performance optimization. Examples include optimizing a Qwen3.5-0.8B model in Zig, achieving 193 tokens/sec, and autonomously overhauling an 8-year-old financial engine, boosting throughput by 185%. Enterprise feedback highlights its exceptional reliability, tool-calling quality, and ability to tackle complex engineering challenges.

K2.6 also introduces **Coding-Driven Design**, turning simple prompts into complete front-end interfaces and supporting lightweight full-stack workflows. Its enhanced **Agent Swarm** architecture scales to 300 sub-agents executing 4,000 steps concurrently, enabling multi-format content generation and turning documents into reusable "Skills."

Furthermore, K2.6 excels in **Proactive Agents**, supporting continuous, 24/7 autonomous operations (demonstrated by a 5-day engineering worklog). The new **Claw Groups** feature fosters human-AI collaboration by coordinating diverse agents with specialized toolkits and persistent memory. Benchmarks show Kimi K2.6 is highly competitive with leading closed-source models and significantly outperforms Kimi K2.5 across various coding, reasoning, and vision tasks, establishing a new benchmark for open-source AI.

---

## 7. Qwen3.6-Max-Preview: Smarter, Sharper, Still Evolving

**原文标题**: Qwen3.6-Max-Preview: Smarter, Sharper, Still Evolving

**原文链接**: [https://qwen.ai/blog?id=qwen3.6-max-preview](https://qwen.ai/blog?id=qwen3.6-max-preview)

生成摘要时出错

---

## 8. NSA is using Anthropic's Mythos despite blacklist

**原文标题**: NSA is using Anthropic's Mythos despite blacklist

**原文链接**: [https://www.axios.com/2026/04/19/nsa-anthropic-mythos-pentagon](https://www.axios.com/2026/04/19/nsa-anthropic-mythos-pentagon)

生成摘要时出错

---

## 9. Atlassian enables default data collection to train AI

**原文标题**: Atlassian enables default data collection to train AI

**原文链接**: [https://letsdatascience.com/news/atlassian-enables-default-data-collection-to-train-ai-f71343d8](https://letsdatascience.com/news/atlassian-enables-default-data-collection-to-train-ai-f71343d8)

生成摘要时出错

---

## 10. Notion leaks email addresses of all editors of any public page

**原文标题**: Notion leaks email addresses of all editors of any public page

**原文链接**: [https://twitter.com/weezerOSINT/status/2045849358462222720](https://twitter.com/weezerOSINT/status/2045849358462222720)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 2 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 3 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 4 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 5 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 6 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 7 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 8 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 9 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 10 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 11 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 12 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 13 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 14 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 15 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 16 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 17 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 18 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 19 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 20 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 21 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 22 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 23 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 24 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 25 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 26 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 27 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 28 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 29 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 30 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 31 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 32 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 33 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 34 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 35 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 36 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 37 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 38 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 39 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 40 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 41 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 42 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 43 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 44 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 45 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 46 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 47 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 48 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 49 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 50 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 51 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 52 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 53 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 54 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 55 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 56 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 57 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 58 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 59 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 60 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 61 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 62 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 63 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 64 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 65 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 66 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 67 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 68 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 69 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 70 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 71 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 72 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 73 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 74 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 75 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 76 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 77 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 78 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 79 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 80 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 81 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 82 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 83 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 84 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 85 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 86 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 87 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 88 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 89 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 90 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 91 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 92 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 93 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 94 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 95 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 96 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 97 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 98 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 99 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 100 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 101 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 102 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 103 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 104 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 105 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 106 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 107 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 108 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 109 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 110 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 111 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 112 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 113 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 114 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 115 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 116 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 117 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 118 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 119 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 120 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 121 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 122 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 123 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 124 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 125 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 126 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 127 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 128 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 129 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 130 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 131 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 132 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 133 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 134 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 135 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 136 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 137 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 138 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 139 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 140 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 141 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 142 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 143 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 144 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 145 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 146 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 147 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 148 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 149 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 150 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 151 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 152 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 153 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 154 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 155 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 156 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 157 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 158 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 159 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
| 160 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 161 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 162 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 163 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 164 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
