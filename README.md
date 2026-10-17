# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-10-17.md)

*最后自动更新时间: 2026-10-17 21:46:13*
## 1. 特斯拉 Roadster

**原文标题**: Tesla Roadster

**原文链接**: [https://www.tesla.com/roadster](https://www.tesla.com/roadster)

特斯拉 Roadster 被誉为全球最快、最先进的汽车，旨在以其全电动性能重新定义超级跑车体验。它拥有无与伦比的加速性能，0-60 英里/小时加速仅需创纪录的 1.9 秒，0-100 英里/小时加速仅需 4.2 秒，四分之一英里加速仅需 8.8 秒。其最高时速超过 250 英里/小时，这得益于惊人的 10,000 牛·米轮上扭矩。

除了惊人的速度，Roadster 单次充电续航里程可达同级领先的 620 英里（1,000 公里）。它配备三电机全轮驱动系统，带有扭矩矢量控制功能，可实现卓越的操控和性能。

其设计时尚、空气动力学且充满未来感，采用可拆卸玻璃车顶，可方便地收纳在后备箱中。尽管注重性能，它仍提供实用的 2+2 座椅配置，可容纳四名成人。内饰现代、以驾驶员为中心且宽敞。特斯拉 Roadster 被定位为特斯拉工程和愿景的终极体现，突破了电动汽车能力的界限。目前已开放预订。

---

## 2. 克劳德揭示ECDSA曲线起源

**原文标题**: Claude reveals ECDSA curve origins

**原文链接**: [https://www.anthropic.com/research/ecdsa-curve-origins](https://www.anthropic.com/research/ecdsa-curve-origins)

Anthropic的AI模型Claude解开了NIST广泛使用的ECDSA椭圆曲线（P-192、P-224、P-256、P-384、P-521）以及多个ANSI X9.62曲线的“种子”参数来源长达25年的谜团。这些种子参数此前由美国国家安全局（NSA）提供，但未作任何解释，这引发了人们对潜在后门的长期担忧。

Claude发现，这些种子并非如传闻所言，是一个幽默短语的哈希值。相反，它们是`lrand48`伪随机数生成器（PRNG）的输出，这种生成器在1990年代的C语言库中很常见，并以1997年5月至1998年4月间的Unix时间戳作为种子。Claude在这些种子中识别出规律，例如顶部比特位持续为零（这是`lrand48`的特征），并利用格基约化算法恢复了PRNG的内部状态和初始时间戳。

这一发现并非密码学上的突破，而是一次重要的信心提振。它增强了人们对这些曲线不含故意后门的信心，因为它们的参数是使用一个标准的、以时钟为种子的PRNG，以无害且可重现的方式生成的。

此外，Claude还查明了P-192和五个ANSI X9.62示例曲线的基点来源，追溯到Arjen Lenstra的FreeLIP软件包中用小整数初始化的随机数生成器。

尽管大多数种子和部分基点现已得到解释，但B-163二进制种子以及P-224、P-256、P-384和P-521曲线的基点仍未解密。解决这一谜团的36,864美元赏金将捐赠给互联网安全研究小组。

---

## 3. DeepSeek-4.1版-闪-1017

**原文标题**: DeepSeek-v4.1-Flash-1017

**原文链接**: [https://huggingface.co/deepseek-ai/DeepSeek-V4.1-Flash-1017](https://huggingface.co/deepseek-ai/DeepSeek-V4.1-Flash-1017)

这篇文章提到了“DeepSeek-v4.1-Flash-1017”，这是DeepSeek最新发布或更新的一个版本，具体来说是4.1版，可能针对速度进行了优化（“Flash”）。该版本包含11个不同的项目或组件。它非常新，大约在16小时前更新。另外，数字“932”也被提及，这可能表示与该版本相关的下载量、浏览量或整体受欢迎程度等指标。

---

## 4. 美国90%的工时用于AI基准未充分覆盖的任务。

**原文标题**: 90% of US working hours are spent on tasks not covered well by AI benchmarks

**原文链接**: [https://www.mercor.com/research/labor-index/benchmark-map/](https://www.mercor.com/research/labor-index/benchmark-map/)

MercorResearch的“基准地图”显示，美国高达90%的工作时长都花在现有AI基准几乎未涵盖的任务上。这一巨大空白使得准确评估AI模型的实际能力和经济影响变得困难。

这项研究将29个与经济相关的AI基准与美国劳工部O*NET分类法（923个职业，18,797项任务）进行对比，发现覆盖范围有限。仅有208个职业的任务由至少五个基准提示所代表。基准覆盖并非随机，它不成比例地侧重于被视为“易受AI影响”的任务、工资支出较大的职业以及被评为“重要”的任务。例如，律师的任务得到了很好的覆盖，但同样易受AI影响的法律秘书或法庭书记员的任务却被忽视，这在中等收入的知识工作中造成了盲点。

虽然当前基准优先考虑AI可能取得进展的领域，但这种狭隘的关注却忽略了经济中一个庞大的部分。研究人员建议使用O*NET加权来更公平地平均模型在各项任务上的表现，确保每项任务对职业的整体AI分数贡献均等。初步测试显示，由于任务覆盖不足，差异很小。重大挑战依然存在，包括许多任务的统计效力低，以及现有基准的质量和难度各异。这些发现强调了迫切需要更广泛、更多样化的高质量基准，以真正理解AI在整个经济中的能力。

---

## 5. DeepSeek：DeepSeek v4.1 Flash 1017

**原文标题**: DeepSeek: DeepSeek v4.1 Flash 1017

**原文链接**: [https://openrouter.ai/deepseek/deepseek-v4.1-flash-1017](https://openrouter.ai/deepseek/deepseek-v4.1-flash-1017)

深度求索 v4.1 Flash 1017 是一款由深度求索开发的大语言模型 (LLM)，它针对高速和成本效益进行了优化，同时不影响性能。该模型可通过 OpenRouter.ai 等平台获取，旨在为各种 AI 应用提供高效的解决方案。

深度求索 v4.1 Flash 1017 的一个关键特性是其令人印象深刻的 128k 上下文窗口，使其能够处理和生成更长、更复杂的文本序列，同时保持连贯性和理解力。这种速度、经济性与大上下文窗口的平衡，使其成为需要快速响应和经济处理任务的有力竞争者。它适用于通用文本生成、摘要、问答以及其他交互式应用，在这些应用中，效率和强大性能至关重要。

---

## 6. Meta新商业条款将允许抓取新闻网站：专家称

**原文标题**: Meta’s new commercial terms will allow the scraping of news sites: experts

**原文链接**: [https://www.niemanlab.org/2026/10/metas-new-commercial-terms-will-allow-the-scraping-of-news-sites-legal-experts-say/](https://www.niemanlab.org/2026/10/metas-new-commercial-terms-will-allow-the-scraping-of-news-sites-legal-experts-say/)

Meta更新的商业条款将于10月30日生效，将允许该公司抓取与商业账户“关联”的网站内容，这包括几乎所有新闻出版商。法律专家警告称，继续使用Facebook、Instagram或WhatsApp的商业账户，意味着默许Meta抓取这些网站，并利用所收集的内容来训练其AI产品。

专家们将这一条款描述为“非同寻常”，它可能让Meta获取通常需要数百万美元许可费的材料。他们认为新条款可能使Meta开发出直接与出版商竞争的AI。尽管Meta声称此次更新整合了现有语言，并允许出版商使用robots.txt进行屏蔽，但专家们认为这些条款可能凌驾于此类指令之上，并且“测试凭证”可能绕过付费墙。

康奈尔大学法学教授James Grimmelmann强调，出版商要么相信Meta的意图，要么停止使用其商业账户。此举被比作反垄断法中的“捆绑销售”，即Meta利用平台访问权限来获取抓取许可。这恰逢Meta的“Meta One”服务，该服务向用户收取发布外部链接的费用，而这些链接指向的内容Meta现在将免费抓取。根据这些条款进行AI训练的合法性仍然是正在进行的诉讼的主题。一些出版商，如《蒸汽朋克探索者》(The Steampunk Explorer)的Stephen Beale，正在考虑关闭他们的Meta账户以示回应。

---

## 7. OpenCode 被黑：用户凭据泄露

**原文标题**: OpenCode Hacked: User credentials leaked

**原文链接**: [https://twitter.com/opencode/status/2111516673953935833](https://twitter.com/opencode/status/2111516673953935833)

OpenCode报告了一起安全漏洞，被确认为“大规模蒸馏攻击”，该事件发生于昨晚，导致用户凭证泄露。此次事件影响了1.4%的OpenCode Console用户，所有受影响用户已于今早通过电子邮件收到通知。

OpenCode表示，目前情况仍在持续，暂时无法透露更多细节。该公司正积极与Anthropic、OpenAI和Google合作以修复该问题。此公告于2026年10月17日发布。

---

## 8. 你本可以凭记忆发明Transformer。

**原文标题**: You could have invented transformers from memory

**原文链接**: [https://alexwang.ai/posts/associative-memory/](https://alexwang.ai/posts/associative-memory/)

生成摘要时出错

---

## 9. How the Claude Code team does code review

**原文标题**: How the Claude Code team does code review

**原文链接**: [https://claude.dev/blog/solving-code-review-at-anthropic/](https://claude.dev/blog/solving-code-review-at-anthropic/)

The Claude Code team reviews an immense volume of code, 90% of which is AI-generated. Their approach redefines code review to minimize human time without increasing reverts or incidents, largely by automating code analysis and preserving human attention for unique challenges.

Code review now primarily finds/fixes issues, acting continuously rather than as a final gate. Most changes are pre-reviewed and fixed by Claude before human involvement. The goal is for most pull requests to merge with at most one human (often the author) while maintaining low error rates.

The review process is multi-layered:
1.  **Before the PR:** Claude verifies its own work, running tests, builds, and a subagent reviews the diff.
2.  **On Every PR:** Automated checks include CI (linting, tests), Claude AI code review (bugs hunted by agents, findings verified), automated security review, and risk-based human approval (0, 1, or 2 people depending on change risk and author's trust). Agent approvals never count as human.
3.  **Merging:** A merge queue re-runs checks against the latest main branch.
4.  **After Merge:** Changes ship behind flags to Anthropic employees first, then gradually release to public channels. Fast detection and rollback capabilities are critical for inevitable mistakes.

The team continuously improves its AI reviewer by converting past incidents and reverts into daily evaluation cases. This iterative process measures comment noise and refines the reviewer's prompts and tools to efficiently catch real bugs and reduce unnecessary feedback.

---

## 10. Solar surpasses nuclear power globally for first time

**原文标题**: Solar surpasses nuclear power globally for first time

**原文链接**: [https://www.pv-magazine.com/2026/09/29/solar-surpasses-nuclear-power-globally-for-first-time/](https://www.pv-magazine.com/2026/09/29/solar-surpasses-nuclear-power-globally-for-first-time/)

The World Nuclear Industry Status Report (WNISR) 2026 reveals that solar and wind power are rapidly surpassing nuclear energy globally. In 2025, solar generation for the first time exceeded nuclear output annually, and monthly solar generation outpaced nuclear starting April 2025. Wind power also individually surpassed nuclear monthly from March 2025.

The report highlights a widening gap: global solar capacity grew by 510 GW (27%) to 2,383 GW in 2025, while wind added 159 GW (14%) to reach 1,291 GW. Conversely, installed nuclear capacity rose by only 1.5 GW to 399.5 GW, with operating capacity slightly declining. Nuclear capacity has remained essentially flat for over 25 years, while renewables have expanded rapidly, further supported by significant grid-scale battery deployment (104 GW/257 GWh in 2025).

The global nuclear sector's expansion is slow, concentrated mainly in China and Russia. In 2025, nuclear output increased by 1.1% globally (driven by China, declining elsewhere), with its share of global electricity generation falling to a 45-year low of 8.8%. More reactors closed (seven) than started (four) in 2025. New nuclear projects face long construction times, averaging 10.9 years for recent startups, with none completed on schedule.

Small modular reactors (SMRs) show limited commercial progress despite growing government support. The report questions claims of lower costs, improved safety, and reduced waste, noting their heavy reliance on public funding and uncertain deployment timelines and benefits.

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-10-17](output/hacker_news_summary_2026-10-17.md) |
| 2 | [2026-10-15](output/hacker_news_summary_2026-10-15.md) |
| 3 | [2026-10-14](output/hacker_news_summary_2026-10-14.md) |
| 4 | [2026-10-16](output/hacker_news_summary_2026-10-16.md) |
| 5 | [2026-10-13](output/hacker_news_summary_2026-10-13.md) |
| 6 | [2026-10-07](output/hacker_news_summary_2026-10-07.md) |
| 7 | [2026-10-10](output/hacker_news_summary_2026-10-10.md) |
| 8 | [2026-10-09](output/hacker_news_summary_2026-10-09.md) |
| 9 | [2026-10-11](output/hacker_news_summary_2026-10-11.md) |
| 10 | [2026-10-01](output/hacker_news_summary_2026-10-01.md) |
| 11 | [2026-09-29](output/hacker_news_summary_2026-09-29.md) |
| 12 | [2026-10-06](output/hacker_news_summary_2026-10-06.md) |
| 13 | [2026-10-04](output/hacker_news_summary_2026-10-04.md) |
| 14 | [2026-09-30](output/hacker_news_summary_2026-09-30.md) |
| 15 | [2026-10-02](output/hacker_news_summary_2026-10-02.md) |
| 16 | [2026-10-03](output/hacker_news_summary_2026-10-03.md) |
| 17 | [2026-09-24](output/hacker_news_summary_2026-09-24.md) |
| 18 | [2026-09-21](output/hacker_news_summary_2026-09-21.md) |
| 19 | [2026-09-23](output/hacker_news_summary_2026-09-23.md) |
| 20 | [2026-09-27](output/hacker_news_summary_2026-09-27.md) |
| 21 | [2026-09-22](output/hacker_news_summary_2026-09-22.md) |
| 22 | [2026-09-25](output/hacker_news_summary_2026-09-25.md) |
| 23 | [2026-09-20](output/hacker_news_summary_2026-09-20.md) |
| 24 | [2026-09-16](output/hacker_news_summary_2026-09-16.md) |
| 25 | [2026-09-17](output/hacker_news_summary_2026-09-17.md) |
| 26 | [2026-09-19](output/hacker_news_summary_2026-09-19.md) |
| 27 | [2026-09-18](output/hacker_news_summary_2026-09-18.md) |
| 28 | [2026-09-09](output/hacker_news_summary_2026-09-09.md) |
| 29 | [2026-09-10](output/hacker_news_summary_2026-09-10.md) |
| 30 | [2026-09-13](output/hacker_news_summary_2026-09-13.md) |
| 31 | [2026-09-14](output/hacker_news_summary_2026-09-14.md) |
| 32 | [2026-09-11](output/hacker_news_summary_2026-09-11.md) |
| 33 | [2026-09-12](output/hacker_news_summary_2026-09-12.md) |
| 34 | [2026-09-15](output/hacker_news_summary_2026-09-15.md) |
| 35 | [2026-09-03](output/hacker_news_summary_2026-09-03.md) |
| 36 | [2026-09-02](output/hacker_news_summary_2026-09-02.md) |
| 37 | [2026-09-04](output/hacker_news_summary_2026-09-04.md) |
| 38 | [2026-09-08](output/hacker_news_summary_2026-09-08.md) |
| 39 | [2026-09-05](output/hacker_news_summary_2026-09-05.md) |
| 40 | [2026-09-07](output/hacker_news_summary_2026-09-07.md) |
| 41 | [2026-09-06](output/hacker_news_summary_2026-09-06.md) |
| 42 | [2026-08-25](output/hacker_news_summary_2026-08-25.md) |
| 43 | [2026-08-31](output/hacker_news_summary_2026-08-31.md) |
| 44 | [2026-08-28](output/hacker_news_summary_2026-08-28.md) |
| 45 | [2026-09-01](output/hacker_news_summary_2026-09-01.md) |
| 46 | [2026-08-29](output/hacker_news_summary_2026-08-29.md) |
| 47 | [2026-08-30](output/hacker_news_summary_2026-08-30.md) |
| 48 | [2026-08-26](output/hacker_news_summary_2026-08-26.md) |
| 49 | [2026-08-22](output/hacker_news_summary_2026-08-22.md) |
| 50 | [2026-08-19](output/hacker_news_summary_2026-08-19.md) |
| 51 | [2026-08-20](output/hacker_news_summary_2026-08-20.md) |
| 52 | [2026-08-16](output/hacker_news_summary_2026-08-16.md) |
| 53 | [2026-08-17](output/hacker_news_summary_2026-08-17.md) |
| 54 | [2026-08-23](output/hacker_news_summary_2026-08-23.md) |
| 55 | [2026-08-18](output/hacker_news_summary_2026-08-18.md) |
| 56 | [2026-08-21](output/hacker_news_summary_2026-08-21.md) |
| 57 | [2026-08-24](output/hacker_news_summary_2026-08-24.md) |
| 58 | [2026-08-12](output/hacker_news_summary_2026-08-12.md) |
| 59 | [2026-08-11](output/hacker_news_summary_2026-08-11.md) |
| 60 | [2026-08-14](output/hacker_news_summary_2026-08-14.md) |
| 61 | [2026-08-10](output/hacker_news_summary_2026-08-10.md) |
| 62 | [2026-08-09](output/hacker_news_summary_2026-08-09.md) |
| 63 | [2026-08-15](output/hacker_news_summary_2026-08-15.md) |
| 64 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 65 | [2026-08-13](output/hacker_news_summary_2026-08-13.md) |
| 66 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 67 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 68 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 69 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 70 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 71 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 72 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 73 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 74 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 75 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 76 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 77 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 78 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 79 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 80 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 81 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 82 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 83 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 84 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 85 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 86 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 87 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 88 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 89 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 90 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 91 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 92 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 93 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 94 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 95 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 96 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 97 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 98 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 99 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 100 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 101 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 102 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 103 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 104 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 105 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 106 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 107 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 108 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 109 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 110 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 111 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 112 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 113 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 114 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 115 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 116 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 117 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 118 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 119 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 120 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 121 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 122 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 123 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 124 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 125 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 126 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 127 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 128 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 129 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 130 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 131 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 132 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 133 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 134 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 135 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 136 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 137 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 138 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 139 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 140 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 141 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 142 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 143 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 144 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 145 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 146 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 147 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 148 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 149 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 150 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 151 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 152 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 153 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 154 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 155 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 156 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 157 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 158 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 159 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 160 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 161 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 162 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 163 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 164 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 165 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 166 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 167 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 168 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 169 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 170 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 171 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 172 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 173 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 174 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 175 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 176 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 177 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 178 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 179 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 180 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 181 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 182 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 183 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 184 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 185 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 186 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 187 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 188 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 189 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 190 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 191 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 192 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 193 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 194 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 195 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 196 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 197 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 198 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 199 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 200 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 201 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 202 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 203 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 204 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 205 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 206 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 207 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 208 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 209 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 210 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 211 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 212 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 213 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 214 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 215 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 216 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 217 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 218 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 219 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 220 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 221 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 222 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 223 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 224 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 225 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 226 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 227 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 228 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 229 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 230 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 231 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 232 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 233 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 234 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 235 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 236 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 237 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 238 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 239 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 240 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 241 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 242 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 243 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 244 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 245 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 246 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 247 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 248 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 249 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 250 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 251 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 252 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 253 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 254 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 255 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 256 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 257 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 258 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 259 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 260 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 261 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 262 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 263 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 264 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 265 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 266 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 267 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 268 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 269 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 270 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 271 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 272 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 273 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 274 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 275 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 276 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 277 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 278 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 279 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 280 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 281 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 282 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 283 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 284 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 285 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 286 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 287 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 288 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 289 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 290 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 291 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 292 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 293 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 294 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 295 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 296 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 297 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 298 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 299 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 300 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 301 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 302 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 303 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 304 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 305 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 306 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 307 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 308 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 309 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 310 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 311 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 312 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 313 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 314 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 315 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 316 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 317 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 318 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 319 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 320 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 321 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 322 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 323 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 324 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 325 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 326 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 327 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 328 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 329 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 330 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 331 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 332 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 333 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 334 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 335 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 336 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 337 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
