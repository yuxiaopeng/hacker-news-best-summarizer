# Hacker News 热门文章摘要 (2026-03-10)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 爱尔兰关闭最后一座燃煤电厂，成为欧洲第15个无煤国家 (2025年)

**原文标题**: Ireland shuts last coal plant, becomes 15th coal-free country in Europe (2025)

**原文链接**: [https://www.pv-magazine.com/2025/06/20/ireland-coal-free-ends-coal-power-generation-moneypoint/](https://www.pv-magazine.com/2025/06/20/ireland-coal-free-ends-coal-power-generation-moneypoint/)

所提供的内容描述了爱尔兰计划在2025年前关闭其最后一座燃煤电厂，旨在成为欧洲第15个“无煤”国家。

然而，附带的评论对此举的真实环境效益表示怀疑。评论者质疑，如果爱尔兰只是简单地从波兰等其他国家采购煤炭并继续燃烧，那么关闭国内电厂是否真正“有益于气候”。他们认为，采矿、公路运输到港口、海运到爱尔兰，以及本地卡车运输这一漫长的运输过程，将显著增加整体污染，可能会因为供应链产生的额外排放而使情况变得更糟。

评论者将这种情况比作砍伐亚马逊雨林并将其运到爱尔兰焚烧，认为这仅仅是“象征性的气候关怀”，旨在“作秀”，而实际上是将环境问题转嫁并扩大到其他地方，而不是真正解决问题。

---

## 2. 托尼·霍尔逝世

**原文标题**: Tony Hoare has died

**原文链接**: [https://blog.computationalcomplexity.org/2026/03/tony-hoare-1934-2026.html](https://blog.computationalcomplexity.org/2026/03/tony-hoare-1934-2026.html)

著名图灵奖得主、前牛津大学教授托尼·霍尔（Tony Hoare）（1934-2026）于2026年3月5日星期四去世，享年92岁。他以对快速排序、ALGOL语言和霍尔逻辑等领域的贡献而闻名，他的离世促使通过剑桥家庭关系认识霍尔的吉姆·迈尔斯（Jim Miles）发表了个人缅怀。

迈尔斯回忆说，霍尔尽管身体抱恙，但思维依然敏锐，为人热情。他讲述了霍尔不同寻常的职业道路：他最初学习古典学和哲学，之后成为一名俄语语言学家，并在苏联担任早期计算机演示员，期间也从事代码开发工作。一个他最喜欢的小故事是“快速排序赌注”，霍尔曾与他的老板打赌六便士，声称他的新算法更快，他最终也确实因此项发现获得了报酬，这一细节体现了他谦逊的专业精神。

迈尔斯还了解到，霍尔在微软工作期间有在下午看电影的习惯。霍尔认同，好莱坞将天才错误地描绘成瞬间的灵感，而非多年的奋斗。最有趣的是，霍尔自信地表示，政府技术“比你想象的领先数年”，当被追问具体细节时，他神秘地耸了耸肩。迈尔斯将非常怀念霍尔的幽默、耐心和敏锐的头脑。

---

## 3. 代理安全屋 – 本地代理的 macOS 原生沙盒

**原文标题**: Agent Safehouse – macOS-native sandboxing for local agents

**原文链接**: [https://agent-safehouse.dev/](https://agent-safehouse.dev/)

代理安全屋为本地AI代理提供macOS原生的沙盒化，以解决概率性LLM执行破坏性或未经授权命令的关键风险。它实现了一个内核强制执行、拒绝优先的访问模型，确保代理只能与明确授予的文件和目录进行交互。这可以防止意外数据丢失（例如，`rm -rf ~`）和未经授权访问敏感信息。

该解决方案以单个Bash脚本的形式提供，无需构建步骤或依赖。当代理在安全屋内部运行时，它会自动获得对其当前项目目录（通常是git根目录）的读/写访问权限，以及对已安装工具链的只读访问权限。关键是，它会拒绝访问SSH密钥 (`~/.ssh`)、AWS凭证以及其他个人文件等敏感区域，内核会阻止这些系统调用。

本文通过展示尝试读取SSH私钥或列出另一个项目目录会显示“Operation not permitted”（操作不允许）来证明这一点。为了便于使用，可以将shell函数添加到`.zshrc`或`.bashrc`中，以便默认自动沙盒化流行的代理（例如Claude、Gemini）。高级用户还可以使用LLM为其特定设置生成自定义的、最小权限的`sandbox-exec`配置文件。

---

## 4. 使用波函数坍缩生成程序化六边形地图

**原文标题**: Building a Procedural Hex Map with Wave Function Collapse

**原文链接**: [https://felixturner.github.io/hex-map-wfc/article/](https://felixturner.github.io/hex-map-wfc/article/)

本文详细介绍了为中世纪岛屿世界创建程序化六边形地图生成器的过程，该生成器使用Three.js WebGPU和TSL着色器构建，能够在约20秒内生成横跨19个网格的约4,100个单元格。其核心技术是受卡卡颂启发的波函数塌缩（WFC），其中30种图块类型（每种有6种旋转和5个海拔高度级别）定义了6种边缘类型，这些边缘类型必须与其邻居匹配。

大型网格面临的一个重大挑战是WFC频繁失败。解决方案是将地图拆分为19个独立的六边形网格，每个网格在受到其邻居边界约束的情况下独立求解。开发了一个强大且分层的恢复系统，包括回溯、"解除固定"冲突的邻居约束，以及一个关键的"局部WFC"步骤来重新解决小问题区域。作为最后的补救措施，该系统会放置山脉以覆盖无法解决的接缝。地图的5个海拔高度级别进一步使3D约束问题复杂化。

除了WFC，柏林噪声还用于生成树木和建筑物的有机聚类，这是WFC难以处理的。视觉效果包括动画水面效果，如滚动焦散波光和辐射状海岸波纹，其中CPU侧的"环绕度"探测解决了海湾中的美学问题。渲染管线使用WebGPU和TSL，并通过后处理堆栈（GTAO、景深、晕影）增强氛围，以及通过动态阴影贴图实现清晰细节。性能通过BatchedMeshes和单个共享材质进行优化，确保在各种设备上达到60帧/秒。最终成果是一张独特、确定性且高度可探索的程序化地图。

---

## 5. 合法等同于正当吗？：AI重实现与Copyleft的侵蚀

**原文标题**: Is legal the same as legitimate: AI reimplementation and the erosion of copyleft

**原文链接**: [https://writings.hongminhee.org/2026/03/legal-vs-legitimate/](https://writings.hongminhee.org/2026/03/legal-vs-legitimate/)

这篇文章探讨了人工智能辅助代码重实现的伦理影响，起因是chardet维护者Dan Blanchard使用人工智能将LGPL许可的Python库重写成新的MIT许可版本。Blanchard只向人工智能提供了API和测试套件，并声称这是一项独立作品。然而，原始作者Mark Pilgrim和本文作者认为，这破坏了LGPL的“共享”原则。

作者批判了著名开源人物Armin Ronacher和Salvatore Sanfilippo的回应，两人都为Blanchard的行为辩护，称其合法。核心论点在于“合法”是否自动等同于“正当”。

Sanfilippo基于版权法和GNU项目合法重实现UNIX的辩护被驳斥。作者认为，虽然在法律上允许，但GNU的先例扩大了公共领域（从专有到自由），而chardet的案例则缩小了公共领域（从Copyleft到宽松许可），消除了分享改进的义务。

Ronacher承认偏见，声称GPL限制了共享。作者驳斥了这一点，解释说GPL *强制*互惠共享，有利于个人开发者，而不像有利于资本的宽松许可。Ronacher自己举例，Vercel对Cloudflare重实现其MIT许可的Next.js感到不满，而Vercel自己却用人工智能将GPL Bash重实现为MIT，这突显了他对共享的矛盾立场。

文章强调，合法性仅仅是底线，而不是正确性的认证。LGPL代表了贡献者之间的社会契约和信任；打破它，即使是合法的，也是反社会的。作者指出“位置不对称性”：像Ronacher和Sanfilippo这样已建立的创作者从人工智能驱动的更容易的重实现中获益，而普通贡献者则失去了Copyleft保护。

作者总结道，人工智能使Copyleft变得*更*有必要来保护用户自由。随着代码生成简化，保护应扩展到规范（建议一种“规范Copyleft”）。潜在的原则——那些从公共领域获取的人有义务回馈——仍然是一个重要的社会判断，独立于不断演变的法律框架。

---

## 6. 美国上诉法院：服务条款可通过电子邮件更新，使用可推定同意

**原文标题**: US Court of Appeals: TOS may be updated by email, use can imply consent [pdf]

**原文链接**: [https://cdn.ca9.uscourts.gov/datastore/memoranda/2026/03/03/25-403.pdf](https://cdn.ca9.uscourts.gov/datastore/memoranda/2026/03/03/25-403.pdf)

所提供的内容是原始PDF数据，无法直接解析以提取可读文本进行摘要。

然而，仅根据所提供的标题“美国上诉法院：服务条款可通过电子邮件更新，使用可暗示同意”，该文章讨论了一项重要的法律裁决。这项来自美国上诉法院的裁决确立了关于服务条款（TOS）协议的两项关键原则：

1.  **电子邮件作为有效的更新方式：** 公司被允许更新其服务条款，并通过电子邮件通知用户这些变更。
2.  **使用行为可暗示同意：** 用户在收到关于更新服务条款的电子邮件通知后继续使用该服务，可被解读为对这些新条款的默示同意行为。

这对于企业如何管理其用户协议以及用户如何受在线服务变更的法律约束具有重大影响，强调了审查此类电子邮件通知的重要性。

---

## 7. 佛罗里达法官裁定红灯摄像头罚单违宪

**原文标题**: Florida judge rules red light camera tickets are unconstitutional

**原文链接**: [https://cbs12.com/news/local/florida-news-judge-rules-red-light-camera-tickets-unconstitutional](https://cbs12.com/news/local/florida-news-judge-rules-red-light-camera-tickets-unconstitutional)

布劳沃德县法官史蒂文·P·德卢卡驳回了一张闯红灯摄像头罚单，裁定佛罗里达州的闯红灯摄像头法律（佛罗里达州法规316.0083）违宪。法官认为该法律不当地将举证责任转移给车主，违反了正当程序保护。

该案件涉及日出市的一张闯红灯摄像头罚单，被告辩称该法规违宪地要求注册车主证明自己当时没有驾驶，而不是要求政府“排除合理怀疑地”证明谁是驾驶员。德卢卡法官对此表示认同，将这些罚单归类为“准刑事”诉讼，因为它们可能带来金钱处罚并影响驾驶记录。该法律推定注册车主负有责任，除非他们提交一份宣誓书指明另一位驾驶员，这种推定被认为是非法地将举证责任从州政府转移出去。

尽管这项具体裁决目前仅适用于布劳沃德县，但律师乔尔·芒福德认为这可能为全州的挑战打开大门。上诉以及地区法院的裁决可能导致其在佛罗里达州全境更广泛地适用。像StopTheCams这样反对自动化执法的驾驶员和倡导团体将这一裁决视为一项重大胜利，证实了他们长期以来的论点，即这些法律在没有证据证明车主参与的情况下惩罚车主。

闯红灯摄像头的支持者认为它们提高了十字路口的安全。目前尚不确定该裁决是否会上诉，或者它将对类似案件产生多大影响，但预计它将重新激发对佛罗里达州闯红灯摄像头执法系统的挑战。

---

## 8. FontCrafter: Turn your handwriting into a real font

**原文标题**: FontCrafter: Turn your handwriting into a real font

**原文链接**: [https://arcade.pirillo.com/fontcrafter.html](https://arcade.pirillo.com/fontcrafter.html)

生成摘要时出错

---

## 9. No, it doesn't cost Anthropic $5k per Claude Code user

**原文标题**: No, it doesn't cost Anthropic $5k per Claude Code user

**原文链接**: [https://martinalderson.com/posts/no-it-doesnt-cost-anthropic-5k-per-claude-code-user/](https://martinalderson.com/posts/no-it-doesnt-cost-anthropic-5k-per-claude-code-user/)

生成摘要时出错

---

## 10. How the Sriracha guys screwed over their supplier

**原文标题**: How the Sriracha guys screwed over their supplier

**原文链接**: [https://old.reddit.com/r/KitchenConfidential/comments/1ro61g2/how_the_sriracha_guys_screwed_over_their_supplier/](https://old.reddit.com/r/KitchenConfidential/comments/1ro61g2/how_the_sriracha_guys_screwed_over_their_supplier/)

生成摘要时出错

---

## 11. OpenAI is walking away from expanding its Stargate data center with Oracle

**原文标题**: OpenAI is walking away from expanding its Stargate data center with Oracle

**原文链接**: [https://www.cnbc.com/2026/03/09/oracle-is-building-yesterdays-data-centers-with-tomorrows-debt.html](https://www.cnbc.com/2026/03/09/oracle-is-building-yesterdays-data-centers-with-tomorrows-debt.html)

生成摘要时出错

---

## 12. Yann LeCun's AI startup raises $1B in Europe's largest ever seed round

**原文标题**: Yann LeCun's AI startup raises $1B in Europe's largest ever seed round

**原文链接**: [https://www.ft.com/content/e5245ec3-1a58-4eff-ab58-480b6259aaf1](https://www.ft.com/content/e5245ec3-1a58-4eff-ab58-480b6259aaf1)

生成摘要时出错

---

## 13. Bluesky CEO Jay Graber is stepping down

**原文标题**: Bluesky CEO Jay Graber is stepping down

**原文链接**: [https://bsky.social/about/blog/03-09-2026-a-new-chapter-for-bluesky](https://bsky.social/about/blog/03-09-2026-a-new-chapter-for-bluesky)

生成摘要时出错

---

## 14. Online age-verification tools for child safety are surveilling adults

**原文标题**: Online age-verification tools for child safety are surveilling adults

**原文链接**: [https://www.cnbc.com/2026/03/08/social-media-child-safety-internet-ai-surveillance.html](https://www.cnbc.com/2026/03/08/social-media-child-safety-internet-ai-surveillance.html)

生成摘要时出错

---

## 15. JSLinux Now Supports x86_64

**原文标题**: JSLinux Now Supports x86_64

**原文链接**: [https://bellard.org/jslinux/](https://bellard.org/jslinux/)

生成摘要时出错

---

## 16. I put my whole life into a single database

**原文标题**: I put my whole life into a single database

**原文链接**: [https://howisfelix.today/](https://howisfelix.today/)

生成摘要时出错

---

## 17. Two Years of Emacs Solo

**原文标题**: Two Years of Emacs Solo

**原文链接**: [https://www.rahuljuliato.com/posts/emacs-solo-two-years](https://www.rahuljuliato.com/posts/emacs-solo-two-years)

生成摘要时出错

---

## 18. Redox OS has adopted a Certificate of Origin policy and a strict no-LLM policy

**原文标题**: Redox OS has adopted a Certificate of Origin policy and a strict no-LLM policy

**原文链接**: [https://gitlab.redox-os.org/redox-os/redox/-/blob/master/CONTRIBUTING.md](https://gitlab.redox-os.org/redox-os/redox/-/blob/master/CONTRIBUTING.md)

生成摘要时出错

---

## 19. Show HN: I built a real-time OSINT dashboard pulling 15 live global feeds

**原文标题**: Show HN: I built a real-time OSINT dashboard pulling 15 live global feeds

**原文链接**: [https://github.com/BigBodyCobain/Shadowbroker](https://github.com/BigBodyCobain/Shadowbroker)

生成摘要时出错

---

## 20. We should revisit literate programming in the agent era

**原文标题**: We should revisit literate programming in the agent era

**原文链接**: [https://silly.business/blog/we-should-revisit-literate-programming-in-the-agent-era/](https://silly.business/blog/we-should-revisit-literate-programming-in-the-agent-era/)

生成摘要时出错

---

## 21. Meta acquires Moltbook

**原文标题**: Meta acquires Moltbook

**原文链接**: [https://www.axios.com/2026/03/10/meta-facebook-moltbook-agent-social-network](https://www.axios.com/2026/03/10/meta-facebook-moltbook-agent-social-network)

生成摘要时出错

---

## 22. Amazon is holding a mandatory meeting about AI breaking its systems

**原文标题**: Amazon is holding a mandatory meeting about AI breaking its systems

**原文链接**: [https://twitter.com/lukolejnik/status/2031257644724342957](https://twitter.com/lukolejnik/status/2031257644724342957)

生成摘要时出错

---

## 23. FFmpeg at Meta: Media Processing at Scale

**原文标题**: FFmpeg at Meta: Media Processing at Scale

**原文链接**: [https://engineering.fb.com/2026/03/02/video-engineering/ffmpeg-at-meta-media-processing-at-scale/](https://engineering.fb.com/2026/03/02/video-engineering/ffmpeg-at-meta-media-processing-at-scale/)

生成摘要时出错

---

## 24. Tony Hoare has died

**原文标题**: Tony Hoare has died

**原文链接**: [http://lefenetrou.blogspot.com/2026/03/in-memoriam-tony-hoare.html](http://lefenetrou.blogspot.com/2026/03/in-memoriam-tony-hoare.html)

生成摘要时出错

---

## 25. The engine of Germany's wealth is blocking its future

**原文标题**: The engine of Germany's wealth is blocking its future

**原文链接**: [https://europeancorrespondent.com/en/r/the-engine-of-germanys-wealth-is-blocking-its-future](https://europeancorrespondent.com/en/r/the-engine-of-germanys-wealth-is-blocking-its-future)

生成摘要时出错

---

## 26. The death of social media is the renaissance of RSS (2025)

**原文标题**: The death of social media is the renaissance of RSS (2025)

**原文链接**: [https://www.smartlab.at/rss-revival-life-after-social-media/](https://www.smartlab.at/rss-revival-life-after-social-media/)

生成摘要时出错

---

## 27. Most of the US economy is in a recession

**原文标题**: Most of the US economy is in a recession

**原文链接**: [https://www.businessinsider.com/recession-economy-us-tech-wall-street-strategist-investing-stocks-market-2026-3](https://www.businessinsider.com/recession-economy-us-tech-wall-street-strategist-investing-stocks-market-2026-3)

生成摘要时出错

---

## 28. DARPA’s new X-76

**原文标题**: DARPA’s new X-76

**原文链接**: [https://www.darpa.mil/news/2026/darpa-new-x-76-speed-of-jet-freedom-of-helicopter](https://www.darpa.mil/news/2026/darpa-new-x-76-speed-of-jet-freedom-of-helicopter)

生成摘要时出错

---

## 29. Workers report watching Ray-Ban Meta-shot footage of people using the bathroom

**原文标题**: Workers report watching Ray-Ban Meta-shot footage of people using the bathroom

**原文链接**: [https://arstechnica.com/gadgets/2026/03/workers-report-watching-ray-ban-meta-shot-footage-of-people-using-the-bathroom/](https://arstechnica.com/gadgets/2026/03/workers-report-watching-ray-ban-meta-shot-footage-of-people-using-the-bathroom/)

生成摘要时出错

---

## 30. Jolla on track to ship new phone with Sailfish OS, user-replaceable battery

**原文标题**: Jolla on track to ship new phone with Sailfish OS, user-replaceable battery

**原文链接**: [https://liliputing.com/the-new-jolla-phone-with-sailfish-os-is-on-track-to-start-shipping-in-the-first-half-of-2026/](https://liliputing.com/the-new-jolla-phone-with-sailfish-os-is-on-track-to-start-shipping-in-the-first-half-of-2026/)

生成摘要时出错

---

## 31. New farm bill would condemn pigs to a lifetime in gestation crates

**原文标题**: New farm bill would condemn pigs to a lifetime in gestation crates

**原文链接**: [https://twitter.com/Lewis_Bollard/status/2030985704902099335](https://twitter.com/Lewis_Bollard/status/2030985704902099335)

生成摘要时出错

---

## 32. Debian decides not to decide on AI-generated contributions

**原文标题**: Debian decides not to decide on AI-generated contributions

**原文链接**: [https://lwn.net/SubscriberLink/1061544/125f911834966dd0/](https://lwn.net/SubscriberLink/1061544/125f911834966dd0/)

生成摘要时出错

---

## 33. Show HN: How I Topped the HuggingFace Open LLM Leaderboard on Two Gaming GPUs

**原文标题**: Show HN: How I Topped the HuggingFace Open LLM Leaderboard on Two Gaming GPUs

**原文链接**: [https://dnhkng.github.io/posts/rys/](https://dnhkng.github.io/posts/rys/)

生成摘要时出错

---

## 34. Intel Demos Chip to Compute with Encrypted Data

**原文标题**: Intel Demos Chip to Compute with Encrypted Data

**原文链接**: [https://spectrum.ieee.org/fhe-intel](https://spectrum.ieee.org/fhe-intel)

生成摘要时出错

---

## 35. Fixfest is a global gathering of repairers, tinkerers, and activists

**原文标题**: Fixfest is a global gathering of repairers, tinkerers, and activists

**原文链接**: [https://fixfest.therestartproject.org/](https://fixfest.therestartproject.org/)

生成摘要时出错

---

## 36. Reverse-engineering the UniFi inform protocol

**原文标题**: Reverse-engineering the UniFi inform protocol

**原文链接**: [https://tamarack.cloud/blog/reverse-engineering-unifi-inform-protocol](https://tamarack.cloud/blog/reverse-engineering-unifi-inform-protocol)

生成摘要时出错

---

## 37. Artificial-life: A simple (300 lines of code) reproduction of Computational Life

**原文标题**: Artificial-life: A simple (300 lines of code) reproduction of Computational Life

**原文链接**: [https://github.com/Rabrg/artificial-life](https://github.com/Rabrg/artificial-life)

生成摘要时出错

---

## 38. Learnings from paying artists royalties for AI-generated art

**原文标题**: Learnings from paying artists royalties for AI-generated art

**原文链接**: [https://www.kapwing.com/blog/learnings-from-paying-artists-royalties-for-ai-generated-art/](https://www.kapwing.com/blog/learnings-from-paying-artists-royalties-for-ai-generated-art/)

生成摘要时出错

---

## 39. Show HN: The Mog Programming Language

**原文标题**: Show HN: The Mog Programming Language

**原文链接**: [https://moglang.org](https://moglang.org)

生成摘要时出错

---

## 40. An opinionated take on how to do important research that matters

**原文标题**: An opinionated take on how to do important research that matters

**原文链接**: [https://nicholas.carlini.com/writing/2026/how-to-win-a-best-paper-award.html](https://nicholas.carlini.com/writing/2026/how-to-win-a-best-paper-award.html)

生成摘要时出错

---

## 41. Rebasing in Magit

**原文标题**: Rebasing in Magit

**原文链接**: [https://entropicthoughts.com/rebasing-in-magit](https://entropicthoughts.com/rebasing-in-magit)

生成摘要时出错

---

## 42. Kuwaiti F/A-18's Triple Friendly Fire Shootdown Gets Stranger by the Day

**原文标题**: Kuwaiti F/A-18's Triple Friendly Fire Shootdown Gets Stranger by the Day

**原文链接**: [https://www.twz.com/air/kuwaiti-f-a-18s-triple-friendly-fire-shootdown-gets-stranger-by-the-day](https://www.twz.com/air/kuwaiti-f-a-18s-triple-friendly-fire-shootdown-gets-stranger-by-the-day)

生成摘要时出错

---

## 43. Show HN: Mcp2cli – One CLI for every API, 96-99% fewer tokens than native MCP

**原文标题**: Show HN: Mcp2cli – One CLI for every API, 96-99% fewer tokens than native MCP

**原文链接**: [https://github.com/knowsuchagency/mcp2cli](https://github.com/knowsuchagency/mcp2cli)

生成摘要时出错

---

## 44. Blacksky AppView

**原文标题**: Blacksky AppView

**原文链接**: [https://github.com/blacksky-algorithms/atproto](https://github.com/blacksky-algorithms/atproto)

生成摘要时出错

---

## 45. FreeBSD 14.4-Release Announcement

**原文标题**: FreeBSD 14.4-Release Announcement

**原文链接**: [https://www.freebsd.org/releases/14.4R/announce/](https://www.freebsd.org/releases/14.4R/announce/)

生成摘要时出错

---

## 46. Peter Thiel and Jeffrey Epstein Had a Yearslong Relationship

**原文标题**: Peter Thiel and Jeffrey Epstein Had a Yearslong Relationship

**原文链接**: [https://jacobin.com/2026/03/thiel-epstein-barak-ai-israel/](https://jacobin.com/2026/03/thiel-epstein-barak-ai-israel/)

生成摘要时出错

---

## 47. Optimizing Top K in Postgres

**原文标题**: Optimizing Top K in Postgres

**原文链接**: [https://www.paradedb.com/blog/optimizing-top-k](https://www.paradedb.com/blog/optimizing-top-k)

生成摘要时出错

---

## 48. I don't know Apple's endgame for the Fn/Globe key–or if Apple does

**原文标题**: I don't know Apple's endgame for the Fn/Globe key–or if Apple does

**原文链接**: [https://aresluna.org/fn/](https://aresluna.org/fn/)

生成摘要时出错

---

## 49. So you want to write an “app” (2025)

**原文标题**: So you want to write an “app” (2025)

**原文链接**: [https://arcanenibble.github.io/so-you-want-to-write-an-app.html](https://arcanenibble.github.io/so-you-want-to-write-an-app.html)

生成摘要时出错

---

## 50. Show HN: DenchClaw – Local CRM on Top of OpenClaw

**原文标题**: Show HN: DenchClaw – Local CRM on Top of OpenClaw

**原文链接**: [https://github.com/DenchHQ/DenchClaw](https://github.com/DenchHQ/DenchClaw)

生成摘要时出错

---

## 51. No leap second will be introduced at the end of June 2026

**原文标题**: No leap second will be introduced at the end of June 2026

**原文链接**: [https://lists.iana.org/hyperkitty/list/tz@iana.org/thread/P6D36VZSZBUSSTSMZKFXKF4T4IXWN23P/](https://lists.iana.org/hyperkitty/list/tz@iana.org/thread/P6D36VZSZBUSSTSMZKFXKF4T4IXWN23P/)

生成摘要时出错

---

## 52. Launch HN: RunAnywhere (YC W26) – Faster AI Inference on Apple Silicon

**原文标题**: Launch HN: RunAnywhere (YC W26) – Faster AI Inference on Apple Silicon

**原文链接**: [https://github.com/RunanywhereAI/rcli](https://github.com/RunanywhereAI/rcli)

生成摘要时出错

---

## 53. US missile hit military base near Iran school, video analysis shows

**原文标题**: US missile hit military base near Iran school, video analysis shows

**原文链接**: [https://www.bbc.com/news/articles/cvg548lyjnyo](https://www.bbc.com/news/articles/cvg548lyjnyo)

生成摘要时出错

---

## 54. LoGeR – 3D reconstruction from extremely long videos (DeepMind, UC Berkeley)

**原文标题**: LoGeR – 3D reconstruction from extremely long videos (DeepMind, UC Berkeley)

**原文链接**: [https://loger-project.github.io](https://loger-project.github.io)

生成摘要时出错

---

## 55. Linux Internals: How /proc/self/mem writes to unwritable memory (2021)

**原文标题**: Linux Internals: How /proc/self/mem writes to unwritable memory (2021)

**原文链接**: [https://offlinemark.com/an-obscure-quirk-of-proc/](https://offlinemark.com/an-obscure-quirk-of-proc/)

生成摘要时出错

---

## 56. Yann LeCun raises $1B to build AI that understands the physical world

**原文标题**: Yann LeCun raises $1B to build AI that understands the physical world

**原文链接**: [https://www.wired.com/story/yann-lecun-raises-dollar1-billion-to-build-ai-that-understands-the-physical-world/](https://www.wired.com/story/yann-lecun-raises-dollar1-billion-to-build-ai-that-understands-the-physical-world/)

生成摘要时出错

---

## 57. FreeBSD Capsicum vs. Linux Seccomp Process Sandboxing

**原文标题**: FreeBSD Capsicum vs. Linux Seccomp Process Sandboxing

**原文链接**: [https://vivianvoss.net/blog/capsicum-vs-seccomp](https://vivianvoss.net/blog/capsicum-vs-seccomp)

生成摘要时出错

---

## 58. Swiss vote places right to use cash in country's constitution

**原文标题**: Swiss vote places right to use cash in country's constitution

**原文链接**: [https://www.politico.eu/article/switzerland-cash-right-constitution-vote/](https://www.politico.eu/article/switzerland-cash-right-constitution-vote/)

生成摘要时出错

---

## 59. Windows: Microsoft broke the only thing that mattered

**原文标题**: Windows: Microsoft broke the only thing that mattered

**原文链接**: [https://www.yankodesign.com/2026/03/08/microsoft-broke-the-only-thing-that-actually-mattered/](https://www.yankodesign.com/2026/03/08/microsoft-broke-the-only-thing-that-actually-mattered/)

生成摘要时出错

---

## 60. The Government Told Courts It Could Easily Refund Tariffs. Now It Says It Can't

**原文标题**: The Government Told Courts It Could Easily Refund Tariffs. Now It Says It Can't

**原文链接**: [https://www.techdirt.com/2026/03/09/the-government-told-courts-it-could-easily-refund-unlawful-tariffs-now-it-says-it-cant/](https://www.techdirt.com/2026/03/09/the-government-told-courts-it-could-easily-refund-unlawful-tariffs-now-it-says-it-cant/)

生成摘要时出错

---

## 61. Uber reported to the state that I was fired for "annoying a coworker."

**原文标题**: Uber reported to the state that I was fired for "annoying a coworker."

**原文链接**: [https://anon-ex-uber.medium.com/uber-reported-to-the-state-that-i-was-fired-for-annoying-a-coworker-4ba7490cc0b8](https://anon-ex-uber.medium.com/uber-reported-to-the-state-that-i-was-fired-for-annoying-a-coworker-4ba7490cc0b8)

生成摘要时出错

---

## 62. Restoring a Sun SPARCstation IPX part 1: PSU and NVRAM (2020)

**原文标题**: Restoring a Sun SPARCstation IPX part 1: PSU and NVRAM (2020)

**原文链接**: [https://www.rs-online.com/designspark/restoring-a-sun-sparcstation-ipx-part-1-psu-and-nvram](https://www.rs-online.com/designspark/restoring-a-sun-sparcstation-ipx-part-1-psu-and-nvram)

生成摘要时出错

---

## 63. Traffic from Russia to Cloudflare is 60% down from last year

**原文标题**: Traffic from Russia to Cloudflare is 60% down from last year

**原文链接**: [https://radar.cloudflare.com/traffic/ru?dateRange=52w](https://radar.cloudflare.com/traffic/ru?dateRange=52w)

生成摘要时出错

---

## 64. Iranians describe scenes of catastrophe after Tehran's oil depots bombed

**原文标题**: Iranians describe scenes of catastrophe after Tehran's oil depots bombed

**原文链接**: [https://www.theguardian.com/world/2026/mar/08/dark-like-our-future-iranians-describe-scenes-of-catastrophe-after-tehrans-oil-depots-bombed](https://www.theguardian.com/world/2026/mar/08/dark-like-our-future-iranians-describe-scenes-of-catastrophe-after-tehrans-oil-depots-bombed)

生成摘要时出错

---

## 65. Lil Finder Guy

**原文标题**: Lil Finder Guy

**原文链接**: [https://basicappleguy.com/basicappleblog/lil-finder-guy](https://basicappleguy.com/basicappleblog/lil-finder-guy)

生成摘要时出错

---

## 66. Amazon holds engineering meeting following AI-related outages

**原文标题**: Amazon holds engineering meeting following AI-related outages

**原文链接**: [https://www.ft.com/content/7cab4ec7-4712-4137-b602-119a44f771de](https://www.ft.com/content/7cab4ec7-4712-4137-b602-119a44f771de)

生成摘要时出错

---

## 67. Rendezvous with Rama

**原文标题**: Rendezvous with Rama

**原文链接**: [https://blog.engora.com/2026/03/rendezvous-with-rama.html](https://blog.engora.com/2026/03/rendezvous-with-rama.html)

生成摘要时出错

---

## 68. Mark Zuckerberg creating new Applied AI engineering company, reorganises teams

**原文标题**: Mark Zuckerberg creating new Applied AI engineering company, reorganises teams

**原文链接**: [https://timesofindia.indiatimes.com/technology/tech-news/mark-zuckerberg-is-creating-new-applied-ai-engineering-company-reorganises-key-teams/articleshow/129018841.cms](https://timesofindia.indiatimes.com/technology/tech-news/mark-zuckerberg-is-creating-new-applied-ai-engineering-company-reorganises-key-teams/articleshow/129018841.cms)

生成摘要时出错

---

## 69. Neural Boids

**原文标题**: Neural Boids

**原文链接**: [https://campedersen.com/noid](https://campedersen.com/noid)

生成摘要时出错

---

## 70. RFC 454545 – Human Em Dash Standard

**原文标题**: RFC 454545 – Human Em Dash Standard

**原文链接**: [https://gist.github.com/bignimbus/a75cc9d703abf0b21a57c0d21a79e2be](https://gist.github.com/bignimbus/a75cc9d703abf0b21a57c0d21a79e2be)

生成摘要时出错

---

## 71. Revealed: UK's multibillion AI drive is built on 'phantom investments'

**原文标题**: Revealed: UK's multibillion AI drive is built on 'phantom investments'

**原文链接**: [https://www.theguardian.com/technology/2026/mar/09/revealed-uks-multibillion-ai-drive-is-built-on-phantom-investments](https://www.theguardian.com/technology/2026/mar/09/revealed-uks-multibillion-ai-drive-is-built-on-phantom-investments)

生成摘要时出错

---

## 72. Hisense TVs add unskippable startup ads before live TV

**原文标题**: Hisense TVs add unskippable startup ads before live TV

**原文链接**: [https://www.guru3d.com/story/hisense-vidaa-tvs-reportedly-add-unskippable-startup-ads-before-live-tv/](https://www.guru3d.com/story/hisense-vidaa-tvs-reportedly-add-unskippable-startup-ads-before-live-tv/)

生成摘要时出错

---

## 73. US blindsides states with surprise settlement in Live Nation/Ticketmaster trial

**原文标题**: US blindsides states with surprise settlement in Live Nation/Ticketmaster trial

**原文链接**: [https://arstechnica.com/tech-policy/2026/03/us-blindsides-states-with-surprise-settlement-in-live-nation-ticketmaster-trial/](https://arstechnica.com/tech-policy/2026/03/us-blindsides-states-with-surprise-settlement-in-live-nation-ticketmaster-trial/)

生成摘要时出错

---

## 74. Algebraic topology: knots links and braids

**原文标题**: Algebraic topology: knots links and braids

**原文链接**: [https://aeb.win.tue.nl/at/algtop-5.html](https://aeb.win.tue.nl/at/algtop-5.html)

生成摘要时出错

---

## 75. Show HN: VS Code Agent Kanban: Task Management for the AI-Assisted Developer

**原文标题**: Show HN: VS Code Agent Kanban: Task Management for the AI-Assisted Developer

**原文链接**: [https://www.appsoftware.com/blog/introducing-vs-code-agent-kanban-task-management-for-the-ai-assisted-developer](https://www.appsoftware.com/blog/introducing-vs-code-agent-kanban-task-management-for-the-ai-assisted-developer)

生成摘要时出错

---

## 76. 60 Minutes Havana Syndrome report finds U.S. government tested energy weapon

**原文标题**: 60 Minutes Havana Syndrome report finds U.S. government tested energy weapon

**原文链接**: [https://www.cbsnews.com/news/60-minutes-havana-syndrome-report-finds-u-s-government-tested-energy-weapon/](https://www.cbsnews.com/news/60-minutes-havana-syndrome-report-finds-u-s-government-tested-energy-weapon/)

生成摘要时出错

---

## 77. Owner of ICE detention facility sees big opportunity in AI man camps

**原文标题**: Owner of ICE detention facility sees big opportunity in AI man camps

**原文链接**: [https://techcrunch.com/2026/03/08/owner-of-ice-detention-facility-sees-big-opportunity-in-ai-man-camps/](https://techcrunch.com/2026/03/08/owner-of-ice-detention-facility-sees-big-opportunity-in-ai-man-camps/)

生成摘要时出错

---

## 78. Microsoft Outlook app now showing paid spam/phishing ad's

**原文标题**: Microsoft Outlook app now showing paid spam/phishing ad's

**原文链接**: [https://imgur.com/a/O9bjjQQ](https://imgur.com/a/O9bjjQQ)

生成摘要时出错

---

## 79. The optimal age to freeze eggs is 19

**原文标题**: The optimal age to freeze eggs is 19

**原文链接**: [https://www.lesswrong.com/posts/dxffBxGqt2eidxwRR/the-optimal-age-to-freeze-eggs-is-19](https://www.lesswrong.com/posts/dxffBxGqt2eidxwRR/the-optimal-age-to-freeze-eggs-is-19)

生成摘要时出错

---

## 80. We Stopped Using the Mathematics That Works

**原文标题**: We Stopped Using the Mathematics That Works

**原文链接**: [https://gfrm.in/posts/why-decision-theory-lost/index.html](https://gfrm.in/posts/why-decision-theory-lost/index.html)

生成摘要时出错

---

## 81. The first airplane fatality

**原文标题**: The first airplane fatality

**原文链接**: [https://www.amusingplanet.com/2026/03/thomas-selfridge-first-airplane-fatality.html](https://www.amusingplanet.com/2026/03/thomas-selfridge-first-airplane-fatality.html)

生成摘要时出错

---

## 82. Things I've Done with AI

**原文标题**: Things I've Done with AI

**原文链接**: [https://sjer.red/blog/2026/built-with-ai/](https://sjer.red/blog/2026/built-with-ai/)

生成摘要时出错

---

## 83. Uber is letting women avoid male drivers and riders in the US

**原文标题**: Uber is letting women avoid male drivers and riders in the US

**原文链接**: [https://www.dexerto.com/entertainment/uber-is-letting-women-avoid-male-drivers-and-riders-in-the-us-3229899/](https://www.dexerto.com/entertainment/uber-is-letting-women-avoid-male-drivers-and-riders-in-the-us-3229899/)

生成摘要时出错

---

## 84. The “JVG algorithm” only wins on tiny numbers

**原文标题**: The “JVG algorithm” only wins on tiny numbers

**原文链接**: [https://scottaaronson.blog/?p=9615](https://scottaaronson.blog/?p=9615)

生成摘要时出错

---

## 85. Ad-tech is fascist tech

**原文标题**: Ad-tech is fascist tech

**原文链接**: [https://pluralistic.net/2026/03/10/ice-tech/#foreseeable-outcomes](https://pluralistic.net/2026/03/10/ice-tech/#foreseeable-outcomes)

生成摘要时出错

---

## 86. Code Review for Claude Code

**原文标题**: Code Review for Claude Code

**原文链接**: [https://claude.com/blog/code-review](https://claude.com/blog/code-review)

生成摘要时出错

---

## 87. Anthropic sues to block Pentagon blacklisting over AI use restrictions

**原文标题**: Anthropic sues to block Pentagon blacklisting over AI use restrictions

**原文链接**: [https://www.reuters.com/world/anthropic-sues-block-pentagon-blacklisting-over-ai-use-restrictions-2026-03-09/](https://www.reuters.com/world/anthropic-sues-block-pentagon-blacklisting-over-ai-use-restrictions-2026-03-09/)

生成摘要时出错

---

## 88. PgAdmin 4 9.13 with AI Assistant Panel

**原文标题**: PgAdmin 4 9.13 with AI Assistant Panel

**原文链接**: [https://www.pgadmin.org/docs/pgadmin4/9.13/query_tool.html#ai-assistant-panel](https://www.pgadmin.org/docs/pgadmin4/9.13/query_tool.html#ai-assistant-panel)

生成摘要时出错

---

## 89. Germany's Solar Boom Eases Power Costs as Gas Price Jumps

**原文标题**: Germany's Solar Boom Eases Power Costs as Gas Price Jumps

**原文链接**: [https://www.bloomberg.com/news/articles/2026-03-06/germany-s-solar-boom-eases-power-costs-as-gas-price-jumps](https://www.bloomberg.com/news/articles/2026-03-06/germany-s-solar-boom-eases-power-costs-as-gas-price-jumps)

生成摘要时出错

---

## 90. Notes on Baking at the South Pole

**原文标题**: Notes on Baking at the South Pole

**原文链接**: [https://www.newyorker.com/culture/the-weekend-essay/the-most-beautiful-freezer-in-the-world](https://www.newyorker.com/culture/the-weekend-essay/the-most-beautiful-freezer-in-the-world)

生成摘要时出错

---

## 91. House Committee Passes Child "Safety" Bills That Push National Age Verification

**原文标题**: House Committee Passes Child "Safety" Bills That Push National Age Verification

**原文链接**: [https://reclaimthenet.org/child-safety-bills-age-verification-surveillance-concerns](https://reclaimthenet.org/child-safety-bills-age-verification-surveillance-concerns)

生成摘要时出错

---

## 92. Getting Started in Common Lisp

**原文标题**: Getting Started in Common Lisp

**原文链接**: [https://lisp-stat.dev/blog/2026/03/09/getting-started/](https://lisp-stat.dev/blog/2026/03/09/getting-started/)

生成摘要时出错

---

## 93. Oil is near a price that hurts the economy

**原文标题**: Oil is near a price that hurts the economy

**原文链接**: [https://www.wsj.com/business/energy-oil/oil-is-already-near-a-price-that-hurts-the-economy-3cebcfdc](https://www.wsj.com/business/energy-oil/oil-is-already-near-a-price-that-hurts-the-economy-3cebcfdc)

生成摘要时出错

---

## 94. Claude helped select targets for Iran strikes, possibly including school

**原文标题**: Claude helped select targets for Iran strikes, possibly including school

**原文链接**: [https://twitter.com/robertwrighter/status/2030482402628214841](https://twitter.com/robertwrighter/status/2030482402628214841)

生成摘要时出错

---

## 95. I built a programming language using Claude Code

**原文标题**: I built a programming language using Claude Code

**原文链接**: [https://ankursethi.com/blog/programming-language-claude-code/](https://ankursethi.com/blog/programming-language-claude-code/)

生成摘要时出错

---

## 96. AI doesn't replace white collar work

**原文标题**: AI doesn't replace white collar work

**原文链接**: [https://www.marble.onl/posts/ai_doesnt_replace_work.html](https://www.marble.onl/posts/ai_doesnt_replace_work.html)

生成摘要时出错

---

## 97. Durdraw – ANSI art editor for Unix-like systems

**原文标题**: Durdraw – ANSI art editor for Unix-like systems

**原文链接**: [https://durdraw.org/](https://durdraw.org/)

生成摘要时出错

---

## 98. Grammarly is using our identities without permission

**原文标题**: Grammarly is using our identities without permission

**原文链接**: [https://www.theverge.com/ai-artificial-intelligence/890921/grammarly-ai-expert-reviews](https://www.theverge.com/ai-artificial-intelligence/890921/grammarly-ai-expert-reviews)

生成摘要时出错

---

## 99. Americans aren't facing a democratic collapse. We're living in its aftermath

**原文标题**: Americans aren't facing a democratic collapse. We're living in its aftermath

**原文链接**: [https://www.theguardian.com/global/commentisfree/2026/mar/08/trump-democracy-oligarchy-policy](https://www.theguardian.com/global/commentisfree/2026/mar/08/trump-democracy-oligarchy-policy)

生成摘要时出错

---

## 100. Show HN: I Was Here – Draw on street view, others can find your drawings

**原文标题**: Show HN: I Was Here – Draw on street view, others can find your drawings

**原文链接**: [https://washere.live](https://washere.live)

生成摘要时出错

---

