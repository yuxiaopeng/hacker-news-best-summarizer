# Hacker News 热门文章摘要 (2025-12-20)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

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

## 11. Airbus to migrate critical apps to a sovereign Euro cloud

**原文标题**: Airbus to migrate critical apps to a sovereign Euro cloud

**原文链接**: [https://www.theregister.com/2025/12/19/airbus_sovereign_cloud/](https://www.theregister.com/2025/12/19/airbus_sovereign_cloud/)

生成摘要时出错

---

## 12. NTP at NIST Boulder Has Lost Power

**原文标题**: NTP at NIST Boulder Has Lost Power

**原文链接**: [https://lists.nanog.org/archives/list/nanog@lists.nanog.org/message/ACADD3NKOG2QRWZ56OSNNG7UIEKKTZXL/](https://lists.nanog.org/archives/list/nanog@lists.nanog.org/message/ACADD3NKOG2QRWZ56OSNNG7UIEKKTZXL/)

生成摘要时出错

---

## 13. LLM Year in Review

**原文标题**: LLM Year in Review

**原文链接**: [https://karpathy.bearblog.dev/year-in-review-2025/](https://karpathy.bearblog.dev/year-in-review-2025/)

生成摘要时出错

---

## 14. TP-Link Tapo C200: Hardcoded Keys, Buffer Overflows and Privacy

**原文标题**: TP-Link Tapo C200: Hardcoded Keys, Buffer Overflows and Privacy

**原文链接**: [https://www.evilsocket.net/2025/12/18/TP-Link-Tapo-C200-Hardcoded-Keys-Buffer-Overflows-and-Privacy-in-the-Era-of-AI-Assisted-Reverse-Engineering/](https://www.evilsocket.net/2025/12/18/TP-Link-Tapo-C200-Hardcoded-Keys-Buffer-Overflows-and-Privacy-in-the-Era-of-AI-Assisted-Reverse-Engineering/)

生成摘要时出错

---

## 15. You can now play Grand Theft Auto Vice City in the browser

**原文标题**: You can now play Grand Theft Auto Vice City in the browser

**原文链接**: [https://dos.zone/grand-theft-auto-vice-city/](https://dos.zone/grand-theft-auto-vice-city/)

生成摘要时出错

---

## 16. 8-bit Boléro

**原文标题**: 8-bit Boléro

**原文链接**: [https://linusakesson.net/music/bolero/index.php](https://linusakesson.net/music/bolero/index.php)

生成摘要时出错

---

## 17. TikTok Deal Is the Shittiest Possible Outcome, Making Everything Worse

**原文标题**: TikTok Deal Is the Shittiest Possible Outcome, Making Everything Worse

**原文链接**: [https://www.techdirt.com/2025/12/19/tiktok-deal-done-and-its-somehow-the-shittiest-possible-outcome-making-everything-worse/](https://www.techdirt.com/2025/12/19/tiktok-deal-done-and-its-somehow-the-shittiest-possible-outcome-making-everything-worse/)

生成摘要时出错

---

## 18. Privacy doesn't mean anything anymore, anonymity does

**原文标题**: Privacy doesn't mean anything anymore, anonymity does

**原文链接**: [https://servury.com/blog/privacy-is-marketing-anonymity-is-architecture/](https://servury.com/blog/privacy-is-marketing-anonymity-is-architecture/)

生成摘要时出错

---

## 19. Getting bitten by Intel's poor naming schemes

**原文标题**: Getting bitten by Intel's poor naming schemes

**原文链接**: [https://lorendb.dev/posts/getting-bitten-by-poor-naming-schemes/](https://lorendb.dev/posts/getting-bitten-by-poor-naming-schemes/)

生成摘要时出错

---

## 20. Charles Proxy

**原文标题**: Charles Proxy

**原文链接**: [https://www.charlesproxy.com/](https://www.charlesproxy.com/)

生成摘要时出错

---

## 21. Go ahead, self-host Postgres

**原文标题**: Go ahead, self-host Postgres

**原文链接**: [https://pierce.dev/notes/go-ahead-self-host-postgres#user-content-fn-1](https://pierce.dev/notes/go-ahead-self-host-postgres#user-content-fn-1)

生成摘要时出错

---

## 22. Graphite is joining Cursor

**原文标题**: Graphite is joining Cursor

**原文链接**: [https://cursor.com/blog/graphite](https://cursor.com/blog/graphite)

生成摘要时出错

---

## 23. 2026 Apple introducing more ads to increase opportunity in search results

**原文标题**: 2026 Apple introducing more ads to increase opportunity in search results

**原文链接**: [https://ads.apple.com/app-store/help/ad-placements/0082-search-results](https://ads.apple.com/app-store/help/ad-placements/0082-search-results)

生成摘要时出错

---

## 24. Wall Street ruined the Roomba and then blamed Lina Khan

**原文标题**: Wall Street ruined the Roomba and then blamed Lina Khan

**原文链接**: [https://www.thebignewsletter.com/p/how-wall-street-ruined-the-roomba](https://www.thebignewsletter.com/p/how-wall-street-ruined-the-roomba)

生成摘要时出错

---

## 25. FunctionGemma 270M Model

**原文标题**: FunctionGemma 270M Model

**原文链接**: [https://blog.google/technology/developers/functiongemma/](https://blog.google/technology/developers/functiongemma/)

生成摘要时出错

---

## 26. Show HN: TinyPDF – 3kb pdf library (70x smaller than jsPDF)

**原文标题**: Show HN: TinyPDF – 3kb pdf library (70x smaller than jsPDF)

**原文链接**: [https://github.com/Lulzx/tinypdf](https://github.com/Lulzx/tinypdf)

生成摘要时出错

---

## 27. Rust's Block Pattern

**原文标题**: Rust's Block Pattern

**原文链接**: [https://notgull.net/block-pattern/](https://notgull.net/block-pattern/)

生成摘要时出错

---

## 28. Android introduces $2-4 install fee and 10–20% cut for US external content links

**原文标题**: Android introduces $2-4 install fee and 10–20% cut for US external content links

**原文链接**: [https://support.google.com/googleplay/android-developer/answer/16470497?hl=en](https://support.google.com/googleplay/android-developer/answer/16470497?hl=en)

生成摘要时出错

---

## 29. Great ideas in theoretical computer science

**原文标题**: Great ideas in theoretical computer science

**原文链接**: [https://www.cs251.com/](https://www.cs251.com/)

生成摘要时出错

---

## 30. Skills Officially Comes to Codex

**原文标题**: Skills Officially Comes to Codex

**原文链接**: [https://developers.openai.com/codex/skills/](https://developers.openai.com/codex/skills/)

生成摘要时出错

---

## 31. Show HN: Hacker News, but every headline is hysterical clickbait

**原文标题**: Show HN: Hacker News, but every headline is hysterical clickbait

**原文链接**: [https://dosaygo-studio.github.io/hn-front-page-2035/news-max.html](https://dosaygo-studio.github.io/hn-front-page-2035/news-max.html)

生成摘要时出错

---

## 32. Brown/MIT shooting suspect found dead, officials say

**原文标题**: Brown/MIT shooting suspect found dead, officials say

**原文链接**: [https://www.washingtonpost.com/nation/2025/12/18/brown-university-shooting-person-of-interest/](https://www.washingtonpost.com/nation/2025/12/18/brown-university-shooting-person-of-interest/)

生成摘要时出错

---

## 33. The Deviancy Signal: Having "Nothing to Hide" Is a Threat to Us All

**原文标题**: The Deviancy Signal: Having "Nothing to Hide" Is a Threat to Us All

**原文链接**: [https://thompson2026.com/blog/deviancy-signal/](https://thompson2026.com/blog/deviancy-signal/)

生成摘要时出错

---

## 34. The FreeBSD Foundation's Laptop Support and Usability Project

**原文标题**: The FreeBSD Foundation's Laptop Support and Usability Project

**原文链接**: [https://github.com/FreeBSDFoundation/proj-laptop](https://github.com/FreeBSDFoundation/proj-laptop)

生成摘要时出错

---

## 35. How to hack Discord, Vercel and more with one easy trick

**原文标题**: How to hack Discord, Vercel and more with one easy trick

**原文链接**: [https://kibty.town/blog/mintlify/](https://kibty.town/blog/mintlify/)

生成摘要时出错

---

## 36. Reconstructed Commander Keen 1-3 Source Code

**原文标题**: Reconstructed Commander Keen 1-3 Source Code

**原文链接**: [https://pckf.com/viewtopic.php?t=18248](https://pckf.com/viewtopic.php?t=18248)

生成摘要时出错

---

## 37. A better zip bomb (2019)

**原文标题**: A better zip bomb (2019)

**原文链接**: [https://www.bamsoftware.com/hacks/zipbomb/](https://www.bamsoftware.com/hacks/zipbomb/)

生成摘要时出错

---

## 38. Prepare for That Stupid World

**原文标题**: Prepare for That Stupid World

**原文链接**: [https://ploum.net/2025-12-19-prepare-for-that-world.html](https://ploum.net/2025-12-19-prepare-for-that-world.html)

生成摘要时出错

---

## 39. Cursor Acquires Graphite

**原文标题**: Cursor Acquires Graphite

**原文链接**: [https://graphite.com/blog/graphite-joins-cursor](https://graphite.com/blog/graphite-joins-cursor)

生成摘要时出错

---

## 40. Believe the Checkbook

**原文标题**: Believe the Checkbook

**原文链接**: [https://robertgreiner.com/believe-the-checkbook/](https://robertgreiner.com/believe-the-checkbook/)

生成摘要时出错

---

## 41. Build Your Own React

**原文标题**: Build Your Own React

**原文链接**: [https://pomb.us/build-your-own-react/](https://pomb.us/build-your-own-react/)

生成摘要时出错

---

## 42. The Scottish Highlands, the Appalachians, Atlas are the same mountain range

**原文标题**: The Scottish Highlands, the Appalachians, Atlas are the same mountain range

**原文链接**: [https://vividmaps.com/central-pangean-mountains/](https://vividmaps.com/central-pangean-mountains/)

生成摘要时出错

---

## 43. PBS News Hour West to go dark after ASU discontinues contract

**原文标题**: PBS News Hour West to go dark after ASU discontinues contract

**原文链接**: [https://www.statepress.com/article/2025/12/politics-pbs-newshour-west-closure](https://www.statepress.com/article/2025/12/politics-pbs-newshour-west-closure)

生成摘要时出错

---

## 44. T5Gemma 2: The next generation of encoder-decoder models

**原文标题**: T5Gemma 2: The next generation of encoder-decoder models

**原文链接**: [https://blog.google/technology/developers/t5gemma-2/](https://blog.google/technology/developers/t5gemma-2/)

生成摘要时出错

---

## 45. Reflections on AI at the End of 2025

**原文标题**: Reflections on AI at the End of 2025

**原文链接**: [https://antirez.com/news/157](https://antirez.com/news/157)

生成摘要时出错

---

## 46. AI vending machine was tricked into giving away everything

**原文标题**: AI vending machine was tricked into giving away everything

**原文链接**: [https://kottke.org/25/12/this-ai-vending-machine-was-tricked-into-giving-away-everything](https://kottke.org/25/12/this-ai-vending-machine-was-tricked-into-giving-away-everything)

生成摘要时出错

---

## 47. Is Proton leaving Switzerland?

**原文标题**: Is Proton leaving Switzerland?

**原文链接**: [https://www.techradar.com/vpn/vpn-privacy-security/is-proton-leaving-switzerland-legal-uncertainty-of-proposed-surveillance-laws-is-pushing-them-to-make-several-changes](https://www.techradar.com/vpn/vpn-privacy-security/is-proton-leaving-switzerland-legal-uncertainty-of-proposed-surveillance-laws-is-pushing-them-to-make-several-changes)

生成摘要时出错

---

## 48. Pure Silicon Demo Coding: No CPU, No Memory, Just 4k Gates

**原文标题**: Pure Silicon Demo Coding: No CPU, No Memory, Just 4k Gates

**原文链接**: [https://www.a1k0n.net/2025/12/19/tiny-tapeout-demo.html](https://www.a1k0n.net/2025/12/19/tiny-tapeout-demo.html)

生成摘要时出错

---

## 49. Two kinds of vibe coding

**原文标题**: Two kinds of vibe coding

**原文链接**: [https://davidbau.com/archives/2025/12/16/vibe_coding.html](https://davidbau.com/archives/2025/12/16/vibe_coding.html)

生成摘要时出错

---

## 50. What Does a Database for SSDs Look Like?

**原文标题**: What Does a Database for SSDs Look Like?

**原文链接**: [https://brooker.co.za/blog/2025/12/15/database-for-ssd.html](https://brooker.co.za/blog/2025/12/15/database-for-ssd.html)

生成摘要时出错

---

## 51. Qwen-Image-Layered: transparency and layer aware open diffusion model

**原文标题**: Qwen-Image-Layered: transparency and layer aware open diffusion model

**原文链接**: [https://huggingface.co/papers/2512.15603](https://huggingface.co/papers/2512.15603)

生成摘要时出错

---

## 52. Over 40% of Deceased Drivers in Vehicle Crashes Test Positive for THC: Study

**原文标题**: Over 40% of Deceased Drivers in Vehicle Crashes Test Positive for THC: Study

**原文链接**: [https://www.facs.org/media-center/press-releases/2025/over-40-of-deceased-drivers-in-motor-vehicle-crashes-test-positive-for-thc-study-shows/](https://www.facs.org/media-center/press-releases/2025/over-40-of-deceased-drivers-in-motor-vehicle-crashes-test-positive-for-thc-study-shows/)

生成摘要时出错

---

## 53. Reverse Engineering US Airline's PNR System and Accessing All Reservations

**原文标题**: Reverse Engineering US Airline's PNR System and Accessing All Reservations

**原文链接**: [https://alexschapiro.com/security/vulnerability/2025/11/20/avelo-airline-reservation-api-vulnerability](https://alexschapiro.com/security/vulnerability/2025/11/20/avelo-airline-reservation-api-vulnerability)

生成摘要时出错

---

## 54. Making Google Sans Flex

**原文标题**: Making Google Sans Flex

**原文链接**: [https://design.google/library/google-sans-flex-font](https://design.google/library/google-sans-flex-font)

生成摘要时出错

---

## 55. Contrails Map

**原文标题**: Contrails Map

**原文链接**: [https://map.contrails.org/](https://map.contrails.org/)

生成摘要时出错

---

## 56. Performance Hints (2023)

**原文标题**: Performance Hints (2023)

**原文链接**: [https://abseil.io/fast/hints.html](https://abseil.io/fast/hints.html)

生成摘要时出错

---

## 57. A train-sized tunnel is now carrying electricity under South London

**原文标题**: A train-sized tunnel is now carrying electricity under South London

**原文链接**: [https://www.ianvisits.co.uk/articles/a-train-sized-tunnel-is-now-carrying-electricity-under-south-london-86221/](https://www.ianvisits.co.uk/articles/a-train-sized-tunnel-is-now-carrying-electricity-under-south-london-86221/)

生成摘要时出错

---

## 58. Immersa: Open-source Web-based 3D Presentation Tool

**原文标题**: Immersa: Open-source Web-based 3D Presentation Tool

**原文链接**: [https://github.com/ertugrulcetin/immersa](https://github.com/ertugrulcetin/immersa)

生成摘要时出错

---

## 59. AMD officially confirms fresh next-gen Zen 6 CPU details

**原文标题**: AMD officially confirms fresh next-gen Zen 6 CPU details

**原文链接**: [https://overclock3d.net/news/cpu_mainboard/amd-officially-confirms-fresh-next-gen-zen-6-cpu-details/](https://overclock3d.net/news/cpu_mainboard/amd-officially-confirms-fresh-next-gen-zen-6-cpu-details/)

生成摘要时出错

---

## 60. The most banned books in U.S. schools

**原文标题**: The most banned books in U.S. schools

**原文链接**: [https://pen.org/top-52-banned-books-since-2021/](https://pen.org/top-52-banned-books-since-2021/)

生成摘要时出错

---

## 61. Using AI Generated Code Will Make You a Bad Programmer

**原文标题**: Using AI Generated Code Will Make You a Bad Programmer

**原文链接**: [https://unsolicited-opinions.rudism.com/bad-programmer/](https://unsolicited-opinions.rudism.com/bad-programmer/)

生成摘要时出错

---

## 62. We ran Anthropic’s interviews through structured LLM analysis

**原文标题**: We ran Anthropic’s interviews through structured LLM analysis

**原文链接**: [https://www.playbookatlas.com/research/ai-adoption-explorer](https://www.playbookatlas.com/research/ai-adoption-explorer)

生成摘要时出错

---

## 63. I have to give Fortnite my passport to use Bluesky

**原文标题**: I have to give Fortnite my passport to use Bluesky

**原文链接**: [https://spitfirenews.com/p/why-i-have-to-give-fortnite-my-passport-to-use-bluesky](https://spitfirenews.com/p/why-i-have-to-give-fortnite-my-passport-to-use-bluesky)

生成摘要时出错

---

## 64. Show HN: I open-sourced my Go and Next B2B SaaS Starter (deploy anywhere, MIT)

**原文标题**: Show HN: I open-sourced my Go and Next B2B SaaS Starter (deploy anywhere, MIT)

**原文链接**: [https://github.com/moasq/production-saas-starter](https://github.com/moasq/production-saas-starter)

生成摘要时出错

---

## 65. North Korean infiltrator caught at Amazon due to 110ms keystroke lag

**原文标题**: North Korean infiltrator caught at Amazon due to 110ms keystroke lag

**原文链接**: [https://www.tomshardware.com/tech-industry/cyber-security/north-korean-infiltrator-caught-working-in-amazon-it-department-thanks-to-lag-110ms-keystroke-input-raises-red-flags-over-true-location](https://www.tomshardware.com/tech-industry/cyber-security/north-korean-infiltrator-caught-working-in-amazon-it-department-thanks-to-lag-110ms-keystroke-input-raises-red-flags-over-true-location)

生成摘要时出错

---

## 66. Engineers who dismiss AI

**原文标题**: Engineers who dismiss AI

**原文链接**: [https://terriblesoftware.org/2025/12/19/the-strange-case-of-engineers-who-dismiss-ai/](https://terriblesoftware.org/2025/12/19/the-strange-case-of-engineers-who-dismiss-ai/)

生成摘要时出错

---

## 67. SMB Direct – SMB3 over RDMA

**原文标题**: SMB Direct – SMB3 over RDMA

**原文链接**: [https://docs.kernel.org/filesystems/smb/smbdirect.html](https://docs.kernel.org/filesystems/smb/smbdirect.html)

生成摘要时出错

---

## 68. Show HN: I Made Loom for Mobile

**原文标题**: Show HN: I Made Loom for Mobile

**原文链接**: [https://demoscope.app](https://demoscope.app)

生成摘要时出错

---

## 69. Building a Transparent Keyserver

**原文标题**: Building a Transparent Keyserver

**原文链接**: [https://words.filippo.io/keyserver-tlog/](https://words.filippo.io/keyserver-tlog/)

生成摘要时出错

---

## 70. Buteyko Method

**原文标题**: Buteyko Method

**原文链接**: [https://en.wikipedia.org/wiki/Buteyko_method](https://en.wikipedia.org/wiki/Buteyko_method)

生成摘要时出错

---

## 71. The scariest boot loader code

**原文标题**: The scariest boot loader code

**原文链接**: [http://miod.online.fr/software/openbsd/stories/boot_hppa.html](http://miod.online.fr/software/openbsd/stories/boot_hppa.html)

生成摘要时出错

---

## 72. AMD Ryzen 7 5800X3D sells for more than 9800X3D, enthusiasts flock to AM4 DDR4

**原文标题**: AMD Ryzen 7 5800X3D sells for more than 9800X3D, enthusiasts flock to AM4 DDR4

**原文链接**: [https://www.tomshardware.com/pc-components/cpus/amds-legacy-ryzen-7-5800x3d-chips-now-sell-for-up-to-usd800-more-than-a-new-9800x3d-am4-chip-costs-twice-as-much-as-msrp-as-enthusiasts-flock-to-old-ddr4-memory](https://www.tomshardware.com/pc-components/cpus/amds-legacy-ryzen-7-5800x3d-chips-now-sell-for-up-to-usd800-more-than-a-new-9800x3d-am4-chip-costs-twice-as-much-as-msrp-as-enthusiasts-flock-to-old-ddr4-memory)

生成摘要时出错

---

## 73. The New Right-Wing Tech Intelligentsia

**原文标题**: The New Right-Wing Tech Intelligentsia

**原文链接**: [https://bayareacurrent.com/meet-the-new-right-wing-tech-intelligentsia/](https://bayareacurrent.com/meet-the-new-right-wing-tech-intelligentsia/)

生成摘要时出错

---

## 74. At least $9B billed across 14 Medicaid services in Minnesota may be fraudulent

**原文标题**: At least $9B billed across 14 Medicaid services in Minnesota may be fraudulent

**原文链接**: [https://www.cbsnews.com/minnesota/news/billions-paid-out-by-medicaid-in-minnesota-may-be-fraudulent-us-attorney/](https://www.cbsnews.com/minnesota/news/billions-paid-out-by-medicaid-in-minnesota-may-be-fraudulent-us-attorney/)

生成摘要时出错

---

## 75. AI's Unpaid Debt: How LLM Scrapers Destroy the Social Contract of Open Source

**原文标题**: AI's Unpaid Debt: How LLM Scrapers Destroy the Social Contract of Open Source

**原文链接**: [https://www.quippd.com/writing/2025/12/17/AIs-unpaid-debt-how-llm-scrapers-destroy-the-social-contract-of-open-source.html](https://www.quippd.com/writing/2025/12/17/AIs-unpaid-debt-how-llm-scrapers-destroy-the-social-contract-of-open-source.html)

生成摘要时出错

---

## 76. Property-Based Testing Caught a Security Bug I Never Would Have Found

**原文标题**: Property-Based Testing Caught a Security Bug I Never Would Have Found

**原文链接**: [https://kiro.dev/blog/property-based-testing-fixed-security-bug/](https://kiro.dev/blog/property-based-testing-fixed-security-bug/)

生成摘要时出错

---

## 77. OpenSCAD Is Kinda Neat

**原文标题**: OpenSCAD Is Kinda Neat

**原文链接**: [https://nuxx.net/blog/2025/12/20/openscad-is-kinda-neat/](https://nuxx.net/blog/2025/12/20/openscad-is-kinda-neat/)

生成摘要时出错

---

## 78. What Makes You Senior

**原文标题**: What Makes You Senior

**原文链接**: [https://terriblesoftware.org/2025/11/25/what-actually-makes-you-senior/](https://terriblesoftware.org/2025/11/25/what-actually-makes-you-senior/)

生成摘要时出错

---

## 79. A proposed amendment to ban under 16s in the UK from common online services

**原文标题**: A proposed amendment to ban under 16s in the UK from common online services

**原文链接**: [https://decoded.legal/blog/2025/12/a-proposed-legislative-amendment-to-attempt-to-ban-under-16s-in-the-uk-from-common-messaging-services-sharing-family-photos-using-wikipedia-and-doing-much-else-online-by-imposing-age-assurance-on-everyone/](https://decoded.legal/blog/2025/12/a-proposed-legislative-amendment-to-attempt-to-ban-under-16s-in-the-uk-from-common-messaging-services-sharing-family-photos-using-wikipedia-and-doing-much-else-online-by-imposing-age-assurance-on-everyone/)

生成摘要时出错

---

## 80. Why we're taking legal action against SerpApi's unlawful scraping

**原文标题**: Why we're taking legal action against SerpApi's unlawful scraping

**原文链接**: [https://blog.google/technology/safety-security/serpapi-lawsuit/](https://blog.google/technology/safety-security/serpapi-lawsuit/)

生成摘要时出错

---

## 81. Is Firefox Firefucked?

**原文标题**: Is Firefox Firefucked?

**原文链接**: [https://kevquirk.com/blog/is-firefox-firefucked/](https://kevquirk.com/blog/is-firefox-firefucked/)

生成摘要时出错

---

## 82. Airbus moving critical systems away from AWS, Google, and MS

**原文标题**: Airbus moving critical systems away from AWS, Google, and MS

**原文链接**: [https://old.reddit.com/r/europe/comments/1pqucbz/airbus_moving_critical_systems_away_from_aws/](https://old.reddit.com/r/europe/comments/1pqucbz/airbus_moving_critical_systems_away_from_aws/)

生成摘要时出错

---

## 83. Performance Hints

**原文标题**: Performance Hints

**原文链接**: [https://abseil.io/fast/hints.html](https://abseil.io/fast/hints.html)

生成摘要时出错

---

## 84. Oliver Sacks put himself into his case studies – what was the cost?

**原文标题**: Oliver Sacks put himself into his case studies – what was the cost?

**原文链接**: [https://www.newyorker.com/magazine/2025/12/15/oliver-sacks-put-himself-into-his-case-studies-what-was-the-cost](https://www.newyorker.com/magazine/2025/12/15/oliver-sacks-put-himself-into-his-case-studies-what-was-the-cost)

生成摘要时出错

---

## 85. Zuckerberg Cut Ties with Pro-Immigration Organization He Founded

**原文标题**: Zuckerberg Cut Ties with Pro-Immigration Organization He Founded

**原文链接**: [https://www.bloomberg.com/news/articles/2025-12-19/mark-zuckerberg-s-philanthropy-cut-ties-with-pro-immigration-organization-fwd-us](https://www.bloomberg.com/news/articles/2025-12-19/mark-zuckerberg-s-philanthropy-cut-ties-with-pro-immigration-organization-fwd-us)

生成摘要时出错

---

## 86. Debian adds LoongArch as officially supported architecture

**原文标题**: Debian adds LoongArch as officially supported architecture

**原文链接**: [https://lists.debian.org/debian-devel-announce/2025/12/msg00004.html](https://lists.debian.org/debian-devel-announce/2025/12/msg00004.html)

生成摘要时出错

---

## 87. Show HN: Stickerbox, a kid-safe, AI-powered voice to sticker printer

**原文标题**: Show HN: Stickerbox, a kid-safe, AI-powered voice to sticker printer

**原文链接**: [https://stickerbox.com/](https://stickerbox.com/)

生成摘要时出错

---

## 88. A Starlink satellite exploded

**原文标题**: A Starlink satellite exploded

**原文链接**: [https://twitter.com/Starlink/status/2001691802911289712](https://twitter.com/Starlink/status/2001691802911289712)

生成摘要时出错

---

## 89. Data Bank – Nuforc – Latest UFO Sightings

**原文标题**: Data Bank – Nuforc – Latest UFO Sightings

**原文链接**: [https://nuforc.org/databank/](https://nuforc.org/databank/)

生成摘要时出错

---

## 90. Gamers Are Overwhelmingly Negative About Gen AI in Video Games

**原文标题**: Gamers Are Overwhelmingly Negative About Gen AI in Video Games

**原文链接**: [https://quanticfoundry.com/2025/12/18/gen-ai/](https://quanticfoundry.com/2025/12/18/gen-ai/)

生成摘要时出错

---

## 91. Devastated PC builder orders DDR5 RAM from Amazon receives DDR2 and some weights

**原文标题**: Devastated PC builder orders DDR5 RAM from Amazon receives DDR2 and some weights

**原文链接**: [https://www.tomshardware.com/pc-components/ddr5/sealed-ddr5-kit-sold-on-amazon-reportedly-contained-ddr2-modules-and-a-fake-weight-plate](https://www.tomshardware.com/pc-components/ddr5/sealed-ddr5-kit-sold-on-amazon-reportedly-contained-ddr2-modules-and-a-fake-weight-plate)

生成摘要时出错

---

## 92. Recursive Project Search in Emacs

**原文标题**: Recursive Project Search in Emacs

**原文链接**: [https://lukeplant.me.uk/blog/posts/recursive-project-search-in-emacs/](https://lukeplant.me.uk/blog/posts/recursive-project-search-in-emacs/)

生成摘要时出错

---

## 93. Unix v4 tape raw binary image recovered

**原文标题**: Unix v4 tape raw binary image recovered

**原文链接**: [https://elk.zone/hachyderm.io/@ricci@discuss.systems/115748594405893972](https://elk.zone/hachyderm.io/@ricci@discuss.systems/115748594405893972)

生成摘要时出错

---

## 94. Pa. high court rules that police can access Google searches without a warrant

**原文标题**: Pa. high court rules that police can access Google searches without a warrant

**原文链接**: [https://therecord.media/google-searches-police-access-without-warrant-pennsylvania-court-ruling](https://therecord.media/google-searches-police-access-without-warrant-pennsylvania-court-ruling)

生成摘要时出错

---

## 95. Show HN: Linggen – A local-first memory layer for your AI (Cursor, Zed, Claude)

**原文标题**: Show HN: Linggen – A local-first memory layer for your AI (Cursor, Zed, Claude)

**原文链接**: [https://github.com/linggen/linggen](https://github.com/linggen/linggen)

生成摘要时出错

---

## 96. Approaching 50 Years of String Theory

**原文标题**: Approaching 50 Years of String Theory

**原文链接**: [https://www.math.columbia.edu/~woit/wordpress/?p=15401](https://www.math.columbia.edu/~woit/wordpress/?p=15401)

生成摘要时出错

---

## 97. Interactive Fluid Typography

**原文标题**: Interactive Fluid Typography

**原文链接**: [https://electricmagicfactory.com/articles/interactive-fluid-typography/](https://electricmagicfactory.com/articles/interactive-fluid-typography/)

生成摘要时出错

---

## 98. The post-GeForce era: What if Nvidia abandons PC gaming?

**原文标题**: The post-GeForce era: What if Nvidia abandons PC gaming?

**原文链接**: [https://www.pcworld.com/article/3013044/the-post-geforce-era-what-if-nvidia-abandons-pc-gaming.html](https://www.pcworld.com/article/3013044/the-post-geforce-era-what-if-nvidia-abandons-pc-gaming.html)

生成摘要时出错

---

## 99. Jeffrey Epstein Court Records

**原文标题**: Jeffrey Epstein Court Records

**原文链接**: [https://www.justice.gov/epstein/court-records](https://www.justice.gov/epstein/court-records)

生成摘要时出错

---

## 100. Man sues cops who jailed him for 37 days for trolling a Charlie Kirk vigil

**原文标题**: Man sues cops who jailed him for 37 days for trolling a Charlie Kirk vigil

**原文链接**: [https://arstechnica.com/tech-policy/2025/12/man-sues-cops-who-jailed-him-for-37-days-for-trolling-a-charlie-kirk-vigil/](https://arstechnica.com/tech-policy/2025/12/man-sues-cops-who-jailed-him-for-37-days-for-trolling-a-charlie-kirk-vigil/)

生成摘要时出错

---

