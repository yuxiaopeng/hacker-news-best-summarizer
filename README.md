# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-08-17.md)

*最后自动更新时间: 2026-08-17 19:57:18*
## 1. Qwen 3.8 27B 很优秀，但它默认会想太多。

**原文标题**: Qwen 3.8 27B is excellent, but it defaults to overthinking things

**原文链接**: [https://simonwillison.net/2026/Aug/16/qwen-38-27b/](https://simonwillison.net/2026/Aug/16/qwen-38-27b/)

本文评测了阿里巴巴于2026年8月16日发布的Qwen 3.8 27B，这是一个采用Apache 2许可、拥有27B参数且具备视觉能力的LLM。作者赞扬了它的潜力，指出其适合在笔记本电脑上运行的尺寸以及令人印象深刻的自测基准。

一个关键发现是，该模型默认的“xhigh”推理级别导致它对任务“过度思考”，从而产生了极长的生成时间（例如，生成一个鹈鹕SVG需21分钟）和过于复杂的输出（例如，对于简单的“绘制一个圆形SVG”提示，却生成了一个动画圆形）。作者强烈建议最初使用“low”或“no reasoning”级别，尤其是在消费级硬件上，尽管推理对于构建编码工具等更复杂的任务可能是有益的。

尽管有此默认设置，Qwen 3.8 27B 仍展示了出色的能力：它能精确识别图像中的边界框，并有效驱动像Pi这样的编码代理，生成Python代码和脚本。

主要缺点是其速度，每秒仅返回15-30个token，与托管API模型相比感觉很慢。然而，多token预测（MTP）架构与`llama serve`结合使用时，可将推理性能显著提升约72%。

最终，作者对该模型能够在性能强大的笔记本电脑上的一个17GB文件中运行一个通用的、具备视觉能力的LLM，并具有强大的工具调用和代码生成能力感到惊叹。这一进展强调了强大的、开放权重的模型不再需要昂贵的数据中心硬件。

---

## 2. 克劳德: 系统提示

**原文标题**: Claude: System Prompts

**原文链接**: [https://platform.claude.com/docs/en/release-notes/system-prompts](https://platform.claude.com/docs/en/release-notes/system-prompts)

文章内容仅是“Loading”重复多次。因此，没有实质性信息可供总结。这段文字表明内容尚未加载或加载失败。

---

## 3. Anthropic's ‘watermark’ text adulteration in Claude is a perversion of writing

**原文标题**: Anthropic's ‘watermark’ text adulteration in Claude is a perversion of writing

**原文链接**: [https://daringfireball.net/2026/08/anthropics_watermark_text_adulteration_in_claude_is_a_perversion_of_writing](https://daringfireball.net/2026/08/anthropics_watermark_text_adulteration_in_claude_is_a_perversion_of_writing)

生成摘要时出错

---

## 4. GitHub.com 事件

**原文标题**: Incident with Github.com

**原文链接**: [https://www.githubstatus.com/incidents/zkxwbgr0cnmx](https://www.githubstatus.com/incidents/zkxwbgr0cnmx)

2023年12月6日，GitHub经历了一次严重的服务中断，影响了包括Actions、Packages、Pages、Codespaces以及API请求在内的多项服务。此次事件始于协调世界时（UTC）13:50，起因是一次旨在提高系统韧性的内部网络更新。这次更新意外地引发了网络分区事件，隔离了GitHub基础设施的关键部分，导致多种产品性能下降并出现错误。

工程师将网络问题确定为根本原因，并启动了对问题更改的回滚。网络于协调世界时14:48完全恢复，GitHub的大多数服务在协调世界时15:35开始恢复。然而，遗留问题，特别是GitHub Actions和webhook交付方面的问题，持续了一段时间，需要进一步修复。

该事件于协调世界时17:34宣布解决，但GitHub继续监控系统以确保完全稳定。该公司承诺进行彻底的内部审查，以防止再次发生，并改进其变更管理和网络架构。

---

## 5. 火狐浏览器 iOS 版现已内置原生广告拦截器

**原文标题**: Firefox for iOS now has a native adblocker

**原文链接**: [https://support.mozilla.org/en-US/kb/block-ads-firefox-ios](https://support.mozilla.org/en-US/kb/block-ads-firefox-ios)

所提供的内容，尽管其标题为“iOS 版 Firefox 现已内置广告拦截器”，但它并非一篇详细介绍此新功能的文章。相反，它是一条错误消息，表明某个网站组件未能加载。该消息将此故障归因于各种潜在问题，包括 JavaScript 被禁用、网络问题、浏览器设置，或者，值得注意的是，一个正在运行的广告拦截器。它指示用户启用 JavaScript、验证其连接、禁用广告拦截器，或者使用其他浏览器来解决问题。这种讽刺意味值得注意，因为一条建议禁用广告拦截器的错误消息，竟然出现在一个宣布新的内置广告拦截器的标题语境中。

---

## 6. A third world engineer responds to “RISC-V: They should have known better”

**原文标题**: A third world engineer responds to “RISC-V: They should have known better”

**原文链接**: [https://rvembedded.com/blog_post/12/](https://rvembedded.com/blog_post/12/)

生成摘要时出错

---

## 7. 据报道，Stripe 将以逾70亿美元收购 OpenRouter。

**原文标题**: Stripe will reportedly acquire OpenRouter for $7B+

**原文链接**: [https://techcrunch.com/2026/08/16/stripe-will-reportedly-acquire-ai-gateway-startup-openrouter-for-7b/](https://techcrunch.com/2026/08/16/stripe-will-reportedly-acquire-ai-gateway-startup-openrouter-for-7b/)

据彭博社2026年8月16日发布的一份报告，Stripe据称将以逾70亿美元的价格收购AI网关初创公司OpenRouter。此消息此前已在《华尔街日报》的报道中有所提及，当时指出收购谈判正在进行中。

OpenRouter专注于为客户提供单一访问点，使其能够根据特定需求和预算选择并利用各种AI模型，有效避免了供应商锁定。首席执行官亚历克斯·阿塔拉此前曾将该公司比作“AI界的Stripe”，因为它在简化不同系统访问方面发挥着作用。这家初创公司拥有800万全球用户，并提供对400多种模型的访问。

五月，OpenRouter完成了1.13亿美元的B轮融资，公司估值达到13亿美元，投资者包括红杉资本、安德森·霍洛维茨基金、门罗风投以及Alphabet旗下的CapitalG。Stripe的一位发言人拒绝就收购传闻发表评论。

---

## 8. 超强厄尔尼诺持续增强，冬季来临前最新预测已创历史新高

**原文标题**: Super El Niño Keeps Growing as New Forecasts Reach Record Territory Ahead Winter

**原文链接**: [https://www.severe-weather.eu/long-range-2/super-el-nino-growth-accelerating-to-record-strength-fall-winter-2026-2027-forecast-impact-united-states-canada-europe-fa/](https://www.severe-weather.eu/long-range-2/super-el-nino-growth-accelerating-to-record-strength-fall-winter-2026-2027-forecast-impact-united-states-canada-europe-fa/)

2026/2027年，一场“超级厄尔尼诺”事件正在热带太平洋迅速增强，新数据和预测表明，其强度将达到破纪录水平。这种加速增长得益于赤道太平洋前所未有的西风异常以及强大的次表层开尔文波，后者不断输送暖水。该事件已超越2015-2016年超级厄尔尼诺的速度和强度，预计将在11-12月达到峰值，主要ENSO区域的异常可能超过+3°C，标志着这是一次历史性事件。

这次超级厄尔尼诺事件正在深刻重塑全球大气环流，形成一个“大气驻波”。证据包括2026年6-7月创纪录高的多变量ENSO指数（MEI），证实了强大的海洋与大气耦合。环流变化加剧了急流，形成了更深的太平洋低压槽和更强的加拿大高压脊。

因此，2026年秋季的预报已经显示出通常与厄尔尼诺冬季相关的模式：加拿大上空出现高压异常，北太平洋出现低压区，以及一条活跃的风暴路径横穿美国南部进入大西洋。这意味着美国北部和加拿大气温将更温和，而美国中南部和东部由于风暴活动增加，气温将正常。随着冬季临近，持续的西风预计将进一步增强超级厄尔尼诺事件。

---

## 9. 科研论文使用“肾失望”而非“肾衰竭”

**原文标题**: Research papers using "kidney disappointment" instead of "kidney failure"

**原文链接**: [https://scholar.google.com/scholar?q=%22kidney+disappointment%22](https://scholar.google.com/scholar?q=%22kidney+disappointment%22)

无法访问文章链接。

在尝试访问提供的 Google Scholar 网址 (https://scholar.google.com/scholar?q=%22kidney+disappointment%22) 以查找使用短语“kidney disappointment”的研究论文时，搜索结果显示“未找到任何结果”。

这表明“kidney disappointment”在学术或医学文献中，无论是作为“kidney failure”（肾衰竭）的替代词，还是在 Google Scholar 收录的学术出版物中的任何其他语境下，都不是一个公认或使用的术语。目前没有研究论文或文章使用这个特定短语。

---

## 10. A Preview of DuckDB v2.0

**原文标题**: A Preview of DuckDB v2.0

**原文链接**: [https://duckdb.org/2026/08/17/duckdb-20-highlights](https://duckdb.org/2026/08/17/duckdb-20-highlights)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-08-17](output/hacker_news_summary_2026-08-17.md) |
| 2 | [2026-08-09](output/hacker_news_summary_2026-08-09.md) |
| 3 | [2026-08-10](output/hacker_news_summary_2026-08-10.md) |
| 4 | [2026-08-15](output/hacker_news_summary_2026-08-15.md) |
| 5 | [2026-08-11](output/hacker_news_summary_2026-08-11.md) |
| 6 | [2026-08-12](output/hacker_news_summary_2026-08-12.md) |
| 7 | [2026-08-13](output/hacker_news_summary_2026-08-13.md) |
| 8 | [2026-08-14](output/hacker_news_summary_2026-08-14.md) |
| 9 | [2026-08-16](output/hacker_news_summary_2026-08-16.md) |
| 10 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 11 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 12 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 13 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 14 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 15 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 16 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 17 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 18 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 19 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 20 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 21 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 22 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 23 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 24 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 25 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 26 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 27 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 28 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 29 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 30 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 31 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 32 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 33 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 34 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 35 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 36 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 37 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 38 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 39 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 40 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 41 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 42 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 43 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 44 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 45 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 46 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 47 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 48 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 49 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 50 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 51 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 52 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 53 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 54 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 55 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 56 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 57 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 58 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 59 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 60 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 61 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 62 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 63 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 64 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 65 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 66 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 67 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 68 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 69 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 70 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 71 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 72 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 73 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 74 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 75 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 76 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 77 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 78 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 79 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 80 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 81 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 82 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 83 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 84 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 85 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 86 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 87 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 88 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 89 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 90 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 91 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 92 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 93 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 94 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 95 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 96 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 97 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 98 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 99 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 100 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 101 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 102 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 103 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 104 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 105 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 106 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 107 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 108 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 109 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 110 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 111 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 112 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 113 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 114 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 115 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 116 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 117 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 118 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 119 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 120 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 121 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 122 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 123 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 124 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 125 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 126 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 127 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 128 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 129 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 130 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 131 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 132 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 133 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 134 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 135 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 136 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 137 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 138 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 139 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 140 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 141 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 142 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 143 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 144 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 145 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 146 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 147 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 148 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 149 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 150 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 151 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 152 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 153 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 154 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 155 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 156 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 157 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 158 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 159 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 160 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 161 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 162 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 163 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 164 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 165 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 166 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 167 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 168 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 169 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 170 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 171 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 172 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 173 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 174 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 175 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 176 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 177 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 178 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 179 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 180 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 181 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 182 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 183 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 184 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 185 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 186 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 187 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 188 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 189 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 190 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 191 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 192 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 193 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 194 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 195 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 196 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 197 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 198 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 199 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 200 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 201 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 202 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 203 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 204 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 205 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 206 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 207 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 208 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 209 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 210 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 211 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 212 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 213 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 214 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 215 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 216 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 217 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 218 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 219 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 220 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 221 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 222 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 223 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 224 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 225 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 226 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 227 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 228 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 229 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 230 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 231 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 232 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 233 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 234 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 235 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 236 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 237 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 238 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 239 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 240 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 241 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 242 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 243 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 244 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 245 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 246 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 247 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 248 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 249 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 250 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 251 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 252 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 253 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 254 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 255 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 256 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 257 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 258 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 259 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 260 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 261 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 262 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 263 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 264 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 265 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 266 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 267 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 268 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 269 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 270 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 271 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 272 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 273 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 274 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 275 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 276 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 277 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 278 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 279 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 280 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 281 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 282 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
