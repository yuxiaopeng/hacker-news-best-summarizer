# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-07-04.md)

*最后自动更新时间: 2026-07-04 20:28:59*
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

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 2 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 3 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 4 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 5 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 6 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 7 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 8 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 9 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 10 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 11 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 12 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 13 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 14 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 15 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 16 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 17 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 18 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 19 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 20 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 21 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 22 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 23 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 24 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 25 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 26 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 27 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 28 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 29 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 30 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 31 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 32 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 33 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 34 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 35 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 36 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 37 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 38 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 39 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 40 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 41 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 42 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 43 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 44 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 45 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 46 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 47 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 48 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 49 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 50 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 51 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 52 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 53 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 54 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 55 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 56 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 57 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 58 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 59 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 60 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 61 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 62 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 63 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 64 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 65 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 66 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 67 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 68 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 69 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 70 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 71 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 72 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 73 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 74 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 75 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 76 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 77 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 78 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 79 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 80 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 81 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 82 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 83 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 84 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 85 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 86 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 87 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 88 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 89 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 90 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 91 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 92 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 93 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 94 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 95 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 96 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 97 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 98 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 99 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 100 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 101 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 102 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 103 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 104 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 105 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 106 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 107 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 108 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 109 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 110 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 111 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 112 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 113 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 114 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 115 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 116 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 117 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 118 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 119 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 120 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 121 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 122 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 123 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 124 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 125 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 126 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 127 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 128 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 129 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 130 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 131 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 132 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 133 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 134 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 135 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 136 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 137 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 138 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 139 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 140 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 141 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 142 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 143 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 144 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 145 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 146 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 147 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 148 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 149 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 150 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 151 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 152 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 153 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 154 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 155 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 156 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 157 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 158 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 159 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 160 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 161 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 162 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 163 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 164 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 165 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 166 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 167 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 168 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 169 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 170 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 171 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 172 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 173 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 174 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 175 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 176 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 177 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 178 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 179 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 180 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 181 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 182 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 183 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 184 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 185 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 186 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 187 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 188 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 189 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 190 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 191 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 192 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 193 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 194 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 195 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 196 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 197 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 198 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 199 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 200 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 201 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 202 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 203 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 204 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 205 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 206 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 207 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 208 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 209 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 210 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 211 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 212 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 213 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 214 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 215 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 216 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 217 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 218 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 219 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 220 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 221 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 222 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 223 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 224 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 225 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 226 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 227 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 228 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 229 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 230 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 231 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 232 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 233 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 234 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 235 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 236 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 237 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 238 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 239 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
