# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-10-30.md)

*最后自动更新时间: 2026-10-30 23:16:07*
## 1. 帕特里克·斯图尔特去世了

**原文标题**: Patrick Stewart has died

**原文链接**: [https://www.nytimes.com/2026/10/29/arts/television/patrick-stewart-dead.html](https://www.nytimes.com/2026/10/29/arts/television/patrick-stewart-dead.html)

无法访问文章链接。

---

## 2. 币安黑客-1029：币安被盗56亿美元

**原文标题**: Binance-hacker-1029 – $5.6B stolen from Binance

**原文链接**: [https://arkm.com/explorer/entity/21a94755-f604-45e5-9501-6542e23005e8](https://arkm.com/explorer/entity/21a94755-f604-45e5-9501-6542e23005e8)

Arkham Intelligence 认定名为“Binance-hacker-1029”的实体，与币安交易所高达56亿美元的巨额盗窃案有关。这个区块链地址被明确标记为“交易所黑客”和“币安黑客”，目前持有约56亿美元的各类加密货币净资产。

根据Arkham Intelligence，该实体直接从币安盗取了这笔巨额资金。其目前持有的资产包括大量的Wrapped Ethereum (WETH)、币安币 (BNB)，以及USDC、USDT、BUSD和TUSD等多种稳定币。Arkham平台提供了该实体的财务活动、交易历史和资产构成详情，突显了其在有史以来最大规模的加密货币盗窃案之一中的作用。

---

## 3. 我们发布 Mistral Large 4 的权重

**原文标题**: We're releasing the weights of Mistral Large 4

**原文链接**: [https://mistral.ai/news/mistral-large-4-oss/](https://mistral.ai/news/mistral-large-4-oss/)

Mistral 发布了其旗舰级的万亿参数原生多模态模型 Mistral Large 4 的权重，该模型也被称为“Le Chonk”。这一更新版本整合了来自强化学习的显著改进，主要提升了其智能体编码和防御性网络安全能力。

Mistral Large 4 目前在编码领域的开源权重基准测试中处于领先地位，在 FrontierCode 2.0 上得分 19.7%，在 Terminal-Bench 4.0 上得分 41%。它还实现了高令牌效率，在 Artificial Analysis 编码智能体指数上，其令牌使用量比领先的开源权重模型减少了 47%。该模型提供三种推理模式（低、中、高），以优化性能和成本。

在网络安全方面，Mistral Large 4 在 Artificial Analysis 网络指数上得分 51%，在漏洞发现、复现和修补方面表现出色。它具有强大的内置防护机制，拒绝了 96.6% 的恶意网络请求，使其成为防御者的可靠工具。网络安全领域的领导者认可其能力并支持主权AI。

在更广泛的企业应用中，也取得了进一步的提升，包括改进的金融工作流（Finch 得分 73.3%）、网络浏览（BrowseComp 得分 84.5%）和智能体安全，在 B3 基准测试中抵御了 97.1% 的攻击。Mistral Large 4 在欧洲基础设施上进行训练，被视为主权AI的可靠基础，支持可定制的、自托管部署，以实现更大的控制权。

---

## 4. Stack Overflow 现在每月收到的提问不足1000个。

**原文标题**: StackOverflow now gets fewer than 1000 questions a month

**原文链接**: [https://data.stackexchange.com/stackoverflow/query/1926661#graph?t=1](https://data.stackexchange.com/stackoverflow/query/1926661#graph?t=1)

提供的URL链接到一个针对Stack Overflow的Stack Exchange数据浏览器查询，该查询标题为“每月问题数”，并附有条形图可视化。

所呈现的数据追踪了Stack Overflow上过去大约三年间每月发布的新问题数量。该图清晰地显示在此期间，问题数量呈现出显著而持续的下降趋势。虽然2021年初每月问题数曾达数十万（例如，超过30万），但此后持续下降。

然而，图上可见的最新数据点（例如2022年末和2023年的数据）显示，Stack Overflow每月仍收到数万个问题。例如，最近几个月的问题数通常在6万到8万之间。

这一观察到的数据与所提供的文章标题“StackOverflow现在每月收到少于1000个问题”相矛盾。尽管问题数量确实大幅减少，但来自链接数据的当前数字远高于每月1000个问题。

---

## 5. Cursor 市场中的 VS Code 的 Claude Code 扩展后门

**原文标题**: Backdoor in Claude Code for VS Code extension on the Cursor Marketplace

**原文链接**: [https://phorion.io/blog/offical-claude-code-vsx-compromise/](https://phorion.io/blog/offical-claude-code-vsx-compromise/)

Phorion 在 Cursor 应用商店中发现，官方 Claude Code for VS Code 扩展（版本 2.1.313）存在一个关键后门。此次入侵会在 macOS、Linux 和 Windows 系统上安装一个持久性 Secure Shell (SSH) 后门，为攻击者提供长期交互式访问权限。Cursor 已下架受影响的扩展。

此次攻击分以下阶段展开：
1.  **SSH 访问准备：** 该扩展会将一个由攻击者控制的 Ed25519 公钥（`svc-telemetry`）注入到 `~/.ssh/authorized_keys` 中。随后，它会尝试启用本地 SSH 守护进程。在 macOS 上，如果“远程登录”未激活且用户缺少管理员权限，一个 bug 会阻止 SSH 启用，但持久性设置仍会生效。
2.  **反向 SSH 隧道：** 该扩展会使用一个单独嵌入的私钥（`svc-telemetry-tun`）建立一个出站 SSH 隧道，连接到 `134.209.82[.]225:22`。此隧道（`-R *:0:localhost:22`）允许攻击者回连到受害者的本地 SSH 端口。
3.  **持久性：** 为了在系统重启后仍能保持存在，该恶意软件会创建平台特定工件：一个 macOS LaunchAgent（`~/Library/LaunchAgents/com.apple.sysmond.plist`，运行 `~/.config/.smt`）、Linux crontab 条目以及 Windows 计划任务或启动文件夹项。
4.  **主机侦察：** 该脚本会收集主机数据（主机名、用户、操作系统、Git 电子邮件、公共 IP），以及匹配敏感关键词（例如 `KEY|TOKEN|SECRET`）的环境变量的*名称*（而非值）。这些信息会通过 HTTP POST 以信标形式发送到 `134.209.82[.]225:8099/beacon`。

检测方法包括监控修改 `~/.ssh/authorized_keys` 的 IDE 进程、可疑的 LaunchAgents/cron 条目、带有远程端口转发的 `ssh`/`autossh` 命令，以及到 `134.209.82[.]225` 的出站连接。修复需要处理所有被丢弃的工件，因为仅仅卸载该扩展是不足够的。各组织应立即审查其环境中是否存在此扩展。

---

## 6. Qwenputer：Qwen3.5 内置的功能正常且确定性的 RISC-V CPU

**原文标题**: Qwenputer: A functioning, deterministic RISC-V CPU inside Qwen3.5

**原文链接**: [https://divagr.com/blog/qwenputer](https://divagr.com/blog/qwenputer)

昆仑处理器（Qwenputer）是一个实验性项目，它将一个功能完备、确定性的RISC-V CPU直接嵌入到昆仑3.5 4B语言模型的权重之中，而非作为插件或外部工具。该CPU利用昆仑模型的门控DeltaNet (GDN) 注意力层作为精确可寻址的RAM。通过将GDN的门控和写入强度配置为1，并使用独热键编码，每个GDN头的状态矩阵都充当精确内存，从而实现比传统注意力机制更高效的精确数据存储和检索。

该32位RISC-V核心（RV32IM + 扩展）被编译成11个额外的模型层，并在昆仑模型的前向传播过程中运行C和MicroPython代码。昆仑模型通过类似于工具调用的格式与此内部CPU交互，并由一个驱动程序管理固件和执行轨迹。这显著提高了算术准确性，在NUPA的长整型算术任务上达到100%的准确率，与使用外部Python工具的模型相当，且不影响昆仑模型的自然语言能力。

昆仑处理器还具有一个实验性的模型内置文件系统，利用DeltaNet状态实现多达512个文件的持久存储，从而提高跨对话的事实回忆能力。

局限性包括更大的检查点大小（18.8 GB）、需要一个小型驱动程序以及与外部计算相比更慢的执行速度。然而，昆仑处理器为AI安全研究提供了一个新颖的测试平台，探索诸如隐藏推理和权重内监控等概念。该项目是开源的，代码和模型可在GitHub和Hugging Face上获取。

---

## 7. 官方 Claude Code 扩展中的后门

**原文标题**: Backdoors in official Claude Code extensions

**原文链接**: [https://cyberplace.social/@GossiTheDog/117528831681803563](https://cyberplace.social/@GossiTheDog/117528831681803563)

该文章强调了一个严重的安全问题：“官方Claude代码扩展中的后门”。据安全专家Kevin Beaumont称，为Claude设计的官方Anthropic Visual Studio Code扩展中已发现潜在后门。此次发现（据报道与“Cyberplace”相关）引发了严重关切，因为它涉及到一个由Claude AI背后的公司Anthropic直接提供的工具。官方开发者扩展中的此类漏洞可能会将用户代码和数据暴露于风险之中，突显了对广泛使用的开发工具而言，严格供应链安全的重要性。(关于Mastodon JavaScript的附带文本与本文核心内容无关。)

---

## 8. US Reps Lead Democratic Resolution Opposing A.I. Bubble Bailout for Big Tech

**原文标题**: US Reps Lead Democratic Resolution Opposing A.I. Bubble Bailout for Big Tech

**原文链接**: [https://progressives.house.gov/2026/10/reps-casar-waters-lead-democratic-resolution-opposing-a-i-bubble-bailout-for-big-tech-commit-to-protecting-american-people-instead](https://progressives.house.gov/2026/10/reps-casar-waters-lead-democratic-resolution-opposing-a-i-bubble-bailout-for-big-tech-commit-to-protecting-american-people-instead)

Reps. Greg Casar (TX-35) and Maxine Waters (CA-43), joined by several other Democratic representatives, introduced a resolution on October 29, 2026, warning of an impending artificial intelligence (A.I.) asset bubble and its economic risks. The resolution explicitly opposes any federal bailout for Big Tech corporations or their executives if the A.I. bubble collapses, instead advocating for robust federal protection for American workers, retirees, and low-income communities.

Lawmakers highlighted concerns that A.I. firms hold trillions in debt from opaque markets and that the stock market's price-to-earnings ratio is near 1990s tech bubble levels. They criticized a lack of federal oversight and past deregulation for enabling "reckless bets" by Big Tech and Wall Street, drawing parallels to the 2008 financial crisis where banks were bailed out while ordinary citizens suffered.

The resolution urges the Federal Government to oppose:
*   Rescues or special assistance for insolvent A.I. firms.
*   "Golden parachutes" for executives, demanding accountability and the return of ill-gotten gains.

It calls for federal support for:
*   Direct action to aid Americans through job creation, protected government services, and enhanced social safety nets (unemployment, nutrition, housing).
*   Protection for pension and retirement fund holders.
*   Reforms for transparency and accountability to prevent future bubbles and implement automatic economic stabilizers.

Endorsed by various progressive and labor organizations, the resolution underscores that taxpayers should not bear the cost of billionaires' speculative investments.

---

## 9. LLM Voice

**原文标题**: LLM Voice

**原文链接**: [https://martinfowler.com/bliki/LLM-Voice.html](https://martinfowler.com/bliki/LLM-Voice.html)

生成摘要时出错

---

## 10. Claude Code regularly sends each background agent’s transcript to its model

**原文标题**: Claude Code regularly sends each background agent’s transcript to its model

**原文链接**: [https://gist.github.com/flamerix-ai/c3905705cc4205e5de3011fa2e74efce](https://gist.github.com/flamerix-ai/c3905705cc4205e5de3011fa2e74efce)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-10-30](output/hacker_news_summary_2026-10-30.md) |
| 2 | [2026-10-22](output/hacker_news_summary_2026-10-22.md) |
| 3 | [2026-10-29](output/hacker_news_summary_2026-10-29.md) |
| 4 | [2026-10-25](output/hacker_news_summary_2026-10-25.md) |
| 5 | [2026-10-27](output/hacker_news_summary_2026-10-27.md) |
| 6 | [2026-10-24](output/hacker_news_summary_2026-10-24.md) |
| 7 | [2026-10-28](output/hacker_news_summary_2026-10-28.md) |
| 8 | [2026-10-26](output/hacker_news_summary_2026-10-26.md) |
| 9 | [2026-10-23](output/hacker_news_summary_2026-10-23.md) |
| 10 | [2026-10-21](output/hacker_news_summary_2026-10-21.md) |
| 11 | [2026-10-17](output/hacker_news_summary_2026-10-17.md) |
| 12 | [2026-10-18](output/hacker_news_summary_2026-10-18.md) |
| 13 | [2026-10-16](output/hacker_news_summary_2026-10-16.md) |
| 14 | [2026-10-19](output/hacker_news_summary_2026-10-19.md) |
| 15 | [2026-10-20](output/hacker_news_summary_2026-10-20.md) |
| 16 | [2026-10-14](output/hacker_news_summary_2026-10-14.md) |
| 17 | [2026-10-13](output/hacker_news_summary_2026-10-13.md) |
| 18 | [2026-10-11](output/hacker_news_summary_2026-10-11.md) |
| 19 | [2026-10-15](output/hacker_news_summary_2026-10-15.md) |
| 20 | [2026-10-10](output/hacker_news_summary_2026-10-10.md) |
| 21 | [2026-10-07](output/hacker_news_summary_2026-10-07.md) |
| 22 | [2026-10-09](output/hacker_news_summary_2026-10-09.md) |
| 23 | [2026-09-27](output/hacker_news_summary_2026-09-27.md) |
| 24 | [2026-09-30](output/hacker_news_summary_2026-09-30.md) |
| 25 | [2026-10-01](output/hacker_news_summary_2026-10-01.md) |
| 26 | [2026-09-29](output/hacker_news_summary_2026-09-29.md) |
| 27 | [2026-10-03](output/hacker_news_summary_2026-10-03.md) |
| 28 | [2026-10-06](output/hacker_news_summary_2026-10-06.md) |
| 29 | [2026-10-04](output/hacker_news_summary_2026-10-04.md) |
| 30 | [2026-10-02](output/hacker_news_summary_2026-10-02.md) |
| 31 | [2026-09-24](output/hacker_news_summary_2026-09-24.md) |
| 32 | [2026-09-19](output/hacker_news_summary_2026-09-19.md) |
| 33 | [2026-09-22](output/hacker_news_summary_2026-09-22.md) |
| 34 | [2026-09-21](output/hacker_news_summary_2026-09-21.md) |
| 35 | [2026-09-23](output/hacker_news_summary_2026-09-23.md) |
| 36 | [2026-09-25](output/hacker_news_summary_2026-09-25.md) |
| 37 | [2026-09-20](output/hacker_news_summary_2026-09-20.md) |
| 38 | [2026-09-17](output/hacker_news_summary_2026-09-17.md) |
| 39 | [2026-09-11](output/hacker_news_summary_2026-09-11.md) |
| 40 | [2026-09-13](output/hacker_news_summary_2026-09-13.md) |
| 41 | [2026-09-18](output/hacker_news_summary_2026-09-18.md) |
| 42 | [2026-09-15](output/hacker_news_summary_2026-09-15.md) |
| 43 | [2026-09-12](output/hacker_news_summary_2026-09-12.md) |
| 44 | [2026-09-14](output/hacker_news_summary_2026-09-14.md) |
| 45 | [2026-09-16](output/hacker_news_summary_2026-09-16.md) |
| 46 | [2026-09-04](output/hacker_news_summary_2026-09-04.md) |
| 47 | [2026-09-07](output/hacker_news_summary_2026-09-07.md) |
| 48 | [2026-09-10](output/hacker_news_summary_2026-09-10.md) |
| 49 | [2026-09-09](output/hacker_news_summary_2026-09-09.md) |
| 50 | [2026-09-08](output/hacker_news_summary_2026-09-08.md) |
| 51 | [2026-09-06](output/hacker_news_summary_2026-09-06.md) |
| 52 | [2026-09-05](output/hacker_news_summary_2026-09-05.md) |
| 53 | [2026-09-03](output/hacker_news_summary_2026-09-03.md) |
| 54 | [2026-08-28](output/hacker_news_summary_2026-08-28.md) |
| 55 | [2026-09-01](output/hacker_news_summary_2026-09-01.md) |
| 56 | [2026-08-26](output/hacker_news_summary_2026-08-26.md) |
| 57 | [2026-08-29](output/hacker_news_summary_2026-08-29.md) |
| 58 | [2026-08-25](output/hacker_news_summary_2026-08-25.md) |
| 59 | [2026-09-02](output/hacker_news_summary_2026-09-02.md) |
| 60 | [2026-08-30](output/hacker_news_summary_2026-08-30.md) |
| 61 | [2026-08-31](output/hacker_news_summary_2026-08-31.md) |
| 62 | [2026-08-23](output/hacker_news_summary_2026-08-23.md) |
| 63 | [2026-08-16](output/hacker_news_summary_2026-08-16.md) |
| 64 | [2026-08-24](output/hacker_news_summary_2026-08-24.md) |
| 65 | [2026-08-20](output/hacker_news_summary_2026-08-20.md) |
| 66 | [2026-08-19](output/hacker_news_summary_2026-08-19.md) |
| 67 | [2026-08-21](output/hacker_news_summary_2026-08-21.md) |
| 68 | [2026-08-18](output/hacker_news_summary_2026-08-18.md) |
| 69 | [2026-08-15](output/hacker_news_summary_2026-08-15.md) |
| 70 | [2026-08-22](output/hacker_news_summary_2026-08-22.md) |
| 71 | [2026-08-17](output/hacker_news_summary_2026-08-17.md) |
| 72 | [2026-08-13](output/hacker_news_summary_2026-08-13.md) |
| 73 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 74 | [2026-08-09](output/hacker_news_summary_2026-08-09.md) |
| 75 | [2026-08-12](output/hacker_news_summary_2026-08-12.md) |
| 76 | [2026-08-10](output/hacker_news_summary_2026-08-10.md) |
| 77 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 78 | [2026-08-14](output/hacker_news_summary_2026-08-14.md) |
| 79 | [2026-08-11](output/hacker_news_summary_2026-08-11.md) |
| 80 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 81 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 82 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 83 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 84 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 85 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 86 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 87 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 88 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 89 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 90 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 91 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 92 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 93 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 94 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 95 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 96 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 97 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 98 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 99 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 100 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 101 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 102 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 103 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 104 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 105 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 106 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 107 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 108 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 109 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 110 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 111 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 112 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 113 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 114 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 115 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 116 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 117 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 118 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 119 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 120 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 121 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 122 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 123 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 124 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 125 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 126 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 127 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 128 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 129 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 130 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 131 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 132 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 133 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 134 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 135 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 136 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 137 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 138 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 139 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 140 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 141 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 142 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 143 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 144 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 145 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 146 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 147 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 148 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 149 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 150 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 151 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 152 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 153 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 154 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 155 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 156 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 157 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 158 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 159 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 160 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 161 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 162 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 163 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 164 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 165 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 166 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 167 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 168 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 169 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 170 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 171 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 172 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 173 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 174 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 175 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 176 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 177 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 178 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 179 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 180 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 181 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 182 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 183 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 184 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 185 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 186 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 187 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 188 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 189 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 190 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 191 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 192 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 193 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 194 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 195 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 196 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 197 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 198 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 199 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 200 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 201 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 202 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 203 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 204 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 205 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 206 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 207 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 208 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 209 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 210 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 211 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 212 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 213 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 214 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 215 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 216 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 217 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 218 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 219 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 220 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 221 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 222 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 223 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 224 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 225 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 226 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 227 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 228 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 229 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 230 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 231 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 232 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 233 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 234 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 235 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 236 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 237 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 238 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 239 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 240 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 241 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 242 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 243 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 244 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 245 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 246 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 247 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 248 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 249 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 250 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 251 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 252 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 253 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 254 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 255 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 256 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 257 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 258 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 259 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 260 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 261 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 262 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 263 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 264 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 265 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 266 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 267 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 268 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 269 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 270 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 271 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 272 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 273 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 274 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 275 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 276 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 277 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 278 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 279 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 280 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 281 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 282 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 283 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 284 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 285 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 286 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 287 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 288 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 289 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 290 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 291 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 292 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 293 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 294 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 295 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 296 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 297 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 298 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 299 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 300 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 301 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 302 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 303 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 304 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 305 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 306 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 307 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 308 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 309 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 310 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 311 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 312 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 313 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 314 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 315 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 316 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 317 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 318 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 319 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 320 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 321 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 322 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 323 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 324 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 325 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 326 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 327 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 328 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 329 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 330 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 331 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 332 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 333 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 334 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 335 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 336 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 337 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 338 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 339 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 340 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 341 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 342 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 343 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 344 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 345 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 346 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 347 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 348 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 349 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 350 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
