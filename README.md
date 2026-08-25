# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-08-25.md)

*最后自动更新时间: 2026-08-25 20:02:59*
## 1. 欧洲如何扼杀创客和微创业者

**原文标题**: How Europe is killing makers and micro-entrepreneurs

**原文链接**: [https://lectronz.com/u/lectronz/articles/how-europe-is-killing-makers-and-micro-entrepreneurs](https://lectronz.com/u/lectronz/articles/how-europe-is-killing-makers-and-micro-entrepreneurs)

欧盟新《包装和包装废弃物条例》（PPWR）将于2026年8月生效，对包括开源硬件制造商、艺术家和手工艺人在内的微型创业者构成严重威胁。尽管该条例旨在落实生产者责任延伸（EPR）——即让生产者为包装废弃物的收集和回收提供资金——这一目标是合理的，但其执行方式存在严重缺陷。

PPWR并未建立统一的欧洲系统，而是保留了分散的国家模式。这迫使在欧盟范围内销售产品的小企业必须在每个成员国单独注册、报告和缴纳费用。一个例子可以说明这种不相称的负担：一位希腊工程师向四个欧盟国家销售仅十件低价值商品，每年因极少量包装废弃物而面临的合规成本将超过1150欧元。这种行政和财政负担使得小批量卖家的跨境销售变得不可行，从而扼杀了对创新至关重要的“创意试验空间”。

这种监管环境偏袒大公司而非微型企业和中小企业，威胁着整个独立创作者生态系统。硬件制造商交易平台Lectronz担心许多卖家将退出欧盟市场，这可能危及其自身的生存。对于一些企业而言，向非欧盟市场发货甚至可能比在欧盟内部贸易更具经济可行性。

为解决这一问题，文章提出了解决方案：设立全欧盟范围的“微量豁免”门槛以豁免小批量卖家，建立集中的欧盟EPR“一站式服务”以简化合规流程，并允许交易平台为其卖家集体管理EPR。尽管欧盟委员会已提议暂时中止授权代表要求，但这一部分措施仍不足够。作者敦促个人通过在线请愿和欧盟委员会反馈页面表达担忧，强调现有规则正在破坏欧盟针对微型企业的单一市场。

---

## 2. 我的所有，皆已拥有。

**原文标题**: Everything I own, owned

**原文链接**: [https://schlarp.com/posts/everything-i-own-owned/](https://schlarp.com/posts/everything-i-own-owned/)

作者详细描述了他使用AI（Claude Opus 5）进行外设“代理驱动逆向工程”的经历，将数周的手动工作转变为一个基本无需人工干预的过程。在两周多的时间里，他投入了大约13小时的AI工作和98次提示，成功“控制”了五台设备。

他的方法是向AI提供设备固件和更新工具，并指令AI执行固件文档化、逆向工程更新协议、评估安全性、枚举功能以及发现隐藏功能。

值得注意的成果包括：
*   **Insta360 Link 网络摄像头：** 他在录制时禁用了活动指示灯，并实现了完全无需用户交互的固件刷写，同时发现该设备缺乏防篡改机制。
*   **华硕 ROG Swift 显示器：** 他找到了禁用烦人的“像素清洁”弹窗的方法，并通过Linux获得了DDC/CI控制。
*   **舒尔 MV7 麦克风：** 他发现了一个通过USB HID实现的明文命令行界面，可通过网页界面访问，其四级权限系统（“su sup”）可被轻易绕过，从而控制LED、内存和DSP设置。
*   **Elgato Cam Link 4K 采集卡：** AI完全拆解并自主开发了固件更新程序。
*   **Elgato Key Light Mini：** 尽管存在Ed25519固件签名验证，他仍发现了一个可以禁用签名检查的HTTP POST命令，从而允许进行未签名固件更新。

尽管对硬件定制和互操作性的潜力感到兴奋，但作为一名安全专业人士，作者表达了深切担忧。他现在认为任何连接的设备都可能搭载恶意固件，而操作系统尚未为此类威胁做好准备。他警告说，WebUSB/HID/Bluetooth可能通过用户疏忽导致设备永久后门，并且联网设备“几乎普遍面临风险”。他担心配备AI、能够自我复制的恶意软件会利用这种新发现的逆向工程便利性，感染大量设备，他相信这种情况可能已经正在发生。

---

## 3. 小米：新CPU单线程性能匹敌苹果核心，多线程则快得多。

**原文标题**: Xiaomi: New CPU matches Apple cores single threaded, much faster multithreaded

**原文链接**: [https://twitter.com/lemire/status/2091894299289874926](https://twitter.com/lemire/status/2091894299289874926)

小米发布了其新款Xring O3 CPU，标志着移动处理器技术的一项重大进展。据报道，这款新芯片在单线程性能上可与苹果核心相媲美，并在多线程执行方面提供显著更快的速度。冰宇宙分享的Geekbench分数证实了这一点，单核得分高达3,945，多核得分更是“前所未有”的15,221。

Xring O3的一个显著特点是其高达44 MB的总缓存，这一缓存容量甚至超过了许多笔记本电脑CPU。其强大的C1-Ultra核心配备了用于AI加速的SME2和用于数据并行（SIMD）的SVE2。该芯片拥有异常宽的架构，具有21个执行端口，其中六个支持128位SIMD操作，超过了许多英特尔/AMD处理器中的执行端口数量。

这一发展凸显了CPU设计的一个清晰趋势：即转向大规模并行核心，拥有更多执行单元、增强的SIMD能力、更多算术单元和更大的片上缓存。尽管苹果预计很快将发布其下一代处理器，并且Xring O3最初可能难以在手机中找到，但小米的新CPU依然标志着计算能力，尤其是在并行任务方面，取得了显著飞跃。

---

## 4. MS Paint 和 Photos 甚至会给本地生成的输出内容隐形地添加 GUID 水印。

**原文标题**: MS Paint and Photos inivisibly watermark even locally generated output with GUID

**原文链接**: [https://xusheng.dev/posts/reversing/mspaint_invisible_watermark/main/](https://xusheng.dev/posts/reversing/mspaint_invisible_watermark/main/)

微软画图和照片应用使用服务器颁发的GUID，对本地生成的AI图像进行隐形水印。尽管特别是在Copilot+电脑上利用本地AI模型，该过程并非完全离线。画图会将用户提示发送到远程微软服务器进行审核，服务器随后会返回一个唯一的GUID以及经过审核的提示。这个GUID通过`WmkWriteWatermark`函数直接嵌入到本地生成图像的像素中，进行细微的量化改变。这种嵌入失败会导致整个图像生成失败，凸显了其重要性。这种隐形水印与画图应用中可选的可见Copilot标志是不同的。

此外，这个相同的服务器颁发的GUID也会包含在保存的AI生成图像所附带的C2PA内容凭证元数据中，形成一种“软绑定”，将图像内容与其来源关联起来。对于Copilot+电脑上的“Cocreator”等功能来说，本地水印是必需的，因为这些功能的图像生成是本地的，但唯一标识符却是远程生成的。因此，保存AI生成图像的格式仅限于PNG、JPEG、GIF和.paint等C2PA兼容格式。

---

## 5. 苹果推出M6和M5 Ultra

**原文标题**: Apple introduces M6 and M5 Ultra

**原文链接**: [https://www.apple.com/newsroom/2026/08/apple-introduces-m6-and-m5-ultra-for-a-big-leap-in-performance-and-ai-compute/](https://www.apple.com/newsroom/2026/08/apple-introduces-m6-and-m5-ultra-for-a-big-leap-in-performance-and-ai-compute/)

苹果发布了全新的M6和M5 Ultra芯片，在性能和AI能力方面实现了显著飞跃，并首次搭载于新款Mac mini和Mac Studio。

M6是苹果首款2纳米芯片，搭载12核中央处理器 (CPU) (包括2个超高性能核心、4个性能核心和6个能效核心)，多线程处理性能比M5快达1.2倍。其12核图形处理器 (GPU) 现已集成神经网络加速器，AI运算能力比M5提升近30%，并支持先进图形处理。双16核神经网络引擎提供比前代产品高达2倍的峰值AI算力。M6支持高达32GB统一内存，具备170GB/s的带宽，专为日常用户、学生和开发者设计，能够高效处理设备端AI和高要求任务。

M5 Ultra是苹果迄今为止最强大的芯片，专为专业人士和高强度AI工作负载而打造。它采用四晶粒架构，借助UltraFusion技术。它搭载最高达36核中央处理器 (CPU) (包括12个超高性能核心和24个性能核心)，多线程处理性能比M3 Ultra高出1.3倍。其新一代最高达80核图形处理器 (GPU) 集成神经网络加速器，提供比M3 Ultra高达4.5倍的峰值AI算力，图形处理速度提升40%。凭借高达512GB的统一内存和1.2TB/s的带宽 (比M3 Ultra多50%)，M5 Ultra能够处理复杂的3D渲染、高分辨率视频编辑和大规模设备端AI模型。这两款芯片都强调安全、设备端AI以及行业领先的能效。

---

## 6. 安德森·霍洛维茨正向黯淡的未来投资数十亿。

**原文标题**: Andreessen Horowitz is investing billions into a bleak future

**原文链接**: [https://www.modelrepublic.org/articles/a16z-portfolio](https://www.modelrepublic.org/articles/a16z-portfolio)

文章批评Andreessen Horowitz (a16z) 投资数十亿美元给那些道德可疑的公司，同时积极塑造人工智能政策，以营造一个有利于其投资组合的宽松监管环境。

该公司的投资包括“Doublespeed”，一个“机器人农场”，它利用人工智能生成的虚假账户制造欺骗性社交媒体广告，经常以弱势群体为目标，用误导性声明宣传如保健品之类的产品。这种商业模式违反了平台政策和联邦贸易委员会（FTC）的披露规定。另一个投资是“Cluely AI”，最初其市场定位是帮助用户在约会、求职面试和考试中“作弊”，其创始人甚至公开承认学术不端。尽管后来重新定位，其“不可检测”的功能仍然突出。

A16z还投资了“Coverd”等赌博公司，该公司鼓励用户“押注账单”，将信用卡支付与赌场式游戏挂钩。批评者认为，这种模式旨在针对经济弱势群体，打着“金融精明”的幌子，利用他们的绝望心理。

与此同时，a16z正花费数百万美元影响人工智能政策，其前合伙人担任政府职务，并推动削弱州级人工智能法律。该报告总结称，这些投资揭示了一种行为模式和跨越道德底线的意愿，a16z倡导建立一个监管环境，以进一步有利于这些有争议的企业，最终导致一个“黯淡”的未来。

---

## 7. 海洋温度创历史新高

**原文标题**: Oceans hit highest temperature on record

**原文链接**: [https://www.bbc.com/news/articles/c62m4gpnp78o](https://www.bbc.com/news/articles/c62m4gpnp78o)

全球海洋温度已达有记录以来最高水平，极地以外海域的平均表面温度达到21.1摄氏度（70华氏度），超过了2024年3月的先前记录。这一惊人的高温是人类引起的气候变化和快速增强的厄尔尼诺天气现象共同作用的结果。

科学家指出，8月份的这一记录尤为令人担忧，因为海洋温度通常在3月或4月达到峰值。这一提前到来的峰值预示着日益增强的厄尔尼诺现象的强大威力，它给热带太平洋带来了异常温暖的海水，并且预计将持续增强直至圣诞节，可能成为几个世纪以来最强的一次，进一步推高全球气温。

这种暖化现象普遍存在，例如，英吉利海峡西部等地区正经历持续的海洋热浪，并在7月份达到比正常水平高出7摄氏度的峰值。专家证实，海洋吸收了人类温室气体排放产生的90%以上的过剩热量。

海洋变暖会带来严重后果：它会加剧极端天气，提高海平面，增加沿海洪灾风险，并破坏珊瑚礁等海洋生态系统。这种对海洋环境不断升级的压力对生物多样性以及依赖海洋的社区构成了重大威胁。

---

## 8. New Mac Studio with M5 Max and M5 Ultra

**原文标题**: New Mac Studio with M5 Max and M5 Ultra

**原文链接**: [https://www.apple.com/newsroom/2026/08/apple-introduces-new-mac-studio-with-m5-max-and-m5-ultra/](https://www.apple.com/newsroom/2026/08/apple-introduces-new-mac-studio-with-m5-max-and-m5-ultra/)

生成摘要时出错

---

## 9. I were 17, I'd learn how to build LLMs from scratch

**原文标题**: I were 17, I'd learn how to build LLMs from scratch

**原文链接**: [https://twitter.com/paulg/status/2091544343589060625](https://twitter.com/paulg/status/2091544343589060625)

生成摘要时出错

---

## 10. iCloud+ Hide My Email addresses will remain on icloud.com

**原文标题**: iCloud+ Hide My Email addresses will remain on icloud.com

**原文链接**: [https://developer.apple.com/news/?id=1ptvdtcm](https://developer.apple.com/news/?id=1ptvdtcm)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-08-25](output/hacker_news_summary_2026-08-25.md) |
| 2 | [2026-08-24](output/hacker_news_summary_2026-08-24.md) |
| 3 | [2026-08-23](output/hacker_news_summary_2026-08-23.md) |
| 4 | [2026-08-18](output/hacker_news_summary_2026-08-18.md) |
| 5 | [2026-08-15](output/hacker_news_summary_2026-08-15.md) |
| 6 | [2026-08-21](output/hacker_news_summary_2026-08-21.md) |
| 7 | [2026-08-19](output/hacker_news_summary_2026-08-19.md) |
| 8 | [2026-08-20](output/hacker_news_summary_2026-08-20.md) |
| 9 | [2026-08-14](output/hacker_news_summary_2026-08-14.md) |
| 10 | [2026-08-17](output/hacker_news_summary_2026-08-17.md) |
| 11 | [2026-08-16](output/hacker_news_summary_2026-08-16.md) |
| 12 | [2026-08-22](output/hacker_news_summary_2026-08-22.md) |
| 13 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 14 | [2026-08-09](output/hacker_news_summary_2026-08-09.md) |
| 15 | [2026-08-10](output/hacker_news_summary_2026-08-10.md) |
| 16 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 17 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 18 | [2026-08-11](output/hacker_news_summary_2026-08-11.md) |
| 19 | [2026-08-12](output/hacker_news_summary_2026-08-12.md) |
| 20 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 21 | [2026-08-13](output/hacker_news_summary_2026-08-13.md) |
| 22 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 23 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 24 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 25 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 26 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 27 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 28 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 29 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 30 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 31 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 32 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 33 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 34 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 35 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 36 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 37 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 38 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 39 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 40 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 41 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 42 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 43 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 44 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 45 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 46 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 47 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 48 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 49 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 50 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 51 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 52 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 53 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 54 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 55 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 56 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 57 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 58 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 59 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 60 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 61 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 62 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 63 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 64 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 65 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 66 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 67 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 68 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 69 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 70 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 71 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 72 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 73 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 74 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 75 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 76 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 77 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 78 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 79 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 80 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 81 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 82 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 83 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 84 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 85 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 86 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 87 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 88 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 89 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 90 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 91 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 92 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 93 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 94 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 95 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 96 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 97 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 98 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 99 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 100 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 101 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 102 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 103 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 104 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 105 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 106 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 107 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 108 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 109 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 110 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 111 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 112 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 113 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 114 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 115 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 116 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 117 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 118 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 119 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 120 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 121 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 122 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 123 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 124 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 125 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 126 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 127 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 128 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 129 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 130 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 131 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 132 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 133 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 134 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 135 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 136 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 137 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 138 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 139 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 140 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 141 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 142 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 143 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 144 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 145 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 146 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 147 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 148 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 149 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 150 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 151 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 152 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 153 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 154 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 155 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 156 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 157 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 158 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 159 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 160 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 161 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 162 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 163 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 164 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 165 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 166 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 167 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 168 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 169 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 170 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 171 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 172 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 173 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 174 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 175 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 176 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 177 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 178 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 179 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 180 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 181 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 182 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 183 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 184 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 185 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 186 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 187 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 188 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 189 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 190 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 191 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 192 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 193 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 194 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 195 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 196 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 197 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 198 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 199 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 200 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 201 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 202 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 203 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 204 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 205 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 206 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 207 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 208 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 209 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 210 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 211 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 212 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 213 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 214 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 215 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 216 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 217 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 218 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 219 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 220 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 221 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 222 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 223 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 224 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 225 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 226 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 227 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 228 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 229 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 230 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 231 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 232 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 233 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 234 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 235 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 236 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 237 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 238 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 239 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 240 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 241 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 242 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 243 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 244 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 245 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 246 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 247 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 248 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 249 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 250 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 251 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 252 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 253 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 254 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 255 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 256 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 257 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 258 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 259 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 260 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 261 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 262 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 263 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 264 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 265 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 266 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 267 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 268 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 269 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 270 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 271 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 272 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 273 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 274 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 275 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 276 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 277 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 278 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 279 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 280 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 281 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 282 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 283 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 284 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 285 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 286 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 287 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 288 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 289 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 290 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
