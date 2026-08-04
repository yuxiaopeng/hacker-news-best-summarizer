# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-08-04.md)

*最后自动更新时间: 2026-08-04 21:00:55*
## 1. 别当炮灰

**原文标题**: Don't be a meat proxy

**原文链接**: [https://gruhn.me/blog/2026-08-03/](https://gruhn.me/blog/2026-08-03/)

文章批评了一种日益增长的趋势，即个人在专业和个人交流中，一字不差地转述人工智能（如Claude等工具）生成的内容，充当“肉身代理人”。作者认为这种做法毫无价值，因为接收者可以更快地直接访问人工智能，并自行控制语境。

阅读人工智能的输出被描述为“额外的精力”，因为它冗长、常有似是而非的废话以及密集的行话，Claude的一个复杂技术句子就可为例证。

作者敦促用户不要仅仅转发人工智能的回复，而是将其作为工具来利用，但随后要批判性地“阅读、理解、验证它，然后用自己的语言撰写回复”。这种综合和个人表达的过程被认为是个人能够增加的真正价值。

文章以代码审查为例，说明开发者如何在没有真正理解的情况下使用人工智能生成代码并回应反馈，从而有效地使审查者（和人工智能）成为真正的实现者，而开发者仅仅充当“肉身代理人”。核心信息强调了人类批判性思维和个人贡献的重要性，而非被动地转述人工智能的输出。

---

## 2. 大语言模型回报专业知识

**原文标题**: LLMs reward expertise

**原文链接**: [https://www.seangoedecke.com/llms-reward-expertise/](https://www.seangoedecke.com/llms-reward-expertise/)

本文挑战了“与大型语言模型（LLM）合作无需技能”的观点，认为虽然LLM通过让每个人都成为通才来普及基础任务，但真正价值的提取则取决于**领域专业知识**。

作者以数学家陶哲轩在复杂数学问题上与ChatGPT的卓越互动（相比于业余爱好者）为例阐述了这一点。陶哲轩的成功不仅源于简短精确的提示、间接的质疑和提出自己的建议，更关键的是他深厚的数学理解。这种专业知识使他能够提取相关想法、提出替代表述并识别不准确之处，有效地“将模型引导至‘与数学家对话’模式”。

作者通过个人编程经验证实了这一点，指出熟悉代码库能够以更具体的问题更深入地驱动LLM，并将其引导至最佳解决方案。这强调了具体、专门的知识往往比通用原理更有价值。

最终，虽然没有领域知识的人可以获得基本输出，但专家可以通过精准引导LLM，“榨取”远超于此的价值。文章总结道，人类专业知识依然至关重要，因为瓶颈往往在于人类准确传达所需解决方案的能力，从而有效地从模型中提取出已存在的信息。

---

## 3. Qwen3.8-Max：编程与协同工作的新标杆

**原文标题**: Qwen3.8-Max: A New Bar for Coding and Cowork

**原文链接**: [https://qwen.ai/blog?id=qwen3.8](https://qwen.ai/blog?id=qwen3.8)

文章提供的内容极其有限，仅包含“Qwen”一词。

然而，根据标题“Qwen3.8-Max：编码与协作的新标杆”，该文章很可能会介绍Qwen3.8-Max，作为Qwen大语言模型系列的一个新迭代版本。其核心信息将强调其在编码和协作（“cowork”）领域的先进能力。文章会突出Qwen3.8-Max如何旨在为这些领域的性能和实用性树立更高的标准或基准。文章可能会深入探讨具体的特性、改进和用例，以展示其对开发者、团队以及从事编程任务和协作项目的个人所提升的熟练度，从而将其定位为一个旨在提升这些关键专业领域生产力和效率的重大进展。

---

## 4. SQLite 关键CVE 还是 LLM 胡言乱语？

**原文标题**: SQLite Critical CVEs or LLM Slop?

**原文链接**: [https://research.jfrog.com/post/sqlite-critical-cves-or-llm-slops/](https://research.jfrog.com/post/sqlite-critical-cves-or-llm-slops/)

JFrog安全研究人员发现了一批关键的SQLite CVEs，这些CVE最初由NVD和CISA标记，但似乎大部分是伪造的，或者说是“LLM垃圾信息”。一个新的GitHub仓库发布了50多条此类通告，但JFrog的调查显示，其中引用的代码不存在，PoC（概念验证）有效载荷失败，且SQLite的官方通告也未提及这些漏洞。AI检测工具进一步表明这些通告是由AI生成的。

具体例子包括CVE-2026-51302，它声称SQLite 3.41.0中一个不存在的函数存在“Use-After-Free”漏洞，以及CVE-2026-51303，它引用了一个从未发生过的“补丁”且具有无效的PoC。其他CVE则引用了不可能的行号或不相关的代码。

这种普遍存在的伪造行为凸显了漏洞报告生态系统中的一个关键缺陷。MITRE的提交过程缺乏身份验证，NIST的国家漏洞数据库（NVD）由于报告激增，于2024年2月暂停了深度人工分析，这导致系统支离破碎，缺乏强制性的概念验证。

该事件表明了一个系统性问题，即自动化摄取可能传播虚假信息。来自问题GitHub账户的55条通告中，有54条是完全伪造的。这种“垃圾CVE”浪费了组织资源，污染了数据库，并可能误导AI驱动的漏洞分类工作。JFrog建议不要盲目相信来自未经验证来源的新CVE，应调查关键声明、验证环境影响并重现PoC。JFrog已将这些发现报告给GHSA、Red Hat和NVD，以便采取补救措施。

---

## 5. AI 生成的图片让我不想读你的博客

**原文标题**: AI-Generated Images Discourage Me from Reading Your Blog

**原文链接**: [https://nelson.cloud/ai-generated-images-discourage-me-from-reading-your-blog/](https://nelson.cloud/ai-generated-images-discourage-me-from-reading-your-blog/)

作者对博客中出现的AI生成图片表达了强烈且日益增长的反感，并指出这些图片的存在会极大地降低他们阅读的意愿。这种反感源于一种怀疑：如果图片是AI生成的，那么附带的文字在某种程度上也可能是大型语言模型（LLM）的产物，而非真实的人类思想。

作者认为这在个人或“独立”博客中尤为令人失望，因为他们期待在那里看到真实的人类表达，这与企业博客形成对比，在企业博客中，此类图片更容易被预料到。他们声称，即使是拙劣的人工绘制图片，例如用Microsoft Paint画的，也比AI图片更受青睐，因为前者能确认有人类参与。作者强调了自己博客的真实性，向读者保证内容是真实的人类思想。他们最后敦促个人博客所有者避免使用AI生成图片。

---

## 6. 开发者工具必须开源

**原文标题**: Devtools must be open source

**原文链接**: [https://blog.exe.dev/devtools-must-be-open-source](https://blog.exe.dev/devtools-must-be-open-source)

文章认为，AI代理正在从根本上改变软件个性化，使工程师能够“惊人地容易地”为个人需求定制应用程序。过去，由于高昂的开发和维护成本，编写个人软件的情况很少见。现在，代理可以下载、修改、构建，并持续将本地更改与上游源代码进行变基，这极大地提升了个性化投资回报率。

这种代理驱动的方法允许用户通过简单的文本提示来实现功能或集成工具，直接修改源代码本身，而不是依赖预定义的配置文件、扩展API或插件系统。作者通过一个简单的提示将名为“meat.dev”的工具集成到Shelley代理中来阐述这一点，这项任务在传统方法下被认为是“几乎不可能”的。

文章认为，这一转变使得复杂的配置系统变得过时。代理现在可以承担理解和修改源代码的“繁重工作”，使单个用户或小型团队能够从现有组件中创建高度定制的软件。为了使软件产品，尤其是开发工具，在这个“个性化软件时代”保持竞争力，它们必须提供对其源代码的访问权限。只提供预定义定制挂钩的闭源代理或应用程序将受到限制，而开源替代方案则允许真正的、代理驱动的个性化，其中源代码是终极扩展系统。

---

## 7. 数学与理论计算机科学的十大进展

**原文标题**: Ten advances in mathematics and theoretical computer science

**原文链接**: [https://openai.com/index/ten-advances-in-mathematics/](https://openai.com/index/ten-advances-in-mathematics/)

2026年8月1日，一份刊物宣布了由OpenAI下一代主要AI模型Astra的内部版本在数学和理论计算机科学领域取得的十项重大进展。这项举措建立在他们为学术研究者提供模型免费访问的“面向学术研究者的ChatGPT”计划基础之上，并继先前AI生成的对埃尔德什单位距离猜想的证伪之后。

这十项新成果解决了或在长期存在的开放问题上取得了实质性进展，涵盖高维几何、编码理论、群论、算子代数、量子复杂性、格密码学和极值组合学等多个领域。值得注意的成就包括球体堆积密度的新上界、二进制码和球面码的改进界限、构造出非索非克群、证伪科恩斯的刚性猜想、算术电路复杂性的新下界、量子博弈的指数并行重复定理，以及最近向量问题的多项式因子硬度。若干成果也解决了埃尔德什的特定问题。

AI模型Astra生成了这些数学论证，据估计花费了大约2000美元的代币。人类研究人员随后在模型的协助下准备了手稿，并在Lean证书中形式化了这些论证。OpenAI强调了诚实归属的重要性，即承认AI的贡献，同时对证明的正确性负责。他们邀请数学界参与讨论这些成果，并随着AI系统发展成为复杂的科研合作者，倡导广泛开放这些工具以支持科学发现。

---

## 8. More German than many Germans

**原文标题**: More German than many Germans

**原文链接**: [https://mertbulan.com/more-german-than-many-germans/](https://mertbulan.com/more-german-than-many-germans/)

生成摘要时出错

---

## 9. Prevent cognitive debt by manually retyping LLM-generated code

**原文标题**: Prevent cognitive debt by manually retyping LLM-generated code

**原文链接**: [https://ankursethi.com/blog/prevent-cognitive-debt-by-manually-retyping-llm-generated-code/](https://ankursethi.com/blog/prevent-cognitive-debt-by-manually-retyping-llm-generated-code/)

生成摘要时出错

---

## 10. Ray Bradbury's "There Will Come Soft Rains" is set today (2026-08-04)

**原文标题**: Ray Bradbury's "There Will Come Soft Rains" is set today (2026-08-04)

**原文链接**: [https://short-stories.co/@raybradbury/there-will-come-soft-rains-6k8vr4xxlnmj](https://short-stories.co/@raybradbury/there-will-come-soft-rains-6k8vr4xxlnmj)

Set on August 4, 2026, in a post-apocalyptic Allendale, California, a fully automated house meticulously carries out its daily routine despite the absence of human occupants. The voice-clock announces the time, the kitchen prepares breakfast, and tiny robot mice clean the floors, all for a family long gone, their atomic silhouettes burned into the charred west wall from a past cataclysm. Outside, the city is rubble, giving off a radioactive glow, and the house stands as the sole survivor.

Later, a diseased, emaciated dog enters, tracks mud, and dies, only to be incinerated by the house. Automated bridge tables and a glowing nursery activate, serving no one. In the evening, the house recites Sara Teasdale's "There Will Come Soft Rains," a poignant poem about nature's indifference to humanity's extinction.

Suddenly, a falling tree bough shatters a kitchen window, starting a fire. The house's advanced systems fiercely fight the blaze, pumping water and chemicals, but the fire proves relentless, eventually destroying the attic "brain" and overwhelming the defenses. The automated voices wail "Fire!" in a tragic, chaotic symphony as the house collapses into ruins. Ultimately, only one wall remains, its last voice repeatedly announcing, "Today is August 5, 2026."

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 2 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 3 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 4 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 5 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 6 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 7 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 8 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 9 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 10 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 11 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 12 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 13 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 14 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 15 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 16 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 17 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 18 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 19 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 20 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 21 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 22 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 23 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 24 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 25 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 26 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 27 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 28 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 29 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 30 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 31 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 32 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 33 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 34 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 35 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 36 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 37 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 38 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 39 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 40 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 41 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 42 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 43 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 44 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 45 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 46 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 47 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 48 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 49 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 50 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 51 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 52 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 53 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 54 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 55 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 56 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 57 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 58 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 59 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 60 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 61 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 62 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 63 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 64 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 65 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 66 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 67 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 68 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 69 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 70 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 71 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 72 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 73 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 74 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 75 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 76 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 77 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 78 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 79 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 80 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 81 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 82 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 83 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 84 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 85 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 86 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 87 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 88 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 89 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 90 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 91 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 92 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 93 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 94 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 95 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 96 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 97 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 98 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 99 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 100 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 101 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 102 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 103 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 104 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 105 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 106 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 107 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 108 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 109 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 110 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 111 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 112 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 113 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 114 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 115 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 116 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 117 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 118 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 119 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 120 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 121 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 122 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 123 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 124 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 125 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 126 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 127 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 128 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 129 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 130 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 131 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 132 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 133 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 134 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 135 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 136 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 137 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 138 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 139 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 140 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 141 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 142 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 143 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 144 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 145 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 146 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 147 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 148 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 149 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 150 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 151 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 152 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 153 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 154 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 155 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 156 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 157 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 158 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 159 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 160 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 161 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 162 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 163 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 164 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 165 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 166 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 167 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 168 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 169 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 170 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 171 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 172 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 173 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 174 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 175 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 176 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 177 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 178 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 179 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 180 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 181 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 182 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 183 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 184 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 185 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 186 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 187 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 188 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 189 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 190 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 191 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 192 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 193 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 194 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 195 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 196 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 197 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 198 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 199 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 200 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 201 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 202 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 203 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 204 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 205 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 206 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 207 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 208 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 209 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 210 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 211 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 212 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 213 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 214 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 215 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 216 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 217 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 218 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 219 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 220 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 221 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 222 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 223 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 224 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 225 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 226 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 227 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 228 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 229 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 230 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 231 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 232 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 233 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 234 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 235 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 236 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 237 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 238 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 239 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 240 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 241 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 242 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 243 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 244 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 245 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 246 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 247 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 248 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 249 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 250 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 251 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 252 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 253 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 254 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 255 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 256 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 257 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 258 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 259 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 260 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 261 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 262 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 263 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 264 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 265 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 266 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 267 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 268 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 269 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 270 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
