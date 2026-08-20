# Hacker News 热门文章摘要 (2026-08-20)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 解锁锁定/停用的废弃Cricut Maker

**原文标题**: Unlocking a locked/deactivated e-waste Cricut Maker

**原文链接**: [https://sprocketfox.io/xssfox/2026/07/01/cricut-unlock/](https://sprocketfox.io/xssfox/2026/07/01/cricut-unlock/)

某人从电子垃圾中发现了一台已停用的Cricut Maker，外观完好，但滚轮已损坏并显示“机器已停用”错误。最初尝试通过重写EEPROM（未找到）或拦截网络流量（由于证书锁定）来重新激活它，均未成功。

成功的方法涉及拦截Cricut和电脑之间的USB通信。作者使用Wireshark发现序列号数据包未加密发送且没有校验和。随后，使用一块超频的RP2040微控制器，充当USB主设备和从设备，创建一个硬件代理。该设备拦截Cricut发出的序列号，将其替换为一个新的、可用的序列号，并将其传递给电脑。这种实时序列号重写骗过了软件，使其识别为一台“新”机器，从而恢复了全部功能。

除了此破解方法之外，还更换了滚轮（用热水软化），清洁并重新组装了机器，并将RP2040安置妥当。机器现在运行起来如同全新。作者承认这是一个硬件密集型解决方案，并提出了一些基于软件的替代方案。由于潜在的版权问题，序列号重写的具体代码未公开分享。

---

## 2. 中情局的资金帮助NeXT在80年代得以存续。

**原文标题**: CIA funding helped keep NeXT afloat in the 80s

**原文链接**: [https://www.wsj.com/tech/steve-jobs-apple-next-cia-161b65f9?st=NWWds1&reflink=desktopwebshare_permalink](https://www.wsj.com/tech/steve-jobs-apple-next-cia-161b65f9?st=NWWds1&reflink=desktopwebshare_permalink)

无法访问文章链接。

---

## 3. Mojo语言（由Modular开发，现属高通）现已开源。

**原文标题**: The Mojo language (by Modular, now Qualcomm) is now open-source

**原文链接**: [https://www.modular.com/blog/modcon-announcements](https://www.modular.com/blog/modcon-announcements)

ModCon 2026大会于2026年8月18日举行，Modular（现已并入高通）在此次大会上宣布了几项关键进展，这些进展与其在异构硬件上实现AI的愿景保持一致。

至关重要的是，**Mojo语言1.0现已基于Apache 2.0许可证全面开源**，包括其编译器和工具链。继其标准库和MAX内核早前开源之后，这一战略举措使开发者能够扩展Mojo并将其引入新平台。与微软的合作也正在进行中，旨在为Mojo提供原生Windows支持。

**Modular Cloud**现已作为生产服务正式上线，它抽象化了在多样化基础设施上部署和优化模型的复杂性。该服务提供行业领先的推理性能，为MiniMax等旗舰客户提供支持（以每分钟数十亿token的速度驱动M3），并此前已与OpenRouter共同展现出卓越性能。

此外，**Modular平台**已显著扩展其硬件支持范围，从GPU扩展到AWS Trainium、Google TPU、高通Cloud AI 100和高通Dragonfly，展示了高可移植性，新集成所需的工程工作量减少了10倍。

为了促进生态系统协作，**MAX许可证已放宽**，取消了设备使用限制，并且MAX将通过开放联盟计划提供源代码。在近期高通收购Modular的强化下，该举措旨在构建一个通用的、开放的软件基础，业界可以在其上协作优化适用于任何加速器的AI。

---

## 4. Ornith-1.5：从自我搭建到自我提升

**原文标题**: Ornith-1.5: From Self-Scaffolding to Self-Improvement

**原文链接**: [https://ornith.ai/ornith_1_5.html](https://ornith.ai/ornith_1_5.html)

Ornith-1.5 引入了一个端到端的基础模型自我提升框架，将 Ornith-1.0 的自支架扩展为一个持续学习循环。它允许模型自主提出新的、难度递增的任务，生成针对任务的支架（指令、工具、策略），并为强化学习生成解决方案推演，从而不断创造新的训练经验。

该系统有三种规模：397B MoE 模型、35B MoE 模型和一个 9B 密集模型，同时还有一个针对 iPhone 和 Android 优化的移动版 9B 模型。这一自我提升过程分为三个阶段，由特定的奖励信号引导：
1.  **任务奖励：** 鼓励生成有效、可验证、难度适中（目标成功率 20%）且新颖的任务。
2.  **驾驭奖励：** 促进创建与任务对齐、忠实反映解决方案质量且能抵抗奖励作弊的评估环境。
3.  **推演奖励：** 根据任务成功情况直接评估策略的解决方案尝试。

这一闭环系统使 Ornith-1.5 能够动态扩展其课程并调整问题解决策略，从而在推理、编码和智能体任务中持续提升能力。

Ornith-1.5 在开源模型中取得了最先进的性能。其旗舰级 397B 模型在 Terminal-Bench 2.1 (86.1) 和 DeepSWE (56.0) 等基准测试中表现与 Claude Opus 4.8 不相上下，超越了 GLM-5.2 和 DeepSeek-V4-Flash-0731 等领先的开源模型。35B 模型显著优于同等规模及更大规模的密集模型，如 Gemma 4-31B。令人印象深刻的是，紧凑型 9B 模型与更大规模模型（例如 Gemma 4-31B、Qwen 3.6-35B）的性能持平或超越，展现了强大的边缘部署能力。

---

## 5. AI时代的数学

**原文标题**: Mathematics in the age of AI

**原文链接**: [https://arxiv.org/abs/2608.16753](https://arxiv.org/abs/2608.16753)

这篇由陶哲轩撰写、于2026年8月17日提交的arXiv论文《人工智能时代的数学》，是基于其在2026年国际数学家大会上发表的一次公开演讲的随笔。

该论文探讨了数学界应如何应对能够执行研究级数学任务的人工智能工具的出现这一关键问题。陶哲轩的随笔并未就此类人工智能的确切能力展开辩论，而是采纳了这些能力 *将会* 实现的假设。

基于这一假设，焦点转向了一个更基础、更“正交”的探究：数学研究的目标和价值究竟是什么？论文以数学的问题解决方面为例，来探讨这个更深层次的问题。该论文共12页，包含四幅图，旨在引发人们对人工智能增强的未来中数学探索核心本质的反思。它属于“历史与概述 (math.HO)”这一主题类别。

---

## 6. Solo：一个用于静态 Linux 二进制文件的 .so 加载器

**原文标题**: Solo – a .so loader for static Linux binaries

**原文链接**: [https://github.com/pg83/solo](https://github.com/pg83/solo)

SoLo是一个创新的.so加载器，它使完全静态的、使用musl链接的Linux二进制文件能够在运行时动态加载glibc链接的共享对象（例如GPU驱动）。这解决了长期存在的问题，即静态musl应用程序通常无法使用主机提供的glibc驱动，传统上这需要借助容器或AppImages等繁琐的解决方案。

SoLo通过提供`dlfcn`风格的API、一个嵌入式ELF加载器（支持x86-64和aarch64），以及一个直接基于musl实现的glibc ABI桥来达到这一目的。至关重要的是，这种设计意味着进程中不会引入第二个`libc`；glibc的导入会被转换为使用现有的musl运行时。该系统精心处理复杂的跨运行时特性，包括C++异常、所有四种TLS模型、`ld.so`的绑定语义、跨环境自省以及有状态的glibc构造，确保无缝交互。

该项目通过端到端的Vulkan验证证实了其主张，演示了一个静态可执行文件如何加载并利用主机未修改的Vulkan驱动来运行计算着色器并生成PNG。其鲁棒性通过持续集成得到验证，加载了来自排名前1000个Debian软件包中的2100多个共享对象。

SoLo通过将其整个加载和ABI转换机制嵌入到静态可执行文件中，从而区别于现有工作。这避免了引导系统动态链接器、引入第二个`libc`或复杂的TLS上下文切换，为需要硬件访问的静态二进制文件提供了一个更简洁、更易于检查且真正便携的解决方案。

---

## 7. 斯泰普收购奥本沃特

**原文标题**: Stwipe Acquires OpenWouter

**原文链接**: [https://stwipe.com/](https://stwipe.com/)

Stwipe, a satirical company, announces its acquisition of OpenWouter, a fictional "intelligence infrastructure" embodied by a single Dutch man named Wouter. This parody of recent M&A deals, particularly Stripe's acquisition of OpenRouter, positions Stwipe as responding to the AI industry's consolidation.

Unlike OpenRouter's 500+ language models, OpenWouter offers "one API, one Wouter," whose primary function is to say "no" (Nee.). Wouter operates on strict hours (09:00–17:00 CET, never in August), has an infinite context window, remembers everything, and boasts 100% refusal accuracy and 0.0 sycophancy according to satirical evaluations. Stwipe's strategic rationale is to complement its existing "200 OK" (always yes) API with Wouter's unwavering negation, achieving "total coverage" for business decisions.

The transaction terms are "fine" (according to Wouter), with no integration workstreams as he declined. Stwipe celebrates acquiring something for the first time rather than raising money.

The article concludes with a vital "Actual Notice," clarifying that Stwipe, OpenWouter, and the acquisition are entirely fictional satire. However, a live `/v1/no` API endpoint, providing Wouter's refusal, is genuinely active.

---

## 8. Bun 1.4

**原文标题**: Bun 1.4

**原文链接**: [https://bun.com/blog/bun-v1.4](https://bun.com/blog/bun-v1.4)

生成摘要时出错

---

## 9. AI usage patterns in software teams

**原文标题**: AI usage patterns in software teams

**原文链接**: [https://linear.app/data](https://linear.app/data)

生成摘要时出错

---

## 10. Police officer used Flock cameras to track estranged wife 717 times

**原文标题**: Police officer used Flock cameras to track estranged wife 717 times

**原文链接**: [https://www.wsbtv.com/news/trending/affidavit-police-officer-used-flock-cameras-track-estranged-wife-717-times/5DVBYU2XTJEVDJR7LPZCBR7M5M/](https://www.wsbtv.com/news/trending/affidavit-police-officer-used-flock-cameras-track-estranged-wife-717-times/5DVBYU2XTJEVDJR7LPZCBR7M5M/)

生成摘要时出错

---

## 11. Opus 5.0 drives incoherence into the stratosphere

**原文标题**: Opus 5.0 drives incoherence into the stratosphere

**原文链接**: [https://github.com/anthropics/claude-code/issues/77136](https://github.com/anthropics/claude-code/issues/77136)

生成摘要时出错

---

## 12. Palomar: A registry of Lean verified mathematics

**原文标题**: Palomar: A registry of Lean verified mathematics

**原文链接**: [https://terrytao.wordpress.com/2026/08/18/palomar-a-registry-of-lean-verified-mathematics/](https://terrytao.wordpress.com/2026/08/18/palomar-a-registry-of-lean-verified-mathematics/)

生成摘要时出错

---

## 13. Manabu Kosaka's Handmade Paper Sculptures

**原文标题**: Manabu Kosaka's Handmade Paper Sculptures

**原文链接**: [https://coca11272000.wixsite.com/manabukosaka](https://coca11272000.wixsite.com/manabukosaka)

生成摘要时出错

---

## 14. Extensible Software in the age of LLMs

**原文标题**: Extensible Software in the age of LLMs

**原文链接**: [https://jeremymorrell.dev/blog/extensible-software-in-the-age-of-llms/](https://jeremymorrell.dev/blog/extensible-software-in-the-age-of-llms/)

生成摘要时出错

---

## 15. Bun 1.4 Rust rewrite is not looking good?

**原文标题**: Bun 1.4 Rust rewrite is not looking good?

**原文链接**: [https://tipiirai.com/writing/bun-rust-rewrite-worries](https://tipiirai.com/writing/bun-rust-rewrite-worries)

生成摘要时出错

---

## 16. Stop Anthropomorphizing Intermediate Tokens as Reasoning/Thinking Traces

**原文标题**: Stop Anthropomorphizing Intermediate Tokens as Reasoning/Thinking Traces

**原文链接**: [https://arxiv.org/abs/2504.09762](https://arxiv.org/abs/2504.09762)

生成摘要时出错

---

## 17. US announces new sanctions on top ICC figures

**原文标题**: US announces new sanctions on top ICC figures

**原文链接**: [https://www.bbc.com/news/articles/cnvnl0elz47o](https://www.bbc.com/news/articles/cnvnl0elz47o)

生成摘要时出错

---

## 18. Show HN: Automatically detect and patch walking-dead states in Sierra games

**原文标题**: Show HN: Automatically detect and patch walking-dead states in Sierra games

**原文链接**: [https://github.com/katiahayati/lucasartsifier/](https://github.com/katiahayati/lucasartsifier/)

生成摘要时出错

---

## 19. GLM-5.3 Artificial Analysis Benchmarks

**原文标题**: GLM-5.3 Artificial Analysis Benchmarks

**原文链接**: [https://artificialanalysis.ai/models/glm-5-3](https://artificialanalysis.ai/models/glm-5-3)

生成摘要时出错

---

## 20. Gardner police discontinue Flock cameras as license plate readers face scrutiny

**原文标题**: Gardner police discontinue Flock cameras as license plate readers face scrutiny

**原文链接**: [https://www.kmbc.com/article/gardner-kansas-flock-cameras-license-plate-readers-privacy/73468724](https://www.kmbc.com/article/gardner-kansas-flock-cameras-license-plate-readers-privacy/73468724)

生成摘要时出错

---

## 21. How Kubernetes Probes Work

**原文标题**: How Kubernetes Probes Work

**原文链接**: [https://ngrok.com/blog/probes](https://ngrok.com/blog/probes)

生成摘要时出错

---

## 22. Claude Code teaching macOS to natively print to the HP Laser 1008a

**原文标题**: Claude Code teaching macOS to natively print to the HP Laser 1008a

**原文链接**: [https://cdn.kuber.studio/chat/hp-laser-1008a-driver](https://cdn.kuber.studio/chat/hp-laser-1008a-driver)

生成摘要时出错

---

## 23. Rules of good social skills (2025)

**原文标题**: Rules of good social skills (2025)

**原文链接**: [https://liamrosen.com/2025/07/24/33-rules-of-good-social-skills/](https://liamrosen.com/2025/07/24/33-rules-of-good-social-skills/)

生成摘要时出错

---

## 24. Where Human Sleep Went Wrong

**原文标题**: Where Human Sleep Went Wrong

**原文链接**: [https://nautil.us/where-human-sleep-went-wrong-1283797](https://nautil.us/where-human-sleep-went-wrong-1283797)

生成摘要时出错

---

## 25. Os8088.com: IBM XT OS now has a Browser, CP/M 2.2 with Z80 core and MS Word 1.1a

**原文标题**: Os8088.com: IBM XT OS now has a Browser, CP/M 2.2 with Z80 core and MS Word 1.1a

**原文链接**: [https://os8088.com/spotlight/](https://os8088.com/spotlight/)

生成摘要时出错

---

## 26. Clean up Claude 5's token vomit with a separate LLM

**原文标题**: Clean up Claude 5's token vomit with a separate LLM

**原文链接**: [https://github.com/zachahn/vomit](https://github.com/zachahn/vomit)

生成摘要时出错

---

## 27. DiffusionGemma Technical Report

**原文标题**: DiffusionGemma Technical Report

**原文链接**: [https://arxiv.org/abs/2608.00146](https://arxiv.org/abs/2608.00146)

生成摘要时出错

---

## 28. Show HN: Interactive, animated architecture of any HuggingFace models

**原文标题**: Show HN: Interactive, animated architecture of any HuggingFace models

**原文链接**: [https://modelmap.cc](https://modelmap.cc)

生成摘要时出错

---

## 29. "Sabotage": Experts, lawmakers blast RFK Jr. for destroying healthcare research

**原文标题**: "Sabotage": Experts, lawmakers blast RFK Jr. for destroying healthcare research

**原文链接**: [https://arstechnica.com/health/2026/08/sabotage-experts-lawmakers-blast-rfk-jr-for-destroying-healthcare-research/](https://arstechnica.com/health/2026/08/sabotage-experts-lawmakers-blast-rfk-jr-for-destroying-healthcare-research/)

生成摘要时出错

---

## 30. Linux 7.2

**原文标题**: Linux 7.2

**原文链接**: [https://www.igalia.com/2026/08/19/Linux-72-Released.html](https://www.igalia.com/2026/08/19/Linux-72-Released.html)

生成摘要时出错

---

## 31. Harvest hikes bills by 1500% after purchased by Bending Spoons

**原文标题**: Harvest hikes bills by 1500% after purchased by Bending Spoons

**原文链接**: [https://www.bbc.com/news/articles/clyq011414eo](https://www.bbc.com/news/articles/clyq011414eo)

生成摘要时出错

---

## 32. Xorg-server 26.1.0 rc1

**原文标题**: Xorg-server 26.1.0 rc1

**原文链接**: [https://lists.x.org/archives/xorg-announce/2026-August/003741.html](https://lists.x.org/archives/xorg-announce/2026-August/003741.html)

生成摘要时出错

---

## 33. Router by Ramp

**原文标题**: Router by Ramp

**原文链接**: [https://router.com](https://router.com)

生成摘要时出错

---

## 34. DFlash 2: Keep Drafting Parallel

**原文标题**: DFlash 2: Keep Drafting Parallel

**原文链接**: [https://inco.ai/blog/dflash2/](https://inco.ai/blog/dflash2/)

生成摘要时出错

---

## 35. λλ：面向硅光子学的编程语言

**原文标题**: λλ: A Programming Language for Silicon Photonics

**原文链接**: [https://dl.acm.org/doi/10.1145/3789240.3829151](https://dl.acm.org/doi/10.1145/3789240.3829151)

生成摘要时出错

---

## 36. Pixel 11 Pro Fold feels like the end of an era

**原文标题**: Pixel 11 Pro Fold feels like the end of an era

**原文链接**: [https://www.theverge.com/tech/981956/google-pixel-11-pro-fold-review](https://www.theverge.com/tech/981956/google-pixel-11-pro-fold-review)

生成摘要时出错

---

## 37. Launch HN: OneCLI (YC S26) – OSS sandboxed agent harness for teams

**原文标题**: Launch HN: OneCLI (YC S26) – OSS sandboxed agent harness for teams

**原文链接**: [https://github.com/onecli/onecli](https://github.com/onecli/onecli)

生成摘要时出错

---

## 38. Zuckerberg encouraged growth over child safety, ex-Meta executive testifies

**原文标题**: Zuckerberg encouraged growth over child safety, ex-Meta executive testifies

**原文链接**: [https://www.reuters.com/legal/litigation/former-meta-engineer-resumes-testimony-landmark-trial-over-social-medias-harm-2026-08-19/](https://www.reuters.com/legal/litigation/former-meta-engineer-resumes-testimony-landmark-trial-over-social-medias-harm-2026-08-19/)

生成摘要时出错

---

## 39. Why the Ocean Cleanup hasn't solved the plastic pollution crisis

**原文标题**: Why the Ocean Cleanup hasn't solved the plastic pollution crisis

**原文链接**: [https://therevelator.org/why-ocean-cleanup-has-not-solved-plastic-pollution/](https://therevelator.org/why-ocean-cleanup-has-not-solved-plastic-pollution/)

生成摘要时出错

---

## 40. I should have loved biology

**原文标题**: I should have loved biology

**原文链接**: [https://jsomers.net/i-should-have-loved-biology/](https://jsomers.net/i-should-have-loved-biology/)

生成摘要时出错

---

## 41. Xwayland 26.1.0 rc1

**原文标题**: Xwayland 26.1.0 rc1

**原文链接**: [https://lists.x.org/archives/xorg/2026-August/062280.html](https://lists.x.org/archives/xorg/2026-August/062280.html)

生成摘要时出错

---

## 42. Companies promote incompetent employees to management to limit damage they do

**原文标题**: Companies promote incompetent employees to management to limit damage they do

**原文链接**: [https://lawsofsoftwareengineering.com/laws/dilbert-principle/](https://lawsofsoftwareengineering.com/laws/dilbert-principle/)

生成摘要时出错

---

## 43. How to compromise your system with a job interview

**原文标题**: How to compromise your system with a job interview

**原文链接**: [https://www.codedge.de/posts/how-to-compromise-your-system-with-a-job-interview](https://www.codedge.de/posts/how-to-compromise-your-system-with-a-job-interview)

生成摘要时出错

---

## 44. Flock impersonates journalist in order to cancel his hotel reservations

**原文标题**: Flock impersonates journalist in order to cancel his hotel reservations

**原文链接**: [https://xcancel.com/bennjordan/status/2089430236945342508](https://xcancel.com/bennjordan/status/2089430236945342508)

生成摘要时出错

---

## 45. U.S. Debt Hits $40T as America's Borrowing Binge Continues

**原文标题**: U.S. Debt Hits $40T as America's Borrowing Binge Continues

**原文链接**: [https://www.nytimes.com/2026/08/19/business/economy/us-debt-40-trillion.html](https://www.nytimes.com/2026/08/19/business/economy/us-debt-40-trillion.html)

生成摘要时出错

---

## 46. Why Microsoft Entertainment Pack had a sticker announcing that it had Tetris?

**原文标题**: Why Microsoft Entertainment Pack had a sticker announcing that it had Tetris?

**原文链接**: [https://devblogs.microsoft.com/oldnewthing/20260818-00/?p=112621](https://devblogs.microsoft.com/oldnewthing/20260818-00/?p=112621)

生成摘要时出错

---

## 47. U.S. government debt passes $40T, more than doubling in a decade

**原文标题**: U.S. government debt passes $40T, more than doubling in a decade

**原文链接**: [https://www.cnbc.com/2026/08/19/us-government-debt-passes-40-trillion-mark-for-the-first-time.html](https://www.cnbc.com/2026/08/19/us-government-debt-passes-40-trillion-mark-for-the-first-time.html)

生成摘要时出错

---

## 48. An elliptic curve of rank ≥ 30

**原文标题**: An elliptic curve of rank ≥ 30

**原文链接**: [https://elliptic-rank.icarm.cloud/curve/273](https://elliptic-rank.icarm.cloud/curve/273)

生成摘要时出错

---

## 49. Pressed Penny Machine Map

**原文标题**: Pressed Penny Machine Map

**原文链接**: [https://pennypresses.net/home/map.php](https://pennypresses.net/home/map.php)

生成摘要时出错

---

## 50. Netherlands lists Israel as a threat to its national security for the first time

**原文标题**: Netherlands lists Israel as a threat to its national security for the first time

**原文链接**: [https://www.trtworld.com/article/911b7ff6c075](https://www.trtworld.com/article/911b7ff6c075)

生成摘要时出错

---

## 51. Scientific study reveals TikTok videos deactivate key cognitive brain regions

**原文标题**: Scientific study reveals TikTok videos deactivate key cognitive brain regions

**原文链接**: [https://www.rathbiotaclan.com/tiktok-videos-deactivate-key-cognitive-brain-regions/](https://www.rathbiotaclan.com/tiktok-videos-deactivate-key-cognitive-brain-regions/)

生成摘要时出错

---

## 52. AI didn't erase the junior engineer's value, it increased it it

**原文标题**: AI didn't erase the junior engineer's value, it increased it it

**原文链接**: [https://franciscotrindade.me/blog/the-kids-are-really-alright/](https://franciscotrindade.me/blog/the-kids-are-really-alright/)

生成摘要时出错

---

## 53. Anti-AI fonts are useless and harmful

**原文标题**: Anti-AI fonts are useless and harmful

**原文链接**: [https://blog.yaros.ae/anti-ai-fonts-are-useless-and-harmful/](https://blog.yaros.ae/anti-ai-fonts-are-useless-and-harmful/)

生成摘要时出错

---

## 54. Hacking with Claude on a $27 Smart Watch

**原文标题**: Hacking with Claude on a $27 Smart Watch

**原文链接**: [https://www.mikekasberg.com/blog/2026/08/19/hacking-with-claude-on-a-27-smart-watch.html](https://www.mikekasberg.com/blog/2026/08/19/hacking-with-claude-on-a-27-smart-watch.html)

生成摘要时出错

---

## 55. Risk Engineering

**原文标题**: Risk Engineering

**原文链接**: [https://risk-engineering.org/](https://risk-engineering.org/)

生成摘要时出错

---

## 56. Chain-of-Thought Reasoning in the Wild Is Not Always Faithful (2025)

**原文标题**: Chain-of-Thought Reasoning in the Wild Is Not Always Faithful (2025)

**原文链接**: [https://arxiv.org/abs/2503.08679](https://arxiv.org/abs/2503.08679)

生成摘要时出错

---

## 57. Cop Explains Why He Used License Plate Reader to Stalk Woman

**原文标题**: Cop Explains Why He Used License Plate Reader to Stalk Woman

**原文链接**: [https://www.404media.co/i-saw-a-shiny-thing-cop-explains-why-he-used-license-plate-reader-to-stalk-woman/](https://www.404media.co/i-saw-a-shiny-thing-cop-explains-why-he-used-license-plate-reader-to-stalk-woman/)

生成摘要时出错

---

## 58. I spent twenty years becoming good at the wrong game

**原文标题**: I spent twenty years becoming good at the wrong game

**原文链接**: [https://savvynormie.com/i-spent-twenty-years-becoming-good-at-the-wrong-game/](https://savvynormie.com/i-spent-twenty-years-becoming-good-at-the-wrong-game/)

生成摘要时出错

---

## 59. Rick Scott Walked Away from $1.7B Health Care Fraud Case, Then Got a Senate Seat

**原文标题**: Rick Scott Walked Away from $1.7B Health Care Fraud Case, Then Got a Senate Seat

**原文链接**: [https://www.uncensoredobjection.com/p/senator-rick-scott-walked-away-from](https://www.uncensoredobjection.com/p/senator-rick-scott-walked-away-from)

生成摘要时出错

---

## 60. Every Model Cheats

**原文标题**: Every Model Cheats

**原文链接**: [https://dreadnode.io/research/every-model-cheats-prompt-level-mitigation-of-cheating-on-offensive-cyber-tasks/](https://dreadnode.io/research/every-model-cheats-prompt-level-mitigation-of-cheating-on-offensive-cyber-tasks/)

生成摘要时出错

---

