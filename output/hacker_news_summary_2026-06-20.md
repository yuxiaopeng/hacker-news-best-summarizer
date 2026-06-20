# Hacker News 热门文章摘要 (2026-06-20)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. Let's Encrypt 今天有90分钟的较高错误率。

**原文标题**: Let's Encrypt had a higher error rate for 90 minutes today

**原文链接**: [https://letsencrypt.status.io/#2026](https://letsencrypt.status.io/#2026)

2026年6月18日，Let's Encrypt 的生产API (acme-v02.api.letsencrypt.org) 经历了性能下降，导致部分客户端的错误率升高。该事件始于世界标准时间16:04（UTC），致使一些用户遇到400和500错误响应，尽管大多数客户端仍能成功。

该问题归因于一次上游网络事件，它中断了Let's Encrypt的两个高安全数据中心之间的流量。截至世界标准时间16:35（UTC），即初步报告发布后约31分钟，Let's Encrypt 成功重新路由了流量，使用户的成功率恢复正常。

尽管面向客户端的性能已解决，但服务仍以降低冗余的方式运行。截至2026年6月19日世界标准时间04:45（UTC），Let's Encrypt 仍在积极与其上游ISP合作，以全面识别并解决潜在的网络问题，从而恢复完全的冗余。

---

## 2. 如何喂养独裁者

**原文标题**: How to feed a dictator

**原文链接**: [https://www.theguardian.com/film/2026/jun/09/how-to-feed-a-dictator-film](https://www.theguardian.com/film/2026/jun/09/how-to-feed-a-dictator-film)

“如何喂养独裁者”是一部由安德鲁·尼尔执导，改编自维托尔德·沙布沃斯基著作的新纪录片，它审视了伊迪·阿明、萨达姆·侯赛因、金正日、波尔布特和奥古斯托·皮诺切特等残暴强人的私人厨师们的生活。影片探讨了这些人在一个危险世界中所面临的道德困境，在这个世界里，餐桌常常成为权力的舞台。

厨师们的经历大相径庭。阿明的前厨师查尔斯·奥通德·奥德拉，最初享受着富裕的生活，但后来却被老板的暴行所折磨，包括被命令烹饪人心，并因一个孩子的胃痛而面临死刑。金正日的披萨师埃尔曼诺·富尔拉尼斯，忍受着持续的监视。波尔布特的厨师吉奥·萨蒙，努力调和那位曾帮助过她的人与那位种族灭绝领导者的形象，她面临着一位在红色高棉统治下受苦的翻译带来的巨大挑战。与此形成鲜明对比的是，皮诺切特的厨师科科·帕切科以及萨达姆·侯赛因的一位匿名厨师，则始终忠心耿耿，对他们领导人骇人听闻的侵犯人权行为不屑一顾。

这部纪录片强调了“好差事”心态，即舒适和地位的诱惑常常成为他们扮演角色的正当理由。这些厨师享受着丰厚的待遇，而给他们的雇主下毒的想法是不可想象的，这既是因为独裁者核心圈内的深厚信任，也是因为他们与外界的隔绝。尼尔强调了“恶的平庸性”，即在暴政统治下，烹饪等日常行为也带上了邪恶的色彩。影片最终指出，个体通过共谋或自我保护，在维系威权政权中扮演着角色，给社会留下了复杂的遗产。

---

## 3. Datasette 应用：在 Datasette 中托管自定义 HTML 应用

**原文标题**: Datasette Apps: Host custom HTML applications inside Datasette

**原文链接**: [https://simonwillison.net/2026/Jun/18/datasette-apps/](https://simonwillison.net/2026/Jun/18/datasette-apps/)

Datasette App 于 2026 年 6 月 18 日发布，使得在 Datasette 实例中托管独立的 HTML+JavaScript 应用程序成为可能，这些应用程序在一个严格受限的 `<iframe>` 沙箱中运行。这些应用可以执行只读的 SQL 查询，并通过预配置的“存储查询”对 Datasette 数据执行写入操作。

安全是核心设计原则：应用程序通过 `<iframe> sandbox="allow-scripts allow-forms"` 和严格的 Content Security Policy (CSP) 头部进行隔离。这可以防止应用程序访问 cookies、localStorage 和外部 HTTP 请求，从而保护私有数据。SQL 操作的通信通过 `postMessage()` 和 `MessageChannel()` 安全处理。系统还提供查询和错误的可见日志，以辅助开发。

受 Claude Artifacts 和灵活的 HTML 工具启发，Datasette App 旨在将 Datasette 的后端能力与可定制的交互式前端结合起来。该插件有助于 AI 辅助；应用程序创建表单会为大型语言模型（LLMs）生成提示以构建新的应用程序，并且 Datasette Agent 可以管理它们。AI 还在开发和安全评估中发挥了关键作用，识别出一个与 CSP 允许列表相关的重大漏洞，这促使为受信任的用户设置了新的权限。

此版本标志着 Datasette 从只读数据服务器的演进，提供了一个更丰富的生态系统，用于创建自定义界面和可视化，以探索和交互数据。

---

## 4. 挪威为首个大型船舶隧道开绿灯

**原文标题**: Norway greenlights first full-scale ship tunnel

**原文链接**: [https://eandt.theiet.org/2026/06/18/norway-greenlights-world-s-first-full-scale-ship-tunnel](https://eandt.theiet.org/2026/06/18/norway-greenlights-world-s-first-full-scale-ship-tunnel)

挪威已最终批准斯塔德船舶隧道项目的建设，这是世界上首个全尺寸隧道，旨在让船只避开臭名昭著的危险斯塔德哈维特海域。挪威海岸管理局 (NCA) 宣布了这一批准，预计将于2026年开工，目标是在2030年完工。

这条1.7公里长的隧道将宽36米，高49米，能够容纳高达16,000总吨的船只，包括沿海快船和大型货船。它将连接莫尔德峡湾和谢德波伦，显著提高航行于暴露的斯塔德半岛区域的海上交通的安全性和效率。该区域以其狂风、强流和恶劣海况而闻名。

该项目预计耗资约39亿挪威克朗（约合2.9亿英镑），旨在创造一个更安全、更可预测的通道，缩短航程时间，并为挪威西海岸的商业和客运开辟新的机遇。尽管已经为船只修建了较小的运河，斯塔德船舶隧道却是首个为大型船只设计的隧道。其设计包括创新的爆破技术来开凿巨大的隧道，以及复杂的交通管理系统以确保安全通行。

---

## 5. 大语言模型现在变得复杂了

**原文标题**: LLMs Are Complicated Now

**原文链接**: [https://ianbarber.blog/2026/06/19/llms-are-complicated-now/](https://ianbarber.blog/2026/06/19/llms-are-complicated-now/)

LLM，曾经以简洁的Transformer堆栈为特征，如今已变得显著更加复杂，这反映了推荐系统（recsys）的演进路径。这种复杂性的增加源于多样化的注意力变体（例如，查询分组、滑动窗口）、专家混合模型（MoE）从前馈层扩展到注意力块和残差连接、视觉和音频编码器的集成，以及多GPU推理的开销。

就像推荐系统一样，从简单的神经网络演变为复杂的系统，这种演变是由对能力和推理效率的需求驱动的，LLM也面临着类似的困境。尽管人们可能倾向于相信AI智能体将自动优化这些复杂的架构，但仅仅依赖它们是存在问题的。生成最优融合的核函数需要一个固定且可验证的基线来确保正确性。然而，随着性能改进变得举足轻重并对实际部署至关重要，纯粹的概念模型与优化后的生产就绪模型之间的差距缩小，这使得评估新的、未优化的变体变得困难。

当未经优化的新想法显得远不如高度融合的现有方案时，研究迭代循环就会受阻。手动融合新组件耗时费力，而纯粹的自动生成又缺乏关键的基线。文章认为，唯一可行的解决方案是从一开始就进行可组合性设计。PyTorch的FlexAttention便体现了这种方法，它使用Triton模板为一类注意力操作生成核函数，由于其固有的可组合性和可验证性，使得探索可以在性能影响最小的情况下进行。Andrej Karpathy等专家也强调了这种将架构精髓化并确保可组合性的原则，认为它对于推进前沿AI研究至关重要。

---

## 6. 意想不到的负载均衡系统经济学

**原文标题**: Surprising economics of load-balanced systems

**原文链接**: [https://brooker.co.za/blog/2020/08/06/erlang.html](https://brooker.co.za/blog/2020/08/06/erlang.html)

Marc Brooker的《负载均衡系统的惊人经济学》探讨了在一个M/M/c排队系统中，当服务器数量(c)增加且每个服务器负载保持不变时，客户端观察到的延迟如何变化。与直觉相反的是，平均请求时间并非保持不变，而是迅速下降，渐近地接近一秒钟的基本服务时间。

这个惊人的结果可以通过爱尔兰C公式来解释。随着“c”的增长，即使总负载按比例增加，入站请求被排队（从而经历额外延迟）的概率也会显著下降。例如，将服务器和总负载翻倍可以大幅减少排队请求的百分比。这意味着一个更大的系统天生就能处理更高比例的无延迟流量。

仿真进一步证实，这种改进不仅限于平均值；高百分位数（如p99和p99.9）也显示出类似的积极趋势。这对云服务和提供商具有重大的经济意义：更大的“c”可以在相同利用率下实现更好的延迟，或者在相同延迟下实现更好的利用率，同时保持每个服务器相同的吞吐量。这种效率增益尤其有益，因为它即使在适度的服务器数量下也能显著累积，使其成为分布式系统扩展反而能简化问题的罕见案例。尽管M/M/c的假设是理想化的，但其基本原理仍然成立。

---

## 7. So You Want to Define a Well-Known URI

**原文标题**: So You Want to Define a Well-Known URI

**原文链接**: [https://mnot.net/blog/2026/well_known_uris](https://mnot.net/blog/2026/well_known_uris)

马克·诺丁汉，知名URI（Well-Known URI）规范的合著者和指定专家，阐明了它们的恰当用法。知名URI最适用于客户端已知源（网站）并需要高效发现或与整个网站相关的事物进行交互的场景，例如用于访问策略的`robots.txt`或全站范围的密码更改机制。

如果仅仅为了赋予合法性、促进采用，或在能提供完整URL时用作URL缩短器，那么它们就是错误的工具。将它们用作快捷方式会产生僵化，将服务锁定为与网站的1:1关系，从而阻碍部署灵活性。

诺丁汉强调了常见陷阱：
*   **发现：** 假设存在一个清晰的“网站”进行发现是有问题的。客户端可能从子域名（例如`login.example.com`）开始，而知名位置却位于顶级域名（例如`example.com`），这需要仔细设计以实现可靠的主机名解析。
*   **内容元数据：** 集中式元数据（如`robots.txt`）对于托管多个发布者的网站来说具有挑战性，因为它在便利性和粒度之间产生了冲突，往往需要并行的元数据机制。

其他考虑因素包括规划现有固定位置的过渡、明确列出除HTTP/HTTPS之外所有适用的URL方案，以及确保在官方注册表中正确注册。知名URI解决了特定的问题，而滥用它们可能会引入不必要的复杂性。

---

## 8. Ubisoft co-founder Claude Guillemot has died in a plane crash

**原文标题**: Ubisoft co-founder Claude Guillemot has died in a plane crash

**原文链接**: [https://www.reuters.com/world/ubisofts-co-founder-claude-guillemot-dies-plane-crash-2026-06-20/](https://www.reuters.com/world/ubisofts-co-founder-claude-guillemot-dies-plane-crash-2026-06-20/)

生成摘要时出错

---

## 9. 海洋观测计划最新进展

**原文标题**: Update on Ocean Observatories Initiative

**原文链接**: [https://www.nsf.gov/news/update-ocean-observatories-initiative](https://www.nsf.gov/news/update-ocean-observatories-initiative)

The U.S. National Science Foundation (NSF) announced on June 18, 2026, a significant update to its Ocean Observatories Initiative (OOI) in response to stakeholder concerns about data reliance.

Effective immediately, NSF will cease any further removal or descoping of equipment from the remaining OOI arrays and will continue operations, including planned maintenance. While the Endurance Array has already been removed, NSF is developing plans to redeploy it after servicing.

Moving forward, NSF will issue a "Dear Colleague Letter" to gather stakeholder input. Additionally, an expert panel will be convened to assess observational needs, evaluate available data sources, consider responses to the letter, and help identify a sustainable path for NSF’s ocean observing systems. NSF reaffirmed its commitment to ocean sciences, responsible stewardship of its research infrastructure, and supporting its dependent stakeholders.

---

## 10. Iran requires insurance on ships using Strait of Hormuz, fees likely to follow

**原文标题**: Iran requires insurance on ships using Strait of Hormuz, fees likely to follow

**原文链接**: [https://www.lloydslist.com/LL1157571/Iran-imposes-mandatory-insurance-on-ships-transiting-Strait-of-Hormuz-with-fees-likely-to-follow](https://www.lloydslist.com/LL1157571/Iran-imposes-mandatory-insurance-on-ships-transiting-Strait-of-Hormuz-with-fees-likely-to-follow)

生成摘要时出错

---

## 11. From PGP to Mythos: a brief history of export controls that didn't stop anyone

**原文标题**: From PGP to Mythos: a brief history of export controls that didn't stop anyone

**原文链接**: [https://techcrunch.com/2026/06/19/encryption-spyware-and-now-mythos-history-shows-why-cyber-export-control-doesnt-work/](https://techcrunch.com/2026/06/19/encryption-spyware-and-now-mythos-history-shows-why-cyber-export-control-doesnt-work/)

生成摘要时出错

---

## 12. AURpocalypse now: a look at the recent AUR attacks

**原文标题**: AURpocalypse now: a look at the recent AUR attacks

**原文链接**: [https://lwn.net/SubscriberLink/1077619/f7b07c5489fdd43a/](https://lwn.net/SubscriberLink/1077619/f7b07c5489fdd43a/)

The Arch User Repository (AUR) has recently experienced a large-scale, sustained attack where malicious actors created new accounts to adopt orphaned packages and inject malware. Starting around May 27, 2026, attackers pushed updates installing malicious npm packages like `crypto-javascript` and `atomic-lockfile`, exfiltrating sensitive user data. Over 1,500 packages were affected, marking this as a significantly larger incident than previous attacks.

The AUR's open-door policy facilitates these vulnerabilities: there's no formal review process for packages or updates, and any registered user can easily adopt orphaned packages. Unlike services such as Fedora's Copr, AUR packages reside in a single namespace, making ownership changes simple to abuse. While users are warned to "use at their own risk" and review PKGBUILDs, this often doesn't happen, especially during updates.

In response, AUR new-user registration was temporarily disabled multiple times. The attackers also attempted to obfuscate their install commands. Discussions for long-term solutions include AI-powered threat detection, locking orphaned packages until proper adoption requests are reviewed, or integrating "loud warnings" into AUR helpers for adopted packages. However, concerns exist about discouraging legitimate contributions and the ability of simple scanning to keep pace with evolving attacker tactics. The incident highlights the inherent challenges of securing large, trust-based community repositories.

---

## 13. DOS Game "F-15 Strike Eagle II" reversing project needs DOS test pilots

**原文标题**: DOS Game "F-15 Strike Eagle II" reversing project needs DOS test pilots

**原文链接**: [https://neuviemeporte.github.io/f15-se2/2026/06/20/needyou.html](https://neuviemeporte.github.io/f15-se2/2026/06/20/needyou.html)

生成摘要时出错

---

## 14. SMPTE Makes Its Standards Freely Accessible

**原文标题**: SMPTE Makes Its Standards Freely Accessible

**原文链接**: [https://www.smpte.org/blog/smpte-makes-its-standards-freely-accessible-openingstandards-library-to-the-global-media-technology-community](https://www.smpte.org/blog/smpte-makes-its-standards-freely-accessible-openingstandards-library-to-the-global-media-technology-community)

生成摘要时出错

---

## 15. Companies rein in AI usage as costs strain budgets

**原文标题**: Companies rein in AI usage as costs strain budgets

**原文链接**: [https://www.ft.com/content/1d37cc08-e0aa-45a4-a45d-4ad282529314](https://www.ft.com/content/1d37cc08-e0aa-45a4-a45d-4ad282529314)

生成摘要时出错

---

## 16. Zenzizenzizenzic

**原文标题**: Zenzizenzizenzic

**原文链接**: [https://en.wikipedia.org/wiki/Zenzizenzizenzic](https://en.wikipedia.org/wiki/Zenzizenzizenzic)

生成摘要时出错

---

## 17. Lithuanian startup launches open-source network to detect Shahed-type drones

**原文标题**: Lithuanian startup launches open-source network to detect Shahed-type drones

**原文链接**: [https://www.lrt.lt/en/news-in-english/19/2965205/lithuanian-startup-launches-open-source-network-to-detect-shahed-type-drones](https://www.lrt.lt/en/news-in-english/19/2965205/lithuanian-startup-launches-open-source-network-to-detect-shahed-type-drones)

生成摘要时出错

---

## 18. Temporary Cloudflare accounts for AI agents

**原文标题**: Temporary Cloudflare accounts for AI agents

**原文链接**: [https://blog.cloudflare.com/temporary-accounts/](https://blog.cloudflare.com/temporary-accounts/)

生成摘要时出错

---

## 19. The European Social Stack

**原文标题**: The European Social Stack

**原文链接**: [https://european.social](https://european.social)

生成摘要时出错

---

## 20. Bootimus – A Self-Contained PXE and HTTP Boot Server

**原文标题**: Bootimus – A Self-Contained PXE and HTTP Boot Server

**原文链接**: [https://bootimus.com](https://bootimus.com)

Bootimus is described as a self-contained PXE and HTTP Boot Server, designed for simplicity and ease of use. Its core feature is being a single Go binary that embeds all necessary components, including iPXE, a web user interface, SQLite database, and all other assets. This architecture eliminates runtime dependencies, allowing for extremely straightforward deployment—users can simply copy (scp) the binary and run it without needing to install additional software.

---

## 21. The UK's new under-16 social media ban will cause more harm than it prevents

**原文标题**: The UK's new under-16 social media ban will cause more harm than it prevents

**原文链接**: [https://www.eff.org/deeplinks/2026/06/uks-new-under-16-social-media-ban-will-cause-more-harm-it-prevents](https://www.eff.org/deeplinks/2026/06/uks-new-under-16-social-media-ban-will-cause-more-harm-it-prevents)

生成摘要时出错

---

## 22. Zork name origin got an update on Wikipedia

**原文标题**: Zork name origin got an update on Wikipedia

**原文链接**: [https://www.dpolakovic.space/blogs/zork-part2#update](https://www.dpolakovic.space/blogs/zork-part2#update)

生成摘要时出错

---

## 23. Fable Converted Pylint to Rust

**原文标题**: Fable Converted Pylint to Rust

**原文链接**: [https://pypi.org/project/prylint/](https://pypi.org/project/prylint/)

生成摘要时出错

---

## 24. Show HN: StartupWiki – A Free Alternative to Crunchbase

**原文标题**: Show HN: StartupWiki – A Free Alternative to Crunchbase

**原文链接**: [https://startupwiki.tech/](https://startupwiki.tech/)

生成摘要时出错

---

## 25. Russell Vought is going to destroy American Science

**原文标题**: Russell Vought is going to destroy American Science

**原文链接**: [https://elizabethginexi.substack.com/p/summary-of-key-changes-in-ombs-proposed](https://elizabethginexi.substack.com/p/summary-of-key-changes-in-ombs-proposed)

生成摘要时出错

---

## 26. UHF X11: X11 Built for VisionOS and Apple Vision Pro

**原文标题**: UHF X11: X11 Built for VisionOS and Apple Vision Pro

**原文链接**: [https://www.lispm.net/apps/uhf-x11/](https://www.lispm.net/apps/uhf-x11/)

生成摘要时出错

---

## 27. Leave a Trace

**原文标题**: Leave a Trace

**原文链接**: [https://www.jakeworth.com/posts/leave-a-trace](https://www.jakeworth.com/posts/leave-a-trace)

生成摘要时出错

---

## 28. The ability to regrow body parts is dormant in mammals, not lost

**原文标题**: The ability to regrow body parts is dormant in mammals, not lost

**原文链接**: [https://www.sciencedaily.com/releases/2026/06/260617032207.htm](https://www.sciencedaily.com/releases/2026/06/260617032207.htm)

生成摘要时出错

---

## 29. A record 242 US cities now have starter homes that cost $1M

**原文标题**: A record 242 US cities now have starter homes that cost $1M

**原文链接**: [https://investors.zillowgroup.com/news-and-events/news/news-details/2026/A-record-242-US-cities-now-have-starter-homes-that-cost-1M/default.aspx](https://investors.zillowgroup.com/news-and-events/news/news-details/2026/A-record-242-US-cities-now-have-starter-homes-that-cost-1M/default.aspx)

生成摘要时出错

---

