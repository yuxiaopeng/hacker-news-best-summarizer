# Hacker News 热门文章摘要 (2026-06-14)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 里约热内卢的“本土”大语言模型，看来是现有模型的一个合并版。

**原文标题**: Rio de Janeiro's "homegrown" LLM appears to be a merge of an existing model

**原文链接**: [https://github.com/nex-agi/Nex-N2/issues/4](https://github.com/nex-agi/Nex-N2/issues/4)

Nex-AGI提出一项指控，声称IplanRIO宣称为原创的大型语言模型 (LLM) Rio-3.5-Open-397B并非“自主研发”，而是现有模型的直接逐元素合并。

Nex-AGI指出，Rio-3.5-Open-397B的权重中约60%来自他们自己的模型Nex-N2_pro，40%来自官方的Qwen3.5-397B-A17B基座。他们声称没有证据表明IplanRIO进行了自主训练。

Nex-AGI提供了两项关键证据：
1.  **自我识别：** 当移除Rio-3.5-Open-397B模型中硬编码的“你是Rio”系统提示后，该模型在79%的情况下会识别自己为“我是Nex，来自Nex-AGI”，甚至会复述Nex-AGI的特定背景故事，而从未将自己识别为“Rio”。
2.  **权重分析：** Rio-3.5-Open-397B中的每个权重张量，在所有60个层和网络组件中，都一致地显示出Nex和Qwen模型精确的0.6/0.4混合比例。Nex-AGI指出，这种一致的插值无法用标准的微调过程来解释。

---

## 2. Phoenix LiveView 1.2

**原文标题**: Phoenix LiveView 1.2

**原文链接**: [https://phoenixframework.org/blog/phoenix-liveview-1-2-released](https://phoenixframework.org/blog/phoenix-liveview-1-2-released)

Phoenix LiveView 1.2 已发布，主要特性是 **共置 CSS**。基于 LiveView 1.1 中的共置 Hook 和 JavaScript，开发者现在可以使用 `<style :type={MyApp.ColocatedCSS}>` 直接在 HEEx 模板中嵌入 CSS。LiveView 会在编译时提取此 CSS，供 Tailwind 或 Esbuild 等打包工具处理。

共置样式的一个主要挑战是作用域。LiveView 通过利用新的 `@scope` CSS 规则来解决此问题，该规则接受根选择器和可选的限制选择器。为实现这一点，LiveView 为所有最外层模板元素引入了一个可配置的 `phx-r` 属性（作为限制选择器），并为组件根引入了唯一的 `phx-css-*` 属性。这使得像 `@scope ([phx-css-foo]) to ([phx-r]) { p { font-weight: bold; } }` 这样的 CSS 规则只能应用于特定组件的边界内。

尽管 `@scope` 的技术基础已经奠定，但由于浏览器支持有限（截至 2026 年 6 月），LiveView 1.2 默认不提供此功能。相反，它提供了一个 `@behaviour` 用于实现自定义作用域策略，并且 `@scope` 的实现细节在文档中为早期采用者进行了详细说明。共置 CSS 的实现也导致 HEEx 模板编译进行了重大重构，将其拆分为词法分析和解析步骤，以提高可维护性。

LiveView 1.2 的其他显著改进包括：
*   用于格式化 `<script>` 和 `<style>` 标签的 `Phoenix.LiveView.HTMLFormatter.TagFormatter`。
*   使用 `push_event` 发送 `Phoenix.LiveView.JS` 结构体时自动编码。
*   HEEx 调试注解（`@debug_heex_annotations`、`@debug_attributes`）的模块级配置。
*   按类别配置测试警告。
*   JavaScript 客户端的独立文档。

本次发布鼓励反馈和错误报告，并特别感谢 Dashbit 赞助了这项工作。

---

## 3. 牧羊犬：Fable出品

**原文标题**: Shepherd's Dog: A Game by Fable

**原文链接**: [https://koenvangilst.nl/lab/claude-fable-shepherds-dog](https://koenvangilst.nl/lab/claude-fable-shepherds-dog)

文章描述了一位用户对Anthropic公司最近发布的、据称“危险”的AI模型进行的测试。作者挑战该AI模型，一次性构建他们构思多年的一个游戏理念——“牧羊犬”。

经过45分钟的推理，并花费了超过20欧元的token，该AI模型成功生成了一个完整的、2,319行且零依赖的游戏`index.html`文件。作者对此表示欣喜，称这款游戏“非常有趣，完全符合我的想象”，并指出这是AI模型首次为他们一次性实现这样的成果。该文章提供了链接，可用于玩这款AI生成的游戏，并查看其他模型之前的尝试。

---

## 4. JavaScript的诞生与消亡 (2014)

**原文标题**: The Birth and Death of JavaScript (2014)

**原文链接**: [https://www.destroyallsoftware.com/talks/the-birth-and-death-of-javascript](https://www.destroyallsoftware.com/talks/the-birth-and-death-of-javascript)

本文介绍了Gary Bernhardt在2014年PyCon大会上发表的演讲“JavaScript的诞生与消亡”。这场被描述为“科幻/喜剧/极其严肃”的演讲，追溯了JavaScript和编程从1995年到未来2035年的历史。

该演讲采取了平衡的视角，坦诚地讨论了该语言的缺陷，同时最终强调了它对行业“极其积极”的影响。对于那些对Bernhardt更严肃的编程见解感兴趣的人，推荐观看他的“Destroy All Software”系列截屏视频。

本文还推广了一个名为“Execute Program”的平台，该平台提供关于TypeScript、现代JavaScript、SQL和正则表达式等主题的互动课程，其中包含数百个实时代码示例。

---

## 5. 吃豆人，但你是幽灵

**原文标题**: Pac-Man, but you're the ghost

**原文链接**: [https://garrit.xyz/posts/2026-06-13-pac-man-but-you-re-the-ghost](https://garrit.xyz/posts/2026-06-13-pac-man-but-you-re-the-ghost)

生成摘要时出错

---

## 6. HN 展示: Kage — 将任意网站打包为单个二进制文件，以供离线浏览

**原文标题**: Show HN: Kage – Shadow any website to a single binary for offline viewing

**原文链接**: [https://github.com/tamnd/kage](https://github.com/tamnd/kage)

Kage（影，“影子”）是一个基于Go语言的工具，旨在为动态网站创建完全离线、静态的副本，解决了现代JavaScript密集型页面简单地“保存”时出现的故障问题。

Kage通过驱动一个真实的无头Chrome浏览器工作。对于每个页面，它会等待内容完全渲染和所有JavaScript执行完毕，然后捕获最终的DOM。随后，它会剥离所有脚本，本地化CSS、图片和字体，并重写所有路径，使其相对于本地副本。这个过程会生成一个可浏览的静态`.html`文件文件夹，这些文件不运行任何代码，不进行任何外部网络调用，并且完全离线可用。

主要命令包括`kage clone`（用于镜像一个网站，带有深度、页面限制和范围等选项）和`kage serve`（通过轻量级HTTP服务器预览本地副本）。为了便携性和共享，`kage pack`可以将镜像打包成一个单一文件。这可以是一个开放标准的ZIM存档（兼容Kiwix，可在多种设备上离线阅读），也可以是一个自包含的可执行二进制文件。该二进制文件将Kage和网站内容打包在一起，使其无需安装Kage即可在任何机器上提供内容服务。一个可选的“webview”构建标签允许打包的网站在原生操作系统窗口中打开，提供类似应用程序的体验，而非浏览器标签页。Kage的设计优先考虑网络内容的长期保存、隐私保护和便捷共享。

---

## 7. 瑞士选民否决将人口上限设为一千万的提案

**原文标题**: Swiss voters reject proposal to cap population at ten million

**原文链接**: [https://www.swissinfo.ch/eng/swiss-politics/swiss-voters-reject-proposal-to-cap-population-at-ten-million/91548146](https://www.swissinfo.ch/eng/swiss-politics/swiss-voters-reject-proposal-to-cap-population-at-ten-million/91548146)

文章标题显示，瑞士选民拒绝了一项旨在将该国人口上限设为一千万的提案。

然而，文章内文所提供的内容却完全偏离，讨论的是无国界医生（MSF）在苏丹接触有需要人群时面临的挑战，并指出难以接触到那些需要帮助的人。所提供的正文中没有阐述瑞士投票或其影响的信息。

因此，根据所提供的文本，唯一实质性的信息与无国界医生在苏丹的行动困难有关，而瑞士人口上限投票的细节则完全通过标题传达。

---

## 8. Show HN: Paca – Lightweight Jira alternative for human-AI collaboration

**原文标题**: Show HN: Paca – Lightweight Jira alternative for human-AI collaboration

**原文链接**: [https://github.com/Paca-AI/paca](https://github.com/Paca-AI/paca)

生成摘要时出错

---

## 9. A 'cold blob' in the Atlantic could be a sign of AMOC shutdown

**原文标题**: A 'cold blob' in the Atlantic could be a sign of AMOC shutdown

**原文链接**: [https://www.cnn.com/2026/06/12/climate/cold-blob-atlantic-amoc-ocean-circulation](https://www.cnn.com/2026/06/12/climate/cold-blob-atlantic-amoc-ocean-circulation)

生成摘要时出错

---

## 10. Linux 7.1

**原文标题**: Linux 7.1

**原文链接**: [https://lore.kernel.org/lkml/CAHk-=wi4BF4bMhZNZ1tqs+FFV4OuZRe3ZqdWB+LxRLmRweUzQw@mail.gmail.com/T/#u](https://lore.kernel.org/lkml/CAHk-=wi4BF4bMhZNZ1tqs+FFV4OuZRe3ZqdWB+LxRLmRweUzQw@mail.gmail.com/T/#u)

The displayed page is a robot verification challenge powered by "Anubis," a server protection mechanism. Its primary goal is to prevent AI companies from aggressively scraping website content, which can lead to server crashes and service disruption for all users.

Anubis employs a Proof-of-Work (PoW) mechanism, similar to Hashcash, designed to impose a negligible computational burden on individual legitimate users while creating a significant, cumulative cost for large-scale AI scrapers. This deters abusive data collection.

Currently, Anubis serves as a temporary solution, allowing time for the development of more sophisticated methods like fingerprinting and identifying headless browsers, aiming to reduce the need for PoW challenges for legitimate users. Crucially, modern JavaScript functionality is required for Anubis to operate. Users must disable plugins like JShelter that may block these functions, as JavaScript is mandatory for the current verification due to AI companies altering the 'social contract' of website hosting. Solutions that do not require JavaScript are actively under development.

---

## 11. UK set to announce social media ban for under-16s

**原文标题**: UK set to announce social media ban for under-16s

**原文链接**: [https://www.manchestereveningnews.co.uk/news/uk-news/uk-set-announce-social-media-34119132](https://www.manchestereveningnews.co.uk/news/uk-news/uk-set-announce-social-media-34119132)

生成摘要时出错

---

## 12. The adder at the heart of Intel's 8087 floating-point chip

**原文标题**: The adder at the heart of Intel's 8087 floating-point chip

**原文链接**: [https://www.righto.com/2026/06/intel-8087-adder-reverse-engineered.html](https://www.righto.com/2026/06/intel-8087-adder-reverse-engineered.html)

生成摘要时出错

---

## 13. 里约热内卢市政府的模型 Rio3.5 在最近的基准测试中击败了 Qwen3.7。

**原文标题**: Rio de Janeiro's city government model Rio3.5 beats Qwen3.7 in recent benchmarks

**原文链接**: [https://twitter.com/zenmagnets/status/2065796012820848699](https://twitter.com/zenmagnets/status/2065796012820848699)

生成摘要时出错

---

## 14. Extinction-Level Capitalism

**原文标题**: Extinction-Level Capitalism

**原文链接**: [https://matthewbutterick.com/extinction-level-capitalism.html](https://matthewbutterick.com/extinction-level-capitalism.html)

生成摘要时出错

---

## 15. Caddy compatibility for zeroserve: 3x throughput and 70% lower latency

**原文标题**: Caddy compatibility for zeroserve: 3x throughput and 70% lower latency

**原文链接**: [https://su3.io/posts/zeroserve-caddy-compat](https://su3.io/posts/zeroserve-caddy-compat)

生成摘要时出错

---

## 16. Formal methods and the future of programming

**原文标题**: Formal methods and the future of programming

**原文链接**: [https://blog.janestreet.com/formal-methods-at-jane-street-index/?from_theconsensus=1](https://blog.janestreet.com/formal-methods-at-jane-street-index/?from_theconsensus=1)

生成摘要时出错

---

## 17. Measles surge in Utah sparks fears US could undo decades of progress

**原文标题**: Measles surge in Utah sparks fears US could undo decades of progress

**原文链接**: [https://www.dailymail.com/news/article-15897903/measles-surge-utah-US-elimination-status.html](https://www.dailymail.com/news/article-15897903/measles-surge-utah-US-elimination-status.html)

生成摘要时出错

---

## 18. Running DOS on Behringers DDX3216 with a DIY x86-Bios from Scratch

**原文标题**: Running DOS on Behringers DDX3216 with a DIY x86-Bios from Scratch

**原文链接**: [https://chrisdevblog.com/2026/06/08/running-dos-on-behringers-ddx3216-using-a-diy-x86-bios/](https://chrisdevblog.com/2026/06/08/running-dos-on-behringers-ddx3216-using-a-diy-x86-bios/)

生成摘要时出错

---

## 19. What happens to an economy when it's too hot to work?

**原文标题**: What happens to an economy when it's too hot to work?

**原文链接**: [https://www.bloomberg.com/news/features/2026-06-12/india-s-extreme-heat-is-hurting-its-economy-and-workers](https://www.bloomberg.com/news/features/2026-06-12/india-s-extreme-heat-is-hurting-its-economy-and-workers)

生成摘要时出错

---

## 20. KPMG pulls report on AI usage due to apparent hallucinations

**原文标题**: KPMG pulls report on AI usage due to apparent hallucinations

**原文链接**: [https://techcrunch.com/2026/06/13/kpmg-pulls-report-on-ai-usage-due-to-apparent-hallucinations/](https://techcrunch.com/2026/06/13/kpmg-pulls-report-on-ai-usage-due-to-apparent-hallucinations/)

生成摘要时出错

---

## 21. /architect: Reduce Fable tokens by 80%, Fable orchestrates/reviews, Codex builds

**原文标题**: /architect: Reduce Fable tokens by 80%, Fable orchestrates/reviews, Codex builds

**原文链接**: [https://github.com/DanMcInerney/architect-loop](https://github.com/DanMcInerney/architect-loop)

生成摘要时出错

---

## 22. Orthodox C++ (2016)

**原文标题**: Orthodox C++ (2016)

**原文链接**: [https://bkaradzic.github.io/posts/orthodoxc++/](https://bkaradzic.github.io/posts/orthodoxc++/)

Orthodox C++ (or C+) defines a minimal subset of C++ designed to enhance C while eschewing the complexities of "Modern C++." Its proponents argue that many contemporary C++ features, like RTTI, exceptions, and streams, have proven to be unnecessary, lead to increased code complexity, or impose hidden runtime costs.

The philosophy aims for codebases that are simpler, easier to understand, compatible with older compilers, and more portable. Orthodox C++ strives for a "C-like" readability.

Key "Don't" rules include:
*   **Avoid exceptions:** They incur runtime costs even when unused, offer no compile-time enforcement, and clash with C-style error codes.
*   **No RTTI.**
*   **Use C standard headers:** Prefer `<stdio.h>` over `<cstdio>`.
*   **Opt for `printf` style functions:** Shun C++ streams like `<iostream>`.
*   **Limit STL containers that allocate memory:** Unless explicit memory management is not a concern.
*   **Use metaprogramming sparingly:** Only when it genuinely reduces complexity.
*   **Be wary of new C++ standard features:** Wait for them to mature (e.g., C++year + 5 rule) to ensure compiler adoption and stability.
*   **Avoid modules:** They introduce portability issues, build system complexity, and refactoring without significant benefits for most developers.

Orthodox C++ advocates for pragmatism and simplicity, prioritizing maintainability and broad compatibility. It aligns with similar "minimal C++" approaches and is exemplified in projects like Doom 3 BFG and Qt (configured without RTTI/exceptions).

---

## 23. Our response to the US ban on Fable 5 and Mythos 5

**原文标题**: Our response to the US ban on Fable 5 and Mythos 5

**原文链接**: [https://isaacus.com/blog/our-response-to-the-us-ban-on-fable-5-and-mythos-5](https://isaacus.com/blog/our-response-to-the-us-ban-on-fable-5-and-mythos-5)

生成摘要时出错

---

## 24. AMD Stiffs Researcher $10k Bug Bounty

**原文标题**: AMD Stiffs Researcher $10k Bug Bounty

**原文链接**: [https://www.gadgetreview.com/amd-stiffs-researcher-10000-bug-bounty-after-critical-security-flaw-takes-124-days-to-fix](https://www.gadgetreview.com/amd-stiffs-researcher-10000-bug-bounty-after-critical-security-flaw-takes-124-days-to-fix)

生成摘要时出错

---

## 25. Mmorpg World of ClaudeCraft, vibe coded with Fable 5

**原文标题**: Mmorpg World of ClaudeCraft, vibe coded with Fable 5

**原文链接**: [https://worldofclaudecraft.com/](https://worldofclaudecraft.com/)

生成摘要时出错

---

## 26. 4 things to know about the new sunscreen ingredient the FDA approved

**原文标题**: 4 things to know about the new sunscreen ingredient the FDA approved

**原文链接**: [https://www.npr.org/2026/06/13/nx-s1-5856385/sunscreen-skin-protection-bemotrizinol](https://www.npr.org/2026/06/13/nx-s1-5856385/sunscreen-skin-protection-bemotrizinol)

The FDA has approved bemotrizinol, the first new chemical UV filter for U.S. sunscreens in nearly three decades, an approval widely praised by dermatologists. This ingredient, which will be sold as Parsol Shield, offers several significant advantages.

1.  **Broad-Spectrum and Photostable Protection:** Bemotrizinol provides comprehensive protection against both UVA (aging) and UVB (sunburn) rays. Unlike older U.S. chemical filters like avobenzone, it is photostable, meaning its protective capabilities break down much more slowly in sunlight, offering more consistent and longer-lasting defense.
2.  **Long International Track Record:** Widely used and trusted in Europe and Asia for decades, bemotrizinol's delayed U.S. approval is attributed to the FDA's rigorous classification of sunscreens as over-the-counter drugs, requiring extensive and costly safety and efficacy testing, unlike Europe's cosmetic classification.
3.  **Well-Documented Safety Profile:** The rigorous testing means bemotrizinol boasts more safety data than any other chemical sunscreen ingredient currently approved in the U.S. It has been shown to be non-irritating, causes no reproductive harm, and its larger molecules are minimally absorbed into the bloodstream, addressing key safety concerns raised about other chemical filters and countering misinformation about sunscreen.
4.  **Improved Aesthetics:** Unlike mineral sunscreens (e.g., zinc oxide) which can leave a noticeable white cast, bemotrizinol is transparent on the skin. Its potent protection also reduces the need for a multitude of other chemical filters and stabilizers, promising less greasy and more aesthetically pleasing sunscreen formulations that consumers will be more inclined to use regularly.

This approval is hailed as a major public health victory, improving sunscreen effectiveness, safety, and user experience. Sunscreen products containing bemotrizinol are expected to be available in U.S. stores around September.

---

## 27. As a result of a US Government directive, we are suspending access to Fable 5

**原文标题**: As a result of a US Government directive, we are suspending access to Fable 5

**原文链接**: [https://twitter.com/ClaudeDevs/status/2065597942602531163](https://twitter.com/ClaudeDevs/status/2065597942602531163)

生成摘要时出错

---

## 28. Sam Bankman-Fried loses bid to appeal against fraud conviction in FTX case

**原文标题**: Sam Bankman-Fried loses bid to appeal against fraud conviction in FTX case

**原文链接**: [https://www.theguardian.com/business/2026/jun/12/sam-bankman-fried-loses-appeal](https://www.theguardian.com/business/2026/jun/12/sam-bankman-fried-loses-appeal)

生成摘要时出错

---

