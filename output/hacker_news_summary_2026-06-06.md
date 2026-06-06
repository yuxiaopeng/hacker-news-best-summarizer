# Hacker News 热门文章摘要 (2026-06-06)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 宝可梦 绿宝石 移植到 WebAssembly (10万 FPS)

**原文标题**: Pokemon Emerald Ported to WebAssembly (100k FPS)

**原文链接**: [https://pokeemerald.com/](https://pokeemerald.com/)

本文宣布经典游戏《宝可梦 绿宝石》已成功移植到WebAssembly，并展示了令人印象深刻的性能，达到每秒10万帧（FPS）。随附内容展示了该移植版本的交互式网页界面。界面开始时显示“loading wasm…”指示器，随后是屏幕上的游戏控制按钮，包括方向键（↑、←、→、↓）和动作按钮（B、A、SELECT、START）。界面还显示当前游戏速度设置为“1x”。重要的是，它提供了清晰的键盘操作映射：方向键控制移动，'Z'键作为'A'按钮，'X'键作为'B'按钮，'Enter'键作为'Start'，'Shift'键作为'Select'。这种设置突显了这款深受喜爱的Game Boy Advance游戏的高度优化且用户友好的网络版再现。

---

## 2. 消息人士称，五角大楼将以色列对美间谍威胁级别升至最高。

**原文标题**: Pentagon raised threat of Israeli spying on U.S. to highest level, sources say

**原文链接**: [https://www.nbcnews.com/politics/national-security/pentagon-raised-threat-israeli-spying-us-highest-level-sources-say-rcna348565](https://www.nbcnews.com/politics/national-security/pentagon-raised-threat-israeli-spying-us-highest-level-sources-say-rcna348565)

五角大楼已将以色列对美国间谍活动的反情报威胁级别提升至“危急”，美国官员表示，这是最高级别。美国国防情报局（DIA）发布了这一评估，此前有担忧指出，以色列正在大幅增加对美国高级官员的监视。其目的据报是收集有关特朗普政府在中东冲突，特别是与伊朗的战争方面的内部审议和决策信息。

国防情报局的评估在一份七页的详细文件中指出具体事件，并将以色列的人力和技术情报收集能力评定为“危急”。这一举动发生之际，特朗普总统与以色列总理本雅明·内塔尼亚胡在对伊战争方向问题上的紧张关系日益加剧，特朗普寻求外交协议，而内塔尼亚胡则主张恢复军事行动。

以色列驻华盛顿大使馆强烈否认这些指控，声明以色列不刺探美国，只针对其敌人。一位白宫官员也驳斥这一说法“不实”。

虽然盟友之间存在间谍活动并非罕见，但美国官员认为以色列目前的行动超出了寻常水平。历史上，以色列以对美国进行咄咄逼人的情报收集而闻名，乔纳森·波拉德案便是例证。实际影响是，美国官员在与以色列同行互动或赴以色列时将格外谨慎，尽管与伊朗战争相关的关键情报共享似乎仍未受影响。这一局面存在侵蚀这两个亲密盟友之间信任的风险。

---

## 3. 超越 fork() + exec()

**原文标题**: Moving beyond fork() + exec()

**原文链接**: [https://lwn.net/SubscriberLink/1076018/16f01bbbb8e0d1f0/](https://lwn.net/SubscriberLink/1076018/16f01bbbb8e0d1f0/)

文章指出了Unix/Linux中 `fork()` + `exec()` 进程创建模型长期存在的低效问题。`fork()` 开销很大，它会复制父进程的整个状态，而 `exec()` 却往往立即丢弃这些内存。

陈立提出了“spawn模板”来优化这一问题，其思路是允许应用程序在重复启动*相同*的可执行文件时，通过 `spawn_template_create()` 创建一个模板。这会缓存可执行文件信息，使得后续的 `spawn_template_spawn()` 调用（这些调用指定参数、环境变量和文件描述符操作）变得更快。基准测试显示性能约有2%的提升，分摊了 `exec()` 部分的设置成本。

然而，内核开发者，特别是Mateusz Guzik，批评陈立的提议未能解决主要开销：`fork()`。Guzik主张直接“创建一个纯净的进程”。Christian Brauner同意这一目标，但建议基于 `pidfd` 构建一个更健壮的API。他的设想是使用 `pidfd_open()` 创建一个空进程，随后通过 `pidfd_config()` 调用设置其环境变量、可执行映像及其他属性。这个新接口的一个关键目标将是在用户空间支持一个原生的、高效的 `posix_spawn()` 实现，从而避免当前 `posix_spawn()` 实现中隐藏的 `fork()` + `exec()` 调用。

陈立接受了Brauner的方向。因此，“spawn模板”将不会被合入。相反，未来的工作将集中于开发一个基于 `pidfd` 的API，以提供一个适当的、优化的 `posix_spawn()` 实现，最终超越存在问题的 `fork()` + `exec()` 范式。

---

## 4. Fine-tuning an LLM to write docs like it's 1995

**原文标题**: Fine-tuning an LLM to write docs like it's 1995

**原文链接**: [https://passo.uno/fine-tuning-docs-llm/](https://passo.uno/fine-tuning-docs-llm/)

The author experimented with fine-tuning an LLM to emulate 1990s software technical writing style, a step towards potential future local, specialized LLMs. For training data, they utilized Bitsavers' Microsoft collection of old manuals (1977-2005), cleaning 37 million words down to 192,456 JSONL examples with Python and `gemma-4-26b` for intelligibility.

Instead of training from scratch, QLoRA fine-tuning was chosen for style transfer, not factual retrieval, using Runpod for GPU access (costing around $50). The experiment involved Llama 3.1 8B Instruct, Qwen 2.5 7B Instruct, and a Llama base model. Various parameters were tested, including training data volume, epochs, and QLoRA rank.

Results showed significant style transfer. For documenting `malloc()`, fine-tuned models adopted period-correct structures (Synopsis, Return Value). For a fictitious `ConnectWifi()` function, the 3-epoch Qwen model best maintained the 90s fiction. Most remarkably, Qwen fine-tunes, especially `msft-qwen-192k`, excelled at explaining a modern `REST API` in a convincing, anachronistic 90s-Microsoft style chapter opening. Llama Instruct, due to heavy RLHF, produced bland marketing prose, while the base model failed entirely. Smaller QLoRA ranks (e.g., rank 8) with fewer epochs committed more strongly to the impersonation.

The author concludes that fine-tuned models are effective, relatively cheap style impersonators, useful for augmenting tech writers in tasks like style review or drafting. However, they demand high-quality data, careful model and parameter selection, and still lack human judgment, necessitating significant steering.

---

## 5. Programmers will document for Claude, but not for each other

**原文标题**: Programmers will document for Claude, but not for each other

**原文链接**: [https://blog.plover.com/2026/03/09/#documentation-wins-2](https://blog.plover.com/2026/03/09/#documentation-wins-2)

生成摘要时出错

---

## 6. 量子纠缠构建时空。现在，“神奇”赋予其引力。

**原文标题**: Entanglement Builds Space-Time. Now "Magic" Gives It Gravity

**原文链接**: [https://www.quantamagazine.org/entanglement-builds-space-time-now-magic-gives-it-gravity-20260603/](https://www.quantamagazine.org/entanglement-builds-space-time-now-magic-gives-it-gravity-20260603/)

物理学家在理解引力如何从量子力学中涌现方面迈出了重要一步，解决了约翰·阿奇博尔德·惠勒提出的“物质告诉时空如何弯曲”的挑战。在全息理论中，时空被视为量子粒子集合。此前，这些粒子间的纠缠被证明能构建时空结构，使得空间能够告诉物质如何运动。然而，这些模型产生的时空是“惰性的”，不会响应物质而弯曲。

查尔斯·曹（Charles Cao）领导的新研究将一种名为“魔性”（magic）的量子特性确定为缺失的要素。魔性是量子纠错码中由“非克利福德门”（non-Clifford gates）引入的一种量子性度量，它使时空变得可弯曲。与此前完美分离空间和物质的“稳定器码”（stabilizer codes）不同，新的魔性码允许与空间和物质相关的纠缠相互作用。这种相互作用赋予了空间以灵活性，并将其与引力联系起来。

这一发现表明空间本身是深刻的量子性的，引力则源于量子编码的不完美性。尽管目前仍处于概念验证阶段，但这一框架为发展完整的量子引力理论以及未来在量子计算机上模拟引力现象提供了关键方向。

---

## 7. The Smart TV in Your LivingRoom Is a Node in the AIScraping Economy

**原文标题**: The Smart TV in Your LivingRoom Is a Node in the AIScraping Economy

**原文链接**: [https://blog.includesecurity.com/2026/06/the-smart-tv-in-your-livingroom-is-a-node-in-the-aiscraping-economy/](https://blog.includesecurity.com/2026/06/the-smart-tv-in-your-livingroom-is-a-node-in-the-aiscraping-economy/)

生成摘要时出错

---

## 8. Hacker News, Sans AI

**原文标题**: Hacker News, Sans AI

**原文链接**: [https://elijahpotter.dev/articles/hacker-news-sans-AI](https://elijahpotter.dev/articles/hacker-news-sans-AI)

生成摘要时出错

---

## 9. WSL 2 正在获得更快的 Windows 文件系统访问

**原文标题**: WSL 2 is getting faster Windows file system access

**原文链接**: [https://www.boxofcables.dev/wsl2-per-device-swiotlb-pools-for-virtiofs-and-virtioproxy/](https://www.boxofcables.dev/wsl2-per-device-swiotlb-pools-for-virtiofs-and-virtioproxy/)

WSL 2 is significantly improving cross-OS file system access, crucial for workflows spanning Windows and Linux. WSL 1 initially provided fast Windows drive access via DrvFs. WSL 2, with its Hyper-V VM architecture, shifted to Plan 9 (9P) over Hyper-V sockets, which incurred protocol overhead.

Around 2021, virtiofs was introduced as an experimental opt-in, using VirtIO transport for shared-memory access to reduce serialization overhead compared to 9P. The latest major enhancement, merged in May 2026, addresses a critical bottleneck in the DMA layer. Previously, all virtio devices (like virtiofs mounts and network adapters) shared a single global DMA pool (SWIOTLB), causing contention during heavy I/O. PR #40654 now allocates a dedicated DMA pool for each virtio device, eliminating this shared queue contention.

This fix dramatically benefits file-heavy cross-OS workloads, such as building projects located on a Windows drive within Linux (e.g., `npm install` on `/mnt/c`). VirtioProxy networking also benefits.

To utilize these improvements, users must enable `virtiofs=true` in their `.wslconfig`, update to the latest pre-release WSL kernel (Microsoft.WSL.Kernel 6.18.26.3-1), and ensure their WSL 2 session has over 1 GB of RAM. While virtiofs remains opt-in (9P is still the default), these ongoing efforts are continuously narrowing the performance gap for cross-OS file operations.

---

## 10. Nvidia is proposing a beast of a CPU system for Windows PCs

**原文标题**: Nvidia is proposing a beast of a CPU system for Windows PCs

**原文链接**: [https://twitter.com/lemire/status/2062880075117113739](https://twitter.com/lemire/status/2062880075117113739)

生成摘要时出错

---

## 11. The Causes of Long Covid

**原文标题**: The Causes of Long Covid

**原文链接**: [https://www.science.org/content/blog-post/causes-long-covid](https://www.science.org/content/blog-post/causes-long-covid)

生成摘要时出错

---

## 12. Pre-Modern Armies for Worldbuilders, Part I: Why They Fight

**原文标题**: Pre-Modern Armies for Worldbuilders, Part I: Why They Fight

**原文链接**: [https://acoup.blog/2026/06/05/collections-pre-modern-armies-for-worldbuilders-part-i-why-they-fight/](https://acoup.blog/2026/06/05/collections-pre-modern-armies-for-worldbuilders-part-i-why-they-fight/)

生成摘要时出错

---

## 13. Lee Kuan Yew's Singapore Story (2023)

**原文标题**: Lee Kuan Yew's Singapore Story (2023)

**原文链接**: [https://www.historytoday.com/archive/feature/lee-kuan-yews-singapore-story](https://www.historytoday.com/archive/feature/lee-kuan-yews-singapore-story)

生成摘要时出错

---

## 14. IPv6 zones in URLs are a mistake

**原文标题**: IPv6 zones in URLs are a mistake

**原文链接**: [https://xeiaso.net/notes/2026/ipv6-zones-go-url/](https://xeiaso.net/notes/2026/ipv6-zones-go-url/)

生成摘要时出错

---

## 15. Cloudflare CEO is lying to you about the bot traffic jump

**原文标题**: Cloudflare CEO is lying to you about the bot traffic jump

**原文链接**: [https://www.flyingpenguin.com/cloudflare-ceo-is-lying-to-you-about-the-bot-traffic-jump/](https://www.flyingpenguin.com/cloudflare-ceo-is-lying-to-you-about-the-bot-traffic-jump/)

生成摘要时出错

---

## 16. Show HN: Lowfat – pluggable CLI filter that saved 91.8% of my LLM tokens

**原文标题**: Show HN: Lowfat – pluggable CLI filter that saved 91.8% of my LLM tokens

**原文链接**: [https://github.com/zdk/lowfat](https://github.com/zdk/lowfat)

生成摘要时出错

---

## 17. The perils of UUID primary keys in SQLite

**原文标题**: The perils of UUID primary keys in SQLite

**原文链接**: [https://andersmurphy.com/2026/06/05/the-perils-of-uuid-primary-keys-in-sqlite.html](https://andersmurphy.com/2026/06/05/the-perils-of-uuid-primary-keys-in-sqlite.html)

生成摘要时出错

---

## 18. Transformers are inherently succinct

**原文标题**: Transformers are inherently succinct

**原文链接**: [https://openreview.net/pdf?id=Yxz92UuPLQ](https://openreview.net/pdf?id=Yxz92UuPLQ)

生成摘要时出错

---

## 19. The back cover of C++: The Language raises questions not answered by front cover

**原文标题**: The back cover of C++: The Language raises questions not answered by front cover

**原文链接**: [https://devblogs.microsoft.com/oldnewthing/20260605-01/?p=112391](https://devblogs.microsoft.com/oldnewthing/20260605-01/?p=112391)

生成摘要时出错

---

## 20. Iran Shock Jolts Asia and Europe to Speed Up Energy Transition

**原文标题**: Iran Shock Jolts Asia and Europe to Speed Up Energy Transition

**原文链接**: [https://www.bloomberg.com/graphics/2026-energy-transition-iran-war/](https://www.bloomberg.com/graphics/2026-energy-transition-iran-war/)

生成摘要时出错

---

## 21. Accidentally deleted subscriptions for chat integrations (Slack and MS Teams)

**原文标题**: Accidentally deleted subscriptions for chat integrations (Slack and MS Teams)

**原文链接**: [https://www.githubstatus.com/incidents/2nmfnbknhlnv](https://www.githubstatus.com/incidents/2nmfnbknhlnv)

生成摘要时出错

---

## 22. The IsUpMap lets you check the status of over 100 major sites at once

**原文标题**: The IsUpMap lets you check the status of over 100 major sites at once

**原文链接**: [https://isupmap.com/](https://isupmap.com/)

生成摘要时出错

---

## 23. Zeroserve: A zero-config web server you can script with eBPF

**原文标题**: Zeroserve: A zero-config web server you can script with eBPF

**原文链接**: [https://su3.io/posts/introducing-zeroserve](https://su3.io/posts/introducing-zeroserve)

生成摘要时出错

---

## 24. Zig Zen Update

**原文标题**: Zig Zen Update

**原文链接**: [https://codeberg.org/ziglang/zig/commit/621844bde551ee1a9b8142d7d146d1fa804247a2](https://codeberg.org/ziglang/zig/commit/621844bde551ee1a9b8142d7d146d1fa804247a2)

生成摘要时出错

---

## 25. The Pentagon is running an AI propaganda mill targeting Latin America

**原文标题**: The Pentagon is running an AI propaganda mill targeting Latin America

**原文链接**: [https://theintercept.com/2026/06/02/la-tilde-propaganda-latin-america-pentagon/](https://theintercept.com/2026/06/02/la-tilde-propaganda-latin-america-pentagon/)

生成摘要时出错

---

## 26. Police in England and Wales told to halt AI use in court statements

**原文标题**: Police in England and Wales told to halt AI use in court statements

**原文链接**: [https://www.ft.com/content/229e5949-3ebc-4151-8a86-a01b5e259241](https://www.ft.com/content/229e5949-3ebc-4151-8a86-a01b5e259241)

生成摘要时出错

---

## 27. U.S. Military Turned GPS into a Global "Numbers Station"

**原文标题**: U.S. Military Turned GPS into a Global "Numbers Station"

**原文链接**: [https://www.404media.co/the-u-s-military-quietly-turned-gps-into-a-global-numbers-station-evidence-suggests/](https://www.404media.co/the-u-s-military-quietly-turned-gps-into-a-global-numbers-station-evidence-suggests/)

生成摘要时出错

---

## 28. Aging and Eye Problems

**原文标题**: Aging and Eye Problems

**原文链接**: [https://ldstephens.net/posts/aging-and-eye-problems/](https://ldstephens.net/posts/aging-and-eye-problems/)

生成摘要时出错

---

## 29. The Quiet Numbers Station: Decoding Nineteen Years of GPS Cryptography

**原文标题**: The Quiet Numbers Station: Decoding Nineteen Years of GPS Cryptography

**原文链接**: [https://www.benthamsgaze.org/2026/06/02/the-quiet-numbers-station-decoding-nineteen-years-of-gps-cryptography/](https://www.benthamsgaze.org/2026/06/02/the-quiet-numbers-station-decoding-nineteen-years-of-gps-cryptography/)

生成摘要时出错

---

## 30. Python JIT project was asked to pause development

**原文标题**: Python JIT project was asked to pause development

**原文链接**: [https://discuss.python.org/t/an-announcement-from-the-steering-council-regarding-the-jit-project/107638](https://discuss.python.org/t/an-announcement-from-the-steering-council-regarding-the-jit-project/107638)

生成摘要时出错

---

## 31. Benchmarks in Leipzig

**原文标题**: Benchmarks in Leipzig

**原文链接**: [https://arxiv.org/abs/2606.05818](https://arxiv.org/abs/2606.05818)

生成摘要时出错

---

## 32. Queen bees emerge from special wax chambers

**原文标题**: Queen bees emerge from special wax chambers

**原文链接**: [https://cen.acs.org/materials/biobased-materials/queen-bees-special-wax/104/web/2026/06](https://cen.acs.org/materials/biobased-materials/queen-bees-special-wax/104/web/2026/06)

生成摘要时出错

---

## 33. Communication on European Tech Sovereignty, and an EU Open-Source Strategy

**原文标题**: Communication on European Tech Sovereignty, and an EU Open-Source Strategy

**原文链接**: [https://digital-strategy.ec.europa.eu/en/library/communication-european-tech-sovereignty-accompanied-eu-open-source-strategy](https://digital-strategy.ec.europa.eu/en/library/communication-european-tech-sovereignty-accompanied-eu-open-source-strategy)

生成摘要时出错

---

## 34. US House lawmakers release draft bill to prohibit state AI rules

**原文标题**: US House lawmakers release draft bill to prohibit state AI rules

**原文链接**: [https://www.reuters.com/business/us-house-lawmakers-release-draft-bill-regulate-ai-2026-06-04/](https://www.reuters.com/business/us-house-lawmakers-release-draft-bill-regulate-ai-2026-06-04/)

生成摘要时出错

---

## 35. NSA using Anthropic's Mythos for cyber attacks

**原文标题**: NSA using Anthropic's Mythos for cyber attacks

**原文链接**: [https://www.ft.com/content/d02d91b3-2636-454e-9442-dc7e69f51815](https://www.ft.com/content/d02d91b3-2636-454e-9442-dc7e69f51815)

生成摘要时出错

---

## 36. Show HN: FFmpeg WebCLI – Full FFmpeg in Browser, Offline PWA, No Uploads(WASM)

**原文标题**: Show HN: FFmpeg WebCLI – Full FFmpeg in Browser, Offline PWA, No Uploads(WASM)

**原文链接**: [https://github.com/tejaswigowda/ffmpeg-webCLI](https://github.com/tejaswigowda/ffmpeg-webCLI)

生成摘要时出错

---

## 37. Lockdown Mode

**原文标题**: Lockdown Mode

**原文链接**: [https://help.openai.com/en/articles/20001061-lockdown-mode](https://help.openai.com/en/articles/20001061-lockdown-mode)

生成摘要时出错

---

## 38. Google to pay SpaceX $920M a month for compute capacity at xAI data centers

**原文标题**: Google to pay SpaceX $920M a month for compute capacity at xAI data centers

**原文链接**: [https://www.cnbc.com/2026/06/05/google-to-pay-spacex-920-million-a-month-for-xai-compute-capacity.html](https://www.cnbc.com/2026/06/05/google-to-pay-spacex-920-million-a-month-for-xai-compute-capacity.html)

生成摘要时出错

---

## 39. Meta confirms 1000s of Instagram accounts were hacked by abusing its AI chatbot

**原文标题**: Meta confirms 1000s of Instagram accounts were hacked by abusing its AI chatbot

**原文链接**: [https://this.weekinsecurity.com/meta-confirms-thousands-of-instagram-accounts-were-hacked-by-abusing-its-ai-chatbot/](https://this.weekinsecurity.com/meta-confirms-thousands-of-instagram-accounts-were-hacked-by-abusing-its-ai-chatbot/)

生成摘要时出错

---

## 40. Show HN: Formally verified polygon intersection – Opus 4.8 oneshots, prev failed

**原文标题**: Show HN: Formally verified polygon intersection – Opus 4.8 oneshots, prev failed

**原文链接**: [https://github.com/schildep/verified-polygon-intersection](https://github.com/schildep/verified-polygon-intersection)

生成摘要时出错

---

## 41. New York just passed a one-year temporary ban on data centers

**原文标题**: New York just passed a one-year temporary ban on data centers

**原文链接**: [https://scienceaim.com/new-york-just-passed-a-one-year-temporary-ban-on-data-centers/](https://scienceaim.com/new-york-just-passed-a-one-year-temporary-ban-on-data-centers/)

生成摘要时出错

---

## 42. Valve says it's ready to launch the Steam Machine this summer

**原文标题**: Valve says it's ready to launch the Steam Machine this summer

**原文链接**: [https://www.theverge.com/games/943657/valve-steam-machine-frame-summer-launch-verified](https://www.theverge.com/games/943657/valve-steam-machine-frame-summer-launch-verified)

生成摘要时出错

---

## 43. The company I work for is losing all of its humanity, I don't know where to go

**原文标题**: The company I work for is losing all of its humanity, I don't know where to go

**原文链接**: [https://superlemon.bearblog.dev/the-company-i-work-for-is-losing-all-of-its-humanity-but-i-dont-know-where-else-to-go/](https://superlemon.bearblog.dev/the-company-i-work-for-is-losing-all-of-its-humanity-but-i-dont-know-where-else-to-go/)

生成摘要时出错

---

## 44. Dear Microsoft, enough is enough

**原文标题**: Dear Microsoft, enough is enough

**原文链接**: [https://www.politico.eu/sponsored-content/dear-microsoft-enough-is-enough/](https://www.politico.eu/sponsored-content/dear-microsoft-enough-is-enough/)

生成摘要时出错

---

## 45. Let's celebrate work that is 100% human-made

**原文标题**: Let's celebrate work that is 100% human-made

**原文链接**: [https://www.human-made.work/](https://www.human-made.work/)

生成摘要时出错

---

## 46. Do we need billionaires?

**原文标题**: Do we need billionaires?

**原文链接**: [https://bjhess.com/posts/do-we-need-billionaires](https://bjhess.com/posts/do-we-need-billionaires)

生成摘要时出错

---

## 47. Mantine-datatable (and others) compromised – owner account suspended

**原文标题**: Mantine-datatable (and others) compromised – owner account suspended

**原文链接**: [https://github.com/icflorescu/mantine-datatable/discussions/813](https://github.com/icflorescu/mantine-datatable/discussions/813)

生成摘要时出错

---

## 48. Microsoft wants users to be addicted to Scout, their AI personal assistant

**原文标题**: Microsoft wants users to be addicted to Scout, their AI personal assistant

**原文链接**: [https://disassociated.com/microsoft-users-addicted-ai-personal-assistant/](https://disassociated.com/microsoft-users-addicted-ai-personal-assistant/)

生成摘要时出错

---

## 49. Azure Linux Desktop

**原文标题**: Azure Linux Desktop

**原文链接**: [https://www.boxofcables.dev/azure-linux-desktop-a-build-2026-mashup-of-wslc-winui-reactor-and-azure-linux-4-0/](https://www.boxofcables.dev/azure-linux-desktop-a-build-2026-mashup-of-wslc-winui-reactor-and-azure-linux-4-0/)

生成摘要时出错

---

## 50. Leak Reveals Microsoft Wants Its AI to Be 'Addictive'

**原文标题**: Leak Reveals Microsoft Wants Its AI to Be 'Addictive'

**原文链接**: [https://kotaku.com/microsoft-ai-scout-addictive-satya-nadella-404-media-copilot-2000702924](https://kotaku.com/microsoft-ai-scout-addictive-satya-nadella-404-media-copilot-2000702924)

生成摘要时出错

---

## 51. Delacroix's Entry of the Crusaders into Constantinople Restored

**原文标题**: Delacroix's Entry of the Crusaders into Constantinople Restored

**原文链接**: [https://www.louvre.fr/en/explore/life-at-the-museum/delacroix-s-entry-of-the-crusaders-into-constantinople-restored-to-its-original-glory](https://www.louvre.fr/en/explore/life-at-the-museum/delacroix-s-entry-of-the-crusaders-into-constantinople-restored-to-its-original-glory)

生成摘要时出错

---

## 52. Magenta RealTime 2: Open and Local Live Music Models

**原文标题**: Magenta RealTime 2: Open and Local Live Music Models

**原文链接**: [https://magenta.withgoogle.com/magenta-realtime-2](https://magenta.withgoogle.com/magenta-realtime-2)

生成摘要时出错

---

## 53. Introduction – Rust for Python Programmers

**原文标题**: Introduction – Rust for Python Programmers

**原文链接**: [https://microsoft.github.io/RustTraining/python-book/](https://microsoft.github.io/RustTraining/python-book/)

生成摘要时出错

---

## 54. Castor: CERN Advanced STORage Manager

**原文标题**: Castor: CERN Advanced STORage Manager

**原文链接**: [https://castor.web.cern.ch/content/home.html](https://castor.web.cern.ch/content/home.html)

生成摘要时出错

---

## 55. Show HN: Mercek – A Desktop IDE for AWS ECS

**原文标题**: Show HN: Mercek – A Desktop IDE for AWS ECS

**原文链接**: [https://www.mercek.dev/](https://www.mercek.dev/)

生成摘要时出错

---

## 56. The new bibliomaniacs

**原文标题**: The new bibliomaniacs

**原文链接**: [https://engelsbergideas.com/notebook/the-new-bibliomaniacs/](https://engelsbergideas.com/notebook/the-new-bibliomaniacs/)

生成摘要时出错

---

## 57. Meta Keeps Delaying the Release of Its New AI Model to Developers

**原文标题**: Meta Keeps Delaying the Release of Its New AI Model to Developers

**原文链接**: [https://www.wsj.com/tech/ai/meta-keeps-delaying-the-release-of-its-new-ai-model-to-developers-f8569c8c](https://www.wsj.com/tech/ai/meta-keeps-delaying-the-release-of-its-new-ai-model-to-developers-f8569c8c)

生成摘要时出错

---

## 58. Technical Interviews Reject the Wrong Engineers

**原文标题**: Technical Interviews Reject the Wrong Engineers

**原文链接**: [https://fagnerbrack.com/technical-interviews-reject-the-wrong-engineers-a8e78ca04b2e](https://fagnerbrack.com/technical-interviews-reject-the-wrong-engineers-a8e78ca04b2e)

生成摘要时出错

---

## 59. Linear Cosine Palettes(2025)

**原文标题**: Linear Cosine Palettes(2025)

**原文链接**: [https://blog.djnavarro.net/posts/2025-09-14_cosine-palettes/](https://blog.djnavarro.net/posts/2025-09-14_cosine-palettes/)

生成摘要时出错

---

## 60. Nordstjernen 1.0

**原文标题**: Nordstjernen 1.0

**原文链接**: [https://github.com/nordstjernen-web/nordstjernen/releases/tag/1.0.0](https://github.com/nordstjernen-web/nordstjernen/releases/tag/1.0.0)

生成摘要时出错

---

## 61. You Can Run

**原文标题**: You Can Run

**原文链接**: [https://magazine.atavist.com/2026/mccann-cocaine-fugitives](https://magazine.atavist.com/2026/mccann-cocaine-fugitives)

生成摘要时出错

---

## 62. Running Python code in a sandbox with MicroPython and WASM

**原文标题**: Running Python code in a sandbox with MicroPython and WASM

**原文链接**: [https://simonwillison.net/2026/Jun/6/micropython-in-a-sandbox/](https://simonwillison.net/2026/Jun/6/micropython-in-a-sandbox/)

生成摘要时出错

---

## 63. Neocities domain suspended by Namecheap for unrelated court case

**原文标题**: Neocities domain suspended by Namecheap for unrelated court case

**原文链接**: [https://bsky.app/profile/neocities.org/post/3mnkqgxostk2k](https://bsky.app/profile/neocities.org/post/3mnkqgxostk2k)

生成摘要时出错

---

## 64. Adyen Selected as Payment Services Provider for GOV.UK Pay

**原文标题**: Adyen Selected as Payment Services Provider for GOV.UK Pay

**原文链接**: [https://www.adyen.com/press-and-media/adyen-payments-gov-uk](https://www.adyen.com/press-and-media/adyen-payments-gov-uk)

生成摘要时出错

---

## 65. Ntsc-rs – open-source video emulation of analog TV and VHS artifacts

**原文标题**: Ntsc-rs – open-source video emulation of analog TV and VHS artifacts

**原文链接**: [https://ntsc.rs/](https://ntsc.rs/)

生成摘要时出错

---

## 66. S&P Global keeps fast index entry rules unchanged as SpaceX listing looms

**原文标题**: S&P Global keeps fast index entry rules unchanged as SpaceX listing looms

**原文链接**: [https://www.reuters.com/business/finance/sp-global-keeps-fast-entry-proposal-unchanged-spacex-listing-looms-2026-06-04/](https://www.reuters.com/business/finance/sp-global-keeps-fast-entry-proposal-unchanged-spacex-listing-looms-2026-06-04/)

生成摘要时出错

---

## 67. I Must Attempt to Explain the Lego Scandal Rocking YouTube State of Utah

**原文标题**: I Must Attempt to Explain the Lego Scandal Rocking YouTube State of Utah

**原文链接**: [https://www.404media.co/the-lego-bricks-and-minifigs-reckless-benyoutube-scandal-has-broken-containment-can-no-longer-be-ignored/](https://www.404media.co/the-lego-bricks-and-minifigs-reckless-benyoutube-scandal-has-broken-containment-can-no-longer-be-ignored/)

生成摘要时出错

---

## 68. CEO to staff: You're not getting a raise. We're spending on AI instead

**原文标题**: CEO to staff: You're not getting a raise. We're spending on AI instead

**原文链接**: [https://www.businessinsider.com/teradata-pauses-raises-employee-compensation-ai-budget-2026-6](https://www.businessinsider.com/teradata-pauses-raises-employee-compensation-ai-budget-2026-6)

生成摘要时出错

---

## 69. What happens if Japan takes in zero immigrants?

**原文标题**: What happens if Japan takes in zero immigrants?

**原文链接**: [https://www.konichivalue.com/p/what-happens-if-japan-takes-in-zero](https://www.konichivalue.com/p/what-happens-if-japan-takes-in-zero)

生成摘要时出错

---

## 70. Microsoft Compromised Again. Shuts Down Azure Function GitHub Actions

**原文标题**: Microsoft Compromised Again. Shuts Down Azure Function GitHub Actions

**原文链接**: [https://opensourcemalware.com/blog/miasma-reaches-azure](https://opensourcemalware.com/blog/miasma-reaches-azure)

生成摘要时出错

---

## 71. SpaceX: Flying High on Impunity

**原文标题**: SpaceX: Flying High on Impunity

**原文链接**: [https://georgiebc.wordpress.com/2026/06/01/flying-high-on-impunity/](https://georgiebc.wordpress.com/2026/06/01/flying-high-on-impunity/)

生成摘要时出错

---

## 72. White House will dump $700M of public funds into costly, unreliable coal again

**原文标题**: White House will dump $700M of public funds into costly, unreliable coal again

**原文链接**: [https://electrek.co/2026/06/04/white-house-will-dump-700m-of-public-funds-into-costly-unreliable-coal-again/](https://electrek.co/2026/06/04/white-house-will-dump-700m-of-public-funds-into-costly-unreliable-coal-again/)

生成摘要时出错

---

## 73. Texas is America Inc's new centre of gravity

**原文标题**: Texas is America Inc's new centre of gravity

**原文链接**: [https://economist.com/business/2026/05/31/texas-is-america-incs-new-centre-of-gravity](https://economist.com/business/2026/05/31/texas-is-america-incs-new-centre-of-gravity)

生成摘要时出错

---

## 74. Do women’s mate preferences change across the ovulatory cycle? (2014) [pdf]

**原文标题**: Do women’s mate preferences change across the ovulatory cycle? (2014) [pdf]

**原文链接**: [https://www.martiehaselton.com/_files/ugd/3ae410_aeb76edab75f457aae0c14c4c68d93c0.pdf](https://www.martiehaselton.com/_files/ugd/3ae410_aeb76edab75f457aae0c14c4c68d93c0.pdf)

生成摘要时出错

---

## 75. Google Buying Computing from SpaceX in $920M-a-Month Deal

**原文标题**: Google Buying Computing from SpaceX in $920M-a-Month Deal

**原文链接**: [https://www.bloomberg.com/news/articles/2026-06-05/google-buying-computing-from-spacex-in-920-million-a-month-deal](https://www.bloomberg.com/news/articles/2026-06-05/google-buying-computing-from-spacex-in-920-million-a-month-deal)

生成摘要时出错

---

## 76. Fake Money Built America

**原文标题**: Fake Money Built America

**原文链接**: [https://mail.blockworks.com/p/how-fake-money-built-america](https://mail.blockworks.com/p/how-fake-money-built-america)

生成摘要时出错

---

## 77. AI will consume as much water in 2030 as 1.3B people

**原文标题**: AI will consume as much water in 2030 as 1.3B people

**原文链接**: [https://english.elpais.com/technology/2026-06-03/ai-will-consume-as-much-water-in-2030-as-13-billion-people.html](https://english.elpais.com/technology/2026-06-03/ai-will-consume-as-much-water-in-2030-as-13-billion-people.html)

生成摘要时出错

---

## 78. ZEC drops 30% as Shielded Labs reveals more about infinite counterfeit bug

**原文标题**: ZEC drops 30% as Shielded Labs reveals more about infinite counterfeit bug

**原文链接**: [https://cointelegraph.com/news/zec-tanks-30-after-ai-security-review-discovers-critical-zcash-vulnerability](https://cointelegraph.com/news/zec-tanks-30-after-ai-security-review-discovers-critical-zcash-vulnerability)

生成摘要时出错

---

## 79. Show HN: ABC Classic 100 Rankings visualised

**原文标题**: Show HN: ABC Classic 100 Rankings visualised

**原文链接**: [https://classic100.gotski.workers.dev/](https://classic100.gotski.workers.dev/)

生成摘要时出错

---

## 80. There's still no point in gigabit broadband

**原文标题**: There's still no point in gigabit broadband

**原文链接**: [https://shkspr.mobi/blog/2026/06/theres-still-no-point-in-gigabit-broadband/](https://shkspr.mobi/blog/2026/06/theres-still-no-point-in-gigabit-broadband/)

生成摘要时出错

---

## 81. P/E Tells You the Price. Reality Gap Tells You the Delusion

**原文标题**: P/E Tells You the Price. Reality Gap Tells You the Delusion

**原文链接**: [https://hstre.github.io/Reality-Gap/](https://hstre.github.io/Reality-Gap/)

生成摘要时出错

---

## 82. Tribute to Jiro Yamada, Automotive Artist (1960-2025) [video]

**原文标题**: Tribute to Jiro Yamada, Automotive Artist (1960-2025) [video]

**原文链接**: [https://www.youtube.com/watch?v=rJ2gQ5Md60U](https://www.youtube.com/watch?v=rJ2gQ5Md60U)

生成摘要时出错

---

## 83. Jolt: Clojure Interpreter on Janet

**原文标题**: Jolt: Clojure Interpreter on Janet

**原文链接**: [https://github.com/yogthos/jolt/](https://github.com/yogthos/jolt/)

生成摘要时出错

---

## 84. Documentary, "C++: The Most Consequential Programming Language"

**原文标题**: Documentary, "C++: The Most Consequential Programming Language"

**原文链接**: [https://www.youtube.com/watch?v=lI7tMxzSJ7w](https://www.youtube.com/watch?v=lI7tMxzSJ7w)

生成摘要时出错

---

## 85. Investigation: Russian censorship systems (TMCT) expose Chinese DPI signatures

**原文标题**: Investigation: Russian censorship systems (TMCT) expose Chinese DPI signatures

**原文链接**: [https://freenet.monster/china-unicom.html?lang=en](https://freenet.monster/china-unicom.html?lang=en)

生成摘要时出错

---

## 86. Meta Silently Added Face-Recognition for Its Smart Glasses to Phones

**原文标题**: Meta Silently Added Face-Recognition for Its Smart Glasses to Phones

**原文链接**: [https://www.wired.com/story/meta-smart-glasses-face-recognition-nametag-connections/](https://www.wired.com/story/meta-smart-glasses-face-recognition-nametag-connections/)

生成摘要时出错

---

## 87. Alzheimer's patient gets back speech, bladder control and memory in drug trial

**原文标题**: Alzheimer's patient gets back speech, bladder control and memory in drug trial

**原文链接**: [https://nypost.com/2026/06/04/health/alzheimers-patient-recovers-speech-continence-and-memory-with-this-drug/](https://nypost.com/2026/06/04/health/alzheimers-patient-recovers-speech-continence-and-memory-with-this-drug/)

生成摘要时出错

---

