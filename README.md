# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-06-16.md)

*最后自动更新时间: 2026-06-16 22:07:24*
## 1. 领英工作邀约中的后门

**原文标题**: A backdoor in a LinkedIn job offer

**原文链接**: [https://roman.pt/posts/linkedin-backdoor/](https://roman.pt/posts/linkedin-backdoor/)

一名软件工程师收到了一份来自加密货币初创公司的可疑LinkedIn工作邀约，其中要求他审查一个公共GitHub仓库，并特别指出“查看废弃的Node模块问题”——这是一个巧妙的提示，意在让他运行 `npm install`。

工程师没有直接与代码交互，而是使用了一次性VPS和一个只读AI代理（Pi）进行分析。该代理立即标记了 `app/test/index.js` 这个伪装成测试套件的文件。这个恶意脚本旨在组装一个URL (`https://rest-icon-handler.store/icons/77`)，并执行从该服务器接收到的任何有效载荷。

后门自动触发：`package.json`中的 `prepare` 脚本在 `npm install` 之后执行，运行了 `app/index.js`，而后者又 `require` 并执行了 `app/test/index.js`。因此，仅仅安装依赖项就会激活有效载荷。

进一步调查揭示了严重的身份盗用行为。GitHub仓库的提交被归因于一位合法的开发者，他证实自己被冒充，与该项目没有任何关系。同样，“招聘人员”的LinkedIn个人资料属于一名非技术出身的艺术记者，当被追问安装问题时，她却莫名其妙地表现出对npm的专业知识。

作者强调，此类复杂的社会工程攻击可能影响任何人，强调在审查外部代码时保持警惕和良好的安全卫生习惯的重要性。该事件也凸显了使用AI代理快速识别隐藏威胁的效率。该仓库和招聘人员已被举报，但仍处于活跃状态。

---

## 2. 艾洛 1.0

**原文标题**: Iroh 1.0

**原文链接**: [https://www.iroh.computer/blog/v1](https://www.iroh.computer/blog/v1)

Iroh 1.0 正式发布，标志着互联网架构从脆弱的IP地址向“拨号键”（dial keys）的根本性转变。这些由用户控制的持久密钥允许设备在任何地方，即使在防火墙后也能安全、直接地连接，有效地将互联网转变为“安全本地主机”（secure localhost）。

经过四年多的开发和65个预发布版本，Iroh 1.0是第一个稳定版本。它已被广泛采用，公共中继在30天内创建了超过2亿个端点，为数百万设备上的视频流、LLM、游戏和文件共享等各种应用提供支持。

主要创新包括遵循开放标准、定制化的QUIC多路径和NAT穿透以实现弹性、加密的直接连接，以及本地优先（local-first）配置。Iroh支持蓝牙和Tor等自定义传输方式，可编译为WASM，并实现高效的直接数据传输（95%直接），从而降低出口成本并提高整体网络效率。

除了其Rust核心，Iroh 1.0现在正式支持Python、Node.js、Swift和Kotlin，从而能够集成到移动和Web应用程序中。此版本保证了v1端点的有线协议（wire protocol）和语言API的稳定性，并有明确的时间表支持。鼓励开发者基于这个成熟的开源网络堆栈进行开发，利用其安全、直接和普遍可寻址的连接。

---

## 3. TinyWind: 一款搭载真实风力物理引擎的像素海盗航海游戏（累计航行38万+公里）

**原文标题**: TinyWind: A pixel pirate sailing game with real wind physics (380k+ kms sailed)

**原文链接**: [https://tinywind.io](https://tinywind.io)

TinyWind是一款像素海盗航海游戏，其特色在于融入了真实的风力物理系统，为玩家提供真实的航海体验。该游戏吸引了大量玩家参与，玩家们在其像素世界中累计航行了超过38万公里。

---

## 4. 你的 ePub 没问题

**原文标题**: Your ePub Is fine

**原文链接**: [https://andreklein.net/your-epub-is-fine-kobo-disagrees-blame-adobe/](https://andreklein.net/your-epub-is-fine-kobo-disagrees-blame-adobe/)

生成摘要时出错

---

## 5. 我钦佩 Fabrice Bellard。他几乎肯定是一个更优秀的全能程序员。

**原文标题**: I admire Fabrice Bellard. He is almost certainly a better overall programmer

**原文链接**: [https://twitter.com/ID_AA_Carmack/status/2064095424420487226](https://twitter.com/ID_AA_Carmack/status/2064095424420487226)

文章强调了法国工程师法布里斯·贝拉尔对互联网基础设施的深刻但鲜为人知的贡献。传奇程序员约翰·卡马克对贝拉尔表达了极大的钦佩，称他“几乎可以肯定是一个比自己更优秀的全面型程序员”。斯宾塞·巴金斯进一步阐述了贝拉尔的影响，指出这位在巴黎工作了30年的沉默工程师，开发了支撑着现代互联网大部分的基础软件。具体来说，贝拉尔被认为是编写了为YouTube、Netflix和TikTok等平台实现流媒体传输的核心代码。文章强调的核心讽刺是，尽管数十亿人每天都依赖他的软件，他的名字却在公众中鲜为人知。

---

## 6. 现在运行本地模型很不错

**原文标题**: Running local models is good now

**原文链接**: [https://vickiboykis.com/2026/06/15/running-local-models-is-good-now/](https://vickiboykis.com/2026/06/15/running-local-models-is-good-now/)

作者自本地模型诞生之初便与其打交道，注意到其性能有了显著提升，尤其是在GPT-OSS发布之后，以及最近谷歌Gemma 4系列的推出。作者使用一台搭载64GB内存的M2 Mac，在包括LM Studio和Ollama在内的多种配置下，试验过Mistral 7B、Gemma 3、通义千问（Qwen）变体以及OpenAI OSS-20B等模型。

过去，本地模型运行缓慢且准确性不高，但现在它们在代理式编码方面表现已足够出色，能达到前沿模型约75%的准确性和速度。作者主要使用的本地模型是`gemma-4-26b-a4b`（后来更新为`gemma-4-12b-qat`），它已被用于重构Python脚本、代码检查、校对博客文章、编写单元测试，甚至用于引导一个双塔推荐模型代码库。这些任务在仅仅六个月前对于本地模型来说还被认为是不可能完成的，这充分展示了它们能力的显著提升。

为了在本地运行代理工作流，作者使用Pi作为代理框架，LM Studio作为推理服务器，并推荐`gemma-4-12b-qat`，因为它在模型大小和性能之间取得了良好的平衡。文中还提供了一个详细的基于Docker的设置，用于实现安全、隔离的执行环境，从而防止代理修改宿主系统。

尽管作者承认本地模型存在推理速度、上下文窗口大小以及提示模板不匹配等局限性（尽管这些问题通常能迅速得到修复），但作者强调了其诸多优势。本地模型允许用户深入探究token推理过程、观察上下文窗口调整带来的性能变化，并能在GPU上进行处理。这使得广泛的定制化、实验成为可能，并促进了一个至关重要的开源生态系统，即使这些模型尚未完全达到生产就绪状态。

---

## 7. Curl will not accept vulnerability reports during July 2026

**原文标题**: Curl will not accept vulnerability reports during July 2026

**原文链接**: [https://daniel.haxx.se/blog/2026/06/15/curl-summer-of-bliss/](https://daniel.haxx.se/blog/2026/06/15/curl-summer-of-bliss/)

生成摘要时出错

---

## 8. SpaceX to buy Cursor for $60B

**原文标题**: SpaceX to buy Cursor for $60B

**原文链接**: [https://www.reuters.com/legal/transactional/spacex-buy-anysphere-60-billion-2026-06-16/](https://www.reuters.com/legal/transactional/spacex-buy-anysphere-60-billion-2026-06-16/)

生成摘要时出错

---

## 9. 极客怎么了？

**原文标题**: What happened to nerds?

**原文链接**: [https://mrmarket.lol/what-the-fuck-happened-to-nerds/](https://mrmarket.lol/what-the-fuck-happened-to-nerds/)

生成摘要时出错

---

## 10. CrankGPT

**原文标题**: CrankGPT

**原文链接**: [https://crankgpt.com](https://crankgpt.com)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 2 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 3 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 4 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 5 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 6 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 7 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 8 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 9 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 10 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 11 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 12 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 13 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 14 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 15 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 16 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 17 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 18 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 19 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 20 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 21 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 22 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 23 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 24 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 25 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 26 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 27 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 28 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 29 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 30 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 31 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 32 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 33 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 34 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 35 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 36 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 37 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 38 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 39 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 40 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 41 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 42 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 43 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 44 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 45 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 46 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 47 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 48 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 49 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 50 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 51 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 52 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 53 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 54 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 55 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 56 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 57 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 58 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 59 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 60 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 61 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 62 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 63 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 64 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 65 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 66 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 67 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 68 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 69 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 70 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 71 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 72 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 73 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 74 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 75 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 76 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 77 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 78 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 79 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 80 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 81 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 82 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 83 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 84 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 85 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 86 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 87 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 88 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 89 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 90 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 91 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 92 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 93 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 94 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 95 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 96 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 97 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 98 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 99 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 100 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 101 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 102 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 103 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 104 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 105 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 106 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 107 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 108 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 109 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 110 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 111 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 112 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 113 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 114 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 115 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 116 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 117 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 118 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 119 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 120 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 121 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 122 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 123 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 124 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 125 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 126 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 127 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 128 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 129 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 130 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 131 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 132 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 133 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 134 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 135 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 136 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 137 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 138 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 139 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 140 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 141 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 142 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 143 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 144 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 145 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 146 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 147 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 148 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 149 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 150 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 151 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 152 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 153 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 154 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 155 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 156 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 157 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 158 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 159 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 160 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 161 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 162 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 163 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 164 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 165 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 166 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 167 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 168 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 169 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 170 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 171 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 172 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 173 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 174 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 175 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 176 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 177 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 178 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 179 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 180 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 181 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 182 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 183 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 184 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 185 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 186 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 187 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 188 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 189 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 190 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 191 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 192 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 193 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 194 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 195 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 196 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 197 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 198 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 199 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 200 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 201 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 202 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 203 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 204 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 205 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 206 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 207 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 208 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 209 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 210 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 211 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 212 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 213 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 214 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 215 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 216 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 217 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 218 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 219 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 220 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 221 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
