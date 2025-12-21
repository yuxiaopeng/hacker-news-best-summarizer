# Hacker News 热门文章摘要 (2025-12-21)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 备份 Spotify

**原文标题**: Backing up Spotify

**原文链接**: [https://annas-archive.li/blog/backing-up-spotify.html](https://annas-archive.li/blog/backing-up-spotify.html)

Anna's Archive，主要以文本保存而闻名，已启动一项重要项目来备份Spotify的音乐库，创建了“世界上第一个”音乐保存档案库。这一举措弥补了现有音乐档案的空白，这些档案库经常忽视不太流行的曲目，或只专注于高质量文件，使得全面保存变得困难。

该档案库包含2.56亿首曲目（占Spotify的99.9%）的元数据，以及8600万个音乐文件，约占总收听量的99.6%，总计约300TB。这使其成为最大的公开可用音乐元数据数据库，拥有1.86亿个独一无二的ISRC。

该收藏以批量种子（torrents）的形式分发，并根据Spotify的流行度指标进行优先级排序。流行度大于0的曲目以其原始的OGG Vorbis 160kbit/s质量保存，添加元数据时不进行重新编码。流行度等于0的曲目则被重新编码为OGG Opus 75kbit/s，涵盖了约一半此类曲目。所有元数据均以可查询的SQLite数据库形式提供。

该档案库设计为完全开放且易于镜像，旨在保护人类的音乐遗产。Anna's Archive鼓励捐款和种子分享，以支持这项保存工作。丰富的元数据还支持诸如在Spotify整个曲库中实现“真正的随机播放”等功能。

---

## 2. HN 展示：Jmail – 爱泼斯坦文件版谷歌套件

**原文标题**: Show HN: Jmail – Google Suite for Epstein files

**原文链接**: [https://www.jmail.world](https://www.jmail.world)

“Jmail”是一个自称是讽刺艺术项目或概念设计的网站，其带有煽动性地冠名为“爱泼斯坦文件专用谷歌套件”。它声称是一个革命性的云端生产力套件，专门为管理、组织和保护与杰弗里·爱泼斯坦丑闻相关的数字资产而设计。

该平台模仿了成熟的办公套件，提供“Jdrive”等工具用于安全云存储“证据、证词、飞行记录”，以及“Jdocs”用于协作文档编辑。其他功能包括用于财务记录的“Jsheet”，用于安排法律诉讼的“Jcalendar”，用于安全通信的“Jchat”，用于视频会议的“Jmeet”，以及用于端到端加密存储高度敏感数据的“Jvault”。

Jmail 概述了一项使命，即为爱泼斯坦案的所有利益相关者提供一个强大、安全、直观的数字生态系统，强调透明度、问责制和安全性。尽管它详细介绍了功能甚至模拟定价层级（基本版、高级版、企业版），但其明确而敏感的主题，结合对企业的戏仿，将“Jmail”定位为对数据管理、隐私以及公众对备受瞩目案件兴趣的评论，而非真正的商业产品。

---

## 3. CSS 网格轨道

**原文标题**: CSS Grid Lanes

**原文链接**: [https://webkit.org/blog/17660/introducing-css-grid-lanes/](https://webkit.org/blog/17660/introducing-css-grid-lanes/)

CSS Grid Lanes 于 2025 年 12 月 19 日推出，标志着网页布局的重大进步，特别是对于原生瀑布流（masonry-style）设计。经过多年的开发和讨论，它为动态内容排列提供了一个强大的解决方案。

在实现时，开发者在容器上使用 `display: grid-lanes`。这些轨道则通过 `grid-template-columns` 或 `grid-template-rows` 来定义，充分利用 CSS Grid 的强大功能，实现灵活、响应式的布局。例如，`grid-template-columns: repeat(auto-fill, minmax(250px, 1fr))` 可以创建填充可用空间的响应式列，无需媒体查询。

主要特性包括创建不同大小的轨道、让项目跨越多个轨道 (`grid-column: span 4`)，以及显式定位元素的能力。当使用 `grid-template-columns` 时，Grid Lanes 会自动创建“瀑布流”布局；当使用 `grid-template-rows` 时，则创建“砖块”布局，这得益于 `grid-auto-flow` 的新默认值。该系统通过保持逻辑的 Tab 键顺序来提高可访问性，并支持无需 JavaScript 的无限滚动布局。

一个新概念是 `item-tolerance`（默认 `1em`），它控制布局算法放置项目的严格程度，防止细微的尺寸差异导致视觉上和逻辑上令人不适的内容重排。这确保了更流畅的用户体验。

Grid Lanes 目前已在 Safari Technology Preview 234 中可用，其核心语法已趋于稳定，尽管像 `item-tolerance` 这样的一些属性名称仍在最终确定中。鼓励开发者尝试使用它、构建演示，并向 CSS 工作组提供反馈。

---

## 4. 尽管自托管Postgres

**原文标题**: Go ahead, self-host Postgres

**原文链接**: [https://pierce.dev/notes/go-ahead-self-host-postgres#user-content-fn-1](https://pierce.dev/notes/go-ahead-self-host-postgres#user-content-fn-1)

这篇文章挑战了云服务提供商的主流叙事，即自托管数据库，尤其是Postgres，是可怕且危险的。文章认为，这种在2009年随Amazon RDS推出而受到关注并在2015年左右加速发展的“数据库即服务”（DaaS）模式，已经变得过于昂贵，并且往往是一种“无差别的繁重工作”抽象层，而非神奇的解决方案。

作者解释说，托管服务大多运行的是略微修改过的开源Postgres，并配备了运维工具。作者自己运行自托管Postgres两年，每天处理数百万次查询的经验表明，它快速、稳定且便宜得多，仅造成了30分钟的压力。由于更大的调优灵活性，自托管实例的性能甚至可以超越DaaS。

运维复杂性常被夸大；像安全更新和容量规划这样的常规月度任务是可管理的。尽管自托管需要事件响应，但云服务中断也会向用户发出警报，而且通常提供的工具更少。

建议大多数人采用自托管，但绝对的初学者、需要专属数据库工程师的超大型企业或受高度监管的工作负载除外。自托管的关键配置包括：
*   **内存：** 调整 `shared_buffers`、`effective_cache_size`、`work_mem` 和 `maintenance_work_mem`。
*   **连接管理：** 利用 PgBouncer 等连接池工具提高效率。
*   **存储：** 为NVMe SSD优化 `random_page_cost` 等设置。
*   **WAL：** 配置 `wal_level` 和 `max_wal_size` 以确保持久性。

作者总结道，自托管Postgres对许多团队来说占据了一个重要的“最佳位置”，并倡导一个混合基础设施的未来，在这种未来中，自托管应被重新考虑，尤其对于那些为DaaS支付高额月费的用户。

---

## 5. Flock 和 Cyble 公司将所谓的“网络犯罪”取缔行动武器化，以压制批评者。

**原文标题**: Flock and Cyble Inc. weaponize “cybercrime” takedowns to silence critics

**原文链接**: [https://haveibeenflocked.com/news/cyble-downtime](https://haveibeenflocked.com/news/cyble-downtime)

文章《Flock和Cyble公司将“网络犯罪”的关闭用作武器来压制批评》指责网络安全公司Flock和Cyble公司滥用法律和技术机制来压制批评，而非打击真正的网络犯罪。其主要目标是“我被Flocked了吗？”（HIBF），这是一个旨在批判性审查Cyble产品和商业实践的网站，包括过去对可疑数据来源和夸大宣传的指控。

文章称，由Beenu Arora和Deepansh Singh共同创立的Cyble公司，多次对HIBF用于批判性评论的合理使用内容（其中包含Cyble自身的营销材料）发出毫无根据的DMCA通知，声称其侵犯了版权。更令人担忧的是，他们被指控向HIBF的托管服务提供商和域名注册商发送捏造的滥用报告，虚假指控HIBF参与网络犯罪，例如分发恶意软件或进行网络钓鱼。据报道，其中一起事件涉及将HIBF与一个托管在不相关网站上的合法渗透测试工具关联起来，暗示捏造证据以证明关闭行为的合理性。

这些行为导致HIBF大量停机，并迫使其进行多次基础设施迁移。文章将此定性为一种“针对公众参与的战略性诉讼”（SLAPP）策略，并警告称，如果此类做法不受制止，将树立危险先例，允许公司通过虚假指控批评者有犯罪行为来压制合法批评。

---

## 6. 空客将关键应用迁移至主权欧洲云

**原文标题**: Airbus to migrate critical apps to a sovereign Euro cloud

**原文链接**: [https://www.theregister.com/2025/12/19/airbus_sovereign_cloud/](https://www.theregister.com/2025/12/19/airbus_sovereign_cloud/)

空客正准备一项大规模招标，旨在将其包括ERP、制造、CRM和飞机设计在内的关键任务应用程序迁移至欧洲主权云。此举旨在维护对高度敏感数据的数字主权，使其置于欧洲控制之下，并从SAP等供应商那里获取新的、云专属的软件创新。

这家航空航天制造商正寻求减少对美国云服务提供商（微软、AWS、谷歌）的依赖，原因是对美国《云法案》的担忧——该法案允许美国当局访问美国公司在海外持有的数据，以及唐纳德·特朗普预计重返白宫所加剧的更广泛的地缘政治不稳定。空客数字执行副总裁凯瑟琳·杰斯汀对欧洲云服务提供商的规模表示担忧，认为找到合适解决方案的可能性只有80%，尽管提供了超过5000万欧元、为期十年的合同。

提案请求（RFP）将于2026年1月初启动，预计在夏季前做出决定。空客还在寻求关于真正免受域外法律和服务中断影响的监管明确性。

---

## 7. NIST博尔德的NTP已断电

**原文标题**: NTP at NIST Boulder Has Lost Power

**原文链接**: [https://lists.nanog.org/archives/list/nanog@lists.nanog.org/message/ACADD3NKOG2QRWZ56OSNNG7UIEKKTZXL/](https://lists.nanog.org/archives/list/nanog@lists.nanog.org/message/ACADD3NKOG2QRWZ56OSNNG7UIEKKTZXL/)

NIST博尔德的互联网时间服务目前正在传播不准确时间，原因在于长时间的市电中断以及一台关键备用发电机的故障。园区于2025年12月17日世界协调时22:23停电，这是由于强风损坏电力线以及为预防野火而进行的预防性电力关停所致。

此次停电已经影响了原子集成时间尺度，尽管像time-a-b.nist.gov这样的服务器仍通过另一台发电机在线，但NIST正在努力禁用它们，以防止不正确时间的传播。博尔德园区仍对非紧急人员关闭，这阻碍了监测和控制工作。

当前的努力集中在确保替代电源，以保护依靠电池备用运行的氢激微波钟。在电力恢复且工作人员能够进入设施之前，尚无法提供修复估算。NIST希望，一旦情况稳定下来，另一栋楼中由独立发电机供电的额外时钟将允许重新校准主时间尺度。

---

## 8. Privacy doesn't mean anything anymore, anonymity does

**原文标题**: Privacy doesn't mean anything anymore, anonymity does

**原文链接**: [https://servury.com/blog/privacy-is-marketing-anonymity-is-architecture/](https://servury.com/blog/privacy-is-marketing-anonymity-is-architecture/)

生成摘要时出错

---

## 9. Pure Silicon Demo Coding: No CPU, No Memory, Just 4k Gates

**原文标题**: Pure Silicon Demo Coding: No CPU, No Memory, Just 4k Gates

**原文链接**: [https://www.a1k0n.net/2025/12/19/tiny-tapeout-demo.html](https://www.a1k0n.net/2025/12/19/tiny-tapeout-demo.html)

生成摘要时出错

---

## 10. LLM Year in Review

**原文标题**: LLM Year in Review

**原文链接**: [https://karpathy.bearblog.dev/year-in-review-2025/](https://karpathy.bearblog.dev/year-in-review-2025/)

生成摘要时出错

---

## 11. You can now play Grand Theft Auto Vice City in the browser

**原文标题**: You can now play Grand Theft Auto Vice City in the browser

**原文链接**: [https://dos.zone/grand-theft-auto-vice-city/](https://dos.zone/grand-theft-auto-vice-city/)

生成摘要时出错

---

## 12. Over 40% of deceased drivers in vehicle crashes test positive for THC: Study

**原文标题**: Over 40% of deceased drivers in vehicle crashes test positive for THC: Study

**原文链接**: [https://www.facs.org/media-center/press-releases/2025/over-40-of-deceased-drivers-in-motor-vehicle-crashes-test-positive-for-thc-study-shows/](https://www.facs.org/media-center/press-releases/2025/over-40-of-deceased-drivers-in-motor-vehicle-crashes-test-positive-for-thc-study-shows/)

生成摘要时出错

---

## 13. Charles Proxy

**原文标题**: Charles Proxy

**原文链接**: [https://www.charlesproxy.com/](https://www.charlesproxy.com/)

生成摘要时出错

---

## 14. OpenSCAD is kinda neat

**原文标题**: OpenSCAD is kinda neat

**原文链接**: [https://nuxx.net/blog/2025/12/20/openscad-is-kinda-neat/](https://nuxx.net/blog/2025/12/20/openscad-is-kinda-neat/)

The author embarked on learning OpenSCAD by recreating a parameterized battery holder previously designed in Autodesk Fusion. OpenSCAD is a distinctive CAD tool where users write code to generate 3D objects. The simple design of the battery holder—essentially a box with patterned cutouts controlled by input parameters—made it an excellent introductory project and a potential alternative to Fusion for basic designs.

After a few hours, the author successfully developed `battery_holder_generator.scad`. This script allows users to customize a battery holder by adjusting variables like `numRows`, `numColumns`, and `batteryType` (AA or AAA), producing a printable model comparable to the Fusion version without needing expensive software.

The core OpenSCAD code draws a main `cube()` and then uses a `difference()` operation to subtract multiple smaller `cube()` shapes. These smaller cubes represent the battery compartments, and their quantity and precise location are iterated through nested `for` loops and `translate()` commands, with dimensions defined by parameters such as `batteryType` and `thicknessWall`. The author noted some confusion regarding the `let()` statement's necessity within the loop.

While acknowledged as less suitable for complex designs, OpenSCAD is deemed "super useful" for generating simple, parameterized geometric shapes like bearing drifts and spacers, offering a practical and efficient solution for specific real-world needs.

---

## 15. Skills Officially Comes to Codex

**原文标题**: Skills Officially Comes to Codex

**原文链接**: [https://developers.openai.com/codex/skills/](https://developers.openai.com/codex/skills/)

生成摘要时出错

---

## 16. Ireland’s Diarmuid Early wins world Microsoft Excel title

**原文标题**: Ireland’s Diarmuid Early wins world Microsoft Excel title

**原文链接**: [https://www.bbc.com/news/articles/cj4qzgvxxgvo](https://www.bbc.com/news/articles/cj4qzgvxxgvo)

生成摘要时出错

---

## 17. Claude in Chrome

**原文标题**: Claude in Chrome

**原文链接**: [https://claude.com/chrome](https://claude.com/chrome)

生成摘要时出错

---

## 18. Ruby website redesigned

**原文标题**: Ruby website redesigned

**原文链接**: [https://www.ruby-lang.org/en/](https://www.ruby-lang.org/en/)

生成摘要时出错

---

## 19. Show HN: HN Wrapped 2025 - an LLM reviews your year on HN

**原文标题**: Show HN: HN Wrapped 2025 - an LLM reviews your year on HN

**原文链接**: [https://hn-wrapped.kadoa.com?year=2025](https://hn-wrapped.kadoa.com?year=2025)

生成摘要时出错

---

## 20. Big GPUs don't need big PCs

**原文标题**: Big GPUs don't need big PCs

**原文链接**: [https://www.jeffgeerling.com/blog/2025/big-gpus-dont-need-big-pcs](https://www.jeffgeerling.com/blog/2025/big-gpus-dont-need-big-pcs)

生成摘要时出错

---

## 21. Wall Street ruined the Roomba and then blamed Lina Khan

**原文标题**: Wall Street ruined the Roomba and then blamed Lina Khan

**原文链接**: [https://www.thebignewsletter.com/p/how-wall-street-ruined-the-roomba](https://www.thebignewsletter.com/p/how-wall-street-ruined-the-roomba)

生成摘要时出错

---

## 22. Reflections on AI at the End of 2025

**原文标题**: Reflections on AI at the End of 2025

**原文链接**: [https://antirez.com/news/157](https://antirez.com/news/157)

The provided "article" titled "Reflections on AI at the End of 2025" consists solely of its title and no further content. As such, there are no main points, key information, or discussions about AI at the end of 2025 to summarize.

---

## 23. Android introduces $2-4 install fee and 10–20% cut for US external content links

**原文标题**: Android introduces $2-4 install fee and 10–20% cut for US external content links

**原文链接**: [https://support.google.com/googleplay/android-developer/answer/16470497?hl=en](https://support.google.com/googleplay/android-developer/answer/16470497?hl=en)

生成摘要时出错

---

## 24. The Deviancy Signal: Having "Nothing to Hide" Is a Threat to Us All

**原文标题**: The Deviancy Signal: Having "Nothing to Hide" Is a Threat to Us All

**原文链接**: [https://thompson2026.com/blog/deviancy-signal/](https://thompson2026.com/blog/deviancy-signal/)

生成摘要时出错

---

## 25. Why do people leave comments on OpenBenches?

**原文标题**: Why do people leave comments on OpenBenches?

**原文链接**: [https://shkspr.mobi/blog/2025/12/why-do-people-leave-comments-on-openbenches/](https://shkspr.mobi/blog/2025/12/why-do-people-leave-comments-on-openbenches/)

生成摘要时出错

---

## 26. Measuring AI Ability to Complete Long Tasks

**原文标题**: Measuring AI Ability to Complete Long Tasks

**原文链接**: [https://metr.org/blog/2025-03-19-measuring-ai-ability-to-complete-long-tasks/](https://metr.org/blog/2025-03-19-measuring-ai-ability-to-complete-long-tasks/)

生成摘要时出错

---

## 27. A better zip bomb (2019)

**原文标题**: A better zip bomb (2019)

**原文链接**: [https://www.bamsoftware.com/hacks/zipbomb/](https://www.bamsoftware.com/hacks/zipbomb/)

生成摘要时出错

---

## 28. You have reached the end of the internet (2006)

**原文标题**: You have reached the end of the internet (2006)

**原文链接**: [https://hmpg.net/](https://hmpg.net/)

生成摘要时出错

---

## 29. Indoor tanning makes youthful skin much older on a genetic level

**原文标题**: Indoor tanning makes youthful skin much older on a genetic level

**原文链接**: [https://www.ucsf.edu/news/2025/12/431206/indoor-tanning-makes-youthful-skin-much-older-genetic-level](https://www.ucsf.edu/news/2025/12/431206/indoor-tanning-makes-youthful-skin-much-older-genetic-level)

生成摘要时出错

---

## 30. Build Your Own React

**原文标题**: Build Your Own React

**原文链接**: [https://pomb.us/build-your-own-react/](https://pomb.us/build-your-own-react/)

生成摘要时出错

---

## 31. Show HN: Books mentioned on Hacker News in 2025

**原文标题**: Show HN: Books mentioned on Hacker News in 2025

**原文链接**: [https://hackernews-readings-613604506318.us-west1.run.app](https://hackernews-readings-613604506318.us-west1.run.app)

生成摘要时出错

---

## 32. I spent a week without IPv4 (2023)

**原文标题**: I spent a week without IPv4 (2023)

**原文链接**: [https://www.apalrd.net/posts/2023/network_ipv6/](https://www.apalrd.net/posts/2023/network_ipv6/)

生成摘要时出错

---

## 33. Immersa: Open-source Web-based 3D Presentation Tool

**原文标题**: Immersa: Open-source Web-based 3D Presentation Tool

**原文链接**: [https://github.com/ertugrulcetin/immersa](https://github.com/ertugrulcetin/immersa)

生成摘要时出错

---

## 34. PBS News Hour West to go dark after ASU discontinues contract

**原文标题**: PBS News Hour West to go dark after ASU discontinues contract

**原文链接**: [https://www.statepress.com/article/2025/12/politics-pbs-newshour-west-closure](https://www.statepress.com/article/2025/12/politics-pbs-newshour-west-closure)

生成摘要时出错

---

## 35. Clair Obscur having its Indie Game Game Of The Year award stripped due to AI use

**原文标题**: Clair Obscur having its Indie Game Game Of The Year award stripped due to AI use

**原文链接**: [https://www.thegamer.com/clair-obscur-expedition-33-indie-game-awards-goty-stripped-ai-use/](https://www.thegamer.com/clair-obscur-expedition-33-indie-game-awards-goty-stripped-ai-use/)

生成摘要时出错

---

## 36. Is Proton leaving Switzerland?

**原文标题**: Is Proton leaving Switzerland?

**原文链接**: [https://www.techradar.com/vpn/vpn-privacy-security/is-proton-leaving-switzerland-legal-uncertainty-of-proposed-surveillance-laws-is-pushing-them-to-make-several-changes](https://www.techradar.com/vpn/vpn-privacy-security/is-proton-leaving-switzerland-legal-uncertainty-of-proposed-surveillance-laws-is-pushing-them-to-make-several-changes)

生成摘要时出错

---

## 37. What Does a Database for SSDs Look Like?

**原文标题**: What Does a Database for SSDs Look Like?

**原文链接**: [https://brooker.co.za/blog/2025/12/15/database-for-ssd.html](https://brooker.co.za/blog/2025/12/15/database-for-ssd.html)

生成摘要时出错

---

## 38. A train-sized tunnel is now carrying electricity under South London

**原文标题**: A train-sized tunnel is now carrying electricity under South London

**原文链接**: [https://www.ianvisits.co.uk/articles/a-train-sized-tunnel-is-now-carrying-electricity-under-south-london-86221/](https://www.ianvisits.co.uk/articles/a-train-sized-tunnel-is-now-carrying-electricity-under-south-london-86221/)

生成摘要时出错

---

## 39. Coarse Is Better

**原文标题**: Coarse Is Better

**原文链接**: [https://borretti.me/article/coarse-is-better](https://borretti.me/article/coarse-is-better)

生成摘要时出错

---

## 40. Show HN: WalletWallet – create Apple passes from anything

**原文标题**: Show HN: WalletWallet – create Apple passes from anything

**原文链接**: [https://walletwallet.alen.ro/](https://walletwallet.alen.ro/)

生成摘要时出错

---

## 41. Contrails Map

**原文标题**: Contrails Map

**原文链接**: [https://map.contrails.org/](https://map.contrails.org/)

生成摘要时出错

---

## 42. Inca Stone Masonry

**原文标题**: Inca Stone Masonry

**原文链接**: [https://www.earthasweknowit.com/pages/inca_construction](https://www.earthasweknowit.com/pages/inca_construction)

生成摘要时出错

---

## 43. MIRA – An open-source persistent AI entity with memory

**原文标题**: MIRA – An open-source persistent AI entity with memory

**原文链接**: [https://github.com/taylorsatula/mira-OSS](https://github.com/taylorsatula/mira-OSS)

生成摘要时出错

---

## 44. Reasons Not to Become Famous (2020)

**原文标题**: Reasons Not to Become Famous (2020)

**原文链接**: [https://tim.blog/2020/02/02/reasons-to-not-become-famous/](https://tim.blog/2020/02/02/reasons-to-not-become-famous/)

生成摘要时出错

---

## 45. ARIN Public Incident Report – 4.10 Misissuance Error

**原文标题**: ARIN Public Incident Report – 4.10 Misissuance Error

**原文链接**: [https://www.arin.net/announcements/20251212/](https://www.arin.net/announcements/20251212/)

生成摘要时出错

---

## 46. Logging Sucks

**原文标题**: Logging Sucks

**原文链接**: [https://loggingsucks.com/](https://loggingsucks.com/)

生成摘要时出错

---

## 47. Isengard in Oxford

**原文标题**: Isengard in Oxford

**原文链接**: [https://lareviewofbooks.org/article/isengard-in-oxford/](https://lareviewofbooks.org/article/isengard-in-oxford/)

生成摘要时出错

---

## 48. Show HN: Shittp – Volatile Dotfiles over SSH

**原文标题**: Show HN: Shittp – Volatile Dotfiles over SSH

**原文链接**: [https://github.com/FOBshippingpoint/shittp](https://github.com/FOBshippingpoint/shittp)

生成摘要时出错

---

## 49. We ran Anthropic’s interviews through structured LLM analysis

**原文标题**: We ran Anthropic’s interviews through structured LLM analysis

**原文链接**: [https://www.playbookatlas.com/research/ai-adoption-explorer](https://www.playbookatlas.com/research/ai-adoption-explorer)

生成摘要时出错

---

## 50. Anatomy of US inequality

**原文标题**: Anatomy of US inequality

**原文链接**: [https://www.nber.org/papers/w34558](https://www.nber.org/papers/w34558)

生成摘要时出错

---

## 51. Waymo halts service during S.F. blackout after causing traffic jams

**原文标题**: Waymo halts service during S.F. blackout after causing traffic jams

**原文链接**: [https://missionlocal.org/2025/12/sf-waymo-halts-service-blackout/](https://missionlocal.org/2025/12/sf-waymo-halts-service-blackout/)

生成摘要时出错

---

## 52. Anthropic: You can't change your Claude account email address

**原文标题**: Anthropic: You can't change your Claude account email address

**原文链接**: [https://support.claude.com/en/articles/8452276-how-do-i-change-the-email-address-associated-with-my-account](https://support.claude.com/en/articles/8452276-how-do-i-change-the-email-address-associated-with-my-account)

生成摘要时出错

---

## 53. Approaching 50 Years of String Theory

**原文标题**: Approaching 50 Years of String Theory

**原文链接**: [https://www.math.columbia.edu/~woit/wordpress/?p=15401](https://www.math.columbia.edu/~woit/wordpress/?p=15401)

生成摘要时出错

---

## 54. PG&E outages in S.F. leave 130k without electricity

**原文标题**: PG&E outages in S.F. leave 130k without electricity

**原文链接**: [https://www.sfchronicle.com/sf/article/pg-e-outage-40-000-customers-without-power-21254326.php](https://www.sfchronicle.com/sf/article/pg-e-outage-40-000-customers-without-power-21254326.php)

生成摘要时出错

---

## 55. I doubt that anything resembling genuine AGI is within reach of current AI tools

**原文标题**: I doubt that anything resembling genuine AGI is within reach of current AI tools

**原文链接**: [https://mathstodon.xyz/@tao/115722360006034040](https://mathstodon.xyz/@tao/115722360006034040)

生成摘要时出错

---

## 56. The scariest boot loader code

**原文标题**: The scariest boot loader code

**原文链接**: [http://miod.online.fr/software/openbsd/stories/boot_hppa.html](http://miod.online.fr/software/openbsd/stories/boot_hppa.html)

生成摘要时出错

---

## 57. Structured Outputs Create False Confidence

**原文标题**: Structured Outputs Create False Confidence

**原文链接**: [https://boundaryml.com/blog/structured-outputs-create-false-confidence](https://boundaryml.com/blog/structured-outputs-create-false-confidence)

生成摘要时出错

---

## 58. Buteyko Method

**原文标题**: Buteyko Method

**原文链接**: [https://en.wikipedia.org/wiki/Buteyko_method](https://en.wikipedia.org/wiki/Buteyko_method)

生成摘要时出错

---

## 59. E.W.Dijkstra Archive

**原文标题**: E.W.Dijkstra Archive

**原文链接**: [https://www.cs.utexas.edu/~EWD/welcome.html](https://www.cs.utexas.edu/~EWD/welcome.html)

生成摘要时出错

---

## 60. AI will make our children stupid

**原文标题**: AI will make our children stupid

**原文链接**: [https://thecritic.co.uk/ai-will-make-our-children-stupid/](https://thecritic.co.uk/ai-will-make-our-children-stupid/)

生成摘要时出错

---

## 61. The WhatsApp Whisperer

**原文标题**: The WhatsApp Whisperer

**原文链接**: [https://www.whatsprivcy.com/](https://www.whatsprivcy.com/)

生成摘要时出错

---

## 62. Three Ways to Solve Problems

**原文标题**: Three Ways to Solve Problems

**原文链接**: [https://andreasfragner.com/writing/three-ways-to-solve-problems](https://andreasfragner.com/writing/three-ways-to-solve-problems)

生成摘要时出错

---

## 63. ISBN Visualization

**原文标题**: ISBN Visualization

**原文链接**: [https://annas-archive.li/isbn-visualization/](https://annas-archive.li/isbn-visualization/)

生成摘要时出错

---

## 64. At least $9B billed across 14 Medicaid services in Minnesota may be fraudulent

**原文标题**: At least $9B billed across 14 Medicaid services in Minnesota may be fraudulent

**原文链接**: [https://www.cbsnews.com/minnesota/news/billions-paid-out-by-medicaid-in-minnesota-may-be-fraudulent-us-attorney/](https://www.cbsnews.com/minnesota/news/billions-paid-out-by-medicaid-in-minnesota-may-be-fraudulent-us-attorney/)

生成摘要时出错

---

## 65. The New Right-Wing Tech Intelligentsia

**原文标题**: The New Right-Wing Tech Intelligentsia

**原文链接**: [https://bayareacurrent.com/meet-the-new-right-wing-tech-intelligentsia/](https://bayareacurrent.com/meet-the-new-right-wing-tech-intelligentsia/)

生成摘要时出错

---

## 66. AI's Unpaid Debt: How LLM Scrapers Destroy the Social Contract of Open Source

**原文标题**: AI's Unpaid Debt: How LLM Scrapers Destroy the Social Contract of Open Source

**原文链接**: [https://www.quippd.com/writing/2025/12/17/AIs-unpaid-debt-how-llm-scrapers-destroy-the-social-contract-of-open-source.html](https://www.quippd.com/writing/2025/12/17/AIs-unpaid-debt-how-llm-scrapers-destroy-the-social-contract-of-open-source.html)

生成摘要时出错

---

## 67. Airbus moving critical systems away from AWS, Google, and MS

**原文标题**: Airbus moving critical systems away from AWS, Google, and MS

**原文链接**: [https://old.reddit.com/r/europe/comments/1pqucbz/airbus_moving_critical_systems_away_from_aws/](https://old.reddit.com/r/europe/comments/1pqucbz/airbus_moving_critical_systems_away_from_aws/)

生成摘要时出错

---

## 68. Mullvad VPN: "This is a Chat Control 3.0 attempt."

**原文标题**: Mullvad VPN: "This is a Chat Control 3.0 attempt."

**原文链接**: [https://mastodon.online/@mullvadnet/115742530333573065](https://mastodon.online/@mullvadnet/115742530333573065)

生成摘要时出错

---

## 69. Google and Apple warn employees on visas to avoid international travel

**原文标题**: Google and Apple warn employees on visas to avoid international travel

**原文链接**: [https://techcrunch.com/2025/12/20/google-and-apple-reportedly-warn-employees-on-visas-to-avoid-international-travel/](https://techcrunch.com/2025/12/20/google-and-apple-reportedly-warn-employees-on-visas-to-avoid-international-travel/)

生成摘要时出错

---

## 70. New mathematical framework reshapes debate over simulation hypothesis

**原文标题**: New mathematical framework reshapes debate over simulation hypothesis

**原文链接**: [https://www.santafe.edu/news-center/news/new-mathematical-framework-reshapes-debate-over-simulation-hypothesis](https://www.santafe.edu/news-center/news/new-mathematical-framework-reshapes-debate-over-simulation-hypothesis)

生成摘要时出错

---

## 71. Why we're taking legal action against SerpApi's unlawful scraping

**原文标题**: Why we're taking legal action against SerpApi's unlawful scraping

**原文链接**: [https://blog.google/technology/safety-security/serpapi-lawsuit/](https://blog.google/technology/safety-security/serpapi-lawsuit/)

生成摘要时出错

---

## 72. Mathematicians don't care about foundations (2022)

**原文标题**: Mathematicians don't care about foundations (2022)

**原文链接**: [https://matteocapucci.wordpress.com/2022/12/21/mathematicians-dont-care-about-foundations/](https://matteocapucci.wordpress.com/2022/12/21/mathematicians-dont-care-about-foundations/)

生成摘要时出错

---

## 73. Waymo suspends service in San Francisco as robotaxis stall during blackout

**原文标题**: Waymo suspends service in San Francisco as robotaxis stall during blackout

**原文链接**: [https://techcrunch.com/2025/12/21/waymo-suspends-service-in-san-francisco-as-robotaxis-stall-during-blackout/](https://techcrunch.com/2025/12/21/waymo-suspends-service-in-san-francisco-as-robotaxis-stall-during-blackout/)

生成摘要时出错

---

## 74. Show HN: The Official National Train Map Sucked, So I Made My Own

**原文标题**: Show HN: The Official National Train Map Sucked, So I Made My Own

**原文链接**: [https://www.bdzmap.com/](https://www.bdzmap.com/)

生成摘要时出错

---

## 75. Show HN: Claude Code Plugin to play music when waiting on user input

**原文标题**: Show HN: Claude Code Plugin to play music when waiting on user input

**原文链接**: [https://github.com/Sevii/agent-marketplace/blob/main/plugins/elevator-music/README.md](https://github.com/Sevii/agent-marketplace/blob/main/plugins/elevator-music/README.md)

生成摘要时出错

---

## 76. Performance Hints

**原文标题**: Performance Hints

**原文链接**: [https://abseil.io/fast/hints.html](https://abseil.io/fast/hints.html)

生成摘要时出错

---

## 77. TailwindSQL – Like TailwindCSS, but for SQL queries in React Server components

**原文标题**: TailwindSQL – Like TailwindCSS, but for SQL queries in React Server components

**原文链接**: [https://github.com/mmarinovic/tailwindsql](https://github.com/mmarinovic/tailwindsql)

生成摘要时出错

---

## 78. More databases should be single-threaded

**原文标题**: More databases should be single-threaded

**原文链接**: [https://blog.konsti.xyz/p/8c8a399f-8cfe-47dd-9278-9527105d07dc/](https://blog.konsti.xyz/p/8c8a399f-8cfe-47dd-9278-9527105d07dc/)

生成摘要时出错

---

## 79. Mountain home near Aspen, built for monks, sold to Palantir CEO for $120M

**原文标题**: Mountain home near Aspen, built for monks, sold to Palantir CEO for $120M

**原文链接**: [https://coloradosun.com/2025/12/19/monastery-sells-palantir-ceo/](https://coloradosun.com/2025/12/19/monastery-sells-palantir-ceo/)

生成摘要时出错

---

## 80. Debian adds LoongArch as officially supported architecture

**原文标题**: Debian adds LoongArch as officially supported architecture

**原文链接**: [https://lists.debian.org/debian-devel-announce/2025/12/msg00004.html](https://lists.debian.org/debian-devel-announce/2025/12/msg00004.html)

生成摘要时出错

---

## 81. Mozilla right now (Digital Painting)

**原文标题**: Mozilla right now (Digital Painting)

**原文链接**: [https://www.davidrevoy.com/article1108/mozilla-right-now](https://www.davidrevoy.com/article1108/mozilla-right-now)

生成摘要时出错

---

## 82. Show HN: Stickerbox, a kid-safe, AI-powered voice to sticker printer

**原文标题**: Show HN: Stickerbox, a kid-safe, AI-powered voice to sticker printer

**原文链接**: [https://stickerbox.com/](https://stickerbox.com/)

生成摘要时出错

---

## 83. Data Bank – Nuforc – Latest UFO Sightings

**原文标题**: Data Bank – Nuforc – Latest UFO Sightings

**原文链接**: [https://nuforc.org/databank/](https://nuforc.org/databank/)

生成摘要时出错

---

## 84. School security AI flagged clarinet as a gun. Exec says it wasn't an error

**原文标题**: School security AI flagged clarinet as a gun. Exec says it wasn't an error

**原文链接**: [https://arstechnica.com/tech-policy/2025/12/florida-schools-plan-to-vastly-expand-use-of-ai-that-mistook-clarinet-for-gun/](https://arstechnica.com/tech-policy/2025/12/florida-schools-plan-to-vastly-expand-use-of-ai-that-mistook-clarinet-for-gun/)

生成摘要时出错

---

## 85. Unix v4 tape raw binary image recovered

**原文标题**: Unix v4 tape raw binary image recovered

**原文链接**: [https://elk.zone/hachyderm.io/@ricci@discuss.systems/115748594405893972](https://elk.zone/hachyderm.io/@ricci@discuss.systems/115748594405893972)

生成摘要时出错

---

## 86. White House website mysteriously streams personal finance YouTube creator

**原文标题**: White House website mysteriously streams personal finance YouTube creator

**原文链接**: [https://www.pbs.org/newshour/politics/white-house-website-mysteriously-streams-personal-finance-youtube-creator](https://www.pbs.org/newshour/politics/white-house-website-mysteriously-streams-personal-finance-youtube-creator)

生成摘要时出错

---

## 87. Show HN: RenderCV – Open-source CV/resume generator, YAML → PDF

**原文标题**: Show HN: RenderCV – Open-source CV/resume generator, YAML → PDF

**原文链接**: [https://github.com/rendercv/rendercv](https://github.com/rendercv/rendercv)

生成摘要时出错

---

## 88. I wrote a code editor in C and now I'm a changed man

**原文标题**: I wrote a code editor in C and now I'm a changed man

**原文链接**: [https://github.com/thisismars-x/light](https://github.com/thisismars-x/light)

生成摘要时出错

---

## 89. Recursive Project Search in Emacs

**原文标题**: Recursive Project Search in Emacs

**原文链接**: [https://lukeplant.me.uk/blog/posts/recursive-project-search-in-emacs/](https://lukeplant.me.uk/blog/posts/recursive-project-search-in-emacs/)

生成摘要时出错

---

## 90. U.S. Plans $80B Nuclear Power Expansion

**原文标题**: U.S. Plans $80B Nuclear Power Expansion

**原文链接**: [https://spectrum.ieee.org/80-billion-us-nuclear-power](https://spectrum.ieee.org/80-billion-us-nuclear-power)

生成摘要时出错

---

## 91. Sequoia partner spreads debunked Brown shooting theory, testing new leadership

**原文标题**: Sequoia partner spreads debunked Brown shooting theory, testing new leadership

**原文链接**: [https://techcrunch.com/2025/12/19/sequoia-partner-spreads-debunked-brown-shooting-theory-testing-new-leadership/](https://techcrunch.com/2025/12/19/sequoia-partner-spreads-debunked-brown-shooting-theory-testing-new-leadership/)

生成摘要时出错

---

## 92. Jeffrey Epstein Court Records

**原文标题**: Jeffrey Epstein Court Records

**原文链接**: [https://www.justice.gov/epstein/court-records](https://www.justice.gov/epstein/court-records)

生成摘要时出错

---

## 93. ELF Crimes: Program Interpreter Fun

**原文标题**: ELF Crimes: Program Interpreter Fun

**原文链接**: [https://nytpu.com/gemlog/2025-12-21](https://nytpu.com/gemlog/2025-12-21)

生成摘要时出错

---

## 94. Pa. high court rules that police can access Google searches without a warrant

**原文标题**: Pa. high court rules that police can access Google searches without a warrant

**原文链接**: [https://therecord.media/google-searches-police-access-without-warrant-pennsylvania-court-ruling](https://therecord.media/google-searches-police-access-without-warrant-pennsylvania-court-ruling)

生成摘要时出错

---

## 95. Day laborers protest noise machines installed at Home Depot

**原文标题**: Day laborers protest noise machines installed at Home Depot

**原文链接**: [https://www.latimes.com/california/story/2025-12-17/day-laborers-protest-noise-machines-home-depot](https://www.latimes.com/california/story/2025-12-17/day-laborers-protest-noise-machines-home-depot)

生成摘要时出错

---

## 96. The post-GeForce era: What if Nvidia abandons PC gaming?

**原文标题**: The post-GeForce era: What if Nvidia abandons PC gaming?

**原文链接**: [https://www.pcworld.com/article/3013044/the-post-geforce-era-what-if-nvidia-abandons-pc-gaming.html](https://www.pcworld.com/article/3013044/the-post-geforce-era-what-if-nvidia-abandons-pc-gaming.html)

生成摘要时出错

---

## 97. Man sues cops who jailed him for 37 days for trolling a Charlie Kirk vigil

**原文标题**: Man sues cops who jailed him for 37 days for trolling a Charlie Kirk vigil

**原文链接**: [https://arstechnica.com/tech-policy/2025/12/man-sues-cops-who-jailed-him-for-37-days-for-trolling-a-charlie-kirk-vigil/](https://arstechnica.com/tech-policy/2025/12/man-sues-cops-who-jailed-him-for-37-days-for-trolling-a-charlie-kirk-vigil/)

生成摘要时出错

---

## 98. Humankind's 10 million year love affair with booze might end

**原文标题**: Humankind's 10 million year love affair with booze might end

**原文链接**: [https://www.economist.com/christmas-specials/2025/12/18/how-humankinds-10m-year-love-affair-with-booze-might-end](https://www.economist.com/christmas-specials/2025/12/18/how-humankinds-10m-year-love-affair-with-booze-might-end)

生成摘要时出错

---

## 99. It's time to accept the US Supreme Court is illegitimate and must be replaced

**原文标题**: It's time to accept the US Supreme Court is illegitimate and must be replaced

**原文链接**: [https://www.theguardian.com/commentisfree/2025/dec/19/us-supreme-court-legitimacy](https://www.theguardian.com/commentisfree/2025/dec/19/us-supreme-court-legitimacy)

生成摘要时出错

---

## 100. A brief history of Sam Altman's hype

**原文标题**: A brief history of Sam Altman's hype

**原文链接**: [https://www.technologyreview.com/2025/12/15/1129169/a-brief-history-of-sam-altmans-hype/](https://www.technologyreview.com/2025/12/15/1129169/a-brief-history-of-sam-altmans-hype/)

生成摘要时出错

---

