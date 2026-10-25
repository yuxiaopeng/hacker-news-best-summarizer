# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-10-25.md)

*最后自动更新时间: 2026-10-25 22:00:46*
## 1. 苹果安全研究设备

**原文标题**: Apple Security Research Device

**原文链接**: [https://security.apple.com/research-device/](https://security.apple.com/research-device/)

苹果安全研究设备 (SRD) 项目旨在加速新手和经验丰富的研究人员对 iOS 的安全研究。该项目提供一款特殊熔断的 iPhone，即安全研究设备 (SRD)，可进行深度安全研究，且无需绕过其原生安全功能。

使用 SRD 的研究人员可获得 shell 访问权限，能够运行自定义工具、选择授权，甚至自定义内核。该项目还提供软件预览版、安全测试版项目、专属研究社区以及专用工具的访问权限。研究可涵盖所有 iOS 和 iPhone 组件，但不包括 Apple Pay 和第三方应用。

通过 SRD 发现的漏洞将自动纳入苹果安全赏金计划的考量范围，包括针对预览版和测试版软件的额外奖励。参与者需及时向苹果报告所有发现，并在适用情况下向相关的第三方报告。

SRD 以 12 个月可续借的借用形式提供，仍归苹果所有，且严格用于受控的安全研究。该设备不得用于个人用途，必须保留在项目参与者的场所内，访问权限仅限于苹果授权人员。

申请资格要求包括在苹果或其他现代平台上发现安全问题的良好记录、达到法定成年年龄、在过去 12 个月内未曾是苹果员工，以及居住在符合条件的国家/地区。申请截止日期为 2026 年 10 月 30 日，每年可用的设备数量有限。

---

## 2. 演变中的威胁：http2shell 是 Node、Python 等中的远程代码执行（RCE）漏洞

**原文标题**: Evolving Threat: http2shell is an RCE in Node, Python, and more

**原文链接**: [https://nitter.click/AikidoSecurity/status/2113759110625906950?__galadriel=lPmlGl9id4oAd5UeBwMhlYKArHyr6lR2IDGujPwB5HV2kQ1aLoPWFd5A9sGuzNcmrp8fUso8qygmHcKTDZ8MNHWqQ3bDJcycV87xp_0VypzQLYj6O_RRHlZuQqj33oASGY2YLSoAiMjeOZN40h7Stf8AG7DPrGZbAPVKUXy36HoMudRbvwF3_r2uYNmfJMhpKzywQDM6Ab8](https://nitter.click/AikidoSecurity/status/2113759110625906950?__galadriel=lPmlGl9id4oAd5UeBwMhlYKArHyr6lR2IDGujPwB5HV2kQ1aLoPWFd5A9sGuzNcmrp8fUso8qygmHcKTDZ8MNHWqQ3bDJcycV87xp_0VypzQLYj6O_RRHlZuQqj33oASGY2YLSoAiMjeOZN40h7Stf8AG7DPrGZbAPVKUXy36HoMudRbvwF3_r2uYNmfJMhpKzywQDM6Ab8)

The content you provided appears to be a browser security check or CAPTCHA page ("Checking your browserTo defend Nitter from evil bots, click here to continue"), not the actual article titled "Evolving Threat: http2shell is an RCE in Node, Python, and more."

Therefore, I cannot provide a summary of the article itself. Please provide the full text of the article for me to summarize.

---

## 3. 小型程序与语言

**原文标题**: Small Programs and Languages

**原文链接**: [https://ratfactor.com/cards/pl-small](https://ratfactor.com/cards/pl-small)

生成摘要时出错

---

## 4. 五个 Qwen3.8-27B 模型使用 GVS5H Harness 媲美 Fable 5

**原文标题**: Five Qwen3.8-27B models match Fable 5 Using GVS5H Harness

**原文链接**: [https://github.com/slee-persis/GVS5H](https://github.com/slee-persis/GVS5H)

GVS5H方法，也称为“大猩猩 vs. 5 个人类”，引入了基于账本的零样本自编排技术。这是一种无需训练的方法，能够让单个模型的新实例分解复杂的编码问题，并通过共享文件系统进行协作。该方法使得Qwen3.8-27B等开源模型在编码基准测试中，能够达到或超越Fable 5等前沿模型的性能。

在100个困难的LiveCodeBench问题上，GVS5H带来了显著的性能提升，最高达25.6个百分点。值得注意的是，经过编排的Qwen3.8 Flash Next实现了93.0%的pass@1，超越了Fable 5的90.4%，而成本仅为后者的9%。此外，一个在本地部署的开源Qwen3.8-27B模型将其pass@1分数从66.8%大幅提升至92.4%，有效地与Fable 5的能力持平。

该论文将这些提升归因于问题分解和持久上下文，表明推理时期的组织通过可自托管的权重，能够以一小部分成本接近甚至略微超越前沿编码准确性。尽管功能强大，但该方法并非能普遍改进所有模型。其代码已根据MIT许可开源。

---

## 5. 梦-1

**原文标题**: Dream-1

**原文链接**: [https://dreamlabs.ai/research/dream-1/](https://dreamlabs.ai/research/dream-1/)

Dream Labs已成功推出，并获得9000万美元种子轮融资，同时推出了Dream-1——一款配备平行夹爪的双臂机器人，可通过公共API在全球范围内使用。Dream-1旨在解决机器人领域长期存在的“鸡生蛋，蛋生鸡”难题：机器人需有用才能收集数据，但又需数据才能变得有用。

这一突破得益于两个因素：机器人硬件成本的迅速下降（例如，一套双臂机器人仅需2000美元）以及无需大量特定本体数据即可泛化的模型。Dream-1是一种基于DreamZero论文构建的“世界动作模型”（WAM），该论文表明30分钟的数据即可传递通用任务知识。

Dream-1提供零样本泛化能力，使其无需微调或机器学习专业知识，即可开箱即用，直接控制未知环境中的未知机器人执行未知任务。它通过预测末端执行器（EEF）姿态来工作，任何配备双臂平行夹爪的机器人都可以通过其逆运动学求解器将其转换为关节指令。WAM通过学习预测视频和动作来实现这一点，将所有机器人视为像素数据。

该服务设计为即插即用，Dream-1每小时收费3美元，Dream-1-flash每小时收费2美元。Robocurve的一份独立报告强调，与现有模型相比，Dream-1的性能“更好、更快、更便宜”。如果初始性能不尽如人意，用户还可以使用FaaS对Dream-1进行特定任务的微调。

---

## 6. Meta员工称卢拉巴西大选账号受限：报道

**原文标题**: Meta employees say Lula’s accounts restricted in Brazil election: Report

**原文链接**: [https://www.aljazeera.com/economy/2026/10/16/meta-employees-say-lulas-accounts-restricted-in-brazil-election-report](https://www.aljazeera.com/economy/2026/10/16/meta-employees-say-lulas-accounts-restricted-in-brazil-election-report)

巴西《圣保罗页报》援引内部通讯报道称，Meta员工承认，在该国大选期间，限制措施对巴西总统路易斯·伊纳西奥·卢拉·达席尔瓦的Instagram账户产生了负面影响，而据报道，挑战者参议员弗拉维奥·博索纳罗的个人资料和WhatsApp频道则获得了推荐。

Meta回应称，这些是公开的技术问题，内部讨论关注的是其严重性，而非政治干预，并明确否认存在任何偏见。

此前，卢拉曾抱怨Meta在10月25日总统决选前使用有偏见的算法和AI限制来偏袒博索纳罗。卢拉的政党指出，他的帖子有时缺少分享按钮，触达率降低，并且缺少其他互动选项。

因此，巴西最高选举法院法官马可·奥雷利奥·贝利泽命令Meta立即确保对两位候选人一视同仁。该裁决禁止Meta以造成不平衡的方式减少政治内容分发、限制搜索或删除帖子，并要求对两个竞选活动采用相同的AI标准。若不遵守，将面临每日50万雷亚尔（约合98,700美元）的罚款。

---

## 7. 鹅编程语言

**原文标题**: The Goose Programming Language

**原文链接**: [https://aardappel.github.io/goose/](https://aardappel.github.io/goose/)

Goose 编程语言是一种内存安全的系统级语言，旨在实现卓越性能和低内存消耗，据报道在基准测试中超越了 C++ 和 Rust。其创新的内存模型完全依赖于编译器管理的数据栈，从而消除了堆分配器、垃圾回收器、引用计数和显式生命周期注解。内存在其作用域结束时自动释放，动态增长操作从不移动数据，从而确保引用始终有效。

Goose 通过静态推断引用根来实现内存安全，无需 `unsafe` 块或生命周期语法即可防止悬空引用。复杂数据结构，包括可变大小数组、字符串和带动态字段的记录，均以连续内联方式存储，无需指针，这使得许多类型实现零分配并有效利用缓存。可变模式枚举 (Enums) 通过以其实际大小存储变体，进一步优化内存。

其他主要特性包括用于高效序列化的窄的、与位置无关的相对引用，以及保证的就地值构造以避免复制。一种独特的错误处理机制，即 `return E from f`，允许沿调用栈进行静态的、检查过的返回，而无需 `Result` 类型。线程通过带 `memcpy` 的类型化队列进行通信，无需共享内存、锁或原子操作即可运行。泛型和高阶函数是编译时实体，经单态化处理后运行时开销为零。Goose 编译为 C 语言，提供广泛的兼容性。其语法对于 C 和 Rust 程序员来说很熟悉。

---

## 8. 1505年纽伦堡骑士工具书

**原文标题**: Tool book of a Nuremberg knight from 1505

**原文链接**: [https://loeffelholz-codex.org/en/](https://loeffelholz-codex.org/en/)

生成摘要时出错

---

## 9. AI use leads UC Berkeley math professor to see 'no point' in grading homework

**原文标题**: AI use leads UC Berkeley math professor to see 'no point' in grading homework

**原文链接**: [https://www.dailycal.org/news/campus/academics/ai-use-leads-uc-berkeley-math-professor-to-see-no-point-in-grading-homework/article_bdf1eae2-c08b-491f-b9f1-81a7cea177de.html](https://www.dailycal.org/news/campus/academics/ai-use-leads-uc-berkeley-math-professor-to-see-no-point-in-grading-homework/article_bdf1eae2-c08b-491f-b9f1-81a7cea177de.html)

生成摘要时出错

---

## 10. Show HN: 我把员工放进标普500市值气泡中

**原文标题**: Show HN: I put employees inside S&P 500 market-cap bubbles

**原文链接**: [https://bigwhalehunting.com/workforce/](https://bigwhalehunting.com/workforce/)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-10-25](output/hacker_news_summary_2026-10-25.md) |
| 2 | [2026-10-23](output/hacker_news_summary_2026-10-23.md) |
| 3 | [2026-10-22](output/hacker_news_summary_2026-10-22.md) |
| 4 | [2026-10-24](output/hacker_news_summary_2026-10-24.md) |
| 5 | [2026-10-21](output/hacker_news_summary_2026-10-21.md) |
| 6 | [2026-10-20](output/hacker_news_summary_2026-10-20.md) |
| 7 | [2026-10-17](output/hacker_news_summary_2026-10-17.md) |
| 8 | [2026-10-18](output/hacker_news_summary_2026-10-18.md) |
| 9 | [2026-10-15](output/hacker_news_summary_2026-10-15.md) |
| 10 | [2026-10-16](output/hacker_news_summary_2026-10-16.md) |
| 11 | [2026-10-19](output/hacker_news_summary_2026-10-19.md) |
| 12 | [2026-10-13](output/hacker_news_summary_2026-10-13.md) |
| 13 | [2026-10-07](output/hacker_news_summary_2026-10-07.md) |
| 14 | [2026-10-14](output/hacker_news_summary_2026-10-14.md) |
| 15 | [2026-10-10](output/hacker_news_summary_2026-10-10.md) |
| 16 | [2026-10-09](output/hacker_news_summary_2026-10-09.md) |
| 17 | [2026-10-11](output/hacker_news_summary_2026-10-11.md) |
| 18 | [2026-10-01](output/hacker_news_summary_2026-10-01.md) |
| 19 | [2026-09-29](output/hacker_news_summary_2026-09-29.md) |
| 20 | [2026-10-06](output/hacker_news_summary_2026-10-06.md) |
| 21 | [2026-10-04](output/hacker_news_summary_2026-10-04.md) |
| 22 | [2026-09-30](output/hacker_news_summary_2026-09-30.md) |
| 23 | [2026-10-02](output/hacker_news_summary_2026-10-02.md) |
| 24 | [2026-10-03](output/hacker_news_summary_2026-10-03.md) |
| 25 | [2026-09-24](output/hacker_news_summary_2026-09-24.md) |
| 26 | [2026-09-21](output/hacker_news_summary_2026-09-21.md) |
| 27 | [2026-09-23](output/hacker_news_summary_2026-09-23.md) |
| 28 | [2026-09-27](output/hacker_news_summary_2026-09-27.md) |
| 29 | [2026-09-22](output/hacker_news_summary_2026-09-22.md) |
| 30 | [2026-09-25](output/hacker_news_summary_2026-09-25.md) |
| 31 | [2026-09-20](output/hacker_news_summary_2026-09-20.md) |
| 32 | [2026-09-16](output/hacker_news_summary_2026-09-16.md) |
| 33 | [2026-09-17](output/hacker_news_summary_2026-09-17.md) |
| 34 | [2026-09-19](output/hacker_news_summary_2026-09-19.md) |
| 35 | [2026-09-18](output/hacker_news_summary_2026-09-18.md) |
| 36 | [2026-09-09](output/hacker_news_summary_2026-09-09.md) |
| 37 | [2026-09-10](output/hacker_news_summary_2026-09-10.md) |
| 38 | [2026-09-13](output/hacker_news_summary_2026-09-13.md) |
| 39 | [2026-09-14](output/hacker_news_summary_2026-09-14.md) |
| 40 | [2026-09-11](output/hacker_news_summary_2026-09-11.md) |
| 41 | [2026-09-12](output/hacker_news_summary_2026-09-12.md) |
| 42 | [2026-09-15](output/hacker_news_summary_2026-09-15.md) |
| 43 | [2026-09-03](output/hacker_news_summary_2026-09-03.md) |
| 44 | [2026-09-02](output/hacker_news_summary_2026-09-02.md) |
| 45 | [2026-09-04](output/hacker_news_summary_2026-09-04.md) |
| 46 | [2026-09-08](output/hacker_news_summary_2026-09-08.md) |
| 47 | [2026-09-05](output/hacker_news_summary_2026-09-05.md) |
| 48 | [2026-09-07](output/hacker_news_summary_2026-09-07.md) |
| 49 | [2026-09-06](output/hacker_news_summary_2026-09-06.md) |
| 50 | [2026-08-31](output/hacker_news_summary_2026-08-31.md) |
| 51 | [2026-08-28](output/hacker_news_summary_2026-08-28.md) |
| 52 | [2026-09-01](output/hacker_news_summary_2026-09-01.md) |
| 53 | [2026-08-29](output/hacker_news_summary_2026-08-29.md) |
| 54 | [2026-08-30](output/hacker_news_summary_2026-08-30.md) |
| 55 | [2026-08-26](output/hacker_news_summary_2026-08-26.md) |
| 56 | [2026-08-22](output/hacker_news_summary_2026-08-22.md) |
| 57 | [2026-08-25](output/hacker_news_summary_2026-08-25.md) |
| 58 | [2026-08-19](output/hacker_news_summary_2026-08-19.md) |
| 59 | [2026-08-20](output/hacker_news_summary_2026-08-20.md) |
| 60 | [2026-08-17](output/hacker_news_summary_2026-08-17.md) |
| 61 | [2026-08-23](output/hacker_news_summary_2026-08-23.md) |
| 62 | [2026-08-18](output/hacker_news_summary_2026-08-18.md) |
| 63 | [2026-08-21](output/hacker_news_summary_2026-08-21.md) |
| 64 | [2026-08-24](output/hacker_news_summary_2026-08-24.md) |
| 65 | [2026-08-12](output/hacker_news_summary_2026-08-12.md) |
| 66 | [2026-08-11](output/hacker_news_summary_2026-08-11.md) |
| 67 | [2026-08-14](output/hacker_news_summary_2026-08-14.md) |
| 68 | [2026-08-16](output/hacker_news_summary_2026-08-16.md) |
| 69 | [2026-08-10](output/hacker_news_summary_2026-08-10.md) |
| 70 | [2026-08-15](output/hacker_news_summary_2026-08-15.md) |
| 71 | [2026-08-13](output/hacker_news_summary_2026-08-13.md) |
| 72 | [2026-08-09](output/hacker_news_summary_2026-08-09.md) |
| 73 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 74 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 75 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 76 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 77 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 78 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 79 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 80 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 81 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 82 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 83 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 84 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 85 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 86 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 87 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 88 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 89 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 90 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 91 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 92 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 93 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 94 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 95 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 96 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 97 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 98 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 99 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 100 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 101 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 102 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 103 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 104 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 105 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 106 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 107 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 108 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 109 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 110 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 111 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 112 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 113 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 114 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 115 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 116 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 117 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 118 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 119 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 120 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 121 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 122 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 123 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 124 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 125 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 126 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 127 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 128 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 129 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 130 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 131 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 132 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 133 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 134 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 135 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 136 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 137 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 138 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 139 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 140 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 141 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 142 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 143 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 144 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 145 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 146 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 147 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 148 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 149 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 150 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 151 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 152 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 153 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 154 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 155 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 156 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 157 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 158 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 159 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 160 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 161 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 162 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 163 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 164 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 165 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 166 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 167 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 168 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 169 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 170 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 171 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 172 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 173 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 174 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 175 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 176 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 177 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 178 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 179 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 180 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 181 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 182 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 183 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 184 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 185 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 186 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 187 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 188 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 189 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 190 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 191 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 192 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 193 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 194 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 195 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 196 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 197 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 198 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 199 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 200 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 201 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 202 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 203 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 204 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 205 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 206 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 207 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 208 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 209 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 210 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 211 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 212 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 213 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 214 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 215 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 216 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 217 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 218 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 219 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 220 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 221 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 222 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 223 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 224 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 225 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 226 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 227 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 228 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 229 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 230 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 231 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 232 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 233 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 234 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 235 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 236 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 237 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 238 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 239 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 240 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 241 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 242 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 243 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 244 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 245 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 246 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 247 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 248 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 249 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 250 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 251 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 252 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 253 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 254 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 255 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 256 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 257 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 258 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 259 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 260 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 261 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 262 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 263 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 264 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 265 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 266 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 267 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 268 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 269 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 270 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 271 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 272 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 273 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 274 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 275 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 276 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 277 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 278 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 279 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 280 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 281 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 282 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 283 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 284 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 285 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 286 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 287 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 288 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 289 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 290 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 291 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 292 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 293 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 294 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 295 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 296 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 297 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 298 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 299 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 300 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 301 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 302 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 303 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 304 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 305 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 306 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 307 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 308 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 309 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 310 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 311 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 312 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 313 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 314 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 315 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 316 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 317 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 318 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 319 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 320 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 321 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 322 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 323 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 324 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 325 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 326 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 327 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 328 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 329 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 330 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 331 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 332 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 333 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 334 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 335 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 336 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 337 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 338 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 339 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 340 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 341 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
| 342 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 343 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 344 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 345 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
