# Hacker News 热门文章摘要 (2026-07-11)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 请不要停用 Gemini 2.5 Flash

**原文标题**: Please don't discontinue Gemini 2.5 Flash

**原文链接**: [https://discuss.ai.google.dev/t/please-dont-discontinue-gemini-2-5-flash/174246](https://discuss.ai.google.dev/t/please-dont-discontinue-gemini-2-5-flash/174246)

作者感谢Gemini团队提供的模型，尤其强调了Gemini 2.5 Flash在其工作流程中扮演的关键角色。他们报告称，内部基准测试显示，即使在尝试根据新指南调整提示后，Gemini 3 Flash在他们的特定用例中表现也不佳。作者认为其他人可能也有类似的经历，并在切换时面临困难，因此强烈恳请不要停用Gemini 2.5 Flash。

---

## 2. 我们将PgBouncer的吞吐量提升了4倍

**原文标题**: We scaled PgBouncer to 4x throughput

**原文链接**: [https://clickhouse.com/blog/pgbouncer-clickhouse-managed-postgres](https://clickhouse.com/blog/pgbouncer-clickhouse-managed-postgres)

PgBouncer是单线程的，在多核机器上仅利用一个CPU核心，从而限制了吞吐量。ClickHouse Managed Postgres通过运行一个与可用核心数匹配的PgBouncer“进程集群”来克服这一限制。这些进程使用`so_reuseport`共享一个端口，使内核能够将传入的客户端连接在它们之间进行负载均衡，从而使这种多进程设置对客户端是透明的。

一个关键挑战是查询取消，因为取消请求可能发送到一个与管理查询会话的PgBouncer进程不同的实例。这通过“对等通信”来解决，即进程之间相互通信并将来取消请求转发到正确的实例。`max_client_conn`和`max_db_connections`等连接预算也分配到整个集群中，以防止Postgres过载。

在AWS EC2（16个vCPU实例）上的实际测试表明，单个PgBouncer进程峰值达到8.7万事务/秒，仅使用一个核心，而机器的其余部分处于空闲状态。相比之下，由16个PgBouncer进程组成的集群通过有效利用多达8个核心，实现了大约33.6万事务/秒，吞吐量提高了4倍。这显示了CPU利用率的显著提升（例如，在256个客户端下，单个进程为9%，而集群为52%）。

总而言之，通过运行一个利用`so_reuseport`和进程间对等通信的扩展集群，PgBouncer从一个吞吐量瓶颈转变为高效的管道，最大限度地提高了资源利用率。这种设置现在已成为ClickHouse Managed Postgres的标准配置。

---

## 3. Modern decor may be straining people's brains

**原文标题**: Modern decor may be straining people's brains

**原文链接**: [https://studyfinds.com/modern-decor-may-be-straining-peoples-brains/](https://studyfinds.com/modern-decor-may-be-straining-peoples-brains/)

生成摘要时出错

---

## 4. 美国女划船手完成加州至夏威夷历史性单人划行

**原文标题**: Female US rower completes historic solo journey from California to Hawaii

**原文链接**: [https://www.theguardian.com/us-news/2026/jul/04/california-hawaii-rowing-solo-journey](https://www.theguardian.com/us-news/2026/jul/04/california-hawaii-rowing-solo-journey)

美国赛艇运动员兼大峡谷漂流向导凯尔西·芬德勒(Kelsey Pfendler)成功完成了一次历史性的单人旅程，她从加利福尼亚州蒙特雷划船2400多英里，抵达夏威夷檀香山。经过近一个半月的海上航行，她于周五晚上抵达檀香山港口。

芬德勒的目标是成为首位完成太平洋中部单人横渡的美国女性、最年轻的女性和速度最快的女性。根据国际海洋划船协会的记录，她实现了这些目标，用时不到44天。这一非凡的成绩不仅打破了此前86天的女性可比速度纪录，甚至超越了52天的男性纪录。

数千人在线关注了芬德勒的旅程，她在网上分享了视频日记，详细记录了遇到的挑战和经历。她坦率地讲述了手上的水泡、在强风中难以入睡的挣扎，以及对抗不利洋流所造成的精神和身体上的消耗。她的视频还涵盖了烹饪、防晒和制造淡水等后勤细节，通常将情感上的反思与幽默融为一体。

作为一名拥有八年经验的专业漂流向导，芬德勒形容自己热爱“在荒无人烟的地方划船”。接近目的地时，她分享了一条强有力的信息，希望自己的成就能够激励他人“找到属于自己的宏大、艰难、可怕的事情”，并强调一个人“绝对足够强大去开始它”。

---

## 5. 你的代码很快——全看运气。

**原文标题**: Your code is fast – if you're lucky

**原文链接**: [https://tiki.li/blog/lucky_code.html](https://tiki.li/blog/lucky_code.html)

This article details an attempt to optimize a Quicksort implementation for speed, focusing on leveraging modern compilers' ability (like Clang) to generate fast, branch-free instructions. The author's custom C Quicksort uses several techniques: sorting networks for small partitions (up to 12 elements), median-of-5 pivot selection, and a specialized partitioning algorithm that temporarily stores elements in a `swbuf` array. Loop unrolling is also employed.

However, the initial optimized code performs surprisingly poorly on macOS/M1 (Clang, -O3), sorting 50 million doubles in 4.39 seconds, significantly slower than C++ `std::sort` which completes the same task in 1.33 seconds.

The core insight, highlighting the "luck" factor, is that minor "cosmetic" changes in code style can dramatically impact compiler optimization. The article points to rewriting explicit pointer increments, such as `*lwr = x; lwr++;` to the more idiomatic `*lwr++ = x;`, as the key modification. This suggests that compilers are highly sensitive to how code is written, and a subtle stylistic change can unlock superior, branch-free instruction generation, leading to substantial performance improvements. The article ends before presenting the benchmark results of the rewritten code.

---

## 6. 含铅汽油：问世即知其毒 (2016)

**原文标题**: Leaded Gas Was a Known Poison the Day It Was Invented (2016)

**原文链接**: [https://www.smithsonianmag.com/smart-news/leaded-gas-poison-invented-180961368/](https://www.smithsonianmag.com/smart-news/leaded-gas-poison-invented-180961368/)

文章《含铅汽油从发明之日起就已知是毒药》详细介绍了含铅汽油充满争议的历史。1921年，通用汽车工程师小托马斯·米基利（Thomas Midgley Jr.）发现四乙基铅（TEL）可以减少发动机“爆震”。尽管乙醇是一种更安全、有效的替代品，但通用汽车和石油公司却拒绝了它，因为它无法申请专利，并且威胁到他们对市场的控制。

TEL被认为剧毒；杜邦公司一位高管在1922年将其描述为“剧毒”，米基利本人也曾患有严重的铅中毒。含铅汽油于1923年首次销售，1924年五名工人因接触TEL死亡后，引发了强烈反弹。然而，1926年的一份公共卫生报告却将公众风险轻描淡写为“微乎其微”，得出“没有理由禁止销售”的结论，并将潜在的未来问题推迟为“下一代人的问题”。

这一先例使得逐步淘汰含铅汽油变得困难，美国环境保护署（EPA）直到20世纪70年代中期才开始这一进程。其长期影响是深远的：铅暴露，特别是儿童的铅暴露，与智商下降、多动症、行为问题、学习障碍有关，大量研究还将其与暴力犯罪联系起来。大部分铅仍残留在受污染的环境中，构成持续的健康挑战。

---

## 7. 苹果起诉OpenAI，指控其窃取公司机密

**原文标题**: Apple sues OpenAI, accusing it of stealing company secrets

**原文链接**: [https://www.nytimes.com/2026/07/10/technology/apple-openai-lawsuit.html](https://www.nytimes.com/2026/07/10/technology/apple-openai-lawsuit.html)

无法访问文章链接。

---

## 8. AI 2040 and the cult of intelligence

**原文标题**: AI 2040 and the cult of intelligence

**原文链接**: [https://geohot.github.io//blog/jekyll/update/2026/07/11/ai-2040.html](https://geohot.github.io//blog/jekyll/update/2026/07/11/ai-2040.html)

生成摘要时出错

---

## 9. FCC批准太空镜照亮夜空试验

**原文标题**: FCC approves test of space mirror to light night sky

**原文链接**: [https://theconversation.com/the-u-s-just-approved-a-giant-space-mirror-to-test-sunlight-on-demand-low-earth-orbit-is-getting-weird-283482](https://theconversation.com/the-u-s-just-approved-a-giant-space-mirror-to-test-sunlight-on-demand-low-earth-orbit-is-getting-weird-283482)

生成摘要时出错

---

## 10. Exit Chat Control

**原文标题**: Exit Chat Control

**原文链接**: [https://exitchatcontrol.org/](https://exitchatcontrol.org/)

This article introduces an encrypted messenger, presented as a simple, direct replacement for WhatsApp, offering secure texts, calls, video, and group chats. Its core value proposition is robust privacy and security: end-to-end encryption by default, a non-profit structure, an audited world-standard protocol, and minimal metadata retention. Notably, the team has pledged to exit the EU rather than comply with scanning mandates.

Recommended for everyone, starting immediately, it's seen as a vital first step for digital privacy. While a phone number is required for setup, users can create a username to hide it. To install, visit signal.org (App Store, Google Play, or direct APK). After confirming your number via SMS and setting a PIN, users should navigate to Settings > Privacy to create a username and enable registration lock, then invite contacts and link the desktop app as needed.

---

## 11. Focus

**原文标题**: Focus

**原文链接**: [https://boz.com/articles/focus](https://boz.com/articles/focus)

生成摘要时出错

---

## 12. Why it's so difficult to produce American-made medical gloves

**原文标题**: Why it's so difficult to produce American-made medical gloves

**原文链接**: [https://www.bloomberg.com/news/features/2026-07-07/why-it-s-so-difficult-to-produce-100-american-made-medical-gloves](https://www.bloomberg.com/news/features/2026-07-07/why-it-s-so-difficult-to-produce-100-american-made-medical-gloves)

生成摘要时出错

---

## 13. Prefer Strict Tables in SQLite

**原文标题**: Prefer Strict Tables in SQLite

**原文链接**: [https://evanhahn.com/prefer-strict-tables-in-sqlite/](https://evanhahn.com/prefer-strict-tables-in-sqlite/)

生成摘要时出错

---

## 14. GhostLock, a stack-UAF that has existed in ALL Linux distributions for 15 years

**原文标题**: GhostLock, a stack-UAF that has existed in ALL Linux distributions for 15 years

**原文链接**: [https://nebusec.ai/research/ionstack-part-2/](https://nebusec.ai/research/ionstack-part-2/)

生成摘要时出错

---

## 15. Europe's Largest Unions Demand Right to Cancel Work on Days Above 30C

**原文标题**: Europe's Largest Unions Demand Right to Cancel Work on Days Above 30C

**原文链接**: [https://novaramedia.com/2026/07/09/europes-largest-unions-demand-right-to-cancel-work-on-days-above-30c/](https://novaramedia.com/2026/07/09/europes-largest-unions-demand-right-to-cancel-work-on-days-above-30c/)

生成摘要时出错

---

## 16. 45% of Enthusiasts 'Seriously Considering' Leaving Sony for PC

**原文标题**: 45% of Enthusiasts 'Seriously Considering' Leaving Sony for PC

**原文链接**: [https://www.pushsquare.com/news/2026/07/ps5-has-put-a-dampener-on-gaming-45percent-of-enthusiasts-seriously-considering-leaving-sony-for-pc](https://www.pushsquare.com/news/2026/07/ps5-has-put-a-dampener-on-gaming-45percent-of-enthusiasts-seriously-considering-leaving-sony-for-pc)

生成摘要时出错

---

## 17. Speculations Concerning the First Ultraintelligent Machine (1965) [pdf]

**原文标题**: Speculations Concerning the First Ultraintelligent Machine (1965) [pdf]

**原文链接**: [https://languagelog.ldc.upenn.edu/myl/Good1964.pdf](https://languagelog.ldc.upenn.edu/myl/Good1964.pdf)

生成摘要时出错

---

## 18. Ben Bernanke Joins Anthropic Oversight Trust

**原文标题**: Ben Bernanke Joins Anthropic Oversight Trust

**原文链接**: [https://www.anthropic.com/news/ben-bernanke](https://www.anthropic.com/news/ben-bernanke)

生成摘要时出错

---

## 19. Apple Sues OpenAI, Alleging It Stole Trade Secrets

**原文标题**: Apple Sues OpenAI, Alleging It Stole Trade Secrets

**原文链接**: [https://www.wsj.com/tech/apple-openai-lawsuit-f86bd58c](https://www.wsj.com/tech/apple-openai-lawsuit-f86bd58c)

生成摘要时出错

---

## 20. Ryanair passenger sucked toward broken window after midair engine failure

**原文标题**: Ryanair passenger sucked toward broken window after midair engine failure

**原文链接**: [https://simpleflying.com/ryanair-thessaloniki-diversion-window-damage/](https://simpleflying.com/ryanair-thessaloniki-diversion-window-damage/)

生成摘要时出错

---

## 21. Unified Memory, Explained: Why Mini PCs Can Run 70B Models a Big GPU Can't

**原文标题**: Unified Memory, Explained: Why Mini PCs Can Run 70B Models a Big GPU Can't

**原文链接**: [https://vettedconsumer.com/unified-memory-explained-why-mini-pcs-can-run-70b-models-a-big-gpu-cant-and-where-they-slow-down/](https://vettedconsumer.com/unified-memory-explained-why-mini-pcs-can-run-70b-models-a-big-gpu-cant-and-where-they-slow-down/)

生成摘要时出错

---

## 22. Count Binface, Nigel Farage's space-warrior foe

**原文标题**: Count Binface, Nigel Farage's space-warrior foe

**原文链接**: [https://www.economist.com/the-world-in-brief/2026/07/11/b240d63f-2768-43dd-89b6-2bdceb6df745](https://www.economist.com/the-world-in-brief/2026/07/11/b240d63f-2768-43dd-89b6-2bdceb6df745)

生成摘要时出错

---

## 23. The Annotated JEPA

**原文标题**: The Annotated JEPA

**原文链接**: [https://elonlit.com/scrivings/the-annotated-jepa/](https://elonlit.com/scrivings/the-annotated-jepa/)

生成摘要时出错

---

## 24. Lisp as the Maxwell's Equations of Software (2012)

**原文标题**: Lisp as the Maxwell's Equations of Software (2012)

**原文链接**: [https://michaelnielsen.org/ddi/lisp-as-the-maxwells-equations-of-software/](https://michaelnielsen.org/ddi/lisp-as-the-maxwells-equations-of-software/)

生成摘要时出错

---

## 25. Build your own vulnerability harness

**原文标题**: Build your own vulnerability harness

**原文链接**: [https://blog.cloudflare.com/build-your-own-vulnerability-harness/](https://blog.cloudflare.com/build-your-own-vulnerability-harness/)

生成摘要时出错

---

## 26. Software Engineer's Firing Ruled Illegal in a Rare Win for a Tech Worker

**原文标题**: Software Engineer's Firing Ruled Illegal in a Rare Win for a Tech Worker

**原文链接**: [https://www.nytimes.com/2026/07/10/business/atlassian-tech-worker-wrongful-termination.html](https://www.nytimes.com/2026/07/10/business/atlassian-tech-worker-wrongful-termination.html)

生成摘要时出错

---

## 27. The early History of the Singular Value Decomposition (1993) [pdf]

**原文标题**: The early History of the Singular Value Decomposition (1993) [pdf]

**原文链接**: [https://www.math.ucdavis.edu/~saito/courses/229A/stewart-svd.pdf](https://www.math.ucdavis.edu/~saito/courses/229A/stewart-svd.pdf)

生成摘要时出错

---

## 28. USAA closed 51% of home insurance claims without making a payment in 2025

**原文标题**: USAA closed 51% of home insurance claims without making a payment in 2025

**原文链接**: [https://www.expressnews.com/business/article/san-antonio-usaa-insurance-claims-rejected-22293061.php](https://www.expressnews.com/business/article/san-antonio-usaa-insurance-claims-rejected-22293061.php)

生成摘要时出错

---

## 29. Pirate Site Blocking Is Legally Impossible in Bulgaria, Supreme Court Ruled

**原文标题**: Pirate Site Blocking Is Legally Impossible in Bulgaria, Supreme Court Ruled

**原文链接**: [https://torrentfreak.com/pirate-site-blocking-is-legally-impossible-in-bulgaria-supreme-court-ruled/](https://torrentfreak.com/pirate-site-blocking-is-legally-impossible-in-bulgaria-supreme-court-ruled/)

生成摘要时出错

---

## 30. Show HN: Learn by rebuilding Redis, Git, a database from scratch

**原文标题**: Show HN: Learn by rebuilding Redis, Git, a database from scratch

**原文链接**: [https://shipthatcode.com](https://shipthatcode.com)

生成摘要时出错

---

## 31. Clojure FFI layer for libgdx-core

**原文标题**: Clojure FFI layer for libgdx-core

**原文链接**: [https://github.com/damn/com.badlogic.gdx/tree/main](https://github.com/damn/com.badlogic.gdx/tree/main)

生成摘要时出错

---

## 32. ActivityPub over ATProto (2023)

**原文标题**: ActivityPub over ATProto (2023)

**原文链接**: [https://berjon.com/ap-at/](https://berjon.com/ap-at/)

生成摘要时出错

---

## 33. China's public QR codes are being hijacked to redirect users to porn and scams

**原文标题**: China's public QR codes are being hijacked to redirect users to porn and scams

**原文链接**: [https://www.sixthtone.com/news/1018752/ScanScam:CriminalsRedirectChina’sPublicQRCodestoPorn](https://www.sixthtone.com/news/1018752/ScanScam:CriminalsRedirectChina’sPublicQRCodestoPorn)

生成摘要时出错

---

## 34. Cpp2Rust: Translates C++ to safe Rust automatically

**原文标题**: Cpp2Rust: Translates C++ to safe Rust automatically

**原文链接**: [https://github.com/Cpp2Rust/cpp2rust](https://github.com/Cpp2Rust/cpp2rust)

生成摘要时出错

---

## 35. Meta pulls new AI image feature after days of backlash

**原文标题**: Meta pulls new AI image feature after days of backlash

**原文链接**: [https://www.bbc.com/news/articles/c2dy6e8klw0o](https://www.bbc.com/news/articles/c2dy6e8klw0o)

生成摘要时出错

---

## 36. Show HN: Reviving my 2001 college band with AI

**原文标题**: Show HN: Reviving my 2001 college band with AI

**原文链接**: [https://www.fadingmaize.com](https://www.fadingmaize.com)

生成摘要时出错

---

## 37. Reverse centaurs are the answer to the AI paradox

**原文标题**: Reverse centaurs are the answer to the AI paradox

**原文链接**: [https://pluralistic.net/2025/09/11/vulgar-thatcherism/#there-is-an-alternative](https://pluralistic.net/2025/09/11/vulgar-thatcherism/#there-is-an-alternative)

生成摘要时出错

---

## 38. Show HN: Richest people in the world by wealth creation instead of ownership

**原文标题**: Show HN: Richest people in the world by wealth creation instead of ownership

**原文链接**: [https://anti-forbes-list.vercel.app](https://anti-forbes-list.vercel.app)

生成摘要时出错

---

## 39. Java 27: What's New?

**原文标题**: Java 27: What's New?

**原文链接**: [https://www.loicmathieu.fr/wordpress/informatique/java-27-whats-new/](https://www.loicmathieu.fr/wordpress/informatique/java-27-whats-new/)

生成摘要时出错

---

## 40. How to Hide from Killer Drones

**原文标题**: How to Hide from Killer Drones

**原文链接**: [https://www.economist.com/science-and-technology/2026/07/08/how-to-hide-from-killer-drones](https://www.economist.com/science-and-technology/2026/07/08/how-to-hide-from-killer-drones)

生成摘要时出错

---

## 41. Microsoft admits Windows 11 has a GDID tracker with no off switch

**原文标题**: Microsoft admits Windows 11 has a GDID tracker with no off switch

**原文链接**: [https://www.windowslatest.com/2026/07/10/you-cant-fully-disable-microsofts-gdid-windows-11-tracker-but-these-settings-limit-what-it-captures/](https://www.windowslatest.com/2026/07/10/you-cant-fully-disable-microsofts-gdid-windows-11-tracker-but-these-settings-limit-what-it-captures/)

生成摘要时出错

---

## 42. Hands-On with the AMD Ryzen AI Halo

**原文标题**: Hands-On with the AMD Ryzen AI Halo

**原文链接**: [https://www.microcenter.com/site/mc-news/article/amd-ryzen-ai-halo-review.aspx](https://www.microcenter.com/site/mc-news/article/amd-ryzen-ai-halo-review.aspx)

生成摘要时出错

---

## 43. Auburn California Flock Surveillance Cameras Stolen and Dumped in a Canal

**原文标题**: Auburn California Flock Surveillance Cameras Stolen and Dumped in a Canal

**原文链接**: [https://www.gadgetreview.com/auburn-california-flock-surveillance-cameras-stolen-and-dumped-in-a-canal](https://www.gadgetreview.com/auburn-california-flock-surveillance-cameras-stolen-and-dumped-in-a-canal)

生成摘要时出错

---

## 44. Nvidia, CoreWeave, and Nebius: Inside the Circular Financing of the GPU Boom

**原文标题**: Nvidia, CoreWeave, and Nebius: Inside the Circular Financing of the GPU Boom

**原文链接**: [https://io-fund.com/ai-stocks/nvidia-coreweave-nebius-circular-financing-gpu-boom](https://io-fund.com/ai-stocks/nvidia-coreweave-nebius-circular-financing-gpu-boom)

生成摘要时出错

---

## 45. FreeCAD in the Browser

**原文标题**: FreeCAD in the Browser

**原文链接**: [https://magik.net/freecad/](https://magik.net/freecad/)

生成摘要时出错

---

## 46. Anyone else get a vague GitHub shakedown notice?

**原文标题**: Anyone else get a vague GitHub shakedown notice?

**原文链接**: [https://lists.osgeo.org/pipermail/qgis-developer/2026-July/068430.html](https://lists.osgeo.org/pipermail/qgis-developer/2026-July/068430.html)

生成摘要时出错

---

## 47. Tropical forests facing increasing risks of exposure to critical temp thresholds

**原文标题**: Tropical forests facing increasing risks of exposure to critical temp thresholds

**原文链接**: [https://www.pnas.org/doi/10.1073/pnas.2528622123](https://www.pnas.org/doi/10.1073/pnas.2528622123)

生成摘要时出错

---

## 48. Microsoft latest report shows 25% emissions raised due to AI data centers

**原文标题**: Microsoft latest report shows 25% emissions raised due to AI data centers

**原文链接**: [https://www.windowscentral.com/microsoft/dropping-greenwashing-credits-and-expanding-ai-datacenters-caused-microsofts-25-percent-emissions-jump](https://www.windowscentral.com/microsoft/dropping-greenwashing-credits-and-expanding-ai-datacenters-caused-microsofts-25-percent-emissions-jump)

生成摘要时出错

---

## 49. Show HN: Runloom – Go-style coroutines for Python free-threaded

**原文标题**: Show HN: Runloom – Go-style coroutines for Python free-threaded

**原文链接**: [https://github.com/robertsdotpm/runloom](https://github.com/robertsdotpm/runloom)

生成摘要时出错

---

## 50. Texas ICE Killing Darkens: Rep Says Witnesses Were Pressured to Self-Deport

**原文标题**: Texas ICE Killing Darkens: Rep Says Witnesses Were Pressured to Self-Deport

**原文链接**: [https://newrepublic.com/article/212900/texas-ice-killing-darkens-rep-says-witnesses-pressured-self-deport](https://newrepublic.com/article/212900/texas-ice-killing-darkens-rep-says-witnesses-pressured-self-deport)

生成摘要时出错

---

## 51. Companies are scrambling to curtail soaring AI costs

**原文标题**: Companies are scrambling to curtail soaring AI costs

**原文链接**: [https://www.economist.com/business/2026/06/14/companies-are-scrambling-to-curtail-soaring-ai-costs](https://www.economist.com/business/2026/06/14/companies-are-scrambling-to-curtail-soaring-ai-costs)

生成摘要时出错

---

## 52. What's the best way to do authentication in modern applications

**原文标题**: What's the best way to do authentication in modern applications

**原文链接**: [https://neciudan.dev/most-secure-way-to-store-auth-token](https://neciudan.dev/most-secure-way-to-store-auth-token)

生成摘要时出错

---

## 53. Who manages the agents?

**原文标题**: Who manages the agents?

**原文链接**: [https://www.off-policy.com/dont-go-quietly-into-the-ai-night/](https://www.off-policy.com/dont-go-quietly-into-the-ai-night/)

生成摘要时出错

---

## 54. You're Not a Better Engineer Because You Type Git Commands by Hand

**原文标题**: You're Not a Better Engineer Because You Type Git Commands by Hand

**原文链接**: [https://www.minid.net/2026/7/10/ai-works-for-me](https://www.minid.net/2026/7/10/ai-works-for-me)

生成摘要时出错

---

## 55. Star Just Ate a Planet, and It's Not Done Yet

**原文标题**: Star Just Ate a Planet, and It's Not Done Yet

**原文链接**: [https://www.nytimes.com/2026/07/09/science/space/planetary-engulfment-hungry-star.html](https://www.nytimes.com/2026/07/09/science/space/planetary-engulfment-hungry-star.html)

生成摘要时出错

---

## 56. Disable autoplay and infinite scroll or risk fines, EU tells Meta

**原文标题**: Disable autoplay and infinite scroll or risk fines, EU tells Meta

**原文链接**: [https://arstechnica.com/tech-policy/2026/07/disable-auto-play-and-infinite-scroll-or-risk-massive-fines-eu-tells-meta/](https://arstechnica.com/tech-policy/2026/07/disable-auto-play-and-infinite-scroll-or-risk-massive-fines-eu-tells-meta/)

生成摘要时出错

---

## 57. Capitalism Gone Wrong

**原文标题**: Capitalism Gone Wrong

**原文链接**: [https://kasperjunge.com/blog/capitalism-gone-wrong/](https://kasperjunge.com/blog/capitalism-gone-wrong/)

生成摘要时出错

---

## 58. China may restrict foreign access to Chinese open-source AI models

**原文标题**: China may restrict foreign access to Chinese open-source AI models

**原文链接**: [https://www.reuters.com/technology/artificial-intelligence/china-weighs-silicon-curtain-around-sought-after-ai-models-2026-07-08/](https://www.reuters.com/technology/artificial-intelligence/china-weighs-silicon-curtain-around-sought-after-ai-models-2026-07-08/)

生成摘要时出错

---

## 59. Proton AG Services is currently experiencing some issues

**原文标题**: Proton AG Services is currently experiencing some issues

**原文链接**: [https://status.proton.me/incidents/01lxtcq155lc](https://status.proton.me/incidents/01lxtcq155lc)

生成摘要时出错

---

## 60. BLISS

**原文标题**: BLISS

**原文链接**: [https://en.wikipedia.org/wiki/BLISS](https://en.wikipedia.org/wiki/BLISS)

生成摘要时出错

---

## 61. AI Can't Recreate the Thrust Game (But It Can Help You Understand It)

**原文标题**: AI Can't Recreate the Thrust Game (But It Can Help You Understand It)

**原文链接**: [https://www.jamesdrandall.com/posts/thrust_ai_powered_software_archaeology/](https://www.jamesdrandall.com/posts/thrust_ai_powered_software_archaeology/)

生成摘要时出错

---

## 62. France to ban advertising for fossil fuels

**原文标题**: France to ban advertising for fossil fuels

**原文链接**: [https://www.lemonde.fr/en/economy/article/2026/07/09/france-to-ban-advertising-for-fossil-fuels_6755307_19.html](https://www.lemonde.fr/en/economy/article/2026/07/09/france-to-ban-advertising-for-fossil-fuels_6755307_19.html)

生成摘要时出错

---

## 63. Filipino virtual assistants behind LinkedIn's "thought leadership" content mill

**原文标题**: Filipino virtual assistants behind LinkedIn's "thought leadership" content mill

**原文链接**: [https://restofworld.org/2026/virtual-assistant-linkedin-engagement/](https://restofworld.org/2026/virtual-assistant-linkedin-engagement/)

生成摘要时出错

---

## 64. Don't Get Sick in America

**原文标题**: Don't Get Sick in America

**原文链接**: [https://blogography.com/archives/2026/07/dont-get-sick-in-america.html](https://blogography.com/archives/2026/07/dont-get-sick-in-america.html)

生成摘要时出错

---

## 65. China's Open AI Models Are Advancing Its Global Soft Power

**原文标题**: China's Open AI Models Are Advancing Its Global Soft Power

**原文链接**: [https://www.noemamag.com/chinas-open-ai-models-are-advancing-its-global-soft-power/](https://www.noemamag.com/chinas-open-ai-models-are-advancing-its-global-soft-power/)

生成摘要时出错

---

## 66. Guy is banned by OpenAI for cyber abuse, his AI appeals, another AI approves it

**原文标题**: Guy is banned by OpenAI for cyber abuse, his AI appeals, another AI approves it

**原文链接**: [https://twitter.com/endpointarena/status/2075245286339846145](https://twitter.com/endpointarena/status/2075245286339846145)

生成摘要时出错

---

## 67. Ex-Epoch Times CFO pleads guilty in $67M multinational money laundering scheme

**原文标题**: Ex-Epoch Times CFO pleads guilty in $67M multinational money laundering scheme

**原文链接**: [https://apnews.com/article/epoch-times-cfo-indictment-money-laundering-a015b35aaeae44284f0026dc10395acc](https://apnews.com/article/epoch-times-cfo-indictment-money-laundering-a015b35aaeae44284f0026dc10395acc)

生成摘要时出错

---

## 68. How GitHub gave every repository a durable owner

**原文标题**: How GitHub gave every repository a durable owner

**原文链接**: [https://github.blog/security/application-security/how-github-gave-every-repository-a-durable-owner/](https://github.blog/security/application-security/how-github-gave-every-repository-a-durable-owner/)

生成摘要时出错

---

## 69. Earendel (Astronomical Object)

**原文标题**: Earendel (Astronomical Object)

**原文链接**: [https://en.wikipedia.org/wiki/Earendel_(astronomical_object)](https://en.wikipedia.org/wiki/Earendel_(astronomical_object))

生成摘要时出错

---

## 70. Materials innovation has a scale-up problem, not discovery

**原文标题**: Materials innovation has a scale-up problem, not discovery

**原文链接**: [https://www.atomscale.ai/updates/our-thesis-atom-to-scale](https://www.atomscale.ai/updates/our-thesis-atom-to-scale)

生成摘要时出错

---

## 71. Gary Kildall's Death Investigation

**原文标题**: Gary Kildall's Death Investigation

**原文链接**: [https://dfarq.homeip.net/gary-kildalls-death-investigation/](https://dfarq.homeip.net/gary-kildalls-death-investigation/)

生成摘要时出错

---

## 72. Apple sues OpenAI, two former employees for trade secrets theft

**原文标题**: Apple sues OpenAI, two former employees for trade secrets theft

**原文链接**: [https://www.reuters.com/legal/litigation/apple-sues-openai-alleging-misappropriation-trade-secrets-court-records-show-2026-07-10/](https://www.reuters.com/legal/litigation/apple-sues-openai-alleging-misappropriation-trade-secrets-court-records-show-2026-07-10/)

生成摘要时出错

---

## 73. Steam sales reportedly topped $11B during H1 2026 due to shifting trends

**原文标题**: Steam sales reportedly topped $11B during H1 2026 due to shifting trends

**原文链接**: [https://www.tomshardware.com/video-games/pc-gaming/steam-sales-reportedly-topped-usd11-billion-during-h1-2026-due-to-shifting-trends-staggering-growth-driven-by-influx-of-chinese-players-and-booming-legacy-catalogues](https://www.tomshardware.com/video-games/pc-gaming/steam-sales-reportedly-topped-usd11-billion-during-h1-2026-due-to-shifting-trends-staggering-growth-driven-by-influx-of-chinese-players-and-booming-legacy-catalogues)

生成摘要时出错

---

## 74. Publishers Are Preparing to Opt Out of Google Search

**原文标题**: Publishers Are Preparing to Opt Out of Google Search

**原文链接**: [https://www.adweek.com/media/publishers-opt-out-google-search/](https://www.adweek.com/media/publishers-opt-out-google-search/)

生成摘要时出错

---

## 75. UPI: Anatomy of a Payment Transaction

**原文标题**: UPI: Anatomy of a Payment Transaction

**原文链接**: [https://timeseriesofindia.com/economy/reads/upi-architecture/](https://timeseriesofindia.com/economy/reads/upi-architecture/)

生成摘要时出错

---

## 76. I think I was part of a model distillation attack

**原文标题**: I think I was part of a model distillation attack

**原文链接**: [https://sebastianmarines.com/post/i-think-i-was-part-of-a-model-distillation-attack/](https://sebastianmarines.com/post/i-think-i-was-part-of-a-model-distillation-attack/)

生成摘要时出错

---

## 77. Goldman Sachs limits prediction market betting for employees

**原文标题**: Goldman Sachs limits prediction market betting for employees

**原文链接**: [https://www.ft.com/content/7a2a3200-763f-4141-8372-f2f6afba521d](https://www.ft.com/content/7a2a3200-763f-4141-8372-f2f6afba521d)

生成摘要时出错

---

## 78. New York Times says OpenAI hid evidence in ChatGPT copyright trial

**原文标题**: New York Times says OpenAI hid evidence in ChatGPT copyright trial

**原文链接**: [https://techcrunch.com/2026/07/09/new-york-times-says-openai-hid-evidence-in-chatgpt-copyright-trial/](https://techcrunch.com/2026/07/09/new-york-times-says-openai-hid-evidence-in-chatgpt-copyright-trial/)

生成摘要时出错

---

## 79. Show HN: RandoFont – A browser for Google Fonts

**原文标题**: Show HN: RandoFont – A browser for Google Fonts

**原文链接**: [https://randofont.alesh.com](https://randofont.alesh.com)

生成摘要时出错

---

## 80. How RCA Victor sold Sound Service to classrooms in 1939

**原文标题**: How RCA Victor sold Sound Service to classrooms in 1939

**原文链接**: [https://pncnmnp.github.io/blogs/rca-victor-education.html](https://pncnmnp.github.io/blogs/rca-victor-education.html)

生成摘要时出错

---

## 81. He Wanted to Track Microplastics in the Sea. The EPA Fired Him

**原文标题**: He Wanted to Track Microplastics in the Sea. The EPA Fired Him

**原文链接**: [https://www.nytimes.com/2026/07/10/climate/fish-farm-microplastics-maha-epa-firing.html](https://www.nytimes.com/2026/07/10/climate/fish-farm-microplastics-maha-epa-firing.html)

生成摘要时出错

---

## 82. Show HN: SubjectiveZero, an open-source agentic node editor for creative coding

**原文标题**: Show HN: SubjectiveZero, an open-source agentic node editor for creative coding

**原文链接**: [https://sxp.studio/apps/subz](https://sxp.studio/apps/subz)

生成摘要时出错

---

## 83. Show HN: Rubiks Cube Solver

**原文标题**: Show HN: Rubiks Cube Solver

**原文链接**: [https://speedcube.com.br/](https://speedcube.com.br/)

生成摘要时出错

---

## 84. Meta removes AI feature on Instagram after global backlash

**原文标题**: Meta removes AI feature on Instagram after global backlash

**原文链接**: [https://www.rnz.co.nz/news/science-and-technology/700735/missed-the-mark-meta-removes-ai-feature-on-instagram-after-global-backlash](https://www.rnz.co.nz/news/science-and-technology/700735/missed-the-mark-meta-removes-ai-feature-on-instagram-after-global-backlash)

生成摘要时出错

---

