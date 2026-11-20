# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-11-20.md)

*最后自动更新时间: 2026-11-20 01:34:28*
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

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-11-20](output/hacker_news_summary_2026-11-20.md) |
| 2 | [2026-11-19](output/hacker_news_summary_2026-11-19.md) |
| 3 | [2026-11-18](output/hacker_news_summary_2026-11-18.md) |
| 4 | [2026-11-14](output/hacker_news_summary_2026-11-14.md) |
| 5 | [2026-11-15](output/hacker_news_summary_2026-11-15.md) |
| 6 | [2026-11-13](output/hacker_news_summary_2026-11-13.md) |
| 7 | [2026-11-17](output/hacker_news_summary_2026-11-17.md) |
| 8 | [2026-11-07](output/hacker_news_summary_2026-11-07.md) |
| 9 | [2026-11-06](output/hacker_news_summary_2026-11-06.md) |
| 10 | [2026-11-11](output/hacker_news_summary_2026-11-11.md) |
| 11 | [2026-11-08](output/hacker_news_summary_2026-11-08.md) |
| 12 | [2026-11-12](output/hacker_news_summary_2026-11-12.md) |
| 13 | [2026-11-10](output/hacker_news_summary_2026-11-10.md) |
| 14 | [2026-11-01](output/hacker_news_summary_2026-11-01.md) |
| 15 | [2026-11-03](output/hacker_news_summary_2026-11-03.md) |
| 16 | [2026-11-05](output/hacker_news_summary_2026-11-05.md) |
| 17 | [2026-10-31](output/hacker_news_summary_2026-10-31.md) |
| 18 | [2026-11-04](output/hacker_news_summary_2026-11-04.md) |
| 19 | [2026-10-25](output/hacker_news_summary_2026-10-25.md) |
| 20 | [2026-10-27](output/hacker_news_summary_2026-10-27.md) |
| 21 | [2026-10-28](output/hacker_news_summary_2026-10-28.md) |
| 22 | [2026-10-26](output/hacker_news_summary_2026-10-26.md) |
| 23 | [2026-10-29](output/hacker_news_summary_2026-10-29.md) |
| 24 | [2026-10-30](output/hacker_news_summary_2026-10-30.md) |
| 25 | [2026-10-19](output/hacker_news_summary_2026-10-19.md) |
| 26 | [2026-10-24](output/hacker_news_summary_2026-10-24.md) |
| 27 | [2026-10-23](output/hacker_news_summary_2026-10-23.md) |
| 28 | [2026-10-21](output/hacker_news_summary_2026-10-21.md) |
| 29 | [2026-10-22](output/hacker_news_summary_2026-10-22.md) |
| 30 | [2026-10-20](output/hacker_news_summary_2026-10-20.md) |
| 31 | [2026-10-18](output/hacker_news_summary_2026-10-18.md) |
| 32 | [2026-10-17](output/hacker_news_summary_2026-10-17.md) |
| 33 | [2026-10-15](output/hacker_news_summary_2026-10-15.md) |
| 34 | [2026-10-16](output/hacker_news_summary_2026-10-16.md) |
| 35 | [2026-10-13](output/hacker_news_summary_2026-10-13.md) |
| 36 | [2026-10-09](output/hacker_news_summary_2026-10-09.md) |
| 37 | [2026-10-11](output/hacker_news_summary_2026-10-11.md) |
| 38 | [2026-10-14](output/hacker_news_summary_2026-10-14.md) |
| 39 | [2026-10-07](output/hacker_news_summary_2026-10-07.md) |
| 40 | [2026-10-10](output/hacker_news_summary_2026-10-10.md) |
| 41 | [2026-10-03](output/hacker_news_summary_2026-10-03.md) |
| 42 | [2026-10-02](output/hacker_news_summary_2026-10-02.md) |
| 43 | [2026-09-30](output/hacker_news_summary_2026-09-30.md) |
| 44 | [2026-10-01](output/hacker_news_summary_2026-10-01.md) |
| 45 | [2026-10-06](output/hacker_news_summary_2026-10-06.md) |
| 46 | [2026-10-04](output/hacker_news_summary_2026-10-04.md) |
| 47 | [2026-09-24](output/hacker_news_summary_2026-09-24.md) |
| 48 | [2026-09-23](output/hacker_news_summary_2026-09-23.md) |
| 49 | [2026-09-29](output/hacker_news_summary_2026-09-29.md) |
| 50 | [2026-09-25](output/hacker_news_summary_2026-09-25.md) |
| 51 | [2026-09-27](output/hacker_news_summary_2026-09-27.md) |
| 52 | [2026-09-21](output/hacker_news_summary_2026-09-21.md) |
| 53 | [2026-09-18](output/hacker_news_summary_2026-09-18.md) |
| 54 | [2026-09-20](output/hacker_news_summary_2026-09-20.md) |
| 55 | [2026-09-19](output/hacker_news_summary_2026-09-19.md) |
| 56 | [2026-09-22](output/hacker_news_summary_2026-09-22.md) |
| 57 | [2026-09-13](output/hacker_news_summary_2026-09-13.md) |
| 58 | [2026-09-14](output/hacker_news_summary_2026-09-14.md) |
| 59 | [2026-09-17](output/hacker_news_summary_2026-09-17.md) |
| 60 | [2026-09-16](output/hacker_news_summary_2026-09-16.md) |
| 61 | [2026-09-15](output/hacker_news_summary_2026-09-15.md) |
| 62 | [2026-09-12](output/hacker_news_summary_2026-09-12.md) |
| 63 | [2026-09-06](output/hacker_news_summary_2026-09-06.md) |
| 64 | [2026-09-08](output/hacker_news_summary_2026-09-08.md) |
| 65 | [2026-09-07](output/hacker_news_summary_2026-09-07.md) |
| 66 | [2026-09-11](output/hacker_news_summary_2026-09-11.md) |
| 67 | [2026-09-09](output/hacker_news_summary_2026-09-09.md) |
| 68 | [2026-09-10](output/hacker_news_summary_2026-09-10.md) |
| 69 | [2026-09-05](output/hacker_news_summary_2026-09-05.md) |
| 70 | [2026-09-01](output/hacker_news_summary_2026-09-01.md) |
| 71 | [2026-09-02](output/hacker_news_summary_2026-09-02.md) |
| 72 | [2026-09-03](output/hacker_news_summary_2026-09-03.md) |
| 73 | [2026-08-30](output/hacker_news_summary_2026-08-30.md) |
| 74 | [2026-09-04](output/hacker_news_summary_2026-09-04.md) |
| 75 | [2026-08-31](output/hacker_news_summary_2026-08-31.md) |
| 76 | [2026-08-29](output/hacker_news_summary_2026-08-29.md) |
| 77 | [2026-08-22](output/hacker_news_summary_2026-08-22.md) |
| 78 | [2026-08-24](output/hacker_news_summary_2026-08-24.md) |
| 79 | [2026-08-25](output/hacker_news_summary_2026-08-25.md) |
| 80 | [2026-08-26](output/hacker_news_summary_2026-08-26.md) |
| 81 | [2026-08-28](output/hacker_news_summary_2026-08-28.md) |
| 82 | [2026-08-23](output/hacker_news_summary_2026-08-23.md) |
| 83 | [2026-08-20](output/hacker_news_summary_2026-08-20.md) |
| 84 | [2026-08-16](output/hacker_news_summary_2026-08-16.md) |
| 85 | [2026-08-18](output/hacker_news_summary_2026-08-18.md) |
| 86 | [2026-08-17](output/hacker_news_summary_2026-08-17.md) |
| 87 | [2026-08-15](output/hacker_news_summary_2026-08-15.md) |
| 88 | [2026-08-21](output/hacker_news_summary_2026-08-21.md) |
| 89 | [2026-08-14](output/hacker_news_summary_2026-08-14.md) |
| 90 | [2026-08-19](output/hacker_news_summary_2026-08-19.md) |
| 91 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 92 | [2026-08-11](output/hacker_news_summary_2026-08-11.md) |
| 93 | [2026-08-10](output/hacker_news_summary_2026-08-10.md) |
| 94 | [2026-08-12](output/hacker_news_summary_2026-08-12.md) |
| 95 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 96 | [2026-08-09](output/hacker_news_summary_2026-08-09.md) |
| 97 | [2026-08-13](output/hacker_news_summary_2026-08-13.md) |
| 98 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 99 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 100 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 101 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 102 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 103 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 104 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 105 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 106 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 107 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 108 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 109 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 110 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 111 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 112 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 113 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 114 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 115 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 116 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 117 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 118 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 119 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 120 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 121 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 122 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 123 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 124 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 125 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 126 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 127 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 128 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 129 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 130 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 131 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 132 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 133 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 134 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 135 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 136 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 137 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 138 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 139 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 140 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 141 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 142 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 143 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 144 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 145 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 146 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 147 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 148 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 149 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 150 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 151 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 152 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 153 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 154 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 155 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 156 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 157 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 158 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 159 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 160 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 161 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 162 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 163 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 164 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 165 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 166 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 167 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 168 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 169 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 170 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 171 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 172 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 173 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 174 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 175 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 176 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 177 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 178 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 179 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 180 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 181 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 182 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 183 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 184 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 185 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 186 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 187 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 188 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 189 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 190 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 191 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 192 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 193 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 194 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 195 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 196 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 197 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 198 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 199 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 200 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 201 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 202 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 203 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 204 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 205 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 206 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 207 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 208 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 209 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 210 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 211 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 212 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 213 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 214 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 215 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 216 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 217 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 218 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 219 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 220 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 221 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 222 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 223 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 224 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 225 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 226 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 227 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 228 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 229 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 230 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 231 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 232 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 233 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 234 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 235 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 236 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 237 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 238 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 239 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 240 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 241 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 242 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 243 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 244 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 245 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 246 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 247 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 248 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 249 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 250 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 251 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 252 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 253 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 254 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 255 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 256 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 257 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 258 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 259 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 260 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 261 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 262 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 263 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 264 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 265 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 266 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 267 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 268 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 269 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 270 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 271 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 272 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 273 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 274 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 275 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 276 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 277 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 278 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 279 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 280 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 281 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 282 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 283 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 284 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 285 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 286 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 287 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 288 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 289 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 290 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 291 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 292 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 293 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 294 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 295 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 296 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 297 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 298 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 299 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 300 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 301 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 302 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 303 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 304 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 305 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 306 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 307 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 308 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 309 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 310 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 311 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 312 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 313 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 314 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 315 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 316 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 317 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 318 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 319 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 320 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 321 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 322 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 323 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 324 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 325 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 326 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 327 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 328 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 329 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 330 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 331 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 332 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 333 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 334 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 335 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 336 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 337 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 338 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 339 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 340 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 341 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 342 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 343 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 344 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 345 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 346 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 347 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 348 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 349 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 350 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 351 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 352 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 353 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 354 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 355 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 356 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 357 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 358 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 359 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 360 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 361 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 362 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 363 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 364 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
| 365 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 366 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 367 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 368 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
