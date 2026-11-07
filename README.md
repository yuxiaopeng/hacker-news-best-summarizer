# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-11-07.md)

*最后自动更新时间: 2026-11-07 00:04:29*
## 1. 混蛋

**原文标题**: sshole

**原文链接**: [https://sshhole.com](https://sshhole.com)

文章深入探讨了Unix安全性的早期历史，特别是1980年的`/etc/passwd`文件。在那个时代，包含用户名及其对应密码哈希值的`passwd`文件对所有用户都是可读的。

Bill Joy为不用于直接用户登录的账户引入了一个简单而有效的安全措施。对于`daemon`账户，他将密码哈希值替换为一个星号（`*`）。由于`*`不是一个有效的哈希值，任何密码都无法匹配它，从而阻止任何人登录该账户。这种禁用登录的方法至今仍在类Unix系统中沿用。

更添幽默的是，Joy还将`daemon`账户的真实姓名字段填写为描述性短语“the devil himself”。这一历史细节保存在1980年的3BSD `/etc/passwd`文件中。

---

## 2. Claude Code 将你的电子邮件地址发送给网站

**原文标题**: Claude Code sends your email address to websites

**原文链接**: [https://github.com/anthropics/claude-code/issues/107757](https://github.com/anthropics/claude-code/issues/107757)

GitHub上的一份bug报告（Issue #107757，2026年11月5日）揭示了AI编码工具Claude Code中一个重要的隐私漏洞。用户taylor-edwards报告称，Claude在进行网络搜索时，通过User-Agent HTTP标头将他们的电子邮件地址泄露给任意第三方，导致他们收到了大量的诈骗邮件。报告者强调，这种行为是未经授权的，应该被永久移除，而不仅仅是一个选择退出设置，因为它损害了匿名性并使恶意行为者受益。

mkubenka的进一步调查显示，Claude不仅泄露电子邮件地址，还泄露项目或客户名称，可能将用户身份与特定工作关联起来。即使Claude编写并执行脚本，绕过现有防护措施，也观察到了这种情况。

开发者poteat宣布，2.1.317及更高版本中引入了一个内置隐私模块（cc-plugin-privacy），默认启用，以阻止这种行为。然而，mkubenka批判了这一解决方案，指出它只针对账户邮箱，仍允许项目名称泄露，并且如果Claude将邮件地址直接集成到它生成并运行的脚本中，则该解决方案可能被绕过。

这个问题在社区中引发了广泛的担忧和负面反响，表达了对Anthropic隐私实践的严重不信任。许多评论者强调，隐私应该是该工具的一项基本且不可选的方面，主张默认使用通用的User-Agent标头，除非用户明确同意提供个性化信息。

---

## 3. 特斯拉将逐步停产赛博卡车

**原文标题**: Tesla to wind down Cybertruck production

**原文链接**: [https://www.nbcnews.com/tech/tech-news/tesla-wind-cybertruck-production-years-poor-sales-markets-rcna607817](https://www.nbcnews.com/tech/tech-news/tesla-wind-cybertruck-production-years-poor-sales-markets-rcna607817)

特斯拉首席执行官埃隆·马斯克宣布，该公司将于2027年中期之前，逐步停止其德克萨斯超级工厂的Cybertruck生产。这一决定是由于这款未来派皮卡（于2023年末首次交付）多年来销售持续疲软所致，旨在为新推出的Cybercab车型增加产量让路，该车型是特斯拉机器人出租车宏伟计划的核心。

尽管马斯克将其吹捧为“特斯拉有史以来最好的汽车”，但其销量却远未达到目标。去年，Cybertruck在美国仅售出20,237辆，较2024年的38,965辆下降了48%，远低于马斯克此前预测的每年25万辆。前阿斯顿·马丁首席执行官安迪·帕尔默称，由于未能实现目标，逐步停止生产是理性之举。

Cybertruck厚重、棱角分明的设计自2019年发布以来一直备受争议。其锋利边缘的不锈钢车身因行人安全标准，使得在欧洲等关键市场无法获得监管批准。尽管电动皮卡在美国市场普遍面临困境，但Cybertruck独特的设计尤其限制了其全球影响力。

奥斯汀工厂目前是唯一能够生产Cybertruck专用零部件的设施，其2027年中期之后的生产命运仍不明确。特斯拉的重心现在转向Cybercab，这是一款没有方向盘或踏板的车型，马斯克将其设想为全球机器人出租车网络的主要自动驾驶汽车。Cybertruck的首席工程师指出，它为Cybercab提供了一个“令人难以置信的技术开发平台”。

---

## 4. 搜索所有人

**原文标题**: Search for everyone

**原文链接**: [https://kagi.com/changelog#11820](https://kagi.com/changelog#11820)

Kagi宣布了一项重大变革：**Kagi搜索**现在对所有人开放，无需账户即可进行前50次搜索（注册后可额外获得100次搜索）。此举旨在促进口碑传播。Kagi还强烈批评了谷歌禁用学校账户的AI工具和谷歌搜索的决定，将Kagi定位为优先考虑教育而非企业利润的替代方案。

主要产品更新包括：

*   **Kagi搜索（安卓应用）：** 重新设计了主屏幕，重建了语音搜索并增加了新选项，新增了快捷设置磁贴、主屏幕小部件、图片搜索和集成式快速回答按钮。
*   **Kagi助手：** 共享的对话串现在可以直接打开，语音输入更加流畅，临时对话串被清晰区分。用户现在可以直接将图片/文件粘贴到提示中。
*   **Kagi新闻：** 在Google Play上获得了推荐，现在它会避免在不同类别中重复报道同一事件的故事，并且设置界面也进行了重新设计。
*   **Kagi** 校对功能可实时显示更正，完成的翻译在页面重新加载后仍会保留，并提高了多种语言的准确性。现在可以查看AI使用额度，并且该扩展程序提供最佳质量的翻译。
*   **Small Web（应用）：** 新增了主题（设计与用户体验、工作与商业、体育），主题现在是持久可隐藏的，整体触觉反馈和无障碍功能也得到了改进。

所有产品都实施了许多其他改进和错误修复，以提升用户体验。

---

## 5. 微软画图远程代码执行漏洞

**原文标题**: MS Paint Remote Code Execution Vulnerability

**原文链接**: [https://www.cve.org/CVERecord?id=CVE-2026-83844](https://www.cve.org/CVERecord?id=CVE-2026-83844)

这段题为“MS Paint 远程代码执行漏洞”的文本，旨在讨论 Microsoft Paint 中一个潜在的安全漏洞。然而，所提供的内容并未描述该漏洞。相反，它展示了一个来自通用漏洞披露（CVE）网站的通用错误消息。这条消息告知用户，CVE 网站需要 JavaScript 才能正常运行，并请求用户激活它。因此，这篇文章没有提供关于 MS Paint 漏洞本身的任何细节，包括其性质或影响。

---

## 6. Blender 的 UI 和运行时：远超 GPUI

**原文标题**: Blender's UI and Runtime: Much Faster Than GPUI

**原文链接**: [https://github.com/ppmpreetham/BUI](https://github.com/ppmpreetham/BUI)

BUI (Blender's UI) is a standalone, high-performance UI library that extracts Blender's iconic user interface, interactions, and aesthetic into a compact C core. Its primary goal is to empower developers in various languages to create applications with Blender's renowned speed, efficiency, and unique user experience, such as continuous value dragging, fuzzy search, and math input fields in number fields.

BUI is not Blender itself, nor a browser engine; it's a direct port of Blender's UI code. It offers extensive language bindings, supporting Python (including existing tkinter and Qt-style apps, and native Blender components), Rust (with HTML+CSS, Tailwind, and React/Leptos-style hooks), JavaScript/React/Svelte (DOM-like API, JSX/Svelte components), Dear ImGui (with Blender's theme or actual widgets), and C.

Key features include damage rendering for zero CPU usage when idle, optional GPU rendering, native text rendering (Inter font), and comprehensive image and video decoding (PNG, JPEG, WebP, animated GIF, 1080p video) with intelligent caching and off-thread processing. Developers can build small, standalone executables (6-7 MB) with embedded JavaScript engines for quick startup. BUI runs natively on Windows, Linux, and macOS, with HiDPI support and a headless mode for testing. It aims to deliver Blender's intuitive and frugal interface to any application.

---

## 7. 沙龙告别

**原文标题**: Goodbye from Salon

**原文链接**: [https://www.salon.com/2026/11/05/goodbye-from-salon/](https://www.salon.com/2026/11/05/goodbye-from-salon/)

生成摘要时出错

---

## 8. Alpine Linux Security Advisory: OpenSSH-server password authentication bypass

**原文标题**: Alpine Linux Security Advisory: OpenSSH-server password authentication bypass

**原文链接**: [https://alpinelinux.org/posts/2026-11-05-openssh-password-authentication-bypass/](https://alpinelinux.org/posts/2026-11-05-openssh-password-authentication-bypass/)

生成摘要时出错

---

## 9. 荷兰“理想主义”银行ASN禁用非谷歌安卓系统，包括GrapheneOS

**原文标题**: Dutch 'idealist' bank ASN blocks non-Google Android, including GrapheneOS

**原文链接**: [https://github.com/PrivSec-dev/banking-apps-compat-report/issues/105](https://github.com/PrivSec-dev/banking-apps-compat-report/issues/105)

生成摘要时出错

---

## 10. Motorola Signature 27 with GrapheneOS support

**原文标题**: Motorola Signature 27 with GrapheneOS support

**原文链接**: [https://motorolanews.com/motorola-signature-27-2/](https://motorolanews.com/motorola-signature-27-2/)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-11-07](output/hacker_news_summary_2026-11-07.md) |
| 2 | [2026-11-06](output/hacker_news_summary_2026-11-06.md) |
| 3 | [2026-11-05](output/hacker_news_summary_2026-11-05.md) |
| 4 | [2026-11-03](output/hacker_news_summary_2026-11-03.md) |
| 5 | [2026-10-31](output/hacker_news_summary_2026-10-31.md) |
| 6 | [2026-11-01](output/hacker_news_summary_2026-11-01.md) |
| 7 | [2026-11-04](output/hacker_news_summary_2026-11-04.md) |
| 8 | [2026-10-29](output/hacker_news_summary_2026-10-29.md) |
| 9 | [2026-10-25](output/hacker_news_summary_2026-10-25.md) |
| 10 | [2026-10-30](output/hacker_news_summary_2026-10-30.md) |
| 11 | [2026-10-27](output/hacker_news_summary_2026-10-27.md) |
| 12 | [2026-10-24](output/hacker_news_summary_2026-10-24.md) |
| 13 | [2026-10-28](output/hacker_news_summary_2026-10-28.md) |
| 14 | [2026-10-26](output/hacker_news_summary_2026-10-26.md) |
| 15 | [2026-10-21](output/hacker_news_summary_2026-10-21.md) |
| 16 | [2026-10-22](output/hacker_news_summary_2026-10-22.md) |
| 17 | [2026-10-19](output/hacker_news_summary_2026-10-19.md) |
| 18 | [2026-10-23](output/hacker_news_summary_2026-10-23.md) |
| 19 | [2026-10-20](output/hacker_news_summary_2026-10-20.md) |
| 20 | [2026-10-17](output/hacker_news_summary_2026-10-17.md) |
| 21 | [2026-10-14](output/hacker_news_summary_2026-10-14.md) |
| 22 | [2026-10-18](output/hacker_news_summary_2026-10-18.md) |
| 23 | [2026-10-16](output/hacker_news_summary_2026-10-16.md) |
| 24 | [2026-10-15](output/hacker_news_summary_2026-10-15.md) |
| 25 | [2026-10-13](output/hacker_news_summary_2026-10-13.md) |
| 26 | [2026-10-11](output/hacker_news_summary_2026-10-11.md) |
| 27 | [2026-10-10](output/hacker_news_summary_2026-10-10.md) |
| 28 | [2026-10-07](output/hacker_news_summary_2026-10-07.md) |
| 29 | [2026-10-09](output/hacker_news_summary_2026-10-09.md) |
| 30 | [2026-09-30](output/hacker_news_summary_2026-09-30.md) |
| 31 | [2026-10-01](output/hacker_news_summary_2026-10-01.md) |
| 32 | [2026-09-29](output/hacker_news_summary_2026-09-29.md) |
| 33 | [2026-10-03](output/hacker_news_summary_2026-10-03.md) |
| 34 | [2026-10-06](output/hacker_news_summary_2026-10-06.md) |
| 35 | [2026-10-04](output/hacker_news_summary_2026-10-04.md) |
| 36 | [2026-10-02](output/hacker_news_summary_2026-10-02.md) |
| 37 | [2026-09-27](output/hacker_news_summary_2026-09-27.md) |
| 38 | [2026-09-24](output/hacker_news_summary_2026-09-24.md) |
| 39 | [2026-09-22](output/hacker_news_summary_2026-09-22.md) |
| 40 | [2026-09-23](output/hacker_news_summary_2026-09-23.md) |
| 41 | [2026-09-25](output/hacker_news_summary_2026-09-25.md) |
| 42 | [2026-09-19](output/hacker_news_summary_2026-09-19.md) |
| 43 | [2026-09-17](output/hacker_news_summary_2026-09-17.md) |
| 44 | [2026-09-18](output/hacker_news_summary_2026-09-18.md) |
| 45 | [2026-09-21](output/hacker_news_summary_2026-09-21.md) |
| 46 | [2026-09-20](output/hacker_news_summary_2026-09-20.md) |
| 47 | [2026-09-16](output/hacker_news_summary_2026-09-16.md) |
| 48 | [2026-09-11](output/hacker_news_summary_2026-09-11.md) |
| 49 | [2026-09-10](output/hacker_news_summary_2026-09-10.md) |
| 50 | [2026-09-13](output/hacker_news_summary_2026-09-13.md) |
| 51 | [2026-09-15](output/hacker_news_summary_2026-09-15.md) |
| 52 | [2026-09-12](output/hacker_news_summary_2026-09-12.md) |
| 53 | [2026-09-14](output/hacker_news_summary_2026-09-14.md) |
| 54 | [2026-09-04](output/hacker_news_summary_2026-09-04.md) |
| 55 | [2026-09-07](output/hacker_news_summary_2026-09-07.md) |
| 56 | [2026-09-09](output/hacker_news_summary_2026-09-09.md) |
| 57 | [2026-09-08](output/hacker_news_summary_2026-09-08.md) |
| 58 | [2026-09-06](output/hacker_news_summary_2026-09-06.md) |
| 59 | [2026-09-05](output/hacker_news_summary_2026-09-05.md) |
| 60 | [2026-09-03](output/hacker_news_summary_2026-09-03.md) |
| 61 | [2026-08-28](output/hacker_news_summary_2026-08-28.md) |
| 62 | [2026-09-01](output/hacker_news_summary_2026-09-01.md) |
| 63 | [2026-08-29](output/hacker_news_summary_2026-08-29.md) |
| 64 | [2026-09-02](output/hacker_news_summary_2026-09-02.md) |
| 65 | [2026-08-30](output/hacker_news_summary_2026-08-30.md) |
| 66 | [2026-08-31](output/hacker_news_summary_2026-08-31.md) |
| 67 | [2026-08-23](output/hacker_news_summary_2026-08-23.md) |
| 68 | [2026-08-24](output/hacker_news_summary_2026-08-24.md) |
| 69 | [2026-08-26](output/hacker_news_summary_2026-08-26.md) |
| 70 | [2026-08-20](output/hacker_news_summary_2026-08-20.md) |
| 71 | [2026-08-19](output/hacker_news_summary_2026-08-19.md) |
| 72 | [2026-08-25](output/hacker_news_summary_2026-08-25.md) |
| 73 | [2026-08-21](output/hacker_news_summary_2026-08-21.md) |
| 74 | [2026-08-22](output/hacker_news_summary_2026-08-22.md) |
| 75 | [2026-08-16](output/hacker_news_summary_2026-08-16.md) |
| 76 | [2026-08-13](output/hacker_news_summary_2026-08-13.md) |
| 77 | [2026-08-18](output/hacker_news_summary_2026-08-18.md) |
| 78 | [2026-08-15](output/hacker_news_summary_2026-08-15.md) |
| 79 | [2026-08-14](output/hacker_news_summary_2026-08-14.md) |
| 80 | [2026-08-17](output/hacker_news_summary_2026-08-17.md) |
| 81 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 82 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 83 | [2026-08-09](output/hacker_news_summary_2026-08-09.md) |
| 84 | [2026-08-12](output/hacker_news_summary_2026-08-12.md) |
| 85 | [2026-08-10](output/hacker_news_summary_2026-08-10.md) |
| 86 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 87 | [2026-08-11](output/hacker_news_summary_2026-08-11.md) |
| 88 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 89 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 90 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 91 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 92 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 93 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 94 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 95 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 96 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 97 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 98 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 99 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 100 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 101 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 102 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 103 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 104 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 105 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 106 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 107 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 108 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 109 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 110 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 111 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 112 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 113 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 114 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 115 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 116 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 117 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 118 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 119 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 120 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 121 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 122 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 123 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 124 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 125 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 126 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 127 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 128 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 129 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 130 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 131 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 132 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 133 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 134 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 135 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 136 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 137 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 138 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 139 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 140 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 141 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 142 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 143 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 144 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 145 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 146 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 147 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 148 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 149 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 150 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 151 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 152 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 153 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 154 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 155 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 156 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 157 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 158 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 159 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 160 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 161 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 162 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 163 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 164 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 165 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 166 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 167 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 168 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 169 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 170 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 171 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 172 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 173 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 174 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 175 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 176 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 177 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 178 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 179 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 180 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 181 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 182 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 183 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 184 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 185 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 186 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 187 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 188 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 189 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 190 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 191 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 192 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 193 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 194 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 195 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 196 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 197 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 198 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 199 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 200 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 201 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 202 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 203 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 204 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 205 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 206 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 207 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 208 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 209 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 210 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 211 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 212 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 213 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 214 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 215 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 216 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 217 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 218 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 219 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 220 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 221 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 222 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 223 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 224 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 225 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 226 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 227 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 228 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 229 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 230 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 231 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 232 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 233 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 234 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 235 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 236 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 237 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 238 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 239 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 240 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 241 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 242 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 243 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 244 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 245 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 246 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 247 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 248 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 249 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 250 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 251 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 252 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 253 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 254 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 255 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 256 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 257 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 258 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 259 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 260 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 261 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 262 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 263 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 264 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 265 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 266 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 267 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 268 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 269 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 270 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 271 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 272 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 273 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 274 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 275 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 276 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 277 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 278 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 279 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 280 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 281 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 282 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 283 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 284 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 285 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 286 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 287 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 288 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 289 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 290 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 291 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 292 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 293 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 294 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 295 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 296 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 297 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 298 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 299 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 300 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 301 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 302 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 303 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 304 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 305 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 306 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 307 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 308 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 309 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 310 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 311 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 312 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 313 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 314 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 315 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 316 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 317 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 318 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 319 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 320 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 321 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 322 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 323 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 324 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 325 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 326 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 327 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 328 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 329 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 330 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 331 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 332 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 333 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 334 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 335 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 336 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 337 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 338 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 339 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 340 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 341 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 342 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 343 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 344 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 345 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 346 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 347 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 348 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 349 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 350 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 351 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 352 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 353 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 354 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 355 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 356 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 357 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
