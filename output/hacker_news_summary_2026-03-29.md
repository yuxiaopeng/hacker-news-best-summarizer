# Hacker News 热门文章摘要 (2026-03-29)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. GitLab 创始人通过创办公司抗癌

**原文标题**: Founder of GitLab battles cancer by founding companies

**原文链接**: [https://sytse.com/cancer/](https://sytse.com/cancer/)

GitLab创始人正在积极对抗骨肉瘤（上脊椎骨癌）。在用尽了标准医疗方案且找不到可用的临床试验后，他采取了一种赋权、自主的治疗方法。这包括寻求最大程度的诊断、创造新颖的治疗方法、实施并行治疗，现在，最重要的是，推广这种创新方法以造福其他患者。

他的抗癌历程在Elliot Hershberg的一篇文章、一个嵌入式的癌症历程幻灯片和一份OpenAI论坛演示文稿中得到了详尽记录。为了推广这种以患者为中心的方法，他正在evenone.ventures旗下成立新公司。他还在osteosarc.com公开分享他的个人健康数据，包括治疗时间表和25TB可公开访问的Google Cloud数据。

他主张建立一个以患者为先的医疗行业，并引用了一篇文章，该文章揭示了官僚障碍。对他的工作、数据或方法感兴趣的人可以订阅他的邮件列表，或直接通过cancer@sytse.com联系他。

---

## 2. 西班牙法律 Git 仓库

**原文标题**: Spanish legislation as a Git repo

**原文链接**: [https://github.com/EnriqueLop/legalize-es](https://github.com/EnriqueLop/legalize-es)

"Legalize — España" 将西班牙立法转化为一个Git仓库，为来自《国家官方公报》(BOE) 开放数据API的8600多部合并法律提供了一个版本控制系统。它包含这些法律自1960年以来的完整修订历史。

每部法律都是一个Markdown文件（例如，西班牙宪法的`BOE-A-1978-31229.md`），以包含标题、标识符和发布日期等元数据的YAML前言（frontmatter）开始。每项修订都记录为一个独立的Git提交，并在提交信息中附带其官方发布日期、标识符和指向来源的链接。

用户可以克隆此仓库，轻松搜索特定条款（使用`grep`）、查阅更改历史（使用`git log`），并获取修订的精确差异（使用`git diff`）。该仓库收录所有“国家级”合并立法，例如宪法、组织法和皇家法令。

内容来源于BOE的API，属于公共领域；本项目则增加了结构、版本控制和元数据。即将推出的Legalize API将提供编程访问接口，用于搜索、过滤、比较版本和接收通知。欢迎贡献，报告错误或缺失的修订。该项目由Enrique Lopez创建，其结构和工具采用MIT许可证。

---

## 3. AI过度肯定求助个人建议的用户

**原文标题**: AI overly affirms users asking for personal advice

**原文链接**: [https://news.stanford.edu/stories/2026/03/ai-advice-sycophantic-models-research](https://news.stanford.edu/stories/2026/03/ai-advice-sycophantic-models-research)

无法访问文章链接。

---

## 4. 我反编译了白宫的新应用

**原文标题**: I decompiled the White House's new app

**原文链接**: [https://thereallo.dev/blog/decompiling-the-white-house-app](https://thereallo.dev/blog/decompiling-the-white-house-app)

作者反编译了在iOS和安卓平台上均可使用的新“白宫”手机应用。该应用由美国数字服务局使用React Native技术开发，本质上是一个网页封装应用，显示的是whitehouse.gov的网页视图。这意味着内容是动态的，并非内嵌在应用本身中。

作者使用适用于安卓的jadx-gui和GHIDRA，以及适用于iOS的class-dump等工具，发现该应用极其基础，缺乏高级功能或复杂逻辑。主要发现包括：

*   **安全性：** 该应用在调试版本中明确允许出于调试目的进行不安全的HTTP连接，但重要的是，此选项在生产版本中已被禁用。其极简的原生代码中没有明显的严重安全漏洞，因为大多数交互都是通过网页视图进行的。
*   **隐私：** 它利用Google Analytics进行跟踪，并包含一个“联系我们”功能，该功能直接在网页视图中打开whitehouse.gov的联系页面。应用程序的原生代码似乎不直接处理个人数据。
*   **权限：** 安卓应用请求最少的权限：INTERNET和ACCESS_NETWORK_STATE。
*   **未混淆：** 代码未混淆，使反编译变得简单直接。
*   **极简性：** 该应用的简洁性表明它主要作为访问白宫网站的便捷快捷方式，而非提供独特的应用专属功能。

作者总结道，该应用是一个简单、实用的网站封装应用，结构良好，符合其目的，且不包含通过反编译发现的任何隐藏的恶意代码或严重漏洞。其主要价值在于方便用户访问白宫的在线平台。

---

## 5. 严格对待代理，而非文件系统

**原文标题**: Go hard on agents, not on your filesystem

**原文链接**: [https://jai.scs.stanford.edu/](https://jai.scs.stanford.edu/)

严管AI代理，而非您的文件系统。jai是一款免费软件工具，旨在Linux上轻松隔离AI代理。它通过提供轻量级沙盒解决方案，解决了AI工具导致意外数据丢失（从清空主目录到丢失开发项目）的关键问题。

jai填补了在赋予AI代理完全机器访问权限与设置完整容器或虚拟机的复杂性之间的鸿沟。通过一个简单的命令（`jai your-agent`），它创建了一个安全的环境：您的当前工作目录保持完全可写，您的主目录受写时复制（copy-on-write）叠加保护（或完全隐藏），所有其他文件系统均为只读。这显著减少了在快速编码帮助、一次性任务或运行未知脚本时的“爆炸半径”（潜在损害范围）。

它提供了三种模式——休闲（Casual）、严格（Strict）和裸机（Bare）——以适应不同的隔离需求，在便利性和安全性之间取得平衡。虽然它不能替代Docker等强大的容器运行时或用于多租户强隔离的虚拟机，但jai作为一个“休闲沙盒”，使代理隔离比在YOLO模式下运行代理更容易。由斯坦福大学开发，jai旨在通过使文件系统保护变得简单易用，从而促进更安全的AI交互。

---

## 6. 真正地让 macOS 持续烂下去

**原文标题**: Make macOS consistently bad unironically

**原文链接**: [https://lr0.org/blog/p/macos/](https://lr0.org/blog/p/macos/)

作者批评macOS 26存在“臭名昭著的窗口圆角不一致问题”，凸显了UI设计中过度圆润化的“丑陋”趋势，YouTube即是其例。尽管作者认为圆角本身尚有争议，但应用程序之间的*不一致性*则被认为非常恼人。

许多用户试图通过取消圆角化来纠正这个问题，这通常需要禁用系统完整性保护 (SIP) 来修改Safari等系统应用程序。作者基于安全考虑反对禁用SIP，尽管他也承认，如果系统已经受到威胁，SIP的有效性备受争议。

相反，作者提出了一种解决方案，旨在使*所有*窗口圆角都*保持一致地更加圆润*。这种方法通过仅针对用户应用程序来避免禁用SIP。文章提供了一个技术实现，使用Objective-C代码混编（swizzle）第三方GUI应用程序的`NSThemeFrame`方法（例如`_cornerRadius`和`_topCornerSize`），设置统一的`kDesiredCornerRadius`（例如23.0）。文章包含了编译此动态库、对其签名，并通过`LaunchAgent` plist利用`DYLD_INSERT_LIBRARIES`在启动时加载它的说明。其目的是实现一个“一致的糟糕”UI，将统一性置于可能存在缺陷的默认美学之上。

---

## 7. 欧洲抵制帕兰提尔

**原文标题**: Say No to Palantir in Europe

**原文链接**: [https://action.wemove.eu/sign/2026-03-palantir-petition-EN](https://action.wemove.eu/sign/2026-03-palantir-petition-EN)

This petition, "Say No to Palantir in Europe," urges European governments and the EU to halt the expansion of US surveillance company Palantir. It calls on governments to stop signing new contracts, review and phase out existing ones, and invest in transparent European alternatives. The EU is pressed to investigate Palantir's operations, ensure full transparency over contracts and data use, and push for a halt to new deals until strong safeguards are guaranteed.

The petition argues that Europe must not entrust its public systems, data, and security to a private US company known for enabling controversial actions, including alleged genocide in Gaza, family separations by ICE, and fueling wars. Palantir, often operating out of public sight, is quietly gaining access to sensitive public data and systems across Europe, from police tracking in Germany to healthcare datasets in the UK. The company's CEO, Alex Karp, has openly stated aggressive intentions. The petition aims to build momentum, expose Palantir's activities, and prevent the expansion of mass surveillance and the handover of Europe's data and security to a foreign spy-tech giant.

---

## 8. CSS 劫数难逃

**原文标题**: CSS is DOOMed

**原文链接**: [https://nielsleenheer.com/articles/2026/css-is-doomed-rendering-doom-in-3d-with-css/](https://nielsleenheer.com/articles/2026/css-is-doomed-rendering-doom-in-3d-with-css/)

生成摘要时出错

---

## 9. 丁腈和乳胶手套可能导致微塑料高估

**原文标题**: Nitrile and latex gloves may cause overestimation of microplastics

**原文链接**: [https://news.umich.edu/nitrile-and-latex-gloves-may-cause-overestimation-of-microplastics-u-m-study-reveals/](https://news.umich.edu/nitrile-and-latex-gloves-may-cause-overestimation-of-microplastics-u-m-study-reveals/)

生成摘要时出错

---

## 10. I Built an Open-World Engine for the N64 [video]

**原文标题**: I Built an Open-World Engine for the N64 [video]

**原文链接**: [https://www.youtube.com/watch?v=lXxmIw9axWw](https://www.youtube.com/watch?v=lXxmIw9axWw)

生成摘要时出错

---

## 11. Britain today generating 90%+ of electricity from renewables

**原文标题**: Britain today generating 90%+ of electricity from renewables

**原文链接**: [https://grid.iamkate.com/](https://grid.iamkate.com/)

生成摘要时出错

---

## 12. South Korea Mandates Solar Panels for Public Parking Lots

**原文标题**: South Korea Mandates Solar Panels for Public Parking Lots

**原文链接**: [https://www.reutersconnect.com/item/south-korea-mandates-solar-panels-for-public-parking-lots/dGFnOnJldXRlcnMuY29tLDIwMjY6bmV3c21sX01UMU5VUlBITzAwMFZKRjFZQQ](https://www.reutersconnect.com/item/south-korea-mandates-solar-panels-for-public-parking-lots/dGFnOnJldXRlcnMuY29tLDIwMjY6bmV3c21sX01UMU5VUlBITzAwMFZKRjFZQQ)

生成摘要时出错

---

## 13. CERN uses ultra-compact AI models on FPGAs for real-time LHC data filtering

**原文标题**: CERN uses ultra-compact AI models on FPGAs for real-time LHC data filtering

**原文链接**: [https://theopenreader.org/Journalism:CERN_Uses_Tiny_AI_Models_Burned_into_Silicon_for_Real-Time_LHC_Data_Filtering](https://theopenreader.org/Journalism:CERN_Uses_Tiny_AI_Models_Burned_into_Silicon_for_Real-Time_LHC_Data_Filtering)

生成摘要时出错

---

## 14. Cocoa-Way – Native macOS Wayland compositor for running Linux apps seamlessly

**原文标题**: Cocoa-Way – Native macOS Wayland compositor for running Linux apps seamlessly

**原文链接**: [https://github.com/J-x-Z/cocoa-way](https://github.com/J-x-Z/cocoa-way)

生成摘要时出错

---

## 15. AMD's Ryzen 9 9950X3D2 Dual Edition crams 208MB of cache into a single chip

**原文标题**: AMD's Ryzen 9 9950X3D2 Dual Edition crams 208MB of cache into a single chip

**原文链接**: [https://arstechnica.com/gadgets/2026/03/amds-ryzen-9-9950x3d2-dual-edition-crams-208mb-of-cache-into-a-single-chip/](https://arstechnica.com/gadgets/2026/03/amds-ryzen-9-9950x3d2-dual-edition-crams-208mb-of-cache-into-a-single-chip/)

生成摘要时出错

---

## 16. Folk are getting dangerously attached to AI that always tells them they're right

**原文标题**: Folk are getting dangerously attached to AI that always tells them they're right

**原文链接**: [https://www.theregister.com/2026/03/27/sycophantic_ai_risks/](https://www.theregister.com/2026/03/27/sycophantic_ai_risks/)

生成摘要时出错

---

## 17. DOJ confirms FBI Director Kash Patel's personal email was hacked

**原文标题**: DOJ confirms FBI Director Kash Patel's personal email was hacked

**原文链接**: [https://arstechnica.com/tech-policy/2026/03/doj-confirms-fbi-director-kash-patels-personal-email-was-hacked/](https://arstechnica.com/tech-policy/2026/03/doj-confirms-fbi-director-kash-patels-personal-email-was-hacked/)

生成摘要时出错

---

## 18. Further human + AI + proof assistant work on Knuth's "Claude Cycles" problem

**原文标题**: Further human + AI + proof assistant work on Knuth's "Claude Cycles" problem

**原文链接**: [https://twitter.com/BoWang87/status/2037648937453232504](https://twitter.com/BoWang87/status/2037648937453232504)

生成摘要时出错

---

## 19. Linux is an interpreter

**原文标题**: Linux is an interpreter

**原文链接**: [https://astrid.tech/2026/03/28/0/linux-is-an-interpreter/](https://astrid.tech/2026/03/28/0/linux-is-an-interpreter/)

生成摘要时出错

---

## 20. Miasma: A tool to trap AI web scrapers in an endless poison pit

**原文标题**: Miasma: A tool to trap AI web scrapers in an endless poison pit

**原文链接**: [https://github.com/austin-weeks/miasma](https://github.com/austin-weeks/miasma)

生成摘要时出错

---

## 21. Police used AI facial recognition to wrongly arrest TN woman for crimes in ND

**原文标题**: Police used AI facial recognition to wrongly arrest TN woman for crimes in ND

**原文链接**: [https://www.cnn.com/2026/03/29/us/angela-lipps-ai-facial-recognition](https://www.cnn.com/2026/03/29/us/angela-lipps-ai-facial-recognition)

生成摘要时出错

---

## 22. ISBN Visualization

**原文标题**: ISBN Visualization

**原文链接**: [https://annas-archive.gd/isbn-visualization?](https://annas-archive.gd/isbn-visualization?)

生成摘要时出错

---

## 23. The first 40 months of the AI era

**原文标题**: The first 40 months of the AI era

**原文链接**: [https://lzon.ca/posts/other/thoughts-ai-era/](https://lzon.ca/posts/other/thoughts-ai-era/)

生成摘要时出错

---

## 24. Voyager 1 runs on 69 KB of memory and an 8-track tape recorder

**原文标题**: Voyager 1 runs on 69 KB of memory and an 8-track tape recorder

**原文链接**: [https://techfixated.com/a-1977-time-capsule-voyager-1-runs-on-69-kb-of-memory-and-an-8-track-tape-recorder-4/](https://techfixated.com/a-1977-time-capsule-voyager-1-runs-on-69-kb-of-memory-and-an-8-track-tape-recorder-4/)

生成摘要时出错

---

## 25. Alzheimer's disease mortality among taxi and ambulance drivers (2024)

**原文标题**: Alzheimer's disease mortality among taxi and ambulance drivers (2024)

**原文链接**: [https://www.bmj.com/content/387/bmj-2024-082194](https://www.bmj.com/content/387/bmj-2024-082194)

生成摘要时出错

---

## 26. Velxio 2.0 – Emulate Arduino, ESP32, and Raspberry Pi 3 in the Browser

**原文标题**: Velxio 2.0 – Emulate Arduino, ESP32, and Raspberry Pi 3 in the Browser

**原文链接**: [https://github.com/davidmonterocrespo24/velxio](https://github.com/davidmonterocrespo24/velxio)

生成摘要时出错

---

## 27. Slovenia becomes first EU country to introduce fuel rationing

**原文标题**: Slovenia becomes first EU country to introduce fuel rationing

**原文链接**: [https://www.bbc.com/news/articles/c77m4zx6zvmo](https://www.bbc.com/news/articles/c77m4zx6zvmo)

生成摘要时出错

---

## 28. OpenCiv1 – open-source rewrite of Civ1

**原文标题**: OpenCiv1 – open-source rewrite of Civ1

**原文链接**: [https://github.com/rajko-horvat/OpenCiv1](https://github.com/rajko-horvat/OpenCiv1)

生成摘要时出错

---

