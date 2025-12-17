# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2025-12-17.md)

*最后自动更新时间: 2025-12-17 19:50:17*
## 1. 车牌识别监控

**原文标题**: alpr.watch

**原文链接**: [https://alpr.watch/](https://alpr.watch/)

alpr.watch 是一个平台，帮助市民追踪地方政府关于监控技术（例如 Flock 摄像头、面部识别和自动车牌识别系统 (ALPR)）的讨论。该网站强调，市政当局正在越来越多地采用这些系统，目前已部署超过 80,000 个摄像头，用于追踪行踪、收集生物识别数据，并建立关于居民的庞大数据库。

该平台扫描会议议程，寻找“flock”和“alpr”等关键词，并绘制出这些讨论发生的地点，以便用户参与。它允许用户查看当前和过去的会议，查看现有 ALPR 摄像头的部署位置（可通过 deflock.me 报告），并接收其所在区域的电子邮件提醒。

ALPR 系统利用摄像头和人工智能持续记录和存储车牌数据，从而创建车辆乃至个人行踪的全面日志。Flock Safety 是一家领先的 ALPR 制造商，其摄像头捕捉车辆详细信息，并在广泛的机构网络中共享数据。该网站警告存在“滑坡效应”，即监控系统会超出其最初意图进行扩展，导致更广泛的数据共享、新的侵入性使用以及滞后的监管。

alpr.watch 鼓励支持积极对抗大规模监控和保护隐私的组织，包括电子前沿基金会 (EFF)、美国公民自由联盟 (ACLU)、为未来而战 (Fight for the Future)、监控技术监督项目 (STOP) 和司法研究所 (Institute for Justice)。

---

## 2. 800万用户AI对话被“隐私”扩展倒卖牟利

**原文标题**: 8M users' AI conversations sold for profit by "privacy" extensions

**原文链接**: [https://www.koi.ai/blog/urban-vpn-browser-extension-ai-conversations-data-collection](https://www.koi.ai/blog/urban-vpn-browser-extension-ai-conversations-data-collection)

Koi Research（一家网络安全公司）的一项调查显示，“隐私”浏览器扩展，其中以Urban VPN Proxy最为突出，一直在秘密收集并出售来自Chrome和Edge浏览器上超过800万用户的敏感AI对话。尽管这些扩展程序经常带有谷歌和微软的“推荐”徽章，它们却捕获了ChatGPT、Claude和Gemini等十大主流AI平台的所有提示和响应。

数据收集始于2025年7月9日的一次静默更新，将其版本更新至5.5.0。这些扩展程序通过向AI聊天页面注入脚本、覆盖浏览器网络功能以拦截原始API流量，并最终将对话——包括个人困境、健康问题、财务细节和专有代码——导出到Urban VPN的服务器，声称用于“营销分析”。这些信息随后被分享给BiScience，一家与发行商Urban Cyber Security Inc.关联的数据经纪公司。

具有讽刺意味的是，这些扩展程序经常宣传“AI保护”功能，警告用户不要共享敏感数据，却同时收集并出售正是这些数据。它们的披露信息具有误导性，应用商店列表中谎称数据不会出售给第三方，这与它们自己的隐私政策相矛盾。谷歌和微软的“推荐”徽章尤其令人担忧，因为它们暗示着一个本应能检测出这种严重侵犯用户隐私和平台政策行为的审查过程却失败了。强烈建议用户立即卸载所有受影响的扩展程序，因为自2025年7月以来所有的AI对话都可能已被泄露。

---

## 3. 无图形API

**原文标题**: No Graphics API

**原文链接**: [https://www.sebastianaaltonen.com/blog/no-graphics-api](https://www.sebastianaaltonen.com/blog/no-graphics-api)

生成摘要出错

---

## 4. 人工智能将使形式化验证成为主流

**原文标题**: AI will make formal verification go mainstream

**原文链接**: [https://martin.kleppmann.com/2025/12/08/ai-formal-verification.html](https://martin.kleppmann.com/2025/12/08/ai-formal-verification.html)

在2025年12月8日发表的一篇文章中，Martin Kleppmann预测人工智能（AI）将把形式化验证（FV）推向主流软件工程。传统上，FV利用Rocq、Isabelle和Lean等工具，根据形式化规范从数学上证明代码的正确性，一直是一种小众实践。它极其困难、费力，且需要专业知识——例如，验证seL4微内核耗费了20人年的精力。这种高昂的成本历史上使其在经济上对于大多数工业应用而言不可行。

然而，人工智能驱动的编码助手在生成证明脚本方面正迅速改进，而这个过程目前需要大量的人力投入。Kleppmann预计在不久的将来会实现完全自动化，这将大幅降低FV的成本并使其易于普及。这也带来了一个关键需求：相较于人工审查，人工智能生成的代码可以由人工智能进行形式化验证，证明检查器将确保其有效性，并消除大型语言模型（LLM）的“幻觉”。

尽管定义准确的形式化规范仍然是一个挑战，但这比手动编写证明要容易得多，人工智能最终也能在这方面提供帮助。Kleppmann设想了一个未来，开发人员只需指定所需的代码属性，人工智能将生成实现及其经过验证的证明，从而消除了人工代码审查的必要性。总之，人工智能使FV大大降低了成本，对于可靠的人工智能生成代码至关重要，其精确性抵消了LLM的不精确性，这预示着它即将被主流采用，而文化接受是主要障碍。

---

## 5. Announcing the Beta release of ty

**原文标题**: Announcing the Beta release of ty

**原文链接**: [https://astral.sh/blog/ty](https://astral.sh/blog/ty)

Astral, creators of `uv` and `Ruff`, has announced the Beta release of `ty`, an extremely fast Python type checker and language server written in Rust. Designed as a high-performance alternative to tools like mypy and Pyright, `ty` is already used exclusively in Astral's projects and is recommended for production use by motivated users.

`ty` is built on core principles of obsessive performance, correctness, and ergonomics. It boasts significant speed improvements, running 10x to 60x faster than mypy and Pyright without caching. Its incremental architecture, designed for language servers, makes live updates dramatically faster, with re-computations occurring in milliseconds. It pushes the state of the art with features like first-class intersection types, advanced type narrowing, and sophisticated reachability analysis, aiming for more accurate feedback and fewer false positives.

The tool features a best-in-class diagnostic system, inspired by the Rust compiler, providing rich context from multiple files to explain errors and suggest fixes. `ty` offers full Language Server Protocol (LSP) support, including Go to Definition, Auto-Complete, and Semantic Syntax Highlighting, and is available via `uv tool install ty@latest` or a VS Code extension.

Built openly under the MIT license with dozens of contributors, `ty` plans for a Stable release next year, focusing on stability, completing Python typing specification features, and first-class support for libraries like Pydantic and Django. Longer-term, `ty` will power semantic capabilities across the entire Astral toolchain, including dead code elimination and type-aware linting, furthering Astral's goal to enhance Python's productivity.

---

## 6. GitHub Actions 价格调整

**原文标题**: Pricing Changes for GitHub Actions

**原文链接**: [https://resources.github.com/actions/2026-pricing-changes-for-github-actions/](https://resources.github.com/actions/2026-pricing-changes-for-github-actions/)

GitHub 宣布了其 Actions 定价更新，尤其值得注意的是，推迟了此前宣布的自托管 GitHub Actions 的计费变更。这一决定是在听取社区反馈后做出的，GitHub 承认他们“未能准确把握”，需要通过倾听开发者、客户和合作伙伴的意见来重新评估其方法。

尽管有所推迟，GitHub 仍将大幅降低 GitHub 托管型运行器的价格，从 2026 年 1 月 1 日起，成本将降低高达 39%。这是通过将所有运行器尺寸的价格大约降低 40% 来实现的，同时引入了每分钟 0.002 美元的 Actions 云平台新费用，该费用已包含在新的、更低的托管运行器费率中。

这些变更的初衷是为了使成本与使用情况更加紧密地匹配，因为自托管运行器过去一直免费使用 GitHub 的基础设施，由托管运行器定价进行补贴。在 Actions 后端进行了大规模重新架构以处理庞大规模（现在每天处理 7100 万个作业）之后，这种重新调整旨在推动进一步的创新。

对客户的总体影响微乎其微：96% 的客户将不会看到变化，而受影响的 4% 客户中，有 85% 的账单将减少，剩余的 15% 则面临约 13 美元的中位数增长。Actions 对公共仓库仍然免费，GitHub Enterprise Server 的定价不受影响。

GitHub 还确认将继续投资于自托管体验，引入了 GitHub 规模集客户端、多标签支持、Actions Runner Controller (ARC) 0.14.0 和 Actions 数据流等功能，以增强可扩展性和可观测性。此前宣布的自托管运行器收费的 2026 年 3 月 1 日日期现已搁置。

---

## 7. 这不是未来

**原文标题**: This is not the future

**原文链接**: [https://blog.mathieui.net/this-is-not-the-future.html](https://blog.mathieui.net/this-is-not-the-future.html)

在《这不是未来》一文中，mathieui 强烈反对科技行业普遍存在的“某些新技术不可避免”的论调，将其斥为“令人作呕”，并坚称“没有什么事是不可避免的”。作者批评现代技术具有滥用性，认为用户（从普通大众到老年人）都被软硬件“训练得甘于被滥用”，被动接受持续的变化，并因缺乏控制而忍受挫败。

文章谴责那些不加批判的科技狂热者，并指出“同意、炒作和预设的消费者需求是如何通过营销和长期滥用被制造出来的”。文章列举了一系列技术和实践——包括联网床、AI浏览器、无法修复的设备、NFT、元宇宙、“Copilot PC”以及用于AI训练的强制数据共享——明确指出这些都是“并非不可避免”的事例。

尽管承认有些产品确实不错，但作者最终将这些（常常带来痛苦的）发展归咎于“科技骗子”，认为他们通过利用个人数据和注意力来推动这些发展。文章最后强调，每一个选择都是影响未来的政治声明，我们没有必要成为这些趋势的帮凶。

---

## 8. 谋智正在作死吗？

**原文标题**: Is Mozilla trying hard to kill itself?

**原文链接**: [https://infosec.press/brunomiguel/is-mozilla-trying-hard-to-kill-itself](https://infosec.press/brunomiguel/is-mozilla-trying-hard-to-kill-itself)

文章对Mozilla新任首席执行官Enzor-DeMeo在“The Verge”采访中的一番言论表达了深切关注。据报道，这位首席执行官提到，在Firefox中禁用广告拦截器可能会带来1.5亿美元的收入，尽管他声称不想这样做，并称其“偏离了使命”。

作者作为一名长期Firefox用户，将此解读为一个强烈暗示：尽管首席执行官口头表示不情愿，但为了经济利益，取消广告拦截器仍在考虑之中。作者强调，Firefox对开放标准、开放网络及其强大的附加组件系统（尤其是实用的广告拦截器）的承诺，是吸引并留住其忠实用户群体的关键特性，特别是那些注重隐私的科技爱好者。

作者认为，取消广告拦截器将消除Firefox相对于Chromium的一大优势，损害其对抗恶意广告的重要安全功能，并疏远其核心社区。此举可能对该项目产生负面影响，因为这些精通技术的用户经常影响他人的技术选择。

作者在承认Mozilla需要收入的同时，质疑首席执行官为何要公开提出一个他声称不情愿的选择，暗示此举使得这种可能性依然存在，并有产生负面公关的风险。作者仍持“观望态度”，希望自己的解读有误，但又担心这一选择仍然“摆在台面上”。

---

## 9. Thin desires are eating life

**原文标题**: Thin desires are eating life

**原文链接**: [https://www.joanwestenberg.com/thin-desires-are-eating-your-life/](https://www.joanwestenberg.com/thin-desires-are-eating-your-life/)

生成摘要时出错

---

## 10. “Super secure” messaging app leaks everyone's phone number

**原文标题**: “Super secure” messaging app leaks everyone's phone number

**原文链接**: [https://ericdaigle.ca/posts/super-secure-maga-messaging-app-leaks-everyones-phone-number/](https://ericdaigle.ca/posts/super-secure-maga-messaging-app-leaks-everyones-phone-number/)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 2 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 3 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 4 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 5 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 6 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 7 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 8 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 9 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 10 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 11 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 12 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 13 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 14 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 15 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 16 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 17 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 18 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 19 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 20 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 21 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 22 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 23 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 24 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 25 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 26 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 27 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 28 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 29 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 30 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 31 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 32 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 33 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 34 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 35 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 36 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 37 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 38 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 39 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 40 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 41 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 42 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
