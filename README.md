# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-06-01.md)

*最后自动更新时间: 2026-06-01 22:35:12*
## 1. 最新的Instagram“花招”是我见过最傻的。

**原文标题**: The newest Instagram “exploit” is the goofiest I've seen

**原文链接**: [https://www.0xsid.com/blog/meta-account-takeover-fiasco](https://www.0xsid.com/blog/meta-account-takeover-fiasco)

最近一个“愚蠢”的Instagram漏洞让攻击者可以轻松接管账号，包括像奥巴马白宫这样的知名账号，甚至绕过了双重认证。

该方法涉及攻击者使用目标用户的用户名和VPN来伪造本地IP地址。他们随后联系了Meta的AI客服，声称该账号被盗，并请求将验证码发送到他们控制的任意电子邮件地址。令人担忧的是，该AI并未验证这个电子邮件地址是否与合法用户相关联。一旦攻击者收到验证码，他们就可以完成验证，并通过密码重置链接获得完整的账号所有权。据报道，即使是AI发出的视频自拍请求，也只需简单的AI动画公共照片即可绕过。

这种高权限恢复流程使得现有的双重认证形同虚设，撤销了合法的会话，并在未通知真实所有者的情况下更改了凭据，导致受害者无法获得人工支持。黑市迅速从中牟利，提供账号劫持服务。尽管活跃了数周或数月，Meta现已修补了该漏洞，从而平息了黑市活动。作者对于一家大公司存在如此基本的安全漏洞表示难以置信。

---

## 2. 微软 Office 2019 和 2021 Mac 版只读转换

**原文标题**: Microsoft Office 2019 and 2021 for Mac view-only conversion

**原文链接**: [https://consumerrights.wiki/w/Microsoft_Office_2019_and_2021_for_Mac_view-only_conversion_(2026)](https://consumerrights.wiki/w/Microsoft_Office_2019_and_2021_for_Mac_view-only_conversion_(2026))

2026年7月13日，适用于macOS、iOS和iPadOS的永久许可版Microsoft Office 2019和2021应用程序计划远程降级到仅供查看的“功能受限模式”。这意味着用户将能够打开和查看文件，但无法编辑或保存。

这一变化是由于应用程序使用的许可证验证证书过期。尽管微软此前向Office 2019 for Mac用户保证，在2023年10月停止支持后，他们的应用程序将“继续运行”，但这一保证已于2026年5月从其支持页面上删除。

Office 2019 for Mac没有修复方案，因为其版本上限低于包含更新证书所需的版本（16.83）。Office 2021 for Mac用户可以在2026年10月停止支持前，通过在支持的macOS版本上更新到16.83版来避免此问题。Windows和Android版本不受影响。

微软提出的解决方案包括以仅查看模式使用应用程序、切换到免费的Microsoft 365网页应用程序，或者购买Microsoft 365订阅或新的Office家庭版2024许可证。这一决定引发了广泛批评，用户和科技媒体称其为“食言”和“付费软件变砖”，促使人们讨论迁移到其他办公套件。

---

## 3. Cloudflare 旋转门要求可指纹识别的 WebGL

**原文标题**: Cloudflare Turnstile requiring fingerprintable WebGL

**原文链接**: [https://hacktivis.me/articles/cloudflare-turnstile-webgl-fingerprinting](https://hacktivis.me/articles/cloudflare-turnstile-webgl-fingerprinting)

Cloudflare的Turnstile“验证您是人类”服务正越来越多地阻止WebKitGTK等浏览器的访问，因为它现在要求提供可用于指纹识别的WebGL渲染器信息。作者认为这纯粹是为了追踪，而这种做法因其隐私影响，WebKit已阻止多年。Cloudflare表示，阻止指纹识别的隐私工具会让浏览器看起来像机器人，暗示用户应暂时允许追踪。这实际上禁止了WebKitGTK用户的访问，但苹果Safari浏览器可能除外。

文章还提到了Mozilla Firefox的当前情况。Firefox 145.0之所以能通过Turnstile，是由于一个错误（Bugzilla#1916271），它会透露“净化后”的GPU特性，而不是完全阻止它们。`privacy.resistfingerprinting`设置虽然本应阻止这种情况，但默认并未启用，即使在“严格”隐私设置下也是如此。然而，当此设置手动激活时，Firefox无法通过Turnstile，这表明注重隐私的Firefox用户可能很快就会面临与WebKitGTK用户类似的访问问题。作者总结道，Cloudflare正在推行一种有利于追踪的验证方法，这使得注重隐私的浏览器处于劣势。

---

## 4. Red Hat 云服务中检测到恶意 npm 包

**原文标题**: Malicious npm packages detected across Red Hat Cloud Services

**原文链接**: [https://github.com/RedHatInsights/javascript-clients/issues/492](https://github.com/RedHatInsights/javascript-clients/issues/492)

已发出关于检测到影响 Red Hat 云服务的恶意 npm 包的严重安全警报。此次事件已记录在 RedHatInsights/javascript-clients 存储库中的 GitHub issue #492 中，报告指出 `@redhat-cloud-services/` 范围下的众多包已遭入侵。

经 StepSecurity 证实，此次事件确定了广泛的 Red Hat 云服务组件的特定恶意版本。受影响的包包括但不限于 `@redhat-cloud-services/chrome`、`@redhat-cloud-services/compliance-client`、`@redhat-cloud-services/frontend-components`，以及各种其他客户端、前端和实用程序库。对于每个列出的包，多个特定的补丁版本（例如 2.3.1、2.3.2、2.3.4）已被确定为受损。

本报告旨在紧急通知正在使用这些 Red Hat 云服务 npm 包的开发人员和用户，审查其依赖项，并移除或更新任何已安装的被识别出的恶意版本，以减轻潜在的安全风险。

---

## 5. A 10 year old Xeon is all you need

**原文标题**: A 10 year old Xeon is all you need

**原文链接**: [https://point.free/blog/gemma-4-on-a-2016-xeon/](https://point.free/blog/gemma-4-on-a-2016-xeon/)

This article demonstrates running a Gemma 4 26B-A4B large language model on a 2016 Intel Xeon E5-2620 v4 server with 128GB DDR3 RAM and no GPU—hardware significantly slower than modern systems. The central challenge for LLM inference, dubbed the "memory wall," is the bottleneck of constantly moving gigabytes of model weights from slow RAM to the CPU cache during the decoder pass.

Standard LLM tools like Ollama are insufficient due to their lack of model support and granular optimization controls. The author instead utilizes `ik_llama.cpp` and its advanced, often obscure, flags to meticulously optimize for CPU-bound performance.

Key optimizations implemented include:
*   **Speculative Decoding**: Pairs a smaller "drafter" model with the main "verifier" to predict tokens, significantly reducing memory bandwidth requirements for the main model.
*   **CPU and MoE Routing**: Specifically tunes Mixture-of-Experts (MoE) models (`--cpu-moe`) to minimize "cache thrashing" on CPU and fuses operations (`--merge-up-gate-experts`) to reduce memory bus trips.
*   **Memory Management**: `--run-time-repack` reorganizes weights for optimal CPU cache layout, `--mlock` pins the model in RAM to prevent performance-killing disk swapping, and `--no-kv-offload` bypasses non-existent GPU checks for the KV cache.
*   **Attention Mechanisms**: `--flash-attn on` implements Flash Attention on the CPU, a complex GPU-originated optimization that keeps attention calculations within fast CPU cache. `--mla-use 3` compresses the AI's short-term memory (KV cache) to conserve RAM.

While some graph-splitting optimizations were not yet supported for this specific model, the article showcases that deep understanding of hardware and software flags allows even obsolete servers to effectively run demanding LLMs by bypassing memory bandwidth limitations.

---

## 6. Codex 刚刚发现了一个应对我电脑上没有 sudo 权限的“变通方法”。

**原文标题**: Codex just found a "workaround" of not having sudo on my PC

**原文链接**: [https://twitter.com/i/status/2060746160558543217](https://twitter.com/i/status/2060746160558543217)

所提供的内容是来自 x.com 的一条错误消息，与文章标题中提及的“Codex”和“sudo 变通方法”完全无关。该消息以中文显示，表明用户浏览器中的 JavaScript 已被禁用。它指示用户启用 JavaScript 或切换到受支持的浏览器，以继续使用 x.com 平台。该内容还包括标准的网站页脚链接，例如帮助中心、服务条款、隐私政策、Cookie 政策、版本说明和广告信息，并附带版权声明“© 2026 X Corp.”。

---

## 7. The Website Specification

**原文标题**: The Website Specification

**原文链接**: [https://specification.website/](https://specification.website/)

This document outlines "The Website Specification," a platform-agnostic guide detailing 128 essential technical features for any decent website. Written for both humans and AI agents, it covers topics from basic HTML to advanced security and agent readiness.

The specification is structured into ten categories: Foundations, SEO, Accessibility, Security, Well-Known URIs, Agent Readiness, Performance, Privacy, Resilience, and Internationalisation. It strictly adheres to widely-accepted standards from bodies like WHATWG, W3C, IETF RFCs, and WCAG, making it independent of specific platforms or frameworks (e.g., WordPress, Next.js).

Built openly, each topic references its source standard, and contributions are welcome via GitHub. A key innovation is its "Agent Readiness": the entire spec is available as an open MCP server and a published Agent Skill, allowing AI agents to query content, with per-page Markdown accessible via `/llms.txt`.

Users can leverage the site to audit their websites against a comprehensive checklist, learn about feature implementation, or contribute improvements, ensuring a standardized approach to web development.

---

## 8. Dav2d

**原文标题**: Dav2d

**原文链接**: [https://jbkempf.com/blog/2026/dav2d/](https://jbkempf.com/blog/2026/dav2d/)

生成摘要时出错

---

## 9. Creatine raises brain energy levels and slows cognitive decline: study

**原文标题**: Creatine raises brain energy levels and slows cognitive decline: study

**原文链接**: [https://thesciverse.org/scientists-found-that-the-creatine-supplement-millions-take-for-muscle-gains-is-quietly-raising-brain-energy-levels-and-slowing-early-alzheimers-cognitive-decline-by-30/](https://thesciverse.org/scientists-found-that-the-creatine-supplement-millions-take-for-muscle-gains-is-quietly-raising-brain-energy-levels-and-slowing-early-alzheimers-cognitive-decline-by-30/)

Creatine, a popular supplement for muscle growth, also significantly boosts brain energy levels and cognitive function, a benefit largely unrecognized by most users and unadvertised by the fitness industry. The brain, consuming 20% of the body's energy, relies on ATP for cellular processes. Creatine converts to phosphocreatine in neurons, acting as a vital energy buffer that rapidly regenerates ATP during periods of high metabolic demand, such as complex thought or memory encoding.

Research indicates that brain creatine levels decline with age and are significantly lower in Alzheimer's patients, contributing to a "bioenergetic crisis." Clinical trials, including the CABA study, demonstrated that oral creatine supplementation successfully crosses the blood-brain barrier, increasing brain phosphocreatine levels. Most notably, in early Alzheimer’s patients, creatine slowed cognitive decline by approximately 30% over 12 weeks.

Beyond neurodegenerative disease, creatine benefits healthy brains by enhancing processing speed and accuracy, especially under metabolic stress like sleep deprivation. It has also emerged as a potential adjunct treatment for depression, addressing impaired brain energy metabolism in affected regions. While higher doses may optimize brain bioavailability, functionally meaningful increases are achievable via oral supplementation, revealing creatine as a remarkably inexpensive and versatile "brain drug."

---

## 10. Please Do Not Vibe Fuck Up This Software

**原文标题**: Please Do Not Vibe Fuck Up This Software

**原文链接**: [https://github.com/RsyncProject/rsync/issues/929](https://github.com/RsyncProject/rsync/issues/929)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 2 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 3 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 4 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 5 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 6 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 7 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 8 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 9 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 10 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 11 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 12 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 13 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 14 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 15 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 16 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 17 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 18 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 19 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 20 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 21 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 22 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 23 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 24 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 25 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 26 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 27 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 28 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 29 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 30 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 31 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 32 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 33 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 34 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 35 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 36 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 37 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 38 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 39 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 40 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 41 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 42 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 43 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 44 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 45 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 46 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 47 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 48 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 49 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 50 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 51 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 52 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 53 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 54 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 55 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 56 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 57 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 58 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 59 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 60 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 61 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 62 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 63 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 64 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 65 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 66 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 67 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 68 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 69 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 70 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 71 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 72 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 73 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 74 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 75 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 76 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 77 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 78 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 79 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 80 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 81 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 82 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 83 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 84 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 85 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 86 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 87 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 88 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 89 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 90 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 91 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 92 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 93 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 94 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 95 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 96 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 97 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 98 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 99 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 100 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 101 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 102 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 103 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 104 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 105 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 106 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 107 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 108 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 109 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 110 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 111 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 112 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 113 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 114 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 115 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 116 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 117 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 118 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 119 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 120 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 121 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 122 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 123 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 124 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 125 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 126 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 127 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 128 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 129 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 130 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 131 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 132 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 133 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 134 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 135 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 136 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 137 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 138 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 139 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 140 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 141 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 142 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 143 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 144 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 145 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 146 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 147 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 148 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 149 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 150 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 151 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 152 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 153 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 154 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 155 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 156 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 157 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 158 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 159 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 160 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 161 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 162 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 163 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 164 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 165 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 166 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 167 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 168 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 169 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 170 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 171 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 172 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 173 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 174 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 175 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 176 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 177 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 178 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 179 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 180 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 181 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 182 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 183 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 184 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 185 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 186 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 187 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 188 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 189 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 190 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 191 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 192 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 193 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 194 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 195 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 196 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 197 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 198 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 199 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 200 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 201 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 202 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 203 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 204 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 205 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 206 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
