# Hacker News 热门文章摘要 (2026-06-16)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

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

## 11. Mechanical Watch (2022)

**原文标题**: Mechanical Watch (2022)

**原文链接**: [https://ciechanow.ski/mechanical-watch/](https://ciechanow.ski/mechanical-watch/)

生成摘要时出错

---

## 12. Banned book library in a wi-fi smart light bulb

**原文标题**: Banned book library in a wi-fi smart light bulb

**原文链接**: [https://www.richardosgood.com/posts/banned-book-library/](https://www.richardosgood.com/posts/banned-book-library/)

生成摘要时出错

---

## 13. Windows 11 users are tired of MS account requirements creeping into everything

**原文标题**: Windows 11 users are tired of MS account requirements creeping into everything

**原文链接**: [https://www.windowscentral.com/microsoft/windows-11/windows-11-users-are-tired-of-microsoft-account-requirements-and-workarounds](https://www.windowscentral.com/microsoft/windows-11/windows-11-users-are-tired-of-microsoft-account-requirements-and-workarounds)

生成摘要时出错

---

## 14. Feds freaked over Fable 5 after 'fix this code', not jailbreak, say researchers

**原文标题**: Feds freaked over Fable 5 after 'fix this code', not jailbreak, say researchers

**原文链接**: [https://www.theregister.com/security/2026/06/15/feds-freaked-over-fable-5-after-simple-fix-this-code-prompt-not-jailbreak-says-researcher/5255827](https://www.theregister.com/security/2026/06/15/feds-freaked-over-fable-5-after-simple-fix-this-code-prompt-not-jailbreak-says-researcher/5255827)

生成摘要时出错

---

## 15. Hetzner Price Adjustment

**原文标题**: Hetzner Price Adjustment

**原文链接**: [https://docs.hetzner.com/general/infrastructure-and-availability/price-adjustment/#cloud-servers](https://docs.hetzner.com/general/infrastructure-and-availability/price-adjustment/#cloud-servers)

生成摘要时出错

---

## 16. Apple Foundation Models

**原文标题**: Apple Foundation Models

**原文链接**: [https://platform.claude.com/docs/en/cli-sdks-libraries/libraries/apple-foundation-models](https://platform.claude.com/docs/en/cli-sdks-libraries/libraries/apple-foundation-models)

生成摘要时出错

---

## 17. The time the x86 emulator team found code so bad they fixed it during emulation

**原文标题**: The time the x86 emulator team found code so bad they fixed it during emulation

**原文链接**: [https://devblogs.microsoft.com/oldnewthing/20260615-00/?p=112419](https://devblogs.microsoft.com/oldnewthing/20260615-00/?p=112419)

生成摘要时出错

---

## 18. Apple's weird anti-nausea dots cured my car sickness

**原文标题**: Apple's weird anti-nausea dots cured my car sickness

**原文链接**: [https://www.theverge.com/tech/942854/apple-vehicle-motion-cues-review-really-work](https://www.theverge.com/tech/942854/apple-vehicle-motion-cues-review-really-work)

生成摘要时出错

---

## 19. My Homelab AI Dev Platform

**原文标题**: My Homelab AI Dev Platform

**原文链接**: [https://rsgm.dev/post/ai-dev-platform/](https://rsgm.dev/post/ai-dev-platform/)

生成摘要时出错

---

## 20. Fox to buy Roku

**原文标题**: Fox to buy Roku

**原文链接**: [https://www.wsj.com/business/deals/fox-roku-deal-f6e564f9](https://www.wsj.com/business/deals/fox-roku-deal-f6e564f9)

生成摘要时出错

---

## 21. Even more batteries included with Emacs

**原文标题**: Even more batteries included with Emacs

**原文链接**: [https://karthinks.com/software/even-more-batteries-included-with-emacs/](https://karthinks.com/software/even-more-batteries-included-with-emacs/)

生成摘要时出错

---

## 22. Copper transport drug restores memory and clears toxic Alzheimer's proteins

**原文标题**: Copper transport drug restores memory and clears toxic Alzheimer's proteins

**原文链接**: [https://www.monash.edu/news/articles/copper-drug-restores-memory-and-clears-toxic-alzheimers-proteins](https://www.monash.edu/news/articles/copper-drug-restores-memory-and-clears-toxic-alzheimers-proteins)

生成摘要时出错

---

## 23. U.S. pulling ocean sensors a 'shock' for Canadian research as El Niño nears

**原文标题**: U.S. pulling ocean sensors a 'shock' for Canadian research as El Niño nears

**原文链接**: [https://www.timescolonist.com/local-news/us-pulling-ocean-sensors-a-shock-for-canadian-research-as-el-nino-nears-12422874](https://www.timescolonist.com/local-news/us-pulling-ocean-sensors-a-shock-for-canadian-research-as-el-nino-nears-12422874)

生成摘要时出错

---

## 24. Typst 0.15.0

**原文标题**: Typst 0.15.0

**原文链接**: [https://typst.app/docs/changelog/0.15.0/](https://typst.app/docs/changelog/0.15.0/)

生成摘要时出错

---

## 25. Salesforce to Acquire Fin (formerly Intercom) for $3.6B

**原文标题**: Salesforce to Acquire Fin (formerly Intercom) for $3.6B

**原文链接**: [https://www.salesforce.com/news/press-releases/2026/06/15/salesforce-signs-definitive-agreement-to-acquire-fin/?bc=HL](https://www.salesforce.com/news/press-releases/2026/06/15/salesforce-signs-definitive-agreement-to-acquire-fin/?bc=HL)

生成摘要时出错

---

## 26. I Love the Computer

**原文标题**: I Love the Computer

**原文链接**: [https://michaelenger.com/blog/i-love-the-computer/](https://michaelenger.com/blog/i-love-the-computer/)

生成摘要时出错

---

## 27. SpaceX Is Buying Cursor

**原文标题**: SpaceX Is Buying Cursor

**原文链接**: [https://www.bbc.com/news/articles/cvgd5g7d7gyo](https://www.bbc.com/news/articles/cvgd5g7d7gyo)

生成摘要时出错

---

## 28. Is Meta destroying its engineering organization?

**原文标题**: Is Meta destroying its engineering organization?

**原文链接**: [https://newsletter.pragmaticengineer.com/p/why-is-meta-destroying-its-engineering](https://newsletter.pragmaticengineer.com/p/why-is-meta-destroying-its-engineering)

生成摘要时出错

---

## 29. Peopleless economy? Not technically impossible

**原文标题**: Peopleless economy? Not technically impossible

**原文链接**: [https://gmalandrakis.com/writings/ad-economicum.html](https://gmalandrakis.com/writings/ad-economicum.html)

生成摘要时出错

---

## 30. I Could've Rickrolled the FIFA World Cup. All I Needed Was My ID

**原文标题**: I Could've Rickrolled the FIFA World Cup. All I Needed Was My ID

**原文链接**: [https://bobdahacker.com/blog/fifa-hack](https://bobdahacker.com/blog/fifa-hack)

生成摘要时出错

---

## 31. Google Chrome update will close the door on ad blockers

**原文标题**: Google Chrome update will close the door on ad blockers

**原文链接**: [https://9to5google.com/2026/06/15/google-chromes-next-update-will-mark-the-end-of-popular-ad-blockers/](https://9to5google.com/2026/06/15/google-chromes-next-update-will-mark-the-end-of-popular-ad-blockers/)

生成摘要时出错

---

## 32. Correlated randomness in Slay the Spire 2

**原文标题**: Correlated randomness in Slay the Spire 2

**原文链接**: [https://tck.mn/blog/correlated-randomness-sts2/](https://tck.mn/blog/correlated-randomness-sts2/)

生成摘要时出错

---

## 33. What job interviews taught me about Kubernetes

**原文标题**: What job interviews taught me about Kubernetes

**原文链接**: [https://notnotp.com/notes/what-job-interviews-taught-me-about-kubernetes/](https://notnotp.com/notes/what-job-interviews-taught-me-about-kubernetes/)

生成摘要时出错

---

## 34. Apple is about to make Hide My Email useless

**原文标题**: Apple is about to make Hide My Email useless

**原文链接**: [https://arseniyshestakov.com/2026/06/16/apple-is-about-to-make-hide-my-email-useless/](https://arseniyshestakov.com/2026/06/16/apple-is-about-to-make-hide-my-email-useless/)

生成摘要时出错

---

## 35. Game Engine White Papers: Commander Keen

**原文标题**: Game Engine White Papers: Commander Keen

**原文链接**: [https://forgottenbytes.net/commander_keen.html](https://forgottenbytes.net/commander_keen.html)

生成摘要时出错

---

## 36. US battery manufacturing output continues to break records

**原文标题**: US battery manufacturing output continues to break records

**原文链接**: [https://fred.stlouisfed.org/series/IPG33591S](https://fred.stlouisfed.org/series/IPG33591S)

生成摘要时出错

---

## 37. Stanford grads walk out on Google CEO Sundar Pichai speech

**原文标题**: Stanford grads walk out on Google CEO Sundar Pichai speech

**原文链接**: [https://twitter.com/maattttbrown/status/2066215255987163246](https://twitter.com/maattttbrown/status/2066215255987163246)

生成摘要时出错

---

## 38. Why I email complete strangers

**原文标题**: Why I email complete strangers

**原文链接**: [https://www.goodinternetmagazine.com/why-i-email-complete-strangers/](https://www.goodinternetmagazine.com/why-i-email-complete-strangers/)

生成摘要时出错

---

## 39. Openrouter Fusion API

**原文标题**: Openrouter Fusion API

**原文链接**: [https://openrouter.ai/openrouter/fusion](https://openrouter.ai/openrouter/fusion)

生成摘要时出错

---

## 40. Anthropic's Safety Superpower

**原文标题**: Anthropic's Safety Superpower

**原文链接**: [https://stratechery.com/2026/anthropics-safety-superpower/](https://stratechery.com/2026/anthropics-safety-superpower/)

生成摘要时出错

---

## 41. Improvement in advanced Alzheimer’s disease following high-dose psilocybin

**原文标题**: Improvement in advanced Alzheimer’s disease following high-dose psilocybin

**原文链接**: [https://www.frontiersin.org/journals/neuroscience/articles/10.3389/fnins.2026.1813281/full](https://www.frontiersin.org/journals/neuroscience/articles/10.3389/fnins.2026.1813281/full)

生成摘要时出错

---

## 42. Did Anthropic ask for this?

**原文标题**: Did Anthropic ask for this?

**原文链接**: [https://www.verysane.ai/p/did-anthropic-ask-for-this](https://www.verysane.ai/p/did-anthropic-ask-for-this)

生成摘要时出错

---

## 43. TIL: You can make HTTP requests without curl using Bash /dev/TCP

**原文标题**: TIL: You can make HTTP requests without curl using Bash /dev/TCP

**原文链接**: [https://mareksuppa.com/til/bash-dev-tcp-http-without-curl/](https://mareksuppa.com/til/bash-dev-tcp-http-without-curl/)

生成摘要时出错

---

## 44. Claude: Elevated errors across many models [resolved]

**原文标题**: Claude: Elevated errors across many models [resolved]

**原文链接**: [https://status.claude.com/incidents/xmhsglsz3h3w](https://status.claude.com/incidents/xmhsglsz3h3w)

生成摘要时出错

---

## 45. How TimescaleDB compresses time-series data

**原文标题**: How TimescaleDB compresses time-series data

**原文链接**: [https://roszigit.com/en/blog/timescaledb-compression-hypercore](https://roszigit.com/en/blog/timescaledb-compression-hypercore)

生成摘要时出错

---

## 46. But yak shaving is fun (2019)

**原文标题**: But yak shaving is fun (2019)

**原文链接**: [https://parksb.github.io/en/article/32.html](https://parksb.github.io/en/article/32.html)

生成摘要时出错

---

## 47. Humanity isn't ready for the coming intelligence explosion

**原文标题**: Humanity isn't ready for the coming intelligence explosion

**原文链接**: [https://www.economist.com/by-invitation/2026/06/15/humanity-isnt-ready-for-the-coming-intelligence-explosion](https://www.economist.com/by-invitation/2026/06/15/humanity-isnt-ready-for-the-coming-intelligence-explosion)

生成摘要时出错

---

## 48. Commodore Releases Flip Phone

**原文标题**: Commodore Releases Flip Phone

**原文链接**: [https://commodore.net/why-a-flip-phone/](https://commodore.net/why-a-flip-phone/)

生成摘要时出错

---

## 49. I've always wondered if anyone used sharing buttons on news sites and blogs

**原文标题**: I've always wondered if anyone used sharing buttons on news sites and blogs

**原文链接**: [https://ankursethi.com/links/nobody-clicks-your-share-buttons/](https://ankursethi.com/links/nobody-clicks-your-share-buttons/)

生成摘要时出错

---

## 50. Claude Corps

**原文标题**: Claude Corps

**原文链接**: [https://www.anthropic.com/news/claude-corps](https://www.anthropic.com/news/claude-corps)

生成摘要时出错

---

## 51. The rich aren't your role models

**原文标题**: The rich aren't your role models

**原文链接**: [https://theslowburningfuse.wordpress.com/2026/06/14/the-rich-arent-your-role-models-theyre-your-oppressors/](https://theslowburningfuse.wordpress.com/2026/06/14/the-rich-arent-your-role-models-theyre-your-oppressors/)

生成摘要时出错

---

## 52. Microsoft turns to AWS as GitHub faces AI capacity crunch

**原文标题**: Microsoft turns to AWS as GitHub faces AI capacity crunch

**原文链接**: [https://runtimewire.com/article/microsoft-github-aws-ai-capacity-crunch](https://runtimewire.com/article/microsoft-github-aws-ai-capacity-crunch)

生成摘要时出错

---

## 53. Calvin and Hobbes and the price of integrity

**原文标题**: Calvin and Hobbes and the price of integrity

**原文链接**: [https://therepublicofletters.substack.com/p/calvin-and-hobbes-and-the-price-of](https://therepublicofletters.substack.com/p/calvin-and-hobbes-and-the-price-of)

生成摘要时出错

---

## 54. Show HN: I wrote a C++ ray tracer from scratch without AI

**原文标题**: Show HN: I wrote a C++ ray tracer from scratch without AI

**原文链接**: [https://github.com/themartiano/luz](https://github.com/themartiano/luz)

生成摘要时出错

---

## 55. Google Flight Simulator

**原文标题**: Google Flight Simulator

**原文链接**: [https://developers.google.com/maps/documentation/earth/flight-simulator](https://developers.google.com/maps/documentation/earth/flight-simulator)

生成摘要时出错

---

## 56. I Fired Google

**原文标题**: I Fired Google

**原文链接**: [https://www.theartofdoingstuff.com/i-fired-google/](https://www.theartofdoingstuff.com/i-fired-google/)

生成摘要时出错

---

## 57. Show HN: Garden of Flowers – an archive of pictorial typography before ASCII art

**原文标题**: Show HN: Garden of Flowers – an archive of pictorial typography before ASCII art

**原文链接**: [https://garden-of-flowers.heikkilotvonen.com/](https://garden-of-flowers.heikkilotvonen.com/)

生成摘要时出错

---

## 58. 21 years and counting of 'eight fallacies of distributed computing' (2025)

**原文标题**: 21 years and counting of 'eight fallacies of distributed computing' (2025)

**原文链接**: [https://blog.apnic.net/2025/12/08/21-years-and-counting-of-eight-fallacies-of-distributed-computing/](https://blog.apnic.net/2025/12/08/21-years-and-counting-of-eight-fallacies-of-distributed-computing/)

生成摘要时出错

---

## 59. How memory safety CVEs differ between Rust and C/C++

**原文标题**: How memory safety CVEs differ between Rust and C/C++

**原文链接**: [https://kobzol.github.io/rust/2026/06/15/how-memory-safety-cves-differ-between-rust-and-c-cpp.html](https://kobzol.github.io/rust/2026/06/15/how-memory-safety-cves-differ-between-rust-and-c-cpp.html)

生成摘要时出错

---

## 60. Stop Using JWTs

**原文标题**: Stop Using JWTs

**原文链接**: [https://gist.github.com/samsch/0d1f3d3b4745d778f78b230cf6061452](https://gist.github.com/samsch/0d1f3d3b4745d778f78b230cf6061452)

生成摘要时出错

---

## 61. 'Ghost jobs' could soon be illegal in New York

**原文标题**: 'Ghost jobs' could soon be illegal in New York

**原文链接**: [https://www.fastcompany.com/91558427/ghost-jobs-could-soon-be-illegal-in-new-york](https://www.fastcompany.com/91558427/ghost-jobs-could-soon-be-illegal-in-new-york)

生成摘要时出错

---

## 62. Around 200 Stanford students walk out as Google CEO takes stage

**原文标题**: Around 200 Stanford students walk out as Google CEO takes stage

**原文链接**: [https://www.sfgate.com/tech/article/sundar-pichai-stanford-commencement-22304888.php](https://www.sfgate.com/tech/article/sundar-pichai-stanford-commencement-22304888.php)

生成摘要时出错

---

## 63. Russian artist and Putin critic shot dead in Poland

**原文标题**: Russian artist and Putin critic shot dead in Poland

**原文链接**: [https://www.bbc.com/news/articles/clyrzd5g6k2o](https://www.bbc.com/news/articles/clyrzd5g6k2o)

生成摘要时出错

---

## 64. Can Europe train a frontier AI model on the compute it owns?

**原文标题**: Can Europe train a frontier AI model on the compute it owns?

**原文链接**: [https://github.com/sammysltd/euromesh](https://github.com/sammysltd/euromesh)

生成摘要时出错

---

## 65. Google Chrome's Next Update Will Mark the End of Popular Ad Blockers

**原文标题**: Google Chrome's Next Update Will Mark the End of Popular Ad Blockers

**原文链接**: [https://tech.slashdot.org/story/26/06/15/205219/google-chromes-next-update-will-mark-the-end-of-popular-ad-blockers](https://tech.slashdot.org/story/26/06/15/205219/google-chromes-next-update-will-mark-the-end-of-popular-ad-blockers)

生成摘要时出错

---

## 66. OpenAI Losses Increased Nearly 8X in 2025, with Spending Hitting $34B

**原文标题**: OpenAI Losses Increased Nearly 8X in 2025, with Spending Hitting $34B

**原文链接**: [https://www.wheresyoured.at/exclusive-openai-financials/](https://www.wheresyoured.at/exclusive-openai-financials/)

生成摘要时出错

---

## 67. Boot Naked Linux

**原文标题**: Boot Naked Linux

**原文链接**: [https://nick.zoic.org/art/boot-naked-linux/](https://nick.zoic.org/art/boot-naked-linux/)

生成摘要时出错

---

## 68. Amazon Announces Multibillion-Dollar Data Center in Missouri

**原文标题**: Amazon Announces Multibillion-Dollar Data Center in Missouri

**原文链接**: [https://www.narracomm.com/amazon-announces-multibillion-dollar-data-center-in-missouri/](https://www.narracomm.com/amazon-announces-multibillion-dollar-data-center-in-missouri/)

生成摘要时出错

---

## 69. Why Is Claude Turning into an a**Hole?

**原文标题**: Why Is Claude Turning into an a**Hole?

**原文链接**: [https://bramcohen.com/p/why-is-claude-turning-into-an-asshole](https://bramcohen.com/p/why-is-claude-turning-into-an-asshole)

生成摘要时出错

---

## 70. Understanding the rationale behind a rule when trying to circumvent it

**原文标题**: Understanding the rationale behind a rule when trying to circumvent it

**原文链接**: [https://devblogs.microsoft.com/oldnewthing/20260611-00/?p=112415](https://devblogs.microsoft.com/oldnewthing/20260611-00/?p=112415)

生成摘要时出错

---

## 71. Fable ban was never about a jailbreak?

**原文标题**: Fable ban was never about a jailbreak?

**原文链接**: [https://techcrunch.com/2026/06/15/the-us-governments-anthropic-models-ban-was-never-about-an-ai-jailbreak/](https://techcrunch.com/2026/06/15/the-us-governments-anthropic-models-ban-was-never-about-an-ai-jailbreak/)

生成摘要时出错

---

## 72. US Air Force B-52 bomber crashes after takeoff, Edwards Air Force Base says

**原文标题**: US Air Force B-52 bomber crashes after takeoff, Edwards Air Force Base says

**原文链接**: [https://www.reuters.com/business/aerospace-defense/us-air-force-b-52-bomber-crashes-after-takeoff-edwards-air-force-base-says-2026-06-15/](https://www.reuters.com/business/aerospace-defense/us-air-force-b-52-bomber-crashes-after-takeoff-edwards-air-force-base-says-2026-06-15/)

生成摘要时出错

---

## 73. US and Iran announce deal to end military operations

**原文标题**: US and Iran announce deal to end military operations

**原文链接**: [https://www.bbc.com/news/live/cj0grpyg4v1t](https://www.bbc.com/news/live/cj0grpyg4v1t)

生成摘要时出错

---

## 74. Trinket.io shutting down, so we saved it and hosted it a trinket.strivemath.org

**原文标题**: Trinket.io shutting down, so we saved it and hosted it a trinket.strivemath.org

**原文链接**: [https://trinket.strivemath.org/](https://trinket.strivemath.org/)

生成摘要时出错

---

## 75. SubQ 1.1 Small

**原文标题**: SubQ 1.1 Small

**原文链接**: [https://subq.ai/subq-1-1-small-technical-report](https://subq.ai/subq-1-1-small-technical-report)

生成摘要时出错

---

## 76. GPT‑NL: a sovereign language model for the Netherlands

**原文标题**: GPT‑NL: a sovereign language model for the Netherlands

**原文链接**: [https://www.tno.nl/en/digital/artificial-intelligence/gpt-nl/](https://www.tno.nl/en/digital/artificial-intelligence/gpt-nl/)

生成摘要时出错

---

## 77. Never talk to the police

**原文标题**: Never talk to the police

**原文链接**: [https://www.campolalaw.com/why-you-should-never-talk-to-the-po](https://www.campolalaw.com/why-you-should-never-talk-to-the-po)

生成摘要时出错

---

## 78. Qwen-Robot Suite: A Foundation Model Suite for Physical World Intelligence

**原文标题**: Qwen-Robot Suite: A Foundation Model Suite for Physical World Intelligence

**原文链接**: [https://qwen.ai/blog?id=qwen-robotsuite](https://qwen.ai/blog?id=qwen-robotsuite)

生成摘要时出错

---

## 79. Show HN: machine0 – Persistent NixOS VMs You Control from the CLI

**原文标题**: Show HN: machine0 – Persistent NixOS VMs You Control from the CLI

**原文链接**: [https://machine0.io](https://machine0.io)

生成摘要时出错

---

## 80. The hallucinogenic mushroom that contains no known psychedelic

**原文标题**: The hallucinogenic mushroom that contains no known psychedelic

**原文链接**: [https://psychedelics.co.uk/news/a-mushroom-genus-that-gets-people-high-but-not-the](https://psychedelics.co.uk/news/a-mushroom-genus-that-gets-people-high-but-not-the)

生成摘要时出错

---

## 81. After AI Takes Everything

**原文标题**: After AI Takes Everything

**原文链接**: [https://ursb.me/en/posts/after-ai-takes-everything/](https://ursb.me/en/posts/after-ai-takes-everything/)

生成摘要时出错

---

## 82. Unicorn – The Ultimate CPU Emulator

**原文标题**: Unicorn – The Ultimate CPU Emulator

**原文链接**: [https://www.unicorn-engine.org/](https://www.unicorn-engine.org/)

生成摘要时出错

---

## 83. Vance: Iran can have access to $300B reconstruction fund

**原文标题**: Vance: Iran can have access to $300B reconstruction fund

**原文链接**: [https://thehill.com/homenews/administration/5924963-vance-iran-300b-reconstruction-fund/](https://thehill.com/homenews/administration/5924963-vance-iran-300b-reconstruction-fund/)

生成摘要时出错

---

## 84. 'Wow, it really worked ': 70s TV show causing worldwide panic today

**原文标题**: 'Wow, it really worked ': 70s TV show causing worldwide panic today

**原文链接**: [https://www.theguardian.com/tv-and-radio/2026/jun/16/alternative-3-mockumentary-missing-scientists-conspiracy-50-years-later](https://www.theguardian.com/tv-and-radio/2026/jun/16/alternative-3-mockumentary-missing-scientists-conspiracy-50-years-later)

生成摘要时出错

---

## 85. Abu Fanous

**原文标题**: Abu Fanous

**原文链接**: [https://en.wikipedia.org/wiki/Abu_Fanous](https://en.wikipedia.org/wiki/Abu_Fanous)

生成摘要时出错

---

## 86. Fox Is Buying Roku

**原文标题**: Fox Is Buying Roku

**原文链接**: [https://www.fastcompany.com/91559558/fox-corp-buying-roku-stock-prices-fall-on-tv-streaming-merger](https://www.fastcompany.com/91559558/fox-corp-buying-roku-stock-prices-fall-on-tv-streaming-merger)

生成摘要时出错

---

## 87. Reviews have become expensive, rewrites have become cheap

**原文标题**: Reviews have become expensive, rewrites have become cheap

**原文链接**: [http://ishmeetbindra.com/posts/reviews-have-become-expensive-rewrites-have-become-cheap/](http://ishmeetbindra.com/posts/reviews-have-become-expensive-rewrites-have-become-cheap/)

生成摘要时出错

---

## 88. San Francisco Weighs PG&E Takeover Amid Soaring Utility Costs

**原文标题**: San Francisco Weighs PG&E Takeover Amid Soaring Utility Costs

**原文链接**: [https://www.kqed.org/news/12081882/san-francisco-has-been-trying-to-leave-pge-for-100-years-will-this-time-be-different](https://www.kqed.org/news/12081882/san-francisco-has-been-trying-to-leave-pge-for-100-years-will-this-time-be-different)

生成摘要时出错

---

## 89. KDE Plasma 6.7 Released

**原文标题**: KDE Plasma 6.7 Released

**原文链接**: [https://kde.org/announcements/plasma/6/6.7.0/](https://kde.org/announcements/plasma/6/6.7.0/)

生成摘要时出错

---

## 90. Show HN: Veterinarian turned founder, AI lawn diagnosis

**原文标题**: Show HN: Veterinarian turned founder, AI lawn diagnosis

**原文链接**: [https://grassdx.com/](https://grassdx.com/)

生成摘要时出错

---

## 91. Making espresso with ultrasound

**原文标题**: Making espresso with ultrasound

**原文链接**: [https://www.unsw.edu.au/newsroom/news/2026/06/New-way-making-espresso](https://www.unsw.edu.au/newsroom/news/2026/06/New-way-making-espresso)

生成摘要时出错

---

## 92. Under-16s to be banned from social media, Starmer announces

**原文标题**: Under-16s to be banned from social media, Starmer announces

**原文链接**: [https://www.bbc.co.uk/news/live/c77yx1jpg1nt](https://www.bbc.co.uk/news/live/c77yx1jpg1nt)

生成摘要时出错

---

## 93. Making ast.walk 220x Faster

**原文标题**: Making ast.walk 220x Faster

**原文链接**: [https://reflex.dev/blog/why-ast-walk-when-you-can-ast-sprint/](https://reflex.dev/blog/why-ast-walk-when-you-can-ast-sprint/)

生成摘要时出错

---

## 94. Is Fable 5 Back?

**原文标题**: Is Fable 5 Back?

**原文链接**: [https://isfable5back.com](https://isfable5back.com)

生成摘要时出错

---

## 95. America has lost its war with Iran

**原文标题**: America has lost its war with Iran

**原文链接**: [https://www.independent.co.uk/voices/editorials/america-trump-iran-ceasefire-agreement-war-hormuz-b2995971.html](https://www.independent.co.uk/voices/editorials/america-trump-iran-ceasefire-agreement-war-hormuz-b2995971.html)

生成摘要时出错

---

## 96. Techno-libertarians are flocking to the Caribbean

**原文标题**: Techno-libertarians are flocking to the Caribbean

**原文链接**: [https://economist.com/the-americas/2026/06/11/techno-libertarians-are-flocking-to-the-caribbean](https://economist.com/the-americas/2026/06/11/techno-libertarians-are-flocking-to-the-caribbean)

生成摘要时出错

---

## 97. Has AI already killed self-help nonfiction books?

**原文标题**: Has AI already killed self-help nonfiction books?

**原文链接**: [https://tim.blog/2026/06/12/has-ai-already-killed-nonfiction/](https://tim.blog/2026/06/12/has-ai-already-killed-nonfiction/)

生成摘要时出错

---

## 98. 10Gb/s Ethernet: switching to a Broadcom SFP+ module

**原文标题**: 10Gb/s Ethernet: switching to a Broadcom SFP+ module

**原文链接**: [https://www.gilesthomas.com/2026/06/10g-ethernet-switching-to-broadcom-sfp-plus](https://www.gilesthomas.com/2026/06/10g-ethernet-switching-to-broadcom-sfp-plus)

生成摘要时出错

---

## 99. UK to require ID or face scan before you can make social media accounts

**原文标题**: UK to require ID or face scan before you can make social media accounts

**原文链接**: [https://www.bleepingcomputer.com/news/security/uk-to-require-id-or-face-scan-before-you-can-make-social-media-accounts/](https://www.bleepingcomputer.com/news/security/uk-to-require-id-or-face-scan-before-you-can-make-social-media-accounts/)

生成摘要时出错

---

## 100. Anthropic flies staff to D.C. to clean up White House fight

**原文标题**: Anthropic flies staff to D.C. to clean up White House fight

**原文链接**: [https://www.axios.com/2026/06/14/anthropic-white-house-mythos-fable](https://www.axios.com/2026/06/14/anthropic-white-house-mythos-fable)

生成摘要时出错

---

