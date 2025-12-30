# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2025-12-30.md)

*最后自动更新时间: 2025-12-30 19:47:05*
## 1. 未处理照片的样子

**原文标题**: What an unprocessed photo looks like

**原文链接**: [https://maurycyz.com/misc/raw_photo/](https://maurycyz.com/misc/raw_photo/)

未经处理的相机传感器照片并非彩色，而是一个亮度范围有限的“灰蒙蒙”图像。初始的14位模数转换器 (ADC) 输出需要将其值映射到完整的0-255范围，以获得基本对比度。

真正的色彩是通过传感器上的拜耳滤镜阵列引入的，其中每个像素只捕捉红色、绿色或蓝色光。为了创建全彩色图像，一个称为去马赛克的过程会平均相邻像素值，以插值每个像素缺失的颜色信息。

即使在去马赛克之后，图像看起来依然很暗。这是因为人类对亮度的感知是非线性的，并且线性传感器数据直接显示在显示器上（动态范围有限）会显得曝光不足。应用非线性曲线（伽马校正）可以提亮这些暗区。

一个常见问题是偏绿，这源于传感器对绿色光较高的敏感性以及拜耳滤镜中绿色像素数量是其他颜色的两倍。这通过白平衡进行校正，白平衡能够均衡色彩通道。这些步骤，包括动态范围调整、去马赛克、伽马校正和白平衡，代表了最低限度的处理。

文章总结说，相机“未经编辑”的JPEG图像已经是大量数学处理的产物，而非直接的原始输出。编辑软件的调整只是复制和细化了这些相机内部的处理，旨在在显示技术的限制下，生成一个最能代表人类感知的图像。

---

## 2. 被德国铁路绑架

**原文标题**: Kidnapped by Deutsche Bahn

**原文链接**: [https://www.theocharis.dev/blog/kidnapped-by-deutsche-bahn/](https://www.theocharis.dev/blog/kidnapped-by-deutsche-bahn/)

作者讲述了2025年12月24日乘坐德国铁路（DB）的一次离奇经历，当时他正尝试完成从科隆到梅肯海姆35公里的火车旅程。RE5列车已经晚点20分钟，鉴于德国铁路宽松的正点率标准（晚点不足六分钟的列车算“准点”；取消的列车不计），作者讽刺地认为这已经算“早”了。

起初，司机宣布“波恩附近有问题”，建议乘客提前下车或继续前往特罗斯多夫，作者原计划在那里与父亲会面。然而，当列车接近特罗斯多夫时，司机竟声称他们“未在此轨道登记”，“无法停车”，迫使作者眼睁睁看着父亲在车站等候，而列车却疾驰而过。

列车继续开过15个车站，驶向诺伊维德，那里距离祖母家63公里——比起点更远，且位于另一个联邦州。感觉自己像“货物”一样，作者无意中听到一位英国乘客惊呼：“我被绑架了！”对此，另一位乘客无奈地回应了一句“德国铁路”。

最终，这次意想不到的绕行意味着作者“被绑架，还蒙受损失”，因为潜在的1.50欧元赔偿低于德国铁路4.00欧元的最低赔付门槛。此次事件凸显了德国铁路深刻的运营失误和普遍的问责缺失。

---

## 3. Google已死。我们何去何从？

**原文标题**: Google is dead. Where do we go now?

**原文链接**: [https://www.circusscientist.com/2025/12/29/google-is-dead-where-do-we-go-now/](https://www.circusscientist.com/2025/12/29/google-is-dead-where-do-we-go-now/)

无法访问文章链接。

---

## 4. GOG 被其原始联合创始人收购

**原文标题**: GOG is getting acquired by its original co-founder

**原文链接**: [https://www.gog.com/blog/gog-is-getting-acquired-by-its-original-co-founder-what-it-means-for-you/](https://www.gog.com/blog/gog-is-getting-acquired-by-its-original-co-founder-what-it-means-for-you/)

GOG.com 正被其联合创始人 Marcin Iwiński 从母公司 CD PROJEKT S.A. 手中收购。此战略举措旨在通过让 GOG 在更大的 CD PROJEKT 集团之外更独立、更灵活地运营，从而确保其未来。

Marcin Iwiński 将从 CD PROJEKT 联席 CEO 的职位离任，转而领导 GOG。他表示，此次收购将使 GOG 能够重新专注于其核心使命：数字游戏保存、提供无 DRM 游戏以及维护一个玩家至上的平台。

对于用户而言，不会有任何即时变化。现有的游戏库、账户、GOG GALAXY 功能以及客户支持将不受影响。GOG 对无 DRM 游戏、区域定价、现有支付方式以及与开发商和发行商关系的承诺都将一如既往地持续下去。此次收购被视为 GOG "重新发现其独特 DNA" 的机会，从而促进与社区更紧密的联系并巩固其创立原则。这项交易目前正在等待监管机构的批准。

---

## 5. Tesla's 4680 battery supply chain collapses as partner writes down deal by 99%

**原文标题**: Tesla's 4680 battery supply chain collapses as partner writes down deal by 99%

**原文链接**: [https://electrek.co/2025/12/29/tesla-4680-battery-supply-chain-collapses-partner-writes-down-dea/](https://electrek.co/2025/12/29/tesla-4680-battery-supply-chain-collapses-partner-writes-down-dea/)

生成摘要时出错

---

## 6. 你可以编造HTML标签

**原文标题**: You can make up HTML tags

**原文链接**: [https://maurycyz.com/misc/make-up-tags/](https://maurycyz.com/misc/make-up-tags/)

生成摘要时出错

---

## 7. 网飞开放内容

**原文标题**: Netflix Open Content

**原文链接**: [https://opencontent.netflix.com/](https://opencontent.netflix.com/)

奈飞开放内容为娱乐、技术和学术领域提供了宝贵资源，用于探索和原型化尖端媒体技术。为保护其授权节目，奈飞提供涵盖纪录片、真人表演和动画类别的开源测试片源，旨在促进全行业的实验和发现。

这些在知识共享署名4.0国际公共许可协议下发布的资源，展示了4K、高动态范围 (HDR)、高帧率 (HFR) 和杜比全景声 (Dolby Atmos) 等先进格式。许多片源也可在奈飞上流媒体播放，并针对配备高级订阅的HDR设备进行了优化。

用户可以通过网络浏览器直接下载单个文件；然而，对于大型文件和长帧序列，建议使用AWS CLI等命令行工具，并提供详细说明。广告拦截器可能会干扰下载过程。

主要项目包括：
*   **Sol Levante (2020)：** 首部4K HDR杜比全景声动画短片，探索新的制作流程。
*   **Nocturne (2018)：** 一部120帧/秒的真人表演作品，旨在挑战编解码器。
*   **Sparks (2017)：** 以4K HFR拍摄，并使用ACES以4000尼特亮度完成制作。
*   **Meridian (2016)：** 奈飞首个故事驱动的测试片源，采用杜比视界HDR和杜比全景声。
*   **Cosmos Laundromat (2016)：** 一部使用开源Blender制作的动画短片，经重新调色至杜比视界HDR。
*   **Chimera (2014) & El Fuente (2013)：** 早期的4K测试素材，《Chimera》提供挑战编解码器的真实场景，《El Fuente》则侧重于高分辨率和高帧率。

所有资源均可通过 `http://download.opencontent.netflix.com/` 下载。

---

## 8. Show HN: Z80-μLM，容量仅 40KB 的“对话式人工智能”

**原文标题**: Show HN: Z80-μLM, a 'Conversational AI' That Fits in 40KB

**原文链接**: [https://github.com/HarryR/z80ai](https://github.com/HarryR/z80ai)

Z80-μLM 是一个“对话式AI”项目，旨在展示语言模型在保持个性和易于分发的同时可以有多小。它设计用于在配备64KB内存的老式Z80处理器上运行，整个系统——包括推理、权重和一个聊天风格的用户界面——都可装入一个约40KB的.COM文件中。它生成短小的、逐字符的序列，利用量化感知训练（QAT）在其极其受限的环境中运行。

该模型使用三元组哈希编码进行交互，将输入抽象为128个桶。这使得它对短语具有容错性和词序不变性，但对较长、依赖词序的句子则表现不佳。响应有意地简洁（1-2个词），通过上下文传达细微差别，例如“tinychat”（问答）和“guess”（20个问题游戏）等示例所示。

从架构上看，它使用128个输入/上下文桶、可配置的隐藏层，并输出字符。一个关键创新是其2比特权重量化，每个字节封装四个权重，并且所有计算都完全依赖Z80原生的16比特整数算术。定制的汇编循环高效地处理乘法累加操作和算术右移，以防止溢出。

尽管Z80-μLM并非设计用于生成新颖句子或处理深度多轮上下文，但它擅长模糊匹配、通过词汇建立个性，并在严苛的8比特硬件限制下运行。它采用MIT或Apache-2.0许可证发布。

---

## 9. List of domains censored by German ISPs

**原文标题**: List of domains censored by German ISPs

**原文链接**: [https://cuiiliste.de/domains](https://cuiiliste.de/domains)

生成摘要时出错

---

## 10. The future of software development is software developers

**原文标题**: The future of software development is software developers

**原文链接**: [https://codemanship.wordpress.com/2025/11/25/the-future-of-software-development-is-software-developers/](https://codemanship.wordpress.com/2025/11/25/the-future-of-software-development-is-software-developers/)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 2 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 3 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 4 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 5 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 6 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 7 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 8 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 9 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 10 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 11 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 12 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 13 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 14 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 15 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 16 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 17 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 18 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 19 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 20 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 21 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 22 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 23 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 24 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 25 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 26 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 27 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 28 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 29 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 30 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 31 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 32 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 33 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 34 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 35 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 36 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 37 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 38 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 39 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 40 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 41 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 42 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 43 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 44 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 45 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 46 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 47 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 48 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 49 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 50 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 51 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 52 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 53 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 54 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
| 55 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
