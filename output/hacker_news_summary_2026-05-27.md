# Hacker News 热门文章摘要 (2026-05-27)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 我厌倦了和AI说话。

**原文标题**: I'm Tired of Talking to AI

**原文链接**: [https://orchidfiles.com/im-tired-of-ai-generated-answers/](https://orchidfiles.com/im-tired-of-ai-generated-answers/)

作者对与AI互动深感厌倦，尤其是在寻求真人输入时。他讲述了几个令人沮丧的经历来佐证这一点。

有一次，在发现传播恶意软件的GitHub仓库后，作者向AI查询却得到了无用的建议。当他随后在GitHub上发起讨论时，两个不同的人回复了*完全相同*的、AI生成且毫无帮助的文本，这表明他们缺乏原创思想。

类似地，在职场环境中，作为一名开发者的作者向一位企业主询问一项任务。该企业主回复了一个ChatGPT的截图，作者认为这既不相关也不正确。一分钟后，这位企业主又发送了*另一个*ChatGPT截图，显然没有阅读其内容。

作者还描述了最近在Reddit上的一次互动，经过几次交流后，他才意识到自己正在与一个AI代理对话。

这些经历让作者得出结论，他已经厌倦了与AI对话，渴望真正的真人互动。然而，即使在与人交流时，他也经常发现自己的问题被转交给了AI，而AI未经审查的答案随后又被转发回给他。

---

## 2. 用AI更缓慢地编写更好的代码

**原文标题**: Using AI to write better code more slowly

**原文链接**: [https://nolanlawson.com/2026/05/25/using-ai-to-write-better-code-more-slowly/](https://nolanlawson.com/2026/05/25/using-ai-to-write-better-code-more-slowly/)

Nolan Lawson argues against the common perception that AI coding tools are solely for generating low-quality code quickly. He posits that LLMs are highly effective for writing *high-quality code more slowly*, emphasizing their capability to identify numerous bugs.

Lawson details his workflow, which involves a custom "Claude skill" orchestrating multiple AI agents (like Claude, Codex, and Cursor Bugbot) to meticulously review Pull Requests (PRs). This multi-agent approach significantly reduces false positives, uncovering a wide range of bugs from critical security issues to minor code inconsistencies.

His process includes using agents to fix critical and high-priority bugs, selectively addressing others, and sometimes abandoning fundamentally flawed PRs. While this method doesn't necessarily accelerate development—often leading to "side-quests" to fix pre-existing issues—it profoundly improves codebase health and deepens the developer's understanding of complex systems.

Lawson advocates for this methodical, quality-obsessed approach, which he finds more satisfying and beneficial for long-term codebase maintainability. He encourages developers to embrace this slower, deliberate use of AI to write better code, even if it means sacrificing immediate "productivity" in terms of raw output.

---

## 3. 西班牙因缺乏赌博执照禁止Polymarket、Kalshi预测市场

**原文标题**: Spain blocks prediction markets Polymarket, Kalshi over lack of gambling licence

**原文链接**: [https://www.reuters.com/business/spain-blocks-prediction-markets-polymarket-kalshi-over-lack-gambling-licences-2026-05-26/](https://www.reuters.com/business/spain-blocks-prediction-markets-polymarket-kalshi-over-lack-gambling-licences-2026-05-26/)

生成摘要时出错

---

## 4. GitHub Actions 宕机了

**原文标题**: GitHub Actions was down

**原文链接**: [https://www.githubstatus.com/?today](https://www.githubstatus.com/?today)

GitHub Actions在2026年5月经历了多次性能下降和中断。

5月26日，Actions和Pages发生了一起事件，大约从10:57 UTC持续到13:18 UTC。这由认证问题引起，导致Actions运行的启动和下载失败，影响了大多数工作流。尽管某些相关内容，如Issues和PRs，被暂时隐藏，但没有数据丢失，问题通过缓解措施得以解决。

5月20日发生的另一起重大事件，导致GitHub Actions客户在16:00 UTC至17:45 UTC之间经历了运行启动延迟超过5分钟。大约4.5%的所有运行被延迟，其中规模化作业受影响尤为严重（30%延迟，4%失败）。根本原因是内部服务上的健康检查配置错误，导致区域集群发生连锁故障。通过扩容和重新平衡流量解决了问题。

早些时候，5月15日，Actions面临可用性下降，大约从07:43 UTC到08:48 UTC，导致工作流运行失败或延迟。在高峰期，42%的Actions运行失败。这归因于在计划的基础设施故障转移期间，自动化服务发现更新未能正确传播，影响了Pages和Copilot服务。人工干预纠正了路由问题，恢复了稳定性。

GitHub正在实施纠正措施，包括加强健康检查配置和提高依赖项弹性，以防止未来再次发生此类事件。

---

## 5. 我最糟糕的面试

**原文标题**: The worst job interview I ever had

**原文链接**: [https://www.oliverio.dev/blog/the-worst-job-interview-i-had](https://www.oliverio.dev/blog/the-worst-job-interview-i-had)

作者，一名工程师，讲述了他最糟糕的一次面试经历：为了一个心理健康初创公司的创始工程师职位，他接受了一次“未经请求的心理评估”。虽然他理解初创公司中文化契合度的重要性，但他认为这种特定的面试方式存在严重问题。

在一次初步的信息交流面试之后，他被安排参加一次90分钟的“非传统”文化契合度对话。这次对话包含“诱导创伤”的问题，涉及他最艰难的一天、最大的生活挑战、失败的人际关系和家庭困境。尽管他觉得这些问题具有侵犯性，他还是分享了个人细节，相信这是一个“安全空间”，而面试官却鲜有透露。作者在通话结束后感到心力交瘁，期间完全没有讨论任何技术技能。

二十四小时后，他收到了一封简短的拒信。这迅速将他的心力交瘁转变为羞耻和愤怒。他感到非常糟糕，因为分享了如此私密的个人信息，结果却因为“他这个人”而不是他的技术能力而被拒绝。令他尤为不解的是，一家心理健康初创公司竟会采用这种让应聘者感到如此脆弱的面试方式。作者最后呼吁招聘经理在评估文化契合度时，不应强迫应聘者为了获得一份工作而披露他们最深的创伤。

---

## 6. 研究发现：散步比久坐更能激发创造力 (2014)

**原文标题**: Taking a walk may lead to more creativity than sitting, study finds (2014)

**原文链接**: [https://www.apa.org/news/press/releases/2014/04/creativity-walk](https://www.apa.org/news/press/releases/2014/04/creativity-walk)

A 2014 study by Marily Oppezzo (Santa Clara University) and Daniel L. Schwartz (Stanford University) revealed that walking significantly enhances creative thinking compared to sitting. Published in the Journal of Experimental Psychology: Learning, Memory and Cognition, the research involved 176 college students.

Participants performed tasks such as generating alternative uses for common objects and creating original analogies. Across multiple experiments, those who walked—whether on a treadmill indoors or outdoors—consistently produced a higher number of creative and novel responses than those who remained seated or were pushed in a wheelchair. In one experiment, 100% of walkers generated more creative ideas.

Conversely, for tasks requiring focused concentration or a single correct answer, walkers performed slightly less effectively than their seated counterparts. The study highlighted that the physical act of walking itself, rather than the outdoor environment, was the primary factor in boosting creativity. Notably, even walking *before* a task showed a residual positive effect on creativity when participants subsequently sat down.

This research suggests that incorporating simple walks can be an "easy and productive" method to foster free-flowing thought and innovation, benefiting both cognitive function and work-related activities. Further studies are recommended to fully elucidate the complex physiological and cognitive pathways involved.

---

## 7. 荷兰阻止美国收购关键数字供应商

**原文标题**: Netherlands blocks US takeover of vital digital supplier

**原文链接**: [https://www.politico.eu/article/netherlands-blocks-us-takeover-vital-digital-supplier/](https://www.politico.eu/article/netherlands-blocks-us-takeover-vital-digital-supplier/)

荷兰政府阻止了美国公司Kyndryl收购一家重要的荷兰数字供应商Solvinity。Solvinity运营着荷兰国家在线身份识别应用DigiD的平台，公民使用DigiD来验证身份，以获取预约医生或与公共机构互动等基本服务。

此次收购被叫停，原因是对一个重要的国家身份识别工具将落入外国控制之下表示担忧，这构成“对公共利益的潜在风险”。数字经济国务秘书Willemijn Aerdts在听取了国家投资审查机构的建议后宣布了这一决定。

尽管荷兰重视外国科技公司，但它维持着一个独立的投资审查框架，以保护公共利益，适用于所有投资者。此举与欧洲日益增长的对欧盟依赖美国技术的担忧相吻合，并且早于欧盟委员会即将出台的旨在减少在云计算、微芯片和人工智能等领域依赖的“技术主权一揽子计划”。

Kyndryl对此表示极度失望，声称这一过程被“政治化”，并掩盖了此次交易的益处。

---

## 8. Big tech's anti-labor playbook has come for Wikipedia

**原文标题**: Big tech's anti-labor playbook has come for Wikipedia

**原文链接**: [https://medium.com/@jakeorlowitz/wikipedia-is-doing-the-capitalist-thing-56a393232943](https://medium.com/@jakeorlowitz/wikipedia-is-doing-the-capitalist-thing-56a393232943)

生成摘要时出错

---

## 9. Last.fm is now independent

**原文标题**: Last.fm is now independent

**原文链接**: [https://support.last.fm/t/last-fm-is-now-independent/118591](https://support.last.fm/t/last-fm-is-now-independent/118591)

生成摘要时出错

---

## 10. Ferrari Luce

**原文标题**: Ferrari Luce

**原文链接**: [https://www.ferrari.com/en-EN/auto/ferrari-luce](https://www.ferrari.com/en-EN/auto/ferrari-luce)

生成摘要时出错

---

## 11. 在谷歌表示人们喜爱AI模式后，DuckDuckGo搜索的访问量增长了28%。

**原文标题**: DuckDuckGo search saw 28% more visits after Google said people love AI mode

**原文链接**: [https://www.pcgamer.com/hardware/duckduckgos-ai-free-search-saw-nearly-28-percent-more-visits-in-the-week-following-googles-insistence-that-people-love-ai-mode/](https://www.pcgamer.com/hardware/duckduckgos-ai-free-search-saw-nearly-28-percent-more-visits-in-the-week-following-googles-insistence-that-people-love-ai-mode/)

生成摘要时出错

---

## 12. Tech CEOs are apparently suffering from AI psychosis

**原文标题**: Tech CEOs are apparently suffering from AI psychosis

**原文链接**: [https://techcrunch.com/2026/05/27/tech-ceos-are-apparently-suffering-from-ai-psychosis/](https://techcrunch.com/2026/05/27/tech-ceos-are-apparently-suffering-from-ai-psychosis/)

生成摘要时出错

---

## 13. I think Anthropic and OpenAI have found product-market fit

**原文标题**: I think Anthropic and OpenAI have found product-market fit

**原文链接**: [https://simonwillison.net/2026/May/27/product-market-fit/](https://simonwillison.net/2026/May/27/product-market-fit/)

生成摘要时出错

---

## 14. Hacker News front page as a site

**原文标题**: Hacker News front page as a site

**原文链接**: [https://thefrontpage.dev/](https://thefrontpage.dev/)

生成摘要时出错

---

## 15. That Methyl Methacrylate Tank

**原文标题**: That Methyl Methacrylate Tank

**原文链接**: [https://www.science.org/content/blog-post/methyl-methacrylate-tank](https://www.science.org/content/blog-post/methyl-methacrylate-tank)

生成摘要时出错

---

## 16. The real cost of owning a home

**原文标题**: The real cost of owning a home

**原文链接**: [https://ericturner.dev/posts/cost-of-home-ownership/](https://ericturner.dev/posts/cost-of-home-ownership/)

生成摘要时出错

---

## 17. A few interesting modern pixel fonts

**原文标题**: A few interesting modern pixel fonts

**原文链接**: [https://unsung.aresluna.org/a-few-interesting-modern-pixel-fonts/](https://unsung.aresluna.org/a-few-interesting-modern-pixel-fonts/)

生成摘要时出错

---

## 18. Motorola phones have started hijacking the Amazon app to insert affiliate codes

**原文标题**: Motorola phones have started hijacking the Amazon app to insert affiliate codes

**原文链接**: [https://9to5google.com/2026/05/25/motorola-amazon-app-hijacking-behavior/](https://9to5google.com/2026/05/25/motorola-amazon-app-hijacking-behavior/)

生成摘要时出错

---

## 19. How Shamir's Secret Sharing Works

**原文标题**: How Shamir's Secret Sharing Works

**原文链接**: [https://ente.com/blog/how-shamirs-secret-sharing-works/](https://ente.com/blog/how-shamirs-secret-sharing-works/)

生成摘要时出错

---

## 20. Dropbox CEO Drew Houston to step down

**原文标题**: Dropbox CEO Drew Houston to step down

**原文链接**: [https://www.cnbc.com/2026/05/26/dropbox-ceo-drew-houston-ashraf-alkarmi.html](https://www.cnbc.com/2026/05/26/dropbox-ceo-drew-houston-ashraf-alkarmi.html)

生成摘要时出错

---

## 21. Private Equity Bought America's Essential Services

**原文标题**: Private Equity Bought America's Essential Services

**原文链接**: [https://rubbishtalk.com/economy/how-private-equity-bought-americas-essential-services/](https://rubbishtalk.com/economy/how-private-equity-bought-americas-essential-services/)

生成摘要时出错

---

## 22. Cloudflare Flagship

**原文标题**: Cloudflare Flagship

**原文链接**: [https://developers.cloudflare.com/flagship/](https://developers.cloudflare.com/flagship/)

生成摘要时出错

---

## 23. DynIP – Dynamic DNS with RFC 2136, IPv6, DNSSEC, and BYOD

**原文标题**: DynIP – Dynamic DNS with RFC 2136, IPv6, DNSSEC, and BYOD

**原文链接**: [https://dynip.dev/](https://dynip.dev/)

生成摘要时出错

---

## 24. All of human cooking compressed into 2 megabytes

**原文标题**: All of human cooking compressed into 2 megabytes

**原文链接**: [https://arxiv.org/abs/2605.22391](https://arxiv.org/abs/2605.22391)

生成摘要时出错

---

## 25. Claude Code as a Daily Driver: Claude.md, Skills, Subagents, Plugins, and MCPs

**原文标题**: Claude Code as a Daily Driver: Claude.md, Skills, Subagents, Plugins, and MCPs

**原文链接**: [https://arps18.github.io/posts/claude-code-mastery/](https://arps18.github.io/posts/claude-code-mastery/)

生成摘要时出错

---

## 26. Outsourcing plus local AI will soon become more economical vs. frontier labs

**原文标题**: Outsourcing plus local AI will soon become more economical vs. frontier labs

**原文链接**: [https://www.signalbloom.ai/posts/outsourcing-plus-localai-will-soon-become-more-economical-vs-frontier-labs/](https://www.signalbloom.ai/posts/outsourcing-plus-localai-will-soon-become-more-economical-vs-frontier-labs/)

生成摘要时出错

---

## 27. Stripe is friendly to “friendly fraud”

**原文标题**: Stripe is friendly to “friendly fraud”

**原文链接**: [https://www.gingerlime.com/2026/stripe-seem-friendly-to-friendly-fraud/](https://www.gingerlime.com/2026/stripe-seem-friendly-to-friendly-fraud/)

生成摘要时出错

---

## 28. Uber president says AI spending is getting 'harder to justify'

**原文标题**: Uber president says AI spending is getting 'harder to justify'

**原文链接**: [https://www.theverge.com/transportation/937116/uber-ai-investment-hard-to-justify](https://www.theverge.com/transportation/937116/uber-ai-investment-hard-to-justify)

生成摘要时出错

---

## 29. Nobody cracks open a programming book anymore

**原文标题**: Nobody cracks open a programming book anymore

**原文链接**: [https://unix.foo/posts/nobody-cracks-open-a-programming-book/](https://unix.foo/posts/nobody-cracks-open-a-programming-book/)

生成摘要时出错

---

## 30. The user is visibly frustrated

**原文标题**: The user is visibly frustrated

**原文链接**: [https://pscanf.com/s/354/](https://pscanf.com/s/354/)

生成摘要时出错

---

## 31. Uber, Lyft drivers in Massachusetts form first US ride-share union

**原文标题**: Uber, Lyft drivers in Massachusetts form first US ride-share union

**原文链接**: [https://www.reuters.com/business/world-at-work/uber-lyft-drivers-massachusetts-form-first-us-ride-share-union-2026-05-26/](https://www.reuters.com/business/world-at-work/uber-lyft-drivers-massachusetts-form-first-us-ride-share-union-2026-05-26/)

生成摘要时出错

---

## 32. Erin Brockovich made a map to track data centers around the country

**原文标题**: Erin Brockovich made a map to track data centers around the country

**原文链接**: [https://www.niemanlab.org/2026/05/erin-brockovich-made-a-map-to-track-data-centers-around-the-country/](https://www.niemanlab.org/2026/05/erin-brockovich-made-a-map-to-track-data-centers-around-the-country/)

生成摘要时出错

---

## 33. Microsoft Copilot Cowork Exfiltrates Files

**原文标题**: Microsoft Copilot Cowork Exfiltrates Files

**原文链接**: [https://www.promptarmor.com/resources/microsoft-copilot-cowork-exfiltrates-files](https://www.promptarmor.com/resources/microsoft-copilot-cowork-exfiltrates-files)

生成摘要时出错

---

## 34. The Melancholy of Slaying Monsters

**原文标题**: The Melancholy of Slaying Monsters

**原文链接**: [https://thereader.mitpress.mit.edu/the-strange-melancholy-of-slaying-monsters/](https://thereader.mitpress.mit.edu/the-strange-melancholy-of-slaying-monsters/)

生成摘要时出错

---

## 35. Does anybody like React?

**原文标题**: Does anybody like React?

**原文链接**: [https://jsx.lol](https://jsx.lol)

生成摘要时出错

---

## 36. Canada to order military plane fleet from Sweden in shift from US suppliers

**原文标题**: Canada to order military plane fleet from Sweden in shift from US suppliers

**原文链接**: [https://www.theguardian.com/world/2026/may/27/canada-sweden-saab-globaleye-aircraft](https://www.theguardian.com/world/2026/may/27/canada-sweden-saab-globaleye-aircraft)

生成摘要时出错

---

## 37. Incident with Pull Requests, Issues, Git Operations and API Requests

**原文标题**: Incident with Pull Requests, Issues, Git Operations and API Requests

**原文链接**: [https://www.githubstatus.com/incidents/xy1tt3hs572m](https://www.githubstatus.com/incidents/xy1tt3hs572m)

生成摘要时出错

---

## 38. Mini Micro Fantasy Computer

**原文标题**: Mini Micro Fantasy Computer

**原文链接**: [https://miniscript.org/MiniMicro/index.html#about](https://miniscript.org/MiniMicro/index.html#about)

生成摘要时出错

---

## 39. Is "colorectal cancer" rising in "young people"?

**原文标题**: Is "colorectal cancer" rising in "young people"?

**原文链接**: [https://dynomight.net/crc-rates/](https://dynomight.net/crc-rates/)

生成摘要时出错

---

## 40. A sleep-like consolidation mechanism for LLMs

**原文标题**: A sleep-like consolidation mechanism for LLMs

**原文链接**: [https://arxiv.org/abs/2605.26099](https://arxiv.org/abs/2605.26099)

生成摘要时出错

---

## 41. Where does next-token prediction leave us?

**原文标题**: Where does next-token prediction leave us?

**原文链接**: [https://pop.rdi.sh/where-does-next-token-prediction-leave-us/](https://pop.rdi.sh/where-does-next-token-prediction-leave-us/)

生成摘要时出错

---

## 42. AWS Fired the One Employee Who Gave a Damn

**原文标题**: AWS Fired the One Employee Who Gave a Damn

**原文链接**: [https://www.seuros.com/blog/aws-fired-the-human-who-made-the-difference/](https://www.seuros.com/blog/aws-fired-the-human-who-made-the-difference/)

生成摘要时出错

---

## 43. Yoti age checks share facial photos and device fingerprints with third parties

**原文标题**: Yoti age checks share facial photos and device fingerprints with third parties

**原文链接**: [https://techxplore.com/news/2026-05-online-age-pointless-privacy.html](https://techxplore.com/news/2026-05-online-age-pointless-privacy.html)

生成摘要时出错

---

## 44. Valve raises Steam Deck prices by more than $200

**原文标题**: Valve raises Steam Deck prices by more than $200

**原文链接**: [https://www.theverge.com/games/938340/valve-steam-deck-price-increase](https://www.theverge.com/games/938340/valve-steam-deck-price-increase)

生成摘要时出错

---

## 45. Stop Advertising in Your Commits

**原文标题**: Stop Advertising in Your Commits

**原文链接**: [https://akselmo.dev/posts/stop-advertising-in-your-commits/](https://akselmo.dev/posts/stop-advertising-in-your-commits/)

生成摘要时出错

---

## 46. SimCity 3k in 4k (2025)

**原文标题**: SimCity 3k in 4k (2025)

**原文链接**: [https://www.thran.uk/writ/hdid/2025/12/simcity-3k-in-4k.html](https://www.thran.uk/writ/hdid/2025/12/simcity-3k-in-4k.html)

生成摘要时出错

---

## 47. Stack Overflow’s forum is dead but the company’s still kicking

**原文标题**: Stack Overflow’s forum is dead but the company’s still kicking

**原文链接**: [https://sherwood.news/tech/stack-overflow-forum-dead-thanks-ai-but-companys-still-kicking-ai/](https://sherwood.news/tech/stack-overflow-forum-dead-thanks-ai-but-companys-still-kicking-ai/)

生成摘要时出错

---

## 48. Training our own AI models

**原文标题**: Training our own AI models

**原文链接**: [https://posthog.com/blog/training-ai-models](https://posthog.com/blog/training-ai-models)

生成摘要时出错

---

## 49. CVE-2026-28952: Apple macOS 26.5 Kernel Vuln found by Claude

**原文标题**: CVE-2026-28952: Apple macOS 26.5 Kernel Vuln found by Claude

**原文链接**: [https://support.apple.com/en-us/127115](https://support.apple.com/en-us/127115)

生成摘要时出错

---

## 50. The just-say-no engineer was a ZIRP phenomenon

**原文标题**: The just-say-no engineer was a ZIRP phenomenon

**原文链接**: [https://www.seangoedecke.com/the-just-say-no-engineer-was-a-zirp-phenomenon/](https://www.seangoedecke.com/the-just-say-no-engineer-was-a-zirp-phenomenon/)

生成摘要时出错

---

## 51. YouTube to automatically label AI-generated videos

**原文标题**: YouTube to automatically label AI-generated videos

**原文链接**: [https://variety.com/2026/digital/news/youtube-ai-video-labels-automatic-detection-1236758865/](https://variety.com/2026/digital/news/youtube-ai-video-labels-automatic-detection-1236758865/)

生成摘要时出错

---

## 52. Earthion: A New Mega Drive-Style Shoot-Em-Up

**原文标题**: Earthion: A New Mega Drive-Style Shoot-Em-Up

**原文链接**: [https://earthiongame.com/](https://earthiongame.com/)

生成摘要时出错

---

## 53. A portentous reunion

**原文标题**: A portentous reunion

**原文链接**: [https://bcantrill.dtrace.org/2026/05/25/a-portentous-reunion/](https://bcantrill.dtrace.org/2026/05/25/a-portentous-reunion/)

生成摘要时出错

---

## 54. Lombardy increases charges for the construction of data centres in green areas

**原文标题**: Lombardy increases charges for the construction of data centres in green areas

**原文链接**: [https://en.ilsole24ore.com/art/lombardy-introduces-increased-charges-of-up-to-200-per-cent-for-data-centre-construction-in-green-and-agricultural-areas-AI6Jp4ID](https://en.ilsole24ore.com/art/lombardy-introduces-increased-charges-of-up-to-200-per-cent-for-data-centre-construction-in-green-and-agricultural-areas-AI6Jp4ID)

生成摘要时出错

---

## 55. What color is your function? (2015)

**原文标题**: What color is your function? (2015)

**原文链接**: [https://journal.stuffwithstuff.com/2015/02/01/what-color-is-your-function/](https://journal.stuffwithstuff.com/2015/02/01/what-color-is-your-function/)

生成摘要时出错

---

## 56. Performance of Rust Language [pdf]

**原文标题**: Performance of Rust Language [pdf]

**原文链接**: [https://github.com/yugr/rust-slides/](https://github.com/yugr/rust-slides/)

生成摘要时出错

---

## 57. Go: Support for Generic Methods

**原文标题**: Go: Support for Generic Methods

**原文链接**: [https://github.com/golang/go/issues/77273](https://github.com/golang/go/issues/77273)

生成摘要时出错

---

## 58. Sonny Rollins, jazz saxophonist, has died

**原文标题**: Sonny Rollins, jazz saxophonist, has died

**原文链接**: [https://www.rollingstone.com/music/music-news/sonny-rollins-jazz-legend-saxophone-colossus-dead-obit-1234715446/](https://www.rollingstone.com/music/music-news/sonny-rollins-jazz-legend-saxophone-colossus-dead-obit-1234715446/)

生成摘要时出错

---

## 59. Don't Subscribe So Casually

**原文标题**: Don't Subscribe So Casually

**原文链接**: [https://thebestworstcase.substack.com/p/dont-subscribe-so-casually](https://thebestworstcase.substack.com/p/dont-subscribe-so-casually)

生成摘要时出错

---

## 60. From Rust to Ruby

**原文标题**: From Rust to Ruby

**原文链接**: [https://xlii.space/eng/from-rust-to-ruby/](https://xlii.space/eng/from-rust-to-ruby/)

生成摘要时出错

---

## 61. Xiaomi MiMo-v2.5 Series API Permanent Price Reduction Up to 99%

**原文标题**: Xiaomi MiMo-v2.5 Series API Permanent Price Reduction Up to 99%

**原文链接**: [https://platform.xiaomimimo.com/docs/en-US/news/v2.5-price-update](https://platform.xiaomimimo.com/docs/en-US/news/v2.5-price-update)

生成摘要时出错

---

## 62. Corporations can vote in some Delaware elections, judge says

**原文标题**: Corporations can vote in some Delaware elections, judge says

**原文链接**: [https://news.bloomberglaw.com/esg/corporations-have-the-right-to-vote-in-delaware-town-judge-says](https://news.bloomberglaw.com/esg/corporations-have-the-right-to-vote-in-delaware-town-judge-says)

生成摘要时出错

---

## 63. Raft Consensus with a Minority of Nodes

**原文标题**: Raft Consensus with a Minority of Nodes

**原文链接**: [https://padhye.org/raft-minority/](https://padhye.org/raft-minority/)

生成摘要时出错

---

## 64. BadHost – CVE-2026-48710: Starlette Host-Header Auth Bypass

**原文标题**: BadHost – CVE-2026-48710: Starlette Host-Header Auth Bypass

**原文链接**: [https://badhost.org/](https://badhost.org/)

生成摘要时出错

---

## 65. Modern Blu-ray drives can now rip GameCube, Wii, and Xbox 360 games to PC

**原文标题**: Modern Blu-ray drives can now rip GameCube, Wii, and Xbox 360 games to PC

**原文链接**: [https://www.tomshardware.com/video-games/console-gaming/modern-blu-ray-drives-can-now-rip-gamecube-wii-and-xbox-360-games-to-pc-third-party-firmware-unlocks-game-rips-from-physical-media-on-select-players](https://www.tomshardware.com/video-games/console-gaming/modern-blu-ray-drives-can-now-rip-gamecube-wii-and-xbox-360-games-to-pc-third-party-firmware-unlocks-game-rips-from-physical-media-on-select-players)

生成摘要时出错

---

## 66. The Ballad of TIGIT

**原文标题**: The Ballad of TIGIT

**原文链接**: [https://www.owlposting.com/p/the-ballad-of-tigit](https://www.owlposting.com/p/the-ballad-of-tigit)

生成摘要时出错

---

## 67. Flatpak Will Depend on Systemd

**原文标题**: Flatpak Will Depend on Systemd

**原文链接**: [https://www.osnews.com/story/145071/flatpak-will-depend-on-systemd/](https://www.osnews.com/story/145071/flatpak-will-depend-on-systemd/)

生成摘要时出错

---

## 68. Launch HN: Minicor (YC P26) – Windows desktop automations at scale

**原文标题**: Launch HN: Minicor (YC P26) – Windows desktop automations at scale

**原文链接**: [https://www.minicor.com/](https://www.minicor.com/)

生成摘要时出错

---

## 69. Incident with Actions and Pages

**原文标题**: Incident with Actions and Pages

**原文链接**: [https://www.githubstatus.com/incidents/gnftqj9htp0g](https://www.githubstatus.com/incidents/gnftqj9htp0g)

生成摘要时出错

---

## 70. C64 Basic: Game Map Overhead “Camera View”

**原文标题**: C64 Basic: Game Map Overhead “Camera View”

**原文链接**: [https://retrogamecoders.com/overhead-camera-view/](https://retrogamecoders.com/overhead-camera-view/)

生成摘要时出错

---

## 71. Show HN: OpenBrief – Local-first video downloader/summarizer

**原文标题**: Show HN: OpenBrief – Local-first video downloader/summarizer

**原文链接**: [https://github.com/tantara/openbrief](https://github.com/tantara/openbrief)

生成摘要时出错

---

## 72. I bypassed AWS API Gateway auth with a trailing slash. Got $12K bounty

**原文标题**: I bypassed AWS API Gateway auth with a trailing slash. Got $12K bounty

**原文链接**: [https://theguptalog.blogspot.com/2026/04/i-bypassed-aws-api-gateway-auth-with.html](https://theguptalog.blogspot.com/2026/04/i-bypassed-aws-api-gateway-auth-with.html)

生成摘要时出错

---

## 73. AI tools are only as good as your judgment

**原文标题**: AI tools are only as good as your judgment

**原文链接**: [https://theaileverageweekly.com/posts/your-ai-tools-are-only-as-good-as-your-judgment-and-that-s-the-point.html](https://theaileverageweekly.com/posts/your-ai-tools-are-only-as-good-as-your-judgment-and-that-s-the-point.html)

生成摘要时出错

---

## 74. Ferrari shares fall after launch of first EV as Jony Ive design proves divisive

**原文标题**: Ferrari shares fall after launch of first EV as Jony Ive design proves divisive

**原文链接**: [https://www.theguardian.com/business/2026/may/26/ferrari-luce-ev-jony-ive-design-sports-car](https://www.theguardian.com/business/2026/may/26/ferrari-luce-ev-jony-ive-design-sports-car)

生成摘要时出错

---

## 75. The AI bubble isn't like the internet bubble

**原文标题**: The AI bubble isn't like the internet bubble

**原文链接**: [https://pluralistic.net/2026/05/26/the-ai-will-continue/#until-morale-improves](https://pluralistic.net/2026/05/26/the-ai-will-continue/#until-morale-improves)

生成摘要时出错

---

## 76. What Is a Direct Attach Copper (DAC) Cable

**原文标题**: What Is a Direct Attach Copper (DAC) Cable

**原文链接**: [https://www.servethehome.com/what-is-a-direct-attach-copper-dac-cable/](https://www.servethehome.com/what-is-a-direct-attach-copper-dac-cable/)

生成摘要时出错

---

## 77. Xiaomi MiMo Token Plan is Now Globally Available

**原文标题**: Xiaomi MiMo Token Plan is Now Globally Available

**原文链接**: [https://platform.xiaomimimo.com/docs/en-US/welcome](https://platform.xiaomimimo.com/docs/en-US/welcome)

生成摘要时出错

---

## 78. TSDuck: Open-source toolkit for MPEG-TS analysis and manipulation

**原文标题**: TSDuck: Open-source toolkit for MPEG-TS analysis and manipulation

**原文链接**: [https://tsduck.io/](https://tsduck.io/)

生成摘要时出错

---

## 79. Show HN: Posthorn, self-hosted mail gateway

**原文标题**: Show HN: Posthorn, self-hosted mail gateway

**原文链接**: [https://github.com/craigmccaskill/posthorn](https://github.com/craigmccaskill/posthorn)

生成摘要时出错

---

## 80. What Apple and Google are doing to your push notifications

**原文标题**: What Apple and Google are doing to your push notifications

**原文链接**: [https://www.jacquescorbytuech.com/writing/what-apple-and-google-are-doing-your-push-notifications](https://www.jacquescorbytuech.com/writing/what-apple-and-google-are-doing-your-push-notifications)

生成摘要时出错

---

## 81. Germany news: Childfree adults to pay more for elder care

**原文标题**: Germany news: Childfree adults to pay more for elder care

**原文链接**: [https://www.dw.com/en/germany-news-childfree-adults-to-pay-more-for-elder-care/live-77292208](https://www.dw.com/en/germany-news-childfree-adults-to-pay-more-for-elder-care/live-77292208)

生成摘要时出错

---

## 82. Scientists say they've reversed brain aging in mice with a nasal spray

**原文标题**: Scientists say they've reversed brain aging in mice with a nasal spray

**原文链接**: [https://www.sciencedaily.com/releases/2026/05/260526022018.htm](https://www.sciencedaily.com/releases/2026/05/260526022018.htm)

生成摘要时出错

---

## 83. Tunecat: Simple Internet Radio

**原文标题**: Tunecat: Simple Internet Radio

**原文链接**: [https://codeberg.org/lindenii/tunecat/](https://codeberg.org/lindenii/tunecat/)

生成摘要时出错

---

## 84. Eagle 3.1: Collaboration Between the EAGLE Team, vLLM Team, and TorchSpec Team

**原文标题**: Eagle 3.1: Collaboration Between the EAGLE Team, vLLM Team, and TorchSpec Team

**原文链接**: [https://vllm.ai/blog/2026-05-26-eagle-3-1](https://vllm.ai/blog/2026-05-26-eagle-3-1)

生成摘要时出错

---

## 85. Real wages start to shrink in developed countries

**原文标题**: Real wages start to shrink in developed countries

**原文链接**: [https://www.ft.com/content/e126f744-3db9-4305-8871-31f83ebc4ed7](https://www.ft.com/content/e126f744-3db9-4305-8871-31f83ebc4ed7)

生成摘要时出错

---

## 86. Trump DOJ mass-deletes info on Jan. 6 riot cases, incl violent assaults on cops

**原文标题**: Trump DOJ mass-deletes info on Jan. 6 riot cases, incl violent assaults on cops

**原文链接**: [https://text.npr.org/nx-s1-5834992](https://text.npr.org/nx-s1-5834992)

生成摘要时出错

---

## 87. Notes on Pope Leo XIV's Encyclical on AI

**原文标题**: Notes on Pope Leo XIV's Encyclical on AI

**原文链接**: [https://simonwillison.net/2026/May/25/encyclical-on-ai/](https://simonwillison.net/2026/May/25/encyclical-on-ai/)

生成摘要时出错

---

## 88. Show HN: I made an emergency page for my family

**原文标题**: Show HN: I made an emergency page for my family

**原文链接**: [https://help.delduca.org](https://help.delduca.org)

生成摘要时出错

---

## 89. Declassified CIA Cartography Maps from the 1980s

**原文标题**: Declassified CIA Cartography Maps from the 1980s

**原文链接**: [https://brilliantmaps.com/cia-maps-1980s/](https://brilliantmaps.com/cia-maps-1980s/)

生成摘要时出错

---

## 90. DeepSWE: A contamination-free benchmark for long-horizon coding agents

**原文标题**: DeepSWE: A contamination-free benchmark for long-horizon coding agents

**原文链接**: [https://deepswe.datacurve.ai/blog](https://deepswe.datacurve.ai/blog)

生成摘要时出错

---

## 91. Canada losing top talent as workers head to the U.S.

**原文标题**: Canada losing top talent as workers head to the U.S.

**原文链接**: [https://www.bnnbloomberg.ca/investing/market-outlook/2026/05/25/market-outlook-canada-losing-top-talent-as-workers-head-to-the-us/](https://www.bnnbloomberg.ca/investing/market-outlook/2026/05/25/market-outlook-canada-losing-top-talent-as-workers-head-to-the-us/)

生成摘要时出错

---

## 92. The VibeSec Reckoning

**原文标题**: The VibeSec Reckoning

**原文链接**: [https://martinfowler.com/articles/vibesec-reckoning.html](https://martinfowler.com/articles/vibesec-reckoning.html)

生成摘要时出错

---

## 93. XLIDE: VBA without excel

**原文标题**: XLIDE: VBA without excel

**原文链接**: [https://github.com/WilliamSmithEdward/xlide_vscode](https://github.com/WilliamSmithEdward/xlide_vscode)

生成摘要时出错

---

## 94. Gemini, Gophers, and Fingers. Oh My Alternative Internets Beyond HTTPS

**原文标题**: Gemini, Gophers, and Fingers. Oh My Alternative Internets Beyond HTTPS

**原文链接**: [https://brennan.day/gemini-gophers-and-fingers-oh-my-alternative-internets-beyond-https/](https://brennan.day/gemini-gophers-and-fingers-oh-my-alternative-internets-beyond-https/)

生成摘要时出错

---

## 95. Bay Area mom out thousands after scammers use AI to mimic daughter's voice

**原文标题**: Bay Area mom out thousands after scammers use AI to mimic daughter's voice

**原文链接**: [https://abc7news.com/post/bay-area-mom-thousands-scammers-use-ai-mimic-daughters-voice-fake-kidnapping-part-growing-trend/19154381/](https://abc7news.com/post/bay-area-mom-thousands-scammers-use-ai-mimic-daughters-voice-fake-kidnapping-part-growing-trend/19154381/)

生成摘要时出错

---

## 96. Show HN: Open-source Workspace (mail,docs,spreadsheet,drive) web/iOS

**原文标题**: Show HN: Open-source Workspace (mail,docs,spreadsheet,drive) web/iOS

**原文链接**: [https://tinycld.org/](https://tinycld.org/)

生成摘要时出错

---

## 97. Nvidia Vera CPU Benchmarks: Olympus Cores Delivering Great Performance

**原文标题**: Nvidia Vera CPU Benchmarks: Olympus Cores Delivering Great Performance

**原文链接**: [https://www.phoronix.com/review/nvidia-vera-benchmarks](https://www.phoronix.com/review/nvidia-vera-benchmarks)

生成摘要时出错

---

## 98. The Best Engineers Write Less Code

**原文标题**: The Best Engineers Write Less Code

**原文链接**: [https://shvetsm.github.io/posts/the-best-engineers-write-less-code/](https://shvetsm.github.io/posts/the-best-engineers-write-less-code/)

生成摘要时出错

---

## 99. Show HN: A website that tracks every stock trade Congress makes

**原文标题**: Show HN: A website that tracks every stock trade Congress makes

**原文链接**: [https://congress.kadoa.com/](https://congress.kadoa.com/)

生成摘要时出错

---

## 100. Atomically precise mechanosynthesis of carbon structures on hydrogenated Silicon

**原文标题**: Atomically precise mechanosynthesis of carbon structures on hydrogenated Silicon

**原文链接**: [https://arxiv.org/abs/2605.27250](https://arxiv.org/abs/2605.27250)

生成摘要时出错

---

