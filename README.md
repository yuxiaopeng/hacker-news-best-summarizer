# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-07-11.md)

*最后自动更新时间: 2026-07-11 20:27:26*
## 1. 请不要停用 Gemini 2.5 Flash

**原文标题**: Please don't discontinue Gemini 2.5 Flash

**原文链接**: [https://discuss.ai.google.dev/t/please-dont-discontinue-gemini-2-5-flash/174246](https://discuss.ai.google.dev/t/please-dont-discontinue-gemini-2-5-flash/174246)

作者感谢Gemini团队提供的模型，尤其强调了Gemini 2.5 Flash在其工作流程中扮演的关键角色。他们报告称，内部基准测试显示，即使在尝试根据新指南调整提示后，Gemini 3 Flash在他们的特定用例中表现也不佳。作者认为其他人可能也有类似的经历，并在切换时面临困难，因此强烈恳请不要停用Gemini 2.5 Flash。

---

## 2. 我们将PgBouncer的吞吐量提升了4倍

**原文标题**: We scaled PgBouncer to 4x throughput

**原文链接**: [https://clickhouse.com/blog/pgbouncer-clickhouse-managed-postgres](https://clickhouse.com/blog/pgbouncer-clickhouse-managed-postgres)

PgBouncer是单线程的，在多核机器上仅利用一个CPU核心，从而限制了吞吐量。ClickHouse Managed Postgres通过运行一个与可用核心数匹配的PgBouncer“进程集群”来克服这一限制。这些进程使用`so_reuseport`共享一个端口，使内核能够将传入的客户端连接在它们之间进行负载均衡，从而使这种多进程设置对客户端是透明的。

一个关键挑战是查询取消，因为取消请求可能发送到一个与管理查询会话的PgBouncer进程不同的实例。这通过“对等通信”来解决，即进程之间相互通信并将来取消请求转发到正确的实例。`max_client_conn`和`max_db_connections`等连接预算也分配到整个集群中，以防止Postgres过载。

在AWS EC2（16个vCPU实例）上的实际测试表明，单个PgBouncer进程峰值达到8.7万事务/秒，仅使用一个核心，而机器的其余部分处于空闲状态。相比之下，由16个PgBouncer进程组成的集群通过有效利用多达8个核心，实现了大约33.6万事务/秒，吞吐量提高了4倍。这显示了CPU利用率的显著提升（例如，在256个客户端下，单个进程为9%，而集群为52%）。

总而言之，通过运行一个利用`so_reuseport`和进程间对等通信的扩展集群，PgBouncer从一个吞吐量瓶颈转变为高效的管道，最大限度地提高了资源利用率。这种设置现在已成为ClickHouse Managed Postgres的标准配置。

---

## 3. Modern decor may be straining people's brains

**原文标题**: Modern decor may be straining people's brains

**原文链接**: [https://studyfinds.com/modern-decor-may-be-straining-peoples-brains/](https://studyfinds.com/modern-decor-may-be-straining-peoples-brains/)

生成摘要时出错

---

## 4. 美国女划船手完成加州至夏威夷历史性单人划行

**原文标题**: Female US rower completes historic solo journey from California to Hawaii

**原文链接**: [https://www.theguardian.com/us-news/2026/jul/04/california-hawaii-rowing-solo-journey](https://www.theguardian.com/us-news/2026/jul/04/california-hawaii-rowing-solo-journey)

美国赛艇运动员兼大峡谷漂流向导凯尔西·芬德勒(Kelsey Pfendler)成功完成了一次历史性的单人旅程，她从加利福尼亚州蒙特雷划船2400多英里，抵达夏威夷檀香山。经过近一个半月的海上航行，她于周五晚上抵达檀香山港口。

芬德勒的目标是成为首位完成太平洋中部单人横渡的美国女性、最年轻的女性和速度最快的女性。根据国际海洋划船协会的记录，她实现了这些目标，用时不到44天。这一非凡的成绩不仅打破了此前86天的女性可比速度纪录，甚至超越了52天的男性纪录。

数千人在线关注了芬德勒的旅程，她在网上分享了视频日记，详细记录了遇到的挑战和经历。她坦率地讲述了手上的水泡、在强风中难以入睡的挣扎，以及对抗不利洋流所造成的精神和身体上的消耗。她的视频还涵盖了烹饪、防晒和制造淡水等后勤细节，通常将情感上的反思与幽默融为一体。

作为一名拥有八年经验的专业漂流向导，芬德勒形容自己热爱“在荒无人烟的地方划船”。接近目的地时，她分享了一条强有力的信息，希望自己的成就能够激励他人“找到属于自己的宏大、艰难、可怕的事情”，并强调一个人“绝对足够强大去开始它”。

---

## 5. 你的代码很快——全看运气。

**原文标题**: Your code is fast – if you're lucky

**原文链接**: [https://tiki.li/blog/lucky_code.html](https://tiki.li/blog/lucky_code.html)

This article details an attempt to optimize a Quicksort implementation for speed, focusing on leveraging modern compilers' ability (like Clang) to generate fast, branch-free instructions. The author's custom C Quicksort uses several techniques: sorting networks for small partitions (up to 12 elements), median-of-5 pivot selection, and a specialized partitioning algorithm that temporarily stores elements in a `swbuf` array. Loop unrolling is also employed.

However, the initial optimized code performs surprisingly poorly on macOS/M1 (Clang, -O3), sorting 50 million doubles in 4.39 seconds, significantly slower than C++ `std::sort` which completes the same task in 1.33 seconds.

The core insight, highlighting the "luck" factor, is that minor "cosmetic" changes in code style can dramatically impact compiler optimization. The article points to rewriting explicit pointer increments, such as `*lwr = x; lwr++;` to the more idiomatic `*lwr++ = x;`, as the key modification. This suggests that compilers are highly sensitive to how code is written, and a subtle stylistic change can unlock superior, branch-free instruction generation, leading to substantial performance improvements. The article ends before presenting the benchmark results of the rewritten code.

---

## 6. 含铅汽油：问世即知其毒 (2016)

**原文标题**: Leaded Gas Was a Known Poison the Day It Was Invented (2016)

**原文链接**: [https://www.smithsonianmag.com/smart-news/leaded-gas-poison-invented-180961368/](https://www.smithsonianmag.com/smart-news/leaded-gas-poison-invented-180961368/)

文章《含铅汽油从发明之日起就已知是毒药》详细介绍了含铅汽油充满争议的历史。1921年，通用汽车工程师小托马斯·米基利（Thomas Midgley Jr.）发现四乙基铅（TEL）可以减少发动机“爆震”。尽管乙醇是一种更安全、有效的替代品，但通用汽车和石油公司却拒绝了它，因为它无法申请专利，并且威胁到他们对市场的控制。

TEL被认为剧毒；杜邦公司一位高管在1922年将其描述为“剧毒”，米基利本人也曾患有严重的铅中毒。含铅汽油于1923年首次销售，1924年五名工人因接触TEL死亡后，引发了强烈反弹。然而，1926年的一份公共卫生报告却将公众风险轻描淡写为“微乎其微”，得出“没有理由禁止销售”的结论，并将潜在的未来问题推迟为“下一代人的问题”。

这一先例使得逐步淘汰含铅汽油变得困难，美国环境保护署（EPA）直到20世纪70年代中期才开始这一进程。其长期影响是深远的：铅暴露，特别是儿童的铅暴露，与智商下降、多动症、行为问题、学习障碍有关，大量研究还将其与暴力犯罪联系起来。大部分铅仍残留在受污染的环境中，构成持续的健康挑战。

---

## 7. 苹果起诉OpenAI，指控其窃取公司机密

**原文标题**: Apple sues OpenAI, accusing it of stealing company secrets

**原文链接**: [https://www.nytimes.com/2026/07/10/technology/apple-openai-lawsuit.html](https://www.nytimes.com/2026/07/10/technology/apple-openai-lawsuit.html)

无法访问文章链接。

---

## 8. AI 2040 and the cult of intelligence

**原文标题**: AI 2040 and the cult of intelligence

**原文链接**: [https://geohot.github.io//blog/jekyll/update/2026/07/11/ai-2040.html](https://geohot.github.io//blog/jekyll/update/2026/07/11/ai-2040.html)

生成摘要时出错

---

## 9. FCC批准太空镜照亮夜空试验

**原文标题**: FCC approves test of space mirror to light night sky

**原文链接**: [https://theconversation.com/the-u-s-just-approved-a-giant-space-mirror-to-test-sunlight-on-demand-low-earth-orbit-is-getting-weird-283482](https://theconversation.com/the-u-s-just-approved-a-giant-space-mirror-to-test-sunlight-on-demand-low-earth-orbit-is-getting-weird-283482)

生成摘要时出错

---

## 10. Exit Chat Control

**原文标题**: Exit Chat Control

**原文链接**: [https://exitchatcontrol.org/](https://exitchatcontrol.org/)

This article introduces an encrypted messenger, presented as a simple, direct replacement for WhatsApp, offering secure texts, calls, video, and group chats. Its core value proposition is robust privacy and security: end-to-end encryption by default, a non-profit structure, an audited world-standard protocol, and minimal metadata retention. Notably, the team has pledged to exit the EU rather than comply with scanning mandates.

Recommended for everyone, starting immediately, it's seen as a vital first step for digital privacy. While a phone number is required for setup, users can create a username to hide it. To install, visit signal.org (App Store, Google Play, or direct APK). After confirming your number via SMS and setting a PIN, users should navigate to Settings > Privacy to create a username and enable registration lock, then invite contacts and link the desktop app as needed.

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 2 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 3 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 4 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 5 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 6 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 7 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 8 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 9 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 10 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 11 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 12 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 13 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 14 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 15 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 16 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 17 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 18 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 19 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 20 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 21 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 22 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 23 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 24 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 25 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 26 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 27 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 28 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 29 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 30 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 31 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 32 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 33 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 34 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 35 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 36 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 37 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 38 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 39 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 40 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 41 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 42 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 43 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 44 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 45 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 46 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 47 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 48 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 49 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 50 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 51 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 52 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 53 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 54 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 55 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 56 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 57 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 58 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 59 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 60 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 61 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 62 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 63 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 64 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 65 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 66 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 67 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 68 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 69 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 70 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 71 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 72 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 73 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 74 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 75 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 76 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 77 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 78 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 79 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 80 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 81 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 82 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 83 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 84 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 85 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 86 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 87 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 88 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 89 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 90 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 91 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 92 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 93 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 94 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 95 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 96 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 97 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 98 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 99 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 100 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 101 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 102 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 103 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 104 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 105 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 106 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 107 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 108 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 109 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 110 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 111 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 112 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 113 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 114 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 115 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 116 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 117 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 118 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 119 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 120 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 121 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 122 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 123 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 124 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 125 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 126 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 127 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 128 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 129 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 130 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 131 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 132 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 133 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 134 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 135 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 136 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 137 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 138 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 139 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 140 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 141 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 142 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 143 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 144 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 145 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 146 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 147 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 148 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 149 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 150 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 151 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 152 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 153 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 154 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 155 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 156 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 157 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 158 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 159 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 160 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 161 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 162 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 163 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 164 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 165 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 166 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 167 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 168 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 169 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 170 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 171 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 172 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 173 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 174 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 175 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 176 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 177 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 178 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 179 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 180 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 181 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 182 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 183 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 184 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 185 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 186 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 187 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 188 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 189 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 190 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 191 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 192 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 193 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 194 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 195 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 196 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 197 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 198 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 199 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 200 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 201 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 202 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 203 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 204 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 205 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 206 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 207 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 208 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 209 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 210 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 211 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 212 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 213 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 214 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 215 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 216 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 217 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 218 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 219 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 220 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 221 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 222 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 223 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 224 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 225 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 226 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 227 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 228 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 229 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 230 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 231 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 232 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 233 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 234 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 235 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 236 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 237 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 238 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 239 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 240 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 241 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 242 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 243 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 244 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 245 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 246 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
