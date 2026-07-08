# Hacker News 热门文章摘要 (2026-07-08)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 我们每周收费1万美元删除AI生成的代码。

**原文标题**: We charge $10k a week to delete AI-generated code

**原文链接**: [https://odra.dev/slopfix/](https://odra.dev/slopfix/)

本文介绍了一项旨在解决维护AI生成代码库挑战的服务，这些代码库往往会随着项目规模的扩大而变得臃肿、拖慢功能开发并引入新bug。

这项由三位资深工程师团队提供的服务，首先对客户的代码库进行免费分析。如果他们认为可以提供帮助，他们会承诺一个固定价格和具体的代码行数缩减目标（例如，从100,000行缩减到35,000行），同时确保功能完整性。

核心工作为期一周的集中精力。他们首先建立一份应用程序功能的全面清单。然后，通过整合重复代码、用库替换自定义框架以及清晰地重建无法挽救的部分来进行重构。团队明确指出，尽管他们会利用Claude Code等AI工具，但严格遵循他们三十年关于可维护代码实践的人类经验。

客户将收到一个更小、更清晰的代码库、一份质量保证清单，以及一套用于持续维护代码质量的“护栏”（例如，lint规则、CI检查），外加两周的工作质保期。

费用为每周10,000美元，付款与达成的缩减目标成比例。例如，如果完成了承诺缩减量的40%，则支付40%的费用（4,000美元）。代码行数通过`scc`工具测量（非空行、非注释行），明确禁止为追求代码简洁性而牺牲可读性的“代码高尔夫”行为。

有意者请将您的代码仓库发送给Maciej (maciej@odra.dev)，以获得免费且无义务的分析。

---

## 2. 高技能人才为何来德国后又离开

**原文标题**: Why skilled workers come to Germany and then leave again

**原文链接**: [https://www.dw.com/en/germany-migrants-skilled-workers-integration-labor-market-bureaucracy-language-housing/a-77853162](https://www.dw.com/en/germany-migrants-skilled-workers-integration-labor-market-bureaucracy-language-housing/a-77853162)

德国就业研究所 (IAB) 的一项研究探讨了技术工人移民德国后又常常离开的原因。这一决定是多方面的，受家庭原因、歧视经历以及官僚主义、住房和语言习得等政策影响因素驱动。

离开的移民通常更年轻，在德国居住时间较短，常有在国外的伴侣和子女，德语水平较低但英语流利。尽管60%的人返回原籍国，但40%的人则迁往其他欧洲国家，这凸显了德国在人才竞争中的地位。

官僚主义是主要的诟病，移民对入籍、许可、签证和学历认证的漫长办理时间，以及高额费用和缓慢的回复感到沮丧。这阻碍了他们的长期规划、就业机会和归属感。

语言能力是另一个关键因素；德语习得方面支持不足会显著提高离开率。此外，许多移民面临着大材小用的情况，工作与他们的资历不符。

政策制定者现在正致力于人才挽留。联邦就业局的集中式系统、州一级的移民管理机构以及计划中的联邦“工作与居留”机构等举措正在涌现。然而，挑战依然存在，包括公共机构的人员短缺以及缓慢、零散的数字化进程，缺乏全面的国家解决方案。对技术工人，特别是老年护理领域的需求依然强劲。

---

## 3. 小型AI模型在网络不可靠地区受青睐

**原文标题**: Small AI Models Gain Traction In places with unreliable networks

**原文链接**: [https://spectrum.ieee.org/small-language-models-ai-pharmaceuticals](https://spectrum.ieee.org/small-language-models-ai-pharmaceuticals)

小型人工智能模型，特别是TinyML（微型机器学习），正在全球范围内获得显著关注，尤其是在网络不可靠且缺乏数据中心基础设施的地区。这一趋势凸显了向更本地化、资源效率更高的人工智能解决方案的转变。巴西伊塔茹巴大学的研究员何塞·阿尔贝托·费雷拉 (José Alberto Ferreira) 就是这种应用的一个例子，他正在积极测试一个旨在生成心电图的TinyML模型，这展示了这些小型人工智能系统在挑战性环境中的实际应用和潜力。

---

## 4. 苹果将增加与博通的支出，用于生产额外数十亿枚美国芯片。

**原文标题**: Apple to increase spend with Broadcom to produce billions more U.S. chips

**原文链接**: [https://www.apple.com/newsroom/2026/07/apple-to-increase-spend-with-broadcom-to-produce-billions-more-us-chips/](https://www.apple.com/newsroom/2026/07/apple-to-increase-spend-with-broadcom-to-produce-billions-more-us-chips/)

2026年7月8日，苹果公司宣布与博通公司达成一项新的多年期协议，承诺投入超过300亿美元，用于为其产品设计和生产定制硅组件和无线连接技术。这项里程碑式的协议是苹果公司在其“美国制造计划”（AMP）下最大的一笔，预计将生产超过150亿枚美国制造的芯片，并支持数百个美国就业岗位。

这项承诺包括博通公司投入15亿美元的资本支出，用于扩建和现代化其位于科罗拉多州柯林斯堡的制造工厂。该工厂将负责生产先进的射频组件，例如FBAR滤波器，以及其他尖端无线连接技术。

苹果公司首席执行官蒂姆·库克强调了此次合作在加速美国制造业和创新方面的作用，并强调了柯林斯堡生产的组件的关键性。博通公司首席执行官霍克·谭（Hock Tan）对双方的长期合作以及在美国扩大制造足迹表示自豪。

这项举措是苹果公司更广泛承诺的一部分，即在四年内向美国经济投资6000亿美元，旨在促进制造业、创造就业和技术发展，并有助于在美国建立一个端到端的硅供应链。

---

## 5. GAO：能源部过早排除核清理的更经济方案

**原文标题**: GAO: DOE Is Prematurely Excluding Less Expensive Options for Nuclear Cleanup

**原文链接**: [https://www.gao.gov/products/gao-26-108193](https://www.gao.gov/products/gao-26-108193)

生成摘要时出错

---

## 6. 欧洲公司的网站大多由美国供应商提供服务。

**原文标题**: Europe's company websites are mostly served by US vendors

**原文链接**: [https://ciphercue.com/blog/european-web-hosting-vendor-share-2026](https://ciphercue.com/blog/european-web-hosting-vendor-share-2026)

CipherCue的一项研究分析了七个市场中19,450个欧洲公司网站，结果显示，总部位于美国的供应商为大多数或绝大多数主要网站提供服务。英国（67.5%）和荷兰（53.6%）显示美国供应商占主导地位，而意大利（48.4%）、西班牙（44.6%）和法国（44.2%）则将其视为最大的服务商群体。德国（31.0%）和波兰（18.8%）是例外，两国拥有强大的国内托管行业。

Cloudflare被确定为所有被调查国家中最大的面向互联网的基础设施供应商，超越所有其他美国、欧洲和国内提供商。亚马逊始终是第二大美国供应商。

该研究阐明，这是一项“供应商归属”研究，旨在识别响应顶级域名和www记录的DNS查询的自治系统（AS）运营商，因此它指明的是面向互联网的供应商（例如Cloudflare），而不一定是源托管提供商。

这种区别对于欧盟侧重于ICT供应链、第三国风险敞口和集中风险的监管制度至关重要。该研究不衡量物理数据中心位置、源托管或具体的欧盟子处理器安排。实际意义在于，主权讨论必须从面向互联网的层面开始，要求组织首先了解哪些供应商在其公共网络资产中处于前端。

---

## 7. Why we built yet another Postgres connection pooler

**原文标题**: Why we built yet another Postgres connection pooler

**原文链接**: [https://pgdog.dev/blog/why-yet-another-connection-pooler](https://pgdog.dev/blog/why-yet-another-connection-pooler)

PgDog is a new Postgres connection pooler designed to overcome the "leaky abstractions" of existing tools like PgBouncer and RDS Proxy, which often force users to alter application code and abandon core Postgres features.

Traditional poolers break session control (`SET` commands), leading to state "leaks" between clients. This can cause issues like incorrect `statement_timeout` or, critically, dysfunctional Row Level Security (RLS). PgDog addresses this by incorporating a built-in SQL parser that detects, extracts, and manages client-specific `SET` states. It efficiently updates the server's state when necessary, allowing full use of `SET` commands without performance degradation.

Another casualty of existing poolers is Postgres's `LISTEN/NOTIFY` publish/subscribe feature. PgDog restores this functionality by internally handling these commands, acting as a proxy broker while preserving transactional semantics. It uses Tokio's broadcast channels for inter-client communication within a process and a dedicated Postgres connection for inter-process messaging, making the feature "just work" at scale.

Architecturally, PgDog leverages Tokio's Rust async runtime with multithreaded workers. This allows a single PgDog process to utilize multiple CPUs, serving significantly more clients and queries per second than single-threaded, sharded solutions. This design improves connection utilization, handles burst traffic better without relying on slow autoscaling, and simplifies operational management compared to distributed proxy setups.

In essence, PgDog aims to provide robust Postgres scaling without demanding application changes or compromising on database features, offering an open-source, performant alternative proven in production.

---

## 8. 欧盟重启私信扫描规则仅一步之遥。

**原文标题**: EU now one step away from reviving private message scanning rules

**原文链接**: [https://cyberinsider.com/eu-now-one-step-away-from-reviving-private-message-scanning-rules/](https://cyberinsider.com/eu-now-one-step-away-from-reviving-private-message-scanning-rules/)

欧洲议会已批准一项紧急程序（331票赞成，304票反对），旨在加速立法，以恢复欧盟已失效的“聊天管控1.0”规则。这为2026年7月9日的一项决定性投票奠定了基础，该投票将决定在线平台是否可以再次自愿扫描用户的私人通讯，以查找儿童性虐待材料（CSAM）。

这项临时措施，正式名称为《欧盟条例(EU) 2021/1232》，此前允许Gmail和Facebook Messenger等服务自愿扫描消息，使其免受《电子隐私指令》的约束。在议会于3月否决延期后，该措施于2026年4月4日到期。然而，欧盟理事会此后又重新提出了一项包含实质相同条款的提案。

这项倡议与停滞不前的“聊天管控2.0”（即《儿童性虐待条例》或CSAR）是分开的，后者是一项旨在建立永久框架的长期谈判。关于广泛、无差别扫描与经司法授权的定向扫描之间存在分歧，尤其对于端到端加密服务而言。据报道，甚至理事会的法律服务部门也曾警告反对普遍的“自愿”扫描。

周四议会对该临时框架的投票，需要绝对多数（361票）才能否决或修改该提案；否则，理事会的文本预计将通过。欧盟目前正在推进两条平行的立法轨道：一条旨在临时恢复已失效的自愿扫描制度，另一条则针对更广泛、更具争议的永久性法规。

---

## 9. The Art of Computer Programming by Donald E. Knuth

**原文标题**: The Art of Computer Programming by Donald E. Knuth

**原文链接**: [https://www-cs-faculty.stanford.edu/~knuth/taocp.html](https://www-cs-faculty.stanford.edu/~knuth/taocp.html)

生成摘要时出错

---

## 10. GPT-5.6 Sol, along with Terra and Luna, will launch publicly this Thursday

**原文标题**: GPT-5.6 Sol, along with Terra and Luna, will launch publicly this Thursday

**原文链接**: [https://twitter.com/OpenAI/status/2074704958419792299](https://twitter.com/OpenAI/status/2074704958419792299)

生成摘要时出错

---

## 11. We're extending access to Fable 5 on all paid plans through July 12

**原文标题**: We're extending access to Fable 5 on all paid plans through July 12

**原文链接**: [https://twitter.com/claudeai/status/2074548242386178258](https://twitter.com/claudeai/status/2074548242386178258)

生成摘要时出错

---

## 12. OpenBSD has a use-after-free allowing local privilege escalation to root

**原文标题**: OpenBSD has a use-after-free allowing local privilege escalation to root

**原文链接**: [https://nvd.nist.gov/vuln/detail/cve-2026-57589](https://nvd.nist.gov/vuln/detail/cve-2026-57589)

生成摘要时出错

---

## 13. Show HN: Rowboat – Open-source, local-first alternative to Claude Desktop

**原文标题**: Show HN: Rowboat – Open-source, local-first alternative to Claude Desktop

**原文链接**: [https://github.com/rowboatlabs/rowboat](https://github.com/rowboatlabs/rowboat)

生成摘要时出错

---

## 14. Astro 7.0

**原文标题**: Astro 7.0

**原文链接**: [https://astro.build/blog/astro-7/](https://astro.build/blog/astro-7/)

生成摘要时出错

---

## 15. Jim's TrueType QR Code Font

**原文标题**: Jim's TrueType QR Code Font

**原文链接**: [https://github.com/jimparis/qr-font](https://github.com/jimparis/qr-font)

生成摘要时出错

---

## 16. FDA rejects petition to set PFAS limits in food

**原文标题**: FDA rejects petition to set PFAS limits in food

**原文链接**: [https://www.theguardian.com/us-news/2026/jul/08/us-food-and-drug-administration-rejects-petition-to-set-pfas-limits-in-food](https://www.theguardian.com/us-news/2026/jul/08/us-food-and-drug-administration-rejects-petition-to-set-pfas-limits-in-food)

生成摘要时出错

---

## 17. SWE-1.7 Reach Near GPT 5.5 and Opus Intelligence

**原文标题**: SWE-1.7 Reach Near GPT 5.5 and Opus Intelligence

**原文链接**: [https://cognition.com/blog/swe-1-7](https://cognition.com/blog/swe-1-7)

生成摘要时出错

---

## 18. LineageOS Statistics

**原文标题**: LineageOS Statistics

**原文链接**: [https://stats.lineageos.org](https://stats.lineageos.org)

生成摘要时出错

---

## 19. Cloudflare Meerkat - Globally distributed consensus

**原文标题**: Cloudflare Meerkat - Globally distributed consensus

**原文链接**: [https://blog.cloudflare.com/meerkat-introduction/](https://blog.cloudflare.com/meerkat-introduction/)

生成摘要时出错

---

## 20. Copy That Floppy – Cambridge guide for preserving data from fragile floppy disks

**原文标题**: Copy That Floppy – Cambridge guide for preserving data from fragile floppy disks

**原文链接**: [https://www.digipres.org/the-floppy-guide/](https://www.digipres.org/the-floppy-guide/)

生成摘要时出错

---

## 21. l: A new runtime for k and q

**原文标题**: l: A new runtime for k and q

**原文链接**: [https://lv1.sh/](https://lv1.sh/)

生成摘要时出错

---

## 22. Mark Zuckerberg's biggest legal nightmare yet could cost Meta $1.4T

**原文标题**: Mark Zuckerberg's biggest legal nightmare yet could cost Meta $1.4T

**原文链接**: [https://www.the-independent.com/tech/mark-zuckerberg-meta-fine-trillion-b3010281.html](https://www.the-independent.com/tech/mark-zuckerberg-meta-fine-trillion-b3010281.html)

生成摘要时出错

---

## 23. The revenge of the philosophy majors

**原文标题**: The revenge of the philosophy majors

**原文链接**: [https://www.nytimes.com/2026/07/05/business/philosophy-majors-ai-jobs.html](https://www.nytimes.com/2026/07/05/business/philosophy-majors-ai-jobs.html)

生成摘要时出错

---

## 24. Notes on Software Quality

**原文标题**: Notes on Software Quality

**原文链接**: [https://anthonyhobday.com/blog/20260410](https://anthonyhobday.com/blog/20260410)

生成摘要时出错

---

## 25. Python 3.14 compiled to metal – no interpreter

**原文标题**: Python 3.14 compiled to metal – no interpreter

**原文链接**: [https://github.com/can1357/pon](https://github.com/can1357/pon)

生成摘要时出错

---

## 26. NSA and IETF: Fairness

**原文标题**: NSA and IETF: Fairness

**原文链接**: [https://blog.cr.yp.to/20260706-fairness.html](https://blog.cr.yp.to/20260706-fairness.html)

生成摘要时出错

---

## 27. What Do We Know About the Microplastics Inside Us?

**原文标题**: What Do We Know About the Microplastics Inside Us?

**原文链接**: [https://e360.yale.edu/features/cassandra-rauert-interview](https://e360.yale.edu/features/cassandra-rauert-interview)

生成摘要时出错

---

## 28. Price per 1M tokens is meaningless

**原文标题**: Price per 1M tokens is meaningless

**原文链接**: [https://janilowski.pl/en/blog/2026/price-per-m-tokens/](https://janilowski.pl/en/blog/2026/price-per-m-tokens/)

生成摘要时出错

---

## 29. It seems that the age of reading might be a short anomaly in human history

**原文标题**: It seems that the age of reading might be a short anomaly in human history

**原文链接**: [https://www.theatlantic.com/magazine/2026/08/reading-crisis-postliterate-age/687618/](https://www.theatlantic.com/magazine/2026/08/reading-crisis-postliterate-age/687618/)

生成摘要时出错

---

## 30. Is The Economist Always Wrong?

**原文标题**: Is The Economist Always Wrong?

**原文链接**: [https://www.economist.com/interactive/finance-and-economics/2026/07/02/is-the-economist-always-wrong](https://www.economist.com/interactive/finance-and-economics/2026/07/02/is-the-economist-always-wrong)

生成摘要时出错

---

## 31. PlayStation can delete all your digital games after 3 years of inactivity (EU)

**原文标题**: PlayStation can delete all your digital games after 3 years of inactivity (EU)

**原文链接**: [https://www.flatpanelshd.com/news.php?subaction=showfull&id=1783340582](https://www.flatpanelshd.com/news.php?subaction=showfull&id=1783340582)

生成摘要时出错

---

## 32. Automating AI Away

**原文标题**: Automating AI Away

**原文链接**: [https://replicated.live/blog/away](https://replicated.live/blog/away)

生成摘要时出错

---

## 33. Better Auth is joining Vercel

**原文标题**: Better Auth is joining Vercel

**原文链接**: [https://better-auth.com/blog/better-auth-joins-vercel](https://better-auth.com/blog/better-auth-joins-vercel)

生成摘要时出错

---

## 34. Geosql: A Claude/Codex skill for geospatial data

**原文标题**: Geosql: A Claude/Codex skill for geospatial data

**原文链接**: [https://github.com/dekart-xyz/geosql](https://github.com/dekart-xyz/geosql)

生成摘要时出错

---

## 35. OpenSSH 10.4/10.4p1 Released

**原文标题**: OpenSSH 10.4/10.4p1 Released

**原文链接**: [https://www.openssh.org/txt/release-10.4](https://www.openssh.org/txt/release-10.4)

生成摘要时出错

---

## 36. YC CEO says he ships 37K LoC AI code per day. A developer looked under the hood

**原文标题**: YC CEO says he ships 37K LoC AI code per day. A developer looked under the hood

**原文链接**: [https://www.fastcompany.com/91520702/y-combinator-garry-tan-agentic-ai-social-media](https://www.fastcompany.com/91520702/y-combinator-garry-tan-agentic-ai-social-media)

生成摘要时出错

---

## 37. AI Meets Cryptography 1: What AI Found in Cloudflare's Circl

**原文标题**: AI Meets Cryptography 1: What AI Found in Cloudflare's Circl

**原文链接**: [https://blog.zksecurity.xyz/posts/circl-bugs/](https://blog.zksecurity.xyz/posts/circl-bugs/)

生成摘要时出错

---

## 38. Mapping homes you can buy from the US government for <$100k

**原文标题**: Mapping homes you can buy from the US government for <$100k

**原文链接**: [https://govauctions.app/research/cheapest-homes-in-america](https://govauctions.app/research/cheapest-homes-in-america)

生成摘要时出错

---

## 39. Kernel anti-cheat is an overreach

**原文标题**: Kernel anti-cheat is an overreach

**原文链接**: [https://nooneshappy.com/article/kernel-anti-cheat-is-an-overreach/](https://nooneshappy.com/article/kernel-anti-cheat-is-an-overreach/)

生成摘要时出错

---

## 40. Show HN: Microsoft releases Flint, a visualization language for AI agents

**原文标题**: Show HN: Microsoft releases Flint, a visualization language for AI agents

**原文链接**: [https://microsoft.github.io/flint-chart/#/](https://microsoft.github.io/flint-chart/#/)

生成摘要时出错

---

## 41. Show HN: Fast, native Mac file manager (filters, fuzzy find, 9 MB, no Electron)

**原文标题**: Show HN: Fast, native Mac file manager (filters, fuzzy find, 9 MB, no Electron)

**原文链接**: [https://whimfiles.com](https://whimfiles.com)

生成摘要时出错

---

## 42. Odin 1.0 Announcement

**原文标题**: Odin 1.0 Announcement

**原文链接**: [https://www.youtube.com/watch?v=dLPAqXi9In0](https://www.youtube.com/watch?v=dLPAqXi9In0)

生成摘要时出错

---

## 43. Show HN: PostgreSQL performance and cost across 23 EC2 instance types

**原文标题**: Show HN: PostgreSQL performance and cost across 23 EC2 instance types

**原文链接**: [https://postgres.saneengineer.com](https://postgres.saneengineer.com)

生成摘要时出错

---

## 44. Full Writeup of the Windows GDID

**原文标题**: Full Writeup of the Windows GDID

**原文链接**: [https://github.com/SmtimesIWndr/gdid-reversal](https://github.com/SmtimesIWndr/gdid-reversal)

生成摘要时出错

---

## 45. M/PC – A Concatenative OS

**原文标题**: M/PC – A Concatenative OS

**原文链接**: [https://wiki.xxiivv.com/site/m_pc.html](https://wiki.xxiivv.com/site/m_pc.html)

生成摘要时出错

---

## 46. Windows Drops Under 60% in Global Desktop OS Share for the First Time in Years

**原文标题**: Windows Drops Under 60% in Global Desktop OS Share for the First Time in Years

**原文链接**: [https://linuxiac.com/windows-drops-under-60-in-global-desktop-os-share-for-the-first-time-in-years/](https://linuxiac.com/windows-drops-under-60-in-global-desktop-os-share-for-the-first-time-in-years/)

生成摘要时出错

---

## 47. MacSurf 1.68 – NetSurf on OS 9 Released

**原文标题**: MacSurf 1.68 – NetSurf on OS 9 Released

**原文链接**: [https://github.com/mplsllc/macsurf/releases/tag/v1.86](https://github.com/mplsllc/macsurf/releases/tag/v1.86)

生成摘要时出错

---

## 48. Men's average testosterone levels have halved in last 50 years

**原文标题**: Men's average testosterone levels have halved in last 50 years

**原文链接**: [https://www.theguardian.com/society/2026/jul/07/mens-average-testosterone-levels-have-halved-in-last-50-years-say-scientists](https://www.theguardian.com/society/2026/jul/07/mens-average-testosterone-levels-have-halved-in-last-50-years-say-scientists)

生成摘要时出错

---

## 49. Poly/ML – A Standard ML Implementation

**原文标题**: Poly/ML – A Standard ML Implementation

**原文链接**: [https://github.com/polyml/polyml](https://github.com/polyml/polyml)

生成摘要时出错

---

## 50. Show HN: Chiptune Radio

**原文标题**: Show HN: Chiptune Radio

**原文链接**: [https://chiptune-radio.alephvoid.com/](https://chiptune-radio.alephvoid.com/)

生成摘要时出错

---

## 51. Meta says it's facing $1.4T in penalties in teen mental health case

**原文标题**: Meta says it's facing $1.4T in penalties in teen mental health case

**原文链接**: [https://nypost.com/2026/07/07/business/meta-says-its-facing-1-4t-in-penalties-in-teen-mental-health-case-sum-equal-to-tech-giants-valuation/](https://nypost.com/2026/07/07/business/meta-says-its-facing-1-4t-in-penalties-in-teen-mental-health-case-sum-equal-to-tech-giants-valuation/)

生成摘要时出错

---

## 52. AI: The ROI Runway Could Be Long Outside the Tech Sector

**原文标题**: AI: The ROI Runway Could Be Long Outside the Tech Sector

**原文链接**: [https://www.apollo.com/wealth/insights-news/insights/daily-spark/ai-the-roi-runway-could-be-long-outside-the-tech-sector](https://www.apollo.com/wealth/insights-news/insights/daily-spark/ai-the-roi-runway-could-be-long-outside-the-tech-sector)

生成摘要时出错

---

## 53. Tiny data centre used to heat public swimming pool

**原文标题**: Tiny data centre used to heat public swimming pool

**原文链接**: [https://www.bbc.com/news/technology-64939558](https://www.bbc.com/news/technology-64939558)

生成摘要时出错

---

## 54. Show HN: Docx-CLI: agents read/edit Word docs using 1/2 the time and tokens

**原文标题**: Show HN: Docx-CLI: agents read/edit Word docs using 1/2 the time and tokens

**原文链接**: [https://github.com/kklimuk/docx-cli](https://github.com/kklimuk/docx-cli)

生成摘要时出错

---

## 55. The space bit of SpaceX is worth $8 a share, says Morgan Stanley

**原文标题**: The space bit of SpaceX is worth $8 a share, says Morgan Stanley

**原文链接**: [https://www.ft.com/content/09a62ed4-16af-433c-adb7-c877d1975388](https://www.ft.com/content/09a62ed4-16af-433c-adb7-c877d1975388)

生成摘要时出错

---

## 56. Re: I'm Begging You to Leave Your AI Note-Taker at Home

**原文标题**: Re: I'm Begging You to Leave Your AI Note-Taker at Home

**原文链接**: [https://firesphere.dev/articles/yes-actually-i-do-fucking-mind](https://firesphere.dev/articles/yes-actually-i-do-fucking-mind)

生成摘要时出错

---

## 57. Beijing is looking at curbing overseas access to China's top AI models

**原文标题**: Beijing is looking at curbing overseas access to China's top AI models

**原文链接**: [https://www.reuters.com/world/beijing-is-looking-curbing-overseas-access-chinas-top-ai-models-sources-say-2026-07-07/](https://www.reuters.com/world/beijing-is-looking-curbing-overseas-access-chinas-top-ai-models-sources-say-2026-07-07/)

生成摘要时出错

---

## 58. The Making of Claude Code

**原文标题**: The Making of Claude Code

**原文链接**: [https://www.anthropic.com/features/making-of-claude-code](https://www.anthropic.com/features/making-of-claude-code)

生成摘要时出错

---

## 59. Acronym Fatigue Series Introduction: why I'm wary of acronyms

**原文标题**: Acronym Fatigue Series Introduction: why I'm wary of acronyms

**原文链接**: [https://devz.cl/posts/acryonym-fatigue-series-why-i-m-wary-of-engineering-acronyms/](https://devz.cl/posts/acryonym-fatigue-series-why-i-m-wary-of-engineering-acronyms/)

生成摘要时出错

---

## 60. How little exercise can you get away with?

**原文标题**: How little exercise can you get away with?

**原文链接**: [https://www.economist.com/science-and-technology/2026/07/03/how-little-exercise-can-you-get-away-with](https://www.economist.com/science-and-technology/2026/07/03/how-little-exercise-can-you-get-away-with)

生成摘要时出错

---

## 61. Reform UK leader 'in real trouble' against Count Binface

**原文标题**: Reform UK leader 'in real trouble' against Count Binface

**原文链接**: [https://www.mirror.co.uk/news/uk-news/nigel-farage-resigns-clacton-live-37401478](https://www.mirror.co.uk/news/uk-news/nigel-farage-resigns-clacton-live-37401478)

生成摘要时出错

---

## 62. Waymo reports teen riders for bad behavior and delivers them to the police

**原文标题**: Waymo reports teen riders for bad behavior and delivers them to the police

**原文链接**: [https://www.latimes.com/business/story/2026-07-07/waymo-reports-teen-riders-for-bad-behavior-delivers-them-to-police](https://www.latimes.com/business/story/2026-07-07/waymo-reports-teen-riders-for-bad-behavior-delivers-them-to-police)

生成摘要时出错

---

## 63. Woman's hip replacement disintegrates, causing metal poisoning

**原文标题**: Woman's hip replacement disintegrates, causing metal poisoning

**原文链接**: [https://arstechnica.com/health/2026/07/womans-puzzling-decline-turns-out-to-be-cobalt-poisoning-from-hip-replacement/](https://arstechnica.com/health/2026/07/womans-puzzling-decline-turns-out-to-be-cobalt-poisoning-from-hip-replacement/)

生成摘要时出错

---

## 64. How did Windows 95 decide that a setup program ran?

**原文标题**: How did Windows 95 decide that a setup program ran?

**原文链接**: [https://devblogs.microsoft.com/oldnewthing/20260707-00/?p=112508](https://devblogs.microsoft.com/oldnewthing/20260707-00/?p=112508)

生成摘要时出错

---

## 65. Show HN: Free Mermaid Diagram Editor

**原文标题**: Show HN: Free Mermaid Diagram Editor

**原文链接**: [https://moxiedocs.com/mermaid-diagram-editor](https://moxiedocs.com/mermaid-diagram-editor)

生成摘要时出错

---

## 66. An agent in 100 lines of Lisp

**原文标题**: An agent in 100 lines of Lisp

**原文链接**: [https://thebeach.dev/posts/lisp-agent/](https://thebeach.dev/posts/lisp-agent/)

生成摘要时出错

---

## 67. Treasury Has an Internal Report Warning About the Dangers of an AI Bubble

**原文标题**: Treasury Has an Internal Report Warning About the Dangers of an AI Bubble

**原文链接**: [https://www.notus.org/economy/treasury-internal-report-warning-dangers-ai-bubble](https://www.notus.org/economy/treasury-internal-report-warning-dangers-ai-bubble)

生成摘要时出错

---

## 68. Midtown Manhattan blocks evacuated after beams buckling at construction site

**原文标题**: Midtown Manhattan blocks evacuated after beams buckling at construction site

**原文链接**: [https://abcnews.com/US/midtown-manhattan-blocks-evacuated-after-beams-found-buckling/story?id=134549272](https://abcnews.com/US/midtown-manhattan-blocks-evacuated-after-beams-found-buckling/story?id=134549272)

生成摘要时出错

---

## 69. Almost all coders at Id Software have been fired, following Xbox reset

**原文标题**: Almost all coders at Id Software have been fired, following Xbox reset

**原文链接**: [https://xcancel.com/ScottApogee/status/2074198967550685268#m](https://xcancel.com/ScottApogee/status/2074198967550685268#m)

生成摘要时出错

---

## 70. An interactive explorer for Benford's Law across real datasets

**原文标题**: An interactive explorer for Benford's Law across real datasets

**原文链接**: [https://vatsalbakshi.com/blog/benfords-law/](https://vatsalbakshi.com/blog/benfords-law/)

生成摘要时出错

---

## 71. Show HN: Fortress – a stealth Chromium so your agents stop getting blocked

**原文标题**: Show HN: Fortress – a stealth Chromium so your agents stop getting blocked

**原文链接**: [https://github.com/tiliondev/fortress](https://github.com/tiliondev/fortress)

生成摘要时出错

---

## 72. Biff.graph: structure your Clojure codebase as a queryable graph

**原文标题**: Biff.graph: structure your Clojure codebase as a queryable graph

**原文链接**: [https://github.com/jacobobryant/biff/tree/v2.x/libs/graph](https://github.com/jacobobryant/biff/tree/v2.x/libs/graph)

生成摘要时出错

---

## 73. Learning another language appears to slow brain ageing by up to 13 years

**原文标题**: Learning another language appears to slow brain ageing by up to 13 years

**原文链接**: [https://www.theguardian.com/education/2026/jul/06/learning-another-language-appears-to-slow-brain-ageing-scientists-say](https://www.theguardian.com/education/2026/jul/06/learning-another-language-appears-to-slow-brain-ageing-scientists-say)

生成摘要时出错

---

## 74. List of European organizations that have banned personal messaging apps at work

**原文标题**: List of European organizations that have banned personal messaging apps at work

**原文链接**: [https://www.birdy.chat/blog/the-growing-list-of-european-organisations-that-ban-personal-messaging-apps-at-work](https://www.birdy.chat/blog/the-growing-list-of-european-organisations-that-ban-personal-messaging-apps-at-work)

生成摘要时出错

---

## 75. Honey, We Bought an AI Story

**原文标题**: Honey, We Bought an AI Story

**原文链接**: [https://www.bona-books.com/news/we-bought-an-ai-story](https://www.bona-books.com/news/we-bought-an-ai-story)

生成摘要时出错

---

## 76. Sodium-ion "salt" batteries will revolutionize electric-vehicle and grid storage

**原文标题**: Sodium-ion "salt" batteries will revolutionize electric-vehicle and grid storage

**原文链接**: [https://www.newscientist.com/article/2532997-salt-batteries-are-about-to-shake-up-evs-and-grid-storage/](https://www.newscientist.com/article/2532997-salt-batteries-are-about-to-shake-up-evs-and-grid-storage/)

生成摘要时出错

---

## 77. A verification loop 4x'd DeepSeek's intelligence, matching Opus at 1/7 the cost

**原文标题**: A verification loop 4x'd DeepSeek's intelligence, matching Opus at 1/7 the cost

**原文链接**: [https://ironbee.medium.com/what-a-verification-loop-adds-to-a-coding-agent-a-first-look-5049017e636e](https://ironbee.medium.com/what-a-verification-loop-adds-to-a-coding-agent-a-first-look-5049017e636e)

生成摘要时出错

---

## 78. Eliza Archaeology Project

**原文标题**: Eliza Archaeology Project

**原文链接**: [https://sites.google.com/view/elizaarchaeology/](https://sites.google.com/view/elizaarchaeology/)

生成摘要时出错

---

## 79. JPMorgan, BofA and Others Explore Buying Card Network to Raise Debit-Card Fees

**原文标题**: JPMorgan, BofA and Others Explore Buying Card Network to Raise Debit-Card Fees

**原文链接**: [https://www.wsj.com/finance/banking/jpmorgan-bank-of-america-and-other-banks-explore-a-deal-to-shake-up-payments-world-9d8639fb](https://www.wsj.com/finance/banking/jpmorgan-bank-of-america-and-other-banks-explore-a-deal-to-shake-up-payments-world-9d8639fb)

生成摘要时出错

---

## 80. Biohacker seeking immortality afflicted with incurable 'stomach eating' disease

**原文标题**: Biohacker seeking immortality afflicted with incurable 'stomach eating' disease

**原文链接**: [https://www.lifesitenews.com/news/biohacker-seeking-immortality-afflicted-with-incurable-stomach-eating-disease/](https://www.lifesitenews.com/news/biohacker-seeking-immortality-afflicted-with-incurable-stomach-eating-disease/)

生成摘要时出错

---

## 81. Show HN: Halo – open-source, tamper-evident runtime evidence for AI agents

**原文标题**: Show HN: Halo – open-source, tamper-evident runtime evidence for AI agents

**原文链接**: [https://github.com/bkuan001/halo-record](https://github.com/bkuan001/halo-record)

生成摘要时出错

---

## 82. Wikipedia Is Battling for the Soul of the Internet

**原文标题**: Wikipedia Is Battling for the Soul of the Internet

**原文链接**: [https://www.nytimes.com/2026/07/05/business/media/wikipedia-ai-elon-musk.html](https://www.nytimes.com/2026/07/05/business/media/wikipedia-ai-elon-musk.html)

生成摘要时出错

---

## 83. A bug which affected only left handed users

**原文标题**: A bug which affected only left handed users

**原文链接**: [https://shkspr.mobi/blog/2026/07/a-bug-which-only-affected-left-handed-users/](https://shkspr.mobi/blog/2026/07/a-bug-which-only-affected-left-handed-users/)

生成摘要时出错

---

## 84. Cloudflare Drop

**原文标题**: Cloudflare Drop

**原文链接**: [https://www.cloudflare.com/drop/](https://www.cloudflare.com/drop/)

生成摘要时出错

---

## 85. US manufacturers' energy costs soar because of AI data center demand

**原文标题**: US manufacturers' energy costs soar because of AI data center demand

**原文链接**: [https://arstechnica.com/tech-policy/2026/07/us-manufacturers-energy-costs-soar-because-of-ai-data-center-demand/](https://arstechnica.com/tech-policy/2026/07/us-manufacturers-energy-costs-soar-because-of-ai-data-center-demand/)

生成摘要时出错

---

## 86. Software Bonkers

**原文标题**: Software Bonkers

**原文链接**: [https://craigmod.com/essays/software_bonkers/](https://craigmod.com/essays/software_bonkers/)

生成摘要时出错

---

## 87. Majority of id software to be laid off by Microsoft

**原文标题**: Majority of id software to be laid off by Microsoft

**原文链接**: [https://bsky.app/profile/dark1x.bsky.social/post/3mpyugwk5yc27](https://bsky.app/profile/dark1x.bsky.social/post/3mpyugwk5yc27)

生成摘要时出错

---

