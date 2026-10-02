# Hacker News 热门文章摘要 (2026-10-02)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

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

## 11. Micron CEO Says Memory Supply Will Be Much Tighter in 2027 and 2028 Than in 2026

**原文标题**: Micron CEO Says Memory Supply Will Be Much Tighter in 2027 and 2028 Than in 2026

**原文链接**: [https://www.techpowerup.com/353296/micron-ceo-says-memory-supply-will-be-much-tighter-in-2027-and-2028-than-in-2026](https://www.techpowerup.com/353296/micron-ceo-says-memory-supply-will-be-much-tighter-in-2027-and-2028-than-in-2026)

生成摘要时出错

---

## 12. DeepSeek Harness Desktop for macOS and Windows

**原文标题**: DeepSeek Harness Desktop for macOS and Windows

**原文链接**: [https://www.deepseek.com/en/harness/](https://www.deepseek.com/en/harness/)

生成摘要时出错

---

## 13. RIP, vector database

**原文标题**: RIP, vector database

**原文链接**: [https://turbopuffer.com/blog/rip-vector-database](https://turbopuffer.com/blog/rip-vector-database)

生成摘要时出错

---

## 14. Google breaks promise to provide 10 years of updates to Chromebooks

**原文标题**: Google breaks promise to provide 10 years of updates to Chromebooks

**原文链接**: [https://www.osnews.com/story/146052/google-breaks-promise-to-provide-10-years-of-updates-to-chromebooks/](https://www.osnews.com/story/146052/google-breaks-promise-to-provide-10-years-of-updates-to-chromebooks/)

生成摘要时出错

---

## 15. Fuck Android Developer Verification Program

**原文标题**: Fuck Android Developer Verification Program

**原文链接**: [https://twitter.com/0xcrypto/status/2105515822643114182](https://twitter.com/0xcrypto/status/2105515822643114182)

生成摘要时出错

---

## 16. The top secret URSALA, RAQUEL, and FARRAH satellites (2025)

**原文标题**: The top secret URSALA, RAQUEL, and FARRAH satellites (2025)

**原文链接**: [https://www.thespacereview.com/article/4951/1](https://www.thespacereview.com/article/4951/1)

生成摘要时出错

---

## 17. Cops Can Bypass iPhone's Automatic Reboot to Get into Locked Phones

**原文标题**: Cops Can Bypass iPhone's Automatic Reboot to Get into Locked Phones

**原文链接**: [https://www.404media.co/cops-can-bypass-iphone-automatic-inactivity-reboot-graykey/](https://www.404media.co/cops-can-bypass-iphone-automatic-inactivity-reboot-graykey/)

生成摘要时出错

---

## 18. Cloudflare K2: serverless event streams

**原文标题**: Cloudflare K2: serverless event streams

**原文链接**: [https://blog.cloudflare.com/cloudflare-k2-streams/](https://blog.cloudflare.com/cloudflare-k2-streams/)

生成摘要时出错

---

## 19. Shimano Bicycle Museum Review

**原文标题**: Shimano Bicycle Museum Review

**原文链接**: [https://inrng.com/2026/10/shimano-bicycle-museum/](https://inrng.com/2026/10/shimano-bicycle-museum/)

生成摘要时出错

---

## 20. Various Projects Find Hidden SDR Capabilities in ESP32 Microcontrollers

**原文标题**: Various Projects Find Hidden SDR Capabilities in ESP32 Microcontrollers

**原文链接**: [https://www.rtl-sdr.com/various-projects-independently-find-hidden-sdr-capabilities-in-esp32-microcontrollers/](https://www.rtl-sdr.com/various-projects-independently-find-hidden-sdr-capabilities-in-esp32-microcontrollers/)

生成摘要时出错

---

## 21. How to speed up the Rust compiler in September 2026

**原文标题**: How to speed up the Rust compiler in September 2026

**原文链接**: [https://nnethercote.github.io/2026/09/30/how-to-speed-up-the-rust-compiler-in-september-2026.html](https://nnethercote.github.io/2026/09/30/how-to-speed-up-the-rust-compiler-in-september-2026.html)

生成摘要时出错

---

## 22. 56k.rip – the 1996 dial-up internet experience

**原文标题**: 56k.rip – the 1996 dial-up internet experience

**原文链接**: [https://56k.rip/](https://56k.rip/)

生成摘要时出错

---

## 23. Apple Pass Designer

**原文标题**: Apple Pass Designer

**原文链接**: [https://developer.apple.com/pass-designer/](https://developer.apple.com/pass-designer/)

生成摘要时出错

---

## 24. Meta Uses A.I. Data Centers to Avoid Billions in Federal Taxes

**原文标题**: Meta Uses A.I. Data Centers to Avoid Billions in Federal Taxes

**原文链接**: [https://www.nytimes.com/2026/09/30/technology/meta-ai-data-centers-taxes.html](https://www.nytimes.com/2026/09/30/technology/meta-ai-data-centers-taxes.html)

生成摘要时出错

---

## 25. Automatic Transmission – a data-privacy study of connected vehicles

**原文标题**: Automatic Transmission – a data-privacy study of connected vehicles

**原文链接**: [https://automatictransmission.khoury.northeastern.edu/index.html](https://automatictransmission.khoury.northeastern.edu/index.html)

生成摘要时出错

---

## 26. How Singapore's government-run dating service works

**原文标题**: How Singapore's government-run dating service works

**原文链接**: [https://www.singapore-samizdat.com/p/how-singapores-government-run-dating-service-firstdate-works](https://www.singapore-samizdat.com/p/how-singapores-government-run-dating-service-firstdate-works)

生成摘要时出错

---

## 27. FLUX 3 Image

**原文标题**: FLUX 3 Image

**原文链接**: [https://bfl.ai/models/flux-3-image](https://bfl.ai/models/flux-3-image)

生成摘要时出错

---

## 28. The death of web development education

**原文标题**: The death of web development education

**原文链接**: [https://molily.de/web-dev-education/](https://molily.de/web-dev-education/)

生成摘要时出错

---

## 29. The Legend of von Neumann (1973) [pdf]

**原文标题**: The Legend of von Neumann (1973) [pdf]

**原文链接**: [https://gwern.net/doc/math/1973-halmos.pdf](https://gwern.net/doc/math/1973-halmos.pdf)

生成摘要时出错

---

## 30. Using Opus 5.5 to discover a new eyewitness record of the dodo

**原文标题**: Using Opus 5.5 to discover a new eyewitness record of the dodo

**原文链接**: [https://resobscura.substack.com/p/using-opus-55-to-discover-a-new-eyewitness](https://resobscura.substack.com/p/using-opus-55-to-discover-a-new-eyewitness)

生成摘要时出错

---

## 31. Red Hat being phased out of existence?

**原文标题**: Red Hat being phased out of existence?

**原文链接**: [https://techrights.org/n/2026/10/01/Red_Hat_Being_Phased_Out_of_Existence_Like_Many_Other_Companies.shtml](https://techrights.org/n/2026/10/01/Red_Hat_Being_Phased_Out_of_Existence_Like_Many_Other_Companies.shtml)

生成摘要时出错

---

## 32. FTC is investigating OpenAI, Anthropic and other AI companies over product risks

**原文标题**: FTC is investigating OpenAI, Anthropic and other AI companies over product risks

**原文链接**: [https://www.cnbc.com/2026/09/30/ftc-ai-probe-openai-anthropic.html](https://www.cnbc.com/2026/09/30/ftc-ai-probe-openai-anthropic.html)

生成摘要时出错

---

## 33. Big Tech ruined the cloud, so we're renaming ours

**原文标题**: Big Tech ruined the cloud, so we're renaming ours

**原文链接**: [https://www.home-assistant.io/blog/2026/10/02/big-tech-ruined-the-cloud-so-were-renaming-ours/](https://www.home-assistant.io/blog/2026/10/02/big-tech-ruined-the-cloud-so-were-renaming-ours/)

生成摘要时出错

---

## 34. Vote on which of Hacker News' challenges for AI have been met

**原文标题**: Vote on which of Hacker News' challenges for AI have been met

**原文链接**: [https://stoppels.ch/goalposts/](https://stoppels.ch/goalposts/)

生成摘要时出错

---

## 35. Turbo Haskell

**原文标题**: Turbo Haskell

**原文链接**: [https://comonad.com/reader/2026/turbo-haskell/](https://comonad.com/reader/2026/turbo-haskell/)

生成摘要时出错

---

## 36. ICC judge on what U.S. sanctions mean for her and global courts

**原文标题**: ICC judge on what U.S. sanctions mean for her and global courts

**原文链接**: [https://www.npr.org/2026/10/01/nx-s1-5977815/trump-icc-sanctions-kimberly-prost](https://www.npr.org/2026/10/01/nx-s1-5977815/trump-icc-sanctions-kimberly-prost)

生成摘要时出错

---

## 37. Supabase is acquiring Turso

**原文标题**: Supabase is acquiring Turso

**原文链接**: [https://supabase.com/blog/supabase-is-acquiring-turso](https://supabase.com/blog/supabase-is-acquiring-turso)

生成摘要时出错

---

## 38. Figma restricts MCP access to whitelisted clients, excluding Pi

**原文标题**: Figma restricts MCP access to whitelisted clients, excluding Pi

**原文链接**: [https://twitter.com/GayaniFigma/status/2105295629941350454](https://twitter.com/GayaniFigma/status/2105295629941350454)

生成摘要时出错

---

## 39. GPT-Synopsys: Frontier Intelligence to Revolutionize Chip Design

**原文标题**: GPT-Synopsys: Frontier Intelligence to Revolutionize Chip Design

**原文链接**: [https://news.synopsys.com/2026-09-30-OpenAI-and-Synopsys-Announce-GPT-Synopsys-Frontier-Intelligence-to-Revolutionize-Chip-Design](https://news.synopsys.com/2026-09-30-OpenAI-and-Synopsys-Announce-GPT-Synopsys-Frontier-Intelligence-to-Revolutionize-Chip-Design)

生成摘要时出错

---

## 40. AI Makes Me Sad

**原文标题**: AI Makes Me Sad

**原文链接**: [https://mondobe.com/ai-makes-me-sad](https://mondobe.com/ai-makes-me-sad)

生成摘要时出错

---

## 41. Show HN: Giving Opus 5.5 a simulated paint canvas

**原文标题**: Show HN: Giving Opus 5.5 a simulated paint canvas

**原文链接**: [https://stillwet.art/](https://stillwet.art/)

生成摘要时出错

---

## 42. Sites in ChatGPT

**原文标题**: Sites in ChatGPT

**原文链接**: [https://chatgpt.com/features/sites/](https://chatgpt.com/features/sites/)

生成摘要时出错

---

## 43. Context Language Models

**原文标题**: Context Language Models

**原文链接**: [https://arxiv.org/abs/2609.37725](https://arxiv.org/abs/2609.37725)

生成摘要时出错

---

## 44. Mike Tomlin spent 12 years building a Minecraft city

**原文标题**: Mike Tomlin spent 12 years building a Minecraft city

**原文链接**: [https://www.nytimes.com/athletic/7648198/2026/10/01/mike-tomlin-minecraft-nfl-coach/](https://www.nytimes.com/athletic/7648198/2026/10/01/mike-tomlin-minecraft-nfl-coach/)

生成摘要时出错

---

## 45. CSS Bed: Classless CSS themes to use as starting points in web development

**原文标题**: CSS Bed: Classless CSS themes to use as starting points in web development

**原文链接**: [https://www.cssbed.com](https://www.cssbed.com)

生成摘要时出错

---

## 46. RacketCon Is Saturday

**原文标题**: RacketCon Is Saturday

**原文链接**: [https://con.racket-lang.org/](https://con.racket-lang.org/)

生成摘要时出错

---

## 47. Greg Kroah-Hartman – Security in the LLM Age [video]

**原文标题**: Greg Kroah-Hartman – Security in the LLM Age [video]

**原文链接**: [https://www.youtube.com/watch?v=NnV_cWeoo5Q](https://www.youtube.com/watch?v=NnV_cWeoo5Q)

生成摘要时出错

---

## 48. Zig v0.17.0

**原文标题**: Zig v0.17.0

**原文链接**: [https://ziglang.org/download/0.17.0/release-notes.html](https://ziglang.org/download/0.17.0/release-notes.html)

生成摘要时出错

---

## 49. A 12-year sequence of telescope images of a star and four planets orbiting

**原文标题**: A 12-year sequence of telescope images of a star and four planets orbiting

**原文链接**: [https://bsky.app/profile/theplanetaryguy.com/post/3mwucf5ert22f](https://bsky.app/profile/theplanetaryguy.com/post/3mwucf5ert22f)

生成摘要时出错

---

## 50. ArXiv's Updated Rate Limit Policy

**原文标题**: ArXiv's Updated Rate Limit Policy

**原文链接**: [https://blog.arxiv.org/2026/10/01/updated-rate-limit-policy/](https://blog.arxiv.org/2026/10/01/updated-rate-limit-policy/)

生成摘要时出错

---

## 51. Loss of cell identity drives human aging: Two new papers

**原文标题**: Loss of cell identity drives human aging: Two new papers

**原文链接**: [https://erictopol.substack.com/p/loss-of-cell-identity-drives-human](https://erictopol.substack.com/p/loss-of-cell-identity-drives-human)

生成摘要时出错

---

## 52. With most information hidden, the game Stratego had stumped AI until now

**原文标题**: With most information hidden, the game Stratego had stumped AI until now

**原文链接**: [https://arstechnica.com/science/2026/10/ai-finally-beat-the-best-stratego-player-in-history-and-did-it-on-a-budget/](https://arstechnica.com/science/2026/10/ai-finally-beat-the-best-stratego-player-in-history-and-did-it-on-a-budget/)

生成摘要时出错

---

## 53. Tiny Brutalism

**原文标题**: Tiny Brutalism

**原文链接**: [https://placeholders.itch.io/tiny-brutalism](https://placeholders.itch.io/tiny-brutalism)

生成摘要时出错

---

## 54. Show HN: Audionaut – an open-source cross-platform multitrack audio editor

**原文标题**: Show HN: Audionaut – an open-source cross-platform multitrack audio editor

**原文链接**: [https://github.com/kvoltmer/Audionaut](https://github.com/kvoltmer/Audionaut)

生成摘要时出错

---

## 55. To grieve, or not to grieve?

**原文标题**: To grieve, or not to grieve?

**原文链接**: [https://xenaproject.wordpress.com/2026/10/01/to-grieve-or-not-to-grieve/](https://xenaproject.wordpress.com/2026/10/01/to-grieve-or-not-to-grieve/)

生成摘要时出错

---

## 56. Oxygen-deprived underwater zones may not be “dead zones” but clue to early life

**原文标题**: Oxygen-deprived underwater zones may not be “dead zones” but clue to early life

**原文链接**: [https://agupubs.onlinelibrary.wiley.com/doi/10.1029/2026AV002570](https://agupubs.onlinelibrary.wiley.com/doi/10.1029/2026AV002570)

生成摘要时出错

---

## 57. SlutCon

**原文标题**: SlutCon

**原文链接**: [https://www.thenewcritic.com/p/safe-at-slutcon](https://www.thenewcritic.com/p/safe-at-slutcon)

生成摘要时出错

---

## 58. Bez: Generating a browser engine from specs and tests

**原文标题**: Bez: Generating a browser engine from specs and tests

**原文链接**: [https://tangled.org/burrito.space/bez](https://tangled.org/burrito.space/bez)

生成摘要时出错

---

## 59. 10-year Treasury yield climbs above 5.3% to a level not seen in 24 years

**原文标题**: 10-year Treasury yield climbs above 5.3% to a level not seen in 24 years

**原文链接**: [https://www.wsj.com/finance/investing/surging-yields-bring-the-bond-market-back-to-the-turn-of-the-century-2b74773f](https://www.wsj.com/finance/investing/surging-yields-bring-the-bond-market-back-to-the-turn-of-the-century-2b74773f)

生成摘要时出错

---

## 60. Nazi Germany had no hope of making an atomic bomb, uranium cubes reveal

**原文标题**: Nazi Germany had no hope of making an atomic bomb, uranium cubes reveal

**原文链接**: [https://www.science.org/content/article/nazi-germany-had-no-hope-making-atomic-bomb-uranium-cubes-reveal](https://www.science.org/content/article/nazi-germany-had-no-hope-making-atomic-bomb-uranium-cubes-reveal)

生成摘要时出错

---

## 61. On social reality in China

**原文标题**: On social reality in China

**原文链接**: [https://www.lesswrong.com/posts/b5cSYh4emQb2qrGmK/on-social-reality-in-china](https://www.lesswrong.com/posts/b5cSYh4emQb2qrGmK/on-social-reality-in-china)

生成摘要时出错

---

## 62. From the creator of Redis; run LLM locally with ds4

**原文标题**: From the creator of Redis; run LLM locally with ds4

**原文链接**: [https://dwarfstar.sh/](https://dwarfstar.sh/)

生成摘要时出错

---

## 63. The Four Horsemen of Agentic Coding

**原文标题**: The Four Horsemen of Agentic Coding

**原文链接**: [https://distantprovince.substack.com/p/the-four-horsemen-of-agentic-coding](https://distantprovince.substack.com/p/the-four-horsemen-of-agentic-coding)

生成摘要时出错

---

## 64. Dutch computer museums (2022)

**原文标题**: Dutch computer museums (2022)

**原文链接**: [https://aresluna.org/dutch-computer-museums/](https://aresluna.org/dutch-computer-museums/)

生成摘要时出错

---

## 65. Show HN: Janus – Go binary that runs GGUF models via Vulkan on AMD/Intel/Nvidia

**原文标题**: Show HN: Janus – Go binary that runs GGUF models via Vulkan on AMD/Intel/Nvidia

**原文链接**: [https://github.com/Vibra-Ingenn/Janus](https://github.com/Vibra-Ingenn/Janus)

生成摘要时出错

---

## 66. US tells France and Germany to release diesel stocks or face US export ban

**原文标题**: US tells France and Germany to release diesel stocks or face US export ban

**原文链接**: [https://www.reuters.com/business/energy/us-tells-france-germany-release-diesel-stocks-or-face-us-export-ban-sources-say-2026-10-01/](https://www.reuters.com/business/energy/us-tells-france-germany-release-diesel-stocks-or-face-us-export-ban-sources-say-2026-10-01/)

生成摘要时出错

---

## 67. Cities Are Forced to Funnel License Plate Data to a Federal Surveillance Program

**原文标题**: Cities Are Forced to Funnel License Plate Data to a Federal Surveillance Program

**原文链接**: [https://www.404media.co/how-cities-are-forced-to-funnel-license-plate-data-to-a-massive-federal-surveillance-program-hidta/](https://www.404media.co/how-cities-are-forced-to-funnel-license-plate-data-to-a-massive-federal-surveillance-program-hidta/)

生成摘要时出错

---

## 68. An AI sovereign wealth fund isn't progressive – it's techno-imperialism

**原文标题**: An AI sovereign wealth fund isn't progressive – it's techno-imperialism

**原文链接**: [https://www.ft.com/content/bc178357-793b-45d8-ae3b-d5929159c243](https://www.ft.com/content/bc178357-793b-45d8-ae3b-d5929159c243)

生成摘要时出错

---

## 69. Everyone's Packing Up

**原文标题**: Everyone's Packing Up

**原文链接**: [https://widdershins.verja.net/everyones-packing-up/](https://widdershins.verja.net/everyones-packing-up/)

生成摘要时出错

---

## 70. How to set up SPF, DKIM, and DMARC for your sending domain

**原文标题**: How to set up SPF, DKIM, and DMARC for your sending domain

**原文链接**: [https://mailfully.com/blog/spf-dkim-dmarc-setup](https://mailfully.com/blog/spf-dkim-dmarc-setup)

生成摘要时出错

---

## 71. GrapheneOS has fixed the Android 17 QPR1 kernel performance regression

**原文标题**: GrapheneOS has fixed the Android 17 QPR1 kernel performance regression

**原文链接**: [https://discuss.grapheneos.org/d/42511-grapheneos-has-fixed-the-massive-android-17-qpr1-kernel-performance-regression](https://discuss.grapheneos.org/d/42511-grapheneos-has-fixed-the-massive-android-17-qpr1-kernel-performance-regression)

生成摘要时出错

---

## 72. Suits Are Better Tech Than Modern Clothes

**原文标题**: Suits Are Better Tech Than Modern Clothes

**原文链接**: [https://devz.cl/posts/the-lost-tech-in-contemporary-clothing/](https://devz.cl/posts/the-lost-tech-in-contemporary-clothing/)

生成摘要时出错

---

## 73. Lightweight PDF parser with layout, tables, formulas and bounding boxes

**原文标题**: Lightweight PDF parser with layout, tables, formulas and bounding boxes

**原文链接**: [https://github.com/beatrizalmeidaf/papero-pdf-text-extractor](https://github.com/beatrizalmeidaf/papero-pdf-text-extractor)

生成摘要时出错

---

## 74. Effect 4.0

**原文标题**: Effect 4.0

**原文链接**: [https://effect.website/blog/releases/effect/40](https://effect.website/blog/releases/effect/40)

生成摘要时出错

---

## 75. One month coding with GLM 5.3 Flash

**原文标题**: One month coding with GLM 5.3 Flash

**原文链接**: [https://wagtail.org/blog/one-month-on-glm-53-flash/](https://wagtail.org/blog/one-month-on-glm-53-flash/)

生成摘要时出错

---

## 76. Crypto Capture of Foreign Aid

**原文标题**: Crypto Capture of Foreign Aid

**原文链接**: [https://www.nber.org/papers/w35655](https://www.nber.org/papers/w35655)

生成摘要时出错

---

## 77. Canada fast-tracks Pacific oil pipeline to reduce US dependence

**原文标题**: Canada fast-tracks Pacific oil pipeline to reduce US dependence

**原文链接**: [https://apnews.com/article/alberta-canada-carney-pipeline-68539133d6e0245fad3622263afd4aeb](https://apnews.com/article/alberta-canada-carney-pipeline-68539133d6e0245fad3622263afd4aeb)

生成摘要时出错

---

## 78. California bans child marriage, a practice still legal in 32 US states

**原文标题**: California bans child marriage, a practice still legal in 32 US states

**原文链接**: [https://www.bbc.com/news/articles/c6rm9mnn0w3eo](https://www.bbc.com/news/articles/c6rm9mnn0w3eo)

生成摘要时出错

---

## 79. Identity Management for Agentic AI [pdf] (2025)

**原文标题**: Identity Management for Agentic AI [pdf] (2025)

**原文链接**: [https://openid.net/wp-content/uploads/2025/10/Identity-Management-for-Agentic-AI.pdf](https://openid.net/wp-content/uploads/2025/10/Identity-Management-for-Agentic-AI.pdf)

生成摘要时出错

---

## 80. Butterflies use optical illusions to dodge predators

**原文标题**: Butterflies use optical illusions to dodge predators

**原文链接**: [https://www.essex.ac.uk/news/2026/09/30/butterflies-use-optical-illusions-to-dodge-predators](https://www.essex.ac.uk/news/2026/09/30/butterflies-use-optical-illusions-to-dodge-predators)

生成摘要时出错

---

## 81. Redditor buys used CPU, turns out it was banned on Valorant and they are SoL

**原文标题**: Redditor buys used CPU, turns out it was banned on Valorant and they are SoL

**原文链接**: [https://www.reddit.com/r/LinusTechTips/comments/1wvr096/wan_show_topic_redditor_buys_used_cpu_turns_out/](https://www.reddit.com/r/LinusTechTips/comments/1wvr096/wan_show_topic_redditor_buys_used_cpu_turns_out/)

生成摘要时出错

---

## 82. Updates to Full Disk Access in macOS

**原文标题**: Updates to Full Disk Access in macOS

**原文链接**: [https://developer.apple.com/news/?id=p6zjojqw](https://developer.apple.com/news/?id=p6zjojqw)

生成摘要时出错

---

## 83. Amazon seeks to offload $8B of Nvidia chips to investors

**原文标题**: Amazon seeks to offload $8B of Nvidia chips to investors

**原文链接**: [https://www.reuters.com/business/retail-consumer/amazon-seeks-offload-8-billion-nvidia-chips-investors-ft-reports-2026-10-02/](https://www.reuters.com/business/retail-consumer/amazon-seeks-offload-8-billion-nvidia-chips-investors-ft-reports-2026-10-02/)

生成摘要时出错

---

## 84. GPT-6 Astra plays World of Warcraft for the first time with agent-wow

**原文标题**: GPT-6 Astra plays World of Warcraft for the first time with agent-wow

**原文链接**: [https://agent-wow.sh/gpt-6-astra-plays-world-of-warcraft-for-the-first-time-with-agent-wow/](https://agent-wow.sh/gpt-6-astra-plays-world-of-warcraft-for-the-first-time-with-agent-wow/)

生成摘要时出错

---

## 85. Muse Gadgets

**原文标题**: Muse Gadgets

**原文链接**: [https://gadgets.muse.ai](https://gadgets.muse.ai)

生成摘要时出错

---

## 86. Why media fans want to escape algorithms with CDs, DVDs and vinyl

**原文标题**: Why media fans want to escape algorithms with CDs, DVDs and vinyl

**原文链接**: [https://www.theguardian.com/media/2026/oct/02/physical-media-fans-streaming-algorithms-cds-dvds-vinyl](https://www.theguardian.com/media/2026/oct/02/physical-media-fans-streaming-algorithms-cds-dvds-vinyl)

生成摘要时出错

---

## 87. ParadeDB Search Performance Improvements

**原文标题**: ParadeDB Search Performance Improvements

**原文链接**: [https://www.paradedb.com/blog/opening-a-closed-tin](https://www.paradedb.com/blog/opening-a-closed-tin)

生成摘要时出错

---

## 88. Alarm Grows over 'Clearly Illegal' US Election Meddling in Brazil

**原文标题**: Alarm Grows over 'Clearly Illegal' US Election Meddling in Brazil

**原文链接**: [https://www.commondreams.org/news/trump-election-interference-brazil](https://www.commondreams.org/news/trump-election-interference-brazil)

生成摘要时出错

---

## 89. Don't be fooled–LLMs don't reason

**原文标题**: Don't be fooled–LLMs don't reason

**原文链接**: [https://www.technologyreview.com/2026/10/02/1145639/dont-be-fooled-llms-dont-reason/](https://www.technologyreview.com/2026/10/02/1145639/dont-be-fooled-llms-dont-reason/)

生成摘要时出错

---

## 90. European payments groups join forces to challenge US dominance

**原文标题**: European payments groups join forces to challenge US dominance

**原文链接**: [https://www.rte.ie/news/business/2026/1001/1593639-european-payments-group/](https://www.rte.ie/news/business/2026/1001/1593639-european-payments-group/)

生成摘要时出错

---

## 91. Meta's Muse is fantastic for web scraping

**原文标题**: Meta's Muse is fantastic for web scraping

**原文链接**: [https://sigh.dev/posts/metas-muse-is-fantastic-for-web-scraping/](https://sigh.dev/posts/metas-muse-is-fantastic-for-web-scraping/)

生成摘要时出错

---

## 92. A fifth of Swiss Alpine ice has vanished in five years

**原文标题**: A fifth of Swiss Alpine ice has vanished in five years

**原文链接**: [https://www.swissinfo.ch/eng/glaciers-permafrost/a-fifth-of-swiss-alpine-ice-has-vanished-in-five-years/92132132](https://www.swissinfo.ch/eng/glaciers-permafrost/a-fifth-of-swiss-alpine-ice-has-vanished-in-five-years/92132132)

生成摘要时出错

---

## 93. Show HN: Rhun, an open-source code editor written in assembly

**原文标题**: Show HN: Rhun, an open-source code editor written in assembly

**原文链接**: [https://rhun.app/](https://rhun.app/)

生成摘要时出错

---

## 94. Anatomy of a Lean proof for software engineers

**原文标题**: Anatomy of a Lean proof for software engineers

**原文链接**: [https://agostbiro.net/posts/2026-10-anatomy-of-a-lean-proof/](https://agostbiro.net/posts/2026-10-anatomy-of-a-lean-proof/)

生成摘要时出错

---

## 95. Polyedergarten: Garden of Paper Polyhedron Models

**原文标题**: Polyedergarten: Garden of Paper Polyhedron Models

**原文链接**: [https://www.polyedergarten.de/e_index.htm](https://www.polyedergarten.de/e_index.htm)

生成摘要时出错

---

## 96. IANA's email about why example.com changed

**原文标题**: IANA's email about why example.com changed

**原文链接**: [https://www.oliverdunk.com/2026/09/30/iana-reply](https://www.oliverdunk.com/2026/09/30/iana-reply)

生成摘要时出错

---

## 97. Venice’s failed war against Constantinople led to the first bond market

**原文标题**: Venice’s failed war against Constantinople led to the first bond market

**原文链接**: [https://bigthink.com/books/a-fabulous-debt/](https://bigthink.com/books/a-fabulous-debt/)

生成摘要时出错

---

## 98. Show HN: Pyxel – A Python retro game engine with built-in art and sound editors

**原文标题**: Show HN: Pyxel – A Python retro game engine with built-in art and sound editors

**原文链接**: [https://github.com/kitao/pyxel](https://github.com/kitao/pyxel)

生成摘要时出错

---

## 99. Giving friends custom text buzzes based on Morse code

**原文标题**: Giving friends custom text buzzes based on Morse code

**原文链接**: [https://liquidbrain.net/blog/giving-friends-custom-text-buzzes-based-on-morse-code/](https://liquidbrain.net/blog/giving-friends-custom-text-buzzes-based-on-morse-code/)

生成摘要时出错

---

## 100. macOS 27 is so buggy

**原文标题**: macOS 27 is so buggy

**原文链接**: [https://osxdaily.com/2026/09/30/buggy-laggy-mission-control-spaces-stage-manager-in-macos-27-golden-gate-try-these-tips/](https://osxdaily.com/2026/09/30/buggy-laggy-mission-control-spaces-stage-manager-in-macos-27-golden-gate-try-these-tips/)

生成摘要时出错

---

