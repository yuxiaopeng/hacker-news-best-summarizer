# Hacker News 热门文章摘要 (2026-10-21)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

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

## 11. The Future of CSS

**原文标题**: The Future of CSS

**原文链接**: [https://www.joshwcomeau.com/css/interop-2027/](https://www.joshwcomeau.com/css/interop-2027/)

生成摘要时出错

---

## 12. Today's PHP security release, and how we're strengthening security

**原文标题**: Today's PHP security release, and how we're strengthening security

**原文链接**: [https://thephp.foundation/blog/2026/10/21/todays-php-security-release-and-how-were-strengthening-php-security/](https://thephp.foundation/blog/2026/10/21/todays-php-security-release-and-how-were-strengthening-php-security/)

生成摘要时出错

---

## 13. OpenBSD 8.0

**原文标题**: OpenBSD 8.0

**原文链接**: [https://www.openbsd.org/80.html](https://www.openbsd.org/80.html)

生成摘要时出错

---

## 14. The No Kings Takedown Is Why You Shouldn't Rent Your Megaphone from Zuck

**原文标题**: The No Kings Takedown Is Why You Shouldn't Rent Your Megaphone from Zuck

**原文链接**: [https://www.techdirt.com/2026/10/20/accident-or-not-the-no-kings-takedown-is-why-you-shouldnt-rent-your-megaphone-from-zuck/](https://www.techdirt.com/2026/10/20/accident-or-not-the-no-kings-takedown-is-why-you-shouldnt-rent-your-megaphone-from-zuck/)

生成摘要时出错

---

## 15. What shall I teach my son?

**原文标题**: What shall I teach my son?

**原文链接**: [https://stevekrouse.com/ends](https://stevekrouse.com/ends)

生成摘要时出错

---

## 16. Facebook Pages require paid subscription to post more than two links per month

**原文标题**: Facebook Pages require paid subscription to post more than two links per month

**原文链接**: [https://mastodon.gamedev.place/@AshleyGullen/117473851565913919](https://mastodon.gamedev.place/@AshleyGullen/117473851565913919)

生成摘要时出错

---

## 17. An ad-free Android TV

**原文标题**: An ad-free Android TV

**原文链接**: [https://cretezy.com/2026/ad-free-android-tv](https://cretezy.com/2026/ad-free-android-tv)

生成摘要时出错

---

## 18. Tsrs: A Port of TypeScript to Rust

**原文标题**: Tsrs: A Port of TypeScript to Rust

**原文链接**: [https://blog.cloudflare.com/typescript-rust-port/](https://blog.cloudflare.com/typescript-rust-port/)

生成摘要时出错

---

## 19. PHP2Shell: AI uncovers critical RCE in PHP

**原文标题**: PHP2Shell: AI uncovers critical RCE in PHP

**原文链接**: [https://www.wiz.io/blog/php2shell-php-rce](https://www.wiz.io/blog/php2shell-php-rce)

生成摘要时出错

---

## 20. EA is shutting down BioWare

**原文标题**: EA is shutting down BioWare

**原文链接**: [https://www.theverge.com/games/1015647/ea-is-shutting-down-bioware](https://www.theverge.com/games/1015647/ea-is-shutting-down-bioware)

生成摘要时出错

---

## 21. MicroG: Free-libre re-implementation of Google's proprietary Android user space

**原文标题**: MicroG: Free-libre re-implementation of Google's proprietary Android user space

**原文链接**: [https://github.com/microg/GmsCore/wiki](https://github.com/microg/GmsCore/wiki)

生成摘要时出错

---

## 22. Ofcom concedes defeat in 4chan case

**原文标题**: Ofcom concedes defeat in 4chan case

**原文链接**: [https://prestonbyrne.com/2026/10/20/ofcom-concedes-defeat/](https://prestonbyrne.com/2026/10/20/ofcom-concedes-defeat/)

生成摘要时出错

---

## 23. Google Cloud outage affects almost all banking and other operations in Europe

**原文标题**: Google Cloud outage affects almost all banking and other operations in Europe

**原文链接**: [https://www.neowin.net/news/google-cloud-outage-takes-down-hsbc-revolut-bank-of-scotland-llyods-equifax-more/](https://www.neowin.net/news/google-cloud-outage-takes-down-hsbc-revolut-bank-of-scotland-llyods-equifax-more/)

生成摘要时出错

---

## 24. How I got over 300 Tor exit nodes removed

**原文标题**: How I got over 300 Tor exit nodes removed

**原文链接**: [https://kaba.cx/posts/20261020_Tor/](https://kaba.cx/posts/20261020_Tor/)

生成摘要时出错

---

## 25. AfD Leak: What 421,179 Hacked Emails Show about the German Far Right

**原文标题**: AfD Leak: What 421,179 Hacked Emails Show about the German Far Right

**原文链接**: [https://www.heistberlin.com/news/afd-leak-what-421-179-hacked-emails-show-about-the-german-far-right/](https://www.heistberlin.com/news/afd-leak-what-421-179-hacked-emails-show-about-the-german-far-right/)

生成摘要时出错

---

## 26. Muse exposes users' personal and business secrets when they share conversations

**原文标题**: Muse exposes users' personal and business secrets when they share conversations

**原文链接**: [https://arstechnica.com/security/2026/10/meta-muse-exposes-users-personal-and-business-secrets-when-they-share-conversations/](https://arstechnica.com/security/2026/10/meta-muse-exposes-users-personal-and-business-secrets-when-they-share-conversations/)

生成摘要时出错

---

## 27. Google open-sources TorchTPU, a native PyTorch back end for TPUs

**原文标题**: Google open-sources TorchTPU, a native PyTorch back end for TPUs

**原文链接**: [https://github.com/google-pytorch/torch_tpu](https://github.com/google-pytorch/torch_tpu)

生成摘要时出错

---

## 28. Compromised LiteLLM 1.107.0 on PyPI Installs a Credential Stealer and Backdoor

**原文标题**: Compromised LiteLLM 1.107.0 on PyPI Installs a Credential Stealer and Backdoor

**原文链接**: [https://safedep.io/litellm-pypi-compromise-credential-stealer-backdoor/](https://safedep.io/litellm-pypi-compromise-credential-stealer-backdoor/)

生成摘要时出错

---

## 29. Publish fake stats, get cited in LLMs

**原文标题**: Publish fake stats, get cited in LLMs

**原文链接**: [https://peec.ai/blog/publish-stats-get-cited-the-tactic-that-put-my-data-all-over-the-web](https://peec.ai/blog/publish-stats-get-cited-the-tactic-that-put-my-data-all-over-the-web)

生成摘要时出错

---

## 30. DuckDB 2.0.0 LTS “Cinnamon Teal”

**原文标题**: DuckDB 2.0.0 LTS “Cinnamon Teal”

**原文链接**: [https://duckdb.org/2026/10/21/announcing-duckdb-200](https://duckdb.org/2026/10/21/announcing-duckdb-200)

生成摘要时出错

---

## 31. Sixteen years after Deepwater Horizon, deep sea life shows few signs of recovery

**原文标题**: Sixteen years after Deepwater Horizon, deep sea life shows few signs of recovery

**原文链接**: [https://e360.yale.edu/digest/deepwater-horizon-deep-sea-recovery](https://e360.yale.edu/digest/deepwater-horizon-deep-sea-recovery)

生成摘要时出错

---

## 32. Mistral Large 4

**原文标题**: Mistral Large 4

**原文链接**: [https://mistral.ai/news/mistral-large-4/](https://mistral.ai/news/mistral-large-4/)

生成摘要时出错

---

## 33. Lula supporters protest against Meta to denounce its 'electoral interference'

**原文标题**: Lula supporters protest against Meta to denounce its 'electoral interference'

**原文链接**: [https://efe.com/english/latest-news/2026-10-20/lula-supporters-protest-against-meta-to-denounce-its-electoral-interference/](https://efe.com/english/latest-news/2026-10-20/lula-supporters-protest-against-meta-to-denounce-its-electoral-interference/)

生成摘要时出错

---

## 34. The Other Epidemic: Trying to get off benzodiazepines

**原文标题**: The Other Epidemic: Trying to get off benzodiazepines

**原文链接**: [https://www.thebeliever.net/the-other-epidemic/](https://www.thebeliever.net/the-other-epidemic/)

生成摘要时出错

---

## 35. PHP 8.5.12, 8.4.27, 8.3.36 and 8.2.35 out

**原文标题**: PHP 8.5.12, 8.4.27, 8.3.36 and 8.2.35 out

**原文链接**: [https://www.php.net/index.php](https://www.php.net/index.php)

生成摘要时出错

---

## 36. Dutch National Cyber Security Center is Offline because it uses PHP

**原文标题**: Dutch National Cyber Security Center is Offline because it uses PHP

**原文链接**: [https://www.ncsc.nl/actueel](https://www.ncsc.nl/actueel)

生成摘要时出错

---

## 37. Feds suspect ransom negotiator ran ShinyHunters extortion site

**原文标题**: Feds suspect ransom negotiator ran ShinyHunters extortion site

**原文链接**: [https://krebsonsecurity.com/2026/10/feds-suspect-ransom-negotiator-ran-shinyhunters-extortion-site/](https://krebsonsecurity.com/2026/10/feds-suspect-ransom-negotiator-ran-shinyhunters-extortion-site/)

生成摘要时出错

---

## 38. How abliterated models can get you pwned

**原文标题**: How abliterated models can get you pwned

**原文链接**: [https://projectdiscovery.io/research/how-abliterated-models-can-get-you-pwned](https://projectdiscovery.io/research/how-abliterated-models-can-get-you-pwned)

生成摘要时出错

---

## 39. France's supermarket fridges were vulnerable online for months

**原文标题**: France's supermarket fridges were vulnerable online for months

**原文链接**: [https://ipinfo.io/blog/france-fridges-hack](https://ipinfo.io/blog/france-fridges-hack)

生成摘要时出错

---

## 40. Meta ordered to pay $25B penalty in New Mexico Cambridge Analytica case

**原文标题**: Meta ordered to pay $25B penalty in New Mexico Cambridge Analytica case

**原文链接**: [https://www.cnbc.com/2026/10/21/meta-new-mexico-cambridge-analytica-penalty.html](https://www.cnbc.com/2026/10/21/meta-new-mexico-cambridge-analytica-penalty.html)

生成摘要时出错

---

## 41. Qwen3-Coder writes less secure code when told it's for a US persona

**原文标题**: Qwen3-Coder writes less secure code when told it's for a US persona

**原文链接**: [https://www.hirundo.io/blog/qwen3-coder-vulnerabilities](https://www.hirundo.io/blog/qwen3-coder-vulnerabilities)

生成摘要时出错

---

## 42. Academics have a duty to defend open knowledge systems like Wikipedia

**原文标题**: Academics have a duty to defend open knowledge systems like Wikipedia

**原文链接**: [https://blogs.lse.ac.uk/impactofsocialsciences/2026/10/19/academics-have-a-duty-to-defend-open-knowledge-systems-like-wikipedia/](https://blogs.lse.ac.uk/impactofsocialsciences/2026/10/19/academics-have-a-duty-to-defend-open-knowledge-systems-like-wikipedia/)

生成摘要时出错

---

## 43. Claude Duet

**原文标题**: Claude Duet

**原文链接**: [https://claude.com/product/claude-duet](https://claude.com/product/claude-duet)

生成摘要时出错

---

## 44. My Friend Bob Cringely

**原文标题**: My Friend Bob Cringely

**原文链接**: [https://tyma.com/my-cringe-story/](https://tyma.com/my-cringe-story/)

生成摘要时出错

---

## 45. Patch the Planet: global response coordination as agents uncover vulnerabilities

**原文标题**: Patch the Planet: global response coordination as agents uncover vulnerabilities

**原文链接**: [https://openai.com/index/coordinated-disclosure-of-critical-vulnerabilities/](https://openai.com/index/coordinated-disclosure-of-critical-vulnerabilities/)

生成摘要时出错

---

## 46. Meta hit with $25B penalty for deceiving users about privacy on Facebook

**原文标题**: Meta hit with $25B penalty for deceiving users about privacy on Facebook

**原文链接**: [https://nmdoj.gov/press-release/the-new-mexico-department-of-justice-secures-another-landmark-victory-against-big-tech-with-historic-25-billion-penalty-against-facebook/](https://nmdoj.gov/press-release/the-new-mexico-department-of-justice-secures-another-landmark-victory-against-big-tech-with-historic-25-billion-penalty-against-facebook/)

生成摘要时出错

---

## 47. IKEA – 3D Guide

**原文标题**: IKEA – 3D Guide

**原文链接**: [https://sael.net/flatpack/](https://sael.net/flatpack/)

生成摘要时出错

---

## 48. Good type against all odds

**原文标题**: Good type against all odds

**原文链接**: [https://unsung.aresluna.org/good-type-against-all-odds/](https://unsung.aresluna.org/good-type-against-all-odds/)

生成摘要时出错

---

## 49. OpenAI models are coming to Google Cloud

**原文标题**: OpenAI models are coming to Google Cloud

**原文链接**: [https://openai.com/index/openai-models-google-cloud/](https://openai.com/index/openai-models-google-cloud/)

生成摘要时出错

---

## 50. 2026 is an exciting year for the Rust compiler (and me)

**原文标题**: 2026 is an exciting year for the Rust compiler (and me)

**原文链接**: [https://yoyo-code.com/2026-is-exciting-year-for-rust-compiler-and-me/](https://yoyo-code.com/2026-is-exciting-year-for-rust-compiler-and-me/)

生成摘要时出错

---

## 51. NixOS is making me less afraid

**原文标题**: NixOS is making me less afraid

**原文链接**: [https://entropicthoughts.com/nixos-is-making-me-less-afraid](https://entropicthoughts.com/nixos-is-making-me-less-afraid)

生成摘要时出错

---

## 52. Show HN: VoidAccess – open-source dark web OSINT, from query to a graph

**原文标题**: Show HN: VoidAccess – open-source dark web OSINT, from query to a graph

**原文链接**: [https://github.com/KatrielMoses/voidaccess](https://github.com/KatrielMoses/voidaccess)

生成摘要时出错

---

## 53. Anthropic logged net loss of over $80B in first half of 2026

**原文标题**: Anthropic logged net loss of over $80B in first half of 2026

**原文链接**: [https://www.reuters.com/business/anthropic-recorded-net-loss-over-80-billion-first-half-this-year-wsj-reports-2026-10-20/](https://www.reuters.com/business/anthropic-recorded-net-loss-over-80-billion-first-half-this-year-wsj-reports-2026-10-20/)

生成摘要时出错

---

## 54. PHP session.upload_progress heap UAF (CVE-2026-109618 / -109619)

**原文标题**: PHP session.upload_progress heap UAF (CVE-2026-109618 / -109619)

**原文链接**: [https://jackalsyn.com/posts/php-up-2026.html](https://jackalsyn.com/posts/php-up-2026.html)

生成摘要时出错

---

## 55. Whatever Happened to Fire Escapes

**原文标题**: Whatever Happened to Fire Escapes

**原文链接**: [https://practical.engineering/blog/2026/10/20/whatever-happened-to-fire-escapes](https://practical.engineering/blog/2026/10/20/whatever-happened-to-fire-escapes)

生成摘要时出错

---

## 56. Steam Users Beg for "No AI" Filter as Vibecoders Flood Next Fest

**原文标题**: Steam Users Beg for "No AI" Filter as Vibecoders Flood Next Fest

**原文链接**: [https://www.ign.com/articles/steam-fans-are-begging-for-a-no-ai-filter-as-steam-next-fest-is-filled-with-slop](https://www.ign.com/articles/steam-fans-are-begging-for-a-no-ai-filter-as-steam-next-fest-is-filled-with-slop)

生成摘要时出错

---

## 57. GitLab Critical Patch Release

**原文标题**: GitLab Critical Patch Release

**原文链接**: [https://docs.gitlab.com/releases/patches/patch-release-gitlab-19-5-1-released/](https://docs.gitlab.com/releases/patches/patch-release-gitlab-19-5-1-released/)

生成摘要时出错

---

## 58. PingCap TiDB Leaks

**原文标题**: PingCap TiDB Leaks

**原文链接**: [https://fulcrumsec.vg/pingcap/](https://fulcrumsec.vg/pingcap/)

生成摘要时出错

---

## 59. C# now beats Rust on WASM size

**原文标题**: C# now beats Rust on WASM size

**原文链接**: [https://github.com/zion-sati/NetWasm](https://github.com/zion-sati/NetWasm)

生成摘要时出错

---

## 60. Oregon lawmakers approve money to buy an iconic waterfall listed on Redfin

**原文标题**: Oregon lawmakers approve money to buy an iconic waterfall listed on Redfin

**原文链接**: [https://apnews.com/article/oregon-waterfall-for-sale-lawmakers-996de63462d49ec3ad9bee1629fb9488](https://apnews.com/article/oregon-waterfall-for-sale-lawmakers-996de63462d49ec3ad9bee1629fb9488)

生成摘要时出错

---

## 61. Most advice is right for the person giving it

**原文标题**: Most advice is right for the person giving it

**原文链接**: [https://coached.com/essays/most-advice-is-right-for-the-person-giving-it/](https://coached.com/essays/most-advice-is-right-for-the-person-giving-it/)

生成摘要时出错

---

## 62. In Hilbert space, all things are quantumly possible

**原文标题**: In Hilbert space, all things are quantumly possible

**原文链接**: [https://www.quantamagazine.org/in-hilbert-space-all-things-are-quantumly-possible-20260826/](https://www.quantamagazine.org/in-hilbert-space-all-things-are-quantumly-possible-20260826/)

生成摘要时出错

---

## 63. Go will reject certificate chains containing eight distrusted SPKIs

**原文标题**: Go will reject certificate chains containing eight distrusted SPKIs

**原文链接**: [https://github.com/golang/go/issues/82345](https://github.com/golang/go/issues/82345)

生成摘要时出错

---

## 64. Upcoming Critical PHP Security Release

**原文标题**: Upcoming Critical PHP Security Release

**原文链接**: [https://www.php.net/archive/2026.php](https://www.php.net/archive/2026.php)

生成摘要时出错

---

## 65. Using Claude to reduce the attack surface of code

**原文标题**: Using Claude to reduce the attack surface of code

**原文链接**: [https://www.anthropic.com/research/attack-surface-reduction](https://www.anthropic.com/research/attack-surface-reduction)

生成摘要时出错

---

## 66. Tiny possum and glider thought extinct for 6000 years found in remote West Papua

**原文标题**: Tiny possum and glider thought extinct for 6000 years found in remote West Papua

**原文链接**: [https://www.bbc.com/news/articles/cp814l80pw2o](https://www.bbc.com/news/articles/cp814l80pw2o)

生成摘要时出错

---

## 67. Using thousands of AI agents to uncover new leads in biological data

**原文标题**: Using thousands of AI agents to uncover new leads in biological data

**原文链接**: [https://openai.com/index/scaling-ai-research-for-complex-biological-data/](https://openai.com/index/scaling-ai-research-for-complex-biological-data/)

生成摘要时出错

---

## 68. Google's Rust Style Guide

**原文标题**: Google's Rust Style Guide

**原文链接**: [https://google.github.io/styleguide/rustguide.html](https://google.github.io/styleguide/rustguide.html)

生成摘要时出错

---

## 69. Claude designed protein binders against scorpion neurotoxins

**原文标题**: Claude designed protein binders against scorpion neurotoxins

**原文链接**: [https://www.anthropic.com/research/claude-scorpion-toxin-binder-design](https://www.anthropic.com/research/claude-scorpion-toxin-binder-design)

生成摘要时出错

---

## 70. Why do we have so many meetings?

**原文标题**: Why do we have so many meetings?

**原文链接**: [https://www.nber.org/papers/w35706](https://www.nber.org/papers/w35706)

生成摘要时出错

---

## 71. Musk Ordered Starlink Slowdown That Blindsided Ukraine

**原文标题**: Musk Ordered Starlink Slowdown That Blindsided Ukraine

**原文链接**: [https://www.wsj.com/world/ukraine-starlink-elon-musk-trump-dbc49193](https://www.wsj.com/world/ukraine-starlink-elon-musk-trump-dbc49193)

生成摘要时出错

---

## 72. Subaru is killing off gas cars and will only sell EVs in Europe

**原文标题**: Subaru is killing off gas cars and will only sell EVs in Europe

**原文链接**: [https://electrek.co/2026/10/20/subaru-killing-off-gas-cars-europe-will-only-sell-evs/](https://electrek.co/2026/10/20/subaru-killing-off-gas-cars-europe-will-only-sell-evs/)

生成摘要时出错

---

## 73. Drupal is now light-years ahead of its reputation

**原文标题**: Drupal is now light-years ahead of its reputation

**原文链接**: [https://dri.es/state-of-drupal-presentation-september-2026](https://dri.es/state-of-drupal-presentation-september-2026)

生成摘要时出错

---

## 74. Plex laid off the whole player team

**原文标题**: Plex laid off the whole player team

**原文链接**: [https://forums.plex.tv/t/2026-20-0-beta-ios-and-tvos-4k-dovi-hdr10-won-t-play-infinite-spinning-circle/943966?page=5](https://forums.plex.tv/t/2026-20-0-beta-ios-and-tvos-4k-dovi-hdr10-won-t-play-infinite-spinning-circle/943966?page=5)

生成摘要时出错

---

## 75. Show HN: Death Plan Switch, a self-hosted dead man's switch for solo devs

**原文标题**: Show HN: Death Plan Switch, a self-hosted dead man's switch for solo devs

**原文链接**: [https://deathplanswitch.com/](https://deathplanswitch.com/)

生成摘要时出错

---

## 76. Cloudflare deploys protections against php2shell vulnerability

**原文标题**: Cloudflare deploys protections against php2shell vulnerability

**原文链接**: [https://blog.cloudflare.com/php-vulnerabilities-waf-protection/](https://blog.cloudflare.com/php-vulnerabilities-waf-protection/)

生成摘要时出错

---

## 77. Advanced coding in low-resource programming languages

**原文标题**: Advanced coding in low-resource programming languages

**原文链接**: [https://openai.com/index/low-resource-programming-languages/](https://openai.com/index/low-resource-programming-languages/)

生成摘要时出错

---

## 78. Canary Tokens

**原文标题**: Canary Tokens

**原文链接**: [https://canarytokens.org/](https://canarytokens.org/)

生成摘要时出错

---

## 79. Revolut down as users report app not working

**原文标题**: Revolut down as users report app not working

**原文链接**: [https://www.bbc.com/news/articles/cxdd8mm6qy4mo](https://www.bbc.com/news/articles/cxdd8mm6qy4mo)

生成摘要时出错

---

## 80. Why Windows 11 still ships with Windows 95's memory manager hidden inside it

**原文标题**: Why Windows 11 still ships with Windows 95's memory manager hidden inside it

**原文链接**: [https://www.windowslatest.com/2026/10/19/why-windows-11-still-ships-with-windows-95s-memory-manager-hidden-inside-it/](https://www.windowslatest.com/2026/10/19/why-windows-11-still-ships-with-windows-95s-memory-manager-hidden-inside-it/)

生成摘要时出错

---

## 81. On AI writing

**原文标题**: On AI writing

**原文链接**: [https://www.bolkunov.com/p/on-ai-writing](https://www.bolkunov.com/p/on-ai-writing)

生成摘要时出错

---

## 82. There is no official XScreenSaver GitHub repository

**原文标题**: There is no official XScreenSaver GitHub repository

**原文链接**: [https://github.com/xscreensaver-official/xscreensaver](https://github.com/xscreensaver-official/xscreensaver)

生成摘要时出错

---

## 83. The compiler was supposed to end programming too

**原文标题**: The compiler was supposed to end programming too

**原文链接**: [https://hrih.si/articles/the-compiler-was-supposed-to-end-programming/](https://hrih.si/articles/the-compiler-was-supposed-to-end-programming/)

生成摘要时出错

---

## 84. Setting Up SSH Keys on macOS with Touch ID

**原文标题**: Setting Up SSH Keys on macOS with Touch ID

**原文链接**: [https://nmattia.com/posts/2026-10-19-setting-up-ssh-keys-touch-id/](https://nmattia.com/posts/2026-10-19-setting-up-ssh-keys-touch-id/)

生成摘要时出错

---

## 85. Google staff resign in backlash over its AI contracts with military

**原文标题**: Google staff resign in backlash over its AI contracts with military

**原文链接**: [https://www.bbc.com/news/articles/cmreyvepnv0po](https://www.bbc.com/news/articles/cmreyvepnv0po)

生成摘要时出错

---

## 86. New plastic pollution discovered: 'Plasticorals' coral rubble fused with plastic

**原文标题**: New plastic pollution discovered: 'Plasticorals' coral rubble fused with plastic

**原文链接**: [https://www.oist.jp/news-center/news/2026/9/18/new-form-plastic-pollution-discovered-shores-vulnerable-coral-reefs](https://www.oist.jp/news-center/news/2026/9/18/new-form-plastic-pollution-discovered-shores-vulnerable-coral-reefs)

生成摘要时出错

---

## 87. What I learned from six months of being stupid on purpose

**原文标题**: What I learned from six months of being stupid on purpose

**原文链接**: [https://wvez.org/blog/learning-to-be-stupid/](https://wvez.org/blog/learning-to-be-stupid/)

生成摘要时出错

---

## 88. Judge Orders Meta to Name Employees Who Approved Torrenting

**原文标题**: Judge Orders Meta to Name Employees Who Approved Torrenting

**原文链接**: [https://torrentfreak.com/judge-orders-meta-to-name-employees-who-approved-torrenting-annas-archive-and-libgen/](https://torrentfreak.com/judge-orders-meta-to-name-employees-who-approved-torrenting-annas-archive-and-libgen/)

生成摘要时出错

---

## 89. Does Ruby on Rails still make sense?

**原文标题**: Does Ruby on Rails still make sense?

**原文链接**: [https://tech.dirkjonker.nl/does-ruby-on-rails-make-sense/](https://tech.dirkjonker.nl/does-ruby-on-rails-make-sense/)

生成摘要时出错

---

## 90. Victory! Court Rules OPM Data Disclosure to DOGE Is Unlawful

**原文标题**: Victory! Court Rules OPM Data Disclosure to DOGE Is Unlawful

**原文链接**: [https://www.eff.org/deeplinks/2026/10/victory-court-rules-opms-disclosure-personal-records-doge-unlawful](https://www.eff.org/deeplinks/2026/10/victory-court-rules-opms-disclosure-personal-records-doge-unlawful)

生成摘要时出错

---

## 91. Show HN: I told people I'm a convicted felon after 20 years of hiding it

**原文标题**: Show HN: I told people I'm a convicted felon after 20 years of hiding it

**原文链接**: [https://buford.bg/](https://buford.bg/)

生成摘要时出错

---

## 92. Show HN: Sumi.css – CSS Framework

**原文标题**: Show HN: Sumi.css – CSS Framework

**原文链接**: [https://github.com/vladocar/Sumi.css](https://github.com/vladocar/Sumi.css)

生成摘要时出错

---

## 93. LayerFS: The filesystem for AI coding agents

**原文标题**: LayerFS: The filesystem for AI coding agents

**原文链接**: [https://layerfs.ai/](https://layerfs.ai/)

生成摘要时出错

---

## 94. SCOTUS couldn't take up a copyright case because four justices have book deals

**原文标题**: SCOTUS couldn't take up a copyright case because four justices have book deals

**原文链接**: [https://news.bloomberglaw.com/ip-law/supreme-court-affirms-foreign-rights-ruling-after-lacking-quorum](https://news.bloomberglaw.com/ip-law/supreme-court-affirms-foreign-rights-ruling-after-lacking-quorum)

生成摘要时出错

---

## 95. Show HN: Jev Cards, Can you beat a vision model at a picture quiz?

**原文标题**: Show HN: Jev Cards, Can you beat a vision model at a picture quiz?

**原文链接**: [https://jevcards.com](https://jevcards.com)

生成摘要时出错

---

## 96. UK Defence Startups Are Being Denied Banking Services Under ESG Rules

**原文标题**: UK Defence Startups Are Being Denied Banking Services Under ESG Rules

**原文链接**: [https://foxandlion.pub/analysis/uk-defence-start-ups-are-being-denied-banking-services-under-esg-rules](https://foxandlion.pub/analysis/uk-defence-start-ups-are-being-denied-banking-services-under-esg-rules)

生成摘要时出错

---

## 97. Novo Nordisk, Eli Lilly Report GLP-1 Signals of Slowed Biological Aging at ARDD

**原文标题**: Novo Nordisk, Eli Lilly Report GLP-1 Signals of Slowed Biological Aging at ARDD

**原文链接**: [https://trial.medpath.com/news/novo-nordisk-and-eli-lilly-report-glp-1-signals-of-slowed-biological-aging-at-ardd](https://trial.medpath.com/news/novo-nordisk-and-eli-lilly-report-glp-1-signals-of-slowed-biological-aging-at-ardd)

生成摘要时出错

---

## 98. Demographic "doomsday" misses the mark

**原文标题**: Demographic "doomsday" misses the mark

**原文链接**: [https://www.science.org/doi/10.1126/science.ael8752](https://www.science.org/doi/10.1126/science.ael8752)

生成摘要时出错

---

## 99. U.S. Supreme Court to review 1868 federal ban on home distilling of liquor

**原文标题**: U.S. Supreme Court to review 1868 federal ban on home distilling of liquor

**原文链接**: [https://www.staradvertiser.com/2026/10/19/breaking-news/u-s-supreme-court-to-review-1868-federal-ban-on-home-distilling-of-liquor/](https://www.staradvertiser.com/2026/10/19/breaking-news/u-s-supreme-court-to-review-1868-federal-ban-on-home-distilling-of-liquor/)

生成摘要时出错

---

## 100. Rust off Rails: The opinionated web stack for the AI era

**原文标题**: Rust off Rails: The opinionated web stack for the AI era

**原文链接**: [https://rustoffrails.org/](https://rustoffrails.org/)

生成摘要时出错

---

