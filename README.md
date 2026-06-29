# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-06-29.md)

*最后自动更新时间: 2026-06-29 21:02:26*
## 1. 寻路者路由器：本地与托管LLM之间的确定性查询路由

**原文标题**: Wayfinder Router: deterministic routing of queries between local and hosted LLM

**原文链接**: [https://github.com/itsthelore/wayfinder-router](https://github.com/itsthelore/wayfinder-router)

Wayfinder Router是一个离线、确定性工具，旨在根据LLM查询的复杂性进行路由，从而优化成本和延迟。它不通过模型调用来做决策，而是根据每个提示的结构（长度、标题、列表、代码）以及可选地根据措辞（证明、数学、约束）进行评分，生成一个0.0到1.0的复杂性分数。“简单”的提示会被路由到本地/小型模型，而“困难”的提示则会发送到更大、通常更昂贵、托管模型。

这种路由决策在毫秒级以下完成，完全离线且是确定性的，决策过程本身不需要API密钥或网络调用。这与大多数路由器形成对比，后者通过使用训练好的分类器或LLM判断器，带来延迟、成本和随机性。

Wayfinder作为OpenAI兼容的API网关运行。用户只需将其现有客户端的`base_url`指向Wayfinder，Wayfinder随后会透明地将请求转发到选定的本地（例如Ollama、vLLM）或托管（例如OpenAI、Groq）后端。它支持自托管，并允许用户根据自己的数据进行校准，以调整路由阈值或层级，包括考虑成本的目标。

配置通过一个`wayfinder-router.toml`文件完成，用于指定模型和路由逻辑。单个请求可以通过`model`字段（例如`model="local"`）、`X-Wayfinder-Threshold`头部，或消息内的斜杠指令来覆盖默认路由，实现精细控制。该系统确保LLM使用的一致性、效率和成本效益。

---

## 2. CachyOS 2026年6月发布

**原文标题**: CachyOS June 2026 Release

**原文链接**: [https://cachyos.org/blog/2606-june-release/](https://cachyos.org/blog/2606-june-release/)

CachyOS 2026年6月版本是本年度的第四个版本，引入了全新的CachyOS Hyprland Noctalia桌面选项，并在安装程序中附带了预览视频。

为Python工作负载扩展了PGO，并通过GCC补丁改进了现代CPU上的x86分支预测错误调优，从而提升了性能。Pacman现在为脚本和钩子提供了网络隔离，并修复了高核心数CPU上OpenBLAS的性能退化问题。Proton-cachyos已更名为proton-cachyos-native。

安装程序移除了paru，推荐使用Shelly；MangoWM现在使用SDDM。GNOME系统监视器被Resources取代，实时会话键盘检测得到改进。

CachyOS-Welcome通过blocky增加了对DNS-over-QUIC (DoQ) 的支持、一个专门的故障排除页面、Ptyxis终端支持，以及新增阿塞拜疆语和希腊语本地化。chwd现在可以解决多GPU驱动冲突，包含一个用于虚拟机的32位Vulkan驱动，并增加了土耳其语本地化。cachyos-settings应用了用户服务超时设置（启动15秒，关机10秒），以防止90秒的关机延迟。

主要修复包括修正了安装程序配置（键盘、区域设置、pacman）、正确的Calamares清理，以及CachyOS-Welcome的稳定性改进，防止了与应用程序安装或不可读设置相关的崩溃。现有用户可以通过`sudo pacman -Syu`进行更新。

---

## 3. 奥地利游说欧盟，在美国准入限制后争取安索罗匹克落户

**原文标题**: Austria Lobbies EU to Host Anthropic After US Access Curbs

**原文链接**: [https://www.bloomberg.com/news/articles/2026-06-28/austria-lobbies-eu-to-host-anthropic-after-us-access-curbs](https://www.bloomberg.com/news/articles/2026-06-28/austria-lobbies-eu-to-host-anthropic-after-us-access-curbs)

生成摘要时出错

---

## 4. 一名农民因在数据中心会议上超时5秒被捕

**原文标题**: A Farmer Arrested for Going 5 Seconds over His Time Limit at Data Center Meeting

**原文链接**: [https://www.gadgetreview.com/arrest-him-the-moment-police-handcuffed-a-farmer-for-going-5-seconds-over-his-time-limit-at-data-center-meeting](https://www.gadgetreview.com/arrest-him-the-moment-police-handcuffed-a-farmer-for-going-5-seconds-over-his-time-limit-at-data-center-meeting)

克莱尔莫尔居民达伦·布兰查德在二月的一次市议会会议上，因在公开评论环节发言略微超出三分钟限制，而被捕并被控非法侵入。该事件发生在一场讨论“野马项目”的会议上，该项目是一个拟议的占地300英亩的数据中心园区。

执法记录仪录像显示，在布兰查德要求提交文件后，警官将其逮捕。该录像是一名当地申请人最初费尽周折才获得的（最初报价1750美元，最终支付120美元）。据报道，布兰查德的法律团队已提交动议要求撤销指控，并要求市检察官回避，声称此次逮捕是对受保护言论的报复，并已经遏制了社区参与。

由贝尔基础设施公司开发的“野马项目”是一个多栋建筑的数据中心，面临着居民的反对。许多居民认为，关键的项目条款和激励措施是在有意义的公众意见征集之前确定的，引发了对用水量、电力需求、耕地流失以及未核算成本的担忧。尽管官员们将其定位为经济发展，但反对者则认为这是一个高影响的工业项目。

此次逮捕引发了关于超出公众评论时间几秒是否足以构成非法侵入罪的辩论，并凸显了当大型基础设施项目引入时，城镇如何处理异议的更广泛问题。

---

## 5. Show HN: DRM-Free Books

**原文标题**: Show HN: DRM-Free Books

**原文链接**: [https://frequal.com/Perspectives/DrmFreeAuthors.html](https://frequal.com/Perspectives/DrmFreeAuthors.html)

本文题为《Show HN：无DRM图书》，重点介绍了提供无数字版权管理（DRM）图书的作者和平台。

文章介绍了三位当代作者：
*   **安德鲁·奥利弗**：他的悬疑小说《手段与动机》可在亚马逊和巴诺书店购买，并提供免费的EPUB和PDF试读章节。
*   **蒂莫西·扎恩**：他的科幻小说《伊卡洛斯之针》可在Baen出版社购买。
*   **凯西·埃泽尔**：她的奇幻小说《沙中血迹》也可在Baen出版社购买。

文章接着提供了查找更多无DRM图书的指南：
*   **亚马逊（Amazon）**：查找提供EPUB和PDF下载的图书。
*   **TOR出版社**：该出版社的所有图书十多年来一直都是无DRM的。
*   **Baen出版社**：查找明确标明“本书不含DRM”的标题。
*   **Bookshop.org**：在搜索结果中使用“格式/电子书/无DRM”筛选器。
*   **科里·多克托罗（Cory Doctorow）**：他所有的电子书均不含DRM销售。

最后，对于已过版权保护期的无DRM图书，文章推荐**古腾堡计划（Project Gutenberg）**和**标准电子书（Standard Ebooks）**。

---

## 6. 教育体系的初衷是培养独立的、批判性思考者 (2024)

**原文标题**: The origins of the school system aimed to produce independent, critical thinkers (2024)

**原文链接**: [https://www.cbc.ca/radio/ideas/humboldt-education-system-bildung-1.7172093](https://www.cbc.ca/radio/ideas/humboldt-education-system-bildung-1.7172093)

两百年前，普鲁士哲学家威廉·冯·洪堡迅速创建了公共教育体系和现代研究型大学，这些体系如今已被全球采纳。他哲学的核心是“教养”（Bildung）——一个源于宗教根源的概念，旨在表明个体充分发挥其内在潜能并培养自我修养。

受让-雅克·卢梭的影响，洪堡认为教育应该发展人的能力，摆脱商业或国家需求等外部限制。他设想了一个教导学生“如何学习”的体系，鼓励批判性思维、独立研究以及对高深理论和哲学的理解，而非仅仅死记硬背。他认为，这将培养出具有自我意识的独立思考者，乃至能理解政策原则、更高效的公务员。

洪堡的抱负是创建一个由智力卓越的个体组成的社会，这些个体能够改善他们的世界。然而，随着他的公共教育体系在全球范围内被采纳和修改，“教养”（即人类潜能的培养）这一关键要素却常常被忽视。随着时间的推移，国家的影响和议程开始塑造教育，这可能偏离了洪堡最初关于个体全面发展的愿景。

---

## 7. Bashblog — 一个单一的 Bash 脚本，用于创建博客

**原文标题**: Bashblog – a single bash script to create blogs

**原文链接**: [https://github.com/cfenollosa/bashblog](https://github.com/cfenollosa/bashblog)

Bashblog 是一个独特的、单一的 Bash 脚本，旨在创建简单、无依赖的博客。它允许用户以极低的要求将博客文章发布到公共服务器文件夹，可在 GNU/Linux、OSX 和 BSD 上运行。其用法简单明了：将 `bb.sh` 复制到一个公共文件夹，然后输入 `./bb.sh post` 即可开始撰写您的博客文章，默认支持 Markdown。

主要功能包括超简单的操作，无需安装或模板，仅依赖于 `date`、`grep` 和 `sed` 等基础系统工具。它自动生成静态 HTML 内容、RSS 订阅源以及标签/分类页面。Bashblog 还支持草稿、Disqus 评论、Twitter 集成、Feedburner 和 Google Analytics。附带一个简洁的样式表，并且每次发布新文章时网站都会自动备份。

配置灵活，用户可以直接在 `bb.sh` 中修改变量，也可以使用 `.config` 文件覆盖它们，这有助于更轻松地进行更新。该项目强调极简主义和可维护性，欢迎错误修复，但新功能需要充分的理由才能被采纳，以保持其简洁的代码库并遵循 UNIX 哲学。Bashblog 采用 GNU 通用公共许可证 v3 许可。

---

## 8. 更多证据与火星上可能存在的古代生命一致 (2025)

**原文标题**: More evidence is consistent with possible ancient life on Mars (2025)

**原文链接**: [https://www.cbc.ca/radio/quirks/more-evidence-of-life-on-mars-but-still-no-life-1.7649645](https://www.cbc.ca/radio/quirks/more-evidence-of-life-on-mars-but-still-no-life-1.7649645)

NASA's Perseverance rover has found new geological evidence consistent with possible ancient life on Mars, though definitive proof remains elusive. In July 2024, the rover discovered vivianite and greigite in a former river delta, chemicals often formed by microbial activity on Earth. However, these formations can also result from non-biological chemical reactions.

This latest finding adds to a long history of tantalizing clues and subsequent debunkings, starting with Percival Lowell's mistaken observation of Martian canals in 1894. Later robotic missions revealed dried riverbeds, suggesting past water and thus potential life. In 1976, Viking landers detected reactions consistent with microbes but found no organic molecules. The 1996 discovery of a worm-like structure in a Martian meteorite also faced non-biological explanations, though NASA's Curiosity rover recently detected complex organic molecules, reigniting the debate.

Despite over a century of exploration, no conclusive evidence of surface life has been found. Scientists are now increasingly focusing on the possibility of life thriving deep within the Martian crust, similar to Earth's underground microbial ecosystems. This shielded environment, potentially with liquid water beneath a permafrost layer, represents a promising new avenue for future exploration, suggesting astronauts may need to drill deep to uncover Mars' secrets.

---

## 9. Reflections on software engineering in the age of AI

**原文标题**: Reflections on software engineering in the age of AI

**原文链接**: [https://adiamond.me/2026/06/software-engineering-in-the-age-of-ai/](https://adiamond.me/2026/06/software-engineering-in-the-age-of-ai/)

生成摘要时出错

---

## 10. Building Principia for Windows XP

**原文标题**: Building Principia for Windows XP

**原文链接**: [https://voxelmanip.se/2026/06/28/building-principia-for-windows-xp/](https://voxelmanip.se/2026/06/28/building-principia-for-windows-xp/)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 2 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 3 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 4 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 5 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 6 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 7 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 8 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 9 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 10 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 11 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 12 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 13 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 14 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 15 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 16 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 17 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 18 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 19 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 20 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 21 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 22 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 23 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 24 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 25 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 26 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 27 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 28 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 29 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 30 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 31 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 32 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 33 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 34 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 35 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 36 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 37 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 38 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 39 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 40 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 41 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 42 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 43 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 44 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 45 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 46 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 47 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 48 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 49 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 50 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 51 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 52 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 53 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 54 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 55 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 56 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 57 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 58 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 59 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 60 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 61 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 62 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 63 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 64 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 65 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 66 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 67 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 68 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 69 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 70 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 71 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 72 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 73 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 74 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 75 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 76 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 77 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 78 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 79 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 80 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 81 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 82 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 83 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 84 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 85 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 86 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 87 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 88 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 89 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 90 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 91 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 92 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 93 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 94 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 95 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 96 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 97 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 98 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 99 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 100 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 101 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 102 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 103 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 104 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 105 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 106 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 107 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 108 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 109 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 110 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 111 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 112 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 113 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 114 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 115 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 116 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 117 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 118 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 119 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 120 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 121 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 122 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 123 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 124 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 125 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 126 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 127 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 128 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 129 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 130 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 131 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 132 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 133 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 134 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 135 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 136 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 137 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 138 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 139 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 140 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 141 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 142 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 143 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 144 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 145 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 146 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 147 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 148 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 149 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 150 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 151 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 152 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 153 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 154 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 155 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 156 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 157 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 158 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 159 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 160 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 161 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 162 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 163 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 164 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 165 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 166 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 167 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 168 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 169 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 170 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 171 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 172 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 173 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 174 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 175 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 176 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 177 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 178 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 179 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 180 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 181 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 182 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 183 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 184 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 185 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 186 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 187 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 188 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 189 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 190 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 191 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 192 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 193 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 194 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 195 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 196 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 197 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 198 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 199 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 200 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 201 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 202 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 203 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 204 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 205 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 206 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 207 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 208 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 209 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 210 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 211 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 212 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 213 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 214 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 215 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 216 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 217 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 218 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 219 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 220 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 221 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 222 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 223 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 224 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 225 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 226 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 227 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 228 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 229 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
| 230 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 231 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 232 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 233 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 234 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
