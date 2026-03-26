# Hacker News 热门文章摘要 (2026-03-26)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 量化：自下而上

**原文标题**: Quantization from the Ground Up

**原文链接**: [https://ngrok.com/blog/quantization](https://ngrok.com/blog/quantization)

ngrok 的文章《从零开始的量化》对量化，特别是在深度学习模型背景下的量化，提供了易于理解的介绍。它解释了量化是一种降低模型中数字精度的技术，通常将 32 位浮点数 (FP32) 转换为较低位数的整数（例如，8 位整数，INT8）。

量化的核心动机是为了实现显著的优势：降低内存占用、提高推理速度和降低功耗。这些优势对于在资源受限的设备（如手机或嵌入式系统）上部署大型模型至关重要。

文章通过引入“缩放因子”和“零点”等概念详细介绍了该过程。对于给定的 FP32 值范围，缩放因子将此范围映射到所需的整数范围（例如，对于 INT8，范围是 -128 到 127）。零点用于处理任何偏移，确保浮点零正确映射到整数。讨论的两种主要类型是对称量化（其中 FP32 范围以零为中心，使零点为 0）和非对称量化（处理不以零为中心的范围）。

文章进一步解释了这种转换不仅应用于权重和偏置，还应用于激活值，后者由于其动态范围而更复杂。文章最后强调了权衡取舍：尽管量化提供了效率，但它可能导致模型精度略有下降，这需要仔细的校准和验证。

---

## 2. FreeCAD 1.1

**原文标题**: FreeCAD  v1.1

**原文链接**: [https://blog.freecad.org/2026/03/25/freecad-version-1-1-released/](https://blog.freecad.org/2026/03/25/freecad-version-1-1-released/)

Unable to access the article link.

---

## 3. Landmark L.A. jury verdict finds Instagram, YouTube were designed to addict kids

**原文标题**: Landmark L.A. jury verdict finds Instagram, YouTube were designed to addict kids

**原文链接**: [https://www.latimes.com/california/story/2026-03-25/social-media-lawsuit-trial-meta-google-verdict](https://www.latimes.com/california/story/2026-03-25/social-media-lawsuit-trial-meta-google-verdict)

生成摘要时出错

---

## 4. Swift 6.3

**原文标题**: Swift 6.3

**原文链接**: [https://www.swift.org/blog/swift-6.3-released/](https://www.swift.org/blog/swift-6.3-released/)

Swift 6.3 已发布，旨在使该语言在整个软件栈中更易于访问，提升开发者体验，并拓展到新领域。

关键语言改进包括用于灵活C语言互操作性的`@c`属性，它允许Swift函数和枚举暴露给C代码，并使Swift能够实现C声明。模块名选择器（例如`ModuleA::getValue()`）提供API消歧功能，而`@specialize`、`@inline(always)`和`@export(implementation)`等新属性则为库作者提供了对编译器优化更细粒度的控制。

在构建和包管理方面，Swift Build 集成到 Swift Package Manager 中的预览版已推出，旨在提供统一的跨平台构建体验。SPM（Swift Package Manager）也获得了改进，例如为共享宏库提供预构建的Swift Syntax，以及可发现的包特性。

核心库更新包括对Swift Testing的增强，涵盖警告问题、测试取消和图像附件。DocC 引入了实验性功能，例如Markdown输出、用于提高可发现性的每页静态HTML，以及高级代码块注解（例如`highlight`、`showLineNumbers`）。

显著的平台进展包括对Embedded Swift的广泛改进，增强了C语言互操作性、调试和链接。最值得注意的是，Swift 6.3 发布了首个官方Swift Android SDK，支持使用Swift进行原生Android开发，并将Swift代码无缝集成到现有的Kotlin/Java应用程序中。

本次发布是社区贡献的成果，特别是Android工作组的贡献。鼓励用户通过提供的工具链尝试Swift 6.3。

---

## 5. 为什么这么多控制室是海沫绿的 (2025)

**原文标题**: Why so many control rooms were seafoam green (2025)

**原文链接**: [https://bethmathews.substack.com/p/why-so-many-control-rooms-were-seafoam](https://bethmathews.substack.com/p/why-so-many-control-rooms-were-seafoam)

以下是文章《许多控制室为何采用海沫绿 (2025)》的简明摘要：

该文章探讨了20世纪中期控制室中海沫绿（特指一种名为“绿雾”的颜色，孟塞尔7.5G 6/4）的盛行，并将其归因于一种专注于人因和“人机工程学”的设计理念。

这种颜色选择源于二战期间军方进行的研究，特别是人因工程学先驱阿尔方斯·查帕尼斯，旨在提高雷达操作员的效率和舒适度。该研究旨在识别能够减少视觉疲劳和眩光，并能作为发光显示器和设备中性背景的颜色。经过测试各种颜色，发现绿雾具有最佳反射率（约30-35%），从而提供了一个舒适的视觉环境，而不会引起眼睛疲劳或分散注意力。

这些军事研究的结果随后被亨利·德雷福斯和沃尔特·多温·蒂格等工业设计师和顾问采纳，他们在为贝尔实验室等公司工作时，改进了发电厂、飞行控制中心和化工厂等民用控制室的设计。他们将这些原则转化为行业标准，使海沫绿成为操作员需要长时间保持专注的环境中一种普遍且有科学依据的选择。这种颜色不仅仅是为了美观；它是一个旨在提高操作员表现和福祉的深思熟虑的人机工程学决策。

---

## 6. 陪审团裁定Meta为牟利蓄意伤害儿童，作出里程碑式判决。

**原文标题**: Jury says Meta knowingly harmed children for profit, awarding landmark verdict

**原文链接**: [https://www.latimes.com/business/story/2026-03-25/jury-says-meta-knowingly-harmed-children-for-profit-awarding-landmark-verdict](https://www.latimes.com/business/story/2026-03-25/jury-says-meta-knowingly-harmed-children-for-profit-awarding-landmark-verdict)

生成摘要时出错

---

## 7. 崔西·基德去世了

**原文标题**: Tracy Kidder has died

**原文链接**: [https://www.nytimes.com/2026/03/25/books/tracy-kidder-dead.html](https://www.nytimes.com/2026/03/25/books/tracy-kidder-dead.html)

无法访问文章链接。

---

## 8. 我为何分叉 httpx

**原文标题**: Why I forked httpx

**原文链接**: [https://tildeweb.nl/~michiel/httpxyz.html](https://tildeweb.nl/~michiel/httpxyz.html)

The author has forked `httpx`, a popular Python HTTP client, creating a new project called `httpxyz`. The decision stems from several issues with `httpx`'s maintenance and direction.

Key reasons for the fork include:
1.  **Unaddressed Bugs and Stalled Releases:** A fix for a broken zstd content decoding contribution, merged in 2024, was ignored, and no new release containing it has been made since November 2024. The latest patch release has been in draft for over a year.
2.  **Community Engagement Issues:** Issues have been hidden and discussions turned off on the `httpx` GitHub repository, hindering contributions and user support.
3.  **Uncertain 1.0 Future:** The 1.0 release has been in planning for years and is expected to be significantly different and potentially breaking, leading major users like OpenAI and Anthropic to guard against it. The author previously introduced breaking changes in minor updates, citing pre-1.0 status.
4.  **Recurring Patterns:** Similar maintenance issues, including turning off issues and discussions, have been observed in the author's other high-profile projects like Django REST framework and MkDocs.
5.  **Lack of Maintenance/Collaboration:** The author expresses concern about the lack of maintenance and unwillingness to allow others to help, despite `httpx`'s high profile.

The goal for `httpxyz` is to provide a stable, maintained path, focusing on faster, non-breaking releases without major rewrites. The author, joined by co-maintainer Sander Wegter, aims to prevent burnout. `httpxyz` will be hosted on Codeberg, a non-profit platform, to avoid GitHub monoculture. Users are advised that porting may not be immediately necessary if `httpx` currently works for them, and `niquests` is suggested as another alternative.

---

## 9. 政府机构大量购买美国人的商业数据

**原文标题**: Government agencies buy commercial data about Americans in bulk

**原文链接**: [https://www.npr.org/2026/03/25/nx-s1-5752369/ice-surveillance-data-brokers-congress-anthropic](https://www.npr.org/2026/03/25/nx-s1-5752369/ice-surveillance-data-brokers-congress-anthropic)

U.S. government agencies, including ICE, FBI, and the Department of Defense, are reportedly circumventing Fourth Amendment warrant requirements and a 2015 law banning bulk data collection by purchasing vast quantities of commercial data, such as cell phone location information, from data brokers. This practice allows agencies to track Americans without judicial oversight, revealing intimate details about their lives.

Privacy advocates and a bipartisan coalition in Congress view the upcoming reauthorization of Section 702 of the Foreign Intelligence Surveillance Act (FISA), set to expire on April 20th, as the crucial opportunity to close this "data broker loophole." They argue this warrantless data acquisition constitutes mass surveillance, which is significantly exacerbated by artificial intelligence's capacity to analyze and create comprehensive profiles. FBI Director Kash Patel declined to commit to ceasing the purchase of location data.

Despite calls for reform from lawmakers like Sen. Ron Wyden and Rep. Warren Davidson, and over 130 civil society organizations, the White House and House Speaker Mike Johnson are pushing for a "clean" FISA reauthorization without changes. Advocates warn that without reform, this expanding infrastructure of private sector surveillance, especially when combined with AI, is hurtling society towards a "dystopian surveillance society." They contend that purchasing data to bypass warrants is unconstitutional, drawing parallels to illegal home searches.

---

## 10. Woman who never stopped updating her lost dog's chip reunites with him after 11y

**原文标题**: Woman who never stopped updating her lost dog's chip reunites with him after 11y

**原文链接**: [https://www.cbc.ca/radio/asithappens/11-year-dog-reunion-9.7140780](https://www.cbc.ca/radio/asithappens/11-year-dog-reunion-9.7140780)

生成摘要时出错

---

## 11. Earthquake scientists reveal how overplowing weakens soil at experimental farm

**原文标题**: Earthquake scientists reveal how overplowing weakens soil at experimental farm

**原文链接**: [https://www.washington.edu/news/2026/03/19/earthquake-scientists-reveal-how-overplowing-weakens-soil-at-experimental-farm/](https://www.washington.edu/news/2026/03/19/earthquake-scientists-reveal-how-overplowing-weakens-soil-at-experimental-farm/)

生成摘要时出错

---

## 12. Disney Exits OpenAI Deal After AI Giant Shutters Sora

**原文标题**: Disney Exits OpenAI Deal After AI Giant Shutters Sora

**原文链接**: [https://www.hollywoodreporter.com/business/digital/openai-shutting-down-sora-ai-video-app-1236546187/](https://www.hollywoodreporter.com/business/digital/openai-shutting-down-sora-ai-video-app-1236546187/)

生成摘要时出错

---

## 13. Sodium-ion EV battery breakthrough delivers 11-min charging and 450 km range

**原文标题**: Sodium-ion EV battery breakthrough delivers 11-min charging and 450 km range

**原文链接**: [https://electrek.co/2026/03/25/sodium-ion-ev-battery-delivers-11-min-charging-450-km-range/](https://electrek.co/2026/03/25/sodium-ion-ev-battery-delivers-11-min-charging-450-km-range/)

生成摘要时出错

---

## 14. My minute-by-minute response to the LiteLLM malware attack

**原文标题**: My minute-by-minute response to the LiteLLM malware attack

**原文链接**: [https://futuresearch.ai/blog/litellm-attack-transcript/](https://futuresearch.ai/blog/litellm-attack-transcript/)

生成摘要时出错

---

## 15. LibreOffice and the art of overreacting

**原文标题**: LibreOffice and the art of overreacting

**原文链接**: [https://blog.documentfoundation.org/blog/2026/03/25/libreoffice-and-the-art-of-overreacting/](https://blog.documentfoundation.org/blog/2026/03/25/libreoffice-and-the-art-of-overreacting/)

生成摘要时出错

---

## 16. China is mass-producing hypersonic missiles for $99,000

**原文标题**: China is mass-producing hypersonic missiles for $99,000

**原文链接**: [https://kdwalmsley.substack.com/p/on-sale-now-china-is-mass-producing](https://kdwalmsley.substack.com/p/on-sale-now-china-is-mass-producing)

生成摘要时出错

---

## 17. Obsolete Sounds

**原文标题**: Obsolete Sounds

**原文链接**: [https://citiesandmemory.com/obsolete-sounds/](https://citiesandmemory.com/obsolete-sounds/)

生成摘要时出错

---

## 18. Ball Pit

**原文标题**: Ball Pit

**原文链接**: [https://codepen.io/mrdoob_/full/NPRwLZd](https://codepen.io/mrdoob_/full/NPRwLZd)

The provided URL leads to an interactive 3D web demonstration titled "Ball Pit" by Mr.doob, a well-known developer and creator of the Three.js library. Rather than a traditional article with textual content, the page presents a real-time simulation of a large number of colorful spheres contained within a virtual pit.

The core of the demo is its physics engine, which allows the balls to move, bounce, and collide realistically with each other and the pit's walls. Users can interact with the scene by clicking and dragging their mouse to rotate the camera and view the dynamic interactions from various angles. The simulation showcases impressive performance in rendering and calculating physics for numerous objects simultaneously within a web browser, likely utilizing WebGL and Three.js. It serves as a visual testament to modern web capabilities in 3D graphics and interactive physics simulations.

---

## 19. Newly purchased Vizio TVs now require Walmart accounts to use smart features

**原文标题**: Newly purchased Vizio TVs now require Walmart accounts to use smart features

**原文链接**: [https://arstechnica.com/gadgets/2026/03/newly-purchased-vizio-tvs-now-require-walmart-accounts-to-use-smart-features/](https://arstechnica.com/gadgets/2026/03/newly-purchased-vizio-tvs-now-require-walmart-accounts-to-use-smart-features/)

生成摘要时出错

---

## 20. I tried to prove I'm not AI. My aunt wasn't convinced

**原文标题**: I tried to prove I'm not AI. My aunt wasn't convinced

**原文链接**: [https://www.bbc.com/future/article/20260324-i-tried-to-prove-im-not-an-ai-deepfake](https://www.bbc.com/future/article/20260324-i-tried-to-prove-im-not-an-ai-deepfake)

生成摘要时出错

---

## 21. Regular army and reserve components enlistment program: Summary of change

**原文标题**: Regular army and reserve components enlistment program: Summary of change

**原文链接**: [https://armypubs.army.mil/epubs/DR_pubs/DR_a/ARN42922-AR_601-210-000-WEB-1.pdf](https://armypubs.army.mil/epubs/DR_pubs/DR_a/ARN42922-AR_601-210-000-WEB-1.pdf)

生成摘要时出错

---

## 22. AI users whose lives were wrecked by delusion

**原文标题**: AI users whose lives were wrecked by delusion

**原文链接**: [https://www.theguardian.com/lifeandstyle/2026/mar/26/ai-chatbot-users-lives-wrecked-by-delusion](https://www.theguardian.com/lifeandstyle/2026/mar/26/ai-chatbot-users-lives-wrecked-by-delusion)

生成摘要时出错

---

## 23. Health NZ staff told to stop using ChatGPT to write clinical notes

**原文标题**: Health NZ staff told to stop using ChatGPT to write clinical notes

**原文链接**: [https://www.rnz.co.nz/news/national/590645/health-nz-staff-told-to-stop-using-chatgpt-to-write-clinical-notes](https://www.rnz.co.nz/news/national/590645/health-nz-staff-told-to-stop-using-chatgpt-to-write-clinical-notes)

生成摘要时出错

---

## 24. Interoperability Can Save the Open Web (2023)

**原文标题**: Interoperability Can Save the Open Web (2023)

**原文链接**: [https://spectrum.ieee.org/doctorow-interoperability](https://spectrum.ieee.org/doctorow-interoperability)

生成摘要时出错

---

## 25. Sony V. Cox Decision Reversed

**原文标题**: Sony V. Cox Decision Reversed

**原文链接**: [https://supreme.justia.com/cases/federal/us/607/24-171/](https://supreme.justia.com/cases/federal/us/607/24-171/)

生成摘要时出错

---

## 26. Show HN: A plain-text cognitive architecture for Claude Code

**原文标题**: Show HN: A plain-text cognitive architecture for Claude Code

**原文链接**: [https://lab.puga.com.br/cog/](https://lab.puga.com.br/cog/)

生成摘要时出错

---

## 27. US expected to send thousands more soldiers to Middle East, sources say

**原文标题**: US expected to send thousands more soldiers to Middle East, sources say

**原文链接**: [https://www.reuters.com/world/middle-east/us-expected-send-thousands-soldiers-middle-east-sources-say-2026-03-24/](https://www.reuters.com/world/middle-east/us-expected-send-thousands-soldiers-middle-east-sources-say-2026-03-24/)

生成摘要时出错

---

## 28. A Eulogy for Vim

**原文标题**: A Eulogy for Vim

**原文链接**: [https://drewdevault.com/2026/03/25/2026-03-25-Forking-vim.html](https://drewdevault.com/2026/03/25/2026-03-25-Forking-vim.html)

生成摘要时出错

---

## 29. A Compiler Writing Journey

**原文标题**: A Compiler Writing Journey

**原文链接**: [https://github.com/DoctorWkt/acwj](https://github.com/DoctorWkt/acwj)

生成摘要时出错

---

## 30. Intel Announces Arc Pro B70 and Arc Pro B65 GPUs

**原文标题**: Intel Announces Arc Pro B70 and Arc Pro B65 GPUs

**原文链接**: [https://www.techpowerup.com/347703/intel-announces-arc-pro-b70-and-arc-pro-b65-gpus-maxes-out-xe2-battlemage-architecture](https://www.techpowerup.com/347703/intel-announces-arc-pro-b70-and-arc-pro-b65-gpus-maxes-out-xe2-battlemage-architecture)

生成摘要时出错

---

