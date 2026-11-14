# Hacker News 热门文章摘要 (2026-11-14)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 黄仁勋辞职

**原文标题**: Jensen Huang resigns

**原文链接**: [https://apnews.com/article/nvidia-megaspeed-china-singapore-huang-5403f152a601cf82ce939f1d24fffa0f](https://apnews.com/article/nvidia-megaspeed-china-singapore-huang-5403f152a601cf82ce939f1d24fffa0f)

英伟达首席执行官黄仁勋宣布，计划在新加坡建造一台名为“Ceerwun项目”的“超高速”人工智能超级计算机。这项倡议旨在将新加坡打造成东南亚的人工智能中心，为训练大型语言模型提供关键基础设施，并培育强大的人工智能生态系统。

黄仁勋强调，每个国家都需要发展自己的“人工智能工厂”——拥有自己的数据、基础设施和模型——并将其描述为一场以“主权人工智能”为核心的新工业革命。新加坡已承诺在未来五年内投入5亿新元（3.7亿美元）以提升其人工智能能力，其中包括支持英伟达的超级计算机项目。此举突显了英伟达在全球人工智能革命中发挥的核心作用，它为先进的人工智能发展提供了必要的硬件和软件。

---

## 2. Microsoft 365 服务降级

**原文标题**: Service degradation on Microsoft 365

**原文链接**: [https://status.cloud.microsoft/](https://status.cloud.microsoft/)

所提供的文本表明 Microsoft 365 存在服务降级。然而，它并未提供有关此次降级性质、范围或影响的具体细节。相反，内容主要阐明了一个技术

---

## 3. FAA issues national ground stop

**原文标题**: FAA issues national ground stop

**原文链接**: [https://www.nbcnews.com/news/us-news/faa-orders-nationwide-ground-stop-departing-flights-reasons-safety-rcna609247](https://www.nbcnews.com/news/us-news/faa-orders-nationwide-ground-stop-departing-flights-reasons-safety-rcna609247)

生成摘要时出错

---

## 4. 安索罗匹克上市

**原文标题**: Anthropic IPO

**原文链接**: [https://ipo.anthropic.com/us/](https://ipo.anthropic.com/us/)

生成摘要时出错

---

## 5. Rust 1.100

**原文标题**: Rust 1.100

**原文链接**: [https://blog.rust-lang.org/2026/11/12/Rust-1.100.0/](https://blog.rust-lang.org/2026/11/12/Rust-1.100.0/)

Rust 1.100.0 为语言及其工具带来了实质性更新。一个主要亮点是 **never 类型 (`!`)** 在十年后正式稳定。这种代表发散计算的空类型现在可以在任何地方命名，并且 `Infallible` 是它的别名。这涉及旧版本中的一个轻微的破坏性更改，将 never 类型的回退从 `()` 切换到了 `!`。

核心的 **Allocator API** 已经稳定，通过新的 `Allocator` trait，库作者可以为 `Vec` 和 `Box` 等类型定义和使用自定义分配器。

`core::mem::DropGuard` 被引入，它是一个辅助类型，在被丢弃时运行一个闭包，简化了函数退出时的清理逻辑。它提供了一个 `dismiss` 函数，用于事务性模式。对于创建零大小类型，`std::mem::conjure_zst` 提供了一个专用的（且 `unsafe` 的）函数。

Cargo 获得了显著改进：
*   一个新的 lint 会报告未使用的依赖，有助于减少构建时间。
*   通过对构建目录的内部重组，Cargo 缓存冲突减少了，提高了可靠性，并为未来的缓存改进铺平了道路。
*   `Cargo min-publish-age` 已经稳定，允许用户配置一个“依赖冷却”期，以便在采用新发布的包版本之前等待最短时间，从而提高供应链安全性。

许多其他 API，例如 `Box::new_in`、`Vec::new_in`、`bool::toggle`、`str::trim_prefix` 和 `UnsafeCell` 的方法，也已稳定。

---

## 6. LibreOffice actually works 365 days a year

**原文标题**: LibreOffice actually works 365 days a year

**原文链接**: [https://twitter.com/LibreOffice/status/2121205272479998268](https://twitter.com/LibreOffice/status/2121205272479998268)

On November 13, 2026, the official LibreOffice Twitter account (@LibreOffice) posted a concise statement affirming the consistent reliability of its software. The tweet declared, "LibreOffice actually works 365 days a year. Just saying," highlighting the software's continuous functionality and dependability. This post garnered significant attention, accumulating 1.237 million views and tens of millions of interactions, indicating its broad reach and resonance with the audience.

---

## 7. 英伟达员工请愿黄仁勋回归

**原文标题**: Nvidia employees petition to bring back Jensen Huang

**原文链接**: [https://www.wired.com/story/nvidia-employees-petition-for-jensen-huangs-return/](https://www.wired.com/story/nvidia-employees-petition-for-jensen-huangs-return/)

英伟达员工正在积极请愿，要求首席执行官黄仁勋复职。黄仁勋最近因多起婚外情报道而辞职，其中一起涉及一名疑似中国情报人员，另一起涉及一名直接下属。黄仁勋曾承认“对妻子不忠”。

黄仁勋辞职前提交的一份内部“意见箱”帖子已吸引了超过1600条评论，许多员工表达了对黄仁勋的强烈支持。评论中包括“让老板回来”的恳求和“再给一次机会”的呼吁，认可了他的贡献。一名员工发送了一封全公司邮件，要求透明化，并表示“我支持黄仁勋”。许多人还在LinkedIn上发帖支持他，没有发现任何支持他辞职的帖子。

员工们担心，这家已损失1万亿美元市值的公司，如果没有其创始人将遭受重创。他们原以为董事会调查会在任何变动前结束，但黄仁勋在调查开始时突然辞职，震惊了许多人。这场危机也促使美国议员和联邦调查局展开调查，并引发了对新芯片出口管制的担忧。董事会主要由黄仁勋的亲信组成，已任命首席财务官Colette Kress为临时首席执行官。员工们普遍认为“英伟达之所以是英伟达，是因为黄仁勋”，并且他的领导对公司的未来至关重要。

---

## 8. HN 展示：我的 300 美元绣花机要订阅，我干脆自己写了个 App

**原文标题**: Show HN: My $300 embroidery machine needed a subscription, so I built my own app

**原文链接**: [https://github.com/simpsoka/zigzag](https://github.com/simpsoka/zigzag)

ZigZag是一款使用Rust构建的可视化刺绣编辑器，旨在规避一台300美元刺绣机的订阅要求。它允许用户将SVG艺术作品转换为针迹，精细调整设计，并以PES、DST、EXP、JEF或VP3等常见格式导出，确保广泛的机器兼容性。一个突出的特点是它对Brother Skitch (PP1)机器的直接蓝牙连接功能。

该应用程序通过模型上下文协议 (MCP) 支持AI代理，使代理能够协作设计。用户可以直接在ZigZag中绘图，从Illustrator导入，或利用AI进行设计创作。一个命令行工具在编辑器之外也提供了类似的工作流程功能。

ZigZag支持Mac (通过DMG或Homebrew) 和Windows平台，并提供应用内更新。它支持多种针迹类型，包括榻榻米填充、缎面针、运行针、贴花、十字绣等。高级规划功能包括重叠移除、优化针迹路径以隐藏走线、自定义起始/结束点以及面料预设。

该编辑器的“工作室”界面设计成让Illustrator用户感到熟悉，提供选择、绘图 (钢笔、画笔、形状)、文本和测量工具。关键功能包括智能参考线、一个“图像描摹”功能可将栅格图像转换为纯色刺绣设计，以及一个“代理”面板，集成了Claude Code等AI模型进行设计协助，并在代理工作时在画布上提供可视化反馈。

---

## 9. 逆向工程我的Coway空气净化器，摆脱云端

**原文标题**: Reverse engineering my Coway air purifier to ditch the cloud

**原文链接**: [https://scottjg.com/posts/2026-11-11-reverse-engineering-my-coway-air-purifier-to-ditch-the-cloud/](https://scottjg.com/posts/2026-11-11-reverse-engineering-my-coway-air-purifier-to-ditch-the-cloud/)

作者详细介绍了他们逆向工程一台Coway Airmega IconS空气净化器的过程，旨在消除其对Coway不可靠云服务的依赖。由于频繁的服务中断、强制更改密码以及服务最终可能停止的风险，作者感到沮丧，因此目标是实现本地控制，并通过Home Assistant将其整合到Apple Home中。

最初，作者因SSL证书绕过和中间人（MitM）设置的感知难度而却步，但有两个因素促使他们采取行动：一是2026年涉及一个弱证书颁发机构（eMudhra）的安全事件，二是AI能够简化MitM环境配置。

作者设置了一个树莓派作为独立的Wi-Fi接入点，将净化器的流量通过`mitmproxy`进行路由。一个关键发现是，该风扇通过*明文HTTP*下载其根CA证书（AmazonRootCA1.pem）。这使得`mitmproxy`能够注入自己的CA证书，从而实现对HTTPS流量的完全拦截，而无需利用eMudhra的漏洞。

进一步的嗅探显示，设备通过一个特定的POST请求获取其MQTT服务器地址和证书URL。风扇命令，例如速度调节，通过TLS上的MQTT在8883端口进行通信。通过AI辅助拦截和分析这些MQTT消息，作者成功破译了控制协议。

这一突破提供了足够的信息来构建一个自定义的Web服务器以颁发证书，以及一个MQTT服务器以发送命令，从而完全将Coway云服务从设备的运行循环中移除。下一步是逆向工程蓝牙设置过程，以消除对Coway应用进行设备初始配置的依赖。

---

## 10. Gemini 4 Hydrogen

**原文标题**: Gemini 4 Hydrogen

**原文链接**: [https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-4-hydrogen/](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-4-hydrogen/)

生成摘要时出错

---

## 11. Gemini 4 Hydrogen and Orchestrator

**原文标题**: Gemini 4 Hydrogen and Orchestrator

**原文链接**: [https://antigravity.google/blog/gemini-4-hydrogen-in-google-antigravity/](https://antigravity.google/blog/gemini-4-hydrogen-in-google-antigravity/)

生成摘要时出错

---

## 12. Elevated errors on claude.ai, Claude Code, and platform.claude.com

**原文标题**: Elevated errors on claude.ai, Claude Code, and platform.claude.com

**原文链接**: [https://status.claude.com/incidents/nn11wk485zfn](https://status.claude.com/incidents/nn11wk485zfn)

On November 13, 2026, Claude experienced elevated errors across several of its services, including claude.ai, Claude Code, platform.claude.com (Claude Console), and Claude Cowork.

The incident began with users encountering issues authenticating to Claude.ai and Claude Code, which the team started investigating around 09:58 UTC. A fix for the affecting services was deployed by 11:05 UTC, followed by a period of monitoring for recovery. The issue was ultimately resolved by 11:58 UTC, with full resolution confirmed for claude.ai and Claude Cowork. The incident report was powered by Atlassian Statuspage.

---

## 13. I'm making LLMs work on small and old devices

**原文标题**: I'm making LLMs work on small and old devices

**原文链接**: [https://github.com/hyperionaidev/smolmaxxing/](https://github.com/hyperionaidev/smolmaxxing/)

生成摘要时出错

---

## 14. 微软Outlook/365持续宕机12小时

**原文标题**: Microsoft Outlook/365 still down after 12 hours

**原文链接**: [https://twitter.com/MSFT365Status/status/2121079061774491735](https://twitter.com/MSFT365Status/status/2121079061774491735)

生成摘要时出错

---

## 15. Former Nvidia CEO Huang had a relationship with a second employee, sources say

**原文标题**: Former Nvidia CEO Huang had a relationship with a second employee, sources say

**原文链接**: [https://www.reuters.com/technology/former-nvidia-ceo-huang-had-relationship-with-second-employee-sources-say-2026-11-12/](https://www.reuters.com/technology/former-nvidia-ceo-huang-had-relationship-with-second-employee-sources-say-2026-11-12/)

生成摘要时出错

---

## 16. Doomsday: Friday, 13 November, A.D. 2026 (1960)

**原文标题**: Doomsday: Friday, 13 November, A.D. 2026 (1960)

**原文链接**: [https://www.science.org/doi/10.1126/science.132.3436.1291](https://www.science.org/doi/10.1126/science.132.3436.1291)

生成摘要时出错

---

## 17. "Humble Bundle just killed most of their security through vibecoding"

**原文标题**: "Humble Bundle just killed most of their security through vibecoding"

**原文链接**: [https://forums.spacebattles.com/threads/humble-bundle-just-completely-killed-most-of-their-security-through-vibecoding.1346295/](https://forums.spacebattles.com/threads/humble-bundle-just-completely-killed-most-of-their-security-through-vibecoding.1346295/)

生成摘要时出错

---

## 18. Dwarf planet candidate appears which takes roughly 280 years to orbit our sun

**原文标题**: Dwarf planet candidate appears which takes roughly 280 years to orbit our sun

**原文链接**: [https://www.smithsonianmag.com/smart-news/astronomers-found-a-mysterious-object-orbiting-far-beyond-pluto-it-could-be-a-new-dwarf-planet-hidden-in-our-solar-system-180989857/](https://www.smithsonianmag.com/smart-news/astronomers-found-a-mysterious-object-orbiting-far-beyond-pluto-it-could-be-a-new-dwarf-planet-hidden-in-our-solar-system-180989857/)

生成摘要时出错

---

## 19. Jensen Huang resigns as Nvidia CEO immediately

**原文标题**: Jensen Huang resigns as Nvidia CEO immediately

**原文链接**: [https://www.reuters.com/live/nvidia-live-board-meets-fate-ceo-jensen-huang-after-affair-reports-2026-11-12/](https://www.reuters.com/live/nvidia-live-board-meets-fate-ceo-jensen-huang-after-affair-reports-2026-11-12/)

生成摘要时出错

---

## 20. Writing correct software is hard and math alone won’t help us (2016)

**原文标题**: Writing correct software is hard and math alone won’t help us (2016)

**原文链接**: [https://pron.github.io/posts/correctness-and-complexity](https://pron.github.io/posts/correctness-and-complexity)

生成摘要时出错

---

## 21. Critical RCE Vulnerability in Apache HTTP Server

**原文标题**: Critical RCE Vulnerability in Apache HTTP Server

**原文链接**: [https://www.wiz.io/blog/cve-2026-119618-rce-apache-http-server-vulnerability](https://www.wiz.io/blog/cve-2026-119618-rce-apache-http-server-vulnerability)

生成摘要时出错

---

## 22. IceWM

**原文标题**: IceWM

**原文链接**: [https://ice-wm.org/](https://ice-wm.org/)

生成摘要时出错

---

## 23. Chinese frontier AI models carry the fingerprint of export-controlled GPUs

**原文标题**: Chinese frontier AI models carry the fingerprint of export-controlled GPUs

**原文链接**: [https://unemploymentlabs.com/checkpoint-forensics](https://unemploymentlabs.com/checkpoint-forensics)

生成摘要时出错

---

## 24. Edge0-145B: Frontier AI Capabilities on Your Own Computer

**原文标题**: Edge0-145B: Frontier AI Capabilities on Your Own Computer

**原文链接**: [https://edge0.ai/blog/introducing-edge0-145b-frontier-ai-capabilities-on-your-own-computer](https://edge0.ai/blog/introducing-edge0-145b-frontier-ai-capabilities-on-your-own-computer)

生成摘要时出错

---

## 25. Nintendo Takes Down Emulators and Firmware in Massive GitHub DMCA Sweep

**原文标题**: Nintendo Takes Down Emulators and Firmware in Massive GitHub DMCA Sweep

**原文链接**: [https://www.ign.com/articles/nintendo-takes-down-switch-emulators-and-mod-chip-firmware-in-massive-github-dmca-sweep](https://www.ign.com/articles/nintendo-takes-down-switch-emulators-and-mod-chip-firmware-in-massive-github-dmca-sweep)

生成摘要时出错

---

## 26. Rust 1.100

**原文标题**: Rust 1.100

**原文链接**: [https://github.com/rust-lang/rust/releases/tag/1.100.0](https://github.com/rust-lang/rust/releases/tag/1.100.0)

生成摘要时出错

---

## 27. AI unlocks Gödel's notebooks, said to contain hundreds of proved theorems

**原文标题**: AI unlocks Gödel's notebooks, said to contain hundreds of proved theorems

**原文链接**: [https://www.theguardian.com/science/2026/nov/13/kurt-godel-notebooks-ai-helps-unlock-hidden-discoveries-man-who-transformed-maths](https://www.theguardian.com/science/2026/nov/13/kurt-godel-notebooks-ai-helps-unlock-hidden-discoveries-man-who-transformed-maths)

生成摘要时出错

---

## 28. AI is destroying the trust between writers and readers

**原文标题**: AI is destroying the trust between writers and readers

**原文链接**: [https://www.theatlantic.com/books/2026/11/ai-literary-scams-amazon/689391/](https://www.theatlantic.com/books/2026/11/ai-literary-scams-amazon/689391/)

生成摘要时出错

---

## 29. Abandoned Quake 4 expansion finished by modders and now playable

**原文标题**: Abandoned Quake 4 expansion finished by modders and now playable

**原文链接**: [https://www.moddb.com/mods/openq4/downloads/openq4-0141-windows-x64](https://www.moddb.com/mods/openq4/downloads/openq4-0141-windows-x64)

生成摘要时出错

---

## 30. Global Microsoft Outage

**原文标题**: Global Microsoft Outage

**原文链接**: [https://www.cnn.com/2026/11/12/business/live-news/microsoft-global-outage-intl-hnk](https://www.cnn.com/2026/11/12/business/live-news/microsoft-global-outage-intl-hnk)

生成摘要时出错

---

## 31. $11.4M in Nvidia hardware vanishes during shipment from CA to TX

**原文标题**: $11.4M in Nvidia hardware vanishes during shipment from CA to TX

**原文链接**: [https://www.freightwaves.com/news/11-4-million-in-nvidia-hardware-vanishes-during-shipment-from-california-to-texas](https://www.freightwaves.com/news/11-4-million-in-nvidia-hardware-vanishes-during-shipment-from-california-to-texas)

生成摘要时出错

---

## 32. Foundation Models framework

**原文标题**: Foundation Models framework

**原文链接**: [https://developer.apple.com/foundation-models-framework/](https://developer.apple.com/foundation-models-framework/)

生成摘要时出错

---

## 33. Eli Lilly CEO pushes back on Dario Amodei's medical claims

**原文标题**: Eli Lilly CEO pushes back on Dario Amodei's medical claims

**原文链接**: [https://garymarcus.substack.com/p/breaking-eli-lilly-ceo-becomes-latest](https://garymarcus.substack.com/p/breaking-eli-lilly-ceo-becomes-latest)

生成摘要时出错

---

## 34. It Takes 16 Clicks for a Student to Open a PowerPoint on an iPad

**原文标题**: It Takes 16 Clicks for a Student to Open a PowerPoint on an iPad

**原文链接**: [https://www.reddit.com/r/Teachers/comments/1xuup7a/technology_sucks_it_literally_takes_16_clicks_for/](https://www.reddit.com/r/Teachers/comments/1xuup7a/technology_sucks_it_literally_takes_16_clicks_for/)

生成摘要时出错

---

## 35. Brave Search API now accepts agentic payments via the x402 protocol

**原文标题**: Brave Search API now accepts agentic payments via the x402 protocol

**原文链接**: [https://brave.com/blog/search-api-agentic-payments/](https://brave.com/blog/search-api-agentic-payments/)

生成摘要时出错

---

## 36. Our software engineering interviews are changing a little

**原文标题**: Our software engineering interviews are changing a little

**原文链接**: [https://blog.janestreet.com/software-engineering-interviews-are-changing-a-little/](https://blog.janestreet.com/software-engineering-interviews-are-changing-a-little/)

生成摘要时出错

---

## 37. Talking Zen 6 with Mike Clark at AMD In-Depth

**原文标题**: Talking Zen 6 with Mike Clark at AMD In-Depth

**原文链接**: [https://chipsandcheese.com/p/talking-zen-6-with-mike-clark-at](https://chipsandcheese.com/p/talking-zen-6-with-mike-clark-at)

生成摘要时出错

---

## 38. Turning a 22-year-old Postgres type-confusion primitive into RCE

**原文标题**: Turning a 22-year-old Postgres type-confusion primitive into RCE

**原文链接**: [https://mehmetince.net/part-3-6-how-i-ended-up-turning-a-22-year-old-postgresql-type-confusion-primitive-into-rce-cve-2026-6460/](https://mehmetince.net/part-3-6-how-i-ended-up-turning-a-22-year-old-postgresql-type-confusion-primitive-into-rce-cve-2026-6460/)

生成摘要时出错

---

## 39. Why Zig over C for Systems Programming

**原文标题**: Why Zig over C for Systems Programming

**原文链接**: [https://www.mtsoukalos.eu/2026/11/why-zig-over-c-for-systems-programming/](https://www.mtsoukalos.eu/2026/11/why-zig-over-c-for-systems-programming/)

生成摘要时出错

---

## 40. After 600 experiments, here's what I discovered about JEPA world models

**原文标题**: After 600 experiments, here's what I discovered about JEPA world models

**原文链接**: [https://haddyalchaer.com/jepa](https://haddyalchaer.com/jepa)

生成摘要时出错

---

## 41. Big tech is here to let us down

**原文标题**: Big tech is here to let us down

**原文链接**: [https://blog.jsweeting.me/big-tech-is-here-to-let-us-down](https://blog.jsweeting.me/big-tech-is-here-to-let-us-down)

生成摘要时出错

---

## 42. Data centers need power – lower income, rural residents pay the price

**原文标题**: Data centers need power – lower income, rural residents pay the price

**原文链接**: [https://news.cornell.edu/stories/2026/11/data-centers-need-power-lower-income-rural-residents-pay-price](https://news.cornell.edu/stories/2026/11/data-centers-need-power-lower-income-rural-residents-pay-price)

生成摘要时出错

---

## 43. AI is turning Apple's app review process into a nightmare for synth developers

**原文标题**: AI is turning Apple's app review process into a nightmare for synth developers

**原文链接**: [https://synthanatomy.com/2026/11/ai-is-turning-apples-app-review-process-into-a-nightmare-for-developers.html](https://synthanatomy.com/2026/11/ai-is-turning-apples-app-review-process-into-a-nightmare-for-developers.html)

生成摘要时出错

---

## 44. Claude Is Down

**原文标题**: Claude Is Down

**原文链接**: [https://status.claude.com/history](https://status.claude.com/history)

生成摘要时出错

---

## 45. Singapore Says U.S. Not Helpful on Investigation into Suspected Spy's Company

**原文标题**: Singapore Says U.S. Not Helpful on Investigation into Suspected Spy's Company

**原文链接**: [https://www.nytimes.com/2026/11/12/business/nvidia-megaspeed-alice-huang.html](https://www.nytimes.com/2026/11/12/business/nvidia-megaspeed-alice-huang.html)

生成摘要时出错

---

## 46. No AI Slop: A Manifesto

**原文标题**: No AI Slop: A Manifesto

**原文链接**: [https://www.slopmanifesto.com/](https://www.slopmanifesto.com/)

生成摘要时出错

---

## 47. FM-1 Workbench

**原文标题**: FM-1 Workbench

**原文链接**: [https://open.m-vave.com/fm1-workbench](https://open.m-vave.com/fm1-workbench)

生成摘要时出错

---

## 48. A technical vision for the Haskell ecosystem

**原文标题**: A technical vision for the Haskell ecosystem

**原文链接**: [https://discourse.haskell.org/t/a-technical-vision-for-the-haskell-ecosystem/15078](https://discourse.haskell.org/t/a-technical-vision-for-the-haskell-ecosystem/15078)

生成摘要时出错

---

## 49. Nvidia CEO Jensen Huang resigns after reports of second affair deepened scandal

**原文标题**: Nvidia CEO Jensen Huang resigns after reports of second affair deepened scandal

**原文链接**: [https://www.bbc.co.uk/news/live/c6zjry11v8w1t](https://www.bbc.co.uk/news/live/c6zjry11v8w1t)

生成摘要时出错

---

## 50. Brazil's Caixa insurer breach exposes names and tax IDs of all 7.6M customers

**原文标题**: Brazil's Caixa insurer breach exposes names and tax IDs of all 7.6M customers

**原文链接**: [https://filemanager-cdn.mziq.com/published/3972906b-e50b-4f74-ab74-4d0d32125d11/9567a559-d20a-486e-a7ae-5c6bbc030c5e](https://filemanager-cdn.mziq.com/published/3972906b-e50b-4f74-ab74-4d0d32125d11/9567a559-d20a-486e-a7ae-5c6bbc030c5e)

生成摘要时出错

---

## 51. Why is Google cutting off Search from AI-free schools? Here are some theories

**原文标题**: Why is Google cutting off Search from AI-free schools? Here are some theories

**原文链接**: [https://text.npr.org/nx-s1-6029408](https://text.npr.org/nx-s1-6029408)

生成摘要时出错

---

## 52. 'The Netherlands is negotiating dismantling the International Criminal Court'

**原文标题**: 'The Netherlands is negotiating dismantling the International Criminal Court'

**原文链接**: [https://rightsforum.org/en/diplomatic-sources-the-netherlands-is-negotiating-the-dismantling-of-the-international-criminal-court/](https://rightsforum.org/en/diplomatic-sources-the-netherlands-is-negotiating-the-dismantling-of-the-international-criminal-court/)

生成摘要时出错

---

## 53. Libreagi – Save OSS Models

**原文标题**: Libreagi – Save OSS Models

**原文链接**: [https://libreagi.com/](https://libreagi.com/)

生成摘要时出错

---

## 54. Jonathan Blow – If AI Solved Coding, Why Is My Software Still the Same? [video]

**原文标题**: Jonathan Blow – If AI Solved Coding, Why Is My Software Still the Same? [video]

**原文链接**: [https://www.youtube.com/watch?v=IRK8h67ol7Q](https://www.youtube.com/watch?v=IRK8h67ol7Q)

生成摘要时出错

---

## 55. Switcher (2004)

**原文标题**: Switcher (2004)

**原文链接**: [https://folklore.org/Switcher.html](https://folklore.org/Switcher.html)

生成摘要时出错

---

## 56. All US airports are currently ground stopped

**原文标题**: All US airports are currently ground stopped

**原文链接**: [https://twitter.com/flightradar24/status/2121347654714077605](https://twitter.com/flightradar24/status/2121347654714077605)

生成摘要时出错

---

## 57. OpenAI disbands its robotics team as its general models start running robots

**原文标题**: OpenAI disbands its robotics team as its general models start running robots

**原文链接**: [https://fortune.com/2026/11/13/openai-disbands-robotics-team-as-its-general-models-start-running-robots/](https://fortune.com/2026/11/13/openai-disbands-robotics-team-as-its-general-models-start-running-robots/)

生成摘要时出错

---

## 58. Researchers discover rare star system that emits radio signals every 8 minutes

**原文标题**: Researchers discover rare star system that emits radio signals every 8 minutes

**原文链接**: [https://www.curtin.edu.au/news/media-release/researchers-discover-rare-star-system-that-emits-radio-signals-every-eight-minutes/](https://www.curtin.edu.au/news/media-release/researchers-discover-rare-star-system-that-emits-radio-signals-every-eight-minutes/)

生成摘要时出错

---

## 59. Show HN: Isometric SF – A pixel-art map of the SF Bay Area

**原文标题**: Show HN: Isometric SF – A pixel-art map of the SF Bay Area

**原文链接**: [https://isometricsf.com/](https://isometricsf.com/)

生成摘要时出错

---

## 60. The Dawn of the Data Intelligence Engineer

**原文标题**: The Dawn of the Data Intelligence Engineer

**原文链接**: [https://motherduck.com/blog/the-data-intelligence-engineer/](https://motherduck.com/blog/the-data-intelligence-engineer/)

生成摘要时出错

---

## 61. Africa's solar revolution is vast and speedy

**原文标题**: Africa's solar revolution is vast and speedy

**原文链接**: [https://www.economist.com/middle-east-and-africa/2026/11/12/africas-solar-revolution-is-vast-and-speedy](https://www.economist.com/middle-east-and-africa/2026/11/12/africas-solar-revolution-is-vast-and-speedy)

生成摘要时出错

---

## 62. Show HN: AgentRun – open-source, Self-improving Managed Agents

**原文标题**: Show HN: AgentRun – open-source, Self-improving Managed Agents

**原文链接**: [https://github.com/Parcha-ai/agentrun/blob/main/README.md](https://github.com/Parcha-ai/agentrun/blob/main/README.md)

生成摘要时出错

---

## 63. Live airband on all frequencies from KORS. Victoria, CA also ground stopped

**原文标题**: Live airband on all frequencies from KORS. Victoria, CA also ground stopped

**原文链接**: [https://orcasairband.com/](https://orcasairband.com/)

生成摘要时出错

---

## 64. I'm Working on a FOSS Linux Pinbal Simulation Engine

**原文标题**: I'm Working on a FOSS Linux Pinbal Simulation Engine

**原文链接**: [https://www.getlazarus.org/forums/topic/17/](https://www.getlazarus.org/forums/topic/17/)

生成摘要时出错

---

## 65. Weight Space Misfolding

**原文标题**: Weight Space Misfolding

**原文链接**: [https://www.alphaxiv.org/abs/2611.weight-space-misfolding](https://www.alphaxiv.org/abs/2611.weight-space-misfolding)

生成摘要时出错

---

## 66. ExcalidrawZ: Local Native Excalidraw on macOS/iOS

**原文标题**: ExcalidrawZ: Local Native Excalidraw on macOS/iOS

**原文链接**: [https://github.com/chocoford/ExcalidrawZ](https://github.com/chocoford/ExcalidrawZ)

生成摘要时出错

---

## 67. Lonewolf 0.3 – A standalone XMPP server written in Rust

**原文标题**: Lonewolf 0.3 – A standalone XMPP server written in Rust

**原文链接**: [https://github.com/lonewolf-im/lonewolf/releases/tag/v0.3.0](https://github.com/lonewolf-im/lonewolf/releases/tag/v0.3.0)

生成摘要时出错

---

## 68. Minnesota guitarist's "palmfrets" invention strikes a new chord

**原文标题**: Minnesota guitarist's "palmfrets" invention strikes a new chord

**原文链接**: [https://www.echopress.com/business/minnesota-guitarists-invention-strikes-a-new-chord](https://www.echopress.com/business/minnesota-guitarists-invention-strikes-a-new-chord)

生成摘要时出错

---

## 69. Microsoft outage gives customers a crash course in dependence on Redmond

**原文标题**: Microsoft outage gives customers a crash course in dependence on Redmond

**原文链接**: [https://www.theregister.com/saas/2026/11/13/microsoft-outage-gives-customers-a-crash-course-in-dependence-on-redmond/5309805](https://www.theregister.com/saas/2026/11/13/microsoft-outage-gives-customers-a-crash-course-in-dependence-on-redmond/5309805)

生成摘要时出错

---

## 70. EU Digital Identity Wallet rollout: every EU state on one board

**原文标题**: EU Digital Identity Wallet rollout: every EU state on one board

**原文链接**: [https://myid.ie/business/eu-digital-wallet-tracker/](https://myid.ie/business/eu-digital-wallet-tracker/)

生成摘要时出错

---

## 71. TSMC Hacked

**原文标题**: TSMC Hacked

**原文链接**: [https://www.sec.gov/Archives/edgar/data/1046179/000104617926000800/a20261112statementregardin.htm](https://www.sec.gov/Archives/edgar/data/1046179/000104617926000800/a20261112statementregardin.htm)

生成摘要时出错

---

## 72. Vibes Don't Maintain

**原文标题**: Vibes Don't Maintain

**原文链接**: [https://roll.bybacon.com/2026/10/14/vibes-dont-maintain.html](https://roll.bybacon.com/2026/10/14/vibes-dont-maintain.html)

生成摘要时出错

---

## 73. Running web sites makes me not want to

**原文标题**: Running web sites makes me not want to

**原文链接**: [https://lowkey.party/running-web-sites-makes-me-not-want-to](https://lowkey.party/running-web-sites-makes-me-not-want-to)

生成摘要时出错

---

## 74. PostgreSQL 18.7, 17.12, 16.16, 15.20, 14.25, and 19 RC 2 Released

**原文标题**: PostgreSQL 18.7, 17.12, 16.16, 15.20, 14.25, and 19 RC 2 Released

**原文链接**: [https://www.postgresql.org/about/news/postgresql-187-1712-1616-1520-1425-and-19-rc-2-released-3442/](https://www.postgresql.org/about/news/postgresql-187-1712-1616-1520-1425-and-19-rc-2-released-3442/)

生成摘要时出错

---

## 75. US university students tell surveillance cameras to Flock off

**原文标题**: US university students tell surveillance cameras to Flock off

**原文链接**: [https://www.theguardian.com/technology/ng-interactive/2026/nov/13/universities-drop-flock-camera-contracts](https://www.theguardian.com/technology/ng-interactive/2026/nov/13/universities-drop-flock-camera-contracts)

生成摘要时出错

---

## 76. FAA issues nationwide ground stop due to "extraordinary circumstances"

**原文标题**: FAA issues nationwide ground stop due to "extraordinary circumstances"

**原文链接**: [https://www.axios.com/2026/11/13/faa-nationwide-ground-stop](https://www.axios.com/2026/11/13/faa-nationwide-ground-stop)

生成摘要时出错

---

## 77. Found: A protein that drives ageing without unleashing inflammation

**原文标题**: Found: A protein that drives ageing without unleashing inflammation

**原文链接**: [https://www.nature.com/articles/d41586-026-03638-3](https://www.nature.com/articles/d41586-026-03638-3)

生成摘要时出错

---

## 78. Scientists claim the universe is twice as old as believed

**原文标题**: Scientists claim the universe is twice as old as believed

**原文链接**: [https://geekspin.co/scientists-claim-the-universe-is-twice-as-old-as-believed/](https://geekspin.co/scientists-claim-the-universe-is-twice-as-old-as-believed/)

生成摘要时出错

---

## 79. Why You Should Expect an AI Crash

**原文标题**: Why You Should Expect an AI Crash

**原文链接**: [https://www.economist.com/leaders/2026/11/12/why-you-should-expect-an-ai-crash](https://www.economist.com/leaders/2026/11/12/why-you-should-expect-an-ai-crash)

生成摘要时出错

---

## 80. Europe's electric car sales jump 49% as global EV sales grow

**原文标题**: Europe's electric car sales jump 49% as global EV sales grow

**原文链接**: [https://electrek.co/2026/11/11/europes-electric-car-sales-jump-49-as-global-ev-sales-grow/](https://electrek.co/2026/11/11/europes-electric-car-sales-jump-49-as-global-ev-sales-grow/)

生成摘要时出错

---

## 81. The 42-Year Journey to Bring 'Neuromancer' to the Screen

**原文标题**: The 42-Year Journey to Bring 'Neuromancer' to the Screen

**原文链接**: [https://www.wired.com/story/exclusive-apple-tv-neuromancer-creator-interviews/](https://www.wired.com/story/exclusive-apple-tv-neuromancer-creator-interviews/)

生成摘要时出错

---

## 82. Bad ideas that aren't bad anymore

**原文标题**: Bad ideas that aren't bad anymore

**原文链接**: [https://devonestes.com/bad-ideas-that-arent-bad-anymore](https://devonestes.com/bad-ideas-that-arent-bad-anymore)

生成摘要时出错

---

## 83. Fitting Four 32 GB Resizable Bars Behind a PCIe Switch on Linux

**原文标题**: Fitting Four 32 GB Resizable Bars Behind a PCIe Switch on Linux

**原文链接**: [https://doug.sh/posts/gpu-bars-behind-a-pcie-switch/](https://doug.sh/posts/gpu-bars-behind-a-pcie-switch/)

生成摘要时出错

---

## 84. North Korean hackers used fake video calls in $400M crypto hack, says FBI

**原文标题**: North Korean hackers used fake video calls in $400M crypto hack, says FBI

**原文链接**: [https://www.bbc.com/news/articles/cqdj1ellpd70o](https://www.bbc.com/news/articles/cqdj1ellpd70o)

生成摘要时出错

---

## 85. Perplexity Decider v1.3: Training, eval, and use cases

**原文标题**: Perplexity Decider v1.3: Training, eval, and use cases

**原文链接**: [https://www.perplexity.ai/hub/blog/perplexity-decider](https://www.perplexity.ai/hub/blog/perplexity-decider)

生成摘要时出错

---

## 86. Microsoft says attempts to fix global outage not going 'as expected'

**原文标题**: Microsoft says attempts to fix global outage not going 'as expected'

**原文链接**: [https://www.bbc.com/news/live/cq5y10ge3dp3t](https://www.bbc.com/news/live/cq5y10ge3dp3t)

生成摘要时出错

---

## 87. Chicago schools to Google – we'd rather lose Search than be forced to accept AI

**原文标题**: Chicago schools to Google – we'd rather lose Search than be forced to accept AI

**原文链接**: [https://www.techspot.com/news/114532-chicago-schools-tell-google-they-can-live-without.html](https://www.techspot.com/news/114532-chicago-schools-tell-google-they-can-live-without.html)

生成摘要时出错

---

## 88. Apify Security Incident

**原文标题**: Apify Security Incident

**原文链接**: [https://status.apify.com/incidents/sxd1dj5j6749](https://status.apify.com/incidents/sxd1dj5j6749)

生成摘要时出错

---

## 89. Adapting CPython for Yk

**原文标题**: Adapting CPython for Yk

**原文链接**: [https://tratt.net/laurie/blog/2026/adapting_cpython_for_yk.html](https://tratt.net/laurie/blog/2026/adapting_cpython_for_yk.html)

生成摘要时出错

---

## 90. AWS Lambda Web Functions keep billing memory ~7 minutes after the last request

**原文标题**: AWS Lambda Web Functions keep billing memory ~7 minutes after the last request

**原文链接**: [https://www.easel.sh/blog/lambda-web-functions-idle-memory](https://www.easel.sh/blog/lambda-web-functions-idle-memory)

生成摘要时出错

---

## 91. US test reactor cleared for operations

**原文标题**: US test reactor cleared for operations

**原文链接**: [https://www.world-nuclear-news.org/articles/us-test-reactor-cleared-for-operations](https://www.world-nuclear-news.org/articles/us-test-reactor-cleared-for-operations)

生成摘要时出错

---

## 92. NYC Council passes ban on 'surveillance pricing'

**原文标题**: NYC Council passes ban on 'surveillance pricing'

**原文链接**: [https://gothamist.com/news/nyc-council-passes-ban-on-surveillance-pricing-that-relies-on-personal-data](https://gothamist.com/news/nyc-council-passes-ban-on-surveillance-pricing-that-relies-on-personal-data)

生成摘要时出错

---

## 93. Mercedes-Benz to halt 'all future investments' in Germany

**原文标题**: Mercedes-Benz to halt 'all future investments' in Germany

**原文链接**: [https://www.ft.com/content/f4a1fd87-9abc-4965-963a-a5349dbfdab7](https://www.ft.com/content/f4a1fd87-9abc-4965-963a-a5349dbfdab7)

生成摘要时出错

---

## 94. Show HN: Fable52.games – Play and inspect Fable 5.2 single-file HTML games

**原文标题**: Show HN: Fable52.games – Play and inspect Fable 5.2 single-file HTML games

**原文链接**: [https://fable52.games](https://fable52.games)

生成摘要时出错

---

## 95. Electric ship batteries promise compact, cooler power

**原文标题**: Electric ship batteries promise compact, cooler power

**原文链接**: [https://spectrum.ieee.org/electric-ship-batteries](https://spectrum.ieee.org/electric-ship-batteries)

生成摘要时出错

---

## 96. Nvidia CEO Jensen Huang resigns after reports of extramarital relationships

**原文标题**: Nvidia CEO Jensen Huang resigns after reports of extramarital relationships

**原文链接**: [https://www.nbcnews.com/tech/tech-news/nvidia-ceo-jensen-huang-resigns-reports-extramarital-relationships-rcna608402](https://www.nbcnews.com/tech/tech-news/nvidia-ceo-jensen-huang-resigns-reports-extramarital-relationships-rcna608402)

生成摘要时出错

---

## 97. CERN Built the Large Hadron Collider's Next-Gen Magnets

**原文标题**: CERN Built the Large Hadron Collider's Next-Gen Magnets

**原文链接**: [https://spectrum.ieee.org/large-hadron-collider-superconducting-magnets](https://spectrum.ieee.org/large-hadron-collider-superconducting-magnets)

生成摘要时出错

---

## 98. The Downfall of Jensen Huang: Nvidia's Greed and Corruption [video]

**原文标题**: The Downfall of Jensen Huang: Nvidia's Greed and Corruption [video]

**原文链接**: [https://www.youtube.com/watch?v=YYU_geUwQoA](https://www.youtube.com/watch?v=YYU_geUwQoA)

生成摘要时出错

---

## 99. Jensen Huang Admitted He Was Facing an "Avalanche" of Excess Wafers and Memory

**原文标题**: Jensen Huang Admitted He Was Facing an "Avalanche" of Excess Wafers and Memory

**原文链接**: [https://respawnfirst.com/before-resigning-jensen-huang-admitted-he-was-facing-an-avalanche-of-excess-wafers-and-memory-new-report-sheds-more-light-on-the-gpu-ram-crisis/](https://respawnfirst.com/before-resigning-jensen-huang-admitted-he-was-facing-an-avalanche-of-excess-wafers-and-memory-new-report-sheds-more-light-on-the-gpu-ram-crisis/)

生成摘要时出错

---

## 100. Arm boss Rene Haas approached in Nvidia CEO search

**原文标题**: Arm boss Rene Haas approached in Nvidia CEO search

**原文链接**: [https://www.ft.com/content/2a64f698-46dd-4178-a3f4-4c5f4c0a0926](https://www.ft.com/content/2a64f698-46dd-4178-a3f4-4c5f4c0a0926)

生成摘要时出错

---

