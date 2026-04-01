# Hacker News 热门文章摘要 (2026-04-01)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

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

## 11. OpenAI closes funding round at an $852B valuation

**原文标题**: OpenAI closes funding round at an $852B valuation

**原文链接**: [https://www.cnbc.com/2026/03/31/openai-funding-round-ipo.html](https://www.cnbc.com/2026/03/31/openai-funding-round-ipo.html)

生成摘要时出错

---

## 12. GitHub's Historic Uptime

**原文标题**: GitHub's Historic Uptime

**原文链接**: [https://damrnelson.github.io/github-historical-uptime/](https://damrnelson.github.io/github-historical-uptime/)

生成摘要时出错

---

## 13. Universal Claude.md – cut Claude output tokens

**原文标题**: Universal Claude.md – cut Claude output tokens

**原文链接**: [https://github.com/drona23/claude-token-efficient](https://github.com/drona23/claude-token-efficient)

生成摘要时出错

---

## 14. OkCupid gave 3M dating-app photos to facial recognition firm, FTC says

**原文标题**: OkCupid gave 3M dating-app photos to facial recognition firm, FTC says

**原文链接**: [https://arstechnica.com/tech-policy/2026/03/okcupid-match-pay-no-fine-for-sharing-user-photos-with-facial-recognition-firm/](https://arstechnica.com/tech-policy/2026/03/okcupid-match-pay-no-fine-for-sharing-user-photos-with-facial-recognition-firm/)

生成摘要时出错

---

## 15. Why the US Navy won't blast the Iranians and 'open' Strait of Hormuz

**原文标题**: Why the US Navy won't blast the Iranians and 'open' Strait of Hormuz

**原文链接**: [https://responsiblestatecraft.org/iran-strait-of-hormuz/](https://responsiblestatecraft.org/iran-strait-of-hormuz/)

生成摘要时出错

---

## 16. 1美元硬件，MacBook秒变触摸屏 (2018)

**原文标题**: Turning a MacBook into a touchscreen with $1 of hardware (2018)

**原文链接**: [https://anishathalye.com/macbook-touchscreen/](https://anishathalye.com/macbook-touchscreen/)

Project Sistine is a proof-of-concept that transforms a MacBook into a touchscreen using only $1 of hardware and computer vision, prototyped in 16 hours by Kevin, Guillermo, Logan, and the author.

The core principle involves positioning a small mirror in front of the MacBook's built-in webcam. This allows the webcam to view the screen at a sharp angle, detecting fingers by observing their reflection on the surface. This idea evolved from an earlier project called ShinyTouch. The hardware setup is simple, requiring a small mirror, a rigid paper plate, a door hinge, and hot glue to secure the mirror at the appropriate angle.

The software processes video frames to detect and interpret touch. Finger detection involves filtering for skin colors, finding the two largest contours (finger and its reflection), and identifying the touch/hover point as the midpoint between them. The vertical distance between these contours distinguishes between a touch and a hover. The final step is mapping these webcam coordinates to on-screen coordinates using a homography matrix, which is computed through a calibration process where the user touches specific points on the screen. RANSAC is used for robust estimation.

Currently, Project Sistine translates hover and touch inputs into mouse events, making existing applications touch-enabled. Future enhancements could allow for direct touch data, including hover height. Although a proof-of-concept, it works effectively, with potential for practical application through improvements like a higher resolution webcam (current prototype uses 480p) and a curved mirror for full screen coverage. The prototype's source code is open source under the MIT License.

---

## 17. Show HN: 1-Bit Bonsai, the First Commercially Viable 1-Bit LLMs

**原文标题**: Show HN: 1-Bit Bonsai, the First Commercially Viable 1-Bit LLMs

**原文链接**: [https://prismml.com/](https://prismml.com/)

生成摘要时出错

---

## 18. Open source CAD in the browser (Solvespace)

**原文标题**: Open source CAD in the browser (Solvespace)

**原文链接**: [https://solvespace.com/webver.pl](https://solvespace.com/webver.pl)

生成摘要时出错

---

## 19. CERN levels up with new superconducting karts

**原文标题**: CERN levels up with new superconducting karts

**原文链接**: [https://home.cern/news/news/engineering/cern-levels-new-superconducting-karts](https://home.cern/news/news/engineering/cern-levels-new-superconducting-karts)

CERN has unveiled new superconducting karts designed to provide engineers and technicians with high-speed transport through the 27-km Large Hadron Collider (LHC) tunnel. These vehicles will replace bicycles during the upcoming Long Shutdown 3 (LS3), accelerating work on the High-Luminosity LHC upgrade.

Each kart, described by project leader Mario Idraulico, is "turbo-boosted" by 64 superconducting engines. When cooled, these engines utilize the Meissner effect to levitate the karts, enabling rapid movement. Safety coordinator Luigi Fratello has equipped drivers with SHELLS gear, humorously cautioning against "bananas in the tunnel." Equipment will reach underground areas via giant green pipes.

Remarkably, the kart project's inspiration came from designs by children at CERN's onsite nursery school, who are now dubbed "Luma" for their contributions. Their school director, Rosalina Pfirsich, highlighted the school's focus on curiosity, symbolized by question marks on their yellow walls. Beyond CERN's research, the Knowledge Transfer Group is exploring aerospace applications with Quantum Mushroom for next-generation anti-gravity vehicles.

Dated April 1, 2026, the announcement incorporates numerous playful references to popular video game characters, subtly indicating its lighthearted nature.

---

## 20. I Quit. The Clankers Won

**原文标题**: I Quit. The Clankers Won

**原文链接**: [https://dbushell.com/2026/04/01/i-quit-the-clankers-won/](https://dbushell.com/2026/04/01/i-quit-the-clankers-won/)

生成摘要时出错

---

## 21. Android Developer Verification

**原文标题**: Android Developer Verification

**原文链接**: [https://android-developers.googleblog.com/2026/03/android-developer-verification-rolling-out-to-all-developers.html](https://android-developers.googleblog.com/2026/03/android-developer-verification-rolling-out-to-all-developers.html)

生成摘要时出错

---

## 22. Claude Code users hitting usage limits 'way faster than expected'

**原文标题**: Claude Code users hitting usage limits 'way faster than expected'

**原文链接**: [https://www.theregister.com/2026/03/31/anthropic_claude_code_limits/](https://www.theregister.com/2026/03/31/anthropic_claude_code_limits/)

生成摘要时出错

---

## 23. EmDash – a spiritual successor to WordPress that solves plugin security

**原文标题**: EmDash – a spiritual successor to WordPress that solves plugin security

**原文链接**: [https://blog.cloudflare.com/emdash-wordpress/](https://blog.cloudflare.com/emdash-wordpress/)

生成摘要时出错

---

## 24. Google's 200M-parameter time-series foundation model with 16k context

**原文标题**: Google's 200M-parameter time-series foundation model with 16k context

**原文链接**: [https://github.com/google-research/timesfm](https://github.com/google-research/timesfm)

生成摘要时出错

---

## 25. MiniStack (replacement for LocalStack)

**原文标题**: MiniStack (replacement for LocalStack)

**原文链接**: [https://ministack.org/](https://ministack.org/)

生成摘要时出错

---

## 26. Slop is not necessarily the future

**原文标题**: Slop is not necessarily the future

**原文链接**: [https://www.greptile.com/blog/ai-slopware-future](https://www.greptile.com/blog/ai-slopware-future)

生成摘要时出错

---

## 27. Learn Claude Code by doing, not reading

**原文标题**: Learn Claude Code by doing, not reading

**原文链接**: [https://claude.nagdy.me/](https://claude.nagdy.me/)

生成摘要时出错

---

## 28. Show HN: 30u30.fyi – Is your startup founder on Forbes' most fraudulent list?

**原文标题**: Show HN: 30u30.fyi – Is your startup founder on Forbes' most fraudulent list?

**原文链接**: [https://30u30.fyi](https://30u30.fyi)

生成摘要时出错

---

## 29. U.S. exempts oil industry from protecting Gulf animals, for 'national security'

**原文标题**: U.S. exempts oil industry from protecting Gulf animals, for 'national security'

**原文链接**: [https://www.npr.org/2026/03/30/nx-s1-5745926/endangered-species-committee-hegseth-security](https://www.npr.org/2026/03/30/nx-s1-5745926/endangered-species-committee-hegseth-security)

生成摘要时出错

---

## 30. Safeguarding cryptocurrency by disclosing quantum vulnerabilities responsibly

**原文标题**: Safeguarding cryptocurrency by disclosing quantum vulnerabilities responsibly

**原文链接**: [https://research.google/blog/safeguarding-cryptocurrency-by-disclosing-quantum-vulnerabilities-responsibly/](https://research.google/blog/safeguarding-cryptocurrency-by-disclosing-quantum-vulnerabilities-responsibly/)

生成摘要时出错

---

## 31. Sony halts memory card shipments due to NAND shortage

**原文标题**: Sony halts memory card shipments due to NAND shortage

**原文链接**: [https://www.techzine.eu/news/devices/140058/sony-halts-memory-card-shipments-due-to-nand-shortage/](https://www.techzine.eu/news/devices/140058/sony-halts-memory-card-shipments-due-to-nand-shortage/)

生成摘要时出错

---

## 32. A Nursing Home Owner Got a Pardon. The Families of His Patients Got Nothing

**原文标题**: A Nursing Home Owner Got a Pardon. The Families of His Patients Got Nothing

**原文链接**: [https://www.propublica.org/article/joseph-schwartz-trump-pardon-skyline-nursing-home-patients](https://www.propublica.org/article/joseph-schwartz-trump-pardon-skyline-nursing-home-patients)

生成摘要时出错

---

## 33. Iran says it will target US tech companies in Middle East

**原文标题**: Iran says it will target US tech companies in Middle East

**原文链接**: [https://thehill.com/policy/technology/5809104-iran-irgc-apple-microsoft-google-hp-meta-tesla/](https://thehill.com/policy/technology/5809104-iran-irgc-apple-microsoft-google-hp-meta-tesla/)

生成摘要时出错

---

## 34. The Document Foundation ejects its core developers

**原文标题**: The Document Foundation ejects its core developers

**原文链接**: [https://www.collaboraonline.com/blog/tdf-ejects-its-core-developers/](https://www.collaboraonline.com/blog/tdf-ejects-its-core-developers/)

生成摘要时出错

---

## 35. A new way to measure poverty shows the US falling behind Europe

**原文标题**: A new way to measure poverty shows the US falling behind Europe

**原文链接**: [https://www.euronews.com/business/2026/03/29/a-new-way-to-measure-poverty-shows-the-us-falling-behind-europe](https://www.euronews.com/business/2026/03/29/a-new-way-to-measure-poverty-shows-the-us-falling-behind-europe)

生成摘要时出错

---

## 36. Accidentally created my first fork bomb with Claude Code

**原文标题**: Accidentally created my first fork bomb with Claude Code

**原文链接**: [https://www.droppedasbaby.com/posts/2602-01/](https://www.droppedasbaby.com/posts/2602-01/)

生成摘要时出错

---

## 37. Ukrainian Drone Holds Position for 6 Weeks

**原文标题**: Ukrainian Drone Holds Position for 6 Weeks

**原文链接**: [https://defenceleaders.com/news/ukrainian-combat-robot-holds-frontline-position-for-six-weeks-in-sign-of-growing-ugv-maturity/](https://defenceleaders.com/news/ukrainian-combat-robot-holds-frontline-position-for-six-weeks-in-sign-of-growing-ugv-maturity/)

生成摘要时出错

---

## 38. Incident March 30th, 2026 – Accidental CDN Caching

**原文标题**: Incident March 30th, 2026 – Accidental CDN Caching

**原文链接**: [https://blog.railway.com/p/incident-report-march-30-2026-accidental-cdn-caching](https://blog.railway.com/p/incident-report-march-30-2026-accidental-cdn-caching)

生成摘要时出错

---

## 39. We Built It with Slide Rules. Then We Forgot How

**原文标题**: We Built It with Slide Rules. Then We Forgot How

**原文链接**: [https://unmitigatedrisk.com/?p=1227](https://unmitigatedrisk.com/?p=1227)

生成摘要时出错

---

## 40. What Is Copilot Exactly?

**原文标题**: What Is Copilot Exactly?

**原文链接**: [https://idiallo.com/blog/what-is-copilot-exactly](https://idiallo.com/blog/what-is-copilot-exactly)

生成摘要时出错

---

## 41. We hid a free trip to Switzerland in our privacy policy

**原文标题**: We hid a free trip to Switzerland in our privacy policy

**原文链接**: [https://www.cape.co/blog/easter-egg-in-privacy-policy](https://www.cape.co/blog/easter-egg-in-privacy-policy)

生成摘要时出错

---

## 42. Marc Andreessen's dangerously unexamined life

**原文标题**: Marc Andreessen's dangerously unexamined life

**原文链接**: [https://www.thenation.com/article/society/marc-andreessen-silicon-valley-military-tech/](https://www.thenation.com/article/society/marc-andreessen-silicon-valley-military-tech/)

生成摘要时出错

---

## 43. Claude Code bug can silently 10-20x API costs

**原文标题**: Claude Code bug can silently 10-20x API costs

**原文链接**: [https://old.reddit.com/r/ClaudeCode/comments/1s7mitf/psa_claude_code_has_two_cache_bugs_that_can](https://old.reddit.com/r/ClaudeCode/comments/1s7mitf/psa_claude_code_has_two_cache_bugs_that_can)

生成摘要时出错

---

## 44. Google's insecure-by-default API keys and 30h billing lag cost my startup $15k

**原文标题**: Google's insecure-by-default API keys and 30h billing lag cost my startup $15k

**原文链接**: [https://old.reddit.com/r/googlecloud/comments/1s7v5x9/how_googles_insecurebydefault_api_keys_and_a/](https://old.reddit.com/r/googlecloud/comments/1s7v5x9/how_googles_insecurebydefault_api_keys_and_a/)

生成摘要时出错

---

## 45. Show HN: I turned a sketch into a 3D-print pegboard for my kid with an AI agent

**原文标题**: Show HN: I turned a sketch into a 3D-print pegboard for my kid with an AI agent

**原文链接**: [https://github.com/virpo/pegboard](https://github.com/virpo/pegboard)

生成摘要时出错

---

## 46. Scotty: A beautiful SSH task runner

**原文标题**: Scotty: A beautiful SSH task runner

**原文链接**: [https://freek.dev/3064-scotty-a-beautiful-ssh-task-runner](https://freek.dev/3064-scotty-a-beautiful-ssh-task-runner)

生成摘要时出错

---

## 47. 7,655 Ransomware Claims in One Year: Group, Sector, and Country Breakdown

**原文标题**: 7,655 Ransomware Claims in One Year: Group, Sector, and Country Breakdown

**原文链接**: [https://ciphercue.com/blog/7655-ransomware-claims-march-2025-to-march-2026](https://ciphercue.com/blog/7655-ransomware-claims-march-2025-to-march-2026)

生成摘要时出错

---

## 48. Show HN: Baton – A desktop app for developing with AI agents

**原文标题**: Show HN: Baton – A desktop app for developing with AI agents

**原文链接**: [https://getbaton.dev/](https://getbaton.dev/)

生成摘要时出错

---

## 49. OnlyOffice kills Nextcloud partnership for forking its project without approval

**原文标题**: OnlyOffice kills Nextcloud partnership for forking its project without approval

**原文链接**: [https://www.neowin.net/news/onlyoffice-suspends-nextcloud-partnership-over-unapproved-euro-office-fork/](https://www.neowin.net/news/onlyoffice-suspends-nextcloud-partnership-over-unapproved-euro-office-fork/)

生成摘要时出错

---

## 50. Iran war sparks renewables boom as Europeans rush to buy solar, heat pumps, EVs

**原文标题**: Iran war sparks renewables boom as Europeans rush to buy solar, heat pumps, EVs

**原文链接**: [https://www.euronews.com/2026/03/31/iran-war-sparks-renewables-boom-as-europeans-rush-to-buy-solar-heat-pumps-and-evs](https://www.euronews.com/2026/03/31/iran-war-sparks-renewables-boom-as-europeans-rush-to-buy-solar-heat-pumps-and-evs)

生成摘要时出错

---

## 51. SpaceX Files to Go Public

**原文标题**: SpaceX Files to Go Public

**原文链接**: [https://www.nytimes.com/2026/04/01/technology/spacex-ipo-elon-musk.html](https://www.nytimes.com/2026/04/01/technology/spacex-ipo-elon-musk.html)

生成摘要时出错

---

## 52. Show HN: Real-time dashboard for Claude Code agent teams

**原文标题**: Show HN: Real-time dashboard for Claude Code agent teams

**原文链接**: [https://github.com/simple10/agents-observe](https://github.com/simple10/agents-observe)

生成摘要时出错

---

## 53. Show HN: Sundial – a new way to look at a weather forecast

**原文标题**: Show HN: Sundial – a new way to look at a weather forecast

**原文链接**: [https://sundial.page/](https://sundial.page/)

生成摘要时出错

---

## 54. Prediction: The Shopify CEO's Pull Request Will Never Be Merged nor Closed

**原文标题**: Prediction: The Shopify CEO's Pull Request Will Never Be Merged nor Closed

**原文链接**: [https://joshmoody.org/blog/shopify-ceo-autoresearch-pr/](https://joshmoody.org/blog/shopify-ceo-autoresearch-pr/)

生成摘要时出错

---

## 55. The AI Marketing BS Index

**原文标题**: The AI Marketing BS Index

**原文链接**: [https://bastian.rieck.me/blog/2026/bs/](https://bastian.rieck.me/blog/2026/bs/)

生成摘要时出错

---

## 56. President's new science council: 9 billionaires and 1 scientist

**原文标题**: President's new science council: 9 billionaires and 1 scientist

**原文链接**: [https://www.scientificamerican.com/article/trumps-new-science-panel-includes-9-tech-billionaires-and-just-one-scientist/](https://www.scientificamerican.com/article/trumps-new-science-panel-includes-9-tech-billionaires-and-just-one-scientist/)

生成摘要时出错

---

## 57. TurboQuant KV Compression and SSD Expert Streaming for M5 Pro and IOS

**原文标题**: TurboQuant KV Compression and SSD Expert Streaming for M5 Pro and IOS

**原文链接**: [https://github.com/SharpAI/SwiftLM](https://github.com/SharpAI/SwiftLM)

生成摘要时出错

---

## 58. Securing Elliptic Curve Cryptocurrencies Against Quantum Vulnerabilities [pdf]

**原文标题**: Securing Elliptic Curve Cryptocurrencies Against Quantum Vulnerabilities [pdf]

**原文链接**: [https://quantumai.google/static/site-assets/downloads/cryptocurrency-whitepaper.pdf](https://quantumai.google/static/site-assets/downloads/cryptocurrency-whitepaper.pdf)

生成摘要时出错

---

## 59. A second Starlink satellite exploded in orbit

**原文标题**: A second Starlink satellite exploded in orbit

**原文链接**: [https://twitter.com/LeoLabs_Space/status/2038680177408880719](https://twitter.com/LeoLabs_Space/status/2038680177408880719)

生成摘要时出错

---

## 60. AI has suddenly become more useful to open-source developers

**原文标题**: AI has suddenly become more useful to open-source developers

**原文链接**: [https://www.zdnet.com/article/maybe-open-source-needs-ai/](https://www.zdnet.com/article/maybe-open-source-needs-ai/)

生成摘要时出错

---

## 61. Zelensky says allies asked him to scale back attacks on Russian energy

**原文标题**: Zelensky says allies asked him to scale back attacks on Russian energy

**原文链接**: [https://www.bbc.com/news/articles/c0e7lrxrelwo](https://www.bbc.com/news/articles/c0e7lrxrelwo)

生成摘要时出错

---

## 62. Entirety of Wikinews to be shut down

**原文标题**: Entirety of Wikinews to be shut down

**原文链接**: [https://en.wikipedia.org/wiki/Wikipedia:Wikipedia_Signpost/2026-03-31/News_and_notes](https://en.wikipedia.org/wiki/Wikipedia:Wikipedia_Signpost/2026-03-31/News_and_notes)

生成摘要时出错

---

## 63. Claude Code full source code leaked on NPM

**原文标题**: Claude Code full source code leaked on NPM

**原文链接**: [https://github.com/chatgptprojects/claude-code](https://github.com/chatgptprojects/claude-code)

生成摘要时出错

---

## 64. The German state (Schleswig-Holstein) trying to break free from Microsoft

**原文标题**: The German state (Schleswig-Holstein) trying to break free from Microsoft

**原文链接**: [https://www.ft.com/content/95bd87c8-a112-49a5-9b80-c280a6bb4283](https://www.ft.com/content/95bd87c8-a112-49a5-9b80-c280a6bb4283)

生成摘要时出错

---

## 65. Apple Removes iPhone Vibe Coding App from App Store

**原文标题**: Apple Removes iPhone Vibe Coding App from App Store

**原文链接**: [https://gizmodo.com/apple-removes-iphone-vibe-coding-app-from-app-store-2000740084](https://gizmodo.com/apple-removes-iphone-vibe-coding-app-from-app-store-2000740084)

生成摘要时出错

---

## 66. Solar panels at Lidl? Plug-in versions set to appear in shops

**原文标题**: Solar panels at Lidl? Plug-in versions set to appear in shops

**原文链接**: [https://www.thisismoney.co.uk/money/bills/article-15673955/Solar-panels-Lidl-Plug-versions-set-appear-shops-MONTHS.html](https://www.thisismoney.co.uk/money/bills/article-15673955/Solar-panels-Lidl-Plug-versions-set-appear-shops-MONTHS.html)

生成摘要时出错

---

## 67. Mad Bugs: Vim vs. Emacs vs. Claude

**原文标题**: Mad Bugs: Vim vs. Emacs vs. Claude

**原文链接**: [https://blog.calif.io/p/mad-bugs-vim-vs-emacs-vs-claude](https://blog.calif.io/p/mad-bugs-vim-vs-emacs-vs-claude)

生成摘要时出错

---

## 68. I built a 516-panel financial terminal in 3 weeks using AI

**原文标题**: I built a 516-panel financial terminal in 3 weeks using AI

**原文链接**: [https://neuberg.ai/](https://neuberg.ai/)

生成摘要时出错

---

## 69. A million new SpaceX satellites will destroy the night sky

**原文标题**: A million new SpaceX satellites will destroy the night sky

**原文链接**: [https://theconversation.com/a-million-new-spacex-satellites-will-destroy-the-night-sky-for-everyone-on-earth-277938](https://theconversation.com/a-million-new-spacex-satellites-will-destroy-the-night-sky-for-everyone-on-earth-277938)

生成摘要时出错

---

## 70. Show HN: Claude Code rewritten as a bash script

**原文标题**: Show HN: Claude Code rewritten as a bash script

**原文链接**: [https://github.com/jdcodes1/claude-sh](https://github.com/jdcodes1/claude-sh)

生成摘要时出错

---

## 71. Age verification now required for DNS resolution

**原文标题**: Age verification now required for DNS resolution

**原文链接**: [https://easydns.com/blog/2026/04/01/age-verification-now-required-for-dns-resolution/](https://easydns.com/blog/2026/04/01/age-verification-now-required-for-dns-resolution/)

生成摘要时出错

---

## 72. Jami – free/libre, end-to-end encrypted, and private communication software

**原文标题**: Jami – free/libre, end-to-end encrypted, and private communication software

**原文链接**: [https://jami.net/](https://jami.net/)

生成摘要时出错

---

## 73. What we learned building 100 API integrations with OpenCode

**原文标题**: What we learned building 100 API integrations with OpenCode

**原文链接**: [https://nango.dev/blog/learned-building-200-api-integrations-with-opencode/](https://nango.dev/blog/learned-building-200-api-integrations-with-opencode/)

生成摘要时出错

---

## 74. Apple at 50

**原文标题**: Apple at 50

**原文链接**: [https://www.apple.com/](https://www.apple.com/)

生成摘要时出错

---

## 75. Analyzing Geekbench 6 under Intel's BOT

**原文标题**: Analyzing Geekbench 6 under Intel's BOT

**原文链接**: [https://www.geekbench.com/blog/2026/03/analyzing-geekbench-6-under-intels-bot/](https://www.geekbench.com/blog/2026/03/analyzing-geekbench-6-under-intels-bot/)

生成摘要时出错

---

## 76. Super Micro Computer Investors Look for Exits

**原文标题**: Super Micro Computer Investors Look for Exits

**原文链接**: [https://catenaa.com/markets/equities/super-micro-computer-investors-look-for-exits/](https://catenaa.com/markets/equities/super-micro-computer-investors-look-for-exits/)

生成摘要时出错

---

## 77. CEO of largest public hospital says he's ready to replace radiologists with AI

**原文标题**: CEO of largest public hospital says he's ready to replace radiologists with AI

**原文链接**: [https://radiologybusiness.com/topics/artificial-intelligence/ceo-americas-largest-public-hospital-system-says-hes-ready-replace-radiologists-ai](https://radiologybusiness.com/topics/artificial-intelligence/ceo-americas-largest-public-hospital-system-says-hes-ready-replace-radiologists-ai)

生成摘要时出错

---

## 78. Objections to systemd age-attestation changes go overboard

**原文标题**: Objections to systemd age-attestation changes go overboard

**原文链接**: [https://lwn.net/SubscriberLink/1064706/ba8e449d224f5067/](https://lwn.net/SubscriberLink/1064706/ba8e449d224f5067/)

生成摘要时出错

---

## 79. Scientists uncovered the nutrients bees were missing – Colonies surged 15-fold

**原文标题**: Scientists uncovered the nutrients bees were missing – Colonies surged 15-fold

**原文链接**: [https://www.sciencedaily.com/releases/2026/03/260327000518.htm](https://www.sciencedaily.com/releases/2026/03/260327000518.htm)

生成摘要时出错

---

## 80. Iran threatens Nvidia, Apple and other 18 tech companies

**原文标题**: Iran threatens Nvidia, Apple and other 18 tech companies

**原文链接**: [https://www.cnbc.com/2026/04/01/iran-irgc-nvidia-appple-attack-threat.html](https://www.cnbc.com/2026/04/01/iran-irgc-nvidia-appple-attack-threat.html)

生成摘要时出错

---

## 81. DDR5 RAM prices fall by as much as 30%, but memory shortage likely far from over

**原文标题**: DDR5 RAM prices fall by as much as 30%, but memory shortage likely far from over

**原文链接**: [https://www.notebookcheck.net/DDR5-RAM-prices-fall-by-as-much-as-30-but-memory-shortage-likely-far-from-over.1263431.0.html](https://www.notebookcheck.net/DDR5-RAM-prices-fall-by-as-much-as-30-but-memory-shortage-likely-far-from-over.1263431.0.html)

生成摘要时出错

---

## 82. Closed Source AI = Neofeudalism

**原文标题**: Closed Source AI = Neofeudalism

**原文链接**: [https://geohot.github.io//blog/jekyll/update/2026/03/31/free-intelligence.html](https://geohot.github.io//blog/jekyll/update/2026/03/31/free-intelligence.html)

生成摘要时出错

---

## 83. Trump Tells Aides He's Willing to End War Without Reopening Hormuz

**原文标题**: Trump Tells Aides He's Willing to End War Without Reopening Hormuz

**原文链接**: [https://www.wsj.com/world/middle-east/trump-iran-war-strait-of-hormuz-ee950ad4](https://www.wsj.com/world/middle-east/trump-iran-war-strait-of-hormuz-ee950ad4)

生成摘要时出错

---

## 84. Forth VM and compiler written in C++ and Scryer Prolog

**原文标题**: Forth VM and compiler written in C++ and Scryer Prolog

**原文链接**: [https://github.com/no382001/forth-vm](https://github.com/no382001/forth-vm)

生成摘要时出错

---

## 85. Trump signs order exerting federal control on mail-in ballots

**原文标题**: Trump signs order exerting federal control on mail-in ballots

**原文链接**: [https://www.usatoday.com/story/news/politics/2026/03/31/president-donald-trump-voting-mail-in-ballots-postal-service/89410268007/](https://www.usatoday.com/story/news/politics/2026/03/31/president-donald-trump-voting-mail-in-ballots-postal-service/89410268007/)

生成摘要时出错

---

## 86. Safe ways to do things in bash (2023)

**原文标题**: Safe ways to do things in bash (2023)

**原文链接**: [https://github.com/anordal/shellharden/blob/master/how_to_do_things_safely_in_bash.md](https://github.com/anordal/shellharden/blob/master/how_to_do_things_safely_in_bash.md)

生成摘要时出错

---

