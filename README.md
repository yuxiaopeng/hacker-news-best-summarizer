# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-07-08.md)

*最后自动更新时间: 2026-07-08 20:53:58*
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

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 2 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 3 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 4 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 5 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 6 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 7 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 8 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 9 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 10 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 11 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 12 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 13 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 14 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 15 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 16 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 17 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 18 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 19 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 20 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 21 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 22 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 23 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 24 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 25 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 26 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 27 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 28 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 29 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 30 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 31 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 32 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 33 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 34 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 35 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 36 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 37 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 38 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 39 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 40 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 41 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 42 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 43 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 44 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 45 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 46 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 47 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 48 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 49 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 50 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 51 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 52 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 53 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 54 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 55 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 56 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 57 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 58 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 59 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 60 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 61 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 62 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 63 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 64 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 65 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 66 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 67 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 68 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 69 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 70 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 71 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 72 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 73 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 74 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 75 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 76 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 77 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 78 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 79 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 80 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 81 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 82 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 83 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 84 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 85 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 86 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 87 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 88 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 89 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 90 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 91 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 92 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 93 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 94 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 95 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 96 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 97 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 98 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 99 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 100 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 101 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 102 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 103 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 104 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 105 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 106 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 107 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 108 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 109 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 110 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 111 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 112 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 113 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 114 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 115 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 116 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 117 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 118 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 119 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 120 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 121 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 122 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 123 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 124 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 125 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 126 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 127 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 128 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 129 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 130 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 131 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 132 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 133 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 134 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 135 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 136 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 137 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 138 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 139 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 140 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 141 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 142 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 143 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 144 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 145 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 146 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 147 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 148 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 149 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 150 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 151 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 152 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 153 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 154 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 155 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 156 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 157 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 158 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 159 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 160 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 161 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 162 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 163 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 164 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 165 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 166 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 167 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 168 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 169 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 170 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 171 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 172 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 173 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 174 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 175 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 176 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 177 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 178 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 179 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 180 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 181 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 182 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 183 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 184 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 185 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 186 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 187 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 188 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 189 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 190 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 191 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 192 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 193 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 194 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 195 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 196 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 197 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 198 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 199 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 200 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 201 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 202 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 203 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 204 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 205 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 206 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 207 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 208 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 209 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 210 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 211 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 212 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 213 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 214 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 215 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 216 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 217 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 218 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 219 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 220 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 221 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 222 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 223 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 224 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 225 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 226 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 227 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 228 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 229 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 230 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 231 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 232 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 233 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 234 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 235 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 236 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 237 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 238 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 239 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 240 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 241 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 242 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 243 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
