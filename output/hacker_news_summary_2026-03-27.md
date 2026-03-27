# Hacker News 热门文章摘要 (2026-03-27)

这是今日 [Hacker News](https://news.ycombinator.com/) 上最热门的文章摘要。

## 1. 欧盟仍然想扫描你的私人信息和照片

**原文标题**: The EU still wants to scan  your private messages and photos

**原文链接**: [https://fightchatcontrol.eu/?foo=bar](https://fightchatcontrol.eu/?foo=bar)

该文章主要通过其标题传达，强调了人们持续的担忧，即欧盟打算实施允许扫描私人信息和照片的措施。

随附的极简内容，由表情符号和社交媒体账号组成，旨在为这个常被称为“聊天控制”的争议性问题提供背景信息。这些表情符号象征着争论的关键方面：**📡️**（数字通信监控）、**⚖️**（安全与隐私权之间的法律和伦理困境）、**🎯**（常以儿童保护为由的既定目标）、**👨‍👩‍👧‍👦**（对普通公民和家庭的影响）以及**🌍**（该提案在欧盟范围内的影响）。

包含“@chatcontrol@mastodon.social”特别是“@fightchatcontrol”等社交媒体账号，直接指出了公众和活动家对强制扫描私人数字内容的积极反对，凸显了欧盟内部抵制此类立法的持续努力。

---

## 2. 用事故车零件在桌上运行特斯拉Model 3电脑

**原文标题**: Running Tesla Model 3's computer on my desk using parts from crashed cars

**原文链接**: [https://bugs.xdavidhu.me/tesla/2026/03/23/running-tesla-model-3s-computer-on-my-desk-using-parts-from-crashed-cars/](https://bugs.xdavidhu.me/tesla/2026/03/23/running-tesla-model-3s-computer-on-my-desk-using-parts-from-crashed-cars/)

作者启动了一个项目，旨在将其特斯拉Model 3的电脑（包括媒体控制单元MCU和自动驾驶电脑）放在桌面上运行，进行安全研究，以期参与特斯拉的漏洞赏金计划。他们从eBay上列出的事故车中采购了这些组件以及一个触摸屏，还购买了一个能够提供10A电流的12V直流电源。

最大的障碍是获取连接MCU与屏幕的特定6针Rosenberger显示电缆。尽管特斯拉的公开电气参考资料提供了引脚定义和零件编号，但该电缆并未单独出售。尝试使用外观相似的宝马LVDS电缆失败了，因为连接器不兼容，这导致一次拙劣的直接接线尝试，短路了MCU上的一个电源控制器芯片，因此不得不进行维修并购买第二台电脑。

最终，作者发现所需的电缆仅作为更大型的“仪表板线束”的一部分进行生产。购买了这套完整的线束后，系统成功启动，并在触摸屏上显示了汽车的操作系统。

初步调查显示，MCU上有一个内部以太网（192.168.90.X/24），上面有可访问的服务，其中包括一个SSH服务器（需要特斯拉签名的密钥，但会向发现漏洞的研究人员提供root权限），以及一个在8080端口上运行的、名为“ODIN”的类REST API，特斯拉的诊断工具会使用它。随着系统成功运行，作者计划进一步研究用户界面、网络接口、CAN总线以及固件提取。

---

## 3. 个人百科

**原文标题**: Personal Encyclopedias

**原文链接**: [https://whoami.wiki/blog/personal-encyclopedias](https://whoami.wiki/blog/personal-encyclopedias)

生成摘要时出错

---

## 4. 我们还没见到赌博和预测市场会带来的最坏影响。

**原文标题**: We haven't seen the worst of what gambling and prediction markets will do

**原文链接**: [https://www.derekthompson.org/p/we-havent-seen-the-worst-of-what](https://www.derekthompson.org/p/we-havent-seen-the-worst-of-what)

文章警告称，赌博和预测市场对美国社会构成了一种被低估的严重威胁，其影响远超娱乐范畴。文章举例指出，有棒球投手为区区小钱操纵投球；在美军轰炸伊朗前数小时出现可疑的高额投注，暗示存在内幕消息；以及赌客威胁记者篡改战争报道以影响市场赔付。

自2018年以来，体育博彩每年从50亿美元激增至1600亿美元，规模已与航空业不相上下。预测市场将这种趋势延伸到生活的几乎每个方面，从名人事件到地缘政治危机，比如饥荒，作者称之为“怪诞”。这种不受限制的扩张带来了四大主要风险：个人赌客成瘾和破产人数增加；赌徒对运动员和记者进行辱骂和威胁；机构信任度急剧下降（例如，三分之二的美国人认为运动员操纵比赛）；以及最黑暗的风险——政治腐败，即官员可能将政策与投注立场挂钩，或利用内幕信息牟利，从而有效地“操纵”政治结果。

在一个信任度低的社会中，当投票和新闻等传统机构被视为已遭破坏时，市场——以其明确的输赢——已成为一种“最终的美德”。金钱取代了爱国主义、宗教和社区，成为道德仲裁者，通过将共同身份溶解为个人风险，并助长与信息对立的关系，从而侵蚀文化。作者总结道，如果没有防护措施，这将导致普遍的欺诈、不信任和犬儒主义。

---

## 5. 「聊天控制」告终：欧盟议会叫停大规模监控

**原文标题**: End of "Chat Control": EU parliament stops mass surveillance

**原文链接**: [https://www.patrick-breyer.de/en/end-of-chat-control-eu-parliament-stops-mass-surveillance-in-voting-thriller-paving-the-way-for-genuine-child-protection/](https://www.patrick-breyer.de/en/end-of-chat-control-eu-parliament-stops-mass-surveillance-in-voting-thriller-paving-the-way-for-genuine-child-protection/)

欧洲议会已投票决定终止“聊天监控”（Chat Control），停止了欧盟境内对私人消息的大规模监控。在一次险胜的投票中，议会首先否决了对未知私人照片和文本的自动评估，随后导致整个提案未能通过。截至4月4日，Meta、谷歌和微软等美国科技公司必须停止对欧洲公民私人聊天的无差别扫描，从而恢复了数字隐私。

这项决定并未造成法律真空；基于司法搜查令的定向监控、对公开帖子的扫描以及用户举报仍然是被允许的。文章指出，“聊天监控”是一次彻底的失败：其算法不可靠，容易被犯罪分子绕过，并产生了大量无关报告（德国为48%），使警方不堪重负。它还将未成年人定罪，且与定罪之间没有可衡量的关联，随着端到端加密的普及而变得过时。99%的报告仅来自Meta，该公司实际上充当了私人辅助警察部队的角色。

尽管取得了这场胜利，斗争仍在继续。关于一项永久性“聊天监控2.0”法规的谈判仍在进行中，欧盟各国政府仍在推动无差别扫描。此外，对消息服务和应用商店强制进行年龄验证，威胁着匿名通信。帕特里克·布雷耶（Patrick Breyer）等倡导者呼吁进行范式转变：通过“设计安全”（security by design）来防止滥用，进行定向监控，并由欧盟儿童保护中心主动删除非法材料，从而摆脱有缺陷的大规模监控策略。

---

## 6. 苹果停产Mac Pro

**原文标题**: Apple discontinues the Mac Pro

**原文链接**: [https://9to5mac.com/2026/03/26/apple-discontinues-the-mac-pro/](https://9to5mac.com/2026/03/26/apple-discontinues-the-mac-pro/)

Apple 已正式停产 Mac Pro，并于2026年3月26日向 9to5Mac 证实，没有未来硬件计划。该产品已从苹果官网移除，其“购买”页面现已重定向至 Mac 电脑主页。

这一决定是在 Mac Pro 停滞不前之后做出的，它最后一次更新是在2023年6月，搭载 M2 Ultra 芯片，此后再无更新，价格仍为6,999美元。Mac Studio 在去年获得了更强大的 M3 Ultra 芯片，现已定位为苹果主要的“专业级”台式电脑。Mac Studio 可配置 M3 Ultra 芯片、32 核 CPU、80 核 GPU、最高 256GB 统一内存和 16TB 固态硬盘存储。于2019年与 Mac Pro 一同发布的 Pro Display XDR 显示器也于本月早些时候停产。

随着 Mac Pro 的移除，苹果的台式电脑产品线现在包括 24 英寸 iMac (M4)、Mac mini (M4 和 M4 Pro) 和 Mac Studio (M4 Max 和 M3 Ultra)。其笔记本电脑产品则有 MacBook Neo、MacBook Air 和 MacBook Pro。作者认为这是多年来最强大的 Mac 产品线，提供了多样化的选择。最近的 macOS Tahoe 26.2 更新，通过 Thunderbolt 5 实现了 RDMA 连接多台 Mac，进一步暗示了 Mac Pro 的必要性正在减弱。作者总结道，停产过时的 Mac Pro 是正确的战略举措，优先发展 Mac Studio 的未来。

---

## 7. Moving from GitHub to Codeberg, for lazy people

**原文标题**: Moving from GitHub to Codeberg, for lazy people

**原文链接**: [https://unterwaditzer.net/2025/codeberg.html](https://unterwaditzer.net/2025/codeberg.html)

This article, "Moving from GitHub to Codeberg, for lazy people," offers a practical guide for migrating repositories, aiming to simplify the process for hesitant users. The author notes that Codeberg has matured, making the transition smoother than anticipated.

Key aspects of the migration include:
1.  **Issues, Pull Requests, Releases:** This is the easiest part. Codeberg's repository import feature from GitHub works seamlessly, preserving issue numbers, labels, and authorship, with a UI very similar to GitHub's.
2.  **GitHub Pages:** `codeberg.page` serves as a direct alternative, functioning much like the old GitHub Pages by pushing HTML to a branch. Alternatives like `grebedoc.dev` or `statichost.eu` are also mentioned.
3.  **Continuous Integration (CI):** This is the "nastiest part." Users lose GitHub's free macOS runners and infinite public repo capacity. Recommendations include cross-compilation and self-hosting a runner for Forgejo Actions. Forgejo Actions is preferred over Woodpecker CI for its familiarity, closely mirroring GitHub Actions' UI and YAML syntax, allowing existing workflows to largely work by just updating `uses:` paths. For essential macOS runners, the author suggests maintaining GitHub Actions on the GitHub repo, mirroring commits from Codeberg, and syncing CI status.
4.  **Old GitHub Repository:** The advice is to update the README and archive the repo. Destructive actions like disabling issues are discouraged due to data loss. While mirroring commits is an option, it requires careful management to prevent continued user interaction on GitHub.

---

## 8. 让生活更轻松、告别抓狂的 Shell 技巧

**原文标题**: Shell Tricks That Make Life Easier (and Save Your Sanity)

**原文链接**: [https://blog.hofstede.it/shell-tricks-that-actually-make-life-easier-and-save-your-sanity/](https://blog.hofstede.it/shell-tricks-that-actually-make-life-easier-and-save-your-sanity/)

本文强调许多工程师未充分利用强大的shell功能，导致工作流程效率低下和沮丧。它将shell技巧分为适用于通用类POSIX shell的“几乎处处可用（Works (Almost) Everywhere）”和适用于现代交互式shell的“Bash和Zsh舒适区（Bash & Zsh Comfort Zone）”。

通用技巧包括Emacs风格的行编辑快捷键，例如`CTRL+W`（删除单词）、`CTRL+U`/`K`（剪切到行首/行尾）、`CTRL+A`/`E`（跳转到行首/行尾）以及`ALT+B`/`F`（逐词移动）。其他重要提示包括用于终端恢复的`reset`、用于命令控制/退出的`CTRL+C`/`D`、用于清屏的`CTRL+L`、用于目录切换的`cd -`、用于目录栈管理的`pushd`/`popd`、用于即时文件截断的`> file.txt`、用于获取上一个参数的`$_`以及用于健壮脚本编写的`set -e`/`set -u`。

Bash和Zsh特有的增强功能包括用于反向历史搜索的`CTRL+R`、用于重复上一个命令的`!!`（例如与`sudo`一起使用）、用于在文本编辑器中编辑复杂命令的`CTRL+X, CTRL+E`或`fc`、用于插入上一个参数的`ESC+.`（或`ALT+.`）、用于高效备份/重命名的花括号扩展（`file{,.bak}`）、进程替换（`diff <(sort file1)`）、用于递归文件匹配的`**`（globstar），以及用于分离后台进程的`CTRL+Z`、`bg`、`disown`。最后，`command |& tee file.log`在显示输出的同时记录标准输出和标准错误。作者敦促用户逐步整合这些技巧，将shell转变为更高效的工具。

---

## 9. European Parliament decided that Chat Control 1.0 must stop

**原文标题**: European Parliament decided that Chat Control 1.0 must stop

**原文链接**: [https://bsky.app/profile/tuta.com/post/3mhxkfowv322c](https://bsky.app/profile/tuta.com/post/3mhxkfowv322c)

生成摘要时出错

---

## 10. Hold on to Your Hardware

**原文标题**: Hold on to Your Hardware

**原文链接**: [https://xn--gckvb8fzb.com/hold-on-to-your-hardware/](https://xn--gckvb8fzb.com/hold-on-to-your-hardware/)

生成摘要时出错

---

## 11. The 'paperwork flood': How I drowned a bureaucrat before dinner

**原文标题**: The 'paperwork flood': How I drowned a bureaucrat before dinner

**原文链接**: [https://sightlessscribbles.com/posts/the-paperwork-flood/](https://sightlessscribbles.com/posts/the-paperwork-flood/)

生成摘要时出错

---

## 12. Apple randomly closes bug reports unless you "verify" the bug remains unfixed

**原文标题**: Apple randomly closes bug reports unless you "verify" the bug remains unfixed

**原文链接**: [https://lapcatsoftware.com/articles/2026/3/11.html](https://lapcatsoftware.com/articles/2026/3/11.html)

生成摘要时出错

---

## 13. $500 GPU outperforms Claude Sonnet on coding benchmarks

**原文标题**: $500 GPU outperforms Claude Sonnet on coding benchmarks

**原文链接**: [https://github.com/itigges22/ATLAS](https://github.com/itigges22/ATLAS)

生成摘要时出错

---

## 14. Judge blocks Pentagon effort to 'punish' Anthropic with supply chain risk label

**原文标题**: Judge blocks Pentagon effort to 'punish' Anthropic with supply chain risk label

**原文链接**: [https://www.cnn.com/2026/03/26/business/anthropic-pentagon-injunction-supply-chain-risk](https://www.cnn.com/2026/03/26/business/anthropic-pentagon-injunction-supply-chain-risk)

生成摘要时出错

---

## 15. My minute-by-minute response to the LiteLLM malware attack

**原文标题**: My minute-by-minute response to the LiteLLM malware attack

**原文链接**: [https://futuresearch.ai/blog/litellm-attack-transcript/](https://futuresearch.ai/blog/litellm-attack-transcript/)

生成摘要时出错

---

## 16. Updates to GitHub Copilot interaction data usage policy

**原文标题**: Updates to GitHub Copilot interaction data usage policy

**原文链接**: [https://github.blog/news-insights/company-news/updates-to-github-copilot-interaction-data-usage-policy/](https://github.blog/news-insights/company-news/updates-to-github-copilot-interaction-data-usage-policy/)

生成摘要时出错

---

## 17. Olympic Committee bars transgender athletes from women’s events

**原文标题**: Olympic Committee bars transgender athletes from women’s events

**原文链接**: [https://www.nytimes.com/2026/03/26/world/olympics/ioc-transgender-athletes-ban.html?unlocked_article_code=1.WFA.U8U0.iEs61HsUkQj5](https://www.nytimes.com/2026/03/26/world/olympics/ioc-transgender-athletes-ban.html?unlocked_article_code=1.WFA.U8U0.iEs61HsUkQj5)

生成摘要时出错

---

## 18. False claims in a widely-cited paper

**原文标题**: False claims in a widely-cited paper

**原文链接**: [https://statmodeling.stat.columbia.edu/2026/03/24/false-claims-in-a-published-no-corrections-no-consequences-welcome-to-the-business-school/](https://statmodeling.stat.columbia.edu/2026/03/24/false-claims-in-a-published-no-corrections-no-consequences-welcome-to-the-business-school/)

生成摘要时出错

---

## 19. A Faster Alternative to Jq

**原文标题**: A Faster Alternative to Jq

**原文链接**: [https://micahkepe.com/blog/jsongrep/](https://micahkepe.com/blog/jsongrep/)

生成摘要时出错

---

## 20. FreeCAD  v1.1

**原文标题**: FreeCAD  v1.1

**原文链接**: [https://blog.freecad.org/2026/03/25/freecad-version-1-1-released/](https://blog.freecad.org/2026/03/25/freecad-version-1-1-released/)

生成摘要时出错

---

## 21. Swift 6.3

**原文标题**: Swift 6.3

**原文链接**: [https://www.swift.org/blog/swift-6.3-released/](https://www.swift.org/blog/swift-6.3-released/)

生成摘要时出错

---

## 22. Show HN: I put an AI agent on a $7/month VPS with IRC as its transport layer

**原文标题**: Show HN: I put an AI agent on a $7/month VPS with IRC as its transport layer

**原文链接**: [https://georgelarson.me/writing/2026-03-23-nullclaw-doorman/](https://georgelarson.me/writing/2026-03-23-nullclaw-doorman/)

生成摘要时出错

---

## 23. People inside Microsoft are fighting to drop mandatory Microsoft Account

**原文标题**: People inside Microsoft are fighting to drop mandatory Microsoft Account

**原文链接**: [https://www.windowscentral.com/microsoft/windows-11/people-inside-microsoft-are-fighting-to-drop-windows-11s-mandatory-microsoft-account-requirements-during-setup](https://www.windowscentral.com/microsoft/windows-11/people-inside-microsoft-are-fighting-to-drop-windows-11s-mandatory-microsoft-account-requirements-during-setup)

生成摘要时出错

---

## 24. New York City hospitals drop Palantir as controversial AI firm expands in UK

**原文标题**: New York City hospitals drop Palantir as controversial AI firm expands in UK

**原文链接**: [https://www.theguardian.com/technology/2026/mar/26/new-york-hospitals-palantir-ai](https://www.theguardian.com/technology/2026/mar/26/new-york-hospitals-palantir-ai)

生成摘要时出错

---

## 25. Landmark L.A. jury verdict finds Instagram, YouTube were designed to addict kids

**原文标题**: Landmark L.A. jury verdict finds Instagram, YouTube were designed to addict kids

**原文链接**: [https://www.latimes.com/california/story/2026-03-25/social-media-lawsuit-trial-meta-google-verdict](https://www.latimes.com/california/story/2026-03-25/social-media-lawsuit-trial-meta-google-verdict)

生成摘要时出错

---

## 26. John Bradley, author of xv, has died

**原文标题**: John Bradley, author of xv, has died

**原文链接**: [https://voxday.net/2026/03/25/rip-john-bradley/](https://voxday.net/2026/03/25/rip-john-bradley/)

生成摘要时出错

---

## 27. Government agencies buy commercial data about Americans in bulk

**原文标题**: Government agencies buy commercial data about Americans in bulk

**原文链接**: [https://www.npr.org/2026/03/25/nx-s1-5752369/ice-surveillance-data-brokers-congress-anthropic](https://www.npr.org/2026/03/25/nx-s1-5752369/ice-surveillance-data-brokers-congress-anthropic)

生成摘要时出错

---

## 28. Schedule tasks on the web

**原文标题**: Schedule tasks on the web

**原文链接**: [https://code.claude.com/docs/en/web-scheduled-tasks](https://code.claude.com/docs/en/web-scheduled-tasks)

生成摘要时出错

---

## 29. Anatomy of the .claude/ folder

**原文标题**: Anatomy of the .claude/ folder

**原文链接**: [https://blog.dailydoseofds.com/p/anatomy-of-the-claude-folder](https://blog.dailydoseofds.com/p/anatomy-of-the-claude-folder)

生成摘要时出错

---

## 30. We rewrote JSONata with AI in a day, saved $500k/year

**原文标题**: We rewrote JSONata with AI in a day, saved $500k/year

**原文链接**: [https://www.reco.ai/blog/we-rewrote-jsonata-with-ai](https://www.reco.ai/blog/we-rewrote-jsonata-with-ai)

生成摘要时出错

---

## 31. Using FireWire on a Raspberry Pi

**原文标题**: Using FireWire on a Raspberry Pi

**原文链接**: [https://www.jeffgeerling.com/blog/2026/firewire-on-a-raspberry-pi/](https://www.jeffgeerling.com/blog/2026/firewire-on-a-raspberry-pi/)

生成摘要时出错

---

## 32. Last gasps of the rent seeking class?

**原文标题**: Last gasps of the rent seeking class?

**原文链接**: [https://geohot.github.io//blog/jekyll/update/2026/02/26/the-last-gasps-of-the-rent-seeking-class.html](https://geohot.github.io//blog/jekyll/update/2026/02/26/the-last-gasps-of-the-rent-seeking-class.html)

生成摘要时出错

---

## 33. The European AllSky7 fireball network

**原文标题**: The European AllSky7 fireball network

**原文链接**: [https://www.allsky7.net/#archive](https://www.allsky7.net/#archive)

生成摘要时出错

---

## 34. Chicago artist creates tourism posters for city's neighborhoods

**原文标题**: Chicago artist creates tourism posters for city's neighborhoods

**原文链接**: [https://www.chicagotribune.com/2026/03/25/chicago-neighborhood-posters/](https://www.chicagotribune.com/2026/03/25/chicago-neighborhood-posters/)

生成摘要时出错

---

## 35. Anthropic Subprocessor Changes

**原文标题**: Anthropic Subprocessor Changes

**原文链接**: [https://trust.anthropic.com](https://trust.anthropic.com)

生成摘要时出错

---

## 36. Building a Blog with Elixir and Phoenix

**原文标题**: Building a Blog with Elixir and Phoenix

**原文链接**: [https://jola.dev/posts/building-a-blog-with-elixir-and-phoenix](https://jola.dev/posts/building-a-blog-with-elixir-and-phoenix)

生成摘要时出错

---

## 37. I am leaving the AI party after one drink

**原文标题**: I am leaving the AI party after one drink

**原文链接**: [https://lara-aigmueller.at/thoughts/leaving-the-ai-party/](https://lara-aigmueller.at/thoughts/leaving-the-ai-party/)

生成摘要时出错

---

## 38. Show HN: Fio: 3D World editor/game engine – inspired by Radiant and Hammer

**原文标题**: Show HN: Fio: 3D World editor/game engine – inspired by Radiant and Hammer

**原文链接**: [https://github.com/ViciousSquid/Fio](https://github.com/ViciousSquid/Fio)

生成摘要时出错

---

## 39. Day 1 of ARC-AGI-3

**原文标题**: Day 1 of ARC-AGI-3

**原文链接**: [https://www.symbolica.ai/blog/arc-agi-3](https://www.symbolica.ai/blog/arc-agi-3)

生成摘要时出错

---

## 40. Show HN: Veil – Dark mode PDFs without destroying images, runs in the browser

**原文标题**: Show HN: Veil – Dark mode PDFs without destroying images, runs in the browser

**原文链接**: [https://veil.simoneamico.com/](https://veil.simoneamico.com/)

生成摘要时出错

---

## 41. Meow.camera

**原文标题**: Meow.camera

**原文链接**: [https://meow.camera/#4258783365322591678](https://meow.camera/#4258783365322591678)

生成摘要时出错

---

## 42. Apple says no one using Lockdown Mode has been hacked with spyware

**原文标题**: Apple says no one using Lockdown Mode has been hacked with spyware

**原文链接**: [https://techcrunch.com/2026/03/27/apple-says-no-one-using-lockdown-mode-has-been-hacked-with-spyware/](https://techcrunch.com/2026/03/27/apple-says-no-one-using-lockdown-mode-has-been-hacked-with-spyware/)

生成摘要时出错

---

## 43. Laws Suppressing Boycotts of Israel Violate Civil Liberties

**原文标题**: Laws Suppressing Boycotts of Israel Violate Civil Liberties

**原文链接**: [https://www.aclu.org/news/free-speech/laws-suppressing-boycotts-israel-dont-prevent-discrimination-they-violate-civil](https://www.aclu.org/news/free-speech/laws-suppressing-boycotts-israel-dont-prevent-discrimination-they-violate-civil)

生成摘要时出错

---

## 44. Telnyx package compromised on PyPI

**原文标题**: Telnyx package compromised on PyPI

**原文链接**: [https://www.aikido.dev/blog/telnyx-pypi-compromised-teampcp-canisterworm](https://www.aikido.dev/blog/telnyx-pypi-compromised-teampcp-canisterworm)

生成摘要时出错

---

## 45. Show HN: Robust LLM extractor for websites in TypeScript

**原文标题**: Show HN: Robust LLM extractor for websites in TypeScript

**原文链接**: [https://github.com/lightfeed/extractor](https://github.com/lightfeed/extractor)

生成摘要时出错

---

## 46. Author of Red Mars calls 'bullshit' on emigrating to the planet

**原文标题**: Author of Red Mars calls 'bullshit' on emigrating to the planet

**原文链接**: [https://www.newscientist.com/article/2520312-author-of-red-mars-calls-bullshit-on-emigrating-to-the-planet/](https://www.newscientist.com/article/2520312-author-of-red-mars-calls-bullshit-on-emigrating-to-the-planet/)

生成摘要时出错

---

## 47. Iran oil revenue soars as it's the only exporter out of Hormuz

**原文标题**: Iran oil revenue soars as it's the only exporter out of Hormuz

**原文链接**: [https://financialpost.com/commodities/energy/oil-gas/iran-oil-revenue-soars-hormuz](https://financialpost.com/commodities/energy/oil-gas/iran-oil-revenue-soars-hormuz)

生成摘要时出错

---

## 48. Meta and YouTube Found Negligent in Social-Media Addiction Trial

**原文标题**: Meta and YouTube Found Negligent in Social-Media Addiction Trial

**原文链接**: [https://www.wsj.com/tech/personal-tech/meta-and-youtube-found-negligent-in-social-media-addiction-trial-35b2830d](https://www.wsj.com/tech/personal-tech/meta-and-youtube-found-negligent-in-social-media-addiction-trial-35b2830d)

生成摘要时出错

---

## 49. The Little Book of C

**原文标题**: The Little Book of C

**原文链接**: [https://little-book-of.github.io/c/books/en-US/book.html](https://little-book-of.github.io/c/books/en-US/book.html)

生成摘要时出错

---

## 50. Chroma Context-1: Training a Self-Editing Search Agent

**原文标题**: Chroma Context-1: Training a Self-Editing Search Agent

**原文链接**: [https://www.trychroma.com/research/context-1](https://www.trychroma.com/research/context-1)

生成摘要时出错

---

## 51. Memorial to IT Workers Who Have Fallen in Ukraine

**原文标题**: Memorial to IT Workers Who Have Fallen in Ukraine

**原文链接**: [https://dou.ua/memorial/](https://dou.ua/memorial/)

生成摘要时出错

---

## 52. Drone attack on parked U.S. Army BlackHawk in Iraq

**原文标题**: Drone attack on parked U.S. Army BlackHawk in Iraq

**原文链接**: [https://www.twz.com/air/drone-attack-on-parked-u-s-army-black-hawk-in-iraq-a-harbinger-of-whats-to-come](https://www.twz.com/air/drone-attack-on-parked-u-s-army-black-hawk-in-iraq-a-harbinger-of-whats-to-come)

生成摘要时出错

---

## 53. Zero Days: Electric Motorcycles Are a Security Nightmare

**原文标题**: Zero Days: Electric Motorcycles Are a Security Nightmare

**原文链接**: [https://persephonekarnstein.github.io/post/zero-days/](https://persephonekarnstein.github.io/post/zero-days/)

生成摘要时出错

---

## 54. Netflix raises prices for every subscription tier by up to 12.5 percent

**原文标题**: Netflix raises prices for every subscription tier by up to 12.5 percent

**原文链接**: [https://arstechnica.com/gadgets/2026/03/netflix-increases-prices-for-all-plans-by-up-to-2-per-month/](https://arstechnica.com/gadgets/2026/03/netflix-increases-prices-for-all-plans-by-up-to-2-per-month/)

生成摘要时出错

---

## 55. Claude loses its >99% uptime in Q1 2026

**原文标题**: Claude loses its >99% uptime in Q1 2026

**原文链接**: [https://bsky.app/profile/teropa.bsky.social/post/3mi2dbt27m226](https://bsky.app/profile/teropa.bsky.social/post/3mi2dbt27m226)

生成摘要时出错

---

## 56. Meta Lays Off 700 Employees, While Rewarding Top Executives

**原文标题**: Meta Lays Off 700 Employees, While Rewarding Top Executives

**原文链接**: [https://www.nytimes.com/2026/03/25/technology/meta-lays-off-700-employees-while-rewarding-top-executives.html](https://www.nytimes.com/2026/03/25/technology/meta-lays-off-700-employees-while-rewarding-top-executives.html)

生成摘要时出错

---

## 57. Airport wait times are longest in TSA history, agency says

**原文标题**: Airport wait times are longest in TSA history, agency says

**原文链接**: [https://www.usatoday.com/story/news/nation/2026/03/25/tsa-line-airport-wait-times-highest-in-history/89314232007/](https://www.usatoday.com/story/news/nation/2026/03/25/tsa-line-airport-wait-times-highest-in-history/89314232007/)

生成摘要时出错

---

## 58. Should QA exist?

**原文标题**: Should QA exist?

**原文链接**: [https://www.rubick.com/should-qa-exist/](https://www.rubick.com/should-qa-exist/)

生成摘要时出错

---

## 59. How much precision can you squeeze out of a table?

**原文标题**: How much precision can you squeeze out of a table?

**原文链接**: [https://www.johndcook.com/blog/2026/03/26/table-precision/](https://www.johndcook.com/blog/2026/03/26/table-precision/)

生成摘要时出错

---

## 60. We broke 92% of SHA-256 – you should start to migrate from it

**原文标题**: We broke 92% of SHA-256 – you should start to migrate from it

**原文链接**: [https://stateofutopia.com/papers/2/we-broke-92-percent-of-sha-256.html](https://stateofutopia.com/papers/2/we-broke-92-percent-of-sha-256.html)

生成摘要时出错

---

## 61. School uses AI to remove 200 books, including Orwell's 1984 and Twilight

**原文标题**: School uses AI to remove 200 books, including Orwell's 1984 and Twilight

**原文链接**: [https://www.lbc.co.uk/article/librarian-gobsmacked-school-ai-remove-books-5HjdWsc_2/](https://www.lbc.co.uk/article/librarian-gobsmacked-school-ai-remove-books-5HjdWsc_2/)

生成摘要时出错

---

## 62. The Military Failures of Fascism

**原文标题**: The Military Failures of Fascism

**原文链接**: [https://acoup.blog/2024/02/23/fireside-friday-february-23-2024-on-the-military-failures-of-fascism/](https://acoup.blog/2024/02/23/fireside-friday-february-23-2024-on-the-military-failures-of-fascism/)

生成摘要时出错

---

## 63. Show HN: Yoink – Spotify to lossless with full metadata, self-hostable, ad-free

**原文标题**: Show HN: Yoink – Spotify to lossless with full metadata, self-hostable, ad-free

**原文链接**: [https://yoinkify.com](https://yoinkify.com)

生成摘要时出错

---

## 64. Anthropic Update on Session Limits

**原文标题**: Anthropic Update on Session Limits

**原文链接**: [https://old.reddit.com/r/Anthropic/comments/1s4iefu/update_on_session_limits/](https://old.reddit.com/r/Anthropic/comments/1s4iefu/update_on_session_limits/)

生成摘要时出错

---

## 65. JCal – Jeffrey Epstein's Activities Recreated in Google Calendar

**原文标题**: JCal – Jeffrey Epstein's Activities Recreated in Google Calendar

**原文链接**: [https://jmail.world/calendar](https://jmail.world/calendar)

生成摘要时出错

---

## 66. Delta Air Lines Says It Will Suspend Special Services for Congress Members

**原文标题**: Delta Air Lines Says It Will Suspend Special Services for Congress Members

**原文链接**: [https://www.nytimes.com/2026/03/24/business/delta-congress-travel-services-suspended.html](https://www.nytimes.com/2026/03/24/business/delta-congress-travel-services-suspended.html)

生成摘要时出错

---

## 67. AMD Announces the Ryzen 9 9950X3D2

**原文标题**: AMD Announces the Ryzen 9 9950X3D2

**原文链接**: [https://www.phoronix.com/news/AMD-Ryzen-9-9950X3D2](https://www.phoronix.com/news/AMD-Ryzen-9-9950X3D2)

生成摘要时出错

---

## 68. A leak reveals that Anthropic is testing a more capable AI model "Claude Mythos"

**原文标题**: A leak reveals that Anthropic is testing a more capable AI model "Claude Mythos"

**原文链接**: [https://fortune.com/2026/03/26/anthropic-says-testing-mythos-powerful-new-ai-model-after-data-leak-reveals-its-existence-step-change-in-capabilities/](https://fortune.com/2026/03/26/anthropic-says-testing-mythos-powerful-new-ai-model-after-data-leak-reveals-its-existence-step-change-in-capabilities/)

生成摘要时出错

---

## 69. Model Collapse Is Happening, We Just Pretend It Isn't

**原文标题**: Model Collapse Is Happening, We Just Pretend It Isn't

**原文链接**: [https://cacm.acm.org/blogcacm/model-collapse-is-already-happening-we-just-pretend-it-isnt/](https://cacm.acm.org/blogcacm/model-collapse-is-already-happening-we-just-pretend-it-isnt/)

生成摘要时出错

---

## 70. Mazda may have found the apex in ICE design with the Skyactiv-Z

**原文标题**: Mazda may have found the apex in ICE design with the Skyactiv-Z

**原文链接**: [https://newatlas.com/automotive/mazda-skyactiv-z/](https://newatlas.com/automotive/mazda-skyactiv-z/)

生成摘要时出错

---

## 71. Netflix Raising U.S. Prices for Second Time in Less Than Two Years

**原文标题**: Netflix Raising U.S. Prices for Second Time in Less Than Two Years

**原文链接**: [https://variety.com/2026/tv/news/netflix-raising-prices-second-time-in-a-year-1236700999/](https://variety.com/2026/tv/news/netflix-raising-prices-second-time-in-a-year-1236700999/)

生成摘要时出错

---

## 72. Chat Control: How Governments and Tech Lobby Try to Overturn EU Parliament

**原文标题**: Chat Control: How Governments and Tech Lobby Try to Overturn EU Parliament

**原文链接**: [https://www.patrick-breyer.de/en/the-battle-over-chat-control-how-eu-governments-and-the-tech-lobby-are-trying-to-overturn-parliaments-vote-a-comprehensive-fact-check/](https://www.patrick-breyer.de/en/the-battle-over-chat-control-how-eu-governments-and-the-tech-lobby-are-trying-to-overturn-parliaments-vote-a-comprehensive-fact-check/)

生成摘要时出错

---

## 73. Rank the 50 best Apple products

**原文标题**: Rank the 50 best Apple products

**原文链接**: [https://www.theverge.com/cs/tech/900477/apple-50-anniversary-rank-products](https://www.theverge.com/cs/tech/900477/apple-50-anniversary-rank-products)

生成摘要时出错

---

## 74. 21,864 Yugoslavian .yu domains

**原文标题**: 21,864 Yugoslavian .yu domains

**原文链接**: [https://jacobfilipp.com/yu/](https://jacobfilipp.com/yu/)

生成摘要时出错

---

## 75. The Oxford Comma – Why and Why Not (2024)

**原文标题**: The Oxford Comma – Why and Why Not (2024)

**原文链接**: [https://www.deborahcourtbooks.com/post/the-oxford-comma-why-and-why-not](https://www.deborahcourtbooks.com/post/the-oxford-comma-why-and-why-not)

生成摘要时出错

---

## 76. Why Sora Failed: $15M/day inference cost vs. $2.1M lifetime revenue

**原文标题**: Why Sora Failed: $15M/day inference cost vs. $2.1M lifetime revenue

**原文链接**: [https://www.revolutioninai.com/2026/03/%20chatgpt-gpt-54-mini-silent-switch-march-2026.html](https://www.revolutioninai.com/2026/03/%20chatgpt-gpt-54-mini-silent-switch-march-2026.html)

生成摘要时出错

---

## 77. Scientists Just Broke the Solar Power Limit Everyone Thought Was Absolute

**原文标题**: Scientists Just Broke the Solar Power Limit Everyone Thought Was Absolute

**原文链接**: [https://scitechdaily.com/scientists-just-broke-the-solar-power-limit-everyone-thought-was-absolute/](https://scitechdaily.com/scientists-just-broke-the-solar-power-limit-everyone-thought-was-absolute/)

生成摘要时出错

---

## 78. Taming LLMs: Using Executable Oracles to Prevent Bad Code

**原文标题**: Taming LLMs: Using Executable Oracles to Prevent Bad Code

**原文链接**: [https://john.regehr.org/writing/zero_dof_programming.html](https://john.regehr.org/writing/zero_dof_programming.html)

生成摘要时出错

---

## 79. HandyMKV for MakeMKV and HandBrake Automation

**原文标题**: HandyMKV for MakeMKV and HandBrake Automation

**原文链接**: [https://github.com/dmars8047/handymkv](https://github.com/dmars8047/handymkv)

生成摘要时出错

---

## 80. Claude Code adjusting down 5hr limits

**原文标题**: Claude Code adjusting down 5hr limits

**原文链接**: [https://twitter.com/trq212/status/2037254607001559305](https://twitter.com/trq212/status/2037254607001559305)

生成摘要时出错

---

## 81. Building FireStriker: Making Civic Tech Free

**原文标题**: Building FireStriker: Making Civic Tech Free

**原文链接**: [https://firestriker.org/blog/building-firestriker-why-im-making-civic-tech-free](https://firestriker.org/blog/building-firestriker-why-im-making-civic-tech-free)

生成摘要时出错

---

## 82. Grove: Distributed ML Training over AirDrop

**原文标题**: Grove: Distributed ML Training over AirDrop

**原文链接**: [https://swarnimjain.com/grove](https://swarnimjain.com/grove)

生成摘要时出错

---

## 83. MacBook Neo, the Benchmarks

**原文标题**: MacBook Neo, the Benchmarks

**原文链接**: [https://birchtree.me/blog/macbook-neo-the-benchmarks/](https://birchtree.me/blog/macbook-neo-the-benchmarks/)

生成摘要时出错

---

## 84. Judge's Remarks on Anthropic vs. Pentagon

**原文标题**: Judge's Remarks on Anthropic vs. Pentagon

**原文链接**: [https://www.businessinsider.com/anthropic-pentagon-trump-hearing-judge-rita-lin-remarks-stakes-2026-3](https://www.businessinsider.com/anthropic-pentagon-trump-hearing-judge-rita-lin-remarks-stakes-2026-3)

生成摘要时出错

---

## 85. A Year with the Framework 13

**原文标题**: A Year with the Framework 13

**原文链接**: [https://kevquirk.com/a-year-with-the-framework-13](https://kevquirk.com/a-year-with-the-framework-13)

生成摘要时出错

---

## 86. Make macOS consistently bad (unironically)

**原文标题**: Make macOS consistently bad (unironically)

**原文链接**: [https://lr0.org/blog/p/macos/](https://lr0.org/blog/p/macos/)

生成摘要时出错

---

## 87. Google Just Patented the End of Your Website

**原文标题**: Google Just Patented the End of Your Website

**原文链接**: [https://www.forbes.com/sites/joetoscano1/2026/03/06/google-just-patented-the-end-of-your-website/](https://www.forbes.com/sites/joetoscano1/2026/03/06/google-just-patented-the-end-of-your-website/)

生成摘要时出错

---

## 88. Japan research uncovers how coffee constituent limit growth of colorectal cancer

**原文标题**: Japan research uncovers how coffee constituent limit growth of colorectal cancer

**原文链接**: [https://mainichi.jp/english/articles/20260326/p2a/00m/0sc/002000c](https://mainichi.jp/english/articles/20260326/p2a/00m/0sc/002000c)

生成摘要时出错

---

## 89. Anthropic is preparing to release new models – Mythos and Capybara

**原文标题**: Anthropic is preparing to release new models – Mythos and Capybara

**原文链接**: [https://m1astra-mythos.pages.dev/](https://m1astra-mythos.pages.dev/)

生成摘要时出错

---

