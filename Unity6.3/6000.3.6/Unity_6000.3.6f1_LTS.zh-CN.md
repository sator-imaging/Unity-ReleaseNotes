# Unity 6000.3.6f1 LTS
发布于 Thu, 29 Jan 2026 10:44:38 GMT
https://unity.com/releases/editor/whats-new/6000.3.6f1

# 6000.3.6f1 中的已知问题

- 6000.0.54f1：在配置文件分析器比较工具中加载两个配置文件捕获时，崩溃率为 100%
    ([uum-132332](https://issuetracker.unity3d.com/issues/100-percent-crash-rate-when-loading-two-profiler-captures-in-the-profile-analyzer-compare-tool))

- 6000.0.55f1,6000.3.0a4：在切换用户界面时创建多人房间时发生 RaiseException 时崩溃
    ([uum-132182](https://issuetracker.unity3d.com/issues/crash-on-raiseexception-when-creating-a-multiplayer-room-while-toggling-ui))

- 6000.0.64f1：[DX12] [Win11 ARM64] 尝试创建新项目时机器崩溃并重启
    ([uum-131104](https://issuetracker.unity3d.com/issues/dx12-win11-arm64-machine-crashes-and-restarts-while-trying-to-create-a-new-project))

- 6000.1.0a2,6000.0.64f1：单通道立体渲染在进入播放模式时只显示天空盒
    ([uum-132342](https://issuetracker.unity3d.com/issues/single-pass-stereo-rendering-shows-only-skybox-when-entering-play-mode))

- 6000.3.0a1: 当发生域重载时，停靠动画窗口前最后选定的资产被选中
    ([uum-131198](https://issuetracker.unity3d.com/issues/last-selected-asset-before-docking-animation-window-gets-selected-when-a-domain-reload-occurs))

- 6000.3.0a1: [WinEditor] 当搜索本地对话框时，编辑器在焦点丢失后 "冻结
    ([uum-132303](https://issuetracker.unity3d.com/issues/the-editor-freezes-and-leaks-memory-when-cancelling-the-switch-of-the-default-render-pipeline-while-using-the-advanced-object-selector))

- 6000.3.0b1,6000.0.65f1：当质量设置（QualitySettings.maxQueuedFrames）设为 1 并使用 DX12 时，编辑器会冻结
    ([uum-131962](https://issuetracker.unity3d.com/issues/editor-freezes-when-qualitysettings-dot-maxqueuedframes-is-set-to-1-and-dx12-is-used))

- 6000.5.0a1,6000.3.2f1：当使用 DX12 并选择所有样条线节时，出现多个堆栈跟踪的崩溃现象
    ([uum-131707](https://issuetracker.unity3d.com/issues/crash-with-multiple-stack-traces-when-using-dx12-and-selecting-all-spline-knots))

- iOS：  启用 "显示闪屏 "并使用 "Unity 作为库 "构建项目时，渲染冻结和 UnityGfxDeviceWorker 崩溃
    ([uum-130881](https://issuetracker.unity3d.com/issues/ios-rendering-freezes-and-unitygfxdeviceworker-crash-when-show-splash-screen-is-enabled-and-project-is-built-using-unity-as-a-library))

- 金属：  命令缓冲区超时错误后游戏冻结
    ([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- 金属：[iOS] iOS 闪屏后屏幕闪烁
    ([uum-121453](https://issuetracker.unity3d.com/issues/ios-screen-flashing-after-the-ios-splash-screen))

- 平台音频：[Windows] 在编辑器中执行各种操作时，AudioManager::InitFMOD 会崩溃
    ([uum-126803](https://issuetracker.unity3d.com/issues/crash-on-audiomanager-initfmod-when-performing-various-actions-in-the-editor))

- SRP 模板：删除了 VR 模块依赖性，导致 URP 样本无法编译
    ([uum-130083](https://issuetracker.unity3d.com/issues/removed-vr-module-dependency-prevents-urp-sample-from-compiling))

- uGUI 控件：[iOS][Android]在移动端取消键盘后，在 UGUI 输入字段上无限期触发 OnSubmit 事件
    ([uum-130350](https://issuetracker.unity3d.com/issues/ios-android-onsubmit-event-is-triggered-indefinitely-on-ugui-input-field-after-dismissing-keyboard-on-mobile))

- : 在空白 URP 项目中进入和退出播放模式时编辑器内存泄漏
    ([uum-132677](https://issuetracker.unity3d.com/issues/editor-memory-leak-when-entering-and-exiting-play-mode-in-a-blank-urp-project))

- : 导入 SVG 文件时无声崩溃
    ([uum-132415](https://issuetracker.unity3d.com/issues/silent-crash-when-importing-svg-files))



# 6000.3.6f1 发行说明

## 修复

- 自适应性能：修正了自适应性能非开发版本的日志记录。
    (UUM-131941)

- 编辑器：更改了工具栏元素的最大宽度，以修复过小的元素。
    (STO-3747)

- 编辑器修复了 BIDI 包装溢出。
    (UUM-128666)

- 编辑器：修正了使用多线程时文本中的空异常。
    (UUM-132168)

- 编辑器：修正了 UGUI<br>。
    修正了在某些显示分辨率下滚动矩形会失去惯性的问题。
    ([UUM-99716](https://issuetracker.unity3d.com/issues/scroll-view-is-not-moving-by-inertia-after-scrolling-by-click-and-dragging-when-editor-window-is-minimized-and-canvas-render-mode-is-set-to-world-space))

- 编辑器：如果偏好文件夹不存在，Linux 编辑器现在会在启动编辑器时创建该文件夹。如果无法创建，将在 Editor.log 中写入错误信息。
    ([uum-128719](https://issuetracker.unity3d.com/issues/linux-preferences-directory-is-not-created-when-the-editor-is-installed-or-launched))

- 多人游戏：当安装了安卓支持但安卓 SDK 未链接到 Unity 编辑器时，多人游戏模式 "本地实例 "列表显示为空并抛出 ArgumentNullException。
    ([uum-131458](https://issuetracker.unity3d.com/issues/multiplayer-play-mode-local-instances-list-appears-empty-and-throws-an-argumentnullexception-when-android-support-is-installed-but-android-sdk-is-not-linked-to-the-unity-editor))

- 软件包管理器：修复了在资产商店更新 UPM 软件包时进度指示器不起作用的问题。
    (UUM-115289)

- 用户界面工具包：修正了精灵加载。
    ([UUM-131361](https://issuetracker.unity3d.com/issues/trygetvalue-fails-to-parse-uss-variable-into-sprite-when-using-customstyleproperty))




## 6000.3.6f1 中的软件包变更

## 更新的软件包

- com.unity.animation.rigging：[1.4.0](https://docs.unity3d.com/Packages/com.unity.animation.rigging@1.4//changelog/CHANGELOG.html) 到 [1.4.1](https://docs.unity3d.com/Packages/com.unity.animation.rigging@1.4//changelog/CHANGELOG.html)

- com.unity.inputsystem：[1.17.0](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.17//changelog/CHANGELOG.html) 到 [1.18.0](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.18//changelog/CHANGELOG.html)

- com.unity.performance.profile-analyzer：[1.2.4](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.2//changelog/CHANGELOG.html) 到 [1.3.1](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.3//changelog/CHANGELOG.html)

- com.unity.services.cloud-build：[2.0.6](https://docs.unity3d.com/Packages/com.unity.services.cloud-build@2.0//changelog/CHANGELOG.html) 到 [2.0.7](https://docs.unity3d.com/Packages/com.unity.services.cloud-build@2.0//changelog/CHANGELOG.html)

- com.unity.multiplayer.tools：[2.2.6](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@2.2//changelog/CHANGELOG.html) 到 [2.2.7](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@2.2//changelog/CHANGELOG.html)