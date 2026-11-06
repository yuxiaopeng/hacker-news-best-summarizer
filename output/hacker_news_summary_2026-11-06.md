# Hacker News 热门文章摘要 (2026-11-06)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

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

## 11. Search for everyone

**原文标题**: Search for everyone

**原文链接**: [https://kagi.com/changelog#11820](https://kagi.com/changelog#11820)

生成摘要时出错

---

## 12. C++26 未批准

**原文标题**: C++26 Disapproved

**原文链接**: [https://andreasfertig.com/blog/2026/11/cpp26-dis-failed-how-does-cpp-survive/](https://andreasfertig.com/blog/2026/11/cpp26-dis-failed-how-does-cpp-survive/)

生成摘要时出错

---

## 13. 新的Go JSON API

**原文标题**: A new Go API for JSON

**原文链接**: [https://go.dev/blog/jsonv2](https://go.dev/blog/jsonv2)

生成摘要时出错

---

## 14. Kitty 0.50

**原文标题**: Kitty 0.50

**原文链接**: [https://sw.kovidgoyal.net/kitty/changelog/#](https://sw.kovidgoyal.net/kitty/changelog/#)

生成摘要时出错

---

## 15. Motorola Signature 27 with GrapheneOS support

**原文标题**: Motorola Signature 27 with GrapheneOS support

**原文链接**: [https://motorolanews.com/motorola-signature-27-2/](https://motorolanews.com/motorola-signature-27-2/)

生成摘要时出错

---

## 16. Lemmings CSS Animation

**原文标题**: Lemmings CSS Animation

**原文链接**: [https://markblah.github.io/lemmings/](https://markblah.github.io/lemmings/)

生成摘要时出错

---

## 17. Images 2.6

**原文标题**: Images 2.6

**原文链接**: [https://openai.com/index/introducing-images-2-6/](https://openai.com/index/introducing-images-2-6/)

生成摘要时出错

---

## 18. Discord is ditching Electron and its new app uses less RAM

**原文标题**: Discord is ditching Electron and its new app uses less RAM

**原文链接**: [https://www.theverge.com/news/1027379/discord-ditching-electron-web-app](https://www.theverge.com/news/1027379/discord-ditching-electron-web-app)

生成摘要时出错

---

## 19. Goodbye from Salon

**原文标题**: Goodbye from Salon

**原文链接**: [https://www.salon.com/2026/11/05/goodbye-from-salon/](https://www.salon.com/2026/11/05/goodbye-from-salon/)

生成摘要时出错

---

## 20. US voters roundly reject data centers in ballot measures

**原文标题**: US voters roundly reject data centers in ballot measures

**原文链接**: [https://www.semafor.com/article/11/04/2026/us-voters-roundly-reject-data-centers-in-ballot-measures](https://www.semafor.com/article/11/04/2026/us-voters-roundly-reject-data-centers-in-ballot-measures)

生成摘要时出错

---

## 21. Guerrilla bike lanes: San Francisco makes illicit infrastructure permanent (2016)

**原文标题**: Guerrilla bike lanes: San Francisco makes illicit infrastructure permanent (2016)

**原文链接**: [https://99percentinvisible.org/article/guerrilla-bike-lanes-san-francisco-makes-illicit-infrastructure-permanent/](https://99percentinvisible.org/article/guerrilla-bike-lanes-san-francisco-makes-illicit-infrastructure-permanent/)

生成摘要时出错

---

## 22. Ripple-65B Preview: U.S. Open-Weight SOTA on Agentic Coding

**原文标题**: Ripple-65B Preview: U.S. Open-Weight SOTA on Agentic Coding

**原文链接**: [https://www.ricursive.com/ripple](https://www.ricursive.com/ripple)

生成摘要时出错

---

## 23. Geoffrey Hinton: it might turn out we were better off without AI

**原文标题**: Geoffrey Hinton: it might turn out we were better off without AI

**原文链接**: [https://www.theguardian.com/uk-news/2026/nov/03/ai-godfather-geoffrey-hinton-better-off-without-ai](https://www.theguardian.com/uk-news/2026/nov/03/ai-godfather-geoffrey-hinton-better-off-without-ai)

生成摘要时出错

---

## 24. Insects don't swarm at LED lights

**原文标题**: Insects don't swarm at LED lights

**原文链接**: [https://www.birdsoutsidemywindow.org/2026/11/03/insects-dont-swarm-at-led-lights/](https://www.birdsoutsidemywindow.org/2026/11/03/insects-dont-swarm-at-led-lights/)

生成摘要时出错

---

## 25. Claude Code sends your email address to websites

**原文标题**: Claude Code sends your email address to websites

**原文链接**: [https://github.com/anthropics/claude-code/issues/107757](https://github.com/anthropics/claude-code/issues/107757)

生成摘要时出错

---

## 26. Tencent Hy4

**原文标题**: Tencent Hy4

**原文链接**: [https://hy.tencent.ai/research/hy4](https://hy.tencent.ai/research/hy4)

生成摘要时出错

---

## 27. GPT-6 Astra covertly underperforms on safety research

**原文标题**: GPT-6 Astra covertly underperforms on safety research

**原文链接**: [https://alignment.openai.com/misalignment-reports/covert-underperformance-on-safety-research-tasks/](https://alignment.openai.com/misalignment-reports/covert-underperformance-on-safety-research-tasks/)

生成摘要时出错

---

## 28. I wish tech companies knew more about me

**原文标题**: I wish tech companies knew more about me

**原文链接**: [https://rakhim.exotext.com/i-wish-tech-companies-knew-more-about-me](https://rakhim.exotext.com/i-wish-tech-companies-knew-more-about-me)

生成摘要时出错

---

## 29. Democrats win control of the House of Representatives

**原文标题**: Democrats win control of the House of Representatives

**原文链接**: [https://www.nbcnews.com/politics/2026-election/democrats-house-control-midterm-election-wins-trump-check-rcna603397](https://www.nbcnews.com/politics/2026-election/democrats-house-control-midterm-election-wins-trump-check-rcna603397)

生成摘要时出错

---

## 30. Awesome repositories are no longer awesome

**原文标题**: Awesome repositories are no longer awesome

**原文链接**: [https://erikgahner.github.io/posts/2026/awesome-repositories-are-no-longer-awesome/](https://erikgahner.github.io/posts/2026/awesome-repositories-are-no-longer-awesome/)

生成摘要时出错

---

## 31. Starfall – Affordable, routine access to microgravity

**原文标题**: Starfall – Affordable, routine access to microgravity

**原文链接**: [https://www.spacex.com/starfall](https://www.spacex.com/starfall)

生成摘要时出错

---

## 32. Incident with Pull Requests, Git Operations and Issues

**原文标题**: Incident with Pull Requests, Git Operations and Issues

**原文链接**: [https://www.githubstatus.com/incidents/smtdswd1h2w4](https://www.githubstatus.com/incidents/smtdswd1h2w4)

生成摘要时出错

---

## 33. OpenAI to acquire Pierre Computer Company

**原文标题**: OpenAI to acquire Pierre Computer Company

**原文链接**: [https://openai.com/index/openai-to-acquire-pierre/](https://openai.com/index/openai-to-acquire-pierre/)

生成摘要时出错

---

## 34. Download your favourite YouTube videos

**原文标题**: Download your favourite YouTube videos

**原文链接**: [https://criminallyvulgar.dev/you-should-absolutely-download-your-favourite-youtube-videos/](https://criminallyvulgar.dev/you-should-absolutely-download-your-favourite-youtube-videos/)

生成摘要时出错

---

## 35. MS Paint Remote Code Execution Vulnerability

**原文标题**: MS Paint Remote Code Execution Vulnerability

**原文链接**: [https://www.cve.org/CVERecord?id=CVE-2026-83844](https://www.cve.org/CVERecord?id=CVE-2026-83844)

生成摘要时出错

---

## 36. Show HN: After a decade of reversing, I got co-op working in DOS Wing Commander

**原文标题**: Show HN: After a decade of reversing, I got co-op working in DOS Wing Commander

**原文链接**: [https://fireflyk64.github.io/wcmulti/](https://fireflyk64.github.io/wcmulti/)

生成摘要时出错

---

## 37. Verification Is Not Knowledge: Science needs more than answers

**原文标题**: Verification Is Not Knowledge: Science needs more than answers

**原文链接**: [https://blog.cosmos-institute.org/p/verification-is-not-knowledge](https://blog.cosmos-institute.org/p/verification-is-not-knowledge)

生成摘要时出错

---

## 38. Progress on provable inference for large language models

**原文标题**: Progress on provable inference for large language models

**原文链接**: [https://www.anthropic.com/research/provable-inference](https://www.anthropic.com/research/provable-inference)

生成摘要时出错

---

## 39. OpenSSH 10.6p2 Critical workaround for alpine without PAM

**原文标题**: OpenSSH 10.6p2 Critical workaround for alpine without PAM

**原文链接**: [https://www.openssh.org/releasenotes.html#10.6p2](https://www.openssh.org/releasenotes.html#10.6p2)

生成摘要时出错

---

## 40. MCP Explained

**原文标题**: MCP Explained

**原文链接**: [https://mcp-explained.com/](https://mcp-explained.com/)

生成摘要时出错

---

## 41. Synaptics Appears to Use Legal Threats to Block Open-Source DisplayLink Driver

**原文标题**: Synaptics Appears to Use Legal Threats to Block Open-Source DisplayLink Driver

**原文链接**: [https://www.phoronix.com/news/Synaptics-Blocks-Vino-Driver](https://www.phoronix.com/news/Synaptics-Blocks-Vino-Driver)

生成摘要时出错

---

## 42. Window Sweaters

**原文标题**: Window Sweaters

**原文链接**: [https://github.com/saragordic/window-sweaters](https://github.com/saragordic/window-sweaters)

生成摘要时出错

---

## 43. Conductor is joining Meta

**原文标题**: Conductor is joining Meta

**原文链接**: [https://www.conductor.build/announcement](https://www.conductor.build/announcement)

生成摘要时出错

---

## 44. Nasdaq plummets 4% into correction territory

**原文标题**: Nasdaq plummets 4% into correction territory

**原文链接**: [https://www.cnbc.com/2026/11/04/stock-market-today-live-updates.html](https://www.cnbc.com/2026/11/04/stock-market-today-live-updates.html)

生成摘要时出错

---

## 45. Obscure audio codec is a perfect fit for the N64

**原文标题**: Obscure audio codec is a perfect fit for the N64

**原文链接**: [https://phoboslab.org/log/2026/11/n64-ulc-codec](https://phoboslab.org/log/2026/11/n64-ulc-codec)

生成摘要时出错

---

## 46. September in Servo: <progress>, rounded rectangles, and more

**原文标题**: September in Servo: <progress>, rounded rectangles, and more

**原文链接**: [https://servo.org/blog/2026/11/05/september-in-servo/](https://servo.org/blog/2026/11/05/september-in-servo/)

生成摘要时出错

---

## 47. So my ISP was hijacking my DNS

**原文标题**: So my ISP was hijacking my DNS

**原文链接**: [https://www.karthihegde.dev/posts/dns_tampering](https://www.karthihegde.dev/posts/dns_tampering)

生成摘要时出错

---

## 48. OpenSSH 10.6p2 has been released with a workaround for a critical vulnerability

**原文标题**: OpenSSH 10.6p2 has been released with a workaround for a critical vulnerability

**原文链接**: [https://hachyderm.io/@damienmiller/117563026759098135](https://hachyderm.io/@damienmiller/117563026759098135)

生成摘要时出错

---

## 49. Qualcomm Cloud AI 100 Ultra – 150W AI Accelerator Card with 128GB at 548GB/s

**原文标题**: Qualcomm Cloud AI 100 Ultra – 150W AI Accelerator Card with 128GB at 548GB/s

**原文链接**: [https://www.qualcomm.com/data-center/products/cloud-ai-100-ultra](https://www.qualcomm.com/data-center/products/cloud-ai-100-ultra)

生成摘要时出错

---

## 50. The Hackintosh Reborn

**原文标题**: The Hackintosh Reborn

**原文链接**: [https://www.naut.ca/blog/2026/11/05/the-hackintosh-reborn-with-ai/](https://www.naut.ca/blog/2026/11/05/the-hackintosh-reborn-with-ai/)

生成摘要时出错

---

## 51. Baidu released ERNIE 5.5 Flash Base

**原文标题**: Baidu released ERNIE 5.5 Flash Base

**原文链接**: [https://ernie.baidu.com/release/ernie-5-5-flash-base/](https://ernie.baidu.com/release/ernie-5-5-flash-base/)

生成摘要时出错

---

## 52. The lost malloc()

**原文标题**: The lost malloc()

**原文链接**: [https://napcakes.nekoweb.org/posts/malloc/](https://napcakes.nekoweb.org/posts/malloc/)

生成摘要时出错

---

## 53. 'It's just vape, nail, charity shops': Can anything save UK high street?

**原文标题**: 'It's just vape, nail, charity shops': Can anything save UK high street?

**原文链接**: [https://www.theguardian.com/business/2026/nov/04/what-can-save-the-british-high-street-rotherham](https://www.theguardian.com/business/2026/nov/04/what-can-save-the-british-high-street-rotherham)

生成摘要时出错

---

## 54. My psychophysics as a bilateral cochlear implant user

**原文标题**: My psychophysics as a bilateral cochlear implant user

**原文链接**: [https://claude.ai/artifact/L8qsMc3SorytGW3LA81nYf](https://claude.ai/artifact/L8qsMc3SorytGW3LA81nYf)

生成摘要时出错

---

## 55. Everything is an AI scam now

**原文标题**: Everything is an AI scam now

**原文链接**: [https://www.davidralphlewis.co.uk/posts/everything-is-an-ai-scam-now/](https://www.davidralphlewis.co.uk/posts/everything-is-an-ai-scam-now/)

生成摘要时出错

---

## 56. Nasdaq Sinks 5% as Investors Retreat from AI Trade After Election

**原文标题**: Nasdaq Sinks 5% as Investors Retreat from AI Trade After Election

**原文链接**: [https://www.wsj.com/livecoverage/stock-market-today-dow-sp-500-nasdaq-11-05-2026](https://www.wsj.com/livecoverage/stock-market-today-dow-sp-500-nasdaq-11-05-2026)

生成摘要时出错

---

## 57. Debian apt security update (man-in-the-middle)

**原文标题**: Debian apt security update (man-in-the-middle)

**原文链接**: [https://lists.debian.org/debian-security-announce/2026/msg00526.html?pow_referer=](https://lists.debian.org/debian-security-announce/2026/msg00526.html?pow_referer=)

生成摘要时出错

---

## 58. Giant canyon on Mars is still tectonically active

**原文标题**: Giant canyon on Mars is still tectonically active

**原文链接**: [https://lamont.columbia.edu/news/giant-canyon-mars-still-tectonically-active-today](https://lamont.columbia.edu/news/giant-canyon-mars-still-tectonically-active-today)

生成摘要时出错

---

## 59. US midterm elections 2026 live updates: Democrats win Senate control and edge

**原文标题**: US midterm elections 2026 live updates: Democrats win Senate control and edge

**原文链接**: [https://www.theguardian.com/us-news/live/2026/nov/03/midterm-election-results-live-updates](https://www.theguardian.com/us-news/live/2026/nov/03/midterm-election-results-live-updates)

生成摘要时出错

---

## 60. A wave of plastic-free coffee pods and machines

**原文标题**: A wave of plastic-free coffee pods and machines

**原文链接**: [https://www.cnn.com/2026/11/02/food/coffee-machine-plastic-free](https://www.cnn.com/2026/11/02/food/coffee-machine-plastic-free)

生成摘要时出错

---

## 61. Hacking the Xbox 360 Hypervisor Part 3: Bad Update Improvements

**原文标题**: Hacking the Xbox 360 Hypervisor Part 3: Bad Update Improvements

**原文链接**: [https://icode4.coffee/?p=1746](https://icode4.coffee/?p=1746)

生成摘要时出错

---

## 62. Distinct cellular and genetic differences in colorectal cancer in young patients

**原文标题**: Distinct cellular and genetic differences in colorectal cancer in young patients

**原文链接**: [https://www.dana-farber.org/newsroom/news-releases/2026/study-reveals-distinct-cellular-and-genetic-differences-in-colorectal-cancer-in-younger-patients](https://www.dana-farber.org/newsroom/news-releases/2026/study-reveals-distinct-cellular-and-genetic-differences-in-colorectal-cancer-in-younger-patients)

生成摘要时出错

---

## 63. Hungary: Communist-era files released, up to 60k former agents revealed

**原文标题**: Hungary: Communist-era files released, up to 60k former agents revealed

**原文链接**: [https://www.euronews.com/2026/11/04/hungary-communist-era-files-opened-up-to-60000-former-agents-revealed](https://www.euronews.com/2026/11/04/hungary-communist-era-files-opened-up-to-60000-former-agents-revealed)

生成摘要时出错

---

## 64. BYD doubles its Brazil market share to 9.7% a year after opening its local plant

**原文标题**: BYD doubles its Brazil market share to 9.7% a year after opening its local plant

**原文链接**: [https://www.bloomberg.com/news/articles/2026-11-03/china-s-byd-doubles-market-share-in-brazil-with-new-plant-eyed](https://www.bloomberg.com/news/articles/2026-11-03/china-s-byd-doubles-market-share-in-brazil-with-new-plant-eyed)

生成摘要时出错

---

## 65. Show HN: A decent text-to-image model trained for ~$20K (Apache 2.0 Weights)

**原文标题**: Show HN: A decent text-to-image model trained for ~$20K (Apache 2.0 Weights)

**原文链接**: [https://www.linum.ai/field-notes/pjit-21k](https://www.linum.ai/field-notes/pjit-21k)

生成摘要时出错

---

## 66. Have I befriended a murderer?

**原文标题**: Have I befriended a murderer?

**原文链接**: [https://longreads.com/2026/11/03/murder-friendship-doubt/](https://longreads.com/2026/11/03/murder-friendship-doubt/)

生成摘要时出错

---

## 67. Education shouldn't be held for ransom

**原文标题**: Education shouldn't be held for ransom

**原文链接**: [https://blog.kagi.com/education-should-not-be-held-for-ransom](https://blog.kagi.com/education-should-not-be-held-for-ransom)

生成摘要时出错

---

## 68. Image of our satellite-choked night skies

**原文标题**: Image of our satellite-choked night skies

**原文链接**: [https://kottke.org/26/11/stunning-image-of-our-satellite-choked-night-skies](https://kottke.org/26/11/stunning-image-of-our-satellite-choked-night-skies)

生成摘要时出错

---

## 69. Being a kid making games in the early 2000s

**原文标题**: Being a kid making games in the early 2000s

**原文链接**: [https://jaytholen.net/teengamedev/](https://jaytholen.net/teengamedev/)

生成摘要时出错

---

## 70. This Month in Ladybird – October 2026

**原文标题**: This Month in Ladybird – October 2026

**原文链接**: [https://ladybird.org/newsletter/2026-10-31/](https://ladybird.org/newsletter/2026-10-31/)

生成摘要时出错

---

## 71. Show HN: I built a tool that prices a pre-built PC part by part

**原文标题**: Show HN: I built a tool that prices a pre-built PC part by part

**原文链接**: [https://pcdealcheck.com/](https://pcdealcheck.com/)

生成摘要时出错

---

## 72. Evergreen: A Provably Safe Systems Language

**原文标题**: Evergreen: A Provably Safe Systems Language

**原文链接**: [https://evergreenlang.net](https://evergreenlang.net)

生成摘要时出错

---

## 73. $2.5T has been wiped from US stocks

**原文标题**: $2.5T has been wiped from US stocks

**原文链接**: [https://finlaws.substack.com/p/25t-has-been-wiped-from-us-stocks](https://finlaws.substack.com/p/25t-has-been-wiped-from-us-stocks)

生成摘要时出错

---

## 74. YC's Garry Tan uses AI agents so much, he spends up to $200K a year on tokens

**原文标题**: YC's Garry Tan uses AI agents so much, he spends up to $200K a year on tokens

**原文链接**: [https://techcrunch.com/2026/11/02/y-combinators-garry-tan-uses-ai-agents-so-much-he-spends-up-to-200k-a-year-on-tokens/](https://techcrunch.com/2026/11/02/y-combinators-garry-tan-uses-ai-agents-so-much-he-spends-up-to-200k-a-year-on-tokens/)

生成摘要时出错

---

## 75. Debian apt security update: man-in-the-middle arbitrary code execution

**原文标题**: Debian apt security update: man-in-the-middle arbitrary code execution

**原文链接**: [https://lists.debian.org/debian-security-announce/2026/msg00526.html](https://lists.debian.org/debian-security-announce/2026/msg00526.html)

生成摘要时出错

---

## 76. Democrats Rout GOP

**原文标题**: Democrats Rout GOP

**原文链接**: [https://www.nytimes.com/live/2026/11/03/us/midterms-2026-election-day-trump](https://www.nytimes.com/live/2026/11/03/us/midterms-2026-election-day-trump)

生成摘要时出错

---

## 77. We can do better than line-buffered output

**原文标题**: We can do better than line-buffered output

**原文链接**: [https://nullprogram.com/blog/2026/11/05/](https://nullprogram.com/blog/2026/11/05/)

生成摘要时出错

---

## 78. Vibe Coding Keypad

**原文标题**: Vibe Coding Keypad

**原文链接**: [https://www.keychron.com/products/keychron-f4-he-8k-vibe-coding-keypad](https://www.keychron.com/products/keychron-f4-he-8k-vibe-coding-keypad)

生成摘要时出错

---

## 79. Hackers hit French national blood bank

**原文标题**: Hackers hit French national blood bank

**原文链接**: [https://www.telegraph.co.uk/world-news/2026/11/04/hackers-hit-french-blood-bank/](https://www.telegraph.co.uk/world-news/2026/11/04/hackers-hit-french-blood-bank/)

生成摘要时出错

---

## 80. A map of 5000+ midterm ads

**原文标题**: A map of 5000+ midterm ads

**原文链接**: [https://admap.org/](https://admap.org/)

生成摘要时出错

---

## 81. Milkman – The Better Alternative to Postman

**原文标题**: Milkman – The Better Alternative to Postman

**原文链接**: [https://milkman.dev/](https://milkman.dev/)

生成摘要时出错

---

## 82. Arrows to arrows, categories to queries (2025)

**原文标题**: Arrows to arrows, categories to queries (2025)

**原文链接**: [https://reasonablypolymorphic.com/blog/arrows-to-arrows/](https://reasonablypolymorphic.com/blog/arrows-to-arrows/)

生成摘要时出错

---

## 83. My gym forced a social media down my throat. So I reverse-engineered its app

**原文标题**: My gym forced a social media down my throat. So I reverse-engineered its app

**原文链接**: [https://shayon.work/blog/reverse-engineering-gym-pass](https://shayon.work/blog/reverse-engineering-gym-pass)

生成摘要时出错

---

## 84. California Gov Newsom commutes death sentences for all 548 people on death row

**原文标题**: California Gov Newsom commutes death sentences for all 548 people on death row

**原文链接**: [https://www.bbc.com/news/articles/cqrkyyd2j8mvo](https://www.bbc.com/news/articles/cqrkyyd2j8mvo)

生成摘要时出错

---

## 85. Death Comes for XSLT

**原文标题**: Death Comes for XSLT

**原文链接**: [https://dbushell.com/2026/11/03/xslt-rip/](https://dbushell.com/2026/11/03/xslt-rip/)

生成摘要时出错

---

## 86. Tencent Launches Hy4, One of the Leading Open-Source AI Models

**原文标题**: Tencent Launches Hy4, One of the Leading Open-Source AI Models

**原文链接**: [https://www.tencent.com/tencent-launches-hy4-joining-the-ranks-of-the-worlds-leading-open-source-ai-models/](https://www.tencent.com/tencent-launches-hy4-joining-the-ranks-of-the-worlds-leading-open-source-ai-models/)

生成摘要时出错

---

