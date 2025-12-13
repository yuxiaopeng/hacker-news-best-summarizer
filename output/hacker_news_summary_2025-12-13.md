# Hacker News 热门文章摘要 (2025-12-13)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 苹果已锁定我的Apple ID，我申诉无门。求助

**原文标题**: Apple has locked my Apple ID, and I have no recourse. A plea for help

**原文链接**: [https://hey.paris/posts/appleid/](https://hey.paris/posts/appleid/)

资深苹果用户兼开发者巴黎（Paris）的Apple ID被永久锁定，导致价值超过3万美元的设备形同“砖块”，并失去对数十年数据、已购软件和其专业数字身份的访问权限。此事源于他试图兑换一张购自大型实体零售商的500美元苹果礼品卡，但兑换失败，并被怀疑可能已被盗用。苹果随后以违反“Apple媒体服务条款和条件”为由禁用了其账户。

尽管苹果声称受影响的仅是媒体服务，但巴黎（Paris）因认证错误，已无法使用iMessage、退出iCloud或访问关键的苹果支持服务。数TB的家庭照片和信息历史记录均无法访问，且目前没有实际方法可以恢复。

苹果支持部门态度冷漠，毫无帮助，拒绝提供禁用的具体原因或升级处理该案件。他们甚至建议创建一个新的Apple ID，但巴黎（Paris）认为这是一个技术上灾难性的解决方案，并可能导致进一步的封禁，尤其考虑到他作为苹果开发者以及苹果编程技术书籍作者的专业身份。

作为近30年的忠实用户和苹果开发者社区的知名人物，巴黎（Paris）认为一次自动化的欺诈标记触发了“核打击式”的回应。他正在恳求人工审查他的案件，以恢复他的数字生活，强调了他绝望的处境以及由此造成的巨大个人和职业损失。

---

## 2. 厌倦智能电视？你的最佳选择。

**原文标题**: Sick of smart TVs? Here are your best options

**原文链接**: [https://arstechnica.com/gadgets/2025/12/the-ars-technica-guide-to-dumb-tvs/](https://arstechnica.com/gadgets/2025/12/the-ars-technica-guide-to-dumb-tvs/)

对智能电视的隐私问题、广告和复杂性感到沮丧？本文提供了一些替代方案，以获得更简单的观看体验。首要建议是将智能电视离线，并连接一个Apple TV机顶盒。这种设置用苹果更简洁、无广告的tvOS取代了电视内置的侵入性操作系统，确保了更好的隐私、可靠性和易用性，同时仍可访问先进的显示技术。用户可以通过路由器阻止电视的互联网访问，或者在Google TV上使用“基本电视”模式。

对于那些寻求真正“非智能”显示器的人来说，像Emerson、Westinghouse和Sceptre这样的品牌提供非智能型号，不过这些通常在图像和音质方面有所妥协，缺乏高端功能。在亚马逊上搜索也可以帮助找到这些选项。

替代的显示解决方案包括投影仪，它们提供大屏幕尺寸，但需要昏暗的环境；以及电脑显示器，它们提供详细的规格和高刷新率，尤其适用于小屏幕，但缺乏电视调谐器和通常没有内置扬声器。数字标牌显示器经久耐用，但往往更昂贵，且不适合家庭娱乐优化。

为了驱动这些非智能显示器，用户可以连接笔记本电脑或手机等设备。笔记本电脑提供广泛的自定义选项、广泛的流媒体服务访问（尽管4K/HDR流媒体可能对浏览器/GPU有特定要求）以及多视图功能。从沙发上舒适地控制可能需要蓝牙鼠标/键盘或空中鼠标。手机可以通过适配器连接，但通常面临分辨率限制（例如，iPhone上的Netflix仅支持1080p），并且与某些服务的屏幕镜像存在不一致性。

至关重要的是，任何旨在播放4K或HDR内容的设置，都必须确保显示器和连接设备都符合HDCP 2.2标准。

---

## 3. OpenAI 悄然采用技能，现已登陆 ChatGPT 和 Codex CLI

**原文标题**: OpenAI are quietly adopting skills, now available in ChatGPT and Codex CLI

**原文链接**: [https://simonwillison.net/2025/Dec/12/openai-skills/](https://simonwillison.net/2025/Dec/12/openai-skills/)

2025年12月12日，这篇文章宣布OpenAI正在悄然将“技能（skills）”集成到ChatGPT的Code Interpreter和Codex CLI工具中，此举模仿了Anthropic早期的实现方式。技能的实现方式很简单：一个包含Markdown文件和可选资源的文件夹，旨在让能够进行文件系统导航的LLM轻松采用。

在ChatGPT中，技能位于一个新的`/home/oai/skills`文件夹中，支持电子表格、DOCX和PDF文件。对于文档和PDF文件，OpenAI的方法是将页面转换为PNG图片，然后使用具备视觉能力的GPT模型进行处理，以保留布局和图形细节。一个例子展示了GPT-5.2精心创建了一个PDF摘要，包括对字体兼容性的自我修正。

另外，OpenAI的开源Codex CLI最近增加了对技能的实验性支持。`~/.codex/skills`中的任何文件夹都可以作为一项技能，通过`--enable skills`选项激活。作者成功地使用Codex CLI生成了一个Datasette插件，展示了其实际应用。

作者强调，OpenAI的迅速采纳验证了他此前对技能是一项非常重要的发展的评估，并呼吁对其进行正式的文档编写，最好由Agentic AI Foundation来完成。

---

## 4. macOS 26.2 支持基于雷雳RDMA的快速AI集群

**原文标题**: macOS 26.2 enables fast AI clusters with RDMA over Thunderbolt

**原文链接**: [https://developer.apple.com/documentation/macos-release-notes/macos-26_2-release-notes#RDMA-over-Thunderbolt](https://developer.apple.com/documentation/macos-release-notes/macos-26_2-release-notes#RDMA-over-Thunderbolt)

所提供的内容不包含题为“macOS 26.2 通过雷电上的RDMA实现快速AI集群”的文章。相反，它显示一条消息，指出该页面需要JavaScript且无法查看。

因此，无法总结该预期文章的主要观点和关键信息。该标题表明，文章将详细介绍macOS 26.2（可能代号为“Tahoe”）如何通过在雷电技术上实现远程直接内存访问（RDMA）来促进高速AI集群，这将显著增强AI工作负载的数据传输和处理能力。然而，支持这一点的实际内容却无法获取。

---

## 5. 诺基亚 N900 起死回生

**原文标题**: Nokia N900 Necromancy

**原文链接**: [https://yaky.dev/2025-12-11-nokia-n900-necromancy/](https://yaky.dev/2025-12-11-nokia-n900-necromancy/)

该项目详细介绍了朋友的诺基亚N900“起死回生”的过程，该手机电池已失效，无法启动。作者摒弃了不可靠的替代电池，最初使用超级电容器和电阻器制作了一个原型“假电池”，成功启动了该设备。

后来，这项设计演变为一个定制的3D打印外壳，可容纳十个小型超级电容器（总计0.5F），并能适配电池仓。在测试过程中，电源波动损坏了内部操作系统，这促使作者改为从SD卡启动。

试图通过N900原装micro-USB端口统一供电却适得其反，造成了严重后果。该端口本身已知的脆弱性，再加上意外损坏，导致主板上一个关键的+5V焊盘被毁坏，使得原装USB端口彻底失效。

作者并未气馁，进行了“彻底的改造”。一个小型USB-C端口经过物理改造以适应N900的机身。由于空间限制，仅连接了5V和地线，将充电电流限制在0.5A，仅支持基本的USB-A转USB-C线缆充电。随后设计了一个新的3D打印“电池”，用于容纳一个大电容器、一个二极管以及从报废原装电池中取出的控制模块，通过新的USB-C端口供电。

这种定制的解决方案成功地“复活”了N900，使其能够从SD卡启动，并以网络收音机设备的身份找到了新的用途。

---

## 6. 谷歌取消收录了熊博客，我不知道为什么。

**原文标题**: Google de-indexed Bear Blog and I don't know why

**原文链接**: [https://journal.james-zhan.com/google-de-indexed-my-entire-bear-blog-and-i-dont-know-why/](https://journal.james-zhan.com/google-de-indexed-my-entire-bear-blog-and-i-dont-know-why/)

詹姆斯·詹在blog.james-zhan.com上的Bear Blog，尽管最初成功收录，但由于未知原因，其在Google上被完全取消索引。问题始于10月14日，当时詹不小心为RSS订阅源URL启动了Google Search Console (GSC) 验证。截至10月20日，他除一篇博文外，所有文章都已被取消索引，显示状态为“已抓取 - 当前未编入索引”，最后一篇文章也在11月3日被取消索引。

詹进行了大量的故障排除工作。他通过在另一个子域名 (www.james-zhan.com) 上成功索引另一个Bear Blog，排除了域名问题。内容质量或数量也被排除，因为其他极简主义的Bear博客收录正常。同样，URL结构也不是原因，这已通过使用相同默认设置的其他Bear博客证实。Bear Blog的创始人Herman也确认博客或其CSS代码没有阻止索引的技术问题。关键是，该博客仍被DuckDuckGo、Bing和Brave等其他搜索引擎正常索引，这表明网站本身没有内在的技术缺陷。

詹无法解决这个神秘的取消索引问题，于是将他的博客迁移到一个新的子域名journal.james-zhan.com（当前网站），将域名转发转移到Porkbun，并设置了重定向。对于新博客，他决定不再手动向GSC提交站点地图，希望其能自然索引。詹现在寻求公众的帮助，以了解最初取消索引的原因。

---

## 7. Epic在iOS支付案胜诉后，庆祝“苹果税”的终结。

**原文标题**: Epic celebrates "the end of the Apple Tax" after court win in iOS payments case

**原文链接**: [https://arstechnica.com/tech-policy/2025/12/epic-celebrates-the-end-of-the-apple-tax-after-appeals-court-win-in-ios-payments-case/](https://arstechnica.com/tech-policy/2025/12/epic-celebrates-the-end-of-the-apple-tax-after-appeals-court-win-in-ios-payments-case/)

The Ninth Circuit Court of Appeals has largely upheld a lower court's ruling finding Apple in "willful violation" of a 2021 injunction concerning iOS App Store payments. Epic Games CEO Tim Sweeney hailed the decision as "the end of the Apple Tax" in the USA, anticipating "untaxed competition" on iOS payments worldwide.

The appeals court affirmed that Apple's initial 27 percent fee for external payment options was "prohibitive" and its restrictions on external links were "overly broad." It also agreed that Apple acted in "bad faith" by resisting compliance. However, the appellate court did modify the lower court's blanket ban on fees, suggesting Apple *can* charge a "reasonable fee" based on its "actual costs to ensure user security and privacy." Sweeney believes these should be minimal, covering only app review costs.

Sweeney expects "rapid adoption" of outside payment processors, including Epic Web Shops, predicting web payments will be the norm by next year. He also highlighted a widespread "fear of retaliation" among developers, where Apple allegedly uses "soft power"—like delaying app reviews or burying products—against those using alternative payment methods. Sweeney called this "totally illegal" and urged regulators to address this pervasive fear, stating, "everybody’s afraid of Apple." Apple has not yet commented.

---

## 8. UK House of Lords attempting to ban use of VPNs by anyone under 16

**原文标题**: UK House of Lords attempting to ban use of VPNs by anyone under 16

**原文链接**: [https://alecmuffett.com/article/134925](https://alecmuffett.com/article/134925)

生成摘要时出错

---

## 9. Rats Play DOOM

**原文标题**: Rats Play DOOM

**原文链接**: [https://ratsplaydoom.com/](https://ratsplaydoom.com/)

生成摘要时出错

---

## 10. SQLite JSON at full index speed using generated columns

**原文标题**: SQLite JSON at full index speed using generated columns

**原文链接**: [https://www.dbpro.app/blog/sqlite-json-virtual-columns-indexing](https://www.dbpro.app/blog/sqlite-json-virtual-columns-indexing)

生成摘要时出错

---

## 11. The Tor Project is switching to Rust

**原文标题**: The Tor Project is switching to Rust

**原文链接**: [https://itsfoss.com/news/tor-rust-rewrite-progress/](https://itsfoss.com/news/tor-rust-rewrite-progress/)

The Tor Project is gradually transitioning its core network from its original C codebase to Rust due to persistent memory safety issues like buffer overflows and use-after-free bugs. This rewrite, named Arti, leverages Rust's memory safety features to enhance security.

A recent release, Arti 1.8.0, introduces significant improvements. The main highlight is a rework of circuit timeouts. Previously, Tor used a predictable "Circuit Dirty Timeout" (CDT), which could aid in traffic fingerprinting. Arti 1.8.0 implements usage-based timeouts with separate, randomized timers for accepting new connections and closing idle circuits, thus reducing fingerprinting risks.

Additionally, the release includes an experimental `arti hsc ctor-migrate` command. This tool allows onion service operators to easily migrate their restricted discovery keys (which manage client authorization) from the C-based Tor to Arti's keystore, automating a previously manual process. Other enhancements cover routing architecture, protocol implementation, directory cache support, and OR port listener configuration.

---

## 12. Denial of service and source code exposure in React Server Components

**原文标题**: Denial of service and source code exposure in React Server Components

**原文链接**: [https://react.dev/blog/2025/12/11/denial-of-service-and-source-code-exposure-in-react-server-components](https://react.dev/blog/2025/12/11/denial-of-service-and-source-code-exposure-in-react-server-components)

生成摘要时出错

---

## 13. An SVG is all you need

**原文标题**: An SVG is all you need

**原文链接**: [https://jon.recoil.org/blog/2025/12/an-svg-is-all-you-need.html](https://jon.recoil.org/blog/2025/12/an-svg-is-all-you-need.html)

生成摘要时出错

---

## 14. Id Software devs form "wall-to-wall" union

**原文标题**: Id Software devs form "wall-to-wall" union

**原文链接**: [https://www.rockpapershotgun.com/id-software-devs-form-wall-to-wall-union-with-165-workers-at-doom-studio-the-latest-to-vote-in-favour](https://www.rockpapershotgun.com/id-software-devs-form-wall-to-wall-union-with-165-workers-at-doom-studio-the-latest-to-vote-in-favour)

生成摘要时出错

---

## 15. Koralm Railway

**原文标题**: Koralm Railway

**原文链接**: [https://infrastruktur.oebb.at/en/projects-for-austria/railway-lines/southern-line-vienna-villach/koralm-railway](https://infrastruktur.oebb.at/en/projects-for-austria/railway-lines/southern-line-vienna-villach/koralm-railway)

生成摘要时出错

---

## 16. GNU Unifont

**原文标题**: GNU Unifont

**原文链接**: [https://unifoundry.com/unifont/index.html](https://unifoundry.com/unifont/index.html)

生成摘要时出错

---

## 17. CRISPR fungus: Protein-packed, sustainable, and tastes like meat

**原文标题**: CRISPR fungus: Protein-packed, sustainable, and tastes like meat

**原文链接**: [https://www.isaaa.org/kc/cropbiotechupdate/article/default.asp?ID=21607](https://www.isaaa.org/kc/cropbiotechupdate/article/default.asp?ID=21607)

生成摘要时出错

---

## 18. My productivity app is a never-ending .txt file (2020)

**原文标题**: My productivity app is a never-ending .txt file (2020)

**原文链接**: [https://jeffhuang.com/productivity_text_file/](https://jeffhuang.com/productivity_text_file/)

生成摘要时出错

---

## 19. The tiniest yet real telescope I've built

**原文标题**: The tiniest yet real telescope I've built

**原文链接**: [https://lucassifoni.info/blog/miniscope-tiny-telescope/](https://lucassifoni.info/blog/miniscope-tiny-telescope/)

生成摘要时出错

---

## 20. Home Depot GitHub token exposed for a year, granted access to internal systems

**原文标题**: Home Depot GitHub token exposed for a year, granted access to internal systems

**原文链接**: [https://techcrunch.com/2025/12/12/home-depot-exposed-access-to-internal-systems-for-a-year-says-researcher/](https://techcrunch.com/2025/12/12/home-depot-exposed-access-to-internal-systems-for-a-year-says-researcher/)

生成摘要时出错

---

## 21. Going Through Snowden Documents, Part 1

**原文标题**: Going Through Snowden Documents, Part 1

**原文链接**: [https://libroot.org/posts/going-through-snowden-documents-part-1/](https://libroot.org/posts/going-through-snowden-documents-part-1/)

生成摘要时出错

---

## 22. Google removes Sci-Hub domains from U.S. search results due to dated court order

**原文标题**: Google removes Sci-Hub domains from U.S. search results due to dated court order

**原文链接**: [https://torrentfreak.com/google-removes-sci-hub-domains-from-u-s-search-results-due-to-dated-court-order/](https://torrentfreak.com/google-removes-sci-hub-domains-from-u-s-search-results-due-to-dated-court-order/)

生成摘要时出错

---

## 23. Framework Raises DDR5 Memory Prices by 50% for DIY Laptops

**原文标题**: Framework Raises DDR5 Memory Prices by 50% for DIY Laptops

**原文链接**: [https://www.phoronix.com/news/Framework-50p-DDR5-Memory](https://www.phoronix.com/news/Framework-50p-DDR5-Memory)

生成摘要时出错

---

## 24. Google releases its new Google Sans Flex font as open source

**原文标题**: Google releases its new Google Sans Flex font as open source

**原文链接**: [https://www.omgubuntu.co.uk/2025/11/google-sans-flex-font-ubuntu](https://www.omgubuntu.co.uk/2025/11/google-sans-flex-font-ubuntu)

生成摘要时出错

---

## 25. 1300 Still Images from the Animated Films of Hayao Miyazaki's Studio Ghibli (2023)

**原文标题**: 1300 Still Images from the Animated Films of Hayao Miyazaki's Studio Ghibli (2023)

**原文链接**: [https://www.ghibli.jp/info/013772/](https://www.ghibli.jp/info/013772/)

生成摘要时出错

---

## 26. CM0 – A new Raspberry Pi you can't buy

**原文标题**: CM0 – A new Raspberry Pi you can't buy

**原文链接**: [https://www.jeffgeerling.com/blog/2025/cm0-new-raspberry-pi-you-cant-buy](https://www.jeffgeerling.com/blog/2025/cm0-new-raspberry-pi-you-cant-buy)

生成摘要时出错

---

## 27. Show HN: Tiny VM sandbox in C with apps in Rust, C and Zig

**原文标题**: Show HN: Tiny VM sandbox in C with apps in Rust, C and Zig

**原文链接**: [https://github.com/ringtailsoftware/uvm32](https://github.com/ringtailsoftware/uvm32)

生成摘要时出错

---

## 28. Ensuring a National Policy Framework for Artificial Intelligence

**原文标题**: Ensuring a National Policy Framework for Artificial Intelligence

**原文链接**: [https://www.whitehouse.gov/presidential-actions/2025/12/eliminating-state-law-obstruction-of-national-artificial-intelligence-policy/](https://www.whitehouse.gov/presidential-actions/2025/12/eliminating-state-law-obstruction-of-national-artificial-intelligence-policy/)

生成摘要时出错

---

## 29. String theory inspires a brilliant, baffling new math proof

**原文标题**: String theory inspires a brilliant, baffling new math proof

**原文链接**: [https://www.quantamagazine.org/string-theory-inspires-a-brilliant-baffling-new-math-proof-20251212/](https://www.quantamagazine.org/string-theory-inspires-a-brilliant-baffling-new-math-proof-20251212/)

生成摘要时出错

---

## 30. Benn Jordan’s flock camera jammer will send you to jail in Florida now [video]

**原文标题**: Benn Jordan’s flock camera jammer will send you to jail in Florida now [video]

**原文链接**: [https://www.youtube.com/watch?v=qEllWdK4l_A](https://www.youtube.com/watch?v=qEllWdK4l_A)

生成摘要时出错

---

## 31. What is the nicest thing a stranger has ever done for you?

**原文标题**: What is the nicest thing a stranger has ever done for you?

**原文链接**: [https://louplummer.lol/nice-stranger/](https://louplummer.lol/nice-stranger/)

生成摘要时出错

---

## 32. Guarding My Git Forge Against AI Scrapers

**原文标题**: Guarding My Git Forge Against AI Scrapers

**原文链接**: [https://vulpinecitrus.info/blog/guarding-git-forge-ai-scrapers/](https://vulpinecitrus.info/blog/guarding-git-forge-ai-scrapers/)

生成摘要时出错

---

## 33. Japan law opening phone app stores to go into effect

**原文标题**: Japan law opening phone app stores to go into effect

**原文链接**: [https://www3.nhk.or.jp/nhkworld/en/news/20251210_B1/](https://www3.nhk.or.jp/nhkworld/en/news/20251210_B1/)

生成摘要时出错

---

## 34. YouTube's CEO limits his kids' social media use – other tech bosses do the same

**原文标题**: YouTube's CEO limits his kids' social media use – other tech bosses do the same

**原文链接**: [https://www.cnbc.com/2025/12/13/youtubes-ceo-is-latest-tech-boss-limiting-his-kids-social-media-use.html](https://www.cnbc.com/2025/12/13/youtubes-ceo-is-latest-tech-boss-limiting-his-kids-social-media-use.html)

生成摘要时出错

---

## 35. Berlin Approves New Expansion of Police Surveillance Powers

**原文标题**: Berlin Approves New Expansion of Police Surveillance Powers

**原文链接**: [https://reclaimthenet.org/berlin-approves-new-expansion-of-police-surveillance-powers](https://reclaimthenet.org/berlin-approves-new-expansion-of-police-surveillance-powers)

生成摘要时出错

---

## 36. LG TV's new software update installed MS Copilot, which cannot be deleted

**原文标题**: LG TV's new software update installed MS Copilot, which cannot be deleted

**原文链接**: [https://old.reddit.com/r/mildlyinfuriating/comments/1plldqo/my_lg_tvs_new_software_update_installed_microsoft/](https://old.reddit.com/r/mildlyinfuriating/comments/1plldqo/my_lg_tvs_new_software_update_installed_microsoft/)

生成摘要时出错

---

## 37. Pop_OS 24.04 LTS with COSMIC desktop environment

**原文标题**: Pop_OS 24.04 LTS with COSMIC desktop environment

**原文链接**: [https://blog.system76.com/post/pop-os-letter-from-our-founder/](https://blog.system76.com/post/pop-os-letter-from-our-founder/)

生成摘要时出错

---

## 38. Young journalists expose Russian-linked vessels off the Dutch and German coast

**原文标题**: Young journalists expose Russian-linked vessels off the Dutch and German coast

**原文链接**: [https://www.digitaldigging.org/p/they-droned-back](https://www.digitaldigging.org/p/they-droned-back)

生成摘要时出错

---

## 39. The true story of the Windows 3.1 'Hot Dog Stand' color scheme

**原文标题**: The true story of the Windows 3.1 'Hot Dog Stand' color scheme

**原文链接**: [https://www.pcgamer.com/software/windows/windows-3-1-included-a-red-and-yellow-hot-dog-stand-color-scheme-so-garish-it-was-long-assumed-to-be-a-joke-so-i-tracked-down-the-original-designer-to-get-the-true-story/](https://www.pcgamer.com/software/windows/windows-3-1-included-a-red-and-yellow-hot-dog-stand-color-scheme-so-garish-it-was-long-assumed-to-be-a-joke-so-i-tracked-down-the-original-designer-to-get-the-true-story/)

生成摘要时出错

---

## 40. Freeing a Xiaomi humidifier from the cloud

**原文标题**: Freeing a Xiaomi humidifier from the cloud

**原文链接**: [https://0l.de/blog/2025/11/xiaomi-humidifier/](https://0l.de/blog/2025/11/xiaomi-humidifier/)

生成摘要时出错

---

## 41. Oracle made a $300B bet on OpenAI. It's paying the price

**原文标题**: Oracle made a $300B bet on OpenAI. It's paying the price

**原文链接**: [https://finance.yahoo.com/news/oracle-made-a-300-billion-bet-on-openai-its-paying-the-price-205441863.html](https://finance.yahoo.com/news/oracle-made-a-300-billion-bet-on-openai-its-paying-the-price-205441863.html)

生成摘要时出错

---

## 42. Nuclear energy key to decarbonising Europe, says EESC

**原文标题**: Nuclear energy key to decarbonising Europe, says EESC

**原文链接**: [https://www.eesc.europa.eu/en/news-media/news/nuclear-energy-key-decarbonising-europe-says-eesc](https://www.eesc.europa.eu/en/news-media/news/nuclear-energy-key-decarbonising-europe-says-eesc)

生成摘要时出错

---

## 43. Using secondary school maths to demystify AI

**原文标题**: Using secondary school maths to demystify AI

**原文链接**: [https://www.raspberrypi.org/blog/secondary-school-maths-showing-that-ai-systems-dont-think/](https://www.raspberrypi.org/blog/secondary-school-maths-showing-that-ai-systems-dont-think/)

生成摘要时出错

---

## 44. We built another object storage

**原文标题**: We built another object storage

**原文链接**: [https://fractalbits.com/blog/why-we-built-another-object-storage/](https://fractalbits.com/blog/why-we-built-another-object-storage/)

生成摘要时出错

---

## 45. Doxers posing as cops are tricking big tech firms into sharing people's data

**原文标题**: Doxers posing as cops are tricking big tech firms into sharing people's data

**原文链接**: [https://www.wired.com/story/doxers-posing-as-cops-are-tricking-big-tech-firms-into-sharing-peoples-private-data/](https://www.wired.com/story/doxers-posing-as-cops-are-tricking-big-tech-firms-into-sharing-peoples-private-data/)

生成摘要时出错

---

## 46. Async DNS

**原文标题**: Async DNS

**原文链接**: [https://flak.tedunangst.com/post/async-dns](https://flak.tedunangst.com/post/async-dns)

生成摘要时出错

---

## 47. 50 years of proof assistants

**原文标题**: 50 years of proof assistants

**原文链接**: [https://lawrencecpaulson.github.io//2025/12/05/History_of_Proof_Assistants.html](https://lawrencecpaulson.github.io//2025/12/05/History_of_Proof_Assistants.html)

生成摘要时出错

---

## 48. Fedora: Open-source repository for long-term digital preservation

**原文标题**: Fedora: Open-source repository for long-term digital preservation

**原文链接**: [https://fedorarepository.org/](https://fedorarepository.org/)

生成摘要时出错

---

## 49. Stoolap: High-performance embedded SQL database in pure Rust

**原文标题**: Stoolap: High-performance embedded SQL database in pure Rust

**原文链接**: [https://github.com/stoolap/stoolap](https://github.com/stoolap/stoolap)

生成摘要时出错

---

## 50. I tried Gleam for Advent of Code

**原文标题**: I tried Gleam for Advent of Code

**原文链接**: [https://blog.tymscar.com/posts/gleamaoc2025/](https://blog.tymscar.com/posts/gleamaoc2025/)

生成摘要时出错

---

## 51. We built a resource hub to fight back against age verification

**原文标题**: We built a resource hub to fight back against age verification

**原文链接**: [https://www.eff.org/deeplinks/2025/12/age-verification-coming-internet-we-built-you-resource-hub-fight-back](https://www.eff.org/deeplinks/2025/12/age-verification-coming-internet-we-built-you-resource-hub-fight-back)

生成摘要时出错

---

## 52. Security issues with electronic invoices

**原文标题**: Security issues with electronic invoices

**原文链接**: [https://invoice.secvuln.info/](https://invoice.secvuln.info/)

生成摘要时出错

---

## 53. Smartphone without a battery (2022)

**原文标题**: Smartphone without a battery (2022)

**原文链接**: [https://yaky.dev/2022-09-06-smartphone-without-battery/](https://yaky.dev/2022-09-06-smartphone-without-battery/)

生成摘要时出错

---

## 54. Senator endorses discredited book that claims chemical treats autism, cancer

**原文标题**: Senator endorses discredited book that claims chemical treats autism, cancer

**原文链接**: [https://www.propublica.org/article/ron-johnson-wisconsin-chlorine-dioxide-pierre-kory-endorsement](https://www.propublica.org/article/ron-johnson-wisconsin-chlorine-dioxide-pierre-kory-endorsement)

生成摘要时出错

---

## 55. Why isn't online age verification just like showing your ID in person?

**原文标题**: Why isn't online age verification just like showing your ID in person?

**原文链接**: [https://www.eff.org/deeplinks/2025/12/why-isnt-online-age-verification-just-showing-your-id-person](https://www.eff.org/deeplinks/2025/12/why-isnt-online-age-verification-just-showing-your-id-person)

生成摘要时出错

---

## 56. Laying out the 404 Media zine

**原文标题**: Laying out the 404 Media zine

**原文链接**: [https://tedium.co/2025/12/10/404-media-zine-linux-affinity/?](https://tedium.co/2025/12/10/404-media-zine-linux-affinity/?)

生成摘要时出错

---

## 57. Tesla US sales drop to nearly 4-year low in November

**原文标题**: Tesla US sales drop to nearly 4-year low in November

**原文链接**: [https://www.reuters.com/business/autos-transportation/tesla-us-sales-drop-nearly-3-year-low-november-despite-launch-cheaper-versions-2025-12-11/](https://www.reuters.com/business/autos-transportation/tesla-us-sales-drop-nearly-3-year-low-november-despite-launch-cheaper-versions-2025-12-11/)

生成摘要时出错

---

## 58. New Kindle feature uses AI to answer questions about books

**原文标题**: New Kindle feature uses AI to answer questions about books

**原文链接**: [https://reactormag.com/new-kindle-feature-ai-answer-questions-books-authors/](https://reactormag.com/new-kindle-feature-ai-answer-questions-books-authors/)

生成摘要时出错

---

## 59. Capsudo: Rethinking sudo with object capabilities

**原文标题**: Capsudo: Rethinking sudo with object capabilities

**原文链接**: [https://ariadne.space/2025/12/12/rethinking-sudo-with-object-capabilities.html](https://ariadne.space/2025/12/12/rethinking-sudo-with-object-capabilities.html)

生成摘要时出错

---

## 60. The Checkerboard

**原文标题**: The Checkerboard

**原文链接**: [https://99percentinvisible.org/episode/650-the-checkerboard/](https://99percentinvisible.org/episode/650-the-checkerboard/)

生成摘要时出错

---

## 61. Oliver sacks put himself into his case studies. What was the cost?

**原文标题**: Oliver sacks put himself into his case studies. What was the cost?

**原文链接**: [https://www.newyorker.com/magazine/2025/12/15/oliver-sacks-put-himself-into-his-case-studies-what-was-the-cost](https://www.newyorker.com/magazine/2025/12/15/oliver-sacks-put-himself-into-his-case-studies-what-was-the-cost)

生成摘要时出错

---

## 62. America's betting craze has spread to its news networks

**原文标题**: America's betting craze has spread to its news networks

**原文链接**: [https://www.newyorker.com/news/the-lede/americas-betting-craze-has-spread-to-its-news-networks](https://www.newyorker.com/news/the-lede/americas-betting-craze-has-spread-to-its-news-networks)

生成摘要时出错

---

## 63. A Lisp Interpreter Implemented in Conway's Game of Life (2021)

**原文标题**: A Lisp Interpreter Implemented in Conway's Game of Life (2021)

**原文链接**: [https://woodrush.github.io/blog/posts/2022-01-12-lisp-in-life.html](https://woodrush.github.io/blog/posts/2022-01-12-lisp-in-life.html)

生成摘要时出错

---

## 64. Cadmium Zinc Telluride: The wonder material powering a medical 'revolution'

**原文标题**: Cadmium Zinc Telluride: The wonder material powering a medical 'revolution'

**原文链接**: [https://www.bbc.com/news/articles/c24l223d9n7o](https://www.bbc.com/news/articles/c24l223d9n7o)

生成摘要时出错

---

## 65. Poor Johnny still won't encrypt

**原文标题**: Poor Johnny still won't encrypt

**原文链接**: [https://bfswa.substack.com/p/poor-johnny-still-wont-encrypt](https://bfswa.substack.com/p/poor-johnny-still-wont-encrypt)

生成摘要时出错

---

## 66. Training LLMs for honesty via confessions

**原文标题**: Training LLMs for honesty via confessions

**原文链接**: [https://arxiv.org/abs/2512.08093](https://arxiv.org/abs/2512.08093)

生成摘要时出错

---

## 67. Building small Docker images faster

**原文标题**: Building small Docker images faster

**原文链接**: [https://sgt.hootr.club/blog/docker-protips/](https://sgt.hootr.club/blog/docker-protips/)

生成摘要时出错

---

## 68. Germany's train service is one of Europe's worst. How did it get so bad?

**原文标题**: Germany's train service is one of Europe's worst. How did it get so bad?

**原文链接**: [https://www.npr.org/2025/12/12/g-s1-100794/germany-train-rail-deutsche-bahn](https://www.npr.org/2025/12/12/g-s1-100794/germany-train-rail-deutsche-bahn)

生成摘要时出错

---

## 69. Wine 11.0 RC2 – Run Windows Applications on Linux, BSD, Solaris and macOS

**原文标题**: Wine 11.0 RC2 – Run Windows Applications on Linux, BSD, Solaris and macOS

**原文链接**: [https://gitlab.winehq.org/wine/wine/-/releases/wine-11.0-rc2](https://gitlab.winehq.org/wine/wine/-/releases/wine-11.0-rc2)

生成摘要时出错

---

## 70. BpfJailer: eBPF Mandatory Access Control [pdf]

**原文标题**: BpfJailer: eBPF Mandatory Access Control [pdf]

**原文链接**: [https://lpc.events/event/19/contributions/2159/attachments/1833/3929/BpfJailer%20LPC%202025.pdf](https://lpc.events/event/19/contributions/2159/attachments/1833/3929/BpfJailer%20LPC%202025.pdf)

生成摘要时出错

---

## 71. Powder and stone, or, why medieval rulers loved castles

**原文标题**: Powder and stone, or, why medieval rulers loved castles

**原文链接**: [https://1517.substack.com/p/powder-and-stone-or-why-medieval](https://1517.substack.com/p/powder-and-stone-or-why-medieval)

生成摘要时出错

---

## 72. Pope criticizes US bid to 'break apart' US-Europe alliance

**原文标题**: Pope criticizes US bid to 'break apart' US-Europe alliance

**原文链接**: [https://apnews.com/article/vatican-russia-ukraine-trump-pope-leo-60c898afe3241ff67552f417a06900b0](https://apnews.com/article/vatican-russia-ukraine-trump-pope-leo-60c898afe3241ff67552f417a06900b0)

生成摘要时出错

---

## 73. The Coming Need for Formal Specification

**原文标题**: The Coming Need for Formal Specification

**原文链接**: [https://benjamincongdon.me/blog/2025/12/12/The-Coming-Need-for-Formal-Specification/](https://benjamincongdon.me/blog/2025/12/12/The-Coming-Need-for-Formal-Specification/)

生成摘要时出错

---

## 74. Analysis finds anytime electricity from solar available as battery costs plummet

**原文标题**: Analysis finds anytime electricity from solar available as battery costs plummet

**原文链接**: [https://pv-magazine-usa.com/2025/12/12/analysis-finds-anytime-electricity-from-solar-available-as-battery-costs-plummet/](https://pv-magazine-usa.com/2025/12/12/analysis-finds-anytime-electricity-from-solar-available-as-battery-costs-plummet/)

生成摘要时出错

---

## 75. Last quarter I rolled out Microsoft Copilot to 4k employees

**原文标题**: Last quarter I rolled out Microsoft Copilot to 4k employees

**原文链接**: [https://twitter.com/gothburz/status/1999124665801880032](https://twitter.com/gothburz/status/1999124665801880032)

生成摘要时出错

---

## 76. US threatens new ICC sanctions unless court pledges not to prosecute Trump

**原文标题**: US threatens new ICC sanctions unless court pledges not to prosecute Trump

**原文链接**: [https://www.reuters.com/world/us/us-threatens-new-icc-sanctions-unless-court-pledges-not-prosecute-trump-2025-12-10/](https://www.reuters.com/world/us/us-threatens-new-icc-sanctions-unless-court-pledges-not-prosecute-trump-2025-12-10/)

生成摘要时出错

---

## 77. Think Tanker Altered Ukraine War Map Before Big Polymarket Payout

**原文标题**: Think Tanker Altered Ukraine War Map Before Big Polymarket Payout

**原文链接**: [https://responsiblestatecraft.org/isw-polymarket-ukraine-war-map/](https://responsiblestatecraft.org/isw-polymarket-ukraine-war-map/)

生成摘要时出错

---

## 78. Building an efficient hash table in Java

**原文标题**: Building an efficient hash table in Java

**原文链接**: [https://bluuewhale.github.io/posts/building-a-fast-and-memory-efficient-hash-table-in-java-by-borrowing-the-best-ideas/](https://bluuewhale.github.io/posts/building-a-fast-and-memory-efficient-hash-table-in-java-by-borrowing-the-best-ideas/)

生成摘要时出错

---

## 79. AI is bringing old nuclear plants out of retirement

**原文标题**: AI is bringing old nuclear plants out of retirement

**原文链接**: [https://www.wbur.org/hereandnow/2025/12/09/nuclear-power-ai](https://www.wbur.org/hereandnow/2025/12/09/nuclear-power-ai)

生成摘要时出错

---

## 80. Instacart reaches into your pocket and lops a third off your dollars

**原文标题**: Instacart reaches into your pocket and lops a third off your dollars

**原文链接**: [https://pluralistic.net/2025/12/11/nothing-personal/](https://pluralistic.net/2025/12/11/nothing-personal/)

生成摘要时出错

---

## 81. Super-Emitter of the Most Damaging Greenhouse Gas Found in Germany

**原文标题**: Super-Emitter of the Most Damaging Greenhouse Gas Found in Germany

**原文链接**: [https://industrydecarbonization.com/news/super-emitter-of-the-most-damaging-greenhouse-gas-found-in-germany.html](https://industrydecarbonization.com/news/super-emitter-of-the-most-damaging-greenhouse-gas-found-in-germany.html)

生成摘要时出错

---

## 82. Opinion: US Authorities Have Far-Reaching Access to European Cloud Data

**原文标题**: Opinion: US Authorities Have Far-Reaching Access to European Cloud Data

**原文链接**: [https://www.heise.de/en/news/Opinion-US-Authorities-Have-Far-Reaching-Access-to-European-Cloud-Data-11111060.html](https://www.heise.de/en/news/Opinion-US-Authorities-Have-Far-Reaching-Access-to-European-Cloud-Data-11111060.html)

生成摘要时出错

---

## 83. Show HN: Epstein's emails reconstructed in a message-style UI (OCR and LLMs)

**原文标题**: Show HN: Epstein's emails reconstructed in a message-style UI (OCR and LLMs)

**原文链接**: [https://github.com/Toon-nooT/epsteins-phone-reconstructed](https://github.com/Toon-nooT/epsteins-phone-reconstructed)

生成摘要时出错

---

## 84. Show HN: Gotui – a modern Go terminal dashboard library

**原文标题**: Show HN: Gotui – a modern Go terminal dashboard library

**原文链接**: [https://github.com/metaspartan/gotui](https://github.com/metaspartan/gotui)

生成摘要时出错

---

## 85. When did the job market get so rude?

**原文标题**: When did the job market get so rude?

**原文链接**: [https://www.theatlantic.com/culture/2025/12/job-ghosting-manners/685206/](https://www.theatlantic.com/culture/2025/12/job-ghosting-manners/685206/)

生成摘要时出错

---

## 86. Something Ominous Is Happening in the AI Economy

**原文标题**: Something Ominous Is Happening in the AI Economy

**原文链接**: [https://www.theatlantic.com/economy/2025/12/nvidia-ai-financing-deals/685197/](https://www.theatlantic.com/economy/2025/12/nvidia-ai-financing-deals/685197/)

生成摘要时出错

---

## 87. TerraUSD creator Do Kwon sentenced to 15 years over $40B crypto collapse

**原文标题**: TerraUSD creator Do Kwon sentenced to 15 years over $40B crypto collapse

**原文链接**: [https://www.reuters.com/legal/government/terrausd-creator-do-kwon-be-sentenced-over-40-billion-crypto-collapse-2025-12-11/](https://www.reuters.com/legal/government/terrausd-creator-do-kwon-be-sentenced-over-40-billion-crypto-collapse-2025-12-11/)

生成摘要时出错

---

## 88. Amazon pulls AI-powered Fallout recap after getting key story details wrong

**原文标题**: Amazon pulls AI-powered Fallout recap after getting key story details wrong

**原文链接**: [https://www.ign.com/articles/everyone-disliked-that-amazon-pulls-ai-powered-fallout-recap-after-getting-key-story-details-wrong](https://www.ign.com/articles/everyone-disliked-that-amazon-pulls-ai-powered-fallout-recap-after-getting-key-story-details-wrong)

生成摘要时出错

---

## 89. US TikTok investors in limbo as deal set to be delayed again

**原文标题**: US TikTok investors in limbo as deal set to be delayed again

**原文链接**: [https://www.bbc.com/news/articles/cp34442z25ko](https://www.bbc.com/news/articles/cp34442z25ko)

生成摘要时出错

---

## 90. The choice between Rust and C-derived languages is not only about memory safety

**原文标题**: The choice between Rust and C-derived languages is not only about memory safety

**原文链接**: [https://bbuyukliev.blogspot.com/2025/12/the-choice-between-rust-and-c-derived.html](https://bbuyukliev.blogspot.com/2025/12/the-choice-between-rust-and-c-derived.html)

生成摘要时出错

---

## 91. The Average Founder Ages 6 Months Each Year

**原文标题**: The Average Founder Ages 6 Months Each Year

**原文链接**: [https://tomtunguz.com/founder-age-median-trend/](https://tomtunguz.com/founder-age-median-trend/)

生成摘要时出错

---

## 92. The Boot Order of the Raspberry Pi Is Unusual

**原文标题**: The Boot Order of the Raspberry Pi Is Unusual

**原文链接**: [https://patrickmccanna.net/the-raspberry-pi-boot-order-is-unusual/](https://patrickmccanna.net/the-raspberry-pi-boot-order-is-unusual/)

生成摘要时出错

---

## 93. Bad Opsec Considered Harmful

**原文标题**: Bad Opsec Considered Harmful

**原文链接**: [https://buttondown.com/grugq/archive/bad-opsec-considered-harmful/](https://buttondown.com/grugq/archive/bad-opsec-considered-harmful/)

生成摘要时出错

---

## 94. Cut off by their banks and from Alexa, sanctioned ICC staffers remain resolute

**原文标题**: Cut off by their banks and from Alexa, sanctioned ICC staffers remain resolute

**原文链接**: [https://apnews.com/article/international-court-sanctions-trump-icc-hague-4cdefe4de067432f6cdb9b137908c463](https://apnews.com/article/international-court-sanctions-trump-icc-hague-4cdefe4de067432f6cdb9b137908c463)

生成摘要时出错

---

## 95. Deno 2.6

**原文标题**: Deno 2.6

**原文链接**: [https://deno.com/blog/v2.6](https://deno.com/blog/v2.6)

生成摘要时出错

---

## 96. Show HN: tomcp.org – Turn any URL into an MCP server

**原文标题**: Show HN: tomcp.org – Turn any URL into an MCP server

**原文链接**: [https://github.com/Ami3466/tomcp](https://github.com/Ami3466/tomcp)

生成摘要时出错

---

## 97. Congress Kills Military "Right to Repair"

**原文标题**: Congress Kills Military "Right to Repair"

**原文链接**: [https://theintercept.com/2025/12/09/congress-military-ndaa-right-to-repair/](https://theintercept.com/2025/12/09/congress-military-ndaa-right-to-repair/)

生成摘要时出错

---

## 98. 'Mamdani Effect' Is Seeing More People Moving to New York, Not Leaving It

**原文标题**: 'Mamdani Effect' Is Seeing More People Moving to New York, Not Leaving It

**原文链接**: [https://www.newsweek.com/mamdani-effect-more-people-moving-new-york-city-not-leaving-11193747](https://www.newsweek.com/mamdani-effect-more-people-moving-new-york-city-not-leaving-11193747)

生成摘要时出错

---

## 99. Nintendo Switch 2 RAM prices rise 41%, NAND flash up 8% – shares nosedive

**原文标题**: Nintendo Switch 2 RAM prices rise 41%, NAND flash up 8% – shares nosedive

**原文链接**: [https://www.tomshardware.com/video-games/nintendo/nintendo-switch-2-ram-prices-rise-41-percent-nand-flash-up-8-percent-console-giant-shares-nosedive-in-face-of-increased-cost-warnings](https://www.tomshardware.com/video-games/nintendo/nintendo-switch-2-ram-prices-rise-41-percent-nand-flash-up-8-percent-console-giant-shares-nosedive-in-face-of-increased-cost-warnings)

生成摘要时出错

---

## 100. Two new RSC protocol vulnerabilities uncovered

**原文标题**: Two new RSC protocol vulnerabilities uncovered

**原文链接**: [https://nextjs.org/blog/security-update-2025-12-11](https://nextjs.org/blog/security-update-2025-12-11)

生成摘要时出错

---

