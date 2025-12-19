# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2025-12-19.md)

*最后自动更新时间: 2025-12-19 19:48:26*
## 1. 从2026年1月起，所有ACM出版物将实现开放获取

**原文标题**: Beginning January 2026, all ACM publications will be made open access

**原文链接**: [https://dl.acm.org/openaccess](https://dl.acm.org/openaccess)

自2026年1月起，美国计算机协会（ACM）出版的所有新学术文章将立即在全球范围内免费开放阅读，并采用开放获取（OA）许可。这一里程碑式的转变标志着ACM向完全开放获取出版商的转型完成，该转型建立在其2020年启动的“ACM开放”模式之上。

根据新政策，在ACM数字图书馆发表的所有研究将默认采用知识共享CC BY 4.0许可发布，从而实现最大程度的重复利用和传播。作者将保留其作品的版权。此举旨在加速科学发现，并使计算研究面向更广泛的全球受众，促进更大的合作和更高的社会影响力。

对于此前订阅ACM数字图书馆的机构，“ACM开放”计划将继续提供过渡协议。这些协议将订阅费转换为年度文章处理费（APC）支付，允许其附属作者在ACM期刊上开放获取出版作品而无需直接付费。未与“ACM开放”机构关联的个人作者将需要支付APC，但ACM将为来自低收入国家的作者提供豁免，并设有支持无资金作者的机制。

这一举措强调了ACM对开放科学和公平获取研究的承诺，巩固了其在学术出版领域的领导地位。

---

## 2. 现在的Hacker News首页，但标题是真实的。

**原文标题**: Hacker News front page now, but the titles are honest

**原文链接**: [https://dosaygo-studio.github.io/hn-front-page-2035/news-honest.html](https://dosaygo-studio.github.io/hn-front-page-2035/news-honest.html)

《Hacker News：诚实版》以讽刺的手法重新解读了典型的科技新闻标题，揭露了行业中普遍存在的潜规则和常见套路。这些重新设计的标题对科技世界的方方面面进行了坦率的评论。

其中涵盖的主题包括对新兴技术（如Rust）和人工智能的强行炒作；企业弊端（亚马逊功能采用迟缓、英特尔的营销、OpenAI的各种“花活”、Ngrok的伪装广告）；以及开发者对既有概念的不断“重塑”（如Rails状态机、拖放功能）。

该列表还触及了社会和政治议题，例如政治家对科技的无知、意外的隐私保护成果以及制裁的影响。开发者们的痛点也得到了强调，如依赖地狱、为个人学习构建小众工具以及通过GitHub星标寻找工作机会。此外，它还讽刺了人工智能训练数据的偏见、其被企业用来转移注意力的方式，以及为促进不必要的消费而制定新标准。实质上，这份汇编对科技创新的周期、企业战略、开发者挑战以及科技论述中潜在的偏见，提供了一种批判性且常常是犬儒主义的审视。

---

## 3. 我们通过供应链攻击攻陷了 X、Vercel、Cursor 和 Discord。

**原文标题**: We pwned X, Vercel, Cursor, and Discord through a supply-chain attack

**原文链接**: [https://gist.github.com/hackermondev/5e2cdc32849405fff6b46957747a2d28](https://gist.github.com/hackermondev/5e2cdc32849405fff6b46957747a2d28)

十六岁的Daniel与朋友xyzeva和MDL一同，发现了一个关键的供应链跨站脚本（XSS）漏洞，该漏洞影响了人工智能文档平台Mintlify。这一发现始于Daniel调查Discord新版开发者文档时，该文档最近已切换到Mintlify。

Daniel发现，由Mintlify支持的网站，即使是像Discord那样使用自定义域名的网站，也暴露了一个内部端点：`/_mintlify/static/[subdomain]/[...route]`。关键在于，这个端点没有验证所请求的`[subdomain]`是否与主机匹配，这使得它能够从任何Mintlify客户的文档中获取静态文件。

随后，Daniel发现他可以将JavaScript嵌入到SVG文件中。通过将这样一个恶意SVG文件上传到他自己的Mintlify文档中，并（例如通过`https://discord.com/_mintlify/_static/hackerone-a00f3c6c/lmao.svg`）通过目标域名上的漏洞端点访问它，他就可以执行任意代码。这种攻击方式允许攻击者向受影响的文档中注入恶意脚本，有可能窃取用户凭据，并通过一个恶意链接实现账户劫持。

该漏洞影响广泛，几乎波及所有Mintlify客户，包括X（Twitter）、Vercel、Cursor和Discord等主要公司，它们都将其文档托管在其主域名上。在负责任的披露之后，Discord暂时关闭了其开发者文档，并恢复使用旧平台。Mintlify的工程团队迅速与研究人员合作，修复了此漏洞及其他相关漏洞。该团队总共获得了约11,000美元的赏金，这突显了此次供应链攻击的严重性和广泛影响。

---

## 4. 你的工作是交付你已证明可运行的代码。

**原文标题**: Your job is to deliver code you have proven to work

**原文链接**: [https://simonwillison.net/2025/Dec/18/code-proven-to-work/](https://simonwillison.net/2025/Dec/18/code-proven-to-work/)

这篇发表于2025年12月18日的文章认为，软件开发者的核心工作是交付经过*验证*能正常工作的代码，而不仅仅是生成代码。它批评了这样一种趋势：工程师，尤其是那些使用AI辅助的工程师，提交大量未经测试的拉取请求，给评审者带来了不公平的负担。

验证代码功能需要两个必不可少的步骤。首先是**手动测试**，即开发者亲自验证代码的行为。这包括设置初始状态、执行代码更改并展示其效果——通常通过共享终端输出或屏幕录制视频来完成。掌握手动测试还包括识别并处理边缘情况。

其次是**自动化测试**，这意味着将代码更改与测试用例一起提交，这些测试用例既能确认功能，又能在实现被回滚时失败。文章强调，AI工具使编写自动化测试变得显著更容易，从而消除了任何省略它们的借口。它还告诫不要仅仅依赖自动化测试而跳过手动验证。

作者将这一原则扩展到AI编码代理，建议开发者教授这些工具来验证它们自己的更改。代理可以执行“手动”检查（例如，运行CLI命令，为UI更改截取屏幕截图），并且擅长生成自动化测试，尤其是在有良好结构化现有测试套件的指导下。

最终，人类开发者对交付经过验证的代码负有责任。价值不在于仅仅向大型语言模型（LLM）发出代码提示，而在于贡献附带明确证据表明其按预期工作的代码。文章敦促开发者始终在他们的拉取请求中包含这些证明。

---

## 5. 历史大语言模型：仅基于1913年以前文本训练的模型

**原文标题**: History LLMs: Models trained exclusively on pre-1913 texts

**原文链接**: [https://github.com/DGoettlich/history-llms](https://github.com/DGoettlich/history-llms)

苏黎世大学和科隆大学的研究人员正在开发“历史大语言模型”（History LLMs），这是一系列大型语言模型，专门利用截至特定“知识截止日期”（例如1913年、1929年、1933年、1939年、1946年）的带时间戳历史数据进行训练。其目标是为人文科学、社会科学和计算机科学研究创建“通往过去的窗口”。

这些模型的一个核心特点是它们“完全时间锁定”，不包含任何超出其截止日期的信息。这避免了现代LLM（如GPT-5）中常见的“后见之明污染”，因为后者“知道”未来的事件。历史LLM真实地体现了其时代的文本文化，使研究人员能够在没有现代干扰的情况下，探索特定时刻什么是可思、可预测或可说的。

即将推出的“兰克-4B”系列，基于通义千问3架构，将利用从一个精选的6000亿token历史数据集中提取的800亿个token进行训练。例如，“兰克-4B-1913”模型仅用1913年之前的文本训练，它提供了一个错误的阿道夫·希特勒传记（1913年时希特勒尚不为人知），很好地说明了这一点。尽管它谴责奴隶制，但其对女性就业或同性恋的回复反映了20世纪初普遍存在的偏见和规范（例如，偏爱男性就业，对男同性恋者持厌恶态度或视为疾病）。

这些模型是海量文本语料库的压缩表示，有助于探索话语模式。它们并非公众舆论的完美反映，而是反映了已发布的文本。该项目承认模型会重现训练数据中存在的历史偏见（种族主义、厌女症），并认为这是理解过去的一个关键特征。所有研究成果都将公开发布，并为研究人员提供负责任的访问框架。

---

## 6. 古典雕塑并非被涂得很糟糕

**原文标题**: Classical statues were not painted horribly

**原文链接**: [https://worksinprogress.co/issue/were-classical-statues-painted-horribly/](https://worksinprogress.co/issue/were-classical-statues-painted-horribly/)

古希腊罗马雕塑如今以其未上色形式的美感而广受赞赏，但它们最初是彩色的。现代的复原作品，例如“众神之彩”展览中的那些，旨在展示它们最初的样子，但通常被认为是艳俗和丑陋的。

对于这种丑陋，常见的解释是古代品味与现代品味截然不同，而我们因历史偶然成了“厌色症”患者——但这一说法受到作者的质疑。古代对雕像的描绘，如庞贝壁画所示，表明它们是以细腻微妙的色彩精心绘制的，而非现代复原作品那种哑光、高饱和度的色调。其他古代艺术形式，如壁画、马赛克和室内设计，也展现了敏感且常是自然主义的色彩运用，在现代人眼中也具有美感。此外，其他文化（如埃及、尼泊尔、中世纪）的彩绘雕塑，通常并未被普遍认为丑陋。

作者提出，这些复原作品之所以显得丑陋，仅仅是因为它们“拙劣的涂绘”。它们基于有限的考古证据（仅有代表底层的微量颜料），且常省略了原作的精细上层涂料和艺术技巧。专家们自己也承认这些并非精确的复制。这一“拙劣涂绘理论”表明，古希腊和罗马人可能也会不喜欢这些粗糙的复原作品，因为他们实际的色彩运用可能更为微妙和精致。

这些“丑陋”复原作品的可能原因包括复原者缺乏艺术技巧，严格的文物保护准则（仅限于包含有直接证据的特征），甚至可能是刻意采用其醒目但刺眼的外观来吸引公众兴趣的策略，从而导致公众对古典彩绘艺术的误解。

---

## 7. 我被黑了：我的Hetzner服务器开始挖门罗币

**原文标题**: I got hacked: My Hetzner server started mining Monero

**原文链接**: [https://blog.jakesaunders.dev/my-server-started-mining-monero-this-morning/](https://blog.jakesaunders.dev/my-server-started-mining-monero-this-morning/)

杰克·桑德斯 (Jake Saunders) 发现他的 Hetzner 服务器被黑客入侵并用于挖掘门罗币，此事是通过一份 Hetzner 滥用报告揭露的。由于 `javae` 和 `xmrig`（门罗币挖矿程序）进程，他的 CPU 负载飙升。罪魁祸首是一个被攻破的 Umami 分析容器，它利用了 Next.js 中的一个关键 RCE（远程代码执行）漏洞 CVE-2025-66478——而 Jake 之前并不知道 Umami 使用了 Next.js 这个依赖项。

最初，Jake 因进程列表的存在而担心整个主机已被攻陷，但他的调查发现恶意软件并*未*逃逸出容器。关键在于强大的 Docker 隔离机制：Umami 容器以非 root 用户 (`nextjs`) 运行，是非特权的，并且没有卷挂载。这将恶意活动（门罗币挖矿和网络扫描）完全限制在容器内部，从而阻止了主机持久化或更广泛的系统访问。

杰克通过停止并移除受损容器解决了问题，使 CPU 恢复正常，并实施了防火墙 (UFW)。吸取的教训包括：务必了解你的依赖项，容器隔离在安全配置（非 root 用户、非特权）下是有效的，以及纵深防御至关重要。他承认自己很幸运，因为良好的容器实践使他避免了更糟糕的情况。

---

## 8. Please just try HTMX

**原文标题**: Please just try HTMX

**原文链接**: [http://pleasejusttryhtmx.com/](http://pleasejusttryhtmx.com/)

生成摘要时出错

---

## 9. GPT-5.2-Codex

**原文标题**: GPT-5.2-Codex

**原文链接**: [https://openai.com/index/introducing-gpt-5-2-codex/](https://openai.com/index/introducing-gpt-5-2-codex/)

Unable to access the article link.

---

## 10. 1.5 TB of VRAM on Mac Studio – RDMA over Thunderbolt 5

**原文标题**: 1.5 TB of VRAM on Mac Studio – RDMA over Thunderbolt 5

**原文链接**: [https://www.jeffgeerling.com/blog/2025/15-tb-vram-on-mac-studio-rdma-over-thunderbolt-5](https://www.jeffgeerling.com/blog/2025/15-tb-vram-on-mac-studio-rdma-over-thunderbolt-5)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 2 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 3 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 4 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 5 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 6 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 7 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 8 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 9 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 10 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 11 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 12 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 13 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 14 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 15 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 16 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 17 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 18 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 19 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 20 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 21 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 22 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 23 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 24 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 25 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 26 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 27 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 28 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 29 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 30 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 31 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 32 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 33 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 34 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 35 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 36 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 37 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 38 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 39 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 40 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 41 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 42 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 43 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
| 44 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
