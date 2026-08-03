# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-08-03.md)

*最后自动更新时间: 2026-08-03 20:56:56*
## 1. 不要做肉的替身

**原文标题**: Don't be a meat proxy

**原文链接**: [https://gruhn.me/blog/2026-08-03/](https://gruhn.me/blog/2026-08-03/)

作者批评了在专业或个人交流中，仅仅逐字转发AI输出的做法，并将这种行为称为“人肉代理”。这种情况经常发生在Slack、代码审查或聊天群组中，用户复制粘贴像Claude这样的AI工具的回复。

核心论点是这种做法毫无价值。接收者可以直接与AI互动，控制上下文并更快地获得答案。此外，AI输出往往冗长、可能包含看似合理但不正确的信息，并且越来越术语密集，这使得读者需要付出额外的努力来解读。一个例子是Claude关于“NATS控制平面事件”的复杂句子，需要进行大量的查阅才能理解。

作者不主张仅仅转发AI的回复，而是敦促用户向AI提问，然后阅读、理解并验证其输出。关键一步是用自己的话重写回复，这既是理解的证明，也是人类可以添加的真正价值。

文章将代码审查作为一个典型例子。开发者可能会将工单描述复制粘贴给AI，生成代码，然后利用AI来处理审查者的反馈，而没有真正地投入或理解代码。在这种情况下，AI和审查者成为了实际的执行者，而原始开发者仅仅充当了传导者。

---

## 2. Qwen3.8-Max：编程与协同的新标杆

**原文标题**: Qwen3.8-Max: A New Bar for Coding and Cowork

**原文链接**: [https://qwen.ai/blog?id=qwen3.8](https://qwen.ai/blog?id=qwen3.8)

提供的文章内容仅包含“Qwen”一词。

尽管标题“Qwen3.8-Max：编码与协作的新标杆”强烈暗示文章会讨论一个名为Qwen3.8-Max的新AI模型，并强调其在编码辅助和协作工作等方面的先进能力，但实际文章中却缺失了总结这些要点的具体内容。

因此，无法根据所提供的内容生成一份概括文章主要观点和关键信息的简洁摘要。

---

## 3. SQLite 关键CVE 还是 LLM 糟粕？

**原文标题**: SQLite Critical CVEs or LLM Slop?

**原文链接**: [https://research.jfrog.com/post/sqlite-critical-cves-or-llm-slops/](https://research.jfrog.com/post/sqlite-critical-cves-or-llm-slops/)

JFrog 安全研究人员驳斥了一系列严重的 SQLite 漏洞通报，这些通报发布在 GitHub 上，最初由 NVD 和 CISA 标记，并被认定为大多是捏造的“大语言模型垃圾内容”。他们的调查显示，这些通报引用了不存在的代码，提及了不相关的逻辑，提供了无法运行的漏洞验证（PoC）代码，并且未列入 SQLite 官方通报页面。人工智能检测工具进一步表明这些通报是人工智能生成的。

例如，CVE-2026-51302，最初被 Red Hat 评定为 10.0 级的严重漏洞，在 JFrog 证明其主张是基于不存在的函数后被降级。其他 CVE 也存在类似问题，其声称的问题包括捏造的补丁和不可能存在的行号。

此次事件暴露了 CVE 提交流程中存在的系统性漏洞。MITRE 的公共表格缺乏身份验证，而 NIST 的 NVD 自 2024 年 2 月以来面临大量积压，从而减少了其人工验证工作。至关重要的是，当前系统不要求提供 PoC，这使得看似合理但虚假的通报能够进入安全流程。

“垃圾 CVE”的泛滥可能会严重影响企业，导致浪费时间调查不存在的威胁，污染漏洞数据库，并可能导致人工智能驱动的安全工具生成错误的修复方案。JFrog 建议保持警惕，建议用户验证新的 CVE，尤其是来自未经证实来源的。警示标志包括缺乏供应商证实、缺失提交历史、矛盾的元数据以及引用不存在的代码。务必在安全环境中通过 PoC 重现报告的问题。JFrog 已将其调查结果报告给相关机构，以便采取补救措施。

---

## 4. 卡帕西的鹈鹕

**原文标题**: Karpathy’s Pelican

**原文链接**: [https://twitter.com/karpathy/status/2083749667410727319](https://twitter.com/karpathy/status/2083749667410727319)

安德烈·卡帕西（Andrej Karpathy）指出LLM测试正在发生转变，不再局限于简单的图像生成，而是转向复杂的生成任务。他通过挑战Opus 5将《指环王》第一段渲染到一个3D JavaScript环境中来展示这一点，并提供了100万个token预算。Opus 5花费两小时生成了5500行程序代码，令人印象深刻地协调多边形和动画来渲染故事，尽管存在一些“瑕疵”。

卡帕西强调了LLM独特的耐力和耐心，使它们能够承担人类通常认为过于耗时或复杂的“超定制”项目。他展望了一个“超定制世界”或“按需瞬时生成GTA-X”的未来，玩家可以作为NPC或角色沉浸在故事中，所有这些都是按需生成的。

然而，他也指出了一个关键弱点：LLM无法有效审查自身的视觉作品。Opus 5不得不依赖缓慢而费力的屏幕截图来检查其输出，这导致了错误和不完善之处。卡帕西总结道，改进的多模态能力，特别是LLM在其创作中原生感知视频或玩游戏的能力，对于在这些复杂的生成任务中实现更高质量和自我纠正至关重要。

---

## 5. 结构

**原文标题**: Diátaxis

**原文链接**: [https://diataxis.fr/](https://diataxis.fr/)

Diátaxis是一种系统化的技术文档方法，它根据对用户需求的理解，规定了内容、架构和形式的方法。它识别出四种不同的用户需求以及相应的文档形式：教程、操作指南、技术参考和解释，将它们置于系统的关系中，并提出文档应围绕这些结构进行组织。

该框架解决了关于写什么（内容）、如何写（风格）以及如何组织（架构）的问题。Diátaxis不仅帮助文档用户找到他们所需，也惠及创建者和维护者。它轻量级、易于掌握且易于应用，为他们的工作带来了积极的质量原则，同时不施加实施限制。

为便于开始，建议用户阅读一份简要的入门指南并立即应用其原则。也可以获取对Diátaxis基础和原则的更深入的理论理解。这种方法在实践中得到验证，已在数百个项目中成功采用，像Vonage、Gatsby和Cloudflare等公司的评价证明了它在提高文档质量、可发现性以及整体用户和贡献者体验方面的有效性。

---

## 6. 希丹 2.5

**原文标题**: Seedance 2.5

**原文链接**: [https://seed.bytedance.com/en/blog/one-take-creation-flexible-referencing-introducing-seedance-2-5](https://seed.bytedance.com/en/blog/one-take-creation-flexible-referencing-introducing-seedance-2-5)

Seedance 2.5，新一代视频创作模型，于2026年7月31日正式发布，在Seedance 2.0的多模态架构基础上，将重心从单纯的片段生成转向完成创意作品，并在长篇叙事、多模态参考和编辑方面实现了重大突破。

在长篇叙事方面，Seedance 2.5一次性可生成长达30秒的高质量音视频片段，支持多轮扩展以创作数分钟的内容。它增强了连贯性、镜头切换和整体视听质量，使完整的故事能够以一致的视听语言展开。

多模态参考功能得到显著升级，允许最多30张图片、10个视频片段和10个音频片段作为参考输入。粘土渲染、运动和创意参考等增强功能提供了对主题、动作和镜头工作的更精细控制，更好地理解复杂的创意意图，并确保多角色一致性和逼真的光照。

Seedance 2.5 还提供了更精确、更稳定的编辑能力。它提供时间戳级别的控制，以便在生成过程中和生成后进行有针对性的调整。绿幕、镜头透视和基于参考的编辑等高级功能已提升以满足电影和广告等领域的严苛专业需求，确保主体无缝融入新环境。

Seedance 2.5 已在即梦AI和豆包专业版上线，API接口即将开放，旨在释放更大的创意想象力和生产力，并将扩展到教育和制造等实际应用领域。

---

## 7. 开发工具必须开源

**原文标题**: Devtools must be open source

**原文链接**: [https://blog.exe.dev/devtools-must-be-open-source](https://blog.exe.dev/devtools-must-be-open-source)

文章认为，AI智能体正在彻底改变软件个性化，使其变得异常简单，并颠覆了以往的挑战。历史上，由于开发和维护成本高昂，工程师很少为自己编写或大幅定制软件，他们通常选择僵化、现成的解决方案。

现在，智能体让用户能够通过直接修改软件源代码来实现个性化。它们可以在本地下载、构建和集成修改，最重要的是，通过每晚的rebase（变基）自动管理与上游更新的同步。这大大减少了初始工作量和持续维护，使得个性化软件成为一种投入成本低、易于实现且可行的尝试。

作者以一个例子对此进行阐释：通过一个简单的提示，将他们的`meat.dev`工具集成到Shelley（一个智能体）中。这使得Shelley能够在后台预处理Git提交并显示过滤后的差异，这项复杂任务如果使用VS Code或Vim等传统、受限的扩展API，将会是“难以理清的痛苦”。

这种智能体驱动的方法与经典的配置或插件系统有着根本性的不同。智能体理解并能适应底层源代码，从而无需复杂、预先设计的扩展点。这意味着软件不再需要精密的插件系统或庞大的配置文件；智能体可以直接为个人用户，甚至是小型团队，实现所需功能。

归根结底，这种个性化能力完全取决于对软件源代码的访问权限。虽然Shelley、Pi或Codex等开源智能体可以深度个性化，但Claude Code等闭源软件将用户限制在预定义的定制钩子中，从而阻碍了智能体驱动的个性化定制的全部潜力。个性化软件时代需要开源。

---

## 8. Go 1.27 交互式导览

**原文标题**: Go 1.27 Interactive Tour

**原文链接**: [https://victoriametrics.com/blog/go-1-27/index.html](https://victoriametrics.com/blog/go-1-27/index.html)

生成摘要时出错

---

## 9. 比很多德国人更德国

**原文标题**: More German than many Germans

**原文链接**: [https://mertbulan.com/more-german-than-many-germans/](https://mertbulan.com/more-german-than-many-germans/)

The author recounts their transformative journey from Turkey to Germany, beginning with a 2017 internship in Hamburg. Initially holding stereotypical views of Germans as cold and rule-bound, their perception shifted after positive experiences with a trusting flatmate and friendly, inclusive colleagues. They found work culture surprisingly supportive, emphasizing well-being over overwork, and appreciated the flat hierarchies and social democracy reflected in equitable access to services like restaurants.

A key revelation was their affinity for German rules, both written (like fire safety) and unwritten (punctuality, *Ruhezeit*), finding them logical and trust-based. This appreciation led others to label them "more German than many Germans." The author also delved into German history and culture through extensive reading, noting the country's unique self-reflection and commitment to democratic values, evident in public protests against the far-right.

Despite a "soft landing" as an English-speaking professional in an international company, the author's observations extended to smaller German firms. Deciding to make Germany their home, they successfully navigated the citizenship process, emphasizing that becoming German meant embracing the country's democratic values, not just obtaining a passport. Their experience underscores a deep integration fostered by shared values rather than forced assimilation.

---

## 10. AI financial advice is surprisingly good, especially if you ask right questions

**原文标题**: AI financial advice is surprisingly good, especially if you ask right questions

**原文链接**: [https://mitsloan.mit.edu/ideas-made-to-matter/ai-financial-advice-surprisingly-good-especially-if-you-ask-right-questions](https://mitsloan.mit.edu/ideas-made-to-matter/ai-financial-advice-surprisingly-good-especially-if-you-ask-right-questions)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 2 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 3 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 4 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 5 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 6 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 7 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 8 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 9 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 10 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 11 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 12 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 13 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 14 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 15 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 16 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 17 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 18 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 19 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 20 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 21 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 22 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 23 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 24 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 25 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 26 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 27 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 28 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 29 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 30 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 31 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 32 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 33 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 34 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 35 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 36 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 37 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 38 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 39 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 40 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 41 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 42 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 43 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 44 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 45 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 46 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 47 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 48 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 49 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 50 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 51 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 52 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 53 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 54 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 55 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 56 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 57 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 58 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 59 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 60 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 61 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 62 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 63 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 64 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 65 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 66 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 67 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 68 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 69 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 70 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 71 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 72 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 73 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 74 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 75 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 76 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 77 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 78 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 79 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 80 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 81 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 82 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 83 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 84 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 85 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 86 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 87 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 88 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 89 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 90 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 91 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 92 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 93 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 94 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 95 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 96 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 97 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 98 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 99 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 100 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 101 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 102 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 103 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 104 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 105 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 106 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 107 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 108 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 109 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 110 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 111 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 112 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 113 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 114 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 115 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 116 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 117 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 118 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 119 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 120 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 121 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 122 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 123 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 124 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 125 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 126 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 127 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 128 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 129 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 130 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 131 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 132 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 133 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 134 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 135 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 136 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 137 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 138 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 139 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 140 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 141 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 142 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 143 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 144 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 145 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 146 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 147 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 148 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 149 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 150 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 151 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 152 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 153 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 154 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 155 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 156 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 157 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 158 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 159 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 160 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 161 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 162 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 163 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 164 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 165 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 166 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 167 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 168 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 169 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 170 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 171 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 172 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 173 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 174 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 175 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 176 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 177 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 178 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 179 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 180 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 181 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 182 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 183 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 184 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 185 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 186 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 187 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 188 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 189 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 190 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 191 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 192 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 193 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 194 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 195 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 196 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 197 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 198 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 199 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 200 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 201 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 202 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 203 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 204 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 205 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 206 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 207 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 208 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 209 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 210 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 211 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 212 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 213 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 214 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 215 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 216 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 217 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 218 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 219 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 220 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 221 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 222 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 223 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 224 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 225 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 226 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 227 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 228 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 229 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 230 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 231 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 232 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 233 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 234 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 235 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 236 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 237 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 238 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 239 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 240 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 241 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 242 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 243 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 244 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 245 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 246 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 247 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 248 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 249 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 250 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 251 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 252 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 253 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 254 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 255 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 256 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 257 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 258 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 259 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 260 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 261 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 262 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 263 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 264 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 265 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
| 266 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 267 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 268 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 269 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
