# Hacker News 热门文章摘要 (2026-04-25)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. DeepSeek v4

**原文标题**: DeepSeek v4

**原文链接**: [https://api-docs.deepseek.com/news/news260424](https://api-docs.deepseek.com/news/news260424)

DeepSeek-V4 Preview 正式上线并开源，开启了高性价比的百万级上下文时代。本次发布包含两款模型：

1.  **DeepSeek-V4-Pro**：一款强大的模型，拥有 1.6 万亿（T）总参数和 490 亿（B）活跃参数，性能可与顶级的闭源模型媲美。它在智能体编程方面表现卓越（开源SOTA），拥有丰富的世界知识（仅次于 Gemini-3.1-Pro），并在数学、STEM 和编码领域展现世界级的推理能力。
2.  **DeepSeek-V4-Flash**：一个更高效的选择，拥有 2840 亿（B）总参数和 130 亿（B）活跃参数，提供快速响应时间和经济实惠的 API 定价。其推理能力与 V4-Pro 接近，并在简单智能体任务上表现相当。

主要创新包括一种新颖的注意力机制（分词压缩 + DeepSeek 稀疏注意力），用于实现超高上下文效率，使百万级上下文成为所有 DeepSeek 服务的默认配置，并大幅降低了计算和内存成本。

DeepSeek-V4 还针对智能体能力进行了专门优化，可与领先的 AI 智能体无缝集成，并为 DeepSeek 内部的智能体编程提供支持。

API 即日起可用，支持 OpenAI ChatCompletions 和 Anthropic API。用户只需将模型更新为 `deepseek-v4-pro` 或 `deepseek-v4-flash`，这两款模型均支持百万级上下文和思/非思双模式。旧模型（`deepseek-chat`、`deepseek-reasoner`）将于 2026 年 7 月 24 日停用。DeepSeek 强调应以官方新闻渠道为准，并重申其对 AGI 的承诺。

---

## 2. 我取消了Claude：Token问题、质量下降、支持不佳

**原文标题**: I cancelled Claude: Token issues, declining quality, and poor support

**原文链接**: [https://nickyreinert.de/en/2026/2026-04-24-claude-critics/](https://nickyreinert.de/en/2026/2026-04-24-claude-critics/)

作者起初对Claude Code抱有极大的热情，称赞其速度快、token配额合理且质量高。然而，由于严重的token问题、感知到的质量下降以及糟糕的客户支持，这种热情迅速消退了。

一个主要的痛点是，在回答简单问题时，token使用量会无故飙升至100%。AI客服毫无帮助，而人工客服则以一份通用、复制粘贴的使用限制说明来回应，既未能解决具体问题，随后又突然关闭了工单。

作者还发现Claude的质量有所下降，token额度消耗得快得多。一个明显的例子是，Claude Opus建议了一个“偷懒”的权宜之计，而不是一个恰当的代码修复，而他为了纠正这个方案，又消耗了50%的token额度。此外，会话缓存在中断后经常消失，这迫使他不得不耗费token重新读取代码库。没有解释或文档的不一致的“月度使用限制”警告会不时出现，随后又消失。

尽管作者是Claude的“忠实用户”，承认它带来了显著的生产力优势，并理解提供推理服务所固有的扩展挑战，他仍取消了订阅。他断定Anthropic似乎无法应对涌入的新客户，并决定“为该公司减轻一些负担”。

---

## 3. Meta 告知员工将裁员 10%

**原文标题**: Meta tells staff it will cut 10% of jobs

**原文链接**: [https://www.bloomberg.com/news/articles/2026-04-23/meta-tells-staff-it-will-cut-10-of-jobs-in-push-for-efficiency](https://www.bloomberg.com/news/articles/2026-04-23/meta-tells-staff-it-will-cut-10-of-jobs-in-push-for-efficiency)

无法访问文章链接。

---

## 4. 谷歌计划向Anthropic投资最高400亿美元。

**原文标题**: Google plans to invest up to $40B in Anthropic

**原文链接**: [https://www.bloomberg.com/news/articles/2026-04-24/google-plans-to-invest-up-to-40-billion-in-anthropic](https://www.bloomberg.com/news/articles/2026-04-24/google-plans-to-invest-up-to-40-billion-in-anthropic)

无法访问文章链接。

---

## 5. US special forces soldier arrested after allegedly winning $400k on Maduro raid

**原文标题**: US special forces soldier arrested after allegedly winning $400k on Maduro raid

**原文链接**: [https://www.cnn.com/2026/04/23/politics/us-special-forces-soldier-arrested-maduro-raid-trade](https://www.cnn.com/2026/04/23/politics/us-special-forces-soldier-arrested-maduro-raid-trade)

生成摘要时出错

---

## 6. Sabotaging projects by overthinking, scope creep, and structural diffing

**原文标题**: Sabotaging projects by overthinking, scope creep, and structural diffing

**原文链接**: [https://kevinlynagh.com/newsletter/2026_04_overthinking/](https://kevinlynagh.com/newsletter/2026_04_overthinking/)

生成摘要时出错

---

## 7. 新的 10 GbE USB 网卡散热更好、更小、更便宜。

**原文标题**: New 10 GbE USB adapters are cooler, smaller, cheaper

**原文链接**: [https://www.jeffgeerling.com/blog/2026/new-10-gbe-usb-adapters-cooler-smaller-cheaper/](https://www.jeffgeerling.com/blog/2026/new-10-gbe-usb-adapters-cooler-smaller-cheaper/)

基于RTL8159芯片的新型10GbE USB 3.2适配器正逐渐成为传统笨重Thunderbolt 10GbE适配器运行温度更低、体积更小、价格更便宜的替代品。例如，售价80美元的WisdPi型号价格不到Thunderbolt同类产品的一半。

然而，要达到完整的10 Gbps速度，高度依赖于主机的USB端口。作者发现，只有配备USB 3.2 Gen 2x2 (20 Gbps) 端口的台式PC才能达到完整的9.5 Gbps性能。而在配备USB 3.1/3.2 Gen 2 (10 Gbps) 端口的笔记本电脑（如MacBooks和Framework 13）上，速度则限制在6-7 Gbps。混乱的USB命名规范和Windows系统端口速度报告不足，使这一挑战更加严峻。

尽管在普通端口上存在潜在的速度限制，这些新型适配器运行温度显著更低（约42.5°C），功耗也低于以发热量大而闻名的老式基于Aquantia芯片的10G解决方案。

总而言之，如果您已拥有10 Gbps RJ45网络和USB 3.2 Gen 2x2端口，或者优先考虑紧凑、低温的设备，这些新型USB适配器具有不错的价值。然而，如果必须保证完整的10 Gbps速度或SFP+支持，Thunderbolt仍然是更优的选择。对于大多数用户而言，2.5 Gbps或5 Gbps的USB适配器因其更低的成本和在普通USB 3.2 Gen 2端口上可比的实际性能，仍然具有更好的整体价值。

---

## 8. 挪威将成为最新一个禁用16岁以下未成年人社交媒体的国家。

**原文标题**: Norway set to become latest country to ban social media for under 16s

**原文链接**: [https://www.bloomberg.com/news/articles/2026-04-24/norway-wants-kids-to-be-kids-with-social-media-ban-for-under-16s](https://www.bloomberg.com/news/articles/2026-04-24/norway-wants-kids-to-be-kids-with-social-media-ban-for-under-16s)

无法访问文章链接。

---

## 9. 如何反社交：非连贯且孤立的社交体验指南

**原文标题**: How to be anti-social – a guide to incoherent and isolating social experiences

**原文链接**: [https://nate.leaflet.pub/3mk4xkaxobc2p](https://nate.leaflet.pub/3mk4xkaxobc2p)

本指南题为“如何反社会”，概述了培养脱节且孤立社交体验的策略。它建议读者，假设他人做出令人困惑或不安的行为缺乏理智原因，并将模糊不清的行为解读为恶意、无知或不道德，且通过个人恐惧来过滤这些行为。该指南强调绝对信任自己的直觉和感受，不鼓励对个人假设提出任何挑战。

它建议，当个人假设受到质疑或当讨论超出自己的专业领域时，转移对话焦点，以避免表现出弱点。提问时，应该暗示自己原有立场的正确性。该指南提倡面对压倒性的异议时固执己见，并通过精心筛选互动细节来利用直接的社交网络，争取支持者对抗反对者。

进一步的指示包括，忽略与自己意见相左者的资历或过往记录，并且不宽恕他人的错误，特别是陌生人的错误。最终，当对话失败时，建议是退回内心，并避免去理解那些尚未被理解的人。

---

## 10. Firefox Has Integrated Brave's Adblock Engine

**原文标题**: Firefox Has Integrated Brave's Adblock Engine

**原文链接**: [https://itsfoss.com/news/firefox-ships-brave-adblock-engine/](https://itsfoss.com/news/firefox-ships-brave-adblock-engine/)

生成摘要时出错

---

## 11. Spinel: Ruby AOT Native Compiler

**原文标题**: Spinel: Ruby AOT Native Compiler

**原文链接**: [https://github.com/matz/spinel](https://github.com/matz/spinel)

生成摘要时出错

---

## 12. There Will Be a Scientific Theory of Deep Learning

**原文标题**: There Will Be a Scientific Theory of Deep Learning

**原文链接**: [https://arxiv.org/abs/2604.21691](https://arxiv.org/abs/2604.21691)

生成摘要时出错

---

## 13. Ubuntu 26.04

**原文标题**: Ubuntu 26.04

**原文链接**: [https://lwn.net/Articles/1069399/](https://lwn.net/Articles/1069399/)

生成摘要时出错

---

## 14. My audio interface has SSH enabled by default

**原文标题**: My audio interface has SSH enabled by default

**原文链接**: [https://hhh.hn/rodecaster-duo-fw/](https://hhh.hn/rodecaster-duo-fw/)

生成摘要时出错

---

## 15. Show HN: Tolaria – Open-source macOS app to manage Markdown knowledge bases

**原文标题**: Show HN: Tolaria – Open-source macOS app to manage Markdown knowledge bases

**原文链接**: [https://github.com/refactoringhq/tolaria](https://github.com/refactoringhq/tolaria)

生成摘要时出错

---

## 16. Replace IBM Quantum back end with /dev/urandom

**原文标题**: Replace IBM Quantum back end with /dev/urandom

**原文链接**: [https://github.com/yuvadm/quantumslop/blob/25ad2e76ae58baa96f6219742459407db9dd17f5/URANDOM_DEMO.md](https://github.com/yuvadm/quantumslop/blob/25ad2e76ae58baa96f6219742459407db9dd17f5/URANDOM_DEMO.md)

生成摘要时出错

---

## 17. Why I Write (1946)

**原文标题**: Why I Write (1946)

**原文链接**: [https://www.orwellfoundation.com/the-orwell-foundation/orwell/essays-and-other-works/why-i-write/](https://www.orwellfoundation.com/the-orwell-foundation/orwell/essays-and-other-works/why-i-write/)

生成摘要时出错

---

## 18. SDL Now Supports DOS

**原文标题**: SDL Now Supports DOS

**原文链接**: [https://github.com/libsdl-org/SDL/pull/15377](https://github.com/libsdl-org/SDL/pull/15377)

生成摘要时出错

---

## 19. Habitual coffee intake shapes the microbiome, modifies physiology and cognition

**原文标题**: Habitual coffee intake shapes the microbiome, modifies physiology and cognition

**原文链接**: [https://www.nature.com/articles/s41467-026-71264-8](https://www.nature.com/articles/s41467-026-71264-8)

生成摘要时出错

---

## 20. The Classic American Diner

**原文标题**: The Classic American Diner

**原文链接**: [https://blogs.loc.gov/picturethis/2026/04/the-classic-american-diner/](https://blogs.loc.gov/picturethis/2026/04/the-classic-american-diner/)

生成摘要时出错

---

## 21. OpenAI releases GPT-5.5 and GPT-5.5 Pro in the API

**原文标题**: OpenAI releases GPT-5.5 and GPT-5.5 Pro in the API

**原文链接**: [https://developers.openai.com/api/docs/changelog](https://developers.openai.com/api/docs/changelog)

生成摘要时出错

---

## 22. Using the internet like it's 1999

**原文标题**: Using the internet like it's 1999

**原文链接**: [https://joshblais.com/blog/using-the-internet-like-its-1999/](https://joshblais.com/blog/using-the-internet-like-its-1999/)

生成摘要时出错

---

## 23. U.S. soldier charged with using classified info to profit from prediction market

**原文标题**: U.S. soldier charged with using classified info to profit from prediction market

**原文链接**: [https://www.justice.gov/usao-sdny/pr/us-soldier-charged-using-classified-information-profit-prediction-market-bets?bm-verify=AAQAAAAN_____y6To7sZYZ502biZwIHXlr-7zXZUqV4H0xLTfW__wDA3SjNLqifXRaQwsikyuz6IJknyuL8xfVYRkesxcDk5V10m-HoXl2K93f17rygBphL77WVFoQ_XvlmUo922IwM_DQ66137X6wWMtpdHslcEjpJG7KbBmUw9Su4kDENpDt_yv2spThQZehgv-X1Adk5U2VHfp41co2s_QJGjRj4y0KmL1mhSCyVaE7MC1LHG0mtP-xYmD0xBOQwn6PlHkPiP5Nt46h5ZIjLGXgCZDEVD42i7rIEM379DKLPUPX0PDNmOAwFSuTqcTDVnT_UUV8vxpHLRMb7rUxPxKUPcIB23iZTRJddWDDtPHMXadpwv67xr-f1sKDLZT9NgHCO4iuC2EthmAt0](https://www.justice.gov/usao-sdny/pr/us-soldier-charged-using-classified-information-profit-prediction-market-bets?bm-verify=AAQAAAAN_____y6To7sZYZ502biZwIHXlr-7zXZUqV4H0xLTfW__wDA3SjNLqifXRaQwsikyuz6IJknyuL8xfVYRkesxcDk5V10m-HoXl2K93f17rygBphL77WVFoQ_XvlmUo922IwM_DQ66137X6wWMtpdHslcEjpJG7KbBmUw9Su4kDENpDt_yv2spThQZehgv-X1Adk5U2VHfp41co2s_QJGjRj4y0KmL1mhSCyVaE7MC1LHG0mtP-xYmD0xBOQwn6PlHkPiP5Nt46h5ZIjLGXgCZDEVD42i7rIEM379DKLPUPX0PDNmOAwFSuTqcTDVnT_UUV8vxpHLRMb7rUxPxKUPcIB23iZTRJddWDDtPHMXadpwv67xr-f1sKDLZT9NgHCO4iuC2EthmAt0)

生成摘要时出错

---

## 24. Show HN: How LLMs Work – Interactive visual guide based on Karpathy's lecture

**原文标题**: Show HN: How LLMs Work – Interactive visual guide based on Karpathy's lecture

**原文链接**: [https://ynarwal.github.io/how-llms-work/](https://ynarwal.github.io/how-llms-work/)

生成摘要时出错

---

## 25. South Korea police arrest man for posting AI photo of runaway wolf

**原文标题**: South Korea police arrest man for posting AI photo of runaway wolf

**原文链接**: [https://www.bbc.com/news/articles/c4gx1n0dl9no](https://www.bbc.com/news/articles/c4gx1n0dl9no)

生成摘要时出错

---

## 26. Plain text has been around for decades and it’s here to stay

**原文标题**: Plain text has been around for decades and it’s here to stay

**原文链接**: [https://unsung.aresluna.org/plain-text-has-been-around-for-decades-and-its-here-to-stay/](https://unsung.aresluna.org/plain-text-has-been-around-for-decades-and-its-here-to-stay/)

生成摘要时出错

---

## 27. Girl, 10, finds rare Mexican axolotl under Welsh bridge

**原文标题**: Girl, 10, finds rare Mexican axolotl under Welsh bridge

**原文链接**: [https://www.bbc.com/news/articles/c9d4zgnqpqeo](https://www.bbc.com/news/articles/c9d4zgnqpqeo)

生成摘要时出错

---

## 28. Show HN: A Karpathy-style LLM wiki your agents maintain (Markdown and Git)

**原文标题**: Show HN: A Karpathy-style LLM wiki your agents maintain (Markdown and Git)

**原文链接**: [https://github.com/nex-crm/wuphf](https://github.com/nex-crm/wuphf)

生成摘要时出错

---

## 29. Google to invest up to $40B in Anthropic in cash and compute

**原文标题**: Google to invest up to $40B in Anthropic in cash and compute

**原文链接**: [https://techcrunch.com/2026/04/24/google-to-invest-up-to-40b-in-anthropic-in-cash-and-compute/](https://techcrunch.com/2026/04/24/google-to-invest-up-to-40b-in-anthropic-in-cash-and-compute/)

生成摘要时出错

---

## 30. Hear your agent suffer through your code

**原文标题**: Hear your agent suffer through your code

**原文链接**: [https://github.com/AndrewVos/endless-toil](https://github.com/AndrewVos/endless-toil)

生成摘要时出错

---

## 31. TorchTPU: Running PyTorch Natively on TPUs at Google Scale

**原文标题**: TorchTPU: Running PyTorch Natively on TPUs at Google Scale

**原文链接**: [https://developers.googleblog.com/torchtpu-running-pytorch-natively-on-tpus-at-google-scale/](https://developers.googleblog.com/torchtpu-running-pytorch-natively-on-tpus-at-google-scale/)

生成摘要时出错

---

## 32. I'm done making desktop applications (2009)

**原文标题**: I'm done making desktop applications (2009)

**原文链接**: [https://www.kalzumeus.com/2009/09/05/desktop-aps-versus-web-apps/](https://www.kalzumeus.com/2009/09/05/desktop-aps-versus-web-apps/)

生成摘要时出错

---

## 33. Turbo Vision 2.0 – a modern port

**原文标题**: Turbo Vision 2.0 – a modern port

**原文链接**: [https://github.com/magiblot/tvision](https://github.com/magiblot/tvision)

生成摘要时出错

---

## 34. UK Biobank leak: Health details of 500k people offered for sale on Alibaba

**原文标题**: UK Biobank leak: Health details of 500k people offered for sale on Alibaba

**原文链接**: [https://www.bmj.com/content/393/bmj.s781](https://www.bmj.com/content/393/bmj.s781)

生成摘要时出错

---

## 35. Show HN: I've built a nice home server OS

**原文标题**: Show HN: I've built a nice home server OS

**原文链接**: [https://lightwhale.asklandd.dk/](https://lightwhale.asklandd.dk/)

生成摘要时出错

---

## 36. Tariffs Raised Consumers' Prices, but the Refunds Go Only to Businesses

**原文标题**: Tariffs Raised Consumers' Prices, but the Refunds Go Only to Businesses

**原文链接**: [https://www.nytimes.com/2026/04/24/us/politics/companies-consumers-tariff-refunds.html](https://www.nytimes.com/2026/04/24/us/politics/companies-consumers-tariff-refunds.html)

生成摘要时出错

---

## 37. Niri 26.04: Scrollable-tiling Wayland compositor

**原文标题**: Niri 26.04: Scrollable-tiling Wayland compositor

**原文链接**: [https://github.com/niri-wm/niri/releases/tag/v26.04](https://github.com/niri-wm/niri/releases/tag/v26.04)

生成摘要时出错

---

## 38. Refuse to let your doctor record you

**原文标题**: Refuse to let your doctor record you

**原文链接**: [https://buttondown.com/maiht3k/archive/why-you-should-refuse-to-let-your-doctor-record/](https://buttondown.com/maiht3k/archive/why-you-should-refuse-to-let-your-doctor-record/)

生成摘要时出错

---

## 39. DeepSeek-V4: Towards Highly Efficient Million-Token Context Intelligence

**原文标题**: DeepSeek-V4: Towards Highly Efficient Million-Token Context Intelligence

**原文链接**: [https://huggingface.co/deepseek-ai/DeepSeek-V4-Pro](https://huggingface.co/deepseek-ai/DeepSeek-V4-Pro)

生成摘要时出错

---

## 40. Open source memory layer so any AI agent can do what Claude.ai and ChatGPT do

**原文标题**: Open source memory layer so any AI agent can do what Claude.ai and ChatGPT do

**原文链接**: [https://alash3al.github.io/stash?_v01](https://alash3al.github.io/stash?_v01)

生成摘要时出错

---

## 41. SFO Quiet Airport (2025)

**原文标题**: SFO Quiet Airport (2025)

**原文链接**: [https://viewfromthewing.com/san-francisco-airport-removed-90-minutes-of-daily-noise-travelers-say-it-changed-everything/](https://viewfromthewing.com/san-francisco-airport-removed-90-minutes-of-daily-noise-travelers-say-it-changed-everything/)

生成摘要时出错

---

## 42. Why Not Venus?

**原文标题**: Why Not Venus?

**原文链接**: [https://mceglowski.substack.com/p/why-not-venus](https://mceglowski.substack.com/p/why-not-venus)

生成摘要时出错

---

## 43. Google Flow Music

**原文标题**: Google Flow Music

**原文链接**: [https://www.flowmusic.app/](https://www.flowmusic.app/)

生成摘要时出错

---

## 44. Do I belong in tech anymore?

**原文标题**: Do I belong in tech anymore?

**原文链接**: [https://ky.fyi/posts/ai-burnout](https://ky.fyi/posts/ai-burnout)

生成摘要时出错

---

## 45. Diatec, known for its mechanical keyboard brand FILCO, has ceased operations

**原文标题**: Diatec, known for its mechanical keyboard brand FILCO, has ceased operations

**原文链接**: [https://gigazine.net/gsc_news/en/20260424-filco-diatec/](https://gigazine.net/gsc_news/en/20260424-filco-diatec/)

生成摘要时出错

---

## 46. Show HN: Gova – The declarative GUI framework for Go

**原文标题**: Show HN: Gova – The declarative GUI framework for Go

**原文链接**: [https://github.com/NV404/gova](https://github.com/NV404/gova)

生成摘要时出错

---

## 47. The operating cost of adult and gambling startups

**原文标题**: The operating cost of adult and gambling startups

**原文链接**: [https://orchidfiles.com/stigma-is-a-tax-on-every-operational-decision/](https://orchidfiles.com/stigma-is-a-tax-on-every-operational-decision/)

生成摘要时出错

---

## 48. Martin Galway's music source files from 1980's Commodore 64 games

**原文标题**: Martin Galway's music source files from 1980's Commodore 64 games

**原文链接**: [https://github.com/MartinGalway/C64_music](https://github.com/MartinGalway/C64_music)

生成摘要时出错

---

## 49. Education must go beyond the mere production of words

**原文标题**: Education must go beyond the mere production of words

**原文链接**: [https://www.ncregister.com/commentaries/schnell-repairing-the-ruins](https://www.ncregister.com/commentaries/schnell-repairing-the-ruins)

生成摘要时出错

---

## 50. Mounting tar archives as a filesystem in WebAssembly

**原文标题**: Mounting tar archives as a filesystem in WebAssembly

**原文链接**: [https://jeroen.github.io/notes/webassembly-tar/](https://jeroen.github.io/notes/webassembly-tar/)

生成摘要时出错

---

## 51. Aspartame is not that bad? (2022)

**原文标题**: Aspartame is not that bad? (2022)

**原文链接**: [https://dynomight.net/aspartame/](https://dynomight.net/aspartame/)

生成摘要时出错

---

## 52. Composition shouldn't be this hard

**原文标题**: Composition shouldn't be this hard

**原文链接**: [https://www.cambra.dev/blog/announcement/](https://www.cambra.dev/blog/announcement/)

生成摘要时出错

---

## 53. Show HN: Browser Harness – Gives LLM freedom to complete any browser task

**原文标题**: Show HN: Browser Harness – Gives LLM freedom to complete any browser task

**原文链接**: [https://github.com/browser-use/browser-harness](https://github.com/browser-use/browser-harness)

生成摘要时出错

---

## 54. Different language models learn similar number representations

**原文标题**: Different language models learn similar number representations

**原文链接**: [https://arxiv.org/abs/2604.20817](https://arxiv.org/abs/2604.20817)

This paper, "Convergent Evolution: How Different Language Models Learn Similar Number Representations," reveals that various language models (LMs) consistently learn to represent numbers using periodic features, with dominant periods at T=2, 5, and 10. The authors identify a two-tiered hierarchy: while all tested models (Transformers, Linear RNNs, LSTMs, word embeddings) exhibit "period-T spikes" in the Fourier domain (Fourier domain sparsity), only some acquire "geometrically separable features" that allow for linear classification of a number mod-T.

The research theoretically proves that Fourier domain sparsity is necessary but not sufficient for mod-T geometric separability. Empirically, the study investigates the conditions under which models develop geometrically separable features, finding that data, architecture, optimizer, and tokenizer all play significant roles. They identify two primary routes: models can learn these features from complementary co-occurrence signals in general language data (e.g., text-number co-occurrence and cross-number interaction) or from multi-token (but not single-token) addition problems.

Overall, the findings underscore a phenomenon of "convergent evolution," where a diverse range of models learn remarkably similar numerical representations despite being trained with different signals and architectures.

---

## 55. Framework Laptop 13 Pro: Major Upgrades and Linux Front and Center

**原文标题**: Framework Laptop 13 Pro: Major Upgrades and Linux Front and Center

**原文链接**: [https://boilingsteam.com/framework-laptop-13-pro-announced/](https://boilingsteam.com/framework-laptop-13-pro-announced/)

生成摘要时出错

---

## 56. How the Tech World Turned Evil

**原文标题**: How the Tech World Turned Evil

**原文链接**: [https://newrepublic.com/article/208876/tech-world-evil-musk-bezos-thiel](https://newrepublic.com/article/208876/tech-world-evil-musk-bezos-thiel)

生成摘要时出错

---

## 57. nowhere: an entire website encoded in a URL

**原文标题**: nowhere: an entire website encoded in a URL

**原文链接**: [https://hostednowhere.com/](https://hostednowhere.com/)

生成摘要时出错

---

## 58. Lambda Calculus Benchmark for AI

**原文标题**: Lambda Calculus Benchmark for AI

**原文链接**: [https://victortaelin.github.io/lambench/](https://victortaelin.github.io/lambench/)

生成摘要时出错

---

## 59. Discret 11, the French TV encryption of the 80s

**原文标题**: Discret 11, the French TV encryption of the 80s

**原文链接**: [https://fabiensanglard.net/discret11/](https://fabiensanglard.net/discret11/)

生成摘要时出错

---

## 60. Familiarity is the enemy: On why Enterprise systems have failed for 60 years

**原文标题**: Familiarity is the enemy: On why Enterprise systems have failed for 60 years

**原文链接**: [https://felixbarbalet.com/familiarity-is-the-enemy/](https://felixbarbalet.com/familiarity-is-the-enemy/)

生成摘要时出错

---

## 61. A quick look at Mythos run on Firefox: too much hype?

**原文标题**: A quick look at Mythos run on Firefox: too much hype?

**原文链接**: [https://xark.es/b/mythos-firefox-150](https://xark.es/b/mythos-firefox-150)

生成摘要时出错

---

## 62. Cosmology with Geometry Nodes

**原文标题**: Cosmology with Geometry Nodes

**原文链接**: [https://www.blender.org/user-stories/cosmology-with-geometry-nodes/](https://www.blender.org/user-stories/cosmology-with-geometry-nodes/)

生成摘要时出错

---

## 63. Anthropic's Claude Desktop App Installs Undisclosed Native Messaging Bridge

**原文标题**: Anthropic's Claude Desktop App Installs Undisclosed Native Messaging Bridge

**原文链接**: [https://letsdatascience.com/news/claude-desktop-installs-preauthorized-browser-extension-mani-4064fb1a](https://letsdatascience.com/news/claude-desktop-installs-preauthorized-browser-extension-mani-4064fb1a)

生成摘要时出错

---

## 64. GitHub Merge Queue Silently Reverted Code

**原文标题**: GitHub Merge Queue Silently Reverted Code

**原文链接**: [https://www.githubstatus.com/incidents/zsg1lk7w13cf](https://www.githubstatus.com/incidents/zsg1lk7w13cf)

生成摘要时出错

---

## 65. A web-based RDP client built with Go WebAssembly and grdp

**原文标题**: A web-based RDP client built with Go WebAssembly and grdp

**原文链接**: [https://github.com/nakagami/grdpwasm](https://github.com/nakagami/grdpwasm)

生成摘要时出错

---

## 66. GPT 5.5 biosafety bounty

**原文标题**: GPT 5.5 biosafety bounty

**原文链接**: [https://openai.com/index/gpt-5-5-bio-bug-bounty/](https://openai.com/index/gpt-5-5-bio-bug-bounty/)

生成摘要时出错

---

## 67. Microsoft offers buyouts up to 7% of US employees

**原文标题**: Microsoft offers buyouts up to 7% of US employees

**原文链接**: [https://techcrunch.com/2026/04/23/microsoft-offers-buyout-for-up-to-7-of-u-s-employees/](https://techcrunch.com/2026/04/23/microsoft-offers-buyout-for-up-to-7-of-u-s-employees/)

生成摘要时出错

---

## 68. Could a Claude Code routine watch my finances?

**原文标题**: Could a Claude Code routine watch my finances?

**原文链接**: [https://driggsby.com/blog/claude-code-routine-watch-my-finances](https://driggsby.com/blog/claude-code-routine-watch-my-finances)

生成摘要时出错

---

## 69. CSS as a Query Language

**原文标题**: CSS as a Query Language

**原文链接**: [https://evdc.me/blog/css-query](https://evdc.me/blog/css-query)

生成摘要时出错

---

## 70. Iran caused more extensive damage to U.S. military bases than publicly known

**原文标题**: Iran caused more extensive damage to U.S. military bases than publicly known

**原文链接**: [https://www.nbcnews.com/world/iran/iran-caused-extensive-damage-us-military-bases-publicly-known-rcna331853](https://www.nbcnews.com/world/iran/iran-caused-extensive-damage-us-military-bases-publicly-known-rcna331853)

生成摘要时出错

---

## 71. Tesla discloses $2B AI hardware company acquisition in filing

**原文标题**: Tesla discloses $2B AI hardware company acquisition in filing

**原文链接**: [https://electrek.co/2026/04/23/tesla-tsla-quietly-discloses-2-billion-ai-hardware-acquisition-10q/](https://electrek.co/2026/04/23/tesla-tsla-quietly-discloses-2-billion-ai-hardware-acquisition-10q/)

生成摘要时出错

---

## 72. Redesigning the Recurse Center application to inspire curious programmers

**原文标题**: Redesigning the Recurse Center application to inspire curious programmers

**原文链接**: [https://www.recurse.com/blog/192-redesigning-the-recurse-center-application](https://www.recurse.com/blog/192-redesigning-the-recurse-center-application)

生成摘要时出错

---

## 73. Jumping into cold water can stop your heart

**原文标题**: Jumping into cold water can stop your heart

**原文链接**: [https://jorgenmelau.substack.com/p/the-first-sixty-seconds](https://jorgenmelau.substack.com/p/the-first-sixty-seconds)

生成摘要时出错

---

## 74. Behind-the-Scenes of MacBook Neo Introduction Video

**原文标题**: Behind-the-Scenes of MacBook Neo Introduction Video

**原文链接**: [https://www.youtube.com/shorts/y4DnsCzJTRQ](https://www.youtube.com/shorts/y4DnsCzJTRQ)

生成摘要时出错

---

## 75. ML supports existence of unrecognized transient astronomical phenomena

**原文标题**: ML supports existence of unrecognized transient astronomical phenomena

**原文链接**: [https://arxiv.org/abs/2604.18799](https://arxiv.org/abs/2604.18799)

生成摘要时出错

---

## 76. 8087 Emulation on 8086 Systems

**原文标题**: 8087 Emulation on 8086 Systems

**原文链接**: [https://www.os2museum.com/wp/learn-something-old-every-day-part-xx-8087-emulation-on-8086-systems/](https://www.os2museum.com/wp/learn-something-old-every-day-part-xx-8087-emulation-on-8086-systems/)

生成摘要时出错

---

## 77. CC-Canary: Detect early signs of regressions in Claude Code

**原文标题**: CC-Canary: Detect early signs of regressions in Claude Code

**原文链接**: [https://github.com/delta-hq/cc-canary](https://github.com/delta-hq/cc-canary)

生成摘要时出错

---

## 78. Physicists revive 1990s laser concept to propose a next-generation atomic clock

**原文标题**: Physicists revive 1990s laser concept to propose a next-generation atomic clock

**原文链接**: [https://phys.org/news/2026-04-physicists-revive-1990s-laser-concept.html](https://phys.org/news/2026-04-physicists-revive-1990s-laser-concept.html)

生成摘要时出错

---

## 79. Show HN: Atomic – Local-first, AI-augmented personal knowledge base

**原文标题**: Show HN: Atomic – Local-first, AI-augmented personal knowledge base

**原文链接**: [https://atomicapp.ai/](https://atomicapp.ai/)

生成摘要时出错

---

## 80. A Collection of Chronic Medical Conditions Common in Autistic and ADHD Adults [pdf] (2023)

**原文标题**: A Collection of Chronic Medical Conditions Common in Autistic and ADHD Adults [pdf] (2023)

**原文链接**: [https://allbrainsbelong.org/wp-content/uploads/2023/08/CLINICIAN-GUIDE-Everything-is-Connected-to-Everything-Project-All-Brains-Belong-VT-8.15.23.pdf](https://allbrainsbelong.org/wp-content/uploads/2023/08/CLINICIAN-GUIDE-Everything-is-Connected-to-Everything-Project-All-Brains-Belong-VT-8.15.23.pdf)

生成摘要时出错

---

## 81. What's missing in the 'agentic' story: a well-defined user agent role

**原文标题**: What's missing in the 'agentic' story: a well-defined user agent role

**原文链接**: [https://www.mnot.net/blog/2026/04/24/agents_as_collective_bargains](https://www.mnot.net/blog/2026/04/24/agents_as_collective_bargains)

生成摘要时出错

---

## 82. Only One Side Will Be the True Successor to MS-DOS – Windows 2.x

**原文标题**: Only One Side Will Be the True Successor to MS-DOS – Windows 2.x

**原文链接**: [https://blisscast.wordpress.com/2026/04/21/windows-2-gui-wonderland-12a/](https://blisscast.wordpress.com/2026/04/21/windows-2-gui-wonderland-12a/)

生成摘要时出错

---

## 83. Netherlands reaches deal to cut reliance on U.S. cloud tech

**原文标题**: Netherlands reaches deal to cut reliance on U.S. cloud tech

**原文链接**: [https://nltimes.nl/2026/04/24/netherlands-reaches-deal-european-cloud-company-decrease-us-tech-reliance](https://nltimes.nl/2026/04/24/netherlands-reaches-deal-european-cloud-company-decrease-us-tech-reliance)

生成摘要时出错

---

## 84. Oxford All Souls College General Examination (2025) [pdf]

**原文标题**: Oxford All Souls College General Examination (2025) [pdf]

**原文链接**: [https://www.asc.ox.ac.uk/sites/default/files/2025-10/General%202025.pdf](https://www.asc.ox.ac.uk/sites/default/files/2025-10/General%202025.pdf)

生成摘要时出错

---

## 85. $8800 house design helps prevent fatal diseases in African children

**原文标题**: $8800 house design helps prevent fatal diseases in African children

**原文链接**: [https://www.science.org/content/article/simple-house-may-help-prevent-multiple-fatal-diseases-african-children](https://www.science.org/content/article/simple-house-may-help-prevent-multiple-fatal-diseases-african-children)

生成摘要时出错

---

## 86. MiniZinc, constraint modelling language solve discrete optimisation problems

**原文标题**: MiniZinc, constraint modelling language solve discrete optimisation problems

**原文链接**: [https://www.minizinc.org](https://www.minizinc.org)

生成摘要时出错

---

## 87. Google investing up to $40B in Anthropic

**原文标题**: Google investing up to $40B in Anthropic

**原文链接**: [https://www.bloomberg.com/news/articles/2026-04-24/google-plans-to-invest-up-to-40-billion-in-anthropic](https://www.bloomberg.com/news/articles/2026-04-24/google-plans-to-invest-up-to-40-billion-in-anthropic)

生成摘要时出错

---

## 88. The Rich and Powerful Want to Live Forever. What If They Could?

**原文标题**: The Rich and Powerful Want to Live Forever. What If They Could?

**原文链接**: [https://www.nytimes.com/2026/04/24/magazine/eternal-life-longevity-world-leaders.html](https://www.nytimes.com/2026/04/24/magazine/eternal-life-longevity-world-leaders.html)

生成摘要时出错

---

## 89. The Digesting Duck: a 1739 automaton that appeared to eat, digest, and defecate

**原文标题**: The Digesting Duck: a 1739 automaton that appeared to eat, digest, and defecate

**原文链接**: [https://en.wikipedia.org/wiki/Digesting_Duck](https://en.wikipedia.org/wiki/Digesting_Duck)

生成摘要时出错

---

## 90. Linux 7.1 Removes Drivers for Bus Mouse Support

**原文标题**: Linux 7.1 Removes Drivers for Bus Mouse Support

**原文链接**: [https://www.phoronix.com/news/Linux-7.1-Input](https://www.phoronix.com/news/Linux-7.1-Input)

生成摘要时出错

---

## 91. Hokusai and Tesselations

**原文标题**: Hokusai and Tesselations

**原文链接**: [https://dl.ndl.go.jp/pid/1899550/1/11/](https://dl.ndl.go.jp/pid/1899550/1/11/)

生成摘要时出错

---

## 92. Show HN: leaf – a terminal Markdown previewer with a GUI-like experience

**原文标题**: Show HN: leaf – a terminal Markdown previewer with a GUI-like experience

**原文链接**: [https://github.com/RivoLink/leaf](https://github.com/RivoLink/leaf)

生成摘要时出错

---

## 93. Do I belong in tech anymore?

**原文标题**: Do I belong in tech anymore?

**原文链接**: [https://ky.fyi/posts/ai-burnout](https://ky.fyi/posts/ai-burnout)

生成摘要时出错

---

## 94. The Surveillance Accountability Act

**原文标题**: The Surveillance Accountability Act

**原文链接**: [https://www.surveillanceaccountability.com](https://www.surveillanceaccountability.com)

生成摘要时出错

---

## 95. Possibility of modifying an image to see without glasses? (2010)

**原文标题**: Possibility of modifying an image to see without glasses? (2010)

**原文链接**: [https://stackoverflow.com/questions/2563471/is-it-possible-to-modify-an-image-so-someone-with-myopia-could-see-it-clearly-wi](https://stackoverflow.com/questions/2563471/is-it-possible-to-modify-an-image-so-someone-with-myopia-could-see-it-clearly-wi)

生成摘要时出错

---

## 96. Escrow Security for iCloud Keychain

**原文标题**: Escrow Security for iCloud Keychain

**原文链接**: [https://support.apple.com/guide/security/escrow-security-for-icloud-keychain-sec3e341e75d/web](https://support.apple.com/guide/security/escrow-security-for-icloud-keychain-sec3e341e75d/web)

生成摘要时出错

---

## 97. Design.md: A format spec for describing a visual identity to coding agents

**原文标题**: Design.md: A format spec for describing a visual identity to coding agents

**原文链接**: [https://github.com/google-labs-code/design.md](https://github.com/google-labs-code/design.md)

生成摘要时出错

---

## 98. HEALPix

**原文标题**: HEALPix

**原文链接**: [https://en.wikipedia.org/wiki/HEALPix](https://en.wikipedia.org/wiki/HEALPix)

生成摘要时出错

---

## 99. Iran war has drained U.S. supplies of critical, costly weapons

**原文标题**: Iran war has drained U.S. supplies of critical, costly weapons

**原文链接**: [https://www.nytimes.com/2026/04/23/us/politics/iran-war-cost-military.html](https://www.nytimes.com/2026/04/23/us/politics/iran-war-cost-military.html)

生成摘要时出错

---

## 100. Stock markets are too high and set to fall, says Bank of England deputy

**原文标题**: Stock markets are too high and set to fall, says Bank of England deputy

**原文链接**: [https://www.bbc.com/news/articles/c75kp1y43lgo](https://www.bbc.com/news/articles/c75kp1y43lgo)

生成摘要时出错

---

