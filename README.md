# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-06-28.md)

*最后自动更新时间: 2026-06-28 20:39:15*
## 1. 匿名 GitHub 账号批量投放未公开的零日漏洞

**原文标题**: Anonymous GitHub account mass-dropping undisclosed 0-days

**原文链接**: [https://github.com/bikini/exploitarium](https://github.com/bikini/exploitarium)

An anonymous GitHub account, identified by Discord handle `@ashdfrkl`, has launched "Exploitarium," a public repository mass-dropping undisclosed 0-day vulnerabilities. The author, a researcher with a degree and published papers in fuzzing methodology, acknowledges initial findings were "kinda ass" but promises future drops will be high-quality, focusing on projects like Floci, libssh2, FFmpeg, and c-ares.

The researcher clarifies their use of AI: GPT-5.5-3-Codex-Spark automated the fuzzing workflow with a strict harness, not for "vibe-coding" or generating PoCs (except for RustDesk due to language unfamiliarity). They emphasize that efficient harnesses and human oversight are more crucial than state-of-the-art AI models for identifying issues. README files, however, are AI-generated and reviewed.

The repository includes a diverse collection of vulnerabilities for applications like 7zip, Anydesk, Docker, Firefox, Ghidra, ImageMagick, Nmap, PHP, VLC, and several others. Some entries are preserved from older standalone repos, while others are new, direct additions. The author credits another researcher for a superior `objdump` finding.

Promising a major new drop soon, followed by daily PoCs, the author also plans to broaden PoC usability. They invite collaboration via Discord and stress that the research is for good-faith, open disclosure, explicitly condemning malicious use.

---

## 2. DSpark: Speculative decoding accelerates LLM inference [pdf]

**原文标题**: DSpark: Speculative decoding accelerates LLM inference [pdf]

**原文链接**: [https://github.com/deepseek-ai/DeepSpec/blob/main/DSpark_paper.pdf](https://github.com/deepseek-ai/DeepSpec/blob/main/DSpark_paper.pdf)

生成摘要时出错

---

## 3. OpenRA

**原文标题**: OpenRA

**原文链接**: [https://www.openra.net/](https://www.openra.net/)

生成摘要时出错

---

## 4. Zuckerberg's war on whistleblowers

**原文标题**: Zuckerberg's war on whistleblowers

**原文链接**: [https://pluralistic.net/2026/06/27/zuckerstreisand-2/](https://pluralistic.net/2026/06/27/zuckerstreisand-2/)

生成摘要时出错

---

## 5. 金融科技工程手册

**原文标题**: Fintech Engineering Handbook

**原文链接**: [https://w.pitula.me/fintech-engineering-handbook/](https://w.pitula.me/fintech-engineering-handbook/)

The Fintech Engineering Handbook outlines critical software engineering patterns for reliable money systems, targeting fintech professionals and newcomers. It's built on three principles: **No invented data** (preventing duplicates/arbitrary updates via idempotency, deduplication, reconciliation), **No lost data** (tracking everything with full precision, at-least-once delivery, event sourcing, audit trails, immutability), and **No trust** (verifying external/internal components and failing loudly).

**Representing Money** covers fundamental decisions:
*   **Precision handling:** Avoid floating-points; prefer arbitrary precision (e.g., BigDecimal), minor-units (integers for smallest units, careful with crypto's high decimals), or rational numbers. Serialize money as a string or smallest-unit integer to prevent precision loss.
*   **Rounding strategies:** Explicit, business-driven, round as seldom as possible, and acknowledge that rounding can break sums.
*   **Currency handling:** Always pair amount with currency in a custom type. Prohibit cross-currency arithmetic without explicit conversion. Use controlled currency sets and understand that crypto requires network/contract address for identification.
*   **FX Rates:** Rates are directional and time-sensitive (current vs. value date). Distinguish transactional rates from reference rates, and note that there's no single canonical rate, so sources are crucial.

**Recording Money: The Ledger** details how money movements are tracked:
*   **Double-entry bookkeeping:** The core method, where every transaction (credit, debit, amount) ensures books always balance. Balances are derived, not stored, and accounts are typed. Posted entries are immutable, with corrections made by new compensating entries.
*   **Value time vs. Booking time vs. Settlement time:** Differentiate these critical timestamps, as they often diverge and are important for various reporting and traceability needs.
*   **Audits and audit trails:** Systems require robust audit trails to explain state changes (what, when, who, why) for regulatory scrutiny, covering money movements, manual interventions, and configuration changes.
*   **Event sourcing:** A principled approach where state is derived from an immutable stream of events (the ledger itself is an example), ensuring the audit trail is the source of truth, though it adds system complexity.
*   **Immutability:** Records must be append-only, with updates/deletions forbidden. Corrections are new records. This is enforced through construction, runtime checks, or tamper-evidence mechanisms.

---

## 6. U.S. allows Anthropic to release Mythos AI to ‘trusted’ US organizations

**原文标题**: U.S. allows Anthropic to release Mythos AI to ‘trusted’ US organizations

**原文链接**: [https://www.semafor.com/article/06/27/2026/us-releases-powerful-anthropic-model-mythos-to-some-us-companies](https://www.semafor.com/article/06/27/2026/us-releases-powerful-anthropic-model-mythos-to-some-us-companies)

生成摘要时出错

---

## 7. Om

**原文标题**: Om

**原文链接**: [https://daringfireball.net/2026/06/om](https://daringfireball.net/2026/06/om)

生成摘要时出错

---

## 8. 我们仍能阻止加州3D打印机监控方案

**原文标题**: We can still stop California's 3D printer surveillance scheme

**原文链接**: [https://www.eff.org/deeplinks/2026/06/we-can-still-stop-californias-3d-printer-surveillance-scheme](https://www.eff.org/deeplinks/2026/06/we-can-still-stop-californias-3d-printer-surveillance-scheme)

The California State Assembly has advanced AB 2047, a bill mandating surveillance software for 3D printers, despite warnings from the EFF about its dangers and impracticality. The legislation, initially aimed at preventing unlicensed firearm manufacturing, is opposed due to severe risks to privacy, free speech, and consumer rights, while being ineffective for its stated purpose.

While a welcome amendment removed criminalization for the private resale of 3D printers, most changes have exacerbated concerns. Carveouts for open-source tools are deemed insufficient, as they still require developers to integrate "compliant censorship software," burdening them with ambiguous standards and chilling open-source experimentation.

Crucially, the bill drops any pretense of the technology actually working, changing its performance standard from "effectively prevent" circumvention to merely "substantially reduce the likelihood of foreseeable circumvention attempts." This maintains surveillance on all prints but acknowledges its futility against determined users, creating an unclear process reliant on non-governmental bodies and self-policing.

A new carveout benefits large entertainment studios, exempting them from surveillance, but excludes indie filmmakers, cosplayers, and small creators. This creates a two-tiered system and raises risks of IP theft for surveilled commercial users.

The article concludes that this "printer surveillance system" will not achieve its intended goal but will instead harm law-abiding users through ineffective, invasive surveillance. It urges California Senators to oppose AB 2047 and protect creators' tools.

---

## 9. The case for physical media ownership

**原文标题**: The case for physical media ownership

**原文链接**: [https://dervis.de/physical/](https://dervis.de/physical/)

The article argues that digital media purchases typically grant a revocable license rather than true ownership, in stark contrast to physical media like Blu-rays, game cartridges, or books. This distinction has significant implications for consumers.

Physical media can be owned, resold, lent, archived, and used offline, retaining secondary market value. Digital licenses, however, are often tied to accounts, non-transferable, and lack resale value. Court rulings, like the ReDigi case, confirm that the first-sale doctrine doesn't apply to digital files.

A primary concern is the potential for content removal. Digital items can disappear due to licensing expirations, policy changes, or even store shutdowns. Numerous examples highlight this, including Disney+ and HBO Max removing original titles, Sony delisting purchased content from PlayStation Store, Konami's P.T. demo, and various games being delisted (Scott Pilgrim, Deadpool). Furthermore, digital storefronts like Microsoft's ebook store, Google Play Music, Nintendo's eShops, and Google Stadia have shut down, often rendering purchased content inaccessible.

Subscriptions, a common model for digital access, entail continuous payments that can increase (e.g., Netflix, Adobe Creative Cloud). If payments stop, access is lost, unlike a one-time physical purchase.

Quality also differs; physical Blu-rays offer significantly higher video bitrates and lossless audio compared to compressed streaming, providing a more faithful experience independent of internet conditions.

Finally, digital content is susceptible to remote alteration or censorship, as seen with Amazon removing books from Kindles, Disney+ editing classic films, and Rockstar altering games in remasters. Physical media, once acquired, remains in its original form, offering greater control and permanence.

---

## 10. 欧盟将闭门立法聊天监控。

**原文标题**: EU to legislate about Chat Control behind closed doors

**原文链接**: [https://www.patrick-breyer.de/en/double-threat-to-private-communications-undemocratic-chat-control-backroom-deals-and-imminent-concessions-spark-relaunch-of-fightchatcontrol-eu/](https://www.patrick-breyer.de/en/double-threat-to-private-communications-undemocratic-chat-control-backroom-deals-and-imminent-concessions-spark-relaunch-of-fightchatcontrol-eu/)

Civil rights activist Dr. Patrick Breyer warns of an unprecedented "double-attack" by EU institutions threatening secure messaging and anonymous communication. Ahead of critical EU meetings this Friday and Monday, Breyer highlights two significant threats.

Firstly, European Parliament President Roberta Metsola is reportedly attempting an undemocratic "power play" to resurrect the expired "Chat Control 1.0" mass scanning regime. This move, which ignores the Parliament's prior rejection, is being pushed via a Council meeting this Friday to adopt a first-reading position.

Secondly, on Monday, final trilogue negotiations for the permanent "Chat Control 2.0" (CSAR) regulation will take place. Breyer fears the European Parliament is rushing a new mandate on detection/scanning, potentially leading to "fatal concessions." The worst-case scenario includes the return of mass scanning of private messages (potentially made mandatory), warrantless scanning orders without court approval, and mandatory age verification for online services, effectively ending anonymous communication.

In response, the civil society campaign fightchatcontrol.eu has been urgently relaunched, enabling citizens to email EU lawmakers and government representatives. Breyer emphasizes that genuine child protection is achievable through targeted investigations, security-by-design, and proactive darknet deletion, rather than error-prone algorithms that undermine fundamental rights. He urges citizens to take action this weekend to defend digital civil liberties.

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 2 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 3 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 4 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 5 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 6 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 7 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 8 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 9 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 10 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 11 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 12 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 13 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 14 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 15 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 16 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 17 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 18 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 19 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 20 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 21 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 22 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 23 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 24 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 25 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 26 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 27 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 28 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 29 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 30 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 31 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 32 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 33 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 34 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 35 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 36 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 37 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 38 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 39 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 40 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 41 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 42 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 43 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 44 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 45 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 46 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 47 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 48 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 49 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 50 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 51 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 52 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 53 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 54 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 55 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 56 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 57 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 58 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 59 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 60 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 61 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 62 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 63 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 64 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 65 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 66 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 67 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 68 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 69 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 70 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 71 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 72 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 73 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 74 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 75 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 76 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 77 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 78 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 79 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 80 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 81 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 82 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 83 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 84 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 85 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 86 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 87 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 88 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 89 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 90 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 91 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 92 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 93 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 94 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 95 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 96 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 97 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 98 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 99 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 100 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 101 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 102 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 103 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 104 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 105 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 106 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 107 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 108 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 109 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 110 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 111 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 112 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 113 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 114 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 115 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 116 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 117 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 118 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 119 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 120 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 121 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 122 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 123 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 124 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 125 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 126 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 127 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 128 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 129 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 130 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 131 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 132 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 133 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 134 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 135 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 136 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 137 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 138 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 139 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 140 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 141 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 142 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 143 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 144 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 145 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 146 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 147 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 148 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 149 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 150 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 151 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 152 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 153 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 154 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 155 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 156 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 157 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 158 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 159 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 160 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 161 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 162 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 163 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 164 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 165 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 166 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 167 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 168 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 169 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 170 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 171 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 172 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 173 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 174 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 175 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 176 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 177 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 178 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 179 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 180 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 181 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 182 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 183 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 184 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 185 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 186 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 187 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 188 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 189 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 190 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 191 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 192 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 193 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 194 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 195 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 196 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 197 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 198 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 199 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 200 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 201 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 202 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 203 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 204 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 205 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 206 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 207 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 208 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 209 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 210 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 211 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 212 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 213 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 214 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 215 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 216 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 217 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 218 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 219 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 220 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 221 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 222 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 223 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 224 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 225 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 226 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 227 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 228 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 229 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 230 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 231 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 232 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 233 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
