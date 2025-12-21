# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2025-12-21.md)

*最后自动更新时间: 2025-12-21 19:46:09*
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

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 2 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 3 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 4 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 5 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 6 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 7 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 8 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 9 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 10 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 11 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 12 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 13 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 14 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 15 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 16 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 17 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 18 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 19 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 20 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 21 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 22 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 23 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 24 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 25 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 26 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 27 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 28 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 29 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 30 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 31 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 32 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 33 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 34 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 35 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 36 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 37 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 38 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 39 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 40 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 41 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 42 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 43 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 44 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 45 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
| 46 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
