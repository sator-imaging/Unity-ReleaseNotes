# Unity 6000.0.67f1 LTS
发布于 星期三, 04 二月 2026 11:53:51 GMT
https://unity.com/releases/editor/whats-new/6000.0.67f1

# 6000.0.67f1 中的已知问题

- `6000.0.55f1,6000.3.0a4`：在切换用户界面时创建多人房间时发生 RaiseException 时崩溃
    ([uum-132182](https://issuetracker.unity3d.com/issues/crash-on-raiseexception-when-creating-a-multiplayer-room-while-toggling-ui))

- 6000.1.0a2,6000.0.64f1`：进入游戏模式时，单通道立体渲染只显示天空盒
    ([uum-132342](https://issuetracker.unity3d.com/issues/single-pass-stereo-rendering-shows-only-skybox-when-entering-play-mode))

- 6000.3.0b1,6000.0.65f1`：当质量设置（QualitySettings.maxQueuedFrames）设为 1 并使用 DX12 时，编辑器会冻结
    ([uum-131962](https://issuetracker.unity3d.com/issues/editor-freezes-when-qualitysettings-dot-maxqueuedframes-is-set-to-1-and-dx12-is-used))

- `6000.5.0a4`:剖析器（单机版）窗口无法打开
    ([uum-131071](https://issuetracker.unity3d.com/issues/profiler-standalone-window-doesnt-open))

- `IL2CPP`：[iOS] [Android] IL2CPP 编译过程中外部库泛型失败
    ([uum-125284](https://issuetracker.unity3d.com/issues/ios-android-external-library-generics-fail-during-il2cpp-build))

- iOS`：  启用 "显示闪屏 "并使用 Unity 作为库构建项目时，渲染冻结和 UnityGfxDeviceWorker 崩溃
    ([uum-130881](https://issuetracker.unity3d.com/issues/ios-rendering-freezes-and-unitygfxdeviceworker-crash-when-show-splash-screen-is-enabled-and-project-is-built-using-unity-as-a-library))

- 金属  命令缓冲区超时错误后游戏冻结
    ([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- 金属"： MacOS 在编辑器中的最小项目在播放模式下出现卡顿
    ([uum-85256](https://issuetracker.unity3d.com/issues/macos-stutters-in-a-minimal-project))

- `金属`：[iOS] iOS 闪屏后屏幕闪烁
    ([uum-121453](https://issuetracker.unity3d.com/issues/ios-screen-flashing-after-the-ios-splash-screen))

- 平台音频`：[Windows] 在编辑器中执行各种操作时，AudioManager::InitFMOD 会崩溃
    ([uum-126803](https://issuetracker.unity3d.com/issues/crash-on-audiomanager-initfmod-when-performing-various-actions-in-the-editor))

- : 在空白的 URP 项目中进入和退出播放模式时，编辑器内存泄漏
    ([uum-132677](https://issuetracker.unity3d.com/issues/editor-memory-leak-when-entering-and-exiting-play-mode-in-a-blank-urp-project))



# 6000.0.67f1 发行说明

## 改进

- 阴影图添加了一个问题，在该问题中，swizzle 节点的输入插槽可能最终处于不良状态。已更改行为，使节点的输入和输出插槽始终反映swizzle掩码。
    ([uum-120808](https://issuetracker.unity3d.com/issues/shader-graph-swizzle-node-input-slash-output-and-mask-update-incorrectly-after-undo))



## 修复

- `2D`:修正了用户在任意位置使用空画笔作画并在（0, 0, 0\ ）处清除瓷砖的问题。
    ([uum-128709](https://issuetracker.unity3d.com/issues/painting-on-a-tilemap-erases-random-tile-when-an-empty-tile-was-selected-in-the-tilemap-palette))

- `2D`:修正了磁贴调色板窗口的问题，即如果用户的指针在平移时离开了磁贴调色板窗口，则用户可以继续平移磁贴调色板窗口，并停用磁贴调色板窗口外的平移。
    ([uum-128466](https://issuetracker.unity3d.com/issues/tile-palette-grid-keeps-panning-when-the-mouse-click-is-released-outside-of-the-grid))

- 文档修正了指向创建剖析器模块页面的链接。

- 编辑器改进了对 `worldToGUIPoint` 和 `OnDrawGizmos` API 行为的描述。

- 图形修正了在解析 MSAA 无内存深度缓冲区时出现金属验证错误的崩溃问题。
    (UUM-125478)

- `uGUI`：修复了在 overrideSorting=true 时销毁画布而导致的 UI 元素屏蔽。
    ([UUM-127287](https://issuetracker.unity3d.com/issues/canvas-masking-is-not-updated-when-destroying-the-canvas-component-with-an-overridesorting))

- 版本控制修正了 2.11.2 中 WaitForPendingOperations.cs.meta 中因无效重复 GUID 而导致的编译错误。

- 版本控制修正了在 Unity 6.3 以下版本中直接访问编辑器内部的问题。




## 6000.0.67f1 中软件包的更改

## 更新的软件包

- com.unity.charactercontroller`：[1.4.1](https://docs.unity3d.com/Packages/com.unity.charactercontroller@1.4//changelog/CHANGELOG.html) 到 [1.4.2](https://docs.unity3d.com/Packages/com.unity.charactercontroller@1.4//changelog/CHANGELOG.html)

- `com.unity.animation.rigging`：[1.4.0](https://docs.unity3d.com/Packages/com.unity.animation.rigging@1.4//changelog/CHANGELOG.html) 到 [1.4.1](https://docs.unity3d.com/Packages/com.unity.animation.rigging@1.4//changelog/CHANGELOG.html)

- com.unity.collab-proxy`：[2.11.2](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.11//changelog/CHANGELOG.html) 到 [2.11.3](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.11//changelog/CHANGELOG.html)

- com.unity.ide.rider`：[3.0.38](https://docs.unity3d.com/Packages/com.unity.ide.rider@3.0//changelog/CHANGELOG.html) 到 [3.0.39](https://docs.unity3d.com/Packages/com.unity.ide.rider@3.0//changelog/CHANGELOG.html)

- com.unity.inputsystem`：[1.17.0](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.17//changelog/CHANGELOG.html) 到 [1.18.0](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.18//changelog/CHANGELOG.html)

- com.unity.mobile.android-logcat`：[1.4.6](https://docs.unity3d.com/Packages/com.unity.mobile.android-logcat@1.4//changelog/CHANGELOG.html) 到 [1.4.7](https://docs.unity3d.com/Packages/com.unity.mobile.android-logcat@1.4//changelog/CHANGELOG.html)

- com.unity.performance.profile-analyzer`：[1.2.3](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.2//changelog/CHANGELOG.html) 到 [1.3.1](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.3//changelog/CHANGELOG.html)

- com.unity.services.analytics`：[6.2.0](https://docs.unity3d.com/Packages/com.unity.services.analytics@6.2//changelog/CHANGELOG.html) 到 [6.2.1](https://docs.unity3d.com/Packages/com.unity.services.analytics@6.2//changelog/CHANGELOG.html)

- com.unity.testtools.codecoverage`：[1.2.6](https://docs.unity3d.com/Packages/com.unity.testtools.codecoverage@1.2//changelog/CHANGELOG.html) 到 [1.3.0](https://docs.unity3d.com/Packages/com.unity.testtools.codecoverage@1.3//changelog/CHANGELOG.html)

- com.unity.xr.hands`：[1.7.2](https://docs.unity3d.com/Packages/com.unity.xr.hands@1.7//changelog/CHANGELOG.html) 到 [1.7.3](https://docs.unity3d.com/Packages/com.unity.xr.hands@1.7//changelog/CHANGELOG.html)

- com.unity.profiling.systemmetrics.mali`：[1.1.0](https://docs.unity3d.com/Packages/com.unity.profiling.systemmetrics.mali@1.1//changelog/CHANGELOG.html) 到 [1.1.1](https://docs.unity3d.com/Packages/com.unity.profiling.systemmetrics.mali@1.1//changelog/CHANGELOG.html)

- com.unity.multiplayer.tools`：[2.2.6](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@2.2//changelog/CHANGELOG.html) 到 [2.2.7](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@2.2//changelog/CHANGELOG.html)

- com.unity.ai.navigation`：[2.0.9](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html) 到 [2.0.10](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html)