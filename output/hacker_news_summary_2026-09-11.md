# Hacker News 热门文章摘要 (2026-09-11)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. Shopify 从 React Native 回归到 Swift 和 Kotlin

**原文标题**: Shopify is moving from React Native back to Swift and Kotlin

**原文链接**: [https://shopify.engineering/back-to-native](https://shopify.engineering/back-to-native)

Shopify正在将其移动应用程序从React Native重新迁移回原生的Swift和Kotlin，这一战略转变主要是由AI编码代理（LLM）的显著进步所驱动的。尽管React Native自2020年采用以来取得了巨大成功，通过节省开发时间并实现跨栈贡献，但LLM已经从根本上改变了两次构建功能的成本效益分析。

AI代理现在极大地减少了跨平台的实现、转换、测试和审查工作量，从而削弱了React Native共享代码的核心优势。这使得Shopify能够拥抱原生开发的优势——更紧密的平台能力和工具，而无需承担此前令人望而却却步的“两次构建”成本。

Shopify正在采用全新的（从零开始重建）方法，利用LLM加速开发；Shop应用仅用12周就完成了原生重建并发布。为确保质量，他们开发了“Helix”系统，该系统将迁移过程分解为小块、测试驱动并经过人工审查的检查点。此外，一种新的代理可寻址架构将业务逻辑与UI解耦，使代理能够通过CLI在毫秒内迭代和测试代码，绕过缓慢的模拟器交互。

关于他们的开源React Native库：Skia将被分叉并继续由William Candillon负责维护，FlashList将获得关键修复，同时寻找新的长期维护者，Restyle将被归档。Shopify计划迁移所有应用，旨在超越当前的质量标准，并将公开分享此次雄心勃勃的AI驱动移动工程实践的经验。

---

## 2. 深度求索 v4.1 闪

**原文标题**: DeepSeek v4.1 Flash

**原文链接**: [https://twitter.com/deepseek_ai/status/2097930608790167907](https://twitter.com/deepseek_ai/status/2097930608790167907)

DeepSeek推出了其新的AI模型DeepSeek-V4.1-Flash，强调其更智能、更快、更高效。该模型是他们新架构系列中最小的一款，并具备原生的视觉理解能力。DeepSeek-V4.1-Flash旨在提升能力、加快推理速度、提高吞吐量，并可扩展至更大的模型。

---

## 3. 更多质疑：研究人员能否将未发表数学托付给OpenAI

**原文标题**: More questions about whether researchers can trust OpenAI with unpublished math

**原文链接**: [https://mathstodon.xyz/@andreasthom/117240535270608201](https://mathstodon.xyz/@andreasthom/117240535270608201)

生成摘要时出错

---

## 4. 不要让任何人拿走你的一大箱线缆。

**原文标题**: Don't let anyone take away your big box of cables

**原文链接**: [https://blog.jim-nielsen.com/2026/hands-off-my-cables/](https://blog.jim-nielsen.com/2026/hands-off-my-cables/)

作者偶然发现了一篇泰勒·高（Tyler Gaw）的在线帖子，深有共鸣。高在文中分享了他终于从自己那存了十多年的“一大箱线缆”中找到两根线缆的经历，这验证了他囤积线缆的习惯是正确的。他最后总结道：“永远不要让任何人拿走你那一大箱线缆。”

受到这个令人感同身受的“启示”的启发，作者决定采取行动。他截屏了高的帖子，打印出来，剪下，然后用透明打包胶带将其贴在了自己那“一大箱线缆”的正面，这箱线缆被他妻子标注为“家庭科技箱”（FAMILY TECHNO BOX）。这个实际行动不仅时刻提醒着盒子存在的价值，也让作者每当放入新线缆时，都能重拾乐趣和目的感。它也对那些可能考虑扔掉其内容的家庭成员起到了警示作用。作者希望有一天，他的孩子们能发现这个箱子，并听从箱子外面所展示的“永恒的忠告”。

---

## 5. Rust is tier-1 language at Microsoft

**原文标题**: Rust is tier-1 language at Microsoft

**原文链接**: [https://rustfoundation.org/media/guest-post-rust-is-tier-1-language-at-microsoft/](https://rustfoundation.org/media/guest-post-rust-is-tier-1-language-at-microsoft/)

Microsoft has officially designated Rust as a "Tier-1 language" for internal development, positioning it alongside C++, C#, and TypeScript. This reflects Rust's strategic importance and Microsoft's substantial investment in the language. The Tier-1 status ensures a "paved path" for internal teams, providing secure toolchain builds, productive tooling, quality workflows, deep platform integration, and compliance with Microsoft's SDL requirements.

A key innovation driving this integration is `rustc_codegen_utc`, an alternative code generation backend for `rustc`. This backend connects Rust directly to the MSVC backend (UTC), Windows' native platform compiler. Its development ensures high compatibility with the Windows tooling ecosystem and ABI, enabling crucial features like binary hardening, code security, post-link compliance (including Hotpatch), and seamless interoperability for hybrid Rust/C++ projects. `rustc_codegen_utc` leverages existing MSVC capabilities for cross-language optimization, debugging, profiling, and diagnostics, avoiding redundant development for Windows-specific features.

This unified code generation platform for Rust and C++ on Windows minimizes maintenance and evolution costs, allowing new platform innovations to benefit both languages simultaneously. It's particularly vital for hybrid projects, ensuring both Rust and C++ participate equally in development workflows. `rustc_codegen_utc` has been production-ready since early 2026, is self-hosted since Rust 1.90, and is being adopted by a growing number of Microsoft repositories, signifying a sustained investment in Rust's complete engineering lifecycle at the company.

---

## 6. HN 展示：如果光速是 5 公里/小时会怎么样？

**原文标题**: Show HN: What if the speed of light was 5 km/h?

**原文链接**: [https://rivendell.dmitrybrant.com/relativity/](https://rivendell.dmitrybrant.com/relativity/)

“相对论公园”是一个交互式模拟，它通过将光速大幅降低至每小时仅5公里（相当于轻快的步行速度），探索狭义相对论的奇异效应。

在这个虚拟环境中，用户可以亲身体验如果光速与日常人类运动速度相当，会发生什么。当玩家加速时，他们将观察到经典的相对论现象，例如长度收缩（物体看起来更短）、时间膨胀（他们的个人时钟比“世界”时钟走得慢）以及特雷尔旋转。光的多普勒效应也变得明显，导致前方的物体发生蓝移，后方的物体发生红移，以及移动的物体表现出横向多普勒效应。

该模拟强调，即使在如此低速下，光速仍然是一个渐近极限，永远无法真正达到。用户使用键盘控制（加速、停止、切换效果、重置）和鼠标进行环顾来导航和交互，让他们沉浸在一个相对论物理可见且直观的世界中。

---

## 7. 克劳德仅限18岁以上人士使用。

**原文标题**: Claude is only available to people over 18 years

**原文链接**: [https://support.claude.com/en/articles/15171100-age-assurance-on-claude](https://support.claude.com/en/articles/15171100-age-assurance-on-claude)

Anthropic的消费级产品Claude仅限18岁及以上用户使用。用户在账户设置时需要确认年龄。如果系统检测到用户可能未满18岁的信号，其账户将被禁用，并要求进行年龄验证。

年龄验证过程由第三方平台Yoti处理。用户将收到一封包含验证链接的电子邮件。验证成功后，账户将被恢复。Yoti提供以下几种选项：
1.  **面部年龄估算：** 用户拍摄自拍照进行年龄估算，无需身份证件。
2.  **证件验证：** 用户上传政府颁发的身份证件（如护照或驾照）照片。
3.  **Yoti数字身份App：** 用户可以从其现有Yoti App中共享已验证的“18岁以上”属性。

关于数据保护，Yoti是一家经过独立审计的服务提供商。您的自拍照、证件图像以及任何个人数据在年龄验证完成后会立即被Yoti删除。Anthropic绝不会查看或存储您的身份证件或图像；它仅从Yoti接收通过/失败的结果，从而确保用户隐私。

---

## 8. 我有一个理论，软件会把人逼疯。

**原文标题**: I have a theory that software drives people insane

**原文链接**: [https://graybeard.ing/software-drives-people-insane/](https://graybeard.ing/software-drives-people-insane/)

生成摘要时出错

---

## 9. Automattic's board forces CEO Matt Mullenweg into leave of absence

**原文标题**: Automattic's board forces CEO Matt Mullenweg into leave of absence

**原文链接**: [https://techcrunch.com/2026/09/09/automattics-board-forces-ceo-matt-mullenweg-into-leave-of-absence/](https://techcrunch.com/2026/09/09/automattics-board-forces-ceo-matt-mullenweg-into-leave-of-absence/)

Automattic founder and CEO Matt Mullenweg has been forced into a paid leave of absence by the company's board of directors, a decision he opposed and described as a "conspiracy." According to a Slack message from Mullenweg, CFO Mark Davies, along with board members Ann Dunwoody, Toni Schneider, and Sue Decker, voted for the leave, denying his request for legal counsel. Mark Davies has been appointed interim CEO.

Automattic confirmed the leave, stating full confidence in Davies' leadership. While Mullenweg is on leave from Automattic, Mary Hubbard, Executive Director of WordPress.org, clarified that Mullenweg remains the leader of the open-source WordPress project, which is unaffected by the change at the commercial company.

The board's action follows a period of controversy under Mullenweg's leadership. Automattic is engaged in a protracted legal dispute with WP Engine, initiated by Mullenweg's demand for royalty fees for WordPress brand usage, leading to WP Engine suing for defamation and abuse of power. Other issues include Mullenweg telling employees to quit if they disagreed with him (leading to 159 departures), threatening and deactivating accounts of open-source community members, and a 16% staff layoff in April 2025.

Employee reactions vary from "ecstatic" and "relieved" to concerns about instability. Mullenweg's recent posts on X hinted at the cause, referencing an allegation of spoiling evidence in the WP Engine lawsuit and anticipating "smear attacks."

---

## 10. Cognition launches new SWE-2 model, Rivaling Fable 5.1 and GPT-Astra

**原文标题**: Cognition launches new SWE-2 model, Rivaling Fable 5.1 and GPT-Astra

**原文链接**: [https://cognition.com/blog/swe-2](https://cognition.com/blog/swe-2)

生成摘要时出错

---

## 11. List of references on Sony websites to players "owning" their digital games

**原文标题**: List of references on Sony websites to players "owning" their digital games

**原文链接**: [https://consumerrights.wiki/w/Sony_PlayStation_digital_game_ownership_lawsuit](https://consumerrights.wiki/w/Sony_PlayStation_digital_game_ownership_lawsuit)

生成摘要时出错

---

## 12. Astra for Coding: Why Are We Doing This Again?

**原文标题**: Astra for Coding: Why Are We Doing This Again?

**原文链接**: [https://lucumr.pocoo.org/2026/9/7/astra-why/](https://lucumr.pocoo.org/2026/9/7/astra-why/)

生成摘要时出错

---

## 13. A misalignment of AI in mathematics

**原文标题**: A misalignment of AI in mathematics

**原文链接**: [https://mathandai.org/](https://mathandai.org/)

生成摘要时出错

---

## 14. The same nine streaming subscriptions cost $702/year more than in 2021

**原文标题**: The same nine streaming subscriptions cost $702/year more than in 2021

**原文链接**: [https://honestlyranked.com/guides/streaming-price-increases/](https://honestlyranked.com/guides/streaming-price-increases/)

生成摘要时出错

---

## 15. Mexican student creates an acoustic fire extinguisher to put out fire in seconds

**原文标题**: Mexican student creates an acoustic fire extinguisher to put out fire in seconds

**原文链接**: [https://www.upsocl.com/en/16-year-old-mexican-student-creates-an-acoustic-fire-extinguisher-that-uses-sound-waves-to-put-out-fires-in-seconds/](https://www.upsocl.com/en/16-year-old-mexican-student-creates-an-acoustic-fire-extinguisher-that-uses-sound-waves-to-put-out-fires-in-seconds/)

生成摘要时出错

---

## 16. Technique for Manipulating Satellite Photos Now Reveals Ancient Images (2025)

**原文标题**: Technique for Manipulating Satellite Photos Now Reveals Ancient Images (2025)

**原文链接**: [https://spinoff.nasa.gov/Manipulating_Satellite_Photos_Now_Reveals_Ancient_Images](https://spinoff.nasa.gov/Manipulating_Satellite_Photos_Now_Reveals_Ancient_Images)

生成摘要时出错

---

## 17. What algorithm did Windows XP use to choose your initial user picture?

**原文标题**: What algorithm did Windows XP use to choose your initial user picture?

**原文链接**: [https://devblogs.microsoft.com/oldnewthing/20260909-00/?p=112683](https://devblogs.microsoft.com/oldnewthing/20260909-00/?p=112683)

生成摘要时出错

---

## 18. Houthis 'take control' of key island in global shipping route

**原文标题**: Houthis 'take control' of key island in global shipping route

**原文链接**: [https://www.bbc.com/news/live/cmd683p01eljt](https://www.bbc.com/news/live/cmd683p01eljt)

生成摘要时出错

---

## 19. OpenAI Agents API

**原文标题**: OpenAI Agents API

**原文链接**: [https://developers.openai.com/api/docs/guides/agents-api/overview](https://developers.openai.com/api/docs/guides/agents-api/overview)

生成摘要时出错

---

## 20. The Waymo effect: how AI is quietly making research less collaborative

**原文标题**: The Waymo effect: how AI is quietly making research less collaborative

**原文链接**: [https://www.researchagenda.news/articles/the-waymo-effect.html](https://www.researchagenda.news/articles/the-waymo-effect.html)

生成摘要时出错

---

## 21. Google will buy half the electricity from one of Finland's nuclear power plants

**原文标题**: Google will buy half the electricity from one of Finland's nuclear power plants

**原文链接**: [https://www.bbc.com/news/articles/c8r6y4me2g6o](https://www.bbc.com/news/articles/c8r6y4me2g6o)

生成摘要时出错

---

## 22. OpenAI might have stolen another major proof

**原文标题**: OpenAI might have stolen another major proof

**原文链接**: [https://twitter.com/ValerioCapraro/status/2097791836269977996](https://twitter.com/ValerioCapraro/status/2097791836269977996)

生成摘要时出错

---

## 23. Music Theory for the 21st-Century Classroom

**原文标题**: Music Theory for the 21st-Century Classroom

**原文链接**: [https://musictheory.pugetsound.edu/mt21c/MusicTheory.html](https://musictheory.pugetsound.edu/mt21c/MusicTheory.html)

生成摘要时出错

---

## 24. Neki – Sharded Postgres

**原文标题**: Neki – Sharded Postgres

**原文链接**: [https://planetscale.com/blog/introducing-neki](https://planetscale.com/blog/introducing-neki)

生成摘要时出错

---

## 25. All grown-ups were once children, but only few of them remember it

**原文标题**: All grown-ups were once children, but only few of them remember it

**原文链接**: [https://mathstodon.xyz/@tao/117244102901892965](https://mathstodon.xyz/@tao/117244102901892965)

生成摘要时出错

---

## 26. The Deathray: A simple way for an untrusted site to freeze a Mac

**原文标题**: The Deathray: A simple way for an untrusted site to freeze a Mac

**原文链接**: [https://auberon.xyz/blog/posts/deathray/](https://auberon.xyz/blog/posts/deathray/)

生成摘要时出错

---

## 27. Another researcher says OpenAI trained on conversations, then claimed breakthrou

**原文标题**: Another researcher says OpenAI trained on conversations, then claimed breakthrou

**原文链接**: [https://bsky.app/profile/did:plc:ckaz32jwl6t2cno6fmuw2nhn/post/3mv4mt4ikss2d](https://bsky.app/profile/did:plc:ckaz32jwl6t2cno6fmuw2nhn/post/3mv4mt4ikss2d)

生成摘要时出错

---

## 28. Blizzard Workers Win Historic Union Contract

**原文标题**: Blizzard Workers Win Historic Union Contract

**原文链接**: [https://www.latimes.com/entertainment-arts/business/story/2026-09-09/blizzard-video-game-workers-ratify-union-contract](https://www.latimes.com/entertainment-arts/business/story/2026-09-09/blizzard-video-game-workers-ratify-union-contract)

生成摘要时出错

---

## 29. HuggingFace: Security.txt

**原文标题**: HuggingFace: Security.txt

**原文链接**: [https://huggingface.co/security.txt](https://huggingface.co/security.txt)

生成摘要时出错

---

## 30. The EPA is planning to scrap public review rules for data center pollution

**原文标题**: The EPA is planning to scrap public review rules for data center pollution

**原文链接**: [https://capitalbnews.org/data-centers-permit-rules-epa/](https://capitalbnews.org/data-centers-permit-rules-epa/)

生成摘要时出错

---

## 31. Measuring the sloppiness of code

**原文标题**: Measuring the sloppiness of code

**原文链接**: [https://earendil.com/posts/measuring-code-sloppiness/](https://earendil.com/posts/measuring-code-sloppiness/)

生成摘要时出错

---

## 32. Cherenkov Radiation

**原文标题**: Cherenkov Radiation

**原文链接**: [http://www.iaea.org/newscenter/news/what-is-cherenkov-radiation](http://www.iaea.org/newscenter/news/what-is-cherenkov-radiation)

生成摘要时出错

---

## 33. Forgejo <=16.0.3 Critical RCE

**原文标题**: Forgejo <=16.0.3 Critical RCE

**原文链接**: [https://codeberg.org/forgejo/forgejo/src/branch/forgejo/release-notes-published/16.0.4.md](https://codeberg.org/forgejo/forgejo/src/branch/forgejo/release-notes-published/16.0.4.md)

生成摘要时出错

---

## 34. Muse, the band, lost its social media handles to Muse, Meta's new AI agent

**原文标题**: Muse, the band, lost its social media handles to Muse, Meta's new AI agent

**原文链接**: [https://www.engadget.com/2254419/muse-the-band-lost-its-social-media-handles-to-muse-meta-s-new-ai-agent/](https://www.engadget.com/2254419/muse-the-band-lost-its-social-media-handles-to-muse-meta-s-new-ai-agent/)

生成摘要时出错

---

## 35. I think I hate the internet

**原文标题**: I think I hate the internet

**原文链接**: [https://strategictree.bearblog.dev/i-think-i-hate-the-internet/](https://strategictree.bearblog.dev/i-think-i-hate-the-internet/)

生成摘要时出错

---

## 36. Matt Mullenweg put on 'leave of absence'

**原文标题**: Matt Mullenweg put on 'leave of absence'

**原文链接**: [https://www.404media.co/wordpress-automattic-ceo-matt-mullenweg-put-on-leave-of-absence/](https://www.404media.co/wordpress-automattic-ceo-matt-mullenweg-put-on-leave-of-absence/)

生成摘要时出错

---

## 37. Silicon Valley is transforming the military-industrial complex? (2024)

**原文标题**: Silicon Valley is transforming the military-industrial complex? (2024)

**原文链接**: [https://costsofwar.watson.brown.edu/paper/how-big-tech-and-silicon-valley-are-transforming-military-industrial-complex](https://costsofwar.watson.brown.edu/paper/how-big-tech-and-silicon-valley-are-transforming-military-industrial-complex)

生成摘要时出错

---

## 38. OpenAI’s Navier-Stokes release included a Lean 4 formal proof

**原文标题**: OpenAI’s Navier-Stokes release included a Lean 4 formal proof

**原文链接**: [https://www.johndcook.com/blog/2026/09/09/formal-method-revolution/](https://www.johndcook.com/blog/2026/09/09/formal-method-revolution/)

生成摘要时出错

---

## 39. Nine coding harnesses vs. your laptop

**原文标题**: Nine coding harnesses vs. your laptop

**原文链接**: [https://nasutton.notion.site/Nine-coding-harnesses-vs-your-laptop-3d139990182b80d59fa3cf500f0450ba?pvs=74](https://nasutton.notion.site/Nine-coding-harnesses-vs-your-laptop-3d139990182b80d59fa3cf500f0450ba?pvs=74)

生成摘要时出错

---

## 40. Detecting and countering misuse of AI: September 2026

**原文标题**: Detecting and countering misuse of AI: September 2026

**原文链接**: [https://www.anthropic.com/threat-intelligence-report-september-2026](https://www.anthropic.com/threat-intelligence-report-september-2026)

生成摘要时出错

---

## 41. Thanks to Siri Recaps, your Apple Watch is always listening

**原文标题**: Thanks to Siri Recaps, your Apple Watch is always listening

**原文链接**: [https://www.techradar.com/health-fitness/smartwatches/thanks-to-siri-recaps-your-apple-watch-is-always-listening-as-you-go-about-your-day-but-apple-may-be-risking-a-meta-glasses-style-backlash](https://www.techradar.com/health-fitness/smartwatches/thanks-to-siri-recaps-your-apple-watch-is-always-listening-as-you-go-about-your-day-but-apple-may-be-risking-a-meta-glasses-style-backlash)

生成摘要时出错

---

## 42. Creativity is the new moat

**原文标题**: Creativity is the new moat

**原文链接**: [https://www.inventbuild.studio/blog/genuine-creativity-is-your-new-moat](https://www.inventbuild.studio/blog/genuine-creativity-is-your-new-moat)

生成摘要时出错

---

## 43. Feeling Sad about AI

**原文标题**: Feeling Sad about AI

**原文链接**: [https://artificialworlds.net/blog/2026/09/11/feeling-sad-about-ai/](https://artificialworlds.net/blog/2026/09/11/feeling-sad-about-ai/)

生成摘要时出错

---

## 44. Show HN: Hacker News, without AI

**原文标题**: Show HN: Hacker News, without AI

**原文链接**: [https://hcker.news/?ai=exclude](https://hcker.news/?ai=exclude)

生成摘要时出错

---

## 45. Show HN: Hacker News, Without AI

**原文标题**: Show HN: Hacker News, Without AI

**原文链接**: [https://www.unslop.news/](https://www.unslop.news/)

生成摘要时出错

---

## 46. A Misalignment of AI in Mathematics

**原文标题**: A Misalignment of AI in Mathematics

**原文链接**: [https://terrytao.wordpress.com/2026/09/11/a-severe-misalignment-of-ai-in-mathematics/](https://terrytao.wordpress.com/2026/09/11/a-severe-misalignment-of-ai-in-mathematics/)

生成摘要时出错

---

## 47. NTSB issues investigative update on B-767 runway excursion accident in Miami

**原文标题**: NTSB issues investigative update on B-767 runway excursion accident in Miami

**原文链接**: [https://www.ntsb.gov:443/news/press-releases/Pages/NR20260909.aspx](https://www.ntsb.gov:443/news/press-releases/Pages/NR20260909.aspx)

生成摘要时出错

---

## 48. Global Glacier Extinction Explorer

**原文标题**: Global Glacier Extinction Explorer

**原文链接**: [https://glacierextinction.com](https://glacierextinction.com)

生成摘要时出错

---

## 49. Amazon refused to give pregnant workers bathroom breaks

**原文标题**: Amazon refused to give pregnant workers bathroom breaks

**原文链接**: [https://arstechnica.com/tech-policy/2026/09/lawsuit-amazon-refused-to-give-pregnant-workers-bathroom-breaks-and-chairs/](https://arstechnica.com/tech-policy/2026/09/lawsuit-amazon-refused-to-give-pregnant-workers-bathroom-breaks-and-chairs/)

生成摘要时出错

---

## 50. RTK reports token savings, but our cost benchmarks disagree

**原文标题**: RTK reports token savings, but our cost benchmarks disagree

**原文链接**: [https://quesma.com/blog/does-rtk-make-ai-coding-cheaper/](https://quesma.com/blog/does-rtk-make-ai-coding-cheaper/)

生成摘要时出错

---

## 51. Show HN: Bodily Oddities

**原文标题**: Show HN: Bodily Oddities

**原文链接**: [https://vester.si/bodily-oddities/](https://vester.si/bodily-oddities/)

生成摘要时出错

---

## 52. Proof of Capture: Apple Reference Image, but open source and using steganography

**原文标题**: Proof of Capture: Apple Reference Image, but open source and using steganography

**原文链接**: [https://merybenavente.me/blog/proof-of-capture](https://merybenavente.me/blog/proof-of-capture)

生成摘要时出错

---

## 53. Matt Mullenweg tells Automattic staff in Slack he's back in control after ouster

**原文标题**: Matt Mullenweg tells Automattic staff in Slack he's back in control after ouster

**原文链接**: [https://techcrunch.com/2026/09/11/matt-mullenweg-tells-automattic-staff-in-slack-hes-back-in-control-after-ceo-ouster/](https://techcrunch.com/2026/09/11/matt-mullenweg-tells-automattic-staff-in-slack-hes-back-in-control-after-ceo-ouster/)

生成摘要时出错

---

## 54. Exercise intensity is associated with cardiometabolic health

**原文标题**: Exercise intensity is associated with cardiometabolic health

**原文链接**: [https://www.cell.com/cell-reports-medicine/fulltext/S2666-3791(26)00405-2](https://www.cell.com/cell-reports-medicine/fulltext/S2666-3791(26)00405-2)

生成摘要时出错

---

## 55. Room 641A

**原文标题**: Room 641A

**原文链接**: [https://en.wikipedia.org/wiki/Room_641A](https://en.wikipedia.org/wiki/Room_641A)

生成摘要时出错

---

## 56. South Park creators rename show 'South America'

**原文标题**: South Park creators rename show 'South America'

**原文链接**: [https://www.bbc.co.uk/news/articles/cp9340rg7k8o](https://www.bbc.co.uk/news/articles/cp9340rg7k8o)

生成摘要时出错

---

## 57. Thelio Mira AI Linux Workstation: 192 GB GPU Memory

**原文标题**: Thelio Mira AI Linux Workstation: 192 GB GPU Memory

**原文链接**: [https://system76.com/workstations/thelio-mira-ai](https://system76.com/workstations/thelio-mira-ai)

生成摘要时出错

---

## 58. GrapheneOS' rewritten Messages app is released

**原文标题**: GrapheneOS' rewritten Messages app is released

**原文链接**: [https://github.com/GrapheneOS/Messaging/releases/tag/13](https://github.com/GrapheneOS/Messaging/releases/tag/13)

生成摘要时出错

---

## 59. Training a 3.8B LLM to 0.384 CORE for $998

**原文标题**: Training a 3.8B LLM to 0.384 CORE for $998

**原文链接**: [https://hugovergnes.github.io/little-lm-3-8b/](https://hugovergnes.github.io/little-lm-3-8b/)

生成摘要时出错

---

## 60. AI Is Breaking This Thing We Call Trust

**原文标题**: AI Is Breaking This Thing We Call Trust

**原文链接**: [https://terriblesoftware.org/2026/09/10/ai-is-breaking-this-thing-we-call-trust/](https://terriblesoftware.org/2026/09/10/ai-is-breaking-this-thing-we-call-trust/)

生成摘要时出错

---

## 61. Neijuan

**原文标题**: Neijuan

**原文链接**: [https://en.wikipedia.org/wiki/Neijuan](https://en.wikipedia.org/wiki/Neijuan)

生成摘要时出错

---

## 62. Rune is now open source

**原文标题**: Rune is now open source

**原文链接**: [https://rune.build/blog/rune-is-now-open-source](https://rune.build/blog/rune-is-now-open-source)

生成摘要时出错

---

## 63. Diesel prices in U.S. top $6 a gallon for first time

**原文标题**: Diesel prices in U.S. top $6 a gallon for first time

**原文链接**: [https://www.cbsnews.com/news/rising-diesel-prices-consumer-impact/](https://www.cbsnews.com/news/rising-diesel-prices-consumer-impact/)

生成摘要时出错

---

## 64. YuE2 · Frontier Music with Symbolic Planning

**原文标题**: YuE2 · Frontier Music with Symbolic Planning

**原文链接**: [https://map-yue2.github.io/](https://map-yue2.github.io/)

生成摘要时出错

---

## 65. Neki is sharded Postgres by PlanetScale

**原文标题**: Neki is sharded Postgres by PlanetScale

**原文链接**: [https://neki.dev/](https://neki.dev/)

生成摘要时出错

---

## 66. Bending Spoons buying Miro for $1.355B

**原文标题**: Bending Spoons buying Miro for $1.355B

**原文链接**: [https://investors.bendingspoons.com/newsroom/bending-spoons-agrees-to-acquire-miro](https://investors.bendingspoons.com/newsroom/bending-spoons-agrees-to-acquire-miro)

生成摘要时出错

---

## 67. JEP 544: Ahead-of-Time Code Compilation

**原文标题**: JEP 544: Ahead-of-Time Code Compilation

**原文链接**: [https://openjdk.org/jeps/544](https://openjdk.org/jeps/544)

生成摘要时出错

---

## 68. OpenAI have no mathematicians capable of understanding what they put out

**原文标题**: OpenAI have no mathematicians capable of understanding what they put out

**原文链接**: [https://mastodon.social/@tristanbuckmaster/117237555794407063](https://mastodon.social/@tristanbuckmaster/117237555794407063)

生成摘要时出错

---

## 69. Hacker News with reduced priority for AI driven content

**原文标题**: Hacker News with reduced priority for AI driven content

**原文链接**: [https://sprinklz.io/public/pdwt4dve5uai](https://sprinklz.io/public/pdwt4dve5uai)

生成摘要时出错

---

## 70. Instagram's head says engagement falls by half without the algorithm

**原文标题**: Instagram's head says engagement falls by half without the algorithm

**原文链接**: [https://thenextweb.com/news/mosseri-instagram-algorithm-opt-out-engagement-australia](https://thenextweb.com/news/mosseri-instagram-algorithm-opt-out-engagement-australia)

生成摘要时出错

---

## 71. New York thoracic surgeon: "For many patients 9/11 is not over"

**原文标题**: New York thoracic surgeon: "For many patients 9/11 is not over"

**原文链接**: [https://www.statnews.com/2026/09/11/sept-11-25th-anniversary-ground-zero-exposure-cancer-moment-of-silence/](https://www.statnews.com/2026/09/11/sept-11-25th-anniversary-ground-zero-exposure-cancer-moment-of-silence/)

生成摘要时出错

---

## 72. A Stupid Idea for AI Alignment We Came with by Looking at Specification Gaming

**原文标题**: A Stupid Idea for AI Alignment We Came with by Looking at Specification Gaming

**原文链接**: [https://slimemoldtimemold.com/2026/08/05/a-stupid-idea-for-ai-alignment-we-came-up-with-by-looking-at-the-list-of-specification-gaming-behaviours/](https://slimemoldtimemold.com/2026/08/05/a-stupid-idea-for-ai-alignment-we-came-up-with-by-looking-at-the-list-of-specification-gaming-behaviours/)

生成摘要时出错

---

## 73. Top mathematicians are outraged by OpenAI's methods

**原文标题**: Top mathematicians are outraged by OpenAI's methods

**原文链接**: [https://www.economist.com/science-and-technology/2026/09/11/top-mathematicians-are-outraged-by-openais-methods](https://www.economist.com/science-and-technology/2026/09/11/top-mathematicians-are-outraged-by-openais-methods)

生成摘要时出错

---

## 74. Amazon pilots ad services in ChatGPT

**原文标题**: Amazon pilots ad services in ChatGPT

**原文链接**: [https://www.marketingdive.com/news/amazon-pilots-ad-services-in-chatgpt-what-marketers-need-to-know/829945/](https://www.marketingdive.com/news/amazon-pilots-ad-services-in-chatgpt-what-marketers-need-to-know/829945/)

生成摘要时出错

---

## 75. CSS Curiosities of the Past

**原文标题**: CSS Curiosities of the Past

**原文链接**: [https://vale.rocks/posts/css-relics](https://vale.rocks/posts/css-relics)

生成摘要时出错

---

## 76. PlayStation cancels Kojima's PHYSINT, Xbox steps in

**原文标题**: PlayStation cancels Kojima's PHYSINT, Xbox steps in

**原文链接**: [https://twitter.com/hideo_kojima_en/status/2097877506401681753](https://twitter.com/hideo_kojima_en/status/2097877506401681753)

生成摘要时出错

---

## 77. I'm sorry, you're not going to die from an AI-engineered supervirus

**原文标题**: I'm sorry, you're not going to die from an AI-engineered supervirus

**原文链接**: [https://blog.genesmindsmachines.com/p/im-sorry-youre-not-going-to-die-from](https://blog.genesmindsmachines.com/p/im-sorry-youre-not-going-to-die-from)

生成摘要时出错

---

## 78. Λ Snap – An inviting programming language for kids and adults for CS study

**原文标题**: Λ Snap – An inviting programming language for kids and adults for CS study

**原文链接**: [https://snap.berkeley.edu/](https://snap.berkeley.edu/)

生成摘要时出错

---

## 79. I spent $220 on Google app ads. 60% of the installs were robots

**原文标题**: I spent $220 on Google app ads. 60% of the installs were robots

**原文链接**: [https://dayzlegame.com/blog/google-ads-bot-farm/](https://dayzlegame.com/blog/google-ads-bot-farm/)

生成摘要时出错

---

## 80. 118M Queries per Second on Neki

**原文标题**: 118M Queries per Second on Neki

**原文链接**: [https://planetscale.com/blog/118-million-queries-per-second-on-neki](https://planetscale.com/blog/118-million-queries-per-second-on-neki)

生成摘要时出错

---

## 81. Omarchy Is a Power Grab

**原文标题**: Omarchy Is a Power Grab

**原文链接**: [https://tante.cc/2026/09/11/power-grab/](https://tante.cc/2026/09/11/power-grab/)

生成摘要时出错

---

## 82. Mathematicians want proof OpenAI didn't use their work

**原文标题**: Mathematicians want proof OpenAI didn't use their work

**原文链接**: [https://www.theverge.com/ai-artificial-intelligence/993263/where-does-openai-get-mathematics-training-data](https://www.theverge.com/ai-artificial-intelligence/993263/where-does-openai-get-mathematics-training-data)

生成摘要时出错

---

## 83. Show HN: Toast, a beautiful by default in terminal IDE

**原文标题**: Show HN: Toast, a beautiful by default in terminal IDE

**原文链接**: [https://github.com/paradise-runner/toast](https://github.com/paradise-runner/toast)

生成摘要时出错

---

## 84. Show HN: Godot and Rust based multiplexer (terminal panes and more)

**原文标题**: Show HN: Godot and Rust based multiplexer (terminal panes and more)

**原文链接**: [https://github.com/godot-pty/gpty](https://github.com/godot-pty/gpty)

生成摘要时出错

---

## 85. Who People Talk to When They're Struggling

**原文标题**: Who People Talk to When They're Struggling

**原文链接**: [https://www.graphsaboutreligion.com/p/who-do-you-talk-to-when-youre-struggling](https://www.graphsaboutreligion.com/p/who-do-you-talk-to-when-youre-struggling)

生成摘要时出错

---

## 86. What Comes After Git

**原文标题**: What Comes After Git

**原文链接**: [https://ersc.io/blog/what-comes-after-git](https://ersc.io/blog/what-comes-after-git)

生成摘要时出错

---

## 87. Remember Hong Kong

**原文标题**: Remember Hong Kong

**原文链接**: [https://www.thenextmove.org/p/remember-hong-kong](https://www.thenextmove.org/p/remember-hong-kong)

生成摘要时出错

---

## 88. 1M+ German households have hung solar panels off their balcony railings

**原文标题**: 1M+ German households have hung solar panels off their balcony railings

**原文链接**: [https://spacedaily.com/b-more-than-a-million-german-households-have-hung-solar-panels-off-their-balcony-railings-and-plugged-them-into-a-wall-socket-and-the-law-caps-each-at-800-watts-a-fridge-and-a-laptop/](https://spacedaily.com/b-more-than-a-million-german-households-have-hung-solar-panels-off-their-balcony-railings-and-plugged-them-into-a-wall-socket-and-the-law-caps-each-at-800-watts-a-fridge-and-a-laptop/)

生成摘要时出错

---

## 89. Anthropic says it blocked possible efforts to build biological weapons

**原文标题**: Anthropic says it blocked possible efforts to build biological weapons

**原文链接**: [https://www.nytimes.com/2026/09/10/us/politics/anthropic-ai-biological-weapons.html](https://www.nytimes.com/2026/09/10/us/politics/anthropic-ai-biological-weapons.html)

生成摘要时出错

---

## 90. Tor VPN Beta: What we've learned building our own VPN for Android from scratch

**原文标题**: Tor VPN Beta: What we've learned building our own VPN for Android from scratch

**原文链接**: [https://blog.torproject.org/tor-vpn-beta/](https://blog.torproject.org/tor-vpn-beta/)

生成摘要时出错

---

## 91. Copying login keychains between Macs fails on Secure Enclave Macs with Tahoe

**原文标题**: Copying login keychains between Macs fails on Secure Enclave Macs with Tahoe

**原文链接**: [https://derflounder.wordpress.com/2026/09/08/manually-copying-login-keychain-files-from-one-mac-to-another-no-longer-works-on-secure-enclave-equipped-macs-running-macos-tahoe/](https://derflounder.wordpress.com/2026/09/08/manually-copying-login-keychain-files-from-one-mac-to-another-no-longer-works-on-secure-enclave-equipped-macs-running-macos-tahoe/)

生成摘要时出错

---

## 92. The Death of Shame Is Tearing Us Apart

**原文标题**: The Death of Shame Is Tearing Us Apart

**原文链接**: [https://www.newyorker.com/news/fault-lines/the-death-of-shame-is-tearing-us-apart](https://www.newyorker.com/news/fault-lines/the-death-of-shame-is-tearing-us-apart)

生成摘要时出错

---

## 93. Cognition's SWE-2 achieves 92.8 on Terminal-Bench 2.1

**原文标题**: Cognition's SWE-2 achieves 92.8 on Terminal-Bench 2.1

**原文链接**: [https://tokenstead.ai/models/swe-2](https://tokenstead.ai/models/swe-2)

生成摘要时出错

---

## 94. Litelm: LiteLLM Without the Bloat

**原文标题**: Litelm: LiteLLM Without the Bloat

**原文链接**: [https://github.com/kennethwolters/litelm](https://github.com/kennethwolters/litelm)

生成摘要时出错

---

## 95. Resist "AI"

**原文标题**: Resist "AI"

**原文链接**: [https://ronjeffries.com/articles/-v026/x/t/](https://ronjeffries.com/articles/-v026/x/t/)

生成摘要时出错

---

## 96. Mind-altering drugs played key role in rise of Andean civilization

**原文标题**: Mind-altering drugs played key role in rise of Andean civilization

**原文链接**: [https://www.science.org/content/article/mind-altering-drugs-played-key-role-rise-andean-civilization](https://www.science.org/content/article/mind-altering-drugs-played-key-role-rise-andean-civilization)

生成摘要时出错

---

## 97. CIA Releases President's Daily Briefs in Commemoration of 9/11

**原文标题**: CIA Releases President's Daily Briefs in Commemoration of 9/11

**原文链接**: [https://www.cia.gov/stories/story/cia-releases-presidents-daily-briefs-in-commemoration-of-the-25th-anniversary-of-9-11/](https://www.cia.gov/stories/story/cia-releases-presidents-daily-briefs-in-commemoration-of-the-25th-anniversary-of-9-11/)

生成摘要时出错

---

## 98. US diesel hits record $6 a gallon on Iran supply shock

**原文标题**: US diesel hits record $6 a gallon on Iran supply shock

**原文链接**: [https://www.ft.com/content/ebfa69a3-323b-450d-8bfd-0b12e01d2a5b](https://www.ft.com/content/ebfa69a3-323b-450d-8bfd-0b12e01d2a5b)

生成摘要时出错

---

## 99. AI 2027 (2025)

**原文标题**: AI 2027 (2025)

**原文链接**: [https://ai-2027.com](https://ai-2027.com)

生成摘要时出错

---

## 100. Moonshot serves Claude instead of Kimi and collects exchanges for model training

**原文标题**: Moonshot serves Claude instead of Kimi and collects exchanges for model training

**原文链接**: [https://twitter.com/DavidAgranovich/status/2098168522862215449](https://twitter.com/DavidAgranovich/status/2098168522862215449)

生成摘要时出错

---

