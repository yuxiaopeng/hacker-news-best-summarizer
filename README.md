# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-10-13.md)

*最后自动更新时间: 2026-10-13 23:36:24*
## 1. 黑客启动遍及欧洲的超市冷柜自动除霜功能。

**原文标题**: Hackers activate automatic defrosting in supermarket fridges across Europe

**原文链接**: [https://www.tomshardware.com/tech-industry/cyber-security/unprecedented-cyberattack-cripples-supermarket-fridges-across-europe-as-hackers-activate-automatic-defrosting-delivery-and-store-prices-also-impacted-by-incident](https://www.tomshardware.com/tech-industry/cyber-security/unprecedented-cyberattack-cripples-supermarket-fridges-across-europe-as-hackers-activate-automatic-defrosting-delivery-and-store-prices-also-impacted-by-incident)

一场重大的网络攻击扰乱了欧洲主要超市连锁店，主要目标是法国和荷兰的制冷控制系统。包括Intermarché、Leclerc和Coopérative U在内的法国零售商受到影响，Coopérative U总裁Dominique Schelcher证实这是一起“极其严重”的事件。

此次攻击破坏了丹佛斯制造的制冷控制器，激活了持续的强制除霜循环，设置为高达50摄氏度，导致冰箱和冰柜“热浪滚滚”。这导致了商品大范围变质，初步损失估计接近30万欧元，潜在损失可能达到数百万。

在荷兰，Albert Heijn、Etos和Gall & Gall的网站遭遇中断，影响了配送服务，电子货架标签也受到影响，扰乱了店内定价。隶属于Albert Heijn的比利时Delhaize连锁店也报告了中断情况，包括会员忠诚计划问题。超市正在采取措施，包括暂时关闭受影响的IT系统。目前尚不清楚法国和荷兰的事件是否相关，也尚不清楚攻击的全面影响。

---

## 2. 双子星4号 氩

**原文标题**: Gemini 4 Argon

**原文链接**: [https://deepmind.google/models/gemini/](https://deepmind.google/models/gemini/)

Argon 使 Chrome 团队能够将核心网页处理功能从 Chromium 庞大的4000万行代码库中一个约600万行的遗留文件夹中解耦出来。通过促进多项并发的代码更改，Argon 加速了一项涉及数百个文件的重大架构重构，将数月的工作压缩到数周完成。这一效率提升将使 Chrome 的数十亿用户受益，因为它允许活动网页在标签页、侧边面板和浮动窗口之间无缝移动，无需重新加载，从而消除了浏览器崩溃的一个常见原因。

---

## 3. Fingerprints are the new cookies

**原文标题**: Fingerprints are the new cookies

**原文链接**: [https://royfish.dev/fingerprints-are-the-new-cookies](https://royfish.dev/fingerprints-are-the-new-cookies)

生成摘要时出错

---

## 4. C语言现代Web应用

**原文标题**: A Modern Web App in C

**原文链接**: [https://prophitt.me/writing/a-modern-web-app-in-c](https://prophitt.me/writing/a-modern-web-app-in-c)

2026年，作者成功推出了“marketyour.games”——一个现代商业网络产品，但它使用的是C语言和CGI，这些技术让人想起1994年。其内部技术栈被称为“BCHS”，包含OpenBSD、C语言、httpd和SQLite，刻意避开了框架、数据库服务器或容器。

工作流程直接明了：一个C程序读取CGI环境变量，将响应写入标准输出（stdout），将日志写入标准错误（stderr），并通过其C API直接与SQLite交互。部署只需替换静态链接的二进制文件。项目使用的外部依赖极少（libcurl, libsodium），并且将libcjson和SQLite内部集成以进一步实现自包含并降低供应链风险。所有资产都嵌入到二进制文件中，从而实现了快速、整洁的构建。

主要优点包括CGI稳定、基础的特性，只需理解HTTP即可。这种方法确保了Web服务器和应用程序逻辑之间的清晰关注点分离，从而简化了调试。极简的依赖图显著降低了供应链漏洞。开发者可以利用gdb和valgrind等成熟、老牌的C语言工具，甚至直接在C语言中编写HTML也避免了模板语言常见的编辑器冲突。SQLite的直接文件访问消除了传统数据库服务器相关的运维负担。

主要的缺点是CGI缺乏内置实用程序，这迫使开发者必须为cookie解析、表单验证和输入转义等常见任务实现自定义解决方案。

尽管CGI历史悠久，作者认为其过去的局限性，如进程forking的开销，在现代内核中已基本得到缓解。这次体验令人愉快，证明了这个“老旧”的技术栈不仅对现代网络应用可行，而且还提供了独特的优势。

---

## 5. GLM-法律

**原文标题**: GLM-Legal

**原文链接**: [https://z.ai/blog/glm-legal](https://z.ai/blog/glm-legal)

Unable to access the article link.

---

## 6. Muse Wonder

**原文标题**: Muse Wonder

**原文链接**: [https://research.meta.ai/blog/muse-wonder](https://research.meta.ai/blog/muse-wonder)

生成摘要时出错

---

## 7. Rust 借用检查器中发现存在11年的不健全性漏洞

**原文标题**: 11 year old unsoundness bugs found in Rust borrow checker

**原文链接**: [https://github.com/rust-lang/rust/issues/164250](https://github.com/rust-lang/rust/issues/164250)

Rust 借用检查器中发现了一个严重的健全性缺陷，具体来说，它允许通过协变字段赋值来绕过 `struct` 的生命周期要求。这个 `P-high`、`I-unsound` 的 bug 可能导致内存不安全，例如作用域后使用 (use-after-scope) 错误和段错误 (segfaults)，可重现的示例在 AddressSanitizer 下崩溃就证明了这一点。

核心问题在于，它允许将一个非`'static`的引用赋值给一个在形式上期望`'static`生命周期的 `struct` 字段。这变得可被利用，尤其是在 `Drop` 实现中，已释放的数据随后可以被访问或移动，从而导致未定义行为。

值得注意的是，这个 bug 已经存在 11 年了，其概念验证代码可以在可追溯到 1.4 或 1.18.0 的稳定 Rust 版本上编译。它的迟滞发现表明它不容易被意外触发，并且利用通常需要一个“蓄意恶意的 `Drop` 实现”。

Rust 类型团队正在高度重视并处理此问题，强调他们致力于修复所有类型系统的不健全性，并加强该语言的安全基础。由于讨论激烈，该问题的讨论帖曾被暂时锁定。

---

## 8. AI is a tool and using it well takes skill

**原文标题**: AI is a tool and using it well takes skill

**原文链接**: [https://yyhh.org/blog/2026/10/ai-is-a-tool/](https://yyhh.org/blog/2026/10/ai-is-a-tool/)

The article refutes Rich Hickey's argument that LLMs are not tools but automation because they cannot be "wielded." The author asserts that LLMs *are* tools, and using them effectively demands skill, much like any other instrument. Good tool operation requires the user to direct, interpret feedback, recognize mistakes, and make corrections—qualities equally applicable to LLMs. The author likens AI to a "mirror," reflecting the user's curiosity, judgment, and habits, emphasizing the importance of well-posed questions and rigorous standards.

While LLMs exhibit unpredictability, the author argues that qualities like reliability or simplicity are measures for *evaluating* tools, not prerequisites for their category membership. The distinction between tools and automation is deemed false, as automation can be a *feature* of tools like compilers or spreadsheets, which users still "wield" by specifying inputs and examining results.

The claim that LLM use lacks intention, feedback, or expertise is also challenged. Users engage in deliberate feedback loops, questioning, testing, and refining requests, which requires significant human expertise. While LLMs *can* be used to avoid intellectual work (e.g., uncritically accepting summaries), they can also augment it, depending on the user's approach.

The author also criticizes the anthropomorphic language ("go rogue," "conspire") often used in AI discussions, suggesting it misrepresents engineering problems as having human motives. The true distinction, the article concludes, is between skillfully wielding an instrument and delegating work without adequate understanding or oversight—a practical framework for AI.

---

## 9. 苹果家庭视图

**原文标题**: Apple HomeView

**原文链接**: [https://www.apple.com/apple-homeview/](https://www.apple.com/apple-homeview/)

苹果 HomeView 将于11月13日（可预购）上市，这是一款新型智能家居设备，旨在将全家连接起来，并在一个私密中心提供娱乐和信息。它搭载由Apple Intelligence驱动的Siri AI，提供个性化协助、全球知识和无缝对话，同时通过安全隔区（Secure Exclaves）和私有云计算（Private Cloud Compute）严格保护隐私。

该设备最多支持六位用户，提供定制体验并确保个人数据独立。它配备一块生动的7英寸Liquid Retina显示屏，支持原彩显示（True Tone），以及一个用于视频通话的1200万像素人物居中（Center Stage）摄像头。音频是其一大亮点，强大的扬声器提供充满整个房间的空间音频（Spatial Audio）和多房间播放功能，以及四个波束成形麦克风，用于实现水晶般清晰的语音命令和通话。

HomeView可作为终极智能家居中枢，与“家庭”App深度集成，用于管理配件、实时查看摄像头画面以及接收智能通知。它提供丰富的娱乐选择，支持Apple自家和兼容的第三方音视频App。

HomeView提供可调节的弧形铝制底座设计（四种颜色）和壁挂式选项（两种颜色），精心设计以适应任何空间。Apple提供全面的支持，包括引导式购物（Guided Shopping）、个性化设置（Personal Setup）、专业安装服务和灵活的配送选项，以提升整体用户体验。

---

## 10. Deloitte falsified documents to evade tax on Abramovich's wealth

**原文标题**: Deloitte falsified documents to evade tax on Abramovich's wealth

**原文链接**: [https://www.bbc.com/news/articles/c64g1l5389kvo](https://www.bbc.com/news/articles/c64g1l5389kvo)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-10-13](output/hacker_news_summary_2026-10-13.md) |
| 2 | [2026-10-07](output/hacker_news_summary_2026-10-07.md) |
| 3 | [2026-10-06](output/hacker_news_summary_2026-10-06.md) |
| 4 | [2026-10-04](output/hacker_news_summary_2026-10-04.md) |
| 5 | [2026-10-10](output/hacker_news_summary_2026-10-10.md) |
| 6 | [2026-10-09](output/hacker_news_summary_2026-10-09.md) |
| 7 | [2026-10-11](output/hacker_news_summary_2026-10-11.md) |
| 8 | [2026-10-01](output/hacker_news_summary_2026-10-01.md) |
| 9 | [2026-09-29](output/hacker_news_summary_2026-09-29.md) |
| 10 | [2026-09-30](output/hacker_news_summary_2026-09-30.md) |
| 11 | [2026-10-02](output/hacker_news_summary_2026-10-02.md) |
| 12 | [2026-09-27](output/hacker_news_summary_2026-09-27.md) |
| 13 | [2026-10-03](output/hacker_news_summary_2026-10-03.md) |
| 14 | [2026-09-24](output/hacker_news_summary_2026-09-24.md) |
| 15 | [2026-09-21](output/hacker_news_summary_2026-09-21.md) |
| 16 | [2026-09-23](output/hacker_news_summary_2026-09-23.md) |
| 17 | [2026-09-20](output/hacker_news_summary_2026-09-20.md) |
| 18 | [2026-09-22](output/hacker_news_summary_2026-09-22.md) |
| 19 | [2026-09-25](output/hacker_news_summary_2026-09-25.md) |
| 20 | [2026-09-16](output/hacker_news_summary_2026-09-16.md) |
| 21 | [2026-09-14](output/hacker_news_summary_2026-09-14.md) |
| 22 | [2026-09-17](output/hacker_news_summary_2026-09-17.md) |
| 23 | [2026-09-19](output/hacker_news_summary_2026-09-19.md) |
| 24 | [2026-09-18](output/hacker_news_summary_2026-09-18.md) |
| 25 | [2026-09-15](output/hacker_news_summary_2026-09-15.md) |
| 26 | [2026-09-09](output/hacker_news_summary_2026-09-09.md) |
| 27 | [2026-09-10](output/hacker_news_summary_2026-09-10.md) |
| 28 | [2026-09-13](output/hacker_news_summary_2026-09-13.md) |
| 29 | [2026-09-08](output/hacker_news_summary_2026-09-08.md) |
| 30 | [2026-09-11](output/hacker_news_summary_2026-09-11.md) |
| 31 | [2026-09-12](output/hacker_news_summary_2026-09-12.md) |
| 32 | [2026-09-03](output/hacker_news_summary_2026-09-03.md) |
| 33 | [2026-09-02](output/hacker_news_summary_2026-09-02.md) |
| 34 | [2026-08-31](output/hacker_news_summary_2026-08-31.md) |
| 35 | [2026-09-04](output/hacker_news_summary_2026-09-04.md) |
| 36 | [2026-09-05](output/hacker_news_summary_2026-09-05.md) |
| 37 | [2026-09-01](output/hacker_news_summary_2026-09-01.md) |
| 38 | [2026-09-07](output/hacker_news_summary_2026-09-07.md) |
| 39 | [2026-09-06](output/hacker_news_summary_2026-09-06.md) |
| 40 | [2026-08-25](output/hacker_news_summary_2026-08-25.md) |
| 41 | [2026-08-28](output/hacker_news_summary_2026-08-28.md) |
| 42 | [2026-08-23](output/hacker_news_summary_2026-08-23.md) |
| 43 | [2026-08-29](output/hacker_news_summary_2026-08-29.md) |
| 44 | [2026-08-24](output/hacker_news_summary_2026-08-24.md) |
| 45 | [2026-08-30](output/hacker_news_summary_2026-08-30.md) |
| 46 | [2026-08-26](output/hacker_news_summary_2026-08-26.md) |
| 47 | [2026-08-22](output/hacker_news_summary_2026-08-22.md) |
| 48 | [2026-08-14](output/hacker_news_summary_2026-08-14.md) |
| 49 | [2026-08-19](output/hacker_news_summary_2026-08-19.md) |
| 50 | [2026-08-20](output/hacker_news_summary_2026-08-20.md) |
| 51 | [2026-08-16](output/hacker_news_summary_2026-08-16.md) |
| 52 | [2026-08-17](output/hacker_news_summary_2026-08-17.md) |
| 53 | [2026-08-18](output/hacker_news_summary_2026-08-18.md) |
| 54 | [2026-08-15](output/hacker_news_summary_2026-08-15.md) |
| 55 | [2026-08-21](output/hacker_news_summary_2026-08-21.md) |
| 56 | [2026-08-12](output/hacker_news_summary_2026-08-12.md) |
| 57 | [2026-08-11](output/hacker_news_summary_2026-08-11.md) |
| 58 | [2026-08-10](output/hacker_news_summary_2026-08-10.md) |
| 59 | [2026-08-09](output/hacker_news_summary_2026-08-09.md) |
| 60 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 61 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 62 | [2026-08-13](output/hacker_news_summary_2026-08-13.md) |
| 63 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 64 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 65 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 66 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 67 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 68 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 69 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 70 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 71 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 72 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 73 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 74 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 75 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 76 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 77 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 78 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 79 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 80 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 81 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 82 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 83 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 84 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 85 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 86 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 87 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 88 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 89 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 90 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 91 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 92 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 93 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 94 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 95 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 96 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 97 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 98 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 99 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 100 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 101 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 102 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 103 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 104 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 105 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 106 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 107 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 108 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 109 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 110 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 111 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 112 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 113 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 114 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 115 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 116 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 117 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 118 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 119 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 120 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 121 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 122 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 123 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 124 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 125 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 126 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 127 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 128 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 129 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 130 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 131 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 132 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 133 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 134 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 135 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 136 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 137 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 138 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 139 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 140 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 141 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 142 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 143 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 144 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 145 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 146 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 147 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 148 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 149 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 150 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 151 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 152 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 153 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 154 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 155 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 156 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 157 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 158 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 159 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 160 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 161 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 162 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 163 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 164 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 165 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 166 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 167 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 168 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 169 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 170 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 171 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 172 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 173 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 174 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 175 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 176 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 177 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 178 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 179 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 180 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 181 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 182 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 183 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 184 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 185 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 186 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 187 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 188 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 189 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 190 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 191 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 192 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 193 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 194 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 195 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 196 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 197 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 198 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 199 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 200 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 201 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 202 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 203 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 204 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 205 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 206 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 207 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 208 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 209 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 210 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 211 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 212 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 213 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 214 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 215 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 216 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 217 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 218 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 219 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 220 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 221 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 222 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 223 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 224 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 225 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 226 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 227 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 228 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 229 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 230 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 231 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 232 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 233 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 234 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 235 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 236 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 237 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 238 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 239 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 240 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 241 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 242 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 243 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 244 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 245 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 246 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 247 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 248 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 249 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 250 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 251 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 252 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 253 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 254 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 255 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 256 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 257 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 258 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 259 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 260 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 261 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 262 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 263 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 264 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 265 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 266 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 267 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 268 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 269 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 270 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 271 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 272 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 273 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 274 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 275 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 276 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 277 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 278 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 279 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 280 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 281 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 282 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 283 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 284 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 285 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 286 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 287 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 288 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 289 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 290 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 291 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 292 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 293 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 294 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 295 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 296 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 297 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 298 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 299 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 300 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 301 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 302 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 303 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 304 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 305 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 306 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 307 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 308 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 309 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 310 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 311 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 312 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 313 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 314 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 315 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 316 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 317 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 318 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 319 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 320 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 321 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 322 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 323 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 324 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 325 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 326 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 327 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 328 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 329 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
| 330 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 331 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 332 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 333 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
