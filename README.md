# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-04-23.md)

*最后自动更新时间: 2026-04-23 20:33:44*
## 1. 阿尔伯塔初创企业半价销售无科技拖拉机

**原文标题**: Alberta startup sells no-tech tractors for half price

**原文链接**: [https://wheelfront.com/this-alberta-startup-sells-no-tech-tractors-for-half-price/](https://wheelfront.com/this-alberta-startup-sells-no-tech-tractors-for-half-price/)

这篇文章来自《汽车新闻》，重点报道了一家总部位于阿尔伯塔省的初创公司，该公司向农业市场推出了一款独特的产品：“无科技”拖拉机。这些车辆的核心卖点是其显著更低的成本，定价仅为传统或技术先进型号的一半。该公司的策略似乎侧重于通过有意省略复杂技术，为农民提供一种更简单、更经济实惠的替代方案。

---

## 2. Windows 9x Linux 子系统

**原文标题**: Windows 9x Subsystem for Linux

**原文链接**: [https://social.hails.org/@hailey/116446826733136456](https://social.hails.org/@hailey/116446826733136456)

The provided text briefly introduces the concept of a "Windows 9x Subsystem for Linux." Quoting Hailey from hails.org, the snippet indicates that this subsystem would allow users to "run a..." (the sentence is truncated). Due to the brevity and incomplete nature of the provided content, further details regarding the exact functionality or purpose of this proposed subsystem are not available.

---

## 3. Qwen3.6-27B：27B稠密模型中的旗舰级编程能力

**原文标题**: Qwen3.6-27B: Flagship-Level Coding in a 27B Dense Model

**原文链接**: [https://qwen.ai/blog?id=qwen3.6-27b](https://qwen.ai/blog?id=qwen3.6-27b)

本文介绍了Qwen3.6-27B，一个旨在提供旗舰级编码能力的新模型。其主要亮点在于它能够在270亿参数的密集模型架构中实现如此高的性能。标题表明Qwen3.6-27B旨在成为编码领域的顶级竞争者，证明了即使是这种规模和类型的模型也能获得具有竞争力的高质量性能。

（注：所提供的内容极其简短，仅包含“Qwen”一词。因此，本摘要主要根据文章标题推导得出。）

---

## 4. 我正在构建云

**原文标题**: I am building a cloud

**原文链接**: [https://crawshaw.io/blog/building-a-cloud](https://crawshaw.io/blog/building-a-cloud)

David Crawshaw，某成功初创公司的联合创始人，正基于个人热情以及对当前云计算现状的深刻不满，推出exe.dev。尽管他喜欢各种平台上的计算机，但他发现当今的云产品根本上是“错误”且具有限制性的。

克劳肖指出了几个核心问题：
1.  **虚拟机抽象：** 当前的虚拟机与CPU/内存资源低效绑定，迫使用户采取复杂的变通方案或专有PaaS系统，从而限制了功能。
2.  **磁盘性能：** 远程块设备是为慢速硬盘设计的，在现代SSD上引入了严重的10倍性能损失。高IOPS价格过高，并且通常比本地硬件更慢。
3.  **网络成本：** 云端出口流量费用过高，使得每月不花费数百万美元的用户难以负担项目开销。
4.  **API与Kubernetes：** 云API令人痛苦。Kubernetes尽管初衷良好，但无法解决这些根深蒂固的架构缺陷；它只不过是“给猪涂口红”。

AI代理和大型语言模型的出现，使得解决这些问题变得迫在眉睫。代理将指数级地增加软件创建量，要求更高效、更经济、更易于管理的计算资源，而这正是当前云抽象无法提供的。

Exe.dev的解决方案通过允许用户配置裸机CPU和内存来运行他们想要的虚拟机，从而解决了这些问题。它提供带有异步复制的本地NVMe磁盘，包括内置的TLS和认证代理，提供全球区域，并利用任播网络实现低延迟访问。克劳肖旨在构建一个他真正想使用的云，并希望也能为其他人提供卓越的体验。

---

## 5. 我们发现了一个能关联你所有Tor私密身份的稳定的Firefox标识符。

**原文标题**: We found a stable Firefox identifier linking all your private Tor identities

**原文链接**: [https://fingerprint.com/blog/firefox-tor-indexeddb-privacy-vulnerability/](https://fingerprint.com/blog/firefox-tor-indexeddb-privacy-vulnerability/)

在所有基于Firefox的浏览器中，包括Firefox隐私浏览模式和Tor浏览器，都发现了一个重大的隐私漏洞。这个缺陷允许网站为正在运行的浏览器进程生成一个唯一、确定性且稳定的标识符，从而关联用户在不同来源的活动，甚至能绕过Tor浏览器“新身份”等隐私功能。

该漏洞存在于`indexedDB.databases()` API中。它没有以中立或规范的顺序返回数据库名称，而是暴露了基于浏览器内部哈希表结构的顺序。这种内部排序在浏览器进程的整个生命周期中充当一个稳定的标识符，仅在Firefox完全重启时才会重置。它还在所有来源之间共享，这意味着任何网站都可以观察到相同的标识符。

这种稳定性导致了两个主要的隐私泄露：
1.  **跨源追踪**：不相关的网站可以观察到相同的标识符，从而无需cookie或其他共享存储就能关联用户在不同域上的活动。
2.  **破坏隔离**：在Firefox隐私浏览中，即使在所有隐私窗口关闭后，该标识符仍然存在。在Tor浏览器中，它破坏了旨在提供完全隔离的“新身份”功能，允许网站关联本应相互独立的会话。

该标识符具有高熵，使其对于指纹识别非常有效。Mozilla已负责任地解决了这个问题，并在Firefox 150和ESR 140.10.0中发布了修复程序。该解决方案涉及对`indexedDB.databases()`返回的结果进行规范化（例如，排序），以消除泄露的内部排序，从而消除指纹识别信号。这一发现强调了微妙的内部实现细节如何能演变为关键的隐私漏洞。

---

## 6. SpaceX 称已达成协议，将以 600 亿美元收购 Cursor

**原文标题**: SpaceX says it has agreement to acquire Cursor for $60B

**原文链接**: [https://twitter.com/spacex/status/2046713419978453374](https://twitter.com/spacex/status/2046713419978453374)

文章标题“SpaceX 称已同意以 600 亿美元收购 Cursor”宣布了一项重大的商业进展。然而，所提供的内容并未包含任何有关此次收购的信息。

相反，文章的整个正文是来自 x.com（前身为 Twitter）的一条技术错误消息。它告知读者，他们的浏览器中禁用了 JavaScript，从而阻止了内容的显示，并建议他们启用 JavaScript 或切换到受支持的浏览器。该消息附带了标准的网站元素，例如指向帮助中心、服务条款、隐私政策、Cookie 政策、版本说明、广告信息等的链接，以及“© 2026 X Corp.”的版权声明。因此，尽管标题暗示了一项重大收购，文章正文并未提供任何有关此事件的详细信息以供总结。

---

## 7. 苹果修复了警方曾用于从iPhone中提取已删除聊天记录的漏洞。

**原文标题**: Apple fixes bug that cops used to extract deleted chat messages from iPhones

**原文链接**: [https://techcrunch.com/2026/04/22/apple-fixes-bug-that-cops-used-to-extract-deleted-chat-messages-from-iphones/](https://techcrunch.com/2026/04/22/apple-fixes-bug-that-cops-used-to-extract-deleted-chat-messages-from-iphones/)

Apple 已为 iPhone 和 iPad 发布了软件更新，修复了一个允许执法部门提取已删除或自动消失的聊天消息的漏洞。该漏洞源于通知显示的消息内容在设备上被缓存长达一个月，即使原始消息已从 Signal 等应用中删除。

这个问题最初由 404 Media 曝光，报道称 FBI 曾利用法医工具利用此漏洞从 iPhone 中恢复已删除的 Signal 消息。此后，Signal 总裁 Meredith Whittaker 公开呼吁苹果修复该问题，强调已删除消息的通知不应保留在任何操作系统数据库中。

隐私活动家对此表示担忧，指出该漏洞规避了一项关键的安全功能——定时消息删除——而这一功能是高风险用户用来保护敏感对话的。苹果的安全通知证实，“标记为删除的通知可能会被意外保留”。该公司此后已将此修复程序移植到旧版 iOS 中，表明这种保留是一个无意的错误。

---

## 8. Claude Code to be removed from Anthropic's Pro plan?

**原文标题**: Claude Code to be removed from Anthropic's Pro plan?

**原文链接**: [https://bsky.app/profile/edzitron.com/post/3mjzxwfx3qs2a](https://bsky.app/profile/edzitron.com/post/3mjzxwfx3qs2a)

生成摘要时出错

---

## 9. GPT-5.5

**原文标题**: GPT-5.5

**原文链接**: [https://openai.com/index/introducing-gpt-5-5/](https://openai.com/index/introducing-gpt-5-5/)

生成摘要时出错

---

## 10. Bitwarden CLI compromised in ongoing Checkmarx supply chain campaign

**原文标题**: Bitwarden CLI compromised in ongoing Checkmarx supply chain campaign

**原文链接**: [https://socket.dev/blog/bitwarden-cli-compromised](https://socket.dev/blog/bitwarden-cli-compromised)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 2 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 3 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 4 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 5 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 6 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 7 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 8 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 9 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 10 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 11 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 12 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 13 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 14 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 15 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 16 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 17 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 18 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 19 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 20 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 21 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 22 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 23 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 24 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 25 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 26 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 27 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 28 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 29 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 30 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 31 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 32 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 33 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 34 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 35 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 36 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 37 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 38 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 39 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 40 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 41 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 42 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 43 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 44 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 45 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 46 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 47 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 48 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 49 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 50 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 51 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 52 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 53 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 54 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 55 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 56 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 57 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 58 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 59 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 60 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 61 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 62 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 63 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 64 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 65 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 66 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 67 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 68 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 69 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 70 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 71 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 72 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 73 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 74 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 75 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 76 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 77 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 78 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 79 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 80 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 81 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 82 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 83 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 84 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 85 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 86 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 87 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 88 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 89 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 90 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 91 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 92 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 93 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 94 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 95 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 96 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 97 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 98 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 99 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 100 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 101 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 102 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 103 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 104 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 105 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 106 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 107 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 108 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 109 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 110 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 111 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 112 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 113 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 114 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 115 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 116 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 117 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 118 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 119 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 120 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 121 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 122 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 123 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 124 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 125 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 126 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 127 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 128 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 129 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 130 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 131 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 132 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 133 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 134 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 135 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 136 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 137 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 138 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 139 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 140 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 141 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 142 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 143 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 144 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 145 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 146 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 147 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 148 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 149 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 150 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 151 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 152 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 153 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 154 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 155 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 156 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 157 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 158 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 159 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 160 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
| 161 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 162 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 163 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 164 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 165 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 166 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 167 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
