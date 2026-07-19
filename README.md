# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-07-19.md)

*最后自动更新时间: 2026-07-19 20:31:45*
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

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 2 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 3 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 4 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 5 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 6 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 7 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 8 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 9 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 10 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 11 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 12 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 13 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 14 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 15 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 16 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 17 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 18 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 19 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 20 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 21 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 22 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 23 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 24 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 25 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 26 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 27 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 28 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 29 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 30 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 31 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 32 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 33 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 34 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 35 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 36 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 37 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 38 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 39 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 40 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 41 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 42 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 43 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 44 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 45 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 46 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 47 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 48 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 49 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 50 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 51 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 52 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 53 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 54 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 55 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 56 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 57 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 58 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 59 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 60 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 61 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 62 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 63 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 64 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 65 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 66 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 67 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 68 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 69 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 70 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 71 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 72 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 73 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 74 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 75 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 76 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 77 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 78 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 79 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 80 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 81 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 82 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 83 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 84 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 85 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 86 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 87 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 88 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 89 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 90 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 91 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 92 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 93 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 94 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 95 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 96 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 97 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 98 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 99 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 100 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 101 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 102 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 103 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 104 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 105 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 106 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 107 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 108 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 109 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 110 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 111 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 112 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 113 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 114 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 115 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 116 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 117 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 118 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 119 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 120 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 121 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 122 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 123 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 124 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 125 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 126 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 127 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 128 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 129 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 130 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 131 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 132 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 133 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 134 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 135 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 136 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 137 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 138 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 139 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 140 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 141 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 142 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 143 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 144 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 145 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 146 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 147 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 148 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 149 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 150 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 151 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 152 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 153 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 154 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 155 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 156 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 157 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 158 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 159 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 160 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 161 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 162 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 163 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 164 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 165 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 166 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 167 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 168 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 169 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 170 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 171 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 172 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 173 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 174 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 175 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 176 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 177 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 178 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 179 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 180 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 181 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 182 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 183 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 184 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 185 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 186 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 187 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 188 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 189 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 190 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 191 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 192 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 193 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 194 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 195 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 196 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 197 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 198 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 199 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 200 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 201 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 202 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 203 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 204 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 205 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 206 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 207 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 208 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 209 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 210 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 211 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 212 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 213 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 214 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 215 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 216 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 217 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 218 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 219 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 220 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 221 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 222 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 223 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 224 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 225 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 226 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 227 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 228 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 229 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 230 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 231 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 232 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 233 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 234 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 235 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 236 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 237 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 238 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 239 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 240 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 241 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 242 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 243 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 244 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 245 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 246 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 247 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 248 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 249 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 250 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 251 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 252 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 253 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 254 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
