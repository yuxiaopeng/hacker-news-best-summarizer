# Hacker News 热门文章摘要 (2026-07-26)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 安卓可能很快会限制本机ADB

**原文标题**: Android may soon restrict on-device ADB

**原文链接**: [https://kitsumed.github.io/blog/posts/android-may-soon-restrict-on-device-adb/](https://kitsumed.github.io/blog/posts/android-may-soon-restrict-on-device-adb/)

Google IssueTracker 上的一场持续讨论表明，Google 可能会限制设备上的 ADB 连接，这一举动已被 Shizuku 相关应用的开发者 Kitsumed 指出。ADB（安卓调试桥）是一款功能强大的开发者工具，能够授予高权限，传统上通过 USB、TCP/IP 或无线调试进行连接。

“设备上 ADB”是指通过回环地址 (127.0.0.1) 在同一设备上运行 ADB 客户端和服务器。这种设置支持了一个小众但重要的开发者和高级用户工具生态系统，例如 Shizuku，它能够为残障用户提供通话录音等功能。

这项由一个安全漏洞 (CVE-2026-0073) 引发的拟议更改，建议将 ADB 守护进程 (ADBD) 限制为仅绑定到 Wi-Fi 接口 (`wlan0`)。一位 Google 维护者解释说，此举是出于对恶意应用利用本地主机套接字进行权限提升的担忧。

Kitsumed 认为，这种全面限制是过度且不必要的。他解释说，“恶意行为者”无法单方面利用设备上 ADB；它需要用户进行多项明确的手动操作，例如启用 USB 调试、无线 ADB 配对或授权 TCP/IP 连接。他强调了设备上 ADB 对于无法使用电脑的开发者以及各种重要的，高级用户工具来说，存在诸多合法用途。

作者倡导一种平衡的方法：默认限制设备上 ADB，但在用户知晓相关风险后，允许他们通过持久设置禁用此限制。他认为彻底锁定是没有必要的，这类似于因潜在滥用而移除其他强大的安卓功能（如辅助功能服务），并鼓励技术用户在 Google IssueTracker 上提供建设性反馈。

---

## 2. 干掉Cookie横幅

**原文标题**: Kill The Cookie Banner

**原文链接**: [https://killthecookiebanner.eu/](https://killthecookiebanner.eu/)

文章呼吁#废除Cookie横幅，认为这些普遍存在的横幅旨在诱骗用户同意在线追踪，尽管欧盟法律默认禁止此类行为。文章指出，误导性横幅导致高达90%的同意率，而实际上只有大约3%的用户真正希望被追踪。

欧盟委员会为2025年秋季提出的解决方案涉及自动化隐私信号。用户只需在浏览器中一次性设置其追踪偏好（接受、拒绝、限制），浏览器随后便会将这些偏好传达给网站和应用程序。这种简单且现有的技术已在美国某些州获得法律支持。

然而，追踪行业，尤其是谷歌，正在极力游说反对这项提案。它们担心一旦用户可以轻松表达其偏好，同意率将会下降，因此已成功影响了多个成员国阻止这项倡议，并正在向欧洲议会施压，要求其否决该提案。

文章敦促公众采取行动，因为这项决定尚未最终确定。鼓励读者联系他们在欧洲议会或国家政府的代表，以表达他们的不满，并支持自动化隐私信号提案。文章澄清，虽然支持这项具体的提案，但对更广泛的“数字综合法案”法律改革的其他部分不予支持，因为担心这会削弱民众的权利。这项倡议由欧洲各地的公民社会组织牵头。

---

## 3. 汉娜·弗莱荣获2026年莱拉瓦蒂奖，表彰其数学普及贡献

**原文标题**: Hannah Fry Wins the Leelavati Prize in 2026 for Mathematics Outreach

**原文链接**: [https://www.maths.cam.ac.uk/features/professor-hannah-fry-wins-leelavati-prize](https://www.maths.cam.ac.uk/features/professor-hannah-fry-wins-leelavati-prize)

汉娜·弗莱教授在国际数学家大会（ICM）上荣获国际数学联盟（IMU）于2026年颁发的莱拉瓦蒂奖，以表彰她在提高公众对数学认知方面所做的杰出贡献。弗莱于2025年1月成为剑桥大学首位“公众理解数学”教授，她是一位著名的播音员、作家、播客主持人以及社交媒体明星。

颁奖词称赞她为“数学思维最重要的全球大使”，其工作超越了传统的科学传播。她通过多种媒体，以非凡的创造力将数学转化为“充满奇迹和实用性的语言”，同时不减损其深度和广度。弗莱解释了她分享数学“绝对乐趣”和“奇妙秘密”的热情，她认为自己的角色是通过“开启人们的想象空间”来提供动力。

弗莱获得的广泛认可包括克里斯托弗·齐曼奖章（2018年）、皇家学会戴维·阿滕伯勒奖（2024年）、凭借《与汉娜·弗莱共创未来》获得的艾美奖（2025年），以及凭借《科学万象》获得的威比奖（2026年）。她于2026年被《时代》杂志评为全球100位最具影响力的数字创作者之一，其Instagram粉丝超过200万。她还通过皇家学会圣诞讲座等活动激励未来的数学家。DAMTP系主任尼克·多利教授称赞她是现代生活中数学重要性传播方面最重要的贡献者之一。

---

## 4. 他们对你玩消失了吗？

**原文标题**: Did they ghost you?

**原文链接**: [https://didtheyghostyou.com/](https://didtheyghostyou.com/)

这份题为“你被‘放鸽子’了吗？”的文本传递了一个直接的信息：如果你在面试后经历公司对你“放鸽子”，你应该举报他们。核心建议是，对那些在面试后不予回应的雇主采取行动。

---

## 5. Claude 5 生成模型的上下文工程新规

**原文标题**: The new rules of context engineering for Claude 5 generation models

**原文链接**: [https://claude.com/blog/the-new-rules-of-context-engineering-for-claude-5-generation-models](https://claude.com/blog/the-new-rules-of-context-engineering-for-claude-5-generation-models)

本文概述了针对Claude 5代模型（例如Opus 5、Fable 5）的“上下文工程新规则”，强调了从过度约束模型转向利用其增强的判断力和能力的重大转变。Anthropic移除了Claude Code系统提示中80%以上的内容，且性能没有下降，这表明旧方法对于高级模型而言适得其反。

最佳实践的关键变化包括：

*   **从明确规则到允许Claude判断：** 不再使用严格的指令（例如，“无注释”），而是引导Claude匹配周围代码的风格。
*   **从工具示例到设计富有表现力的接口：** 侧重于精心设计的参数，而非具体的用法示例，后者可能会限制探索。
*   **从预先提供上下文到渐进式披露：** 仅在需要时加载技能、工具和`CLAUDE.md`内容，避免不必要的上下文。
*   **从重复指令到简单的工具描述：** 将指令放置在工具描述中，而非在系统提示中重复。
*   **从手动`CLAUDE.md`记忆到自动记忆：** Claude现在自动保存相关记忆。
*   **从简单规范到丰富参考：** 利用详细的测试、函数、HTML工件或评分标准作为高保真参考，优先选择基于代码的格式。

对用户而言，这意味着保持`CLAUDE.md`轻量化并专注于代码库中的“陷阱”，使用技能作为特定知识的定向指南，并提供丰富、上下文相关的参考。`claude doctor`命令有助于简化现有上下文。核心原则是，通过信任Claude的高级智能并提供动态、简洁的指导来“解放”它。

---

## 6. 开放权重AI正迎来其Kubernetes般的时刻。

**原文标题**: Open-weight AI is having its Kubernetes moment

**原文链接**: [https://tobi.knaup.me/2026-07-25-open-weight-ai-is-having-its-kubernetes-moment/](https://tobi.knaup.me/2026-07-25-open-weight-ai-is-having-its-kubernetes-moment/)

无法访问文章链接。

---

## 7. Opus 5 is currently #1 on Artificial Analysis Intelligence Leaderboard

**原文标题**: Opus 5 is currently #1 on Artificial Analysis Intelligence Leaderboard

**原文链接**: [https://artificialanalysis.ai/models](https://artificialanalysis.ai/models)

The "Artificial Analysis Intelligence Leaderboard" offers a comprehensive comparison of AI models across key performance metrics. **Claude Opus 5 (max) and Claude Opus 5 (xhigh) are currently ranked #1 for intelligence**, closely followed by Claude Fable 5 and GPT-5.6 Sol (max).

The platform evaluates models across several critical dimensions:
*   **Intelligence:** Measured by the Artificial Analysis Intelligence Index v4.1, which synthesizes results from 9 evaluations including agentic tasks (GDPval-AA v2, 𝜏³-Banking, Terminal-Bench v2.1), coding (SciCode), reasoning (Humanity's Last Exam, GPQA Diamond, CritPt), knowledge (AA-Omniscience), and long context reasoning (AA-LCR).
*   **Output Speed:** Mercury 2 (953 tokens/s) and Gemini 3.5 Flash-Lite (417 tokens/s) are the fastest.
*   **Latency:** Gemini 2.5 Flash-Lite (0.35s) and Command A+ (0.39s) exhibit the lowest latency.
*   **Price:** Devstral 2 and North Mini Code are the most cost-effective at $0.00 per M tokens.
*   **Context Window:** Llama 4 Scout (10M tokens) and Grok 4.20 0309 (2M tokens) offer the largest context windows.

The analysis also provides breakdowns of intelligence evaluations, model openness, and detailed cost metrics, including cost per task, total cost, and token pricing for input, output, reasoning, and caching. Comparative charts show relationships such as Intelligence vs. Cost, Speed, and Time per Task. Performance figures represent first-party API data or the median across providers.

---

## 8. A shell colon does nothing. Use it anyway

**原文标题**: A shell colon does nothing. Use it anyway

**原文链接**: [https://refp.se/articles/your-shell-and-the-magic-colon](https://refp.se/articles/your-shell-and-the-magic-colon)

生成摘要时出错

---

## 9. GrapheneOS protections against data extraction from locked devices

**原文标题**: GrapheneOS protections against data extraction from locked devices

**原文链接**: [https://discuss.grapheneos.org/d/40700-grapheneos-protections-against-data-extraction-from-locked-devices](https://discuss.grapheneos.org/d/40700-grapheneos-protections-against-data-extraction-from-locked-devices)

GrapheneOS provides robust defenses against data extraction from locked devices, building upon Android's security features and Pixel hardware. Its core protections include strong disk encryption, which requires exploiting the OS or brute-forcing the PIN/password.

A key feature is its advanced secure element (SE), implementing strict rate limiting compliant with Android 16 QPR2 standards. This allows only 20 attempts, with escalating delays (e.g., 4 hours after 10 attempts, 41 days after 15), and resists insider attacks by requiring owner authentication for firmware updates. This SE capability has been present in Pixels since the Pixel 2.

GrapheneOS enhances authentication by raising password limits to 128 characters for high-entropy passphrases. It introduces an optional 2nd factor fingerprint PIN, reducing fingerprint attempts to 5 and requiring a PIN to unlock the hardware keystore.

For exploit protection, GrapheneOS hardens the OS with memory allocators and hardware memory tagging (MTE). Physical attack defenses include blocking new USB connections and disabling USB data while locked.

GrapheneOS pioneered a locked device auto-reboot timer (default 18 hours), which returns the device to Before First Unlock (BFU) state with memory zeroing, a feature later adopted by Apple and Google. It also enables secondary users and Private Spaces to return to BFU without a full reboot.

Finally, a duress PIN/password feature allows wiping the device if entered in any authentication prompt across all profiles, providing a critical failsafe against forced data recovery, though it is not the primary defense mechanism.

---

## 10. Taylor Farms Called White House to Try to Delay Cyclospora Recall

**原文标题**: Taylor Farms Called White House to Try to Delay Cyclospora Recall

**原文链接**: [https://www.wsj.com/health/taylor-farms-cyclospora-recall-delay-call-41fef0bc](https://www.wsj.com/health/taylor-farms-cyclospora-recall-delay-call-41fef0bc)

Unable to access the article link.

---

## 11. Ruff v0.16.0 – Significant new updates – 413 default rules up from 59

**原文标题**: Ruff v0.16.0 – Significant new updates – 413 default rules up from 59

**原文链接**: [https://astral.sh/blog/ruff-v0.16.0](https://astral.sh/blog/ruff-v0.16.0)

生成摘要时出错

---

## 12. Google Discloses $94.1B in SpaceX Stock, Marking 6% Stake

**原文标题**: Google Discloses $94.1B in SpaceX Stock, Marking 6% Stake

**原文链接**: [https://www.wsj.com/tech/google-discloses-94-1-billion-in-spacex-stock-marking-6-stake-91655d7c](https://www.wsj.com/tech/google-discloses-94-1-billion-in-spacex-stock-marking-6-stake-91655d7c)

Unable to access the article link.

---

## 13. Running a 28.9M parameter LLM on an $8 microcontroller

**原文标题**: Running a 28.9M parameter LLM on an $8 microcontroller

**原文链接**: [https://github.com/slvDev/esp32-ai](https://github.com/slvDev/esp32-ai)

生成摘要时出错

---

## 14. The growing vigilante movement to knock out Flock surveillance cameras

**原文标题**: The growing vigilante movement to knock out Flock surveillance cameras

**原文链接**: [https://www.theguardian.com/us-news/ng-interactive/2026/jul/25/flock-surveillance-cameras](https://www.theguardian.com/us-news/ng-interactive/2026/jul/25/flock-surveillance-cameras)

生成摘要时出错

---

## 15. An ESP32 based plane radar for my desk

**原文标题**: An ESP32 based plane radar for my desk

**原文链接**: [https://blog.ktz.me/esp32-plane-radar/](https://blog.ktz.me/esp32-plane-radar/)

生成摘要时出错

---

## 16. Bitchat is now on Radicle

**原文标题**: Bitchat is now on Radicle

**原文链接**: [https://radicle.network/nodes/rosa.radicle.network/rad%3Az2v9tRJz1oknFAqCSY5W5c76nVvm6](https://radicle.network/nodes/rosa.radicle.network/rad%3Az2v9tRJz1oknFAqCSY5W5c76nVvm6)

生成摘要时出错

---

## 17. JetZero

**原文标题**: JetZero

**原文链接**: [https://www.jetzero.aero](https://www.jetzero.aero)

生成摘要时出错

---

## 18. London Gatwick has launched a robotic airport parking service

**原文标题**: London Gatwick has launched a robotic airport parking service

**原文链接**: [https://aerospaceglobalnews.com/news/gatwick-airport-robotic-parking-stanley-robotics/](https://aerospaceglobalnews.com/news/gatwick-airport-robotic-parking-stanley-robotics/)

生成摘要时出错

---

## 19. DeepSeek pause fundraise after comments on compute gap to US leaked (transcript) [pdf]

**原文标题**: DeepSeek pause fundraise after comments on compute gap to US leaked (transcript) [pdf]

**原文链接**: [https://github.com/demo-zexuan/liang-wenfeng-investor-meeting-2026-7-22/blob/master/%E6%A2%81%E6%96%87%E9%94%8B%E6%8A%95%E8%B5%84%E8%80%85%E4%BA%A4%E6%B5%81%E4%BC%9A-%E6%96%87%E5%AD%97%E7%A8%BF_1_18_translate_20260723201651.pdf](https://github.com/demo-zexuan/liang-wenfeng-investor-meeting-2026-7-22/blob/master/%E6%A2%81%E6%96%87%E9%94%8B%E6%8A%95%E8%B5%84%E8%80%85%E4%BA%A4%E6%B5%81%E4%BC%9A-%E6%96%87%E5%AD%97%E7%A8%BF_1_18_translate_20260723201651.pdf)

生成摘要时出错

---

## 20. What is happening to jobs? Separating AI hype from reality

**原文标题**: What is happening to jobs? Separating AI hype from reality

**原文链接**: [https://siepr.stanford.edu/publications/policy-brief/what-really-happening-jobs-separating-ai-hype-reality](https://siepr.stanford.edu/publications/policy-brief/what-really-happening-jobs-separating-ai-hype-reality)

生成摘要时出错

---

## 21. Show HN: Brolly, a plain-text weather forecast site

**原文标题**: Show HN: Brolly, a plain-text weather forecast site

**原文链接**: [https://brolly.sh/forecast/RWFP2qW8](https://brolly.sh/forecast/RWFP2qW8)

生成摘要时出错

---

## 22. Turn And Face The Strange

**原文标题**: Turn And Face The Strange

**原文链接**: [https://fly.io/blog/kurt-scott-money-sprites/](https://fly.io/blog/kurt-scott-money-sprites/)

生成摘要时出错

---

## 23. The Dark Night of Mathematics

**原文标题**: The Dark Night of Mathematics

**原文链接**: [https://kirwinhampshire.substack.com/p/the-dark-night-of-mathematics](https://kirwinhampshire.substack.com/p/the-dark-night-of-mathematics)

生成摘要时出错

---

## 24. Htmx 4.0, the first JavaScript library to release exclusively on the Game Boy

**原文标题**: Htmx 4.0, the first JavaScript library to release exclusively on the Game Boy

**原文链接**: [https://swag.htmx.org/en-cad/products/htmx-4-the-game](https://swag.htmx.org/en-cad/products/htmx-4-the-game)

生成摘要时出错

---

## 25. Third Drone Shot Down in Three Days in Romanian Territory

**原文标题**: Third Drone Shot Down in Three Days in Romanian Territory

**原文链接**: [https://english.mapn.ro/](https://english.mapn.ro/)

生成摘要时出错

---

## 26. LLM Usage in Debian: Three Proposals

**原文标题**: LLM Usage in Debian: Three Proposals

**原文链接**: [https://www.debian.org/vote/2026/vote_002](https://www.debian.org/vote/2026/vote_002)

生成摘要时出错

---

## 27. Show HN: I mapped every US golf course

**原文标题**: Show HN: I mapped every US golf course

**原文链接**: [https://golfcoursebrowser.com/](https://golfcoursebrowser.com/)

生成摘要时出错

---

## 28. GM Backs Sodium Ion Batteries for U.S. Grid Storage

**原文标题**: GM Backs Sodium Ion Batteries for U.S. Grid Storage

**原文链接**: [https://spectrum.ieee.org/sodium-ion-battery-peak-energy](https://spectrum.ieee.org/sodium-ion-battery-peak-energy)

生成摘要时出错

---

## 29. Inflect-Micro-v2: complete voice in 9.36M parameters

**原文标题**: Inflect-Micro-v2: complete voice in 9.36M parameters

**原文链接**: [https://huggingface.co/owensong/Inflect-Micro-v2](https://huggingface.co/owensong/Inflect-Micro-v2)

生成摘要时出错

---

## 30. MouthPad: A Tongue-Controlled Touchpad

**原文标题**: MouthPad: A Tongue-Controlled Touchpad

**原文链接**: [https://www.augmental.tech/](https://www.augmental.tech/)

生成摘要时出错

---

## 31. Cloudflare's new AI traffic options for customers

**原文标题**: Cloudflare's new AI traffic options for customers

**原文链接**: [https://blog.cloudflare.com/content-independence-day-ai-options/](https://blog.cloudflare.com/content-independence-day-ai-options/)

生成摘要时出错

---

## 32. ARC-AGI Leaderboard

**原文标题**: ARC-AGI Leaderboard

**原文链接**: [https://arcprize.org/leaderboard](https://arcprize.org/leaderboard)

生成摘要时出错

---

## 33. Tile's security is so bad it's a feature for stalkers

**原文标题**: Tile's security is so bad it's a feature for stalkers

**原文链接**: [https://blog.adafruit.com/2026/03/05/tiles-security-is-so-bad-its-a-feature-for-stalkers/](https://blog.adafruit.com/2026/03/05/tiles-security-is-so-bad-its-a-feature-for-stalkers/)

生成摘要时出错

---

## 34. Alien World Chemistry Found Inside Meteorite That Struck New Jersey Home

**原文标题**: Alien World Chemistry Found Inside Meteorite That Struck New Jersey Home

**原文链接**: [https://www.seti.org/news/alien-world-chemistry-found-inside-meteorite/](https://www.seti.org/news/alien-world-chemistry-found-inside-meteorite/)

生成摘要时出错

---

## 35. A 77-year-old Republican man is staging a solo protest against Flock cameras

**原文标题**: A 77-year-old Republican man is staging a solo protest against Flock cameras

**原文链接**: [https://www.cltampa.com/news/a-77-year-old-republican-man-is-staging-a-solo-protest-against-st-petes-flock-cameras/](https://www.cltampa.com/news/a-77-year-old-republican-man-is-staging-a-solo-protest-against-st-petes-flock-cameras/)

生成摘要时出错

---

## 36. The Fedora 45 Sausage Factory

**原文标题**: The Fedora 45 Sausage Factory

**原文链接**: [https://supakeen.com/weblog/the-fedora-45-sausage-factory/](https://supakeen.com/weblog/the-fedora-45-sausage-factory/)

生成摘要时出错

---

## 37. Go Analysis Framework: modular static analysis by go team

**原文标题**: Go Analysis Framework: modular static analysis by go team

**原文链接**: [https://pkg.go.dev/golang.org/x/tools/go/analysis](https://pkg.go.dev/golang.org/x/tools/go/analysis)

生成摘要时出错

---

## 38. Engineering management after the cost of code collapsed

**原文标题**: Engineering management after the cost of code collapsed

**原文链接**: [https://karimjedda.com/engineering-management-after-cost-of-code-collapse/](https://karimjedda.com/engineering-management-after-cost-of-code-collapse/)

生成摘要时出错

---

## 39. Producing ammonia and fertiliser using wind power in Morris, Minnesota

**原文标题**: Producing ammonia and fertiliser using wind power in Morris, Minnesota

**原文链接**: [https://ammoniaenergy.org/articles/flexible-renewable-ammonia-demonstrator-now-operational-in-minnesota/](https://ammoniaenergy.org/articles/flexible-renewable-ammonia-demonstrator-now-operational-in-minnesota/)

生成摘要时出错

---

## 40. Clinical failure rates over the decades: yikes

**原文标题**: Clinical failure rates over the decades: yikes

**原文链接**: [https://www.science.org/content/blog-post/clinical-failure-rates-over-decades-yikes](https://www.science.org/content/blog-post/clinical-failure-rates-over-decades-yikes)

生成摘要时出错

---

## 41. UK AISI / Caisi Preliminary Assessment of Kimi K3's Cyber Capabilities

**原文标题**: UK AISI / Caisi Preliminary Assessment of Kimi K3's Cyber Capabilities

**原文链接**: [https://www.nist.gov/news-events/news/2026/07/uk-aisi-caisi-preliminary-assessment-kimi-k3s-cyber-capabilities](https://www.nist.gov/news-events/news/2026/07/uk-aisi-caisi-preliminary-assessment-kimi-k3s-cyber-capabilities)

生成摘要时出错

---

## 42. Memory safety absolutists

**原文标题**: Memory safety absolutists

**原文链接**: [https://itsallaboutthebit.com/memory-safety-absolutists/](https://itsallaboutthebit.com/memory-safety-absolutists/)

生成摘要时出错

---

## 43. Extinct Media Museum Tokyo

**原文标题**: Extinct Media Museum Tokyo

**原文链接**: [https://extinct-media-museum.blog.jp/otemachi/](https://extinct-media-museum.blog.jp/otemachi/)

生成摘要时出错

---

## 44. The Strongest El Niño Ever

**原文标题**: The Strongest El Niño Ever

**原文链接**: [https://www.theclimatebrink.com/p/the-strongest-el-nino-ever](https://www.theclimatebrink.com/p/the-strongest-el-nino-ever)

生成摘要时出错

---

## 45. SpaceX Starship Flight 13 livestream [video]

**原文标题**: SpaceX Starship Flight 13 livestream [video]

**原文链接**: [https://www.spacex.com/launches/starship-flight-13](https://www.spacex.com/launches/starship-flight-13)

生成摘要时出错

---

## 46. Sperm Whales blow bubbles to achieve restful, vertical sleep

**原文标题**: Sperm Whales blow bubbles to achieve restful, vertical sleep

**原文链接**: [https://news.st-andrews.ac.uk/archive/sperm-whales-blow-bubbles-to-achieve-restful-vertical-sleep/](https://news.st-andrews.ac.uk/archive/sperm-whales-blow-bubbles-to-achieve-restful-vertical-sleep/)

生成摘要时出错

---

## 47. Design is compromise

**原文标题**: Design is compromise

**原文链接**: [https://stephango.com/design-is-compromise](https://stephango.com/design-is-compromise)

生成摘要时出错

---

## 48. Git rebase -i is not that scary

**原文标题**: Git rebase -i is not that scary

**原文链接**: [https://cachebag.sh/journal/interactive-rebasing/](https://cachebag.sh/journal/interactive-rebasing/)

生成摘要时出错

---

## 49. The relay market powering token resellers and fraud

**原文标题**: The relay market powering token resellers and fraud

**原文链接**: [https://vectoral.com/blog/token-relay-market](https://vectoral.com/blog/token-relay-market)

生成摘要时出错

---

## 50. Elevated Errors for Opus 5

**原文标题**: Elevated Errors for Opus 5

**原文链接**: [https://status.claude.com/incidents/zftg3gqkmv18](https://status.claude.com/incidents/zftg3gqkmv18)

生成摘要时出错

---

## 51. Prosecutor Investigating U.S. Boat Strikes Was Murdered in Ecuador

**原文标题**: Prosecutor Investigating U.S. Boat Strikes Was Murdered in Ecuador

**原文链接**: [https://www.dropsitenews.com/p/prosecutor-investigating-ecuador-boat-strikes-murdered](https://www.dropsitenews.com/p/prosecutor-investigating-ecuador-boat-strikes-murdered)

生成摘要时出错

---

## 52. AIs don't do what you want. This is bad

**原文标题**: AIs don't do what you want. This is bad

**原文链接**: [https://rewardhacking.org](https://rewardhacking.org)

生成摘要时出错

---

## 53. Wind turbine is being used to produce zero-carbon "green ammonia" fertilizer

**原文标题**: Wind turbine is being used to produce zero-carbon "green ammonia" fertilizer

**原文链接**: [https://energiesmedia.com/wind-turbine-stopped-electricity-wind-water-air/](https://energiesmedia.com/wind-turbine-stopped-electricity-wind-water-air/)

生成摘要时出错

---

## 54. Show HN: Reverse Minesweeper

**原文标题**: Show HN: Reverse Minesweeper

**原文链接**: [https://sunflowersgame.com/](https://sunflowersgame.com/)

生成摘要时出错

---

## 55. What if we made advertising illegal?

**原文标题**: What if we made advertising illegal?

**原文链接**: [https://simone.org/advertising/](https://simone.org/advertising/)

生成摘要时出错

---

## 56. Bringing PyTorch Monarch to AMD GPUs

**原文标题**: Bringing PyTorch Monarch to AMD GPUs

**原文链接**: [https://pytorch.org/blog/bringing-pytorch-monarch-to-amd-gpus-single-controller-distributed-training-on-rocm/](https://pytorch.org/blog/bringing-pytorch-monarch-to-amd-gpus-single-controller-distributed-training-on-rocm/)

生成摘要时出错

---

## 57. The New AI Superpowers: Focus and Followthrough

**原文标题**: The New AI Superpowers: Focus and Followthrough

**原文链接**: [https://www.rickmanelius.com/p/the-new-ai-superpowers-focus-and](https://www.rickmanelius.com/p/the-new-ai-superpowers-focus-and)

生成摘要时出错

---

## 58. Humans haven't stopped evolving

**原文标题**: Humans haven't stopped evolving

**原文链接**: [https://www.harvardmagazine.com/research/harvard-human-evolution-genes-selective-pressure](https://www.harvardmagazine.com/research/harvard-human-evolution-genes-selective-pressure)

生成摘要时出错

---

## 59. Systems and Delays

**原文标题**: Systems and Delays

**原文链接**: [https://martin.janiczek.cz/2026/07/24/systems-and-delays.html](https://martin.janiczek.cz/2026/07/24/systems-and-delays.html)

生成摘要时出错

---

## 60. Terence Tao: Mathematics in the Age of AI [pdf]

**原文标题**: Terence Tao: Mathematics in the Age of AI [pdf]

**原文链接**: [https://teorth.github.io/tao-web/slides/age-of-ai-icm-2026.pdf](https://teorth.github.io/tao-web/slides/age-of-ai-icm-2026.pdf)

生成摘要时出错

---

## 61. Show HN: Bribes.fyi – Know before you go. New feature added

**原文标题**: Show HN: Bribes.fyi – Know before you go. New feature added

**原文链接**: [https://bribes.fyi/before-you-go](https://bribes.fyi/before-you-go)

生成摘要时出错

---

## 62. The Silurian Hypothesis (2020)

**原文标题**: The Silurian Hypothesis (2020)

**原文链接**: [https://www.theparisreview.org/blog/2020/01/23/the-silurian-hypothesis/](https://www.theparisreview.org/blog/2020/01/23/the-silurian-hypothesis/)

生成摘要时出错

---

## 63. Politician reads AI prompt during assembly

**原文标题**: Politician reads AI prompt during assembly

**原文链接**: [https://www.youtube.com/watch?v=wlYa8NV5k-U](https://www.youtube.com/watch?v=wlYa8NV5k-U)

生成摘要时出错

---

## 64. Scanwheel is a drum style mechanical television you can build yourself

**原文标题**: Scanwheel is a drum style mechanical television you can build yourself

**原文链接**: [https://github.com/AncientJames/Scanwheel/](https://github.com/AncientJames/Scanwheel/)

生成摘要时出错

---

## 65. French firefighters face 'pyrocumulonimbus' for first time

**原文标题**: French firefighters face 'pyrocumulonimbus' for first time

**原文链接**: [https://www.france24.com/en/live-news/20260726-french-firefighters-face-pyrocumulonimbus-for-first-time](https://www.france24.com/en/live-news/20260726-french-firefighters-face-pyrocumulonimbus-for-first-time)

生成摘要时出错

---

## 66. Decker, a platform that builds on the legacy of Hypercard and classic macOS

**原文标题**: Decker, a platform that builds on the legacy of Hypercard and classic macOS

**原文链接**: [https://beyondloom.com/decker/](https://beyondloom.com/decker/)

生成摘要时出错

---

## 67. Corporate America Has Suddenly Decided to Stop Blowing Money on AI

**原文标题**: Corporate America Has Suddenly Decided to Stop Blowing Money on AI

**原文链接**: [https://www.wsj.com/business/china-us-ai-model-costs-53a12e96](https://www.wsj.com/business/china-us-ai-model-costs-53a12e96)

生成摘要时出错

---

## 68. 'AI Mania Is Eviscerating Global Decision-Making'

**原文标题**: 'AI Mania Is Eviscerating Global Decision-Making'

**原文链接**: [https://daringfireball.net/linked/2026/07/25/ai-mania-nikhil-suresh](https://daringfireball.net/linked/2026/07/25/ai-mania-nikhil-suresh)

生成摘要时出错

---

## 69. Multicast TV Distribution on My Home Network

**原文标题**: Multicast TV Distribution on My Home Network

**原文链接**: [https://www.apalrd.net/posts/2026/isp_mcast/](https://www.apalrd.net/posts/2026/isp_mcast/)

生成摘要时出错

---

## 70. No Stack Overflow, No Autocomplete: What Coding Felt Like in the 80s

**原文标题**: No Stack Overflow, No Autocomplete: What Coding Felt Like in the 80s

**原文链接**: [https://comuniq.xyz/post?t=1439](https://comuniq.xyz/post?t=1439)

生成摘要时出错

---

## 71. Brazilian farmers tokenized dairy cows to get loans, bypassing bank limits

**原文标题**: Brazilian farmers tokenized dairy cows to get loans, bypassing bank limits

**原文链接**: [https://www.coindesk.com/markets/2026/07/24/brazilian-farmers-tokenized-dairy-cows-to-get-loans-bypassing-bank-lending-limits](https://www.coindesk.com/markets/2026/07/24/brazilian-farmers-tokenized-dairy-cows-to-get-loans-bypassing-bank-lending-limits)

生成摘要时出错

---

## 72. The AI Productivity Illusion

**原文标题**: The AI Productivity Illusion

**原文链接**: [https://www.hardresetmedia.com/p/the-ai-productivity-illusion](https://www.hardresetmedia.com/p/the-ai-productivity-illusion)

生成摘要时出错

---

## 73. Show HN: CheapSecurity – Lightweight, Self-Hosted CCTV for Linux SBCs

**原文标题**: Show HN: CheapSecurity – Lightweight, Self-Hosted CCTV for Linux SBCs

**原文链接**: [https://github.com/gmrandazzo/CheapSecurity](https://github.com/gmrandazzo/CheapSecurity)

生成摘要时出错

---

## 74. Kimi K3 built a Windows XP in browser

**原文标题**: Kimi K3 built a Windows XP in browser

**原文链接**: [https://windows-xp.kimi.site/](https://windows-xp.kimi.site/)

生成摘要时出错

---

## 75. Harddrive Is Probably Full

**原文标题**: Harddrive Is Probably Full

**原文链接**: [https://www.marginalia.nu/log/a_139_hdd/](https://www.marginalia.nu/log/a_139_hdd/)

生成摘要时出错

---

## 76. What if the RAM/GPU shortage is deliberate?

**原文标题**: What if the RAM/GPU shortage is deliberate?

**原文链接**: [https://xn--vk5b17r.online/posts/ram-gpu-consp/](https://xn--vk5b17r.online/posts/ram-gpu-consp/)

生成摘要时出错

---

## 77. Who does Anubis actually stop?

**原文标题**: Who does Anubis actually stop?

**原文链接**: [https://fzakaria.com/2026/07/09/who-does-anubis-actually-stop](https://fzakaria.com/2026/07/09/who-does-anubis-actually-stop)

生成摘要时出错

---

## 78. The AI jobs apocalypse probably isn't coming anytime soon

**原文标题**: The AI jobs apocalypse probably isn't coming anytime soon

**原文链接**: [https://www.theguardian.com/technology/2026/jul/25/ai-jobs-apocalypse-human-labor](https://www.theguardian.com/technology/2026/jul/25/ai-jobs-apocalypse-human-labor)

生成摘要时出错

---

## 79. US accuses American of allegedly wiping his phone during border search

**原文标题**: US accuses American of allegedly wiping his phone during border search

**原文链接**: [https://techcrunch.com/2026/07/24/us-accuses-american-of-allegedly-wiping-his-phone-using-a-duress-password-during-border-search/](https://techcrunch.com/2026/07/24/us-accuses-american-of-allegedly-wiping-his-phone-using-a-duress-password-during-border-search/)

生成摘要时出错

---

## 80. Systemd Linger

**原文标题**: Systemd Linger

**原文链接**: [https://etbe.coker.com.au/2026/07/24/systemd-linger/](https://etbe.coker.com.au/2026/07/24/systemd-linger/)

生成摘要时出错

---

## 81. Lidl Introduces the European Payment Method Wero in Germany

**原文标题**: Lidl Introduces the European Payment Method Wero in Germany

**原文链接**: [https://unternehmen.lidl.de/pressreleases/260724_lidl_pi_einfuehrung_wero](https://unternehmen.lidl.de/pressreleases/260724_lidl_pi_einfuehrung_wero)

生成摘要时出错

---

## 82. League of Legends designer shares game design field manual

**原文标题**: League of Legends designer shares game design field manual

**原文链接**: [https://areadenial.games/design/preface#00-01](https://areadenial.games/design/preface#00-01)

生成摘要时出错

---

## 83. This July I Was Fired from Simple AI (A Deeply YC Company)

**原文标题**: This July I Was Fired from Simple AI (A Deeply YC Company)

**原文链接**: [https://andys.blog/this-july-i-was-fired-from-simple-ai/](https://andys.blog/this-july-i-was-fired-from-simple-ai/)

生成摘要时出错

---

## 84. Becoming a Research Engineer at a Big LLM Lab

**原文标题**: Becoming a Research Engineer at a Big LLM Lab

**原文链接**: [https://www.maxmynter.com/pages/blog/jobhunt](https://www.maxmynter.com/pages/blog/jobhunt)

生成摘要时出错

---

## 85. Task-centered iproute2 user guide

**原文标题**: Task-centered iproute2 user guide

**原文链接**: [https://baturin.org/docs/iproute2/](https://baturin.org/docs/iproute2/)

生成摘要时出错

---

## 86. Apple seeks U.S. approval to buy memory chips from blacklisted CXMT

**原文标题**: Apple seeks U.S. approval to buy memory chips from blacklisted CXMT

**原文链接**: [https://fortune.com/2026/06/27/apple-us-approval-chips-blacklisted-cxmt-price-hikes-mac-memory-shortage/](https://fortune.com/2026/06/27/apple-us-approval-chips-blacklisted-cxmt-price-hikes-mac-memory-shortage/)

生成摘要时出错

---

## 87. Amen Break

**原文标题**: Amen Break

**原文链接**: [https://en.wikipedia.org/wiki/Amen_break](https://en.wikipedia.org/wiki/Amen_break)

生成摘要时出错

---

## 88. Man convicted of child sex crime by added _ char "Fus Ro Dah" Skyrim username

**原文标题**: Man convicted of child sex crime by added _ char "Fus Ro Dah" Skyrim username

**原文链接**: [https://www.cbc.ca/news/canada/nova-scotia/how-a-single-underscore-led-to-an-innocent-halifax-man-s-conviction-9.7283149](https://www.cbc.ca/news/canada/nova-scotia/how-a-single-underscore-led-to-an-innocent-halifax-man-s-conviction-9.7283149)

生成摘要时出错

---

## 89. Chrome's Breaking and Entering

**原文标题**: Chrome's Breaking and Entering

**原文链接**: [https://unsung.aresluna.org/chromes-breaking-and-entering/](https://unsung.aresluna.org/chromes-breaking-and-entering/)

生成摘要时出错

---

## 90. My web version of Mars MIPS, now has built-in C compiler

**原文标题**: My web version of Mars MIPS, now has built-in C compiler

**原文链接**: [https://webmars.nfiles.top/](https://webmars.nfiles.top/)

生成摘要时出错

---

## 91. GNU Hurd gets 9pfs, OpenNTPD, dynamic /dev/ entries, and more

**原文标题**: GNU Hurd gets 9pfs, OpenNTPD, dynamic /dev/ entries, and more

**原文链接**: [https://www.osnews.com/story/145603/the-hurd-gets-9pfs-openntpd-dynamic-dev-entries-and-more/](https://www.osnews.com/story/145603/the-hurd-gets-9pfs-openntpd-dynamic-dev-entries-and-more/)

生成摘要时出错

---

## 92. Silicon Valley has a science fiction problem

**原文标题**: Silicon Valley has a science fiction problem

**原文链接**: [https://aeon.co/essays/silicon-valley-has-a-science-fiction-problem](https://aeon.co/essays/silicon-valley-has-a-science-fiction-problem)

生成摘要时出错

---

## 93. The whole premise of checking for human writing is daft

**原文标题**: The whole premise of checking for human writing is daft

**原文链接**: [https://mohammedshehu.com/checking-for-human-writing-is-daft/](https://mohammedshehu.com/checking-for-human-writing-is-daft/)

生成摘要时出错

---

## 94. Using ThinkPad T480 as a mobile phone

**原文标题**: Using ThinkPad T480 as a mobile phone

**原文链接**: [https://grego.site/blog/thinkphone](https://grego.site/blog/thinkphone)

生成摘要时出错

---

## 95. Show HN: SpinWin – A macOS menu bar app to visually rotate or spin any window

**原文标题**: Show HN: SpinWin – A macOS menu bar app to visually rotate or spin any window

**原文链接**: [https://github.com/alokdhir/spinwin](https://github.com/alokdhir/spinwin)

生成摘要时出错

---

## 96. France and Spain wildfires: more than 300k people displaced

**原文标题**: France and Spain wildfires: more than 300k people displaced

**原文链接**: [https://www.cnn.com/2026/07/26/world/live-news/france-spain-wildfires-evacuations](https://www.cnn.com/2026/07/26/world/live-news/france-spain-wildfires-evacuations)

生成摘要时出错

---

## 97. Possible invasive species superspreader event near Strait of Hormuz

**原文标题**: Possible invasive species superspreader event near Strait of Hormuz

**原文链接**: [https://abcnews.com/International/scientists-warn-invasive-species-superspreader-event-due-stalling/story?id=135051186](https://abcnews.com/International/scientists-warn-invasive-species-superspreader-event-due-stalling/story?id=135051186)

生成摘要时出错

---

## 98. Pope's official prayer app commits cardinal sin, leaks 700K+ users' info

**原文标题**: Pope's official prayer app commits cardinal sin, leaks 700K+ users' info

**原文链接**: [https://www.theregister.com/security/2026/07/24/popes-official-prayer-app-commits-cardinal-sin-leaks-700k-users-info/5278603](https://www.theregister.com/security/2026/07/24/popes-official-prayer-app-commits-cardinal-sin-leaks-700k-users-info/5278603)

生成摘要时出错

---

## 99. A system prompt to get AI to stop pretending to be human

**原文标题**: A system prompt to get AI to stop pretending to be human

**原文链接**: [https://swiftrocks.com/a-system-prompt-to-get-ai-to-stop-pretending-to-be-human](https://swiftrocks.com/a-system-prompt-to-get-ai-to-stop-pretending-to-be-human)

生成摘要时出错

---

## 100. ID requirement to halt freedom of information in Germany

**原文标题**: ID requirement to halt freedom of information in Germany

**原文链接**: [https://www.heise.de/en/news/Dobrindt-ID-requirement-to-halt-freedom-of-information-11376646.html](https://www.heise.de/en/news/Dobrindt-ID-requirement-to-halt-freedom-of-information-11376646.html)

生成摘要时出错

---

