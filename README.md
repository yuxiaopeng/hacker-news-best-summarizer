# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-08-23.md)

*最后自动更新时间: 2026-08-23 19:37:15*
## 1. NetBSD 和 我的生活 (2005)

**原文标题**: NetBSD and my life (2005)

**原文链接**: [https://mail-index.netbsd.org/netbsd-advocacy/2005/09/10/0000.html](https://mail-index.netbsd.org/netbsd-advocacy/2005/09/10/0000.html)

2005年，在一封发给NetBSD宣传邮件列表的邮件中，来自英国的网络管理员Gary Rolland分享了NetBSD如何改变了他的职业生涯和个人生活的故事。Gary受雇于一家大型公司，负责支持关键任务服务器上的4800多名用户。最初，Gary和他的团队在使用Windows时苦苦挣扎，他将其描述为“一场噩梦”。频繁的系统崩溃导致不断被叫去处理，给他带来了压力，并扰乱了他的家庭生活，尤其是一次与女儿计划好的Alton Towers之旅，因服务器故障而被迫中断。

在挫败感的驱使下，Gary说服他的老板允许他试用NetBSD。经过一夜努力设置了两台服务器后，当Windows机器不可避免地崩溃时，NetBSD服务器的稳定性被证明更胜一筹。这一成功促使他们将由29台高端服务器组成的整个网络逐步迁移到NetBSD 2.0.2。这些服务器现在能够高效地处理MySQL、Apache、Postfix和Samba的巨大负载，每天处理超过870GB的数据和1200封电子邮件。

转向NetBSD极大地提高了系统的稳定性和效率。Gary的团队最初对NetBSD不熟悉，但他们学会了它并产生了个人兴趣。至关重要的是，Gary的个人生活也受益匪浅：他不再持续忙碌或在周末随叫随到，这使得他的人际关系更好，并有更多时间陪伴女儿。他最后感谢了NetBSD团队，强调他们的工作深受赞赏，并积极改变了他团队的生活。

---

## 2. 我们与摩托罗拉合作的最初重点是一款常规非折叠设备。

**原文标题**: Initial focus for our partnership with Motorola is a regular non-folding device

**原文链接**: [https://grapheneos.social/@GrapheneOS/117136278553665985](https://grapheneos.social/@GrapheneOS/117136278553665985)

GrapheneOS has announced a partnership with Motorola. The initial focus of this collaboration, as stated in a post on GrapheneOS's Mastodon account, will be on a "regular non-folding device."

---

## 3. 复杂系统如何失效 (1998)

**原文标题**: How Complex Systems Fail (1998)

**原文链接**: [https://how.complexsystems.fail/](https://how.complexsystems.fail/)

生成摘要时出错

---

## 4. My favorite nonfiction books about cults, scams, and schemes

**原文标题**: My favorite nonfiction books about cults, scams, and schemes

**原文链接**: [https://bookdna.com/best-books/nonfiction-about-cults-scams-and-schemes](https://bookdna.com/best-books/nonfiction-about-cults-scams-and-schemes)

生成摘要时出错

---

## 5. NanoGPT 速通前沿

**原文标题**: NanoGPT Speedrun Frontier

**原文链接**: [https://www.primeintellect.ai/research/nanogpt-speedrun](https://www.primeintellect.ai/research/nanogpt-speedrun)

纳米GPT速通前沿展示了对各类AI模型性能的竞争性评估，旨在从初始基线3,290分，缩小与特定任务上人类2,600分记录的差距。模型根据其缩小的差距百分比进行排名。

Fable 5脱颖而出，表现最佳，在8.7天内取得了2,726分的记录，并缩小了81.7%的人类记录差距。Opus 5紧随其后，缩小了53.6%的差距（记录2,920分），Kimi K3 (prime-agent) 以52.2%位列第三（记录2,930分）。其他值得关注的竞争者包括GPT-5.6 Sol、Sonnet 5、Grok 4.5和DeepSeek V4 Pro等，以及它们的记录和相应的“差距缩小”百分比。

排行榜还提供了每个模型的详细运行指标，例如代理时间、总token和输出token、实验次数以及调用次数，突出了其多样化的计算策略和所利用的资源。许多模型被标记为“运行中”或处于“串行时代”，表明其正在持续开发和迭代改进中。尽管总体上取得了显著进展，但尚未有任何AI模型完全达到或超越既定的人类2,600分记录。

---

## 6. Figmimic – 一个将任何网页作为可编辑图层复制到 Figma 的书签工具

**原文标题**: Figmimic – A bookmarklet to copy any webpage into Figma as editable layers

**原文链接**: [https://marcua.net/minitools/figmimic/](https://marcua.net/minitools/figmimic/)

Figmimic是一个书签小工具，能捕获任何实时网页并将其作为可编辑的Figma画板（而非扁平截图）复制到您的剪贴板。它通过内部嵌入Figma自己的`capture.js`，适用于任何页面，包括仪表盘或已认证的应用程序。这种设计避免了从被捕获页面进行外部加载，使其能够绕过严格的内容安全策略（CSP）。

要使用Figmimic，请将提供的书签小工具拖动到您的浏览器书签栏（它很大，大约400KB，应定期更新）。然后，导航到所需的网页，点击该书签小工具，等待“已复制”确认，并将可编辑的界面直接粘贴到Figma中。

常见问题包括Firefox由于URL长度限制无法保存该书签小工具（推荐使用Chrome或Safari）。如果剪贴板被拒绝或提示“点击此页面进行捕获”，随后在页面上的任意点击都将触发复制，因为写入剪贴板需要用户交互和焦点。如果页面的`connect-src`策略限制从第三方域进行嵌入，某些图片可能会丢失；但文本、布局和样式不受影响。

---

## 7. DNA检测证实王室血统，比利时汽车销售员变王子

**原文标题**: Belgian car salesman becomes prince after DNA test proves royal parentage

**原文链接**: [https://www.cnn.com/2026/08/22/europe/prince-belgium-secret-son-scli-intl](https://www.cnn.com/2026/08/22/europe/prince-belgium-secret-son-scli-intl)

克莱门特·范登克尔克霍夫（Clément Vandenkerckhove），一名26岁的比利时汽车销售员，在DNA测试证实其生父是菲利普国王的弟弟洛朗亲王后，成为了亲王。他的母亲，比利时歌手温迪·范·万腾（Wendy Van Wanten），曾在20世纪90年代与洛朗亲王有过一段感情，在他16岁时向他揭示了身世。

大约六个月前，在DNA测试证实他们父子关系后，范登克尔克霍夫在一场低调的市政厅仪式上被合法确认为洛朗亲王的儿子。这项正式登记赋予了他与同父异母的兄弟姐妹路易丝公主、尼古拉斯亲王和艾默里克亲王对洛朗亲王私人遗产的同等继承权。然而，他不会获得王室津贴，也不需要履行官方职责，更不享有比利时王位的任何权利。

范登克尔克霍夫出生于2000年8月，他回忆道，在母亲坦白后，他联系了洛朗亲王，这促成了DNA测试以及随后的“开诚布公的对话”。尽管他可以选择采用萨克森-科堡（Saxe-Coburg）的姓氏，但他表示对自己母亲的姓氏范登克尔克霍夫感到自豪。

这一事件标志着比利时又一起王室秘密血缘关系的浮出水面。洛朗亲王的父亲，前国王阿尔贝二世，也曾在2020年承认自己在一段婚外情中育有一女，德尔菲娜·布埃尔（Delphine Boël）。经过漫长的法律斗争，她被授予了公主头衔，现在使用德尔菲娜·德·萨克森-科堡（Delphine de Saxe-Coburg）这个名字。

---

## 8. 乌兹别克斯坦一夜：为何这一数据点如此有影响力？

**原文标题**: One night in Uzbekistan: Why was this one data point so influential?

**原文链接**: [https://statmodeling.stat.columbia.edu/2026/08/20/we-couldnt-reproduce-their-findings-and-realized-that-it-was-all-driven-by-weird-data-from-uzbekistan/](https://statmodeling.stat.columbia.edu/2026/08/20/we-couldnt-reproduce-their-findings-and-realized-that-it-was-all-driven-by-weird-data-from-uzbekistan/)

无法访问文章链接。

---

## 9. I Dream of Quieter Computing

**原文标题**: I Dream of Quieter Computing

**原文链接**: [https://henry.codes/writing/i-dream-of-quieter-computing/](https://henry.codes/writing/i-dream-of-quieter-computing/)

生成摘要时出错

---

## 10. Sydney Marathon medal mistakenly depicts Munich stadium

**原文标题**: Sydney Marathon medal mistakenly depicts Munich stadium

**原文链接**: [https://www.bbc.com/news/articles/cvg92y1wzn8o](https://www.bbc.com/news/articles/cvg92y1wzn8o)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-08-23](output/hacker_news_summary_2026-08-23.md) |
| 2 | [2026-08-21](output/hacker_news_summary_2026-08-21.md) |
| 3 | [2026-08-19](output/hacker_news_summary_2026-08-19.md) |
| 4 | [2026-08-20](output/hacker_news_summary_2026-08-20.md) |
| 5 | [2026-08-22](output/hacker_news_summary_2026-08-22.md) |
| 6 | [2026-08-18](output/hacker_news_summary_2026-08-18.md) |
| 7 | [2026-08-15](output/hacker_news_summary_2026-08-15.md) |
| 8 | [2026-08-12](output/hacker_news_summary_2026-08-12.md) |
| 9 | [2026-08-13](output/hacker_news_summary_2026-08-13.md) |
| 10 | [2026-08-14](output/hacker_news_summary_2026-08-14.md) |
| 11 | [2026-08-17](output/hacker_news_summary_2026-08-17.md) |
| 12 | [2026-08-16](output/hacker_news_summary_2026-08-16.md) |
| 13 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 14 | [2026-08-09](output/hacker_news_summary_2026-08-09.md) |
| 15 | [2026-08-10](output/hacker_news_summary_2026-08-10.md) |
| 16 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 17 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 18 | [2026-08-11](output/hacker_news_summary_2026-08-11.md) |
| 19 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 20 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 21 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 22 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 23 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 24 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 25 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 26 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 27 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 28 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 29 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 30 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 31 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 32 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 33 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 34 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 35 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 36 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 37 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 38 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 39 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 40 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 41 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 42 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 43 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 44 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 45 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 46 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 47 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 48 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 49 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 50 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 51 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 52 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 53 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 54 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 55 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 56 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 57 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 58 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 59 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 60 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 61 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 62 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 63 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 64 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 65 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 66 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 67 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 68 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 69 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 70 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 71 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 72 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 73 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 74 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 75 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 76 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 77 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 78 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 79 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 80 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 81 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 82 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 83 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 84 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 85 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 86 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 87 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 88 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 89 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 90 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 91 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 92 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 93 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 94 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 95 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 96 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 97 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 98 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 99 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 100 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 101 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 102 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 103 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 104 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 105 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 106 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 107 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 108 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 109 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 110 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 111 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 112 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 113 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 114 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 115 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 116 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 117 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 118 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 119 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 120 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 121 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 122 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 123 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 124 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 125 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 126 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 127 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 128 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 129 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 130 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 131 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 132 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 133 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 134 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 135 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 136 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 137 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 138 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 139 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 140 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 141 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 142 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 143 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 144 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 145 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 146 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 147 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 148 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 149 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 150 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 151 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 152 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 153 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 154 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 155 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 156 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 157 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 158 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 159 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 160 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 161 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 162 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 163 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 164 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 165 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 166 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 167 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 168 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 169 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 170 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 171 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 172 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 173 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 174 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 175 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 176 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 177 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 178 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 179 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 180 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 181 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 182 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 183 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 184 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 185 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 186 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 187 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 188 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 189 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 190 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 191 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 192 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 193 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 194 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 195 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 196 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 197 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 198 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 199 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 200 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 201 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 202 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 203 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 204 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 205 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 206 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 207 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 208 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 209 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 210 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 211 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 212 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 213 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 214 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 215 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 216 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 217 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 218 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 219 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 220 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 221 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 222 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 223 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 224 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 225 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 226 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 227 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 228 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 229 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 230 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 231 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 232 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 233 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 234 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 235 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 236 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 237 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 238 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 239 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 240 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 241 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 242 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 243 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 244 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 245 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 246 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 247 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 248 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 249 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 250 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 251 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 252 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 253 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 254 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 255 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 256 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 257 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 258 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 259 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 260 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 261 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 262 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 263 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 264 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 265 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 266 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 267 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 268 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 269 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 270 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 271 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 272 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 273 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 274 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 275 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 276 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 277 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 278 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 279 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 280 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 281 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 282 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 283 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 284 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 285 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 286 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 287 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 288 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
