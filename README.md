# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-08-29.md)

*最后自动更新时间: 2026-08-29 22:00:37*
## 1. 防止智能电视被用来对付你

**原文标题**: Stopping the smart TV from being used against you

**原文链接**: [https://www.s-config.com/stopping-a-smart-tv-from-being-used-against-you/](https://www.s-config.com/stopping-a-smart-tv-from-being-used-against-you/)

该文章严厉抨击智能电视制造商，特别是LG，指责它们利用用户信任、侵犯隐私来安装不需要的软件并以此创收。文章指出，这些公司将用户视为被许可方而非所有者，并且“恶意软件”（如迈克菲杀毒软件等未经请求的软件）经常被推送到连接设备上，即使电视没有连接互联网。

这种攻击的主要机制被确定为扩展显示识别数据（EDID）。当一台已连接互联网的笔记本电脑（尤其是Windows系统）通过HDMI连接到智能电视时，据称制造商会利用传输显示信息的EDID协议。文章声称，这使得电视的“驱动程序”可以通过Windows Update安装，充当额外臃肿软件的特洛伊木马，而微软可能因经济利益而有所勾结。Linux系统目前更安全，但面临潜在的未来风险。

为了应对这些威胁，文章强烈推荐使用基于硬件的EDID阻断器。这些设备会向电脑谎报电视的身份，从而阻止安装制造商特定的驱动程序和相关恶意软件。其他策略包括永不将智能设备连接到互联网、使用强大的防火墙、切换到基于Linux的操作系统进行媒体消费，或者选择非智能替代品，如投影仪。作者总结道，主动进行硬件保护，例如EDID阻断器，对于防止智能电视被用来对付你至关重要，尤其是在被迫连接工作笔记本电脑时。

---

## 2. Stripe称放弃500亿美元收购PayPal

**原文标题**: Stripe said to abandon $50B pursuit of PayPal

**原文链接**: [https://www.bloomberg.com/news/articles/2026-08-28/advent-stripe-consortium-is-said-to-drop-pursuit-of-paypal](https://www.bloomberg.com/news/articles/2026-08-28/advent-stripe-consortium-is-said-to-drop-pursuit-of-paypal)

无法访问文章链接。

---

## 3. StemDeck，一个免费、开源、本地的 AI 音轨分离器

**原文标题**: StemDeck, a free, open-source and local AI stem separator

**原文链接**: [https://github.com/stemdeckapp/stemdeck](https://github.com/stemdeckapp/stemdeck)

生成摘要时出错

---

## 4. 国土安全部正利用鲜为人知的法律窥探记者、非营利组织和工会。

**原文标题**: DHS is using obscure law to snoop on journalists, non-profits, unions

**原文链接**: [https://www.theguardian.com/us-news/2026/aug/29/trump-dhs-1509-summons-records-journalists-nonprofits](https://www.theguardian.com/us-news/2026/aug/29/trump-dhs-1509-summons-records-journalists-nonprofits)

国土安全部（DHS）正在争议性地利用一项鲜为人知的海关法（19 USC 1509），秘密获取记者、非营利组织和工会的私人信息，规避了传统的司法监督。这项条款原本旨在调查关税和进口，但目前却被应用于与其初衷无关的国内事务。

对于记者乔治亚·福特，国土安全部在使用这份行政传票，向T-Mobile索要了六个月的电话记录，并向谷歌索要了YouTube账户信息，此前法官曾两次以缺乏合理理由为由驳回了搜查令请求。T-Mobile在未通知福特的情况下照办了电话记录请求，而谷歌则予以抵制，质疑其与海关调查的关联。

批评人士，包括前国土安全部官员，认为这是一种“令人发指”且“不当”的权力滥用，他们认为这绕过了第四修正案的保护，并威胁到新闻来源和第一修正案的权利。国土安全部还曾针对其他记者（如唐·莱蒙、梅根·凯利）、媒体机构（如“民主现在时”）、活动组织（如“日出运动”、美国服务业雇员国际工会、争取种族正义之声）以及批评移民和海关执法局（ICE）的个人。

国土安全部声称该法规赋予了超越海关的广泛调查权力，但专家普遍认为这是一种“过度宽泛的误读”。尽管谷歌等一些公司挑战这些要求，但其他公司却遵从，将质疑合法性的昂贵负担转嫁给用户。令人担忧的是，国土安全部在法院受到质疑时经常撤回这些传票，批评人士认为这种策略是为了避免对其合法性做出明确的法律裁决。一份2017年的总检察长报告此前曾指出，这些1509号传票的使用存在“不一致——在某些情况下，甚至是不当”的问题。

---

## 5. 我为一家初创公司使用过AWS Cognito，我不会再这样做了。

**原文标题**: I used AWS cognito for a startup. I wouldn't do it again

**原文链接**: [https://joshkaramuth.com/blog/aws-cognito-authentication-startup-nightmare/](https://joshkaramuth.com/blog/aws-cognito-authentication-startup-nightmare/)

作者，作为一名经验丰富的开发者，讲述了在使用AWS Cognito为其初创公司设置身份验证时，一次令人深感沮丧的经历。尽管最初因其生态系统集成和慷慨的免费套餐而吸引人，但Cognito却成为了一个巨大的阻碍。

突出显示的关键问题包括：

1.  **文档混乱：** 文档试图服务于过多的受众，导致其成为一个杂乱无章、非线性的超链接网络，其中包含过时和混合版本的代码示例（如旧的JavaScript SDK、Amplify v1和原始AWS SDK），使得查找相关信息变得困难。
2.  **破坏性API变更：** Amplify从v5到v6的一次重大更新，彻底重构了与Cognito的交互方式，迫使作者不得不完全重写现有且原本可用的身份验证逻辑。
3.  **本地开发支持不佳：** Cognito仅限于云端的特性使得本地测试充满挑战，开发者不得不依赖于不一致的社区模拟器而非官方本地实例，从而导致错误在预发布环境中才出现。
4.  **定制化能力有限：** 托管UI提供的品牌定制选项极少（主要限于Logo和基本的CSS调整），这迫使开发者构建自定义UI，大大削弱了其本应提供的便利性。
5.  **配置不灵活：** 一个关键痛点是用户池创建后无法更改属性类型（例如，自定义属性与标准属性），导致开发者为了一个看似微小的设置错误，面临删除用户池或进行复杂用户迁移的两难境地。

作者总结道，在选择身份验证解决方案时，开发者体验应是首要考虑因素，而非生态系统便利性或免费定价。因Cognito问题而损失的工程时间远远超过了任何成本节约。他们建议任何考虑使用Cognito的人进行彻底的概念验证，并警告其可能带来耗时的沮丧。尽管心怀不满，但他们目前投入过大，已无法切换。

---

## 6. 地图现状 2026

**原文标题**: State of the Map 2026

**原文链接**: [https://2026.stateofthemap.org/](https://2026.stateofthemap.org/)

State of the Map 2026 大会是制图者和OpenStreetMap用户一年一度的盛会，将于2026年8月28日至30日在法国巴黎举行。为期三天的会议地点设在马恩河畔尚皮涅的笛卡尔城，将包括讲座、研讨会和讨论环节，支持线上和线下两种参与方式。

与会者可以找到关于会议日程、场馆路线、社交活动和会议海报等重要信息。线上参与将通过Matrix或Telegram上的聊天室、Mastodon等社交媒体渠道以及直播进行，Venueless门票持有者可获得互动功能访问权限。

本次活动强调了通过捐款支持OpenStreetMap的重要性，以确保其稳定性、质量和独立性。本次大会得到了众多合作伙伴和赞助商的支持。白金赞助商包括致力于加强OSM生态系统并促进合作的TomTom，以及米其林（Michelin）。米其林是一家全球领导者，凭借其在工程材料方面的深厚专有技术，提供数据和人工智能驱动的互联解决方案，同时也是《米其林指南》的发布者。其他赞助商分为金、银、铜和支持者等级别，包括FerryGoGo、YellowMap和OpenRunner等公司。

---

## 7. TurboKV：极速Rust键值存储

**原文标题**: TurboKV: Insanely fast Rust key-value store

**原文链接**: [https://github.com/kingroryg/turbokv](https://github.com/kingroryg/turbokv)

TurboKV 是一个快速、异步、嵌入式的键值存储，采用 Rust 编写，具有原子批处理、有序范围扫描、可配置的持久性、压缩和后台压缩等特性。它旨在提供高性能，利用硬件 AES 实现其布隆过滤器格式。

安装非常简单，只需使用 `cargo add turbokv tokio` 命令，并要求设置特定的 RUSTFLAGS（x86/x86_64 平台为 `+aes,+sse2`，ARM/AArch64 平台为 `+aes,+neon`）以启用硬件加速。

快速入门演示了如何使用 `Db::open_with_options` 打开数据库，执行 `insert`、`get`、`remove` 和 `write_batch` 操作，并使用 `scan_prefix` 进行迭代。键和值是任意字节序列。

TurboKV 提供三种持久性预设：
*   **DbOptions::fast()**：内存可见性，无 WAL（预写日志），适用于缓存。
*   **DbOptions::durable()**：（推荐的默认设置）启用 WAL，用于进程崩溃恢复，并定期进行断电检查点。
*   **DbOptions::paranoid()**：最强模式，按写入组同步 WAL 以提供最大保证，但受文件系统影响。

核心操作包括 `insert`、`get`、`remove`、`take`（原子获取并移除）、`contains_key` 以及用于原子事务的 `write_batch`。范围和前缀扫描提供即时视图，返回急切收集的向量或流式迭代器以实现高效遍历。维护 API 包括 `flush`（刷新）、`compact`（压缩）和各种 `stats`（统计）快照。

基准测试凸显了 TurboKV 的速度：
*   **Fast** 和 **Durable** 模式在单键操作中达到每秒数百万个键的速度，批量操作速度更高。
*   **Paranoid** 模式的单键吞吐量较低，原因是严格的存储同步延迟，但通过批处理可以显著提高，从而分摊同步成本。
*   与 fjall 和 redb 相比，TurboKV 在其 `Fast` 和 `Durable` 配置中表现出卓越的吞吐量，并且批处理显著提升了 `Paranoid` 模式的性能。

---

## 8. 第九巡回法院在卡尔希赌博纠纷中支持各州。

**原文标题**: 9th Circuit sides with states in Kalshi gambling fight

**原文链接**: [https://azmirror.com/2026/08/28/9th-circuit-sides-with-states-in-kalshi-gambling-fight-potentially-reviving-arizonas-prosecution/](https://azmirror.com/2026/08/28/9th-circuit-sides-with-states-in-kalshi-gambling-fight-potentially-reviving-arizonas-prosecution/)

The 9th U.S. Circuit Court of Appeals has ruled that gambling on sporting events is not protected by the federal Commodity Exchange Act (CEA), a decision significantly bolstering states' authority to regulate prediction market companies like Kalshi. This ruling, from a Nevada case, directly undercuts a federal judge's injunction that had stopped Arizona from prosecuting Kalshi for violating state gambling laws, including betting on election outcomes.

The three-judge panel unanimously concluded that sports events do not qualify as "swaps" under the CEA, rejecting Kalshi's broad interpretation that "events" and "occurrences" in the act cover sports outcomes. The court clarified that while an event *happening* is an occurrence, *who wins* is not, stating Congress did not intend to dismantle decades of state and tribal gambling regulations.

Arizona Attorney General Kris Mayes lauded the decision as a "significant win for states’ authority," explaining that the CEA was never meant to strip states of their traditional police power over gambling. The ruling paves the way for Arizona to ask for the dissolution of the injunction, potentially allowing the state's criminal case against Kalshi to resume.

This 9th Circuit decision creates a circuit split, contradicting an earlier 3rd U.S. Circuit Court of Appeals ruling that sided with Kalshi. The 9th Circuit invoked the "major questions doctrine," arguing that granting the Commodity Futures Trading Commission authority over sports betting would be an "extraordinary" power requiring clear congressional authorization. This legal divergence sets the stage for a potential review by the U.S. Supreme Court.

---

## 9. Good Culture Is the Biggest Productivity Hack, Not AI

**原文标题**: Good Culture Is the Biggest Productivity Hack, Not AI

**原文链接**: [https://newsletter.eng-leadership.com/p/good-culture-is-the-biggest-productivity](https://newsletter.eng-leadership.com/p/good-culture-is-the-biggest-productivity)

生成摘要时出错

---

## 10. Verschlimmbesserung: The Word Your Software Updates Need

**原文标题**: Verschlimmbesserung: The Word Your Software Updates Need

**原文链接**: [https://geekyschmidt.com/post/2026-08-25-verschlimmbesserung/](https://geekyschmidt.com/post/2026-08-25-verschlimmbesserung/)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-08-29](output/hacker_news_summary_2026-08-29.md) |
| 2 | [2026-08-21](output/hacker_news_summary_2026-08-21.md) |
| 3 | [2026-08-25](output/hacker_news_summary_2026-08-25.md) |
| 4 | [2026-08-20](output/hacker_news_summary_2026-08-20.md) |
| 5 | [2026-08-26](output/hacker_news_summary_2026-08-26.md) |
| 6 | [2026-08-24](output/hacker_news_summary_2026-08-24.md) |
| 7 | [2026-08-28](output/hacker_news_summary_2026-08-28.md) |
| 8 | [2026-08-23](output/hacker_news_summary_2026-08-23.md) |
| 9 | [2026-08-22](output/hacker_news_summary_2026-08-22.md) |
| 10 | [2026-08-18](output/hacker_news_summary_2026-08-18.md) |
| 11 | [2026-08-15](output/hacker_news_summary_2026-08-15.md) |
| 12 | [2026-08-19](output/hacker_news_summary_2026-08-19.md) |
| 13 | [2026-08-13](output/hacker_news_summary_2026-08-13.md) |
| 14 | [2026-08-14](output/hacker_news_summary_2026-08-14.md) |
| 15 | [2026-08-17](output/hacker_news_summary_2026-08-17.md) |
| 16 | [2026-08-16](output/hacker_news_summary_2026-08-16.md) |
| 17 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 18 | [2026-08-09](output/hacker_news_summary_2026-08-09.md) |
| 19 | [2026-08-10](output/hacker_news_summary_2026-08-10.md) |
| 20 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 21 | [2026-08-11](output/hacker_news_summary_2026-08-11.md) |
| 22 | [2026-08-12](output/hacker_news_summary_2026-08-12.md) |
| 23 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 24 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 25 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 26 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 27 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 28 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 29 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 30 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 31 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 32 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 33 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 34 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 35 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 36 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 37 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 38 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 39 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 40 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 41 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 42 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 43 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 44 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 45 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 46 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 47 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 48 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 49 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 50 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 51 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 52 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 53 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 54 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 55 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 56 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 57 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 58 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 59 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 60 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 61 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 62 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 63 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 64 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 65 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 66 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 67 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 68 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 69 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 70 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 71 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 72 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 73 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 74 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 75 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 76 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 77 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 78 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 79 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 80 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 81 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 82 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 83 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 84 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 85 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 86 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 87 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 88 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 89 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 90 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 91 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 92 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 93 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 94 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 95 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 96 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 97 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 98 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 99 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 100 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 101 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 102 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 103 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 104 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 105 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 106 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 107 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 108 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 109 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 110 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 111 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 112 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 113 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 114 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 115 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 116 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 117 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 118 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 119 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 120 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 121 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 122 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 123 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 124 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 125 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 126 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 127 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 128 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 129 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 130 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 131 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 132 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 133 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 134 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 135 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 136 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 137 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 138 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 139 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 140 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 141 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 142 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 143 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 144 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 145 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 146 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 147 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 148 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 149 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 150 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 151 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 152 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 153 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 154 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 155 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 156 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 157 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 158 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 159 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 160 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 161 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 162 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 163 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 164 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 165 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 166 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 167 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 168 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 169 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 170 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 171 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 172 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 173 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 174 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 175 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 176 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 177 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 178 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 179 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 180 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 181 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 182 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 183 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 184 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 185 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 186 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 187 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 188 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 189 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 190 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 191 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 192 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 193 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 194 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 195 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 196 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 197 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 198 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 199 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 200 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 201 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 202 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 203 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 204 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 205 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 206 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 207 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 208 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 209 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 210 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 211 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 212 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 213 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 214 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 215 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 216 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 217 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 218 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 219 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 220 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 221 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 222 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 223 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 224 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 225 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 226 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 227 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 228 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 229 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 230 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 231 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 232 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 233 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 234 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 235 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 236 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 237 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 238 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 239 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 240 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 241 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 242 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 243 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 244 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 245 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 246 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 247 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 248 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 249 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 250 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 251 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 252 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 253 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 254 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 255 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 256 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 257 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 258 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 259 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 260 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 261 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 262 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 263 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 264 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 265 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 266 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 267 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 268 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 269 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 270 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 271 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 272 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 273 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 274 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 275 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 276 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 277 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 278 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 279 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 280 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 281 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 282 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 283 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 284 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 285 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 286 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 287 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 288 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 289 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 290 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 291 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 292 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 293 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
