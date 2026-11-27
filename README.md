# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-11-27.md)

*最后自动更新时间: 2026-11-27 02:28:59*
## 1. 我靠，我靠，我靠，我靠：现在所发生的一切的规模

**原文标题**: Holy shit holy shit holy shit holy shit: The magnitude of what’s now happening

**原文链接**: [https://scottaaronson.blog/?p=10379](https://scottaaronson.blog/?p=10379)

斯科特·阿伦森对人工智能驱动的数学突破接连涌现深感震惊。他重点提到了几项主要证明：OpenAI 和 Anthropic 证明了 VP ≠ VNP，Alpöge/Anthropic 证明了黎曼猜想，以及 OpenAI 确定矩阵乘法指数 (ω) 恰好是 9/4（至关重要的是，这还包含一个下界）。此外，OpenAI 还找到了傅里叶变换的精确线性门计数，包括一个新的下界。

阿伦森强调，这些并非渐进式的发现，而是对长期未解之谜的直接解答，代表着“数学真理的新大陆”。他将这种体验比作早期通过显微镜或望远镜获得的科学启示。他现在认为 P ≠ NP 的证明指日可待，并表示人工智能正在“攀登”这座山峰。

作者强烈呼吁不要否认这些进步，指出经过 Lean 认证的证明是可靠的验证。他驳斥了那些质疑证明有效性（尽管有形式化验证）或要求即时日常相关性的批评者，认为如此强大的人工智能的存在对世界经济、潜在的密码系统漏洞甚至生存风险都具有惊人的影响，并将当前时期比作“AI 奇点”的开端。他强调这些发展在智力上的巨大意义，远超对比特币安全等具体担忧。

---

## 2. 1Password 安全事件

**原文标题**: 1Password Security Incident

**原文链接**: [https://1password.com/blog/update-on-nov-2026-security-incident](https://1password.com/blog/update-on-nov-2026-security-incident)

2026年11月19日，1Password发现一起安全事件，攻击者获取了一名员工的企业GitHub账户的访问权限。攻击者利用此权限下载了源代码，向后端服务推送了恶意代码，并因此下载了与部分客户相关的管理数据。

受影响的信息包括客户姓名、电子邮件地址、账户和用户标识符、账户创建/上次登录时间、公钥、安全远程密码协议参数、某些用于邀请/账户恢复的电子邮件链接中的令牌，以及其他非秘密的内部元数据。攻击者还从私人代码库中复制了源代码，并访问了包含基础设施相关秘密的CI/CD系统。少数拥有活跃配置或恢复邀请令牌的用户已收到特别通知。

关键的是，客户保险库内容、保护保险库的密钥、用户账户密码、秘密密钥以及账户恢复密钥均**未**被访问或受到影响。1Password强调其不存储用户密码或秘密密钥，且保险库内容仍由用户持有的密钥加密，攻击者无法访问。

作为回应，1Password禁用了被入侵的GitHub账户，撤销了被盗令牌，轮换了所有可能已暴露的内部凭据，并将邀请/恢复代码从六位增加到十位字母数字字符，以防止暴力破解。他们还加强了内部控制，增加了新的检测机制，确认没有用户账户被接管，并聘请了独立的网络安全专家。

建议用户警惕提及1Password、邀请或账户恢复的网络钓鱼尝试（电子邮件、短信、电话）。用户应仅在官方1Password应用程序或网站中输入凭据，并向support@1password.com报告任何可疑活动。

---

## 3. 矩阵乘法指数是四分之九 [pdf]

**原文标题**: The matrix multiplication exponent is nine fourths [pdf]

**原文链接**: [https://github.com/openai/math/blob/main/preprints/The-matrix-multiplication-exponent-is-nine-fourths-November-24-2026/paper.pdf](https://github.com/openai/math/blob/main/preprints/The-matrix-multiplication-exponent-is-nine-fourths-November-24-2026/paper.pdf)

仅从标题《矩阵乘法指数是九分之四》来看，本文声称矩阵乘法指数（常用ω表示）取得了突破性的新上限。具体来说，它断言ω至多为四分之九 (9/4)，即2.25。

矩阵乘法指数是理论计算机科学中的一个基本参数，代表着两个n x n矩阵相乘时，渐进运行时间O(n^ω)中可能达到的最小指数。几十年来，研究人员一直致力于降低这个指数，目前已知的最佳上限略高于2.3728。

降至2.25将代表一个非常重大的飞跃，大幅改进了施特拉森算法 (log2(7) ≈ 2.807) 和Coppersmith-Winograd算法 (≈ 2.376) 等先前的结果。它将使指数更接近于2这个推测的最佳值。如果这一主张得到证实，将对众多依赖矩阵乘法作为子程序的算法效率产生深远影响，从而惠及图论、科学计算和复杂性理论等领域。该文章很可能详细介绍了为实现这一前所未有的降低而采用的新颖算法技术或理论进展。这样的发现将是计算复杂性领域的一个重大突破。

---

## 4. 按钮音效 – 专业录制的按钮点击与按压声合集

**原文标题**: Button Sounds – collection of professionally-recorded button clicks and presses

**原文链接**: [https://buttons.joshwcomeau.com/](https://buttons.joshwcomeau.com/)

本文介绍“按钮音效”，一套专业录制的音效合集。它包含各种按钮点击和按压声，被描述为专为用户界面（UI）设计的“触觉音效”。这套合集提供高质量的音频反馈，以提升用户体验。

---

## 5. 纽约时报警告摄影师不要为了AI功能更新Photoshop。

**原文标题**: The New York Times warns photographers not to update Photoshop over AI features

**原文链接**: [https://www.theverge.com/ai-artificial-intelligence/1041227/the-new-york-times-warns-photographers-not-to-update-photoshop-over-ai-features](https://www.theverge.com/ai-artificial-intelligence/1041227/the-new-york-times-warns-photographers-not-to-update-photoshop-over-ai-features)

《纽约时报》正建议其自由摄影师避免更新至Adobe Photoshop 2027，原因是担心新的AI功能可能会嵌入元数据，将照片标记为AI生成。这对此报严格禁止大幅度照片篡改的编辑政策构成了威胁，而该政策旨在维护读者信任。

最新Photoshop更新（28.0.0版本）引入了多项AI驱动工具，包括“AI辅助编辑器”、基于提示的编辑、AI放大和图像重构。《时报》担心，即使是这些工具的轻微或“不明显”使用，也可能触发元数据标签，尤其是在Adobe正推广C2PA元数据以表明AI生成或AI编辑内容的情况下。

鉴于《时报》承诺照片除了最基本的色彩调整外不进行“修饰或数字处理”，无意中产生的AI元数据可能会暗示存在广泛的篡改，从而损害其视觉新闻的完整性。因此，《纽约时报》要求所有投稿摄影师在执行任务时避免使用Photoshop 2027及后续更新，这一政策已得到报社确认。引起担忧的具体AI功能并未完全公布，但目的是防止任何可能歪曲照片原创性的元数据。

---

## 6. Much shorter version of GRH Lean verification from Anthropic

**原文标题**: Much shorter version of GRH Lean verification from Anthropic

**原文链接**: [https://github.com/lsernau/grh-lean](https://github.com/lsernau/grh-lean)

This artifact presents a Lean 4 proof of the Riemann Hypothesis and the Generalized Riemann Hypothesis (GRH) for Dirichlet L-functions. Developed by Anthropic colleagues and Claude, it's a "much shorter version" based on Levent Alpöge's work.

The proof is built on Mathlib and adheres to strict axiomatic foundations, using only `propext`, `Classical.choice`, and `Quot.sound`. Two editions are provided: a readable `grh/` at about 300,000 lines, and a compact `grh-compact/` at approximately 76,000 lines, both proving the same five theorems.

To build, users need Lean v4.35.0 and a specific Mathlib commit. The process can take 1-2 hours on a 12-core machine with 24 GB of memory.

Crucially, the proof has only undergone machine checks. It has not been reviewed by human mathematicians, and no accompanying paper has been released. The project is licensed under Apache 2.0, Copyright 2026 Anthropic, PBC, and is explicitly stated as not maintained or accepting contributions.

---

## 7. 有传闻称，实验室可能已攻克了多项式时间因数分解问题。

**原文标题**: Rumors swirling that labs might have cracked Factoring in P

**原文链接**: [https://www.reddit.com/r/singularity/comments/1y59ef1/rumor_that_openai_or_anthropic_found_a_way_to/](https://www.reddit.com/r/singularity/comments/1y59ef1/rumor_that_openai_or_anthropic_found_a_way_to/)

A Reddit thread titled "Rumors swirling that labs might have cracked Factoring in P" discusses speculative claims that major AI labs like OpenAI or Anthropic may have found a polynomial-time algorithm for integer factorization. This would be a monumental breakthrough, effectively rendering much of modern public-key cryptography (like RSA) obsolete, as its security relies on the computational difficulty of factoring large numbers.

The thread's original post is highly speculative, admitting the rumor is "wild" and unsubstantiated. Commenters widely express extreme skepticism, highlighting several reasons why such a rumor is unlikely to be true, or at least public in this manner:
*   **Secrecy:** A discovery of this magnitude would likely be classified or kept under wraps by governments or the discovering entity due to its profound implications for national security and global finance.
*   **Verification:** The mathematical community would demand rigorous proof, and such a discovery would likely be published in academic journals, not leaked as a vague rumor on Reddit.
*   **Difficulty:** Factoring in P is a long-standing, extremely difficult problem in computer science and mathematics; a solution would fundamentally alter the field.
*   **Alternative Explanations:** Some suggest the rumor might stem from misinterpretations of progress in quantum computing (Shor's algorithm *can* factor in polynomial time, but requires a fault-tolerant quantum computer, which doesn't yet exist at scale), or simply be a false alarm designed to create buzz.

While acknowledging the "singularity" sub-reddit often deals with speculative ideas, the overwhelming consensus within the thread is that the rumor is almost certainly false, or at best, grossly exaggerated, lacking any credible evidence.

---

## 8. Google releases Cogentic papers on integer factorization, discrete logs and more

**原文标题**: Google releases Cogentic papers on integer factorization, discrete logs and more

**原文链接**: [https://github.com/google-research/google-research/tree/master/cogentic_research_papers](https://github.com/google-research/google-research/tree/master/cogentic_research_papers)

生成摘要时出错

---

## 9. A few questions for the guy who went snorkeling in a Home Depot retention pond

**原文标题**: A few questions for the guy who went snorkeling in a Home Depot retention pond

**原文链接**: [https://www.vox.com/down-to-earth/511999/home-depot-retention-pond-snorkel-joseph-ricketts](https://www.vox.com/down-to-earth/511999/home-depot-retention-pond-snorkel-joseph-ricketts)

生成摘要时出错

---

## 10. Intel One Mono font (2023)

**原文标题**: Intel One Mono font (2023)

**原文链接**: [https://github.com/intel/intel-one-mono](https://github.com/intel/intel-one-mono)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-11-27](output/hacker_news_summary_2026-11-27.md) |
| 2 | [2026-11-24](output/hacker_news_summary_2026-11-24.md) |
| 3 | [2026-11-25](output/hacker_news_summary_2026-11-25.md) |
| 4 | [2026-11-26](output/hacker_news_summary_2026-11-26.md) |
| 5 | [2026-11-23](output/hacker_news_summary_2026-11-23.md) |
| 6 | [2026-11-19](output/hacker_news_summary_2026-11-19.md) |
| 7 | [2026-11-22](output/hacker_news_summary_2026-11-22.md) |
| 8 | [2026-11-21](output/hacker_news_summary_2026-11-21.md) |
| 9 | [2026-11-18](output/hacker_news_summary_2026-11-18.md) |
| 10 | [2026-11-20](output/hacker_news_summary_2026-11-20.md) |
| 11 | [2026-11-14](output/hacker_news_summary_2026-11-14.md) |
| 12 | [2026-11-15](output/hacker_news_summary_2026-11-15.md) |
| 13 | [2026-11-12](output/hacker_news_summary_2026-11-12.md) |
| 14 | [2026-11-13](output/hacker_news_summary_2026-11-13.md) |
| 15 | [2026-11-17](output/hacker_news_summary_2026-11-17.md) |
| 16 | [2026-11-07](output/hacker_news_summary_2026-11-07.md) |
| 17 | [2026-11-06](output/hacker_news_summary_2026-11-06.md) |
| 18 | [2026-11-11](output/hacker_news_summary_2026-11-11.md) |
| 19 | [2026-11-08](output/hacker_news_summary_2026-11-08.md) |
| 20 | [2026-11-05](output/hacker_news_summary_2026-11-05.md) |
| 21 | [2026-11-10](output/hacker_news_summary_2026-11-10.md) |
| 22 | [2026-11-01](output/hacker_news_summary_2026-11-01.md) |
| 23 | [2026-11-03](output/hacker_news_summary_2026-11-03.md) |
| 24 | [2026-10-31](output/hacker_news_summary_2026-10-31.md) |
| 25 | [2026-10-30](output/hacker_news_summary_2026-10-30.md) |
| 26 | [2026-11-04](output/hacker_news_summary_2026-11-04.md) |
| 27 | [2026-10-24](output/hacker_news_summary_2026-10-24.md) |
| 28 | [2026-10-23](output/hacker_news_summary_2026-10-23.md) |
| 29 | [2026-10-25](output/hacker_news_summary_2026-10-25.md) |
| 30 | [2026-10-27](output/hacker_news_summary_2026-10-27.md) |
| 31 | [2026-10-28](output/hacker_news_summary_2026-10-28.md) |
| 32 | [2026-10-26](output/hacker_news_summary_2026-10-26.md) |
| 33 | [2026-10-29](output/hacker_news_summary_2026-10-29.md) |
| 34 | [2026-10-19](output/hacker_news_summary_2026-10-19.md) |
| 35 | [2026-10-18](output/hacker_news_summary_2026-10-18.md) |
| 36 | [2026-10-21](output/hacker_news_summary_2026-10-21.md) |
| 37 | [2026-10-22](output/hacker_news_summary_2026-10-22.md) |
| 38 | [2026-10-20](output/hacker_news_summary_2026-10-20.md) |
| 39 | [2026-10-17](output/hacker_news_summary_2026-10-17.md) |
| 40 | [2026-10-13](output/hacker_news_summary_2026-10-13.md) |
| 41 | [2026-10-11](output/hacker_news_summary_2026-10-11.md) |
| 42 | [2026-10-15](output/hacker_news_summary_2026-10-15.md) |
| 43 | [2026-10-14](output/hacker_news_summary_2026-10-14.md) |
| 44 | [2026-10-16](output/hacker_news_summary_2026-10-16.md) |
| 45 | [2026-10-03](output/hacker_news_summary_2026-10-03.md) |
| 46 | [2026-10-09](output/hacker_news_summary_2026-10-09.md) |
| 47 | [2026-10-07](output/hacker_news_summary_2026-10-07.md) |
| 48 | [2026-10-10](output/hacker_news_summary_2026-10-10.md) |
| 49 | [2026-10-06](output/hacker_news_summary_2026-10-06.md) |
| 50 | [2026-10-04](output/hacker_news_summary_2026-10-04.md) |
| 51 | [2026-10-02](output/hacker_news_summary_2026-10-02.md) |
| 52 | [2026-09-29](output/hacker_news_summary_2026-09-29.md) |
| 53 | [2026-09-30](output/hacker_news_summary_2026-09-30.md) |
| 54 | [2026-09-25](output/hacker_news_summary_2026-09-25.md) |
| 55 | [2026-09-27](output/hacker_news_summary_2026-09-27.md) |
| 56 | [2026-10-01](output/hacker_news_summary_2026-10-01.md) |
| 57 | [2026-09-24](output/hacker_news_summary_2026-09-24.md) |
| 58 | [2026-09-21](output/hacker_news_summary_2026-09-21.md) |
| 59 | [2026-09-23](output/hacker_news_summary_2026-09-23.md) |
| 60 | [2026-09-20](output/hacker_news_summary_2026-09-20.md) |
| 61 | [2026-09-22](output/hacker_news_summary_2026-09-22.md) |
| 62 | [2026-09-18](output/hacker_news_summary_2026-09-18.md) |
| 63 | [2026-09-19](output/hacker_news_summary_2026-09-19.md) |
| 64 | [2026-09-14](output/hacker_news_summary_2026-09-14.md) |
| 65 | [2026-09-17](output/hacker_news_summary_2026-09-17.md) |
| 66 | [2026-09-16](output/hacker_news_summary_2026-09-16.md) |
| 67 | [2026-09-15](output/hacker_news_summary_2026-09-15.md) |
| 68 | [2026-09-12](output/hacker_news_summary_2026-09-12.md) |
| 69 | [2026-09-13](output/hacker_news_summary_2026-09-13.md) |
| 70 | [2026-09-08](output/hacker_news_summary_2026-09-08.md) |
| 71 | [2026-09-11](output/hacker_news_summary_2026-09-11.md) |
| 72 | [2026-09-09](output/hacker_news_summary_2026-09-09.md) |
| 73 | [2026-09-10](output/hacker_news_summary_2026-09-10.md) |
| 74 | [2026-09-05](output/hacker_news_summary_2026-09-05.md) |
| 75 | [2026-09-01](output/hacker_news_summary_2026-09-01.md) |
| 76 | [2026-09-02](output/hacker_news_summary_2026-09-02.md) |
| 77 | [2026-09-06](output/hacker_news_summary_2026-09-06.md) |
| 78 | [2026-09-03](output/hacker_news_summary_2026-09-03.md) |
| 79 | [2026-09-07](output/hacker_news_summary_2026-09-07.md) |
| 80 | [2026-09-04](output/hacker_news_summary_2026-09-04.md) |
| 81 | [2026-08-29](output/hacker_news_summary_2026-08-29.md) |
| 82 | [2026-08-24](output/hacker_news_summary_2026-08-24.md) |
| 83 | [2026-08-25](output/hacker_news_summary_2026-08-25.md) |
| 84 | [2026-08-30](output/hacker_news_summary_2026-08-30.md) |
| 85 | [2026-08-26](output/hacker_news_summary_2026-08-26.md) |
| 86 | [2026-08-31](output/hacker_news_summary_2026-08-31.md) |
| 87 | [2026-08-28](output/hacker_news_summary_2026-08-28.md) |
| 88 | [2026-08-23](output/hacker_news_summary_2026-08-23.md) |
| 89 | [2026-08-20](output/hacker_news_summary_2026-08-20.md) |
| 90 | [2026-08-16](output/hacker_news_summary_2026-08-16.md) |
| 91 | [2026-08-22](output/hacker_news_summary_2026-08-22.md) |
| 92 | [2026-08-18](output/hacker_news_summary_2026-08-18.md) |
| 93 | [2026-08-17](output/hacker_news_summary_2026-08-17.md) |
| 94 | [2026-08-15](output/hacker_news_summary_2026-08-15.md) |
| 95 | [2026-08-21](output/hacker_news_summary_2026-08-21.md) |
| 96 | [2026-08-19](output/hacker_news_summary_2026-08-19.md) |
| 97 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 98 | [2026-08-11](output/hacker_news_summary_2026-08-11.md) |
| 99 | [2026-08-10](output/hacker_news_summary_2026-08-10.md) |
| 100 | [2026-08-12](output/hacker_news_summary_2026-08-12.md) |
| 101 | [2026-08-14](output/hacker_news_summary_2026-08-14.md) |
| 102 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 103 | [2026-08-09](output/hacker_news_summary_2026-08-09.md) |
| 104 | [2026-08-13](output/hacker_news_summary_2026-08-13.md) |
| 105 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 106 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 107 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 108 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 109 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 110 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 111 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 112 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 113 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 114 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 115 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 116 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 117 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 118 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 119 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 120 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 121 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 122 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 123 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 124 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 125 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 126 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 127 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 128 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 129 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 130 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 131 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 132 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 133 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 134 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 135 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 136 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 137 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 138 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 139 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 140 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 141 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 142 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 143 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 144 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 145 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 146 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 147 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 148 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 149 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 150 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 151 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 152 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 153 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 154 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 155 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 156 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 157 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 158 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 159 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 160 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 161 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 162 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 163 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 164 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 165 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 166 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 167 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 168 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 169 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 170 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 171 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 172 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 173 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 174 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 175 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 176 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 177 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 178 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 179 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 180 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 181 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 182 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 183 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 184 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 185 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 186 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 187 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 188 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 189 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 190 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 191 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 192 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 193 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 194 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 195 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 196 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 197 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 198 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 199 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 200 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 201 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 202 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 203 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 204 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 205 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 206 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 207 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 208 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 209 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 210 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 211 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 212 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 213 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 214 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 215 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 216 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 217 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 218 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 219 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 220 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 221 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 222 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 223 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 224 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 225 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 226 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 227 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 228 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 229 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 230 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 231 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 232 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 233 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 234 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 235 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 236 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 237 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 238 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 239 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 240 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 241 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 242 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 243 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 244 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 245 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 246 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 247 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 248 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 249 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 250 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 251 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 252 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 253 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 254 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 255 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 256 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 257 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 258 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 259 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 260 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 261 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 262 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 263 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 264 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 265 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 266 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 267 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 268 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 269 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 270 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 271 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 272 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 273 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 274 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 275 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 276 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 277 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 278 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 279 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 280 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 281 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 282 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 283 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 284 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 285 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 286 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 287 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 288 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 289 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 290 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 291 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 292 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 293 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 294 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 295 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 296 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 297 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 298 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 299 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 300 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 301 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 302 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 303 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 304 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 305 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 306 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 307 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 308 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 309 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 310 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 311 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 312 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 313 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 314 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 315 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 316 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 317 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 318 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 319 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 320 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 321 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 322 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 323 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 324 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 325 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 326 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 327 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 328 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 329 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 330 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 331 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 332 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 333 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 334 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 335 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 336 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 337 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 338 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 339 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 340 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 341 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 342 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 343 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 344 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 345 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 346 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 347 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 348 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 349 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 350 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 351 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 352 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 353 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 354 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 355 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 356 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 357 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 358 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 359 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 360 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 361 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 362 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 363 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 364 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 365 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 366 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 367 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 368 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 369 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 370 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 371 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 372 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 373 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 374 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 375 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
