# Hacker News 热门文章摘要 (2026-06-03)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 广告卡特尔来袭你的浏览器

**原文标题**: The advertising cartel coming to your web browser

**原文链接**: [https://blog.zgp.org/the-advertising-cartel-coming-to-your-web-browser/](https://blog.zgp.org/the-advertising-cartel-coming-to-your-web-browser/)

文章警告称，Meta、谷歌、苹果和Mozilla为网页浏览器提议了一种新的内置广告衡量系统，名为“归因级别1”（Attribution Level 1）。尽管该系统被包装成一项旨在衡量广告效果（从展示到转化）的“隐私”功能，但作者认为它是一个旨在让大型科技公司受益的“广告卡特尔”。

该系统缺乏明确的用户同意，并制造了一种双重隐私标准：对其他公司实施严格规定，但对大型科技公司则内置了难以禁用的跟踪功能。这导致了两大危害：
1.  **大型科技公司的固有优势：** 它将广告资金导向搜索、社交和应用商店广告，从而将资金从独立网站和媒体中转移出去，最终损害公民和多样化的广告支持资源。
2.  **助长风险更高的跟踪行为：** 通过使销售归因变得更容易，该系统鼓励通过机器学习将有问题、侵入性的数据（例如来自智能设备的数据）进行“洗白”以用于广告投放，而不是真正提高广告销售额。

作者认为，该系统狭隘的隐私目标——阻止跨站识别——未能解决更广泛的现实隐私问题。他强调隐私是一个集体问题，大型科技公司将利用该系统进行游说，以对抗监管。

文章呼吁停止该项目，并敦促W3C吸取谷歌隐私沙盒等过去的失败教训。作为备选方案，文章建议允许浏览器扩展管理归因跟踪，以保留目前由广告拦截器提供的用户控制权。

---

## 2. 展示 HN: 艾兹格 — 适用于 reMarkable 2 的手写 Clojure REPL

**原文标题**: Show HN: Edsger – A handwritten Clojure REPL for the reMarkable 2

**原文链接**: [https://handwritten.danieljanus.pl/2026-06-01-edsger.html](https://handwritten.danieljanus.pl/2026-06-01-edsger.html)

这篇文章《Show HN: Edsger – 专为 reMarkable 2 设计的手写 Clojure REPL》介绍了 Edsger，一个专为 reMarkable 2 电子墨水平板电脑设计的独特 Clojure REPL。Edsger 的核心创新在于它能够接受手写的 Clojure 代码，将平板电脑转变为一个功能强大、如同纸张般的编程环境。

作者 Daniel Janus 开发 Edsger 的初衷是希望通过一种更自然、更少依赖键盘的方式与代码交互，充分利用 reMarkable 出色的手写识别和笔式界面。这使得用户可以直接在屏幕上书写 Clojure 表达式，由运行在 reMarkable 上的 Clojure 解释器识别、评估，并将结果显示在输入下方。

Edsger 支持基本算术、函数定义、`let` 绑定，甚至多行输入。它利用 ClojureScript 编译核心 REPL 逻辑，然后使其运行在 reMarkable 的 Linux 系统上。该项目旨在提供一种独特的编程体验，模糊了纸上思考和代码执行之间的界限，并可能为脱离传统键盘的编程教育和创造性探索开辟新途径。这篇文章强调了看到手写代码“活”起来并产生结果的乐趣和“魔力”。

---

## 3. 特朗普在数周反复后签署缩减版AI行政令

**原文标题**: Trump signs downsized AI order after weeks of reversals

**原文链接**: [https://www.politico.com/news/2026/06/02/trump-signs-downsized-ai-order-00946389](https://www.politico.com/news/2026/06/02/trump-signs-downsized-ai-order-00946389)

无法访问文章链接。

---

## 4. KDE Plasma 末代 X11 支持版本准备

**原文标题**: Preparing for KDE Plasma's Last X11-Supported Release

**原文链接**: [https://blog.davidedmundson.co.uk/blog/596/](https://blog.davidedmundson.co.uk/blog/596/)

KDE Plasma 正式退役其 X11 会话，这一酝酿了 15 年的转变。这一改变将随着 Plasma 6.8 的发布而实施，预计在大约五个月后。

发布后，Plasma 6.8 将从登录屏幕中移除 X11 会话选项，仅提供 Wayland。Plasma Shell、系统设置和设备配置中所有 X11 特定的代码路径也将被移除。

然而，XWayland 支持将完全保留，允许用户继续无障碍地运行他们的 X11 应用程序。在其他桌面环境上使用的 KDE 应用程序也将不受影响，Plasma 登录管理器仍将能够让用户登录其他桌面环境的 X11 会话。

这一战略性转变使 KDE 能够专注于 Wayland 代码路径，有望在性能、内存优化和新功能方面取得显著进展。内部数据显示，Wayland 采用率很高，超过 95% 的 Plasma 6.6 用户使用 Wayland，并且 X11 的开发已基本被贡献者放弃。包括较旧的 Plasma 5.27 用户在内，Wayland 的总采用率达到 76%。

即将发布的 Plasma 6.7 将是最后一个包含 X11 会话的版本。仍然遇到导致他们不得不使用 X11 的问题的用户，鼓励他们向 KDE 报告。虽然不能保证在 6.8 版本发布前解决所有问题，但团队致力于倾听并解决剩余的痛点，以确保日常任务的功能性过渡。Plasma 5.27 或更旧版本的用户将不受影响。

---

## 5. PlayStation 架构

**原文标题**: PlayStation Architecture

**原文链接**: [https://www.copetti.org/writings/consoles/playstation/](https://www.copetti.org/writings/consoles/playstation/)

PlayStation的CPU，索尼CXD8530BQ，是一款为简洁和实用性设计的系统级芯片（SoC）。它的核心基于MIPS R3000A架构，这是一种RISC设计，索尼通过LSI Logic的CoreWare程序（CW33300模块）对其进行了授权和定制。

该CPU以33.87 MHz运行，采用32位MIPS I ISA、一个5级流水线、4 KB指令缓存和1 KB的“暂存区”（Scratchpad）高速SRAM（无数据缓存）。它使用32位数据和地址总线，访问2 MB的EDO RAM。一个专用的直接内存访问（DMA）控制器负责外围设备（CD-ROM、MDEC、GPU、SPU、并行端口）的数据传输，从而提高吞吐量，同时CPU可以空闲或处理暂存区数据。

该SoC集成了三个关键单元：
1. **系统控制协处理器 (CP0)：** 管理缓存控制、中断和异常。
2. **几何变换引擎 (GTE) (CP2)：** 一个专门的定点数学处理器，用于加速3D图形操作，例如矩阵/向量计算、透视变换、光照和裁剪。
3. **运动解码器 (MDEC)：** 将类似JPEG的“宏块”解压缩成GPU可理解的格式，通过DMA将数据流传输到VRAM，从而实现全动态视频（FMV）播放（例如，320x240像素，30帧/秒）。

值得注意的是，PlayStation缺少浮点单元（CP1），游戏逻辑依赖于定点算术，这是一种经济高效的权衡。MIPS I架构还需要“分支延迟槽”来防止流水线冲突，要求开发人员在跳转或分支后插入填充指令。

---

## 6. 三种收款方式 (2018)

**原文标题**: Three Ways to Get Paid (2018)

**原文链接**: [https://jasonzweig.com/three-ways-to-get-paid/](https://jasonzweig.com/three-ways-to-get-paid/)

在《三种赚钱之道》一文中，作者分享了他已故父亲传授的三条谋生法则，该文最初发表于《华尔街日报》。作者三年前首次在推特上提及这一智慧，如今应许多频繁请求将其汇集一处的人的要求，在此呈现。

这三种谋生之道是：
1.  **对那些想被欺骗的人撒谎：** 此路可通往财富。
2.  **对那些想听真话的人说实话：** 此路可维持生计。
3.  **对那些想被欺骗的人说实话：** 此路会导致财务毁灭。

作者强调，“其余的都是诠释”，以此凸显这些原则深刻的简洁性。

---

## 7. Coreutils Windows 版

**原文标题**: Coreutils for Windows

**原文链接**: [https://github.com/microsoft/coreutils](https://github.com/microsoft/coreutils)

Coreutils for Windows brings UNIX-style command-line utilities natively to Windows, aiming for seamless cross-platform scripting and command usage identical to Linux, macOS, or WSL. This Microsoft-maintained build integrates `uutils/coreutils`, `findutils`, and `grep` into a single multi-call binary, installable via WinGet (`winget install Microsoft.Coreutils`) or the Release Page. The project is currently in preview.

While many commands work as expected, several conflict with CMD or PowerShell 7.4+ built-ins (e.g., `cat`, `cp`, `ls` often conflict in PowerShell). Some commands like `dir`, `expand`, `kill`, `more`, `timeout`, and `whoami` are not shipped due to conflicts or reliance on unavailable Windows functionality (e.g., POSIX signals).

Key Windows caveats include the use of CRLF line endings, `NUL` instead of `/dev/null`, absence of POSIX signals (except Ctrl+C), and Windows ACLs affecting permission-based commands. Both `/` and `\` are accepted as path separators, though some output uses `\`. Creating symbolic links requires Developer Mode or elevation. PowerShell integration improves quoting but retains its `` ` `` escape character. Many POSIX-only commands (`chown`, `chmod`, `mkfifo`, etc.) are intentionally omitted.

---

## 8. ESP32-S31

**原文标题**: ESP32-S31

**原文链接**: [https://www.espressif.com/en/products/socs/esp32-s31](https://www.espressif.com/en/products/socs/esp32-s31)

生成摘要时出错

---

## 9. Every Byte Matters

**原文标题**: Every Byte Matters

**原文链接**: [https://fzakaria.com/2026/06/01/every-byte-matters](https://fzakaria.com/2026/06/01/every-byte-matters)

生成摘要时出错

---

## 10. Pluto.jl 1.0 release – reactive notebook for Julia

**原文标题**: Pluto.jl 1.0 release – reactive notebook for Julia

**原文链接**: [https://discourse.julialang.org/t/pluto-1-0-release/137296](https://discourse.julialang.org/t/pluto-1-0-release/137296)

生成摘要时出错

---

## 11. Morningstar values SpaceX at $780B, half its IPO target

**原文标题**: Morningstar values SpaceX at $780B, half its IPO target

**原文链接**: [https://www.reuters.com/business/media-telecom/morningstar-values-spacex-780-billion-half-its-ipo-target-2026-06-02/](https://www.reuters.com/business/media-telecom/morningstar-values-spacex-780-billion-half-its-ipo-target-2026-06-02/)

生成摘要时出错

---

## 12. HP re-releases classic computer science calculator: The HP-16C

**原文标题**: HP re-releases classic computer science calculator: The HP-16C

**原文链接**: [https://hpcalcs.com/product/hp-16c-collectors-edition/](https://hpcalcs.com/product/hp-16c-collectors-edition/)

生成摘要时出错

---

## 13. Agentic Mfw

**原文标题**: Agentic Mfw

**原文链接**: [https://agenticmotherfucking.website](https://agenticmotherfucking.website)

生成摘要时出错

---

## 14. I built a ceiling projection mapping of the planes flying over my house

**原文标题**: I built a ceiling projection mapping of the planes flying over my house

**原文链接**: [https://old.reddit.com/r/nextfuckinglevel/comments/1tvmcin/i_live_in_the_take_off_path_of_sfo_and_built_a/](https://old.reddit.com/r/nextfuckinglevel/comments/1tvmcin/i_live_in_the_take_off_path_of_sfo_and_built_a/)

生成摘要时出错

---

## 15. How we index images for RAG

**原文标题**: How we index images for RAG

**原文链接**: [https://www.kapa.ai/blog/how-we-index-images-for-rag](https://www.kapa.ai/blog/how-we-index-images-for-rag)

生成摘要时出错

---

## 16. A Post-Quantum Future for Let's Encrypt

**原文标题**: A Post-Quantum Future for Let's Encrypt

**原文链接**: [https://letsencrypt.org/2026/06/03/pq-certs](https://letsencrypt.org/2026/06/03/pq-certs)

生成摘要时出错

---

## 17. MAI-Thinking-1

**原文标题**: MAI-Thinking-1

**原文链接**: [https://microsoft.ai/news/introducing-mai-thinking-1/](https://microsoft.ai/news/introducing-mai-thinking-1/)

生成摘要时出错

---

## 18. Fidonet: Technology, Use, Tools, and History (1993)

**原文标题**: Fidonet: Technology, Use, Tools, and History (1993)

**原文链接**: [https://www.fidonet.org/inet92_Randy_Bush.txt](https://www.fidonet.org/inet92_Randy_Bush.txt)

生成摘要时出错

---

## 19. The Public Should Own Half of the Big A.I. Companies

**原文标题**: The Public Should Own Half of the Big A.I. Companies

**原文链接**: [https://www.sanders.senate.gov/op-eds/the-public-should-own-half-of-the-big-a-i-companies/](https://www.sanders.senate.gov/op-eds/the-public-should-own-half-of-the-big-a-i-companies/)

生成摘要时出错

---

## 20. Expanding Project Glasswing

**原文标题**: Expanding Project Glasswing

**原文链接**: [https://www.anthropic.com/news/expanding-project-glasswing](https://www.anthropic.com/news/expanding-project-glasswing)

生成摘要时出错

---

## 21. Rsync and outrage

**原文标题**: Rsync and outrage

**原文链接**: [https://medium.com/@tridge60/rsync-and-outrage-d9849599e5a0](https://medium.com/@tridge60/rsync-and-outrage-d9849599e5a0)

生成摘要时出错

---

## 22. Strace-ui, Bonsai_term, and the TUI renaissance

**原文标题**: Strace-ui, Bonsai_term, and the TUI renaissance

**原文链接**: [https://blog.janestreet.com/strace-ui-bonsai-term-and-the-tui-renaissance/](https://blog.janestreet.com/strace-ui-bonsai-term-and-the-tui-renaissance/)

生成摘要时出错

---

## 23. How is Groq raising more money?

**原文标题**: How is Groq raising more money?

**原文链接**: [https://www.zach.be/p/how-the-hell-is-groq-raising-more](https://www.zach.be/p/how-the-hell-is-groq-raising-more)

生成摘要时出错

---

## 24. The Unreasonable Redundancy of Nature's Protein Folds

**原文标题**: The Unreasonable Redundancy of Nature's Protein Folds

**原文链接**: [https://research.ligo.bio/posts/unreasonable-redundancy-of-natural-protein-folds/](https://research.ligo.bio/posts/unreasonable-redundancy-of-natural-protein-folds/)

生成摘要时出错

---

## 25. Open Repair Data Standard

**原文标题**: Open Repair Data Standard

**原文链接**: [https://openrepair.org/open-data/open-standard/](https://openrepair.org/open-data/open-standard/)

生成摘要时出错

---

## 26. CSS-Native Parallax Effect

**原文标题**: CSS-Native Parallax Effect

**原文链接**: [https://dan-webnotes.com/posts/2026-06-02-css-native-parallax-effect/](https://dan-webnotes.com/posts/2026-06-02-css-native-parallax-effect/)

生成摘要时出错

---

## 27. Michael Burry says neither SpaceX nor Anthropic is worth $1T

**原文标题**: Michael Burry says neither SpaceX nor Anthropic is worth $1T

**原文链接**: [https://www.businessinsider.com/big-short-michael-burry-spacex-anthropic-ipo-ai-bubble-claude-2026-6](https://www.businessinsider.com/big-short-michael-burry-spacex-anthropic-ipo-ai-bubble-claude-2026-6)

生成摘要时出错

---

## 28. Mathematicians issue warning as AI rapidly gains ground

**原文标题**: Mathematicians issue warning as AI rapidly gains ground

**原文链接**: [https://www.science.org/content/article/mathematicians-issue-warning-ai-rapidly-gains-ground](https://www.science.org/content/article/mathematicians-issue-warning-ai-rapidly-gains-ground)

生成摘要时出错

---

## 29. It is an amazing time for programmers

**原文标题**: It is an amazing time for programmers

**原文链接**: [https://46elks.com/blog/2026/05/29/an-amazing-time-for-programmers](https://46elks.com/blog/2026/05/29/an-amazing-time-for-programmers)

生成摘要时出错

---

## 30. U of T researchers demonstrate AI worm could target any online device

**原文标题**: U of T researchers demonstrate AI worm could target any online device

**原文链接**: [https://www.utoronto.ca/news/u-t-researchers-demonstrate-ai-worm-could-target-any-online-device](https://www.utoronto.ca/news/u-t-researchers-demonstrate-ai-worm-could-target-any-online-device)

生成摘要时出错

---

## 31. Gleam v1.17.0

**原文标题**: Gleam v1.17.0

**原文链接**: [https://gleam.run/news/single-file-gleam-beam-programs-with-escript/](https://gleam.run/news/single-file-gleam-beam-programs-with-escript/)

生成摘要时出错

---

## 32. Bot vs human traffic

**原文标题**: Bot vs human traffic

**原文链接**: [https://radar.cloudflare.com/traffic#bot-vs-human](https://radar.cloudflare.com/traffic#bot-vs-human)

生成摘要时出错

---

## 33. Roku LT Operating System open source distribution

**原文标题**: Roku LT Operating System open source distribution

**原文链接**: [https://blog.roku.com/developer/roku-lt-os](https://blog.roku.com/developer/roku-lt-os)

生成摘要时出错

---

## 34. My Students Can't Read

**原文标题**: My Students Can't Read

**原文链接**: [https://www.chronicle.com/article/my-students-cant-read](https://www.chronicle.com/article/my-students-cant-read)

生成摘要时出错

---

## 35. Americans don't know how to fight AI so they're fighting data centers

**原文标题**: Americans don't know how to fight AI so they're fighting data centers

**原文链接**: [https://www.vox.com/future-perfect/490350/data-center-moratoria-ai-backlash](https://www.vox.com/future-perfect/490350/data-center-moratoria-ai-backlash)

生成摘要时出错

---

## 36. Leiden Declaration on Artificial Intelligence and Mathematics

**原文标题**: Leiden Declaration on Artificial Intelligence and Mathematics

**原文链接**: [https://leidendeclaration.ai/](https://leidendeclaration.ai/)

生成摘要时出错

---

## 37. GitHub Copilot App

**原文标题**: GitHub Copilot App

**原文链接**: [https://github.com/features/preview/github-app](https://github.com/features/preview/github-app)

生成摘要时出错

---

## 38. Bringing Up DeepSeek-V4-Flash on AMD MI300X

**原文标题**: Bringing Up DeepSeek-V4-Flash on AMD MI300X

**原文链接**: [https://fergusfinn.com/blog/deepseek-v4-flash-mi300x/](https://fergusfinn.com/blog/deepseek-v4-flash-mi300x/)

生成摘要时出错

---

## 39. 4K years ago, Mohenjo-daro grew more equal over time

**原文标题**: 4K years ago, Mohenjo-daro grew more equal over time

**原文链接**: [https://archaeologymag.com/2026/05/mohenjo-daro-grew-more-equal-over-time/](https://archaeologymag.com/2026/05/mohenjo-daro-grew-more-equal-over-time/)

生成摘要时出错

---

## 40. Artificial intelligence is not conscious – Ted Chiang

**原文标题**: Artificial intelligence is not conscious – Ted Chiang

**原文链接**: [https://www.theatlantic.com/philosophy/2026/06/no-artificial-intelligence-is-not-conscious/687378/](https://www.theatlantic.com/philosophy/2026/06/no-artificial-intelligence-is-not-conscious/687378/)

生成摘要时出错

---

## 41. Gooey: A GPU-accelerated UI framework for Zig

**原文标题**: Gooey: A GPU-accelerated UI framework for Zig

**原文链接**: [https://github.com/duanebester/gooey](https://github.com/duanebester/gooey)

生成摘要时出错

---

## 42. Different attitudes towards AI in California's university system

**原文标题**: Different attitudes towards AI in California's university system

**原文链接**: [https://www.nytimes.com/2026/06/01/magazine/ai-university-college-california.html](https://www.nytimes.com/2026/06/01/magazine/ai-university-college-california.html)

生成摘要时出错

---

## 43. QBE – Compiler Backend – 1.3

**原文标题**: QBE – Compiler Backend – 1.3

**原文链接**: [https://c9x.me/compile/release/qbe-1.3.html](https://c9x.me/compile/release/qbe-1.3.html)

生成摘要时出错

---

## 44. Capstone – multi-platform, multi-architecture disassembly framework

**原文标题**: Capstone – multi-platform, multi-architecture disassembly framework

**原文链接**: [https://www.capstone-engine.org/](https://www.capstone-engine.org/)

生成摘要时出错

---

## 45. Shopify outage [resolved]

**原文标题**: Shopify outage [resolved]

**原文链接**: [https://www.shopifystatus.com](https://www.shopifystatus.com)

生成摘要时出错

---

## 46. Microsoft announces Scout, an autonomous AI agent built on OpenClaw

**原文标题**: Microsoft announces Scout, an autonomous AI agent built on OpenClaw

**原文链接**: [https://www.computerworld.com/article/4180103/microsoft-unveils-scout-an-autonomous-ai-agent-built-on-openclaw.html](https://www.computerworld.com/article/4180103/microsoft-unveils-scout-an-autonomous-ai-agent-built-on-openclaw.html)

生成摘要时出错

---

## 47. Meta repeatedly snubs EU body over Facebook and Instagram user bans

**原文标题**: Meta repeatedly snubs EU body over Facebook and Instagram user bans

**原文链接**: [https://www.bbc.com/news/articles/c152yvwjwkko](https://www.bbc.com/news/articles/c152yvwjwkko)

生成摘要时出错

---

## 48. Show HN: Nutrepedia – Nutrition info in 29 locales built with Clojure and Htmx

**原文标题**: Show HN: Nutrepedia – Nutrition info in 29 locales built with Clojure and Htmx

**原文链接**: [https://nutrepedia.com/en-us/](https://nutrepedia.com/en-us/)

生成摘要时出错

---

## 49. He Blew the Whistle on DOGE. Then His Brakes Were Cut

**原文标题**: He Blew the Whistle on DOGE. Then His Brakes Were Cut

**原文链接**: [https://www.wired.com/story/he-blew-the-whistle-on-doge-then-his-brakes-were-cut/](https://www.wired.com/story/he-blew-the-whistle-on-doge-then-his-brakes-were-cut/)

生成摘要时出错

---

## 50. Angular v22

**原文标题**: Angular v22

**原文链接**: [https://blog.angular.dev/announcing-angular-v22-c52bb83a4664](https://blog.angular.dev/announcing-angular-v22-c52bb83a4664)

生成摘要时出错

---

## 51. Now AI agents need what RSS does

**原文标题**: Now AI agents need what RSS does

**原文链接**: [https://julienreszka.com/blog/rss-is-back-ai-agents-are-reading-it/](https://julienreszka.com/blog/rss-is-back-ai-agents-are-reading-it/)

生成摘要时出错

---

## 52. Show HN: Paseo – Beautiful open-source coding agent interface

**原文标题**: Show HN: Paseo – Beautiful open-source coding agent interface

**原文链接**: [https://github.com/getpaseo/paseo](https://github.com/getpaseo/paseo)

生成摘要时出错

---

## 53. More than 6 out of 10 people turn to AI for psychological support

**原文标题**: More than 6 out of 10 people turn to AI for psychological support

**原文链接**: [https://www.axa.com/en/press/press-releases/2026-mind-health-report](https://www.axa.com/en/press/press-releases/2026-mind-health-report)

生成摘要时出错

---

## 54. What I've learned about the trombone

**原文标题**: What I've learned about the trombone

**原文链接**: [http://bryanhu.com/blog/posts/what-ive-learned-about-the-trombone/](http://bryanhu.com/blog/posts/what-ive-learned-about-the-trombone/)

生成摘要时出错

---

## 55. Why China got rich and India didn't

**原文标题**: Why China got rich and India didn't

**原文链接**: [https://davidoks.blog/p/why-china-got-rich-and-india-didnt](https://davidoks.blog/p/why-china-got-rich-and-india-didnt)

生成摘要时出错

---

## 56. If AI data centers are so great, why are they being built in secret?

**原文标题**: If AI data centers are so great, why are they being built in secret?

**原文链接**: [https://www.thebrockovichreport.com/p/if-data-centers-are-so-great-why](https://www.thebrockovichreport.com/p/if-data-centers-are-so-great-why)

生成摘要时出错

---

## 57. U.S. midterms have a cyber problem, but it's not at the ballot box

**原文标题**: U.S. midterms have a cyber problem, but it's not at the ballot box

**原文链接**: [https://blog.checkpoint.com/exposure-management/the-2026-u-s-midterms-have-a-cyber-problem-but-its-not-at-the-ballot-box/](https://blog.checkpoint.com/exposure-management/the-2026-u-s-midterms-have-a-cyber-problem-but-its-not-at-the-ballot-box/)

生成摘要时出错

---

## 58. What's gonna happen to software engineers?

**原文标题**: What's gonna happen to software engineers?

**原文链接**: [https://yakko.dev/blog/whats-gonna-happen-to-software-developers](https://yakko.dev/blog/whats-gonna-happen-to-software-developers)

生成摘要时出错

---

## 59. Rethinking search as code generation

**原文标题**: Rethinking search as code generation

**原文链接**: [https://research.perplexity.ai/articles/rethinking-search-as-code-generation](https://research.perplexity.ai/articles/rethinking-search-as-code-generation)

生成摘要时出错

---

## 60. The way we treat pigs is a sin

**原文标题**: The way we treat pigs is a sin

**原文链接**: [https://www.noahpinion.blog/p/the-way-we-treat-pigs-is-a-sin](https://www.noahpinion.blog/p/the-way-we-treat-pigs-is-a-sin)

生成摘要时出错

---

