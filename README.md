# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-03-09.md)

*最后自动更新时间: 2026-03-09 20:09:25*
## 1. 代理安全屋 – 针对本地代理的macOS原生沙盒

**原文标题**: Agent Safehouse – macOS-native sandboxing for local agents

**原文链接**: [https://agent-safehouse.dev/](https://agent-safehouse.dev/)

Agent Safehouse 为本地AI代理提供 macOS 原生沙盒机制，解决概率性大语言模型可能造成的破坏性错误的风险。它通过 macOS 内核强制执行“默认拒绝”访问模型，在代理访问或修改未经授权的文件之前阻止系统调用。这意味着代理被拒绝在指定项目目录之外的写入权限，并且无法读取诸如 `~/.ssh` 或 `~/other-repos` 等敏感区域，从而确保操作零风险。

该工具确保代理在其沙盒内完美运行，自动拥有对当前项目目录的读写权限，以及对已安装工具链的读取权限。入门简单：下载一个Bash脚本，并在 `safehouse` 中运行你的代理命令即可。文章演示了内核如何拒绝未经授权的文件访问，而项目内的允许操作则成功执行。

为了优化工作流程，用户可以配置shell函数，默认在Safehouse中自动运行他们偏好的代理（例如，Claude、Codex、Gemini），并可选择在需要时绕过沙盒。高级用户甚至可以利用大语言模型生成定制的、最小权限的 `sandbox-exec` 配置文件，根据他们特定的主目录和工具链设置进行调整，确保最大的安全性和控制。Safehouse 旨在通过默认使代理交互安全，从而使开发者能够“快速行动，不破坏任何东西”。

---

## 2. 爱尔兰关闭最后一座燃煤电厂，成为欧洲第15个无煤国家 (2025年)

**原文标题**: Ireland shuts last coal plant, becomes 15th coal-free country in Europe (2025)

**原文链接**: [https://www.pv-magazine.com/2025/06/20/ireland-coal-free-ends-coal-power-generation-moneypoint/](https://www.pv-magazine.com/2025/06/20/ireland-coal-free-ends-coal-power-generation-moneypoint/)

这段文字是对爱尔兰宣布将于2025年关闭其最后一座燃煤电厂，从而成为一个无煤国家的举动所做的批判性评论。尽管承认其“对气候友好”的初衷，作者却质疑，如果爱尔兰继续燃烧煤炭，但转而从其他国家进口，这是否具有真正的环境效益。核心论点是，在他处（例如波兰）开采煤炭，通过船舶和卡车运到爱尔兰，然后再燃烧，这种做法实际上会因全球物流产生的额外排放而加剧污染。作者将此比作一个荒谬的场景：为了供应爱尔兰的一座发电厂而砍伐亚马逊雨林。最终，评论者认为这种政策是“象征性的气候关怀”，仅仅是制造出一种环保责任的表象，同时却可能通过将问题转移并加剧到其他地方，从而扩大整体碳足迹。

---

## 3. 显微镜能看到激光视盘上的视频。

**原文标题**: Microscopes can see video on a laserdisc

**原文链接**: [https://www.youtube.com/watch?v=qZuR-772cks](https://www.youtube.com/watch?v=qZuR-772cks)

文章标题“显微镜能看到激光影碟上的视频”暗示了可能会讨论在激光影碟上微观观看视频数据的技术可行性或相关现象。

然而，所提供的内容并未详细阐述该主题。相反，该内容完全由一系列常见于YouTube网站页脚或“关于”部分的中文短语组成。

这些短语提及了YouTube本身、新闻、版权、联系方式、创作者、广告商、开发者、条款、隐私政策、安全、YouTube的工作原理、测试新功能，以及“NFL Sunday Ticket© 2026 Google LLC。”。

因此，所提供的文本没有提供任何关于显微镜、视频或激光影碟的信息或讨论，反而似乎是来自其他来源的无关紧要的样板文本。

---

## 4. 框架书

**原文标题**: FrameBook

**原文链接**: [https://fb.edoo.gg](https://fb.edoo.gg)

“FrameBook”项目涉及将2006年黑色MacBook（型号A1181）的机箱改装为现代内部组件，灵感来源于改装旧Mac和PC。创作者采购了旧的MacBook和OEM机箱部件，旨在将怀旧美学与当前性能相结合。

主要组件包括一个Framework Laptop 13主板（Intel i7-1280P，64GB RAM）、一块CSOT显示面板、Framework扬声器、一个8MP网络摄像头和各种USB集线器。在集成过程中出现了重大挑战：通过将USB-C线焊接到其PCB上，使原装键盘和触控板恢复功能，这是创作者的首次焊接体验。内部安装使用了定制的3D打印支架，并用强力胶固定。

I/O端口需要大量修改；左侧被用电磨工具挖空，以容纳拆下的USB集线器，并由定制的3D打印I/O挡板覆盖。右侧利用了旧的DVD光驱槽来安装USB-C集线器。安装了一个定制的LED，以重现标志性的发光苹果标志。网络摄像头和电源按钮也需要定制集成。

这个为期三个月的项目让创作者学会了焊接和3D建模技能。尽管承认存在一些“粗糙”之处，例如内部安装依赖强力胶，以及希望拥有定制PCB，“FrameBook”项目仍成功地创造了一款独特、功能齐全的笔记本电脑，将经典设计与现代硬件完美结合。

---

## 5. 美国上诉法院：服务条款可通过邮件更新，使用即视为同意 [pdf]

**原文标题**: US Court of Appeals: TOS may be updated by email, use can imply consent [pdf]

**原文链接**: [https://cdn.ca9.uscourts.gov/datastore/memoranda/2026/03/03/25-403.pdf](https://cdn.ca9.uscourts.gov/datastore/memoranda/2026/03/03/25-403.pdf)

提供的内容是PDF文件的原始二进制格式，而非可读文本。要总结一篇文章，需要先提取文本内容。遗憾的是，我无法直接解读和总结这个原始PDF字节流中的信息。

---

## 6. 如何在本地运行Qwen 3.5

**原文标题**: How to run Qwen 3.5 locally

**原文链接**: [https://unsloth.ai/docs/models/qwen3.5](https://unsloth.ai/docs/models/qwen3.5)

本文提供了在本地运行阿里巴巴通义千问 3.5 大语言模型系列（包括从 0.8B 到 397B 参数的模型）的全面指南。这些多模态大语言模型性能卓越，支持 256K 上下文、201 种语言，并在智能体编程、视觉、聊天和长文本任务方面表现出色。

最新更新通过 Unsloth Dynamic 2.0 改进了 GGUF 量化，增强了聊天、编程、长上下文和工具调用能力。硬件要求差异很大：0.8B 模型只需 3GB 内存，而 397B-A17B 模型在 BF16 模式下可能需要高达 810GB，4 位量化下则需要 256GB。用户应确保总内存（显存 + 系统内存）超过模型文件大小，以获得最佳性能。

通义千问 3.5 支持“思考”和“非思考”模式，每种模式都为通用或精确的编程/推理任务推荐了 `temperature`、`top_p`、`top_k`、`min_p` 和 `presence_penalty` 设置。小型模型（0.8B-9B）默认禁用思考模式，可以通过 `--chat-template-kwargs '{"enable_thinking":true/false}'` 进行切换。

本地推理主要通过 `llama.cpp` 实现 CPU/GPU 运行，或使用 `LM Studio` 这种基于图形用户界面的方法。该过程包括获取 `llama.cpp`、通过 Hugging Face 下载 GGUF 模型（例如 UD-Q4_K_XL），并使用根据模型大小和所需思考模式定制的特定命令运行它们。LM Studio 用户下载模型后，可能需要通过 YAML 文件启用“思考”模式切换。对于生产环境，推荐使用 `llama-server`。请注意，通义千问 3.5 的 GGUF 模型目前与 Ollama 不兼容。

---

## 7. 邮编放前面

**原文标题**: Put the zip code first

**原文链接**: [https://zipcodefirst.com](https://zipcodefirst.com)

这篇文章热情地倡导在在线地址表单中将邮政编码放在首位，批评当前普遍存在的做法低效且过时。文章强调，一个5位数的美国邮政编码可以立即确定并自动填充城市、州和国家，从而省去用户手动输入这些字段以及浏览冗长下拉菜单的麻烦。

作者指出，这项功能是一个“已解决的问题”，只需利用免费API（如 `zippopotam.us`）的几行代码即可实现。将邮政编码放在首位还能大幅缩小搜索范围，显著提高街道地址的自动补全功能，从而实现更快、更准确的数据录入，并为公司提供更清晰的数据。

文章列出了常见表单设计失败的“耻辱榜”：将邮政编码放在最后且不用于自动填充（例如亚马逊、Target），收集了邮政编码却不利用它，提供无法搜索、只能滚动的国家下拉菜单（特别是当“美国”被错误归类时），以及点击返回按钮时会重置进度的表单。

其他建议包括对数字字段使用 `inputmode="numeric"` 以调出正确的手机键盘，以及利用适当的 `autocomplete` 属性与浏览器自动填充功能配合。尽管作者承认在国际情境下，国家选择可能需要先于邮政编码（并可能通过IP预填充），但核心信息依然是：不要再让用户输入那些可以轻易得知或推断的信息。作者恳请开发者实施这一简单而有益的改变，最后呼吁道：“把它放在首位，你们这些家伙！”

---

## 8. The changing goalposts of AGI and timelines

**原文标题**: The changing goalposts of AGI and timelines

**原文链接**: [https://mlumiste.com/general/openai-charter/](https://mlumiste.com/general/openai-charter/)

生成摘要时出错

---

## 9. Apple's 512GB Mac Studio vanishes, a quiet acknowledgment of the RAM shortage

**原文标题**: Apple's 512GB Mac Studio vanishes, a quiet acknowledgment of the RAM shortage

**原文链接**: [https://arstechnica.com/gadgets/2026/03/apples-512gb-mac-studio-vanishes-a-quiet-acknowledgement-of-the-ram-shortage/](https://arstechnica.com/gadgets/2026/03/apples-512gb-mac-studio-vanishes-a-quiet-acknowledgement-of-the-ram-shortage/)

生成摘要时出错

---

## 10. LibreOffice Writer now supports Markdown

**原文标题**: LibreOffice Writer now supports Markdown

**原文链接**: [https://blog.documentfoundation.org/blog/2026/02/04/libreoffice-26-2-is-here/](https://blog.documentfoundation.org/blog/2026/02/04/libreoffice-26-2-is-here/)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 2 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 3 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 4 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 5 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 6 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 7 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 8 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 9 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 10 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 11 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 12 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 13 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 14 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 15 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 16 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 17 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 18 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 19 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 20 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 21 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 22 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 23 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 24 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 25 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 26 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 27 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 28 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 29 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 30 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 31 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 32 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 33 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 34 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 35 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 36 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 37 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 38 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 39 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 40 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 41 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 42 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 43 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 44 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 45 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 46 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 47 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 48 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 49 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 50 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 51 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 52 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 53 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 54 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 55 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 56 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 57 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 58 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 59 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 60 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 61 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 62 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 63 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 64 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 65 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 66 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 67 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 68 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 69 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 70 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 71 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 72 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 73 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 74 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 75 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 76 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 77 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 78 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 79 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 80 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 81 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 82 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 83 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 84 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 85 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 86 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 87 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 88 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 89 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 90 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 91 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 92 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 93 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 94 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 95 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 96 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 97 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 98 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 99 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 100 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 101 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 102 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 103 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 104 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 105 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 106 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 107 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 108 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 109 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 110 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 111 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 112 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 113 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 114 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 115 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 116 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 117 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 118 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
| 119 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 120 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 121 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 122 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 123 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
