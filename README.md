# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-07-26.md)

*最后自动更新时间: 2026-07-26 20:37:32*
## 1. 安卓可能很快会限制本机ADB

**原文标题**: Android may soon restrict on-device ADB

**原文链接**: [https://kitsumed.github.io/blog/posts/android-may-soon-restrict-on-device-adb/](https://kitsumed.github.io/blog/posts/android-may-soon-restrict-on-device-adb/)

Google IssueTracker 上的一场持续讨论表明，Google 可能会限制设备上的 ADB 连接，这一举动已被 Shizuku 相关应用的开发者 Kitsumed 指出。ADB（安卓调试桥）是一款功能强大的开发者工具，能够授予高权限，传统上通过 USB、TCP/IP 或无线调试进行连接。

“设备上 ADB”是指通过回环地址 (127.0.0.1) 在同一设备上运行 ADB 客户端和服务器。这种设置支持了一个小众但重要的开发者和高级用户工具生态系统，例如 Shizuku，它能够为残障用户提供通话录音等功能。

这项由一个安全漏洞 (CVE-2026-0073) 引发的拟议更改，建议将 ADB 守护进程 (ADBD) 限制为仅绑定到 Wi-Fi 接口 (`wlan0`)。一位 Google 维护者解释说，此举是出于对恶意应用利用本地主机套接字进行权限提升的担忧。

Kitsumed 认为，这种全面限制是过度且不必要的。他解释说，“恶意行为者”无法单方面利用设备上 ADB；它需要用户进行多项明确的手动操作，例如启用 USB 调试、无线 ADB 配对或授权 TCP/IP 连接。他强调了设备上 ADB 对于无法使用电脑的开发者以及各种重要的，高级用户工具来说，存在诸多合法用途。

作者倡导一种平衡的方法：默认限制设备上 ADB，但在用户知晓相关风险后，允许他们通过持久设置禁用此限制。他认为彻底锁定是没有必要的，这类似于因潜在滥用而移除其他强大的安卓功能（如辅助功能服务），并鼓励技术用户在 Google IssueTracker 上提供建设性反馈。

---

## 2. 干掉Cookie横幅

**原文标题**: Kill The Cookie Banner

**原文链接**: [https://killthecookiebanner.eu/](https://killthecookiebanner.eu/)

文章呼吁#废除Cookie横幅，认为这些普遍存在的横幅旨在诱骗用户同意在线追踪，尽管欧盟法律默认禁止此类行为。文章指出，误导性横幅导致高达90%的同意率，而实际上只有大约3%的用户真正希望被追踪。

欧盟委员会为2025年秋季提出的解决方案涉及自动化隐私信号。用户只需在浏览器中一次性设置其追踪偏好（接受、拒绝、限制），浏览器随后便会将这些偏好传达给网站和应用程序。这种简单且现有的技术已在美国某些州获得法律支持。

然而，追踪行业，尤其是谷歌，正在极力游说反对这项提案。它们担心一旦用户可以轻松表达其偏好，同意率将会下降，因此已成功影响了多个成员国阻止这项倡议，并正在向欧洲议会施压，要求其否决该提案。

文章敦促公众采取行动，因为这项决定尚未最终确定。鼓励读者联系他们在欧洲议会或国家政府的代表，以表达他们的不满，并支持自动化隐私信号提案。文章澄清，虽然支持这项具体的提案，但对更广泛的“数字综合法案”法律改革的其他部分不予支持，因为担心这会削弱民众的权利。这项倡议由欧洲各地的公民社会组织牵头。

---

## 3. 汉娜·弗莱荣获2026年莱拉瓦蒂奖，表彰其数学普及贡献

**原文标题**: Hannah Fry Wins the Leelavati Prize in 2026 for Mathematics Outreach

**原文链接**: [https://www.maths.cam.ac.uk/features/professor-hannah-fry-wins-leelavati-prize](https://www.maths.cam.ac.uk/features/professor-hannah-fry-wins-leelavati-prize)

汉娜·弗莱教授在国际数学家大会（ICM）上荣获国际数学联盟（IMU）于2026年颁发的莱拉瓦蒂奖，以表彰她在提高公众对数学认知方面所做的杰出贡献。弗莱于2025年1月成为剑桥大学首位“公众理解数学”教授，她是一位著名的播音员、作家、播客主持人以及社交媒体明星。

颁奖词称赞她为“数学思维最重要的全球大使”，其工作超越了传统的科学传播。她通过多种媒体，以非凡的创造力将数学转化为“充满奇迹和实用性的语言”，同时不减损其深度和广度。弗莱解释了她分享数学“绝对乐趣”和“奇妙秘密”的热情，她认为自己的角色是通过“开启人们的想象空间”来提供动力。

弗莱获得的广泛认可包括克里斯托弗·齐曼奖章（2018年）、皇家学会戴维·阿滕伯勒奖（2024年）、凭借《与汉娜·弗莱共创未来》获得的艾美奖（2025年），以及凭借《科学万象》获得的威比奖（2026年）。她于2026年被《时代》杂志评为全球100位最具影响力的数字创作者之一，其Instagram粉丝超过200万。她还通过皇家学会圣诞讲座等活动激励未来的数学家。DAMTP系主任尼克·多利教授称赞她是现代生活中数学重要性传播方面最重要的贡献者之一。

---

## 4. 他们对你玩消失了吗？

**原文标题**: Did they ghost you?

**原文链接**: [https://didtheyghostyou.com/](https://didtheyghostyou.com/)

这份题为“你被‘放鸽子’了吗？”的文本传递了一个直接的信息：如果你在面试后经历公司对你“放鸽子”，你应该举报他们。核心建议是，对那些在面试后不予回应的雇主采取行动。

---

## 5. Claude 5 生成模型的上下文工程新规

**原文标题**: The new rules of context engineering for Claude 5 generation models

**原文链接**: [https://claude.com/blog/the-new-rules-of-context-engineering-for-claude-5-generation-models](https://claude.com/blog/the-new-rules-of-context-engineering-for-claude-5-generation-models)

本文概述了针对Claude 5代模型（例如Opus 5、Fable 5）的“上下文工程新规则”，强调了从过度约束模型转向利用其增强的判断力和能力的重大转变。Anthropic移除了Claude Code系统提示中80%以上的内容，且性能没有下降，这表明旧方法对于高级模型而言适得其反。

最佳实践的关键变化包括：

*   **从明确规则到允许Claude判断：** 不再使用严格的指令（例如，“无注释”），而是引导Claude匹配周围代码的风格。
*   **从工具示例到设计富有表现力的接口：** 侧重于精心设计的参数，而非具体的用法示例，后者可能会限制探索。
*   **从预先提供上下文到渐进式披露：** 仅在需要时加载技能、工具和`CLAUDE.md`内容，避免不必要的上下文。
*   **从重复指令到简单的工具描述：** 将指令放置在工具描述中，而非在系统提示中重复。
*   **从手动`CLAUDE.md`记忆到自动记忆：** Claude现在自动保存相关记忆。
*   **从简单规范到丰富参考：** 利用详细的测试、函数、HTML工件或评分标准作为高保真参考，优先选择基于代码的格式。

对用户而言，这意味着保持`CLAUDE.md`轻量化并专注于代码库中的“陷阱”，使用技能作为特定知识的定向指南，并提供丰富、上下文相关的参考。`claude doctor`命令有助于简化现有上下文。核心原则是，通过信任Claude的高级智能并提供动态、简洁的指导来“解放”它。

---

## 6. 开放权重AI正迎来其Kubernetes般的时刻。

**原文标题**: Open-weight AI is having its Kubernetes moment

**原文链接**: [https://tobi.knaup.me/2026-07-25-open-weight-ai-is-having-its-kubernetes-moment/](https://tobi.knaup.me/2026-07-25-open-weight-ai-is-having-its-kubernetes-moment/)

无法访问文章链接。

---

## 7. Opus 5 is currently #1 on Artificial Analysis Intelligence Leaderboard

**原文标题**: Opus 5 is currently #1 on Artificial Analysis Intelligence Leaderboard

**原文链接**: [https://artificialanalysis.ai/models](https://artificialanalysis.ai/models)

The "Artificial Analysis Intelligence Leaderboard" offers a comprehensive comparison of AI models across key performance metrics. **Claude Opus 5 (max) and Claude Opus 5 (xhigh) are currently ranked #1 for intelligence**, closely followed by Claude Fable 5 and GPT-5.6 Sol (max).

The platform evaluates models across several critical dimensions:
*   **Intelligence:** Measured by the Artificial Analysis Intelligence Index v4.1, which synthesizes results from 9 evaluations including agentic tasks (GDPval-AA v2, 𝜏³-Banking, Terminal-Bench v2.1), coding (SciCode), reasoning (Humanity's Last Exam, GPQA Diamond, CritPt), knowledge (AA-Omniscience), and long context reasoning (AA-LCR).
*   **Output Speed:** Mercury 2 (953 tokens/s) and Gemini 3.5 Flash-Lite (417 tokens/s) are the fastest.
*   **Latency:** Gemini 2.5 Flash-Lite (0.35s) and Command A+ (0.39s) exhibit the lowest latency.
*   **Price:** Devstral 2 and North Mini Code are the most cost-effective at $0.00 per M tokens.
*   **Context Window:** Llama 4 Scout (10M tokens) and Grok 4.20 0309 (2M tokens) offer the largest context windows.

The analysis also provides breakdowns of intelligence evaluations, model openness, and detailed cost metrics, including cost per task, total cost, and token pricing for input, output, reasoning, and caching. Comparative charts show relationships such as Intelligence vs. Cost, Speed, and Time per Task. Performance figures represent first-party API data or the median across providers.

---

## 8. A shell colon does nothing. Use it anyway

**原文标题**: A shell colon does nothing. Use it anyway

**原文链接**: [https://refp.se/articles/your-shell-and-the-magic-colon](https://refp.se/articles/your-shell-and-the-magic-colon)

生成摘要时出错

---

## 9. GrapheneOS protections against data extraction from locked devices

**原文标题**: GrapheneOS protections against data extraction from locked devices

**原文链接**: [https://discuss.grapheneos.org/d/40700-grapheneos-protections-against-data-extraction-from-locked-devices](https://discuss.grapheneos.org/d/40700-grapheneos-protections-against-data-extraction-from-locked-devices)

GrapheneOS provides robust defenses against data extraction from locked devices, building upon Android's security features and Pixel hardware. Its core protections include strong disk encryption, which requires exploiting the OS or brute-forcing the PIN/password.

A key feature is its advanced secure element (SE), implementing strict rate limiting compliant with Android 16 QPR2 standards. This allows only 20 attempts, with escalating delays (e.g., 4 hours after 10 attempts, 41 days after 15), and resists insider attacks by requiring owner authentication for firmware updates. This SE capability has been present in Pixels since the Pixel 2.

GrapheneOS enhances authentication by raising password limits to 128 characters for high-entropy passphrases. It introduces an optional 2nd factor fingerprint PIN, reducing fingerprint attempts to 5 and requiring a PIN to unlock the hardware keystore.

For exploit protection, GrapheneOS hardens the OS with memory allocators and hardware memory tagging (MTE). Physical attack defenses include blocking new USB connections and disabling USB data while locked.

GrapheneOS pioneered a locked device auto-reboot timer (default 18 hours), which returns the device to Before First Unlock (BFU) state with memory zeroing, a feature later adopted by Apple and Google. It also enables secondary users and Private Spaces to return to BFU without a full reboot.

Finally, a duress PIN/password feature allows wiping the device if entered in any authentication prompt across all profiles, providing a critical failsafe against forced data recovery, though it is not the primary defense mechanism.

---

## 10. Taylor Farms Called White House to Try to Delay Cyclospora Recall

**原文标题**: Taylor Farms Called White House to Try to Delay Cyclospora Recall

**原文链接**: [https://www.wsj.com/health/taylor-farms-cyclospora-recall-delay-call-41fef0bc](https://www.wsj.com/health/taylor-farms-cyclospora-recall-delay-call-41fef0bc)

Unable to access the article link.

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 2 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 3 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 4 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 5 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 6 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 7 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 8 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 9 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 10 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 11 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 12 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 13 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 14 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 15 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 16 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 17 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 18 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 19 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 20 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 21 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 22 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 23 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 24 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 25 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 26 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 27 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 28 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 29 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 30 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 31 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 32 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 33 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 34 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 35 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 36 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 37 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 38 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 39 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 40 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 41 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 42 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 43 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 44 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 45 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 46 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 47 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 48 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 49 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 50 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 51 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 52 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 53 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 54 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 55 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 56 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 57 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 58 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 59 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 60 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 61 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 62 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 63 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 64 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 65 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 66 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 67 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 68 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 69 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 70 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 71 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 72 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 73 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 74 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 75 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 76 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 77 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 78 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 79 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 80 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 81 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 82 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 83 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 84 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 85 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 86 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 87 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 88 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 89 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 90 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 91 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 92 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 93 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 94 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 95 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 96 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 97 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 98 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 99 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 100 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 101 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 102 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 103 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 104 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 105 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 106 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 107 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 108 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 109 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 110 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 111 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 112 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 113 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 114 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 115 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 116 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 117 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 118 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 119 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 120 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 121 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 122 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 123 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 124 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 125 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 126 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 127 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 128 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 129 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 130 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 131 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 132 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 133 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 134 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 135 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 136 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 137 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 138 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 139 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 140 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 141 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 142 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 143 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 144 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 145 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 146 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 147 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 148 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 149 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 150 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 151 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 152 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 153 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 154 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 155 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 156 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 157 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 158 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 159 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 160 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 161 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 162 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 163 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 164 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 165 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 166 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 167 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 168 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 169 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 170 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 171 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 172 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 173 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 174 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 175 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 176 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 177 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 178 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 179 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 180 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 181 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 182 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 183 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 184 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 185 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 186 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 187 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 188 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 189 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 190 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 191 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 192 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 193 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 194 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 195 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 196 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 197 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 198 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 199 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 200 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 201 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 202 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 203 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 204 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 205 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 206 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 207 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 208 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 209 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 210 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 211 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 212 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 213 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 214 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 215 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 216 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 217 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 218 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 219 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 220 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 221 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 222 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 223 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 224 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 225 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 226 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 227 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 228 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 229 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 230 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 231 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 232 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 233 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 234 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 235 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 236 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 237 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 238 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 239 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 240 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 241 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 242 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 243 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 244 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 245 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 246 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 247 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 248 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 249 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 250 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 251 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 252 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 253 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 254 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 255 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
| 256 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 257 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 258 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 259 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 260 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 261 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
