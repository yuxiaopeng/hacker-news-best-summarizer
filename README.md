# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-10-06.md)

*最后自动更新时间: 2026-10-06 01:12:52*
## 1. 在消费级硬件 (RTX 4090) 上以 100T/s 运行 Qwen 3.8 Flash Next (125B)

**原文标题**: Run Qwen 3.8 Flash Next (125B) on consumer hardware (RTX 4090) at 100T/s

**原文链接**: [https://github.com/Niko1221/Strata](https://github.com/Niko1221/Strata)

Strata是一款免费开源工具，允许用户在消费级电脑上运行大型的1250亿参数Qwen 3.8 Flash Next AI模型。它专为NVIDIA RTX 20/30/40/50系列和特定AMD Radeon GPU设计，要求显存至少12 GB，并需要在Windows或Linux系统上至少32 GB内存（所有模型则需64 GB）和80 GB SSD存储空间。

该模型完全在本地运行，确保了聊天、代码生成、图像解析以及与现有应用程序和编码代理集成的隐私性。性能因硬件和模型压缩（例如Q2_0、IQ3_S、Coder）而异，在游戏PC上，“写入答案”速度通常在每秒44-94个token之间，“读取提示”速度为每秒1,100-2,650个token。预计RTX 3090（24GB）生成答案速度可达每秒100-140个token。

安装过程简单，可通过AI编码助手或手动运行脚本进行。安装程序会帮助用户选择模型大小、上下文和图像功能，然后下载约70 GB的模型。首次启动时，由于有35-55 GB的数据加载到内存中，系统可能会减速1-3分钟。用户可以通过 `http://127.0.0.1:8080` 的浏览器应用程序进行交互，或通过与OpenAI/Anthropic兼容的API端点连接其他应用程序。Strata有效地将模型的工作负载分布到GPU、内存、CPU和SSD上，采用“猜测与检查”和批处理等技术以实现最佳性能。

---

## 2. 关闭 macOS 27 上的苹果智能并收回其磁盘空间

**原文标题**: Turn off Apple Intelligence on macOS 27 and get its disk space back

**原文链接**: [https://github.com/omlahore/RemoveMacAI](https://github.com/omlahore/RemoveMacAI)

RemoveMacAI是一款工具，旨在完全禁用macOS 27上的苹果智能功能并释放磁盘空间，因为简单地关闭这些功能并不会移除相关的下载模型。它面向运行macOS 27的搭载Apple芯片的Mac设备。

该工具通过应用配置描述文件来限制苹果智能功能，并将模型下载重定向到一个关闭的本地端口，从而阻止macOS重新下载这些模型。它通过苹果的资产服务来移除模型，同时确保系统完整性保护（SIP）保持启用。

RemoveMacAI会关闭Siri、写作工具、Genmoji、图像游乐场、ChatGPT扩展、各种摘要、邮件智能回复、内联文本预测、空间照片、照片清理和Xcode预测代码补全等功能。然后，它会移除相应的基础模型以及用于图像生成、Genmoji、空间照片、照片清理和Xcode代码补全的模型。听写功能仍然可用，并且这些更改在macOS更新后仍会保留。

通过一条curl命令或Homebrew即可轻松安装。用户可以查看当前状态（`removemacai status`），有选择地保留某些功能（`removemacai off --keep <features>`），或撤销所有更改（`removemacai revert`）。此过程需要用户批准配置描述文件的安装。

该工具不进行网络请求，不收集任何数据。它基于`pared`工具开发，并在MIT许可下开源。作者Om Lahore对新职位持开放态度。

---

## 3. 我们将需要对几乎所有方面都设定默认的硬性预算上限。

**原文标题**: We're going to need default hard budget caps on pretty much everything

**原文链接**: [https://simonwillison.net/2026/Oct/3/default-hard-budget-caps/](https://simonwillison.net/2026/Oct/3/default-hard-budget-caps/)

这篇文章主张紧急实施对按用量付费服务和API的默认硬性预算上限。作者认为，通过AI代理（编码代理和个人代理）部署代码的日益便捷，加剧了用户因付费API、托管应用程序或存储/计算等服务而产生巨额、意想不到费用的风险。仅发出警告的软性上限被认为不足，因为服务可能一夜之间累积大量费用。相反，一旦超出预设的每月预算，硬性上限将自动切断服务并返回错误。虽然企业可能会担心应用程序报错，但作者坚称，错误远比超过1万美元的意外账单好得多。该提案建议将硬性上限设为默认设置，对于愿意接受无上限费用的用户，则需要明确选择退出。AWS被特别指出是急需此功能的服务，因为有许多用户因个人项目上的失控费用而“蒙受损失”的故事。令人鼓舞的是，AWS于2026年9月推出了“支出限制”功能（目前处于有限发布阶段），该功能在达到每月限额时会暂停项目。谷歌云于2026年7月也推出了类似的“费用上限”功能，这表明了积极的行业趋势。文章最后希望AI代理能很快推荐具有硬性预算上限的服务提供商，并警告用户避免使用无上限服务。

---

## 4. 不当遮蔽泄露谷歌数据中心水电用量

**原文标题**: Improper redaction reveals Google Data Center water and electricity usage

**原文链接**: [https://www.1011now.com/2026/09/30/more-questions-than-answers-about-lincolns-google-data-center-water-electricity-usage/](https://www.1011now.com/2026/09/30/more-questions-than-answers-about-lincolns-google-data-center-water-electricity-usage/)

KOLN的一项调查显示，由于提交给水、能源和环境部（DWEE）的报告存在不当遮盖，谷歌内布拉斯加州数据中心的敏感运营数据和预计退税额被泄露。谷歌曾声称这些信息，包括用电量和用水量，是商业机密。

通过高亮和复制被遮盖的文本，Agate有限责任公司（谷歌位于林肯的数据中心）的报告显示，其在高峰需求期间的电力消耗为52.65兆瓦，年用水量为13.299兆加仑（1300万加仑），这相当于约20个奥林匹克标准游泳池的水量。Fireball Group有限责任公司（位于帕皮利恩）被确定为用水量最高的公司，报告称2025年用水量为547.88兆加仑。去年，六个报告数据中心共使用了7.65亿加仑水。

此次遮盖失败还暴露了2025年预计的大额退税：Agate有限责任公司预计为5580万美元，Fireball有限责任公司为3910万美元，以及Westwood Solutions有限责任公司（位于奥马哈）为2250万美元。这些报告是根据州长皮伦的行政命令强制要求的，旨在评估数据中心对州资源的影响。

---

## 5. Anthropic报警举报日记内容，女子面临重罪指控。

**原文标题**: Anthropic reported diary entry to police, woman faces felony charge

**原文链接**: [https://www.techspot.com/news/114091-florida-woman-used-claude-diary-anthropic-reported-shoot.html](https://www.techspot.com/news/114091-florida-woman-used-claude-diary-anthropic-reported-shoot.html)

佛罗里达州一名女子凯莉·米歇尔·海勒因据称利用Anthropic公司的Claude AI作为日记，写下关于“血洗”警长办公室的威胁，而面临重罪指控。Claude的安全系统标记了这条记录，随后升级至人工审核员处理。审核员认为其是可信威胁，便将其报告给了执法部门。

Anthropic公司声明，在紧急情况下可能会共享用户信息，以防止死亡或严重的身体伤害。海勒随后被拘留，并依据佛罗里达州法规836.10，因发出书面暴力威胁而被指控犯有二级重罪。

这一事件深刻地警示人们，AI互动中缺乏隐私，以及与聊天机器人分享内容会带来真实世界的后果。此前还有其他备受关注的案件，AI公司因用户生成的威胁而受到审查。OpenAI目前正被不列颠哥伦比亚省起诉，罪名是据称未能阻止一场大规模枪击事件，尽管此前曾标记过一名行凶者关于枪支暴力的对话。佛罗里达州也曾起诉OpenAI，将ChatGPT与过去的枪击事件联系起来。文章警告用户，聊天机器人不是私人日记，并建议对他们输入的信息保持谨慎。

---

## 6. Web Search API

**原文标题**: Web Search API

**原文链接**: [https://developers.cloudflare.com/changelog/post/2026-10-02-introducing-web-search-api/](https://developers.cloudflare.com/changelog/post/2026-10-02-introducing-web-search-api/)

Cloudflare introduced its Web Search API in beta on October 2, 2026, designed to empower AI agents and applications with real-time internet search capabilities. This allows AI to ground responses in live information, overcoming limitations of model training cutoffs or inaccurate URL guessing.

The API operates via Cloudflare's AI Gateway, ensuring all search requests are logged and billed against AI Gateway credits at the respective provider's list API price, without additional markup. Users can also opt to use their own provider API key.

Initially, the Web Search API supports three search providers: Ceramic.ai, Exa, and Linkup. All chosen providers ensure Zero Data Retention for requests made through Cloudflare and comply with Cloudflare's verified bot crawling standards.

Developers can integrate the Web Search API using either a REST API call or by utilizing the AI binding within a Cloudflare Worker. A guide titled "How to use Web Search API" is available for getting started.

---

## 7. 丹麦数据泄露致880万人个人数据外泄

**原文标题**: Denmark data breach exposes 8.8M people's personal data

**原文链接**: [https://www.cpr.dk/cpr-nyt/nyhedsarkiv/2026/okt/omfattende-uautoriseret-adgang-til-borgeres-cpr-oplysninger](https://www.cpr.dk/cpr-nyt/nyhedsarkiv/2026/okt/omfattende-uautoriseret-adgang-til-borgeres-cpr-oplysninger)

生成摘要时出错

---

## 8. 浏览器原生的经典 Visual Basic VB6 IDE

**原文标题**: A browser-native classic Visual Basic VB6 IDE

**原文链接**: [https://wieslawsoltes.github.io/VB6/](https://wieslawsoltes.github.io/VB6/)

生成摘要时出错

---

## 9. Pixel 11 doesn't yet meet the GrapheneOS security standards and may be skipped

**原文标题**: Pixel 11 doesn't yet meet the GrapheneOS security standards and may be skipped

**原文链接**: [https://discuss.grapheneos.org/d/41564-pixel-11-doesnt-yet-meet-the-grapheneos-security-standards-and-may-be-skipped](https://discuss.grapheneos.org/d/41564-pixel-11-doesnt-yet-meet-the-grapheneos-security-standards-and-may-be-skipped)

生成摘要时出错

---

## 10. Germany’s RobCo hits $1B valuation

**原文标题**: Germany’s RobCo hits $1B valuation

**原文链接**: [https://techfundingnews.com/europes-new-robotics-unicorn-germanys-robco-hits-1b-valuation/](https://techfundingnews.com/europes-new-robotics-unicorn-germanys-robco-hits-1b-valuation/)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-10-06](output/hacker_news_summary_2026-10-06.md) |
| 2 | [2026-10-04](output/hacker_news_summary_2026-10-04.md) |
| 3 | [2026-10-01](output/hacker_news_summary_2026-10-01.md) |
| 4 | [2026-09-29](output/hacker_news_summary_2026-09-29.md) |
| 5 | [2026-09-30](output/hacker_news_summary_2026-09-30.md) |
| 6 | [2026-10-02](output/hacker_news_summary_2026-10-02.md) |
| 7 | [2026-09-27](output/hacker_news_summary_2026-09-27.md) |
| 8 | [2026-10-03](output/hacker_news_summary_2026-10-03.md) |
| 9 | [2026-09-24](output/hacker_news_summary_2026-09-24.md) |
| 10 | [2026-09-21](output/hacker_news_summary_2026-09-21.md) |
| 11 | [2026-09-23](output/hacker_news_summary_2026-09-23.md) |
| 12 | [2026-09-20](output/hacker_news_summary_2026-09-20.md) |
| 13 | [2026-09-22](output/hacker_news_summary_2026-09-22.md) |
| 14 | [2026-09-25](output/hacker_news_summary_2026-09-25.md) |
| 15 | [2026-09-16](output/hacker_news_summary_2026-09-16.md) |
| 16 | [2026-09-14](output/hacker_news_summary_2026-09-14.md) |
| 17 | [2026-09-17](output/hacker_news_summary_2026-09-17.md) |
| 18 | [2026-09-19](output/hacker_news_summary_2026-09-19.md) |
| 19 | [2026-09-18](output/hacker_news_summary_2026-09-18.md) |
| 20 | [2026-09-15](output/hacker_news_summary_2026-09-15.md) |
| 21 | [2026-09-09](output/hacker_news_summary_2026-09-09.md) |
| 22 | [2026-09-10](output/hacker_news_summary_2026-09-10.md) |
| 23 | [2026-09-13](output/hacker_news_summary_2026-09-13.md) |
| 24 | [2026-09-08](output/hacker_news_summary_2026-09-08.md) |
| 25 | [2026-09-11](output/hacker_news_summary_2026-09-11.md) |
| 26 | [2026-09-12](output/hacker_news_summary_2026-09-12.md) |
| 27 | [2026-09-03](output/hacker_news_summary_2026-09-03.md) |
| 28 | [2026-09-02](output/hacker_news_summary_2026-09-02.md) |
| 29 | [2026-09-04](output/hacker_news_summary_2026-09-04.md) |
| 30 | [2026-09-05](output/hacker_news_summary_2026-09-05.md) |
| 31 | [2026-09-01](output/hacker_news_summary_2026-09-01.md) |
| 32 | [2026-09-07](output/hacker_news_summary_2026-09-07.md) |
| 33 | [2026-09-06](output/hacker_news_summary_2026-09-06.md) |
| 34 | [2026-08-25](output/hacker_news_summary_2026-08-25.md) |
| 35 | [2026-08-31](output/hacker_news_summary_2026-08-31.md) |
| 36 | [2026-08-28](output/hacker_news_summary_2026-08-28.md) |
| 37 | [2026-08-23](output/hacker_news_summary_2026-08-23.md) |
| 38 | [2026-08-29](output/hacker_news_summary_2026-08-29.md) |
| 39 | [2026-08-24](output/hacker_news_summary_2026-08-24.md) |
| 40 | [2026-08-30](output/hacker_news_summary_2026-08-30.md) |
| 41 | [2026-08-26](output/hacker_news_summary_2026-08-26.md) |
| 42 | [2026-08-22](output/hacker_news_summary_2026-08-22.md) |
| 43 | [2026-08-19](output/hacker_news_summary_2026-08-19.md) |
| 44 | [2026-08-20](output/hacker_news_summary_2026-08-20.md) |
| 45 | [2026-08-16](output/hacker_news_summary_2026-08-16.md) |
| 46 | [2026-08-17](output/hacker_news_summary_2026-08-17.md) |
| 47 | [2026-08-18](output/hacker_news_summary_2026-08-18.md) |
| 48 | [2026-08-15](output/hacker_news_summary_2026-08-15.md) |
| 49 | [2026-08-21](output/hacker_news_summary_2026-08-21.md) |
| 50 | [2026-08-12](output/hacker_news_summary_2026-08-12.md) |
| 51 | [2026-08-11](output/hacker_news_summary_2026-08-11.md) |
| 52 | [2026-08-14](output/hacker_news_summary_2026-08-14.md) |
| 53 | [2026-08-10](output/hacker_news_summary_2026-08-10.md) |
| 54 | [2026-08-09](output/hacker_news_summary_2026-08-09.md) |
| 55 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 56 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 57 | [2026-08-13](output/hacker_news_summary_2026-08-13.md) |
| 58 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 59 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 60 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 61 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 62 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 63 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 64 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 65 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 66 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 67 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 68 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 69 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 70 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 71 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 72 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 73 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 74 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 75 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 76 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 77 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 78 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 79 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 80 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 81 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 82 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 83 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 84 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 85 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 86 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 87 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 88 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 89 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 90 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 91 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 92 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 93 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 94 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 95 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 96 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 97 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 98 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 99 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 100 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 101 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 102 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 103 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 104 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 105 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 106 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 107 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 108 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 109 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 110 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 111 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 112 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 113 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 114 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 115 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 116 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 117 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 118 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 119 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 120 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 121 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 122 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 123 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 124 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 125 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 126 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 127 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 128 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 129 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 130 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 131 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 132 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 133 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 134 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 135 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 136 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 137 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 138 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 139 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 140 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 141 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 142 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 143 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 144 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 145 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 146 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 147 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 148 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 149 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 150 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 151 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 152 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 153 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 154 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 155 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 156 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 157 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 158 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 159 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 160 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 161 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 162 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 163 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 164 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 165 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 166 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 167 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 168 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 169 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 170 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 171 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 172 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 173 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 174 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 175 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 176 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 177 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 178 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 179 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 180 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 181 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 182 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 183 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 184 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 185 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 186 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 187 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 188 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 189 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 190 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 191 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 192 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 193 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 194 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 195 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 196 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 197 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 198 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 199 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 200 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 201 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 202 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 203 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 204 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 205 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 206 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 207 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 208 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 209 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 210 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 211 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 212 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 213 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 214 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 215 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 216 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 217 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 218 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 219 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 220 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 221 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 222 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 223 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 224 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 225 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 226 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 227 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 228 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 229 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 230 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 231 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 232 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 233 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 234 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 235 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 236 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 237 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 238 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 239 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 240 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 241 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 242 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 243 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 244 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 245 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 246 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 247 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 248 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 249 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 250 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 251 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 252 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 253 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 254 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 255 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 256 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 257 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 258 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 259 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 260 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 261 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 262 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 263 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 264 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 265 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 266 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 267 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 268 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 269 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 270 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 271 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 272 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 273 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 274 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 275 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 276 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 277 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 278 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 279 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 280 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 281 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 282 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 283 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 284 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 285 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 286 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 287 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 288 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 289 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 290 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 291 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 292 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 293 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 294 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 295 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 296 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 297 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 298 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 299 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 300 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 301 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 302 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 303 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 304 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 305 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 306 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 307 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 308 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 309 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 310 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 311 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 312 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 313 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 314 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 315 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 316 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 317 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 318 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 319 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 320 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 321 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 322 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 323 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 324 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 325 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 326 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 327 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 328 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
