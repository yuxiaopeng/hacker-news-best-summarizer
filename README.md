# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-06-03.md)

*最后自动更新时间: 2026-06-03 22:17:09*
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

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 2 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 3 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 4 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 5 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 6 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 7 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 8 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 9 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 10 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 11 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 12 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 13 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 14 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 15 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 16 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 17 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 18 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 19 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 20 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 21 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 22 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 23 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 24 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 25 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 26 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 27 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 28 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 29 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 30 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 31 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 32 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 33 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 34 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 35 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 36 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 37 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 38 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 39 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 40 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 41 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 42 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 43 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 44 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 45 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 46 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 47 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 48 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 49 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 50 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 51 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 52 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 53 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 54 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 55 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 56 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 57 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 58 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 59 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 60 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 61 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 62 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 63 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 64 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 65 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 66 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 67 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 68 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 69 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 70 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 71 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 72 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 73 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 74 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 75 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 76 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 77 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 78 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 79 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 80 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 81 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 82 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 83 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 84 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 85 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 86 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 87 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 88 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 89 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 90 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 91 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 92 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 93 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 94 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 95 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 96 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 97 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 98 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 99 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 100 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 101 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 102 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 103 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 104 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 105 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 106 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 107 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 108 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 109 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 110 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 111 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 112 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 113 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 114 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 115 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 116 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 117 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 118 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 119 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 120 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 121 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 122 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 123 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 124 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 125 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 126 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 127 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 128 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 129 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 130 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 131 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 132 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 133 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 134 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 135 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 136 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 137 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 138 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 139 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 140 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 141 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 142 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 143 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 144 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 145 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 146 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 147 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 148 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 149 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 150 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 151 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 152 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 153 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 154 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 155 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 156 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 157 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 158 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 159 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 160 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 161 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 162 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 163 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 164 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 165 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 166 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 167 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 168 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 169 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 170 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 171 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 172 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 173 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 174 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 175 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 176 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 177 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 178 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 179 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 180 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 181 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 182 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 183 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 184 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 185 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 186 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 187 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 188 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 189 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 190 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 191 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 192 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 193 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 194 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 195 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 196 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 197 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 198 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 199 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 200 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 201 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 202 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 203 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 204 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 205 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 206 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 207 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 208 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
