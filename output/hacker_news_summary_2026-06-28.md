# Hacker News 热门文章摘要 (2026-06-28)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

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

## 11. Why does kinetic energy increase quadratically, not linearly, with speed? (2011)

**原文标题**: Why does kinetic energy increase quadratically, not linearly, with speed? (2011)

**原文链接**: [https://physics.stackexchange.com/questions/535/why-does-kinetic-energy-increase-quadratically-not-linearly-with-speed](https://physics.stackexchange.com/questions/535/why-does-kinetic-energy-increase-quadratically-not-linearly-with-speed)

生成摘要时出错

---

## 12. Marfa Public Radio Puts You to Sleep

**原文标题**: Marfa Public Radio Puts You to Sleep

**原文链接**: [https://www.marfapublicradio.org/podcast/marfa-public-radio-puts-you-to-sleep](https://www.marfapublicradio.org/podcast/marfa-public-radio-puts-you-to-sleep)

生成摘要时出错

---

## 13. The best response to AI slop and online noise is from Robin Williams

**原文标题**: The best response to AI slop and online noise is from Robin Williams

**原文链接**: [https://jayacunzo.com/blog/your-move-chief](https://jayacunzo.com/blog/your-move-chief)

生成摘要时出错

---

## 14. PlayStation Is Deleting 551 Movies from Customers' Accounts

**原文标题**: PlayStation Is Deleting 551 Movies from Customers' Accounts

**原文链接**: [https://kotaku.com/playstation-store-movies-digital-studio-canal-terminator-2000711013](https://kotaku.com/playstation-store-movies-digital-studio-canal-terminator-2000711013)

生成摘要时出错

---

## 15. IP Crawl: Living atlas of open webcams discovered on the public internet

**原文标题**: IP Crawl: Living atlas of open webcams discovered on the public internet

**原文链接**: [https://ipcrawl.com/](https://ipcrawl.com/)

生成摘要时出错

---

## 16. Flock cameras track more than your license plate, and they're spreading fast

**原文标题**: Flock cameras track more than your license plate, and they're spreading fast

**原文链接**: [https://www.engadget.com/2203000/flock-cameras-recording-license-plate/](https://www.engadget.com/2203000/flock-cameras-recording-license-plate/)

生成摘要时出错

---

## 17. The gap between open weights LLMs and closed source LLMs

**原文标题**: The gap between open weights LLMs and closed source LLMs

**原文链接**: [https://blog.doubleword.ai/frontier-os-llm](https://blog.doubleword.ai/frontier-os-llm)

生成摘要时出错

---

## 18. Turn your site into a place people can bump into each other

**原文标题**: Turn your site into a place people can bump into each other

**原文链接**: [https://cauenapier.com/blog/townsquare_release/](https://cauenapier.com/blog/townsquare_release/)

生成摘要时出错

---

## 19. Streaming services' obnoxiously loud ads become illegal on July 1 in California

**原文标题**: Streaming services' obnoxiously loud ads become illegal on July 1 in California

**原文链接**: [https://arstechnica.com/gadgets/2026/06/streaming-services-obnoxiously-loud-ads-become-illegal-on-july-1-in-california/](https://arstechnica.com/gadgets/2026/06/streaming-services-obnoxiously-loud-ads-become-illegal-on-july-1-in-california/)

生成摘要时出错

---

## 20. 5k menus from the New York Public Library’s Buttolph Collection (1880-1920)

**原文标题**: 5k menus from the New York Public Library’s Buttolph Collection (1880-1920)

**原文链接**: [https://pudding.cool/2026/06/menu-story/](https://pudding.cool/2026/06/menu-story/)

生成摘要时出错

---

## 21. Suspicious Discontinuities (2020)

**原文标题**: Suspicious Discontinuities (2020)

**原文链接**: [https://danluu.com/discontinuities/](https://danluu.com/discontinuities/)

生成摘要时出错

---

## 22. Asian AI startups launch Mythos-like models

**原文标题**: Asian AI startups launch Mythos-like models

**原文链接**: [https://techcrunch.com/2026/06/27/asian-ai-startups-launch-mythos-like-models-as-anthropics-export-ban-drags-on/](https://techcrunch.com/2026/06/27/asian-ai-startups-launch-mythos-like-models-as-anthropics-export-ban-drags-on/)

生成摘要时出错

---

## 23. Choosing a Public DNS Resolver

**原文标题**: Choosing a Public DNS Resolver

**原文链接**: [https://evilbit.de/dns-resolver-guide.html](https://evilbit.de/dns-resolver-guide.html)

生成摘要时出错

---

## 24. Ford hired AI and sacked humans. It backfired badly

**原文标题**: Ford hired AI and sacked humans. It backfired badly

**原文链接**: [https://www.the-independent.com/tech/ford-ai-automation-human-workers-b3003787.html](https://www.the-independent.com/tech/ford-ai-automation-human-workers-b3003787.html)

生成摘要时出错

---

## 25. OpenTTD 16.0-Beta1

**原文标题**: OpenTTD 16.0-Beta1

**原文链接**: [https://www.openttd.org/news/2026/06/25/openttd-16-0-beta1](https://www.openttd.org/news/2026/06/25/openttd-16-0-beta1)

生成摘要时出错

---

## 26. AMD Strix Halo RDMA Cluster Setup Guide

**原文标题**: AMD Strix Halo RDMA Cluster Setup Guide

**原文链接**: [https://github.com/kyuz0/amd-strix-halo-vllm-toolboxes/blob/main/rdma_cluster/setup_guide.md](https://github.com/kyuz0/amd-strix-halo-vllm-toolboxes/blob/main/rdma_cluster/setup_guide.md)

生成摘要时出错

---

## 27. AI in mathematics is forcing big questions

**原文标题**: AI in mathematics is forcing big questions

**原文链接**: [https://spectrum.ieee.org/ai-in-mathematics](https://spectrum.ieee.org/ai-in-mathematics)

生成摘要时出错

---

## 28. 'Careless People' author claims Meta surveilled her for 12mos to enforce silence

**原文标题**: 'Careless People' author claims Meta surveilled her for 12mos to enforce silence

**原文链接**: [https://fortune.com/2026/06/26/meta-wynn-williams-surveillance-gag-order-lawsuit-2026/](https://fortune.com/2026/06/26/meta-wynn-williams-surveillance-gag-order-lawsuit-2026/)

生成摘要时出错

---

## 29. Michigan bill would bar employers from requiring after-hours coms with workers

**原文标题**: Michigan bill would bar employers from requiring after-hours coms with workers

**原文链接**: [https://www.cbsnews.com/detroit/news/workplace-boundaries-act-employees-after-hours/](https://www.cbsnews.com/detroit/news/workplace-boundaries-act-employees-after-hours/)

生成摘要时出错

---

## 30. Michigan spent $1.8B and only created 602 jobs

**原文标题**: Michigan spent $1.8B and only created 602 jobs

**原文链接**: [https://www.msn.com/en-us/money/general/michigan-spent-1-8-billion-and-only-created-602-jobs/ar-AA26Cusu](https://www.msn.com/en-us/money/general/michigan-spent-1-8-billion-and-only-created-602-jobs/ar-AA26Cusu)

生成摘要时出错

---

## 31. The origins of the school system aimed to produce independent, critical thinkers (2024)

**原文标题**: The origins of the school system aimed to produce independent, critical thinkers (2024)

**原文链接**: [https://www.cbc.ca/radio/ideas/humboldt-education-system-bildung-1.7172093](https://www.cbc.ca/radio/ideas/humboldt-education-system-bildung-1.7172093)

生成摘要时出错

---

## 32. Turning music into a chore is how I became a musician (2022)

**原文标题**: Turning music into a chore is how I became a musician (2022)

**原文链接**: [https://the.scapegoat.dev/turning-music-into-a-chore-is-what-made-me-an-artist/](https://the.scapegoat.dev/turning-music-into-a-chore-is-what-made-me-an-artist/)

生成摘要时出错

---

## 33. Evan's Jujutsu Tutorial

**原文标题**: Evan's Jujutsu Tutorial

**原文链接**: [https://evmar.github.io/jjtut/](https://evmar.github.io/jjtut/)

生成摘要时出错

---

## 34. Reflections on software engineering in the age of AI

**原文标题**: Reflections on software engineering in the age of AI

**原文链接**: [https://adiamond.me/2026/06/software-engineering-in-the-age-of-ai/](https://adiamond.me/2026/06/software-engineering-in-the-age-of-ai/)

生成摘要时出错

---

## 35. Enhancing x11 Application Security with LXC (2025)

**原文标题**: Enhancing x11 Application Security with LXC (2025)

**原文链接**: [https://dobrowolski.dev/article/enhancing-x11-application-security-with-lxc/](https://dobrowolski.dev/article/enhancing-x11-application-security-with-lxc/)

生成摘要时出错

---

## 36. Doctors suspected man had brain cancer. He had worms

**原文标题**: Doctors suspected man had brain cancer. He had worms

**原文链接**: [https://arstechnica.com/health/2026/06/doctors-suspected-man-had-brain-cancer-he-actually-had-worms/](https://arstechnica.com/health/2026/06/doctors-suspected-man-had-brain-cancer-he-actually-had-worms/)

生成摘要时出错

---

## 37. Daisugi, the Japanese technique of growing trees out of other trees (2020)

**原文标题**: Daisugi, the Japanese technique of growing trees out of other trees (2020)

**原文链接**: [https://www.openculture.com/2020/10/daisugi.html](https://www.openculture.com/2020/10/daisugi.html)

生成摘要时出错

---

## 38. Librepods: AirPods liberated from Apple's ecosystem

**原文标题**: Librepods: AirPods liberated from Apple's ecosystem

**原文链接**: [https://github.com/librepods-org/librepods](https://github.com/librepods-org/librepods)

生成摘要时出错

---

## 39. Tokenmaxxing is dead, long live tokenmaxxing

**原文标题**: Tokenmaxxing is dead, long live tokenmaxxing

**原文链接**: [https://12gramsofcarbon.com/p/agentics-tech-things-tokenmaxxing](https://12gramsofcarbon.com/p/agentics-tech-things-tokenmaxxing)

生成摘要时出错

---

## 40. Software Is Becoming Marketing

**原文标题**: Software Is Becoming Marketing

**原文链接**: [https://www.terezatizkova.com/writing/software-abundance](https://www.terezatizkova.com/writing/software-abundance)

生成摘要时出错

---

## 41. America's Large Homebuilders Shift the Cost of Shoddy Construction to Buyers

**原文标题**: America's Large Homebuilders Shift the Cost of Shoddy Construction to Buyers

**原文链接**: [https://hntrbrk.com/investigations/homebuilders](https://hntrbrk.com/investigations/homebuilders)

生成摘要时出错

---

## 42. The cost YAGNI was never about

**原文标题**: The cost YAGNI was never about

**原文链接**: [https://newsletter.kentbeck.com/p/the-cost-yagni-was-never-about](https://newsletter.kentbeck.com/p/the-cost-yagni-was-never-about)

生成摘要时出错

---

## 43. Running a software jam in a world of slop

**原文标题**: Running a software jam in a world of slop

**原文链接**: [https://foxmoss.com/blog/radish/](https://foxmoss.com/blog/radish/)

生成摘要时出错

---

## 44. Examining circuit boards from the Space Shuttle's I/O Processor

**原文标题**: Examining circuit boards from the Space Shuttle's I/O Processor

**原文链接**: [https://www.righto.com/2026/06/space-shuttle-io-processor-boards.html](https://www.righto.com/2026/06/space-shuttle-io-processor-boards.html)

生成摘要时出错

---

## 45. Working around dragons with the Lemote Yeeloong laptop and OpenBSD

**原文标题**: Working around dragons with the Lemote Yeeloong laptop and OpenBSD

**原文链接**: [http://oldvcr.blogspot.com/2026/06/working-around-dragons-with-lemote.html](http://oldvcr.blogspot.com/2026/06/working-around-dragons-with-lemote.html)

生成摘要时出错

---

## 46. The MUMPS 76 Primer – anniversary edition

**原文标题**: The MUMPS 76 Primer – anniversary edition

**原文链接**: [https://github.com/rochus-keller/MUMPS/blob/main/docs/MUMPS_Primer.adoc](https://github.com/rochus-keller/MUMPS/blob/main/docs/MUMPS_Primer.adoc)

生成摘要时出错

---

## 47. Ships keep moving through Hormuz despite strike

**原文标题**: Ships keep moving through Hormuz despite strike

**原文链接**: [https://www.lloydslist.com/LL1157680/Ships-keep-moving-through-Hormuz-despite-strike-and-suspension-of-IMO-exit-strategy](https://www.lloydslist.com/LL1157680/Ships-keep-moving-through-Hormuz-despite-strike-and-suspension-of-IMO-exit-strategy)

生成摘要时出错

---

## 48. Codeberg Is Down

**原文标题**: Codeberg Is Down

**原文链接**: [https://social.anoxinon.de/@codebergstatus/116824443563698727](https://social.anoxinon.de/@codebergstatus/116824443563698727)

生成摘要时出错

---

## 49. Is America becoming a gerontocracy?

**原文标题**: Is America becoming a gerontocracy?

**原文链接**: [https://www.economist.com/culture/2026/06/25/is-america-becoming-a-gerontocracy](https://www.economist.com/culture/2026/06/25/is-america-becoming-a-gerontocracy)

生成摘要时出错

---

## 50. IBM MCGA Gate Array Reverse Engineering

**原文标题**: IBM MCGA Gate Array Reverse Engineering

**原文链接**: [https://github.com/schlae/IBM_MCGA](https://github.com/schlae/IBM_MCGA)

生成摘要时出错

---

## 51. Ford rehires 'gray beard' engineers after AI falls short

**原文标题**: Ford rehires 'gray beard' engineers after AI falls short

**原文链接**: [https://techcrunch.com/2026/06/28/ford-rehires-gray-beard-engineers-after-ai-falls-short/](https://techcrunch.com/2026/06/28/ford-rehires-gray-beard-engineers-after-ai-falls-short/)

生成摘要时出错

---

## 52. Tuta: They are bringing back ChatControl

**原文标题**: Tuta: They are bringing back ChatControl

**原文链接**: [https://mastodon.social/@Tutanota/116815262001889776](https://mastodon.social/@Tutanota/116815262001889776)

生成摘要时出错

---

## 53. Researchers have developed pixels that can emit and analyse light together

**原文标题**: Researchers have developed pixels that can emit and analyse light together

**原文链接**: [https://ethz.ch/en/news-and-events/eth-news/news/2026/06/a-new-type-of-pixel.html](https://ethz.ch/en/news-and-events/eth-news/news/2026/06/a-new-type-of-pixel.html)

生成摘要时出错

---

## 54. Can China build its own ASML?

**原文标题**: Can China build its own ASML?

**原文链接**: [https://nikkei.shorthandstories.com/can-china-build-its-own-asml/](https://nikkei.shorthandstories.com/can-china-build-its-own-asml/)

生成摘要时出错

---

## 55. The Nationwide Backlash Against Cameras Watching Your Car

**原文标题**: The Nationwide Backlash Against Cameras Watching Your Car

**原文链接**: [https://www.wsj.com/us-news/the-nationwide-backlash-against-cameras-watching-your-car-401a656a](https://www.wsj.com/us-news/the-nationwide-backlash-against-cameras-watching-your-car-401a656a)

生成摘要时出错

---

## 56. Climate.us launches independent website for trusted climate information

**原文标题**: Climate.us launches independent website for trusted climate information

**原文链接**: [https://www.climate.us/news-features/feed/climateus-launches-independent-website-trusted-climate-information](https://www.climate.us/news-features/feed/climateus-launches-independent-website-trusted-climate-information)

生成摘要时出错

---

## 57. A peek into Reddit's anti-spam internals

**原文标题**: A peek into Reddit's anti-spam internals

**原文链接**: [https://lyra.horse/blog/2026/06/reddit-spam-internals/](https://lyra.horse/blog/2026/06/reddit-spam-internals/)

生成摘要时出错

---

## 58. Apple Neural Engine: Architecture, Programming, and Performance

**原文标题**: Apple Neural Engine: Architecture, Programming, and Performance

**原文链接**: [https://arxiv.org/abs/2606.22283](https://arxiv.org/abs/2606.22283)

生成摘要时出错

---

## 59. More evidence is consistent with possible ancient life on Mars (2025)

**原文标题**: More evidence is consistent with possible ancient life on Mars (2025)

**原文链接**: [https://www.cbc.ca/radio/quirks/more-evidence-of-life-on-mars-but-still-no-life-1.7649645](https://www.cbc.ca/radio/quirks/more-evidence-of-life-on-mars-but-still-no-life-1.7649645)

生成摘要时出错

---

## 60. Professor denounces mass AI fraud on an exam at Brown University

**原文标题**: Professor denounces mass AI fraud on an exam at Brown University

**原文链接**: [https://english.elpais.com/education/2026-06-28/ai-fraud-at-brown-university-academic-integrity-is-at-risk.html](https://english.elpais.com/education/2026-06-28/ai-fraud-at-brown-university-academic-integrity-is-at-risk.html)

生成摘要时出错

---

## 61. Anthropic says Alibaba used 25k accounts to mine Claude

**原文标题**: Anthropic says Alibaba used 25k accounts to mine Claude

**原文链接**: [https://arstechnica.com/tech-policy/2026/06/anthropic-claims-alibaba-defied-trump-to-attack-claude-and-steal-capabilities/](https://arstechnica.com/tech-policy/2026/06/anthropic-claims-alibaba-defied-trump-to-attack-claude-and-steal-capabilities/)

生成摘要时出错

---

## 62. AgentKits – 60 production-ready AI agent blueprints with guardrails

**原文标题**: AgentKits – 60 production-ready AI agent blueprints with guardrails

**原文链接**: [https://www.agent-kits.com](https://www.agent-kits.com)

生成摘要时出错

---

## 63. Semgrep: GLM 5.2 beats Claude in our Cyber Benchmarks

**原文标题**: Semgrep: GLM 5.2 beats Claude in our Cyber Benchmarks

**原文链接**: [https://semgrep.dev/blog/2026/we-have-mythos-at-home-glm-52-beats-claude-in-our-cyber-benchmarks/](https://semgrep.dev/blog/2026/we-have-mythos-at-home-glm-52-beats-claude-in-our-cyber-benchmarks/)

生成摘要时出错

---

## 64. Factorio 2.1 Experimental Release

**原文标题**: Factorio 2.1 Experimental Release

**原文链接**: [https://factorio.com/blog/post/fff-444](https://factorio.com/blog/post/fff-444)

生成摘要时出错

---

## 65. It's dead, Jim – the old Microsoft UEFI CA from 2011 expired yesterday

**原文标题**: It's dead, Jim – the old Microsoft UEFI CA from 2011 expired yesterday

**原文链接**: [https://blog.einval.com/2026/06/27](https://blog.einval.com/2026/06/27)

生成摘要时出错

---

## 66. Mojo programming language will become open-source soon

**原文标题**: Mojo programming language will become open-source soon

**原文链接**: [https://console.modular.com/signup](https://console.modular.com/signup)

生成摘要时出错

---

## 67. You've tried DuckDuckGo and Brave Search, now get serious with SearXNG

**原文标题**: You've tried DuckDuckGo and Brave Search, now get serious with SearXNG

**原文链接**: [https://www.neowin.net/editorials/youve-tried-duckduckgo-and-brave-search-now-get-serious-with-searxng/](https://www.neowin.net/editorials/youve-tried-duckduckgo-and-brave-search-now-get-serious-with-searxng/)

生成摘要时出错

---

## 68. Show HN: DRM-Free Books

**原文标题**: Show HN: DRM-Free Books

**原文链接**: [https://frequal.com/Perspectives/DrmFreeAuthors.html](https://frequal.com/Perspectives/DrmFreeAuthors.html)

生成摘要时出错

---

## 69. Armadillo – A DNS Server in Gleam for Homelab Use

**原文标题**: Armadillo – A DNS Server in Gleam for Homelab Use

**原文链接**: [https://github.com/vshakitskiy/armadillo](https://github.com/vshakitskiy/armadillo)

生成摘要时出错

---

## 70. The AI Industry as You Know It Died Today

**原文标题**: The AI Industry as You Know It Died Today

**原文链接**: [https://www.thealgorithmicbridge.com/p/the-ai-industry-as-you-know-it-died](https://www.thealgorithmicbridge.com/p/the-ai-industry-as-you-know-it-died)

生成摘要时出错

---

## 71. Russian citizens told "switch to Android" after Apple blocks key Russian apps

**原文标题**: Russian citizens told "switch to Android" after Apple blocks key Russian apps

**原文链接**: [https://arstechnica.com/gadgets/2026/06/russian-citizens-told-switch-to-android-after-apple-blocks-key-russian-apps/](https://arstechnica.com/gadgets/2026/06/russian-citizens-told-switch-to-android-after-apple-blocks-key-russian-apps/)

生成摘要时出错

---

## 72. Check out the new US passport

**原文标题**: Check out the new US passport

**原文链接**: [https://mishtalk.com/economics/does-president-trump-have-any-idea-what-passports-are-for/](https://mishtalk.com/economics/does-president-trump-have-any-idea-what-passports-are-for/)

生成摘要时出错

---

## 73. Greece Is Richer. So Why Do So Many Greeks Still Feel Poor?

**原文标题**: Greece Is Richer. So Why Do So Many Greeks Still Feel Poor?

**原文链接**: [https://www.dnews.gr/eidhseis/news-in-english/596650/greece-is-richer-so-why-do-so-many-greeks-still-feel-poor](https://www.dnews.gr/eidhseis/news-in-english/596650/greece-is-richer-so-why-do-so-many-greeks-still-feel-poor)

生成摘要时出错

---

## 74. Programmable Probabilistic Computer with 1M p-bits

**原文标题**: Programmable Probabilistic Computer with 1M p-bits

**原文链接**: [https://arxiv.org/abs/2606.25313](https://arxiv.org/abs/2606.25313)

生成摘要时出错

---

## 75. Dr. Alan Kay on the meaning of "object-oriented programming" (2003)

**原文标题**: Dr. Alan Kay on the meaning of "object-oriented programming" (2003)

**原文链接**: [https://notes.shixiangxi.com/en/docs/appendix/alan-kay-on-oop/](https://notes.shixiangxi.com/en/docs/appendix/alan-kay-on-oop/)

生成摘要时出错

---

## 76. Historical memory prices 1960-2026

**原文标题**: Historical memory prices 1960-2026

**原文链接**: [https://dam.stanford.edu/memory-prices.html](https://dam.stanford.edu/memory-prices.html)

生成摘要时出错

---

## 77. What If a Man Practised Shooting a Million Times? Shot 90172, Football Progress [video]

**原文标题**: What If a Man Practised Shooting a Million Times? Shot 90172, Football Progress [video]

**原文链接**: [https://www.youtube.com/watch?v=CI9oUUnUzw0](https://www.youtube.com/watch?v=CI9oUUnUzw0)

生成摘要时出错

---

## 78. Show HN: Starglyphs - A constellation puzzle game based on Euler paths

**原文标题**: Show HN: Starglyphs - A constellation puzzle game based on Euler paths

**原文链接**: [https://starglyphs.com](https://starglyphs.com)

生成摘要时出错

---

## 79. Perry – compiles TypeScript to native GUI and CLI apps. No runtime / Electron

**原文标题**: Perry – compiles TypeScript to native GUI and CLI apps. No runtime / Electron

**原文链接**: [https://perryts.com](https://perryts.com)

生成摘要时出错

---

## 80. Set Up Your Own DoH Service

**原文标题**: Set Up Your Own DoH Service

**原文链接**: [https://nochan.net/b/Internet-Crap/20260602-Set-Up-Your-Own-DoH-Service/](https://nochan.net/b/Internet-Crap/20260602-Set-Up-Your-Own-DoH-Service/)

生成摘要时出错

---

## 81. Germany: Hottest temperature on record 41.3C (106.3°F)

**原文标题**: Germany: Hottest temperature on record 41.3C (106.3°F)

**原文链接**: [https://phys.org/news/2026-06-germany-hottest-temperature-413c-weather.html](https://phys.org/news/2026-06-germany-hottest-temperature-413c-weather.html)

生成摘要时出错

---

## 82. Yap – free offline voice dictation for Mac/Windows/Linux (Wispr Flow alt)

**原文标题**: Yap – free offline voice dictation for Mac/Windows/Linux (Wispr Flow alt)

**原文链接**: [https://github.com/AkuchiS/yap](https://github.com/AkuchiS/yap)

生成摘要时出错

---

## 83. I Build a 10 Inch Mini Rack from Aluminium Extrusions

**原文标题**: I Build a 10 Inch Mini Rack from Aluminium Extrusions

**原文链接**: [https://louwrentius.com/i-build-a-10-inch-mini-rack-from-aluminium-extrusions.html](https://louwrentius.com/i-build-a-10-inch-mini-rack-from-aluminium-extrusions.html)

生成摘要时出错

---

## 84. The Card That Made the Apple II Serious

**原文标题**: The Card That Made the Apple II Serious

**原文链接**: [https://www.wiseowl.com/articles/a2fpga-videx-01-the-card-that-made-the-apple-ii-serious/](https://www.wiseowl.com/articles/a2fpga-videx-01-the-card-that-made-the-apple-ii-serious/)

生成摘要时出错

---

## 85. 32bit Apple app running on M4 natively

**原文标题**: 32bit Apple app running on M4 natively

**原文链接**: [https://old.reddit.com/r/MacOS/comments/1ufug75/major_breakthrough_32bit_apple_app_running_on_m4/](https://old.reddit.com/r/MacOS/comments/1ufug75/major_breakthrough_32bit_apple_app_running_on_m4/)

生成摘要时出错

---

## 86. Peppa Pig studio wants to clone child actors' voices with AI indefinitely

**原文标题**: Peppa Pig studio wants to clone child actors' voices with AI indefinitely

**原文链接**: [https://www.gadgetreview.com/peppa-pigs-ai-voice-clause-draws-nearly-1000-industry-objections](https://www.gadgetreview.com/peppa-pigs-ai-voice-clause-draws-nearly-1000-industry-objections)

生成摘要时出错

---

## 87. The US Used to Demand the Best Tech. Now We Ban It

**原文标题**: The US Used to Demand the Best Tech. Now We Ban It

**原文链接**: [https://www.pcmag.com/opinions/the-us-used-to-demand-the-best-tech-now-we-ban-it](https://www.pcmag.com/opinions/the-us-used-to-demand-the-best-tech-now-we-ban-it)

生成摘要时出错

---

