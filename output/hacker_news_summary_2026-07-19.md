# Hacker News 热门文章摘要 (2026-07-19)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. LG显示器通过 Windows 更新静默安装软件，未经同意。

**原文标题**: LG monitors silently install software through Windows Update without consent

**原文链接**: [https://videocardz.com/newz/lg-monitors-silently-install-software-through-windows-update-without-user-consent](https://videocardz.com/newz/lg-monitors-silently-install-software-through-windows-update-without-user-consent)

LG 显示器正在未经用户同意的情况下，通过 Windows Update 静默安装软件，主要推广 McAfee 订阅服务。Gamers Nexus 使用一台 LG UltraGear 34GX900A-B 重现了这种行为，观察到 Windows Update 首先安装了 LG 扩展和软件组件，随后是 LG 显示器应用安装程序。在 32 次系统启动测试中，该安装程序有 31 次显示了 McAfee 推广信息，提供 30 天试用；剩余的一次启动则推广了 LG 的一个实用工具。

这个问题并非仅限于新型显示器；Gamers Nexus 还在一台三年旧的 LG UltraFine 32UN880-B 上收到了弹窗，用户投诉至少可以追溯到 2024 年。所安装的应用程序会获得互联网访问权限和所有系统资源。

这种自动软件安装并非 LG 独有；戴尔也采用类似方法，通过 Windows Update 为兼容硬件分发 Alienware Command Center。

用户可以通过启用位于“计算机配置”、“管理模板”、“系统”和“设备安装”下的“阻止与设备元数据相关的应用程序自动下载”组策略设置来阻止这些不必要的安装。然而，这样做也会阻止其他可能实用的显示器或外围设备软件自动安装，需要用户手动下载。

---

## 2. 退行JPEGs

**原文标题**: Regressive JPEGs

**原文链接**: [https://maurycyz.com/projects/bad_jpeg/](https://maurycyz.com/projects/bad_jpeg/)

“倒退式JPEG”探索了JPEG文件的渐进式渲染特性，即图像通过多次“扫描”首先显示低分辨率组件。每次扫描定义了颜色通道（Y、Cb、Cr）的特定频谱范围（DCT量化区）和精度，从而实现细节的逐步增强。

作者尝试操纵这种结构，将多个不同的图像嵌入到单个JPEG中。最初的尝试是连接完整的JPEG文件并去除冗余标记。虽然这使得图像在部分下载时可以切换帧，但解码器通常将此限制在大约九次扫描，从而导致重影，因为后续的AC（高频）扫描会优化先前渲染的数据。

为了克服这些问题，作者设计了一种方法，为每个“帧” *仅* 使用DC（第0量化区）扫描。这创建了符合标准、低分辨率（1/16）的“帧”，且不包含AC数据，从而消除了重影，并显著增加了可渲染帧的数量——在Chrome中可达90帧。这有效地将一个短“视频”打包到单个JPEG中。

尽管由于依赖网络计时而缺乏实际应用，但这项技术为非常规的交互式内容或“rickrolls”提供了新颖的可能性，展示了对JPEG渐进式特性的一种创造性再利用。

---

## 3. 转录.cpp

**原文标题**: Transcribe.cpp

**原文链接**: [https://workshop.cjpais.com/projects/transcribe-cpp](https://workshop.cjpais.com/projects/transcribe-cpp)

transcribe.cpp 于2026年4月推出，是一个基于ggml的新转录库，旨在解决分发跨平台语音转文本应用时的痛点。该作者（Handy应用的维护者）创建transcribe.cpp，旨在为whisper.cpp和ONNX等现有解决方案提供一个可靠、高性能的替代品，因为这些现有方案在广泛分发和信任方面面临显著挑战。

这个v0.1.0库提供了一个快速准确的推理引擎，具有广泛的模型支持，目前涵盖16个ASR系列（60多个模型）并持续增长。它通过Vulkan、Metal、CUDA和TinyBLAS提供广泛的加速功能。准确性是其核心原则：每个受支持的模型都经过数值验证和WER测试，以匹配其参考实现，并且结果公开发布。

transcribe.cpp 被设计成 whisper.cpp 的近乎直接替代品，甚至可以运行现有的`.bin`文件，同时提供可比的性能。对于实际应用至关重要，它为Python、Javascript/Typescript、Rust和ObjC/Swift提供了维护者支持的语言绑定。该项目致力于使本地ASR更易于访问和高效，在各种设备上使用最先进的模型实现了超越实时的转录。

该项目感谢Mozilla AI（BiR项目）、ggml社区、Modal（用于WER测试）、Blacksmith（用于CI/CD）以及Hugging Face的大力支持。作者确认在引擎开发中使用了AI辅助，但项目公告本身并非由AI撰写。

---

## 4. 通义千问 3.8

**原文标题**: Qwen 3.8

**原文链接**: [https://twitter.com/Alibaba_Qwen/status/2078759124914098291](https://twitter.com/Alibaba_Qwen/status/2078759124914098291)

阿里巴巴通义千问即将推出参数规模达2.4万亿的巨型模型通义千问3.8，并很快将开源。开发者声称，它是目前最强大的模型之一，可与领先的前沿AI模型媲美，且仅次于Fable 5。用户现已可在阿里巴巴的Token Plan、Qoder和QoderWork平台上测试通义千问3.8-Max-预览版。该公告鼓励早期采用和创新，并提供了面向国际和中国用户的Token Plan链接。

---

## 5. GPT-5.6 used a prompt to close a 30-year gap in convex optimization

**原文标题**: GPT-5.6 used a prompt to close a 30-year gap in convex optimization

**原文链接**: [https://old.reddit.com/r/math/comments/1uxj3cy/after_openais_cdc_proof_announcement_gpt56_used_a/](https://old.reddit.com/r/math/comments/1uxj3cy/after_openais_cdc_proof_announcement_gpt56_used_a/)

生成摘要时出错

---

## 6. 淇幂 K3 时刻

**原文标题**: The Kimi K3 Moment

**原文链接**: [https://stephen.bochinski.dev/blog/2026/07/18/the-kimi-k3-moment/](https://stephen.bochinski.dev/blog/2026/07/18/the-kimi-k3-moment/)

作者发现，Kimi K3这一开放模型在编码任务上与Claude难分伯仲，其性能、输出质量和token消耗量都旗鼓相当。然而，Kimi K3明显更实惠，API成本仅为Claude的一小部分（每百万token $3/$15 对比 $10/$50），订阅计划也提供了更大的价值（$19/$39 对比 Claude严格按量计费的选项）。作者还指出Claude的不可靠性，例如其因经济不可持续性而从付费计划中移除了Fable访问权限，而Kimi的分级定价则避免了此问题。

文章接着批评美国人工智能政策是“彻头彻尾的失败”。它认为美国模型受到限制的阻碍，拒绝执行某些类型的工作，而Kimi K3和GLM 5.2等前沿质量模型（由中国实验室在宽松许可下发布）则公开可用，不受美国监管，并在基准测试中超越受限的美国模型。作者指出，这项政策只限制了美国客户。与Anthropic形成对比的是，OpenAI似乎更有效地应对了政府审查，在更便宜的计划中维持了一个可行的旗舰模型。

作者预测，美国政府未来将效仿其汽车行业的策略，通过补贴和关税来监管人工智能和开源。这将培养竞争力较弱的国内公私合营人工智能模型，并使美国用户无法以合理价格获取全球最佳模型。因此，作者认为没有理由继续为Claude付费。

---

## 7. 凯撒护士称AI、监控使其工作和患者护理恶化

**原文标题**: Kaiser nurses say AI, surveillance are making their jobs and patient care worse

**原文链接**: [https://localnewsmatters.org/2026/07/15/kaiser-nurses-say-ai-workplace-surveillance-are-making-their-jobs-and-patient-care-worse/](https://localnewsmatters.org/2026/07/15/kaiser-nurses-say-ai-workplace-surveillance-are-making-their-jobs-and-patient-care-worse/)

Kaiser Permanente nurses report that artificial intelligence and surveillance technologies are negatively impacting patient care and increasing workplace stress. They describe being criticized and receiving poor performance scores for spending over 15 minutes on calls, despite Kaiser's claim it doesn't use "Average Handle Time" metrics. Software monitors productivity and call speed, and AI has been used to assess empathy and tone of voice, which nurses found inaccurate and unhelpful.

Nurses, like Raquel Alvarez Sanchez, detail instances where critical patient needs—such as suicidal callers or patients receiving life-altering diagnoses—require extended conversations, forcing them to prioritize patient care over avoiding reprimands. This pressure, they contend, leads to withholding advice, rushing complex calls, and increased emotional exhaustion, potentially compromising patient safety. Many calls involving multiple symptoms, chronic illnesses, or interpreters routinely exceed the implied 15-minute limit, which nurses deem unsafe.

The California Nurses Association (CNA) is making AI a key issue in upcoming contract negotiations, following past protests. While Kaiser states its AI use prioritizes patient safety with human oversight, nurses feel harassed and unsupported. Experts note that such intense surveillance increases worker stress and burnout, which can lead to mistakes in high-stakes healthcare settings. Nurses emphasize that their role requires human judgment and compassion, not the rigid efficiency models often imposed by algorithmic management, fearing that the focus on cost-cutting over care will ultimately fail patients.

---

## 8. 纽约市可能要求房东和房地产经纪人在房源信息中披露人工智能的使用。

**原文标题**: NYC may require landlords and realtors to disclose the use of AI in listings

**原文链接**: [https://petapixel.com/2026/07/16/mayor-mamdani-says-landlords-cant-secretly-use-ai-images-to-advertise-properties/](https://petapixel.com/2026/07/16/mayor-mamdani-says-landlords-cant-secretly-use-ai-images-to-advertise-properties/)

生成摘要时出错

---

## 9. If You Build It, They Will Come

**原文标题**: If You Build It, They Will Come

**原文链接**: [https://www.benlandautaylor.com/p/if-you-build-it-they-will-come](https://www.benlandautaylor.com/p/if-you-build-it-they-will-come)

生成摘要时出错

---

## 10. Why do AI company logos look like buttholes? (2025)

**原文标题**: Why do AI company logos look like buttholes? (2025)

**原文链接**: [https://velvetshark.com/ai-company-logos-that-look-like-buttholes](https://velvetshark.com/ai-company-logos-that-look-like-buttholes)

生成摘要时出错

---

## 11. What AI did to stackoverflow in a graph

**原文标题**: What AI did to stackoverflow in a graph

**原文链接**: [https://data.stackexchange.com/stackoverflow/query/1953768#graph](https://data.stackexchange.com/stackoverflow/query/1953768#graph)

生成摘要时出错

---

## 12. AI Mania Is Eviscerating Global Decision-Making

**原文标题**: AI Mania Is Eviscerating Global Decision-Making

**原文链接**: [https://ludic.mataroa.blog/blog/ai-mania-is-eviscerating-global-decision-making/#fnref:3](https://ludic.mataroa.blog/blog/ai-mania-is-eviscerating-global-decision-making/#fnref:3)

生成摘要时出错

---

## 13. What I learned selling 2,500 MIDI recorders: Hardware is not so hard

**原文标题**: What I learned selling 2,500 MIDI recorders: Hardware is not so hard

**原文链接**: [https://chipweinberger.com/articles/20260719-hardware-is-not-so-hard](https://chipweinberger.com/articles/20260719-hardware-is-not-so-hard)

生成摘要时出错

---

## 14. Claude Code uses Bun written in Rust now

**原文标题**: Claude Code uses Bun written in Rust now

**原文链接**: [https://simonwillison.net/2026/Jul/19/claude-code-in-bun-in-rust/](https://simonwillison.net/2026/Jul/19/claude-code-in-bun-in-rust/)

生成摘要时出错

---

## 15. 欧盟对未售衣物和鞋类的销毁禁令开始适用

**原文标题**: EU ban on destruction of unsold clothes and shoes enters into application

**原文链接**: [https://environment.ec.europa.eu/news/ban-destruction-unsold-clothes-and-shoes-enters-application-2026-07-17_en](https://environment.ec.europa.eu/news/ban-destruction-unsold-clothes-and-shoes-enters-application-2026-07-17_en)

生成摘要时出错

---

## 16. Better and Cheaper Than IPTV

**原文标题**: Better and Cheaper Than IPTV

**原文链接**: [https://github.com/stupside/castor](https://github.com/stupside/castor)

生成摘要时出错

---

## 17. The Zilog Z80 has turned 50

**原文标题**: The Zilog Z80 has turned 50

**原文链接**: [https://goliath32.com/blog/z80.html](https://goliath32.com/blog/z80.html)

生成摘要时出错

---

## 18. Goodbye, and Thanks for All the Bikesheds

**原文标题**: Goodbye, and Thanks for All the Bikesheds

**原文链接**: [https://queue.acm.org/detail.cfm?id=3818307](https://queue.acm.org/detail.cfm?id=3818307)

生成摘要时出错

---

## 19. Codex Resets

**原文标题**: Codex Resets

**原文链接**: [https://codex-resets.com/](https://codex-resets.com/)

生成摘要时出错

---

## 20. OpenAI reduces Codex Model Context Size from 372k to 272k

**原文标题**: OpenAI reduces Codex Model Context Size from 372k to 272k

**原文链接**: [https://github.com/openai/codex/pull/33972/files](https://github.com/openai/codex/pull/33972/files)

生成摘要时出错

---

## 21. Fable 5 vs. GPT-5.6 Sol on an NP-Hard Problem: Does /goal help?

**原文标题**: Fable 5 vs. GPT-5.6 Sol on an NP-Hard Problem: Does /goal help?

**原文链接**: [https://charlesazam.com/blog/fable-5-gpt-5-6-sol-goal/](https://charlesazam.com/blog/fable-5-gpt-5-6-sol-goal/)

生成摘要时出错

---

## 22. Elixir-lang.org has a new design

**原文标题**: Elixir-lang.org has a new design

**原文链接**: [https://elixir-lang.org/](https://elixir-lang.org/)

生成摘要时出错

---

## 23. Gleam Is Now on Tangled

**原文标题**: Gleam Is Now on Tangled

**原文链接**: [https://tangled.org/gleam.run/gleam](https://tangled.org/gleam.run/gleam)

Gleam, a language designed for building type-safe and scalable systems, has launched on Tangled. The article emphasizes that Gleam is not corporately owned but relies on the generous support of its sponsors. Users who appreciate Gleam's benefits are encouraged to consider sponsoring the project or members of its core team to help ensure its continued development. The team expresses deep gratitude for all support.

---

## 24. Setting up your spare Mac for Claude Code to control, a step-by-step guide

**原文标题**: Setting up your spare Mac for Claude Code to control, a step-by-step guide

**原文链接**: [https://ykdojo.github.io/claude-controls-mac/](https://ykdojo.github.io/claude-controls-mac/)

生成摘要时出错

---

## 25. Hardcore IndieWeb: Run your own website 100% independently for only $0.01/day

**原文标题**: Hardcore IndieWeb: Run your own website 100% independently for only $0.01/day

**原文链接**: [https://www.neatnik.net/hardcore-indieweb](https://www.neatnik.net/hardcore-indieweb)

生成摘要时出错

---

## 26. TP-Link Kasa cameras leaked home GPS via unauthenticated UDP for 6 years

**原文标题**: TP-Link Kasa cameras leaked home GPS via unauthenticated UDP for 6 years

**原文链接**: [https://github.com/BadChemical/IoT-Vulnerability-Research-Public/blob/main/TP-Link_Kasa_EC71/Kasa_EC71.md](https://github.com/BadChemical/IoT-Vulnerability-Research-Public/blob/main/TP-Link_Kasa_EC71/Kasa_EC71.md)

生成摘要时出错

---

## 27. Qwen 3.8 Max Preview

**原文标题**: Qwen 3.8 Max Preview

**原文链接**: [https://www.qwencloud.com/pricing/token-plan](https://www.qwencloud.com/pricing/token-plan)

生成摘要时出错

---

## 28. Minecraft: Java Edition now uses SDL3

**原文标题**: Minecraft: Java Edition now uses SDL3

**原文链接**: [https://www.minecraft.net/en-us/article/minecraft-26-3-snapshot-4](https://www.minecraft.net/en-us/article/minecraft-26-3-snapshot-4)

生成摘要时出错

---

## 29. Texas wins court order to suspend domain name for violating age-verification law

**原文标题**: Texas wins court order to suspend domain name for violating age-verification law

**原文链接**: [https://www.texasattorneygeneral.gov/news/releases/attorney-general-ken-paxton-secures-landmark-legal-victory-lock-pornographic-website-domain-and](https://www.texasattorneygeneral.gov/news/releases/attorney-general-ken-paxton-secures-landmark-legal-victory-lock-pornographic-website-domain-and)

生成摘要时出错

---

## 30. FAA lets Boeing sign off on 737 MAX, 787 airworthiness certificates again

**原文标题**: FAA lets Boeing sign off on 737 MAX, 787 airworthiness certificates again

**原文链接**: [https://www.cnbc.com/2026/07/17/faa-boeing-737-max-787.html](https://www.cnbc.com/2026/07/17/faa-boeing-737-max-787.html)

生成摘要时出错

---

## 31. Static search trees: 40x faster than binary search (2024)

**原文标题**: Static search trees: 40x faster than binary search (2024)

**原文链接**: [https://curiouscoding.nl/posts/static-search-tree/](https://curiouscoding.nl/posts/static-search-tree/)

生成摘要时出错

---

## 32. Classic Amiga titles, free to download

**原文标题**: Classic Amiga titles, free to download

**原文链接**: [https://amigafreeware.downer.tech/](https://amigafreeware.downer.tech/)

生成摘要时出错

---

## 33. The Computer at the Bottom of a Canal

**原文标题**: The Computer at the Bottom of a Canal

**原文链接**: [https://negroniventurestudios.com/2026/07/18/the-computer-at-the-bottom-of-a-canal/](https://negroniventurestudios.com/2026/07/18/the-computer-at-the-bottom-of-a-canal/)

生成摘要时出错

---

## 34. Open Book Touch: open-source e-reader

**原文标题**: Open Book Touch: open-source e-reader

**原文链接**: [https://www.crowdsupply.com/oddly-specific-objects/open-book-touch](https://www.crowdsupply.com/oddly-specific-objects/open-book-touch)

生成摘要时出错

---

## 35. Show HN: IKEA Complexity Index

**原文标题**: Show HN: IKEA Complexity Index

**原文链接**: [https://ikea.greg.technology/](https://ikea.greg.technology/)

生成摘要时出错

---

## 36. Painting the sides of railroad rails white to reduce derailment

**原文标题**: Painting the sides of railroad rails white to reduce derailment

**原文链接**: [https://www.up.com/news/safety/Tracking-Rail-Heat-260608](https://www.up.com/news/safety/Tracking-Rail-Heat-260608)

生成摘要时出错

---

## 37. British runner Josh Kerr breaks world record for mile which stood for 27 years

**原文标题**: British runner Josh Kerr breaks world record for mile which stood for 27 years

**原文链接**: [https://news.sky.com/story/british-runner-josh-kerr-breaks-world-record-for-mile-which-had-stood-for-27-years-13564688](https://news.sky.com/story/british-runner-josh-kerr-breaks-world-record-for-mile-which-had-stood-for-27-years-13564688)

生成摘要时出错

---

## 38. Topcoat: The full full-stack framework for Rust

**原文标题**: Topcoat: The full full-stack framework for Rust

**原文链接**: [https://github.com/tokio-rs/topcoat](https://github.com/tokio-rs/topcoat)

生成摘要时出错

---

## 39. I started a “dirt notebook”

**原文标题**: I started a “dirt notebook”

**原文链接**: [https://pinewind.bearblog.dev/i-started-a-dirt-notebook/](https://pinewind.bearblog.dev/i-started-a-dirt-notebook/)

生成摘要时出错

---

## 40. I joined the IndieWeb, here's what I learned

**原文标题**: I joined the IndieWeb, here's what I learned

**原文链接**: [https://en.andros.dev/blog/0b8e451e/i-joined-the-indieweb-heres-what-i-learned/](https://en.andros.dev/blog/0b8e451e/i-joined-the-indieweb-heres-what-i-learned/)

生成摘要时出错

---

## 41. Fake food delivery site for the dopamine

**原文标题**: Fake food delivery site for the dopamine

**原文链接**: [https://old.reddit.com/r/BingeEatingDisorder/comments/1uzr3ui/fake_food_delivery_site_for_the_dopamine/](https://old.reddit.com/r/BingeEatingDisorder/comments/1uzr3ui/fake_food_delivery_site_for_the_dopamine/)

生成摘要时出错

---

## 42. Steam Machine: Between 12k and 15k Units Sold per week

**原文标题**: Steam Machine: Between 12k and 15k Units Sold per week

**原文链接**: [https://boilingsteam.com/steam-machine-between-10k-and-15k-sold-per-week/](https://boilingsteam.com/steam-machine-between-10k-and-15k-sold-per-week/)

生成摘要时出错

---

## 43. Typing Speed Test, but for Developers

**原文标题**: Typing Speed Test, but for Developers

**原文链接**: [https://haxxorwpm.0s.is/](https://haxxorwpm.0s.is/)

生成摘要时出错

---

## 44. Moonshot AI suspends new subscriptions due to Kimi K3 demand

**原文标题**: Moonshot AI suspends new subscriptions due to Kimi K3 demand

**原文链接**: [https://twitter.com/kimi_moonshot/status/2078855608565207130](https://twitter.com/kimi_moonshot/status/2078855608565207130)

生成摘要时出错

---

## 45. REO Trucks I4 4WD Pickup Truck Starts at $21,500

**原文标题**: REO Trucks I4 4WD Pickup Truck Starts at $21,500

**原文链接**: [https://reotrucks.com](https://reotrucks.com)

生成摘要时出错

---

## 46. FDA approves new kind of cholesterol pill

**原文标题**: FDA approves new kind of cholesterol pill

**原文链接**: [https://www.fda.gov/news-events/press-announcements/fda-approves-first-oral-pcsk9-inhibitor-lower-ldl-cholesterol-adults-high-cholesterol](https://www.fda.gov/news-events/press-announcements/fda-approves-first-oral-pcsk9-inhibitor-lower-ldl-cholesterol-adults-high-cholesterol)

生成摘要时出错

---

## 47. The death and rebirth of my home server

**原文标题**: The death and rebirth of my home server

**原文链接**: [https://sgt.hootr.club/blog/home-server-rebirth/](https://sgt.hootr.club/blog/home-server-rebirth/)

生成摘要时出错

---

## 48. Show HN: Q3Edit – Edit and play Quake 3 maps in the browser

**原文标题**: Show HN: Q3Edit – Edit and play Quake 3 maps in the browser

**原文链接**: [https://q3edit.com](https://q3edit.com)

生成摘要时出错

---

## 49. Qubes OS Security in the Public Record

**原文标题**: Qubes OS Security in the Public Record

**原文链接**: [https://arxiv.org/abs/2607.14587](https://arxiv.org/abs/2607.14587)

生成摘要时出错

---

## 50. The US grocery slowdown is real

**原文标题**: The US grocery slowdown is real

**原文链接**: [https://www.bain.com/insights/the-us-grocery-slowdown-is-real-snap-chart/](https://www.bain.com/insights/the-us-grocery-slowdown-is-real-snap-chart/)

生成摘要时出错

---

## 51. Texas Police Spent $4.5M on Four Chevy Tahoes

**原文标题**: Texas Police Spent $4.5M on Four Chevy Tahoes

**原文链接**: [https://www.thedrive.com/news/how-texas-police-spent-4-5-million-on-four-chevy-tahoes](https://www.thedrive.com/news/how-texas-police-spent-4-5-million-on-four-chevy-tahoes)

生成摘要时出错

---

## 52. I burned all my tokens researching how to save tokens

**原文标题**: I burned all my tokens researching how to save tokens

**原文链接**: [https://quesma.com/blog/custom-deep-research-pipeline/](https://quesma.com/blog/custom-deep-research-pipeline/)

生成摘要时出错

---

## 53. Co-evolution of self-replication and function in a digital primordial soup

**原文标题**: Co-evolution of self-replication and function in a digital primordial soup

**原文链接**: [https://arxiv.org/abs/2607.09211](https://arxiv.org/abs/2607.09211)

生成摘要时出错

---

## 54. Meta trying to destroy whistleblower Sarah Wynn-Williams, US senator says

**原文标题**: Meta trying to destroy whistleblower Sarah Wynn-Williams, US senator says

**原文链接**: [https://www.theguardian.com/technology/2026/jul/17/meta-whistleblower-sarah-wynn-williams-us-senator-josh-hawley](https://www.theguardian.com/technology/2026/jul/17/meta-whistleblower-sarah-wynn-williams-us-senator-josh-hawley)

生成摘要时出错

---

## 55. Bananas sprout in Rayleigh Garden UK after 15 years

**原文标题**: Bananas sprout in Rayleigh Garden UK after 15 years

**原文链接**: [https://www.bbc.com/news/articles/cvg8edqq5g5o](https://www.bbc.com/news/articles/cvg8edqq5g5o)

生成摘要时出错

---

## 56. Stenchill: 3D Printable Solder Paste Stencil Generator

**原文标题**: Stenchill: 3D Printable Solder Paste Stencil Generator

**原文链接**: [https://www.stenchill.com/en/](https://www.stenchill.com/en/)

生成摘要时出错

---

## 57. The Isomorphic Labs Drug Design Engine unlocks a new frontier beyond AlphaFold

**原文标题**: The Isomorphic Labs Drug Design Engine unlocks a new frontier beyond AlphaFold

**原文链接**: [https://www.isomorphiclabs.com/articles/the-isomorphic-labs-drug-design-engine-unlocks-a-new-frontier](https://www.isomorphiclabs.com/articles/the-isomorphic-labs-drug-design-engine-unlocks-a-new-frontier)

生成摘要时出错

---

## 58. Tech note: making your own V-I plots at home

**原文标题**: Tech note: making your own V-I plots at home

**原文链接**: [https://lcamtuf.substack.com/p/tech-note-making-your-own-v-i-plots](https://lcamtuf.substack.com/p/tech-note-making-your-own-v-i-plots)

生成摘要时出错

---

## 59. Our Approach to Bioresilience: Isomorphic Labs and Google DeepMind

**原文标题**: Our Approach to Bioresilience: Isomorphic Labs and Google DeepMind

**原文链接**: [https://deepmind.google/blog/our-approach-to-bioresilience/](https://deepmind.google/blog/our-approach-to-bioresilience/)

生成摘要时出错

---

## 60. The Last MPEG-4 Visual Patent Has Expired

**原文标题**: The Last MPEG-4 Visual Patent Has Expired

**原文链接**: [https://www.phoronix.com/news/Last-MPEG-4-Patent-Expired](https://www.phoronix.com/news/Last-MPEG-4-Patent-Expired)

生成摘要时出错

---

## 61. Harness Engineering

**原文标题**: Harness Engineering

**原文链接**: [https://github.com/lopopolo/harness-engineering](https://github.com/lopopolo/harness-engineering)

生成摘要时出错

---

## 62. Flock CEO Apologizes for Calling Activists 'Terrorists'

**原文标题**: Flock CEO Apologizes for Calling Activists 'Terrorists'

**原文链接**: [https://www.forbes.com/sites/thomasbrewster/2026/07/17/flock-ceo-sorry-for-labelling-activists-terrorists/](https://www.forbes.com/sites/thomasbrewster/2026/07/17/flock-ceo-sorry-for-labelling-activists-terrorists/)

生成摘要时出错

---

## 63. No link between acetaminophen use during pregnancy and adverse birth outcomes

**原文标题**: No link between acetaminophen use during pregnancy and adverse birth outcomes

**原文链接**: [https://sph.unc.edu/sph-news/no-link-between-acetaminophen-use-during-pregnancy-and-adverse-birth-outcomes-study-finds/](https://sph.unc.edu/sph-news/no-link-between-acetaminophen-use-during-pregnancy-and-adverse-birth-outcomes-study-finds/)

生成摘要时出错

---

## 64. What's the deal with all the random weekly quota resets for agents lately?

**原文标题**: What's the deal with all the random weekly quota resets for agents lately?

**原文链接**: [https://minimaxir.com/2026/07/agent-quota-reset/](https://minimaxir.com/2026/07/agent-quota-reset/)

生成摘要时出错

---

## 65. Young adults are poor despite every metric which suggests otherwise

**原文标题**: Young adults are poor despite every metric which suggests otherwise

**原文链接**: [https://xcancel.com/i/article/2077113148524417439](https://xcancel.com/i/article/2077113148524417439)

生成摘要时出错

---

## 66. AI Mania Is Eviscerating Global Decision-Making

**原文标题**: AI Mania Is Eviscerating Global Decision-Making

**原文链接**: [https://ludic.mataroa.blog/blog/ai-mania-is-eviscerating-global-decision-making/](https://ludic.mataroa.blog/blog/ai-mania-is-eviscerating-global-decision-making/)

生成摘要时出错

---

## 67. Mac gaming is finally getting the overpowered upgrade it deserves

**原文标题**: Mac gaming is finally getting the overpowered upgrade it deserves

**原文链接**: [https://www.macworld.com/article/3189951/apples-latest-game-porting-toolkit-beta-changed-how-i-think-about-mac-gaming.html](https://www.macworld.com/article/3189951/apples-latest-game-porting-toolkit-beta-changed-how-i-think-about-mac-gaming.html)

生成摘要时出错

---

## 68. Everybody's Weirded Out by AI–Except the People Who Foist It on Us

**原文标题**: Everybody's Weirded Out by AI–Except the People Who Foist It on Us

**原文链接**: [https://newrepublic.com/article/213004/everybody-weirded-ai-except-people-foist-us](https://newrepublic.com/article/213004/everybody-weirded-ai-except-people-foist-us)

生成摘要时出错

---

## 69. Moonstone: Modern, cross-platform Lua runtime and package manager written in Zig

**原文标题**: Moonstone: Modern, cross-platform Lua runtime and package manager written in Zig

**原文链接**: [https://moonstone.sh/](https://moonstone.sh/)

生成摘要时出错

---

## 70. Judge a book by its first pages

**原文标题**: Judge a book by its first pages

**原文链接**: [https://uncovered.ink](https://uncovered.ink)

生成摘要时出错

---

## 71. Real-Time LuaTeX: Recompiling Large Documents in 1ms [pdf]

**原文标题**: Real-Time LuaTeX: Recompiling Large Documents in 1ms [pdf]

**原文链接**: [https://www.tug.org/tug2026/preprints/lode-realtime.pdf](https://www.tug.org/tug2026/preprints/lode-realtime.pdf)

生成摘要时出错

---

## 72. The Art of Insight in Science and Engineering – Mastering Complexity(2014) [pdf]

**原文标题**: The Art of Insight in Science and Engineering – Mastering Complexity(2014) [pdf]

**原文链接**: [https://ocw.mit.edu/courses/res-6-011-the-art-of-insight-in-science-and-engineering-mastering-complexity-fall-2014/3bca850386a3005c22134fa62fb3bad5_MITRES_6-011F14_art_insfin.pdf](https://ocw.mit.edu/courses/res-6-011-the-art-of-insight-in-science-and-engineering-mastering-complexity-fall-2014/3bca850386a3005c22134fa62fb3bad5_MITRES_6-011F14_art_insfin.pdf)

生成摘要时出错

---

## 73. Ollama: All Aboard Open Models

**原文标题**: Ollama: All Aboard Open Models

**原文链接**: [https://ollama.com/blog/all-aboard-open-models](https://ollama.com/blog/all-aboard-open-models)

生成摘要时出错

---

## 74. UnifiedIR for Julia

**原文标题**: UnifiedIR for Julia

**原文链接**: [https://github.com/JuliaLang/julia/pull/62334](https://github.com/JuliaLang/julia/pull/62334)

生成摘要时出错

---

## 75. A grumpy screed about AI in software engineering

**原文标题**: A grumpy screed about AI in software engineering

**原文链接**: [https://sam.sutch.net/posts/a-grumpy-ai-screed](https://sam.sutch.net/posts/a-grumpy-ai-screed)

生成摘要时出错

---

## 76. Clever hacker fits 537,000 domains in a $5 ESP32 ad-blocking dongle

**原文标题**: Clever hacker fits 537,000 domains in a $5 ESP32 ad-blocking dongle

**原文链接**: [https://www.tomshardware.com/networking/clever-hacker-fits-537-000-domains-in-a-tiny-usd5-esp32-ad-blocking-dongle-firmware-uses-only-around-50kb-of-ram-and-can-answer-blocked-lookups-in-10-milliseconds](https://www.tomshardware.com/networking/clever-hacker-fits-537-000-domains-in-a-tiny-usd5-esp32-ad-blocking-dongle-firmware-uses-only-around-50kb-of-ram-and-can-answer-blocked-lookups-in-10-milliseconds)

生成摘要时出错

---

## 77. Scrying the AMD GFX1250 LLVM Tea Leaves

**原文标题**: Scrying the AMD GFX1250 LLVM Tea Leaves

**原文链接**: [https://chipsandcheese.com/p/scrying-the-amd-gfx1250-llvm-tea](https://chipsandcheese.com/p/scrying-the-amd-gfx1250-llvm-tea)

生成摘要时出错

---

## 78. Deepsec

**原文标题**: Deepsec

**原文链接**: [https://github.com/vercel-labs/deepsec](https://github.com/vercel-labs/deepsec)

生成摘要时出错

---

## 79. Flock Safety had a car journalist stalked, wrongly accused, and detained

**原文标题**: Flock Safety had a car journalist stalked, wrongly accused, and detained

**原文链接**: [https://www.thedrive.com/news/inside-the-flock-dragnet-how-systemic-errors-led-to-police-ambushing-me-for-no-reason](https://www.thedrive.com/news/inside-the-flock-dragnet-how-systemic-errors-led-to-police-ambushing-me-for-no-reason)

生成摘要时出错

---

## 80. Traders are increasingly betting against SpaceX just weeks after IPO

**原文标题**: Traders are increasingly betting against SpaceX just weeks after IPO

**原文链接**: [https://www.ft.com/content/2b96703d-440b-46db-8d86-9fff9ecc59d5](https://www.ft.com/content/2b96703d-440b-46db-8d86-9fff9ecc59d5)

生成摘要时出错

---

## 81. Terence McKenna's Mega Bad Trip

**原文标题**: Terence McKenna's Mega Bad Trip

**原文链接**: [https://psychedelics.community/cultural-icons/terence-mckennas-mega-bad-trip](https://psychedelics.community/cultural-icons/terence-mckennas-mega-bad-trip)

生成摘要时出错

---

## 82. Perforce charges $500 for training training videos.. and it's AI narrated

**原文标题**: Perforce charges $500 for training training videos.. and it's AI narrated

**原文链接**: [https://training.perforce.com/learn/courses/535/p4-helix-core-user-basic](https://training.perforce.com/learn/courses/535/p4-helix-core-user-basic)

生成摘要时出错

---

## 83. SpaceX and the myth of independent Wall St research

**原文标题**: SpaceX and the myth of independent Wall St research

**原文链接**: [https://www.ft.com/content/ce345155-d897-4f49-b7c8-13680e3b5434](https://www.ft.com/content/ce345155-d897-4f49-b7c8-13680e3b5434)

生成摘要时出错

---

## 84. LG monitors installing adware on Windows PCs

**原文标题**: LG monitors installing adware on Windows PCs

**原文链接**: [https://www.techradar.com/televisions/lgs-gaming-monitors-and-tvs-are-facing-a-user-revolt](https://www.techradar.com/televisions/lgs-gaming-monitors-and-tvs-are-facing-a-user-revolt)

生成摘要时出错

---

## 85. Even Microsoft couldn't make Windows 11 work well on 8GB of RAM

**原文标题**: Even Microsoft couldn't make Windows 11 work well on 8GB of RAM

**原文链接**: [https://www.theverge.com/tech/966937/microsoft-surface-laptop-13-inch-8gb-ram-2026-review](https://www.theverge.com/tech/966937/microsoft-surface-laptop-13-inch-8gb-ram-2026-review)

生成摘要时出错

---

## 86. HMD Touch 4G

**原文标题**: HMD Touch 4G

**原文链接**: [https://www.hmd.com/en_int/hmd-touch-4g](https://www.hmd.com/en_int/hmd-touch-4g)

生成摘要时出错

---

## 87. Valve say there's no end in sight to the memory crisis, prices going to increase

**原文标题**: Valve say there's no end in sight to the memory crisis, prices going to increase

**原文链接**: [https://www.pcgamer.com/hardware/steam-machines/valve-says-theres-no-end-in-sight-to-the-memory-crisis-and-prices-are-only-going-to-increase-honestly-its-still-getting-worse/](https://www.pcgamer.com/hardware/steam-machines/valve-says-theres-no-end-in-sight-to-the-memory-crisis-and-prices-are-only-going-to-increase-honestly-its-still-getting-worse/)

生成摘要时出错

---

## 88. Half a Second – a book about the XZ backdoor

**原文标题**: Half a Second – a book about the XZ backdoor

**原文链接**: [https://www.half-second.com/](https://www.half-second.com/)

生成摘要时出错

---

## 89. curl can be used to send emails with SMTP

**原文标题**: curl can be used to send emails with SMTP

**原文链接**: [https://mastodon.social/@chr1stian/116924759058231144](https://mastodon.social/@chr1stian/116924759058231144)

生成摘要时出错

---

## 90. Anthropic's newest ad is creeping people out

**原文标题**: Anthropic's newest ad is creeping people out

**原文链接**: [https://techcrunch.com/2026/07/14/anthropics-newest-ad-is-creeping-people-out/](https://techcrunch.com/2026/07/14/anthropics-newest-ad-is-creeping-people-out/)

生成摘要时出错

---

## 91. Heresy (2022]

**原文标题**: Heresy (2022]

**原文链接**: [https://paulgraham.com/heresy.html](https://paulgraham.com/heresy.html)

生成摘要时出错

---

## 92. I built a browser-based P2P file transfer tool using WebRTC

**原文标题**: I built a browser-based P2P file transfer tool using WebRTC

**原文链接**: [https://airdows.com/](https://airdows.com/)

生成摘要时出错

---

## 93. Texas spent $4.5M in Spy SUVs that scan phones in 3 minutes

**原文标题**: Texas spent $4.5M in Spy SUVs that scan phones in 3 minutes

**原文链接**: [https://letsaddresstexas.substack.com/p/texas-spent-45-million-on-israeli](https://letsaddresstexas.substack.com/p/texas-spent-45-million-on-israeli)

生成摘要时出错

---

## 94. Dumber Mini: A Nokia-Style Phone with WhatsApp and Maps

**原文标题**: Dumber Mini: A Nokia-Style Phone with WhatsApp and Maps

**原文链接**: [https://dumbermini.com/](https://dumbermini.com/)

生成摘要时出错

---

## 95. LLM-Integrated Multivariable Calculus Course

**原文标题**: LLM-Integrated Multivariable Calculus Course

**原文链接**: [https://calculus.academa.ai/](https://calculus.academa.ai/)

生成摘要时出错

---

## 96. Beginning July 20, Claude Fable 5 will be included in all Max plans

**原文标题**: Beginning July 20, Claude Fable 5 will be included in all Max plans

**原文链接**: [https://twitter.com/claudeai/status/2078302415804379218](https://twitter.com/claudeai/status/2078302415804379218)

生成摘要时出错

---

## 97. C64 Basic Dungeon Crawler: Goblin Attack (C64 Basic Part 8)

**原文标题**: C64 Basic Dungeon Crawler: Goblin Attack (C64 Basic Part 8)

**原文链接**: [https://retrogamecoders.com/c64-basic-dungeon-part8/](https://retrogamecoders.com/c64-basic-dungeon-part8/)

生成摘要时出错

---

## 98. AI Mania Is Eviscerating Global Decision-Making

**原文标题**: AI Mania Is Eviscerating Global Decision-Making

**原文链接**: [https://hermit-tech.com/blog/ai-mania-is-eviscerating-global-decisionmaking](https://hermit-tech.com/blog/ai-mania-is-eviscerating-global-decisionmaking)

生成摘要时出错

---

## 99. The Fermi Paradox, Percolation, and Inbreeding

**原文标题**: The Fermi Paradox, Percolation, and Inbreeding

**原文链接**: [https://reactormag.com/the-fermi-paradox-percolation-and-inbreeding/](https://reactormag.com/the-fermi-paradox-percolation-and-inbreeding/)

生成摘要时出错

---

## 100. Credit Card Points Are a Transfer from the Broke to the Comfortable

**原文标题**: Credit Card Points Are a Transfer from the Broke to the Comfortable

**原文链接**: [https://willisallstead.substack.com/p/your-credit-card-points-are-a-transfer](https://willisallstead.substack.com/p/your-credit-card-points-are-a-transfer)

生成摘要时出错

---

