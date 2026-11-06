# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-11-06.md)

*最后自动更新时间: 2026-11-06 00:26:00*
## 1. 混蛋

**原文标题**: sshole

**原文链接**: [https://sshhole.com](https://sshhole.com)

这篇题为“sshole”的文章讲述了一段关于Unix密码存储的历史。在早期的Unix系统中，密码哈希值存储在对所有人可读的`/etc/passwd`文件中，这带来了重大的安全风险。

1980年，Bill Joy引入了一个巧妙的变通方法。对于像“daemon”这样不用于直接登录的系统账户，他在密码哈希字段中放入了一个星号（`*`）。由于星号不是一个有效的密码哈希值，任何密码都无法与之匹配，有效地阻止了任何人登录该账户。这种方法至今仍在类Unix系统中被使用。

1980年3BSD的`/etc/passwd`文件中的一个值得注意的细节显示，Joy幽默地将“daemon”账户的真实名称描述为“魔鬼本人”。这个趣闻突出了早期计算机历史中一个简单而有效的安全措施。

---

## 2. AI迫使我们偿还40年的技术债。

**原文标题**: AI is forcing us to pay off 40 years of technical debt

**原文链接**: [https://spectrum.ieee.org/ai-in-cybersecurity-php2shell-vulnerability](https://spectrum.ieee.org/ai-in-cybersecurity-php2shell-vulnerability)

本文由《IEEE Spectrum》计算与硬件编辑 Dina Genkina 撰写，指出人工智能正迫使计算行业解决长达40年的技术债。文章强调，“PHP2Shell 漏洞”是严重网络安全威胁的一个典型案例，这预示着网络安全领域未来充满挑战，并凸显了迫切需要正视并解决这些长期未决的技术问题。

---

## 3. Residential proxies detected on White House network

**原文标题**: Residential proxies detected on White House network

**原文链接**: [https://layer3intel.com/blog/residential-proxies-white-house-network](https://layer3intel.com/blog/residential-proxies-white-house-network)

生成摘要时出错

---

## 4. 朝鲜假招聘面试导致63亿美元币安盗窃案

**原文标题**: North Korean fake job interview led to $6.3B Binance heist

**原文链接**: [https://www.theregister.com/security/2026/11/03/north-korean-fake-job-interview-led-to-63b-binance-heist/5307398](https://www.theregister.com/security/2026/11/03/north-korean-fake-job-interview-led-to-63b-binance-heist/5307398)

联邦调查局认定为TraderTraitor（与Lazarus Group有关联）的朝鲜黑客策划了一场复杂的、多阶段的行动，从币安窃取了63亿美元的加密货币。

这场精心策划的攻击始于六月，通过在一名币安工程师的电脑上恶意安装Homebrew，实施了供应链攻击。尽管被发现并得到缓解，但这一事件仍让黑客知晓了该工程师的角色。

九月，另一名币安软件工程师通过虚假的招聘面试流程成为目标。攻击者假扮成一个虚构公司的项目总监，后来又冒充“CEO”，建立了信任，随后诱骗该工程师下载了一个带有恶意软件的代码库作为“任务”。这个恶意软件替换了一个合法的开发工具组件，与攻击者控制的服务器建立了通信，并成功躲避了检测。

截至10月20日，攻击者利用受损电脑和内部AI工具访问了其他钱包基础设施工程师的机器。10月29日，他们通过另一名工程师的电脑，利用窃取的凭证（来自一名拥有容器部署权限的工程师），部署了一个容器并启动了窃取加密货币的脚本。

币安此后已重建了受损系统，更换了受影响的设备，注销了凭证，并正与执法部门和网络安全专家合作，以追踪资产并实施额外的保护措施，包括设立一个专注于区块链环境中人工智能的新安全研究基金。

---

## 5. Kimi K3.1 Pro 模型权重已放出

**原文标题**: Kimi K3.1 Pro model weights are out

**原文链接**: [https://huggingface.co/moonshotai/Kimi-K3.1-Pro](https://huggingface.co/moonshotai/Kimi-K3.1-Pro)

Kimi K3.1 Pro 模型权重已发布，引入了一个开源、原生多模态、且具备智能体能力的模型。作为 Kimi 最强大的 3T 级模型，它采用了专家混合 (MoE) 架构，拥有 2.8 万亿总参数（其中 1040 亿参数处于激活状态），并具备惊人的 100 万 token 上下文窗口。其主要架构特点包括 KDA 和门控 DSA 注意力机制、SiTU-GLU 激活函数，以及 MoonViT-V2 视觉编码器，支持文本和图像模态，并采用 MXFP4/MXFP8 量化。

该模型在编码、3D 创作、金融研究、事实准确性以及其他智能体能力等多个领域表现出显著改进。评估结果显示，在 Terminal-Bench 4.0、BenchCAD、BrowseComp、MMMU-Pro、GPQA-Diamond、OSWorld V2.1 和 ExploitBench 等基准测试中，Kimi K3.1 Pro 常常超越 Claude Fable 5.1、GPT-6 Astra 和 Claude Opus 5.5 等领先模型，或与其保持高度竞争力。

Kimi K3.1 Pro 可通过 platform.kimi.ai 上与 OpenAI/Anthropic 兼容的 API 进行访问，并推荐在 vLLM、SGLang 和 TokenSpeed 上进行推理。用户可以配置其“思考努力程度”（低、高、最大），并且在多轮交互中必须完整传回助理消息，包括 `reasoning_content` 和 `tool_calls`。该模型根据 Kimi K3.1 Pro 许可协议发布。

---

## 6. 英伟达 RTX Spark 加密固件导致 Linux 推理速度下降至 35%

**原文标题**: Nvidia RTX Spark encrypted firmware slows inference speed to 35% on Linux

**原文链接**: [https://www.mindstudio.ai/blog/linux-nvidia-rtx-spark-laptop](https://www.mindstudio.ai/blog/linux-nvidia-rtx-spark-laptop)

英伟达RTX Spark笔记本电脑专为AI开发设计，可运行Linux，但存在一个关键的性能问题。当连接外部电源时，原生Linux上的GPU频率会被严重限制在约780 MHz，远低于其在Windows上能达到的2.2 GHz以上。这一瓶颈将AI推理速度降低了大约80%，对于120B参数模型，其推理速度从Windows上的每秒约65个token降至Linux上的仅14个。

这种速度下降源于一个仅限Windows的组件，名为“英伟达平台控制器和框架”（Nvidia Platform Controllers and Framework）。该固件和驱动逻辑负责管理CPU和GPU之间的供电，它使用一个加密的电源表，只有Windows驱动程序才能解密。Linux目前缺乏读取和管理这些设置的同等解决方案，导致GPU在连接电源时性能不佳。

原生Linux的其他障碍包括复杂的安装（需要针对Wi-Fi、外设和显示器采取变通措施）和内存分配。默认情况下，96GB的统一内存会为GPU预留，这个设置只能在Windows中调整，必须先更改才能让Linux访问更多RAM。

有趣的是，这个问题与电源有关：在电池供电下，Linux GPU的性能与Windows相当。然而，对于持续的高性能任务，这并不实用。

目前，适用于Linux的Windows子系统（WSL）提供了最实用的解决方案。WSL利用Windows驱动栈，从而避免了时钟限制并保持了GPU的全部性能提升，同时仍允许开发者使用vLLM等Linux优先的AI工具。

真正的解决方案需要英伟达将其平台控制器的电源管理逻辑，包括电源表的解密功能，直接集成到其Linux驱动程序中。

---

## 7. AMD 预计第四季度销量将首次超越英特尔。

**原文标题**: AMD expects to outsell Intel in Q4 for the first time in history

**原文链接**: [https://www.tomshardware.com/pc-components/cpus/amd-expects-to-outsell-intel-in-q4-for-the-first-time-in-history-usd17b-guidance-would-exceed-intels-projections](https://www.tomshardware.com/pc-components/cpus/amd-expects-to-outsell-intel-in-q4-for-the-first-time-in-history-usd17b-guidance-would-exceed-intels-projections)

AMD在第三季度报告了有史以来最高的季度营收，达到133.77亿美元，这主要得益于其Epyc数据中心处理器和Instinct人工智能加速器。该公司预计第四季度营收将达到惊人的约170亿美元，这将使其历史上首次超越英特尔，预计领先15亿美元。

数据中心业务是主要的增长动力，第三季度销售额同比飙升97%，达到85.5亿美元，目前占AMD总营收的64%。该部门的营业收入激增168%。AMD预计第四季度数据中心营收将大幅增长，并预计到2027年，在Meta和微软等主要客户对其AI解决方案的强劲需求推动下，数据中心业务将贡献公司总销售额的80%以上。

相比之下，AMD的客户端和游戏业务部门营收同比下降8%，至37.22亿美元，受到主机SoC销量下降和独立GPU需求疲软的影响。AMD预计2027年PC出货量将出现两位数下降，但旨在通过专注于企业和高端消费市场来超越整体市场表现。然而，嵌入式业务表现出强劲增长，营收增长29%，达到11.1亿美元。

市场领导地位的这一预期转变，凸显了AMD成功拓展高增长的数据中心和AI市场，与英特尔继续严重依赖面临市场挑战的PC和传统服务器处理器形成鲜明对比。

---

## 8. Alpine Linux 安全公告：OpenSSH 服务器密码认证绕过

**原文标题**: Alpine Linux Security Advisory: OpenSSH-server password authentication bypass

**原文链接**: [https://alpinelinux.org/posts/2026-11-05-openssh-password-authentication-bypass/](https://alpinelinux.org/posts/2026-11-05-openssh-password-authentication-bypass/)

生成摘要时出错

---

## 9. A thousand fewer paths to root

**原文标题**: A thousand fewer paths to root

**原文链接**: [https://openai.com/index/a-thousand-fewer-paths-to-root/](https://openai.com/index/a-thousand-fewer-paths-to-root/)

生成摘要时出错

---

## 10. Jelly Sheet

**原文标题**: Jelly Sheet

**原文链接**: [https://mrdoob.github.io/codevember-2026/01/](https://mrdoob.github.io/codevember-2026/01/)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-11-06](output/hacker_news_summary_2026-11-06.md) |
| 2 | [2026-11-05](output/hacker_news_summary_2026-11-05.md) |
| 3 | [2026-11-03](output/hacker_news_summary_2026-11-03.md) |
| 4 | [2026-11-01](output/hacker_news_summary_2026-11-01.md) |
| 5 | [2026-11-04](output/hacker_news_summary_2026-11-04.md) |
| 6 | [2026-10-29](output/hacker_news_summary_2026-10-29.md) |
| 7 | [2026-10-30](output/hacker_news_summary_2026-10-30.md) |
| 8 | [2026-10-27](output/hacker_news_summary_2026-10-27.md) |
| 9 | [2026-10-28](output/hacker_news_summary_2026-10-28.md) |
| 10 | [2026-10-31](output/hacker_news_summary_2026-10-31.md) |
| 11 | [2026-10-26](output/hacker_news_summary_2026-10-26.md) |
| 12 | [2026-10-21](output/hacker_news_summary_2026-10-21.md) |
| 13 | [2026-10-22](output/hacker_news_summary_2026-10-22.md) |
| 14 | [2026-10-25](output/hacker_news_summary_2026-10-25.md) |
| 15 | [2026-10-24](output/hacker_news_summary_2026-10-24.md) |
| 16 | [2026-10-23](output/hacker_news_summary_2026-10-23.md) |
| 17 | [2026-10-20](output/hacker_news_summary_2026-10-20.md) |
| 18 | [2026-10-17](output/hacker_news_summary_2026-10-17.md) |
| 19 | [2026-10-18](output/hacker_news_summary_2026-10-18.md) |
| 20 | [2026-10-16](output/hacker_news_summary_2026-10-16.md) |
| 21 | [2026-10-19](output/hacker_news_summary_2026-10-19.md) |
| 22 | [2026-10-15](output/hacker_news_summary_2026-10-15.md) |
| 23 | [2026-10-14](output/hacker_news_summary_2026-10-14.md) |
| 24 | [2026-10-13](output/hacker_news_summary_2026-10-13.md) |
| 25 | [2026-10-11](output/hacker_news_summary_2026-10-11.md) |
| 26 | [2026-10-10](output/hacker_news_summary_2026-10-10.md) |
| 27 | [2026-10-07](output/hacker_news_summary_2026-10-07.md) |
| 28 | [2026-10-09](output/hacker_news_summary_2026-10-09.md) |
| 29 | [2026-10-01](output/hacker_news_summary_2026-10-01.md) |
| 30 | [2026-10-03](output/hacker_news_summary_2026-10-03.md) |
| 31 | [2026-10-06](output/hacker_news_summary_2026-10-06.md) |
| 32 | [2026-10-04](output/hacker_news_summary_2026-10-04.md) |
| 33 | [2026-10-02](output/hacker_news_summary_2026-10-02.md) |
| 34 | [2026-09-27](output/hacker_news_summary_2026-09-27.md) |
| 35 | [2026-09-24](output/hacker_news_summary_2026-09-24.md) |
| 36 | [2026-09-30](output/hacker_news_summary_2026-09-30.md) |
| 37 | [2026-09-29](output/hacker_news_summary_2026-09-29.md) |
| 38 | [2026-09-23](output/hacker_news_summary_2026-09-23.md) |
| 39 | [2026-09-25](output/hacker_news_summary_2026-09-25.md) |
| 40 | [2026-09-19](output/hacker_news_summary_2026-09-19.md) |
| 41 | [2026-09-18](output/hacker_news_summary_2026-09-18.md) |
| 42 | [2026-09-22](output/hacker_news_summary_2026-09-22.md) |
| 43 | [2026-09-21](output/hacker_news_summary_2026-09-21.md) |
| 44 | [2026-09-20](output/hacker_news_summary_2026-09-20.md) |
| 45 | [2026-09-17](output/hacker_news_summary_2026-09-17.md) |
| 46 | [2026-09-13](output/hacker_news_summary_2026-09-13.md) |
| 47 | [2026-09-15](output/hacker_news_summary_2026-09-15.md) |
| 48 | [2026-09-14](output/hacker_news_summary_2026-09-14.md) |
| 49 | [2026-09-16](output/hacker_news_summary_2026-09-16.md) |
| 50 | [2026-09-11](output/hacker_news_summary_2026-09-11.md) |
| 51 | [2026-09-07](output/hacker_news_summary_2026-09-07.md) |
| 52 | [2026-09-10](output/hacker_news_summary_2026-09-10.md) |
| 53 | [2026-09-12](output/hacker_news_summary_2026-09-12.md) |
| 54 | [2026-09-09](output/hacker_news_summary_2026-09-09.md) |
| 55 | [2026-09-08](output/hacker_news_summary_2026-09-08.md) |
| 56 | [2026-09-06](output/hacker_news_summary_2026-09-06.md) |
| 57 | [2026-09-04](output/hacker_news_summary_2026-09-04.md) |
| 58 | [2026-09-01](output/hacker_news_summary_2026-09-01.md) |
| 59 | [2026-08-29](output/hacker_news_summary_2026-08-29.md) |
| 60 | [2026-09-02](output/hacker_news_summary_2026-09-02.md) |
| 61 | [2026-09-05](output/hacker_news_summary_2026-09-05.md) |
| 62 | [2026-08-30](output/hacker_news_summary_2026-08-30.md) |
| 63 | [2026-08-31](output/hacker_news_summary_2026-08-31.md) |
| 64 | [2026-09-03](output/hacker_news_summary_2026-09-03.md) |
| 65 | [2026-08-23](output/hacker_news_summary_2026-08-23.md) |
| 66 | [2026-08-28](output/hacker_news_summary_2026-08-28.md) |
| 67 | [2026-08-24](output/hacker_news_summary_2026-08-24.md) |
| 68 | [2026-08-26](output/hacker_news_summary_2026-08-26.md) |
| 69 | [2026-08-25](output/hacker_news_summary_2026-08-25.md) |
| 70 | [2026-08-21](output/hacker_news_summary_2026-08-21.md) |
| 71 | [2026-08-22](output/hacker_news_summary_2026-08-22.md) |
| 72 | [2026-08-16](output/hacker_news_summary_2026-08-16.md) |
| 73 | [2026-08-13](output/hacker_news_summary_2026-08-13.md) |
| 74 | [2026-08-20](output/hacker_news_summary_2026-08-20.md) |
| 75 | [2026-08-19](output/hacker_news_summary_2026-08-19.md) |
| 76 | [2026-08-18](output/hacker_news_summary_2026-08-18.md) |
| 77 | [2026-08-15](output/hacker_news_summary_2026-08-15.md) |
| 78 | [2026-08-14](output/hacker_news_summary_2026-08-14.md) |
| 79 | [2026-08-17](output/hacker_news_summary_2026-08-17.md) |
| 80 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 81 | [2026-08-09](output/hacker_news_summary_2026-08-09.md) |
| 82 | [2026-08-12](output/hacker_news_summary_2026-08-12.md) |
| 83 | [2026-08-10](output/hacker_news_summary_2026-08-10.md) |
| 84 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 85 | [2026-08-11](output/hacker_news_summary_2026-08-11.md) |
| 86 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 87 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 88 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 89 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 90 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 91 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 92 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 93 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 94 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 95 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 96 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 97 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 98 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 99 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 100 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 101 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 102 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 103 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 104 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 105 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 106 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 107 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 108 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 109 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 110 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 111 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 112 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 113 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 114 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 115 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 116 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 117 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 118 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 119 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 120 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 121 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 122 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 123 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 124 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 125 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 126 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 127 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 128 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 129 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 130 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 131 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 132 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 133 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 134 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 135 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 136 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 137 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 138 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 139 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 140 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 141 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 142 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 143 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 144 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 145 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 146 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 147 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 148 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 149 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 150 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 151 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 152 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 153 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 154 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 155 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 156 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 157 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 158 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 159 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 160 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 161 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 162 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 163 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 164 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 165 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 166 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 167 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 168 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 169 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 170 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 171 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 172 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 173 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 174 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 175 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 176 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 177 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 178 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 179 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 180 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 181 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 182 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 183 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 184 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 185 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 186 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 187 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 188 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 189 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 190 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 191 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 192 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 193 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 194 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 195 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 196 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 197 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 198 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 199 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 200 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 201 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 202 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 203 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 204 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 205 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 206 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 207 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 208 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 209 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 210 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 211 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 212 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 213 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 214 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 215 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 216 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 217 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 218 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 219 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 220 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 221 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 222 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 223 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 224 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 225 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 226 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 227 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 228 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 229 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 230 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 231 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 232 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 233 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 234 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 235 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 236 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 237 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 238 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 239 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 240 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 241 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 242 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 243 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 244 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 245 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 246 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 247 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 248 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 249 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 250 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 251 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 252 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 253 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 254 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 255 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 256 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 257 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 258 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 259 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 260 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 261 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 262 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 263 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 264 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 265 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 266 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 267 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 268 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 269 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 270 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 271 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 272 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 273 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 274 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 275 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 276 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 277 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 278 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 279 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 280 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 281 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 282 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 283 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 284 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 285 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 286 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 287 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 288 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 289 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 290 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 291 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 292 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 293 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 294 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 295 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 296 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 297 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 298 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 299 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 300 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 301 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 302 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 303 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 304 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 305 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 306 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 307 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 308 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 309 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 310 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 311 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 312 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 313 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 314 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 315 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 316 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 317 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 318 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 319 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 320 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 321 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 322 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 323 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 324 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 325 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 326 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 327 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 328 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 329 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 330 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 331 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 332 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 333 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 334 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 335 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 336 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 337 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 338 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 339 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 340 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 341 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 342 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 343 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 344 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 345 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 346 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 347 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 348 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 349 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 350 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 351 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 352 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 353 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 354 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 355 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 356 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
