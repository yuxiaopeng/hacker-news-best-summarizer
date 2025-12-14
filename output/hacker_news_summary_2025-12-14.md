# Hacker News 热门文章摘要 (2025-12-14)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 我的Apple ID被苹果锁定了，我束手无策。求助。

**原文标题**: Apple has locked my Apple ID, and I have no recourse. A plea for help

**原文链接**: [https://hey.paris/posts/appleid/](https://hey.paris/posts/appleid/)

忠实的苹果用户兼专业开发者帕里斯报告称，他拥有25年之久的Apple ID已被永久锁定，这事实上已使他的数字生活陷入瘫痪，并导致其价值超过3万美元的苹果硬件形同废铁。该问题源于他尝试兑换一张价值500美元的苹果礼品卡，这张卡购自一家大型实体零售店，但据苹果公司称，该卡被标记为已被盗用。

此举已导致他的iPhone、iPad、Mac电脑和Apple Watch基本无法使用，并阻止了他访问数TB的家庭照片、消息历史记录以及数千美元的已购软件和媒体内容。他无法退出iCloud、无法使用iMessage、无法下载他的数据，也无法访问许多需要活跃Apple ID的苹果支持系统。

苹果支持部门没有提供任何关于此次封禁的解释，拒绝升级处理，并且不屑一顾地建议他“创建一个新的Apple账户”。这一建议是灾难性的，存在硬件被标记、因规避安全措施而导致账户进一步被禁用，以及他作为一名苹果开发者可能被列入黑名单的风险。

作为苹果编程语言技术书籍的作者和大型开发者活动的组织者，帕里斯强调了他长期以来对苹果生态系统的投入。他认为，是自动欺诈标记错误地触发了这种“核打击”，他恳求对他的案件进行人工审查，以恢复他的数字身份和访问权限。

---

## 2. OpenAI正在悄悄采用技能，现已在ChatGPT和Codex CLI中可用

**原文标题**: OpenAI are quietly adopting skills, now available in ChatGPT and Codex CLI

**原文链接**: [https://simonwillison.net/2025/Dec/12/openai-skills/](https://simonwillison.net/2025/Dec/12/openai-skills/)

OpenAI正在悄然整合一套类似于Anthropic的“技能”机制，到ChatGPT的Code Interpreter（代码解释器）和其Codex CLI工具中，截至2025年12月。这一采用验证了作者之前将技能视为AI重大发展的评估。

技能被构造成文件夹，包含一个Markdown文件（`skill.md`）和可选的资源/脚本，使大型语言模型（LLM）易于实现。

在**ChatGPT**中，技能可以通过`/home/oai/skills`文件夹在Code Interpreter（代码解释器）内部访问。当前技能涵盖电子表格、DOCX和PDF。值得注意的是，对于PDF和文档，OpenAI将页面转换为PNG，利用支持视觉的GPT模型来保留布局和图形，而不仅仅是提取文本。一个示例展示了GPT-5.2精心创建了一份关于新西兰红松（rimu trees）和鸮鹦鹉（kakapo）的PDF，甚至能自我纠正长音符号（macrons）的字体问题。

对于**Codex CLI**，两周前引入了技能的实验性支持。用户可以将技能安装到`~/.codex/skills`中，并通过`--enable skills`选项激活它们。一个示例展示了使用自定义技能完美生成了一个Datasette插件。

文章强调，OpenAI迅速采纳这种“轻量级规范”进一步证实了技能概念的强大。作者建议，对技能规范进行正式文档化将大有裨益，这可能由Agentic AI Foundation牵头。

---

## 3. 欧洲健康数据售予前以色列间谍掌管的美国公司

**原文标题**: Europeans' health data sold to US firm run by ex-Israeli spies

**原文链接**: [https://www.ftm.eu/articles/europe-health-data-us-firm-israel-spies](https://www.ftm.eu/articles/europe-health-data-us-firm-israel-spies)

欧洲通讯服务Zivver，被欧盟和英国政府、医院及法院用于机密通讯，现已被出售给一家与以色列情报机构有密切联系的美国公司Kiteworks，这引发了严重关切。

荷兰公司Zivver，经调查发现，尽管声称“零访问”，但其能够读取客户的“加密”内容。这意味着包括医疗和政府通讯在内的敏感欧洲数据，Zivver本身就已经可能访问。

Kiteworks的此次收购带来了两个主要问题：
1.  **美国司法管辖权：** 这些数据现在受制于侵入性的美国法律，这意味着无论数据存储在哪里，美国政府都可以要求访问。
2.  **与以色列情报机构的联系：** Kiteworks的首席执行官乔纳森·亚伦（Jonathan Yaron）和几位高级管理人员都曾是以色列精英军事情报8200部队的成员，该部队以窃听闻名。专家警告称，以色列情报机构与科技行业之间存在“旋转门”现象，这造成了一个漏洞，Zivver的敏感数据“金矿”可能被外国情报机构利用。

荷兰当局未能阻止或适当评估此次收购，将Zivver归类为非关键基础设施——专家称这一决定是“巨大失误”。批评人士强调，欧洲对其数字基础设施缺乏战略控制，呼吁加强监管，以保护重要的通讯服务免受外国影响和潜在的数据滥用。

---

## 4. macOS 26.2 通过 Thunderbolt RDMA 实现快速 AI 集群

**原文标题**: macOS 26.2 enables fast AI clusters with RDMA over Thunderbolt

**原文链接**: [https://developer.apple.com/documentation/macos-release-notes/macos-26_2-release-notes#RDMA-over-Thunderbolt](https://developer.apple.com/documentation/macos-release-notes/macos-26_2-release-notes#RDMA-over-Thunderbolt)

标题为“macOS 26.2 enables fast AI clusters with RDMA over Thunderbolt”的文章内容无法访问。页面没有显示文章，而是显示了一条错误消息，表明需要JavaScript才能查看其内容。

因此，无法提供关于macOS 26.2、其实现快速AI集群的能力以及通过Thunderbolt使用RDMA的实际文章内容的摘要。根据输入，文章本身的要点和关键信息均无法获取。

---

## 5. VPN宣称的位置与实际流量出口不符

**原文标题**: VPN location claims don't match real traffic exits

**原文链接**: [https://ipinfo.io/blog/vpn-location-mismatch-report](https://ipinfo.io/blog/vpn-location-mismatch-report)

IPinfo 的研究显示，在 20 个热门 VPN 中，有 17 个谎报了其流量出口位置。通过分析 137 个国家/地区的 15 万个出口 IP，他们发现许多提供商声称支持超过 100 个国家/地区，但实际上却通过少数几个物理数据中心（主要位于美国或欧洲）路由流量。其中有 38 个声称的国家/地区是“纯虚拟”的，意味着没有实际流量从这些地方出口。只有 Mullvad、IVPN 和 Windscribe 展现了完全可验证的位置。

当 VPN 应用甚至 IP 注册数据声称是“国家 X”，但活跃网络测量却显示流量从“国家 Y”出口时，就会出现虚拟位置，两者通常相隔数千公里（例如，巴哈马的流量从美国出口，索马里的流量从法国/英国出口）。传统的 IP 数据提供商常常依赖于自报数据，从而延续了这些错误，其位置中位数误差高达 3100 公里。

尽管虚拟位置存在技术原因（风险、成本），但缺乏透明度和大规模的不匹配现象造成了严重的信任问题，影响了用户、记者和反欺诈系统。IPinfo 通过“测量优先”的方法来解决这个问题，利用其 ProbeNet（1200 多个全球 PoP）进行主动 RTT 测量，以验证真实的物理位置。用户应对过长的国家列表持怀疑态度，并寻找透明标注虚拟位置的提供商。

---

## 6. 老鼠玩毁灭战士

**原文标题**: Rats Play DOOM

**原文链接**: [https://ratsplaydoom.com/](https://ratsplaydoom.com/)

《老鼠玩DOOM》一文详细介绍了一种专门为老鼠设计用于玩电子游戏的头戴设备，强调其独特的视觉界面和集成的感官功能。该头显能牢固地环绕老鼠的头部，集成一个可折叠的AMOLED屏幕，提供全高清分辨率以实现最大沉浸感，同时确保老鼠的胡须不受阻碍。

除了显示屏，该头显还集成了几个关键的感官组件。它在左右胡须附近设有两个小型气嘴，能够提供定向气流，以提示游戏内事件，例如撞墙。框架还为奖励系统的分配管提供了一个牢固的安装点，将其方便地定位在老鼠嘴巴附近。此外，该设计还在每只耳朵附近预留了微型立体声扬声器的安装位置，表明未来有集成音频提示的计划。该描述还辅以对视觉辅助材料的引用，例如“头显特写”和“3D模型：头显”。

---

## 7. GNU 统一字体

**原文标题**: GNU Unifont

**原文链接**: [https://unifoundry.com/unifont/index.html](https://unifoundry.com/unifont/index.html)

GNU Unifont 是一个 GNU 项目字体，提供对可打印 Unicode 码点的全面覆盖，主要涵盖基本多文种平面 (BMP)，并日益支持辅助多文种平面 (SMP) 和 ConScript Unicode 注册表 (CSUR)。

它采用双重许可，即附带 GNU 字体嵌入例外条款的 GNU GPLv2+ 许可和 SIL 开放字体许可 1.1。此许可明确允许商业使用，确保派生字体保持自由，并鸣谢志愿者贡献者。

Unifont 提供 OpenType、PCF、BDF、PSF 和 HEX 等多种格式下载，并提供针对日文、更高 Unicode 平面和 CSUR 字形的专门版本。Windows 和 Mac OS X 用户可以将未压缩的字体文件安装到其系统的“字体”文件夹中。在 Mac 终端上，为了实现正确显示，可能需要启用抗锯齿功能。

Unifont 的一个显著局限是每个码点只存储一个字形。这使其不太适合需要上下文塑形、连字或浮动元音标记才能准确显示的复杂文字系统（如印度语系或阿拉伯语系文字）。对于这些文字系统，它通常作为“最后的备用字体”使用。

开发工作持续进行，众多贡献者在所有 Unicode 平面添加和修改字形。近期发布的版本（例如 17.0、16.0）详细说明了广泛的更新，包括对中文、阿拉伯文、格鲁吉亚文、古突厥文和表情符号字形的改进，以及新增的文字和符号。鼓励希望贡献新字形的志愿者提前联系项目组协调工作，需注意受中华人民共和国版权保护的 CJK 字形不能包含在该自由字体中。

---

## 8. I tried Gleam for Advent of Code

**原文标题**: I tried Gleam for Advent of Code

**原文链接**: [https://blog.tymscar.com/posts/gleamaoc2025/](https://blog.tymscar.com/posts/gleamaoc2025/)

生成摘要时出错

---

## 9. Linux Sandboxes and Fil-C

**原文标题**: Linux Sandboxes and Fil-C

**原文链接**: [https://fil-c.org/seccomp](https://fil-c.org/seccomp)

生成摘要时出错

---

## 10. Recovering Anthony Bourdain's Li.st's

**原文标题**: Recovering Anthony Bourdain's Li.st's

**原文链接**: [https://sandyuraz.com/blogs/bourdain/](https://sandyuraz.com/blogs/bourdain/)

生成摘要时出错

---

## 11. Google removes Sci-Hub domains from U.S. search results due to dated court order

**原文标题**: Google removes Sci-Hub domains from U.S. search results due to dated court order

**原文链接**: [https://torrentfreak.com/google-removes-sci-hub-domains-from-u-s-search-results-due-to-dated-court-order/](https://torrentfreak.com/google-removes-sci-hub-domains-from-u-s-search-results-due-to-dated-court-order/)

生成摘要时出错

---

## 12. I fed 24 years of my blog posts to a Markov model

**原文标题**: I fed 24 years of my blog posts to a Markov model

**原文链接**: [https://susam.net/fed-24-years-of-posts-to-markov-model.html](https://susam.net/fed-24-years-of-posts-to-markov-model.html)

生成摘要时出错

---

## 13. Why Twilio Segment moved from microservices back to a monolith

**原文标题**: Why Twilio Segment moved from microservices back to a monolith

**原文链接**: [https://www.twilio.com/en-us/blog/developers/best-practices/goodbye-microservices](https://www.twilio.com/en-us/blog/developers/best-practices/goodbye-microservices)

生成摘要时出错

---

## 14. 1300 Still Images from the Animated Films of Hayao Miyazaki's Studio Ghibli (2023)

**原文标题**: 1300 Still Images from the Animated Films of Hayao Miyazaki's Studio Ghibli (2023)

**原文链接**: [https://www.ghibli.jp/info/013772/](https://www.ghibli.jp/info/013772/)

生成摘要时出错

---

## 15. YouTube's CEO limits his kids' social media use – other tech bosses do the same

**原文标题**: YouTube's CEO limits his kids' social media use – other tech bosses do the same

**原文链接**: [https://www.cnbc.com/2025/12/13/youtubes-ceo-is-latest-tech-boss-limiting-his-kids-social-media-use.html](https://www.cnbc.com/2025/12/13/youtubes-ceo-is-latest-tech-boss-limiting-his-kids-social-media-use.html)

生成摘要时出错

---

## 16. An off-grid, flat-packable washing machine

**原文标题**: An off-grid, flat-packable washing machine

**原文链接**: [https://www.positive.news/society/flat-pack-washing-machine-spins-a-fairer-future/](https://www.positive.news/society/flat-pack-washing-machine-spins-a-fairer-future/)

生成摘要时出错

---

## 17. Show HN: Tiny VM sandbox in C with apps in Rust, C and Zig

**原文标题**: Show HN: Tiny VM sandbox in C with apps in Rust, C and Zig

**原文链接**: [https://github.com/ringtailsoftware/uvm32](https://github.com/ringtailsoftware/uvm32)

生成摘要时出错

---

## 18. LG TV's new software update installed MS Copilot, which cannot be deleted

**原文标题**: LG TV's new software update installed MS Copilot, which cannot be deleted

**原文链接**: [https://old.reddit.com/r/mildlyinfuriating/comments/1plldqo/my_lg_tvs_new_software_update_installed_microsoft/](https://old.reddit.com/r/mildlyinfuriating/comments/1plldqo/my_lg_tvs_new_software_update_installed_microsoft/)

生成摘要时出错

---

## 19. Benn Jordan’s flock camera jammer will send you to jail in Florida now [video]

**原文标题**: Benn Jordan’s flock camera jammer will send you to jail in Florida now [video]

**原文链接**: [https://www.youtube.com/watch?v=qEllWdK4l_A](https://www.youtube.com/watch?v=qEllWdK4l_A)

生成摘要时出错

---

## 20. Want to sway an election? Here’s how much fake online accounts cost

**原文标题**: Want to sway an election? Here’s how much fake online accounts cost

**原文链接**: [https://www.science.org/content/article/want-sway-election-here-s-how-much-fake-online-accounts-cost](https://www.science.org/content/article/want-sway-election-here-s-how-much-fake-online-accounts-cost)

生成摘要时出错

---

## 21. Are we stuck with the same Desktop UX forever? [video]

**原文标题**: Are we stuck with the same Desktop UX forever? [video]

**原文链接**: [https://www.youtube.com/watch?v=1fZTOjd_bOQ](https://www.youtube.com/watch?v=1fZTOjd_bOQ)

生成摘要时出错

---

## 22. AI and the ironies of automation – Part 2

**原文标题**: AI and the ironies of automation – Part 2

**原文链接**: [https://www.ufried.com/blog/ironies_of_ai_2/](https://www.ufried.com/blog/ironies_of_ai_2/)

生成摘要时出错

---

## 23. Some surprising things about DuckDuckGo

**原文标题**: Some surprising things about DuckDuckGo

**原文链接**: [https://gabrielweinberg.com/p/some-surprising-things-about-duckduckgo](https://gabrielweinberg.com/p/some-surprising-things-about-duckduckgo)

生成摘要时出错

---

## 24. The true story of the Windows 3.1 'Hot Dog Stand' color scheme

**原文标题**: The true story of the Windows 3.1 'Hot Dog Stand' color scheme

**原文链接**: [https://www.pcgamer.com/software/windows/windows-3-1-included-a-red-and-yellow-hot-dog-stand-color-scheme-so-garish-it-was-long-assumed-to-be-a-joke-so-i-tracked-down-the-original-designer-to-get-the-true-story/](https://www.pcgamer.com/software/windows/windows-3-1-included-a-red-and-yellow-hot-dog-stand-color-scheme-so-garish-it-was-long-assumed-to-be-a-joke-so-i-tracked-down-the-original-designer-to-get-the-true-story/)

生成摘要时出错

---

## 25. Kimi K2 1T model runs on 2 512GB M3 Ultras

**原文标题**: Kimi K2 1T model runs on 2 512GB M3 Ultras

**原文链接**: [https://twitter.com/awnihannun/status/1943723599971443134](https://twitter.com/awnihannun/status/1943723599971443134)

生成摘要时出错

---

## 26. 50 years of proof assistants

**原文标题**: 50 years of proof assistants

**原文链接**: [https://lawrencecpaulson.github.io//2025/12/05/History_of_Proof_Assistants.html](https://lawrencecpaulson.github.io//2025/12/05/History_of_Proof_Assistants.html)

生成摘要时出错

---

## 27. Analysis finds anytime electricity from solar available as battery costs plummet

**原文标题**: Analysis finds anytime electricity from solar available as battery costs plummet

**原文链接**: [https://pv-magazine-usa.com/2025/12/12/analysis-finds-anytime-electricity-from-solar-available-as-battery-costs-plummet/](https://pv-magazine-usa.com/2025/12/12/analysis-finds-anytime-electricity-from-solar-available-as-battery-costs-plummet/)

生成摘要时出错

---

## 28. Doxers posing as cops are tricking big tech firms into sharing people's data

**原文标题**: Doxers posing as cops are tricking big tech firms into sharing people's data

**原文链接**: [https://www.wired.com/story/doxers-posing-as-cops-are-tricking-big-tech-firms-into-sharing-peoples-private-data/](https://www.wired.com/story/doxers-posing-as-cops-are-tricking-big-tech-firms-into-sharing-peoples-private-data/)

生成摘要时出错

---

## 29. We built another object storage

**原文标题**: We built another object storage

**原文链接**: [https://fractalbits.com/blog/why-we-built-another-object-storage/](https://fractalbits.com/blog/why-we-built-another-object-storage/)

生成摘要时出错

---

## 30. If a Meta AI model can read a brain-wide signal, why wouldn't the brain?

**原文标题**: If a Meta AI model can read a brain-wide signal, why wouldn't the brain?

**原文链接**: [https://1393.xyz/writing/if-a-meta-ai-model-can-read-a-brain-wide-signal-why-wouldnt-the-brain](https://1393.xyz/writing/if-a-meta-ai-model-can-read-a-brain-wide-signal-why-wouldnt-the-brain)

生成摘要时出错

---

## 31. The Rise of Computer Games, Part I: Adventure

**原文标题**: The Rise of Computer Games, Part I: Adventure

**原文链接**: [https://technicshistory.com/2025/12/13/the-rise-of-computer-games-part-i-adventure/](https://technicshistory.com/2025/12/13/the-rise-of-computer-games-part-i-adventure/)

生成摘要时出错

---

## 32. Apple Maps claims it's 29,905 miles away

**原文标题**: Apple Maps claims it's 29,905 miles away

**原文链接**: [https://mathstodon.xyz/@dpiponi/115651419771418748](https://mathstodon.xyz/@dpiponi/115651419771418748)

生成摘要时出错

---

## 33. The Gorman Paradox: Where Are All the AI-Generated Apps?

**原文标题**: The Gorman Paradox: Where Are All the AI-Generated Apps?

**原文链接**: [https://codemanship.wordpress.com/2025/12/14/the-gorman-paradox-where-are-all-the-ai-generated-apps/](https://codemanship.wordpress.com/2025/12/14/the-gorman-paradox-where-are-all-the-ai-generated-apps/)

生成摘要时出错

---

## 34. Bye, Mom

**原文标题**: Bye, Mom

**原文链接**: [https://aella.substack.com/p/bye-mom](https://aella.substack.com/p/bye-mom)

生成摘要时出错

---

## 35. “You should never build a CMS”

**原文标题**: “You should never build a CMS”

**原文链接**: [https://www.sanity.io/blog/you-should-never-build-a-cms](https://www.sanity.io/blog/you-should-never-build-a-cms)

生成摘要时出错

---

## 36. Dick Van Dyke turns 100

**原文标题**: Dick Van Dyke turns 100

**原文链接**: [https://www.theguardian.com/film/2025/dec/13/dick-van-dyke-centenarian-100-mary-poppins-chitty-chitty-bang-bang](https://www.theguardian.com/film/2025/dec/13/dick-van-dyke-centenarian-100-mary-poppins-chitty-chitty-bang-bang)

生成摘要时出错

---

## 37. Shai-Hulud compromised a dev machine and raided GitHub org access: a post-mortem

**原文标题**: Shai-Hulud compromised a dev machine and raided GitHub org access: a post-mortem

**原文链接**: [https://trigger.dev/blog/shai-hulud-postmortem](https://trigger.dev/blog/shai-hulud-postmortem)

生成摘要时出错

---

## 38. Heavy metal is healing teens on the Blackfeet Nation

**原文标题**: Heavy metal is healing teens on the Blackfeet Nation

**原文链接**: [https://www.hcn.org/issues/57-11/heavy-metal-is-healing-teens-on-the-blackfeet-nation/](https://www.hcn.org/issues/57-11/heavy-metal-is-healing-teens-on-the-blackfeet-nation/)

生成摘要时出错

---

## 39. A Lisp Interpreter Implemented in Conway's Game of Life (2021)

**原文标题**: A Lisp Interpreter Implemented in Conway's Game of Life (2021)

**原文链接**: [https://woodrush.github.io/blog/posts/2022-01-12-lisp-in-life.html](https://woodrush.github.io/blog/posts/2022-01-12-lisp-in-life.html)

生成摘要时出错

---

## 40. Hashcards: A Plain-Text Spaced Repetition System

**原文标题**: Hashcards: A Plain-Text Spaced Repetition System

**原文链接**: [https://borretti.me/article/hashcards-plain-text-spaced-repetition](https://borretti.me/article/hashcards-plain-text-spaced-repetition)

生成摘要时出错

---

## 41. Closures as Win32 Window Procedures

**原文标题**: Closures as Win32 Window Procedures

**原文链接**: [https://nullprogram.com/blog/2025/12/12/](https://nullprogram.com/blog/2025/12/12/)

生成摘要时出错

---

## 42. Security issues with electronic invoices

**原文标题**: Security issues with electronic invoices

**原文链接**: [https://invoice.secvuln.info/](https://invoice.secvuln.info/)

生成摘要时出错

---

## 43. The Checkerboard

**原文标题**: The Checkerboard

**原文链接**: [https://99percentinvisible.org/episode/650-the-checkerboard/](https://99percentinvisible.org/episode/650-the-checkerboard/)

生成摘要时出错

---

## 44. Capsudo: Rethinking sudo with object capabilities

**原文标题**: Capsudo: Rethinking sudo with object capabilities

**原文链接**: [https://ariadne.space/2025/12/12/rethinking-sudo-with-object-capabilities.html](https://ariadne.space/2025/12/12/rethinking-sudo-with-object-capabilities.html)

生成摘要时出错

---

## 45. Poor Johnny still won't encrypt

**原文标题**: Poor Johnny still won't encrypt

**原文链接**: [https://bfswa.substack.com/p/poor-johnny-still-wont-encrypt](https://bfswa.substack.com/p/poor-johnny-still-wont-encrypt)

生成摘要时出错

---

## 46. Workday project at Washington University hits $266M

**原文标题**: Workday project at Washington University hits $266M

**原文链接**: [https://www.theregister.com/2025/12/12/washington_university_workday_costs_revealed/](https://www.theregister.com/2025/12/12/washington_university_workday_costs_revealed/)

生成摘要时出错

---

## 47. New Kindle feature uses AI to answer questions about books

**原文标题**: New Kindle feature uses AI to answer questions about books

**原文链接**: [https://reactormag.com/new-kindle-feature-ai-answer-questions-books-authors/](https://reactormag.com/new-kindle-feature-ai-answer-questions-books-authors/)

生成摘要时出错

---

## 48. Tesla US sales drop to nearly 4-year low in November

**原文标题**: Tesla US sales drop to nearly 4-year low in November

**原文链接**: [https://www.reuters.com/business/autos-transportation/tesla-us-sales-drop-nearly-3-year-low-november-despite-launch-cheaper-versions-2025-12-11/](https://www.reuters.com/business/autos-transportation/tesla-us-sales-drop-nearly-3-year-low-november-despite-launch-cheaper-versions-2025-12-11/)

生成摘要时出错

---

## 49. An Implementation of J (1992)

**原文标题**: An Implementation of J (1992)

**原文链接**: [https://www.jsoftware.com/ioj/ioj.htm](https://www.jsoftware.com/ioj/ioj.htm)

生成摘要时出错

---

## 50. Oliver Sacks put himself into his case studies. What was the cost?

**原文标题**: Oliver Sacks put himself into his case studies. What was the cost?

**原文链接**: [https://www.newyorker.com/magazine/2025/12/15/oliver-sacks-put-himself-into-his-case-studies-what-was-the-cost](https://www.newyorker.com/magazine/2025/12/15/oliver-sacks-put-himself-into-his-case-studies-what-was-the-cost)

生成摘要时出错

---

## 51. Compiler Engineering in Practice

**原文标题**: Compiler Engineering in Practice

**原文链接**: [https://chisophugis.github.io/2025/12/08/compiler-engineering-in-practice-part-1-what-is-a-compiler.html](https://chisophugis.github.io/2025/12/08/compiler-engineering-in-practice-part-1-what-is-a-compiler.html)

生成摘要时出错

---

## 52. Free Software Awards Winners Announced: Andy Wingo, Alx Sa, Govdirectory

**原文标题**: Free Software Awards Winners Announced: Andy Wingo, Alx Sa, Govdirectory

**原文链接**: [https://www.fsf.org/news/2024-free-software-awards-winners](https://www.fsf.org/news/2024-free-software-awards-winners)

生成摘要时出错

---

## 53. Lean theorem prover mathlib

**原文标题**: Lean theorem prover mathlib

**原文链接**: [https://github.com/leanprover-community/mathlib4](https://github.com/leanprover-community/mathlib4)

生成摘要时出错

---

## 54. 30 Years of <Br> Tags

**原文标题**: 30 Years of <Br> Tags

**原文链接**: [https://www.artmann.co/articles/30-years-of-br-tags](https://www.artmann.co/articles/30-years-of-br-tags)

生成摘要时出错

---

## 55. Germany's train service is one of Europe's worst. How did it get so bad?

**原文标题**: Germany's train service is one of Europe's worst. How did it get so bad?

**原文链接**: [https://www.npr.org/2025/12/12/g-s1-100794/germany-train-rail-deutsche-bahn](https://www.npr.org/2025/12/12/g-s1-100794/germany-train-rail-deutsche-bahn)

生成摘要时出错

---

## 56. Willison on Merchant's "Copywriters reveal how AI has decimated their industry"

**原文标题**: Willison on Merchant's "Copywriters reveal how AI has decimated their industry"

**原文链接**: [https://simonwillison.net/2025/Dec/14/copywriters-reveal-how-ai-has-decimated-their-industry/](https://simonwillison.net/2025/Dec/14/copywriters-reveal-how-ai-has-decimated-their-industry/)

生成摘要时出错

---

## 57. RemoveWindowsAI

**原文标题**: RemoveWindowsAI

**原文链接**: [https://github.com/zoicware/RemoveWindowsAI](https://github.com/zoicware/RemoveWindowsAI)

生成摘要时出错

---

## 58. Update Now: iOS 26.2 Fixes 20 Security Vulnerabilities, 2 Actively Exploited

**原文标题**: Update Now: iOS 26.2 Fixes 20 Security Vulnerabilities, 2 Actively Exploited

**原文链接**: [https://www.macrumors.com/2025/12/12/ios-26-2-security-vulnerabilities/](https://www.macrumors.com/2025/12/12/ios-26-2-security-vulnerabilities/)

生成摘要时出错

---

## 59. Purdue University approves new AI requirement for all undergrads

**原文标题**: Purdue University approves new AI requirement for all undergrads

**原文链接**: [https://www.forbes.com/sites/michaeltnietzel/2025/12/13/purdue-university-approves-new-ai-requirement-for-all-undergrads/](https://www.forbes.com/sites/michaeltnietzel/2025/12/13/purdue-university-approves-new-ai-requirement-for-all-undergrads/)

生成摘要时出错

---

## 60. Pope criticizes US bid to 'break apart' US-Europe alliance

**原文标题**: Pope criticizes US bid to 'break apart' US-Europe alliance

**原文链接**: [https://apnews.com/article/vatican-russia-ukraine-trump-pope-leo-60c898afe3241ff67552f417a06900b0](https://apnews.com/article/vatican-russia-ukraine-trump-pope-leo-60c898afe3241ff67552f417a06900b0)

生成摘要时出错

---

## 61. Kids Rarely Read Whole Books Anymore. Even in English Class

**原文标题**: Kids Rarely Read Whole Books Anymore. Even in English Class

**原文链接**: [https://www.nytimes.com/2025/12/12/us/high-school-english-teachers-assigning-books.html](https://www.nytimes.com/2025/12/12/us/high-school-english-teachers-assigning-books.html)

生成摘要时出错

---

## 62. Surface Tension of Software

**原文标题**: Surface Tension of Software

**原文链接**: [https://iamstelios.com/blog/surface-tension-of-software/](https://iamstelios.com/blog/surface-tension-of-software/)

生成摘要时出错

---

## 63. Awesome-Jj: Jujutsu Things

**原文标题**: Awesome-Jj: Jujutsu Things

**原文链接**: [https://github.com/Necior/awesome-jj](https://github.com/Necior/awesome-jj)

生成摘要时出错

---

## 64. Wine 11.0 RC2 – Run Windows Applications on Linux, BSD, Solaris and macOS

**原文标题**: Wine 11.0 RC2 – Run Windows Applications on Linux, BSD, Solaris and macOS

**原文链接**: [https://gitlab.winehq.org/wine/wine/-/releases/wine-11.0-rc2](https://gitlab.winehq.org/wine/wine/-/releases/wine-11.0-rc2)

生成摘要时出错

---

## 65. Therapeutic use of cannabis and cannabinoids: A review

**原文标题**: Therapeutic use of cannabis and cannabinoids: A review

**原文链接**: [https://jamanetwork.com/journals/jama/fullarticle/2842072?guestAccessKey=a368e622-e374-4a0c-8d3b-22a976500305](https://jamanetwork.com/journals/jama/fullarticle/2842072?guestAccessKey=a368e622-e374-4a0c-8d3b-22a976500305)

生成摘要时出错

---

## 66. Building an efficient hash table in Java

**原文标题**: Building an efficient hash table in Java

**原文链接**: [https://bluuewhale.github.io/posts/building-a-fast-and-memory-efficient-hash-table-in-java-by-borrowing-the-best-ideas/](https://bluuewhale.github.io/posts/building-a-fast-and-memory-efficient-hash-table-in-java-by-borrowing-the-best-ideas/)

生成摘要时出错

---

## 67. The Coming Need for Formal Specification

**原文标题**: The Coming Need for Formal Specification

**原文链接**: [https://benjamincongdon.me/blog/2025/12/12/The-Coming-Need-for-Formal-Specification/](https://benjamincongdon.me/blog/2025/12/12/The-Coming-Need-for-Formal-Specification/)

生成摘要时出错

---

## 68. AI is bringing old nuclear plants out of retirement

**原文标题**: AI is bringing old nuclear plants out of retirement

**原文链接**: [https://www.wbur.org/hereandnow/2025/12/09/nuclear-power-ai](https://www.wbur.org/hereandnow/2025/12/09/nuclear-power-ai)

生成摘要时出错

---

## 69. A giant ball will help this man survive a year on an iceberg

**原文标题**: A giant ball will help this man survive a year on an iceberg

**原文链接**: [https://www.outsideonline.com/outdoor-adventure/exploration-survival/how-giant-ball-will-help-man-survive-year-iceberg/](https://www.outsideonline.com/outdoor-adventure/exploration-survival/how-giant-ball-will-help-man-survive-year-iceberg/)

生成摘要时出错

---

## 70. Private Equity Finds a New Source of Profit: Volunteer Fire Departments

**原文标题**: Private Equity Finds a New Source of Profit: Volunteer Fire Departments

**原文链接**: [https://www.nytimes.com/2025/12/14/us/fire-department-software-private-equity.html](https://www.nytimes.com/2025/12/14/us/fire-department-software-private-equity.html)

生成摘要时出错

---

## 71. Windows 3.1 in the Browser

**原文标题**: Windows 3.1 in the Browser

**原文链接**: [https://www.pcjs.org/software/pcx86/sys/windows/3.10/](https://www.pcjs.org/software/pcx86/sys/windows/3.10/)

生成摘要时出错

---

## 72. Denmark sees US as potential security concern

**原文标题**: Denmark sees US as potential security concern

**原文链接**: [https://www.cnn.com/2025/12/10/europe/denmark-intelligence-report-intl](https://www.cnn.com/2025/12/10/europe/denmark-intelligence-report-intl)

生成摘要时出错

---

## 73. Think Tanker Altered Ukraine War Map Before Big Polymarket Payout

**原文标题**: Think Tanker Altered Ukraine War Map Before Big Polymarket Payout

**原文链接**: [https://responsiblestatecraft.org/isw-polymarket-ukraine-war-map/](https://responsiblestatecraft.org/isw-polymarket-ukraine-war-map/)

生成摘要时出错

---

## 74. Vacuum Is a Lie: About Your Indexes

**原文标题**: Vacuum Is a Lie: About Your Indexes

**原文链接**: [https://boringsql.com/posts/vacuum-is-lie/](https://boringsql.com/posts/vacuum-is-lie/)

生成摘要时出错

---

## 75. Z8086: Rebuilding the 8086 from Original Microcode

**原文标题**: Z8086: Rebuilding the 8086 from Original Microcode

**原文链接**: [https://nand2mario.github.io/posts/2025/z8086/](https://nand2mario.github.io/posts/2025/z8086/)

生成摘要时出错

---

## 76. GraphQL: The Enterprise Honeymoon Is Over

**原文标题**: GraphQL: The Enterprise Honeymoon Is Over

**原文链接**: [https://johnjames.blog/posts/graphql-the-enterprise-honeymoon-is-over](https://johnjames.blog/posts/graphql-the-enterprise-honeymoon-is-over)

生成摘要时出错

---

## 77. Rust Coreutils 0.5.0 Release: 87.75% compatibility with GNU Coreutils

**原文标题**: Rust Coreutils 0.5.0 Release: 87.75% compatibility with GNU Coreutils

**原文链接**: [https://github.com/uutils/coreutils/releases/tag/0.5.0](https://github.com/uutils/coreutils/releases/tag/0.5.0)

生成摘要时出错

---

## 78. Claude Code's DX is too good. And that's a problem

**原文标题**: Claude Code's DX is too good. And that's a problem

**原文链接**: [https://www.bharath.sh/writing/claude-code-dx](https://www.bharath.sh/writing/claude-code-dx)

生成摘要时出错

---

## 79. When did the job market get so rude?

**原文标题**: When did the job market get so rude?

**原文链接**: [https://www.theatlantic.com/culture/2025/12/job-ghosting-manners/685206/](https://www.theatlantic.com/culture/2025/12/job-ghosting-manners/685206/)

生成摘要时出错

---

## 80. Baumol's Cost Disease

**原文标题**: Baumol's Cost Disease

**原文链接**: [https://en.wikipedia.org/wiki/Baumol_effect](https://en.wikipedia.org/wiki/Baumol_effect)

生成摘要时出错

---

## 81. US TikTok investors in limbo as deal set to be delayed again

**原文标题**: US TikTok investors in limbo as deal set to be delayed again

**原文链接**: [https://www.bbc.com/news/articles/cp34442z25ko](https://www.bbc.com/news/articles/cp34442z25ko)

生成摘要时出错

---

## 82. We Lost Something: 1970s REPLs Were Better Than Modern Development Environments

**原文标题**: We Lost Something: 1970s REPLs Were Better Than Modern Development Environments

**原文链接**: [https://programmingsimplicity.substack.com/p/we-lost-something-1970s-repls-were](https://programmingsimplicity.substack.com/p/we-lost-something-1970s-repls-were)

生成摘要时出错

---

## 83. llamafile: Distribute and Run LLMs with a Single File

**原文标题**: llamafile: Distribute and Run LLMs with a Single File

**原文链接**: [https://github.com/mozilla-ai/llamafile](https://github.com/mozilla-ai/llamafile)

生成摘要时出错

---

## 84. The choice between Rust and C-derived languages is not only about memory safety

**原文标题**: The choice between Rust and C-derived languages is not only about memory safety

**原文链接**: [https://bbuyukliev.blogspot.com/2025/12/the-choice-between-rust-and-c-derived.html](https://bbuyukliev.blogspot.com/2025/12/the-choice-between-rust-and-c-derived.html)

生成摘要时出错

---

## 85. Illuminating the processor core with LLVM-mca

**原文标题**: Illuminating the processor core with LLVM-mca

**原文链接**: [https://abseil.io/fast/99](https://abseil.io/fast/99)

生成摘要时出错

---

## 86. Defrag.exfat Is Inefficient and Dangerous

**原文标题**: Defrag.exfat Is Inefficient and Dangerous

**原文链接**: [https://github.com/exfatprogs/exfatprogs/issues/318](https://github.com/exfatprogs/exfatprogs/issues/318)

生成摘要时出错

---

## 87. The Average Founder Ages 6 Months Each Year

**原文标题**: The Average Founder Ages 6 Months Each Year

**原文链接**: [https://tomtunguz.com/founder-age-median-trend/](https://tomtunguz.com/founder-age-median-trend/)

生成摘要时出错

---

## 88. Show HN: I audited 500 K8s pods. Java wastes ~48% RAM, Go ~18%

**原文标题**: Show HN: I audited 500 K8s pods. Java wastes ~48% RAM, Go ~18%

**原文链接**: [https://github.com/WozzHQ/wozz](https://github.com/WozzHQ/wozz)

生成摘要时出错

---

## 89. Interactive Common Lisp: An Enhanced REPL

**原文标题**: Interactive Common Lisp: An Enhanced REPL

**原文链接**: [https://github.com/atgreen/icl](https://github.com/atgreen/icl)

生成摘要时出错

---

## 90. What is a build system, anyway?

**原文标题**: What is a build system, anyway?

**原文链接**: [https://jyn.dev/what-is-a-build-system-anyway/](https://jyn.dev/what-is-a-build-system-anyway/)

生成摘要时出错

---

## 91. Sen. WHITEHOUSE: We are moving to file a bipartisan Section 230 repeal

**原文标题**: Sen. WHITEHOUSE: We are moving to file a bipartisan Section 230 repeal

**原文链接**: [https://bsky.app/profile/judiciarydems.senate.gov/post/3m7sjbvhbms2z](https://bsky.app/profile/judiciarydems.senate.gov/post/3m7sjbvhbms2z)

生成摘要时出错

---

## 92. I think I might be done for a while

**原文标题**: I think I might be done for a while

**原文链接**: [https://varunraghu.com/i-think-i-might-be-done-for-a-while/](https://varunraghu.com/i-think-i-might-be-done-for-a-while/)

生成摘要时出错

---

## 93. The Typeframe PX-88 Portable Computing System

**原文标题**: The Typeframe PX-88 Portable Computing System

**原文链接**: [https://www.typeframe.net/](https://www.typeframe.net/)

生成摘要时出错

---

## 94. 'Mamdani Effect' Is Seeing More People Moving to New York, Not Leaving It

**原文标题**: 'Mamdani Effect' Is Seeing More People Moving to New York, Not Leaving It

**原文链接**: [https://www.newsweek.com/mamdani-effect-more-people-moving-new-york-city-not-leaving-11193747](https://www.newsweek.com/mamdani-effect-more-people-moving-new-york-city-not-leaving-11193747)

生成摘要时出错

---

## 95. Efficient Basic Coding for the ZX Spectrum

**原文标题**: Efficient Basic Coding for the ZX Spectrum

**原文链接**: [https://blog.jafma.net/2020/02/24/efficient-basic-coding-for-the-zx-spectrum/](https://blog.jafma.net/2020/02/24/efficient-basic-coding-for-the-zx-spectrum/)

生成摘要时出错

---

## 96. Live Nation, Ticketmaster must face sprawling class action over prices

**原文标题**: Live Nation, Ticketmaster must face sprawling class action over prices

**原文链接**: [https://www.reuters.com/sustainability/boards-policy-regulation/live-nation-ticketmaster-must-face-sprawling-class-action-over-prices-2025-12-12/](https://www.reuters.com/sustainability/boards-policy-regulation/live-nation-ticketmaster-must-face-sprawling-class-action-over-prices-2025-12-12/)

生成摘要时出错

---

## 97. Sacrificing accessibility for not getting web scraped

**原文标题**: Sacrificing accessibility for not getting web scraped

**原文链接**: [https://tilschuenemann.de/projects/sacrificing-accessibility-for-not-getting-web-scraped](https://tilschuenemann.de/projects/sacrificing-accessibility-for-not-getting-web-scraped)

生成摘要时出错

---

## 98. Battery storage hits $65/MWh, a tipping point for solar

**原文标题**: Battery storage hits $65/MWh, a tipping point for solar

**原文链接**: [https://electrek.co/2025/12/12/battery-storage-hits-65-mwh-tipping-point-solar/](https://electrek.co/2025/12/12/battery-storage-hits-65-mwh-tipping-point-solar/)

生成摘要时出错

---

## 99. UK Lords propose ban on VPNs for children

**原文标题**: UK Lords propose ban on VPNs for children

**原文链接**: [https://www.techradar.com/vpn/vpn-privacy-security/uk-lords-propose-ban-on-vpns-for-children](https://www.techradar.com/vpn/vpn-privacy-security/uk-lords-propose-ban-on-vpns-for-children)

生成摘要时出错

---

## 100. The Chinese Billionaires Having 100s of U.S.-Born Babies via Surrogate

**原文标题**: The Chinese Billionaires Having 100s of U.S.-Born Babies via Surrogate

**原文链接**: [https://www.wsj.com/us-news/chinese-billionaires-surrogacy-pregnancy-7fdfc0c3](https://www.wsj.com/us-news/chinese-billionaires-surrogacy-pregnancy-7fdfc0c3)

生成摘要时出错

---

