# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-08-02.md)

*最后自动更新时间: 2026-08-02 20:28:40*
## 1. GitHub有替代品，但无可取代

**原文标题**: GitHub has alternatives, but no replacement

**原文链接**: [https://lalitm.com/post/github-alternatives/](https://lalitm.com/post/github-alternatives/)

文章指出，尽管GitHub有许多Git仓库托管的替代方案，但没有一个能有效取代其对开源社区至关重要的“社交层”。这种缺失显而易见，因为项目正在离开GitHub，原因包括用户体验恶化、频繁中断，以及人们认为它忽视了核心开发协作功能，转而青睐AI集成（例如Copilot）。

自托管虽然技术上可行，但对于协作项目来说被认为是不切实际的，因为它会给贡献者带来创建新账户和学习陌生界面的负担，从而阻碍了项目的发现和参与。现有的替代方案各有显著缺点：GitLab过于企业化；SourceHut的邮件导向工作流过于小众；Forgejo的联邦化项目仍处于实验阶段；Radicle在技术上很有趣但过于不成熟，需要特定的客户端软件才能交互。甚至像Tangled这样有前途的新平台也还处于Alpha阶段。

作者提出了一种“无聊的公司”——一家只专注于提供可靠、愉快的开源协作，直接收费，并且没有风投支持野心的营利性实体——作为一种潜在的解决方案。然而，根本挑战仍然是“冷启动问题”：即为共享身份、约定和发现建立必要的规模。文章总结道，一个真正的GitHub替代品必须积极开发并把这个社交层作为其主要产品，而不是把它看作是会自动出现的东西。

---

## 2. HN 展示：Fuse —— 静态类型函数式编程语言

**原文标题**: Show HN: Fuse – statically typed functional programming language

**原文链接**: [https://fuselang.org](https://fuselang.org)

Fuse是一种新型的静态类型纯函数式编程语言，具有高阶类型和通过“特性（traits）”实现的即时多态性。它通过GRIN全程序优化器和LLVM编译为原生代码，承诺提供快速、小巧且具有零开销抽象的二进制文件。

该语言专为纯函数式编程设计，融合了代数数据类型、泛型、模式匹配、高阶函数和do记法，以实现富有表达力、可组合的代码。其类型系统基于具有高阶多态性的System F，并由双向类型推断支持，这在很大程度上消除了显式类型注解的需要，但函数签名除外。

Fuse的语法借鉴了Rust、Python、Scala和Haskell，采用基于缩进的代码块、lambda表达式和类似ML的风格，以提高可读性。提供的代码示例展示了如何定义像`Functor`这样的特性，如何为`List`等类型实现这些特性，以及如何使用泛型、`fold`、`map`和`fmap`以函数式方式操作数据。

Fuse工具链适用于Linux (x86_64)和macOS (ARM64)，可通过简单的`curl`命令安装。它旨在在一个简洁、高效、纯函数式的环境中提供强大的领域建模工具。

---

## 3. Rust All Hands 2026 Retrospective

**原文标题**: Rust All Hands 2026 Retrospective

**原文链接**: [https://blog.rust-lang.org/inside-rust/2026/07/31/all-hands-2026-retrospective/](https://blog.rust-lang.org/inside-rust/2026/07/31/all-hands-2026-retrospective/)

生成摘要时出错

---

## 4. RFC 10015: 弃用 TLS 1.2 和 DTLS 1.2 中过时的密钥交换方法

**原文标题**: RFC 10015: Deprecating Obsolete Key Exchange Methods in TLS 1.2 and DTLS 1.2

**原文链接**: [https://www.rfc-editor.org/rfc/rfc10015.html](https://www.rfc-editor.org/rfc/rfc10015.html)

RFC 10015，于2026年7月发布，是一份标准规范文档，旨在废弃并劝退专门用于TLS 1.2和DTLS 1.2连接的过时密钥交换方法。

该文档规定，客户端**不得**提供，服务器**不得**选择以下内容：
*   基于有限域的非临时迪菲-赫尔曼 (FFDH) 密码套件。
*   有限域临时迪菲-赫尔曼 (FFDHE) 密码套件。
*   RSA密钥交换密码套件。

此外，客户端**不应**提供，服务器**不应**选择静态椭圆曲线迪菲-赫尔曼 (ECDH) 密码套件。同样不鼓励使用具有固定DH参数的证书（例如，rsa_fixed_dh、dss_fixed_dh、rsa_fixed_ecdh、ecdsa_fixed_ecdh）。

这些规定仅适用于TLS 1.2和DTLS 1.2。TLS 1.0和1.1已被废弃，而TLS 1.3要么不使用受影响的算法，要么以不同方式处理相关的配置问题。

此次废弃是出于重大的安全隐患：
*   **缺乏前向保密性：** 影响非临时DH和RSA密钥交换。
*   **易受侧信道攻击：** 包括浣熊攻击 (FFDH/FFDHE) 和无效曲线攻击 (ECDH)，通常因公钥重用或复杂的缓解要求而加剧。
*   **已知RSA漏洞：** 例如Bleichenbacher攻击的变种 (ROBOT、DROWN)，难以正确缓解。
*   **FFDHE特有问题：** 由于缺乏群组协商导致的互操作性问题，易受小群组攻击，以及使用常见1024位群组时安全裕度不足。

本RFC更新了多份此前的RFC，并指示IANA在相关注册表中将受影响的密码套件和证书类型标记为“D”（已废弃）。

---

## 5. 欧盟将从8月2日起强制要求对看似真实的AI内容加贴标签

**原文标题**: EU will mandate labels on authentic-looking AI content starting August 2

**原文链接**: [https://www.engadget.com/2227966/eu-mandate-labels-on-authentic-looking-ai-content/](https://www.engadget.com/2227966/eu-mandate-labels-on-authentic-looking-ai-content/)

The European Union will mandate labels on AI-generated content that could be mistaken for authentic material, starting August 2. This regulation, part of the EU's landmark AI Act, aims to enhance transparency and prevent deception by requiring providers of AI systems to clearly label deepfakes and other synthetic content.

The rule applies to "authentic-looking" content like AI-generated images, audio, video, and text that could mislead the public, regardless of whether it's harmful. The labels will need to be machine-readable where possible, and users must be notified when interacting with an AI system. The goal is to inform citizens about AI's use and potential manipulations.

While the AI Act won't fully take effect until 2025, specific provisions are being phased in. This labeling requirement is one of the first to be implemented, underscoring the EU's proactive stance on regulating AI and its potential impact on information integrity.

---

## 6. ESP32-C3 超级迷你天线改装

**原文标题**: ESP32-C3 SuperMini antenna modification

**原文链接**: [https://peterneufeld.wordpress.com/2025/03/04/esp32-c3-supermini-antenna-modification/](https://peterneufeld.wordpress.com/2025/03/04/esp32-c3-supermini-antenna-modification/)

生成摘要时出错

---

## 7. Show HN: Syncular – 离线优先的 SQL 同步，基于 TypeScript 和 Rust 核心

**原文标题**: Show HN: Syncular – offline-first SQL sync with TypeScript and Rust cores

**原文链接**: [https://github.com/syncular/syncular](https://github.com/syncular/syncular)

Syncular是一个离线优先、服务器权威的SQL同步解决方案。客户端维护一个真实的本地SQLite数据库（在浏览器中使用OPFS，在其他地方使用原生实现），乐观地写入到一个发件箱，而服务器则维护一个单一的、有序的提交日志作为数据真相来源。

该项目秉持“规范优先”原则，配备规范性文档和黄金测试夹具。它拥有TypeScript和Rust双核心，通过独立于实现的符合性测试套件保持同步，从而确保跨核心的一致性。严格的测试规范，包括内存中的环回传输和故障注入，确保了其可靠性。

该系统由独立的服务器组件（支持SQLite、Postgres、D1，并提供Hono/Cloudflare Workers绑定）和客户端核心（基于WebAssembly SQLite的TypeScript Web客户端，以及通过FFI的Rust客户端）组成。它提供React Hooks、TypeScript模式生成器，以及每列端到端加密和Yjs CRDT合并器等高级功能。计划为Tauri、React Native、Swift、Kotlin和Flutter提供绑定。

Syncular的开发原则（在AGENTS.md中概述）强调规范优先原则和所有贡献者的高质量。虽然欢迎AI在各种任务中提供协助，但所有提交，尤其是生产代码，都需要经过彻底的审查、理解和辩护，并拒绝低质量的机器生成内容。

---

## 8. Pgtestdb的模板克隆测试方法很快。

**原文标题**: Pgtestdb's template cloning approach to testing is fast

**原文链接**: [https://brandur.org/fragments/pgtestdb](https://brandur.org/fragments/pgtestdb)

文章介绍了`pgtestdb`，一个Go/Postgres测试包，它利用Postgres模板数据库实现快速测试设置。这种方法能快速复制具象化的数据库文件，优于基于迁移或Docker的技术。

作者将`pgtestdb`与River现有的基于schema的测试方法进行了比较，后者在独立的schema中隔离测试，允许调试和测试数据库范围的功能，但每个新schema都需要进行迁移。

令人惊讶的是，初始设置时间相似：`pgtestdb`的数据库克隆和River的schema创建+迁移平均每次设置都在100毫秒左右。这挑战了作者关于完整数据库创建会很慢的先入之见。

然而，River的整体测试套件运行速度快了约3.5倍（14.54秒对51.07秒）。这种速度差异归因于River对*schema复用*的优化。River的测试辅助工具会池化并清理schema，并将其用于后续测试，从而显著减少了整个套件中每个测试的有效设置时间。

文章总结道，尽管`pgtestdb`的模板克隆对于单个设置本身很快，但对于大型应用程序而言，实施复用策略（如River的schema池化）将至关重要，以实现最佳的整体测试套件速度。作者将继续使用River的现有方法，因为它附带的额外好处，但会推荐`pgtestdb`用于特定的端到端测试场景。

---

## 9. Scope of Hacks on U.S. Water Supply Widens as Evidence Points to Iran

**原文标题**: Scope of Hacks on U.S. Water Supply Widens as Evidence Points to Iran

**原文链接**: [https://www.nytimes.com/2026/08/01/us/politics/iran-cyberattack-water-systems.html](https://www.nytimes.com/2026/08/01/us/politics/iran-cyberattack-water-systems.html)

生成摘要时出错

---

## 10. Demystifying DRAM Read Disturbance: RowHammer and RowPress Phenomena

**原文标题**: Demystifying DRAM Read Disturbance: RowHammer and RowPress Phenomena

**原文链接**: [https://arxiv.org/abs/2607.28233](https://arxiv.org/abs/2607.28233)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 2 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 3 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 4 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 5 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 6 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 7 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 8 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 9 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 10 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 11 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 12 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 13 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 14 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 15 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 16 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 17 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 18 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 19 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 20 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 21 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 22 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 23 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 24 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 25 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 26 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 27 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 28 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 29 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 30 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 31 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 32 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 33 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 34 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 35 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 36 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 37 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 38 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 39 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 40 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 41 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 42 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 43 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 44 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 45 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 46 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 47 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 48 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 49 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 50 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 51 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 52 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 53 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 54 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 55 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 56 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 57 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 58 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 59 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 60 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 61 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 62 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 63 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 64 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 65 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 66 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 67 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 68 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 69 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 70 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 71 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 72 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 73 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 74 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 75 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 76 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 77 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 78 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 79 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 80 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 81 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 82 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 83 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 84 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 85 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 86 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 87 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 88 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 89 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 90 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 91 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 92 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 93 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 94 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 95 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 96 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 97 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 98 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 99 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 100 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 101 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 102 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 103 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 104 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 105 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 106 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 107 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 108 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 109 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 110 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 111 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 112 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 113 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 114 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 115 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 116 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 117 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 118 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 119 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 120 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 121 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 122 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 123 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 124 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 125 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 126 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 127 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 128 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 129 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 130 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 131 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 132 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 133 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 134 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 135 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 136 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 137 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 138 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 139 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 140 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 141 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 142 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 143 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 144 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 145 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 146 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 147 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 148 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 149 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 150 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 151 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 152 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 153 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 154 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 155 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 156 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 157 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 158 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 159 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 160 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 161 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 162 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 163 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 164 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 165 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 166 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 167 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 168 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 169 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 170 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 171 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 172 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 173 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 174 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 175 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 176 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 177 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 178 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 179 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 180 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 181 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 182 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 183 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 184 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 185 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 186 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 187 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 188 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 189 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 190 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 191 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 192 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 193 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 194 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 195 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 196 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 197 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 198 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 199 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 200 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 201 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 202 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 203 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 204 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 205 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 206 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 207 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 208 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 209 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 210 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 211 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 212 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 213 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 214 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 215 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 216 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 217 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 218 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 219 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 220 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 221 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 222 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 223 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 224 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 225 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 226 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 227 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 228 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 229 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 230 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 231 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 232 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 233 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 234 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 235 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 236 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 237 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 238 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 239 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 240 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 241 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 242 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 243 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 244 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 245 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 246 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 247 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 248 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 249 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 250 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 251 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 252 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 253 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 254 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 255 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 256 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 257 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 258 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 259 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 260 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 261 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 262 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 263 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 264 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
| 265 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 266 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 267 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 268 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
