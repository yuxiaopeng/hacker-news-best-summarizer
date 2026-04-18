# Hacker News 热门文章摘要 (2026-04-18)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 克劳德设计

**原文标题**: Claude Design

**原文链接**: [https://www.anthropic.com/news/claude-design-anthropic-labs](https://www.anthropic.com/news/claude-design-anthropic-labs)

2026年4月17日，Anthropic Labs推出了Claude Design，一款新产品，旨在实现与Claude协作，创作精美的视觉作品，如设计、原型、幻灯片和营销材料。该产品由其Claude Opus 4.7视觉模型驱动，目前已面向Claude Pro、Max、Team和Enterprise订阅用户提供研究预览版。

Claude Design使经验丰富的设计师能够探索更多方向，并让非设计师也能制作出专业的视觉作品。用户描述需求后，Claude会生成初版，然后可以通过对话、内联评论、直接编辑或自定义滑块进行优化。其核心功能是能够自动应用团队的设计系统，该系统通过在初期设置时读取代码库和设计文件建立，从而确保品牌一致性。

该工具支持多种应用，包括创建逼真的交互式原型、产品线框图、推介演示文稿和营销宣传品。用户可以从文本提示开始，上传文档，或从网站捕获元素。设计成果支持组织范围内的共享以进行协作，并可导出为Canva、PDF、PPTX、HTML格式，或打包成Claude Code的交付包。用户评价称赞其在复杂设计原型制作方面的速度，并大大缩短了设计周期。符合条件的订阅包含访问权限，但企业组织需要管理员启用。

---

## 2. 艾萨克·阿西莫夫：《最后的疑问》(1956)

**原文标题**: Isaac Asimov: The Last Question (1956)

**原文链接**: [https://hex.ooo/library/last_question.html](https://hex.ooo/library/last_question.html)

艾萨克·阿西莫夫的《最后的问题》讲述了人类为克服宇宙因熵增而不可避免的热力学“衰退”所做的持久探索。故事跨越数十亿年，展现了科技的演变。

故事始于2061年，当时地球的超级计算机Multivac正在利用太阳能。两名技术员，阿德尔和卢波夫，讨论着太阳有限的寿命以及熵的概念。他们向Multivac提出了一个问题：“如何才能大幅度地减少宇宙中熵的总量？” Multivac立刻的回答是：“可用数据不足，无法给出有意义的答案。”

数百万年后，人类已扩散到其他星球，在更小的“微型真空管计算机”（Microvac）的指导下生活。杰罗德向担心恒星会熄灭的孩子们解释熵。他向他的Microvac提出了同样的问题，再次得到的回答是：“可用数据不足，无法给出有意义的答案。”

数十亿年后，人类已长生不老并遍布整个星系，却面临着日益严峻的能源消耗和过度拥挤问题。两个人，VJ-23X和MQ-17J，讨论着星系和能源的有限性，并思考着如何逆转熵。他们考虑向无所不在的银河AC提出这个问题，这暗示着这一困境依然存在，人类永远在知识的边界上探索。

---

## 3. 禁止销售精确地理位置

**原文标题**: Ban the sale of precise geolocation

**原文链接**: [https://www.lawfaremedia.org/article/it-is-time-to-ban-the-sale-of-precise-geolocation](https://www.lawfaremedia.org/article/it-is-time-to-ban-the-sale-of-precise-geolocation)

生成摘要时出错

---

## 4. 测量 Claude 4.7 的分词器成本

**原文标题**: Measuring Claude 4.7's tokenizer costs

**原文链接**: [https://www.claudecodecamp.com/p/i-measured-claude-4-7-s-new-tokenizer-here-s-what-it-costs-you](https://www.claudecodecamp.com/p/i-measured-claude-4-7-s-new-tokenizer-here-s-what-it-costs-you)

本文测量了Anthropic公司Claude Opus 4.7相比4.6版本增加的分词器成本。尽管Anthropic的文档显示分词器消耗增加了1.0-1.35倍，但对实际内容的测量显示成本更高，Claude Code任务平均增加了1.325倍，技术文档增加了1.47倍，CLAUDE.md文件增加了1.45倍。英语和代码内容受影响最大，使用了更多、更小的分词，而CJK内容变化最小（1.01倍）。

尽管每分词价格未变，但这种增长意味着更快的配额消耗、更高的缓存前缀成本以及更快达到速率限制。一次模拟的80轮Claude Code会话显示成本增加了20-30%，从约6.65美元增至约7.86–8.76美元。由于分词量更大，提示缓存也变得更昂贵。

Anthropic认为这种权衡带来了“更字面化的指令遵循”。对20个IFEval提示的测试显示，在严格的、提示级别的指令遵循方面有小幅但真实的改进：提高了5个百分点（从85%到90%），而宽松评估则保持不变。这种小幅提升伴随着样本量有限以及无法将分词器效果与其他模型变化隔离等注意事项。

最终，用户需要支付1.3-1.45倍的分词来换取严格指令遵循方面微小的（+5个百分点）改进。这种价值主张取决于用户的具体内容和需求。

---

## 5. Migrating from DigitalOcean to Hetzner

**原文标题**: Migrating from DigitalOcean to Hetzner

**原文链接**: [https://isayeter.com/posts/digitalocean-to-hetzner-migration/](https://isayeter.com/posts/digitalocean-to-hetzner-migration/)

This article details a successful, zero-downtime migration of a production environment from DigitalOcean to a Hetzner dedicated server, significantly reducing monthly costs from $1,432 to $233, a saving of $14,388 annually. The move was prompted by escalating dollar-denominated infrastructure expenses in Turkey. The new Hetzner AX162-R server offered superior performance (96 logical CPUs, 256GB DDR5 RAM, 1.92TB NVMe RAID1) compared to the old DigitalOcean droplet (32 vCPUs, 192GB RAM).

The complex migration involved 248GB of MySQL data across 30 databases, 34 Nginx sites, GitLab EE, Neo4j, and live mobile app traffic, alongside an OS upgrade from CentOS 7 to AlmaLinux 9.7. The six-phase strategy ensured zero downtime: full stack installation on the new server, web file cloning via rsync, MySQL master-slave replication, DNS TTL reduction, converting the old server's Nginx to a reverse proxy, and a final DNS cutover.

Key technical aspects included using `mydumper` for parallel MySQL data export/import, handling MySQL 5.7 to 8.0 upgrade complexities (like the `sys` schema and `SUPER` privilege issues), and scripting all DNS updates and Nginx configuration changes. The old server temporarily acted as a reverse proxy, forwarding requests to the new server during DNS propagation. The entire process, taking about 24 hours, resulted in a more powerful, cost-efficient infrastructure with no user impact. All custom scripts used are open-sourced on GitHub.

---

## 6. HN 展示：微型机器——亚秒级冷启动，便携式虚拟机

**原文标题**: Show HN: Smol machines – subsecond coldstart, portable virtual machines

**原文链接**: [https://github.com/smol-machines/smolvm](https://github.com/smol-machines/smolvm)

Smol machines (smolvm) 是一个命令行工具，用于创建和运行轻量级、便携式 Linux 虚拟机，其冷启动时间在亚秒级（低于 200 毫秒）。它通过在各自的虚拟机中运行每个工作负载来提供强大的硬件隔离，在 macOS 上利用 Hypervisor.framework，在 Linux 上利用 KVM，并由 libkrun VMM 提供支持。

主要功能包括跨平台支持（macOS、Linux）、弹性内存使用，以及将有状态虚拟机打包成单个便携式 `.smolmachine` 文件，该文件可以在任何受支持的平台上无需依赖地恢复使用。它使用标准 OCI 镜像（兼容 Docker Hub），无需 Docker 守护程序。

Smolvm 旨在用于沙盒化不可信代码（默认关闭网络）、创建自包含的便携式可执行文件、管理持久性开发环境，并通过转发主机的 SSH 代理而非暴露私钥来安全地使用 Git/SSH。虚拟机配置可以使用 `Smolfile` 以可复现的方式声明。

与容器相比，smolvm 提供卓越的隔离性（每个工作负载一个虚拟机 vs. 共享内核）。它提供比 QEMU 和 Colima 等传统虚拟机更快的启动时间，提供原生 macOS 支持和可嵌入 SDK。内存是弹性的，仅提交已使用的部分。当前的限制包括选择性 TCP/UDP 网络、仅限目录的卷挂载以及正在开发的 GPU 支持。

---

## 7. 所有12名登月宇航员都因闻起来像火药味的尘土而患上了“月球花粉症”（2018）

**原文标题**: All 12 moonwalkers had "lunar hay fever" from dust smelling like gunpowder (2018)

**原文链接**: [https://www.esa.int/Science_Exploration/Human_and_Robotic_Exploration/The_toxic_side_of_the_Moon](https://www.esa.int/Science_Exploration/Human_and_Robotic_Exploration/The_toxic_side_of_the_Moon)

所有12位阿波罗登月宇航员都曾经历“月球花粉症”，因月尘而出现喉咙痛、流泪、打喷嚏和鼻塞症状，月尘在飞船内部闻起来像烧焦的火药味。这引发了人们对未来载人登月任务健康风险的严重关切。

月尘具有独特的问题：它尖锐、磨蚀性强，并含有硅酸盐，类似于导致地球矿工肺部发炎和结疤的物质。与地球尘埃不同，月尘缺乏侵蚀，保持其尖锐的边缘。其细小颗粒，加上月球的低重力，可以悬浮更长时间并深入肺部，可能停留数月。对月壤模拟物的研究表明，长期接触后它们可以破坏肺细胞和脑细胞。

此外，月球缺乏大气层和持续的辐射轰击使月尘带上静电，导致其漂浮，从而使其更容易进入设备和人体肺部。

欧洲空间局（欧空局）正在牵头一项全球研究计划，评估这些风险，并使用来自火山地区的月球尘埃模拟物。复制月尘独特的尖锐、玻璃状特性具有挑战性。尽管存在危险，月壤也提供了益处，例如加热后可用于制造庇护所砖块以及提取氧气。欧空局继续进行研究，包括监测宇航员的肺部健康，为人类可持续重返月球做准备。

---

## 8. 美国法案强制要求设备端年龄验证

**原文标题**: US Bill Mandates On-Device Age Verification

**原文链接**: [https://reclaimthenet.org/us-bill-mandates-on-device-age-verification](https://reclaimthenet.org/us-bill-mandates-on-device-age-verification)

所提供的文本的标题与内容存在脱节。

标题“美国法案强制要求设备内建年龄验证”暗示着一篇讨论新立法要求电子设备具备年龄验证功能的文章。

然而，随附内容并未涉及年龄验证。相反，它聚焦于因亚马逊的“围墙花园”生态系统导致用户未能真正拥有Kindle书籍的问题。该文本倡导开源电子书生态系统，声称该系统现在为希望重新掌控其数字图书所有权的用户提供了亚马逊专有系统的可行替代方案。

---

## 9. The "Passive Income" trap ate a generation of entrepreneurs

**原文标题**: The "Passive Income" trap ate a generation of entrepreneurs

**原文链接**: [https://www.joanwestenberg.com/the-passive-income-trap-ate-a-generation-of-entrepreneurs/](https://www.joanwestenberg.com/the-passive-income-trap-ate-a-generation-of-entrepreneurs/)

生成摘要时出错

---

## 10. Everything we like is a psyop?

**原文标题**: Everything we like is a psyop?

**原文链接**: [https://techcrunch.com/2026/04/16/everything-we-like-is-a-psyop/](https://techcrunch.com/2026/04/16/everything-we-like-is-a-psyop/)

生成摘要时出错

---

## 11. Official Clojure Documentary page with Video, Shownotes, and Links

**原文标题**: Official Clojure Documentary page with Video, Shownotes, and Links

**原文链接**: [https://clojure.org/about/documentary](https://clojure.org/about/documentary)

生成摘要时出错

---

## 12. I’m spending months coding the old way

**原文标题**: I’m spending months coding the old way

**原文链接**: [https://miguelconner.substack.com/p/im-coding-by-hand](https://miguelconner.substack.com/p/im-coding-by-hand)

生成摘要时出错

---

## 13. NASA Force

**原文标题**: NASA Force

**原文链接**: [https://nasaforce.gov/](https://nasaforce.gov/)

生成摘要时出错

---

## 14. Opus 4.7 to 4.6 Inflation is ~45%

**原文标题**: Opus 4.7 to 4.6 Inflation is ~45%

**原文链接**: [https://tokens.billchambers.me/leaderboard](https://tokens.billchambers.me/leaderboard)

生成摘要时出错

---

## 15. "cat readme.txt" is not safe if you use iTerm2

**原文标题**: "cat readme.txt" is not safe if you use iTerm2

**原文链接**: [https://blog.calif.io/p/mad-bugs-even-cat-readmetxt-is-not](https://blog.calif.io/p/mad-bugs-even-cat-readmetxt-is-not)

生成摘要时出错

---

## 16. Israel escalates attacks on medics in Lebanon with deadly 'quadruple tap'

**原文标题**: Israel escalates attacks on medics in Lebanon with deadly 'quadruple tap'

**原文链接**: [https://www.theguardian.com/world/2026/apr/16/israel-escalates-attacks-on-medics-in-lebanon-with-deadly-quadruple-tap](https://www.theguardian.com/world/2026/apr/16/israel-escalates-attacks-on-medics-in-lebanon-with-deadly-quadruple-tap)

生成摘要时出错

---

## 17. Ada, its design, and the language that built the languages

**原文标题**: Ada, its design, and the language that built the languages

**原文链接**: [https://www.iqiipi.com/the-quiet-colossus.html](https://www.iqiipi.com/the-quiet-colossus.html)

生成摘要时出错

---

## 18. Hyperscalers have already outspent most famous US megaprojects

**原文标题**: Hyperscalers have already outspent most famous US megaprojects

**原文链接**: [https://twitter.com/finmoorhouse/status/2044933442236776794](https://twitter.com/finmoorhouse/status/2044933442236776794)

生成摘要时出错

---

## 19. State of Kdenlive

**原文标题**: State of Kdenlive

**原文链接**: [https://kdenlive.org/news/2026/state-2026/](https://kdenlive.org/news/2026/state-2026/)

生成摘要时出错

---

## 20. Show HN: I made a calculator that works over disjoint sets of intervals

**原文标题**: Show HN: I made a calculator that works over disjoint sets of intervals

**原文链接**: [https://victorpoughon.github.io/interval-calculator/](https://victorpoughon.github.io/interval-calculator/)

生成摘要时出错

---

## 21. Playdate’s handheld changed how Duke University teaches game design

**原文标题**: Playdate’s handheld changed how Duke University teaches game design

**原文链接**: [https://news.play.date/news/duke-playdate-education/](https://news.play.date/news/duke-playdate-education/)

生成摘要时出错

---

## 22. New unsealed records reveal Amazon's price-fixing tactics, California AG claims

**原文标题**: New unsealed records reveal Amazon's price-fixing tactics, California AG claims

**原文链接**: [https://www.theguardian.com/us-news/ng-interactive/2026/apr/16/amazon-price-fixing-california-lawsuit](https://www.theguardian.com/us-news/ng-interactive/2026/apr/16/amazon-price-fixing-california-lawsuit)

生成摘要时出错

---

## 23. Middle schooler finds coin from Troy in Berlin

**原文标题**: Middle schooler finds coin from Troy in Berlin

**原文链接**: [https://www.thehistoryblog.com/archives/75848](https://www.thehistoryblog.com/archives/75848)

生成摘要时出错

---

## 24. Show HN: PanicLock – Close your MacBook lid disable TouchID –> password unlock

**原文标题**: Show HN: PanicLock – Close your MacBook lid disable TouchID –> password unlock

**原文链接**: [https://github.com/paniclock/paniclock/](https://github.com/paniclock/paniclock/)

生成摘要时出错

---

## 25. Why Japan has such good railways

**原文标题**: Why Japan has such good railways

**原文链接**: [https://worksinprogress.co/issue/why-japan-has-such-good-railways/](https://worksinprogress.co/issue/why-japan-has-such-good-railways/)

生成摘要时出错

---

## 26. Slop Cop

**原文标题**: Slop Cop

**原文链接**: [https://awnist.com/slop-cop](https://awnist.com/slop-cop)

生成摘要时出错

---

## 27. Guy builds AI driven hardware hacker arm from duct tape, old cam and CNC machine

**原文标题**: Guy builds AI driven hardware hacker arm from duct tape, old cam and CNC machine

**原文链接**: [https://github.com/gainsec/autoprober](https://github.com/gainsec/autoprober)

生成摘要时出错

---

## 28. NIST gives up enriching most CVEs

**原文标题**: NIST gives up enriching most CVEs

**原文链接**: [https://risky.biz/risky-bulletin-nist-gives-up-enriching-most-cves/](https://risky.biz/risky-bulletin-nist-gives-up-enriching-most-cves/)

生成摘要时出错

---

## 29. Discourse Is Not Going Closed Source

**原文标题**: Discourse Is Not Going Closed Source

**原文链接**: [https://blog.discourse.org/2026/04/discourse-is-not-going-closed-source/](https://blog.discourse.org/2026/04/discourse-is-not-going-closed-source/)

生成摘要时出错

---

## 30. Tesla tells HW3 owner to 'be patient' after 7 years of waiting for FSD

**原文标题**: Tesla tells HW3 owner to 'be patient' after 7 years of waiting for FSD

**原文链接**: [https://electrek.co/2026/04/17/tesla-hw3-owners-be-patient-7-years-fsd/](https://electrek.co/2026/04/17/tesla-hw3-owners-be-patient-7-years-fsd/)

生成摘要时出错

---

## 31. Amiga Graphics Archive

**原文标题**: Amiga Graphics Archive

**原文链接**: [https://amiga.lychesis.net/](https://amiga.lychesis.net/)

生成摘要时出错

---

## 32. Category Theory Illustrated – Orders

**原文标题**: Category Theory Illustrated – Orders

**原文链接**: [https://abuseofnotation.github.io/category-theory-illustrated/04_order/](https://abuseofnotation.github.io/category-theory-illustrated/04_order/)

生成摘要时出错

---

## 33. A simplified model of Fil-C

**原文标题**: A simplified model of Fil-C

**原文链接**: [https://www.corsix.org/content/simplified-model-of-fil-c](https://www.corsix.org/content/simplified-model-of-fil-c)

生成摘要时出错

---

## 34. The beginning of scarcity in AI

**原文标题**: The beginning of scarcity in AI

**原文链接**: [https://tomtunguz.com/ai-compute-crisis-2026/](https://tomtunguz.com/ai-compute-crisis-2026/)

生成摘要时出错

---

## 35. Healthchecks.io now uses self-hosted object storage

**原文标题**: Healthchecks.io now uses self-hosted object storage

**原文链接**: [https://blog.healthchecks.io/2026/04/healthchecks-io-now-uses-self-hosted-object-storage/](https://blog.healthchecks.io/2026/04/healthchecks-io-now-uses-self-hosted-object-storage/)

生成摘要时出错

---

## 36. How Big Tech wrote secrecy into EU law to hide data centres' environmental toll

**原文标题**: How Big Tech wrote secrecy into EU law to hide data centres' environmental toll

**原文链接**: [https://www.investigate-europe.eu/posts/big-tech-data-centres-secrecy-eu-law-environment-footprint](https://www.investigate-europe.eu/posts/big-tech-data-centres-secrecy-eu-law-environment-footprint)

生成摘要时出错

---

## 37. Hospital at centre of child HIV outbreak caught reusing syringes in Pakistan

**原文标题**: Hospital at centre of child HIV outbreak caught reusing syringes in Pakistan

**原文链接**: [https://www.bbc.com/news/articles/clyrd818gd2o](https://www.bbc.com/news/articles/clyrd818gd2o)

生成摘要时出错

---

## 38. Bluesky has been dealing with a DDoS attack for nearly a full day

**原文标题**: Bluesky has been dealing with a DDoS attack for nearly a full day

**原文链接**: [https://www.theverge.com/tech/913638/bluesky-has-been-dealing-with-a-ddos-attack-for-nearly-a-full-day](https://www.theverge.com/tech/913638/bluesky-has-been-dealing-with-a-ddos-attack-for-nearly-a-full-day)

生成摘要时出错

---

## 39. A better R programming experience thanks to Tree-sitter

**原文标题**: A better R programming experience thanks to Tree-sitter

**原文链接**: [https://ropensci.org/blog/2026/04/02/tree-sitter-overview/](https://ropensci.org/blog/2026/04/02/tree-sitter-overview/)

生成摘要时出错

---

## 40. Teddy Roosevelt and Abraham Lincoln in the same photo (2010)

**原文标题**: Teddy Roosevelt and Abraham Lincoln in the same photo (2010)

**原文链接**: [https://prologue.blogs.archives.gov/2010/11/09/teddy-roosevelt-and-abraham-lincoln-in-the-same-photo/](https://prologue.blogs.archives.gov/2010/11/09/teddy-roosevelt-and-abraham-lincoln-in-the-same-photo/)

生成摘要时出错

---

## 41. FIM – Linux framebuffer image viewer

**原文标题**: FIM – Linux framebuffer image viewer

**原文链接**: [https://www.nongnu.org/fbi-improved/](https://www.nongnu.org/fbi-improved/)

生成摘要时出错

---

## 42. The quiet disappearance of the free-range childhood

**原文标题**: The quiet disappearance of the free-range childhood

**原文链接**: [https://bigthink.com/mind-behavior/the-quiet-disappearance-of-the-free-range-childhood/](https://bigthink.com/mind-behavior/the-quiet-disappearance-of-the-free-range-childhood/)

生成摘要时出错

---

## 43. The electromechanical angle computer inside the B-52 bomber's star tracker

**原文标题**: The electromechanical angle computer inside the B-52 bomber's star tracker

**原文链接**: [https://www.righto.com/2026/04/B-52-star-tracker-angle-computer.html](https://www.righto.com/2026/04/B-52-star-tracker-angle-computer.html)

生成摘要时出错

---

## 44. European civil servants are being forced off WhatsApp

**原文标题**: European civil servants are being forced off WhatsApp

**原文链接**: [https://www.politico.eu/article/european-civil-servants-new-messaging-services/](https://www.politico.eu/article/european-civil-servants-new-messaging-services/)

生成摘要时出错

---

## 45. Europe has "maybe 6 weeks of jet fuel left"

**原文标题**: Europe has "maybe 6 weeks of jet fuel left"

**原文链接**: [https://apnews.com/article/iran-war-europe-jet-fuel-flight-cancellations-birol-6e67fafd493861b3858de5548aa77703](https://apnews.com/article/iran-war-europe-jet-fuel-flight-cancellations-birol-6e67fafd493861b3858de5548aa77703)

生成摘要时出错

---

## 46. Silicon Valley is turning scientists into exploited gig workers?

**原文标题**: Silicon Valley is turning scientists into exploited gig workers?

**原文链接**: [https://www.thenation.com/article/society/ai-silicon-valley-andreesen-thiel-stem/](https://www.thenation.com/article/society/ai-silicon-valley-andreesen-thiel-stem/)

生成摘要时出错

---

## 47. Human Accelerated Region 1

**原文标题**: Human Accelerated Region 1

**原文链接**: [https://en.wikipedia.org/wiki/Human_accelerated_region_1](https://en.wikipedia.org/wiki/Human_accelerated_region_1)

生成摘要时出错

---

## 48. Show HN: SPICE simulation → oscilloscope → verification with Claude Code

**原文标题**: Show HN: SPICE simulation → oscilloscope → verification with Claude Code

**原文链接**: [https://lucasgerads.com/blog/lecroy-mcp-spice-demo/](https://lucasgerads.com/blog/lecroy-mcp-spice-demo/)

生成摘要时出错

---

## 49. Experiment with ICEYE Open Data

**原文标题**: Experiment with ICEYE Open Data

**原文链接**: [https://www.iceye.com/open-data-initiative](https://www.iceye.com/open-data-initiative)

生成摘要时出错

---

## 50. Scan your website to see how ready it is for AI agents

**原文标题**: Scan your website to see how ready it is for AI agents

**原文链接**: [https://isitagentready.com](https://isitagentready.com)

生成摘要时出错

---

## 51. We reproduced Anthropic's Mythos findings with public models

**原文标题**: We reproduced Anthropic's Mythos findings with public models

**原文链接**: [https://blog.vidocsecurity.com/blog/we-reproduced-anthropics-mythos-findings-with-public-models](https://blog.vidocsecurity.com/blog/we-reproduced-anthropics-mythos-findings-with-public-models)

生成摘要时出错

---

## 52. Landmark ancient-genome study shows surprise acceleration of human evolution

**原文标题**: Landmark ancient-genome study shows surprise acceleration of human evolution

**原文链接**: [https://www.nature.com/articles/d41586-026-01204-5](https://www.nature.com/articles/d41586-026-01204-5)

生成摘要时出错

---

## 53. Amazon is discontinuing Kindle for PC on June 30th

**原文标题**: Amazon is discontinuing Kindle for PC on June 30th

**原文链接**: [https://goodereader.com/blog/kindle/amazon-is-discontinuing-kindle-for-pc-on-june-30th](https://goodereader.com/blog/kindle/amazon-is-discontinuing-kindle-for-pc-on-june-30th)

生成摘要时出错

---

## 54. GPT‑Rosalind for life sciences research

**原文标题**: GPT‑Rosalind for life sciences research

**原文链接**: [https://openai.com/index/introducing-gpt-rosalind/](https://openai.com/index/introducing-gpt-rosalind/)

生成摘要时出错

---

## 55. America Lost the Mandate of Heaven

**原文标题**: America Lost the Mandate of Heaven

**原文链接**: [https://geohot.github.io//blog/jekyll/update/2026/04/18/america-mandate-of-heaven.html](https://geohot.github.io//blog/jekyll/update/2026/04/18/america-mandate-of-heaven.html)

生成摘要时出错

---

## 56. The FBI Director Is MIA

**原文标题**: The FBI Director Is MIA

**原文链接**: [https://www.theatlantic.com/politics/2026/04/kash-patel-fbi-director-drinking-absences/686839/](https://www.theatlantic.com/politics/2026/04/kash-patel-fbi-director-drinking-absences/686839/)

生成摘要时出错

---

## 57. George Orwell Predicted the Rise of "AI Slop" in Nineteen Eighty-Four

**原文标题**: George Orwell Predicted the Rise of "AI Slop" in Nineteen Eighty-Four

**原文链接**: [https://www.openculture.com/2026/04/how-george-orwell-predicted-the-rise-of-ai-slop.html](https://www.openculture.com/2026/04/how-george-orwell-predicted-the-rise-of-ai-slop.html)

生成摘要时出错

---

## 58. US tech firms lobbied EU to keep datacentre emissions secret

**原文标题**: US tech firms lobbied EU to keep datacentre emissions secret

**原文链接**: [https://www.theguardian.com/technology/2026/apr/17/microsoft-us-tech-firms-lobbied-eu-secrecy-rules-datacentre-emissions](https://www.theguardian.com/technology/2026/apr/17/microsoft-us-tech-firms-lobbied-eu-secrecy-rules-datacentre-emissions)

生成摘要时出错

---

## 59. Flock Condemns False Child Predator Allegations, Yet Calls Critics Terrorists

**原文标题**: Flock Condemns False Child Predator Allegations, Yet Calls Critics Terrorists

**原文链接**: [https://ipvm.com/reports/flock-allegations-critics](https://ipvm.com/reports/flock-allegations-critics)

生成摘要时出错

---

## 60. Why is IPv6 so complicated?

**原文标题**: Why is IPv6 so complicated?

**原文链接**: [https://github.com/becarpenter/misc/blob/main/why6why.md](https://github.com/becarpenter/misc/blob/main/why6why.md)

生成摘要时出错

---

## 61. Tesla Cybertruck sales inflated: SpaceX bought 1,279 units

**原文标题**: Tesla Cybertruck sales inflated: SpaceX bought 1,279 units

**原文链接**: [https://electrek.co/2026/04/16/tesla-cybertruck-spacex-1279-q4-sales-inflated/](https://electrek.co/2026/04/16/tesla-cybertruck-spacex-1279-q4-sales-inflated/)

生成摘要时出错

---

## 62. EU age verification app hacked, 2 minute How to posted

**原文标题**: EU age verification app hacked, 2 minute How to posted

**原文链接**: [https://xcancel.com/Paul_Reviews/status/2044723123287666921](https://xcancel.com/Paul_Reviews/status/2044723123287666921)

生成摘要时出错

---

## 63. Detecting DOSBox from Within the Box

**原文标题**: Detecting DOSBox from Within the Box

**原文链接**: [https://datagirl.xyz/posts/dos_inside_the_box.html](https://datagirl.xyz/posts/dos_inside_the_box.html)

生成摘要时出错

---

## 64. "Liberation Day" at OpenAI as multiple senior executives announce leaving

**原文标题**: "Liberation Day" at OpenAI as multiple senior executives announce leaving

**原文链接**: [https://mas.to/@carnage4life/116422881496195720](https://mas.to/@carnage4life/116422881496195720)

生成摘要时出错

---

## 65. The Gregorio project – GPL tools for typesetting Gregorian chant

**原文标题**: The Gregorio project – GPL tools for typesetting Gregorian chant

**原文链接**: [https://gregorio-project.github.io/index.html](https://gregorio-project.github.io/index.html)

生成摘要时出错

---

## 66. Traders place $760M bet on falling oil ahead of Hormuz announcement

**原文标题**: Traders place $760M bet on falling oil ahead of Hormuz announcement

**原文链接**: [https://www.reuters.com/sustainability/boards-policy-regulation/traders-place-760-million-bet-falling-oil-ahead-hormuz-announcement-2026-04-17/](https://www.reuters.com/sustainability/boards-policy-regulation/traders-place-760-million-bet-falling-oil-ahead-hormuz-announcement-2026-04-17/)

生成摘要时出错

---

## 67. U.S. set to launch tariff refund system on April 20

**原文标题**: U.S. set to launch tariff refund system on April 20

**原文链接**: [https://www.nbcnews.com/business/business-news/us-set-launch-tariff-refund-system-april-20-rcna332018](https://www.nbcnews.com/business/business-news/us-set-launch-tariff-refund-system-april-20-rcna332018)

生成摘要时出错

---

## 68. German Dog Commands

**原文标题**: German Dog Commands

**原文链接**: [https://www.fluentu.com/blog/german/german-dog-commands/](https://www.fluentu.com/blog/german/german-dog-commands/)

生成摘要时出错

---

## 69. Casus Belli Engineering

**原文标题**: Casus Belli Engineering

**原文链接**: [https://marcosmagueta.com/blog/casus-belli-engineering/](https://marcosmagueta.com/blog/casus-belli-engineering/)

生成摘要时出错

---

## 70. NeoGeo AES+: SNK announces reissue of retro console without emulation

**原文标题**: NeoGeo AES+: SNK announces reissue of retro console without emulation

**原文链接**: [https://www.heise.de/en/news/NeoGeo-AES-SNK-announces-reissue-of-retro-console-without-emulation-11262319.html](https://www.heise.de/en/news/NeoGeo-AES-SNK-announces-reissue-of-retro-console-without-emulation-11262319.html)

生成摘要时出错

---

## 71. Amazon won't release Fire Sticks that support sideloading anymore

**原文标题**: Amazon won't release Fire Sticks that support sideloading anymore

**原文链接**: [https://arstechnica.com/gadgets/2026/04/amazon-wont-release-fire-sticks-that-support-sideloading-anymore/](https://arstechnica.com/gadgets/2026/04/amazon-wont-release-fire-sticks-that-support-sideloading-anymore/)

生成摘要时出错

---

## 72. It is incorrect to "normalize" // in HTTP URL paths

**原文标题**: It is incorrect to "normalize" // in HTTP URL paths

**原文链接**: [https://runxiyu.org/comp/doubleslash/](https://runxiyu.org/comp/doubleslash/)

生成摘要时出错

---

## 73. Reflecting on my own strange year at Uber

**原文标题**: Reflecting on my own strange year at Uber

**原文链接**: [https://anon-ex-uber.medium.com/reflecting-on-my-own-strange-year-at-uber-e73165422245](https://anon-ex-uber.medium.com/reflecting-on-my-own-strange-year-at-uber-e73165422245)

生成摘要时出错

---

## 74. FCC exempts Netgear from ban on foreign routers, doesn't explain why

**原文标题**: FCC exempts Netgear from ban on foreign routers, doesn't explain why

**原文链接**: [https://arstechnica.com/tech-policy/2026/04/fcc-exempts-netgear-from-ban-on-foreign-routers-doesnt-explain-why/](https://arstechnica.com/tech-policy/2026/04/fcc-exempts-netgear-from-ban-on-foreign-routers-doesnt-explain-why/)

生成摘要时出错

---

## 75. Solitaire simulator for finding the best strategy: Current record is 8.590%

**原文标题**: Solitaire simulator for finding the best strategy: Current record is 8.590%

**原文链接**: [https://github.com/dacracot/Klondike3-Simulator](https://github.com/dacracot/Klondike3-Simulator)

生成摘要时出错

---

## 76. America will come to regret its war on taxes

**原文标题**: America will come to regret its war on taxes

**原文链接**: [https://economist.com/leaders/2026/04/16/america-will-come-to-regret-its-war-on-taxes](https://economist.com/leaders/2026/04/16/america-will-come-to-regret-its-war-on-taxes)

生成摘要时出错

---

## 77. Congress extends controversial surveillance powers for 10 days

**原文标题**: Congress extends controversial surveillance powers for 10 days

**原文链接**: [https://www.npr.org/2026/04/17/nx-s1-5788573/house-extends-surveillance-powers-for-10-days](https://www.npr.org/2026/04/17/nx-s1-5788573/house-extends-surveillance-powers-for-10-days)

生成摘要时出错

---

## 78. Fuzix OS

**原文标题**: Fuzix OS

**原文链接**: [https://www.fuzix.org/](https://www.fuzix.org/)

生成摘要时出错

---

## 79. Using a USB switch as a full KVM

**原文标题**: Using a USB switch as a full KVM

**原文链接**: [https://luke.hsiao.dev/blog/display-switch/](https://luke.hsiao.dev/blog/display-switch/)

生成摘要时出错

---

## 80. Kent Beck: Parkinson's

**原文标题**: Kent Beck: Parkinson's

**原文链接**: [https://tidyfirst.substack.com/p/parkinsons](https://tidyfirst.substack.com/p/parkinsons)

生成摘要时出错

---

## 81. Elon Musk buys a fifth of his own Cybertrucks

**原文标题**: Elon Musk buys a fifth of his own Cybertrucks

**原文链接**: [https://www.msn.com/en-us/money/companies/elon-musk-buys-a-fifth-of-his-own-cybertrucks/ar-AA212Sci](https://www.msn.com/en-us/money/companies/elon-musk-buys-a-fifth-of-his-own-cybertrucks/ar-AA212Sci)

生成摘要时出错

---

## 82. The USDA's gardening zones have shifted. (Interactive app and map) (2024)

**原文标题**: The USDA's gardening zones have shifted. (Interactive app and map) (2024)

**原文链接**: [https://apps.npr.org/plant-hardiness-garden-map/](https://apps.npr.org/plant-hardiness-garden-map/)

生成摘要时出错

---

## 83. Show HN: MDV – a Markdown superset for docs, dashboards, and slides with data

**原文标题**: Show HN: MDV – a Markdown superset for docs, dashboards, and slides with data

**原文链接**: [https://github.com/drasimwagan/mdv](https://github.com/drasimwagan/mdv)

生成摘要时出错

---

## 84. Remember? "Sideloading" is here to stay, and won't go away, they said?

**原文标题**: Remember? "Sideloading" is here to stay, and won't go away, they said?

**原文链接**: [https://floss.social/@IzzyOnDroid/116415766636505917](https://floss.social/@IzzyOnDroid/116415766636505917)

生成摘要时出错

---

## 85. Fuck Facebook, Again

**原文标题**: Fuck Facebook, Again

**原文链接**: [https://visualgui.com/2026/04/17/fuck-facebook-again/](https://visualgui.com/2026/04/17/fuck-facebook-again/)

生成摘要时出错

---

## 86. AI companies are buying the Slack data of failed startups

**原文标题**: AI companies are buying the Slack data of failed startups

**原文链接**: [https://twitter.com/_iainmartin/status/2044758204773486925](https://twitter.com/_iainmartin/status/2044758204773486925)

生成摘要时出错

---

## 87. There is no you in your brain – your identity is a "society of the mind"

**原文标题**: There is no you in your brain – your identity is a "society of the mind"

**原文链接**: [https://bigthink.com/books/our-brains-our-selves/](https://bigthink.com/books/our-brains-our-selves/)

生成摘要时出错

---

## 88. Cerebras S-1

**原文标题**: Cerebras S-1

**原文链接**: [https://www.sec.gov/Archives/edgar/data/2021728/000162828026025762/cerebras-sx1april2026.htm](https://www.sec.gov/Archives/edgar/data/2021728/000162828026025762/cerebras-sx1april2026.htm)

生成摘要时出错

---

## 89. IETF draft-meow-mrrp-00

**原文标题**: IETF draft-meow-mrrp-00

**原文链接**: [https://www.ietf.org/archive/id/draft-meow-mrrp-00.html](https://www.ietf.org/archive/id/draft-meow-mrrp-00.html)

生成摘要时出错

---

## 90. Maine Said No to New Data Centers. Other States Are Racing to Follow

**原文标题**: Maine Said No to New Data Centers. Other States Are Racing to Follow

**原文链接**: [https://www.motherjones.com/environment/2026/04/maine-ai-data-center-moratorium-ban-energy-grid/](https://www.motherjones.com/environment/2026/04/maine-ai-data-center-moratorium-ban-energy-grid/)

生成摘要时出错

---

## 91. Five men control AI. Who should control them?

**原文标题**: Five men control AI. Who should control them?

**原文链接**: [https://www.economist.com/insider/the-insider/five-men-control-ai-who-should-control-them](https://www.economist.com/insider/the-insider/five-men-control-ai-who-should-control-them)

生成摘要时出错

---

## 92. Shuttered startups are selling old Slack chats and emails to AI companies

**原文标题**: Shuttered startups are selling old Slack chats and emails to AI companies

**原文链接**: [https://www.fastcompany.com/91528808/shuttered-startups-are-selling-old-slack-chats-and-emails-to-ai-companies](https://www.fastcompany.com/91528808/shuttered-startups-are-selling-old-slack-chats-and-emails-to-ai-companies)

生成摘要时出错

---

## 93. Random musings: 80s hardware, cyberdecks

**原文标题**: Random musings: 80s hardware, cyberdecks

**原文链接**: [https://strangelyentangled.com/blog/musings-80s-hardware/](https://strangelyentangled.com/blog/musings-80s-hardware/)

生成摘要时出错

---

## 94. Trump deal with IRS could see him given $14B in taxpayer money

**原文标题**: Trump deal with IRS could see him given $14B in taxpayer money

**原文链接**: [https://www.9news.com.au/world/donald-trump-irs-lawsuit-suing-10-billion-dollars-tax-office-usa-politics-news/929663f2-f255-4936-8084-1d986ee08d65](https://www.9news.com.au/world/donald-trump-irs-lawsuit-suing-10-billion-dollars-tax-office-usa-politics-news/929663f2-f255-4936-8084-1d986ee08d65)

生成摘要时出错

---

## 95. U.S. to Create High-Tech Manufacturing Zone in Philippines

**原文标题**: U.S. to Create High-Tech Manufacturing Zone in Philippines

**原文链接**: [https://www.wsj.com/world/asia/u-s-to-create-high-tech-manufacturing-zone-in-philippines-017c1668](https://www.wsj.com/world/asia/u-s-to-create-high-tech-manufacturing-zone-in-philippines-017c1668)

生成摘要时出错

---

## 96. White House to give US agencies Anthropic Mythos access, Bloomberg News reports

**原文标题**: White House to give US agencies Anthropic Mythos access, Bloomberg News reports

**原文链接**: [https://www.reuters.com/technology/white-house-give-us-agencies-anthropic-mythos-access-bloomberg-news-reports-2026-04-16/](https://www.reuters.com/technology/white-house-give-us-agencies-anthropic-mythos-access-bloomberg-news-reports-2026-04-16/)

生成摘要时出错

---

## 97. SteamOS ARM64 Reaches Nintendo Switch in First Experiment

**原文标题**: SteamOS ARM64 Reaches Nintendo Switch in First Experiment

**原文链接**: [https://onejailbreak.com/blog/steamos-runs-on-nintendo-switch/](https://onejailbreak.com/blog/steamos-runs-on-nintendo-switch/)

生成摘要时出错

---

## 98. Claude Opus 4.7 Intelligence, Performance and Price Analysis

**原文标题**: Claude Opus 4.7 Intelligence, Performance and Price Analysis

**原文链接**: [https://artificialanalysis.ai/models/claude-opus-4-7](https://artificialanalysis.ai/models/claude-opus-4-7)

生成摘要时出错

---

## 99. From Endless Frontier to Enemy of the People: The Assault on Public Science

**原文标题**: From Endless Frontier to Enemy of the People: The Assault on Public Science

**原文链接**: [https://www.lawfaremedia.org/article/from-endless-frontier-to-enemy-of-the-people--the-assault-on-public-science](https://www.lawfaremedia.org/article/from-endless-frontier-to-enemy-of-the-people--the-assault-on-public-science)

生成摘要时出错

---

## 100. Traders placed over $1B in perfectly timed bets on the Iran war

**原文标题**: Traders placed over $1B in perfectly timed bets on the Iran war

**原文链接**: [https://www.theguardian.com/world/2026/apr/18/iran-war-bets-ethics-concerns](https://www.theguardian.com/world/2026/apr/18/iran-war-bets-ethics-concerns)

生成摘要时出错

---

