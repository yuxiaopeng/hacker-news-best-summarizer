# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2025-12-24.md)

*最后自动更新时间: 2025-12-24 19:46:38*
## 1. CECOT内幕 — 60分钟

**原文标题**: Inside CECOT – 60 Minutes [video]

**原文链接**: [https://archive.org/details/insidececot](https://archive.org/details/insidececot)

这个互联网档案馆条目收录了一个名为“深入CECOT | 60分钟”的视频，这是莎伦·阿尔丰西 (Sharyn Alfonsi) 为哥伦比亚广播公司新闻 (CBS News) 的《60分钟》节目制作的一份报道。一个显著的细节是，该片段被声称“遭到巴里·韦斯 (Bari Weiss) 审查”，并出现在加拿大环球电视 (Global TV) 应用程序上。

该视频项目，标识为“insidececot”，由科林·哈斯金斯 (Colin Haskins) 于2025年12月23日上传，其发布日期列为2025年12月22日。它的大小为1.4G，并被归类到“60分钟”主题下。该页面提供了分享、嵌入和标记内容的选项，以举报如血腥暴力或虚假信息等问题。用户还可以下载该视频，采用多种格式，包括H.264 IA、MPEG4和TORRENT。截至列表显示，它已累计128次观看、4个收藏和4条评论。

---

## 2. 法布里斯·贝拉尔发布MicroQuickJS

**原文标题**: Fabrice Bellard Releases MicroQuickJS

**原文链接**: [https://github.com/bellard/mquickjs/blob/main/README.md](https://github.com/bellard/mquickjs/blob/main/README.md)

备受尊敬的开发者法布里斯·贝拉德已正式发布MicroQuickJS (mquickjs)。这个新项目似乎托管在一个公共代码仓库上，从“bellard/mquickjs”的命名方式便可看出。

此次发布迅速获得了开发者社区的广泛关注和积极反响。这体现在其令人印象深刻的参与度指标上：该项目已累计 69 个分支和多达 2,600 个星标。这些数字凸显了人们对贝拉德最新作品的强烈兴趣，表明MicroQuickJS被视为对开源领域一项有价值且有影响力的贡献。

---

## 3. Some Epstein file redactions are being undone with hacks

**原文标题**: Some Epstein file redactions are being undone with hacks

**原文链接**: [https://www.theguardian.com/us-news/2025/dec/23/epstein-unredacted-files-social-media](https://www.theguardian.com/us-news/2025/dec/23/epstein-unredacted-files-social-media)

生成摘要时出错

---

## 4. Meta 在其服务器上使用专为 Valve Steam Deck 设计的 Linux 调度器。

**原文标题**: Meta is using the Linux scheduler designed for Valve's Steam Deck on its servers

**原文链接**: [https://www.phoronix.com/news/Meta-SCX-LAVD-Steam-Deck-Server](https://www.phoronix.com/news/Meta-SCX-LAVD-Steam-Deck-Server)

Meta（脸书）已在其大型服务器上采纳了最初为Valve的Steam Deck设计的Linux调度器SCX-LAVD（低延迟感知虚拟截止时间调度器）。由Linux咨询公司Igalia为Valve开发的SCX-LAVD，被证明对Steam Deck非常有效，匹敌甚至超越了EEVDF的性能，并已被各种Linux游戏项目所利用。

2025年Linux Plumbers大会上一个有趣的发现揭示，Meta发现这款调度器尽管起源于手持设备，却能出色地适应超大规模服务器环境。Meta工程师展示了他们关于“我们如何让Steam Deck调度器在大型服务器上工作”的研究成果，探索将SCX-LAVD作为潜在的“默认”集群调度器。

他们将SCX-LAVD称为“Meta的新默认调度器”（构建于sched_ext之上），发现它在广泛的CPU和内存配置下表现出色，提供高效的负载均衡。这使得SCX-LAVD适用于不需要专门调度器的通用服务器工作负载。

---

## 5. X-ray：一个用于查找 PDF 文档中无效遮盖的 Python 库

**原文标题**: X-ray: a Python library for finding bad redactions in PDF documents

**原文链接**: [https://github.com/freelawproject/x-ray](https://github.com/freelawproject/x-ray)

X-ray 是由 Free Law Project 开发的一个 Python 库，用于检测 PDF 文档中的“不良”密文处理。当敏感文本仅仅被黑色矩形或高亮遮盖，而非被彻底移除时，就会出现这个问题，导致底层文本仍然可选且可读。

该库有助于评估此类无效密文处理的普遍性。用户可以通过本地文件路径、URL 或内存中的字节数据提供 PDF。X-ray 既提供命令行工具（例如 `xray path/to/file.pdf` 或 `uvx --from x-ray xray URL`），也提供 Python API（`xray.inspect()`）。

输出以 JSON 格式（或 Python 对象）提供，结构为一个字典。键代表页码，映射到一个字典列表。每个字典描述一个不良密文处理，包括其 `bbox`（边界框坐标）以及密文下方发现的 `text`（文本）。

在内部，X-ray 利用 PyMuPDF 库工作。它通过识别同一位置的黑色矩形和相应文本来运行。然后，它将可疑的密文区域渲染为图像并检查其是否为纯色，这表明密文应用不当。该项目正在持续开发中，以识别更多种形式的不良密文处理，并欢迎社区贡献。它在宽松的 BSD 许可证下分发。

---

## 6. 美国叫停所有海上风电建设，称原因是机密

**原文标题**: US blocks all offshore wind construction, says reason is classified

**原文链接**: [https://arstechnica.com/science/2025/12/us-government-finds-new-excuse-to-stop-construction-of-offshore-wind/](https://arstechnica.com/science/2025/12/us-government-finds-new-excuse-to-stop-construction-of-offshore-wind/)

美国内政部突然叫停了所有五个在建海上风电项目的施工，理由是国防部一份机密报告披露了未指明的“国家安全风险”。此举引发争议，因为这些项目早已进展顺利，有些甚至接近完工，并且此前已通过广泛审批，国防部在此前审批中也未曾提出此类担忧。

这一决定反映了特朗普政府对海上风电的持续敌意。此前阻挠项目的尝试，包括一项行政命令以及对“帝国风电”（Empire Wind）和“革命风电”（Revolution Wind）等特定项目的搁置，往往因缺乏实质性理由（除了对风力发电普遍存在的不满外）而被法院推翻。例如，“革命风电”项目在赢得了针对内政部早期阻挠的诉讼后恢复施工时，已完成了80%。

目前暂停的五个项目包括弗吉尼亚海岸海上风电（2.6吉瓦）、帝国风电（810兆瓦）、革命风电（700兆瓦）、日出风电（925兆瓦）以及原计划于今年完工的葡萄园风电1号（800兆瓦）等主要设施。

国防部报告的机密性质使得法律挑战变得异常困难。然而，受影响的州（如康涅狄格州）以及投入巨资的项目开发商，预计将反对这项“非法且反复无常”的命令，该命令似乎旨在规避此前的法院裁决。文章指出，这一机密理由可能只是又一次缺乏实质性依据地叫停项目的尝试，意在借用机密性质以规避审查。

---

## 7. 我们用JPEG截图取代了H.264视频流，效果更好。

**原文标题**: We replaced H.264 streaming with JPEG screenshots (and it worked better)

**原文链接**: [https://blog.helix.ml/p/we-mass-deployed-15-year-old-screen](https://blog.helix.ml/p/we-mass-deployed-15-year-old-screen)

HelixML是一家开发需要自主代理进行屏幕共享的人工智能平台的公司。他们努力在各种网络条件下，尤其是在受限的企业网络和糟糕的WiFi环境下，实现可靠的视频流传输。

他们最初尝试使用WebRTC，但因企业防火墙阻断UDP和对TURN服务器的要求而失败。随后，他们设计了一个复杂的、硬件加速的H.264流传输管道，通过WebSockets传输，并利用HTTPS/443端口绕过防火墙。

尽管技术上很精巧，这个40Mbps的H.264传输管道在不稳定的连接下仍告失败。TCP缓冲导致严重的延迟，视频落后实时30多秒，使其无法使用。只发送H.264关键帧的尝试也因底层协议限制而存在问题。

沮丧之余，团队偶然发现了一个简单的调试端点，可以提供即时JPEG截图。这一发现促使他们用通过HTTP请求轮询JPEG图像的方式，取代了复杂的视频传输管道。JPEG证明了其优越性：它们是独立的（无需解码器状态，不会损坏），比H.264关键帧更小（100-150KB 对比 200-500KB），并且在糟糕的网络上更可靠，传输的帧数虽少，但每一帧都是完美的。

最终的架构是混合式的：在良好连接（RTT < 150ms）下，使用H.264流传输实现60fps；在不良连接下，动态切换到2-10fps的JPEG轮询。输入（键盘/鼠标）始终通过WebSockets传输，通过一个控制消息来切换视频。一个机制防止了模式的频繁切换。这一经历强调，在现实环境中，简单、优雅降级的解决方案往往优于复杂、高性能的方案。

---

## 8. 图解Transformer

**原文标题**: The Illustrated Transformer

**原文链接**: [https://jalammar.github.io/illustrated-transformer/](https://jalammar.github.io/illustrated-transformer/)

《图解Transformer》解释了Transformer，这是一种在论文《Attention Is All You Need》中提出的神经网络架构，旨在提升神经机器翻译等模型的训练速度，尤其受益于并行化。

宏观来看，Transformer由一个编码器组件和一个解码器组件组成，每个都堆叠了多个相同的编码器和解码器。编码器处理输入序列，而解码器生成输出序列。每个编码器包含两个子层：一个自注意力层和一个前馈神经网络。

自注意力机制对于理解句子内部上下文至关重要，它使得模型在编码特定词时，能够权衡其他词的重要性（例如，将“it”解析为“animal”）。其工作原理是为每个词嵌入创建三个向量：查询 (Q)、键 (K) 和值 (V)。通过查询向量与所有键向量的点积计算得分，经softmax归一化后，再与值向量相乘并求和，以生成该词的上下文相关输出。这个过程通过矩阵乘法高效实现。

模型通过“多头注意力”机制对此进行改进，采用多组Q/K/V矩阵。每个“头”学习关注输入中不同方面或位置，提供多样化的表示子空间。这些多头的输出随后被拼接并进行线性变换。

最后，为了考虑词语的顺序（这种顺序在自注意力机制的并行处理中丢失了），Transformer将“位置编码”向量添加到输入嵌入中。这些向量遵循特定的、可学习的模式，传达序列中每个词的位置信息。

---

## 9. It's Always TCP_NODELAY

**原文标题**: It's Always TCP_NODELAY

**原文链接**: [https://brooker.co.za/blog/2024/05/09/nagle.html](https://brooker.co.za/blog/2024/05/09/nagle.html)

生成摘要时出错

---

## 10. GLM-4.7: Advancing the Coding Capability

**原文标题**: GLM-4.7: Advancing the Coding Capability

**原文链接**: [https://z.ai/blog/glm-4.7](https://z.ai/blog/glm-4.7)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 2 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 3 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 4 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 5 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 6 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 7 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 8 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 9 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 10 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 11 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 12 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 13 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 14 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 15 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 16 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 17 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 18 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 19 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 20 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 21 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 22 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 23 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 24 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 25 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 26 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 27 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 28 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 29 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 30 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 31 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 32 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 33 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 34 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 35 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 36 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 37 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 38 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 39 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 40 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 41 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 42 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 43 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 44 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 45 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 46 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 47 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 48 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 49 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
