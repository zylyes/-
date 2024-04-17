# 弹跳球模拟器

欢迎使用弹跳球模拟器，这是一个利用`pygame`库构建的简单2D物理引擎，用来展示小球在包含边界的盒子中，受力作用下的动态行为，包括重力、摩擦力和空气阻力等基本物理效应。

## 目录

- [开发信息](#开发信息)
- [特性概述](#特性概述)
- [安装指导](#安装指导)
- [使用教程](#使用教程)
- [文件说明](#文件说明)
- [程序结构说明](#程序结构说明)
- [技术细节](#技术细节)
- [许可与支持](#许可与支持)
- [团队与贡献](#团队与贡献)

## 开发信息

- **开发日期**：2024/04/14
- **开发者**：周咏霖

## 特性概述

本程序提供以下特性：

- **重力影响**：小球具有垂直下落的行为，模拟真实世界中的重力效应。
- **空气阻力**：小球在移动过程中会受到空气阻力的影响，影响其速度和加速度。
- **摩擦力模拟**：当小球与边界底部接触时，小球会受到摩擦力的作用，进而改变其运动状态。
- **能量损耗**：在与边界的碰撞过程中，小球会损失部分能量，这使得每次弹跳的高度逐渐减小。
- **可视化界面**：通过`pygame`库提供实时的图形界面，用户可以直观地观察到模拟中的物理现象。

## 安装指导

为了运行这个模拟器，你需要先安装`pygame`库。确保你的计算机已经安装了Python，并且版本至少为3.x。可以通过以下命令安装`pygame`库：

```bash
pip install pygame
```

**注意**：如果你使用的是Linux或macOS，可能需要在命令前加上`sudo`用于获取权限。

## 使用教程

1. **启动模拟器**：使用命令行切换到包含`Ball.py`的目录，执行以下命令启动程序：

   ```bash
   python Ball.py
   ```

2. **程序操作**：模拟器启动后不需要任何用户输入，小球会自动开始在框内弹跳。

例子：

参数：

gravity = 0.1   重力加速度

energy_loss_coeff = 0.8   反弹能量损失系数

friction_coeff = 0.02   摩擦系数

air_resistance_coeff = 0.001   空气阻力系数

运行演示：

![image](https://github.com/ZhengYaWei1992/ZWProgressView/blob/master/Untitled3.gif)

3. **退出模拟器**：当你想退出模拟器时，简单地关闭图形界面窗口即可。

## 文件说明

- `Ball.py`：主程序文件，包含小球和边界框的定义及游戏循环。

## 程序结构说明

程序主要包含以下几个部分：

1. `Ball` 类：用于创建小球对象，包含了小球的位置、半径、速度和颜色以及绘制小球的方法。
2. `Box` 类：用于创建边界框对象，定义了框的位置、大小和颜色以及绘制边界框的方法。
3. `pygame` 时间循环：程序的主循环，处理事件和更新小球位置及状态。
4. 碰撞检测：检查小球是否达到边界，并相应改变速度方向和大小，模仿物理中的能量损失。

## 技术细节

- 支持的Python版本：Python 3.x
- 依赖的第三方库：`pygame`

## 许可与支持

本软件是一个开源项目，请遵守项目中LICENSE文件的许可条款。

如果您有任何问题或建议，欢迎通过以下方式联系开发者：
- 电子邮件：[]
- 项目Issue页面：[]/issues

## 团队与贡献

目前这个项目由我个人维护。如果你有兴趣贡献代码或提供功能建议，非常欢迎你的加入！

感谢使用本模拟器，希望你在使用过程中有所获得，并对其中的物理现象有更深入的了解。
