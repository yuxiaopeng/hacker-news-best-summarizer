# Hacker News 热门文章摘要 (2026-11-05)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. Postman 静默自动安装AI插件并试图共享所有API数据

**原文标题**: Postman silently auto-installs AI plugins and attempts to share all API data

**原文链接**: [https://github.com/postmanlabs/postman-app-support/issues/14370](https://github.com/postmanlabs/postman-app-support/issues/14370)

已有报告指出一个严重问题，详细说明了Postman桌面应用程序(v12.33.4)在未经用户明确同意的情况下，据称自动安装了AI插件（Codex 1.1.0, Claude Code 2.0.1）以及一个Postman命令行工具 (CLI)。

来自Mac设备的证据显示，Postman的日志记录了这些安装为“auto-existing-upgrade”。据报道，该过程修改了编码代理的全局用户配置，启用了Postman插件，并注入了一个启动指令钩子。这个钩子指示AI代理将“任何重要的API工程任务”通过Postman路由，从而有效地使Postman成为API工程工作流程的默认选择。

一个主要担忧是，Postman的安装程序明确试图自我批准其自身的钩子，绕过了用户的信任和同意。该安装还启用了一个远程的Postman管理控制平面 (MCP) 连接。

用户将此归类为“严重的同意和信任边界问题”，要求停止自动安装、移除自我批准、明确选择加入集成，并提供一个完整的卸载路径。该问题已引起社区的广泛负面反馈，许多用户对此表示担忧，并将Postman的行为比作恶意软件。

---

## 2. AI迫使我们偿还40年的技术债务。

**原文标题**: AI is forcing us to pay off 40 years of technical debt

**原文链接**: [https://spectrum.ieee.org/ai-in-cybersecurity-php2shell-vulnerability](https://spectrum.ieee.org/ai-in-cybersecurity-php2shell-vulnerability)

这篇题为“人工智能正迫使我们偿还40年的技术债务”的ComputingNews文章认为，人工智能正在揭示数十年累积的技术负债，并迫使人们对其采取行动。该文章特别指出“PHP2Shell漏洞”是一起重大事件，被描述为预示着“网络安全地狱”，这突显了这项技术债务的严重影响。该文章由IEEE Spectrum的计算和硬件编辑Dina Genkina撰写，并于2026年11月2日发布。阅读时长为四分钟。

---

## 3. 题为“Astra可以读写权重以改进Qwen”的帖子具有误导性。

**原文标题**: The 'Astra can read and write weights to improve Qwen' post is misleading

**原文链接**: [https://honnibal.dev/blog/astra-read-write-misleading](https://honnibal.dev/blog/astra-read-write-misleading)

本文认为，“Astra可以读写权重来改进Qwen”的帖子具有误导性，就像魔术师的把戏，暗示一种单一技术可以完成多种壮举。原始摘要指出，GPT-6 Astra取得的成果（包括改进Qwen的数学能力）是“仅仅通过查看原始权重”来实现的。然而，作者详细说明这并非普遍适用。

文章将原始帖子的实验分为两类。只有实验1、2和4（涉及用于识别游戏类型或修复汽车保险策略等任务的小型网络，权重范围为1.7万至17.2万）才真正依赖Astra在没有额外工具或运行网络的情况下分析“原始权重”。

相比之下，更复杂和引人注目的成就，例如从头开始编写游戏网络（实验5、6）以及显著提高Qwen3.5的数学性能（实验8），*并未*使用这种仅查看原始权重的方法。这些令人印象深刻的结果涉及Astra编写并执行Python程序，对于Qwen，还包括在多达50批练习题上运行模型。

作者总结道，将这些不同的方法论混为一谈，会造成一种单一、深刻能力的错误印象。尽管Astra通过Python设计和执行机器学习工程任务的能力值得关注，但这与“仅仅查看原始权重”有着根本区别，不应混淆，特别是对于备受瞩目的Qwen成果。

---

## 4. 斯特林曼，一款800美元的开源房间尺度抓取机器人

**原文标题**: Stringman, an $800 open-source room scale gripper robot

**原文链接**: [https://neufangled.com/](https://neufangled.com/)

文章介绍了“Stringman”——一款售价800美元的开源房间尺度抓手机器人。所提供的内容给出了安装固定件的具体说明，这些固定件可能对机器人的设置或运行至关重要。这些固定件既可以用木螺钉固定在靠近天花板的墙柱上，也可以用棘轮捆扎带固定在柱子上，这表明该系统具有灵活的安装选项。

---

## 5. Qwen 3.8 27B 在我的笔记本电脑上也能解释模型权重。

**原文标题**: Qwen 3.8 27B on my laptop can interpret model weights, too

**原文链接**: [https://simonwillison.net/2026/Nov/3/qwen-can-interpret-model-weights/](https://simonwillison.net/2026/Nov/3/qwen-can-interpret-model-weights/)

本文演示了在笔记本电脑上本地运行的Qwen 3.8 27B能够解释原始神经网络权重。这种被称为“权重空间编程”（Weight-Space Programming）的能力，最近被《权重空间编程的火花》（Sparks of Weight-Space Programming）这篇论文所强调，该论文声称GPT-6 Astra等前沿模型可以在无需外部工具的情况下分析和修改权重。

作者侧重于“无需工具”这一方面，回应了关于原始论文将纯粹的权重解释与工具辅助的修改混为一谈的批评。作者使用原始论文GitHub上的提示，将来自训练用于玩简化网格游戏（打砖块、乒乓、吃豆人、高速公路）的网络的原始权重输入给Qwen 3.8 27B，并要求模型识别游戏。

在具有长上下文窗口的笔记本电脑上运行的Qwen 3.8 27B，成功识别了吃豆人、乒乓和打砖块，并在经过大量的处理时间（45分钟到一小时以上）和token使用后，提供了描述和置信度。它在识别更鲜为人知的高速公路游戏时遇到了困难。

尽管作者承认Qwen直接“读取”权重的能力令人印象深刻，但告诫不要夸大其影响，强调复杂的推理痕迹并不一定意味着源代码的终结，也不是一个无法理解的机器自我编辑时代的到来。

---

## 6. 谷歌将对拒绝人工智能的学校关闭搜索

**原文标题**: Google will turn off search for schools that reject AI

**原文链接**: [https://www.nytimes.com/2026/11/03/us/google-search-schools-restrict-ai.html](https://www.nytimes.com/2026/11/03/us/google-search-schools-restrict-ai.html)

无法访问文章链接。

---

## 7. 英伟达 RTX Spark 加密固件使 Linux 推理速度降至 35%。

**原文标题**: Nvidia RTX Spark encrypted firmware slows inference speed to 35% on Linux

**原文链接**: [https://www.mindstudio.ai/blog/linux-nvidia-rtx-spark-laptop](https://www.mindstudio.ai/blog/linux-nvidia-rtx-spark-laptop)

生成摘要时出错

---

## 8. North Korean fake job interview led to $6.3B Binance heist

**原文标题**: North Korean fake job interview led to $6.3B Binance heist

**原文链接**: [https://www.theregister.com/security/2026/11/03/north-korean-fake-job-interview-led-to-63b-binance-heist/5307398](https://www.theregister.com/security/2026/11/03/north-korean-fake-job-interview-led-to-63b-binance-heist/5307398)

生成摘要时出错

---

## 9. Residential proxies detected on White House network

**原文标题**: Residential proxies detected on White House network

**原文链接**: [https://layer3intel.com/blog/residential-proxies-white-house-network](https://layer3intel.com/blog/residential-proxies-white-house-network)

生成摘要时出错

---

## 10. Safari introduces Adaptive Dark Mode in 27.3

**原文标题**: Safari introduces Adaptive Dark Mode in 27.3

**原文链接**: [https://webkit.org/blog/18541/introducing-adaptive-dark-mode/](https://webkit.org/blog/18541/introducing-adaptive-dark-mode/)

生成摘要时出错

---

## 11. Kalshi and its co-founders face felony charges for violating Utah gambling laws

**原文标题**: Kalshi and its co-founders face felony charges for violating Utah gambling laws

**原文链接**: [https://arstechnica.com/tech-policy/2026/10/trump-admin-sues-utah-to-save-kalshi-from-the-states-total-ban-on-gambling/](https://arstechnica.com/tech-policy/2026/10/trump-admin-sues-utah-to-save-kalshi-from-the-states-total-ban-on-gambling/)

生成摘要时出错

---

## 12. Could a modern chess engine on a Pentium have defeated Kasparov in 1996?

**原文标题**: Could a modern chess engine on a Pentium have defeated Kasparov in 1996?

**原文链接**: [https://nicholas.carlini.com/writing/2026/algorithmic-improvements-chess.html](https://nicholas.carlini.com/writing/2026/algorithmic-improvements-chess.html)

生成摘要时出错

---

## 13. Show HN: Hacker Times, a New York Times-inspired version of Hacker News

**原文标题**: Show HN: Hacker Times, a New York Times-inspired version of Hacker News

**原文链接**: [https://hackertimes.ca/](https://hackertimes.ca/)

生成摘要时出错

---

## 14. Show HN: HackerTV – HN's most-recommended Youtube videos as 24/7 TV channels

**原文标题**: Show HN: HackerTV – HN's most-recommended Youtube videos as 24/7 TV channels

**原文链接**: [https://hackertv.org](https://hackertv.org)

生成摘要时出错

---

## 15. Jelly Sheet

**原文标题**: Jelly Sheet

**原文链接**: [https://mrdoob.github.io/codevember-2026/01/](https://mrdoob.github.io/codevember-2026/01/)

生成摘要时出错

---

## 16. AMD expects to outsell Intel in Q4 for the first time in history

**原文标题**: AMD expects to outsell Intel in Q4 for the first time in history

**原文链接**: [https://www.tomshardware.com/pc-components/cpus/amd-expects-to-outsell-intel-in-q4-for-the-first-time-in-history-usd17b-guidance-would-exceed-intels-projections](https://www.tomshardware.com/pc-components/cpus/amd-expects-to-outsell-intel-in-q4-for-the-first-time-in-history-usd17b-guidance-would-exceed-intels-projections)

生成摘要时出错

---

## 17. Mac at any scale

**原文标题**: Mac at any scale

**原文链接**: [https://namespace.so/blog/mac-at-any-scale](https://namespace.so/blog/mac-at-any-scale)

生成摘要时出错

---

## 18. US tech giants' hidden AI debt swells 90% to $3.2T in 6 months

**原文标题**: US tech giants' hidden AI debt swells 90% to $3.2T in 6 months

**原文链接**: [https://asia.nikkei.com/business/technology/artificial-intelligence/us-tech-giants-hidden-ai-debt-swells-90-to-3.2tn-in-6-months](https://asia.nikkei.com/business/technology/artificial-intelligence/us-tech-giants-hidden-ai-debt-swells-90-to-3.2tn-in-6-months)

生成摘要时出错

---

## 19. C++26 Disapproved

**原文标题**: C++26 Disapproved

**原文链接**: [https://andreasfertig.com/blog/2026/11/cpp26-dis-failed-how-does-cpp-survive/](https://andreasfertig.com/blog/2026/11/cpp26-dis-failed-how-does-cpp-survive/)

生成摘要时出错

---

## 20. The Little Book of Generative AI Foundations: An Intuitive Mathematical Primer

**原文标题**: The Little Book of Generative AI Foundations: An Intuitive Mathematical Primer

**原文链接**: [https://arxiv.org/abs/2605.29713](https://arxiv.org/abs/2605.29713)

生成摘要时出错

---

## 21. The Internals of PostgreSQL

**原文标题**: The Internals of PostgreSQL

**原文链接**: [https://www.interdb.jp/pg/index.html](https://www.interdb.jp/pg/index.html)

生成摘要时出错

---

## 22. DiscImageStudio: burn visible artwork onto CDs, DVDs and Blu-ray discs

**原文标题**: DiscImageStudio: burn visible artwork onto CDs, DVDs and Blu-ray discs

**原文链接**: [https://github.com/JiaFeiMiao-K-Cat/DiscImageStudio](https://github.com/JiaFeiMiao-K-Cat/DiscImageStudio)

生成摘要时出错

---

## 23. Kitty 0.50

**原文标题**: Kitty 0.50

**原文链接**: [https://sw.kovidgoyal.net/kitty/changelog/#](https://sw.kovidgoyal.net/kitty/changelog/#)

生成摘要时出错

---

## 24. Kimi K3.1 Pro model weights are out

**原文标题**: Kimi K3.1 Pro model weights are out

**原文链接**: [https://huggingface.co/moonshotai/Kimi-K3.1-Pro](https://huggingface.co/moonshotai/Kimi-K3.1-Pro)

生成摘要时出错

---

## 25. US voters roundly reject data centers in ballot measures

**原文标题**: US voters roundly reject data centers in ballot measures

**原文链接**: [https://www.semafor.com/article/11/04/2026/us-voters-roundly-reject-data-centers-in-ballot-measures](https://www.semafor.com/article/11/04/2026/us-voters-roundly-reject-data-centers-in-ballot-measures)

生成摘要时出错

---

## 26. Geoffrey Hinton: it might turn out we were better off without AI

**原文标题**: Geoffrey Hinton: it might turn out we were better off without AI

**原文链接**: [https://www.theguardian.com/uk-news/2026/nov/03/ai-godfather-geoffrey-hinton-better-off-without-ai](https://www.theguardian.com/uk-news/2026/nov/03/ai-godfather-geoffrey-hinton-better-off-without-ai)

生成摘要时出错

---

## 27. Nvidia – open-source auto-ontology

**原文标题**: Nvidia – open-source auto-ontology

**原文链接**: [https://github.com/NVIDIA/auto-ontology](https://github.com/NVIDIA/auto-ontology)

生成摘要时出错

---

## 28. Scaling Git at OpenAI

**原文标题**: Scaling Git at OpenAI

**原文链接**: [https://openai.com/index/scaling-git-at-openai/](https://openai.com/index/scaling-git-at-openai/)

生成摘要时出错

---

## 29. Study estimates 75% of NFL players who died over 15-year span had CTE

**原文标题**: Study estimates 75% of NFL players who died over 15-year span had CTE

**原文链接**: [https://www.nbcnews.com/health/health-news/study-estimates-75-nfl-players-died-15-year-span-may-cte-rcna605975](https://www.nbcnews.com/health/health-news/study-estimates-75-nfl-players-died-15-year-span-may-cte-rcna605975)

生成摘要时出错

---

## 30. Democrats win control of the House of Representatives

**原文标题**: Democrats win control of the House of Representatives

**原文链接**: [https://www.nbcnews.com/politics/2026-election/democrats-house-control-midterm-election-wins-trump-check-rcna603397](https://www.nbcnews.com/politics/2026-election/democrats-house-control-midterm-election-wins-trump-check-rcna603397)

生成摘要时出错

---

## 31. Incident with Pull Requests, Git Operations and Issues

**原文标题**: Incident with Pull Requests, Git Operations and Issues

**原文链接**: [https://www.githubstatus.com/incidents/smtdswd1h2w4](https://www.githubstatus.com/incidents/smtdswd1h2w4)

生成摘要时出错

---

## 32. How I use AI (Oct 2026)

**原文标题**: How I use AI (Oct 2026)

**原文链接**: [https://ben.stolovitz.com/posts/how-use-ai-oct-2026/](https://ben.stolovitz.com/posts/how-use-ai-oct-2026/)

生成摘要时出错

---

## 33. Guerrilla bike lanes: San Francisco makes illicit infrastructure permanent (2016)

**原文标题**: Guerrilla bike lanes: San Francisco makes illicit infrastructure permanent (2016)

**原文链接**: [https://99percentinvisible.org/article/guerrilla-bike-lanes-san-francisco-makes-illicit-infrastructure-permanent/](https://99percentinvisible.org/article/guerrilla-bike-lanes-san-francisco-makes-illicit-infrastructure-permanent/)

生成摘要时出错

---

## 34. Intel stock collapse worsens as $3.5T chip rout spreads

**原文标题**: Intel stock collapse worsens as $3.5T chip rout spreads

**原文链接**: [https://finance.yahoo.com/markets/article/the-intel-stock-collapse-is-getting-worse--and-the-37-trillion-chip-rout-is-spreading-212154947.html](https://finance.yahoo.com/markets/article/the-intel-stock-collapse-is-getting-worse--and-the-37-trillion-chip-rout-is-spreading-212154947.html)

生成摘要时出错

---

## 35. Preparing for the Flipper One Kickstarter and opening pre-orders

**原文标题**: Preparing for the Flipper One Kickstarter and opening pre-orders

**原文链接**: [https://flipper.net/pages/flipper-one](https://flipper.net/pages/flipper-one)

生成摘要时出错

---

## 36. Verification Is Not Knowledge: Science needs more than answers

**原文标题**: Verification Is Not Knowledge: Science needs more than answers

**原文链接**: [https://blog.cosmos-institute.org/p/verification-is-not-knowledge](https://blog.cosmos-institute.org/p/verification-is-not-knowledge)

生成摘要时出错

---

## 37. A new Go API for JSON

**原文标题**: A new Go API for JSON

**原文链接**: [https://go.dev/blog/jsonv2](https://go.dev/blog/jsonv2)

生成摘要时出错

---

## 38. Ripple-65B Preview: U.S. Open-Weight SOTA on Agentic Coding

**原文标题**: Ripple-65B Preview: U.S. Open-Weight SOTA on Agentic Coding

**原文链接**: [https://www.ricursive.com/ripple](https://www.ricursive.com/ripple)

生成摘要时出错

---

## 39. Net worth for people aged 30–33 in the U.S.

**原文标题**: Net worth for people aged 30–33 in the U.S.

**原文链接**: [https://www.keepingup.com/benchmarks/net-worth/age-30-33](https://www.keepingup.com/benchmarks/net-worth/age-30-33)

生成摘要时出错

---

## 40. Synaptics Appears to Use Legal Threats to Block Open-Source DisplayLink Driver

**原文标题**: Synaptics Appears to Use Legal Threats to Block Open-Source DisplayLink Driver

**原文链接**: [https://www.phoronix.com/news/Synaptics-Blocks-Vino-Driver](https://www.phoronix.com/news/Synaptics-Blocks-Vino-Driver)

生成摘要时出错

---

## 41. Revolut moves to self-hosted GLM

**原文标题**: Revolut moves to self-hosted GLM

**原文链接**: [https://twitter.com/guilleflorvs/status/2117379073785696395](https://twitter.com/guilleflorvs/status/2117379073785696395)

生成摘要时出错

---

## 42. Just a little AI resistance, as a treat

**原文标题**: Just a little AI resistance, as a treat

**原文链接**: [https://shkspr.mobi/blog/2026/11/just-a-little-ai-resistance-as-a-treat/](https://shkspr.mobi/blog/2026/11/just-a-little-ai-resistance-as-a-treat/)

生成摘要时出错

---

## 43. Tencent Hy4

**原文标题**: Tencent Hy4

**原文链接**: [https://hy.tencent.ai/research/hy4](https://hy.tencent.ai/research/hy4)

生成摘要时出错

---

## 44. Progress on provable inference for large language models

**原文标题**: Progress on provable inference for large language models

**原文链接**: [https://www.anthropic.com/research/provable-inference](https://www.anthropic.com/research/provable-inference)

生成摘要时出错

---

## 45. OpenAI to acquire Pierre Computer Company

**原文标题**: OpenAI to acquire Pierre Computer Company

**原文链接**: [https://openai.com/index/openai-to-acquire-pierre/](https://openai.com/index/openai-to-acquire-pierre/)

生成摘要时出错

---

## 46. I dumped Apple’s word list

**原文标题**: I dumped Apple’s word list

**原文链接**: [https://helgesver.re/articles/macos-vulgar-word-flags](https://helgesver.re/articles/macos-vulgar-word-flags)

生成摘要时出错

---

## 47. Insects don't swarm at LED lights

**原文标题**: Insects don't swarm at LED lights

**原文链接**: [https://www.birdsoutsidemywindow.org/2026/11/03/insects-dont-swarm-at-led-lights/](https://www.birdsoutsidemywindow.org/2026/11/03/insects-dont-swarm-at-led-lights/)

生成摘要时出错

---

## 48. The lost malloc()

**原文标题**: The lost malloc()

**原文链接**: [https://napcakes.nekoweb.org/posts/malloc/](https://napcakes.nekoweb.org/posts/malloc/)

生成摘要时出错

---

## 49. Giant canyon on Mars is still tectonically active

**原文标题**: Giant canyon on Mars is still tectonically active

**原文链接**: [https://lamont.columbia.edu/news/giant-canyon-mars-still-tectonically-active-today](https://lamont.columbia.edu/news/giant-canyon-mars-still-tectonically-active-today)

生成摘要时出错

---

## 50. macOS 27 does not support CoreStorage volumes

**原文标题**: macOS 27 does not support CoreStorage volumes

**原文链接**: [https://wadetregaskis.com/macos-27-golden-gate-does-not-actually-support-corestorage-or-hfs-volumes/](https://wadetregaskis.com/macos-27-golden-gate-does-not-actually-support-corestorage-or-hfs-volumes/)

生成摘要时出错

---

## 51. Debian apt security update (man-in-the-middle)

**原文标题**: Debian apt security update (man-in-the-middle)

**原文链接**: [https://lists.debian.org/debian-security-announce/2026/msg00526.html?pow_referer=](https://lists.debian.org/debian-security-announce/2026/msg00526.html?pow_referer=)

生成摘要时出错

---

## 52. uBlock Origin filter to block autoplay videos in TechCrunch

**原文标题**: uBlock Origin filter to block autoplay videos in TechCrunch

**原文链接**: [https://cornfieldlabs.github.io/posts/ublock-stop-techcrunch-autoplay-video/post.html](https://cornfieldlabs.github.io/posts/ublock-stop-techcrunch-autoplay-video/post.html)

生成摘要时出错

---

## 53. US midterm elections 2026 live updates: Democrats win Senate control and edge

**原文标题**: US midterm elections 2026 live updates: Democrats win Senate control and edge

**原文链接**: [https://www.theguardian.com/us-news/live/2026/nov/03/midterm-election-results-live-updates](https://www.theguardian.com/us-news/live/2026/nov/03/midterm-election-results-live-updates)

生成摘要时出错

---

## 54. AI is destroying my CS degree

**原文标题**: AI is destroying my CS degree

**原文链接**: [https://lordtoots.bearblog.dev/ai-is-destroying-my-cs-degree/](https://lordtoots.bearblog.dev/ai-is-destroying-my-cs-degree/)

生成摘要时出错

---

## 55. Charles Tandy, the mastermind behind Radio Shack

**原文标题**: Charles Tandy, the mastermind behind Radio Shack

**原文链接**: [https://dfarq.homeip.net/charles-tandy-the-mastermind-behind-radio-shack/](https://dfarq.homeip.net/charles-tandy-the-mastermind-behind-radio-shack/)

生成摘要时出错

---

## 56. BYD doubles its Brazil market share to 9.7% a year after opening its local plant

**原文标题**: BYD doubles its Brazil market share to 9.7% a year after opening its local plant

**原文链接**: [https://www.bloomberg.com/news/articles/2026-11-03/china-s-byd-doubles-market-share-in-brazil-with-new-plant-eyed](https://www.bloomberg.com/news/articles/2026-11-03/china-s-byd-doubles-market-share-in-brazil-with-new-plant-eyed)

生成摘要时出错

---

## 57. Distinct cellular and genetic differences in colorectal cancer in young patients

**原文标题**: Distinct cellular and genetic differences in colorectal cancer in young patients

**原文链接**: [https://www.dana-farber.org/newsroom/news-releases/2026/study-reveals-distinct-cellular-and-genetic-differences-in-colorectal-cancer-in-younger-patients](https://www.dana-farber.org/newsroom/news-releases/2026/study-reveals-distinct-cellular-and-genetic-differences-in-colorectal-cancer-in-younger-patients)

生成摘要时出错

---

## 58. Bear turns 10, and it still feels like day one

**原文标题**: Bear turns 10, and it still feels like day one

**原文链接**: [https://blog.bear.app/2026/11/bear-turns-10-and-it-still-feels-like-day-one/](https://blog.bear.app/2026/11/bear-turns-10-and-it-still-feels-like-day-one/)

生成摘要时出错

---

## 59. Show HN: Uncracked City, detective game where you question LLM suspects that lie

**原文标题**: Show HN: Uncracked City, detective game where you question LLM suspects that lie

**原文链接**: [https://uncracked.city](https://uncracked.city)

生成摘要时出错

---

## 60. Everything is an AI scam now

**原文标题**: Everything is an AI scam now

**原文链接**: [https://www.davidralphlewis.co.uk/posts/everything-is-an-ai-scam-now/](https://www.davidralphlewis.co.uk/posts/everything-is-an-ai-scam-now/)

生成摘要时出错

---

## 61. There is no posttraining data commons

**原文标题**: There is no posttraining data commons

**原文链接**: [https://openathena.ai/blog/there-is-no-posttraining-data-commons/](https://openathena.ai/blog/there-is-no-posttraining-data-commons/)

生成摘要时出错

---

## 62. Education shouldn't be held for ransom

**原文标题**: Education shouldn't be held for ransom

**原文链接**: [https://blog.kagi.com/education-should-not-be-held-for-ransom](https://blog.kagi.com/education-should-not-be-held-for-ransom)

生成摘要时出错

---

## 63. Practice speaking Japanese with real YouTube videos, graded line by line

**原文标题**: Practice speaking Japanese with real YouTube videos, graded line by line

**原文链接**: [https://jivx.com/yt](https://jivx.com/yt)

生成摘要时出错

---

## 64. This Month in Ladybird – October 2026

**原文标题**: This Month in Ladybird – October 2026

**原文链接**: [https://ladybird.org/newsletter/2026-10-31/](https://ladybird.org/newsletter/2026-10-31/)

生成摘要时出错

---

## 65. Show HN: Kairos – Open-source risk and fraud decisioning platform

**原文标题**: Show HN: Kairos – Open-source risk and fraud decisioning platform

**原文链接**: [https://github.com/finic-ai/kairos](https://github.com/finic-ai/kairos)

生成摘要时出错

---

## 66. Microsoft fixes a Windows 11 annoyance as PC revenue declines

**原文标题**: Microsoft fixes a Windows 11 annoyance as PC revenue declines

**原文链接**: [https://arstechnica.com/gadgets/2026/10/windows-11-gets-right-click-menu-improvements-as-pc-revenue-slides/](https://arstechnica.com/gadgets/2026/10/windows-11-gets-right-click-menu-improvements-as-pc-revenue-slides/)

生成摘要时出错

---

## 67. Have I befriended a murderer?

**原文标题**: Have I befriended a murderer?

**原文链接**: [https://longreads.com/2026/11/03/murder-friendship-doubt/](https://longreads.com/2026/11/03/murder-friendship-doubt/)

生成摘要时出错

---

## 68. Evergreen: A Provably Safe Systems Language

**原文标题**: Evergreen: A Provably Safe Systems Language

**原文链接**: [https://evergreenlang.net](https://evergreenlang.net)

生成摘要时出错

---

## 69. Quili AI

**原文标题**: Quili AI

**原文链接**: [https://www.quili.ai/](https://www.quili.ai/)

生成摘要时出错

---

## 70. Debian apt security update: man-in-the-middle arbitrary code execution

**原文标题**: Debian apt security update: man-in-the-middle arbitrary code execution

**原文链接**: [https://lists.debian.org/debian-security-announce/2026/msg00526.html](https://lists.debian.org/debian-security-announce/2026/msg00526.html)

生成摘要时出错

---

## 71. Show HN: After a decade of reversing, I got co-op working in DOS Wing Commander

**原文标题**: Show HN: After a decade of reversing, I got co-op working in DOS Wing Commander

**原文链接**: [https://fireflyk64.github.io/wcmulti/](https://fireflyk64.github.io/wcmulti/)

生成摘要时出错

---

## 72. Binance hackers used fake job interview to breach PC before $6.3B attack

**原文标题**: Binance hackers used fake job interview to breach PC before $6.3B attack

**原文链接**: [https://www.reuters.com/world/binance-says-hackers-used-fake-job-interview-compromise-computer-before-63-2026-11-03/](https://www.reuters.com/world/binance-says-hackers-used-fake-job-interview-compromise-computer-before-63-2026-11-03/)

生成摘要时出错

---

## 73. Google researchers demand freedom to tell the world what they know about AI

**原文标题**: Google researchers demand freedom to tell the world what they know about AI

**原文链接**: [https://www.washingtonpost.com/technology/2026/11/03/google-deepmind-staff-protest-lifetime-ban-criticizing-company/](https://www.washingtonpost.com/technology/2026/11/03/google-deepmind-staff-protest-lifetime-ban-criticizing-company/)

生成摘要时出错

---

## 74. Show HN: I built a tool that prices a pre-built PC part by part

**原文标题**: Show HN: I built a tool that prices a pre-built PC part by part

**原文链接**: [https://pcdealcheck.com/](https://pcdealcheck.com/)

生成摘要时出错

---

## 75. Conductor is joining Meta

**原文标题**: Conductor is joining Meta

**原文链接**: [https://www.conductor.build/announcement](https://www.conductor.build/announcement)

生成摘要时出错

---

## 76. Qualcomm Cloud AI 100 Ultra – 150W AI Accelerator Card with 128GB at 548GB/s

**原文标题**: Qualcomm Cloud AI 100 Ultra – 150W AI Accelerator Card with 128GB at 548GB/s

**原文链接**: [https://www.qualcomm.com/data-center/products/cloud-ai-100-ultra](https://www.qualcomm.com/data-center/products/cloud-ai-100-ultra)

生成摘要时出错

---

## 77. Introduction to Programming in ATS

**原文标题**: Introduction to Programming in ATS

**原文链接**: [https://ats-lang.sourceforge.net/DOCUMENT/INT2PROGINATS/HTML/book1.html](https://ats-lang.sourceforge.net/DOCUMENT/INT2PROGINATS/HTML/book1.html)

生成摘要时出错

---

## 78. Anthropic IPO filing: $1.7B quarterly payroll, about $107K per employee monthly

**原文标题**: Anthropic IPO filing: $1.7B quarterly payroll, about $107K per employee monthly

**原文链接**: [https://www.techspot.com/news/114428-anthropic-ipo-filing-reveals-17-billion-quarterly-personnel.html](https://www.techspot.com/news/114428-anthropic-ipo-filing-reveals-17-billion-quarterly-personnel.html)

生成摘要时出错

---

## 79. Too Expensive to Exist

**原文标题**: Too Expensive to Exist

**原文链接**: [https://mapwriting.substack.com/p/too-expensive-to-exist](https://mapwriting.substack.com/p/too-expensive-to-exist)

生成摘要时出错

---

## 80. Democrats Rout GOP

**原文标题**: Democrats Rout GOP

**原文链接**: [https://www.nytimes.com/live/2026/11/03/us/midterms-2026-election-day-trump](https://www.nytimes.com/live/2026/11/03/us/midterms-2026-election-day-trump)

生成摘要时出错

---

## 81. Hackers hit French national blood bank

**原文标题**: Hackers hit French national blood bank

**原文链接**: [https://www.telegraph.co.uk/world-news/2026/11/04/hackers-hit-french-blood-bank/](https://www.telegraph.co.uk/world-news/2026/11/04/hackers-hit-french-blood-bank/)

生成摘要时出错

---

## 82. Milkman – The Better Alternative to Postman

**原文标题**: Milkman – The Better Alternative to Postman

**原文链接**: [https://milkman.dev/](https://milkman.dev/)

生成摘要时出错

---

## 83. Arrows to arrows, categories to queries (2025)

**原文标题**: Arrows to arrows, categories to queries (2025)

**原文链接**: [https://reasonablypolymorphic.com/blog/arrows-to-arrows/](https://reasonablypolymorphic.com/blog/arrows-to-arrows/)

生成摘要时出错

---

## 84. The AI Boom May Be Sowing Seeds of Another Financial Crisis

**原文标题**: The AI Boom May Be Sowing Seeds of Another Financial Crisis

**原文链接**: [https://www.bloomberg.com/opinion/articles/2026-11-03/ai-investment-boom-demands-stronger-financial-oversight](https://www.bloomberg.com/opinion/articles/2026-11-03/ai-investment-boom-demands-stronger-financial-oversight)

生成摘要时出错

---

## 85. Snapchat Is Harming Children at an Industrial Scale (2025)

**原文标题**: Snapchat Is Harming Children at an Industrial Scale (2025)

**原文链接**: [https://www.afterbabel.com/p/industrial-scale-snapchat](https://www.afterbabel.com/p/industrial-scale-snapchat)

生成摘要时出错

---

## 86. Cloudflare experiencing multiple active incidents

**原文标题**: Cloudflare experiencing multiple active incidents

**原文链接**: [https://www.cloudflarestatus.com/](https://www.cloudflarestatus.com/)

生成摘要时出错

---

## 87. A map of 5000+ midterm ads

**原文标题**: A map of 5000+ midterm ads

**原文链接**: [https://admap.org/](https://admap.org/)

生成摘要时出错

---

## 88. Tiny Basic for Arduino

**原文标题**: Tiny Basic for Arduino

**原文链接**: [https://dilshan.github.io/tiny-basic/](https://dilshan.github.io/tiny-basic/)

生成摘要时出错

---

## 89. Apple opens the door to a nightmare world of always-listening tech

**原文标题**: Apple opens the door to a nightmare world of always-listening tech

**原文链接**: [https://this.weekinsecurity.com/watch-what-you-say-apple-opens-the-door-to-a-nightmare-world-of-always-listening-tech/](https://this.weekinsecurity.com/watch-what-you-say-apple-opens-the-door-to-a-nightmare-world-of-always-listening-tech/)

生成摘要时出错

---

## 90. Show HN: HackerChurn – which SaaS tools HN wants to cancel

**原文标题**: Show HN: HackerChurn – which SaaS tools HN wants to cancel

**原文链接**: [https://hissingkitty.com/hacker-churn](https://hissingkitty.com/hacker-churn)

生成摘要时出错

---

## 91. Show HN: I built a little browser game to practice Vim commands

**原文标题**: Show HN: I built a little browser game to practice Vim commands

**原文链接**: [https://hjkl.duy.run](https://hjkl.duy.run)

生成摘要时出错

---

## 92. Handles are the better pointers (2018)

**原文标题**: Handles are the better pointers (2018)

**原文链接**: [https://floooh.github.io/2018/06/17/handles-vs-pointers.html](https://floooh.github.io/2018/06/17/handles-vs-pointers.html)

生成摘要时出错

---

## 93. The AI Bubble Monitor

**原文标题**: The AI Bubble Monitor

**原文链接**: [https://cepr.net/publications/ai-bubble-monitor/](https://cepr.net/publications/ai-bubble-monitor/)

生成摘要时出错

---

## 94. No Vehicles in the Park

**原文标题**: No Vehicles in the Park

**原文链接**: [https://novehiclesinthepark.com/](https://novehiclesinthepark.com/)

生成摘要时出错

---

## 95. Pratt parsing is a black box

**原文标题**: Pratt parsing is a black box

**原文链接**: [https://vinipsmaker.github.io/blog/article/pratt-parsing-is-a-black-box/](https://vinipsmaker.github.io/blog/article/pratt-parsing-is-a-black-box/)

生成摘要时出错

---

## 96. Proton Colleagues, Unionize Now

**原文标题**: Proton Colleagues, Unionize Now

**原文链接**: [https://molecule.build/](https://molecule.build/)

生成摘要时出错

---

## 97. $20M in Fines and Vizio Smart TVs Opt Out of Spying Option Does Nothing

**原文标题**: $20M in Fines and Vizio Smart TVs Opt Out of Spying Option Does Nothing

**原文链接**: [https://pcper.com/2026/11/20-million-in-fines-and-still-vizio-smart-tvs-opt-out-of-spying-option-does-nothing/](https://pcper.com/2026/11/20-million-in-fines-and-still-vizio-smart-tvs-opt-out-of-spying-option-does-nothing/)

生成摘要时出错

---

## 98. AI data centers comprehensively defeated at US midterm elections

**原文标题**: AI data centers comprehensively defeated at US midterm elections

**原文链接**: [https://www.tomshardware.com/tech-industry/data-centers/ai-data-centers-comprehensively-defeated-at-us-midterm-elections-45-measures-put-on-the-ballot-as-americans-overwhelmingly-vote-against-developments](https://www.tomshardware.com/tech-industry/data-centers/ai-data-centers-comprehensively-defeated-at-us-midterm-elections-45-measures-put-on-the-ballot-as-americans-overwhelmingly-vote-against-developments)

生成摘要时出错

---

## 99. Octomind – open-source AI harness that saves your tokens, static rust

**原文标题**: Octomind – open-source AI harness that saves your tokens, static rust

**原文链接**: [https://github.com/Muvon/octomind](https://github.com/Muvon/octomind)

生成摘要时出错

---

## 100. One of Google's Android partners turned 1.3M set-top boxes into a botnet

**原文标题**: One of Google's Android partners turned 1.3M set-top boxes into a botnet

**原文链接**: [https://www.theverge.com/1024807/google-botnet-android-tv-shut-down](https://www.theverge.com/1024807/google-botnet-android-tv-shut-down)

生成摘要时出错

---

