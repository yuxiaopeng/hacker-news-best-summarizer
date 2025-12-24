# Hacker News 热门文章摘要 (2025-12-24)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

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

## 11. Instant database clones with PostgreSQL 18

**原文标题**: Instant database clones with PostgreSQL 18

**原文链接**: [https://boringsql.com/posts/instant-database-clones/](https://boringsql.com/posts/instant-database-clones/)

生成摘要时出错

---

## 12. Unifi Travel Router

**原文标题**: Unifi Travel Router

**原文链接**: [https://blog.ui.com/article/travel-in-style-unifi-style-unifi-travel-router](https://blog.ui.com/article/travel-in-style-unifi-style-unifi-travel-router)

生成摘要时出错

---

## 13. Ultrasound Cancer Treatment: Sound Waves Fight Tumors

**原文标题**: Ultrasound Cancer Treatment: Sound Waves Fight Tumors

**原文链接**: [https://spectrum.ieee.org/ultrasound-cancer-treatment](https://spectrum.ieee.org/ultrasound-cancer-treatment)

生成摘要时出错

---

## 14. Show HN: CineCLI – Browse and torrent movies directly from your terminal

**原文标题**: Show HN: CineCLI – Browse and torrent movies directly from your terminal

**原文链接**: [https://github.com/eyeblech/cinecli](https://github.com/eyeblech/cinecli)

生成摘要时出错

---

## 15. Snitch – A friendlier ss/netstat

**原文标题**: Snitch – A friendlier ss/netstat

**原文链接**: [https://github.com/karol-broda/snitch](https://github.com/karol-broda/snitch)

生成摘要时出错

---

## 16. Lotusbail npm package found to be harvesting WhatsApp messages and contacts

**原文标题**: Lotusbail npm package found to be harvesting WhatsApp messages and contacts

**原文链接**: [https://www.koi.ai/blog/npm-package-with-56k-downloads-malware-stealing-whatsapp-messages](https://www.koi.ai/blog/npm-package-with-56k-downloads-malware-stealing-whatsapp-messages)

生成摘要时出错

---

## 17. 10 years bootstrapped: €6.5M revenue with a team of 13

**原文标题**: 10 years bootstrapped: €6.5M revenue with a team of 13

**原文链接**: [https://www.datocms.com/blog/a-look-back-at-2025](https://www.datocms.com/blog/a-look-back-at-2025)

生成摘要时出错

---

## 18. iOS 26.3 brings AirPods-like pairing to third-party devices in EU under DMA

**原文标题**: iOS 26.3 brings AirPods-like pairing to third-party devices in EU under DMA

**原文链接**: [https://www.macrumors.com/2025/12/22/ios-26-3-dma-airpods-pairing/](https://www.macrumors.com/2025/12/22/ios-26-3-dma-airpods-pairing/)

生成摘要时出错

---

## 19. Texas app store age verification law blocked by federal judge

**原文标题**: Texas app store age verification law blocked by federal judge

**原文链接**: [https://www.macrumors.com/2025/12/23/texas-app-store-law-blocked/](https://www.macrumors.com/2025/12/23/texas-app-store-law-blocked/)

生成摘要时出错

---

## 20. The Garbage Collection Handbook

**原文标题**: The Garbage Collection Handbook

**原文链接**: [https://gchandbook.org/index.html](https://gchandbook.org/index.html)

生成摘要时出错

---

## 21. How did DOGE disrupt so much while saving so little?

**原文标题**: How did DOGE disrupt so much while saving so little?

**原文链接**: [https://www.nytimes.com/2025/12/23/us/politics/doge-musk-trump-analysis.html](https://www.nytimes.com/2025/12/23/us/politics/doge-musk-trump-analysis.html)

生成摘要时出错

---

## 22. Ryanair fined €256M over ‘abusive strategy’ to limit ticket sales by OTAs

**原文标题**: Ryanair fined €256M over ‘abusive strategy’ to limit ticket sales by OTAs

**原文链接**: [https://www.theguardian.com/business/2025/dec/23/ryanair-fined-limit-online-travel-agencies-ticket-sales-ota](https://www.theguardian.com/business/2025/dec/23/ryanair-fined-limit-online-travel-agencies-ticket-sales-ota)

生成摘要时出错

---

## 23. Archivists posted the 60 minutes CECOT segment Bari Weiss killed

**原文标题**: Archivists posted the 60 minutes CECOT segment Bari Weiss killed

**原文链接**: [https://www.404media.co/archivists-posted-the-60-minutes-cecot-segment-bari-weiss-killed/](https://www.404media.co/archivists-posted-the-60-minutes-cecot-segment-bari-weiss-killed/)

生成摘要时出错

---

## 24. Local AI is driving the biggest change in laptops in decades

**原文标题**: Local AI is driving the biggest change in laptops in decades

**原文链接**: [https://spectrum.ieee.org/ai-models-locally](https://spectrum.ieee.org/ai-models-locally)

生成摘要时出错

---

## 25. I didn't realize my LG TV was spying on me until I turned off Live Plus

**原文标题**: I didn't realize my LG TV was spying on me until I turned off Live Plus

**原文链接**: [https://www.pocket-lint.com/lg-tv-turn-off-live-plus/](https://www.pocket-lint.com/lg-tv-turn-off-live-plus/)

生成摘要时出错

---

## 26. Pulled 60 Minutes segment on CECOT

**原文标题**: Pulled 60 Minutes segment on CECOT

**原文链接**: [https://archive.org/details/60minutes-cecotsegment](https://archive.org/details/60minutes-cecotsegment)

生成摘要时出错

---

## 27. Nabokov's guide to foreigners learning Russian

**原文标题**: Nabokov's guide to foreigners learning Russian

**原文链接**: [https://twitter.com/haravayin_hogh/status/2003299405907247502](https://twitter.com/haravayin_hogh/status/2003299405907247502)

生成摘要时出错

---

## 28. Don't Become the Machine

**原文标题**: Don't Become the Machine

**原文链接**: [https://armeet.bearblog.dev/becoming-the-machine/](https://armeet.bearblog.dev/becoming-the-machine/)

生成摘要时出错

---

## 29. Test, don't just verify

**原文标题**: Test, don't just verify

**原文链接**: [https://alperenkeles.com/posts/test-dont-verify/](https://alperenkeles.com/posts/test-dont-verify/)

生成摘要时出错

---

## 30. US destroying its reputation as a scientific leader – European science diplomat

**原文标题**: US destroying its reputation as a scientific leader – European science diplomat

**原文链接**: [https://sciencebusiness.net/news/horizon-europe/us-demolishing-its-scientific-leadership-wrecking-ball-says-chief-eu-research](https://sciencebusiness.net/news/horizon-europe/us-demolishing-its-scientific-leadership-wrecking-ball-says-chief-eu-research)

生成摘要时出错

---

## 31. Things I learnt about passkeys when building passkeybot

**原文标题**: Things I learnt about passkeys when building passkeybot

**原文链接**: [https://enzom.dev/b/passkeys/](https://enzom.dev/b/passkeys/)

生成摘要时出错

---

## 32. HTTP Caching, a Refresher

**原文标题**: HTTP Caching, a Refresher

**原文链接**: [https://danburzo.ro/http-caching-refresher/](https://danburzo.ro/http-caching-refresher/)

生成摘要时出错

---

## 33. The 60 Minutes report that Bari Weiss censored is now internet contraband

**原文标题**: The 60 Minutes report that Bari Weiss censored is now internet contraband

**原文链接**: [https://www.theverge.com/policy/849432/60-minutes-cecot-censored-canada-leak](https://www.theverge.com/policy/849432/60-minutes-cecot-censored-canada-leak)

生成摘要时出错

---

## 34. Postponed '60 Minutes' segment on Salvadoran prison is streamed by Canadian news

**原文标题**: Postponed '60 Minutes' segment on Salvadoran prison is streamed by Canadian news

**原文链接**: [https://www.nbcnews.com/news/us-news/cbs-news-el-salvador-cecot-prison-sharyn-alfonsi-bari-weiss-rcna250618](https://www.nbcnews.com/news/us-news/cbs-news-el-salvador-cecot-prison-sharyn-alfonsi-bari-weiss-rcna250618)

生成摘要时出错

---

## 35. Satellites reveal heat leaking from largest US cryptocurrency mining center

**原文标题**: Satellites reveal heat leaking from largest US cryptocurrency mining center

**原文链接**: [https://www.space.com/space-exploration/satellites/satellites-reveal-heat-leaking-from-largest-us-cryptocurrency-mining-center](https://www.space.com/space-exploration/satellites/satellites-reveal-heat-leaking-from-largest-us-cryptocurrency-mining-center)

生成摘要时出错

---

## 36. Why We Abandoned Matrix (2024)

**原文标题**: Why We Abandoned Matrix (2024)

**原文链接**: [https://forum.hackliberty.org/t/why-we-abandoned-matrix-the-dark-truth-about-user-security-and-safety/224](https://forum.hackliberty.org/t/why-we-abandoned-matrix-the-dark-truth-about-user-security-and-safety/224)

生成摘要时出错

---

## 37. Font with Built-In Syntax Highlighting (2024)

**原文标题**: Font with Built-In Syntax Highlighting (2024)

**原文链接**: [https://blog.glyphdrawing.club/font-with-built-in-syntax-highlighting/](https://blog.glyphdrawing.club/font-with-built-in-syntax-highlighting/)

生成摘要时出错

---

## 38. Google 2025 recap: Research breakthroughs of the year

**原文标题**: Google 2025 recap: Research breakthroughs of the year

**原文链接**: [https://blog.google/technology/ai/2025-research-breakthroughs/](https://blog.google/technology/ai/2025-research-breakthroughs/)

生成摘要时出错

---

## 39. Vince Zampella, developer of Call of Duty and Battlefield has died

**原文标题**: Vince Zampella, developer of Call of Duty and Battlefield has died

**原文链接**: [https://comicbook.com/gaming/news/vince-zampella-developer-of-call-of-duty-and-battlefield-dead-at-55/](https://comicbook.com/gaming/news/vince-zampella-developer-of-call-of-duty-and-battlefield-dead-at-55/)

生成摘要时出错

---

## 40. Stop Slopware

**原文标题**: Stop Slopware

**原文链接**: [https://stopslopware.net/](https://stopslopware.net/)

生成摘要时出错

---

## 41. When Compilers Surprise You

**原文标题**: When Compilers Surprise You

**原文链接**: [https://xania.org/202512/24-cunning-clang](https://xania.org/202512/24-cunning-clang)

生成摘要时出错

---

## 42. Show HN: Turn raw HTML into production-ready images for free

**原文标题**: Show HN: Turn raw HTML into production-ready images for free

**原文链接**: [https://html2png.dev](https://html2png.dev)

生成摘要时出错

---

## 43. State regulators vote to keep utility profits high angering customers across CA

**原文标题**: State regulators vote to keep utility profits high angering customers across CA

**原文链接**: [https://www.latimes.com/environment/story/2025-12-18/state-regulators-vote-to-keep-utility-profits-high-angering-customers](https://www.latimes.com/environment/story/2025-12-18/state-regulators-vote-to-keep-utility-profits-high-angering-customers)

生成摘要时出错

---

## 44. Universal Reasoning Model (53.8% pass 1 ARC1 and 16.0% ARC 2)

**原文标题**: Universal Reasoning Model (53.8% pass 1 ARC1 and 16.0% ARC 2)

**原文链接**: [https://arxiv.org/abs/2512.14693](https://arxiv.org/abs/2512.14693)

生成摘要时出错

---

## 45. Autonomously navigating the real world: lessons from the PG&E outage

**原文标题**: Autonomously navigating the real world: lessons from the PG&E outage

**原文链接**: [https://waymo.com/blog/2025/12/autonomously-navigating-the-real-world](https://waymo.com/blog/2025/12/autonomously-navigating-the-real-world)

生成摘要时出错

---

## 46. Volvo Centum is Dalton Maag's new typeface for Volvo

**原文标题**: Volvo Centum is Dalton Maag's new typeface for Volvo

**原文链接**: [https://www.wallpaper.com/design-interiors/corporate-design-branding/volvo-new-font-volvo-centum](https://www.wallpaper.com/design-interiors/corporate-design-branding/volvo-new-font-volvo-centum)

生成摘要时出错

---

## 47. Help My c64 caught on fire

**原文标题**: Help My c64 caught on fire

**原文链接**: [https://c0de517e.com/026_c64fire.htm](https://c0de517e.com/026_c64fire.htm)

生成摘要时出错

---

## 48. AMD entered the CPU market with reverse-engineered Intel 8080 clone 50 years ago

**原文标题**: AMD entered the CPU market with reverse-engineered Intel 8080 clone 50 years ago

**原文链接**: [https://www.tomshardware.com/pc-components/cpus/amd-first-entered-the-cpu-market-with-reverse-engineered-intel-8080-clone-50-years-ago-the-am9080-cost-50-cents-apiece-to-make-but-sold-for-usd700](https://www.tomshardware.com/pc-components/cpus/amd-first-entered-the-cpu-market-with-reverse-engineered-intel-8080-clone-50-years-ago-the-am9080-cost-50-cents-apiece-to-make-but-sold-for-usd700)

生成摘要时出错

---

## 49. We just unredacted some of the Epstein files

**原文标题**: We just unredacted some of the Epstein files

**原文链接**: [https://krassencast.com/p/breaking-we-just-unredacted-the-epstein](https://krassencast.com/p/breaking-we-just-unredacted-the-epstein)

生成摘要时出错

---

## 50. US sanctions EU government officials behind the DSA

**原文标题**: US sanctions EU government officials behind the DSA

**原文链接**: [https://mastodon.social/@fj/115773761468906515](https://mastodon.social/@fj/115773761468906515)

生成摘要时出错

---

## 51. Carnap – A formal logic framework for Haskell

**原文标题**: Carnap – A formal logic framework for Haskell

**原文链接**: [https://carnap.io/](https://carnap.io/)

生成摘要时出错

---

## 52. I know you didn't write this

**原文标题**: I know you didn't write this

**原文链接**: [https://ammil.industries/i-know-you-didnt-write-this/](https://ammil.industries/i-know-you-didnt-write-this/)

生成摘要时出错

---

## 53. FCC Updates Covered List to Include Foreign UAS and UAS Critical Components [pdf]

**原文标题**: FCC Updates Covered List to Include Foreign UAS and UAS Critical Components [pdf]

**原文链接**: [https://docs.fcc.gov/public/attachments/DOC-416839A1.pdf](https://docs.fcc.gov/public/attachments/DOC-416839A1.pdf)

生成摘要时出错

---

## 54. US bars approvals of new models of DJI, all other foreign drones

**原文标题**: US bars approvals of new models of DJI, all other foreign drones

**原文链接**: [https://www.reuters.com/business/aerospace-defense/us-adds-dji-other-foreign-drones-national-security-list-2025-12-22/](https://www.reuters.com/business/aerospace-defense/us-adds-dji-other-foreign-drones-national-security-list-2025-12-22/)

生成摘要时出错

---

## 55. The e-scooter isn't new – London was zooming around on Autopeds a century ago

**原文标题**: The e-scooter isn't new – London was zooming around on Autopeds a century ago

**原文链接**: [https://www.ianvisits.co.uk/articles/the-e-scooter-isnt-new-london-was-zooming-around-on-autopeds-a-century-ago-86263/](https://www.ianvisits.co.uk/articles/the-e-scooter-isnt-new-london-was-zooming-around-on-autopeds-a-century-ago-86263/)

生成摘要时出错

---

## 56. Is Northern Virginia still the least reliable AWS region?

**原文标题**: Is Northern Virginia still the least reliable AWS region?

**原文链接**: [https://statusgator.com/blog/aws-least-reliable-region-in-2025/](https://statusgator.com/blog/aws-least-reliable-region-in-2025/)

生成摘要时出错

---

## 57. There Is No Future for Online Safety Without Privacy and Security

**原文标题**: There Is No Future for Online Safety Without Privacy and Security

**原文链接**: [https://itsfoss.com/news/alexander-linton-interview/](https://itsfoss.com/news/alexander-linton-interview/)

生成摘要时出错

---

## 58. Terrence Malick's Disciples

**原文标题**: Terrence Malick's Disciples

**原文链接**: [https://yalereview.org/article/bilge-ebiri-terrence-malick](https://yalereview.org/article/bilge-ebiri-terrence-malick)

生成摘要时出错

---

## 59. Super Mario Bros. and Yoshi Games (Yields) Reduced Burnout Risk

**原文标题**: Super Mario Bros. and Yoshi Games (Yields) Reduced Burnout Risk

**原文链接**: [https://games.jmir.org/2025/1/e84219/](https://games.jmir.org/2025/1/e84219/)

生成摘要时出错

---

## 60. The Ultimate Windows Utility (2022)

**原文标题**: The Ultimate Windows Utility (2022)

**原文链接**: [https://christitus.com/windows-tool/](https://christitus.com/windows-tool/)

生成摘要时出错

---

## 61. Help my website is too small

**原文标题**: Help my website is too small

**原文链接**: [https://lukeplant.me.uk/blog/posts/help-my-website-is-too-small/](https://lukeplant.me.uk/blog/posts/help-my-website-is-too-small/)

生成摘要时出错

---

## 62. Towards a secure peer-to-peer app platform for Clan

**原文标题**: Towards a secure peer-to-peer app platform for Clan

**原文链接**: [https://clan.lol/blog/towards-app-platform-vmtech/](https://clan.lol/blog/towards-app-platform-vmtech/)

生成摘要时出错

---

## 63. An initial analysis of the discovered Unix V4 tape

**原文标题**: An initial analysis of the discovered Unix V4 tape

**原文链接**: [https://www.spinellis.gr/blog/20251223/?yc261223](https://www.spinellis.gr/blog/20251223/?yc261223)

生成摘要时出错

---

## 64. US bars 5 Europeans it says pressured tech firms to censor American viewpoints

**原文标题**: US bars 5 Europeans it says pressured tech firms to censor American viewpoints

**原文链接**: [https://apnews.com/article/state-department-trump-immigration-rubio-visas-87c8a4692f3184e4f83fdd8ed5093886](https://apnews.com/article/state-department-trump-immigration-rubio-visas-87c8a4692f3184e4f83fdd8ed5093886)

生成摘要时出错

---

## 65. Open source USB to GPIB converter (for Test and Measurement instruments)

**原文标题**: Open source USB to GPIB converter (for Test and Measurement instruments)

**原文链接**: [https://github.com/xyphro/UsbGpib](https://github.com/xyphro/UsbGpib)

生成摘要时出错

---

## 66. When irate product support customers demand to speak to Bill Gates

**原文标题**: When irate product support customers demand to speak to Bill Gates

**原文链接**: [https://devblogs.microsoft.com/oldnewthing/20251223-00/?p=111896](https://devblogs.microsoft.com/oldnewthing/20251223-00/?p=111896)

生成摘要时出错

---

## 67. Avoid Mini-Frameworks

**原文标题**: Avoid Mini-Frameworks

**原文链接**: [https://laike9m.com/blog/avoid-mini-frameworks,171/](https://laike9m.com/blog/avoid-mini-frameworks,171/)

生成摘要时出错

---

## 68. Microsoft to replace all C/C++ code with Rust

**原文标题**: Microsoft to replace all C/C++ code with Rust

**原文链接**: [https://www.thurrott.com/dev/330980/microsoft-to-replace-all-c-c-code-with-rust-by-2030](https://www.thurrott.com/dev/330980/microsoft-to-replace-all-c-c-code-with-rust-by-2030)

生成摘要时出错

---

## 69. Permission Systems for Enterprise That Scale

**原文标题**: Permission Systems for Enterprise That Scale

**原文链接**: [https://eliocapella.com/blog/permission-systems-for-enterprise/](https://eliocapella.com/blog/permission-systems-for-enterprise/)

生成摘要时出错

---

## 70. 'Dracula's Chivito': Hubble reveals largest birthplace of planets ever observed

**原文标题**: 'Dracula's Chivito': Hubble reveals largest birthplace of planets ever observed

**原文链接**: [https://phys.org/news/2025-12-chaotic-dracula-chivito-hubble-reveals.html](https://phys.org/news/2025-12-chaotic-dracula-chivito-hubble-reveals.html)

生成摘要时出错

---

## 71. Could lockfiles just be SBOMs?

**原文标题**: Could lockfiles just be SBOMs?

**原文链接**: [https://nesbitt.io/2025/12/23/could-lockfiles-just-be-sboms.html](https://nesbitt.io/2025/12/23/could-lockfiles-just-be-sboms.html)

生成摘要时出错

---

## 72. The Duodecimal Bulletin, Vol. 55, No. 1, Year 1209 [pdf]

**原文标题**: The Duodecimal Bulletin, Vol. 55, No. 1, Year 1209 [pdf]

**原文链接**: [https://dozenal.org/drupal/sites_bck/default/files/DuodecimalBulletinIssue551.pdf](https://dozenal.org/drupal/sites_bck/default/files/DuodecimalBulletinIssue551.pdf)

生成摘要时出错

---

## 73. Donald E. Knuth and Peter van Emde Boas on priority deques (1977) [pdf]

**原文标题**: Donald E. Knuth and Peter van Emde Boas on priority deques (1977) [pdf]

**原文链接**: [https://staff.fnwi.uva.nl/p.vanemdeboas/knuthnote.pdf](https://staff.fnwi.uva.nl/p.vanemdeboas/knuthnote.pdf)

生成摘要时出错

---

## 74. Former EU commissioner and activists barred from US

**原文标题**: Former EU commissioner and activists barred from US

**原文链接**: [https://www.theguardian.com/technology/2025/dec/24/us-state-department-visa-ban-former-eu-commissioner-europe](https://www.theguardian.com/technology/2025/dec/24/us-state-department-visa-ban-former-eu-commissioner-europe)

生成摘要时出错

---

## 75. Un-Redactor

**原文标题**: Un-Redactor

**原文链接**: [https://github.com/kvthweatt/unredactor](https://github.com/kvthweatt/unredactor)

生成摘要时出错

---

## 76. I'm returning my Framework 16

**原文标题**: I'm returning my Framework 16

**原文链接**: [https://yorickpeterse.com/articles/im-returning-my-framework-16/](https://yorickpeterse.com/articles/im-returning-my-framework-16/)

生成摘要时出错

---

## 77. CEO killed at industrial site by worker operating forklift

**原文标题**: CEO killed at industrial site by worker operating forklift

**原文链接**: [https://www.12onyourside.com/2025/12/23/ceo-killed-industrial-site-by-worker-operating-forklift-while-talking-phone-osha-report-shows/](https://www.12onyourside.com/2025/12/23/ceo-killed-industrial-site-by-worker-operating-forklift-while-talking-phone-osha-report-shows/)

生成摘要时出错

---

## 78. Lua 5.5 Released

**原文标题**: Lua 5.5 Released

**原文链接**: [https://www.lua.org/manual/5.5/readme.html#changes](https://www.lua.org/manual/5.5/readme.html#changes)

生成摘要时出错

---

## 79. Dutch rental fleet Mistergreen goes bankrupt after betting on Tesla self-driving

**原文标题**: Dutch rental fleet Mistergreen goes bankrupt after betting on Tesla self-driving

**原文链接**: [https://guessingheadlights.com/dutch-tesla-fleet-goes-bust-after-betting-on-musks-self-driving-promises/](https://guessingheadlights.com/dutch-tesla-fleet-goes-bust-after-betting-on-musks-self-driving-promises/)

生成摘要时出错

---

## 80. Jim Beam halts production at main distillery for a year

**原文标题**: Jim Beam halts production at main distillery for a year

**原文链接**: [https://www.bbc.com/news/articles/cy5gv5z24n2o](https://www.bbc.com/news/articles/cy5gv5z24n2o)

生成摘要时出错

---

## 81. New reactor produces clean energy and carbon nanotubes from natural gas

**原文标题**: New reactor produces clean energy and carbon nanotubes from natural gas

**原文链接**: [https://phys.org/news/2025-12-reactor-energy-carbon-nanotubes-natural.html](https://phys.org/news/2025-12-reactor-energy-carbon-nanotubes-natural.html)

生成摘要时出错

---

## 82. Fuck You, I Won't Use Tailwind

**原文标题**: Fuck You, I Won't Use Tailwind

**原文链接**: [https://fuckyouiwontusetailwind.com](https://fuckyouiwontusetailwind.com)

生成摘要时出错

---

## 83. I'm tired of Hacker News slop

**原文标题**: I'm tired of Hacker News slop

**原文链接**: [https://blog.absurdpirate.com/im-tired-of-hacker-news-slop/](https://blog.absurdpirate.com/im-tired-of-hacker-news-slop/)

生成摘要时出错

---

## 84. Is the golden age of Indie software over?

**原文标题**: Is the golden age of Indie software over?

**原文链接**: [https://successfulsoftware.net/2025/12/22/is-the-golden-age-of-indie-software-over/](https://successfulsoftware.net/2025/12/22/is-the-golden-age-of-indie-software-over/)

生成摘要时出错

---

## 85. Feds demand compromise on Colorado River while states flounder

**原文标题**: Feds demand compromise on Colorado River while states flounder

**原文链接**: [https://nevadacurrent.com/2025/12/22/feds-demand-compromise-on-colorado-river-states-flounder-despite-water-shoratge/](https://nevadacurrent.com/2025/12/22/feds-demand-compromise-on-colorado-river-states-flounder-despite-water-shoratge/)

生成摘要时出错

---

## 86. Researchers achieved 1,270 Wh/L in an anode-free lithium metal battery

**原文标题**: Researchers achieved 1,270 Wh/L in an anode-free lithium metal battery

**原文链接**: [https://postech.ac.kr/eng/research/research_results.do?mode=view&articleNo=43617&title=Anode-Free+Battery+Doubles+Electric+Vehicle+Driving+Range](https://postech.ac.kr/eng/research/research_results.do?mode=view&articleNo=43617&title=Anode-Free+Battery+Doubles+Electric+Vehicle+Driving+Range)

生成摘要时出错

---

## 87. The EU's Fine Against X Is Not About Speech or 'Censorship'

**原文标题**: The EU's Fine Against X Is Not About Speech or 'Censorship'

**原文链接**: [https://www.techpolicy.press/the-eus-fine-against-x-is-not-about-speech-or-censorship/](https://www.techpolicy.press/the-eus-fine-against-x-is-not-about-speech-or-censorship/)

生成摘要时出错

---

## 88. iOS 26.2 lockscreen clock is slowly moving left

**原文标题**: iOS 26.2 lockscreen clock is slowly moving left

**原文链接**: [https://twitter.com/ffaebi/status/2003548130936332519](https://twitter.com/ffaebi/status/2003548130936332519)

生成摘要时出错

---

## 89. Mt. Gox CEO Karpelès Reveals Details of 2014 Collapse and Japanese Detention

**原文标题**: Mt. Gox CEO Karpelès Reveals Details of 2014 Collapse and Japanese Detention

**原文链接**: [https://bitcoinmagazine.com/business/former-mt-gox-ceo-mark-karpeles-reveals-details-of-2014-collapse-and-japanese-detention](https://bitcoinmagazine.com/business/former-mt-gox-ceo-mark-karpeles-reveals-details-of-2014-collapse-and-japanese-detention)

生成摘要时出错

---

## 90. Amnezia – Self-Hosted VPN

**原文标题**: Amnezia – Self-Hosted VPN

**原文链接**: [https://amnezia.org/self-hosted](https://amnezia.org/self-hosted)

生成摘要时出错

---

## 91. Tc – Theodore Calvin's language-agnostic testing framework

**原文标题**: Tc – Theodore Calvin's language-agnostic testing framework

**原文链接**: [https://github.com/ahoward/tc](https://github.com/ahoward/tc)

生成摘要时出错

---

## 92. Custom Cross Compiler with Nix

**原文标题**: Custom Cross Compiler with Nix

**原文链接**: [https://www.hobson.space/posts/nixcross/](https://www.hobson.space/posts/nixcross/)

生成摘要时出错

---

## 93. NYC Spends $200 Million on Cell Service for School Chromebooks

**原文标题**: NYC Spends $200 Million on Cell Service for School Chromebooks

**原文链接**: [https://nysfocus.com/2025/12/22/eric-adams-school-chromebooks-contract](https://nysfocus.com/2025/12/22/eric-adams-school-chromebooks-contract)

生成摘要时出错

---

## 94. Show HN: Vibium – Browser automation for AI and humans, by Selenium's creator

**原文标题**: Show HN: Vibium – Browser automation for AI and humans, by Selenium's creator

**原文链接**: [https://github.com/VibiumDev/vibium](https://github.com/VibiumDev/vibium)

生成摘要时出错

---

## 95. Diesel pollution particles impair lysosomal functions of iPSC-derived microglia

**原文标题**: Diesel pollution particles impair lysosomal functions of iPSC-derived microglia

**原文链接**: [https://www.sciencedirect.com/science/article/pii/S0160412025002181](https://www.sciencedirect.com/science/article/pii/S0160412025002181)

生成摘要时出错

---

## 96. GitHub Is Down

**原文标题**: GitHub Is Down

**原文链接**: [https://downdetector.com/status/github/](https://downdetector.com/status/github/)

生成摘要时出错

---

## 97. Deplatforming Backfired

**原文标题**: Deplatforming Backfired

**原文链接**: [https://reason.com/2025/12/22/deplatforming-backfired/](https://reason.com/2025/12/22/deplatforming-backfired/)

生成摘要时出错

---

## 98. An amateur codebreaker may have just solved the Black Dahlia and Zodiac killings

**原文标题**: An amateur codebreaker may have just solved the Black Dahlia and Zodiac killings

**原文链接**: [https://www.latimes.com/california/story/2025-12-23/black-dahlia-zodiac-killings-connected-one-killer-theory](https://www.latimes.com/california/story/2025-12-23/black-dahlia-zodiac-killings-connected-one-killer-theory)

生成摘要时出错

---

## 99. Quake's Player Speed According to John Romero (2017)

**原文标题**: Quake's Player Speed According to John Romero (2017)

**原文链接**: [https://rome.ro/quakes-player-speed-1](https://rome.ro/quakes-player-speed-1)

生成摘要时出错

---

## 100. Show HN: Kapso – WhatsApp for developers

**原文标题**: Show HN: Kapso – WhatsApp for developers

**原文链接**: [https://kapso.ai/](https://kapso.ai/)

生成摘要时出错

---

