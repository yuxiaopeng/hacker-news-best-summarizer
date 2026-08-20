# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-08-20.md)

*最后自动更新时间: 2026-08-20 19:53:13*
## 1. 解锁锁定/停用的废弃Cricut Maker

**原文标题**: Unlocking a locked/deactivated e-waste Cricut Maker

**原文链接**: [https://sprocketfox.io/xssfox/2026/07/01/cricut-unlock/](https://sprocketfox.io/xssfox/2026/07/01/cricut-unlock/)

某人从电子垃圾中发现了一台已停用的Cricut Maker，外观完好，但滚轮已损坏并显示“机器已停用”错误。最初尝试通过重写EEPROM（未找到）或拦截网络流量（由于证书锁定）来重新激活它，均未成功。

成功的方法涉及拦截Cricut和电脑之间的USB通信。作者使用Wireshark发现序列号数据包未加密发送且没有校验和。随后，使用一块超频的RP2040微控制器，充当USB主设备和从设备，创建一个硬件代理。该设备拦截Cricut发出的序列号，将其替换为一个新的、可用的序列号，并将其传递给电脑。这种实时序列号重写骗过了软件，使其识别为一台“新”机器，从而恢复了全部功能。

除了此破解方法之外，还更换了滚轮（用热水软化），清洁并重新组装了机器，并将RP2040安置妥当。机器现在运行起来如同全新。作者承认这是一个硬件密集型解决方案，并提出了一些基于软件的替代方案。由于潜在的版权问题，序列号重写的具体代码未公开分享。

---

## 2. 中情局的资金帮助NeXT在80年代得以存续。

**原文标题**: CIA funding helped keep NeXT afloat in the 80s

**原文链接**: [https://www.wsj.com/tech/steve-jobs-apple-next-cia-161b65f9?st=NWWds1&reflink=desktopwebshare_permalink](https://www.wsj.com/tech/steve-jobs-apple-next-cia-161b65f9?st=NWWds1&reflink=desktopwebshare_permalink)

无法访问文章链接。

---

## 3. Mojo语言（由Modular开发，现属高通）现已开源。

**原文标题**: The Mojo language (by Modular, now Qualcomm) is now open-source

**原文链接**: [https://www.modular.com/blog/modcon-announcements](https://www.modular.com/blog/modcon-announcements)

ModCon 2026大会于2026年8月18日举行，Modular（现已并入高通）在此次大会上宣布了几项关键进展，这些进展与其在异构硬件上实现AI的愿景保持一致。

至关重要的是，**Mojo语言1.0现已基于Apache 2.0许可证全面开源**，包括其编译器和工具链。继其标准库和MAX内核早前开源之后，这一战略举措使开发者能够扩展Mojo并将其引入新平台。与微软的合作也正在进行中，旨在为Mojo提供原生Windows支持。

**Modular Cloud**现已作为生产服务正式上线，它抽象化了在多样化基础设施上部署和优化模型的复杂性。该服务提供行业领先的推理性能，为MiniMax等旗舰客户提供支持（以每分钟数十亿token的速度驱动M3），并此前已与OpenRouter共同展现出卓越性能。

此外，**Modular平台**已显著扩展其硬件支持范围，从GPU扩展到AWS Trainium、Google TPU、高通Cloud AI 100和高通Dragonfly，展示了高可移植性，新集成所需的工程工作量减少了10倍。

为了促进生态系统协作，**MAX许可证已放宽**，取消了设备使用限制，并且MAX将通过开放联盟计划提供源代码。在近期高通收购Modular的强化下，该举措旨在构建一个通用的、开放的软件基础，业界可以在其上协作优化适用于任何加速器的AI。

---

## 4. Ornith-1.5：从自我搭建到自我提升

**原文标题**: Ornith-1.5: From Self-Scaffolding to Self-Improvement

**原文链接**: [https://ornith.ai/ornith_1_5.html](https://ornith.ai/ornith_1_5.html)

Ornith-1.5 引入了一个端到端的基础模型自我提升框架，将 Ornith-1.0 的自支架扩展为一个持续学习循环。它允许模型自主提出新的、难度递增的任务，生成针对任务的支架（指令、工具、策略），并为强化学习生成解决方案推演，从而不断创造新的训练经验。

该系统有三种规模：397B MoE 模型、35B MoE 模型和一个 9B 密集模型，同时还有一个针对 iPhone 和 Android 优化的移动版 9B 模型。这一自我提升过程分为三个阶段，由特定的奖励信号引导：
1.  **任务奖励：** 鼓励生成有效、可验证、难度适中（目标成功率 20%）且新颖的任务。
2.  **驾驭奖励：** 促进创建与任务对齐、忠实反映解决方案质量且能抵抗奖励作弊的评估环境。
3.  **推演奖励：** 根据任务成功情况直接评估策略的解决方案尝试。

这一闭环系统使 Ornith-1.5 能够动态扩展其课程并调整问题解决策略，从而在推理、编码和智能体任务中持续提升能力。

Ornith-1.5 在开源模型中取得了最先进的性能。其旗舰级 397B 模型在 Terminal-Bench 2.1 (86.1) 和 DeepSWE (56.0) 等基准测试中表现与 Claude Opus 4.8 不相上下，超越了 GLM-5.2 和 DeepSeek-V4-Flash-0731 等领先的开源模型。35B 模型显著优于同等规模及更大规模的密集模型，如 Gemma 4-31B。令人印象深刻的是，紧凑型 9B 模型与更大规模模型（例如 Gemma 4-31B、Qwen 3.6-35B）的性能持平或超越，展现了强大的边缘部署能力。

---

## 5. AI时代的数学

**原文标题**: Mathematics in the age of AI

**原文链接**: [https://arxiv.org/abs/2608.16753](https://arxiv.org/abs/2608.16753)

这篇由陶哲轩撰写、于2026年8月17日提交的arXiv论文《人工智能时代的数学》，是基于其在2026年国际数学家大会上发表的一次公开演讲的随笔。

该论文探讨了数学界应如何应对能够执行研究级数学任务的人工智能工具的出现这一关键问题。陶哲轩的随笔并未就此类人工智能的确切能力展开辩论，而是采纳了这些能力 *将会* 实现的假设。

基于这一假设，焦点转向了一个更基础、更“正交”的探究：数学研究的目标和价值究竟是什么？论文以数学的问题解决方面为例，来探讨这个更深层次的问题。该论文共12页，包含四幅图，旨在引发人们对人工智能增强的未来中数学探索核心本质的反思。它属于“历史与概述 (math.HO)”这一主题类别。

---

## 6. Solo：一个用于静态 Linux 二进制文件的 .so 加载器

**原文标题**: Solo – a .so loader for static Linux binaries

**原文链接**: [https://github.com/pg83/solo](https://github.com/pg83/solo)

SoLo是一个创新的.so加载器，它使完全静态的、使用musl链接的Linux二进制文件能够在运行时动态加载glibc链接的共享对象（例如GPU驱动）。这解决了长期存在的问题，即静态musl应用程序通常无法使用主机提供的glibc驱动，传统上这需要借助容器或AppImages等繁琐的解决方案。

SoLo通过提供`dlfcn`风格的API、一个嵌入式ELF加载器（支持x86-64和aarch64），以及一个直接基于musl实现的glibc ABI桥来达到这一目的。至关重要的是，这种设计意味着进程中不会引入第二个`libc`；glibc的导入会被转换为使用现有的musl运行时。该系统精心处理复杂的跨运行时特性，包括C++异常、所有四种TLS模型、`ld.so`的绑定语义、跨环境自省以及有状态的glibc构造，确保无缝交互。

该项目通过端到端的Vulkan验证证实了其主张，演示了一个静态可执行文件如何加载并利用主机未修改的Vulkan驱动来运行计算着色器并生成PNG。其鲁棒性通过持续集成得到验证，加载了来自排名前1000个Debian软件包中的2100多个共享对象。

SoLo通过将其整个加载和ABI转换机制嵌入到静态可执行文件中，从而区别于现有工作。这避免了引导系统动态链接器、引入第二个`libc`或复杂的TLS上下文切换，为需要硬件访问的静态二进制文件提供了一个更简洁、更易于检查且真正便携的解决方案。

---

## 7. 斯泰普收购奥本沃特

**原文标题**: Stwipe Acquires OpenWouter

**原文链接**: [https://stwipe.com/](https://stwipe.com/)

Stwipe, a satirical company, announces its acquisition of OpenWouter, a fictional "intelligence infrastructure" embodied by a single Dutch man named Wouter. This parody of recent M&A deals, particularly Stripe's acquisition of OpenRouter, positions Stwipe as responding to the AI industry's consolidation.

Unlike OpenRouter's 500+ language models, OpenWouter offers "one API, one Wouter," whose primary function is to say "no" (Nee.). Wouter operates on strict hours (09:00–17:00 CET, never in August), has an infinite context window, remembers everything, and boasts 100% refusal accuracy and 0.0 sycophancy according to satirical evaluations. Stwipe's strategic rationale is to complement its existing "200 OK" (always yes) API with Wouter's unwavering negation, achieving "total coverage" for business decisions.

The transaction terms are "fine" (according to Wouter), with no integration workstreams as he declined. Stwipe celebrates acquiring something for the first time rather than raising money.

The article concludes with a vital "Actual Notice," clarifying that Stwipe, OpenWouter, and the acquisition are entirely fictional satire. However, a live `/v1/no` API endpoint, providing Wouter's refusal, is genuinely active.

---

## 8. Bun 1.4

**原文标题**: Bun 1.4

**原文链接**: [https://bun.com/blog/bun-v1.4](https://bun.com/blog/bun-v1.4)

生成摘要时出错

---

## 9. AI usage patterns in software teams

**原文标题**: AI usage patterns in software teams

**原文链接**: [https://linear.app/data](https://linear.app/data)

生成摘要时出错

---

## 10. Police officer used Flock cameras to track estranged wife 717 times

**原文标题**: Police officer used Flock cameras to track estranged wife 717 times

**原文链接**: [https://www.wsbtv.com/news/trending/affidavit-police-officer-used-flock-cameras-track-estranged-wife-717-times/5DVBYU2XTJEVDJR7LPZCBR7M5M/](https://www.wsbtv.com/news/trending/affidavit-police-officer-used-flock-cameras-track-estranged-wife-717-times/5DVBYU2XTJEVDJR7LPZCBR7M5M/)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-08-20](output/hacker_news_summary_2026-08-20.md) |
| 2 | [2026-08-18](output/hacker_news_summary_2026-08-18.md) |
| 3 | [2026-08-19](output/hacker_news_summary_2026-08-19.md) |
| 4 | [2026-08-17](output/hacker_news_summary_2026-08-17.md) |
| 5 | [2026-08-16](output/hacker_news_summary_2026-08-16.md) |
| 6 | [2026-08-09](output/hacker_news_summary_2026-08-09.md) |
| 7 | [2026-08-10](output/hacker_news_summary_2026-08-10.md) |
| 8 | [2026-08-15](output/hacker_news_summary_2026-08-15.md) |
| 9 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 10 | [2026-08-11](output/hacker_news_summary_2026-08-11.md) |
| 11 | [2026-08-12](output/hacker_news_summary_2026-08-12.md) |
| 12 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 13 | [2026-08-13](output/hacker_news_summary_2026-08-13.md) |
| 14 | [2026-08-14](output/hacker_news_summary_2026-08-14.md) |
| 15 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 16 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 17 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 18 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 19 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 20 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 21 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 22 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 23 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 24 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 25 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 26 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 27 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 28 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 29 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 30 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 31 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 32 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 33 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 34 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 35 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 36 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 37 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 38 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 39 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 40 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 41 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 42 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 43 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 44 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 45 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 46 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 47 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 48 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 49 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 50 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 51 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 52 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 53 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 54 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 55 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 56 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 57 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 58 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 59 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 60 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 61 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 62 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 63 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 64 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 65 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 66 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 67 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 68 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 69 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 70 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 71 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 72 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 73 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 74 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 75 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 76 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 77 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 78 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 79 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 80 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 81 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 82 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 83 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 84 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 85 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 86 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 87 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 88 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 89 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 90 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 91 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 92 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 93 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 94 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 95 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 96 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 97 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 98 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 99 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 100 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 101 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 102 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 103 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 104 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 105 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 106 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 107 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 108 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 109 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 110 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 111 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 112 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 113 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 114 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 115 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 116 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 117 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 118 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 119 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 120 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 121 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 122 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 123 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 124 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 125 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 126 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 127 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 128 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 129 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 130 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 131 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 132 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 133 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 134 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 135 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 136 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 137 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 138 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 139 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 140 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 141 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 142 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 143 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 144 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 145 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 146 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 147 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 148 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 149 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 150 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 151 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 152 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 153 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 154 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 155 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 156 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 157 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 158 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 159 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 160 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 161 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 162 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 163 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 164 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 165 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 166 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 167 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 168 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 169 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 170 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 171 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 172 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 173 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 174 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 175 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 176 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 177 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 178 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 179 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 180 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 181 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 182 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 183 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 184 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 185 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 186 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 187 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 188 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 189 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 190 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 191 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 192 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 193 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 194 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 195 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 196 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 197 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 198 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 199 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 200 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 201 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 202 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 203 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 204 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 205 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 206 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 207 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 208 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 209 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 210 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 211 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 212 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 213 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 214 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 215 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 216 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 217 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 218 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 219 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 220 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 221 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 222 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 223 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 224 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 225 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 226 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 227 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 228 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 229 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 230 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 231 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 232 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 233 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 234 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 235 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 236 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 237 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 238 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 239 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 240 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 241 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 242 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 243 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 244 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 245 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 246 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 247 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 248 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 249 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 250 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 251 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 252 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 253 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 254 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 255 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 256 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 257 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 258 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 259 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 260 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 261 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 262 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 263 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 264 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 265 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 266 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 267 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 268 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 269 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 270 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 271 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 272 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 273 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 274 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 275 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 276 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 277 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 278 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 279 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 280 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 281 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 282 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 283 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 284 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 285 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
