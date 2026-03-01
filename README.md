# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-03-01.md)

*最后自动更新时间: 2026-03-01 19:53:27*
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

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 2 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 3 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 4 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 5 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 6 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 7 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 8 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 9 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 10 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 11 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 12 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 13 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 14 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 15 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 16 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 17 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 18 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 19 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 20 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 21 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 22 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 23 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 24 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 25 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 26 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 27 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 28 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 29 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 30 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 31 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 32 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 33 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 34 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 35 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 36 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 37 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 38 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 39 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 40 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 41 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 42 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 43 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 44 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 45 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 46 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 47 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 48 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 49 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 50 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 51 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 52 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 53 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 54 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 55 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 56 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 57 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 58 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 59 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 60 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 61 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 62 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 63 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 64 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 65 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 66 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 67 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 68 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 69 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 70 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 71 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 72 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 73 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 74 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 75 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 76 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 77 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 78 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 79 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 80 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 81 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 82 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 83 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 84 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 85 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 86 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 87 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 88 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 89 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 90 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 91 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 92 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 93 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 94 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 95 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 96 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 97 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 98 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 99 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 100 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 101 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 102 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 103 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 104 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 105 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 106 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 107 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 108 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 109 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
| 110 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 111 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 112 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 113 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 114 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 115 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
