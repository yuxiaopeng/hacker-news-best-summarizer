# Hacker News 热门文章摘要 (2026-02-26)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 谷歌 API 密钥原本不是秘密，但 Gemini 改变了规则

**原文标题**: Google API keys weren't secrets, but then Gemini changed the rules

**原文链接**: [https://trufflesecurity.com/blog/google-api-keys-werent-secrets-but-then-gemini-changed-the-rules](https://trufflesecurity.com/blog/google-api-keys-werent-secrets-but-then-gemini-changed-the-rules)

Truffle Security 发现了一个重大漏洞：过去被认为可以安全地公开嵌入在地图和 Firebase 等服务中的 Google API 密钥，现在却能提供对 Gemini AI API 的敏感访问。十多年来，Google 一直告知开发者，这些密钥并非秘密，主要作为项目标识符用于计费，且功能受限。

然而，当 Google Cloud 项目中启用了 Gemini API（即生成式语言 API）时，该项目内现有的 API 密钥，即使是那些已公开暴露的，也会悄无声息地获得对 Gemini 端点的完全访问权限。这种“追溯性权限扩展”意味着一个旧的、公开的地图密钥可能突然变成访问上传文件、缓存数据并产生巨额 AI 计费的凭据。新的 API 密钥也默认为“无限制”，一旦启用，它们会立即对 Gemini 生效。

Truffle Security 扫描了数百万个网站，发现了 2,863 个此类易受攻击的 Google API 密钥，其中一些甚至被 Google 自己使用。攻击者可以轻易地从公共网页抓取这些密钥，无需触及受害者的基础设施，即可访问私人数据或耗尽配额。

Google 最初驳回了该报告，但在收到包括来自 Google 自身基础设施的示例在内的具体证据后，将其重新归类为 bug。Google 现在正在实施变革，例如为新密钥设置作用域默认值、阻止泄露的密钥以及主动发送通知，以解决此问题。建议用户检查其 GCP 项目是否启用了生成式语言 API，审计密钥是否存在无限制或 Gemini 访问权限，验证此类密钥是否未公开，并立即轮换任何已暴露的凭据。

---

## 2. 丹麦政府机构将弃用微软软件 (2025)

**原文标题**: Danish government agency to ditch Microsoft software (2025)

**原文链接**: [https://therecord.media/denmark-digital-agency-microsoft-digital-independence](https://therecord.media/denmark-digital-agency-microsoft-digital-independence)

丹麦数字化部计划用包括LibreOffice在内的开源软件替代微软软件，以实现数字独立并减少对美国科技公司的依赖。丹麦数字化大臣卡罗琳·施塔格·奥尔森证实，该部一半以上的员工将于下月从Microsoft Office转向LibreOffice，预计年底前完成全面过渡。此举也旨在避免管理将于10月失去官方支持的过时Windows 10系统所产生的费用。

这一决定是出于对“数字主权”的追求、成本考量、微软的市场主导地位以及过去与华盛顿在数据保护方面的政治紧张关系。虽然如果过渡过于复杂，该部可能会恢复原状，但这一转变与丹麦最大城市哥本哈根和奥胡斯的类似计划不谋而合。这也反映了更广泛的欧洲趋势，德国石勒苏益格-荷尔斯泰因州同样正在转向LibreOffice和Open-Xchange，并计划迁移到Linux操作系统，以建立一个“数字主权IT工作场所”。

---

## 3. Never buy a .online domain

**原文标题**: Never buy a .online domain

**原文链接**: [https://www.0xsid.com/blog/online-tld-is-pain](https://www.0xsid.com/blog/online-tld-is-pain)

生成摘要时出错

---

## 4. HN上的新用户更可能使用破折号。

**原文标题**: New accounts on HN more likely to use em-dashes

**原文链接**: [https://www.marginalia.nu/weird-ai-crap/hn/](https://www.marginalia.nu/weird-ai-crap/hn/)

作者对近期Hacker News (HN) 上机器人数量激增表示担忧，并指出评论明显出现异常以及讨论质量普遍下降，表现为平庸或离题的言论。

为了调查，他们分别从`/newcomments`（最新评论）和`/noobcomments`（新注册账户的最新评论）中抓取了大约700条评论。分析揭示了两个重要发现：

1.  **符号使用：** 新注册账户的评论使用破折号、箭头及其他符号的可能性高出近10倍（在评论中占比17.47% 对 1.83%；p = 7e-20）。
2.  **提及AI/LLM：** 新账户提及AI和LLM的可能性也更高（在评论中占比18.67% 对 11.8%；p = 0.0018）。

尽管样本量适中，作者仍强调这些是“相当大的差异”，尤其是符号使用率高出10倍这一点，他们认为这难以用合法的真人用户行为来解释，并将其解读为机器人活动增加的有力证据。

---

## 5. 安特罗匹克放弃旗舰安全承诺

**原文标题**: Anthropic Drops Flagship Safety Pledge

**原文链接**: [https://time.com/7380854/exclusive-anthropic-drops-flagship-safety-pledge/](https://time.com/7380854/exclusive-anthropic-drops-flagship-safety-pledge/)

Anthropic, an AI company that positioned itself as the most safety-conscious, has dropped a central pledge from its 2023 Responsible Scaling Policy (RSP). Previously, Anthropic committed to never training an AI system without guaranteeing adequate safety measures in advance, a promise touted as resisting market pressures.

The revamped RSP eliminates this "guarantee in advance" stipulation. Instead, Anthropic now pledges greater transparency on AI risks, aims to match or exceed competitors' safety efforts, and will only "delay" AI development if it's both leading the AI race and believes catastrophic risks are significant.

Chief Science Officer Jared Kaplan explained the shift, citing the lack of similar commitments from rivals, the failure of national/international regulations to materialize, and the increasing complexity of AI safety evaluations. He stressed that stopping development while competitors advanced would render Anthropic irrelevant for safety research. The company argues that to understand and mitigate frontier risks, it must build frontier models.

This policy change coincides with Anthropic's recent commercial and technological successes, including a $30 billion investment. While Kaplan denies capitulating to market incentives, framing it as a pragmatic response to emerging realities, critics like Chris Painter of METR view it as a "bearish signal" that society is unprepared for potential AI catastrophes, warning of a "frog-boiling" effect without clear safety thresholds.

Anthropic maintains the new policy reinforces its commitment to safety by promising regular "Frontier Safety Roadmaps" and "Risk Reports" to drive transparency and prioritize safety research.

---

## 6. 亚马逊被控普遍哄抬物价，波及整个经济。

**原文标题**: Amazon accused of widespread scheme to inflate prices across the economy

**原文链接**: [https://www.thebignewsletter.com/p/amazon-busted-for-widespread-price](https://www.thebignewsletter.com/p/amazon-busted-for-widespread-price)

由联邦贸易委员会（FTC）和17个州检察长提起的一项诉讼，指控亚马逊实施一项旨在在整个经济领域内普遍抬高物价的计划，损害了消费者和竞争企业双方的利益。诉状声称，亚马逊利用其垄断权力，强迫第三方卖家签订反竞争协议，阻止他们在竞争性电商平台上提供更低的价格。

一项关键指控集中在亚马逊的“公平定价政策”上，诉讼称其为一项欺骗性的价格均等条款。根据这项政策，亚马逊据称会惩罚那些在沃尔玛或eBay等竞争网站上以更低价格列出商品的卖家。惩罚包括降低商品可见度、移除备受追捧的“购买按钮”，甚至完全下架商品，从而有效切断卖家与亚马逊庞大客户群的联系。这种压力迫使卖家在其他平台上提高价格，以避免亚马逊的制裁，导致整个互联网上的价格被人为抬高。

诉讼进一步详细说明了亚马逊如何利用算法检测其他地方的更低价格，并随后提高自身价格，有时在热门商品上涨幅高达16%。FTC认为这些做法扼杀竞争、抑制创新，并每年从消费者那里攫取数十亿美元。这项法律行动旨在制止亚马逊涉嫌的反竞争行为，处以金钱罚款，并可能强制进行结构性改革，以恢复电商市场的竞争。

---

## 7. 吉米·亨德里克斯是一名系统工程师

**原文标题**: Jimi Hendrix was a systems engineer

**原文链接**: [https://spectrum.ieee.org/jimi-hendrix-systems-engineer](https://spectrum.ieee.org/jimi-hendrix-systems-engineer)

在《DIY动手杂志》的一篇文章中，边缘计算架构师Rohan S. Puranik提出，吉米·亨德里克斯（Jimi Hendrix）实际上是一名系统工程师。Puranik认为，亨德里克斯通过一系列组件精确控制了声音调制和反馈回路。他“工程学”的一个关键方面在于通过策略性地调整吉他相对于放大器扬声器的位置来操纵反馈。

---

## 8. Mac mini will be made at a new facility in Houston

**原文标题**: Mac mini will be made at a new facility in Houston

**原文链接**: [https://www.apple.com/newsroom/2026/02/apple-accelerates-us-manufacturing-with-mac-mini-production/](https://www.apple.com/newsroom/2026/02/apple-accelerates-us-manufacturing-with-mac-mini-production/)

生成摘要时出错

---

## 9. Pi — 极简终端编程套件

**原文标题**: Pi – A minimal terminal coding harness

**原文链接**: [https://pi.dev](https://pi.dev)

Pi 是一个极简的终端编码框架，旨在实现最大程度的适应性和可扩展性。它不强制规定工作流程，而是提供一个灵活的核心，用户可以使用 TypeScript 扩展、技能、提示模板和主题进行扩展，所有这些都可以作为 npm 或 Git 包共享。

它支持超过 15 个 AI 提供商和数百种模型（例如 Anthropic、OpenAI、Google），并允许在会话中途切换模型。Pi 具有树状结构、可共享的会话历史记录，支持导航、分支、导出为 HTML 或作为 GitHub gist 共享。它对上下文工程的重视，通过 `AGENTS.md`、`SYSTEM.md` 和可自定义的压缩功能，提供了对提示和上下文窗口的精确控制。

Pi 以四种模式运行：交互式 TUI、用于脚本的打印/JSON、用于非 Node 集成的 RPC 和用于嵌入的 SDK。它的理念是提供“原语，而非功能”；其他代理中常见的功能——例如子代理、计划模式或权限门控——都留给用户通过扩展自行构建，或从社区包中安装。这种方法确保了核心的极简性，同时允许用户根据自身特定需求完全塑造 Pi。社区互动通过 GitHub、Discord 和全面的文档进行。

---

## 10. Anthropic ditches its core safety promise

**原文标题**: Anthropic ditches its core safety promise

**原文链接**: [https://www.cnn.com/2026/02/25/tech/anthropic-safety-policy-change](https://www.cnn.com/2026/02/25/tech/anthropic-safety-policy-change)

生成摘要时出错

---

## 11. Claude Code Remote Control

**原文标题**: Claude Code Remote Control

**原文链接**: [https://code.claude.com/docs/en/remote-control](https://code.claude.com/docs/en/remote-control)

生成摘要时出错

---

## 12. US orders diplomats to fight data sovereignty initiatives

**原文标题**: US orders diplomats to fight data sovereignty initiatives

**原文链接**: [https://www.reuters.com/sustainability/boards-policy-regulation/us-orders-diplomats-fight-data-sovereignty-initiatives-2026-02-25/](https://www.reuters.com/sustainability/boards-policy-regulation/us-orders-diplomats-fight-data-sovereignty-initiatives-2026-02-25/)

生成摘要时出错

---

## 13. How we rebuilt Next.js with AI in one week

**原文标题**: How we rebuilt Next.js with AI in one week

**原文链接**: [https://blog.cloudflare.com/vinext/](https://blog.cloudflare.com/vinext/)

生成摘要时出错

---

## 14. Following 35% growth, solar has passed hydro on US grid

**原文标题**: Following 35% growth, solar has passed hydro on US grid

**原文链接**: [https://arstechnica.com/science/2026/02/final-2025-data-is-in-us-energy-use-is-up-as-solar-passes-hydro/](https://arstechnica.com/science/2026/02/final-2025-data-is-in-us-energy-use-is-up-as-solar-passes-hydro/)

生成摘要时出错

---

## 15. Banned in California

**原文标题**: Banned in California

**原文链接**: [https://www.bannedincalifornia.org/](https://www.bannedincalifornia.org/)

生成摘要时出错

---

## 16. Tech companies shouldn't be bullied into doing surveillance

**原文标题**: Tech companies shouldn't be bullied into doing surveillance

**原文链接**: [https://www.eff.org/deeplinks/2026/02/tech-companies-shouldnt-be-bullied-doing-surveillance](https://www.eff.org/deeplinks/2026/02/tech-companies-shouldnt-be-bullied-doing-surveillance)

生成摘要时出错

---

## 17. How will OpenAI compete?

**原文标题**: How will OpenAI compete?

**原文链接**: [https://www.ben-evans.com/benedictevans/2026/2/19/how-will-openai-compete-nkg2x](https://www.ben-evans.com/benedictevans/2026/2/19/how-will-openai-compete-nkg2x)

生成摘要时出错

---

## 18. Bus stop balancing is fast, cheap, and effective

**原文标题**: Bus stop balancing is fast, cheap, and effective

**原文链接**: [https://worksinprogress.co/issue/the-united-states-needs-fewer-bus-stops/](https://worksinprogress.co/issue/the-united-states-needs-fewer-bus-stops/)

生成摘要时出错

---

## 19. RAM now represents 35 percent of bill of materials for HP PCs

**原文标题**: RAM now represents 35 percent of bill of materials for HP PCs

**原文链接**: [https://arstechnica.com/gadgets/2026/02/ram-now-represents-35-percent-of-bill-of-materials-for-hp-pcs/](https://arstechnica.com/gadgets/2026/02/ram-now-represents-35-percent-of-bill-of-materials-for-hp-pcs/)

生成摘要时出错

---

## 20. Nano Banana 2: Google's latest AI image generation model

**原文标题**: Nano Banana 2: Google's latest AI image generation model

**原文链接**: [https://blog.google/innovation-and-ai/technology/ai/nano-banana-2/](https://blog.google/innovation-and-ai/technology/ai/nano-banana-2/)

生成摘要时出错

---

## 21. Mercury 2: Fast reasoning LLM powered by diffusion

**原文标题**: Mercury 2: Fast reasoning LLM powered by diffusion

**原文链接**: [https://www.inceptionlabs.ai/blog/introducing-mercury-2](https://www.inceptionlabs.ai/blog/introducing-mercury-2)

生成摘要时出错

---

## 22. Windows 11 Notepad to support Markdown

**原文标题**: Windows 11 Notepad to support Markdown

**原文链接**: [https://blogs.windows.com/windows-insider/2026/01/21/notepad-and-paint-updates-begin-rolling-out-to-windows-insiders/](https://blogs.windows.com/windows-insider/2026/01/21/notepad-and-paint-updates-begin-rolling-out-to-windows-insiders/)

生成摘要时出错

---

## 23. Hacking an old Kindle to display bus arrival times

**原文标题**: Hacking an old Kindle to display bus arrival times

**原文链接**: [https://www.mariannefeng.com/portfolio/kindle/](https://www.mariannefeng.com/portfolio/kindle/)

生成摘要时出错

---

## 24. Show HN: Moonshine Open-Weights STT models – higher accuracy than WhisperLargev3

**原文标题**: Show HN: Moonshine Open-Weights STT models – higher accuracy than WhisperLargev3

**原文链接**: [https://github.com/moonshine-ai/moonshine](https://github.com/moonshine-ai/moonshine)

生成摘要时出错

---

## 25. Making MCP cheaper via CLI

**原文标题**: Making MCP cheaper via CLI

**原文链接**: [https://kanyilmaz.me/2026/02/23/cli-vs-mcp.html](https://kanyilmaz.me/2026/02/23/cli-vs-mcp.html)

生成摘要时出错

---

## 26. First Website (1992)

**原文标题**: First Website (1992)

**原文链接**: [https://info.cern.ch](https://info.cern.ch)

生成摘要时出错

---

## 27. The Om Programming Language

**原文标题**: The Om Programming Language

**原文链接**: [https://www.om-language.com/](https://www.om-language.com/)

生成摘要时出错

---

## 28. LLM=True

**原文标题**: LLM=True

**原文链接**: [https://blog.codemine.be/posts/2026/20260222-be-quiet/](https://blog.codemine.be/posts/2026/20260222-be-quiet/)

生成摘要时出错

---

## 29. AIs can't stop recommending nuclear strikes in war game simulations

**原文标题**: AIs can't stop recommending nuclear strikes in war game simulations

**原文链接**: [https://www.newscientist.com/article/2516885-ais-cant-stop-recommending-nuclear-strikes-in-war-game-simulations/](https://www.newscientist.com/article/2516885-ais-cant-stop-recommending-nuclear-strikes-in-war-game-simulations/)

生成摘要时出错

---

## 30. Show HN: Terminal Phone – E2EE Walkie Talkie from the Command Line

**原文标题**: Show HN: Terminal Phone – E2EE Walkie Talkie from the Command Line

**原文链接**: [https://gitlab.com/here_forawhile/terminalphone](https://gitlab.com/here_forawhile/terminalphone)

生成摘要时出错

---

## 31. AirSnitch: Demystifying and breaking client isolation in Wi-Fi networks [pdf]

**原文标题**: AirSnitch: Demystifying and breaking client isolation in Wi-Fi networks [pdf]

**原文链接**: [https://www.ndss-symposium.org/wp-content/uploads/2026-f1282-paper.pdf](https://www.ndss-symposium.org/wp-content/uploads/2026-f1282-paper.pdf)

生成摘要时出错

---

## 32. Show HN: I ported Tree-sitter to Go

**原文标题**: Show HN: I ported Tree-sitter to Go

**原文链接**: [https://github.com/odvcencio/gotreesitter](https://github.com/odvcencio/gotreesitter)

生成摘要时出错

---

## 33. Show HN: A real-time strategy game that AI agents can play

**原文标题**: Show HN: A real-time strategy game that AI agents can play

**原文链接**: [https://llmskirmish.com/](https://llmskirmish.com/)

生成摘要时出错

---

## 34. Show HN: Respectify – A comment moderator that teaches people to argue better

**原文标题**: Show HN: Respectify – A comment moderator that teaches people to argue better

**原文链接**: [https://respectify.org/](https://respectify.org/)

生成摘要时出错

---

## 35. US Military leaders meet with Anthropic to argue against Claude safeguards

**原文标题**: US Military leaders meet with Anthropic to argue against Claude safeguards

**原文链接**: [https://www.theguardian.com/us-news/2026/feb/24/anthropic-claude-military-ai](https://www.theguardian.com/us-news/2026/feb/24/anthropic-claude-military-ai)

生成摘要时出错

---

## 36. You Want to Visit the UK? You Better Have a Google Play or App Store Account

**原文标题**: You Want to Visit the UK? You Better Have a Google Play or App Store Account

**原文链接**: [https://www.heltweg.org/posts/you-want-to-visit-the-uk-you-better-have-a-google-play-or-app-store-account/](https://www.heltweg.org/posts/you-want-to-visit-the-uk-you-better-have-a-google-play-or-app-store-account/)

生成摘要时出错

---

## 37. In 2025, Meta paid an effective federal tax rate of 3.5%

**原文标题**: In 2025, Meta paid an effective federal tax rate of 3.5%

**原文链接**: [https://bsky.app/profile/rbreich.bsky.social/post/3mfptlfeucn2i](https://bsky.app/profile/rbreich.bsky.social/post/3mfptlfeucn2i)

生成摘要时出错

---

## 38. Looks like it is happening

**原文标题**: Looks like it is happening

**原文链接**: [https://www.math.columbia.edu/~woit/wordpress/?p=15500](https://www.math.columbia.edu/~woit/wordpress/?p=15500)

生成摘要时出错

---

## 39. GNU Texmacs

**原文标题**: GNU Texmacs

**原文链接**: [https://www.texmacs.org/tmweb/home/welcome.en.html](https://www.texmacs.org/tmweb/home/welcome.en.html)

生成摘要时出错

---

## 40. The Pentagon threatens Anthropic

**原文标题**: The Pentagon threatens Anthropic

**原文链接**: [https://www.astralcodexten.com/p/the-pentagon-threatens-anthropic](https://www.astralcodexten.com/p/the-pentagon-threatens-anthropic)

生成摘要时出错

---

## 41. 100M-Row Challenge with PHP

**原文标题**: 100M-Row Challenge with PHP

**原文链接**: [https://github.com/tempestphp/100-million-row-challenge](https://github.com/tempestphp/100-million-row-challenge)

生成摘要时出错

---

## 42. Cell Service for the Fairly Paranoid

**原文标题**: Cell Service for the Fairly Paranoid

**原文链接**: [https://www.cape.co/](https://www.cape.co/)

生成摘要时出错

---

## 43. Jane Street Hit with Terra $40B Insider Trading Suit

**原文标题**: Jane Street Hit with Terra $40B Insider Trading Suit

**原文链接**: [https://www.disruptionbanking.com/2026/02/24/jane-street-hit-with-terra-40b-insider-trading-suit/](https://www.disruptionbanking.com/2026/02/24/jane-street-hit-with-terra-40b-insider-trading-suit/)

生成摘要时出错

---

## 44. I don't know how you get here from “predict the next word”

**原文标题**: I don't know how you get here from “predict the next word”

**原文链接**: [https://www.grumpy-economist.com/p/refine](https://www.grumpy-economist.com/p/refine)

生成摘要时出错

---

## 45. The Misuses of the University

**原文标题**: The Misuses of the University

**原文链接**: [https://www.publicbooks.org/the-misuses-of-the-university/](https://www.publicbooks.org/the-misuses-of-the-university/)

生成摘要时出错

---

## 46. Racket v9.1

**原文标题**: Racket v9.1

**原文链接**: [https://blog.racket-lang.org/2026/02/racket-v9-1.html](https://blog.racket-lang.org/2026/02/racket-v9-1.html)

生成摘要时出错

---

## 47. Pentagon threatens to make Anthropic a pariah

**原文标题**: Pentagon threatens to make Anthropic a pariah

**原文链接**: [https://www.cnn.com/2026/02/24/tech/hegseth-anthropic-ai-military-amodei](https://www.cnn.com/2026/02/24/tech/hegseth-anthropic-ai-military-amodei)

生成摘要时出错

---

## 48. Open Source Endowment – new funding source for open source maintainers

**原文标题**: Open Source Endowment – new funding source for open source maintainers

**原文链接**: [https://endowment.dev/](https://endowment.dev/)

生成摘要时出错

---

## 49. Turing Completeness of GNU find

**原文标题**: Turing Completeness of GNU find

**原文链接**: [https://arxiv.org/abs/2602.20762](https://arxiv.org/abs/2602.20762)

生成摘要时出错

---

## 50. Why isn't LA repaving streets?

**原文标题**: Why isn't LA repaving streets?

**原文链接**: [https://lapublicpress.org/2026/02/why-isnt-la-repaving-streets/](https://lapublicpress.org/2026/02/why-isnt-la-repaving-streets/)

生成摘要时出错

---

## 51. Show HN: Django Control Room – All Your Tools Inside the Django Admin

**原文标题**: Show HN: Django Control Room – All Your Tools Inside the Django Admin

**原文链接**: [https://github.com/yassi/dj-control-room](https://github.com/yassi/dj-control-room)

生成摘要时出错

---

## 52. An autopsy of AI-generated 3D slop

**原文标题**: An autopsy of AI-generated 3D slop

**原文链接**: [https://aircada.com/blog/ai-vs-human-3d-ecommerce](https://aircada.com/blog/ai-vs-human-3d-ecommerce)

生成摘要时出错

---

## 53. Stripe reportedly makes offer to acquire PayPal

**原文标题**: Stripe reportedly makes offer to acquire PayPal

**原文链接**: [https://www.cnbc.com/2026/02/24/paypal-stock-stripe-acquisition-report.html](https://www.cnbc.com/2026/02/24/paypal-stock-stripe-acquisition-report.html)

生成摘要时出错

---

## 54. Learnings from 4 months of Image-Video VAE experiments

**原文标题**: Learnings from 4 months of Image-Video VAE experiments

**原文链接**: [https://www.linum.ai/field-notes/vae-reconstruction-vs-generation](https://www.linum.ai/field-notes/vae-reconstruction-vs-generation)

生成摘要时出错

---

## 55. Red Hat takes on Docker Desktop with its enterprise Podman Desktop build

**原文标题**: Red Hat takes on Docker Desktop with its enterprise Podman Desktop build

**原文链接**: [https://thenewstack.io/red-hat-enters-the-cloud-native-developer-desktop-market/](https://thenewstack.io/red-hat-enters-the-cloud-native-developer-desktop-market/)

生成摘要时出错

---

## 56. Show HN: Clocksimulator.com – A minimalist, distraction-free analog clock

**原文标题**: Show HN: Clocksimulator.com – A minimalist, distraction-free analog clock

**原文链接**: [https://www.clocksimulator.com/](https://www.clocksimulator.com/)

生成摘要时出错

---

## 57. Sandboxes won't save you from OpenClaw

**原文标题**: Sandboxes won't save you from OpenClaw

**原文链接**: [https://tachyon.so/blog/sandboxes-wont-save-you](https://tachyon.so/blog/sandboxes-wont-save-you)

生成摘要时出错

---

## 58. Will vibe coding end like the maker movement?

**原文标题**: Will vibe coding end like the maker movement?

**原文链接**: [https://read.technically.dev/p/vibe-coding-and-the-maker-movement](https://read.technically.dev/p/vibe-coding-and-the-maker-movement)

生成摘要时出错

---

## 59. The Slow Death of the Power User

**原文标题**: The Slow Death of the Power User

**原文链接**: [https://fireborn.mataroa.blog/blog/the-slow-death-of-the-power-user/](https://fireborn.mataroa.blog/blog/the-slow-death-of-the-power-user/)

生成摘要时出错

---

## 60. BuildKit: Docker's Hidden Gem That Can Build Almost Anything

**原文标题**: BuildKit: Docker's Hidden Gem That Can Build Almost Anything

**原文链接**: [https://tuananh.net/2026/02/25/buildkit-docker-hidden-gem/](https://tuananh.net/2026/02/25/buildkit-docker-hidden-gem/)

生成摘要时出错

---

## 61. Story of XZ Backdoor [video]

**原文标题**: Story of XZ Backdoor [video]

**原文链接**: [https://www.youtube.com/watch?v=aoag03mSuXQ](https://www.youtube.com/watch?v=aoag03mSuXQ)

生成摘要时出错

---

## 62. Bcachefs creator insists his custom LLM is female and 'fully conscious'

**原文标题**: Bcachefs creator insists his custom LLM is female and 'fully conscious'

**原文链接**: [https://www.theregister.com/2026/02/25/bcachefs_creator_ai/](https://www.theregister.com/2026/02/25/bcachefs_creator_ai/)

生成摘要时出错

---

## 63. Tuna: A new, modern, modal launcher for macOS

**原文标题**: Tuna: A new, modern, modal launcher for macOS

**原文链接**: [https://tunaformac.com](https://tunaformac.com)

生成摘要时出错

---

## 64. Americans Are Leaving the U.S. in Record Numbers

**原文标题**: Americans Are Leaving the U.S. in Record Numbers

**原文链接**: [https://www.wsj.com/us-news/americans-leaving-the-us-migration-a5795bfa](https://www.wsj.com/us-news/americans-leaving-the-us-migration-a5795bfa)

生成摘要时出错

---

## 65. Technical Excellence Is Not Enough

**原文标题**: Technical Excellence Is Not Enough

**原文链接**: [https://raccoon.land/posts/technical-excellence-is-not-enough/](https://raccoon.land/posts/technical-excellence-is-not-enough/)

生成摘要时出错

---

## 66. We are changing our developer productivity experiment design

**原文标题**: We are changing our developer productivity experiment design

**原文链接**: [https://metr.org/blog/2026-02-24-uplift-update/](https://metr.org/blog/2026-02-24-uplift-update/)

生成摘要时出错

---

## 67. Men in their 50s may be aging faster due to toxic 'forever chemicals'

**原文标题**: Men in their 50s may be aging faster due to toxic 'forever chemicals'

**原文链接**: [https://www.cnn.com/2026/02/26/health/forever-chemicals-aging-men-wellness](https://www.cnn.com/2026/02/26/health/forever-chemicals-aging-men-wellness)

生成摘要时出错

---

## 68. I asked Claude for 37,500 random names, and it can't stop saying Marcus

**原文标题**: I asked Claude for 37,500 random names, and it can't stop saying Marcus

**原文链接**: [https://github.com/benjismith/ai-randomness](https://github.com/benjismith/ai-randomness)

生成摘要时出错

---

## 69. just-bash: Bash for Agents

**原文标题**: just-bash: Bash for Agents

**原文链接**: [https://github.com/vercel-labs/just-bash](https://github.com/vercel-labs/just-bash)

生成摘要时出错

---

## 70. Google Street View in 2026

**原文标题**: Google Street View in 2026

**原文链接**: [https://tech.marksblogg.com/google-street-view-coverage.html](https://tech.marksblogg.com/google-street-view-coverage.html)

生成摘要时出错

---

## 71. What Happened to Fry's Electronics

**原文标题**: What Happened to Fry's Electronics

**原文链接**: [https://dfarq.homeip.net/what-happened-to-frys-electronics/](https://dfarq.homeip.net/what-happened-to-frys-electronics/)

生成摘要时出错

---

## 72. Show HN: Context Mode – 315 KB of MCP output becomes 5.4 KB in Claude Code

**原文标题**: Show HN: Context Mode – 315 KB of MCP output becomes 5.4 KB in Claude Code

**原文链接**: [https://github.com/mksglu/claude-context-mode](https://github.com/mksglu/claude-context-mode)

生成摘要时出错

---

## 73. Palm OS User Interface Guidelines (2003) [pdf]

**原文标题**: Palm OS User Interface Guidelines (2003) [pdf]

**原文链接**: [https://cs.uml.edu/~fredm/courses/91.308-spr05/files/palmdocs/uiguidelines.pdf](https://cs.uml.edu/~fredm/courses/91.308-spr05/files/palmdocs/uiguidelines.pdf)

生成摘要时出错

---

## 74. Amazon would rather blame its own engineers than its AI

**原文标题**: Amazon would rather blame its own engineers than its AI

**原文链接**: [https://www.theregister.com/2026/02/24/amazon_blame_human_not_ai/](https://www.theregister.com/2026/02/24/amazon_blame_human_not_ai/)

生成摘要时出错

---

## 75. Twitch: "Hey, come back! This commercial break can't play while you're away."

**原文标题**: Twitch: "Hey, come back! This commercial break can't play while you're away."

**原文链接**: [https://twitter.com/KryDotExe/status/2026806591517856208](https://twitter.com/KryDotExe/status/2026806591517856208)

生成摘要时出错

---

## 76. Leaked Documents Show Meta Cracking Down on Access to Abortion Information

**原文标题**: Leaked Documents Show Meta Cracking Down on Access to Abortion Information

**原文链接**: [https://www.motherjones.com/politics/2026/02/meta-abortion-ai-chatbot-leak-teen-info-ban/](https://www.motherjones.com/politics/2026/02/meta-abortion-ai-chatbot-leak-teen-info-ban/)

生成摘要时出错

---

## 77. Large-scale online deanonymization with LLMs

**原文标题**: Large-scale online deanonymization with LLMs

**原文链接**: [https://arxiv.org/abs/2602.16800](https://arxiv.org/abs/2602.16800)

生成摘要时出错

---

## 78. LibreOffice resumes work on its self-hosted Google Docs alternative

**原文标题**: LibreOffice resumes work on its self-hosted Google Docs alternative

**原文链接**: [https://www.xda-developers.com/libreoffice-resumes-work-on-its-self-hosted-google-docs-alternative/](https://www.xda-developers.com/libreoffice-resumes-work-on-its-self-hosted-google-docs-alternative/)

生成摘要时出错

---

## 79. Fed's Cook says AI triggering big changes, sees possible unemployment rise

**原文标题**: Fed's Cook says AI triggering big changes, sees possible unemployment rise

**原文链接**: [https://www.reuters.com/business/feds-cook-says-ai-triggering-big-changes-sees-possible-short-term-unemployment-2026-02-24/](https://www.reuters.com/business/feds-cook-says-ai-triggering-big-changes-sees-possible-short-term-unemployment-2026-02-24/)

生成摘要时出错

---

## 80. Manjaro website off-line again due to lapsed certificate

**原文标题**: Manjaro website off-line again due to lapsed certificate

**原文链接**: [https://distrowatch.com/dwres.php?resource=showheadline&story=20140](https://distrowatch.com/dwres.php?resource=showheadline&story=20140)

生成摘要时出错

---

## 81. Show HN: Agent Swarm – Multi-agent self-learning teams (OSS)

**原文标题**: Show HN: Agent Swarm – Multi-agent self-learning teams (OSS)

**原文链接**: [https://github.com/desplega-ai/agent-swarm](https://github.com/desplega-ai/agent-swarm)

生成摘要时出错

---

## 82. Origin of the rule that swap size should be 2x of the physical memory

**原文标题**: Origin of the rule that swap size should be 2x of the physical memory

**原文链接**: [https://retrocomputing.stackexchange.com/questions/32492/origin-of-the-rule-that-swap-size-should-be-2x-of-the-physical-memory](https://retrocomputing.stackexchange.com/questions/32492/origin-of-the-rule-that-swap-size-should-be-2x-of-the-physical-memory)

生成摘要时出错

---

## 83. Number of UK workers on zero-hours contracts hits record high ahead of crackdown

**原文标题**: Number of UK workers on zero-hours contracts hits record high ahead of crackdown

**原文链接**: [https://www.bbc.co.uk/news/articles/czj1m7d4gxpo](https://www.bbc.co.uk/news/articles/czj1m7d4gxpo)

生成摘要时出错

---

## 84. Fentanyl makeover: Core structural redesign could lead to safer pain medications

**原文标题**: Fentanyl makeover: Core structural redesign could lead to safer pain medications

**原文链接**: [https://www.scripps.edu/news-and-events/press-room/2026/20260211-janda-molecule.html](https://www.scripps.edu/news-and-events/press-room/2026/20260211-janda-molecule.html)

生成摘要时出错

---

## 85. The Pentagon Feuding with an AI Company Is a Bad Sign

**原文标题**: The Pentagon Feuding with an AI Company Is a Bad Sign

**原文链接**: [https://foreignpolicy.com/2026/02/25/anthropic-pentagon-feud-ai/](https://foreignpolicy.com/2026/02/25/anthropic-pentagon-feud-ai/)

生成摘要时出错

---

## 86. RK3588 and RK3576 video decoders support merged in the upstream Linux Kernel

**原文标题**: RK3588 and RK3576 video decoders support merged in the upstream Linux Kernel

**原文链接**: [https://www.collabora.com/news-and-blog/news-and-events/rk3588-and-rk3576-video-decoders-support-merged-in-the-upstream-linux-kernel.html](https://www.collabora.com/news-and-blog/news-and-events/rk3588-and-rk3576-video-decoders-support-merged-in-the-upstream-linux-kernel.html)

生成摘要时出错

---

## 87. SynthID

**原文标题**: SynthID

**原文链接**: [https://deepmind.google/models/synthid/](https://deepmind.google/models/synthid/)

生成摘要时出错

---

## 88. LibreOffice Online: A Fresh Start

**原文标题**: LibreOffice Online: A Fresh Start

**原文链接**: [https://blog.documentfoundation.org/blog/2026/02/24/libreoffice-online-a-fresh-start/](https://blog.documentfoundation.org/blog/2026/02/24/libreoffice-online-a-fresh-start/)

生成摘要时出错

---

## 89. SynthID

**原文标题**: SynthID

**原文链接**: [https://deepmind.google/models/synthid/](https://deepmind.google/models/synthid/)

生成摘要时出错

---

## 90. Burger King will use AI to check if employees say 'please' and 'thank you'

**原文标题**: Burger King will use AI to check if employees say 'please' and 'thank you'

**原文链接**: [https://www.theverge.com/ai-artificial-intelligence/884911/burger-king-ai-assistant-patty](https://www.theverge.com/ai-artificial-intelligence/884911/burger-king-ai-assistant-patty)

生成摘要时出错

---

## 91. Ed Zitron loses his mind annotating an AI doomer macro memo

**原文标题**: Ed Zitron loses his mind annotating an AI doomer macro memo

**原文链接**: [https://www.dropbox.com/scl/fi/1p1n0y1ip48ianok9dvbp/Annotation-The-Global-Intelligence-Crisis.pdf?dl=0&e=1&noscript=1&rlkey=qaar8ea6l5hh6jqls4x6g8q4b](https://www.dropbox.com/scl/fi/1p1n0y1ip48ianok9dvbp/Annotation-The-Global-Intelligence-Crisis.pdf?dl=0&e=1&noscript=1&rlkey=qaar8ea6l5hh6jqls4x6g8q4b)

生成摘要时出错

---

## 92. iPhone and iPad approved to handle classified NATO information

**原文标题**: iPhone and iPad approved to handle classified NATO information

**原文链接**: [https://www.apple.com/newsroom/2026/02/iphone-and-ipad-approved-to-handle-classified-nato-information/](https://www.apple.com/newsroom/2026/02/iphone-and-ipad-approved-to-handle-classified-nato-information/)

生成摘要时出错

---

## 93. Launch HN: TeamOut (YC W22) – AI agent for planning company retreats

**原文标题**: Launch HN: TeamOut (YC W22) – AI agent for planning company retreats

**原文链接**: [https://app.teamout.com/ai](https://app.teamout.com/ai)

生成摘要时出错

---

## 94. 去虚拟化与静态多态

**原文标题**: Devirtualization and Static Polymorphism

**原文链接**: [https://david.alvarezrosa.com/posts/devirtualization-and-static-polymorphism/](https://david.alvarezrosa.com/posts/devirtualization-and-static-polymorphism/)

生成摘要时出错

---

## 95. Why Developers Keep Choosing Claude over Every Other AI

**原文标题**: Why Developers Keep Choosing Claude over Every Other AI

**原文链接**: [https://www.bhusalmanish.com.np/blog/posts/why-claude-wins-coding.html](https://www.bhusalmanish.com.np/blog/posts/why-claude-wins-coding.html)

生成摘要时出错

---

## 96. Why High FOV Sucks – Fixing It with Panini Projection

**原文标题**: Why High FOV Sucks – Fixing It with Panini Projection

**原文链接**: [https://www.youtube.com/watch?v=LE9kxUQ-l14](https://www.youtube.com/watch?v=LE9kxUQ-l14)

生成摘要时出错

---

## 97. Palantir Built the Data Layer That Right to Erasure Can't Touch

**原文标题**: Palantir Built the Data Layer That Right to Erasure Can't Touch

**原文链接**: [https://frontierlabs.substack.com/p/the-ai-is-the-last-thing-to-worry](https://frontierlabs.substack.com/p/the-ai-is-the-last-thing-to-worry)

生成摘要时出错

---

## 98. Anthropic digs in heels in dispute with Pentagon

**原文标题**: Anthropic digs in heels in dispute with Pentagon

**原文链接**: [https://www.reuters.com/world/anthropic-digs-heels-dispute-with-pentagon-source-says-2026-02-24/](https://www.reuters.com/world/anthropic-digs-heels-dispute-with-pentagon-source-says-2026-02-24/)

生成摘要时出错

---

## 99. Larry Page has moved to Florida

**原文标题**: Larry Page has moved to Florida

**原文链接**: [https://twitter.com/paulg/status/2026737030257062253](https://twitter.com/paulg/status/2026737030257062253)

生成摘要时出错

---

## 100. Tech Firms Aren't Just Encouraging Their Workers to Use AI. They're Enforcing It

**原文标题**: Tech Firms Aren't Just Encouraging Their Workers to Use AI. They're Enforcing It

**原文链接**: [https://www.wsj.com/tech/ai/tech-firms-arent-just-encouraging-their-workers-to-use-ai-theyre-enforcing-it-d43ebf84](https://www.wsj.com/tech/ai/tech-firms-arent-just-encouraging-their-workers-to-use-ai-theyre-enforcing-it-d43ebf84)

生成摘要时出错

---

