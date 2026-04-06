# Hacker News 热门文章摘要 (2026-04-06)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 威胁在于安逸地滑向对自身所为一无所知。

**原文标题**: The threat is comfortable drift toward not understanding what you're doing

**原文链接**: [https://ergosphere.blog/posts/the-machines-are-fine/](https://ergosphere.blog/posts/the-machines-are-fine/)

文章《威胁在于安逸地滑向对自身所为的不知所云》指出，人工智能在学术界的主要危险并非机器本身，而是对人类理解力的侵蚀。作者用一个比喻阐明了这一点：爱丽丝通过传统的刻苦学习掌握了天体物理学，建立了深厚的内在知识，而鲍勃使用AI代理进行总结、调试和写作，也产出了一篇同样可以发表的论文，但却缺乏真正的理解。侧重于产出的学术评估标准无法区分这两种情况，从而助长了权宜之计，而非智力发展。

作者断言，对于天体物理学等领域，真正的价值在于人类的发现过程和对思维的培养，而不仅仅是结果。一项实验表明，AI可以生成一篇可发表的论文，但仅限于在一位专家的严格监督下，这位专家凭借其深厚的理解力捕捉到了AI的“幻觉”和错误。更强大的AI模型并不会消除对这种人类专业知识的需求；它们只会拓宽*受监督*代理的应用范围，从而使人类理解力的缺失更难被察觉。

作者驳斥了关于AI的极端立场，并将真正的威胁定义为“缓慢而舒适地滑向对自身所为的不知所云”。这会造就那些能产出结果却缺乏基础理解的研究人员，他们只知道“要按哪些按钮，却不知道这些按钮为何存在”。科学的核心，即成为一个独立思考者的缓慢而往往痛苦的过程，是唯一真正不可替代的部分；如果为了追求更快的产出而绕过这一过程，就可能失去“科学的伟大之处”。作者作为一名AI用户，强调有效利用AI仍然需要事先具备人类的理解力。

---

## 2. 八年夙愿，三个月AI构建

**原文标题**: Eight years of wanting, three months of building with AI

**原文链接**: [https://lalitm.com/post/building-syntaqlite-ai/](https://lalitm.com/post/building-syntaqlite-ai/)

经过八年夙愿和三个月（250小时）的投入，作者发布了“syntaqlite”，一套高质量的SQLite开发工具，并将其创建主要归因于AI编码代理。该项目解决了长期以来开源SQLite工具（特别是PerfettoSQL）不足的痛点。构建它充满挑战，因为SQLite独特且未明确规范的C语言解析器，使得一个独立开发者完成这项工作“既困难又繁琐”。

最初，在1月份，作者与Claude Code进行了“凭直觉编码”，将大部分设计和实现工作委托给它。尽管这验证了方法并生成了大量测试，但却导致了一个“一团乱麻的代码库”。作者随后放弃了它，用Rust重写，并采取了严谨的方法，完全掌握了所有权，并将AI用作特定任务的“超级自动补全”。

AI通过提供具体的问题和原型，在克服惰性方面发挥了宝贵作用。它加速了显而易见任务的代码生成，并促进了持续重构。作为一名“助教”，AI协助进行研究（例如：代码美化），并快速学习Rust工具链和编辑器扩展API等新领域，使项目能够包含编辑器扩展和WASM游乐场等“长尾”功能，从而提高了其完整性和用户体验。

然而，使用AI也付出了代价。作者体验到一种类似老虎机的“上瘾”，导致疲劳时陷入低效的提示循环。更重要的是，过度委托导致他“脱离”了代码库的复杂细节，阻碍了调试以及与AI代理的有效沟通。最终，AI使该项目得以实现并变得全面，但需要仔细、亲力亲为的指导来管理其弊端。

---

## 3. 何必用多代币，少代币就搞定。

**原文标题**: Caveman: Why use many token when few token do trick

**原文链接**: [https://github.com/JuliusBrussee/caveman](https://github.com/JuliusBrussee/caveman)

“Caveman”是一款用于LLM代理（如Claude Code和Codex）的工具和插件，它通过让AI“像穴居人一样说话”来显著减少token使用量——平均削减65%的输出token，同时保持完整的技术准确性。

该工具通过消除填充词、冠词、客套话和模糊措辞来发挥作用，但它一丝不苟地保留了代码块、技术术语和精确的错误信息。这种“话少，但脑子不小”的方法带来了更快的响应速度（最高可达3倍），通过消除“大段文字”提高了可读性，并显著节省了成本。用户可以通过“Lite”、“Full”和“Ultra”强度级别来调整压缩程度。基准测试表明，在各种技术任务中，token节省量介于22%到87%之间。

一个配套工具“Caveman Compress”则处理输入token。它将项目内存文件（例如CLAUDE.md）重写成“穴居人”风格的语言，平均节省了每次会话加载的45%的token。这种压缩只针对自然语言散文，保留了代码、URL、标题和其他技术结构不变，同时还保留了一个人类可读的原始版本。

安装通过`npx skills add`或相应的插件系统进行，非常简单。通过结合用于输出的“Caveman”和用于输入的“Caveman Compress”，用户可以在整个LLM对话中实现全面的token节省，从而提高效率并降低成本。

---

## 4. Gemma 4 在 iPhone 上

**原文标题**: Gemma 4 on iPhone

**原文链接**: [https://apps.apple.com/nl/app/google-ai-edge-gallery/id6749645337](https://apps.apple.com/nl/app/google-ai-edge-gallery/id6749645337)

Gemma 4 已作为一次重大更新发布，为用户带来了最新的高性能模型。其一个主要特点是能够完全离线运行。此外，Gemma 4 还引入了新功能：“思考模式”和“代理技能”。

---

## 5. Show HN: 我做了一个小型LLM来揭秘语言模型的工作原理

**原文标题**: Show HN: I built a tiny LLM to demystify how language models work

**原文链接**: [https://github.com/arman-bd/guppylm](https://github.com/arman-bd/guppylm)

GuppyLM是一个拥有约900万参数的大型语言模型 (LLM)，旨在揭秘语言模型，证明训练一个LLM无需博士学位或庞大GPU集群也能实现。用户可以在单个Colab T4 GPU上，仅需5分钟从零开始训练一个功能性LLM，涵盖数据生成、分词器、架构、训练和推理。该项目旨在使LLM的内部运作透明化，展示原始文本如何转化为训练好的权重和生成的输出。

GuppyLM本身就具象化为一条名为Guppy的小鱼，以简短的小写句子谈论水、食物和鱼缸生活，刻意避免人类的抽象概念。其架构是一个简单的“香草”Transformer，拥有6层，384个隐藏维度，一个4096个词元（token）的BPE词汇表，以及128个词元的最大序列长度。它在60个以鱼为中心的主题上，通过6万次合成对话进行训练。

关键设计选择包括将个性直接融入权重（无系统提示），由于其128个词元的上下文窗口，仅支持单轮对话，以及在其小规模下为保持清晰和效率而采用简单的Transformer。合成数据集确保了一致的、鱼类般的个性。用户可以与预训练模型聊天，或训练自己的模型，训练出的模型足够小，可以在浏览器中运行。

---

## 6. 微软有多少产品名为'Copilot'？

**原文标题**: How many products does Microsoft have named 'Copilot'?

**原文链接**: [https://teybannerman.com/strategy/2026/03/31/how-many-microsoft-copilot-are-there.html](https://teybannerman.com/strategy/2026/03/31/how-many-microsoft-copilot-are-there.html)

The article details the author's challenge in explaining "Microsoft Copilot" due to the name referring to a vast and diverse array of products and features. Initially, the author identified at least 75 different "Copilots," a number later updated to 80 after the community pointed out omissions like Gaming Copilot and Microsoft Dragon Copilot.

The term "Copilot" now encompasses everything from apps, features, and platforms to a dedicated keyboard key, an entire category of laptops, and even a tool designed for building more Copilots. The author found no single comprehensive list, not even from Microsoft's own sources, prompting them to piece together this information from product pages, launch announcements, and marketing materials.

To illustrate the complexity, the author created an interactive visualization mapping all 80 "Copilots," grouped by category, but admitted they could not find any discernible pattern in Microsoft's naming convention. The piece highlights the significant fragmentation and potential user confusion surrounding the "Copilot" brand across Microsoft's ecosystem.

---

## 7. 微软自 Petzold 以来就没有连贯的 GUI 策略。

**原文标题**: Microsoft hasn't had a coherent GUI strategy since Petzold

**原文链接**: [https://www.jsnover.com/blog/2026/03/13/microsoft-hasnt-had-a-coherent-gui-strategy-since-petzold/](https://www.jsnover.com/blog/2026/03/13/microsoft-hasnt-had-a-coherent-gui-strategy-since-petzold/)

生成摘要时出错

---

## 8. 为什么瑞士有25 Gbit互联网而美国没有

**原文标题**: Why Switzerland has 25 Gbit internet and America doesn't

**原文链接**: [https://sschueller.github.io/posts/the-free-market-lie/](https://sschueller.github.io/posts/the-free-market-lie/)

The article "Why Switzerland has 25 Gbit internet and America doesn't" argues that superior internet in Switzerland compared to the US and Germany stems from differing approaches to natural monopolies. Switzerland enjoys 25 Gbit symmetrical fiber internet with multiple providers and dedicated connections, while the US and Germany suffer from slower speeds, limited choices, and often shared infrastructure.

The core concept is a "natural monopoly," where infrastructure costs are high, but serving additional customers is low. The article contends that allowing multiple companies to build redundant infrastructure ("overbuild" in Germany) or establishing territorial monopolies (as in the US) leads to stagnation, high prices, and lack of innovation, rather than true competition.

Switzerland treats its fiber infrastructure as a neutral, shared asset, often publicly or semi-publicly built. Each home receives a dedicated 4-strand Point-to-Point fiber line that terminates in an open hub. This "Layer 1" open access allows any Internet Service Provider (ISP) to connect, fostering genuine competition on service quality and price. Swiss regulators have been instrumental in mandating this open-access standard, even intervening to prevent the incumbent, Swisscom, from switching to a shared (P2MP) model that would have restricted competitor access.

Conversely, the US model fosters territorial monopolies, offering shared P2MP connections with little incentive for incumbents to innovate or lower prices. Germany's focus on infrastructure competition has led to wasteful "overbuild" and incumbent advantages despite heavy regulation.

The article concludes that real capitalism, for natural monopolies like internet infrastructure, requires regulated open access to shared assets to enable genuine competition. It recommends policies such as mandating open access, enforcing Point-to-Point architecture, establishing neutral fiber standards, empowering competition authorities, and supporting municipal fiber to achieve better internet services.

---

## 9. I won't download your app. The web version is a-ok

**原文标题**: I won't download your app. The web version is a-ok

**原文链接**: [https://www.0xsid.com/blog/wont-download-your-app](https://www.0xsid.com/blog/wont-download-your-app)

生成摘要时出错

---

## 10. German implementation of eIDAS will require an Apple/Google account to function

**原文标题**: German implementation of eIDAS will require an Apple/Google account to function

**原文链接**: [https://bmi.usercontent.opencode.de/eudi-wallet/wallet-development-documentation-public/latest/architecture-concept/06-mobile-devices/02-mdvm/](https://bmi.usercontent.opencode.de/eudi-wallet/wallet-development-documentation-public/latest/architecture-concept/06-mobile-devices/02-mdvm/)

生成摘要时出错

---

## 11. France pulls last gold held in US for $15B gain

**原文标题**: France pulls last gold held in US for $15B gain

**原文链接**: [https://www.mining.com/france-pulls-last-gold-held-in-us-for-15b-gain/](https://www.mining.com/france-pulls-last-gold-held-in-us-for-15b-gain/)

生成摘要时出错

---

## 12. Artemis II crew see first glimpse of far side of Moon [video]

**原文标题**: Artemis II crew see first glimpse of far side of Moon [video]

**原文链接**: [https://www.bbc.com/news/videos/ce3d5gkd2geo](https://www.bbc.com/news/videos/ce3d5gkd2geo)

生成摘要时出错

---

## 13. Claude Code is unusable for complex engineering tasks with the Feb updates

**原文标题**: Claude Code is unusable for complex engineering tasks with the Feb updates

**原文链接**: [https://github.com/anthropics/claude-code/issues/42796](https://github.com/anthropics/claude-code/issues/42796)

生成摘要时出错

---

## 14. Employers use your personal data to figure out the lowest salary you'll accept

**原文标题**: Employers use your personal data to figure out the lowest salary you'll accept

**原文链接**: [https://www.marketwatch.com/story/employers-are-using-your-personal-data-to-figure-out-the-lowest-salary-youll-accept-c2b968fb](https://www.marketwatch.com/story/employers-are-using-your-personal-data-to-figure-out-the-lowest-salary-youll-accept-c2b968fb)

生成摘要时出错

---

## 15. AWS engineer reports PostgreSQL perf halved by Linux 7.0, fix may not be easy

**原文标题**: AWS engineer reports PostgreSQL perf halved by Linux 7.0, fix may not be easy

**原文链接**: [https://www.phoronix.com/news/Linux-7.0-AWS-PostgreSQL-Drop](https://www.phoronix.com/news/Linux-7.0-AWS-PostgreSQL-Drop)

生成摘要时出错

---

## 16. Running Gemma 4 locally with LM Studio's new headless CLI and Claude Code

**原文标题**: Running Gemma 4 locally with LM Studio's new headless CLI and Claude Code

**原文链接**: [https://ai.georgeliu.com/p/running-google-gemma-4-locally-with](https://ai.georgeliu.com/p/running-google-gemma-4-locally-with)

生成摘要时出错

---

## 17. Someone at BrowserStack is leaking users' email addresses

**原文标题**: Someone at BrowserStack is leaking users' email addresses

**原文链接**: [https://shkspr.mobi/blog/2026/04/someone-at-browserstack-is-leaking-users-email-address/](https://shkspr.mobi/blog/2026/04/someone-at-browserstack-is-leaking-users-email-address/)

生成摘要时出错

---

## 18. Finnish sauna heat exposure induces stronger immune cell than cytokine responses

**原文标题**: Finnish sauna heat exposure induces stronger immune cell than cytokine responses

**原文链接**: [https://www.tandfonline.com/doi/full/10.1080/23328940.2026.2645467#abstract](https://www.tandfonline.com/doi/full/10.1080/23328940.2026.2645467#abstract)

生成摘要时出错

---

## 19. My Google Workspace account suspension

**原文标题**: My Google Workspace account suspension

**原文链接**: [https://zencapital.substack.com/p/sad-story-of-my-google-workspace](https://zencapital.substack.com/p/sad-story-of-my-google-workspace)

生成摘要时出错

---

## 20. Music for Programming

**原文标题**: Music for Programming

**原文链接**: [https://musicforprogramming.net](https://musicforprogramming.net)

生成摘要时出错

---

## 21. Show HN: I made a YouTube search form with advanced filters

**原文标题**: Show HN: I made a YouTube search form with advanced filters

**原文链接**: [https://playlists.at/youtube/search/](https://playlists.at/youtube/search/)

生成摘要时出错

---

## 22. Age verification as mass surveillance infrastructure

**原文标题**: Age verification as mass surveillance infrastructure

**原文链接**: [https://tboteproject.com/surveillancefindings/](https://tboteproject.com/surveillancefindings/)

生成摘要时出错

---

## 23. 81yo Dodgers fan can no longer get tickets because he doesn't have a smartphone

**原文标题**: 81yo Dodgers fan can no longer get tickets because he doesn't have a smartphone

**原文链接**: [https://twitter.com/Suzierizzo1/status/2040864617467924865](https://twitter.com/Suzierizzo1/status/2040864617467924865)

生成摘要时出错

---

## 24. Lisette a little language inspired by Rust that compiles to Go

**原文标题**: Lisette a little language inspired by Rust that compiles to Go

**原文链接**: [https://lisette.run/](https://lisette.run/)

生成摘要时出错

---

## 25. The 1987 game “The Last Ninja” was 40 kilobytes

**原文标题**: The 1987 game “The Last Ninja” was 40 kilobytes

**原文链接**: [https://twitter.com/exQUIZitely/status/2040777977521398151](https://twitter.com/exQUIZitely/status/2040777977521398151)

生成摘要时出错

---

## 26. What being ripped off taught me

**原文标题**: What being ripped off taught me

**原文链接**: [https://belief.horse/notes/what-being-ripped-off-taught-me/](https://belief.horse/notes/what-being-ripped-off-taught-me/)

生成摘要时出错

---

## 27. The cult of vibe coding is insane

**原文标题**: The cult of vibe coding is insane

**原文链接**: [https://bramcohen.com/p/the-cult-of-vibe-coding-is-insane](https://bramcohen.com/p/the-cult-of-vibe-coding-is-insane)

生成摘要时出错

---

## 28. Show HN: Real-time AI (audio/video in, voice out) on an M3 Pro with Gemma E2B

**原文标题**: Show HN: Real-time AI (audio/video in, voice out) on an M3 Pro with Gemma E2B

**原文链接**: [https://github.com/fikrikarim/parlor](https://github.com/fikrikarim/parlor)

生成摘要时出错

---

## 29. An open-source 240-antenna array to bounce signals off the Moon

**原文标题**: An open-source 240-antenna array to bounce signals off the Moon

**原文链接**: [https://moonrf.com/](https://moonrf.com/)

生成摘要时出错

---

## 30. Introduction to Computer Music (2009) [pdf]

**原文标题**: Introduction to Computer Music (2009) [pdf]

**原文链接**: [https://composerprogrammer.com/introductiontocomputermusic.pdf](https://composerprogrammer.com/introductiontocomputermusic.pdf)

生成摘要时出错

---

## 31. Is Germany's gold safe in New York ?

**原文标题**: Is Germany's gold safe in New York ?

**原文链接**: [https://www.dw.com/en/is-germanys-gold-safe-in-new-york/video-75766873](https://www.dw.com/en/is-germanys-gold-safe-in-new-york/video-75766873)

生成摘要时出错

---

## 32. Battle for Wesnoth: open-source, turn-based strategy game

**原文标题**: Battle for Wesnoth: open-source, turn-based strategy game

**原文链接**: [https://www.wesnoth.org](https://www.wesnoth.org)

生成摘要时出错

---

## 33. Germany Doxes "UNKN," Head of RU Ransomware Gangs REvil, GandCrab

**原文标题**: Germany Doxes "UNKN," Head of RU Ransomware Gangs REvil, GandCrab

**原文链接**: [https://krebsonsecurity.com/2026/04/germany-doxes-unkn-head-of-ru-ransomware-gangs-revil-gandcrab/](https://krebsonsecurity.com/2026/04/germany-doxes-unkn-head-of-ru-ransomware-gangs-revil-gandcrab/)

生成摘要时出错

---

## 34. OpenAI's fall from grace as investors race to Anthropic

**原文标题**: OpenAI's fall from grace as investors race to Anthropic

**原文链接**: [https://www.latimes.com/business/story/2026-04-01/openais-shocking-fall-from-grace-as-investors-race-to-anthropic](https://www.latimes.com/business/story/2026-04-01/openais-shocking-fall-from-grace-as-investors-race-to-anthropic)

生成摘要时出错

---

## 35. Nanocode: The best Claude Code that $200 can buy in pure JAX on TPUs

**原文标题**: Nanocode: The best Claude Code that $200 can buy in pure JAX on TPUs

**原文链接**: [https://github.com/salmanmohammadi/nanocode/discussions/1](https://github.com/salmanmohammadi/nanocode/discussions/1)

生成摘要时出错

---

## 36. Codex pricing to align with API token usage, instead of per-message

**原文标题**: Codex pricing to align with API token usage, instead of per-message

**原文链接**: [https://help.openai.com/en/articles/20001106-codex-rate-card](https://help.openai.com/en/articles/20001106-codex-rate-card)

生成摘要时出错

---

## 37. LibreOffice – Let's put an end to the speculation

**原文标题**: LibreOffice – Let's put an end to the speculation

**原文链接**: [https://blog.documentfoundation.org/blog/2026/04/05/lets-put-an-end-to-the-speculation/](https://blog.documentfoundation.org/blog/2026/04/05/lets-put-an-end-to-the-speculation/)

生成摘要时出错

---

## 38. Media scraper Gallery-dl is moving to Codeberg after receiving a DMCA notice

**原文标题**: Media scraper Gallery-dl is moving to Codeberg after receiving a DMCA notice

**原文链接**: [https://github.com/mikf/gallery-dl/discussions/9304](https://github.com/mikf/gallery-dl/discussions/9304)

生成摘要时出错

---

## 39. A tail-call interpreter in (nightly) Rust

**原文标题**: A tail-call interpreter in (nightly) Rust

**原文链接**: [https://www.mattkeeter.com/blog/2026-04-05-tailcall/](https://www.mattkeeter.com/blog/2026-04-05-tailcall/)

生成摘要时出错

---

## 40. In Japan, the robot isn't coming for your job; it's filling the one nobody wants

**原文标题**: In Japan, the robot isn't coming for your job; it's filling the one nobody wants

**原文链接**: [https://techcrunch.com/2026/04/05/japan-is-proving-experimental-physical-ai-is-ready-for-the-real-world/](https://techcrunch.com/2026/04/05/japan-is-proving-experimental-physical-ai-is-ready-for-the-real-world/)

生成摘要时出错

---

## 41. Computational Physics (2nd Edition) (2025)

**原文标题**: Computational Physics (2nd Edition) (2025)

**原文链接**: [https://websites.umich.edu/~mejn/cp2/](https://websites.umich.edu/~mejn/cp2/)

生成摘要时出错

---

## 42. Show HN: M. C. Escher spiral in WebGL inspired by 3Blue1Brown

**原文标题**: Show HN: M. C. Escher spiral in WebGL inspired by 3Blue1Brown

**原文链接**: [https://static.laszlokorte.de/escher/](https://static.laszlokorte.de/escher/)

生成摘要时出错

---

## 43. Sam Altman May Control Our Future – Can He Be Trusted?

**原文标题**: Sam Altman May Control Our Future – Can He Be Trusted?

**原文链接**: [https://www.newyorker.com/magazine/2026/04/13/sam-altman-may-control-our-future-can-he-be-trusted](https://www.newyorker.com/magazine/2026/04/13/sam-altman-may-control-our-future-can-he-be-trusted)

生成摘要时出错

---

## 44. Nvim-treesitter (13K+ Stars) is Archived

**原文标题**: Nvim-treesitter (13K+ Stars) is Archived

**原文链接**: [https://github.com/nvim-treesitter/nvim-treesitter/discussions/8627](https://github.com/nvim-treesitter/nvim-treesitter/discussions/8627)

生成摘要时出错

---

## 45. Advice to young people, the lies I tell myself (2024)

**原文标题**: Advice to young people, the lies I tell myself (2024)

**原文链接**: [https://jxnl.co/writing/2024/06/01/advice-to-young-people/](https://jxnl.co/writing/2024/06/01/advice-to-young-people/)

生成摘要时出错

---

## 46. A cryptography engineer's perspective on quantum computing timelines

**原文标题**: A cryptography engineer's perspective on quantum computing timelines

**原文链接**: [https://words.filippo.io/crqc-timeline/](https://words.filippo.io/crqc-timeline/)

生成摘要时出错

---

## 47. Japanese, French and Omani vessels cross Strait of Hormuz

**原文标题**: Japanese, French and Omani vessels cross Strait of Hormuz

**原文链接**: [https://japantoday.com/category/politics/japanese-french-and-omani-vessels-cross-the-strait-of-hormuz](https://japantoday.com/category/politics/japanese-french-and-omani-vessels-cross-the-strait-of-hormuz)

生成摘要时出错

---

## 48. Copilot is 'for entertainment purposes only', per Microsoft's terms of use

**原文标题**: Copilot is 'for entertainment purposes only', per Microsoft's terms of use

**原文链接**: [https://techcrunch.com/2026/04/05/copilot-is-for-entertainment-purposes-only-according-to-microsofts-terms-of-service/](https://techcrunch.com/2026/04/05/copilot-is-for-entertainment-purposes-only-according-to-microsofts-terms-of-service/)

生成摘要时出错

---

## 49. Friendica – A Decentralized Social Network

**原文标题**: Friendica – A Decentralized Social Network

**原文链接**: [https://friendi.ca/](https://friendi.ca/)

生成摘要时出错

---

## 50. Shooting down ideas is not a skill

**原文标题**: Shooting down ideas is not a skill

**原文链接**: [https://scottlawsonbc.com/post/shooting-down-ideas](https://scottlawsonbc.com/post/shooting-down-ideas)

生成摘要时出错

---

## 51. Bacteria found in the human intestine capable of improving muscle strength

**原文标题**: Bacteria found in the human intestine capable of improving muscle strength

**原文链接**: [https://www.ugr.es/en/about/news/bacteria-found-human-intestine-capable-improving-muscle-strength](https://www.ugr.es/en/about/news/bacteria-found-human-intestine-capable-improving-muscle-strength)

生成摘要时出错

---

## 52. Book review: There is no antimemetics division

**原文标题**: Book review: There is no antimemetics division

**原文链接**: [https://www.stephendiehl.com/posts/no_antimimetics/](https://www.stephendiehl.com/posts/no_antimimetics/)

生成摘要时出错

---

## 53. Phone-free bars and restaurants on the rise across the U.S.

**原文标题**: Phone-free bars and restaurants on the rise across the U.S.

**原文链接**: [https://www.axios.com/2026/04/05/phone-free-restaurants-bars-bans-restrictions-offline](https://www.axios.com/2026/04/05/phone-free-restaurants-bars-bans-restrictions-offline)

生成摘要时出错

---

## 54. Aegis – open-source FPGA silicon

**原文标题**: Aegis – open-source FPGA silicon

**原文链接**: [https://github.com/MidstallSoftware/aegis](https://github.com/MidstallSoftware/aegis)

生成摘要时出错

---

## 55. Show HN: Gemma Gem – AI model embedded in a browser – no API keys, no cloud

**原文标题**: Show HN: Gemma Gem – AI model embedded in a browser – no API keys, no cloud

**原文链接**: [https://github.com/kessler/gemma-gem](https://github.com/kessler/gemma-gem)

生成摘要时出错

---

## 56. Ubuntu now requires more RAM than Windows 11

**原文标题**: Ubuntu now requires more RAM than Windows 11

**原文链接**: [https://www.howtogeek.com/ubuntu-now-requires-more-ram-than-windows-11/](https://www.howtogeek.com/ubuntu-now-requires-more-ram-than-windows-11/)

生成摘要时出错

---

## 57. Common drug tests lead to tens of thousands wrongful arrests a year

**原文标题**: Common drug tests lead to tens of thousands wrongful arrests a year

**原文链接**: [https://www.cnn.com/2026/04/05/us/colorado-field-drug-test-law](https://www.cnn.com/2026/04/05/us/colorado-field-drug-test-law)

生成摘要时出错

---

## 58. Adobe modifies hosts file to detect whether Creative Cloud is installed

**原文标题**: Adobe modifies hosts file to detect whether Creative Cloud is installed

**原文链接**: [https://www.osnews.com/story/144737/adobe-secretly-modifies-your-hosts-file-for-the-stupidest-reason/](https://www.osnews.com/story/144737/adobe-secretly-modifies-your-hosts-file-for-the-stupidest-reason/)

生成摘要时出错

---

## 59. Usenet Archives

**原文标题**: Usenet Archives

**原文链接**: [https://usenetarchives.com](https://usenetarchives.com)

生成摘要时出错

---

## 60. Show HN: Contrapunk – Real-time counterpoint harmony from guitar input

**原文标题**: Show HN: Contrapunk – Real-time counterpoint harmony from guitar input

**原文链接**: [https://contrapunk.com/](https://contrapunk.com/)

生成摘要时出错

---

## 61. Launch HN: Freestyle: Sandboxes for AI Coding Agents

**原文标题**: Launch HN: Freestyle: Sandboxes for AI Coding Agents

**原文链接**: [https://www.freestyle.sh](https://www.freestyle.sh)

生成摘要时出错

---

## 62. Drop, formerly Massdrop, ends most collaborations and rebrands under Corsair

**原文标题**: Drop, formerly Massdrop, ends most collaborations and rebrands under Corsair

**原文链接**: [https://drop.com/](https://drop.com/)

生成摘要时出错

---

## 63. Musician says AI company is cloning her music, filing claims against her

**原文标题**: Musician says AI company is cloning her music, filing claims against her

**原文链接**: [https://twitter.com/unlimited_ls/status/2040577536136974444](https://twitter.com/unlimited_ls/status/2040577536136974444)

生成摘要时出错

---

## 64. Case study: recovery of a corrupted 12 TB multi-device pool

**原文标题**: Case study: recovery of a corrupted 12 TB multi-device pool

**原文链接**: [https://github.com/kdave/btrfs-progs/issues/1107](https://github.com/kdave/btrfs-progs/issues/1107)

生成摘要时出错

---

## 65. Number in man page titles e.g. sleep(3)

**原文标题**: Number in man page titles e.g. sleep(3)

**原文链接**: [https://lalitm.com/til-number-in-man-page-titles-e-g-sleep-3/](https://lalitm.com/til-number-in-man-page-titles-e-g-sleep-3/)

生成摘要时出错

---

## 66. Isseven

**原文标题**: Isseven

**原文链接**: [https://isseven.app/](https://isseven.app/)

生成摘要时出错

---

## 67. UK intelligence censored report on global warming and homeland security

**原文标题**: UK intelligence censored report on global warming and homeland security

**原文链接**: [https://theoryofchange1.substack.com/p/from-global-warming-to-homeland-security](https://theoryofchange1.substack.com/p/from-global-warming-to-homeland-security)

生成摘要时出错

---

## 68. Iguanaworks has closed and our products are no longer sold

**原文标题**: Iguanaworks has closed and our products are no longer sold

**原文链接**: [http://iguanaworks.net/products/usb-ir-transceiver.html](http://iguanaworks.net/products/usb-ir-transceiver.html)

生成摘要时出错

---

## 69. Writing Lisp is AI resistant and I'm sad

**原文标题**: Writing Lisp is AI resistant and I'm sad

**原文链接**: [https://blog.djhaskin.com/blog/writing-lisp-is-ai-resistant-and-im-sad/](https://blog.djhaskin.com/blog/writing-lisp-is-ai-resistant-and-im-sad/)

生成摘要时出错

---

## 70. Show HN: Modo – I built an open-source alternative to Kiro, Cursor, and Windsurf

**原文标题**: Show HN: Modo – I built an open-source alternative to Kiro, Cursor, and Windsurf

**原文链接**: [https://github.com/mohshomis/modo](https://github.com/mohshomis/modo)

生成摘要时出错

---

## 71. The Mechanics of Steins Gate (2023) [pdf]

**原文标题**: The Mechanics of Steins Gate (2023) [pdf]

**原文链接**: [https://github.com/Votuko/steins-gate-mechanics/blob/main/The%20Mechanics%20of%20Steins%20Gate%20v1.0.3.pdf](https://github.com/Votuko/steins-gate-mechanics/blob/main/The%20Mechanics%20of%20Steins%20Gate%20v1.0.3.pdf)

生成摘要时出错

---

## 72. Sc-im: Spreadsheets in your terminal

**原文标题**: Sc-im: Spreadsheets in your terminal

**原文链接**: [https://github.com/andmarti1424/sc-im](https://github.com/andmarti1424/sc-im)

生成摘要时出错

---

## 73. Sky – an Elm-inspired language that compiles to Go

**原文标题**: Sky – an Elm-inspired language that compiles to Go

**原文链接**: [https://github.com/anzellai/sky](https://github.com/anzellai/sky)

生成摘要时出错

---

## 74. Show HN: GovAuctions lets you browse government auctions at once

**原文标题**: Show HN: GovAuctions lets you browse government auctions at once

**原文链接**: [https://www.govauctions.app/](https://www.govauctions.app/)

生成摘要时出错

---

## 75. My university uses prompt injection to catch cheaters

**原文标题**: My university uses prompt injection to catch cheaters

**原文链接**: [https://varun.ch/til/prompt-injection-catch-cheaters/](https://varun.ch/til/prompt-injection-catch-cheaters/)

生成摘要时出错

---

## 76. Show HN: OsintRadar – Curated directory for osint tools

**原文标题**: Show HN: OsintRadar – Curated directory for osint tools

**原文链接**: [https://osintradar.com/](https://osintradar.com/)

生成摘要时出错

---

## 77. Brain scans reveal how to enters a psychedelic-like trance without drugs

**原文标题**: Brain scans reveal how to enters a psychedelic-like trance without drugs

**原文链接**: [https://www.psypost.org/brain-scans-reveal-how-a-woman-voluntarily-enters-a-psychedelic-like-trance-without-drugs/](https://www.psypost.org/brain-scans-reveal-how-a-woman-voluntarily-enters-a-psychedelic-like-trance-without-drugs/)

生成摘要时出错

---

## 78. How Pope Leo is pushing back on divine justification of war

**原文标题**: How Pope Leo is pushing back on divine justification of war

**原文链接**: [https://www.cnn.com/2026/04/04/middleeast/pope-leo-iran-war-analysis-latam-intl](https://www.cnn.com/2026/04/04/middleeast/pope-leo-iran-war-analysis-latam-intl)

生成摘要时出错

---

## 79. The Team Behind a Pro-Iran, Lego-Themed Viral-Video Campaign

**原文标题**: The Team Behind a Pro-Iran, Lego-Themed Viral-Video Campaign

**原文链接**: [https://www.newyorker.com/culture/infinite-scroll/the-team-behind-a-pro-iran-lego-themed-viral-video-campaign](https://www.newyorker.com/culture/infinite-scroll/the-team-behind-a-pro-iran-lego-themed-viral-video-campaign)

生成摘要时出错

---

## 80. Reaffirming our commitment to child safety in the face of EuropeanUnion inaction

**原文标题**: Reaffirming our commitment to child safety in the face of EuropeanUnion inaction

**原文链接**: [https://blog.google/company-news/inside-google/around-the-globe/google-europe/reaffirming-commitment-to-child-safety/](https://blog.google/company-news/inside-google/around-the-globe/google-europe/reaffirming-commitment-to-child-safety/)

生成摘要时出错

---

## 81. Modern Generic SVGA driver for Windows 3.1

**原文标题**: Modern Generic SVGA driver for Windows 3.1

**原文链接**: [https://github.com/PluMGMK/vbesvga.drv](https://github.com/PluMGMK/vbesvga.drv)

生成摘要时出错

---

## 82. Women were never meant to give birth on their backs

**原文标题**: Women were never meant to give birth on their backs

**原文链接**: [https://www.bbc.com/future/article/20260401-women-were-never-meant-to-give-birth-on-their-backs](https://www.bbc.com/future/article/20260401-women-were-never-meant-to-give-birth-on-their-backs)

生成摘要时出错

---

## 83. OpenJDK: Panama

**原文标题**: OpenJDK: Panama

**原文链接**: [https://openjdk.org/projects/panama/](https://openjdk.org/projects/panama/)

生成摘要时出错

---

## 84. Iran's IRGC Publishes Satellite Imagery of OpenAI's $30B Stargate Datacenter

**原文标题**: Iran's IRGC Publishes Satellite Imagery of OpenAI's $30B Stargate Datacenter

**原文链接**: [https://newclawtimes.com/articles/iran-irgc-satellite-imagery-openai-stargate-abu-dhabi-datacenter-threat/](https://newclawtimes.com/articles/iran-irgc-satellite-imagery-openai-stargate-abu-dhabi-datacenter-threat/)

生成摘要时出错

---

## 85. AI that copied musical artist files copyright claim against artist [updated]

**原文标题**: AI that copied musical artist files copyright claim against artist [updated]

**原文链接**: [https://twitter.com/VladTheInflator/status/2039577001531768906](https://twitter.com/VladTheInflator/status/2039577001531768906)

生成摘要时出错

---

## 86. Netflix must refund customers for years of price hikes, Italian court rules

**原文标题**: Netflix must refund customers for years of price hikes, Italian court rules

**原文链接**: [https://arstechnica.com/gadgets/2026/04/netflix-ordered-to-refund-subscribers-up-to-e500-for-unlawful-price-hikes/](https://arstechnica.com/gadgets/2026/04/netflix-ordered-to-refund-subscribers-up-to-e500-for-unlawful-price-hikes/)

生成摘要时出错

---

## 87. Iran threatens 'complete and utter annihilation' of OpenAI's $30B Stargate

**原文标题**: Iran threatens 'complete and utter annihilation' of OpenAI's $30B Stargate

**原文链接**: [https://www.tomshardware.com/tech-industry/iran-threatens-complete-and-utter-annihilation-of-openais-usd30b-stargate-ai-data-center-in-abu-dhabi-regime-posts-video-with-satellite-imagery-of-chatgpt-makers-premier-1gw-data-center](https://www.tomshardware.com/tech-industry/iran-threatens-complete-and-utter-annihilation-of-openais-usd30b-stargate-ai-data-center-in-abu-dhabi-regime-posts-video-with-satellite-imagery-of-chatgpt-makers-premier-1gw-data-center)

生成摘要时出错

---

## 88. We replaced Node.js with Bun for 5x throughput

**原文标题**: We replaced Node.js with Bun for 5x throughput

**原文链接**: [https://trigger.dev/blog/firebun](https://trigger.dev/blog/firebun)

生成摘要时出错

---

## 89. GabeN Is Shitting Yacht Money into Flatpak and You're Still Arguing Init Systems

**原文标题**: GabeN Is Shitting Yacht Money into Flatpak and You're Still Arguing Init Systems

**原文链接**: [https://s3kshun8.games/blog/flatpak-won/](https://s3kshun8.games/blog/flatpak-won/)

生成摘要时出错

---

## 90. The Intelligence Failure in Iran

**原文标题**: The Intelligence Failure in Iran

**原文链接**: [https://www.theatlantic.com/national-security/2026/04/iran-war-intelligence-failure-trump/686694/](https://www.theatlantic.com/national-security/2026/04/iran-war-intelligence-failure-trump/686694/)

生成摘要时出错

---

## 91. Does coding with LLMs mean more microservices?

**原文标题**: Does coding with LLMs mean more microservices?

**原文链接**: [https://ben.page/microservices](https://ben.page/microservices)

生成摘要时出错

---

## 92. EPA official in charge of methane regulations was an oil and gas lobbyist

**原文标题**: EPA official in charge of methane regulations was an oil and gas lobbyist

**原文链接**: [https://www.propublica.org/article/trump-epa-methane-deregulation-aaron-szabo-oil-gas-axpc](https://www.propublica.org/article/trump-epa-methane-deregulation-aaron-szabo-oil-gas-axpc)

生成摘要时出错

---

## 93. When Virality Is the Message: The New Age of AI Propaganda

**原文标题**: When Virality Is the Message: The New Age of AI Propaganda

**原文链接**: [https://time.com/article/2026/04/02/when-virality-is-the-message-the-new-age-of-ai-propaganda/](https://time.com/article/2026/04/02/when-virality-is-the-message-the-new-age-of-ai-propaganda/)

生成摘要时出错

---

## 94. Qwen-3.6-Plus is the first model to break 1T tokens processed in a day

**原文标题**: Qwen-3.6-Plus is the first model to break 1T tokens processed in a day

**原文链接**: [https://twitter.com/openrouter/status/2040239467865489874](https://twitter.com/openrouter/status/2040239467865489874)

生成摘要时出错

---

## 95. Introducing GEN-1 [video]

**原文标题**: Introducing GEN-1 [video]

**原文链接**: [https://www.youtube.com/watch?v=SY2xyrmV44Y](https://www.youtube.com/watch?v=SY2xyrmV44Y)

生成摘要时出错

---

## 96. Student Debt Burdened Them, So They Moved Abroad and Stopped Paying

**原文标题**: Student Debt Burdened Them, So They Moved Abroad and Stopped Paying

**原文链接**: [https://www.nytimes.com/2026/04/04/business/student-loans-abroad-default.html](https://www.nytimes.com/2026/04/04/business/student-loans-abroad-default.html)

生成摘要时出错

---

## 97. Perfmon – Consolidate your favorite CLI monitoring tools into a single TUI

**原文标题**: Perfmon – Consolidate your favorite CLI monitoring tools into a single TUI

**原文链接**: [https://github.com/sumant1122/Perfmon](https://github.com/sumant1122/Perfmon)

生成摘要时出错

---

## 98. I used AI. It worked. I hated it

**原文标题**: I used AI. It worked. I hated it

**原文链接**: [https://taggart-tech.com/reckoning/](https://taggart-tech.com/reckoning/)

生成摘要时出错

---

## 99. Demonstrating Real Time AV2 Decoding on Consumer Laptops

**原文标题**: Demonstrating Real Time AV2 Decoding on Consumer Laptops

**原文链接**: [http://aomedia.org/blog%20posts/Demonstrating-Real-Time-AV2-Decoding-on-Consumer-Laptops/](http://aomedia.org/blog%20posts/Demonstrating-Real-Time-AV2-Decoding-on-Consumer-Laptops/)

生成摘要时出错

---

## 100. Tiny Corp's Exabox

**原文标题**: Tiny Corp's Exabox

**原文链接**: [https://twitter.com/__tinygrad__/status/2040944508402360592](https://twitter.com/__tinygrad__/status/2040944508402360592)

生成摘要时出错

---

