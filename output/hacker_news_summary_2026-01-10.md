# Hacker News 热门文章摘要 (2026-01-10)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 如何用200行代码编写克劳德代码

**原文标题**: How to code Claude Code in 200 lines of code

**原文链接**: [https://www.mihaileric.com/The-Emperor-Has-No-Clothes/](https://www.mihaileric.com/The-Emperor-Has-No-Clothes/)

本文演示了如何用大约200行Python代码构建一个功能性AI编程代理，类似于Claude Code。作者认为，这些工具的“魔力”在于强大的大型语言模型（LLM）与一套本地工具之间直接的对话循环。

这种思维模型包括：
1.  你向LLM发送一条消息。
2.  LLM决定使用一个工具，并以结构化的工具调用形式响应。
3.  你的程序在本地执行该工具。
4.  结果作为上下文发送回LLM。
5.  LLM继续处理或作出响应。

核心代理需要三个基本工具：
*   `read_file_tool`：用于获取文件内容。
*   `list_files_tool`：用于导航目录。
*   `edit_file_tool`：用于创建或修改文件（替换文本，或在`old_str`为空时创建新文件）。

这些工具注册在一个`TOOL_REGISTRY`中。关键一步是通过生成一个动态系统提示来教会LLM这些工具，该提示包含每个工具的名称、描述（来自文档字符串）和签名。这个提示还指定了LLM调用工具时必须使用的确切格式 (`tool: TOOL_NAME({JSON_ARGS})`)。

代理的主循环：
1.  接收用户输入。
2.  使用对话历史和系统提示调用LLM。
3.  解析LLM的响应以识别`tool:`调用。
4.  如果调用了工具，则执行它们，将`tool_result(...)`发送回LLM，并重复内部循环，直到LLM响应时不请求工具。
5.  如果没有调用工具，则打印LLM的响应，并且外部循环等待新的用户输入。

尽管生产级代理会增加错误处理、流式传输和更多工具等功能，但LLM决定做什么、你的代码执行它以及结果回流的底层架构保持不变。本文鼓励读者在此简单而强大的模式基础上进行构建和扩展。

---

## 2. 谷歌AI工作室现已赞助Tailwind CSS

**原文标题**: Google AI Studio is now sponsoring Tailwind CSS

**原文链接**: [https://twitter.com/OfficialLoganK/status/2009339263251566902](https://twitter.com/OfficialLoganK/status/2009339263251566902)

所提供的“文章”内容并未讨论其标题所暗示的 Google AI Studio 对 Tailwind CSS 的所谓赞助。相反，整个内容是一条来自 x.com（前身为 Twitter）的错误消息，以英文和中文两种语言显示。

该消息写道：“We’ve detected that JavaScript is disabled in this browser. Please enable JavaScript or switch to a supported browser to continue using x.com.” 随后，它列出了各种页脚链接，例如“Help Center”、“Terms of Service”、“Privacy Policy”、“Cookie Policy”、“Imprint”和“Ads info”，以及一条版权声明“© 2026 X Corp.”。该文本没有提供任何关于 Google AI Studio、Tailwind CSS 或任何赞助协议的信息。

---

## 3. Cloudflare CEO 谈意大利罚款

**原文标题**: Cloudflare CEO on the Italy fines

**原文链接**: [https://twitter.com/eastdakota/status/2009654937303896492](https://twitter.com/eastdakota/status/2009654937303896492)

生成摘要时出错

---

## 4. 安特罗匹克禁止第三方使用克劳德代码订阅

**原文标题**: Anthropic blocks third-party use of Claude Code subscriptions

**原文链接**: [https://github.com/anomalyco/opencode/issues/7410](https://github.com/anomalyco/opencode/issues/7410)

一个标题为“Broken Claude Max #7410”的GitHub问题于2026年1月9日由用户piotryordanov创建，报告称“claude max停止使用”，并伴随一个未指明的错误。该用户确认尝试重新连接也以相同的错误失败。此问题发生在Mac OS上运行的OpenCode 1.1.8版本中，被标记为“bug”和“某处出现问题”。

正如文章标题所暗示，该问题表明Anthropic已阻止第三方应用程序使用Claude Code订阅，直接导致了所报告的服务中断。该问题获得的巨大反响（320个👍和44个😕）表明，通过OpenCode等第三方集成使用Claude Max服务的众多用户受到了广泛影响。此问题已分配给thdxr。

---

## 5. “Erdos problem #728 was solved more or less autonomously by AI”

**原文标题**: “Erdos problem #728 was solved more or less autonomously by AI”

**原文链接**: [https://mathstodon.xyz/@tao/115855840223258103](https://mathstodon.xyz/@tao/115855840223258103)

The article announces the significant news that Erdos problem #728 has been "more or less autonomously" solved by Artificial Intelligence. This breakthrough is further highlighted by a quote from renowned mathematician Terence Tao on Mathstodon, where he refers to "the application of AI tools to Erdos problems." The core message indicates a major advancement in AI's capability to tackle complex, previously unsolved mathematical challenges, marking a notable milestone in the field.

---

## 6. 让我来介绍，雪铁龙C15

**原文标题**: Allow me to introduce, the Citroen C15

**原文链接**: [https://eupolicy.social/@jmaris/115860595238097654](https://eupolicy.social/@jmaris/115860595238097654)

生成摘要时出错

---

## 7. 越南政府已禁止越狱手机使用任何银行应用。

**原文标题**: The Vietnam government has banned rooted phones from using any banking app

**原文链接**: [https://xdaforums.com/t/discussion-the-root-and-mod-hiding-fingerprint-spoofing-keybox-stealing-cat-and-mouse-game.4425939/page-118](https://xdaforums.com/t/discussion-the-root-and-mod-hiding-fingerprint-spoofing-keybox-stealing-cat-and-mouse-game.4425939/page-118)

提供的文章标题指出，越南政府已禁止root过的手机使用任何银行应用程序。然而，后续内容并未支持或详细阐述这一说法。

相反，其内容是2016年10月用户“zgfg”和“ldeveraux”之间的一段旧论坛讨论。用户ldeveraux正在寻求帮助，解决其设备Google Play商店相关的问题，特别是检查和安装更新的问题，以及尽管尝试清除缓存和数据后仍然持续出现的“空间不足”错误。他们提到使用了“PI中的GMS和Play Store欺骗”（可能是一个root相关工具），并禁用了其中的设置。用户zgfg回应，要求澄清所使用的具体“PI欺骗”工具（例如，“PI Fork”或“PI Fix Inject”）。

该讨论完全集中于在root过或修改过的安卓设备上排查Play商店的功能问题，并未提及银行应用程序、政府法规或越南。

---

## 8. Show HN: I made a memory game to teach you to play piano by ear

**原文标题**: Show HN: I made a memory game to teach you to play piano by ear

**原文链接**: [https://lend-me-your-ears.specr.net](https://lend-me-your-ears.specr.net)

The "Show HN" post announces a new memory game developed to teach users how to play piano by ear. The creator designed this interactive tool to make ear training—a fundamental musical skill—both accessible and engaging.

While specific gameplay mechanics are not detailed, the concept implies auditory challenges where players must listen to, identify, and remember musical notes, intervals, or short melodies. This process aims to enhance pitch recognition, improve auditory memory, and ultimately enable players to replicate sounds on the piano without relying on sheet music.

The accompanying phrase, "Lend Me Your Ears," serves as a direct invitation from the developer, encouraging the Hacker News community to try the game. This call to action seeks engagement, user feedback, and participation in the learning experience, transforming a potentially daunting musical skill into a fun, game-based activity.

---

## 9. 弗洛克硬编码了美国监控基础设施的密码53次

**原文标题**: Flock Hardcoded the Password for America's Surveillance Infrastructure 53 Times

**原文链接**: [https://nexanet.ai/blog/53-times-flocksafety-hardcoded-the-password-for-americas-surveillance-infrastructure](https://nexanet.ai/blog/53-times-flocksafety-hardcoded-the-password-for-americas-surveillance-infrastructure)

生成摘要时出错

---

## 10. Kagi releases alpha version of Orion for Linux

**原文标题**: Kagi releases alpha version of Orion for Linux

**原文链接**: [https://help.kagi.com/orion/misc/linux-status.html](https://help.kagi.com/orion/misc/linux-status.html)

Kagi has released the alpha version of its Orion browser for Linux, an early, unstable build intended primarily for testing. This initial release focuses on core functionality and visual elements.

Users can test all visual components, including main menus, submenus, dialogs, buttons, toolbars, and basic window layouts. Basic website navigation is supported, allowing for homepage access, tab usage, and simple searches. Advanced tab management is largely complete, featuring independent tabs that open in parallel, session persistence to restore previous tabs and history, and tab support in both the main window and left sidebar (though the Tab Switcher UI is still absent).

A basic bookmarks system is implemented, enabling users to save pages, organize them into folders, and view them via a dialog, sidebar, or bookmarks bar. The browser also includes advanced history management and a foundational password management framework, laying the groundwork for future security features.

Key functionalities not yet included but planned for future development are WebKit Extension support and sync infrastructure.

---

## 11. European Commission issues call for evidence on open source

**原文标题**: European Commission issues call for evidence on open source

**原文链接**: [https://lwn.net/Articles/1053107/](https://lwn.net/Articles/1053107/)

生成摘要时出错

---

## 12. Mathematics for Computer Science (2018) [pdf]

**原文标题**: Mathematics for Computer Science (2018) [pdf]

**原文链接**: [https://courses.csail.mit.edu/6.042/spring18/mcs.pdf](https://courses.csail.mit.edu/6.042/spring18/mcs.pdf)

生成摘要时出错

---

## 13. How Markdown took over the world

**原文标题**: How Markdown took over the world

**原文链接**: [https://www.anildash.com/2026/01/09/how-markdown-took-over-the-world/](https://www.anildash.com/2026/01/09/how-markdown-took-over-the-world/)

生成摘要时出错

---

## 14. Let's call a murder a murder

**原文标题**: Let's call a murder a murder

**原文链接**: [https://daringfireball.net/2026/01/lets_call_a_murder_a_murder](https://daringfireball.net/2026/01/lets_call_a_murder_a_murder)

生成摘要时出错

---

## 15. Exercise can be nearly as effective as therapy for depression

**原文标题**: Exercise can be nearly as effective as therapy for depression

**原文链接**: [https://www.sciencedaily.com/releases/2026/01/260107225516.htm](https://www.sciencedaily.com/releases/2026/01/260107225516.htm)

生成摘要时出错

---

## 16. Sopro TTS: A 169M model with zero-shot voice cloning that runs on the CPU

**原文标题**: Sopro TTS: A 169M model with zero-shot voice cloning that runs on the CPU

**原文链接**: [https://github.com/samuel-vitorino/sopro](https://github.com/samuel-vitorino/sopro)

生成摘要时出错

---

## 17. London–Calcutta bus service

**原文标题**: London–Calcutta bus service

**原文链接**: [https://en.wikipedia.org/wiki/London%E2%80%93Calcutta_bus_service](https://en.wikipedia.org/wiki/London%E2%80%93Calcutta_bus_service)

生成摘要时出错

---

## 18. What happened to WebAssembly

**原文标题**: What happened to WebAssembly

**原文链接**: [https://emnudge.dev/blog/what-happened-to-webassembly/](https://emnudge.dev/blog/what-happened-to-webassembly/)

生成摘要时出错

---

## 19. Embassy: Modern embedded framework, using Rust and async

**原文标题**: Embassy: Modern embedded framework, using Rust and async

**原文链接**: [https://github.com/embassy-rs/embassy](https://github.com/embassy-rs/embassy)

生成摘要时出错

---

## 20. JavaScript Demos in 140 Characters

**原文标题**: JavaScript Demos in 140 Characters

**原文链接**: [https://beta.dwitter.net](https://beta.dwitter.net)

生成摘要时出错

---

## 21. Show HN: Scroll Wikipedia like TikTok

**原文标题**: Show HN: Scroll Wikipedia like TikTok

**原文链接**: [https://quack.sdan.io](https://quack.sdan.io)

生成摘要时出错

---

## 22. The unreasonable effectiveness of the Fourier transform

**原文标题**: The unreasonable effectiveness of the Fourier transform

**原文链接**: [https://joshuawise.com/resources/ofdm/](https://joshuawise.com/resources/ofdm/)

生成摘要时出错

---

## 23. Oh My Zsh adds bloat

**原文标题**: Oh My Zsh adds bloat

**原文链接**: [https://rushter.com/blog/zsh-shell/](https://rushter.com/blog/zsh-shell/)

生成摘要时出错

---

## 24. A Eulogy for Dark Sky, a Data Visualization Masterpiece (2023)

**原文标题**: A Eulogy for Dark Sky, a Data Visualization Masterpiece (2023)

**原文链接**: [https://nightingaledvs.com/dark-sky-weather-data-viz/](https://nightingaledvs.com/dark-sky-weather-data-viz/)

生成摘要时出错

---

## 25. Richard D. James aka Aphex Twin speaks to Tatsuya Takahashi (2017)

**原文标题**: Richard D. James aka Aphex Twin speaks to Tatsuya Takahashi (2017)

**原文链接**: [https://web.archive.org/web/20180719052026/http://item.warp.net/interview/aphex-twin-speaks-to-tatsuya-takahashi/](https://web.archive.org/web/20180719052026/http://item.warp.net/interview/aphex-twin-speaks-to-tatsuya-takahashi/)

生成摘要时出错

---

## 26. I replaced Windows with Linux and everything's going great

**原文标题**: I replaced Windows with Linux and everything's going great

**原文链接**: [https://www.theverge.com/tech/858910/linux-diary-gaming-desktop](https://www.theverge.com/tech/858910/linux-diary-gaming-desktop)

生成摘要时出错

---

## 27. RTX 5090 and Raspberry Pi: Can it game?

**原文标题**: RTX 5090 and Raspberry Pi: Can it game?

**原文链接**: [https://scottjg.com/posts/2026-01-08-crappy-computer-showdown/](https://scottjg.com/posts/2026-01-08-crappy-computer-showdown/)

生成摘要时出错

---

## 28. Why I left iNaturalist

**原文标题**: Why I left iNaturalist

**原文链接**: [https://kueda.net/blog/2026/01/06/why-i-left-inat/](https://kueda.net/blog/2026/01/06/why-i-left-inat/)

生成摘要时出错

---

## 29. Start your meetings at 5 minutes past

**原文标题**: Start your meetings at 5 minutes past

**原文链接**: [https://philipotoole.com/start-your-meetings-at-5-minutes-past/](https://philipotoole.com/start-your-meetings-at-5-minutes-past/)

生成摘要时出错

---

## 30. UK government exempting itself from cyber law inspires little confidence

**原文标题**: UK government exempting itself from cyber law inspires little confidence

**原文链接**: [https://www.theregister.com/2026/01/10/csr_bill_analysis/](https://www.theregister.com/2026/01/10/csr_bill_analysis/)

生成摘要时出错

---

## 31. Microsoft May Have Created the Slowest Windows in 25 Years with Windows 11

**原文标题**: Microsoft May Have Created the Slowest Windows in 25 Years with Windows 11

**原文链接**: [https://www.eteknix.com/microsoft-may-have-created-the-slowest-windows-in-25-years-with-windows-11/](https://www.eteknix.com/microsoft-may-have-created-the-slowest-windows-in-25-years-with-windows-11/)

生成摘要时出错

---

## 32. Do not mistake a resilient global economy for populist success

**原文标题**: Do not mistake a resilient global economy for populist success

**原文链接**: [https://www.economist.com/leaders/2026/01/08/do-not-mistake-a-resilient-global-economy-for-populist-success](https://www.economist.com/leaders/2026/01/08/do-not-mistake-a-resilient-global-economy-for-populist-success)

生成摘要时出错

---

## 33. Video filmed by ICE agent who shot Minneapolis woman emerges

**原文标题**: Video filmed by ICE agent who shot Minneapolis woman emerges

**原文链接**: [https://www.bbc.com/news/articles/cz7yv4524gqo](https://www.bbc.com/news/articles/cz7yv4524gqo)

生成摘要时出错

---

## 34. New information extracted from Snowden PDFs through metadata version analysis

**原文标题**: New information extracted from Snowden PDFs through metadata version analysis

**原文链接**: [https://libroot.org/posts/going-through-snowden-documents-part-4/](https://libroot.org/posts/going-through-snowden-documents-part-4/)

生成摘要时出错

---

## 35. SendGrid isn’t emailing about ICE or BLM – it’s a phishing attack

**原文标题**: SendGrid isn’t emailing about ICE or BLM – it’s a phishing attack

**原文链接**: [https://fredbenenson.com/blog/2026/01/09/sendgrid-isnt-emailing-you-about-ice-or-blm-its-a-phishing-attack/](https://fredbenenson.com/blog/2026/01/09/sendgrid-isnt-emailing-you-about-ice-or-blm-its-a-phishing-attack/)

生成摘要时出错

---

## 36. The No Fakes Act has a “fingerprinting” trap that kills open source?

**原文标题**: The No Fakes Act has a “fingerprinting” trap that kills open source?

**原文链接**: [https://old.reddit.com/r/LocalLLaMA/comments/1q7qcux/the_no_fakes_act_has_a_fingerprinting_trap_that/](https://old.reddit.com/r/LocalLLaMA/comments/1q7qcux/the_no_fakes_act_has_a_fingerprinting_trap_that/)

生成摘要时出错

---

## 37. Iran Protest Map

**原文标题**: Iran Protest Map

**原文链接**: [https://pouyaii.github.io/Iran/](https://pouyaii.github.io/Iran/)

生成摘要时出错

---

## 38. Org Mode Syntax Is One of the Most Reasonable Markup Languages to Use for Text

**原文标题**: Org Mode Syntax Is One of the Most Reasonable Markup Languages to Use for Text

**原文链接**: [https://karl-voit.at/2017/09/23/orgmode-as-markup-only/](https://karl-voit.at/2017/09/23/orgmode-as-markup-only/)

生成摘要时出错

---

## 39. Fixing a Buffer Overflow in Unix v4 Like It's 1973

**原文标题**: Fixing a Buffer Overflow in Unix v4 Like It's 1973

**原文链接**: [https://sigma-star.at/blog/2025/12/unix-v4-buffer-overflow/](https://sigma-star.at/blog/2025/12/unix-v4-buffer-overflow/)

生成摘要时出错

---

## 40. Show HN: Rocket Launch and Orbit Simulator

**原文标题**: Show HN: Rocket Launch and Orbit Simulator

**原文链接**: [https://www.donutthejedi.com/](https://www.donutthejedi.com/)

生成摘要时出错

---

## 41. OLED, Not for Me

**原文标题**: OLED, Not for Me

**原文链接**: [https://nuxx.net/blog/2026/01/09/oled-not-for-me/](https://nuxx.net/blog/2026/01/09/oled-not-for-me/)

生成摘要时出错

---

## 42. My article on why AI is great (or terrible) or how to use it

**原文标题**: My article on why AI is great (or terrible) or how to use it

**原文链接**: [https://matthewrocklin.com/ai-zealotry/](https://matthewrocklin.com/ai-zealotry/)

生成摘要时出错

---

## 43. MCP is a fad

**原文标题**: MCP is a fad

**原文链接**: [https://tombedor.dev/mcp-is-a-fad/](https://tombedor.dev/mcp-is-a-fad/)

生成摘要时出错

---

## 44. Scientists discover oldest poison, on 60k-year-old arrows

**原文标题**: Scientists discover oldest poison, on 60k-year-old arrows

**原文链接**: [https://www.nytimes.com/2026/01/07/science/poison-arrows-south-africa.html](https://www.nytimes.com/2026/01/07/science/poison-arrows-south-africa.html)

生成摘要时出错

---

## 45. Open Chaos: A self-evolving open-source project

**原文标题**: Open Chaos: A self-evolving open-source project

**原文链接**: [https://www.openchaos.dev/](https://www.openchaos.dev/)

生成摘要时出错

---

## 46. How to store a chess position in 26 bytes (2022)

**原文标题**: How to store a chess position in 26 bytes (2022)

**原文链接**: [https://ezzeriesa.notion.site/How-to-store-a-chess-position-in-26-bytes-using-bit-level-magic-df1fdb5364eb42fdac11eb23b25e9605](https://ezzeriesa.notion.site/How-to-store-a-chess-position-in-26-bytes-using-bit-level-magic-df1fdb5364eb42fdac11eb23b25e9605)

生成摘要时出错

---

## 47. Surveillance Watch – A map that shows connections between surveillance companies

**原文标题**: Surveillance Watch – A map that shows connections between surveillance companies

**原文链接**: [https://www.surveillancewatch.io](https://www.surveillancewatch.io)

生成摘要时出错

---

## 48. Texas court blocks Samsung from tracking TV viewing, then vacates order

**原文标题**: Texas court blocks Samsung from tracking TV viewing, then vacates order

**原文链接**: [https://www.bleepingcomputer.com/news/security/texas-court-blocks-samsung-from-tracking-tv-viewing-then-vacates-order/](https://www.bleepingcomputer.com/news/security/texas-court-blocks-samsung-from-tracking-tv-viewing-then-vacates-order/)

生成摘要时出错

---

## 49. X faces global investigations for deepfake porn of women and minors

**原文标题**: X faces global investigations for deepfake porn of women and minors

**原文链接**: [https://boingboing.net/2026/01/06/x-faces-global-investigations-as-grok-generates-deepfake-porn-of-women-and-minors.html](https://boingboing.net/2026/01/06/x-faces-global-investigations-as-grok-generates-deepfake-porn-of-women-and-minors.html)

生成摘要时出错

---

## 50. Latest SteamOS Beta Now Includes Ntsync Kernel Driver

**原文标题**: Latest SteamOS Beta Now Includes Ntsync Kernel Driver

**原文链接**: [https://www.phoronix.com/news/Steam-OS-Beta-NTSYNC](https://www.phoronix.com/news/Steam-OS-Beta-NTSYNC)

生成摘要时出错

---

## 51. CDC staff 'blindsided' as child vaccine schedule unilaterally overhauled

**原文标题**: CDC staff 'blindsided' as child vaccine schedule unilaterally overhauled

**原文链接**: [https://www.unmc.edu/healthsecurity/transmission/2026/01/07/cdc-staff-blindsided-as-child-vaccine-schedule-unilaterally-overhauled/](https://www.unmc.edu/healthsecurity/transmission/2026/01/07/cdc-staff-blindsided-as-child-vaccine-schedule-unilaterally-overhauled/)

生成摘要时出错

---

## 52. SQL Studio

**原文标题**: SQL Studio

**原文链接**: [https://sql.studio/](https://sql.studio/)

生成摘要时出错

---

## 53. U.S. mandates more foreign travelers to pay $15,000 visa bond deposits

**原文标题**: U.S. mandates more foreign travelers to pay $15,000 visa bond deposits

**原文链接**: [https://www.washingtonpost.com/immigration/2026/01/06/visa-bonds-state-overstay-rates/](https://www.washingtonpost.com/immigration/2026/01/06/visa-bonds-state-overstay-rates/)

生成摘要时出错

---

## 54. I got paid minimum wage to solve an impossible problem

**原文标题**: I got paid minimum wage to solve an impossible problem

**原文链接**: [https://tiespetersen.substack.com/p/i-got-paid-minimum-wage-to-solve](https://tiespetersen.substack.com/p/i-got-paid-minimum-wage-to-solve)

生成摘要时出错

---

## 55. Turn a single image into a navigable 3D Gaussian Splat with depth

**原文标题**: Turn a single image into a navigable 3D Gaussian Splat with depth

**原文链接**: [https://lab.revelium.studio/ml-sharp](https://lab.revelium.studio/ml-sharp)

生成摘要时出错

---

## 56. How Hackers Are Fighting Back Against ICE

**原文标题**: How Hackers Are Fighting Back Against ICE

**原文链接**: [https://www.eff.org/deeplinks/2026/01/how-hackers-are-fighting-back-against-ice](https://www.eff.org/deeplinks/2026/01/how-hackers-are-fighting-back-against-ice)

生成摘要时出错

---

## 57. 73% People Detained by ICE Have No Convictions

**原文标题**: 73% People Detained by ICE Have No Convictions

**原文链接**: [https://www.cato.org/blog/5-ice-detainees-have-violent-convictions-73-no-convictions](https://www.cato.org/blog/5-ice-detainees-have-violent-convictions-73-no-convictions)

生成摘要时出错

---

## 58. Washington National Opera Is Leaving the Kennedy Center

**原文标题**: Washington National Opera Is Leaving the Kennedy Center

**原文链接**: [https://www.nytimes.com/2026/01/09/arts/music/washington-national-opera-kennedy-center.html](https://www.nytimes.com/2026/01/09/arts/music/washington-national-opera-kennedy-center.html)

生成摘要时出错

---

## 59. Show HN: A geofence-based social network app 6 years in development

**原文标题**: Show HN: A geofence-based social network app 6 years in development

**原文链接**: [https://www.localvideoapp.com](https://www.localvideoapp.com)

生成摘要时出错

---

## 60. Grok turns off image generator for most after outcry over sexualised AI imagery

**原文标题**: Grok turns off image generator for most after outcry over sexualised AI imagery

**原文链接**: [https://www.theguardian.com/technology/2026/jan/09/grok-image-generator-outcry-sexualised-ai-imagery](https://www.theguardian.com/technology/2026/jan/09/grok-image-generator-outcry-sexualised-ai-imagery)

生成摘要时出错

---

## 61. "They Saw a Protest": Cognitive Illiberalism and the Speech-Conduct Distinction [pdf] (2012)

**原文标题**: "They Saw a Protest": Cognitive Illiberalism and the Speech-Conduct Distinction [pdf] (2012)

**原文链接**: [https://www.stanfordlawreview.org/wp-content/uploads/sites/3/2012/05/Kahan-64-Stan-L-Rev-851.pdf](https://www.stanfordlawreview.org/wp-content/uploads/sites/3/2012/05/Kahan-64-Stan-L-Rev-851.pdf)

生成摘要时出错

---

## 62. Why Is Greenland Part of the Kingdom of Denmark? A Short History

**原文标题**: Why Is Greenland Part of the Kingdom of Denmark? A Short History

**原文链接**: [https://www.diis.dk/en/research/why-is-greenland-part-of-the-kingdom-of-denmark-a-short-history](https://www.diis.dk/en/research/why-is-greenland-part-of-the-kingdom-of-denmark-a-short-history)

生成摘要时出错

---

## 63. Tumblr removed from Apple App Store over abuse images (2018)

**原文标题**: Tumblr removed from Apple App Store over abuse images (2018)

**原文链接**: [https://www.bbc.com/news/technology-46275138](https://www.bbc.com/news/technology-46275138)

生成摘要时出错

---

## 64. Code and Let Live

**原文标题**: Code and Let Live

**原文链接**: [https://fly.io/blog/code-and-let-live/](https://fly.io/blog/code-and-let-live/)

生成摘要时出错

---

## 65. All my new code will be closed-source from now on

**原文标题**: All my new code will be closed-source from now on

**原文链接**: [https://twitter.com/MarcJSchmidt/status/2009688028931875156](https://twitter.com/MarcJSchmidt/status/2009688028931875156)

生成摘要时出错

---

## 66. Task-free intelligence testing of LLMs

**原文标题**: Task-free intelligence testing of LLMs

**原文链接**: [https://www.marble.onl/posts/tapping/index.html](https://www.marble.onl/posts/tapping/index.html)

生成摘要时出错

---

## 67. Show HN: EuConform – Offline-first EU AI Act compliance tool (open source)

**原文标题**: Show HN: EuConform – Offline-first EU AI Act compliance tool (open source)

**原文链接**: [https://github.com/Hiepler/EuConform](https://github.com/Hiepler/EuConform)

生成摘要时出错

---

## 68. Show HN: Various shape regularization algorithms

**原文标题**: Show HN: Various shape regularization algorithms

**原文链接**: [https://github.com/nickponline/shreg](https://github.com/nickponline/shreg)

生成摘要时出错

---

## 69. The Trump Administration Says It's Illegal to Record Videos of ICE

**原文标题**: The Trump Administration Says It's Illegal to Record Videos of ICE

**原文链接**: [https://reason.com/2026/01/08/you-have-the-right-to-record-ice/](https://reason.com/2026/01/08/you-have-the-right-to-record-ice/)

生成摘要时出错

---

## 70. Iran's internet shutdown is chillingly precise and may last some time

**原文标题**: Iran's internet shutdown is chillingly precise and may last some time

**原文链接**: [https://www.theguardian.com/world/2026/jan/10/irans-internet-shutdown-is-strikingly-sophisticated-and-may-last-some-time](https://www.theguardian.com/world/2026/jan/10/irans-internet-shutdown-is-strikingly-sophisticated-and-may-last-some-time)

生成摘要时出错

---

## 71. Logistics Is Dying; Or – Dude, Where's My Mail?

**原文标题**: Logistics Is Dying; Or – Dude, Where's My Mail?

**原文链接**: [https://lagomor.ph/2026/01/logistics-is-dying-or-dude-wheres-my-mail/](https://lagomor.ph/2026/01/logistics-is-dying-or-dude-wheres-my-mail/)

生成摘要时出错

---

## 72. Memoir by Steve Jobs’ eldest daughter describes ways he was cruel to her (2018)

**原文标题**: Memoir by Steve Jobs’ eldest daughter describes ways he was cruel to her (2018)

**原文链接**: [https://finance.yahoo.com/news/memoir-steve-jobs-apos-daughter-133000491.html](https://finance.yahoo.com/news/memoir-steve-jobs-apos-daughter-133000491.html)

生成摘要时出错

---

## 73. Caltrain shows why every region should be moving toward regional rail

**原文标题**: Caltrain shows why every region should be moving toward regional rail

**原文链接**: [https://www.hsrail.org/blog/caltrain-shows-why-every-region-should-be-moving-toward-regional-rail/](https://www.hsrail.org/blog/caltrain-shows-why-every-region-should-be-moving-toward-regional-rail/)

生成摘要时出错

---

## 74. Deno has made its PyPI distribution official

**原文标题**: Deno has made its PyPI distribution official

**原文链接**: [https://github.com/denoland/deno/issues/31254](https://github.com/denoland/deno/issues/31254)

生成摘要时出错

---

## 75. Why Are Grok and X Still Available in App Stores?

**原文标题**: Why Are Grok and X Still Available in App Stores?

**原文链接**: [https://www.wired.com/story/x-grok-app-store-nudify-csam-apple-google-content-moderation/](https://www.wired.com/story/x-grok-app-store-nudify-csam-apple-google-content-moderation/)

生成摘要时出错

---

## 76. Texas first state to end American bar association oversight of law schools

**原文标题**: Texas first state to end American bar association oversight of law schools

**原文链接**: [https://www.keranews.org/news/2026-01-06/texas-supreme-court-ends-american-bar-association-law-school-accreditation](https://www.keranews.org/news/2026-01-06/texas-supreme-court-ends-american-bar-association-law-school-accreditation)

生成摘要时出错

---

## 77. Iran's complete Internet shutdown reaches 24 hours

**原文标题**: Iran's complete Internet shutdown reaches 24 hours

**原文链接**: [https://mastodon.social/@netblocks/115866066884567356](https://mastodon.social/@netblocks/115866066884567356)

生成摘要时出错

---

## 78. Robotopia: A 3D, first-person, talking simulator

**原文标题**: Robotopia: A 3D, first-person, talking simulator

**原文链接**: [https://elbowgreasegames.substack.com/p/introducing-robotopia-a-3d-first](https://elbowgreasegames.substack.com/p/introducing-robotopia-a-3d-first)

生成摘要时出错

---

## 79. DHS Invokes Immigration Enforcement to Justify Gathering Americans' DNA

**原文标题**: DHS Invokes Immigration Enforcement to Justify Gathering Americans' DNA

**原文链接**: [https://reason.com/2026/01/09/dhs-invokes-immigration-enforcement-to-justify-gathering-americans-dna/](https://reason.com/2026/01/09/dhs-invokes-immigration-enforcement-to-justify-gathering-americans-dna/)

生成摘要时出错

---

## 80. Amiga Pointer Archive

**原文标题**: Amiga Pointer Archive

**原文链接**: [https://heckmeck.de/pointers/](https://heckmeck.de/pointers/)

生成摘要时出错

---

## 81. Landlords are using automated services to monitor tenant promotions

**原文标题**: Landlords are using automated services to monitor tenant promotions

**原文链接**: [https://old.reddit.com/r/shitrentals/comments/1q38sh4/if_you_get_promoted_at_work_keep_it_a_secret_from/](https://old.reddit.com/r/shitrentals/comments/1q38sh4/if_you_get_promoted_at_work_keep_it_a_secret_from/)

生成摘要时出错

---

## 82. Flint Confirms Biodegradable Paper Batteries Are Now in Production

**原文标题**: Flint Confirms Biodegradable Paper Batteries Are Now in Production

**原文链接**: [https://audioxpress.com/news/flint-confirms-biodegradable-paper-batteries-are-now-in-production](https://audioxpress.com/news/flint-confirms-biodegradable-paper-batteries-are-now-in-production)

Flint, a Singapore-based company, has announced that its sustainable, cellulose-based, biodegradable, PFAS-free paper batteries have entered production in Singapore. This technology offers a promising lower-carbon alternative for consumer electronics, designed to be rechargeable, non-toxic, non-flammable, and non-explosive.

Flint's proprietary batteries use cellulose paper at their core for all key components, remaining operational even when damaged and integrating easily with existing manufacturing processes. The purpose-built production line in Singapore utilizes water-based methods, aiming to reduce reliance on traditional battery materials like lithium, nickel, cobalt, and lead, and enabling improved end-of-life options.

This production milestone follows a successful 2025 for Flint, which included winning the Best of CES Sustainability Award at CES 2025. The company has since expanded its commercial pipeline, secured US$2 million in funding, and initiated pilot programs with global brands like Logitech, while also collaborating with MIT's Climate Tech Accelerator.

Flint will formally unveil its first two commercial paper battery products with live demonstrations at CES 2026. Beyond Singapore, the company is preparing for further expansion into Europe and is developing a solid-state derivative of its chemistry for higher-density applications. Initial battery allocations will prioritize pilot deployments and early commercial rollouts with strategic partners.

---

## 83. AI is a business model stress test

**原文标题**: AI is a business model stress test

**原文链接**: [https://dri.es/ai-is-a-business-model-stress-test](https://dri.es/ai-is-a-business-model-stress-test)

生成摘要时出错

---

## 84. Iran vows regime will "not back down" as web blackout continues

**原文标题**: Iran vows regime will "not back down" as web blackout continues

**原文链接**: [https://www.cbsnews.com/news/iran-protests-internet-blackout-khamenei-vows-not-back-down-trump-threat/](https://www.cbsnews.com/news/iran-protests-internet-blackout-khamenei-vows-not-back-down-trump-threat/)

生成摘要时出错

---

## 85. Circumcision classed as possible child abuse in draft CPS document

**原文标题**: Circumcision classed as possible child abuse in draft CPS document

**原文链接**: [https://www.theguardian.com/society/2026/jan/10/circumcision-classed-as-possible-child-abuse-in-draft-cps-document](https://www.theguardian.com/society/2026/jan/10/circumcision-classed-as-possible-child-abuse-in-draft-cps-document)

生成摘要时出错

---

## 86. See it with your lying ears

**原文标题**: See it with your lying ears

**原文链接**: [https://lcamtuf.substack.com/p/see-it-with-your-lying-ears](https://lcamtuf.substack.com/p/see-it-with-your-lying-ears)

生成摘要时出错

---

## 87. Landline phones cut in parts of Iran, eyewitnesses say

**原文标题**: Landline phones cut in parts of Iran, eyewitnesses say

**原文链接**: [https://www.iranintl.com/en/202601085355](https://www.iranintl.com/en/202601085355)

生成摘要时出错

---

## 88. NASA announces unprecedented return of sick ISS astronaut and crew

**原文标题**: NASA announces unprecedented return of sick ISS astronaut and crew

**原文链接**: [https://www.livescience.com/space/space-exploration/nasa-cancels-spacewalk-and-considers-early-crew-return-from-iss-due-to-medical-issues](https://www.livescience.com/space/space-exploration/nasa-cancels-spacewalk-and-considers-early-crew-return-from-iss-due-to-medical-issues)

生成摘要时出错

---

## 89. My mouse stopped working because Logitech's servers went down

**原文标题**: My mouse stopped working because Logitech's servers went down

**原文链接**: [https://old.reddit.com/r/logitech/comments/1q621k6/logi_options_is_down/](https://old.reddit.com/r/logitech/comments/1q621k6/logi_options_is_down/)

生成摘要时出错

---

## 90. Cloudspecs: Cloud Hardware Evolution Through the Looking Glass

**原文标题**: Cloudspecs: Cloud Hardware Evolution Through the Looking Glass

**原文链接**: [http://muratbuffalo.blogspot.com/2026/01/cloudspecs-cloud-hardware-evolution.html](http://muratbuffalo.blogspot.com/2026/01/cloudspecs-cloud-hardware-evolution.html)

生成摘要时出错

---

## 91. US oil giant ExxonMobil says Venezuela is 'uninvestable'

**原文标题**: US oil giant ExxonMobil says Venezuela is 'uninvestable'

**原文链接**: [https://www.ft.com/content/4c21c031-443e-4834-a7a6-3dd59672b54e](https://www.ft.com/content/4c21c031-443e-4834-a7a6-3dd59672b54e)

生成摘要时出错

---

## 92. "If Starmer is successful in banning X in Britain, I will move forward in . . ."

**原文标题**: "If Starmer is successful in banning X in Britain, I will move forward in . . ."

**原文链接**: [https://twitter.com/RepLuna/status/2009460496668426449](https://twitter.com/RepLuna/status/2009460496668426449)

生成摘要时出错

---

## 93. Tim Cook and Sundar Pichai are cowards

**原文标题**: Tim Cook and Sundar Pichai are cowards

**原文链接**: [https://www.theverge.com/policy/859902/apple-google-run-by-cowards](https://www.theverge.com/policy/859902/apple-google-run-by-cowards)

生成摘要时出错

---

## 94. How Terminals Work

**原文标题**: How Terminals Work

**原文链接**: [https://how-terminals-work.vercel.app/](https://how-terminals-work.vercel.app/)

生成摘要时出错

---

## 95. "We write to ask that you enforce your app stores' terms of service against X" [pdf]

**原文标题**: "We write to ask that you enforce your app stores' terms of service against X" [pdf]

**原文链接**: [https://www.wyden.senate.gov/imo/media/doc/letter_to_apple_and_google_on_removing_x_and_grok_from_app_store_192026pdf.pdf](https://www.wyden.senate.gov/imo/media/doc/letter_to_apple_and_google_on_removing_x_and_grok_from_app_store_192026pdf.pdf)

生成摘要时出错

---

## 96. QtNat – Open you port with Qt UPnP

**原文标题**: QtNat – Open you port with Qt UPnP

**原文链接**: [http://renaudguezennec.eu/index.php/2026/01/09/qtnat-open-you-port-with-qt/](http://renaudguezennec.eu/index.php/2026/01/09/qtnat-open-you-port-with-qt/)

生成摘要时出错

---

## 97. Monero Replaced Bitcoin on the Internet's Underground

**原文标题**: Monero Replaced Bitcoin on the Internet's Underground

**原文链接**: [https://darknetbible.info/news/how-monero-replaced-bitcoin-on-the-darknet/](https://darknetbible.info/news/how-monero-replaced-bitcoin-on-the-darknet/)

生成摘要时出错

---

## 98. USDA suspends federal financial awards to Minnesota and Minneapolis

**原文标题**: USDA suspends federal financial awards to Minnesota and Minneapolis

**原文链接**: [https://turnto10.com/news/nation-world/enough-is-enough-usda-suspends-federal-financial-awards-to-minnesota-and-minneapolis-fraud-scheme-investigation-governor-tim-walz-mayor-jacob-frey-nick-shirley-feeding-our-children-food-programs](https://turnto10.com/news/nation-world/enough-is-enough-usda-suspends-federal-financial-awards-to-minnesota-and-minneapolis-fraud-scheme-investigation-governor-tim-walz-mayor-jacob-frey-nick-shirley-feeding-our-children-food-programs)

生成摘要时出错

---

## 99. Sigmund Freud's Begonia

**原文标题**: Sigmund Freud's Begonia

**原文链接**: [https://observer.co.uk/news/first-person/article/emma-freud-sigmund-freuds-begonia](https://observer.co.uk/news/first-person/article/emma-freud-sigmund-freuds-begonia)

生成摘要时出错

---

## 100. Why Are Federal Agents Using GoPros, Smart Glasses, and Phones to Record Us?

**原文标题**: Why Are Federal Agents Using GoPros, Smart Glasses, and Phones to Record Us?

**原文链接**: [https://gizmodo.com/why-are-federal-agents-using-gopros-smart-glasses-and-phones-to-record-us-2000707835](https://gizmodo.com/why-are-federal-agents-using-gopros-smart-glasses-and-phones-to-record-us-2000707835)

生成摘要时出错

---

