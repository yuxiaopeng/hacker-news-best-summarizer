# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-07-18.md)

*最后自动更新时间: 2026-07-18 20:28:28*
## 1. LG 显示器未经用户同意通过 Windows 更新静默安装软件

**原文标题**: LG monitors silently install software through Windows Update without consent

**原文链接**: [https://videocardz.com/newz/lg-monitors-silently-install-software-through-windows-update-without-user-consent](https://videocardz.com/newz/lg-monitors-silently-install-software-through-windows-update-without-user-consent)

据报道，LG 显示器通过 Windows 更新在未经用户同意的情况下安装了不需要的软件，其中包括迈克菲（McAfee）推广内容。Gamers Nexus 使用一台 LG UltraGear 34GX900A-B 显示器重现了这一情况，并观察到 Windows 更新首先安装了 LG 扩展包，随后“LG 显示器应用安装程序”在一分钟内悄然出现。

整个安装过程没有出现任何同意提示。Gamers Nexus 发现，该软件在 32 次系统启动中有 31 次显示了迈克菲的推广内容，提供为期 30 天的试用，到期后将转为付费订阅。在另一次启动中，它则推广了一个 LG 工具程序。这种行为不限于新显示器，因为它也影响了一台使用了三年的 LG UltraFine 32UN880-B。

令人担忧的问题包括缺乏用户批准、持续出现的迈克菲弹窗，以及该应用程序在微软商店中列出的广泛权限（互联网访问、所有系统资源）。

戴尔也将其 Alienware 命令中心软件用于这种自动安装方法。为了阻止此类安装，用户可以在 Windows 组策略（计算机配置、管理模板、系统和设备安装）中启用“阻止自动下载与设备元数据相关的应用程序”设置。然而，此设置也可能会阻止有用且合法的显示器或外设软件自动安装。

---

## 2. 倒退式 JPEG

**原文标题**: Regressive JPEGs

**原文链接**: [https://maurycyz.com/projects/bad_jpeg/](https://maurycyz.com/projects/bad_jpeg/)

文章《逆向JPEG》探讨了如何操纵渐进式JPEG格式，该格式通常通过将数据保存在多个“扫描”中，先显示低分辨率图像，然后逐步添加细节。作者发现，这些扫描可以被构造，以有效地*覆盖*先前渲染的图像数据。

最初尝试连接多个完整图像并过滤掉标记，展示了这种切换行为，但大多数解码器在大约九次扫描后停止处理，以防止类似“压缩炸弹”的问题。此外，旨在细化现有数据的高频（AC）扫描，以这种方式使用时会导致不希望的“重影”效果。

解决方案是创建仅由“纯DC”扫描组成的JPEG。每个纯DC扫描仅提供所有颜色通道（YCbCr）的最低频率分量，有效地逐块呈现一个新的、低分辨率（原始图像的1/16）图像，而没有重影。该技术使得大约90帧可以被打包到一个JPEG中，从而创建了一个基本的视频。

尽管这是对JPEG标准进行利用的巧妙演示，但该方法缺乏实际应用，因为它无法嵌入时间信息；播放速度完全取决于网络下载速率。然而，它支持创造性的用途，例如非传统形式的“瑞克摇”（rickrolls）或在没有CSS或JavaScript的单个HTML文件中实现独特的交互式局部渲染体验。

---

## 3. 凯撒护士称，人工智能和监控正在损害他们的工作和病患护理。

**原文标题**: Kaiser nurses say AI, surveillance are making their jobs and patient care worse

**原文链接**: [https://localnewsmatters.org/2026/07/15/kaiser-nurses-say-ai-workplace-surveillance-are-making-their-jobs-and-patient-care-worse/](https://localnewsmatters.org/2026/07/15/kaiser-nurses-say-ai-workplace-surveillance-are-making-their-jobs-and-patient-care-worse/)

凯撒医疗机构的护士们对人工智能（AI）和监控如何对其工作和患者护理产生负面影响发出了警报。护士们，特别是那些在咨询和分诊呼叫中心的护士，报告称如果她们的通话时长超过15分钟，就会面临批评和绩效评估，通话时长甚至会计入她们的月度评分。凯撒还使用软件来预测低效率，并测试了AI系统来评估护士的同理心和语调。

护士们表示，她们感到有压力要缩短那些复杂或情绪化的通话，例如与有自杀倾向的患者、慢性病患者或需要翻译的患者的通话，原因是对受到斥责的恐惧。她们说，这种压力迫使她们优先考虑效率而非提供富有同情心、周全的护理，并可能导致无法提供关键建议，从而使患者面临风险。她们感到受到骚扰，并且认为AI工具经常误解她们的工作。

加州护士协会（CNA）正在将AI作为与凯撒正在进行的合同谈判中的一个核心议题，此前她们已举行了罢工和抗议活动，反对AI的使用。护士们认为，这些监控方法损害了她们的专业判断，并导致了压力和职业倦怠，尽管凯撒声称它们能提高患者治疗效果，并否认使用“平均处理时间”进行绩效考核。

专家和倡导者，包括“消费者监督”组织，认为这种模式反映了凯撒长期以来优先考虑成本而非护理质量的倾向，并将其与更广泛的算法管理趋势联系起来，这种趋势将员工变成了“血肉机器人”。护士们强调，她们面对的是生命，而不仅仅是客户服务，技术应该造福患者，而不仅仅是提高生产力和削减成本。

---

## 4. 遥远恒星宜居带类地行星首次发现大气层

**原文标题**: First atmosphere found on Earth-like planet in habitable zone of distant star

**原文链接**: [https://www.bbc.com/news/articles/cy4kdd1e0ejo](https://www.bbc.com/news/articles/cy4kdd1e0ejo)

研究人员取得了一项突破性发现：首次在一个遥远恒星的宜居带内，类地岩石行星上探测到大气层。哈佛大学的Collin Cherubim博士称这项发现为“一项重大发现”，它提供了迄今为止最有力的证据，表明太阳系外可能存在类似地球的条件。

这颗行星被命名为LHS 1140 b，距离地球48光年，围绕一颗红矮星运行。尽管探测到的大气气体主要由氦组成，这种气体本身无法维持生命，但科学家推测，在更低的高度可能存在其他更能支持生命的气体。

这项发现是回答“生命是否存在于其他地方”这一根本性问题的关键一步。位于“宜居带”（即与恒星距离适中，足以使液态水存在的区域）的行星被认为是生命存在的首要候选者。尽管已在这些区域发现数百颗行星，但LHS 1140 b的独特之处在于它是一颗被证实拥有大气层的小型岩石世界。

David Charbonneau博士强调了在太阳系外发现一颗拥有大气层的类地行星的重要性。尽管此前对K2-18b和TRAPPIST-1等系外行星的研究提供了引人入胜的线索，但LHS 1140 b标志着首次在宜居带的岩石世界上确定性地探测到大气层。尽管尚未发现生命，但这项发现使人类离实现这一终极科学目标又近了一大步。

---

## 5. 开源AI的现状

**原文标题**: The state of open source AI

**原文链接**: [https://stateofopensource.ai/](https://stateofopensource.ai/)

2026年7月发布的《开源AI现状V1.0》报告强调了开源AI在促进竞争、互操作性和用户所有权方面的关键作用，这呼应了Mozilla过去为开放网络而战的经历。

报告显示，开源权重模型已大大缩小与顶级闭源模型的能力差距，在编码和通用知识等领域取得了对等能力，尽管闭源模型在推理方面仍保持领先。与此同时，GPT-4级别的推理成本在36个月内下降了50倍，使得开源模型显著更具成本效益。因此，在注重成本的开发者驱动下，开源模型目前在OpenRouter等平台上承载了大部分生产级令牌。

尽管开源模型在开发者采纳方面处于领先地位（79%），但它们在投入生产方面面临重大障碍（仅51%，而闭源模型为63%）。这种“运营差距”源于缺乏成熟的工具、标准化和企业级就绪性，而非模型能力。开源AI技术栈在能力上得分较高，但在运营成熟度上得分较低。

在财务方面，开源权重AI是一个数千亿美元的商业市场，获得了大量风险投资支持，并拥有经过验证的收入模式（例如，托管推理、企业平台）。DeepSeek和Mistral等公司展现出快速增长和高估值。闭源模型的按量计费模式在规模化应用中正变得不可持续，促使用户转向更经济的开源替代方案。

在全球范围内，开源AI是一种“主权选择”。在自有硬件上运行模型的能力提供了选择性并摆脱了供应商锁定——这是从提供商突然切断访问的案例中吸取的惨痛教训。中国通过有意的政策，成为开源权重模型的主要来源，将其视为对抗技术垄断和出口管制的一种对冲，从而在全球范围内获得了大规模采用。

报告最后指出，“代理束缚”（agentic harness）是新的前沿，将其设想为AI的用户代理，就像开放网络的浏览器一样。

---

## 6. Evidence of inconsistencies in evaluation process and selection of winners

**原文标题**: Evidence of inconsistencies in evaluation process and selection of winners

**原文链接**: [https://www.kaggle.com/competitions/kaggle-measuring-agi/discussion/724918#3498423](https://www.kaggle.com/competitions/kaggle-measuring-agi/discussion/724918#3498423)

生成摘要时出错

---

## 7. 苹果向数十名OpenAI员工发出律师函

**原文标题**: Apple targets dozens of OpenAI employees with legal letters

**原文链接**: [https://www.ft.com/content/1b8c9d52-88a9-426b-ba47-f1811f859166](https://www.ft.com/content/1b8c9d52-88a9-426b-ba47-f1811f859166)

所提供的文本并非全文，而是《金融时报》文章的付费墙。唯一可获取的实质性信息来自标题：**据报道，苹果公司正以律师函针对数十名OpenAI员工。**

其余内容包括《金融时报》的各种订阅优惠，例如“FT Edit”、“Standard Digital”和“Premium Digital”套餐，详细介绍了它们各自的功能和定价结构。苹果公司针对OpenAI员工采取法律行动的实际细节、原因和背景都需通过这些订阅选项才能获取。

---

## 8. GPT-5.6 used a prompt to close a 30-year gap in convex optimization

**原文标题**: GPT-5.6 used a prompt to close a 30-year gap in convex optimization

**原文链接**: [https://old.reddit.com/r/math/comments/1uxj3cy/after_openais_cdc_proof_announcement_gpt56_used_a/](https://old.reddit.com/r/math/comments/1uxj3cy/after_openais_cdc_proof_announcement_gpt56_used_a/)

生成摘要时出错

---

## 9. Why do AI company logos look like buttholes? (2025)

**原文标题**: Why do AI company logos look like buttholes? (2025)

**原文链接**: [https://velvetshark.com/ai-company-logos-that-look-like-buttholes](https://velvetshark.com/ai-company-logos-that-look-like-buttholes)

生成摘要时出错

---

## 10. $100 AI Music Video: Claude Fable 5 vs. GPT-5.6 Sol

**原文标题**: $100 AI Music Video: Claude Fable 5 vs. GPT-5.6 Sol

**原文链接**: [https://www.tryai.dev/blog/ai-music-video-arena-claude-vs-gpt-5.6](https://www.tryai.dev/blog/ai-music-video-arena-claude-vs-gpt-5.6)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 2 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 3 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 4 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 5 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 6 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 7 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 8 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 9 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 10 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 11 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 12 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 13 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 14 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 15 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 16 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 17 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 18 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 19 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 20 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 21 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 22 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 23 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 24 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 25 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 26 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 27 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 28 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 29 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 30 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 31 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 32 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 33 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 34 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 35 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 36 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 37 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 38 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 39 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 40 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 41 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 42 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 43 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 44 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 45 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 46 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 47 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 48 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 49 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 50 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 51 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 52 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 53 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 54 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 55 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 56 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 57 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 58 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 59 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 60 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 61 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 62 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 63 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 64 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 65 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 66 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 67 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 68 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 69 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 70 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 71 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 72 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 73 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 74 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 75 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 76 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 77 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 78 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 79 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 80 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 81 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 82 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 83 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 84 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 85 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 86 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 87 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 88 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 89 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 90 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 91 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 92 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 93 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 94 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 95 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 96 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 97 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 98 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 99 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 100 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 101 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 102 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 103 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 104 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 105 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 106 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 107 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 108 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 109 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 110 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 111 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 112 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 113 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 114 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 115 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 116 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 117 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 118 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 119 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 120 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 121 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 122 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 123 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 124 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 125 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 126 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 127 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 128 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 129 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 130 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 131 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 132 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 133 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 134 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 135 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 136 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 137 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 138 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 139 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 140 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 141 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 142 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 143 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 144 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 145 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 146 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 147 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 148 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 149 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 150 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 151 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 152 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 153 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 154 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 155 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 156 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 157 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 158 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 159 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 160 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 161 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 162 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 163 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 164 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 165 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 166 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 167 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 168 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 169 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 170 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 171 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 172 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 173 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 174 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 175 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 176 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 177 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 178 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 179 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 180 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 181 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 182 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 183 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 184 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 185 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 186 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 187 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 188 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 189 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 190 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 191 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 192 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 193 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 194 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 195 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 196 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 197 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 198 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 199 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 200 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 201 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 202 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 203 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 204 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 205 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 206 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 207 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 208 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 209 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 210 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 211 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 212 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 213 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 214 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 215 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 216 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 217 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 218 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 219 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 220 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 221 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 222 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 223 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 224 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 225 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 226 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 227 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 228 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 229 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 230 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 231 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 232 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 233 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 234 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 235 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 236 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 237 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 238 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 239 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 240 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 241 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 242 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 243 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 244 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 245 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 246 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 247 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 248 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 249 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 250 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 251 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 252 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 253 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
