# Hacker News 热门文章摘要 (2026-01-24)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 苹果钟爱的Bug

**原文标题**: Bugs Apple loves

**原文链接**: [https://www.bugsappleloves.com](https://www.bugsappleloves.com)

这篇题为“苹果钟爱的漏洞”的文章篇幅极短，仅包含“正在加载苹果漏洞”这一短语。这种极简的内容，加上具有讽刺意味的标题，暗示了对苹果产品中软件缺陷反复出现这一现象的讽刺评论。这篇文章充当了比喻性的公告或占位符，承认了苹果生态系统中漏洞的存在，但没有提供关于这些漏洞的性质、影响或普遍性的具体细节。它幽默地暗示，这些漏洞是苹果用户体验中一个持续存在的特点，而非一个受喜爱之处。

---

## 2. 微软向联邦调查局提供了BitLocker加密密钥，以解锁嫌疑人的笔记本电脑。

**原文标题**: Microsoft gave FBI set of BitLocker encryption keys to unlock suspects' laptops

**原文链接**: [https://techcrunch.com/2026/01/23/microsoft-gave-fbi-a-set-of-bitlocker-encryption-keys-to-unlock-suspects-laptops-reports/](https://techcrunch.com/2026/01/23/microsoft-gave-fbi-a-set-of-bitlocker-encryption-keys-to-unlock-suspects-laptops-reports/)

微软向美国联邦调查局（FBI）提供了BitLocker恢复密钥，以解锁三名嫌疑人的笔记本电脑，这是关岛一项联邦欺诈调查的一部分。BitLocker是Windows的默认全盘加密功能，它默认会自动将这些恢复密钥上传到微软的云端。这使得微软，以及随后凭搜查令获得授权的执法部门，能够访问并使用这些密钥来解密硬盘。

《福布斯》报道了这起事件，指出微软每年平均收到20份此类请求。此案涉及一项“疫情失业援助计划”欺诈方案的嫌疑人，微软收到了搜查令，要求访问其加密硬盘。

约翰霍普金斯大学教授兼密码学专家马修·格林（Matthew Green）批评了微软的做法，强调了重大的隐私和安全风险。他指出，虽然此举方便了执法部门的访问，但如果微软的云基础设施被攻破（此类事件以前也曾发生过），这些关键密钥也会面临被恶意黑客窃取的潜在风险。格林指出，“微软无力保护关键客户密钥的做法，正使其在行业中显得格格不入”，并强调这些担忧早已是众所周知。

---

## 3. 欧洲替代方案

**原文标题**: European Alternatives

**原文链接**: [https://european-alternatives.eu](https://european-alternatives.eu)

生成摘要时出错

---

## 4. 我因为生成了一个Claude.md文件就被Claude封禁了？

**原文标题**: I was banned from Claude for scaffolding a Claude.md file?

**原文链接**: [https://hugodaniel.com/posts/claude-code-banned-me/](https://hugodaniel.com/posts/claude-code-banned-me/)

许戈·丹尼尔（Hugo Daniel）详细讲述了他因“滥用服务”违规行为而被Claude永久封禁的经历，这源于他试图利用该AI工具来搭建一个`claude.md`文件。他的本意是为“Claude插件”定义一个规范，类似于OpenAI的插件清单，他随后将该规范上传到了GitHub。

由于Anthropic没有提供任何具体解释，丹尼尔猜测了封禁的原因。他考虑的可能性包括：在文件名和内容中使用“Claude”可能导致版权或商标侵权，或是AI审核系统产生了误判。他怀疑系统是否错误地将其活动标记为自我复制、逆向工程或利用的尝试，而非在Claude生态系统内进行构建的合法努力。

丹尼尔对此次封禁的不透明性、他的对话历史永久丢失以及完全没有关于具体违规行为的沟通表示深切担忧。他主张AI提供商应提高其服务条款和账户终止原因的透明度，强调需要更明确的指导方针和更好的用户沟通来建立信任。

---

## 5. Why does SSH send 100 packets per keystroke?

**原文标题**: Why does SSH send 100 packets per keystroke?

**原文链接**: [https://eieio.games/blog/ssh-sends-100-packets-per-keystroke/](https://eieio.games/blog/ssh-sends-100-packets-per-keystroke/)

作者在通过 SSH 开发一款高性能游戏时，当一个测试工具无意中停止发送游戏数据后，观察到 CPU 和带宽意外减少了 50%。这表明即使没有活跃的游戏玩法，也存在显著的开销。

使用 `tcpdump`，他们发现 SSH 会话中的一次按键操作会生成大约 270 个数据包，其中包括 179 个神秘的 36 字节消息和 90 个 TCP ACK，这些数据包大约每隔 20 毫秒到达。这种模式在标准的 SSH 会话中普遍存在，而不仅仅是他们的游戏。

通过 `ssh -vvv` 进一步调查，揭示了根本原因：SSH 的按键时序混淆功能，该功能于 2023 年添加。此功能大约每 20 毫秒发送一次“干扰”数据包（SSH2_MSG_PING），以防止攻击者通过分析打字速度来推断输入的字符。尽管这对普通 SSH 使用中的隐私保护有益，但却给对延迟敏感的游戏带来了过多的开销。

客户端修复（`ObscureKeystrokeTiming=no`）虽然有效，但对用户来说不切实际。最终解决方案涉及一个服务器端补丁：作者发现干扰数据包仅在服务器宣称支持 `[email protected]` 扩展时才发送。通过分叉 Go 的 SSH 库并撤销添加此宣称的提交，他们显著降低了 CPU 使用率（从 29.9% 降至 11.6%）、系统调用、加密操作和带宽（降低超过 50%）。

作者还指出，像 Claude Code 这样的 LLM 在调试 `tcpdump` 输出和代码更改方面提供了显著帮助，尽管在关键洞察方面仍需要人类直觉，并且需要纠正一些 LLM 自信但错误的回复。

---

## 6. Proton垃圾邮件和AI同意问题

**原文标题**: Proton spam and the AI consent problem

**原文链接**: [https://dbushell.com/2026/01/22/proton-spam/](https://dbushell.com/2026/01/22/proton-spam/)

作者，一位Proton的付费用户，详细讲述了他们收到一封推广Proton的AI产品“Lumo”的邮件，尽管他们已明确选择退出“Lumo产品更新”。他们认为这封未经请求的邮件是垃圾邮件，侵犯了同意权，尤其是在GDPR（通用数据保护条例）框架下。

最初，Proton支持团队提供了关于如何退订的无用建议，随后又试图将该邮件重新归类为“Proton for Business新闻通讯”，以证明其发送的合理性，但作者对此斥之为“胡说八道”。作者将这一事件归结为一个更广泛的“AI同意问题”，认为该行业普遍无视用户选择、知识产权和隐私，并举例说明，尽管他们已禁用通知，但仍收到GitHub/微软发送的、与AI相关的垃圾邮件。

在作者公开详细描述了他们的经历后，Proton升级了问题处理级别。专业支持团队最初将问题归咎于通知的“类别重叠”。最终，Proton的客户支持主管和首席技术官公开承认存在一个系统漏洞，为沟通失误致歉，并向作者保证他们认真对待沟通同意。虽然作者目前接受了这一解释，但他们强调了一个令人不安的趋势：包括Proton这样倡导隐私价值观的科技公司，在推进AI整合的过程中，正在凌驾于用户偏好之上。

---

## 7. AI使用政策

**原文标题**: AI Usage Policy

**原文链接**: [https://github.com/ghostty-org/ghostty/blob/main/AI_POLICY.md](https://github.com/ghostty-org/ghostty/blob/main/AI_POLICY.md)

The provided content does not contain an "AI Usage Policy." Instead, it appears to be metadata related to a GitHub repository:

*   **Repository:** `ghostty-org/ghostty`
*   **Status:** Public
*   **Notifications:** Requires sign-in to change settings
*   **Metrics:** 1.5k forks, 42k stars

As there is no policy text, a summary of an AI Usage Policy cannot be generated from the given information.

---

## 8. 我做了一盏对无线电波有反应的灯 [视频]

**原文标题**: I built a light that reacts to radio waves [video]

**原文链接**: [https://www.youtube.com/watch?v=moBCOEiqiPs](https://www.youtube.com/watch?v=moBCOEiqiPs)

所提供的内容描述了一个项目，其中创建者制作了一个旨在对无线电波作出反应的灯，并以视频形式呈现。然而，随附的文本仅包含标准的YouTube页脚和样板信息。这包括指向YouTube新闻、版权信息、联系方式、创作者和开发者资源、广告信息、服务条款、隐私政策以及安全指南的链接。它还提到了YouTube的运作方式、测试新功能的选项、NFL周日门票©，以及2026年Google LLC的版权信息。所提供的文本本身没有提供任何关于那个对无线电波作出反应的灯的项目的进一步细节。

---

## 9. Proof of Corn

**原文标题**: Proof of Corn

**原文链接**: [https://proofofcorn.com/](https://proofofcorn.com/)

生成摘要时出错

---

## 10. Unrolling the Codex agent loop

**原文标题**: Unrolling the Codex agent loop

**原文链接**: [https://openai.com/index/unrolling-the-codex-agent-loop/](https://openai.com/index/unrolling-the-codex-agent-loop/)

生成摘要时出错

---

## 11. Gas Town's agent patterns, design bottlenecks, and vibecoding at scale

**原文标题**: Gas Town's agent patterns, design bottlenecks, and vibecoding at scale

**原文链接**: [https://maggieappleton.com/gastown](https://maggieappleton.com/gastown)

生成摘要时出错

---

## 12. Capital One to acquire Brex for $5.15B

**原文标题**: Capital One to acquire Brex for $5.15B

**原文链接**: [https://www.reuters.com/legal/transactional/capital-one-buy-fintech-firm-brex-515-billion-deal-2026-01-22/](https://www.reuters.com/legal/transactional/capital-one-buy-fintech-firm-brex-515-billion-deal-2026-01-22/)

生成摘要时出错

---

## 13. Booting from a vinyl record (2020)

**原文标题**: Booting from a vinyl record (2020)

**原文链接**: [https://boginjr.com/it/sw/dev/vinyl-boot/](https://boginjr.com/it/sw/dev/vinyl-boot/)

生成摘要时出错

---

## 14. Doing gigabit Ethernet over my British phone wires

**原文标题**: Doing gigabit Ethernet over my British phone wires

**原文链接**: [https://thehftguy.com/2026/01/22/doing-gigabit-ethernet-over-my-british-phone-wires/](https://thehftguy.com/2026/01/22/doing-gigabit-ethernet-over-my-british-phone-wires/)

生成摘要时出错

---

## 15. Comma openpilot – Open source driver-assistance

**原文标题**: Comma openpilot – Open source driver-assistance

**原文链接**: [https://comma.ai](https://comma.ai)

生成摘要时出错

---

## 16. Tesla kills Autopilot, locks lane-keeping behind $99/month fee

**原文标题**: Tesla kills Autopilot, locks lane-keeping behind $99/month fee

**原文链接**: [https://arstechnica.com/cars/2026/01/tesla-wants-recurring-revenue-discontinues-autopilot-in-favor-of-fsd/](https://arstechnica.com/cars/2026/01/tesla-wants-recurring-revenue-discontinues-autopilot-in-favor-of-fsd/)

生成摘要时出错

---

## 17. Scaling PostgreSQL to power 800M ChatGPT users

**原文标题**: Scaling PostgreSQL to power 800M ChatGPT users

**原文链接**: [https://openai.com/index/scaling-postgresql/](https://openai.com/index/scaling-postgresql/)

生成摘要时出错

---

## 18. New YC homepage

**原文标题**: New YC homepage

**原文链接**: [https://www.ycombinator.com/](https://www.ycombinator.com/)

生成摘要时出错

---

## 19. How I estimate work

**原文标题**: How I estimate work

**原文链接**: [https://www.seangoedecke.com/how-i-estimate-work/](https://www.seangoedecke.com/how-i-estimate-work/)

生成摘要时出错

---

## 20. MS confirms it will give the FBI your Windows PC data encryption key if asked

**原文标题**: MS confirms it will give the FBI your Windows PC data encryption key if asked

**原文链接**: [https://www.windowscentral.com/microsoft/windows-11/microsoft-bitlocker-encryption-keys-give-fbi-legal-order-privacy-nightmare](https://www.windowscentral.com/microsoft/windows-11/microsoft-bitlocker-encryption-keys-give-fbi-legal-order-privacy-nightmare)

生成摘要时出错

---

## 21. Radicle: The Sovereign Forge

**原文标题**: Radicle: The Sovereign Forge

**原文链接**: [https://radicle.xyz](https://radicle.xyz)

生成摘要时出错

---

## 22. Show HN: Whosthere: A LAN discovery tool with a modern TUI, written in Go

**原文标题**: Show HN: Whosthere: A LAN discovery tool with a modern TUI, written in Go

**原文链接**: [https://github.com/ramonvermeulen/whosthere](https://github.com/ramonvermeulen/whosthere)

生成摘要时出错

---

## 23. What has Docker become?

**原文标题**: What has Docker become?

**原文链接**: [https://tuananh.net/2026/01/20/what-has-docker-become/](https://tuananh.net/2026/01/20/what-has-docker-become/)

生成摘要时出错

---

## 24. KORG phase8 – Acoustic Synthesizer

**原文标题**: KORG phase8 – Acoustic Synthesizer

**原文链接**: [https://www.korg.com/us/products/dj/phase8/](https://www.korg.com/us/products/dj/phase8/)

生成摘要时出错

---

## 25. Why medieval city-builder video games are historically inaccurate (2020)

**原文标题**: Why medieval city-builder video games are historically inaccurate (2020)

**原文链接**: [https://www.leidenmedievalistsblog.nl/articles/why-medieval-city-builder-video-games-are-historically-inaccurate](https://www.leidenmedievalistsblog.nl/articles/why-medieval-city-builder-video-games-are-historically-inaccurate)

生成摘要时出错

---

## 26. Microsoft mishandling example.com

**原文标题**: Microsoft mishandling example.com

**原文链接**: [https://tinyapps.org/blog/microsoft-mishandling-example-com.html](https://tinyapps.org/blog/microsoft-mishandling-example-com.html)

生成摘要时出错

---

## 27. Zotero 8

**原文标题**: Zotero 8

**原文链接**: [https://www.zotero.org/blog/zotero-8/](https://www.zotero.org/blog/zotero-8/)

生成摘要时出错

---

## 28. The tech monoculture is finally breaking

**原文标题**: The tech monoculture is finally breaking

**原文链接**: [http://www.jasonwillems.com/technology/2025/12/17/Tech-Is-Fun-Again/](http://www.jasonwillems.com/technology/2025/12/17/Tech-Is-Fun-Again/)

生成摘要时出错

---

## 29. Updates to our web search products and  Programmable Search Engine capabilities

**原文标题**: Updates to our web search products and  Programmable Search Engine capabilities

**原文链接**: [https://programmablesearchengine.googleblog.com/2026/01/updates-to-our-web-search-products.html](https://programmablesearchengine.googleblog.com/2026/01/updates-to-our-web-search-products.html)

生成摘要时出错

---

## 30. Banned C++ features in Chromium

**原文标题**: Banned C++ features in Chromium

**原文链接**: [https://chromium.googlesource.com/chromium/src/+/main/styleguide/c++/c++-features.md](https://chromium.googlesource.com/chromium/src/+/main/styleguide/c++/c++-features.md)

生成摘要时出错

---

## 31. White House Posts Digitally Altered Image of Woman Arrested After ICE Protest

**原文标题**: White House Posts Digitally Altered Image of Woman Arrested After ICE Protest

**原文链接**: [https://www.theguardian.com/us-news/2026/jan/22/white-house-ice-protest-arrest-altered-image](https://www.theguardian.com/us-news/2026/jan/22/white-house-ice-protest-arrest-altered-image)

生成摘要时出错

---

## 32. Auto-compact not triggering on Claude.ai despite being marked as fixed

**原文标题**: Auto-compact not triggering on Claude.ai despite being marked as fixed

**原文链接**: [https://github.com/anthropics/claude-code/issues/18866](https://github.com/anthropics/claude-code/issues/18866)

生成摘要时出错

---

## 33. Man shot and killed by federal agents in south Minneapolis this morning

**原文标题**: Man shot and killed by federal agents in south Minneapolis this morning

**原文链接**: [https://www.startribune.com/ice-raids-minnesota/601546426](https://www.startribune.com/ice-raids-minnesota/601546426)

生成摘要时出错

---

## 34. Replacing Protobuf with Rust

**原文标题**: Replacing Protobuf with Rust

**原文链接**: [https://pgdog.dev/blog/replace-protobuf-with-rust](https://pgdog.dev/blog/replace-protobuf-with-rust)

生成摘要时出错

---

## 35. Talking to LLMs has improved my thinking

**原文标题**: Talking to LLMs has improved my thinking

**原文链接**: [https://philipotoole.com/why-talking-to-llms-has-improved-my-thinking/](https://philipotoole.com/why-talking-to-llms-has-improved-my-thinking/)

生成摘要时出错

---

## 36. Route leak incident on January 22, 2026

**原文标题**: Route leak incident on January 22, 2026

**原文链接**: [https://blog.cloudflare.com/route-leak-incident-january-22-2026/](https://blog.cloudflare.com/route-leak-incident-january-22-2026/)

生成摘要时出错

---

## 37. Minnesota activist releases arrest video after manipulated White House version

**原文标题**: Minnesota activist releases arrest video after manipulated White House version

**原文链接**: [https://apnews.com/article/minnesota-activist-ice-protest-church-video-49faf3efd54e496388651aac1369fb44](https://apnews.com/article/minnesota-activist-ice-protest-church-video-49faf3efd54e496388651aac1369fb44)

生成摘要时出错

---

## 38. I Like GitLab

**原文标题**: I Like GitLab

**原文链接**: [https://www.whileforloop.com/en/blog/2026/01/21/i-like-gitlab/](https://www.whileforloop.com/en/blog/2026/01/21/i-like-gitlab/)

生成摘要时出错

---

## 39. The lost art of XML

**原文标题**: The lost art of XML

**原文链接**: [https://marcosmagueta.com/blog/the-lost-art-of-xml/](https://marcosmagueta.com/blog/the-lost-art-of-xml/)

生成摘要时出错

---

## 40. Improving the usability of C libraries in Swift

**原文标题**: Improving the usability of C libraries in Swift

**原文链接**: [https://www.swift.org/blog/improving-usability-of-c-libraries-in-swift/](https://www.swift.org/blog/improving-usability-of-c-libraries-in-swift/)

生成摘要时出错

---

## 41. “Let people help” – Advice that made a big difference to a grieving widow

**原文标题**: “Let people help” – Advice that made a big difference to a grieving widow

**原文链接**: [https://www.npr.org/2026/01/20/nx-s1-5683170/let-them-the-small-bit-of-advice-that-made-a-big-difference-to-a-grieving-widow](https://www.npr.org/2026/01/20/nx-s1-5683170/let-them-the-small-bit-of-advice-that-made-a-big-difference-to-a-grieving-widow)

生成摘要时出错

---

## 42. TikTok is now collecting more data about its users

**原文标题**: TikTok is now collecting more data about its users

**原文链接**: [https://www.wired.com/story/tiktok-new-privacy-policy/](https://www.wired.com/story/tiktok-new-privacy-policy/)

生成摘要时出错

---

## 43. Anthropic Economic Index report: economic primitives

**原文标题**: Anthropic Economic Index report: economic primitives

**原文链接**: [https://www.anthropic.com/research/anthropic-economic-index-january-2026-report](https://www.anthropic.com/research/anthropic-economic-index-january-2026-report)

生成摘要时出错

---

## 44. White House defends sharing AI image showing arrested woman crying

**原文标题**: White House defends sharing AI image showing arrested woman crying

**原文链接**: [https://www.bbc.co.uk/news/live/ce9yydgmzdvt](https://www.bbc.co.uk/news/live/ce9yydgmzdvt)

生成摘要时出错

---

## 45. 'Active' sitting is better for brain health: review of studies

**原文标题**: 'Active' sitting is better for brain health: review of studies

**原文链接**: [https://www.sciencealert.com/not-all-sitting-is-equal-one-type-was-just-linked-to-better-brain-health](https://www.sciencealert.com/not-all-sitting-is-equal-one-type-was-just-linked-to-better-brain-health)

生成摘要时出错

---

## 46. U.S. Formally Withdraws from World Health Organization

**原文标题**: U.S. Formally Withdraws from World Health Organization

**原文链接**: [https://www.nytimes.com/2026/01/22/us/politics/united-states-withdraws-world-health-organization.html](https://www.nytimes.com/2026/01/22/us/politics/united-states-withdraws-world-health-organization.html)

生成摘要时出错

---

## 47. Many Small Queries Are Efficient in SQLite

**原文标题**: Many Small Queries Are Efficient in SQLite

**原文链接**: [https://www.sqlite.org/np1queryprob.html](https://www.sqlite.org/np1queryprob.html)

生成摘要时出错

---

## 48. Claude Code's new hidden feature: Swarms

**原文标题**: Claude Code's new hidden feature: Swarms

**原文链接**: [https://twitter.com/NicerInPerson/status/2014989679796347375](https://twitter.com/NicerInPerson/status/2014989679796347375)

生成摘要时出错

---

## 49. Mental Models (2018)

**原文标题**: Mental Models (2018)

**原文链接**: [https://fs.blog/mental-models/](https://fs.blog/mental-models/)

生成摘要时出错

---

## 50. Stunnel

**原文标题**: Stunnel

**原文链接**: [https://www.stunnel.org/](https://www.stunnel.org/)

生成摘要时出错

---

## 51. United States Completes WHO Withdrawal

**原文标题**: United States Completes WHO Withdrawal

**原文链接**: [https://www.hhs.gov/press-room/united-states-completes-who-withdrawal.html](https://www.hhs.gov/press-room/united-states-completes-who-withdrawal.html)

生成摘要时出错

---

## 52. White House Posts Altered Photo Showing Arrested Minnesota Protester Crying

**原文标题**: White House Posts Altered Photo Showing Arrested Minnesota Protester Crying

**原文链接**: [https://www.nytimes.com/2026/01/22/us/politics/nekima-armstrong-photo-white-house.html](https://www.nytimes.com/2026/01/22/us/politics/nekima-armstrong-photo-white-house.html)

生成摘要时出错

---

## 53. Federal Agents Kill Another Person in Minneapolis Immigration Crackdown

**原文标题**: Federal Agents Kill Another Person in Minneapolis Immigration Crackdown

**原文链接**: [https://time.com/7357547/minneapolis-shooting-ice-agent/](https://time.com/7357547/minneapolis-shooting-ice-agent/)

生成摘要时出错

---

## 54. House vote keeps federal "kill switch" vehicle mandate

**原文标题**: House vote keeps federal "kill switch" vehicle mandate

**原文链接**: [https://reclaimthenet.org/house-vote-keeps-federal-kill-switch-vehicle-mandat](https://reclaimthenet.org/house-vote-keeps-federal-kill-switch-vehicle-mandat)

生成摘要时出错

---

## 55. SEC obtains final consent judgments against former FTX and Alameda executives

**原文标题**: SEC obtains final consent judgments against former FTX and Alameda executives

**原文链接**: [https://www.sec.gov/enforcement-litigation/litigation-releases/lr-26450](https://www.sec.gov/enforcement-litigation/litigation-releases/lr-26450)

生成摘要时出错

---

## 56. After two years of vibecoding, I'm back to writing by hand [video]

**原文标题**: After two years of vibecoding, I'm back to writing by hand [video]

**原文链接**: [https://www.youtube.com/watch?v=SKTsNV41DYg](https://www.youtube.com/watch?v=SKTsNV41DYg)

生成摘要时出错

---

## 57. Notes on the Intel 8086 processor's arithmetic-logic unit

**原文标题**: Notes on the Intel 8086 processor's arithmetic-logic unit

**原文链接**: [https://www.righto.com/2026/01/notes-on-intel-8086-processors.html](https://www.righto.com/2026/01/notes-on-intel-8086-processors.html)

生成摘要时出错

---

## 58. The state of modern AI text to speech systems for screen reader users

**原文标题**: The state of modern AI text to speech systems for screen reader users

**原文链接**: [https://stuff.interfree.ca/2026/01/05/ai-tts-for-screenreaders.html](https://stuff.interfree.ca/2026/01/05/ai-tts-for-screenreaders.html)

生成摘要时出错

---

## 59. Tao Te Ching – Translated by Ursula K. Le Guin

**原文标题**: Tao Te Ching – Translated by Ursula K. Le Guin

**原文链接**: [https://github.com/nrrb/tao-te-ching/blob/master/Ursula%20K%20Le%20Guin.md](https://github.com/nrrb/tao-te-ching/blob/master/Ursula%20K%20Le%20Guin.md)

生成摘要时出错

---

## 60. Nobody likes lag: How to make low-latency dev sandboxes

**原文标题**: Nobody likes lag: How to make low-latency dev sandboxes

**原文链接**: [https://www.compyle.ai/blog/nobody-likes-lag/](https://www.compyle.ai/blog/nobody-likes-lag/)

生成摘要时出错

---

## 61. Why I don't have fun with Claude Code

**原文标题**: Why I don't have fun with Claude Code

**原文链接**: [https://brennan.io/2026/01/23/claude-code/](https://brennan.io/2026/01/23/claude-code/)

生成摘要时出错

---

## 62. DOGE improperly accessed and shared Social Security data

**原文标题**: DOGE improperly accessed and shared Social Security data

**原文链接**: [https://blog.quintarelli.it/2026/01/how-doge-improperly-accessed-and-shared-social-security-data-npr/](https://blog.quintarelli.it/2026/01/how-doge-improperly-accessed-and-shared-social-security-data-npr/)

生成摘要时出错

---

## 63. Killing the ISP Appliance: An eBPF/XDP Approach to Distributed BNG

**原文标题**: Killing the ISP Appliance: An eBPF/XDP Approach to Distributed BNG

**原文链接**: [https://markgascoyne.co.uk/posts/ebpf-bng/](https://markgascoyne.co.uk/posts/ebpf-bng/)

生成摘要时出错

---

## 64. 80386 Multiplication and Division

**原文标题**: 80386 Multiplication and Division

**原文链接**: [https://nand2mario.github.io/posts/2026/80386_multiplication_and_division/](https://nand2mario.github.io/posts/2026/80386_multiplication_and_division/)

生成摘要时出错

---

## 65. Are we all plagiarists now?

**原文标题**: Are we all plagiarists now?

**原文链接**: [https://www.economist.com/culture/2026/01/22/are-we-all-plagiarists-now](https://www.economist.com/culture/2026/01/22/are-we-all-plagiarists-now)

生成摘要时出错

---

## 66. Waypoint-1: Real-Time Interactive Video Diffusion from Overworld

**原文标题**: Waypoint-1: Real-Time Interactive Video Diffusion from Overworld

**原文链接**: [https://huggingface.co/blog/waypoint-1](https://huggingface.co/blog/waypoint-1)

生成摘要时出错

---

## 67. Tesla fined for repeatedly failing to help UK police over driving offences

**原文标题**: Tesla fined for repeatedly failing to help UK police over driving offences

**原文链接**: [https://www.bbc.co.uk/news/articles/c0r44zpprg7o](https://www.bbc.co.uk/news/articles/c0r44zpprg7o)

生成摘要时出错

---

## 68. Presence in Death

**原文标题**: Presence in Death

**原文链接**: [https://rubinmuseum.org/presence-in-death/](https://rubinmuseum.org/presence-in-death/)

生成摘要时出错

---

## 69. December in Servo: multiple windows, proxy support, better caching, and more

**原文标题**: December in Servo: multiple windows, proxy support, better caching, and more

**原文链接**: [https://servo.org/blog/2026/01/23/december-in-servo/](https://servo.org/blog/2026/01/23/december-in-servo/)

生成摘要时出错

---

## 70. Extracting a UART Password via SPI Flash Instruction Tracing

**原文标题**: Extracting a UART Password via SPI Flash Instruction Tracing

**原文链接**: [https://zuernerd.github.io/blog/2026/01/07/switch-password.html](https://zuernerd.github.io/blog/2026/01/07/switch-password.html)

生成摘要时出错

---

## 71. ICE detains five-year-old Minnesota boy arriving home, say school officials

**原文标题**: ICE detains five-year-old Minnesota boy arriving home, say school officials

**原文链接**: [https://www.theguardian.com/us-news/2026/jan/21/ice-arrests-five-year-old-boy-minnesota](https://www.theguardian.com/us-news/2026/jan/21/ice-arrests-five-year-old-boy-minnesota)

生成摘要时出错

---

## 72. Repatriate the gold': German economists advise withdrawal from US vaults

**原文标题**: Repatriate the gold': German economists advise withdrawal from US vaults

**原文链接**: [https://www.theguardian.com/world/2026/jan/24/repatriate-the-gold-german-economists-advise-withdrawal-from-us-vaults](https://www.theguardian.com/world/2026/jan/24/repatriate-the-gold-german-economists-advise-withdrawal-from-us-vaults)

生成摘要时出错

---

## 73. Wilson Lin on FastRender: a browser built by parallel agents

**原文标题**: Wilson Lin on FastRender: a browser built by parallel agents

**原文链接**: [https://simonwillison.net/2026/Jan/23/fastrender/](https://simonwillison.net/2026/Jan/23/fastrender/)

生成摘要时出错

---

## 74. AI can 10x developers in creating tech debt

**原文标题**: AI can 10x developers in creating tech debt

**原文链接**: [https://stackoverflow.blog/2026/01/23/ai-can-10x-developers-in-creating-tech-debt/](https://stackoverflow.blog/2026/01/23/ai-can-10x-developers-in-creating-tech-debt/)

生成摘要时出错

---

## 75. Is liberal democracy in terminal decline?

**原文标题**: Is liberal democracy in terminal decline?

**原文链接**: [https://www.ft.com/content/b4d2c7a3-587d-440f-a7a9-7e5e85b93a88](https://www.ft.com/content/b4d2c7a3-587d-440f-a7a9-7e5e85b93a88)

生成摘要时出错

---

## 76. Colorectal cancer is now the top cause of cancer death in younger people

**原文标题**: Colorectal cancer is now the top cause of cancer death in younger people

**原文链接**: [https://www.wsj.com/health/healthcare/colorectal-cancer-is-now-the-top-cause-of-cancer-death-in-younger-people-02f08587](https://www.wsj.com/health/healthcare/colorectal-cancer-is-now-the-top-cause-of-cancer-death-in-younger-people-02f08587)

生成摘要时出错

---

## 77. Microsoft Gave FBI Keys to Unlock Encrypted Data, Exposing Major Privacy Flaw

**原文标题**: Microsoft Gave FBI Keys to Unlock Encrypted Data, Exposing Major Privacy Flaw

**原文链接**: [https://www.forbes.com/sites/thomasbrewster/2026/01/22/microsoft-gave-fbi-keys-to-unlock-bitlocker-encrypted-data/](https://www.forbes.com/sites/thomasbrewster/2026/01/22/microsoft-gave-fbi-keys-to-unlock-bitlocker-encrypted-data/)

生成摘要时出错

---

## 78. Minneapolis Authorities Respond to Shooting Involving ICE Agents

**原文标题**: Minneapolis Authorities Respond to Shooting Involving ICE Agents

**原文链接**: [https://www.nytimes.com/live/2026/01/24/us/minneapolis-shooting-ice](https://www.nytimes.com/live/2026/01/24/us/minneapolis-shooting-ice)

生成摘要时出错

---

## 79. FOSS "just fork it" delusion

**原文标题**: FOSS "just fork it" delusion

**原文链接**: [https://hamishcampbell.com/foss-just-fork-it-delusion/](https://hamishcampbell.com/foss-just-fork-it-delusion/)

生成摘要时出错

---

## 80. My review of the Nüborn Baby at 3 months

**原文标题**: My review of the Nüborn Baby at 3 months

**原文链接**: [https://joshcollinsworth.com/blog/baby-review](https://joshcollinsworth.com/blog/baby-review)

生成摘要时出错

---

## 81. Neko: History of a Software Pet (2022)

**原文标题**: Neko: History of a Software Pet (2022)

**原文链接**: [https://eliotakira.com/neko/](https://eliotakira.com/neko/)

生成摘要时出错

---

## 82. The Uncomfortable Math of Working for Yourself

**原文标题**: The Uncomfortable Math of Working for Yourself

**原文链接**: [https://thomasunise.com/the-uncomfortable-math-of-working-for-yourself/](https://thomasunise.com/the-uncomfortable-math-of-working-for-yourself/)

生成摘要时出错

---

## 83. You can't pay me to prompt

**原文标题**: You can't pay me to prompt

**原文链接**: [https://dbushell.com/2025/06/18/ai-policy/](https://dbushell.com/2025/06/18/ai-policy/)

生成摘要时出错

---

## 84. Show HN: I built a space travel calculator using Vanilla JavaScript

**原文标题**: Show HN: I built a space travel calculator using Vanilla JavaScript

**原文链接**: [https://cosmic-odometer.vercel.app/](https://cosmic-odometer.vercel.app/)

生成摘要时出错

---

## 85. CEOs Say AI Is Making Work More Efficient. Employees Tell a Different Story

**原文标题**: CEOs Say AI Is Making Work More Efficient. Employees Tell a Different Story

**原文链接**: [https://www.wsj.com/lifestyle/workplace/ceos-say-ai-is-making-work-more-efficient-employees-tell-a-different-story-6613ce9d](https://www.wsj.com/lifestyle/workplace/ceos-say-ai-is-making-work-more-efficient-employees-tell-a-different-story-6613ce9d)

生成摘要时出错

---

## 86. Arkansas inmates restricted from receiving physical books, other media directly

**原文标题**: Arkansas inmates restricted from receiving physical books, other media directly

**原文链接**: [https://arkansasadvocate.com/2025/12/19/arkansas-inmates-restricted-from-receiving-physical-books-other-media-directly-under-new-policy/](https://arkansasadvocate.com/2025/12/19/arkansas-inmates-restricted-from-receiving-physical-books-other-media-directly-under-new-policy/)

生成摘要时出错

---

## 87. US Vaccine Panel Chair Says Polio and Other Shots Should Be Optional

**原文标题**: US Vaccine Panel Chair Says Polio and Other Shots Should Be Optional

**原文链接**: [https://www.nytimes.com/2026/01/23/health/milhoan-vaccines-optional-polio.html](https://www.nytimes.com/2026/01/23/health/milhoan-vaccines-optional-polio.html)

生成摘要时出错

---

## 88. What Will You Do When AI runs Out of Money and Disappear?

**原文标题**: What Will You Do When AI runs Out of Money and Disappear?

**原文链接**: [https://louwrentius.com/what-will-you-do-when-ai-will-run-out-of-money-and-disappear.html](https://louwrentius.com/what-will-you-do-when-ai-will-run-out-of-money-and-disappear.html)

生成摘要时出错

---

## 89. Yann LeCun's new venture is a contrarian bet against large language models

**原文标题**: Yann LeCun's new venture is a contrarian bet against large language models

**原文链接**: [https://www.technologyreview.com/2026/01/22/1131661/yann-lecuns-new-venture-ami-labs/](https://www.technologyreview.com/2026/01/22/1131661/yann-lecuns-new-venture-ami-labs/)

生成摘要时出错

---

## 90. Viking Ship Museum in Denmark announces the discovery of the largest cog

**原文标题**: Viking Ship Museum in Denmark announces the discovery of the largest cog

**原文链接**: [https://www.medievalists.net/2025/12/medieval-ship-discovered-copenhagen/](https://www.medievalists.net/2025/12/medieval-ship-discovered-copenhagen/)

生成摘要时出错

---

## 91. Show HN: CLI for working with Apple Core ML models

**原文标题**: Show HN: CLI for working with Apple Core ML models

**原文链接**: [https://github.com/schappim/coreml-cli](https://github.com/schappim/coreml-cli)

生成摘要时出错

---

## 92. Skill.md: An open standard for agent skills

**原文标题**: Skill.md: An open standard for agent skills

**原文链接**: [https://www.mintlify.com/blog/skill-md](https://www.mintlify.com/blog/skill-md)

生成摘要时出错

---

## 93. Rent-Only Copyright Culture Makes Us All Worse Off

**原文标题**: Rent-Only Copyright Culture Makes Us All Worse Off

**原文链接**: [https://www.eff.org/deeplinks/2026/01/rent-only-copyright-culture-makes-us-all-worse](https://www.eff.org/deeplinks/2026/01/rent-only-copyright-culture-makes-us-all-worse)

生成摘要时出错

---

## 94. Maze Algorithms (2017)

**原文标题**: Maze Algorithms (2017)

**原文链接**: [http://www.jamisbuck.org/mazes/](http://www.jamisbuck.org/mazes/)

生成摘要时出错

---

## 95. Doubting U.S. resolve, Europe looks to bolster its own nuclear arsenal

**原文标题**: Doubting U.S. resolve, Europe looks to bolster its own nuclear arsenal

**原文链接**: [https://www.nbcnews.com/politics/white-house/doubting-us-resolve-europe-looks-bolster-nuclear-arsenal-rcna254925](https://www.nbcnews.com/politics/white-house/doubting-us-resolve-europe-looks-bolster-nuclear-arsenal-rcna254925)

生成摘要时出错

---

## 96. XHTML Club

**原文标题**: XHTML Club

**原文链接**: [https://xhtml.club/](https://xhtml.club/)

生成摘要时出错

---

## 97. Modetc: Move your dotfiles from kernel space

**原文标题**: Modetc: Move your dotfiles from kernel space

**原文链接**: [https://maxwell.eurofusion.eu/git/rnhmjoj/modetc](https://maxwell.eurofusion.eu/git/rnhmjoj/modetc)

生成摘要时出错

---

## 98. Autodesk burns the village to feed AI and the Cloud – cuts 7% of workforce

**原文标题**: Autodesk burns the village to feed AI and the Cloud – cuts 7% of workforce

**原文链接**: [https://blog.adafruit.com/2026/01/22/autodesk-burns-the-village-to-feed-ai-and-the-cloud-cuts-7-of-workforce/](https://blog.adafruit.com/2026/01/22/autodesk-burns-the-village-to-feed-ai-and-the-cloud-cuts-7-of-workforce/)

生成摘要时出错

---

## 99. The Internet Doesn't Suck: Blame Big Tech, Not the Internet

**原文标题**: The Internet Doesn't Suck: Blame Big Tech, Not the Internet

**原文链接**: [https://riverseeber.net/blog/post/the-internet-doesnt-suck/](https://riverseeber.net/blog/post/the-internet-doesnt-suck/)

生成摘要时出错

---

## 100. Why are there so many CPU bugs nowadays

**原文标题**: Why are there so many CPU bugs nowadays

**原文链接**: [https://mas.to/@gabrielesvelto/115939583202357863](https://mas.to/@gabrielesvelto/115939583202357863)

生成摘要时出错

---

