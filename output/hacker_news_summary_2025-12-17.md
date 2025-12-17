# Hacker News 热门文章摘要 (2025-12-17)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

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

## 11. Secret Documents Show Pepsi and Walmart Colluded to Raise Food Prices

**原文标题**: Secret Documents Show Pepsi and Walmart Colluded to Raise Food Prices

**原文链接**: [https://www.thebignewsletter.com/p/secret-documents-show-pepsi-and-walmart](https://www.thebignewsletter.com/p/secret-documents-show-pepsi-and-walmart)

生成摘要时出错

---

## 12. Mozilla appoints new CEO Anthony Enzor-Demeo

**原文标题**: Mozilla appoints new CEO Anthony Enzor-Demeo

**原文链接**: [https://blog.mozilla.org/en/mozilla/leadership/mozillas-next-chapter-anthony-enzor-demeo-new-ceo/](https://blog.mozilla.org/en/mozilla/leadership/mozillas-next-chapter-anthony-enzor-demeo-new-ceo/)

生成摘要时出错

---

## 13. Children with cancer scammed out of millions fundraised for their treatment

**原文标题**: Children with cancer scammed out of millions fundraised for their treatment

**原文链接**: [https://www.bbc.com/news/articles/ckgz318y8elo](https://www.bbc.com/news/articles/ckgz318y8elo)

生成摘要时出错

---

## 14. SHARP, an approach to photorealistic view synthesis from a single image

**原文标题**: SHARP, an approach to photorealistic view synthesis from a single image

**原文链接**: [https://apple.github.io/ml-sharp/](https://apple.github.io/ml-sharp/)

生成摘要时出错

---

## 15. GPT Image 1.5

**原文标题**: GPT Image 1.5

**原文链接**: [https://openai.com/index/new-chatgpt-images-is-here/](https://openai.com/index/new-chatgpt-images-is-here/)

生成摘要时出错

---

## 16. 40 percent of fMRI signals do not correspond to actual brain activity

**原文标题**: 40 percent of fMRI signals do not correspond to actual brain activity

**原文链接**: [https://www.tum.de/en/news-and-events/all-news/press-releases/details/40-percent-of-mri-signals-do-not-correspond-to-actual-brain-activity](https://www.tum.de/en/news-and-events/all-news/press-releases/details/40-percent-of-mri-signals-do-not-correspond-to-actual-brain-activity)

生成摘要时出错

---

## 17. No AI* Here – A Response to Mozilla's Next Chapter

**原文标题**: No AI* Here – A Response to Mozilla's Next Chapter

**原文链接**: [https://www.waterfox.com/blog/no-ai-here-response-to-mozilla/](https://www.waterfox.com/blog/no-ai-here-response-to-mozilla/)

生成摘要时出错

---

## 18. Quill OS: An open-source OS for Kobo's eReaders

**原文标题**: Quill OS: An open-source OS for Kobo's eReaders

**原文链接**: [https://quill-os.org/](https://quill-os.org/)

生成摘要时出错

---

## 19. Coming soon: Simpler pricing and a better experience for GitHub Actions

**原文标题**: Coming soon: Simpler pricing and a better experience for GitHub Actions

**原文链接**: [https://github.blog/changelog/2025-12-16-coming-soon-simpler-pricing-and-a-better-experience-for-github-actions/](https://github.blog/changelog/2025-12-16-coming-soon-simpler-pricing-and-a-better-experience-for-github-actions/)

生成摘要时出错

---

## 20. Ford kills the All-Electric F-150

**原文标题**: Ford kills the All-Electric F-150

**原文链接**: [https://www.wired.com/story/ford-kills-electric-f-150-lightning-for-hybrid/](https://www.wired.com/story/ford-kills-electric-f-150-lightning-for-hybrid/)

生成摘要时出错

---

## 21. Gemini 3 Flash: frontier intelligence built for speed

**原文标题**: Gemini 3 Flash: frontier intelligence built for speed

**原文链接**: [https://blog.google/products/gemini/gemini-3-flash/](https://blog.google/products/gemini/gemini-3-flash/)

生成摘要时出错

---

## 22. JetBlue flight averts mid-air collision with US Air Force jet

**原文标题**: JetBlue flight averts mid-air collision with US Air Force jet

**原文链接**: [https://www.reuters.com/world/americas/jetblue-flight-averts-mid-air-collision-with-us-air-force-jet-2025-12-15/](https://www.reuters.com/world/americas/jetblue-flight-averts-mid-air-collision-with-us-air-force-jet-2025-12-15/)

生成摘要时出错

---

## 23. AWS CEO says replacing junior devs with AI is 'one of the dumbest ideas'

**原文标题**: AWS CEO says replacing junior devs with AI is 'one of the dumbest ideas'

**原文链接**: [https://www.finalroundai.com/blog/aws-ceo-ai-cannot-replace-junior-developers](https://www.finalroundai.com/blog/aws-ceo-ai-cannot-replace-junior-developers)

生成摘要时出错

---

## 24. Problems with D-Bus on the Linux desktop

**原文标题**: Problems with D-Bus on the Linux desktop

**原文链接**: [https://blog.vaxry.net/articles/2025-dbusSucks](https://blog.vaxry.net/articles/2025-dbusSucks)

生成摘要时出错

---

## 25. Upcoming Changes to Let's Encrypt Certificates

**原文标题**: Upcoming Changes to Let's Encrypt Certificates

**原文链接**: [https://community.letsencrypt.org/t/upcoming-changes-to-let-s-encrypt-certificates/243873](https://community.letsencrypt.org/t/upcoming-changes-to-let-s-encrypt-certificates/243873)

生成摘要时出错

---

## 26. Fix HDMI-CEC weirdness with a Raspberry Pi and a $7 cable

**原文标题**: Fix HDMI-CEC weirdness with a Raspberry Pi and a $7 cable

**原文链接**: [https://johnlian.net/posts/hdmi-cec/](https://johnlian.net/posts/hdmi-cec/)

生成摘要时出错

---

## 27. Sega Channel: VGHF Recovers over 100 Sega Channel ROMs (and More)

**原文标题**: Sega Channel: VGHF Recovers over 100 Sega Channel ROMs (and More)

**原文链接**: [https://gamehistory.org/segachannel/](https://gamehistory.org/segachannel/)

生成摘要时出错

---

## 28. Coursera to combine with Udemy

**原文标题**: Coursera to combine with Udemy

**原文链接**: [https://investor.coursera.com/news/news-details/2025/Coursera-to-Combine-with-Udemy-to-Empower-the-Global-Workforce-with-Skills-for-the-AI-Era/default.aspx](https://investor.coursera.com/news/news-details/2025/Coursera-to-Combine-with-Udemy-to-Empower-the-Global-Workforce-with-Skills-for-the-AI-Era/default.aspx)

生成摘要时出错

---

## 29. Japan to revise romanization rules for first time in 70 years

**原文标题**: Japan to revise romanization rules for first time in 70 years

**原文链接**: [https://www.japantimes.co.jp/news/2025/08/21/japan/panel-hepburn-style-romanization/](https://www.japantimes.co.jp/news/2025/08/21/japan/panel-hepburn-style-romanization/)

生成摘要时出错

---

## 30. Bonsai: A Voxel Engine, from scratch

**原文标题**: Bonsai: A Voxel Engine, from scratch

**原文链接**: [https://github.com/scallyw4g/bonsai](https://github.com/scallyw4g/bonsai)

生成摘要时出错

---

## 31. MIT professor shot at his Massachusetts home dies

**原文标题**: MIT professor shot at his Massachusetts home dies

**原文链接**: [https://www.bbc.com/news/articles/cly08y25688o](https://www.bbc.com/news/articles/cly08y25688o)

生成摘要时出错

---

## 32. I ported JustHTML from Python to JavaScript with Codex CLI and GPT-5.2 in hours

**原文标题**: I ported JustHTML from Python to JavaScript with Codex CLI and GPT-5.2 in hours

**原文链接**: [https://simonwillison.net/2025/Dec/15/porting-justhtml/](https://simonwillison.net/2025/Dec/15/porting-justhtml/)

生成摘要时出错

---

## 33. Umbrel – Personal Cloud

**原文标题**: Umbrel – Personal Cloud

**原文链接**: [https://umbrel.com](https://umbrel.com)

生成摘要时出错

---

## 34. The GitHub Actions control plane is no longer free

**原文标题**: The GitHub Actions control plane is no longer free

**原文链接**: [https://www.blacksmith.sh/blog/actions-pricing](https://www.blacksmith.sh/blog/actions-pricing)

生成摘要时出错

---

## 35. VS Code deactivates IntelliCode in favor of the paid Copilot

**原文标题**: VS Code deactivates IntelliCode in favor of the paid Copilot

**原文链接**: [https://www.heise.de/en/news/VS-Code-deactivates-IntelliCode-in-favor-of-the-paid-Copilot-11115783.html](https://www.heise.de/en/news/VS-Code-deactivates-IntelliCode-in-favor-of-the-paid-Copilot-11115783.html)

生成摘要时出错

---

## 36. The appropriate amount of effort is zero

**原文标题**: The appropriate amount of effort is zero

**原文链接**: [https://expandingawareness.org/blog/the-appropriate-amount-of-effort-is-zero/](https://expandingawareness.org/blog/the-appropriate-amount-of-effort-is-zero/)

生成摘要时出错

---

## 37. Economics of Orbital vs. Terrestrial Data Centers

**原文标题**: Economics of Orbital vs. Terrestrial Data Centers

**原文链接**: [https://andrewmccalip.com/space-datacenters](https://andrewmccalip.com/space-datacenters)

生成摘要时出错

---

## 38. Rust GCC backend: Why and how

**原文标题**: Rust GCC backend: Why and how

**原文链接**: [https://blog.guillaume-gomez.fr/articles/2025-12-15+Rust+GCC+backend%3A+Why+and+how](https://blog.guillaume-gomez.fr/articles/2025-12-15+Rust+GCC+backend%3A+Why+and+how)

生成摘要时出错

---

## 39. Vibe coding creates fatigue?

**原文标题**: Vibe coding creates fatigue?

**原文链接**: [https://www.tabulamag.com/p/too-fast-to-think-the-hidden-fatigue](https://www.tabulamag.com/p/too-fast-to-think-the-hidden-fatigue)

生成摘要时出错

---

## 40. AI's real superpower: consuming, not creating

**原文标题**: AI's real superpower: consuming, not creating

**原文链接**: [https://msanroman.io/blog/ai-consumption-paradigm](https://msanroman.io/blog/ai-consumption-paradigm)

生成摘要时出错

---

## 41. Erdős Problem #1026

**原文标题**: Erdős Problem #1026

**原文链接**: [https://terrytao.wordpress.com/2025/12/08/the-story-of-erdos-problem-126/](https://terrytao.wordpress.com/2025/12/08/the-story-of-erdos-problem-126/)

生成摘要时出错

---

## 42. I'm a Tech Lead, and nobody listens to me. What should I do?

**原文标题**: I'm a Tech Lead, and nobody listens to me. What should I do?

**原文链接**: [https://world.hey.com/joaoqalves/i-m-a-tech-lead-and-nobody-listens-to-me-what-should-i-do-e16e454d](https://world.hey.com/joaoqalves/i-m-a-tech-lead-and-nobody-listens-to-me-what-should-i-do-e16e454d)

生成摘要时出错

---

## 43. ArkhamMirror: Airgapped investigation platform with CIA-style hypothesis testing

**原文标题**: ArkhamMirror: Airgapped investigation platform with CIA-style hypothesis testing

**原文链接**: [https://github.com/mantisfury/ArkhamMirror](https://github.com/mantisfury/ArkhamMirror)

生成摘要时出错

---

## 44. The World Happiness Report is beset with methodological problems

**原文标题**: The World Happiness Report is beset with methodological problems

**原文链接**: [https://yaschamounk.substack.com/p/the-world-happiness-report-is-a-sham](https://yaschamounk.substack.com/p/the-world-happiness-report-is-a-sham)

生成摘要时出错

---

## 45. A2UI: A Protocol for Agent-Driven Interfaces

**原文标题**: A2UI: A Protocol for Agent-Driven Interfaces

**原文链接**: [https://a2ui.org/](https://a2ui.org/)

生成摘要时出错

---

## 46. A quarter of US-trained scientists eventually leave

**原文标题**: A quarter of US-trained scientists eventually leave

**原文链接**: [https://arxiv.org/abs/2512.11146](https://arxiv.org/abs/2512.11146)

生成摘要时出错

---

## 47. Tesla reports another Robotaxi crash

**原文标题**: Tesla reports another Robotaxi crash

**原文链接**: [https://electrek.co/2025/12/15/tesla-reports-another-robotaxi-crash-even-with-supervisor/](https://electrek.co/2025/12/15/tesla-reports-another-robotaxi-crash-even-with-supervisor/)

生成摘要时出错

---

## 48. A Safer Container Ecosystem with Docker: Free Docker Hardened Images

**原文标题**: A Safer Container Ecosystem with Docker: Free Docker Hardened Images

**原文链接**: [https://www.docker.com/blog/docker-hardened-images-for-every-developer/](https://www.docker.com/blog/docker-hardened-images-for-every-developer/)

生成摘要时出错

---

## 49. AI is wiping out entry-level tech jobs, leaving graduates stranded

**原文标题**: AI is wiping out entry-level tech jobs, leaving graduates stranded

**原文链接**: [https://restofworld.org/2025/engineering-graduates-ai-job-losses/](https://restofworld.org/2025/engineering-graduates-ai-job-losses/)

生成摘要时出错

---

## 50. Writing a blatant Telegram clone using Qt, QML and Rust. And C++

**原文标题**: Writing a blatant Telegram clone using Qt, QML and Rust. And C++

**原文链接**: [https://kemble.net/blog/provoke/](https://kemble.net/blog/provoke/)

生成摘要时出错

---

## 51. Ideas aren't getting harder to find

**原文标题**: Ideas aren't getting harder to find

**原文链接**: [https://asteriskmag.com/issues/12-books/ideas-arent-getting-harder-to-find](https://asteriskmag.com/issues/12-books/ideas-arent-getting-harder-to-find)

生成摘要时出错

---

## 52. FVWM-95 (2001)

**原文标题**: FVWM-95 (2001)

**原文链接**: [https://fvwm95.sourceforge.net/](https://fvwm95.sourceforge.net/)

生成摘要时出错

---

## 53. The biggest heat pumps

**原文标题**: The biggest heat pumps

**原文链接**: [https://www.bbc.com/news/articles/c17p44w87rno](https://www.bbc.com/news/articles/c17p44w87rno)

生成摘要时出错

---

## 54. Overconsumption is a spiritual problem

**原文标题**: Overconsumption is a spiritual problem

**原文链接**: [https://www.sherryning.com/p/youre-overspending-because-you-lack-values](https://www.sherryning.com/p/youre-overspending-because-you-lack-values)

生成摘要时出错

---

## 55. A kernel bug froze my machine: Debugging an async-profiler deadlock

**原文标题**: A kernel bug froze my machine: Debugging an async-profiler deadlock

**原文链接**: [https://questdb.com/blog/async-profiler-kernel-bug/](https://questdb.com/blog/async-profiler-kernel-bug/)

生成摘要时出错

---

## 56. Yep, Passkeys Still Have Problems

**原文标题**: Yep, Passkeys Still Have Problems

**原文链接**: [https://fy.blackhats.net.au/blog/2025-12-17-yep-passkeys-still-have-problems/](https://fy.blackhats.net.au/blog/2025-12-17-yep-passkeys-still-have-problems/)

生成摘要时出错

---

## 57. A linear-time alternative for Dimensionality Reduction and fast visualisation

**原文标题**: A linear-time alternative for Dimensionality Reduction and fast visualisation

**原文链接**: [https://medium.com/@roman.f/a-linear-time-alternative-to-t-sne-for-dimensionality-reduction-and-fast-visualisation-5cd1a7219d6f](https://medium.com/@roman.f/a-linear-time-alternative-to-t-sne-for-dimensionality-reduction-and-fast-visualisation-5cd1a7219d6f)

生成摘要时出错

---

## 58. A brief history of Times New Roman

**原文标题**: A brief history of Times New Roman

**原文链接**: [https://typographyforlawyers.com/a-brief-history-of-times-new-roman.html](https://typographyforlawyers.com/a-brief-history-of-times-new-roman.html)

生成摘要时出错

---

## 59. Devs say Apple still flouting EU's Digital Markets Act six months on

**原文标题**: Devs say Apple still flouting EU's Digital Markets Act six months on

**原文链接**: [https://www.theregister.com/2025/12/16/apple_dma_complaint/](https://www.theregister.com/2025/12/16/apple_dma_complaint/)

生成摘要时出错

---

## 60. Introduction to Software Development Tooling (2024)

**原文标题**: Introduction to Software Development Tooling (2024)

**原文链接**: [https://bernsteinbear.com/isdt/](https://bernsteinbear.com/isdt/)

生成摘要时出错

---

## 61. Native vs. emulation: World of Warcraft game performance on Snapdragon X Elite

**原文标题**: Native vs. emulation: World of Warcraft game performance on Snapdragon X Elite

**原文链接**: [https://rkblog.dev/posts/pc-hardware/pc-on-arm/x86_versus_arm_native_game/](https://rkblog.dev/posts/pc-hardware/pc-on-arm/x86_versus_arm_native_game/)

生成摘要时出错

---

## 62. Firefox is becoming an AI browser and the internet is not at all happy about it

**原文标题**: Firefox is becoming an AI browser and the internet is not at all happy about it

**原文链接**: [https://www.pcgamer.com/hardware/firefox-is-becoming-an-ai-browser-and-the-internet-is-not-at-all-happy-about-it/](https://www.pcgamer.com/hardware/firefox-is-becoming-an-ai-browser-and-the-internet-is-not-at-all-happy-about-it/)

生成摘要时出错

---

## 63. US threatens EU digital services market access

**原文标题**: US threatens EU digital services market access

**原文链接**: [https://twitter.com/ustraderep/status/2000990028835508258](https://twitter.com/ustraderep/status/2000990028835508258)

生成摘要时出错

---

## 64. The Bob Dylan concert for just one person

**原文标题**: The Bob Dylan concert for just one person

**原文链接**: [https://www.flaggingdown.com/p/the-bob-dylan-concert-for-just-one](https://www.flaggingdown.com/p/the-bob-dylan-concert-for-just-one)

生成摘要时出错

---

## 65. United 777-200 fleet faces an uncertain future after Dulles engine failure

**原文标题**: United 777-200 fleet faces an uncertain future after Dulles engine failure

**原文链接**: [https://liveandletsfly.com/united-airlines-777-200-future/](https://liveandletsfly.com/united-airlines-777-200-future/)

生成摘要时出错

---

## 66. SoundCloud confirms breach after member data stolen, VPN access disrupted

**原文标题**: SoundCloud confirms breach after member data stolen, VPN access disrupted

**原文链接**: [https://www.bleepingcomputer.com/news/security/soundcloud-confirms-breach-after-member-data-stolen-vpn-access-disrupted/](https://www.bleepingcomputer.com/news/security/soundcloud-confirms-breach-after-member-data-stolen-vpn-access-disrupted/)

生成摘要时出错

---

## 67. Chat-tails: Throwback terminal chat, built on Tailscale

**原文标题**: Chat-tails: Throwback terminal chat, built on Tailscale

**原文链接**: [https://tailscale.com/blog/chat-tails-terminal-chat](https://tailscale.com/blog/chat-tails-terminal-chat)

生成摘要时出错

---

## 68. Thomas Piketty: 'The reality is the US is losing control of the world'

**原文标题**: Thomas Piketty: 'The reality is the US is losing control of the world'

**原文链接**: [https://www.lemonde.fr/en/opinion/article/2025/04/12/thomas-piketty-the-reality-is-the-us-is-losing-control-of-the-world_6740140_23.html](https://www.lemonde.fr/en/opinion/article/2025/04/12/thomas-piketty-the-reality-is-the-us-is-losing-control-of-the-world_6740140_23.html)

生成摘要时出错

---

## 69. TLA+ Modeling Tips

**原文标题**: TLA+ Modeling Tips

**原文链接**: [http://muratbuffalo.blogspot.com/2025/12/tla-modeling-tips.html](http://muratbuffalo.blogspot.com/2025/12/tla-modeling-tips.html)

生成摘要时出错

---

## 70. U.S. unemployment rose in November despite job gains

**原文标题**: U.S. unemployment rose in November despite job gains

**原文链接**: [https://www.wsj.com/economy/jobs/jobs-report-october-november-2025-unemployment-economy-7f6eea90](https://www.wsj.com/economy/jobs/jobs-report-october-november-2025-unemployment-economy-7f6eea90)

生成摘要时出错

---

## 71. Dafny: Verification-Aware Programming Language

**原文标题**: Dafny: Verification-Aware Programming Language

**原文链接**: [https://dafny.org/](https://dafny.org/)

生成摘要时出错

---

## 72. Show HN: Learn Japanese contextually while browsing

**原文标题**: Show HN: Learn Japanese contextually while browsing

**原文链接**: [https://lingoku.ai/learn-japanese](https://lingoku.ai/learn-japanese)

生成摘要时出错

---

## 73. Canada's Carney called out for 'utilizing' British spelling

**原文标题**: Canada's Carney called out for 'utilizing' British spelling

**原文链接**: [https://www.bbc.com/news/articles/cj69d89l8l5o](https://www.bbc.com/news/articles/cj69d89l8l5o)

生成摘要时出错

---

## 74. Opus 1.6 Released – Interactive Audio Codec

**原文标题**: Opus 1.6 Released – Interactive Audio Codec

**原文链接**: [https://opus-codec.org/demo/opus-1.6/](https://opus-codec.org/demo/opus-1.6/)

生成摘要时出错

---

## 75. Linux Kernel Rust Code Sees Its First CVE Vulnerability

**原文标题**: Linux Kernel Rust Code Sees Its First CVE Vulnerability

**原文链接**: [https://www.phoronix.com/news/First-Linux-Rust-CVE](https://www.phoronix.com/news/First-Linux-Rust-CVE)

生成摘要时出错

---

## 76. More than 100 rally against data centers at Michigan Capitol

**原文标题**: More than 100 rally against data centers at Michigan Capitol

**原文链接**: [https://www.lansingstatejournal.com/story/news/local/2025/12/16/lansing-state-capitol-data-centers-rally-michigan/87792001007/](https://www.lansingstatejournal.com/story/news/local/2025/12/16/lansing-state-capitol-data-centers-rally-michigan/87792001007/)

生成摘要时出错

---

## 77. Put a ring on it: a lock-free MPMC ring buffer

**原文标题**: Put a ring on it: a lock-free MPMC ring buffer

**原文链接**: [https://h4x0r.org/ring/](https://h4x0r.org/ring/)

生成摘要时出错

---

## 78. Letta Code

**原文标题**: Letta Code

**原文链接**: [https://www.letta.com/blog/letta-code](https://www.letta.com/blog/letta-code)

生成摘要时出错

---

## 79. Creating custom yellow handshake emojis with zero-width joiners

**原文标题**: Creating custom yellow handshake emojis with zero-width joiners

**原文链接**: [https://blog.alexbeals.com/posts/custom-yellow-handshake-emojis-with-zero-width-joiners](https://blog.alexbeals.com/posts/custom-yellow-handshake-emojis-with-zero-width-joiners)

生成摘要时出错

---

## 80. Windows 11 will ask consent before sharing personal files with AI after outrage

**原文标题**: Windows 11 will ask consent before sharing personal files with AI after outrage

**原文链接**: [https://www.windowslatest.com/2025/12/17/microsoft-confirms-windows-11-will-ask-for-consent-before-sharing-your-personal-files-with-ai-after-outrage/](https://www.windowslatest.com/2025/12/17/microsoft-confirms-windows-11-will-ask-for-consent-before-sharing-your-personal-files-with-ai-after-outrage/)

生成摘要时出错

---

## 81. CEOs to Keep Spending on AI, Despite Spotty Returns

**原文标题**: CEOs to Keep Spending on AI, Despite Spotty Returns

**原文链接**: [https://www.wsj.com/tech/ai/ceos-to-keep-spending-on-ai-despite-spotty-returns-2eaeb6b](https://www.wsj.com/tech/ai/ceos-to-keep-spending-on-ai-despite-spotty-returns-2eaeb6b)

生成摘要时出错

---

## 82. Liskell – Haskell Semantics with Lisp Syntax [pdf]

**原文标题**: Liskell – Haskell Semantics with Lisp Syntax [pdf]

**原文链接**: [http://clemens.endorphin.org/ILC07-Liskell-draft.pdf](http://clemens.endorphin.org/ILC07-Liskell-draft.pdf)

生成摘要时出错

---

## 83. Locked out: How a gift card purchase destroyed an Apple account

**原文标题**: Locked out: How a gift card purchase destroyed an Apple account

**原文链接**: [https://appleinsider.com/articles/25/12/13/locked-out-how-a-gift-card-purchase-destroyed-an-apple-account](https://appleinsider.com/articles/25/12/13/locked-out-how-a-gift-card-purchase-destroyed-an-apple-account)

生成摘要时出错

---

## 84. 'It's surreal': How US sanctions lock ICC judges out of daily life

**原文标题**: 'It's surreal': How US sanctions lock ICC judges out of daily life

**原文链接**: [https://www.irishtimes.com/world/us/2025/12/12/its-surreal-us-sanctions-lock-international-criminal-court-judge-out-of-daily-life/](https://www.irishtimes.com/world/us/2025/12/12/its-surreal-us-sanctions-lock-international-criminal-court-judge-out-of-daily-life/)

生成摘要时出错

---

## 85. Four Million U.S. Children Had No Health Insurance in 2024

**原文标题**: Four Million U.S. Children Had No Health Insurance in 2024

**原文链接**: [https://www.scientificamerican.com/article/how-rising-rates-of-uninsured-children-will-increase-pediatric-cancer-deaths/](https://www.scientificamerican.com/article/how-rising-rates-of-uninsured-children-will-increase-pediatric-cancer-deaths/)

生成摘要时出错

---

## 86. California judge rules that Tesla engaged in deceptive marketing for Autopilot

**原文标题**: California judge rules that Tesla engaged in deceptive marketing for Autopilot

**原文链接**: [https://www.cnbc.com/2025/12/16/california-judge-says-tesla-engaged-in-deceptive-autopilot-marketing-.html](https://www.cnbc.com/2025/12/16/california-judge-says-tesla-engaged-in-deceptive-autopilot-marketing-.html)

生成摘要时出错

---

## 87. Mozilla's new CEO is doubling down on an AI future for Firefox

**原文标题**: Mozilla's new CEO is doubling down on an AI future for Firefox

**原文链接**: [https://www.theverge.com/tech/845216/mozilla-ceo-anthony-enzor-demeo](https://www.theverge.com/tech/845216/mozilla-ceo-anthony-enzor-demeo)

生成摘要时出错

---

## 88. The new ChatGPT Images is here

**原文标题**: The new ChatGPT Images is here

**原文链接**: [https://openai.com/index/new-chatgpt-images-is-here/](https://openai.com/index/new-chatgpt-images-is-here/)

生成摘要时出错

---

## 89. FCC chair suggests agency isn't independent, word cut from mission statement

**原文标题**: FCC chair suggests agency isn't independent, word cut from mission statement

**原文链接**: [https://www.axios.com/2025/12/17/brendan-carr-fcc-independent-senate-testimony-website](https://www.axios.com/2025/12/17/brendan-carr-fcc-independent-senate-testimony-website)

生成摘要时出错

---

## 90. FTX insider Caroline Ellison has been moved out of prison

**原文标题**: FTX insider Caroline Ellison has been moved out of prison

**原文链接**: [https://www.businessinsider.com/caroline-ellison-prison-release-ftx-sam-bankman-fried-2025-12](https://www.businessinsider.com/caroline-ellison-prison-release-ftx-sam-bankman-fried-2025-12)

生成摘要时出错

---

## 91. EU household real income per capita up 22% since 2004

**原文标题**: EU household real income per capita up 22% since 2004

**原文链接**: [https://ec.europa.eu/eurostat/web/products-eurostat-news/w/ddn-20251125-2](https://ec.europa.eu/eurostat/web/products-eurostat-news/w/ddn-20251125-2)

生成摘要时出错

---

## 92. MIT Professor Is Fatally Shot in His Home

**原文标题**: MIT Professor Is Fatally Shot in His Home

**原文链接**: [https://www.nytimes.com/2025/12/16/us/mit-professor-shot-brookline-nuno-loureiro.html](https://www.nytimes.com/2025/12/16/us/mit-professor-shot-brookline-nuno-loureiro.html)

生成摘要时出错

---

## 93. Stephen Miller's Dark Plot to Build a MAGA Terror State

**原文标题**: Stephen Miller's Dark Plot to Build a MAGA Terror State

**原文链接**: [https://newrepublic.com/article/204191/stephen-miller-maga-terror-state-dark-plot](https://newrepublic.com/article/204191/stephen-miller-maga-terror-state-dark-plot)

生成摘要时出错

---

## 94. AIsbom – open-source CLI to detect "Pickle Bombs" in PyTorch models

**原文标题**: AIsbom – open-source CLI to detect "Pickle Bombs" in PyTorch models

**原文链接**: [https://github.com/Lab700xOrg/aisbom](https://github.com/Lab700xOrg/aisbom)

生成摘要时出错

---

## 95. O'saasy License Agreement

**原文标题**: O'saasy License Agreement

**原文链接**: [https://osaasy.dev/](https://osaasy.dev/)

生成摘要时出错

---

## 96. We are discontinuing the dark web report

**原文标题**: We are discontinuing the dark web report

**原文链接**: [https://support.google.com/websearch/answer/16767242?hl=en](https://support.google.com/websearch/answer/16767242?hl=en)

生成摘要时出错

---

## 97. Reverse-engineering the RK3588 NPU: Hacking limits to run vision transformers

**原文标题**: Reverse-engineering the RK3588 NPU: Hacking limits to run vision transformers

**原文链接**: [https://amohan.dev/blog/2025/shard-optimizing-vision-transformers-edge-npu/](https://amohan.dev/blog/2025/shard-optimizing-vision-transformers-edge-npu/)

生成摘要时出错

---

## 98. Should we fear Microsoft's monopoly?

**原文标题**: Should we fear Microsoft's monopoly?

**原文链接**: [https://www.cursor.tue.nl/en/background/2025/december/week-2/should-we-fear-microsofts-monopoly](https://www.cursor.tue.nl/en/background/2025/december/week-2/should-we-fear-microsofts-monopoly)

生成摘要时出错

---

## 99. UK to "encourage" Apple and Google to put nudity-blocking systems on phones

**原文标题**: UK to "encourage" Apple and Google to put nudity-blocking systems on phones

**原文链接**: [https://arstechnica.com/tech-policy/2025/12/uk-to-encourage-apple-and-google-to-put-nudity-blocking-systems-on-phones/](https://arstechnica.com/tech-policy/2025/12/uk-to-encourage-apple-and-google-to-put-nudity-blocking-systems-on-phones/)

生成摘要时出错

---

## 100. UK Lawmakers Propose Mandatory On-Device Surveillance and VPN Age Verification

**原文标题**: UK Lawmakers Propose Mandatory On-Device Surveillance and VPN Age Verification

**原文链接**: [https://reclaimthenet.org/uk-lawmakers-propose-mandatory-on-device-surveillance-and-vpn-age-verification](https://reclaimthenet.org/uk-lawmakers-propose-mandatory-on-device-surveillance-and-vpn-age-verification)

生成摘要时出错

---

