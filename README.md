# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-06-20.md)

*最后自动更新时间: 2026-06-20 20:32:01*
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

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 2 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 3 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 4 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 5 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 6 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 7 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 8 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 9 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 10 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 11 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 12 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 13 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 14 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 15 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 16 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 17 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 18 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 19 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 20 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 21 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 22 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 23 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 24 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 25 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 26 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 27 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 28 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 29 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 30 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 31 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 32 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 33 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 34 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 35 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 36 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 37 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 38 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 39 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 40 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 41 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 42 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 43 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 44 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 45 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 46 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 47 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 48 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 49 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 50 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 51 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 52 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 53 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 54 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 55 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 56 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 57 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 58 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 59 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 60 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 61 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 62 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 63 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 64 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 65 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 66 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 67 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 68 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 69 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 70 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 71 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 72 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 73 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 74 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 75 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 76 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 77 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 78 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 79 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 80 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 81 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 82 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 83 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 84 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 85 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 86 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 87 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 88 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 89 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 90 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 91 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 92 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 93 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 94 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 95 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 96 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 97 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 98 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 99 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 100 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 101 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 102 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 103 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 104 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 105 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 106 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 107 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 108 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 109 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 110 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 111 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 112 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 113 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 114 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 115 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 116 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 117 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 118 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 119 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 120 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 121 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 122 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 123 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 124 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 125 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 126 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 127 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 128 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 129 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 130 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 131 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 132 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 133 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 134 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 135 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 136 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 137 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 138 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 139 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 140 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 141 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 142 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 143 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 144 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 145 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 146 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 147 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 148 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 149 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 150 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 151 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 152 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 153 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 154 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 155 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 156 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 157 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 158 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 159 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 160 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 161 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 162 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 163 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 164 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 165 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 166 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 167 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 168 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 169 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 170 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 171 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 172 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 173 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 174 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 175 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 176 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 177 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 178 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 179 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 180 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 181 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 182 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 183 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 184 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 185 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 186 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 187 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 188 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 189 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 190 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 191 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 192 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 193 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 194 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 195 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 196 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 197 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 198 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 199 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 200 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 201 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 202 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 203 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 204 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 205 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 206 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 207 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 208 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 209 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 210 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 211 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 212 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 213 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 214 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 215 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 216 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 217 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 218 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 219 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 220 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 221 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 222 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 223 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 224 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 225 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
