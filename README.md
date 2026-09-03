# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-09-03.md)

*最后自动更新时间: 2026-09-03 22:02:08*
## 1. 双子座 3.8 闪 和 3.8 闪 赛博

**原文标题**: Gemini 3.8 Flash and 3.8 Flash Cyber

**原文链接**: [https://blog.google/innovation-and-ai/models-and-research/gemini-models/3-8-flash-and-3-8-flash-cyber/](https://blog.google/innovation-and-ai/models-and-research/gemini-models/3-8-flash-and-3-8-flash-cyber/)

谷歌于2026年9月2日推出了Gemini 3.8 Flash和3.8 Flash Cyber，为代理工作流和网络安全提供下一代智能。这些模型建立在相同的基本智能之上，并通过代理循环和严格的网络安全训练得到加速。

Gemini 3.8 Flash被描述为谷歌最智能的“主力模型”，在软件工程、代理任务和多步推理方面相比3.7 Flash有显著改进，性能常接近更高成本的前沿模型。它通过执行更多推理步骤和工具调用来“更努力地工作”。该模型通过Gemini API、Google AI Studio和Android Studio向开发者开放；通过Gemini Enterprise向企业提供；并通过Google AI Pro和Ultra订阅向消费者提供。它保持与3.7 Flash相同的入门价格。

Gemini 3.8 Flash Cyber是谷歌最强大的网络安全模型，在自主漏洞发现（例如CyberGym）和自动化补丁修复（例如CWE-Bench）方面展现出前沿水平的性能。它专注于防御能力，并已在保护谷歌代码安全方面展现出实际影响，包括Chrome和云服务的漏洞。由于其更灵活的网络安全缓解措施，Flash Cyber仅通过新的“顺风计划”向可信赖的防御者（例如政府机构和关键基础设施运营商）提供。

这两个模型在设计时都考虑了安全性，融入了防范在核生化（CBRN）和网络攻击领域滥用的安全措施，并在提示注入的鲁棒性方面有显著改进。

---

## 2. .name 终止

**原文标题**: .name Termination

**原文链接**: [https://neil.fraser.name/news/2026/09/03/](https://neil.fraser.name/news/2026/09/03/)

Neil Fraser报告称，包括他近25年前作为网站、电子邮件和API服务器设立并长期使用的neil.fraser.name在内的所有三级.name域名即将被终止。Verisign于2026年4月15日提出此举，旨在简化管理，ICANN于2026年7月28日批准，尽管Fraser的域名已付费至2040年。该终止将于2027年2月生效。

作为22,000名受影响用户之一，Fraser强调，.name三级域名是合法的，拥有完整的WHOIS记录，这与其他可疑的三级域名服务不同。他最初选择.name域名是因为不信任Verisign，而Verisign后来收购了Global Name Registry，并通过其提案中他所称的Verisign的“大量谎言”证实了他的担忧。

此次终止意味着Fraser的网站和电子邮件将消失，与其域名关联的物联网设备也将停止运作。一个更严重的威胁是，其他人可能会注册现在空置的二级域名（fraser.name）。这将使他们能够重新创建neil.fraser.name，从而可能劫持数百个关联账户，以他的身份提交代码，并夺取对他物联网设备的控制权。Fraser最后表示他将“寻求法律帮助”。

---

## 3. Audacity 4.0

**原文标题**: Audacity 4.0

**原文链接**: [https://github.com/audacity/audacity/releases/tag/Audacity-4.0.0](https://github.com/audacity/audacity/releases/tag/Audacity-4.0.0)

Audacity 4.0 标志着这款音频编辑器的一次重大重建，引入了一个基于 Qt 全面革新的界面，具有原生的DPI渲染和广泛的自定义功能。用户可以将 UI 布局保存为工作区（现代、经典、音乐），从多种主题中选择，并可停靠/浮动工具栏。新的“主页”屏幕显示带有预览缩略图的近期项目。

一个重要的关注点是新的片段编辑模型，允许直接选择和编辑多个片段、进行分组，并灵活地在不同轨道上放置。专用的分割工具和改进的粘贴功能简化了工作流程。以前独立的工具模式（选择、包络、绘图、多工具）现在变为上下文敏感。

播放和录制方面也有增强，例如持久、可拖动的播放头、无需停止即可查找以及可在时间轴上任何位置开始录制。官方 Windows 版本现在支持 ASIO。轨道头部包含实时电平表，内置效果已针对新界面进行重建，支持 VST3、Nyquist、LV2 和 Audio Units。频谱图也经过重新设计，以提高清晰度。

项目现在使用 .aup4 格式，转换 .aup3 项目时，原始文件保持不变（尽管无法保存回 .aup3 格式）。更旧的 .aup 项目也可以导入。Audacity 标志已更新。

Audacity 3 中目前缺失的关键功能包括时间轨道、音符/MIDI 轨道、混音器、宏管理器/脚本管道、VAMP/LADSPA 插件宿主和变速播放，但计划在未来重新引入。部分导出、渲染、分析器和效果也暂时缺失。

---

## 4. GPT-6 阿斯特拉

**原文标题**: GPT-6 Astra

**原文链接**: [https://openai.com/index/gpt-6-astra/](https://openai.com/index/gpt-6-astra/)

GPT-6 Astra 被推出为 OpenAI 的下一代、最智能、最对齐的模型，在多个领域树立了新基准。它取得了最先进的性能，包括在 FrontierMath Tier 4 上达到 98%，在 ARC-AGI-3 上达到 99.9%，并在 ExploitBench 上达到完美的 100%。

Astra 显著提升了计算机使用效率，在 OSWorld 2.0 上完成任务的速度比 GPT-5.6 Sol 快 47%，在 Mind2Web 上快 1.9 倍。它擅长自动化繁琐任务、在线研究、数据分析和网络开发。在专业工作中，它能生成精美的文档，遵循模板，并有效解读指令。在软件工程领域，Astra 是迄今为止最好的模型，具备最先进的编码能力和创新的 Codex 功能以保留上下文。它也代表了科学发现方面的一大进步。

在网络安全领域，Astra 达到了“关键”能力阈值，展示了识别和开发零日漏洞的熟练度，甚至在评估期间发现了新的漏洞。虽然最初专注于安全代码审查等防御性应用，但计划在漏洞分析和恶意软件分析方面提供更广泛的访问。

至关重要的是，Astra 是 OpenAI 最对齐的模型，在理解用户意图、遵守任务边界（在关键测试中偏差为 0%）和透明沟通方面表现出显著改进。它将首先向有限的组织推出，随后面向 ChatGPT Plus、Pro、Business、Enterprise 用户，并通过 OpenAI API 和 AWS 提供。

---

## 5. LWN 订阅价格说明

**原文标题**: A note on subscription prices from LWN

**原文链接**: [https://lwn.net/Articles/1090585/](https://lwn.net/Articles/1090585/)

LWN宣布将于9月15日起上调订阅价格，将此决定归因于全球经济的重大变化和成本的上涨。自2022年初上次价格调整以来，消费价格通胀已接近20%，而医疗保险等一些费用甚至增长更多。

该出版物于2002年采纳了读者支持的订阅模式，以保持其独立性，不受广告影响，并强调读者的支持对其生存至关重要。LWN 很少涨价（24年内仅两次）。上次涨价使他们得以通过聘用新员工（Daroc Alden和Joe Brockmeier）来扩大内容覆盖范围，增强网站功能（例如EPUB文章、Markdown评论、深色模式、内核数据库），并加强了对爬虫攻击的防御。

新价格将上涨约20%以匹配通胀，具体为：Starving hacker（6.00美元）、Professional hacker（11.00美元）、Project leader（19.00美元）和Maniacal supporter（55.00美元）。团体订阅价格也将按比例上涨。

现有的预购订阅将继续有效，直至其原始到期日。在公告发布前活跃的月度订阅者将在未来六个月内继续支付旧价格，在新价格生效前会收到提醒。

尽管LWN倾向于保持低价并扩大订阅量，但订阅用户增长停滞迫使他们采取这一短期措施，同时他们也在制定长期增长战略。随着LWN即将迎来成立30周年，它向忠实读者表达了深切的感谢，并将持续的活力归功于他们的支持。

---

## 6. 缪斯火花 1.3

**原文标题**: Muse Spark 1.3

**原文链接**: [https://developer.meta.com/ai/models/muse-spark/](https://developer.meta.com/ai/models/muse-spark/)

Muse Spark 被视为 Meta 最紧凑、最高效的生成式AI模型，专为设备端应用和边缘部署而设计。它是Meta AI模型家族的一部分，针对低延迟、小模型尺寸和本地处理至关重要的场景进行了优化。

其主要特点包括高效率和直接在设备上运行的能力，使其适用于广泛的移动、可穿戴设备和物联网应用。这使得无需依赖云连接即可实现实时AI功能，从而增强用户隐私并降低运营成本。Muse Spark 定位用于设备端内容创作、个性化AI体验和智能语音助手等用例。

开发者可以通过Meta的AI模型计划访问Muse Spark，并可获得相关资源将其集成到他们的应用程序中。该模型强调使开发者能够将创新、保护隐私且高性能的AI功能直接构建到他们的产品中。

---

## 7. 三个网站制作了215,128个AI“最佳软件”页面。Perplexity引用了这些网站。

**原文标题**: Three sites made 215,128 “best software” pages for AI. Perplexity cites them

**原文链接**: [https://trellner.com/reports/manufactured-sources-behind-ai-recommendations/](https://trellner.com/reports/manufactured-sources-behind-ai-recommendations/)

一项研究调查了Perplexity AI模型（sonar和sonar-pro）在回答380个类别中“最佳软件”问题时使用的来源，并分析了7,534条引文。一个惊人的发现是，59.8%的引文指向Tranco排名低于100,000的域名，而23.4%的引文则完全在排名前一百万之外。这些低排名域名也明显更新，其Wayback Machine首次捕获时间的中间值为2020年，而有排名的域名则为2011年。

主要的问题来源包括guideflow.com，这是一个供应商的营销博客，尽管它不是评论网站，也不在引用的类别中竞争，却是被引用次数第三多的域名。更令人担忧的是，有三个网站——wifitalents.com、worldmetrics.org和gitnux.org——近期（2023年12月至2024年5月）注册并共享基础设施，共同发布了215,128个机器生成的“最佳<类别>软件”页面。它们的首页标题为“事实与基础页面”，表明它们是为AI检索而非人类读者优化的。这些网站还为同一类别提供了不一致的“最佳”排名。

此外，一些被推荐的供应商主页无法访问，或被重定向到不相关的网站，例如在线赌博门户。该研究澄清，它衡量的是Perplexity的检索层，而非其他AI模型，并且侧重于证据基础的性质，而非最终推荐的质量。这凸显了AI模型在获取基础信息时，对新的、低质量和机器生成内容的严重依赖。

---

## 8. Can I opt out of my input or output data being used for training?

**原文标题**: Can I opt out of my input or output data being used for training?

**原文链接**: [https://help.mistral.ai/en/articles/455207-can-i-opt-out-of-my-input-or-output-data-being-used-for-training](https://help.mistral.ai/en/articles/455207-can-i-opt-out-of-my-input-or-output-data-being-used-for-training)

生成摘要时出错

---

## 9. Google avoids a breakup of its ad tech business

**原文标题**: Google avoids a breakup of its ad tech business

**原文链接**: [https://www.nytimes.com/2026/09/02/technology/google-ad-tech-remedies.html](https://www.nytimes.com/2026/09/02/technology/google-ad-tech-remedies.html)

生成摘要时出错

---

## 10. FBI Probes Service Selling 153M+ Drivers Licenses

**原文标题**: FBI Probes Service Selling 153M+ Drivers Licenses

**原文链接**: [https://krebsonsecurity.com/2026/09/fbi-probes-service-selling-153m-drivers-licenses/](https://krebsonsecurity.com/2026/09/fbi-probes-service-selling-153m-drivers-licenses/)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-09-03](output/hacker_news_summary_2026-09-03.md) |
| 2 | [2026-08-29](output/hacker_news_summary_2026-08-29.md) |
| 3 | [2026-08-31](output/hacker_news_summary_2026-08-31.md) |
| 4 | [2026-09-01](output/hacker_news_summary_2026-09-01.md) |
| 5 | [2026-09-02](output/hacker_news_summary_2026-09-02.md) |
| 6 | [2026-08-30](output/hacker_news_summary_2026-08-30.md) |
| 7 | [2026-08-21](output/hacker_news_summary_2026-08-21.md) |
| 8 | [2026-08-25](output/hacker_news_summary_2026-08-25.md) |
| 9 | [2026-08-26](output/hacker_news_summary_2026-08-26.md) |
| 10 | [2026-08-24](output/hacker_news_summary_2026-08-24.md) |
| 11 | [2026-08-28](output/hacker_news_summary_2026-08-28.md) |
| 12 | [2026-08-23](output/hacker_news_summary_2026-08-23.md) |
| 13 | [2026-08-22](output/hacker_news_summary_2026-08-22.md) |
| 14 | [2026-08-18](output/hacker_news_summary_2026-08-18.md) |
| 15 | [2026-08-15](output/hacker_news_summary_2026-08-15.md) |
| 16 | [2026-08-19](output/hacker_news_summary_2026-08-19.md) |
| 17 | [2026-08-20](output/hacker_news_summary_2026-08-20.md) |
| 18 | [2026-08-13](output/hacker_news_summary_2026-08-13.md) |
| 19 | [2026-08-14](output/hacker_news_summary_2026-08-14.md) |
| 20 | [2026-08-17](output/hacker_news_summary_2026-08-17.md) |
| 21 | [2026-08-16](output/hacker_news_summary_2026-08-16.md) |
| 22 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 23 | [2026-08-09](output/hacker_news_summary_2026-08-09.md) |
| 24 | [2026-08-10](output/hacker_news_summary_2026-08-10.md) |
| 25 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 26 | [2026-08-11](output/hacker_news_summary_2026-08-11.md) |
| 27 | [2026-08-12](output/hacker_news_summary_2026-08-12.md) |
| 28 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 29 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 30 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 31 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 32 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 33 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 34 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 35 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 36 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 37 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 38 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 39 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 40 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 41 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 42 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 43 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 44 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 45 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 46 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 47 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 48 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 49 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 50 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 51 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 52 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 53 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 54 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 55 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 56 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 57 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 58 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 59 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 60 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 61 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 62 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 63 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 64 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 65 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 66 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 67 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 68 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 69 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 70 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 71 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 72 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 73 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 74 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 75 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 76 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 77 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 78 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 79 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 80 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 81 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 82 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 83 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 84 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 85 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 86 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 87 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 88 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 89 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 90 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 91 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 92 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 93 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 94 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 95 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 96 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 97 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 98 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 99 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 100 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 101 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 102 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 103 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 104 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 105 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 106 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 107 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 108 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 109 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 110 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 111 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 112 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 113 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 114 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 115 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 116 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 117 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 118 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 119 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 120 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 121 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 122 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 123 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 124 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 125 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 126 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 127 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 128 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 129 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 130 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 131 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 132 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 133 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 134 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 135 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 136 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 137 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 138 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 139 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 140 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 141 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 142 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 143 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 144 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 145 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 146 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 147 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 148 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 149 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 150 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 151 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 152 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 153 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 154 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 155 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 156 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 157 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 158 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 159 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 160 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 161 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 162 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 163 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 164 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 165 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 166 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 167 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 168 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 169 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 170 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 171 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 172 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 173 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 174 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 175 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 176 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 177 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 178 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 179 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 180 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 181 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 182 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 183 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 184 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 185 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 186 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 187 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 188 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 189 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 190 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 191 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 192 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 193 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 194 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 195 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 196 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 197 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 198 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 199 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 200 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 201 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 202 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 203 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 204 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 205 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 206 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 207 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 208 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 209 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 210 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 211 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 212 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 213 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 214 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 215 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 216 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 217 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 218 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 219 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 220 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 221 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 222 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 223 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 224 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 225 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 226 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 227 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 228 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 229 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 230 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 231 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 232 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 233 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 234 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 235 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 236 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 237 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 238 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 239 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 240 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 241 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 242 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 243 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 244 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 245 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 246 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 247 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 248 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 249 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 250 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 251 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 252 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 253 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 254 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 255 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 256 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 257 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 258 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 259 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 260 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 261 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 262 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 263 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 264 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 265 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 266 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 267 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 268 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 269 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 270 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 271 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 272 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 273 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 274 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 275 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 276 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 277 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 278 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 279 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 280 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 281 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 282 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 283 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 284 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 285 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 286 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 287 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 288 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 289 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 290 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 291 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 292 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 293 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
| 294 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 295 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 296 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 297 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 298 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
