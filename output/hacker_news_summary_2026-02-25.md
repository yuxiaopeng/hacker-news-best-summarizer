# Hacker News 热门文章摘要 (2026-02-25)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 以色列国防军在2025年大屠杀中近距离射杀加沙援助人员：报告

**原文标题**: IDF killed Gaza aid workers at point blank range in 2025 massacre: Report

**原文链接**: [https://www.dropsitenews.com/p/israeli-soldiers-tel-sultan-gaza-red-crescent-civil-defense-massacre-report-forensic-architecture-earshot](https://www.dropsitenews.com/p/israeli-soldiers-tel-sultan-gaza-red-crescent-civil-defense-massacre-report-forensic-architecture-earshot)

Earshot和Forensic Architecture的一项联合调查报告称，2025年3月23日，在加沙南部的Tel al-Sultan，以色列士兵“近距离射击”杀害了15名巴勒斯坦援助人员。该报告基于目击者证词、音视频分析和卫星图像，重建了一场“大屠杀”：士兵们向清晰标记的应急车辆和工作人员发射了900多发子弹，其中至少八发子弹的射击距离近至一米。

这起事件造成巴勒斯坦红新月会（PRCS）的八名工作人员、巴勒斯坦民防部门的六名工作人员以及一名联合国救援机构工作人员死亡。报告详细描述了士兵如何伏击援助车队，从高处持续射击了两个多小时，随后推进并处决了工作人员。音频分析证实至少有五名枪手同时开火。两名幸存者证实现场有12至30名士兵。

以色列军方最初几次改变其说法，最终进行了一项内部调查，称没有证据支持处决指控，并建议不采取任何刑事行动，称这些指控为“血腥诽谤”。袭击发生后，据报道以色列军队压碎并试图掩埋车辆，并进行了大规模的土方工程，随后在该地区修建了“莫拉格走廊”安全区。几天后，穿着制服的援助人员的尸体在一个乱葬坑中被发现。

---

## 2. 我在帮我家狗凭感觉编游戏。

**原文标题**: I'm helping my dog vibe code games

**原文链接**: [https://www.calebleak.com/posts/dog-game/](https://www.calebleak.com/posts/dog-game/)

作者开发了一套独特的系统，让他9磅重的卡瓦犬Momo能够使用Claude Code AI“氛围编程”视频游戏。这个项目是作者在被裁员后启动的，灵感来源于Momo之前意外打字到他键盘上的一次事件。

该设置包括Momo在蓝牙键盘上打字，键击通过树莓派5路由到一个名为DogKeyboard的Rust应用程序。这个应用程序会过滤特殊按键，并将输入转发给Claude Code。当Momo输入足够字符时，智能宠物喂食器会分发零食，一声提示音则表示Claude已准备好接收更多输入。游戏使用Godot 4.6和C#开发。

一个关键方面是提示工程：Claude Code被指示扮演一个“杰出的人工智能游戏开发者”，负责从一个“古怪的游戏设计师”那里，即使是从无意义的输入中，解读“神秘的谜语”。强大的护栏机制和最低游戏要求清单（例如，声音、玩家角色、控制）显著改善了结果。

为了扩展系统，强大的验证工具至关重要。作者让Claude能够启动游戏、截取屏幕截图，并发送输入序列（例如“向左3秒，开火”），有效地将AI变成了它自己的质量保证测试员。这使得Claude能够识别并修复诸如用户界面损坏或控制无响应等问题。针对Godot场景和着色器的额外linter，加上一个输入动作映射器，进一步完善了这一过程。

Momo的训练大约持续了两周，最初是在键盘上放置高价值零食以建立关联，然后逐渐通过宠物喂食器自动奖励打字行为。该项目展示了惊人的良好结果，随着工具和Claude能力的演进，游戏质量也随之提高。一个关键发现是在新游戏开始前清除Claude持久化的`MEMORY.md`文件，以防止它强制执行特定的“标志性风格”。Momo创造了各种可玩的游戏，从节奏挑战到解谜游戏和放牧模拟。

---

## 3. 美国人破坏 Flock 监控摄像头

**原文标题**: Americans are destroying Flock surveillance cameras

**原文链接**: [https://techcrunch.com/2026/02/23/americans-are-destroying-flock-surveillance-cameras/](https://techcrunch.com/2026/02/23/americans-are-destroying-flock-surveillance-cameras/)

美国人正在全国范围内日益拆除和破坏Flock监控摄像头，原因是公众对这些车牌识别器协助美国移民局（ICE）进行驱逐出境感到愤怒，以及对隐私的担忧。Flock是一家总部位于亚特兰大的初创公司，生产这些通过拍摄车牌来跟踪车辆移动的摄像头。

尽管Flock声称不直接与ICE共享数据，但据报道，当地警察部门允许联邦当局访问他们的Flock摄像头和数据库。这种间接访问被视为助长了特朗普政府的移民打击行动。

布莱恩·默钱特报告了多起破坏事件，其中包括加利福尼亚州拉梅萨的摄像头被损坏，此事发生在该市议会不顾公众反对投票决定继续部署这些摄像头之后。类似的事件也发生在加利福尼亚州、康涅狄格州、伊利诺伊州和弗吉尼亚州等多个州。在俄勒冈州，六个摄像头被切断并喷漆，并留下了表达强烈反监控情绪的纸条。

根据DeFlock（一个绘制这些设备地图的项目）的数据，美国各地有近8万个摄像头。为了回应争议，数十个城市拒绝了Flock的摄像头，一些警察部门也阻止了联邦当局访问其资源。Flock发言人没有评论该公司是否追踪被毁摄像头的数量。这股破坏浪潮反映了人们对被视为侵犯隐私和有争议的政府政策工具的监控技术日益增长的抵制。

---

## 4. 丹麦政府机构将弃用微软软件 (2025年)

**原文标题**: Danish government agency to ditch Microsoft software (2025)

**原文链接**: [https://therecord.media/denmark-digital-agency-microsoft-digital-independence](https://therecord.media/denmark-digital-agency-microsoft-digital-independence)

丹麦数字化部将用开源替代品取代微软软件，目标是实现“数字独立”并减少对美国科技公司的依赖。数字化部长卡罗琳·斯塔奇·奥尔森证实，该部一半以上的员工将于下月从Microsoft Office转向LibreOffice，并将在年底前全面过渡到开源软件。

此举受多方面因素驱动，包括避免管理过时Windows 10系统的开销、成本考量、微软的市场主导地位以及美国与丹麦之间过去存在的政治紧张关系。LibreOffice由总部位于柏林的非营利组织The Document Foundation开发，提供免费的开源办公套件。斯塔奇指出，如果此次过渡过于复杂，该部可能会恢复使用微软产品。

这一决定反映了欧洲范围内走向数字主权的更广泛趋势。丹麦最大的两个城市哥本哈根和奥胡斯此前也宣布了类似的计划。此外，德国石勒苏益格-荷尔斯泰因州正在放弃Microsoft Office工具，转用LibreOffice和Open-Xchange，并计划迁移到Linux操作系统，这凸显了整个欧洲大陆对独立、安全和可持续IT工作场所日益增长的推动。

---

## 5. 亚马逊被控在全经济范围大范围哄抬物价。

**原文标题**: Amazon accused of widespread scheme to inflate prices across the economy

**原文链接**: [https://www.thebignewsletter.com/p/amazon-busted-for-widespread-price](https://www.thebignewsletter.com/p/amazon-busted-for-widespread-price)

联邦贸易委员会（FTC）和17个州的检察长已对亚马逊提起一项里程碑式的反垄断诉讼，指控这家电子商务巨头运营一项非法且广泛的计划，以在整个经济中抬高物价并抑制竞争。

该诉讼指控亚马逊使用了两种主要的******竞争策略。首先，它实施了反折扣政策，常被称为“公平定价”政策，如果第三方卖家在竞争对手的在线平台上以更低的价格销售商品，就会对其进行惩罚。通过算法强制执行以及威胁将其从亚马逊关键的“购买按钮”中移除，卖家被迫在其他网站上保持更高的价格，否则就有可能被有效排除在亚马逊市场之外。据称，这种做法消除了价格竞争，迫使消费者在整个互联网上支付更多费用。

其次，该诉讼针对亚马逊的“亚马逊物流”（FBA）服务。FTC声称，亚马逊对这项类似强制性物流服务收取过高费用，有效地迫使卖家使用它，进一步抬高了他们的成本，这些成本最终转嫁给了消费者。诉讼认为，这些做法使亚马逊能够人为地抬高价格，扼杀创新，损害竞争对手的零售商，最终通过使产品比在竞争市场中更昂贵来损害消费者。该诉讼旨在结束亚马逊被指控的******竞争行为并恢复竞争。

---

## 6. OpenAI、美国政府和佩尔索纳打造了一个身份监控系统。

**原文标题**: OpenAI, the US government and Persona built an identity surveillance machine

**原文链接**: [https://vmfunc.re/blog/persona/](https://vmfunc.re/blog/persona/)

一份调查报告声称，OpenAI、美国政府和身份验证服务Persona已合作构建了一台“身份监控机器”。研究人员通过对公共资源的被动侦察发现了这一点，识别出一个自2023年11月起活跃的专用Google Cloud实例（`openai-watchlistdb.withpersona.com`）。这比OpenAI公开宣布其身份验证服务早了18个月。

据报道，这个独立于Persona通用网络的隔离基础设施被用于“观察名单”筛选。在一个政府端点上发现的未经认证的源映射暴露了代码，揭示了人脸识别功能、针对14类“负面媒体”（包括恐怖主义和间谍活动）的筛选，以及向FinCEN提交可疑活动报告（SARs）。Persona的公共API文档证实了其收集广泛的用户数据，包括法定姓名、出生详情、国籍、地址、政府文件信息以及生物识别数据（身份证照片、自拍和视频）。

进一步调查发现了`withpersona-gov.com`，这是一个位于Google Cloud数据中心、专门针对政府的并行部署，并于2025年10月获得了FedRAMP授权状态。其Content-Security-Policy标头显示其连接到OpenAI的API，并与第三方服务集成，用于浏览器指纹识别、文档扫描、错误跟踪、用户分析、实时用户监控和财务数据。一个新子域名`onyx.withpersona-gov.com`于2026年2月出现，作者将其与ICE（美国移民和海关执法局）的AI监控项目联系起来。作者强调，所有发现均来自公共可访问数据，构成受保护的新闻报道和安全研究。

---

## 7. Mac mini 将在休斯顿的一处新设施生产。

**原文标题**: Mac mini will be made at a new facility in Houston

**原文链接**: [https://www.apple.com/newsroom/2026/02/apple-accelerates-us-manufacturing-with-mac-mini-production/](https://www.apple.com/newsroom/2026/02/apple-accelerates-us-manufacturing-with-mac-mini-production/)

Apple announced a significant expansion of its U.S. manufacturing operations, bringing Mac mini production to a new facility in Houston, Texas, for the first time, starting later this year (2026). The Houston site will also expand its advanced AI server manufacturing, which began in 2025 and is currently ahead of schedule, supplying Apple's U.S. data centers.

Complementing these production efforts, Apple will open a 20,000-square-foot Advanced Manufacturing Center in Houston later this year. This center will provide hands-on training in advanced manufacturing techniques to students, supplier employees, and American businesses, fostering skills development and creating thousands of jobs.

CEO Tim Cook emphasized Apple's deep commitment to American manufacturing. This Houston expansion is part of Apple's broader $600 billion U.S. manufacturing program, which has achieved several milestones. These include sourcing over 20 billion U.S.-made chips, GlobalWafers starting bare silicon wafer production in Sherman, Texas, and Amkor breaking ground on a $7 billion semiconductor facility in Arizona with Apple as its first customer. Furthermore, Corning's Kentucky facility is now 100% dedicated to iPhone and Apple Watch cover glass, and Apple plans to significantly increase chip purchases from TSMC's Arizona facility in 2026. The company also launched the Apple Manufacturing Academy in Detroit to support American manufacturers with training in AI and automation.

---

## 8. Anthropic Drops Flagship Safety Pledge

**原文标题**: Anthropic Drops Flagship Safety Pledge

**原文链接**: [https://time.com/7380854/exclusive-anthropic-drops-flagship-safety-pledge/](https://time.com/7380854/exclusive-anthropic-drops-flagship-safety-pledge/)

生成摘要时出错

---

## 9. Never buy a .online domain

**原文标题**: Never buy a .online domain

**原文链接**: [https://www.0xsid.com/blog/online-tld-is-pain](https://www.0xsid.com/blog/online-tld-is-pain)

生成摘要时出错

---

## 10. Pi – A minimal terminal coding harness

**原文标题**: Pi – A minimal terminal coding harness

**原文链接**: [https://pi.dev](https://pi.dev)

生成摘要时出错

---

## 11. Binance fired employees who found $1.7B in crypto was sent to Iran

**原文标题**: Binance fired employees who found $1.7B in crypto was sent to Iran

**原文链接**: [https://www.nytimes.com/2026/02/23/technology/binance-employees-iran-firings.html](https://www.nytimes.com/2026/02/23/technology/binance-employees-iran-firings.html)

生成摘要时出错

---

## 12. I pitched a roller coaster to Disneyland at age 10 in 1978

**原文标题**: I pitched a roller coaster to Disneyland at age 10 in 1978

**原文链接**: [https://wordglyph.xyz/one-piece-at-a-time](https://wordglyph.xyz/one-piece-at-a-time)

In 1978, 10-year-old Kevin Glikmann, inspired by Disneyland's Space Mountain, conceived "The Quadrupuler," a roller coaster with four loops, after realizing upside-down coasters weren't common. Despite a friend informing him of an upcoming single-loop coaster, Kevin was determined to build his more ambitious version.

He meticulously drew blueprints, then painstakingly constructed a model from balsa wood. Facing the challenge of creating the loops, he ingeniously (and cautiously, due to a past fire incident) heated and bent plastic strips over a stovetop. Once complete, he sent Polaroids of his model and a letter to Disneyland.

Weeks later, he received a letter from WED Enterprises (Walt Disney Imagineering), signed by Tom Fitzgerald. Though the letter mentioned their own upcoming Big Thunder Mountain Railroad, it positively acknowledged Kevin's "quite an adventure" design. Far from being crushed, Kevin was elated; the validation from Disney launched his self-esteem and gave him "bulletproof resilience."

This early experience profoundly impacted Kevin. He continued inventing, designing board games and even a Rubik's Cube modification, undeterred by rejections. Today, he works in acting, a field rich in rejection, finding both inventing and acting feed his spirit of discovery. The 10-year-old's motto, "one piece at a time," and the resilience gained from that Disney letter, continue to guide him through life's challenges.

---

## 13. How we rebuilt Next.js with AI in one week

**原文标题**: How we rebuilt Next.js with AI in one week

**原文链接**: [https://blog.cloudflare.com/vinext/](https://blog.cloudflare.com/vinext/)

生成摘要时出错

---

## 14. Firefox 148 Launches with AI Kill Switch Feature and More Enhancements

**原文标题**: Firefox 148 Launches with AI Kill Switch Feature and More Enhancements

**原文链接**: [https://serverhost.com/blog/firefox-148-launches-with-exciting-ai-kill-switch-feature-and-more-enhancements/](https://serverhost.com/blog/firefox-148-launches-with-exciting-ai-kill-switch-feature-and-more-enhancements/)

生成摘要时出错

---

## 15. Discord cuts ties with identity verification software, Persona

**原文标题**: Discord cuts ties with identity verification software, Persona

**原文链接**: [https://fortune.com/2026/02/24/discord-peter-thiel-backed-persona-identity-verification-breach/](https://fortune.com/2026/02/24/discord-peter-thiel-backed-persona-identity-verification-breach/)

生成摘要时出错

---

## 16. Open Letter to Google on Mandatory Developer Registration for App Distribution

**原文标题**: Open Letter to Google on Mandatory Developer Registration for App Distribution

**原文链接**: [https://keepandroidopen.org/open-letter/](https://keepandroidopen.org/open-letter/)

生成摘要时出错

---

## 17. 血液检测将阿尔茨海默症诊断准确率提升至94.5%，临床研究表明。

**原文标题**: Blood test boosts Alzheimer's diagnosis accuracy to 94.5%, clinical study shows

**原文链接**: [https://medicalxpress.com/news/2026-02-blood-boosts-alzheimer-diagnosis-accuracy.html](https://medicalxpress.com/news/2026-02-blood-boosts-alzheimer-diagnosis-accuracy.html)

生成摘要时出错

---

## 18. FreeBSD doesn't have Wi-Fi driver for my old MacBook, so AI built one for me

**原文标题**: FreeBSD doesn't have Wi-Fi driver for my old MacBook, so AI built one for me

**原文链接**: [https://vladimir.varank.in/notes/2026/02/freebsd-brcmfmac/](https://vladimir.varank.in/notes/2026/02/freebsd-brcmfmac/)

生成摘要时出错

---

## 19. New accounts on HN more likely to use em-dashes

**原文标题**: New accounts on HN more likely to use em-dashes

**原文链接**: [https://www.marginalia.nu/weird-ai-crap/hn/](https://www.marginalia.nu/weird-ai-crap/hn/)

生成摘要时出错

---

## 20. Nearby Glasses

**原文标题**: Nearby Glasses

**原文链接**: [https://github.com/yjeanrenaud/yj_nearbyglasses](https://github.com/yjeanrenaud/yj_nearbyglasses)

生成摘要时出错

---

## 21. Claude Code Remote Control

**原文标题**: Claude Code Remote Control

**原文链接**: [https://code.claude.com/docs/en/remote-control](https://code.claude.com/docs/en/remote-control)

生成摘要时出错

---

## 22. “Car Wash” test with 53 models

**原文标题**: “Car Wash” test with 53 models

**原文链接**: [https://opper.ai/blog/car-wash-test](https://opper.ai/blog/car-wash-test)

生成摘要时出错

---

## 23. Goodbye InnerHTML, Hello SetHTML: Stronger XSS Protection in Firefox 148

**原文标题**: Goodbye InnerHTML, Hello SetHTML: Stronger XSS Protection in Firefox 148

**原文链接**: [https://hacks.mozilla.org/2026/02/goodbye-innerhtml-hello-sethtml-stronger-xss-protection-in-firefox-148/](https://hacks.mozilla.org/2026/02/goodbye-innerhtml-hello-sethtml-stronger-xss-protection-in-firefox-148/)

生成摘要时出错

---

## 24. Mercury 2: Fast reasoning LLM powered by diffusion

**原文标题**: Mercury 2: Fast reasoning LLM powered by diffusion

**原文链接**: [https://www.inceptionlabs.ai/blog/introducing-mercury-2](https://www.inceptionlabs.ai/blog/introducing-mercury-2)

生成摘要时出错

---

## 25. Hacking an old Kindle to display bus arrival times

**原文标题**: Hacking an old Kindle to display bus arrival times

**原文链接**: [https://www.mariannefeng.com/portfolio/kindle/](https://www.mariannefeng.com/portfolio/kindle/)

生成摘要时出错

---

## 26. Show HN: Steerling-8B, a language model that can explain any token it generates

**原文标题**: Show HN: Steerling-8B, a language model that can explain any token it generates

**原文链接**: [https://www.guidelabs.ai/post/steerling-8b-base-model-release/](https://www.guidelabs.ai/post/steerling-8b-base-model-release/)

生成摘要时出错

---

## 27. US orders diplomats to fight data sovereignty initiatives

**原文标题**: US orders diplomats to fight data sovereignty initiatives

**原文链接**: [https://www.reuters.com/sustainability/boards-policy-regulation/us-orders-diplomats-fight-data-sovereignty-initiatives-2026-02-25/](https://www.reuters.com/sustainability/boards-policy-regulation/us-orders-diplomats-fight-data-sovereignty-initiatives-2026-02-25/)

生成摘要时出错

---

## 28. Show HN: Moonshine Open-Weights STT models – higher accuracy than WhisperLargev3

**原文标题**: Show HN: Moonshine Open-Weights STT models – higher accuracy than WhisperLargev3

**原文链接**: [https://github.com/moonshine-ai/moonshine](https://github.com/moonshine-ai/moonshine)

生成摘要时出错

---

## 29. Making Wolfram tech available as a foundation tool for LLM systems

**原文标题**: Making Wolfram tech available as a foundation tool for LLM systems

**原文链接**: [https://writings.stephenwolfram.com/2026/02/making-wolfram-tech-available-as-a-foundation-tool-for-llm-systems/](https://writings.stephenwolfram.com/2026/02/making-wolfram-tech-available-as-a-foundation-tool-for-llm-systems/)

生成摘要时出错

---

## 30. I Ported Coreboot to the ThinkPad X270

**原文标题**: I Ported Coreboot to the ThinkPad X270

**原文链接**: [https://dork.dev/posts/2026-02-20-ported-coreboot/](https://dork.dev/posts/2026-02-20-ported-coreboot/)

生成摘要时出错

---

## 31. AI Added 'Basically Zero' to US Economic Growth Last Year, Goldman Sachs Says

**原文标题**: AI Added 'Basically Zero' to US Economic Growth Last Year, Goldman Sachs Says

**原文链接**: [https://gizmodo.com/ai-added-basically-zero-to-us-economic-growth-last-year-goldman-sachs-says-2000725380](https://gizmodo.com/ai-added-basically-zero-to-us-economic-growth-last-year-goldman-sachs-says-2000725380)

生成摘要时出错

---

## 32. Show HN: X86CSS – An x86 CPU emulator written in CSS

**原文标题**: Show HN: X86CSS – An x86 CPU emulator written in CSS

**原文链接**: [https://lyra.horse/x86css/](https://lyra.horse/x86css/)

生成摘要时出错

---

## 33. Steel Bank Common Lisp

**原文标题**: Steel Bank Common Lisp

**原文链接**: [https://www.sbcl.org/](https://www.sbcl.org/)

生成摘要时出错

---

## 34. Flock cameras gifted by Horowitz Foundation, avoiding public oversight

**原文标题**: Flock cameras gifted by Horowitz Foundation, avoiding public oversight

**原文链接**: [https://thenevadaindependent.com/article/vegas-police-are-big-users-of-license-plate-readers-public-has-little-input-because-its-a-gift](https://thenevadaindependent.com/article/vegas-police-are-big-users-of-license-plate-readers-public-has-little-input-because-its-a-gift)

生成摘要时出错

---

## 35. You are not supposed to install OpenClaw on your personal computer

**原文标题**: You are not supposed to install OpenClaw on your personal computer

**原文链接**: [https://twitter.com/BenjaminBadejo/status/2025987544853188836](https://twitter.com/BenjaminBadejo/status/2025987544853188836)

生成摘要时出错

---

## 36. Stripe valued at $159B, 2025 annual letter

**原文标题**: Stripe valued at $159B, 2025 annual letter

**原文链接**: [https://stripe.com/newsroom/news/stripe-2025-update](https://stripe.com/newsroom/news/stripe-2025-update)

生成摘要时出错

---

## 37. Tesla registrations crash 17% in Europe as BEV market surges 14%

**原文标题**: Tesla registrations crash 17% in Europe as BEV market surges 14%

**原文链接**: [https://electrek.co/2026/02/24/tesla-eu-registrations-crash-january-2026-bev-growth/](https://electrek.co/2026/02/24/tesla-eu-registrations-crash-january-2026-bev-growth/)

生成摘要时出错

---

## 38. Osaka: Kansai Airport proud to have never lost single piece of luggage (2024)

**原文标题**: Osaka: Kansai Airport proud to have never lost single piece of luggage (2024)

**原文链接**: [https://japannews.yomiuri.co.jp/features/japan-focus/20241228-229891/](https://japannews.yomiuri.co.jp/features/japan-focus/20241228-229891/)

生成摘要时出错

---

## 39. IRS Tactics Against Meta Open a New Front in the Corporate Tax Fight

**原文标题**: IRS Tactics Against Meta Open a New Front in the Corporate Tax Fight

**原文链接**: [https://www.nytimes.com/2026/02/24/business/irs-meta-corporate-taxes.html](https://www.nytimes.com/2026/02/24/business/irs-meta-corporate-taxes.html)

生成摘要时出错

---

## 40. OpenAI resets spending expectations, from $1.4T to $600B

**原文标题**: OpenAI resets spending expectations, from $1.4T to $600B

**原文链接**: [https://www.cnbc.com/2026/02/20/openai-resets-spend-expectations-targets-around-600-billion-by-2030.html](https://www.cnbc.com/2026/02/20/openai-resets-spend-expectations-targets-around-600-billion-by-2030.html)

生成摘要时出错

---

## 41. Shatner is making an album with 35 metal icons

**原文标题**: Shatner is making an album with 35 metal icons

**原文链接**: [https://www.guitarworld.com/artists/guitarists/william-shatner-announces-all-star-metal-album](https://www.guitarworld.com/artists/guitarists/william-shatner-announces-all-star-metal-album)

生成摘要时出错

---

## 42. UNIX99, a UNIX-like OS for the TI-99/4A (2025)

**原文标题**: UNIX99, a UNIX-like OS for the TI-99/4A (2025)

**原文链接**: [https://forums.atariage.com/topic/380883-unix99-a-unix-like-os-for-the-ti-994a/page/5/#findComment-5713334](https://forums.atariage.com/topic/380883-unix99-a-unix-like-os-for-the-ti-994a/page/5/#findComment-5713334)

生成摘要时出错

---

## 43. Following 35% growth, solar has passed hydro on US grid

**原文标题**: Following 35% growth, solar has passed hydro on US grid

**原文链接**: [https://arstechnica.com/science/2026/02/final-2025-data-is-in-us-energy-use-is-up-as-solar-passes-hydro/](https://arstechnica.com/science/2026/02/final-2025-data-is-in-us-energy-use-is-up-as-solar-passes-hydro/)

生成摘要时出错

---

## 44. Show HN: enveil – hide your .env secrets from prAIng eyes

**原文标题**: Show HN: enveil – hide your .env secrets from prAIng eyes

**原文链接**: [https://github.com/GreatScott/enveil](https://github.com/GreatScott/enveil)

生成摘要时出错

---

## 45. Show HN: Emdash – Open-source agentic development environment

**原文标题**: Show HN: Emdash – Open-source agentic development environment

**原文链接**: [https://github.com/generalaction/emdash](https://github.com/generalaction/emdash)

生成摘要时出错

---

## 46. Bus stop balancing is fast, cheap, and effective

**原文标题**: Bus stop balancing is fast, cheap, and effective

**原文链接**: [https://worksinprogress.co/issue/the-united-states-needs-fewer-bus-stops/](https://worksinprogress.co/issue/the-united-states-needs-fewer-bus-stops/)

生成摘要时出错

---

## 47. LLM=True

**原文标题**: LLM=True

**原文链接**: [https://blog.codemine.be/posts/2026/20260222-be-quiet/](https://blog.codemine.be/posts/2026/20260222-be-quiet/)

生成摘要时出错

---

## 48. Hugging Face Skills

**原文标题**: Hugging Face Skills

**原文链接**: [https://github.com/huggingface/skills](https://github.com/huggingface/skills)

生成摘要时出错

---

## 49. US Military leaders meet with Anthropic to argue against Claude safeguards

**原文标题**: US Military leaders meet with Anthropic to argue against Claude safeguards

**原文链接**: [https://www.theguardian.com/us-news/2026/feb/24/anthropic-claude-military-ai](https://www.theguardian.com/us-news/2026/feb/24/anthropic-claude-military-ai)

生成摘要时出错

---

## 50. Looks like it is happening

**原文标题**: Looks like it is happening

**原文链接**: [https://www.math.columbia.edu/~woit/wordpress/?p=15500](https://www.math.columbia.edu/~woit/wordpress/?p=15500)

生成摘要时出错

---

## 51. Show HN: A real-time strategy game that AI agents can play

**原文标题**: Show HN: A real-time strategy game that AI agents can play

**原文链接**: [https://llmskirmish.com/](https://llmskirmish.com/)

生成摘要时出错

---

## 52. Iowa farmers are leading the fight for repair

**原文标题**: Iowa farmers are leading the fight for repair

**原文链接**: [https://www.ifixit.com/News/115722/iowa-farmers-are-leading-the-fight-for-repair](https://www.ifixit.com/News/115722/iowa-farmers-are-leading-the-fight-for-repair)

生成摘要时出错

---

## 53. Cell Service for the Fairly Paranoid

**原文标题**: Cell Service for the Fairly Paranoid

**原文链接**: [https://www.cape.co/](https://www.cape.co/)

生成摘要时出错

---

## 54. 100M-Row Challenge with PHP

**原文标题**: 100M-Row Challenge with PHP

**原文链接**: [https://github.com/tempestphp/100-million-row-challenge](https://github.com/tempestphp/100-million-row-challenge)

生成摘要时出错

---

## 55. Show HN: Babyshark – Wireshark made easy (terminal UI for PCAPs)

**原文标题**: Show HN: Babyshark – Wireshark made easy (terminal UI for PCAPs)

**原文链接**: [https://github.com/vignesh07/babyshark](https://github.com/vignesh07/babyshark)

生成摘要时出错

---

## 56. Pentagon threatens to make Anthropic a pariah

**原文标题**: Pentagon threatens to make Anthropic a pariah

**原文链接**: [https://www.cnn.com/2026/02/24/tech/hegseth-anthropic-ai-military-amodei](https://www.cnn.com/2026/02/24/tech/hegseth-anthropic-ai-military-amodei)

生成摘要时出错

---

## 57. Why the KeePass format should be based on SQLite

**原文标题**: Why the KeePass format should be based on SQLite

**原文链接**: [https://mketab.org/blog/sqlite_kdbx/](https://mketab.org/blog/sqlite_kdbx/)

生成摘要时出错

---

## 58. Stripe reportedly makes offer to acquire PayPal

**原文标题**: Stripe reportedly makes offer to acquire PayPal

**原文链接**: [https://www.cnbc.com/2026/02/24/paypal-stock-stripe-acquisition-report.html](https://www.cnbc.com/2026/02/24/paypal-stock-stripe-acquisition-report.html)

生成摘要时出错

---

## 59. Denver dumps Flock, awards contract to Axon

**原文标题**: Denver dumps Flock, awards contract to Axon

**原文链接**: [https://www.9news.com/article/news/local/denver-removing-flock-cameras-new-axon-contract/73-640b5af3-7c87-4fea-8aa1-2510ad3257b8](https://www.9news.com/article/news/local/denver-removing-flock-cameras-new-axon-contract/73-640b5af3-7c87-4fea-8aa1-2510ad3257b8)

生成摘要时出错

---

## 60. The Pentagon Threatens Anthropic

**原文标题**: The Pentagon Threatens Anthropic

**原文链接**: [https://www.astralcodexten.com/p/the-pentagon-threatens-anthropic](https://www.astralcodexten.com/p/the-pentagon-threatens-anthropic)

生成摘要时出错

---

## 61. Stop Killing Games update says EU petition advances

**原文标题**: Stop Killing Games update says EU petition advances

**原文链接**: [https://videocardz.com/newz/stop-killing-games-update-says-eu-petition-advances](https://videocardz.com/newz/stop-killing-games-update-says-eu-petition-advances)

生成摘要时出错

---

## 62. IBM Plunges After Anthropic's Latest Update Takes on COBOL

**原文标题**: IBM Plunges After Anthropic's Latest Update Takes on COBOL

**原文链接**: [https://www.zerohedge.com/markets/ibm-plunges-after-anthropics-latest-update-takes-cobol](https://www.zerohedge.com/markets/ibm-plunges-after-anthropics-latest-update-takes-cobol)

生成摘要时出错

---

## 63. Turing Completeness of GNU find

**原文标题**: Turing Completeness of GNU find

**原文链接**: [https://arxiv.org/abs/2602.20762](https://arxiv.org/abs/2602.20762)

生成摘要时出错

---

## 64. Cardiorespiratory fitness is associated with lower anger and anxiety

**原文标题**: Cardiorespiratory fitness is associated with lower anger and anxiety

**原文链接**: [https://linkinghub.elsevier.com/retrieve/pii/S000169182600171X](https://linkinghub.elsevier.com/retrieve/pii/S000169182600171X)

生成摘要时出错

---

## 65. Red Hat takes on Docker Desktop with its enterprise Podman Desktop build

**原文标题**: Red Hat takes on Docker Desktop with its enterprise Podman Desktop build

**原文链接**: [https://thenewstack.io/red-hat-enters-the-cloud-native-developer-desktop-market/](https://thenewstack.io/red-hat-enters-the-cloud-native-developer-desktop-market/)

生成摘要时出错

---

## 66. om

**原文标题**: om

**原文链接**: [https://www.om-language.com/](https://www.om-language.com/)

生成摘要时出错

---

## 67. Russian soldiers tell BBC they saw fellow troops executed on commanders' orders

**原文标题**: Russian soldiers tell BBC they saw fellow troops executed on commanders' orders

**原文链接**: [https://www.bbc.com/news/articles/cz7gw3l395ro](https://www.bbc.com/news/articles/cz7gw3l395ro)

生成摘要时出错

---

## 68. AIs can't stop recommending nuclear strikes in war game simulations

**原文标题**: AIs can't stop recommending nuclear strikes in war game simulations

**原文链接**: [https://www.newscientist.com/article/2516885-ais-cant-stop-recommending-nuclear-strikes-in-war-game-simulations/](https://www.newscientist.com/article/2516885-ais-cant-stop-recommending-nuclear-strikes-in-war-game-simulations/)

生成摘要时出错

---

## 69. Racket v9.1

**原文标题**: Racket v9.1

**原文链接**: [https://blog.racket-lang.org/2026/02/racket-v9-1.html](https://blog.racket-lang.org/2026/02/racket-v9-1.html)

生成摘要时出错

---

## 70. Hegseth gives Anthropic until Friday to back down on AI safeguards

**原文标题**: Hegseth gives Anthropic until Friday to back down on AI safeguards

**原文链接**: [https://www.axios.com/2026/02/24/anthropic-pentagon-claude-hegseth-dario](https://www.axios.com/2026/02/24/anthropic-pentagon-claude-hegseth-dario)

生成摘要时出错

---

## 71. Large-Scale Online Deanonymization with LLMs

**原文标题**: Large-Scale Online Deanonymization with LLMs

**原文链接**: [https://simonlermen.substack.com/p/large-scale-online-deanonymization](https://simonlermen.substack.com/p/large-scale-online-deanonymization)

生成摘要时出错

---

## 72. The challenges of porting Shufflepuck Cafe to the 8 bits Apple II

**原文标题**: The challenges of porting Shufflepuck Cafe to the 8 bits Apple II

**原文链接**: [https://www.colino.net/wordpress/archives/2026/02/23/the-challenges-of-porting-shufflepuck-cafe-to-the-8-bits-apple-ii/](https://www.colino.net/wordpress/archives/2026/02/23/the-challenges-of-porting-shufflepuck-cafe-to-the-8-bits-apple-ii/)

生成摘要时出错

---

## 73. We are changing our developer productivity experiment design

**原文标题**: We are changing our developer productivity experiment design

**原文链接**: [https://metr.org/blog/2026-02-24-uplift-update/](https://metr.org/blog/2026-02-24-uplift-update/)

生成摘要时出错

---

## 74. Show HN: Django Control Room – All Your Tools Inside the Django Admin

**原文标题**: Show HN: Django Control Room – All Your Tools Inside the Django Admin

**原文链接**: [https://github.com/yassi/dj-control-room](https://github.com/yassi/dj-control-room)

生成摘要时出错

---

## 75. The Misuses of the University

**原文标题**: The Misuses of the University

**原文链接**: [https://www.publicbooks.org/the-misuses-of-the-university/](https://www.publicbooks.org/the-misuses-of-the-university/)

生成摘要时出错

---

## 76. Sam Altman Is Losing His Grip on Humanity

**原文标题**: Sam Altman Is Losing His Grip on Humanity

**原文链接**: [https://www.theatlantic.com/technology/2026/02/sam-altman-train-a-human/686120/](https://www.theatlantic.com/technology/2026/02/sam-altman-train-a-human/686120/)

生成摘要时出错

---

## 77. AI-generated replies are a scourge these days

**原文标题**: AI-generated replies are a scourge these days

**原文链接**: [https://twitter.com/simonw/status/2025909963445707171](https://twitter.com/simonw/status/2025909963445707171)

生成摘要时出错

---

## 78. Sandboxes won't save you from OpenClaw

**原文标题**: Sandboxes won't save you from OpenClaw

**原文链接**: [https://tachyon.so/blog/sandboxes-wont-save-you](https://tachyon.so/blog/sandboxes-wont-save-you)

生成摘要时出错

---

## 79. Show HN: Context Mode – 315 KB of MCP output becomes 5.4 KB in Claude Code

**原文标题**: Show HN: Context Mode – 315 KB of MCP output becomes 5.4 KB in Claude Code

**原文链接**: [https://github.com/mksglu/claude-context-mode](https://github.com/mksglu/claude-context-mode)

生成摘要时出错

---

## 80. A lithium-ion breakthrough that could boost range and lower costs

**原文标题**: A lithium-ion breakthrough that could boost range and lower costs

**原文链接**: [https://www.techradar.com/vehicle-tech/hybrid-electric-vehicles/forget-solid-state-batteries-researchers-have-made-a-lithium-ion-breakthrough-that-could-boost-range-and-drastically-lower-costs](https://www.techradar.com/vehicle-tech/hybrid-electric-vehicles/forget-solid-state-batteries-researchers-have-made-a-lithium-ion-breakthrough-that-could-boost-range-and-drastically-lower-costs)

生成摘要时出错

---

## 81. Bcachefs creator insists his custom LLM is female and 'fully conscious'

**原文标题**: Bcachefs creator insists his custom LLM is female and 'fully conscious'

**原文链接**: [https://www.theregister.com/2026/02/25/bcachefs_creator_ai/](https://www.theregister.com/2026/02/25/bcachefs_creator_ai/)

生成摘要时出错

---

## 82. Tuna: A new, modern, modal launcher for macOS

**原文标题**: Tuna: A new, modern, modal launcher for macOS

**原文链接**: [https://tunaformac.com](https://tunaformac.com)

生成摘要时出错

---

## 83. What Happened to Fry's Electronics

**原文标题**: What Happened to Fry's Electronics

**原文链接**: [https://dfarq.homeip.net/what-happened-to-frys-electronics/](https://dfarq.homeip.net/what-happened-to-frys-electronics/)

生成摘要时出错

---

## 84. Sovereignty in a System Prompt

**原文标题**: Sovereignty in a System Prompt

**原文链接**: [https://pop.rdi.sh/sovereignty-in-a-system-prompt/](https://pop.rdi.sh/sovereignty-in-a-system-prompt/)

生成摘要时出错

---

## 85. Show HN: I ported Tree-sitter to Go

**原文标题**: Show HN: I ported Tree-sitter to Go

**原文链接**: [https://github.com/odvcencio/gotreesitter](https://github.com/odvcencio/gotreesitter)

生成摘要时出错

---

## 86. Show HN: Clocksimulator.com – A minimalist, distraction-free analog clock

**原文标题**: Show HN: Clocksimulator.com – A minimalist, distraction-free analog clock

**原文链接**: [https://www.clocksimulator.com/](https://www.clocksimulator.com/)

生成摘要时出错

---

## 87. Large-scale online deanonymization with LLMs

**原文标题**: Large-scale online deanonymization with LLMs

**原文链接**: [https://arxiv.org/abs/2602.16800](https://arxiv.org/abs/2602.16800)

生成摘要时出错

---

## 88. GNU Texmacs

**原文标题**: GNU Texmacs

**原文链接**: [https://www.texmacs.org/tmweb/home/welcome.en.html](https://www.texmacs.org/tmweb/home/welcome.en.html)

生成摘要时出错

---

## 89. Fed's Cook says AI triggering big changes, sees possible unemployment rise

**原文标题**: Fed's Cook says AI triggering big changes, sees possible unemployment rise

**原文链接**: [https://www.reuters.com/business/feds-cook-says-ai-triggering-big-changes-sees-possible-short-term-unemployment-2026-02-24/](https://www.reuters.com/business/feds-cook-says-ai-triggering-big-changes-sees-possible-short-term-unemployment-2026-02-24/)

生成摘要时出错

---

## 90. An AI doomsday report shook US markets

**原文标题**: An AI doomsday report shook US markets

**原文链接**: [https://www.theguardian.com/technology/2026/feb/24/feedback-loop-no-brake-how-ai-doomsday-report-rattled-markets](https://www.theguardian.com/technology/2026/feb/24/feedback-loop-no-brake-how-ai-doomsday-report-rattled-markets)

生成摘要时出错

---

## 91. Amazon would rather blame its own engineers than its AI

**原文标题**: Amazon would rather blame its own engineers than its AI

**原文链接**: [https://www.theregister.com/2026/02/24/amazon_blame_human_not_ai/](https://www.theregister.com/2026/02/24/amazon_blame_human_not_ai/)

生成摘要时出错

---

## 92. Manjaro website off-line again due to lapsed certificate

**原文标题**: Manjaro website off-line again due to lapsed certificate

**原文链接**: [https://distrowatch.com/dwres.php?resource=showheadline&story=20140](https://distrowatch.com/dwres.php?resource=showheadline&story=20140)

生成摘要时出错

---

## 93. Trump Fake Electors Plot

**原文标题**: Trump Fake Electors Plot

**原文链接**: [https://en.wikipedia.org/wiki/Trump_fake_electors_plot](https://en.wikipedia.org/wiki/Trump_fake_electors_plot)

生成摘要时出错

---

## 94. Intel XeSS 3: expanded support for Core Ultra/Core Ultra 2 and Arc A, B series

**原文标题**: Intel XeSS 3: expanded support for Core Ultra/Core Ultra 2 and Arc A, B series

**原文链接**: [https://www.intel.com/content/www/us/en/download/785597/intel-arc-graphics-windows.html](https://www.intel.com/content/www/us/en/download/785597/intel-arc-graphics-windows.html)

生成摘要时出错

---

## 95. xAI and Pentagon reach deal to use Grok in classified systems

**原文标题**: xAI and Pentagon reach deal to use Grok in classified systems

**原文链接**: [https://www.axios.com/2026/02/23/ai-defense-department-deal-musk-xai-grok](https://www.axios.com/2026/02/23/ai-defense-department-deal-musk-xai-grok)

生成摘要时出错

---

## 96. Human Existence Is Just as Wasteful as AI Data Centers, Sam Altman Suggests

**原文标题**: Human Existence Is Just as Wasteful as AI Data Centers, Sam Altman Suggests

**原文链接**: [https://decrypt.co/358849/human-existence-wasteful-ai-data-centers-sam-altman](https://decrypt.co/358849/human-existence-wasteful-ai-data-centers-sam-altman)

生成摘要时出错

---

## 97. I think WebRTC is better than SSH-ing for connecting to Mac terminal from iPhone

**原文标题**: I think WebRTC is better than SSH-ing for connecting to Mac terminal from iPhone

**原文链接**: [https://macky.dev](https://macky.dev)

生成摘要时出错

---

## 98. Ed Zitron loses his mind annotating an AI doomer macro memo

**原文标题**: Ed Zitron loses his mind annotating an AI doomer macro memo

**原文链接**: [https://www.dropbox.com/scl/fi/1p1n0y1ip48ianok9dvbp/Annotation-The-Global-Intelligence-Crisis.pdf?dl=0&e=1&noscript=1&rlkey=qaar8ea6l5hh6jqls4x6g8q4b](https://www.dropbox.com/scl/fi/1p1n0y1ip48ianok9dvbp/Annotation-The-Global-Intelligence-Crisis.pdf?dl=0&e=1&noscript=1&rlkey=qaar8ea6l5hh6jqls4x6g8q4b)

生成摘要时出错

---

## 99. My lobster lost $450k this weekend

**原文标题**: My lobster lost $450k this weekend

**原文链接**: [https://pashpashpash.substack.com/p/my-lobster-lost-450000-this-weekend](https://pashpashpash.substack.com/p/my-lobster-lost-450000-this-weekend)

生成摘要时出错

---

## 100. Porting Doom to a 20-year-old VoIP phone

**原文标题**: Porting Doom to a 20-year-old VoIP phone

**原文链接**: [https://0x19.co/post/snom360_doom/](https://0x19.co/post/snom360_doom/)

生成摘要时出错

---

