# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-01-24.md)

*最后自动更新时间: 2026-01-24 19:46:58*
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

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 2 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 3 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 4 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 5 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 6 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 7 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 8 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 9 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 10 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 11 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 12 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 13 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 14 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 15 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 16 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 17 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 18 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 19 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 20 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 21 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 22 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 23 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 24 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 25 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 26 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 27 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 28 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 29 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 30 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 31 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 32 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 33 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 34 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 35 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 36 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 37 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 38 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 39 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 40 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 41 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 42 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 43 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 44 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 45 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 46 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 47 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 48 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 49 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 50 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 51 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 52 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 53 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 54 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 55 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 56 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 57 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 58 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 59 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 60 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 61 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 62 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 63 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 64 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 65 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 66 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 67 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 68 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 69 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 70 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 71 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 72 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 73 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 74 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 75 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 76 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 77 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 78 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 79 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
| 80 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
