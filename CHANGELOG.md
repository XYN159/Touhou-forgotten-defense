# 更新日志

格式遵循 [Keep a Changelog](https://keepachangelog.com/zh-CN/1.1.0/)，版本号遵循[语义化版本](https://semver.org/lang/zh-CN/)。

## [Unreleased]

### 变更

- 首页介绍的启动图去掉左右两块黑色空白，空出来的位置补上神社夜景。标题、灵梦和「点击开始」没有改。
- 服务器选择图里，红魔馆、白玉楼、月之廊各只写一遍。
- 仓库首页的介绍加上二十张界面原画。登录和选服务器只是画面，不建账号，也不连网。
- 对外名称从 The Last Survivor（最后的幸存者）改为《东方守幻录》。英文仓库名是 touhou-forgotten-defense。定位改为东方Project 同人、个人免费非商业的竖屏角色塔防，不是弹幕射击。调试 APK 文件名改为 `touhou-forgotten-defense-*`，Android 包名改为 `com.xyn159.touhouforgottendefense`。
- GitHub 首页的 `README.md` 整份改写成《东方守幻录》的介绍。

### 新增

- 为 60 秒宣传 PV 补了概念静帧：红美铃、十六夜咲夜、上白泽慧音、藤原妹红、东风谷早苗、大妖精、蕾米莉亚、射命丸文，以及「忘」的剪影场景和结界尽头场景。图在 `docs/design/art/concepts/`，待挑选，不是游戏正式立绘，不进 `assets/`。
- 建立 Godot 4.7.2 竖屏工程，包含标题画面和占位战斗车道。
- 加入 GDScript 格式检查、GUT 单元测试，以及调试版 Android APK 的持续集成。CI 固定在 Ubuntu 24.04 上运行。
- 写好协作文档、玩法草案、架构说明和架构决定记录。
- 加入 Cursor 工作区配置（推荐 godot-tools、语言服务器端口 6005、从编辑器启动游戏），并写好每天并排改游戏的说明 `docs/DEV_LOOP.md`。
- 把 Cursor 里的 Godot 路径改成这台 Windows 电脑上的 `D:/Godot_v4.7.2-stable_win64.exe/Godot_v4.7.2-stable_win64.exe`。

[Unreleased]: https://github.com/XYN159/touhou-forgotten-defense/compare/main...HEAD
