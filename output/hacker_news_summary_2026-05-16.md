# Hacker News 热门文章摘要 (2026-05-16)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 我相信目前许多公司都患上了“AI狂想症”。

**原文标题**: I believe there are entire companies right now under AI psychosis

**原文链接**: [https://twitter.com/mitchellh/status/2055380239711457578](https://twitter.com/mitchellh/status/2055380239711457578)

尽管提供了标题“我相信现在有整家公司都处于AI精神病状态”，但内容本身并非一篇关于此主题的文章或讨论。相反，所提供的文本是一条来自x.com（原Twitter）的错误消息。

该消息写着：“JavaScript 不可用。我们检测到此浏览器中JavaScript已禁用。请启用JavaScript或切换到受支持的浏览器以继续使用x.com。”它指示用户启用JavaScript或切换到受支持的浏览器以访问网站。该消息还包括指向帮助中心、服务条款、隐私政策、Cookie政策、版本说明和广告信息的链接，版权所有 © 2026 X Corp。

因此，没有提供与“AI精神病”相关的内容以供总结；所提供的文本是一条技术性浏览器错误消息。

---

## 2. 古腾堡计划 – 越来越好

**原文标题**: Project Gutenberg – keeps getting better

**原文链接**: [https://www.gutenberg.org/](https://www.gutenberg.org/)

古腾堡计划是一个开创性的在线图书馆，提供超过75,000本完全免费的电子书。它成立于1971年，将美国版权已过期的旧作品数字化并进行细致的校对，从而使经典文学及其他文本得以广泛传播。用户可以下载epub和Kindle格式的图书，或在线阅读，无需任何应用、费用或注册。

这个由数千名志愿者开发的庞大藏书包括《弗兰肯斯坦》和《傲慢与偏见》等热门书目、新出版物，以及从文学、历史到科学、哲学等广泛的类别。用户可以通过搜索选项、主要类别或精选阅读列表来查找书籍。

古腾堡计划还提供大量有声读物，其中包括662部人工朗读的作品，近5,000部由2023年与微软和麻省理工学院合作产生的计算机生成作品，以及LibriVox人工朗读有声读物的访问权限。

该组织以志愿者为基础运作，并依靠捐款来继续其使命。个人可以通过校对（通过分布式校对）、报告错误或录制有声读物来做出贡献。网站提供全面的帮助、常见问题解答以及阅读选项的信息。

---

## 3. arXiv 新政策：虚构参考文献禁封一年

**原文标题**: New arXiv policy: 1-year ban for hallucinated references

**原文链接**: [https://twitter.com/tdietterich/status/2055000956144935055](https://twitter.com/tdietterich/status/2055000956144935055)

提供的内​​容是x.com（原Twitter）发出的错误消息，表明JavaScript已禁用，而不是一篇关于arXiv政策的文章。

然而，*仅根据所提供的标题*：“arXiv新政策：虚构参考文献作者将被禁一年”，关键信息是arXiv已实施了一项新政策。该政策规定，提交包含虚构（捏造或不存在的）参考文献的预印本的作者将面临一年禁令。

---

## 4. 穆瓦德的出口IP竟然是可识别的

**原文标题**: Mullvad exit IPs are surprisingly identifying

**原文链接**: [https://tmctmt.com/posts/mullvad-exit-ips-as-a-fingerprinting-vector/](https://tmctmt.com/posts/mullvad-exit-ips-as-a-fingerprinting-vector/)

Mullvad的出口IP地址分配系统虽然为每台服务器提供多个IP，但已被识别为一个重要的指纹识别向量。用户在给定服务器的出口IP是根据其WireGuard密钥确定性选择的，该密钥通常每1到30天轮换一次。

研究表明，尽管理论上有数十亿种IP组合，但实际分配的独特组合数量有限。核心问题在于，对于任何给定的WireGuard密钥，在*不同*服务器上分配的出口IP始终在每个服务器各自的IP池中占据*相同的百分位*。这很可能是由于Mullvad使用基于种子的随机数生成器（可能是Rust的`rand::random_range`），其中WireGuard密钥作为种子，输出浮点数按服务器的IP池大小进行缩放。这导致了不同的绝对IP，但相对位置相同。

这一缺陷使得“关联攻击”成为可能。通过观察用户从多个Mullvad服务器的出口IP，攻击者可以推断出一个与其WireGuard密钥相关的狭窄“浮点范围”。如果两个看似不同的用户或连接表现出重叠的浮点范围，则强烈暗示他们是同一个人，有可能通过IP日志或数据泄露，以超过99%的准确率导致去匿名化。

为了缓解此问题，用户应避免使用相同的公钥频繁切换Mullvad服务器，并通过退出Mullvad应用程序主动强制轮换其公钥。

---

## 5. 阻止发行商停运线上游戏的法案在加州获推进

**原文标题**: Bill to block publishers from killing online games advances in California

**原文链接**: [https://arstechnica.com/gaming/2026/05/bill-to-keep-online-games-playable-clears-key-hurdle-in-california/](https://arstechnica.com/gaming/2026/05/bill-to-keep-online-games-playable-clears-key-hurdle-in-california/)

一项旨在确保在线游戏长期可玩性的名为《保护我们的游戏法案》的法案，已在加州议会拨款委员会获得通过，并将提交全体大会进行投票。

该拟议立法将要求数字游戏发行商，如果停止支持某款在线游戏，必须提供全额退款，或提供该游戏的更新独立版本。发行商还需要在终止基本服务前60天通知玩家。该法案一旦通过，将适用于2027年1月1日或之后在加州销售的游戏，但完全免费游戏和仅通过订阅提供的游戏除外。

该法案得到了“停止扼杀游戏”（SKG）的强力支持，该组织是一个为法案起草提供建议的玩家倡导团体，他们认为产品不应“在不通知的情况下被剥夺”。与此相反，代表主要发行商的娱乐软件协会（ESA）则反对该法案。ESA声称，消费者获得的是许可而非完全所有权，且游戏停服是现代软件的“自然特征”。他们还认为，要求无限期可玩性会给有时限的音乐和知识产权许可以及技术可行性带来不合理的负担。

尽管已通过数个委员会，该法案在提交给州长加文·纽森签署之前，仍面临重大障碍，包括在加州议会和参议院全体会议上的投票。然而，它的进展标志着“停止扼杀游戏”运动的一项重大胜利。

---

## 6. Windows XP 桌面风格探索维基百科

**原文标题**: Explore Wikipedia Like a Windows XP Desktop

**原文链接**: [https://explorer.samismith.com/](https://explorer.samismith.com/)

由sami.smith.com开发的“维基百科文件浏览器”项目，重新构想了在Windows XP桌面界面中浏览维基百科的方式。它的目标是让维基百科的分类可以像文件夹一样导航，文章可以像文档一样打开，从而提供对几乎所有维基百科内容的访问。

除了维基百科之外，“媒体”部分允许用户探索维基共享资源的分类，并具备一项独特功能：右键点击任何图片即可将其设置为桌面背景。一项正在开发中的功能“地理文件浏览器”构想将地球作为一个可导航的文件夹，用户可以在其中上传图片或添加文本注释。

Readme.txt文件提供了Sami Smith的联系方式，包括电子邮件、Twitter和Blue Sky，并列举了几个启发性项目，例如Neal.fun的Wiki Files和react-xp.jamiepates.com。它阐明“维基百科”和“媒体”部分中的内容属于维基媒体，并鼓励用户通过编辑维基百科和维基媒体来为文件夹结构做出贡献。整体体验模仿了经典的Windows XP环境，包含“开始”菜单、“我的文档”、“控制面板”等熟悉元素。

---

## 7. 英国政府用自行开发的难民系统取代了Palantir软件

**原文标题**: UK government replaces Palantir software with internally-built refugee system

**原文链接**: [https://www.bbc.com/news/articles/c2l2j1lxdk5o](https://www.bbc.com/news/articles/c2l2j1lxdk5o)

生成摘要时出错

---

## 8. Codex is now in the ChatGPT mobile app

**原文标题**: Codex is now in the ChatGPT mobile app

**原文链接**: [https://openai.com/index/work-with-codex-from-anywhere/](https://openai.com/index/work-with-codex-from-anywhere/)

生成摘要时出错

---

## 9. U.S. DOJ demands Apple and Google unmask over 100k users of car-tinkering app

**原文标题**: U.S. DOJ demands Apple and Google unmask over 100k users of car-tinkering app

**原文链接**: [https://macdailynews.com/2026/05/15/u-s-doj-demands-apple-and-google-unmask-over-100000-users-of-popular-car-tinkering-app-in-emissions-crackdown/](https://macdailynews.com/2026/05/15/u-s-doj-demands-apple-and-google-unmask-over-100000-users-of-popular-car-tinkering-app-in-emissions-crackdown/)

生成摘要时出错

---

## 10. Bun Rust 重写：代码库未能通过基本的 Miri 检查，导致 Safe Rust 中出现未定义行为。

**原文标题**: Bun Rust rewrite: "codebase fails basic miri checks, allows for UB in safe rust"

**原文链接**: [https://github.com/oven-sh/bun/issues/30719](https://github.com/oven-sh/bun/issues/30719)

An issue (#30719) has been filed against the Bun project's Rust rewrite, alleging that the codebase "fails even the most basic miri checks" and permits Undefined Behavior (UB) in ostensibly safe Rust code.

The specific Miri error reported is: "constructing invalid value of type &[u8]: encountered a dangling reference," occurring within the `PathString::slice` function at `src/main.rs:97:18`. The problem arises when `core::slice::from_raw_parts` is used with a pointer to memory that has already been deallocated.

The provided example code illustrates this: a `PathString` is initialized using a reference to data owned by a `Box<[u8]>`. However, the `Box` is subsequently dropped, freeing the underlying memory, *before* `PathString::slice()` is called. This results in the `slice` method attempting to access a dangling pointer, leading to guaranteed Undefined Behavior.

The issue reporter, AwesomeQubic, criticizes the project's coding practices, stating, "AIs are not good at writing Rust," and recommends hiring "a real rust dev," implying a lack of proper Rust expertise or reliance on inadequate automated code generation. The report underscores a critical failure in memory safety that undermines Rust's core guarantees.

---

## 11. A few words on DS4

**原文标题**: A few words on DS4

**原文链接**: [https://antirez.com/news/165](https://antirez.com/news/165)

生成摘要时出错

---

## 12. A 0-click exploit chain for the Pixel 10

**原文标题**: A 0-click exploit chain for the Pixel 10

**原文链接**: [https://projectzero.google/2026/05/pixel-10-exploit.html](https://projectzero.google/2026/05/pixel-10-exploit.html)

生成摘要时出错

---

## 13. 'No way to prevent this,' says only package manager where this regularly happens

**原文标题**: 'No way to prevent this,' says only package manager where this regularly happens

**原文链接**: [https://kevinpatel.xyz/posts/no-way-to-prevent-this/](https://kevinpatel.xyz/posts/no-way-to-prevent-this/)

生成摘要时出错

---

## 14. Amazon workers under pressure to up their AI usage are making up tasks

**原文标题**: Amazon workers under pressure to up their AI usage are making up tasks

**原文链接**: [https://www.fastcompany.com/91541586/amazon-workers-pressured-to-up-ai-use-extraneous-tasks](https://www.fastcompany.com/91541586/amazon-workers-pressured-to-up-ai-use-extraneous-tasks)

生成摘要时出错

---

## 15. ABC News has taken all FiveThirtyEight articles offline

**原文标题**: ABC News has taken all FiveThirtyEight articles offline

**原文链接**: [https://twitter.com/baseballot/status/2055309076209492208](https://twitter.com/baseballot/status/2055309076209492208)

生成摘要时出错

---

## 16. We are retiring our bug bounty program

**原文标题**: We are retiring our bug bounty program

**原文链接**: [https://turso.tech/blog/the-wonders-of-ai](https://turso.tech/blog/the-wonders-of-ai)

生成摘要时出错

---

## 17. Moving away from Tailwind, and learning to structure my CSS

**原文标题**: Moving away from Tailwind, and learning to structure my CSS

**原文链接**: [https://jvns.ca/blog/2026/05/15/moving-away-from-tailwind--and-learning-to-structure-my-css-/](https://jvns.ca/blog/2026/05/15/moving-away-from-tailwind--and-learning-to-structure-my-css-/)

生成摘要时出错

---

## 18. Ontario auditors find doctors' AI note takers routinely blow basic facts

**原文标题**: Ontario auditors find doctors' AI note takers routinely blow basic facts

**原文链接**: [https://www.theregister.com/ai-ml/2026/05/14/ontario-auditors-find-doctors-ai-note-takers-routinely-blow-basic-facts/5240771](https://www.theregister.com/ai-ml/2026/05/14/ontario-auditors-find-doctors-ai-note-takers-routinely-blow-basic-facts/5240771)

生成摘要时出错

---

## 19. SQL patterns I use to catch transaction fraud

**原文标题**: SQL patterns I use to catch transaction fraud

**原文链接**: [https://analytics.fixelsmith.com/posts/sql-fraud-patterns/](https://analytics.fixelsmith.com/posts/sql-fraud-patterns/)

生成摘要时出错

---

## 20. The Zulip Foundation

**原文标题**: The Zulip Foundation

**原文链接**: [https://blog.zulip.com/2026/05/15/announcing-zulip-foundation/](https://blog.zulip.com/2026/05/15/announcing-zulip-foundation/)

生成摘要时出错

---

## 21. Frontier AI has broken the open CTF format

**原文标题**: Frontier AI has broken the open CTF format

**原文链接**: [https://kabir.au/blog/the-ctf-scene-is-dead](https://kabir.au/blog/the-ctf-scene-is-dead)

生成摘要时出错

---

## 22. Show HN: Find the best local LLM for your hardware, ranked by benchmarks

**原文标题**: Show HN: Find the best local LLM for your hardware, ranked by benchmarks

**原文链接**: [https://github.com/Andyyyy64/whichllm](https://github.com/Andyyyy64/whichllm)

生成摘要时出错

---

## 23. The sigmoids won't save you

**原文标题**: The sigmoids won't save you

**原文链接**: [https://www.astralcodexten.com/p/the-sigmoids-wont-save-you](https://www.astralcodexten.com/p/the-sigmoids-wont-save-you)

生成摘要时出错

---

## 24. Details of the Daring Airdrop at Tristan Da Cunha

**原文标题**: Details of the Daring Airdrop at Tristan Da Cunha

**原文链接**: [https://www.tristandc.com/government/news-2026-05-11-airdrop.php](https://www.tristandc.com/government/news-2026-05-11-airdrop.php)

生成摘要时出错

---

## 25. Radicle: Sovereign {code forge} built on Git

**原文标题**: Radicle: Sovereign {code forge} built on Git

**原文链接**: [https://radicle.dev/](https://radicle.dev/)

生成摘要时出错

---

## 26. SANA-WM, a 2.6B open-source world model for 1-minute 720p video

**原文标题**: SANA-WM, a 2.6B open-source world model for 1-minute 720p video

**原文链接**: [https://nvlabs.github.io/Sana/WM/](https://nvlabs.github.io/Sana/WM/)

生成摘要时出错

---

## 27. Bitwarden scrubs 'Always free' and 'Inclusion' values from its site

**原文标题**: Bitwarden scrubs 'Always free' and 'Inclusion' values from its site

**原文链接**: [https://www.fastcompany.com/91542655/bitwarden-scrubs-always-free-and-inclusion-values-from-its-website-as-longtime-execs-step-down](https://www.fastcompany.com/91542655/bitwarden-scrubs-always-free-and-inclusion-values-from-its-website-as-longtime-execs-step-down)

生成摘要时出错

---

## 28. More than sixty percent of the United States is experiencing drought conditions

**原文标题**: More than sixty percent of the United States is experiencing drought conditions

**原文链接**: [https://news.vt.edu/articles/2026/05/drought-united-states-la-nina-expert.html](https://news.vt.edu/articles/2026/05/drought-united-states-la-nina-expert.html)

生成摘要时出错

---

## 29. Fecal transplants for autism deliver success in clinical trials (2025)

**原文标题**: Fecal transplants for autism deliver success in clinical trials (2025)

**原文链接**: [https://refractor.io/adhd-autism/fecal-transplants-for-autism-delivers-success-in-clinical-trials/](https://refractor.io/adhd-autism/fecal-transplants-for-autism-delivers-success-in-clinical-trials/)

生成摘要时出错

---

## 30. Erlang/OTP 29.0

**原文标题**: Erlang/OTP 29.0

**原文链接**: [https://www.erlang.org/news/188](https://www.erlang.org/news/188)

生成摘要时出错

---

## 31. Welcome to the Strip Mining Era of OSS Security

**原文标题**: Welcome to the Strip Mining Era of OSS Security

**原文链接**: [https://www.metabase.com/blog/strip-mining-era-of-open-source-security](https://www.metabase.com/blog/strip-mining-era-of-open-source-security)

生成摘要时出错

---

## 32. I designed a nibble-oriented CPU in Verilog to build a scientific calculator

**原文标题**: I designed a nibble-oriented CPU in Verilog to build a scientific calculator

**原文链接**: [https://github.com/gdevic/FPGA-Calculator](https://github.com/gdevic/FPGA-Calculator)

生成摘要时出错

---

## 33. Solar-based sleep patterns compared to modern norms

**原文标题**: Solar-based sleep patterns compared to modern norms

**原文链接**: [https://dylan.gr/1775146616](https://dylan.gr/1775146616)

生成摘要时出错

---

## 34. Judge bars Kars4Kids from broadcasting 'misleading' ads in California

**原文标题**: Judge bars Kars4Kids from broadcasting 'misleading' ads in California

**原文链接**: [https://www.nytimes.com/2026/05/15/us/kars4kids-advertising-banned-california.html](https://www.nytimes.com/2026/05/15/us/kars4kids-advertising-banned-california.html)

生成摘要时出错

---

## 35. Show HN: Burn, baby, burn (those tokens)

**原文标题**: Show HN: Burn, baby, burn (those tokens)

**原文链接**: [https://github.com/dtnewman/burn-baby-burn](https://github.com/dtnewman/burn-baby-burn)

生成摘要时出错

---

## 36. US is starting to see heavy job losses in roles exposed to AI

**原文标题**: US is starting to see heavy job losses in roles exposed to AI

**原文链接**: [https://www.bloomberg.com/news/articles/2026-05-15/us-is-starting-to-see-heavy-job-losses-in-roles-exposed-to-ai](https://www.bloomberg.com/news/articles/2026-05-15/us-is-starting-to-see-heavy-job-losses-in-roles-exposed-to-ai)

生成摘要时出错

---

## 37. OpenClaw Creator Spent $1.3M on OpenAI Tokens in 30 Days

**原文标题**: OpenClaw Creator Spent $1.3M on OpenAI Tokens in 30 Days

**原文链接**: [https://twitter.com/steipete/status/2055346265869721905](https://twitter.com/steipete/status/2055346265869721905)

生成摘要时出错

---

## 38. reCAPTCHA Mobile Verification Is Bringing the Play Integrity API to Desktops

**原文标题**: reCAPTCHA Mobile Verification Is Bringing the Play Integrity API to Desktops

**原文链接**: [https://discuss.grapheneos.org/d/35428-recaptcha-mobile-verification-is-bringing-the-play-integrity-api-to-desktops](https://discuss.grapheneos.org/d/35428-recaptcha-mobile-verification-is-bringing-the-play-integrity-api-to-desktops)

生成摘要时出错

---

## 39. NYT and vaping: How to lie by saying only true things (2022)

**原文标题**: NYT and vaping: How to lie by saying only true things (2022)

**原文链接**: [https://gwern.net/vaping](https://gwern.net/vaping)

生成摘要时出错

---

## 40. UK sovereign LLM inference

**原文标题**: UK sovereign LLM inference

**原文链接**: [https://relax.ai/docs](https://relax.ai/docs)

生成摘要时出错

---

## 41. Europe built sovereign clouds to escape US control. Forgot about the processors

**原文标题**: Europe built sovereign clouds to escape US control. Forgot about the processors

**原文链接**: [https://www.theregister.com/systems/2026/05/16/europe-built-sovereign-clouds-to-escape-us-control-then-forgot-about-the-processors/5237735](https://www.theregister.com/systems/2026/05/16/europe-built-sovereign-clouds-to-escape-us-control-then-forgot-about-the-processors/5237735)

生成摘要时出错

---

## 42. High dimensional geometry is transforming the MRI industry (2017) [pdf]

**原文标题**: High dimensional geometry is transforming the MRI industry (2017) [pdf]

**原文链接**: [https://www.ams.org/government/DonohoPresentation06-28-17Final.pdf](https://www.ams.org/government/DonohoPresentation06-28-17Final.pdf)

生成摘要时出错

---

## 43. Cursing the government does not fix potholes. Spray-painting them does

**原文标题**: Cursing the government does not fix potholes. Spray-painting them does

**原文链接**: [https://imagenotfound.writeas.com/the-holes-we-painted-and-why-we-did-it-anyway](https://imagenotfound.writeas.com/the-holes-we-painted-and-why-we-did-it-anyway)

生成摘要时出错

---

## 44. We don't know why Malawi is poor

**原文标题**: We don't know why Malawi is poor

**原文链接**: [https://newsletter.deenamousa.com/p/we-dont-know-why-malawi-is-poor](https://newsletter.deenamousa.com/p/we-dont-know-why-malawi-is-poor)

生成摘要时出错

---

## 45. LLM Policy for Rust Compiler

**原文标题**: LLM Policy for Rust Compiler

**原文链接**: [https://github.com/rust-lang/rust-forge/pull/1040](https://github.com/rust-lang/rust-forge/pull/1040)

生成摘要时出错

---

## 46. Futhark by example

**原文标题**: Futhark by example

**原文链接**: [https://futhark-lang.org/examples.html](https://futhark-lang.org/examples.html)

生成摘要时出错

---

## 47. OpenAI is connecting ChatGPT to bank accounts via Plaid

**原文标题**: OpenAI is connecting ChatGPT to bank accounts via Plaid

**原文链接**: [https://firethering.com/chatgpt-bank-account-plaid-openai/](https://firethering.com/chatgpt-bank-account-plaid-openai/)

生成摘要时出错

---

## 48. OVMS: Open source electric vehicle remote monitoring, diagnosis and control

**原文标题**: OVMS: Open source electric vehicle remote monitoring, diagnosis and control

**原文链接**: [https://www.openvehicles.com/home](https://www.openvehicles.com/home)

生成摘要时出错

---

## 49. UK Government Kicks Out Palantir

**原文标题**: UK Government Kicks Out Palantir

**原文链接**: [https://shkspr.mobi/blog/2026/05/uk-government-kicks-out-palantir/](https://shkspr.mobi/blog/2026/05/uk-government-kicks-out-palantir/)

生成摘要时出错

---

## 50. An australian teen team is making radio astronomy affordable for rural schools

**原文标题**: An australian teen team is making radio astronomy affordable for rural schools

**原文链接**: [https://mag.openrockets.com/p/how-an-australian-teen-team-is-making-radio-astronomy-affordable-for-rural-schools-4894opuisyhfdisubgi/?b=2](https://mag.openrockets.com/p/how-an-australian-teen-team-is-making-radio-astronomy-affordable-for-rural-schools-4894opuisyhfdisubgi/?b=2)

生成摘要时出错

---

## 51. I love Linux, but I can't quit Windows

**原文标题**: I love Linux, but I can't quit Windows

**原文链接**: [https://jpain.io/i-love-linux-but-i-cant-quit-windows/](https://jpain.io/i-love-linux-but-i-cant-quit-windows/)

生成摘要时出错

---

## 52. A Meta employee gets real about the horror of working there

**原文标题**: A Meta employee gets real about the horror of working there

**原文链接**: [https://sfstandard.com/pacific-standard-time/2026/05/15/meta-employee-gets-real-horror-working-right-now/](https://sfstandard.com/pacific-standard-time/2026/05/15/meta-employee-gets-real-horror-working-right-now/)

生成摘要时出错

---

## 53. Show HN: Epiq – Distributed Git based issue tracker TUI

**原文标题**: Show HN: Epiq – Distributed Git based issue tracker TUI

**原文链接**: [https://ljtn.github.io/epiq/](https://ljtn.github.io/epiq/)

生成摘要时出错

---

## 54. Greek Alphabet Cards

**原文标题**: Greek Alphabet Cards

**原文链接**: [https://labs.randomquark.com/alphabet_cards/](https://labs.randomquark.com/alphabet_cards/)

生成摘要时出错

---

## 55. DeepSeek V4: The Open-Source Model Frontier Labs Feared

**原文标题**: DeepSeek V4: The Open-Source Model Frontier Labs Feared

**原文链接**: [https://helloai.com/articles/deepseek-v4-open-source-frontier-parity](https://helloai.com/articles/deepseek-v4-open-source-frontier-parity)

生成摘要时出错

---

## 56. My Favorite Bugs: Invalid Surrogate Pairs

**原文标题**: My Favorite Bugs: Invalid Surrogate Pairs

**原文链接**: [https://george.mand.is/2026/05/my-favorite-bugs-invalid-surrogate-pairs/](https://george.mand.is/2026/05/my-favorite-bugs-invalid-surrogate-pairs/)

生成摘要时出错

---

## 57. Microscale Thermite Reaction

**原文标题**: Microscale Thermite Reaction

**原文链接**: [https://sciencedemonstrations.fas.harvard.edu/presentations/microscale-thermite-reaction](https://sciencedemonstrations.fas.harvard.edu/presentations/microscale-thermite-reaction)

生成摘要时出错

---

## 58. Zenith: a live local-first fixed viewport planetarium

**原文标题**: Zenith: a live local-first fixed viewport planetarium

**原文链接**: [https://smorgasb.org/zenith-tech/](https://smorgasb.org/zenith-tech/)

生成摘要时出错

---

## 59. We've made the world too complicated

**原文标题**: We've made the world too complicated

**原文链接**: [https://user8.bearblog.dev/the-world-is-too-complicated/](https://user8.bearblog.dev/the-world-is-too-complicated/)

生成摘要时出错

---

## 60. 7 in 10 Americans oppose data centers being built in their communities

**原文标题**: 7 in 10 Americans oppose data centers being built in their communities

**原文链接**: [https://www.washingtonpost.com/nation/2026/05/13/7-10-americans-oppose-data-centers-being-built-their-communities/](https://www.washingtonpost.com/nation/2026/05/13/7-10-americans-oppose-data-centers-being-built-their-communities/)

生成摘要时出错

---

## 61. Have a Coherent AI Policy

**原文标题**: Have a Coherent AI Policy

**原文链接**: [https://brianmeeker.me/2026/05/14/have-a-coherent-ai-policy/](https://brianmeeker.me/2026/05/14/have-a-coherent-ai-policy/)

生成摘要时出错

---

## 62. Check your fucking sources, people

**原文标题**: Check your fucking sources, people

**原文链接**: [https://brodzinski.com/2026/05/check-fcking-sources.html](https://brodzinski.com/2026/05/check-fcking-sources.html)

生成摘要时出错

---

## 63. Building a UMatrix Replacement

**原文标题**: Building a UMatrix Replacement

**原文链接**: [https://lock.cmpxchg8b.com/umatrix.html](https://lock.cmpxchg8b.com/umatrix.html)

生成摘要时出错

---

## 64. Show HN: GlycemicGPT – Open-source AI-powered diabetes management

**原文标题**: Show HN: GlycemicGPT – Open-source AI-powered diabetes management

**原文链接**: [https://github.com/GlycemicGPT/GlycemicGPT](https://github.com/GlycemicGPT/GlycemicGPT)

生成摘要时出错

---

## 65. Accelerate

**原文标题**: Accelerate

**原文链接**: [https://github.com/AccelerateHS/accelerate](https://github.com/AccelerateHS/accelerate)

生成摘要时出错

---

## 66. Why is this site named Antipope?

**原文标题**: Why is this site named Antipope?

**原文链接**: [https://www.antipope.org/charlie/old/antipope.html](https://www.antipope.org/charlie/old/antipope.html)

生成摘要时出错

---

## 67. Elevated error rates on Opus 4.7

**原文标题**: Elevated error rates on Opus 4.7

**原文链接**: [https://status.claude.com/incidents/8z7l5zcy0v3b](https://status.claude.com/incidents/8z7l5zcy0v3b)

生成摘要时出错

---

## 68. Court bans Kars4Kids ads in California for violating false advertising law

**原文标题**: Court bans Kars4Kids ads in California for violating false advertising law

**原文链接**: [https://www.sfgate.com/bayarea/article/kars4kids-california-false-advertising-22259298.php](https://www.sfgate.com/bayarea/article/kars4kids-california-false-advertising-22259298.php)

生成摘要时出错

---

## 69. Feedr v0.8.0 – a TUI RSS reader, now read the full article from your terminal

**原文标题**: Feedr v0.8.0 – a TUI RSS reader, now read the full article from your terminal

**原文链接**: [https://github.com/bahdotsh/feedr](https://github.com/bahdotsh/feedr)

生成摘要时出错

---

## 70. Overseas fakers using AI videos to push a narrative of UK decline, BBC finds

**原文标题**: Overseas fakers using AI videos to push a narrative of UK decline, BBC finds

**原文链接**: [https://www.bbc.co.uk/news/articles/ckgpyn30dp3o](https://www.bbc.co.uk/news/articles/ckgpyn30dp3o)

生成摘要时出错

---

## 71. Show HN: GridTravel – A community based travel app for users to share routes

**原文标题**: Show HN: GridTravel – A community based travel app for users to share routes

**原文链接**: [https://www.gridtravel.app](https://www.gridtravel.app)

生成摘要时出错

---

## 72. NanoTDB – Golang Append-Only Time Series DB

**原文标题**: NanoTDB – Golang Append-Only Time Series DB

**原文链接**: [https://github.com/aymanhs/nanotdb](https://github.com/aymanhs/nanotdb)

生成摘要时出错

---

## 73. Hawaii passes law bypassing Citizens United, governor signs it

**原文标题**: Hawaii passes law bypassing Citizens United, governor signs it

**原文链接**: [https://ca.news.yahoo.com/hawaii-law-targets-corporate-influence-024038159.html](https://ca.news.yahoo.com/hawaii-law-targets-corporate-influence-024038159.html)

生成摘要时出错

---

## 74. Where's Ed: Anthropic Told Court $5B but Public $19B

**原文标题**: Where's Ed: Anthropic Told Court $5B but Public $19B

**原文链接**: [https://www.flyingpenguin.com/wheres-ed-anthropic-told-court-5-billion-but-public-19-billion/](https://www.flyingpenguin.com/wheres-ed-anthropic-told-court-5-billion-but-public-19-billion/)

生成摘要时出错

---

## 75. Git Is Not Fine

**原文标题**: Git Is Not Fine

**原文链接**: [https://www.billjings.com/posts/title/git-is-not-fine/](https://www.billjings.com/posts/title/git-is-not-fine/)

生成摘要时出错

---

## 76. Someone Shared a Real Monet Painting as AI and Asked for Critiques

**原文标题**: Someone Shared a Real Monet Painting as AI and Asked for Critiques

**原文链接**: [https://petapixel.com/2026/05/14/someone-shared-a-real-monet-painting-as-ai-and-asked-for-critiques/](https://petapixel.com/2026/05/14/someone-shared-a-real-monet-painting-as-ai-and-asked-for-critiques/)

生成摘要时出错

---

## 77. Tesla reveals two Robotaxi crashes involving teleoperators

**原文标题**: Tesla reveals two Robotaxi crashes involving teleoperators

**原文链接**: [https://techcrunch.com/2026/05/15/tesla-reveals-two-robotaxi-crashes-involving-teleoperators/](https://techcrunch.com/2026/05/15/tesla-reveals-two-robotaxi-crashes-involving-teleoperators/)

生成摘要时出错

---

## 78. Fired hacker twins forget to end Teams recording, capture own crimes

**原文标题**: Fired hacker twins forget to end Teams recording, capture own crimes

**原文链接**: [https://arstechnica.com/tech-policy/2026/05/fired-hacker-twins-forget-to-end-teams-recording-capture-own-crimes/](https://arstechnica.com/tech-policy/2026/05/fired-hacker-twins-forget-to-end-teams-recording-capture-own-crimes/)

生成摘要时出错

---

## 79. Why Spain has the greatest cities

**原文标题**: Why Spain has the greatest cities

**原文链接**: [https://worksinprogress.co/issue/why-spain-has-the-worlds-greatest-cities/](https://worksinprogress.co/issue/why-spain-has-the-worlds-greatest-cities/)

生成摘要时出错

---

## 80. Kioxia and Dell cram 10 PB into slim 2RU server

**原文标题**: Kioxia and Dell cram 10 PB into slim 2RU server

**原文链接**: [https://www.blocksandfiles.com/flash/2026/05/14/kioxia-and-dell-cram-10-pb-into-slim-2ru-server/5240574](https://www.blocksandfiles.com/flash/2026/05/14/kioxia-and-dell-cram-10-pb-into-slim-2ru-server/5240574)

生成摘要时出错

---

## 81. Show HN: Sx – an open-source package manager for AI skills, MCPs, and commands

**原文标题**: Show HN: Sx – an open-source package manager for AI skills, MCPs, and commands

**原文链接**: [https://github.com/sleuth-io/sx](https://github.com/sleuth-io/sx)

生成摘要时出错

---

## 82. An Engineer's Post Protesting Laptop Surveillance Is Going Viral Inside Meta

**原文标题**: An Engineer's Post Protesting Laptop Surveillance Is Going Viral Inside Meta

**原文链接**: [https://www.wired.com/story/meta-employee-protest-mouse-tracking-surveillance-ai-training/](https://www.wired.com/story/meta-employee-protest-mouse-tracking-surveillance-ai-training/)

生成摘要时出错

---

## 83. California's Battery Array Is as Powerful as 12 Nuclear Power Plants

**原文标题**: California's Battery Array Is as Powerful as 12 Nuclear Power Plants

**原文链接**: [https://zolairenergy.com/californias-battery-array-is-as-powerful-as-12-nuclear-power-plants-heres-whats-on-the-horizon/](https://zolairenergy.com/californias-battery-array-is-as-powerful-as-12-nuclear-power-plants-heres-whats-on-the-horizon/)

生成摘要时出错

---

## 84. Geography is four-dimensional

**原文标题**: Geography is four-dimensional

**原文链接**: [https://sive.rs/4d](https://sive.rs/4d)

生成摘要时出错

---

## 85. Green Card Holders Targeted for Deportation by New 'Removal Apparatus'

**原文标题**: Green Card Holders Targeted for Deportation by New 'Removal Apparatus'

**原文链接**: [https://www.nytimes.com/2026/05/14/us/politics/green-cards-immigration-deportation-trump.html](https://www.nytimes.com/2026/05/14/us/politics/green-cards-immigration-deportation-trump.html)

生成摘要时出错

---

## 86. Echoes (Live at Pompeii) (1972)

**原文标题**: Echoes (Live at Pompeii) (1972)

**原文链接**: [https://genius.com/Pink-floyd-echoes-live-at-pompeii-lyrics](https://genius.com/Pink-floyd-echoes-live-at-pompeii-lyrics)

生成摘要时出错

---

## 87. AI is wiping out entry-level jobs

**原文标题**: AI is wiping out entry-level jobs

**原文链接**: [https://fortune.com/2026/05/15/ai-entry-level-jobs-higher-education-experience-gap/](https://fortune.com/2026/05/15/ai-entry-level-jobs-higher-education-experience-gap/)

生成摘要时出错

---

## 88. New Linux LPE, 5.10 and above (ptrace_may_access mm-NULL + pidfd_getfd)

**原文标题**: New Linux LPE, 5.10 and above (ptrace_may_access mm-NULL + pidfd_getfd)

**原文链接**: [https://github.com/0xdeadbeefnetwork/ssh-keysign-pwn](https://github.com/0xdeadbeefnetwork/ssh-keysign-pwn)

生成摘要时出错

---

## 89. Best "Brain" for Agents Is Just Versioned Folders of Markdown Files

**原文标题**: Best "Brain" for Agents Is Just Versioned Folders of Markdown Files

**原文链接**: [https://extency.com/blog/markdown-versioned-folders-agent-brain-2026](https://extency.com/blog/markdown-versioned-folders-agent-brain-2026)

生成摘要时出错

---

## 90. Codex is now available on mobile via ChatGPT app

**原文标题**: Codex is now available on mobile via ChatGPT app

**原文链接**: [https://twitter.com/openai/status/2055016850849993072](https://twitter.com/openai/status/2055016850849993072)

生成摘要时出错

---

