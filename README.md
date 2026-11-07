# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-11-07.md)

*最后自动更新时间: 2026-11-07 23:01:53*
## 1. 克劳德代码将您的电子邮件地址发送到网站。

**原文标题**: Claude Code sends your email address to websites

**原文链接**: [https://github.com/anthropics/claude-code/issues/107757](https://github.com/anthropics/claude-code/issues/107757)

2026年11月5日发布的一份严重隐私漏洞报告声称，Anthropic公司开发的AI编码工具Claude Code在进行网络搜索时，未经许可地在HTTP请求的User-Agent标头中泄露了用户的电子邮件地址。最初的报告者“taylor-edwards”表示，这导致了大量的诈骗邮件，并对Anthropic的隐私实践彻底失去信心，敦促Anthropic直接移除此功能，而非提供选择退出/选择加入的设置。

此问题引发了社区的强烈不满，许多用户质疑Anthropic公司推出这种“功能”的判断力。一位名为“poteat”的贡献者回应称，v2.1.317及更高版本中已引入一个名为`cc-plugin-privacy`的内置模组来阻止此行为，并且默认启用。然而，用户批评这一解决方案，认为基本的隐私应该是一个核心组成部分，而不应依赖于一个可选插件。

人们对潜在的GDPR违规和集体诉讼的可能性表示担忧。尽管此问题成为GitHub上获得最多回应的问题之一，但许多用户指出Anthropic公司缺乏官方道歉或全面声明。随后的开发者提交中提到了“拒绝携带账户所有者电子邮件地址的网络调用”，这表明正在实施更直接的代码层面修复。

---

## 2. 特斯拉将停止Cybertruck生产

**原文标题**: Tesla to wind down Cybertruck production

**原文链接**: [https://www.nbcnews.com/tech/tech-news/tesla-wind-cybertruck-production-years-poor-sales-markets-rcna607817](https://www.nbcnews.com/tech/tech-news/tesla-wind-cybertruck-production-years-poor-sales-markets-rcna607817)

Tesla will wind down Cybertruck production at its Texas gigafactory by mid-2027, CEO Elon Musk announced. The decision is driven by years of persistently weak sales for the futuristic pickup and its heavy, angular design, which hindered its regulatory approval in key markets like Europe due to pedestrian safety concerns. The cessation of production will allow Tesla to boost output of its new Cybercab model, which is central to Musk's robotaxi ambitions.

Despite Musk calling the Cybertruck the "best vehicle Tesla has ever made" and its wind-down the "end of an era," sales significantly underperformed. After deliveries began in late 2023, only 20,237 Cybertrucks were sold in the US last year, falling far short of Musk's initial prediction of 250,000 annual units. Experts, including former Aston Martin CEO Andy Palmer, noted it was economically illogical to continue a product not meeting targets.

The Cybertruck was controversial from its 2019 unveiling, with its design drawing criticism and an embarrassing window demonstration incident. While electric pickups generally face market struggles, the Cybertruck's unique design further limited its global viability. Its lead engineer stated the Cybertruck served as an "incredible technology development platform" for the Cybercab. The Cybercab, a steering wheel-less autonomous vehicle, has begun paid rides in Austin but still faces federal safety compliance questions.

---

## 3. Libghostty 1.0

**原文标题**: Libghostty 1.0

**原文链接**: [https://mitchellh.com/writing/libghostty-1-0](https://mitchellh.com/writing/libghostty-1-0)

生成摘要时出错

---

## 4. 极品飞车：地下狂飙2 浏览器在线

**原文标题**: Need for Speed Underground 2 online in the browser

**原文链接**: [https://nfsu2.xyz/](https://nfsu2.xyz/)

无法访问文章链接。

---

## 5. Blender的用户界面和运行时：比GPUI快得多

**原文标题**: Blender's UI and Runtime: Much Faster Than GPUI

**原文链接**: [https://github.com/ppmpreetham/BUI](https://github.com/ppmpreetham/BUI)

BUI (Blender UI) 是一个独立的高性能UI库，源自Blender的用户界面、交互和美学，构建于一个轻量级的C语言核心之上。其宗旨是将Blender闻名遐迩的快速、经济高效且直观的UI体验带给任何应用程序，支持任何语言。

BUI为多种语言和框架提供绑定：Python（支持tkinter、Qt语法和原生Blender组件）、Rust（支持HTML/CSS、Tailwind和React/Leptos风格的钩子）、JavaScript/React/Svelte（提供类似DOM的API和组件支持）、C/C++以及Dear ImGui。它旨在帮助开发者将老旧的Tkinter应用现代化、为熟悉Blender的艺术家构建工具、无需嵌入浏览器即可创建原生桌面UI，或将Blender的主题和控件集成到Dear ImGui项目中。

主要功能包括Blender独特的控件（例如，连续数字拖动、模糊搜索、数学表达式求值）、深色和浅色主题、脏区渲染实现0% CPU空闲占用、可选的GPU渲染器（Direct3D 11/OpenGL 3.3）以及先进的媒体处理。后者包括对各种图像格式（PNG、GIF、WebP、JPEG、SVG，支持动画）的高效、脱线程解码和GPU加速的视频播放。

BUI声称其性能卓越，每帧CPU占用比GPUI-fast少2-4倍，同时内存占用更低，启动速度快（首帧约5毫秒）。它在Windows、Linux和macOS上提供原生窗口并支持HiDPI。小型独立JavaScript应用程序可以使用嵌入式QuickJS引擎构建，启动迅速且内存占用极小。

安装过程简单，可通过标准包管理器完成：`pip install blenderui`、`cargo add blenderui` 或 `npm install @blender-ui/react`。

---

## 6. Dutch 'idealist' bank ASN blocks non-Google Android, including GrapheneOS

**原文标题**: Dutch 'idealist' bank ASN blocks non-Google Android, including GrapheneOS

**原文链接**: [https://github.com/PrivSec-dev/banking-apps-compat-report/issues/105](https://github.com/PrivSec-dev/banking-apps-compat-report/issues/105)

生成摘要时出错

---

## 7. 英国将强制招聘广告公开薪资

**原文标题**: Britain to make salary disclosure in job ads mandatory

**原文链接**: [https://www.reuters.com/business/world-at-work/britain-make-salary-disclosure-job-ads-mandatory-2026-11-05/](https://www.reuters.com/business/world-at-work/britain-make-salary-disclosure-job-ads-mandatory-2026-11-05/)

英国政府计划在2026年11月5日前，强制要求所有招聘广告中必须列出薪资范围。这项举措旨在解决性别和族裔薪酬差距，提高薪酬透明度，并帮助求职者做出更明智的职业选择。

根据新规定，雇主将依法被要求在招聘信息中包含预期薪资或薪资范围。政府认为，这种透明度将使员工能够争取更公平的薪酬，减少求职者和雇主双方的时间浪费，并避免个人在招聘过程后期才发现薪酬不合适的情况。

尽管一些大型公司已提供薪资信息，但此举将这一要求推广至所有企业，无论其规模大小。该提案目前正在进行为期10周的咨询期。这项政策是基于政府此前为解决薪酬不平等所做的努力，例如禁止在面试中询问过往薪资。

商业团体和倡导平等的活动家普遍欢迎这项提案，认为这是朝着在英国建立更公平、更透明的劳动力市场迈出的重要一步。

---

## 8. 一个能够向Opus寻求帮助的Jev，能让Opus以四分之一的成本获得准确性。

**原文标题**: A Jev that can ask Opus for help gives Opus accuracy at 4x lower cost

**原文链接**: [https://hightouch.com/blog/llm-judges-identity-resolution](https://hightouch.com/blog/llm-judges-identity-resolution)

本文探讨了使用大型语言模型（LLMs）和决策模型（Jev, Luna）来评估身份解析（IDR）结果，具体而言，是检测“过度合并”——即一个身份错误地对应了多个真实人物的情况。这项任务对数据分析至关重要，但传统上对人工来说既缓慢又困难。

作者在IDR评分任务中，对比测试了Jev和GPT-6 Luna（更便宜、更快的决策模型）与Claude Opus（昂贵的前沿模型）。最初，决策模型表现尚可（准确率88.8%–97.3%），但落后于Opus（准确率99.0%），尽管成本只是Opus的一小部分（便宜高达90倍，快10倍）。Luna在开箱即用状态下最初优于Jev。

一个关键发现是：Jev的置信度得分比Luna校准得更好。Jev的错误通常伴随着低置信度，而Luna则常常过度自信，尤其是在更困难的案例上。这一洞察促成了一个“混合评估模型”的诞生。

这种混合方法会将廉价模型（Jev或Luna）给出低到中等置信度的案例发送给昂贵的前沿模型（Opus）进行二次判断。这一策略充分利用了Jev卓越的校准能力，取得了显著效果：
*   **混合Jev模型**在成本显著降低的情况下（例如，在较简单的测试中，每1000个身份0.88美元对3.86美元，便宜超过4倍），实现了接近Opus的准确率（例如，在较简单的测试中为98.8%对99.0%）。
*   在更困难的数据集上，混合Jev模型保持了优于混合Luna模型（91.6%）的准确率（95.3%），并根据不确定性动态调整开销。

结论是，模型置信度校准对于有效的混合大型语言模型系统至关重要。像Jev这样经过良好校准的廉价模型，与Opus这样的前沿模型结合使用时，可以大幅降低成本，同时实现高准确率，并能智能地适应问题难度。

---

## 9. 每台 Mac 都附带一个（未记录的）家庭成员分类器

**原文标题**: Every Mac comes with an (undocumented) family member classifier

**原文链接**: [https://8rank.ai/game/apple-intelligence-personal-knowledge-graph](https://8rank.ai/game/apple-intelligence-personal-knowledge-graph)

Since macOS 13 (2022), every Mac ships with two undocumented daemons, `knowledgeconstructiond` and `intelligenceplatformd`, which construct a "Personal Knowledge Graph" (PKG). This system aims to build a comprehensive profile of the user, detailing "who you are, who you know, how those people are related to you, how you communicate with them, where you go, what you do and when."

The PKG cross-references a vast array of on-device data: Contacts, Calendar, Photos (faces), Messages, Mail, location, Screen Time, Family Sharing, Medical ID, Siri Suggestions, app usage, communication logs (metadata, not content), movement, and device signals (e.g., Wi-Fi, Bluetooth, charging, ambient light, and physical proximity records).

All this information is stored in plaintext SQLite databases, primarily `graph.db`, located in `~/Library/IntelligencePlatform`. It operates as a triple store, comprising 181 entity classes and 278 predicates, allowing the system to infer complex relationships, including previously undocumented "kinship" (family ties). This graph is reportedly designed as a queryable store for LLMs.

Apple provides minimal public documentation on this mechanism. The authors of this post offer a deeper analysis, particularly on kinship inference, and have open-sourced "iKnow," a dashboard for users to inspect their own graphs. They warn that this extensive, centralized personal data presents a significant privacy risk, acting as a "privacy single point of failure" if compromised, especially when combined with advanced LLMs.

---

## 10. Cuban: Facebook knowingly runs AI deepfake scam ads; docs say $16B fraud revenue

**原文标题**: Cuban: Facebook knowingly runs AI deepfake scam ads; docs say $16B fraud revenue

**原文链接**: [https://finance.yahoo.com/technology/ai/articles/mark-cuban-says-facebook-knowingly-213000020.html](https://finance.yahoo.com/technology/ai/articles/mark-cuban-says-facebook-knowingly-213000020.html)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-11-07](output/hacker_news_summary_2026-11-07.md) |
| 2 | [2026-11-05](output/hacker_news_summary_2026-11-05.md) |
| 3 | [2026-11-03](output/hacker_news_summary_2026-11-03.md) |
| 4 | [2026-11-04](output/hacker_news_summary_2026-11-04.md) |
| 5 | [2026-11-06](output/hacker_news_summary_2026-11-06.md) |
| 6 | [2026-10-29](output/hacker_news_summary_2026-10-29.md) |
| 7 | [2026-10-25](output/hacker_news_summary_2026-10-25.md) |
| 8 | [2026-10-30](output/hacker_news_summary_2026-10-30.md) |
| 9 | [2026-10-27](output/hacker_news_summary_2026-10-27.md) |
| 10 | [2026-10-28](output/hacker_news_summary_2026-10-28.md) |
| 11 | [2026-10-31](output/hacker_news_summary_2026-10-31.md) |
| 12 | [2026-10-26](output/hacker_news_summary_2026-10-26.md) |
| 13 | [2026-11-01](output/hacker_news_summary_2026-11-01.md) |
| 14 | [2026-10-21](output/hacker_news_summary_2026-10-21.md) |
| 15 | [2026-10-22](output/hacker_news_summary_2026-10-22.md) |
| 16 | [2026-10-18](output/hacker_news_summary_2026-10-18.md) |
| 17 | [2026-10-19](output/hacker_news_summary_2026-10-19.md) |
| 18 | [2026-10-24](output/hacker_news_summary_2026-10-24.md) |
| 19 | [2026-10-23](output/hacker_news_summary_2026-10-23.md) |
| 20 | [2026-10-20](output/hacker_news_summary_2026-10-20.md) |
| 21 | [2026-10-17](output/hacker_news_summary_2026-10-17.md) |
| 22 | [2026-10-14](output/hacker_news_summary_2026-10-14.md) |
| 23 | [2026-10-16](output/hacker_news_summary_2026-10-16.md) |
| 24 | [2026-10-13](output/hacker_news_summary_2026-10-13.md) |
| 25 | [2026-10-11](output/hacker_news_summary_2026-10-11.md) |
| 26 | [2026-10-15](output/hacker_news_summary_2026-10-15.md) |
| 27 | [2026-10-10](output/hacker_news_summary_2026-10-10.md) |
| 28 | [2026-10-01](output/hacker_news_summary_2026-10-01.md) |
| 29 | [2026-10-03](output/hacker_news_summary_2026-10-03.md) |
| 30 | [2026-10-06](output/hacker_news_summary_2026-10-06.md) |
| 31 | [2026-10-04](output/hacker_news_summary_2026-10-04.md) |
| 32 | [2026-10-07](output/hacker_news_summary_2026-10-07.md) |
| 33 | [2026-10-09](output/hacker_news_summary_2026-10-09.md) |
| 34 | [2026-10-02](output/hacker_news_summary_2026-10-02.md) |
| 35 | [2026-09-27](output/hacker_news_summary_2026-09-27.md) |
| 36 | [2026-09-24](output/hacker_news_summary_2026-09-24.md) |
| 37 | [2026-09-30](output/hacker_news_summary_2026-09-30.md) |
| 38 | [2026-09-29](output/hacker_news_summary_2026-09-29.md) |
| 39 | [2026-09-22](output/hacker_news_summary_2026-09-22.md) |
| 40 | [2026-09-23](output/hacker_news_summary_2026-09-23.md) |
| 41 | [2026-09-25](output/hacker_news_summary_2026-09-25.md) |
| 42 | [2026-09-19](output/hacker_news_summary_2026-09-19.md) |
| 43 | [2026-09-17](output/hacker_news_summary_2026-09-17.md) |
| 44 | [2026-09-18](output/hacker_news_summary_2026-09-18.md) |
| 45 | [2026-09-15](output/hacker_news_summary_2026-09-15.md) |
| 46 | [2026-09-21](output/hacker_news_summary_2026-09-21.md) |
| 47 | [2026-09-20](output/hacker_news_summary_2026-09-20.md) |
| 48 | [2026-09-16](output/hacker_news_summary_2026-09-16.md) |
| 49 | [2026-09-11](output/hacker_news_summary_2026-09-11.md) |
| 50 | [2026-09-10](output/hacker_news_summary_2026-09-10.md) |
| 51 | [2026-09-13](output/hacker_news_summary_2026-09-13.md) |
| 52 | [2026-09-12](output/hacker_news_summary_2026-09-12.md) |
| 53 | [2026-09-09](output/hacker_news_summary_2026-09-09.md) |
| 54 | [2026-09-08](output/hacker_news_summary_2026-09-08.md) |
| 55 | [2026-09-14](output/hacker_news_summary_2026-09-14.md) |
| 56 | [2026-09-04](output/hacker_news_summary_2026-09-04.md) |
| 57 | [2026-09-07](output/hacker_news_summary_2026-09-07.md) |
| 58 | [2026-09-01](output/hacker_news_summary_2026-09-01.md) |
| 59 | [2026-08-29](output/hacker_news_summary_2026-08-29.md) |
| 60 | [2026-09-06](output/hacker_news_summary_2026-09-06.md) |
| 61 | [2026-09-02](output/hacker_news_summary_2026-09-02.md) |
| 62 | [2026-09-05](output/hacker_news_summary_2026-09-05.md) |
| 63 | [2026-08-30](output/hacker_news_summary_2026-08-30.md) |
| 64 | [2026-08-31](output/hacker_news_summary_2026-08-31.md) |
| 65 | [2026-09-03](output/hacker_news_summary_2026-09-03.md) |
| 66 | [2026-08-23](output/hacker_news_summary_2026-08-23.md) |
| 67 | [2026-08-28](output/hacker_news_summary_2026-08-28.md) |
| 68 | [2026-08-24](output/hacker_news_summary_2026-08-24.md) |
| 69 | [2026-08-26](output/hacker_news_summary_2026-08-26.md) |
| 70 | [2026-08-20](output/hacker_news_summary_2026-08-20.md) |
| 71 | [2026-08-19](output/hacker_news_summary_2026-08-19.md) |
| 72 | [2026-08-25](output/hacker_news_summary_2026-08-25.md) |
| 73 | [2026-08-21](output/hacker_news_summary_2026-08-21.md) |
| 74 | [2026-08-22](output/hacker_news_summary_2026-08-22.md) |
| 75 | [2026-08-16](output/hacker_news_summary_2026-08-16.md) |
| 76 | [2026-08-13](output/hacker_news_summary_2026-08-13.md) |
| 77 | [2026-08-09](output/hacker_news_summary_2026-08-09.md) |
| 78 | [2026-08-18](output/hacker_news_summary_2026-08-18.md) |
| 79 | [2026-08-12](output/hacker_news_summary_2026-08-12.md) |
| 80 | [2026-08-10](output/hacker_news_summary_2026-08-10.md) |
| 81 | [2026-08-15](output/hacker_news_summary_2026-08-15.md) |
| 82 | [2026-08-14](output/hacker_news_summary_2026-08-14.md) |
| 83 | [2026-08-17](output/hacker_news_summary_2026-08-17.md) |
| 84 | [2026-08-11](output/hacker_news_summary_2026-08-11.md) |
| 85 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 86 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 87 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 88 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 89 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 90 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 91 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 92 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 93 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 94 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 95 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 96 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 97 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 98 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 99 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 100 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 101 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 102 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 103 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 104 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 105 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 106 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 107 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 108 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 109 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 110 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 111 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 112 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 113 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 114 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 115 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 116 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 117 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 118 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 119 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 120 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 121 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 122 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 123 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 124 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 125 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 126 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 127 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 128 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 129 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 130 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 131 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 132 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 133 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 134 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 135 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 136 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 137 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 138 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 139 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 140 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 141 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 142 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 143 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 144 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 145 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 146 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 147 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 148 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 149 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 150 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 151 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 152 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 153 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 154 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 155 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 156 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 157 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 158 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 159 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 160 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 161 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 162 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 163 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 164 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 165 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 166 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 167 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 168 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 169 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 170 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 171 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 172 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 173 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 174 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 175 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 176 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 177 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 178 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 179 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 180 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 181 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 182 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 183 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 184 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 185 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 186 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 187 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 188 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 189 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 190 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 191 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 192 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 193 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 194 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 195 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 196 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 197 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 198 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 199 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 200 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 201 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 202 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 203 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 204 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 205 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 206 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 207 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 208 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 209 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 210 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 211 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 212 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 213 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 214 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 215 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 216 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 217 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 218 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 219 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 220 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 221 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 222 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 223 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 224 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 225 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 226 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 227 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 228 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 229 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 230 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 231 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 232 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 233 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 234 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 235 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 236 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 237 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 238 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 239 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 240 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 241 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 242 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 243 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 244 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 245 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 246 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 247 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 248 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 249 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 250 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 251 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 252 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 253 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 254 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 255 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 256 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 257 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 258 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 259 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 260 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 261 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 262 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 263 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 264 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 265 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 266 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 267 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 268 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 269 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 270 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 271 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 272 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 273 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 274 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 275 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 276 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 277 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 278 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 279 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 280 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 281 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 282 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 283 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 284 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 285 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 286 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 287 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 288 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 289 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 290 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 291 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 292 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 293 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 294 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 295 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 296 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 297 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 298 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 299 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 300 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 301 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 302 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 303 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 304 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 305 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 306 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 307 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 308 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 309 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 310 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 311 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 312 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 313 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 314 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 315 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 316 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 317 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 318 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 319 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 320 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 321 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 322 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 323 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 324 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 325 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 326 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 327 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 328 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 329 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 330 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 331 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 332 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 333 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 334 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 335 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 336 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 337 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 338 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 339 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 340 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 341 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 342 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 343 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 344 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 345 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 346 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 347 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 348 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 349 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 350 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 351 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 352 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
| 353 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 354 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 355 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 356 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 357 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
