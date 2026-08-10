# Hacker News 热门文章摘要 (2026-08-10)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 激励是给失败者的。

**原文标题**: Incentives are for losers

**原文链接**: [https://www.experimental-history.com/p/incentives-are-for-losers](https://www.experimental-history.com/p/incentives-are-for-losers)

在《激励是给失败者的》一文中，亚当·马斯特罗伊安尼（Adam Mastroianni）挑战了“社会问题仅仅源于‘不良激励’”这一普遍观点。他认为，这种心态暗示着激励 *应该* 被服从，将那些受其驱使而生活的人贬低为“傻瓜和笨蛋”。他声称，真正的人类发展在于获得个人目标感并磨砺自己的道德指南针，而不是追逐任意的外部奖励。

马斯特罗伊安尼指出，许多被金钱、权力和名声驱使而攀登社会阶梯的人，往往缺乏真正的信念，变得“精神上软弱无力”。他认为，发展一套健全的价值观是一项难以获得的技能，而非与生俱来的，这类似于学习阅读而非说话。他争辩说，大多数人只持有一些模糊的、“道德化的、治疗性的自然神论”信仰——一种“解释深度的幻觉”——因为他们肤浅的道德观在日常生活中“足够好用”，并且很少受到挑战。

为了形成更深刻的价值观，一个人必须直面一条“大而可怕的鱼”（Big Horrible Fish）：一个未经审视的根本性假设，如果对其进行充分思考，将必然导致个人生活的重大变革。作者回顾了自己的“鱼”时刻，即认识到学术界的社会正义论述与现实世界苦难之间的脱节。他引用了查尔斯·萨姆纳参议员的例子，萨姆纳藐视激励，为废奴主义信念冒生命危险，以此说明他是如何直面自己的“鱼”并培养出深刻正直品格的。文章倡导一种由自我审视的目标而非外部奖励驱动的生活。

---

## 2. 斯奎克 6.1

**原文标题**: Squeak 6.1

**原文链接**: [https://squeak.org/release_notes/6.1/](https://squeak.org/release_notes/6.1/)

Squeak 6.1 "Vanessa" 历经四年、合并逾1700个补丁后，标志着一次重要发布，并庆祝该系统近30周年。尽管主要为Squeak内部的交互体验进行了优化，但本发布说明将重点介绍平台上的各项重大进展。

主要改进包括：用于简化类和类别导航的新分层树形浏览器；Objectland（即“Squeak世界”）的重新引入，并附带交互式示例；以及针对进程和类重塑的核心内核基础设施的若干修复。工具集和用户界面也新增了用于代码检查、调试、性能分析和版本控制的各种功能。

Morphic 受益于树形UI组件的重大改版、文本编辑器增强功能以及大量UI调整，从而提升了稳定性、性能和高DPI支持。Objectland 携经典的BlobMorph回归，Etoys则恢复了教程并优化了游戏。编程工具得到了广泛增强，尤其是新增了支持拖放的树形浏览器、扩展了检查器功能（自定义字段、代理处理）以及显著的调试器升级。新的调试器功能包括用于精确搜索的“send until”、改进的“run to here”、用于VM指令的“byteCodes”模式，以及用于元循环评估器的“simulate”按钮。AndreasSystemProfiler现已集成，大量的UI调整，以及浏览器、检查器和变更恢复方面的稳定性修复，共同促成了这次全面的更新。

---

## 3. Mistral“代码实现的工具调用”专利

**原文标题**: Mistral Patent for “Code implemented tool calls”

**原文链接**: [https://patentsgazette.uspto.gov/week26/OG/html/1547-5/US12670045-20260630.html](https://patentsgazette.uspto.gov/week26/OG/html/1547-5/US12670045-20260630.html)

美国专利号 12,670,045 B1，题为“代码实现的工具调用”，已转让给 Mistral AI，发明人为 Gabriel Vergnaud。该专利于2026年3月4日提交。

该专利的核心描述了一种服务器通过大型语言模型（LLM）管理涉及外部工具调用的用户请求的方法。该过程如下：
1.  服务器接收到一个或多个工具调用的用户请求。
2.  LLM生成一个用编程语言编写的代码块，其中封装了这些工具调用。
3.  服务器在沙盒环境中执行该代码块。
4.  如果在执行期间有工具调用待处理，则暂停代码块的执行。
5.  随后，待处理的工具调用被传输到客户端进行外部执行。
6.  在从客户端接收到待处理工具调用的第一个结果后，服务器恢复代码块的执行，并用接收到的结果替换待处理的调用。
7.  最后，将已执行代码块的完整结果返回给LLM。

这种方法使LLM能够动态编排和管理工具交互，包括根据客户端工具的输出来暂停和恢复执行。

---

## 4. 在苹果Vision Pro上运行安卓ARM64 VR APK

**原文标题**: Run Android ARM64 VR APKs on Apple Vision Pro

**原文链接**: [https://github.com/shinyquagsire23/Klepton](https://github.com/shinyquagsire23/Klepton)

Klepton 是一个项目，旨在实现在 Apple Vision Pro 上执行 Android ARM64 VR APK，而无需即时 (JIT) 编译，尽管某些应用程序最终可能需要它来支持脚本运行时。

其核心技术是 `klepton-ld`，它将 Android 的 `.so` 库转换为兼容的 Apple `.dylib` 和 `.framework` 格式。Klepton 专门针对“Java-thin”应用程序，这意味着它不支持 Android 完整的 ART 运行时或 Java 虚拟机。

在图形方面，GLES 3.2 调用被转换为 ANGLE GLES 3.0（使用其 Metal 后端），Vulkan 调用由 MoltenVK 处理。Klepton 的运行时提供了 Android 的 Bionic C 库（映射到 `libSystem`）、NDK API（如 `ALooper`、`ANativeWindow`）、一个合成的 JNI 环境以及 Oculus VR 平台 (OVRP) 功能的重新实现。一个值得注意的技术细节是它修补了 Android 的 x18 寄存器使用方式，以避免与 macOS 约定冲突。

目前，Beat Saber 可以在 macOS 和 visionOS 上运行，但存在一些轻微的图形问题。针对 Steam VR Link 等应用程序的开发仍在进行中，并致力于提高整体通用性和构建工具。

---

## 5. 我所见人们思想极端化的主要方式 (2025)

**原文标题**: The main way I've seen people turn ideologically crazy (2025)

**原文链接**: [https://blog.andymasley.com/p/the-main-way-ive-seen-people-turn](https://blog.andymasley.com/p/the-main-way-ive-seen-people-turn)

文章描述了一种导致人们“思想狂热”的常见动态：人们产生一个极端想法，遇到大多是无知或非理性的批评，然后错误地认为，由于反对者的弱点，他们的信念更加正确。作者认为，这种“积极更新”是关键的错误。

这种情况的发生，是因为大多数人对复杂问题没有深入的了解或批判性思考。无论这个极端想法是什么（例如，马克思主义、素食主义、核政策），普通的批评很可能是混乱的、事实错误的或道德上过于简单的。信徒们常常将这种普遍的“困惑”解读为对自己观点的证实，感觉自己在“困惑之海”中身处“清醒之岛”，智力上高人一等。

为了避免这个陷阱，作者建议不要根据与普通人的互动来更新信念。相反，个人应该积极寻找那些了解该主题基本事实的、*最令人信服、消息灵通且不偏不倚的批评者*。这种“略显精英主义”的方法意味着只与那些真正“清醒”——求知欲强且有耐心——的人交流，无论他们持有何种特定意识形态。目标是将智力上的“清醒”感与自己的特定信念脱钩，防止因轻易驳斥无知反对者而产生的危险自我强化。

---

## 6. 复活四年旧的reMarkable 2

**原文标题**: Reviving a four year old reMarkable 2

**原文链接**: [https://oskrim.github.io/hardware/2026/08/09/remarkable-over-ssh.html](https://oskrim.github.io/hardware/2026/08/09/remarkable-over-ssh.html)

本文详细介绍了如何“复活”一台四年前的reMarkable 2电子纸平板，该设备之前无法进行云同步（错误0）和软件更新。

最初的“错误0”通过SSH连接到平板（使用USB IP 10.11.99.1，root用户和设备设置中的密码）来解决，即使用`timedatectl`命令校正不同步的时钟。具体操作是：禁用NTP（`set-ntp 0`），设置一个最近的日期（`set-time 'YYYY-MM-DD'`），然后重新启用NTP（`set-ntp 1`），从而允许了首次软件更新。

此后，云同步又因HTTP 400错误而失败，要求使用更高版本的应用程序。`journalctl`显示平板停留在3.11.2.5版本，并且由于重启后的网络解析问题，进一步的更新失败。重启更新服务（`systemctl restart swupdate.service update-engine.service`）后，平板得以更新到最新版本（3.27.3.0）。

值得注意的是，软件版本3.22及以上会静默禁用通过Wi-Fi进行的SSH连接；要重新启用它，用户必须通过USB进行SSH连接并运行`rm-ssh-over-wlan on`命令。

最后，由于新上传文件的云同步仍然无法使用，作者选择启用平板的可选网页服务器进行文件传输。这可以通过SSH编辑`xochitl.conf`文件（`WebInterfaceEnabled=true`）并重启`xochitl.service`来完成，或者直接通过设备用户界面（`设置 → 通用设置 → 存储 → USB网页界面`）进行设置。之后，可以使用`curl`命令直接将文件上传到平板的USB IP，作者发现这种方法比云同步更方便。

---

## 7. “变态眼镜”：Meta智能眼镜引来反弹，声浪日益高涨

**原文标题**: 'Pervert glasses': Backlash against Meta's smart glasses grows

**原文链接**: [https://www.seattletimes.com/business/technology/pervert-glasses-backlash-against-metas-smart-glasses-grows/](https://www.seattletimes.com/business/technology/pervert-glasses-backlash-against-metas-smart-glasses-grows/)

Meta新款雷朋智能眼镜因普遍存在的隐私担忧而面临强烈反弹，被广泛戏称为“变态眼镜”。批评者担心这款眼镜能够在没有充分告知被拍摄者的情况下隐秘地录制视频和音频，这引发了人们对在公共和私人场所被暗中录制的担忧。

一个主要争议点是其小巧的白色LED指示灯，许多人认为它不足以引起注意且容易被忽视，尤其是在明亮的环境或远距离时。社交媒体平台，特别是TikTok，通过病毒式视频放大了这些担忧，视频演示了人们如何在不知情的情况下轻易被录制，从而引发了人们呼吁在健身房、餐馆和酒吧等场所禁用这些眼镜。

这种情况与十年前困扰谷歌眼镜的“Glasshole”（眼镜混蛋）争议如出一辙，后者最终因类似的隐私焦虑导致其商业失败。尽管Meta坚称LED“不可能被忽视”，并强调用户教育和社区准则，但公众的不安和怀疑情绪依然高涨。早期用户报告称，陌生人因担心在不知情的情况下被录制而表现出负面反应。

Meta面临的挑战是如何克服这种“令人毛骨悚然”的看法，并说服公众该产品能够被负责任地使用，而这一障碍对其在智能眼镜市场的前辈来说是无法逾越的。日益增长的舆论表明，当前的隐私保护措施不足以平息公众的担忧。

---

## 8. John C. Lilly on solid state intelligence and the elimination of man (1978)

**原文标题**: John C. Lilly on solid state intelligence and the elimination of man (1978)

**原文链接**: [https://kibotronics.net/unlisted/lilly-machines/](https://kibotronics.net/unlisted/lilly-machines/)

生成摘要时出错

---

## 9. The tragedy of the commons, AI edition

**原文标题**: The tragedy of the commons, AI edition

**原文链接**: [https://www.economist.com/britain/2026/08/06/the-tragedy-of-the-commons-ai-edition](https://www.economist.com/britain/2026/08/06/the-tragedy-of-the-commons-ai-edition)

生成摘要时出错

---

## 10. How We Pushed CDC into Postgres

**原文标题**: How We Pushed CDC into Postgres

**原文链接**: [https://www.snowflake.com/en/blog/engineering/postgres-to-snowflake-replication-mirroring/](https://www.snowflake.com/en/blog/engineering/postgres-to-snowflake-replication-mirroring/)

生成摘要时出错

---

## 11. Parametron: 50s Japanese computer that uses neither transistors nor vacuum tubes

**原文标题**: Parametron: 50s Japanese computer that uses neither transistors nor vacuum tubes

**原文链接**: [https://ethw.org/Milestones:Parametron,_1954](https://ethw.org/Milestones:Parametron,_1954)

生成摘要时出错

---

## 12. Georgia police officers fired after Flock camera misuse

**原文标题**: Georgia police officers fired after Flock camera misuse

**原文链接**: [https://www.wtoc.com/2026/08/07/savannah-police-department-fires-6-employees-over-flock-safety-system-misuse/](https://www.wtoc.com/2026/08/07/savannah-police-department-fires-6-employees-over-flock-safety-system-misuse/)

生成摘要时出错

---

## 13. 50k Boat Names

**原文标题**: 50k Boat Names

**原文链接**: [https://www.beautifulpublicdata.com/boat-names/](https://www.beautifulpublicdata.com/boat-names/)

生成摘要时出错

---

## 14. New Zealand lost its music media, and what we're building to replace it

**原文标题**: New Zealand lost its music media, and what we're building to replace it

**原文链接**: [https://propelmusic.co.nz/articles/the-sound-went-quiet-nz-music-media](https://propelmusic.co.nz/articles/the-sound-went-quiet-nz-music-media)

生成摘要时出错

---

## 15. Tuxedo No. 2 – Cocktail recipes

**原文标题**: Tuxedo No. 2 – Cocktail recipes

**原文链接**: [https://tuxedono2.com](https://tuxedono2.com)

生成摘要时出错

---

## 16. Poland now 6th-largest EU economy, ahead of Switzerland and Belgium

**原文标题**: Poland now 6th-largest EU economy, ahead of Switzerland and Belgium

**原文链接**: [https://www.euronews.com/business/2026/08/09/poland-now-sixth-largest-eu-economy-ahead-of-switzerland-and-belgium](https://www.euronews.com/business/2026/08/09/poland-now-sixth-largest-eu-economy-ahead-of-switzerland-and-belgium)

生成摘要时出错

---

## 17. Should you stop cracking your knuckles?

**原文标题**: Should you stop cracking your knuckles?

**原文链接**: [https://www.bbc.com/future/article/20260807-should-i-stop-cracking-my-knuckles](https://www.bbc.com/future/article/20260807-should-i-stop-cracking-my-knuckles)

生成摘要时出错

---

## 18. Magnitude 7.4 Earthquake – 5 km S of San José del Palmar, Colombia

**原文标题**: Magnitude 7.4 Earthquake – 5 km S of San José del Palmar, Colombia

**原文链接**: [https://earthquake.usgs.gov/earthquakes/eventpage/us6000tjl2/executive](https://earthquake.usgs.gov/earthquakes/eventpage/us6000tjl2/executive)

生成摘要时出错

---

## 19. Saying No

**原文标题**: Saying No

**原文链接**: [https://rozumem.xyz/posts/19](https://rozumem.xyz/posts/19)

生成摘要时出错

---

## 20. Illinois just told every operating system to start reporting your kid's age

**原文标题**: Illinois just told every operating system to start reporting your kid's age

**原文链接**: [https://itsfoss.com/news/illinois-age-verification-bill/](https://itsfoss.com/news/illinois-age-verification-bill/)

生成摘要时出错

---

## 21. The Hacker's Renaissance (2025)

**原文标题**: The Hacker's Renaissance (2025)

**原文链接**: [https://phrack.org/issues/72/19#article](https://phrack.org/issues/72/19#article)

生成摘要时出错

---

## 22. Show HN: A Project Oberon System version running on RISC-V instead of RISC-5

**原文标题**: Show HN: A Project Oberon System version running on RISC-V instead of RISC-5

**原文链接**: [https://github.com/rochus-keller/OberonSystem/tree/op2-rv32](https://github.com/rochus-keller/OberonSystem/tree/op2-rv32)

生成摘要时出错

---

## 23. FCC moves to ban Lidar-equipped foreign drones from US

**原文标题**: FCC moves to ban Lidar-equipped foreign drones from US

**原文链接**: [https://www.tomshardware.com/tech-industry/drones/fcc-moves-to-ban-lidar-equipped-foreign-drones-from-us-classifies-the-technology-as-military-grade-in-a-proposal-that-could-also-hit-thermal-models-and-the-swarms-used-drone-light-shows](https://www.tomshardware.com/tech-industry/drones/fcc-moves-to-ban-lidar-equipped-foreign-drones-from-us-classifies-the-technology-as-military-grade-in-a-proposal-that-could-also-hit-thermal-models-and-the-swarms-used-drone-light-shows)

生成摘要时出错

---

## 24. Kinney Drugs pulls back AI phone assistant after hundreds of customer complaints

**原文标题**: Kinney Drugs pulls back AI phone assistant after hundreds of customer complaints

**原文链接**: [https://www.wcax.com/2026/08/07/kinney-drugs-pulls-back-ai-phone-assistant-after-hundreds-customer-complaints/](https://www.wcax.com/2026/08/07/kinney-drugs-pulls-back-ai-phone-assistant-after-hundreds-customer-complaints/)

生成摘要时出错

---

## 25. Japanese court overturns Red RAW video patent

**原文标题**: Japanese court overturns Red RAW video patent

**原文链接**: [https://www.dpreview.com/news/panasonic-did-what-apple-sony-and-nikon-couldnt-overturn-a-red-raw-video-patent/](https://www.dpreview.com/news/panasonic-did-what-apple-sony-and-nikon-couldnt-overturn-a-red-raw-video-patent/)

生成摘要时出错

---

## 26. Maryland Closes More of Cunningham Falls State Park After Second Beaver Attack

**原文标题**: Maryland Closes More of Cunningham Falls State Park After Second Beaver Attack

**原文链接**: [https://news.maryland.gov/dnr/2026/08/05/dnr-closes-additional-areas-of-cunningham-falls-state-park-following-second-beaver-attack/](https://news.maryland.gov/dnr/2026/08/05/dnr-closes-additional-areas-of-cunningham-falls-state-park-following-second-beaver-attack/)

生成摘要时出错

---

## 27. ChatGPT starts blocking direct requests to copy an author's style

**原文标题**: ChatGPT starts blocking direct requests to copy an author's style

**原文链接**: [https://arstechnica.com/ai/2026/07/chatgpt-stops-cloning-famous-writers-voices-but-may-capture-a-similar-feeling/](https://arstechnica.com/ai/2026/07/chatgpt-stops-cloning-famous-writers-voices-but-may-capture-a-similar-feeling/)

生成摘要时出错

---

## 28. Learning more about Claude's mathematical capabilities

**原文标题**: Learning more about Claude's mathematical capabilities

**原文链接**: [https://www.anthropic.com/research/riemann-zeta](https://www.anthropic.com/research/riemann-zeta)

生成摘要时出错

---

## 29. Study links GLP-1 drugs to bigger jump in women's employment than a degree

**原文标题**: Study links GLP-1 drugs to bigger jump in women's employment than a degree

**原文链接**: [https://finance.yahoo.com/healthcare/articles/harvard-study-links-glp-1-123000637.html](https://finance.yahoo.com/healthcare/articles/harvard-study-links-glp-1-123000637.html)

生成摘要时出错

---

## 30. Tail-call optimization in C is relatively recent (2025)

**原文标题**: Tail-call optimization in C is relatively recent (2025)

**原文链接**: [https://lwn.net/Articles/1034703/](https://lwn.net/Articles/1034703/)

生成摘要时出错

---

