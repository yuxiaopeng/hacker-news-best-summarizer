# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-04-01.md)

*最后自动更新时间: 2026-04-01 20:19:36*
## 1. Claude Code 的源代码已通过其 NPM 注册表中的一个映射文件泄露。

**原文标题**: Claude Code's source code has been leaked via a map file in their NPM registry

**原文链接**: [https://twitter.com/Fried_rice/status/2038894956459290963](https://twitter.com/Fried_rice/status/2038894956459290963)

文章标题宣布了一项重大事件：据称Claude Code的源代码通过其NPM注册表中的一个map文件泄露。

然而，文章所提供的内容并未讨论或证实这次泄露。相反，文章正文仅包含一条来自x.com（原Twitter）的通用消息，指出用户浏览器中的JavaScript已被禁用。该消息提示用户启用JavaScript或切换到受支持的浏览器以继续使用该平台，并包含指向帮助、服务条款、隐私政策的链接以及一份2026年的版权声明。

因此，该文章未能提供任何关于其标题中提及的所谓源代码泄露的信息、细节或证实。

---

## 2. Axios 在 NPM 上被攻陷——恶意版本植入远程访问木马

**原文标题**: Axios compromised on NPM – Malicious versions drop remote access trojan

**原文链接**: [https://www.stepsecurity.io/blog/axios-compromised-on-npm-malicious-versions-drop-remote-access-trojan](https://www.stepsecurity.io/blog/axios-compromised-on-npm-malicious-versions-drop-remote-access-trojan)

On March 30, 2026, the popular JavaScript HTTP client library Axios was hit by a sophisticated supply chain attack on NPM, leading to the publication of malicious versions `axios@1.14.1` and `axios@0.30.4`. StepSecurity identified the compromise, which stemmed from a hijacked maintainer account (`jasonsaayman`).

The attacker injected a hidden dependency, `plain-crypto-js@4.2.1`, into the compromised Axios releases. This dependency, pre-staged 18 hours prior, masqueraded as `crypto-js` but included a `postinstall` script designed to deploy a cross-platform Remote Access Trojan (RAT). Upon installation, the RAT dropper connected to a command-and-control server (`sfrclak.com:8000`) to deliver OS-specific payloads for macOS, Windows, and Linux. To evade detection, the malware then self-destructed, replacing its `package.json` with a clean decoy (`4.2.0`) and deleting its files.

This highly precise attack involved `plain-crypto-js` never being imported into the Axios source, existing solely to trigger the postinstall hook. A key indicator of compromise is the absence of NPM's OIDC Trusted Publisher binding on the malicious Axios releases, unlike legitimate versions, suggesting a stolen long-lived NPM access token. The only actual change in the compromised Axios packages was the version bump and the addition of `plain-crypto-js` in `package.json`.

Users who installed `axios@1.14.1` or `axios@0.30.4` should assume their systems are compromised. The presence of `plain-crypto-js` in `node_modules` is a high-confidence indicator.

---

## 3. 克劳德源代码泄露：假工具、令人抓狂的正则表达式、卧底模式

**原文标题**: The Claude Code Source Leak: fake tools, frustration regexes, undercover mode

**原文链接**: [https://alex000kim.com/posts/2026-03-31-claude-code-source-leak/](https://alex000kim.com/posts/2026-03-31-claude-code-source-leak/)

生成摘要时出错

---

## 4. 克劳德代码拆解：可视化指南

**原文标题**: Claude Code Unpacked : A visual guide

**原文链接**: [https://ccunpacked.dev/](https://ccunpacked.dev/)

Claude 代码揭秘：可视化指南”深入探讨了 Claude 代码的内部运作，详细阐述了其架构、流程和功能。

该指南首先阐述了**代理循环（The Agent Loop）**，概述了从用户按键到渲染响应的逐步过程，涉及输入、消息处理、历史记录、系统交互、API 调用、令牌管理、工具调用和渲染。

接着介绍了**架构探索器（Architecture Explorer）**，将其庞大的代码库分为工具与命令、核心处理、UI 层、基础设施和支持等领域，突出显示了数千个文件和代码行。

详细介绍了**工具系统（Tool System）**，展示了50多种内置工具，涵盖文件操作（如ReadFile、EditFile）、执行（Bash、PowerShell）、搜索与获取（WebBrowser、WebSearch）、代理与任务（TaskCreate、SendMessage）、规划（EnterPlanMode）、系统（AskUserQuestion）以及众多实验性工具等类别。

**命令目录（Command Catalog）**列出了90多个可用的斜杠命令，分为设置与配置、日常工作流程、代码审查与Git、调试与诊断以及高级与实验性等类别，支持从/login和/memory到/review和/debug-tool-call等多种功能。

最后，**隐藏功能（Hidden Features）**揭示了代码中存在但尚未发布的功能。这些功能包括“Buddy”（虚拟宠物）、“Kairos”（具有自主后台操作的持久模式）、“UltraPlan”（长时间规划会话）、“Coordinator Mode”（多代理编排）、“Bridge”（远程控制）、“Daemon Mode”（后台会话）、“UDS Inbox”（会话间通信）和“Auto-Dream”（会话间的AI审查与学习）。

---

## 5. 甲骨文裁员3万人

**原文标题**: Oracle slashes 30k jobs

**原文链接**: [https://rollingout.com/2026/03/31/oracle-slashes-30000-jobs-with-a-cold-6/](https://rollingout.com/2026/03/31/oracle-slashes-30000-jobs-with-a-cold-6/)

The provided title, "Oracle slashes 30k jobs," indicates a major workforce reduction at Oracle.

However, the accompanying content *only* details job cuts at Morgan Stanley. According to the text, Morgan Stanley is cutting 2,500 jobs across three divisions, as reported by the WSJ.

There is no information within the given content about Oracle or any 30,000 job cuts. Therefore, based solely on the provided content, the article reports on Morgan Stanley's job reductions, not Oracle's.

---

## 6. Artemis II is not safe to fly

**原文标题**: Artemis II is not safe to fly

**原文链接**: [https://idlewords.com/2026/03/artemis_ii_is_not_safe_to_fly.htm](https://idlewords.com/2026/03/artemis_ii_is_not_safe_to_fly.htm)

生成摘要时出错

---

## 7. Ollama 现已搭载 MLX，支持 Apple 芯片（预览版）

**原文标题**: Ollama is now powered by MLX on Apple Silicon in preview

**原文链接**: [https://ollama.com/blog/mlx](https://ollama.com/blog/mlx)

Ollama 发布了 0.19 版本的预览版，现在它在 Apple Silicon 设备上由 Apple 的 MLX 框架提供支持，使其成为在这些设备上运行 Ollama 最快的方式。此次集成利用了 Apple Silicon 的统一内存架构和 M5 GPU 神经网络加速器，显著提升了首个 token 生成时间 (TTFT) 和生成速度。性能基准测试显示，Ollama 0.19 使用 Qwen3.5-35B-A3B 模型，在预填充 (prefill) 方面达到 1810 tokens/秒，解码 (decode) 方面达到 112 tokens/秒，相较于 0.18 版本有了显著提升。

此次更新引入了对 NVIDIA NVFP4 格式的支持，在保持模型精度的同时，降低了内存需求，并确保与专业推理提供商达到生产级一致。此外，Ollama 的缓存机制也得到了显著升级，通过在不同对话中复用缓存降低了内存占用，通过智能检查点实现更快响应，并采用了更智能的淘汰策略。

这些增强功能加速了高需求任务，特别是像 OpenClaw 这样的个人助理和 Claude Code 等编码代理。用户需要配备超过 32GB 统一内存的 Mac 才能使用此预览版本。Ollama 计划未来扩展对更多模型的支持，并简化自定义模型的导入。

---

## 8. GitHub 退让，在强烈反弹后取消 Copilot 拉取请求广告

**原文标题**: GitHub backs down, kills Copilot pull-request ads after backlash

**原文链接**: [https://www.theregister.com/2026/03/30/github_copilot_ads_pull_requests/](https://www.theregister.com/2026/03/30/github_copilot_ads_pull_requests/)

GitHub的AI助手Copilot开始直接向拉取请求（PR）中插入未经请求的“提示”，许多开发者将其视为广告，此举引发了强烈的反弹。

澳大利亚开发者Zach Manson率先指出了这个问题。在Copilot被用于简单的错别字修正后，他在同事的PR中发现了一个针对生产力应用Raycast的推广信息。Manson认为这“令人反感”，因为Copilot在他不知情的情况下，更改了他未编写的PR内容。调查显示，GitHub上存在超过11,400个类似案例。

GitHub开发者关系副总裁Martin Woodward解释说，尽管Copilot此前会在其生成的PR中添加提示，但将此行为扩展到任何提及它的PR中是新的且有问题的。Copilot首席产品经理Tim Rogers承认这是一个“错误的判断”，最初的目的是帮助开发者发现新的工作流程。

为迅速回应广泛的批评，GitHub宣布已从所有由Copilot创建或涉及的拉取请求中禁用了这些“提示”，并承诺它们不会再次出现。Woodward后来澄清，该事件是由于一个“编程逻辑问题”，导致一个代理提示在不正确的上下文中出现，他强调GitHub无意包含广告。

---

## 9. Microsoft: Copilot is for entertainment purposes only

**原文标题**: Microsoft: Copilot is for entertainment purposes only

**原文链接**: [https://www.microsoft.com/en-us/microsoft-copilot/for-individuals/termsofuse](https://www.microsoft.com/en-us/microsoft-copilot/for-individuals/termsofuse)

生成摘要时出错

---

## 10. 每天一点，杂乱不来

**原文标题**: A dot a day keeps the clutter away

**原文链接**: [https://scottlawsonbc.com/post/dot-system](https://scottlawsonbc.com/post/dot-system)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 2 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 3 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 4 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 5 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 6 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 7 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 8 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 9 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 10 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 11 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 12 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 13 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 14 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 15 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 16 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 17 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 18 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 19 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 20 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 21 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 22 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 23 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 24 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 25 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 26 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 27 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 28 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 29 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 30 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 31 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 32 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 33 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 34 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 35 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 36 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 37 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 38 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 39 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 40 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 41 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 42 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 43 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 44 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 45 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 46 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 47 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 48 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 49 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 50 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 51 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 52 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 53 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 54 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 55 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 56 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 57 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 58 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 59 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 60 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 61 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 62 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 63 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 64 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 65 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 66 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 67 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 68 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 69 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 70 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 71 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 72 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 73 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 74 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 75 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 76 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 77 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 78 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 79 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 80 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 81 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 82 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 83 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 84 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 85 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 86 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 87 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 88 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 89 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 90 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 91 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 92 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 93 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 94 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 95 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 96 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 97 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 98 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 99 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 100 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 101 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 102 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 103 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 104 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 105 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 106 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 107 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 108 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 109 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 110 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 111 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 112 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 113 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 114 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 115 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 116 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 117 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 118 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 119 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 120 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 121 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 122 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 123 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 124 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 125 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 126 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 127 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 128 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 129 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 130 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 131 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 132 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 133 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 134 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 135 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 136 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 137 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 138 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 139 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 140 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 141 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 142 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 143 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 144 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 145 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
