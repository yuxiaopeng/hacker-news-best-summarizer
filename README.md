# Hacker News 每日摘要
    
这是 Top 10 的每日摘要，更多请点击 [Top 100](output/hacker_news_summary_2025-12-29.md)

*最后自动更新时间: 2025-12-29 19:46:54*
## 1. 原图是什么样子

**原文标题**: What an unprocessed photo looks like

**原文链接**: [https://maurycyz.com/misc/raw_photo/](https://maurycyz.com/misc/raw_photo/)

相机传感器未经处理的照片，远非我们所感知到的样子。最初，它只是一幅由模数转换器 (ADC) 值组成的“灰蒙蒙”图像，通常未充分利用其理论范围，且缺乏对比度。

要转换为可观看的图像，需要经过以下几个处理步骤：

1.  **定标：** 初始 ADC 值需要映射到可显示的黑白范围，以提高对比度，将“灰蒙蒙”的图像转换为具有更清晰明暗色调的图像。
2.  **去马赛克：** 相机传感器不直接感知颜色；它们使用拜耳滤色阵列，其中每个像素只捕获红色、绿色或蓝色光。为了创建全彩图像，去马赛克算法会平均相邻像素值，以插值每个像素缺失的颜色信息。
3.  **色调映射 (伽马校正)：** 即使在去马赛克之后，图像仍显得很暗。这是因为与传感器和人眼相比，显示技术的动态范围有限。此外，人眼对亮度的感知是非线性的。应用非线性曲线（如sRGB）可以提亮较暗区域，使图像更准确地呈现感知的亮度。
4.  **白平衡：** 相机传感器可能对某些颜色（如绿色）更敏感，去马赛克可能会放大这种敏感性，导致偏色。白平衡通过调整每个颜色通道的强度来校正这些问题，确保中性色显示为中性。这一步通常需要在色调映射之前在线性数据上完成。

文章总结道，即使是“机内”JPEG图像也经过了大量的数学处理。在编辑软件中调整图像并非使其“虚假”，而只是对相同原始数据进行不同形式的呈现，旨在显示技术限制内更好地复制人眼感知。

---

## 2. 日历

**原文标题**: Calendar

**原文链接**: [https://neatnik.net/calendar/?year=2026](https://neatnik.net/calendar/?year=2026)

本页面提供一份2026年全年一页式日历，旨在将所有日期呈现在任意尺寸的单张纸上。为获得最佳打印效果，建议用户将打印机设置为横向并禁用页眉和页脚。这份日历鼓励用户一眼纵览全年，折叠便于携带，记录笔记，规划活动，并观察时间的流逝。日历中还包含一则普遍的善意信息。本页日历由Neatnik创建。

---

## 3. Growing up in “404 Not Found”: China's nuclear city in the Gobi Desert

**原文标题**: Growing up in “404 Not Found”: China's nuclear city in the Gobi Desert

**原文链接**: [https://substack.com/inbox/post/182743659](https://substack.com/inbox/post/182743659)

生成摘要时出错

---

## 4. 仅用 HTML 替换 JavaScript

**原文标题**: Replacing JavaScript with Just HTML

**原文链接**: [https://www.htmhell.dev/adventcalendar/2025/27/](https://www.htmhell.dev/adventcalendar/2025/27/)

Aaron T. Grogg的文章《仅用HTML替代JS》倡导利用原生的HTML和CSS功能，以减少对JavaScript在常见网页功能上的依赖。该文章于2025年12月27日发表，认为尽管JS一直至关重要，但许多它传统上处理的任务现在可以由现代HTML和CSS更高效地完成，从而带来更好的用户体验。

核心前提是，将功能卸载到原生浏览器实现中，意味着需要下载、解压缩、评估和内存中维护的JavaScript更少。这将JS解放出来用于更复杂的任务，同时提高网站性能。

Grogg提供了实用示例：
1.  **手风琴/可展开内容面板：** 通过`<details>`和`<summary>`元素实现，提供原生的打开/关闭状态，并可使用`name`属性实现类似单选按钮的行为。
2.  **带自动过滤建议的输入下拉框：** 使用带有`list`属性的`<input>`元素实现，该属性链接到一个`<datalist>`元素，以实现选项的自动过滤。
3.  **模态框/弹出窗口：** 被`<dialog>`元素上的`popover`和`popovertarget`属性替代，能够实现各种类型的弹出窗口，并具有内置的轻量级关闭和辅助功能。
4.  **屏外导航/内容：** 结合CSS动画过渡，使用`popover`属性，创建无需JavaScript的屏外导航菜单。

该文章鼓励开发人员在可用时优先考虑原生解决方案，尊重JavaScript，将其用于真正需要它的地方，从而创建更轻量、更快速的Web应用程序。

---

## 5. 被德国铁路绑架

**原文标题**: Kidnapped by Deutsche Bahn

**原文链接**: [https://www.theocharis.dev/blog/kidnapped-by-deutsche-bahn/](https://www.theocharis.dev/blog/kidnapped-by-deutsche-bahn/)

The article, "Kidnapped by Deutsche Bahn," recounts a frustrating Christmas Eve train journey on December 24th, 2025, that turned into an unexpected ordeal. The author planned a 35-kilometer trip from Cologne to Meckenheim, but the train, already twenty minutes late, announced "issues around Bonn," necessitating a detour.

The author decided to exit at Troisdorf to be picked up by his father. However, as the RE5 train approached Troisdorf, the driver announced it couldn't stop because it was "not registered" for the tracks. The author watched Troisdorf, and his waiting father, pass by. He was unexpectedly carried to Neuwied, 63 kilometers from his grandmother's house and in a different federal state—further away than his starting point.

Feeling like "cargo" and "kidnapped," the author noted the shared frustration among passengers. He also highlighted Deutsche Bahn's lenient punctuality metrics, where trains less than six minutes late are "on time," and cancelled trains aren't counted. His eventual compensation for this severe delay was a mere 1.50 EUR, below the 4.00 EUR minimum payout threshold, meaning he was "kidnapped at a loss." The piece sarcastically details the systemic unreliability and public exasperation with DB's service.

---

## 6. 我们如何将沟通输给了娱乐

**原文标题**: How we lost communication to entertainment

**原文链接**: [https://ploum.net/2025-12-15-communication-entertainment.html](https://ploum.net/2025-12-15-communication-entertainment.html)

生成摘要时出错

---

## 7. 对NHS中的帕兰提尔说不

**原文标题**: Say No to Palantir in the NHS

**原文链接**: [https://notopalantir.goodlawproject.org/email-to-target/stop-palantir-in-the-nhs/](https://notopalantir.goodlawproject.org/email-to-target/stop-palantir-in-the-nhs/)

本文呼吁公众“拒绝Palantir进入NHS”，反对英格兰国民医疗服务体系（NHS England）推出这家美国间谍技术公司用于管理健康记录的软件。

这项运动强调了对Palantir背景的严重担忧，引用其据称在美国参与大规模驱逐出境，并促成加沙种族灭绝。此外，Palantir的联合创始人彼得·蒂尔（Peter Thiel）因其对NHS的公开敌意而闻名，他曾声称NHS“让人生病”，并暗示英国公众因支持NHS而患有“斯德哥尔摩综合症”。

该文章警告不要允许这样一家公司控制英国的医疗保健系统，并呼吁采取紧急行动。它提供了一个工具，供个人检查他们的当地NHS信托机构是否已采用该软件。主要的行动呼吁是向当地NHS信托机构以及卫生大臣韦斯·斯特里廷（Wes Streeting）发送电子邮件，要求他们拒绝Palantir，尤其是在政府向各信托机构施压要求其采用该软件的情况下。

---

## 8. You can make up HTML tags

**原文标题**: You can make up HTML tags

**原文链接**: [https://maurycyz.com/misc/make-up-tags/](https://maurycyz.com/misc/make-up-tags/)

本文强调HTML开发者可以创建和使用自定义标签（例如`<cool-thing>`），而不是使用带有类的通用`div`标签。浏览器会自动将这些未识别的标签视为通用元素，并应用在CSS中为其定义的任何样式。这并非一个异常，而是标准化行为。在自定义标签名称中包含连字符（例如`<main-article>`）可以确保它们不会与未来的HTML标准冲突。

这种方法的主要好处是极大提升了代码的可读性和可维护性，尤其对于复杂或深度嵌套的结构。文章对比了一系列难以理解的带类的嵌套`div`结构，以及使用描述性自定义标签的结构。后者消除了对`</div>`进行计数的需要，使得理解结构和精确找到插入点变得容易得多。尽管在适当情况下应使用现有的语义化HTML标签，但自定义标签为大量使用带有众多类名的`<div>`或`<span>`提供了一种更具可读性的替代方案，从而为自定义组件提供了更好的清晰度。

---

## 9. 去年我的 Mac：难以置信

**原文标题**: Last Year on My Mac: Look Back in Disbelief

**原文链接**: [https://eclecticlight.co/2025/12/28/last-year-on-my-mac-look-back-in-disbelief/](https://eclecticlight.co/2025/12/28/last-year-on-my-mac-look-back-in-disbelief/)

The author expresses profound disappointment with macOS Tahoe's "Liquid Glass" interface changes, stating that feedback from beta testing was ignored and subsequent updates (26.1, 26.2) worsened or failed to address issues.

Key criticisms include:
1.  **Excessively Rounded Corners:** Tahoe's increased window corner radius is a misfit for rectangular content, causing cropping, wasted space, and inconsistent appearance across apps.
2.  **Enlarged Controls:** Controls are bigger but offer no functional benefit, often leading to visual clutter and overlapping elements.
3.  **Uniform App Icons:** The enforced square shape restricts visual cues, making many bundled and Apple apps harder to distinguish and recall in the Dock.
4.  **Lack of Tonal Contrast ("Whiteout"):** Both Light Mode (bleached-out white) and Dark Mode (moonless night) lack sufficient contrast, making it difficult to discern controls, text fields, and other interface elements.
5.  **Problematic Transparency ("Wet-on-wet"):** Extensive transparency renders elements like search boxes and window titles incomprehensible when underlaid by content, creating a confusing and distracting visual experience.
6.  **Accessibility Regression:** The "Reduce Transparency" control in Accessibility settings no longer effectively lessens these visual effects, a significant regression.

The author, drawing on experience with older Apple interfaces, concludes that Tahoe sacrifices clarity and functionality, making the display harder to read and use.

---

## 10. Show HN: Z80-μLM, a 'Conversational AI' That Fits in 40KB

**原文标题**: Show HN: Z80-μLM, a 'Conversational AI' That Fits in 40KB

**原文链接**: [https://github.com/HarryR/z80ai](https://github.com/HarryR/z80ai)

生成摘要时出错

---

## 历史记录

| 序号 | 文件 |
| --- | --- |
| 1 | [2025-12-29](output/hacker_news_summary_2025-12-29.md) |
| 2 | [2025-12-28](output/hacker_news_summary_2025-12-28.md) |
| 3 | [2025-12-23](output/hacker_news_summary_2025-12-23.md) |
| 4 | [2025-12-27](output/hacker_news_summary_2025-12-27.md) |
| 5 | [2025-12-25](output/hacker_news_summary_2025-12-25.md) |
| 6 | [2025-12-24](output/hacker_news_summary_2025-12-24.md) |
| 7 | [2025-12-26](output/hacker_news_summary_2025-12-26.md) |
| 8 | [2025-12-19](output/hacker_news_summary_2025-12-19.md) |
| 9 | [2025-12-21](output/hacker_news_summary_2025-12-21.md) |
| 10 | [2025-12-22](output/hacker_news_summary_2025-12-22.md) |
| 11 | [2025-12-20](output/hacker_news_summary_2025-12-20.md) |
| 12 | [2025-12-16](output/hacker_news_summary_2025-12-16.md) |
| 13 | [2025-12-15](output/hacker_news_summary_2025-12-15.md) |
| 14 | [2025-12-18](output/hacker_news_summary_2025-12-18.md) |
| 15 | [2025-12-17](output/hacker_news_summary_2025-12-17.md) |
| 16 | [2025-12-11](output/hacker_news_summary_2025-12-11.md) |
| 17 | [2025-12-13](output/hacker_news_summary_2025-12-13.md) |
| 18 | [2025-12-12](output/hacker_news_summary_2025-12-12.md) |
| 19 | [2025-12-14](output/hacker_news_summary_2025-12-14.md) |
| 20 | [2025-12-07](output/hacker_news_summary_2025-12-07.md) |
| 21 | [2025-12-06](output/hacker_news_summary_2025-12-06.md) |
| 22 | [2025-12-08](output/hacker_news_summary_2025-12-08.md) |
| 23 | [2025-12-09](output/hacker_news_summary_2025-12-09.md) |
| 24 | [2025-12-10](output/hacker_news_summary_2025-12-10.md) |
| 25 | [2025-12-05](output/hacker_news_summary_2025-12-05.md) |
| 26 | [2025-12-04](output/hacker_news_summary_2025-12-04.md) |
| 27 | [2025-12-03](output/hacker_news_summary_2025-12-03.md) |
| 28 | [2025-12-02](output/hacker_news_summary_2025-12-02.md) |
| 29 | [2025-12-01](output/hacker_news_summary_2025-12-01.md) |
| 30 | [2025-11-30](output/hacker_news_summary_2025-11-30.md) |
| 31 | [2025-11-29](output/hacker_news_summary_2025-11-29.md) |
| 32 | [2025-11-28](output/hacker_news_summary_2025-11-28.md) |
| 33 | [2025-11-27](output/hacker_news_summary_2025-11-27.md) |
| 34 | [2025-11-26](output/hacker_news_summary_2025-11-26.md) |
| 35 | [2025-11-25](output/hacker_news_summary_2025-11-25.md) |
| 36 | [2025-11-24](output/hacker_news_summary_2025-11-24.md) |
| 37 | [2025-11-23](output/hacker_news_summary_2025-11-23.md) |
| 38 | [2025-11-22](output/hacker_news_summary_2025-11-22.md) |
| 39 | [2025-11-21](output/hacker_news_summary_2025-11-21.md) |
| 40 | [2025-11-20](output/hacker_news_summary_2025-11-20.md) |
| 41 | [2025-11-19](output/hacker_news_summary_2025-11-19.md) |
| 42 | [2025-11-18](output/hacker_news_summary_2025-11-18.md) |
| 43 | [2025-11-17](output/hacker_news_summary_2025-11-17.md) |
| 44 | [2025-11-16](output/hacker_news_summary_2025-11-16.md) |
| 45 | [2025-11-11](output/hacker_news_summary_2025-11-11.md) |
| 46 | [2025-11-12](output/hacker_news_summary_2025-11-12.md) |
| 47 | [2025-11-13](output/hacker_news_summary_2025-11-13.md) |
| 48 | [2025-11-15](output/hacker_news_summary_2025-11-15.md) |
| 49 | [2025-11-14](output/hacker_news_summary_2025-11-14.md) |
| 50 | [2025-11-08](output/hacker_news_summary_2025-11-08.md) |
| 51 | [2025-11-06](output/hacker_news_summary_2025-11-06.md) |
| 52 | [2025-11-07](output/hacker_news_summary_2025-11-07.md) |
| 53 | [2025-11-10](output/hacker_news_summary_2025-11-10.md) |
| 54 | [2025-11-09](output/hacker_news_summary_2025-11-09.md) |
