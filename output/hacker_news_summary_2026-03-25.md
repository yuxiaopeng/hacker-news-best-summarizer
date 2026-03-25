# Hacker News 热门文章摘要 (2026-03-25)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

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

## 11. Flighty Airports

**原文标题**: Flighty Airports

**原文链接**: [https://flighty.com/airports](https://flighty.com/airports)

生成摘要时出错

---

## 12. FCC updates covered list to include foreign-made consumer routers

**原文标题**: FCC updates covered list to include foreign-made consumer routers

**原文链接**: [https://www.fcc.gov/document/fcc-updates-covered-list-include-foreign-made-consumer-routers](https://www.fcc.gov/document/fcc-updates-covered-list-include-foreign-made-consumer-routers)

生成摘要时出错

---

## 13. Epoch confirms GPT5.4 Pro solved a frontier math open problem

**原文标题**: Epoch confirms GPT5.4 Pro solved a frontier math open problem

**原文链接**: [https://epoch.ai/frontiermath/open-problems/ramsey-hypergraphs](https://epoch.ai/frontiermath/open-problems/ramsey-hypergraphs)

生成摘要时出错

---

## 14. So where are all the AI apps?

**原文标题**: So where are all the AI apps?

**原文链接**: [https://www.answer.ai/posts/2026-03-12-so-where-are-all-the-ai-apps.html](https://www.answer.ai/posts/2026-03-12-so-where-are-all-the-ai-apps.html)

生成摘要时出错

---

## 15. TurboQuant: Redefining AI efficiency with extreme compression

**原文标题**: TurboQuant: Redefining AI efficiency with extreme compression

**原文链接**: [https://research.google/blog/turboquant-redefining-ai-efficiency-with-extreme-compression/](https://research.google/blog/turboquant-redefining-ai-efficiency-with-extreme-compression/)

生成摘要时出错

---

## 16. Meta told to pay $375M for misleading users over child safety

**原文标题**: Meta told to pay $375M for misleading users over child safety

**原文链接**: [https://www.bbc.com/news/articles/cql75dn07n2o](https://www.bbc.com/news/articles/cql75dn07n2o)

生成摘要时出错

---

## 17. Show HN: Gemini can now natively embed video, so I built sub-second video search

**原文标题**: Show HN: Gemini can now natively embed video, so I built sub-second video search

**原文链接**: [https://github.com/ssrajadh/sentrysearch](https://github.com/ssrajadh/sentrysearch)

生成摘要时出错

---

## 18. Slovenian officials blame Israeli firm Black Cube for trying to manipulate vote

**原文标题**: Slovenian officials blame Israeli firm Black Cube for trying to manipulate vote

**原文链接**: [https://www.wsj.com/world/europe/spies-lies-and-fake-investors-in-disguise-how-plotters-tried-to-flip-a-european-election-1f42b39a](https://www.wsj.com/world/europe/spies-lies-and-fake-investors-in-disguise-how-plotters-tried-to-flip-a-european-election-1f42b39a)

生成摘要时出错

---

## 19. I wanted to build vertical SaaS for pest control, so I took a technician job

**原文标题**: I wanted to build vertical SaaS for pest control, so I took a technician job

**原文链接**: [https://www.onhand.pro/p/i-wanted-to-build-vertical-saas-for-pest-control-i-took-a-technician-job-instead](https://www.onhand.pro/p/i-wanted-to-build-vertical-saas-for-pest-control-i-took-a-technician-job-instead)

生成摘要时出错

---

## 20. Apple Just Lost Me

**原文标题**: Apple Just Lost Me

**原文链接**: [https://andregarzia.com/2026/03/apple-just-lost-me.html](https://andregarzia.com/2026/03/apple-just-lost-me.html)

生成摘要时出错

---

## 21. Arm AGI CPU

**原文标题**: Arm AGI CPU

**原文链接**: [https://newsroom.arm.com/blog/introducing-arm-agi-cpu](https://newsroom.arm.com/blog/introducing-arm-agi-cpu)

生成摘要时出错

---

## 22. Thoughts on slowing the fuck down

**原文标题**: Thoughts on slowing the fuck down

**原文链接**: [https://mariozechner.at/posts/2026-03-25-thoughts-on-slowing-the-fuck-down/](https://mariozechner.at/posts/2026-03-25-thoughts-on-slowing-the-fuck-down/)

生成摘要时出错

---

## 23. LaGuardia pilots raised safety alarms months before deadly runway crash

**原文标题**: LaGuardia pilots raised safety alarms months before deadly runway crash

**原文链接**: [https://www.theguardian.com/us-news/2026/mar/24/laguardia-airplane-pilots-safety-concerns-crash](https://www.theguardian.com/us-news/2026/mar/24/laguardia-airplane-pilots-safety-concerns-crash)

生成摘要时出错

---

## 24. GitHub is once again down

**原文标题**: GitHub is once again down

**原文链接**: [https://www.githubstatus.com/incidents/kp06czybl7dw](https://www.githubstatus.com/incidents/kp06czybl7dw)

生成摘要时出错

---

## 25. Missile defense is NP-complete

**原文标题**: Missile defense is NP-complete

**原文链接**: [https://smu160.github.io/posts/missile-defense-is-np-complete/](https://smu160.github.io/posts/missile-defense-is-np-complete/)

生成摘要时出错

---

## 26. Ripgrep is faster than grep, ag, git grep, ucg, pt, sift (2016)

**原文标题**: Ripgrep is faster than grep, ag, git grep, ucg, pt, sift (2016)

**原文链接**: [https://burntsushi.net/ripgrep/](https://burntsushi.net/ripgrep/)

生成摘要时出错

---

## 27. Show HN: Email.md – Markdown to responsive, email-safe HTML

**原文标题**: Show HN: Email.md – Markdown to responsive, email-safe HTML

**原文链接**: [https://www.emailmd.dev/](https://www.emailmd.dev/)

生成摘要时出错

---

## 28. Epic Games to cut more than 1k jobs as Fortnite usage falls

**原文标题**: Epic Games to cut more than 1k jobs as Fortnite usage falls

**原文链接**: [https://www.reuters.com/legal/litigation/epic-games-said-tuesday-that-it-will-lay-off-more-than-1000-employees-2026-03-24/](https://www.reuters.com/legal/litigation/epic-games-said-tuesday-that-it-will-lay-off-more-than-1000-employees-2026-03-24/)

生成摘要时出错

---

## 29. Log File Viewer for the Terminal

**原文标题**: Log File Viewer for the Terminal

**原文链接**: [https://lnav.org/](https://lnav.org/)

生成摘要时出错

---

## 30. VitruvianOS – Desktop Linux Inspired by the BeOS

**原文标题**: VitruvianOS – Desktop Linux Inspired by the BeOS

**原文链接**: [https://v-os.dev](https://v-os.dev)

生成摘要时出错

---

## 31. Ensu – Ente’s Local LLM app

**原文标题**: Ensu – Ente’s Local LLM app

**原文链接**: [https://ente.com/blog/ensu/](https://ente.com/blog/ensu/)

生成摘要时出错

---

## 32. Hypothesis, Antithesis, synthesis

**原文标题**: Hypothesis, Antithesis, synthesis

**原文链接**: [https://antithesis.com/blog/2026/hegel/](https://antithesis.com/blog/2026/hegel/)

生成摘要时出错

---

## 33. Windows 3.1 tiled background .bmp archive

**原文标题**: Windows 3.1 tiled background .bmp archive

**原文链接**: [https://github.com/andreasjansson/win-3.1-backgrounds](https://github.com/andreasjansson/win-3.1-backgrounds)

生成摘要时出错

---

## 34. Jury says Meta knowingly harmed children for profit, awarding landmark verdict

**原文标题**: Jury says Meta knowingly harmed children for profit, awarding landmark verdict

**原文链接**: [https://www.latimes.com/business/story/2026-03-25/jury-says-meta-knowingly-harmed-children-for-profit-awarding-landmark-verdict](https://www.latimes.com/business/story/2026-03-25/jury-says-meta-knowingly-harmed-children-for-profit-awarding-landmark-verdict)

生成摘要时出错

---

## 35. How I'm Productive with Claude Code

**原文标题**: How I'm Productive with Claude Code

**原文链接**: [https://neilkakkar.com/productive-with-claude-code.html](https://neilkakkar.com/productive-with-claude-code.html)

生成摘要时出错

---

## 36. The bridge to wealth is being pulled up with AI

**原文标题**: The bridge to wealth is being pulled up with AI

**原文链接**: [https://danielhomola.com/m%20&%20e/ai/your-bridge-to-wealth-is-being-pulled-up/](https://danielhomola.com/m%20&%20e/ai/your-bridge-to-wealth-is-being-pulled-up/)

生成摘要时出错

---

## 37. Data centers are transitioning from AC to DC

**原文标题**: Data centers are transitioning from AC to DC

**原文链接**: [https://spectrum.ieee.org/data-center-dc](https://spectrum.ieee.org/data-center-dc)

生成摘要时出错

---

## 38. Miscellanea: The War in Iran

**原文标题**: Miscellanea: The War in Iran

**原文链接**: [https://acoup.blog/2026/03/25/miscellanea-the-war-in-iran/](https://acoup.blog/2026/03/25/miscellanea-the-war-in-iran/)

生成摘要时出错

---

## 39. No Terms. No Conditions

**原文标题**: No Terms. No Conditions

**原文链接**: [https://notermsnoconditions.com](https://notermsnoconditions.com)

生成摘要时出错

---

## 40. Meta and YouTube Found Negligent in Landmark Social Media Addiction Case

**原文标题**: Meta and YouTube Found Negligent in Landmark Social Media Addiction Case

**原文链接**: [https://www.nytimes.com/2026/03/25/technology/social-media-trial-verdict.html](https://www.nytimes.com/2026/03/25/technology/social-media-trial-verdict.html)

生成摘要时出错

---

## 41. Antimatter has been transported for the first time

**原文标题**: Antimatter has been transported for the first time

**原文链接**: [https://www.nature.com/articles/d41586-026-00950-w](https://www.nature.com/articles/d41586-026-00950-w)

生成摘要时出错

---

## 42. Why I forked httpx

**原文标题**: Why I forked httpx

**原文链接**: [https://tildeweb.nl/~michiel/httpxyz.html](https://tildeweb.nl/~michiel/httpxyz.html)

生成摘要时出错

---

## 43. Nanobrew: The fastest macOS package manager compatible with brew

**原文标题**: Nanobrew: The fastest macOS package manager compatible with brew

**原文链接**: [https://nanobrew.trilok.ai/](https://nanobrew.trilok.ai/)

生成摘要时出错

---

## 44. Hypura – A storage-tier-aware LLM inference scheduler for Apple Silicon

**原文标题**: Hypura – A storage-tier-aware LLM inference scheduler for Apple Silicon

**原文链接**: [https://github.com/t8/hypura](https://github.com/t8/hypura)

生成摘要时出错

---

## 45. Local Stack Archived their GitHub repo and requires an account to run

**原文标题**: Local Stack Archived their GitHub repo and requires an account to run

**原文链接**: [https://github.com/localstack/localstack](https://github.com/localstack/localstack)

生成摘要时出错

---

## 46. Disney Exits OpenAI Deal After AI Giant Shutters Sora

**原文标题**: Disney Exits OpenAI Deal After AI Giant Shutters Sora

**原文链接**: [https://www.hollywoodreporter.com/business/digital/openai-shutting-down-sora-ai-video-app-1236546187/](https://www.hollywoodreporter.com/business/digital/openai-shutting-down-sora-ai-video-app-1236546187/)

生成摘要时出错

---

## 47. Debunking Zswap and Zram Myths

**原文标题**: Debunking Zswap and Zram Myths

**原文链接**: [https://chrisdown.name/2026/03/24/zswap-vs-zram-when-to-use-what.html](https://chrisdown.name/2026/03/24/zswap-vs-zram-when-to-use-what.html)

生成摘要时出错

---

## 48. Jury finds Meta liable in case over child sexual exploitation on its platforms

**原文标题**: Jury finds Meta liable in case over child sexual exploitation on its platforms

**原文链接**: [https://www.cnn.com/2026/03/24/tech/meta-new-mexico-trial-jury-deliberation](https://www.cnn.com/2026/03/24/tech/meta-new-mexico-trial-jury-deliberation)

生成摘要时出错

---

## 49. Bets on US-Iran ceasefire show signs of insider knowledge, say experts

**原文标题**: Bets on US-Iran ceasefire show signs of insider knowledge, say experts

**原文链接**: [https://www.theguardian.com/us-news/2026/mar/23/bets-us-iran-ceasefire-show-signs-of-insider-knowledge-say-experts-polymarket](https://www.theguardian.com/us-news/2026/mar/23/bets-us-iran-ceasefire-show-signs-of-insider-knowledge-say-experts-polymarket)

生成摘要时出错

---

## 50. Opera: Rewind The Web to 1996 (Opera at 30)

**原文标题**: Opera: Rewind The Web to 1996 (Opera at 30)

**原文链接**: [https://www.web-rewind.com](https://www.web-rewind.com)

生成摘要时出错

---

## 51. Supreme Court Sides with Cox in Copyright Fight over Pirated Music

**原文标题**: Supreme Court Sides with Cox in Copyright Fight over Pirated Music

**原文链接**: [https://www.nytimes.com/2026/03/25/us/politics/supreme-court-cox-music-copyright.html](https://www.nytimes.com/2026/03/25/us/politics/supreme-court-cox-music-copyright.html)

生成摘要时出错

---

## 52. The AI Industry Is Lying to You

**原文标题**: The AI Industry Is Lying to You

**原文链接**: [https://www.wheresyoured.at/the-ai-industry-is-lying-to-you/](https://www.wheresyoured.at/the-ai-industry-is-lying-to-you/)

生成摘要时出错

---

## 53. Regular army and reserve components enlistment program: Summary of change

**原文标题**: Regular army and reserve components enlistment program: Summary of change

**原文链接**: [https://armypubs.army.mil/epubs/DR_pubs/DR_a/ARN42922-AR_601-210-000-WEB-1.pdf](https://armypubs.army.mil/epubs/DR_pubs/DR_a/ARN42922-AR_601-210-000-WEB-1.pdf)

生成摘要时出错

---

## 54. curl > /dev/sda: How I made a Linux distro that runs wget | dd

**原文标题**: curl > /dev/sda: How I made a Linux distro that runs wget | dd

**原文链接**: [https://astrid.tech/2026/03/24/0/curl-to-dev-sda/](https://astrid.tech/2026/03/24/0/curl-to-dev-sda/)

生成摘要时出错

---

## 55. Country that put backdoors in Cisco routers to spy on world bans foreign routers

**原文标题**: Country that put backdoors in Cisco routers to spy on world bans foreign routers

**原文链接**: [https://www.theregister.com/2026/03/24/fcc_foreign_routers/](https://www.theregister.com/2026/03/24/fcc_foreign_routers/)

生成摘要时出错

---

## 56. Show HN: ProofShot – Give AI coding agents eyes to verify the UI they build

**原文标题**: Show HN: ProofShot – Give AI coding agents eyes to verify the UI they build

**原文链接**: [https://github.com/AmElmo/proofshot](https://github.com/AmElmo/proofshot)

生成摘要时出错

---

## 57. A retro terminal music player inspired by Winamp

**原文标题**: A retro terminal music player inspired by Winamp

**原文链接**: [https://github.com/bjarneo/cliamp](https://github.com/bjarneo/cliamp)

生成摘要时出错

---

## 58. LLM Neuroanatomy II: Modern LLM Hacking and Hints of a Universal Language?

**原文标题**: LLM Neuroanatomy II: Modern LLM Hacking and Hints of a Universal Language?

**原文链接**: [https://dnhkng.github.io/posts/rys-ii/](https://dnhkng.github.io/posts/rys-ii/)

生成摘要时出错

---

## 59. I tried to prove I'm not AI. My aunt wasn't convinced

**原文标题**: I tried to prove I'm not AI. My aunt wasn't convinced

**原文链接**: [https://www.bbc.com/future/article/20260324-i-tried-to-prove-im-not-an-ai-deepfake](https://www.bbc.com/future/article/20260324-i-tried-to-prove-im-not-an-ai-deepfake)

生成摘要时出错

---

## 60. US expected to send thousands more soldiers to Middle East, sources say

**原文标题**: US expected to send thousands more soldiers to Middle East, sources say

**原文链接**: [https://www.reuters.com/world/middle-east/us-expected-send-thousands-soldiers-middle-east-sources-say-2026-03-24/](https://www.reuters.com/world/middle-east/us-expected-send-thousands-soldiers-middle-east-sources-say-2026-03-24/)

生成摘要时出错

---

## 61. Sony V. Cox Decision Reversed

**原文标题**: Sony V. Cox Decision Reversed

**原文链接**: [https://supreme.justia.com/cases/federal/us/607/24-171/](https://supreme.justia.com/cases/federal/us/607/24-171/)

生成摘要时出错

---

## 62. A Compiler Writing Journey

**原文标题**: A Compiler Writing Journey

**原文链接**: [https://github.com/DoctorWkt/acwj](https://github.com/DoctorWkt/acwj)

生成摘要时出错

---

## 63. The Resolv hack: How one compromised key printed $23M

**原文标题**: The Resolv hack: How one compromised key printed $23M

**原文链接**: [https://www.chainalysis.com/blog/lessons-from-the-resolv-hack/](https://www.chainalysis.com/blog/lessons-from-the-resolv-hack/)

生成摘要时出错

---

## 64. American aviation is near collapse?

**原文标题**: American aviation is near collapse?

**原文链接**: [https://www.theatlantic.com/newsletters/2026/03/aviation-failures-tsa-dhs-shutdown/686505/](https://www.theatlantic.com/newsletters/2026/03/aviation-failures-tsa-dhs-shutdown/686505/)

生成摘要时出错

---

## 65. NanoClaw Adopts OneCLI Agent Vault

**原文标题**: NanoClaw Adopts OneCLI Agent Vault

**原文链接**: [https://nanoclaw.dev/blog/nanoclaw-agent-vault/](https://nanoclaw.dev/blog/nanoclaw-agent-vault/)

生成摘要时出错

---

## 66. IRIX 3dfx Voodoo driver and glide2x IRIX port

**原文标题**: IRIX 3dfx Voodoo driver and glide2x IRIX port

**原文链接**: [https://sdz-mods.com/index.php/2026/03/23/irix-3dfx-voodoo-driver-glide2x-irix-port/](https://sdz-mods.com/index.php/2026/03/23/irix-3dfx-voodoo-driver-glide2x-irix-port/)

生成摘要时出错

---

## 67. ARM AGI CPU: Specs and SKUs

**原文标题**: ARM AGI CPU: Specs and SKUs

**原文链接**: [https://sbcwiki.com/docs/soc-manufacturers/arm/arm-silicon/](https://sbcwiki.com/docs/soc-manufacturers/arm/arm-silicon/)

生成摘要时出错

---

## 68. Tracy Kidder has died

**原文标题**: Tracy Kidder has died

**原文链接**: [https://www.nytimes.com/2026/03/25/books/tracy-kidder-dead.html](https://www.nytimes.com/2026/03/25/books/tracy-kidder-dead.html)

生成摘要时出错

---

## 69. A Eulogy for Vim

**原文标题**: A Eulogy for Vim

**原文链接**: [https://drewdevault.com/2026/03/25/2026-03-25-Forking-vim.html](https://drewdevault.com/2026/03/25/2026-03-25-Forking-vim.html)

生成摘要时出错

---

## 70. FCC has banned the import of all new foreign-made routers here's what you can do

**原文标题**: FCC has banned the import of all new foreign-made routers here's what you can do

**原文链接**: [https://blog.adafruit.com/2026/03/24/fcc-just-banned-the-import-of-all-new-foreign-made-routers-heres-what-you-can-do-about-it/](https://blog.adafruit.com/2026/03/24/fcc-just-banned-the-import-of-all-new-foreign-made-routers-heres-what-you-can-do-about-it/)

生成摘要时出错

---

## 71. March, 19-21: God is a comedian

**原文标题**: March, 19-21: God is a comedian

**原文链接**: [https://no01.substack.com/p/march-19-21-god-is-a-comedian](https://no01.substack.com/p/march-19-21-god-is-a-comedian)

生成摘要时出错

---

## 72. Secure Domain Name System (DNS) Deployment 2026 Guide [pdf]

**原文标题**: Secure Domain Name System (DNS) Deployment 2026 Guide [pdf]

**原文链接**: [https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-81r3.pdf](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-81r3.pdf)

生成摘要时出错

---

## 73. WolfGuard: WireGuard with FIPS 140-3 cryptography

**原文标题**: WolfGuard: WireGuard with FIPS 140-3 cryptography

**原文链接**: [https://github.com/wolfssl/wolfguard](https://github.com/wolfssl/wolfguard)

生成摘要时出错

---

## 74. Meta and Google found liable in social media addiction trial

**原文标题**: Meta and Google found liable in social media addiction trial

**原文链接**: [https://www.bbc.co.uk/news/articles/c747x7gz249o](https://www.bbc.co.uk/news/articles/c747x7gz249o)

生成摘要时出错

---

## 75. Show HN: Gridland: make terminal apps that also run in the browser

**原文标题**: Show HN: Gridland: make terminal apps that also run in the browser

**原文链接**: [https://www.gridland.io/](https://www.gridland.io/)

生成摘要时出错

---

## 76. Show HN: AI Roundtable – Let 200 models debate your question

**原文标题**: Show HN: AI Roundtable – Let 200 models debate your question

**原文链接**: [https://opper.ai/ai-roundtable/](https://opper.ai/ai-roundtable/)

生成摘要时出错

---

## 77. Pentagon Adopts New Limits for Journalists After Court Loss

**原文标题**: Pentagon Adopts New Limits for Journalists After Court Loss

**原文链接**: [https://www.nytimes.com/2026/03/23/business/media/pentagon-closes-journalists-work-area.html](https://www.nytimes.com/2026/03/23/business/media/pentagon-closes-journalists-work-area.html)

生成摘要时出错

---

## 78. I created my first AI-assisted pull request

**原文标题**: I created my first AI-assisted pull request

**原文链接**: [https://nelson.cloud/i-created-my-first-ai-assisted-pull-request-and-i-feel-like-a-fraud/](https://nelson.cloud/i-created-my-first-ai-assisted-pull-request-and-i-feel-like-a-fraud/)

生成摘要时出错

---

## 79. Quantization from the Ground Up

**原文标题**: Quantization from the Ground Up

**原文链接**: [https://ngrok.com/blog/quantization](https://ngrok.com/blog/quantization)

生成摘要时出错

---

## 80. Show HN: DuckDB community extension for prefiltered HNSW using ACORN-1

**原文标题**: Show HN: DuckDB community extension for prefiltered HNSW using ACORN-1

**原文链接**: [https://github.com/cigrainger/duckdb-hnsw-acorn](https://github.com/cigrainger/duckdb-hnsw-acorn)

生成摘要时出错

---

## 81. Microsoft blocks trick to unlock native NVMe driver, but workarounds still exist

**原文标题**: Microsoft blocks trick to unlock native NVMe driver, but workarounds still exist

**原文链接**: [https://www.tomshardware.com/software/windows/microsoft-blocks-the-registry-hack-trick-that-unlocked-native-nvme-performance-on-windows-11](https://www.tomshardware.com/software/windows/microsoft-blocks-the-registry-hack-trick-that-unlocked-native-nvme-performance-on-windows-11)

生成摘要时出错

---

## 82. How to Keep ICE Agents Out of Your Devices at Airports

**原文标题**: How to Keep ICE Agents Out of Your Devices at Airports

**原文链接**: [https://theintercept.com/2026/03/25/ice-airports-phone-security-privacy-safety/](https://theintercept.com/2026/03/25/ice-airports-phone-security-privacy-safety/)

生成摘要时出错

---

## 83. Oil at $150 will trigger global recession, says boss of financial BlackRock

**原文标题**: Oil at $150 will trigger global recession, says boss of financial BlackRock

**原文链接**: [https://www.bbc.com/news/articles/c9wqrdkx8ppo](https://www.bbc.com/news/articles/c9wqrdkx8ppo)

生成摘要时出错

---

## 84. Welcome to FastMCP

**原文标题**: Welcome to FastMCP

**原文链接**: [https://gofastmcp.com/getting-started/welcome](https://gofastmcp.com/getting-started/welcome)

生成摘要时出错

---

## 85. Young Graduates Face the Grimmest Job Market in Years

**原文标题**: Young Graduates Face the Grimmest Job Market in Years

**原文链接**: [https://www.nytimes.com/2026/03/24/business/economy/college-graduates-job-market-hiring.html](https://www.nytimes.com/2026/03/24/business/economy/college-graduates-job-market-hiring.html)

生成摘要时出错

---

## 86. Meta ordered to pay $375M in New Mexico trial over child exploitation

**原文标题**: Meta ordered to pay $375M in New Mexico trial over child exploitation

**原文链接**: [https://www.reuters.com/sustainability/boards-policy-regulation/jury-orders-meta-pay-375-mln-new-mexico-lawsuit-over-child-sexual-exploitation-2026-03-24/](https://www.reuters.com/sustainability/boards-policy-regulation/jury-orders-meta-pay-375-mln-new-mexico-lawsuit-over-child-sexual-exploitation-2026-03-24/)

生成摘要时出错

---

## 87. Chat GPT 5.2 cannot explain the German word "geschniegelt"

**原文标题**: Chat GPT 5.2 cannot explain the German word "geschniegelt"

**原文链接**: [https://old.reddit.com/r/ChatGPT/comments/1r4goxh/chat_gpt_52_cannot_explain_the_word_geschniegelt/](https://old.reddit.com/r/ChatGPT/comments/1r4goxh/chat_gpt_52_cannot_explain_the_word_geschniegelt/)

生成摘要时出错

---

## 88. Sunsetting the Techempower Framework Benchmarks

**原文标题**: Sunsetting the Techempower Framework Benchmarks

**原文链接**: [https://github.com/TechEmpower/FrameworkBenchmarks/issues/10932](https://github.com/TechEmpower/FrameworkBenchmarks/issues/10932)

生成摘要时出错

---

## 89. Musketeer d'Artagnan's remains believed found under Dutch church

**原文标题**: Musketeer d'Artagnan's remains believed found under Dutch church

**原文链接**: [https://www.bbc.co.uk/news/articles/cm2rew2dgzzo](https://www.bbc.co.uk/news/articles/cm2rew2dgzzo)

生成摘要时出错

---

## 90. The Treasury just declared the U.S. insolvent

**原文标题**: The Treasury just declared the U.S. insolvent

**原文链接**: [https://fortune.com/2026/03/23/us-government-insolvent-fiscal-crisis-fix/](https://fortune.com/2026/03/23/us-government-insolvent-fiscal-crisis-fix/)

生成摘要时出错

---

## 91. USA bans all new routers for consumers

**原文标题**: USA bans all new routers for consumers

**原文链接**: [https://www.heise.de/en/news/USA-bans-all-new-routers-for-consumers-11222049.html](https://www.heise.de/en/news/USA-bans-all-new-routers-for-consumers-11222049.html)

生成摘要时出错

---

## 92. Minutes before Trump's announcement, $800M in trades made on oil prices

**原文标题**: Minutes before Trump's announcement, $800M in trades made on oil prices

**原文链接**: [https://www.9news.com.au/world/donald-trump-iran-updates-oil-futures-trade-suspicious-betting-activity-usa-world-news/1061ef6b-5fef-401c-b469-98016ccdb9c3](https://www.9news.com.au/world/donald-trump-iran-updates-oil-futures-trade-suspicious-betting-activity-usa-world-news/1061ef6b-5fef-401c-b469-98016ccdb9c3)

生成摘要时出错

---

## 93. Today's Layoffs

**原文标题**: Today's Layoffs

**原文链接**: [https://www.epicgames.com/site/en-US/news/todays-layoffs](https://www.epicgames.com/site/en-US/news/todays-layoffs)

生成摘要时出错

---

## 94. io_uring, libaio performance across Linux kernels and an unexpected IOMMU trap

**原文标题**: io_uring, libaio performance across Linux kernels and an unexpected IOMMU trap

**原文链接**: [https://blog.ydb.tech/how-io-uring-overtook-libaio-performance-across-linux-kernels-and-an-unexpected-iommu-trap-ea6126d9ef14](https://blog.ydb.tech/how-io-uring-overtook-libaio-performance-across-linux-kernels-and-an-unexpected-iommu-trap-ea6126d9ef14)

生成摘要时出错

---

## 95. Krita 5.3.0 and 6.0.0 Released

**原文标题**: Krita 5.3.0 and 6.0.0 Released

**原文链接**: [https://krita.org/en/posts/2026/krita-5.3.0-released/](https://krita.org/en/posts/2026/krita-5.3.0-released/)

生成摘要时出错

---

## 96. Open source isn't a tip jar – it's time to charge for access

**原文标题**: Open source isn't a tip jar – it's time to charge for access

**原文链接**: [https://www.theregister.com/2026/03/25/open_source_bill_opinion/](https://www.theregister.com/2026/03/25/open_source_bill_opinion/)

生成摘要时出错

---

## 97. Epic Games lays off over 1k employees

**原文标题**: Epic Games lays off over 1k employees

**原文链接**: [https://www.gamesindustry.biz/epic-games-lays-off-over-1000-employees-following-downturn-in-fortnite-engagement](https://www.gamesindustry.biz/epic-games-lays-off-over-1000-employees-following-downturn-in-fortnite-engagement)

生成摘要时出错

---

## 98. Firefox introduces Split View: Two tabs side by side, right where you need them

**原文标题**: Firefox introduces Split View: Two tabs side by side, right where you need them

**原文链接**: [https://blog.mozilla.org/en/firefox/split-view/](https://blog.mozilla.org/en/firefox/split-view/)

生成摘要时出错

---

## 99. AI boom risks widening wealth divide, says BlackRock's Larry Fink

**原文标题**: AI boom risks widening wealth divide, says BlackRock's Larry Fink

**原文链接**: [https://www.theguardian.com/technology/2026/mar/23/ai-boom-risks-widening-wealth-divide-blackrock-larry-fink](https://www.theguardian.com/technology/2026/mar/23/ai-boom-risks-widening-wealth-divide-blackrock-larry-fink)

生成摘要时出错

---

## 100. OpenAI's latest repo has Claude as the third top contributor

**原文标题**: OpenAI's latest repo has Claude as the third top contributor

**原文链接**: [https://twitter.com/CodeByNZ/status/2036723050197012771](https://twitter.com/CodeByNZ/status/2036723050197012771)

生成摘要时出错

---

