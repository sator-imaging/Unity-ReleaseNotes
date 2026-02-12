# Unity 2022.3.72f1 LTS
发布于 星期三, 11 二月 2026 12:30:31 GMT
https://unity.com/releases/editor/whats-new/2022.3.72f1

# 2022.3.72f1 中的已知问题

- 金属命令缓冲区超时错误后游戏冻结
    ([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- `金属"`: MacOS 在编辑器中的最小项目在播放模式下出现卡顿
    ([uum-85256](https://issuetracker.unity3d.com/issues/macos-stutters-in-a-minimal-project))

- `视频修正 2022.3.X`: 在某些 Android 设备上多次启用和禁用视频时，视频播放器会冻结或停止
    (UUM-112470)



# 2022.3.72f1 发行说明

## 改进

- 自适应性能将自适应性能从 4 升级到 5，增加了 16KB 支持和更多 5.x 版本的实用功能和错误修复。
    (UUM-126684)



## 修复

- `Android`: 修正了 Android 测试 "ExportGradleProjectForApk_WithSplitBinary_CreatesOBBAndShowsWarning" 中的不稳定性。
    (UUM-122699)

- 编辑器修正了自定义属性抽屉仍在使用时会被 DIsposed 的问题。
    ([UUM-132087](https://issuetracker.unity3d.com/issues/propertydrawer-gets-disposed-while-still-being-active-when-adding-a-secondary-component))

- `图形`: 修复了从 AssetBundles 加载资源（通常是纹理）时，AsyncResourceUploadBlocking\(\) 中偶尔出现的罕见死锁情况。
    ([uum-126066](https://issuetracker.unity3d.com/issues/android-the-application-freezes-during-the-assetbundle-loading))

- `iOS`: 修复了 iOS 26 日志在控制台应用程序中显示为&lt;private&gt;的问题。
    ([uum-129367](https://issuetracker.unity3d.com/issues/ios-debug-dot-log-appears-as-in-console-app))

- `iOS`: 修复了使用数字键盘或电话键盘类型时屏幕键盘无法重新打开的问题。
    (UUM-132968)

- 阴影图复制粘贴或复制后节点现在可以正确选择。
    ([UUM-110841](https://issuetracker.unity3d.com/issues/nodes-in-shader-graph-are-not-selected-when-they-are-duplicated))

- 版本控制修正了 2.11.2 中 WaitForPendingOperations.cs.meta 中因 GUID 无效重复而导致的编译错误。

- 版本控制修正了在 Unity 6.3 以下版本中直接访问编辑器内部的问题。

- 版本控制修正了版本控制原生测试在 linux 上的间歇性故障。
    (UUM-130258)




## 2022.3.72f1 中的软件包变更

## 更新的软件包

- `com.unity.adaptiveperformance`: [4.0.1](https://docs.unity3d.com/Packages/com.unity.adaptiveperformance@4.0//changelog/CHANGELOG.html) 到 [5.1.6](https://docs.unity3d.com/Packages/com.unity.adaptiveperformance@5.1//changelog/CHANGELOG.html)

- `com.unity.adaptiveperformance.samsung.android`: [4.0.2](https://docs.unity3d.com/Packages/com.unity.adaptiveperformance.samsung.android@4.0//changelog/CHANGELOG.html) 至 [5.1.0](https://docs.unity3d.com/Packages/com.unity.adaptiveperformance.samsung.android@5.1//changelog/CHANGELOG.html)

- `com.unity.addressables`: [1.28.1](https://docs.unity3d.com/Packages/com.unity.addressables@1.28//changelog/CHANGELOG.html) 到 [1.28.2](https://docs.unity3d.com/Packages/com.unity.addressables@1.28//changelog/CHANGELOG.html)

- `com.unity.burst`: [1.8.27](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html) 至 [1.8.28](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html)

- `com.unity.collab-proxy`: [2.11.2](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.11//changelog/CHANGELOG.html) 到 [2.11.3](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.11//changelog/CHANGELOG.html)

- `com.unity.ide.rider`: [3.0.38](https://docs.unity3d.com/Packages/com.unity.ide.rider@3.0//changelog/CHANGELOG.html) 到 [3.0.39](https://docs.unity3d.com/Packages/com.unity.ide.rider@3.0//changelog/CHANGELOG.html)

- `com.unity.inputsystem`: [1.17.0](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.17//changelog/CHANGELOG.html) 到 [1.18.0](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.18//changelog/CHANGELOG.html)

- `com.unity.mobile.android-logcat`: [1.4.6](https://docs.unity3d.com/Packages/com.unity.mobile.android-logcat@1.4//changelog/CHANGELOG.html) 到 [1.4.7](https://docs.unity3d.com/Packages/com.unity.mobile.android-logcat@1.4//changelog/CHANGELOG.html)

- `com.unity.mobile.notifications`: [2.4.2](https://docs.unity3d.com/Packages/com.unity.mobile.notifications@2.4//changelog/CHANGELOG.html) 到 [2.4.3](https://docs.unity3d.com/Packages/com.unity.mobile.notifications@2.4//changelog/CHANGELOG.html)

- `com.unity.performance.profile-analyzer`: [1.2.3](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.2//changelog/CHANGELOG.html) 到 [1.3.1](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.3//changelog/CHANGELOG.html)

- `com.unity.purchasing`: [4.14.0](https://docs.unity3d.com/Packages/com.unity.purchasing@4.14//changelog/CHANGELOG.html) 到 [4.14.2](https://docs.unity3d.com/Packages/com.unity.purchasing@4.14//changelog/CHANGELOG.html)

- `com.unity.scriptablebuildpipeline`: [1.23.2](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@1.23//changelog/CHANGELOG.html) 到 [1.23.3](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@1.23//changelog/CHANGELOG.html)

- `com.unity.services.analytics`: [6.2.0](https://docs.unity3d.com/Packages/com.unity.services.analytics@6.2//changelog/CHANGELOG.html) 到 [6.2.1](https://docs.unity3d.com/Packages/com.unity.services.analytics@6.2//changelog/CHANGELOG.html)

- `com.unity.xr.arcore`: [5.2.0](https://docs.unity3d.com/Packages/com.unity.xr.arcore@5.2//changelog/CHANGELOG.html) 到 [5.2.2](https://docs.unity3d.com/Packages/com.unity.xr.arcore@5.2//changelog/CHANGELOG.html)

- `com.unity.xr.arfoundation`: [5.2.0](https://docs.unity3d.com/Packages/com.unity.xr.arfoundation@5.2//changelog/CHANGELOG.html) 到 [5.2.2](https://docs.unity3d.com/Packages/com.unity.xr.arfoundation@5.2//changelog/CHANGELOG.html)

- `com.unity.xr.arkit`: [5.2.0](https://docs.unity3d.com/Packages/com.unity.xr.arkit@5.2//changelog/CHANGELOG.html) 到 [5.2.2](https://docs.unity3d.com/Packages/com.unity.xr.arkit@5.2//changelog/CHANGELOG.html)

- `com.unity.xr.hands`: [1.7.2](https://docs.unity3d.com/Packages/com.unity.xr.hands@1.7//changelog/CHANGELOG.html) 到 [1.7.3](https://docs.unity3d.com/Packages/com.unity.xr.hands@1.7//changelog/CHANGELOG.html)

- `com.unity.profiling.systemmetrics.mali`: [1.1.0](https://docs.unity3d.com/Packages/com.unity.profiling.systemmetrics.mali@1.1//changelog/CHANGELOG.html) 到 [1.1.1](https://docs.unity3d.com/Packages/com.unity.profiling.systemmetrics.mali@1.1//changelog/CHANGELOG.html)

- `com.unity.memoryprofiler`: [1.1.9](https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.1//changelog/CHANGELOG.html) 到 [1.1.10](https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.1//changelog/CHANGELOG.html)

- `com.unity.dt.app-ui`: [1.0.2](https://docs.unity3d.com/Packages/com.unity.dt.app-ui@1.0//changelog/CHANGELOG.html) 到 [1.3.5](https://docs.unity3d.com/Packages/com.unity.dt.app-ui@1.3//changelog/CHANGELOG.html)

- `com.unity.microsoft.gdk`: [1.4.4](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk@1.4//changelog/CHANGELOG.html) 到 [1.5.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk@1.5//changelog/CHANGELOG.html)

- `com.unity.microsoft.gdk.tools`: [1.4.4](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.tools@1.4//changelog/CHANGELOG.html) 到 [1.5.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.tools@1.5//changelog/CHANGELOG.html)

- `com.unity.microsoft.gdk.discovery`: [1.1.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.discovery@1.1//changelog/CHANGELOG.html) 到 [1.2.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.discovery@1.2//changelog/CHANGELOG.html)

- `com.unity.asset-manager-for-unity`: [1.9.0](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.9//changelog/CHANGELOG.html) 到 [1.9.1](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.9//changelog/CHANGELOG.html)