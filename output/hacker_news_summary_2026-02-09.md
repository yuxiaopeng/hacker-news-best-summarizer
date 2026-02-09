# Hacker News 热门文章摘要 (2026-02-09)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 担保

**原文标题**: Vouch

**原文链接**: [https://github.com/mitchellh/vouch](https://github.com/mitchellh/vouch)

Vouch 是一个实验性的社区信任管理系统，旨在恢复开源项目的显式信任，解决低质量、AI 生成贡献的挑战。它允许项目“担保”用户，授予他们访问项目可配置部分的权限，或者“谴责”用户以阻止其互动。

该系统是通用的，可在任何代码托管平台使用，并通过 GitHub Actions 和基于 Nushell 的命令行界面 (CLI) 提供开箱即用的 GitHub 集成。项目完全定义“谁”获得担保、“如何”担保以及相关的后果，从而为他们的社区量身定制策略。

信任列表存储在一个简单的、扁平的 `.td` (Trustdown) 文件中，易于解析。一个关键特性是“信任网络”，它允许项目与其他项目共享已担保/已谴责的用户列表，从而创建一个更广泛、相互关联的信任网络，在此网络中，可信度可以在整个生态系统中自动识别。

GitHub Actions 自动化检查 PR 作者的担保状态，并通过问题或讨论评论促进用户信任的管理。CLI 提供用于检查状态、添加或谴责用户的命令。一个 Nushell 库支持脚本编写。Vouch 目前已被 Ghostty 使用，并将根据实际使用经验继续发展。

---

## 2. 游戏道路艺术

**原文标题**: Art of Roads in Games

**原文链接**: [https://sandboxspirit.com/blog/art-of-roads-in-games/](https://sandboxspirit.com/blog/art-of-roads-in-games/)

作者对复杂图案，特别是人工设计的道路网络，表现出深深的着迷，从中获得类似观察自然结构时的“原始满足感”。这一由《模拟城市2000》等游戏激发的终身兴趣，促使作者对城市建造游戏中道路的模拟方式进行了批判。尽管各类游戏和大量模组都有所进步，但游戏中的道路仍常显得不真实——充斥着急弯、不稳定的匝道和奇怪的转弯半径。

作者解释说，根本原因在于开发者对贝塞尔样条的依赖。尽管优雅，但贝塞尔曲线在偏移时无法保持形状和平行度，导致“捏合”和几何缺陷，因为现实世界中的道路从根本上受车辆车轮轴的限制。

文章提出了替代的曲线类型：圆弧在偏移时能保持完美的平行度，并简化交叉口计算，使它们适用于城市街道。对于高速应用，土木工程师使用缓和曲线，如回旋曲线，它们能平滑地增加曲率，以提供舒适的驾驶体验，尽管它们的数学复杂性较高。

出于好奇心以及对独立开发者可用工具的不足感到不满，作者现在正基于这些工程原理构建自己的道路系统，旨在为未来的城市建造游戏提供一个更真实、更强大的基础。

---

## 3. AI 让简单之处更简单，困难之处更困难

**原文标题**: AI makes the easy part easier and the hard part harder

**原文链接**: [https://www.blundergoat.com/articles/ai-makes-the-easy-part-easier-and-the-hard-part-harder](https://www.blundergoat.com/articles/ai-makes-the-easy-part-easier-and-the-hard-part-harder)

无法访问文章链接。

---

## 4. Discord下个月起将要求人脸扫描或身份证明才能完全访问。

**原文标题**: Discord will require a face scan or ID for full access next month

**原文链接**: [https://www.theverge.com/tech/875309/discord-age-verification-global-roll-out](https://www.theverge.com/tech/875309/discord-age-verification-global-roll-out)

自三月起，Discord 将在全球范围内推行年龄验证，所有用户账号将默认为“适合青少年的体验”。未验证为成年人的用户将面临限制，包括无法访问年龄限制的服务器或频道、无法在“舞台”频道发言、对露骨内容进行内容过滤，以及过滤来自陌生用户的私信。

为解除这些限制，用户可通过几种方式验证年龄：通过AI分析视频自拍进行面部年龄估算（Discord称此数据保留在用户设备上），或提交政府身份证件（由第三方供应商验证，据称图片会迅速删除）。Discord 强调他们使用“面部估算”，不保留身份证件中的个人识别信息。此外，年龄推断模型将分析用户元数据（如玩过的游戏和活动），以高置信度自动授予用户成年身份，使其可以跳过其他验证步骤。

此举是国际上推动在线年龄验证和加强儿童安全保护措施的更广泛努力的一部分。Discord 此前已在英国和澳大利亚实施了年龄验证，但用户最初找到了规避方法。该公司还在2025年10月遭遇了一起数据泄露事件，涉及一名前第三方供应商，导致年龄验证数据外泄，Discord 因此更换了供应商。尽管承认存在一些用户流失的风险，Discord 仍认为大多数用户不会经历重大变化，因为这些措施主要针对的是真正的成人内容。

---

## 5. AI fatigue is real and nobody talks about it

**原文标题**: AI fatigue is real and nobody talks about it

**原文链接**: [https://siddhantkhare.com/writing/ai-fatigue-is-real](https://siddhantkhare.com/writing/ai-fatigue-is-real)

生成摘要时出错

---

## 6. DoNotNotify 现已开源

**原文标题**: DoNotNotify is now Open Source

**原文链接**: [https://donotnotify.com/opensource.html](https://donotnotify.com/opensource.html)

生成摘要时出错

---

## 7. 泔水吓坏我了

**原文标题**: Slop Terrifies Me

**原文链接**: [https://ezhik.jp/ai-slop-terrifies-me/](https://ezhik.jp/ai-slop-terrifies-me/)

作者对软件开发的潜在未来深感恐惧，并将文章命名为“我对平庸之作感到恐惧”。他们的核心焦虑在于，人工智能的能力将停滞在“足够好”的水平——即能完成一个功能性产品约90%的部分——而开发者（即“AI牧者”）和用户都将接受这种被作者称为“平庸之作”的平庸结果，而不去追求剩下10%的卓越。

作者认为，这种接受将导致泛化、缺乏创意的软件，行业将出现“拼多多化”现象，独特的匠心被大规模生产的“平庸的React-Tailwind类应用”所取代。尽管作者承认“平庸之作”本质上是一个源于不当激励（例如“快速行动，打破常规”或市场主导地位）的“人的问题”，但人工智能代理被视为正在加速这一趋势，使得“足够好”的产品能够更快地被生产出来，而无需真正的关心或理解。

尽管存在一丝希望，认为AI工具可以赋能非开发者进行创作，从而弥合用户和创作者之间的鸿沟，但作者最终仍深感恐惧，认为这种“技术性习得性无助”是不可逆转的。他们最大的恐惧是，大多数人根本不关心软件质量、隐私或精心设计的功能。因此，计算的未来可能属于那些能最快生产出最多软件的人，这将导致真正匠心的消亡，且无人为其逝去而哀悼。

---

## 8. GitHub is down again

**原文标题**: GitHub is down again

**原文链接**: [https://www.githubstatus.com/incidents/54hndjxft5bx](https://www.githubstatus.com/incidents/54hndjxft5bx)

On February 9, 2026, GitHub experienced an incident primarily affecting notification delivery. The issue began around 15:54 UTC with reports of impacted performance. Investigation quickly pinpointed the problem as delays in notification delivery, which progressively worsened, reaching an average delay of approximately 1 hour and 20 minutes by 16:51 UTC.

Recovery efforts commenced shortly after, with delays gradually decreasing from 1 hour to 30 minutes, then 15 minutes, as the backlog was processed. By 19:14 UTC, notification delivery delays were resolved, and the incident was officially marked as resolved at 19:29 UTC. GitHub thanked users for their patience and announced that a detailed root cause analysis would be shared once available.

---

## 9. 我手写代码时更开心。

**原文标题**: I am happier writing code by hand

**原文链接**: [https://www.abhinavomprakash.com/posts/i-am-happier-writing-code-by-hand/](https://www.abhinavomprakash.com/posts/i-am-happier-writing-code-by-hand/)

作者描述了在使用Claude-code等大型语言模型进行大量代码生成时，感到抑郁和倦怠的经历，他们将这种做法称为“凭感觉编程”（vibe coding）。这种方法屡次让他们删除该工具，只为了重新发现手动编程的乐趣。

核心论点是，通过手动编程“与问题空间搏斗”对于深入理解、识别API痛点和内化上下文至关重要，这些都是高效软件工程的关键。将代码生成外包给大型语言模型会绕过这个关键的思考过程，使得验证正确性变得更困难，并助长了被动接受而非主动参与。作者指出，“凭感觉编程”可能令人上瘾，使大脑脱离思考，并讽刺地通过增加认知惯性使简单任务变得更慢。即使是快速生成的大型代码库，仍然需要人工审查和理解，这使得开发者成为最终的瓶颈。

作者承认大型语言模型是工具，但强调工具会塑造思维过程；如果一个工具阻碍了深度思考，那么它对知识工作者是有害的。作者现在以一种受控的、“有摩擦的”方式使用大型语言模型：手动提供上下文和具体的代码片段，用于有针对性的更改或测试。这种方法强制熟悉代码，保持大脑活跃，并保留了对幸福和高效工作至关重要的“心流状态”。最终，作者将心理健康置于通过全面功能生成可能获得但却不确定的生产力提升之上，鼓励其他人做出能优化其幸福感的选择。

---

## 10. Claude’s C Compiler vs. GCC

**原文标题**: Claude’s C Compiler vs. GCC

**原文链接**: [https://harshanu.space/en/tech/ccc-vs-gcc/](https://harshanu.space/en/tech/ccc-vs-gcc/)

生成摘要时出错

---

## 11. I put a real-time 3D shader on the Game Boy Color

**原文标题**: I put a real-time 3D shader on the Game Boy Color

**原文链接**: [https://blog.otterstack.com/posts/202512-gbshader/](https://blog.otterstack.com/posts/202512-gbshader/)

生成摘要时出错

---

## 12. Show HN: LocalGPT – A local-first AI assistant in Rust with persistent memory

**原文标题**: Show HN: LocalGPT – A local-first AI assistant in Rust with persistent memory

**原文链接**: [https://github.com/localgpt-app/localgpt](https://github.com/localgpt-app/localgpt)

生成摘要时出错

---

## 13. Show HN: Algorithmically finding the longest line of sight on Earth

**原文标题**: Show HN: Algorithmically finding the longest line of sight on Earth

**原文链接**: [https://alltheviews.world](https://alltheviews.world)

生成摘要时出错

---

## 14. OpenClaw is changing my life

**原文标题**: OpenClaw is changing my life

**原文链接**: [https://reorx.com/blog/openclaw-is-changing-my-life/](https://reorx.com/blog/openclaw-is-changing-my-life/)

生成摘要时出错

---

## 15. Omega-3 is inversely related to risk of early-onset dementia

**原文标题**: Omega-3 is inversely related to risk of early-onset dementia

**原文链接**: [https://pubmed.ncbi.nlm.nih.gov/41506004/](https://pubmed.ncbi.nlm.nih.gov/41506004/)

生成摘要时出错

---

## 16. Show HN: I created a Mars colony RPG based on Kim Stanley Robinson’s Mars books

**原文标题**: Show HN: I created a Mars colony RPG based on Kim Stanley Robinson’s Mars books

**原文链接**: [https://underhillgame.com/](https://underhillgame.com/)

生成摘要时出错

---

## 17. GitHub Agentic Workflows

**原文标题**: GitHub Agentic Workflows

**原文链接**: [https://github.github.io/gh-aw/](https://github.github.io/gh-aw/)

生成摘要时出错

---

## 18. Dave Farber has died

**原文标题**: Dave Farber has died

**原文链接**: [https://lists.nanog.org/archives/list/nanog@lists.nanog.org/thread/TSNPJVFH4DKLINIKSMRIIVNHDG5XKJCM/](https://lists.nanog.org/archives/list/nanog@lists.nanog.org/thread/TSNPJVFH4DKLINIKSMRIIVNHDG5XKJCM/)

生成摘要时出错

---

## 19. The world heard JD Vance being booed at the Olympics. Except for viewers in USA

**原文标题**: The world heard JD Vance being booed at the Olympics. Except for viewers in USA

**原文链接**: [https://www.theguardian.com/sport/2026/feb/07/jd-vance-boos-winter-olympics](https://www.theguardian.com/sport/2026/feb/07/jd-vance-boos-winter-olympics)

生成摘要时出错

---

## 20. More Mac malware from Google search

**原文标题**: More Mac malware from Google search

**原文链接**: [https://eclecticlight.co/2026/01/30/more-malware-from-google-search/](https://eclecticlight.co/2026/01/30/more-malware-from-google-search/)

生成摘要时出错

---

## 21. Beyond agentic coding

**原文标题**: Beyond agentic coding

**原文链接**: [https://haskellforall.com/2026/02/beyond-agentic-coding](https://haskellforall.com/2026/02/beyond-agentic-coding)

生成摘要时出错

---

## 22. Why E cores make Apple silicon fast

**原文标题**: Why E cores make Apple silicon fast

**原文链接**: [https://eclecticlight.co/2026/02/08/last-week-on-my-mac-why-e-cores-make-apple-silicon-fast/](https://eclecticlight.co/2026/02/08/last-week-on-my-mac-why-e-cores-make-apple-silicon-fast/)

生成摘要时出错

---

## 23. Converting a $3.88 analog clock from Walmart into a ESP8266-based Wi-Fi clock

**原文标题**: Converting a $3.88 analog clock from Walmart into a ESP8266-based Wi-Fi clock

**原文链接**: [https://github.com/jim11662418/ESP8266_WiFi_Analog_Clock](https://github.com/jim11662418/ESP8266_WiFi_Analog_Clock)

生成摘要时出错

---

## 24. GitHub Is Down

**原文标题**: GitHub Is Down

**原文链接**: [https://github.com/](https://github.com/)

生成摘要时出错

---

## 25. TSMC to make advanced AI semiconductors in Japan

**原文标题**: TSMC to make advanced AI semiconductors in Japan

**原文链接**: [https://apnews.com/article/semiconductors-tsmc-japan-taiwan-ai-11256f2bfde73ca23d08331ad138d6d5](https://apnews.com/article/semiconductors-tsmc-japan-taiwan-ai-11256f2bfde73ca23d08331ad138d6d5)

生成摘要时出错

---

## 26. Why is the sky blue?

**原文标题**: Why is the sky blue?

**原文链接**: [https://explainers.blog/posts/why-is-the-sky-blue/](https://explainers.blog/posts/why-is-the-sky-blue/)

生成摘要时出错

---

## 27. Nobody knows how the whole system works

**原文标题**: Nobody knows how the whole system works

**原文链接**: [https://surfingcomplexity.blog/2026/02/08/nobody-knows-how-the-whole-system-works/](https://surfingcomplexity.blog/2026/02/08/nobody-knows-how-the-whole-system-works/)

生成摘要时出错

---

## 28. AT&T, Verizon blocking release of Salt Typhoon security assessment reports

**原文标题**: AT&T, Verizon blocking release of Salt Typhoon security assessment reports

**原文链接**: [https://www.reuters.com/business/media-telecom/senator-says-att-verizon-blocking-release-salt-typhoon-security-assessment-2026-02-03/](https://www.reuters.com/business/media-telecom/senator-says-att-verizon-blocking-release-salt-typhoon-security-assessment-2026-02-03/)

生成摘要时出错

---

## 29. A GTA modder has got the 1997 original working on modern PCs and Steam Deck

**原文标题**: A GTA modder has got the 1997 original working on modern PCs and Steam Deck

**原文链接**: [https://gtaforums.com/topic/986492-grand-theft-auto-ready2play-full-game-windows-version/](https://gtaforums.com/topic/986492-grand-theft-auto-ready2play-full-game-windows-version/)

生成摘要时出错

---

## 30. Experts Have World Models. LLMs Have Word Models

**原文标题**: Experts Have World Models. LLMs Have Word Models

**原文链接**: [https://www.latent.space/p/adversarial-reasoning](https://www.latent.space/p/adversarial-reasoning)

生成摘要时出错

---

## 31. Billing can be bypassed using a combo of subagents with an agent definition

**原文标题**: Billing can be bypassed using a combo of subagents with an agent definition

**原文链接**: [https://github.com/microsoft/vscode/issues/292452](https://github.com/microsoft/vscode/issues/292452)

生成摘要时出错

---

## 32. Shifts in U.S. Social Media Use, 2020–2024: Decline, Fragmentation, Polarization (2025)

**原文标题**: Shifts in U.S. Social Media Use, 2020–2024: Decline, Fragmentation, Polarization (2025)

**原文链接**: [https://arxiv.org/abs/2510.25417](https://arxiv.org/abs/2510.25417)

生成摘要时出错

---

## 33. Running Your Own As: BGP on FreeBSD with FRR, GRE Tunnels, and Policy Routing

**原文标题**: Running Your Own As: BGP on FreeBSD with FRR, GRE Tunnels, and Policy Routing

**原文链接**: [https://blog.hofstede.it/running-your-own-as-bgp-on-freebsd-with-frr-gre-tunnels-and-policy-routing/](https://blog.hofstede.it/running-your-own-as-bgp-on-freebsd-with-frr-gre-tunnels-and-policy-routing/)

生成摘要时出错

---

## 34. Matrix messaging gaining ground in government IT

**原文标题**: Matrix messaging gaining ground in government IT

**原文链接**: [https://www.theregister.com/2026/02/09/matrix_element_secure_chat/](https://www.theregister.com/2026/02/09/matrix_element_secure_chat/)

生成摘要时出错

---

## 35. Curating a Show on My Ineffable Mother, Ursula K. Le Guin

**原文标题**: Curating a Show on My Ineffable Mother, Ursula K. Le Guin

**原文链接**: [https://hyperallergic.com/curating-a-show-on-my-ineffable-mother-ursula-k-le-guin/](https://hyperallergic.com/curating-a-show-on-my-ineffable-mother-ursula-k-le-guin/)

生成摘要时出错

---

## 36. Microsoft account bugs locked me out of Notepad – Are thin clients ruining PCs?

**原文标题**: Microsoft account bugs locked me out of Notepad – Are thin clients ruining PCs?

**原文链接**: [https://www.windowscentral.com/microsoft/windows-11/windows-locked-me-out-of-notepad-is-the-thin-client-era-ruining-pcs](https://www.windowscentral.com/microsoft/windows-11/windows-locked-me-out-of-notepad-is-the-thin-client-era-ruining-pcs)

生成摘要时出错

---

## 37. Bun v1.3.9

**原文标题**: Bun v1.3.9

**原文链接**: [https://bun.com/blog/bun-v1.3.9](https://bun.com/blog/bun-v1.3.9)

生成摘要时出错

---

## 38. Vouch

**原文标题**: Vouch

**原文链接**: [https://github.com/mitchellh/vouch](https://github.com/mitchellh/vouch)

生成摘要时出错

---

## 39. Hong Kong pro-democracy tycoon Jimmy Lai gets 20 years' jail

**原文标题**: Hong Kong pro-democracy tycoon Jimmy Lai gets 20 years' jail

**原文链接**: [https://www.bbc.com/news/articles/c8d5pl34vv0o](https://www.bbc.com/news/articles/c8d5pl34vv0o)

生成摘要时出错

---

## 40. AI Doesn't Reduce Work–It Intensifies It

**原文标题**: AI Doesn't Reduce Work–It Intensifies It

**原文链接**: [https://hbr.org/2026/02/ai-doesnt-reduce-work-it-intensifies-it](https://hbr.org/2026/02/ai-doesnt-reduce-work-it-intensifies-it)

生成摘要时出错

---

## 41. Every book recommended on the Odd Lots Discord

**原文标题**: Every book recommended on the Odd Lots Discord

**原文链接**: [https://odd-lots-books.netlify.app/](https://odd-lots-books.netlify.app/)

生成摘要时出错

---

## 42. Let's compile Quake like it's 1997

**原文标题**: Let's compile Quake like it's 1997

**原文链接**: [https://fabiensanglard.net/compile_like_1997/index.html](https://fabiensanglard.net/compile_like_1997/index.html)

生成摘要时出错

---

## 43. Apple XNU: Clutch Scheduler

**原文标题**: Apple XNU: Clutch Scheduler

**原文链接**: [https://github.com/apple-oss-distributions/xnu/blob/main/doc/scheduler/sched_clutch_edge.md](https://github.com/apple-oss-distributions/xnu/blob/main/doc/scheduler/sched_clutch_edge.md)

生成摘要时出错

---

## 44. The first sodium-ion battery EV is a winter range monster

**原文标题**: The first sodium-ion battery EV is a winter range monster

**原文链接**: [https://insideevs.com/news/786509/catl-changan-worlds-first-sodium-ion-battery-ev/](https://insideevs.com/news/786509/catl-changan-worlds-first-sodium-ion-battery-ev/)

生成摘要时出错

---

## 45. Tiny C Compiler

**原文标题**: Tiny C Compiler

**原文链接**: [https://bellard.org/tcc/](https://bellard.org/tcc/)

生成摘要时出错

---

## 46. Offpunk 3.0

**原文标题**: Offpunk 3.0

**原文链接**: [https://ploum.net/2026-02-09-offpunk3.html](https://ploum.net/2026-02-09-offpunk3.html)

生成摘要时出错

---

## 47. Roundcube Webmail: SVG feImage bypasses image blocking to track email opens

**原文标题**: Roundcube Webmail: SVG feImage bypasses image blocking to track email opens

**原文链接**: [https://nullcathedral.com/posts/2026-02-08-roundcube-svg-feimage-remote-image-bypass/](https://nullcathedral.com/posts/2026-02-08-roundcube-svg-feimage-remote-image-bypass/)

生成摘要时出错

---

## 48. RFC 3092 – Etymology of “Foo” (2001)

**原文标题**: RFC 3092 – Etymology of “Foo” (2001)

**原文链接**: [https://datatracker.ietf.org/doc/html/rfc3092](https://datatracker.ietf.org/doc/html/rfc3092)

生成摘要时出错

---

## 49. Thoughts on Generating C

**原文标题**: Thoughts on Generating C

**原文链接**: [https://wingolog.org/archives/2026/02/09/six-thoughts-on-generating-c](https://wingolog.org/archives/2026/02/09/six-thoughts-on-generating-c)

生成摘要时出错

---

## 50. Show HN: A custom font that displays Cistercian numerals using ligatures

**原文标题**: Show HN: A custom font that displays Cistercian numerals using ligatures

**原文链接**: [https://bobbiec.github.io/cistercian-font.html](https://bobbiec.github.io/cistercian-font.html)

生成摘要时出错

---

## 51. UEFI Bindings for JavaScript

**原文标题**: UEFI Bindings for JavaScript

**原文链接**: [https://codeberg.org/smnx/promethee](https://codeberg.org/smnx/promethee)

生成摘要时出错

---

## 52. Stop generating, start thinking

**原文标题**: Stop generating, start thinking

**原文链接**: [https://localghost.dev/blog/stop-generating-start-thinking/](https://localghost.dev/blog/stop-generating-start-thinking/)

生成摘要时出错

---

## 53. Irish man with valid US work permit held in ICE detention for five months

**原文标题**: Irish man with valid US work permit held in ICE detention for five months

**原文链接**: [https://www.theguardian.com/us-news/2026/feb/09/irish-man-seamus-culleton-ice-detention](https://www.theguardian.com/us-news/2026/feb/09/irish-man-seamus-culleton-ice-detention)

生成摘要时出错

---

## 54. Matchlock – Secures AI agent workloads with a Linux-based sandbox

**原文标题**: Matchlock – Secures AI agent workloads with a Linux-based sandbox

**原文链接**: [https://github.com/jingkaihe/matchlock](https://github.com/jingkaihe/matchlock)

生成摘要时出错

---

## 55. FDA intends to take action against non-FDA-approved GLP-1 drugs

**原文标题**: FDA intends to take action against non-FDA-approved GLP-1 drugs

**原文链接**: [https://www.fda.gov/news-events/press-announcements/fda-intends-take-action-against-non-fda-approved-glp-1-drugs](https://www.fda.gov/news-events/press-announcements/fda-intends-take-action-against-non-fda-approved-glp-1-drugs)

生成摘要时出错

---

## 56. Everything – Locate files and folders by name instantly

**原文标题**: Everything – Locate files and folders by name instantly

**原文链接**: [https://www.voidtools.com/](https://www.voidtools.com/)

生成摘要时出错

---

## 57. LineageOS 23.2

**原文标题**: LineageOS 23.2

**原文链接**: [https://lineageos.org/Changelog-31/](https://lineageos.org/Changelog-31/)

生成摘要时出错

---

## 58. The Little Bool of Doom (2025)

**原文标题**: The Little Bool of Doom (2025)

**原文链接**: [https://blog.svgames.pl/article/the-little-bool-of-doom](https://blog.svgames.pl/article/the-little-bool-of-doom)

生成摘要时出错

---

## 59. Exploiting signed bootloaders to circumvent UEFI Secure Boot (2019)

**原文标题**: Exploiting signed bootloaders to circumvent UEFI Secure Boot (2019)

**原文链接**: [https://habr.com/en/articles/446238/](https://habr.com/en/articles/446238/)

生成摘要时出错

---

## 60. Irish man detained by ICE for 5 months

**原文标题**: Irish man detained by ICE for 5 months

**原文链接**: [https://www.rte.ie/news/ireland/2026/0209/1557514-seamus-culleton/](https://www.rte.ie/news/ireland/2026/0209/1557514-seamus-culleton/)

生成摘要时出错

---

## 61. The silent death of good code

**原文标题**: The silent death of good code

**原文链接**: [https://amit.prasad.me/blog/rip-good-code](https://amit.prasad.me/blog/rip-good-code)

生成摘要时出错

---

## 62. Quartz crystals

**原文标题**: Quartz crystals

**原文链接**: [https://www.pa3fwm.nl/technotes/tn13a.html](https://www.pa3fwm.nl/technotes/tn13a.html)

生成摘要时出错

---

## 63. Like Game-of-Life, but on Growing Graphs, with WASM and WebGL

**原文标题**: Like Game-of-Life, but on Growing Graphs, with WASM and WebGL

**原文链接**: [https://znah.net/graphs/](https://znah.net/graphs/)

生成摘要时出错

---

## 64. Humans peak in midlife: A combined cognitive and personality trait perspective

**原文标题**: Humans peak in midlife: A combined cognitive and personality trait perspective

**原文链接**: [https://www.sciencedirect.com/science/article/pii/S0160289625000649](https://www.sciencedirect.com/science/article/pii/S0160289625000649)

生成摘要时出错

---

## 65. Reverse Engineering the Prom for the SGI O2

**原文标题**: Reverse Engineering the Prom for the SGI O2

**原文链接**: [https://mattst88.com/blog/2026/02/08/Reverse_Engineering_the_PROM_for_the_SGI_O2/](https://mattst88.com/blog/2026/02/08/Reverse_Engineering_the_PROM_for_the_SGI_O2/)

生成摘要时出错

---

## 66. Italy Railways Sabotaged

**原文标题**: Italy Railways Sabotaged

**原文链接**: [https://www.bbc.co.uk/news/articles/czr4rx04xjpo](https://www.bbc.co.uk/news/articles/czr4rx04xjpo)

生成摘要时出错

---

## 67. Show HN: Browse Internet Infrastructure

**原文标题**: Show HN: Browse Internet Infrastructure

**原文链接**: [https://www.wirewiki.com](https://www.wirewiki.com)

生成摘要时出错

---

## 68. Roger Ebert Reviews "The Shawshank Redemption" (1999)

**原文标题**: Roger Ebert Reviews "The Shawshank Redemption" (1999)

**原文链接**: [https://www.rogerebert.com/reviews/great-movie-the-shawshank-redemption-1994](https://www.rogerebert.com/reviews/great-movie-the-shawshank-redemption-1994)

生成摘要时出错

---

## 69. Homeland Security Spying on Reddit Users

**原文标题**: Homeland Security Spying on Reddit Users

**原文链接**: [https://www.kenklippenstein.com/p/homeland-security-spies-on-reddit](https://www.kenklippenstein.com/p/homeland-security-spies-on-reddit)

生成摘要时出错

---

## 70. Testing Ads in ChatGPT

**原文标题**: Testing Ads in ChatGPT

**原文链接**: [https://openai.com/index/testing-ads-in-chatgpt/](https://openai.com/index/testing-ads-in-chatgpt/)

生成摘要时出错

---

## 71. Substack confirms data breach affects users’ email addresses and phone numbers

**原文标题**: Substack confirms data breach affects users’ email addresses and phone numbers

**原文链接**: [https://techcrunch.com/2026/02/05/substack-confirms-data-breach-affecting-email-addresses-and-phone-numbers/](https://techcrunch.com/2026/02/05/substack-confirms-data-breach-affecting-email-addresses-and-phone-numbers/)

生成摘要时出错

---

## 72. Brookhaven Lab's RHIC concludes 25-year run with final collisions

**原文标题**: Brookhaven Lab's RHIC concludes 25-year run with final collisions

**原文链接**: [https://www.hpcwire.com/off-the-wire/brookhaven-labs-rhic-concludes-25-year-run-with-final-collisions/](https://www.hpcwire.com/off-the-wire/brookhaven-labs-rhic-concludes-25-year-run-with-final-collisions/)

生成摘要时出错

---

## 73. Show HN: Fine-tuned Qwen2.5-7B on 100 films for probabilistic story graphs

**原文标题**: Show HN: Fine-tuned Qwen2.5-7B on 100 films for probabilistic story graphs

**原文链接**: [https://cinegraphs.ai/](https://cinegraphs.ai/)

生成摘要时出错

---

## 74. Sleeper Shells: Attackers Are Planting Dormant Backdoors in Ivanti EPMM

**原文标题**: Sleeper Shells: Attackers Are Planting Dormant Backdoors in Ivanti EPMM

**原文链接**: [https://defusedcyber.com/ivanti-epmm-sleeper-shells-403jsp](https://defusedcyber.com/ivanti-epmm-sleeper-shells-403jsp)

生成摘要时出错

---

## 75. Hard-braking events as indicators of road segment crash risk

**原文标题**: Hard-braking events as indicators of road segment crash risk

**原文链接**: [https://research.google/blog/hard-braking-events-as-indicators-of-road-segment-crash-risk/](https://research.google/blog/hard-braking-events-as-indicators-of-road-segment-crash-risk/)

生成摘要时出错

---

## 76. A tough labor market for white-collar workers has turned recruiting upside down

**原文标题**: A tough labor market for white-collar workers has turned recruiting upside down

**原文链接**: [https://www.wsj.com/lifestyle/careers/job-hunters-are-so-desperate-that-theyre-paying-to-get-recruited-44891ac2](https://www.wsj.com/lifestyle/careers/job-hunters-are-so-desperate-that-theyre-paying-to-get-recruited-44891ac2)

生成摘要时出错

---

## 77. Reverse Engineering Raiders of the Lost Ark for the Atari 2600

**原文标题**: Reverse Engineering Raiders of the Lost Ark for the Atari 2600

**原文链接**: [https://github.com/joshuanwalker/Raiders2600](https://github.com/joshuanwalker/Raiders2600)

生成摘要时出错

---

## 78. Five disciplines discovered the same math independently

**原文标题**: Five disciplines discovered the same math independently

**原文链接**: [https://freethemath.org](https://freethemath.org)

生成摘要时出错

---

## 79. Bye Bye Humanity: The Potential AMOC Collapse

**原文标题**: Bye Bye Humanity: The Potential AMOC Collapse

**原文链接**: [https://thatjoescott.com/2026/02/03/bye-bye-humanity-the-potential-amoc-collapse/](https://thatjoescott.com/2026/02/03/bye-bye-humanity-the-potential-amoc-collapse/)

生成摘要时出错

---

## 80. Discord Launches Teen-by-Default Settings Globally

**原文标题**: Discord Launches Teen-by-Default Settings Globally

**原文链接**: [https://discord.com/press-releases/discord-launches-teen-by-default-settings-globally](https://discord.com/press-releases/discord-launches-teen-by-default-settings-globally)

生成摘要时出错

---

## 81. You Are Here

**原文标题**: You Are Here

**原文链接**: [https://brooker.co.za/blog/2026/02/07/you-are-here.html](https://brooker.co.za/blog/2026/02/07/you-are-here.html)

生成摘要时出错

---

## 82. Credentials for Linux: Bringing Passkeys to the Linux Desktop

**原文标题**: Credentials for Linux: Bringing Passkeys to the Linux Desktop

**原文链接**: [https://alfioemanuele.io/talks/2026/02/01/fosdem-2026-credentials-for-linux.html](https://alfioemanuele.io/talks/2026/02/01/fosdem-2026-credentials-for-linux.html)

生成摘要时出错

---

## 83. The 'Little red dots' observed by Webb were direct-collapse black holes

**原文标题**: The 'Little red dots' observed by Webb were direct-collapse black holes

**原文链接**: [https://phys.org/news/2026-02-red-dots-webb-collapse-black.html](https://phys.org/news/2026-02-red-dots-webb-collapse-black.html)

生成摘要时出错

---

## 84. Noam Chomsky's wife responds to Epstein controversy

**原文标题**: Noam Chomsky's wife responds to Epstein controversy

**原文链接**: [https://www.aaronmate.net/p/noam-chomskys-wife-responds-to-epstein](https://www.aaronmate.net/p/noam-chomskys-wife-responds-to-epstein)

生成摘要时出错

---

## 85. Stop Using Face ID

**原文标题**: Stop Using Face ID

**原文链接**: [https://www.pcmag.com/explainers/why-you-should-stop-using-face-id-right-now?test_uuid=04IpBmWGZleS0I0J3epvMrC&test_variant=B](https://www.pcmag.com/explainers/why-you-should-stop-using-face-id-right-now?test_uuid=04IpBmWGZleS0I0J3epvMrC&test_variant=B)

生成摘要时出错

---

## 86. Washington imposes 'terrorist-grade sanctions' on Francesca Albanese, ICC judges

**原文标题**: Washington imposes 'terrorist-grade sanctions' on Francesca Albanese, ICC judges

**原文链接**: [https://thecradle.co/articles-id/35816](https://thecradle.co/articles-id/35816)

生成摘要时出错

---

## 87. In the AI gold rush, tech firms are embracing 72-hour weeks

**原文标题**: In the AI gold rush, tech firms are embracing 72-hour weeks

**原文链接**: [https://www.bbc.com/news/articles/cvgn2k285ypo](https://www.bbc.com/news/articles/cvgn2k285ypo)

生成摘要时出错

---

## 88. SCOTUS to decide if 1988 video tape privacy law applies to internet uses

**原文标题**: SCOTUS to decide if 1988 video tape privacy law applies to internet uses

**原文链接**: [https://www.jurist.org/news/2026/01/us-supreme-court-to-decide-if-1988-video-tape-privacy-law-applies-to-internet-uses/](https://www.jurist.org/news/2026/01/us-supreme-court-to-decide-if-1988-video-tape-privacy-law-applies-to-internet-uses/)

生成摘要时出错

---

## 89. From watchdogs to mouthpieces: Washington Post and the wreckage of legacy media

**原文标题**: From watchdogs to mouthpieces: Washington Post and the wreckage of legacy media

**原文链接**: [https://www.thejournal.ie/readme/bezos-washington-post-trump-6950317-Feb2026/](https://www.thejournal.ie/readme/bezos-washington-post-trump-6950317-Feb2026/)

生成摘要时出错

---

## 90. Can Ozempic Cure Addiction?

**原文标题**: Can Ozempic Cure Addiction?

**原文链接**: [https://www.newyorker.com/magazine/2026/02/16/can-ozempic-cure-addiction](https://www.newyorker.com/magazine/2026/02/16/can-ozempic-cure-addiction)

生成摘要时出错

---

## 91. Amazon delivery drone strikes North Texas apartment, causing minor damage

**原文标题**: Amazon delivery drone strikes North Texas apartment, causing minor damage

**原文链接**: [https://www.expressnews.com/news/texas/article/amazon-delivery-drone-crash-richardson-texas-21341387.php](https://www.expressnews.com/news/texas/article/amazon-delivery-drone-crash-richardson-texas-21341387.php)

生成摘要时出错

---

## 92. Long-Sought Proof Tames Some of Math's Unruliest Equations

**原文标题**: Long-Sought Proof Tames Some of Math's Unruliest Equations

**原文链接**: [https://www.quantamagazine.org/long-sought-proof-tames-some-of-maths-unruliest-equations-20260206/](https://www.quantamagazine.org/long-sought-proof-tames-some-of-maths-unruliest-equations-20260206/)

生成摘要时出错

---

## 93. Bitcoin tumbles below $70K, heavy losses in cryptocurrencies in last three weeks

**原文标题**: Bitcoin tumbles below $70K, heavy losses in cryptocurrencies in last three weeks

**原文链接**: [https://www.bloomberg.com/news/articles/2026-02-05/bitcoin-drops-below-70-000-as-forced-deleveraging-accelerates](https://www.bloomberg.com/news/articles/2026-02-05/bitcoin-drops-below-70-000-as-forced-deleveraging-accelerates)

生成摘要时出错

---

## 94. Show HN: Printable Classics – Free printable classic books for hobby bookbinders

**原文标题**: Show HN: Printable Classics – Free printable classic books for hobby bookbinders

**原文链接**: [https://printableclassics.com](https://printableclassics.com)

生成摘要时出错

---

## 95. Apple Container 0.9.0

**原文标题**: Apple Container 0.9.0

**原文链接**: [https://github.com/apple/container/releases/tag/0.9.0](https://github.com/apple/container/releases/tag/0.9.0)

生成摘要时出错

---

## 96. Jony Ive Designed Ferrari Luce EV Interior

**原文标题**: Jony Ive Designed Ferrari Luce EV Interior

**原文链接**: [https://www.topgear.com/car-news/electric/official-ferraris-first-ev-called-luce-interior-apples-old-design-boss](https://www.topgear.com/car-news/electric/official-ferraris-first-ev-called-luce-interior-apples-old-design-boss)

生成摘要时出错

---

## 97. OpenAI exec becomes top Trump donor with $25M gift

**原文标题**: OpenAI exec becomes top Trump donor with $25M gift

**原文链接**: [https://finance.yahoo.com/news/openai-exec-becomes-top-trump-230342268.html](https://finance.yahoo.com/news/openai-exec-becomes-top-trump-230342268.html)

生成摘要时出错

---

## 98. In the Australian outback, we're listening for nuclear tests

**原文标题**: In the Australian outback, we're listening for nuclear tests

**原文链接**: [https://www.abc.net.au/news/2026-02-08/australian-outback-nuclear-tests-listening-warramunga-facility/106307478](https://www.abc.net.au/news/2026-02-08/australian-outback-nuclear-tests-listening-warramunga-facility/106307478)

生成摘要时出错

---

## 99. Gen Z first generation since 1800's with lower cognitive performance

**原文标题**: Gen Z first generation since 1800's with lower cognitive performance

**原文链接**: [https://www.commerce.senate.gov/services/files/A19DF2E8-3C69-4193-A676-430CF0C83DC2](https://www.commerce.senate.gov/services/files/A19DF2E8-3C69-4193-A676-430CF0C83DC2)

生成摘要时出错

---

## 100. Why is Singapore no longer "cool"?

**原文标题**: Why is Singapore no longer "cool"?

**原文链接**: [https://marginalrevolution.com/marginalrevolution/2026/02/why-is-singapore-no-longer-cool.html](https://marginalrevolution.com/marginalrevolution/2026/02/why-is-singapore-no-longer-cool.html)

生成摘要时出错

---

