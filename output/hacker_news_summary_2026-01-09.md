# Hacker News 热门文章摘要 (2026-01-09)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 博士发布了其已停产的SoundTouch扬声器的API文档并开放了API。

**原文标题**: Bose has released API docs and opened the API for its EoL SoundTouch speakers

**原文链接**: [https://arstechnica.com/gadgets/2026/01/bose-open-sources-its-soundtouch-home-theater-smart-speakers-ahead-of-eol/](https://arstechnica.com/gadgets/2026/01/bose-open-sources-its-soundtouch-home-theater-smart-speakers-ahead-of-eol/)

博士公司宣布对其即将终止服务的SoundTouch Wi-Fi音箱和回音壁做出重大调整，这些设备原定于2月18日“变笨”（失去智能功能）。最初在10月份的声明中称，这些昂贵的设备（399至1500美元）将失去Wi-Fi、云连接、应用控制、多房间音频、音乐服务集成和更新，仅限于通过AUX、HDMI或蓝牙连接使用。这一决定曾让许多老客户感到沮丧。

今天，博士公司带来了更好的消息。在致客户的电子邮件中，该公司确认，在SoundTouch音箱终止服务后，AirPlay和Spotify Connect将继续支持这些设备。此外，兼容AirPlay 2的设备将保留多房间音频功能。SoundTouch应用也将得以保留，并将在2026年5月6日获得更新，以支持不依赖云的本地功能。博士公司还提供了一个保存预设的变通方法。

至关重要的是，博士公司已经发布了SoundTouch的应用程序编程接口（API）文档。此举允许独立开发者创建自定义工具和功能，为那些否则可能成为电子垃圾的设备提供了一线生机。尽管部分功能仍然丧失，但与行业常见的“变砖”（使其完全失效）智能设备的做法相比，这一开源决定被视为一种更仁慈的产品停产方式。文章倡导，当智能设备制造商停产产品时，应将开源API和努力维护功能等做法变为标准实践。

---

## 2. 美国将禁止华尔街投资者购买独栋住宅

**原文标题**: US will ban Wall Street investors from buying single-family homes

**原文链接**: [https://www.reuters.com/world/us/us-will-ban-large-institutional-investors-buying-single-family-homes-trump-says-2026-01-07/](https://www.reuters.com/world/us/us-will-ban-large-institutional-investors-buying-single-family-homes-trump-says-2026-01-07/)

唐纳德·特朗普若再次当选，计划禁止大型机构投资者购买独栋住宅。在拉斯维加斯的一次竞选集会上，特朗普宣布了这项提议，称其目的是让美国家庭更能负担得起住房，并为年轻人提供更好的置业机会。

他批评这些机构投资者，包括对冲基金和私募股权公司，通过大量收购房屋来“盘剥”家庭，从而推高房价并减少个人买家可用的房源。这类投资者显著增加了他们的市场份额，尤其是在疫情期间的房地产繁荣时期。批评者认为，他们的大规模购买导致住房难以负担，并将潜在的自住房屋转变为出租房。

特朗普提议的禁令旨在遏制这一趋势，缓解房地产市场的竞争，并稳定房价，最终作为他更广泛的经济议程的一部分，以促进大众拥有住房的更多机会。

---

## 3. Google AI Studio is now sponsoring Tailwind CSS

**原文标题**: Google AI Studio is now sponsoring Tailwind CSS

**原文链接**: [https://twitter.com/OfficialLoganK/status/2009339263251566902](https://twitter.com/OfficialLoganK/status/2009339263251566902)

生成摘要时出错

---

## 4. 如何用 200 行代码编写 Claude 代码

**原文标题**: How to Code Claude Code in 200 Lines of Code

**原文链接**: [https://www.mihaileric.com/The-Emperor-Has-No-Clothes/](https://www.mihaileric.com/The-Emperor-Has-No-Clothes/)

文章《如何用200行代码编写Claude代码》揭示了AI编码助手的神秘面纱，展示了其核心功能可以用大约200行Python代码实现。其底层心智模型是一个简单的对话循环：用户发送一条消息，大型语言模型（LLM）判断是否需要工具，程序在本地执行该工具，并将结果反馈给LLM，LLM随后继续对话或作出回应。LLM本身从不直接与文件系统交互；它将任务委托给本地程序。

实现了三个基本工具：`read_file_tool`（用于获取文件内容）、`list_files_tool`（用于导航目录）和`edit_file_tool`（用于创建新文件或替换文本）。`edit_file_tool`使用空字符串`old_str`来表示文件创建。

关键一步是“教导”LLM了解这些工具。这通过动态生成一个`SYSTEM_PROMPT`来完成，该提示包含每个工具的名称、描述（来自其文档字符串）和签名。该提示还指定了LLM调用工具必须使用的确切格式：`tool: TOOL_NAME({JSON_ARGS})`。然后，一个解析器从LLM的响应中提取这些工具调用。

核心的`run_coding_agent_loop`管理着交互：一个外部循环接收用户输入，一个内部循环调用LLM。如果LLM响应一个工具调用，该工具就会被执行，其结果以`tool_result(...)`的形式附加到对话中，内部循环则重复执行。这允许了链式工具调用。如果LLM不调用工具，则显示其响应，内部循环终止。

尽管生产级智能体包含高级错误处理、流式传输和更多工具等功能，但文章总结道，这种基本的LLM-工具执行循环是即使是复杂的AI编码助手的架构核心。

---

## 5. 杰夫·迪恩语录

**原文标题**: The Jeff Dean Facts

**原文链接**: [https://github.com/LRitzdorf/TheJeffDeanFacts](https://github.com/LRitzdorf/TheJeffDeanFacts)

本文介绍了“杰夫·迪恩趣闻”（The Jeff Dean Facts），这是一系列查克·诺里斯式的段子，幽默地夸大了谷歌员工杰夫·迪恩非凡的编程能力。创建者汇编此合集是为了保存这些趣闻，因为许多原始来源，例如某个Quora帖子，已被删除。

这些“趣闻”将迪恩描绘成一位传奇人物，能够完成不可能的壮举，例如在白板上解决NP问题，将Google搜索作为“新员工项目”（Noogler Project）来创建，发明O(1/n)算法，甚至连编译器都会反过来警告他。他的影响力被描绘成超越了典型的软件开发，影响物理学、内存行为，甚至神灵的创造。有趣的是，有些趣闻被明确标记为“真实”，例如唐纳德·克努特（Don Knuth）在迪恩的斯坦福研讨会上坐在地上，或者迪恩度假时，谷歌的生产服务神秘地出现故障。

该清单是从各种来源汇编而来的，包括Quora、一个保加利亚编程竞赛网站（infO(N)）以及一个现已删除的Google+帖子。

---

## 6. 安思罗匹克禁止第三方使用Claude Code订阅

**原文标题**: Anthropic blocks third-party use of Claude Code subscriptions

**原文链接**: [https://github.com/anomalyco/opencode/issues/7410](https://github.com/anomalyco/opencode/issues/7410)

2026年1月9日，出现了一个问题，表明Anthropic已阻止第三方应用程序（具体来说是OpenCode）访问Claude Code订阅（称为“Claude Max”）。

一位名叫piotryordanov的用户在`anomalyco/opencode` GitHub存储库上报告了这个问题，声称“Claude Max”的使用突然中断，并出现了一个未指明的错误。尝试重新连接也未成功，并产生了相同的错误。

该事件被记录为`Broken Claude Max #7410`，影响OpenCode 1.1.8版的用户，尤其是在macOS上。该GitHub问题迅速获得了超过280名用户的广泛关注和回应，这表明对那些依赖OpenCode使用Claude功能的用户造成了广泛影响。该问题被标记为“bug”，证实了一项关键服务中断。

---

## 7. 伊朗IPv6断网

**原文标题**: Iran Goes Into IPv6 Blackout

**原文链接**: [https://radar.cloudflare.com/routing/ir](https://radar.cloudflare.com/routing/ir)

所提供的URL，https://radar.cloudflare.com/routing/ir，指向Cloudflare Radar上伊朗互联网流量的实时数据仪表盘，而不是一篇题为“伊朗进入IPv6中断”的特定文章。然而，该仪表盘上显示的数据强烈表明伊朗几乎完全没有采用IPv6，实际上代表着该国长期处于“IPv6中断”状态。

根据Cloudflare Radar的数据，伊朗的IPv6流量始终徘徊在互联网总流量的0.25%左右，微不足道，而IPv4则占据了近100%的主导地位。这种极低的采用率远低于全球平均水平，并且随着时间的推移几乎没有实质性变化，这表明伊朗互联网服务提供商普遍缺乏IPv6部署，且终端用户的使用非常有限。该仪表盘的“协议采用”部分清楚地说明了这种差异。尽管数据没有详细说明某个特定的中断事件，但它描绘了一幅IPv6连接在全国范围内几乎不存在的图景，使伊朗成为全球IPv6启用率最低的国家之一。

---

## 8. Open Infrastructure Map

**原文标题**: Open Infrastructure Map

**原文链接**: [https://openinframap.org](https://openinframap.org)

The provided text introduces the "Open Infrastructure Map," which is presented as a specific online service or platform. The sole piece of functional information conveyed is that users are required to have JavaScript enabled in their web browser in order to view or access this map.

---

## 9. Project Patchouli: Open-source electromagnetic drawing tablet hardware

**原文标题**: Project Patchouli: Open-source electromagnetic drawing tablet hardware

**原文链接**: [https://patchouli.readthedocs.io/en/latest/](https://patchouli.readthedocs.io/en/latest/)

生成摘要时出错

---

## 10. ChatGPT Health

**原文标题**: ChatGPT Health

**原文链接**: [https://openai.com/index/introducing-chatgpt-health/](https://openai.com/index/introducing-chatgpt-health/)

生成摘要时出错

---

## 11. AI coding assistants are getting worse?

**原文标题**: AI coding assistants are getting worse?

**原文链接**: [https://spectrum.ieee.org/ai-coding-degrades](https://spectrum.ieee.org/ai-coding-degrades)

生成摘要时出错

---

## 12. A closer look at a BGP anomaly in Venezuela

**原文标题**: A closer look at a BGP anomaly in Venezuela

**原文链接**: [https://blog.cloudflare.com/bgp-route-leak-venezuela/](https://blog.cloudflare.com/bgp-route-leak-venezuela/)

生成摘要时出错

---

## 13. European Commission issues call for evidence on open source

**原文标题**: European Commission issues call for evidence on open source

**原文链接**: [https://lwn.net/Articles/1053107/](https://lwn.net/Articles/1053107/)

生成摘要时出错

---

## 14. Tailscale state file encryption no longer enabled by default

**原文标题**: Tailscale state file encryption no longer enabled by default

**原文链接**: [https://tailscale.com/changelog](https://tailscale.com/changelog)

生成摘要时出错

---

## 15. Minneapolis driver shot and killed by ICE

**原文标题**: Minneapolis driver shot and killed by ICE

**原文链接**: [https://www.nbcnews.com/news/us-news/federal-law-enforcement-involved-ice-related-shooting-minneapolis-rcna252812](https://www.nbcnews.com/news/us-news/federal-law-enforcement-involved-ice-related-shooting-minneapolis-rcna252812)

生成摘要时出错

---

## 16. Sopro TTS: A 169M model with zero-shot voice cloning that runs on the CPU

**原文标题**: Sopro TTS: A 169M model with zero-shot voice cloning that runs on the CPU

**原文链接**: [https://github.com/samuel-vitorino/sopro](https://github.com/samuel-vitorino/sopro)

生成摘要时出错

---

## 17. Minnesota officials say they can't access evidence after fatal ICE shooting

**原文标题**: Minnesota officials say they can't access evidence after fatal ICE shooting

**原文链接**: [https://www.pbs.org/newshour/nation/minnesota-officials-say-they-cant-access-evidence-after-fatal-ice-shooting-and-fbi-wont-work-jointly-on-investigation](https://www.pbs.org/newshour/nation/minnesota-officials-say-they-cant-access-evidence-after-fatal-ice-shooting-and-fbi-wont-work-jointly-on-investigation)

生成摘要时出错

---

## 18. Mathematics for Computer Science (2018) [pdf]

**原文标题**: Mathematics for Computer Science (2018) [pdf]

**原文链接**: [https://courses.csail.mit.edu/6.042/spring18/mcs.pdf](https://courses.csail.mit.edu/6.042/spring18/mcs.pdf)

生成摘要时出错

---

## 19. ICE Is Going on a Surveillance Shopping Spree

**原文标题**: ICE Is Going on a Surveillance Shopping Spree

**原文链接**: [https://www.eff.org/deeplinks/2026/01/ice-going-surveillance-shopping-spree](https://www.eff.org/deeplinks/2026/01/ice-going-surveillance-shopping-spree)

生成摘要时出错

---

## 20. What happened to WebAssembly

**原文标题**: What happened to WebAssembly

**原文链接**: [https://emnudge.dev/blog/what-happened-to-webassembly/](https://emnudge.dev/blog/what-happened-to-webassembly/)

生成摘要时出错

---

## 21. The unreasonable effectiveness of the Fourier transform

**原文标题**: The unreasonable effectiveness of the Fourier transform

**原文链接**: [https://joshuawise.com/resources/ofdm/](https://joshuawise.com/resources/ofdm/)

生成摘要时出错

---

## 22. Embassy: Modern embedded framework, using Rust and async

**原文标题**: Embassy: Modern embedded framework, using Rust and async

**原文链接**: [https://github.com/embassy-rs/embassy](https://github.com/embassy-rs/embassy)

生成摘要时出错

---

## 23. Kernel bugs hide for 2 years on average. Some hide for 20

**原文标题**: Kernel bugs hide for 2 years on average. Some hide for 20

**原文链接**: [https://pebblebed.com/blog/kernel-bugs](https://pebblebed.com/blog/kernel-bugs)

生成摘要时出错

---

## 24. Replit founder Amjad Masad isn’t afraid of Silicon Valley

**原文标题**: Replit founder Amjad Masad isn’t afraid of Silicon Valley

**原文链接**: [https://sfstandard.com/2026/01/07/called-terrorist-sympathizer-now-ai-company-valued-3b/](https://sfstandard.com/2026/01/07/called-terrorist-sympathizer-now-ai-company-valued-3b/)

生成摘要时出错

---

## 25. Kagi releases alpha version of Orion for Linux

**原文标题**: Kagi releases alpha version of Orion for Linux

**原文链接**: [https://help.kagi.com/orion/misc/linux-status.html](https://help.kagi.com/orion/misc/linux-status.html)

生成摘要时出错

---

## 26. Let's call a murder a murder

**原文标题**: Let's call a murder a murder

**原文链接**: [https://daringfireball.net/2026/01/lets_call_a_murder_a_murder](https://daringfireball.net/2026/01/lets_call_a_murder_a_murder)

生成摘要时出错

---

## 27. ICE's Tool to Monitor Phones in Neighborhoods

**原文标题**: ICE's Tool to Monitor Phones in Neighborhoods

**原文链接**: [https://www.404media.co/inside-ices-tool-to-monitor-phones-in-entire-neighborhoods/](https://www.404media.co/inside-ices-tool-to-monitor-phones-in-entire-neighborhoods/)

生成摘要时出错

---

## 28. London–Calcutta Bus Service

**原文标题**: London–Calcutta Bus Service

**原文链接**: [https://en.wikipedia.org/wiki/London%E2%80%93Calcutta_bus_service](https://en.wikipedia.org/wiki/London%E2%80%93Calcutta_bus_service)

生成摘要时出错

---

## 29. Richard D. James aka Aphex Twin speaks to Tatsuya Takahashi (2017)

**原文标题**: Richard D. James aka Aphex Twin speaks to Tatsuya Takahashi (2017)

**原文链接**: [https://web.archive.org/web/20180719052026/http://item.warp.net/interview/aphex-twin-speaks-to-tatsuya-takahashi/](https://web.archive.org/web/20180719052026/http://item.warp.net/interview/aphex-twin-speaks-to-tatsuya-takahashi/)

生成摘要时出错

---

## 30. IBM AI ('Bob') Downloads and Executes Malware

**原文标题**: IBM AI ('Bob') Downloads and Executes Malware

**原文链接**: [https://www.promptarmor.com/resources/ibm-ai-(-bob-)-downloads-and-executes-malware](https://www.promptarmor.com/resources/ibm-ai-(-bob-)-downloads-and-executes-malware)

生成摘要时出错

---

## 31. Why I left iNaturalist

**原文标题**: Why I left iNaturalist

**原文链接**: [https://kueda.net/blog/2026/01/06/why-i-left-inat/](https://kueda.net/blog/2026/01/06/why-i-left-inat/)

生成摘要时出错

---

## 32. The Vietnam government has banned rooted phones from using any banking app

**原文标题**: The Vietnam government has banned rooted phones from using any banking app

**原文链接**: [https://xdaforums.com/t/discussion-the-root-and-mod-hiding-fingerprint-spoofing-keybox-stealing-cat-and-mouse-game.4425939/page-118](https://xdaforums.com/t/discussion-the-root-and-mod-hiding-fingerprint-spoofing-keybox-stealing-cat-and-mouse-game.4425939/page-118)

生成摘要时出错

---

## 33. Fighting back against biometric surveillance at Wegmans

**原文标题**: Fighting back against biometric surveillance at Wegmans

**原文链接**: [https://blog.adafruit.com/2026/01/07/dont-let-the-grocery-store-scan-your-face-a-guide-to-fighting-back-against-biometric-surveillance-at-wegmans/](https://blog.adafruit.com/2026/01/07/dont-let-the-grocery-store-scan-your-face-a-guide-to-fighting-back-against-biometric-surveillance-at-wegmans/)

生成摘要时出错

---

## 34. Notion AI: Unpatched data exfiltration

**原文标题**: Notion AI: Unpatched data exfiltration

**原文链接**: [https://www.promptarmor.com/resources/notion-ai-unpatched-data-exfiltration](https://www.promptarmor.com/resources/notion-ai-unpatched-data-exfiltration)

生成摘要时出错

---

## 35. Do not mistake a resilient global economy for populist success

**原文标题**: Do not mistake a resilient global economy for populist success

**原文链接**: [https://www.economist.com/leaders/2026/01/08/do-not-mistake-a-resilient-global-economy-for-populist-success](https://www.economist.com/leaders/2026/01/08/do-not-mistake-a-resilient-global-economy-for-populist-success)

生成摘要时出错

---

## 36. NPM to implement staged publishing after turbulent shift off classic tokens

**原文标题**: NPM to implement staged publishing after turbulent shift off classic tokens

**原文链接**: [https://socket.dev/blog/npm-to-implement-staged-publishing](https://socket.dev/blog/npm-to-implement-staged-publishing)

生成摘要时出错

---

## 37. The No Fakes Act has a “fingerprinting” trap that kills open source?

**原文标题**: The No Fakes Act has a “fingerprinting” trap that kills open source?

**原文链接**: [https://old.reddit.com/r/LocalLLaMA/comments/1q7qcux/the_no_fakes_act_has_a_fingerprinting_trap_that/](https://old.reddit.com/r/LocalLLaMA/comments/1q7qcux/the_no_fakes_act_has_a_fingerprinting_trap_that/)

生成摘要时出错

---

## 38. Play Aardwolf MUD

**原文标题**: Play Aardwolf MUD

**原文链接**: [https://www.aardwolf.com/](https://www.aardwolf.com/)

生成摘要时出错

---

## 39. Iran Protest Map

**原文标题**: Iran Protest Map

**原文链接**: [https://pouyaii.github.io/Iran/](https://pouyaii.github.io/Iran/)

生成摘要时出错

---

## 40. Claude Code CLI was broken

**原文标题**: Claude Code CLI was broken

**原文链接**: [https://github.com/anthropics/claude-code/issues/16673](https://github.com/anthropics/claude-code/issues/16673)

生成摘要时出错

---

## 41. Go.sum is not a lockfile

**原文标题**: Go.sum is not a lockfile

**原文链接**: [https://words.filippo.io/gosum/](https://words.filippo.io/gosum/)

生成摘要时出错

---

## 42. Cloudflare CEO on the Italy fines

**原文标题**: Cloudflare CEO on the Italy fines

**原文链接**: [https://twitter.com/eastdakota/status/2009654937303896492](https://twitter.com/eastdakota/status/2009654937303896492)

生成摘要时出错

---

## 43. Fixing a Buffer Overflow in Unix v4 Like It's 1973

**原文标题**: Fixing a Buffer Overflow in Unix v4 Like It's 1973

**原文链接**: [https://sigma-star.at/blog/2025/12/unix-v4-buffer-overflow/](https://sigma-star.at/blog/2025/12/unix-v4-buffer-overflow/)

生成摘要时出错

---

## 44. AI misses nearly one-third of breast cancers, study finds

**原文标题**: AI misses nearly one-third of breast cancers, study finds

**原文链接**: [https://www.emjreviews.com/radiology/news/ai-misses-nearly-one-third-of-breast-cancers-study-finds/](https://www.emjreviews.com/radiology/news/ai-misses-nearly-one-third-of-breast-cancers-study-finds/)

生成摘要时出错

---

## 45. Japanese electronics store pleads for old PCs amid ongoing hardware shortage

**原文标题**: Japanese electronics store pleads for old PCs amid ongoing hardware shortage

**原文链接**: [https://www.tomshardware.com/desktops/pc-building/major-japanese-electronics-store-begs-customers-for-their-old-pcs-as-hardware-drought-continues-we-pretty-much-buy-any-pc-pleads-the-akihabara-outlet](https://www.tomshardware.com/desktops/pc-building/major-japanese-electronics-store-begs-customers-for-their-old-pcs-as-hardware-drought-continues-we-pretty-much-buy-any-pc-pleads-the-akihabara-outlet)

生成摘要时出错

---

## 46. Show HN: macOS menu bar app to track Claude usage in real time

**原文标题**: Show HN: macOS menu bar app to track Claude usage in real time

**原文链接**: [https://github.com/richhickson/claudecodeusage](https://github.com/richhickson/claudecodeusage)

生成摘要时出错

---

## 47. Show HN: I made a memory game to teach you to play piano by ear

**原文标题**: Show HN: I made a memory game to teach you to play piano by ear

**原文链接**: [https://lend-me-your-ears.specr.net](https://lend-me-your-ears.specr.net)

生成摘要时出错

---

## 48. U.S. is withdrawing from 66 international bodies

**原文标题**: U.S. is withdrawing from 66 international bodies

**原文链接**: [https://www.whitehouse.gov/fact-sheets/2026/01/fact-sheet-president-donald-j-trump-withdraws-the-united-states-from-international-organizations-that-are-contrary-to-the-interests-of-the-united-states/](https://www.whitehouse.gov/fact-sheets/2026/01/fact-sheet-president-donald-j-trump-withdraws-the-united-states-from-international-organizations-that-are-contrary-to-the-interests-of-the-united-states/)

生成摘要时出错

---

## 49. MCP is a fad

**原文标题**: MCP is a fad

**原文链接**: [https://tombedor.dev/mcp-is-a-fad/](https://tombedor.dev/mcp-is-a-fad/)

生成摘要时出错

---

## 50. Chase to become new issuer of Apple Card

**原文标题**: Chase to become new issuer of Apple Card

**原文链接**: [https://www.jpmorganchase.com/ir/news/2026/chase-to-become-new-issuer-of-apple-card](https://www.jpmorganchase.com/ir/news/2026/chase-to-become-new-issuer-of-apple-card)

生成摘要时出错

---

## 51. Ushikuvirus: Newly discovered virus may offer clues to the origin of eukaryotes

**原文标题**: Ushikuvirus: Newly discovered virus may offer clues to the origin of eukaryotes

**原文链接**: [https://www.tus.ac.jp/en/mediarelations/archive/20251219_9539.html](https://www.tus.ac.jp/en/mediarelations/archive/20251219_9539.html)

生成摘要时出错

---

## 52. Musashi: Motorola 680x0 emulator written in C

**原文标题**: Musashi: Motorola 680x0 emulator written in C

**原文链接**: [https://github.com/kstenerud/Musashi](https://github.com/kstenerud/Musashi)

生成摘要时出错

---

## 53. The virtual AmigaOS runtime (a.k.a. Wine for Amiga:)

**原文标题**: The virtual AmigaOS runtime (a.k.a. Wine for Amiga:)

**原文链接**: [https://github.com/cnvogelg/amitools/blob/main/docs/vamos.md](https://github.com/cnvogelg/amitools/blob/main/docs/vamos.md)

生成摘要时出错

---

## 54. Digital Red Queen: Adversarial Program Evolution in Core War with LLMs

**原文标题**: Digital Red Queen: Adversarial Program Evolution in Core War with LLMs

**原文链接**: [https://sakana.ai/drq/](https://sakana.ai/drq/)

生成摘要时出错

---

## 55. Show HN: I visualized the entire history of Citi Bike in the browser

**原文标题**: Show HN: I visualized the entire history of Citi Bike in the browser

**原文链接**: [https://bikemap.nyc/](https://bikemap.nyc/)

生成摘要时出错

---

## 56. Surveillance Watch – A map that shows connections between surveillance companies

**原文标题**: Surveillance Watch – A map that shows connections between surveillance companies

**原文链接**: [https://www.surveillancewatch.io](https://www.surveillancewatch.io)

生成摘要时出错

---

## 57. Why is SendGrid emailing me about supporting ICE?

**原文标题**: Why is SendGrid emailing me about supporting ICE?

**原文链接**: [https://fredbenenson.com/blog/2026/01/09/why-is-sendgrid-emailing-me-about-supporting-ice/](https://fredbenenson.com/blog/2026/01/09/why-is-sendgrid-emailing-me-about-supporting-ice/)

生成摘要时出错

---

## 58. X faces global investigations for deepfake porn of women and minors

**原文标题**: X faces global investigations for deepfake porn of women and minors

**原文链接**: [https://boingboing.net/2026/01/06/x-faces-global-investigations-as-grok-generates-deepfake-porn-of-women-and-minors.html](https://boingboing.net/2026/01/06/x-faces-global-investigations-as-grok-generates-deepfake-porn-of-women-and-minors.html)

生成摘要时出错

---

## 59. Texas court blocks Samsung from tracking TV viewing, then vacates order

**原文标题**: Texas court blocks Samsung from tracking TV viewing, then vacates order

**原文链接**: [https://www.bleepingcomputer.com/news/security/texas-court-blocks-samsung-from-tracking-tv-viewing-then-vacates-order/](https://www.bleepingcomputer.com/news/security/texas-court-blocks-samsung-from-tracking-tv-viewing-then-vacates-order/)

生成摘要时出错

---

## 60. SQL Studio

**原文标题**: SQL Studio

**原文链接**: [https://sql.studio/](https://sql.studio/)

生成摘要时出错

---

## 61. Claude Code Emergent Behavior: When Skills Combine

**原文标题**: Claude Code Emergent Behavior: When Skills Combine

**原文链接**: [https://vibeandscribe.xyz/posts/2025-01-07-emergent-behavior.html](https://vibeandscribe.xyz/posts/2025-01-07-emergent-behavior.html)

生成摘要时出错

---

## 62. How did TVs get so cheap?

**原文标题**: How did TVs get so cheap?

**原文链接**: [https://www.construction-physics.com/p/how-did-tvs-get-so-cheap](https://www.construction-physics.com/p/how-did-tvs-get-so-cheap)

生成摘要时出错

---

## 63. Chase to become new issuer of Apple Card

**原文标题**: Chase to become new issuer of Apple Card

**原文链接**: [https://www.apple.com/newsroom/2026/01/chase-to-become-new-issuer-of-apple-card/](https://www.apple.com/newsroom/2026/01/chase-to-become-new-issuer-of-apple-card/)

生成摘要时出错

---

## 64. How Hackers Are Fighting Back Against ICE

**原文标题**: How Hackers Are Fighting Back Against ICE

**原文链接**: [https://www.eff.org/deeplinks/2026/01/how-hackers-are-fighting-back-against-ice](https://www.eff.org/deeplinks/2026/01/how-hackers-are-fighting-back-against-ice)

生成摘要时出错

---

## 65. An Honest Review of Go (2025)

**原文标题**: An Honest Review of Go (2025)

**原文链接**: [https://benraz.dev/blog/golang_review.html](https://benraz.dev/blog/golang_review.html)

生成摘要时出错

---

## 66. Show HN: A geofence-based social network app 6 years in development

**原文标题**: Show HN: A geofence-based social network app 6 years in development

**原文链接**: [https://www.localvideoapp.com](https://www.localvideoapp.com)

生成摘要时出错

---

## 67. Tumblr removed from Apple App Store over abuse images (2018)

**原文标题**: Tumblr removed from Apple App Store over abuse images (2018)

**原文链接**: [https://www.bbc.com/news/technology-46275138](https://www.bbc.com/news/technology-46275138)

生成摘要时出错

---

## 68. Grok turns off image generator for most after outcry over sexualised AI imagery

**原文标题**: Grok turns off image generator for most after outcry over sexualised AI imagery

**原文链接**: [https://www.theguardian.com/technology/2026/jan/09/grok-image-generator-outcry-sexualised-ai-imagery](https://www.theguardian.com/technology/2026/jan/09/grok-image-generator-outcry-sexualised-ai-imagery)

生成摘要时出错

---

## 69. SSDs, power loss protection and fsync latency

**原文标题**: SSDs, power loss protection and fsync latency

**原文链接**: [http://smalldatum.blogspot.com/2026/01/ssds-power-loss-protection-and-fsync.html](http://smalldatum.blogspot.com/2026/01/ssds-power-loss-protection-and-fsync.html)

生成摘要时出错

---

## 70. German president says US is destroying world order

**原文标题**: German president says US is destroying world order

**原文链接**: [https://www.reuters.com/world/americas/german-president-says-us-is-destroying-world-order-2026-01-08/](https://www.reuters.com/world/americas/german-president-says-us-is-destroying-world-order-2026-01-08/)

生成摘要时出错

---

## 71. Task-free intelligence testing of LLMs

**原文标题**: Task-free intelligence testing of LLMs

**原文链接**: [https://www.marble.onl/posts/tapping/index.html](https://www.marble.onl/posts/tapping/index.html)

生成摘要时出错

---

## 72. The Trump Administration Says It's Illegal to Record Videos of ICE

**原文标题**: The Trump Administration Says It's Illegal to Record Videos of ICE

**原文链接**: [https://reason.com/2026/01/08/you-have-the-right-to-record-ice/](https://reason.com/2026/01/08/you-have-the-right-to-record-ice/)

生成摘要时出错

---

## 73. Show HN: DeepDream for Video with Temporal Consistency

**原文标题**: Show HN: DeepDream for Video with Temporal Consistency

**原文链接**: [https://github.com/jeremicna/deepdream-video-pytorch](https://github.com/jeremicna/deepdream-video-pytorch)

生成摘要时出错

---

## 74. Texas first state to end American bar association oversight of law schools

**原文标题**: Texas first state to end American bar association oversight of law schools

**原文链接**: [https://www.keranews.org/news/2026-01-06/texas-supreme-court-ends-american-bar-association-law-school-accreditation](https://www.keranews.org/news/2026-01-06/texas-supreme-court-ends-american-bar-association-law-school-accreditation)

生成摘要时出错

---

## 75. Our Changing Planet, as Seen from Space

**原文标题**: Our Changing Planet, as Seen from Space

**原文链接**: [https://e360.yale.edu/digest/nasa-satellite-images-2025](https://e360.yale.edu/digest/nasa-satellite-images-2025)

生成摘要时出错

---

## 76. "They Saw a Protest": Cognitive Illiberalism and the Speech-Conduct Distinction [pdf] (2012)

**原文标题**: "They Saw a Protest": Cognitive Illiberalism and the Speech-Conduct Distinction [pdf] (2012)

**原文链接**: [https://www.stanfordlawreview.org/wp-content/uploads/sites/3/2012/05/Kahan-64-Stan-L-Rev-851.pdf](https://www.stanfordlawreview.org/wp-content/uploads/sites/3/2012/05/Kahan-64-Stan-L-Rev-851.pdf)

生成摘要时出错

---

## 77. Logistics Is Dying; Or – Dude, Where's My Mail?

**原文标题**: Logistics Is Dying; Or – Dude, Where's My Mail?

**原文链接**: [https://lagomor.ph/2026/01/logistics-is-dying-or-dude-wheres-my-mail/](https://lagomor.ph/2026/01/logistics-is-dying-or-dude-wheres-my-mail/)

生成摘要时出错

---

## 78. Memoir by Steve Jobs’ eldest daughter describes ways he was cruel to her (2018)

**原文标题**: Memoir by Steve Jobs’ eldest daughter describes ways he was cruel to her (2018)

**原文链接**: [https://finance.yahoo.com/news/memoir-steve-jobs-apos-daughter-133000491.html](https://finance.yahoo.com/news/memoir-steve-jobs-apos-daughter-133000491.html)

生成摘要时出错

---

## 79. Gmail is entering the Gemini Era

**原文标题**: Gmail is entering the Gemini Era

**原文链接**: [https://blog.google/products-and-platforms/products/gmail/gmail-is-entering-the-gemini-era/](https://blog.google/products-and-platforms/products/gmail/gmail-is-entering-the-gemini-era/)

生成摘要时出错

---

## 80. Supernova Remnant Video from NASA's Chandra Is Decades in Making

**原文标题**: Supernova Remnant Video from NASA's Chandra Is Decades in Making

**原文链接**: [https://www.nasa.gov/missions/chandra/supernova-remnant-video-from-nasas-chandra-is-decades-in-making/](https://www.nasa.gov/missions/chandra/supernova-remnant-video-from-nasas-chandra-is-decades-in-making/)

生成摘要时出错

---

## 81. Minneapolis Mayor Blasts Kristi Noem's BS ICE Shoots Kills Woman in Minnesota

**原文标题**: Minneapolis Mayor Blasts Kristi Noem's BS ICE Shoots Kills Woman in Minnesota

**原文链接**: [https://www.thedailypoliticususa.com/p/minneapolis-mayor-blasts-kristi-noems](https://www.thedailypoliticususa.com/p/minneapolis-mayor-blasts-kristi-noems)

生成摘要时出错

---

## 82. 2026 Predictions Scorecard

**原文标题**: 2026 Predictions Scorecard

**原文链接**: [https://rodneybrooks.com/predictions-scorecard-2026-january-01/](https://rodneybrooks.com/predictions-scorecard-2026-january-01/)

生成摘要时出错

---

## 83. So you wanna de-bog yourself (2024)

**原文标题**: So you wanna de-bog yourself (2024)

**原文链接**: [https://www.experimental-history.com/p/so-you-wanna-de-bog-yourself](https://www.experimental-history.com/p/so-you-wanna-de-bog-yourself)

生成摘要时出错

---

## 84. Why Are Grok and X Still Available in App Stores?

**原文标题**: Why Are Grok and X Still Available in App Stores?

**原文链接**: [https://www.wired.com/story/x-grok-app-store-nudify-csam-apple-google-content-moderation/](https://www.wired.com/story/x-grok-app-store-nudify-csam-apple-google-content-moderation/)

生成摘要时出错

---

## 85. Ubisoft Shuts Assassin's Creed Developer Studio Just Weeks After It Unionized

**原文标题**: Ubisoft Shuts Assassin's Creed Developer Studio Just Weeks After It Unionized

**原文链接**: [https://www.ign.com/articles/ubisoft-shuts-down-assassins-creed-rebellion-developer-halifax-studio-just-weeks-after-it-unionized](https://www.ign.com/articles/ubisoft-shuts-down-assassins-creed-rebellion-developer-halifax-studio-just-weeks-after-it-unionized)

生成摘要时出错

---

## 86. Chinese AI models have lagged the US frontier by 7 months on average since 2023

**原文标题**: Chinese AI models have lagged the US frontier by 7 months on average since 2023

**原文链接**: [https://epoch.ai/data-insights/us-vs-china-eci](https://epoch.ai/data-insights/us-vs-china-eci)

生成摘要时出错

---

## 87. Danish troops told to 'shoot first, ask questions later' if US invades Greenland

**原文标题**: Danish troops told to 'shoot first, ask questions later' if US invades Greenland

**原文链接**: [https://www.lbc.co.uk/article/danish-troops-shoot-first-us-greenland-5HjdQNW_2/](https://www.lbc.co.uk/article/danish-troops-shoot-first-us-greenland-5HjdQNW_2/)

生成摘要时出错

---

## 88. Why we're taking legal action against SerpApi's unlawful scraping (2025)

**原文标题**: Why we're taking legal action against SerpApi's unlawful scraping (2025)

**原文链接**: [https://blog.google/innovation-and-ai/technology/safety-security/serpapi-lawsuit/](https://blog.google/innovation-and-ai/technology/safety-security/serpapi-lawsuit/)

生成摘要时出错

---

## 89. US immigration officer fatally shoots woman, 37, in Minneapolis, officials say

**原文标题**: US immigration officer fatally shoots woman, 37, in Minneapolis, officials say

**原文链接**: [https://www.bbc.com/news/live/c7510l1135wt](https://www.bbc.com/news/live/c7510l1135wt)

生成摘要时出错

---

## 90. Nvidia Kicks Off the Next Generation of AI with Rubin

**原文标题**: Nvidia Kicks Off the Next Generation of AI with Rubin

**原文链接**: [https://nvidianews.nvidia.com/news/rubin-platform-ai-supercomputer](https://nvidianews.nvidia.com/news/rubin-platform-ai-supercomputer)

生成摘要时出错

---

## 91. Dynamic Large Concept Models: Latent Reasoning in an Adaptive Semantic Space

**原文标题**: Dynamic Large Concept Models: Latent Reasoning in an Adaptive Semantic Space

**原文链接**: [https://arxiv.org/abs/2512.24617](https://arxiv.org/abs/2512.24617)

生成摘要时出错

---

## 92. Landline phones cut in parts of Iran, eyewitnesses say

**原文标题**: Landline phones cut in parts of Iran, eyewitnesses say

**原文链接**: [https://www.iranintl.com/en/202601085355](https://www.iranintl.com/en/202601085355)

生成摘要时出错

---

## 93. Flint Confirms Biodegradable Paper Batteries Are Now in Production

**原文标题**: Flint Confirms Biodegradable Paper Batteries Are Now in Production

**原文链接**: [https://audioxpress.com/news/flint-confirms-biodegradable-paper-batteries-are-now-in-production](https://audioxpress.com/news/flint-confirms-biodegradable-paper-batteries-are-now-in-production)

生成摘要时出错

---

## 94. ICE agent fatally shoots woman in Minneapolis

**原文标题**: ICE agent fatally shoots woman in Minneapolis

**原文链接**: [https://www.reuters.com/world/us/us-federal-agent-involved-minneapolis-shooting-during-immigration-surge-city-2026-01-07/](https://www.reuters.com/world/us/us-federal-agent-involved-minneapolis-shooting-during-immigration-surge-city-2026-01-07/)

生成摘要时出错

---

## 95. U.S. mandates more foreign travelers to pay $15,000 visa bond deposits

**原文标题**: U.S. mandates more foreign travelers to pay $15,000 visa bond deposits

**原文链接**: [https://www.washingtonpost.com/immigration/2026/01/06/visa-bonds-state-overstay-rates/](https://www.washingtonpost.com/immigration/2026/01/06/visa-bonds-state-overstay-rates/)

生成摘要时出错

---

## 96. Show HN: A Daily Bible Game

**原文标题**: Show HN: A Daily Bible Game

**原文链接**: [https://bibdle.com](https://bibdle.com)

生成摘要时出错

---

## 97. Latest SteamOS Beta Now Includes Ntsync Kernel Driver

**原文标题**: Latest SteamOS Beta Now Includes Ntsync Kernel Driver

**原文链接**: [https://www.phoronix.com/news/Steam-OS-Beta-NTSYNC](https://www.phoronix.com/news/Steam-OS-Beta-NTSYNC)

生成摘要时出错

---

## 98. DHS Invokes Immigration Enforcement to Justify Gathering Americans' DNA

**原文标题**: DHS Invokes Immigration Enforcement to Justify Gathering Americans' DNA

**原文链接**: [https://reason.com/2026/01/09/dhs-invokes-immigration-enforcement-to-justify-gathering-americans-dna/](https://reason.com/2026/01/09/dhs-invokes-immigration-enforcement-to-justify-gathering-americans-dna/)

生成摘要时出错

---

## 99. Iran vows regime will "not back down" as web blackout continues

**原文标题**: Iran vows regime will "not back down" as web blackout continues

**原文链接**: [https://www.cbsnews.com/news/iran-protests-internet-blackout-khamenei-vows-not-back-down-trump-threat/](https://www.cbsnews.com/news/iran-protests-internet-blackout-khamenei-vows-not-back-down-trump-threat/)

生成摘要时出错

---

## 100. 73% People Detained by ICE Have No Convictions

**原文标题**: 73% People Detained by ICE Have No Convictions

**原文链接**: [https://www.cato.org/blog/5-ice-detainees-have-violent-convictions-73-no-convictions](https://www.cato.org/blog/5-ice-detainees-have-violent-convictions-73-no-convictions)

生成摘要时出错

---

