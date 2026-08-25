# Hacker News 热门文章摘要 (2026-08-25)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

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

## 11. The entire city of San Francisco as a video game

**原文标题**: The entire city of San Francisco as a video game

**原文链接**: [https://sf.thijs.gg/](https://sf.thijs.gg/)

生成摘要时出错

---

## 12. How I find problems to solve as a staff engineer

**原文标题**: How I find problems to solve as a staff engineer

**原文链接**: [https://lalitm.com/post/find-problems-staff-engineer/](https://lalitm.com/post/find-problems-staff-engineer/)

生成摘要时出错

---

## 13. Executable Is a SQLite Database

**原文标题**: Executable Is a SQLite Database

**原文链接**: [https://fzakaria.com/2026/08/23/your-executable-is-a-sqlite-database](https://fzakaria.com/2026/08/23/your-executable-is-a-sqlite-database)

生成摘要时出错

---

## 14. Coding expertise is going to collapse from AI reliance

**原文标题**: Coding expertise is going to collapse from AI reliance

**原文链接**: [https://larsfaye.com/articles/ai-coding-will-prevent-expertise](https://larsfaye.com/articles/ai-coding-will-prevent-expertise)

生成摘要时出错

---

## 15. Dolly Parton has died

**原文标题**: Dolly Parton has died

**原文链接**: [https://www.theguardian.com/music/2026/aug/25/dolly-parton-country-singer-dead](https://www.theguardian.com/music/2026/aug/25/dolly-parton-country-singer-dead)

生成摘要时出错

---

## 16. I built a low-latency AI companion that plays Skyrim with me

**原文标题**: I built a low-latency AI companion that plays Skyrim with me

**原文链接**: [https://pantel.is/projects/ai-gaming-companion/](https://pantel.is/projects/ai-gaming-companion/)

生成摘要时出错

---

## 17. Google Workspace thinks my domain is an email provider (2025)

**原文标题**: Google Workspace thinks my domain is an email provider (2025)

**原文链接**: [https://blog.elis.cc/articles/google-workspace-thinks-my-domain-is-an-email-provider/](https://blog.elis.cc/articles/google-workspace-thinks-my-domain-is-an-email-provider/)

生成摘要时出错

---

## 18. IPFS Maintainers Winding Down

**原文标题**: IPFS Maintainers Winding Down

**原文链接**: [https://ipshipyard.com/blog/2026-the-end-of-ipfs-at-shipyard/](https://ipshipyard.com/blog/2026-the-end-of-ipfs-at-shipyard/)

生成摘要时出错

---

## 19. New Mac mini, featuring M6 and M5 Pro

**原文标题**: New Mac mini, featuring M6 and M5 Pro

**原文链接**: [https://www.apple.com/newsroom/2026/08/apple-unveils-a-more-powerful-mac-mini-featuring-the-all-new-m6-and-m5-pro/](https://www.apple.com/newsroom/2026/08/apple-unveils-a-more-powerful-mac-mini-featuring-the-all-new-m6-and-m5-pro/)

生成摘要时出错

---

## 20. OpenAI: GPT 5.6 Sol price reduction (until at least Nov 21)

**原文标题**: OpenAI: GPT 5.6 Sol price reduction (until at least Nov 21)

**原文链接**: [https://developers.openai.com/api/docs/pricing](https://developers.openai.com/api/docs/pricing)

生成摘要时出错

---

## 21. Where did all the public bathrooms go?

**原文标题**: Where did all the public bathrooms go?

**原文链接**: [https://daily.jstor.org/where-did-all-the-public-bathrooms-go/](https://daily.jstor.org/where-did-all-the-public-bathrooms-go/)

生成摘要时出错

---

## 22. What's new in Emacs 31.1

**原文标题**: What's new in Emacs 31.1

**原文链接**: [https://www.masteringemacs.org/article/whats-new-in-emacs-311](https://www.masteringemacs.org/article/whats-new-in-emacs-311)

生成摘要时出错

---

## 23. Over 170k Nonprofits Lost All Their Data. Is Microsoft to Blame?

**原文标题**: Over 170k Nonprofits Lost All Their Data. Is Microsoft to Blame?

**原文链接**: [https://slate.com/technology/2026/08/microsoft-software-nonprofit-data-delete.html](https://slate.com/technology/2026/08/microsoft-software-nonprofit-data-delete.html)

生成摘要时出错

---

## 24. Anna's Archive Owes $340 Million, Lost Several Domains, but It's Still Online

**原文标题**: Anna's Archive Owes $340 Million, Lost Several Domains, but It's Still Online

**原文链接**: [https://torrentfreak.com/annas-archive-owes-340-million-lost-several-domains-but-its-still-online/](https://torrentfreak.com/annas-archive-owes-340-million-lost-several-domains-but-its-still-online/)

生成摘要时出错

---

## 25. Qwen 3.8-Flash-Next releasing tomorrow (125B a6B)

**原文标题**: Qwen 3.8-Flash-Next releasing tomorrow (125B a6B)

**原文链接**: [https://modelscope.cn/models/Qwen/Qwen3.8-Flash-Next](https://modelscope.cn/models/Qwen/Qwen3.8-Flash-Next)

生成摘要时出错

---

## 26. Nitter project received cease and desist

**原文标题**: Nitter project received cease and desist

**原文链接**: [https://github.com/zedeus/nitter/issues/1442](https://github.com/zedeus/nitter/issues/1442)

生成摘要时出错

---

## 27. Jabber/XMPP: 25 Years of Digital Independence

**原文标题**: Jabber/XMPP: 25 Years of Digital Independence

**原文链接**: [https://gultsch.de/posts/25-years-of-digital-independence/](https://gultsch.de/posts/25-years-of-digital-independence/)

生成摘要时出错

---

## 28. Moon (2024)

**原文标题**: Moon (2024)

**原文链接**: [https://ciechanow.ski/moon/](https://ciechanow.ski/moon/)

生成摘要时出错

---

## 29. New EU-wide product repair rules come into force

**原文标题**: New EU-wide product repair rules come into force

**原文链接**: [https://www.rte.ie/news/business/2026/0824/1588931-repair-rules/](https://www.rte.ie/news/business/2026/0824/1588931-repair-rules/)

生成摘要时出错

---

## 30. Don't Wordle

**原文标题**: Don't Wordle

**原文链接**: [https://dontwordle.com/](https://dontwordle.com/)

生成摘要时出错

---

## 31. How Universities Should Prepare Founders

**原文标题**: How Universities Should Prepare Founders

**原文链接**: [https://paulgraham.com/prepare.html](https://paulgraham.com/prepare.html)

生成摘要时出错

---

## 32. Show HN: A techno machine in one HTML file, with verifiable renders

**原文标题**: Show HN: A techno machine in one HTML file, with verifiable renders

**原文链接**: [https://ssx360.github.io/rack-02/?src=hn](https://ssx360.github.io/rack-02/?src=hn)

生成摘要时出错

---

## 33. Fable and the end of the free lunch

**原文标题**: Fable and the end of the free lunch

**原文链接**: [https://www.dbreunig.com/2026/08/23/fable-the-end-of-moore-s-law.html](https://www.dbreunig.com/2026/08/23/fable-the-end-of-moore-s-law.html)

生成摘要时出错

---

## 34. Peppermint oil reduces blood pressure by 8.48 mmHg in small study

**原文标题**: Peppermint oil reduces blood pressure by 8.48 mmHg in small study

**原文链接**: [https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0344538](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0344538)

生成摘要时出错

---

## 35. How much of HN is AI?

**原文标题**: How much of HN is AI?

**原文链接**: [https://blog.coredump.cx/p/how-much-of-hn-is-ai](https://blog.coredump.cx/p/how-much-of-hn-is-ai)

生成摘要时出错

---

## 36. SeL4 security proofs now complete on AArch64

**原文标题**: SeL4 security proofs now complete on AArch64

**原文链接**: [https://proofcraft.systems/news-2026/#2026-08-21](https://proofcraft.systems/news-2026/#2026-08-21)

生成摘要时出错

---

## 37. Octopus intelligence may be related to never-before-seen mutation

**原文标题**: Octopus intelligence may be related to never-before-seen mutation

**原文链接**: [https://www.smithsonianmag.com/smart-news/why-are-some-octopuses-so-smart-the-answer-might-lie-in-a-never-before-seen-mutation-that-helps-them-accurately-build-proteins-180989319/](https://www.smithsonianmag.com/smart-news/why-are-some-octopuses-so-smart-the-answer-might-lie-in-a-never-before-seen-mutation-that-helps-them-accurately-build-proteins-180989319/)

生成摘要时出错

---

## 38. Woman stranded in Spain after UK's eVisa system mistakes her for twin sister

**原文标题**: Woman stranded in Spain after UK's eVisa system mistakes her for twin sister

**原文链接**: [https://www.theguardian.com/uk-news/2026/aug/24/woman-stranded-spain-uk-evisa-system-mistakes-twin-sister](https://www.theguardian.com/uk-news/2026/aug/24/woman-stranded-spain-uk-evisa-system-mistakes-twin-sister)

生成摘要时出错

---

## 39. Training AI to Paint with Code

**原文标题**: Training AI to Paint with Code

**原文链接**: [https://surya.website/rling-qwen-to-paint-with-code](https://surya.website/rling-qwen-to-paint-with-code)

生成摘要时出错

---

## 40. FDA clears blood test to aid evaluation for Alzheimer's disease

**原文标题**: FDA clears blood test to aid evaluation for Alzheimer's disease

**原文链接**: [https://medicine.washu.edu/news/fda-clears-blood-test-to-aid-evaluation-for-alzheimers-disease/](https://medicine.washu.edu/news/fda-clears-blood-test-to-aid-evaluation-for-alzheimers-disease/)

生成摘要时出错

---

## 41. My Friend Aaron

**原文标题**: My Friend Aaron

**原文链接**: [https://rorz.io/writing/my-friend-aaron](https://rorz.io/writing/my-friend-aaron)

生成摘要时出错

---

## 42. LLMs could control their host machines by exploiting inference engines

**原文标题**: LLMs could control their host machines by exploiting inference engines

**原文链接**: [https://boydkane.com/essays/llms-could-control-their-host-machines-by-exploiting-inference-engines](https://boydkane.com/essays/llms-could-control-their-host-machines-by-exploiting-inference-engines)

生成摘要时出错

---

## 43. Bomb fishing is wreaking havoc on Indonesia's coral reefs

**原文标题**: Bomb fishing is wreaking havoc on Indonesia's coral reefs

**原文链接**: [https://e360.yale.edu/digest/bomb-fishing-coral-reefs](https://e360.yale.edu/digest/bomb-fishing-coral-reefs)

生成摘要时出错

---

## 44. Why some US restaurants are banning tips

**原文标题**: Why some US restaurants are banning tips

**原文链接**: [https://www.bbc.com/news/articles/c4g36yze692o](https://www.bbc.com/news/articles/c4g36yze692o)

生成摘要时出错

---

## 45. One corner of China’s internet is insisting that the Tang Dynasty never existed

**原文标题**: One corner of China’s internet is insisting that the Tang Dynasty never existed

**原文链接**: [https://www.cnn.com/2026/08/19/style/china-tang-dynasty-never-existed-hoax-intl-hnk](https://www.cnn.com/2026/08/19/style/china-tang-dynasty-never-existed-hoax-intl-hnk)

生成摘要时出错

---

## 46. Building a backyard office, the build and cost breakdown

**原文标题**: Building a backyard office, the build and cost breakdown

**原文链接**: [https://www.imkylelambert.com/articles/building-a-backyard-office-the-build-and-cost-breakdown](https://www.imkylelambert.com/articles/building-a-backyard-office-the-build-and-cost-breakdown)

生成摘要时出错

---

## 47. Fast drilldown dashboards from a single Parquet file

**原文标题**: Fast drilldown dashboards from a single Parquet file

**原文链接**: [https://www.hamiltonulmer.com/customer-dashboards-r2-hyparquet/](https://www.hamiltonulmer.com/customer-dashboards-r2-hyparquet/)

生成摘要时出错

---

## 48. Bookshelf – Self-hosted eBook library that runs on object storage

**原文标题**: Bookshelf – Self-hosted eBook library that runs on object storage

**原文链接**: [https://github.com/murerkinn/bookshelf](https://github.com/murerkinn/bookshelf)

生成摘要时出错

---

## 49. Vintage Artificial Intelligence: Before It Got Awkward

**原文标题**: Vintage Artificial Intelligence: Before It Got Awkward

**原文链接**: [https://blog.archive.org/2026/08/16/vintage-artificial-intelligence-before-it-got-awkward/](https://blog.archive.org/2026/08/16/vintage-artificial-intelligence-before-it-got-awkward/)

生成摘要时出错

---

## 50. Was modern art a CIA psy-op? (2020)

**原文标题**: Was modern art a CIA psy-op? (2020)

**原文链接**: [https://daily.jstor.org/was-modern-art-really-a-cia-psy-op/](https://daily.jstor.org/was-modern-art-really-a-cia-psy-op/)

生成摘要时出错

---

## 51. Show HN: PicoMQ – Durable Streams over HTTP, on object storage

**原文标题**: Show HN: PicoMQ – Durable Streams over HTTP, on object storage

**原文链接**: [https://picomq.com/](https://picomq.com/)

生成摘要时出错

---

## 52. Credit Card Rewards Became a $9.2B Wealth Transfer

**原文标题**: Credit Card Rewards Became a $9.2B Wealth Transfer

**原文链接**: [https://www.library.hbs.edu/working-knowledge/how-credit-card-rewards-became-multibillion-dollar-wealth-transfer](https://www.library.hbs.edu/working-knowledge/how-credit-card-rewards-became-multibillion-dollar-wealth-transfer)

生成摘要时出错

---

## 53. OCR It – pull text out of un-copyable documents for your LLM

**原文标题**: OCR It – pull text out of un-copyable documents for your LLM

**原文链接**: [https://github.com/thiagotigaz/ocr-it](https://github.com/thiagotigaz/ocr-it)

生成摘要时出错

---

## 54. Walgit – a Git server that is one binary in front of an object store

**原文标题**: Walgit – a Git server that is one binary in front of an object store

**原文链接**: [https://github.com/tobi/walgit](https://github.com/tobi/walgit)

生成摘要时出错

---

## 55. The treasury bond mess: is this the demise of the US as a safe haven?

**原文标题**: The treasury bond mess: is this the demise of the US as a safe haven?

**原文链接**: [https://www.theguardian.com/business/2026/aug/24/treasury-bonds-trump-administration-debt](https://www.theguardian.com/business/2026/aug/24/treasury-bonds-trump-administration-debt)

The article highlights the "treasury bond mess" and questions the US's continued status as a global safe haven. Rising treasury yields have dramatically increased the cost of servicing the US's record $40 trillion federal debt, with interest payments now consuming 13.5% of federal spending. Treasury Secretary Scott Bessent's efforts to reduce yields by purchasing bonds proved ineffective, as rates quickly rebounded. This situation is impacting Trump's popularity and the housing market, leading him to blame the Federal Reserve and display erratic economic rhetoric.

More profoundly, the article argues this signals the end of US treasurys as a universally accepted safe, liquid asset for global investors. Historically, foreign central banks and investors heavily relied on treasurys as a secure store of wealth, appreciating even during crises. However, this foundation is weakening: foreign official entities have reduced their holdings, with private foreign investors (who are more volatile) filling some of the gap. The US's budget deficit (6% of GDP) is leading to a massive supply of bonds, outstripping demand, while its debt no longer holds top credit ratings.

Crucially, "Trump’s reckless economic governance" has fostered mistrust, causing investors to dump treasurys during high-risk moments, a stark reversal of their traditional safe-haven behavior. The global financial system, accustomed to treasurys as a bedrock asset, faces uncertainty as their reliability diminishes. Limited government interventions are insufficient to counter the massive debt supply and the erosion of trust in American leadership, prompting a search for alternative safe havens.

---

## 56. Over 5,200 Ebola cases recorded in Congo

**原文标题**: Over 5,200 Ebola cases recorded in Congo

**原文链接**: [https://www.afro.who.int/countries/democratic-republic-of-congo/news/over-5200-cases-recorded-democratic-republic-congocrosses100-days-ebola-outbreak-declaration](https://www.afro.who.int/countries/democratic-republic-of-congo/news/over-5200-cases-recorded-democratic-republic-congocrosses100-days-ebola-outbreak-declaration)

生成摘要时出错

---

## 57. Thomson Reuters Launches Its Own Frontier Model

**原文标题**: Thomson Reuters Launches Its Own Frontier Model

**原文链接**: [https://www.thomsonreuters.com/en/press-releases/2026/august/thomson-reuters-leverages-its-world-class-data-assets-to-launch-its-own-frontier-model](https://www.thomsonreuters.com/en/press-releases/2026/august/thomson-reuters-leverages-its-world-class-data-assets-to-launch-its-own-frontier-model)

生成摘要时出错

---

## 58. OpenAI Jalapeño: Better than Nvidia Blackwell

**原文标题**: OpenAI Jalapeño: Better than Nvidia Blackwell

**原文链接**: [https://newsletter.semianalysis.com/p/openai-jalapeno-better-than-nvidia](https://newsletter.semianalysis.com/p/openai-jalapeno-better-than-nvidia)

生成摘要时出错

---

## 59. Crafting QR Codes: A deep dive into QR code art (2024)

**原文标题**: Crafting QR Codes: A deep dive into QR code art (2024)

**原文链接**: [https://kylezhe.ng/writes/crafting-qr-codes](https://kylezhe.ng/writes/crafting-qr-codes)

生成摘要时出错

---

## 60. AI is hitting entry-level jobs hardest, Stanford study finds

**原文标题**: AI is hitting entry-level jobs hardest, Stanford study finds

**原文链接**: [https://arstechnica.com/ai/2026/08/ai-is-hitting-entry-level-jobs-hardest-stanford-study-finds/](https://arstechnica.com/ai/2026/08/ai-is-hitting-entry-level-jobs-hardest-stanford-study-finds/)

生成摘要时出错

---

## 61. SiFive's First Server Platform

**原文标题**: SiFive's First Server Platform

**原文链接**: [https://chipsandcheese.com/p/sifives-first-server-platform](https://chipsandcheese.com/p/sifives-first-server-platform)

生成摘要时出错

---

## 62. Show HN: GlassBox – what the browser reveals, and how identifiable you are

**原文标题**: Show HN: GlassBox – what the browser reveals, and how identifiable you are

**原文链接**: [https://glassbox.codecanary.org](https://glassbox.codecanary.org)

生成摘要时出错

---

## 63. A Blackstone real estate company exposed SSN digits, DOBs, addresses and more

**原文标题**: A Blackstone real estate company exposed SSN digits, DOBs, addresses and more

**原文链接**: [https://alexschapiro.com/security/vulnerability/2026/07/16/beam-living-graphql-data-exposure](https://alexschapiro.com/security/vulnerability/2026/07/16/beam-living-graphql-data-exposure)

生成摘要时出错

---

## 64. Anger, Anxiety and Agency

**原文标题**: Anger, Anxiety and Agency

**原文链接**: [https://lucumr.pocoo.org/2026/8/24/anger-anxiety-agency/](https://lucumr.pocoo.org/2026/8/24/anger-anxiety-agency/)

生成摘要时出错

---

## 65. Nearly 3M Teslas recalled in China over hidden door handles

**原文标题**: Nearly 3M Teslas recalled in China over hidden door handles

**原文链接**: [https://www.bbc.com/news/articles/c4g6ggdg030o](https://www.bbc.com/news/articles/c4g6ggdg030o)

生成摘要时出错

---

## 66. 'The Nerd Reich' tracks the 'unmasking of Silicon Valley's true politics'

**原文标题**: 'The Nerd Reich' tracks the 'unmasking of Silicon Valley's true politics'

**原文链接**: [https://www.npr.org/2026/08/10/nx-s1-5925350/the-nerd-reich-tracks-the-unmasking-of-silicon-valleys-true-politics](https://www.npr.org/2026/08/10/nx-s1-5925350/the-nerd-reich-tracks-the-unmasking-of-silicon-valleys-true-politics)

生成摘要时出错

---

## 67. France's tax agency got hacked (in French)

**原文标题**: France's tax agency got hacked (in French)

**原文链接**: [https://www.cybernetica.fr/piratage-des-impots-comment-en-est-on-arrive-la/](https://www.cybernetica.fr/piratage-des-impots-comment-en-est-on-arrive-la/)

生成摘要时出错

---

## 68. Headlong: A microharness for persistent agents

**原文标题**: Headlong: A microharness for persistent agents

**原文链接**: [https://www.laude.org/updates/headlong-a-microharness-for-persistent-agents](https://www.laude.org/updates/headlong-a-microharness-for-persistent-agents)

生成摘要时出错

---

## 69. Starbase, LA

**原文标题**: Starbase, LA

**原文链接**: [https://www.spacex.com/sites/starbase-la](https://www.spacex.com/sites/starbase-la)

生成摘要时出错

---

## 70. Anthropic tells staff to work from home due to possible security team strike

**原文标题**: Anthropic tells staff to work from home due to possible security team strike

**原文链接**: [https://www.businessinsider.com/anthropic-san-francisco-staff-work-remote-office-security-strike-2026-8](https://www.businessinsider.com/anthropic-san-francisco-staff-work-remote-office-security-strike-2026-8)

生成摘要时出错

---

## 71. Rural Village in Spain Is Welcoming Digital Nomads with Open Arms

**原文标题**: Rural Village in Spain Is Welcoming Digital Nomads with Open Arms

**原文链接**: [https://www.cntraveler.com/story/this-rural-village-in-spain-is-welcoming-digital-nomads-with-open-arms](https://www.cntraveler.com/story/this-rural-village-in-spain-is-welcoming-digital-nomads-with-open-arms)

生成摘要时出错

---

## 72. OpenAI restores 5-hour Codex and Work limits for ChatGPT Plus users

**原文标题**: OpenAI restores 5-hour Codex and Work limits for ChatGPT Plus users

**原文链接**: [https://9to5mac.com/2026/08/24/openai-restores-5-hour-codex-and-work-limits-for-chatgpt-plus-users/](https://9to5mac.com/2026/08/24/openai-restores-5-hour-codex-and-work-limits-for-chatgpt-plus-users/)

生成摘要时出错

---

## 73. The Future Belongs to the Weird

**原文标题**: The Future Belongs to the Weird

**原文链接**: [https://essays.georgestrakhov.com/weird/](https://essays.georgestrakhov.com/weird/)

生成摘要时出错

---

## 74. Windows 95 released August 24, 1995

**原文标题**: Windows 95 released August 24, 1995

**原文链接**: [https://dfarq.homeip.net/happy-20th-birthday-to-windows-95/](https://dfarq.homeip.net/happy-20th-birthday-to-windows-95/)

生成摘要时出错

---

## 75. Hot Chips 2026: CUDA Targets RISC-V – By Chester Lam

**原文标题**: Hot Chips 2026: CUDA Targets RISC-V – By Chester Lam

**原文链接**: [https://chipsandcheese.com/p/hot-chips-2026-cuda-targets-risc](https://chipsandcheese.com/p/hot-chips-2026-cuda-targets-risc)

生成摘要时出错

---

## 76. The planet now has more trees than it did 35 years ago (2018)

**原文标题**: The planet now has more trees than it did 35 years ago (2018)

**原文链接**: [https://psmag.com/environment/the-planet-now-has-more-trees-than-it-did-35-years-ago/](https://psmag.com/environment/the-planet-now-has-more-trees-than-it-did-35-years-ago/)

生成摘要时出错

---

## 77. Implementation of GPT-2 in pure CMake

**原文标题**: Implementation of GPT-2 in pure CMake

**原文链接**: [https://github.com/AlpinDale/gpt2.cmake](https://github.com/AlpinDale/gpt2.cmake)

生成摘要时出错

---

## 78. Black hole singularity is a surface not a point

**原文标题**: Black hole singularity is a surface not a point

**原文链接**: [https://arxiv.org/abs/2608.21590](https://arxiv.org/abs/2608.21590)

生成摘要时出错

---

## 79. Firefox 157 will include JPEG XL by default on all platforms

**原文标题**: Firefox 157 will include JPEG XL by default on all platforms

**原文链接**: [https://groups.google.com/a/mozilla.org/g/dev-platform/c/3YMV4MS34KA?pli=1](https://groups.google.com/a/mozilla.org/g/dev-platform/c/3YMV4MS34KA?pli=1)

生成摘要时出错

---

## 80. Why older tech is sometimes safer from hackers

**原文标题**: Why older tech is sometimes safer from hackers

**原文链接**: [https://www.bbc.com/future/article/20260821-why-older-tech-is-sometimes-safer-from-hackers](https://www.bbc.com/future/article/20260821-why-older-tech-is-sometimes-safer-from-hackers)

生成摘要时出错

---

## 81. Fences, Not Sandboxes

**原文标题**: Fences, Not Sandboxes

**原文链接**: [https://yegge.ai/essays/fences-not-sandboxes/](https://yegge.ai/essays/fences-not-sandboxes/)

生成摘要时出错

---

## 82. Apple Releases New Polishing Cloth

**原文标题**: Apple Releases New Polishing Cloth

**原文链接**: [https://www.macrumors.com/2026/08/25/apple-releases-new-polishing-cloth/](https://www.macrumors.com/2026/08/25/apple-releases-new-polishing-cloth/)

生成摘要时出错

---

## 83. Ox-Alpha Is GLM?

**原文标题**: Ox-Alpha Is GLM?

**原文链接**: [https://dejan.ai/blog/ox-alpha/](https://dejan.ai/blog/ox-alpha/)

生成摘要时出错

---

## 84. We never use AI. For anything

**原文标题**: We never use AI. For anything

**原文链接**: [https://corkmac.app/our-ai-stance/](https://corkmac.app/our-ai-stance/)

生成摘要时出错

---

## 85. Show HN: How to mentally calculate the day of the week for any date

**原文标题**: Show HN: How to mentally calculate the day of the week for any date

**原文链接**: [https://tinkerandsee.com/weekday/](https://tinkerandsee.com/weekday/)

生成摘要时出错

---

## 86. Removed all counters, replies, following/ers, timestamps, from textlog

**原文标题**: Removed all counters, replies, following/ers, timestamps, from textlog

**原文链接**: [https://textlog.cc/post/2059](https://textlog.cc/post/2059)

生成摘要时出错

---

## 87. Man Dressed as Darth Vader Defends Flock Cameras to San Diego City Council

**原文标题**: Man Dressed as Darth Vader Defends Flock Cameras to San Diego City Council

**原文链接**: [https://thehill.com/policy/technology/6042349-darth-vader-flock-surveillance/](https://thehill.com/policy/technology/6042349-darth-vader-flock-surveillance/)

生成摘要时出错

---

## 88. Mourning Steve French

**原文标题**: Mourning Steve French

**原文链接**: [https://lwn.net/Articles/1090098/](https://lwn.net/Articles/1090098/)

生成摘要时出错

---

## 89. Characterizing Agentic Flooding of Government Services

**原文标题**: Characterizing Agentic Flooding of Government Services

**原文链接**: [https://arxiv.org/abs/2608.16603](https://arxiv.org/abs/2608.16603)

生成摘要时出错

---

## 90. Anthropic Claude and API service outages

**原文标题**: Anthropic Claude and API service outages

**原文链接**: [https://status.claude.com/uptime](https://status.claude.com/uptime)

生成摘要时出错

---

## 91. Why is Anthropic's public writing style so unlike Claude's?

**原文标题**: Why is Anthropic's public writing style so unlike Claude's?

**原文链接**: [https://cmart.blog/claude-writing/](https://cmart.blog/claude-writing/)

生成摘要时出错

---

## 92. Former OC actor Ben McKenzie on crusade to take down 'stupid' cryptocurrency

**原文标题**: Former OC actor Ben McKenzie on crusade to take down 'stupid' cryptocurrency

**原文链接**: [https://www.rnz.co.nz/life/people/celebrity/former-oc-actor-ben-mckenzie-on-crusade-to-take-down-stupid-cryptocurrency](https://www.rnz.co.nz/life/people/celebrity/former-oc-actor-ben-mckenzie-on-crusade-to-take-down-stupid-cryptocurrency)

生成摘要时出错

---

## 93. HelloAssembly: The smallest possible complete Windows application (2021)

**原文标题**: HelloAssembly: The smallest possible complete Windows application (2021)

**原文链接**: [https://github.com/PlummersSoftwareLLC/HelloAssembly](https://github.com/PlummersSoftwareLLC/HelloAssembly)

生成摘要时出错

---

## 94. What Is a Syslog Server?

**原文标题**: What Is a Syslog Server?

**原文链接**: [https://blog.greencloudvps.com/what-is-a-syslog-server.php](https://blog.greencloudvps.com/what-is-a-syslog-server.php)

生成摘要时出错

---

## 95. Agent Is Not the Model

**原文标题**: Agent Is Not the Model

**原文链接**: [https://code.joejag.com/2026/your-agent-is-not-the-model.html](https://code.joejag.com/2026/your-agent-is-not-the-model.html)

生成摘要时出错

---

## 96. Migrating a Synology NAS to a UniFi UNAS Pro 8 with Robocopy, SMB Multichannel

**原文标题**: Migrating a Synology NAS to a UniFi UNAS Pro 8 with Robocopy, SMB Multichannel

**原文链接**: [https://www.hanselman.com/blog/migrating-a-synology-nas-to-a-unifi-unas-pro-8-with-robocopy-smb-multichannel-and-surprising-performance-traps](https://www.hanselman.com/blog/migrating-a-synology-nas-to-a-unifi-unas-pro-8-with-robocopy-smb-multichannel-and-surprising-performance-traps)

生成摘要时出错

---

## 97. Show HN: Kern – container and resource runtime in a 1.5 MB binary, no daemon

**原文标题**: Show HN: Kern – container and resource runtime in a 1.5 MB binary, no daemon

**原文链接**: [https://github.com/getkern/kern](https://github.com/getkern/kern)

生成摘要时出错

---

## 98. US data centers tripled annual water consumption to 17B gallons

**原文标题**: US data centers tripled annual water consumption to 17B gallons

**原文链接**: [https://forgeeks.net/us-data-centers-water-use-17-billion-gallons/](https://forgeeks.net/us-data-centers-water-use-17-billion-gallons/)

生成摘要时出错

---

## 99. We are not going anywhere

**原文标题**: We are not going anywhere

**原文链接**: [https://gist.github.com/omeid/a9d6d1e3c25cb3aa577931e60e006f54](https://gist.github.com/omeid/a9d6d1e3c25cb3aa577931e60e006f54)

生成摘要时出错

---

## 100. Codefloe Is a Professionally Hosted Public Git Forge

**原文标题**: Codefloe Is a Professionally Hosted Public Git Forge

**原文链接**: [https://codefloe.com/](https://codefloe.com/)

生成摘要时出错

---

