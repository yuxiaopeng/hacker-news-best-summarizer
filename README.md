# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-06-10.md)

*最后自动更新时间: 2026-06-10 21:45:45*
## 1. 克劳德寓言5

**原文标题**: Claude Fable 5

**原文链接**: [https://www.anthropic.com/news/claude-fable-5-mythos-5](https://www.anthropic.com/news/claude-fable-5-mythos-5)

Anthropic 推出了 Claude Fable 5 和 Claude Mythos 5，这是他们迄今为止最强大的 AI 模型。Fable 5 是一个通用发布的“Mythos 级别”模型，在软件工程、知识工作、视觉和科学研究等领域展现出最先进的性能。显著成就包括为 Stripe 将数月的工程工作压缩至数天、仅凭视觉自主玩转《宝可梦火红》和《异星工厂》等复杂游戏，以及设计 3D 模型。

Mythos 5 作为相同的底层模型，为有限的网络防御者和基础设施提供商（最初通过 Project Glasswing 项目）提供解除限制的防护措施，从而提供全球最强的网络安全能力。它还将药物设计速度提高了十倍，并在分子生物学和基因组学领域持续生成新颖的科学假设。

认识到如此强大 AI 的风险，Fable 5 包含了新的、经过审慎调整的防护措施。对于网络安全和高级生物/化学等敏感主题的查询会自动重定向到 Claude Opus 4.8，以防止滥用。这些回退发生在不到 5% 的会话中，确保安全的同时不断完善系统。

早期反馈赞扬 Fable 5 解决长期问题、执行自主编码、展现资深研究科学家级别的推理能力以及更好地理解用户意图的能力。定价为每百万输入代币 10 美元、每百万输出代币 50 美元，此次发布旨在安全快速地扩大对高级 AI 模型的访问。

---

## 2. macOS Container Machines

**原文标题**: macOS Container Machines

**原文链接**: [https://github.com/apple/container/blob/main/docs/container-machine.md](https://github.com/apple/container/blob/main/docs/container-machine.md)

生成摘要时出错

---

## 3. If Claude Fable stops helping you, you'll never know

**原文标题**: If Claude Fable stops helping you, you'll never know

**原文链接**: [https://jonready.com/blog/posts/claude-fable5-is-allowed-to-sabotage-your-app-if-youre-a-competitor.html](https://jonready.com/blog/posts/claude-fable5-is-allowed-to-sabotage-your-app-if-youre-a-competitor.html)

生成摘要时出错

---

## 4. 德国裁定谷歌须对AI概览中的虚假回答负责。

**原文标题**: German ruling declares Google liable for false answers in AI Overviews

**原文链接**: [https://the-decoder.com/landmark-german-ruling-declares-googles-ai-overviews-are-googles-own-words-and-makes-it-liable-for-false-answers/](https://the-decoder.com/landmark-german-ruling-declares-googles-ai-overviews-are-googles-own-words-and-makes-it-liable-for-false-answers/)

生成摘要时出错

---

## 5. 制作1993年画风

**原文标题**: Making Graphics Like it's 1993

**原文链接**: [https://staniks.github.io/articles/catlantean-3d-blog-1/](https://staniks.github.io/articles/catlantean-3d-blog-1/)

《Catlantean 3D》是一款复古风格的第一人称射击游戏，力求重现90年代初期的画面，特别是320x240分辨率和严格的256色调色板。开发者给自己施加了严格的限制：从零开始构建一切，手动渲染图形，以及混音，同时使用现代编译器和有限的平台抽象层。目标是制作一款精致有趣的游戏，而不仅仅是一个技术演示。

一个基本要素是精心策划的256色调色板，经过反复完善，以包含诸如透明度、纯黑/白，以及特定游戏元素（例如血液、钥匙、用于Catlantis背景的沙漠色调、用于技术设施的灰色）的颜色。

为了在调色板限制内实现动态光照，游戏采用了预处理的“颜色映射表”（colormap）。这个由调色板索引组成的二维矩阵允许高效地O(1)查找着色颜色。对于256种基础颜色中的每一种，都计算出31种更深的变体。将一个变暗因子应用于目标RGB颜色，然后使用Oklab色彩空间找到调色板中最接近的感知颜色，并进行细微的色相偏移以产生更温暖的暗色。这个颜色映射表显著增加了原本扁平的游戏世界的深度。

资产创建融合了两种方法。复杂的动画精灵（如敌人）通过Python脚本从Blender 3D模型高效预渲染，利用Blender的合成功能在调色板量化之前增强对比度。相比之下，需要情感细微差别、清晰度或精确像素控制的元素，例如状态栏头像、拾取物和HUD，则采用手绘。这种方法确保了像素比例的一致性以及刻意而连贯的视觉风格。

---

## 6. 打造HTML优先网站，用户一夜间翻倍

**原文标题**: Building an HTML-first site doubled our users overnight

**原文链接**: [https://mohkohn.co.uk/writing/html-first/](https://mohkohn.co.uk/writing/html-first/)

作者是某公用事业公司的承包商，他面临一个严峻挑战：一个过时的ASP表单和一个失败且无法访问的React应用，导致服务申请率低下，使这家受监管的垄断企业面临数百万美元的罚款风险。此前，两次昂贵的尝试都以失败告终。

他的解决方案是使用Astro构建一个HTML优先的网站，优先考虑通用可访问性。核心逻辑是，一项公共服务必须能在“所有可能的机器上”运行，即使在网络连接不佳的情况下也要确保数据持久性，灵感来源于有人通过PlayStation Portable的有限浏览器访问GOV.UK的经历。

实施时，他将表单向导的每一步都做成独立的页面，在重定向之前将数据提交到后端进行验证和存储。这确保了数据永不丢失。对于客户端验证，他开发了一个HTML Web组件，它渐进式增强了原生的浏览器验证，提供了现代用户体验，同时在JavaScript缺失或失败时能回退到浏览器或后端验证。该网站还符合WCAG AA可访问性标准。

结果是变革性的：用户完成率“一夜之间翻倍”。许多新用户甚至没有被基于JavaScript的分析工具追踪到，这揭示了一个此前未被充分服务的群体。数据持久性证明了其价值，一位用户在一个月前开始填写表单后才完成它。

作者倡导一个成熟的软件行业，它应优先考虑通用访问，而非“蛮荒时代”的做法，构建能够为所有用户（无论设备或连接如何）正常运行的健壮应用，从而确保长寿性和可访问性。

---

## 7. 那些认为AI会取代员工的首席执行官，根本就是不称职的。

**原文标题**: CEOs who think AI replaces their employees are just bad CEOs

**原文链接**: [https://www.techdirt.com/2026/06/09/ceos-who-think-ai-replaces-their-employees-are-just-bad-ceos/](https://www.techdirt.com/2026/06/09/ceos-who-think-ai-replaces-their-employees-are-just-bad-ceos/)

The article asserts that CEOs who believe artificial intelligence can entirely replace their employees are fundamentally "bad CEOs." It argues that while AI tools are indeed powerful, they do not negate the need for human work. The author further speculates that such a mindset indicates a CEO who is self-important and likely harbors a general dislike for their employees.

---

## 8. FCC wants to kill burner phones by forcing telecoms to get all customers' IDs

**原文标题**: FCC wants to kill burner phones by forcing telecoms to get all customers' IDs

**原文链接**: [https://www.404media.co/fcc-wants-to-kill-burner-phones-by-forcing-telecoms-to-get-all-customers-ids/](https://www.404media.co/fcc-wants-to-kill-burner-phones-by-forcing-telecoms-to-get-all-customers-ids/)

生成摘要时出错

---

## 9. 微软开源工具遭入侵，窃取AI开发者密码

**原文标题**: Microsoft's open source tools were hacked to steal passwords of AI developers

**原文链接**: [https://techcrunch.com/2026/06/08/microsofts-open-source-tools-were-hacked-to-steal-passwords-of-ai-developers/](https://techcrunch.com/2026/06/08/microsofts-open-source-tools-were-hacked-to-steal-passwords-of-ai-developers/)

Microsoft has temporarily disabled access to dozens of its open source projects on GitHub after hackers injected password-stealing malware into their code. The affected projects are primarily related to Microsoft's Azure cloud service and tools used by AI developers, including those for Claude Code, Gemini's command-line interface, and VS Code.

Security firms Cloudsmith and OpenSourceMalware first identified the breach, noting the malware's ability to steal passwords and sensitive credentials when users opened the compromised tools within their AI coding applications. While the exact number of affected users is unknown, at least 70 Microsoft projects were reportedly disabled on GitHub due to a violation of its terms of service.

Microsoft confirmed the removal of repositories to investigate "potential malicious content." A spokesperson, Ben Hope, stated that some repositories have since been restored, while others remain offline. Microsoft has notified a "small number" of customers who may have downloaded content from the affected repositories and continues its investigation.

This incident marks another "supply chain" attack, targeting widely used open source code to compromise a large number of users. It's also Microsoft's second known breach involving its open source projects in recent weeks, with OpenSourceMalware suggesting this latest incident is a "re-compromise" of the Durable Task project, which was also hacked in mid-May.

---

## 10. Cleaning up after AI rockstar developers

**原文标题**: Cleaning up after AI rockstar developers

**原文链接**: [https://www.codingwithjesse.com/blog/rockstar-developers/](https://www.codingwithjesse.com/blog/rockstar-developers/)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 2 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 3 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 4 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 5 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 6 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 7 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 8 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 9 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 10 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 11 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 12 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 13 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 14 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 15 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 16 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 17 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 18 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 19 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 20 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 21 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 22 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 23 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 24 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 25 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 26 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 27 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 28 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 29 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 30 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 31 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 32 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 33 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 34 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 35 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 36 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 37 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 38 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 39 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 40 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 41 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 42 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 43 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 44 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 45 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 46 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 47 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 48 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 49 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 50 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 51 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 52 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 53 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 54 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 55 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 56 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 57 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 58 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 59 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 60 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 61 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 62 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 63 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 64 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 65 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 66 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 67 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 68 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 69 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 70 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 71 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 72 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 73 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 74 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 75 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 76 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 77 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 78 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 79 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 80 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 81 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 82 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 83 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 84 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 85 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 86 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 87 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 88 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 89 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 90 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 91 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 92 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 93 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 94 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 95 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 96 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 97 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 98 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 99 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 100 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 101 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 102 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 103 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 104 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 105 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 106 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 107 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 108 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 109 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 110 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 111 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 112 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 113 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 114 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 115 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 116 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 117 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 118 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 119 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 120 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 121 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 122 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 123 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 124 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 125 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 126 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 127 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 128 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 129 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 130 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 131 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 132 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 133 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 134 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 135 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 136 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 137 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 138 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 139 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 140 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 141 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 142 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 143 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 144 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 145 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 146 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 147 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 148 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 149 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 150 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 151 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 152 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 153 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 154 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 155 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 156 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 157 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 158 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 159 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 160 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 161 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 162 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 163 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 164 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 165 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 166 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 167 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 168 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 169 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 170 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 171 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 172 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 173 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 174 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 175 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 176 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 177 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 178 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 179 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 180 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 181 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 182 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 183 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 184 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 185 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 186 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 187 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 188 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 189 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 190 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 191 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 192 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 193 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 194 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 195 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 196 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 197 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 198 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 199 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 200 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 201 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 202 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 203 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 204 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 205 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 206 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 207 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 208 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 209 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 210 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 211 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 212 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 213 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 214 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 215 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
