# Hacker News 热门文章摘要 (2025-12-18)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 双子座3号 闪电：为速度而生的前沿智能

**原文标题**: Gemini 3 Flash: Frontier intelligence built for speed

**原文链接**: [https://blog.google/products/gemini/gemini-3-flash/](https://blog.google/products/gemini/gemini-3-flash/)

谷歌推出了Gemini 3 Flash，这是Gemini 3系列中最新模型，专为前沿智能设计，具有卓越的速度和成本效益。它在Gemini 3 Pro和Deep Think模式的基础上进行扩展，保留了它们先进的推理、多模态和视觉理解能力，但针对Flash级别的低延迟和更低成本进行了优化。

Gemini 3 Flash表现出色，在博士级别的推理基准测试中与更大型的前沿模型不相上下，并在多模态理解方面取得了最先进的分数。它显著超越了Gemini 2.5 Pro，平均速度快三倍，使用的Token减少30%，而成本仅为其一小部分（输入100万个Token仅需0.50美元）。它在编码任务中也表现出色，在SWE-bench Verified测试中获得了78%的分数。

该模型正在全球范围内推出，可供不同用户使用：
*   **开发者**可以通过Gemini API（Google AI Studio、Antigravity、CLI、Android Studio）、Vertex AI和Gemini Enterprise，利用它进行迭代开发、代理式编码和复杂的多模态分析。
*   **普通用户**会发现它成为Gemini应用程序（取代2.5 Flash）和搜索中AI模式的新默认模型，免费提供增强的推理能力，用于视频分析、实时素描、音频摘要和语音到应用创建等任务。
*   JetBrains和Figma等**企业**已通过Vertex AI和Gemini Enterprise开始采用该模型，认可其效率和速度。

Gemini 3 Flash旨在将下一代智能广泛普及，将深度推理与谷歌产品中的快速、高性价比性能相结合。

---

## 2. AWS首席执行官表示，用AI取代初级开发人员是“最愚蠢的想法之一”。

**原文标题**: AWS CEO says replacing junior devs with AI is 'one of the dumbest ideas'

**原文链接**: [https://www.finalroundai.com/blog/aws-ceo-ai-cannot-replace-junior-developers](https://www.finalroundai.com/blog/aws-ceo-ai-cannot-replace-junior-developers)

亚马逊AWS首席执行官Matt Garman称用AI取代初级开发人员是“最愚蠢的想法之一”，并阐述了三个核心反对理由。

首先，初级开发人员通常最擅长使用AI工具。他们伴随新技术成长，能够迅速适应、探索功能并有效利用AI。Stack Overflow的一项调查证实，55.5%的早期职业开发人员每天使用AI工具，这一比例超过了资深员工，许多人甚至帮助年长的同事提升技能。

其次，初级员工通常是成本最低的员工，因此解雇他们是一种低效的成本削减策略。他们较低的薪资意味着有限的节约空间，而真正的成本优化需要更广泛的全公司范围的方法。一些公司在裁员时期望节省开支，但实际上却发现开支增加了。

第三，解雇初级开发人员会切断关键的人才输送管道。公司需要新鲜人才来带来新想法、推动创新并培养未来的领导者。如果不指导新员工，组织将面临经验丰富人员短缺和内部晋升机会减少的风险，尤其考虑到科技行业劳动力预计的增长。

加曼强调，短期思维将损害长期战略。他承认AI将改变工作角色并提高生产力，但他相信它最终创造的就业机会将多于取代的。开发人员需要适应新技术，专注于更高价值的任务，这凸显了拥有扎实基础技能的新人才持续的重要性。

---

## 3. Mozilla在努力自杀吗？

**原文标题**: Is Mozilla trying hard to kill itself?

**原文链接**: [https://infosec.press/brunomiguel/is-mozilla-trying-hard-to-kill-itself](https://infosec.press/brunomiguel/is-mozilla-trying-hard-to-kill-itself)

文章对Mozilla新任CEO恩佐-德梅奥（Enzor-DeMeo）在“The Verge”采访中发表的言论表达了强烈担忧和失望。据报道，这位CEO提及在Firefox中阻止广告拦截器可以带来1.5亿美元的收入，尽管他表示“不想那样做”，因为它感觉“偏离了使命”。

作者作为一位长期的Firefox用户，将此解读为一种隐晦的威胁，认为为了经济利益移除广告拦截器的选项仍然在考虑之中。他们认为，Firefox对开放标准、开放网络及其强大的附加组件系统（尤其是广告拦截器）的承诺，历史上吸引并留住了其忠实的、注重隐私的用户群。

广告拦截器被强调为相较于Chromium的一个关键优势，以及对抗恶意广告的一个重要安全功能。作者警告说，移除此功能将是有害的，会疏远核心社区——这个群体的技术建议常影响主流用户——并可能对该项目造成严重的负面后果。尽管承认Mozilla对收入的需求，但作者质疑，如果该有争议的“偏离使命”的可能性并未仍在考虑中，CEO为何要公开提出？这导致了负面的公关效果，并增加了Firefox未来的不确定性。

---

## 4. ty Beta 版发布

**原文标题**: Announcing the Beta release of ty

**原文链接**: [https://astral.sh/blog/ty](https://astral.sh/blog/ty)

Astral, creators of uv and Ruff, has announced the Beta release of "ty," an extremely fast Python type checker and language server written in Rust. Designed as an alternative to tools like mypy and Pyright, Astral now uses ty exclusively and recommends it for production use to motivated users.

ty's core focus is performance, consistently being 10x-60x faster than competitors without caching. Its incremental architecture makes live editor updates dramatically faster, recomputing diagnostics in milliseconds (e.g., 4.7ms in PyTorch, 80x faster than Pyright), ensuring a highly responsive development experience.

Beyond speed, ty emphasizes correctness and ergonomics, featuring first-class intersection types, advanced type narrowing, and sophisticated reachability analysis to deliver more accurate feedback and reduce false positives. It boasts a best-in-class diagnostic system, inspired by the Rust compiler, providing detailed, multi-file context to explain issues and suggest fixes.

Built open-source under the MIT license with dozens of contributors, ty supports all standard Language Server Protocol capabilities (Go to Definition, Auto-Complete, etc.) and is installable via `uv tool install ty@latest` or its VS Code extension.

Immediate priorities include stability, completing Python typing specification features, and supporting popular third-party libraries like Pydantic and Django. Longer-term, ty will power semantic capabilities across the Astral toolchain, aiming to enhance Python's productivity. The project acknowledges extensive contributions from its community and collaborators.

---

## 5. 无图形API

**原文标题**: No Graphics API

**原文链接**: [https://www.sebastianaaltonen.com/blog/no-graphics-api](https://www.sebastianaaltonen.com/blog/no-graphics-api)

塞巴斯蒂安·阿尔托宁认为，十年前推出的DirectX 12、Vulkan和Metal等“现代”图形API已变得过于复杂，不再适用于当前的GPU架构。这些API最初是为了抽象10-13年前多样化且通常为固定功能的硬件而开发的，它们要求提前将着色器管线状态捆绑到持久对象中，以减少驱动程序开销。这种方法虽然当时是必要的，却导致了“管线状态对象（PSO）爆炸”，产生了庞大的着色器缓存（100GB以上）和复杂的云服务器基础设施。

文章详细阐述了GPU和API的历史演变，从3dfx Voodoo等早期固定功能显卡到DirectX 11时代，展示了API设计如何始终适应硬件限制，例如专用内存、1:1着色器模型以及带有不透明描述符的各种缓冲区类型。

然而，现代GPU已经发生了显著的转变。它们现在具备统一的缓存层次结构、原生64位指针、无绑定纹理采样器以及能够处理所有着色器类型的通用SIMD设计。这些进步使得许多原始API的折衷方案——例如复杂的描述符管理和持久状态对象——变得过时。阿尔托宁认为，如果从当前通用GPU硬件的基本原理出发，设计一个大幅简化的API，就能消除PSO爆炸，简化GPU交互，并显著减少抽象层。

---

## 6. AI将使形式化验证走向主流

**原文标题**: AI will make formal verification go mainstream

**原文链接**: [https://martin.kleppmann.com/2025/12/08/ai-formal-verification.html](https://martin.kleppmann.com/2025/12/08/ai-formal-verification.html)

Martin Kleppmann 预测，人工智能将使形式化验证（FV）在软件工程中成为主流。目前，FV 是一种小众实践，它涉及使用 Isabelle 或 Lean 等工具，根据形式化规范，通过数学方法证明代码的正确性。由于其极高的难度、劳动密集型（需要博士级别专业知识）和高昂的成本，它很少被业界采用；例如，seL4 微内核的验证耗时 20 个人年，涉及 20 万行代码。从经济角度看，修复错误的成本一直低于形式化验证的成本。

然而，基于大型语言模型（LLM）的编码助手正日益擅长编写证明脚本。尽管目前仍需人工指导，但预计这一过程将实现完全自动化，从而大幅降低 FV 的成本。这将彻底改变经济模式。

此外，人工智能还为 FV 创造了“需求”。人工智能可以证明其自身生成代码的正确性，而无需人工审查。这对 LLM 来说是一个理想的应用场景，因为证明检查器会立即拒绝无效的证明，迫使人工智能迭代直到找到正确的证明。这种精确性抵消了 LLM 的概率特性，使得经过形式化验证的人工智能生成代码变得极具吸引力。

届时，挑战将转向正确定义形式化规范，这仍然需要专业知识，但比手动编写证明要简单得多。人工智能甚至可能有助于在形式语言和自然语言之间进行规范的翻译。更低的验证成本、人工智能生成代码的验证需求以及 FV 的精确性共同作用，意味着形式化验证有望成为标准。主要障碍可能将是文化阻力，而非技术局限。

---

## 7. Beginning January 2026, all ACM publications will be made open access

**原文标题**: Beginning January 2026, all ACM publications will be made open access

**原文链接**: [https://dl.acm.org/openaccess](https://dl.acm.org/openaccess)

Beginning January 2026, the Association for Computing Machinery (ACM) will make all its new publications openly accessible for readers globally, marking a significant shift in scholarly publishing for the computing field. This initiative is the culmination of ACM's "ACM Open" program, which has been transitioning the organization from a subscription-based model to a full open access framework since 2020.

Under the new model, authors will retain copyright to their work, which will be published under a Creative Commons CC-BY 4.0 license, ensuring maximum reuse and impact. Funding for this open access model will primarily be facilitated through institutional "Read and Publish" (transformative) agreements. These agreements allow participating institutions to provide unlimited open access publishing for their affiliated authors and grant their users full read access to the entire ACM Digital Library. For authors not covered by such an institutional agreement, an Article Processing Charge (APC) will apply.

The move aims to significantly enhance the dissemination and impact of computing research, foster greater collaboration across the global research community, and promote equity in access to scholarly knowledge. While the January 2026 date specifically applies to all new publications, ACM's broader, long-term vision is to eventually make all content within the ACM Digital Library openly accessible.

---

## 8. Coursera to combine with Udemy

**原文标题**: Coursera to combine with Udemy

**原文链接**: [https://investor.coursera.com/news/news-details/2025/Coursera-to-Combine-with-Udemy-to-Empower-the-Global-Workforce-with-Skills-for-the-AI-Era/default.aspx](https://investor.coursera.com/news/news-details/2025/Coursera-to-Combine-with-Udemy-to-Empower-the-Global-Workforce-with-Skills-for-the-AI-Era/default.aspx)

生成摘要时出错

---

## 9. I got hacked: My Hetzner server started mining Monero

**原文标题**: I got hacked: My Hetzner server started mining Monero

**原文链接**: [https://blog.jakesaunders.dev/my-server-started-mining-monero-this-morning/](https://blog.jakesaunders.dev/my-server-started-mining-monero-this-morning/)

生成摘要时出错

---

## 10. No AI* Here – A Response to Mozilla's Next Chapter

**原文标题**: No AI* Here – A Response to Mozilla's Next Chapter

**原文链接**: [https://www.waterfox.com/blog/no-ai-here-response-to-mozilla/](https://www.waterfox.com/blog/no-ai-here-response-to-mozilla/)

生成摘要时出错

---

## 11. Gut bacteria from amphibians and reptiles achieve tumor elimination in mice

**原文标题**: Gut bacteria from amphibians and reptiles achieve tumor elimination in mice

**原文链接**: [https://www.jaist.ac.jp/english/whatsnew/press/2025/12/17-1.html](https://www.jaist.ac.jp/english/whatsnew/press/2025/12/17-1.html)

生成摘要时出错

---

## 12. Your job is to deliver code you have proven to work

**原文标题**: Your job is to deliver code you have proven to work

**原文链接**: [https://simonwillison.net/2025/Dec/18/code-proven-to-work/](https://simonwillison.net/2025/Dec/18/code-proven-to-work/)

生成摘要时出错

---

## 13. Classical statues were not painted horribly

**原文标题**: Classical statues were not painted horribly

**原文链接**: [https://worksinprogress.co/issue/were-classical-statues-painted-horribly/](https://worksinprogress.co/issue/were-classical-statues-painted-horribly/)

生成摘要时出错

---

## 14. Are Apple gift cards safe to redeem?

**原文标题**: Are Apple gift cards safe to redeem?

**原文链接**: [https://daringfireball.net/linked/2025/12/17/are-apple-gift-cards-safe-to-redeem](https://daringfireball.net/linked/2025/12/17/are-apple-gift-cards-safe-to-redeem)

生成摘要时出错

---

## 15. Creating apps like Signal could be 'hostile activity' claims UK watchdog

**原文标题**: Creating apps like Signal could be 'hostile activity' claims UK watchdog

**原文链接**: [https://www.techradar.com/vpn/vpn-privacy-security/creating-apps-like-signal-or-whatsapp-could-be-hostile-activity-claims-uk-watchdog](https://www.techradar.com/vpn/vpn-privacy-security/creating-apps-like-signal-or-whatsapp-could-be-hostile-activity-claims-uk-watchdog)

生成摘要时出错

---

## 16. A Safer Container Ecosystem with Docker: Free Docker Hardened Images

**原文标题**: A Safer Container Ecosystem with Docker: Free Docker Hardened Images

**原文链接**: [https://www.docker.com/blog/docker-hardened-images-for-every-developer/](https://www.docker.com/blog/docker-hardened-images-for-every-developer/)

生成摘要时出错

---

## 17. How SQLite is tested

**原文标题**: How SQLite is tested

**原文链接**: [https://sqlite.org/testing.html](https://sqlite.org/testing.html)

生成摘要时出错

---

## 18. After ruining a treasured water resource, Iran is drying up

**原文标题**: After ruining a treasured water resource, Iran is drying up

**原文链接**: [https://e360.yale.edu/features/iran-water-drought-dams-qanats](https://e360.yale.edu/features/iran-water-drought-dams-qanats)

生成摘要时出错

---

## 19. OBS Studio Gets a New Renderer

**原文标题**: OBS Studio Gets a New Renderer

**原文链接**: [https://obsproject.com/blog/obs-studio-gets-a-new-renderer](https://obsproject.com/blog/obs-studio-gets-a-new-renderer)

生成摘要时出错

---

## 20. Please Just Try Htmx

**原文标题**: Please Just Try Htmx

**原文链接**: [http://pleasejusttryhtmx.com/](http://pleasejusttryhtmx.com/)

生成摘要时出错

---

## 21. A16z-backed Doublespeed hacked, revealing what its AI-generated accounts promote

**原文标题**: A16z-backed Doublespeed hacked, revealing what its AI-generated accounts promote

**原文链接**: [https://www.404media.co/hack-reveals-the-a16z-backed-phone-farm-flooding-tiktok-with-ai-influencers/](https://www.404media.co/hack-reveals-the-a16z-backed-phone-farm-flooding-tiktok-with-ai-influencers/)

生成摘要时出错

---

## 22. I ported JustHTML from Python to JavaScript with Codex CLI and GPT-5.2 in hours

**原文标题**: I ported JustHTML from Python to JavaScript with Codex CLI and GPT-5.2 in hours

**原文链接**: [https://simonwillison.net/2025/Dec/15/porting-justhtml/](https://simonwillison.net/2025/Dec/15/porting-justhtml/)

生成摘要时出错

---

## 23. MIT professor shot at his Massachusetts home dies

**原文标题**: MIT professor shot at his Massachusetts home dies

**原文链接**: [https://www.bbc.com/news/articles/cly08y25688o](https://www.bbc.com/news/articles/cly08y25688o)

生成摘要时出错

---

## 24. AI's real superpower: consuming, not creating

**原文标题**: AI's real superpower: consuming, not creating

**原文链接**: [https://msanroman.io/blog/ai-consumption-paradigm](https://msanroman.io/blog/ai-consumption-paradigm)

生成摘要时出错

---

## 25. TikTok unlawfully tracks shopping habits and use of dating apps?

**原文标题**: TikTok unlawfully tracks shopping habits and use of dating apps?

**原文链接**: [https://noyb.eu/en/tiktok-unlawfully-tracks-your-shopping-habits-and-your-use-dating-apps](https://noyb.eu/en/tiktok-unlawfully-tracks-your-shopping-habits-and-your-use-dating-apps)

生成摘要时出错

---

## 26. Slowness is a virtue

**原文标题**: Slowness is a virtue

**原文链接**: [https://blog.jakobschwichtenberg.com/p/slowness-is-a-virtue](https://blog.jakobschwichtenberg.com/p/slowness-is-a-virtue)

生成摘要时出错

---

## 27. How getting richer made teenagers less free

**原文标题**: How getting richer made teenagers less free

**原文链接**: [https://www.theargumentmag.com/p/how-getting-richer-made-teenagers](https://www.theargumentmag.com/p/how-getting-richer-made-teenagers)

生成摘要时出错

---

## 28. Germany: Amazon is not allowed to force customers to watch ads on Prime Video

**原文标题**: Germany: Amazon is not allowed to force customers to watch ads on Prime Video

**原文链接**: [https://www.zeit.de/wirtschaft/2025-12/amazon-urteil-video-kunden-werbung](https://www.zeit.de/wirtschaft/2025-12/amazon-urteil-video-kunden-werbung)

生成摘要时出错

---

## 29. 'Ghost jobs' are on the rise – and so are calls to ban them

**原文标题**: 'Ghost jobs' are on the rise – and so are calls to ban them

**原文链接**: [https://www.bbc.com/news/articles/clyzvpp8g3vo](https://www.bbc.com/news/articles/clyzvpp8g3vo)

生成摘要时出错

---

## 30. Judge hints Vizio TV buyers may have rights to source code licensed under GPL

**原文标题**: Judge hints Vizio TV buyers may have rights to source code licensed under GPL

**原文链接**: [https://www.theregister.com/2025/12/05/vizio_gpl_source_code_ruling/](https://www.theregister.com/2025/12/05/vizio_gpl_source_code_ruling/)

生成摘要时出错

---

## 31. Developers can now submit apps to ChatGPT

**原文标题**: Developers can now submit apps to ChatGPT

**原文链接**: [https://openai.com/index/developers-can-now-submit-apps-to-chatgpt/](https://openai.com/index/developers-can-now-submit-apps-to-chatgpt/)

生成摘要时出错

---

## 32. Vibe coding creates fatigue?

**原文标题**: Vibe coding creates fatigue?

**原文链接**: [https://www.tabulamag.com/p/too-fast-to-think-the-hidden-fatigue](https://www.tabulamag.com/p/too-fast-to-think-the-hidden-fatigue)

生成摘要时出错

---

## 33. Yep, Passkeys Still Have Problems

**原文标题**: Yep, Passkeys Still Have Problems

**原文链接**: [https://fy.blackhats.net.au/blog/2025-12-17-yep-passkeys-still-have-problems/](https://fy.blackhats.net.au/blog/2025-12-17-yep-passkeys-still-have-problems/)

生成摘要时出错

---

## 34. AI helps ship faster but it produces 1.7× more bugs

**原文标题**: AI helps ship faster but it produces 1.7× more bugs

**原文链接**: [https://www.coderabbit.ai/blog/state-of-ai-vs-human-code-generation-report](https://www.coderabbit.ai/blog/state-of-ai-vs-human-code-generation-report)

生成摘要时出错

---

## 35. Pornhub extorted after hackers steal Premium member activity data

**原文标题**: Pornhub extorted after hackers steal Premium member activity data

**原文链接**: [https://www.bleepingcomputer.com/news/security/pornhub-extorted-after-hackers-steal-premium-member-activity-data/](https://www.bleepingcomputer.com/news/security/pornhub-extorted-after-hackers-steal-premium-member-activity-data/)

生成摘要时出错

---

## 36. Tesla reports another Robotaxi crash

**原文标题**: Tesla reports another Robotaxi crash

**原文链接**: [https://electrek.co/2025/12/15/tesla-reports-another-robotaxi-crash-even-with-supervisor/](https://electrek.co/2025/12/15/tesla-reports-another-robotaxi-crash-even-with-supervisor/)

生成摘要时出错

---

## 37. FCC chair suggests agency isn't independent, word cut from mission statement

**原文标题**: FCC chair suggests agency isn't independent, word cut from mission statement

**原文链接**: [https://www.axios.com/2025/12/17/brendan-carr-fcc-independent-senate-testimony-website](https://www.axios.com/2025/12/17/brendan-carr-fcc-independent-senate-testimony-website)

生成摘要时出错

---

## 38. GitHub postponing the announced billing change for self-hosted GitHub Actions

**原文标题**: GitHub postponing the announced billing change for self-hosted GitHub Actions

**原文链接**: [https://twitter.com/jaredpalmer/status/2001373329811181846](https://twitter.com/jaredpalmer/status/2001373329811181846)

生成摘要时出错

---

## 39. Egyptian Hieroglyphs: Lesson 1

**原文标题**: Egyptian Hieroglyphs: Lesson 1

**原文链接**: [https://www.egyptianhieroglyphs.net/egyptian-hieroglyphs/lesson-1/](https://www.egyptianhieroglyphs.net/egyptian-hieroglyphs/lesson-1/)

生成摘要时出错

---

## 40. GitHub Actions for self-hosted runners price increase postponed

**原文标题**: GitHub Actions for self-hosted runners price increase postponed

**原文链接**: [https://pricetimeline.com/news/189](https://pricetimeline.com/news/189)

生成摘要时出错

---

## 41. Firefox is becoming an AI browser and the internet is not at all happy about it

**原文标题**: Firefox is becoming an AI browser and the internet is not at all happy about it

**原文链接**: [https://www.pcgamer.com/hardware/firefox-is-becoming-an-ai-browser-and-the-internet-is-not-at-all-happy-about-it/](https://www.pcgamer.com/hardware/firefox-is-becoming-an-ai-browser-and-the-internet-is-not-at-all-happy-about-it/)

生成摘要时出错

---

## 42. The State of AI Coding Report 2025

**原文标题**: The State of AI Coding Report 2025

**原文链接**: [https://www.greptile.com/state-of-ai-coding-2025](https://www.greptile.com/state-of-ai-coding-2025)

生成摘要时出错

---

## 43. Agent Skills is now an open standard

**原文标题**: Agent Skills is now an open standard

**原文链接**: [https://claude.com/blog/organization-skills-and-directory](https://claude.com/blog/organization-skills-and-directory)

生成摘要时出错

---

## 44. What is an elliptic curve? (2019)

**原文标题**: What is an elliptic curve? (2019)

**原文链接**: [https://www.johndcook.com/blog/2019/02/21/what-is-an-elliptic-curve/](https://www.johndcook.com/blog/2019/02/21/what-is-an-elliptic-curve/)

生成摘要时出错

---

## 45. TLA+ Modeling Tips

**原文标题**: TLA+ Modeling Tips

**原文链接**: [http://muratbuffalo.blogspot.com/2025/12/tla-modeling-tips.html](http://muratbuffalo.blogspot.com/2025/12/tla-modeling-tips.html)

生成摘要时出错

---

## 46. Most parked domains now serving malicious content

**原文标题**: Most parked domains now serving malicious content

**原文链接**: [https://krebsonsecurity.com/2025/12/most-parked-domains-now-serving-malicious-content/](https://krebsonsecurity.com/2025/12/most-parked-domains-now-serving-malicious-content/)

生成摘要时出错

---

## 47. RCE via ND6 Router Advertisements in FreeBSD

**原文标题**: RCE via ND6 Router Advertisements in FreeBSD

**原文链接**: [https://www.freebsd.org/security/advisories/FreeBSD-SA-25:12.rtsold.asc](https://www.freebsd.org/security/advisories/FreeBSD-SA-25:12.rtsold.asc)

生成摘要时出错

---

## 48. Linux Kernel Rust Code Sees Its First CVE Vulnerability

**原文标题**: Linux Kernel Rust Code Sees Its First CVE Vulnerability

**原文链接**: [https://www.phoronix.com/news/First-Linux-Rust-CVE](https://www.phoronix.com/news/First-Linux-Rust-CVE)

生成摘要时出错

---

## 49. GPT-5.2-Codex

**原文标题**: GPT-5.2-Codex

**原文链接**: [https://openai.com/index/introducing-gpt-5-2-codex/](https://openai.com/index/introducing-gpt-5-2-codex/)

生成摘要时出错

---

## 50. Why do commercial spaces sit vacant?

**原文标题**: Why do commercial spaces sit vacant?

**原文链接**: [https://archive.strongtowns.org/journal/2025/5/21/why-do-commercial-spaces-sit-vacant](https://archive.strongtowns.org/journal/2025/5/21/why-do-commercial-spaces-sit-vacant)

生成摘要时出错

---

## 51. Introduction to Software Development Tooling (2024)

**原文标题**: Introduction to Software Development Tooling (2024)

**原文链接**: [https://bernsteinbear.com/isdt/](https://bernsteinbear.com/isdt/)

生成摘要时出错

---

## 52. US threatens EU digital services market access

**原文标题**: US threatens EU digital services market access

**原文链接**: [https://twitter.com/ustraderep/status/2000990028835508258](https://twitter.com/ustraderep/status/2000990028835508258)

生成摘要时出错

---

## 53. Cloudflare Radar 2025 Year in Review

**原文标题**: Cloudflare Radar 2025 Year in Review

**原文链接**: [https://radar.cloudflare.com/year-in-review/2025](https://radar.cloudflare.com/year-in-review/2025)

生成摘要时出错

---

## 54. Using TypeScript to Obtain One of the Rarest License Plates

**原文标题**: Using TypeScript to Obtain One of the Rarest License Plates

**原文链接**: [https://www.jack.bio/blog/licenseplate](https://www.jack.bio/blog/licenseplate)

生成摘要时出错

---

## 55. Inside PostHog: SSRF, ClickHouse SQL Escape and Default Postgres Creds to RCE

**原文标题**: Inside PostHog: SSRF, ClickHouse SQL Escape and Default Postgres Creds to RCE

**原文链接**: [https://mdisec.com/inside-posthog-how-ssrf-a-clickhouse-sql-escaping-0day-and-default-postgresql-credentials-formed-an-rce-chain-zdi-25-099-zdi-25-097-zdi-25-096/](https://mdisec.com/inside-posthog-how-ssrf-a-clickhouse-sql-escaping-0day-and-default-postgresql-credentials-formed-an-rce-chain-zdi-25-099-zdi-25-097-zdi-25-096/)

生成摘要时出错

---

## 56. Dafny: Verification-Aware Programming Language

**原文标题**: Dafny: Verification-Aware Programming Language

**原文链接**: [https://dafny.org/](https://dafny.org/)

生成摘要时出错

---

## 57. American Academy of Pediatrics loses HHS funding after criticizing RFK Jr.

**原文标题**: American Academy of Pediatrics loses HHS funding after criticizing RFK Jr.

**原文链接**: [https://www.washingtonpost.com/health/2025/12/17/aap-hhs-funding-rfk/](https://www.washingtonpost.com/health/2025/12/17/aap-hhs-funding-rfk/)

生成摘要时出错

---

## 58. AI Isn't Just Spying on You. It's Tricking You into Spending More

**原文标题**: AI Isn't Just Spying on You. It's Tricking You into Spending More

**原文链接**: [https://newrepublic.com/article/204525/artificial-intelligence-consumers-data-dynamic-pricing](https://newrepublic.com/article/204525/artificial-intelligence-consumers-data-dynamic-pricing)

生成摘要时出错

---

## 59. It's all about momentum

**原文标题**: It's all about momentum

**原文链接**: [https://combo.cc/posts/its-all-about-momentum-innit/](https://combo.cc/posts/its-all-about-momentum-innit/)

生成摘要时出错

---

## 60. Spain fines Airbnb €65M: Why the government is cracking down on illegal rentals

**原文标题**: Spain fines Airbnb €65M: Why the government is cracking down on illegal rentals

**原文链接**: [https://www.euronews.com/travel/2025/12/15/spain-fines-airbnb-65-million-why-the-government-is-cracking-down-on-illegal-rentals](https://www.euronews.com/travel/2025/12/15/spain-fines-airbnb-65-million-why-the-government-is-cracking-down-on-illegal-rentals)

生成摘要时出错

---

## 61. Chat-tails: Throwback terminal chat, built on Tailscale

**原文标题**: Chat-tails: Throwback terminal chat, built on Tailscale

**原文链接**: [https://tailscale.com/blog/chat-tails-terminal-chat](https://tailscale.com/blog/chat-tails-terminal-chat)

生成摘要时出错

---

## 62. A school locked down after AI flagged a gun. It was a clarinet

**原文标题**: A school locked down after AI flagged a gun. It was a clarinet

**原文链接**: [https://www.washingtonpost.com/nation/2025/12/17/ai-gun-school-detection/](https://www.washingtonpost.com/nation/2025/12/17/ai-gun-school-detection/)

生成摘要时出错

---

## 63. Show HN: High-Performance Wavelet Matrix for Python, Implemented in Rust

**原文标题**: Show HN: High-Performance Wavelet Matrix for Python, Implemented in Rust

**原文链接**: [https://pypi.org/project/wavelet-matrix/](https://pypi.org/project/wavelet-matrix/)

生成摘要时出错

---

## 64. Show HN: Learn Japanese contextually while browsing

**原文标题**: Show HN: Learn Japanese contextually while browsing

**原文链接**: [https://lingoku.ai/learn-japanese](https://lingoku.ai/learn-japanese)

生成摘要时出错

---

## 65. Show HN: I built a fast RSS reader in Zig

**原文标题**: Show HN: I built a fast RSS reader in Zig

**原文链接**: [https://github.com/superstarryeyes/hys](https://github.com/superstarryeyes/hys)

生成摘要时出错

---

## 66. Here is the 15 sec coding test I used to instantly filter out most applicants

**原文标题**: Here is the 15 sec coding test I used to instantly filter out most applicants

**原文链接**: [https://josezarazua.com/im-a-former-cto-here-is-the-15-sec-coding-test-i-used-to-instantly-filter-out-50-of-unqualified-applicants/](https://josezarazua.com/im-a-former-cto-here-is-the-15-sec-coding-test-i-used-to-instantly-filter-out-50-of-unqualified-applicants/)

生成摘要时出错

---

## 67. Virtualizing Nvidia HGX B200 GPUs with Open Source

**原文标题**: Virtualizing Nvidia HGX B200 GPUs with Open Source

**原文链接**: [https://www.ubicloud.com/blog/virtualizing-nvidia-hgx-b200-gpus-with-open-source](https://www.ubicloud.com/blog/virtualizing-nvidia-hgx-b200-gpus-with-open-source)

生成摘要时出错

---

## 68. Letta Code

**原文标题**: Letta Code

**原文链接**: [https://www.letta.com/blog/letta-code](https://www.letta.com/blog/letta-code)

生成摘要时出错

---

## 69. More than 100 rally against data centers at Michigan Capitol

**原文标题**: More than 100 rally against data centers at Michigan Capitol

**原文链接**: [https://www.lansingstatejournal.com/story/news/local/2025/12/16/lansing-state-capitol-data-centers-rally-michigan/87792001007/](https://www.lansingstatejournal.com/story/news/local/2025/12/16/lansing-state-capitol-data-centers-rally-michigan/87792001007/)

生成摘要时出错

---

## 70. Windows 11 will ask consent before sharing personal files with AI after outrage

**原文标题**: Windows 11 will ask consent before sharing personal files with AI after outrage

**原文链接**: [https://www.windowslatest.com/2025/12/17/microsoft-confirms-windows-11-will-ask-for-consent-before-sharing-your-personal-files-with-ai-after-outrage/](https://www.windowslatest.com/2025/12/17/microsoft-confirms-windows-11-will-ask-for-consent-before-sharing-your-personal-files-with-ai-after-outrage/)

生成摘要时出错

---

## 71. Learning Fortran (2024)

**原文标题**: Learning Fortran (2024)

**原文链接**: [https://uncenter.dev/posts/learning-fortran/](https://uncenter.dev/posts/learning-fortran/)

生成摘要时出错

---

## 72. VRChat: “There are more Japanese creators than all other countries combined”

**原文标题**: VRChat: “There are more Japanese creators than all other countries combined”

**原文链接**: [https://twitter.com/chyadosensei/status/2001356290531156159](https://twitter.com/chyadosensei/status/2001356290531156159)

生成摘要时出错

---

## 73. Venezuela's Navy Begins Escorting Ships as U.S. Threatens Blockade

**原文标题**: Venezuela's Navy Begins Escorting Ships as U.S. Threatens Blockade

**原文链接**: [https://www.nytimes.com/live/2025/12/17/us/trump-news](https://www.nytimes.com/live/2025/12/17/us/trump-news)

生成摘要时出错

---

## 74. California judge rules that Tesla engaged in deceptive marketing for Autopilot

**原文标题**: California judge rules that Tesla engaged in deceptive marketing for Autopilot

**原文链接**: [https://www.cnbc.com/2025/12/16/california-judge-says-tesla-engaged-in-deceptive-autopilot-marketing-.html](https://www.cnbc.com/2025/12/16/california-judge-says-tesla-engaged-in-deceptive-autopilot-marketing-.html)

生成摘要时出错

---

## 75. Locked out: How a gift card purchase destroyed an Apple account

**原文标题**: Locked out: How a gift card purchase destroyed an Apple account

**原文链接**: [https://appleinsider.com/articles/25/12/13/locked-out-how-a-gift-card-purchase-destroyed-an-apple-account](https://appleinsider.com/articles/25/12/13/locked-out-how-a-gift-card-purchase-destroyed-an-apple-account)

生成摘要时出错

---

## 76. 'It's surreal': How US sanctions lock ICC judges out of daily life

**原文标题**: 'It's surreal': How US sanctions lock ICC judges out of daily life

**原文链接**: [https://www.irishtimes.com/world/us/2025/12/12/its-surreal-us-sanctions-lock-international-criminal-court-judge-out-of-daily-life/](https://www.irishtimes.com/world/us/2025/12/12/its-surreal-us-sanctions-lock-international-criminal-court-judge-out-of-daily-life/)

生成摘要时出错

---

## 77. FTX insider Caroline Ellison has been moved out of prison

**原文标题**: FTX insider Caroline Ellison has been moved out of prison

**原文链接**: [https://www.businessinsider.com/caroline-ellison-prison-release-ftx-sam-bankman-fried-2025-12](https://www.businessinsider.com/caroline-ellison-prison-release-ftx-sam-bankman-fried-2025-12)

生成摘要时出错

---

## 78. Valve Is Running Apple's Playbook in Reverse

**原文标题**: Valve Is Running Apple's Playbook in Reverse

**原文链接**: [https://www.garbagecollected.dev/p/valve-the-reverse-apple](https://www.garbagecollected.dev/p/valve-the-reverse-apple)

生成摘要时出错

---

## 79. MIT Professor Is Fatally Shot in His Home

**原文标题**: MIT Professor Is Fatally Shot in His Home

**原文链接**: [https://www.nytimes.com/2025/12/16/us/mit-professor-shot-brookline-nuno-loureiro.html](https://www.nytimes.com/2025/12/16/us/mit-professor-shot-brookline-nuno-loureiro.html)

生成摘要时出错

---

## 80. Explaining the widening divides in us midlife mortality: Is there a smoking gun?

**原文标题**: Explaining the widening divides in us midlife mortality: Is there a smoking gun?

**原文链接**: [https://www.nber.org/papers/w34553](https://www.nber.org/papers/w34553)

生成摘要时出错

---

## 81. systemd v259 Released

**原文标题**: systemd v259 Released

**原文链接**: [https://github.com/systemd/systemd/releases/tag/v259](https://github.com/systemd/systemd/releases/tag/v259)

生成摘要时出错

---

## 82. More than half of researchers now use AI for peer review, often against guidance

**原文标题**: More than half of researchers now use AI for peer review, often against guidance

**原文链接**: [https://www.nature.com/articles/d41586-025-04066-5](https://www.nature.com/articles/d41586-025-04066-5)

生成摘要时出错

---

## 83. The US govt has revoked the non-immigrant visa of Nobel laureate Wole Soyinka [video]

**原文标题**: The US govt has revoked the non-immigrant visa of Nobel laureate Wole Soyinka [video]

**原文链接**: [https://www.youtube.com/watch?v=ple4xophXfM](https://www.youtube.com/watch?v=ple4xophXfM)

生成摘要时出错

---

## 84. Nvidia plans heavy cuts to GPU supply in early 2026

**原文标题**: Nvidia plans heavy cuts to GPU supply in early 2026

**原文链接**: [https://overclock3d.net/news/gpu-displays/nvidia-plans-heavy-cuts-to-gpu-supply-in-early-2026/](https://overclock3d.net/news/gpu-displays/nvidia-plans-heavy-cuts-to-gpu-supply-in-early-2026/)

生成摘要时出错

---

## 85. Firefox will have an option to disable all AI features

**原文标题**: Firefox will have an option to disable all AI features

**原文链接**: [https://mastodon.social/@firefoxwebdevs/115740500373677782](https://mastodon.social/@firefoxwebdevs/115740500373677782)

生成摘要时出错

---

## 86. America's Dirtiest Carbon Polluters, Mapped to Ridiculous Precision

**原文标题**: America's Dirtiest Carbon Polluters, Mapped to Ridiculous Precision

**原文链接**: [https://gizmodo.com/americas-dirtiest-carbon-polluters-mapped-to-ridiculous-precision-2000700924](https://gizmodo.com/americas-dirtiest-carbon-polluters-mapped-to-ridiculous-precision-2000700924)

生成摘要时出错

---

## 87. Reverse-engineering the RK3588 NPU: Hacking limits to run vision transformers

**原文标题**: Reverse-engineering the RK3588 NPU: Hacking limits to run vision transformers

**原文链接**: [https://amohan.dev/blog/2025/shard-optimizing-vision-transformers-edge-npu/](https://amohan.dev/blog/2025/shard-optimizing-vision-transformers-edge-npu/)

生成摘要时出错

---

## 88. Mozilla's New CEO Confirms Firefox Will Become an "AI Browser"

**原文标题**: Mozilla's New CEO Confirms Firefox Will Become an "AI Browser"

**原文链接**: [https://www.omgubuntu.co.uk/2025/12/mozilla-new-ceo-firefox-ai-browser-strategy](https://www.omgubuntu.co.uk/2025/12/mozilla-new-ceo-firefox-ai-browser-strategy)

生成摘要时出错

---

## 89. AI capability isn't humanness

**原文标题**: AI capability isn't humanness

**原文链接**: [https://research.roundtable.ai/capabilities-humanness/](https://research.roundtable.ai/capabilities-humanness/)

生成摘要时出错

---

## 90. UK Lawmakers Propose Mandatory On-Device Surveillance and VPN Age Verification

**原文标题**: UK Lawmakers Propose Mandatory On-Device Surveillance and VPN Age Verification

**原文链接**: [https://reclaimthenet.org/uk-lawmakers-propose-mandatory-on-device-surveillance-and-vpn-age-verification](https://reclaimthenet.org/uk-lawmakers-propose-mandatory-on-device-surveillance-and-vpn-age-verification)

生成摘要时出错

---

## 91. Heart and Kidney Diseases and Type 2 Diabetes May Be One Ailment

**原文标题**: Heart and Kidney Diseases and Type 2 Diabetes May Be One Ailment

**原文链接**: [https://www.scientificamerican.com/article/heart-and-kidney-diseases-plus-type-2-diabetes-may-be-one-illness-treatable/](https://www.scientificamerican.com/article/heart-and-kidney-diseases-plus-type-2-diabetes-may-be-one-illness-treatable/)

生成摘要时出错

---

## 92. We Let AI Run Our Office Vending Machine. It Lost Hundreds of Dollars

**原文标题**: We Let AI Run Our Office Vending Machine. It Lost Hundreds of Dollars

**原文链接**: [https://www.wsj.com/tech/ai/anthropic-claude-ai-vending-machine-agent-b7e84e34](https://www.wsj.com/tech/ai/anthropic-claude-ai-vending-machine-agent-b7e84e34)

生成摘要时出错

---

## 93. Meta Segment Anything Model Audio

**原文标题**: Meta Segment Anything Model Audio

**原文链接**: [https://ai.meta.com/samaudio/](https://ai.meta.com/samaudio/)

生成摘要时出错

---

## 94. Show HN: Composify – Open-Source Visual Editor / Server-Driven UI for React

**原文标题**: Show HN: Composify – Open-Source Visual Editor / Server-Driven UI for React

**原文链接**: [https://github.com/composify-js/composify](https://github.com/composify-js/composify)

生成摘要时出错

---

## 95. Online Textbook for Braid groups and knots and tangles

**原文标题**: Online Textbook for Braid groups and knots and tangles

**原文链接**: [https://matthematics.com/redoak/redoak.html](https://matthematics.com/redoak/redoak.html)

生成摘要时出错

---

## 96. Make Me CEO of Mozilla

**原文标题**: Make Me CEO of Mozilla

**原文链接**: [https://blog.kingcons.io/posts/make-me-ceo-of-mozilla.html](https://blog.kingcons.io/posts/make-me-ceo-of-mozilla.html)

生成摘要时出错

---

## 97. Flow – A Programmer's Text Editor

**原文标题**: Flow – A Programmer's Text Editor

**原文链接**: [https://flow-control.dev/](https://flow-control.dev/)

生成摘要时出错

---

## 98. Microsoft kills IntelliCode in favor of the paid Copilot

**原文标题**: Microsoft kills IntelliCode in favor of the paid Copilot

**原文链接**: [https://visualstudiomagazine.com/articles/2025/12/17/microsoft-quietly-kills-intellicode-as-ai-strategy-shifts-to-copilot.aspx](https://visualstudiomagazine.com/articles/2025/12/17/microsoft-quietly-kills-intellicode-as-ai-strategy-shifts-to-copilot.aspx)

生成摘要时出错

---

## 99. The Mysterious Forces Steering Views on Hacker News

**原文标题**: The Mysterious Forces Steering Views on Hacker News

**原文链接**: [https://xn--gckvb8fzb.com/the-mysterious-forces-steering-views-on-hacker-news/](https://xn--gckvb8fzb.com/the-mysterious-forces-steering-views-on-hacker-news/)

生成摘要时出错

---

## 100. Show HN: GitForms – Zero-cost contact forms using GitHub Issues as database

**原文标题**: Show HN: GitForms – Zero-cost contact forms using GitHub Issues as database

**原文链接**: [https://gitforms-landing.vercel.app/](https://gitforms-landing.vercel.app/)

生成摘要时出错

---

