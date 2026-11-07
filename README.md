# 清弈

清弈是一款用于中国象棋打谱、复盘和棋谱管理的 Windows 桌面软件。记录一盘棋、整理棋谱收藏，或借助引擎研究局面，都可以在同一个工作区中完成。

本仓库用于公开发布清弈的软件包、更新文件及版本说明，不包含项目源码。

## 下载

- [最新版本](https://github.com/persysc/QingYi_publish/releases/latest)
- [全部版本与更新记录](https://github.com/persysc/QingYi_publish/releases)

首次使用请选择版本说明中提供的完整软件包，并按说明安装或解压。仅用于在线更新的主程序 EXE 不包含全部运行资源，不能代替完整软件包。

## 主要功能

- **打谱与复盘**：录入、浏览和编辑棋谱，支持多分支变招、棋步注释与沙盘推演。
- **棋谱管理**：文件夹与棋库管理，支持多选、批量操作，以及图标、列表、树形视图。
- **多种格式**：支持 QY、QYL、XQF、PGN、UBB／DXQ、象棋桥 CBR／CBL 等棋谱或棋库的读取；可导出的格式以软件内选项为准。
- **引擎分析**：支持本机象棋引擎、多线路 PV 分析与云库招法查询。
- **局面工具**：FEN、UBB 复制与导入，棋图复制、GIF 导出，以及按局面检索棋谱。
- **个性化工作区**：棋盘与棋子皮肤、走棋动画、动态棋盘，以及可自由调整的组件布局。
- **离线帮助**：内置教程说明书与操作练习，方便逐步熟悉软件。

具体功能与兼容情况请以所下载版本的说明为准。

## 在线更新

接入本仓库更新源的清弈版本，可在软件内检查并下载更新。客户端读取 `update.txt`，比较远端 MD5 与当前主程序的 MD5；不同时提示更新。下载优先使用 GH-Proxy 加速，失败后尝试 GitHub 直连，下载完成后再次校验 MD5。

每个用于在线更新的正式 Release 包含以下附件：

| 附件 | 用途 |
| --- | --- |
| `qingyi.exe` | 清弈主程序，由软件内的更新流程下载，用于替换主程序 |
| `update.txt` | 只包含该 EXE 的 32 位 MD5 |
| 完整软件包（如提供） | 用于首次安装或需要同步更新运行资源的版本 |

`update.txt` 使用 UTF-8 编码，只写 EXE 的 32 位 MD5，不附加版本号或下载地址。两个附件都上传完成后，再正式发布并将该 Release 设为 Latest，附件名始终保持不变。

客户端使用固定地址获取最新附件：

```text
https://github.com/persysc/QingYi_publish/releases/latest/download/update.txt
https://github.com/persysc/QingYi_publish/releases/latest/download/qingyi.exe
```

检测只比较文件内容，不判断版本高低，因此请将 Latest 指向希望用户使用的正式版本。

旧版若仍使用已经失效的更新源，需要先手动安装一次接入新更新源的版本。

## 反馈与作者

使用问题可通过 [Issues](https://github.com/persysc/QingYi_publish/issues) 反馈。请尽量附上软件版本、复现步骤和相关截图，方便定位。

作者：可以步武 · [B站主页](https://space.bilibili.com/177937672)
