# Hacker News 热门文章摘要 (2026-08-02)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

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

## 11. Top amputation surgeon had own legs removed due to fetish. Were patients safe?

**原文标题**: Top amputation surgeon had own legs removed due to fetish. Were patients safe?

**原文链接**: [https://www.theguardian.com/uk-news/2026/aug/01/neil-hopper-surgeon-amputated-legs-fetish-extreme-mutilation-patients-questions](https://www.theguardian.com/uk-news/2026/aug/01/neil-hopper-surgeon-amputated-legs-fetish-extreme-mutilation-patients-questions)

生成摘要时出错

---

## 12. Google kills Earth AI generator after one day

**原文标题**: Google kills Earth AI generator after one day

**原文链接**: [https://twitter.com/newsfromgoogle/status/2083249962150760610](https://twitter.com/newsfromgoogle/status/2083249962150760610)

生成摘要时出错

---

## 13. Microsoft raises Xbox prices by up to 43%

**原文标题**: Microsoft raises Xbox prices by up to 43%

**原文链接**: [https://www.theverge.com/games/974253/xbox-prices-increasing-200-euros](https://www.theverge.com/games/974253/xbox-prices-increasing-200-euros)

生成摘要时出错

---

## 14. Has the New Cocaine Arrived?

**原文标题**: Has the New Cocaine Arrived?

**原文链接**: [https://playboy.substack.com/p/has-the-new-cocaine-finally-arrived](https://playboy.substack.com/p/has-the-new-cocaine-finally-arrived)

生成摘要时出错

---

## 15. 石油公司报告天价利润，得益于战时原油价格。

**原文标题**: Oil companies report sky-high profits thanks to wartime crude prices

**原文链接**: [https://www.npr.org/2026/07/31/nx-s1-5910660/big-oil-earnings-q2-2026](https://www.npr.org/2026/07/31/nx-s1-5910660/big-oil-earnings-q2-2026)

生成摘要时出错

---

## 16. Nano Banana 2 removed from Google Earth

**原文标题**: Nano Banana 2 removed from Google Earth

**原文链接**: [https://www.digitaldigging.org/p/nano-banana-2-removed-from-google](https://www.digitaldigging.org/p/nano-banana-2-removed-from-google)

生成摘要时出错

---

## 17. Pushes to arch AUR are suspendended right now.

**原文标题**: Pushes to arch AUR are suspendended right now.

**原文链接**: [https://lists.archlinux.org/archives/list/aur-general@lists.archlinux.org/message/YPJ3FQYJTJXXY3RUXCYLMHUKHLIUNVFF/](https://lists.archlinux.org/archives/list/aur-general@lists.archlinux.org/message/YPJ3FQYJTJXXY3RUXCYLMHUKHLIUNVFF/)

生成摘要时出错

---

## 18. Rooting, firmware analysis and persistent credentials of TP-Link TL-841N

**原文标题**: Rooting, firmware analysis and persistent credentials of TP-Link TL-841N

**原文链接**: [https://blog.juni-mp4.com/posts/42/rooting-the-tplink-tl841n-pt1/](https://blog.juni-mp4.com/posts/42/rooting-the-tplink-tl841n-pt1/)

生成摘要时出错

---

## 19. Kaisel – Routes as Values. Dart 3 Native Router for Flutter

**原文标题**: Kaisel – Routes as Values. Dart 3 Native Router for Flutter

**原文链接**: [https://kaisel.dev/](https://kaisel.dev/)

生成摘要时出错

---

## 20. Show HN: NixOS-DGX-Spark – Nix and NixOS on the DGX Spark

**原文标题**: Show HN: NixOS-DGX-Spark – Nix and NixOS on the DGX Spark

**原文链接**: [https://github.com/graham33/nixos-dgx-spark](https://github.com/graham33/nixos-dgx-spark)

生成摘要时出错

---

## 21. Zitron: "Everyone Has Been Sold a Lie" on AI [video]

**原文标题**: Zitron: "Everyone Has Been Sold a Lie" on AI [video]

**原文链接**: [https://www.youtube.com/watch?v=pHcZpvIfho0](https://www.youtube.com/watch?v=pHcZpvIfho0)

生成摘要时出错

---

## 22. Cyberscript

**原文标题**: Cyberscript

**原文链接**: [https://cyberscript.dev](https://cyberscript.dev)

生成摘要时出错

---

## 23. Nerd culture is murdering intellectuals

**原文标题**: Nerd culture is murdering intellectuals

**原文链接**: [https://www.theintrinsicperspective.com/p/nerd-culture-is-murdering-intellectuals](https://www.theintrinsicperspective.com/p/nerd-culture-is-murdering-intellectuals)

生成摘要时出错

---

## 24. The time filter in Google Search broke a few days ago

**原文标题**: The time filter in Google Search broke a few days ago

**原文链接**: [https://mastodon.online/@mwichary/117023736804129342](https://mastodon.online/@mwichary/117023736804129342)

生成摘要时出错

---

## 25. Cookware Got Worse on Purpose: Who Owns Pyrex and All-Clad Now

**原文标题**: Cookware Got Worse on Purpose: Who Owns Pyrex and All-Clad Now

**原文链接**: [https://www.worseonpurpose.com/p/your-cookware-got-worse-on-purpose](https://www.worseonpurpose.com/p/your-cookware-got-worse-on-purpose)

生成摘要时出错

---

## 26. Google cancels AI Studio app after 800k preorders

**原文标题**: Google cancels AI Studio app after 800k preorders

**原文链接**: [https://twitter.com/GoogleAIStudio/status/2083274575769473092](https://twitter.com/GoogleAIStudio/status/2083274575769473092)

生成摘要时出错

---

## 27. IBM i (OS/400) the Database Operating System

**原文标题**: IBM i (OS/400) the Database Operating System

**原文链接**: [https://osadmins.com/en/ibm-i-os-400-the-database-operating-system/](https://osadmins.com/en/ibm-i-os-400-the-database-operating-system/)

生成摘要时出错

---

## 28. AI's real threat to jobs isn't job loss, it's lower paychecks, new research says

**原文标题**: AI's real threat to jobs isn't job loss, it's lower paychecks, new research says

**原文链接**: [https://www.businessinsider.com/ai-could-lower-workers-pay-job-market-impact-2026-7](https://www.businessinsider.com/ai-could-lower-workers-pay-job-market-impact-2026-7)

生成摘要时出错

---

## 29. An internal OpenAI Astra model solved 10 major open math and CS problems

**原文标题**: An internal OpenAI Astra model solved 10 major open math and CS problems

**原文链接**: [https://twitter.com/polynoamial/status/2083467194663571701](https://twitter.com/polynoamial/status/2083467194663571701)

生成摘要时出错

---

## 30. The teenage hitmen recruited to kill across Europe

**原文标题**: The teenage hitmen recruited to kill across Europe

**原文链接**: [https://www.bbc.com/news/articles/czrjyevmv61o](https://www.bbc.com/news/articles/czrjyevmv61o)

生成摘要时出错

---

## 31. Morten Linderud resigning from Arch Linux development team

**原文标题**: Morten Linderud resigning from Arch Linux development team

**原文链接**: [https://lists.archlinux.org/archives/list/arch-dev-public@lists.archlinux.org/thread/2AX2BCJ3EQX7G3YXSDX73BR4NCAWXXBZ/](https://lists.archlinux.org/archives/list/arch-dev-public@lists.archlinux.org/thread/2AX2BCJ3EQX7G3YXSDX73BR4NCAWXXBZ/)

生成摘要时出错

---

## 32. What liberal arts education is for (2024)

**原文标题**: What liberal arts education is for (2024)

**原文链接**: [https://innig.net/teaching/liberal-arts-manifesto](https://innig.net/teaching/liberal-arts-manifesto)

生成摘要时出错

---

## 33. Dark Hours

**原文标题**: Dark Hours

**原文链接**: [https://darkhours.io](https://darkhours.io)

生成摘要时出错

---

## 34. Apple Will 'Watch Everything Burn' When AI Bubble Bursts

**原文标题**: Apple Will 'Watch Everything Burn' When AI Bubble Bursts

**原文链接**: [https://asymco.com/2026/07/31/apple-will-watch-everything-burn-when-ai-bubble-bursts/](https://asymco.com/2026/07/31/apple-will-watch-everything-burn-when-ai-bubble-bursts/)

生成摘要时出错

---

## 35. Predictive Speculative KV Replication for Bursty LLM Inference

**原文标题**: Predictive Speculative KV Replication for Bursty LLM Inference

**原文链接**: [https://jwlabs.vercel.app/post/biting-the-bullet](https://jwlabs.vercel.app/post/biting-the-bullet)

生成摘要时出错

---

## 36. Only 8.9% of sites block AI crawlers, but 94.8% are never cited in AI answers

**原文标题**: Only 8.9% of sites block AI crawlers, but 94.8% are never cited in AI answers

**原文链接**: [https://website-auditor.io/ai-visibility-index](https://website-auditor.io/ai-visibility-index)

生成摘要时出错

---

## 37. Mathematics Without Mathematicians

**原文标题**: Mathematics Without Mathematicians

**原文链接**: [https://borretti.me/article/mathematics-without-mathematicians](https://borretti.me/article/mathematics-without-mathematicians)

生成摘要时出错

---

## 38. Drug reverses autism-like brain changes in adult mice within hours

**原文标题**: Drug reverses autism-like brain changes in adult mice within hours

**原文链接**: [https://www.uclahealth.org/news/release/drug-reverses-autism-like-brain-changes-adult-mice-within](https://www.uclahealth.org/news/release/drug-reverses-autism-like-brain-changes-adult-mice-within)

生成摘要时出错

---

## 39. Is the Industrial Revolution a good precedent for explosive growth today?

**原文标题**: Is the Industrial Revolution a good precedent for explosive growth today?

**原文链接**: [https://mattsclancy.github.io/2026/07/27/industrial-revolution-growth.html](https://mattsclancy.github.io/2026/07/27/industrial-revolution-growth.html)

生成摘要时出错

---

## 40. The Prospects for 128 Bit Processors ( John Mashey SGI 1995)

**原文标题**: The Prospects for 128 Bit Processors ( John Mashey SGI 1995)

**原文链接**: [https://yarchive.net/comp/128bit.html](https://yarchive.net/comp/128bit.html)

生成摘要时出错

---

## 41. Firefighter arson a long-standing issue – expert

**原文标题**: Firefighter arson a long-standing issue – expert

**原文链接**: [https://www.firerescue1.com/arson-investigation/articles/expert-firefighter-arson-a-long-standing-issue-xHXLFAdYVcQPiuPU/](https://www.firerescue1.com/arson-investigation/articles/expert-firefighter-arson-a-long-standing-issue-xHXLFAdYVcQPiuPU/)

生成摘要时出错

---

## 42. Fermi Paradox

**原文标题**: Fermi Paradox

**原文链接**: [https://en.wikipedia.org/wiki/Fermi_paradox](https://en.wikipedia.org/wiki/Fermi_paradox)

生成摘要时出错

---

## 43. How to Spot AI Writing

**原文标题**: How to Spot AI Writing

**原文链接**: [https://www.economist.com/culture/2026/07/30/how-to-spot-ai-writing](https://www.economist.com/culture/2026/07/30/how-to-spot-ai-writing)

生成摘要时出错

---

## 44. A migrant surge tests Spain's open policies

**原文标题**: A migrant surge tests Spain's open policies

**原文链接**: [https://economist.com/europe/2026/07/31/a-migrant-surge-tests-spains-open-policies](https://economist.com/europe/2026/07/31/a-migrant-surge-tests-spains-open-policies)

生成摘要时出错

---

## 45. Unearthing my 1996 windowed OS in machine code for Am29000 homebrew computer

**原文标题**: Unearthing my 1996 windowed OS in machine code for Am29000 homebrew computer

**原文链接**: [https://nanochess.org/the_am29000_computer.html](https://nanochess.org/the_am29000_computer.html)

生成摘要时出错

---

## 46. Scanning 7.6 Petabytes of HuggingFace Training Data for Secrets

**原文标题**: Scanning 7.6 Petabytes of HuggingFace Training Data for Secrets

**原文链接**: [https://trufflesecurity.com/blog/scanning-7-6-petabytes-of-ai-training-data-for-secrets](https://trufflesecurity.com/blog/scanning-7-6-petabytes-of-ai-training-data-for-secrets)

生成摘要时出错

---

## 47. Generative AI floods and dilutes the market for books

**原文标题**: Generative AI floods and dilutes the market for books

**原文链接**: [https://arxiv.org/abs/2607.20349](https://arxiv.org/abs/2607.20349)

生成摘要时出错

---

## 48. Don't credit the LLM

**原文标题**: Don't credit the LLM

**原文链接**: [https://isaacsu.com/2026/08/dont-credit-the-llm/](https://isaacsu.com/2026/08/dont-credit-the-llm/)

生成摘要时出错

---

## 49. Impro is a handbook for running a cult

**原文标题**: Impro is a handbook for running a cult

**原文链接**: [https://www.seangoedecke.com/impro/](https://www.seangoedecke.com/impro/)

生成摘要时出错

---

## 50. A stray commit buried multiple levels deep cost me months

**原文标题**: A stray commit buried multiple levels deep cost me months

**原文链接**: [https://www.droppedasbaby.com/posts/db-commits/](https://www.droppedasbaby.com/posts/db-commits/)

生成摘要时出错

---

## 51. Franken.domains: Stitched-Together Domains, Because Every .com Is Taken

**原文标题**: Franken.domains: Stitched-Together Domains, Because Every .com Is Taken

**原文链接**: [https://franken.domains/](https://franken.domains/)

生成摘要时出错

---

## 52. Firefox Local Mode for Web Developers

**原文标题**: Firefox Local Mode for Web Developers

**原文链接**: [https://firefox-source-docs.mozilla.org/devtools-user/local_mode/index.html](https://firefox-source-docs.mozilla.org/devtools-user/local_mode/index.html)

生成摘要时出错

---

## 53. OpenAI's claimed disproof of Connes' Rigidity Conjecture is invalid [pdf]

**原文标题**: OpenAI's claimed disproof of Connes' Rigidity Conjecture is invalid [pdf]

**原文链接**: [https://philarchive.org/archive/NIEWTCv17](https://philarchive.org/archive/NIEWTCv17)

生成摘要时出错

---

## 54. Astro Loop

**原文标题**: Astro Loop

**原文链接**: [https://pubdeer.com/](https://pubdeer.com/)

生成摘要时出错

---

## 55. GPUs could explode to multiple TB with new storage-inspired memory tech

**原文标题**: GPUs could explode to multiple TB with new storage-inspired memory tech

**原文链接**: [https://www.theregister.com/storage/2026/07/30/gpus-could-explode-to-multiple-tb-with-new-storage-inspired-memory-tech/5281363](https://www.theregister.com/storage/2026/07/30/gpus-could-explode-to-multiple-tb-with-new-storage-inspired-memory-tech/5281363)

生成摘要时出错

---

## 56. Australia's social media ban has failed

**原文标题**: Australia's social media ban has failed

**原文链接**: [https://www.reuters.com/legal/litigation/australia-defends-teen-social-media-ban-after-study-shows-most-still-online-2026-08-01/](https://www.reuters.com/legal/litigation/australia-defends-teen-social-media-ban-after-study-shows-most-still-online-2026-08-01/)

生成摘要时出错

---

## 57. Coldcard's $38M (so far) exploit shakes faith in self-custody

**原文标题**: Coldcard's $38M (so far) exploit shakes faith in self-custody

**原文链接**: [https://www.coindesk.com/business/2026/07/31/coldcard-s-usd38-million-so-far-exploit-shakes-faith-in-self-custody-may-push-investors-to-etfs](https://www.coindesk.com/business/2026/07/31/coldcard-s-usd38-million-so-far-exploit-shakes-faith-in-self-custody-may-push-investors-to-etfs)

生成摘要时出错

---

## 58. Reddit Stock Collapses 23% as AI Eats Away at User Growth

**原文标题**: Reddit Stock Collapses 23% as AI Eats Away at User Growth

**原文链接**: [https://www.barchart.com/story/news/3584357/reddit-stock-collapses-23-as-ai-eats-away-at-user-growth](https://www.barchart.com/story/news/3584357/reddit-stock-collapses-23-as-ai-eats-away-at-user-growth)

生成摘要时出错

---

## 59. The Coldcard Disaster Gets Worse: The Hack May Have Reached $88.6M

**原文标题**: The Coldcard Disaster Gets Worse: The Hack May Have Reached $88.6M

**原文链接**: [https://medium.com/mountain-movers/the-coldcard-disaster-gets-worse-the-hack-may-have-reached-88-6-af507b028594](https://medium.com/mountain-movers/the-coldcard-disaster-gets-worse-the-hack-may-have-reached-88-6-af507b028594)

生成摘要时出错

---

