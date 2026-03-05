# Hacker News 热门文章摘要 (2026-03-05)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. MacBook 尼奥

**原文标题**: MacBook Neo

**原文链接**: [https://www.apple.com/newsroom/2026/03/say-hello-to-macbook-neo/](https://www.apple.com/newsroom/2026/03/say-hello-to-macbook-neo/)

苹果宣布推出 MacBook Neo，这是一款全新笔记本电脑，旨在让更多用户体验 Mac，将于2026年3月4日上市。其售价突破性地定在599美元（教育优惠价499美元），旨在吸引学生、家庭用户和新的 Mac 用户。

MacBook Neo 采用耐用轻巧的铝金属设计，提供腮红、靛蓝、银色和柑橘四种鲜艳配色。它配备绚丽的13英寸 Liquid Retina 显示屏，拥有高分辨率、500尼特亮度并支持10亿色彩，辅以抗反射涂层。

搭载 A18 Pro 苹果芯片，这款笔记本电脑提供卓越性能，日常任务如网页浏览速度提升高达50%，相比最畅销的英特尔酷睿 Ultra 5 PC，设备端 AI 工作负载速度快达3倍。它还包含一个5核 GPU 和一个16核神经网络引擎，支持 Apple Intelligence 功能，所有这些都集成在无风扇设计中，实现静音运行。

用户单次充电可获得长达16小时的电池续航。Neo 集成1080p FaceTime 高清摄像头、支持定向波束成形的双麦克风，以及带空间音频的双侧出式扬声器。它配备苹果妙控键盘和宽大的多点触控触控板，部分型号支持触控 ID。

运行 macOS Tahoe 系统，MacBook Neo 提供与 iPhone 的无缝集成和强大的内置应用。连接方面包括两个 USB-C 端口、一个耳机插孔、Wi-Fi 6E 和蓝牙6。环保方面，它是苹果碳排放最低的 MacBook，采用60%的回收材料，其中包含90%的回收铝。即日起接受预订，3月11日（星期三）开始发售。

---

## 2. 摩托罗拉 GrapheneOS 设备将支持引导加载程序解锁/重锁。

**原文标题**: Motorola GrapheneOS devices will be bootloader unlockable/relockable

**原文链接**: [https://grapheneos.social/@GrapheneOS/116160393783585567](https://grapheneos.social/@GrapheneOS/116160393783585567)

GrapheneOS宣布了针对摩托罗拉设备用户的一项重要进展。该操作系统通过其Mastodon账户证实，即将推出的、旨在与GrapheneOS配合使用的摩托罗拉设备将同时配备可解锁和可重锁的引导加载程序。此功能对于增强设备安全性至关重要，因为它允许用户在刷入GrapheneOS的同时，仍能保持验证启动功能，而这正是防止操作系统被篡改的核心安全特性。该声明源自GrapheneOS官方Mastodon账户，表明摩托罗拉硬件将直接支持此功能。此举预计将提高GrapheneOS在摩托罗拉设备上的采用率和安全态势。

---

## 3. 没人能因简单而晋升。

**原文标题**: Nobody gets promoted for simplicity

**原文链接**: [https://terriblesoftware.org/2026/03/03/nobody-gets-promoted-for-simplicity/](https://terriblesoftware.org/2026/03/03/nobody-gets-promoted-for-simplicity/)

文章指出，工程中的简洁性往往被低估且得不到应有的奖励，导致了复杂性无意中滋生的文化。文章通过两位工程师的例子来说明这一点：工程师A快速交付了一个简洁有效的解决方案，但其工作却难以构成有力的晋升理由。然而，工程师B却过度设计了一个解决方案，引入了不必要的抽象，耗时更长，却为职业发展创造了一个“令人印象深刻”的故事。

这个问题渗透在整个工程生态系统中。在面试中，应聘者了解到，复杂、可扩展的设计比简洁、实用的设计更令人印象深刻。在设计评审中，工程师面临着“面向未来”的压力，为那些可能永远不会出现的问题添加层层抽象。作者强调，真正的资深之处在于懂得何时*不*使用复杂的工具，区分*必要复杂性*（确有必要时）和*非必要复杂性*（为推测的未来需求而过度设计）。

为了应对此问题，文章为工程师和领导者提供了策略。工程师应该通过记录避免复杂性背后的判断和决策、在设计评审中审慎地提出异议，以及与经理讨论如何构建叙事框架，来凸显其简洁工作的价值。领导者必须通过在设计评审和晋升材料中质疑不必要的复杂性、积极帮助工程师阐明简洁解决方案的价值，以及公开表彰简化行为和避免非必要复杂性的做法来主动改变激励机制。最终，使激励机制与真正重视简洁性保持一致，对于培养更健康的工程文化至关重要。

---

## 4. Google Workspace 命令行界面

**原文标题**: Google Workspace CLI

**原文链接**: [https://github.com/googleworkspace/cli](https://github.com/googleworkspace/cli)

Google Workspace CLI (`gws`) 为所有 Google Workspace API（包括 Drive、Gmail 和 Calendar）提供了一个统一的命令行界面。它专为人机交互和 AI 代理设计，提供零样板代码、结构化 JSON 输出，并从 Google 的 Discovery Service 动态构建其命令表面，自动反映 API 更新。

通过 `npm install -g @googleworkspace/cli` 进行安装非常直接，需要 Node.js 18+ 和一个用于 OAuth 的 Google Cloud 项目。对于人类用户，`gws` 简化了与 `--help`、`--dry-run` 和自动分页等功能的交互。对于 AI 代理，它提供结构化 JSON 响应和超过 100 个预构建的“代理技能”，用于无缝的 Workspace 管理，并集成了 OpenClaw 和 Gemini CLI。

身份验证支持多种工作流程：`gws auth setup`（通过 gcloud）、手动 OAuth、环境变量、服务帐号以及多帐号管理，并在静态存储时加密凭据。高级功能包括分段上传、流式分页结果和用于响应清理的 Model Armor 集成。一个 `gws mcp` 服务器可以将 Workspace API 作为结构化工具暴露给 MCP 兼容客户端。该项目正在积极开发中，但重要的是，它并非 Google 官方支持的产品。

---

## 5. Qwen之地风起云涌

**原文标题**: Something is afoot in the land of Qwen

**原文链接**: [https://simonwillison.net/2026/Mar/4/qwen/](https://simonwillison.net/2026/Mar/4/qwen/)

2026年3月4日，阿里巴巴通义AI团队遭遇重大变动，其核心研究员林俊扬高调辞职。作为推动阿里巴巴开源AI模型发展的关键人物，林俊扬在“卓越”的通义3.5模型家族发布后不久，便宣布了离职。

据报道，此举引发了其他多名通义核心成员的辞职，其中包括惠彬源（通义代码开发负责人）、俞博文（通义后训练研究负责人）和李凯欣（通义3.5/VL/Coder核心贡献者），以及许多年轻研究员。这些离职的未经证实的原因是，有传闻称一次组织架构调整，据称将一位来自谷歌Gemini团队的新研究员任命为通义的负责人。

阿里巴巴集团CEO吴泳铭迅速召集了一场“紧急全员大会”以应对这场危机，突显了公司对人才流失的担忧。尽管林俊扬的最终计划尚不明确，但他向团队发布了一则消息，鼓励他们“按原计划继续”。

作者对这种潜在的解散感到惋惜，强调通义在开发高质量、高效的开源模型方面取得了令人瞩目的成就，最近的通义3.5系列因其在各种尺寸（包括一个微小的2B多模态模型）下的有效性而备受赞扬。目前局势被描述为高度不确定，通义团队及其离职人才的未来仍悬而未决。

---

## 6. 达里奥·阿莫迪称OpenAI关于军事交易的说法“彻头彻尾是谎言”。

**原文标题**: Dario Amodei calls OpenAI’s messaging around military deal ‘straight up lies’

**原文链接**: [https://techcrunch.com/2026/03/04/anthropic-ceo-dario-amodei-calls-openais-messaging-around-military-deal-straight-up-lies-report-says/](https://techcrunch.com/2026/03/04/anthropic-ceo-dario-amodei-calls-openais-messaging-around-military-deal-straight-up-lies-report-says/)

Anthropic首席执行官达里奥·阿莫迪（Dario Amodei）指责OpenAI与美国国防部（DoD）的交易是“彻头彻尾的谎言”和“安全作秀”。阿莫迪的批评源于Anthropic最近拒绝向国防部授予其人工智能的无限制访问权限，尽管该公司已有一份价值2亿美元的军事合同，但仍坚持要求明确保障措施，以防止国内大规模监控和自主武器。

相比之下，OpenAI与国防部达成了一项协议，其首席执行官萨姆·奥特曼（Sam Altman）声称也获得了类似的保护。阿莫迪对此提出异议，称奥特曼是在虚假地将自己描绘成一个“和平缔造者”。核心分歧在于国防部的“任何合法用途”条款；Anthropic拒绝了该条款，而OpenAI声称其“所有合法目的”合同明确排除了大规模国内监控，据称国防部认为后者是非法的。然而，批评人士指出，“合法”的定义可能会改变。

阿莫迪认为Anthropic优先考虑防止滥用，而OpenAI则旨在安抚员工。公众情绪似乎偏向Anthropic，OpenAI与国防部的交易后，ChatGPT卸载量猛增295%就是证据。阿莫迪认为公众将Anthropic视为“英雄”，将OpenAI的交易视为“可疑”，并表达了对OpenAI叙事影响其自身员工的担忧。

---

## 7. 法官命令政府开始退还逾1300亿美元关税

**原文标题**: Judge orders government to begin refunding more than $130B in tariffs

**原文链接**: [https://www.wsj.com/politics/policy/judge-orders-government-to-begin-refunding-more-than-130-billion-in-tariffs-fdc1e62c](https://www.wsj.com/politics/policy/judge-orders-government-to-begin-refunding-more-than-130-billion-in-tariffs-fdc1e62c)

无法访问文章链接。

---

## 8. Building a new Flash

**原文标题**: Building a new Flash

**原文链接**: [https://bill.newgrounds.com/news/post/1607118](https://bill.newgrounds.com/news/post/1607118)

生成摘要时出错

---

## 9. Wikipedia in read-only mode following mass admin account compromise

**原文标题**: Wikipedia in read-only mode following mass admin account compromise

**原文链接**: [https://www.wikimediastatus.net](https://www.wikimediastatus.net)

生成摘要时出错

---

## 10. An interactive map of Flock Cams

**原文标题**: An interactive map of Flock Cams

**原文链接**: [https://deflock.org/map#map=5/37.125286/-96.284180](https://deflock.org/map#map=5/37.125286/-96.284180)

生成摘要时出错

---

## 11. LLM 中的 L 代表撒谎

**原文标题**: The L in "LLM" Stands for Lying

**原文链接**: [https://acko.net/blog/the-l-in-llm-stands-for-lying/](https://acko.net/blog/the-l-in-llm-stands-for-lying/)

生成摘要时出错

---

## 12. Agentic Engineering Patterns

**原文标题**: Agentic Engineering Patterns

**原文链接**: [https://simonwillison.net/guides/agentic-engineering-patterns/](https://simonwillison.net/guides/agentic-engineering-patterns/)

生成摘要时出错

---

## 13. Lenovo’s new ThinkPads score 10/10 for repairability

**原文标题**: Lenovo’s new ThinkPads score 10/10 for repairability

**原文链接**: [https://www.ifixit.com/News/115827/new-thinkpads-score-perfect-10-repairability](https://www.ifixit.com/News/115827/new-thinkpads-score-perfect-10-repairability)

生成摘要时出错

---

## 14. No right to relicense this project

**原文标题**: No right to relicense this project

**原文链接**: [https://github.com/chardet/chardet/issues/327](https://github.com/chardet/chardet/issues/327)

生成摘要时出错

---

## 15. TikTok will not introduce end-to-end encryption, saying it makes users less safe

**原文标题**: TikTok will not introduce end-to-end encryption, saying it makes users less safe

**原文链接**: [https://www.bbc.com/news/articles/cly2m5e5ke4o](https://www.bbc.com/news/articles/cly2m5e5ke4o)

生成摘要时出错

---

## 16. Qwen3.5 Fine-Tuning Guide

**原文标题**: Qwen3.5 Fine-Tuning Guide

**原文链接**: [https://unsloth.ai/docs/models/qwen3.5/fine-tune](https://unsloth.ai/docs/models/qwen3.5/fine-tune)

生成摘要时出错

---

## 17. Government grant-funded research should not be published in for-profit journals

**原文标题**: Government grant-funded research should not be published in for-profit journals

**原文链接**: [https://www.experimental-history.com/p/the-one-science-reform-we-can-all](https://www.experimental-history.com/p/the-one-science-reform-we-can-all)

生成摘要时出错

---

## 18. Relicensing with AI-Assisted Rewrite

**原文标题**: Relicensing with AI-Assisted Rewrite

**原文链接**: [https://tuananh.net/2026/03/05/relicensing-with-ai-assisted-rewrite/](https://tuananh.net/2026/03/05/relicensing-with-ai-assisted-rewrite/)

生成摘要时出错

---

## 19. Nvidia PersonaPlex 7B on Apple Silicon: Full-Duplex Speech-to-Speech in Swift

**原文标题**: Nvidia PersonaPlex 7B on Apple Silicon: Full-Duplex Speech-to-Speech in Swift

**原文链接**: [https://blog.ivan.digital/nvidia-personaplex-7b-on-apple-silicon-full-duplex-speech-to-speech-in-native-swift-with-mlx-0aa5276f2e23](https://blog.ivan.digital/nvidia-personaplex-7b-on-apple-silicon-full-duplex-speech-to-speech-in-native-swift-with-mlx-0aa5276f2e23)

生成摘要时出错

---

## 20. Making Firefox's right-click not suck with about:config

**原文标题**: Making Firefox's right-click not suck with about:config

**原文链接**: [https://joshua.hu/firefox-making-right-click-not-suck](https://joshua.hu/firefox-making-right-click-not-suck)

生成摘要时出错

---

## 21. Iran War Cost Tracker

**原文标题**: Iran War Cost Tracker

**原文链接**: [https://iran-cost-ticker.com](https://iran-cost-ticker.com)

生成摘要时出错

---

## 22. “It turns out” (2010)

**原文标题**: “It turns out” (2010)

**原文链接**: [https://jsomers.net/blog/it-turns-out](https://jsomers.net/blog/it-turns-out)

生成摘要时出错

---

## 23. Moss is a pixel canvas where every brush is a tiny program

**原文标题**: Moss is a pixel canvas where every brush is a tiny program

**原文链接**: [https://www.moss.town/](https://www.moss.town/)

生成摘要时出错

---

## 24. RFC 9849. TLS Encrypted Client Hello

**原文标题**: RFC 9849. TLS Encrypted Client Hello

**原文链接**: [https://www.rfc-editor.org/rfc/rfc9849.html](https://www.rfc-editor.org/rfc/rfc9849.html)

生成摘要时出错

---

## 25. Bet on German Train Delays

**原文标题**: Bet on German Train Delays

**原文链接**: [https://bahn.bet](https://bahn.bet)

生成摘要时出错

---

## 26. Voxile: A ray-traced game made in its own engine and programming language

**原文标题**: Voxile: A ray-traced game made in its own engine and programming language

**原文链接**: [https://elbowgreasegames.substack.com/p/voxray-games-pushes-major-update](https://elbowgreasegames.substack.com/p/voxray-games-pushes-major-update)

生成摘要时出错

---

## 27. A CPU that runs entirely on GPU

**原文标题**: A CPU that runs entirely on GPU

**原文链接**: [https://github.com/robertcprice/nCPU](https://github.com/robertcprice/nCPU)

生成摘要时出错

---

## 28. Don't make me talk to your chatbot

**原文标题**: Don't make me talk to your chatbot

**原文链接**: [https://raymyers.org/post/dont-make-me-talk-to-your-chatbot/](https://raymyers.org/post/dont-make-me-talk-to-your-chatbot/)

生成摘要时出错

---

## 29. Possible US Government iPhone-Hacking Toolkit in foreign spy and criminal hands

**原文标题**: Possible US Government iPhone-Hacking Toolkit in foreign spy and criminal hands

**原文链接**: [https://www.wired.com/story/coruna-iphone-hacking-toolkit-us-government/](https://www.wired.com/story/coruna-iphone-hacking-toolkit-us-government/)

生成摘要时出错

---

## 30. Nobody gets promoted for simplicity

**原文标题**: Nobody gets promoted for simplicity

**原文链接**: [https://terriblesoftware.org/2026/03/03/nobody-gets-promoted-for-simplicity/](https://terriblesoftware.org/2026/03/03/nobody-gets-promoted-for-simplicity/)

生成摘要时出错

---

## 31. Good software knows when to stop

**原文标题**: Good software knows when to stop

**原文链接**: [https://ogirardot.writizzy.com/p/good-software-knows-when-to-stop](https://ogirardot.writizzy.com/p/good-software-knows-when-to-stop)

生成摘要时出错

---

## 32. Glaze by Raycast

**原文标题**: Glaze by Raycast

**原文链接**: [https://www.glazeapp.com/](https://www.glazeapp.com/)

生成摘要时出错

---

## 33. Does that use a lot of energy?

**原文标题**: Does that use a lot of energy?

**原文链接**: [https://hannahritchie.github.io/energy-use-comparisons/](https://hannahritchie.github.io/energy-use-comparisons/)

生成摘要时出错

---

## 34. Google Safe Browsing missed 84% of confirmed phishing sites

**原文标题**: Google Safe Browsing missed 84% of confirmed phishing sites

**原文链接**: [https://www.norn-labs.com/blog/huginn-report-feb-2026](https://www.norn-labs.com/blog/huginn-report-feb-2026)

生成摘要时出错

---

## 35. You Just Reveived

**原文标题**: You Just Reveived

**原文链接**: [https://dylan.gr/1772520728](https://dylan.gr/1772520728)

生成摘要时出错

---

## 36. Google ends its 30 percent app store fee and welcomes third-party app stores

**原文标题**: Google ends its 30 percent app store fee and welcomes third-party app stores

**原文链接**: [https://www.engadget.com/apps/google-ends-its-30-percent-app-store-fee-and-welcomes-third-party-app-stores-185248647.html](https://www.engadget.com/apps/google-ends-its-30-percent-app-store-fee-and-welcomes-third-party-app-stores-185248647.html)

生成摘要时出错

---

## 37. BMW Group to deploy humanoid robots in production in Germany for the first time

**原文标题**: BMW Group to deploy humanoid robots in production in Germany for the first time

**原文链接**: [https://www.press.bmwgroup.com/global/article/detail/T0455864EN/bmw-group-to-deploy-humanoid-robots-in-production-in-germany-for-the-first-time?language=en](https://www.press.bmwgroup.com/global/article/detail/T0455864EN/bmw-group-to-deploy-humanoid-robots-in-production-in-germany-for-the-first-time?language=en)

生成摘要时出错

---

## 38. GitHub having issues [resolved]

**原文标题**: GitHub having issues [resolved]

**原文链接**: [https://www.githubstatus.com/incidents/n07yy1bk6kc4](https://www.githubstatus.com/incidents/n07yy1bk6kc4)

生成摘要时出错

---

## 39. Jensen Huang says Nvidia is pulling back from OpenAI and Anthropic

**原文标题**: Jensen Huang says Nvidia is pulling back from OpenAI and Anthropic

**原文链接**: [https://techcrunch.com/2026/03/04/jensen-huang-says-nvidia-is-pulling-back-from-openai-and-anthropic-but-his-explanation-raises-more-questions-than-it-answers/](https://techcrunch.com/2026/03/04/jensen-huang-says-nvidia-is-pulling-back-from-openai-and-anthropic-but-his-explanation-raises-more-questions-than-it-answers/)

生成摘要时出错

---

## 40. GPT-5.4

**原文标题**: GPT-5.4

**原文链接**: [https://openai.com/index/introducing-gpt-5-4/](https://openai.com/index/introducing-gpt-5-4/)

生成摘要时出错

---

## 41. My spicy take on vibe coding for PMs

**原文标题**: My spicy take on vibe coding for PMs

**原文链接**: [https://www.ddmckinnon.com/2026/02/11/my-%f0%9f%8c%b6-take-on-vibe-coding-for-pms/](https://www.ddmckinnon.com/2026/02/11/my-%f0%9f%8c%b6-take-on-vibe-coding-for-pms/)

生成摘要时出错

---

## 42. Father claims Google's AI product fuelled son's delusional spiral

**原文标题**: Father claims Google's AI product fuelled son's delusional spiral

**原文链接**: [https://www.bbc.com/news/articles/czx44p99457o](https://www.bbc.com/news/articles/czx44p99457o)

生成摘要时出错

---

## 43. MacBook Neo

**原文标题**: MacBook Neo

**原文链接**: [https://www.apple.com/macbook-neo/](https://www.apple.com/macbook-neo/)

生成摘要时出错

---

## 44. Dulce et Decorum Est (1921)

**原文标题**: Dulce et Decorum Est (1921)

**原文链接**: [https://www.poetryfoundation.org/poems/46560/dulce-et-decorum-est](https://www.poetryfoundation.org/poems/46560/dulce-et-decorum-est)

生成摘要时出错

---

## 45. Graphics Programming Resources

**原文标题**: Graphics Programming Resources

**原文链接**: [https://develop--gpvm-website.netlify.app/resources/](https://develop--gpvm-website.netlify.app/resources/)

生成摘要时出错

---

## 46. Helsinki just went a full year without a single traffic death

**原文标题**: Helsinki just went a full year without a single traffic death

**原文链接**: [https://www.politico.eu/article/helsinki-no-traffic-death-roads-eu-accident-finland-driving-transport/](https://www.politico.eu/article/helsinki-no-traffic-death-roads-eu-accident-finland-driving-transport/)

生成摘要时出错

---

## 47. Noem Can't Explain Why She Hired 8-Day-Old Company for Ad Campaign

**原文标题**: Noem Can't Explain Why She Hired 8-Day-Old Company for Ad Campaign

**原文链接**: [https://newrepublic.com/post/207381/kristi-noem-explain-company-ad-campaign](https://newrepublic.com/post/207381/kristi-noem-explain-company-ad-campaign)

生成摘要时出错

---

## 48. Weave – A language aware merge algorithm based on entities

**原文标题**: Weave – A language aware merge algorithm based on entities

**原文链接**: [https://github.com/Ataraxy-Labs/weave](https://github.com/Ataraxy-Labs/weave)

生成摘要时出错

---

## 49. NanoGPT Slowrun: Language Modeling with Limited Data, Infinite Compute

**原文标题**: NanoGPT Slowrun: Language Modeling with Limited Data, Infinite Compute

**原文链接**: [https://qlabs.sh/slowrun](https://qlabs.sh/slowrun)

生成摘要时出错

---

## 50. Emails to Outlook.com rejected due to a fault or overzealous blocking rules

**原文标题**: Emails to Outlook.com rejected due to a fault or overzealous blocking rules

**原文链接**: [https://www.theregister.com/2026/03/04/users_fume_at_outlookcom_email/](https://www.theregister.com/2026/03/04/users_fume_at_outlookcom_email/)

生成摘要时出错

---

## 51. Medical journal says the case reports it has published for 25 years are fiction

**原文标题**: Medical journal says the case reports it has published for 25 years are fiction

**原文链接**: [https://retractionwatch.com/2026/03/03/canadian-pediatric-society-journal-correction-case-reports-fictional-paediatrics-child-health/](https://retractionwatch.com/2026/03/03/canadian-pediatric-society-journal-correction-case-reports-fictional-paediatrics-child-health/)

生成摘要时出错

---

## 52. An Interactive Intro to CRDTs (2023)

**原文标题**: An Interactive Intro to CRDTs (2023)

**原文链接**: [https://jakelazaroff.com/words/an-interactive-intro-to-crdts/](https://jakelazaroff.com/words/an-interactive-intro-to-crdts/)

生成摘要时出错

---

## 53. Show HN: Jido 2.0, Elixir Agent Framework

**原文标题**: Show HN: Jido 2.0, Elixir Agent Framework

**原文链接**: [https://jido.run/blog/jido-2-0-is-here](https://jido.run/blog/jido-2-0-is-here)

生成摘要时出错

---

## 54. Poor Man's Polaroid

**原文标题**: Poor Man's Polaroid

**原文链接**: [https://boxart.lt/blog/poor_mans_polaroid](https://boxart.lt/blog/poor_mans_polaroid)

生成摘要时出错

---

## 55. Show HN: Poppy – A simple app to stay intentional with relationships

**原文标题**: Show HN: Poppy – A simple app to stay intentional with relationships

**原文链接**: [https://poppy-connection-keeper.netlify.app/](https://poppy-connection-keeper.netlify.app/)

生成摘要时出错

---

## 56. Cancel ChatGPT AI boycott surges after OpenAI pentagon military deal

**原文标题**: Cancel ChatGPT AI boycott surges after OpenAI pentagon military deal

**原文链接**: [https://www.euronews.com/next/2026/03/02/cancel-chatgpt-ai-boycott-surges-after-openai-pentagon-military-deal](https://www.euronews.com/next/2026/03/02/cancel-chatgpt-ai-boycott-surges-after-openai-pentagon-military-deal)

生成摘要时出错

---

## 57. The Government Uses Targeted Advertising to Track Your Location

**原文标题**: The Government Uses Targeted Advertising to Track Your Location

**原文链接**: [https://www.eff.org/deeplinks/2026/03/targeted-advertising-gives-your-location-government-just-ask-cbp](https://www.eff.org/deeplinks/2026/03/targeted-advertising-gives-your-location-government-just-ask-cbp)

生成摘要时出错

---

## 58. US tech firms pledge at White House to bear costs of energy for datacenters

**原文标题**: US tech firms pledge at White House to bear costs of energy for datacenters

**原文链接**: [https://www.theguardian.com/us-news/2026/mar/04/us-tech-companies-energy-cost-pledge-white-house](https://www.theguardian.com/us-news/2026/mar/04/us-tech-companies-energy-cost-pledge-white-house)

生成摘要时出错

---

## 59. A GitHub Issue Title Compromised 4k Developer Machines

**原文标题**: A GitHub Issue Title Compromised 4k Developer Machines

**原文链接**: [https://grith.ai/blog/clinejection-when-your-ai-tool-installs-another](https://grith.ai/blog/clinejection-when-your-ai-tool-installs-another)

生成摘要时出错

---

## 60. GPT-5.4

**原文标题**: GPT-5.4

**原文链接**: [https://openai.com/index/introducing-gpt-5-4/](https://openai.com/index/introducing-gpt-5-4/)

生成摘要时出错

---

## 61. MyFirst Kids Watch Hacked. Access to Camera and Microphone

**原文标题**: MyFirst Kids Watch Hacked. Access to Camera and Microphone

**原文链接**: [https://www.kth.se/en/om/nyheter/centrala-nyheter/kth-studenten-hackade-klocka-for-barn-1.1461249](https://www.kth.se/en/om/nyheter/centrala-nyheter/kth-studenten-hackade-klocka-for-barn-1.1461249)

生成摘要时出错

---

## 62. Better JIT for Postgres

**原文标题**: Better JIT for Postgres

**原文链接**: [https://github.com/vladich/pg_jitter](https://github.com/vladich/pg_jitter)

生成摘要时出错

---

## 63. Humans 40k yrs ago developed a system of conventional signs

**原文标题**: Humans 40k yrs ago developed a system of conventional signs

**原文链接**: [https://www.pnas.org/doi/10.1073/pnas.2520385123](https://www.pnas.org/doi/10.1073/pnas.2520385123)

生成摘要时出错

---

## 64. You need to rewrite your CLI for AI agents

**原文标题**: You need to rewrite your CLI for AI agents

**原文链接**: [https://justin.poehnelt.com/posts/rewrite-your-cli-for-ai-agents/](https://justin.poehnelt.com/posts/rewrite-your-cli-for-ai-agents/)

生成摘要时出错

---

## 65. We've freed Cookie's Bustle from copyright hell

**原文标题**: We've freed Cookie's Bustle from copyright hell

**原文链接**: [https://gamehistory.org/cookies-bustle/](https://gamehistory.org/cookies-bustle/)

生成摘要时出错

---

## 66. Did Alibaba just kneecap its powerful Qwen AI team?

**原文标题**: Did Alibaba just kneecap its powerful Qwen AI team?

**原文链接**: [https://venturebeat.com/technology/did-alibaba-just-kneecap-its-powerful-qwen-ai-team-key-figures-depart-in](https://venturebeat.com/technology/did-alibaba-just-kneecap-its-powerful-qwen-ai-team-key-figures-depart-in)

生成摘要时出错

---

## 67. NRC issues first commercial reactor construction approval in 10 years [pdf]

**原文标题**: NRC issues first commercial reactor construction approval in 10 years [pdf]

**原文链接**: [https://www.nrc.gov/sites/default/files/cdn/doc-collection-news/2026/26-028.pdf](https://www.nrc.gov/sites/default/files/cdn/doc-collection-news/2026/26-028.pdf)

生成摘要时出错

---

## 68. The View from RSS

**原文标题**: The View from RSS

**原文链接**: [https://www.carolinecrampton.com/the-view-from-rss/](https://www.carolinecrampton.com/the-view-from-rss/)

生成摘要时出错

---

## 69. Smalltalk's Browser: Unbeatable, yet Not Enough

**原文标题**: Smalltalk's Browser: Unbeatable, yet Not Enough

**原文链接**: [https://blog.lorenzano.eu/smalltalks-browser-unbeatable-yet-not-enough/](https://blog.lorenzano.eu/smalltalks-browser-unbeatable-yet-not-enough/)

生成摘要时出错

---

## 70. Chaos and Dystopian news for the dead internet survivors

**原文标题**: Chaos and Dystopian news for the dead internet survivors

**原文链接**: [https://www.fubardaily.com](https://www.fubardaily.com)

生成摘要时出错

---

## 71. California's Digital Age Assurance Act, and FOSS

**原文标题**: California's Digital Age Assurance Act, and FOSS

**原文链接**: [https://runxiyu.org/comp/ab1043/](https://runxiyu.org/comp/ab1043/)

生成摘要时出错

---

## 72. To understand our fascination with crystals, researchers gave some to chimps

**原文标题**: To understand our fascination with crystals, researchers gave some to chimps

**原文链接**: [https://www.nytimes.com/2026/03/04/science/chimpanzees-crystals.html](https://www.nytimes.com/2026/03/04/science/chimpanzees-crystals.html)

生成摘要时出错

---

## 73. Rising carbon dioxide levels now detected in human blood

**原文标题**: Rising carbon dioxide levels now detected in human blood

**原文链接**: [https://phys.org/news/2026-02-carbon-dioxide-human-blood.html](https://phys.org/news/2026-02-carbon-dioxide-human-blood.html)

生成摘要时出错

---

## 74. Sea level much higher than assumed in most coastal hazard assessments

**原文标题**: Sea level much higher than assumed in most coastal hazard assessments

**原文链接**: [https://www.nature.com/articles/s41586-026-10196-1](https://www.nature.com/articles/s41586-026-10196-1)

生成摘要时出错

---

## 75. Iran war wreaking havoc on shipping and air cargo, could create global delays

**原文标题**: Iran war wreaking havoc on shipping and air cargo, could create global delays

**原文链接**: [https://www.theregister.com/2026/03/02/iran_war_tech_supply_chain/](https://www.theregister.com/2026/03/02/iran_war_tech_supply_chain/)

生成摘要时出错

---

## 76. Was Windows 1.0's lack of overlapping windows a legal or a technical matter?

**原文标题**: Was Windows 1.0's lack of overlapping windows a legal or a technical matter?

**原文链接**: [https://retrocomputing.stackexchange.com/questions/32511/was-windows-1-0s-lack-of-overlapping-windows-a-legal-or-a-technical-matter](https://retrocomputing.stackexchange.com/questions/32511/was-windows-1-0s-lack-of-overlapping-windows-a-legal-or-a-technical-matter)

生成摘要时出错

---

## 77. Show HN: P0 – Yes, AI can ship complex features into real codebases

**原文标题**: Show HN: P0 – Yes, AI can ship complex features into real codebases

**原文链接**: [https://www.bepurple.ai/](https://www.bepurple.ai/)

生成摘要时出错

---

## 78. GPT-5.4 Thinking and GPT-5.4 Pro

**原文标题**: GPT-5.4 Thinking and GPT-5.4 Pro

**原文链接**: [https://twitter.com/i/status/2029620619743219811](https://twitter.com/i/status/2029620619743219811)

生成摘要时出错

---

## 79. The Self-Help Trap: What 20 Years of "Optimizing" Has Taught Me

**原文标题**: The Self-Help Trap: What 20 Years of "Optimizing" Has Taught Me

**原文链接**: [https://tim.blog/2026/03/04/the-self-help-trap/](https://tim.blog/2026/03/04/the-self-help-trap/)

生成摘要时出错

---

## 80. LLMs can unmask pseudonymous users at scale with surprising accuracy

**原文标题**: LLMs can unmask pseudonymous users at scale with surprising accuracy

**原文链接**: [https://arstechnica.com/security/2026/03/llms-can-unmask-pseudonymous-users-at-scale-with-surprising-accuracy/](https://arstechnica.com/security/2026/03/llms-can-unmask-pseudonymous-users-at-scale-with-surprising-accuracy/)

生成摘要时出错

---

## 81. Jails for NetBSD – Kernel Enforced Isolation and Native Resource Control

**原文标题**: Jails for NetBSD – Kernel Enforced Isolation and Native Resource Control

**原文链接**: [https://netbsd-jails.petermann-digital.de/](https://netbsd-jails.petermann-digital.de/)

生成摘要时出错

---

## 82. Data Has Weight but Only on SSDs

**原文标题**: Data Has Weight but Only on SSDs

**原文链接**: [https://cubiclenate.com/2026/03/04/data-has-weight-but-only-on-ssds-blathering/](https://cubiclenate.com/2026/03/04/data-has-weight-but-only-on-ssds-blathering/)

生成摘要时出错

---

## 83. 10% of Firefox crashes are caused by bitflips

**原文标题**: 10% of Firefox crashes are caused by bitflips

**原文链接**: [https://mas.to/@gabrielesvelto/116171750653898304](https://mas.to/@gabrielesvelto/116171750653898304)

生成摘要时出错

---

## 84. OpenAI CEO Sam Altman Defends Pentagon Work to Staff

**原文标题**: OpenAI CEO Sam Altman Defends Pentagon Work to Staff

**原文链接**: [https://www.wsj.com/tech/ai/openai-ceo-altman-defends-pentagon-work-to-staff-calls-backlash-really-painful-76d769ec](https://www.wsj.com/tech/ai/openai-ceo-altman-defends-pentagon-work-to-staff-calls-backlash-really-painful-76d769ec)

生成摘要时出错

---

## 85. US asked Ukraine for help fighting Iranian drones, Zelensky says

**原文标题**: US asked Ukraine for help fighting Iranian drones, Zelensky says

**原文链接**: [https://www.bbc.com/news/articles/cr5llg0e9g9o](https://www.bbc.com/news/articles/cr5llg0e9g9o)

生成摘要时出错

---

## 86. Apple Announces Low-Cost 'MacBook Neo' with A18 Pro Chip

**原文标题**: Apple Announces Low-Cost 'MacBook Neo' with A18 Pro Chip

**原文链接**: [https://www.macrumors.com/2026/03/04/apple-announces-low-cost-macbook-neo-with-a18-pro-chip/](https://www.macrumors.com/2026/03/04/apple-announces-low-cost-macbook-neo-with-a18-pro-chip/)

生成摘要时出错

---

## 87. Indefinite Book Club Hiatus

**原文标题**: Indefinite Book Club Hiatus

**原文链接**: [https://whatever.scalzi.com/2026/03/03/indefinite-book-club-hiatus/](https://whatever.scalzi.com/2026/03/03/indefinite-book-club-hiatus/)

生成摘要时出错

---

## 88. Fast-Servers

**原文标题**: Fast-Servers

**原文链接**: [https://geocar.sdf1.org/fast-servers.html](https://geocar.sdf1.org/fast-servers.html)

生成摘要时出错

---

## 89. 1.5 Million Users Leave ChatGPT

**原文标题**: 1.5 Million Users Leave ChatGPT

**原文链接**: [https://www.forbes.com/sites/barrycollins/2026/03/02/leaving-chatgpt-make-sure-to-do-this-before-you-cancel/](https://www.forbes.com/sites/barrycollins/2026/03/02/leaving-chatgpt-make-sure-to-do-this-before-you-cancel/)

生成摘要时出错

---

## 90. New York could prohibit chatbot medical, legal, engineering advice

**原文标题**: New York could prohibit chatbot medical, legal, engineering advice

**原文链接**: [https://folding-sky.com/blog/ny-senate-bill-s7263-chatbot-liability](https://folding-sky.com/blog/ny-senate-bill-s7263-chatbot-liability)

生成摘要时出错

---

## 91. You can't use a code editor when you're under 18 now?

**原文标题**: You can't use a code editor when you're under 18 now?

**原文链接**: [https://mastodon.online/@marekfort/116164253291515471](https://mastodon.online/@marekfort/116164253291515471)

生成摘要时出错

---

## 92. OpenBSD on SGI: A Rollercoaster Story

**原文标题**: OpenBSD on SGI: A Rollercoaster Story

**原文链接**: [http://miod.online.fr/software/openbsd/stories/sgiall.html](http://miod.online.fr/software/openbsd/stories/sgiall.html)

生成摘要时出错

---

## 93. Faster C software with Dynamic Feature Detection

**原文标题**: Faster C software with Dynamic Feature Detection

**原文链接**: [https://gist.github.com/jjl/d998164191af59a594500687a679b98d](https://gist.github.com/jjl/d998164191af59a594500687a679b98d)

生成摘要时出错

---

## 94. Who Writes the Bugs? A Deeper Look at 125,000 Kernel Vulnerabilities

**原文标题**: Who Writes the Bugs? A Deeper Look at 125,000 Kernel Vulnerabilities

**原文链接**: [https://pebblebed.com/blog/kernel-bugs-part2](https://pebblebed.com/blog/kernel-bugs-part2)

生成摘要时出错

---

## 95. What Python’s asyncio primitives get wrong about shared state

**原文标题**: What Python’s asyncio primitives get wrong about shared state

**原文链接**: [https://www.inngest.com/blog/no-lost-updates-python-asyncio](https://www.inngest.com/blog/no-lost-updates-python-asyncio)

生成摘要时出错

---

## 96. Palantir and other tech companies are stocking offices with tobacco products

**原文标题**: Palantir and other tech companies are stocking offices with tobacco products

**原文链接**: [https://fortune.com/2026/03/04/palantir-tech-companies-offices-vending-machines-tobacco-worker-productivity/](https://fortune.com/2026/03/04/palantir-tech-companies-offices-vending-machines-tobacco-worker-productivity/)

生成摘要时出错

---

## 97. The Brand Age

**原文标题**: The Brand Age

**原文链接**: [https://paulgraham.com/brandage.html](https://paulgraham.com/brandage.html)

生成摘要时出错

---

## 98. Welcome to the Wasteland: A Thousand Gas Towns

**原文标题**: Welcome to the Wasteland: A Thousand Gas Towns

**原文链接**: [https://steve-yegge.medium.com/welcome-to-the-wasteland-a-thousand-gas-towns-a5eb9bc8dc1f](https://steve-yegge.medium.com/welcome-to-the-wasteland-a-thousand-gas-towns-a5eb9bc8dc1f)

生成摘要时出错

---

## 99. Marcus AI Claims Dataset

**原文标题**: Marcus AI Claims Dataset

**原文链接**: [https://github.com/davegoldblatt/marcus-claims-dataset](https://github.com/davegoldblatt/marcus-claims-dataset)

生成摘要时出错

---

## 100. GPT 5.4 Thinking and Pro

**原文标题**: GPT 5.4 Thinking and Pro

**原文链接**: [https://twitter.com/OpenAI/status/2029620619743219811](https://twitter.com/OpenAI/status/2029620619743219811)

生成摘要时出错

---

