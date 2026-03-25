# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-03-25.md)

*最后自动更新时间: 2026-03-25 20:13:54*
## 1. Wine 11 重写内核级Linux运行Windows游戏的方式，大幅提升速度

**原文标题**: Wine 11 rewrites how Linux runs Windows games at kernel with massive speed gains

**原文链接**: [https://www.xda-developers.com/wine-11-rewrites-linux-runs-windows-games-speed-gains/](https://www.xda-developers.com/wine-11-rewrites-linux-runs-windows-games-speed-gains/)

Wine 11标志着Linux游戏领域的里程碑式发布，引入了内核级别的增强功能，有望带来显著的速度提升和兼容性改进。其主要亮点是**NTSYNC**，这是一个新的内核驱动程序（已合并到Linux内核6.14中），它重新设计了Wine处理Windows NT同步原语的方式。与esync和fsync等以往的用户空间变通方法不同，NTSYNC提供了原生的内核级同步，消除了瓶颈，并在多线程游戏中带来了显著的性能提升。一些基准测试显示性能提升高达678%，使得以前运行困难的游戏现在变得可玩且表现良好。这惠及所有基于Wine的项目，包括Valve的Proton和SteamOS 3.7.20测试版。

另一个重大成就是**WoW64架构的全面改造完成**。这使得32位Windows应用程序（包括老旧游戏）无需复杂的32位兼容库（multilibs）即可在64位Linux系统上无缝运行，简化了用户体验，甚至支持16位应用程序。

除了这些主要更新，Wine 11还带来了许多其他改进：
*   **Wayland驱动成熟度提升**：增强了剪贴板支持、拖放功能以及对显示模式变化的正确处理。
*   **图形**：将EGL作为默认的OpenGL后端，支持Vulkan 1.4，并初步实现了硬件加速的H.264解码。
*   **硬件支持**：改进了赛车方向盘/飞行摇杆的力反馈功能，并新增了蓝牙驱动程序。
*   **通用修复**：改进了线程优先级管理，ARM64 4K页面模拟，以及针对《仁王2》和《星际争霸2》等游戏的特定兼容性修复。

总而言之，Wine 11被誉为自Proton使Linux游戏成为可能以来最重要的Wine版本，它深刻地提升了整个生态系统的性能和兼容性。

---

## 2. 告别索拉

**原文标题**: Goodbye to Sora

**原文链接**: [https://twitter.com/soraofficialapp/status/2036532795984715896](https://twitter.com/soraofficialapp/status/2036532795984715896)

所提供的文本是来自x.com（前身为Twitter）的一条技术错误消息。它告知用户其浏览器中JavaScript已禁用，从而阻止他们继续使用该平台。该消息指示用户要么启用JavaScript，要么切换到受支持的浏览器，并引导他们前往帮助中心查看兼容选项列表。

在该错误消息下方，内容包含标准网站页脚链接，例如帮助中心、服务条款、隐私政策、Cookie政策、版本说明和广告信息。该页面版权所有为“© 2026 X Corp.”。

尽管标题为“告别Sora”，但实际内容并未讨论Sora、AI模型或任何相关话题。相反，它完全专注于解决访问x.com的浏览器兼容性问题。

---

## 3. 微软对 Windows 11 的“修复”

**原文标题**: Microsoft's "fix" for Windows 11

**原文链接**: [https://www.sambent.com/microsofts-plan-to-fix-windows-11-is-gaslighting/](https://www.sambent.com/microsofts-plan-to-fix-windows-11-is-gaslighting/)

生成摘要时出错

---

## 4. HN 提醒：PyPI 上的 Litellm 1.82.7 和 1.82.8 已被入侵

**原文标题**: Tell HN: Litellm 1.82.7 and 1.82.8 on PyPI are compromised

**原文链接**: [https://github.com/BerriAI/litellm/issues/24512](https://github.com/BerriAI/litellm/issues/24512)

PyPI 包 `litellm` 的 1.82.7 和 1.82.8 版本已被篡改，构成严重的供应链安全威胁。具体来说，`litellm==1.82.8` 包含一个恶意文件 `litellm_init.pth`，它在 Python 解释器启动时自动执行凭据窃取脚本，无需显式 `import litellm`。

这个经过双重 Base64 编码的载荷精心收集了大量敏感数据，包括系统信息、所有环境变量（捕获 API 密钥、秘密信息、令牌）、SSH 密钥、Git 凭据、云服务提供商凭据（AWS、GCP、Azure、Kubernetes）、Docker 配置、各种包管理器和数据库凭据、Shell 历史记录、加密钱包数据、SSL/TLS 私钥以及 CI/CD 秘密信息。

收集到的数据随后使用 AES-256 加密，会话密钥再由硬编码的 RSA 公钥加密。此加密档案随后被窃取并传输至攻击者控制的服务器 `https://models.litellm.cloud/`，该地址与官方 `litellm.ai` 域名不同。

此次事件影响严重，波及所有安装了 `litellm 1.82.8` 的系统，包括本地开发机器、CI/CD 流水线、Docker 容器和生产服务器。用户必须检查其 `site-packages/` 目录中是否存在 `litellm_init.pth`，并立即轮换受影响系统上暴露的*所有*凭据。建议 PyPI 下架受感染版本，并且 BerriAI（维护者）应审计其发布基础设施。

---

## 5. litellm 1.82.8 PyPI 包中的恶意 litellm_init.pth —— 凭据窃取器

**原文标题**: Malicious litellm_init.pth in litellm 1.82.8 PyPI package – credential stealer

**原文链接**: [https://github.com/BerriAI/litellm/issues/24512](https://github.com/BerriAI/litellm/issues/24512)

`litellm` PyPI软件包版本1.82.8包含一个关键的供应链安全漏洞：一个名为`litellm_init.pth`的恶意文件。这个`.pth`文件在Python解释器每次启动时都会自动执行，无需显式调用`import litellm`语句。

隐藏的恶意负载经过两次Base64编码，分两个阶段运行。首先，它从主机系统收集大量敏感数据，包括：
*   系统信息（主机名、IP地址）
*   所有环境变量（捕获API密钥、秘密信息、令牌）
*   SSH密钥
*   Git、AWS、Kubernetes、GCP、Azure和Docker凭据
*   包管理器配置（如`.npmrc`、`.vault-token`等）
*   Shell和数据库历史记录
*   加密钱包文件
*   SSL/TLS私钥
*   CI/CD秘密信息（例如`terraform.tfvars`、`.gitlab-ci.yml`）
*   数据库凭据和Webhook URL

在第二阶段，收集到的数据使用AES-256算法和随机生成的会话密钥进行加密。然后，该会话密钥会使用一个硬编码的4096位RSA公钥进行加密。加密后的数据和密钥被打包成`tpcp.tar.gz`归档文件，并通过POST请求外泄到攻击者控制的服务器`https://models.litellm.cloud/`。值得注意的是，这个数据外泄域名不同于官方的`litellm.ai`。

任何安装了`litellm==1.82.8`的用户都会受到影响，包括本地开发机器、CI/CD管道、Docker容器和生产服务器。强烈建议用户检查其`site-packages/`目录中是否存在`litellm_init.pth`文件，并轮换受影响系统上可能存在的所有凭据。建议PyPI立即移除受损版本，并建议BerriAI审计其发布凭据和CI/CD管道。

---

## 6. 苹果商务

**原文标题**: Apple Business

**原文链接**: [https://www.apple.com/newsroom/2026/03/introducing-apple-business-a-new-all-in-one-platform-for-businesses-of-all-sizes/](https://www.apple.com/newsroom/2026/03/introducing-apple-business-a-new-all-in-one-platform-for-businesses-of-all-sizes/)

苹果今日宣布推出“Apple Business”这一全新一体化平台，将于4月14日在200多个国家和地区上线。该平台统一了为各类规模企业提供的基本服务，旨在简化设备管理、拓展客户覆盖并优化协作。

核心功能包括内置移动设备管理 (MDM)，借助“蓝图”实现轻松设备设置和零接触部署，使IT管理对小型企业也触手可及。它还提供完全集成的商务电子邮件、日历和目录服务，并支持自定义域名，用于专业沟通。

一项重要新增功能是“地图广告”(Ads on Maps)，将于今年夏天在美国和加拿大推出。这将允许企业在Apple地图中投放本地广告，出现在搜索结果和“推荐地点”中，同时秉持苹果隐私优先的原则。

Apple Business整合了品牌和地点管理工具（原为Apple Business Connect），使企业能够管理其在Apple地图、钱包及其他服务中的形象。它支持“管理式Apple ID”、员工管理、应用分发以及Admin API。员工还将拥有一个配套应用程序。

该服务对Apple Business Connect、Business Essentials和Business Manager的现有及新用户免费，这些现有服务将被取代。可选的iCloud存储和AppleCare+ for Business升级服务。

---

## 7. 还有人厌倦谈论人工智能了吗？

**原文标题**: Is anybody else bored of talking about AI?

**原文链接**: [https://blog.jakesaunders.dev/is-anybody-else-bored-of-talking-about-ai/](https://blog.jakesaunders.dev/is-anybody-else-bored-of-talking-about-ai/)

作者对铺天盖地的人工智能讨论感到厌倦，尽管他们个人在工作中从中受益匪浅，在新岗位上大大提高了生产力。他们抱怨Hacker News和Kagi small web等在线技术社区充斥着关于AI工具和工作流程的重复内容，这给人感觉是自我满足，而非真正的创新。

作者认为，这一趋势标志着从“产品工程师”关注交付产品价值的理想，退化为仅仅将AI视为工程领域简单任务的“过度生长的自动补全工具”的痴迷。他们将其比作木匠们总是讨论他们的锤子，而不是他们创造的桌子。

此外，作者批评了管理层目前的介入，指出老板们以前很少关心IDE或框架等实现细节，现在却强制推行“更多使用AI”的举措，并衡量诸如“每位开发者使用的token数”等无用的指标。这会将焦点从更快的部署等面向产出的目标，转移到不相关的流程指标上。

最终，作者呼吁回归讨论工程师们正在“创造的酷东西”以及他们正在“交付的价值”，而非他们使用的工具。他们强调，包括编程在内的任何手艺的核心目的都是创造有价值的东西。作者最后承认了这篇与AI相关的帖子本身的讽刺意味。

---

## 8. 克劳德代码速查表

**原文标题**: Claude Code Cheat Sheet

**原文链接**: [https://cc.storyfox.cz](https://cc.storyfox.cz)

Claude Code is a comprehensive AI coding environment, navigable via extensive keyboard shortcuts for general controls (e.g., Ctrl+C for cancel, Ctrl+G for editor), mode switching (Shift+Tab for permissions, Alt+P for model), and input prefixes (`/` for commands, `!` for bash, `@` for files).

It integrates with MCP Servers (HTTP, stdio, SSE) with layered configuration scopes. A rich set of Slash Commands (`/`) facilitates session management (clear, rename, branch, cost), configuration (model, theme, effort), tool access (init, memory, agents, skills), and special actions like `/plan`, `/voice` for push-to-talk, `/btw` for context-free questions, and `/remote-control` for web sessions.

Memory is managed through `CLAUDE.md` files (project, personal, organizational) that persist across context compaction, and `.claude/rules`. Key workflows include Plan Mode, Git Worktrees for isolated branches, and Voice Mode. Context management is aided by `/compact` and automatic optimization.

Configuration is highly customizable via `settings.json` files and environment variables (`ANTHROPIC_API_KEY`, `CLAUDE_CODE_EFFORT_LEVEL`). It supports extensible Skills and Agents; built-in skills like `/simplify` and `/batch` are complemented by custom skills with frontmatter for detailed control. Agents can operate with specific permission modes, isolation (e.g., worktrees), and persistent memory.

The CLI offers core commands (`claude`, `claude -p "query"`, `claude -c`, `claude update`) and powerful flags for specifying models, worktrees, agents, output formats (including JSON), cost caps, and permission behaviors, enabling flexible interactive and headless operation, including remote web sessions.

---

## 9. Show HN: I took back Video.js after 16 years and we rewrote it to be 88% smaller

**原文标题**: Show HN: I took back Video.js after 16 years and we rewrote it to be 88% smaller

**原文链接**: [https://videojs.org/blog/videojs-v10-beta-hello-world-again](https://videojs.org/blog/videojs-v10-beta-hello-world-again)

生成摘要时出错

---

## 10. Mystery jump in oil trading ahead of Trump post draws scrutiny

**原文标题**: Mystery jump in oil trading ahead of Trump post draws scrutiny

**原文链接**: [https://www.bbc.com/news/articles/cg547ljepvzo](https://www.bbc.com/news/articles/cg547ljepvzo)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 2 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 3 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 4 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 5 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 6 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 7 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 8 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 9 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 10 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 11 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 12 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 13 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 14 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 15 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 16 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 17 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 18 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 19 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 20 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 21 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 22 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 23 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 24 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 25 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 26 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 27 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 28 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 29 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 30 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 31 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 32 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 33 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 34 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 35 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 36 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 37 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 38 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 39 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 40 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 41 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 42 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 43 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 44 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 45 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 46 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 47 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 48 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 49 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 50 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 51 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 52 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 53 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 54 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 55 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 56 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 57 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 58 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 59 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 60 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 61 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 62 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 63 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 64 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 65 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 66 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 67 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 68 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 69 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 70 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 71 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 72 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 73 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 74 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 75 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 76 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 77 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 78 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 79 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 80 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 81 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 82 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 83 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 84 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 85 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 86 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 87 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 88 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 89 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 90 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 91 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 92 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 93 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 94 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 95 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 96 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 97 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 98 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 99 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 100 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 101 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 102 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 103 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 104 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 105 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 106 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 107 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 108 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 109 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 110 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 111 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 112 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 113 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 114 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 115 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 116 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 117 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 118 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 119 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 120 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 121 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 122 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 123 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 124 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 125 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 126 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 127 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 128 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 129 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 130 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 131 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 132 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 133 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 134 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 135 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 136 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 137 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 138 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
