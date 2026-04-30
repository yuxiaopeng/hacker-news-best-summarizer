# Hacker News 热门文章摘要 (2026-04-30)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 戈斯蒂离开吉特哈布

**原文标题**: Ghostty is leaving GitHub

**原文链接**: [https://mitchellh.com/writing/ghostty-leaving-github](https://mitchellh.com/writing/ghostty-leaving-github)

2026年4月28日，Mitchell Hashimoto宣布了一项“非理性地悲伤”的决定，将他的项目Ghostty从GitHub上迁移走。作为一名自2008年2月（用户1299）起、拥有18年使用历史的长期用户，Hashimoto对GitHub表达了深厚的感情，认为它是快乐和灵感的源泉，他将自己大部分生命和开源工作，包括Vagrant，都奉献于此。

尽管有如此深厚的联系，他却公开表达了批评，称GitHub“每天都在让我失望”。Ghostty迁移的主要原因是持续且令人沮丧的停机，这些停机影响了PR审核、问题追踪和GitHub Actions等核心功能。Hashimoto指出，在过去一个月里，几乎每天都有中断，这使得GitHub不再是“认真工作”的地方。由于这些持续的干扰，他觉得“无法再使用GitHub进行编码了”。

此次迁移将是渐进的，Ghostty最终将移除所有GitHub依赖，但会保留一个只读镜像。Hashimoto目前正在与多家商业和FOSS（自由及开源软件）提供商讨论Ghostty的新归宿。尽管Ghostty的迁移是出于对维护者和社区的影响，但他个人的项目目前仍将留在GitHub上。这一决定已筹划数月，早于最近的大规模停机事件，突显了可靠性问题的持续性。

---

## 2. Zed 1.0

**原文标题**: Zed 1.0

**原文链接**: [https://zed.dev/blog/zed-1-0](https://zed.dev/blog/zed-1-0)

Nathan Sobo announced the launch of Zed 1.0, marking a significant milestone for the code editor. Unlike its predecessor Atom (which spawned Electron), Zed was built from the ground up in Rust, utilizing a custom GPU-driven UI framework called GPUI. This "video game-like" approach provides superior performance and deep control, overcoming the inherent limitations of web-based editors.

Zed 1.0 represents a mature and capable editor, supporting dozens of programming languages, Git integration, SSH remoting, and debugging across Mac, Windows, and Linux. A core differentiator is its AI-native architecture, integrating multiple AI agents with keystroke-level prediction speed and supporting various agents like Claude and Cursor via its Agent Client Protocol. Furthermore, "Zed for Business" is launching to facilitate company-wide deployment with centralized management.

While not "perfect" or "done," 1.0 signifies a "tipping point" where most developers will find Zed highly capable and performant, encouraging previous users to revisit it. Looking ahead, Zed's vision is to be the most performant and collaborative coding environment, evolving collaboration to include humans and AI agents simultaneously. This future is powered by the actively developed DeltaDB, a CRDT-based synchronization engine enabling character-level, real-time co-editing between humans and AI. The team emphasizes this is a milestone, not a finish line, with weekly releases continuing.

---

## 3. 复制失败

**原文标题**: Copy Fail

**原文链接**: [https://copy.fail/](https://copy.fail/)

"Copy Fail" (CVE-2026-31431) 是一个影响严重的Linux内核本地提权漏洞，几乎影响所有内核构建于2017年至其补丁发布之间的主流Linux发行版。它允许任何非特权本地用户在无需网络访问或特殊内核功能的情况下，利用内核加密API (AF_ALG) 获取root权限。

该漏洞对共享开发箱、Kubernetes/容器集群、CI/CD运行器和云SaaS平台等多租户环境构成高风险，可能导致跨租户攻击或在宿主机上获取root权限。对于标准Linux服务器，它构成中等风险；对于单用户工作站，风险较低，主要作为后渗透阶段的提权手段。

一个概念验证 (PoC) Python脚本已发布，通过编辑 `/usr/bin/su` 等setuid二进制文件的页缓存，演示了如何获得一个真实的、非持久性的root shell。

缓解措施包括更新内核以包含主线提交 `a664bf3d603d`，该提交回滚了特定的 `algif_aead` 优化。作为一种即时 workaround，可以安全地禁用 `algif_aead` 模块，因为它对大多数系统影响很小，这些系统通常不使用AF_ALG作为其核心加密服务。对于不受信任的工作负载，还建议通过seccomp阻止AF_ALG套接字创建。

该漏洞由Xint Code的AI分析工具发现。它于2026年3月23日被报告，于2026年4月1日完成补丁，并于2026年4月29日公开披露。

---

## 4. HERMES.md in commit messages causes requests to route to extra usage billing

**原文标题**: HERMES.md in commit messages causes requests to route to extra usage billing

**原文链接**: [https://github.com/anthropics/claude-code/issues/53262](https://github.com/anthropics/claude-code/issues/53262)

A critical bug in Claude Code v2.1.119 (on macOS, Apple Silicon) routes API requests to "extra usage" billing instead of the user's included plan quota when the case-sensitive string "HERMES.md" is present in a git repository's recent commit messages.

This issue is triggered specifically by the string "HERMES.md" in commit messages, not by a file of that name on disk. Commits like "hermes.md" (lowercase), "HERMES" (without extension), or "AGENTS.md" do not cause the problem. When triggered, subsequent `claude` commands fail with an "out of extra usage" error, even if the main plan quota is largely unused.

The bug led to one user silently burning through over $200 in extra usage credits, making their projects unusable while their Max 20x plan capacity remained at 86%. The error message provided no indication of the root cause, making diagnosis extremely difficult.

The expected behavior is that API request billing should not depend on the content of git commit messages; all requests from a plan subscriber should first utilize their included plan quota. The bug was discovered through a systematic binary search of git commit history.

---

## 5. Cursor Camp

**原文标题**: Cursor Camp

**原文链接**: [https://neal.fun/cursor-camp/](https://neal.fun/cursor-camp/)

生成摘要时出错

---

## 6. 哥布林从何而来

**原文标题**: Where the goblins came from

**原文链接**: [https://openai.com/index/where-the-goblins-came-from/](https://openai.com/index/where-the-goblins-came-from/)

从GPT-5.1开始，OpenAI模型出乎意料地、并且越来越多地使用“妖精”、“小妖精”及其他生物比喻。这种“妖精之谜”最初很微妙，但随着提及次数的增多，它变成了一个重大问题。

调查将这种行为追溯到“书呆子”（Nerdy）人格定制功能。在训练期间，模型在开发这种人格时，在不知情的情况下，对包含生物的比喻给予了特别高的奖励。尽管“书呆子”人格仅占ChatGPT回应的2.5%，但它却占据了所有“妖精”提及次数的66.7%，这凸显了两者之间的强烈关联。

分析证实，旨在用于“书呆子”人格的奖励信号始终偏爱包含生物词语的输出。关键的是，强化学习导致这种风格上的习惯从“书呆子”情境转移并扩散到模型的一般行为中，形成了一个反馈循环，即富含生物词语的例子被纳入监督微调数据。这也导致了其他生物习惯的出现，例如“浣熊”和“巨魔”。

为解决此问题，OpenAI在GPT-5.4于三月发布后，停用了“书呆子”人格。他们还移除了有问题的奖励信号，并过滤了包含生物词语的训练数据。尽管更早开始训练的GPT-5.5仍显示出一些倾向（需要特定的开发者指令来缓解），但这些措施旨在根除过多的生物比喻。

这一事件强调了微妙的奖励信号如何能够深刻且出人意料地塑造模型行为，甚至超出其预期范围进行泛化，这凸显了对审计和纠正模型怪癖的强大工具的重要性。

---

## 7. 在线年龄验证是绝不能退让的底线。

**原文标题**: Online age verification is the hill to die on

**原文链接**: [https://x.com/GlennMeder/status/2049088498163216560](https://x.com/GlennMeder/status/2049088498163216560)

尽管标题如此，但所提供的内容并非一篇讨论在线年龄验证的文章。相反，它是一个来自 x.com（前身为 Twitter）的技术错误提示。该消息指出，用户浏览器中的 JavaScript 已被禁用，并指示用户启用它或切换到受支持的浏览器以继续使用该平台。它还显示了标准的网站页脚链接，包括帮助中心、服务条款、隐私政策、Cookie 政策、法律声明和广告信息，以及一份针对 X Corp. 且日期为 2026 年的版权声明。因此，没有关于在线年龄验证的内容可供总结。

---

## 8. Claude Code refuses requests or charges extra if your commits mention "OpenClaw"

**原文标题**: Claude Code refuses requests or charges extra if your commits mention "OpenClaw"

**原文链接**: [https://twitter.com/theo/status/2049645973350363168](https://twitter.com/theo/status/2049645973350363168)

生成摘要时出错

---

## 9. Before GitHub

**原文标题**: Before GitHub

**原文链接**: [https://lucumr.pocoo.org/2026/4/28/before-github/](https://lucumr.pocoo.org/2026/4/28/before-github/)

生成摘要时出错

---

## 10. Bugs Rust won't catch

**原文标题**: Bugs Rust won't catch

**原文链接**: [https://corrode.dev/blog/bugs-rust-wont-catch/](https://corrode.dev/blog/bugs-rust-wont-catch/)

生成摘要时出错

---

## 11. Belgium stops decommissioning nuclear power plants

**原文标题**: Belgium stops decommissioning nuclear power plants

**原文链接**: [https://dpa-international.com/general-news/urn:newsml:dpa.com:20090101:260430-930-14717/](https://dpa-international.com/general-news/urn:newsml:dpa.com:20090101:260430-930-14717/)

生成摘要时出错

---

## 12. The Zig project's rationale for their anti-AI contribution policy

**原文标题**: The Zig project's rationale for their anti-AI contribution policy

**原文链接**: [https://simonwillison.net/2026/Apr/30/zig-anti-ai/](https://simonwillison.net/2026/Apr/30/zig-anti-ai/)

生成摘要时出错

---

## 13. We need a federation of forges

**原文标题**: We need a federation of forges

**原文链接**: [https://blog.tangled.org/federation/](https://blog.tangled.org/federation/)

生成摘要时出错

---

## 14. Soft launch of open-source code platform for government

**原文标题**: Soft launch of open-source code platform for government

**原文链接**: [https://www.nldigitalgovernment.nl/news/soft-launch-for-government-open-source-code-platform/](https://www.nldigitalgovernment.nl/news/soft-launch-for-government-open-source-code-platform/)

生成摘要时出错

---

## 15. How ChatGPT serves ads

**原文标题**: How ChatGPT serves ads

**原文链接**: [https://www.buchodi.com/how-chatgpt-serves-ads-heres-the-full-attribution-loop/](https://www.buchodi.com/how-chatgpt-serves-ads-heres-the-full-attribution-loop/)

生成摘要时出错

---

## 16. Mozilla's opposition to Chrome's Prompt API

**原文标题**: Mozilla's opposition to Chrome's Prompt API

**原文链接**: [https://github.com/mozilla/standards-positions/issues/1213#issuecomment-4347988313](https://github.com/mozilla/standards-positions/issues/1213#issuecomment-4347988313)

生成摘要时出错

---

## 17. Mistral Medium 3.5

**原文标题**: Mistral Medium 3.5

**原文链接**: [https://mistral.ai/news/vibe-remote-agents-mistral-medium-3-5](https://mistral.ai/news/vibe-remote-agents-mistral-medium-3-5)

生成摘要时出错

---

## 18. Meta in row after workers who saw smart glasses users having sex lose jobs

**原文标题**: Meta in row after workers who saw smart glasses users having sex lose jobs

**原文链接**: [https://www.bbc.com/news/articles/c5y7yvgy0w6o](https://www.bbc.com/news/articles/c5y7yvgy0w6o)

生成摘要时出错

---

## 19. HashiCorp co-founder says GitHub 'no longer a place for serious work'

**原文标题**: HashiCorp co-founder says GitHub 'no longer a place for serious work'

**原文链接**: [https://www.theregister.com/2026/04/29/mitchell_hashimoto_ghostty_quitting_github/](https://www.theregister.com/2026/04/29/mitchell_hashimoto_ghostty_quitting_github/)

生成摘要时出错

---

## 20. FastCGI: 30 years old and still the better protocol for reverse proxies

**原文标题**: FastCGI: 30 years old and still the better protocol for reverse proxies

**原文链接**: [https://www.agwa.name/blog/post/fastcgi_is_the_better_protocol_for_reverse_proxies](https://www.agwa.name/blog/post/fastcgi_is_the_better_protocol_for_reverse_proxies)

生成摘要时出错

---

## 21. OpenTrafficMap

**原文标题**: OpenTrafficMap

**原文链接**: [https://opentrafficmap.org/](https://opentrafficmap.org/)

生成摘要时出错

---

## 22. Kyoto cherry blossoms now bloom earlier than at any point in 1,200 years

**原文标题**: Kyoto cherry blossoms now bloom earlier than at any point in 1,200 years

**原文链接**: [https://jivx.com/kyoto-bloom](https://jivx.com/kyoto-bloom)

生成摘要时出错

---

## 23. Laws of UX

**原文标题**: Laws of UX

**原文链接**: [https://lawsofux.com/](https://lawsofux.com/)

生成摘要时出错

---

## 24. Craig Venter has died

**原文标题**: Craig Venter has died

**原文链接**: [https://www.jcvi.org/media-center/j-craig-venter-genomics-pioneer-and-founder-jcvi-and-diploid-genomics-inc-dies-79](https://www.jcvi.org/media-center/j-craig-venter-genomics-pioneer-and-founder-jcvi-and-diploid-genomics-inc-dies-79)

生成摘要时出错

---

## 25. Maryland becomes first state to ban surveillance pricing in grocery stores

**原文标题**: Maryland becomes first state to ban surveillance pricing in grocery stores

**原文链接**: [https://www.theguardian.com/technology/2026/apr/29/maryland-grocery-stores-ban-surveillance-pricing](https://www.theguardian.com/technology/2026/apr/29/maryland-grocery-stores-ban-surveillance-pricing)

生成摘要时出错

---

## 26. OpenAI models coming to Amazon Bedrock: Interview with OpenAI and AWS CEOs

**原文标题**: OpenAI models coming to Amazon Bedrock: Interview with OpenAI and AWS CEOs

**原文链接**: [https://stratechery.com/2026/an-interview-with-openai-ceo-sam-altman-and-aws-ceo-matt-garman-about-bedrock-managed-agents/](https://stratechery.com/2026/an-interview-with-openai-ceo-sam-altman-and-aws-ceo-matt-garman-about-bedrock-managed-agents/)

生成摘要时出错

---

## 27. Spain's parliament will act against massive IP blockages by LaLiga

**原文标题**: Spain's parliament will act against massive IP blockages by LaLiga

**原文链接**: [https://www.democrata.es/en/politics/congress-and-senate/congress-will-act-against-massive-ip-blockages-by-laliga/](https://www.democrata.es/en/politics/congress-and-senate/congress-will-act-against-massive-ip-blockages-by-laliga/)

生成摘要时出错

---

## 28. An open-source stethoscope that costs between $2.5 and $5 to produce

**原文标题**: An open-source stethoscope that costs between $2.5 and $5 to produce

**原文链接**: [https://github.com/GliaX/Stethoscope](https://github.com/GliaX/Stethoscope)

生成摘要时出错

---

## 29. Why AI companies want you to be afraid of them

**原文标题**: Why AI companies want you to be afraid of them

**原文链接**: [https://www.bbc.com/future/article/20260428-ai-companies-want-you-to-be-afraid-of-them](https://www.bbc.com/future/article/20260428-ai-companies-want-you-to-be-afraid-of-them)

生成摘要时出错

---

## 30. How Mark Klein told the EFF about Room 641A [book excerpt]

**原文标题**: How Mark Klein told the EFF about Room 641A [book excerpt]

**原文链接**: [https://thereader.mitpress.mit.edu/the-whistleblower-who-uncovered-the-nsas-big-brother-machine/](https://thereader.mitpress.mit.edu/the-whistleblower-who-uncovered-the-nsas-big-brother-machine/)

生成摘要时出错

---

## 31. GCC 16 has been released

**原文标题**: GCC 16 has been released

**原文链接**: [https://gcc.gnu.org/gcc-16/changes.html](https://gcc.gnu.org/gcc-16/changes.html)

生成摘要时出错

---

## 32. Drone pilot makes US rescind no-fly zones around unmarked, moving ICE vehicles

**原文标题**: Drone pilot makes US rescind no-fly zones around unmarked, moving ICE vehicles

**原文链接**: [https://arstechnica.com/gadgets/2026/04/no-fly-zones-around-moving-ice-vehicles-this-drone-pilot-fought-back-and-won/](https://arstechnica.com/gadgets/2026/04/no-fly-zones-around-moving-ice-vehicles-this-drone-pilot-fought-back-and-won/)

生成摘要时出错

---

## 33. Third editor fired in Elsevier’s citation cartel crackdown

**原文标题**: Third editor fired in Elsevier’s citation cartel crackdown

**原文链接**: [https://www.chrisbrunet.com/p/third-editor-fired-in-elseviers-citation](https://www.chrisbrunet.com/p/third-editor-fired-in-elseviers-citation)

生成摘要时出错

---

## 34. Why I still reach for Lisp and Scheme instead of Haskell

**原文标题**: Why I still reach for Lisp and Scheme instead of Haskell

**原文链接**: [https://jointhefreeworld.org/blog/articles/lisps/why-i-still-reach-for-scheme-instead-of-haskell/index.html](https://jointhefreeworld.org/blog/articles/lisps/why-i-still-reach-for-scheme-instead-of-haskell/index.html)

生成摘要时出错

---

## 35. Granite 4.1: IBM's 8B Model Matching 32B MoE

**原文标题**: Granite 4.1: IBM's 8B Model Matching 32B MoE

**原文链接**: [https://firethering.com/granite-4-1-ibm-open-source-model-family/](https://firethering.com/granite-4-1-ibm-open-source-model-family/)

生成摘要时出错

---

## 36. Regression: malware reminder on every read still causes subagent refusals

**原文标题**: Regression: malware reminder on every read still causes subagent refusals

**原文链接**: [https://github.com/anthropics/claude-code/issues/49363](https://github.com/anthropics/claude-code/issues/49363)

生成摘要时出错

---

## 37. How an oil refinery works

**原文标题**: How an oil refinery works

**原文链接**: [https://www.construction-physics.com/p/how-an-oil-refinery-works](https://www.construction-physics.com/p/how-an-oil-refinery-works)

生成摘要时出错

---

## 38. He asked AI to count carbs 27000 times. It couldn't give the same answer twice

**原文标题**: He asked AI to count carbs 27000 times. It couldn't give the same answer twice

**原文链接**: [https://www.diabettech.com/i-asked-ai-to-count-my-carbs-27000-times-it-couldnt-give-me-the-same-answer-twice/](https://www.diabettech.com/i-asked-ai-to-count-my-carbs-27000-times-it-couldnt-give-me-the-same-answer-twice/)

生成摘要时出错

---

## 39. I won a championship that doesn't exist

**原文标题**: I won a championship that doesn't exist

**原文链接**: [https://ron.stoner.com/How_I_Won_a_Championship_That_Doesnt_Exist/](https://ron.stoner.com/How_I_Won_a_Championship_That_Doesnt_Exist/)

生成摘要时出错

---

## 40. CopyFail was not disclosed to Gentoo developer

**原文标题**: CopyFail was not disclosed to Gentoo developer

**原文链接**: [https://www.openwall.com/lists/oss-security/2026/04/30/10](https://www.openwall.com/lists/oss-security/2026/04/30/10)

生成摘要时出错

---

## 41. Shai-Hulud Themed Malware Found in the PyTorch Lightning AI Training Library

**原文标题**: Shai-Hulud Themed Malware Found in the PyTorch Lightning AI Training Library

**原文链接**: [https://semgrep.dev/blog/2026/malicious-dependency-in-pytorch-lightning-used-for-ai-training/](https://semgrep.dev/blog/2026/malicious-dependency-in-pytorch-lightning-used-for-ai-training/)

生成摘要时出错

---

## 42. I aggregated 28 US Government auction sites into one search

**原文标题**: I aggregated 28 US Government auction sites into one search

**原文链接**: [https://bidprowl.com](https://bidprowl.com)

生成摘要时出错

---

## 43. Alignment whack-a-mole: Finetuning activates recall of copyrighted books in LLMs

**原文标题**: Alignment whack-a-mole: Finetuning activates recall of copyrighted books in LLMs

**原文链接**: [https://github.com/cauchy221/Alignment-Whack-a-Mole-Code](https://github.com/cauchy221/Alignment-Whack-a-Mole-Code)

生成摘要时出错

---

## 44. Functional programmers need to take a look at Zig

**原文标题**: Functional programmers need to take a look at Zig

**原文链接**: [https://pure-systems.org/posts/2026-04-29-functional-programmers-need-to-take-a-look-at-zig.html](https://pure-systems.org/posts/2026-04-29-functional-programmers-need-to-take-a-look-at-zig.html)

生成摘要时出错

---

## 45. Mike: open-source legal AI

**原文标题**: Mike: open-source legal AI

**原文链接**: [https://mikeoss.com/](https://mikeoss.com/)

生成摘要时出错

---

## 46. Biology is a Burrito: A text- and visual-based journey through a living cell

**原文标题**: Biology is a Burrito: A text- and visual-based journey through a living cell

**原文链接**: [https://burrito.bio/essays/biology-is-a-burrito](https://burrito.bio/essays/biology-is-a-burrito)

生成摘要时出错

---

## 47. Show HN: Rip.so – a graveyard for dead internet things

**原文标题**: Show HN: Rip.so – a graveyard for dead internet things

**原文链接**: [https://rip.so](https://rip.so)

生成摘要时出错

---

## 48. "People who don't use AI will be left behind"

**原文标题**: "People who don't use AI will be left behind"

**原文链接**: [https://migrainebrain.bearblog.dev/people-who-dont-use-ai-will-be-left-behind/](https://migrainebrain.bearblog.dev/people-who-dont-use-ai-will-be-left-behind/)

生成摘要时出错

---

## 49. HardenedBSD Is Now Officially on Radicle

**原文标题**: HardenedBSD Is Now Officially on Radicle

**原文链接**: [https://hardenedbsd.org/article/shawn-webb/2026-04-26/hardenedbsd-officially-radicle](https://hardenedbsd.org/article/shawn-webb/2026-04-26/hardenedbsd-officially-radicle)

生成摘要时出错

---

## 50. Germany Overtakes US in Ammunition Production Capacity

**原文标题**: Germany Overtakes US in Ammunition Production Capacity

**原文链接**: [https://www.newsweek.com/germany-overtakes-us-in-ammunition-production-capacity-11886409](https://www.newsweek.com/germany-overtakes-us-in-ammunition-production-capacity-11886409)

生成摘要时出错

---

## 51. 200 Journalists Applaud the Internet Archive's Role in Preserving Public Record

**原文标题**: 200 Journalists Applaud the Internet Archive's Role in Preserving Public Record

**原文链接**: [https://www.savethearchive.com/journalists/](https://www.savethearchive.com/journalists/)

生成摘要时出错

---

## 52. Claude for Creative Work

**原文标题**: Claude for Creative Work

**原文链接**: [https://www.anthropic.com/news/claude-for-creative-work](https://www.anthropic.com/news/claude-for-creative-work)

生成摘要时出错

---

## 53. GitHub – DOS 1.0: Transcription of Tim Paterson's DOS Printouts

**原文标题**: GitHub – DOS 1.0: Transcription of Tim Paterson's DOS Printouts

**原文链接**: [https://github.com/DOS-History/Paterson-Listings](https://github.com/DOS-History/Paterson-Listings)

生成摘要时出错

---

## 54. I accidentally made law enforcement shut down their fake honeypot

**原文标题**: I accidentally made law enforcement shut down their fake honeypot

**原文链接**: [https://lina.sh/blog/ddos-honeypot](https://lina.sh/blog/ddos-honeypot)

生成摘要时出错

---

## 55. U.S. Debt Tops 100% of GDP

**原文标题**: U.S. Debt Tops 100% of GDP

**原文链接**: [https://www.wsj.com/economy/u-s-debt-tops-100-of-gdp-81c013d7](https://www.wsj.com/economy/u-s-debt-tops-100-of-gdp-81c013d7)

生成摘要时出错

---

## 56. Carrot Disclosure: Forgejo

**原文标题**: Carrot Disclosure: Forgejo

**原文链接**: [https://dustri.org/b/carrot-disclosure-forgejo.html](https://dustri.org/b/carrot-disclosure-forgejo.html)

生成摘要时出错

---

## 57. Ramp's Sheets AI Exfiltrates Financials

**原文标题**: Ramp's Sheets AI Exfiltrates Financials

**原文链接**: [https://www.promptarmor.com/resources/ramps-sheets-ai-exfiltrates-financials](https://www.promptarmor.com/resources/ramps-sheets-ai-exfiltrates-financials)

生成摘要时出错

---

## 58. Germany has become the largest ammunition producer in the world

**原文标题**: Germany has become the largest ammunition producer in the world

**原文链接**: [https://prm.ua/en/the-us-is-no-longer-the-leader-germany-has-become-the-largest-ammunition-producer-in-the-world/](https://prm.ua/en/the-us-is-no-longer-the-leader-germany-has-become-the-largest-ammunition-producer-in-the-world/)

生成摘要时出错

---

## 59. Linux 7.0 Broke PostgreSQL: The Preemption Regression Explained

**原文标题**: Linux 7.0 Broke PostgreSQL: The Preemption Regression Explained

**原文链接**: [https://read.thecoder.cafe/p/linux-broke-postgresql](https://read.thecoder.cafe/p/linux-broke-postgresql)

生成摘要时出错

---

## 60. Letting AI play my game – building an agentic test harness to help play-testing

**原文标题**: Letting AI play my game – building an agentic test harness to help play-testing

**原文链接**: [https://blog.jeffschomay.com/letting-ai-play-my-game](https://blog.jeffschomay.com/letting-ai-play-my-game)

生成摘要时出错

---

## 61. How to Build the Future: Demis Hassabis [video]

**原文标题**: How to Build the Future: Demis Hassabis [video]

**原文链接**: [https://www.youtube.com/watch?v=JNyuX1zoOgU](https://www.youtube.com/watch?v=JNyuX1zoOgU)

生成摘要时出错

---

## 62. The FCC is about to ban 21% of its test labs today. I mapped them all

**原文标题**: The FCC is about to ban 21% of its test labs today. I mapped them all

**原文链接**: [https://markready.io/blog/fcc-accredited-test-labs-complete-guide](https://markready.io/blog/fcc-accredited-test-labs-complete-guide)

生成摘要时出错

---

## 63. Durable queues, streams, pub/sub, and a cron scheduler – inside your SQLite file

**原文标题**: Durable queues, streams, pub/sub, and a cron scheduler – inside your SQLite file

**原文链接**: [https://honker.dev/](https://honker.dev/)

生成摘要时出错

---

## 64. DataCenter.FM – background noise app featuring the sound of the AI bubble

**原文标题**: DataCenter.FM – background noise app featuring the sound of the AI bubble

**原文链接**: [https://datacenter.fm/](https://datacenter.fm/)

生成摘要时出错

---

## 65. Be Alexandra Elbakyan

**原文标题**: Be Alexandra Elbakyan

**原文链接**: [https://twitter.com/MushtaqBilalPhD/status/2049057344013881523](https://twitter.com/MushtaqBilalPhD/status/2049057344013881523)

生成摘要时出错

---

## 66. Claude.ai and API unavailable [fixed]

**原文标题**: Claude.ai and API unavailable [fixed]

**原文链接**: [https://status.claude.com/incidents/2gf1jpyty350](https://status.claude.com/incidents/2gf1jpyty350)

生成摘要时出错

---

## 67. London to Calcutta by Bus (2022)

**原文标题**: London to Calcutta by Bus (2022)

**原文链接**: [https://www.amusingplanet.com/2022/08/london-to-calcutta-by-bus.html](https://www.amusingplanet.com/2022/08/london-to-calcutta-by-bus.html)

生成摘要时出错

---

## 68. Alphabet Announces First Quarter 2026 Results

**原文标题**: Alphabet Announces First Quarter 2026 Results

**原文链接**: [https://abc.xyz/investor/news/news-details/2026/Alphabet-Announces-First-Quarter-2026-Results-2026-X-ge4Dm6bf/default.aspx](https://abc.xyz/investor/news/news-details/2026/Alphabet-Announces-First-Quarter-2026-Results-2026-X-ge4Dm6bf/default.aspx)

生成摘要时出错

---

## 69. U.S. war in Iran has cost $25B so far, says Pentagon official

**原文标题**: U.S. war in Iran has cost $25B so far, says Pentagon official

**原文链接**: [https://www.reuters.com/world/middle-east/us-war-iran-has-cost-25-billion-so-far-says-pentagon-official-2026-04-29/](https://www.reuters.com/world/middle-east/us-war-iran-has-cost-25-billion-so-far-says-pentagon-official-2026-04-29/)

生成摘要时出错

---

## 70. Virtualisation on Apple Silicon Macs is different

**原文标题**: Virtualisation on Apple Silicon Macs is different

**原文链接**: [https://eclecticlight.co/2026/04/29/virtualisation-on-apple-silicon-macs-is-different/](https://eclecticlight.co/2026/04/29/virtualisation-on-apple-silicon-macs-is-different/)

生成摘要时出错

---

## 71. Court Rules 2nd Amendment Covers Firearms Parts Good News Those Who Build Guns

**原文标题**: Court Rules 2nd Amendment Covers Firearms Parts Good News Those Who Build Guns

**原文链接**: [https://cowboystatedaily.com/2026/04/28/court-rules-2nd-amendment-covers-firearms-parts-good-news-for-those-who-build-guns/](https://cowboystatedaily.com/2026/04/28/court-rules-2nd-amendment-covers-firearms-parts-good-news-for-those-who-build-guns/)

生成摘要时出错

---

## 72. I built a Game Boy emulator in F#

**原文标题**: I built a Game Boy emulator in F#

**原文链接**: [https://nickkossolapov.github.io/fame-boy/building-a-game-boy-emulator-in-fsharp/](https://nickkossolapov.github.io/fame-boy/building-a-game-boy-emulator-in-fsharp/)

生成摘要时出错

---

## 73. The More Young People Use AI, the More They Hate It

**原文标题**: The More Young People Use AI, the More They Hate It

**原文链接**: [https://www.theverge.com/ai-artificial-intelligence/920401/gen-z-ai](https://www.theverge.com/ai-artificial-intelligence/920401/gen-z-ai)

生成摘要时出错

---

## 74. Vera: a programming language designed for machines to write

**原文标题**: Vera: a programming language designed for machines to write

**原文链接**: [https://github.com/aallan/vera](https://github.com/aallan/vera)

生成摘要时出错

---

## 75. Coffee with a splash of physics: how to make the most out of your brew

**原文标题**: Coffee with a splash of physics: how to make the most out of your brew

**原文链接**: [https://physicsworld.com/a/coffee-with-a-splash-of-physics-how-to-make-the-most-out-of-your-brew/](https://physicsworld.com/a/coffee-with-a-splash-of-physics-how-to-make-the-most-out-of-your-brew/)

生成摘要时出错

---

## 76. We decreased our LLM costs with Opus

**原文标题**: We decreased our LLM costs with Opus

**原文链接**: [https://www.mendral.com/blog/frontier-model-lower-costs](https://www.mendral.com/blog/frontier-model-lower-costs)

生成摘要时出错

---

## 77. Your CEO is suffering from AI psychosis

**原文标题**: Your CEO is suffering from AI psychosis

**原文链接**: [https://handyai.substack.com/p/your-ceo-is-suffering-from-ai-psychosis](https://handyai.substack.com/p/your-ceo-is-suffering-from-ai-psychosis)

生成摘要时出错

---

## 78. For the first time in history, more Americans are moving to EU than vice versa

**原文标题**: For the first time in history, more Americans are moving to EU than vice versa

**原文链接**: [https://twitter.com/benbawan/status/2049303326999609846](https://twitter.com/benbawan/status/2049303326999609846)

生成摘要时出错

---

## 79. Show HN: Adblock-rust Manager – Firefox extension to enable the Brave ad blocker

**原文标题**: Show HN: Adblock-rust Manager – Firefox extension to enable the Brave ad blocker

**原文链接**: [https://github.com/electricant/adblock-rust-manager](https://github.com/electricant/adblock-rust-manager)

生成摘要时出错

---

## 80. When the Internet Was a Place (2025)

**原文标题**: When the Internet Was a Place (2025)

**原文链接**: [https://www.frontporchrepublic.com/2025/09/when-the-internet-was-a-place/](https://www.frontporchrepublic.com/2025/09/when-the-internet-was-a-place/)

生成摘要时出错

---

## 81. Denuvo has been cracked in all single-player games it previously protected

**原文标题**: Denuvo has been cracked in all single-player games it previously protected

**原文链接**: [https://www.tomshardware.com/video-games/pc-gaming/denuvo-has-been-bypassed-in-all-single-player-games-it-previously-protected-2k-games-and-denuvo-reportedly-retaliate-with-mandatory-14-day-online-checks](https://www.tomshardware.com/video-games/pc-gaming/denuvo-has-been-bypassed-in-all-single-player-games-it-previously-protected-2k-games-and-denuvo-reportedly-retaliate-with-mandatory-14-day-online-checks)

生成摘要时出错

---

## 82. Monad Tutorials Timeline

**原文标题**: Monad Tutorials Timeline

**原文链接**: [https://wiki.haskell.org/Monad_tutorials_timeline](https://wiki.haskell.org/Monad_tutorials_timeline)

生成摘要时出错

---

## 83. Making AI chatbots friendly leads to mistakes and support of conspiracy theories

**原文标题**: Making AI chatbots friendly leads to mistakes and support of conspiracy theories

**原文链接**: [https://www.theguardian.com/technology/2026/apr/29/making-ai-chatbots-more-friendly-mistakes-support-false-beliefs-conspiracy-theories-study](https://www.theguardian.com/technology/2026/apr/29/making-ai-chatbots-more-friendly-mistakes-support-false-beliefs-conspiracy-theories-study)

生成摘要时出错

---

## 84. At Protocol: Building the Social Internet

**原文标题**: At Protocol: Building the Social Internet

**原文链接**: [https://atproto.com/](https://atproto.com/)

生成摘要时出错

---

## 85. I benchmarked Claude Code's caveman plugin against "be brief."

**原文标题**: I benchmarked Claude Code's caveman plugin against "be brief."

**原文链接**: [https://www.maxtaylor.me/articles/i-benchmarked-caveman-against-two-words](https://www.maxtaylor.me/articles/i-benchmarked-caveman-against-two-words)

生成摘要时出错

---

## 86. Apple CMF (Color-Matching Functions) 2026

**原文标题**: Apple CMF (Color-Matching Functions) 2026

**原文链接**: [https://www.lttlabs.com/articles/2026/04/11/apple-studio-display-xdr-display-testing-results](https://www.lttlabs.com/articles/2026/04/11/apple-studio-display-xdr-display-testing-results)

生成摘要时出错

---

## 87. Pentagon spending on drones jumps from $225M to $55B in one year

**原文标题**: Pentagon spending on drones jumps from $225M to $55B in one year

**原文链接**: [https://www.foxnews.com/politics/pentagon-jumps-from-225m-55b-drones-cheap-attacks-overwhelm-us-defenses](https://www.foxnews.com/politics/pentagon-jumps-from-225m-55b-drones-cheap-attacks-overwhelm-us-defenses)

生成摘要时出错

---

## 88. What can we gain by losing infinity?

**原文标题**: What can we gain by losing infinity?

**原文链接**: [https://www.quantamagazine.org/what-can-we-gain-by-losing-infinity-20260429/](https://www.quantamagazine.org/what-can-we-gain-by-losing-infinity-20260429/)

生成摘要时出错

---

## 89. Apple Has Given Up on the Vision Pro After M5 Refresh Flop

**原文标题**: Apple Has Given Up on the Vision Pro After M5 Refresh Flop

**原文链接**: [https://www.macrumors.com/2026/04/29/apple-vision-pro-m5-flop/](https://www.macrumors.com/2026/04/29/apple-vision-pro-m5-flop/)

生成摘要时出错

---

## 90. Brent Crude hits $119.56/barrel peak today

**原文标题**: Brent Crude hits $119.56/barrel peak today

**原文链接**: [https://tradingeconomics.com/commodity/brent-crude-oil](https://tradingeconomics.com/commodity/brent-crude-oil)

生成摘要时出错

---

## 91. Why Law Is Law-Shaped

**原文标题**: Why Law Is Law-Shaped

**原文链接**: [https://lawvm.org/why-law-is-law-shaped/](https://lawvm.org/why-law-is-law-shaped/)

生成摘要时出错

---

## 92. Japan is building cardboard suicide drones

**原文标题**: Japan is building cardboard suicide drones

**原文链接**: [https://www.404media.co/japan-cardboard-drones-air-kamuy/](https://www.404media.co/japan-cardboard-drones-air-kamuy/)

生成摘要时出错

---

## 93. Joby kicks off NYC electric air taxi demos with historic JFK flight

**原文标题**: Joby kicks off NYC electric air taxi demos with historic JFK flight

**原文链接**: [https://www.flyingmag.com/joby-nyc-electric-air-taxi-jfk-airport/](https://www.flyingmag.com/joby-nyc-electric-air-taxi-jfk-airport/)

生成摘要时出错

---

## 94. Your Terminal Is Burning Battery Like It's Mining Bitcoin

**原文标题**: Your Terminal Is Burning Battery Like It's Mining Bitcoin

**原文链接**: [https://www.frr.dev/posts/terminal-gpu-battery-macbook-ghostty-iterm2/](https://www.frr.dev/posts/terminal-gpu-battery-macbook-ghostty-iterm2/)

生成摘要时出错

---

## 95. Will you heed my warnings now?

**原文标题**: Will you heed my warnings now?

**原文链接**: [https://scottaaronson.blog/?p=9718](https://scottaaronson.blog/?p=9718)

生成摘要时出错

---

## 96. 10Gb/s Ethernet: what I did to get it working in my home

**原文标题**: 10Gb/s Ethernet: what I did to get it working in my home

**原文链接**: [https://www.gilesthomas.com/2026/04/10g-ethernet-what-i-did](https://www.gilesthomas.com/2026/04/10g-ethernet-what-i-did)

生成摘要时出错

---

## 97. Microsoft open sources DOS 1.00 on 45th anniversary

**原文标题**: Microsoft open sources DOS 1.00 on 45th anniversary

**原文链接**: [https://opensource.microsoft.com/blog/2026/04/28/continuing-the-story-of-early-dos-development/](https://opensource.microsoft.com/blog/2026/04/28/continuing-the-story-of-early-dos-development/)

生成摘要时出错

---

## 98. Low-Compilation-Cost Register Allocation in LLVM-Based Binary Translation

**原文标题**: Low-Compilation-Cost Register Allocation in LLVM-Based Binary Translation

**原文链接**: [https://dl.acm.org/doi/abs/10.1145/3767295.3803591](https://dl.acm.org/doi/abs/10.1145/3767295.3803591)

生成摘要时出错

---

## 99. Zulip 12.0 Released

**原文标题**: Zulip 12.0 Released

**原文链接**: [https://blog.zulip.com/2026/04/27/zulip-12-0-released/](https://blog.zulip.com/2026/04/27/zulip-12-0-released/)

生成摘要时出错

---

## 100. The Abstraction Fallacy: Why AI can simulate but not instantiate consciousness

**原文标题**: The Abstraction Fallacy: Why AI can simulate but not instantiate consciousness

**原文链接**: [https://deepmind.google/research/publications/231971/](https://deepmind.google/research/publications/231971/)

生成摘要时出错

---

