# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2025-12-25.md)

*最后自动更新时间: 2025-12-25 19:47:07*
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

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 2 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 3 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 4 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 5 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 6 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 7 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 8 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 9 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 10 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 11 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 12 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 13 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 14 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 15 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 16 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 17 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 18 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 19 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 20 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 21 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 22 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 23 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 24 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 25 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 26 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 27 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 28 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 29 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 30 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 31 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 32 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 33 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 34 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 35 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 36 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 37 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 38 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 39 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 40 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 41 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 42 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 43 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 44 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 45 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 46 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 47 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 48 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 49 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
| 50 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
