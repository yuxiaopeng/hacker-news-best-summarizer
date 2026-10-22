# Hacker News 热门文章摘要 (2026-10-22)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. PHP 8.2.35

**原文标题**: PHP 8.2.35

**原文链接**: [https://github.com/php/php-src/releases/tag/php-8.2.35](https://github.com/php/php-src/releases/tag/php-8.2.35)

PHP开发团队发布了PHP 8.2.35，这是一个关键安全更新。该版本解决了两个严重漏洞（CVE-2026-109618和CVE-2026-109619），这些漏洞可能导致未经身份验证的远程代码执行。强烈建议所有PHP 8.2用户立即更新，因为更新是唯一安全的缓解措施。

该公告还提醒用户，PHP 8.2将于2026年12月31日停止支持，之后将不再接收安全修复。建议用户规划升级到一个受支持的PHP版本。PHP 8.2.35的源代码下载以及Windows二进制文件可在官方下载页面获取，并且还提供了详细的变更日志。

---

## 2. 八位信任：eMudhra的CA密钥毫秒级破解

**原文标题**: Eight Bits of Trust: eMudhra's CA keys cracked in milliseconds

**原文链接**: [https://scotthelme.co.uk/eight-bits-of-trust-emudhras-ca-keys-cracked-in-milliseconds/](https://scotthelme.co.uk/eight-bits-of-trust-emudhras-ca-keys-cracked-in-milliseconds/)

eMudhra 证书颁发机构 (CA) 的八个中间证书的私钥被发现异常脆弱，它们由单字节数字（例如 4、56、115）组成，而不是加密标准要求的大型随机 384 位椭圆曲线密钥。这一根本性缺陷使得任何人都能在几毫秒内通过暴力破解恢复这些私钥，实际上，自它们于 2025 年 4 月创建以来，这些私钥就已等同于公开。

一名安全研究人员于 10 月 17 日报告了此事，导致 Chrome 和 Firefox 立即将其阻止，Mozilla 也发布了公开声明并移除了 eMudhra 根证书。尽管主要浏览器由于直接阻止和证书透明度 (CT) 强制执行而现在受到保护，但此次泄露的“无法遏制”的性质源于其对庞大的非浏览器 TLS 客户端生态系统（例如 curl、Python、Node、Go、Java、Git、软件包管理器、CI/CD 管道、物联网设备）的影响。

这些客户端通常依赖本地 CA 捆绑包，默认情况下通常不检查证书吊销，并忽略证书透明度，使官方吊销变得无效。这使它们容易受到任何域的伪造证书的攻击，从而实现流量拦截、通过受损更新进行的供应链攻击以及数据窃取。许多固件已固定的物联网和嵌入式设备将持续易受攻击，直到这些证书在 2039 年过期。所有带有 CA 捆绑包的系统都急需更新，但无法更新的设备构成长期、未缓解的风险。这些密钥非常脆弱，即使是像 Claude 这样的 AI 代理也能通过一个简单的提示恢复它们。

---

## 3. eMudhra将退出全球SSL/TLS证书业务

**原文标题**: eMudhra to exit global SSL/TLS certificate business

**原文链接**: [https://emudhra.com/en/press-release/emudhra-to-exit-global-ssl-tls-certificate-business](https://emudhra.com/en/press-release/emudhra-to-exit-global-ssl-tls-certificate-business)

eMudhra Limited 宣布决定退出全球 SSL/TLS 证书业务，自2026年10月22日起生效，以专注于核心企业解决方案和其他数字信任服务。

此举源于近期涉及其全球 SSL/TLS 证书的一起事件，尽管该事件已得到妥善处理，且未发生基础设施受损或数据泄露，但仍引起了社交媒体的过度关注。eMudhra 指出，全球 SSL/TLS 业务仅占其收入的约1%，且其复杂性、成本以及（由于合规性要求增加和免费证书的提供导致）投资回报率降低，已不再符合其战略目标。

eMudhra 承诺为客户提供无缝过渡，在此期间，G1 RSA 根证书将继续运行。受影响的客户将从合作伙伴处获得免费的替换证书，撤销服务将一直运行，直到所有证书过期或被替换。一份完整的根本原因报告将提交给浏览器程序。

公司的核心业务不受影响。其全球数字签名证书 (DSC)、eSign 服务、企业 PKI 解决方案（emCA、CertiNext）、emSigner 电子签名套件以及身份/认证解决方案（SecurePass、emAS）均在独立基础设施上运行，并继续正常运营。eMudhra 现在将专注于其在超过35个国家更广泛的数字身份、信任和安全解决方案组合。

---

## 4. Quad9 (DNS解析器) 将退出法国

**原文标题**: Quad9 (DNS Resolver) to Exit France

**原文链接**: [https://quad9.net/news/blog/au-revoir-france/](https://quad9.net/news/blog/au-revoir-france/)

Quad9, a non-profit DNS resolver, announced its withdrawal from France starting November 24, following an unfavorable French court ruling. The decision, originating from a copyright infringement lawsuit filed by beIN, demands Quad9 block recursive DNS resolution for specific domain names for users in France.

Quad9 states that compliance is technically unfeasible and violates its core mission to protect user privacy, provide cybersecurity, and maintain internet integrity by offering neutral DNS services. They refuse to manipulate DNS responses or extend French legal decisions globally. Geo-blocking is deemed unreliable and previously led to fines in a similar German case, while targeted blocking is impossible as Quad9 collects no user data. The financial penalties from this and 20 other pending lawsuits are unsustainable.

Quad9 argues that DNS blocking is an ineffective anti-piracy measure, merely pushing users to less secure resolvers, and sets a dangerous precedent for censorship by private corporations. This departure will leave numerous French users, including critical infrastructure, without Quad9's cybersecurity protection.

Quad9 urges French citizens to contact legislators and regulatory bodies like ARCOM to advocate against DNS blocking, emphasizing the importance of an open internet and balancing digital rights with copyright concerns. They regret leaving French users unprotected but hope for a future legal environment that permits their return.

---

## 5. Today's PHP security release, and how we're strengthening security

**原文标题**: Today's PHP security release, and how we're strengthening security

**原文链接**: [https://thephp.foundation/blog/2026/10/21/todays-php-security-release-and-how-were-strengthening-php-security/](https://thephp.foundation/blog/2026/10/21/todays-php-security-release-and-how-were-strengthening-php-security/)

生成摘要时出错

---

## 6. EA 关闭 BioWare

**原文标题**: EA is shutting down BioWare

**原文链接**: [https://www.theverge.com/games/1015647/ea-is-shutting-down-bioware](https://www.theverge.com/games/1015647/ea-is-shutting-down-bioware)

生成摘要时出错

---

## 7. Meta被判在新墨西哥州剑桥分析公司案件中支付250亿美元罚款。

**原文标题**: Meta ordered to pay $25B penalty in New Mexico Cambridge Analytica case

**原文链接**: [https://www.cnbc.com/2026/10/21/meta-new-mexico-cambridge-analytica-penalty.html](https://www.cnbc.com/2026/10/21/meta-new-mexico-cambridge-analytica-penalty.html)

新墨西哥州一家法院判决Meta支付250亿美元罚款，此前陪审团裁定该公司在“剑桥分析”丑闻中，就其如何保护和收集用户数据一事误导了该州公民，需承担责任。

圣达菲的陪审团认定Meta违反了新墨西哥州的不公平商业行为法案逾4300万次，这本可能导致2195亿美元的罚款。然而，地区法院法官弗朗西斯·马修最终将罚款减至250亿美元，他指出Meta“故意违规的数量异常巨大”、持续时间长、高层领导参与其中，以及其虚假陈述的“蓄意和系统性”。在罚款付清之前，每年将按15%的利率累计利息。

新墨西哥州总检察长劳尔·托雷斯赞扬了这项裁决，称其表明强大的科技公司对其违规行为将面临后果。Meta首席法务官C.J.马奥尼批评了这项决定，称其为“言论税”，使该公司在该州无法开展业务，并确认公司计划上诉。

新墨西哥州的案件之所以能够进行审判，是因为它未纳入Meta与其他州就类似数据隐私问题达成的一项总计170亿美元的和解协议。法官还强调，Meta对“剑桥分析”丑闻的内部调查“故意无效”，这受到成本削减压力和避免树立先例的愿望影响。这项罚款是继其他与“剑桥分析”相关的和解协议之后的又一笔，其中包括2022年的一项7.25亿美元的集体诉讼和解。此外，Meta在新墨西哥州还面临一项与儿童安全相关的5.67亿美元罚款的上诉。

---

## 8. Jailbreaking the Switch 2

**原文标题**: Jailbreaking the Switch 2

**原文链接**: [https://pepsipu.com/blog/2026-10-switch2-jailbreak-ns2jb/](https://pepsipu.com/blog/2026-10-switch2-jailbreak-ns2jb/)

生成摘要时出错

---

## 9. 巴黎协定的1.5摄氏度目标不再可行。

**原文标题**: The 1.5°C goal of the Paris Agreement is no longer viable

**原文链接**: [https://unric.org/en/unep-emissions-gap-report-2026-1-5-degree-overshoot/](https://unric.org/en/unep-emissions-gap-report-2026-1-5-degree-overshoot/)

The United Nations Environment Programme (UNEP) 2026 Emissions Gap Report, "The Point of Return," states that the Paris Agreement's 1.5°C global warming limit by 2100 is no longer viable, with exceeding this threshold now "imminent and inevitable."

The new imperative is to ensure global warming remains below 2°C, with the ambitious goal of returning to 1.5°C by century's end. This requires drastic action: global greenhouse gas emissions must be cut by 18% by 2030, 45% by 2035, and 69% by 2040, relative to 2025 levels. Current national commitments fall far short, projecting only 5-8% reductions by 2030.

Key actions outlined include accelerating clean energy and electrification, establishing clear roadmaps for transitioning away from fossil fuels, investing in grids and storage, improving energy efficiency, cutting methane, and halting/reversing deforestation. Specific targets involve tripling renewable energy capacity by 2035 and significantly reducing coal, oil, and gas shares in energy production (e.g., coal by 55%, oil by 15%, gas by 5% by 2035).

Additionally, large-scale CO2 removal operations, equivalent to 320 gigatons, will be necessary by the end of the century through biological and technological means. Despite progress in renewable energy since 2015, overall efforts, especially concerning fossil fuels and deforestation, remain insufficient. Urgent, global, and economy-wide action is critical to limit any overshoot of 1.5°C and avert catastrophic irreversible changes.

---

## 10. The Future of CSS

**原文标题**: The Future of CSS

**原文链接**: [https://www.joshwcomeau.com/css/interop-2027/](https://www.joshwcomeau.com/css/interop-2027/)

生成摘要时出错

---

## 11. There isn't an easy exploit for this PHP vulnerability

**原文标题**: There isn't an easy exploit for this PHP vulnerability

**原文链接**: [https://eliastaylor.com/noexploit/](https://eliastaylor.com/noexploit/)

生成摘要时出错

---

## 12. mitmproxy adds --emudhra option

**原文标题**: mitmproxy adds --emudhra option

**原文链接**: [https://github.com/mitmproxy/mitmproxy/commit/169234499088fc2c414644a67efaed3d64ae2e3b](https://github.com/mitmproxy/mitmproxy/commit/169234499088fc2c414644a67efaed3d64ae2e3b)

生成摘要时出错

---

## 13. Compromised LiteLLM 1.107.0 on PyPI Installs a Credential Stealer and Backdoor

**原文标题**: Compromised LiteLLM 1.107.0 on PyPI Installs a Credential Stealer and Backdoor

**原文链接**: [https://safedep.io/litellm-pypi-compromise-credential-stealer-backdoor/](https://safedep.io/litellm-pypi-compromise-credential-stealer-backdoor/)

生成摘要时出错

---

## 14. Security Disclosure

**原文标题**: Security Disclosure

**原文链接**: [https://blog.railway.com/p/security-disclosure-wednesday-october-21st](https://blog.railway.com/p/security-disclosure-wednesday-october-21st)

生成摘要时出错

---

## 15. Claude Duet

**原文标题**: Claude Duet

**原文链接**: [https://claude.com/product/claude-duet](https://claude.com/product/claude-duet)

生成摘要时出错

---

## 16. The No Kings Takedown Is Why You Shouldn't Rent Your Megaphone from Zuck

**原文标题**: The No Kings Takedown Is Why You Shouldn't Rent Your Megaphone from Zuck

**原文链接**: [https://www.techdirt.com/2026/10/20/accident-or-not-the-no-kings-takedown-is-why-you-shouldnt-rent-your-megaphone-from-zuck/](https://www.techdirt.com/2026/10/20/accident-or-not-the-no-kings-takedown-is-why-you-shouldnt-rent-your-megaphone-from-zuck/)

生成摘要时出错

---

## 17. WorldTUI: I trained a 360M model to pretend to be a terminal

**原文标题**: WorldTUI: I trained a 360M model to pretend to be a terminal

**原文链接**: [https://simedw.com/2026/10/21/world-model-terminal/](https://simedw.com/2026/10/21/world-model-terminal/)

生成摘要时出错

---

## 18. DuckDB 2.0.0 LTS “Cinnamon Teal”

**原文标题**: DuckDB 2.0.0 LTS “Cinnamon Teal”

**原文链接**: [https://duckdb.org/2026/10/21/announcing-duckdb-200](https://duckdb.org/2026/10/21/announcing-duckdb-200)

生成摘要时出错

---

## 19. PHP2Shell: AI uncovers critical RCE in PHP

**原文标题**: PHP2Shell: AI uncovers critical RCE in PHP

**原文链接**: [https://www.wiz.io/blog/php2shell-php-rce](https://www.wiz.io/blog/php2shell-php-rce)

生成摘要时出错

---

## 20. PingCap TiDB Leaks

**原文标题**: PingCap TiDB Leaks

**原文链接**: [https://fulcrumsec.vg/pingcap/](https://fulcrumsec.vg/pingcap/)

FulcrumSec has disclosed a massive, undetected breach of PingCAP TiDB Cloud, exfiltrating 10.6 TB of data over nearly two months. The stolen data encompasses the entire TiDB Cloud control plane, its financial and billing estates, GCP/AWS storage, Jira, CRM, analytics, and source code.

Key exfiltrated information includes:
*   **Customer Control Plane:** Details on 180,046 tenant organizations, 403,262 unique emails, 115,308 plaintext customer API keys (42,612 active), and 1,809 customer database credentials (root/admin accounts).
*   **Customer Data:** 20.6 million raw customer SQL statements revealing application schemas, table designs, and sensitive business logic, plus 5 million customer server IPs from four years of gateway access logs.
*   **Financial & Commercial:** 57 months of AWS spend ($107M), detailed per-customer gross margins, HubSpot CRM data with 433,928 contacts and deal values (e.g., $552M deals with clients like PayPay, Atlassian, SBI), and China ledger records including Bank of China.
*   **Source Code:** 413 private repositories revealing critical vulnerabilities in billing, identity services, and a shared crypto library.
*   **Identity Graph:** 13.6 million GA4 device identifiers, Mixpanel profiles, and a developer intelligence graph ranking engineers at companies like Tencent, Huawei, and Mastercard.

The report highlights PingCAP's severe negligence, including "zero visibility" into its cloud services, failure to detect continuous data exfiltration, and an unaddressed 2022 internal security warning (Jira ticket SECURITY-22) about unconditional root password resets for customer clusters. Furthermore, PingCAP engineers routinely pasted sensitive customer production credentials (AWS keys, GitHub tokens, database connection strings) directly into Jira support tickets. Named affected customers include Booking.com, Shopee, Capcom, Mercari, Airbnb, Pinterest, and Databricks. A 200 GB stage-one release is now public.

---

## 21. Muse exposes users' personal and business secrets when they share conversations

**原文标题**: Muse exposes users' personal and business secrets when they share conversations

**原文链接**: [https://arstechnica.com/security/2026/10/meta-muse-exposes-users-personal-and-business-secrets-when-they-share-conversations/](https://arstechnica.com/security/2026/10/meta-muse-exposes-users-personal-and-business-secrets-when-they-share-conversations/)

生成摘要时出错

---

## 22. GitLab critical patch release

**原文标题**: GitLab critical patch release

**原文链接**: [https://docs.gitlab.com/releases/patches/patch-release-gitlab-19-5-1-released/](https://docs.gitlab.com/releases/patches/patch-release-gitlab-19-5-1-released/)

生成摘要时出错

---

## 23. Rust Style Guide

**原文标题**: Rust Style Guide

**原文链接**: [https://google.github.io/styleguide/rustguide.html](https://google.github.io/styleguide/rustguide.html)

生成摘要时出错

---

## 24. Woman faces six years in prison over Cash App account she never opened

**原文标题**: Woman faces six years in prison over Cash App account she never opened

**原文链接**: [https://www.techspot.com/news/114296-woman-spends-three-nights-jail-faces-six-years.html](https://www.techspot.com/news/114296-woman-spends-three-nights-jail-faces-six-years.html)

生成摘要时出错

---

## 25. CVE-2026-111943: Compromised Intermediate Certificate Authority

**原文标题**: CVE-2026-111943: Compromised Intermediate Certificate Authority

**原文链接**: [https://nvd.nist.gov/vuln/detail/cve-2026-111943](https://nvd.nist.gov/vuln/detail/cve-2026-111943)

生成摘要时出错

---

## 26. Mistral Large 4

**原文标题**: Mistral Large 4

**原文链接**: [https://mistral.ai/news/mistral-large-4/](https://mistral.ai/news/mistral-large-4/)

生成摘要时出错

---

## 27. OpenAI models are coming to Google Cloud

**原文标题**: OpenAI models are coming to Google Cloud

**原文链接**: [https://openai.com/index/openai-models-google-cloud/](https://openai.com/index/openai-models-google-cloud/)

生成摘要时出错

---

## 28. What’s getting pwned right now

**原文标题**: What’s getting pwned right now

**原文链接**: [https://pwn.watch/](https://pwn.watch/)

生成摘要时出错

---

## 29. Google cleared 300 hectares of Finnish forest

**原文标题**: Google cleared 300 hectares of Finnish forest

**原文链接**: [https://www.techspot.com/news/114100-google-cleared-300-hectares-finnish-forest-data-center.html](https://www.techspot.com/news/114100-google-cleared-300-hectares-finnish-forest-data-center.html)

生成摘要时出错

---

## 30. The Other Epidemic: Trying to get off benzodiazepines

**原文标题**: The Other Epidemic: Trying to get off benzodiazepines

**原文链接**: [https://www.thebeliever.net/the-other-epidemic/](https://www.thebeliever.net/the-other-epidemic/)

生成摘要时出错

---

## 31. The recently proposed o(n log n) integer multiplication algorithm [pdf]

**原文标题**: The recently proposed o(n log n) integer multiplication algorithm [pdf]

**原文链接**: [https://web.maths.unsw.edu.au/~davidharvey/research/subnlogn.pdf](https://web.maths.unsw.edu.au/~davidharvey/research/subnlogn.pdf)

生成摘要时出错

---

## 32. PHP 8.5.12, 8.4.27, 8.3.36 and 8.2.35 out

**原文标题**: PHP 8.5.12, 8.4.27, 8.3.36 and 8.2.35 out

**原文链接**: [https://www.php.net/index.php](https://www.php.net/index.php)

生成摘要时出错

---

## 33. Dutch National Cyber Security Center is Offline because it uses PHP

**原文标题**: Dutch National Cyber Security Center is Offline because it uses PHP

**原文链接**: [https://www.ncsc.nl/actueel](https://www.ncsc.nl/actueel)

生成摘要时出错

---

## 34. Show HN: Run full iOS 16.5 firmware on Android Devices

**原文标题**: Show HN: Run full iOS 16.5 firmware on Android Devices

**原文链接**: [https://github.com/oosexgang/hackios-xnu-kernel](https://github.com/oosexgang/hackios-xnu-kernel)

生成摘要时出错

---

## 35. Feds suspect ransom negotiator ran ShinyHunters extortion site

**原文标题**: Feds suspect ransom negotiator ran ShinyHunters extortion site

**原文链接**: [https://krebsonsecurity.com/2026/10/feds-suspect-ransom-negotiator-ran-shinyhunters-extortion-site/](https://krebsonsecurity.com/2026/10/feds-suspect-ransom-negotiator-ran-shinyhunters-extortion-site/)

生成摘要时出错

---

## 36. Patch the Planet: global response coordination as agents uncover vulnerabilities

**原文标题**: Patch the Planet: global response coordination as agents uncover vulnerabilities

**原文链接**: [https://openai.com/index/coordinated-disclosure-of-critical-vulnerabilities/](https://openai.com/index/coordinated-disclosure-of-critical-vulnerabilities/)

生成摘要时出错

---

## 37. Amazon identifies Oct 17 PHP2Shell exploitation prior to public disclosure

**原文标题**: Amazon identifies Oct 17 PHP2Shell exploitation prior to public disclosure

**原文链接**: [https://aws.amazon.com/blogs/security/amazon-threat-intelligence-identifies-php2shell-exploitation-prior-to-public-disclosure-in-madpot/](https://aws.amazon.com/blogs/security/amazon-threat-intelligence-identifies-php2shell-exploitation-prior-to-public-disclosure-in-madpot/)

生成摘要时出错

---

## 38. Airbnb bans making guests do dishes and take out the trash

**原文标题**: Airbnb bans making guests do dishes and take out the trash

**原文链接**: [https://www.theverge.com/tech/1015844/airbnb-chores-house-rules-update](https://www.theverge.com/tech/1015844/airbnb-chores-house-rules-update)

生成摘要时出错

---

## 39. Qwen3-Coder writes less secure code when told it's for a US persona

**原文标题**: Qwen3-Coder writes less secure code when told it's for a US persona

**原文链接**: [https://www.hirundo.io/blog/qwen3-coder-vulnerabilities](https://www.hirundo.io/blog/qwen3-coder-vulnerabilities)

生成摘要时出错

---

## 40. Several Linux kernel vulnerabilities accidentally posted to public mailing list

**原文标题**: Several Linux kernel vulnerabilities accidentally posted to public mailing list

**原文链接**: [https://www.phoronix.com/news/LKML-New-Trend-Vulnerabilities](https://www.phoronix.com/news/LKML-New-Trend-Vulnerabilities)

生成摘要时出错

---

## 41. OpenShell – A safe, private runtime for fleets of autonomous AI agents

**原文标题**: OpenShell – A safe, private runtime for fleets of autonomous AI agents

**原文链接**: [https://github.com/NVIDIA/OpenShell](https://github.com/NVIDIA/OpenShell)

生成摘要时出错

---

## 42. OpenAI CLI

**原文标题**: OpenAI CLI

**原文链接**: [https://github.com/openai/openai-cli](https://github.com/openai/openai-cli)

生成摘要时出错

---

## 43. MPs moving to restrict gambling ads in Canada

**原文标题**: MPs moving to restrict gambling ads in Canada

**原文链接**: [https://www.cbc.ca/news/investigates/gambling-ads-restrictions-canada-9.7388888](https://www.cbc.ca/news/investigates/gambling-ads-restrictions-canada-9.7388888)

生成摘要时出错

---

## 44. Good type against all odds

**原文标题**: Good type against all odds

**原文链接**: [https://unsung.aresluna.org/good-type-against-all-odds/](https://unsung.aresluna.org/good-type-against-all-odds/)

生成摘要时出错

---

## 45. Meta hit with $25B penalty for deceiving users about privacy on Facebook

**原文标题**: Meta hit with $25B penalty for deceiving users about privacy on Facebook

**原文链接**: [https://nmdoj.gov/press-release/the-new-mexico-department-of-justice-secures-another-landmark-victory-against-big-tech-with-historic-25-billion-penalty-against-facebook/](https://nmdoj.gov/press-release/the-new-mexico-department-of-justice-secures-another-landmark-victory-against-big-tech-with-historic-25-billion-penalty-against-facebook/)

生成摘要时出错

---

## 46. A farewell to Arc browser

**原文标题**: A farewell to Arc browser

**原文链接**: [https://arc.net/](https://arc.net/)

生成摘要时出错

---

## 47. Using LLM for confidence scoring is a bad idea

**原文标题**: Using LLM for confidence scoring is a bad idea

**原文链接**: [https://rumple.github.io/blog/2026/10/20/asking-llm-for-confidence.html](https://rumple.github.io/blog/2026/10/20/asking-llm-for-confidence.html)

生成摘要时出错

---

## 48. Whatever Happened to Fire Escapes

**原文标题**: Whatever Happened to Fire Escapes

**原文链接**: [https://practical.engineering/blog/2026/10/20/whatever-happened-to-fire-escapes](https://practical.engineering/blog/2026/10/20/whatever-happened-to-fire-escapes)

生成摘要时出错

---

## 49. Oregon lawmakers approve money to buy an iconic waterfall listed on Redfin

**原文标题**: Oregon lawmakers approve money to buy an iconic waterfall listed on Redfin

**原文链接**: [https://apnews.com/article/oregon-waterfall-for-sale-lawmakers-996de63462d49ec3ad9bee1629fb9488](https://apnews.com/article/oregon-waterfall-for-sale-lawmakers-996de63462d49ec3ad9bee1629fb9488)

生成摘要时出错

---

## 50. Faster than earcut: triangulating 3.7M map polygons in 489 ms

**原文标题**: Faster than earcut: triangulating 3.7M map polygons in 489 ms

**原文链接**: [https://globus.software/blog/2026/10/16/cutting-map-polygons/](https://globus.software/blog/2026/10/16/cutting-map-polygons/)

生成摘要时出错

---

## 51. PHP session.upload_progress heap UAF (CVE-2026-109618 / -109619)

**原文标题**: PHP session.upload_progress heap UAF (CVE-2026-109618 / -109619)

**原文链接**: [https://jackalsyn.com/posts/php-up-2026.html](https://jackalsyn.com/posts/php-up-2026.html)

生成摘要时出错

---

## 52. Epic Games Inc v Apple Inc

**原文标题**: Epic Games Inc v Apple Inc

**原文链接**: [https://www.judgments.fedcourt.gov.au/judgments/Judgments/fca/single/2026/2026fca1552](https://www.judgments.fedcourt.gov.au/judgments/Judgments/fca/single/2026/2026fca1552)

生成摘要时出错

---

## 53. Getting ready to operate GNU Taler in Germany

**原文标题**: Getting ready to operate GNU Taler in Germany

**原文链接**: [https://www.taler.net/en/news/2026-13.html](https://www.taler.net/en/news/2026-13.html)

生成摘要时出错

---

## 54. Crystal 1.22

**原文标题**: Crystal 1.22

**原文链接**: [https://crystal-lang.org/2026/10/12/1.22.0-released/](https://crystal-lang.org/2026/10/12/1.22.0-released/)

生成摘要时出错

---

## 55. Canary Tokens

**原文标题**: Canary Tokens

**原文链接**: [https://canarytokens.org/](https://canarytokens.org/)

生成摘要时出错

---

## 56. C# now beats Rust on WASM size

**原文标题**: C# now beats Rust on WASM size

**原文链接**: [https://github.com/zion-sati/NetWasm](https://github.com/zion-sati/NetWasm)

生成摘要时出错

---

## 57. Plex laid off the whole player team

**原文标题**: Plex laid off the whole player team

**原文链接**: [https://forums.plex.tv/t/2026-20-0-beta-ios-and-tvos-4k-dovi-hdr10-won-t-play-infinite-spinning-circle/943966?page=5](https://forums.plex.tv/t/2026-20-0-beta-ios-and-tvos-4k-dovi-hdr10-won-t-play-infinite-spinning-circle/943966?page=5)

生成摘要时出错

---

## 58. Using thousands of AI agents to uncover new leads in biological data

**原文标题**: Using thousands of AI agents to uncover new leads in biological data

**原文链接**: [https://openai.com/index/scaling-ai-research-for-complex-biological-data/](https://openai.com/index/scaling-ai-research-for-complex-biological-data/)

生成摘要时出错

---

## 59. The compiler was supposed to end programming too

**原文标题**: The compiler was supposed to end programming too

**原文链接**: [https://hrih.si/articles/the-compiler-was-supposed-to-end-programming/](https://hrih.si/articles/the-compiler-was-supposed-to-end-programming/)

生成摘要时出错

---

## 60. Most advice is right for the person giving it

**原文标题**: Most advice is right for the person giving it

**原文链接**: [https://coached.com/essays/most-advice-is-right-for-the-person-giving-it/](https://coached.com/essays/most-advice-is-right-for-the-person-giving-it/)

生成摘要时出错

---

## 61. In Hilbert space, all things are quantumly possible

**原文标题**: In Hilbert space, all things are quantumly possible

**原文链接**: [https://www.quantamagazine.org/in-hilbert-space-all-things-are-quantumly-possible-20260826/](https://www.quantamagazine.org/in-hilbert-space-all-things-are-quantumly-possible-20260826/)

生成摘要时出错

---

## 62. A complete bypass of eMudhra’s 1FA OTP login system

**原文标题**: A complete bypass of eMudhra’s 1FA OTP login system

**原文链接**: [https://mastodon.catgirl.cloud/@49016/117475976434068995](https://mastodon.catgirl.cloud/@49016/117475976434068995)

生成摘要时出错

---

## 63. Xbox wants you to pay 24 to 40 cents per hour to stream games you bought

**原文标题**: Xbox wants you to pay 24 to 40 cents per hour to stream games you bought

**原文链接**: [https://arstechnica.com/gaming/2026/10/xbox-wants-you-to-pay-24-to-40-cents-per-hour-to-stream-games-you-already-bought/](https://arstechnica.com/gaming/2026/10/xbox-wants-you-to-pay-24-to-40-cents-per-hour-to-stream-games-you-already-bought/)

生成摘要时出错

---

## 64. 使用 Claude 减少代码攻击面

**原文标题**: Using Claude to reduce the attack surface of code

**原文链接**: [https://www.anthropic.com/research/attack-surface-reduction](https://www.anthropic.com/research/attack-surface-reduction)

生成摘要时出错

---

## 65. New plastic pollution discovered: 'Plasticorals' coral rubble fused with plastic

**原文标题**: New plastic pollution discovered: 'Plasticorals' coral rubble fused with plastic

**原文链接**: [https://www.oist.jp/news-center/news/2026/9/18/new-form-plastic-pollution-discovered-shores-vulnerable-coral-reefs](https://www.oist.jp/news-center/news/2026/9/18/new-form-plastic-pollution-discovered-shores-vulnerable-coral-reefs)

生成摘要时出错

---

## 66. Cloudflare deploys protections against php2shell vulnerability

**原文标题**: Cloudflare deploys protections against php2shell vulnerability

**原文链接**: [https://blog.cloudflare.com/php-vulnerabilities-waf-protection/](https://blog.cloudflare.com/php-vulnerabilities-waf-protection/)

生成摘要时出错

---

## 67. Google staff resign in backlash over its AI contracts with military

**原文标题**: Google staff resign in backlash over its AI contracts with military

**原文链接**: [https://www.bbc.com/news/articles/cmreyvepnv0po](https://www.bbc.com/news/articles/cmreyvepnv0po)

生成摘要时出错

---

## 68. Every AI model has the same "controversial" take on humans

**原文标题**: Every AI model has the same "controversial" take on humans

**原文链接**: [https://www.modelcompare.ai/blog/ai-models-controversial-take-on-humans](https://www.modelcompare.ai/blog/ai-models-controversial-take-on-humans)

生成摘要时出错

---

## 69. PHP web runtimes (CVE-2026-109618 and CVE-2026-109619)

**原文标题**: PHP web runtimes (CVE-2026-109618 and CVE-2026-109619)

**原文链接**: [https://aws.amazon.com/security/security-bulletins/2026-143-aws/](https://aws.amazon.com/security/security-bulletins/2026-143-aws/)

生成摘要时出错

---

## 70. Show HN: Omnara – Open-source alternative to Claude Managed Agents

**原文标题**: Show HN: Omnara – Open-source alternative to Claude Managed Agents

**原文链接**: [https://github.com/omnara-ai/omnara](https://github.com/omnara-ai/omnara)

生成摘要时出错

---

## 71. The Last Museum: Semantic search across 5.8M artworks from major museums

**原文标题**: The Last Museum: Semantic search across 5.8M artworks from major museums

**原文链接**: [https://lastmuseum.com/](https://lastmuseum.com/)

生成摘要时出错

---

## 72. Show HN: Sumi.css – CSS Framework

**原文标题**: Show HN: Sumi.css – CSS Framework

**原文链接**: [https://github.com/vladocar/Sumi.css](https://github.com/vladocar/Sumi.css)

生成摘要时出错

---

## 73. Setting Up SSH Keys on macOS with Touch ID

**原文标题**: Setting Up SSH Keys on macOS with Touch ID

**原文链接**: [https://nmattia.com/posts/2026-10-19-setting-up-ssh-keys-touch-id/](https://nmattia.com/posts/2026-10-19-setting-up-ssh-keys-touch-id/)

生成摘要时出错

---

## 74. Claude Duet

**原文标题**: Claude Duet

**原文链接**: [https://claude.com/resources/articles/claude-duet](https://claude.com/resources/articles/claude-duet)

生成摘要时出错

---

## 75. Tesla profits drop 43% in Q3

**原文标题**: Tesla profits drop 43% in Q3

**原文链接**: [https://arstechnica.com/cars/2026/10/tesla-profits-drop-43-in-q3/](https://arstechnica.com/cars/2026/10/tesla-profits-drop-43-in-q3/)

生成摘要时出错

---

## 76. Claude Now Works with Google Docs, Sheets, and Slides

**原文标题**: Claude Now Works with Google Docs, Sheets, and Slides

**原文链接**: [https://claude.com/resources/articles/claude-now-works-in-google-docs-sheets-and-slides](https://claude.com/resources/articles/claude-now-works-in-google-docs-sheets-and-slides)

生成摘要时出错

---

## 77. What I learned from six months of being stupid on purpose

**原文标题**: What I learned from six months of being stupid on purpose

**原文链接**: [https://wvez.org/blog/learning-to-be-stupid/](https://wvez.org/blog/learning-to-be-stupid/)

生成摘要时出错

---

## 78. Hedra is a 3D open world game I wrote from scratch while in highschool

**原文标题**: Hedra is a 3D open world game I wrote from scratch while in highschool

**原文链接**: [https://github.com/maxilevi/project-hedra/tree/pre-ai](https://github.com/maxilevi/project-hedra/tree/pre-ai)

生成摘要时出错

---

## 79. I told people I'm a convicted felon after 20 years of hiding it

**原文标题**: I told people I'm a convicted felon after 20 years of hiding it

**原文链接**: [https://buford.bg/](https://buford.bg/)

生成摘要时出错

---

## 80. AI and the Enclosure of the Scientific Commons

**原文标题**: AI and the Enclosure of the Scientific Commons

**原文链接**: [https://arxiv.org/abs/2610.27251](https://arxiv.org/abs/2610.27251)

生成摘要时出错

---

## 81. Rust off Rails: The opinionated web stack for the AI era

**原文标题**: Rust off Rails: The opinionated web stack for the AI era

**原文链接**: [https://rustoffrails.org/](https://rustoffrails.org/)

生成摘要时出错

---

## 82. LayerFS: A filesystem for AI coding agents

**原文标题**: LayerFS: A filesystem for AI coding agents

**原文链接**: [https://layerfs.ai/](https://layerfs.ai/)

生成摘要时出错

---

## 83. Victory! Court Rules OPM Data Disclosure to DOGE Is Unlawful

**原文标题**: Victory! Court Rules OPM Data Disclosure to DOGE Is Unlawful

**原文链接**: [https://www.eff.org/deeplinks/2026/10/victory-court-rules-opms-disclosure-personal-records-doge-unlawful](https://www.eff.org/deeplinks/2026/10/victory-court-rules-opms-disclosure-personal-records-doge-unlawful)

生成摘要时出错

---

## 84. Potential third critical PHP CVE

**原文标题**: Potential third critical PHP CVE

**原文链接**: [https://elk.zone/m.webtoo.ls/@elise@katze.sh/117479383721672027](https://elk.zone/m.webtoo.ls/@elise@katze.sh/117479383721672027)

生成摘要时出错

---

## 85. SCOTUS couldn't take up a copyright case because four justices have book deals

**原文标题**: SCOTUS couldn't take up a copyright case because four justices have book deals

**原文链接**: [https://news.bloomberglaw.com/ip-law/supreme-court-affirms-foreign-rights-ruling-after-lacking-quorum](https://news.bloomberglaw.com/ip-law/supreme-court-affirms-foreign-rights-ruling-after-lacking-quorum)

生成摘要时出错

---

## 86. The bridge to agent-scale Git infrastructure

**原文标题**: The bridge to agent-scale Git infrastructure

**原文链接**: [https://github.blog/engineering/architecture-optimization/the-bridge-to-agent-scale-git-infrastructure/](https://github.blog/engineering/architecture-optimization/the-bridge-to-agent-scale-git-infrastructure/)

生成摘要时出错

---

## 87. I can't believe PowerShell is good

**原文标题**: I can't believe PowerShell is good

**原文链接**: [https://www.spacebar.news/powershell-is-actually-good/](https://www.spacebar.news/powershell-is-actually-good/)

生成摘要时出错

---

## 88. Launch HN: Alter (YC S25) – Access control for multi-user agents

**原文标题**: Launch HN: Alter (YC S25) – Access control for multi-user agents

**原文链接**: [https://alterauth.com/](https://alterauth.com/)

生成摘要时出错

---

## 89. Your MCU likely escaped the eMudhra intermediate CA compromise

**原文标题**: Your MCU likely escaped the eMudhra intermediate CA compromise

**原文链接**: [https://danielmangum.com/posts/mcu-emudhra-intermediate-ca-compromise/](https://danielmangum.com/posts/mcu-emudhra-intermediate-ca-compromise/)

生成摘要时出错

---

## 90. People sick of being spied on by their smart TV

**原文标题**: People sick of being spied on by their smart TV

**原文链接**: [https://www.theguardian.com/tv-and-radio/2026/oct/20/smart-tv-television-dumb-wifi-techies-privacy](https://www.theguardian.com/tv-and-radio/2026/oct/20/smart-tv-television-dumb-wifi-techies-privacy)

生成摘要时出错

---

## 91. CDC Ignored Request from States to Validate a New Measles Test

**原文标题**: CDC Ignored Request from States to Validate a New Measles Test

**原文链接**: [https://www.nytimes.com/2026/10/21/health/measles-test-cdc.html](https://www.nytimes.com/2026/10/21/health/measles-test-cdc.html)

生成摘要时出错

---

## 92. How the CIA Gave Steve Jobs Top Secret Clearance and Helped Him Return to Apple

**原文标题**: How the CIA Gave Steve Jobs Top Secret Clearance and Helped Him Return to Apple

**原文链接**: [https://brianroemmele.substack.com/p/how-the-cia-gave-steve-jobs-a-top](https://brianroemmele.substack.com/p/how-the-cia-gave-steve-jobs-a-top)

生成摘要时出错

---

## 93. AI analysis of CT scans finds 42.9% of patients have coronary inflammation

**原文标题**: AI analysis of CT scans finds 42.9% of patients have coronary inflammation

**原文链接**: [https://www.biograph.com/newsroom/biograph-completes-first-u.s.-study-with-caristo-diagnostics%E2%80%99-ai-powered-coronary-inflammation-detection-finding-risk-in-over-42-of-asymptomatic-patients](https://www.biograph.com/newsroom/biograph-completes-first-u.s.-study-with-caristo-diagnostics%E2%80%99-ai-powered-coronary-inflammation-detection-finding-risk-in-over-42-of-asymptomatic-patients)

生成摘要时出错

---

## 94. A Markdown File Should Just Open

**原文标题**: A Markdown File Should Just Open

**原文链接**: [https://joshuamorris.info/notes/2026/10/13/a-markdown-file-should-just-open/](https://joshuamorris.info/notes/2026/10/13/a-markdown-file-should-just-open/)

生成摘要时出错

---

## 95. Show HN: UI micro interactions prompts for AI

**原文标题**: Show HN: UI micro interactions prompts for AI

**原文链接**: [https://www.typeui.sh/micro-interactions](https://www.typeui.sh/micro-interactions)

生成摘要时出错

---

## 96. Show HN: Uberblok – an interactive museum of ZFS internals

**原文标题**: Show HN: Uberblok – an interactive museum of ZFS internals

**原文链接**: [https://uberblok.storagebits.workers.dev/](https://uberblok.storagebits.workers.dev/)

生成摘要时出错

---

## 97. Pillowfort Is Closing

**原文标题**: Pillowfort Is Closing

**原文链接**: [https://www.pillowfort.social/posts/8413273](https://www.pillowfort.social/posts/8413273)

生成摘要时出错

---

## 98. Someone Opened a CashApp in Her Name. She Faces Years in Prison

**原文标题**: Someone Opened a CashApp in Her Name. She Faces Years in Prison

**原文链接**: [https://www.404media.co/amanda-smith-opened-a-cashapp-in-her-name-she-faces-years-in-prison-cashapp-fraud/](https://www.404media.co/amanda-smith-opened-a-cashapp-in-her-name-she-faces-years-in-prison-cashapp-fraud/)

生成摘要时出错

---

## 99. Texas data center boom could erase decades of progress on air quality

**原文标题**: Texas data center boom could erase decades of progress on air quality

**原文链接**: [https://www.texastribune.org/2026/10/20/data-centers-texas-air-quality-report-pollution-health-risks/](https://www.texastribune.org/2026/10/20/data-centers-texas-air-quality-report-pollution-health-risks/)

生成摘要时出错

---

## 100. Delays for Pull Requests and Webhook deliveries

**原文标题**: Delays for Pull Requests and Webhook deliveries

**原文链接**: [https://www.githubstatus.com/incidents/nms1dpzmh9d9](https://www.githubstatus.com/incidents/nms1dpzmh9d9)

生成摘要时出错

---

