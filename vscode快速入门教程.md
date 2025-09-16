# vscode快速入门指南
- 文档版本：1.0
- 最后更新：2025-9-15
- 作者：杨璐（yli8i3@163.com）
- 操作系统：操作步骤和截图均基于Windows 10/11操作系统。如果您使用macOS或Linux，安装、配置和部分操作细节会有所不同，建议您参考官方提供的其他安装指南。
  
## 目标读者
本教程适用于非技术背景，第一次接触代码编辑器的新手。我们假设你没有任何编程经验，仅使用过word或记事本处理文本。本教程将从软件下载开始引导你学习vscode的安装、配置、熟悉核心功能，最终能够使用vscode来编辑和运行你的代码。

## 文档概述
VS Code（全称Visual Studio Code）是一款微软开发的代码编辑器，支持Windows、macOS和Linux系统，具有完善的开发必备功能（如提示、调试），可以满足从简单脚本编写到复杂项目开发等多种需求。
本教程包含以下几个章节
...
安装
配置
页面介绍
核心功能

## 教程

### 1.安装vscode
- 进入[vscode官网](code.visualstudio.com)，在网页顶部最右侧找到`Download`，点击`Download`下载安装包。
如图：
![Download位置](images\Download.png)

- 点击之后会弹出系统各自的版本：
![选择版本](images\Download-system.png)
对于个人使用，建议直接点击最大的`Windows 10,11`

- 在安装的过程中，安装向导会提供一些选项：
  -  `Add to Path (restart required)`:建议勾选，可以通过CMD等命令行工具打开vsode
  -  `Register '.vscode' directory as Git repository root`:建议取消勾选,容易造成版本混乱
  -  `Download additional binaries to support ARM64/ x64 architectures`:建议取消勾选，功能对于新手比较冗余，主要面向专业嵌入式开发者以及需要为多设备交叉编译程序的开发者
  -  `Create a desktop shortcut`：建议勾选，在桌面创建图标便于寻找
- 等待安装完成即可
  
### 2.配置
