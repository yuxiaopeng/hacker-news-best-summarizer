# Hacker News 热门文章摘要 (2026-05-08)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. ZFS、iSCSI 和 PXE 无盘 Linux 启动

**原文标题**: Diskless Linux boot using ZFS, iSCSI and PXE

**原文链接**: [https://aniket.foo/posts/20260505-netboot/](https://aniket.foo/posts/20260505-netboot/)

本文详细介绍了如何使用ZFS、iSCSI和PXE设置无盘Linux启动环境。作者的动机是创建一个隔离的Linux系统进行AI模型测试，同时不干扰现有的Windows游戏安装，避免GRUB、本地磁盘分区或U盘易丢失等问题，并借此机会学习通过iSCSI实现PXE启动。

该设置利用一台中央Debian 13服务器（Proxmox主机）作为PXE启动服务器、TFTP服务器、iSCSI目标和ZFS主机。路由器上的DNSMasq负责将客户端的启动请求指向该服务器。

该过程涉及以下几个关键步骤：
1.  **Netboot.xyz配置：** 安装Netboot.xyz，自定义其模板和一个特定的菜单条目（`debian13-iscsi.ipxe`）。该条目配置了iSCSI服务器、目标、发起方IQN和相互CHAP认证的详细信息，尝试`sanboot`（从iSCSI启动），或在失败时回退到基于网络的Debian安装程序。
2.  **TFTP和DNSMasq：** 配置`tftpd-hpa`以提供iPXE二进制文件，并在路由器上设置DNSMasq，将不同客户端架构（BIOS/UEFI/iPXE）的请求导向正确的网络启动文件。
3.  **ZFS ZVol和iSCSI目标：** 在Proxmox主机上创建一个ZFS ZVol（`tank/debian-disk-12700k`）。然后使用`targetcli`将此ZVol作为iSCSI块设备导出，并配置iSCSI目标、客户端IQN的ACL（访问控制列表）以及相互CHAP认证。
4.  **Debian安装：** 客户端PC通过PXE启动，选择自定义的iSCSI启动选项。如果未找到操作系统，它将进入Debian网络安装程序。在安装程序的磁盘检测阶段，用户切换到TTY手动配置iSCSI发起方的IQN（`/etc/iscsi/initiatorname.iscsi`），重启`iscsid`，然后使用定义的凭据登录iSCSI目标。最后，Debian被安装到远程提供的iSCSI卷上，从而创建了一个持久化的无盘Linux系统。

---

## 2. 戴维·阿滕伯勒的100岁生日

**原文标题**: David Attenborough's 100th Birthday

**原文链接**: [https://www.bbc.com/news/articles/cp3pww9g0p5o](https://www.bbc.com/news/articles/cp3pww9g0p5o)

戴维·阿滕伯勒爵士的百岁生日正通过一波又一波的致敬活动来庆祝，由查尔斯三世国王和卡米拉王后带头，他们分享了私人照片并表达了对他的美好祝愿。威廉王子赞扬了阿滕伯勒持续的启发作用，而哈里王子则因他对气候意识的影响称他为“世俗圣人”。包括大卫·贝克汉姆、乔安娜·拉姆利、克里斯·帕卡姆、朱迪·丹奇女爵士、摩根·弗里曼、汉斯·季默和伊恩·麦克莱恩爵士在内的名人也分享了真挚的祝福，赞扬他对自然历史的独特贡献以及吸引观众的能力。

阿滕伯勒表示对如潮般的爱意感到“完全受宠若惊”。庆祝活动的高潮是在皇家阿尔伯特音乐厅举行的一场由柯斯蒂·杨主持的特别音乐会。该活动将邀请迈克尔·佩林爵士等嘉宾回顾他的一生和遗产，由BBC音乐会管弦乐团现场演奏音乐，重现标志性电视时刻，并有丹·史密斯（巴士底乐队）和席格洛斯等艺术家的表演。

BBC也以一周的特别节目来纪念这一百年诞辰，其中包括经典纪录片和新剧集。为了进一步纪念他的遗产，自然历史博物馆将一种新发现的寄生蜂命名为*Attenboroughnculus tau*，以他的名字命名，此前已有其他几种物种以他命名。戴维爵士生于1926年，于1952年加入BBC，开创了众多具有里程碑意义的自然历史系列节目。

---

## 3. 特斯拉召回其较便宜的Cybertruck，原因是车轮可能脱落。

**原文标题**: Tesla is recalling its cheaper Cybertruck because the wheels might fall off

**原文链接**: [https://www.theverge.com/transportation/926741/tesla-cybertruck-cheaper-recall](https://www.theverge.com/transportation/926741/tesla-cybertruck-cheaper-recall)

特斯拉正在召回全部173辆后驱版Cybertruck长续航车型，特指售价7万美元、配备18英寸钢轮的型号，原因是一个关键安全问题。据Emma Roth于2026年5月8日报道，此次召回源于有缺陷的刹车盘，其螺栓孔可能会开裂，可能导致车轮脱落，尤其是在剧烈驾驶条件下。

这是Cybertruck的第11次召回，此前曾因加速踏板、内饰和摄像头问题而被召回。尽管特斯拉已确认了三起与此问题相关的保修索赔，但该公司尚未报告任何碰撞、死亡或受伤事件。

受影响的车型是去年4月推出并在数月后停产的后驱版Cybertruck。今年2月发布的售价6万美元的新款双电机全驱版Cybertruck不在此次召回范围内。特斯拉将通过免费更换受影响车辆上的前后刹车盘、轮毂和车轮螺母来解决此问题。

---

## 4. 非营利医院斥资数十亿聘请顾问，收效甚微。

**原文标题**: Nonprofit hospitals spend billions on consultants with no clear effect

**原文链接**: [https://www.uchicagomedicine.org/forefront/research-and-discoveries-articles/nonprofit-hospitals-spend-billions-on-management-consultants](https://www.uchicagomedicine.org/forefront/research-and-discoveries-articles/nonprofit-hospitals-spend-billions-on-management-consultants)

《美国医学会杂志》发表的一项新研究显示，非营利医院在管理咨询顾问上花费了数十亿美元，但没有明确证据表明其产生了积极影响。这项由约瑟夫·多夫·布鲁赫博士牵头的首次大规模实证分析，审查了2010年至2022年间的美国国税局990表申报文件，对比了306家聘请了咨询顾问的医院和一个匹配的对照组。

在研究期间，超过20%的非营利医院聘请了管理咨询顾问，用于这些服务的支出至少达78亿美元，平均每家医院1570万美元。如果包括人力资源和IT等其他类型的咨询顾问，总支出则超过250亿美元。

尽管投入了巨额资金，但研究发现，在患者净收入、运营利润、人员配置、运营或患者结果（如再入院率和死亡率）等关键指标方面，均未出现统计学上显著或系统性的改善。布鲁赫指出，咨询顾问带来的结果是“既没有他们承诺的显著效率，也没有批评者有时担心的危害”，并总结称，没有证据表明存在“有意义的改善”。唯一观察到的例外是一个轻微的负面影响：中风再入院率略有上升。

作者建议医院高管应更加谨慎，并呼吁提高税收补贴资金使用方式的透明度和公共问责制。这项研究还旨在为考虑从事医疗管理咨询职业的学生提供信息，提供关于此类角色实际影响的急需证据。

---

## 5. GPT-5.5 涨价：费用详情

**原文标题**: GPT-5.5 Price Increase: What It Costs

**原文链接**: [https://openrouter.ai/announcements/gpt55-cost-analysis](https://openrouter.ai/announcements/gpt55-cost-analysis)

OpenRouter最近的一项分析揭示了OpenAI GPT-5.5的实际成本影响，该版本推出时比GPT-5.4价格上涨了2倍。输入token从每百万2.50美元增加到每百万5.00美元，输出token从每百万15美元增加到每百万30美元。

这项研究基于从GPT-5.4过渡到GPT-5.5的“转换用户群”，发现用户的实际成本增加了49%到92%。

一个关键发现是，GPT-5.5所宣称的减少冗余只对较长的提示词有益。对于超过10K token的提示词，模型生成的补全token减少了19-34%。这种缓解措施部分抵消了价格上涨，使得这些较长提示词的成本增加幅度为49-62%（例如，50K-128K token的提示词成本增加了49%）。

相反，较短的提示词经历了更高的净成本影响。对于2K token以下的提示词，补全内容反而长了7%，导致成本增加了92%。对于2K-10K token之间的提示词，补全内容长了52%，导致成本增加了69%，因为缩短补全内容的益处并未体现。

该方法涉及分析OpenRouter请求日志中的计费成本，并将成本标准化为每百万OpenRouter token的平均成本，以便直接比较。

---

## 6. 梵蒂冈拉丁语网站

**原文标题**: The Vatican's Website in Latin

**原文链接**: [https://www.vatican.va/latin/latin_index.html](https://www.vatican.va/latin/latin_index.html)

这篇题为“梵蒂冈的拉丁语网站”的文章，强调了圣座官方网站上拉丁语内容的存在。所提供的文本“Documenta Lingua Latina exarata”直接翻译为“用拉丁语写的文件”。这表明梵蒂冈的数字平台包含一个专门的板块，提供各种拉丁语材料，可能包括官方声明、历史文献或神学著作。这强调了梵蒂冈持续致力于将拉丁语作为其交流和档案的重要语言。

---

## 7. Cartoon Network Flash Games

**原文标题**: Cartoon Network Flash Games

**原文链接**: [https://www.webdesignmuseum.org/flash-game-exhibitions/cartoon-network-flash-games](https://www.webdesignmuseum.org/flash-game-exhibitions/cartoon-network-flash-games)

生成摘要时出错

---

## 8. 自动取消订阅

**原文标题**: The Self-Cancelling Subscription

**原文链接**: [https://predr.ag/blog/the-self-cancelling-subscription/](https://predr.ag/blog/the-self-cancelling-subscription/)

The author details a frustrating experience with a "self-cancelling" streaming subscription, a perk linked to their credit card. The service repeatedly deactivated itself approximately five minutes after being reactivated. Initial attempts to fix it, including updating credit card information and toggling the perk on the bank's website, only provided temporary relief before the subscription cancelled again.

Calls to both the credit card and streaming service support teams proved fruitless, with each side claiming "no issues on our end" and blaming the other. After a night of "black-box debugging," the author's "aha!" moment led to unlinking the accounts from the bank's website, waiting overnight, and then re-linking them. This successfully resolved the issue.

The author's theory for the problem is a sync-vs-async race condition. Linking the subscription was a synchronous process, granting immediate access. However, unlinking was asynchronous, taking a few minutes to propagate. When the author rapidly re-linked after a cancellation, a delayed asynchronous cancellation from a *previous* unlinking event would eventually catch up and deactivate the newly active subscription. Waiting overnight allowed the asynchronous unlinking process to fully complete before a new, stable linking occurred. The original deactivation was likely triggered by an expired credit card on file, initiating the cycle of confusion.

The essay concludes by celebrating the complexity of systems and the incredible work of builders who make them mostly invisible and functional.

---

## 9. US Government releases first batch of UAP documents and videos

**原文标题**: US Government releases first batch of UAP documents and videos

**原文链接**: [https://www.war.gov/UFO/](https://www.war.gov/UFO/)

生成摘要时出错

---

## 10. Just Use Go

**原文标题**: Just Use Go

**原文链接**: [https://blainsmith.com/articles/just-fucking-use-go/](https://blainsmith.com/articles/just-fucking-use-go/)

生成摘要时出错

---

## 11. Show HN: TRUST – Coding Rust like it's 1989

**原文标题**: Show HN: TRUST – Coding Rust like it's 1989

**原文链接**: [https://github.com/wojtczyk/trust](https://github.com/wojtczyk/trust)

生成摘要时出错

---

## 12. Iran hit more U.S. military targets than has been reported, satellite images

**原文标题**: Iran hit more U.S. military targets than has been reported, satellite images

**原文链接**: [https://www.washingtonpost.com/investigations/2026/05/06/iran-us-bases-satellite-images/](https://www.washingtonpost.com/investigations/2026/05/06/iran-us-bases-satellite-images/)

生成摘要时出错

---

## 13. Serving a website on a Raspberry Pi Zero running in RAM

**原文标题**: Serving a website on a Raspberry Pi Zero running in RAM

**原文链接**: [https://btxx.org/posts/memory/](https://btxx.org/posts/memory/)

生成摘要时出错

---

## 14. ProgramBench: Can language models rebuild programs from scratch?

**原文标题**: ProgramBench: Can language models rebuild programs from scratch?

**原文链接**: [https://arxiv.org/abs/2605.03546](https://arxiv.org/abs/2605.03546)

生成摘要时出错

---

## 15. ShinyHunters claims data theft from 8,800 schools (Instructure/Canvas)

**原文标题**: ShinyHunters claims data theft from 8,800 schools (Instructure/Canvas)

**原文链接**: [https://www.bleepingcomputer.com/news/security/instructure-hacker-claims-data-theft-from-8-800-schools-universities/](https://www.bleepingcomputer.com/news/security/instructure-hacker-claims-data-theft-from-8-800-schools-universities/)

生成摘要时出错

---

## 16. Plasticity and language in the anaesthetized human hippocampus

**原文标题**: Plasticity and language in the anaesthetized human hippocampus

**原文链接**: [https://www.bcm.edu/news/researchers-discover-advanced-language-processing-in-the-unconscious-human-brain](https://www.bcm.edu/news/researchers-discover-advanced-language-processing-in-the-unconscious-human-brain)

生成摘要时出错

---

## 17. Two Home Affairs officials suspended after AI 'hallucinations' found

**原文标题**: Two Home Affairs officials suspended after AI 'hallucinations' found

**原文链接**: [https://www.citizen.co.za/news/home-affairs-officials-suspended-ai-hallucinations/](https://www.citizen.co.za/news/home-affairs-officials-suspended-ai-hallucinations/)

生成摘要时出错

---

## 18. Apple, Intel have reached preliminary chip-making deal

**原文标题**: Apple, Intel have reached preliminary chip-making deal

**原文链接**: [https://www.reuters.com/business/apple-intel-have-reached-preliminary-chip-making-deal-wsj-reports-2026-05-08/](https://www.reuters.com/business/apple-intel-have-reached-preliminary-chip-making-deal-wsj-reports-2026-05-08/)

生成摘要时出错

---

## 19. GeoJSON

**原文标题**: GeoJSON

**原文链接**: [https://geojson.org/](https://geojson.org/)

生成摘要时出错

---

## 20. I switched from Mac to a Lenovo Chromebook

**原文标题**: I switched from Mac to a Lenovo Chromebook

**原文链接**: [https://blog.johnozbay.com/i-left-apples-ecosystem-for-a-lenovo-chromebook-and-you-can-too.html](https://blog.johnozbay.com/i-left-apples-ecosystem-for-a-lenovo-chromebook-and-you-can-too.html)

生成摘要时出错

---

## 21. Making LLM Training Faster with Unsloth and NVIDIA

**原文标题**: Making LLM Training Faster with Unsloth and NVIDIA

**原文链接**: [https://unsloth.ai/blog/nvidia-collab](https://unsloth.ai/blog/nvidia-collab)

生成摘要时出错

---

## 22. Mozilla says 271 vulnerabilities found by Mythos and "almost no false positives"

**原文标题**: Mozilla says 271 vulnerabilities found by Mythos and "almost no false positives"

**原文链接**: [https://arstechnica.com/information-technology/2026/05/mozilla-says-271-vulnerabilities-found-by-mythos-have-almost-no-false-positives/](https://arstechnica.com/information-technology/2026/05/mozilla-says-271-vulnerabilities-found-by-mythos-have-almost-no-false-positives/)

生成摘要时出错

---

## 23. GNU IFUNC is the real culprit behind CVE-2024-3094

**原文标题**: GNU IFUNC is the real culprit behind CVE-2024-3094

**原文链接**: [https://github.com/robertdfrench/ifuncd-up](https://github.com/robertdfrench/ifuncd-up)

生成摘要时出错

---

## 24. What British people mean when they say 'sorry'

**原文标题**: What British people mean when they say 'sorry'

**原文链接**: [https://www.bbc.com/travel/article/20260506-what-british-people-really-mean-when-they-say-sorry](https://www.bbc.com/travel/article/20260506-what-british-people-really-mean-when-they-say-sorry)

生成摘要时出错

---

## 25. The Disappearance of the Public Bench

**原文标题**: The Disappearance of the Public Bench

**原文链接**: [https://placesjournal.org/article/the-disappearance-of-the-public-bench/](https://placesjournal.org/article/the-disappearance-of-the-public-bench/)

生成摘要时出错

---

## 26. ZAYA1-8B matches DeepSeek-R1 on math with less than 1B active parameters

**原文标题**: ZAYA1-8B matches DeepSeek-R1 on math with less than 1B active parameters

**原文链接**: [https://firethering.com/zaya1-8b-open-source-math-coding-model/](https://firethering.com/zaya1-8b-open-source-math-coding-model/)

生成摘要时出错

---

## 27. The Old Guard: Confronting America's Gerontocratic Crisis

**原文标题**: The Old Guard: Confronting America's Gerontocratic Crisis

**原文链接**: [https://harpers.org/archive/2026/05/the-old-guard-samuel-moyn-gerontocracy/](https://harpers.org/archive/2026/05/the-old-guard-samuel-moyn-gerontocracy/)

生成摘要时出错

---

## 28. Principles for agent-native CLIs

**原文标题**: Principles for agent-native CLIs

**原文链接**: [https://twitter.com/trevin/status/2051316002730991795](https://twitter.com/trevin/status/2051316002730991795)

生成摘要时出错

---

## 29. Hackers breach JDownloader's website to serve malware-laced downloads

**原文标题**: Hackers breach JDownloader's website to serve malware-laced downloads

**原文链接**: [https://www.neowin.net/news/if-you-downloaded-this-popular-software-recently-you-might-have-installed-malware/](https://www.neowin.net/news/if-you-downloaded-this-popular-software-recently-you-might-have-installed-malware/)

生成摘要时出错

---

## 30. California leaders report four to six weeks worth of gasoline and diesel supply

**原文标题**: California leaders report four to six weeks worth of gasoline and diesel supply

**原文链接**: [https://kmph.com/news/local/california-leaders-report-four-to-six-weeks-worth-of-gasoline-and-diesel-in-supply](https://kmph.com/news/local/california-leaders-report-four-to-six-weeks-worth-of-gasoline-and-diesel-in-supply)

生成摘要时出错

---

