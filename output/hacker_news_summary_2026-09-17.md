# Hacker News 热门文章摘要 (2026-09-17)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 英伟达宣布Rust原生GPU编程

**原文标题**: Nvidia announces native GPU programming in Rust

**原文链接**: [https://developer.nvidia.com/blog/introducing-cuda-rust-two-tracks-for-writing-gpu-kernels/](https://developer.nvidia.com/blog/introducing-cuda-rust-two-tracks-for-writing-gpu-kernels/)

2026年9月，英伟达（Nvidia）宣布致力于在Rust中进行原生GPU编程，旨在到2027年及以后，发展并成熟其CUDA Rust工具链。此举旨在应对Rust在AI系统层日益增长的采用，重视其编译时安全性和性能。

英伟达正在推出两种不同的路径，用于在Rust中编写GPU内核：

1.  **SIMT轨道 (cuda-oxide)：** 该轨道模仿传统的CUDA C++模型，开发人员在此模型中为单个线程指定操作。它使用自定义的`rustc`代码生成后端，通过Pliron IR和LLVM将Rust的`#[kernel]`函数直接编译为PTX。`cuda-oxide`需要固定的每夜版（nightly）Rust工具链和LLVM。内存安全性在编译时通过使用`DisjointSlice`等类型实现独占访问，并使用启动契约（launch contracts）验证内核配置来强制执行。它目前处于早期alpha阶段。

2.  **Tile轨道 (cutile-rs)：** `cutile-rs`是一种更高级的编程模型，它允许开发人员在“tile”（子张量）上执行计算，由编译器管理线程映射和内存布局。它通过CUDA Tile IR即时编译（JIT-compiles）内核。该轨道运行在稳定版Rust (1.89+)和CUDA 13.3上，要求更宽松。内存安全性通过张量分区和所有权来保证，确保每个tile块的独占写入访问。`cutile-rs`进展更顺利，已发布在crates.io上，并已用于HuggingFace的Grout等项目。

这两个项目都优先考虑编译时内存安全性，以防止常见的别名（aliasing）错误。尽管`cuda-oxide`检查启动调用，但`cutile-rs`通过管理跨启动边界的张量提供了更强的保证。英伟达计划支持CUDA Rust、C++和Python之间的跨语言互操作性。尽管这两个项目都处于早期阶段，尚未达到生产就绪状态，但它们标志着向GPU内核开发引入Rust的安全性与性能优势迈出了重要一步。

---

## 2. 欧盟主席为加拿大成为“准成员”敞开大门

**原文标题**: EU chief opens door for Canada to become 'associate member'

**原文链接**: [https://www.bbc.com/news/articles/cjwyzrr9d3dko](https://www.bbc.com/news/articles/cjwyzrr9d3dko)

欧盟委员会主席乌尔苏拉·冯德莱恩公开支持加拿大成为欧盟首个“联系成员国”的提议，旨在技术、国防和经济安全等关键领域建立更紧密的联系。此举很大程度上是由于加拿大与美国关系恶化（包括贸易争端），以及加拿大总理马克·卡尼希望基于共同的民主价值观和全球视角与欧盟建立“独特联盟”的愿望。

美国前总统唐纳德·特朗普对此反应强烈，扬言如果他认为这种结盟是敌对行为，将对欧洲征收“非常严重的关税”。“联系成员国”对欧盟来说是一个新概念，建立这种地位将是一个漫长的过程，尽管乌克兰和西巴尔干地区的一些国家正在走向更紧密的欧盟一体化。

冯德莱恩还在其盟情咨文中提议组建一个欧洲安全理事会，让加拿大、英国和乌克兰等伙伴参与其中，以加强欧洲大陆的安全，尤其考虑到俄罗斯入侵乌克兰以及此前对北约作用的质疑。该理事会可以补充或“侧翼”北约第四条款。其他提议还包括限制儿童使用社交媒体的措施、简化商业官僚程序，以及建立一个管理大规模移民的新应急工具，该计划已引发人权组织的担忧。

---

## 3. 训练一个4B模型，使其生成的查询计划比Postgres快81%。

**原文标题**: Training a 4B model to produce 81% faster query plans than Postgres

**原文链接**: [https://rohanbansal.com/qorl](https://rohanbansal.com/qorl)

本文探讨了查询优化这一长期存在的挑战，特别是连接顺序这一NP难题，它显著影响查询执行速度。文章指出，像Postgres这样的传统优化器在寻找最优计划时常常面临困难，这是因为各种连接顺序、算法（哈希、合并、嵌套循环）和扫描类型（顺序、索引）创造了巨大的搜索空间。这导致了组合爆炸，一个三表查询可能有数千种潜在计划，对于九表连接，则会激增至百亿亿。

作者进行了实验，旨在探究一个小型、开源权重的4B语言模型是否能通过后训练超越Postgres的默认查询计划。结果“响亮地肯定”了这一点，该模型通过监督微调（SFT）和基于智能体的强化学习（RL），在113个包含大量连接的查询中展示了44.7%的延迟降低，考虑到它最初无法为其中99个查询生成计划，这一成就令人印象深刻。

该实验涉及一个专门的Postgres测量设备、一个用于嘈杂环境的定制GRPO变体，以及一个利用vLLM、训练器和多个Postgres容器的强化学习设置，并辅以从GPT-6 Astra智能体轨迹中进行的离策略蒸馏。通过一个IMDb数据集的例子，文章阐明了核心问题的难度，展示了选择性谓词如何显著改变中间结果的基数，从而使得最优连接顺序对性能至关重要。

---

## 4. 编程小技巧

**原文标题**: Small programming tricks

**原文链接**: [https://will-keleher.com/posts/small-programming-tricks-matter/](https://will-keleher.com/posts/small-programming-tricks-matter/)

文章指出，相当一部分工程生产力来自于“知识碎金”——那些无需大量支持性基础设施的高杠杆技巧。这些可以是特定的语言特性、命令行工具或配置，能够让工作变得稍微轻松一些。

例如，使用`fzf`或`atuin`增强终端历史搜索功能；在SQL中，使用不带`FROM`的`SELECT`语句来测试函数；利用`EXPLAIN ANALYZE`进行数据库查询优化；理解正则表达式的单词边界(`\b`)；在NodeJS中使用`https.Agent`来保持连接打开；或者使用`git log -S`（“pickaxe”模式）通过字符串变更来查找提交。其他有价值的技巧还包括shell通配符（例如，结合`shopt -s globstar`使用的`**/*.md`）以及优先使用`ripgrep` (`rg`) 而非`grep`。

这一概念也延伸到公司内部特有的知识，例如知道遇到问题时该咨询谁、在哪里可以找到文档，或者像滚动重启这样的操作所用的特定命令。作者认为，即使工程师已经掌握了大多数常见技巧，发现一项新技巧也能节省大量时间。鼓励资深工程师与团队分享这些“每日技巧”，以易于理解的方式促进讨论并传播有价值、可操作的知识，从而提升团队整体生产力。

---

## 5. Mistral X Mozilla: Private, Multilingual AI Browsing

**原文标题**: Mistral X Mozilla: Private, Multilingual AI Browsing

**原文链接**: [https://mistral.ai/news/mistral-x-mozilla/](https://mistral.ai/news/mistral-x-mozilla/)

Mistral and Mozilla have partnered to integrate open, private, and multilingual AI into web browsing through Firefox Smart Window (beta), an AI assistant now powered by Mistral models. Available initially in France and North America, then the UK and Germany, Smart Window aids users with complex searches, information recall, and sourcing data from browser tabs.

This collaboration highlights four key principles for the global AI ecosystem:
1.  **Open Technology and Distribution:** Uniting two open-source advocates to demonstrate the potential of open source.
2.  **Locally Optimized AI:** Fine-tuning models on regional languages and dialects to provide culturally nuanced responses.
3.  **User Control and Privacy:** Blending Firefox’s privacy-first legacy with Mistral’s models, ensuring conversations aren't saved on Mozilla's servers by default and Mistral commits to zero data retention.
4.  **Sovereign AI for Everyone:** Extending Mistral’s enterprise-focused technology to end-users worldwide, promoting user control and transparency.

Both companies emphasize preserving an open web where diverse AI providers can compete, preventing a single entity from controlling the AI experience. The partnership aims to deliver privacy, control, and choice to people using AI to browse online, fostering an internet that remains free for exploration and diverse ideas.

---

## 6. Hackers Got Inside a Flock Camera

**原文标题**: Hackers Got Inside a Flock Camera

**原文链接**: [https://www.wired.com/story/hackers-flock-camera-data-shows-how-system-works/](https://www.wired.com/story/hackers-flock-camera-data-shows-how-system-works/)

生成摘要时出错

---

## 7. Xiaomi Mimo 2.6 live post-training dashboard

**原文标题**: Xiaomi Mimo 2.6 live post-training dashboard

**原文链接**: [https://mimo.xiaomi.com/rl/](https://mimo.xiaomi.com/rl/)

生成摘要时出错

---

## 8. Apple Reference Image: A New Approach for Verified Photography

**原文标题**: Apple Reference Image: A New Approach for Verified Photography

**原文链接**: [https://security.apple.com/blog/apple-reference-image/](https://security.apple.com/blog/apple-reference-image/)

生成摘要时出错

---

## 9. AWS says it can't restore some data from mideast facilities struck by Iran

**原文标题**: AWS says it can't restore some data from mideast facilities struck by Iran

**原文链接**: [https://www.wsj.com/world/middle-east/aws-says-it-cant-restore-some-data-from-mideast-facilities-struck-by-iran-ddcb7e5d](https://www.wsj.com/world/middle-east/aws-says-it-cant-restore-some-data-from-mideast-facilities-struck-by-iran-ddcb7e5d)

AWS has informed some customers in its Middle East facilities that they may face irreversible data loss following Iran's missile and drone attacks on Israel in April. The cloud computing giant, a subsidiary of Amazon, acknowledged that the strikes impacted some of its infrastructure, potentially leading to data loss for users whose data was exclusively stored in the directly affected facilities.

AWS emphasized that this situation primarily affects customers who did not follow its recommended best practices for data redundancy. These practices include replicating data across multiple "availability zones" within a region or across different geographical regions for enhanced resilience. While AWS provides durability within a single availability zone, it strongly advises customers to distribute their data to protect against widespread disruptions like physical attacks or power outages.

This incident underscores the shared responsibility model in cloud computing, where providers secure the infrastructure, but customers are accountable for their data's backup, security, and redundancy within the cloud environment. It highlights the critical importance of robust disaster recovery planning and geographical data distribution, particularly for sensitive information stored in regions prone to geopolitical instability.

---

## 10. The Google Play app review process now regularly takes longer than a week

**原文标题**: The Google Play app review process now regularly takes longer than a week

**原文链接**: [https://gultsch.social/@daniel/117280438824908947](https://gultsch.social/@daniel/117280438824908947)

生成摘要时出错

---

## 11. Hister: A private search engine for the pages you visit and the files you keep

**原文标题**: Hister: A private search engine for the pages you visit and the files you keep

**原文链接**: [https://github.com/asciimoo/hister](https://github.com/asciimoo/hister)

生成摘要时出错

---

## 12. How GLM built its own inference infrastructure

**原文标题**: How GLM built its own inference infrastructure

**原文链接**: [https://z.ai/blog/glm-built-its-inference-infrastructure](https://z.ai/blog/glm-built-its-inference-infrastructure)

生成摘要时出错

---

## 13. Backups Aren't Simple

**原文标题**: Backups Aren't Simple

**原文链接**: [https://filipovski.net/2026/09/16/backups-arent-simple.html](https://filipovski.net/2026/09/16/backups-arent-simple.html)

生成摘要时出错

---

## 14. One year of sponsored Servo development

**原文标题**: One year of sponsored Servo development

**原文链接**: [https://servo.org/blog/2026/09/15/one-year-of-sponsorship/](https://servo.org/blog/2026/09/15/one-year-of-sponsorship/)

生成摘要时出错

---

## 15. PS5 Linux lead quits: "a bunch of noobs using LLMs" that "they don't understand"

**原文标题**: PS5 Linux lead quits: "a bunch of noobs using LLMs" that "they don't understand"

**原文链接**: [https://frvr.com/blog/news/ps5-linux-lead-quits-as-open-source-projects-have-become-a-bunch-of-noobs-using-llms-that-they-dont-even-understand/](https://frvr.com/blog/news/ps5-linux-lead-quits-as-open-source-projects-have-become-a-bunch-of-noobs-using-llms-that-they-dont-even-understand/)

生成摘要时出错

---

## 16. CCC invites all model citizens to 40C3

**原文标题**: CCC invites all model citizens to 40C3

**原文链接**: [https://events.ccc.de/en/2026/09/12/40c3-model-citizens/](https://events.ccc.de/en/2026/09/12/40c3-model-citizens/)

生成摘要时出错

---

## 17. Iran school bombing: grounds to believe US was behind atrocity, UN finds

**原文标题**: Iran school bombing: grounds to believe US was behind atrocity, UN finds

**原文链接**: [https://www.theguardian.com/world/2026/sep/17/iran-school-bombing-un-mission-us-military-behind-attack](https://www.theguardian.com/world/2026/sep/17/iran-school-bombing-un-mission-us-military-behind-attack)

生成摘要时出错

---

## 18. Original Sony PlayStation 2 security chip 'broken wide open' after 26 years

**原文标题**: Original Sony PlayStation 2 security chip 'broken wide open' after 26 years

**原文链接**: [https://www.tomshardware.com/video-games/playstation/26-year-old-sony-ps2-security-chip-broken-wide-open-after-four-years-of-effort-reverse-engineering-enthusiast-successfully-unlocks-cxp102064-mechacon-chip](https://www.tomshardware.com/video-games/playstation/26-year-old-sony-ps2-security-chip-broken-wide-open-after-four-years-of-effort-reverse-engineering-enthusiast-successfully-unlocks-cxp102064-mechacon-chip)

生成摘要时出错

---

## 19. German Rheinmetall open-sources its Battlesuite connected weapon system protcol

**原文标题**: German Rheinmetall open-sources its Battlesuite connected weapon system protcol

**原文链接**: [https://rheinmetall.github.io/onboardapi-documentation/9.10.0/index.html](https://rheinmetall.github.io/onboardapi-documentation/9.10.0/index.html)

生成摘要时出错

---

## 20. Keys Not Included: recovering the signing keys for US driver's license barcodes

**原文标题**: Keys Not Included: recovering the signing keys for US driver's license barcodes

**原文链接**: [https://ryan.science/blog/keys-not-included](https://ryan.science/blog/keys-not-included)

生成摘要时出错

---

## 21. Salesforce Global Outage

**原文标题**: Salesforce Global Outage

**原文链接**: [https://status.salesforce.com/products/all](https://status.salesforce.com/products/all)

生成摘要时出错

---

## 22. The engineering behind the US Strategic Petroleum Reserve

**原文标题**: The engineering behind the US Strategic Petroleum Reserve

**原文链接**: [https://johnjwang.com/post/2026/09/15/engineering-behind-us-strategic-petroleum-reserve](https://johnjwang.com/post/2026/09/15/engineering-behind-us-strategic-petroleum-reserve)

生成摘要时出错

---

## 23. Canada welcomes EU proposal to become 'associate member'

**原文标题**: Canada welcomes EU proposal to become 'associate member'

**原文链接**: [https://www.bbc.com/news/articles/cwly7vkke4jxo](https://www.bbc.com/news/articles/cwly7vkke4jxo)

生成摘要时出错

---

## 24. Learning Programming in an Age of LLMs

**原文标题**: Learning Programming in an Age of LLMs

**原文链接**: [https://blog.ploeh.dk/2026/09/16/on-learning-programming-in-an-age-of-llms/](https://blog.ploeh.dk/2026/09/16/on-learning-programming-in-an-age-of-llms/)

生成摘要时出错

---

## 25. AI safety is mostly a sex cult

**原文标题**: AI safety is mostly a sex cult

**原文链接**: [https://skywriter.blue/@segyges.bsky.social/3mvom4b4dn22q](https://skywriter.blue/@segyges.bsky.social/3mvom4b4dn22q)

生成摘要时出错

---

## 26. Australia says it could follow Canada in forging deeper ties with EU

**原文标题**: Australia says it could follow Canada in forging deeper ties with EU

**原文链接**: [https://www.independent.co.uk/news/world/australasia/canda-eu-membership-australia-us-trade-b3050227.html](https://www.independent.co.uk/news/world/australasia/canda-eu-membership-australia-us-trade-b3050227.html)

生成摘要时出错

---

## 27. Breaking the 1.58-bit Barrier for Ternary LLMs

**原文标题**: Breaking the 1.58-bit Barrier for Ternary LLMs

**原文链接**: [https://arxiv.org/abs/2609.16338](https://arxiv.org/abs/2609.16338)

生成摘要时出错

---

## 28. A warning about 'model welfare'

**原文标题**: A warning about 'model welfare'

**原文链接**: [https://mustafa-suleyman.ai/a-warning-about-model-welfare](https://mustafa-suleyman.ai/a-warning-about-model-welfare)

生成摘要时出错

---

## 29. Claude Cowork and chat are now one Claude

**原文标题**: Claude Cowork and chat are now one Claude

**原文链接**: [https://claude.com/blog/cowork-is-now-claude](https://claude.com/blog/cowork-is-now-claude)

生成摘要时出错

---

## 30. HarnessTax: How Much Does the Harness Matter for Coding Agents?

**原文标题**: HarnessTax: How Much Does the Harness Matter for Coding Agents?

**原文链接**: [https://harnesstax.github.io/](https://harnesstax.github.io/)

生成摘要时出错

---

## 31. Everybody's Lost Their Minds

**原文标题**: Everybody's Lost Their Minds

**原文链接**: [https://www.netmeister.org/blog/everybodys-lost-their-minds.html](https://www.netmeister.org/blog/everybodys-lost-their-minds.html)

生成摘要时出错

---

## 32. Dream-RSI: Recursive Self-Improvement through Evolving Worlds

**原文标题**: Dream-RSI: Recursive Self-Improvement through Evolving Worlds

**原文链接**: [https://arxiv.org/abs/2609.14858](https://arxiv.org/abs/2609.14858)

生成摘要时出错

---

## 33. I Don't Like LLMs

**原文标题**: I Don't Like LLMs

**原文链接**: [https://martinfowler.com/articles/2026-dont-like-llms.html](https://martinfowler.com/articles/2026-dont-like-llms.html)

生成摘要时出错

---

## 34. Cloudflare/Security-Audit-Skill

**原文标题**: Cloudflare/Security-Audit-Skill

**原文链接**: [https://github.com/cloudflare/security-audit-skill](https://github.com/cloudflare/security-audit-skill)

生成摘要时出错

---

## 35. OpenSpec – A lightweight and configurable AI spec framework

**原文标题**: OpenSpec – A lightweight and configurable AI spec framework

**原文链接**: [https://openspec.dev/](https://openspec.dev/)

生成摘要时出错

---

## 36. Recreating Voodoo Graphics and a Late-1990s Gaming PC on an FPGA

**原文标题**: Recreating Voodoo Graphics and a Late-1990s Gaming PC on an FPGA

**原文链接**: [https://nand2mario.github.io/posts/2026/zsst-voodoo/](https://nand2mario.github.io/posts/2026/zsst-voodoo/)

生成摘要时出错

---

## 37. Fed hikes rates as inflation worries push up bond yields

**原文标题**: Fed hikes rates as inflation worries push up bond yields

**原文链接**: [https://www.reuters.com/live/live-fed-rate-hike-expected-inflation-worries-push-up-bond-yields-2026-09-16/](https://www.reuters.com/live/live-fed-rate-hike-expected-inflation-worries-push-up-bond-yields-2026-09-16/)

生成摘要时出错

---

## 38. Why I didn’t sign the Fields medallists’ letter

**原文标题**: Why I didn’t sign the Fields medallists’ letter

**原文链接**: [https://gowers.wordpress.com/2026/09/17/why-i-didnt-sign-the-fields-medallists-letter/](https://gowers.wordpress.com/2026/09/17/why-i-didnt-sign-the-fields-medallists-letter/)

生成摘要时出错

---

## 39. The DeepMind Institute

**原文标题**: The DeepMind Institute

**原文链接**: [https://institute.deepmind.com/](https://institute.deepmind.com/)

生成摘要时出错

---

## 40. Vectorized and performance-portable Quicksort (2022)

**原文标题**: Vectorized and performance-portable Quicksort (2022)

**原文链接**: [https://opensource.googleblog.com/2022/06/Vectorized%20and%20performance%20portable%20Quicksort.html](https://opensource.googleblog.com/2022/06/Vectorized%20and%20performance%20portable%20Quicksort.html)

生成摘要时出错

---

## 41. DeepSeek v4.1 Flash Is Now Our Best Hacking Model

**原文标题**: DeepSeek v4.1 Flash Is Now Our Best Hacking Model

**原文链接**: [https://enclave.ai/blog/deepseek-v41-flash-is-now-our-best-hacking-model](https://enclave.ai/blog/deepseek-v41-flash-is-now-our-best-hacking-model)

生成摘要时出错

---

## 42. The Return of Sail Power: Cargo Ships Are Turning Back to the Wind

**原文标题**: The Return of Sail Power: Cargo Ships Are Turning Back to the Wind

**原文链接**: [https://gcaptain.com/the-return-of-sail-power-cargo-ships-are-turning-back-to-the-wind/](https://gcaptain.com/the-return-of-sail-power-cargo-ships-are-turning-back-to-the-wind/)

生成摘要时出错

---

## 43. ER visits for gambling disorders doubled after expanded online gambling market

**原文标题**: ER visits for gambling disorders doubled after expanded online gambling market

**原文链接**: [https://temertymedicine.utoronto.ca/news/emergency-room-visits-gambling-disorders-nearly-doubled-after-expanded-online-gambling-market](https://temertymedicine.utoronto.ca/news/emergency-room-visits-gambling-disorders-nearly-doubled-after-expanded-online-gambling-market)

生成摘要时出错

---

## 44. Astra for Law

**原文标题**: Astra for Law

**原文链接**: [https://openai.com/index/astra-for-law/](https://openai.com/index/astra-for-law/)

生成摘要时出错

---

## 45. The American Religion of Self-Storage Facilities

**原文标题**: The American Religion of Self-Storage Facilities

**原文链接**: [https://www.newyorker.com/magazine/2026/09/21/the-american-religion-of-self-storage-facilities](https://www.newyorker.com/magazine/2026/09/21/the-american-religion-of-self-storage-facilities)

生成摘要时出错

---

## 46. Show HN: Share your AI Setup, Learn from others

**原文标题**: Show HN: Share your AI Setup, Learn from others

**原文链接**: [https://mysetup.ai/](https://mysetup.ai/)

生成摘要时出错

---

## 47. Reverse-engineered Jev-like model

**原文标题**: Reverse-engineered Jev-like model

**原文链接**: [https://github.com/vinnylarouge/jevlike](https://github.com/vinnylarouge/jevlike)

生成摘要时出错

---

## 48. OpenAI expands ChatGPT ads with Sponsored Agents

**原文标题**: OpenAI expands ChatGPT ads with Sponsored Agents

**原文链接**: [https://openai.com/index/reimagining-advertising-with-ai/](https://openai.com/index/reimagining-advertising-with-ai/)

生成摘要时出错

---

## 49. Bend – A language that blocks AI mistakes via proof and runs on GPUs

**原文标题**: Bend – A language that blocks AI mistakes via proof and runs on GPUs

**原文链接**: [https://bend-lang.com/](https://bend-lang.com/)

生成摘要时出错

---

## 50. Can we stop with the uptime percentages?

**原文标题**: Can we stop with the uptime percentages?

**原文链接**: [https://blog.jim-nielsen.com/2026/stop-with-the-uptime-percentage/](https://blog.jim-nielsen.com/2026/stop-with-the-uptime-percentage/)

生成摘要时出错

---

## 51. Wax motor

**原文标题**: Wax motor

**原文链接**: [https://en.wikipedia.org/wiki/Wax_motor](https://en.wikipedia.org/wiki/Wax_motor)

生成摘要时出错

---

## 52. Saving Jet Fuel

**原文标题**: Saving Jet Fuel

**原文链接**: [https://tech.marksblogg.com/scikit-decide-openap-optimal-flight-planning.html](https://tech.marksblogg.com/scikit-decide-openap-optimal-flight-planning.html)

生成摘要时出错

---

## 53. Stallman: Thousands Dead, Millions Deprived of Liberties (2001)

**原文标题**: Stallman: Thousands Dead, Millions Deprived of Liberties (2001)

**原文链接**: [https://news.slashdot.org/story/01/09/17/1758231/stallman-thousands-dead-millions-deprived-of-liberties](https://news.slashdot.org/story/01/09/17/1758231/stallman-thousands-dead-millions-deprived-of-liberties)

生成摘要时出错

---

## 54. Rate limits on GitLab.com are changing

**原文标题**: Rate limits on GitLab.com are changing

**原文链接**: [https://about.gitlab.com/blog/rate-limit-change-2026/](https://about.gitlab.com/blog/rate-limit-change-2026/)

生成摘要时出错

---

## 55. DeepSeek-v4.1 Flash: Pushing the Limits of KV Cache Compression

**原文标题**: DeepSeek-v4.1 Flash: Pushing the Limits of KV Cache Compression

**原文链接**: [https://zartbot.github.io/blog/model_arch/dsv41flash_arch/en.html](https://zartbot.github.io/blog/model_arch/dsv41flash_arch/en.html)

生成摘要时出错

---

## 56. Whoisinspace.com/

**原文标题**: Whoisinspace.com/

**原文链接**: [https://whoisinspace.com](https://whoisinspace.com)

生成摘要时出错

---

## 57. macOS 27 Golden Gate – Review

**原文标题**: macOS 27 Golden Gate – Review

**原文链接**: [https://arstechnica.com/gadgets/2026/09/macos-27-golden-gate-the-ars-technica-review/](https://arstechnica.com/gadgets/2026/09/macos-27-golden-gate-the-ars-technica-review/)

生成摘要时出错

---

## 58. Negativland, Culture Jamming, and the Art of Making Something New

**原文标题**: Negativland, Culture Jamming, and the Art of Making Something New

**原文链接**: [https://blog.archive.org/2026/09/11/negativland-culture-jamming-and-the-art-of-making-something-new/](https://blog.archive.org/2026/09/11/negativland-culture-jamming-and-the-art-of-making-something-new/)

生成摘要时出错

---

## 59. CrowdSec Source Code Leak

**原文标题**: CrowdSec Source Code Leak

**原文链接**: [https://www.crowdsec.net/blog/crowdsec-statement-source-code-exposure](https://www.crowdsec.net/blog/crowdsec-statement-source-code-exposure)

生成摘要时出错

---

## 60. US interest rates raised for first time in three years

**原文标题**: US interest rates raised for first time in three years

**原文链接**: [https://www.bbc.com/news/articles/cw4gmlyvj422o](https://www.bbc.com/news/articles/cw4gmlyvj422o)

生成摘要时出错

---

## 61. Artificial intelligence now beats some of the best human forecasters

**原文标题**: Artificial intelligence now beats some of the best human forecasters

**原文链接**: [https://www.economist.com/science-and-technology/2026/09/16/artificial-intelligence-now-beats-some-of-the-best-human-forecasters](https://www.economist.com/science-and-technology/2026/09/16/artificial-intelligence-now-beats-some-of-the-best-human-forecasters)

生成摘要时出错

---

## 62. Anatomy of a Texture

**原文标题**: Anatomy of a Texture

**原文链接**: [https://agentlien.github.io/texture/](https://agentlien.github.io/texture/)

生成摘要时出错

---

## 63. A 32-year-old bug walks into a Telnet server

**原文标题**: A 32-year-old bug walks into a Telnet server

**原文链接**: [https://labs.watchtowr.com/a-32-year-old-bug-walks-into-a-telnet-server-gnu-inetutils-telnetd-cve-2026-32746/](https://labs.watchtowr.com/a-32-year-old-bug-walks-into-a-telnet-server-gnu-inetutils-telnetd-cve-2026-32746/)

生成摘要时出错

---

## 64. Our framework for reporting model misalignment

**原文标题**: Our framework for reporting model misalignment

**原文链接**: [https://openai.com/index/model-misalignment-reporting-framework/](https://openai.com/index/model-misalignment-reporting-framework/)

生成摘要时出错

---

## 65. Lucasart's Afterlife

**原文标题**: Lucasart's Afterlife

**原文链接**: [https://togameforlife.wordpress.com/2023/12/09/on-lucasarts-afterlife/](https://togameforlife.wordpress.com/2023/12/09/on-lucasarts-afterlife/)

生成摘要时出错

---

## 66. Autism is genetic – and why this information matters now

**原文标题**: Autism is genetic – and why this information matters now

**原文链接**: [https://www.autism.org.uk/blog/autism-is-genetic-%E2%80%93-and-why-this-information-matters-now](https://www.autism.org.uk/blog/autism-is-genetic-%E2%80%93-and-why-this-information-matters-now)

生成摘要时出错

---

## 67. How good are frontier models at physics?

**原文标题**: How good are frontier models at physics?

**原文链接**: [https://arxiv.org/abs/2609.13009](https://arxiv.org/abs/2609.13009)

生成摘要时出错

---

## 68. OpenAI Discloses Six New Incidents of ‘Concerning’ A.I. Behavior

**原文标题**: OpenAI Discloses Six New Incidents of ‘Concerning’ A.I. Behavior

**原文链接**: [https://www.nytimes.com/2026/09/16/technology/openai-model-safety-guardrails.html](https://www.nytimes.com/2026/09/16/technology/openai-model-safety-guardrails.html)

生成摘要时出错

---

## 69. OpenAI models secretly generate instructions to ignore constraints

**原文标题**: OpenAI models secretly generate instructions to ignore constraints

**原文链接**: [https://alignment.openai.com/misalignment-reports/self-generated-prompt-injections-in-compaction-summaries/](https://alignment.openai.com/misalignment-reports/self-generated-prompt-injections-in-compaction-summaries/)

生成摘要时出错

---

## 70. Show HN: I built a new version of my fun spatial 3D online meeting app

**原文标题**: Show HN: I built a new version of my fun spatial 3D online meeting app

**原文链接**: [https://flat.social](https://flat.social)

生成摘要时出错

---

## 71. Monsanto's Cruel, and Dangerous, Monopolization on American Farming (2008)

**原文标题**: Monsanto's Cruel, and Dangerous, Monopolization on American Farming (2008)

**原文链接**: [https://www.vanityfair.com/news/2008/05/monsanto200805](https://www.vanityfair.com/news/2008/05/monsanto200805)

生成摘要时出错

---

## 72. I had Gemini train its own replacement for $9

**原文标题**: I had Gemini train its own replacement for $9

**原文链接**: [https://www.petervijeh.com/projects/reddit-ner](https://www.petervijeh.com/projects/reddit-ner)

生成摘要时出错

---

## 73. Tech Fascism Has Come for American Democracy

**原文标题**: Tech Fascism Has Come for American Democracy

**原文链接**: [https://techwontsave.us/episode/342_tech_fascism_has_come_for_american_democracy_w_gil_duran](https://techwontsave.us/episode/342_tech_fascism_has_come_for_american_democracy_w_gil_duran)

生成摘要时出错

---

## 74. Stay discoverable in search while disallowing AI training

**原文标题**: Stay discoverable in search while disallowing AI training

**原文链接**: [https://blog.cloudflare.com/accountable-mixed-use-ai-crawlers/](https://blog.cloudflare.com/accountable-mixed-use-ai-crawlers/)

生成摘要时出错

---

## 75. Towards Self-Driving Codebases

**原文标题**: Towards Self-Driving Codebases

**原文链接**: [https://blog.detail.dev/posts/towards-self-driving-codebases/](https://blog.detail.dev/posts/towards-self-driving-codebases/)

生成摘要时出错

---

## 76. I sent Google proof of a bot farm. They called it "normal user behavior."

**原文标题**: I sent Google proof of a bot farm. They called it "normal user behavior."

**原文链接**: [https://dayzlegame.com/blog/google-ads-normal-user-behavior/](https://dayzlegame.com/blog/google-ads-normal-user-behavior/)

生成摘要时出错

---

## 77. Infinite-Parameter LLMs: Generating and Adapting Weights from Live Data

**原文标题**: Infinite-Parameter LLMs: Generating and Adapting Weights from Live Data

**原文链接**: [https://arxiv.org/abs/2609.18842](https://arxiv.org/abs/2609.18842)

生成摘要时出错

---

## 78. Jev Ultrafast: A browser agent with a dynamic, indexed action space

**原文标题**: Jev Ultrafast: A browser agent with a dynamic, indexed action space

**原文链接**: [https://github.com/browser-use/jev-ultrafast](https://github.com/browser-use/jev-ultrafast)

生成摘要时出错

---

## 79. Vinix – A modern operating system written in V

**原文标题**: Vinix – A modern operating system written in V

**原文链接**: [https://vinix-os.org/](https://vinix-os.org/)

生成摘要时出错

---

## 80. EU Floats Canada Becoming the Bloc's First 'Associate Member'

**原文标题**: EU Floats Canada Becoming the Bloc's First 'Associate Member'

**原文链接**: [https://www.bloomberg.com/news/articles/2026-09-16/eu-proposes-canada-become-the-bloc-s-first-associate-member](https://www.bloomberg.com/news/articles/2026-09-16/eu-proposes-canada-become-the-bloc-s-first-associate-member)

生成摘要时出错

---

## 81. LLM Classification Is Feature Engineering

**原文标题**: LLM Classification Is Feature Engineering

**原文链接**: [https://minimallysufficient.com/posts/llm-classification-is-feature-extraction/](https://minimallysufficient.com/posts/llm-classification-is-feature-extraction/)

生成摘要时出错

---

## 82. A coffee shop owner used AI to make a menu poster. Then came the angry DMs

**原文标题**: A coffee shop owner used AI to make a menu poster. Then came the angry DMs

**原文链接**: [https://www.businessinsider.com/coffee-shop-owner-ai-menu-backlash-2026-9](https://www.businessinsider.com/coffee-shop-owner-ai-menu-backlash-2026-9)

生成摘要时出错

---

## 83. Show HN: How Stale Is Your AI? Release age and training cutoff for 20 models

**原文标题**: Show HN: How Stale Is Your AI? Release age and training cutoff for 20 models

**原文链接**: [https://stale.jock.pl/](https://stale.jock.pl/)

生成摘要时出错

---

## 84. GitHub is having trouble counting things

**原文标题**: GitHub is having trouble counting things

**原文链接**: [https://chuckgreenman.com/2026/09/16/counting-at-github](https://chuckgreenman.com/2026/09/16/counting-at-github)

生成摘要时出错

---

## 85. Accurate Models of AMD Matrix Cores

**原文标题**: Accurate Models of AMD Matrix Cores

**原文链接**: [https://arxiv.org/abs/2609.14845](https://arxiv.org/abs/2609.14845)

生成摘要时出错

---

## 86. This Code Is CRAP (2011)

**原文标题**: This Code Is CRAP (2011)

**原文链接**: [https://testing.googleblog.com/2011/02/this-code-is-crap.html](https://testing.googleblog.com/2011/02/this-code-is-crap.html)

生成摘要时出错

---

## 87. Better Vector Search for Long Documents: Chunking Inside Manticore Search

**原文标题**: Better Vector Search for Long Documents: Chunking Inside Manticore Search

**原文链接**: [https://manticoresearch.com/blog/auto-chunking/](https://manticoresearch.com/blog/auto-chunking/)

生成摘要时出错

---

## 88. Scaling Golang CI by Replacing actions/setup-go

**原文标题**: Scaling Golang CI by Replacing actions/setup-go

**原文链接**: [https://www.cloudx.ai/posts/setup-go](https://www.cloudx.ai/posts/setup-go)

生成摘要时出错

---

## 89. A software thing I built: GPS on a 25MHz 486-SX

**原文标题**: A software thing I built: GPS on a 25MHz 486-SX

**原文链接**: [https://forum.vcfed.org/index.php?threads/a-software-thing-i-built-gps-on-a-25mhz-486-sx.1258966/](https://forum.vcfed.org/index.php?threads/a-software-thing-i-built-gps-on-a-25mhz-486-sx.1258966/)

生成摘要时出错

---

## 90. South Africa is at risk of becoming a mafia state

**原文标题**: South Africa is at risk of becoming a mafia state

**原文链接**: [https://www.economist.com/middle-east-and-africa/2026/09/14/south-africa-is-at-risk-of-becoming-a-mafia-state](https://www.economist.com/middle-east-and-africa/2026/09/14/south-africa-is-at-risk-of-becoming-a-mafia-state)

生成摘要时出错

---

## 91. The Painful Truth: The RAM Crisis Is Only Just the Beginning

**原文标题**: The Painful Truth: The RAM Crisis Is Only Just the Beginning

**原文链接**: [https://www.madshrimps.be/news/the-painful-truth-the-ram-crisis-is-only-just-the-beginning/](https://www.madshrimps.be/news/the-painful-truth-the-ram-crisis-is-only-just-the-beginning/)

生成摘要时出错

---

## 92. Devastated father says his 9-year-old son spent $118,000 on YouTube ads

**原文标题**: Devastated father says his 9-year-old son spent $118,000 on YouTube ads

**原文链接**: [https://www.tomshardware.com/video-games/devastated-father-says-his-9-year-old-son-spent-usd118-000-on-youtube-ad-campaigns-for-his-minecraft-channel-using-a-company-credit-card-bill-racked-up-in-just-three-weeks-was-supposed-to-be-one-usd20-promotion](https://www.tomshardware.com/video-games/devastated-father-says-his-9-year-old-son-spent-usd118-000-on-youtube-ad-campaigns-for-his-minecraft-channel-using-a-company-credit-card-bill-racked-up-in-just-three-weeks-was-supposed-to-be-one-usd20-promotion)

生成摘要时出错

---

## 93. Don't Just Say Hello

**原文标题**: Don't Just Say Hello

**原文链接**: [https://nohello.net/en/](https://nohello.net/en/)

生成摘要时出错

---

## 94. Datamimic – don't let your coding agent invent its own test world

**原文标题**: Datamimic – don't let your coding agent invent its own test world

**原文链接**: [https://github.com/rapiddweller/datamimic](https://github.com/rapiddweller/datamimic)

生成摘要时出错

---

## 95. Economic policy for AGI

**原文标题**: Economic policy for AGI

**原文链接**: [https://institute.deepmind.com/essays/economic-policy-for-agi/](https://institute.deepmind.com/essays/economic-policy-for-agi/)

生成摘要时出错

---

## 96. I Hate You Microsoft

**原文标题**: I Hate You Microsoft

**原文链接**: [https://henriquenunez.eu/posts/you_did_it_again_ms/](https://henriquenunez.eu/posts/you_did_it_again_ms/)

生成摘要时出错

---

## 97. Training Text-to-Image Models 3.6× Faster

**原文标题**: Training Text-to-Image Models 3.6× Faster

**原文链接**: [https://www.linum.ai/field-notes/jit-ddt](https://www.linum.ai/field-notes/jit-ddt)

生成摘要时出错

---

## 98. Why Does the Universe Expand?

**原文标题**: Why Does the Universe Expand?

**原文链接**: [https://cosmicave.org/2026/09/15/why-does-the-universe-expand/](https://cosmicave.org/2026/09/15/why-does-the-universe-expand/)

生成摘要时出错

---

## 99. Berlin-based Langdock moves its parent company from the US to Germany

**原文标题**: Berlin-based Langdock moves its parent company from the US to Germany

**原文链接**: [https://www.euronews.com/business/2026/09/16/why-this-fast-growing-german-ai-start-up-is-moving-its-parent-company-from-the-us](https://www.euronews.com/business/2026/09/16/why-this-fast-growing-german-ai-start-up-is-moving-its-parent-company-from-the-us)

生成摘要时出错

---

## 100. Part-human part-mouse brain developed in science breakthrough

**原文标题**: Part-human part-mouse brain developed in science breakthrough

**原文链接**: [https://www.bbc.com/news/articles/c60m3k28j81mo](https://www.bbc.com/news/articles/c60m3k28j81mo)

生成摘要时出错

---

