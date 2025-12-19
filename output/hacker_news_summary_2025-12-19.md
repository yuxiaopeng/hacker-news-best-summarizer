# Hacker News 热门文章摘要 (2025-12-19)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

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

## 11. Are Apple gift cards safe to redeem?

**原文标题**: Are Apple gift cards safe to redeem?

**原文链接**: [https://daringfireball.net/linked/2025/12/17/are-apple-gift-cards-safe-to-redeem](https://daringfireball.net/linked/2025/12/17/are-apple-gift-cards-safe-to-redeem)

生成摘要时出错

---

## 12. Firefox will have an option to disable all AI features

**原文标题**: Firefox will have an option to disable all AI features

**原文链接**: [https://mastodon.social/@firefoxwebdevs/115740500373677782](https://mastodon.social/@firefoxwebdevs/115740500373677782)

生成摘要时出错

---

## 13. Gut bacteria from amphibians and reptiles achieve tumor elimination in mice

**原文标题**: Gut bacteria from amphibians and reptiles achieve tumor elimination in mice

**原文链接**: [https://www.jaist.ac.jp/english/whatsnew/press/2025/12/17-1.html](https://www.jaist.ac.jp/english/whatsnew/press/2025/12/17-1.html)

生成摘要时出错

---

## 14. How China built its ‘Manhattan Project’ to rival the West in AI chips

**原文标题**: How China built its ‘Manhattan Project’ to rival the West in AI chips

**原文链接**: [https://www.japantimes.co.jp/business/2025/12/18/tech/china-west-ai-chips/](https://www.japantimes.co.jp/business/2025/12/18/tech/china-west-ai-chips/)

生成摘要时出错

---

## 15. GotaTun -- Mullvad's WireGuard Implementation in Rust

**原文标题**: GotaTun -- Mullvad's WireGuard Implementation in Rust

**原文链接**: [https://mullvad.net/en/blog/announcing-gotatun-the-future-of-wireguard-at-mullvad-vpn](https://mullvad.net/en/blog/announcing-gotatun-the-future-of-wireguard-at-mullvad-vpn)

生成摘要时出错

---

## 16. Independent review of UK national security law warns of overreach

**原文标题**: Independent review of UK national security law warns of overreach

**原文链接**: [https://www.techradar.com/vpn/vpn-privacy-security/creating-apps-like-signal-or-whatsapp-could-be-hostile-activity-claims-uk-watchdog](https://www.techradar.com/vpn/vpn-privacy-security/creating-apps-like-signal-or-whatsapp-could-be-hostile-activity-claims-uk-watchdog)

生成摘要时出错

---

## 17. Noclip.website – A digital museum of video game levels

**原文标题**: Noclip.website – A digital museum of video game levels

**原文链接**: [https://noclip.website/](https://noclip.website/)

生成摘要时出错

---

## 18. Amazon will allow ePub and PDF downloads for DRM-free eBooks

**原文标题**: Amazon will allow ePub and PDF downloads for DRM-free eBooks

**原文链接**: [https://www.kdpcommunity.com/s/article/New-eBook-Download-Options-for-Readers-Coming-in-2026?language=en_US](https://www.kdpcommunity.com/s/article/New-eBook-Download-Options-for-Readers-Coming-in-2026?language=en_US)

生成摘要时出错

---

## 19. After ruining a treasured water resource, Iran is drying up

**原文标题**: After ruining a treasured water resource, Iran is drying up

**原文链接**: [https://e360.yale.edu/features/iran-water-drought-dams-qanats](https://e360.yale.edu/features/iran-water-drought-dams-qanats)

生成摘要时出错

---

## 20. OBS Studio Gets a New Renderer

**原文标题**: OBS Studio Gets a New Renderer

**原文链接**: [https://obsproject.com/blog/obs-studio-gets-a-new-renderer](https://obsproject.com/blog/obs-studio-gets-a-new-renderer)

生成摘要时出错

---

## 21. Skills for organizations, partners, the ecosystem

**原文标题**: Skills for organizations, partners, the ecosystem

**原文链接**: [https://claude.com/blog/organization-skills-and-directory](https://claude.com/blog/organization-skills-and-directory)

生成摘要时出错

---

## 22. Garage – An S3 object store so reliable you can run it outside datacenters

**原文标题**: Garage – An S3 object store so reliable you can run it outside datacenters

**原文链接**: [https://garagehq.deuxfleurs.fr/](https://garagehq.deuxfleurs.fr/)

生成摘要时出错

---

## 23. Slowness is a virtue

**原文标题**: Slowness is a virtue

**原文链接**: [https://blog.jakobschwichtenberg.com/p/slowness-is-a-virtue](https://blog.jakobschwichtenberg.com/p/slowness-is-a-virtue)

生成摘要时出错

---

## 24. Getting bitten by Intel's poor naming schemes

**原文标题**: Getting bitten by Intel's poor naming schemes

**原文链接**: [https://lorendb.dev/posts/getting-bitten-by-poor-naming-schemes/](https://lorendb.dev/posts/getting-bitten-by-poor-naming-schemes/)

生成摘要时出错

---

## 25. 2026 Apple introducing more ads to increase opportunity in search results

**原文标题**: 2026 Apple introducing more ads to increase opportunity in search results

**原文链接**: [https://ads.apple.com/app-store/help/ad-placements/0082-search-results](https://ads.apple.com/app-store/help/ad-placements/0082-search-results)

生成摘要时出错

---

## 26. How getting richer made teenagers less free

**原文标题**: How getting richer made teenagers less free

**原文链接**: [https://www.theargumentmag.com/p/how-getting-richer-made-teenagers](https://www.theargumentmag.com/p/how-getting-richer-made-teenagers)

生成摘要时出错

---

## 27. TikTok Deal Is the Shittiest Possible Outcome, Making Everything Worse

**原文标题**: TikTok Deal Is the Shittiest Possible Outcome, Making Everything Worse

**原文链接**: [https://www.techdirt.com/2025/12/19/tiktok-deal-done-and-its-somehow-the-shittiest-possible-outcome-making-everything-worse/](https://www.techdirt.com/2025/12/19/tiktok-deal-done-and-its-somehow-the-shittiest-possible-outcome-making-everything-worse/)

生成摘要时出错

---

## 28. TikTok unlawfully tracks shopping habits and use of dating apps?

**原文标题**: TikTok unlawfully tracks shopping habits and use of dating apps?

**原文链接**: [https://noyb.eu/en/tiktok-unlawfully-tracks-your-shopping-habits-and-your-use-dating-apps](https://noyb.eu/en/tiktok-unlawfully-tracks-your-shopping-habits-and-your-use-dating-apps)

生成摘要时出错

---

## 29. FunctionGemma 270M Model

**原文标题**: FunctionGemma 270M Model

**原文链接**: [https://blog.google/technology/developers/functiongemma/](https://blog.google/technology/developers/functiongemma/)

生成摘要时出错

---

## 30. Germany: Amazon is not allowed to force customers to watch ads on Prime Video

**原文标题**: Germany: Amazon is not allowed to force customers to watch ads on Prime Video

**原文链接**: [https://www.zeit.de/wirtschaft/2025-12/amazon-urteil-video-kunden-werbung](https://www.zeit.de/wirtschaft/2025-12/amazon-urteil-video-kunden-werbung)

生成摘要时出错

---

## 31. AI helps ship faster but it produces 1.7× more bugs

**原文标题**: AI helps ship faster but it produces 1.7× more bugs

**原文链接**: [https://www.coderabbit.ai/blog/state-of-ai-vs-human-code-generation-report](https://www.coderabbit.ai/blog/state-of-ai-vs-human-code-generation-report)

生成摘要时出错

---

## 32. 'Ghost jobs' are on the rise – and so are calls to ban them

**原文标题**: 'Ghost jobs' are on the rise – and so are calls to ban them

**原文链接**: [https://www.bbc.com/news/articles/clyzvpp8g3vo](https://www.bbc.com/news/articles/clyzvpp8g3vo)

生成摘要时出错

---

## 33. Judge hints Vizio TV buyers may have rights to source code licensed under GPL

**原文标题**: Judge hints Vizio TV buyers may have rights to source code licensed under GPL

**原文链接**: [https://www.theregister.com/2025/12/05/vizio_gpl_source_code_ruling/](https://www.theregister.com/2025/12/05/vizio_gpl_source_code_ruling/)

生成摘要时出错

---

## 34. Developers can now submit apps to ChatGPT

**原文标题**: Developers can now submit apps to ChatGPT

**原文链接**: [https://openai.com/index/developers-can-now-submit-apps-to-chatgpt/](https://openai.com/index/developers-can-now-submit-apps-to-chatgpt/)

生成摘要时出错

---

## 35. Show HN: Hacker News, but every headline is hysterical clickbait

**原文标题**: Show HN: Hacker News, but every headline is hysterical clickbait

**原文链接**: [https://dosaygo-studio.github.io/hn-front-page-2035/news-max.html](https://dosaygo-studio.github.io/hn-front-page-2035/news-max.html)

生成摘要时出错

---

## 36. Using TypeScript to obtain one of the rarest license plates

**原文标题**: Using TypeScript to obtain one of the rarest license plates

**原文链接**: [https://www.jack.bio/blog/licenseplate](https://www.jack.bio/blog/licenseplate)

生成摘要时出错

---

## 37. Great ideas in theoretical computer science

**原文标题**: Great ideas in theoretical computer science

**原文链接**: [https://www.cs251.com/](https://www.cs251.com/)

生成摘要时出错

---

## 38. How to hack Discord, Vercel and more with one easy trick

**原文标题**: How to hack Discord, Vercel and more with one easy trick

**原文链接**: [https://kibty.town/blog/mintlify/](https://kibty.town/blog/mintlify/)

生成摘要时出错

---

## 39. Egyptian Hieroglyphs: Lesson 1

**原文标题**: Egyptian Hieroglyphs: Lesson 1

**原文链接**: [https://www.egyptianhieroglyphs.net/egyptian-hieroglyphs/lesson-1/](https://www.egyptianhieroglyphs.net/egyptian-hieroglyphs/lesson-1/)

生成摘要时出错

---

## 40. Pornhub extorted after hackers steal Premium member activity data

**原文标题**: Pornhub extorted after hackers steal Premium member activity data

**原文链接**: [https://www.bleepingcomputer.com/news/security/pornhub-extorted-after-hackers-steal-premium-member-activity-data/](https://www.bleepingcomputer.com/news/security/pornhub-extorted-after-hackers-steal-premium-member-activity-data/)

生成摘要时出错

---

## 41. Cursor Acquires Graphite

**原文标题**: Cursor Acquires Graphite

**原文链接**: [https://graphite.com/blog/graphite-joins-cursor](https://graphite.com/blog/graphite-joins-cursor)

生成摘要时出错

---

## 42. GitHub postponing the announced billing change for self-hosted GitHub Actions

**原文标题**: GitHub postponing the announced billing change for self-hosted GitHub Actions

**原文链接**: [https://twitter.com/jaredpalmer/status/2001373329811181846](https://twitter.com/jaredpalmer/status/2001373329811181846)

生成摘要时出错

---

## 43. How did IRC ping timeouts end up in a lawsuit?

**原文标题**: How did IRC ping timeouts end up in a lawsuit?

**原文链接**: [https://mjg59.dreamwidth.org/73777.html](https://mjg59.dreamwidth.org/73777.html)

生成摘要时出错

---

## 44. AI vending machine was tricked into giving away everything

**原文标题**: AI vending machine was tricked into giving away everything

**原文链接**: [https://kottke.org/25/12/this-ai-vending-machine-was-tricked-into-giving-away-everything](https://kottke.org/25/12/this-ai-vending-machine-was-tricked-into-giving-away-everything)

生成摘要时出错

---

## 45. T5Gemma 2: The next generation of encoder-decoder models

**原文标题**: T5Gemma 2: The next generation of encoder-decoder models

**原文链接**: [https://blog.google/technology/developers/t5gemma-2/](https://blog.google/technology/developers/t5gemma-2/)

生成摘要时出错

---

## 46. Reconstructed Commander Keen 1-3 Source Code

**原文标题**: Reconstructed Commander Keen 1-3 Source Code

**原文链接**: [https://pckf.com/viewtopic.php?t=18248](https://pckf.com/viewtopic.php?t=18248)

生成摘要时出错

---

## 47. Most parked domains now serving malicious content

**原文标题**: Most parked domains now serving malicious content

**原文链接**: [https://krebsonsecurity.com/2025/12/most-parked-domains-now-serving-malicious-content/](https://krebsonsecurity.com/2025/12/most-parked-domains-now-serving-malicious-content/)

生成摘要时出错

---

## 48. The Scottish Highlands, the Appalachians, Atlas are the same mountain range

**原文标题**: The Scottish Highlands, the Appalachians, Atlas are the same mountain range

**原文链接**: [https://vividmaps.com/central-pangean-mountains/](https://vividmaps.com/central-pangean-mountains/)

生成摘要时出错

---

## 49. GitHub Actions for self-hosted runners price increase postponed

**原文标题**: GitHub Actions for self-hosted runners price increase postponed

**原文链接**: [https://pricetimeline.com/news/189](https://pricetimeline.com/news/189)

生成摘要时出错

---

## 50. What is an elliptic curve? (2019)

**原文标题**: What is an elliptic curve? (2019)

**原文链接**: [https://www.johndcook.com/blog/2019/02/21/what-is-an-elliptic-curve/](https://www.johndcook.com/blog/2019/02/21/what-is-an-elliptic-curve/)

生成摘要时出错

---

## 51. Valve is running Apple's playbook in reverse

**原文标题**: Valve is running Apple's playbook in reverse

**原文链接**: [https://www.garbagecollected.dev/p/valve-the-reverse-apple](https://www.garbagecollected.dev/p/valve-the-reverse-apple)

生成摘要时出错

---

## 52. RCE via ND6 Router Advertisements in FreeBSD

**原文标题**: RCE via ND6 Router Advertisements in FreeBSD

**原文链接**: [https://www.freebsd.org/security/advisories/FreeBSD-SA-25:12.rtsold.asc](https://www.freebsd.org/security/advisories/FreeBSD-SA-25:12.rtsold.asc)

生成摘要时出错

---

## 53. Two kinds of vibe coding

**原文标题**: Two kinds of vibe coding

**原文链接**: [https://davidbau.com/archives/2025/12/16/vibe_coding.html](https://davidbau.com/archives/2025/12/16/vibe_coding.html)

生成摘要时出错

---

## 54. Spain fines Airbnb €65M: Why the government is cracking down on illegal rentals

**原文标题**: Spain fines Airbnb €65M: Why the government is cracking down on illegal rentals

**原文链接**: [https://www.euronews.com/travel/2025/12/15/spain-fines-airbnb-65-million-why-the-government-is-cracking-down-on-illegal-rentals](https://www.euronews.com/travel/2025/12/15/spain-fines-airbnb-65-million-why-the-government-is-cracking-down-on-illegal-rentals)

生成摘要时出错

---

## 55. Why do commercial spaces sit vacant?

**原文标题**: Why do commercial spaces sit vacant?

**原文链接**: [https://archive.strongtowns.org/journal/2025/5/21/why-do-commercial-spaces-sit-vacant](https://archive.strongtowns.org/journal/2025/5/21/why-do-commercial-spaces-sit-vacant)

生成摘要时出错

---

## 56. Cloudflare Radar 2025 Year in Review

**原文标题**: Cloudflare Radar 2025 Year in Review

**原文链接**: [https://radar.cloudflare.com/year-in-review/2025](https://radar.cloudflare.com/year-in-review/2025)

生成摘要时出错

---

## 57. We Let AI Run Our Office Vending Machine. It Lost Hundreds of Dollars

**原文标题**: We Let AI Run Our Office Vending Machine. It Lost Hundreds of Dollars

**原文链接**: [https://www.wsj.com/tech/ai/anthropic-claude-ai-vending-machine-agent-b7e84e34](https://www.wsj.com/tech/ai/anthropic-claude-ai-vending-machine-agent-b7e84e34)

生成摘要时出错

---

## 58. It's all about momentum

**原文标题**: It's all about momentum

**原文链接**: [https://combo.cc/posts/its-all-about-momentum-innit/](https://combo.cc/posts/its-all-about-momentum-innit/)

生成摘要时出错

---

## 59. Inside PostHog: SSRF, ClickHouse SQL Escape and Default Postgres Creds to RCE

**原文标题**: Inside PostHog: SSRF, ClickHouse SQL Escape and Default Postgres Creds to RCE

**原文链接**: [https://mdisec.com/inside-posthog-how-ssrf-a-clickhouse-sql-escaping-0day-and-default-postgresql-credentials-formed-an-rce-chain-zdi-25-099-zdi-25-097-zdi-25-096/](https://mdisec.com/inside-posthog-how-ssrf-a-clickhouse-sql-escaping-0day-and-default-postgresql-credentials-formed-an-rce-chain-zdi-25-099-zdi-25-097-zdi-25-096/)

生成摘要时出错

---

## 60. Virtualizing Nvidia HGX B200 GPUs with Open Source

**原文标题**: Virtualizing Nvidia HGX B200 GPUs with Open Source

**原文链接**: [https://www.ubicloud.com/blog/virtualizing-nvidia-hgx-b200-gpus-with-open-source](https://www.ubicloud.com/blog/virtualizing-nvidia-hgx-b200-gpus-with-open-source)

生成摘要时出错

---

## 61. Making Google Sans Flex

**原文标题**: Making Google Sans Flex

**原文链接**: [https://design.google/library/google-sans-flex-font](https://design.google/library/google-sans-flex-font)

生成摘要时出错

---

## 62. American Academy of Pediatrics loses HHS funding after criticizing RFK Jr.

**原文标题**: American Academy of Pediatrics loses HHS funding after criticizing RFK Jr.

**原文链接**: [https://www.washingtonpost.com/health/2025/12/17/aap-hhs-funding-rfk/](https://www.washingtonpost.com/health/2025/12/17/aap-hhs-funding-rfk/)

生成摘要时出错

---

## 63. AI Isn't Just Spying on You. It's Tricking You into Spending More

**原文标题**: AI Isn't Just Spying on You. It's Tricking You into Spending More

**原文链接**: [https://newrepublic.com/article/204525/artificial-intelligence-consumers-data-dynamic-pricing](https://newrepublic.com/article/204525/artificial-intelligence-consumers-data-dynamic-pricing)

生成摘要时出错

---

## 64. A school locked down after AI flagged a gun. It was a clarinet

**原文标题**: A school locked down after AI flagged a gun. It was a clarinet

**原文链接**: [https://www.washingtonpost.com/nation/2025/12/17/ai-gun-school-detection/](https://www.washingtonpost.com/nation/2025/12/17/ai-gun-school-detection/)

生成摘要时出错

---

## 65. The FreeBSD Foundation's Laptop Support and Usability Project

**原文标题**: The FreeBSD Foundation's Laptop Support and Usability Project

**原文链接**: [https://github.com/FreeBSDFoundation/proj-laptop](https://github.com/FreeBSDFoundation/proj-laptop)

生成摘要时出错

---

## 66. Show HN: High-Performance Wavelet Matrix for Python, Implemented in Rust

**原文标题**: Show HN: High-Performance Wavelet Matrix for Python, Implemented in Rust

**原文链接**: [https://pypi.org/project/wavelet-matrix/](https://pypi.org/project/wavelet-matrix/)

生成摘要时出错

---

## 67. Here is the 15 sec coding test I used to instantly filter out most applicants

**原文标题**: Here is the 15 sec coding test I used to instantly filter out most applicants

**原文链接**: [https://josezarazua.com/im-a-former-cto-here-is-the-15-sec-coding-test-i-used-to-instantly-filter-out-50-of-unqualified-applicants/](https://josezarazua.com/im-a-former-cto-here-is-the-15-sec-coding-test-i-used-to-instantly-filter-out-50-of-unqualified-applicants/)

生成摘要时出错

---

## 68. The most banned books in U.S. schools

**原文标题**: The most banned books in U.S. schools

**原文链接**: [https://pen.org/top-52-banned-books-since-2021/](https://pen.org/top-52-banned-books-since-2021/)

生成摘要时出错

---

## 69. Prepare for That Stupid World

**原文标题**: Prepare for That Stupid World

**原文链接**: [https://ploum.net/2025-12-19-prepare-for-that-world.html](https://ploum.net/2025-12-19-prepare-for-that-world.html)

生成摘要时出错

---

## 70. Systemd v259

**原文标题**: Systemd v259

**原文链接**: [https://github.com/systemd/systemd/releases/tag/v259](https://github.com/systemd/systemd/releases/tag/v259)

生成摘要时出错

---

## 71. Using AI Generated Code Will Make You a Bad Programmer

**原文标题**: Using AI Generated Code Will Make You a Bad Programmer

**原文链接**: [https://unsolicited-opinions.rudism.com/bad-programmer/](https://unsolicited-opinions.rudism.com/bad-programmer/)

生成摘要时出错

---

## 72. VRChat: “There are more Japanese creators than all other countries combined”

**原文标题**: VRChat: “There are more Japanese creators than all other countries combined”

**原文链接**: [https://twitter.com/chyadosensei/status/2001356290531156159](https://twitter.com/chyadosensei/status/2001356290531156159)

生成摘要时出错

---

## 73. AMD officially confirms fresh next-gen Zen 6 CPU details

**原文标题**: AMD officially confirms fresh next-gen Zen 6 CPU details

**原文链接**: [https://overclock3d.net/news/cpu_mainboard/amd-officially-confirms-fresh-next-gen-zen-6-cpu-details/](https://overclock3d.net/news/cpu_mainboard/amd-officially-confirms-fresh-next-gen-zen-6-cpu-details/)

生成摘要时出错

---

## 74. I have to give Fortnite my passport to use Bluesky

**原文标题**: I have to give Fortnite my passport to use Bluesky

**原文链接**: [https://spitfirenews.com/p/why-i-have-to-give-fortnite-my-passport-to-use-bluesky](https://spitfirenews.com/p/why-i-have-to-give-fortnite-my-passport-to-use-bluesky)

生成摘要时出错

---

## 75. Venezuela's Navy Begins Escorting Ships as U.S. Threatens Blockade

**原文标题**: Venezuela's Navy Begins Escorting Ships as U.S. Threatens Blockade

**原文链接**: [https://www.nytimes.com/live/2025/12/17/us/trump-news](https://www.nytimes.com/live/2025/12/17/us/trump-news)

生成摘要时出错

---

## 76. North Korean infiltrator caught at Amazon due to 110ms keystroke lag

**原文标题**: North Korean infiltrator caught at Amazon due to 110ms keystroke lag

**原文链接**: [https://www.tomshardware.com/tech-industry/cyber-security/north-korean-infiltrator-caught-working-in-amazon-it-department-thanks-to-lag-110ms-keystroke-input-raises-red-flags-over-true-location](https://www.tomshardware.com/tech-industry/cyber-security/north-korean-infiltrator-caught-working-in-amazon-it-department-thanks-to-lag-110ms-keystroke-input-raises-red-flags-over-true-location)

生成摘要时出错

---

## 77. Graphite Is Joining Cursor

**原文标题**: Graphite Is Joining Cursor

**原文链接**: [https://cursor.com/blog/graphite](https://cursor.com/blog/graphite)

生成摘要时出错

---

## 78. Show HN: I open-sourced my Go and Next B2B SaaS Starter (deploy anywhere, MIT)

**原文标题**: Show HN: I open-sourced my Go and Next B2B SaaS Starter (deploy anywhere, MIT)

**原文链接**: [https://github.com/moasq/production-saas-starter](https://github.com/moasq/production-saas-starter)

生成摘要时出错

---

## 79. Heart and Kidney Diseases and Type 2 Diabetes May Be One Ailment

**原文标题**: Heart and Kidney Diseases and Type 2 Diabetes May Be One Ailment

**原文链接**: [https://www.scientificamerican.com/article/heart-and-kidney-diseases-plus-type-2-diabetes-may-be-one-illness-treatable/](https://www.scientificamerican.com/article/heart-and-kidney-diseases-plus-type-2-diabetes-may-be-one-illness-treatable/)

生成摘要时出错

---

## 80. Show HN: Composify – Open-Source Visual Editor / Server-Driven UI for React

**原文标题**: Show HN: Composify – Open-Source Visual Editor / Server-Driven UI for React

**原文链接**: [https://github.com/composify-js/composify](https://github.com/composify-js/composify)

生成摘要时出错

---

## 81. Explaining the widening divides in us midlife mortality: Is there a smoking gun?

**原文标题**: Explaining the widening divides in us midlife mortality: Is there a smoking gun?

**原文链接**: [https://www.nber.org/papers/w34553](https://www.nber.org/papers/w34553)

生成摘要时出错

---

## 82. Engineers who dismiss AI

**原文标题**: Engineers who dismiss AI

**原文链接**: [https://terriblesoftware.org/2025/12/19/the-strange-case-of-engineers-who-dismiss-ai/](https://terriblesoftware.org/2025/12/19/the-strange-case-of-engineers-who-dismiss-ai/)

生成摘要时出错

---

## 83. Military standard on software control levels

**原文标题**: Military standard on software control levels

**原文链接**: [https://entropicthoughts.com/mil-std-882e-software-control](https://entropicthoughts.com/mil-std-882e-software-control)

生成摘要时出错

---

## 84. The immortality of Microsoft Word

**原文标题**: The immortality of Microsoft Word

**原文链接**: [https://theredline.versionstory.com/p/on-the-immortality-of-microsoft-word](https://theredline.versionstory.com/p/on-the-immortality-of-microsoft-word)

生成摘要时出错

---

## 85. More than half of researchers now use AI for peer review, often against guidance

**原文标题**: More than half of researchers now use AI for peer review, often against guidance

**原文链接**: [https://www.nature.com/articles/d41586-025-04066-5](https://www.nature.com/articles/d41586-025-04066-5)

生成摘要时出错

---

## 86. The US govt has revoked the non-immigrant visa of Nobel laureate Wole Soyinka [video]

**原文标题**: The US govt has revoked the non-immigrant visa of Nobel laureate Wole Soyinka [video]

**原文链接**: [https://www.youtube.com/watch?v=ple4xophXfM](https://www.youtube.com/watch?v=ple4xophXfM)

生成摘要时出错

---

## 87. SMB Direct – SMB3 over RDMA

**原文标题**: SMB Direct – SMB3 over RDMA

**原文链接**: [https://docs.kernel.org/filesystems/smb/smbdirect.html](https://docs.kernel.org/filesystems/smb/smbdirect.html)

生成摘要时出错

---

## 88. Property-Based Testing Caught a Security Bug I Never Would Have Found

**原文标题**: Property-Based Testing Caught a Security Bug I Never Would Have Found

**原文链接**: [https://kiro.dev/blog/property-based-testing-fixed-security-bug/](https://kiro.dev/blog/property-based-testing-fixed-security-bug/)

生成摘要时出错

---

## 89. Mozilla's New CEO Confirms Firefox Will Become an "AI Browser"

**原文标题**: Mozilla's New CEO Confirms Firefox Will Become an "AI Browser"

**原文链接**: [https://www.omgubuntu.co.uk/2025/12/mozilla-new-ceo-firefox-ai-browser-strategy](https://www.omgubuntu.co.uk/2025/12/mozilla-new-ceo-firefox-ai-browser-strategy)

生成摘要时出错

---

## 90. America's Dirtiest Carbon Polluters, Mapped to Ridiculous Precision

**原文标题**: America's Dirtiest Carbon Polluters, Mapped to Ridiculous Precision

**原文链接**: [https://gizmodo.com/americas-dirtiest-carbon-polluters-mapped-to-ridiculous-precision-2000700924](https://gizmodo.com/americas-dirtiest-carbon-polluters-mapped-to-ridiculous-precision-2000700924)

生成摘要时出错

---

## 91. Believe the Checkbook

**原文标题**: Believe the Checkbook

**原文链接**: [https://robertgreiner.com/believe-the-checkbook/](https://robertgreiner.com/believe-the-checkbook/)

生成摘要时出错

---

## 92. A proposed amendment to ban under 16s in the UK from common online services

**原文标题**: A proposed amendment to ban under 16s in the UK from common online services

**原文链接**: [https://decoded.legal/blog/2025/12/a-proposed-legislative-amendment-to-attempt-to-ban-under-16s-in-the-uk-from-common-messaging-services-sharing-family-photos-using-wikipedia-and-doing-much-else-online-by-imposing-age-assurance-on-everyone/](https://decoded.legal/blog/2025/12/a-proposed-legislative-amendment-to-attempt-to-ban-under-16s-in-the-uk-from-common-messaging-services-sharing-family-photos-using-wikipedia-and-doing-much-else-online-by-imposing-age-assurance-on-everyone/)

生成摘要时出错

---

## 93. TP-Link Tapo C200: Hardcoded Keys, Buffer Overflows and Privacy

**原文标题**: TP-Link Tapo C200: Hardcoded Keys, Buffer Overflows and Privacy

**原文链接**: [https://www.evilsocket.net/2025/12/18/TP-Link-Tapo-C200-Hardcoded-Keys-Buffer-Overflows-and-Privacy-in-the-Era-of-AI-Assisted-Reverse-Engineering/](https://www.evilsocket.net/2025/12/18/TP-Link-Tapo-C200-Hardcoded-Keys-Buffer-Overflows-and-Privacy-in-the-Era-of-AI-Assisted-Reverse-Engineering/)

生成摘要时出错

---

## 94. Online Textbook for Braid groups and knots and tangles

**原文标题**: Online Textbook for Braid groups and knots and tangles

**原文链接**: [https://matthematics.com/redoak/redoak.html](https://matthematics.com/redoak/redoak.html)

生成摘要时出错

---

## 95. The Mysterious Forces Steering Views on Hacker News

**原文标题**: The Mysterious Forces Steering Views on Hacker News

**原文链接**: [https://xn--gckvb8fzb.com/the-mysterious-forces-steering-views-on-hacker-news/](https://xn--gckvb8fzb.com/the-mysterious-forces-steering-views-on-hacker-news/)

生成摘要时出错

---

## 96. Oliver Sacks put himself into his case studies – what was the cost?

**原文标题**: Oliver Sacks put himself into his case studies – what was the cost?

**原文链接**: [https://www.newyorker.com/magazine/2025/12/15/oliver-sacks-put-himself-into-his-case-studies-what-was-the-cost](https://www.newyorker.com/magazine/2025/12/15/oliver-sacks-put-himself-into-his-case-studies-what-was-the-cost)

生成摘要时出错

---

## 97. A Starlink Satellite Exploded

**原文标题**: A Starlink Satellite Exploded

**原文链接**: [https://twitter.com/Starlink/status/2001691802911289712](https://twitter.com/Starlink/status/2001691802911289712)

生成摘要时出错

---

## 98. Make Me CEO of Mozilla

**原文标题**: Make Me CEO of Mozilla

**原文链接**: [https://blog.kingcons.io/posts/make-me-ceo-of-mozilla.html](https://blog.kingcons.io/posts/make-me-ceo-of-mozilla.html)

生成摘要时出错

---

## 99. Is Firefox Firefucked?

**原文标题**: Is Firefox Firefucked?

**原文链接**: [https://kevquirk.com/blog/is-firefox-firefucked/](https://kevquirk.com/blog/is-firefox-firefucked/)

生成摘要时出错

---

## 100. Microsoft kills IntelliCode in favor of the paid Copilot

**原文标题**: Microsoft kills IntelliCode in favor of the paid Copilot

**原文链接**: [https://visualstudiomagazine.com/articles/2025/12/17/microsoft-quietly-kills-intellicode-as-ai-strategy-shifts-to-copilot.aspx](https://visualstudiomagazine.com/articles/2025/12/17/microsoft-quietly-kills-intellicode-as-ai-strategy-shifts-to-copilot.aspx)

生成摘要时出错

---

