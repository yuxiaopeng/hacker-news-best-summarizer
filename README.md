# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2025-12-20.md)

*最后自动更新时间: 2025-12-20 19:45:42*
## 1. Hacker News 现在的首页，但标题很诚实

**原文标题**: Hacker News front page now, but the titles are honest

**原文链接**: [https://dosaygo-studio.github.io/hn-front-page-2035/news-honest.html](https://dosaygo-studio.github.io/hn-front-page-2035/news-honest.html)

本篇文章介绍了一个讽刺性的Hacker News首页“诚实版”。它模仿了熟悉的Hacker News布局，将典型的文章标题替换为对科技新闻和趋势的内容、潜在动机或更广泛影响的讽刺、幽默且常常直白的描述。

这些“诚实”的标题嘲讽了科技行业和在线文化的各个方面，例如：
*   **科技趋势和炒作：** “我们用Rust重写了它，所以你必须点赞”，“Rails开发者第50次重新发明状态机。”
*   **企业行为：** “亚马逊终于添加了一个自2005年以来就已成为标配的功能”，“OpenAI发布新模型以转移人们对其董事会闹剧的注意力。”
*   **营销伪装成内容：** “解释你为什么要购买我们产品的营销博客文章”，“伪装成技术教程的Ngrok广告。”
*   **开发者项目和抱负：** “我只是为了学习泛型而构建了一种没人会用的语言”，“请给我的仓库加星，这样我才能找到工作。”
*   **社会评论：** “连邮件都不会用的政客试图禁用互联网”，“杂货太贵了，我写了个爬虫。”
*   **人工智能的影响：** “用1913年的数据训练AI以避免‘觉醒’偏见（和卫生）”，“利用色情内容污染AI数据集。”

这份合集充当了一种幽默的批判，突出了Hacker News等平台上常常不言而喻的现实和常见套路。

---

## 2. 我们通过供应链攻击攻陷了X、Vercel、Cursor和Discord。

**原文标题**: We pwned X, Vercel, Cursor, and Discord through a supply-chain attack

**原文链接**: [https://gist.github.com/hackermondev/5e2cdc32849405fff6b46957747a2d28](https://gist.github.com/hackermondev/5e2cdc32849405fff6b46957747a2d28)

16岁的高中应届毕业生兼经验丰富的漏洞赏金猎人丹尼尔，详细描述了一次涉及Mintlify的严重供应链攻击，Mintlify是一个被多家大公司采用的人工智能文档平台。

他的调查始于Discord将其开发者文档切换到Mintlify之后。丹尼尔发现了一个源于Mintlify内部API端点的跨站脚本（XSS）漏洞。他最初发现了`/_mintlify/_markdown/_sites/[subdomain]/[...route]`这个端点，它允许从任何Mintlify文档中获取原始markdown内容，但无法执行代码。

进一步深入研究Mintlify的公共CLI软件包后，丹尼尔发现了`/_mintlify/static/[subdomain]/[...route]`。这个端点同样缺乏子域名验证，允许从任何Mintlify托管的文档中获取静态文件。丹尼尔发现SVG文件被列入白名单。他利用这一点，将JavaScript嵌入到一个SVG文件中，并将其托管在他的Mintlify账户上，然后通过一个易受攻击的域名加载（例如，`discord.com/_mintlify/_static/hackerone-a00f3c6c/lmao.svg`）。通过一个恶意链接，这使得在受害者域名上执行任意JavaScript成为可能。

发现后，丹尼尔与同样在Mintlify中发现了其他关键漏洞的朋友xyzeva和MDL合作。他们负责任地向Discord和Mintlify报告了这些问题。Discord立即下线了其开发者文档，并恢复到旧平台。Mintlify的工程团队迅速与这些黑客合作，修复了此漏洞及其他漏洞。

这次XSS攻击影响了几乎所有在其主域名上托管文档的Mintlify客户，包括X（Twitter）、Vercel、Cursor和Discord，使他们面临账户被接管的风险。该团队因其负责任的披露，总共获得了大约11,000美元的漏洞赏金，这突显了供应链漏洞的严重影响。

---

## 3. 历史大语言模型：仅基于1913年前文本训练的模型

**原文标题**: History LLMs: Models trained exclusively on pre-1913 texts

**原文链接**: [https://github.com/DGoettlich/history-llms](https://github.com/DGoettlich/history-llms)

由苏黎世大学和科隆大学研究人员牵头的“历史LLM”项目，正在开发专门基于历史文献训练的大型语言模型（LLM），这些模型的训练数据截止到特定的“知识截断点”，例如1913年、1929年和1933年。他们即将推出的Ranke-4B系列将是基于Qwen3的40亿参数模型，从一个精选的6000亿个token历史数据集中，使用800亿个token从头开始训练。

核心目标是创建“时间锁定”模型，作为人文科学、社会科学和计算机科学研究的“通往过去的窗口”。与存在“后见之明污染”（即已知截断点之后事件）的现代LLM不同，这些模型确实不掌握其训练截止日期之后的信息。这使得它们能够在不受现代干扰的情况下，反映其所处时代的历史文本文化和规范性判断，从而使研究人员能够探索在特定历史时期哪些是可知或可思的。

示例证明了这一点：1913年模型提供了一个关于阿道夫·希特勒的虚构传记，表达了对奴隶制的复杂看法，并反映了关于女性角色和同性恋的历史偏见。该项目承认模型将复现历史文本中存在的敏感内容（如种族主义、厌女症），并将其视为理解过去社会观点的关键特征。目前正在为学术用途开发一个负责任的访问框架，并且所有项目成果，包括模型和数据，都将公开发布。

---

## 4. CSS 网格轨道

**原文标题**: CSS Grid Lanes

**原文链接**: [https://webkit.org/blog/17660/introducing-css-grid-lanes/](https://webkit.org/blog/17660/introducing-css-grid-lanes/)

本文介绍了 CSS Grid 泳道，一项支持原生瀑布流布局的新网页标准。它经过多年的跨浏览器协作开发，目前可在 Safari Technology Preview 234 中使用。

Grid 泳道通过在容器上使用 `display: grid-lanes` 来简化响应式布局。结合 `grid-template-columns`（例如 `repeat(auto-fill, minmax(250px, 1fr))`）和 `gap`，它能创建灵活的、自动填充的列，将项目放置在最靠近顶部的列中。这种方法消除了对媒体查询或容器查询的需求，通过保持逻辑的 Tab 键顺序来提高可访问性，并在无需 JavaScript 的情况下支持无限滚动。

除了基本的瀑布流布局，Grid 泳道还提供了 CSS Grid 的全部功能。开发者可以定义不同的泳道尺寸，让项目跨越多个泳道（`grid-column: span X`），并显式放置元素。布局方向可以通过定义 `grid-template-columns`（用于实现“瀑布”效果）或 `grid-template-rows`（用于实现“砖墙”效果）来控制，同时利用 `grid-auto-flow: normal`。

一个关键创新是 `item-tolerance` 属性，它调整了布局算法在根据微小尺寸差异放置项目时的“挑剔”程度。默认值为 `1em`，它确保只有有意义的尺寸变化才会影响放置，从而防止视觉或逻辑顺序上出现干扰性的改变。

随着该功能（包括像 `item-tolerance` 这样的潜在属性名称更改）的最终确定，鼓励开发者尝试 Grid 泳道，构建演示并提供反馈。

---

## 5. 车库 – S3对象存储，可靠到可在数据中心外部运行

**原文标题**: Garage – An S3 object store so reliable you can run it outside datacenters

**原文链接**: [https://garagehq.deuxfleurs.fr/](https://garagehq.deuxfleurs.fr/)

Garage 是一个 S3 对象存储，旨在实现卓越的可靠性，使其即使在传统数据中心之外也能有效运行。它通过将每个数据块复制到三个独立的区域（每个区域由多台服务器组成）来确保数据冗余。

该项目强调轻量化和高效率，以自包含、无依赖的二进制文件形式交付，兼容所有 Linux 发行版。这种设计使其部署快速、运行安全，优先考虑操作员的友好性。Garage 专为广泛部署而构建，能够跨互联网和多个数据中心运行，对网络故障、延迟、磁盘故障和操作错误表现出高弹性。

它拥有极低的硬件

Garage 实现了 Amazon S3 API，确保与现有应用程序的广泛兼容性。其架构借鉴了知名分布式系统研究的见解，包括亚马逊的 Dynamo、无冲突复制数据类型和 Maglev。该项目已获得 NGI POINTER、NLnet/NGI0 Entrust 和 NLnet/NGI0 Commons 等欧盟项目的重大公共资助，并积极寻求进一步支持。

---

## 6. 亚马逊将允许下载无DRM电子书的ePub和PDF文件。

**原文标题**: Amazon will allow ePub and PDF downloads for DRM-free eBooks

**原文链接**: [https://www.kdpcommunity.com/s/article/New-eBook-Download-Options-for-Readers-Coming-in-2026?language=en_US](https://www.kdpcommunity.com/s/article/New-eBook-Download-Options-for-Readers-Coming-in-2026?language=en_US)

根据所提供的标题“亚马逊将允许下载无DRM保护的ePub和PDF电子书”，该文章可能宣布了亚马逊的一项重大政策变更。

这一更新表明，亚马逊Kindle用户将很快能够直接下载和阅读无数字版权管理（DRM）保护的电子书的ePub和PDF文件。这标志着亚马逊从其历来专注于专有Kindle格式（AZW、MOBI）的做法上，发生了显著的转变。这一变化将为读者提供更大的灵活性，使他们能够更轻松地将从各种来源获取的无DRM保护的数字图书收藏直接整合并访问到Kindle生态系统中，从而简化内容管理，而无需进行格式转换。

（请注意：所提供的内容主体不完整（“KDP Community Loading×Sorry to interruptCSS ErrorRefresh”）。本摘要仅基于标题中明确传达的信息。）

---

## 7. Mac Studio 1.5 TB 显存 — Thunderbolt 5 上的 RDMA

**原文标题**: 1.5 TB of VRAM on Mac Studio – RDMA over Thunderbolt 5

**原文链接**: [https://www.jeffgeerling.com/blog/2025/15-tb-vram-on-mac-studio-rdma-over-thunderbolt-5](https://www.jeffgeerling.com/blog/2025/15-tb-vram-on-mac-studio-rdma-over-thunderbolt-5)

作者测试了一个由四台Apple Mac Studio组成的集群，总计1.5 TB的统一内存，价值近40,000美元，目的是评估macOS 26.2中的一项新功能——基于Thunderbolt 5的RDMA（远程直接内存访问）。利用开源工具Exo 1.0，RDMA使这些Macs能够作为一个巨大的共享内存池运行，将内存访问延迟从300微秒大幅降低到50微秒以下，这对于大型AI模型至关重要。

M3 Ultra Mac Studio展现出强大的独立性能，FP64浮点运算能力突破1 Tflop，并在AI推理方面表现出色，其功耗和效率常优于Nvidia DGX Spark和AMD AI Max+ 395等竞争系统。该集群（安装在DeskPi迷你机架中）成功运行了Kimi K2 Thinking（1万亿参数）和DeepSeek V3.1（6710亿参数）等单机无法处理的巨型AI模型。Exo 1.0利用RDMA，随着节点数量的增加，性能扩展性得到提升，这与效率较低的RPC方法不同。

挑战包括macOS集群管理的繁琐（例如，没有SSH系统升级）、Thunderbolt 5凌乱的布线、缺乏Thunderbolt交换机，以及目前只能交叉连接四台Mac的限制。预发布的RDMA软件也遇到了稳定性问题。作者还对Exo的秘密开发及其对M1/M2 Mac的向后兼容性表示担忧。尽管存在这些障碍，M3 Ultra Mac Studio仍被誉为强大、安静、高效的工作站，甚至超越了AI应用领域。

---

## 8. GotaTun – Mullvad's WireGuard Implementation in Rust

**原文标题**: GotaTun – Mullvad's WireGuard Implementation in Rust

**原文链接**: [https://mullvad.net/en/blog/announcing-gotatun-the-future-of-wireguard-at-mullvad-vpn](https://mullvad.net/en/blog/announcing-gotatun-the-future-of-wireguard-at-mullvad-vpn)

生成摘要时出错

---

## 9. Noclip.website – A digital museum of video game levels

**原文标题**: Noclip.website – A digital museum of video game levels

**原文链接**: [https://noclip.website/](https://noclip.website/)

生成摘要时出错

---

## 10. How China built its ‘Manhattan Project’ to rival the West in AI chips

**原文标题**: How China built its ‘Manhattan Project’ to rival the West in AI chips

**原文链接**: [https://www.japantimes.co.jp/business/2025/12/18/tech/china-west-ai-chips/](https://www.japantimes.co.jp/business/2025/12/18/tech/china-west-ai-chips/)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 2 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 3 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 4 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 5 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 6 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 7 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 8 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 9 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 10 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 11 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 12 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 13 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 14 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 15 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 16 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 17 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 18 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 19 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 20 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 21 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 22 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 23 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 24 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 25 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 26 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 27 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 28 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 29 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 30 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 31 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 32 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 33 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 34 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 35 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 36 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 37 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 38 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 39 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 40 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 41 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 42 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 43 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
| 44 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 45 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
