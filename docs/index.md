# 欢迎阅读 SlopeCraft 文档

![SlopeCraft](_static/image/SlopeCraft.png)

## 关于 SlopeCraft

SlopeCraft是一个Minecraft像素画/地图画生成器，包含如下几个工具：

|                  名称                  | 介绍                                                                            |
| :------------------------------------: | :------------------------------------------------------------------------------ |
|  [SlopeCraft](SlopeCraft-tutorial.md)  | 生成用于 Minecraft 地图的生成器，包括但不限于立体地图和，**不适合玩家直接观看** |
| [VisualCraft](VisualCraft-tutorial.md) | 生成普通像素画的生成器，**适合玩家直接观看**，支持俯视、侧视和仰视视角的像素画  |
|              imageCutter               | 缩放、切割图像用的辅助工具                                                      |
|               MapViewer                | 浏览 Minecraft 地图数据文件的辅助工具                                           |
|                  vccl                  | 与 VisualCraft 功能相同的命令行工具                                             |

## 现有文档

1. [原理简介](./principles-introduction.md)
2. [SlopeCraft 使用教程](./SlopeCraft-tutorial.md)
3. [VisualCraft 使用教程](./VisualCraft-tutorial.md)
4. [编译指南](./compilation-guide/index.md)
5. 代码贡献指南（施工中）
6. 文档贡献指南（施工中）

## 为什么要有 SlopeCraft？

很多玩家在建造地图画之后，会习惯于用地图记录地图画，然后把地图挂在墙上。但这时候细心一点的人就会发现地图呈现的颜色与直接看到的差异很大。SlopeCraft 就是为了克服这种差异而诞生的，也因此，SlopeCraft 生成的地图画在设计之初就不是给玩家直接观看的。

一个常见的误区是，SlopeCraft 允许生成**平板地图画**，但平板地图画与 VisualCraft 的任务是完全不同的。平板地图画在设计之初就不是给玩家直接观看的，而只是立体地图画的一个亚种，它只是二维的立体地图画。

## 为什么要有 VisualCraft？

传统的像素画生成器确实已经很多了，看起来 VisualCraft 似乎不是很必要。但我实现了几个新颖的技术：

1. 将多个半透明方块叠加在不透明方块上，组成上万种不同的新颜色，极大提升像素画转化的效果。
2. 根据生物群系正确计算树叶和草的颜色
3. 通过解析方块模型，支持第三方材质包自定义的方块模型

为了实现这些功能，我开发了 VisualCraft。
