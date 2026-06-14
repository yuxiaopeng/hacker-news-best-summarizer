# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-06-14.md)

*最后自动更新时间: 2026-06-14 20:32:15*
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

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 2 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 3 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 4 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 5 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 6 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 7 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 8 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 9 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 10 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 11 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 12 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 13 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 14 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 15 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 16 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 17 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 18 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 19 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 20 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 21 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 22 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 23 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 24 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 25 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 26 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 27 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 28 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 29 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 30 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 31 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 32 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 33 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 34 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 35 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 36 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 37 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 38 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 39 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 40 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 41 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 42 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 43 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 44 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 45 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 46 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 47 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 48 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 49 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 50 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 51 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 52 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 53 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 54 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 55 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 56 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 57 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 58 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 59 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 60 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 61 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 62 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 63 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 64 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 65 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 66 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 67 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 68 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 69 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 70 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 71 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 72 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 73 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 74 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 75 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 76 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 77 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 78 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 79 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 80 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 81 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 82 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 83 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 84 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 85 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 86 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 87 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 88 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 89 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 90 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 91 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 92 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 93 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 94 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 95 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 96 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 97 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 98 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 99 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 100 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 101 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 102 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 103 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 104 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 105 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 106 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 107 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 108 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 109 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 110 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 111 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 112 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 113 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 114 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 115 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 116 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 117 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 118 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 119 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 120 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 121 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 122 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 123 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 124 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 125 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 126 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 127 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 128 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 129 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 130 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 131 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 132 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 133 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 134 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 135 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 136 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 137 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 138 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 139 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 140 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 141 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 142 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 143 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 144 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 145 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 146 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 147 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 148 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 149 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 150 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 151 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 152 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 153 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 154 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 155 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 156 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 157 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 158 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 159 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 160 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 161 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 162 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 163 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 164 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 165 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 166 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 167 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 168 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 169 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 170 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 171 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 172 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 173 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 174 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 175 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 176 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 177 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 178 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 179 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 180 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 181 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 182 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 183 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 184 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 185 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 186 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 187 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 188 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 189 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 190 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 191 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 192 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 193 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 194 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 195 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 196 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 197 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 198 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 199 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 200 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 201 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 202 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 203 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 204 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 205 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 206 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 207 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 208 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 209 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 210 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 211 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 212 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 213 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 214 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 215 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 216 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 217 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 218 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 219 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
