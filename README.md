# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2026-10-27.md)

*最后自动更新时间: 2026-10-27 23:14:32*
## 1. 法罗 14

**原文标题**: Pharo 14

**原文链接**: [https://pharo.org/news/2026-10-26-Pharo14Release.html](https://pharo.org/news/2026-10-26-Pharo14Release.html)

Pharo 14 已发布，这是对纯面向对象编程语言及其强大的实时环境的一次更新，该语言以其简洁性、即时反馈和卓越的调试器而闻名。Pharo 在 MIT 许可证下完全开源，由社区驱动。

Pharo 14 的主要工作集中在三个主要领域：
1.  **现代化开发工具：** 引入 Mission Control 和 Pulse（取代 Spotter），重构方法浏览器，重写设置浏览器，并将 Epicea 和 ProfStef 整合到 NewTools 中，推进基于 Spec 的工具开发。
2.  **重建重构和命令基础设施：** 将重构命令迁移到基于驱动程序的架构，并扩展用于测试、调试和脚本编写的命令行功能。
3.  **现代化虚拟机：** 统一帧和堆栈管理，添加 RISC-V JIT 支持，扩展内存管理（直接旧空间分配，GC 改进），推进 Slang/C 编译，并现代化构建基础设施。

Pharo 也将其发布时间表从春季调整到秋季，Pharo 14 是此新时间表下的首次发布。此版本是 978 个拉取请求和 616 个已关闭问题的成果，突显了其全球社区的重大贡献。发布日期是 2026 年 10 月 26 日。

---

## 2. 服务器协议类型

**原文标题**: Type Server Protocol

**原文链接**: [https://github.com/microsoft/pylance-release/blob/main/docs/tsp/type-server-protocol.md](https://github.com/microsoft/pylance-release/blob/main/docs/tsp/type-server-protocol.md)

类型服务器协议（TSP）是一种JSON-RPC协议，旨在供客户端查询Python类型服务器以获取分析数据。它采用语言服务器协议（LSP）的数据结构，例如Position和Range，将URI表示为字符串，并为其方法使用`typeServer/`前缀。该协议的权威定义可在TypeScript接口和JSON schema文件中找到。

TSP采用语义版本控制，其中0.x次版本可能会引入破坏性更改。通信通过主JSON-RPC连接进行，通常使用LSP进行初始工作区和文档同步。客户端-服务器启动序列包括初始化、验证协议兼容性（`typeServer/getSupportedProtocolVersion`）、获取快照标识符（`typeServer/getSnapshot`），然后发送类型查询、导入解析或搜索路径请求，所有这些都与当前快照相关联。当分析结果失效时，服务器通过`typeServer/snapshotChanged`通知客户端。

可选的多连接模式允许客户端向同一类型服务器打开额外的只读通道，以获得性能优势，例如并发查询。该模式通过LSP初始化期间的`capabilities.experimental.typeServerMultiConnection`进行协商。额外的连接通过主通道上的`typeServer/connection`请求打开/关闭，并且只处理只读的TSP消息，而主连接则保留所有状态更改操作和LSP生命周期消息的所有权。

快照是非负整数，用于标识服务器分析状态的时间点视图；类型结果仅对其返回时所关联的快照有效。使用过期快照的请求应以LSP `ServerCancelled`错误失败。类型结果是可JSON序列化的带标签对象，具有一个`kind`鉴别器（例如BuiltIn、Function、Class）、`id`和标志。TSP定义了三种类型查询请求：`getComputedType`（推断类型）、`getDeclaredType`（显式声明类型）和`getExpectedType`（上下文预期类型）。错误处理遵循标准的JSON-RPC约定。

---

## 3. 新 iPad mini

**原文标题**: New iPad mini

**原文链接**: [https://www.apple.com/newsroom/2026/10/apple-gives-ipad-mini-its-biggest-update-ever/](https://www.apple.com/newsroom/2026/10/apple-gives-ipad-mini-its-biggest-update-ever/)

苹果公司发布了新款iPad mini，号称是迄今为止最大的一次更新，将于10月28日开始预购，11月6日发货。这款重新设计的iPad mini配备了一块惊艳的8.5英寸OLED超视网膜XDR显示屏，峰值亮度高达1200尼特，可选纳米纹理饰面，所有这些都融入更薄（5.4毫米）、更轻的设计中，并提供全新的午夜色和星光色选项。

性能上的显著飞跃源于全新的A20 Pro芯片，其AI性能提升高达4.5倍，图形处理速度提升2.7倍。该设备还具备IP67级别的抗水防尘功能，并包含创新的声学显示屏以改善音频效果，同时配备了增强型摄像头：一个位于横向边缘的1200万像素人物居中前置摄像头，以及一个带有自适应原彩闪光灯的1200万像素广角后置摄像头。

连接性方面，通过苹果的N1芯片（Wi-Fi 7，蓝牙6）和C2蜂窝调制解调器得到提升，蜂窝网络速度提升50%。搭载iPadOS 27系统，它集成了下一代Apple Intelligence和Siri AI，提供个性化的情境感知辅助、屏幕感知功能以及图像游乐场等全新创意工具。

新款iPad mini起售价为699美元（Wi-Fi版），支持TechWoven智能双面夹、Apple Pencil (USB-C) 和Apple Pencil Pro。它还包含35%的回收材料，符合苹果2030年碳中和目标。

---

## 4. NeXT电脑办公室幕后

**原文标题**: Behind the scenes at the NeXT Computer office

**原文链接**: [https://exhibits.stanford.edu/menuez/browse/next-computer-inc?per_page=96&sort=pub_year_isi+asc%2C+title_sort+asc&view=masonry](https://exhibits.stanford.edu/menuez/browse/next-computer-inc?per_page=96&sort=pub_year_isi+asc%2C+title_sort+asc&view=masonry)

我很抱歉，我无法为您总结文章“NeXT电脑办公室的幕后故事”，因为提供的内容显示：“请启用JavaScript以查看页面内容。”

这意味着我无法获取实际的文章内容。如果您能提供内容，我将很乐意为您总结。

---

## 5. ChatGPT Keeps Telling People 404 Media Can Solve Their Tech Support Problems

**原文标题**: ChatGPT Keeps Telling People 404 Media Can Solve Their Tech Support Problems

**原文链接**: [https://www.404media.co/chatgpt-keeps-telling-people-404-media-can-solve-their-tech-support-problems/](https://www.404media.co/chatgpt-keeps-telling-people-404-media-can-solve-their-tech-support-problems/)

生成摘要时出错

---

## 6. 新 14 英寸 MacBook Pro 搭载 M6

**原文标题**: New 14‑inch MacBook Pro with M6

**原文链接**: [https://www.apple.com/in/newsroom/2026/10/apple-introduces-the-new-14-inch-macbook-pro-with-m6/](https://www.apple.com/in/newsroom/2026/10/apple-introduces-the-new-14-inch-macbook-pro-with-m6/)

生成摘要时出错

---

## 7. PaperPilot – 无云纯Rust PDF引擎，支持WASM和MCP

**原文标题**: PaperPilot – Zero-Cloud, Pure-Rust PDF Engine with WASM and MCP

**原文链接**: [https://github.com/KrushnaVardhanReddy/PaperPilot](https://github.com/KrushnaVardhanReddy/PaperPilot)

PaperPilot 是一个纯 Rust 实现的、零云端的 PDF 引擎，专为 AI 代理和人类用户设计，确保所有文件处理都在本地进行，以实现最大程度的隐私保护。它提供了一个全面的工具包，不依赖于 Chromium、C++ 运行时或外部云服务。

同一个核心引擎可以通过多种“界面”进行访问：一个用于 AI 代理（Codex、Claude、Kimi）的 MCP（消息控制协议）服务器，一个用于批处理工作流的命令行界面（CLI），一个用于零安装使用的基于浏览器的 WASM 版本，一个桌面应用程序（Tauri + Svelte），以及一个本地 REST API（也可用作兼容 Open-WebUI/Tika 的提取服务器）。

v0.6 版本的关键功能包括组织（合并、拆分、旋转、重新排序）、优化（有损压缩、去重）、提取（结构化文本、Markdown 表格、通过 PaddleOCR 实现的纯 Rust OCR）、安全（水印、签名验证、PII 扫描）以及 Office 数据转换（Excel 到 JSON/CSV）。

PaperPilot 的独特之处在于其默认隐私的本地操作、一流的代理就绪性、由于其单一的 Rust 核心而在所有接口上表现出一致的行为，以及其小巧、依赖性轻量级的架构。社区版采用 Apache 2.0 许可证。

---

## 8. I will no longer upload to NEW

**原文标题**: I will no longer upload to NEW

**原文链接**: [https://lists.debian.org/debian-devel/2026/10/msg00263.html](https://lists.debian.org/debian-devel/2026/10/msg00263.html)

Unable to access the article link.

---

## 9. US designates helium as a critical material

**原文标题**: US designates helium as a critical material

**原文链接**: [https://apnews.com/article/energy-critical-materials-minerals-helium-43da160adc1bad389fba0b9ffbd14c3c](https://apnews.com/article/energy-critical-materials-minerals-helium-43da160adc1bad389fba0b9ffbd14c3c)

The United States has officially designated helium as a critical material, a move aimed at ensuring a stable domestic supply for various essential industries. The designation, announced by the U.S. Geological Survey (USGS) and the Department of Energy (DOE), highlights helium's indispensable role in a wide array of high-tech and medical applications.

Helium is crucial for MRI machines, semiconductor manufacturing, fiber optics, rocketry, deep-sea diving, and scientific research due to its unique properties as an inert gas with the lowest boiling point. While not scarce on Earth, it is a non-renewable resource that escapes into space if not captured, making its management and recycling vital.

The designation allows federal agencies to streamline permitting for helium projects, prioritize research and development, and encourage domestic production and recycling efforts. It also enables access to federal funding and programs designed to strengthen critical supply chains. The U.S. has historically been a major producer, but global supply has faced volatility, prompting concerns about future availability and price stability. The move aims to mitigate these risks and secure a reliable supply for national security and economic interests.

---

## 10. 2美元微控制器上的SIMD加速计算机视觉

**原文标题**: SIMD-accelerated computer vision on a $2 microcontroller

**原文链接**: [https://shraiwi.com/blog/simd-fast-esp32s3/](https://shraiwi.com/blog/simd-fast-esp32s3/)

The author developed a SIMD-accelerated FAST feature detector for the $2 ESP32-S3 microcontroller, leveraging its 128-bit SIMD instructions. This implementation roughly doubled the performance of the reference, processing a QVGA (320x240) frame in approximately 6ms. The throughput increased by 220%, from 5.1MP/s to 11.2MP/s, making real-time computer vision, including 30fps VGA stream processing, feasible.

The project required navigating specific hardware limitations of the ESP32-S3's instruction set. Challenges included the absence of direct misaligned reads for SIMD operations, which was overcome by extracting pixel data slices from concatenated registers. A more significant hurdle was the SIMD's exclusive support for signed 8-bit comparisons and its saturating arithmetic. Since pixel data is unsigned 8-bit, a direct reinterpretation or subtraction of 128 would lead to incorrect results due to non-linear mapping or value clamping. The author devised an elegant solution: converting unsigned pixel values to a linearly mapped signed range by XORing them with 0x80 (flipping the most significant bit). This effectively shifts the [0, 255] range to [-128, 127] without using saturating subtraction, enabling accurate comparisons and arithmetic. This resourceful approach demonstrates powerful low-level optimization for embedded systems.

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2026-10-27](output/hacker_news_summary_2026-10-27.md) |
| 2 | [2026-10-23](output/hacker_news_summary_2026-10-23.md) |
| 3 | [2026-10-26](output/hacker_news_summary_2026-10-26.md) |
| 4 | [2026-10-22](output/hacker_news_summary_2026-10-22.md) |
| 5 | [2026-10-24](output/hacker_news_summary_2026-10-24.md) |
| 6 | [2026-10-25](output/hacker_news_summary_2026-10-25.md) |
| 7 | [2026-10-17](output/hacker_news_summary_2026-10-17.md) |
| 8 | [2026-10-18](output/hacker_news_summary_2026-10-18.md) |
| 9 | [2026-10-21](output/hacker_news_summary_2026-10-21.md) |
| 10 | [2026-10-20](output/hacker_news_summary_2026-10-20.md) |
| 11 | [2026-10-19](output/hacker_news_summary_2026-10-19.md) |
| 12 | [2026-10-13](output/hacker_news_summary_2026-10-13.md) |
| 13 | [2026-10-15](output/hacker_news_summary_2026-10-15.md) |
| 14 | [2026-10-14](output/hacker_news_summary_2026-10-14.md) |
| 15 | [2026-10-16](output/hacker_news_summary_2026-10-16.md) |
| 16 | [2026-10-10](output/hacker_news_summary_2026-10-10.md) |
| 17 | [2026-10-11](output/hacker_news_summary_2026-10-11.md) |
| 18 | [2026-10-07](output/hacker_news_summary_2026-10-07.md) |
| 19 | [2026-10-06](output/hacker_news_summary_2026-10-06.md) |
| 20 | [2026-10-04](output/hacker_news_summary_2026-10-04.md) |
| 21 | [2026-10-02](output/hacker_news_summary_2026-10-02.md) |
| 22 | [2026-10-03](output/hacker_news_summary_2026-10-03.md) |
| 23 | [2026-10-09](output/hacker_news_summary_2026-10-09.md) |
| 24 | [2026-09-24](output/hacker_news_summary_2026-09-24.md) |
| 25 | [2026-10-01](output/hacker_news_summary_2026-10-01.md) |
| 26 | [2026-09-29](output/hacker_news_summary_2026-09-29.md) |
| 27 | [2026-09-30](output/hacker_news_summary_2026-09-30.md) |
| 28 | [2026-09-27](output/hacker_news_summary_2026-09-27.md) |
| 29 | [2026-09-25](output/hacker_news_summary_2026-09-25.md) |
| 30 | [2026-09-21](output/hacker_news_summary_2026-09-21.md) |
| 31 | [2026-09-23](output/hacker_news_summary_2026-09-23.md) |
| 32 | [2026-09-20](output/hacker_news_summary_2026-09-20.md) |
| 33 | [2026-09-22](output/hacker_news_summary_2026-09-22.md) |
| 34 | [2026-09-19](output/hacker_news_summary_2026-09-19.md) |
| 35 | [2026-09-18](output/hacker_news_summary_2026-09-18.md) |
| 36 | [2026-09-13](output/hacker_news_summary_2026-09-13.md) |
| 37 | [2026-09-16](output/hacker_news_summary_2026-09-16.md) |
| 38 | [2026-09-14](output/hacker_news_summary_2026-09-14.md) |
| 39 | [2026-09-17](output/hacker_news_summary_2026-09-17.md) |
| 40 | [2026-09-15](output/hacker_news_summary_2026-09-15.md) |
| 41 | [2026-09-09](output/hacker_news_summary_2026-09-09.md) |
| 42 | [2026-09-10](output/hacker_news_summary_2026-09-10.md) |
| 43 | [2026-09-08](output/hacker_news_summary_2026-09-08.md) |
| 44 | [2026-09-07](output/hacker_news_summary_2026-09-07.md) |
| 45 | [2026-09-06](output/hacker_news_summary_2026-09-06.md) |
| 46 | [2026-09-11](output/hacker_news_summary_2026-09-11.md) |
| 47 | [2026-09-12](output/hacker_news_summary_2026-09-12.md) |
| 48 | [2026-09-03](output/hacker_news_summary_2026-09-03.md) |
| 49 | [2026-09-02](output/hacker_news_summary_2026-09-02.md) |
| 50 | [2026-08-31](output/hacker_news_summary_2026-08-31.md) |
| 51 | [2026-09-04](output/hacker_news_summary_2026-09-04.md) |
| 52 | [2026-09-05](output/hacker_news_summary_2026-09-05.md) |
| 53 | [2026-09-01](output/hacker_news_summary_2026-09-01.md) |
| 54 | [2026-08-29](output/hacker_news_summary_2026-08-29.md) |
| 55 | [2026-08-30](output/hacker_news_summary_2026-08-30.md) |
| 56 | [2026-08-22](output/hacker_news_summary_2026-08-22.md) |
| 57 | [2026-08-25](output/hacker_news_summary_2026-08-25.md) |
| 58 | [2026-08-28](output/hacker_news_summary_2026-08-28.md) |
| 59 | [2026-08-23](output/hacker_news_summary_2026-08-23.md) |
| 60 | [2026-08-21](output/hacker_news_summary_2026-08-21.md) |
| 61 | [2026-08-24](output/hacker_news_summary_2026-08-24.md) |
| 62 | [2026-08-26](output/hacker_news_summary_2026-08-26.md) |
| 63 | [2026-08-14](output/hacker_news_summary_2026-08-14.md) |
| 64 | [2026-08-19](output/hacker_news_summary_2026-08-19.md) |
| 65 | [2026-08-20](output/hacker_news_summary_2026-08-20.md) |
| 66 | [2026-08-16](output/hacker_news_summary_2026-08-16.md) |
| 67 | [2026-08-17](output/hacker_news_summary_2026-08-17.md) |
| 68 | [2026-08-18](output/hacker_news_summary_2026-08-18.md) |
| 69 | [2026-08-15](output/hacker_news_summary_2026-08-15.md) |
| 70 | [2026-08-13](output/hacker_news_summary_2026-08-13.md) |
| 71 | [2026-08-12](output/hacker_news_summary_2026-08-12.md) |
| 72 | [2026-08-11](output/hacker_news_summary_2026-08-11.md) |
| 73 | [2026-08-10](output/hacker_news_summary_2026-08-10.md) |
| 74 | [2026-08-09](output/hacker_news_summary_2026-08-09.md) |
| 75 | [2026-08-04](output/hacker_news_summary_2026-08-04.md) |
| 76 | [2026-08-07](output/hacker_news_summary_2026-08-07.md) |
| 77 | [2026-08-05](output/hacker_news_summary_2026-08-05.md) |
| 78 | [2026-08-08](output/hacker_news_summary_2026-08-08.md) |
| 79 | [2026-07-28](output/hacker_news_summary_2026-07-28.md) |
| 80 | [2026-08-01](output/hacker_news_summary_2026-08-01.md) |
| 81 | [2026-07-30](output/hacker_news_summary_2026-07-30.md) |
| 82 | [2026-07-29](output/hacker_news_summary_2026-07-29.md) |
| 83 | [2026-08-02](output/hacker_news_summary_2026-08-02.md) |
| 84 | [2026-07-31](output/hacker_news_summary_2026-07-31.md) |
| 85 | [2026-08-03](output/hacker_news_summary_2026-08-03.md) |
| 86 | [2026-07-20](output/hacker_news_summary_2026-07-20.md) |
| 87 | [2026-07-27](output/hacker_news_summary_2026-07-27.md) |
| 88 | [2026-07-26](output/hacker_news_summary_2026-07-26.md) |
| 89 | [2026-07-22](output/hacker_news_summary_2026-07-22.md) |
| 90 | [2026-07-25](output/hacker_news_summary_2026-07-25.md) |
| 91 | [2026-07-21](output/hacker_news_summary_2026-07-21.md) |
| 92 | [2026-07-19](output/hacker_news_summary_2026-07-19.md) |
| 93 | [2026-07-24](output/hacker_news_summary_2026-07-24.md) |
| 94 | [2026-07-23](output/hacker_news_summary_2026-07-23.md) |
| 95 | [2026-07-12](output/hacker_news_summary_2026-07-12.md) |
| 96 | [2026-07-16](output/hacker_news_summary_2026-07-16.md) |
| 97 | [2026-07-14](output/hacker_news_summary_2026-07-14.md) |
| 98 | [2026-07-18](output/hacker_news_summary_2026-07-18.md) |
| 99 | [2026-07-15](output/hacker_news_summary_2026-07-15.md) |
| 100 | [2026-07-17](output/hacker_news_summary_2026-07-17.md) |
| 101 | [2026-07-13](output/hacker_news_summary_2026-07-13.md) |
| 102 | [2026-07-11](output/hacker_news_summary_2026-07-11.md) |
| 103 | [2026-07-07](output/hacker_news_summary_2026-07-07.md) |
| 104 | [2026-07-05](output/hacker_news_summary_2026-07-05.md) |
| 105 | [2026-07-03](output/hacker_news_summary_2026-07-03.md) |
| 106 | [2026-07-06](output/hacker_news_summary_2026-07-06.md) |
| 107 | [2026-07-09](output/hacker_news_summary_2026-07-09.md) |
| 108 | [2026-07-08](output/hacker_news_summary_2026-07-08.md) |
| 109 | [2026-07-10](output/hacker_news_summary_2026-07-10.md) |
| 110 | [2026-07-04](output/hacker_news_summary_2026-07-04.md) |
| 111 | [2026-06-29](output/hacker_news_summary_2026-06-29.md) |
| 112 | [2026-07-02](output/hacker_news_summary_2026-07-02.md) |
| 113 | [2026-06-27](output/hacker_news_summary_2026-06-27.md) |
| 114 | [2026-06-30](output/hacker_news_summary_2026-06-30.md) |
| 115 | [2026-07-01](output/hacker_news_summary_2026-07-01.md) |
| 116 | [2026-06-28](output/hacker_news_summary_2026-06-28.md) |
| 117 | [2026-06-26](output/hacker_news_summary_2026-06-26.md) |
| 118 | [2026-06-18](output/hacker_news_summary_2026-06-18.md) |
| 119 | [2026-06-24](output/hacker_news_summary_2026-06-24.md) |
| 120 | [2026-06-23](output/hacker_news_summary_2026-06-23.md) |
| 121 | [2026-06-21](output/hacker_news_summary_2026-06-21.md) |
| 122 | [2026-06-19](output/hacker_news_summary_2026-06-19.md) |
| 123 | [2026-06-22](output/hacker_news_summary_2026-06-22.md) |
| 124 | [2026-06-25](output/hacker_news_summary_2026-06-25.md) |
| 125 | [2026-06-20](output/hacker_news_summary_2026-06-20.md) |
| 126 | [2026-06-13](output/hacker_news_summary_2026-06-13.md) |
| 127 | [2026-06-16](output/hacker_news_summary_2026-06-16.md) |
| 128 | [2026-06-12](output/hacker_news_summary_2026-06-12.md) |
| 129 | [2026-06-14](output/hacker_news_summary_2026-06-14.md) |
| 130 | [2026-06-17](output/hacker_news_summary_2026-06-17.md) |
| 131 | [2026-06-15](output/hacker_news_summary_2026-06-15.md) |
| 132 | [2026-06-10](output/hacker_news_summary_2026-06-10.md) |
| 133 | [2026-06-11](output/hacker_news_summary_2026-06-11.md) |
| 134 | [2026-06-06](output/hacker_news_summary_2026-06-06.md) |
| 135 | [2026-06-07](output/hacker_news_summary_2026-06-07.md) |
| 136 | [2026-06-05](output/hacker_news_summary_2026-06-05.md) |
| 137 | [2026-06-04](output/hacker_news_summary_2026-06-04.md) |
| 138 | [2026-06-03](output/hacker_news_summary_2026-06-03.md) |
| 139 | [2026-06-08](output/hacker_news_summary_2026-06-08.md) |
| 140 | [2026-06-09](output/hacker_news_summary_2026-06-09.md) |
| 141 | [2026-05-31](output/hacker_news_summary_2026-05-31.md) |
| 142 | [2026-05-30](output/hacker_news_summary_2026-05-30.md) |
| 143 | [2026-06-01](output/hacker_news_summary_2026-06-01.md) |
| 144 | [2026-05-28](output/hacker_news_summary_2026-05-28.md) |
| 145 | [2026-06-02](output/hacker_news_summary_2026-06-02.md) |
| 146 | [2026-05-29](output/hacker_news_summary_2026-05-29.md) |
| 147 | [2026-05-20](output/hacker_news_summary_2026-05-20.md) |
| 148 | [2026-05-24](output/hacker_news_summary_2026-05-24.md) |
| 149 | [2026-05-27](output/hacker_news_summary_2026-05-27.md) |
| 150 | [2026-05-23](output/hacker_news_summary_2026-05-23.md) |
| 151 | [2026-05-25](output/hacker_news_summary_2026-05-25.md) |
| 152 | [2026-05-26](output/hacker_news_summary_2026-05-26.md) |
| 153 | [2026-05-21](output/hacker_news_summary_2026-05-21.md) |
| 154 | [2026-05-22](output/hacker_news_summary_2026-05-22.md) |
| 155 | [2026-05-15](output/hacker_news_summary_2026-05-15.md) |
| 156 | [2026-05-17](output/hacker_news_summary_2026-05-17.md) |
| 157 | [2026-05-16](output/hacker_news_summary_2026-05-16.md) |
| 158 | [2026-05-18](output/hacker_news_summary_2026-05-18.md) |
| 159 | [2026-05-11](output/hacker_news_summary_2026-05-11.md) |
| 160 | [2026-05-19](output/hacker_news_summary_2026-05-19.md) |
| 161 | [2026-05-14](output/hacker_news_summary_2026-05-14.md) |
| 162 | [2026-05-12](output/hacker_news_summary_2026-05-12.md) |
| 163 | [2026-05-13](output/hacker_news_summary_2026-05-13.md) |
| 164 | [2026-05-05](output/hacker_news_summary_2026-05-05.md) |
| 165 | [2026-05-04](output/hacker_news_summary_2026-05-04.md) |
| 166 | [2026-05-08](output/hacker_news_summary_2026-05-08.md) |
| 167 | [2026-05-10](output/hacker_news_summary_2026-05-10.md) |
| 168 | [2026-05-06](output/hacker_news_summary_2026-05-06.md) |
| 169 | [2026-05-07](output/hacker_news_summary_2026-05-07.md) |
| 170 | [2026-05-09](output/hacker_news_summary_2026-05-09.md) |
| 171 | [2026-05-01](output/hacker_news_summary_2026-05-01.md) |
| 172 | [2026-05-03](output/hacker_news_summary_2026-05-03.md) |
| 173 | [2026-04-27](output/hacker_news_summary_2026-04-27.md) |
| 174 | [2026-04-28](output/hacker_news_summary_2026-04-28.md) |
| 175 | [2026-04-29](output/hacker_news_summary_2026-04-29.md) |
| 176 | [2026-04-26](output/hacker_news_summary_2026-04-26.md) |
| 177 | [2026-04-30](output/hacker_news_summary_2026-04-30.md) |
| 178 | [2026-05-02](output/hacker_news_summary_2026-05-02.md) |
| 179 | [2026-04-25](output/hacker_news_summary_2026-04-25.md) |
| 180 | [2026-04-21](output/hacker_news_summary_2026-04-21.md) |
| 181 | [2026-04-22](output/hacker_news_summary_2026-04-22.md) |
| 182 | [2026-04-24](output/hacker_news_summary_2026-04-24.md) |
| 183 | [2026-04-23](output/hacker_news_summary_2026-04-23.md) |
| 184 | [2026-04-20](output/hacker_news_summary_2026-04-20.md) |
| 185 | [2026-04-19](output/hacker_news_summary_2026-04-19.md) |
| 186 | [2026-04-14](output/hacker_news_summary_2026-04-14.md) |
| 187 | [2026-04-18](output/hacker_news_summary_2026-04-18.md) |
| 188 | [2026-04-16](output/hacker_news_summary_2026-04-16.md) |
| 189 | [2026-04-17](output/hacker_news_summary_2026-04-17.md) |
| 190 | [2026-04-15](output/hacker_news_summary_2026-04-15.md) |
| 191 | [2026-04-10](output/hacker_news_summary_2026-04-10.md) |
| 192 | [2026-04-12](output/hacker_news_summary_2026-04-12.md) |
| 193 | [2026-04-11](output/hacker_news_summary_2026-04-11.md) |
| 194 | [2026-04-13](output/hacker_news_summary_2026-04-13.md) |
| 195 | [2026-04-08](output/hacker_news_summary_2026-04-08.md) |
| 196 | [2026-04-09](output/hacker_news_summary_2026-04-09.md) |
| 197 | [2026-04-04](output/hacker_news_summary_2026-04-04.md) |
| 198 | [2026-04-02](output/hacker_news_summary_2026-04-02.md) |
| 199 | [2026-04-06](output/hacker_news_summary_2026-04-06.md) |
| 200 | [2026-04-07](output/hacker_news_summary_2026-04-07.md) |
| 201 | [2026-04-03](output/hacker_news_summary_2026-04-03.md) |
| 202 | [2026-04-05](output/hacker_news_summary_2026-04-05.md) |
| 203 | [2026-03-28](output/hacker_news_summary_2026-03-28.md) |
| 204 | [2026-03-29](output/hacker_news_summary_2026-03-29.md) |
| 205 | [2026-03-27](output/hacker_news_summary_2026-03-27.md) |
| 206 | [2026-04-01](output/hacker_news_summary_2026-04-01.md) |
| 207 | [2026-03-30](output/hacker_news_summary_2026-03-30.md) |
| 208 | [2026-03-31](output/hacker_news_summary_2026-03-31.md) |
| 209 | [2026-03-26](output/hacker_news_summary_2026-03-26.md) |
| 210 | [2026-03-22](output/hacker_news_summary_2026-03-22.md) |
| 211 | [2026-03-23](output/hacker_news_summary_2026-03-23.md) |
| 212 | [2026-03-25](output/hacker_news_summary_2026-03-25.md) |
| 213 | [2026-03-19](output/hacker_news_summary_2026-03-19.md) |
| 214 | [2026-03-20](output/hacker_news_summary_2026-03-20.md) |
| 215 | [2026-03-21](output/hacker_news_summary_2026-03-21.md) |
| 216 | [2026-03-18](output/hacker_news_summary_2026-03-18.md) |
| 217 | [2026-03-16](output/hacker_news_summary_2026-03-16.md) |
| 218 | [2026-03-15](output/hacker_news_summary_2026-03-15.md) |
| 219 | [2026-03-17](output/hacker_news_summary_2026-03-17.md) |
| 220 | [2026-03-14](output/hacker_news_summary_2026-03-14.md) |
| 221 | [2026-03-12](output/hacker_news_summary_2026-03-12.md) |
| 222 | [2026-03-09](output/hacker_news_summary_2026-03-09.md) |
| 223 | [2026-03-10](output/hacker_news_summary_2026-03-10.md) |
| 224 | [2026-03-11](output/hacker_news_summary_2026-03-11.md) |
| 225 | [2026-03-13](output/hacker_news_summary_2026-03-13.md) |
| 226 | [2026-03-07](output/hacker_news_summary_2026-03-07.md) |
| 227 | [2026-03-06](output/hacker_news_summary_2026-03-06.md) |
| 228 | [2026-03-03](output/hacker_news_summary_2026-03-03.md) |
| 229 | [2026-03-05](output/hacker_news_summary_2026-03-05.md) |
| 230 | [2026-03-04](output/hacker_news_summary_2026-03-04.md) |
| 231 | [2026-03-08](output/hacker_news_summary_2026-03-08.md) |
| 232 | [2026-02-28](output/hacker_news_summary_2026-02-28.md) |
| 233 | [2026-03-02](output/hacker_news_summary_2026-03-02.md) |
| 234 | [2026-02-25](output/hacker_news_summary_2026-02-25.md) |
| 235 | [2026-03-01](output/hacker_news_summary_2026-03-01.md) |
| 236 | [2026-02-27](output/hacker_news_summary_2026-02-27.md) |
| 237 | [2026-02-26](output/hacker_news_summary_2026-02-26.md) |
| 238 | [2026-02-22](output/hacker_news_summary_2026-02-22.md) |
| 239 | [2026-02-20](output/hacker_news_summary_2026-02-20.md) |
| 240 | [2026-02-21](output/hacker_news_summary_2026-02-21.md) |
| 241 | [2026-02-24](output/hacker_news_summary_2026-02-24.md) |
| 242 | [2026-02-23](output/hacker_news_summary_2026-02-23.md) |
| 243 | [2026-02-15](output/hacker_news_summary_2026-02-15.md) |
| 244 | [2026-02-19](output/hacker_news_summary_2026-02-19.md) |
| 245 | [2026-02-16](output/hacker_news_summary_2026-02-16.md) |
| 246 | [2026-02-17](output/hacker_news_summary_2026-02-17.md) |
| 247 | [2026-02-18](output/hacker_news_summary_2026-02-18.md) |
| 248 | [2026-02-12](output/hacker_news_summary_2026-02-12.md) |
| 249 | [2026-02-13](output/hacker_news_summary_2026-02-13.md) |
| 250 | [2026-02-14](output/hacker_news_summary_2026-02-14.md) |
| 251 | [2026-02-10](output/hacker_news_summary_2026-02-10.md) |
| 252 | [2026-02-11](output/hacker_news_summary_2026-02-11.md) |
| 253 | [2026-02-09](output/hacker_news_summary_2026-02-09.md) |
| 254 | [2026-02-04](output/hacker_news_summary_2026-02-04.md) |
| 255 | [2026-02-06](output/hacker_news_summary_2026-02-06.md) |
| 256 | [2026-02-08](output/hacker_news_summary_2026-02-08.md) |
| 257 | [2026-02-05](output/hacker_news_summary_2026-02-05.md) |
| 258 | [2026-02-07](output/hacker_news_summary_2026-02-07.md) |
| 259 | [2026-01-31](output/hacker_news_summary_2026-01-31.md) |
| 260 | [2026-02-01](output/hacker_news_summary_2026-02-01.md) |
| 261 | [2026-01-30](output/hacker_news_summary_2026-01-30.md) |
| 262 | [2026-01-28](output/hacker_news_summary_2026-01-28.md) |
| 263 | [2026-02-03](output/hacker_news_summary_2026-02-03.md) |
| 264 | [2026-01-29](output/hacker_news_summary_2026-01-29.md) |
| 265 | [2026-01-24](output/hacker_news_summary_2026-01-24.md) |
| 266 | [2026-01-23](output/hacker_news_summary_2026-01-23.md) |
| 267 | [2026-01-27](output/hacker_news_summary_2026-01-27.md) |
| 268 | [2026-01-26](output/hacker_news_summary_2026-01-26.md) |
| 269 | [2026-01-25](output/hacker_news_summary_2026-01-25.md) |
| 270 | [2026-01-22](output/hacker_news_summary_2026-01-22.md) |
| 271 | [2026-01-20](output/hacker_news_summary_2026-01-20.md) |
| 272 | [2026-01-18](output/hacker_news_summary_2026-01-18.md) |
| 273 | [2026-01-21](output/hacker_news_summary_2026-01-21.md) |
| 274 | [2026-01-19](output/hacker_news_summary_2026-01-19.md) |
| 275 | [2026-01-17](output/hacker_news_summary_2026-01-17.md) |
| 276 | [2026-01-16](output/hacker_news_summary_2026-01-16.md) |
| 277 | [2026-01-15](output/hacker_news_summary_2026-01-15.md) |
| 278 | [2026-01-14](output/hacker_news_summary_2026-01-14.md) |
| 279 | [2026-01-12](output/hacker_news_summary_2026-01-12.md) |
| 280 | [2026-01-13](output/hacker_news_summary_2026-01-13.md) |
| 281 | [2026-01-11](output/hacker_news_summary_2026-01-11.md) |
| 282 | [2026-01-08](output/hacker_news_summary_2026-01-08.md) |
| 283 | [2026-01-07](output/hacker_news_summary_2026-01-07.md) |
| 284 | [2026-01-10](output/hacker_news_summary_2026-01-10.md) |
| 285 | [2026-01-09](output/hacker_news_summary_2026-01-09.md) |
| 286 | [2026-01-04](output/hacker_news_summary_2026-01-04.md) |
| 287 | [2026-01-06](output/hacker_news_summary_2026-01-06.md) |
| 288 | [2026-01-03](output/hacker_news_summary_2026-01-03.md) |
| 289 | [2026-01-05](output/hacker_news_summary_2026-01-05.md) |
| 290 | [2026-01-01](output/hacker_news_summary_2026-01-01.md) |
| 291 | [2026-01-02](output/hacker_news_summary_2026-01-02.md) |
| 292 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 293 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 294 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 295 | [2025-12-31](output/hacker_news_summary_2025-12-31.md) |
| 296 | [2025-12-30](output/hacker_news_summary_2025-12-30.md) |
| 297 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 298 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 299 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 300 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 301 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 302 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 303 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 304 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 305 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 306 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 307 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 308 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 309 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 310 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 311 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 312 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 313 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 314 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 315 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 316 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 317 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 318 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 319 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 320 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 321 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 322 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 323 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 324 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 325 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 326 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 327 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 328 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 329 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 330 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 331 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 332 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 333 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 334 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 335 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 336 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 337 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 338 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 339 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
| 340 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 341 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 342 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 343 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 344 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 345 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 346 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 347 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
