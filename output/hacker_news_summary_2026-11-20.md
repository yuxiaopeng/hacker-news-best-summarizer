# Hacker News 热门文章摘要 (2026-11-20)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. Nginx 未经身份验证的远程代码执行

**原文标题**: Unauthenticated remote code execution in Nginx

**原文链接**: [https://www.wiz.io/blog/nginx-http2-rce-vulnerabilities](https://www.wiz.io/blog/nginx-http2-rce-vulnerabilities)

Wiz Research、Ikotas Labs、Metnir、Rapid7 和 Xint 独立发现了 NGINX 中两个关键的、未经身份验证的远程代码执行 (RCE) 漏洞：CVE-2026-123633 (HTTP/2 use-after-free) 和 CVE-2026-123007 (HTTP/2 send_window 整数下溢)。两者的 CVSS 4.0 评分均为 9.2。

这些缺陷，其中 CVE-2026-123007 影响的 NGINX 版本可追溯至 1.9.5 (2015 年)，允许攻击者入侵 NGINX 服务器，执行任意代码，窃取数据，篡改网站或中断服务。关键是，它们影响的是 NGINX 本身，而非后端应用程序，并且需要启用 HTTP/2。

此次发现的一个重要方面是 AI 工具 (如 Wiz Atlas、Gemini 4 Carbon 和 ChatGPT 5.6 Sol) 在揭示这些复杂且长期存在的内存安全问题中所发挥的作用。这标志着一个新时代的到来，AI 降低了发现此类漏洞的门槛，加速了风险向实际威胁的转化。

NGINX 的母公司 F5 已被负责任地告知，促成了 2026 年 11 月 18 日的协调安全发布。强烈建议各组织识别受影响的 NGINX 部署并立即更新到最新的修补版本。如果无法立即升级，建议暂时禁用 HTTP/2。

---

## 2. 双子座4 霓虹

**原文标题**: Gemini 4 Neon

**原文链接**: [https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-4-neon/](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-4-neon/)

Google DeepMind于2026年11月18日推出了一款新的前沿级AI模型——Gemini 4 Neon。该模型专为在复杂软件工程、知识工作和科学领域中快速、端到端地完成任务而设计，展现出高超的智能，在Artificial Analysis智能指数中排名第三，在Vals指数中排名第二。它具有卓越的可控性、多步指令遵循能力，以及谷歌迄今最低的幻觉率。

Neon提供了显著的成本效益，输入代币每百万美元3美元，输出代币每百万美元15美元，并拥有100万代币的上下文窗口。它每项任务的成本比Gemini 4 Carbon低32%，比其他同等智能水平的顶级模型便宜50-80%。

该模型在多个领域表现出色：
*   **企业领域：** 在法律研究和税务代理基准测试中排名第一，并在金融、会计和自动化基准测试中处于领先地位。
*   **编码：** 在Artificial Analysis编码智能体指数中排名第一，擅长多文件调试、重构和长期运行的智能体工作流，在Google Antigravity内部的SWE-sweep上取得了最先进的成果。
*   **网络防御：** 生成更安全的代码，在渗透测试中达到最先进水平，并在漏洞发现、验证和修补方面展现出前沿水平的性能。防御者可通过Fairwind计划获取。
*   **科学推理：** 在Terminal-Bench Science和RiemannBench等基准测试中表现同类最佳。

安全性至关重要，Neon对滥用和提示注入保持强大的防护，同时推动模型对齐和规范的智能体行为。它在Gray Swan的间接提示注入基准测试中实现了0.0%的攻击成功率。

Gemini 4 Neon今天正通过Gemini API、Google AI Studio、企业版Gemini以及Google Antigravity和Gemini应用中的Google AI Pro/Ultra订阅者全面推出。它在Gemini 4系列中，定位介于高容量的Carbon和日常使用的Hydrogen之间，在深度和效率之间取得了平衡。

---

## 3. Anthropic纳斯达克首秀

**原文标题**: Anthropic’s Nasdaq debut

**原文链接**: [https://www.reuters.com/business/finance/anthropics-historic-debut-put-ais-promise-peril-wall-st-test-2026-11-19/](https://www.reuters.com/business/finance/anthropics-historic-debut-put-ais-promise-peril-wall-st-test-2026-11-19/)

无法访问文章链接。

---

## 4. AI正在扼杀All About Berlin

**原文标题**: AI is killing All About Berlin

**原文链接**: [https://nicolasbouliane.com/blog/death-by-ai](https://nicolasbouliane.com/blog/death-by-ai)

“All About Berlin”网站的作者报告称，由于谷歌AI概览（Google AI Overviews），其网站流量损失了70-75%，情况十分严重。该网站成立于2017年，自2020年以来一直是他们的主要收入来源。此前，谷歌搜索会直接链接到他们的网站；现在，用户首先看到广告，然后是一个AI生成的答案（通常是根据该网站内容训练的），最后才是一个指向原始网站的链接，这大大降低了点击量。

此次流量骤降使其难以资助他们的工作，可能迫使他们寻求其他收入来源，并分散了他们用于创建新指南的时间。除了财务压力之外，作者还表达了深刻的个人影响：当内容被AI吸收后，他们失去了自己的声音、受众以及精心选择的词语的意义。此前证实他们八年努力的用户个人联系和政府机构的认可也正在减弱。

作者表示，这并非孤立事件，许多其他网站所有者也私下报告了类似的困境，导致一些人选择对内容收费或完全放弃他们的网站。他们警告说情况将会恶化，并引用了谷歌最近的声明：AI生成的答案将完全取代搜索结果并包含广告，从而创造一个由“带广告的聊天框”而非直接网站访问主导的未来互联网。作者质疑“All About Berlin”在这个未来中的地位，并邀请其他受影响者进行联系，同时指出广泛的讨论以及StackOverflow等网站报告的类似流量下降情况。

---

## 5. 我们需要有担当的聪明人。

**原文标题**: We need smart people who give a shit

**原文链接**: [https://violetpixel.com/blog/2026-11-17-we-need-smart-people-who-give-a-shit/](https://violetpixel.com/blog/2026-11-17-we-need-smart-people-who-give-a-shit/)

文章指出，世界各地复杂且常有缺陷的系统——从银行（如ACH）到关键基础设施——之所以能可靠运作，是因为有“那些有担当、有智慧的人”在维护。这些人对系统有着深入的了解，并有决心去修补、绕过或手动解决问题。最近发生在各大机构（如Microsoft 365、空中交通管制、主要银行、苹果）的普遍系统故障表明，这些关键专家正严重短缺。

历史上，出于必要性，资本主义容纳了这些技能娴熟的个体。然而，随着生成式AI的兴起，领导层和管理层——他们往往脱离技术实际——错误地认为AI可以取代人类的专业知识。他们将AI视为一种更便宜、不知疲倦的替代品，能够提供类似“产出”。作者断言，这是一个危险的误解：生成式AI缺乏真正的智能、关心，也无法察觉细微问题、整合信息、处理边缘情况，或提供真正将复杂系统维系在一起的关键“粘合剂”。它看似的智能只是一种假象。

因此，许多“有担当、有智慧的人”被解雇或权力被削弱，他们的职责被简化为“照看大型语言模型（LLMs）”。这种转变侵蚀了他们深厚的知识、主人翁意识和内在动力。文章总结道，我们正在步入一个脆弱系统日益由不那么聪明、不那么上心的人来运行的世界，这必然会导致更广泛的故障。这代表着资本主义的“烫手炉子时刻”，一个正在以所有人的利益为代价学习的惨痛教训。

---

## 6. 德意志银行内幕

**原文标题**: Inside Deutsche Bank

**原文链接**: [https://www.inside-db.com/](https://www.inside-db.com/)

一项基于超过1500万份内部文件泄露的全球重大调查“德意志银行内幕”，揭露了这家金融巨头的有问题文化、系统性盲点以及将利润置于合规之上的做法。这些揭露揭示了该银行运营中广泛存在的非法活动和道德违规行为。

主要发现包括德意志银行涉嫌协助与哥伦比亚虚拟性产业、人口贩卖和剥削相关的洗钱活动。据报道，它因有利可图的金融关系而破坏了其气候承诺，并帮助沙特王子穆罕默德·本·纳伊夫建立离岸结构。该银行不顾警告保护了俄罗斯寡头的利润，并卷入涉及一家匈牙利银行和特朗普旗下公司的洗钱计划，以及与刘特佐和杰弗里·爱泼斯坦相关的可疑交易。

进一步披露的细节显示，德意志银行资助了战争产业，包括向巴勒斯坦平民和“高风险”国家提供武器。该银行因与一位卡塔尔王室成员的交易而受到审查，并因未能标记可疑交易（包括来自斯洛伐克总理儿子账户的交易）而受到制裁。这些泄露描绘了一幅景象：一个机构持续在道德和法律边缘运作，难以维持财务控制。

---

## 7. 谷歌AI答案使搜索流量下降40%

**原文标题**: Google's AI answers reducing search traffic by 40%

**原文链接**: [https://revscope.co/blog/search-seo-geo-2026/](https://revscope.co/blog/search-seo-geo-2026/)

A November 2026 report reveals Google's AI Overviews are significantly reducing search traffic to websites, cutting clicks by approximately 40% when present, according to a randomized experiment. These AI summaries now appear on over 60% of US keywords, up from 6% two years prior, contributing to an estimated 18.5% overall loss in organic clicks and a drastic 58% drop in desktop click-through rates for the first organic result.

Users are increasingly finding answers directly within AI Overviews, causing searches ending without an outbound click to rise from 54% to 73%. While traditional SEO is still crucial, a top ranking now yields 40% fewer visits where an Overview appears.

Generative Engine Optimization (GEO) aims to get content cited in AI answers. This involves standard SEO practices, being present on third-party sites frequently cited by AI (e.g., YouTube, Reddit, Wikipedia), and crafting easily quotable content. Studies show a moderate correlation between a site's link profile and AI citations. Page-level tactics like including the current year in titles, using tables of contents, and citing sources increase citation likelihood. Google, however, disputes traffic decline and states no special optimization is needed beyond standard indexability, and proposed solutions like llms.txt files show no measurable effect.

---

## 8. DNS解析器不应成为打击盗版之处。

**原文标题**: DNS resolvers are the wrong place to fight piracy

**原文链接**: [https://techstackups.com/articles/quad9-leaves-france-dns-blocking/](https://techstackups.com/articles/quad9-leaves-france-dns-blocking/)

Quad9，一家以恶意软件拦截和隐私保护功能著称的瑞士非营利DNS解析器（9.9.9.9），将于2026年11月24日停止在法国的运营。这一决定源于其因拒绝为beIN Sports拦截盗版体育直播域名而被巴黎法院处以罚款，且有大量类似案件正在审理中。Quad9的撤离，被Cloudflare称为“煤矿里的金丝雀”，凸显了中立互联网基础设施面临日益增长的法律压力。

问题的根源在于法国的《L.333-10条》，该条款允许体育版权方获得针对“任何能够帮助阻止侵权行为的人”的动态拦截令，明确包括DNS解析器。这导致了目标范围的扩大，此前已于2024年迫使思科的OpenDNS撤出法国。Quad9的首席技术官称这种自动化实时拦截系统“鲁莽且危险”。

Quad9辩称其无法通过全球拦截来遵守规定，因为这将使法国法院能够左右全球的互联网访问。地理位置拦截在技术上并不可靠，此前在德国的案件中也曾失败，导致罚款。对于一家非营利组织而言，持续的法律战成本构成了“生存威胁”。

文章指出，DNS拦截无效且有害：它无法移除内容，用户可轻易绕过，是一种造成附带损害（例如谷歌云盘在意大利被拦截）的笨拙工具，且对用户不透明。统计数据显示，拦截数量的增长速度快于盗版萎缩的速度。

法国的策略损人害己：用户失去恶意软件保护，依赖Quad9的关键基础设施面临无声中断，隐私保护型解析器市场萎缩，讽刺的是，在将欧洲非营利组织赶走的同时，拥有更多资源的美国科技巨头却得以留下，从而损害了法国的数字主权。作者总结道，执法应针对内容托管方，而非中立的中间服务商。

---

## 9. 欧盟委员会如何向超过4万名员工推广Matrix

**原文标题**: How the European Commission rolled out Matrix to more than 40k staff

**原文链接**: [https://element.io/blog/how-the-european-commission-rolled-out-matrix-to-more-than-40-000-staff/](https://element.io/blog/how-the-european-commission-rolled-out-matrix-to-more-than-40-000-staff/)

生成摘要时出错

---

## 10. Seven new models at scalable price-performance

**原文标题**: Seven new models at scalable price-performance

**原文链接**: [https://microsoft.ai/news/microsoft-ignite-2026/](https://microsoft.ai/news/microsoft-ignite-2026/)

生成摘要时出错

---

## 11. 病毒注射遏制三名胰腺癌患者病情

**原文标题**: Pancreatic cancer halted by virus injection in three patients

**原文链接**: [https://www.newscientist.com/article/2528235-pancreatic-cancer-halted-by-virus-injection-in-three-patients/](https://www.newscientist.com/article/2528235-pancreatic-cancer-halted-by-virus-injection-in-three-patients/)

A small study has shown promising results in halting the progression of advanced pancreatic cancer using a modified virus injected directly into tumors. Three patients with locally advanced, untreatable pancreatic cancer, who had previously undergone chemotherapy and radiotherapy, received injections of the virus, coxsackievirus A21 (CVA21), into their tumors.

After three months, imaging revealed that the tumors in all three patients had stopped growing. In two patients, the tumors had shrunk by 30% and 50% respectively. This viral therapy appeared to make the tumors more susceptible to further treatment, as all three patients subsequently underwent successful surgery to remove their tumors, a procedure previously deemed impossible.

One patient remains cancer-free 12 months post-surgery, while the other two have no evidence of disease at 6 and 9 months. The researchers, who presented their findings at the National Cancer Research Institute’s conference, believe the virus works by infecting and killing cancer cells, while also stimulating an anti-cancer immune response and potentially making tumors more visible to surgeons. This innovative approach offers hope for patients with a highly aggressive cancer with limited treatment options.

---

## 12. Interviewed at a YC startup, found out they used my LinkedIn without permission

**原文标题**: Interviewed at a YC startup, found out they used my LinkedIn without permission

**原文链接**: [https://reddit.com/r/recruitinghell/comments/1xyr6ml/interviewed_at_a_yc_startup_spent_30_hours/](https://reddit.com/r/recruitinghell/comments/1xyr6ml/interviewed_at_a_yc_startup_spent_30_hours/)

生成摘要时出错

---

## 13. ID.me terms required for IRS sign-in

**原文标题**: ID.me terms required for IRS sign-in

**原文链接**: [https://consumerrights.wiki/w/ID.me_terms_required_for_IRS_sign-in](https://consumerrights.wiki/w/ID.me_terms_required_for_IRS_sign-in)

生成摘要时出错

---

## 14. UK government forced to admit it issued Apple a secret encryption order

**原文标题**: UK government forced to admit it issued Apple a secret encryption order

**原文链接**: [https://macanorak.com/uk-government-forced-to-admit-it-issued-apple-a-secret-encryption-order/](https://macanorak.com/uk-government-forced-to-admit-it-issued-apple-a-secret-encryption-order/)

无法访问文章链接。

---

## 15. AI agents ask better questions than KPMG accountants in audit trial

**原文标题**: AI agents ask better questions than KPMG accountants in audit trial

**原文链接**: [https://europeanbusinessmagazine.com/ai-agents-better-questions-kpmg/](https://europeanbusinessmagazine.com/ai-agents-better-questions-kpmg/)

生成摘要时出错

---

## 16. Fuck Your AI Safeguards

**原文标题**: Fuck Your AI Safeguards

**原文链接**: [https://ounapuu.ee/posts/2026/11/19/unsafeguards/](https://ounapuu.ee/posts/2026/11/19/unsafeguards/)

生成摘要时出错

---

## 17. Anthropic prices initial public offering

**原文标题**: Anthropic prices initial public offering

**原文链接**: [https://www.anthropic.com/news/anthropic-prices-initial-public-offering](https://www.anthropic.com/news/anthropic-prices-initial-public-offering)

生成摘要时出错

---

## 18. Ruby2ßhell: Pre-authentication RCE on stock Rails

**原文标题**: Ruby2ßhell: Pre-authentication RCE on stock Rails

**原文链接**: [https://verialabs.com/ruby2shell/](https://verialabs.com/ruby2shell/)

生成摘要时出错

---

## 19. 15M web servers on one VM – smoltcp, DPDK, AF_XDP

**原文标题**: 15M web servers on one VM – smoltcp, DPDK, AF_XDP

**原文链接**: [https://kapteko.com/15-million-webservers/](https://kapteko.com/15-million-webservers/)

The article explores the ambitious goal of running 15 million web servers on a single VM with just 10GB RAM and 1 CPU core.

Initial attempts using standard Linux processes and syscalls quickly hit roadblocks:
1.  **Port Exhaustion:** The default TCP port range limits listening servers to ~65k. While using AnyIP/IPv6 subnets could provide millions of unique IP addresses, this only addresses the address space.
2.  **Excessive RAM:** Running 15 million separate processes or even distinct listening sockets consumes an exorbitant amount of RAM (estimated 20TB). This is because the Linux kernel allocates approximately 3300 bytes per socket for internal structures (like `tcp_sock`, `file`, `dentry`), regardless of whether the connection is active or idle.

To overcome these kernel-imposed limitations, the author proposes a radical two-part solution:
1.  **Userland Runtime:** Instead of individual processes, all 15 million web servers would run as "guests" within a custom userland runtime. A specialized scheduler would switch between these guests, preserving only minimal state (e.g., program counter, client/server file descriptors – roughly 16 bytes per guest), reducing memory overhead for guests to about 220MB.
2.  **Bypass Kernel Networking:** The substantial memory footprint of kernel sockets necessitates bypassing the kernel's network stack entirely. The solution involves implementing a custom TCP/IP stack in userland, specifically mentioning `smoltcp` (a bare-metal, heap-less Rust stack). For I/O, `smoltcp` can use TUN/TAP interfaces, but for ultimate performance and kernel bypass, **DPDK** is highlighted. DPDK allows direct, memory-mapped communication with the network card, eliminating syscalls, data copies, and interrupt overhead, albeit by dedicating a CPU core to a busy-polling loop. This low-level approach is critical to fit 15 million servers within the strict memory budget.

---

## 20. Russia reportedly planned mass-casualty attack in Poland to be blamed on Ukraine

**原文标题**: Russia reportedly planned mass-casualty attack in Poland to be blamed on Ukraine

**原文链接**: [https://www.yahoo.com/news/world/articles/russia-reportedly-planned-mass-casualty-090500574.html](https://www.yahoo.com/news/world/articles/russia-reportedly-planned-mass-casualty-090500574.html)

生成摘要时出错

---

## 21. 克劳德解决了黑洞物理学中的两个开放性问题。

**原文标题**: Claude solves two open problems in the physics of black holes

**原文链接**: [https://www.anthropic.com/research/claude-black-hole-physics](https://www.anthropic.com/research/claude-black-hole-physics)

生成摘要时出错

---

## 22. Someone reported java4shell bug in September 2026

**原文标题**: Someone reported java4shell bug in September 2026

**原文链接**: [https://github.com/openjdk/jdk/pull/32781](https://github.com/openjdk/jdk/pull/32781)

生成摘要时出错

---

## 23. Everything you need to survive and rebuild society

**原文标题**: Everything you need to survive and rebuild society

**原文链接**: [https://lastbook.org/](https://lastbook.org/)

生成摘要时出错

---

## 24. Multiple vulnerabilities in Regexp and String case conversion

**原文标题**: Multiple vulnerabilities in Regexp and String case conversion

**原文链接**: [https://www.ruby-lang.org/en/news/2026/11/18/multiple-vulnerabilities-in-regexp-and-string/](https://www.ruby-lang.org/en/news/2026/11/18/multiple-vulnerabilities-in-regexp-and-string/)

生成摘要时出错

---

## 25. Codeberg.org Not Reachable

**原文标题**: Codeberg.org Not Reachable

**原文链接**: [https://social.anoxinon.de/@codebergstatus/117636437840688845](https://social.anoxinon.de/@codebergstatus/117636437840688845)

生成摘要时出错

---

## 26. Energy-Based Reasoners: 385x more efficient inference

**原文标题**: Energy-Based Reasoners: 385x more efficient inference

**原文链接**: [https://energy-based-reasoners.github.io/](https://energy-based-reasoners.github.io/)

生成摘要时出错

---

## 27. The Cambridge Dictionary has named ‘human’ as the Word of the Year 2026

**原文标题**: The Cambridge Dictionary has named ‘human’ as the Word of the Year 2026

**原文链接**: [https://www.cam.ac.uk/news/cambridge-dictionary-reveals-word-of-the-year-2026](https://www.cam.ac.uk/news/cambridge-dictionary-reveals-word-of-the-year-2026)

生成摘要时出错

---

## 28. SSD prices may begin to decline in the latter half of 2027

**原文标题**: SSD prices may begin to decline in the latter half of 2027

**原文链接**: [https://www.drivevault.io/blog/when-will-hard-drive-prices-come-down.html](https://www.drivevault.io/blog/when-will-hard-drive-prices-come-down.html)

生成摘要时出错

---

## 29. LLM assisted reverse engineering

**原文标题**: LLM assisted reverse engineering

**原文链接**: [https://www.slowchronicle.com/posts/llm-assisted-reverse-engineering](https://www.slowchronicle.com/posts/llm-assisted-reverse-engineering)

生成摘要时出错

---

## 30. Genie 4 is now available

**原文标题**: Genie 4 is now available

**原文链接**: [https://blog.google/innovation-and-ai/models-and-research/google-deepmind/genie-4-now-available-project-genie/](https://blog.google/innovation-and-ai/models-and-research/google-deepmind/genie-4-now-available-project-genie/)

生成摘要时出错

---

## 31. Why is Gemini 4 Carbon taking so long?

**原文标题**: Why is Gemini 4 Carbon taking so long?

**原文链接**: [https://kernel.dev/blog/why-is-gemini-4-carbon-taking-so-long/](https://kernel.dev/blog/why-is-gemini-4-carbon-taking-so-long/)

生成摘要时出错

---

## 32. What's New in PHP 8.6

**原文标题**: What's New in PHP 8.6

**原文链接**: [https://www.php.net/releases/8.6/en.php](https://www.php.net/releases/8.6/en.php)

生成摘要时出错

---

## 33. Distributed, high-performance blob storage on SQLite

**原文标题**: Distributed, high-performance blob storage on SQLite

**原文链接**: [https://zerodha.tech/blog/high-performance-distributed-blob-storage/](https://zerodha.tech/blog/high-performance-distributed-blob-storage/)

生成摘要时出错

---

## 34. Scottish HTTP Codes

**原文标题**: Scottish HTTP Codes

**原文链接**: [https://underwood.network/http/scots.html](https://underwood.network/http/scots.html)

生成摘要时出错

---

## 35. Nintendo takes Picofly firmware down from GitHub [video]

**原文标题**: Nintendo takes Picofly firmware down from GitHub [video]

**原文链接**: [https://www.youtube.com/watch?v=-TLCGUpoD6c](https://www.youtube.com/watch?v=-TLCGUpoD6c)

生成摘要时出错

---

## 36. Gemini 4 Neon looks like an Opus 5.5 competitor

**原文标题**: Gemini 4 Neon looks like an Opus 5.5 competitor

**原文链接**: [https://micjm.com/blog/gemini-4-neon-looks-like-a-top-model/](https://micjm.com/blog/gemini-4-neon-looks-like-a-top-model/)

生成摘要时出错

---

## 37. Do not buy RAM, compress

**原文标题**: Do not buy RAM, compress

**原文链接**: [https://curiousbits.nl/blog/do-not-buy-ram-compress/](https://curiousbits.nl/blog/do-not-buy-ram-compress/)

生成摘要时出错

---

## 38. DaisyRose-27B

**原文标题**: DaisyRose-27B

**原文链接**: [https://www.radixark.com/blog/daisyrose-27b](https://www.radixark.com/blog/daisyrose-27b)

生成摘要时出错

---

## 39. Show HN: ExitPath – Open-source ways out of Slack, Notion and Microsoft 365

**原文标题**: Show HN: ExitPath – Open-source ways out of Slack, Notion and Microsoft 365

**原文链接**: [https://exitpath-ruddy.vercel.app/](https://exitpath-ruddy.vercel.app/)

生成摘要时出错

---

## 40. Making 8-page foldable zines from a single A4 sheet in the browser

**原文标题**: Making 8-page foldable zines from a single A4 sheet in the browser

**原文链接**: [https://krthr.co/paper-folds-and-whats-new-in-fanzines-app/](https://krthr.co/paper-folds-and-whats-new-in-fanzines-app/)

生成摘要时出错

---

## 41. Show HN: Take Voyager 1 apart, down to a single memory chip

**原文标题**: Show HN: Take Voyager 1 apart, down to a single memory chip

**原文链接**: [https://rshekhar.com/voyager/](https://rshekhar.com/voyager/)

生成摘要时出错

---

## 42. Advancing chip design with OpenAI models

**原文标题**: Advancing chip design with OpenAI models

**原文链接**: [https://openai.com/index/advancing-chip-design-with-our-models/](https://openai.com/index/advancing-chip-design-with-our-models/)

生成摘要时出错

---

## 43. Energy drinks linked to 11 times more reports of cardiac arrest

**原文标题**: Energy drinks linked to 11 times more reports of cardiac arrest

**原文链接**: [https://www.sciencedaily.com/releases/2026/11/261110042543.htm](https://www.sciencedaily.com/releases/2026/11/261110042543.htm)

生成摘要时出错

---

## 44. Pete warden on local AI, open models, voice interfaces, the future of hardware

**原文标题**: Pete warden on local AI, open models, voice interfaces, the future of hardware

**原文链接**: [https://thedataexchange.media/pete-warden-moonshine/](https://thedataexchange.media/pete-warden-moonshine/)

生成摘要时出错

---

## 45. F-22 Next-Generation micro–Data Transfer Cartridge (mDTC)

**原文标题**: F-22 Next-Generation micro–Data Transfer Cartridge (mDTC)

**原文链接**: [https://sam.gov/workspace/contract/opp/8948e8601e964c6aba9c801eee16b1be/view](https://sam.gov/workspace/contract/opp/8948e8601e964c6aba9c801eee16b1be/view)

生成摘要时出错

---

## 46. KVM: x86: Unconditionally reset MMU context when emulating INIT (CVE-2026-99312)

**原文标题**: KVM: x86: Unconditionally reset MMU context when emulating INIT (CVE-2026-99312)

**原文链接**: [https://www.cve.org/CVERecord?id=CVE-2026-99312](https://www.cve.org/CVERecord?id=CVE-2026-99312)

生成摘要时出错

---

## 47. The 98% Slot Machine: How Paid Advertising Became an Extraction Tax

**原文标题**: The 98% Slot Machine: How Paid Advertising Became an Extraction Tax

**原文链接**: [https://globalcommercegraph.com/writing/the-ninety-eight-percent-slot-machine](https://globalcommercegraph.com/writing/the-ninety-eight-percent-slot-machine)

生成摘要时出错

---

## 48. Show HN: Cornhole News – A Hacker News inspired site for news across the Midwest

**原文标题**: Show HN: Cornhole News – A Hacker News inspired site for news across the Midwest

**原文链接**: [https://cornholenews.news](https://cornholenews.news)

生成摘要时出错

---

## 49. Unreal Tournament 2004 in the Browser

**原文标题**: Unreal Tournament 2004 in the Browser

**原文链接**: [https://ut2004.dev/](https://ut2004.dev/)

生成摘要时出错

---

## 50. The x86 CPU: From 4004 to 486

**原文标题**: The x86 CPU: From 4004 to 486

**原文链接**: [https://pikuma.com/blog/history-of-x86-4004-to-486](https://pikuma.com/blog/history-of-x86-4004-to-486)

生成摘要时出错

---

## 51. Claude was trained on protein sequences at scale

**原文标题**: Claude was trained on protein sequences at scale

**原文链接**: [http://xinmingtu.cn/blog/2026/claude-opus-5-5-protein-sequences/](http://xinmingtu.cn/blog/2026/claude-opus-5-5-protein-sequences/)

生成摘要时出错

---

## 52. Software companies are trying to kill home computing?

**原文标题**: Software companies are trying to kill home computing?

**原文链接**: [https://lateblt.livejournal.com/526188.html](https://lateblt.livejournal.com/526188.html)

生成摘要时出错

---

## 53. Cooling buildings is overtaking heating them as an energy need, IEA says

**原文标题**: Cooling buildings is overtaking heating them as an energy need, IEA says

**原文链接**: [https://maccus.fr/en/cooling-overtaking-heating/](https://maccus.fr/en/cooling-overtaking-heating/)

生成摘要时出错

---

## 54. Unblockable communication with gravity

**原文标题**: Unblockable communication with gravity

**原文链接**: [https://www.science.org/doi/10.1126/sciadv.aee0802](https://www.science.org/doi/10.1126/sciadv.aee0802)

生成摘要时出错

---

## 55. "Anthropic Is Not a Safe AI Company" – Coalition Challenges Anthropic Safety

**原文标题**: "Anthropic Is Not a Safe AI Company" – Coalition Challenges Anthropic Safety

**原文链接**: [https://www.businesswire.com/news/home/20261118974464/en/Anthropic-is-Not-a-Safe-AI-Company---Broad-Coalition-of-Scientists-Legal-Scholars-and-Tech-Leaders-Challenge-Anthropics-Safety-Branding-Ahead-of-IPO](https://www.businesswire.com/news/home/20261118974464/en/Anthropic-is-Not-a-Safe-AI-Company---Broad-Coalition-of-Scientists-Legal-Scholars-and-Tech-Leaders-Challenge-Anthropics-Safety-Branding-Ahead-of-IPO)

生成摘要时出错

---

## 56. Show HN: Type Fighter 2

**原文标题**: Show HN: Type Fighter 2

**原文链接**: [https://typefighter2.com/](https://typefighter2.com/)

生成摘要时出错

---

## 57. A Primer on Fourier Series (2025)

**原文标题**: A Primer on Fourier Series (2025)

**原文链接**: [https://arxiv.org/abs/2510.18203](https://arxiv.org/abs/2510.18203)

生成摘要时出错

---

## 58. CrossPoint Reader

**原文标题**: CrossPoint Reader

**原文链接**: [https://crosspointreader.com](https://crosspointreader.com)

生成摘要时出错

---

## 59. Chrome AI features wasting much bandwidth

**原文标题**: Chrome AI features wasting much bandwidth

**原文链接**: [https://perishablepress.com/chrome-ai-wasting-much-bandwidth/](https://perishablepress.com/chrome-ai-wasting-much-bandwidth/)

生成摘要时出错

---

## 60. Two stealth models just appeared on the leaderboard, both ahead of Fable 5.2

**原文标题**: Two stealth models just appeared on the leaderboard, both ahead of Fable 5.2

**原文链接**: [https://contralabs.com/frontierdesign](https://contralabs.com/frontierdesign)

生成摘要时出错

---

## 61. DeepMind Employees Are Unionising

**原文标题**: DeepMind Employees Are Unionising

**原文链接**: [https://www.gdmunion.co.uk](https://www.gdmunion.co.uk)

生成摘要时出错

---

## 62. Teaching robots to carve marble sculptures

**原文标题**: Teaching robots to carve marble sculptures

**原文链接**: [https://eleanorwiesler.com/blog/robotic-stone-carving/](https://eleanorwiesler.com/blog/robotic-stone-carving/)

生成摘要时出错

---

## 63. The Magic of Partial Evaluation

**原文标题**: The Magic of Partial Evaluation

**原文链接**: [https://jimmyhmiller.com/magic-of-partial-evaluation](https://jimmyhmiller.com/magic-of-partial-evaluation)

生成摘要时出错

---

## 64. Black high school students sue after AI mistakes Doritos bag for gun

**原文标题**: Black high school students sue after AI mistakes Doritos bag for gun

**原文链接**: [https://www.lawyerscommittee.org/lawyers-committee-files-lawsuit-on-behalf-of-black-students-detained-and-searched-due-to-ai-alert-falsely-identifying-a-bag-of-chips-as-a-firearm/](https://www.lawyerscommittee.org/lawyers-committee-files-lawsuit-on-behalf-of-black-students-detained-and-searched-due-to-ai-alert-falsely-identifying-a-bag-of-chips-as-a-firearm/)

生成摘要时出错

---

## 65. Germany and Austria Call for European Control of TikTok

**原文标题**: Germany and Austria Call for European Control of TikTok

**原文链接**: [https://www.techcentral.ie/germany-and-austria-call-for-european-control-of-tiktok/](https://www.techcentral.ie/germany-and-austria-call-for-european-control-of-tiktok/)

生成摘要时出错

---

## 66. Cerebras Disaggregated Inference

**原文标题**: Cerebras Disaggregated Inference

**原文链接**: [https://www.cerebras.ai/blog/cerebras-launches-disaggregated-inference](https://www.cerebras.ai/blog/cerebras-launches-disaggregated-inference)

生成摘要时出错

---

## 67. AI isn't replacing your job. It's turning it into low-paid gig work

**原文标题**: AI isn't replacing your job. It's turning it into low-paid gig work

**原文链接**: [https://restofworld.org/2026/ai-jobs-skills-gig-work/](https://restofworld.org/2026/ai-jobs-skills-gig-work/)

生成摘要时出错

---

## 68. AI will not make you rich (2025)

**原文标题**: AI will not make you rich (2025)

**原文链接**: [https://colossus.com/article/ai-will-not-make-you-rich/](https://colossus.com/article/ai-will-not-make-you-rich/)

生成摘要时出错

---

## 69. Talos Linux

**原文标题**: Talos Linux

**原文链接**: [https://www.siderolabs.com/talos-linux](https://www.siderolabs.com/talos-linux)

生成摘要时出错

---

## 70. Show HN: Foolscap – a writing app that reads your book and never writes for you

**原文标题**: Show HN: Foolscap – a writing app that reads your book and never writes for you

**原文链接**: [https://foolscap.works/](https://foolscap.works/)

生成摘要时出错

---

## 71. The AI Superintelligence Debate Has Serious Flaws

**原文标题**: The AI Superintelligence Debate Has Serious Flaws

**原文链接**: [https://spectrum.ieee.org/ai-superintelligence-debate](https://spectrum.ieee.org/ai-superintelligence-debate)

生成摘要时出错

---

## 72. Bank CEOs, NSA Tell Congress That AI-Driven Patches Are Behind Outages

**原文标题**: Bank CEOs, NSA Tell Congress That AI-Driven Patches Are Behind Outages

**原文链接**: [https://www.washingtonsun.com/technology/bank-ceos-nsa-tell-congress-ai-driven-patches-behind-outages](https://www.washingtonsun.com/technology/bank-ceos-nsa-tell-congress-ai-driven-patches-behind-outages)

生成摘要时出错

---

## 73. NGINX2Root by Xint – From Nginx visitor to root of the server host

**原文标题**: NGINX2Root by Xint – From Nginx visitor to root of the server host

**原文链接**: [https://nginx2root.com/](https://nginx2root.com/)

生成摘要时出错

---

## 74. Synology Security Advisory

**原文标题**: Synology Security Advisory

**原文链接**: [https://www.synology.com/en-uk/security/advisory/Synology_SA_26_21](https://www.synology.com/en-uk/security/advisory/Synology_SA_26_21)

生成摘要时出错

---

## 75. OpenAI still has a WebRTC Problem

**原文标题**: OpenAI still has a WebRTC Problem

**原文链接**: [https://moq.dev/blog/webrtc-is-still-the-problem/](https://moq.dev/blog/webrtc-is-still-the-problem/)

生成摘要时出错

---

## 76. Google Chrome dev team declares bug report bankruptcy (2012)

**原文标题**: Google Chrome dev team declares bug report bankruptcy (2012)

**原文链接**: [https://blog.plover.com/tech/bug-reports.html](https://blog.plover.com/tech/bug-reports.html)

生成摘要时出错

---

## 77. PostgreSQL 19 Released

**原文标题**: PostgreSQL 19 Released

**原文链接**: [https://www.postgresql.org/about/news/postgresql-19-released-3449/](https://www.postgresql.org/about/news/postgresql-19-released-3449/)

生成摘要时出错

---

## 78. Why Fibonacci?

**原文标题**: Why Fibonacci?

**原文链接**: [https://www.evilgeniuslabs.org/why-fibonacci](https://www.evilgeniuslabs.org/why-fibonacci)

生成摘要时出错

---

## 79. Launch HN: Onlook (YC W25) – An open-source developer tool for designers

**原文标题**: Launch HN: Onlook (YC W25) – An open-source developer tool for designers

**原文链接**: [https://github.com/onlook-dev/onlook/](https://github.com/onlook-dev/onlook/)

生成摘要时出错

---

## 80. Palo Alto Networks to Acquire Applied Compute for $4.5B

**原文标题**: Palo Alto Networks to Acquire Applied Compute for $4.5B

**原文链接**: [https://investors.paloaltonetworks.com/news-releases/news-release-details/palo-alto-networks-acquire-applied-compute-bringing-secure-open](https://investors.paloaltonetworks.com/news-releases/news-release-details/palo-alto-networks-acquire-applied-compute-bringing-secure-open)

生成摘要时出错

---

## 81. Mass launched to orbit each year by rocket builder

**原文标题**: Mass launched to orbit each year by rocket builder

**原文链接**: [https://www.kadoa.com/companies/insights/spacex-europe-payload](https://www.kadoa.com/companies/insights/spacex-europe-payload)

生成摘要时出错

---

## 82. How to Make the Ink Used to Write Hamlet and the Declaration of Independence

**原文标题**: How to Make the Ink Used to Write Hamlet and the Declaration of Independence

**原文链接**: [https://lithub.com/how-to-make-the-ink-used-to-write-hamlet-the-declaration-of-independence-and-beethovens-fifth/](https://lithub.com/how-to-make-the-ink-used-to-write-hamlet-the-declaration-of-independence-and-beethovens-fifth/)

生成摘要时出错

---

## 83. ICE Is Paying AT&T to Dig Through a Mountain of Call Records

**原文标题**: ICE Is Paying AT&T to Dig Through a Mountain of Call Records

**原文链接**: [https://www.404media.co/ice-is-paying-at-t-to-dig-through-a-mountain-of-call-records-hemisphere-data-analytical-services/](https://www.404media.co/ice-is-paying-at-t-to-dig-through-a-mountain-of-call-records-hemisphere-data-analytical-services/)

生成摘要时出错

---

## 84. Should governments slow frontier AI? Jacob Coxon and Robin Hanson debate [video]

**原文标题**: Should governments slow frontier AI? Jacob Coxon and Robin Hanson debate [video]

**原文链接**: [https://www.youtube.com/watch?v=lwfewYL7X0o](https://www.youtube.com/watch?v=lwfewYL7X0o)

生成摘要时出错

---

## 85. GTA 6 Review: It Is a Masterpiece

**原文标题**: GTA 6 Review: It Is a Masterpiece

**原文链接**: [https://www.bloomberg.com/news/features/2026-11-18/gta-6-review-rockstar-games-latest-is-a-masterpiece](https://www.bloomberg.com/news/features/2026-11-18/gta-6-review-rockstar-games-latest-is-a-masterpiece)

生成摘要时出错

---

## 86. Exponential Behavior in Magic: The Gathering

**原文标题**: Exponential Behavior in Magic: The Gathering

**原文链接**: [https://levineuwirth.org/essays/exponential-magic/](https://levineuwirth.org/essays/exponential-magic/)

生成摘要时出错

---

## 87. Can Peer Review Survive AI-Generated Text? [pdf]

**原文标题**: Can Peer Review Survive AI-Generated Text? [pdf]

**原文链接**: [https://www.sas.upenn.edu/~jesusfv/Peer_Review.pdf](https://www.sas.upenn.edu/~jesusfv/Peer_Review.pdf)

生成摘要时出错

---

## 88. C's designated initializers give us named arguments

**原文标题**: C's designated initializers give us named arguments

**原文链接**: [https://quuxplusone.github.io/blog/2026/11/16/named-arguments-in-c/](https://quuxplusone.github.io/blog/2026/11/16/named-arguments-in-c/)

生成摘要时出错

---

## 89. Search Browser – Minimalist WebKit browser with Chrome extension support

**原文标题**: Search Browser – Minimalist WebKit browser with Chrome extension support

**原文链接**: [https://searchbrowser.app/](https://searchbrowser.app/)

生成摘要时出错

---

## 90. Visa, Mastercard and JPMorgan Customer Data Leaked by Hackers

**原文标题**: Visa, Mastercard and JPMorgan Customer Data Leaked by Hackers

**原文链接**: [https://www.wsj.com/finance/banking/visa-mastercard-and-jpmorgan-customer-data-leaked-by-hackers-3b5a0f87](https://www.wsj.com/finance/banking/visa-mastercard-and-jpmorgan-customer-data-leaked-by-hackers-3b5a0f87)

生成摘要时出错

---

## 91. Pushing WireGuard on macOS to 5 Gbit/s

**原文标题**: Pushing WireGuard on macOS to 5 Gbit/s

**原文链接**: [https://www.firezone.dev/blog/apple-client-performance](https://www.firezone.dev/blog/apple-client-performance)

生成摘要时出错

---

## 92. Mosquitoes are Ladakh's latest tourists

**原文标题**: Mosquitoes are Ladakh's latest tourists

**原文链接**: [https://ruralindiaonline.org/article/mosquitoes-are-ladakh-s-latest-tourists](https://ruralindiaonline.org/article/mosquitoes-are-ladakh-s-latest-tourists)

生成摘要时出错

---

## 93. PHP 8.5.13

**原文标题**: PHP 8.5.13

**原文链接**: [https://www.php.net/ChangeLog-8.php](https://www.php.net/ChangeLog-8.php)

生成摘要时出错

---

## 94. Fable: Written, painted and directed by Claude Fable 5.2

**原文标题**: Fable: Written, painted and directed by Claude Fable 5.2

**原文链接**: [https://claudia.gallery/fable/](https://claudia.gallery/fable/)

生成摘要时出错

---

## 95. SuperEMeans: Making e-means 3× faster

**原文标题**: SuperEMeans: Making e-means 3× faster

**原文链接**: [https://www.lkuffo.com/superemeans/](https://www.lkuffo.com/superemeans/)

生成摘要时出错

---

## 96. Voyager 1 hits one light day from Earth

**原文标题**: Voyager 1 hits one light day from Earth

**原文链接**: [https://science.nasa.gov/mission/voyager/where-are-voyager-1-and-voyager-2-now/](https://science.nasa.gov/mission/voyager/where-are-voyager-1-and-voyager-2-now/)

生成摘要时出错

---

## 97. Google Gemini's "Tasks" Personal Assistant Is Now Free

**原文标题**: Google Gemini's "Tasks" Personal Assistant Is Now Free

**原文链接**: [https://blog.google/innovation-and-ai/products/gemini-app/tasks-in-gemini-free-new-features/](https://blog.google/innovation-and-ai/products/gemini-app/tasks-in-gemini-free-new-features/)

生成摘要时出错

---

## 98. Upcoming Critical PHP Security Release

**原文标题**: Upcoming Critical PHP Security Release

**原文链接**: [https://www.php.net/archive/2026.php](https://www.php.net/archive/2026.php)

生成摘要时出错

---

## 99. Attackers Used Optimizely to A/B Test Malware on Top Websites

**原文标题**: Attackers Used Optimizely to A/B Test Malware on Top Websites

**原文链接**: [https://krebsonsecurity.com/2026/11/attackers-used-optimizely-to-a-b-test-malware-on-top-websites/](https://krebsonsecurity.com/2026/11/attackers-used-optimizely-to-a-b-test-malware-on-top-websites/)

生成摘要时出错

---

## 100. Gemini 4 Neon is the new #1 on the Models Engineering Index

**原文标题**: Gemini 4 Neon is the new #1 on the Models Engineering Index

**原文链接**: [https://git-aarvin.github.io/mei/](https://git-aarvin.github.io/mei/)

生成摘要时出错

---

