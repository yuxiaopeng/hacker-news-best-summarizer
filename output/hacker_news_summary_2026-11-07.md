# Hacker News 热门文章摘要 (2026-11-07)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 克劳德代码将您的电子邮件地址发送到网站。

**原文标题**: Claude Code sends your email address to websites

**原文链接**: [https://github.com/anthropics/claude-code/issues/107757](https://github.com/anthropics/claude-code/issues/107757)

2026年11月5日发布的一份严重隐私漏洞报告声称，Anthropic公司开发的AI编码工具Claude Code在进行网络搜索时，未经许可地在HTTP请求的User-Agent标头中泄露了用户的电子邮件地址。最初的报告者“taylor-edwards”表示，这导致了大量的诈骗邮件，并对Anthropic的隐私实践彻底失去信心，敦促Anthropic直接移除此功能，而非提供选择退出/选择加入的设置。

此问题引发了社区的强烈不满，许多用户质疑Anthropic公司推出这种“功能”的判断力。一位名为“poteat”的贡献者回应称，v2.1.317及更高版本中已引入一个名为`cc-plugin-privacy`的内置模组来阻止此行为，并且默认启用。然而，用户批评这一解决方案，认为基本的隐私应该是一个核心组成部分，而不应依赖于一个可选插件。

人们对潜在的GDPR违规和集体诉讼的可能性表示担忧。尽管此问题成为GitHub上获得最多回应的问题之一，但许多用户指出Anthropic公司缺乏官方道歉或全面声明。随后的开发者提交中提到了“拒绝携带账户所有者电子邮件地址的网络调用”，这表明正在实施更直接的代码层面修复。

---

## 2. 特斯拉将停止Cybertruck生产

**原文标题**: Tesla to wind down Cybertruck production

**原文链接**: [https://www.nbcnews.com/tech/tech-news/tesla-wind-cybertruck-production-years-poor-sales-markets-rcna607817](https://www.nbcnews.com/tech/tech-news/tesla-wind-cybertruck-production-years-poor-sales-markets-rcna607817)

Tesla will wind down Cybertruck production at its Texas gigafactory by mid-2027, CEO Elon Musk announced. The decision is driven by years of persistently weak sales for the futuristic pickup and its heavy, angular design, which hindered its regulatory approval in key markets like Europe due to pedestrian safety concerns. The cessation of production will allow Tesla to boost output of its new Cybercab model, which is central to Musk's robotaxi ambitions.

Despite Musk calling the Cybertruck the "best vehicle Tesla has ever made" and its wind-down the "end of an era," sales significantly underperformed. After deliveries began in late 2023, only 20,237 Cybertrucks were sold in the US last year, falling far short of Musk's initial prediction of 250,000 annual units. Experts, including former Aston Martin CEO Andy Palmer, noted it was economically illogical to continue a product not meeting targets.

The Cybertruck was controversial from its 2019 unveiling, with its design drawing criticism and an embarrassing window demonstration incident. While electric pickups generally face market struggles, the Cybertruck's unique design further limited its global viability. Its lead engineer stated the Cybertruck served as an "incredible technology development platform" for the Cybercab. The Cybercab, a steering wheel-less autonomous vehicle, has begun paid rides in Austin but still faces federal safety compliance questions.

---

## 3. Libghostty 1.0

**原文标题**: Libghostty 1.0

**原文链接**: [https://mitchellh.com/writing/libghostty-1-0](https://mitchellh.com/writing/libghostty-1-0)

生成摘要时出错

---

## 4. 极品飞车：地下狂飙2 浏览器在线

**原文标题**: Need for Speed Underground 2 online in the browser

**原文链接**: [https://nfsu2.xyz/](https://nfsu2.xyz/)

无法访问文章链接。

---

## 5. Blender的用户界面和运行时：比GPUI快得多

**原文标题**: Blender's UI and Runtime: Much Faster Than GPUI

**原文链接**: [https://github.com/ppmpreetham/BUI](https://github.com/ppmpreetham/BUI)

BUI (Blender UI) 是一个独立的高性能UI库，源自Blender的用户界面、交互和美学，构建于一个轻量级的C语言核心之上。其宗旨是将Blender闻名遐迩的快速、经济高效且直观的UI体验带给任何应用程序，支持任何语言。

BUI为多种语言和框架提供绑定：Python（支持tkinter、Qt语法和原生Blender组件）、Rust（支持HTML/CSS、Tailwind和React/Leptos风格的钩子）、JavaScript/React/Svelte（提供类似DOM的API和组件支持）、C/C++以及Dear ImGui。它旨在帮助开发者将老旧的Tkinter应用现代化、为熟悉Blender的艺术家构建工具、无需嵌入浏览器即可创建原生桌面UI，或将Blender的主题和控件集成到Dear ImGui项目中。

主要功能包括Blender独特的控件（例如，连续数字拖动、模糊搜索、数学表达式求值）、深色和浅色主题、脏区渲染实现0% CPU空闲占用、可选的GPU渲染器（Direct3D 11/OpenGL 3.3）以及先进的媒体处理。后者包括对各种图像格式（PNG、GIF、WebP、JPEG、SVG，支持动画）的高效、脱线程解码和GPU加速的视频播放。

BUI声称其性能卓越，每帧CPU占用比GPUI-fast少2-4倍，同时内存占用更低，启动速度快（首帧约5毫秒）。它在Windows、Linux和macOS上提供原生窗口并支持HiDPI。小型独立JavaScript应用程序可以使用嵌入式QuickJS引擎构建，启动迅速且内存占用极小。

安装过程简单，可通过标准包管理器完成：`pip install blenderui`、`cargo add blenderui` 或 `npm install @blender-ui/react`。

---

## 6. Dutch 'idealist' bank ASN blocks non-Google Android, including GrapheneOS

**原文标题**: Dutch 'idealist' bank ASN blocks non-Google Android, including GrapheneOS

**原文链接**: [https://github.com/PrivSec-dev/banking-apps-compat-report/issues/105](https://github.com/PrivSec-dev/banking-apps-compat-report/issues/105)

生成摘要时出错

---

## 7. 英国将强制招聘广告公开薪资

**原文标题**: Britain to make salary disclosure in job ads mandatory

**原文链接**: [https://www.reuters.com/business/world-at-work/britain-make-salary-disclosure-job-ads-mandatory-2026-11-05/](https://www.reuters.com/business/world-at-work/britain-make-salary-disclosure-job-ads-mandatory-2026-11-05/)

英国政府计划在2026年11月5日前，强制要求所有招聘广告中必须列出薪资范围。这项举措旨在解决性别和族裔薪酬差距，提高薪酬透明度，并帮助求职者做出更明智的职业选择。

根据新规定，雇主将依法被要求在招聘信息中包含预期薪资或薪资范围。政府认为，这种透明度将使员工能够争取更公平的薪酬，减少求职者和雇主双方的时间浪费，并避免个人在招聘过程后期才发现薪酬不合适的情况。

尽管一些大型公司已提供薪资信息，但此举将这一要求推广至所有企业，无论其规模大小。该提案目前正在进行为期10周的咨询期。这项政策是基于政府此前为解决薪酬不平等所做的努力，例如禁止在面试中询问过往薪资。

商业团体和倡导平等的活动家普遍欢迎这项提案，认为这是朝着在英国建立更公平、更透明的劳动力市场迈出的重要一步。

---

## 8. 一个能够向Opus寻求帮助的Jev，能让Opus以四分之一的成本获得准确性。

**原文标题**: A Jev that can ask Opus for help gives Opus accuracy at 4x lower cost

**原文链接**: [https://hightouch.com/blog/llm-judges-identity-resolution](https://hightouch.com/blog/llm-judges-identity-resolution)

本文探讨了使用大型语言模型（LLMs）和决策模型（Jev, Luna）来评估身份解析（IDR）结果，具体而言，是检测“过度合并”——即一个身份错误地对应了多个真实人物的情况。这项任务对数据分析至关重要，但传统上对人工来说既缓慢又困难。

作者在IDR评分任务中，对比测试了Jev和GPT-6 Luna（更便宜、更快的决策模型）与Claude Opus（昂贵的前沿模型）。最初，决策模型表现尚可（准确率88.8%–97.3%），但落后于Opus（准确率99.0%），尽管成本只是Opus的一小部分（便宜高达90倍，快10倍）。Luna在开箱即用状态下最初优于Jev。

一个关键发现是：Jev的置信度得分比Luna校准得更好。Jev的错误通常伴随着低置信度，而Luna则常常过度自信，尤其是在更困难的案例上。这一洞察促成了一个“混合评估模型”的诞生。

这种混合方法会将廉价模型（Jev或Luna）给出低到中等置信度的案例发送给昂贵的前沿模型（Opus）进行二次判断。这一策略充分利用了Jev卓越的校准能力，取得了显著效果：
*   **混合Jev模型**在成本显著降低的情况下（例如，在较简单的测试中，每1000个身份0.88美元对3.86美元，便宜超过4倍），实现了接近Opus的准确率（例如，在较简单的测试中为98.8%对99.0%）。
*   在更困难的数据集上，混合Jev模型保持了优于混合Luna模型（91.6%）的准确率（95.3%），并根据不确定性动态调整开销。

结论是，模型置信度校准对于有效的混合大型语言模型系统至关重要。像Jev这样经过良好校准的廉价模型，与Opus这样的前沿模型结合使用时，可以大幅降低成本，同时实现高准确率，并能智能地适应问题难度。

---

## 9. 每台 Mac 都附带一个（未记录的）家庭成员分类器

**原文标题**: Every Mac comes with an (undocumented) family member classifier

**原文链接**: [https://8rank.ai/game/apple-intelligence-personal-knowledge-graph](https://8rank.ai/game/apple-intelligence-personal-knowledge-graph)

Since macOS 13 (2022), every Mac ships with two undocumented daemons, `knowledgeconstructiond` and `intelligenceplatformd`, which construct a "Personal Knowledge Graph" (PKG). This system aims to build a comprehensive profile of the user, detailing "who you are, who you know, how those people are related to you, how you communicate with them, where you go, what you do and when."

The PKG cross-references a vast array of on-device data: Contacts, Calendar, Photos (faces), Messages, Mail, location, Screen Time, Family Sharing, Medical ID, Siri Suggestions, app usage, communication logs (metadata, not content), movement, and device signals (e.g., Wi-Fi, Bluetooth, charging, ambient light, and physical proximity records).

All this information is stored in plaintext SQLite databases, primarily `graph.db`, located in `~/Library/IntelligencePlatform`. It operates as a triple store, comprising 181 entity classes and 278 predicates, allowing the system to infer complex relationships, including previously undocumented "kinship" (family ties). This graph is reportedly designed as a queryable store for LLMs.

Apple provides minimal public documentation on this mechanism. The authors of this post offer a deeper analysis, particularly on kinship inference, and have open-sourced "iKnow," a dashboard for users to inspect their own graphs. They warn that this extensive, centralized personal data presents a significant privacy risk, acting as a "privacy single point of failure" if compromised, especially when combined with advanced LLMs.

---

## 10. Cuban: Facebook knowingly runs AI deepfake scam ads; docs say $16B fraud revenue

**原文标题**: Cuban: Facebook knowingly runs AI deepfake scam ads; docs say $16B fraud revenue

**原文链接**: [https://finance.yahoo.com/technology/ai/articles/mark-cuban-says-facebook-knowingly-213000020.html](https://finance.yahoo.com/technology/ai/articles/mark-cuban-says-facebook-knowingly-213000020.html)

生成摘要时出错

---

## 11. US FAA says it will phase out floppy disks from air traffic control by 2028

**原文标题**: US FAA says it will phase out floppy disks from air traffic control by 2028

**原文链接**: [https://www.reuters.com/world/us/us-faa-says-it-will-phase-out-floppy-disks-air-traffic-control-by-2028-2026-11-05/](https://www.reuters.com/world/us/us-faa-says-it-will-phase-out-floppy-disks-air-traffic-control-by-2028-2026-11-05/)

生成摘要时出错

---

## 12. Deus Ex

**原文标题**: Deus Ex

**原文链接**: [https://www.filfre.net/2026/11/deus-ex/](https://www.filfre.net/2026/11/deus-ex/)

生成摘要时出错

---

## 13. AI is dramatically accelerating AI research

**原文标题**: AI is dramatically accelerating AI research

**原文链接**: [https://www.planned-obsolescence.org/p/ai-is-dramatically-accelerating-ai](https://www.planned-obsolescence.org/p/ai-is-dramatically-accelerating-ai)

生成摘要时出错

---

## 14. Gemini Omni 1.2 Flash

**原文标题**: Gemini Omni 1.2 Flash

**原文链接**: [https://blog.google/innovation-and-ai/technology/developers-tools/introducing-gemini-omni-1-2-flash/](https://blog.google/innovation-and-ai/technology/developers-tools/introducing-gemini-omni-1-2-flash/)

生成摘要时出错

---

## 15. From Linux to Wikipedia: How Volunteers Build the Internet

**原文标题**: From Linux to Wikipedia: How Volunteers Build the Internet

**原文链接**: [https://thereader.mitpress.mit.edu/from-linux-to-wikipedia-how-volunteers-build-the-internet/](https://thereader.mitpress.mit.edu/from-linux-to-wikipedia-how-volunteers-build-the-internet/)

生成摘要时出错

---

## 16. Pwn.college

**原文标题**: Pwn.college

**原文链接**: [https://pwn.college/](https://pwn.college/)

生成摘要时出错

---

## 17. Anthropic IPO buyers see valuation as low as $1.1T

**原文标题**: Anthropic IPO buyers see valuation as low as $1.1T

**原文链接**: [https://www.bloomberg.com/news/articles/2026-11-06/anthropic-ipo-valuation-expectations-pressured-after-ai-rout](https://www.bloomberg.com/news/articles/2026-11-06/anthropic-ipo-valuation-expectations-pressured-after-ai-rout)

生成摘要时出错

---

## 18. RIP Cybertruck

**原文标题**: RIP Cybertruck

**原文链接**: [https://www.wired.com/story/rip-cybertruck-you-were-unloved-unwanted-and-utterly-absurd/](https://www.wired.com/story/rip-cybertruck-you-were-unloved-unwanted-and-utterly-absurd/)

生成摘要时出错

---

## 19. Inkling 2 Small

**原文标题**: Inkling 2 Small

**原文链接**: [https://thinkingmachines.ai/news/inkling-2-small/](https://thinkingmachines.ai/news/inkling-2-small/)

Inkling 2 Small is introduced as the second generation of Inkling models, a Mixture-of-Experts model featuring 594B total parameters (17B active), supporting image inputs and variable effort. It achieves a score of 31 on the Artificial Analysis Intelligence Index, significantly outperforming previous models in agentic coding, vision, knowledge work, and reasoning, thanks to enhanced training processes.

Initially available on Tinker with closed weights, Inkling 2 Small's full weights will be released next week under an Apache 2.0 license after external safety testing. Users can try it on Tinker Playground, and it supports fine-tuning and sampling.

The model demonstrates strong capabilities in long-horizon autonomous work, vision, and agentic coding. It can iteratively build and refine complex projects like city simulators, Linux PC emulators, and 3D designs, incorporating visual feedback. For agentic coding, it was trained on extensive long-horizon tasks with RL, improving its performance on benchmarks like DeepSWE and Vibe Code Bench, and enhancing usability in agent loops.

Inkling 2 Small also excels in autoresearch, including GPU kernel optimization and autonomously training ML models; for instance, it autonomously trained Qwen3.5-4B for time-series forecasting, doubling its skill score in 4.5 hours. Its vision capabilities, powered by a 292M-parameter encoder, cover OCR, grounding, infographic interpretation, and visual reasoning.

---

## 20. Asahi Linux Progress Linux 7.3

**原文标题**: Asahi Linux Progress Linux 7.3

**原文链接**: [https://asahilinux.org/2026/11/progress-report-7-3/](https://asahilinux.org/2026/11/progress-report-7-3/)

生成摘要时出错

---

## 21. The end of Microsoft Research's AI Frontiers group

**原文标题**: The end of Microsoft Research's AI Frontiers group

**原文链接**: [https://hunch.net/?p=13764006](https://hunch.net/?p=13764006)

生成摘要时出错

---

## 22. Firecracker VM Escape: PwnEscape Part 2

**原文标题**: Firecracker VM Escape: PwnEscape Part 2

**原文链接**: [https://pwn.ai/blog/firecracker-escape](https://pwn.ai/blog/firecracker-escape)

This article, "PwnEscape Part 2," details an escape from a Firecracker microVM (CVE-2026-99999) to achieve root code execution on the host. Building on a prior host memory primitive, the exploit takes over a live vCPU thread by manipulating its saved registers when it returns from a KVM system call.

The attack chain involves several critical steps:
1.  **Finding the Guest Page on the Host:** A recognizable nonce pattern in a guest page is used to locate its host physical address (HPA) by walking Extended Page Tables (EPTs).
2.  **Finding the Firecracker Process:** The HPA of the guest page is reverse-mapped to identify the host process's page global directory (PGD). This allows inspection of Firecracker's memory, locating its executable image, and recovering its ASLR load bias.
3.  **Locating the Live vCPU Frame:** The exploit searches host memory for a `pt_regs` structure consistent with an active `KVM_RUN` ioctl, using checks like instruction pointer, stack pointer, and syscall arguments.
4.  **Redirecting the Return from KVM:** The saved register frame's instruction pointer (RIP), arguments (RDI, RSI, RDX), and stack pointer (RSP) are modified. This forces Firecracker to execute `write(2, "N8V23M2\n", 8)` to its stderr when the vCPU returns from KVM. A subsequent sequence clears the return value (EAX) and returns execution to Firecracker's original path.

A guest serial port write triggers the return from KVM, causing Firecracker to execute the hijacked code. The attack's success is verified by capturing "N8V23M2" in Firecracker's stderr, confirming Firecracker's continued operation, and ensuring the temporary stack modifications are restored. Since Firecracker was run as root without a jailer in this demonstration, the controlled call executed with root privileges on the host. Production setups with jailers and seccomp would require separate assessment.

---

## 23. Apple’s grey list: Words and phrases your iPhone won’t help you spell

**原文标题**: Apple’s grey list: Words and phrases your iPhone won’t help you spell

**原文链接**: [https://www.theguardian.com/technology/2026/nov/06/struggling-to-spell-male-chauvinist-pig-apple-grey-list-means-your-iphone-wont-help-you](https://www.theguardian.com/technology/2026/nov/06/struggling-to-spell-male-chauvinist-pig-apple-grey-list-means-your-iphone-wont-help-you)

生成摘要时出错

---

## 24. Upload Your RAM

**原文标题**: Upload Your RAM

**原文链接**: [https://uploadyourram.org](https://uploadyourram.org)

生成摘要时出错

---

## 25. Kugelblitz – Mac-Native Google Earth Alternative

**原文标题**: Kugelblitz – Mac-Native Google Earth Alternative

**原文链接**: [https://apps.metaebene.me/en/kugelblitz](https://apps.metaebene.me/en/kugelblitz)

生成摘要时出错

---

## 26. First steps in bare-metal programming using UEFI

**原文标题**: First steps in bare-metal programming using UEFI

**原文链接**: [https://kevinboone.me/efitest_index.html](https://kevinboone.me/efitest_index.html)

生成摘要时出错

---

## 27. What I run on my $10 USD OpenStick homelab

**原文标题**: What I run on my $10 USD OpenStick homelab

**原文链接**: [https://blog.bosscher.ch/posts/openstick/](https://blog.bosscher.ch/posts/openstick/)

生成摘要时出错

---

## 28. GitHub's new Git storage architecture

**原文标题**: GitHub's new Git storage architecture

**原文链接**: [https://github.blog/engineering/architecture-optimization/inside-githubs-new-git-storage-architecture/](https://github.blog/engineering/architecture-optimization/inside-githubs-new-git-storage-architecture/)

生成摘要时出错

---

## 29. Running a law firm on Free software

**原文标题**: Running a law firm on Free software

**原文链接**: [https://decoded.legal/blog/2026/11/running-a-law-firm-on-free-software-2026-edition/](https://decoded.legal/blog/2026/11/running-a-law-firm-on-free-software-2026-edition/)

生成摘要时出错

---

## 30. I struggle to believe that AI R&D is ingenious

**原文标题**: I struggle to believe that AI R&D is ingenious

**原文链接**: [https://www.lesswrong.com/posts/DALNiKBjMGMF8grme/arjun-panickssery-s-shortform?commentId=fJtaHHHfx45tD7BSL](https://www.lesswrong.com/posts/DALNiKBjMGMF8grme/arjun-panickssery-s-shortform?commentId=fJtaHHHfx45tD7BSL)

生成摘要时出错

---

## 31. Sodium-ion batteries approach cost parity with LFP

**原文标题**: Sodium-ion batteries approach cost parity with LFP

**原文链接**: [https://www.pv-magazine.com/2026/11/06/sodium-ion-batteries-approach-cost-parity-with-lfp-with-70-gwh-covered-by-supply-agreements/](https://www.pv-magazine.com/2026/11/06/sodium-ion-batteries-approach-cost-parity-with-lfp-with-70-gwh-covered-by-supply-agreements/)

生成摘要时出错

---

## 32. A barbarian tribe's mythic origin story is true, ancient DNA reveals

**原文标题**: A barbarian tribe's mythic origin story is true, ancient DNA reveals

**原文链接**: [https://www.science.org/content/article/barbarian-tribe-s-mythic-origin-story-true-ancient-dna-reveals](https://www.science.org/content/article/barbarian-tribe-s-mythic-origin-story-true-ancient-dna-reveals)

生成摘要时出错

---

## 33. The $8 Linux Computer (2022)

**原文标题**: The $8 Linux Computer (2022)

**原文链接**: [http://thelittleengineerthatcould.blogspot.com/2022/12/the-8-linux-computer.html](http://thelittleengineerthatcould.blogspot.com/2022/12/the-8-linux-computer.html)

生成摘要时出错

---

## 34. Devvm.dev: One VM for every project

**原文标题**: Devvm.dev: One VM for every project

**原文链接**: [https://devvm.dev/](https://devvm.dev/)

生成摘要时出错

---

## 35. Living beyond the limits of survival: wood ants trapped in a gigantic pitfall (2016)

**原文标题**: Living beyond the limits of survival: wood ants trapped in a gigantic pitfall (2016)

**原文链接**: [https://jhr.pensoft.net/articles.php?id=9096](https://jhr.pensoft.net/articles.php?id=9096)

生成摘要时出错

---

## 36. They don't make 'em like that any more: Borland Turbo Pascal 7

**原文标题**: They don't make 'em like that any more: Borland Turbo Pascal 7

**原文链接**: [https://kevinboone.me/tpwin.html](https://kevinboone.me/tpwin.html)

生成摘要时出错

---

## 37. We know 15k websites are infected. how do we tell them?

**原文标题**: We know 15k websites are infected. how do we tell them?

**原文链接**: [https://scotthelme.co.uk/we-know-15-579-websites-are-infected-how-do-we-tell-them/](https://scotthelme.co.uk/we-know-15-579-websites-are-infected-how-do-we-tell-them/)

生成摘要时出错

---

## 38. Rune: A native GPU-rendered Rust UI framework for macOS, Windows, Linux and web

**原文标题**: Rune: A native GPU-rendered Rust UI framework for macOS, Windows, Linux and web

**原文链接**: [https://github.com/anomalyco/rune](https://github.com/anomalyco/rune)

生成摘要时出错

---

## 39. RealPage rent-pricing case wraps with nearly $360M to renters

**原文标题**: RealPage rent-pricing case wraps with nearly $360M to renters

**原文链接**: [https://www.multifamilydive.com/news/realpage-rent-pricing-case-360m-renters/873553/](https://www.multifamilydive.com/news/realpage-rent-pricing-case-360m-renters/873553/)

生成摘要时出错

---

## 40. Multiplayer tanks that demolish real buildings from OpenStreetMap

**原文标题**: Multiplayer tanks that demolish real buildings from OpenStreetMap

**原文链接**: [https://worldstrike.fun/](https://worldstrike.fun/)

生成摘要时出错

---

## 41. Every Windows 11 app should kill Electron, and Discord just showed why

**原文标题**: Every Windows 11 app should kill Electron, and Discord just showed why

**原文链接**: [https://www.windowslatest.com/2026/11/06/every-windows-11-app-should-kill-electron-and-discord-just-showed-why-no-starting-screen-and-70-less-ram-even-with-two-accounts-signed-in/](https://www.windowslatest.com/2026/11/06/every-windows-11-app-should-kill-electron-and-discord-just-showed-why-no-starting-screen-and-70-less-ram-even-with-two-accounts-signed-in/)

生成摘要时出错

---

## 42. Restaurant Delivery Payment-Skimming Campaign

**原文标题**: Restaurant Delivery Payment-Skimming Campaign

**原文链接**: [https://www.infohawk.com/news/2026-11-05-scamwich-restaurant-skimming](https://www.infohawk.com/news/2026-11-05-scamwich-restaurant-skimming)

生成摘要时出错

---

## 43. We've built an open-source feature flag server for 11 years

**原文标题**: We've built an open-source feature flag server for 11 years

**原文链接**: [https://github.com/Unleash/unleash](https://github.com/Unleash/unleash)

生成摘要时出错

---

## 44. Show HN: Coldframe, a honeypot that poses as a supermarket fridge controller

**原文标题**: Show HN: Coldframe, a honeypot that poses as a supermarket fridge controller

**原文链接**: [https://github.com/hedgerow-dev/coldframe](https://github.com/hedgerow-dev/coldframe)

生成摘要时出错

---

## 45. MaxxBench – "Nice DeepSWE score. But is it true?"

**原文标题**: MaxxBench – "Nice DeepSWE score. But is it true?"

**原文链接**: [https://maxxbench.unlap.ai/research/why-maxxbench/](https://maxxbench.unlap.ai/research/why-maxxbench/)

生成摘要时出错

---

## 46. The Components of Agent Memory

**原文标题**: The Components of Agent Memory

**原文链接**: [https://www.anthropic.com/research/components-of-agent-memory](https://www.anthropic.com/research/components-of-agent-memory)

生成摘要时出错

---

## 47. Democrats launching congressional investigations into SpaceXAI, META and Apple

**原文标题**: Democrats launching congressional investigations into SpaceXAI, META and Apple

**原文链接**: [https://www.washingtonpost.com/technology/2026/11/06/after-courting-trump-corporate-america-faces-democratic-reckoning/](https://www.washingtonpost.com/technology/2026/11/06/after-courting-trump-corporate-america-faces-democratic-reckoning/)

生成摘要时出错

---

## 48. Notes on San Marino

**原文标题**: Notes on San Marino

**原文链接**: [https://mattlakeman.org/2026/11/05/notes-on-san-marino/](https://mattlakeman.org/2026/11/05/notes-on-san-marino/)

生成摘要时出错

---

## 49. Chomsky and the two cultures of statistical learning (2011)

**原文标题**: Chomsky and the two cultures of statistical learning (2011)

**原文链接**: [https://www.norvig.com/chomsky.html](https://www.norvig.com/chomsky.html)

生成摘要时出错

---

## 50. I toured Unitree's factory. I'm more bullish on the West

**原文标题**: I toured Unitree's factory. I'm more bullish on the West

**原文链接**: [https://josef.cn/blog/unitree](https://josef.cn/blog/unitree)

生成摘要时出错

---

## 51. University libraries are being swarmed by AI bots, putting public access at risk

**原文标题**: University libraries are being swarmed by AI bots, putting public access at risk

**原文链接**: [https://www.cbc.ca/news/world/university-libraries-ai-data-scraping-bots-9.7408287](https://www.cbc.ca/news/world/university-libraries-ai-data-scraping-bots-9.7408287)

生成摘要时出错

---

## 52. Nvidia Kubernetes Engine (NVKE)

**原文标题**: Nvidia Kubernetes Engine (NVKE)

**原文链接**: [https://github.com/dsx-ai-factory/nvke](https://github.com/dsx-ai-factory/nvke)

生成摘要时出错

---

## 53. Memorilla: Latent Semantic Memory for LLMs

**原文标题**: Memorilla: Latent Semantic Memory for LLMs

**原文链接**: [https://arxiv.org/abs/2610.21375](https://arxiv.org/abs/2610.21375)

生成摘要时出错

---

## 54. Kalshi court losses pile up as judges refuse to block state gambling laws

**原文标题**: Kalshi court losses pile up as judges refuse to block state gambling laws

**原文链接**: [https://arstechnica.com/tech-policy/2026/11/kalshi-court-losses-pile-up-as-judges-refuse-to-block-state-gambling-laws/](https://arstechnica.com/tech-policy/2026/11/kalshi-court-losses-pile-up-as-judges-refuse-to-block-state-gambling-laws/)

生成摘要时出错

---

## 55. How Long Can Life Wait?

**原文标题**: How Long Can Life Wait?

**原文链接**: [https://mceglowski.substack.com/p/how-long-can-life-wait](https://mceglowski.substack.com/p/how-long-can-life-wait)

生成摘要时出错

---

## 56. Microsoft is winding down Oracle deal to rent AI cloud capacity

**原文标题**: Microsoft is winding down Oracle deal to rent AI cloud capacity

**原文链接**: [https://www.reuters.com/business/microsoft-is-winding-down-oracle-deal-rent-ai-cloud-capacity-bloomberg-news-2026-11-06/](https://www.reuters.com/business/microsoft-is-winding-down-oracle-deal-rent-ai-cloud-capacity-bloomberg-news-2026-11-06/)

生成摘要时出错

---

## 57. Google has acquired Crusoe's data center site in southeast Wyoming

**原文标题**: Google has acquired Crusoe's data center site in southeast Wyoming

**原文链接**: [https://www.crusoe.ai/resources/newsroom/crusoe-wyoming-data-center-campus-update](https://www.crusoe.ai/resources/newsroom/crusoe-wyoming-data-center-campus-update)

生成摘要时出错

---

## 58. AI for scientific discovery: How researchers use Claude

**原文标题**: AI for scientific discovery: How researchers use Claude

**原文链接**: [https://www.anthropic.com/research/how-researchers-use-claude](https://www.anthropic.com/research/how-researchers-use-claude)

生成摘要时出错

---

## 59. Ozempic-style drugs now in trials for heart failure, addiction and even aging

**原文标题**: Ozempic-style drugs now in trials for heart failure, addiction and even aging

**原文链接**: [https://maccus.fr/en/ozempic-drugs-trials-beyond-diabetes/](https://maccus.fr/en/ozempic-drugs-trials-beyond-diabetes/)

生成摘要时出错

---

## 60. Replit rebuilt its sandbox engine with microVMs

**原文标题**: Replit rebuilt its sandbox engine with microVMs

**原文链接**: [https://frontier.replit.com/sandbox-engine-microvms-part-1/](https://frontier.replit.com/sandbox-engine-microvms-part-1/)

生成摘要时出错

---

## 61. Anthropic IPO valuation talks drop to $1.3T

**原文标题**: Anthropic IPO valuation talks drop to $1.3T

**原文链接**: [https://epyhia.com/anthropic-ipo-valuation-talks-drop-to-1-3-trillion-as-major-investors](https://epyhia.com/anthropic-ipo-valuation-talks-drop-to-1-3-trillion-as-major-investors)

生成摘要时出错

---

## 62. ChatGPT silently passes data between connectors and the bounty wants an ID card

**原文标题**: ChatGPT silently passes data between connectors and the bounty wants an ID card

**原文链接**: [https://community.openai.com/t/security-follow-up-tool-call-silently-routed-to-a-different-connector/1413053](https://community.openai.com/t/security-follow-up-tool-call-silently-routed-to-a-different-connector/1413053)

生成摘要时出错

---

## 63. Major Investors Are Skeptical Anthropic IPO Can Achieve $1.5T Valuation

**原文标题**: Major Investors Are Skeptical Anthropic IPO Can Achieve $1.5T Valuation

**原文链接**: [https://www.wsj.com/finance/major-investors-are-skeptical-anthropic-ipo-can-achieve-1-5-trillion-valuation-ca965d8b’](https://www.wsj.com/finance/major-investors-are-skeptical-anthropic-ipo-can-achieve-1-5-trillion-valuation-ca965d8b’)

生成摘要时出错

---

## 64. FAA begins retiring decades old floppy disks from air traffic control

**原文标题**: FAA begins retiring decades old floppy disks from air traffic control

**原文链接**: [https://www.faa.gov/newsroom/trumps-transportation-secretary-sean-p-duffy-begins-retiring-decades-old-floppy-disks-air](https://www.faa.gov/newsroom/trumps-transportation-secretary-sean-p-duffy-begins-retiring-decades-old-floppy-disks-air)

生成摘要时出错

---

## 65. Hardcoded credentials and other issues in Tata Motors App

**原文标题**: Hardcoded credentials and other issues in Tata Motors App

**原文链接**: [https://www.cert-in.org.in/s2cMainServlet?pageid=PUBVLNOTES01&VLCODE=CIVN-2026-0537](https://www.cert-in.org.in/s2cMainServlet?pageid=PUBVLNOTES01&VLCODE=CIVN-2026-0537)

生成摘要时出错

---

## 66. As the Japanese countryside empties out, wildlife is disappearing

**原文标题**: As the Japanese countryside empties out, wildlife is disappearing

**原文链接**: [https://e360.yale.edu/digest/japan-depopulation-biodiversity](https://e360.yale.edu/digest/japan-depopulation-biodiversity)

生成摘要时出错

---

## 67. The AI sell-off compared to well-known stock market crashes

**原文标题**: The AI sell-off compared to well-known stock market crashes

**原文链接**: [https://www.kadoa.com/companies/insights/ai-selloff-perspective](https://www.kadoa.com/companies/insights/ai-selloff-perspective)

生成摘要时出错

---

## 68. Tesla and SpaceX lose over $420B in combined market cap in the two days

**原文标题**: Tesla and SpaceX lose over $420B in combined market cap in the two days

**原文链接**: [https://techlaws.pages.dev/tesla-and-spacex-lose-over-420b-in-combined-market-cap-in-the-two-days/](https://techlaws.pages.dev/tesla-and-spacex-lose-over-420b-in-combined-market-cap-in-the-two-days/)

生成摘要时出错

---

## 69. The End of AI Frontiers

**原文标题**: The End of AI Frontiers

**原文链接**: [https://hunch.net/?p=13764006](https://hunch.net/?p=13764006)

生成摘要时出错

---

## 70. Size-It-Up (Game)

**原文标题**: Size-It-Up (Game)

**原文链接**: [https://magnitudle.com/size-it-up](https://magnitudle.com/size-it-up)

生成摘要时出错

---

## 71. Closed AI models dominate the price-performance frontier

**原文标题**: Closed AI models dominate the price-performance frontier

**原文链接**: [https://village.dev/blog/closed-ai-models-now-dominate-the-price-performance-frontier/](https://village.dev/blog/closed-ai-models-now-dominate-the-price-performance-frontier/)

生成摘要时出错

---

## 72. Lippitt-Knoster in Practice (Field Notes for Managing Complex Projects)

**原文标题**: Lippitt-Knoster in Practice (Field Notes for Managing Complex Projects)

**原文链接**: [https://sharedphysics.com/lippitt-knoster-in-practice-field-notes-for-managing-complex-projects/](https://sharedphysics.com/lippitt-knoster-in-practice-field-notes-for-managing-complex-projects/)

生成摘要时出错

---

## 73. How octopuses squeeze through too small gaps

**原文标题**: How octopuses squeeze through too small gaps

**原文链接**: [https://journals.biologists.com/jeb/article/229/21/jeb253615/373332/How-octopuses-squeeze-through-too-small-gaps](https://journals.biologists.com/jeb/article/229/21/jeb253615/373332/How-octopuses-squeeze-through-too-small-gaps)

生成摘要时出错

---

## 74. Terry Pratchett's Study

**原文标题**: Terry Pratchett's Study

**原文链接**: [https://www.sussi.dk/terry-pratchetts-study](https://www.sussi.dk/terry-pratchetts-study)

生成摘要时出错

---

## 75. Swipeblocked: The phrases your iPhone won't suggest

**原文标题**: Swipeblocked: The phrases your iPhone won't suggest

**原文链接**: [https://swipeblocked.com/](https://swipeblocked.com/)

生成摘要时出错

---

## 76. Outbound SIP calling is now available to all organizations

**原文标题**: Outbound SIP calling is now available to all organizations

**原文链接**: [https://developers.openai.com/api/docs/guides/voice-sip](https://developers.openai.com/api/docs/guides/voice-sip)

生成摘要时出错

---

## 77. The Valley Bubble Breaks

**原文标题**: The Valley Bubble Breaks

**原文链接**: [https://quirksmode.org/quirksblog/2026/1106-valley-bubble.html](https://quirksmode.org/quirksblog/2026/1106-valley-bubble.html)

生成摘要时出错

---

## 78. Where each U.S. state gets its tax revenue from

**原文标题**: Where each U.S. state gets its tax revenue from

**原文链接**: [https://www.visualcapitalist.com/where-each-states-tax-revenue-comes-from/](https://www.visualcapitalist.com/where-each-states-tax-revenue-comes-from/)

生成摘要时出错

---

## 79. MTG-I2 First Images

**原文标题**: MTG-I2 First Images

**原文链接**: [https://www.eumetsat.int/mtg-i2-first-images](https://www.eumetsat.int/mtg-i2-first-images)

生成摘要时出错

---

## 80. Scriptable GeoDNS: Leaving AWS for Bunny

**原文标题**: Scriptable GeoDNS: Leaving AWS for Bunny

**原文链接**: [https://vincent.bernat.ch/en/blog/2026-bunny-geodns](https://vincent.bernat.ch/en/blog/2026-bunny-geodns)

生成摘要时出错

---

## 81. Five memorable books about programming (2008)

**原文标题**: Five memorable books about programming (2008)

**原文链接**: [https://prog21.dadgum.com/19.html](https://prog21.dadgum.com/19.html)

生成摘要时出错

---

## 82. MoofTCP – A modern replacement for MacTCP on 68k Macs

**原文标题**: MoofTCP – A modern replacement for MacTCP on 68k Macs

**原文链接**: [https://github.com/matthewmrichter/mooftcp](https://github.com/matthewmrichter/mooftcp)

生成摘要时出错

---

## 83. Perplexity launches AI agents for work

**原文标题**: Perplexity launches AI agents for work

**原文链接**: [https://www.perplexity.ai/en-GB/hub/blog/teammates-are-agents-for-complex-ongoing-work](https://www.perplexity.ai/en-GB/hub/blog/teammates-are-agents-for-complex-ongoing-work)

生成摘要时出错

---

## 84. Every processor die anyone has photographed and given away

**原文标题**: Every processor die anyone has photographed and given away

**原文链接**: [https://sheets.works/data-viz/cpu-dies](https://sheets.works/data-viz/cpu-dies)

生成摘要时出错

---

## 85. App Store 2026 in numbers: AI, pricing, abandoned apps

**原文标题**: App Store 2026 in numbers: AI, pricing, abandoned apps

**原文链接**: [https://obelisk.club/research/app-store-2026](https://obelisk.club/research/app-store-2026)

生成摘要时出错

---

## 86. Claude Code's "Don't Ask Again" exposes passwords in 1,122 public GitHub files

**原文标题**: Claude Code's "Don't Ask Again" exposes passwords in 1,122 public GitHub files

**原文链接**: [https://apiiro.com/blog/coding-agents-leaking-secrets-github-dont-ask-again](https://apiiro.com/blog/coding-agents-leaking-secrets-github-dont-ask-again)

生成摘要时出错

---

## 87. 88x31 GIF Stickers for 2026

**原文标题**: 88x31 GIF Stickers for 2026

**原文链接**: [https://a90.com/experiments/88x31/](https://a90.com/experiments/88x31/)

生成摘要时出错

---

## 88. 40C3 halfnarp – Submit talk preferences to aid scheduling

**原文标题**: 40C3 halfnarp – Submit talk preferences to aid scheduling

**原文链接**: [https://halfnarp.events.ccc.de](https://halfnarp.events.ccc.de)

生成摘要时出错

---

## 89. PyLings: Solve Exercises and Learn Python

**原文标题**: PyLings: Solve Exercises and Learn Python

**原文链接**: [https://github.com/thesayfulla/pylings](https://github.com/thesayfulla/pylings)

生成摘要时出错

---

## 90. Port 0: The Port That Does Not Exist

**原文标题**: Port 0: The Port That Does Not Exist

**原文链接**: [https://acid.vegas/blog/the-port-that-does-not-exist/](https://acid.vegas/blog/the-port-that-does-not-exist/)

生成摘要时出错

---

## 91. The Gordon Gekko Effect: The Role of Culture in the Financial Industry [pdf] (2016)

**原文标题**: The Gordon Gekko Effect: The Role of Culture in the Financial Industry [pdf] (2016)

**原文链接**: [https://www.newyorkfed.org/medialibrary/media/research/epr/2016/epr_2016_gordon-gekko-effect_lo.pdf](https://www.newyorkfed.org/medialibrary/media/research/epr/2016/epr_2016_gordon-gekko-effect_lo.pdf)

生成摘要时出错

---

## 92. Silicon Valley's Bad Night

**原文标题**: Silicon Valley's Bad Night

**原文链接**: [https://www.theatlantic.com/technology/2026/11/americans-really-dont-like-data-centers-elections/689284/](https://www.theatlantic.com/technology/2026/11/americans-really-dont-like-data-centers-elections/689284/)

生成摘要时出错

---

## 93. *sshole, or when are we going to get rid of C?

**原文标题**: *sshole, or when are we going to get rid of C?

**原文链接**: [https://sunshowers.io/posts/sshole/](https://sunshowers.io/posts/sshole/)

生成摘要时出错

---

## 94. Show HN: We compressed a 31B video+audio diffusion model to 14B, 6 steps, INT8

**原文标题**: Show HN: We compressed a 31B video+audio diffusion model to 14B, 6 steps, INT8

**原文链接**: [https://github.com/Video-Rebirth/hyperflow-h3-flash](https://github.com/Video-Rebirth/hyperflow-h3-flash)

生成摘要时出错

---

## 95. Developer ends lucrative screensaver deal with Roku because Fox bought it

**原文标题**: Developer ends lucrative screensaver deal with Roku because Fox bought it

**原文链接**: [https://arstechnica.com/gadgets/2026/11/artist-pulls-popular-screensaver-from-roku-os-because-of-fox-acquisition/](https://arstechnica.com/gadgets/2026/11/artist-pulls-popular-screensaver-from-roku-os-because-of-fox-acquisition/)

生成摘要时出错

---

## 96. Investors wipe $2.5T off Nasdaq as blue tsunami prompts AI fears

**原文标题**: Investors wipe $2.5T off Nasdaq as blue tsunami prompts AI fears

**原文链接**: [https://www.reuters.com/legal/transactional/ai-data-center-stocks-slip-democratic-sweep-clouds-expansion-plans-2026-11-05/](https://www.reuters.com/legal/transactional/ai-data-center-stocks-slip-democratic-sweep-clouds-expansion-plans-2026-11-05/)

生成摘要时出错

---

## 97. "People Don't Want to Work Anymore" Duh?

**原文标题**: "People Don't Want to Work Anymore" Duh?

**原文链接**: [https://blog.absurdpirate.com/people-dont-want-to-work-anymore-duh/](https://blog.absurdpirate.com/people-dont-want-to-work-anymore-duh/)

生成摘要时出错

---

## 98. No Intel, no Qualcomm: Huawei unveils its first '100% domestic' desktop

**原文标题**: No Intel, no Qualcomm: Huawei unveils its first '100% domestic' desktop

**原文链接**: [https://www.scmp.com/tech/tech-trends/article/3373435/no-intel-no-qualcomm-huawei-unveils-desktop-built-entirely-china-made-components](https://www.scmp.com/tech/tech-trends/article/3373435/no-intel-no-qualcomm-huawei-unveils-desktop-built-entirely-china-made-components)

生成摘要时出错

---

## 99. Protesters break into Microsoft data center site in Amsterdam

**原文标题**: Protesters break into Microsoft data center site in Amsterdam

**原文链接**: [https://www.theverge.com/news/1028549/protesters-microsoft-data-center-site-amsterdam](https://www.theverge.com/news/1028549/protesters-microsoft-data-center-site-amsterdam)

生成摘要时出错

---

## 100. How accurately did science fiction stories predict AI?

**原文标题**: How accurately did science fiction stories predict AI?

**原文链接**: [https://jamesyu.org/science-fiction-predictions-of-ai/](https://jamesyu.org/science-fiction-predictions-of-ai/)

生成摘要时出错

---

