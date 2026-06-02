# Hacker News 热门文章摘要 (2026-06-02)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 最新的 Instagram “花招” 是我见过最荒唐的。

**原文标题**: The newest Instagram “exploit” is the goofiest I've seen

**原文链接**: [https://www.0xsid.com/blog/meta-account-takeover-fiasco](https://www.0xsid.com/blog/meta-account-takeover-fiasco)

该文章详细披露了一项“最离谱”的Instagram漏洞攻击，该漏洞导致了大规模账户劫持，甚至影响了包括奥巴马白宫在内的高知名度账户。这次持续了数周甚至数月的攻击中，攻击者通过VPN伪造其地理位置，然后联系Meta的AI支持系统，声称账户被盗，并要求将验证码发送到他们控制的任意电子邮件地址。

令人震惊的是，据报道，该AI竟然执行了“零验证密码重置”，没有验证新邮箱是否与该账户有任何关联。甚至通过视频自拍进行的身份验证也轻易被绕过，据称，使用AI动画处理的公开照片就能奏效。这种方法彻底绕过了现有的双重身份验证（2FA），撤销了原所有者的会话，更改了密码，并将恢复信息替换为攻击者的，让受害者得不到任何人工支持。

这一漏洞助长了黑市，为有价值的用户名提供账户劫持服务。作者作为一名经验丰富的安全专业人士，对一家市值1.5万亿美元的公司竟有如此薄弱的安全防护表示难以置信。Meta此后已修复了该漏洞，但其长期存在凸显了一个严重的安全缺陷。

---

## 2. Malicious npm packages detected across Red Hat Cloud Services

**原文标题**: Malicious npm packages detected across Red Hat Cloud Services

**原文链接**: [https://github.com/RedHatInsights/javascript-clients/issues/492](https://github.com/RedHatInsights/javascript-clients/issues/492)

2026年6月1日发布了一项编号为#492的安全警报，详细说明检测到影响红帽云服务的恶意npm包。此次大规模入侵影响了`@redhat-cloud-services/`范围下的众多软件包。

该漏洞由StepSecurity发现，更多详情可在其博客和安全信息源中查阅。已提供受影响软件包及其受损版本的完整列表。

主要受影响软件包包括：
*   `@redhat-cloud-services/chrome` (版本 2.3.1, 2.3.2, 2.3.4)
*   `@redhat-cloud-services/compliance-client` (版本 4.0.3, 4.0.4, 4.0.6)
*   `@redhat-cloud-services/frontend-components` (版本 7.7.2, 7.7.3, 7.7.5)
*   `@redhat-cloud-services/host-inventory-client` (版本 5.0.3, 5.0.4, 5.0.6)
*   `@redhat-cloud-services/rbac-client` (版本 9.0.3, 9.0.4, 9.0.6)
*   `@redhat-cloud-services/vulnerabilities-client` (版本 2.1.9, 2.1.11)

许多其他客户端和前端组件包的多个版本也受到影响。建议这些红帽云服务npm软件包的用户检查其依赖项，并采取适当措施以解决这些恶意发布版本带来的安全风险。

---

## 3. 十年志强，就够用了

**原文标题**: A 10 year old Xeon is all you need

**原文链接**: [https://point.free/blog/gemma-4-on-a-2016-xeon/](https://point.free/blog/gemma-4-on-a-2016-xeon/)

文章详细介绍了一项非凡的尝试：在一台使用单个英特尔至强 E5-2620 v4 CPU 和 128GB DDR3 内存的十年老旧服务器上运行大型语言模型 Gemma 4 26B，这台服务器严重缺乏 GPU。主要障碍是“内存墙”，即 LLM 推理性能受限于缓慢的内存带宽，而非 CPU 处理能力，服务器老旧的 DDR3 内存更是加剧了这一问题。

为克服此问题，作者绕过了高级工具，转而利用 `ik_llama.cpp` 中的 `llama-cli`，并配合一系列高度特定、低级别的优化标志。关键策略包括：

1.  **推测解码：** 采用一个较小的“草稿”模型来预测 token，从而最大程度地减少大型“验证器”模型的内存密集型解码器通过次数，利用 CPU 相对廉价的计算能力。
2.  **CPU 和 MoE 优化：** 诸如 `--cpu-moe` 和 `--merge-up-gate-experts` 等标志，针对 CPU 缓存层次结构和融合操作定制了专家混合（MoE）路由，以减少内存传输，防止“缓存颠簸”。
3.  **内存管理：** `--mlock` 将模型锁定在 RAM 中，以防止操作系统将其交换到磁盘。`--run-time-repack` 重新组织了权重以实现最佳的 CPU 缓存对齐，而 `--no-kv-offload` 则禁用了不必要的 GPU KV 缓存搜索。
4.  **高级注意力机制：** `Flash Attention` 经定制移植到 CPU 后，通过在快速 CPU 缓存中对其进行处理，防止了完整的注意力矩阵在 RAM 中实例化。`--mla-use 3`（多头潜在注意力）进一步压缩了 KV 缓存，节省了宝贵的内存。

这表明，即使在严重性能不足的硬件上，通过细致地解决内存带宽瓶颈，深入的软件层面优化也能实现现代 LLM 推理。

---

## 4. 股市能否消化Anthropic、SpaceX 和 OpenAI？

**原文标题**: Can the stockmarket swallow Anthropic, SpaceX and OpenAI?

**原文链接**: [https://www.economist.com/finance-and-economics/2026/06/01/can-the-stockmarket-swallow-anthropic-spacex-and-openai](https://www.economist.com/finance-and-economics/2026/06/01/can-the-stockmarket-swallow-anthropic-spacex-and-openai)

无法访问文章链接

---

## 5. 突袭20年后，海盗湾依然坚挺

**原文标题**: The Pirate Bay Remains Resilient, 20 Years After the Raid

**原文链接**: [https://torrentfreak.com/the-pirate-bay-remains-resilient-20-years-after-the-raid/](https://torrentfreak.com/the-pirate-bay-remains-resilient-20-years-after-the-raid/)

首次大规模突袭二十年后，海盗湾（The Pirate Bay，简称TPB）依然顽强存在，这归功于一次关键备份和运营模式的转变。2006年5月31日，65名瑞典警察在美国政府的压力下，突袭了斯德哥尔摩的一个数据中心，旨在让TPB下线。

就在突袭前，联合创始人弗雷德里克·内伊（Fredrik Neij）察觉到异样，对网站的种子追踪器进行了关键的完整备份。这一快速反应使TPB在三天内复活，并通过暂时更名为“警察湾”（The Police Bay）并采用凤凰标志来嘲讽当局。这次突袭非但没有将其关闭，反而将TPB推向了主流媒体的视野，产生了巨大的流量激增，这与好莱坞的初衷背道而驰。

后来通过2017年《信息自由法》请求获得的信息，揭示了美国在其中扮演的重要角色。美国大使馆的电报证实，好莱坞的美国电影协会（MPA）强烈游说瑞典对TPB采取行动，最终导致了这次突袭。一名使馆工作人员甚至因其“巧妙的对外联络”而被提名获奖，正是这种联络促成了瑞典执法部门的“大胆决定”。

尽管这次突袭让创始人在许多人眼中成为了英雄，但它最终导致了几名关键人物被刑事定罪并判处监禁。这促使最初的团队切断了联系，将网站移交给了一个更为匿名的团队，据称该团队位于塞舌尔。这个新时代带来了“静默运营”，这在2014年网站从另一次突袭中恢复过来时，通过极少的沟通便可见一斑。

如今TPB依然在线，自豪地称自己为“银河系最具韧性的种子网站”，这个称号可以说是在2006年那个决定性的一天赢来的。

---

## 6. Adafruit 收到来自 Fenwick 法律顾问代表 Flux.ai 的律师函

**原文标题**: Adafruit receives demand letter from Fenwick legal counsel on behalf of Flux.ai

**原文链接**: [https://blog.adafruit.com/](https://blog.adafruit.com/)

2026年6月1日，Adafruit宣布其于2026年5月22日收到了Defy Gravity公司旗下Flux.AI（简称“Flux”）的法律顾问Fenwick & West律师事务所发出的一封律师函。该函件由合伙人Jonathan F. Lenzner发出，要求Adafruit停止发布一篇Flux声称包含虚假且可能构成诽谤性言论的文章。这些言论涉及Flux的知识产权、商业吸引力以及用户基础。

该律师函还根据《计算机欺诈和滥用法案》提出了指控。Adafruit驳斥了这些指控，声明其仅访问了因服务器配置错误而由Flux自身系统公开的信息。Adafruit坚称其报告关注的是公共安全利益问题，并且是作为负责任披露的一部分进行的。

尽管Adafruit强烈驳斥Flux的主张，但已暂时停止在其博客上发布内容，以考虑其回应和下一步措施。Adafruit承诺将适时向社区通报最新情况。

---

## 7. CS336：从零开始的语言建模

**原文标题**: CS336: Language Modeling from Scratch

**原文链接**: [https://cs336.stanford.edu/](https://cs336.stanford.edu/)

CS336: Language Modeling from Scratch, offered by Stanford in Spring 2026, is a 5-unit, highly implementation-heavy course led by Instructors Tatsunori Hashimoto and Percy Liang. The course aims to provide a deep, hands-on understanding of language models by guiding students through the entire development process, from data collection and cleaning for pre-training to transformer construction, training, and evaluation.

Key prerequisites include strong proficiency in Python and software engineering, experience with deep learning and systems optimization (PyTorch, GPUs), college-level calculus/linear algebra, basic probability/statistics, and machine learning fundamentals.

The curriculum involves five major assignments:
1.  Implementing core Transformer components.
2.  Optimizing systems with Triton (FlashAttention2) and distributed training.
3.  Understanding and applying scaling laws.
4.  Processing and cleaning pre-training data from sources like Common Crawl.
5.  Applying alignment and reasoning techniques using supervised finetuning and reinforcement learning.

Lectures are Monday/Wednesday, with recordings on YouTube. Students use public Slack channels for course questions and a dedicated email for personal matters. GPU compute options are provided for self-study, with Modal as a sponsor. The Honor Code permits study groups (with attribution) and AI tools for conceptual help, but prohibits direct problem-solving and encourages disabling AI autocomplete. Students have 6 late days, with a maximum of 3 per assignment. A detailed schedule outlines topics and deadlines.

---

## 8. Anthropic confidentially submits draft S-1 to the SEC

**原文标题**: Anthropic confidentially submits draft S-1 to the SEC

**原文链接**: [https://www.anthropic.com/news/confidential-draft-s1-sec](https://www.anthropic.com/news/confidential-draft-s1-sec)

生成摘要时出错

---

## 9. AI Agent Guidelines for CS336 at Stanford

**原文标题**: AI Agent Guidelines for CS336 at Stanford

**原文链接**: [https://github.com/stanford-cs336/assignment1-basics/blob/main/CLAUDE.md](https://github.com/stanford-cs336/assignment1-basics/blob/main/CLAUDE.md)

生成摘要时出错

---

## 10. Age verification for social media, the beginning of the end for a free internet?

**原文标题**: Age verification for social media, the beginning of the end for a free internet?

**原文链接**: [https://mullvad.net/en/blog/age-verification-for-social-media-the-beginning-of-the-end-for-a-free-internet](https://mullvad.net/en/blog/age-verification-for-social-media-the-beginning-of-the-end-for-a-free-internet)

生成摘要时出错

---

## 11. Nvidia RTX Spark

**原文标题**: Nvidia RTX Spark

**原文链接**: [https://www.nvidia.com/en-us/products/rtx-spark/](https://www.nvidia.com/en-us/products/rtx-spark/)

生成摘要时出错

---

## 12. Why Janet? (2023)

**原文标题**: Why Janet? (2023)

**原文链接**: [https://ianthehenry.com/posts/why-janet/](https://ianthehenry.com/posts/why-janet/)

生成摘要时出错

---

## 13. Chuwi Minibook X

**原文标题**: Chuwi Minibook X

**原文链接**: [https://tylercipriani.com/blog/2026/05/28/chuwi-minibook-x/](https://tylercipriani.com/blog/2026/05/28/chuwi-minibook-x/)

生成摘要时出错

---

## 14. Gmail thinks I'm stupid, so I left

**原文标题**: Gmail thinks I'm stupid, so I left

**原文链接**: [https://moddedbear.com/gmail-thinks-im-stupid-so-i-left](https://moddedbear.com/gmail-thinks-im-stupid-so-i-left)

生成摘要时出错

---

## 15. macOS needs its grid back

**原文标题**: macOS needs its grid back

**原文链接**: [https://blog.hopefullyuseful.com/blog/macos-needs-its-grid-back/](https://blog.hopefullyuseful.com/blog/macos-needs-its-grid-back/)

生成摘要时出错

---

## 16. Chipotlai Max

**原文标题**: Chipotlai Max

**原文链接**: [https://github.com/cyberpapiii/chipotlai-max](https://github.com/cyberpapiii/chipotlai-max)

生成摘要时出错

---

## 17. OpenAI frontier models and Codex are now available on AWS

**原文标题**: OpenAI frontier models and Codex are now available on AWS

**原文链接**: [https://openai.com/index/openai-frontier-models-and-codex-are-now-available-on-aws/](https://openai.com/index/openai-frontier-models-and-codex-are-now-available-on-aws/)

生成摘要时出错

---

## 18. A walking tour of surveillance infrastructure in Seattle (2020)

**原文标题**: A walking tour of surveillance infrastructure in Seattle (2020)

**原文链接**: [https://coveillance.org/a-walking-tour-of-surveillance-infrastructure-in-seattle/](https://coveillance.org/a-walking-tour-of-surveillance-infrastructure-in-seattle/)

生成摘要时出错

---

## 19. Should you normalize RGB values by 255 or 256?

**原文标题**: Should you normalize RGB values by 255 or 256?

**原文链接**: [https://30fps.net/pages/255-vs-256-division/](https://30fps.net/pages/255-vs-256-division/)

生成摘要时出错

---

## 20. Love systemd timers

**原文标题**: Love systemd timers

**原文链接**: [https://blog.tjll.net/you-dont-love-systemd-timers-enough/](https://blog.tjll.net/you-dont-love-systemd-timers-enough/)

生成摘要时出错

---

## 21. DuckDuckGo makes its 'no-AI' search engine easier to access as its traffic booms

**原文标题**: DuckDuckGo makes its 'no-AI' search engine easier to access as its traffic booms

**原文链接**: [https://techcrunch.com/2026/06/01/duckduckgo-makes-its-no-ai-search-engine-easier-to-access-as-its-traffic-booms/](https://techcrunch.com/2026/06/01/duckduckgo-makes-its-no-ai-search-engine-easier-to-access-as-its-traffic-booms/)

生成摘要时出错

---

## 22. MAI-Code-1-Flash

**原文标题**: MAI-Code-1-Flash

**原文链接**: [https://microsoft.ai/news/introducingmai-code-1-flash/](https://microsoft.ai/news/introducingmai-code-1-flash/)

生成摘要时出错

---

## 23. Microsoft builds MacBook Pro rival with NVIDIA-powered Surface Laptop Ultra

**原文标题**: Microsoft builds MacBook Pro rival with NVIDIA-powered Surface Laptop Ultra

**原文链接**: [https://www.windowslatest.com/2026/06/01/microsoft-builds-its-ultimate-macbook-pro-rival-with-the-nvidia-powered-surface-laptop-ultra/](https://www.windowslatest.com/2026/06/01/microsoft-builds-its-ultimate-macbook-pro-rival-with-the-nvidia-powered-surface-laptop-ultra/)

生成摘要时出错

---

## 24. Apple rejected my dictation app for using the accessibility API

**原文标题**: Apple rejected my dictation app for using the accessibility API

**原文链接**: [https://www.mitmllc.com/blog/apple-rejected-my-dictation-app/](https://www.mitmllc.com/blog/apple-rejected-my-dictation-app/)

生成摘要时出错

---

## 25. Larry Ellison: "Citizens will be on their best behavior because we’re recording"

**原文标题**: Larry Ellison: "Citizens will be on their best behavior because we’re recording"

**原文链接**: [https://www.techradar.com/pro/quote-of-the-day-by-oracle-co-founder-larry-ellison-citizens-will-be-on-their-best-behavior-because-were-constantly-recording-and-reporting-everything-that-is-going-on-a-dire-warning-on-the-erosion-of-privacy](https://www.techradar.com/pro/quote-of-the-day-by-oracle-co-founder-larry-ellison-citizens-will-be-on-their-best-behavior-because-were-constantly-recording-and-reporting-everything-that-is-going-on-a-dire-warning-on-the-erosion-of-privacy)

生成摘要时出错

---

## 26. Debug Project

**原文标题**: Debug Project

**原文链接**: [https://debug.com/](https://debug.com/)

生成摘要时出错

---

## 27. Florida sues OpenAI and Sam Altman over AI risks

**原文标题**: Florida sues OpenAI and Sam Altman over AI risks

**原文链接**: [https://www.politico.com/news/2026/06/01/openai-hit-with-florida-lawsuit-00944215](https://www.politico.com/news/2026/06/01/openai-hit-with-florida-lawsuit-00944215)

生成摘要时出错

---

## 28. What appear to be biochemical processes may be a natural feature of geology

**原文标题**: What appear to be biochemical processes may be a natural feature of geology

**原文链接**: [https://www.quantamagazine.org/the-dirt-that-refused-to-die-20260601/](https://www.quantamagazine.org/the-dirt-that-refused-to-die-20260601/)

生成摘要时出错

---

## 29. Alphabet announces $80B equity capital raise to expand AI infra and compute

**原文标题**: Alphabet announces $80B equity capital raise to expand AI infra and compute

**原文链接**: [https://abc.xyz/investor/news/news-details/2026/Alphabet-Announces-Proposed-80-Billion-Equity-Capital-Raise-to-Expand-AI-Infrastructure-and-Compute-2026-b0myAMewCa/default.aspx](https://abc.xyz/investor/news/news-details/2026/Alphabet-Announces-Proposed-80-Billion-Equity-Capital-Raise-to-Expand-AI-Infrastructure-and-Compute-2026-b0myAMewCa/default.aspx)

生成摘要时出错

---

## 30. KDE at 30

**原文标题**: KDE at 30

**原文链接**: [https://kde.org/anniversaries/30/](https://kde.org/anniversaries/30/)

生成摘要时出错

---

## 31. GitHub and the crime against software

**原文标题**: GitHub and the crime against software

**原文链接**: [https://eblog.fly.dev/githubbad.html](https://eblog.fly.dev/githubbad.html)

生成摘要时出错

---

## 32. Stop Ruining It

**原文标题**: Stop Ruining It

**原文链接**: [https://seths.blog/2026/06/stop-ruining-it/](https://seths.blog/2026/06/stop-ruining-it/)

生成摘要时出错

---

## 33. Show HN: Eyeball

**原文标题**: Show HN: Eyeball

**原文链接**: [https://eyeball.rory.codes/](https://eyeball.rory.codes/)

生成摘要时出错

---

## 34. Atherton spent $145K to delay train electrification. The rest of us paid $400M

**原文标题**: Atherton spent $145K to delay train electrification. The rest of us paid $400M

**原文链接**: [https://peninsulaforeveryone.org/blog/atherton-spent-145k-to-delay-caltrain-electrification-the-rest-of-us-paid-400-million-and-waited-3-extra-years/](https://peninsulaforeveryone.org/blog/atherton-spent-145k-to-delay-caltrain-electrification-the-rest-of-us-paid-400-million-and-waited-3-extra-years/)

生成摘要时出错

---

## 35. Legal action forces Facebook whistleblower to sit in silence at Hay festival

**原文标题**: Legal action forces Facebook whistleblower to sit in silence at Hay festival

**原文链接**: [https://www.theguardian.com/technology/2026/may/31/meta-legal-action-forces-facebook-whistleblower-to-stay-silent-at-hay-festival](https://www.theguardian.com/technology/2026/may/31/meta-legal-action-forces-facebook-whistleblower-to-stay-silent-at-hay-festival)

生成摘要时出错

---

## 36. Three Ways to Get Paid (2018)

**原文标题**: Three Ways to Get Paid (2018)

**原文链接**: [https://jasonzweig.com/three-ways-to-get-paid/](https://jasonzweig.com/three-ways-to-get-paid/)

生成摘要时出错

---

## 37. Coreutils for Windows

**原文标题**: Coreutils for Windows

**原文链接**: [https://github.com/microsoft/coreutils](https://github.com/microsoft/coreutils)

生成摘要时出错

---

## 38. Morningstar values SpaceX at $780B, half its IPO target

**原文标题**: Morningstar values SpaceX at $780B, half its IPO target

**原文链接**: [https://www.reuters.com/business/media-telecom/morningstar-values-spacex-780-billion-half-its-ipo-target-2026-06-02/](https://www.reuters.com/business/media-telecom/morningstar-values-spacex-780-billion-half-its-ipo-target-2026-06-02/)

生成摘要时出错

---

## 39. Roughly a quarter of American professionals hit a wall in their careers

**原文标题**: Roughly a quarter of American professionals hit a wall in their careers

**原文链接**: [https://www.wsj.com/lifestyle/careers/white-collar-workers-career-nyu-study-a81a7d9c](https://www.wsj.com/lifestyle/careers/white-collar-workers-career-nyu-study-a81a7d9c)

生成摘要时出错

---

## 40. It's Not Just X. It's Y

**原文标题**: It's Not Just X. It's Y

**原文链接**: [https://mail.cyberneticforests.com/its-not-just-data-its-post-training/](https://mail.cyberneticforests.com/its-not-just-data-its-post-training/)

生成摘要时出错

---

## 41. Linux Basics for Hackers (2019)

**原文标题**: Linux Basics for Hackers (2019)

**原文链接**: [https://github.com/ahegazy0/linux-basics-for-hackers-notes](https://github.com/ahegazy0/linux-basics-for-hackers-notes)

生成摘要时出错

---

## 42. Windows GOG DOS Games on M-Series Macs

**原文标题**: Windows GOG DOS Games on M-Series Macs

**原文链接**: [https://f055.net/technology/windows-gog-dos-games-on-m-series-macs/](https://f055.net/technology/windows-gog-dos-games-on-m-series-macs/)

生成摘要时出错

---

## 43. Superintelligence: The Idea That Eats Smart People (2016)

**原文标题**: Superintelligence: The Idea That Eats Smart People (2016)

**原文链接**: [https://idlewords.com/talks/superintelligence.htm](https://idlewords.com/talks/superintelligence.htm)

生成摘要时出错

---

## 44. Flipper Zero Zig Template

**原文标题**: Flipper Zero Zig Template

**原文链接**: [https://github.com/NishantJoshi00/flipper-template](https://github.com/NishantJoshi00/flipper-template)

生成摘要时出错

---

## 45. Nvidia Cosmos 3

**原文标题**: Nvidia Cosmos 3

**原文链接**: [https://developer.nvidia.com/blog/develop-physical-ai-reasoning-world-and-action-models-with-nvidia-cosmos-3/](https://developer.nvidia.com/blog/develop-physical-ai-reasoning-world-and-action-models-with-nvidia-cosmos-3/)

生成摘要时出错

---

## 46. How is Groq raising more money?

**原文标题**: How is Groq raising more money?

**原文链接**: [https://www.zach.be/p/how-the-hell-is-groq-raising-more](https://www.zach.be/p/how-the-hell-is-groq-raising-more)

生成摘要时出错

---

## 47. MAI-Thinking-1

**原文标题**: MAI-Thinking-1

**原文链接**: [https://microsoft.ai/news/introducing-mai-thinking-1/](https://microsoft.ai/news/introducing-mai-thinking-1/)

生成摘要时出错

---

## 48. Expanding Project Glasswing

**原文标题**: Expanding Project Glasswing

**原文链接**: [https://www.anthropic.com/news/expanding-project-glasswing](https://www.anthropic.com/news/expanding-project-glasswing)

生成摘要时出错

---

## 49. Strace-ui, Bonsai_term, and the TUI renaissance

**原文标题**: Strace-ui, Bonsai_term, and the TUI renaissance

**原文链接**: [https://blog.janestreet.com/strace-ui-bonsai-term-and-the-tui-renaissance/](https://blog.janestreet.com/strace-ui-bonsai-term-and-the-tui-renaissance/)

生成摘要时出错

---

## 50. Cessation of public development of Kefir C compiler

**原文标题**: Cessation of public development of Kefir C compiler

**原文链接**: [https://kefir.protopopov.lv/posts/announce2.html](https://kefir.protopopov.lv/posts/announce2.html)

生成摘要时出错

---

## 51. Trump signs downsized AI order after weeks of reversals

**原文标题**: Trump signs downsized AI order after weeks of reversals

**原文链接**: [https://www.politico.com/news/2026/06/02/trump-signs-downsized-ai-order-00946389](https://www.politico.com/news/2026/06/02/trump-signs-downsized-ai-order-00946389)

生成摘要时出错

---

## 52. Fidonet: Technology, Use, Tools, and History (1993)

**原文标题**: Fidonet: Technology, Use, Tools, and History (1993)

**原文链接**: [https://www.fidonet.org/inet92_Randy_Bush.txt](https://www.fidonet.org/inet92_Randy_Bush.txt)

生成摘要时出错

---

## 53. When AI Crosses the Line: The Matplotlib Incident

**原文标题**: When AI Crosses the Line: The Matplotlib Incident

**原文链接**: [https://members.sigmazero.cc/posts/when-ai-crosses-159174096?postId=when-ai-crosses-159174096](https://members.sigmazero.cc/posts/when-ai-crosses-159174096?postId=when-ai-crosses-159174096)

生成摘要时出错

---

## 54. Malaysia enforces ban on social media accounts for children younger than 16

**原文标题**: Malaysia enforces ban on social media accounts for children younger than 16

**原文链接**: [https://apnews.com/article/malaysia-social-media-ban-16-bfaa7b01163b61b5d53c4ecfa870d133](https://apnews.com/article/malaysia-social-media-ban-16-bfaa7b01163b61b5d53c4ecfa870d133)

生成摘要时出错

---

## 55. CSS-Native Parallax Effect

**原文标题**: CSS-Native Parallax Effect

**原文链接**: [https://dan-webnotes.com/posts/2026-06-02-css-native-parallax-effect/](https://dan-webnotes.com/posts/2026-06-02-css-native-parallax-effect/)

生成摘要时出错

---

## 56. GrapheneOS Speech Services version 2 released

**原文标题**: GrapheneOS Speech Services version 2 released

**原文链接**: [https://discuss.grapheneos.org/d/36001-grapheneos-speech-services-version-2-released](https://discuss.grapheneos.org/d/36001-grapheneos-speech-services-version-2-released)

生成摘要时出错

---

## 57. Michael Burry says neither SpaceX nor Anthropic is worth $1T

**原文标题**: Michael Burry says neither SpaceX nor Anthropic is worth $1T

**原文链接**: [https://www.businessinsider.com/big-short-michael-burry-spacex-anthropic-ipo-ai-bubble-claude-2026-6](https://www.businessinsider.com/big-short-michael-burry-spacex-anthropic-ipo-ai-bubble-claude-2026-6)

生成摘要时出错

---

## 58. Uber caps employee AI spending after blowing through budget in four months

**原文标题**: Uber caps employee AI spending after blowing through budget in four months

**原文链接**: [https://techcrunch.com/2026/06/02/uber-caps-employee-ai-spending-after-blowing-through-budget-in-four-months/](https://techcrunch.com/2026/06/02/uber-caps-employee-ai-spending-after-blowing-through-budget-in-four-months/)

生成摘要时出错

---

## 59. Toy Story 5 shows 'terror' of children's screen addiction, says Tom Hanks

**原文标题**: Toy Story 5 shows 'terror' of children's screen addiction, says Tom Hanks

**原文链接**: [https://www.bbc.com/news/articles/cy5222wn410o](https://www.bbc.com/news/articles/cy5222wn410o)

生成摘要时出错

---

## 60. Is Python Becoming Pinyin?

**原文标题**: Is Python Becoming Pinyin?

**原文链接**: [https://lernerpython.com/2026/05/19/is-python-becoming-pinyin/](https://lernerpython.com/2026/05/19/is-python-becoming-pinyin/)

生成摘要时出错

---

## 61. Open Repair Data Standard – Open Repair Alliance

**原文标题**: Open Repair Data Standard – Open Repair Alliance

**原文链接**: [https://openrepair.org/open-data/open-standard/](https://openrepair.org/open-data/open-standard/)

生成摘要时出错

---

## 62. AI Doesn't Have ROI

**原文标题**: AI Doesn't Have ROI

**原文链接**: [https://www.wheresyoured.at/ai-doesnt-have-roi/](https://www.wheresyoured.at/ai-doesnt-have-roi/)

生成摘要时出错

---

## 63. Hackers Used Meta's AI Support Bot to Seize Instagram Accounts

**原文标题**: Hackers Used Meta's AI Support Bot to Seize Instagram Accounts

**原文链接**: [https://krebsonsecurity.com/2026/06/hackers-used-metas-ai-support-bot-to-seize-instagram-accounts/](https://krebsonsecurity.com/2026/06/hackers-used-metas-ai-support-bot-to-seize-instagram-accounts/)

生成摘要时出错

---

## 64. Rubin Tracks Skyscraper-Size Asteroids and Failed Supernovas

**原文标题**: Rubin Tracks Skyscraper-Size Asteroids and Failed Supernovas

**原文链接**: [https://www.quantamagazine.org/rubin-tracks-skyscraper-size-asteroids-failed-supernovas-and-interstellar-visitors-20260515/](https://www.quantamagazine.org/rubin-tracks-skyscraper-size-asteroids-failed-supernovas-and-interstellar-visitors-20260515/)

生成摘要时出错

---

## 65. Rift: Better Alternative to Git Worktrees

**原文标题**: Rift: Better Alternative to Git Worktrees

**原文链接**: [https://github.com/anomalyco/rift](https://github.com/anomalyco/rift)

生成摘要时出错

---

## 66. How we index images for RAG

**原文标题**: How we index images for RAG

**原文链接**: [https://www.kapa.ai/blog/how-we-index-images-for-rag](https://www.kapa.ai/blog/how-we-index-images-for-rag)

生成摘要时出错

---

## 67. Amazon paid music subscription will soon include ads and lose downloads

**原文标题**: Amazon paid music subscription will soon include ads and lose downloads

**原文链接**: [https://old.reddit.com/r/mildlyinfuriating/comments/1tur3w5/amazon_just_informed_me_that_my_paid_music/](https://old.reddit.com/r/mildlyinfuriating/comments/1tur3w5/amazon_just_informed_me_that_my_paid_music/)

生成摘要时出错

---

## 68. Florida AG files lawsuit against OpenAI, CEO Sam Altman for deceptive practices

**原文标题**: Florida AG files lawsuit against OpenAI, CEO Sam Altman for deceptive practices

**原文链接**: [https://www.myfloridalegal.com/newsrelease/attorney-general-james-uthmeier-files-first-nation-state-led-lawsuit-against-openai-ceo](https://www.myfloridalegal.com/newsrelease/attorney-general-james-uthmeier-files-first-nation-state-led-lawsuit-against-openai-ceo)

生成摘要时出错

---

## 69. Martin Scorsese Is Embracing A.I.

**原文标题**: Martin Scorsese Is Embracing A.I.

**原文链接**: [https://www.nytimes.com/2026/06/02/business/media/martin-scorsese-artificial-intelligence.html](https://www.nytimes.com/2026/06/02/business/media/martin-scorsese-artificial-intelligence.html)

生成摘要时出错

---

## 70. Radxa Dragon Q8B: A Laptop Cosplaying as an SBC?

**原文标题**: Radxa Dragon Q8B: A Laptop Cosplaying as an SBC?

**原文链接**: [https://bret.dk/radxa-dragon-q8b-a-laptop-cosplaying-as-an-sbc/](https://bret.dk/radxa-dragon-q8b-a-laptop-cosplaying-as-an-sbc/)

生成摘要时出错

---

## 71. Lid-lifting Kiwi author forced to sit in silence at writers' festival

**原文标题**: Lid-lifting Kiwi author forced to sit in silence at writers' festival

**原文链接**: [https://www.rnz.co.nz/life/books/lid-lifting-kiwi-author-forced-to-sit-in-silence-at-writers-festival](https://www.rnz.co.nz/life/books/lid-lifting-kiwi-author-forced-to-sit-in-silence-at-writers-festival)

生成摘要时出错

---

## 72. Pogroms, American Style

**原文标题**: Pogroms, American Style

**原文链接**: [https://paulkrugman.substack.com/p/pogroms-american-style](https://paulkrugman.substack.com/p/pogroms-american-style)

生成摘要时出错

---

## 73. Nvidia announces new AI chip for personal computers

**原文标题**: Nvidia announces new AI chip for personal computers

**原文链接**: [https://www.bbc.com/news/articles/crmp9mppvzro](https://www.bbc.com/news/articles/crmp9mppvzro)

生成摘要时出错

---

## 74. Anthropic scales Claude Mythos to critical infrastructure in 15 countries

**原文标题**: Anthropic scales Claude Mythos to critical infrastructure in 15 countries

**原文链接**: [https://techcrunch.com/2026/06/02/anthropic-scales-claude-mythos-to-critical-infrastructure-in-15-countries/](https://techcrunch.com/2026/06/02/anthropic-scales-claude-mythos-to-critical-infrastructure-in-15-countries/)

生成摘要时出错

---

## 75. Angry devs vow to flee GitHub Copilot as metered billing takes hold

**原文标题**: Angry devs vow to flee GitHub Copilot as metered billing takes hold

**原文链接**: [https://www.theregister.com/ai-and-ml/2026/06/02/github-copilot-users-threaten-exit-as-metered-billing-kicks-in/5249826](https://www.theregister.com/ai-and-ml/2026/06/02/github-copilot-users-threaten-exit-as-metered-billing-kicks-in/5249826)

生成摘要时出错

---

## 76. The Infosec Phrasebook

**原文标题**: The Infosec Phrasebook

**原文链接**: [https://nesbitt.io/2026/06/01/the-infosec-phrasebook.html](https://nesbitt.io/2026/06/01/the-infosec-phrasebook.html)

生成摘要时出错

---

## 77. Amazon Shuts Down Internal AI Leaderboard After Employees Cheated

**原文标题**: Amazon Shuts Down Internal AI Leaderboard After Employees Cheated

**原文链接**: [https://www.404media.co/amazon-shuts-down-internal-ai-leaderboard-after-employees-cheated/](https://www.404media.co/amazon-shuts-down-internal-ai-leaderboard-after-employees-cheated/)

生成摘要时出错

---

## 78. Macron announces 93B euros in 'Choose France' investments

**原文标题**: Macron announces 93B euros in 'Choose France' investments

**原文链接**: [https://www.euractiv.com/news/macron-announces-93-bn-euros-in-choose-france-investments/](https://www.euractiv.com/news/macron-announces-93-bn-euros-in-choose-france-investments/)

生成摘要时出错

---

## 79. Qwen3.7-Plus: Multimodal Agent Intelligence

**原文标题**: Qwen3.7-Plus: Multimodal Agent Intelligence

**原文链接**: [https://qwen.ai/blog?id=qwen3.7-plus](https://qwen.ai/blog?id=qwen3.7-plus)

生成摘要时出错

---

## 80. My thoughts after using Clojure for about a month

**原文标题**: My thoughts after using Clojure for about a month

**原文链接**: [https://www.acdw.net/clojure/](https://www.acdw.net/clojure/)

生成摘要时出错

---

## 81. I rode Elon Musk's Vegas Loop, the worst transit system on Earth

**原文标题**: I rode Elon Musk's Vegas Loop, the worst transit system on Earth

**原文链接**: [https://www.sfgate.com/travel/article/vegas-loop-22280647.php?link_source=ta_bluesky_link&taid=6a1eccd39d9fbd0001ae2644&utm_campaign=trueanthem%2B3984&utm_medium=social&utm_source=bluesky](https://www.sfgate.com/travel/article/vegas-loop-22280647.php?link_source=ta_bluesky_link&taid=6a1eccd39d9fbd0001ae2644&utm_campaign=trueanthem%2B3984&utm_medium=social&utm_source=bluesky)

生成摘要时出错

---

## 82. Trump Administration to Dismantle Ocean Monitoring System

**原文标题**: Trump Administration to Dismantle Ocean Monitoring System

**原文链接**: [https://www.nytimes.com/2026/06/01/climate/ocean-observatories-initiative.html](https://www.nytimes.com/2026/06/01/climate/ocean-observatories-initiative.html)

生成摘要时出错

---

## 83. Show HN: DepsGuard – One command to harden NPM/pnpm/yarn/bun/uv configs

**原文标题**: Show HN: DepsGuard – One command to harden NPM/pnpm/yarn/bun/uv configs

**原文链接**: [https://github.com/arnica/depsguard](https://github.com/arnica/depsguard)

生成摘要时出错

---

## 84. Build a Basic AI Agent from Scratch: Tools

**原文标题**: Build a Basic AI Agent from Scratch: Tools

**原文链接**: [https://www.ruxu.dev/articles/ai/build-an-ai-agent-with-tools/](https://www.ruxu.dev/articles/ai/build-an-ai-agent-with-tools/)

生成摘要时出错

---

## 85. Unlawful by design: Exposing the human rights costs of generative AI

**原文标题**: Unlawful by design: Exposing the human rights costs of generative AI

**原文链接**: [https://www.amnesty.org/en/documents/pol40/0996/2026/en/](https://www.amnesty.org/en/documents/pol40/0996/2026/en/)

生成摘要时出错

---

## 86. We Sued ICE to Get Its Spyware Contract. The Agency Redacted Nearly Everything

**原文标题**: We Sued ICE to Get Its Spyware Contract. The Agency Redacted Nearly Everything

**原文链接**: [https://www.404media.co/we-sued-ice-to-get-its-spyware-contract-the-agency-is-redacting-essentially-everything/](https://www.404media.co/we-sued-ice-to-get-its-spyware-contract-the-agency-is-redacting-essentially-everything/)

生成摘要时出错

---

