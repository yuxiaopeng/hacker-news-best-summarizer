# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-08-10.md)

*最后自动更新时间: 2026-08-10 20:06:12*
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

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-08-10](output/hacker_news_summary_2026-08-10.md) |
| 2 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 3 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 4 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 5 | [2026-08-09](output/hacker_news_summary_2026-08-09.md) |
| 6 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 7 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 8 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 9 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 10 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 11 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 12 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 13 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 14 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 15 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 16 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 17 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 18 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 19 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 20 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 21 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 22 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 23 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 24 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 25 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 26 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 27 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 28 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 29 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 30 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 31 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 32 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 33 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 34 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 35 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 36 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 37 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 38 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 39 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 40 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 41 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 42 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 43 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 44 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 45 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 46 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 47 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 48 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 49 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 50 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 51 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 52 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 53 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 54 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 55 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 56 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 57 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 58 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 59 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 60 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 61 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 62 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 63 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 64 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 65 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 66 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 67 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 68 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 69 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 70 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 71 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 72 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 73 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 74 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 75 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 76 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 77 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 78 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 79 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 80 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 81 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 82 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 83 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 84 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 85 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 86 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 87 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 88 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 89 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 90 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 91 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 92 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 93 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 94 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 95 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 96 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 97 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 98 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 99 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 100 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 101 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 102 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 103 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 104 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 105 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 106 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 107 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 108 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 109 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 110 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 111 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 112 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 113 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 114 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 115 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 116 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 117 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 118 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 119 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 120 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 121 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 122 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 123 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 124 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 125 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 126 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 127 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 128 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 129 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 130 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 131 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 132 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 133 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 134 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 135 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 136 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 137 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 138 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 139 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 140 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 141 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 142 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 143 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 144 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 145 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 146 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 147 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 148 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 149 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 150 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 151 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 152 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 153 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 154 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 155 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 156 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 157 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 158 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 159 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 160 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 161 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 162 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 163 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 164 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 165 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 166 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 167 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 168 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 169 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 170 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 171 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 172 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 173 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 174 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 175 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 176 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 177 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 178 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 179 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 180 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 181 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 182 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 183 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 184 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 185 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 186 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 187 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 188 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 189 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 190 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 191 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 192 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 193 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 194 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 195 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 196 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 197 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 198 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 199 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 200 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 201 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 202 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 203 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 204 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 205 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 206 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 207 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 208 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 209 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 210 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 211 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 212 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 213 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 214 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 215 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 216 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 217 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 218 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 219 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 220 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 221 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 222 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 223 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 224 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 225 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 226 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 227 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 228 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 229 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 230 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 231 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 232 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 233 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 234 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 235 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 236 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 237 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 238 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 239 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 240 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 241 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 242 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 243 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 244 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 245 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 246 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 247 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 248 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 249 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 250 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 251 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 252 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 253 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 254 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 255 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 256 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 257 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 258 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 259 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 260 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 261 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 262 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 263 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 264 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 265 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 266 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 267 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 268 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 269 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 270 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 271 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 272 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 273 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 274 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 275 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
