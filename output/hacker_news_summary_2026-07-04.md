# Hacker News 热门文章摘要 (2026-07-04)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. Soatok的非正式威胁模型指南

**原文标题**: Soatok's Informal Guide to Threat Models

**原文链接**: [https://soatok.blog/2026/06/30/soatoks-informal-guide-to-threat-models/](https://soatok.blog/2026/06/30/soatoks-informal-guide-to-threat-models/)

Soatok的非正式指南为初学者澄清了“威胁模型”这一术语，该术语常被误用为流行语。它强调，在设计过程中进行正式或非正式的威胁建模，都能显著改善产品成果。一个有用的威胁模型必须回答四个核心问题：我们正在保护什么？谁想对其造成伤害？他们可能如何攻击？以及什么可以阻止这些攻击？

除了这些基础知识，关键细节还包括理解资产关系（以图论思维），明确说明所有假设（因为不正确的假设会损害模型），以及承认那些刻意不予解决的威胁。突出假设有助于识别“未知未知数”，并且威胁模型应该是动态文档。

要开始威胁建模，首先要绘制系统组件及其交互图。然后，从高层视图迭代地深入到特定组件，详细说明输入/输出，并应用核心问题，同时记录对底层所做的假设。

作者展示了他们项目的威胁模型作为有效范例，按假设、资产、行为者和分类风险进行组织。相比之下，Matrix的威胁模型被批评为仅仅是攻击类型列表，缺乏明确的假设、资产关系或加密细节。Signal因没有明确的威胁模型而被认为更糟。

有效的威胁建模使防御者能够主导攻击态势，从而实现真正的深度防御。例如，理解人们为何重复使用密码有助于促使采用通行密钥来防止凭据填充和钓鱼攻击。良好的威胁建模能带来消除攻击向量和提升可用性的设计选择，体现了“以牺牲可用性为代价的安全，是以牺牲安全性为代价的”这一原则。

---

## 2. 美国居民因数据中心被“强塞”而愤怒，正在罢免官员。

**原文标题**: US residents angry datacenters 'shoved down our throats' are recalling officials

**原文链接**: [https://www.theguardian.com/us-news/2026/jul/03/datacenter-recall-elections](https://www.theguardian.com/us-news/2026/jul/03/datacenter-recall-elections)

美国居民对数据中心的激增日益感到愤怒，这导致了广泛的抗议、暂停建设的要求，以及罢免批准这些项目的民选官员的行动。全国各地的社区都觉得数据中心“被强加给我们的”，原因是开发商和地方官员普遍缺乏透明度，通常涉及保密协议（NDA），隐瞒了真正的企业受益方。

这种反对源于对环境和经济影响的重大担忧。数据中心消耗大量水（大型数据中心每天高达500万加仑）和电（相当于数千户家庭的用电量），耗尽当地资源，推高公用事业成本，并造成噪音和空气污染。居民还担心房产价值贬值和潜在的失业，这与经济利益的说法相悖。

这场草根运动促成了共和党和民主党之间罕见的团结。例如，密歇根州莱诺克斯市因被认为存在秘密操作而提交了罢免请愿书；密苏里州费斯图斯市的居民尽管提交了罢免请愿书，仍在通过法律途径挑战市议会批准数据中心的决定；俄克拉荷马州育空市的一位副市长在面临罢免努力后辞职。

尽管一些政客和投资者错误地声称存在外国影响，但专家们发现没有证据表明是中国在推动这种反对。相反，这种抵制是由社区对秘密交易以及这些设施实际负面影响的不满所驱动的，导致全国范围内大量数据中心项目被阻止或延迟。

---

## 3. 环绕地球的暗淡卫星不应超过十万颗。

**原文标题**: No more than 100 000 faint satellites should orbit Earth

**原文链接**: [https://www.eso.org/public/news/eso2607/](https://www.eso.org/public/news/eso2607/)

欧洲南方天文台（ESO）一项新研究显示，目前提议发射的逾170万颗新卫星，包括一些极其明亮的卫星，对夜空观测和天文学构成“严重威胁”。这项由奥利维耶·海诺（Olivier Hainaut）领导的研究建议，将卫星总数限制在不超过10万颗肉眼不可见的暗淡卫星，以保护我们观测宇宙的能力。

目前，地球轨道上有超过1.4万颗卫星，主要来自SpaceX的“星链”计划。然而，SpaceX计划再发射一百万颗用于数据中心，这将导致每晚有数百到数千颗卫星肉眼可见。Reflect Orbital公司提议发射5万颗大型、镜面般的卫星以提供夜间照明，这尤其令人担忧；这些卫星将是迄今为止最亮的，比金星还要亮，一颗卫星发出的光束可能比满月亮四倍。此类卫星群将以明亮的轨迹破坏天文图像，并显著增加夜空的整体亮度，可能使其亮度增加三到四倍。

这些影响将阻碍对暗弱宇宙目标的观测，并可能导致先进望远镜每晚拍摄的大部分图像在数小时内无法使用。ESO与其他天文机构合作，已向美国联邦通信委员会（FCC）提出反对意见，强调这对光学天文学构成“生存威胁”。文章还指出，人们普遍担心光污染对健康、生态系统和大气污染的影响。它敦促国际社会合作，限制未来的发射，并实施严格的缓解措施，为子孙后代保护近地轨道。

---

## 4. 黑客为公司铲雪，获赠网管权限。

**原文标题**: Hackers shoveled snow for company, were rewarded with network admin access

**原文链接**: [https://www.theregister.com/security/2026/07/02/hackers-shoveled-snow-for-company-were-rewarded-with-network-admin-access/5265240](https://www.theregister.com/security/2026/07/02/hackers-shoveled-snow-for-company-were-rewarded-with-network-admin-access/5265240)

专业的红队队员克里斯托弗·约翰逊和迈克尔在达维德·施洛斯的监督下，通过利用物理安全漏洞和人类信任，成功攻破了一家公司的网络。他们冒充新入职的IT员工，在主动提出为维修人员铲雪后获得了进入许可，维修人员随后让约翰逊在没有门禁卡的情况下进入了大楼。

约翰逊在一个未受保护的会议室网络端口植入了一个树莓派，并用垃圾桶将其藏了起来。尽管在另一位置最初被网络访问控制（NAC）阻止，但这个端口缺乏此类保护，使得树莓派保持连接并两周未被发现。

当维修人员感谢IT部门对迈克尔的帮助时，红队队员的真实身份被物理上“抓到”，因为公司中根本没有这些员工。尽管安保人员查看了监控录像，隐藏的树莓派仍未被发现。

在其连接的两周内，红队利用树莓派访问了公司的Active Directory（活动目录）。他们使用“winter2023!”进行密码喷洒攻击，获得了50-60个员工账户的访问权限。随后他们绘制了网络拓扑，枚举了活动目录证书服务（ADCS），并利用ESC1、ESC4和ESC8漏洞，取得了完整的域管理权限。在攻击完成后，一名清洁工在两周后才发现了这个树莓派。

这起事件凸显了重大的安全漏洞：员工缺乏物理安全意识（被称为“滑雪面罩偏见”）、未受保护的网络端口、弱密码策略以及缺乏多因素认证。

---

## 5. 白领士气低落

**原文标题**: The Demoralization of the White-Collar Worker

**原文链接**: [https://nooneshappy.com/article/the-demoralization-of-the-white-collar-worker/](https://nooneshappy.com/article/the-demoralization-of-the-white-collar-worker/)

《白领的士气消沉》概述了专业人士在追求美国梦过程中面临的严峻挑战，导致了普遍的幻灭感。作者的亲身经历便是这种挣扎的典型例证：二十年来，通过严格储蓄，最终却只能通过搬迁到远离其职业和社交网络的乡村小镇才能买得起房。

文章详细阐述了几个系统性问题：
1.  **薪资停滞不前：** 自1979年以来，工人生产力提高了90%，但平均薪酬仅增长了33%。绝大部分流向了高管薪酬、股东回报和企业利润。白领工资持平或下降，公司用更廉价、能力较差的员工取代有经验的员工。
2.  **住房高不可攀：** 自2019年以来，房价飙升了53%，而家庭收入中位数仅增长了24%。首次购房者年龄中位数现已达到40岁，投资者积极抢购住房，将潜在的自住房转化为租赁物业。
3.  **功能失调的医疗体系：** 美国医疗保险系统被描述为一个“榨取系统”，旨在收取高额保费（作者每月700美元）并拒绝赔付。拒绝赔付的决定在申诉后往往被推翻，这表明其以利润为导向而非以患者护理为重，导致治疗延迟和医疗债务。
4.  **退休保障日益削弱：** 从固定福利养老金向401(k)计划的转变，将投资风险转嫁给了个人。退休储蓄中位数低得惊人（32-61岁家庭仅为5000美元），导致许多人对退休毫无准备。
5.  **预算捉襟见肘：** 即使年薪10万美元，在支付住房、医疗保健，尤其是育儿等基本开销后，也所剩无几，育儿费用在全美50个州都可能超过两个孩子的租金。学生贷款债务进一步加剧了这些压力。这并非消费问题，而是固定、非自由支配开支吞噬收入的危机，导致双职工家庭付出更多却回报递减，并导致生育率下降。

这些趋势的累积效应导致了一种“大脱节”，在此背景下，白领的持续努力不再能保证基本财务安全或传统的成功标志。

---

## 6. 赋能智者，成就智慧之举

**原文标题**: Give Smart People the Tools to Do Smart Things

**原文链接**: [https://superuserdone.com/posts/2026-07-03-give-smart-people-the-tools/](https://superuserdone.com/posts/2026-07-03-give-smart-people-the-tools/)

文章《给聪明人做聪明事的工具》批判性地审视了盛行的AI叙事，并将其定性为营销炒作。文章认为，AI取代行业、治愈疾病或淘汰程序员的说法，旨在将AI描绘成凌驾于人类之上，将专家贴上“勒德分子”的标签，并推动高价订阅。

作者认为，AI公司将“工作”简化为可见的“产物”，却忽视了过程中固有的关键人类理解、设计和决策。文章将AI比作编译器、电子表格和CAD系统等工具，强调这些技术增强了专家的能力，使他们更快、更有效，但从未取代其核心知识或判断力。程序员理解软件；会计师识别关键计算；工程师做出战略决策——这些任务在目前AI的设定下无法复制。例如，围绕Anthropic的Mythos进行的“网络武器”营销，贬低了真正的安全研究。

文章指出，这种炒作源于AI公司需要利用投资者对“未来”的渴望，在对当前收入和利润的要求超越投机性承诺之前，获取资本和客户。

作者设想的AI未来是技术补充人类专家，而不是威胁他们。文章引用Unity和Unreal等游戏引擎作为创作者的赋能工具，倡导AI应增强专家能力——例如为医生提供先进的诊断工具——从而大幅提高其效率。对AI高管的最终请求是，开发能够赋能聪明人做聪明事的工具，而不是宣扬取代人类的恐惧。

---

## 7. 我没有禁止AI，而是和学生们制定了课堂公约。

**原文标题**: Instead of banning AI, I made a classroom contract with my students

**原文链接**: [https://www.science.org/content/article/instead-banning-ai-i-made-classroom-contract-my-students](https://www.science.org/content/article/instead-banning-ai-i-made-classroom-contract-my-students)

高中英语老师Nicole Schrad反对禁止ChatGPT等AI工具，认为它是一种不可避免的技术，学生必须学会负责任地使用。她没有禁止AI，而是与学生合作制定了一份AI使用“课堂契约”。

经过多天的讨论，学生们就如何将AI整合到他们的学习工作中进行了讨论和投票，制定了规则。他们契约的关键原则包括：绝对透明，要求学生披露所有AI使用；保持原创性，确保AI不会生成完整的草稿或模仿他们独特的文风；以及批判性评估，教导学生识别AI的局限性、偏见和不准确之处。

该契约将AI定位为头脑风暴、研究辅助或克服写作障碍的辅助工具，而不是原创思维的替代品。这种方法赋予学生权力，培养了他们在数字素养、伦理推理和批判性思维方面的基本技能，这些技能对未来的学业和职业成功至关重要。Schrad的方法优先教导学生负责任地利用AI来提升学习，而不是剥夺他们接触这项变革性技术的机会。

---

## 8. Best Simple System for Now (2025)

**原文标题**: Best Simple System for Now (2025)

**原文链接**: [https://dannorth.net/blog/best-simple-system-for-now/](https://dannorth.net/blog/best-simple-system-for-now/)

生成摘要时出错

---

## 9. The circuit that lets your brain think and see

**原文标题**: The circuit that lets your brain think and see

**原文链接**: [https://www.engineering.columbia.edu/about/news/circuit-lets-your-brain-think-and-see](https://www.engineering.columbia.edu/about/news/circuit-lets-your-brain-think-and-see)

生成摘要时出错

---

## 10. Lightning Memory-Mapped Database Manager (LMDB) 1.0

**原文标题**: Lightning Memory-Mapped Database Manager (LMDB) 1.0

**原文链接**: [http://www.lmdb.tech/doc/](http://www.lmdb.tech/doc/)

生成摘要时出错

---

## 11. Faster embeddings: how we rebuilt the ONNX path in Manticore

**原文标题**: Faster embeddings: how we rebuilt the ONNX path in Manticore

**原文链接**: [https://manticoresearch.com/blog/onnx-embeddings-speedup/](https://manticoresearch.com/blog/onnx-embeddings-speedup/)

生成摘要时出错

---

## 12. AI saves about 3% of your hours, and almost none of it reaches the money

**原文标题**: AI saves about 3% of your hours, and almost none of it reaches the money

**原文链接**: [https://okaneland.com/study/ai-productivity-roi-at-work/](https://okaneland.com/study/ai-productivity-roi-at-work/)

生成摘要时出错

---

## 13. Commodore 64 Basic for PostgreSQL

**原文标题**: Commodore 64 Basic for PostgreSQL

**原文链接**: [https://thombrown.blogspot.com/2026/07/load-plcbmbasic81-commodore-64-basic.html](https://thombrown.blogspot.com/2026/07/load-plcbmbasic81-commodore-64-basic.html)

生成摘要时出错

---

## 14. Verizon is About to Break our Watches

**原文标题**: Verizon is About to Break our Watches

**原文链接**: [https://www.jefftk.com/p/verizon-is-about-to-break-our-watches](https://www.jefftk.com/p/verizon-is-about-to-break-our-watches)

生成摘要时出错

---

## 15. Rust Coreutils cp Ended Up Breaking Ubuntu Image Builds with Incompatibility

**原文标题**: Rust Coreutils cp Ended Up Breaking Ubuntu Image Builds with Incompatibility

**原文链接**: [https://www.phoronix.com/news/Rust-Coreutils-cp-Ubuntu-Images](https://www.phoronix.com/news/Rust-Coreutils-cp-Ubuntu-Images)

生成摘要时出错

---

## 16. Open Source Touhou Clone

**原文标题**: Open Source Touhou Clone

**原文链接**: [https://taisei-project.org/](https://taisei-project.org/)

生成摘要时出错

---

## 17. 'guix substitute' and 'guix pull' Vulnerabilities

**原文标题**: 'guix substitute' and 'guix pull' Vulnerabilities

**原文链接**: [https://guix.gnu.org/en/blog/2026/guix-substitute-pull-vulnerabilities/](https://guix.gnu.org/en/blog/2026/guix-substitute-pull-vulnerabilities/)

生成摘要时出错

---

## 18. Kagi Changelog (July 2): Heads, tails, and an AI toggle

**原文标题**: Kagi Changelog (July 2): Heads, tails, and an AI toggle

**原文链接**: [https://kagi.com/changelog#10959](https://kagi.com/changelog#10959)

生成摘要时出错

---

## 19. A Road to Common Lisp (2018)

**原文标题**: A Road to Common Lisp (2018)

**原文链接**: [https://stevelosh.com/blog/2018/08/a-road-to-common-lisp/](https://stevelosh.com/blog/2018/08/a-road-to-common-lisp/)

生成摘要时出错

---

## 20. GitFut – Your GitHub stats turned into a World-Cup-style player card

**原文标题**: GitFut – Your GitHub stats turned into a World-Cup-style player card

**原文链接**: [https://gitfut.com](https://gitfut.com)

生成摘要时出错

---

## 21. Gemini Code Assist will be shut down on July 17

**原文标题**: Gemini Code Assist will be shut down on July 17

**原文链接**: [https://docs.cloud.google.com/gemini/docs/code-review/review-repo-code](https://docs.cloud.google.com/gemini/docs/code-review/review-repo-code)

生成摘要时出错

---

## 22. Finland's last analogue landline phones go silent after 150 years

**原文标题**: Finland's last analogue landline phones go silent after 150 years

**原文链接**: [https://www.euronews.com/next/2026/06/30/finlands-last-analogue-landline-phones-go-silent-after-150-years](https://www.euronews.com/next/2026/06/30/finlands-last-analogue-landline-phones-go-silent-after-150-years)

生成摘要时出错

---

## 23. Show HN: Mcpsnoop – Wireshark for MCP (transparent proxy and live TUI)

**原文标题**: Show HN: Mcpsnoop – Wireshark for MCP (transparent proxy and live TUI)

**原文链接**: [https://github.com/kerlenton/mcpsnoop](https://github.com/kerlenton/mcpsnoop)

生成摘要时出错

---

## 24. Gun Mistakes in Fiction Writing: Handgun Edition

**原文标题**: Gun Mistakes in Fiction Writing: Handgun Edition

**原文链接**: [https://www.swiftsilentdeadly.com/blog/gun-mistakes-in-fiction-writing-handgun-edition](https://www.swiftsilentdeadly.com/blog/gun-mistakes-in-fiction-writing-handgun-edition)

生成摘要时出错

---

## 25. Windows CE Dreamcast Community Edition (wince-dc)

**原文标题**: Windows CE Dreamcast Community Edition (wince-dc)

**原文链接**: [https://github.com/maximqaxd/wince-dc](https://github.com/maximqaxd/wince-dc)

生成摘要时出错

---

## 26. The Intercept lost control of its Signal-based tip line for months

**原文标题**: The Intercept lost control of its Signal-based tip line for months

**原文链接**: [https://twitter.com/ryangrim/status/2072761908231585845](https://twitter.com/ryangrim/status/2072761908231585845)

生成摘要时出错

---

## 27. What does privatization of the US Postal Service mean?

**原文标题**: What does privatization of the US Postal Service mean?

**原文链接**: [https://phenomenalworld.org/analysis/unstitching-america/](https://phenomenalworld.org/analysis/unstitching-america/)

生成摘要时出错

---

## 28. AI Data Centers Use More Water Than Most Tech Giants Report

**原文标题**: AI Data Centers Use More Water Than Most Tech Giants Report

**原文链接**: [https://www.wsj.com/tech/ai/ai-data-centers-water-use-901e2902](https://www.wsj.com/tech/ai/ai-data-centers-water-use-901e2902)

生成摘要时出错

---

## 29. As downtown Seattle offices empty, city facing years of 'zombie' towers

**原文标题**: As downtown Seattle offices empty, city facing years of 'zombie' towers

**原文链接**: [https://www.seattletimes.com/business/local-business/as-downtown-seattle-offices-empty-city-facing-years-of-zombie-towers/](https://www.seattletimes.com/business/local-business/as-downtown-seattle-offices-empty-city-facing-years-of-zombie-towers/)

生成摘要时出错

---

## 30. Simple, beautiful Emacs modeline: modusregel

**原文标题**: Simple, beautiful Emacs modeline: modusregel

**原文链接**: [https://codeberg.org/jjba23/modusregel](https://codeberg.org/jjba23/modusregel)

生成摘要时出错

---

## 31. 2026 Unslop AI-Written Fiction Contest Results

**原文标题**: 2026 Unslop AI-Written Fiction Contest Results

**原文链接**: [https://www.hyperstitionai.com/unslop-results](https://www.hyperstitionai.com/unslop-results)

生成摘要时出错

---

## 32. It Still Can't Do My Job: Four Years of Moving Goalposts (2022–2026)

**原文标题**: It Still Can't Do My Job: Four Years of Moving Goalposts (2022–2026)

**原文链接**: [https://publicznyprofil.github.io/ai_cant_do_your_work/](https://publicznyprofil.github.io/ai_cant_do_your_work/)

生成摘要时出错

---

## 33. The Common Lisp Cookbook – LispWorks Review

**原文标题**: The Common Lisp Cookbook – LispWorks Review

**原文链接**: [https://lispcookbook.github.io/cl-cookbook/lispworks.html](https://lispcookbook.github.io/cl-cookbook/lispworks.html)

生成摘要时出错

---

## 34. Program-as-Weights: A Programming Paradigm for Fuzzy Functions

**原文标题**: Program-as-Weights: A Programming Paradigm for Fuzzy Functions

**原文链接**: [https://arxiv.org/abs/2607.02512](https://arxiv.org/abs/2607.02512)

生成摘要时出错

---

## 35. Zuckerberg says AI agent development going slower than expected

**原文标题**: Zuckerberg says AI agent development going slower than expected

**原文链接**: [https://www.reuters.com/business/zuckerberg-says-ai-agent-development-going-slower-than-expected-2026-07-02/](https://www.reuters.com/business/zuckerberg-says-ai-agent-development-going-slower-than-expected-2026-07-02/)

生成摘要时出错

---

## 36. Goodbye, Forever, Probably

**原文标题**: Goodbye, Forever, Probably

**原文链接**: [https://whitep4nth3r.com/blog/goodbye-forever-probably/](https://whitep4nth3r.com/blog/goodbye-forever-probably/)

生成摘要时出错

---

## 37. Ed Zitron on CNBC: GenAI Doesn't Work, and Big Tech Is Out of Hypergrowth Ideas

**原文标题**: Ed Zitron on CNBC: GenAI Doesn't Work, and Big Tech Is Out of Hypergrowth Ideas

**原文链接**: [https://www.youtube.com/watch?v=TtmPccUTDP8](https://www.youtube.com/watch?v=TtmPccUTDP8)

生成摘要时出错

---

## 38. Wireless LAN SD

**原文标题**: Wireless LAN SD

**原文链接**: [https://www.sdcard.org/developers/sd-standard-overview/sdio-isdio/wireless-lan-sd/](https://www.sdcard.org/developers/sd-standard-overview/sdio-isdio/wireless-lan-sd/)

生成摘要时出错

---

## 39. Rob Pike – 'Concurrency Is Not Parallelism' [video] (2012)

**原文标题**: Rob Pike – 'Concurrency Is Not Parallelism' [video] (2012)

**原文链接**: [https://vimeo.com/49718712](https://vimeo.com/49718712)

生成摘要时出错

---

## 40. How working memory could give rise to consciousness

**原文标题**: How working memory could give rise to consciousness

**原文链接**: [https://www.scientificamerican.com/article/how-working-memory-could-give-rise-to-consciousness/](https://www.scientificamerican.com/article/how-working-memory-could-give-rise-to-consciousness/)

生成摘要时出错

---

## 41. The Fediverse Is Not the Way Forward

**原文标题**: The Fediverse Is Not the Way Forward

**原文链接**: [https://trialandfailure.net/the-fediverse-is-not-the-way-forward/](https://trialandfailure.net/the-fediverse-is-not-the-way-forward/)

生成摘要时出错

---

## 42. AI coding is addictive. Engineers are paying the price

**原文标题**: AI coding is addictive. Engineers are paying the price

**原文链接**: [https://leaddev.com/ai/ai-coding-is-addictive-engineers-are-paying-the-price](https://leaddev.com/ai/ai-coding-is-addictive-engineers-are-paying-the-price)

生成摘要时出错

---

## 43. Clojure 1.13 adds support for checked keys

**原文标题**: Clojure 1.13 adds support for checked keys

**原文链接**: [https://clojure.org/news/2026/07/02/clojure-1-13-alpha1](https://clojure.org/news/2026/07/02/clojure-1-13-alpha1)

生成摘要时出错

---

## 44. Magit 4.6 Released

**原文标题**: Magit 4.6 Released

**原文链接**: [https://emacsair.me/2026/07/01/magit-4.6/](https://emacsair.me/2026/07/01/magit-4.6/)

生成摘要时出错

---

## 45. FBI Seizes NetNut Proxy Platform, Popa Botnet

**原文标题**: FBI Seizes NetNut Proxy Platform, Popa Botnet

**原文链接**: [https://krebsonsecurity.com/2026/07/fbi-seizes-netnut-proxy-platform-popa-botnet/](https://krebsonsecurity.com/2026/07/fbi-seizes-netnut-proxy-platform-popa-botnet/)

生成摘要时出错

---

## 46. Dispersion loss counteracts embedding condensation in small language models

**原文标题**: Dispersion loss counteracts embedding condensation in small language models

**原文链接**: [https://chenliu-1996.github.io/projects/LM-Dispersion/](https://chenliu-1996.github.io/projects/LM-Dispersion/)

生成摘要时出错

---

## 47. AI is 'not smart' so what's next in artificial intelligence?

**原文标题**: AI is 'not smart' so what's next in artificial intelligence?

**原文链接**: [https://www.bbc.com/news/articles/cj6gr0xkyr3o](https://www.bbc.com/news/articles/cj6gr0xkyr3o)

生成摘要时出错

---

## 48. Pet projects are getting too big to pet

**原文标题**: Pet projects are getting too big to pet

**原文链接**: [https://www.nnehdi.me/p/pet-projects-are-getting-too-big](https://www.nnehdi.me/p/pet-projects-are-getting-too-big)

生成摘要时出错

---

## 49. Olive – Lisp VSCode Extension (Alternative to Alive)

**原文标题**: Olive – Lisp VSCode Extension (Alternative to Alive)

**原文链接**: [https://github.com/kchanqvq/olive](https://github.com/kchanqvq/olive)

生成摘要时出错

---

## 50. Plein Air

**原文标题**: Plein Air

**原文链接**: [https://art.joonas.wtf/](https://art.joonas.wtf/)

生成摘要时出错

---

## 51. A martian rock has lots of carbon on it, and it's not clear why

**原文标题**: A martian rock has lots of carbon on it, and it's not clear why

**原文链接**: [https://arstechnica.com/science/2026/07/a-martian-rock-has-lots-of-carbon-on-it-and-its-not-clear-why/](https://arstechnica.com/science/2026/07/a-martian-rock-has-lots-of-carbon-on-it-and-its-not-clear-why/)

生成摘要时出错

---

## 52. California votes to ruin 3D printing right after voting to keep killing games [video]

**原文标题**: California votes to ruin 3D printing right after voting to keep killing games [video]

**原文链接**: [https://www.youtube.com/watch?v=_GIigWnNRVg](https://www.youtube.com/watch?v=_GIigWnNRVg)

生成摘要时出错

---

## 53. A New Catalog of Stellar Rotation Periods for over a Million Stars

**原文标题**: A New Catalog of Stellar Rotation Periods for over a Million Stars

**原文链接**: [https://aasnova.org/2026/07/01/a-new-catalog-of-stellar-rotation-periods-for-over-a-million-stars/](https://aasnova.org/2026/07/01/a-new-catalog-of-stellar-rotation-periods-for-over-a-million-stars/)

生成摘要时出错

---

## 54. The Reports of Jim Carrey's Death Are a Failure Mode

**原文标题**: The Reports of Jim Carrey's Death Are a Failure Mode

**原文链接**: [https://tane.dev/2026/07/the-reports-of-jim-carreys-death-are-a-failure-mode/](https://tane.dev/2026/07/the-reports-of-jim-carreys-death-are-a-failure-mode/)

生成摘要时出错

---

## 55. This Month in Ladybird: June 2026

**原文标题**: This Month in Ladybird: June 2026

**原文链接**: [https://ladybird.org/newsletter/2026-06-30/](https://ladybird.org/newsletter/2026-06-30/)

生成摘要时出错

---

## 56. Amazon has enough satellites to launch its Starlink competitor

**原文标题**: Amazon has enough satellites to launch its Starlink competitor

**原文链接**: [https://www.theverge.com/science/960563/amazon-leo-service-tipping-point](https://www.theverge.com/science/960563/amazon-leo-service-tipping-point)

生成摘要时出错

---

## 57. Command and Conquer Generals natively ported to macOS, iPhone, iPad using Fable

**原文标题**: Command and Conquer Generals natively ported to macOS, iPhone, iPad using Fable

**原文链接**: [https://github.com/ammaarreshi/Generals-Mac-iOS-iPad/tree/main](https://github.com/ammaarreshi/Generals-Mac-iOS-iPad/tree/main)

生成摘要时出错

---

## 58. BareMetal RAM Dumper – Bare-metal x86 tool for Cold Boot Attack experiments

**原文标题**: BareMetal RAM Dumper – Bare-metal x86 tool for Cold Boot Attack experiments

**原文链接**: [https://github.com/pIat0n/BareMetal-RAM-Dumper](https://github.com/pIat0n/BareMetal-RAM-Dumper)

生成摘要时出错

---

## 59. Sick leave: Germany rising but not the worst in Europe

**原文标题**: Sick leave: Germany rising but not the worst in Europe

**原文链接**: [https://www.dw.com/en/sick-leave-germany-rising-but-not-the-worst-in-europe/a-77815488](https://www.dw.com/en/sick-leave-germany-rising-but-not-the-worst-in-europe/a-77815488)

生成摘要时出错

---

