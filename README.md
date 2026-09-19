# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-09-19.md)

*最后自动更新时间: 2026-09-19 21:48:11*
## 1. AI生成的海报不必糟糕

**原文标题**: AI-generated posters don’t have to be horrible

**原文链接**: [https://john.hartnup.uk/2026/06/07/ai-event-posters.html](https://john.hartnup.uk/2026/06/07/ai-event-posters.html)

文章探讨了普遍存在的“千篇一律”的AI生成海报问题，这些海报尽管“尚可”，但因其重复、同质化的风格而令人感到恼火。作者在观察了无数平淡无奇的乡村集市和啤酒节海报后，旨在证明像ChatGPT这样的AI模型能够实现远超预期的风格多样性。

作者虚构了活动细节，最初提示ChatGPT生成一张“简洁、不花哨、明亮”的春季集市海报，但结果仍然显得千篇一律。意识到需要更具体的指导后，作者随后要求一个“完全不同的设计美学”，从而得到了一张引人注目的“包豪斯/几何现代主义”海报。ChatGPT令人印象深刻地解释了它选择的风格，并在被问及时，提供了一份包含多种设计美学的全面列表，从“孔版印刷风格”、“野兽派平面设计”到“日式极简海报”、“90年代锐舞传单”等。

作者随后通过明确要求这些风格，成功生成了许多风格迥异的海报，甚至尝试了诸如“一位专业平面设计师为他年幼孩子的水粉画添加了排版”这样奇特的提示词。这项实验表明，通过提供具体、描述性的风格提示词，用户可以引导AI生成独特、有特色的设计，从而避免常见、被过度使用的审美风格。核心信息是，AI生成的海报“不必糟糕”，也不必“与众相同”，鼓励用户通过详细的指令来利用AI的多功能性。

---

## 2. 安卓17是自3.x以来，第一个未发布到AOSP就添加新API的版本。

**原文标题**: Android 17 is the first since 3.x to add new APIs without releasing to the AOSP

**原文链接**: [https://grapheneos.social/@GrapheneOS/117282080803799576](https://grapheneos.social/@GrapheneOS/117282080803799576)

GrapheneOS 已在 Mastodon 上宣布，Android 17 QPR1 代表着谷歌 Android 开发策略上的一个重大转变。GrapheneOS 表示，这是自 Android 3.x (Honeycomb) 以来，首次在引入新 API 的同时，没有将其同步发布到 Android 开放源代码项目 (AOSP)。

此举意味着 Android 17 QPR1 中的某些新功能或特性将不会成为自定义 ROM 和其他 AOSP 衍生项目所依赖的开源基础的一部分。这可能导致谷歌官方 Android 与开源社区之间出现更大的分歧，使得替代的 Android 实现若不依赖谷歌专有组件，将更难保持功能对等。

---

## 3. 我一年前用强化学习构建了非自回归决策模型。

**原文标题**: I built non-autoregressive decision models with RL a year ago

**原文链接**: [https://laya.convaiinnovations.com/](https://laya.convaiinnovations.com/)

作者详细阐述了他们对当前非自回归决策模型热潮的沮丧和认同，因为他们在一年前就已经构建并开源了类似的系统，包括arXiv论文（2025年3月、2025年9月）和公开发布的模型。他们认为，将生成式大型语言模型（LLM）用于简单、结构化的“系统1”反射性决策（如路由工单或垃圾邮件检测）效率低下、速度缓慢、成本高昂，且容易产生未经校准的幻觉。

针对专有产品TypeSafe AI的Jev，作者开发了Laya：一个开源（Apache 2.0许可）、横向的系统1决策模型家族。Laya由用于校准决策的强化学习（RLCD）指导，利用双向编码器以闪电般的速度提供针对结构化模式的校准概率预测。它从不生成文本，从而消除了幻觉和模式违规，并依赖于三个基本操作：`choice`（选择）、`score`（评分）和 `noul`（布尔值）。

Laya拥有32.8毫秒的执行速度（批处理时每问题7.2毫秒），比Jev快6到8倍。一个关键创新是其亚毫秒级路由器，它检查输入脚本，自动将文本导向三个专用检查点之一（英语、多语言或类型化决策），解决了LLM在不同语言和脚本之间置信度不可靠的问题。

基准测试表明，Laya在准确性、校准和延迟方面显著优于Jev（单问题快7.8倍，批处理快20倍），同时免费、开源且支持气隙隔离。尽管功能强大，Laya也有局限性：选择问题在20个选项以下效果最佳，需要进行微调，且温度校准可以提高性能。作者总结道，对于高吞吐量的分类、护栏和路由任务，非自回归决策模型提供了一种更优越、更可靠且开源的LLM替代方案。

---

## 4. 微软高管将AI抓取称为“人类历史上最大的劳动盗窃”。

**原文标题**: Microsoft exec called AI scraping 'the largest theft of labor in human history'

**原文链接**: [https://techcrunch.com/2026/09/17/microsoft-exec-called-ai-scraping-the-largest-theft-of-labor-in-human-history-new-unredacted-filings-reveal/](https://techcrunch.com/2026/09/17/microsoft-exec-called-ai-scraping-the-largest-theft-of-labor-in-human-history-new-unredacted-filings-reveal/)

《纽约时报》对OpenAI和微软的版权诉讼中披露的新未经删节信息，揭示了内部承认，这些承认严重削弱了两家公司“合理使用”的辩护。微软一位高级主管布伦特·赫克特曾私下称AI抓取为“人类历史上最大的劳动盗窃”和“前所未有的惊人盗窃”。OpenAI领导层也将其AI模型描述为对出版商的“生存威胁”。

这些披露与“合理使用”的要求相悖，即使用不应损害原创作品的市场。微软内部数据显示，其Copilot“答案引擎”导致《纽约时报》域名的点击率下降了93%，被形容为“厄运循环”。微软首席执行官萨蒂亚·纳德拉作证称，付费墙内容应获得许可，如果他知道OpenAI抓取了这些材料，他会要求OpenAI重新训练其模型。OpenAI高管也承认他们的产品“很大程度上具有替代性”，并与原创来源直接竞争。

诉讼详细披露了复制的巨大规模，其中期训练数据集包含来自新闻出版商的91,000多份副本，仅nytimes.com就有200多万份文件。据称，这些公司绕过了付费墙（一名OpenAI研究员分享了针对《纽约时报》付费墙的“破解方法”），故意删除了版权声明，并交换了大量的训练数据集，这表明他们清楚自己的行为存在问题。OpenAI和微软拒绝对新的备案文件发表评论。

---

## 5. 我 不喜欢 通行密钥

**原文标题**: I don't like passkeys

**原文链接**: [https://hawksley.dev/blog/i-dont-like-passkeys](https://hawksley.dev/blog/i-dont-like-passkeys)

该文章对科技行业大力推广用于个人使用的通行密钥表示怀疑。作者承认通行密钥在防范网络钓鱼和数据泄露方面具有强大的安全优势，使其非常适合企业环境，但认为它们给个人用户带来了巨大风险。

对于个人用户而言，通行密钥将主要安全问题从中间人攻击转移到永久账户锁定、自动封禁或设备丢失等更高的可能性上。这造成了一种虚假的安全感，因为账户访问仍然可能通过短信或电子邮件等较弱的恢复方法受到威胁。

作者强调了以下几个弊端：
*   **硬件密钥：** 它们价格昂贵，无法备份，每个网站都需要单独注册每个密钥，并且账户存储空间有限，需要购买更多。
*   **操作系统同步的通行密钥（苹果/谷歌）：** 它们将用户身份与操作系统绑定，如果操作系统账户被封禁，存在不可逆转地丢失所有关联账户的风险。互操作性和导出选项目前尚不成熟。
*   **第三方管理器：** 用户体验依然零散，缺乏传统密码自动填充的流畅性。
*   **实用性：** 在共享设备上登录不便，依赖可能不可靠的方法，如混合传输（二维码/蓝牙）。

总之，作者认为通行密钥生态系统对个人用户来说尚不成熟。他们认为，对大多数人来说，账户锁定和恢复的风险大于其提供的防钓鱼保护。相反，结合使用第三方管理器中随机生成的密码和独立的TOTP应用程序，可以提供更好的控制和灵活性。虽然通行密钥对于以前重复使用密码的用户来说是一个显著改进，但对其他人来说目前却是一种倒退。

---

## 6. Cloudflare 快速隧道

**原文标题**: Cloudflare Quick Tunnels

**原文链接**: [https://try.cloudflare.com/](https://try.cloudflare.com/)

Cloudflare Quick Tunnels 提供一种快速、免费、安全的方法，通过单个命令将本地 Web 服务器暴露到互联网。开发者可以即时将 `http://localhost:PORT` 转换为公共的、加密的 URL，而无需账户、DNS 配置，也无需在其机器上打开任何入站端口。

`cloudflared` 工具建立一个仅出站连接到 Cloudflare 的全球边缘网络（覆盖 335+ 城市）。导向唯一隧道 URL 的流量通过 Cloudflare 路由回本地机器，受益于自动 HTTPS、DDoS 过滤和加密，确保本地环境保持私密。设置非常迅速，通常只需大约 3 秒。

专为“代理时代”和开发者设计，Quick Tunnels 便于即时共享，用于测试、Webhook（例如 Stripe、GitHub）、评估工具或与队友协作。它们支持任何 Web 框架或端口，并且在设计上是短暂的，这意味着隧道会随进程终止而消亡，无需进行清理。该工具还提供结构化的 JSON 输出，以便集成到自动化工作流中。

---

## 7. Claude 代码现在会读取 AGENTS.md，如果不存在 Claude.md。

**原文标题**: Claude Code now reads AGENTS.md if there is no Claude.md

**原文链接**: [https://code.claude.com/docs/en/changelog](https://code.claude.com/docs/en/changelog)

Claude Code has released several updates, including versions 2.1.275 through 2.1.278, introducing new features, improvements, and extensive bug fixes.

A significant update in version 2.1.277 is the **addition of AGENTS.md support**: Claude Code will now automatically read `AGENTS.md` for project instructions if a `CLAUDE.md` file is not found in the project directory. This configuration is adjustable via “Project instructions” in `/config`.

Version 2.1.278 changed the default auto mode for Claude API and Enterprise users to utilize a **server-side classifier**, eliminating charges for classifier overhead, with an option to opt out. A new `/status` row indicates this setting.

Other key additions across these versions include enhanced Claude apps gateway functionality, a `Ctrl+Enter` "send-now" key, synchronization of `claude.ai` account skills and plugins, and improved startup warnings. General improvements focus on faster session start-up, better plugin installation messaging, prompt cleaning (removing invisible Unicode), and smarter use of the Artifact tool for `claude.ai` links. The deprecated `TaskOutput` tool has been removed.

Numerous bug fixes address critical issues such as Agent SDK session hangs, conversation failures due to empty text blocks, unexpected logouts, and crashes stemming from malformed configuration files or terminal outputs. Improvements also cover tool reliability (Write, Edit, Grep/Glob), plugin management, update processes, and specific enhancements and fixes for VSCode, Claude Code on the web, and Claude Tag environments, significantly improving overall stability and user experience.

---

## 8. 开放杰夫

**原文标题**: OpenJev

**原文链接**: [https://openjev.com/](https://openjev.com/)

生成摘要时出错

---

## 9. Bend——一种通过证明来阻止AI错误并在GPU上运行的语言

**原文标题**: Bend – a language that blocks AI mistakes via proof and runs on GPUs

**原文链接**: [https://bend-lang.com/](https://bend-lang.com/)

生成摘要时出错

---

## 10. How to Write with an LLM

**原文标题**: How to Write with an LLM

**原文链接**: [https://sockpuppet.org/blog/2026/09/17/how-to-write-with-an-llm/](https://sockpuppet.org/blog/2026/09/17/how-to-write-with-an-llm/)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-09-19](output/hacker_news_summary_2026-09-19.md) |
| 2 | [2026-09-17](output/hacker_news_summary_2026-09-17.md) |
| 3 | [2026-09-16](output/hacker_news_summary_2026-09-16.md) |
| 4 | [2026-09-18](output/hacker_news_summary_2026-09-18.md) |
| 5 | [2026-09-15](output/hacker_news_summary_2026-09-15.md) |
| 6 | [2026-09-14](output/hacker_news_summary_2026-09-14.md) |
| 7 | [2026-09-09](output/hacker_news_summary_2026-09-09.md) |
| 8 | [2026-09-08](output/hacker_news_summary_2026-09-08.md) |
| 9 | [2026-09-10](output/hacker_news_summary_2026-09-10.md) |
| 10 | [2026-09-11](output/hacker_news_summary_2026-09-11.md) |
| 11 | [2026-09-13](output/hacker_news_summary_2026-09-13.md) |
| 12 | [2026-09-12](output/hacker_news_summary_2026-09-12.md) |
| 13 | [2026-09-04](output/hacker_news_summary_2026-09-04.md) |
| 14 | [2026-09-07](output/hacker_news_summary_2026-09-07.md) |
| 15 | [2026-09-01](output/hacker_news_summary_2026-09-01.md) |
| 16 | [2026-09-03](output/hacker_news_summary_2026-09-03.md) |
| 17 | [2026-08-31](output/hacker_news_summary_2026-08-31.md) |
| 18 | [2026-09-02](output/hacker_news_summary_2026-09-02.md) |
| 19 | [2026-09-05](output/hacker_news_summary_2026-09-05.md) |
| 20 | [2026-09-06](output/hacker_news_summary_2026-09-06.md) |
| 21 | [2026-08-25](output/hacker_news_summary_2026-08-25.md) |
| 22 | [2026-08-26](output/hacker_news_summary_2026-08-26.md) |
| 23 | [2026-08-23](output/hacker_news_summary_2026-08-23.md) |
| 24 | [2026-08-28](output/hacker_news_summary_2026-08-28.md) |
| 25 | [2026-08-24](output/hacker_news_summary_2026-08-24.md) |
| 26 | [2026-08-30](output/hacker_news_summary_2026-08-30.md) |
| 27 | [2026-08-29](output/hacker_news_summary_2026-08-29.md) |
| 28 | [2026-08-20](output/hacker_news_summary_2026-08-20.md) |
| 29 | [2026-08-18](output/hacker_news_summary_2026-08-18.md) |
| 30 | [2026-08-19](output/hacker_news_summary_2026-08-19.md) |
| 31 | [2026-08-21](output/hacker_news_summary_2026-08-21.md) |
| 32 | [2026-08-17](output/hacker_news_summary_2026-08-17.md) |
| 33 | [2026-08-16](output/hacker_news_summary_2026-08-16.md) |
| 34 | [2026-08-22](output/hacker_news_summary_2026-08-22.md) |
| 35 | [2026-08-15](output/hacker_news_summary_2026-08-15.md) |
| 36 | [2026-08-12](output/hacker_news_summary_2026-08-12.md) |
| 37 | [2026-08-14](output/hacker_news_summary_2026-08-14.md) |
| 38 | [2026-08-10](output/hacker_news_summary_2026-08-10.md) |
| 39 | [2026-08-11](output/hacker_news_summary_2026-08-11.md) |
| 40 | [2026-08-09](output/hacker_news_summary_2026-08-09.md) |
| 41 | [2026-08-13](output/hacker_news_summary_2026-08-13.md) |
| 42 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 43 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 44 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 45 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 46 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 47 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 48 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 49 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 50 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 51 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 52 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 53 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 54 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 55 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 56 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 57 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 58 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 59 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 60 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 61 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 62 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 63 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 64 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 65 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 66 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 67 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 68 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 69 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 70 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 71 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 72 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 73 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 74 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 75 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 76 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 77 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 78 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 79 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 80 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 81 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 82 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 83 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 84 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 85 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 86 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 87 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 88 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 89 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 90 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 91 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 92 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 93 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 94 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 95 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 96 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 97 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 98 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 99 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 100 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 101 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 102 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 103 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 104 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 105 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 106 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 107 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 108 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 109 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 110 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 111 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 112 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 113 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 114 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 115 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 116 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 117 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 118 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 119 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 120 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 121 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 122 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 123 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 124 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 125 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 126 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 127 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 128 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 129 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 130 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 131 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 132 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 133 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 134 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 135 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 136 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 137 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 138 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 139 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 140 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 141 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 142 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 143 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 144 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 145 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 146 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 147 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 148 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 149 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 150 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 151 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 152 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 153 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 154 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 155 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 156 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 157 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 158 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 159 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 160 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 161 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 162 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 163 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 164 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 165 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 166 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 167 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 168 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 169 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 170 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 171 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 172 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 173 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 174 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 175 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 176 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 177 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 178 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 179 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 180 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 181 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 182 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 183 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 184 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 185 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 186 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 187 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 188 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 189 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 190 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 191 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 192 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 193 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 194 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 195 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 196 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 197 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 198 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 199 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 200 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 201 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 202 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 203 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 204 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 205 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 206 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 207 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 208 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 209 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 210 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 211 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 212 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 213 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 214 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 215 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 216 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 217 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 218 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 219 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 220 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 221 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 222 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 223 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 224 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 225 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 226 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 227 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 228 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 229 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 230 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 231 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 232 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 233 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 234 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 235 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 236 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 237 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 238 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 239 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 240 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 241 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 242 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 243 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 244 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 245 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 246 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 247 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 248 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 249 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 250 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 251 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 252 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 253 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 254 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 255 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 256 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 257 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 258 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 259 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 260 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 261 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 262 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 263 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 264 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 265 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 266 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 267 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 268 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 269 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 270 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 271 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 272 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 273 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 274 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 275 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 276 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 277 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 278 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 279 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 280 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 281 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 282 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 283 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 284 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 285 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 286 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 287 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 288 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 289 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 290 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 291 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 292 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 293 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 294 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 295 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 296 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 297 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 298 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 299 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 300 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 301 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 302 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 303 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 304 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 305 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 306 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 307 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 308 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 309 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 310 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 311 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 312 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 313 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 314 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
