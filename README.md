# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-10-22.md)

*最后自动更新时间: 2026-10-22 22:36:53*
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

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-10-22](output/hacker_news_summary_2026-10-22.md) |
| 2 | [2026-10-17](output/hacker_news_summary_2026-10-17.md) |
| 3 | [2026-10-18](output/hacker_news_summary_2026-10-18.md) |
| 4 | [2026-10-15](output/hacker_news_summary_2026-10-15.md) |
| 5 | [2026-10-16](output/hacker_news_summary_2026-10-16.md) |
| 6 | [2026-10-21](output/hacker_news_summary_2026-10-21.md) |
| 7 | [2026-10-20](output/hacker_news_summary_2026-10-20.md) |
| 8 | [2026-10-19](output/hacker_news_summary_2026-10-19.md) |
| 9 | [2026-10-13](output/hacker_news_summary_2026-10-13.md) |
| 10 | [2026-10-07](output/hacker_news_summary_2026-10-07.md) |
| 11 | [2026-10-06](output/hacker_news_summary_2026-10-06.md) |
| 12 | [2026-10-04](output/hacker_news_summary_2026-10-04.md) |
| 13 | [2026-10-14](output/hacker_news_summary_2026-10-14.md) |
| 14 | [2026-10-10](output/hacker_news_summary_2026-10-10.md) |
| 15 | [2026-10-09](output/hacker_news_summary_2026-10-09.md) |
| 16 | [2026-10-11](output/hacker_news_summary_2026-10-11.md) |
| 17 | [2026-09-24](output/hacker_news_summary_2026-09-24.md) |
| 18 | [2026-10-01](output/hacker_news_summary_2026-10-01.md) |
| 19 | [2026-09-29](output/hacker_news_summary_2026-09-29.md) |
| 20 | [2026-09-30](output/hacker_news_summary_2026-09-30.md) |
| 21 | [2026-10-02](output/hacker_news_summary_2026-10-02.md) |
| 22 | [2026-09-27](output/hacker_news_summary_2026-09-27.md) |
| 23 | [2026-10-03](output/hacker_news_summary_2026-10-03.md) |
| 24 | [2026-09-25](output/hacker_news_summary_2026-09-25.md) |
| 25 | [2026-09-21](output/hacker_news_summary_2026-09-21.md) |
| 26 | [2026-09-23](output/hacker_news_summary_2026-09-23.md) |
| 27 | [2026-09-20](output/hacker_news_summary_2026-09-20.md) |
| 28 | [2026-09-16](output/hacker_news_summary_2026-09-16.md) |
| 29 | [2026-09-22](output/hacker_news_summary_2026-09-22.md) |
| 30 | [2026-09-17](output/hacker_news_summary_2026-09-17.md) |
| 31 | [2026-09-19](output/hacker_news_summary_2026-09-19.md) |
| 32 | [2026-09-18](output/hacker_news_summary_2026-09-18.md) |
| 33 | [2026-09-09](output/hacker_news_summary_2026-09-09.md) |
| 34 | [2026-09-10](output/hacker_news_summary_2026-09-10.md) |
| 35 | [2026-09-13](output/hacker_news_summary_2026-09-13.md) |
| 36 | [2026-09-08](output/hacker_news_summary_2026-09-08.md) |
| 37 | [2026-09-14](output/hacker_news_summary_2026-09-14.md) |
| 38 | [2026-09-11](output/hacker_news_summary_2026-09-11.md) |
| 39 | [2026-09-12](output/hacker_news_summary_2026-09-12.md) |
| 40 | [2026-09-15](output/hacker_news_summary_2026-09-15.md) |
| 41 | [2026-09-03](output/hacker_news_summary_2026-09-03.md) |
| 42 | [2026-09-02](output/hacker_news_summary_2026-09-02.md) |
| 43 | [2026-08-31](output/hacker_news_summary_2026-08-31.md) |
| 44 | [2026-09-04](output/hacker_news_summary_2026-09-04.md) |
| 45 | [2026-09-05](output/hacker_news_summary_2026-09-05.md) |
| 46 | [2026-09-01](output/hacker_news_summary_2026-09-01.md) |
| 47 | [2026-08-29](output/hacker_news_summary_2026-08-29.md) |
| 48 | [2026-09-07](output/hacker_news_summary_2026-09-07.md) |
| 49 | [2026-08-30](output/hacker_news_summary_2026-08-30.md) |
| 50 | [2026-09-06](output/hacker_news_summary_2026-09-06.md) |
| 51 | [2026-08-22](output/hacker_news_summary_2026-08-22.md) |
| 52 | [2026-08-25](output/hacker_news_summary_2026-08-25.md) |
| 53 | [2026-08-19](output/hacker_news_summary_2026-08-19.md) |
| 54 | [2026-08-20](output/hacker_news_summary_2026-08-20.md) |
| 55 | [2026-08-17](output/hacker_news_summary_2026-08-17.md) |
| 56 | [2026-08-28](output/hacker_news_summary_2026-08-28.md) |
| 57 | [2026-08-23](output/hacker_news_summary_2026-08-23.md) |
| 58 | [2026-08-18](output/hacker_news_summary_2026-08-18.md) |
| 59 | [2026-08-21](output/hacker_news_summary_2026-08-21.md) |
| 60 | [2026-08-24](output/hacker_news_summary_2026-08-24.md) |
| 61 | [2026-08-26](output/hacker_news_summary_2026-08-26.md) |
| 62 | [2026-08-12](output/hacker_news_summary_2026-08-12.md) |
| 63 | [2026-08-11](output/hacker_news_summary_2026-08-11.md) |
| 64 | [2026-08-14](output/hacker_news_summary_2026-08-14.md) |
| 65 | [2026-08-16](output/hacker_news_summary_2026-08-16.md) |
| 66 | [2026-08-10](output/hacker_news_summary_2026-08-10.md) |
| 67 | [2026-08-09](output/hacker_news_summary_2026-08-09.md) |
| 68 | [2026-08-15](output/hacker_news_summary_2026-08-15.md) |
| 69 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 70 | [2026-08-13](output/hacker_news_summary_2026-08-13.md) |
| 71 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 72 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 73 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 74 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 75 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 76 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 77 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 78 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 79 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 80 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 81 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 82 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 83 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 84 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 85 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 86 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 87 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 88 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 89 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 90 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 91 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 92 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 93 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 94 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 95 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 96 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 97 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 98 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 99 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 100 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 101 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 102 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 103 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 104 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 105 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 106 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 107 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 108 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 109 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 110 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 111 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 112 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 113 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 114 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 115 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 116 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 117 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 118 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 119 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 120 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 121 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 122 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 123 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 124 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 125 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 126 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 127 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 128 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 129 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 130 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 131 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 132 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 133 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 134 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 135 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 136 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 137 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 138 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 139 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 140 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 141 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 142 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 143 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 144 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 145 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 146 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 147 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 148 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 149 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 150 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 151 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 152 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 153 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 154 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 155 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 156 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 157 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 158 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 159 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 160 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 161 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 162 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 163 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 164 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 165 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 166 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 167 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 168 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 169 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 170 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 171 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 172 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 173 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 174 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 175 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 176 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 177 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 178 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 179 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 180 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 181 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 182 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 183 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 184 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 185 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 186 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 187 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 188 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 189 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 190 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 191 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 192 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 193 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 194 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 195 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 196 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 197 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 198 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 199 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 200 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 201 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 202 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 203 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 204 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 205 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 206 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 207 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 208 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 209 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 210 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 211 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 212 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 213 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 214 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 215 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 216 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 217 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 218 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 219 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 220 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 221 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 222 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 223 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 224 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 225 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 226 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 227 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 228 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 229 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 230 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 231 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 232 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 233 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 234 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 235 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 236 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 237 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 238 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 239 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 240 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 241 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 242 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 243 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 244 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 245 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 246 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 247 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 248 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 249 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 250 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 251 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 252 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 253 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 254 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 255 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 256 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 257 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 258 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 259 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 260 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 261 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 262 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 263 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 264 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 265 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 266 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 267 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 268 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 269 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 270 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 271 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 272 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 273 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 274 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 275 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 276 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 277 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 278 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 279 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 280 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 281 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 282 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 283 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 284 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 285 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 286 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 287 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 288 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 289 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 290 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 291 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 292 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 293 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 294 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 295 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 296 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 297 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 298 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 299 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 300 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 301 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 302 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 303 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 304 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 305 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 306 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 307 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 308 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 309 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 310 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 311 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 312 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 313 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 314 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 315 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 316 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 317 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 318 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 319 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 320 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 321 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 322 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 323 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 324 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 325 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 326 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 327 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 328 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 329 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 330 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 331 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 332 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 333 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 334 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 335 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 336 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
| 337 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 338 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 339 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 340 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 341 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 342 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
