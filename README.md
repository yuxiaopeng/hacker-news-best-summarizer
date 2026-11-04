# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-11-04.md)

*最后自动更新时间: 2026-11-04 00:19:02*
## 1. Astra可以读写权重以改进Qwen

**原文标题**: Astra can read and write weights to improve Qwen

**原文链接**: [https://rikiyat.github.io/blog/weight-space-programming/](https://rikiyat.github.io/blog/weight-space-programming/)

本研究介绍了“权重空间编程”，证明了前沿大型语言模型（如GPT-6 Astra）能够直接原生读写神经网络权重。这种范式允许LLM在不依赖传统优化器或训练循环的情况下，通过自然语言目标来推理和修改权重。

本研究提出了几项开创性发现：
1.  **读取权重：** Astra成功识别了PPO网络所训练的游戏、扩散模型生成的形状，甚至仅凭原始权重，就识别出语言模型中间层中的语言和特定的“复制头”（归纳头）。
2.  **修复权重：** Astra通过编辑其3.5%的权重，诊断并修复了一个失败的斜坡汽车策略，将成功率从0%提升至100%。至关重要的是，它通过识别和修复推理循环，仅以极小的（0.016%）权重修改，就提升了Qwen3.5-0.8B的数学表现（MATH-500上从7.9%到48.1%）和指令遵循能力。
3.  **写入权重：** Astra为MinAtar游戏从零开始编写了小型游戏策略网络，其性能超越了经过PPO训练1亿步的策略。

这些壮举是在没有允许Astra编写训练循环或使用梯度下降的情况下完成的，突显了其直接理解和修改底层计算的能力。作者认为，这种“权重空间编程”可能会彻底改变深度学习的优化和可解释性。

---

## 2. 乌班图搞什么鬼？

**原文标题**: WTF Ubuntu?

**原文链接**: [https://chalmovsky.com/posts/wtf-ubuntu](https://chalmovsky.com/posts/wtf-ubuntu)

作者对Ubuntu未能修复一个关键的Linux内核TCP漏洞（CVE-2026-98432，CVSS 9.8）表示极度不满。这个自2016年就存在的漏洞允许远程root访问，并且一个可用的漏洞利用程序已被演示。

尽管Debian已于10月16日修复了该漏洞，但截至2026年11月2日，Ubuntu仍未为其任何受支持版本（包括LTS版本）发布补丁。作者指出，鉴于此次延迟，尤其是在该漏洞被评为关键级九天后、root利用被证实六天后，Ubuntu关于“及时补丁”和“企业级”安全的市场营销承诺显得空洞。

此次延迟导致作者彻底失去了对Ubuntu的信任，促使其决定将所有服务器从该平台迁移出去，并被迫将现有Ubuntu服务器下线。作者进一步批评Canonical这家销售安全订阅服务的公司，竟然落后于Debian、Arch和Alpine等由志愿者运营的发行版，而这些发行版早已提供了修复。

---

## 3. Postman 静默自动安装AI插件并试图共享所有API数据。

**原文标题**: Postman silently auto-installs AI plugins and attempts to share all API data

**原文链接**: [https://github.com/postmanlabs/postman-app-support/issues/14370](https://github.com/postmanlabs/postman-app-support/issues/14370)

生成摘要时出错

---

## 4. 《Astra 可以读写权重来改进 Qwen》一文具有误导性。

**原文标题**: The 'Astra can read and write weights to improve Qwen' post is misleading

**原文链接**: [https://honnibal.dev/blog/astra-read-write-misleading](https://honnibal.dev/blog/astra-read-write-misleading)

这篇文章批评了题为“Astra可以读写权重以改进通义千问”的帖子具有误导性。文章指出，该摘要错误地暗示Astra在所有实验中，特别是针对其标题中强调的通义千问改进，都使用了一种单一的、深层能力——“仅仅通过查看原始权重”。

作者澄清，只有少数在小型网络（1.7万至17.2万个权重）上进行的实验（1、2、4）才真正涉及直接解释原始权重。相比之下，重要的通义千问实验以及其他涉及更大模型或编写游戏对弈网络的实验，并未依赖这种“原始权重”方法。相反，这些任务涉及Astra编写Python程序，而针对通义千问的实验，则是让模型运行多达50批次的练习问题，以分析和修改权重。

文章认为，通义千问的结果表明Astra具备执行类似于人类机器学习工程师设计和执行基于代码的解决方案的任务能力，这令人印象深刻，但与直接理解原始权重有着根本性的区别。作者指出，将这些截然不同的方法——直接权重检查与基于代码的分析/修改并结合模型执行——表现得如同它们源于单一技术，会制造出一种对网络权重拥有统一“格式塔”式理解的错误印象。

---

## 5. If you love a website, back it up

**原文标题**: If you love a website, back it up

**原文链接**: [https://blog.mistys-internet.website/post/2026/10/29/if-you-love-a-website-back-it-up/](https://blog.mistys-internet.website/post/2026/10/29/if-you-love-a-website-back-it-up/)

The author, a web archiving professional, recounts the loss of a beloved fansite, teapuppies.com, which suddenly disappeared and was replaced by gambling ads. This personal tragedy highlights the ephemeral nature of the web and serves as a call to action: individuals can and should proactively back up their favorite websites, rather than waiting for large organizations to do it.

The article explains that personal web archiving is accessible using standard formats like WARC/WACZ. Three main tools, developed by the author's company (mostly free), are recommended:
1.  **ArchiveWeb.page browser extension (Chrome):** The easiest option for single pages or small sites, allowing users to capture what they see in their browser.
2.  **archiveweb.page app:** A standalone application with a built-in browser, offering similar functionality without needing a browser extension.
3.  **Browsertrix:** An automated web crawler suitable for archiving entire large websites or comprehensive social media profiles. It's primarily a web app with a paid per-use model (after a trial), though it's open source.

Once archived, content can be viewed locally using the tools, or shared by sending the WACZ file to others who can use the ArchiveWeb.page app or ReplayWeb.page website. For public display, the ReplayWeb.page embedded viewer can be integrated into any webpage. The author emphasizes that WACZ files are easy to secure and share, promoting collective preservation. The goal is to empower individuals to preserve the digital content that matters to them.

---

## 6. Ubuntu 仍未发布 Linux 0day RCE 补丁，已近三周。

**原文标题**: Ubuntu still has not released patch for Linux 0day RCE in almost 3 weeks

**原文链接**: [https://freenode.net/article/ubuntu-lts-kernels-still-unfixed-for-critical-cve-2026-98432](https://freenode.net/article/ubuntu-lts-kernels-still-unfixed-for-critical-cve-2026-98432)

Ubuntu 尚未发布针对一个关键的 Linux 0day RCE 漏洞 CVE-2026-98432 的补丁，距离该漏洞披露已近三周。该漏洞影响 Ubuntu 的长期支持 (LTS) 内核，特别是 22.04、24.04 和 26.04 版本，其 CVSS 评分高达 9.8，属于严重级别。

这种延迟使得依赖 Ubuntu LTS 内核提供安全和隔离的面向互联网的多租户自托管系统，面临潜在的远程或本地攻击风险。由于缺乏官方供应商更新，管理员无法获取已打补丁的内核软件包来修补这个安全漏洞。

Ubuntu 尚未提供必要修复的预计发布时间（ETA）。这种情况迫使受影响的管理员面临选择：要么在未打补丁的系统上继续运行，要么在可行的情况下实施非官方的树外缓解措施，要么将其工作负载迁移到已解决此漏洞的其他发行版或内核。

---

## 7. 为了调个时间，我竟然给我的车载导航系统越狱了。

**原文标题**: Jailbreaking my car's navigation system just so I can change the time

**原文链接**: [https://blog.nns.ee/2026/11/02/renault-hack/](https://blog.nns.ee/2026/11/02/renault-hack/)

作者遇到一个令人困惑的问题，他们2014年的雷诺纬度（Renault Latitude）在夏令时转换后无法更改汽车时钟。TomTom Carminat LIVE导航单元神秘地缺少了“设置时间”选项。后来发现，访问这个关键设置需要一张特定的、受DRM保护的导航SD卡，而前车主已经将其丢弃，更换一张大约需要60欧元。

作者决心避免这笔开销，于是踏上了一段越狱之旅。对该单元的固件和更新文件进行逆向工程，并建立QEMU模拟器，证实了SD卡的必要性，因为菜单定义都是从SD卡加载的。首次尝试刷入修改后的固件失败了，原因是不明验证，而且大多数文件系统都被挂载为只读或`noexec`，阻止了直接的代码执行。

突破是通过结合两个漏洞实现的：一个`master.script`命令（`LOG`）允许通过目录遍历将任意ASCII写入任何文件路径，而另一个命令（`SHEX`）可以在没有参数的情况下执行现有的rootfs二进制文件。受到内核漏洞利用的启发，作者使用`LOG`将一个shell脚本payload（`|/bin/sh /media/sdcard/payload.sh`）写入`/proc/sys/kernel/core_pattern`。接着，使用`SHEX`执行`/bin/dbus-monitor`，该程序如预期般崩溃，触发了核心转储，并以root权限执行了payload脚本。

获得root权限后，作者创建了完整的eMMC备份。进一步的逆向工程显示，时间偏移量存储在`/mnt/flash/settings.dat`中。将值从180分钟更改为120分钟后，汽车的时钟终于被纠正了。

---

## 8. Google will turn off search for schools that reject AI

**原文标题**: Google will turn off search for schools that reject AI

**原文链接**: [https://www.nytimes.com/2026/11/03/us/google-search-schools-restrict-ai.html](https://www.nytimes.com/2026/11/03/us/google-search-schools-restrict-ai.html)

Unable to access the article link.

---

## 9. OccupySaaS

**原文标题**: OccupySaaS

**原文链接**: [https://occupysaas.com/](https://occupysaas.com/)

生成摘要时出错

---

## 10. US boy names that became girl names and vice versa

**原文标题**: US boy names that became girl names and vice versa

**原文链接**: [https://namedaisy.com/blog/boy-names-that-became-girl-names](https://namedaisy.com/blog/boy-names-that-became-girl-names)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-11-04](output/hacker_news_summary_2026-11-04.md) |
| 2 | [2026-10-30](output/hacker_news_summary_2026-10-30.md) |
| 3 | [2026-11-03](output/hacker_news_summary_2026-11-03.md) |
| 4 | [2026-10-31](output/hacker_news_summary_2026-10-31.md) |
| 5 | [2026-11-01](output/hacker_news_summary_2026-11-01.md) |
| 6 | [2026-10-29](output/hacker_news_summary_2026-10-29.md) |
| 7 | [2026-10-25](output/hacker_news_summary_2026-10-25.md) |
| 8 | [2026-10-27](output/hacker_news_summary_2026-10-27.md) |
| 9 | [2026-10-24](output/hacker_news_summary_2026-10-24.md) |
| 10 | [2026-10-28](output/hacker_news_summary_2026-10-28.md) |
| 11 | [2026-10-26](output/hacker_news_summary_2026-10-26.md) |
| 12 | [2026-10-23](output/hacker_news_summary_2026-10-23.md) |
| 13 | [2026-10-21](output/hacker_news_summary_2026-10-21.md) |
| 14 | [2026-10-22](output/hacker_news_summary_2026-10-22.md) |
| 15 | [2026-10-18](output/hacker_news_summary_2026-10-18.md) |
| 16 | [2026-10-19](output/hacker_news_summary_2026-10-19.md) |
| 17 | [2026-10-20](output/hacker_news_summary_2026-10-20.md) |
| 18 | [2026-10-17](output/hacker_news_summary_2026-10-17.md) |
| 19 | [2026-10-14](output/hacker_news_summary_2026-10-14.md) |
| 20 | [2026-10-16](output/hacker_news_summary_2026-10-16.md) |
| 21 | [2026-10-13](output/hacker_news_summary_2026-10-13.md) |
| 22 | [2026-10-11](output/hacker_news_summary_2026-10-11.md) |
| 23 | [2026-10-15](output/hacker_news_summary_2026-10-15.md) |
| 24 | [2026-10-03](output/hacker_news_summary_2026-10-03.md) |
| 25 | [2026-10-06](output/hacker_news_summary_2026-10-06.md) |
| 26 | [2026-10-10](output/hacker_news_summary_2026-10-10.md) |
| 27 | [2026-10-04](output/hacker_news_summary_2026-10-04.md) |
| 28 | [2026-10-07](output/hacker_news_summary_2026-10-07.md) |
| 29 | [2026-10-09](output/hacker_news_summary_2026-10-09.md) |
| 30 | [2026-09-27](output/hacker_news_summary_2026-09-27.md) |
| 31 | [2026-09-30](output/hacker_news_summary_2026-09-30.md) |
| 32 | [2026-10-01](output/hacker_news_summary_2026-10-01.md) |
| 33 | [2026-09-29](output/hacker_news_summary_2026-09-29.md) |
| 34 | [2026-09-25](output/hacker_news_summary_2026-09-25.md) |
| 35 | [2026-10-02](output/hacker_news_summary_2026-10-02.md) |
| 36 | [2026-09-24](output/hacker_news_summary_2026-09-24.md) |
| 37 | [2026-09-19](output/hacker_news_summary_2026-09-19.md) |
| 38 | [2026-09-22](output/hacker_news_summary_2026-09-22.md) |
| 39 | [2026-09-21](output/hacker_news_summary_2026-09-21.md) |
| 40 | [2026-09-23](output/hacker_news_summary_2026-09-23.md) |
| 41 | [2026-09-20](output/hacker_news_summary_2026-09-20.md) |
| 42 | [2026-09-17](output/hacker_news_summary_2026-09-17.md) |
| 43 | [2026-09-13](output/hacker_news_summary_2026-09-13.md) |
| 44 | [2026-09-18](output/hacker_news_summary_2026-09-18.md) |
| 45 | [2026-09-15](output/hacker_news_summary_2026-09-15.md) |
| 46 | [2026-09-14](output/hacker_news_summary_2026-09-14.md) |
| 47 | [2026-09-16](output/hacker_news_summary_2026-09-16.md) |
| 48 | [2026-09-11](output/hacker_news_summary_2026-09-11.md) |
| 49 | [2026-09-07](output/hacker_news_summary_2026-09-07.md) |
| 50 | [2026-09-10](output/hacker_news_summary_2026-09-10.md) |
| 51 | [2026-09-12](output/hacker_news_summary_2026-09-12.md) |
| 52 | [2026-09-09](output/hacker_news_summary_2026-09-09.md) |
| 53 | [2026-09-08](output/hacker_news_summary_2026-09-08.md) |
| 54 | [2026-09-06](output/hacker_news_summary_2026-09-06.md) |
| 55 | [2026-09-04](output/hacker_news_summary_2026-09-04.md) |
| 56 | [2026-09-01](output/hacker_news_summary_2026-09-01.md) |
| 57 | [2026-09-02](output/hacker_news_summary_2026-09-02.md) |
| 58 | [2026-09-05](output/hacker_news_summary_2026-09-05.md) |
| 59 | [2026-08-30](output/hacker_news_summary_2026-08-30.md) |
| 60 | [2026-08-31](output/hacker_news_summary_2026-08-31.md) |
| 61 | [2026-09-03](output/hacker_news_summary_2026-09-03.md) |
| 62 | [2026-08-23](output/hacker_news_summary_2026-08-23.md) |
| 63 | [2026-08-28](output/hacker_news_summary_2026-08-28.md) |
| 64 | [2026-08-24](output/hacker_news_summary_2026-08-24.md) |
| 65 | [2026-08-26](output/hacker_news_summary_2026-08-26.md) |
| 66 | [2026-08-29](output/hacker_news_summary_2026-08-29.md) |
| 67 | [2026-08-25](output/hacker_news_summary_2026-08-25.md) |
| 68 | [2026-08-22](output/hacker_news_summary_2026-08-22.md) |
| 69 | [2026-08-16](output/hacker_news_summary_2026-08-16.md) |
| 70 | [2026-08-13](output/hacker_news_summary_2026-08-13.md) |
| 71 | [2026-08-20](output/hacker_news_summary_2026-08-20.md) |
| 72 | [2026-08-19](output/hacker_news_summary_2026-08-19.md) |
| 73 | [2026-08-21](output/hacker_news_summary_2026-08-21.md) |
| 74 | [2026-08-18](output/hacker_news_summary_2026-08-18.md) |
| 75 | [2026-08-15](output/hacker_news_summary_2026-08-15.md) |
| 76 | [2026-08-14](output/hacker_news_summary_2026-08-14.md) |
| 77 | [2026-08-17](output/hacker_news_summary_2026-08-17.md) |
| 78 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 79 | [2026-08-09](output/hacker_news_summary_2026-08-09.md) |
| 80 | [2026-08-12](output/hacker_news_summary_2026-08-12.md) |
| 81 | [2026-08-10](output/hacker_news_summary_2026-08-10.md) |
| 82 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 83 | [2026-08-11](output/hacker_news_summary_2026-08-11.md) |
| 84 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 85 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 86 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 87 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 88 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 89 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 90 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 91 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 92 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 93 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 94 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 95 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 96 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 97 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 98 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 99 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 100 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 101 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 102 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 103 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 104 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 105 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 106 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 107 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 108 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 109 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 110 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 111 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 112 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 113 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 114 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 115 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 116 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 117 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 118 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 119 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 120 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 121 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 122 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 123 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 124 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 125 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 126 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 127 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 128 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 129 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 130 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 131 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 132 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 133 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 134 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 135 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 136 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 137 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 138 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 139 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 140 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 141 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 142 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 143 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 144 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 145 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 146 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 147 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 148 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 149 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 150 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 151 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 152 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 153 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 154 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 155 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 156 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 157 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 158 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 159 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 160 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 161 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 162 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 163 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 164 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 165 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 166 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 167 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 168 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 169 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 170 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 171 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 172 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 173 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 174 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 175 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 176 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 177 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 178 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 179 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 180 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 181 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 182 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 183 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 184 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 185 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 186 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 187 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 188 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 189 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 190 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 191 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 192 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 193 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 194 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 195 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 196 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 197 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 198 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 199 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 200 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 201 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 202 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 203 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 204 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 205 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 206 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 207 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 208 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 209 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 210 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 211 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 212 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 213 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 214 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 215 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 216 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 217 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 218 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 219 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 220 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 221 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 222 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 223 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 224 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 225 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 226 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 227 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 228 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 229 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 230 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 231 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 232 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 233 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 234 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 235 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 236 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 237 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 238 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 239 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 240 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 241 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 242 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 243 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 244 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 245 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 246 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 247 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 248 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 249 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 250 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 251 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 252 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 253 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 254 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 255 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 256 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 257 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 258 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 259 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 260 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 261 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 262 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 263 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 264 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 265 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 266 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 267 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 268 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 269 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 270 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 271 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 272 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 273 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 274 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 275 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 276 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 277 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 278 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 279 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 280 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 281 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 282 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 283 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 284 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 285 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 286 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 287 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 288 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 289 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 290 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 291 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 292 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 293 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 294 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 295 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 296 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 297 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 298 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 299 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 300 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 301 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 302 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 303 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 304 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 305 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 306 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 307 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 308 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 309 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 310 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 311 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 312 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 313 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 314 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 315 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 316 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 317 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 318 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 319 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 320 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 321 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 322 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 323 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 324 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 325 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 326 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 327 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 328 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 329 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 330 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 331 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 332 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 333 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 334 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 335 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 336 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 337 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 338 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 339 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 340 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 341 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 342 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 343 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 344 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 345 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 346 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 347 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 348 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 349 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 350 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 351 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 352 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 353 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 354 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
