# Hacker News 热门文章摘要 (2026-09-19)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

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

## 11. Two parallel neural ectoderm progenitors contribute to the developing brain

**原文标题**: Two parallel neural ectoderm progenitors contribute to the developing brain

**原文链接**: [https://med.stanford.edu/news/all-news/2026/09/two-separate-brains.html](https://med.stanford.edu/news/all-news/2026/09/two-separate-brains.html)

生成摘要时出错

---

## 12. Bonsai 2 27B: Near-Lossless Compression in a 9x Smaller Footprint

**原文标题**: Bonsai 2 27B: Near-Lossless Compression in a 9x Smaller Footprint

**原文链接**: [https://prismml.com/news/bonsai-2-27b](https://prismml.com/news/bonsai-2-27b)

生成摘要时出错

---

## 13. US Military had close call after using AI for hallucinated intelligence report

**原文标题**: US Military had close call after using AI for hallucinated intelligence report

**原文链接**: [https://www.cnn.com/2026/09/18/politics/us-military-ai-false-intelligence-china-ship](https://www.cnn.com/2026/09/18/politics/us-military-ai-false-intelligence-china-ship)

生成摘要时出错

---

## 14. A heap overflow and SSO misconfiguration to compromise OpenAI internal repos

**原文标题**: A heap overflow and SSO misconfiguration to compromise OpenAI internal repos

**原文链接**: [https://www.hacktron.ai/blog/hacking-openai](https://www.hacktron.ai/blog/hacking-openai)

生成摘要时出错

---

## 15. Saving another 100TB of RAM

**原文标题**: Saving another 100TB of RAM

**原文链接**: [https://blog.cloudflare.com/saving-100-tb-of-ram-with-math/](https://blog.cloudflare.com/saving-100-tb-of-ram-with-math/)

生成摘要时出错

---

## 16. San Francisco Onion Futures Company

**原文标题**: San Francisco Onion Futures Company

**原文链接**: [https://onionfutures.com/](https://onionfutures.com/)

生成摘要时出错

---

## 17. Qwen 3.8 Omni Flash

**原文标题**: Qwen 3.8 Omni Flash

**原文链接**: [https://qwen.ai/blog?id=qwen3.8-omni-flash](https://qwen.ai/blog?id=qwen3.8-omni-flash)

生成摘要时出错

---

## 18. GPT-6 Astra Solves a WWI German Radio Cipher

**原文标题**: GPT-6 Astra Solves a WWI German Radio Cipher

**原文链接**: [https://www.prinzai.com/p/gpt-6-astra-solves-a-wwi-german-radio](https://www.prinzai.com/p/gpt-6-astra-solves-a-wwi-german-radio)

生成摘要时出错

---

## 19. Jemalloc 5.4.0

**原文标题**: Jemalloc 5.4.0

**原文链接**: [https://github.com/jemalloc/jemalloc/releases/tag/5.4.0](https://github.com/jemalloc/jemalloc/releases/tag/5.4.0)

生成摘要时出错

---

## 20. Inside ZCode: Silently uploading your Git history to the cloud

**原文标题**: Inside ZCode: Silently uploading your Git history to the cloud

**原文链接**: [https://blog.ferstar.org/en/posts/zcode-silent-workspace-snapshot-upload/](https://blog.ferstar.org/en/posts/zcode-silent-workspace-snapshot-upload/)

生成摘要时出错

---

## 21. Korea raises data breach fines to 10% of revenue

**原文标题**: Korea raises data breach fines to 10% of revenue

**原文链接**: [https://www.koreajoongangdaily.com/business/korea-raises-data-breach-fines-to-10-of-revenue/12869899](https://www.koreajoongangdaily.com/business/korea-raises-data-breach-fines-to-10-of-revenue/12869899)

生成摘要时出错

---

## 22. Bend 2 and the Vibe-Coding Trap

**原文标题**: Bend 2 and the Vibe-Coding Trap

**原文链接**: [https://blog.liampwll.com/posts/bend_vibe_coding/](https://blog.liampwll.com/posts/bend_vibe_coding/)

生成摘要时出错

---

## 23. Warren Buffett Steps Down as Berkshire Chairman, Names Son to Replace Him

**原文标题**: Warren Buffett Steps Down as Berkshire Chairman, Names Son to Replace Him

**原文链接**: [https://www.nytimes.com/2026/09/18/business/warren-buffett-berkshire-chairman.html](https://www.nytimes.com/2026/09/18/business/warren-buffett-berkshire-chairman.html)

生成摘要时出错

---

## 24. Minimal Phone 2

**原文标题**: Minimal Phone 2

**原文链接**: [https://minimalcompany.com/](https://minimalcompany.com/)

生成摘要时出错

---

## 25. The scourge of x86 emulation

**原文标题**: The scourge of x86 emulation

**原文链接**: [https://fex-emu.com/Scourge-of-emulation/](https://fex-emu.com/Scourge-of-emulation/)

生成摘要时出错

---

## 26. If math is more than proof, we need to better celebrate the rest of it

**原文标题**: If math is more than proof, we need to better celebrate the rest of it

**原文链接**: [https://terrytao.wordpress.com/2026/09/18/if-math-is-more-than-proof-we-need-to-better-celebrate-the-rest-of-it/](https://terrytao.wordpress.com/2026/09/18/if-math-is-more-than-proof-we-need-to-better-celebrate-the-rest-of-it/)

生成摘要时出错

---

## 27. ZCode, the GLM coding agent, silently uploads your Git history

**原文标题**: ZCode, the GLM coding agent, silently uploads your Git history

**原文链接**: [https://tokenstead.ai/guides/zcode-silent-git-history-upload](https://tokenstead.ai/guides/zcode-silent-git-history-upload)

生成摘要时出错

---

## 28. I vibed a proof of Conway's conjecture

**原文标题**: I vibed a proof of Conway's conjecture

**原文链接**: [https://overreacted.io/how-i-vibed-a-proof-of-conways-conjecture/](https://overreacted.io/how-i-vibed-a-proof-of-conways-conjecture/)

生成摘要时出错

---

## 29. How SpaceX streamlined the Raptor engine

**原文标题**: How SpaceX streamlined the Raptor engine

**原文链接**: [https://www.construction-physics.com/p/how-spacex-streamlined-the-raptor](https://www.construction-physics.com/p/how-spacex-streamlined-the-raptor)

生成摘要时出错

---

## 30. Sex, AI, and the Apocalypse

**原文标题**: Sex, AI, and the Apocalypse

**原文链接**: [https://www.iankduncan.com/personal/2026-09-16-sex-ai-and-the-apocalypse/](https://www.iankduncan.com/personal/2026-09-16-sex-ai-and-the-apocalypse/)

生成摘要时出错

---

## 31. Border agents can search cellphones without a warrant or reasonable suspicion

**原文标题**: Border agents can search cellphones without a warrant or reasonable suspicion

**原文链接**: [https://lawandcrime.com/high-profile/the-government-was-entitled-trumps-border-agents-can-now-search-cellphones-without-a-warrant-probable-cause-or-reasonable-suspicion-2nd-circuit-rules/](https://lawandcrime.com/high-profile/the-government-was-entitled-trumps-border-agents-can-now-search-cellphones-without-a-warrant-probable-cause-or-reasonable-suspicion-2nd-circuit-rules/)

生成摘要时出错

---

## 32. Show HN: Cactus Needle 3: 8-29MB automation models can match DeepSeek V4 Flash

**原文标题**: Show HN: Cactus Needle 3: 8-29MB automation models can match DeepSeek V4 Flash

**原文链接**: [https://cactuscompute.com/needle](https://cactuscompute.com/needle)

生成摘要时出错

---

## 33. North Korean nuclear test sets off years of earthquakes

**原文标题**: North Korean nuclear test sets off years of earthquakes

**原文链接**: [https://www.science.org/content/article/north-korean-nuclear-test-sets-years-earthquakes](https://www.science.org/content/article/north-korean-nuclear-test-sets-years-earthquakes)

生成摘要时出错

---

## 34. An empirical study of harness design for coding agents

**原文标题**: An empirical study of harness design for coding agents

**原文链接**: [https://arxiv.org/abs/2609.20804](https://arxiv.org/abs/2609.20804)

生成摘要时出错

---

## 35. More than 100k people in Japan are now aged 100 or older

**原文标题**: More than 100k people in Japan are now aged 100 or older

**原文链接**: [https://www.bbc.com/news/articles/cmzezj5e18xxo](https://www.bbc.com/news/articles/cmzezj5e18xxo)

生成摘要时出错

---

## 36. Photon-Emission-Guided Laser Fault Injection Enables RP2350 Secure Debug

**原文标题**: Photon-Emission-Guided Laser Fault Injection Enables RP2350 Secure Debug

**原文链接**: [https://donjon.ledger.com/blog/rp2350-secure-debug-laser-fault-injection/](https://donjon.ledger.com/blog/rp2350-secure-debug-laser-fault-injection/)

生成摘要时出错

---

## 37. Warez: The Infrastructure and Aesthetics of Piracy (2021)

**原文标题**: Warez: The Infrastructure and Aesthetics of Piracy (2021)

**原文链接**: [https://archive.org/details/b904a8eb-9c98-4bb1-bf25-3cb9d075b157](https://archive.org/details/b904a8eb-9c98-4bb1-bf25-3cb9d075b157)

生成摘要时出错

---

## 38. There's no point at which turning your brain off will work

**原文标题**: There's no point at which turning your brain off will work

**原文链接**: [https://danluu.com/brain-off/](https://danluu.com/brain-off/)

生成摘要时出错

---

## 39. How OpenAI Used Its Own LLMs to Design Its Jalapeño Chip

**原文标题**: How OpenAI Used Its Own LLMs to Design Its Jalapeño Chip

**原文链接**: [https://spectrum.ieee.org/llms-for-chip-design](https://spectrum.ieee.org/llms-for-chip-design)

生成摘要时出错

---

## 40. US troop deaths during Iran war exceed Pentagon count by at least four

**原文标题**: US troop deaths during Iran war exceed Pentagon count by at least four

**原文链接**: [https://www.reuters.com/world/middle-east/us-troop-deaths-iran-war-exceed-pentagon-count-by-least-four-washington-post-2026-09-18/](https://www.reuters.com/world/middle-east/us-troop-deaths-iran-war-exceed-pentagon-count-by-least-four-washington-post-2026-09-18/)

生成摘要时出错

---

## 41. Pre-Greek: The lost language hidden within Ancient Greek

**原文标题**: Pre-Greek: The lost language hidden within Ancient Greek

**原文链接**: [https://linguisticdiscovery.com/posts/pre-greek/](https://linguisticdiscovery.com/posts/pre-greek/)

生成摘要时出错

---

## 42. C++26: Trivial infinite loops are no longer undefined behaviour

**原文标题**: C++26: Trivial infinite loops are no longer undefined behaviour

**原文链接**: [https://www.sandordargo.com/blog/2026/09/16/cpp26-trivial-infinite-loops](https://www.sandordargo.com/blog/2026/09/16/cpp26-trivial-infinite-loops)

生成摘要时出错

---

## 43. Flet 1.0 – Build cross-platform apps in Python

**原文标题**: Flet 1.0 – Build cross-platform apps in Python

**原文链接**: [https://flet.dev/](https://flet.dev/)

生成摘要时出错

---

## 44. What Zig felt like, coming from Rust

**原文标题**: What Zig felt like, coming from Rust

**原文链接**: [https://besok.github.io/posts/what-zig-felt-like-coming-from-rust/](https://besok.github.io/posts/what-zig-felt-like-coming-from-rust/)

生成摘要时出错

---

## 45. Tin: full-text search for Postgres

**原文标题**: Tin: full-text search for Postgres

**原文链接**: [https://planetscale.com/blog/introducing-tin](https://planetscale.com/blog/introducing-tin)

生成摘要时出错

---

## 46. The most important product decision is what you don't build

**原文标题**: The most important product decision is what you don't build

**原文链接**: [https://liamnugent.me/posts/what-you-dont-build/](https://liamnugent.me/posts/what-you-dont-build/)

生成摘要时出错

---

## 47. Science Is Open Software

**原文标题**: Science Is Open Software

**原文链接**: [https://jepedersen.dk/blog/202505_research/](https://jepedersen.dk/blog/202505_research/)

生成摘要时出错

---

## 48. US Treasuries Have Become Unappetizing for Foreign Central Banks and Governments

**原文标题**: US Treasuries Have Become Unappetizing for Foreign Central Banks and Governments

**原文链接**: [https://wolfstreet.com/2026/09/17/treasuries-have-become-badly-unappetizing-for-foreign-central-banks-governments/](https://wolfstreet.com/2026/09/17/treasuries-have-become-badly-unappetizing-for-foreign-central-banks-governments/)

生成摘要时出错

---

## 49. I hate you Microsoft

**原文标题**: I hate you Microsoft

**原文链接**: [https://henriquenunez.eu/posts/you_did_it_again_ms/](https://henriquenunez.eu/posts/you_did_it_again_ms/)

生成摘要时出错

---

## 50. Xcode 27.1 Beta Release Notes

**原文标题**: Xcode 27.1 Beta Release Notes

**原文链接**: [https://developer.apple.com/documentation/xcode-release-notes/xcode-27_1-release-notes](https://developer.apple.com/documentation/xcode-release-notes/xcode-27_1-release-notes)

生成摘要时出错

---

## 51. I think you should almost never use AI to write

**原文标题**: I think you should almost never use AI to write

**原文链接**: [https://erichgrunewald.substack.com/p/why-you-should-almost-never-use-ai](https://erichgrunewald.substack.com/p/why-you-should-almost-never-use-ai)

生成摘要时出错

---

## 52. Alibaba open-sources AI model that can detect cancer and nearly 150 conditions

**原文标题**: Alibaba open-sources AI model that can detect cancer and nearly 150 conditions

**原文链接**: [https://www.scmp.com/tech/big-tech/article/3368055/alibaba-open-sources-medical-ai-model-can-detect-cancer-and-nearly-150-conditions](https://www.scmp.com/tech/big-tech/article/3368055/alibaba-open-sources-medical-ai-model-can-detect-cancer-and-nearly-150-conditions)

生成摘要时出错

---

## 53. Second Circuit allows government to search electronic devices at the border

**原文标题**: Second Circuit allows government to search electronic devices at the border

**原文链接**: [https://knightcolumbia.org/content/second-circuit-allows-government-to-search-electronic-devices-at-the-border-without-any-suspicion](https://knightcolumbia.org/content/second-circuit-allows-government-to-search-electronic-devices-at-the-border-without-any-suspicion)

生成摘要时出错

---

## 54. Two parallel neural ectoderm progenitors contribute to the developing brain

**原文标题**: Two parallel neural ectoderm progenitors contribute to the developing brain

**原文链接**: [https://www.newscientist.com/article/2589739-our-brain-evolved-from-two-primitive-nervous-systems-that-merged/](https://www.newscientist.com/article/2589739-our-brain-evolved-from-two-primitive-nervous-systems-that-merged/)

生成摘要时出错

---

## 55. We made Playwright 2x faster and 80% more token efficient

**原文标题**: We made Playwright 2x faster and 80% more token efficient

**原文链接**: [https://github.com/browserbase/stagehand](https://github.com/browserbase/stagehand)

生成摘要时出错

---

## 56. Waymo in Singapore

**原文标题**: Waymo in Singapore

**原文链接**: [https://waymo.com/waymo-in-singapore/](https://waymo.com/waymo-in-singapore/)

生成摘要时出错

---

## 57. SDCC – Small Device C Compiler

**原文标题**: SDCC – Small Device C Compiler

**原文链接**: [https://sdcc.sourceforge.net/](https://sdcc.sourceforge.net/)

生成摘要时出错

---

## 58. A graphical desktop for the ZX Spectrum

**原文标题**: A graphical desktop for the ZX Spectrum

**原文链接**: [https://github.com/mindbox77/zxdesk](https://github.com/mindbox77/zxdesk)

生成摘要时出错

---

## 59. AI is an elite crime spree

**原文标题**: AI is an elite crime spree

**原文链接**: [https://www.thebignewsletter.com/p/ai-is-an-elite-crime-spree](https://www.thebignewsletter.com/p/ai-is-an-elite-crime-spree)

生成摘要时出错

---

## 60. AI chatbots are becoming experts at changing people's minds

**原文标题**: AI chatbots are becoming experts at changing people's minds

**原文链接**: [https://www.science.org/content/article/ai-chatbots-are-becoming-experts-changing-people-s-minds-what-s-their-secret](https://www.science.org/content/article/ai-chatbots-are-becoming-experts-changing-people-s-minds-what-s-their-secret)

生成摘要时出错

---

## 61. How Uber Protects Against Retry Storms

**原文标题**: How Uber Protects Against Retry Storms

**原文链接**: [https://www.uber.com/us/en/blog/protecting-against-retry-storms/](https://www.uber.com/us/en/blog/protecting-against-retry-storms/)

生成摘要时出错

---

## 62. Apple M6 Pro Achieves the Highest Single-Core CPU Score in Geekbench 7

**原文标题**: Apple M6 Pro Achieves the Highest Single-Core CPU Score in Geekbench 7

**原文链接**: [https://browser.geekbench.com/v7/cpu/389219](https://browser.geekbench.com/v7/cpu/389219)

生成摘要时出错

---

## 63. Show HN: Snapdrop: Instantly share files between devices. No setup, no signup

**原文标题**: Show HN: Snapdrop: Instantly share files between devices. No setup, no signup

**原文链接**: [https://snapdrop.me](https://snapdrop.me)

生成摘要时出错

---

## 64. Cache-to-Cache: Direct Semantic Communication Between LLMs (2025)

**原文标题**: Cache-to-Cache: Direct Semantic Communication Between LLMs (2025)

**原文链接**: [https://arxiv.org/abs/2510.03215](https://arxiv.org/abs/2510.03215)

生成摘要时出错

---

## 65. Shapelearn Qwen 3.8 27B (13.1 GB VRAM)

**原文标题**: Shapelearn Qwen 3.8 27B (13.1 GB VRAM)

**原文链接**: [https://byteshape.com/blogs/Qwen3.8-27B/](https://byteshape.com/blogs/Qwen3.8-27B/)

生成摘要时出错

---

## 66. Telstra outage: The night a network decided the year was 2006

**原文标题**: Telstra outage: The night a network decided the year was 2006

**原文链接**: [https://www.netnod.se/blog/telstra-outage-night-network-decided-year-was-2006](https://www.netnod.se/blog/telstra-outage-night-network-decided-year-was-2006)

生成摘要时出错

---

## 67. Show HN: Microsoft Office running with Wine on Linux with no virtualization

**原文标题**: Show HN: Microsoft Office running with Wine on Linux with no virtualization

**原文链接**: [https://github.com/Tombert/office365_flake](https://github.com/Tombert/office365_flake)

生成摘要时出错

---

## 68. Black Holes or Black Hole Stars? Astronomers Spar over 'Little Red Dots'

**原文标题**: Black Holes or Black Hole Stars? Astronomers Spar over 'Little Red Dots'

**原文链接**: [https://www.quantamagazine.org/black-holes-or-black-hole-stars-astronomers-spar-over-webb-telescopes-little-red-dots-20260914/](https://www.quantamagazine.org/black-holes-or-black-hole-stars-astronomers-spar-over-webb-telescopes-little-red-dots-20260914/)

生成摘要时出错

---

## 69. Mathematicians Build Long-Awaited Graph Sandwich

**原文标题**: Mathematicians Build Long-Awaited Graph Sandwich

**原文链接**: [https://www.quantamagazine.org/mathematicians-build-long-awaited-graph-sandwich-20260918/](https://www.quantamagazine.org/mathematicians-build-long-awaited-graph-sandwich-20260918/)

生成摘要时出错

---

## 70. Flock Offers Employees Buyouts as Customers Flee

**原文标题**: Flock Offers Employees Buyouts as Customers Flee

**原文链接**: [https://www.wired.com/story/flock-is-offering-voluntary-buyouts-to-employees/](https://www.wired.com/story/flock-is-offering-voluntary-buyouts-to-employees/)

生成摘要时出错

---

## 71. Pentagon weighs pulling nearly a third of U.S. forces from Europe

**原文标题**: Pentagon weighs pulling nearly a third of U.S. forces from Europe

**原文链接**: [https://www.nbcnews.com/politics/national-security/pentagon-weighs-pulling-nearly-third-us-forces-europe-rcna597722](https://www.nbcnews.com/politics/national-security/pentagon-weighs-pulling-nearly-third-us-forces-europe-rcna597722)

生成摘要时出错

---

## 72. The Implications of Linguistic Illegibility for LLM Security

**原文标题**: The Implications of Linguistic Illegibility for LLM Security

**原文链接**: [https://arxiv.org/abs/2609.02852](https://arxiv.org/abs/2609.02852)

生成摘要时出错

---

## 73. Gemini hacked three companies in first known breakout by Google's AI

**原文标题**: Gemini hacked three companies in first known breakout by Google's AI

**原文链接**: [https://www.reuters.com/business/gemini-hacked-three-companies-first-known-breakout-by-google-ai-wsj-reports-2026-09-18/](https://www.reuters.com/business/gemini-hacked-three-companies-first-known-breakout-by-google-ai-wsj-reports-2026-09-18/)

生成摘要时出错

---

## 74. Y Combinator's PAC is throwing money at Republicans across the country

**原文标题**: Y Combinator's PAC is throwing money at Republicans across the country

**原文链接**: [https://sf.gazetteer.co/y-combinators-pac-is-throwing-money-at-a-bunch-of-republicans-across-the-country](https://sf.gazetteer.co/y-combinators-pac-is-throwing-money-at-a-bunch-of-republicans-across-the-country)

生成摘要时出错

---

## 75. Btrfs/ZFS/bcachefs under workloads classic benchmarks skip

**原文标题**: Btrfs/ZFS/bcachefs under workloads classic benchmarks skip

**原文链接**: [https://bartosz.fenski.pl/modern-fs-benchmark/](https://bartosz.fenski.pl/modern-fs-benchmark/)

生成摘要时出错

---

## 76. How did AMD Ryzen get 50% faster in two years?

**原文标题**: How did AMD Ryzen get 50% faster in two years?

**原文链接**: [https://lemire.me/blog/2026/09/18/how-did-amd-ryzen-get-50-faster-in-two-years/](https://lemire.me/blog/2026/09/18/how-did-amd-ryzen-get-50-faster-in-two-years/)

生成摘要时出错

---

## 77. New wild cat species discovered – with only one known living member

**原文标题**: New wild cat species discovered – with only one known living member

**原文链接**: [https://www.bbc.com/news/articles/c6x2zgv9rr4ro](https://www.bbc.com/news/articles/c6x2zgv9rr4ro)

生成摘要时出错

---

## 78. Brood War Bench

**原文标题**: Brood War Bench

**原文链接**: [https://bw.swerdlow.dev/report](https://bw.swerdlow.dev/report)

生成摘要时出错

---

## 79. AI Safety Is Mostly a Sex Cult

**原文标题**: AI Safety Is Mostly a Sex Cult

**原文链接**: [https://bsky.app/profile/segyges.bsky.social/post/3mvom4b4dn22q](https://bsky.app/profile/segyges.bsky.social/post/3mvom4b4dn22q)

生成摘要时出错

---

## 80. Learning Another Language May Be One of the Best Ways to Keep Your Brain Healthy

**原文标题**: Learning Another Language May Be One of the Best Ways to Keep Your Brain Healthy

**原文链接**: [https://theconversation.com/learning-another-language-may-be-one-of-the-best-ways-to-keep-your-brain-healthy-as-you-age-291951](https://theconversation.com/learning-another-language-may-be-one-of-the-best-ways-to-keep-your-brain-healthy-as-you-age-291951)

生成摘要时出错

---

## 81. Ask A Monk – A digital wilderness for thoughts with no immediate answer

**原文标题**: Ask A Monk – A digital wilderness for thoughts with no immediate answer

**原文链接**: [https://askamonk.online](https://askamonk.online)

生成摘要时出错

---

## 82. Show HN: Scry, programmable internet search w/ congestion pricing

**原文标题**: Show HN: Scry, programmable internet search w/ congestion pricing

**原文链接**: [https://scry.io/](https://scry.io/)

生成摘要时出错

---

## 83. War may be coming. Are we psychologically ready?

**原文标题**: War may be coming. Are we psychologically ready?

**原文链接**: [https://www.bbc.com/news/articles/cmn0jke547r5o](https://www.bbc.com/news/articles/cmn0jke547r5o)

生成摘要时出错

---

## 84. NATS publishes preliminary report on technical incident of 8 September

**原文标题**: NATS publishes preliminary report on technical incident of 8 September

**原文链接**: [https://www.nats.aero/news/nats-publishes-preliminary-report-on-technical-incident-of-8-september/](https://www.nats.aero/news/nats-publishes-preliminary-report-on-technical-incident-of-8-september/)

生成摘要时出错

---

## 85. DraftKings Uses A.I. To Target the Gamblers Likeliest to Lose

**原文标题**: DraftKings Uses A.I. To Target the Gamblers Likeliest to Lose

**原文链接**: [https://www.nytimes.com/2026/09/19/business/draftkings-ai.html](https://www.nytimes.com/2026/09/19/business/draftkings-ai.html)

生成摘要时出错

---

## 86. Goose Programming Language

**原文标题**: Goose Programming Language

**原文链接**: [https://github.com/aardappel/goose/tree/master](https://github.com/aardappel/goose/tree/master)

生成摘要时出错

---

## 87. AI Protest in Montreal

**原文标题**: AI Protest in Montreal

**原文链接**: [https://montrealgazette.com/news/photos-anti-ai-protest-in-montreal/](https://montrealgazette.com/news/photos-anti-ai-protest-in-montreal/)

生成摘要时出错

---

## 88. Google illegally retains customer data,and I am taking legal action against them

**原文标题**: Google illegally retains customer data,and I am taking legal action against them

**原文链接**: [https://medium.com/@istokovicsgyorgy79/google-illegally-retains-customer-data-and-i-am-taking-legal-action-against-them-7da0cf95941c](https://medium.com/@istokovicsgyorgy79/google-illegally-retains-customer-data-and-i-am-taking-legal-action-against-them-7da0cf95941c)

生成摘要时出错

---

## 89. Anthropic finally adds AGENTS.md support to Claude Code

**原文标题**: Anthropic finally adds AGENTS.md support to Claude Code

**原文链接**: [https://twitter.com/trq212/status/2101009392611278961](https://twitter.com/trq212/status/2101009392611278961)

生成摘要时出错

---

## 90. Republican bill would order ISPs, DNS providers, and VPNs to block piracy sites

**原文标题**: Republican bill would order ISPs, DNS providers, and VPNs to block piracy sites

**原文链接**: [https://arstechnica.com/tech-policy/2026/09/republican-bill-would-order-isps-dns-providers-and-vpns-to-block-piracy-sites/](https://arstechnica.com/tech-policy/2026/09/republican-bill-would-order-isps-dns-providers-and-vpns-to-block-piracy-sites/)

生成摘要时出错

---

## 91. U.S. Strike on Iranian School May Have Been War Crime, U.N. Report Says

**原文标题**: U.S. Strike on Iranian School May Have Been War Crime, U.N. Report Says

**原文链接**: [https://www.nytimes.com/2026/09/17/world/asia/us-iran-school-strike-report.html](https://www.nytimes.com/2026/09/17/world/asia/us-iran-school-strike-report.html)

生成摘要时出错

---

## 92. NASA-IBM Lunar Foundation open-Source Geospatial AI Model

**原文标题**: NASA-IBM Lunar Foundation open-Source Geospatial AI Model

**原文链接**: [https://newsroom.usra.edu/usra-contributes-planetary-science-expertise-to-nasa-ibm-lunar-foundation-model/](https://newsroom.usra.edu/usra-contributes-planetary-science-expertise-to-nasa-ibm-lunar-foundation-model/)

生成摘要时出错

---

## 93. Microsoft director: AI scraping 'the largest theft of labor in human history'

**原文标题**: Microsoft director: AI scraping 'the largest theft of labor in human history'

**原文链接**: [https://www.tomshardware.com/tech-industry/artificial-intelligence/microsoft-director-called-ai-scraping-the-largest-theft-of-labor-in-human-history-while-openai-head-brands-chatgpt-an-existential-threat-to-publishers-revelations-come-from-legal-briefs-filed-in-nyt-lawsuit](https://www.tomshardware.com/tech-industry/artificial-intelligence/microsoft-director-called-ai-scraping-the-largest-theft-of-labor-in-human-history-while-openai-head-brands-chatgpt-an-existential-threat-to-publishers-revelations-come-from-legal-briefs-filed-in-nyt-lawsuit)

生成摘要时出错

---

## 94. DJ Shadow looks back at "Entroducing" and other early work

**原文标题**: DJ Shadow looks back at "Entroducing" and other early work

**原文链接**: [https://www.msn.com/en-us/news/other/dj-shadow-spent-decades-digging-for-records-now-hes-digging-through-his-own-past/ar-AA2cuuKt](https://www.msn.com/en-us/news/other/dj-shadow-spent-decades-digging-for-records-now-hes-digging-through-his-own-past/ar-AA2cuuKt)

生成摘要时出错

---

## 95. Dear Customer, Fuck You

**原文标题**: Dear Customer, Fuck You

**原文链接**: [https://fuck-off.ai](https://fuck-off.ai)

生成摘要时出错

---

## 96. The US 'Kill Chain' That Destroyed an Iranian School

**原文标题**: The US 'Kill Chain' That Destroyed an Iranian School

**原文链接**: [https://www.bloomberg.com/graphics/2026-iran-school-attack](https://www.bloomberg.com/graphics/2026-iran-school-attack)

生成摘要时出错

---

## 97. Gemini Hacked Three Companies in First Known Breakout by Google's AI

**原文标题**: Gemini Hacked Three Companies in First Known Breakout by Google's AI

**原文链接**: [https://www.wsj.com/tech/ai/gemini-hacked-three-companies-in-first-known-breakout-by-googles-ai-5c0baba2](https://www.wsj.com/tech/ai/gemini-hacked-three-companies-in-first-known-breakout-by-googles-ai-5c0baba2)

生成摘要时出错

---

## 98. I built the fastest PHP webserver in the world

**原文标题**: I built the fastest PHP webserver in the world

**原文链接**: [https://qbixserver.com](https://qbixserver.com)

生成摘要时出错

---

## 99. Show HN: LiveWorld – Every 24/7 YouTube live camera on one globe

**原文标题**: Show HN: LiveWorld – Every 24/7 YouTube live camera on one globe

**原文链接**: [https://liveworld.info/](https://liveworld.info/)

生成摘要时出错

---

## 100. Prepare your iPhone 18 Pro Max to ship

**原文标题**: Prepare your iPhone 18 Pro Max to ship

**原文链接**: [https://support.apple.com/en-us/127848](https://support.apple.com/en-us/127848)

生成摘要时出错

---

