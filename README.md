# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-10-02.md)

*最后自动更新时间: 2026-10-02 23:20:52*
## 1. Pi 1.0

**原文标题**: Pi 1.0

**原文链接**: [https://earendil.com/posts/pi-1-0/](https://earendil.com/posts/pi-1-0/)

Earendil 隆重宣布发布 **Pi 1.0**，这是一个稳定、强化且轻量级的代理平台。Pi 1.0 以其只采用经过验证功能的原则性方法而闻名，是根据广泛的社区反馈而演进的。它继续支持领先的LLM（大型语言模型），并作为日常使用的编码代理，现在正为其代理应用程序增强其“超可塑基底”。

Pi 1.0 的主要新功能包括：
*   **Codemode：** 原生支持MCP和非LLM模型（如Jev和图像模型）。
*   **扩展支持**虚拟模型。
*   **延迟工具加载**。
*   Anthropic模型的**缓存预热**。
*   **会话中系统消息**，用于动态提示/工具更改。
*   默认采用新的TUI主题和全屏模式。

意识到终端之外对更持久、长时间运行的代理应用程序的需求，Earendil 还推出了 **Pi Durable**。这个新的实验性软件包将 Pi 的精简性和超可塑性扩展到新的维度，让开发者能够更灵活地为不同的界面和任务构建和引导智能。

Pi 1.0 和 Pi Durable 即日起均可使用，采用MIT许可证。Pi 1.0 可通过 `curl`（Windows系统为 `powershell`）安装，Pi Durable 则通过 `npm` 安装。文档可在 pi.dev 查阅，代码托管在 GitHub 上。Earendil 的使命是通过软件和开放协议增强人类能动性，而这些发布正是实现这一目标的工具。

---

## 2. StreetComplete iOS 版现已公测

**原文标题**: StreetComplete on iOS is now in public beta

**原文链接**: [https://github.com/streetcomplete/StreetComplete/issues/5421](https://github.com/streetcomplete/StreetComplete/issues/5421)

StreetComplete 正在积极开发和测试一个 iOS 移植版本，并通过一个主工单协调社区贡献。目标是利用其现有的 100% Kotlin 代码库，将该应用带到 iOS 平台。

该技术方案利用 Kotlin Multiplatform (KMP) 实现共享应用逻辑，并使用 Compose Multiplatform 实现统一的用户界面。这种策略与 SwiftUI 或 Flutter 类似，可以最大限度地减少平台特定的代码，并通过维护单一代码库来确保长期维护的效率，这与需要完全重写的替代方案不同。

开发过程包括分离平台特定的代码，并逐步迁移用户界面。这包括将数据访问迁移到 ViewModel，将 Android XML 布局转换为 Android Jetpack Compose，最后移植到 Compose Multiplatform。

目前，迁移工作已完成约 50%，并在 2024 年上半年取得了显著进展。该项目预计需要一年的工作量，严重依赖社区贡献。用户可以通过认领项目看板上的任务、学习 Jetpack Compose/Compose Multiplatform、赞助开发，或协助日常维护和问题分类来提供帮助。

---

## 3. Clef: Open-weight decision models, and new RL fine-tuning platform

**原文标题**: Clef: Open-weight decision models, and new RL fine-tuning platform

**原文链接**: [https://blog.cloudflare.com/clef-decision-models/](https://blog.cloudflare.com/clef-decision-models/)

生成摘要时出错

---

## 4. Git 3.0 即将推行的 SHA-256 默认设置将是一个代价高昂的错误。

**原文标题**: Git 3.0's upcoming SHA-256 default will be a costly mistake

**原文链接**: [https://blog.gitbutler.com/git-3-sha-256](https://blog.gitbutler.com/git-3-sha-256)

所提供的文章，标题为“Git 3.0即将采用SHA-256作为默认哈希算法将是一个代价高昂的错误”，其标题与实际内容严重不符。

尽管标题暗示了对Git 3.0采用SHA-256的批判性讨论，但文章正文却完全偏离了主题。相反，它宣布由Scott Chacon在里斯本主讲的JJ Con 2026大会的所有演讲现已在YouTube上发布。文章承诺对这些演讲进行快速概述，但对于标题中提及的Git 3.0主题却未提供任何进一步的细节。

---

## 5. Linux 内核中已发现多个漏洞。

**原文标题**: Several vulnerabilities have been discovered in the Linux kernel

**原文链接**: [https://lwn.net/Articles/1097401/](https://lwn.net/Articles/1097401/)

Debian 于 2026 年 9 月 29 日发布的安全通告 DSA-6528-1 宣布了 Linux 内核软件包的一项重要安全更新。此更新修复了多达 687 个漏洞，这些漏洞的 CVE ID 编号涵盖 2024 年至 2026 年。

如此大量的 CVE (包括 CVE-2024-52560、CVE-2025-21817 以及 2026 年的数百个漏洞，例如 CVE-2026-23137、CVE-2026-89438、CVE-2026-93037 等等) 表明针对内核中的诸多安全缺陷进行了一项全面的修复工作。尽管此通告摘录中未提供每个漏洞的具体细节，但此更新对于维护运行受影响的 Linux 内核的 Debian 系统的安全性与稳定性至关重要。

---

## 6. 青蛙和蟾蜍和越来越强大的机器

**原文标题**: Frog and Toad and the Increasingly Capable Machines

**原文链接**: [https://www.frogandtoad.ai/](https://www.frogandtoad.ai/)

The provided article content is empty. Therefore, a summary cannot be generated.

---

## 7. Pi Durable

**原文标题**: Pi Durable

**原文链接**: [https://earendil.com/posts/pi-durable/](https://earendil.com/posts/pi-durable/)

生成摘要时出错

---

## 8. Court agrees with EFF: Utah's VPN law demands a technical impossibility

**原文标题**: Court agrees with EFF: Utah's VPN law demands a technical impossibility

**原文链接**: [https://www.eff.org/deeplinks/2026/10/court-agrees-eff-utahs-vpn-law-demands-technical-impossibility](https://www.eff.org/deeplinks/2026/10/court-agrees-eff-utahs-vpn-law-demands-technical-impossibility)

生成摘要时出错

---

## 9. Returning from vacation? The government can search your phone without a warrant

**原文标题**: Returning from vacation? The government can search your phone without a warrant

**原文链接**: [https://arstechnica.com/tech-policy/2026/09/immigration-advocate-sues-border-agents-for-demanding-his-cell-phone/](https://arstechnica.com/tech-policy/2026/09/immigration-advocate-sues-border-agents-for-demanding-his-cell-phone/)

生成摘要时出错

---

## 10. SvelteKit 3

**原文标题**: SvelteKit 3

**原文链接**: [https://svelte.dev/blog/sveltekit-3-is-here](https://svelte.dev/blog/sveltekit-3-is-here)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-10-02](output/hacker_news_summary_2026-10-02.md) |
| 2 | [2026-10-01](output/hacker_news_summary_2026-10-01.md) |
| 3 | [2026-09-29](output/hacker_news_summary_2026-09-29.md) |
| 4 | [2026-09-30](output/hacker_news_summary_2026-09-30.md) |
| 5 | [2026-09-24](output/hacker_news_summary_2026-09-24.md) |
| 6 | [2026-09-21](output/hacker_news_summary_2026-09-21.md) |
| 7 | [2026-09-23](output/hacker_news_summary_2026-09-23.md) |
| 8 | [2026-09-20](output/hacker_news_summary_2026-09-20.md) |
| 9 | [2026-09-27](output/hacker_news_summary_2026-09-27.md) |
| 10 | [2026-09-22](output/hacker_news_summary_2026-09-22.md) |
| 11 | [2026-09-25](output/hacker_news_summary_2026-09-25.md) |
| 12 | [2026-09-16](output/hacker_news_summary_2026-09-16.md) |
| 13 | [2026-09-14](output/hacker_news_summary_2026-09-14.md) |
| 14 | [2026-09-17](output/hacker_news_summary_2026-09-17.md) |
| 15 | [2026-09-19](output/hacker_news_summary_2026-09-19.md) |
| 16 | [2026-09-18](output/hacker_news_summary_2026-09-18.md) |
| 17 | [2026-09-15](output/hacker_news_summary_2026-09-15.md) |
| 18 | [2026-09-09](output/hacker_news_summary_2026-09-09.md) |
| 19 | [2026-09-10](output/hacker_news_summary_2026-09-10.md) |
| 20 | [2026-09-13](output/hacker_news_summary_2026-09-13.md) |
| 21 | [2026-09-08](output/hacker_news_summary_2026-09-08.md) |
| 22 | [2026-09-07](output/hacker_news_summary_2026-09-07.md) |
| 23 | [2026-09-06](output/hacker_news_summary_2026-09-06.md) |
| 24 | [2026-09-11](output/hacker_news_summary_2026-09-11.md) |
| 25 | [2026-09-12](output/hacker_news_summary_2026-09-12.md) |
| 26 | [2026-09-03](output/hacker_news_summary_2026-09-03.md) |
| 27 | [2026-09-02](output/hacker_news_summary_2026-09-02.md) |
| 28 | [2026-08-31](output/hacker_news_summary_2026-08-31.md) |
| 29 | [2026-08-28](output/hacker_news_summary_2026-08-28.md) |
| 30 | [2026-09-04](output/hacker_news_summary_2026-09-04.md) |
| 31 | [2026-09-05](output/hacker_news_summary_2026-09-05.md) |
| 32 | [2026-09-01](output/hacker_news_summary_2026-09-01.md) |
| 33 | [2026-08-29](output/hacker_news_summary_2026-08-29.md) |
| 34 | [2026-08-30](output/hacker_news_summary_2026-08-30.md) |
| 35 | [2026-08-22](output/hacker_news_summary_2026-08-22.md) |
| 36 | [2026-08-25](output/hacker_news_summary_2026-08-25.md) |
| 37 | [2026-08-19](output/hacker_news_summary_2026-08-19.md) |
| 38 | [2026-08-20](output/hacker_news_summary_2026-08-20.md) |
| 39 | [2026-08-17](output/hacker_news_summary_2026-08-17.md) |
| 40 | [2026-08-23](output/hacker_news_summary_2026-08-23.md) |
| 41 | [2026-08-18](output/hacker_news_summary_2026-08-18.md) |
| 42 | [2026-08-21](output/hacker_news_summary_2026-08-21.md) |
| 43 | [2026-08-24](output/hacker_news_summary_2026-08-24.md) |
| 44 | [2026-08-26](output/hacker_news_summary_2026-08-26.md) |
| 45 | [2026-08-12](output/hacker_news_summary_2026-08-12.md) |
| 46 | [2026-08-11](output/hacker_news_summary_2026-08-11.md) |
| 47 | [2026-08-14](output/hacker_news_summary_2026-08-14.md) |
| 48 | [2026-08-16](output/hacker_news_summary_2026-08-16.md) |
| 49 | [2026-08-10](output/hacker_news_summary_2026-08-10.md) |
| 50 | [2026-08-09](output/hacker_news_summary_2026-08-09.md) |
| 51 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 52 | [2026-08-15](output/hacker_news_summary_2026-08-15.md) |
| 53 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 54 | [2026-08-13](output/hacker_news_summary_2026-08-13.md) |
| 55 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 56 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 57 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 58 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 59 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 60 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 61 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 62 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 63 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 64 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 65 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 66 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 67 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 68 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 69 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 70 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 71 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 72 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 73 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 74 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 75 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 76 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 77 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 78 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 79 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 80 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 81 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 82 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 83 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 84 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 85 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 86 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 87 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 88 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 89 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 90 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 91 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 92 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 93 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 94 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 95 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 96 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 97 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 98 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 99 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 100 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 101 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 102 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 103 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 104 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 105 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 106 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 107 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 108 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 109 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 110 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 111 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 112 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 113 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 114 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 115 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 116 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 117 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 118 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 119 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 120 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 121 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 122 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 123 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 124 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 125 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 126 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 127 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 128 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 129 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 130 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 131 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 132 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 133 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 134 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 135 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 136 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 137 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 138 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 139 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 140 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 141 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 142 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 143 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 144 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 145 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 146 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 147 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 148 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 149 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 150 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 151 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 152 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 153 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 154 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 155 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 156 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 157 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 158 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 159 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 160 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 161 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 162 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 163 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 164 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 165 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 166 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 167 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 168 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 169 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 170 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 171 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 172 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 173 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 174 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 175 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 176 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 177 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 178 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 179 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 180 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 181 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 182 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 183 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 184 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 185 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 186 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 187 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 188 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 189 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 190 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 191 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 192 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 193 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 194 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 195 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 196 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 197 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 198 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 199 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 200 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 201 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 202 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 203 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 204 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 205 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 206 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 207 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 208 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 209 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 210 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 211 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 212 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 213 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 214 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 215 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 216 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 217 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 218 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 219 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 220 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 221 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 222 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 223 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 224 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 225 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 226 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 227 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 228 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 229 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 230 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 231 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 232 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 233 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 234 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 235 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 236 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 237 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 238 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 239 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 240 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 241 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 242 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 243 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 244 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 245 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 246 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 247 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 248 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 249 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 250 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 251 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 252 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 253 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 254 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 255 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 256 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 257 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 258 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 259 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 260 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 261 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 262 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 263 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 264 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 265 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 266 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 267 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 268 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 269 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 270 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 271 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 272 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 273 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 274 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 275 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 276 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 277 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 278 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 279 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 280 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 281 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 282 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 283 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 284 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 285 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 286 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 287 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 288 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 289 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 290 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 291 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 292 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 293 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 294 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 295 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 296 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 297 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 298 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 299 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 300 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 301 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 302 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 303 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 304 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 305 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 306 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 307 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 308 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 309 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 310 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 311 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 312 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 313 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 314 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 315 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 316 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 317 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 318 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 319 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 320 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 321 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 322 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 323 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 324 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 325 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
