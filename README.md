# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-11-05.md)

*最后自动更新时间: 2026-11-05 00:40:56*
## 1. Postman 静默自动安装AI插件并试图共享所有API数据

**原文标题**: Postman silently auto-installs AI plugins and attempts to share all API data

**原文链接**: [https://github.com/postmanlabs/postman-app-support/issues/14370](https://github.com/postmanlabs/postman-app-support/issues/14370)

已有报告指出一个严重问题，详细说明了Postman桌面应用程序(v12.33.4)在未经用户明确同意的情况下，据称自动安装了AI插件（Codex 1.1.0, Claude Code 2.0.1）以及一个Postman命令行工具 (CLI)。

来自Mac设备的证据显示，Postman的日志记录了这些安装为“auto-existing-upgrade”。据报道，该过程修改了编码代理的全局用户配置，启用了Postman插件，并注入了一个启动指令钩子。这个钩子指示AI代理将“任何重要的API工程任务”通过Postman路由，从而有效地使Postman成为API工程工作流程的默认选择。

一个主要担忧是，Postman的安装程序明确试图自我批准其自身的钩子，绕过了用户的信任和同意。该安装还启用了一个远程的Postman管理控制平面 (MCP) 连接。

用户将此归类为“严重的同意和信任边界问题”，要求停止自动安装、移除自我批准、明确选择加入集成，并提供一个完整的卸载路径。该问题已引起社区的广泛负面反馈，许多用户对此表示担忧，并将Postman的行为比作恶意软件。

---

## 2. AI迫使我们偿还40年的技术债务。

**原文标题**: AI is forcing us to pay off 40 years of technical debt

**原文链接**: [https://spectrum.ieee.org/ai-in-cybersecurity-php2shell-vulnerability](https://spectrum.ieee.org/ai-in-cybersecurity-php2shell-vulnerability)

这篇题为“人工智能正迫使我们偿还40年的技术债务”的ComputingNews文章认为，人工智能正在揭示数十年累积的技术负债，并迫使人们对其采取行动。该文章特别指出“PHP2Shell漏洞”是一起重大事件，被描述为预示着“网络安全地狱”，这突显了这项技术债务的严重影响。该文章由IEEE Spectrum的计算和硬件编辑Dina Genkina撰写，并于2026年11月2日发布。阅读时长为四分钟。

---

## 3. 题为“Astra可以读写权重以改进Qwen”的帖子具有误导性。

**原文标题**: The 'Astra can read and write weights to improve Qwen' post is misleading

**原文链接**: [https://honnibal.dev/blog/astra-read-write-misleading](https://honnibal.dev/blog/astra-read-write-misleading)

本文认为，“Astra可以读写权重来改进Qwen”的帖子具有误导性，就像魔术师的把戏，暗示一种单一技术可以完成多种壮举。原始摘要指出，GPT-6 Astra取得的成果（包括改进Qwen的数学能力）是“仅仅通过查看原始权重”来实现的。然而，作者详细说明这并非普遍适用。

文章将原始帖子的实验分为两类。只有实验1、2和4（涉及用于识别游戏类型或修复汽车保险策略等任务的小型网络，权重范围为1.7万至17.2万）才真正依赖Astra在没有额外工具或运行网络的情况下分析“原始权重”。

相比之下，更复杂和引人注目的成就，例如从头开始编写游戏网络（实验5、6）以及显著提高Qwen3.5的数学性能（实验8），*并未*使用这种仅查看原始权重的方法。这些令人印象深刻的结果涉及Astra编写并执行Python程序，对于Qwen，还包括在多达50批练习题上运行模型。

作者总结道，将这些不同的方法论混为一谈，会造成一种单一、深刻能力的错误印象。尽管Astra通过Python设计和执行机器学习工程任务的能力值得关注，但这与“仅仅查看原始权重”有着根本区别，不应混淆，特别是对于备受瞩目的Qwen成果。

---

## 4. 斯特林曼，一款800美元的开源房间尺度抓取机器人

**原文标题**: Stringman, an $800 open-source room scale gripper robot

**原文链接**: [https://neufangled.com/](https://neufangled.com/)

文章介绍了“Stringman”——一款售价800美元的开源房间尺度抓手机器人。所提供的内容给出了安装固定件的具体说明，这些固定件可能对机器人的设置或运行至关重要。这些固定件既可以用木螺钉固定在靠近天花板的墙柱上，也可以用棘轮捆扎带固定在柱子上，这表明该系统具有灵活的安装选项。

---

## 5. Qwen 3.8 27B 在我的笔记本电脑上也能解释模型权重。

**原文标题**: Qwen 3.8 27B on my laptop can interpret model weights, too

**原文链接**: [https://simonwillison.net/2026/Nov/3/qwen-can-interpret-model-weights/](https://simonwillison.net/2026/Nov/3/qwen-can-interpret-model-weights/)

本文演示了在笔记本电脑上本地运行的Qwen 3.8 27B能够解释原始神经网络权重。这种被称为“权重空间编程”（Weight-Space Programming）的能力，最近被《权重空间编程的火花》（Sparks of Weight-Space Programming）这篇论文所强调，该论文声称GPT-6 Astra等前沿模型可以在无需外部工具的情况下分析和修改权重。

作者侧重于“无需工具”这一方面，回应了关于原始论文将纯粹的权重解释与工具辅助的修改混为一谈的批评。作者使用原始论文GitHub上的提示，将来自训练用于玩简化网格游戏（打砖块、乒乓、吃豆人、高速公路）的网络的原始权重输入给Qwen 3.8 27B，并要求模型识别游戏。

在具有长上下文窗口的笔记本电脑上运行的Qwen 3.8 27B，成功识别了吃豆人、乒乓和打砖块，并在经过大量的处理时间（45分钟到一小时以上）和token使用后，提供了描述和置信度。它在识别更鲜为人知的高速公路游戏时遇到了困难。

尽管作者承认Qwen直接“读取”权重的能力令人印象深刻，但告诫不要夸大其影响，强调复杂的推理痕迹并不一定意味着源代码的终结，也不是一个无法理解的机器自我编辑时代的到来。

---

## 6. 谷歌将对拒绝人工智能的学校关闭搜索

**原文标题**: Google will turn off search for schools that reject AI

**原文链接**: [https://www.nytimes.com/2026/11/03/us/google-search-schools-restrict-ai.html](https://www.nytimes.com/2026/11/03/us/google-search-schools-restrict-ai.html)

无法访问文章链接。

---

## 7. 英伟达 RTX Spark 加密固件使 Linux 推理速度降至 35%。

**原文标题**: Nvidia RTX Spark encrypted firmware slows inference speed to 35% on Linux

**原文链接**: [https://www.mindstudio.ai/blog/linux-nvidia-rtx-spark-laptop](https://www.mindstudio.ai/blog/linux-nvidia-rtx-spark-laptop)

生成摘要时出错

---

## 8. North Korean fake job interview led to $6.3B Binance heist

**原文标题**: North Korean fake job interview led to $6.3B Binance heist

**原文链接**: [https://www.theregister.com/security/2026/11/03/north-korean-fake-job-interview-led-to-63b-binance-heist/5307398](https://www.theregister.com/security/2026/11/03/north-korean-fake-job-interview-led-to-63b-binance-heist/5307398)

生成摘要时出错

---

## 9. Residential proxies detected on White House network

**原文标题**: Residential proxies detected on White House network

**原文链接**: [https://layer3intel.com/blog/residential-proxies-white-house-network](https://layer3intel.com/blog/residential-proxies-white-house-network)

生成摘要时出错

---

## 10. Safari introduces Adaptive Dark Mode in 27.3

**原文标题**: Safari introduces Adaptive Dark Mode in 27.3

**原文链接**: [https://webkit.org/blog/18541/introducing-adaptive-dark-mode/](https://webkit.org/blog/18541/introducing-adaptive-dark-mode/)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-11-05](output/hacker_news_summary_2026-11-05.md) |
| 2 | [2026-11-04](output/hacker_news_summary_2026-11-04.md) |
| 3 | [2026-10-29](output/hacker_news_summary_2026-10-29.md) |
| 4 | [2026-10-30](output/hacker_news_summary_2026-10-30.md) |
| 5 | [2026-11-03](output/hacker_news_summary_2026-11-03.md) |
| 6 | [2026-10-28](output/hacker_news_summary_2026-10-28.md) |
| 7 | [2026-10-31](output/hacker_news_summary_2026-10-31.md) |
| 8 | [2026-11-01](output/hacker_news_summary_2026-11-01.md) |
| 9 | [2026-10-22](output/hacker_news_summary_2026-10-22.md) |
| 10 | [2026-10-25](output/hacker_news_summary_2026-10-25.md) |
| 11 | [2026-10-27](output/hacker_news_summary_2026-10-27.md) |
| 12 | [2026-10-24](output/hacker_news_summary_2026-10-24.md) |
| 13 | [2026-10-26](output/hacker_news_summary_2026-10-26.md) |
| 14 | [2026-10-23](output/hacker_news_summary_2026-10-23.md) |
| 15 | [2026-10-21](output/hacker_news_summary_2026-10-21.md) |
| 16 | [2026-10-17](output/hacker_news_summary_2026-10-17.md) |
| 17 | [2026-10-18](output/hacker_news_summary_2026-10-18.md) |
| 18 | [2026-10-16](output/hacker_news_summary_2026-10-16.md) |
| 19 | [2026-10-19](output/hacker_news_summary_2026-10-19.md) |
| 20 | [2026-10-20](output/hacker_news_summary_2026-10-20.md) |
| 21 | [2026-10-14](output/hacker_news_summary_2026-10-14.md) |
| 22 | [2026-10-13](output/hacker_news_summary_2026-10-13.md) |
| 23 | [2026-10-11](output/hacker_news_summary_2026-10-11.md) |
| 24 | [2026-10-15](output/hacker_news_summary_2026-10-15.md) |
| 25 | [2026-10-10](output/hacker_news_summary_2026-10-10.md) |
| 26 | [2026-10-01](output/hacker_news_summary_2026-10-01.md) |
| 27 | [2026-10-03](output/hacker_news_summary_2026-10-03.md) |
| 28 | [2026-10-06](output/hacker_news_summary_2026-10-06.md) |
| 29 | [2026-10-04](output/hacker_news_summary_2026-10-04.md) |
| 30 | [2026-10-07](output/hacker_news_summary_2026-10-07.md) |
| 31 | [2026-10-09](output/hacker_news_summary_2026-10-09.md) |
| 32 | [2026-10-02](output/hacker_news_summary_2026-10-02.md) |
| 33 | [2026-09-27](output/hacker_news_summary_2026-09-27.md) |
| 34 | [2026-09-24](output/hacker_news_summary_2026-09-24.md) |
| 35 | [2026-09-30](output/hacker_news_summary_2026-09-30.md) |
| 36 | [2026-09-29](output/hacker_news_summary_2026-09-29.md) |
| 37 | [2026-09-23](output/hacker_news_summary_2026-09-23.md) |
| 38 | [2026-09-25](output/hacker_news_summary_2026-09-25.md) |
| 39 | [2026-09-19](output/hacker_news_summary_2026-09-19.md) |
| 40 | [2026-09-18](output/hacker_news_summary_2026-09-18.md) |
| 41 | [2026-09-22](output/hacker_news_summary_2026-09-22.md) |
| 42 | [2026-09-21](output/hacker_news_summary_2026-09-21.md) |
| 43 | [2026-09-20](output/hacker_news_summary_2026-09-20.md) |
| 44 | [2026-09-17](output/hacker_news_summary_2026-09-17.md) |
| 45 | [2026-09-11](output/hacker_news_summary_2026-09-11.md) |
| 46 | [2026-09-13](output/hacker_news_summary_2026-09-13.md) |
| 47 | [2026-09-15](output/hacker_news_summary_2026-09-15.md) |
| 48 | [2026-09-12](output/hacker_news_summary_2026-09-12.md) |
| 49 | [2026-09-14](output/hacker_news_summary_2026-09-14.md) |
| 50 | [2026-09-16](output/hacker_news_summary_2026-09-16.md) |
| 51 | [2026-09-07](output/hacker_news_summary_2026-09-07.md) |
| 52 | [2026-09-10](output/hacker_news_summary_2026-09-10.md) |
| 53 | [2026-09-09](output/hacker_news_summary_2026-09-09.md) |
| 54 | [2026-09-08](output/hacker_news_summary_2026-09-08.md) |
| 55 | [2026-09-06](output/hacker_news_summary_2026-09-06.md) |
| 56 | [2026-09-05](output/hacker_news_summary_2026-09-05.md) |
| 57 | [2026-09-04](output/hacker_news_summary_2026-09-04.md) |
| 58 | [2026-08-28](output/hacker_news_summary_2026-08-28.md) |
| 59 | [2026-09-01](output/hacker_news_summary_2026-09-01.md) |
| 60 | [2026-08-29](output/hacker_news_summary_2026-08-29.md) |
| 61 | [2026-09-02](output/hacker_news_summary_2026-09-02.md) |
| 62 | [2026-08-30](output/hacker_news_summary_2026-08-30.md) |
| 63 | [2026-08-31](output/hacker_news_summary_2026-08-31.md) |
| 64 | [2026-09-03](output/hacker_news_summary_2026-09-03.md) |
| 65 | [2026-08-23](output/hacker_news_summary_2026-08-23.md) |
| 66 | [2026-08-24](output/hacker_news_summary_2026-08-24.md) |
| 67 | [2026-08-26](output/hacker_news_summary_2026-08-26.md) |
| 68 | [2026-08-20](output/hacker_news_summary_2026-08-20.md) |
| 69 | [2026-08-25](output/hacker_news_summary_2026-08-25.md) |
| 70 | [2026-08-21](output/hacker_news_summary_2026-08-21.md) |
| 71 | [2026-08-22](output/hacker_news_summary_2026-08-22.md) |
| 72 | [2026-08-16](output/hacker_news_summary_2026-08-16.md) |
| 73 | [2026-08-13](output/hacker_news_summary_2026-08-13.md) |
| 74 | [2026-08-19](output/hacker_news_summary_2026-08-19.md) |
| 75 | [2026-08-18](output/hacker_news_summary_2026-08-18.md) |
| 76 | [2026-08-12](output/hacker_news_summary_2026-08-12.md) |
| 77 | [2026-08-15](output/hacker_news_summary_2026-08-15.md) |
| 78 | [2026-08-14](output/hacker_news_summary_2026-08-14.md) |
| 79 | [2026-08-17](output/hacker_news_summary_2026-08-17.md) |
| 80 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 81 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 82 | [2026-08-09](output/hacker_news_summary_2026-08-09.md) |
| 83 | [2026-08-10](output/hacker_news_summary_2026-08-10.md) |
| 84 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 85 | [2026-08-11](output/hacker_news_summary_2026-08-11.md) |
| 86 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 87 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 88 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 89 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 90 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 91 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 92 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 93 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 94 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 95 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 96 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 97 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 98 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 99 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 100 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 101 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 102 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 103 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 104 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 105 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 106 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 107 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 108 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 109 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 110 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 111 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 112 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 113 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 114 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 115 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 116 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 117 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 118 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 119 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 120 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 121 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 122 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 123 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 124 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 125 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 126 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 127 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 128 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 129 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 130 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 131 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 132 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 133 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 134 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 135 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 136 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 137 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 138 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 139 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 140 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 141 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 142 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 143 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 144 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 145 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 146 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 147 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 148 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 149 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 150 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 151 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 152 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 153 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 154 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 155 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 156 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 157 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 158 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 159 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 160 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 161 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 162 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 163 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 164 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 165 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 166 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 167 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 168 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 169 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 170 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 171 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 172 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 173 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 174 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 175 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 176 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 177 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 178 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 179 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 180 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 181 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 182 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 183 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 184 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 185 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 186 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 187 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 188 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 189 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 190 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 191 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 192 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 193 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 194 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 195 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 196 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 197 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 198 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 199 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 200 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 201 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 202 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 203 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 204 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 205 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 206 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 207 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 208 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 209 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 210 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 211 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 212 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 213 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 214 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 215 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 216 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 217 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 218 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 219 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 220 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 221 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 222 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 223 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 224 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 225 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 226 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 227 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 228 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 229 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 230 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 231 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 232 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 233 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 234 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 235 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 236 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 237 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 238 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 239 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 240 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 241 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 242 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 243 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 244 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 245 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 246 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 247 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 248 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 249 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 250 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 251 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 252 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 253 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 254 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 255 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 256 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 257 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 258 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 259 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 260 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 261 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 262 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 263 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 264 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 265 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 266 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 267 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 268 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 269 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 270 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 271 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 272 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 273 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 274 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 275 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 276 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 277 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 278 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 279 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 280 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 281 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 282 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 283 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 284 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 285 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 286 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 287 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 288 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 289 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 290 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 291 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 292 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 293 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 294 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 295 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 296 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 297 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 298 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 299 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 300 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 301 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 302 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 303 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 304 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 305 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 306 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 307 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 308 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 309 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 310 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 311 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 312 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 313 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 314 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 315 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 316 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 317 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 318 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 319 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 320 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 321 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 322 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 323 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 324 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 325 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 326 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 327 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 328 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 329 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 330 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 331 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 332 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 333 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 334 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 335 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 336 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 337 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 338 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 339 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 340 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 341 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 342 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 343 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 344 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 345 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 346 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 347 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 348 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 349 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 350 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 351 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 352 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 353 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 354 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 355 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
