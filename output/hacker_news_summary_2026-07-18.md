# Hacker News 热门文章摘要 (2026-07-18)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

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

## 11. Kimi K3, and what we can still learn from the pelican benchmark

**原文标题**: Kimi K3, and what we can still learn from the pelican benchmark

**原文链接**: [https://simonwillison.net/2026/Jul/16/kimi-k3/](https://simonwillison.net/2026/Jul/16/kimi-k3/)

生成摘要时出错

---

## 12. LM Studio Bionic: the AI agent for open models

**原文标题**: LM Studio Bionic: the AI agent for open models

**原文链接**: [https://lmstudio.ai/blog/introducing-lm-studio-bionic](https://lmstudio.ai/blog/introducing-lm-studio-bionic)

生成摘要时出错

---

## 13. What AI did to stackoverflow in a graph

**原文标题**: What AI did to stackoverflow in a graph

**原文链接**: [https://data.stackexchange.com/stackoverflow/query/1953768#graph](https://data.stackexchange.com/stackoverflow/query/1953768#graph)

生成摘要时出错

---

## 14. Learning a few things about running SQLite

**原文标题**: Learning a few things about running SQLite

**原文链接**: [https://jvns.ca/blog/2026/07/17/learning-about-running-sqlite/](https://jvns.ca/blog/2026/07/17/learning-about-running-sqlite/)

生成摘要时出错

---

## 15. The human-in-the-loop is tired

**原文标题**: The human-in-the-loop is tired

**原文链接**: [https://pydantic.dev/articles/the-human-in-the-loop-is-tired](https://pydantic.dev/articles/the-human-in-the-loop-is-tired)

生成摘要时出错

---

## 16. Pebble Mega Update – July 2026

**原文标题**: Pebble Mega Update – July 2026

**原文链接**: [https://repebble.com/blog/pebble-mega-update-july-2026](https://repebble.com/blog/pebble-mega-update-july-2026)

生成摘要时出错

---

## 17. How Has Roman Concrete Lasted for Millennia? 1,900-Year-Old Latrine Offers Clues

**原文标题**: How Has Roman Concrete Lasted for Millennia? 1,900-Year-Old Latrine Offers Clues

**原文链接**: [https://www.smithsonianmag.com/smart-news/how-has-roman-concrete-lasted-for-millennia-a-1900-year-old-latrine-offers-new-clues-about-the-materials-impressive-durability-180989115/](https://www.smithsonianmag.com/smart-news/how-has-roman-concrete-lasted-for-millennia-a-1900-year-old-latrine-offers-new-clues-about-the-materials-impressive-durability-180989115/)

生成摘要时出错

---

## 18. Three ways people respond to a problem (other than solving it)

**原文标题**: Three ways people respond to a problem (other than solving it)

**原文链接**: [https://improvesomething.today/responses-to-problems/](https://improvesomething.today/responses-to-problems/)

生成摘要时出错

---

## 19. The Zilog Z80 has turned 50

**原文标题**: The Zilog Z80 has turned 50

**原文链接**: [https://goliath32.com/blog/z80.html](https://goliath32.com/blog/z80.html)

生成摘要时出错

---

## 20. EEG shows brain can simultaneous encode two speech streams

**原文标题**: EEG shows brain can simultaneous encode two speech streams

**原文链接**: [https://journals.plos.org/plosbiology/article?id=10.1371/journal.pbio.3003876](https://journals.plos.org/plosbiology/article?id=10.1371/journal.pbio.3003876)

生成摘要时出错

---

## 21. EU ban on destruction of unsold clothes and shoes enters into application

**原文标题**: EU ban on destruction of unsold clothes and shoes enters into application

**原文链接**: [https://environment.ec.europa.eu/news/ban-destruction-unsold-clothes-and-shoes-enters-application-2026-07-17_en](https://environment.ec.europa.eu/news/ban-destruction-unsold-clothes-and-shoes-enters-application-2026-07-17_en)

生成摘要时出错

---

## 22. Mathematics of Data Science

**原文标题**: Mathematics of Data Science

**原文链接**: [https://arxiv.org/abs/2607.11938](https://arxiv.org/abs/2607.11938)

生成摘要时出错

---

## 23. The Little Book of Reinforcement Learning

**原文标题**: The Little Book of Reinforcement Learning

**原文链接**: [https://github.com/alxndrTL/little-book-rl/](https://github.com/alxndrTL/little-book-rl/)

生成摘要时出错

---

## 24. TP-Link Kasa cameras leaked home GPS via unauthenticated UDP for 6 years

**原文标题**: TP-Link Kasa cameras leaked home GPS via unauthenticated UDP for 6 years

**原文链接**: [https://github.com/BadChemical/IoT-Vulnerability-Research-Public/blob/main/TP-Link_Kasa_EC71/Kasa_EC71.md](https://github.com/BadChemical/IoT-Vulnerability-Research-Public/blob/main/TP-Link_Kasa_EC71/Kasa_EC71.md)

生成摘要时出错

---

## 25. A Road to Lisp: Which Lisp

**原文标题**: A Road to Lisp: Which Lisp

**原文链接**: [https://scotto.me/blog/2026-07-17-which-lisp/](https://scotto.me/blog/2026-07-17-which-lisp/)

生成摘要时出错

---

## 26. Texas wins court order to suspend domain name for violating age-verification law

**原文标题**: Texas wins court order to suspend domain name for violating age-verification law

**原文链接**: [https://www.texasattorneygeneral.gov/news/releases/attorney-general-ken-paxton-secures-landmark-legal-victory-lock-pornographic-website-domain-and](https://www.texasattorneygeneral.gov/news/releases/attorney-general-ken-paxton-secures-landmark-legal-victory-lock-pornographic-website-domain-and)

生成摘要时出错

---

## 27. FAA lets Boeing sign off on 737 MAX, 787 airworthiness certificates again

**原文标题**: FAA lets Boeing sign off on 737 MAX, 787 airworthiness certificates again

**原文链接**: [https://www.cnbc.com/2026/07/17/faa-boeing-737-max-787.html](https://www.cnbc.com/2026/07/17/faa-boeing-737-max-787.html)

生成摘要时出错

---

## 28. GrapheneOS recommended for domestic abuse victims

**原文标题**: GrapheneOS recommended for domestic abuse victims

**原文链接**: [https://privacypros.com.au/privacy-hub/articles/dv-safe-phone-australia/](https://privacypros.com.au/privacy-hub/articles/dv-safe-phone-australia/)

生成摘要时出错

---

## 29. Fable 5 vs. GPT-5.6 Sol on an NP-Hard Problem: Does /goal help?

**原文标题**: Fable 5 vs. GPT-5.6 Sol on an NP-Hard Problem: Does /goal help?

**原文链接**: [https://charlesazam.com/blog/fable-5-gpt-5-6-sol-goal/](https://charlesazam.com/blog/fable-5-gpt-5-6-sol-goal/)

生成摘要时出错

---

## 30. Trump Media to sell instant access to 'market-moving' social posts

**原文标题**: Trump Media to sell instant access to 'market-moving' social posts

**原文链接**: [https://www.bbc.com/news/articles/c79gw4lj89eo](https://www.bbc.com/news/articles/c79gw4lj89eo)

生成摘要时出错

---

## 31. Show HN: Watch bots interact with an SSH honeypot in real time

**原文标题**: Show HN: Watch bots interact with an SSH honeypot in real time

**原文链接**: [https://honeypotlive.cc/](https://honeypotlive.cc/)

生成摘要时出错

---

## 32. Static search trees: 40x faster than binary search (2024)

**原文标题**: Static search trees: 40x faster than binary search (2024)

**原文链接**: [https://curiouscoding.nl/posts/static-search-tree/](https://curiouscoding.nl/posts/static-search-tree/)

生成摘要时出错

---

## 33. Short sellers notch $8.7B profit as SpaceX shares dip to IPO price

**原文标题**: Short sellers notch $8.7B profit as SpaceX shares dip to IPO price

**原文链接**: [https://www.reuters.com/business/media-telecom/short-sellers-rack-up-87-bln-profit-spacex-slips-below-ipo-price-ortex-2026-07-16/](https://www.reuters.com/business/media-telecom/short-sellers-rack-up-87-bln-profit-spacex-slips-below-ipo-price-ortex-2026-07-16/)

生成摘要时出错

---

## 34. My car’s OTA update broke Android Auto

**原文标题**: My car’s OTA update broke Android Auto

**原文链接**: [https://imdanielkendall.com/the-great-software-regress-how-move-fast-and-break-things-broke-our-lives/](https://imdanielkendall.com/the-great-software-regress-how-move-fast-and-break-things-broke-our-lives/)

生成摘要时出错

---

## 35. Open Book Touch: open-source e-reader

**原文标题**: Open Book Touch: open-source e-reader

**原文链接**: [https://www.crowdsupply.com/oddly-specific-objects/open-book-touch](https://www.crowdsupply.com/oddly-specific-objects/open-book-touch)

生成摘要时出错

---

## 36. Frame – Linux X server in Assembly

**原文标题**: Frame – Linux X server in Assembly

**原文链接**: [https://isene.org/2026/07/Frame.html](https://isene.org/2026/07/Frame.html)

生成摘要时出错

---

## 37. Lego building instructions through time

**原文标题**: Lego building instructions through time

**原文链接**: [https://www.lego.com/en-us/history/articles/d-lego-building-instructions-through-time](https://www.lego.com/en-us/history/articles/d-lego-building-instructions-through-time)

生成摘要时出错

---

## 38. Helium escaping from atmosphere of nearby rocky exoplanet in a habitable zone

**原文标题**: Helium escaping from atmosphere of nearby rocky exoplanet in a habitable zone

**原文链接**: [https://www.science.org/doi/10.1126/science.aea9708](https://www.science.org/doi/10.1126/science.aea9708)

生成摘要时出错

---

## 39. Claude Code: Anatomy of a Misfeature

**原文标题**: Claude Code: Anatomy of a Misfeature

**原文链接**: [https://www.olafalders.com/2026/07/17/claude-code-anatomy-of-a-misfeature/](https://www.olafalders.com/2026/07/17/claude-code-anatomy-of-a-misfeature/)

生成摘要时出错

---

## 40. Show HN: IKEA Complexity Index

**原文标题**: Show HN: IKEA Complexity Index

**原文链接**: [https://ikea.greg.technology/](https://ikea.greg.technology/)

生成摘要时出错

---

## 41. More Bounce to the Ounce

**原文标题**: More Bounce to the Ounce

**原文链接**: [https://mceglowski.substack.com/p/more-bounce-to-the-ounce](https://mceglowski.substack.com/p/more-bounce-to-the-ounce)

生成摘要时出错

---

## 42. Painting the sides of railroad rails white to reduce derailment

**原文标题**: Painting the sides of railroad rails white to reduce derailment

**原文链接**: [https://www.up.com/news/safety/Tracking-Rail-Heat-260608](https://www.up.com/news/safety/Tracking-Rail-Heat-260608)

生成摘要时出错

---

## 43. Gleam Is Now on Tangled

**原文标题**: Gleam Is Now on Tangled

**原文链接**: [https://tangled.org/gleam.run/gleam](https://tangled.org/gleam.run/gleam)

生成摘要时出错

---

## 44. Goodbye, and Thanks for All the Bikesheds

**原文标题**: Goodbye, and Thanks for All the Bikesheds

**原文链接**: [https://queue.acm.org/detail.cfm?id=3818307](https://queue.acm.org/detail.cfm?id=3818307)

生成摘要时出错

---

## 45. The Computer at the Bottom of a Canal

**原文标题**: The Computer at the Bottom of a Canal

**原文链接**: [https://negroniventurestudios.com/2026/07/18/the-computer-at-the-bottom-of-a-canal/](https://negroniventurestudios.com/2026/07/18/the-computer-at-the-bottom-of-a-canal/)

生成摘要时出错

---

## 46. 'Likweli': A new monkey species discovered in the Congo Basin

**原文标题**: 'Likweli': A new monkey species discovered in the Congo Basin

**原文链接**: [https://news.yale.edu/2026/07/15/meet-likweli-new-monkey-species-discovered-congo-basin](https://news.yale.edu/2026/07/15/meet-likweli-new-monkey-species-discovered-congo-basin)

生成摘要时出错

---

## 47. Kimi K3 is now #1 in the Front end Code Arena with 1679 pts, surpassing Fable 5

**原文标题**: Kimi K3 is now #1 in the Front end Code Arena with 1679 pts, surpassing Fable 5

**原文链接**: [https://twitter.com/arena/status/2077824029126504525](https://twitter.com/arena/status/2077824029126504525)

生成摘要时出错

---

## 48. Topcoat: The full full-stack framework for Rust

**原文标题**: Topcoat: The full full-stack framework for Rust

**原文链接**: [https://github.com/tokio-rs/topcoat](https://github.com/tokio-rs/topcoat)

生成摘要时出错

---

## 49. Setting up your spare Mac for Claude Code to control, a step-by-step guide

**原文标题**: Setting up your spare Mac for Claude Code to control, a step-by-step guide

**原文链接**: [https://ykdojo.github.io/claude-controls-mac/](https://ykdojo.github.io/claude-controls-mac/)

生成摘要时出错

---

## 50. Show HN: A zoomable timeline of 4M Wikipedia events

**原文标题**: Show HN: A zoomable timeline of 4M Wikipedia events

**原文链接**: [https://app.everything.diena.co/](https://app.everything.diena.co/)

生成摘要时出错

---

## 51. The privacy problems hidden in your period tracker

**原文标题**: The privacy problems hidden in your period tracker

**原文链接**: [https://www.bbc.com/future/article/20260715-how-period-trackers-share-womens-private-details](https://www.bbc.com/future/article/20260715-how-period-trackers-share-womens-private-details)

生成摘要时出错

---

## 52. If You Build It, They Will Come

**原文标题**: If You Build It, They Will Come

**原文链接**: [https://www.benlandautaylor.com/p/if-you-build-it-they-will-come](https://www.benlandautaylor.com/p/if-you-build-it-they-will-come)

生成摘要时出错

---

## 53. Elixir-lang.org has a new design

**原文标题**: Elixir-lang.org has a new design

**原文链接**: [https://elixir-lang.org/](https://elixir-lang.org/)

生成摘要时出错

---

## 54. Minikotlin

**原文标题**: Minikotlin

**原文链接**: [https://minikotlin.run](https://minikotlin.run)

生成摘要时出错

---

## 55. The Kimi K3 Moment

**原文标题**: The Kimi K3 Moment

**原文链接**: [https://stephen.bochinski.dev/blog/2026/07/18/the-kimi-k3-moment/](https://stephen.bochinski.dev/blog/2026/07/18/the-kimi-k3-moment/)

生成摘要时出错

---

## 56. I started a “dirt notebook”

**原文标题**: I started a “dirt notebook”

**原文链接**: [https://pinewind.bearblog.dev/i-started-a-dirt-notebook/](https://pinewind.bearblog.dev/i-started-a-dirt-notebook/)

生成摘要时出错

---

## 57. AI Meets Cryptography 2: What AI Found in OpenVM's ZkVM

**原文标题**: AI Meets Cryptography 2: What AI Found in OpenVM's ZkVM

**原文链接**: [https://blog.zksecurity.xyz/posts/openvm-bugs/](https://blog.zksecurity.xyz/posts/openvm-bugs/)

生成摘要时出错

---

## 58. I Owe My Life to the Commodore 64

**原文标题**: I Owe My Life to the Commodore 64

**原文链接**: [https://www.goto10retro.com/p/i-owe-my-life-to-the-commodore-64](https://www.goto10retro.com/p/i-owe-my-life-to-the-commodore-64)

生成摘要时出错

---

## 59. Steam Machine: Between 12k and 15k Units Sold per week

**原文标题**: Steam Machine: Between 12k and 15k Units Sold per week

**原文链接**: [https://boilingsteam.com/steam-machine-between-10k-and-15k-sold-per-week/](https://boilingsteam.com/steam-machine-between-10k-and-15k-sold-per-week/)

生成摘要时出错

---

## 60. Workspaces – Explore the workspaces of modern creators

**原文标题**: Workspaces – Explore the workspaces of modern creators

**原文链接**: [https://workspaces.xyz/](https://workspaces.xyz/)

生成摘要时出错

---

## 61. Homomorphically encrypted CIFAR-10 inference in 200ms

**原文标题**: Homomorphically encrypted CIFAR-10 inference in 200ms

**原文链接**: [https://sofar.belfortlabs.cloud/](https://sofar.belfortlabs.cloud/)

生成摘要时出错

---

## 62. The US grocery slowdown is real

**原文标题**: The US grocery slowdown is real

**原文链接**: [https://www.bain.com/insights/the-us-grocery-slowdown-is-real-snap-chart/](https://www.bain.com/insights/the-us-grocery-slowdown-is-real-snap-chart/)

生成摘要时出错

---

## 63. The Isomorphic Labs Drug Design Engine unlocks a new frontier beyond AlphaFold

**原文标题**: The Isomorphic Labs Drug Design Engine unlocks a new frontier beyond AlphaFold

**原文链接**: [https://www.isomorphiclabs.com/articles/the-isomorphic-labs-drug-design-engine-unlocks-a-new-frontier](https://www.isomorphiclabs.com/articles/the-isomorphic-labs-drug-design-engine-unlocks-a-new-frontier)

生成摘要时出错

---

## 64. British runner Josh Kerr breaks world record for mile which stood for 27 years

**原文标题**: British runner Josh Kerr breaks world record for mile which stood for 27 years

**原文链接**: [https://news.sky.com/story/british-runner-josh-kerr-breaks-world-record-for-mile-which-had-stood-for-27-years-13564688](https://news.sky.com/story/british-runner-josh-kerr-breaks-world-record-for-mile-which-had-stood-for-27-years-13564688)

生成摘要时出错

---

## 65. Meta trying to destroy whistleblower Sarah Wynn-Williams, US senator says

**原文标题**: Meta trying to destroy whistleblower Sarah Wynn-Williams, US senator says

**原文链接**: [https://www.theguardian.com/technology/2026/jul/17/meta-whistleblower-sarah-wynn-williams-us-senator-josh-hawley](https://www.theguardian.com/technology/2026/jul/17/meta-whistleblower-sarah-wynn-williams-us-senator-josh-hawley)

生成摘要时出错

---

## 66. Show HN: Mojibake – A low-level Unicode library written in C

**原文标题**: Show HN: Mojibake – A low-level Unicode library written in C

**原文链接**: [https://mojibake.zaerl.com/](https://mojibake.zaerl.com/)

生成摘要时出错

---

## 67. Stenchill: 3D Printable Solder Paste Stencil Generator

**原文标题**: Stenchill: 3D Printable Solder Paste Stencil Generator

**原文链接**: [https://www.stenchill.com/en/](https://www.stenchill.com/en/)

生成摘要时出错

---

## 68. Scaling to 1M concurrent sandboxes in seconds

**原文标题**: Scaling to 1M concurrent sandboxes in seconds

**原文链接**: [https://modal.com/blog/scaling-to-1-million-concurrent-sandboxes-in-seconds](https://modal.com/blog/scaling-to-1-million-concurrent-sandboxes-in-seconds)

生成摘要时出错

---

## 69. As a musician, I prefer illegal downloading over Spotify (2011)

**原文标题**: As a musician, I prefer illegal downloading over Spotify (2011)

**原文链接**: [https://derekwebb.tumblr.com/post/13503899950/giving-it-away-how-free-music-makes-more-than](https://derekwebb.tumblr.com/post/13503899950/giving-it-away-how-free-music-makes-more-than)

生成摘要时出错

---

## 70. Flock CEO Apologizes for Calling Activists 'Terrorists'

**原文标题**: Flock CEO Apologizes for Calling Activists 'Terrorists'

**原文链接**: [https://www.forbes.com/sites/thomasbrewster/2026/07/17/flock-ceo-sorry-for-labelling-activists-terrorists/](https://www.forbes.com/sites/thomasbrewster/2026/07/17/flock-ceo-sorry-for-labelling-activists-terrorists/)

生成摘要时出错

---

## 71. VulnHunter: Capital One's agentic AI code security tool

**原文标题**: VulnHunter: Capital One's agentic AI code security tool

**原文链接**: [https://www.capitalone.com/tech/open-source/announcing-vulnhunter/](https://www.capitalone.com/tech/open-source/announcing-vulnhunter/)

生成摘要时出错

---

## 72. M 3.9 Experimental Explosion – 147 Km ENE of Ponce Inlet, Florida

**原文标题**: M 3.9 Experimental Explosion – 147 Km ENE of Ponce Inlet, Florida

**原文链接**: [https://earthquake.usgs.gov/earthquakes/eventpage/us7000t13l/executive](https://earthquake.usgs.gov/earthquakes/eventpage/us7000t13l/executive)

生成摘要时出错

---

## 73. Canada says bridge tolls won't be split with U.S. until $6.4B of debt is repaid

**原文标题**: Canada says bridge tolls won't be split with U.S. until $6.4B of debt is repaid

**原文链接**: [https://www.cbc.ca/news/canada/windsor/carney-presser-gord-bridge-9.7272695](https://www.cbc.ca/news/canada/windsor/carney-presser-gord-bridge-9.7272695)

生成摘要时出错

---

## 74. SpaceX stock drops to a new low and loses $1T in value in a month

**原文标题**: SpaceX stock drops to a new low and loses $1T in value in a month

**原文链接**: [https://www.businessinsider.com/spacex-stock-drops-new-low-ipo-price-starship-launch-scrubbed-2026-7](https://www.businessinsider.com/spacex-stock-drops-new-low-ipo-price-starship-launch-scrubbed-2026-7)

生成摘要时出错

---

## 75. Fake food delivery site for the dopamine

**原文标题**: Fake food delivery site for the dopamine

**原文链接**: [https://old.reddit.com/r/BingeEatingDisorder/comments/1uzr3ui/fake_food_delivery_site_for_the_dopamine/](https://old.reddit.com/r/BingeEatingDisorder/comments/1uzr3ui/fake_food_delivery_site_for_the_dopamine/)

生成摘要时出错

---

## 76. CO2 overload, detected in human blood, suggests toxic atmosphere within 50 years

**原文标题**: CO2 overload, detected in human blood, suggests toxic atmosphere within 50 years

**原文链接**: [https://link.springer.com/article/10.1007/s11869-026-01918-5](https://link.springer.com/article/10.1007/s11869-026-01918-5)

生成摘要时出错

---

## 77. Designing emoji for the way we communicate today

**原文标题**: Designing emoji for the way we communicate today

**原文链接**: [https://blog.google/products-and-platforms/platforms/android/world-emoji-day-noto-3d/](https://blog.google/products-and-platforms/platforms/android/world-emoji-day-noto-3d/)

生成摘要时出错

---

## 78. Qubes OS Security in the Public Record

**原文标题**: Qubes OS Security in the Public Record

**原文链接**: [https://arxiv.org/abs/2607.14587](https://arxiv.org/abs/2607.14587)

生成摘要时出错

---

## 79. Everybody's Weirded Out by AI–Except the People Who Foist It on Us

**原文标题**: Everybody's Weirded Out by AI–Except the People Who Foist It on Us

**原文链接**: [https://newrepublic.com/article/213004/everybody-weirded-ai-except-people-foist-us](https://newrepublic.com/article/213004/everybody-weirded-ai-except-people-foist-us)

生成摘要时出错

---

## 80. Moonstone: Modern, cross-platform Lua runtime and package manager written in Zig

**原文标题**: Moonstone: Modern, cross-platform Lua runtime and package manager written in Zig

**原文链接**: [https://moonstone.sh/](https://moonstone.sh/)

生成摘要时出错

---

## 81. Mac gaming is finally getting the overpowered upgrade it deserves

**原文标题**: Mac gaming is finally getting the overpowered upgrade it deserves

**原文链接**: [https://www.macworld.com/article/3189951/apples-latest-game-porting-toolkit-beta-changed-how-i-think-about-mac-gaming.html](https://www.macworld.com/article/3189951/apples-latest-game-porting-toolkit-beta-changed-how-i-think-about-mac-gaming.html)

生成摘要时出错

---

## 82. Ring-Zero: Scaling Zero RL to a Trillion Parameters for Emergent Reasoning

**原文标题**: Ring-Zero: Scaling Zero RL to a Trillion Parameters for Emergent Reasoning

**原文链接**: [https://arxiv.org/abs/2607.12395](https://arxiv.org/abs/2607.12395)

生成摘要时出错

---

## 83. A grumpy screed about AI in software engineering

**原文标题**: A grumpy screed about AI in software engineering

**原文链接**: [https://sam.sutch.net/posts/a-grumpy-ai-screed](https://sam.sutch.net/posts/a-grumpy-ai-screed)

生成摘要时出错

---

## 84. Young adults are poor despite every metric which suggests otherwise

**原文标题**: Young adults are poor despite every metric which suggests otherwise

**原文链接**: [https://xcancel.com/i/article/2077113148524417439](https://xcancel.com/i/article/2077113148524417439)

生成摘要时出错

---

## 85. ICE Flight Monitor Interactive Dashboard

**原文标题**: ICE Flight Monitor Interactive Dashboard

**原文链接**: [https://www.humanrightsfirst.org/ice-flight-monitor-interactive-dashboard](https://www.humanrightsfirst.org/ice-flight-monitor-interactive-dashboard)

生成摘要时出错

---

## 86. Multi-Primary Color Display Emerges as Next-Gen Color Reproduction Technology

**原文标题**: Multi-Primary Color Display Emerges as Next-Gen Color Reproduction Technology

**原文链接**: [https://en.ubiresearchnet.com/multi-primary-color-display-technology-2026/](https://en.ubiresearchnet.com/multi-primary-color-display-technology-2026/)

生成摘要时出错

---

## 87. REO Trucks I4 4WD Pickup Truck Starts at $21,500

**原文标题**: REO Trucks I4 4WD Pickup Truck Starts at $21,500

**原文链接**: [https://reotrucks.com](https://reotrucks.com)

生成摘要时出错

---

## 88. In-toto: A framework to secure the integrity of software supply chains

**原文标题**: In-toto: A framework to secure the integrity of software supply chains

**原文链接**: [https://in-toto.io/](https://in-toto.io/)

生成摘要时出错

---

## 89. Flock Safety had a car journalist stalked, wrongly accused, and detained

**原文标题**: Flock Safety had a car journalist stalked, wrongly accused, and detained

**原文链接**: [https://www.thedrive.com/news/inside-the-flock-dragnet-how-systemic-errors-led-to-police-ambushing-me-for-no-reason](https://www.thedrive.com/news/inside-the-flock-dragnet-how-systemic-errors-led-to-police-ambushing-me-for-no-reason)

生成摘要时出错

---

## 90. US Corporate Insiders Are Selling Stocks at a Near Record Pace

**原文标题**: US Corporate Insiders Are Selling Stocks at a Near Record Pace

**原文链接**: [https://www.bloomberg.com/news/articles/2026-07-17/us-corporate-insiders-are-selling-stocks-at-a-near-record-pace](https://www.bloomberg.com/news/articles/2026-07-17/us-corporate-insiders-are-selling-stocks-at-a-near-record-pace)

生成摘要时出错

---

## 91. Google Kills Custom Search API on Jan 1, 2027

**原文标题**: Google Kills Custom Search API on Jan 1, 2027

**原文链接**: [https://thenextgennexus.com/2026/05/14/google-kills-custom-search-api-on-jan-1-2027-you-have-9-months/](https://thenextgennexus.com/2026/05/14/google-kills-custom-search-api-on-jan-1-2027-you-have-9-months/)

生成摘要时出错

---

## 92. Kimi K3 Intelligence, Performance and Price Analysis

**原文标题**: Kimi K3 Intelligence, Performance and Price Analysis

**原文链接**: [https://artificialanalysis.ai/models/kimi-k3](https://artificialanalysis.ai/models/kimi-k3)

生成摘要时出错

---

## 93. Pushinka

**原文标题**: Pushinka

**原文链接**: [https://en.wikipedia.org/wiki/Pushinka](https://en.wikipedia.org/wiki/Pushinka)

生成摘要时出错

---

## 94. No link between acetaminophen use during pregnancy and adverse birth outcomes

**原文标题**: No link between acetaminophen use during pregnancy and adverse birth outcomes

**原文链接**: [https://sph.unc.edu/sph-news/no-link-between-acetaminophen-use-during-pregnancy-and-adverse-birth-outcomes-study-finds/](https://sph.unc.edu/sph-news/no-link-between-acetaminophen-use-during-pregnancy-and-adverse-birth-outcomes-study-finds/)

生成摘要时出错

---

## 95. Tech note: making your own V-I plots at home

**原文标题**: Tech note: making your own V-I plots at home

**原文链接**: [https://lcamtuf.substack.com/p/tech-note-making-your-own-v-i-plots](https://lcamtuf.substack.com/p/tech-note-making-your-own-v-i-plots)

生成摘要时出错

---

## 96. Cops Use Flock to Track People, Not Cars

**原文标题**: Cops Use Flock to Track People, Not Cars

**原文链接**: [https://www.404media.co/how-cops-use-flock-to-track-people-not-cars/](https://www.404media.co/how-cops-use-flock-to-track-people-not-cars/)

生成摘要时出错

---

## 97. A Year On: The DOGE Disaster

**原文标题**: A Year On: The DOGE Disaster

**原文链接**: [https://donmoynihan.substack.com/p/a-year-on-the-doge-disaster](https://donmoynihan.substack.com/p/a-year-on-the-doge-disaster)

生成摘要时出错

---

## 98. Battery packs: Let's talk about crates, baby

**原文标题**: Battery packs: Let's talk about crates, baby

**原文链接**: [https://smallcultfollowing.com/babysteps/blog/2026/07/15/battery-packs/](https://smallcultfollowing.com/babysteps/blog/2026/07/15/battery-packs/)

生成摘要时出错

---

## 99. LG monitors installing adware on Windows PCs

**原文标题**: LG monitors installing adware on Windows PCs

**原文链接**: [https://www.techradar.com/televisions/lgs-gaming-monitors-and-tvs-are-facing-a-user-revolt](https://www.techradar.com/televisions/lgs-gaming-monitors-and-tvs-are-facing-a-user-revolt)

生成摘要时出错

---

## 100. PennyLane is an open-source quantum software platform for quantum

**原文标题**: PennyLane is an open-source quantum software platform for quantum

**原文链接**: [https://github.com/PennyLaneAI/pennylane](https://github.com/PennyLaneAI/pennylane)

生成摘要时出错

---

