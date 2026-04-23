# Hacker News 热门文章摘要 (2026-04-23)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 阿尔伯塔初创企业半价销售无科技拖拉机

**原文标题**: Alberta startup sells no-tech tractors for half price

**原文链接**: [https://wheelfront.com/this-alberta-startup-sells-no-tech-tractors-for-half-price/](https://wheelfront.com/this-alberta-startup-sells-no-tech-tractors-for-half-price/)

这篇文章来自《汽车新闻》，重点报道了一家总部位于阿尔伯塔省的初创公司，该公司向农业市场推出了一款独特的产品：“无科技”拖拉机。这些车辆的核心卖点是其显著更低的成本，定价仅为传统或技术先进型号的一半。该公司的策略似乎侧重于通过有意省略复杂技术，为农民提供一种更简单、更经济实惠的替代方案。

---

## 2. Windows 9x Linux 子系统

**原文标题**: Windows 9x Subsystem for Linux

**原文链接**: [https://social.hails.org/@hailey/116446826733136456](https://social.hails.org/@hailey/116446826733136456)

The provided text briefly introduces the concept of a "Windows 9x Subsystem for Linux." Quoting Hailey from hails.org, the snippet indicates that this subsystem would allow users to "run a..." (the sentence is truncated). Due to the brevity and incomplete nature of the provided content, further details regarding the exact functionality or purpose of this proposed subsystem are not available.

---

## 3. Qwen3.6-27B：27B稠密模型中的旗舰级编程能力

**原文标题**: Qwen3.6-27B: Flagship-Level Coding in a 27B Dense Model

**原文链接**: [https://qwen.ai/blog?id=qwen3.6-27b](https://qwen.ai/blog?id=qwen3.6-27b)

本文介绍了Qwen3.6-27B，一个旨在提供旗舰级编码能力的新模型。其主要亮点在于它能够在270亿参数的密集模型架构中实现如此高的性能。标题表明Qwen3.6-27B旨在成为编码领域的顶级竞争者，证明了即使是这种规模和类型的模型也能获得具有竞争力的高质量性能。

（注：所提供的内容极其简短，仅包含“Qwen”一词。因此，本摘要主要根据文章标题推导得出。）

---

## 4. 我正在构建云

**原文标题**: I am building a cloud

**原文链接**: [https://crawshaw.io/blog/building-a-cloud](https://crawshaw.io/blog/building-a-cloud)

David Crawshaw，某成功初创公司的联合创始人，正基于个人热情以及对当前云计算现状的深刻不满，推出exe.dev。尽管他喜欢各种平台上的计算机，但他发现当今的云产品根本上是“错误”且具有限制性的。

克劳肖指出了几个核心问题：
1.  **虚拟机抽象：** 当前的虚拟机与CPU/内存资源低效绑定，迫使用户采取复杂的变通方案或专有PaaS系统，从而限制了功能。
2.  **磁盘性能：** 远程块设备是为慢速硬盘设计的，在现代SSD上引入了严重的10倍性能损失。高IOPS价格过高，并且通常比本地硬件更慢。
3.  **网络成本：** 云端出口流量费用过高，使得每月不花费数百万美元的用户难以负担项目开销。
4.  **API与Kubernetes：** 云API令人痛苦。Kubernetes尽管初衷良好，但无法解决这些根深蒂固的架构缺陷；它只不过是“给猪涂口红”。

AI代理和大型语言模型的出现，使得解决这些问题变得迫在眉睫。代理将指数级地增加软件创建量，要求更高效、更经济、更易于管理的计算资源，而这正是当前云抽象无法提供的。

Exe.dev的解决方案通过允许用户配置裸机CPU和内存来运行他们想要的虚拟机，从而解决了这些问题。它提供带有异步复制的本地NVMe磁盘，包括内置的TLS和认证代理，提供全球区域，并利用任播网络实现低延迟访问。克劳肖旨在构建一个他真正想使用的云，并希望也能为其他人提供卓越的体验。

---

## 5. 我们发现了一个能关联你所有Tor私密身份的稳定的Firefox标识符。

**原文标题**: We found a stable Firefox identifier linking all your private Tor identities

**原文链接**: [https://fingerprint.com/blog/firefox-tor-indexeddb-privacy-vulnerability/](https://fingerprint.com/blog/firefox-tor-indexeddb-privacy-vulnerability/)

在所有基于Firefox的浏览器中，包括Firefox隐私浏览模式和Tor浏览器，都发现了一个重大的隐私漏洞。这个缺陷允许网站为正在运行的浏览器进程生成一个唯一、确定性且稳定的标识符，从而关联用户在不同来源的活动，甚至能绕过Tor浏览器“新身份”等隐私功能。

该漏洞存在于`indexedDB.databases()` API中。它没有以中立或规范的顺序返回数据库名称，而是暴露了基于浏览器内部哈希表结构的顺序。这种内部排序在浏览器进程的整个生命周期中充当一个稳定的标识符，仅在Firefox完全重启时才会重置。它还在所有来源之间共享，这意味着任何网站都可以观察到相同的标识符。

这种稳定性导致了两个主要的隐私泄露：
1.  **跨源追踪**：不相关的网站可以观察到相同的标识符，从而无需cookie或其他共享存储就能关联用户在不同域上的活动。
2.  **破坏隔离**：在Firefox隐私浏览中，即使在所有隐私窗口关闭后，该标识符仍然存在。在Tor浏览器中，它破坏了旨在提供完全隔离的“新身份”功能，允许网站关联本应相互独立的会话。

该标识符具有高熵，使其对于指纹识别非常有效。Mozilla已负责任地解决了这个问题，并在Firefox 150和ESR 140.10.0中发布了修复程序。该解决方案涉及对`indexedDB.databases()`返回的结果进行规范化（例如，排序），以消除泄露的内部排序，从而消除指纹识别信号。这一发现强调了微妙的内部实现细节如何能演变为关键的隐私漏洞。

---

## 6. SpaceX 称已达成协议，将以 600 亿美元收购 Cursor

**原文标题**: SpaceX says it has agreement to acquire Cursor for $60B

**原文链接**: [https://twitter.com/spacex/status/2046713419978453374](https://twitter.com/spacex/status/2046713419978453374)

文章标题“SpaceX 称已同意以 600 亿美元收购 Cursor”宣布了一项重大的商业进展。然而，所提供的内容并未包含任何有关此次收购的信息。

相反，文章的整个正文是来自 x.com（前身为 Twitter）的一条技术错误消息。它告知读者，他们的浏览器中禁用了 JavaScript，从而阻止了内容的显示，并建议他们启用 JavaScript 或切换到受支持的浏览器。该消息附带了标准的网站元素，例如指向帮助中心、服务条款、隐私政策、Cookie 政策、版本说明、广告信息等的链接，以及“© 2026 X Corp.”的版权声明。因此，尽管标题暗示了一项重大收购，文章正文并未提供任何有关此事件的详细信息以供总结。

---

## 7. 苹果修复了警方曾用于从iPhone中提取已删除聊天记录的漏洞。

**原文标题**: Apple fixes bug that cops used to extract deleted chat messages from iPhones

**原文链接**: [https://techcrunch.com/2026/04/22/apple-fixes-bug-that-cops-used-to-extract-deleted-chat-messages-from-iphones/](https://techcrunch.com/2026/04/22/apple-fixes-bug-that-cops-used-to-extract-deleted-chat-messages-from-iphones/)

Apple 已为 iPhone 和 iPad 发布了软件更新，修复了一个允许执法部门提取已删除或自动消失的聊天消息的漏洞。该漏洞源于通知显示的消息内容在设备上被缓存长达一个月，即使原始消息已从 Signal 等应用中删除。

这个问题最初由 404 Media 曝光，报道称 FBI 曾利用法医工具利用此漏洞从 iPhone 中恢复已删除的 Signal 消息。此后，Signal 总裁 Meredith Whittaker 公开呼吁苹果修复该问题，强调已删除消息的通知不应保留在任何操作系统数据库中。

隐私活动家对此表示担忧，指出该漏洞规避了一项关键的安全功能——定时消息删除——而这一功能是高风险用户用来保护敏感对话的。苹果的安全通知证实，“标记为删除的通知可能会被意外保留”。该公司此后已将此修复程序移植到旧版 iOS 中，表明这种保留是一个无意的错误。

---

## 8. Claude Code to be removed from Anthropic's Pro plan?

**原文标题**: Claude Code to be removed from Anthropic's Pro plan?

**原文链接**: [https://bsky.app/profile/edzitron.com/post/3mjzxwfx3qs2a](https://bsky.app/profile/edzitron.com/post/3mjzxwfx3qs2a)

生成摘要时出错

---

## 9. GPT-5.5

**原文标题**: GPT-5.5

**原文链接**: [https://openai.com/index/introducing-gpt-5-5/](https://openai.com/index/introducing-gpt-5-5/)

生成摘要时出错

---

## 10. Bitwarden CLI compromised in ongoing Checkmarx supply chain campaign

**原文标题**: Bitwarden CLI compromised in ongoing Checkmarx supply chain campaign

**原文链接**: [https://socket.dev/blog/bitwarden-cli-compromised](https://socket.dev/blog/bitwarden-cli-compromised)

生成摘要时出错

---

## 11. GitHub CLI now collects pseudoanonymous telemetry

**原文标题**: GitHub CLI now collects pseudoanonymous telemetry

**原文链接**: [https://cli.github.com/telemetry](https://cli.github.com/telemetry)

生成摘要时出错

---

## 12. Our eighth generation TPUs: two chips for the agentic era

**原文标题**: Our eighth generation TPUs: two chips for the agentic era

**原文链接**: [https://blog.google/innovation-and-ai/infrastructure-and-cloud/google-cloud/eighth-generation-tpu-agentic-era/](https://blog.google/innovation-and-ai/infrastructure-and-cloud/google-cloud/eighth-generation-tpu-agentic-era/)

生成摘要时出错

---

## 13. Over-editing refers to a model modifying code beyond what is necessary

**原文标题**: Over-editing refers to a model modifying code beyond what is necessary

**原文链接**: [https://nrehiew.github.io/blog/minimal_editing/](https://nrehiew.github.io/blog/minimal_editing/)

生成摘要时出错

---

## 14. Website streamed live directly from a model

**原文标题**: Website streamed live directly from a model

**原文链接**: [https://flipbook.page/](https://flipbook.page/)

生成摘要时出错

---

## 15. Investigation uncovers two sophisticated telecom surveillance campaigns

**原文标题**: Investigation uncovers two sophisticated telecom surveillance campaigns

**原文链接**: [https://techcrunch.com/2026/04/23/surveillance-vendors-caught-abusing-access-to-telcos-to-track-peoples-phone-locations-researchers-say/](https://techcrunch.com/2026/04/23/surveillance-vendors-caught-abusing-access-to-telcos-to-track-peoples-phone-locations-researchers-say/)

生成摘要时出错

---

## 16. An update on recent Claude Code quality reports

**原文标题**: An update on recent Claude Code quality reports

**原文链接**: [https://www.anthropic.com/engineering/april-23-postmortem](https://www.anthropic.com/engineering/april-23-postmortem)

生成摘要时出错

---

## 17. Drunk post: Things I've learned as a senior engineer (2021)

**原文标题**: Drunk post: Things I've learned as a senior engineer (2021)

**原文链接**: [https://luminousmen.substack.com/p/drunk-post-things-ive-learned-as](https://luminousmen.substack.com/p/drunk-post-things-ive-learned-as)

生成摘要时出错

---

## 18. Technical, cognitive, and intent debt

**原文标题**: Technical, cognitive, and intent debt

**原文链接**: [https://martinfowler.com/fragments/2026-04-02.html](https://martinfowler.com/fragments/2026-04-02.html)

生成摘要时出错

---

## 19. Scoring Show HN submissions for AI design patterns

**原文标题**: Scoring Show HN submissions for AI design patterns

**原文链接**: [https://www.adriankrebs.ch/blog/design-slop/](https://www.adriankrebs.ch/blog/design-slop/)

生成摘要时出错

---

## 20. French government agency confirms breach as hacker offers to sell data

**原文标题**: French government agency confirms breach as hacker offers to sell data

**原文链接**: [https://www.bleepingcomputer.com/news/security/french-govt-agency-confirms-breach-as-hacker-offers-to-sell-data/](https://www.bleepingcomputer.com/news/security/french-govt-agency-confirms-breach-as-hacker-offers-to-sell-data/)

生成摘要时出错

---

## 21. Palantir employees are starting to wonder if they're the bad guys

**原文标题**: Palantir employees are starting to wonder if they're the bad guys

**原文链接**: [https://www.wired.com/story/palantir-employees-are-starting-to-wonder-if-theyre-the-bad-guys/](https://www.wired.com/story/palantir-employees-are-starting-to-wonder-if-theyre-the-bad-guys/)

生成摘要时出错

---

## 22. 3.4M Solar Panels

**原文标题**: 3.4M Solar Panels

**原文链接**: [https://tech.marksblogg.com/american-solar-farms-v2.html](https://tech.marksblogg.com/american-solar-farms-v2.html)

生成摘要时出错

---

## 23. Parallel agents in Zed

**原文标题**: Parallel agents in Zed

**原文链接**: [https://zed.dev/blog/parallel-agents](https://zed.dev/blog/parallel-agents)

生成摘要时出错

---

## 24. Claude Code to be removed from Pro Tier?

**原文标题**: Claude Code to be removed from Pro Tier?

**原文链接**: [https://bsky.app/profile/edzitron.com/post/3mjzxwfx3qs2a](https://bsky.app/profile/edzitron.com/post/3mjzxwfx3qs2a)

生成摘要时出错

---

## 25. If America's so rich, how'd it get so sad?

**原文标题**: If America's so rich, how'd it get so sad?

**原文链接**: [https://www.derekthompson.org/p/if-americas-so-rich-howd-it-get-so](https://www.derekthompson.org/p/if-americas-so-rich-howd-it-get-so)

生成摘要时出错

---

## 26. Arch Linux Now Has a Bit-for-Bit Reproducible Docker Image

**原文标题**: Arch Linux Now Has a Bit-for-Bit Reproducible Docker Image

**原文链接**: [https://antiz.fr/blog/archlinux-now-has-a-reproducible-docker-image/](https://antiz.fr/blog/archlinux-now-has-a-reproducible-docker-image/)

生成摘要时出错

---

## 27. Ultraviolet corona discharges on treetops during storms

**原文标题**: Ultraviolet corona discharges on treetops during storms

**原文链接**: [https://www.psu.edu/news/earth-and-mineral-sciences/story/treetops-glowing-during-storms-captured-film-first-time](https://www.psu.edu/news/earth-and-mineral-sciences/story/treetops-glowing-during-storms-captured-film-first-time)

生成摘要时出错

---

## 28. Another Day Has Come

**原文标题**: Another Day Has Come

**原文链接**: [https://daringfireball.net/2026/04/another_day_has_come](https://daringfireball.net/2026/04/another_day_has_come)

生成摘要时出错

---

## 29. I don't want your PRs anymore

**原文标题**: I don't want your PRs anymore

**原文链接**: [https://dpc.pw/posts/i-dont-want-your-prs-anymore/](https://dpc.pw/posts/i-dont-want-your-prs-anymore/)

生成摘要时出错

---

## 30. How does GPS work?

**原文标题**: How does GPS work?

**原文链接**: [https://perthirtysix.com/how-the-heck-does-gps-work](https://perthirtysix.com/how-the-heck-does-gps-work)

生成摘要时出错

---

## 31. Irony as Meta staff unhappy about running surveillance software on work PCs

**原文标题**: Irony as Meta staff unhappy about running surveillance software on work PCs

**原文链接**: [https://www.theregister.com/2026/04/22/meta_employee_surveillance_software/](https://www.theregister.com/2026/04/22/meta_employee_surveillance_software/)

生成摘要时出错

---

## 32. Youth Suicides Declined After Creation of National Hotline

**原文标题**: Youth Suicides Declined After Creation of National Hotline

**原文链接**: [https://www.nytimes.com/2026/04/22/science/988-youth-suicides-decline.html](https://www.nytimes.com/2026/04/22/science/988-youth-suicides-decline.html)

生成摘要时出错

---

## 33. FBI looks into dead or missing scientists tied to NASA, Blue Origin, SpaceX

**原文标题**: FBI looks into dead or missing scientists tied to NASA, Blue Origin, SpaceX

**原文链接**: [https://fortune.com/2026/04/21/scientists-disappear-die-nasa-space-blue-origin-spacex/](https://fortune.com/2026/04/21/scientists-disappear-die-nasa-space-blue-origin-spacex/)

生成摘要时出错

---

## 34. XOR'ing a register with itself is the idiom for zeroing it out. Why not sub?

**原文标题**: XOR'ing a register with itself is the idiom for zeroing it out. Why not sub?

**原文链接**: [https://devblogs.microsoft.com/oldnewthing/20260421-00/?p=112247](https://devblogs.microsoft.com/oldnewthing/20260421-00/?p=112247)

生成摘要时出错

---

## 35. San Diego rents declined following surge in supply

**原文标题**: San Diego rents declined following surge in supply

**原文链接**: [https://www.kpbs.org/news/economy/2026/03/27/san-diego-rents-declined-more-than-19-of-nations-top-20-markets-following-surge-in-supply](https://www.kpbs.org/news/economy/2026/03/27/san-diego-rents-declined-more-than-19-of-nations-top-20-markets-following-surge-in-supply)

生成摘要时出错

---

## 36. 'Hairdryer used to trick weather sensor' to win Polymarket bet

**原文标题**: 'Hairdryer used to trick weather sensor' to win Polymarket bet

**原文链接**: [https://www.telegraph.co.uk/business/2026/04/23/hairdryer-used-trick-weather-sensor-34000-polymarket-bet/](https://www.telegraph.co.uk/business/2026/04/23/hairdryer-used-trick-weather-sensor-34000-polymarket-bet/)

生成摘要时出错

---

## 37. Scores decline again for 13-year-old students in reading and mathematics (2023)

**原文标题**: Scores decline again for 13-year-old students in reading and mathematics (2023)

**原文链接**: [https://www.nationsreportcard.gov/highlights/ltt/2023/](https://www.nationsreportcard.gov/highlights/ltt/2023/)

生成摘要时出错

---

## 38. Show HN: Honker – Postgres NOTIFY/LISTEN Semantics for SQLite

**原文标题**: Show HN: Honker – Postgres NOTIFY/LISTEN Semantics for SQLite

**原文链接**: [https://github.com/russellromney/honker](https://github.com/russellromney/honker)

生成摘要时出错

---

## 39. To Protect and Swerve: NYPD Cop Has 547 Speeding Tickets

**原文标题**: To Protect and Swerve: NYPD Cop Has 547 Speeding Tickets

**原文链接**: [https://nyc.streetsblog.org/2026/04/23/to-protect-and-swerve-nypd-cop-has-527-speeding-tickets-yet-remains-on-the-force](https://nyc.streetsblog.org/2026/04/23/to-protect-and-swerve-nypd-cop-has-527-speeding-tickets-yet-remains-on-the-force)

生成摘要时出错

---

## 40. Meta to cut 10% of jobs, or 8k employees

**原文标题**: Meta to cut 10% of jobs, or 8k employees

**原文链接**: [https://techcrunch.com/2026/04/23/meta-job-cuts-10-percent-8000-employees/](https://techcrunch.com/2026/04/23/meta-job-cuts-10-percent-8000-employees/)

生成摘要时出错

---

## 41. Raylib v6.0

**原文标题**: Raylib v6.0

**原文链接**: [https://github.com/raysan5/raylib/releases/tag/6.0](https://github.com/raysan5/raylib/releases/tag/6.0)

生成摘要时出错

---

## 42. Ping-pong robot beats top-level human players

**原文标题**: Ping-pong robot beats top-level human players

**原文链接**: [https://www.reuters.com/sports/ping-pong-robot-ace-makes-history-by-beating-top-level-human-players-2026-04-22/](https://www.reuters.com/sports/ping-pong-robot-ace-makes-history-by-beating-top-level-human-players-2026-04-22/)

生成摘要时出错

---

## 43. Our newsroom AI policy

**原文标题**: Our newsroom AI policy

**原文链接**: [https://arstechnica.com/staff/2026/04/our-newsroom-ai-policy/](https://arstechnica.com/staff/2026/04/our-newsroom-ai-policy/)

生成摘要时出错

---

## 44. DuckDB 1.5.2 – SQL database that runs on laptop, server, in the browser

**原文标题**: DuckDB 1.5.2 – SQL database that runs on laptop, server, in the browser

**原文链接**: [https://duckdb.org/2026/04/13/announcing-duckdb-152](https://duckdb.org/2026/04/13/announcing-duckdb-152)

生成摘要时出错

---

## 45. Workspace Agents in ChatGPT

**原文标题**: Workspace Agents in ChatGPT

**原文链接**: [https://openai.com/index/introducing-workspace-agents-in-chatgpt/](https://openai.com/index/introducing-workspace-agents-in-chatgpt/)

生成摘要时出错

---

## 46. US Department of Justice has officially reclassified cannabis as less dangerous

**原文标题**: US Department of Justice has officially reclassified cannabis as less dangerous

**原文链接**: [https://www.bbc.com/news/articles/cdxd0xxp0jko](https://www.bbc.com/news/articles/cdxd0xxp0jko)

生成摘要时出错

---

## 47. CATL's new LFP battery can charge from 10 to 98% in less than 7 minutes

**原文标题**: CATL's new LFP battery can charge from 10 to 98% in less than 7 minutes

**原文链接**: [https://arstechnica.com/cars/2026/04/catls-new-lfp-battery-can-charge-from-10-to-98-in-less-than-7-minutes/](https://arstechnica.com/cars/2026/04/catls-new-lfp-battery-can-charge-from-10-to-98-in-less-than-7-minutes/)

生成摘要时出错

---

## 48. You don't need advice from editors on rejected manuscripts

**原文标题**: You don't need advice from editors on rejected manuscripts

**原文链接**: [https://twitter.com/orsonscottcard/status/2046702294406680751](https://twitter.com/orsonscottcard/status/2046702294406680751)

生成摘要时出错

---

## 49. Incident with multple GitHub services

**原文标题**: Incident with multple GitHub services

**原文链接**: [https://www.githubstatus.com/incidents/myrbk7jvvs6p](https://www.githubstatus.com/incidents/myrbk7jvvs6p)

生成摘要时出错

---

## 50. Nobody got fired for Uber's $8M ledger mistake?

**原文标题**: Nobody got fired for Uber's $8M ledger mistake?

**原文链接**: [https://news.alvaroduran.com/p/nobody-got-fired-for-ubers-8-million](https://news.alvaroduran.com/p/nobody-got-fired-for-ubers-8-million)

生成摘要时出错

---

## 51. Kernel code removals driven by LLM-created security reports

**原文标题**: Kernel code removals driven by LLM-created security reports

**原文链接**: [https://lwn.net/Articles/1068928/](https://lwn.net/Articles/1068928/)

生成摘要时出错

---

## 52. Surveillance Pricing: Exploiting Information Asymmetries

**原文标题**: Surveillance Pricing: Exploiting Information Asymmetries

**原文链接**: [https://lpeproject.org/blog/surveillance-pricing-exploiting-information-asymmetries/](https://lpeproject.org/blog/surveillance-pricing-exploiting-information-asymmetries/)

生成摘要时出错

---

## 53. Columnar Storage Is Normalization

**原文标题**: Columnar Storage Is Normalization

**原文链接**: [https://buttondown.com/jaffray/archive/columnar-storage-is-normalization/](https://buttondown.com/jaffray/archive/columnar-storage-is-normalization/)

生成摘要时出错

---

## 54. Meta employees are up in arms over a mandatory program to train AI on their

**原文标题**: Meta employees are up in arms over a mandatory program to train AI on their

**原文链接**: [https://www.businessinsider.com/meta-new-ai-tool-tracks-staff-activity-sparks-concern-2026-4](https://www.businessinsider.com/meta-new-ai-tool-tracks-staff-activity-sparks-concern-2026-4)

生成摘要时出错

---

## 55. Writing a C Compiler, in Zig (2025)

**原文标题**: Writing a C Compiler, in Zig (2025)

**原文链接**: [https://ar-ms.me/thoughts/c-compiler-1-zig/](https://ar-ms.me/thoughts/c-compiler-1-zig/)

生成摘要时出错

---

## 56. SpaceX says it has agreement to acquire Cursor for $60B

**原文标题**: SpaceX says it has agreement to acquire Cursor for $60B

**原文链接**: [https://www.bloomberg.com/news/articles/2026-04-21/spacex-says-has-agreement-to-acquire-cursor-for-60-billion](https://www.bloomberg.com/news/articles/2026-04-21/spacex-says-has-agreement-to-acquire-cursor-for-60-billion)

生成摘要时出错

---

## 57. California has more money than projected after admin miscalculated state budget

**原文标题**: California has more money than projected after admin miscalculated state budget

**原文链接**: [https://www.kcra.com/article/california-more-money-than-projected-newsom-miscalculated-budget/71056376](https://www.kcra.com/article/california-more-money-than-projected-newsom-miscalculated-budget/71056376)

生成摘要时出错

---

## 58. Sam Altman's Creepy Eyeball-Scanning Company Gets in Bed with Zoom and Tinder

**原文标题**: Sam Altman's Creepy Eyeball-Scanning Company Gets in Bed with Zoom and Tinder

**原文链接**: [https://gizmodo.com/sam-altmans-creepy-eyeball-scanning-company-gets-in-bed-with-zoom-and-tinder-2000748013](https://gizmodo.com/sam-altmans-creepy-eyeball-scanning-company-gets-in-bed-with-zoom-and-tinder-2000748013)

生成摘要时出错

---

## 59. New study compares growing corn for energy to solar production

**原文标题**: New study compares growing corn for energy to solar production

**原文链接**: [https://www.anthropocenemagazine.org/2025/04/new-study-compares-growing-corn-for-energy-to-solar-production-its-no-contest/](https://www.anthropocenemagazine.org/2025/04/new-study-compares-growing-corn-for-energy-to-solar-production-its-no-contest/)

生成摘要时出错

---

## 60. Global growth in solar "the largest ever observed for any source"

**原文标题**: Global growth in solar "the largest ever observed for any source"

**原文链接**: [https://arstechnica.com/science/2026/04/global-growth-in-solar-the-largest-ever-observed-for-any-source/](https://arstechnica.com/science/2026/04/global-growth-in-solar-the-largest-ever-observed-for-any-source/)

生成摘要时出错

---

## 61. Tempest vs. Tempest: The Making and Remaking of Atari's Iconic Video Game

**原文标题**: Tempest vs. Tempest: The Making and Remaking of Atari's Iconic Video Game

**原文链接**: [https://tempest.homemade.systems](https://tempest.homemade.systems)

生成摘要时出错

---

## 62. SpaceX与Cursor达成600亿美元交易。

**原文标题**: SpaceX strikes deal with Cursor for $60B

**原文链接**: [https://www.nytimes.com/2026/04/21/business/spacex-cursor-deal.html](https://www.nytimes.com/2026/04/21/business/spacex-cursor-deal.html)

生成摘要时出错

---

## 63. Top MAGA influencer revealed to be AI

**原文标题**: Top MAGA influencer revealed to be AI

**原文链接**: [https://nypost.com/2026/04/21/us-news/top-maga-influencer-emily-hart-revealed-to-be-ai-created-by-a-guy-in-india/](https://nypost.com/2026/04/21/us-news/top-maga-influencer-emily-hart-revealed-to-be-ai-created-by-a-guy-in-india/)

生成摘要时出错

---

## 64. 谷歌云客户收到18,000美元账单，预算却仅7美元

**原文标题**: Google Cloud customer wakes up to $18,000 bill despite $7 budget

**原文链接**: [https://www.tomshardware.com/tech-industry/artificial-intelligence/google-cloud-customer-wakes-up-to-usd18-000-bill-despite-usd7-budget-thanks-to-forgotten-public-api-key-attacker-put-in-60-000-requests-and-blasted-through-usd1-400-spending-cap](https://www.tomshardware.com/tech-industry/artificial-intelligence/google-cloud-customer-wakes-up-to-usd18-000-bill-despite-usd7-budget-thanks-to-forgotten-public-api-key-attacker-put-in-60-000-requests-and-blasted-through-usd1-400-spending-cap)

生成摘要时出错

---

## 65. OpenAI's response to the Axios developer tool compromise

**原文标题**: OpenAI's response to the Axios developer tool compromise

**原文链接**: [https://openai.com/index/axios-developer-tool-compromise/](https://openai.com/index/axios-developer-tool-compromise/)

生成摘要时出错

---

## 66. Iran claims US exploited networking equipment backdoors during strikes

**原文标题**: Iran claims US exploited networking equipment backdoors during strikes

**原文链接**: [https://www.tomshardware.com/tech-industry/cyber-security/iran-claims-us-exploited-networking-equipment-backdoors-during-strikes](https://www.tomshardware.com/tech-industry/cyber-security/iran-claims-us-exploited-networking-equipment-backdoors-during-strikes)

生成摘要时出错

---

## 67. A Boy That Cried Mythos: Verification Is Collapsing Trust in Anthropic

**原文标题**: A Boy That Cried Mythos: Verification Is Collapsing Trust in Anthropic

**原文链接**: [https://www.flyingpenguin.com/the-boy-that-cried-mythos-verification-is-collapsing-trust-in-anthropic/](https://www.flyingpenguin.com/the-boy-that-cried-mythos-verification-is-collapsing-trust-in-anthropic/)

生成摘要时出错

---

## 68. Spam in conversational replies to blog posts

**原文标题**: Spam in conversational replies to blog posts

**原文链接**: [https://shkspr.mobi/blog/2026/04/sneaky-spam-in-conversational-replies-to-blog-posts/](https://shkspr.mobi/blog/2026/04/sneaky-spam-in-conversational-replies-to-blog-posts/)

生成摘要时出错

---

## 69. Borrow-checking without type-checking

**原文标题**: Borrow-checking without type-checking

**原文链接**: [https://www.scattered-thoughts.net/writing/borrow-checking-without-type-checking/](https://www.scattered-thoughts.net/writing/borrow-checking-without-type-checking/)

生成摘要时出错

---

## 70. Claude Code Removed from $20-a-Month "Pro" Subscription for New Users

**原文标题**: Claude Code Removed from $20-a-Month "Pro" Subscription for New Users

**原文链接**: [https://www.wheresyoured.at/news-anthropic-removes-pro-cc/](https://www.wheresyoured.at/news-anthropic-removes-pro-cc/)

生成摘要时出错

---

## 71. MacBook Neo and How the iPad Should Be

**原文标题**: MacBook Neo and How the iPad Should Be

**原文链接**: [https://craigmod.com/essays/ipad_neo/](https://craigmod.com/essays/ipad_neo/)

生成摘要时出错

---

## 72. Bring Your Agent to Teams

**原文标题**: Bring Your Agent to Teams

**原文链接**: [https://microsoft.github.io/teams-sdk/blog/bring-your-agent-to-teams/](https://microsoft.github.io/teams-sdk/blog/bring-your-agent-to-teams/)

生成摘要时出错

---

## 73. MeshCore development team splits over trademark dispute and AI-generated code

**原文标题**: MeshCore development team splits over trademark dispute and AI-generated code

**原文链接**: [https://blog.meshcore.io/2026/04/23/the-split](https://blog.meshcore.io/2026/04/23/the-split)

生成摘要时出错

---

## 74. Show HN: Broccoli, one shot coding agent on the cloud

**原文标题**: Show HN: Broccoli, one shot coding agent on the cloud

**原文链接**: [https://github.com/besimple-oss/broccoli](https://github.com/besimple-oss/broccoli)

生成摘要时出错

---

## 75. The eighth-generation TPU: An architecture deep dive

**原文标题**: The eighth-generation TPU: An architecture deep dive

**原文链接**: [https://cloud.google.com/blog/products/compute/tpu-8t-and-tpu-8i-technical-deep-dive](https://cloud.google.com/blog/products/compute/tpu-8t-and-tpu-8i-technical-deep-dive)

生成摘要时出错

---

## 76. Anker made its own chip to bring AI to all its products

**原文标题**: Anker made its own chip to bring AI to all its products

**原文链接**: [https://www.theverge.com/tech/916463/anker-thus-chip-announcement](https://www.theverge.com/tech/916463/anker-thus-chip-announcement)

生成摘要时出错

---

## 77. Maryland to become first state to ban 'dynamic pricing' in grocery stores

**原文标题**: Maryland to become first state to ban 'dynamic pricing' in grocery stores

**原文链接**: [https://www.yahoo.com/news/articles/maryland-become-first-state-ban-150854726.html](https://www.yahoo.com/news/articles/maryland-become-first-state-ban-150854726.html)

生成摘要时出错

---

## 78. It's time to reclaim the word "Palantir" for JRR Tolkien

**原文标题**: It's time to reclaim the word "Palantir" for JRR Tolkien

**原文链接**: [https://www.zig.art/p/its-time-to-reclaim-the-word-palantir](https://www.zig.art/p/its-time-to-reclaim-the-word-palantir)

生成摘要时出错

---

## 79. Anthropic's Mythos Model Is Being Accessed by Unauthorized Users

**原文标题**: Anthropic's Mythos Model Is Being Accessed by Unauthorized Users

**原文链接**: [https://www.bloomberg.com/news/articles/2026-04-21/anthropic-s-mythos-model-is-being-accessed-by-unauthorized-users](https://www.bloomberg.com/news/articles/2026-04-21/anthropic-s-mythos-model-is-being-accessed-by-unauthorized-users)

生成摘要时出错

---

## 80. US saw record high of 5,668 books banned in libraries in 2025, says agency

**原文标题**: US saw record high of 5,668 books banned in libraries in 2025, says agency

**原文链接**: [https://www.theguardian.com/us-news/2026/apr/22/us-libraries-banned-books](https://www.theguardian.com/us-news/2026/apr/22/us-libraries-banned-books)

生成摘要时出错

---

## 81. The Illuminated Man: an unconventional portrait of JG Ballard

**原文标题**: The Illuminated Man: an unconventional portrait of JG Ballard

**原文链接**: [https://www.theguardian.com/books/2026/apr/20/the-illuminated-man-by-christopher-priest-and-nina-allan-review-an-unconventional-portrait-of-jg-ballard](https://www.theguardian.com/books/2026/apr/20/the-illuminated-man-by-christopher-priest-and-nina-allan-review-an-unconventional-portrait-of-jg-ballard)

生成摘要时出错

---

## 82. CDC blocks study showing Covid shots cut hospital visits after earlier delay

**原文标题**: CDC blocks study showing Covid shots cut hospital visits after earlier delay

**原文链接**: [https://www.washingtonpost.com/health/2026/04/22/covid-vaccine-report-blocked-cdc-mmwr/](https://www.washingtonpost.com/health/2026/04/22/covid-vaccine-report-blocked-cdc-mmwr/)

生成摘要时出错

---

## 83. Show HN: Built a daily game where you sort historical events chronologically

**原文标题**: Show HN: Built a daily game where you sort historical events chronologically

**原文链接**: [https://hisorty.app/](https://hisorty.app/)

生成摘要时出错

---

## 84. Polymarket weather bet manipulated with a hairdryer

**原文标题**: Polymarket weather bet manipulated with a hairdryer

**原文链接**: [https://twitter.com/aaronjmars/status/2047017251270734309](https://twitter.com/aaronjmars/status/2047017251270734309)

生成摘要时出错

---

## 85. Zindex – Diagram Infrastructure for Agents

**原文标题**: Zindex – Diagram Infrastructure for Agents

**原文链接**: [https://zindex.ai/](https://zindex.ai/)

生成摘要时出错

---

## 86. The zero-days are numbered

**原文标题**: The zero-days are numbered

**原文链接**: [https://blog.mozilla.org/en/privacy-security/ai-security-zero-day-vulnerabilities/](https://blog.mozilla.org/en/privacy-security/ai-security-zero-day-vulnerabilities/)

生成摘要时出错

---

## 87. Kuri – Zig based agent-browser alternative

**原文标题**: Kuri – Zig based agent-browser alternative

**原文链接**: [https://github.com/justrach/kuri](https://github.com/justrach/kuri)

生成摘要时出错

---

## 88. Show HN: Run coding agents in microVM sandboxes instead of your host machine

**原文标题**: Show HN: Run coding agents in microVM sandboxes instead of your host machine

**原文链接**: [https://github.com/superhq-ai/superhq](https://github.com/superhq-ai/superhq)

生成摘要时出错

---

## 89. Fundamental Theorem of Calculus

**原文标题**: Fundamental Theorem of Calculus

**原文链接**: [https://david.alvarezrosa.com/posts/fundamental-theorem-of-calculus/](https://david.alvarezrosa.com/posts/fundamental-theorem-of-calculus/)

生成摘要时出错

---

## 90. Tesla admits HW3 owners need upgrades for true 'Full Self-Driving'

**原文标题**: Tesla admits HW3 owners need upgrades for true 'Full Self-Driving'

**原文链接**: [https://techcrunch.com/2026/04/22/elon-musk-admits-millions-of-tesla-owners-need-upgrades-for-true-full-self-driving/](https://techcrunch.com/2026/04/22/elon-musk-admits-millions-of-tesla-owners-need-upgrades-for-true-full-self-driving/)

生成摘要时出错

---

## 91. The Neon King of New Orleans

**原文标题**: The Neon King of New Orleans

**原文链接**: [https://gardenandgun.com/new-orleans-neon-king](https://gardenandgun.com/new-orleans-neon-king)

生成摘要时出错

---

## 92. What Async Promised and What It Delivered

**原文标题**: What Async Promised and What It Delivered

**原文链接**: [https://causality.blog/essays/what-async-promised/](https://causality.blog/essays/what-async-promised/)

生成摘要时出错

---

## 93. Startups brag they spend more money on AI than human employees

**原文标题**: Startups brag they spend more money on AI than human employees

**原文链接**: [https://www.404media.co/startups-brag-they-spend-more-money-on-ai-than-human-employees/](https://www.404media.co/startups-brag-they-spend-more-money-on-ai-than-human-employees/)

生成摘要时出错

---

## 94. The handmade beauty of Machine Age data visualizations

**原文标题**: The handmade beauty of Machine Age data visualizations

**原文链接**: [https://resobscura.substack.com/p/the-handmade-beauty-of-machine-age](https://resobscura.substack.com/p/the-handmade-beauty-of-machine-age)

生成摘要时出错

---

## 95. Southern Poverty Law Center indicted for fraud, money laundering

**原文标题**: Southern Poverty Law Center indicted for fraud, money laundering

**原文链接**: [https://www.politico.com/news/2026/04/21/southern-poverty-law-center-justice-department-investigation-00885376](https://www.politico.com/news/2026/04/21/southern-poverty-law-center-justice-department-investigation-00885376)

生成摘要时出错

---

## 96. OpenAI: Workspace Agents for Business

**原文标题**: OpenAI: Workspace Agents for Business

**原文链接**: [https://openai.com/business/workspace-agents/](https://openai.com/business/workspace-agents/)

生成摘要时出错

---

## 97. Approximating Hyperbolic Tangent

**原文标题**: Approximating Hyperbolic Tangent

**原文链接**: [https://jtomschroeder.com/blog/approximating-tanh/](https://jtomschroeder.com/blog/approximating-tanh/)

生成摘要时出错

---

## 98. Smart TV tracking raises privacy concerns (2024)

**原文标题**: Smart TV tracking raises privacy concerns (2024)

**原文链接**: [https://www.ucl.ac.uk/news/2024/nov/smart-tv-tracking-raises-privacy-concerns](https://www.ucl.ac.uk/news/2024/nov/smart-tv-tracking-raises-privacy-concerns)

生成摘要时出错

---

## 99. Do you want the US to "win" AI?

**原文标题**: Do you want the US to "win" AI?

**原文链接**: [https://geohot.github.io//blog/jekyll/update/2026/04/23/us-win-ai.html](https://geohot.github.io//blog/jekyll/update/2026/04/23/us-win-ai.html)

生成摘要时出错

---

## 100. OpenAI model for masking personally identifiable information (PII) in text

**原文标题**: OpenAI model for masking personally identifiable information (PII) in text

**原文链接**: [https://openai.com/index/introducing-openai-privacy-filter/](https://openai.com/index/introducing-openai-privacy-filter/)

生成摘要时出错

---

