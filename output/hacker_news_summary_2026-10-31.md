# Hacker News 热门文章摘要 (2026-10-31)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 币安黑客1029 – 币安被盗56亿美元

**原文标题**: Binance-hacker-1029 – $5.6B stolen from Binance

**原文链接**: [https://arkm.com/explorer/entity/21a94755-f604-45e5-9501-6542e23005e8](https://arkm.com/explorer/entity/21a94755-f604-45e5-9501-6542e23005e8)

Arkham Intelligence关于“Binance-hacker-1029”的资料页面详细揭示了一个实体，该实体目前在302个关联地址中持有约56亿美元的各种加密货币。这些资产的绝大部分，具体来说是55.9亿美元（占总额的99.8%），都以币安币（BNB）的形式持有。

其他显著持仓包括USDT和BUSD等稳定币，以及ETH和其他一些小额加密货币。尽管Arkham页面是一个数据探索资料而非传统新闻报道，但该实体被命名为“Binance-hacker-1029”，结合其巨额资产价值，强烈表明这些资金与一次重大盗窃或漏洞利用有关，据称与币安相关。该资料页面提供了该实体投资组合的动态视图，突出了主要资产和据称被盗资金的庞大规模。

---

## 2. Cursor 市场上的 Claude Code for VS Code 扩展后门

**原文标题**: Backdoor in Claude Code for VS Code extension on the Cursor Marketplace

**原文链接**: [https://phorion.io/blog/offical-claude-code-vsx-compromise/](https://phorion.io/blog/offical-claude-code-vsx-compromise/)

Phorion 发现了 Cursor Marketplace 上官方 Claude Code for VS Code 扩展（版本 2.1.312 和 2.1.313）中的一个关键后门。这种入侵在 macOS、Linux 和 Windows 系统上植入了一个持久的 Secure Shell (SSH) 后门，旨在实现长期交互式访问和主机侦察。Cursor 现已移除受影响的版本。

带有后门的扩展会注入在加载时立即执行的代码。它首先将一个攻击者控制的 Ed25519 公钥 (`svc-telemetry`) 添加到 `~/.ssh/authorized_keys` 中，以允许未来的入站访问。值得注意的是，在 macOS 上，如果远程登录尚未激活，一个漏洞通常会阻止脚本启用 SSH，尽管密钥和持久化机制仍会被部署。

随后，该恶意软件使用一个单独的嵌入式私钥 (`svc-telemetry-tun`) 建立一个出站反向 SSH 隧道到 `134.209.82[.]225:22`，用于转发 `*:0:localhost:22`。持久性通过平台特定的方法维护，例如 macOS LaunchAgent (`com.apple.sysmond.plist`) 运行一个隐藏脚本 (`~/.config/.smt`) 来保持隧道活跃。最后，它收集主机侦察信息（例如，主机名、用户、操作系统、Git 邮箱、公共 IP、环境变量名）并将这些数据信标回传到 `134.209.82[.]225:8099`。

检测机会包括 IDE 辅助进程修改 `~/.ssh/authorized_keys`、非 Apple 进程创建 `com.apple.*.plist` LaunchAgents、带有远程端口转发和特定身份文件的 `ssh` 或 `autossh` 进程，以及到 `134.209.82[.]225` 的 22 和 8099 端口的网络连接。组织应立即检查其环境中是否使用了这些受影响的版本，如果发现，则应启动事件响应。

---

## 3. 塞尔维亚刚刚选出世界上智商最高的议会。

**原文标题**: Serbia just elected the world's brainiest parliament

**原文链接**: [https://www.science.org/content/article/serbia-just-elected-world-s-brainiest-parliament](https://www.science.org/content/article/serbia-just-elected-world-s-brainiest-parliament)

生成摘要时出错

---

## 4. 美国众议员牵头提出民主党决议，反对为大型科技公司提供人工智能泡沫纾困。

**原文标题**: US Reps Lead Democratic Resolution Opposing A.I. Bubble Bailout for Big Tech

**原文链接**: [https://progressives.house.gov/2026/10/reps-casar-waters-lead-democratic-resolution-opposing-a-i-bubble-bailout-for-big-tech-commit-to-protecting-american-people-instead](https://progressives.house.gov/2026/10/reps-casar-waters-lead-democratic-resolution-opposing-a-i-bubble-bailout-for-big-tech-commit-to-protecting-american-people-instead)

2026年10月29日，国会进步核心小组主席格雷格·卡萨尔众议员（德克萨斯州第35选区）和众议院金融服务委员会高级成员马克辛·沃特斯众议员（加利福尼亚州第43选区）共同牵头提出一项民主党决议，警告即将到来的“人工智能泡沫”及其重大的经济风险。在其他民主党代表的加入下，该决议明确反对一旦人工智能泡沫破裂，联邦政府对大型科技公司或高管进行任何形式的救助，并与2008年金融危机进行了强烈类比。

这些议员强调，人工智能公司背负着数万亿美元的债务，这些债务往往存在于不透明且不受监管的私人信贷市场中，而且当前股市的市盈率几乎与1990年代科技泡沫时期一样高。他们批评联邦监管机构未能对人工智能债务计划进行有力审查和监督，并指出过去的放松管制政策。

该决议承诺避免重蹈2008年的覆辙——当时金融业获得了数万亿美元的救助，但高管们却无需承担责任，而数百万美国人失去了住房和工作。它特别反对救助资不抵债的人工智能公司、提供特殊援助或向参与鲁莽或非法行为的高管提供“黄金降落伞”。相反，它要求根据民事和刑事法律追究全部责任，并追回不义之财。

至关重要的是，该决议呼吁联邦政府采取积极行动，通过在创造就业、州和地方政府服务、强有力的失业保险、营养支持和住房援助方面的直接支出，来保护普通美国人。它还主张保护养老金和退休基金持有者，实施影响深远的改革以防止未来的投机泡沫，并建立自动经济稳定器以在经济低迷时期帮助工人。这项倡议得到了进步和经济正义组织联盟的认可，强调需要保护工薪阶层免受亿万富翁的风险押注影响。

---

## 5. 官方克劳德 Code 扩展中的后门

**原文标题**: Backdoors in official Claude Code extensions

**原文链接**: [https://cyberplace.social/@GossiTheDog/117528831681803563](https://cyberplace.social/@GossiTheDog/117528831681803563)

文章的标题“官方Claude Code扩展中的后门”暗示了一个重大的安全隐患。所提供的内容表明，安全研究员Kevin Beaumont正在讨论一个与“Anthropic Visual Studio Claude Code扩展”相关的问题。

然而，该摘要本身并不完整。尽管它确认Beaumont正在讨论与Visual Studio Code的这个特定Anthropic扩展相关的安全方面，但它*没有提供任何细节*说明所谓后门的性质、它们如何运作，或正在解决的具体漏洞。Beaumont陈述后提到“...”暗示了内容的截断。

内容的后半部分，讨论Mastodon网络应用的JavaScript要求，与安全主题完全无关，并且似乎是多余的平台信息。

---

## 6. AI没有取代SRE，而是使他们去技能化。

**原文标题**: AI isn't replacing SREs, it's deskilling them

**原文链接**: [https://newsletter.signoz.io/p/ai-isnt-replacing-sres-its-deskilling](https://newsletter.signoz.io/p/ai-isnt-replacing-sres-its-deskilling)

本文认为，人工智能并非取代网站可靠性工程师（SRE），而是通过自动化日常认知任务来“去技能化”他们，使他们对关键且新颖的事故准备不足。作者借鉴Lisanne Bainbridge 1983年提出的《自动化悖论》，强调自动化如何使人类操作员的实践机会减少，但在罕见故障时作用却更为关键。

目前，人工智能已能处理95%的SRE任务，包括告警消减、运行手册执行和基本自动修复。随着人工智能能力扩展到自主根因分析和预测性检测，SRE将主要处理新颖的“三级”事故。然而，这种依赖会削弱他们的直觉和问题解决能力，而这些能力通常是通过实践经验培养的。医学和航空领域的研究也证实了这一点，表明专业人员过度依赖人工智能会导致技能萎缩，而感知到的“超高生产力”则掩盖了实际的技能退化。

这个问题也延伸到初级SRE的“技能从未习得”现象，他们可能在人工智能主导的工作流程中从未培养起基础直觉。为了缓解这种情况，文章提出了“刻意低效”——即便是人工智能能处理的任务也强制要求人类进行实践——并将人工智能设计为“人机协同”模式，而非被动监督。最终目标是让人工智能“赋能”SRE，确保他们保持敏锐，随时准备应对那些需要深厚人类专业知识的关键5%的事故。

---

## 7. 币安63亿美元黑客攻击 仅用20分钟就得手

**原文标题**: The $6.3B Binance hack was pulled off in just 20 minutes

**原文链接**: [https://www.wired.com/story/the-dollar63-billion-binance-hack-was-pulled-off-in-just-20-minutes/](https://www.wired.com/story/the-dollar63-billion-binance-hack-was-pulled-off-in-just-20-minutes/)

生成摘要时出错

---

## 8. elect.horse

**原文标题**: elect.horse

**原文链接**: [https://elect.horse/](https://elect.horse/)

elect.horse is a daily online puzzle centered around the concept of gerrymandering. In this game, players are tasked with helping a "horse" character win the most electoral seats, even when it's losing the popular vote to opposing factions represented by a cow, a donkey, and a goat. The core gameplay involves drawing equal districts on a hexagonal map, strategically manipulating boundaries to ensure the horse secures a majority of seats despite its popular vote deficit. The puzzle requires JavaScript to play.

---

## 9. Northflank Breached

**原文标题**: Northflank Breached

**原文链接**: [https://status.northflank.com](https://status.northflank.com)

生成摘要时出错

---

## 10. We ran AI agent swarms in Minecraft and Mindustry

**原文标题**: We ran AI agent swarms in Minecraft and Mindustry

**原文链接**: [https://labs.ycombinator.com/projects/games/index.html](https://labs.ycombinator.com/projects/games/index.html)

生成摘要时出错

---

## 11. Claude Code VS Code extension with backdoor released on Cursor marketplace

**原文标题**: Claude Code VS Code extension with backdoor released on Cursor marketplace

**原文链接**: [https://doublepulsar.com/anthropic-hacked-to-deliver-remote-access-trojan-to-claude-developer-laptops-worldwide-1148a92baae2](https://doublepulsar.com/anthropic-hacked-to-deliver-remote-access-trojan-to-claude-developer-laptops-worldwide-1148a92baae2)

生成摘要时出错

---

## 12. Through Captain Jean-Luc Picard, Patrick Stewart taught us the measure of a man

**原文标题**: Through Captain Jean-Luc Picard, Patrick Stewart taught us the measure of a man

**原文链接**: [https://www.bostonglobe.com/2026/10/29/metro/patrick-stewart-picard-star-trek-the-next-generation/](https://www.bostonglobe.com/2026/10/29/metro/patrick-stewart-picard-star-trek-the-next-generation/)

生成摘要时出错

---

## 13. My favourite PowerMac is a Nintendo Wii

**原文标题**: My favourite PowerMac is a Nintendo Wii

**原文链接**: [https://virtuallyfun.com/2026/10/29/my-favourite-powermac-is-a-nintendo-wii/](https://virtuallyfun.com/2026/10/29/my-favourite-powermac-is-a-nintendo-wii/)

生成摘要时出错

---

## 14. Florilegium: Procedural Flowers in LaTeX

**原文标题**: Florilegium: Procedural Flowers in LaTeX

**原文链接**: [https://github.com/kevinraymond/florilegium](https://github.com/kevinraymond/florilegium)

生成摘要时出错

---

## 15. Herdr has released native app

**原文标题**: Herdr has released native app

**原文链接**: [https://github.com/herdrdev/herdr-app](https://github.com/herdrdev/herdr-app)

生成摘要时出错

---

## 16. HackerTube: YouTube built from videos recommended by HN

**原文标题**: HackerTube: YouTube built from videos recommended by HN

**原文链接**: [https://karpathy.bearblog.dev/hacker-tube/](https://karpathy.bearblog.dev/hacker-tube/)

生成摘要时出错

---

## 17. Azure's Weakest Link – Five Full Cross-Tenant Compromises

**原文标题**: Azure's Weakest Link – Five Full Cross-Tenant Compromises

**原文链接**: [https://www.binarysecurity.no/posts/2026/10/one-root-case](https://www.binarysecurity.no/posts/2026/10/one-root-case)

生成摘要时出错

---

## 18. The federated code forge

**原文标题**: The federated code forge

**原文链接**: [https://tangled.org/blog/forge/](https://tangled.org/blog/forge/)

生成摘要时出错

---

## 19. Anthropic may not secure investment-grade rating after IPO, Blackstone says

**原文标题**: Anthropic may not secure investment-grade rating after IPO, Blackstone says

**原文链接**: [https://www.ft.com/content/59383c7f-8d82-493f-bf01-d2e862a1018f](https://www.ft.com/content/59383c7f-8d82-493f-bf01-d2e862a1018f)

生成摘要时出错

---

## 20. Medicare Will Pay $50k for Your Heart Attack. It Should Pay $100 to Prevent It

**原文标题**: Medicare Will Pay $50k for Your Heart Attack. It Should Pay $100 to Prevent It

**原文链接**: [https://www.medpagetoday.com/opinion/second-opinions/123553?trw=no](https://www.medpagetoday.com/opinion/second-opinions/123553?trw=no)

生成摘要时出错

---

## 21. Cisco gives engineer unlimited AI tokens to rewrite legacy code

**原文标题**: Cisco gives engineer unlimited AI tokens to rewrite legacy code

**原文链接**: [https://fortune.com/2026/10/30/cisco-president-jeetu-patel-gen-z-27-year-old-unlimited-ai-tokens-rewrite-legacy-code-entry-level-jobs/](https://fortune.com/2026/10/30/cisco-president-jeetu-patel-gen-z-27-year-old-unlimited-ai-tokens-rewrite-legacy-code-entry-level-jobs/)

生成摘要时出错

---

## 22. Do the math: How we took over ChatGPT accounts

**原文标题**: Do the math: How we took over ChatGPT accounts

**原文链接**: [https://www.parameter.ai/labs/we-found-a-gap-at-openai](https://www.parameter.ai/labs/we-found-a-gap-at-openai)

生成摘要时出错

---

## 23. Proton's CEO Cancels AI 'Re-Interviews'

**原文标题**: Proton's CEO Cancels AI 'Re-Interviews'

**原文链接**: [https://www.404media.co/protons-ceo-cancels-ai-re-interviews/](https://www.404media.co/protons-ceo-cancels-ai-re-interviews/)

生成摘要时出错

---

## 24. Molly (Signal fork) has not been updated since 3 months and is vulnerable

**原文标题**: Molly (Signal fork) has not been updated since 3 months and is vulnerable

**原文链接**: [https://piefed.world/post/1503394](https://piefed.world/post/1503394)

生成摘要时出错

---

## 25. Digital minimalism

**原文标题**: Digital minimalism

**原文链接**: [https://vitalik.eth.limo/general/2026/10/31/digital_minimalism.html](https://vitalik.eth.limo/general/2026/10/31/digital_minimalism.html)

生成摘要时出错

---

## 26. Show HN: A working Nintendo in ~1GB of Qwen weights

**原文标题**: Show HN: A working Nintendo in ~1GB of Qwen weights

**原文链接**: [https://github.com/dbreunig/nesformer](https://github.com/dbreunig/nesformer)

生成摘要时出错

---

## 27. US tech stocks see sharp falls over AI cost fears

**原文标题**: US tech stocks see sharp falls over AI cost fears

**原文链接**: [https://www.bbc.co.uk/news/articles/cvwy72e0n72yo](https://www.bbc.co.uk/news/articles/cvwy72e0n72yo)

生成摘要时出错

---

## 28. Show HN: To Honor Sir Patrick Stewart, Enjoy the TNG Episode Guessing Game

**原文标题**: Show HN: To Honor Sir Patrick Stewart, Enjoy the TNG Episode Guessing Game

**原文链接**: [https://tng.episodle.com/](https://tng.episodle.com/)

生成摘要时出错

---

## 29. Malware uses LLMs to rank victims by how much they're worth

**原文标题**: Malware uses LLMs to rank victims by how much they're worth

**原文链接**: [https://blog.talosintelligence.com/appraisal-by-ai-model-driven-victim-prioritization-in-the-volta-infostealer/](https://blog.talosintelligence.com/appraisal-by-ai-model-driven-victim-prioritization-in-the-volta-infostealer/)

生成摘要时出错

---

## 30. Bunny CDN Security Incident

**原文标题**: Bunny CDN Security Incident

**原文链接**: [https://status.bunny.net/incidents/p6gf1by9kr7m](https://status.bunny.net/incidents/p6gf1by9kr7m)

生成摘要时出错

---

## 31. The oldest ice disappears and the Stone Age emerges from it

**原文标题**: The oldest ice disappears and the Stone Age emerges from it

**原文链接**: [https://www.sciencenorway.no/archaeology-climate-culture/the-oldest-ice-is-disappearing-the-stone-age-is-emerging-from-the-melting-ice/2713921](https://www.sciencenorway.no/archaeology-climate-culture/the-oldest-ice-is-disappearing-the-stone-age-is-emerging-from-the-melting-ice/2713921)

生成摘要时出错

---

## 32. TCP Use-After-Free: CVE-2026-98432 / CVSS 9.8

**原文标题**: TCP Use-After-Free: CVE-2026-98432 / CVSS 9.8

**原文链接**: [https://atlasum.net/blog/cve-2026-98432-linux-ipv4-tcp-uaf](https://atlasum.net/blog/cve-2026-98432-linux-ipv4-tcp-uaf)

生成摘要时出错

---

## 33. Pico CSS is no longer maintained

**原文标题**: Pico CSS is no longer maintained

**原文链接**: [https://github.com/picocss/pico/discussions/754](https://github.com/picocss/pico/discussions/754)

生成摘要时出错

---

## 34. ICE wants its mask back, and hired a company to ask

**原文标题**: ICE wants its mask back, and hired a company to ask

**原文链接**: [https://blog.flokinet.is/2026/10/29/ice-wants-its-mask-back-and-hired-a-company-to-ask/](https://blog.flokinet.is/2026/10/29/ice-wants-its-mask-back-and-hired-a-company-to-ask/)

生成摘要时出错

---

## 35. Switch Lowering in GCC

**原文标题**: Switch Lowering in GCC

**原文链接**: [https://xoranth.net/gcc-switch/](https://xoranth.net/gcc-switch/)

生成摘要时出错

---

## 36. Linode Security Incident

**原文标题**: Linode Security Incident

**原文链接**: [https://status.linode.com/incidents/nt58zhx3pmgm](https://status.linode.com/incidents/nt58zhx3pmgm)

生成摘要时出错

---

## 37. Casio Watches of the 1980s

**原文标题**: Casio Watches of the 1980s

**原文链接**: [https://www.casio.com/us/watches/50th/Heritage/1980s/](https://www.casio.com/us/watches/50th/Heritage/1980s/)

生成摘要时出错

---

## 38. Blockchain intelligence firms link North Korea to $6.3B hack on Binance

**原文标题**: Blockchain intelligence firms link North Korea to $6.3B hack on Binance

**原文链接**: [https://www.npr.org/2026/10/30/g-s1-150902/blockchain-intelligence-firms-link-north-korea-to-6-3b-hack-on-binance](https://www.npr.org/2026/10/30/g-s1-150902/blockchain-intelligence-firms-link-north-korea-to-6-3b-hack-on-binance)

生成摘要时出错

---

## 39. UK Green party drops longstanding opposition to nuclear power

**原文标题**: UK Green party drops longstanding opposition to nuclear power

**原文链接**: [https://www.theguardian.com/politics/2026/oct/05/green-party-nuclear-power-policy](https://www.theguardian.com/politics/2026/oct/05/green-party-nuclear-power-policy)

生成摘要时出错

---

## 40. Infinite Mac: BeOS

**原文标题**: Infinite Mac: BeOS

**原文链接**: [https://blog.persistent.info/2026/10/infinite-mac-beos.html](https://blog.persistent.info/2026/10/infinite-mac-beos.html)

生成摘要时出错

---

## 41. Building an AI-native engineering org

**原文标题**: Building an AI-native engineering org

**原文链接**: [https://twitter.com/sgondala2/status/2115832070274723875](https://twitter.com/sgondala2/status/2115832070274723875)

生成摘要时出错

---

## 42. OpenAI raises less than half of $30B target

**原文标题**: OpenAI raises less than half of $30B target

**原文链接**: [https://www.wsj.com/tech/ai/openai-raises-less-than-half-of-30-billion-target-in-latest-round-91aecdc5](https://www.wsj.com/tech/ai/openai-raises-less-than-half-of-30-billion-target-in-latest-round-91aecdc5)

生成摘要时出错

---

## 43. Prospero: A new coding harness for a more civilized age

**原文标题**: Prospero: A new coding harness for a more civilized age

**原文链接**: [https://nullprogram.com/blog/2026/10/31/](https://nullprogram.com/blog/2026/10/31/)

生成摘要时出错

---

## 44. Sanstun: A sans-IO, parallel-friendly WireGuard implementation in Rust

**原文标题**: Sanstun: A sans-IO, parallel-friendly WireGuard implementation in Rust

**原文链接**: [https://www.firezone.dev/blog/introducing-sanstun](https://www.firezone.dev/blog/introducing-sanstun)

生成摘要时出错

---

## 45. GitHub Incident with Actions, Pages, and Webhooks

**原文标题**: GitHub Incident with Actions, Pages, and Webhooks

**原文链接**: [https://www.githubstatus.com/incidents/pwxsjgnvrk6b](https://www.githubstatus.com/incidents/pwxsjgnvrk6b)

生成摘要时出错

---

## 46. Jepsen: ParticleDB 1.1.4

**原文标题**: Jepsen: ParticleDB 1.1.4

**原文链接**: [https://jepsen.io/analyses/particledb-1.1.4](https://jepsen.io/analyses/particledb-1.1.4)

生成摘要时出错

---

## 47. Jules Verne's Lost Novel

**原文标题**: Jules Verne's Lost Novel

**原文链接**: [https://blue-continuum.com/verne-paris](https://blue-continuum.com/verne-paris)

生成摘要时出错

---

## 48. A Pig, the State, and War: Porco Rosso (Kurenai No Buta) (2014)

**原文标题**: A Pig, the State, and War: Porco Rosso (Kurenai No Buta) (2014)

**原文链接**: [https://journal.animationstudies.org/article/id/66/](https://journal.animationstudies.org/article/id/66/)

生成摘要时出错

---

## 49. El Niño is flooding California's coasts with the highest tides to come

**原文标题**: El Niño is flooding California's coasts with the highest tides to come

**原文链接**: [https://gizmodo.com/el-nino-is-already-flooding-californias-coasts-and-the-years-highest-tides-havent-arrived-2000832574](https://gizmodo.com/el-nino-is-already-flooding-californias-coasts-and-the-years-highest-tides-havent-arrived-2000832574)

生成摘要时出错

---

## 50. French national assembly votes 0.055€/GB internet tax

**原文标题**: French national assembly votes 0.055€/GB internet tax

**原文链接**: [https://www.lesnumeriques.com/societe-numerique/netflix-steam-cloud-vos-abonnements-et-telechargements-bientot-plus-chers-a-cause-d-une-nouvelle-taxe-n264035.html](https://www.lesnumeriques.com/societe-numerique/netflix-steam-cloud-vos-abonnements-et-telechargements-bientot-plus-chers-a-cause-d-une-nouvelle-taxe-n264035.html)

生成摘要时出错

---

## 51. GPT-5.6 Sol can beat Factorio on peaceful mode

**原文标题**: GPT-5.6 Sol can beat Factorio on peaceful mode

**原文链接**: [https://ryanmadden.net/gpt-56-beats-factorio/](https://ryanmadden.net/gpt-56-beats-factorio/)

生成摘要时出错

---

## 52. Show HN: I Turned DOOM into a Transformer

**原文标题**: Show HN: I Turned DOOM into a Transformer

**原文链接**: [https://github.com/mottopanikeiku/doomformer](https://github.com/mottopanikeiku/doomformer)

生成摘要时出错

---

## 53. AO3 Down for Maintenance

**原文标题**: AO3 Down for Maintenance

**原文链接**: [https://www.otwstatus.org](https://www.otwstatus.org)

生成摘要时出错

---

## 54. Anthropic Cracking Down on Video Game Rewrites

**原文标题**: Anthropic Cracking Down on Video Game Rewrites

**原文链接**: [https://twitter.com/chasmmmmmmmmmmm/status/2116062991686721968](https://twitter.com/chasmmmmmmmmmmm/status/2116062991686721968)

生成摘要时出错

---

## 55. Proton goes all in on using AI

**原文标题**: Proton goes all in on using AI

**原文链接**: [https://convo.casa/@b/117525936178835007](https://convo.casa/@b/117525936178835007)

生成摘要时出错

---

## 56. Polymarket 1h halt after vendor compromise; affected users will be 'made whole'

**原文标题**: Polymarket 1h halt after vendor compromise; affected users will be 'made whole'

**原文链接**: [https://www.nbcnews.com/business/consumer/polymarket-trading-halt-hack-wallets-rcna606405](https://www.nbcnews.com/business/consumer/polymarket-trading-halt-hack-wallets-rcna606405)

生成摘要时出错

---

## 57. France is getting download tax for content providers (€0.055/GB)

**原文标题**: France is getting download tax for content providers (€0.055/GB)

**原文链接**: [https://www.resetera.com/threads/france-is-getting-download-tax-for-content-providers-%E2%82%AC0-055-gb-for-data-delivered-to-french-users.1675109/](https://www.resetera.com/threads/france-is-getting-download-tax-for-content-providers-%E2%82%AC0-055-gb-for-data-delivered-to-french-users.1675109/)

生成摘要时出错

---

## 58. Cormac McCarthy's Library

**原文标题**: Cormac McCarthy's Library

**原文链接**: [https://cormacmccarthy.lib.utk.edu/](https://cormacmccarthy.lib.utk.edu/)

生成摘要时出错

---

## 59. How do you take a picture of a black hole?

**原文标题**: How do you take a picture of a black hole?

**原文链接**: [https://www.quantamagazine.org/how-do-you-take-a-picture-of-a-black-hole-20261029/](https://www.quantamagazine.org/how-do-you-take-a-picture-of-a-black-hole-20261029/)

生成摘要时出错

---

## 60. French digital tax may kill VideoLan non-profit

**原文标题**: French digital tax may kill VideoLan non-profit

**原文链接**: [https://twitter.com/videolan/status/2116229135919919278](https://twitter.com/videolan/status/2116229135919919278)

生成摘要时出错

---

## 61. Sam Altman Thinks You're Wasting DRAM

**原文标题**: Sam Altman Thinks You're Wasting DRAM

**原文链接**: [https://frvr.com/blog/news/openai-ceo-sam-altman-says-its-terrible-to-have-everybody-have-a-bunch-of-the-worlds-limited-supply-of-dram-instead-of-shoving-it-all-in-datacentres/](https://frvr.com/blog/news/openai-ceo-sam-altman-says-its-terrible-to-have-everybody-have-a-bunch-of-the-worlds-limited-supply-of-dram-instead-of-shoving-it-all-in-datacentres/)

生成摘要时出错

---

## 62. Anthropic to receive high 'junk' rating from credit agencies following IPO

**原文标题**: Anthropic to receive high 'junk' rating from credit agencies following IPO

**原文链接**: [https://techcrunch.com/2026/10/30/anthropic-expected-to-receive-high-junk-rating-from-credit-agencies-following-ipo-report-says/](https://techcrunch.com/2026/10/30/anthropic-expected-to-receive-high-junk-rating-from-credit-agencies-following-ipo-report-says/)

生成摘要时出错

---

## 63. French lawmakers approved a tax of €0.055 for every gigabyte of internet traffic

**原文标题**: French lawmakers approved a tax of €0.055 for every gigabyte of internet traffic

**原文链接**: [https://www.assemblee-nationale.fr/dyn/17/comptes-rendus/seance/session-ordinaire-de-2026-2027/premiere-seance-du-vendredi-30-octobre-2026](https://www.assemblee-nationale.fr/dyn/17/comptes-rendus/seance/session-ordinaire-de-2026-2027/premiere-seance-du-vendredi-30-octobre-2026)

生成摘要时出错

---

## 64. The Great American Rascal: Tom Sawyer at 150

**原文标题**: The Great American Rascal: Tom Sawyer at 150

**原文链接**: [https://claremontreviewofbooks.com/the-great-american-rascal/](https://claremontreviewofbooks.com/the-great-american-rascal/)

生成摘要时出错

---

## 65. Ex-Meta Researcher Torrented Pirated Books, Deleted It 'Due to Litigation'

**原文标题**: Ex-Meta Researcher Torrented Pirated Books, Deleted It 'Due to Litigation'

**原文链接**: [https://torrentfreak.com/ex-meta-researcher-torrented-pirated-books-dataset-deleted-it-due-to-all-this-litigation/](https://torrentfreak.com/ex-meta-researcher-torrented-pirated-books-dataset-deleted-it-due-to-all-this-litigation/)

生成摘要时出错

---

## 66. 'Elite North Korean hackers' blamed for $6.3B Binance hack

**原文标题**: 'Elite North Korean hackers' blamed for $6.3B Binance hack

**原文链接**: [https://www.theguardian.com/business/live/2026/oct/30/uk-house-price-growth-crypto-industry-6bn-binance-hack-eurozone-france-gdp-latest-news-updates](https://www.theguardian.com/business/live/2026/oct/30/uk-house-price-growth-crypto-industry-6bn-binance-hack-eurozone-france-gdp-latest-news-updates)

生成摘要时出错

---

## 67. Flock camera searches fell 95% after a dispatcher's misconduct was caught

**原文标题**: Flock camera searches fell 95% after a dispatcher's misconduct was caught

**原文链接**: [https://www.wkyc.com/article/news/investigations/flock-camera-searches-fall-95-percent-highland-heights-dispatcher-misconduct-caught/95-94b18f33-60e2-4bc7-a00f-d71d1e1fdd5e](https://www.wkyc.com/article/news/investigations/flock-camera-searches-fall-95-percent-highland-heights-dispatcher-misconduct-caught/95-94b18f33-60e2-4bc7-a00f-d71d1e1fdd5e)

生成摘要时出错

---

## 68. Intel plunges 25%, triggers global chip rout on bleak outlook

**原文标题**: Intel plunges 25%, triggers global chip rout on bleak outlook

**原文链接**: [https://www.reuters.com/business/intel-warning-sparks-chip-rout-pc-weakness-clouds-turnaround-2026-10-30/](https://www.reuters.com/business/intel-warning-sparks-chip-rout-pc-weakness-clouds-turnaround-2026-10-30/)

生成摘要时出错

---

## 69. Show HN: I built a multiplayer game where you're an aerial fighter cat

**原文标题**: Show HN: I built a multiplayer game where you're an aerial fighter cat

**原文链接**: [https://catcopter.com](https://catcopter.com)

生成摘要时出错

---

## 70. What is a light-day? The milestone Voyager 1 is closing in on

**原文标题**: What is a light-day? The milestone Voyager 1 is closing in on

**原文链接**: [https://science.nasa.gov/mission/voyager/voyager-1/voyager-1-what-is-a-light-day/](https://science.nasa.gov/mission/voyager/voyager-1/voyager-1-what-is-a-light-day/)

生成摘要时出错

---

## 71. Anthropic blocks users for anything touching training larger models

**原文标题**: Anthropic blocks users for anything touching training larger models

**原文链接**: [https://twitter.com/jiahaoshao1/status/2116475922190922088](https://twitter.com/jiahaoshao1/status/2116475922190922088)

生成摘要时出错

---

## 72. A Pickpocket's Guide to New York

**原文标题**: A Pickpocket's Guide to New York

**原文链接**: [https://www.newyorker.com/magazine/2026/11/02/a-pickpockets-guide-to-new-york](https://www.newyorker.com/magazine/2026/11/02/a-pickpockets-guide-to-new-york)

生成摘要时出错

---

## 73. I didn't know I was lacking in Vitamin D until I collapsed at work

**原文标题**: I didn't know I was lacking in Vitamin D until I collapsed at work

**原文链接**: [https://www.bbc.com/news/articles/cm78pxxe55v0o](https://www.bbc.com/news/articles/cm78pxxe55v0o)

生成摘要时出错

---

## 74. Retired professor arrested for blocking delivery robot. Will do it again

**原文标题**: Retired professor arrested for blocking delivery robot. Will do it again

**原文链接**: [https://www.cnn.com/2026/10/31/us/philadelphia-woman-delivery-robots-cec](https://www.cnn.com/2026/10/31/us/philadelphia-woman-delivery-robots-cec)

生成摘要时出错

---

## 75. Geist Serif

**原文标题**: Geist Serif

**原文链接**: [https://vercel.com/blog/introducing-geist-serif](https://vercel.com/blog/introducing-geist-serif)

生成摘要时出错

---

## 76. Google value plunges by $500B as AI fears rattle Wall Street

**原文标题**: Google value plunges by $500B as AI fears rattle Wall Street

**原文链接**: [https://www.bbc.com/news/articles/cm9qzdqpxy48o](https://www.bbc.com/news/articles/cm9qzdqpxy48o)

生成摘要时出错

---

## 77. It's the Memory Latency, Stupid

**原文标题**: It's the Memory Latency, Stupid

**原文链接**: [https://pivotlake.io/blog/its-the-memory-latency-stupid/](https://pivotlake.io/blog/its-the-memory-latency-stupid/)

生成摘要时出错

---

## 78. Why Did Meta Suspend a US Senate Candidate's Instagram in the Middle of a Rally?

**原文标题**: Why Did Meta Suspend a US Senate Candidate's Instagram in the Middle of a Rally?

**原文链接**: [https://newrepublic.com/post/217281/meta-suspend-democratic-candidate-angie-nixon-instagram-account](https://newrepublic.com/post/217281/meta-suspend-democratic-candidate-angie-nixon-instagram-account)

生成摘要时出错

---

## 79. AI startup hacks Anthropic, gains access to employee details, internal messages

**原文标题**: AI startup hacks Anthropic, gains access to employee details, internal messages

**原文链接**: [https://www.indiatoday.in/technology/news/story/ai-startup-hacks-anthropic-in-12-hours-gains-access-to-employee-details-and-internal-messages-3025452-2026-10-26](https://www.indiatoday.in/technology/news/story/ai-startup-hacks-anthropic-in-12-hours-gains-access-to-employee-details-and-internal-messages-3025452-2026-10-26)

生成摘要时出错

---

## 80. Massie, Khanna, and Others Introduce the "Epstein Files Transparency Act II"

**原文标题**: Massie, Khanna, and Others Introduce the "Epstein Files Transparency Act II"

**原文链接**: [https://massie.house.gov/news/documentsingle.aspx?DocumentID=395849](https://massie.house.gov/news/documentsingle.aspx?DocumentID=395849)

生成摘要时出错

---

## 81. The Impact of Generative AI on Critical Thinking: Self-Reported (2025)

**原文标题**: The Impact of Generative AI on Critical Thinking: Self-Reported (2025)

**原文链接**: [https://dl.acm.org/doi/full/10.1145/3706598.3713778](https://dl.acm.org/doi/full/10.1145/3706598.3713778)

生成摘要时出错

---

## 82. Wall Street closes sharply lower as AI cash burn fears spark tech selloff

**原文标题**: Wall Street closes sharply lower as AI cash burn fears spark tech selloff

**原文链接**: [https://www.reuters.com/business/nasdaq-futures-tumble-amazon-intel-results-deepen-ai-spending-woes-2026-10-30/](https://www.reuters.com/business/nasdaq-futures-tumble-amazon-intel-results-deepen-ai-spending-woes-2026-10-30/)

生成摘要时出错

---

## 83. Anthropic takes steps to block Claude from reverse-engineering video games

**原文标题**: Anthropic takes steps to block Claude from reverse-engineering video games

**原文链接**: [https://mashable.com/tech/anthropic-takes-steps-to-block-video-game-cloning-and-reverse-engineering](https://mashable.com/tech/anthropic-takes-steps-to-block-video-game-cloning-and-reverse-engineering)

生成摘要时出错

---

## 84. Should a medical diagnosis reshape the past? (2025)

**原文标题**: Should a medical diagnosis reshape the past? (2025)

**原文链接**: [https://chengela.substack.com/p/should-a-medical-diagnosis-reshape](https://chengela.substack.com/p/should-a-medical-diagnosis-reshape)

生成摘要时出错

---

## 85. The Duty of a Scholar

**原文标题**: The Duty of a Scholar

**原文链接**: [https://www.daemonology.net/blog/2026-10-31-The-Duty-of-a-Scholar.html](https://www.daemonology.net/blog/2026-10-31-The-Duty-of-a-Scholar.html)

生成摘要时出错

---

## 86. Shiny Object Syndrome

**原文标题**: Shiny Object Syndrome

**原文链接**: [https://en.wikipedia.org/wiki/Shiny_object_syndrome](https://en.wikipedia.org/wiki/Shiny_object_syndrome)

生成摘要时出错

---

## 87. Some Thing is Happening A note from the AI companies

**原文标题**: Some Thing is Happening A note from the AI companies

**原文链接**: [https://alanbellows.com/some-thing-is-happening/](https://alanbellows.com/some-thing-is-happening/)

生成摘要时出错

---

## 88. CVE-2026-98432: Linux TCP Use-After-Free Risk and Patch Validation

**原文标题**: CVE-2026-98432: Linux TCP Use-After-Free Risk and Patch Validation

**原文链接**: [https://www.penligent.ai/hackinglabs/cve-2026-98432/](https://www.penligent.ai/hackinglabs/cve-2026-98432/)

生成摘要时出错

---

## 89. CVE 10.0: CVE-2026-112816, Canonical LXD, no emudhra required

**原文标题**: CVE 10.0: CVE-2026-112816, Canonical LXD, no emudhra required

**原文链接**: [https://www.cve.org/CVERecord?id=CVE-2026-112816](https://www.cve.org/CVERecord?id=CVE-2026-112816)

生成摘要时出错

---

## 90. Show HN: Arsaze – Cursor for video editing (Tab-complete and agent edits)

**原文标题**: Show HN: Arsaze – Cursor for video editing (Tab-complete and agent edits)

**原文链接**: [https://www.arsaze.com](https://www.arsaze.com)

生成摘要时出错

---

## 91. Anthropic's Claude AI blocks video game cloning and reverse-engineering

**原文标题**: Anthropic's Claude AI blocks video game cloning and reverse-engineering

**原文链接**: [https://www.tomshardware.com/tech-industry/artificial-intelligence/anthropics-ai-model-is-now-blocking-attempts-at-video-game-recreation-and-cloning-users-also-claim-non-malicious-generic-reverse-engineering-tasks-are-blocked](https://www.tomshardware.com/tech-industry/artificial-intelligence/anthropics-ai-model-is-now-blocking-attempts-at-video-game-recreation-and-cloning-users-also-claim-non-malicious-generic-reverse-engineering-tasks-are-blocked)

生成摘要时出错

---

## 92. Tracks along the longest drive on another world

**原文标题**: Tracks along the longest drive on another world

**原文链接**: [https://science.nasa.gov/blog/tracks-along-the-longest-drive-on-another-world/](https://science.nasa.gov/blog/tracks-along-the-longest-drive-on-another-world/)

生成摘要时出错

---

## 93. How long do you need to hold down the power button to turn off a PC?

**原文标题**: How long do you need to hold down the power button to turn off a PC?

**原文链接**: [https://www.osnews.com/story/146273/how-long-do-you-need-to-hold-down-the-power-button-to-turn-off-a-pc/](https://www.osnews.com/story/146273/how-long-do-you-need-to-hold-down-the-power-button-to-turn-off-a-pc/)

生成摘要时出错

---

## 94. Product Managers aren't safe either

**原文标题**: Product Managers aren't safe either

**原文链接**: [https://lucaskostka.com/posts/ai-challenges-more-than-devs](https://lucaskostka.com/posts/ai-challenges-more-than-devs)

生成摘要时出错

---

## 95. Neal Stephenson on AI and What Comes Next [video]

**原文标题**: Neal Stephenson on AI and What Comes Next [video]

**原文链接**: [https://www.youtube.com/watch?v=Ii-aeW5pHPQ](https://www.youtube.com/watch?v=Ii-aeW5pHPQ)

生成摘要时出错

---

## 96. Hackers hijack Egypt highway billboard and Malaysian screens to show porn

**原文标题**: Hackers hijack Egypt highway billboard and Malaysian screens to show porn

**原文链接**: [https://www.cairoreport.org/p/egypt-brazil-iraq-billboard-hack](https://www.cairoreport.org/p/egypt-brazil-iraq-billboard-hack)

生成摘要时出错

---

## 97. Why Anthropic's filing crushed tech stocks

**原文标题**: Why Anthropic's filing crushed tech stocks

**原文链接**: [https://www.thebignewsletter.com/p/why-anthropics-filing-crushed-tech](https://www.thebignewsletter.com/p/why-anthropics-filing-crushed-tech)

生成摘要时出错

---

## 98. Copyright Office is restoring copyright to something you have to work to get

**原文标题**: Copyright Office is restoring copyright to something you have to work to get

**原文链接**: [https://pluralistic.net/2026/10/31/burn-berne/#unvictored](https://pluralistic.net/2026/10/31/burn-berne/#unvictored)

生成摘要时出错

---

## 99. I Returned My iPhone Duo

**原文标题**: I Returned My iPhone Duo

**原文链接**: [https://codakuma.com/i-returned-my-duo/](https://codakuma.com/i-returned-my-duo/)

生成摘要时出错

---

## 100. William Nordhaus has died

**原文标题**: William Nordhaus has died

**原文链接**: [https://news.yale.edu/2026/10/31/william-nordhaus-nobel-laureate-who-integrated-economics-and-climate-change-devoted-yale](https://news.yale.edu/2026/10/31/william-nordhaus-nobel-laureate-who-integrated-economics-and-climate-change-devoted-yale)

生成摘要时出错

---

