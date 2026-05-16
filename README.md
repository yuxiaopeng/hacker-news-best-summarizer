# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-05-16.md)

*最后自动更新时间: 2026-05-16 20:25:23*
## 1. 我相信目前许多公司都患上了“AI狂想症”。

**原文标题**: I believe there are entire companies right now under AI psychosis

**原文链接**: [https://twitter.com/mitchellh/status/2055380239711457578](https://twitter.com/mitchellh/status/2055380239711457578)

尽管提供了标题“我相信现在有整家公司都处于AI精神病状态”，但内容本身并非一篇关于此主题的文章或讨论。相反，所提供的文本是一条来自x.com（原Twitter）的错误消息。

该消息写着：“JavaScript 不可用。我们检测到此浏览器中JavaScript已禁用。请启用JavaScript或切换到受支持的浏览器以继续使用x.com。”它指示用户启用JavaScript或切换到受支持的浏览器以访问网站。该消息还包括指向帮助中心、服务条款、隐私政策、Cookie政策、版本说明和广告信息的链接，版权所有 © 2026 X Corp。

因此，没有提供与“AI精神病”相关的内容以供总结；所提供的文本是一条技术性浏览器错误消息。

---

## 2. 古腾堡计划 – 越来越好

**原文标题**: Project Gutenberg – keeps getting better

**原文链接**: [https://www.gutenberg.org/](https://www.gutenberg.org/)

古腾堡计划是一个开创性的在线图书馆，提供超过75,000本完全免费的电子书。它成立于1971年，将美国版权已过期的旧作品数字化并进行细致的校对，从而使经典文学及其他文本得以广泛传播。用户可以下载epub和Kindle格式的图书，或在线阅读，无需任何应用、费用或注册。

这个由数千名志愿者开发的庞大藏书包括《弗兰肯斯坦》和《傲慢与偏见》等热门书目、新出版物，以及从文学、历史到科学、哲学等广泛的类别。用户可以通过搜索选项、主要类别或精选阅读列表来查找书籍。

古腾堡计划还提供大量有声读物，其中包括662部人工朗读的作品，近5,000部由2023年与微软和麻省理工学院合作产生的计算机生成作品，以及LibriVox人工朗读有声读物的访问权限。

该组织以志愿者为基础运作，并依靠捐款来继续其使命。个人可以通过校对（通过分布式校对）、报告错误或录制有声读物来做出贡献。网站提供全面的帮助、常见问题解答以及阅读选项的信息。

---

## 3. arXiv 新政策：虚构参考文献禁封一年

**原文标题**: New arXiv policy: 1-year ban for hallucinated references

**原文链接**: [https://twitter.com/tdietterich/status/2055000956144935055](https://twitter.com/tdietterich/status/2055000956144935055)

提供的内​​容是x.com（原Twitter）发出的错误消息，表明JavaScript已禁用，而不是一篇关于arXiv政策的文章。

然而，*仅根据所提供的标题*：“arXiv新政策：虚构参考文献作者将被禁一年”，关键信息是arXiv已实施了一项新政策。该政策规定，提交包含虚构（捏造或不存在的）参考文献的预印本的作者将面临一年禁令。

---

## 4. 穆瓦德的出口IP竟然是可识别的

**原文标题**: Mullvad exit IPs are surprisingly identifying

**原文链接**: [https://tmctmt.com/posts/mullvad-exit-ips-as-a-fingerprinting-vector/](https://tmctmt.com/posts/mullvad-exit-ips-as-a-fingerprinting-vector/)

Mullvad的出口IP地址分配系统虽然为每台服务器提供多个IP，但已被识别为一个重要的指纹识别向量。用户在给定服务器的出口IP是根据其WireGuard密钥确定性选择的，该密钥通常每1到30天轮换一次。

研究表明，尽管理论上有数十亿种IP组合，但实际分配的独特组合数量有限。核心问题在于，对于任何给定的WireGuard密钥，在*不同*服务器上分配的出口IP始终在每个服务器各自的IP池中占据*相同的百分位*。这很可能是由于Mullvad使用基于种子的随机数生成器（可能是Rust的`rand::random_range`），其中WireGuard密钥作为种子，输出浮点数按服务器的IP池大小进行缩放。这导致了不同的绝对IP，但相对位置相同。

这一缺陷使得“关联攻击”成为可能。通过观察用户从多个Mullvad服务器的出口IP，攻击者可以推断出一个与其WireGuard密钥相关的狭窄“浮点范围”。如果两个看似不同的用户或连接表现出重叠的浮点范围，则强烈暗示他们是同一个人，有可能通过IP日志或数据泄露，以超过99%的准确率导致去匿名化。

为了缓解此问题，用户应避免使用相同的公钥频繁切换Mullvad服务器，并通过退出Mullvad应用程序主动强制轮换其公钥。

---

## 5. 阻止发行商停运线上游戏的法案在加州获推进

**原文标题**: Bill to block publishers from killing online games advances in California

**原文链接**: [https://arstechnica.com/gaming/2026/05/bill-to-keep-online-games-playable-clears-key-hurdle-in-california/](https://arstechnica.com/gaming/2026/05/bill-to-keep-online-games-playable-clears-key-hurdle-in-california/)

一项旨在确保在线游戏长期可玩性的名为《保护我们的游戏法案》的法案，已在加州议会拨款委员会获得通过，并将提交全体大会进行投票。

该拟议立法将要求数字游戏发行商，如果停止支持某款在线游戏，必须提供全额退款，或提供该游戏的更新独立版本。发行商还需要在终止基本服务前60天通知玩家。该法案一旦通过，将适用于2027年1月1日或之后在加州销售的游戏，但完全免费游戏和仅通过订阅提供的游戏除外。

该法案得到了“停止扼杀游戏”（SKG）的强力支持，该组织是一个为法案起草提供建议的玩家倡导团体，他们认为产品不应“在不通知的情况下被剥夺”。与此相反，代表主要发行商的娱乐软件协会（ESA）则反对该法案。ESA声称，消费者获得的是许可而非完全所有权，且游戏停服是现代软件的“自然特征”。他们还认为，要求无限期可玩性会给有时限的音乐和知识产权许可以及技术可行性带来不合理的负担。

尽管已通过数个委员会，该法案在提交给州长加文·纽森签署之前，仍面临重大障碍，包括在加州议会和参议院全体会议上的投票。然而，它的进展标志着“停止扼杀游戏”运动的一项重大胜利。

---

## 6. Windows XP 桌面风格探索维基百科

**原文标题**: Explore Wikipedia Like a Windows XP Desktop

**原文链接**: [https://explorer.samismith.com/](https://explorer.samismith.com/)

由sami.smith.com开发的“维基百科文件浏览器”项目，重新构想了在Windows XP桌面界面中浏览维基百科的方式。它的目标是让维基百科的分类可以像文件夹一样导航，文章可以像文档一样打开，从而提供对几乎所有维基百科内容的访问。

除了维基百科之外，“媒体”部分允许用户探索维基共享资源的分类，并具备一项独特功能：右键点击任何图片即可将其设置为桌面背景。一项正在开发中的功能“地理文件浏览器”构想将地球作为一个可导航的文件夹，用户可以在其中上传图片或添加文本注释。

Readme.txt文件提供了Sami Smith的联系方式，包括电子邮件、Twitter和Blue Sky，并列举了几个启发性项目，例如Neal.fun的Wiki Files和react-xp.jamiepates.com。它阐明“维基百科”和“媒体”部分中的内容属于维基媒体，并鼓励用户通过编辑维基百科和维基媒体来为文件夹结构做出贡献。整体体验模仿了经典的Windows XP环境，包含“开始”菜单、“我的文档”、“控制面板”等熟悉元素。

---

## 7. 英国政府用自行开发的难民系统取代了Palantir软件

**原文标题**: UK government replaces Palantir software with internally-built refugee system

**原文链接**: [https://www.bbc.com/news/articles/c2l2j1lxdk5o](https://www.bbc.com/news/articles/c2l2j1lxdk5o)

生成摘要时出错

---

## 8. Codex is now in the ChatGPT mobile app

**原文标题**: Codex is now in the ChatGPT mobile app

**原文链接**: [https://openai.com/index/work-with-codex-from-anywhere/](https://openai.com/index/work-with-codex-from-anywhere/)

生成摘要时出错

---

## 9. U.S. DOJ demands Apple and Google unmask over 100k users of car-tinkering app

**原文标题**: U.S. DOJ demands Apple and Google unmask over 100k users of car-tinkering app

**原文链接**: [https://macdailynews.com/2026/05/15/u-s-doj-demands-apple-and-google-unmask-over-100000-users-of-popular-car-tinkering-app-in-emissions-crackdown/](https://macdailynews.com/2026/05/15/u-s-doj-demands-apple-and-google-unmask-over-100000-users-of-popular-car-tinkering-app-in-emissions-crackdown/)

生成摘要时出错

---

## 10. Bun Rust 重写：代码库未能通过基本的 Miri 检查，导致 Safe Rust 中出现未定义行为。

**原文标题**: Bun Rust rewrite: "codebase fails basic miri checks, allows for UB in safe rust"

**原文链接**: [https://github.com/oven-sh/bun/issues/30719](https://github.com/oven-sh/bun/issues/30719)

An issue (#30719) has been filed against the Bun project's Rust rewrite, alleging that the codebase "fails even the most basic miri checks" and permits Undefined Behavior (UB) in ostensibly safe Rust code.

The specific Miri error reported is: "constructing invalid value of type &[u8]: encountered a dangling reference," occurring within the `PathString::slice` function at `src/main.rs:97:18`. The problem arises when `core::slice::from_raw_parts` is used with a pointer to memory that has already been deallocated.

The provided example code illustrates this: a `PathString` is initialized using a reference to data owned by a `Box<[u8]>`. However, the `Box` is subsequently dropped, freeing the underlying memory, *before* `PathString::slice()` is called. This results in the `slice` method attempting to access a dangling pointer, leading to guaranteed Undefined Behavior.

The issue reporter, AwesomeQubic, criticizes the project's coding practices, stating, "AIs are not good at writing Rust," and recommends hiring "a real rust dev," implying a lack of proper Rust expertise or reliance on inadequate automated code generation. The report underscores a critical failure in memory safety that undermines Rust's core guarantees.

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 2 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 3 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 4 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 5 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 6 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 7 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 8 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 9 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 10 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 11 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 12 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 13 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 14 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 15 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 16 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 17 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 18 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 19 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 20 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 21 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 22 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 23 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 24 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 25 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 26 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 27 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 28 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 29 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 30 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 31 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 32 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 33 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 34 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 35 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 36 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 37 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 38 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 39 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 40 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 41 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 42 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 43 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 44 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 45 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 46 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 47 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 48 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 49 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 50 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 51 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 52 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 53 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 54 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 55 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 56 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 57 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 58 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 59 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 60 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 61 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 62 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 63 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 64 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 65 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 66 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 67 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 68 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 69 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 70 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 71 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 72 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 73 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 74 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 75 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 76 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 77 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 78 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 79 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 80 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 81 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 82 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 83 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 84 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 85 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 86 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 87 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 88 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 89 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 90 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 91 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 92 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 93 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 94 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 95 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 96 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 97 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 98 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 99 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 100 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 101 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 102 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 103 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 104 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 105 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 106 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 107 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 108 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 109 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 110 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 111 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 112 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 113 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 114 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 115 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 116 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 117 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 118 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 119 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 120 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 121 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 122 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 123 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 124 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 125 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 126 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 127 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 128 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 129 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 130 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 131 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 132 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 133 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 134 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 135 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 136 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 137 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 138 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 139 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 140 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 141 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 142 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 143 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 144 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 145 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 146 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 147 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 148 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 149 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 150 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 151 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 152 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 153 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 154 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 155 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 156 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 157 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 158 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 159 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 160 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 161 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 162 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 163 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 164 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 165 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 166 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 167 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 168 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 169 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 170 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 171 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 172 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 173 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 174 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 175 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 176 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 177 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 178 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 179 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 180 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 181 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 182 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 183 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 184 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 185 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 186 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 187 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 188 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 189 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 190 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
