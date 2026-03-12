# Unity 2022.3.74f1 LTS
发布于北京时间 2026 年 3 月 11 日星期三 10:15:36
https://unity.com/releases/editor/whats-new/2022.3.74f1

# 2022.3.74f1 中的已知问题



* iOS/tvOs：目标最低 iOS/tvOs 版本显示为 12，而由于 UIScene 要求，iOS/tvOS 13 自 2022.3.72f1 起已是新的最低版本。手动提高至 13，以避免在不支持 UIScene 的 iOS12 设备上发生崩溃。
* 金属：  命令缓冲区超时错误后游戏冻结
([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))
* 金属：在 "播放模式 "下的 "编辑器 "中的最小项目中，macOS 会出现卡顿现象
([uum-85256](https://issuetracker.unity3d.com/issues/macos-stutters-in-a-minimal-project))
* 视频：修复 2022.3.X：在某些 Android 设备上多次启用和禁用视频时，VideoPlayer 会冻结或停止的问题
(UUM-112470)
* 视窗：启用 "后台运行 "并切换活动窗口时播放器会挂起
([UUM-130495](https://issuetracker.unity3d.com/issues/player-hangs-when-the-run-in-background-is-enabled-and-active-window-is-switched))



# 2022.3.74f1 发行说明

## 功能

* 编辑器：新增洞察力和引擎诊断（默认关闭）。


