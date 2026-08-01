# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-08-01.md)

*最后自动更新时间: 2026-08-01 20:27:42*
## 1. Solid Queue 1.6.0 现在支持协程工作器

**原文标题**: Solid Queue 1.6.0 now supports fiber workers

**原文链接**: [https://github.com/rails/solid_queue/releases/tag/v1.6.0](https://github.com/rails/solid_queue/releases/tag/v1.6.0)

Solid Queue 版本 1.6.0 已发布，引入了一个重要的新功能：支持协程工作者执行模式。这使得 Solid Queue 能够在单个协程反应器线程上使用协程运行作业，而不是依赖传统的线程池。要利用此功能，用户需要在其工作者配置中指定 `fibers` 的数量而非 `threads` 的数量（例如，`fibers: 100`）。此功能利用了 `Async` gem，该 gem 必须作为依赖项包含在内，并且要求 Rails 应用程序使用协程隔离（`config.active_support.isolation_level = :fiber`）。这种新的基于协程的方法特别有利于 I/O 密集型工作负载，例如涉及调用大型语言模型 (LLMs) 的工作负载，有望提高效率和资源利用率。本次发布的其他值得注意的更改包括：回滚测试中被终止的作业线程泄露的事务，以及改进了动态周期性任务更新的文档。协程工作者模式主要由 @crmne 贡献。

---

## 2. 矩阵一周

**原文标题**: A week in Matrix

**原文链接**: [https://piegames.de/dumps/a-week-in-matrix/](https://piegames.de/dumps/a-week-in-matrix/)

作者记录了其在Matrix上管理社区的“令人沮丧的一周”，揭示了诸多技术和可用性挑战。事件包括用户不慎在Matrix空间中聊天，由于持续的权限重置和跨 homeserver 的不同步问题，导致所有成员都收到通知。

调试一个源自共享审核列表的虚假用户封禁，过程异常艰巨，由于客户端搜索限制和无法应用本地覆盖，耗时40分钟。审核机器人Draupnir因Dendrite homeserver配置错误而离线一个多月，这凸显了维护已弃用服务器软件的困难以及缺乏便捷的迁移路径。其他问题包括新用户看不到聊天室，以及homeserver联邦问题导致账户“被遗忘”。

作者最后表达了深深的幻灭，因为Matrix基金会积极的公关宣传——宣称Matrix是“Discord的严肃替代品”——与运营复杂社区的日常现实之间存在着鲜明对比。他们批评该平台专注于基础的1对1私聊和旗舰客户端/服务器体验，认为其忽视了互操作性以及高级社区管理的需求，导致一种被食言“精神操控”（gaslit）的感觉。

---

## 3. Using the railway network as a flatbed scanner [video]

**原文标题**: Using the railway network as a flatbed scanner [video]

**原文链接**: [https://media.ccc.de/v/emf2026-74-1-using-the-railway-network-as-a-flatbed-scanner](https://media.ccc.de/v/emf2026-74-1-using-the-railway-network-as-a-flatbed-scanner)

生成摘要时出错

---

## 4. 反诈工具跟不上机器人电话诈骗者

**原文标题**: Anti-fraud tools can't keep pace with robocall scammers

**原文链接**: [https://broadbandbreakfast.com/how-to-fight-back-against-fraudulent-robocalls/](https://broadbandbreakfast.com/how-to-fight-back-against-fraudulent-robocalls/)

反欺诈工具难以跟上机器人电话诈骗犯的步伐，他们利用廉价的互联网通话和人工智能。专家指出，没有简单的解决方案，需要结合认证、溯源、拦截和消费者警惕。

转向互联网通话消除了有线网络的“物理信任”，使不法分子容易伪造身份。虽然STIR/SHAKEN等协议可以认证通话，但它们并非“灵丹妙药”，因为诈骗者可以获取合法的号码。历史上开放网络的竞争政策可能无意中助长了这种情况。

碎片化的通信生态系统（短信与RCS）使问题更加复杂，操作系统和运营商之间的可见性分离，导致难以实施类似电子邮件的垃圾信息解决方案。运营商可以分析通话模式但不能分析内容，这凸显了对提供商进行“了解您的客户”审查的必要性。

建议的解决方案包括为经过验证的来电者开发带有加密令牌的“使用权”系统，以及通过持续的消费者报告来促进全行业的合作和“群体智能”。

诈骗损失每年增长25%，通常与跨国有组织犯罪有关，执法工作正在改善。然而，小组成员警告不要让运营商独自承担网络钓鱼损失的责任，担心这可能导致过度拦截。建议消费者保持警惕，报告所有可疑信息，并在回应任何感觉不对劲的事情之前“深呼吸”或“暂停”。

---

## 5. Ruby中心遗祸

**原文标题**: Ruby Central's Destructive Legacy

**原文链接**: [https://andre.arko.net/2026/07/30/ruby-centrals-destructive-legacy/](https://andre.arko.net/2026/07/30/ruby-centrals-destructive-legacy/)

Ruby Central被指控在10个月前“恶意接管”了RubyGems、Bundler和RubyGems.org开源项目，并解除了长期维护者的职务。这一举动导致了严重的衰落：Ruby Central失去了其两个年度会议，将Bundler和RubyGems转移给了Matz，并且目睹了十分之九的开源贡献者、大多数董事会成员以及所有执行董事的离职。其当前的活动包括一个新的安全项目和一项赞助募捐活动，作者指出其中存在与董事会成员的利益冲突。

作者与Ruby Central的个人争议仍未解决。在作者声称Bundler名称侵权后，Ruby Central威胁要提起诉讼，指控作者“黑客行为”，并向联邦调查局(FBI)举报了作者，此举是其无法撤回的。Ruby Central要求作者放弃所有指控（侵权、违反雇佣法），以撤回诉讼威胁。

作者提出了多项和解提议，旨在就名誉攻击获得道歉并报销法律费用，但Ruby Central坚持要求签署一份单方面的互不诋毁协议，并提供了关于配合联邦调查局的非法条款。尽管审计结果未发现作者造成任何损害的证据，Ruby Central仍未公开道歉或充分解释其行为，仅以“安全”为由进行辩护。作者对Ruby Central当前“破坏性的遗产”表示遗憾，并将其与该组织在构建Ruby社区方面的历史作用形成对比。

---

## 6. 如何做伟大的工作 (2023)

**原文标题**: How to Do Great Work (2023)

**原文链接**: [https://paulgraham.com/greatwork.html](https://paulgraham.com/greatwork.html)

文章《如何做出卓越工作》概述了一种实现卓越成就的战略方法，强调这不仅仅是努力工作。关键的第一步是找到与你的天赋和深厚甚至“过分”的兴趣相契合的工作，从而留下广阔的施展空间。由于这种发现并非总是显而易见，尤其在年轻时，一个人必须通过“猜测并着手尝试”积极探索，培养由“激动的好奇心”驱动的个人项目。

一旦找到一个引人入胜的领域，这个过程就包括广泛学习以达到“知识前沿”，认真识别被忽视的空白，并大胆探索有前景的“非主流想法”，甚至拥抱一丝怪诞。这一旅程需要强烈而持续的努力，由真正的兴趣、好奇心以及创造出令人印象深刻之物的愿望所驱动。

对于仍在探索的人，建议是保持不懈的好奇心，尝试多种事物，并优先考虑真正让你感兴趣的，即使它不那么传统。如果出现了更令人兴奋的事物，不要害怕改变方向。在创作时，专注于你真正想要的东西，而不是臆想中的受众可能想要什么。与其进行僵化的长期规划，不如通过持续选择最有趣且能保留未来可能性的选项来“保持上风”。

实用的工作技巧包括管理精力以避免倦怠，投入大块的专注时间，以及利用“小窍门”克服最初的惰性。完成你开始的工作至关重要，并通过定期自问是否在处理最高优先级的事情，从而警惕地对抗每个项目的拖延症。卓越的工作是累积的努力，通过持之以恒和理解常被低估的指数增长力量来实现。

---

## 7. Dario Amodei 关于开放权重的立场是利己且短视的。

**原文标题**: Dario Amodei's stance on open weights is self-serving and short-sighted

**原文链接**: [https://janilowski.pl/en/blog/2026/amodei-memo/](https://janilowski.pl/en/blog/2026/amodei-memo/)

Dario Amodei在开放权重AI模型上的立场被批评为自私自利和短视。作者强调了Amodei明显的矛盾，指出尽管Amodei否认主张禁止，Anthropic仍在私下游说限制中国的开放权重模型。Amodei辩称，开放权重模型由于其可修改的防护措施，本质上更难确保安全，这与可以监控使用并撤销访问权限的专有模型不同。

作者认为，Amodei提出的监管体系——包括昂贵的发布前评估、持续监控和身份验证——等同于监管俘获。这一框架本质上偏袒Anthropic等大型专有模型提供商，它们已拥有必要的基础设施，同时却不利于小型实体、初创企业和开源项目。此外，开放模型将面临不公平的更严格评估标准，它们将在最坏可能修改的情境下进行评估。

文章指出，在西方限制开放权重将扼杀全球AI竞争力，损害西方公司，并矛盾地加速中国自主AI技术栈的发展，从而削弱西方的技术影响力。Amodei对“工业级蒸馏”的担忧被驳斥为商业抱怨而非战略威胁。

作者虽然同意需要一个行业机构来评估AI模型，但总结认为，Anthropic的“信任与安全”理念似乎已被“寻求权力的机会主义”所玷污，并援引了其过去的虚伪行为。拟议的监管体系，即便没有明确的禁令，也将有效地为Anthropic等公司保留前沿AI的控制权，并为其他公司规定访问条款。

---

## 8. GitHub有替代品，但无可取代。

**原文标题**: GitHub has alternatives, but no replacement

**原文链接**: [https://lalitm.com/post/github-alternatives/](https://lalitm.com/post/github-alternatives/)

The article argues that despite GitHub's declining performance, no existing alternative offers a true replacement due to the absence of a comparable "social layer." The recent Codeberg decision to ban AI-generated code highlighted this gap, as many were disappointed, having hoped it would be a universal alternative to GitHub's perceived neutrality.

GitHub's unique value lies in providing a shared pool of identities, common contribution habits, and a strong discovery mechanism for open-source projects, effectively fostering a community. However, GitHub is increasingly criticized for being slow, unreliable, having a poor pull request experience, and prioritizing AI tools like Copilot over its core forge. Major outages have even prompted projects like Ghostty to leave.

Self-hosting, while decentralized, creates too much friction for new contributors who would need to create accounts and learn new systems, and it lacks project discovery. Existing alternatives like GitLab are too corporate, SourceHut's email workflow is unfamiliar, Forgejo and Radicle are promising but immature and present barriers to entry, and Tangled is still in early development.

The author suggests a "boring company" focused purely on reliable open-source collaboration could fill the void. However, the critical challenge remains the "cold-start problem": building the essential social layer—shared identity, conventions, and discovery—which only becomes valuable at scale. A true GitHub replacement must prioritize this social infrastructure as its product, rather than expecting it to emerge automatically.

---

## 9. The EU is making the Right to Repair the new standard in Europe

**原文标题**: The EU is making the Right to Repair the new standard in Europe

**原文链接**: [https://ec.social-network.europa.eu/@EUCommission/117013565926587088](https://ec.social-network.europa.eu/@EUCommission/117013565926587088)

生成摘要时出错

---

## 10. BMW Is Showing Commercials on Their Car's Dash Screens as a Treat

**原文标题**: BMW Is Showing Commercials on Their Car's Dash Screens as a Treat

**原文链接**: [https://www.theautopian.com/bmw-is-showing-commercials-on-their-cars-dash-screens-and-they-want-you-to-think-its-a-treat/](https://www.theautopian.com/bmw-is-showing-commercials-on-their-cars-dash-screens-and-they-want-you-to-think-its-a-treat/)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 2 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 3 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 4 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 5 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 6 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 7 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 8 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 9 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 10 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 11 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 12 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 13 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 14 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 15 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 16 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 17 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 18 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 19 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 20 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 21 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 22 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 23 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 24 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 25 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 26 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 27 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 28 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 29 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 30 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 31 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 32 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 33 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 34 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 35 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 36 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 37 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 38 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 39 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 40 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 41 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 42 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 43 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 44 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 45 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 46 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 47 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 48 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 49 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 50 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 51 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 52 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 53 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 54 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 55 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 56 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 57 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 58 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 59 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 60 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 61 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 62 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 63 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 64 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 65 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 66 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 67 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 68 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 69 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 70 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 71 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 72 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 73 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 74 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 75 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 76 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 77 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 78 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 79 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 80 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 81 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 82 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 83 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 84 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 85 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 86 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 87 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 88 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 89 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 90 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 91 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 92 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 93 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 94 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 95 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 96 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 97 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 98 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 99 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 100 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 101 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 102 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 103 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 104 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 105 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 106 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 107 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 108 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 109 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 110 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 111 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 112 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 113 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 114 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 115 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 116 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 117 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 118 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 119 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 120 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 121 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 122 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 123 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 124 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 125 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 126 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 127 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 128 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 129 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 130 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 131 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 132 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 133 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 134 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 135 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 136 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 137 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 138 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 139 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 140 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 141 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 142 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 143 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 144 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 145 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 146 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 147 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 148 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 149 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 150 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 151 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 152 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 153 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 154 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 155 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 156 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 157 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 158 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 159 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 160 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 161 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 162 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 163 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 164 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 165 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 166 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 167 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 168 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 169 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 170 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 171 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 172 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 173 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 174 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 175 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 176 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 177 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 178 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 179 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 180 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 181 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 182 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 183 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 184 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 185 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 186 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 187 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 188 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 189 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 190 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 191 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 192 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 193 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 194 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 195 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 196 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 197 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 198 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 199 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 200 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 201 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 202 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 203 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 204 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 205 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 206 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 207 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 208 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 209 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 210 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 211 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 212 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 213 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 214 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 215 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 216 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 217 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 218 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 219 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 220 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 221 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 222 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 223 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 224 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 225 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 226 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 227 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 228 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 229 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 230 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 231 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 232 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 233 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 234 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 235 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 236 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 237 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 238 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 239 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 240 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 241 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 242 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 243 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 244 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 245 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 246 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 247 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 248 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 249 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 250 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 251 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 252 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 253 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 254 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 255 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 256 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 257 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 258 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 259 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 260 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 261 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 262 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 263 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 264 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 265 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 266 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 267 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
