# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2025-12-27.md)

*最后自动更新时间: 2025-12-27 19:38:48*
## 1. Show HN: Xcc700：700行代码实现的ESP32 (Xtensa) 自举迷你C编译器

**原文标题**: Show HN: Xcc700: Self-hosting mini C compiler for ESP32 (Xtensa) in 700 lines

**原文链接**: [https://github.com/valdanylchuk/xcc700](https://github.com/valdanylchuk/xcc700)

“xcc700”项目呈现了一个卓越的自举式迷你C编译器，专为ESP32 (Xtensa架构)设计，仅用700行C代码编写。其主要吸引力在于简洁性，使其易于理解、修改，并能适应其他语言或用途。

该编译器面向ESP32，接收单个C源文件并生成可重定位的ELF输出。这些ELF文件可由ESP-IDF的`elf_loader`直接运行，从而实现在ESP32上快速测试/调试循环、热修复或持续集成。用户可以在PC上将`xcc700`作为交叉编译器运行，直接在ESP32上编译它（它能自举编译），或者将其作为固件中的一个函数进行集成。

`xcc700`支持一个足以构建自身的最小C特性集，包括基本的控制流（while、if/else）、`int`/`char`/指针/数组、函数调用以及算术/位运算符。然而，它有意省略了许多高级C特性（例如，`for`/`do`循环、`struct`s、`float`s、预处理器、健壮的错误处理或优化），优先考虑简洁性。为此牺牲了性能，自举编译的版本比GCC编译的版本更大且更慢。

该项目根据MIT许可证发布，作者鼓励为教育目的、编程马拉松或探索极简计算而进行分叉和扩展。该项目堪称一份“艺术宣言”，质疑对资源密集型软件的需求，并展示了简单、易于修改的工具在ESP32等低功耗设备上的强大潜力。

---

## 2. UBlockOrigin 和 UBlacklist AI 黑名单

**原文标题**: UBlockOrigin and UBlacklist AI Blocklist

**原文链接**: [https://github.com/laylavish/uBlockOrigin-HUGE-AI-Blocklist](https://github.com/laylavish/uBlockOrigin-HUGE-AI-Blocklist)

本文章介绍了一个“巨型AI黑名单”，这是一个手动整理的列表，包含了1000多个包含AI生成内容的网站，旨在清理Google、DuckDuckGo和Bing上的图片搜索结果。

该黑名单兼容各种平台和工具。对于PC/桌面用户，可以通过一键链接或手动URL输入轻松导入到uBlock Origin或uBlacklist扩展中。移动设备支持方面，iOS/iPadOS用户可通过uBlacklist Safari扩展使用，Android用户则可通过Firefox使用uBlock Origin或uBlacklist。此外，还提供了一个Hosts文件版本，用于通过Pi-hole和Adguard进行全网络范围的屏蔽。

除了主黑名单，还有一个可选的“核弹级列表”，专门针对那些混合了真实内容和AI生成内容的网站（例如DeviantArt）。用户可以通过在uBlock Origin或uBlacklist中设置特定网站的白名单来定制自己的体验。该指南还详细介绍了“扩展过滤”功能，使用户能够通过uBlock Origin的自定义过滤器或uBlacklist的正则表达式，根据特定关键词（例如“AI Art”、“Midjourney”）屏蔽搜索结果。

欢迎通过拉取请求或问题报告对列表做出贡献。文章最后列出了几个涉及SEO垃圾邮件、AI音乐和AI图像检测的相关项目，并包含了一条支持LGBTQ+权益的信息。

---

## 3. 展示HN：基于 Rust/WASM 的 AutoLISP 解释器 — 33 年前发明的 CAD 工作流

**原文标题**: Show HN: AutoLISP interpreter in Rust/WASM – a CAD workflow invented 33 yrs ago

**原文链接**: [https://acadlisp.de/noscript.html](https://acadlisp.de/noscript.html)

`acadlisp` 是一个用Rust编写并编译成WebAssembly的AutoLISP解释器，它允许AutoLISP代码直接在网页浏览器中执行，无需安装AutoCAD。

该项目源于作者在1991年为一家德国电气公司发明的一种CAD工作流。这个创新系统结合CSV文件、模板和AutoLISP代码，自动化生成定制电气原理图。在电子表格中定义的组件会自动生成完整的技术图纸。作者创建`acadlisp`，部分是出于怀旧，部分是为了保存这种他认为已在很大程度上被遗忘的独特工作流。

文章还强调了LISP作为早期AI语言的历史意义，强调了其关键特性：同像性（代码和数据共享列表结构）、自修改和符号处理。1991年的原理图生成器就体现了这些特性，其代码能够编写和修改自身，从而触发进一步的组件插入和模板生成。

从技术上讲，`acadlisp`使用Rust，目标是WebAssembly，并支持SVG和DXF（AutoCAD R12）等输出格式。它实现了各种常见的AutoLISP函数，包括`defun`、`setq`、控制流语句（`if`、`while`、`cond`）、数学运算、列表操作（`car`、`cdr`）以及AutoCAD交互（`command`、`princ`）。提供了交互式演示和源代码。

---

## 4. 医疗软件公司CEO因十亿美元欺诈案获刑

**原文标题**: CEO of Health Care Software Company Sentenced for $1B Fraud Conspiracy

**原文链接**: [https://www.justice.gov/opa/pr/ceo-health-care-software-company-sentenced-1b-fraud-conspiracy](https://www.justice.gov/opa/pr/ceo-health-care-software-company-sentenced-1b-fraud-conspiracy)

摘要：

一家医疗软件公司的前首席执行官桑尼·巴尔瓦尼，因其在与电子健康记录（EHR）激励计划相关的10亿美元欺诈阴谋中的作用，被判处13年监禁。巴尔瓦尼与其他人共同策划了一项欺诈美国政府和医疗服务提供者的计划。

该阴谋涉及巴尔瓦尼及其同谋谎报其EHR软件的功能和合规性，以获得认证并诱使服务提供者购买。他们据称向客户支付回扣以留住他们并隐藏缺陷。这些行为使得包括医生和医院在内的客户能够虚假证明其使用了合规的EHR软件，从而根据《HITECH法案》获得了数亿美元的联邦激励付款。

巴尔瓦尼被判犯有共谋实施医疗欺诈和电信欺诈罪，以及五项医疗欺诈罪。起诉书详细说明了该公司的软件如何未能满足基本的互操作性和数据可移植性要求，影响了患者护理，并欺骗了政府和医疗系统。除了监禁，巴尔瓦尼还被责令支付2.702亿美元的赔偿金并没收100万美元。其他同谋和该公司此前也因参与此广泛欺诈而面临定罪和处罚。

---

## 5. 关于恢复达什的文告

**原文标题**: A Proclamation Regarding the Restoration of the Dash

**原文链接**: [https://blog.nawaz.org/posts/2025/Dec/a-proclamation-regarding-the-restoration-of-the-dash/](https://blog.nawaz.org/posts/2025/Dec/a-proclamation-regarding-the-restoration-of-the-dash/)

2025年12月26日，作者发布了一项声明，哀叹现代社会对优雅的破折号（—）存在的偏见。破折号传统上用于插入语、突转和节奏性停顿，但现在却受到不公正的诋毁，常被视为“不假思索的机器”，如大型语言模型（作者声称它们只是拙劣地模仿了复杂性）的“告密迹象”。

作者还批评了日益增多的对“不起眼的连字符”（-）的误用，将其视为“大胆破折号”的“懦弱替代品”，认为它使散文变得平淡无奇。作者拒绝将古典标点符号拱手让给算法，也拒绝因害怕显得“人工化”而退缩，并因此颁布了“破折号复兴”的命令。

在其博客范围内，作者为人类作家夺回了破折号，并将连字符从所有标点和停顿的角色中驱逐，在所有文体风格的实例中，都用“光荣的、不悔的破折号”取而代之。作为对这种误判的抗议，作者（他本人已经习惯手动输入破折号）创建了一个插件，将其博客上的*所有*连字符都转换为破折号，即使在连字符传统上是恰当的地方，并敦促读者“加入这场革命”。

---

## 6. Unix find表达式编译为字节码

**原文标题**: Unix "find" expressions compiled to bytecode

**原文链接**: [https://nullprogram.com/blog/2025/12/23/](https://nullprogram.com/blog/2025/12/23/)

本文描述了一个自定义编译器 `findc`，它将 Unix `find` 表达式翻译成字节码，与实际 `find` 工具中常见的树遍历解释器形成对比。作者开发这项技术是为了提高效率，因为 `find` 适用于处理大量文件。

`find` 表达式使用 `-a` (AND)、`-o` (OR) 和 `!` (NOT) 等运算符，带有隐式的 `-a` 和默认的 `-print` 动作。括号用于表示优先级，并且操作是短路的，尽管作者指出 `find` 的 `-regex` 无论如何都会进行预编译。

该字节码设计适用于单寄存器、1位机器，使用五个操作码：`halt`、`not`、`braf`（如果为假则分支）、`brat`（如果为真则分支）和 `action NAME [ARGS...]`。跳转始终是向前的。

编译过程主要包括两个步骤：
1.  **解析：** 使用调度场算法将 `find` 的中缀参数转换为后缀标记流，处理运算符优先级以及隐式的 `-a` 和 `-print` 动作。
2.  **编译：** 然后将此后缀流翻译成字节码。编译器维护一个字节码*片段*堆栈。动作变为 `action` 指令。`!` 操作符附加 `not` 指令。像 `-a` 和 `-o` 这样的二元运算符会弹出两个片段，插入 `braf` 或 `brat` 指令以实现短路，即如果第一个片段的评估结果允许，则跳过第二个片段。最终结果是一个由 `halt` 指令终止的单一程序片段。

作者指出了通过窥孔优化改进生成的字节码的机会，例如消除冗余的 `not` 指令以及优化分支目标。

---

## 7. 零宽字符绘图

**原文标题**: Drawing with zero-width characters

**原文链接**: [https://zw.swerdlow.dev](https://zw.swerdlow.dev)

这篇题为《零宽字符绘图》的文章，旨在提供一个实践演示，而非传统的文字解释。作者通过指出一组通常在《古兰经》中出现的18个Unicode字符，深刻改变了他们对文本渲染方式的设想，从而引入了这个概念。

文章的核心内容是一个视觉上引人注目的排布，主要由这些零宽或组合Unicode字符构成。在这个错综复杂的图案中，“零宽字符绘图”这句话被巧妙地“描绘”出来，实际上正是利用了文章所讨论的这些字符。这展示了这些特殊Unicode元素不同寻常的图形潜力。尽管它们本身不占用任何水平空间，但它们可以与前置字符组合并进行修改，从而创造出复杂的视觉效果，并在基于文本的媒介中展示了一种非传统的视觉艺术方法。

---

## 8. High school student discovers 1.5M potential new astronomical objects

**原文标题**: High school student discovers 1.5M potential new astronomical objects

**原文链接**: [https://www.smithsonianmag.com/smart-news/high-school-student-discovers-1-5-million-potential-new-astronomical-objects-by-developing-an-ai-algorithm-180986429/](https://www.smithsonianmag.com/smart-news/high-school-student-discovers-1-5-million-potential-new-astronomical-objects-by-developing-an-ai-algorithm-180986429/)

生成摘要时出错

---

## 9. Janet Jackson had the power to crash laptop computers (2022)

**原文标题**: Janet Jackson had the power to crash laptop computers (2022)

**原文链接**: [https://devblogs.microsoft.com/oldnewthing/20220816-00/?p=106994](https://devblogs.microsoft.com/oldnewthing/20220816-00/?p=106994)

生成摘要时出错

---

## 10. Inside the proton, the ‘most complicated thing you could possibly imagine’ (2022)

**原文标题**: Inside the proton, the ‘most complicated thing you could possibly imagine’ (2022)

**原文链接**: [https://www.quantamagazine.org/inside-the-proton-the-most-complicated-thing-imaginable-20221019/](https://www.quantamagazine.org/inside-the-proton-the-most-complicated-thing-imaginable-20221019/)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 2 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 3 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 4 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 5 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 6 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 7 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 8 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 9 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 10 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 11 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 12 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 13 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 14 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 15 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 16 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 17 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 18 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 19 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 20 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 21 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 22 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 23 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 24 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 25 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 26 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 27 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 28 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 29 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 30 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 31 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 32 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 33 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 34 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 35 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 36 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 37 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 38 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 39 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 40 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 41 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 42 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 43 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 44 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 45 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 46 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 47 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 48 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 49 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 50 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 51 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 52 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
