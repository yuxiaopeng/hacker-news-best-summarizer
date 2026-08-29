# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-08-29.md)

*最后自动更新时间: 2026-08-29 02:29:41*
## 1. 英伟达同意以130亿美元收购Hugging Face

**原文标题**: Nvidia agrees to acquire Hugging Face for $13B

**原文链接**: [https://www.businessinsider.com/nvidia-in-talks-to-buy-hugging-face-13-billion-dollars-2026-8](https://www.businessinsider.com/nvidia-in-talks-to-buy-hugging-face-13-billion-dollars-2026-8)

英伟达据报道已同意以高达130亿美元的巨额资金收购Hugging Face。这项意义重大的交易表明，图形处理单元（GPU）巨头英伟达正在采取一项重大的战略举措，旨在将广受欢迎的开源人工智能平台Hugging Face整合到其生态系统之中。这项价值130亿美元的收购标志着在快速发展的人工智能领域中的一个关键时刻，它可能会将关键的人工智能开发工具和基础设施整合到英伟达日益扩大的影响力之下。

---

## 2. 总裁解雇了开发者，为人工智能腾出空间。开发者创建了开源人工智能CEO。

**原文标题**: CEO fired developers to make room for AI. Developers create open source AI CEO

**原文链接**: [https://github.com/SenteLabsAI/OpenExecutive](https://github.com/SenteLabsAI/OpenExecutive)

"Open Executive"是一个开源AI系统，旨在充当虚拟高管团队，提供为特定企业量身定制的哈佛MBA级别知识。该系统由sentelabs.ai开发，提供统一、一致的高管声音，由八个专业AI代理驱动，包括首席战略官、首席财务官、首席人力资源官、首席法务官、首席运营官、首席营销官、首席产品官以及一位董事会沟通总监。

该系统利用一个“高管编排器”（Executive Orchestrator）将用户消息路由至这些并行的专业代理。每个代理都从内置的MBA知识和上传的公司文档中检索相关上下文（通过ChromaDB实现RAG）。它在SQLite中维护过往决策的情景记忆，并包含一个用于主动跟进的调度器。

“Open Executive”基于Anthropic Claude API骨干（可选择使用本地或OpenRouter模型），后端采用Python/FastAPI，前端采用Next.js 15网页UI，并根据Apache 2.0协议授权。它提供广泛的接口，如网页UI、Slack、电子邮件、Telegram、Google Chat、Discord和CLI，以及文档上传功能。部署已针对Fly.io进行优化，支持开发和QA环境。用户可以通过一个引导向导快速设置公司资料，确保获得量身定制的建议。由于其调度器架构，它被设计为单实例部署。

---

## 3. 通过优化1.1.1.1的DNS缓存，节省了100TB内存

**原文标题**: Saving 100 terabytes of memory by optimizing 1.1.1.1's DNS cache

**原文链接**: [https://blog.cloudflare.com/dns-cache-memory-optimization-1111/](https://blog.cloudflare.com/dns-cache-memory-optimization-1111/)

Cloudflare 的 Big Pineapple 平台，为 1.1.1.1 及其他 DNS 服务提供支持，存储着超过 2500 亿个 DNS 缓存条目。鉴于巨大的内存开销，Cloudflare 对其 DNS 缓存条目存储进行了一系列五项优化，从而大幅节省了内存并提升了性能。

这些改动使每个条目的内存占用减少了 56%（从 953 字节降至 420 字节），每个条目的内存分配减少了 58%。在其整个服务器集群中，这总共释放了大约 100 TB 的内存。性能也获得了显著提升：缓存插入吞吐量增加了 43%，查询延迟降低了 19%。

实施的关键优化措施包括：
1.  **消除 `Vec` 和 `String` 的容量开销：** 通过用 `Box<[T]>` 和 `Box<str>` 替换 `Vec<T>` 和 `String`，移除了未使用的容量字段和多余的堆空间，每个条目至少节省了 64 字节。
2.  **整合记录列表：** 用带有 2 字节偏移量的单一列表替代了分别存储应答、授权和附加记录的独立列表，通过减少指针开销，每个条目节省了 28 字节。
3.  **优化记录所有者存储：** 对于所有者与查询域名相同的大多数记录，移除了所有者字段，并从缓存键中推断，从而避免了堆分配。
4.  **装箱大型 `RecordData` 枚举变体：** 为防止 Rust 的和类型枚举按其最大变体（NAPTR，144 字节）进行大小调整，将较大的变体进行了装箱。这显著减少了对 A 和 AAAA 记录等常见小型类型造成的填充浪费。
5.  **以“线缆格式”(`Box<[u8]>`) 存储记录数据：** 这是影响最大的一项改动。它消除了每个变体的枚举开销和独立的堆分配，将数据连续打包以获得更好的 CPU 缓存局部性，并在响应构建过程中允许直接复制大多数记录类型，从而进一步减少了序列化工作和延迟。

经过类似生产环境流量的基准测试和分阶段部署验证，这些改动使得各实例的常驻内存使用量减少了 42-43%。释放的内存将重新投入使用，以增加缓存容量，从而提高命中率并减少上游查询量。

---

## 4. 小模型来了

**原文标题**: Small Models Have Arrived

**原文链接**: [https://calv.info/small-models-have-arrived](https://calv.info/small-models-have-arrived)

本文强调了gpt-5.6-luna等功能强大且经济实惠的“小型模型”的出现，这些模型令人惊讶地强大、快速且智能，完成复杂任务仅需几十美分。这一发展解决了AI普及的一个主要瓶颈：token成本。

此前，高昂的推理成本使得消费者AI应用在经济上不可行，从而阻碍了公司。例如，一个每次交互成本为1美元的个性化新闻网站是难以维持的。现在，随着小型模型将每次交互的成本降至约0.10美元，这类消费级AI产品变得可行，为新公司打开了大门。

在商业领域，作者区分了“智商180”型工作（解决新颖问题）和“令牌生成型”工作（响应式、日常任务管理）。尽管前沿模型对于“智商180”型任务至关重要，但大约95%的业务运营，包括持续沟通和任务推进，都属于“令牌生成型”范畴。

文章预测，用于与同事、供应商和客户日常业务交互的“快速/廉价/足够好”模型的需求将迎来即将到来的激增。这些模型符合对响应迅速、高效处理日常任务的普遍需求。尽管存在提示注入安全等挑战，作者仍对其广泛采用持乐观态度，预示着一个成本效益高、AI驱动的生产力新时代。

---

## 5. 微鸭

**原文标题**: Microduck

**原文链接**: [https://pollen-robotics.com/microduck/](https://pollen-robotics.com/microduck/)

Microduck是一款25厘米、800克的开源双足机器人，专为用户进行强化学习训练而设计。它“开箱即玩”，内置7种预编程行为，例如行走、坐/站、踢腿和起身。

其主要特点是“虚实迁移”能力：用户可以在自己的机器上或通过Hugging Face Jobs平台，在物理模拟器（MuJoCo）中训练新的策略，并将其无缝部署到实体机器人上。整个软件栈，包括SDK和强化学习训练栈，均为开源（采用Apache-2.0许可证），并在GitHub上提供，以鼓励社区分享新的行为。

Microduck配备15个电机、一个摄像头、激光雷达和两个IMU，有四种配色可选。预订将于2026年8月27日开放，首发价格为399美元（不含税费和运费）。同时提供可选的附加包，例如充电器包、开发包（包含备用电机、电池和Hugging Face积分）以及配件包（包含滚轮、球和激光指示器）。一个Discord社区支持用户进行构建和分享。

---

## 6. 507 Mechanical Movements

**原文标题**: 507 Mechanical Movements

**原文链接**: [https://507movements.com/](https://507movements.com/)

生成摘要时出错

---

## 7. Get your Windows license refund

**原文标题**: Get your Windows license refund

**原文链接**: [https://en.refund4freedom.org/](https://en.refund4freedom.org/)

生成摘要时出错

---

## 8. Show HN: The load-bearing vocabulary of Claude

**原文标题**: Show HN: The load-bearing vocabulary of Claude

**原文链接**: [https://louisabraham.github.io/load-bearing/](https://louisabraham.github.io/load-bearing/)

生成摘要时出错

---

## 9. “It works better in the app”

**原文标题**: “It works better in the app”

**原文链接**: [https://shkspr.mobi/blog/2026/08/it-works-better-in-the-app/](https://shkspr.mobi/blog/2026/08/it-works-better-in-the-app/)

生成摘要时出错

---

## 10. GUIs should be fully keyboard-driven

**原文标题**: GUIs should be fully keyboard-driven

**原文链接**: [https://ckardaris.com/blog/2026/08/28/keyboard-driven-guis.html](https://ckardaris.com/blog/2026/08/28/keyboard-driven-guis.html)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-08-29](output/hacker_news_summary_2026-08-29.md) |
| 2 | [2026-08-21](output/hacker_news_summary_2026-08-21.md) |
| 3 | [2026-08-25](output/hacker_news_summary_2026-08-25.md) |
| 4 | [2026-08-26](output/hacker_news_summary_2026-08-26.md) |
| 5 | [2026-08-24](output/hacker_news_summary_2026-08-24.md) |
| 6 | [2026-08-28](output/hacker_news_summary_2026-08-28.md) |
| 7 | [2026-08-23](output/hacker_news_summary_2026-08-23.md) |
| 8 | [2026-08-22](output/hacker_news_summary_2026-08-22.md) |
| 9 | [2026-08-18](output/hacker_news_summary_2026-08-18.md) |
| 10 | [2026-08-15](output/hacker_news_summary_2026-08-15.md) |
| 11 | [2026-08-19](output/hacker_news_summary_2026-08-19.md) |
| 12 | [2026-08-12](output/hacker_news_summary_2026-08-12.md) |
| 13 | [2026-08-20](output/hacker_news_summary_2026-08-20.md) |
| 14 | [2026-08-13](output/hacker_news_summary_2026-08-13.md) |
| 15 | [2026-08-14](output/hacker_news_summary_2026-08-14.md) |
| 16 | [2026-08-17](output/hacker_news_summary_2026-08-17.md) |
| 17 | [2026-08-16](output/hacker_news_summary_2026-08-16.md) |
| 18 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 19 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 20 | [2026-08-09](output/hacker_news_summary_2026-08-09.md) |
| 21 | [2026-08-10](output/hacker_news_summary_2026-08-10.md) |
| 22 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 23 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 24 | [2026-08-11](output/hacker_news_summary_2026-08-11.md) |
| 25 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 26 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 27 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 28 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 29 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 30 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 31 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 32 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 33 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 34 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 35 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 36 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 37 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 38 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 39 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 40 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 41 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 42 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 43 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 44 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 45 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 46 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 47 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 48 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 49 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 50 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 51 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 52 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 53 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 54 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 55 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 56 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 57 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 58 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 59 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 60 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 61 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 62 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 63 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 64 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 65 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 66 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 67 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 68 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 69 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 70 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 71 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 72 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 73 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 74 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 75 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 76 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 77 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 78 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 79 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 80 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 81 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 82 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 83 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 84 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 85 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 86 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 87 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 88 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 89 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 90 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 91 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 92 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 93 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 94 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 95 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 96 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 97 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 98 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 99 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 100 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 101 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 102 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 103 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 104 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 105 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 106 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 107 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 108 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 109 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 110 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 111 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 112 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 113 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 114 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 115 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 116 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 117 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 118 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 119 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 120 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 121 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 122 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 123 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 124 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 125 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 126 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 127 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 128 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 129 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 130 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 131 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 132 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 133 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 134 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 135 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 136 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 137 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 138 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 139 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 140 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 141 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 142 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 143 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 144 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 145 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 146 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 147 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 148 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 149 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 150 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 151 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 152 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 153 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 154 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 155 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 156 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 157 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 158 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 159 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 160 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 161 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 162 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 163 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 164 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 165 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 166 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 167 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 168 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 169 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 170 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 171 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 172 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 173 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 174 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 175 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 176 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 177 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 178 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 179 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 180 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 181 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 182 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 183 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 184 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 185 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 186 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 187 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 188 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 189 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 190 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 191 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 192 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 193 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 194 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 195 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 196 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 197 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 198 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 199 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 200 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 201 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 202 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 203 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 204 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 205 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 206 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 207 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 208 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 209 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 210 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 211 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 212 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 213 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 214 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 215 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 216 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 217 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 218 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 219 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 220 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 221 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 222 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 223 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 224 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 225 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 226 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 227 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 228 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 229 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 230 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 231 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 232 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 233 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 234 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 235 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 236 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 237 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 238 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 239 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 240 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 241 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 242 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 243 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 244 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 245 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 246 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 247 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 248 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 249 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 250 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 251 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 252 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 253 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 254 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 255 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 256 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 257 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 258 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 259 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 260 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 261 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 262 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 263 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 264 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 265 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 266 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 267 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 268 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 269 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 270 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 271 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 272 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 273 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 274 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 275 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 276 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 277 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 278 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 279 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 280 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 281 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 282 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 283 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 284 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 285 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 286 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 287 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 288 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 289 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 290 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 291 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 292 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 293 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
