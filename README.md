# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-09-11.md)

*最后自动更新时间: 2026-09-11 22:02:57*
## 1. Shopify 从 React Native 回归到 Swift 和 Kotlin

**原文标题**: Shopify is moving from React Native back to Swift and Kotlin

**原文链接**: [https://shopify.engineering/back-to-native](https://shopify.engineering/back-to-native)

Shopify正在将其移动应用程序从React Native重新迁移回原生的Swift和Kotlin，这一战略转变主要是由AI编码代理（LLM）的显著进步所驱动的。尽管React Native自2020年采用以来取得了巨大成功，通过节省开发时间并实现跨栈贡献，但LLM已经从根本上改变了两次构建功能的成本效益分析。

AI代理现在极大地减少了跨平台的实现、转换、测试和审查工作量，从而削弱了React Native共享代码的核心优势。这使得Shopify能够拥抱原生开发的优势——更紧密的平台能力和工具，而无需承担此前令人望而却却步的“两次构建”成本。

Shopify正在采用全新的（从零开始重建）方法，利用LLM加速开发；Shop应用仅用12周就完成了原生重建并发布。为确保质量，他们开发了“Helix”系统，该系统将迁移过程分解为小块、测试驱动并经过人工审查的检查点。此外，一种新的代理可寻址架构将业务逻辑与UI解耦，使代理能够通过CLI在毫秒内迭代和测试代码，绕过缓慢的模拟器交互。

关于他们的开源React Native库：Skia将被分叉并继续由William Candillon负责维护，FlashList将获得关键修复，同时寻找新的长期维护者，Restyle将被归档。Shopify计划迁移所有应用，旨在超越当前的质量标准，并将公开分享此次雄心勃勃的AI驱动移动工程实践的经验。

---

## 2. 深度求索 v4.1 闪

**原文标题**: DeepSeek v4.1 Flash

**原文链接**: [https://twitter.com/deepseek_ai/status/2097930608790167907](https://twitter.com/deepseek_ai/status/2097930608790167907)

DeepSeek推出了其新的AI模型DeepSeek-V4.1-Flash，强调其更智能、更快、更高效。该模型是他们新架构系列中最小的一款，并具备原生的视觉理解能力。DeepSeek-V4.1-Flash旨在提升能力、加快推理速度、提高吞吐量，并可扩展至更大的模型。

---

## 3. 更多质疑：研究人员能否将未发表数学托付给OpenAI

**原文标题**: More questions about whether researchers can trust OpenAI with unpublished math

**原文链接**: [https://mathstodon.xyz/@andreasthom/117240535270608201](https://mathstodon.xyz/@andreasthom/117240535270608201)

生成摘要时出错

---

## 4. 不要让任何人拿走你的一大箱线缆。

**原文标题**: Don't let anyone take away your big box of cables

**原文链接**: [https://blog.jim-nielsen.com/2026/hands-off-my-cables/](https://blog.jim-nielsen.com/2026/hands-off-my-cables/)

作者偶然发现了一篇泰勒·高（Tyler Gaw）的在线帖子，深有共鸣。高在文中分享了他终于从自己那存了十多年的“一大箱线缆”中找到两根线缆的经历，这验证了他囤积线缆的习惯是正确的。他最后总结道：“永远不要让任何人拿走你那一大箱线缆。”

受到这个令人感同身受的“启示”的启发，作者决定采取行动。他截屏了高的帖子，打印出来，剪下，然后用透明打包胶带将其贴在了自己那“一大箱线缆”的正面，这箱线缆被他妻子标注为“家庭科技箱”（FAMILY TECHNO BOX）。这个实际行动不仅时刻提醒着盒子存在的价值，也让作者每当放入新线缆时，都能重拾乐趣和目的感。它也对那些可能考虑扔掉其内容的家庭成员起到了警示作用。作者希望有一天，他的孩子们能发现这个箱子，并听从箱子外面所展示的“永恒的忠告”。

---

## 5. Rust is tier-1 language at Microsoft

**原文标题**: Rust is tier-1 language at Microsoft

**原文链接**: [https://rustfoundation.org/media/guest-post-rust-is-tier-1-language-at-microsoft/](https://rustfoundation.org/media/guest-post-rust-is-tier-1-language-at-microsoft/)

Microsoft has officially designated Rust as a "Tier-1 language" for internal development, positioning it alongside C++, C#, and TypeScript. This reflects Rust's strategic importance and Microsoft's substantial investment in the language. The Tier-1 status ensures a "paved path" for internal teams, providing secure toolchain builds, productive tooling, quality workflows, deep platform integration, and compliance with Microsoft's SDL requirements.

A key innovation driving this integration is `rustc_codegen_utc`, an alternative code generation backend for `rustc`. This backend connects Rust directly to the MSVC backend (UTC), Windows' native platform compiler. Its development ensures high compatibility with the Windows tooling ecosystem and ABI, enabling crucial features like binary hardening, code security, post-link compliance (including Hotpatch), and seamless interoperability for hybrid Rust/C++ projects. `rustc_codegen_utc` leverages existing MSVC capabilities for cross-language optimization, debugging, profiling, and diagnostics, avoiding redundant development for Windows-specific features.

This unified code generation platform for Rust and C++ on Windows minimizes maintenance and evolution costs, allowing new platform innovations to benefit both languages simultaneously. It's particularly vital for hybrid projects, ensuring both Rust and C++ participate equally in development workflows. `rustc_codegen_utc` has been production-ready since early 2026, is self-hosted since Rust 1.90, and is being adopted by a growing number of Microsoft repositories, signifying a sustained investment in Rust's complete engineering lifecycle at the company.

---

## 6. HN 展示：如果光速是 5 公里/小时会怎么样？

**原文标题**: Show HN: What if the speed of light was 5 km/h?

**原文链接**: [https://rivendell.dmitrybrant.com/relativity/](https://rivendell.dmitrybrant.com/relativity/)

“相对论公园”是一个交互式模拟，它通过将光速大幅降低至每小时仅5公里（相当于轻快的步行速度），探索狭义相对论的奇异效应。

在这个虚拟环境中，用户可以亲身体验如果光速与日常人类运动速度相当，会发生什么。当玩家加速时，他们将观察到经典的相对论现象，例如长度收缩（物体看起来更短）、时间膨胀（他们的个人时钟比“世界”时钟走得慢）以及特雷尔旋转。光的多普勒效应也变得明显，导致前方的物体发生蓝移，后方的物体发生红移，以及移动的物体表现出横向多普勒效应。

该模拟强调，即使在如此低速下，光速仍然是一个渐近极限，永远无法真正达到。用户使用键盘控制（加速、停止、切换效果、重置）和鼠标进行环顾来导航和交互，让他们沉浸在一个相对论物理可见且直观的世界中。

---

## 7. 克劳德仅限18岁以上人士使用。

**原文标题**: Claude is only available to people over 18 years

**原文链接**: [https://support.claude.com/en/articles/15171100-age-assurance-on-claude](https://support.claude.com/en/articles/15171100-age-assurance-on-claude)

Anthropic的消费级产品Claude仅限18岁及以上用户使用。用户在账户设置时需要确认年龄。如果系统检测到用户可能未满18岁的信号，其账户将被禁用，并要求进行年龄验证。

年龄验证过程由第三方平台Yoti处理。用户将收到一封包含验证链接的电子邮件。验证成功后，账户将被恢复。Yoti提供以下几种选项：
1.  **面部年龄估算：** 用户拍摄自拍照进行年龄估算，无需身份证件。
2.  **证件验证：** 用户上传政府颁发的身份证件（如护照或驾照）照片。
3.  **Yoti数字身份App：** 用户可以从其现有Yoti App中共享已验证的“18岁以上”属性。

关于数据保护，Yoti是一家经过独立审计的服务提供商。您的自拍照、证件图像以及任何个人数据在年龄验证完成后会立即被Yoti删除。Anthropic绝不会查看或存储您的身份证件或图像；它仅从Yoti接收通过/失败的结果，从而确保用户隐私。

---

## 8. 我有一个理论，软件会把人逼疯。

**原文标题**: I have a theory that software drives people insane

**原文链接**: [https://graybeard.ing/software-drives-people-insane/](https://graybeard.ing/software-drives-people-insane/)

生成摘要时出错

---

## 9. Automattic's board forces CEO Matt Mullenweg into leave of absence

**原文标题**: Automattic's board forces CEO Matt Mullenweg into leave of absence

**原文链接**: [https://techcrunch.com/2026/09/09/automattics-board-forces-ceo-matt-mullenweg-into-leave-of-absence/](https://techcrunch.com/2026/09/09/automattics-board-forces-ceo-matt-mullenweg-into-leave-of-absence/)

Automattic founder and CEO Matt Mullenweg has been forced into a paid leave of absence by the company's board of directors, a decision he opposed and described as a "conspiracy." According to a Slack message from Mullenweg, CFO Mark Davies, along with board members Ann Dunwoody, Toni Schneider, and Sue Decker, voted for the leave, denying his request for legal counsel. Mark Davies has been appointed interim CEO.

Automattic confirmed the leave, stating full confidence in Davies' leadership. While Mullenweg is on leave from Automattic, Mary Hubbard, Executive Director of WordPress.org, clarified that Mullenweg remains the leader of the open-source WordPress project, which is unaffected by the change at the commercial company.

The board's action follows a period of controversy under Mullenweg's leadership. Automattic is engaged in a protracted legal dispute with WP Engine, initiated by Mullenweg's demand for royalty fees for WordPress brand usage, leading to WP Engine suing for defamation and abuse of power. Other issues include Mullenweg telling employees to quit if they disagreed with him (leading to 159 departures), threatening and deactivating accounts of open-source community members, and a 16% staff layoff in April 2025.

Employee reactions vary from "ecstatic" and "relieved" to concerns about instability. Mullenweg's recent posts on X hinted at the cause, referencing an allegation of spoiling evidence in the WP Engine lawsuit and anticipating "smear attacks."

---

## 10. Cognition launches new SWE-2 model, Rivaling Fable 5.1 and GPT-Astra

**原文标题**: Cognition launches new SWE-2 model, Rivaling Fable 5.1 and GPT-Astra

**原文链接**: [https://cognition.com/blog/swe-2](https://cognition.com/blog/swe-2)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-09-11](output/hacker_news_summary_2026-09-11.md) |
| 2 | [2026-09-10](output/hacker_news_summary_2026-09-10.md) |
| 3 | [2026-09-04](output/hacker_news_summary_2026-09-04.md) |
| 4 | [2026-09-09](output/hacker_news_summary_2026-09-09.md) |
| 5 | [2026-09-07](output/hacker_news_summary_2026-09-07.md) |
| 6 | [2026-09-08](output/hacker_news_summary_2026-09-08.md) |
| 7 | [2026-09-03](output/hacker_news_summary_2026-09-03.md) |
| 8 | [2026-09-05](output/hacker_news_summary_2026-09-05.md) |
| 9 | [2026-09-06](output/hacker_news_summary_2026-09-06.md) |
| 10 | [2026-08-26](output/hacker_news_summary_2026-08-26.md) |
| 11 | [2026-09-01](output/hacker_news_summary_2026-09-01.md) |
| 12 | [2026-08-31](output/hacker_news_summary_2026-08-31.md) |
| 13 | [2026-08-28](output/hacker_news_summary_2026-08-28.md) |
| 14 | [2026-09-02](output/hacker_news_summary_2026-09-02.md) |
| 15 | [2026-08-30](output/hacker_news_summary_2026-08-30.md) |
| 16 | [2026-08-29](output/hacker_news_summary_2026-08-29.md) |
| 17 | [2026-08-20](output/hacker_news_summary_2026-08-20.md) |
| 18 | [2026-08-25](output/hacker_news_summary_2026-08-25.md) |
| 19 | [2026-08-18](output/hacker_news_summary_2026-08-18.md) |
| 20 | [2026-08-19](output/hacker_news_summary_2026-08-19.md) |
| 21 | [2026-08-21](output/hacker_news_summary_2026-08-21.md) |
| 22 | [2026-08-17](output/hacker_news_summary_2026-08-17.md) |
| 23 | [2026-08-23](output/hacker_news_summary_2026-08-23.md) |
| 24 | [2026-08-22](output/hacker_news_summary_2026-08-22.md) |
| 25 | [2026-08-24](output/hacker_news_summary_2026-08-24.md) |
| 26 | [2026-08-12](output/hacker_news_summary_2026-08-12.md) |
| 27 | [2026-08-14](output/hacker_news_summary_2026-08-14.md) |
| 28 | [2026-08-10](output/hacker_news_summary_2026-08-10.md) |
| 29 | [2026-08-11](output/hacker_news_summary_2026-08-11.md) |
| 30 | [2026-08-16](output/hacker_news_summary_2026-08-16.md) |
| 31 | [2026-08-13](output/hacker_news_summary_2026-08-13.md) |
| 32 | [2026-08-15](output/hacker_news_summary_2026-08-15.md) |
| 33 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 34 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 35 | [2026-08-09](output/hacker_news_summary_2026-08-09.md) |
| 36 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 37 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 38 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 39 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 40 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 41 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 42 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 43 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 44 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 45 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 46 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 47 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 48 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 49 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 50 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 51 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 52 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 53 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 54 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 55 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 56 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 57 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 58 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 59 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 60 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 61 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 62 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 63 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 64 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 65 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 66 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 67 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 68 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 69 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 70 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 71 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 72 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 73 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 74 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 75 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 76 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 77 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 78 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 79 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 80 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 81 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 82 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 83 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 84 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 85 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 86 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 87 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 88 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 89 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 90 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 91 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 92 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 93 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 94 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 95 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 96 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 97 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 98 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 99 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 100 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 101 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 102 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 103 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 104 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 105 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 106 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 107 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 108 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 109 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 110 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 111 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 112 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 113 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 114 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 115 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 116 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 117 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 118 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 119 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 120 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 121 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 122 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 123 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 124 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 125 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 126 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 127 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 128 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 129 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 130 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 131 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 132 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 133 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 134 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 135 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 136 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 137 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 138 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 139 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 140 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 141 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 142 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 143 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 144 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 145 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 146 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 147 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 148 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 149 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 150 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 151 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 152 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 153 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 154 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 155 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 156 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 157 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 158 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 159 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 160 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 161 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 162 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 163 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 164 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 165 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 166 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 167 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 168 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 169 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 170 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 171 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 172 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 173 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 174 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 175 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 176 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 177 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 178 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 179 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 180 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 181 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 182 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 183 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 184 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 185 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 186 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 187 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 188 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 189 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 190 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 191 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 192 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 193 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 194 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 195 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 196 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 197 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 198 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 199 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 200 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 201 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 202 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 203 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 204 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 205 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 206 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 207 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 208 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 209 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 210 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 211 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 212 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 213 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 214 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 215 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 216 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 217 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 218 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 219 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 220 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 221 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 222 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 223 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 224 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 225 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 226 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 227 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 228 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 229 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 230 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 231 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 232 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 233 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 234 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 235 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 236 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 237 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 238 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 239 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 240 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 241 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 242 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 243 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 244 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 245 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 246 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 247 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 248 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 249 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 250 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 251 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 252 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 253 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 254 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 255 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 256 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 257 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 258 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 259 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 260 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 261 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 262 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 263 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 264 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 265 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 266 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 267 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 268 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 269 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 270 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 271 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 272 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 273 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 274 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 275 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 276 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 277 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 278 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 279 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 280 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 281 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 282 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 283 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 284 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 285 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 286 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 287 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 288 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 289 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 290 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 291 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 292 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 293 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 294 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 295 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 296 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 297 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 298 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 299 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 300 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 301 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 302 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 303 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 304 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 305 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 306 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
