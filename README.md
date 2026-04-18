# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-04-18.md)

*最后自动更新时间: 2026-04-18 20:10:49*
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

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 2 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 3 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 4 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 5 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 6 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 7 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 8 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 9 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 10 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 11 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 12 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 13 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 14 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 15 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 16 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 17 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 18 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 19 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 20 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 21 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 22 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 23 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 24 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 25 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 26 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 27 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 28 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 29 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 30 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 31 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 32 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 33 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 34 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 35 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 36 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 37 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 38 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 39 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 40 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 41 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 42 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 43 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 44 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 45 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 46 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 47 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 48 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 49 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 50 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 51 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 52 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 53 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 54 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 55 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 56 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 57 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 58 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 59 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 60 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 61 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 62 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 63 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 64 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 65 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 66 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 67 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 68 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 69 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 70 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 71 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 72 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 73 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 74 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 75 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 76 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 77 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 78 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 79 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 80 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 81 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 82 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 83 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 84 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 85 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 86 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 87 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 88 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 89 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 90 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 91 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 92 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 93 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 94 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 95 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 96 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 97 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 98 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 99 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 100 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 101 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 102 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 103 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 104 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 105 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 106 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 107 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 108 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 109 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 110 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 111 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 112 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 113 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 114 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 115 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 116 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 117 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 118 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 119 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 120 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 121 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 122 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 123 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 124 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 125 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 126 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 127 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 128 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 129 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 130 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 131 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 132 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 133 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 134 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 135 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 136 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 137 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 138 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 139 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 140 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 141 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 142 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 143 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 144 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 145 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 146 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 147 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 148 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 149 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 150 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 151 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 152 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 153 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 154 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 155 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 156 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 157 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 158 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 159 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 160 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 161 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 162 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
