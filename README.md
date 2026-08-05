# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-08-05.md)

*最后自动更新时间: 2026-08-05 20:45:57*
## 1. 将团队编码标准带入 Claude Code 和 Codex 的代理技能

**原文标题**: Agent skills that bring team coding standards to Claude Code and Codex

**原文链接**: [https://github.com/tikalk/adlc-team-skills](https://github.com/tikalk/adlc-team-skills)

`adlc-team-skills` 套件解决了 AI 编码代理在没有特定团队背景的情况下启动会话，从而导致不合规代码和机构知识流失的问题。它提供了一个结构化框架，用于将团队编码标准和决策制定注入、维护和演进到代理工作流中。

核心功能包括：

1.  **上下文注入：** `team-boot` 在会话开始时自动注入团队规则、角色和决策的索引（来自版本化的 `team-ai-directives` Git 仓库），仅在相关时加载完整规则以避免上下文冗余。
2.  **结构化规划：** `mission-brief` 强制采用契约优先的方法，在实施前定义目标、约束和成功标准，确保代理对齐并修复规范，而不仅仅是代码。
3.  **自动化评估：** `evals` 技能创建可执行评估套件（PromptFoo/DeepEval），使用二进制评分器和 LLM 评判员，在人工审查 PR 之前验证代码是否符合标准。
4.  **知识捕获：** `levelup-specify` 从成功的会话中提取“上下文指令记录”（CDR），并将其提交回团队仓库，以使未来的代理交互更智能。
5.  **决策可追溯性：** `product-*` 和 `architect-*` 技能捕获产品需求（PDR）和架构决策（ADR），将其编译成 PRD.md 和 AD.md，提供从决策到代码的清晰可追溯性。
6.  **上下文剪枝：** `team-repair --build-to-delete` 主动识别并提议删除过时规则，确保代理的上下文保持相关性和效率。

这些技能与各种编码代理（如 Claude Code, Codex 等）集成，并与“十二因素代理式 SDLC”对齐，强调版本控制的指令、结构化工作流和在人工监督下的持续改进。

---

## 2. 为什么自行车迟迟才问世？ (2019)

**原文标题**: Why did we wait so long for the bicycle? (2019)

**原文链接**: [https://blog.rootsofprogress.org/why-did-we-wait-so-long-for-the-bicycle](https://blog.rootsofprogress.org/why-did-we-wait-so-long-for-the-bicycle)

本文探讨了为何看似简单的自行车直到19世纪后期才被发明出来。最初的假设考虑了技术进步（金属加工、轮胎、链条）、设计迭代、道路质量、马匹竞争以及经济因素。尽管材料和制造工艺的改进对自行车最终的商业成功和实用性至关重要（例如廉价钢铁、充气轮胎、精密齿轮），但它们未能完全解释*基本*实验为何经历了长达数世纪的延迟。

主要原因在于一个根本性的概念误导。几个世纪以来，发明家们（从15世纪到18世纪）将人力车辆设想为多人乘坐的四轮*马车*，结果这些设计都过于笨重且不切实际。关键的转变发生在19世纪初，卡尔·冯·德莱斯率先推出了单人、两轮的“跑步机”（德莱辛车），骑行者通过双脚蹬地来驱动。这种“机械马”是一项突破，尽管它缺乏踏板，并面临安全和公众接受度方面的问题。

现代自行车随后通过数十年的迭代演变而来：
1.  **19世纪60年代：** 增加了踏板（“骨头颠簸者”），但直接连接到前轮，几乎没有机械优势。
2.  **19世纪70年代：** 出现了大前轮的“便士法丁车”或“高轮车”设计，提高了速度但危险性高。
3.  **1885年：** 约翰·史塔利（John Starley）的“安全自行车”引入了关键的链条传动装置，使得车轮大小相等，大大提高了稳定性。
4.  **1888年：** 约翰·邓洛普（John Dunlop）的充气轮胎提供了舒适性和安全性，最终确定了现代设计。

总之，自行车的漫长等待源于长期的概念障碍（模仿马车而非两轮形式），以及随后的漫长设计迭代过程，最终因关键技术进步使其变得实用并被广泛采用。

---

## 3. 艺电的出售已敲定。

**原文标题**: The sale of Electronic Arts has been finalized

**原文链接**: [https://www.bbc.com/news/articles/cjejyl34345o](https://www.bbc.com/news/articles/cjejyl34345o)

艺电（EA）已以550亿美元的价格出售给一个沙特领导的团体，其中包括沙特阿拉伯公共投资基金（PIF）和由贾里德·库什纳领导的Affinity Partners。在PIF为此次交易借贷200亿美元后，EA将实现私有化，这使其成为历史上最大的杠杆收购。

此次出售引发了对EA未来走向的广泛猜测，分析师预测可能出现大规模裁员、增加游戏内购以及更“亲力亲为”的管理方式。人们担心EA可能会优先考虑“稳妥”的续作和大型特许经营系列，而非其传统上多元化的产品组合。

鉴于沙特阿拉伯严格的法律和人权记录，粉丝们尤其担心此举对《模拟人生》等游戏的影响，该游戏以倡导包容性和LGBT+关系而闻名。诸如Players Alliance HQ等倡导团体担心，创意决策可能会受到影响，导致言论自由、性别和LGBTQI+代表性等主题遭到审查。

由穆罕默德·本·萨勒曼亲王控制的沙特阿拉伯PIF，将EA视为一个“有吸引力”的金融机会（因其长久的生命力和强劲表现），同时也是一项“软实力资产”。此次收购是继其他大型体育投资之后进行的，旨在扩大沙特在全球体育和游戏社区的影响力，尽管这招致了“体育洗白”的指责。联合国此前曾认定沙特阿拉伯对记者贾马尔·卡舒吉的死亡负有责任。

---

## 4. Celld: 自托管分布式持久化对象

**原文标题**: Celld: Self-hosted, distributed Durable Objects

**原文链接**: [https://github.com/denoland/celld](https://github.com/denoland/celld)

Celld 是一个开源守护进程，支持您在自己的基础设施上自托管分布式 Cloudflare Workers 和 Durable Objects。每个 Durable Object 都充当一个独立的 SQLite 数据库，通过名称寻址并持续复制到 S3 兼容存储桶。节点仅通过此存储桶，利用对象存储的比较并交换（compare-and-swap）机制来确定所有权，从而无需控制平面、故障检测器或共识服务。

这种架构本身就对应用程序进行分片，隔离故障并防止共享数据库中常见的争用。Celld 嵌入 V8 以执行 Wrangler 包，S3 存储桶作为持久的真相来源，使节点能够完全替换。空闲对象可以休眠以最大程度地减少资源使用。

安装很简单，通过 `curl | sh` 脚本或提供的 Docker 容器即可完成。部署涉及使用 `celld deploy` 将 worker 代码和资产推送到 S3 存储桶，然后运行配置为使用相同存储桶的 `celld` 守护进程。它利用标准的 AWS 凭证链。

集群操作使用 `celld diagnose` 进行监控，该工具会探测活跃的对等节点并报告它们的状态和资源指标。对等节点间的 HTTP 通信通过 HMAC 认证进行保护，并且必须在受信任的私有网络上进行，不直接公开暴露。贡献通过 `git format-patch` 在 Apache-2.0 许可证和贡献者许可协议下接受。

---

## 5. 毫无扰乱的掌声，却仍导致了逮捕

**原文标题**: The applause that disrupted nothing – yet still led to an arrest

**原文链接**: [https://expression.fire.org/p/the-applause-that-disrupted-nothing](https://expression.fire.org/p/the-applause-that-disrupted-nothing)

在7月22日堪萨斯州恩波利亚市议会会议上，高中物理老师拉克丝·克拉里奇因短暂鼓掌五次以支持一位批评拟议数据中心的发言者而被捕。此前，公民们一直在公众评论之间鼓掌，促使市议员警告禁止所有观众反应，包括无声挥手。克拉里奇鼓掌后，一名被指示带走“下一个”鼓掌者的警官立即命令她离开。她因拒绝而遭到强制带离、逮捕，并被指控行为不检和妨碍执法。

文章认为，克拉里奇的鼓掌并非扰乱行为，仅在发言者之间持续了几秒钟，没有打断或拖延会议。文章指出，唯一真正的扰乱是克拉里奇被捕和随后的休会。恩波利亚的规定并未禁止鼓掌，仅授权在发出警告后，若出现扰乱行为方可将其带离。

作者认为，模糊的礼仪政策允许官员将不受欢迎的表达，特别是批评，定性为“扰乱行为”。文章指出，此类政策常常被选择性地执行，以惩罚异议。尽管第一修正案允许政府维持秩序，但它并不要求“修道院般的寂静”，也不能证明惩罚短暂鼓掌这种表达公众情绪的非扰乱性反应是正当的。此次事件引发了人们对官员是在真正维护秩序还是仅仅压制批评的担忧。

---

## 6. Learning-Rust.Github.io：人人可学的 Rust 编程语言教程

**原文标题**: Learning-Rust.Github.io: Rust Programming Language Tutorials for Everyone

**原文链接**: [https://learning-rust.github.io](https://learning-rust.github.io)

Learning-Rust.Github.io 为 Rust 编程语言提供了易于理解且以人为本的教程，旨在让 Rust “明晰易懂”，并使每个人都能轻松掌握。

该网站通过实际代码示例，在以下三个关键领域阐释了 Rust 的核心概念：
1.  **数据与行为**：演示如何定义自定义数据类型（`structs` 结构体）、实现方法（`impls` 实现块）以及通过 `traits`（特质）建立共享功能，并以 `Person` 结构体和 `Greet` 特质为例。
2.  **函数式编程**：通过迭代器（iterators）、过滤器（filters）和映射（maps）展示 Rust 强大的数据转换能力，处理一个分数数组以解析、转换和求和这些值。
3.  **进阶模式**：探讨泛型枚举（generic enums）、模式匹配（pattern matching）以及使用 `HashMap` 进行高效数据聚合等复杂模式，阐明如何处理和组织多样化的数据结构。

该平台强调实际应用，鼓励社区贡献，并重点介绍了涵盖 Web 开发、搜索和文档等相关领域的 Rust 生态系统工具。其主要目标是为 Rust 提供清晰、可操作的学习资源。

---

## 7. 缪斯代码和缪斯星火 1.2

**原文标题**: Muse Code and Muse Spark 1.2

**原文链接**: [https://research.meta.ai/blog/introducing-muse-code-and-muse-spark-1-2](https://research.meta.ai/blog/introducing-muse-code-and-muse-spark-1-2)

Meta 推出了 Muse Code (测试版)，这是一款终端编码代理，由他们最新的模型 Muse Spark 1.2 提供支持。Muse Code 旨在处理大型代码库中复杂的软件工程任务，包括代码规划、编写和验证。它利用持久的异步子代理来加速问题解决、提高准确性，并通过避免重复信息收集来减少用户干预。其运行时设计包括一个本地事件日志，用于实现精确重放和重启安全操作，使其能够在中断后恢复长时间运行的任务。其捆绑的关键技能包括 `/plan`、`/grill` 和 `/goal`，其中一个演示展示了它解释视频并生成度假屋营销页面的能力。

Muse Spark 1.2 是 Muse Spark 1.1 的一个专注于编码的更新版本，在代码生成、复杂调试、代码库理解和端到端开发者工作流方面都有显著改进。这些进步源于扩展的训练计算资源和多样化的环境，同时保持了其在通用代理能力方面的优势。它与 Muse Code 协同训练，以实现最佳性能协同效应。Muse Spark 1.2 擅长长周期编码任务，例如整个代码库生成和自动研究，它通过规划、目标条件设定和上下文压缩来实现这些。一个自我改进循环，即 Muse Spark 1.1 生成并评估训练数据，进一步增强了其指令遵循能力。一个案例研究强调了它在数千次工具调用中迭代优化 GPU 内核（KDA、MLA）的成功，从而实现了显著的性能提升。

Muse Spark 1.2 目前在全球范围内通过 Muse Code 和 Meta 模型 API 提供。

---

## 8. The Golden Age of British Ice Cream

**原文标题**: The Golden Age of British Ice Cream

**原文链接**: [https://www.vittlesmagazine.com/p/the-golden-age-of-british-ice-cream](https://www.vittlesmagazine.com/p/the-golden-age-of-british-ice-cream)

The "Golden Age of British Ice Cream," a transformative period from 1976 to 1991, saw the invention of most ice creams found in British freezers today. This era of unprecedented industrial innovation marked a strategic shift from targeting children to attracting adult consumers.

The catalyst was the Cornetto, successfully launched in 1976 by Wall's (Unilever). After an initial failure in the UK in the mid-sixties, extensive chemical tweaking perfected an Italian formula: a pre-packaged, bias-cut wafer cone sprayed with a chocolate-coconut oil barrier, filled with a stable, vegetable-fat ice cream emulsion designed to withstand freezer storage. Its launch coincided with a record-hot summer and a proto-viral marketing campaign, leading to 70 million annual sales within a decade.

This success sparked a wave of creations: Mini Milks (1976), Funny Feet (1980), Twister (1982), Viennetta (1982), Calippo (1982), Feast (1983), Mars ice cream bars (1988), Carte d’Or (1990), and the global titan, Magnum (1990).

Historically, British ice cream evolved from street-sold "penny licks" to basic wartime offerings. Post-rationing in 1954, with increased spending power and the shift from ice cream vans to home freezers and supermarket cabinets, companies sought new opportunities. Early technological advances yielded novelty lollies for children, but by the mid-seventies, the core question became: "How do you sell ice cream to grown-ups?"

Kevin Hillman, a Unilever product developer, embodied this new approach with the Viennetta (1982). Inspired by millefeuille, he used advanced industrial extrusion and spray technologies (borrowed from Cornettos) to create its iconic layered structure of vegetable-fat ice cream and chocolate. This period, driven by corporate competition and technological leaps, profoundly reshaped British food culture in just fifteen years.

---

## 9. AI Data Centers Are Driving Up Power Bills – This Map Shows Where

**原文标题**: AI Data Centers Are Driving Up Power Bills – This Map Shows Where

**原文链接**: [https://www.gadgetreview.com/ai-data-centers-are-driving-up-power-bills-this-map-shows-where](https://www.gadgetreview.com/ai-data-centers-are-driving-up-power-bills-this-map-shows-where)

生成摘要时出错

---

## 10. An SLM trained on $8 ESP32-S3

**原文标题**: An SLM trained on $8 ESP32-S3

**原文链接**: [https://github.com/Carloscodix/qapla](https://github.com/Carloscodix/qapla)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 2 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 3 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 4 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 5 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 6 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 7 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 8 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 9 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 10 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 11 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 12 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 13 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 14 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 15 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 16 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 17 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 18 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 19 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 20 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 21 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 22 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 23 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 24 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 25 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 26 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 27 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 28 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 29 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 30 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 31 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 32 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 33 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 34 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 35 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 36 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 37 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 38 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 39 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 40 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 41 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 42 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 43 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 44 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 45 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 46 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 47 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 48 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 49 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 50 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 51 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 52 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 53 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 54 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 55 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 56 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 57 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 58 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 59 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 60 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 61 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 62 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 63 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 64 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 65 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 66 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 67 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 68 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 69 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 70 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 71 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 72 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 73 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 74 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 75 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 76 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 77 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 78 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 79 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 80 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 81 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 82 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 83 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 84 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 85 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 86 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 87 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 88 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 89 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 90 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 91 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 92 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 93 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 94 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 95 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 96 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 97 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 98 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 99 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 100 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 101 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 102 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 103 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 104 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 105 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 106 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 107 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 108 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 109 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 110 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 111 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 112 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 113 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 114 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 115 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 116 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 117 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 118 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 119 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 120 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 121 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 122 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 123 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 124 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 125 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 126 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 127 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 128 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 129 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 130 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 131 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 132 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 133 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 134 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 135 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 136 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 137 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 138 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 139 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 140 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 141 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 142 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 143 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 144 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 145 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 146 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 147 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 148 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 149 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 150 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 151 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 152 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 153 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 154 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 155 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 156 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 157 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 158 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 159 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 160 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 161 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 162 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 163 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 164 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 165 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 166 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 167 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 168 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 169 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 170 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 171 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 172 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 173 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 174 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 175 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 176 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 177 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 178 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 179 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 180 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 181 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 182 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 183 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 184 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 185 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 186 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 187 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 188 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 189 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 190 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 191 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 192 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 193 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 194 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 195 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 196 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 197 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 198 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 199 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 200 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 201 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 202 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 203 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 204 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 205 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 206 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 207 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 208 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 209 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 210 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 211 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 212 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 213 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 214 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 215 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 216 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 217 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 218 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 219 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 220 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 221 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 222 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 223 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 224 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 225 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 226 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 227 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 228 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 229 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 230 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 231 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 232 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 233 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 234 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 235 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 236 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 237 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 238 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 239 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 240 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 241 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 242 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 243 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 244 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 245 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 246 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 247 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 248 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 249 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 250 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 251 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 252 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 253 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 254 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 255 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 256 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 257 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 258 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 259 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 260 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 261 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 262 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 263 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 264 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 265 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 266 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 267 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 268 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 269 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 270 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 271 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
