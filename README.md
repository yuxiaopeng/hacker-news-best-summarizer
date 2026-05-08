# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-05-08.md)

*最后自动更新时间: 2026-05-08 20:22:22*
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

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 2 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 3 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 4 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 5 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 6 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 7 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 8 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 9 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 10 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 11 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 12 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 13 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 14 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 15 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 16 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 17 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 18 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 19 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 20 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 21 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 22 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 23 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 24 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 25 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 26 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 27 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 28 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 29 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 30 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 31 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 32 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 33 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 34 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 35 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 36 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 37 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 38 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 39 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 40 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 41 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 42 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 43 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 44 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 45 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 46 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 47 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 48 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 49 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 50 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 51 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 52 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 53 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 54 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 55 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 56 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 57 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 58 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 59 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 60 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 61 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 62 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 63 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 64 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 65 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 66 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 67 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 68 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 69 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 70 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 71 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 72 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 73 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 74 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 75 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 76 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 77 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 78 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 79 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 80 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 81 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 82 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 83 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 84 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 85 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 86 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 87 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 88 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 89 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 90 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 91 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 92 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 93 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 94 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 95 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 96 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 97 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 98 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 99 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 100 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 101 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 102 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 103 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 104 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 105 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 106 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 107 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 108 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 109 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 110 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 111 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 112 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 113 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 114 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 115 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 116 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 117 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 118 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 119 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 120 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 121 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 122 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 123 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 124 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 125 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 126 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 127 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 128 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 129 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 130 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 131 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 132 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 133 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 134 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 135 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 136 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 137 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 138 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 139 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 140 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 141 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 142 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 143 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 144 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 145 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 146 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 147 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 148 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 149 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 150 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 151 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 152 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 153 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 154 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 155 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 156 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 157 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 158 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 159 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 160 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 161 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 162 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 163 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 164 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 165 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 166 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 167 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 168 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 169 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 170 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 171 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 172 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 173 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 174 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 175 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 176 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 177 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 178 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 179 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 180 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 181 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 182 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
