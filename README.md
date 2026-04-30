# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-04-30.md)

*最后自动更新时间: 2026-04-30 20:38:29*
## 1. 戈斯蒂离开吉特哈布

**原文标题**: Ghostty is leaving GitHub

**原文链接**: [https://mitchellh.com/writing/ghostty-leaving-github](https://mitchellh.com/writing/ghostty-leaving-github)

2026年4月28日，Mitchell Hashimoto宣布了一项“非理性地悲伤”的决定，将他的项目Ghostty从GitHub上迁移走。作为一名自2008年2月（用户1299）起、拥有18年使用历史的长期用户，Hashimoto对GitHub表达了深厚的感情，认为它是快乐和灵感的源泉，他将自己大部分生命和开源工作，包括Vagrant，都奉献于此。

尽管有如此深厚的联系，他却公开表达了批评，称GitHub“每天都在让我失望”。Ghostty迁移的主要原因是持续且令人沮丧的停机，这些停机影响了PR审核、问题追踪和GitHub Actions等核心功能。Hashimoto指出，在过去一个月里，几乎每天都有中断，这使得GitHub不再是“认真工作”的地方。由于这些持续的干扰，他觉得“无法再使用GitHub进行编码了”。

此次迁移将是渐进的，Ghostty最终将移除所有GitHub依赖，但会保留一个只读镜像。Hashimoto目前正在与多家商业和FOSS（自由及开源软件）提供商讨论Ghostty的新归宿。尽管Ghostty的迁移是出于对维护者和社区的影响，但他个人的项目目前仍将留在GitHub上。这一决定已筹划数月，早于最近的大规模停机事件，突显了可靠性问题的持续性。

---

## 2. Zed 1.0

**原文标题**: Zed 1.0

**原文链接**: [https://zed.dev/blog/zed-1-0](https://zed.dev/blog/zed-1-0)

Nathan Sobo announced the launch of Zed 1.0, marking a significant milestone for the code editor. Unlike its predecessor Atom (which spawned Electron), Zed was built from the ground up in Rust, utilizing a custom GPU-driven UI framework called GPUI. This "video game-like" approach provides superior performance and deep control, overcoming the inherent limitations of web-based editors.

Zed 1.0 represents a mature and capable editor, supporting dozens of programming languages, Git integration, SSH remoting, and debugging across Mac, Windows, and Linux. A core differentiator is its AI-native architecture, integrating multiple AI agents with keystroke-level prediction speed and supporting various agents like Claude and Cursor via its Agent Client Protocol. Furthermore, "Zed for Business" is launching to facilitate company-wide deployment with centralized management.

While not "perfect" or "done," 1.0 signifies a "tipping point" where most developers will find Zed highly capable and performant, encouraging previous users to revisit it. Looking ahead, Zed's vision is to be the most performant and collaborative coding environment, evolving collaboration to include humans and AI agents simultaneously. This future is powered by the actively developed DeltaDB, a CRDT-based synchronization engine enabling character-level, real-time co-editing between humans and AI. The team emphasizes this is a milestone, not a finish line, with weekly releases continuing.

---

## 3. 复制失败

**原文标题**: Copy Fail

**原文链接**: [https://copy.fail/](https://copy.fail/)

"Copy Fail" (CVE-2026-31431) 是一个影响严重的Linux内核本地提权漏洞，几乎影响所有内核构建于2017年至其补丁发布之间的主流Linux发行版。它允许任何非特权本地用户在无需网络访问或特殊内核功能的情况下，利用内核加密API (AF_ALG) 获取root权限。

该漏洞对共享开发箱、Kubernetes/容器集群、CI/CD运行器和云SaaS平台等多租户环境构成高风险，可能导致跨租户攻击或在宿主机上获取root权限。对于标准Linux服务器，它构成中等风险；对于单用户工作站，风险较低，主要作为后渗透阶段的提权手段。

一个概念验证 (PoC) Python脚本已发布，通过编辑 `/usr/bin/su` 等setuid二进制文件的页缓存，演示了如何获得一个真实的、非持久性的root shell。

缓解措施包括更新内核以包含主线提交 `a664bf3d603d`，该提交回滚了特定的 `algif_aead` 优化。作为一种即时 workaround，可以安全地禁用 `algif_aead` 模块，因为它对大多数系统影响很小，这些系统通常不使用AF_ALG作为其核心加密服务。对于不受信任的工作负载，还建议通过seccomp阻止AF_ALG套接字创建。

该漏洞由Xint Code的AI分析工具发现。它于2026年3月23日被报告，于2026年4月1日完成补丁，并于2026年4月29日公开披露。

---

## 4. HERMES.md in commit messages causes requests to route to extra usage billing

**原文标题**: HERMES.md in commit messages causes requests to route to extra usage billing

**原文链接**: [https://github.com/anthropics/claude-code/issues/53262](https://github.com/anthropics/claude-code/issues/53262)

A critical bug in Claude Code v2.1.119 (on macOS, Apple Silicon) routes API requests to "extra usage" billing instead of the user's included plan quota when the case-sensitive string "HERMES.md" is present in a git repository's recent commit messages.

This issue is triggered specifically by the string "HERMES.md" in commit messages, not by a file of that name on disk. Commits like "hermes.md" (lowercase), "HERMES" (without extension), or "AGENTS.md" do not cause the problem. When triggered, subsequent `claude` commands fail with an "out of extra usage" error, even if the main plan quota is largely unused.

The bug led to one user silently burning through over $200 in extra usage credits, making their projects unusable while their Max 20x plan capacity remained at 86%. The error message provided no indication of the root cause, making diagnosis extremely difficult.

The expected behavior is that API request billing should not depend on the content of git commit messages; all requests from a plan subscriber should first utilize their included plan quota. The bug was discovered through a systematic binary search of git commit history.

---

## 5. Cursor Camp

**原文标题**: Cursor Camp

**原文链接**: [https://neal.fun/cursor-camp/](https://neal.fun/cursor-camp/)

生成摘要时出错

---

## 6. 哥布林从何而来

**原文标题**: Where the goblins came from

**原文链接**: [https://openai.com/index/where-the-goblins-came-from/](https://openai.com/index/where-the-goblins-came-from/)

从GPT-5.1开始，OpenAI模型出乎意料地、并且越来越多地使用“妖精”、“小妖精”及其他生物比喻。这种“妖精之谜”最初很微妙，但随着提及次数的增多，它变成了一个重大问题。

调查将这种行为追溯到“书呆子”（Nerdy）人格定制功能。在训练期间，模型在开发这种人格时，在不知情的情况下，对包含生物的比喻给予了特别高的奖励。尽管“书呆子”人格仅占ChatGPT回应的2.5%，但它却占据了所有“妖精”提及次数的66.7%，这凸显了两者之间的强烈关联。

分析证实，旨在用于“书呆子”人格的奖励信号始终偏爱包含生物词语的输出。关键的是，强化学习导致这种风格上的习惯从“书呆子”情境转移并扩散到模型的一般行为中，形成了一个反馈循环，即富含生物词语的例子被纳入监督微调数据。这也导致了其他生物习惯的出现，例如“浣熊”和“巨魔”。

为解决此问题，OpenAI在GPT-5.4于三月发布后，停用了“书呆子”人格。他们还移除了有问题的奖励信号，并过滤了包含生物词语的训练数据。尽管更早开始训练的GPT-5.5仍显示出一些倾向（需要特定的开发者指令来缓解），但这些措施旨在根除过多的生物比喻。

这一事件强调了微妙的奖励信号如何能够深刻且出人意料地塑造模型行为，甚至超出其预期范围进行泛化，这凸显了对审计和纠正模型怪癖的强大工具的重要性。

---

## 7. 在线年龄验证是绝不能退让的底线。

**原文标题**: Online age verification is the hill to die on

**原文链接**: [https://x.com/GlennMeder/status/2049088498163216560](https://x.com/GlennMeder/status/2049088498163216560)

尽管标题如此，但所提供的内容并非一篇讨论在线年龄验证的文章。相反，它是一个来自 x.com（前身为 Twitter）的技术错误提示。该消息指出，用户浏览器中的 JavaScript 已被禁用，并指示用户启用它或切换到受支持的浏览器以继续使用该平台。它还显示了标准的网站页脚链接，包括帮助中心、服务条款、隐私政策、Cookie 政策、法律声明和广告信息，以及一份针对 X Corp. 且日期为 2026 年的版权声明。因此，没有关于在线年龄验证的内容可供总结。

---

## 8. Claude Code refuses requests or charges extra if your commits mention "OpenClaw"

**原文标题**: Claude Code refuses requests or charges extra if your commits mention "OpenClaw"

**原文链接**: [https://twitter.com/theo/status/2049645973350363168](https://twitter.com/theo/status/2049645973350363168)

生成摘要时出错

---

## 9. Before GitHub

**原文标题**: Before GitHub

**原文链接**: [https://lucumr.pocoo.org/2026/4/28/before-github/](https://lucumr.pocoo.org/2026/4/28/before-github/)

生成摘要时出错

---

## 10. Bugs Rust won't catch

**原文标题**: Bugs Rust won't catch

**原文链接**: [https://corrode.dev/blog/bugs-rust-wont-catch/](https://corrode.dev/blog/bugs-rust-wont-catch/)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 2 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 3 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 4 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 5 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 6 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 7 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 8 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 9 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 10 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 11 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 12 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 13 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 14 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 15 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 16 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 17 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 18 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 19 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 20 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 21 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 22 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 23 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 24 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 25 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 26 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 27 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 28 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 29 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 30 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 31 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 32 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 33 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 34 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 35 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 36 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 37 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 38 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 39 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 40 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 41 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 42 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 43 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 44 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 45 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 46 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 47 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 48 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 49 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 50 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 51 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 52 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 53 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 54 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 55 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 56 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 57 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 58 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 59 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 60 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 61 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 62 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 63 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 64 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 65 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 66 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 67 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 68 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 69 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 70 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 71 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 72 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 73 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 74 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 75 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 76 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 77 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 78 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 79 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 80 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 81 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 82 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 83 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 84 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 85 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 86 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 87 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 88 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 89 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 90 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 91 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 92 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 93 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 94 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 95 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 96 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 97 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 98 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 99 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 100 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 101 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 102 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 103 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 104 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 105 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 106 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 107 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 108 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 109 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 110 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 111 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 112 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 113 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 114 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 115 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 116 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 117 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 118 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 119 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 120 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 121 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 122 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 123 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 124 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 125 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 126 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 127 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 128 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 129 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 130 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 131 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 132 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 133 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 134 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 135 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 136 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 137 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 138 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 139 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 140 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 141 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 142 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 143 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 144 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 145 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 146 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 147 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 148 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 149 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 150 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 151 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 152 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 153 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 154 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 155 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 156 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 157 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 158 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 159 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 160 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 161 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 162 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 163 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 164 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 165 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 166 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 167 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 168 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 169 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 170 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 171 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 172 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 173 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 174 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
