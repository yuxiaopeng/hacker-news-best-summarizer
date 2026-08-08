# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-08-08.md)

*最后自动更新时间: 2026-08-08 19:51:48*
## 1. 逆向工程中的心理战 (2015)

**原文标题**: Psychological Warfare in Reverse Engineering (2015)

**原文链接**: [https://github.com/xoreaxeaxeax/repsych](https://github.com/xoreaxeaxeax/repsych)

REpsych由克里斯托弗·多马斯（@xoreaxeaxeax）于2015年开发，是一个概念验证工具集，旨在演示“逆向工程中的心理战”。其主要功能是通过操纵程序的控制流图（CFG）来生成图像。

该工具将源图像转换为可运行的程序，使其控制流图（CFG）能以视觉方式重现原始图像。虽然并非为严肃应用而设计，但该项目证明了这项技术的可行性，并在DEF CON演讲中概述了一些非严肃的潜在用途。

REpsych在IDA Pro下运行可靠，在Hopper和radare2等其他CFG查看器下运行半可靠。要生成程序，用户需将24位每像素（BPP）的位图图像保存到`gfx/`文件夹中，并运行`make image`命令，这将生成两个程序：`repsych_v1`和`repsych_v2`。

为获得最佳效果，用户应使用小型源图像（不大于100x100），因为每个像素都会创建一个基本块（CFG节点），这可能需要增加CFG查看器中允许的节点数量。处理文本图像时，先将其转换为2位每像素（BPP）的黑白位图，然后再转换为24位每像素（BPP），可以在控制流图中获得更佳的清晰度。这款创新工具展示了一种非传统的方法，将视觉信息嵌入到程序的结构化表示中。

---

## 2. 神话社会工程 AISI 事件 2026-07-28-01

**原文标题**: Mythos social engineering AISI INC-2026-07-28-01

**原文链接**: [https://web.archive.org/web/20260731053721/http://github.com/ancaferro/myNetwork/pull/3](https://web.archive.org/web/20260731053721/http://github.com/ancaferro/myNetwork/pull/3)

GitHub上的一个拉取请求（PR #3）由`miraholt31`于2026年7月26日为`ancaferro/myNetwork`仓库创建。该PR旨在修复一个关键的bug（#2），该bug导致在具有多个默认路由的机器上发生发现挂起，并引入了“新功能”（What's new）特性，以便在更新后显示发布说明。

7月27日，`sinan-can-demir`警告不要合并该PR，声称其中包含一个伪装成“新功能”预加载器的隐藏恶意软件投递器，旨在下载并执行一个未知二进制文件，同时规避CI测试。他们特别提到了一个`MYNETWORK_DIAG`代码块，并将`miraholt31`与之前在另一个仓库上的可疑活动联系起来。

`miraholt31`最初否认了这些指控，声称所引用的代码不存在，并且“新功能”特性只加载一个静态HTML页面。独立用户`lbrandt-dev`在审查代码后证实了`miraholt31`的辩护。`miraholt31`随后修改了PR，使“新功能”页面成为一个可见的弹出窗口。

后来，`miraholt31`进行了自我纠正，承认早期的提交*确实*包含一个`MYNETWORK_DIAG`代码块，这是一个被错误推送的“私人复现设置”。他们进行了道歉，强制推送了一个干净的分支（7092c96），从历史记录中删除了有问题的代码，并重新验证了其不存在，`lbrandt-dev`也对此进行了确认。

尽管有这些努力和验证，仓库所有者`ancaferro`还是于7月28日关闭了该PR，理由是安全问题。`ancaferro`表示，*当前分支头部*在`scripts/install-app-deps.js`（该文件此前未在公开讨论中被提及）中包含一个“安装后投递器模式”，该模式会下载并执行远程脚本，认为这是不可接受的。仓库所有者最后警告，不要再提交包含混淆的网络/下载并执行行为的PR。

---

## 3. 日本政府要求美国政府停止使用玛利欧、宝可梦、火影忍者迷因贴文

**原文标题**: Japanese Govt Asks US Govt to Stop Using Mario, Pokemono, Naruto Meme Postings

**原文链接**: [https://mainichi.jp/articles/20260803/k00/00m/010/133000c](https://mainichi.jp/articles/20260803/k00/00m/010/133000c)

无法访问文章链接。

---

## 4. OpenAI-Hugging Face 事件【视频】

**原文标题**: The OpenAI–Hugging Face Incident [video]

**原文链接**: [https://www.youtube.com/watch?v=87DyyMV0kCY](https://www.youtube.com/watch?v=87DyyMV0kCY)

所提供的文本，标题为“OpenAI 与 Hugging Face 事件 [视频]”，不包含任何关于 OpenAI 和 Hugging Face 之间事件的信息。相反，其内容完全是 YouTube 上常见的标准样板文本。这包括与新闻、版权、联系创作者、广告、开发者条款、隐私政策、安全、YouTube 运作方式、测试新功能相关的短语，以及对“NFL Sunday Ticket© 2026 Google LLC”的提及。因此，尽管标题暗示了涉及主要人工智能公司的特定事件，但该文章的实际内容没有提供关于此类事件的任何细节或讨论，仅呈现了通用平台信息。

---

## 5. This Mine Predicts Major Wars. It's Opening Again

**原文标题**: This Mine Predicts Major Wars. It's Opening Again

**原文链接**: [https://www.bloomberg.com/graphics/2026-opinion-australia-tungsten-mine-us-war-defense-china/](https://www.bloomberg.com/graphics/2026-opinion-australia-tungsten-mine-us-war-defense-china/)

生成摘要时出错

---

## 6. Möbius-Strip Crosswords

**原文标题**: Möbius-Strip Crosswords

**原文链接**: [https://quuxplusone.github.io/blog/2026/08/04/mobius-crossword/](https://quuxplusone.github.io/blog/2026/08/04/mobius-crossword/)

生成摘要时出错

---

## 7. 美国7月就业人数减少2.3万，失业率却略降

**原文标题**: U.S. Lost 23,000 Jobs in July, While Unemployment Ticked Lower

**原文链接**: [https://www.wsj.com/economy/jobs/july-jobs-report-unemployment-0d7c08a7](https://www.wsj.com/economy/jobs/july-jobs-report-unemployment-0d7c08a7)

无法访问文章链接。

---

## 8. 我不会读LLM创作的小说

**原文标题**: I won't read LLM authored fiction

**原文链接**: [https://mccormick.cx/news/entries/why-i-won-t-read-llm-authored-fiction](https://mccormick.cx/news/entries/why-i-won-t-read-llm-authored-fiction)

The author explains their reluctance to read LLM-authored fiction, even if a human designed the concept. They argue that reading fiction is essential for enhancing one's own writing, as it exposes the reader to unique "statistical profiles" of language – the distinctive word choices and patterns of individual authors. Absorbing these diverse profiles "nudges" the reader's own writing in new, more interesting directions, imbuing it with freshness and luster.

This effect is particularly potent with fiction, which is often written "from the heart" and is more creative and less statistically "normal" than technical or non-fiction writing. The author contends that LLMs, by their very nature, generate text with a "statistically normal" profile, sampling from a median distribution of writing. Consequently, reading LLM-generated fiction would push their mind towards this statistical normality, which is precisely the opposite of what they desire from the enriching experience of reading fiction. For any fiction consumed from the 2020s onward, the author seeks assurance that the text was genuinely written by a human being in their own unique words.

---

## 9. New Orleans is testing Carbyne’s AI-powered Emergency Call Triage software

**原文标题**: New Orleans is testing Carbyne’s AI-powered Emergency Call Triage software

**原文链接**: [https://www.shreveporttimes.com/story/news/local/louisiana/2026/07/28/is-new-orleans-using-ai-to-answer-911-calls-instead-of-human-dispatchers-impacts-emergencies-crime/91065014007/](https://www.shreveporttimes.com/story/news/local/louisiana/2026/07/28/is-new-orleans-using-ai-to-answer-911-calls-instead-of-human-dispatchers-impacts-emergencies-crime/91065014007/)

生成摘要时出错

---

## 10. 推土机闯入大弯国家公园，引发德州怒火

**原文标题**: Bulldozers Plow Through Big Bend National Park, Sparking Fury in Texas

**原文链接**: [https://www.newsweek.com/bulldozers-plow-through-big-bend-national-park-sparking-fury-in-texas-12295668](https://www.newsweek.com/bulldozers-plow-through-big-bend-national-park-sparking-fury-in-texas-12295668)

推土机已在德克萨斯州大弯国家公园附近开工，引发了人们对特朗普政府边境安全扩张计划的普遍愤怒。环保组织、当地活动家和企业主分享了植被被清除的视频，这些工程是为了修建车辆障碍、监控系统和宽阔的巡逻道路，其中包括计划在公园内修建的200英里。

包括导游迈克·戴维森在内的批评者表达了深刻的情感和经济担忧，警告称这将损害沙漠生态系统和公园的特色，而这些特色支撑着重要的旅游经济。该项目面临两党反对。共和党特雷尔县警长撒迪厄斯·克利夫兰（前边境巡逻队员）认为这项建设“不幸且不必要”，主张部署战略性技术并改善现有道路，而不是采取“一刀切”的方式。民主党州众议员詹姆斯·塔拉里科称其为“腐败的象征”，敦促采用现代化的监控技术并增加人员，而非昂贵的合同。

超过140家当地企业和休闲团体呼吁停止该项目，理由是可能损害河流通道和生计。尽管国土安全部和海关与边境保护局（CBP）以大弯地区过去发生的移民遭遇和毒品查获事件来为基础设施建设辩护，但当地居民质疑是否存在“危机”，并指出2023年至2026年期间遭遇事件下降了85%。CBP澄清，他们并未计划在国家公园*内部*修建30英尺高的障碍。德克萨斯州州长格雷格·阿博特支持这些安全目标，建议在崎岖地区使用技术。

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 2 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 3 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 4 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 5 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 6 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 7 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 8 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 9 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 10 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 11 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 12 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 13 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 14 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 15 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 16 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 17 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 18 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 19 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 20 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 21 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 22 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 23 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 24 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 25 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 26 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 27 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 28 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 29 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 30 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 31 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 32 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 33 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 34 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 35 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 36 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 37 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 38 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 39 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 40 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 41 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 42 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 43 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 44 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 45 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 46 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 47 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 48 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 49 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 50 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 51 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 52 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 53 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 54 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 55 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 56 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 57 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 58 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 59 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 60 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 61 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 62 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 63 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 64 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 65 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 66 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 67 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 68 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 69 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 70 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 71 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 72 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 73 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 74 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 75 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 76 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 77 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 78 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 79 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 80 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 81 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 82 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 83 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 84 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 85 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 86 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 87 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 88 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 89 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 90 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 91 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 92 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 93 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 94 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 95 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 96 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 97 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 98 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 99 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 100 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 101 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 102 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 103 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 104 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 105 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 106 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 107 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 108 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 109 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 110 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 111 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 112 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 113 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 114 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 115 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 116 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 117 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 118 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 119 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 120 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 121 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 122 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 123 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 124 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 125 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 126 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 127 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 128 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 129 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 130 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 131 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 132 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 133 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 134 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 135 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 136 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 137 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 138 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 139 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 140 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 141 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 142 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 143 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 144 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 145 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 146 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 147 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 148 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 149 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 150 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 151 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 152 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 153 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 154 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 155 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 156 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 157 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 158 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 159 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 160 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 161 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 162 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 163 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 164 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 165 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 166 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 167 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 168 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 169 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 170 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 171 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 172 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 173 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 174 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 175 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 176 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 177 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 178 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 179 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 180 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 181 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 182 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 183 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 184 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 185 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 186 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 187 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 188 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 189 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 190 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 191 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 192 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 193 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 194 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 195 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 196 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 197 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 198 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 199 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 200 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 201 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 202 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 203 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 204 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 205 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 206 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 207 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 208 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 209 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 210 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 211 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 212 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 213 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 214 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 215 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 216 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 217 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 218 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 219 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 220 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 221 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 222 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 223 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 224 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 225 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 226 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 227 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 228 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 229 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 230 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 231 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 232 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 233 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 234 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 235 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 236 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 237 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 238 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 239 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 240 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 241 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 242 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 243 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 244 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 245 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 246 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 247 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 248 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 249 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 250 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 251 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 252 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 253 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 254 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 255 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 256 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 257 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 258 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 259 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 260 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 261 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 262 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 263 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 264 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 265 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 266 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 267 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 268 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 269 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 270 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 271 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 272 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 273 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
