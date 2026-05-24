# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-05-24.md)

*最后自动更新时间: 2026-05-24 20:22:25*
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

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 2 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 3 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 4 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 5 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 6 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 7 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 8 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 9 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 10 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 11 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 12 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 13 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 14 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 15 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 16 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 17 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 18 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 19 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 20 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 21 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 22 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 23 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 24 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 25 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 26 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 27 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 28 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 29 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 30 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 31 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 32 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 33 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 34 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 35 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 36 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 37 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 38 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 39 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 40 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 41 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 42 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 43 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 44 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 45 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 46 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 47 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 48 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 49 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 50 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 51 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 52 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 53 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 54 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 55 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 56 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 57 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 58 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 59 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 60 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 61 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 62 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 63 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 64 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 65 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 66 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 67 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 68 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 69 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 70 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 71 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 72 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 73 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 74 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 75 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 76 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 77 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 78 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 79 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 80 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 81 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 82 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 83 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 84 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 85 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 86 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 87 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 88 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 89 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 90 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 91 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 92 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 93 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 94 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 95 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 96 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 97 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 98 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 99 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 100 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 101 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 102 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 103 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 104 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 105 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 106 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 107 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 108 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 109 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 110 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 111 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 112 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 113 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 114 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 115 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 116 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 117 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 118 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 119 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 120 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 121 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 122 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 123 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 124 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 125 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 126 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 127 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 128 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 129 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 130 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 131 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 132 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 133 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 134 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 135 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 136 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 137 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 138 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 139 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 140 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 141 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 142 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 143 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 144 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 145 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 146 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 147 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 148 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 149 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 150 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 151 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 152 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 153 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 154 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 155 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 156 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 157 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 158 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 159 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 160 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 161 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 162 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 163 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 164 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 165 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 166 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 167 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 168 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 169 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 170 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 171 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 172 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 173 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 174 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 175 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 176 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 177 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 178 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 179 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 180 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 181 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 182 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 183 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 184 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 185 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 186 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 187 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 188 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 189 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 190 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 191 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 192 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 193 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 194 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 195 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 196 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 197 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 198 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
