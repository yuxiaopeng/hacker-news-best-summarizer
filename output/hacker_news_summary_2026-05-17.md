# Hacker News 热门文章摘要 (2026-05-17)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

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

## 11. Technofascism

**原文标题**: Technofascism

**原文链接**: [https://third-bit.com/2026/05/15/technofascism/](https://third-bit.com/2026/05/15/technofascism/)

生成摘要时出错

---

## 12. Ten Signs of Fascism. America has all of them

**原文标题**: Ten Signs of Fascism. America has all of them

**原文链接**: [https://rutgerbregman.substack.com/p/10-signs-of-fascism-america-has-all](https://rutgerbregman.substack.com/p/10-signs-of-fascism-america-has-all)

生成摘要时出错

---

## 13. Greek Alphabet Cards

**原文标题**: Greek Alphabet Cards

**原文链接**: [https://labs.randomquark.com/alphabet_cards/](https://labs.randomquark.com/alphabet_cards/)

生成摘要时出错

---

## 14. WinCE64 – Windows CE 2.11 for N64

**原文标题**: WinCE64 – Windows CE 2.11 for N64

**原文链接**: [https://github.com/ThroatyMumbo/WinCE64](https://github.com/ThroatyMumbo/WinCE64)

生成摘要时出错

---

## 15. Meta deletes popular 1M follower account after Kuwaiti request

**原文标题**: Meta deletes popular 1M follower account after Kuwaiti request

**原文链接**: [https://twitter.com/ryangrim/status/2055992439031185782](https://twitter.com/ryangrim/status/2055992439031185782)

生成摘要时出错

---

## 16. Kioxia and Dell cram 10 PB into slim 2RU server

**原文标题**: Kioxia and Dell cram 10 PB into slim 2RU server

**原文链接**: [https://www.blocksandfiles.com/flash/2026/05/14/kioxia-and-dell-cram-10-pb-into-slim-2ru-server/5240574](https://www.blocksandfiles.com/flash/2026/05/14/kioxia-and-dell-cram-10-pb-into-slim-2ru-server/5240574)

生成摘要时出错

---

## 17. PART Telescopes – Bringing radio astronomy within reach of rural schools

**原文标题**: PART Telescopes – Bringing radio astronomy within reach of rural schools

**原文链接**: [https://mag.openrockets.com/p/how-an-australian-teen-team-is-making-radio-astronomy-affordable-for-rural-schools-4894opuisyhfdisubgi/?b=2](https://mag.openrockets.com/p/how-an-australian-teen-team-is-making-radio-astronomy-affordable-for-rural-schools-4894opuisyhfdisubgi/?b=2)

生成摘要时出错

---

## 18. MCP Hello Page

**原文标题**: MCP Hello Page

**原文链接**: [https://www.hybridlogic.co.uk/blog/2026/05/mcp-hello-page](https://www.hybridlogic.co.uk/blog/2026/05/mcp-hello-page)

生成摘要时出错

---

## 19. Europe built sovereign clouds to escape US control. Forgot about the processors

**原文标题**: Europe built sovereign clouds to escape US control. Forgot about the processors

**原文链接**: [https://www.theregister.com/systems/2026/05/16/europe-built-sovereign-clouds-to-escape-us-control-then-forgot-about-the-processors/5237735](https://www.theregister.com/systems/2026/05/16/europe-built-sovereign-clouds-to-escape-us-control-then-forgot-about-the-processors/5237735)

生成摘要时出错

---

## 20. NYT and vaping: How to lie by saying only true things (2022)

**原文标题**: NYT and vaping: How to lie by saying only true things (2022)

**原文链接**: [https://gwern.net/vaping](https://gwern.net/vaping)

生成摘要时出错

---

## 21. EU weighs restricting use of US cloud platforms to process government data

**原文标题**: EU weighs restricting use of US cloud platforms to process government data

**原文链接**: [https://www.osnews.com/story/144943/eu-weighs-restricting-use-of-us-cloud-platforms-to-process-sensitive-government-data/](https://www.osnews.com/story/144943/eu-weighs-restricting-use-of-us-cloud-platforms-to-process-sensitive-government-data/)

生成摘要时出错

---

## 22. Futhark by example (2020)

**原文标题**: Futhark by example (2020)

**原文链接**: [https://futhark-lang.org/examples.html](https://futhark-lang.org/examples.html)

生成摘要时出错

---

## 23. Judge bars Kars4Kids from broadcasting 'misleading' ads in California

**原文标题**: Judge bars Kars4Kids from broadcasting 'misleading' ads in California

**原文链接**: [https://www.nytimes.com/2026/05/15/us/kars4kids-advertising-banned-california.html](https://www.nytimes.com/2026/05/15/us/kars4kids-advertising-banned-california.html)

生成摘要时出错

---

## 24. Japan’s robot wolf sells out as record bear attacks drive demand

**原文标题**: Japan’s robot wolf sells out as record bear attacks drive demand

**原文链接**: [https://www.independent.co.uk/asia/japan/japan-robot-wolf-bear-attacks-ohta-seiki-b2975670.html](https://www.independent.co.uk/asia/japan/japan-robot-wolf-bear-attacks-ohta-seiki-b2975670.html)

生成摘要时出错

---

## 25. Show HN: Rocksky – Music scrobbling and discovery on the AT Protocol

**原文标题**: Show HN: Rocksky – Music scrobbling and discovery on the AT Protocol

**原文链接**: [https://tangled.org/rocksky.app/rocksky](https://tangled.org/rocksky.app/rocksky)

生成摘要时出错

---

## 26. A Meta employee gets real about the horror of working there

**原文标题**: A Meta employee gets real about the horror of working there

**原文链接**: [https://sfstandard.com/pacific-standard-time/2026/05/15/meta-employee-gets-real-horror-working-right-now/](https://sfstandard.com/pacific-standard-time/2026/05/15/meta-employee-gets-real-horror-working-right-now/)

生成摘要时出错

---

## 27. My Favorite Bugs: Invalid Surrogate Pairs

**原文标题**: My Favorite Bugs: Invalid Surrogate Pairs

**原文链接**: [https://george.mand.is/2026/05/my-favorite-bugs-invalid-surrogate-pairs/](https://george.mand.is/2026/05/my-favorite-bugs-invalid-surrogate-pairs/)

生成摘要时出错

---

## 28. Playing Atari ST Music on the Amiga with Zero CPU

**原文标题**: Playing Atari ST Music on the Amiga with Zero CPU

**原文链接**: [https://arnaud-carre.github.io/2026-05-15-ym-fast-emu/](https://arnaud-carre.github.io/2026-05-15-ym-fast-emu/)

生成摘要时出错

---

## 29. Self-Distillation Enables Continual Learning [pdf]

**原文标题**: Self-Distillation Enables Continual Learning [pdf]

**原文链接**: [https://arxiv.org/abs/2601.19897](https://arxiv.org/abs/2601.19897)

生成摘要时出错

---

## 30. Tesla Solar Roof is on life support as it pivot to panels

**原文标题**: Tesla Solar Roof is on life support as it pivot to panels

**原文链接**: [https://electrek.co/2026/05/14/tesla-solar-roof-promise-vs-reality-pivot-panels/](https://electrek.co/2026/05/14/tesla-solar-roof-promise-vs-reality-pivot-panels/)

生成摘要时出错

---

