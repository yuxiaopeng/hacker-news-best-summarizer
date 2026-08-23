# Hacker News 热门文章摘要 (2026-08-23)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

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

## 11. Tragically, as many as 9625 out of every 10k individuals may be neurotypical

**原文标题**: Tragically, as many as 9625 out of every 10k individuals may be neurotypical

**原文链接**: [https://erikengdahl.se/autism/isnt/](https://erikengdahl.se/autism/isnt/)

生成摘要时出错

---

## 12. Fast and Hard Code

**原文标题**: Fast and Hard Code

**原文链接**: [https://lucumr.pocoo.org/2026/8/22/fast-hard-code/](https://lucumr.pocoo.org/2026/8/22/fast-hard-code/)

生成摘要时出错

---

## 13. A website for debloated open source alternatives

**原文标题**: A website for debloated open source alternatives

**原文链接**: [https://debloat.dev/](https://debloat.dev/)

生成摘要时出错

---

## 14. GPT 5.6 Sol 20% price reduction

**原文标题**: GPT 5.6 Sol 20% price reduction

**原文链接**: [https://developers.openai.com/api/docs/models/gpt-5.6-sol](https://developers.openai.com/api/docs/models/gpt-5.6-sol)

生成摘要时出错

---

## 15. 'Ghost job' ads are getting so bad that lawmakers want to ban them

**原文标题**: 'Ghost job' ads are getting so bad that lawmakers want to ban them

**原文链接**: [https://www.wsj.com/lifestyle/careers/ghost-job-ads-are-getting-so-bad-that-lawmakers-want-to-ban-them-2580bc3e](https://www.wsj.com/lifestyle/careers/ghost-job-ads-are-getting-so-bad-that-lawmakers-want-to-ban-them-2580bc3e)

生成摘要时出错

---

## 16. Tumble Forth – from assembly to OS with C compiler (2023)

**原文标题**: Tumble Forth – from assembly to OS with C compiler (2023)

**原文链接**: [https://tumbleforth.hardcoded.net/](https://tumbleforth.hardcoded.net/)

生成摘要时出错

---

## 17. Coconut Oil Jet Fuel Matches Kerosene's Efficiency in Engine Tests

**原文标题**: Coconut Oil Jet Fuel Matches Kerosene's Efficiency in Engine Tests

**原文链接**: [https://studyfinds.com/coconut-oil-jet-fuel-matches-kerosenes-efficiency-in-engine-tests/](https://studyfinds.com/coconut-oil-jet-fuel-matches-kerosenes-efficiency-in-engine-tests/)

生成摘要时出错

---

## 18. Show HN: OzBrain, a shared brain for knowledge between agents and your team

**原文标题**: Show HN: OzBrain, a shared brain for knowledge between agents and your team

**原文链接**: [https://ozbrain.com](https://ozbrain.com)

生成摘要时出错

---

## 19. The Sloppification of Peptides

**原文标题**: The Sloppification of Peptides

**原文链接**: [https://henryaj.substack.com/p/the-sloppification-of-peptides](https://henryaj.substack.com/p/the-sloppification-of-peptides)

生成摘要时出错

---

## 20. US Military newspaper editor voices censorship fears after being fired

**原文标题**: US Military newspaper editor voices censorship fears after being fired

**原文链接**: [https://www.bbc.com/news/articles/cm2g23ng8p4o](https://www.bbc.com/news/articles/cm2g23ng8p4o)

生成摘要时出错

---

## 21. HN: The Good Parts (2016)

**原文标题**: HN: The Good Parts (2016)

**原文链接**: [https://danluu.com/hn-comments/](https://danluu.com/hn-comments/)

生成摘要时出错

---

## 22. Electric shock gloves in use by police departments in Bellevue, Omaha

**原文标题**: Electric shock gloves in use by police departments in Bellevue, Omaha

**原文链接**: [https://nebraskapublicmedia.org/en/news/news-articles/electric-shock-gloves-already-in-use-by-police-departments-in-bellevue-omaha/](https://nebraskapublicmedia.org/en/news/news-articles/electric-shock-gloves-already-in-use-by-police-departments-in-bellevue-omaha/)

生成摘要时出错

---

## 23. Mathematicians will probably become obsolete before anyone else [pdf] (2004)

**原文标题**: Mathematicians will probably become obsolete before anyone else [pdf] (2004)

**原文链接**: [https://olli.unt.edu/handouts/fall24/tk-writing-sample.pdf](https://olli.unt.edu/handouts/fall24/tk-writing-sample.pdf)

生成摘要时出错

---

## 24. I set a trap for a book-marketing scammer (2025)

**原文标题**: I set a trap for a book-marketing scammer (2025)

**原文链接**: [https://rwwgreene.substack.com/p/i-set-a-trap-for-a-book-marketing](https://rwwgreene.substack.com/p/i-set-a-trap-for-a-book-marketing)

生成摘要时出错

---

## 25. Paul Atkins misreads Adam Smith and the American founding

**原文标题**: Paul Atkins misreads Adam Smith and the American founding

**原文链接**: [https://sites.duke.edu/thefinregblog/2026/08/03/paul-atkins-misreads-adam-smith-and-the-american-founding/](https://sites.duke.edu/thefinregblog/2026/08/03/paul-atkins-misreads-adam-smith-and-the-american-founding/)

生成摘要时出错

---

## 26. Iranian hackers shut down UK power plant for 4 days

**原文标题**: Iranian hackers shut down UK power plant for 4 days

**原文链接**: [https://www.telegraph.co.uk/news/2026/08/22/iranian-hackers-shut-down-uk-power-plant/](https://www.telegraph.co.uk/news/2026/08/22/iranian-hackers-shut-down-uk-power-plant/)

生成摘要时出错

---

## 27. Show HN: Make your logo extra bright on HDR screens

**原文标题**: Show HN: Make your logo extra bright on HDR screens

**原文链接**: [https://www.soverybright.com/](https://www.soverybright.com/)

生成摘要时出错

---

## 28. Why Sal Khan't: On Learning by Making but Teaching by Telling

**原文标题**: Why Sal Khan't: On Learning by Making but Teaching by Telling

**原文链接**: [https://punyamishra.com/2026/04/16/why-sal-khant-on-learning-by-making-but-teaching-by-telling/](https://punyamishra.com/2026/04/16/why-sal-khant-on-learning-by-making-but-teaching-by-telling/)

生成摘要时出错

---

## 29. Chinese robot runs 100M sprint quicker than Usain Bolt's world record

**原文标题**: Chinese robot runs 100M sprint quicker than Usain Bolt's world record

**原文链接**: [https://www.theguardian.com/sport/2026/aug/22/chinese-robot-runs-100m-sprint-quicker-usain-bolt-world-record](https://www.theguardian.com/sport/2026/aug/22/chinese-robot-runs-100m-sprint-quicker-usain-bolt-world-record)

生成摘要时出错

---

