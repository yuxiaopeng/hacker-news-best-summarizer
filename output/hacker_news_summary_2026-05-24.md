# Hacker News 热门文章摘要 (2026-05-24)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 别光把AI甩给我。

**原文标题**: Don't just paste the AI at me

**原文链接**: [https://dontquotetheai.com/](https://dontquotetheai.com/)

文章《不要只是把AI内容发给我》批评了直接复制并发送AI聊天机器人回复来回答问题的常见做法。文章认为，这种做法没有帮助，因为接收方也能使用同样的工具，他们寻求的是提问者的个人背景、判断和独特视角，而不是一个通用的答案。仅仅作为AI的“代理人”显示了原创思想的缺失。

相反，作者建议将AI用作“起草伙伴”。推荐的方法是，阅读AI的输出后，再根据自己的理解进行加工，加入个人见解。主要建议包括：仅提取最相关的信息；保持回复简洁（例如三句话）；引用真正有用的AI段落并解释其价值。如果没有什么实质性的内容可补充，也可以说“我对此没有强烈看法”。

这篇文章本身就是一个可分享的链接（dontpastetheai.com），巧妙地传达了这一信息。它被描述为“带着温和的爱”和“由人类特意撰写”，鼓励人们进行深思熟虑的人际互动，而不是被动地转述AI内容。

---

## 2. Rubish：纯 Ruby 编写的 Unix shell

**原文标题**: Rubish: A Unix shell written in pure Ruby

**原文链接**: [https://github.com/amatsuda/rubish](https://github.com/amatsuda/rubish)

Rubish 是一个完全用纯 Ruby 编写的 UNIX shell，旨在完全兼容 Bash，同时深度集成 Ruby 的特性。它解析 shell 语法并将其编译成 Ruby 代码，允许用户无缝运行现有的 Bash 脚本。

超越标准 Bash 的主要特性包括：
*   **深度 Ruby 集成：** 用户可以混合使用 shell 命令和 Ruby 代码，使用 Ruby 表达式进行条件判断（如 `if { ... }`），以 Ruby 方法调用语法调用命令（如 `ls('-la')`），并用 Ruby 方法链式调用命令（如 `ls().sort`）。它支持 Ruby 迭代器块（如 `ls.each { |f| ... }`），以大写字母开头的行进行内联 Ruby 求值，Ruby 数组/正则表达式字面量，以及 Ruby 风格的函数定义。
*   **智能 Tab 补全：** 它能从工具的 `--help` 输出中自动推导子命令和标志，缓存结果，支持 fish 风格的自动建议，以及 zsh 风格的路径缩写补全。
*   **懒加载：** 将缓慢的 shell 初始化延迟到后台线程，以保持即时启动。
*   **受限模式：** 禁用 Ruby 集成，以安全执行不受信任的脚本。
*   **Zsh 兼容性：** 支持 `setopt`、`compdef` 和 `RPROMPT`。

Rubish 可以通过 Homebrew 或源代码安装，并可用作交互式 shell、运行脚本或作为登录 shell。它还提供公共 Ruby API，从而实现程序化控制，以便嵌入到其他应用程序中。

---

## 3. 觅悬日：找到太阳何时与你的街道对齐

**原文标题**: Hengefinder: Finding when the sun aligns with your street

**原文链接**: [https://victoriaritvo.com/blog/hengefinder/](https://victoriaritvo.com/blog/hengefinder/)

文章介绍了Hengefinder，一个旨在预测“日行现象”的工具——即太阳与街道完美对齐的时刻，类似于“曼哈顿悬日”。受纽约这一现象的启发，作者试图将这种预测推广到任何地点。

核心过程包括三个步骤：找到道路的方位角（相对于正北方向的角度），确定每天日落时太阳的方位角，以及找出这些角度匹配的日期。作者在将这些看似简单的步骤转化为一个功能性工具时遇到了几个挑战。

一个主要挑战是准确计算道路的方位角。在球形地球上，标准的经纬度差值不再适用，因为经度度数会随着接近两极而缩小。解决方案是使用平均纬度的余弦值来缩放经度，以确保在使用`atan2`计算角度之前单位一致。

另一个挑战是为日行现象定义“日落”。天文学定义（太阳完全在地平线以下）太迟了。相反，作者寻找太阳圆盘完全可见并刚好接触地平线的精确时刻。这通过使用“最后一个真值”的二分查找来解决，以找到太阳高度满足特定阈值的最晚时间。

最后，寻找对齐日期很复杂，因为太阳在日落时的方位角全年并非单调变化。为了避免暴力式的每日检查，采用了两阶段搜索：首先进行粗略的初步扫描（例如每30天一次），以识别可能发生对齐或太阳方向反转的窗口，然后对这些标记的窗口进行细致的逐日搜索，以精确定位具体日期。

该项目催生了Hengefinder网站和一个手机应用（由John Pribyl开发），其中还包括“索伦日行现象”（太阳/月亮与建筑物顶部对齐）。该工具揭示了以前未被注意到的日行现象，例如在阿姆斯特丹古老运河上的那些，这突出表明这些几何上罕见但美丽的对齐现象在全球范围内发生，但往往不为人所知。

---

## 4. 橙县制造工厂有毒化学品泄漏

**原文标题**: Toxic chemical leak at a manufacturing facility in Orange County

**原文链接**: [https://www.bbc.com/news/articles/c3w2l249j8go](https://www.bbc.com/news/articles/c3w2l249j8go)

加利福尼亚州宣布进入紧急状态，因为消防队员正在努力控制橙县加登格罗夫市GKN航空航天制造工厂的有毒化学品泄漏。这一危急情况涉及一个装有约7000加仑甲基丙烯酸甲酯的储罐，甲基丙烯酸甲酯是一种用于塑料的高度挥发性易燃物质，官员警告称该储罐有破裂或爆炸的风险。

数千名加登格罗夫居民已作为预防措施被疏散。最初，官员们担心储罐会泄漏或发生“热失控”并爆炸。然而，周日一个专业团队调查后发现储罐存在“潜在裂缝”，这可能有助于缓解内部压力。

此次事件因一个“无法操作的阀门”以及内部温度显著升高（已达到32摄氏度/90华氏度）而变得复杂。应急人员正持续向储罐喷水，以稳定其温度并减缓化学反应。消防局长克雷格·科维强调：“我们绝不能让它失控爆炸。”

当局正在为所有情况做准备，包括修建堤坝以防止任何泄漏物进入雨水排放系统或海洋。当地学校已关闭，主要道路出口已封闭。卫生官员建议居民报告任何“果味浓郁的气味”，因为吸入其蒸汽可能导致呼吸系统问题、眼睛刺激和头晕。该设施距离迪士尼乐园约5英里，迪士尼乐园仍在疏散区之外并保持开放。

---

## 5. 移民海关执法局授予Bi2科技公司2500万美元虹膜识别合同

**原文标题**: ICE Awards $25M Iris-Scanning Contract to Bi2 Technologies

**原文链接**: [https://www.projectsaltbox.com/p/ice-awards-25-million-iris-scanning](https://www.projectsaltbox.com/p/ice-awards-25-million-iris-scanning)

移民与海关执法局已向Bi2 Technologies授予一份价值2510万美元的无竞标合同，用于采购虹膜扫描生物识别技术并访问生物识别信息系统。该交易于2026年5月22日授予，其规模是该机构此前于2025年9月与这家马萨诸塞州公司签订的460万美元合同的五倍多。

该合同将向移民与海关执法局的执法与遣返行动部门提供1570台设备，相比之前的200台有所增加，使特工能够在外勤行动中快速验证身份。它还允许持续访问Bi2的数据库，其中包含超过500万条入库记录。

值得注意的是，此次采购并未要求处理敏感数据的云系统进行FedRAMP认证，也未强制要求进行独立审计、国会通知或对系统使用方式进行外部审查。这些设备预计将在6月底前交付至移民与海关执法局的各个地点。

---

## 6. Models.dev：AI模型规格、定价与能力开源数据库

**原文标题**: Models.dev: open-source database of AI model specs, pricing, and capabilities

**原文链接**: [https://github.com/anomalyco/models.dev](https://github.com/anomalyco/models.dev)

Models.dev 是一个综合性的开源、社区贡献的AI模型规格、定价和能力数据库，旨在解决缺乏集中式资源的问题。它也由 opencode 内部使用。数据可通过公共API (`https://models.dev/api.json`) 访问，提供商徽标以SVG文件形式提供。

贡献 Models.dev 涉及在项目仓库中添加或更新存储在 TOML 文件（用于提供商和模型）和 SVG 文件（用于徽标）中的数据。要添加新模型，贡献者首先要创建提供商条目（如果尚不存在），包括名称、AI SDK 包、环境变量、文档以及可选的 OpenAI 兼容 API 端点等详细信息。也可以添加 SVG 徽标。

模型定义存储在 TOML 文件中，详细说明了显示名称、对附件、推理、工具调用和结构化输出等功能的支持。它们还指定了温度控制、知识截止日期、发布和更新日期、开放权重状态、token 成本（输入、输出、推理、缓存、音频）、token 限制（上下文、输入、输出）以及支持的输入/输出模态。一个 `extends` 功能允许包装模型重用并覆盖现有规范模型定义中的字段。所有提交都会经过自动模式验证。

开发人员可以使用 Bun 进行前端开发，并通过 opencode 在本地测试更改。Models.dev 由 SST 的创建者维护，通过 Discord、YouTube 和 X.com 促进社区互动。

---

## 7. DeepSeek 旗舰AI模型永久二五折

**原文标题**: DeepSeek to Make Permanent 75% Discount on Flagship AI Model

**原文链接**: [https://www.bloomberg.com/news/articles/2026-05-23/deepseek-to-make-permanent-75-discount-on-flagship-ai-model](https://www.bloomberg.com/news/articles/2026-05-23/deepseek-to-make-permanent-75-discount-on-flagship-ai-model)

无法访问文章链接

---

## 8. Greg Brockman interview [video]

**原文标题**: Greg Brockman interview [video]

**原文链接**: [https://fs.blog/knowledge-project-podcast/greg-brockman/](https://fs.blog/knowledge-project-podcast/greg-brockman/)

生成摘要时出错

---

## 9. Electrobun 2.0 will be decoupled from Bun due to the Rust rewrite

**原文标题**: Electrobun 2.0 will be decoupled from Bun due to the Rust rewrite

**原文链接**: [https://twitter.com/YoavCodes/status/2058064720553222567](https://twitter.com/YoavCodes/status/2058064720553222567)

生成摘要时出错

---

## 10. Omarchy Is Not A Distro

**原文标题**: Omarchy Is Not A Distro

**原文链接**: [https://abyss.fish/your_dotfiles_are_not_a_distro](https://abyss.fish/your_dotfiles_are_not_a_distro)

生成摘要时出错

---

## 11. The seed oil panic is hurting my cardiac patients

**原文标题**: The seed oil panic is hurting my cardiac patients

**原文链接**: [https://www.statnews.com/2026/05/22/seed-oils-healthy-fats-tallow-fact-check-cardiac-health/](https://www.statnews.com/2026/05/22/seed-oils-healthy-fats-tallow-fact-check-cardiac-health/)

生成摘要时出错

---

## 12. DHS Quits Granting Green Cards–Almost

**原文标题**: DHS Quits Granting Green Cards–Almost

**原文链接**: [https://www.cato.org/blog/dhs-quits-granting-green-cards-almost-entirely](https://www.cato.org/blog/dhs-quits-granting-green-cards-almost-entirely)

生成摘要时出错

---

## 13. 'AI washing': firms are scrambling to rebrand themselves as tech-focused

**原文标题**: 'AI washing': firms are scrambling to rebrand themselves as tech-focused

**原文链接**: [https://www.theguardian.com/technology/2026/may/24/ai-washing-pr-firms-scrambling-rebrand](https://www.theguardian.com/technology/2026/may/24/ai-washing-pr-firms-scrambling-rebrand)

生成摘要时出错

---

## 14. TikTok disproportionately served anti-Democratic videos during the 2024 election

**原文标题**: TikTok disproportionately served anti-Democratic videos during the 2024 election

**原文链接**: [https://www.psypost.org/tiktok-disproportionately-served-anti-democratic-videos-during-the-2024-election-study-finds/](https://www.psypost.org/tiktok-disproportionately-served-anti-democratic-videos-during-the-2024-election-study-finds/)

生成摘要时出错

---

## 15. z386: An Open-Source 80386 Built Around Original Microcode

**原文标题**: z386: An Open-Source 80386 Built Around Original Microcode

**原文链接**: [https://nand2mario.github.io/posts/2026/z386/](https://nand2mario.github.io/posts/2026/z386/)

生成摘要时出错

---

## 16. Judson's Last Ride

**原文标题**: Judson's Last Ride

**原文链接**: [https://www.realclearpolitics.com/articles/2026/05/22/judsons_last_ride_154150.html](https://www.realclearpolitics.com/articles/2026/05/22/judsons_last_ride_154150.html)

生成摘要时出错

---

## 17. Usborne 1980s Computer Books

**原文标题**: Usborne 1980s Computer Books

**原文链接**: [https://usborne.com/us/books/computer-and-coding-books](https://usborne.com/us/books/computer-and-coding-books)

生成摘要时出错

---

## 18. Childhood Computing

**原文标题**: Childhood Computing

**原文链接**: [https://susam.net/childhood-computing.html](https://susam.net/childhood-computing.html)

生成摘要时出错

---

## 19. Air France and Airbus found guilty of manslaughter over 2009 plane crash

**原文标题**: Air France and Airbus found guilty of manslaughter over 2009 plane crash

**原文链接**: [https://www.bbc.com/news/articles/czd2qmdvmq6o](https://www.bbc.com/news/articles/czd2qmdvmq6o)

生成摘要时出错

---

## 20. Constraint Decay: The Fragility of LLM Agents in Back End Code Generation

**原文标题**: Constraint Decay: The Fragility of LLM Agents in Back End Code Generation

**原文链接**: [https://arxiv.org/abs/2605.06445](https://arxiv.org/abs/2605.06445)

生成摘要时出错

---

## 21. My I3-Emacs Integration

**原文标题**: My I3-Emacs Integration

**原文链接**: [https://khz.ac/software/i3-integration.html](https://khz.ac/software/i3-integration.html)

生成摘要时出错

---

## 22. Don't Roll Your Own

**原文标题**: Don't Roll Your Own

**原文链接**: [https://susam.net/do-not-roll-your-own.html](https://susam.net/do-not-roll-your-own.html)

生成摘要时出错

---

## 23. Alexander Grothendieck Revolutionized 20th-Century Mathematics

**原文标题**: Alexander Grothendieck Revolutionized 20th-Century Mathematics

**原文链接**: [https://www.quantamagazine.org/how-alexander-grothendieck-revolutionized-20th-century-mathematics-20260520/](https://www.quantamagazine.org/how-alexander-grothendieck-revolutionized-20th-century-mathematics-20260520/)

生成摘要时出错

---

## 24. The C64 Dead Test Font

**原文标题**: The C64 Dead Test Font

**原文链接**: [https://www.masswerk.at/nowgobang/2026/c64-dead-test-font](https://www.masswerk.at/nowgobang/2026/c64-dead-test-font)

生成摘要时出错

---

## 25. Justice Department scrubs its website of news releases about Jan. 6 defendants

**原文标题**: Justice Department scrubs its website of news releases about Jan. 6 defendants

**原文链接**: [https://apnews.com/article/justice-department-capitol-riot-news-releases-purged-29c580044a9ed27b643c99feac9e2964](https://apnews.com/article/justice-department-capitol-riot-news-releases-purged-29c580044a9ed27b643c99feac9e2964)

生成摘要时出错

---

## 26. Ebola Outbreak Now Third Largest Recorded and "Spreading Rapidly"

**原文标题**: Ebola Outbreak Now Third Largest Recorded and "Spreading Rapidly"

**原文链接**: [https://arstechnica.com/health/2026/05/ebola-outbreak-now-third-largest-recorded-and-spreading-rapidly/](https://arstechnica.com/health/2026/05/ebola-outbreak-now-third-largest-recorded-and-spreading-rapidly/)

生成摘要时出错

---

## 27. Mastering Dyalog APL

**原文标题**: Mastering Dyalog APL

**原文链接**: [https://mastering.dyalog.com/README.html](https://mastering.dyalog.com/README.html)

生成摘要时出错

---

## 28. 'Fuck you, Bambu': How one private message could change the face of 3D printing

**原文标题**: 'Fuck you, Bambu': How one private message could change the face of 3D printing

**原文链接**: [https://www.theverge.com/tech/931532/bambu-agpl-pawel-jarczak-open-source-threat-dmca-github](https://www.theverge.com/tech/931532/bambu-agpl-pawel-jarczak-open-source-threat-dmca-github)

生成摘要时出错

---

## 29. Reverse engineering circuitry in a Spacelab computer from 1980

**原文标题**: Reverse engineering circuitry in a Spacelab computer from 1980

**原文链接**: [https://www.righto.com/2026/05/reverse-engineering-spacelab-computer.html](https://www.righto.com/2026/05/reverse-engineering-spacelab-computer.html)

生成摘要时出错

---

## 30. Claude Is Not Your Architect. Stop Letting It Pretend

**原文标题**: Claude Is Not Your Architect. Stop Letting It Pretend

**原文链接**: [https://www.hollandtech.net/claude-is-not-your-architect/](https://www.hollandtech.net/claude-is-not-your-architect/)

生成摘要时出错

---

