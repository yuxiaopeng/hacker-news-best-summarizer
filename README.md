# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-03-27.md)

*最后自动更新时间: 2026-03-27 20:06:20*
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

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 2 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 3 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 4 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 5 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 6 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 7 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 8 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 9 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 10 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 11 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 12 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 13 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 14 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 15 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 16 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 17 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 18 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 19 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 20 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 21 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 22 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 23 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 24 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 25 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 26 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 27 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 28 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 29 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 30 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 31 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 32 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 33 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 34 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 35 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 36 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 37 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 38 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 39 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 40 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 41 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 42 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 43 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 44 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 45 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 46 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 47 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 48 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 49 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 50 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 51 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 52 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 53 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 54 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 55 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 56 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 57 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 58 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 59 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 60 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 61 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 62 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 63 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 64 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 65 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 66 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 67 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 68 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 69 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 70 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 71 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 72 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 73 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 74 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 75 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 76 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 77 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 78 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 79 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 80 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 81 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 82 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 83 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 84 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 85 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 86 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 87 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 88 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 89 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 90 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 91 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 92 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 93 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 94 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 95 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 96 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 97 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 98 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 99 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 100 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 101 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 102 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 103 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 104 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 105 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 106 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 107 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 108 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 109 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 110 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 111 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 112 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 113 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 114 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 115 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 116 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 117 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 118 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 119 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 120 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 121 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 122 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 123 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 124 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 125 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 126 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 127 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 128 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 129 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 130 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 131 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 132 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 133 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 134 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 135 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 136 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 137 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 138 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 139 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 140 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
