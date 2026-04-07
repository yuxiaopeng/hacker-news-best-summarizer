# Hacker News 热门文章摘要 (2026-04-07)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

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

## 11. Employers use your personal data to figure out the lowest salary you'll accept

**原文标题**: Employers use your personal data to figure out the lowest salary you'll accept

**原文链接**: [https://www.marketwatch.com/story/employers-are-using-your-personal-data-to-figure-out-the-lowest-salary-youll-accept-c2b968fb](https://www.marketwatch.com/story/employers-are-using-your-personal-data-to-figure-out-the-lowest-salary-youll-accept-c2b968fb)

生成摘要时出错

---

## 12. Show HN: Ghost Pepper – Local hold-to-talk speech-to-text for macOS

**原文标题**: Show HN: Ghost Pepper – Local hold-to-talk speech-to-text for macOS

**原文链接**: [https://github.com/matthartman/ghost-pepper](https://github.com/matthartman/ghost-pepper)

生成摘要时出错

---

## 13. What being ripped off taught me

**原文标题**: What being ripped off taught me

**原文链接**: [https://belief.horse/notes/what-being-ripped-off-taught-me/](https://belief.horse/notes/what-being-ripped-off-taught-me/)

生成摘要时出错

---

## 14. 81yo Dodgers fan can no longer get tickets because he doesn't have a smartphone

**原文标题**: 81yo Dodgers fan can no longer get tickets because he doesn't have a smartphone

**原文链接**: [https://twitter.com/Suzierizzo1/status/2040864617467924865](https://twitter.com/Suzierizzo1/status/2040864617467924865)

生成摘要时出错

---

## 15. We found an undocumented bug in the Apollo 11 guidance computer code

**原文标题**: We found an undocumented bug in the Apollo 11 guidance computer code

**原文链接**: [https://www.juxt.pro/blog/a-bug-on-the-dark-side-of-the-moon/](https://www.juxt.pro/blog/a-bug-on-the-dark-side-of-the-moon/)

生成摘要时出错

---

## 16. Dropping Cloudflare for Bunny.net

**原文标题**: Dropping Cloudflare for Bunny.net

**原文链接**: [https://jola.dev/posts/dropping-cloudflare](https://jola.dev/posts/dropping-cloudflare)

生成摘要时出错

---

## 17. Project Glasswing: Securing critical software for the AI era

**原文标题**: Project Glasswing: Securing critical software for the AI era

**原文链接**: [https://www.anthropic.com/glasswing](https://www.anthropic.com/glasswing)

生成摘要时出错

---

## 18. Adobe modifies hosts file to detect whether Creative Cloud is installed

**原文标题**: Adobe modifies hosts file to detect whether Creative Cloud is installed

**原文链接**: [https://www.osnews.com/story/144737/adobe-secretly-modifies-your-hosts-file-for-the-stupidest-reason/](https://www.osnews.com/story/144737/adobe-secretly-modifies-your-hosts-file-for-the-stupidest-reason/)

生成摘要时出错

---

## 19. German police name alleged leaders of GandCrab and REvil ransomware groups

**原文标题**: German police name alleged leaders of GandCrab and REvil ransomware groups

**原文链接**: [https://krebsonsecurity.com/2026/04/germany-doxes-unkn-head-of-ru-ransomware-gangs-revil-gandcrab/](https://krebsonsecurity.com/2026/04/germany-doxes-unkn-head-of-ru-ransomware-gangs-revil-gandcrab/)

生成摘要时出错

---

## 20. Show HN: I made a YouTube search form with advanced filters

**原文标题**: Show HN: I made a YouTube search form with advanced filters

**原文链接**: [https://playlists.at/youtube/search/](https://playlists.at/youtube/search/)

生成摘要时出错

---

## 21. Launch HN: Freestyle – Sandboxes for Coding Agents

**原文标题**: Launch HN: Freestyle – Sandboxes for Coding Agents

**原文链接**: [https://www.freestyle.sh/](https://www.freestyle.sh/)

生成摘要时出错

---

## 22. Show HN: GovAuctions lets you browse government auctions at once

**原文标题**: Show HN: GovAuctions lets you browse government auctions at once

**原文链接**: [https://www.govauctions.app/](https://www.govauctions.app/)

生成摘要时出错

---

## 23. The 1987 game “The Last Ninja” was 40 kilobytes

**原文标题**: The 1987 game “The Last Ninja” was 40 kilobytes

**原文链接**: [https://twitter.com/exQUIZitely/status/2040777977521398151](https://twitter.com/exQUIZitely/status/2040777977521398151)

生成摘要时出错

---

## 24. Age verification as mass surveillance infrastructure

**原文标题**: Age verification as mass surveillance infrastructure

**原文链接**: [https://tboteproject.com/surveillancefindings/](https://tboteproject.com/surveillancefindings/)

生成摘要时出错

---

## 25. Every GPU That Mattered

**原文标题**: Every GPU That Mattered

**原文链接**: [https://sheets.works/data-viz/every-gpu](https://sheets.works/data-viz/every-gpu)

生成摘要时出错

---

## 26. Book review: There Is No Antimemetics Division

**原文标题**: Book review: There Is No Antimemetics Division

**原文链接**: [https://www.stephendiehl.com/posts/no_antimimetics/](https://www.stephendiehl.com/posts/no_antimimetics/)

生成摘要时出错

---

## 27. Anthropic expands partnership with Google and Broadcom for next-gen compute

**原文标题**: Anthropic expands partnership with Google and Broadcom for next-gen compute

**原文链接**: [https://www.anthropic.com/news/google-broadcom-partnership-compute](https://www.anthropic.com/news/google-broadcom-partnership-compute)

生成摘要时出错

---

## 28. GLM-5.1: Towards Long-Horizon Tasks

**原文标题**: GLM-5.1: Towards Long-Horizon Tasks

**原文链接**: [https://z.ai/blog/glm-5.1](https://z.ai/blog/glm-5.1)

生成摘要时出错

---

## 29. An open-source 240-antenna array to bounce signals off the Moon

**原文标题**: An open-source 240-antenna array to bounce signals off the Moon

**原文链接**: [https://moonrf.com/](https://moonrf.com/)

生成摘要时出错

---

## 30. Peptides: where to begin?

**原文标题**: Peptides: where to begin?

**原文链接**: [https://www.science.org/content/blog-post/ah-peptides-where-begin](https://www.science.org/content/blog-post/ah-peptides-where-begin)

生成摘要时出错

---

## 31. Is Germany's gold safe in New York ?

**原文标题**: Is Germany's gold safe in New York ?

**原文链接**: [https://www.dw.com/en/is-germanys-gold-safe-in-new-york/video-75766873](https://www.dw.com/en/is-germanys-gold-safe-in-new-york/video-75766873)

生成摘要时出错

---

## 32. AI singer now occupies eleven spots on iTunes singles chart

**原文标题**: AI singer now occupies eleven spots on iTunes singles chart

**原文链接**: [https://www.showbiz411.com/2026/04/05/itunes-takeover-by-fake-ai-singer-eddie-dalton-now-occupies-eleven-spots-on-chart-despite-not-being-human-or-real-exclusive](https://www.showbiz411.com/2026/04/05/itunes-takeover-by-fake-ai-singer-eddie-dalton-now-occupies-eleven-spots-on-chart-despite-not-being-human-or-real-exclusive)

生成摘要时出错

---

## 33. System Card: Claude Mythos Preview [pdf]

**原文标题**: System Card: Claude Mythos Preview [pdf]

**原文链接**: [https://www-cdn.anthropic.com/53566bf5440a10affd749724787c8913a2ae0841.pdf](https://www-cdn.anthropic.com/53566bf5440a10affd749724787c8913a2ae0841.pdf)

生成摘要时出错

---

## 34. Show HN: Stop paying for Dropbox/Google Drive, use your own S3 bucket instead

**原文标题**: Show HN: Stop paying for Dropbox/Google Drive, use your own S3 bucket instead

**原文链接**: [https://locker.dev](https://locker.dev)

生成摘要时出错

---

## 35. After 20 years I turned off Google Adsense for my websites (2025)

**原文标题**: After 20 years I turned off Google Adsense for my websites (2025)

**原文链接**: [https://blog.ericgoldman.org/archives/2025/06/after-20-years-i-turned-off-google-adsense-for-my-websites.htm](https://blog.ericgoldman.org/archives/2025/06/after-20-years-i-turned-off-google-adsense-for-my-websites.htm)

生成摘要时出错

---

## 36. OpenAI's fall from grace as investors race to Anthropic

**原文标题**: OpenAI's fall from grace as investors race to Anthropic

**原文链接**: [https://www.latimes.com/business/story/2026-04-01/openais-shocking-fall-from-grace-as-investors-race-to-anthropic](https://www.latimes.com/business/story/2026-04-01/openais-shocking-fall-from-grace-as-investors-race-to-anthropic)

生成摘要时出错

---

## 37. Claude Code is locking people out for hours

**原文标题**: Claude Code is locking people out for hours

**原文链接**: [https://github.com/anthropics/claude-code/issues/44257](https://github.com/anthropics/claude-code/issues/44257)

生成摘要时出错

---

## 38. 12k Tons of Dumped Orange Peel Grew into a Landscape Nobody Expected (2017)

**原文标题**: 12k Tons of Dumped Orange Peel Grew into a Landscape Nobody Expected (2017)

**原文链接**: [https://www.sciencealert.com/how-12-000-tonnes-of-dumped-orange-peel-produced-something-nobody-imagined](https://www.sciencealert.com/how-12-000-tonnes-of-dumped-orange-peel-produced-something-nobody-imagined)

生成摘要时出错

---

## 39. AI may be making us think and write more alike

**原文标题**: AI may be making us think and write more alike

**原文链接**: [https://dornsife.usc.edu/news/stories/ai-may-be-making-us-think-and-write-more-alike/](https://dornsife.usc.edu/news/stories/ai-may-be-making-us-think-and-write-more-alike/)

生成摘要时出错

---

## 40. Cloudflare targets 2029 for full post-quantum security

**原文标题**: Cloudflare targets 2029 for full post-quantum security

**原文链接**: [https://blog.cloudflare.com/post-quantum-roadmap/](https://blog.cloudflare.com/post-quantum-roadmap/)

生成摘要时出错

---

## 41. Media scraper Gallery-dl is moving to Codeberg after receiving a DMCA notice

**原文标题**: Media scraper Gallery-dl is moving to Codeberg after receiving a DMCA notice

**原文链接**: [https://github.com/mikf/gallery-dl/discussions/9304](https://github.com/mikf/gallery-dl/discussions/9304)

生成摘要时出错

---

## 42. In Japan, the robot isn't coming for your job; it's filling the one nobody wants

**原文标题**: In Japan, the robot isn't coming for your job; it's filling the one nobody wants

**原文链接**: [https://techcrunch.com/2026/04/05/japan-is-proving-experimental-physical-ai-is-ready-for-the-real-world/](https://techcrunch.com/2026/04/05/japan-is-proving-experimental-physical-ai-is-ready-for-the-real-world/)

生成摘要时出错

---

## 43. Trump says 'a whole civilization will die tonight' if Iran does not make a deal

**原文标题**: Trump says 'a whole civilization will die tonight' if Iran does not make a deal

**原文链接**: [https://www.reuters.com/world/middle-east/trump-says-a-whole-civilization-will-die-tonight-if-iran-does-not-make-deal-2026-04-07/](https://www.reuters.com/world/middle-east/trump-says-a-whole-civilization-will-die-tonight-if-iran-does-not-make-deal-2026-04-07/)

生成摘要时出错

---

## 44. Sky – an Elm-inspired language that compiles to Go

**原文标题**: Sky – an Elm-inspired language that compiles to Go

**原文链接**: [https://github.com/anzellai/sky](https://github.com/anzellai/sky)

生成摘要时出错

---

## 45. Good Taste the Only Real Moat Left

**原文标题**: Good Taste the Only Real Moat Left

**原文链接**: [https://rajnandan.com/posts/taste-in-the-age-of-ai-and-llms/](https://rajnandan.com/posts/taste-in-the-age-of-ai-and-llms/)

生成摘要时出错

---

## 46. Solod – A subset of Go that translates to C

**原文标题**: Solod – A subset of Go that translates to C

**原文链接**: [https://github.com/solod-dev/solod](https://github.com/solod-dev/solod)

生成摘要时出错

---

## 47. Copilot is 'for entertainment purposes only', per Microsoft's terms of use

**原文标题**: Copilot is 'for entertainment purposes only', per Microsoft's terms of use

**原文链接**: [https://techcrunch.com/2026/04/05/copilot-is-for-entertainment-purposes-only-according-to-microsofts-terms-of-service/](https://techcrunch.com/2026/04/05/copilot-is-for-entertainment-purposes-only-according-to-microsofts-terms-of-service/)

生成摘要时出错

---

## 48. Identify a London Underground Line just by listening to it

**原文标题**: Identify a London Underground Line just by listening to it

**原文链接**: [https://tubesoundquiz.com/](https://tubesoundquiz.com/)

生成摘要时出错

---

## 49. A macOS bug that causes TCP networking to stop working after 49.7 days

**原文标题**: A macOS bug that causes TCP networking to stop working after 49.7 days

**原文链接**: [https://photon.codes/blog/we-found-a-ticking-time-bomb-in-macos-tcp-networking](https://photon.codes/blog/we-found-a-ticking-time-bomb-in-macos-tcp-networking)

生成摘要时出错

---

## 50. Blackholing My Email

**原文标题**: Blackholing My Email

**原文链接**: [https://www.johnsto.co.uk/blog/blackholing-my-email/](https://www.johnsto.co.uk/blog/blackholing-my-email/)

生成摘要时出错

---

## 51. The team behind a pro-Iran, Lego-themed viral-video campaign

**原文标题**: The team behind a pro-Iran, Lego-themed viral-video campaign

**原文链接**: [https://www.newyorker.com/culture/infinite-scroll/the-team-behind-a-pro-iran-lego-themed-viral-video-campaign](https://www.newyorker.com/culture/infinite-scroll/the-team-behind-a-pro-iran-lego-themed-viral-video-campaign)

生成摘要时出错

---

## 52. Show HN: Gemma Gem – AI model embedded in a browser – no API keys, no cloud

**原文标题**: Show HN: Gemma Gem – AI model embedded in a browser – no API keys, no cloud

**原文链接**: [https://github.com/kessler/gemma-gem](https://github.com/kessler/gemma-gem)

生成摘要时出错

---

## 53. Bacteria found in the human intestine capable of improving muscle strength

**原文标题**: Bacteria found in the human intestine capable of improving muscle strength

**原文链接**: [https://www.ugr.es/en/about/news/bacteria-found-human-intestine-capable-improving-muscle-strength](https://www.ugr.es/en/about/news/bacteria-found-human-intestine-capable-improving-muscle-strength)

生成摘要时出错

---

## 54. Cambodia unveils a statue of famous landmine-sniffing rat Magawa

**原文标题**: Cambodia unveils a statue of famous landmine-sniffing rat Magawa

**原文链接**: [https://www.bbc.com/news/articles/c0rx7xzd10xo](https://www.bbc.com/news/articles/c0rx7xzd10xo)

生成摘要时出错

---

## 55. Show HN: A cartographer's attempt to realistically map Tolkien's world

**原文标题**: Show HN: A cartographer's attempt to realistically map Tolkien's world

**原文链接**: [https://www.intofarlands.com/atlasofarda](https://www.intofarlands.com/atlasofarda)

生成摘要时出错

---

## 56. Drop, formerly Massdrop, ends most collaborations and rebrands under Corsair

**原文标题**: Drop, formerly Massdrop, ends most collaborations and rebrands under Corsair

**原文链接**: [https://drop.com/](https://drop.com/)

生成摘要时出错

---

## 57. Usenet Archives

**原文标题**: Usenet Archives

**原文链接**: [https://usenetarchives.com](https://usenetarchives.com)

生成摘要时出错

---

## 58. Number in man page titles e.g. sleep(3)

**原文标题**: Number in man page titles e.g. sleep(3)

**原文链接**: [https://lalitm.com/til-number-in-man-page-titles-e-g-sleep-3/](https://lalitm.com/til-number-in-man-page-titles-e-g-sleep-3/)

生成摘要时出错

---

## 59. Assessing Claude Mythos Preview's cybersecurity capabilities

**原文标题**: Assessing Claude Mythos Preview's cybersecurity capabilities

**原文链接**: [https://red.anthropic.com/2026/mythos-preview/](https://red.anthropic.com/2026/mythos-preview/)

生成摘要时出错

---

## 60. Musician says AI company is cloning her music, filing claims against her

**原文标题**: Musician says AI company is cloning her music, filing claims against her

**原文链接**: [https://twitter.com/unlimited_ls/status/2040577536136974444](https://twitter.com/unlimited_ls/status/2040577536136974444)

生成摘要时出错

---

