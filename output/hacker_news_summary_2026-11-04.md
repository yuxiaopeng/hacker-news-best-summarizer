# Hacker News 热门文章摘要 (2026-11-04)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. Astra可以读写权重以改进Qwen

**原文标题**: Astra can read and write weights to improve Qwen

**原文链接**: [https://rikiyat.github.io/blog/weight-space-programming/](https://rikiyat.github.io/blog/weight-space-programming/)

本研究介绍了“权重空间编程”，证明了前沿大型语言模型（如GPT-6 Astra）能够直接原生读写神经网络权重。这种范式允许LLM在不依赖传统优化器或训练循环的情况下，通过自然语言目标来推理和修改权重。

本研究提出了几项开创性发现：
1.  **读取权重：** Astra成功识别了PPO网络所训练的游戏、扩散模型生成的形状，甚至仅凭原始权重，就识别出语言模型中间层中的语言和特定的“复制头”（归纳头）。
2.  **修复权重：** Astra通过编辑其3.5%的权重，诊断并修复了一个失败的斜坡汽车策略，将成功率从0%提升至100%。至关重要的是，它通过识别和修复推理循环，仅以极小的（0.016%）权重修改，就提升了Qwen3.5-0.8B的数学表现（MATH-500上从7.9%到48.1%）和指令遵循能力。
3.  **写入权重：** Astra为MinAtar游戏从零开始编写了小型游戏策略网络，其性能超越了经过PPO训练1亿步的策略。

这些壮举是在没有允许Astra编写训练循环或使用梯度下降的情况下完成的，突显了其直接理解和修改底层计算的能力。作者认为，这种“权重空间编程”可能会彻底改变深度学习的优化和可解释性。

---

## 2. 乌班图搞什么鬼？

**原文标题**: WTF Ubuntu?

**原文链接**: [https://chalmovsky.com/posts/wtf-ubuntu](https://chalmovsky.com/posts/wtf-ubuntu)

作者对Ubuntu未能修复一个关键的Linux内核TCP漏洞（CVE-2026-98432，CVSS 9.8）表示极度不满。这个自2016年就存在的漏洞允许远程root访问，并且一个可用的漏洞利用程序已被演示。

尽管Debian已于10月16日修复了该漏洞，但截至2026年11月2日，Ubuntu仍未为其任何受支持版本（包括LTS版本）发布补丁。作者指出，鉴于此次延迟，尤其是在该漏洞被评为关键级九天后、root利用被证实六天后，Ubuntu关于“及时补丁”和“企业级”安全的市场营销承诺显得空洞。

此次延迟导致作者彻底失去了对Ubuntu的信任，促使其决定将所有服务器从该平台迁移出去，并被迫将现有Ubuntu服务器下线。作者进一步批评Canonical这家销售安全订阅服务的公司，竟然落后于Debian、Arch和Alpine等由志愿者运营的发行版，而这些发行版早已提供了修复。

---

## 3. Postman 静默自动安装AI插件并试图共享所有API数据。

**原文标题**: Postman silently auto-installs AI plugins and attempts to share all API data

**原文链接**: [https://github.com/postmanlabs/postman-app-support/issues/14370](https://github.com/postmanlabs/postman-app-support/issues/14370)

生成摘要时出错

---

## 4. 《Astra 可以读写权重来改进 Qwen》一文具有误导性。

**原文标题**: The 'Astra can read and write weights to improve Qwen' post is misleading

**原文链接**: [https://honnibal.dev/blog/astra-read-write-misleading](https://honnibal.dev/blog/astra-read-write-misleading)

这篇文章批评了题为“Astra可以读写权重以改进通义千问”的帖子具有误导性。文章指出，该摘要错误地暗示Astra在所有实验中，特别是针对其标题中强调的通义千问改进，都使用了一种单一的、深层能力——“仅仅通过查看原始权重”。

作者澄清，只有少数在小型网络（1.7万至17.2万个权重）上进行的实验（1、2、4）才真正涉及直接解释原始权重。相比之下，重要的通义千问实验以及其他涉及更大模型或编写游戏对弈网络的实验，并未依赖这种“原始权重”方法。相反，这些任务涉及Astra编写Python程序，而针对通义千问的实验，则是让模型运行多达50批次的练习问题，以分析和修改权重。

文章认为，通义千问的结果表明Astra具备执行类似于人类机器学习工程师设计和执行基于代码的解决方案的任务能力，这令人印象深刻，但与直接理解原始权重有着根本性的区别。作者指出，将这些截然不同的方法——直接权重检查与基于代码的分析/修改并结合模型执行——表现得如同它们源于单一技术，会制造出一种对网络权重拥有统一“格式塔”式理解的错误印象。

---

## 5. If you love a website, back it up

**原文标题**: If you love a website, back it up

**原文链接**: [https://blog.mistys-internet.website/post/2026/10/29/if-you-love-a-website-back-it-up/](https://blog.mistys-internet.website/post/2026/10/29/if-you-love-a-website-back-it-up/)

The author, a web archiving professional, recounts the loss of a beloved fansite, teapuppies.com, which suddenly disappeared and was replaced by gambling ads. This personal tragedy highlights the ephemeral nature of the web and serves as a call to action: individuals can and should proactively back up their favorite websites, rather than waiting for large organizations to do it.

The article explains that personal web archiving is accessible using standard formats like WARC/WACZ. Three main tools, developed by the author's company (mostly free), are recommended:
1.  **ArchiveWeb.page browser extension (Chrome):** The easiest option for single pages or small sites, allowing users to capture what they see in their browser.
2.  **archiveweb.page app:** A standalone application with a built-in browser, offering similar functionality without needing a browser extension.
3.  **Browsertrix:** An automated web crawler suitable for archiving entire large websites or comprehensive social media profiles. It's primarily a web app with a paid per-use model (after a trial), though it's open source.

Once archived, content can be viewed locally using the tools, or shared by sending the WACZ file to others who can use the ArchiveWeb.page app or ReplayWeb.page website. For public display, the ReplayWeb.page embedded viewer can be integrated into any webpage. The author emphasizes that WACZ files are easy to secure and share, promoting collective preservation. The goal is to empower individuals to preserve the digital content that matters to them.

---

## 6. Ubuntu 仍未发布 Linux 0day RCE 补丁，已近三周。

**原文标题**: Ubuntu still has not released patch for Linux 0day RCE in almost 3 weeks

**原文链接**: [https://freenode.net/article/ubuntu-lts-kernels-still-unfixed-for-critical-cve-2026-98432](https://freenode.net/article/ubuntu-lts-kernels-still-unfixed-for-critical-cve-2026-98432)

Ubuntu 尚未发布针对一个关键的 Linux 0day RCE 漏洞 CVE-2026-98432 的补丁，距离该漏洞披露已近三周。该漏洞影响 Ubuntu 的长期支持 (LTS) 内核，特别是 22.04、24.04 和 26.04 版本，其 CVSS 评分高达 9.8，属于严重级别。

这种延迟使得依赖 Ubuntu LTS 内核提供安全和隔离的面向互联网的多租户自托管系统，面临潜在的远程或本地攻击风险。由于缺乏官方供应商更新，管理员无法获取已打补丁的内核软件包来修补这个安全漏洞。

Ubuntu 尚未提供必要修复的预计发布时间（ETA）。这种情况迫使受影响的管理员面临选择：要么在未打补丁的系统上继续运行，要么在可行的情况下实施非官方的树外缓解措施，要么将其工作负载迁移到已解决此漏洞的其他发行版或内核。

---

## 7. 为了调个时间，我竟然给我的车载导航系统越狱了。

**原文标题**: Jailbreaking my car's navigation system just so I can change the time

**原文链接**: [https://blog.nns.ee/2026/11/02/renault-hack/](https://blog.nns.ee/2026/11/02/renault-hack/)

作者遇到一个令人困惑的问题，他们2014年的雷诺纬度（Renault Latitude）在夏令时转换后无法更改汽车时钟。TomTom Carminat LIVE导航单元神秘地缺少了“设置时间”选项。后来发现，访问这个关键设置需要一张特定的、受DRM保护的导航SD卡，而前车主已经将其丢弃，更换一张大约需要60欧元。

作者决心避免这笔开销，于是踏上了一段越狱之旅。对该单元的固件和更新文件进行逆向工程，并建立QEMU模拟器，证实了SD卡的必要性，因为菜单定义都是从SD卡加载的。首次尝试刷入修改后的固件失败了，原因是不明验证，而且大多数文件系统都被挂载为只读或`noexec`，阻止了直接的代码执行。

突破是通过结合两个漏洞实现的：一个`master.script`命令（`LOG`）允许通过目录遍历将任意ASCII写入任何文件路径，而另一个命令（`SHEX`）可以在没有参数的情况下执行现有的rootfs二进制文件。受到内核漏洞利用的启发，作者使用`LOG`将一个shell脚本payload（`|/bin/sh /media/sdcard/payload.sh`）写入`/proc/sys/kernel/core_pattern`。接着，使用`SHEX`执行`/bin/dbus-monitor`，该程序如预期般崩溃，触发了核心转储，并以root权限执行了payload脚本。

获得root权限后，作者创建了完整的eMMC备份。进一步的逆向工程显示，时间偏移量存储在`/mnt/flash/settings.dat`中。将值从180分钟更改为120分钟后，汽车的时钟终于被纠正了。

---

## 8. Google will turn off search for schools that reject AI

**原文标题**: Google will turn off search for schools that reject AI

**原文链接**: [https://www.nytimes.com/2026/11/03/us/google-search-schools-restrict-ai.html](https://www.nytimes.com/2026/11/03/us/google-search-schools-restrict-ai.html)

Unable to access the article link.

---

## 9. OccupySaaS

**原文标题**: OccupySaaS

**原文链接**: [https://occupysaas.com/](https://occupysaas.com/)

生成摘要时出错

---

## 10. US boy names that became girl names and vice versa

**原文标题**: US boy names that became girl names and vice versa

**原文链接**: [https://namedaisy.com/blog/boy-names-that-became-girl-names](https://namedaisy.com/blog/boy-names-that-became-girl-names)

生成摘要时出错

---

## 11. Qwen 3.8 27B on my laptop can interpret model weights, too

**原文标题**: Qwen 3.8 27B on my laptop can interpret model weights, too

**原文链接**: [https://simonwillison.net/2026/Nov/3/qwen-can-interpret-model-weights/](https://simonwillison.net/2026/Nov/3/qwen-can-interpret-model-weights/)

生成摘要时出错

---

## 12. Show HN: Hacker Times, a New York Times-inspired version of Hacker News

**原文标题**: Show HN: Hacker Times, a New York Times-inspired version of Hacker News

**原文链接**: [https://hackertimes.ca/](https://hackertimes.ca/)

生成摘要时出错

---

## 13. Kalshi and its co-founders face felony charges for violating Utah gambling laws

**原文标题**: Kalshi and its co-founders face felony charges for violating Utah gambling laws

**原文链接**: [https://arstechnica.com/tech-policy/2026/10/trump-admin-sues-utah-to-save-kalshi-from-the-states-total-ban-on-gambling/](https://arstechnica.com/tech-policy/2026/10/trump-admin-sues-utah-to-save-kalshi-from-the-states-total-ban-on-gambling/)

生成摘要时出错

---

## 14. Could a modern chess engine on a Pentium have defeated Kasparov in 1996?

**原文标题**: Could a modern chess engine on a Pentium have defeated Kasparov in 1996?

**原文链接**: [https://nicholas.carlini.com/writing/2026/algorithmic-improvements-chess.html](https://nicholas.carlini.com/writing/2026/algorithmic-improvements-chess.html)

生成摘要时出错

---

## 15. Supermarket freezers across Europe hit by second suspected cyber-attack

**原文标题**: Supermarket freezers across Europe hit by second suspected cyber-attack

**原文链接**: [https://www.theguardian.com/world/2026/nov/02/supermarket-freezers-across-europe-hit-by-second-suspected-cyber-attack](https://www.theguardian.com/world/2026/nov/02/supermarket-freezers-across-europe-hit-by-second-suspected-cyber-attack)

生成摘要时出错

---

## 16. The SEC Should Block Anthropic's IPO to Protect the Public

**原文标题**: The SEC Should Block Anthropic's IPO to Protect the Public

**原文链接**: [https://www.techpolicy.press/the-sec-should-block-anthropics-ipo-to-protect-the-public/](https://www.techpolicy.press/the-sec-should-block-anthropics-ipo-to-protect-the-public/)

生成摘要时出错

---

## 17. Fujifilm to boost tape production 5x as AI fuels archiving demand

**原文标题**: Fujifilm to boost tape production 5x as AI fuels archiving demand

**原文链接**: [https://arstechnica.com/gadgets/2026/10/fujifilm-to-boost-tape-production-5x-as-ai-fuels-archiving-demand/](https://arstechnica.com/gadgets/2026/10/fujifilm-to-boost-tape-production-5x-as-ai-fuels-archiving-demand/)

生成摘要时出错

---

## 18. U.S. workers took home their smallest share of capital since at least 1947

**原文标题**: U.S. workers took home their smallest share of capital since at least 1947

**原文链接**: [https://fortune.com/article/why-did-us-workers-just-take-home-smallest-share-of-capital-since-1947-lowest-ever-recorded/](https://fortune.com/article/why-did-us-workers-just-take-home-smallest-share-of-capital-since-1947-lowest-ever-recorded/)

生成摘要时出错

---

## 19. Anthropic's internal AI use, at retail prices, now exceeds its employee pay

**原文标题**: Anthropic's internal AI use, at retail prices, now exceeds its employee pay

**原文链接**: [https://www.businessinsider.com/anthropic-claude-internal-ai-use-exceeds-employee-pay-tokens-2026-11](https://www.businessinsider.com/anthropic-claude-internal-ai-use-exceeds-employee-pay-tokens-2026-11)

生成摘要时出错

---

## 20. DiscImageStudio: burn visible artwork onto CDs, DVDs and Blu-ray discs

**原文标题**: DiscImageStudio: burn visible artwork onto CDs, DVDs and Blu-ray discs

**原文链接**: [https://github.com/JiaFeiMiao-K-Cat/DiscImageStudio](https://github.com/JiaFeiMiao-K-Cat/DiscImageStudio)

生成摘要时出错

---

## 21. Show HN: Wikihack – HackerTube, but for Wikipedia articles mentioned on HN

**原文标题**: Show HN: Wikihack – HackerTube, but for Wikipedia articles mentioned on HN

**原文链接**: [https://wikihack.netlify.app](https://wikihack.netlify.app)

生成摘要时出错

---

## 22. Bones may release proteins that slow aging and extend life span

**原文标题**: Bones may release proteins that slow aging and extend life span

**原文链接**: [https://www.science.org/content/article/bones-may-release-proteins-slow-aging-and-extend-life-span](https://www.science.org/content/article/bones-may-release-proteins-slow-aging-and-extend-life-span)

生成摘要时出错

---

## 23. Stringman, an $800 open-source room scale gripper robot

**原文标题**: Stringman, an $800 open-source room scale gripper robot

**原文链接**: [https://neufangled.com/](https://neufangled.com/)

生成摘要时出错

---

## 24. Self-Employed? Solopreneur? NIST Has a Cybersecurity Guide Just for You

**原文标题**: Self-Employed? Solopreneur? NIST Has a Cybersecurity Guide Just for You

**原文链接**: [https://www.nist.gov/news-events/news/2026/11/self-employed-solopreneur-nist-has-cybersecurity-guide-just-you](https://www.nist.gov/news-events/news/2026/11/self-employed-solopreneur-nist-has-cybersecurity-guide-just-you)

生成摘要时出错

---

## 25. Show HN: Warsaw in voxels – An interactive 3D map of the city centre

**原文标题**: Show HN: Warsaw in voxels – An interactive 3D map of the city centre

**原文链接**: [https://p.migdal.pl/warsaw-vibe-voxel/](https://p.migdal.pl/warsaw-vibe-voxel/)

生成摘要时出错

---

## 26. Mac at Any Scale

**原文标题**: Mac at Any Scale

**原文链接**: [https://namespace.so/blog/mac-at-any-scale](https://namespace.so/blog/mac-at-any-scale)

生成摘要时出错

---

## 27. BYD sold more EVs last month than the US did all quarter

**原文标题**: BYD sold more EVs last month than the US did all quarter

**原文链接**: [https://electrek.co/2026/11/02/byd-sold-more-evs-last-month-than-the-us-did-all-quarter/](https://electrek.co/2026/11/02/byd-sold-more-evs-last-month-than-the-us-did-all-quarter/)

生成摘要时出错

---

## 28. Scaling Git at OpenAI

**原文标题**: Scaling Git at OpenAI

**原文链接**: [https://openai.com/index/scaling-git-at-openai/](https://openai.com/index/scaling-git-at-openai/)

生成摘要时出错

---

## 29. Nvidia – open-source auto-ontology

**原文标题**: Nvidia – open-source auto-ontology

**原文链接**: [https://github.com/NVIDIA/auto-ontology](https://github.com/NVIDIA/auto-ontology)

生成摘要时出错

---

## 30. Study estimates 75% of NFL players who died over 15-year span had CTE

**原文标题**: Study estimates 75% of NFL players who died over 15-year span had CTE

**原文链接**: [https://www.nbcnews.com/health/health-news/study-estimates-75-nfl-players-died-15-year-span-may-cte-rcna605975](https://www.nbcnews.com/health/health-news/study-estimates-75-nfl-players-died-15-year-span-may-cte-rcna605975)

生成摘要时出错

---

## 31. Anthropic reports $17B in Q3 revenue, commitments of $895B in revised S-1

**原文标题**: Anthropic reports $17B in Q3 revenue, commitments of $895B in revised S-1

**原文链接**: [https://www.cnbc.com/2026/11/02/anthropic-ant-s-1-quarter-financials.html](https://www.cnbc.com/2026/11/02/anthropic-ant-s-1-quarter-financials.html)

生成摘要时出错

---

## 32. Show HN: I've updated my Linux System Call website and API

**原文标题**: Show HN: I've updated my Linux System Call website and API

**原文链接**: [https://syscall.sh/](https://syscall.sh/)

生成摘要时出错

---

## 33. Anthropic's growth just flattened

**原文标题**: Anthropic's growth just flattened

**原文链接**: [https://www.regenerator1.com/p/anthropics-growth-just-flattened](https://www.regenerator1.com/p/anthropics-growth-just-flattened)

生成摘要时出错

---

## 34. Intel stock collapse worsens as $3.5T chip rout spreads

**原文标题**: Intel stock collapse worsens as $3.5T chip rout spreads

**原文链接**: [https://finance.yahoo.com/markets/article/the-intel-stock-collapse-is-getting-worse--and-the-37-trillion-chip-rout-is-spreading-212154947.html](https://finance.yahoo.com/markets/article/the-intel-stock-collapse-is-getting-worse--and-the-37-trillion-chip-rout-is-spreading-212154947.html)

生成摘要时出错

---

## 35. F/OSS Comics #13: BSD Unix, Part 3 – The Beginning of BSD Unix

**原文标题**: F/OSS Comics #13: BSD Unix, Part 3 – The Beginning of BSD Unix

**原文链接**: [https://fosscomics.com/posts/13.%20BSD%20Unix%20Part%203%20-%20The%20Beginning%20of%20BSD%20Unix/](https://fosscomics.com/posts/13.%20BSD%20Unix%20Part%203%20-%20The%20Beginning%20of%20BSD%20Unix/)

生成摘要时出错

---

## 36. Safari introduces Adaptive Dark Mode in 27.3

**原文标题**: Safari introduces Adaptive Dark Mode in 27.3

**原文链接**: [https://webkit.org/blog/18541/introducing-adaptive-dark-mode/](https://webkit.org/blog/18541/introducing-adaptive-dark-mode/)

生成摘要时出错

---

## 37. My Favourite Laptop

**原文标题**: My Favourite Laptop

**原文链接**: [https://blog.jsbarretto.com/post/laptop](https://blog.jsbarretto.com/post/laptop)

生成摘要时出错

---

## 38. Net worth for people aged 30–33 in the U.S.

**原文标题**: Net worth for people aged 30–33 in the U.S.

**原文链接**: [https://www.keepingup.com/benchmarks/net-worth/age-30-33](https://www.keepingup.com/benchmarks/net-worth/age-30-33)

生成摘要时出错

---

## 39. Oracle files to sell $20B in new stock, bonds to finance AI buildout

**原文标题**: Oracle files to sell $20B in new stock, bonds to finance AI buildout

**原文链接**: [https://www.cnbc.com/2026/11/02/oracle-files-to-sell-20-billion-in-new-stock-bonds-to-finance-ai-buildout.html](https://www.cnbc.com/2026/11/02/oracle-files-to-sell-20-billion-in-new-stock-bonds-to-finance-ai-buildout.html)

生成摘要时出错

---

## 40. European RISC-V Industrial Computing Initiative

**原文标题**: European RISC-V Industrial Computing Initiative

**原文链接**: [https://erici.eu](https://erici.eu)

生成摘要时出错

---

## 41. We halved DNS build delay and cut memory use by 85%

**原文标题**: We halved DNS build delay and cut memory use by 85%

**原文链接**: [https://blog.cloudflare.com/dns-targeted-zone-builds/](https://blog.cloudflare.com/dns-targeted-zone-builds/)

生成摘要时出错

---

## 42. Let Me Ch...

**原文标题**: Let Me Ch...

**原文链接**: [https://blog.alxgsv.com/let-me-check/](https://blog.alxgsv.com/let-me-check/)

生成摘要时出错

---

## 43. Jobless tech workers are being left out of San Francisco's AI boom

**原文标题**: Jobless tech workers are being left out of San Francisco's AI boom

**原文链接**: [https://www.bloomberg.com/news/features/2026-09-17/san-francisco-s-ai-wealth-boom-skirts-engineers-as-openai-anthropic-ipos-near](https://www.bloomberg.com/news/features/2026-09-17/san-francisco-s-ai-wealth-boom-skirts-engineers-as-openai-anthropic-ipos-near)

生成摘要时出错

---

## 44. Revolut moves to self-hosted GLM

**原文标题**: Revolut moves to self-hosted GLM

**原文链接**: [https://twitter.com/guilleflorvs/status/2117379073785696395](https://twitter.com/guilleflorvs/status/2117379073785696395)

生成摘要时出错

---

## 45. Moving our warehouse off DuckDB

**原文标题**: Moving our warehouse off DuckDB

**原文链接**: [https://posthog.com/blog/moving-off-duckdb](https://posthog.com/blog/moving-off-duckdb)

生成摘要时出错

---

## 46. Why are Soviet math textbooks so hardcore in comparison to US textbooks? (2017)

**原文标题**: Why are Soviet math textbooks so hardcore in comparison to US textbooks? (2017)

**原文链接**: [https://www.quora.com/Why-are-Soviet-mathematics-physics-textbooks-so-insanely-hardcore-in-comparison-to-US-textbooks/answer/Scott-Miller-307?share=1](https://www.quora.com/Why-are-Soviet-mathematics-physics-textbooks-so-insanely-hardcore-in-comparison-to-US-textbooks/answer/Scott-Miller-307?share=1)

生成摘要时出错

---

## 47. Show HN: HackerHack – HackerBooks but for Posts Posted on HN

**原文标题**: Show HN: HackerHack – HackerBooks but for Posts Posted on HN

**原文链接**: [https://news.ycombinator.com/](https://news.ycombinator.com/)

生成摘要时出错

---

## 48. Egoless Mathematics in the AI Era

**原文标题**: Egoless Mathematics in the AI Era

**原文链接**: [https://terrytao.wordpress.com/2026/11/02/egoless-mathematics-in-the-ai-era/](https://terrytao.wordpress.com/2026/11/02/egoless-mathematics-in-the-ai-era/)

生成摘要时出错

---

## 49. Never Complain, Never Explain

**原文标题**: Never Complain, Never Explain

**原文链接**: [https://en.wikipedia.org/wiki/Never_complain,_never_explain](https://en.wikipedia.org/wiki/Never_complain,_never_explain)

生成摘要时出错

---

## 50. Just a little AI resistance, as a treat

**原文标题**: Just a little AI resistance, as a treat

**原文链接**: [https://shkspr.mobi/blog/2026/11/just-a-little-ai-resistance-as-a-treat/](https://shkspr.mobi/blog/2026/11/just-a-little-ai-resistance-as-a-treat/)

生成摘要时出错

---

## 51. Trigger.dev customer environment variables exposed

**原文标题**: Trigger.dev customer environment variables exposed

**原文链接**: [https://trigger.dev/blog/security-incident-nov-2026](https://trigger.dev/blog/security-incident-nov-2026)

生成摘要时出错

---

## 52. Preparing for the Flipper One Kickstarter and opening pre-orders

**原文标题**: Preparing for the Flipper One Kickstarter and opening pre-orders

**原文链接**: [https://flipper.net/pages/flipper-one](https://flipper.net/pages/flipper-one)

生成摘要时出错

---

## 53. Launch HN: Momentic (YC W24) – Agents that catch bugs by using your app

**原文标题**: Launch HN: Momentic (YC W24) – Agents that catch bugs by using your app

**原文链接**: [https://momentic.ai/](https://momentic.ai/)

生成摘要时出错

---

## 54. China's First Frontier AI Export Controls: Mofcom Announcement No. 48

**原文标题**: China's First Frontier AI Export Controls: Mofcom Announcement No. 48

**原文链接**: [https://labs.cloudsecurityalliance.org/research/csa-research-note-china-ai-export-controls-announcement-48-2/](https://labs.cloudsecurityalliance.org/research/csa-research-note-china-ai-export-controls-announcement-48-2/)

生成摘要时出错

---

## 55. Polyend releases the Tracker firmware source code

**原文标题**: Polyend releases the Tracker firmware source code

**原文链接**: [https://polyend.com/whats-up/tracker-the-biggest-update-yet/](https://polyend.com/whats-up/tracker-the-biggest-update-yet/)

生成摘要时出错

---

## 56. The Little Book of Generative AI Foundations: An Intuitive Mathematical Primer

**原文标题**: The Little Book of Generative AI Foundations: An Intuitive Mathematical Primer

**原文链接**: [https://arxiv.org/abs/2605.29713](https://arxiv.org/abs/2605.29713)

生成摘要时出错

---

## 57. Sneaking into the auditorium for the Windows 2000 launch rehearsal

**原文标题**: Sneaking into the auditorium for the Windows 2000 launch rehearsal

**原文链接**: [https://devblogs.microsoft.com/oldnewthing/20261102-00/?p=112818/](https://devblogs.microsoft.com/oldnewthing/20261102-00/?p=112818/)

生成摘要时出错

---

## 58. Katamari Damacy but it's The Met collection

**原文标题**: Katamari Damacy but it's The Met collection

**原文链接**: [https://katamari.vaguespac.es/](https://katamari.vaguespac.es/)

生成摘要时出错

---

## 59. The Megadonors Who Have Poured $1.2B into the Midterms

**原文标题**: The Megadonors Who Have Poured $1.2B into the Midterms

**原文链接**: [https://www.nytimes.com/interactive/2026/08/28/us/politics/billionaire-midterms-donors.html](https://www.nytimes.com/interactive/2026/08/28/us/politics/billionaire-midterms-donors.html)

生成摘要时出错

---

## 60. Last night an AI agent performed brain surgery on a mouse

**原文标题**: Last night an AI agent performed brain surgery on a mouse

**原文链接**: [https://twitter.com/OcanaSantero/status/2115442964574908902](https://twitter.com/OcanaSantero/status/2115442964574908902)

生成摘要时出错

---

## 61. LLMs are not superhuman at reading and writing neural network weights

**原文标题**: LLMs are not superhuman at reading and writing neural network weights

**原文链接**: [https://www.seangoedecke.com/llms-are-not-superhuman-at-reading-and-writing-neural-network-weights/](https://www.seangoedecke.com/llms-are-not-superhuman-at-reading-and-writing-neural-network-weights/)

生成摘要时出错

---

## 62. BioWare co-founder: game execs "have never made a game" and don't get it

**原文标题**: BioWare co-founder: game execs "have never made a game" and don't get it

**原文链接**: [https://www.pcgamer.com/gaming-industry/none-of-these-people-have-ever-made-a-game-bioware-co-founder-greg-zeschuk-says-of-game-industry-executives-they-just-dont-know-how-it-works/](https://www.pcgamer.com/gaming-industry/none-of-these-people-have-ever-made-a-game-bioware-co-founder-greg-zeschuk-says-of-game-industry-executives-they-just-dont-know-how-it-works/)

生成摘要时出错

---

## 63. I dumped Apple’s word list

**原文标题**: I dumped Apple’s word list

**原文链接**: [https://helgesver.re/articles/macos-vulgar-word-flags](https://helgesver.re/articles/macos-vulgar-word-flags)

生成摘要时出错

---

## 64. uBlock Origin filter to block autoplay videos in TechCrunch

**原文标题**: uBlock Origin filter to block autoplay videos in TechCrunch

**原文链接**: [https://cornfieldlabs.github.io/posts/ublock-stop-techcrunch-autoplay-video/post.html](https://cornfieldlabs.github.io/posts/ublock-stop-techcrunch-autoplay-video/post.html)

生成摘要时出错

---

## 65. Sam Altman: All the RAM Should Belong to Me, So I Can Charge People to Use It

**原文标题**: Sam Altman: All the RAM Should Belong to Me, So I Can Charge People to Use It

**原文链接**: [https://gizmodo.com/sam-altman-all-the-ram-should-belong-to-me-so-i-can-charge-people-to-use-it-2000833412](https://gizmodo.com/sam-altman-all-the-ram-should-belong-to-me-so-i-can-charge-people-to-use-it-2000833412)

生成摘要时出错

---

## 66. Show HN: HackerTV – HN's most-recommended Youtube videos as 24/7 TV channels

**原文标题**: Show HN: HackerTV – HN's most-recommended Youtube videos as 24/7 TV channels

**原文链接**: [https://hackertv.org](https://hackertv.org)

生成摘要时出错

---

## 67. The U.S. Census Bureau and "Super Intelligence"

**原文标题**: The U.S. Census Bureau and "Super Intelligence"

**原文链接**: [https://simonwillison.net/2026/Nov/2/census-bureau-super-intelligence/](https://simonwillison.net/2026/Nov/2/census-bureau-super-intelligence/)

生成摘要时出错

---

## 68. US tech giants' hidden AI debt swells 90% to $3.2T in 6 months

**原文标题**: US tech giants' hidden AI debt swells 90% to $3.2T in 6 months

**原文链接**: [https://asia.nikkei.com/business/technology/artificial-intelligence/us-tech-giants-hidden-ai-debt-swells-90-to-3.2tn-in-6-months](https://asia.nikkei.com/business/technology/artificial-intelligence/us-tech-giants-hidden-ai-debt-swells-90-to-3.2tn-in-6-months)

生成摘要时出错

---

## 69. Why Don't We Live in an Art Nouveau World?

**原文标题**: Why Don't We Live in an Art Nouveau World?

**原文链接**: [https://asteriskmag.com/issues/16/why-don-t-we-life-in-an-art-nouveau-world](https://asteriskmag.com/issues/16/why-don-t-we-life-in-an-art-nouveau-world)

生成摘要时出错

---

## 70. AI is destroying my CS degree

**原文标题**: AI is destroying my CS degree

**原文链接**: [https://lordtoots.bearblog.dev/ai-is-destroying-my-cs-degree/](https://lordtoots.bearblog.dev/ai-is-destroying-my-cs-degree/)

生成摘要时出错

---

## 71. Skill to Create Product Videos

**原文标题**: Skill to Create Product Videos

**原文链接**: [https://github.com/aaitor/skill-video-studio](https://github.com/aaitor/skill-video-studio)

生成摘要时出错

---

## 72. Ballot Rejections Have Soared in Rural Counties as USPS Reduces Mail Service

**原文标题**: Ballot Rejections Have Soared in Rural Counties as USPS Reduces Mail Service

**原文链接**: [https://www.propublica.org/article/mail-ballot-delays-postal-service-midterms](https://www.propublica.org/article/mail-ballot-delays-postal-service-midterms)

生成摘要时出错

---

## 73. Writing seen in PHerc. 306B, for the first time in 2000 years

**原文标题**: Writing seen in PHerc. 306B, for the first time in 2000 years

**原文链接**: [https://scrollprize.substack.com/p/writing-seen-in-pherc-306b-for-the](https://scrollprize.substack.com/p/writing-seen-in-pherc-306b-for-the)

生成摘要时出错

---

## 74. Agentic backdoors via pretraining poisoning

**原文标题**: Agentic backdoors via pretraining poisoning

**原文链接**: [https://arxiv.org/abs/2610.37741](https://arxiv.org/abs/2610.37741)

生成摘要时出错

---

## 75. Supermarket freezers in Belgium and Sweden hit by suspected cyber-attack

**原文标题**: Supermarket freezers in Belgium and Sweden hit by suspected cyber-attack

**原文链接**: [https://www.bbc.com/news/articles/cq1kd1nee80eo](https://www.bbc.com/news/articles/cq1kd1nee80eo)

生成摘要时出错

---

## 76. SLAC researchers find proof of altermagnetism, a new magnetic phase

**原文标题**: SLAC researchers find proof of altermagnetism, a new magnetic phase

**原文链接**: [https://www6.slac.stanford.edu/news/2026-10-29-slac-researchers-find-proof-altermagnetism-new-magnetic-phase](https://www6.slac.stanford.edu/news/2026-10-29-slac-researchers-find-proof-altermagnetism-new-magnetic-phase)

生成摘要时出错

---

## 77. Claude Opus 5.5 Can Draw Permit-Level Architectural Drawings

**原文标题**: Claude Opus 5.5 Can Draw Permit-Level Architectural Drawings

**原文链接**: [https://stephenjgallagher.substack.com/p/ai-can-draw-blueprints-now](https://stephenjgallagher.substack.com/p/ai-can-draw-blueprints-now)

生成摘要时出错

---

## 78. Charles Tandy, the mastermind behind Radio Shack

**原文标题**: Charles Tandy, the mastermind behind Radio Shack

**原文链接**: [https://dfarq.homeip.net/charles-tandy-the-mastermind-behind-radio-shack/](https://dfarq.homeip.net/charles-tandy-the-mastermind-behind-radio-shack/)

生成摘要时出错

---

## 79. AI fan wikis riddled with errors are muddying the waters of games culture

**原文标题**: AI fan wikis riddled with errors are muddying the waters of games culture

**原文链接**: [https://www.eurogamer.net/ai-fan-wikis-errors-complicating-games-culture](https://www.eurogamer.net/ai-fan-wikis-errors-complicating-games-culture)

生成摘要时出错

---

## 80. Antimony: CAD Software Evolved from Lisp Machines and Not Drafting Tables (2015)

**原文标题**: Antimony: CAD Software Evolved from Lisp Machines and Not Drafting Tables (2015)

**原文链接**: [https://www.mattkeeter.com/projects/antimony/3/](https://www.mattkeeter.com/projects/antimony/3/)

生成摘要时出错

---

## 81. Bear turns 10, and it still feels like day one

**原文标题**: Bear turns 10, and it still feels like day one

**原文链接**: [https://blog.bear.app/2026/11/bear-turns-10-and-it-still-feels-like-day-one/](https://blog.bear.app/2026/11/bear-turns-10-and-it-still-feels-like-day-one/)

生成摘要时出错

---

## 82. Quili AI

**原文标题**: Quili AI

**原文链接**: [https://www.quili.ai/](https://www.quili.ai/)

生成摘要时出错

---

## 83. Apple reports fourth quarter results

**原文标题**: Apple reports fourth quarter results

**原文链接**: [https://www.apple.com/newsroom/2026/11/apple-reports-fourth-quarter-results/](https://www.apple.com/newsroom/2026/11/apple-reports-fourth-quarter-results/)

生成摘要时出错

---

## 84. LongCat-2.5: Native Multimodality for Agentic Tasks

**原文标题**: LongCat-2.5: Native Multimodality for Agentic Tasks

**原文链接**: [https://longcat.ai/blog/longcat-2.5/](https://longcat.ai/blog/longcat-2.5/)

生成摘要时出错

---

## 85. macOS 27 does not support CoreStorage volumes

**原文标题**: macOS 27 does not support CoreStorage volumes

**原文链接**: [https://wadetregaskis.com/macos-27-golden-gate-does-not-actually-support-corestorage-or-hfs-volumes/](https://wadetregaskis.com/macos-27-golden-gate-does-not-actually-support-corestorage-or-hfs-volumes/)

生成摘要时出错

---

## 86. C64 Basic Dungeon Crawler: Stairs, Levels and Levelling Up (Part 11)

**原文标题**: C64 Basic Dungeon Crawler: Stairs, Levels and Levelling Up (Part 11)

**原文链接**: [https://retrogamecoders.com/c64-basic-dungeon-part11/](https://retrogamecoders.com/c64-basic-dungeon-part11/)

生成摘要时出错

---

## 87. Too Expensive to Exist

**原文标题**: Too Expensive to Exist

**原文链接**: [https://mapwriting.substack.com/p/too-expensive-to-exist](https://mapwriting.substack.com/p/too-expensive-to-exist)

生成摘要时出错

---

## 88. Google researchers demand freedom to tell the world what they know about AI

**原文标题**: Google researchers demand freedom to tell the world what they know about AI

**原文链接**: [https://www.washingtonpost.com/technology/2026/11/03/google-deepmind-staff-protest-lifetime-ban-criticizing-company/](https://www.washingtonpost.com/technology/2026/11/03/google-deepmind-staff-protest-lifetime-ban-criticizing-company/)

生成摘要时出错

---

## 89. Japan's Jimi 'Mundane' Halloween Costumes of 2026

**原文标题**: Japan's Jimi 'Mundane' Halloween Costumes of 2026

**原文链接**: [https://spoon-tamago.com/japan-jimi-mundane-halloween-costumes-2026/](https://spoon-tamago.com/japan-jimi-mundane-halloween-costumes-2026/)

生成摘要时出错

---

## 90. Anthropic IPO filing: $1.7B quarterly payroll, about $107K per employee monthly

**原文标题**: Anthropic IPO filing: $1.7B quarterly payroll, about $107K per employee monthly

**原文链接**: [https://www.techspot.com/news/114428-anthropic-ipo-filing-reveals-17-billion-quarterly-personnel.html](https://www.techspot.com/news/114428-anthropic-ipo-filing-reveals-17-billion-quarterly-personnel.html)

生成摘要时出错

---

## 91. Binance hackers used fake job interview to breach PC before $6.3B attack

**原文标题**: Binance hackers used fake job interview to breach PC before $6.3B attack

**原文链接**: [https://www.reuters.com/world/binance-says-hackers-used-fake-job-interview-compromise-computer-before-63-2026-11-03/](https://www.reuters.com/world/binance-says-hackers-used-fake-job-interview-compromise-computer-before-63-2026-11-03/)

生成摘要时出错

---

## 92. Cloudflare experiencing multiple active incidents

**原文标题**: Cloudflare experiencing multiple active incidents

**原文链接**: [https://www.cloudflarestatus.com/](https://www.cloudflarestatus.com/)

生成摘要时出错

---

## 93. Anthropic reveals $900B AI spending commitments ahead of IPO

**原文标题**: Anthropic reveals $900B AI spending commitments ahead of IPO

**原文链接**: [https://www.ft.com/content/4d91dbab-6fe4-45ab-beee-d77e091cb37f](https://www.ft.com/content/4d91dbab-6fe4-45ab-beee-d77e091cb37f)

生成摘要时出错

---

## 94. Practice speaking Japanese with real YouTube videos, graded line by line

**原文标题**: Practice speaking Japanese with real YouTube videos, graded line by line

**原文链接**: [https://jivx.com/yt](https://jivx.com/yt)

生成摘要时出错

---

## 95. The future in old computer magazines (1984–2004)

**原文标题**: The future in old computer magazines (1984–2004)

**原文链接**: [https://tomorrowasusual.substack.com/p/blast-from-the-past-the-future-in](https://tomorrowasusual.substack.com/p/blast-from-the-past-the-future-in)

生成摘要时出错

---

## 96. GPT-Rosalind-6 System Card Addendum

**原文标题**: GPT-Rosalind-6 System Card Addendum

**原文链接**: [https://deploymentsafety.openai.com/gpt-rosalind-6](https://deploymentsafety.openai.com/gpt-rosalind-6)

生成摘要时出错

---

## 97. Show HN: HackerChurn – which SaaS tools HN wants to cancel

**原文标题**: Show HN: HackerChurn – which SaaS tools HN wants to cancel

**原文链接**: [https://hissingkitty.com/hacker-churn](https://hissingkitty.com/hacker-churn)

生成摘要时出错

---

## 98. Pray for Chaos

**原文标题**: Pray for Chaos

**原文链接**: [https://geohot.github.io//blog/jekyll/update/2026/11/01/pray-for-chaos.html](https://geohot.github.io//blog/jekyll/update/2026/11/01/pray-for-chaos.html)

生成摘要时出错

---

## 99. How I use AI (Oct 2026)

**原文标题**: How I use AI (Oct 2026)

**原文链接**: [https://ben.stolovitz.com/posts/how-use-ai-oct-2026/](https://ben.stolovitz.com/posts/how-use-ai-oct-2026/)

生成摘要时出错

---

## 100. No Vehicles in the Park

**原文标题**: No Vehicles in the Park

**原文链接**: [https://novehiclesinthepark.com/](https://novehiclesinthepark.com/)

生成摘要时出错

---

