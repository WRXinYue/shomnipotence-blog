---
title: 为 NanaZip 设计图标
date: 1684466197
updated: 1684558880
---

NanaZip 是一个开源文件归档器，旨在提供现代 Windows 体验，从著名的开源文件归档器 7-Zip 的源代码派生而来。  这也是世界上第一个支持 Windows 11 新版右键菜单 API 的应用。我与毛利目标相同，都旨在推动 Windows 应用的现代化。

<!-- more -->

## 概述
NanaZip 是一个开源文件归档器，旨在提供现代 Windows 体验，从著名的开源文件归档器 7-Zip 的源代码派生而来。

这也是世界上第一个支持 Windows 11 新版右键菜单 API 的应用。我与毛利目标相同，都旨在推动 Windows 应用的现代化。

## GitHub/路线图/构建
https://github.com/M2Team/NanaZip

## 下载地址
https://www.microsoft.com/store/productId/9N8G7TSCL18R

## 关键词
毛利告诉我，这个名字来自于

![输入图片说明](/uploads/20230519/d4fcc8bf201b2244ab4ab7a2acf62f86.png)

因此最好包含辣椒，和数字“7”（毕竟 NanaZip 派生自 7-Zip）

毛利和我都认为，NanaZip 显然需要一个 Fluent Design 风格的图标。

## 头脑风暴
### 第一组尝试

![输入图片说明](/uploads/20230519/8b98dc63db3aba39d611cd34e0d0ea77.png)

但毛利老哥说，这个主色调要红一些，于是……

![输入图片说明](/uploads/20230519/8eaff8561b68ee4429c48783133dbd0c.png)

但这显然不太合适，红色看起来像红包，黄色看起来像纸钱。

### 第二组尝试

这个色彩搭配是一个可以考虑融入的点，把衣物融入进来，就形成下图的样子

![输入图片说明](/uploads/20230519/5df1e919b3a3c831a82129a3c620af16.png)


![输入图片说明](/uploads/20230519/3ec38993ecd04459908e0284ad01a04a.png)

我个人非常喜欢这个想法，不过毛利说，还是更希望接近系统原生一些（虽然我反驳说这也很接近）。

### 第三组尝试

我认为档案袋也是一个可以考虑的方向，

![输入图片说明](/uploads/20230519/b6c59677af5685b20fcd889b0e609eda.png)

不过看到效果后毛利老哥更喜欢第二组的方向，但修改为蓝色配色。

## 细化方案

我们反复微调了配色、尺寸和圆角半径，确保在任务栏这类小尺寸情况，和深色、浅色两种主题中都能够拥有足够的辨识度。确保色系与 Windows 现有图标保持和谐且拥有独特的深蓝色的品牌色。

![输入图片说明](/uploads/20230519/28be6d748cbca3168bb85ea4d81d2065.png)

根据毛利的建议，在 1024x1024px 尺寸下，建立 64px 的网格，将线条对齐到网格，这样当缩小到 32x32px 时，边界仍然是清晰的。

在一开始底部是未对齐网格的，我认为1.5也是可以接受的。

![输入图片说明](/uploads/20230519/9876832fe22ff8d957929bc40781452d.png)

但毛利认为，应该对齐到网格，且保持从 16x16px 到 1024-1024px 的一致性。经过权衡，我认为毛利的观点更正确。我们最终决定

![输入图片说明](/uploads/20230519/c5823c78221cf27fdb2ee15a4c2ea9f0.png)

图标自然提供高对比度版本支持轻松访问功能。

![输入图片说明](/uploads/20230519/2284cf47aa364ba2234373b3e17ba3e1.png)

## 最终效果

![输入图片说明](/uploads/20230519/a2aa6fe5a2adfb0ca7f237bfaf64c531.png)

![输入图片说明](/uploads/20230519/896a75e365f8ad3a71b354be781769d2.png)

## 多尺寸适配

尽管 Figma 提供了一次性导出多尺寸功能，但我们仍然需要针对每个尺寸进行微调


![输入图片说明](/uploads/20230519/9bfc30225c02ac93344ccf0189bd91a8.png)

这是一项艰辛繁琐的工作，但完成之后可以确保每个尺寸下图标的边界都是清晰的。

## 设计文件类型图标

有些 App 将主图标和文件类型图标几乎混在一起，长得非常相似，这是不负责任的。

我们的设计目标是：
- 与系统当前的文件类型图标一致；
- 更多体现文件，而不是像默认的 Zip 文件类型图标一样体现为文件夹；
- 与应用主图标相呼应。

![输入图片说明](/uploads/20230519/ef7d972b96421db8d17702bdcdd3c93f.png)

在我们实际测试中，尽管在大尺寸下图左最合适，但它在“详细信息列表”中表现不佳，拉链太小，几乎无法分辨。因此我们使用中间和右边那版。
