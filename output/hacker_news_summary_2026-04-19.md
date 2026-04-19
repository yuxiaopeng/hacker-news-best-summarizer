# Hacker News 热门文章摘要 (2026-04-19)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 从数字海洋迁移到赫兹纳

**原文标题**: Migrating from DigitalOcean to Hetzner

**原文链接**: [https://isayeter.com/posts/digitalocean-to-hetzner-migration/](https://isayeter.com/posts/digitalocean-to-hetzner-migration/)

本文详述了将生产环境从DigitalOcean成功迁移到Hetzner的过程，实现了零停机，将每月基础设施成本从1,432美元降至233美元，每年节省14,388美元。此举是由于土耳其的经济状况，使得以美元计价的云服务变得难以承受。

此次迁移涉及庞大的设置：30个MySQL数据库共计248GB，34个Nginx站点，GitLab EE，Neo4j，以及实时的移动应用流量。此外，它还促成了一次重要的操作系统升级，从CentOS 7升级到AlmaLinux 9.7。

零停机策略包含六个阶段：在新服务器上安装完整堆栈、通过rsync克隆Web文件、MySQL主从复制、DNS TTL值缩减、将旧的Nginx服务器转换为反向代理，以及最终的DNS切换。关键在于持续提供服务流量，无论是直接提供还是通过代理。

技术亮点包括使用`mydumper`进行MySQL并行导出/导入，这大大加快了248GB数据库的传输速度。诸如MySQL 5.7到8.0升级问题（通过删除并升级`sys`模式解决）和复制错误（通过`SET GLOBAL slave_exec_mode = 'IDEMPOTENT'`解决）等挑战都得到了细致的解决。一个关键发现是撤销应用程序用户的`SUPER`权限，以在从库上强制执行`read_only`。所有DNS更新、Nginx配置更改和GitLab webhook更新均使用Python脚本自动化完成。

此次迁移在大约24小时内完成，实现了零停机，并以极低的成本获得了一台更强大的服务器（96个逻辑CPU，256GB DDR5内存，2TB NVMe RAID1）。所使用的所有Python脚本均已在GitHub上开源。

---

## 2. Opus 4.6 与 Opus 4.7 的匿名请求令牌比较

**原文标题**: Anonymous request-token comparisons from Opus 4.6 and Opus 4.7

**原文链接**: [https://tokens.billchambers.me/leaderboard](https://tokens.billchambers.me/leaderboard)

本文介绍了一个托管在 billchambers.me 上的网页工具，该工具旨在促进 Anthropic 的 Opus 4.6 和 Opus 4.7 大型语言模型之间的“匿名请求-令牌比较”。该平台的目的是展示这两个 AI 模型在处理其用户社区提交的“真实输入”时，在令牌成本和使用量方面有何不同。

该工具作为一个独立的“Anthropic 令牌成本计算器”，允许用户提交自己的提示，且数据匿名存储。它还会计算并显示这些比较的“社区平均值”。这是一个开源项目，并明确声明其“不隶属于 Anthropic，也未获得 Anthropic 的认可”，作为一个第三方工具，用于分析 AI 模型的令牌经济学。

---

## 3. 为什么日本有这么好的铁路

**原文标题**: Why Japan has such good railways

**原文链接**: [https://worksinprogress.co/issue/why-japan-has-such-good-railways/](https://worksinprogress.co/issue/why-japan-has-such-good-railways/)

日本拥有世界上最成功的铁路系统，客运周转量占28%，远超其他发达国家。其广泛的网络主要由私营企业运营并盈利，与欧美同行不同，获得的公共补贴极少。这一成就并非归因于独特的日本文化，而是得益于健全且可能复制的公共政策。

该系统的机构多样性令人瞩目，它由六家私有化的国有铁路（JR集团）和众多自成立以来就一直是私营的“传统私营铁路”组成。这些公司经常相互竞争，并发展出一种始终如一的商业模式：“铁路主导的都市主义”。他们不仅仅连接城市，更创造城市。东急或阪急等公司将铁路运营与广泛的副业相结合，拥有沿线从住房、超市到医院和游乐园等一切设施。这使他们能够捕获其基础设施所创造的价值，从而形成一个良性循环，即发展反过来促进客流量。

这种模式得益于日本宽松的土地使用法规和“土地整理”方案，这促进了以公共交通为导向的开发，并创建了超高密度的城市中心，非常适合铁路的空间效率。尽管日本也有出色的高速公路，但文章暗示，与西方国家相比，日本政府对汽车的隐性补贴较少。

最终，日本卓越的铁路系统是创新商业结构、灵活土地使用和健全法规的产物，这表明，成功的公共政策而非一成不变的文化特质，能够促进铁路的卓越发展。

---

## 4. Kdenlive 现状

**原文标题**: State of Kdenlive

**原文链接**: [https://kdenlive.org/news/2026/state-2026/](https://kdenlive.org/news/2026/state-2026/)

《Kdenlive 2026年度报告》强调了富有成效的2025年，在平衡新功能、错误修复、用户界面改进和性能的同时，将稳定性作为优先事项。Kdenlive网站重新上线，与MLT和OpenTimelineIO开发者的协作也得到加强。

2025年的主要发布版本包括：
*   **25.04.0**：引入了基于SAM2的背景移除功能，具备强大的自动遮罩工具；改进了OpenTimelineIO的导入/导出；音频波形生成速度提升了300%。
*   **25.08.0**：重点提升了稳定性，修复了超过15个崩溃问题，并带来了重新设计的音频混音器和全面改进的标记/参考线。
*   **25.12.0**：通过新的欢迎界面、灵活的停靠系统和重新设计的项目监视器，增强了用户体验。

展望未来，**26.04**版本将推出监视器镜像和动画过渡预览功能。路线图包括10/12位色彩支持、OpenFX集成、播放优化，以及一个带有时间轴视图（Dopesheet）的重构关键帧系统（由NGI Zero Commons资助支持）。Kdenlive也正在为Microsoft Store发布做准备。

社区参与度强劲，2025年共有38位代码贡献者，其中一半是首次贡献者。在阿姆斯特丹和柏林举办的冲刺活动促进了技术进步和战略规划。2025年，Kdenlive网站下载量超过1150万次，Flatpak月下载量达41,499次。捐款总额为9,344.80欧元，用于支持基础设施和Kdenlive的维护者。该报告呼吁增加社区资金，以加速开发并可能雇佣更多开发者。

---

## 5. 大学教师启用打字机遏制AI代写作业

**原文标题**: College instructor turns to typewriters to curb AI-written work

**原文链接**: [https://sentinelcolorado.com/uncategorized/a-college-instructor-turns-to-typewriters-to-curb-ai-written-work-and-teach-life-lessons/](https://sentinelcolorado.com/uncategorized/a-college-instructor-turns-to-typewriters-to-curb-ai-written-work-and-teach-life-lessons/)

康奈尔大学德语讲师Grit Matthias Phelps因学生在作业中使用人工智能和在线翻译而感到沮丧，因此从2023年春季开始，她在课堂上引入了手动打字机。学生们每学期使用一次这些没有屏幕、拼写检查和删除键的“模拟”机器来完成写作作业。

菲尔普斯的这项举措旨在让学生们摆脱对技术的依赖，体验数字化之前的写作方式，并迫使他们独立思考，而不是依靠人工智能来生成语法完美的作业。她希望学生们在一切数字化之前，理解写作、思考和课堂的真谛。

学生们最初不熟悉打字机的操作，认为其富有挑战性，但最终受益匪浅。大二学生Ratchaphon Lertdamrongwong指出，没有屏幕消除了干扰，而没有唾手可得的答案则促使他更多地与同学互动，并进行更深入的思考。大一新生Catherine Mong尽管最初对错误感到沮丧，但她欣然接受了这种“有趣且富有挑战性”的、没有删除键而必须接受错误的过程。

这项练习迫使学生放慢速度，一次只专注于一项任务，并接受不完美。这种回归“老派”方法（如使用打字机）的举动，反映了教育工作者采用纸笔考试或口试来打击作业中AI使用的全国性趋势。学生们很欣赏这种独特的体验，常常将那些充满错误的打字页视为他们独立努力的实物证据而珍藏。

---

## 6. B-52轰炸机星光跟踪器内的机电角度计算机

**原文标题**: The electromechanical angle computer inside the B-52 bomber's star tracker

**原文链接**: [https://www.righto.com/2026/04/B-52-star-tracker-angle-computer.html](https://www.righto.com/2026/04/B-52-star-tracker-angle-computer.html)

生成摘要时出错

---

## 7. NIST scientists create 'any wavelength' lasers

**原文标题**: NIST scientists create 'any wavelength' lasers

**原文链接**: [https://www.nist.gov/news-events/news/2026/04/any-color-you-nist-scientists-create-any-wavelength-lasers-tiny-circuits](https://www.nist.gov/news-events/news/2026/04/any-color-you-nist-scientists-create-any-wavelength-lasers-tiny-circuits)

NIST scientists have developed groundbreaking integrated photonics chips capable of generating a full spectrum of laser colors on tiny circuits. This innovation addresses the limitation of current bulky, expensive, and power-hungry laser systems, which are typically restricted to only a few wavelengths.

The fingernail-sized chips are created by stacking specialized materials onto silicon wafers. Key to this process is the layering of silicon dioxide, lithium niobate (for electrical control and light modulation), and tantalum pentoxide (tantala), a material capable of transforming a single laser color into a wide range of visible and infrared wavelengths. This multilayered design allows for seamless integration and efficient routing of light between layers.

This breakthrough is a significant step towards miniaturizing quantum technologies like optical atomic clocks and quantum computers, which require precise, bespoke laser colors for different atomic systems. By making these devices cheaper, more compact, and portable, NIST's chips could enable their wider adoption outside specialized labs, impacting areas such as biomedicine, navigation (alternative to GPS), communications, and artificial intelligence. While not yet ready for mass production, this technique provides a clear path forward for making light-based circuitry as powerful and ubiquitous as electronics.

---

## 8. Thoughts and feelings around Claude Design

**原文标题**: Thoughts and feelings around Claude Design

**原文链接**: [https://samhenri.gold/blog/20260418-claude-design/](https://samhenri.gold/blog/20260418-claude-design/)

生成摘要时出错

---

## 9. Vercel says internal systems hit in breach

**原文标题**: Vercel says internal systems hit in breach

**原文链接**: [https://decipher.sc/2026/04/19/vercel-says-internal-systems-hit-in-breach/](https://decipher.sc/2026/04/19/vercel-says-internal-systems-hit-in-breach/)

生成摘要时出错

---

## 10. Traders placed over $1B in perfectly timed bets on the Iran war

**原文标题**: Traders placed over $1B in perfectly timed bets on the Iran war

**原文链接**: [https://www.theguardian.com/world/2026/apr/18/iran-war-bets-ethics-concerns](https://www.theguardian.com/world/2026/apr/18/iran-war-bets-ethics-concerns)

生成摘要时出错

---

## 11. Show HN: I made a calculator that works over disjoint sets of intervals

**原文标题**: Show HN: I made a calculator that works over disjoint sets of intervals

**原文链接**: [https://victorpoughon.github.io/interval-calculator/](https://victorpoughon.github.io/interval-calculator/)

生成摘要时出错

---

## 12. Vercel April 2026 security incident

**原文标题**: Vercel April 2026 security incident

**原文链接**: [https://vercel.com/kb/bulletin/vercel-april-2026-security-incident](https://vercel.com/kb/bulletin/vercel-april-2026-security-incident)

生成摘要时出错

---

## 13. Amiga Graphics Archive

**原文标题**: Amiga Graphics Archive

**原文链接**: [https://amiga.lychesis.net/](https://amiga.lychesis.net/)

生成摘要时出错

---

## 14. The quiet disappearance of the free-range childhood

**原文标题**: The quiet disappearance of the free-range childhood

**原文链接**: [https://bigthink.com/mind-behavior/the-quiet-disappearance-of-the-free-range-childhood/](https://bigthink.com/mind-behavior/the-quiet-disappearance-of-the-free-range-childhood/)

生成摘要时出错

---

## 15. Category Theory Illustrated – Orders

**原文标题**: Category Theory Illustrated – Orders

**原文链接**: [https://abuseofnotation.github.io/category-theory-illustrated/04_order/](https://abuseofnotation.github.io/category-theory-illustrated/04_order/)

生成摘要时出错

---

## 16. Tesla tells HW3 owner to 'be patient' after 7 years of waiting for FSD

**原文标题**: Tesla tells HW3 owner to 'be patient' after 7 years of waiting for FSD

**原文链接**: [https://electrek.co/2026/04/17/tesla-hw3-owners-be-patient-7-years-fsd/](https://electrek.co/2026/04/17/tesla-hw3-owners-be-patient-7-years-fsd/)

生成摘要时出错

---

## 17. Notion leaks email addresses of all editors of any public page

**原文标题**: Notion leaks email addresses of all editors of any public page

**原文链接**: [https://twitter.com/weezerOSINT/status/2045849358462222720](https://twitter.com/weezerOSINT/status/2045849358462222720)

生成摘要时出错

---

## 18. NASA Shuts Off Instrument on Voyager 1 to Keep Spacecraft Operating

**原文标题**: NASA Shuts Off Instrument on Voyager 1 to Keep Spacecraft Operating

**原文链接**: [https://science.nasa.gov/blogs/voyager/2026/04/17/nasa-shuts-off-instrument-on-voyager-1-to-keep-spacecraft-operating/](https://science.nasa.gov/blogs/voyager/2026/04/17/nasa-shuts-off-instrument-on-voyager-1-to-keep-spacecraft-operating/)

生成摘要时出错

---

## 19. The seven programming ur-languages (2022)

**原文标题**: The seven programming ur-languages (2022)

**原文链接**: [https://madhadron.com/programming/seven_ur_languages.html](https://madhadron.com/programming/seven_ur_languages.html)

生成摘要时出错

---

## 20. Airline worker arrested after sharing photos of bomb damage in WhatsApp group

**原文标题**: Airline worker arrested after sharing photos of bomb damage in WhatsApp group

**原文链接**: [https://www.lbc.co.uk/article/dubai-police-spied-private-whatsapp-5HjdXwr_2/](https://www.lbc.co.uk/article/dubai-police-spied-private-whatsapp-5HjdXwr_2/)

生成摘要时出错

---

## 21. A simplified model of Fil-C

**原文标题**: A simplified model of Fil-C

**原文链接**: [https://www.corsix.org/content/simplified-model-of-fil-c](https://www.corsix.org/content/simplified-model-of-fil-c)

生成摘要时出错

---

## 22. The world in which IPv6 was a good design (2017)

**原文标题**: The world in which IPv6 was a good design (2017)

**原文链接**: [https://apenwarr.ca/log/20170810](https://apenwarr.ca/log/20170810)

生成摘要时出错

---

## 23. Keep Pushing: We Get 10 More Days to Reform Section 702

**原文标题**: Keep Pushing: We Get 10 More Days to Reform Section 702

**原文链接**: [https://www.eff.org/deeplinks/2026/04/keep-pushing-we-get-10-more-days-reform-section-702](https://www.eff.org/deeplinks/2026/04/keep-pushing-we-get-10-more-days-reform-section-702)

生成摘要时出错

---

## 24. Dad brains: How fatherhood rewires the male mind

**原文标题**: Dad brains: How fatherhood rewires the male mind

**原文链接**: [https://www.bbc.com/future/article/20260417-fatherhood-how-the-male-brain-and-body-prepare-for-childcare](https://www.bbc.com/future/article/20260417-fatherhood-how-the-male-brain-and-body-prepare-for-childcare)

生成摘要时出错

---

## 25. Amazon is discontinuing Kindle for PC on June 30th

**原文标题**: Amazon is discontinuing Kindle for PC on June 30th

**原文链接**: [https://goodereader.com/blog/kindle/amazon-is-discontinuing-kindle-for-pc-on-june-30th](https://goodereader.com/blog/kindle/amazon-is-discontinuing-kindle-for-pc-on-june-30th)

生成摘要时出错

---

## 26. The creative software industry has declared war on Adobe

**原文标题**: The creative software industry has declared war on Adobe

**原文链接**: [https://www.theverge.com/tech/913765/adobe-rivals-free-creative-software-app-updates](https://www.theverge.com/tech/913765/adobe-rivals-free-creative-software-app-updates)

生成摘要时出错

---

## 27. SPEAKE(a)R: Turn Speakers to Microphones for Fun and Profit [pdf] (2017)

**原文标题**: SPEAKE(a)R: Turn Speakers to Microphones for Fun and Profit [pdf] (2017)

**原文链接**: [https://www.usenix.org/system/files/conference/woot17/woot17-paper-guri.pdf](https://www.usenix.org/system/files/conference/woot17/woot17-paper-guri.pdf)

生成摘要时出错

---

## 28. PgQue: Zero-Bloat Postgres Queue

**原文标题**: PgQue: Zero-Bloat Postgres Queue

**原文链接**: [https://github.com/NikolayS/pgque](https://github.com/NikolayS/pgque)

生成摘要时出错

---

## 29. Show HN: MDV – a Markdown superset for docs, dashboards, and slides with data

**原文标题**: Show HN: MDV – a Markdown superset for docs, dashboards, and slides with data

**原文链接**: [https://github.com/drasimwagan/mdv](https://github.com/drasimwagan/mdv)

生成摘要时出错

---

## 30. Optimizing Ruby Path Methods

**原文标题**: Optimizing Ruby Path Methods

**原文链接**: [https://byroot.github.io/ruby/performance/2026/04/18/faster-paths.html](https://byroot.github.io/ruby/performance/2026/04/18/faster-paths.html)

生成摘要时出错

---

## 31. Landmark ancient-genome study shows surprise acceleration of human evolution

**原文标题**: Landmark ancient-genome study shows surprise acceleration of human evolution

**原文链接**: [https://www.nature.com/articles/d41586-026-01204-5](https://www.nature.com/articles/d41586-026-01204-5)

生成摘要时出错

---

## 32. Why is IPv6 so complicated?

**原文标题**: Why is IPv6 so complicated?

**原文链接**: [https://github.com/becarpenter/misc/blob/main/why6why.md](https://github.com/becarpenter/misc/blob/main/why6why.md)

生成摘要时出错

---

## 33. Zero-Copy GPU Inference from WebAssembly on Apple Silicon

**原文标题**: Zero-Copy GPU Inference from WebAssembly on Apple Silicon

**原文链接**: [https://abacusnoir.com/2026/04/18/zero-copy-gpu-inference-from-webassembly-on-apple-silicon/](https://abacusnoir.com/2026/04/18/zero-copy-gpu-inference-from-webassembly-on-apple-silicon/)

生成摘要时出错

---

## 34. Fuzix OS

**原文标题**: Fuzix OS

**原文链接**: [https://www.fuzix.org/](https://www.fuzix.org/)

生成摘要时出错

---

## 35. Graphs that explain the state of AI in 2026

**原文标题**: Graphs that explain the state of AI in 2026

**原文链接**: [https://spectrum.ieee.org/state-of-ai-index-2026](https://spectrum.ieee.org/state-of-ai-index-2026)

生成摘要时出错

---

## 36. Notes from the SF Peptide Scene

**原文标题**: Notes from the SF Peptide Scene

**原文链接**: [https://12gramsofcarbon.com/p/notes-from-the-sf-peptide-scene](https://12gramsofcarbon.com/p/notes-from-the-sf-peptide-scene)

生成摘要时出错

---

## 37. America Lost the Mandate of Heaven

**原文标题**: America Lost the Mandate of Heaven

**原文链接**: [https://geohot.github.io//blog/jekyll/update/2026/04/18/america-mandate-of-heaven.html](https://geohot.github.io//blog/jekyll/update/2026/04/18/america-mandate-of-heaven.html)

生成摘要时出错

---

## 38. The FBI Director Is MIA

**原文标题**: The FBI Director Is MIA

**原文链接**: [https://www.theatlantic.com/politics/2026/04/kash-patel-fbi-director-drinking-absences/686839/](https://www.theatlantic.com/politics/2026/04/kash-patel-fbi-director-drinking-absences/686839/)

生成摘要时出错

---

## 39. Turtle WoW classic server announces shutdown after Blizzard wins injunction

**原文标题**: Turtle WoW classic server announces shutdown after Blizzard wins injunction

**原文链接**: [https://www.pcgamer.com/games/world-of-warcraft/turtle-wow-classic-server-announces-shutdown-after-blizzard-wins-injunction/](https://www.pcgamer.com/games/world-of-warcraft/turtle-wow-classic-server-announces-shutdown-after-blizzard-wins-injunction/)

生成摘要时出错

---

## 40. Amazon won't release Fire Sticks that support sideloading anymore

**原文标题**: Amazon won't release Fire Sticks that support sideloading anymore

**原文链接**: [https://arstechnica.com/gadgets/2026/04/amazon-wont-release-fire-sticks-that-support-sideloading-anymore/](https://arstechnica.com/gadgets/2026/04/amazon-wont-release-fire-sticks-that-support-sideloading-anymore/)

生成摘要时出错

---

## 41. Flock Condemns False Child Predator Allegations, Yet Calls Critics Terrorists

**原文标题**: Flock Condemns False Child Predator Allegations, Yet Calls Critics Terrorists

**原文链接**: [https://ipvm.com/reports/flock-allegations-critics](https://ipvm.com/reports/flock-allegations-critics)

生成摘要时出错

---

## 42. When moving fast, talking is the first thing to break

**原文标题**: When moving fast, talking is the first thing to break

**原文链接**: [https://daverupert.com/2026/04/more-talk-less-grok/](https://daverupert.com/2026/04/more-talk-less-grok/)

生成摘要时出错

---

## 43. The USDA's gardening zones have shifted. (Interactive app and map) (2024)

**原文标题**: The USDA's gardening zones have shifted. (Interactive app and map) (2024)

**原文链接**: [https://apps.npr.org/plant-hardiness-garden-map/](https://apps.npr.org/plant-hardiness-garden-map/)

生成摘要时出错

---

## 44. PM Carney declares U.S. ties now a 'weakness' in address to Canadians

**原文标题**: PM Carney declares U.S. ties now a 'weakness' in address to Canadians

**原文链接**: [https://www.ctvnews.ca/politics/article/pm-carney-declares-us-ties-now-a-weakness-in-address-to-canadians/](https://www.ctvnews.ca/politics/article/pm-carney-declares-us-ties-now-a-weakness-in-address-to-canadians/)

生成摘要时出错

---

## 45. Tesla Cybertruck sales inflated: SpaceX bought 1,279 units

**原文标题**: Tesla Cybertruck sales inflated: SpaceX bought 1,279 units

**原文链接**: [https://electrek.co/2026/04/16/tesla-cybertruck-spacex-1279-q4-sales-inflated/](https://electrek.co/2026/04/16/tesla-cybertruck-spacex-1279-q4-sales-inflated/)

生成摘要时出错

---

## 46. "Liberation Day" at OpenAI as multiple senior executives announce leaving

**原文标题**: "Liberation Day" at OpenAI as multiple senior executives announce leaving

**原文链接**: [https://mas.to/@carnage4life/116422881496195720](https://mas.to/@carnage4life/116422881496195720)

生成摘要时出错

---

## 47. Russia's doping program is run by the same FSB team that poisoned Navalny

**原文标题**: Russia's doping program is run by the same FSB team that poisoned Navalny

**原文链接**: [https://theins.press/en/inv/291614](https://theins.press/en/inv/291614)

生成摘要时出错

---

## 48. Changes in the system prompt between Claude Opus 4.6 and 4.7

**原文标题**: Changes in the system prompt between Claude Opus 4.6 and 4.7

**原文链接**: [https://simonwillison.net/2026/Apr/18/opus-system-prompt/](https://simonwillison.net/2026/Apr/18/opus-system-prompt/)

生成摘要时出错

---

## 49. America will come to regret its war on taxes

**原文标题**: America will come to regret its war on taxes

**原文链接**: [https://economist.com/leaders/2026/04/16/america-will-come-to-regret-its-war-on-taxes](https://economist.com/leaders/2026/04/16/america-will-come-to-regret-its-war-on-taxes)

生成摘要时出错

---

## 50. Casus Belli Engineering

**原文标题**: Casus Belli Engineering

**原文链接**: [https://marcosmagueta.com/blog/casus-belli-engineering/](https://marcosmagueta.com/blog/casus-belli-engineering/)

生成摘要时出错

---

## 51. Binary GCD

**原文标题**: Binary GCD

**原文链接**: [https://en.algorithmica.org/hpc/algorithms/gcd/#binary-gcd](https://en.algorithmica.org/hpc/algorithms/gcd/#binary-gcd)

生成摘要时出错

---

## 52. Traders place $760M bet on falling oil ahead of Hormuz announcement

**原文标题**: Traders place $760M bet on falling oil ahead of Hormuz announcement

**原文链接**: [https://www.reuters.com/sustainability/boards-policy-regulation/traders-place-760-million-bet-falling-oil-ahead-hormuz-announcement-2026-04-17/](https://www.reuters.com/sustainability/boards-policy-regulation/traders-place-760-million-bet-falling-oil-ahead-hormuz-announcement-2026-04-17/)

生成摘要时出错

---

## 53. It is incorrect to "normalize" // in HTTP URL paths

**原文标题**: It is incorrect to "normalize" // in HTTP URL paths

**原文链接**: [https://runxiyu.org/comp/doubleslash/](https://runxiyu.org/comp/doubleslash/)

生成摘要时出错

---

## 54. Show HN: Prompt-to-Excalidraw demo with Gemma 4 E2B in the browser (3.1GB)

**原文标题**: Show HN: Prompt-to-Excalidraw demo with Gemma 4 E2B in the browser (3.1GB)

**原文链接**: [https://teamchong.github.io/turboquant-wasm/draw.html](https://teamchong.github.io/turboquant-wasm/draw.html)

生成摘要时出错

---

## 55. The RAM shortage could last years

**原文标题**: The RAM shortage could last years

**原文链接**: [https://www.theverge.com/ai-artificial-intelligence/914672/the-ram-shortage-could-last-years](https://www.theverge.com/ai-artificial-intelligence/914672/the-ram-shortage-could-last-years)

生成摘要时出错

---

## 56. Why Zip drives dominated the 90s, then vanished almost overnight

**原文标题**: Why Zip drives dominated the 90s, then vanished almost overnight

**原文链接**: [https://www.xda-developers.com/zip-drives-dominated-90s-vanished-almost-overnight/](https://www.xda-developers.com/zip-drives-dominated-90s-vanished-almost-overnight/)

生成摘要时出错

---

## 57. Reflecting on my own strange year at Uber

**原文标题**: Reflecting on my own strange year at Uber

**原文链接**: [https://anon-ex-uber.medium.com/reflecting-on-my-own-strange-year-at-uber-e73165422245](https://anon-ex-uber.medium.com/reflecting-on-my-own-strange-year-at-uber-e73165422245)

生成摘要时出错

---

## 58. Using a USB switch as a full KVM

**原文标题**: Using a USB switch as a full KVM

**原文链接**: [https://luke.hsiao.dev/blog/display-switch/](https://luke.hsiao.dev/blog/display-switch/)

生成摘要时出错

---

## 59. My first impressions on ROCm and Strix Halo

**原文标题**: My first impressions on ROCm and Strix Halo

**原文链接**: [https://blog.marcoinacio.com/posts/my-first-impressions-rocm-strix-halo/](https://blog.marcoinacio.com/posts/my-first-impressions-rocm-strix-halo/)

生成摘要时出错

---

## 60. 4-bit floating point FP4

**原文标题**: 4-bit floating point FP4

**原文链接**: [https://www.johndcook.com/blog/2026/04/17/fp4/](https://www.johndcook.com/blog/2026/04/17/fp4/)

生成摘要时出错

---

## 61. Matt Mullenweg Overrules Core Committers; Puts Akismet on WP 7's Connector List

**原文标题**: Matt Mullenweg Overrules Core Committers; Puts Akismet on WP 7's Connector List

**原文链接**: [https://www.therepository.email/matt-mullenweg-overrules-core-committers-to-put-akismet-on-wordpress-7-0s-connectors-screen](https://www.therepository.email/matt-mullenweg-overrules-core-committers-to-put-akismet-on-wordpress-7-0s-connectors-screen)

生成摘要时出错

---

## 62. Young sons of U.S. marshal ride horseback from Oklahoma to New York (2018)

**原文标题**: Young sons of U.S. marshal ride horseback from Oklahoma to New York (2018)

**原文链接**: [https://texascooppower.com/the-astonishing-ride-of-the-abernathy-boys/](https://texascooppower.com/the-astonishing-ride-of-the-abernathy-boys/)

生成摘要时出错

---

## 63. Remember? "Sideloading" is here to stay, and won't go away, they said?

**原文标题**: Remember? "Sideloading" is here to stay, and won't go away, they said?

**原文链接**: [https://floss.social/@IzzyOnDroid/116415766636505917](https://floss.social/@IzzyOnDroid/116415766636505917)

生成摘要时出错

---

## 64. I dug into the Postgres sources to write my own WAL receiver

**原文标题**: I dug into the Postgres sources to write my own WAL receiver

**原文链接**: [https://medium.com/@mailbox.sq7/a-long-story-about-how-i-dug-into-the-postgresql-source-code-to-write-my-own-wal-receiver-and-what-53fd251d8f25](https://medium.com/@mailbox.sq7/a-long-story-about-how-i-dug-into-the-postgresql-source-code-to-write-my-own-wal-receiver-and-what-53fd251d8f25)

生成摘要时出错

---

## 65. Apple TV's Upcoming Cyberpunk Series Will Be the Matrix Meets Blade Runner

**原文标题**: Apple TV's Upcoming Cyberpunk Series Will Be the Matrix Meets Blade Runner

**原文链接**: [https://screenrant.com/neuromancer-apple-tv-matrix-meets-blade-runner/](https://screenrant.com/neuromancer-apple-tv-matrix-meets-blade-runner/)

生成摘要时出错

---

## 66. Show HN: AI Subroutines – Run automation scripts inside your browser tab

**原文标题**: Show HN: AI Subroutines – Run automation scripts inside your browser tab

**原文链接**: [https://www.rtrvr.ai/blog/ai-subroutines-zero-token-deterministic-automation](https://www.rtrvr.ai/blog/ai-subroutines-zero-token-deterministic-automation)

生成摘要时出错

---

## 67. Global freedom declined for the 20th consecutive year in 2025

**原文标题**: Global freedom declined for the 20th consecutive year in 2025

**原文链接**: [https://freedomhouse.org/report/freedom-world/2026/growing-shadow-autocracy](https://freedomhouse.org/report/freedom-world/2026/growing-shadow-autocracy)

生成摘要时出错

---

## 68. Trump deal with IRS could see him given $14B in taxpayer money

**原文标题**: Trump deal with IRS could see him given $14B in taxpayer money

**原文链接**: [https://www.9news.com.au/world/donald-trump-irs-lawsuit-suing-10-billion-dollars-tax-office-usa-politics-news/929663f2-f255-4936-8084-1d986ee08d65](https://www.9news.com.au/world/donald-trump-irs-lawsuit-suing-10-billion-dollars-tax-office-usa-politics-news/929663f2-f255-4936-8084-1d986ee08d65)

生成摘要时出错

---

## 69. Shuttered startups are selling old Slack chats and emails to AI companies

**原文标题**: Shuttered startups are selling old Slack chats and emails to AI companies

**原文链接**: [https://www.fastcompany.com/91528808/shuttered-startups-are-selling-old-slack-chats-and-emails-to-ai-companies](https://www.fastcompany.com/91528808/shuttered-startups-are-selling-old-slack-chats-and-emails-to-ai-companies)

生成摘要时出错

---

## 70. Maine Said No to New Data Centers. Other States Are Racing to Follow

**原文标题**: Maine Said No to New Data Centers. Other States Are Racing to Follow

**原文链接**: [https://www.motherjones.com/environment/2026/04/maine-ai-data-center-moratorium-ban-energy-grid/](https://www.motherjones.com/environment/2026/04/maine-ai-data-center-moratorium-ban-energy-grid/)

生成摘要时出错

---

## 71. Cerebras S-1

**原文标题**: Cerebras S-1

**原文链接**: [https://www.sec.gov/Archives/edgar/data/2021728/000162828026025762/cerebras-sx1april2026.htm](https://www.sec.gov/Archives/edgar/data/2021728/000162828026025762/cerebras-sx1april2026.htm)

生成摘要时出错

---

## 72. There is no you in your brain – your identity is a "society of the mind"

**原文标题**: There is no you in your brain – your identity is a "society of the mind"

**原文链接**: [https://bigthink.com/books/our-brains-our-selves/](https://bigthink.com/books/our-brains-our-selves/)

生成摘要时出错

---

## 73. Show HN: Faceoff – A terminal UI for following NHL games

**原文标题**: Show HN: Faceoff – A terminal UI for following NHL games

**原文链接**: [https://www.vincentgregoire.com/faceoff/](https://www.vincentgregoire.com/faceoff/)

生成摘要时出错

---

## 74. Fulu bounty for Ring Camera jailbreak reaches $23k

**原文标题**: Fulu bounty for Ring Camera jailbreak reaches $23k

**原文链接**: [https://bounties.fulu.org/bounties/ring-video-doorbells](https://bounties.fulu.org/bounties/ring-video-doorbells)

生成摘要时出错

---

## 75. From Endless Frontier to Enemy of the People: The Assault on Public Science

**原文标题**: From Endless Frontier to Enemy of the People: The Assault on Public Science

**原文链接**: [https://www.lawfaremedia.org/article/from-endless-frontier-to-enemy-of-the-people--the-assault-on-public-science](https://www.lawfaremedia.org/article/from-endless-frontier-to-enemy-of-the-people--the-assault-on-public-science)

生成摘要时出错

---

## 76. Bluetooth tracker hidden in postcard and mailed to warship exposed its location

**原文标题**: Bluetooth tracker hidden in postcard and mailed to warship exposed its location

**原文链接**: [https://www.tomshardware.com/tech-industry/cyber-security/bluetooth-tracker-hidden-in-a-postcard-and-mailed-to-a-warship-exposed-its-location-a-eur5-gadget-put-a-eur500-million-dutch-ship-at-risk-for-24-hours](https://www.tomshardware.com/tech-industry/cyber-security/bluetooth-tracker-hidden-in-a-postcard-and-mailed-to-a-warship-exposed-its-location-a-eur5-gadget-put-a-eur500-million-dutch-ship-at-risk-for-24-hours)

生成摘要时出错

---

## 77. The big business of survival bunkers

**原文标题**: The big business of survival bunkers

**原文链接**: [https://www.economist.com/united-states/2026/04/16/the-big-business-of-survival-bunkers](https://www.economist.com/united-states/2026/04/16/the-big-business-of-survival-bunkers)

生成摘要时出错

---

## 78. EU age verification app: "Worry-free package" with security vulnerabilities

**原文标题**: EU age verification app: "Worry-free package" with security vulnerabilities

**原文链接**: [https://www.heise.de/en/news/EU-age-verification-app-Worry-free-package-with-security-vulnerabilities-11262921.html](https://www.heise.de/en/news/EU-age-verification-app-Worry-free-package-with-security-vulnerabilities-11262921.html)

生成摘要时出错

---

## 79. In the AI propaganda war, Iran is winning

**原文标题**: In the AI propaganda war, Iran is winning

**原文链接**: [https://www.economist.com/culture/2026/04/17/in-the-ai-propaganda-war-iran-is-winning](https://www.economist.com/culture/2026/04/17/in-the-ai-propaganda-war-iran-is-winning)

生成摘要时出错

---

## 80. Claude Opus 4.7 Intelligence, Performance and Price Analysis

**原文标题**: Claude Opus 4.7 Intelligence, Performance and Price Analysis

**原文链接**: [https://artificialanalysis.ai/models/claude-opus-4-7](https://artificialanalysis.ai/models/claude-opus-4-7)

生成摘要时出错

---

## 81. Uber's AI Push Hits a Wall–CTO Says Budget Struggles Despite $3.4B Spend

**原文标题**: Uber's AI Push Hits a Wall–CTO Says Budget Struggles Despite $3.4B Spend

**原文链接**: [https://finance.yahoo.com/sectors/technology/articles/ubers-anthropic-ai-push-hits-223109852.html](https://finance.yahoo.com/sectors/technology/articles/ubers-anthropic-ai-push-hits-223109852.html)

生成摘要时出错

---

## 82. The Bromine Chokepoint: How Strife Could Halt Production of World’s Memory Chips

**原文标题**: The Bromine Chokepoint: How Strife Could Halt Production of World’s Memory Chips

**原文链接**: [https://warontherocks.com/cogs-of-war/the-bromine-chokepoint-how-strife-in-the-middle-east-could-halt-production-of-the-worlds-memory-chips/](https://warontherocks.com/cogs-of-war/the-bromine-chokepoint-how-strife-in-the-middle-east-could-halt-production-of-the-worlds-memory-chips/)

生成摘要时出错

---

## 83. Sidephone: A minimalist Android phone with swappable USB keypads

**原文标题**: Sidephone: A minimalist Android phone with swappable USB keypads

**原文链接**: [https://www.sidephone.com/](https://www.sidephone.com/)

生成摘要时出错

---

## 84. Sherry Turkle: "We're losing the raw human part of being with each other" (2013)

**原文标题**: Sherry Turkle: "We're losing the raw human part of being with each other" (2013)

**原文链接**: [https://www.theguardian.com/science/2013/may/05/rational-heroes-sherry-turkle-mit](https://www.theguardian.com/science/2013/may/05/rational-heroes-sherry-turkle-mit)

生成摘要时出错

---

## 85. Deutsche Telekom has a bad DKIM key

**原文标题**: Deutsche Telekom has a bad DKIM key

**原文链接**: [https://infosec.exchange/@badkeys/116407565746342278](https://infosec.exchange/@badkeys/116407565746342278)

生成摘要时出错

---

## 86. PostgreSQL production incident caused by transaction ID wraparound

**原文标题**: PostgreSQL production incident caused by transaction ID wraparound

**原文链接**: [https://www.sqlservercentral.com/articles/i-too-have-a-production-story-a-downtime-caused-by-postgres-transaction-id-wraparound-problem](https://www.sqlservercentral.com/articles/i-too-have-a-production-story-a-downtime-caused-by-postgres-transaction-id-wraparound-problem)

生成摘要时出错

---

