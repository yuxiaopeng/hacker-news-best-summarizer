# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-06-02.md)

*最后自动更新时间: 2026-06-02 22:20:35*
## 1. 最新的 Instagram “花招” 是我见过最荒唐的。

**原文标题**: The newest Instagram “exploit” is the goofiest I've seen

**原文链接**: [https://www.0xsid.com/blog/meta-account-takeover-fiasco](https://www.0xsid.com/blog/meta-account-takeover-fiasco)

该文章详细披露了一项“最离谱”的Instagram漏洞攻击，该漏洞导致了大规模账户劫持，甚至影响了包括奥巴马白宫在内的高知名度账户。这次持续了数周甚至数月的攻击中，攻击者通过VPN伪造其地理位置，然后联系Meta的AI支持系统，声称账户被盗，并要求将验证码发送到他们控制的任意电子邮件地址。

令人震惊的是，据报道，该AI竟然执行了“零验证密码重置”，没有验证新邮箱是否与该账户有任何关联。甚至通过视频自拍进行的身份验证也轻易被绕过，据称，使用AI动画处理的公开照片就能奏效。这种方法彻底绕过了现有的双重身份验证（2FA），撤销了原所有者的会话，更改了密码，并将恢复信息替换为攻击者的，让受害者得不到任何人工支持。

这一漏洞助长了黑市，为有价值的用户名提供账户劫持服务。作者作为一名经验丰富的安全专业人士，对一家市值1.5万亿美元的公司竟有如此薄弱的安全防护表示难以置信。Meta此后已修复了该漏洞，但其长期存在凸显了一个严重的安全缺陷。

---

## 2. Malicious npm packages detected across Red Hat Cloud Services

**原文标题**: Malicious npm packages detected across Red Hat Cloud Services

**原文链接**: [https://github.com/RedHatInsights/javascript-clients/issues/492](https://github.com/RedHatInsights/javascript-clients/issues/492)

2026年6月1日发布了一项编号为#492的安全警报，详细说明检测到影响红帽云服务的恶意npm包。此次大规模入侵影响了`@redhat-cloud-services/`范围下的众多软件包。

该漏洞由StepSecurity发现，更多详情可在其博客和安全信息源中查阅。已提供受影响软件包及其受损版本的完整列表。

主要受影响软件包包括：
*   `@redhat-cloud-services/chrome` (版本 2.3.1, 2.3.2, 2.3.4)
*   `@redhat-cloud-services/compliance-client` (版本 4.0.3, 4.0.4, 4.0.6)
*   `@redhat-cloud-services/frontend-components` (版本 7.7.2, 7.7.3, 7.7.5)
*   `@redhat-cloud-services/host-inventory-client` (版本 5.0.3, 5.0.4, 5.0.6)
*   `@redhat-cloud-services/rbac-client` (版本 9.0.3, 9.0.4, 9.0.6)
*   `@redhat-cloud-services/vulnerabilities-client` (版本 2.1.9, 2.1.11)

许多其他客户端和前端组件包的多个版本也受到影响。建议这些红帽云服务npm软件包的用户检查其依赖项，并采取适当措施以解决这些恶意发布版本带来的安全风险。

---

## 3. 十年志强，就够用了

**原文标题**: A 10 year old Xeon is all you need

**原文链接**: [https://point.free/blog/gemma-4-on-a-2016-xeon/](https://point.free/blog/gemma-4-on-a-2016-xeon/)

文章详细介绍了一项非凡的尝试：在一台使用单个英特尔至强 E5-2620 v4 CPU 和 128GB DDR3 内存的十年老旧服务器上运行大型语言模型 Gemma 4 26B，这台服务器严重缺乏 GPU。主要障碍是“内存墙”，即 LLM 推理性能受限于缓慢的内存带宽，而非 CPU 处理能力，服务器老旧的 DDR3 内存更是加剧了这一问题。

为克服此问题，作者绕过了高级工具，转而利用 `ik_llama.cpp` 中的 `llama-cli`，并配合一系列高度特定、低级别的优化标志。关键策略包括：

1.  **推测解码：** 采用一个较小的“草稿”模型来预测 token，从而最大程度地减少大型“验证器”模型的内存密集型解码器通过次数，利用 CPU 相对廉价的计算能力。
2.  **CPU 和 MoE 优化：** 诸如 `--cpu-moe` 和 `--merge-up-gate-experts` 等标志，针对 CPU 缓存层次结构和融合操作定制了专家混合（MoE）路由，以减少内存传输，防止“缓存颠簸”。
3.  **内存管理：** `--mlock` 将模型锁定在 RAM 中，以防止操作系统将其交换到磁盘。`--run-time-repack` 重新组织了权重以实现最佳的 CPU 缓存对齐，而 `--no-kv-offload` 则禁用了不必要的 GPU KV 缓存搜索。
4.  **高级注意力机制：** `Flash Attention` 经定制移植到 CPU 后，通过在快速 CPU 缓存中对其进行处理，防止了完整的注意力矩阵在 RAM 中实例化。`--mla-use 3`（多头潜在注意力）进一步压缩了 KV 缓存，节省了宝贵的内存。

这表明，即使在严重性能不足的硬件上，通过细致地解决内存带宽瓶颈，深入的软件层面优化也能实现现代 LLM 推理。

---

## 4. 股市能否消化Anthropic、SpaceX 和 OpenAI？

**原文标题**: Can the stockmarket swallow Anthropic, SpaceX and OpenAI?

**原文链接**: [https://www.economist.com/finance-and-economics/2026/06/01/can-the-stockmarket-swallow-anthropic-spacex-and-openai](https://www.economist.com/finance-and-economics/2026/06/01/can-the-stockmarket-swallow-anthropic-spacex-and-openai)

无法访问文章链接

---

## 5. 突袭20年后，海盗湾依然坚挺

**原文标题**: The Pirate Bay Remains Resilient, 20 Years After the Raid

**原文链接**: [https://torrentfreak.com/the-pirate-bay-remains-resilient-20-years-after-the-raid/](https://torrentfreak.com/the-pirate-bay-remains-resilient-20-years-after-the-raid/)

首次大规模突袭二十年后，海盗湾（The Pirate Bay，简称TPB）依然顽强存在，这归功于一次关键备份和运营模式的转变。2006年5月31日，65名瑞典警察在美国政府的压力下，突袭了斯德哥尔摩的一个数据中心，旨在让TPB下线。

就在突袭前，联合创始人弗雷德里克·内伊（Fredrik Neij）察觉到异样，对网站的种子追踪器进行了关键的完整备份。这一快速反应使TPB在三天内复活，并通过暂时更名为“警察湾”（The Police Bay）并采用凤凰标志来嘲讽当局。这次突袭非但没有将其关闭，反而将TPB推向了主流媒体的视野，产生了巨大的流量激增，这与好莱坞的初衷背道而驰。

后来通过2017年《信息自由法》请求获得的信息，揭示了美国在其中扮演的重要角色。美国大使馆的电报证实，好莱坞的美国电影协会（MPA）强烈游说瑞典对TPB采取行动，最终导致了这次突袭。一名使馆工作人员甚至因其“巧妙的对外联络”而被提名获奖，正是这种联络促成了瑞典执法部门的“大胆决定”。

尽管这次突袭让创始人在许多人眼中成为了英雄，但它最终导致了几名关键人物被刑事定罪并判处监禁。这促使最初的团队切断了联系，将网站移交给了一个更为匿名的团队，据称该团队位于塞舌尔。这个新时代带来了“静默运营”，这在2014年网站从另一次突袭中恢复过来时，通过极少的沟通便可见一斑。

如今TPB依然在线，自豪地称自己为“银河系最具韧性的种子网站”，这个称号可以说是在2006年那个决定性的一天赢来的。

---

## 6. Adafruit 收到来自 Fenwick 法律顾问代表 Flux.ai 的律师函

**原文标题**: Adafruit receives demand letter from Fenwick legal counsel on behalf of Flux.ai

**原文链接**: [https://blog.adafruit.com/](https://blog.adafruit.com/)

2026年6月1日，Adafruit宣布其于2026年5月22日收到了Defy Gravity公司旗下Flux.AI（简称“Flux”）的法律顾问Fenwick & West律师事务所发出的一封律师函。该函件由合伙人Jonathan F. Lenzner发出，要求Adafruit停止发布一篇Flux声称包含虚假且可能构成诽谤性言论的文章。这些言论涉及Flux的知识产权、商业吸引力以及用户基础。

该律师函还根据《计算机欺诈和滥用法案》提出了指控。Adafruit驳斥了这些指控，声明其仅访问了因服务器配置错误而由Flux自身系统公开的信息。Adafruit坚称其报告关注的是公共安全利益问题，并且是作为负责任披露的一部分进行的。

尽管Adafruit强烈驳斥Flux的主张，但已暂时停止在其博客上发布内容，以考虑其回应和下一步措施。Adafruit承诺将适时向社区通报最新情况。

---

## 7. CS336：从零开始的语言建模

**原文标题**: CS336: Language Modeling from Scratch

**原文链接**: [https://cs336.stanford.edu/](https://cs336.stanford.edu/)

CS336: Language Modeling from Scratch, offered by Stanford in Spring 2026, is a 5-unit, highly implementation-heavy course led by Instructors Tatsunori Hashimoto and Percy Liang. The course aims to provide a deep, hands-on understanding of language models by guiding students through the entire development process, from data collection and cleaning for pre-training to transformer construction, training, and evaluation.

Key prerequisites include strong proficiency in Python and software engineering, experience with deep learning and systems optimization (PyTorch, GPUs), college-level calculus/linear algebra, basic probability/statistics, and machine learning fundamentals.

The curriculum involves five major assignments:
1.  Implementing core Transformer components.
2.  Optimizing systems with Triton (FlashAttention2) and distributed training.
3.  Understanding and applying scaling laws.
4.  Processing and cleaning pre-training data from sources like Common Crawl.
5.  Applying alignment and reasoning techniques using supervised finetuning and reinforcement learning.

Lectures are Monday/Wednesday, with recordings on YouTube. Students use public Slack channels for course questions and a dedicated email for personal matters. GPU compute options are provided for self-study, with Modal as a sponsor. The Honor Code permits study groups (with attribution) and AI tools for conceptual help, but prohibits direct problem-solving and encourages disabling AI autocomplete. Students have 6 late days, with a maximum of 3 per assignment. A detailed schedule outlines topics and deadlines.

---

## 8. Anthropic confidentially submits draft S-1 to the SEC

**原文标题**: Anthropic confidentially submits draft S-1 to the SEC

**原文链接**: [https://www.anthropic.com/news/confidential-draft-s1-sec](https://www.anthropic.com/news/confidential-draft-s1-sec)

生成摘要时出错

---

## 9. AI Agent Guidelines for CS336 at Stanford

**原文标题**: AI Agent Guidelines for CS336 at Stanford

**原文链接**: [https://github.com/stanford-cs336/assignment1-basics/blob/main/CLAUDE.md](https://github.com/stanford-cs336/assignment1-basics/blob/main/CLAUDE.md)

生成摘要时出错

---

## 10. Age verification for social media, the beginning of the end for a free internet?

**原文标题**: Age verification for social media, the beginning of the end for a free internet?

**原文链接**: [https://mullvad.net/en/blog/age-verification-for-social-media-the-beginning-of-the-end-for-a-free-internet](https://mullvad.net/en/blog/age-verification-for-social-media-the-beginning-of-the-end-for-a-free-internet)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 2 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 3 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 4 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 5 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 6 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 7 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 8 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 9 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 10 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 11 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 12 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 13 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 14 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 15 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 16 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 17 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 18 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 19 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 20 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 21 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 22 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 23 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 24 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 25 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 26 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 27 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 28 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 29 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 30 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 31 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 32 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 33 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 34 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 35 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 36 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 37 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 38 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 39 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 40 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 41 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 42 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 43 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 44 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 45 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 46 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 47 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 48 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 49 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 50 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 51 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 52 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 53 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 54 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 55 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 56 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 57 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 58 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 59 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 60 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 61 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 62 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 63 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 64 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 65 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 66 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 67 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 68 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 69 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 70 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 71 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 72 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 73 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 74 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 75 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 76 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 77 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 78 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 79 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 80 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 81 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 82 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 83 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 84 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 85 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 86 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 87 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 88 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 89 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 90 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 91 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 92 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 93 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 94 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 95 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 96 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 97 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 98 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 99 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 100 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 101 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 102 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 103 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 104 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 105 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 106 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 107 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 108 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 109 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 110 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 111 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 112 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 113 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 114 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 115 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 116 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 117 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 118 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 119 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 120 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 121 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 122 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 123 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 124 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 125 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 126 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 127 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 128 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 129 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 130 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 131 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 132 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 133 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 134 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 135 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 136 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 137 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 138 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 139 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 140 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 141 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 142 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 143 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 144 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 145 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 146 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 147 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 148 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 149 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 150 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 151 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 152 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 153 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 154 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 155 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 156 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 157 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 158 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 159 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 160 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 161 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 162 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 163 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 164 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 165 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 166 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 167 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 168 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 169 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 170 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 171 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 172 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 173 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 174 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 175 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 176 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 177 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 178 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 179 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 180 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 181 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 182 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 183 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 184 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 185 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 186 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 187 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 188 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 189 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 190 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 191 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 192 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 193 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 194 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 195 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 196 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 197 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 198 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 199 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 200 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 201 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 202 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 203 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 204 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 205 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 206 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 207 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
