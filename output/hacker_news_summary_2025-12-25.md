# Hacker News 热门文章摘要 (2025-12-25)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 爱泼斯坦档案的一些删节正在被撤销

**原文标题**: Some Epstein file redactions are being undone

**原文链接**: [https://www.theguardian.com/us-news/2025/dec/23/epstein-unredacted-files-social-media](https://www.theguardian.com/us-news/2025/dec/23/epstein-unredacted-files-social-media)

司法部公布的杰弗里·爱泼斯坦案文件中，被遮盖的部分正通过Photoshop或高亮显示等简单技术被还原，导致未经涂黑处理的文本在社交媒体上传播。

一份针对爱泼斯坦遗产执行人达伦·R·因迪克和理查德·D·卡恩的民事案件证物显示，因迪克在2015年至2019年间签署了超过40万美元的支票，支付给年轻女性模特和演员，其中包括给一名前俄罗斯模特38万美元。因迪克作为爱泼斯坦数十年的律师，曾以1.05亿美元了结了一宗民事性交易案，但尚未受到刑事起诉。他目前的律师事务所曾代表唐纳德·特朗普。

更多未经涂黑处理的段落描述了爱泼斯坦的团伙通过支付参与者兼证人的法律费用、威胁受害者、发布关于他们的负面消息以及指示销毁证据来隐瞒罪行。财务违规行为也随之曝光，显示爱泼斯坦成立的公司支付了巨额房产税（例如，Cypress公司在2018年为圣达菲的房产支付了超过10万美元的税款），而这些税款并未反映在其资产负债表上。

尽管《爱泼斯坦文件透明法案》允许扣留受害者信息或可能危及正在进行的调查的细节，但尚不清楚关于房产税信息的涂黑处理如何符合该法案。

---

## 2. X-ray：一个用于查找 PDF 文档中不当密文遮盖的 Python 库

**原文标题**: X-ray: a Python library for finding bad redactions in PDF documents

**原文链接**: [https://github.com/freelawproject/x-ray](https://github.com/freelawproject/x-ray)

`x-ray` 是 Free Law Project 开发的一个 Python 库，用于识别 PDF 文档中的“无效遮盖”。它解决的问题是，许多人通过简单地在文本上方绘制黑色矩形或高亮来遮盖敏感信息，这使得底层文本仍然可以被轻易选中和读取。

该工具接受 PDF 文件路径、URL 或字节对象作为输入，并分析其中是否存在此类无效遮盖。它输出 JSON（用于命令行界面）或 Python 字典（用于程序化使用），详细说明了发现结果。该输出以页码作为键，每个页码对应一个字典列表。每个字典都提供了无效遮盖的 `bbox`（边框坐标）以及被不当隐藏的 `text`（文本）。

使用 `uv` (`uv add x-ray`) 或 `pip` (`pip install x-ray`) 进行安装非常简单。它可以通过命令行使用，包括 `uvx` 临时运行或安装后直接使用；也可以通过 `xray.inspect()` 方法集成到 Python 脚本中。

在底层，`x-ray` 利用了高性能的 PyMuPDF 库。它的工作原理是识别 PDF 中的矩形和文本，然后将矩形渲染成图像，以判断它是否为纯色（表示无效遮盖）或多种颜色混合（表明是适当的遮盖）。

该项目欢迎贡献，以解决更复杂的遮盖类型，并以宽松的 BSD 许可证发布。

---

## 3. 圣诞节时，我们请了一个男人来家里，他一住就是45年。

**原文标题**: We invited a man into our home at Christmas and he stayed with us for 45 years

**原文链接**: [https://www.bbc.co.uk/news/articles/cdxwllqz1l0o](https://www.bbc.co.uk/news/articles/cdxwllqz1l0o)

1975年12月，年轻的卡迪夫夫妇罗布和黛安·帕森斯将无家可归、提着一只冻鸡来到他们家门口的罗尼·洛克伍德迎进家中过圣诞。罗布隐约记得罗尼是儿时旧识，他患有自闭症。最初是出于暂时的同情之举，却发展成一段长达45年的独特情谊，直到罗尼于2020年去世。

这对当时27岁和26岁的夫妇得知，罗尼自15岁起就无家可归，此前他被一家福利院和一所“智障男孩学校”逐出。他们帮助他找到了一份废物收集员的工作，给他买了新衣服，并将他融入他们的生活。罗尼反过来也成了他们家中不可或缺的一员，他一丝不苟地执行日常惯例，并在他们的教堂大量做义工。当黛安患上慢性疲劳综合征时，他在照顾他们的孩子劳埃德和凯蒂方面表现尤为出色。

尽管面临挑战，包括罗尼长达20年的赌博成瘾，帕森斯夫妇依然珍视他的存在。让他们让他独立生活的念头一闪而过就被打消，是因为罗尼一句真挚的问话“我是不是做错了什么？”，让罗布承诺他们将“永远在一起”。

罗尼75岁去世后，一个新的福利中心“洛克伍德之家”（Lockwood House）以他的名字命名，以示纪念。令人称奇的是，罗尼的遗嘱将4万英镑留给了慈善机构，恰好是资助该中心屋顶维修所需的金额，确保“这位无家可归者为我们所有人提供了庇护”。罗布和黛安回顾说，罗尼“丰富了他们的生活”，而他们这段独特的旅程是“一天一天走过来的”。

---

## 4. 英伟达将以200亿美元现金收购Groq的资产

**原文标题**: Nvidia to buy assets from Groq for $20B cash

**原文链接**: [https://www.cnbc.com/2025/12/24/nvidia-buying-ai-chip-startup-groq-for-about-20-billion-biggest-deal.html](https://www.cnbc.com/2025/12/24/nvidia-buying-ai-chip-startup-groq-for-about-20-billion-biggest-deal.html)

英伟达已同意以200亿美元现金收购AI芯片初创公司Groq的资产，这标志着其有史以来最大的一笔收购。Groq由谷歌张量处理单元（TPU）的创始团队创建，是英伟达在AI工作负载领域的竞争对手，就在三个月前，其在一轮融资中估值达69亿美元。

虽然Groq将其描述为一项针对其推理技术的“非独家许可协议”，但消息人士指出，英伟达正在收购Groq的所有资产，但其GroqCloud业务除外，该业务将继续独立运营。Groq的创始人兼首席执行官Jonathan Ross，以及总裁Sunny Madra和其他高级领导人将加入英伟达。Groq本身将继续作为一家独立公司存在，由新任首席执行官Simon Edwards领导。

英伟达首席执行官黄仁勋表示，该协议将把Groq的低延迟处理器整合到英伟达的AI工厂架构中，从而扩展AI推理和实时工作负载的能力。他澄清说，英伟达正在许可知识产权并吸纳人才，而不是收购Groq这家公司。这项200亿美元的交易显著超越了英伟达此前最大的收购——2019年以70亿美元收购Mellanox，并且符合英伟达通过许可协议大力投资AI初创公司和人才的战略。据报道，Groq此前并未寻求出售，并曾设定今年实现5亿美元营收的目标。

---

## 5. Ruby 4.0.0

**原文标题**: Ruby 4.0.0

**原文链接**: [https://www.ruby-lang.org/en/news/2025/12/25/ruby-4-0-0-released/](https://www.ruby-lang.org/en/news/2025/12/25/ruby-4-0-0-released/)

Ruby 4.0.0 引入了两项主要的实验性功能：“Ruby Box”和“ZJIT”。Ruby Box 为定义提供了隔离环境，非常适合测试、蓝绿部署以及通过防止猴子补丁和全局变量泄露来管理依赖。ZJIT 是一个新的下一代 JIT 编译器，作为 YJIT 的继任者，用 Rust 构建，旨在提高性能并促进外部贡献，尽管目前它比 YJIT 慢。

Ruby 的并行执行机制 Ractor 获得了显著增强。新的 `Ractor::Port` 类简化了消息传递，`Ractor.shareable_proc` 促进了 `Proc` 对象的共享，内部优化减少了全局锁竞争，从而提高了并行性。Ractor 的实验性状态计划于明年移除。

语言变化包括 `*nil` 不再调用 `nil.to_a`，以及逻辑二元运算符（`||`、`&&`、`and`、`or`）在行首时会隐式地继续上一行。`Pathname` 和 `Set` 被提升为核心类。值得注意的核心类更新包括 `Array#rfind`、`Enumerator.produce` 接受 `size` 参数、`ArgumentError` 的 `ErrorHighlight` 得到增强、`Kernel#inspect` 允许通过 `#instance_variables_to_inspect` 进行自定义，以及 `String` 更新到 Unicode 17.0.0。

在兼容性方面，几个 `Ractor` 方法（`.yield`、`#take`、`#close_incoming`、`#close_outgoing`）被移除，由 `Ractor::Port` 取代。`ObjectSpace._id2ref` 已弃用，并且 `Process::Status#&` 和 `Process::Status#>>` 被移除。`CGI` 库已基本从默认 gem 中移除（除了转义函数），并且 `SortedSet` 不再自动加载，需要单独的 gem。C 实现方法的堆栈跟踪现在显示得如同来自 Ruby 源代码。RubyGems 和 Bundler 更新到版本 4。

---

## 6. 凤凰：一个用 Zig 从零开始编写的现代 X 服务器

**原文标题**: Phoenix: A modern X server written from scratch in Zig

**原文链接**: [https://git.dec05eba.com/phoenix/about/](https://git.dec05eba.com/phoenix/about/)

Phoenix 是一个使用 Zig 从零开始编写的新 X 服务器，旨在成为 Xorg 的现代替代品。目前，它尚未准备好投入一般使用，但可以渲染具有完整硬件加速的简单 GLX、EGL 或 Vulkan 应用程序，并可嵌套在现有 X 服务器（X11；计划支持 Wayland）中运行。

它的主要目标是：
1.  **简洁性：** 仅支持与现代应用程序（近 20 年）和现代硬件（近 15-20 年）相关的 X11 协议子集，利用 Linux DRM 和 Mesa GBM，并且不包含服务器驱动接口。
2.  **安全性：** 通过 Zig 的自动协议解析和边界检查增强安全性。它默认进行应用程序隔离，需要通过 GUI 提示才能进行应用程序间访问（例如屏幕录制）或明确的预启动权限。全局热键默认需要一个修饰键，并可以选择禁用隔离。
3.  **现代技术：** 更好地支持多显示器（不同的刷新率、VRR、HDR），并通过内置合成器默认实现无撕裂的改进图形显示（对外部合成器或全屏应用程序禁用）。
4.  **新标准：** 开发并记录诸如每显示器 DPI 属性等扩展。
5.  **Wayland 兼容性：** 未来将通过原生或桥接方式支持仅限 Wayland 的应用程序。
6.  **嵌套操作：** 有助于调试和开发。

非目标包括替代 Xorg、X11 "屏幕"、GrabServer 功能、字节序交换的客户端/服务器以及间接 GLX。Phoenix 还简化了核心 X11 协议，仅实现游标相关字体操作等基本部分，并默认使用 UTF-8 字符串。该项目声称，编写一个简单实用的 X 服务器比编写一个 Wayland 合成器更容易。

---

## 7. 优倍快 旅行路由器

**原文标题**: Unifi Travel Router

**原文链接**: [https://blog.ui.com/article/travel-in-style-unifi-style-unifi-travel-router](https://blog.ui.com/article/travel-in-style-unifi-style-unifi-travel-router)

UniFi旅行路由器提供无缝便携性，让用户能够将他们信赖的UniFi网络随身携带。只需开机即可访问始终如一的网络环境，旅途中无需重新配置或考虑连接问题。

---

## 8. Show HN: Minimalist editor that lives in browser, stores everything in the URL

**原文标题**: Show HN: Minimalist editor that lives in browser, stores everything in the URL

**原文链接**: [https://github.com/antonmedv/textarea](https://github.com/antonmedv/textarea)

生成摘要时出错

---

## 9. Show HN: Vibium – Browser automation for AI and humans, by Selenium's creator

**原文标题**: Show HN: Vibium – Browser automation for AI and humans, by Selenium's creator

**原文链接**: [https://github.com/VibiumDev/vibium](https://github.com/VibiumDev/vibium)

生成摘要时出错

---

## 10. Fabrice Bellard: Biography (2009) [pdf]

**原文标题**: Fabrice Bellard: Biography (2009) [pdf]

**原文链接**: [https://www.ipaidia.gr/wp-content/uploads/2020/12/117-2020-fabrice-bellard.pdf](https://www.ipaidia.gr/wp-content/uploads/2020/12/117-2020-fabrice-bellard.pdf)

生成摘要时出错

---

## 11. Texas app store age verification law blocked by federal judge

**原文标题**: Texas app store age verification law blocked by federal judge

**原文链接**: [https://www.macrumors.com/2025/12/23/texas-app-store-law-blocked/](https://www.macrumors.com/2025/12/23/texas-app-store-law-blocked/)

生成摘要时出错

---

## 12. Alzheimer’s disease can be reversed in animal models: Study

**原文标题**: Alzheimer’s disease can be reversed in animal models: Study

**原文链接**: [https://case.edu/news/new-study-shows-alzheimers-disease-can-be-reversed-achieve-full-neurological-recovery-not-just-prevented-or-slowed-animal-models](https://case.edu/news/new-study-shows-alzheimers-disease-can-be-reversed-achieve-full-neurological-recovery-not-just-prevented-or-slowed-animal-models)

生成摘要时出错

---

## 13. Mattermost restricted access to old messages after 10000 limit is reached

**原文标题**: Mattermost restricted access to old messages after 10000 limit is reached

**原文链接**: [https://github.com/mattermost/mattermost/issues/34271](https://github.com/mattermost/mattermost/issues/34271)

生成摘要时出错

---

## 14. I'm returning my Framework 16

**原文标题**: I'm returning my Framework 16

**原文链接**: [https://yorickpeterse.com/articles/im-returning-my-framework-16/](https://yorickpeterse.com/articles/im-returning-my-framework-16/)

生成摘要时出错

---

## 15. I didn't realize my LG TV was spying on me until I turned off Live Plus

**原文标题**: I didn't realize my LG TV was spying on me until I turned off Live Plus

**原文链接**: [https://www.pocket-lint.com/lg-tv-turn-off-live-plus/](https://www.pocket-lint.com/lg-tv-turn-off-live-plus/)

生成摘要时出错

---

## 16. Who Watches the Waymos? I do [video]

**原文标题**: Who Watches the Waymos? I do [video]

**原文链接**: [https://www.youtube.com/watch?v=oYU2hAbx_Fc](https://www.youtube.com/watch?v=oYU2hAbx_Fc)

生成摘要时出错

---

## 17. Don't Become the Machine

**原文标题**: Don't Become the Machine

**原文链接**: [https://armeet.bearblog.dev/becoming-the-machine/](https://armeet.bearblog.dev/becoming-the-machine/)

生成摘要时出错

---

## 18. When compilers surprise you

**原文标题**: When compilers surprise you

**原文链接**: [https://xania.org/202512/24-cunning-clang](https://xania.org/202512/24-cunning-clang)

生成摘要时出错

---

## 19. I sell onions on the Internet (2019)

**原文标题**: I sell onions on the Internet (2019)

**原文链接**: [https://www.deepsouthventures.com/i-sell-onions-on-the-internet/](https://www.deepsouthventures.com/i-sell-onions-on-the-internet/)

生成摘要时出错

---

## 20. Microsoft please get your tab to autocomplete shit together

**原文标题**: Microsoft please get your tab to autocomplete shit together

**原文链接**: [https://ivanca.github.io/programming/2025/11/26/microsoft-pls-get-your-tab-to-autocomplete-shit-together/](https://ivanca.github.io/programming/2025/11/26/microsoft-pls-get-your-tab-to-autocomplete-shit-together/)

生成摘要时出错

---

## 21. Nabokov's guide to foreigners learning Russian

**原文标题**: Nabokov's guide to foreigners learning Russian

**原文链接**: [https://twitter.com/haravayin_hogh/status/2003299405907247502](https://twitter.com/haravayin_hogh/status/2003299405907247502)

生成摘要时出错

---

## 22. Python 3.15’s interpreter for Windows x86-64 should hopefully be 15% faster

**原文标题**: Python 3.15’s interpreter for Windows x86-64 should hopefully be 15% faster

**原文链接**: [https://fidget-spinner.github.io/posts/no-longer-sorry.html](https://fidget-spinner.github.io/posts/no-longer-sorry.html)

生成摘要时出错

---

## 23. Google's year in review: areas with research breakthroughs in 2025

**原文标题**: Google's year in review: areas with research breakthroughs in 2025

**原文链接**: [https://blog.google/technology/ai/2025-research-breakthroughs/](https://blog.google/technology/ai/2025-research-breakthroughs/)

生成摘要时出错

---

## 24. Why We Abandoned Matrix (2024)

**原文标题**: Why We Abandoned Matrix (2024)

**原文链接**: [https://forum.hackliberty.org/t/why-we-abandoned-matrix-the-dark-truth-about-user-security-and-safety/224](https://forum.hackliberty.org/t/why-we-abandoned-matrix-the-dark-truth-about-user-security-and-safety/224)

生成摘要时出错

---

## 25. Free Software Foundation receives historic private donations

**原文标题**: Free Software Foundation receives historic private donations

**原文链接**: [https://www.fsf.org/news/free-software-foundation-receives-historic-private-donations](https://www.fsf.org/news/free-software-foundation-receives-historic-private-donations)

生成摘要时出错

---

## 26. AMD entered the CPU market with reverse-engineered Intel 8080 clone 50 years ago

**原文标题**: AMD entered the CPU market with reverse-engineered Intel 8080 clone 50 years ago

**原文链接**: [https://www.tomshardware.com/pc-components/cpus/amd-first-entered-the-cpu-market-with-reverse-engineered-intel-8080-clone-50-years-ago-the-am9080-cost-50-cents-apiece-to-make-but-sold-for-usd700](https://www.tomshardware.com/pc-components/cpus/amd-first-entered-the-cpu-market-with-reverse-engineered-intel-8080-clone-50-years-ago-the-am9080-cost-50-cents-apiece-to-make-but-sold-for-usd700)

生成摘要时出错

---

## 27. How I Left YouTube

**原文标题**: How I Left YouTube

**原文链接**: [https://zhach.news/how-i-left-youtube/](https://zhach.news/how-i-left-youtube/)

生成摘要时出错

---

## 28. The e-scooter isn't new – London was zooming around on Autopeds a century ago

**原文标题**: The e-scooter isn't new – London was zooming around on Autopeds a century ago

**原文链接**: [https://www.ianvisits.co.uk/articles/the-e-scooter-isnt-new-london-was-zooming-around-on-autopeds-a-century-ago-86263/](https://www.ianvisits.co.uk/articles/the-e-scooter-isnt-new-london-was-zooming-around-on-autopeds-a-century-ago-86263/)

生成摘要时出错

---

## 29. HTTP Caching, a Refresher

**原文标题**: HTTP Caching, a Refresher

**原文链接**: [https://danburzo.ro/http-caching-refresher/](https://danburzo.ro/http-caching-refresher/)

生成摘要时出错

---

## 30. Asterisk AI Voice Agent

**原文标题**: Asterisk AI Voice Agent

**原文链接**: [https://github.com/hkjarral/Asterisk-AI-Voice-Agent](https://github.com/hkjarral/Asterisk-AI-Voice-Agent)

生成摘要时出错

---

## 31. Games’ affordance of childlike wonder and reduced burnout risk in young adults

**原文标题**: Games’ affordance of childlike wonder and reduced burnout risk in young adults

**原文链接**: [https://games.jmir.org/2025/1/e84219/](https://games.jmir.org/2025/1/e84219/)

生成摘要时出错

---

## 32. Salesforce regrets firing 4000 experienced staff and replacing them with AI

**原文标题**: Salesforce regrets firing 4000 experienced staff and replacing them with AI

**原文链接**: [https://maarthandam.com/2025/12/25/salesforce-regrets-firing-4000-staff-ai/](https://maarthandam.com/2025/12/25/salesforce-regrets-firing-4000-staff-ai/)

生成摘要时出错

---

## 33. Lessons from the PG&E outage

**原文标题**: Lessons from the PG&E outage

**原文链接**: [https://waymo.com/blog/2025/12/autonomously-navigating-the-real-world](https://waymo.com/blog/2025/12/autonomously-navigating-the-real-world)

生成摘要时出错

---

## 34. Avoid Mini-Frameworks

**原文标题**: Avoid Mini-Frameworks

**原文链接**: [https://laike9m.com/blog/avoid-mini-frameworks,171/](https://laike9m.com/blog/avoid-mini-frameworks,171/)

生成摘要时出错

---

## 35. Show HN: Turn raw HTML into production-ready images for free

**原文标题**: Show HN: Turn raw HTML into production-ready images for free

**原文链接**: [https://html2png.dev](https://html2png.dev)

生成摘要时出错

---

## 36. Spaced repetition for efficient learning (2019)

**原文标题**: Spaced repetition for efficient learning (2019)

**原文链接**: [https://gwern.net/spaced-repetition](https://gwern.net/spaced-repetition)

生成摘要时出错

---

## 37. Volvo Centum is Dalton Maag's new typeface for Volvo

**原文标题**: Volvo Centum is Dalton Maag's new typeface for Volvo

**原文链接**: [https://www.wallpaper.com/design-interiors/corporate-design-branding/volvo-new-font-volvo-centum](https://www.wallpaper.com/design-interiors/corporate-design-branding/volvo-new-font-volvo-centum)

生成摘要时出错

---

## 38. US sanctions EU government officials behind the DSA

**原文标题**: US sanctions EU government officials behind the DSA

**原文链接**: [https://mastodon.social/@fj/115773761468906515](https://mastodon.social/@fj/115773761468906515)

生成摘要时出错

---

## 39. Help My c64 caught on fire

**原文标题**: Help My c64 caught on fire

**原文链接**: [https://c0de517e.com/026_c64fire.htm](https://c0de517e.com/026_c64fire.htm)

生成摘要时出错

---

## 40. Researchers achieved 1,270 Wh/L in an anode-free lithium metal battery

**原文标题**: Researchers achieved 1,270 Wh/L in an anode-free lithium metal battery

**原文链接**: [https://postech.ac.kr/eng/research/research_results.do?mode=view&articleNo=43617&title=Anode-Free+Battery+Doubles+Electric+Vehicle+Driving+Range](https://postech.ac.kr/eng/research/research_results.do?mode=view&articleNo=43617&title=Anode-Free+Battery+Doubles+Electric+Vehicle+Driving+Range)

生成摘要时出错

---

## 41. My 2026 Open Social Web Predictions

**原文标题**: My 2026 Open Social Web Predictions

**原文链接**: [https://www.timothychambers.net/2025/12/23/my-open-social-web-predictions.html](https://www.timothychambers.net/2025/12/23/my-open-social-web-predictions.html)

生成摘要时出错

---

## 42. Help my website is too small

**原文标题**: Help my website is too small

**原文链接**: [https://lukeplant.me.uk/blog/posts/help-my-website-is-too-small/](https://lukeplant.me.uk/blog/posts/help-my-website-is-too-small/)

生成摘要时出错

---

## 43. Is Northern Virginia still the least reliable AWS region?

**原文标题**: Is Northern Virginia still the least reliable AWS region?

**原文链接**: [https://statusgator.com/blog/aws-least-reliable-region-in-2025/](https://statusgator.com/blog/aws-least-reliable-region-in-2025/)

生成摘要时出错

---

## 44. The Ultimate Windows Utility (2022)

**原文标题**: The Ultimate Windows Utility (2022)

**原文链接**: [https://christitus.com/windows-tool/](https://christitus.com/windows-tool/)

生成摘要时出错

---

## 45. Permission Systems for Enterprise That Scale

**原文标题**: Permission Systems for Enterprise That Scale

**原文链接**: [https://eliocapella.com/blog/permission-systems-for-enterprise/](https://eliocapella.com/blog/permission-systems-for-enterprise/)

生成摘要时出错

---

## 46. Terrence Malick's Disciples

**原文标题**: Terrence Malick's Disciples

**原文链接**: [https://yalereview.org/article/bilge-ebiri-terrence-malick](https://yalereview.org/article/bilge-ebiri-terrence-malick)

生成摘要时出错

---

## 47. Open source USB to GPIB converter (for Test and Measurement instruments)

**原文标题**: Open source USB to GPIB converter (for Test and Measurement instruments)

**原文链接**: [https://github.com/xyphro/UsbGpib](https://github.com/xyphro/UsbGpib)

生成摘要时出错

---

## 48. US bars 5 Europeans it says pressured tech firms to censor American viewpoints

**原文标题**: US bars 5 Europeans it says pressured tech firms to censor American viewpoints

**原文链接**: [https://apnews.com/article/state-department-trump-immigration-rubio-visas-87c8a4692f3184e4f83fdd8ed5093886](https://apnews.com/article/state-department-trump-immigration-rubio-visas-87c8a4692f3184e4f83fdd8ed5093886)

生成摘要时出错

---

## 49. Asahi Linux with Sway on the MacBook Air M2

**原文标题**: Asahi Linux with Sway on the MacBook Air M2

**原文链接**: [https://daniel.lawrence.lu/blog/2024-12-01-asahi-linux-with-sway-on-the-macbook-air-m2/](https://daniel.lawrence.lu/blog/2024-12-01-asahi-linux-with-sway-on-the-macbook-air-m2/)

生成摘要时出错

---

## 50. European Majority favours more social media regulation

**原文标题**: European Majority favours more social media regulation

**原文链接**: [https://yougov.co.uk/technology/articles/53241-european-political-monthly-where-do-europeans-stand-on-social-media-regulation](https://yougov.co.uk/technology/articles/53241-european-political-monthly-where-do-europeans-stand-on-social-media-regulation)

生成摘要时出错

---

## 51. Mt. Gox CEO Karpelès Reveals Details of 2014 Collapse and Japanese Detention

**原文标题**: Mt. Gox CEO Karpelès Reveals Details of 2014 Collapse and Japanese Detention

**原文链接**: [https://bitcoinmagazine.com/business/former-mt-gox-ceo-mark-karpeles-reveals-details-of-2014-collapse-and-japanese-detention](https://bitcoinmagazine.com/business/former-mt-gox-ceo-mark-karpeles-reveals-details-of-2014-collapse-and-japanese-detention)

生成摘要时出错

---

## 52. Beijing is enforcing tough rules to ensure chatbots don’t misbehave

**原文标题**: Beijing is enforcing tough rules to ensure chatbots don’t misbehave

**原文链接**: [https://www.wsj.com/tech/ai/china-is-worried-ai-threatens-party-ruleand-is-trying-to-tame-it-bfdcda2d](https://www.wsj.com/tech/ai/china-is-worried-ai-threatens-party-ruleand-is-trying-to-tame-it-bfdcda2d)

生成摘要时出错

---

## 53. Python Applied Mathematics Labs

**原文标题**: Python Applied Mathematics Labs

**原文链接**: [https://labs.acme.byu.edu/Pages/intro.html](https://labs.acme.byu.edu/Pages/intro.html)

生成摘要时出错

---

## 54. 'Dracula's Chivito': Hubble reveals largest birthplace of planets ever observed

**原文标题**: 'Dracula's Chivito': Hubble reveals largest birthplace of planets ever observed

**原文链接**: [https://phys.org/news/2025-12-chaotic-dracula-chivito-hubble-reveals.html](https://phys.org/news/2025-12-chaotic-dracula-chivito-hubble-reveals.html)

生成摘要时出错

---

## 55. The next-gen mainboard designed with amigaos4 and morphos in mind

**原文标题**: The next-gen mainboard designed with amigaos4 and morphos in mind

**原文链接**: [https://mirari.vitasys.nl/our-story/](https://mirari.vitasys.nl/our-story/)

生成摘要时出错

---

## 56. Could lockfiles just be SBOMs?

**原文标题**: Could lockfiles just be SBOMs?

**原文链接**: [https://nesbitt.io/2025/12/23/could-lockfiles-just-be-sboms.html](https://nesbitt.io/2025/12/23/could-lockfiles-just-be-sboms.html)

生成摘要时出错

---

## 57. Silicon Valley's tone-deaf take on the AI backlash will matter in 2026

**原文标题**: Silicon Valley's tone-deaf take on the AI backlash will matter in 2026

**原文链接**: [https://fortune.com/2025/12/23/silicon-valleys-tone-deaf-take-on-the-ai-backlash-will-matter-in-2026/](https://fortune.com/2025/12/23/silicon-valleys-tone-deaf-take-on-the-ai-backlash-will-matter-in-2026/)

生成摘要时出错

---

## 58. Steam Store is offline

**原文标题**: Steam Store is offline

**原文链接**: [https://steamstat.us/](https://steamstat.us/)

生成摘要时出错

---

## 59. Microsoft denies rewriting Windows 11 in Rust using AI

**原文标题**: Microsoft denies rewriting Windows 11 in Rust using AI

**原文链接**: [https://www.windowslatest.com/2025/12/24/microsoft-denies-rewriting-windows-11-using-ai-after-an-employees-one-engineer-one-month-one-million-code-post-on-linkedin-causes-outrage/](https://www.windowslatest.com/2025/12/24/microsoft-denies-rewriting-windows-11-using-ai-after-an-employees-one-engineer-one-month-one-million-code-post-on-linkedin-causes-outrage/)

生成摘要时出错

---

## 60. Former EU commissioner and activists barred from US

**原文标题**: Former EU commissioner and activists barred from US

**原文链接**: [https://www.theguardian.com/technology/2025/dec/24/us-state-department-visa-ban-former-eu-commissioner-europe](https://www.theguardian.com/technology/2025/dec/24/us-state-department-visa-ban-former-eu-commissioner-europe)

生成摘要时出错

---

## 61. New reactor produces clean energy and carbon nanotubes from natural gas

**原文标题**: New reactor produces clean energy and carbon nanotubes from natural gas

**原文链接**: [https://phys.org/news/2025-12-reactor-energy-carbon-nanotubes-natural.html](https://phys.org/news/2025-12-reactor-energy-carbon-nanotubes-natural.html)

生成摘要时出错

---

## 62. Donald E. Knuth and Peter van Emde Boas on priority deques (1977) [pdf]

**原文标题**: Donald E. Knuth and Peter van Emde Boas on priority deques (1977) [pdf]

**原文链接**: [https://staff.fnwi.uva.nl/p.vanemdeboas/knuthnote.pdf](https://staff.fnwi.uva.nl/p.vanemdeboas/knuthnote.pdf)

生成摘要时出错

---

## 63. Un-Redactor

**原文标题**: Un-Redactor

**原文链接**: [https://github.com/kvthweatt/unredactor](https://github.com/kvthweatt/unredactor)

生成摘要时出错

---

## 64. CEO killed at industrial site by worker operating forklift

**原文标题**: CEO killed at industrial site by worker operating forklift

**原文链接**: [https://www.12onyourside.com/2025/12/23/ceo-killed-industrial-site-by-worker-operating-forklift-while-talking-phone-osha-report-shows/](https://www.12onyourside.com/2025/12/23/ceo-killed-industrial-site-by-worker-operating-forklift-while-talking-phone-osha-report-shows/)

生成摘要时出错

---

## 65. Dutch rental fleet Mistergreen goes bankrupt after betting on Tesla self-driving

**原文标题**: Dutch rental fleet Mistergreen goes bankrupt after betting on Tesla self-driving

**原文链接**: [https://guessingheadlights.com/dutch-tesla-fleet-goes-bust-after-betting-on-musks-self-driving-promises/](https://guessingheadlights.com/dutch-tesla-fleet-goes-bust-after-betting-on-musks-self-driving-promises/)

生成摘要时出错

---

## 66. Microsoft Agent Framework

**原文标题**: Microsoft Agent Framework

**原文链接**: [https://learn.microsoft.com/en-us/agent-framework/overview/agent-framework-overview](https://learn.microsoft.com/en-us/agent-framework/overview/agent-framework-overview)

生成摘要时出错

---

## 67. Quantum Error Correction Goes FOOM

**原文标题**: Quantum Error Correction Goes FOOM

**原文链接**: [https://algassert.com/post/2503](https://algassert.com/post/2503)

生成摘要时出错

---

## 68. The EU's fine against X is not about speech or ‘censorship’

**原文标题**: The EU's fine against X is not about speech or ‘censorship’

**原文链接**: [https://www.techpolicy.press/the-eus-fine-against-x-is-not-about-speech-or-censorship/](https://www.techpolicy.press/the-eus-fine-against-x-is-not-about-speech-or-censorship/)

生成摘要时出错

---

## 69. Self-referencing Page Tables for the x86-Architecture

**原文标题**: Self-referencing Page Tables for the x86-Architecture

**原文链接**: [https://0l.de/blog/2015/01/bachelor-thesis-abstract/](https://0l.de/blog/2015/01/bachelor-thesis-abstract/)

生成摘要时出错

---

## 70. Fuck You, I Won't Use Tailwind

**原文标题**: Fuck You, I Won't Use Tailwind

**原文链接**: [https://fuckyouiwontusetailwind.com](https://fuckyouiwontusetailwind.com)

生成摘要时出错

---

## 71. iOS 26.2 lockscreen clock is slowly moving left

**原文标题**: iOS 26.2 lockscreen clock is slowly moving left

**原文链接**: [https://twitter.com/ffaebi/status/2003548130936332519](https://twitter.com/ffaebi/status/2003548130936332519)

生成摘要时出错

---

## 72. An amateur codebreaker may have just solved the Black Dahlia and Zodiac killings

**原文标题**: An amateur codebreaker may have just solved the Black Dahlia and Zodiac killings

**原文链接**: [https://www.latimes.com/california/story/2025-12-23/black-dahlia-zodiac-killings-connected-one-killer-theory](https://www.latimes.com/california/story/2025-12-23/black-dahlia-zodiac-killings-connected-one-killer-theory)

生成摘要时出错

---

## 73. Custom Cross Compiler with Nix

**原文标题**: Custom Cross Compiler with Nix

**原文链接**: [https://www.hobson.space/posts/nixcross/](https://www.hobson.space/posts/nixcross/)

生成摘要时出错

---

## 74. Show HN: Kapso – WhatsApp for developers

**原文标题**: Show HN: Kapso – WhatsApp for developers

**原文链接**: [https://kapso.ai/](https://kapso.ai/)

生成摘要时出错

---

## 75. AI Withholds Life-or-Death Information Unless You Know the Magic Words

**原文标题**: AI Withholds Life-or-Death Information Unless You Know the Magic Words

**原文链接**: [https://substack.com/home/post/p-182524207](https://substack.com/home/post/p-182524207)

生成摘要时出错

---

## 76. No Longer Evil – new life for dead/outdated Nest Generation 1 and 2 thermostats

**原文标题**: No Longer Evil – new life for dead/outdated Nest Generation 1 and 2 thermostats

**原文链接**: [https://nolongerevil.com/](https://nolongerevil.com/)

生成摘要时出错

---

## 77. Spice: A 40-year old open-source success story (2011)

**原文标题**: Spice: A 40-year old open-source success story (2011)

**原文链接**: [https://www.edn.com/spice-a-40-year-old-open-source-success-story/](https://www.edn.com/spice-a-40-year-old-open-source-success-story/)

生成摘要时出错

---

## 78. Pantograph: Building a preschool for robots

**原文标题**: Pantograph: Building a preschool for robots

**原文链接**: [https://pantograph.com/blog/building-a-preschool-for-robots.html](https://pantograph.com/blog/building-a-preschool-for-robots.html)

生成摘要时出错

---

## 79. Show HN: Just Fucking Use Cloudflare – A satirical guide to the CF stack

**原文标题**: Show HN: Just Fucking Use Cloudflare – A satirical guide to the CF stack

**原文链接**: [https://justfuckingusecloudflare.com](https://justfuckingusecloudflare.com)

生成摘要时出错

---

## 80. US denies visas to ex-EU commissioner and others over social media rules

**原文标题**: US denies visas to ex-EU commissioner and others over social media rules

**原文链接**: [https://www.bbc.co.uk/news/articles/cp39kngz008o](https://www.bbc.co.uk/news/articles/cp39kngz008o)

生成摘要时出错

---

## 81. The Phone-Based Retirement Is Here

**原文标题**: The Phone-Based Retirement Is Here

**原文链接**: [https://www.theatlantic.com/technology/2025/12/do-your-parents-have-screen-time-problem/685424/](https://www.theatlantic.com/technology/2025/12/do-your-parents-have-screen-time-problem/685424/)

生成摘要时出错

---

## 82. Show HN: A local-first, reversible PII scrubber for AI workflows

**原文标题**: Show HN: A local-first, reversible PII scrubber for AI workflows

**原文链接**: [https://medium.com/@tj.ruesch/a-local-first-reversible-pii-scrubber-for-ai-workflows-using-onnx-and-regex-e9850a7531fc](https://medium.com/@tj.ruesch/a-local-first-reversible-pii-scrubber-for-ai-workflows-using-onnx-and-regex-e9850a7531fc)

生成摘要时出错

---

## 83. Name That Part: 3D Part Segmentation and Naming

**原文标题**: Name That Part: 3D Part Segmentation and Naming

**原文链接**: [https://name-that-part.github.io/](https://name-that-part.github.io/)

生成摘要时出错

---

## 84. Salmon Recipe

**原文标题**: Salmon Recipe

**原文链接**: [https://waveinscriber.com/posts/002-salmon-recipe/](https://waveinscriber.com/posts/002-salmon-recipe/)

生成摘要时出错

---

## 85. Judge in Vizio Case Rules on Issue Irrelevant to Rights Under Copyleft

**原文标题**: Judge in Vizio Case Rules on Issue Irrelevant to Rights Under Copyleft

**原文链接**: [https://sfconservancy.org/news/2025/dec/24/vizio-msa-irrelevant-ruling/](https://sfconservancy.org/news/2025/dec/24/vizio-msa-irrelevant-ruling/)

生成摘要时出错

---

## 86. Starlink satellite fails, polluting orbit with debris and falling toward Earth

**原文标题**: Starlink satellite fails, polluting orbit with debris and falling toward Earth

**原文链接**: [https://www.theregister.com/2025/12/23/starlink_satellite_fails_debris/](https://www.theregister.com/2025/12/23/starlink_satellite_fails_debris/)

生成摘要时出错

---

## 87. LAVD: Meta's New Default Scheduler [pdf]

**原文标题**: LAVD: Meta's New Default Scheduler [pdf]

**原文链接**: [https://lpc.events/event/19/contributions/2099/attachments/1875/4020/lpc-2025-lavd-meta.pdf](https://lpc.events/event/19/contributions/2099/attachments/1875/4020/lpc-2025-lavd-meta.pdf)

生成摘要时出错

---

## 88. A Father, a Son and Their $108B Push for Media Moguldom (Larry Ellison)

**原文标题**: A Father, a Son and Their $108B Push for Media Moguldom (Larry Ellison)

**原文链接**: [https://www.nytimes.com/2025/12/24/business/media/larry-david-ellison-warner-bros-discovery-cbs.html](https://www.nytimes.com/2025/12/24/business/media/larry-david-ellison-warner-bros-discovery-cbs.html)

生成摘要时出错

---

## 89. U.S. Bars 5 European Tech Regulators and Researchers

**原文标题**: U.S. Bars 5 European Tech Regulators and Researchers

**原文链接**: [https://www.nytimes.com/2025/12/23/technology/trump-rubio-european-tech-disinformation-digital-services-act.html](https://www.nytimes.com/2025/12/23/technology/trump-rubio-european-tech-disinformation-digital-services-act.html)

生成摘要时出错

---

## 90. Microspeak: North Star – The Old New Thing (2015)

**原文标题**: Microspeak: North Star – The Old New Thing (2015)

**原文链接**: [https://devblogs.microsoft.com/oldnewthing/20151103-00/?p=91861](https://devblogs.microsoft.com/oldnewthing/20151103-00/?p=91861)

生成摘要时出错

---

## 91. Ultra-Low-Latency Trading System

**原文标题**: Ultra-Low-Latency Trading System

**原文链接**: [https://submicro.krishnabajpai.me/](https://submicro.krishnabajpai.me/)

生成摘要时出错

---

## 92. Learn LaTeX in 30 Minutes

**原文标题**: Learn LaTeX in 30 Minutes

**原文链接**: [https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes)

生成摘要时出错

---

## 93. 2D Signed Distance Functions

**原文标题**: 2D Signed Distance Functions

**原文链接**: [https://iquilezles.org/articles/distfunctions2d/](https://iquilezles.org/articles/distfunctions2d/)

生成摘要时出错

---

## 94. Google Built Its Empire Scraping the Web. Now It's Suing a Scraper of Google

**原文标题**: Google Built Its Empire Scraping the Web. Now It's Suing a Scraper of Google

**原文链接**: [https://www.techdirt.com/2025/12/24/google-built-its-empire-scraping-the-web-now-its-suing-to-stop-others-from-scraping-google/](https://www.techdirt.com/2025/12/24/google-built-its-empire-scraping-the-web-now-its-suing-to-stop-others-from-scraping-google/)

生成摘要时出错

---

## 95. We Must Seize the Means of Compute

**原文标题**: We Must Seize the Means of Compute

**原文链接**: [https://thompson2026.com/blog/seize-the-means-of-compute/](https://thompson2026.com/blog/seize-the-means-of-compute/)

生成摘要时出错

---

## 96. Fixed-Wing Runway Design

**原文标题**: Fixed-Wing Runway Design

**原文链接**: [https://www.wbdg.org/building/aviation/fixed-wing-runway-design](https://www.wbdg.org/building/aviation/fixed-wing-runway-design)

生成摘要时出错

---

## 97. Nature Is Laughing at the AI Build Out

**原文标题**: Nature Is Laughing at the AI Build Out

**原文链接**: [https://markmaunder.com/2025/nature-is-laughing-at-the-ai-build-out/](https://markmaunder.com/2025/nature-is-laughing-at-the-ai-build-out/)

生成摘要时出错

---

## 98. Memory is running out, and so are excuses for software bloat

**原文标题**: Memory is running out, and so are excuses for software bloat

**原文链接**: [https://www.theregister.com/2025/12/23/memory_software_opinion/](https://www.theregister.com/2025/12/23/memory_software_opinion/)

生成摘要时出错

---

## 99. Linus - kernel copyright licence covers software, does not extend to hardware

**原文标题**: Linus - kernel copyright licence covers software, does not extend to hardware

**原文链接**: [https://social.kernel.org/notice/B1aR6QFuzksLVSyBZQ](https://social.kernel.org/notice/B1aR6QFuzksLVSyBZQ)

生成摘要时出错

---

## 100. Microsoft: "30% of Our Code Is AI." Also Microsoft: "Windows Is Broken."

**原文标题**: Microsoft: "30% of Our Code Is AI." Also Microsoft: "Windows Is Broken."

**原文链接**: [https://michael-dev-tech.github.io/Website/broken.html](https://michael-dev-tech.github.io/Website/broken.html)

生成摘要时出错

---

