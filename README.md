# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-04-02.md)

*最后自动更新时间: 2026-04-02 20:13:09*
## 1. 报告大幅增加

**原文标题**: Significant Raise of Reports

**原文链接**: [https://lwn.net/Articles/1065620/](https://lwn.net/Articles/1065620/)

文章报道称，内核安全邮件列表上的安全漏洞报告出现了显著而快速的增长。两年前每周只有2-3份报告，去年增至每周约10份（常是“AI垃圾”），而自2026年初以来，这一数字已惊人地跃升至每天5-10份。与之前的“AI垃圾”不同，这些新报告大多是正确的，需要更多的维护者，并导致每天都发现重复的漏洞。

尽管报告速度的加快“令人担忧且疲惫不堪”，作者指出修复可能被犯罪分子利用的真实漏洞带来了满足感，并推测这种高强度工作可能正在清除长期积压的漏洞。

作者预测软件安全实践将发生根本性转变：
1. **禁运消失：** 由于漏洞很容易被重新发现，隐藏它们将变得毫无意义。
2. **关注更新：** 人们将明白安全漏洞仅仅是漏洞，因此定期软件更新（而非关注特定的CVE）将是保持安全的唯一明智方式。
3. **强制维护：** 那些历来忽视持续维护的项目将被迫适应，因为所有软件都将成为持续攻击的目标。

最终，作者预见软件质量将回归更高的水平，类似于2000年前的严格标准，但承认这将经历一个持续数年的“巨大混乱”时期。

---

## 2. OpenAI 墓地：所有未能实现的交易和产品

**原文标题**: The OpenAI graveyard: All the deals and products that haven't happened

**原文链接**: [https://www.forbes.com/sites/phoebeliu/2026/03/31/openai-graveyard-deals-and-products-havent-happened-openai/](https://www.forbes.com/sites/phoebeliu/2026/03/31/openai-graveyard-deals-and-products-havent-happened-openai/)

无法访问文章链接。

---

## 3. Neanderthals survived on a knife's edge for 350k years

**原文标题**: Neanderthals survived on a knife's edge for 350k years

**原文链接**: [https://www.science.org/content/article/neanderthals-survived-knife-s-edge-350-000-years](https://www.science.org/content/article/neanderthals-survived-knife-s-edge-350-000-years)

生成摘要时出错

---

## 4. 我们拦截了白宫应用的流量。

**原文标题**: We intercepted the White House app's network traffic

**原文链接**: [https://www.atomic.computer/blog/white-house-app-network-traffic-analysis/](https://www.atomic.computer/blog/white-house-app-network-traffic-analysis/)

通过MITM代理对白宫iOS应用（v47.0.4）进行的动态分析显示，该应用存在大量第三方网络活动，与其隐私声明相悖。在206个由应用发起的请求中，只有48个（23%）指向whitehouse.gov，其余77%联系了31个独特的第三方服务，如Elfsight、OneSignal、YouTube、Google DoubleClick、Facebook和Twitter。

应用启动时，第三方分析公司OneSignal会收到用户的“实时画像”。这包括语言、时区、国家、完整IP地址、首次和末次活动的确切时间戳、设备型号和操作系统、网络类型、运营商、越狱状态、会话次数、会话持续时间以及一个持久的唯一标识符。该画像会在不同会话间更新。

该应用还联系了13个Elfsight域名，证实了一个两阶段JavaScript加载器，允许Elfsight服务器注入各种社交媒体小部件脚本（例如TikTok、Instagram）并设置超过10个跟踪cookie。此外，YouTube嵌入内容会触发谷歌的DoubleClick广告投放和跟踪基础设施。

尽管有这些发现，该应用的隐私声明却虚假地声称“未收集数据”和“NSPrivacyTracking: false”。分析总结道，官方白宫应用存在大量未披露的第三方数据收集和跟踪行为。

---

## 5. 用于 ocamlc 的新 C++ 后端

**原文标题**: A new C++ back end for ocamlc

**原文链接**: [https://github.com/ocaml/ocaml/pull/14701](https://github.com/ocaml/ocaml/pull/14701)

一则愚人节公告推出 `ocamlc` 的新 C++ 后端，使得 OCaml 程序能够使用 `ocamlc -incr-c primes.ml` 命令编译成 C++ 模板元编程代码。该后端旨在改进现有的 C 运行时和 FFI（外部函数接口），将 OCaml 的列表和函数等构造翻译成冗长的 C++ 模板结构体。

提供了一个 OCaml 质数筛示例程序，演示了整数、列表 cons 单元格 (`Cons`) 和函数应用 (`app`) 如何在生成的 C++ 中表示。运行带有 `g++ -Dlimit=N` 参数的 C++ 代码的输出被幽默地格式化为编译器错误消息。

C++ 模板的“纯函数式”特性意味着 OCaml 的可变标准库不可用，需要进行纯函数式的重新实现。性能被认为是一个重大挑战：计算高达 10,000 的质数会消耗“大约 11 GiB 的内存”，并且需要调整 `ftemplate-depth` 参数。据称 `clang++` 会出现段错误。尽管算法改进可以加速执行，内存使用量仍然巨大。

这场日期为 2026 年 4 月 1 日的讨论，进一步证实了这个精心设计的笑话，参与者提出了幽默的问题，涉及非均匀递归数据类型等特性，并对 C++ 的固有特性发表评论。

---

## 6. 揭秘尼泊尔虚假救援骗局

**原文标题**: Inside Nepal's Fake Rescue Racket

**原文链接**: [https://kathmandupost.com/money/2026/03/27/inside-nepal-s-fake-rescue-racket](https://kathmandupost.com/money/2026/03/27/inside-nepal-s-fake-rescue-racket)

所提供的文章标题“尼泊尔假救援骗局内幕”暗示了一篇关于尼泊尔境内涉及欺诈性救援活动的不法操作的报道。

然而，所提供的内容**与该标题不符**。唯一给出的信息是：“尼泊尔证券交易所收盘上涨至2,782.18点，成交额达88.1亿卢比。”

因此，*仅*根据所提供的内容，该文章报道称尼泊尔证券交易所（Nepse）当天交易收盘上涨至2,782.18点，总成交额达88.1亿卢比。所提供文本中不包含任何关于“假救援骗局”的信息。

---

## 7. 德尔夫据称盗用了一个开源工具，并将其作为自己的产品出售。

**原文标题**: Delve allegedly forked an open-source tool and sold it as its own

**原文链接**: [https://techcrunch.com/2026/04/01/the-reputation-of-troubled-yc-startup-delve-has-gotten-even-worse/](https://techcrunch.com/2026/04/01/the-reputation-of-troubled-yc-startup-delve-has-gotten-even-worse/)

合规初创公司Delve陷入新的争议，一位名叫“DeepDelver”的匿名举报人指控称，该公司非法分叉了Sim.ai的一款名为SimStudio的开源工具，并将其作为Delve自有的“Pathways”产品出售。DeepDelver声称，Delve曾将“Pathways”宣传为内部开发的产品，尽管其与SimStudio非常相似。如果属实，此举将违反要求注明出处的Apache软件许可证。

Sim.ai的创始人兼首席执行官埃米尔·卡拉贝格（Emir Karabeg）向TechCrunch证实，Delve并未获得SimStudio的许可协议。卡拉贝格表示，他并不知道Delve会销售一个修改版本作为独立的解决方案，特别是考虑到Sim.ai此前曾是Delve的客户。卡拉贝格此前曾就Delve伪造客户数据的指控安抚过其创始人，但在得知Sim.ai的指控后，他已停止与Delve联系。

在这些指控浮出水面后，据报道，Delve已从其网站上删除了所有提及“Pathways”以及许多其他页面的内容，其媒体问询邮箱也已失效。该公司尚未回应置评请求。Delve的A轮投资者Insight Partners此前短暂下架了其关于该投资的博客文章，其在LinkedIn上的帖子也仍未恢复。此事件引发了强烈反响，并在X平台上成为热门话题。

---

## 8. 美产水泥和混凝土的AI

**原文标题**: AI for American-produced cement and concrete

**原文链接**: [https://engineering.fb.com/2026/03/30/data-center-engineering/ai-for-american-produced-cement-and-concrete/](https://engineering.fb.com/2026/03/30/data-center-engineering/ai-for-american-produced-cement-and-concrete/)

Meta is advancing the U.S. construction industry by leveraging AI to produce high-quality, sustainable concrete mixes using domestically sourced materials, aiming to reduce reliance on imported cement. Concurrent with the 2026 ACI Spring Convention, Meta is releasing an open-source AI model, Bayesian Optimization for Concrete (BOxCrete), and foundational data for developing concrete mixes.

The U.S. imports 20-25% of its cement, impacting domestic manufacturing, jobs, and adherence to U.S. environmental standards. Traditional concrete mix design is slow and expensive, relying on trial-and-error. Meta's AI-driven approach seeks to accelerate the adoption of U.S.-made materials, supporting reshoring efforts that boost American jobs and economic value.

BOxCrete, an improved model, uses Bayesian optimization to intelligently design concrete mixes. It learns from existing data, proposes high-potential formulations, incorporates user-defined constraints, and refines predictions with each test, significantly speeding up the discovery process.

This initiative has shown real-world impact through partnerships. Meta, with Amrize (North America's largest cement manufacturer) and the University of Illinois at Urbana-Champaign, is implementing AI for sustainable, domestically-produced concrete. In Rosemount, MN, an AI-optimized mix for a Meta data center achieved 43% faster structural strength and 10% reduced cracking using U.S.-sourced materials. Additionally, Pennsylvania-based Quadrel, an enterprise SaaS platform, has integrated Meta’s open-source AI framework into its software for daily mix design and quality control.

Meta's goal is to foster an industry-wide shift, making AI-optimized mix design broadly accessible to producers without changing existing workflows, ultimately reducing barriers to domestic material adoption, boosting supply chain resilience, and improving sustainability.

---

## 9. My son pleasured himself on Gemini Live. Entire family's Google accounts banned

**原文标题**: My son pleasured himself on Gemini Live. Entire family's Google accounts banned

**原文链接**: [https://old.reddit.com/r/LegalAdviceUK/comments/1s92fql/my_son_pleasured_himself_in_front_of_gemini_live/](https://old.reddit.com/r/LegalAdviceUK/comments/1s92fql/my_son_pleasured_himself_in_front_of_gemini_live/)

生成摘要时出错

---

## 10. The Claude Code Leak

**原文标题**: The Claude Code Leak

**原文链接**: [https://build.ms/2026/4/1/the-claude-code-leak/](https://build.ms/2026/4/1/the-claude-code-leak/)

The article analyzes the implications of a hypothetical "Claude Code Leak," offering five key observations beyond the leak itself.

Firstly, the author notes that despite being perceived as "garbage" code, Claude Code achieved significant success, demonstrating that strong product-market fit can trump code quality, even for developer-centric tools. This challenges the traditional belief that immaculate code is essential for valuable software.

Secondly, the piece argues that the "what" the code does matters more than "how" it's written. Anthropic prioritizes robust observability and self-healing systems to ensure functionality, enabling rapid development without perfect underlying code.

Thirdly, product-market fit remains paramount; users prioritize effective problem-solving. If Claude Code faltered, competitors like OpenAI or Google are poised to meet the existing demand for coding products.

Fourthly, the copyright response was telling. Anthropic's swift DMCA notices for leaked code forks, juxtaposed with the AI industry's stance that AI-rewritten content isn't derivative, highlights a double standard and potentially furthers the notion that "code should be free" in a libertarian sense.

Finally, the leak is ultimately deemed inconsequential. The true value of AI ecosystems lies in the seamless integration of models and their "harness" (the complete service), not the underlying source code. Users pay for great results and a cohesive experience, as evidenced by successful integrated services maintaining mindshare over open-source alternatives. The author concludes that code's intrinsic value is often overestimated; effective problem-solving and seamless integration are what truly matter to users.

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 2 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 3 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 4 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 5 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 6 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 7 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 8 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 9 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 10 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 11 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 12 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 13 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 14 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 15 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 16 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 17 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 18 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 19 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 20 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 21 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 22 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 23 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 24 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 25 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 26 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 27 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 28 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 29 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 30 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 31 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 32 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 33 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 34 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 35 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 36 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 37 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 38 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 39 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 40 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 41 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 42 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 43 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 44 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 45 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 46 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 47 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 48 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 49 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 50 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 51 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 52 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 53 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 54 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 55 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 56 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 57 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 58 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 59 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 60 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 61 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 62 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 63 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 64 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 65 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 66 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 67 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 68 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 69 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 70 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 71 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 72 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 73 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 74 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 75 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 76 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 77 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 78 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 79 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 80 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 81 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 82 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 83 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 84 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 85 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 86 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 87 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 88 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 89 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 90 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 91 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 92 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 93 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 94 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 95 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 96 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 97 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 98 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 99 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 100 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 101 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 102 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 103 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 104 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 105 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 106 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 107 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 108 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 109 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 110 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 111 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 112 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 113 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 114 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 115 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 116 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 117 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 118 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 119 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 120 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 121 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 122 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 123 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 124 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 125 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 126 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 127 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 128 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 129 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 130 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 131 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 132 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 133 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 134 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 135 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 136 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 137 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 138 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 139 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 140 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 141 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 142 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 143 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 144 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 145 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 146 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
