# Hacker News 热门文章摘要 (2026-04-02)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 报告大幅增加

**原文标题**: Significant Raise of Reports

**原文链接**: [https://lwn.net/Articles/1065620/](https://lwn.net/Articles/1065620/)

文章报道称，内核安全邮件列表上的安全漏洞报告出现了显著而快速的增长。两年前每周只有2-3份报告，去年增至每周约10份（常是“AI垃圾”），而自2026年初以来，这一数字已惊人地跃升至每天5-10份。与之前的“AI垃圾”不同，这些新报告大多是正确的，需要更多的维护者，并导致每天都发现重复的漏洞。

尽管报告速度的加快“令人担忧且疲惫不堪”，作者指出修复可能被犯罪分子利用的真实漏洞带来了满足感，并推测这种高强度工作可能正在清除长期积压的漏洞。

作者预测软件安全实践将发生根本性转变：
1. **禁运消失：** 由于漏洞很容易被重新发现，隐藏它们将变得毫无意义。
2. **关注更新：** 人们将明白安全漏洞仅仅是漏洞，因此定期软件更新（而非关注特定的CVE）将是保持安全的唯一明智方式。
3. **强制维护：** 那些历来忽视持续维护的项目将被迫适应，因为所有软件都将成为持续攻击的目标。

最终，作者预见软件质量将回归更高的水平，类似于2000年前的严格标准，但承认这将经历一个持续数年的“巨大混乱”时期。

---

## 2. OpenAI 墓地：所有未能实现的交易和产品

**原文标题**: The OpenAI graveyard: All the deals and products that haven't happened

**原文链接**: [https://www.forbes.com/sites/phoebeliu/2026/03/31/openai-graveyard-deals-and-products-havent-happened-openai/](https://www.forbes.com/sites/phoebeliu/2026/03/31/openai-graveyard-deals-and-products-havent-happened-openai/)

无法访问文章链接。

---

## 3. Neanderthals survived on a knife's edge for 350k years

**原文标题**: Neanderthals survived on a knife's edge for 350k years

**原文链接**: [https://www.science.org/content/article/neanderthals-survived-knife-s-edge-350-000-years](https://www.science.org/content/article/neanderthals-survived-knife-s-edge-350-000-years)

生成摘要时出错

---

## 4. 我们拦截了白宫应用的流量。

**原文标题**: We intercepted the White House app's network traffic

**原文链接**: [https://www.atomic.computer/blog/white-house-app-network-traffic-analysis/](https://www.atomic.computer/blog/white-house-app-network-traffic-analysis/)

通过MITM代理对白宫iOS应用（v47.0.4）进行的动态分析显示，该应用存在大量第三方网络活动，与其隐私声明相悖。在206个由应用发起的请求中，只有48个（23%）指向whitehouse.gov，其余77%联系了31个独特的第三方服务，如Elfsight、OneSignal、YouTube、Google DoubleClick、Facebook和Twitter。

应用启动时，第三方分析公司OneSignal会收到用户的“实时画像”。这包括语言、时区、国家、完整IP地址、首次和末次活动的确切时间戳、设备型号和操作系统、网络类型、运营商、越狱状态、会话次数、会话持续时间以及一个持久的唯一标识符。该画像会在不同会话间更新。

该应用还联系了13个Elfsight域名，证实了一个两阶段JavaScript加载器，允许Elfsight服务器注入各种社交媒体小部件脚本（例如TikTok、Instagram）并设置超过10个跟踪cookie。此外，YouTube嵌入内容会触发谷歌的DoubleClick广告投放和跟踪基础设施。

尽管有这些发现，该应用的隐私声明却虚假地声称“未收集数据”和“NSPrivacyTracking: false”。分析总结道，官方白宫应用存在大量未披露的第三方数据收集和跟踪行为。

---

## 5. 用于 ocamlc 的新 C++ 后端

**原文标题**: A new C++ back end for ocamlc

**原文链接**: [https://github.com/ocaml/ocaml/pull/14701](https://github.com/ocaml/ocaml/pull/14701)

一则愚人节公告推出 `ocamlc` 的新 C++ 后端，使得 OCaml 程序能够使用 `ocamlc -incr-c primes.ml` 命令编译成 C++ 模板元编程代码。该后端旨在改进现有的 C 运行时和 FFI（外部函数接口），将 OCaml 的列表和函数等构造翻译成冗长的 C++ 模板结构体。

提供了一个 OCaml 质数筛示例程序，演示了整数、列表 cons 单元格 (`Cons`) 和函数应用 (`app`) 如何在生成的 C++ 中表示。运行带有 `g++ -Dlimit=N` 参数的 C++ 代码的输出被幽默地格式化为编译器错误消息。

C++ 模板的“纯函数式”特性意味着 OCaml 的可变标准库不可用，需要进行纯函数式的重新实现。性能被认为是一个重大挑战：计算高达 10,000 的质数会消耗“大约 11 GiB 的内存”，并且需要调整 `ftemplate-depth` 参数。据称 `clang++` 会出现段错误。尽管算法改进可以加速执行，内存使用量仍然巨大。

这场日期为 2026 年 4 月 1 日的讨论，进一步证实了这个精心设计的笑话，参与者提出了幽默的问题，涉及非均匀递归数据类型等特性，并对 C++ 的固有特性发表评论。

---

## 6. 揭秘尼泊尔虚假救援骗局

**原文标题**: Inside Nepal's Fake Rescue Racket

**原文链接**: [https://kathmandupost.com/money/2026/03/27/inside-nepal-s-fake-rescue-racket](https://kathmandupost.com/money/2026/03/27/inside-nepal-s-fake-rescue-racket)

所提供的文章标题“尼泊尔假救援骗局内幕”暗示了一篇关于尼泊尔境内涉及欺诈性救援活动的不法操作的报道。

然而，所提供的内容**与该标题不符**。唯一给出的信息是：“尼泊尔证券交易所收盘上涨至2,782.18点，成交额达88.1亿卢比。”

因此，*仅*根据所提供的内容，该文章报道称尼泊尔证券交易所（Nepse）当天交易收盘上涨至2,782.18点，总成交额达88.1亿卢比。所提供文本中不包含任何关于“假救援骗局”的信息。

---

## 7. 德尔夫据称盗用了一个开源工具，并将其作为自己的产品出售。

**原文标题**: Delve allegedly forked an open-source tool and sold it as its own

**原文链接**: [https://techcrunch.com/2026/04/01/the-reputation-of-troubled-yc-startup-delve-has-gotten-even-worse/](https://techcrunch.com/2026/04/01/the-reputation-of-troubled-yc-startup-delve-has-gotten-even-worse/)

合规初创公司Delve陷入新的争议，一位名叫“DeepDelver”的匿名举报人指控称，该公司非法分叉了Sim.ai的一款名为SimStudio的开源工具，并将其作为Delve自有的“Pathways”产品出售。DeepDelver声称，Delve曾将“Pathways”宣传为内部开发的产品，尽管其与SimStudio非常相似。如果属实，此举将违反要求注明出处的Apache软件许可证。

Sim.ai的创始人兼首席执行官埃米尔·卡拉贝格（Emir Karabeg）向TechCrunch证实，Delve并未获得SimStudio的许可协议。卡拉贝格表示，他并不知道Delve会销售一个修改版本作为独立的解决方案，特别是考虑到Sim.ai此前曾是Delve的客户。卡拉贝格此前曾就Delve伪造客户数据的指控安抚过其创始人，但在得知Sim.ai的指控后，他已停止与Delve联系。

在这些指控浮出水面后，据报道，Delve已从其网站上删除了所有提及“Pathways”以及许多其他页面的内容，其媒体问询邮箱也已失效。该公司尚未回应置评请求。Delve的A轮投资者Insight Partners此前短暂下架了其关于该投资的博客文章，其在LinkedIn上的帖子也仍未恢复。此事件引发了强烈反响，并在X平台上成为热门话题。

---

## 8. 美产水泥和混凝土的AI

**原文标题**: AI for American-produced cement and concrete

**原文链接**: [https://engineering.fb.com/2026/03/30/data-center-engineering/ai-for-american-produced-cement-and-concrete/](https://engineering.fb.com/2026/03/30/data-center-engineering/ai-for-american-produced-cement-and-concrete/)

Meta is advancing the U.S. construction industry by leveraging AI to produce high-quality, sustainable concrete mixes using domestically sourced materials, aiming to reduce reliance on imported cement. Concurrent with the 2026 ACI Spring Convention, Meta is releasing an open-source AI model, Bayesian Optimization for Concrete (BOxCrete), and foundational data for developing concrete mixes.

The U.S. imports 20-25% of its cement, impacting domestic manufacturing, jobs, and adherence to U.S. environmental standards. Traditional concrete mix design is slow and expensive, relying on trial-and-error. Meta's AI-driven approach seeks to accelerate the adoption of U.S.-made materials, supporting reshoring efforts that boost American jobs and economic value.

BOxCrete, an improved model, uses Bayesian optimization to intelligently design concrete mixes. It learns from existing data, proposes high-potential formulations, incorporates user-defined constraints, and refines predictions with each test, significantly speeding up the discovery process.

This initiative has shown real-world impact through partnerships. Meta, with Amrize (North America's largest cement manufacturer) and the University of Illinois at Urbana-Champaign, is implementing AI for sustainable, domestically-produced concrete. In Rosemount, MN, an AI-optimized mix for a Meta data center achieved 43% faster structural strength and 10% reduced cracking using U.S.-sourced materials. Additionally, Pennsylvania-based Quadrel, an enterprise SaaS platform, has integrated Meta’s open-source AI framework into its software for daily mix design and quality control.

Meta's goal is to foster an industry-wide shift, making AI-optimized mix design broadly accessible to producers without changing existing workflows, ultimately reducing barriers to domestic material adoption, boosting supply chain resilience, and improving sustainability.

---

## 9. My son pleasured himself on Gemini Live. Entire family's Google accounts banned

**原文标题**: My son pleasured himself on Gemini Live. Entire family's Google accounts banned

**原文链接**: [https://old.reddit.com/r/LegalAdviceUK/comments/1s92fql/my_son_pleasured_himself_in_front_of_gemini_live/](https://old.reddit.com/r/LegalAdviceUK/comments/1s92fql/my_son_pleasured_himself_in_front_of_gemini_live/)

生成摘要时出错

---

## 10. The Claude Code Leak

**原文标题**: The Claude Code Leak

**原文链接**: [https://build.ms/2026/4/1/the-claude-code-leak/](https://build.ms/2026/4/1/the-claude-code-leak/)

The article analyzes the implications of a hypothetical "Claude Code Leak," offering five key observations beyond the leak itself.

Firstly, the author notes that despite being perceived as "garbage" code, Claude Code achieved significant success, demonstrating that strong product-market fit can trump code quality, even for developer-centric tools. This challenges the traditional belief that immaculate code is essential for valuable software.

Secondly, the piece argues that the "what" the code does matters more than "how" it's written. Anthropic prioritizes robust observability and self-healing systems to ensure functionality, enabling rapid development without perfect underlying code.

Thirdly, product-market fit remains paramount; users prioritize effective problem-solving. If Claude Code faltered, competitors like OpenAI or Google are poised to meet the existing demand for coding products.

Fourthly, the copyright response was telling. Anthropic's swift DMCA notices for leaked code forks, juxtaposed with the AI industry's stance that AI-rewritten content isn't derivative, highlights a double standard and potentially furthers the notion that "code should be free" in a libertarian sense.

Finally, the leak is ultimately deemed inconsequential. The true value of AI ecosystems lies in the seamless integration of models and their "harness" (the complete service), not the underlying source code. Users pay for great results and a cohesive experience, as evidenced by successful integrated services maintaining mindshare over open-source alternatives. The author concludes that code's intrinsic value is often overestimated; effective problem-solving and seamless integration are what truly matter to users.

---

## 11. Bringing Clojure programming to Enterprise (2021)

**原文标题**: Bringing Clojure programming to Enterprise (2021)

**原文链接**: [https://blogit.michelin.io/clojure-programming/](https://blogit.michelin.io/clojure-programming/)

生成摘要时出错

---

## 12. Artemis computer running two instances of MS outlook; they can't figure out why

**原文标题**: Artemis computer running two instances of MS outlook; they can't figure out why

**原文链接**: [https://bsky.app/profile/nikigrayson.com/post/3miik2wzosk25](https://bsky.app/profile/nikigrayson.com/post/3miik2wzosk25)

生成摘要时出错

---

## 13. r/programming bans all discussion of LLM programming

**原文标题**: r/programming bans all discussion of LLM programming

**原文链接**: [https://old.reddit.com/r/programming/comments/1s9jkzi/announcement_temporary_llm_content_ban/](https://old.reddit.com/r/programming/comments/1s9jkzi/announcement_temporary_llm_content_ban/)

生成摘要时出错

---

## 14. StepFun 3.5 Flash is #1 cost-effective model for OpenClaw tasks (300 battles)

**原文标题**: StepFun 3.5 Flash is #1 cost-effective model for OpenClaw tasks (300 battles)

**原文链接**: [https://app.uniclaw.ai/arena?tab=costEffectiveness&via=hn](https://app.uniclaw.ai/arena?tab=costEffectiveness&via=hn)

生成摘要时出错

---

## 15. Ukrainian drone holds position for 6 weeks

**原文标题**: Ukrainian drone holds position for 6 weeks

**原文链接**: [https://defenceleaders.com/news/ukrainian-combat-robot-holds-frontline-position-for-six-weeks-in-sign-of-growing-ugv-maturity/](https://defenceleaders.com/news/ukrainian-combat-robot-holds-frontline-position-for-six-weeks-in-sign-of-growing-ugv-maturity/)

生成摘要时出错

---

## 16. Renewables reached nearly 50% of global electricity capacity last year

**原文标题**: Renewables reached nearly 50% of global electricity capacity last year

**原文链接**: [https://www.theregister.com/2026/04/01/renewables_generated_nearly_half_global_power/](https://www.theregister.com/2026/04/01/renewables_generated_nearly_half_global_power/)

生成摘要时出错

---

## 17. I traced my traffic through a home Tailscale exit node

**原文标题**: I traced my traffic through a home Tailscale exit node

**原文链接**: [https://tech.stonecharioteer.com/posts/2026/tailscale-exit-nodes/](https://tech.stonecharioteer.com/posts/2026/tailscale-exit-nodes/)

生成摘要时出错

---

## 18. New laws to make it easier to cancel subscriptions and get refunds

**原文标题**: New laws to make it easier to cancel subscriptions and get refunds

**原文链接**: [https://www.bbc.co.uk/news/articles/cvg0v36ek2go](https://www.bbc.co.uk/news/articles/cvg0v36ek2go)

生成摘要时出错

---

## 19. Ordinary Lab Gloves May Have Skewed Microplastic Data

**原文标题**: Ordinary Lab Gloves May Have Skewed Microplastic Data

**原文链接**: [https://nautil.us/ordinary-lab-gloves-may-have-skewed-microplastic-data-1279386](https://nautil.us/ordinary-lab-gloves-may-have-skewed-microplastic-data-1279386)

生成摘要时出错

---

## 20. OpenAI demand sinks on secondary market as Anthropic runs hot

**原文标题**: OpenAI demand sinks on secondary market as Anthropic runs hot

**原文链接**: [https://www.bloomberg.com/news/articles/2026-04-01/openai-demand-sinks-on-secondary-market-as-anthropic-runs-hot](https://www.bloomberg.com/news/articles/2026-04-01/openai-demand-sinks-on-secondary-market-as-anthropic-runs-hot)

生成摘要时出错

---

## 21. Show HN: Dull – Instagram Without Reels, YouTube Without Shorts (iOS)

**原文标题**: Show HN: Dull – Instagram Without Reels, YouTube Without Shorts (iOS)

**原文链接**: [https://getdull.app](https://getdull.app)

生成摘要时出错

---

## 22. 'Backrooms' and the Rise of the Institutional Gothic

**原文标题**: 'Backrooms' and the Rise of the Institutional Gothic

**原文链接**: [https://thereader.mitpress.mit.edu/backrooms-and-the-rise-of-the-institutional-gothic/](https://thereader.mitpress.mit.edu/backrooms-and-the-rise-of-the-institutional-gothic/)

生成摘要时出错

---

## 23. Mercor says it was hit by cyberattack tied to compromise LiteLLM

**原文标题**: Mercor says it was hit by cyberattack tied to compromise LiteLLM

**原文链接**: [https://techcrunch.com/2026/03/31/mercor-says-it-was-hit-by-cyberattack-tied-to-compromise-of-open-source-litellm-project/](https://techcrunch.com/2026/03/31/mercor-says-it-was-hit-by-cyberattack-tied-to-compromise-of-open-source-litellm-project/)

生成摘要时出错

---

## 24. Random numbers, Persian code: A mysterious signal transfixes radio sleuths

**原文标题**: Random numbers, Persian code: A mysterious signal transfixes radio sleuths

**原文链接**: [https://www.rferl.org/a/mystery-numbers-station-persian-signal-iran-war/33700659.html](https://www.rferl.org/a/mystery-numbers-station-persian-signal-iran-war/33700659.html)

生成摘要时出错

---

## 25. Apple at 50

**原文标题**: Apple at 50

**原文链接**: [https://www.apple.com/](https://www.apple.com/)

生成摘要时出错

---

## 26. New patches allow building Linux IPv6-only

**原文标题**: New patches allow building Linux IPv6-only

**原文链接**: [https://www.phoronix.com/news/Linux-IPv6-IPv4-Legacy-Knobs](https://www.phoronix.com/news/Linux-IPv6-IPv4-Legacy-Knobs)

生成摘要时出错

---

## 27. Modern SQLite: Features You Didn't Know It Had

**原文标题**: Modern SQLite: Features You Didn't Know It Had

**原文链接**: [https://slicker.me/sqlite/features.htm](https://slicker.me/sqlite/features.htm)

生成摘要时出错

---

## 28. Signing data structures the wrong way

**原文标题**: Signing data structures the wrong way

**原文链接**: [https://blog.foks.pub/posts/domain-separation-in-idl/](https://blog.foks.pub/posts/domain-separation-in-idl/)

生成摘要时出错

---

## 29. Swappa.com for GrapheneOS compatible devices – Stay Away

**原文标题**: Swappa.com for GrapheneOS compatible devices – Stay Away

**原文链接**: [https://discuss.grapheneos.org/d/33727-swappacom-for-grapheneos-compatible-devices-stay-away](https://discuss.grapheneos.org/d/33727-swappacom-for-grapheneos-compatible-devices-stay-away)

生成摘要时出错

---

## 30. Tailscale's New macOS Home

**原文标题**: Tailscale's New macOS Home

**原文链接**: [https://tailscale.com/blog/macos-notch-escape](https://tailscale.com/blog/macos-notch-escape)

生成摘要时出错

---

## 31. The Document Foundation ejects its core developers

**原文标题**: The Document Foundation ejects its core developers

**原文链接**: [https://www.collaboraonline.com/blog/tdf-ejects-its-core-developers/](https://www.collaboraonline.com/blog/tdf-ejects-its-core-developers/)

生成摘要时出错

---

## 32. The AI Marketing BS Index

**原文标题**: The AI Marketing BS Index

**原文链接**: [https://bastian.rieck.me/blog/2026/bs/](https://bastian.rieck.me/blog/2026/bs/)

生成摘要时出错

---

## 33. A new way to measure poverty shows the US falling behind Europe

**原文标题**: A new way to measure poverty shows the US falling behind Europe

**原文链接**: [https://www.euronews.com/business/2026/03/29/a-new-way-to-measure-poverty-shows-the-us-falling-behind-europe](https://www.euronews.com/business/2026/03/29/a-new-way-to-measure-poverty-shows-the-us-falling-behind-europe)

生成摘要时出错

---

## 34. The Anti-Intellectualism of Silicon Valley Elites

**原文标题**: The Anti-Intellectualism of Silicon Valley Elites

**原文链接**: [https://www.elizabethspiers.com/the-anti-intellectualism-of-silicon-valley-elites/](https://www.elizabethspiers.com/the-anti-intellectualism-of-silicon-valley-elites/)

生成摘要时出错

---

## 35. Show HN: Sycamore – next gen Rust web UI library using fine-grained reactivity

**原文标题**: Show HN: Sycamore – next gen Rust web UI library using fine-grained reactivity

**原文链接**: [https://sycamore.dev](https://sycamore.dev)

生成摘要时出错

---

## 36. The SpaceX IPO: retail investor notes

**原文标题**: The SpaceX IPO: retail investor notes

**原文链接**: [https://report.bearblog.dev/the-spacex-ipo-will-be-the-perfect-storm-of-retail-investor-fallacies/](https://report.bearblog.dev/the-spacex-ipo-will-be-the-perfect-storm-of-retail-investor-fallacies/)

生成摘要时出错

---

## 37. What Is Copilot Exactly?

**原文标题**: What Is Copilot Exactly?

**原文链接**: [https://idiallo.com/blog/what-is-copilot-exactly](https://idiallo.com/blog/what-is-copilot-exactly)

生成摘要时出错

---

## 38. A forecast of the fair market value of SpaceX's businesses

**原文标题**: A forecast of the fair market value of SpaceX's businesses

**原文链接**: [https://futuresearch.ai/spacex-ipo-valuation/](https://futuresearch.ai/spacex-ipo-valuation/)

生成摘要时出错

---

## 39. Show HN: NASA Artemis II Mission Timeline Tracker

**原文标题**: Show HN: NASA Artemis II Mission Timeline Tracker

**原文链接**: [https://www.sunnywingsvirtual.com/artemis2/timeline.html](https://www.sunnywingsvirtual.com/artemis2/timeline.html)

生成摘要时出错

---

## 40. March heat in American west has left snowpack at record-low levels

**原文标题**: March heat in American west has left snowpack at record-low levels

**原文链接**: [https://www.theguardian.com/us-news/2026/apr/01/snowmelt-american-west](https://www.theguardian.com/us-news/2026/apr/01/snowmelt-american-west)

生成摘要时出错

---

## 41. Solar Balconies Take Europe by Storm

**原文标题**: Solar Balconies Take Europe by Storm

**原文链接**: [https://hackaday.com/2026/03/31/solar-balconies-take-europe-by-storm/](https://hackaday.com/2026/03/31/solar-balconies-take-europe-by-storm/)

生成摘要时出错

---

## 42. Jax's true calling: Ray-Marching renderers on WebGL

**原文标题**: Jax's true calling: Ray-Marching renderers on WebGL

**原文链接**: [https://benoit.paris/posts/jax-ray-marcher/](https://benoit.paris/posts/jax-ray-marcher/)

生成摘要时出错

---

## 43. Iran war sparks renewables boom as Europeans rush to buy solar, heat pumps, EVs

**原文标题**: Iran war sparks renewables boom as Europeans rush to buy solar, heat pumps, EVs

**原文链接**: [https://www.euronews.com/2026/03/31/iran-war-sparks-renewables-boom-as-europeans-rush-to-buy-solar-heat-pumps-and-evs](https://www.euronews.com/2026/03/31/iran-war-sparks-renewables-boom-as-europeans-rush-to-buy-solar-heat-pumps-and-evs)

生成摘要时出错

---

## 44. Cursor 3

**原文标题**: Cursor 3

**原文链接**: [https://cursor.com/blog/cursor-3](https://cursor.com/blog/cursor-3)

生成摘要时出错

---

## 45. Scientists crack a 20-year nuclear mystery behind the creation of gold

**原文标题**: Scientists crack a 20-year nuclear mystery behind the creation of gold

**原文链接**: [https://www.sciencedaily.com/releases/2026/03/260313002633.htm](https://www.sciencedaily.com/releases/2026/03/260313002633.htm)

生成摘要时出错

---

## 46. Show HN: Flight-Viz – 10K flights on a 3D globe in 3.5MB of Rust+WASM

**原文标题**: Show HN: Flight-Viz – 10K flights on a 3D globe in 3.5MB of Rust+WASM

**原文链接**: [https://flight-viz.com](https://flight-viz.com)

生成摘要时出错

---

## 47. Marc Andreessen's dangerously unexamined life

**原文标题**: Marc Andreessen's dangerously unexamined life

**原文链接**: [https://www.thenation.com/article/society/marc-andreessen-silicon-valley-military-tech/](https://www.thenation.com/article/society/marc-andreessen-silicon-valley-military-tech/)

生成摘要时出错

---

## 48. TurboQuant KV Compression and SSD Expert Streaming for M5 Pro and IOS

**原文标题**: TurboQuant KV Compression and SSD Expert Streaming for M5 Pro and IOS

**原文链接**: [https://github.com/SharpAI/SwiftLM](https://github.com/SharpAI/SwiftLM)

生成摘要时出错

---

## 49. We Built It with Slide Rules. Then We Forgot How

**原文标题**: We Built It with Slide Rules. Then We Forgot How

**原文链接**: [https://unmitigatedrisk.com/?p=1227](https://unmitigatedrisk.com/?p=1227)

生成摘要时出错

---

## 50. SpaceX confidentially files to go public at $1.75T, reports say

**原文标题**: SpaceX confidentially files to go public at $1.75T, reports say

**原文链接**: [https://www.theguardian.com/technology/2026/apr/01/spacex-public-offering-stock-market](https://www.theguardian.com/technology/2026/apr/01/spacex-public-offering-stock-market)

生成摘要时出错

---

## 51. IPv6 address, as a sentence you can remember

**原文标题**: IPv6 address, as a sentence you can remember

**原文链接**: [https://sentence2ipv6.tib3rius.com/](https://sentence2ipv6.tib3rius.com/)

生成摘要时出错

---

## 52. Show HN: Real-time dashboard for Claude Code agent teams

**原文标题**: Show HN: Real-time dashboard for Claude Code agent teams

**原文链接**: [https://github.com/simple10/agents-observe](https://github.com/simple10/agents-observe)

生成摘要时出错

---

## 53. ZomboCom stolen by a hacker, sold, now replaced with AI-generated makeover

**原文标题**: ZomboCom stolen by a hacker, sold, now replaced with AI-generated makeover

**原文链接**: [https://old.reddit.com/r/oldinternet/comments/1raiz8v/zombocom_was_stolen_by_hacker_put_up_for_sale_and/](https://old.reddit.com/r/oldinternet/comments/1raiz8v/zombocom_was_stolen_by_hacker_put_up_for_sale_and/)

生成摘要时出错

---

## 54. Show HN: I built a DNS resolver from scratch in Rust – no DNS libraries

**原文标题**: Show HN: I built a DNS resolver from scratch in Rust – no DNS libraries

**原文链接**: [https://github.com/razvandimescu/numa](https://github.com/razvandimescu/numa)

生成摘要时出错

---

## 55. Pam Bondi ousted as Attorney General

**原文标题**: Pam Bondi ousted as Attorney General

**原文链接**: [https://www.cnn.com/2026/04/02/politics/pam-bondi-role-trump](https://www.cnn.com/2026/04/02/politics/pam-bondi-role-trump)

生成摘要时出错

---

## 56. The Windows equivalents of the most used Linux commands

**原文标题**: The Windows equivalents of the most used Linux commands

**原文链接**: [http://techkettle.blogspot.com/2026/04/the-windows-equivalents-of-most-used.html](http://techkettle.blogspot.com/2026/04/the-windows-equivalents-of-most-used.html)

生成摘要时出错

---

## 57. ReactOS Shows Improved Stability and 64-Bit Support at Chemnitz Linux Days 2026

**原文标题**: ReactOS Shows Improved Stability and 64-Bit Support at Chemnitz Linux Days 2026

**原文链接**: [https://old.reddit.com/r/reactos/comments/1sa26yu/back_from_chemnitz_linux_days_2026/](https://old.reddit.com/r/reactos/comments/1sa26yu/back_from_chemnitz_linux_days_2026/)

生成摘要时出错

---

## 58. Enabling Codex to Analyze Two Decades of Hacker News Data

**原文标题**: Enabling Codex to Analyze Two Decades of Hacker News Data

**原文链接**: [https://modolap.com/publication/hn-analysis-1](https://modolap.com/publication/hn-analysis-1)

生成摘要时出错

---

## 59. OnlyOffice kills Nextcloud partnership for forking its project without approval

**原文标题**: OnlyOffice kills Nextcloud partnership for forking its project without approval

**原文链接**: [https://www.neowin.net/news/onlyoffice-suspends-nextcloud-partnership-over-unapproved-euro-office-fork/](https://www.neowin.net/news/onlyoffice-suspends-nextcloud-partnership-over-unapproved-euro-office-fork/)

生成摘要时出错

---

## 60. Show HN: Baton – A desktop app for developing with AI agents

**原文标题**: Show HN: Baton – A desktop app for developing with AI agents

**原文链接**: [https://getbaton.dev/](https://getbaton.dev/)

生成摘要时出错

---

## 61. Montana referendum to outlaw corporate campaign contributions [video]

**原文标题**: Montana referendum to outlaw corporate campaign contributions [video]

**原文链接**: [https://www.youtube.com/watch?v=p1fPbGHe3xE](https://www.youtube.com/watch?v=p1fPbGHe3xE)

生成摘要时出错

---

## 62. Apple removes iPhone vibe coding app from app store

**原文标题**: Apple removes iPhone vibe coding app from app store

**原文链接**: [https://gizmodo.com/apple-removes-iphone-vibe-coding-app-from-app-store-2000740084](https://gizmodo.com/apple-removes-iphone-vibe-coding-app-from-app-store-2000740084)

生成摘要时出错

---

## 63. The future of code search is not regex – 100x faster than ripgrep

**原文标题**: The future of code search is not regex – 100x faster than ripgrep

**原文链接**: [https://fff.dmtrkovalenko.dev/](https://fff.dmtrkovalenko.dev/)

生成摘要时出错

---

## 64. OpenAI Acquires TBPN

**原文标题**: OpenAI Acquires TBPN

**原文链接**: [https://openai.com/index/openai-acquires-tbpn/](https://openai.com/index/openai-acquires-tbpn/)

生成摘要时出错

---

## 65. AI has suddenly become more useful to open-source developers

**原文标题**: AI has suddenly become more useful to open-source developers

**原文链接**: [https://www.zdnet.com/article/maybe-open-source-needs-ai/](https://www.zdnet.com/article/maybe-open-source-needs-ai/)

生成摘要时出错

---

## 66. Trinity Large Thinking

**原文标题**: Trinity Large Thinking

**原文链接**: [https://openrouter.ai/arcee-ai/trinity-large-thinking](https://openrouter.ai/arcee-ai/trinity-large-thinking)

生成摘要时出错

---

## 67. A million new SpaceX satellites will destroy the night sky

**原文标题**: A million new SpaceX satellites will destroy the night sky

**原文链接**: [https://theconversation.com/a-million-new-spacex-satellites-will-destroy-the-night-sky-for-everyone-on-earth-277938](https://theconversation.com/a-million-new-spacex-satellites-will-destroy-the-night-sky-for-everyone-on-earth-277938)

生成摘要时出错

---

## 68. Solar panels at Lidl? Plug-in versions set to appear in shops

**原文标题**: Solar panels at Lidl? Plug-in versions set to appear in shops

**原文链接**: [https://www.thisismoney.co.uk/money/bills/article-15673955/Solar-panels-Lidl-Plug-versions-set-appear-shops-MONTHS.html](https://www.thisismoney.co.uk/money/bills/article-15673955/Solar-panels-Lidl-Plug-versions-set-appear-shops-MONTHS.html)

生成摘要时出错

---

## 69. Show HN: Claude Code rewritten as a bash script

**原文标题**: Show HN: Claude Code rewritten as a bash script

**原文链接**: [https://github.com/jdcodes1/claude-sh](https://github.com/jdcodes1/claude-sh)

生成摘要时出错

---

## 70. Even GPT-5.2 Can't Count to Five: Zero-Error Horizons in Trustworthy LLMs

**原文标题**: Even GPT-5.2 Can't Count to Five: Zero-Error Horizons in Trustworthy LLMs

**原文链接**: [https://arxiv.org/abs/2601.15714](https://arxiv.org/abs/2601.15714)

生成摘要时出错

---

## 71. EmDash: A Fresh Take on CMS

**原文标题**: EmDash: A Fresh Take on CMS

**原文链接**: [https://maciekpalmowski.dev/blog/emdash-a-fresh-take-on-cms/](https://maciekpalmowski.dev/blog/emdash-a-fresh-take-on-cms/)

生成摘要时出错

---

## 72. The German state (Schleswig-Holstein) trying to break free from Microsoft

**原文标题**: The German state (Schleswig-Holstein) trying to break free from Microsoft

**原文链接**: [https://www.ft.com/content/95bd87c8-a112-49a5-9b80-c280a6bb4283](https://www.ft.com/content/95bd87c8-a112-49a5-9b80-c280a6bb4283)

生成摘要时出错

---

## 73. A.I. Helped One Man (and His Brother) Build a $1.8B Company

**原文标题**: A.I. Helped One Man (and His Brother) Build a $1.8B Company

**原文链接**: [https://www.nytimes.com/2026/04/02/technology/ai-billion-dollar-company-medvi.html](https://www.nytimes.com/2026/04/02/technology/ai-billion-dollar-company-medvi.html)

生成摘要时出错

---

## 74. Age verification now required for DNS resolution

**原文标题**: Age verification now required for DNS resolution

**原文链接**: [https://easydns.com/blog/2026/04/01/age-verification-now-required-for-dns-resolution/](https://easydns.com/blog/2026/04/01/age-verification-now-required-for-dns-resolution/)

生成摘要时出错

---

## 75. CEO of largest public hospital says he's ready to replace radiologists with AI

**原文标题**: CEO of largest public hospital says he's ready to replace radiologists with AI

**原文链接**: [https://radiologybusiness.com/topics/artificial-intelligence/ceo-americas-largest-public-hospital-system-says-hes-ready-replace-radiologists-ai](https://radiologybusiness.com/topics/artificial-intelligence/ceo-americas-largest-public-hospital-system-says-hes-ready-replace-radiologists-ai)

生成摘要时出错

---

## 76. George Goble died recently – known for first dual-CPU-Unix and fast BBQ lighting

**原文标题**: George Goble died recently – known for first dual-CPU-Unix and fast BBQ lighting

**原文链接**: [https://www.legacy.com/us/obituaries/wlfi/name/george-goble-obituary?id=61144779](https://www.legacy.com/us/obituaries/wlfi/name/george-goble-obituary?id=61144779)

生成摘要时出错

---

## 77. Men are ditching TV for YouTube as AI usage and social media fatigue grow

**原文标题**: Men are ditching TV for YouTube as AI usage and social media fatigue grow

**原文链接**: [https://www.ofcom.org.uk/media-use-and-attitudes/media-habits-adults/passive-social-media-use-ai-companionship-and-online-side-hustles-uk-adults-media-and-online-lives-revealed](https://www.ofcom.org.uk/media-use-and-attitudes/media-habits-adults/passive-social-media-use-ai-companionship-and-online-side-hustles-uk-adults-media-and-online-lives-revealed)

生成摘要时出错

---

## 78. Head of FEMA defends claim that he was teleported

**原文标题**: Head of FEMA defends claim that he was teleported

**原文链接**: [https://www.cnn.com/2026/04/01/politics/fema-official-gregg-phillips-defends-teleportation-claim](https://www.cnn.com/2026/04/01/politics/fema-official-gregg-phillips-defends-teleportation-claim)

生成摘要时出错

---

## 79. Mad Bugs: Vim vs. Emacs vs. Claude

**原文标题**: Mad Bugs: Vim vs. Emacs vs. Claude

**原文链接**: [https://blog.calif.io/p/mad-bugs-vim-vs-emacs-vs-claude](https://blog.calif.io/p/mad-bugs-vim-vs-emacs-vs-claude)

生成摘要时出错

---

## 80. I built a 516-panel financial terminal in 3 weeks using AI

**原文标题**: I built a 516-panel financial terminal in 3 weeks using AI

**原文链接**: [https://neuberg.ai/](https://neuberg.ai/)

生成摘要时出错

---

## 81. Jami – free/libre, end-to-end encrypted, and private communication software

**原文标题**: Jami – free/libre, end-to-end encrypted, and private communication software

**原文链接**: [https://jami.net/](https://jami.net/)

生成摘要时出错

---

## 82. xkcd: Creation

**原文标题**: xkcd: Creation

**原文链接**: [https://xkcd.com/3227/](https://xkcd.com/3227/)

生成摘要时出错

---

## 83. Dutch armed forces recruiting 1,200 drone specialists

**原文标题**: Dutch armed forces recruiting 1,200 drone specialists

**原文链接**: [https://nltimes.nl/2026/04/01/dutch-armed-forces-recruiting-1200-drone-specialists-first-reported-duty-today](https://nltimes.nl/2026/04/01/dutch-armed-forces-recruiting-1200-drone-specialists-first-reported-duty-today)

生成摘要时出错

---

## 84. Iran threatens Nvidia, Apple and other 18 tech companies

**原文标题**: Iran threatens Nvidia, Apple and other 18 tech companies

**原文链接**: [https://www.cnbc.com/2026/04/01/iran-irgc-nvidia-appple-attack-threat.html](https://www.cnbc.com/2026/04/01/iran-irgc-nvidia-appple-attack-threat.html)

生成摘要时出错

---

## 85. Almighty Lisp: Lisp and Emacs Essentials Book

**原文标题**: Almighty Lisp: Lisp and Emacs Essentials Book

**原文链接**: [https://almightylisp.com/](https://almightylisp.com/)

生成摘要时出错

---

## 86. Analyzing Geekbench 6 under Intel's BOT

**原文标题**: Analyzing Geekbench 6 under Intel's BOT

**原文链接**: [https://www.geekbench.com/blog/2026/03/analyzing-geekbench-6-under-intels-bot/](https://www.geekbench.com/blog/2026/03/analyzing-geekbench-6-under-intels-bot/)

生成摘要时出错

---

## 87. DDR5 RAM prices fall by as much as 30%, but memory shortage likely far from over

**原文标题**: DDR5 RAM prices fall by as much as 30%, but memory shortage likely far from over

**原文链接**: [https://www.notebookcheck.net/DDR5-RAM-prices-fall-by-as-much-as-30-but-memory-shortage-likely-far-from-over.1263431.0.html](https://www.notebookcheck.net/DDR5-RAM-prices-fall-by-as-much-as-30-but-memory-shortage-likely-far-from-over.1263431.0.html)

生成摘要时出错

---

