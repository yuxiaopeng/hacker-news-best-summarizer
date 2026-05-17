# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-05-17.md)

*最后自动更新时间: 2026-05-17 20:16:20*
## 1. 帕兰提尔已聘用了30多名英国政府高级官员。

**原文标题**: Palantir has hired more than 30 senior UK Government officials

**原文链接**: [https://www.thenational.scot/news/26055524.palantir-hired-30-senior-uk-government-officials/](https://www.thenational.scot/news/26055524.palantir-hired-30-senior-uk-government-officials/)

据《The Nerve》的一项调查发现，美国科技公司Palantir自2012年以来，据报道已雇佣了32名英国政府和公共部门高级官员。这些官员来自不同部门，包括英国国家医疗服务体系（NHS）、国防部（MoD）、内政部、外交部、英国卫生安全局、情报机构以及唐宁街。

这一消息传出之际，正值Palantir在英国政府合同不断增加以及其有争议的活动受到密切审查。这些争议活动包括与美国移民与海关执法局（ICE）合作，以及通过向以色列国防军（IDF）提供服务，被指控在加沙“从种族灭绝中获利”。

透明度专家警告称，尽管没有暗示存在不当行为，但这种大量前官员的涌入造成了“严重的腐败风险”，因为他们可能利用特权信息和人脉。值得注意的聘用包括国防部高级人工智能官员（曾参与编写英国军事人工智能战略）和英格兰国家医疗服务体系前人工智能主管。此外，四名上议院议员曾为Palantir提供咨询，其顾问团队中包括两名将军和一名前首相首席顾问。

Palantir否认存在“旋转门”策略，并表示在提到的32名官员中（跨越15年），有14人已不再为该公司工作，且有六人是前武装部队退伍军人。该公司辩称，将退伍军人纳入此类指控是不恰当的，因为社会应该支持他们的职业转型，并否认寻求特权洞察力的说法。

---

## 2. 如何写入SSD [pdf]

**原文标题**: How to Write to SSDs [pdf]

**原文链接**: [https://www.vldb.org/pvldb/vol19/p1469-lee.pdf](https://www.vldb.org/pvldb/vol19/p1469-lee.pdf)

论文《如何写入SSD》介绍了一种名为Snail的新颖软件架构，旨在缓解数据库系统在与传统固态硬盘（SSD）交互时所遇到的显著写入放大（WA）和性能下降问题。传统的数据库存储引擎，特别是使用日志结构合并树（LSM树）的那些，会产生大量小、随机且异地写入。这与SSD基于块的“先擦除再写入”操作及其内部垃圾回收机制相冲突，从而导致高写入放大、吞吐量降低、延迟增加以及SSD寿命缩短。

尽管像区域命名空间（ZNS）SSD这样的解决方案在硬件层面解决了WA问题，但它们需要专门的硬件和广泛的软件修改。Snail提供了一种纯软件解决方案，作为介于存储引擎（例如RocksDB）和传统SSD之间的块设备驱动层。

Snail通过将数据组织成“写入优化块”（WOBs）和“写入优化块组”（WOBGs）来重新优化软件-SSD接口。它在这些单元内部以只追加方式管理数据，逻辑上分离有效页和无效页，并在WOBGs上执行其自身高效的垃圾回收。这种方法有效地将随机数据库写入转换为SSD接口上的顺序写入，从而避免了闪存转换层（FTL）执行大量的异地更新和随后的内部垃圾回收。

评估结果表明，与原生SSD使用相比，Snail显著降低了写入放大，最高可达7倍，并在无需专门硬件的情况下实现了与ZNS SSD相当的WA水平。这种降低意味着写入吞吐量大幅提高、尾延迟更低，以及数据库工作负载下SSD寿命的延长，提供了一种实用且可部署的解决方案来优化SSD利用率。

---

## 3. P2P冰毒的主要特点就是其供应量巨大 (2021年)

**原文标题**: The main thing about P2P meth is that there's so much of it (2021)

**原文链接**: [https://dynomight.net/p2p-meth/](https://dynomight.net/p2p-meth/)

本文挑战了Sam Quinones提出的观点，即自2017年以来流行的“新型”P2P合成冰毒在化学上与“旧型”麻黄碱冰毒不同，并导致使用者“发疯”。

作者解释说，由于对麻黄碱前体物的禁令，美国的冰毒供应在2009年至2012年间转向P2P合成。尽管最初的P2P冰毒确实含有l-甲基苯丙胺（一种效力较低的异构体），但美国缉毒局的数据显示，到2019年，这种异构体已几乎被消除。此外，分析表明，现代街头冰毒的纯度比以往任何时候都高，d-甲基苯丙胺平均含量达95%，而且P2P合成方法的变化（例如，醋酸铅的使用变化）与精神分裂症报告增加的时间线不符。

相反，文章提出，P2P合成的主要影响是冰毒可及性和使用量的急剧增加。其证据包括边境查获量飙升、约在2017年西雅图等城市冰毒使用量翻倍、2015年至2019年间重度使用者数量增加了两倍、街头价格暴跌，以及吸毒过量死亡人数的严重激增（2020年超过24,000人）。

作者总结说，微妙的化学差异或污染物不太可能是原因。相反，历史上巨量的强效冰毒供应导致了广泛和强烈的使用，这是观察到的社会问题最可能的原因，作者认为“量变引起质变”。

---

## 4. Meta将为其100亿美元的路易斯安那州数据中心获得33亿美元的税收减免

**原文标题**: Meta to receive $3.3B in tax breaks for its $10B Louisiana data center

**原文链接**: [https://fortune.com/2026/05/14/meta-data-center-tax-break-hyperion-louisiana/](https://fortune.com/2026/05/14/meta-data-center-tax-break-hyperion-louisiana/)

各州为吸引对人工智能至关重要的数据中心，正提供巨额税收减免，导致数十亿美元的税收损失。弗吉尼亚州每年提供19亿美元，佐治亚州提供26亿美元，而路易斯安那州则为其价值100亿美元的Hyperion数据中心向Meta提供了约33亿美元的税收减免。这笔补贴相当于路易斯安那州逾七年的警方预算，免除了Meta在设备（包括GPU）上长达20年的州和地方销售及使用税。

“好工作第一”组织的Kasia Tarczynska等专家谴责这些是对一个本已蓬勃发展的行业的“浪费性补贴”，并指出真实成本可能更高。亚马逊也获得了数十亿美元的减免，例如在印第安纳州获得了82亿美元。

各州以创造就业和当地投资为由，为这些激励措施辩护；Meta承诺创造5000个建筑工作岗位、500个运营职位，并为当地基础设施投资3亿美元。然而，公众和立法机构的反弹日益强烈。2025年，当地反对派阻止了48个数据中心项目，盖洛普民意调查发现，超过70%的美国人反对在他们社区内建设数据中心。因此，至少有28个州正在考虑修改税收减免政策，9个州正在考虑彻底废除，质疑它们对州预算的真正益处，尤其考虑到许多此类交易缺乏透明度。

---

## 5. 急停并着火

**原文标题**: Halt and Catch Fire

**原文链接**: [https://unstack.io/halt-and-catch-fire](https://unstack.io/halt-and-catch-fire)

本文深入探讨了“Halt and Catch Fire”（HCF，停机并着火）这一短语，这个术语最初是程序员间的幽默，但在计算机历史中却有着实际的影响。HCF描述的是一种机器代码，它会导致CPU停止正常工作，需要系统重置。“着火”这个元素并非完全是比喻；例如，IBM System/360在处理某些无效操作码时，可能因为持续的内存访问而过热。

这个短语最初是工程界的幽默，符合常见的三字母汇编助记符，类似于“Execute Programmer Immediately”（EPI，立即处决程序员）等笑话。然而，HCF在Motorola 6800微处理器上成为了现实。1977年，Gerry Wheeler记录了触发HCF的特定未公开操作码（$9D, $DD）。执行时，6800的程序计数器会无休止地递增，导致地址总线顺序循环遍历内存，同时忽略数据。这种锁定状态对中断无动于衷，只能通过重置来解决。

摩托罗拉工程师后来证实了这种内部的“HACOF”行为，并出人意料地将其保留为一个“愉快的意外”，因为它在产品开发期间被证明对快速RAM扫描很有用。最近的硬件分析也证实了这一行为。

类似的CPU锁定问题也出现在其他处理器中，从非法的6502操作码和臭名昭著的奔腾F00F错误，到通过模糊测试发现的现代x86漏洞。文章总结道，HCF代表了计算机幽默、历史工程怪癖和硬件设计复杂现实的丰富交集。

---

## 6. 我把一台80美元的RK3562安卓平板改造成了Debian Linux工作站。

**原文标题**: I turned a $80 RK3562 Android tablet into a Debian Linux workstation

**原文链接**: [https://github.com/tech4bot/rk3562deb](https://github.com/tech4bot/rk3562deb)

本文档详细介绍了“rkdebian”项目，该项目旨在将一台售价80美元的Doogee U10 (RK3562) 安卓平板电脑改造为一台Debian 12 Bookworm Linux工作站。该解决方案允许从SD卡启动Debian，而无需修改平板电脑的内部存储，通过移除SD卡即可恢复到安卓系统。由于缺乏官方支持，该系统是通过逆向工程实现的。

主要特性包括对10.1英寸显示屏、10点多点触控、Wi-Fi、蓝牙、音频、麦克风、加速度计、手电筒、电源按钮和电池管理的完整支持。对3D加速 (Panfrost OpenGL ES) 和摄像头 (前后摄像头管道功能正常，但需要颜色校准) 提供部分支持。

一项重要成就是，通过瑞芯微的RKLLM堆栈，在RK3562的NPU上实现了对本地LLM推理的活跃支持，基准测试显示Qwen3-0.6B的性能优于Qwen2.5-1.5B。

该Debian镜像预装了Firefox ESR、Chromium、FreeTube、Dolphin和Plasma Discover等应用程序。设备上的用户体验集成包括Phosh电源模式映射、原生手电筒开关、自定义电源按钮行为以及保留锁屏方向。通过将生成的 `update.tar.gz` 文件复制到平板电脑上，即可支持OTA更新。

构建镜像需要一台安装特定依赖项的x86-64架构Linux主机。`build.sh` 脚本支持完整的端到端构建，并提供选项来自定义UI会话 (Phosh)、GPU堆栈 (Mali或Panfrost)、显示服务器、CPU调速器和镜像大小。将压缩镜像刷入SD卡通过 `dd` 命令完成。默认凭据为 `chaos/chaos` 和 `root/root`。SD卡使用带有自动扩展rootfs的GPT分区表。

---

## 7. 伦敦警方首次在抗议活动中部署人脸识别

**原文标题**: London Police Deploy Facial Recognition at Protest for First Time

**原文链接**: [https://reclaimthenet.org/london-police-deploy-facial-recognition-at-protest-for-first-time](https://reclaimthenet.org/london-police-deploy-facial-recognition-at-protest-for-first-time)

本文提出了关于数字控制和隐私的两个既不同又相关的担忧。标题公布了一项重大进展：伦敦警方首次在抗议活动中部署了面部识别技术。

随后的内容则转向一项更广泛的批评，认为“网络正在将人类区分为获准者和未获准者”。文章以谷歌为例，指出该公司在2023年曾请求许可“限制开放网络”，但遭到拒绝，却通过一次产品更新实现了类似的结果，作者称此举未经公众同意。

---

## 8. Fisker went bankrupt and owners built an open source car company from the ashes

**原文标题**: Fisker went bankrupt and owners built an open source car company from the ashes

**原文链接**: [https://electrek.co/2026/05/16/fisker-ocean-open-source-ev-story-after-bankruptcy/](https://electrek.co/2026/05/16/fisker-ocean-open-source-ev-story-after-bankruptcy/)

生成摘要时出错

---

## 9. US is starting to see heavy job losses in roles exposed to AI

**原文标题**: US is starting to see heavy job losses in roles exposed to AI

**原文链接**: [https://www.bloomberg.com/news/articles/2026-05-15/us-is-starting-to-see-heavy-job-losses-in-roles-exposed-to-ai](https://www.bloomberg.com/news/articles/2026-05-15/us-is-starting-to-see-heavy-job-losses-in-roles-exposed-to-ai)

生成摘要时出错

---

## 10. OpenClaw Creator Spent $1.3M on OpenAI Tokens in 30 Days

**原文标题**: OpenClaw Creator Spent $1.3M on OpenAI Tokens in 30 Days

**原文链接**: [https://twitter.com/steipete/status/2055346265869721905](https://twitter.com/steipete/status/2055346265869721905)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 2 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 3 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 4 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 5 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 6 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 7 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 8 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 9 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 10 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 11 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 12 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 13 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 14 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 15 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 16 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 17 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 18 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 19 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 20 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 21 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 22 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 23 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 24 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 25 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 26 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 27 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 28 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 29 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 30 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 31 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 32 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 33 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 34 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 35 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 36 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 37 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 38 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 39 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 40 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 41 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 42 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 43 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 44 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 45 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 46 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 47 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 48 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 49 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 50 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 51 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 52 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 53 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 54 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 55 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 56 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 57 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 58 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 59 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 60 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 61 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 62 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 63 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 64 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 65 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 66 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 67 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 68 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 69 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 70 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 71 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 72 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 73 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 74 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 75 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 76 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 77 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 78 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 79 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 80 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 81 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 82 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 83 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 84 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 85 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 86 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 87 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 88 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 89 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 90 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 91 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 92 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 93 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 94 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 95 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 96 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 97 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 98 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 99 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 100 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 101 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 102 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 103 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 104 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 105 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 106 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 107 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 108 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 109 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 110 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 111 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 112 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 113 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 114 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 115 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 116 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 117 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 118 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 119 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 120 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 121 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 122 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 123 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 124 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 125 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 126 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 127 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 128 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 129 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 130 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 131 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 132 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 133 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 134 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 135 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 136 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 137 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 138 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 139 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 140 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 141 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 142 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 143 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 144 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 145 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 146 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 147 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 148 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 149 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 150 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 151 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 152 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 153 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 154 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 155 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 156 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 157 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 158 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 159 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 160 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 161 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 162 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 163 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 164 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 165 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 166 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 167 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 168 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 169 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 170 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 171 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 172 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 173 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 174 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 175 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 176 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 177 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 178 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 179 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 180 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 181 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 182 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 183 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 184 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 185 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 186 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 187 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 188 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 189 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 190 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 191 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
