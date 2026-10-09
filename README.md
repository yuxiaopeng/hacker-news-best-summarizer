# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-10-09.md)

*最后自动更新时间: 2026-10-09 23:34:44*
## 1. 为什么业界没有为DeepSeek 4.1 Flash感到恐慌？

**原文标题**: Why isn't the industry freaking out about DeepSeek 4.1 Flash?

**原文链接**: [https://www.dgt.is/blog/2026-10-07-deepseek-freek-out/](https://www.dgt.is/blog/2026-10-07-deepseek-freek-out/)

作者对DeepSeek 4.1 Flash未被业界认可为颠覆者感到不解，尽管它以显著更低的成本提供了“前沿模型”的能力。经过一个月的密集使用，作者发现其在性能和速度上与Anthropic的Opus等模型不相上下，但价格却便宜了几个数量级，典型的会话成本不到1美元。

这种通过每月10美元订阅实现的经济实惠性，彻底改变了作者的开发流程，使其能够进行大量、低成本的实验和“无需动脑的任务”。一个关键创新是DeepSeek的“缓存魔法”，它大幅减少了KV缓存的大小，使其在GPU内存、电力和用水消耗方面效率更高，从而将其定位为可持续的替代方案。

作者批评了业界当前不惜一切代价追求最大智能的主流思维模式，并指出像DeepSeek这样的中国公司正在通过提供功能强大、类似于仿制药的“蒸馏”模型来颠覆这一现状——以一小部分价格提供相似的性能。这种转变普及了对高级智能的访问，并挑战了传统前沿实验室乃至注重成本的用户自行部署的经济可行性，尽管缓存优化预计很快将实现高效的本地部署。

---

## 2. Cloudflare 收购 Deno

**原文标题**: Cloudflare acquires Deno

**原文链接**: [https://deno.com/blog/cloudflare](https://deno.com/blog/cloudflare)

2026年10月9日，Ryan Dahl宣布Deno团队将加入Cloudflare，并将其工作整合到Cloudflare的生态系统中。此次收购源于Deno长期以来简化服务器软件和分布式应用的目标，这一目标通过Deno Deploy和`celld`项目不断发展，`celld`项目基于Cloudflare Workers编程模型，旨在构建可扩展的分布式应用。

Deno团队将与Cloudflare的Workers和Durable Objects团队合并工作，专注于一个共享平台，而非独立的运行时和托管开发。

这一举动将给Deno用户带来重大变化：
*   **Deno运行时：** 将再支持一年，提供每月错误修复和安全更新；此后，Deno团队将停止开发，尽管它仍将保持开源。
*   **Deno Deploy：** 将再运营六个月后关闭，并为付费客户提供迁移到Cloudflare Workers的支持。
*   **JSR：** 将继续运营，其基础设施将迁移到Cloudflare。
*   **rusty_v8：** 将继续得到支持并集成到`workerd`中。

团队特别期待探索与AI的协同作用，利用Durable Objects构建代理线束，这是`celld`项目在Cloudflare内部的一个重点。

---

## 3. 特朗普政府暂停微软参与一项绿卡项目。

**原文标题**: Trump administration is suspending Microsoft from a green card program

**原文链接**: [https://apnews.com/article/h1b-visa-program-vance-microsoft-e7b3a407f822702b269ee277d21343ea](https://apnews.com/article/h1b-visa-program-vance-microsoft-e7b3a407f822702b269ee277d21343ea)

特朗普政府暂停了微软参与一项绿卡项目的资格，此前发现该公司未能充分向美国工人发布招聘信息。此举立即生效，并将持续至少两年，这意味着微软不能使用PERM（电子审查管理计划）劳工认证程序在美国招聘外国工人担任永久职位。

劳工部的调查结果是在对两份具体的绿卡申请进行审计后得出的。尽管审计没有发现故意欺诈的证据，但它认定微软对这些职位的招聘方法不符合旨在确保美国工人优先考虑的联邦法规。这包括在报纸和在线广告职位时存在的问题，未能满足特定的时间和内容要求。

微软是H-1B签证项目的主要使用者，也是限制性移民政策的强烈批评者。该公司对此表示失望并计划提出上诉。微软表示，它相信自己完全遵守了所有法规，并且这项决定只影响其极少数的绿卡申请。

这一举动突显了特朗普政府优先考虑美国工人并审查移民项目的更广泛努力。尽管此次暂停是针对微软和PERM程序，但它向其他依赖类似途径雇佣外国人才的科技公司发出了警告。

---

## 4. Whistle：16.9 MB 轻量级语音转文字

**原文标题**: Whistle: Speech to Text in 16.9 MB

**原文链接**: [https://cactuscompute.com/blog/whistle](https://cactuscompute.com/blog/whistle)

Cactus Compute 发布了 Whistle，一款新的语音识别模型，专为在手机、可穿戴设备和微控制器等设备上部署而优化。Whistle 仅 16.9 MB，可在 CPU 上高效运行，无需任何依赖，采用与其 Needle 模型相同的 C++ 引擎和量化技术。

Whistle 提供三大核心功能：对 16 kHz 单声道音频（最长 30 秒）进行转录，支持英语、德语、法语、西班牙语、意大利语、荷兰语和波兰语（带自动语言检测功能）；精确的单词时间戳，包括开始时间、结束时间和概率；以及语音嵌入。

基准测试证明了其效率：Whistle 明显小于 Whisper base（16.9 MB 对比 145.3 MB）和 Moonshine tiny v2（41.9 MB）。它还拥有卓越的速度，在 Apple M4 Pro CPU 上实现了 11.1 毫秒的首个 token 生成时间（time-to-first-token）和 1,319 tokens/秒的解码速率，优于这两个竞争对手。尽管在 LibriSpeech 和 SPGISpeech 等数据集的词错误率（Word Error Rate）方面具有竞争力，但 Whisper base 在 TED-LIUM 等其他数据集上仍保持优势。

开发者可以通过 Python 的 `pip install cactus-needle` 或 C++ API 集成 Whistle，预构建的二进制文件支持包括 Android、iOS 和 WebAssembly 在内的 17 种目标平台。该模型还可以与 Needle 结合，用于语音激活的工具调用。模型权重可在 Hugging Face 上获取，引擎源代码可在 GitHub 上获取。

---

## 5. 是的，而且

**原文标题**: Yes, and

**原文链接**: [https://htmx.org/essays/yes-and/](https://htmx.org/essays/yes-and/)

卡森·格罗斯是一位计算机科学教授，他回答了在人工智能时代是否还应该学习计算机编程的问题，他的回答是“是的，而且……”。

他认为，编程的核心——用计算机解决问题和控制复杂性——仍将具有价值。然而，他警告说，如果仅仅将人工智能用于代码生成，它对初级程序员来说是危险的。初级程序员*必须*编写代码，以培养深刻的理解，有效地阅读，并避免创建他们无法控制的系统（例如“魔法师的学徒”陷阱）。他将人工智能与编译器区分开来，指出人工智能的非确定性以及增加意外复杂性的潜力。

格罗斯鼓励学生将人工智能用作“优秀的助教”——一个理解概念和克服障碍的伙伴，而不是主要的C代码生成器。

展望未来，他认为人工智能将从根本上改变编程。尽管纯粹的编码在相对重要性上可能会下降，但其他技能将变得更加关键：清晰的沟通、理解业务问题以及“架构”复杂系统（这仍然需要编码经验）。他建议高级程序员和初级程序员应采用不同的LLM使用方式：高级程序员可用于分析、处理小型任务和编写不理想的代码；而初级程序员则应将其用于理解概念，但*仍需编写代码*以培养直觉。

关于当前严峻的就业市场，格罗斯认为它是暂时的、周期性的。他建议求职者利用个人关系（家人、朋友、朋友的家人）而非仅仅依赖在线招聘平台，并强调即使是非科技公司也需要程序员。

总之，编程仍然是一个有价值的职业。成功将涉及掌握基础编码和复杂性控制，培养沟通和商业敏锐度等更广泛的技能，并明智地将人工智能用作学习工具，而不是编码本身的替代品。他强调，公司必须允许初级程序员编写代码，以促进他们的长期发展。

---

## 6. 抱歉，我正在开会。

**原文标题**: Sorry, I'm in a meeting

**原文链接**: [https://iminafleeting.com/](https://iminafleeting.com/)

网站iminafleeting.com上题为“抱歉，我在开会”的文章深入探讨了“在开会”这一普遍存在的现代借口。作者观察到，这句话虽然有时确实是真话，却经常被用作一种方便的社交润滑剂，以表明自己没空、避免不必要的互动、推脱任务，或者为专注工作、思考，甚至个人时间创造空间。在“永远在线”的工作文化中，它已成为一种广泛使用的划定界限的工具。

文章的核心思想强调重新掌控自己的时间和注意力。在承认这句话在管理需求方面的实用性的同时，作者含蓄地批评了它的过度使用，认为它可能成为一种拐杖而非深思熟虑的策略。文章鼓励读者更有意识地管理日程并沟通自己的可用性，优先考虑深度工作、个人幸福和真正有价值的参与，而非持续承受随时可用的压力。该网站的标题“iminafleeting.com”巧妙地玩味了许多会议的短暂性，以及时间转瞬即逝的更广泛概念。

---

## 7. “Math 2.0” will need to value mathematical progress more holistically

**原文标题**: “Math 2.0” will need to value mathematical progress more holistically

**原文链接**: [https://mathstodon.xyz/@tao/117395269325940185](https://mathstodon.xyz/@tao/117395269325940185)

生成摘要时出错

---

## 8. Our $445M Series D

**原文标题**: Our $445M Series D

**原文链接**: [https://oxide.computer/blog/our-445m-series-d](https://oxide.computer/blog/our-445m-series-d)

生成摘要时出错

---

## 9. Theranos.world

**原文标题**: Theranos.world

**原文链接**: [https://www.theranos.world/](https://www.theranos.world/)

生成摘要时出错

---

## 10. Triple-A Minesweeper

**原文标题**: Triple-A Minesweeper

**原文链接**: [https://minesweeper.mikelacher.com/](https://minesweeper.mikelacher.com/)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-10-09](output/hacker_news_summary_2026-10-09.md) |
| 2 | [2026-10-07](output/hacker_news_summary_2026-10-07.md) |
| 3 | [2026-10-06](output/hacker_news_summary_2026-10-06.md) |
| 4 | [2026-10-04](output/hacker_news_summary_2026-10-04.md) |
| 5 | [2026-10-02](output/hacker_news_summary_2026-10-02.md) |
| 6 | [2026-10-03](output/hacker_news_summary_2026-10-03.md) |
| 7 | [2026-09-24](output/hacker_news_summary_2026-09-24.md) |
| 8 | [2026-10-01](output/hacker_news_summary_2026-10-01.md) |
| 9 | [2026-09-29](output/hacker_news_summary_2026-09-29.md) |
| 10 | [2026-09-30](output/hacker_news_summary_2026-09-30.md) |
| 11 | [2026-09-27](output/hacker_news_summary_2026-09-27.md) |
| 12 | [2026-09-25](output/hacker_news_summary_2026-09-25.md) |
| 13 | [2026-09-21](output/hacker_news_summary_2026-09-21.md) |
| 14 | [2026-09-23](output/hacker_news_summary_2026-09-23.md) |
| 15 | [2026-09-20](output/hacker_news_summary_2026-09-20.md) |
| 16 | [2026-09-22](output/hacker_news_summary_2026-09-22.md) |
| 17 | [2026-09-19](output/hacker_news_summary_2026-09-19.md) |
| 18 | [2026-09-13](output/hacker_news_summary_2026-09-13.md) |
| 19 | [2026-09-16](output/hacker_news_summary_2026-09-16.md) |
| 20 | [2026-09-14](output/hacker_news_summary_2026-09-14.md) |
| 21 | [2026-09-17](output/hacker_news_summary_2026-09-17.md) |
| 22 | [2026-09-18](output/hacker_news_summary_2026-09-18.md) |
| 23 | [2026-09-15](output/hacker_news_summary_2026-09-15.md) |
| 24 | [2026-09-09](output/hacker_news_summary_2026-09-09.md) |
| 25 | [2026-09-10](output/hacker_news_summary_2026-09-10.md) |
| 26 | [2026-09-08](output/hacker_news_summary_2026-09-08.md) |
| 27 | [2026-09-07](output/hacker_news_summary_2026-09-07.md) |
| 28 | [2026-09-06](output/hacker_news_summary_2026-09-06.md) |
| 29 | [2026-09-11](output/hacker_news_summary_2026-09-11.md) |
| 30 | [2026-09-12](output/hacker_news_summary_2026-09-12.md) |
| 31 | [2026-09-03](output/hacker_news_summary_2026-09-03.md) |
| 32 | [2026-09-02](output/hacker_news_summary_2026-09-02.md) |
| 33 | [2026-08-31](output/hacker_news_summary_2026-08-31.md) |
| 34 | [2026-09-04](output/hacker_news_summary_2026-09-04.md) |
| 35 | [2026-09-05](output/hacker_news_summary_2026-09-05.md) |
| 36 | [2026-09-01](output/hacker_news_summary_2026-09-01.md) |
| 37 | [2026-08-29](output/hacker_news_summary_2026-08-29.md) |
| 38 | [2026-08-30](output/hacker_news_summary_2026-08-30.md) |
| 39 | [2026-08-22](output/hacker_news_summary_2026-08-22.md) |
| 40 | [2026-08-25](output/hacker_news_summary_2026-08-25.md) |
| 41 | [2026-08-28](output/hacker_news_summary_2026-08-28.md) |
| 42 | [2026-08-23](output/hacker_news_summary_2026-08-23.md) |
| 43 | [2026-08-21](output/hacker_news_summary_2026-08-21.md) |
| 44 | [2026-08-24](output/hacker_news_summary_2026-08-24.md) |
| 45 | [2026-08-26](output/hacker_news_summary_2026-08-26.md) |
| 46 | [2026-08-14](output/hacker_news_summary_2026-08-14.md) |
| 47 | [2026-08-19](output/hacker_news_summary_2026-08-19.md) |
| 48 | [2026-08-20](output/hacker_news_summary_2026-08-20.md) |
| 49 | [2026-08-16](output/hacker_news_summary_2026-08-16.md) |
| 50 | [2026-08-17](output/hacker_news_summary_2026-08-17.md) |
| 51 | [2026-08-18](output/hacker_news_summary_2026-08-18.md) |
| 52 | [2026-08-15](output/hacker_news_summary_2026-08-15.md) |
| 53 | [2026-08-13](output/hacker_news_summary_2026-08-13.md) |
| 54 | [2026-08-12](output/hacker_news_summary_2026-08-12.md) |
| 55 | [2026-08-11](output/hacker_news_summary_2026-08-11.md) |
| 56 | [2026-08-10](output/hacker_news_summary_2026-08-10.md) |
| 57 | [2026-08-09](output/hacker_news_summary_2026-08-09.md) |
| 58 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 59 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 60 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 61 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 62 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 63 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 64 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 65 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 66 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 67 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 68 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 69 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 70 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 71 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 72 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 73 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 74 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 75 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 76 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 77 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 78 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 79 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 80 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 81 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 82 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 83 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 84 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 85 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 86 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 87 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 88 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 89 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 90 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 91 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 92 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 93 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 94 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 95 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 96 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 97 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 98 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 99 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 100 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 101 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 102 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 103 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 104 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 105 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 106 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 107 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 108 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 109 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 110 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 111 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 112 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 113 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 114 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 115 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 116 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 117 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 118 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 119 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 120 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 121 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 122 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 123 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 124 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 125 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 126 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 127 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 128 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 129 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 130 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 131 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 132 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 133 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 134 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 135 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 136 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 137 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 138 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 139 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 140 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 141 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 142 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 143 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 144 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 145 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 146 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 147 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 148 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 149 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 150 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 151 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 152 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 153 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 154 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 155 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 156 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 157 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 158 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 159 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 160 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 161 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 162 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 163 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 164 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 165 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 166 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 167 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 168 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 169 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 170 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 171 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 172 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 173 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 174 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 175 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 176 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 177 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 178 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 179 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 180 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 181 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 182 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 183 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 184 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 185 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 186 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 187 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 188 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 189 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 190 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 191 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 192 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 193 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 194 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 195 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 196 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 197 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 198 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 199 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 200 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 201 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 202 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 203 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 204 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 205 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 206 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 207 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 208 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 209 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 210 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 211 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 212 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 213 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 214 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 215 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 216 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 217 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 218 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 219 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 220 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 221 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 222 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 223 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 224 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 225 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 226 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 227 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 228 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 229 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 230 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 231 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 232 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 233 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 234 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 235 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 236 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 237 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 238 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 239 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 240 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 241 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 242 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 243 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 244 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 245 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 246 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 247 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 248 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 249 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 250 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 251 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 252 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 253 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 254 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 255 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 256 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 257 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 258 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 259 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 260 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 261 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 262 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 263 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 264 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 265 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 266 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 267 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 268 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 269 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 270 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 271 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 272 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 273 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 274 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 275 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 276 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 277 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 278 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 279 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 280 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 281 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 282 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 283 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 284 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 285 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 286 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 287 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 288 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 289 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 290 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 291 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 292 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 293 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 294 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 295 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 296 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 297 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 298 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 299 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 300 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 301 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 302 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 303 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 304 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 305 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 306 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 307 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 308 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 309 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 310 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 311 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 312 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 313 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 314 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 315 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 316 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 317 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 318 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 319 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 320 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 321 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 322 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 323 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 324 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 325 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 326 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
| 327 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 328 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 329 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 330 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
