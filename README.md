# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-11-14.md)

*最后自动更新时间: 2026-11-14 00:38:48*
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

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-11-14](output/hacker_news_summary_2026-11-14.md) |
| 2 | [2026-11-12](output/hacker_news_summary_2026-11-12.md) |
| 3 | [2026-11-13](output/hacker_news_summary_2026-11-13.md) |
| 4 | [2026-11-11](output/hacker_news_summary_2026-11-11.md) |
| 5 | [2026-11-05](output/hacker_news_summary_2026-11-05.md) |
| 6 | [2026-11-06](output/hacker_news_summary_2026-11-06.md) |
| 7 | [2026-11-08](output/hacker_news_summary_2026-11-08.md) |
| 8 | [2026-11-07](output/hacker_news_summary_2026-11-07.md) |
| 9 | [2026-11-10](output/hacker_news_summary_2026-11-10.md) |
| 10 | [2026-10-30](output/hacker_news_summary_2026-10-30.md) |
| 11 | [2026-10-28](output/hacker_news_summary_2026-10-28.md) |
| 12 | [2026-11-03](output/hacker_news_summary_2026-11-03.md) |
| 13 | [2026-10-31](output/hacker_news_summary_2026-10-31.md) |
| 14 | [2026-11-04](output/hacker_news_summary_2026-11-04.md) |
| 15 | [2026-11-01](output/hacker_news_summary_2026-11-01.md) |
| 16 | [2026-10-29](output/hacker_news_summary_2026-10-29.md) |
| 17 | [2026-10-25](output/hacker_news_summary_2026-10-25.md) |
| 18 | [2026-10-21](output/hacker_news_summary_2026-10-21.md) |
| 19 | [2026-10-23](output/hacker_news_summary_2026-10-23.md) |
| 20 | [2026-10-22](output/hacker_news_summary_2026-10-22.md) |
| 21 | [2026-10-24](output/hacker_news_summary_2026-10-24.md) |
| 22 | [2026-10-27](output/hacker_news_summary_2026-10-27.md) |
| 23 | [2026-10-26](output/hacker_news_summary_2026-10-26.md) |
| 24 | [2026-10-16](output/hacker_news_summary_2026-10-16.md) |
| 25 | [2026-10-20](output/hacker_news_summary_2026-10-20.md) |
| 26 | [2026-10-17](output/hacker_news_summary_2026-10-17.md) |
| 27 | [2026-10-15](output/hacker_news_summary_2026-10-15.md) |
| 28 | [2026-10-19](output/hacker_news_summary_2026-10-19.md) |
| 29 | [2026-10-18](output/hacker_news_summary_2026-10-18.md) |
| 30 | [2026-10-11](output/hacker_news_summary_2026-10-11.md) |
| 31 | [2026-10-10](output/hacker_news_summary_2026-10-10.md) |
| 32 | [2026-10-06](output/hacker_news_summary_2026-10-06.md) |
| 33 | [2026-10-14](output/hacker_news_summary_2026-10-14.md) |
| 34 | [2026-10-13](output/hacker_news_summary_2026-10-13.md) |
| 35 | [2026-10-09](output/hacker_news_summary_2026-10-09.md) |
| 36 | [2026-10-07](output/hacker_news_summary_2026-10-07.md) |
| 37 | [2026-10-02](output/hacker_news_summary_2026-10-02.md) |
| 38 | [2026-09-29](output/hacker_news_summary_2026-09-29.md) |
| 39 | [2026-10-03](output/hacker_news_summary_2026-10-03.md) |
| 40 | [2026-09-27](output/hacker_news_summary_2026-09-27.md) |
| 41 | [2026-10-01](output/hacker_news_summary_2026-10-01.md) |
| 42 | [2026-09-30](output/hacker_news_summary_2026-09-30.md) |
| 43 | [2026-10-04](output/hacker_news_summary_2026-10-04.md) |
| 44 | [2026-09-25](output/hacker_news_summary_2026-09-25.md) |
| 45 | [2026-09-24](output/hacker_news_summary_2026-09-24.md) |
| 46 | [2026-09-22](output/hacker_news_summary_2026-09-22.md) |
| 47 | [2026-09-21](output/hacker_news_summary_2026-09-21.md) |
| 48 | [2026-09-23](output/hacker_news_summary_2026-09-23.md) |
| 49 | [2026-09-20](output/hacker_news_summary_2026-09-20.md) |
| 50 | [2026-09-17](output/hacker_news_summary_2026-09-17.md) |
| 51 | [2026-09-15](output/hacker_news_summary_2026-09-15.md) |
| 52 | [2026-09-14](output/hacker_news_summary_2026-09-14.md) |
| 53 | [2026-09-19](output/hacker_news_summary_2026-09-19.md) |
| 54 | [2026-09-16](output/hacker_news_summary_2026-09-16.md) |
| 55 | [2026-09-18](output/hacker_news_summary_2026-09-18.md) |
| 56 | [2026-09-08](output/hacker_news_summary_2026-09-08.md) |
| 57 | [2026-09-12](output/hacker_news_summary_2026-09-12.md) |
| 58 | [2026-09-09](output/hacker_news_summary_2026-09-09.md) |
| 59 | [2026-09-13](output/hacker_news_summary_2026-09-13.md) |
| 60 | [2026-09-07](output/hacker_news_summary_2026-09-07.md) |
| 61 | [2026-09-10](output/hacker_news_summary_2026-09-10.md) |
| 62 | [2026-09-11](output/hacker_news_summary_2026-09-11.md) |
| 63 | [2026-09-06](output/hacker_news_summary_2026-09-06.md) |
| 64 | [2026-09-03](output/hacker_news_summary_2026-09-03.md) |
| 65 | [2026-08-31](output/hacker_news_summary_2026-08-31.md) |
| 66 | [2026-09-01](output/hacker_news_summary_2026-09-01.md) |
| 67 | [2026-08-30](output/hacker_news_summary_2026-08-30.md) |
| 68 | [2026-09-02](output/hacker_news_summary_2026-09-02.md) |
| 69 | [2026-09-04](output/hacker_news_summary_2026-09-04.md) |
| 70 | [2026-09-05](output/hacker_news_summary_2026-09-05.md) |
| 71 | [2026-08-29](output/hacker_news_summary_2026-08-29.md) |
| 72 | [2026-08-23](output/hacker_news_summary_2026-08-23.md) |
| 73 | [2026-08-26](output/hacker_news_summary_2026-08-26.md) |
| 74 | [2026-08-25](output/hacker_news_summary_2026-08-25.md) |
| 75 | [2026-08-20](output/hacker_news_summary_2026-08-20.md) |
| 76 | [2026-08-28](output/hacker_news_summary_2026-08-28.md) |
| 77 | [2026-08-19](output/hacker_news_summary_2026-08-19.md) |
| 78 | [2026-08-24](output/hacker_news_summary_2026-08-24.md) |
| 79 | [2026-08-21](output/hacker_news_summary_2026-08-21.md) |
| 80 | [2026-08-22](output/hacker_news_summary_2026-08-22.md) |
| 81 | [2026-08-12](output/hacker_news_summary_2026-08-12.md) |
| 82 | [2026-08-10](output/hacker_news_summary_2026-08-10.md) |
| 83 | [2026-08-14](output/hacker_news_summary_2026-08-14.md) |
| 84 | [2026-08-09](output/hacker_news_summary_2026-08-09.md) |
| 85 | [2026-08-18](output/hacker_news_summary_2026-08-18.md) |
| 86 | [2026-08-15](output/hacker_news_summary_2026-08-15.md) |
| 87 | [2026-08-16](output/hacker_news_summary_2026-08-16.md) |
| 88 | [2026-08-11](output/hacker_news_summary_2026-08-11.md) |
| 89 | [2026-08-17](output/hacker_news_summary_2026-08-17.md) |
| 90 | [2026-08-13](output/hacker_news_summary_2026-08-13.md) |
| 91 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 92 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 93 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 94 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 95 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 96 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 97 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 98 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 99 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 100 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 101 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 102 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 103 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 104 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 105 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 106 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 107 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 108 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 109 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 110 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 111 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 112 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 113 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 114 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 115 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 116 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 117 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 118 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 119 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 120 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 121 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 122 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 123 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 124 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 125 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 126 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 127 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 128 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 129 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 130 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 131 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 132 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 133 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 134 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 135 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 136 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 137 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 138 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 139 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 140 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 141 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 142 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 143 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 144 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 145 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 146 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 147 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 148 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 149 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 150 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 151 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 152 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 153 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 154 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 155 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 156 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 157 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 158 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 159 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 160 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 161 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 162 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 163 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 164 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 165 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 166 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 167 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 168 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 169 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 170 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 171 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 172 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 173 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 174 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 175 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 176 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 177 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 178 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 179 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 180 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 181 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 182 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 183 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 184 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 185 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 186 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 187 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 188 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 189 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 190 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 191 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 192 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 193 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 194 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 195 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 196 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 197 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 198 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 199 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 200 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 201 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 202 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 203 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 204 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 205 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 206 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 207 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 208 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 209 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 210 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 211 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 212 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 213 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 214 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 215 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 216 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 217 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 218 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 219 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 220 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 221 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 222 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 223 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 224 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 225 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 226 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 227 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 228 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 229 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 230 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 231 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 232 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 233 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 234 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 235 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 236 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 237 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 238 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 239 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 240 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 241 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 242 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 243 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 244 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 245 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 246 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 247 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 248 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 249 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 250 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 251 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 252 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 253 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 254 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 255 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 256 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 257 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 258 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 259 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 260 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 261 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 262 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 263 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 264 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 265 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 266 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 267 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 268 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 269 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 270 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 271 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 272 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 273 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 274 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 275 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 276 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 277 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 278 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 279 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 280 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 281 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 282 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 283 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 284 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 285 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 286 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 287 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 288 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 289 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 290 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 291 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 292 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 293 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 294 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 295 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 296 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 297 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 298 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 299 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 300 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 301 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 302 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 303 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 304 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 305 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 306 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 307 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 308 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 309 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 310 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 311 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 312 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 313 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 314 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 315 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 316 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 317 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 318 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 319 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 320 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 321 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 322 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 323 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 324 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 325 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 326 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 327 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 328 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 329 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 330 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 331 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 332 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 333 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 334 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 335 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 336 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 337 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 338 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 339 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 340 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 341 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 342 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 343 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 344 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 345 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 346 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 347 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 348 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 349 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 350 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 351 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 352 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 353 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 354 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 355 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 356 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 357 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 358 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 359 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 360 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 361 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 362 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 363 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
