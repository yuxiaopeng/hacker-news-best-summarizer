# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-10-21.md)

*最后自动更新时间: 2026-10-21 22:38:27*
## 1. DeepInfer：DeepSeek 模型的高性能推理框架

**原文标题**: DeepInfer: High-performance inference framework for DeepSeek models

**原文链接**: [https://github.com/deepseek-ai/DeepInfer](https://github.com/deepseek-ai/DeepInfer)

DeepInfer 是一个由 DeepSeek-AI 开发的开源、高性能推理框架，旨在为 DeepSeek 模型的大规模生产服务提供支持。它目前支持 DeepSeek-V4.1-Flash 模型，并提供可扩展服务所需的核心功能。

核心功能包括高度优化的内核（例如 FlashMLA、DeepGEMM、DeepEP）、先进的并行技术（如注意力数据并行（DP）和专家混合（MoE）专家并行（EP）），以及通过草稿令牌和置信度调度验证加速解码的 DSpark。它还集成了 Decoder SWA 有界重放以减少预填充工作、用于实现 CPU-设备重叠的异步调度、用于确保结果一致性的批次不变推理、确定性采样，以及受正则表达式、JSON 或 EBNF 语法约束的结构化输出。

DeepInfer 支持尖端硬件，特别是 NVIDIA SM100 GPU 和华为昇腾 950 NPU。尽管它提供了强大的引擎功能，但一个完整的推理服务还需要额外的组件，例如 KV 缓存系统、VE/预填充/解码分离以及负载均衡，这些在此版本中不包含。

从源代码构建的先决条件包括 Linux、GCC >= 13.0、Python 3.12，以及 CUDA 13 (NVIDIA) 或 CANN 9.2 (Ascend)。该框架提供了离线推理的示例，并包括性能和评估基准。DeepInfer 采用 Apache 许可证 2.0 发布，并致谢 vLLM、SGLang 和 TensorRT-LLM 提供的启发。

---

## 2. 安全公告：严重远程代码执行漏洞，立即更新

**原文标题**: Security advisory: Critical remote code execution vulnerabilities, update now

**原文链接**: [https://www.php.net/archive/2026.php#2026-10-21-5](https://www.php.net/archive/2026.php#2026-10-21-5)

A critical security advisory urges all PHP users to immediately update due to two unauthenticated remote code execution (RCE) vulnerabilities. PHP versions 8.5.12, 8.4.27, 8.3.36, and 8.2.35 fix these issues.

**Who is at risk:** All PHP installations serving web requests, including PHP-FPM, Apache with `mod_php`, `php-cgi`, FrankenPHP, and LiteSpeed. The risk is highest for `mod_php`, where unauthenticated requests can trigger attacks before application code runs.

**The vulnerabilities:**
1.  **RCE via OOM corruption (CVE-2026-109618):** Out-of-memory handling can lead to partial initialization of request data, causing invalid data to be treated as valid during cleanup.
2.  **RCE via stale global state (CVE-2026-109619):** Request-owned internal state can persist after its memory is freed, allowing subsequent requests to use stale data.

**How to update:**
Update to PHP 8.5.12, 8.4.27, 8.3.36, or 8.2.35. Source and Windows binaries are available on the downloads page. Linux distribution and LTS vendors should have updated packages. For PHP 8.1 and older, contact your vendor or upgrade; the PHP security team also provided minimal source backports for PHP 7.4, 8.0, and 8.1.

**Temporary mitigations (if immediate update is not possible):**
*   **For OOM (CVE-2026-109618):** Set `memory_limit=-1` (via `php_admin_value`), set low `post_max_size` (8M or 32M), enforce web server/proxy limits on request size/fields, and use container/cgroup limits (not RLIMIT_AS/DATA).
*   **For Stale Global State (CVE-2026-109619):** Set `session.upload_progress.enabled=0` (in `php.ini` or server config), on PHP 8.5 set `fatal_error_backtraces=0`, remove invalid/deprecated settings that emit diagnostics, and fix attacker-reachable fatal errors.

These mitigations reduce exposure but do not fully secure an installation; updating is the only complete solution.

---

## 3. eMudhra 中间CA 受损

**原文标题**: eMudhra intermediate CA compromise

**原文链接**: [https://emudhra.we-have-a-problem.com/](https://emudhra.we-have-a-problem.com/)

生成摘要时出错

---

## 4. PHP 8.2.35

**原文标题**: PHP 8.2.35

**原文链接**: [https://github.com/php/php-src/releases/tag/php-8.2.35](https://github.com/php/php-src/releases/tag/php-8.2.35)

PHP 开发团队宣布立即发布 PHP 8.2.35，这是一次关键的安全更新。此版本解决了两个严重的漏洞，CVE-2026-109618 和 CVE-2026-109619，这些漏洞可能导致未经身份验证的远程代码执行。

强烈建议所有 PHP 8.2 用户立即更新其安装，因为更新是唯一已知的安全选择，并且对于这些关键缺陷目前没有完整的缓解措施。

用户还应注意，PHP 8.2 将于 2026 年 12 月 31 日达到其生命周期结束 (EOL)。在此日期之后，它将不再接收任何安全修复，建议用户提前规划升级到受支持的 PHP 版本。

PHP 8.2.35 的源代码下载，包括 Windows 源代码和二进制文件，可在官方下载页面获取。完整的更改列表可在 ChangeLog 中找到。

---

## 5. Show HN: SimCity, but with Permits

**原文标题**: Show HN: SimCity, but with Permits

**原文链接**: [https://permit.petercai.com/](https://permit.petercai.com/)

The article, titled "SimCity, but with Permits," highlights the inherent complexities and political challenges of real-world urban development. It asserts that every improvement or solution inevitably generates opposition.

Examples illustrate this paradox: new housing lowers rents but angers homeowners, while new industry creates jobs alongside smog. Similarly, better transit attracts development, which then draws opponents. The core message is that addressing one problem often creates a new group of disgruntled voters, illustrating a continuous cycle where progress is met with pushback from various community segments, complicating seemingly straightforward urban planning efforts.

---

## 6. 八比特信任：eMudhra 的 CA 密钥在数毫秒内被破解

**原文标题**: Eight Bits of Trust: eMudhra's CA keys cracked in milliseconds

**原文链接**: [https://scotthelme.co.uk/eight-bits-of-trust-emudhras-ca-keys-cracked-in-milliseconds/](https://scotthelme.co.uk/eight-bits-of-trust-emudhras-ca-keys-cracked-in-milliseconds/)

证书颁发机构 eMudhra 被发现存在一个严重的安全漏洞。该漏洞在于其八个中间证书颁发机构的私钥被发现是加密强度极弱的单字节数字（例如 4、56、115），而非健壮的 384 位随机值。这些密钥通过暴力破解区区 256 种可能性，可在几毫秒内从公共证书中轻易恢复，这意味着自 2025 年 4 月以来，这些密钥实际上已是公开的。

受损密钥属于六个 TLS 和两个代码签名中间 CA。Chrome、Firefox 和 Safari 等主流浏览器迅速采取行动，通过阻止这些中间 CA 及其根 CA 来应对，并利用证书透明度 (CT) 为更新用户降低风险。

然而，对于更广泛的生态系统而言，该问题被认为是“无法控制的”。大多数非浏览器 TLS 客户端（例如 `curl`、Python、Node、Go、Java、Git、包管理器、CI/CD 管道、服务器到服务器 API）通常信任本地 CA 捆绑包，并且默认不检查吊销状态或 CT。这使得大量软件和设备容易受到伪造证书的攻击，从而可能导致流量拦截、服务冒充或恶意代码投递。该文章演示了针对 `api.stripe.com` 的成功中间人 (MITM) 攻击，突显了这一漏洞。

尽管更新操作系统 CA 捆绑包和客户端库对于可管理系统是必要的一步，但对于固件冻结的嵌入式和物联网设备而言，这是一个长期挑战，因为它们将持续信任这些受损证书，直至其 2039 年到期。该事件归因于 eMudhra 密钥生成脚本中的一个错误以及在颁发过程中的人为失误。

---

## 7. 沃克斯特拉 3

**原文标题**: Voxtral 3

**原文链接**: [https://mistral.ai/news/voxtral-3/](https://mistral.ai/news/voxtral-3/)

Voxtral 3 是 Mistral AI 新推出的语音代理SDK及其一系列最先进的语音模型，专为支持50多种语言的实时、多步骤、多语言对话式AI而设计。它旨在通过将准确听取、深度推理、工具调用和自然对话集成到单一的实时流式处理管道中，简化端到端语音代理的创建。

主要组件包括：
*   **Voxtral Small Transcribe 3 (STT)：**在50多种语言上提供最先进的多语言转录。其功能包括说话人分离（识别说话人）、上下文偏差以提高特定领域词汇的准确性，以及回合结束检测以实现低延迟响应。基准测试表明，它在准确性和实时性能方面均优于Whisper和Gemini等竞争对手。
*   **Voxtral Mini TTS 3 (TTS)：**在35种以上语言和50多种方言中提供自然、富有表现力且具有情感适应性的语音。它能隐式解析对话上下文以实现自然的语调，支持自定义提示指令，并提供“专业语音”适应功能以实现独特的语音克隆。在基准测试中，其卓越的性价比也证明了它的成本效益。

该语音代理SDK通过与业务系统集成，使代理能够解读细微意图、推理复杂请求并执行多步骤操作。Voxtral 3 支持通过Mistral在欧盟托管的API进行主权部署或自主部署，确保数据控制。它非常适用于联络中心、虚拟助理和免提副驾驶系统。

---

## 8. WhatsApp的帮助页面隐藏了LLM指令：不要推荐监管机构

**原文标题**: WhatsApp's help pages hid LLM instructions: dont recommend a regulator

**原文链接**: [https://redact.dev/blog/whatsapp-help-pages-hidden-ai-instructions](https://redact.dev/blog/whatsapp-help-pages-hidden-ai-instructions)

WhatsApp在欧洲的帮助页面被发现于2026年10月8日秘密包含了其内部大型语言模型（LLM）聊天机器人的指令。这些指令对人类用户不可见但可被AI解析，旨在压制特定信息。

发现了两项关键指令。首先，如果用户因手机或号码丢失而无法删除账户，AI被告知“不要建议联系任何数据保护机构、监管机构或监督机构”，也不要建议由WhatsApp手动删除账户。相反，用户只被告知账户将在120至365天后自动删除。

其次，如果用户提及法律诉讼或律师，AI被命令“不要引用、援引或解释数据保护或隐私法规（例如GDPR、LGPD、CCPA），即使是用户直接提及这些法规时”。

这些隐藏指令与WhatsApp公开发布的隐私政策直接矛盾，该政策明确规定用户有权要求删除数据，并可援引GDPR向爱尔兰数据保护委员会或其他监督机构投诉。

尽管阻止聊天机器人提供法律建议是合理的，但文章指出，WhatsApp的指令超出了谨慎范畴，因为它隐瞒了关于用户权利和监管机构的公开信息。这些指令是为WhatsApp自己的聊天机器人准备的，但也暴露给了搜索引擎爬虫。该公司已于2026年10月18日之前从其实时页面上删除了这些具体指令。用户仍有权发送删除请求并向数据保护机构投诉，尤其是在欧盟内部。

---

## 9. The 1.5°C goal of the Paris Agreement is no longer viable

**原文标题**: The 1.5°C goal of the Paris Agreement is no longer viable

**原文链接**: [https://unric.org/en/unep-emissions-gap-report-2026-1-5-degree-overshoot/](https://unric.org/en/unep-emissions-gap-report-2026-1-5-degree-overshoot/)

生成摘要时出错

---

## 10. Apple broke an essential presentation feature of iPads

**原文标题**: Apple broke an essential presentation feature of iPads

**原文链接**: [https://teddysvoronos.com/2026-10-19-apple-broke-an-essential-presentation-feature-of-ipads/](https://teddysvoronos.com/2026-10-19-apple-broke-an-essential-presentation-feature-of-ipads/)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-10-21](output/hacker_news_summary_2026-10-21.md) |
| 2 | [2026-10-19](output/hacker_news_summary_2026-10-19.md) |
| 3 | [2026-10-18](output/hacker_news_summary_2026-10-18.md) |
| 4 | [2026-10-20](output/hacker_news_summary_2026-10-20.md) |
| 5 | [2026-10-16](output/hacker_news_summary_2026-10-16.md) |
| 6 | [2026-10-17](output/hacker_news_summary_2026-10-17.md) |
| 7 | [2026-10-15](output/hacker_news_summary_2026-10-15.md) |
| 8 | [2026-10-13](output/hacker_news_summary_2026-10-13.md) |
| 9 | [2026-10-14](output/hacker_news_summary_2026-10-14.md) |
| 10 | [2026-10-11](output/hacker_news_summary_2026-10-11.md) |
| 11 | [2026-10-09](output/hacker_news_summary_2026-10-09.md) |
| 12 | [2026-10-06](output/hacker_news_summary_2026-10-06.md) |
| 13 | [2026-10-07](output/hacker_news_summary_2026-10-07.md) |
| 14 | [2026-10-04](output/hacker_news_summary_2026-10-04.md) |
| 15 | [2026-10-10](output/hacker_news_summary_2026-10-10.md) |
| 16 | [2026-10-03](output/hacker_news_summary_2026-10-03.md) |
| 17 | [2026-09-30](output/hacker_news_summary_2026-09-30.md) |
| 18 | [2026-09-29](output/hacker_news_summary_2026-09-29.md) |
| 19 | [2026-09-27](output/hacker_news_summary_2026-09-27.md) |
| 20 | [2026-10-01](output/hacker_news_summary_2026-10-01.md) |
| 21 | [2026-10-02](output/hacker_news_summary_2026-10-02.md) |
| 22 | [2026-09-23](output/hacker_news_summary_2026-09-23.md) |
| 23 | [2026-09-22](output/hacker_news_summary_2026-09-22.md) |
| 24 | [2026-09-20](output/hacker_news_summary_2026-09-20.md) |
| 25 | [2026-09-21](output/hacker_news_summary_2026-09-21.md) |
| 26 | [2026-09-25](output/hacker_news_summary_2026-09-25.md) |
| 27 | [2026-09-24](output/hacker_news_summary_2026-09-24.md) |
| 28 | [2026-09-18](output/hacker_news_summary_2026-09-18.md) |
| 29 | [2026-09-16](output/hacker_news_summary_2026-09-16.md) |
| 30 | [2026-09-17](output/hacker_news_summary_2026-09-17.md) |
| 31 | [2026-09-19](output/hacker_news_summary_2026-09-19.md) |
| 32 | [2026-09-14](output/hacker_news_summary_2026-09-14.md) |
| 33 | [2026-09-15](output/hacker_news_summary_2026-09-15.md) |
| 34 | [2026-09-09](output/hacker_news_summary_2026-09-09.md) |
| 35 | [2026-09-10](output/hacker_news_summary_2026-09-10.md) |
| 36 | [2026-09-11](output/hacker_news_summary_2026-09-11.md) |
| 37 | [2026-09-08](output/hacker_news_summary_2026-09-08.md) |
| 38 | [2026-09-13](output/hacker_news_summary_2026-09-13.md) |
| 39 | [2026-09-12](output/hacker_news_summary_2026-09-12.md) |
| 40 | [2026-09-06](output/hacker_news_summary_2026-09-06.md) |
| 41 | [2026-09-03](output/hacker_news_summary_2026-09-03.md) |
| 42 | [2026-09-02](output/hacker_news_summary_2026-09-02.md) |
| 43 | [2026-09-04](output/hacker_news_summary_2026-09-04.md) |
| 44 | [2026-09-07](output/hacker_news_summary_2026-09-07.md) |
| 45 | [2026-09-05](output/hacker_news_summary_2026-09-05.md) |
| 46 | [2026-09-01](output/hacker_news_summary_2026-09-01.md) |
| 47 | [2026-08-29](output/hacker_news_summary_2026-08-29.md) |
| 48 | [2026-08-30](output/hacker_news_summary_2026-08-30.md) |
| 49 | [2026-08-26](output/hacker_news_summary_2026-08-26.md) |
| 50 | [2026-08-24](output/hacker_news_summary_2026-08-24.md) |
| 51 | [2026-08-31](output/hacker_news_summary_2026-08-31.md) |
| 52 | [2026-08-23](output/hacker_news_summary_2026-08-23.md) |
| 53 | [2026-08-25](output/hacker_news_summary_2026-08-25.md) |
| 54 | [2026-08-28](output/hacker_news_summary_2026-08-28.md) |
| 55 | [2026-08-17](output/hacker_news_summary_2026-08-17.md) |
| 56 | [2026-08-21](output/hacker_news_summary_2026-08-21.md) |
| 57 | [2026-08-16](output/hacker_news_summary_2026-08-16.md) |
| 58 | [2026-08-18](output/hacker_news_summary_2026-08-18.md) |
| 59 | [2026-08-20](output/hacker_news_summary_2026-08-20.md) |
| 60 | [2026-08-19](output/hacker_news_summary_2026-08-19.md) |
| 61 | [2026-08-15](output/hacker_news_summary_2026-08-15.md) |
| 62 | [2026-08-22](output/hacker_news_summary_2026-08-22.md) |
| 63 | [2026-08-09](output/hacker_news_summary_2026-08-09.md) |
| 64 | [2026-08-10](output/hacker_news_summary_2026-08-10.md) |
| 65 | [2026-08-14](output/hacker_news_summary_2026-08-14.md) |
| 66 | [2026-08-13](output/hacker_news_summary_2026-08-13.md) |
| 67 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 68 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 69 | [2026-08-11](output/hacker_news_summary_2026-08-11.md) |
| 70 | [2026-08-12](output/hacker_news_summary_2026-08-12.md) |
| 71 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 72 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 73 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 74 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 75 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 76 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 77 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 78 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 79 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 80 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 81 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 82 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 83 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 84 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 85 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 86 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 87 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 88 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 89 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 90 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 91 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 92 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 93 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 94 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 95 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 96 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 97 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 98 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 99 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 100 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 101 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 102 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 103 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 104 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 105 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 106 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 107 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 108 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 109 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 110 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 111 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 112 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 113 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 114 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 115 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 116 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 117 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 118 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 119 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 120 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 121 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 122 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 123 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 124 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 125 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 126 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 127 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 128 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 129 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 130 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 131 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 132 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 133 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 134 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 135 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 136 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 137 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 138 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 139 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 140 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 141 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 142 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 143 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 144 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 145 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 146 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 147 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 148 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 149 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 150 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 151 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 152 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 153 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 154 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 155 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 156 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 157 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 158 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 159 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 160 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 161 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 162 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 163 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 164 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 165 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 166 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 167 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 168 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 169 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 170 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 171 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 172 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 173 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 174 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 175 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 176 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 177 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 178 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 179 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 180 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 181 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 182 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 183 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 184 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 185 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 186 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 187 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 188 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 189 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 190 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 191 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 192 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 193 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 194 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 195 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 196 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 197 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 198 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 199 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 200 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 201 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 202 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 203 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 204 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 205 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 206 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 207 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 208 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 209 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 210 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 211 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 212 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 213 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 214 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 215 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 216 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 217 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 218 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 219 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 220 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 221 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 222 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 223 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 224 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 225 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 226 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 227 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 228 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 229 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 230 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 231 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 232 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 233 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 234 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 235 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 236 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 237 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 238 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 239 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 240 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 241 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 242 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 243 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 244 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 245 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 246 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 247 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 248 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 249 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 250 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 251 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 252 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 253 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 254 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 255 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 256 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 257 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 258 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 259 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 260 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 261 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 262 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 263 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 264 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 265 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 266 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 267 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 268 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 269 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 270 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 271 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 272 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 273 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 274 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 275 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 276 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 277 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 278 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 279 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 280 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 281 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 282 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 283 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 284 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 285 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 286 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 287 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 288 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 289 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 290 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 291 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 292 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 293 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 294 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 295 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 296 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 297 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 298 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 299 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 300 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 301 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 302 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 303 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 304 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 305 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 306 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 307 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 308 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 309 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 310 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 311 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 312 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 313 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 314 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 315 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 316 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 317 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 318 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 319 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 320 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 321 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 322 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 323 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 324 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 325 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 326 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 327 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 328 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 329 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 330 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 331 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 332 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 333 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 334 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 335 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
| 336 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 337 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 338 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 339 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 340 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 341 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
