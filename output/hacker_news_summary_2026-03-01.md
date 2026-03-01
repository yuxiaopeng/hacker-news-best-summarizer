# Hacker News 热门文章摘要 (2026-03-01)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 我们不会被分裂

**原文标题**: We Will Not Be Divided

**原文链接**: [https://notdivided.org](https://notdivided.org)

无法访问文章链接。

---

## 2. OpenAI – 如何注销账户

**原文标题**: OpenAI – How to delete your account

**原文链接**: [https://help.openai.com/en/articles/6378407-how-to-delete-your-account](https://help.openai.com/en/articles/6378407-how-to-delete-your-account)

要删除您的OpenAI账户，用户通常会遵循一个简单的流程。首先，登录您的OpenAI账户。然后，点击屏幕右下角的“帮助”气泡图标，并选择“向我们发送消息”。在聊天窗口中，输入“删除我的账户”，并在系统提示时确认您的电子邮件地址以完成请求。

如果您无法登录，仍然可以通过访问 help.openai.com，点击聊天气泡，选择“账户删除”，并提供与账户关联的电子邮件地址来请求删除。

需要特别指出的是，账户删除是永久且不可逆的。账户一旦删除，所有相关数据，包括过去的对话和API使用记录，都将从OpenAI的系统中永久移除。该账户无法被重新激活，并且用于已删除账户的电子邮件地址可能会在删除后立即被暂时阻止用于创建新账户。

---

## 3. Microgpt

**原文标题**: Microgpt

**原文链接**: [http://karpathy.github.io/2026/02/12/microgpt/](http://karpathy.github.io/2026/02/12/microgpt/)

"Microgpt" is a 200-line, single-file Python project by Andrej Karpathy, designed to train and infer a GPT model from scratch with no external dependencies. It consolidates concepts from earlier projects like micrograd and makemore, aiming to simplify LLMs to their essential algorithmic components.

The project includes a dataset of 32,000 names (from `names.txt`), which the model learns to generate. It uses a character-level tokenizer, assigning unique integer IDs to each character (a-z) and a special Beginning of Sequence (BOS) token, resulting in a vocabulary of 27 tokens.

A custom autograd engine, `Value`, is implemented to handle automatic differentiation. This `Value` class wraps scalar numbers, records computation graphs, and uses the chain rule for backpropagation, allowing gradients to be calculated for all parameters—algorithmically similar to PyTorch's `backward()` but for scalars.

The model parameters, totaling 4,192 for this tiny GPT, are initialized randomly and organized into embedding tables, attention, and MLP weights. The architecture is a simplified GPT-2, utilizing `linear` transformations, `softmax` for probability distributions, and `rmsnorm` for stabilization. It incorporates token and position embeddings, and a multi-head attention block (though the description cuts off before the full MLP detail). The ultimate goal is for the model to "hallucinate" plausible new names based on learned patterns.

---

## 4. OpenAI 同意与战争部在其机密网络中部署模型。

**原文标题**: OpenAI agrees with Dept. of War to deploy models in their classified network

**原文链接**: [https://twitter.com/sama/status/2027578652477821175](https://twitter.com/sama/status/2027578652477821175)

所提供的文本在其标题中指出了一项重大进展：“OpenAI 同意与战争部合作，在其机密网络中部署模型。”这表明人工智能公司OpenAI已与某个军事或国防部门达成协议，将其AI模型集成到敏感的机密政府网络中。

然而，“文章”的主体内容无法访问。取而代之的是，显示的内容是来自x.com（原Twitter）的一条技术错误消息，声称“此浏览器中JavaScript已禁用”，并指示用户启用JavaScript或切换到受支持的浏览器来查看内容。

因此，关于协议条款、将部署的具体模型类型、该决定的理由或任何潜在影响的更多细节，都无法从所提供的文本中进行总结。唯一实质性的信息来自标题，而内容本身是一个平台错误消息。

---

## 5. 我指示战争部将Anthropic认定为供应链风险。

**原文标题**: I am directing the Department of War to designate Anthropic a supply-chain risk

**原文链接**: [https://twitter.com/secwar/status/2027507717469049070](https://twitter.com/secwar/status/2027507717469049070)

文章标题显示，一位未具名的权威人士指示战争部将人工智能公司Anthropic指定为供应链风险。然而，文章的实际内容却无法获取。所提供的文本仅包含一条来自x.com（原Twitter）的技术错误信息，指出浏览器中JavaScript已禁用。此信息阻止了任何内容的显示，并指示用户启用JavaScript或切换到受支持的浏览器以继续使用该平台。因此，尽管标题概述了一项重要的政策决定，但有关这项指定的细节、理由或任何讨论在所提供的文本中完全缺失。

---

## 6. 美国和以色列对伊朗发动了重大袭击。

**原文标题**: The United States and Israel have launched a major attack on Iran

**原文链接**: [https://www.cnn.com/2026/02/28/middleeast/israel-attack-iran-intl-hnk](https://www.cnn.com/2026/02/28/middleeast/israel-attack-iran-intl-hnk)

生成摘要时出错

---

## 7. 战争部长皮特·赫格塞斯言论声明

**原文标题**: Statement on the comments from Secretary of War Pete Hegseth

**原文链接**: [https://www.anthropic.com/news/statement-comments-secretary-war](https://www.anthropic.com/news/statement-comments-secretary-war)

2026年2月27日，战争部长皮特·赫格塞斯宣布，他打算将Anthropic公司指定为“供应链风险”。此举源于Anthropic公司在经过数月谈判后，仍拒绝允许其人工智能模型Claude被用于对美国人进行大规模国内监控或开发全自主武器。

Anthropic公司表示，它支持所有其他合法的国家安全人工智能用途，但坚持这两项例外，原因至关重要：当前的尖端人工智能模型在全自主武器方面不够可靠，对作战人员和普通民众构成风险；大规模国内监控侵犯了基本权利。

Anthropic公司认为，此举是前所未有的、在法律上站不住脚的行动，通常只针对美国的对手，而非自2024年6月以来一直支持美国作战人员的一家美国公司。他们计划在法庭上挑战任何此类指定，认为这开创了一个危险的先例。

Anthropic公司澄清，部长声称的广泛限制缺乏法定授权。如果获得通过，此项指定将仅影响战争部承包商在特定战争部合同工作中对Claude的使用。个人客户以及Claude的商业合同（通过API、claude.ai等）将完全不受影响。Anthropic公司重申其对客户的承诺，以及其反对恐吓的立场。

---

## 8. 如何取消我的ChatGPT订阅？

**原文标题**: How do I cancel my ChatGPT subscription?

**原文链接**: [https://help.openai.com/en/articles/7232927-how-do-i-cancel-my-chatgpt-subscription](https://help.openai.com/en/articles/7232927-how-do-i-cancel-my-chatgpt-subscription)

OpenAI帮助文章详细说明了如何取消ChatGPT Plus订阅，具体操作说明会因订阅是通过网页、iOS应用还是Android应用启动而异。

对于**网页端订阅**，用户需要登录chat.openai.com，点击左下角的“我的计划”，然后点击“管理我的订阅”。此操作会将他们重定向到Stripe账单门户，在那里他们可以点击“取消计划”并确认取消。

**iOS应用订阅**必须通过Apple的App Store设置取消。用户应前往设备的“设置”，点击顶部的Apple ID，选择“订阅”，找到他们的ChatGPT订阅，然后点击“取消订阅”。

对于**Android应用订阅**，取消操作通过Google Play商店完成。用户打开Play商店应用，点击个人资料图标，进入“付款与订阅”，然后是“订阅”，找到他们的ChatGPT订阅，然后点击“取消订阅”。

一旦取消，订阅在当前计费周期结束前仍然有效，且不会再产生任何费用。OpenAI不提供部分订阅周期的退款。当前计费周期结束后，用户将恢复使用免费的ChatGPT服务，而他们的聊天记录仍然可以访问。

---

## 9. The whole thing was a scam

**原文标题**: The whole thing was a scam

**原文链接**: [https://garymarcus.substack.com/p/the-whole-thing-was-scam](https://garymarcus.substack.com/p/the-whole-thing-was-scam)

In the article "The whole thing was a scam," Gary Marcus critically examines the recent hype surrounding large language models (LLMs) and artificial intelligence, particularly following Sam Altman's testimony to Congress. Marcus argues that the narrative presented by Altman and others—suggesting an imminent threat of superintelligent AI needing urgent regulation—is a carefully constructed "bait-and-switch" to benefit companies like OpenAI.

Marcus posits that while current LLMs are impressive in certain tasks, they lack true understanding, common sense, and reliability, frequently "hallucinating" information. He points out that the real threats posed by current AI are more mundane but significant: job displacement, bias amplification, and the spread of misinformation, issues that existing regulatory frameworks could largely address. The "existential threat" narrative, he contends, distracts from these concrete problems and serves to create a new regulatory body that would primarily protect the market positions of leading AI firms by imposing high barriers to entry for competitors.

He suggests that the industry is trying to secure a future where they maintain control and avoid more stringent, existing forms of regulation while appearing to act responsibly. Marcus concludes that the true "scam" is the manufactured panic over an imagined future superintelligence, designed to manipulate public opinion and policy for corporate gain, rather than genuinely address the immediate challenges and limitations of current AI technology.

---

## 10. We do not think Anthropic should be designated as a supply chain risk

**原文标题**: We do not think Anthropic should be designated as a supply chain risk

**原文链接**: [https://twitter.com/OpenAI/status/2027846016423321831](https://twitter.com/OpenAI/status/2027846016423321831)

生成摘要时出错

---

## 11. Obsidian Sync now has a headless client

**原文标题**: Obsidian Sync now has a headless client

**原文链接**: [https://help.obsidian.md/sync/headless](https://help.obsidian.md/sync/headless)

生成摘要时出错

---

## 12. 将 Claude 代码上下文消耗降低 98% 的 MCP 服务器

**原文标题**: MCP server that reduces Claude Code context consumption by 98%

**原文链接**: [https://mksg.lu/blog/context-mode](https://mksg.lu/blog/context-mode)

生成摘要时出错

---

## 13. Croatia declared free of landmines after 31 years

**原文标题**: Croatia declared free of landmines after 31 years

**原文链接**: [https://glashrvatske.hrt.hr/en/domestic/croatia-declared-free-of-landmines-after-31-years-12593533](https://glashrvatske.hrt.hr/en/domestic/croatia-declared-free-of-landmines-after-31-years-12593533)

生成摘要时出错

---

## 14. Cognitive Debt: When Velocity Exceeds Comprehension

**原文标题**: Cognitive Debt: When Velocity Exceeds Comprehension

**原文链接**: [https://www.rockoder.com/beyondthecode/cognitive-debt-when-velocity-exceeds-comprehension/](https://www.rockoder.com/beyondthecode/cognitive-debt-when-velocity-exceeds-comprehension/)

生成摘要时出错

---

## 15. Leaving Google has actively improved my life

**原文标题**: Leaving Google has actively improved my life

**原文链接**: [https://pseudosingleton.com/leaving-google-improved-my-life/](https://pseudosingleton.com/leaving-google-improved-my-life/)

生成摘要时出错

---

## 16. Switch to Claude without starting over

**原文标题**: Switch to Claude without starting over

**原文链接**: [https://claude.com/import-memory](https://claude.com/import-memory)

生成摘要时出错

---

## 17. Qwen3.5 122B and 35B models offer Sonnet 4.5 performance on local computers

**原文标题**: Qwen3.5 122B and 35B models offer Sonnet 4.5 performance on local computers

**原文链接**: [https://venturebeat.com/technology/alibabas-new-open-source-qwen3-5-medium-models-offer-sonnet-4-5-performance](https://venturebeat.com/technology/alibabas-new-open-source-qwen3-5-medium-models-offer-sonnet-4-5-performance)

生成摘要时出错

---

## 18. Iran's Ayatollah Ali Khamenei is killed in Israeli strike, ending 36-year rule

**原文标题**: Iran's Ayatollah Ali Khamenei is killed in Israeli strike, ending 36-year rule

**原文链接**: [https://www.npr.org/2026/02/28/1123499337/iran-israel-ayatollah-ali-khamenei-killed](https://www.npr.org/2026/02/28/1123499337/iran-israel-ayatollah-ali-khamenei-killed)

生成摘要时出错

---

## 19. Ghostty – Terminal Emulator

**原文标题**: Ghostty – Terminal Emulator

**原文链接**: [https://ghostty.org/docs](https://ghostty.org/docs)

生成摘要时出错

---

## 20. AI Made Writing Code Easier. It Made Being an Engineer Harder

**原文标题**: AI Made Writing Code Easier. It Made Being an Engineer Harder

**原文链接**: [https://www.ivanturkovic.com/2026/02/25/ai-made-writing-code-easier-engineering-harder/](https://www.ivanturkovic.com/2026/02/25/ai-made-writing-code-easier-engineering-harder/)

生成摘要时出错

---

## 21. Our Agreement with the Department of War

**原文标题**: Our Agreement with the Department of War

**原文链接**: [https://openai.com/index/our-agreement-with-the-department-of-war](https://openai.com/index/our-agreement-with-the-department-of-war)

生成摘要时出错

---

## 22. I built a demo of what AI chat will look like when it's "free" and ad-supported

**原文标题**: I built a demo of what AI chat will look like when it's "free" and ad-supported

**原文链接**: [https://99helpers.com/tools/ad-supported-chat](https://99helpers.com/tools/ad-supported-chat)

生成摘要时出错

---

## 23. The Windows 95 user interface: A case study in usability engineering (1996)

**原文标题**: The Windows 95 user interface: A case study in usability engineering (1996)

**原文链接**: [https://dl.acm.org/doi/fullHtml/10.1145/238386.238611](https://dl.acm.org/doi/fullHtml/10.1145/238386.238611)

生成摘要时出错

---

## 24. Don't trust AI agents

**原文标题**: Don't trust AI agents

**原文链接**: [https://nanoclaw.dev/blog/nanoclaw-security-model](https://nanoclaw.dev/blog/nanoclaw-security-model)

生成摘要时出错

---

## 25. President Trump bans Anthropic from use in government systems

**原文标题**: President Trump bans Anthropic from use in government systems

**原文链接**: [https://www.npr.org/2026/02/27/nx-s1-5729118/trump-anthropic-pentagon-openai-ai-weapons-ban](https://www.npr.org/2026/02/27/nx-s1-5729118/trump-anthropic-pentagon-openai-ai-weapons-ban)

生成摘要时出错

---

## 26. What AI coding costs you

**原文标题**: What AI coding costs you

**原文链接**: [https://tomwojcik.com/posts/2026-02-15/finding-the-right-amount-of-ai/](https://tomwojcik.com/posts/2026-02-15/finding-the-right-amount-of-ai/)

生成摘要时出错

---

## 27. Decision trees – the unreasonable power of nested decision rules

**原文标题**: Decision trees – the unreasonable power of nested decision rules

**原文链接**: [https://mlu-explain.github.io/decision-tree/](https://mlu-explain.github.io/decision-tree/)

生成摘要时出错

---

## 28. Block the “Upgrade to Tahoe” Alerts

**原文标题**: Block the “Upgrade to Tahoe” Alerts

**原文链接**: [https://robservatory.com/block-the-upgrade-to-tahoe-alerts-and-system-settings-indicator/](https://robservatory.com/block-the-upgrade-to-tahoe-alerts-and-system-settings-indicator/)

生成摘要时出错

---

## 29. Techno‑feudal elite are attempting to build a twenty‑first‑century fascist state

**原文标题**: Techno‑feudal elite are attempting to build a twenty‑first‑century fascist state

**原文链接**: [https://collapseofindustrialcivilization.com/2026/02/16/americas-oligarchic-techno-feudal-elite-are-attempting-to-build-a-twenty-first-century-fascist-state/](https://collapseofindustrialcivilization.com/2026/02/16/americas-oligarchic-techno-feudal-elite-are-attempting-to-build-a-twenty-first-century-fascist-state/)

生成摘要时出错

---

## 30. OpenAI fires an employee for prediction market insider trading

**原文标题**: OpenAI fires an employee for prediction market insider trading

**原文链接**: [https://www.wired.com/story/openai-fires-employee-insider-trading-polymarket-kalshi/](https://www.wired.com/story/openai-fires-employee-insider-trading-polymarket-kalshi/)

生成摘要时出错

---

## 31. Rob Grant, creator of Red Dwarf, has died

**原文标题**: Rob Grant, creator of Red Dwarf, has died

**原文链接**: [https://www.beyondthejoke.co.uk/content/17193/red-dwarf-rob-grant](https://www.beyondthejoke.co.uk/content/17193/red-dwarf-rob-grant)

生成摘要时出错

---

## 32. U.S. and Israel Conduct Strikes on Iran

**原文标题**: U.S. and Israel Conduct Strikes on Iran

**原文链接**: [https://www.nytimes.com/live/2026/02/28/world/iran-strikes-trump](https://www.nytimes.com/live/2026/02/28/world/iran-strikes-trump)

生成摘要时出错

---

## 33. Show HN: Now I Get It – Translate scientific papers into interactive webpages

**原文标题**: Show HN: Now I Get It – Translate scientific papers into interactive webpages

**原文链接**: [https://nowigetit.us](https://nowigetit.us)

生成摘要时出错

---

## 34. Don't use passkeys for encrypting user data

**原文标题**: Don't use passkeys for encrypting user data

**原文链接**: [https://blog.timcappalli.me/p/passkeys-prf-warning/](https://blog.timcappalli.me/p/passkeys-prf-warning/)

生成摘要时出错

---

## 35. Addressing Antigravity Bans and Reinstating Access

**原文标题**: Addressing Antigravity Bans and Reinstating Access

**原文链接**: [https://github.com/google-gemini/gemini-cli/discussions/20632](https://github.com/google-gemini/gemini-cli/discussions/20632)

生成摘要时出错

---

## 36. Unsloth Dynamic 2.0 GGUFs

**原文标题**: Unsloth Dynamic 2.0 GGUFs

**原文链接**: [https://unsloth.ai/docs/basics/unsloth-dynamic-2.0-ggufs](https://unsloth.ai/docs/basics/unsloth-dynamic-2.0-ggufs)

生成摘要时出错

---

## 37. MinIO Is Dead, Long Live MinIO

**原文标题**: MinIO Is Dead, Long Live MinIO

**原文链接**: [https://blog.vonng.com/en/db/minio-resurrect/](https://blog.vonng.com/en/db/minio-resurrect/)

生成摘要时出错

---

## 38. Claude becomes number one app on the U.S. App Store

**原文标题**: Claude becomes number one app on the U.S. App Store

**原文链接**: [https://apps.apple.com/us/iphone/charts](https://apps.apple.com/us/iphone/charts)

生成摘要时出错

---

## 39. Verified Spec-Driven Development (VSDD)

**原文标题**: Verified Spec-Driven Development (VSDD)

**原文链接**: [https://gist.github.com/dollspace-gay/d8d3bc3ecf4188df049d7a4726bb2a00](https://gist.github.com/dollspace-gay/d8d3bc3ecf4188df049d7a4726bb2a00)

生成摘要时出错

---

## 40. 10-202: Introduction to Modern AI (CMU)

**原文标题**: 10-202: Introduction to Modern AI (CMU)

**原文链接**: [https://modernaicourse.org](https://modernaicourse.org)

生成摘要时出错

---

## 41. Let's discuss sandbox isolation

**原文标题**: Let's discuss sandbox isolation

**原文链接**: [https://www.shayon.dev/post/2026/52/lets-discuss-sandbox-isolation/](https://www.shayon.dev/post/2026/52/lets-discuss-sandbox-isolation/)

生成摘要时出错

---

## 42. Rust is just a tool

**原文标题**: Rust is just a tool

**原文链接**: [https://lewiscampbell.tech/blog/260204.html](https://lewiscampbell.tech/blog/260204.html)

生成摘要时出错

---

## 43. Samsung Galaxy update removes Android recovery menu tools, including sideloading

**原文标题**: Samsung Galaxy update removes Android recovery menu tools, including sideloading

**原文链接**: [https://9to5google.com/2026/02/27/samsung-galaxy-update-android-recovery-menu-removed/](https://9to5google.com/2026/02/27/samsung-galaxy-update-android-recovery-menu-removed/)

生成摘要时出错

---

## 44. "Cancel ChatGPT" movement goes mainstream after OpenAI closes deal with U.S. Dow

**原文标题**: "Cancel ChatGPT" movement goes mainstream after OpenAI closes deal with U.S. Dow

**原文链接**: [https://www.windowscentral.com/artificial-intelligence/cancel-chatgpt-movement-goes-mainstream-after-openai-closes-deal-with-u-s-department-of-war-as-anthropic-refuses-to-surveil-american-citizens](https://www.windowscentral.com/artificial-intelligence/cancel-chatgpt-movement-goes-mainstream-after-openai-closes-deal-with-u-s-department-of-war-as-anthropic-refuses-to-surveil-american-citizens)

生成摘要时出错

---

## 45. Trump orders US Government to cut ties with Anthropic

**原文标题**: Trump orders US Government to cut ties with Anthropic

**原文链接**: [https://abcnews.com/Politics/anthropic-latest-pentagon-contract-bar-ai-autonomous-weapons/story?id=130558898](https://abcnews.com/Politics/anthropic-latest-pentagon-contract-bar-ai-autonomous-weapons/story?id=130558898)

生成摘要时出错

---

## 46. OpenAI reaches deal to deploy AI models on U.S. DoW classified network

**原文标题**: OpenAI reaches deal to deploy AI models on U.S. DoW classified network

**原文链接**: [https://www.reuters.com/business/openai-reaches-deal-deploy-ai-models-us-department-war-classified-network-2026-02-28/](https://www.reuters.com/business/openai-reaches-deal-deploy-ai-models-us-department-war-classified-network-2026-02-28/)

生成摘要时出错

---

## 47. The Future of AI

**原文标题**: The Future of AI

**原文链接**: [https://lucijagregov.com/2026/02/26/the-future-of-ai/](https://lucijagregov.com/2026/02/26/the-future-of-ai/)

生成摘要时出错

---

## 48. Ape Coding

**原文标题**: Ape Coding

**原文链接**: [https://rsaksida.com/blog/ape-coding/](https://rsaksida.com/blog/ape-coding/)

生成摘要时出错

---

## 49. Anthropic says it will challenge Pentagon supply chain risk designation in court

**原文标题**: Anthropic says it will challenge Pentagon supply chain risk designation in court

**原文链接**: [https://www.reuters.com/world/us/anthropic-says-it-will-challenge-pentagons-supply-chain-risk-designation-court-2026-02-28/](https://www.reuters.com/world/us/anthropic-says-it-will-challenge-pentagons-supply-chain-risk-designation-court-2026-02-28/)

生成摘要时出错

---

## 50. Pentagon chief blocks officers from Ivy League schools and top universities

**原文标题**: Pentagon chief blocks officers from Ivy League schools and top universities

**原文链接**: [https://fortune.com/2026/02/28/pentagon-officer-education-ivy-league-schools-universities-partners-ai-space/](https://fortune.com/2026/02/28/pentagon-officer-education-ivy-league-schools-universities-partners-ai-space/)

生成摘要时出错

---

## 51. New iron nanomaterial wipes out cancer cells without harming healthy tissue

**原文标题**: New iron nanomaterial wipes out cancer cells without harming healthy tissue

**原文链接**: [https://www.sciencedaily.com/releases/2026/02/260228093456.htm](https://www.sciencedaily.com/releases/2026/02/260228093456.htm)

生成摘要时出错

---

## 52. Qt45: A small polymerase ribozyme that can synthesize itself

**原文标题**: Qt45: A small polymerase ribozyme that can synthesize itself

**原文链接**: [https://www.science.org/doi/10.1126/science.adt2760](https://www.science.org/doi/10.1126/science.adt2760)

生成摘要时出错

---

## 53. Bootc and OSTree: Modernizing Linux System Deployment

**原文标题**: Bootc and OSTree: Modernizing Linux System Deployment

**原文链接**: [https://a-cup-of.coffee/blog/ostree-bootc/](https://a-cup-of.coffee/blog/ostree-bootc/)

生成摘要时出错

---

## 54. Flightradar24 for Ships

**原文标题**: Flightradar24 for Ships

**原文链接**: [https://atlas.flexport.com/](https://atlas.flexport.com/)

生成摘要时出错

---

## 55. Cash issuing terminals

**原文标题**: Cash issuing terminals

**原文链接**: [https://computer.rip/2026-02-27-ibm-atm.html](https://computer.rip/2026-02-27-ibm-atm.html)

生成摘要时出错

---

## 56. US and Israel carrying out strikes against Iran

**原文标题**: US and Israel carrying out strikes against Iran

**原文链接**: [https://www.cnn.com/world/live-news/israel-iran-attack-02-28-26-hnk-intl](https://www.cnn.com/world/live-news/israel-iran-attack-02-28-26-hnk-intl)

生成摘要时出错

---

## 57. Why is the first C++ (m)allocation always 72 KB?

**原文标题**: Why is the first C++ (m)allocation always 72 KB?

**原文链接**: [https://joelsiks.com/posts/cpp-emergency-pool-72kb-allocation/](https://joelsiks.com/posts/cpp-emergency-pool-72kb-allocation/)

生成摘要时出错

---

## 58. AI is making junior devs useless

**原文标题**: AI is making junior devs useless

**原文链接**: [https://beabetterdev.com/2026/03/01/ai-is-making-junior-devs-useless/](https://beabetterdev.com/2026/03/01/ai-is-making-junior-devs-useless/)

生成摘要时出错

---

## 59. Just two days of oatmeal cut bad cholesterol by 10%

**原文标题**: Just two days of oatmeal cut bad cholesterol by 10%

**原文链接**: [https://www.sciencedaily.com/releases/2026/02/260225081217.htm](https://www.sciencedaily.com/releases/2026/02/260225081217.htm)

生成摘要时出错

---

## 60. Timeline: Anthropic, OpenAI, and U.S. Government

**原文标题**: Timeline: Anthropic, OpenAI, and U.S. Government

**原文链接**: [https://anthropic-timeline.vercel.app](https://anthropic-timeline.vercel.app)

生成摘要时出错

---

## 61. The Robotic Dexterity Deadlock

**原文标题**: The Robotic Dexterity Deadlock

**原文链接**: [https://www.origami-robotics.com/blog/dexterity-deadlocks.html](https://www.origami-robotics.com/blog/dexterity-deadlocks.html)

生成摘要时出错

---

## 62. When does MCP make sense vs CLI?

**原文标题**: When does MCP make sense vs CLI?

**原文链接**: [https://ejholmes.github.io/2026/02/28/mcp-is-dead-long-live-the-cli.html](https://ejholmes.github.io/2026/02/28/mcp-is-dead-long-live-the-cli.html)

生成摘要时出错

---

## 63. The Life Cycle of Money

**原文标题**: The Life Cycle of Money

**原文链接**: [https://doap.metal.bohyen.space/blog/post/complete-life-cycle-of-money/](https://doap.metal.bohyen.space/blog/post/complete-life-cycle-of-money/)

生成摘要时出错

---

## 64. Trump orders federal agencies to stop using Anthropic AI tech 'immediately'

**原文标题**: Trump orders federal agencies to stop using Anthropic AI tech 'immediately'

**原文链接**: [https://www.cnbc.com/2026/02/27/trump-anthropic-ai-pentagon.html](https://www.cnbc.com/2026/02/27/trump-anthropic-ai-pentagon.html)

生成摘要时出错

---

## 65. Khamenei Dead

**原文标题**: Khamenei Dead

**原文链接**: [https://twitter.com/BarakRavid/status/2027830773328302396](https://twitter.com/BarakRavid/status/2027830773328302396)

生成摘要时出错

---

## 66. Why XML Tags Are So Fundamental to Claude

**原文标题**: Why XML Tags Are So Fundamental to Claude

**原文链接**: [https://glthr.com/XML-fundamental-to-Claude](https://glthr.com/XML-fundamental-to-Claude)

生成摘要时出错

---

## 67. Running a One Trillion-Parameter LLM Locally on AMD Ryzen AI Max+ Cluster

**原文标题**: Running a One Trillion-Parameter LLM Locally on AMD Ryzen AI Max+ Cluster

**原文链接**: [https://www.amd.com/en/developer/resources/technical-articles/2026/how-to-run-a-one-trillion-parameter-llm-locally-an-amd.html](https://www.amd.com/en/developer/resources/technical-articles/2026/how-to-run-a-one-trillion-parameter-llm-locally-an-amd.html)

生成摘要时出错

---

## 68. Emuko: Fast RISC-V emulator written in Rust, boots Linux

**原文标题**: Emuko: Fast RISC-V emulator written in Rust, boots Linux

**原文链接**: [https://github.com/wkoszek/emuko](https://github.com/wkoszek/emuko)

生成摘要时出错

---

## 69. Building a Minimal Transformer for 10-digit Addition

**原文标题**: Building a Minimal Transformer for 10-digit Addition

**原文链接**: [https://alexlitzenberger.com/blog/post.html?post=/building_a_minimal_transformer_for_10_digit_addition](https://alexlitzenberger.com/blog/post.html?post=/building_a_minimal_transformer_for_10_digit_addition)

生成摘要时出错

---

## 70. Altman says OpenAI agrees with Anthropic's red lines in Pentagon dispute

**原文标题**: Altman says OpenAI agrees with Anthropic's red lines in Pentagon dispute

**原文链接**: [https://thehill.com/policy/technology/5758898-altman-backs-anthropic-pentagon-stand/](https://thehill.com/policy/technology/5758898-altman-backs-anthropic-pentagon-stand/)

生成摘要时出错

---

## 71. Trump Bans Anthropic from All US Federal Agencies

**原文标题**: Trump Bans Anthropic from All US Federal Agencies

**原文链接**: [https://twitter.com/WhiteHouse/status/2027497719678255148](https://twitter.com/WhiteHouse/status/2027497719678255148)

生成摘要时出错

---

## 72. Show HN: Xmloxide – an agent-made Rust replacement for libxml2

**原文标题**: Show HN: Xmloxide – an agent-made Rust replacement for libxml2

**原文链接**: [https://github.com/jonwiggins/xmloxide](https://github.com/jonwiggins/xmloxide)

生成摘要时出错

---

## 73. Latency numbers every programmer should know

**原文标题**: Latency numbers every programmer should know

**原文链接**: [https://cheat.sh/latency](https://cheat.sh/latency)

生成摘要时出错

---

## 74. The most-seen UI on the internet? Redesigning turnstile and challenge pages

**原文标题**: The most-seen UI on the internet? Redesigning turnstile and challenge pages

**原文链接**: [https://blog.cloudflare.com/the-most-seen-ui-on-the-internet-redesigning-turnstile-and-challenge-pages/](https://blog.cloudflare.com/the-most-seen-ui-on-the-internet-redesigning-turnstile-and-challenge-pages/)

生成摘要时出错

---

## 75. Show HN: SplatHash – A lightweight alternative to BlurHash and ThumbHash

**原文标题**: Show HN: SplatHash – A lightweight alternative to BlurHash and ThumbHash

**原文链接**: [https://github.com/junevm/splathash](https://github.com/junevm/splathash)

生成摘要时出错

---

## 76. Inferring car movement patterns from passive TPMS measurements

**原文标题**: Inferring car movement patterns from passive TPMS measurements

**原文链接**: [https://dspace.networks.imdea.org/handle/20.500.12761/2011](https://dspace.networks.imdea.org/handle/20.500.12761/2011)

生成摘要时出错

---

## 77. GitHub Copilot CLI downloads and executes malware

**原文标题**: GitHub Copilot CLI downloads and executes malware

**原文链接**: [https://www.promptarmor.com/resources/github-copilot-cli-downloads-and-executes-malware](https://www.promptarmor.com/resources/github-copilot-cli-downloads-and-executes-malware)

生成摘要时出错

---

## 78. Please do not use auto-scrolling content on the web and in applications

**原文标题**: Please do not use auto-scrolling content on the web and in applications

**原文链接**: [https://cerovac.com/a11y/2026/01/please-do-not-use-auto-scrolling-content-on-the-web-and-in-applications/](https://cerovac.com/a11y/2026/01/please-do-not-use-auto-scrolling-content-on-the-web-and-in-applications/)

生成摘要时出错

---

## 79. Customer Update on Simplenote

**原文标题**: Customer Update on Simplenote

**原文链接**: [https://forums.simplenote.com/forums/topic/customer-update-on-simplenote/?view=all](https://forums.simplenote.com/forums/topic/customer-update-on-simplenote/?view=all)

生成摘要时出错

---

## 80. Why consumer choice is stripped away and how the tech industry profits from it

**原文标题**: Why consumer choice is stripped away and how the tech industry profits from it

**原文链接**: [https://fireborn.mataroa.blog/blog/because-fuck-you-why-consumer-choice-is-being-stripped-away-and-how-the-tech-industry-profits-from-it/](https://fireborn.mataroa.blog/blog/because-fuck-you-why-consumer-choice-is-being-stripped-away-and-how-the-tech-industry-profits-from-it/)

生成摘要时出错

---

## 81. Show HN: Decided to play god this morning, so I built an agent civilisation

**原文标题**: Show HN: Decided to play god this morning, so I built an agent civilisation

**原文链接**: [https://github.com/nocodemf/werld](https://github.com/nocodemf/werld)

生成摘要时出错

---

## 82. Iran agreed zero enriched uranium, and israel immediately bombs Tehran

**原文标题**: Iran agreed zero enriched uranium, and israel immediately bombs Tehran

**原文链接**: [https://twitter.com/muhammadshehad2/status/2027645609621033376](https://twitter.com/muhammadshehad2/status/2027645609621033376)

生成摘要时出错

---

## 83. "Tonight, we reached an agreement with the Dept. of War to deploy our models"

**原文标题**: "Tonight, we reached an agreement with the Dept. of War to deploy our models"

**原文链接**: [https://twitter.com/sama/status/2027578508042723599](https://twitter.com/sama/status/2027578508042723599)

生成摘要时出错

---

## 84. The Science of Detecting LLM-Generated Text (2024)

**原文标题**: The Science of Detecting LLM-Generated Text (2024)

**原文链接**: [https://dl.acm.org/doi/10.1145/3624725](https://dl.acm.org/doi/10.1145/3624725)

生成摘要时出错

---

## 85. Anthropic refuses to bend to Pentagon on AI safeguards as dispute nears deadline

**原文标题**: Anthropic refuses to bend to Pentagon on AI safeguards as dispute nears deadline

**原文链接**: [https://apnews.com/article/anthropic-pentagon-ai-hegseth-dario-amodei-b72d1894bc842d9acf026df3867bee8a](https://apnews.com/article/anthropic-pentagon-ai-hegseth-dario-amodei-b72d1894bc842d9acf026df3867bee8a)

生成摘要时出错

---

## 86. US Military says 3 service members have been killed

**原文标题**: US Military says 3 service members have been killed

**原文链接**: [https://apnews.com/live/us-israel-strikes-iran-khamenei-03-01-2026](https://apnews.com/live/us-israel-strikes-iran-khamenei-03-01-2026)

生成摘要时出错

---

## 87. 4,500 Physicians Agree (About Bacon)

**原文标题**: 4,500 Physicians Agree (About Bacon)

**原文链接**: [https://machielreyneke.com/blog/persuasion/](https://machielreyneke.com/blog/persuasion/)

生成摘要时出错

---

## 88. The Lancet: Robert F Kennedy Jr: 1 year of failure

**原文标题**: The Lancet: Robert F Kennedy Jr: 1 year of failure

**原文链接**: [https://www.thelancet.com/journals/lancet/article/PIIS0140-6736(26)00414-9/fulltext](https://www.thelancet.com/journals/lancet/article/PIIS0140-6736(26)00414-9/fulltext)

生成摘要时出错

---

## 89. Show HN: SQLite for Rivet Actors – one database per agent, tenant, or document

**原文标题**: Show HN: SQLite for Rivet Actors – one database per agent, tenant, or document

**原文链接**: [https://github.com/rivet-dev/rivet](https://github.com/rivet-dev/rivet)

生成摘要时出错

---

## 90. Anthropic's Claude rises to No. 2 in the App Store following Pentagon dispute

**原文标题**: Anthropic's Claude rises to No. 2 in the App Store following Pentagon dispute

**原文链接**: [https://techcrunch.com/2026/02/28/anthropics-claude-rises-to-no-2-in-the-app-store-following-pentagon-dispute/](https://techcrunch.com/2026/02/28/anthropics-claude-rises-to-no-2-in-the-app-store-following-pentagon-dispute/)

生成摘要时出错

---

## 91. Otters as Bioindicators of Estuarine Health

**原文标题**: Otters as Bioindicators of Estuarine Health

**原文链接**: [https://emt.pensoft.net/article/185117/](https://emt.pensoft.net/article/185117/)

生成摘要时出错

---

## 92. Monitor the Situation

**原文标题**: Monitor the Situation

**原文链接**: [https://monitor-the-situation.com/middle-east](https://monitor-the-situation.com/middle-east)

生成摘要时出错

---

## 93. Claude just jumped to #2 on the iOS App Store

**原文标题**: Claude just jumped to #2 on the iOS App Store

**原文链接**: [https://xcancel.com/search?f=tweets&q=2027614403693318348](https://xcancel.com/search?f=tweets&q=2027614403693318348)

生成摘要时出错

---

## 94. Trump Orders Government to Stop Using Anthropic After Pentagon Standoff

**原文标题**: Trump Orders Government to Stop Using Anthropic After Pentagon Standoff

**原文链接**: [https://www.nytimes.com/2026/02/27/us/politics/anthropic-military-ai.html](https://www.nytimes.com/2026/02/27/us/politics/anthropic-military-ai.html)

生成摘要时出错

---

## 95. Warner Bros signs $110B deal with Paramount

**原文标题**: Warner Bros signs $110B deal with Paramount

**原文链接**: [https://www.reuters.com/sustainability/sustainable-finance-reporting/warner-bros-signs-110-billion-deal-with-paramount-its-executive-discloses-2026-02-27/](https://www.reuters.com/sustainability/sustainable-finance-reporting/warner-bros-signs-110-billion-deal-with-paramount-its-executive-discloses-2026-02-27/)

生成摘要时出错

---

## 96. Pentagon Adopts Incel-Speak

**原文标题**: Pentagon Adopts Incel-Speak

**原文链接**: [https://www.theguardian.com/science/2026/mar/01/incel-slang-mainstream-government-media](https://www.theguardian.com/science/2026/mar/01/incel-slang-mainstream-government-media)

生成摘要时出错

---

## 97. Show HN: Gitcredits – movie-style end credits for any Git repo in your terminal

**原文标题**: Show HN: Gitcredits – movie-style end credits for any Git repo in your terminal

**原文链接**: [https://github.com/Higangssh/gitcredits](https://github.com/Higangssh/gitcredits)

生成摘要时出错

---

## 98. US Customs destroy a rare floppy disk containing demo version of Tsukihime

**原文标题**: US Customs destroy a rare floppy disk containing demo version of Tsukihime

**原文链接**: [https://www.timeextension.com/news/2026/02/literally-crying-right-now-50-copies-of-this-adult-only-visual-novel-demo-exist-and-one-just-got-destroyed-in-transit](https://www.timeextension.com/news/2026/02/literally-crying-right-now-50-copies-of-this-adult-only-visual-novel-demo-exist-and-one-just-got-destroyed-in-transit)

生成摘要时出错

---

## 99. 390TB video game archive being taken offline due to skyrocketing RAM, SSD

**原文标题**: 390TB video game archive being taken offline due to skyrocketing RAM, SSD

**原文链接**: [https://www.tomshardware.com/video-games/390tb-video-game-archive-being-taken-offline-due-to-skyrocketing-ram-ssd-and-hard-drive-prices-ai-driven-supply-squeeze-results-in-closure-of-one-of-the-largest-online-video-game-archives](https://www.tomshardware.com/video-games/390tb-video-game-archive-being-taken-offline-due-to-skyrocketing-ram-ssd-and-hard-drive-prices-ai-driven-supply-squeeze-results-in-closure-of-one-of-the-largest-online-video-game-archives)

生成摘要时出错

---

## 100. No Bookmarks

**原文标题**: No Bookmarks

**原文链接**: [https://nik.art/no-bookmarks/](https://nik.art/no-bookmarks/)

生成摘要时出错

---

