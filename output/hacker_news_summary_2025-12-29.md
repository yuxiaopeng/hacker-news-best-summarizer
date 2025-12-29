# Hacker News 热门文章摘要 (2025-12-29)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 原图是什么样子

**原文标题**: What an unprocessed photo looks like

**原文链接**: [https://maurycyz.com/misc/raw_photo/](https://maurycyz.com/misc/raw_photo/)

相机传感器未经处理的照片，远非我们所感知到的样子。最初，它只是一幅由模数转换器 (ADC) 值组成的“灰蒙蒙”图像，通常未充分利用其理论范围，且缺乏对比度。

要转换为可观看的图像，需要经过以下几个处理步骤：

1.  **定标：** 初始 ADC 值需要映射到可显示的黑白范围，以提高对比度，将“灰蒙蒙”的图像转换为具有更清晰明暗色调的图像。
2.  **去马赛克：** 相机传感器不直接感知颜色；它们使用拜耳滤色阵列，其中每个像素只捕获红色、绿色或蓝色光。为了创建全彩图像，去马赛克算法会平均相邻像素值，以插值每个像素缺失的颜色信息。
3.  **色调映射 (伽马校正)：** 即使在去马赛克之后，图像仍显得很暗。这是因为与传感器和人眼相比，显示技术的动态范围有限。此外，人眼对亮度的感知是非线性的。应用非线性曲线（如sRGB）可以提亮较暗区域，使图像更准确地呈现感知的亮度。
4.  **白平衡：** 相机传感器可能对某些颜色（如绿色）更敏感，去马赛克可能会放大这种敏感性，导致偏色。白平衡通过调整每个颜色通道的强度来校正这些问题，确保中性色显示为中性。这一步通常需要在色调映射之前在线性数据上完成。

文章总结道，即使是“机内”JPEG图像也经过了大量的数学处理。在编辑软件中调整图像并非使其“虚假”，而只是对相同原始数据进行不同形式的呈现，旨在显示技术限制内更好地复制人眼感知。

---

## 2. 日历

**原文标题**: Calendar

**原文链接**: [https://neatnik.net/calendar/?year=2026](https://neatnik.net/calendar/?year=2026)

本页面提供一份2026年全年一页式日历，旨在将所有日期呈现在任意尺寸的单张纸上。为获得最佳打印效果，建议用户将打印机设置为横向并禁用页眉和页脚。这份日历鼓励用户一眼纵览全年，折叠便于携带，记录笔记，规划活动，并观察时间的流逝。日历中还包含一则普遍的善意信息。本页日历由Neatnik创建。

---

## 3. Growing up in “404 Not Found”: China's nuclear city in the Gobi Desert

**原文标题**: Growing up in “404 Not Found”: China's nuclear city in the Gobi Desert

**原文链接**: [https://substack.com/inbox/post/182743659](https://substack.com/inbox/post/182743659)

生成摘要时出错

---

## 4. 仅用 HTML 替换 JavaScript

**原文标题**: Replacing JavaScript with Just HTML

**原文链接**: [https://www.htmhell.dev/adventcalendar/2025/27/](https://www.htmhell.dev/adventcalendar/2025/27/)

Aaron T. Grogg的文章《仅用HTML替代JS》倡导利用原生的HTML和CSS功能，以减少对JavaScript在常见网页功能上的依赖。该文章于2025年12月27日发表，认为尽管JS一直至关重要，但许多它传统上处理的任务现在可以由现代HTML和CSS更高效地完成，从而带来更好的用户体验。

核心前提是，将功能卸载到原生浏览器实现中，意味着需要下载、解压缩、评估和内存中维护的JavaScript更少。这将JS解放出来用于更复杂的任务，同时提高网站性能。

Grogg提供了实用示例：
1.  **手风琴/可展开内容面板：** 通过`<details>`和`<summary>`元素实现，提供原生的打开/关闭状态，并可使用`name`属性实现类似单选按钮的行为。
2.  **带自动过滤建议的输入下拉框：** 使用带有`list`属性的`<input>`元素实现，该属性链接到一个`<datalist>`元素，以实现选项的自动过滤。
3.  **模态框/弹出窗口：** 被`<dialog>`元素上的`popover`和`popovertarget`属性替代，能够实现各种类型的弹出窗口，并具有内置的轻量级关闭和辅助功能。
4.  **屏外导航/内容：** 结合CSS动画过渡，使用`popover`属性，创建无需JavaScript的屏外导航菜单。

该文章鼓励开发人员在可用时优先考虑原生解决方案，尊重JavaScript，将其用于真正需要它的地方，从而创建更轻量、更快速的Web应用程序。

---

## 5. 被德国铁路绑架

**原文标题**: Kidnapped by Deutsche Bahn

**原文链接**: [https://www.theocharis.dev/blog/kidnapped-by-deutsche-bahn/](https://www.theocharis.dev/blog/kidnapped-by-deutsche-bahn/)

The article, "Kidnapped by Deutsche Bahn," recounts a frustrating Christmas Eve train journey on December 24th, 2025, that turned into an unexpected ordeal. The author planned a 35-kilometer trip from Cologne to Meckenheim, but the train, already twenty minutes late, announced "issues around Bonn," necessitating a detour.

The author decided to exit at Troisdorf to be picked up by his father. However, as the RE5 train approached Troisdorf, the driver announced it couldn't stop because it was "not registered" for the tracks. The author watched Troisdorf, and his waiting father, pass by. He was unexpectedly carried to Neuwied, 63 kilometers from his grandmother's house and in a different federal state—further away than his starting point.

Feeling like "cargo" and "kidnapped," the author noted the shared frustration among passengers. He also highlighted Deutsche Bahn's lenient punctuality metrics, where trains less than six minutes late are "on time," and cancelled trains aren't counted. His eventual compensation for this severe delay was a mere 1.50 EUR, below the 4.00 EUR minimum payout threshold, meaning he was "kidnapped at a loss." The piece sarcastically details the systemic unreliability and public exasperation with DB's service.

---

## 6. 我们如何将沟通输给了娱乐

**原文标题**: How we lost communication to entertainment

**原文链接**: [https://ploum.net/2025-12-15-communication-entertainment.html](https://ploum.net/2025-12-15-communication-entertainment.html)

生成摘要时出错

---

## 7. 对NHS中的帕兰提尔说不

**原文标题**: Say No to Palantir in the NHS

**原文链接**: [https://notopalantir.goodlawproject.org/email-to-target/stop-palantir-in-the-nhs/](https://notopalantir.goodlawproject.org/email-to-target/stop-palantir-in-the-nhs/)

本文呼吁公众“拒绝Palantir进入NHS”，反对英格兰国民医疗服务体系（NHS England）推出这家美国间谍技术公司用于管理健康记录的软件。

这项运动强调了对Palantir背景的严重担忧，引用其据称在美国参与大规模驱逐出境，并促成加沙种族灭绝。此外，Palantir的联合创始人彼得·蒂尔（Peter Thiel）因其对NHS的公开敌意而闻名，他曾声称NHS“让人生病”，并暗示英国公众因支持NHS而患有“斯德哥尔摩综合症”。

该文章警告不要允许这样一家公司控制英国的医疗保健系统，并呼吁采取紧急行动。它提供了一个工具，供个人检查他们的当地NHS信托机构是否已采用该软件。主要的行动呼吁是向当地NHS信托机构以及卫生大臣韦斯·斯特里廷（Wes Streeting）发送电子邮件，要求他们拒绝Palantir，尤其是在政府向各信托机构施压要求其采用该软件的情况下。

---

## 8. You can make up HTML tags

**原文标题**: You can make up HTML tags

**原文链接**: [https://maurycyz.com/misc/make-up-tags/](https://maurycyz.com/misc/make-up-tags/)

本文强调HTML开发者可以创建和使用自定义标签（例如`<cool-thing>`），而不是使用带有类的通用`div`标签。浏览器会自动将这些未识别的标签视为通用元素，并应用在CSS中为其定义的任何样式。这并非一个异常，而是标准化行为。在自定义标签名称中包含连字符（例如`<main-article>`）可以确保它们不会与未来的HTML标准冲突。

这种方法的主要好处是极大提升了代码的可读性和可维护性，尤其对于复杂或深度嵌套的结构。文章对比了一系列难以理解的带类的嵌套`div`结构，以及使用描述性自定义标签的结构。后者消除了对`</div>`进行计数的需要，使得理解结构和精确找到插入点变得容易得多。尽管在适当情况下应使用现有的语义化HTML标签，但自定义标签为大量使用带有众多类名的`<div>`或`<span>`提供了一种更具可读性的替代方案，从而为自定义组件提供了更好的清晰度。

---

## 9. 去年我的 Mac：难以置信

**原文标题**: Last Year on My Mac: Look Back in Disbelief

**原文链接**: [https://eclecticlight.co/2025/12/28/last-year-on-my-mac-look-back-in-disbelief/](https://eclecticlight.co/2025/12/28/last-year-on-my-mac-look-back-in-disbelief/)

The author expresses profound disappointment with macOS Tahoe's "Liquid Glass" interface changes, stating that feedback from beta testing was ignored and subsequent updates (26.1, 26.2) worsened or failed to address issues.

Key criticisms include:
1.  **Excessively Rounded Corners:** Tahoe's increased window corner radius is a misfit for rectangular content, causing cropping, wasted space, and inconsistent appearance across apps.
2.  **Enlarged Controls:** Controls are bigger but offer no functional benefit, often leading to visual clutter and overlapping elements.
3.  **Uniform App Icons:** The enforced square shape restricts visual cues, making many bundled and Apple apps harder to distinguish and recall in the Dock.
4.  **Lack of Tonal Contrast ("Whiteout"):** Both Light Mode (bleached-out white) and Dark Mode (moonless night) lack sufficient contrast, making it difficult to discern controls, text fields, and other interface elements.
5.  **Problematic Transparency ("Wet-on-wet"):** Extensive transparency renders elements like search boxes and window titles incomprehensible when underlaid by content, creating a confusing and distracting visual experience.
6.  **Accessibility Regression:** The "Reduce Transparency" control in Accessibility settings no longer effectively lessens these visual effects, a significant regression.

The author, drawing on experience with older Apple interfaces, concludes that Tahoe sacrifices clarity and functionality, making the display harder to read and use.

---

## 10. Show HN: Z80-μLM, a 'Conversational AI' That Fits in 40KB

**原文标题**: Show HN: Z80-μLM, a 'Conversational AI' That Fits in 40KB

**原文链接**: [https://github.com/HarryR/z80ai](https://github.com/HarryR/z80ai)

生成摘要时出错

---

## 11. Fathers’ choices may be packaged and passed down in sperm RNA

**原文标题**: Fathers’ choices may be packaged and passed down in sperm RNA

**原文链接**: [https://www.quantamagazine.org/how-dads-fitness-may-be-packaged-and-passed-down-in-sperm-rna-20251222/](https://www.quantamagazine.org/how-dads-fitness-may-be-packaged-and-passed-down-in-sperm-rna-20251222/)

生成摘要时出错

---

## 12. GOG is getting acquired by its original co-founder: What it means for you

**原文标题**: GOG is getting acquired by its original co-founder: What it means for you

**原文链接**: [https://www.gog.com/blog/gog-is-getting-acquired-by-its-original-co-founder-what-it-means-for-you/](https://www.gog.com/blog/gog-is-getting-acquired-by-its-original-co-founder-what-it-means-for-you/)

生成摘要时出错

---

## 13. As AI gobbles up chips, prices for devices may rise

**原文标题**: As AI gobbles up chips, prices for devices may rise

**原文链接**: [https://www.npr.org/2025/12/28/nx-s1-5656190/ai-chips-memory-prices-ram](https://www.npr.org/2025/12/28/nx-s1-5656190/ai-chips-memory-prices-ram)

生成摘要时出错

---

## 14. Learn computer graphics from scratch and for free

**原文标题**: Learn computer graphics from scratch and for free

**原文链接**: [https://www.scratchapixel.com](https://www.scratchapixel.com)

生成摘要时出错

---

## 15. Rainbow Six Siege hacked as players get billions of credits and random bans

**原文标题**: Rainbow Six Siege hacked as players get billions of credits and random bans

**原文链接**: [https://www.shanethegamer.com/esports-news/rainbow-six-siege-hacked-global-server-outage/](https://www.shanethegamer.com/esports-news/rainbow-six-siege-hacked-global-server-outage/)

生成摘要时出错

---

## 16. Building a macOS app to know when my Mac is thermal throttling

**原文标题**: Building a macOS app to know when my Mac is thermal throttling

**原文链接**: [https://stanislas.blog/2025/12/macos-thermal-throttling-app/](https://stanislas.blog/2025/12/macos-thermal-throttling-app/)

生成摘要时出错

---

## 17. Software engineers should be a little bit cynical

**原文标题**: Software engineers should be a little bit cynical

**原文链接**: [https://www.seangoedecke.com/a-little-bit-cynical/](https://www.seangoedecke.com/a-little-bit-cynical/)

生成摘要时出错

---

## 18. Stepping down as Mockito maintainer after ten years

**原文标题**: Stepping down as Mockito maintainer after ten years

**原文链接**: [https://github.com/mockito/mockito/issues/3777](https://github.com/mockito/mockito/issues/3777)

生成摘要时出错

---

## 19. Unity's Mono problem: Why your C# code runs slower than it should

**原文标题**: Unity's Mono problem: Why your C# code runs slower than it should

**原文链接**: [https://marekfiser.com/blog/mono-vs-dot-net-in-unity/](https://marekfiser.com/blog/mono-vs-dot-net-in-unity/)

生成摘要时出错

---

## 20. MongoBleed Explained Simply

**原文标题**: MongoBleed Explained Simply

**原文链接**: [https://bigdata.2minutestreaming.com/p/mongobleed-explained-simply](https://bigdata.2minutestreaming.com/p/mongobleed-explained-simply)

生成摘要时出错

---

## 21. CEOs are hugely expensive. Why not automate them? (2021)

**原文标题**: CEOs are hugely expensive. Why not automate them? (2021)

**原文链接**: [https://www.newstatesman.com/business/companies/2023/05/ceos-salaries-expensive-automate-robots](https://www.newstatesman.com/business/companies/2023/05/ceos-salaries-expensive-automate-robots)

生成摘要时出错

---

## 22. Show HN: Vibe coding a bookshelf with Claude Code

**原文标题**: Show HN: Vibe coding a bookshelf with Claude Code

**原文链接**: [https://balajmarius.com/writings/vibe-coding-a-bookshelf-with-claude-code/](https://balajmarius.com/writings/vibe-coding-a-bookshelf-with-claude-code/)

生成摘要时出错

---

## 23. Staying ahead of censors in 2025

**原文标题**: Staying ahead of censors in 2025

**原文链接**: [https://forum.torproject.org/t/staying-ahead-of-censors-in-2025-what-weve-learned-from-fighting-censorship-in-iran-and-russia/20898](https://forum.torproject.org/t/staying-ahead-of-censors-in-2025-what-weve-learned-from-fighting-censorship-in-iran-and-russia/20898)

生成摘要时出错

---

## 24. PySDR: A Guide to SDR and DSP Using Python

**原文标题**: PySDR: A Guide to SDR and DSP Using Python

**原文链接**: [https://pysdr.org/content/intro.html](https://pysdr.org/content/intro.html)

生成摘要时出错

---

## 25. Toll roads are spreading in America

**原文标题**: Toll roads are spreading in America

**原文链接**: [https://www.economist.com/united-states/2025/12/18/toll-roads-are-spreading-in-america](https://www.economist.com/united-states/2025/12/18/toll-roads-are-spreading-in-america)

生成摘要时出错

---

## 26. Tesla's 4680 battery supply chain collapses as partner writes down deal by 99%

**原文标题**: Tesla's 4680 battery supply chain collapses as partner writes down deal by 99%

**原文链接**: [https://electrek.co/2025/12/29/tesla-4680-battery-supply-chain-collapses-partner-writes-down-dea/](https://electrek.co/2025/12/29/tesla-4680-battery-supply-chain-collapses-partner-writes-down-dea/)

生成摘要时出错

---

## 27. Researchers discover molecular difference in autistic brains

**原文标题**: Researchers discover molecular difference in autistic brains

**原文链接**: [https://medicine.yale.edu/news-article/molecular-difference-in-autistic-brains/](https://medicine.yale.edu/news-article/molecular-difference-in-autistic-brains/)

生成摘要时出错

---

## 28. Rich Hickey: Thanks AI

**原文标题**: Rich Hickey: Thanks AI

**原文链接**: [https://gist.github.com/richhickey/ea94e3741ff0a4e3af55b9fe6287887f](https://gist.github.com/richhickey/ea94e3741ff0a4e3af55b9fe6287887f)

生成摘要时出错

---

## 29. Show HN: My not-for-profit search engine with no ads, no AI, & all DDG bangs

**原文标题**: Show HN: My not-for-profit search engine with no ads, no AI, & all DDG bangs

**原文链接**: [https://nilch.org](https://nilch.org)

生成摘要时出错

---

## 30. Huge Binaries

**原文标题**: Huge Binaries

**原文链接**: [https://fzakaria.com/2025/12/28/huge-binaries](https://fzakaria.com/2025/12/28/huge-binaries)

生成摘要时出错

---

## 31. No, it's not a battleship

**原文标题**: No, it's not a battleship

**原文链接**: [https://www.navalgazing.net/No-its-not](https://www.navalgazing.net/No-its-not)

生成摘要时出错

---

## 32. Hungry Fat Cells Could Someday Starve Cancer

**原文标题**: Hungry Fat Cells Could Someday Starve Cancer

**原文链接**: [https://www.ucsf.edu/news/2025/01/429411/how-hungry-fat-cells-could-someday-starve-cancer-death](https://www.ucsf.edu/news/2025/01/429411/how-hungry-fat-cells-could-someday-starve-cancer-death)

生成摘要时出错

---

## 33. You can't design software you don't work on

**原文标题**: You can't design software you don't work on

**原文链接**: [https://www.seangoedecke.com/you-cant-design-software-you-dont-work-on/](https://www.seangoedecke.com/you-cant-design-software-you-dont-work-on/)

生成摘要时出错

---

## 34. AI Slop Report: The Global Rise of Low-Quality AI Videos

**原文标题**: AI Slop Report: The Global Rise of Low-Quality AI Videos

**原文链接**: [https://www.kapwing.com/blog/ai-slop-report-the-global-rise-of-low-quality-ai-videos/](https://www.kapwing.com/blog/ai-slop-report-the-global-rise-of-low-quality-ai-videos/)

生成摘要时出错

---

## 35. Richard Stallman at the First Hackers Conference in 1984 [video]

**原文标题**: Richard Stallman at the First Hackers Conference in 1984 [video]

**原文链接**: [https://www.youtube.com/watch?v=Hf2pfzzWPYE](https://www.youtube.com/watch?v=Hf2pfzzWPYE)

生成摘要时出错

---

## 36. Functional programming and reliability: ADTs, safety, critical infrastructure

**原文标题**: Functional programming and reliability: ADTs, safety, critical infrastructure

**原文链接**: [https://blog.rastrian.dev/post/why-reliability-demands-functional-programming-adts-safety-and-critical-infrastructure](https://blog.rastrian.dev/post/why-reliability-demands-functional-programming-adts-safety-and-critical-infrastructure)

生成摘要时出错

---

## 37. Liberating Bluetooth on the ESP32

**原文标题**: Liberating Bluetooth on the ESP32

**原文链接**: [https://exquisite.tube/w/mEzF442Q4hUXnhQ8HmfZuq](https://exquisite.tube/w/mEzF442Q4hUXnhQ8HmfZuq)

生成摘要时出错

---

## 38. UK accounting body to halt remote exams amid AI cheating

**原文标题**: UK accounting body to halt remote exams amid AI cheating

**原文链接**: [https://www.theguardian.com/business/2025/dec/29/uk-accounting-remote-exams-ai-cheating-acca](https://www.theguardian.com/business/2025/dec/29/uk-accounting-remote-exams-ai-cheating-acca)

生成摘要时出错

---

## 39. Panoramas of Star Trek Sets

**原文标题**: Panoramas of Star Trek Sets

**原文链接**: [https://mijofr.github.io/st-panorama/](https://mijofr.github.io/st-panorama/)

生成摘要时出错

---

## 40. Libgodc: Write Go Programs for Sega Dreamcast

**原文标题**: Libgodc: Write Go Programs for Sega Dreamcast

**原文链接**: [https://github.com/drpaneas/libgodc](https://github.com/drpaneas/libgodc)

生成摘要时出错

---

## 41. My First Meshtastic Network

**原文标题**: My First Meshtastic Network

**原文链接**: [https://rickcarlino.com/notes/electronics/my-first-meshtastic-network.html](https://rickcarlino.com/notes/electronics/my-first-meshtastic-network.html)

生成摘要时出错

---

## 42. Feynman's Hughes Lectures: 950 pages of notes

**原文标题**: Feynman's Hughes Lectures: 950 pages of notes

**原文链接**: [https://thehugheslectures.info/the-lectures/](https://thehugheslectures.info/the-lectures/)

生成摘要时出错

---

## 43. 62 years in the making: NYC's newest water tunnel nears the finish line

**原文标题**: 62 years in the making: NYC's newest water tunnel nears the finish line

**原文链接**: [https://ny1.com/nyc/all-boroughs/news/2025/11/09/water--dep--tunnels-](https://ny1.com/nyc/all-boroughs/news/2025/11/09/water--dep--tunnels-)

生成摘要时出错

---

## 44. C++ says “We have try... finally at home”

**原文标题**: C++ says “We have try... finally at home”

**原文链接**: [https://devblogs.microsoft.com/oldnewthing/20251222-00/?p=111890](https://devblogs.microsoft.com/oldnewthing/20251222-00/?p=111890)

生成摘要时出错

---

## 45. EU to build no-fee payments service like Visa/Mastercard and Apple/Google Pay

**原文标题**: EU to build no-fee payments service like Visa/Mastercard and Apple/Google Pay

**原文链接**: [https://www.independent.ie/business/digital-euro-what-it-is-and-how-we-will-use-the-new-form-of-cash/a165973061.html](https://www.independent.ie/business/digital-euro-what-it-is-and-how-we-will-use-the-new-form-of-cash/a165973061.html)

生成摘要时出错

---

## 46. Dolphin Progress Report: Release 2512

**原文标题**: Dolphin Progress Report: Release 2512

**原文链接**: [https://dolphin-emu.org/blog/2025/12/22/dolphin-progress-report-release-2512/](https://dolphin-emu.org/blog/2025/12/22/dolphin-progress-report-release-2512/)

生成摘要时出错

---

## 47. Spherical Cow

**原文标题**: Spherical Cow

**原文链接**: [https://lib.rs/crates/spherical-cow](https://lib.rs/crates/spherical-cow)

生成摘要时出错

---

## 48. Scientists edited genes in a living person and saved his life

**原文标题**: Scientists edited genes in a living person and saved his life

**原文链接**: [https://www.popularmechanics.com/science/health/a64815804/crispr-therapy/](https://www.popularmechanics.com/science/health/a64815804/crispr-therapy/)

生成摘要时出错

---

## 49. Public Domain Day 2026

**原文标题**: Public Domain Day 2026

**原文链接**: [https://web.law.duke.edu/cspd/publicdomainday/2026/](https://web.law.duke.edu/cspd/publicdomainday/2026/)

生成摘要时出错

---

## 50. My app just won best iOS Japanese learning tool of 2025 award (blog)

**原文标题**: My app just won best iOS Japanese learning tool of 2025 award (blog)

**原文链接**: [https://skerritt.blog/best-japanese-learning-tools-2025-award-show/](https://skerritt.blog/best-japanese-learning-tools-2025-award-show/)

生成摘要时出错

---

## 51. Pfizer ended up passing on my GLP-1 work back in the early '90s (2024)

**原文标题**: Pfizer ended up passing on my GLP-1 work back in the early '90s (2024)

**原文链接**: [https://www.statnews.com/2024/09/09/glp-1-history-pfizer-john-baxter-jeffrey-flier-calbio-metabio/](https://www.statnews.com/2024/09/09/glp-1-history-pfizer-john-baxter-jeffrey-flier-calbio-metabio/)

生成摘要时出错

---

## 52. Swapping SIM cards used to be easy, and then came eSIM

**原文标题**: Swapping SIM cards used to be easy, and then came eSIM

**原文链接**: [https://arstechnica.com/gadgets/2025/12/i-switched-to-esim-in-2025-and-i-am-full-of-regret/](https://arstechnica.com/gadgets/2025/12/i-switched-to-esim-in-2025-and-i-am-full-of-regret/)

生成摘要时出错

---

## 53. Dialtone – AOL 3.0 Server

**原文标题**: Dialtone – AOL 3.0 Server

**原文链接**: [https://dialtone.live/](https://dialtone.live/)

生成摘要时出错

---

## 54. Why I Disappeared – My week with minimal internet in a remote island chain

**原文标题**: Why I Disappeared – My week with minimal internet in a remote island chain

**原文链接**: [https://www.kenklippenstein.com/p/why-i-disappeared](https://www.kenklippenstein.com/p/why-i-disappeared)

生成摘要时出错

---

## 55. Linux DAW: Help Linux musicians to quickly and easily find the tools they need

**原文标题**: Linux DAW: Help Linux musicians to quickly and easily find the tools they need

**原文链接**: [https://linuxdaw.org/](https://linuxdaw.org/)

生成摘要时出错

---

## 56. An ounce of silver is now worth more than a barrel of oil

**原文标题**: An ounce of silver is now worth more than a barrel of oil

**原文链接**: [https://www.wsj.com/finance/commodities-futures/an-ounce-of-silver-is-now-worth-more-than-a-barrel-of-oil-196e149e](https://www.wsj.com/finance/commodities-futures/an-ounce-of-silver-is-now-worth-more-than-a-barrel-of-oil-196e149e)

生成摘要时出错

---

## 57. Self-hosting is being enshittified

**原文标题**: Self-hosting is being enshittified

**原文链接**: [https://troubled.engineer/posts/selfhosting-in-2025/](https://troubled.engineer/posts/selfhosting-in-2025/)

生成摘要时出错

---

## 58. Static Allocation with Zig

**原文标题**: Static Allocation with Zig

**原文链接**: [https://nickmonad.blog/2025/static-allocation-with-zig-kv/](https://nickmonad.blog/2025/static-allocation-with-zig-kv/)

生成摘要时出错

---

## 59. Asking Gemini 3 to generate Brainfuck code results in an infinite loop

**原文标题**: Asking Gemini 3 to generate Brainfuck code results in an infinite loop

**原文链接**: [https://teodordyakov.github.io/brainfuck-agi/](https://teodordyakov.github.io/brainfuck-agi/)

生成摘要时出错

---

## 60. Global Memory Shortage Crisis: Market Analysis

**原文标题**: Global Memory Shortage Crisis: Market Analysis

**原文链接**: [https://www.idc.com/resource-center/blog/global-memory-shortage-crisis-market-analysis-and-the-potential-impact-on-the-smartphone-and-pc-markets-in-2026/](https://www.idc.com/resource-center/blog/global-memory-shortage-crisis-market-analysis-and-the-potential-impact-on-the-smartphone-and-pc-markets-in-2026/)

生成摘要时出错

---

## 61. The Dangers of SSL Certificates

**原文标题**: The Dangers of SSL Certificates

**原文链接**: [https://surfingcomplexity.blog/2025/12/27/the-dangers-of-ssl-certificates/](https://surfingcomplexity.blog/2025/12/27/the-dangers-of-ssl-certificates/)

生成摘要时出错

---

## 62. Remembering Lou Gerstner

**原文标题**: Remembering Lou Gerstner

**原文链接**: [https://newsroom.ibm.com/2025-12-28-Remembering-Lou-Gerstner](https://newsroom.ibm.com/2025-12-28-Remembering-Lou-Gerstner)

生成摘要时出错

---

## 63. How We Found Out About COINTELPRO (2014)

**原文标题**: How We Found Out About COINTELPRO (2014)

**原文链接**: [https://monthlyreview.org/articles/how-we-found-out-about-cointelpro/](https://monthlyreview.org/articles/how-we-found-out-about-cointelpro/)

生成摘要时出错

---

## 64. 2 in 3 Americans think AI will cause major harm to humans in the next 20 years [pdf] (2024)

**原文标题**: 2 in 3 Americans think AI will cause major harm to humans in the next 20 years [pdf] (2024)

**原文链接**: [https://www.pewresearch.org/wp-content/uploads/sites/20/2025/03/pi_2025.04.03_us-public-and-ai-experts_topline.pdf](https://www.pewresearch.org/wp-content/uploads/sites/20/2025/03/pi_2025.04.03_us-public-and-ai-experts_topline.pdf)

生成摘要时出错

---

## 65. Private equity is killing private ownership: first it was housing, now it's PCs

**原文标题**: Private equity is killing private ownership: first it was housing, now it's PCs

**原文链接**: [https://old.reddit.com/r/pcmasterrace/comments/1px9xwx/private_equity_is_killing_private_ownership_first/](https://old.reddit.com/r/pcmasterrace/comments/1px9xwx/private_equity_is_killing_private_ownership_first/)

生成摘要时出错

---

## 66. Show HN: See what readers who loved your favorite book/author also loved to read

**原文标题**: Show HN: See what readers who loved your favorite book/author also loved to read

**原文链接**: [https://shepherd.com/bboy/2025](https://shepherd.com/bboy/2025)

生成摘要时出错

---

## 67. John Simpson: 'I've reported on 40 wars but I've never seen a year like 2025'

**原文标题**: John Simpson: 'I've reported on 40 wars but I've never seen a year like 2025'

**原文链接**: [https://www.bbc.com/news/articles/cj4qp17e1lqo](https://www.bbc.com/news/articles/cj4qp17e1lqo)

生成摘要时出错

---

## 68. Nvidia takes $5B stake in Intel under September agreement

**原文标题**: Nvidia takes $5B stake in Intel under September agreement

**原文链接**: [https://www.reuters.com/legal/transactional/nvidia-takes-5-billion-stake-intel-under-september-agreement-2025-12-29/](https://www.reuters.com/legal/transactional/nvidia-takes-5-billion-stake-intel-under-september-agreement-2025-12-29/)

生成摘要时出错

---

## 69. Fast GPU Interconnect over Radio

**原文标题**: Fast GPU Interconnect over Radio

**原文链接**: [https://spectrum.ieee.org/rf-over-fiber](https://spectrum.ieee.org/rf-over-fiber)

生成摘要时出错

---

## 70. Loss of moist broadleaf forest in Africa has turned a carbon sink into source

**原文标题**: Loss of moist broadleaf forest in Africa has turned a carbon sink into source

**原文链接**: [https://www.nature.com/articles/s41598-025-27462-3](https://www.nature.com/articles/s41598-025-27462-3)

生成摘要时出错

---

## 71. How to complain (2024)

**原文标题**: How to complain (2024)

**原文链接**: [https://outerproduct.net/trivial/2024-03-25_complain.html](https://outerproduct.net/trivial/2024-03-25_complain.html)

生成摘要时出错

---

## 72. Slaughtering Competition Problems with Quantifier Elimination (2021)

**原文标题**: Slaughtering Competition Problems with Quantifier Elimination (2021)

**原文链接**: [https://grossack.site/2021/12/22/qe-competition.html](https://grossack.site/2021/12/22/qe-competition.html)

生成摘要时出错

---

## 73. Delete LinkedIn – you'll have zero fucking regrets (2021)

**原文标题**: Delete LinkedIn – you'll have zero fucking regrets (2021)

**原文链接**: [https://thenextweb.com/news/delete-linkedin-youll-have-zero-regrets-syndication](https://thenextweb.com/news/delete-linkedin-youll-have-zero-regrets-syndication)

生成摘要时出错

---

## 74. CIA Star Gate Project: An Overview (1993) [pdf]

**原文标题**: CIA Star Gate Project: An Overview (1993) [pdf]

**原文链接**: [https://www.cia.gov/readingroom/docs/CIA-RDP96-00789R002800180001-2.pdf](https://www.cia.gov/readingroom/docs/CIA-RDP96-00789R002800180001-2.pdf)

生成摘要时出错

---

## 75. Kubernetes egress control with squid proxy

**原文标题**: Kubernetes egress control with squid proxy

**原文链接**: [https://interlaye.red/kubernetes_002degress_002dsquid.html](https://interlaye.red/kubernetes_002degress_002dsquid.html)

生成摘要时出错

---

## 76. Why I think Valve’s retiring the Steam Deck LCD

**原文标题**: Why I think Valve’s retiring the Steam Deck LCD

**原文链接**: [https://gardinerbryant.com/why-valves-retiring-the-steam-deck-lcd/](https://gardinerbryant.com/why-valves-retiring-the-steam-deck-lcd/)

生成摘要时出错

---

## 77. List of domains censored by German ISPs

**原文标题**: List of domains censored by German ISPs

**原文链接**: [https://cuiiliste.de/domains](https://cuiiliste.de/domains)

生成摘要时出错

---

## 78. Show HN: Pion SCTP with RACK is 70% faster with 30% less latency

**原文标题**: Show HN: Pion SCTP with RACK is 70% faster with 30% less latency

**原文链接**: [https://pion.ly/blog/sctp-and-rack/](https://pion.ly/blog/sctp-and-rack/)

生成摘要时出错

---

## 79. Yanis Varoufakis on the future of capitalism [video]

**原文标题**: Yanis Varoufakis on the future of capitalism [video]

**原文链接**: [https://www.youtube.com/watch?v=P_TMuVQPfxw](https://www.youtube.com/watch?v=P_TMuVQPfxw)

生成摘要时出错

---

## 80. Designing Predictable LLM-Verifier Systems for Formal Method Guarantee

**原文标题**: Designing Predictable LLM-Verifier Systems for Formal Method Guarantee

**原文链接**: [https://arxiv.org/abs/2512.02080](https://arxiv.org/abs/2512.02080)

生成摘要时出错

---

## 81. Bankruptcies are exploding across the economy

**原文标题**: Bankruptcies are exploding across the economy

**原文链接**: [https://www.businessinsider.com/bankruptcies-across-economy-small-business-households-corporate-2025-12](https://www.businessinsider.com/bankruptcies-across-economy-small-business-households-corporate-2025-12)

生成摘要时出错

---

## 82. In 1995, a Netscape employee wrote a hack in 10 days that now runs the Internet

**原文标题**: In 1995, a Netscape employee wrote a hack in 10 days that now runs the Internet

**原文链接**: [https://arstechnica.com/gadgets/2025/12/in-1995-a-netscape-employee-wrote-a-hack-in-10-days-that-now-runs-the-internet/](https://arstechnica.com/gadgets/2025/12/in-1995-a-netscape-employee-wrote-a-hack-in-10-days-that-now-runs-the-internet/)

生成摘要时出错

---

## 83. Keep the Robots Out of the Gym

**原文标题**: Keep the Robots Out of the Gym

**原文链接**: [https://danielmiessler.com/blog/keep-the-robots-out-of-the-gym](https://danielmiessler.com/blog/keep-the-robots-out-of-the-gym)

生成摘要时出错

---

## 84. 临终忠告/遗憾

**原文标题**: Deathbed Advice/Regret

**原文链接**: [https://hazn.com/deathbed-regret](https://hazn.com/deathbed-regret)

生成摘要时出错

---

## 85. Ubuntu 26.04 LTS – The Roadmap

**原文标题**: Ubuntu 26.04 LTS – The Roadmap

**原文链接**: [https://discourse.ubuntu.com/t/ubuntu-26-04-lts-the-roadmap/72740](https://discourse.ubuntu.com/t/ubuntu-26-04-lts-the-roadmap/72740)

生成摘要时出错

---

## 86. America's richest 10% now hold 60% of the nation's wealth

**原文标题**: America's richest 10% now hold 60% of the nation's wealth

**原文链接**: [https://bsky.app/profile/rbreich.bsky.social/post/3mayikzgatu2v](https://bsky.app/profile/rbreich.bsky.social/post/3mayikzgatu2v)

生成摘要时出错

---

## 87. LLMs Are Not Fun

**原文标题**: LLMs Are Not Fun

**原文链接**: [https://orib.dev/nofun.html](https://orib.dev/nofun.html)

生成摘要时出错

---

## 88. Salesforce pulls back from LLMs, pivots Agentforce to deterministic automation

**原文标题**: Salesforce pulls back from LLMs, pivots Agentforce to deterministic automation

**原文链接**: [https://timesofindia.indiatimes.com/technology/tech-news/after-laying-off-4000-employees-and-automating-with-ai-agents-salesforce-executives-admit-we-were-more-confident-about-/articleshow/126121875.cms](https://timesofindia.indiatimes.com/technology/tech-news/after-laying-off-4000-employees-and-automating-with-ai-agents-salesforce-executives-admit-we-were-more-confident-about-/articleshow/126121875.cms)

生成摘要时出错

---

## 89. Fast CVVDP implementation in C

**原文标题**: Fast CVVDP implementation in C

**原文链接**: [https://github.com/halidecx/fcvvdp](https://github.com/halidecx/fcvvdp)

生成摘要时出错

---

## 90. If you care about security you might want to move the iPhone Camera app

**原文标题**: If you care about security you might want to move the iPhone Camera app

**原文链接**: [https://blog.jgc.org/2025/12/if-you-care-about-security-you-might.html](https://blog.jgc.org/2025/12/if-you-care-about-security-you-might.html)

生成摘要时出错

---

## 91. Hacker News Made of Primes

**原文标题**: Hacker News Made of Primes

**原文链接**: [https://dosaygo-studio.github.io/prime-news/index.html](https://dosaygo-studio.github.io/prime-news/index.html)

生成摘要时出错

---

## 92. Rust errors without dependencies

**原文标题**: Rust errors without dependencies

**原文链接**: [https://vincents.dev/blog/rust-errors-without-dependencies/](https://vincents.dev/blog/rust-errors-without-dependencies/)

生成摘要时出错

---

## 93. 'Off switch' discovery could help clear our brains of a common parasite

**原文标题**: 'Off switch' discovery could help clear our brains of a common parasite

**原文链接**: [https://www.sciencealert.com/off-switch-discovery-could-help-clear-our-brains-of-a-common-parasite](https://www.sciencealert.com/off-switch-discovery-could-help-clear-our-brains-of-a-common-parasite)

生成摘要时出错

---

## 94. The Prison of Financial Mediocrity

**原文标题**: The Prison of Financial Mediocrity

**原文链接**: [https://twitter.com/systematicls/status/2004900241745883205](https://twitter.com/systematicls/status/2004900241745883205)

生成摘要时出错

---

## 95. 7- and 14-segment fonts "DSEG"

**原文标题**: 7- and 14-segment fonts "DSEG"

**原文链接**: [https://www.keshikan.net/fonts.html](https://www.keshikan.net/fonts.html)

生成摘要时出错

---

## 96. KDE – Highlights from 2025

**原文标题**: KDE – Highlights from 2025

**原文链接**: [https://pointieststick.com/2025/12/28/highlights-from-2025/](https://pointieststick.com/2025/12/28/highlights-from-2025/)

生成摘要时出错

---

## 97. Legal sports betting linked to sharp increases in violent crime

**原文标题**: Legal sports betting linked to sharp increases in violent crime

**原文链接**: [https://news.rice.edu/news/2025/legal-sports-betting-linked-sharp-increases-violent-crime-study-finds](https://news.rice.edu/news/2025/legal-sports-betting-linked-sharp-increases-violent-crime-study-finds)

生成摘要时出错

---

## 98. Scientists discover beer bottle in the Mariana Trench (2024)

**原文标题**: Scientists discover beer bottle in the Mariana Trench (2024)

**原文链接**: [https://www.unilad.com/news/scientist-beer-bottle-deepest-point-ocean-mariana-trench-667878-20240213](https://www.unilad.com/news/scientist-beer-bottle-deepest-point-ocean-mariana-trench-667878-20240213)

生成摘要时出错

---

## 99. 'PromptQuest' is the worst game of 2025 (trying to make chatbots work)

**原文标题**: 'PromptQuest' is the worst game of 2025 (trying to make chatbots work)

**原文链接**: [https://www.theregister.com/2025/12/26/ai_is_like_adventure_games/](https://www.theregister.com/2025/12/26/ai_is_like_adventure_games/)

生成摘要时出错

---

## 100. Five Years of Tinygrad

**原文标题**: Five Years of Tinygrad

**原文链接**: [https://geohot.github.io//blog/jekyll/update/2025/12/29/five-years-of-tinygrad.html](https://geohot.github.io//blog/jekyll/update/2025/12/29/five-years-of-tinygrad.html)

生成摘要时出错

---

