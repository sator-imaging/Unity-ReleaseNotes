# Unity 2022.3.72f1 LTS
Published at Wed, 11 Feb 2026 12:30:31 GMT  
https://unity.com/releases/editor/whats-new/2022.3.72f1

# Known Issues in 2022.3.72f1

- `Metal`: Game freezes after command buffer Timeout error
    ([UUM-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- `Metal`: macOS stutters in a minimal project in the Editor in Play Mode
    ([UUM-85256](https://issuetracker.unity3d.com/issues/macos-stutters-in-a-minimal-project))

- `Video`: Fix for 2022.3.X: VideoPlayer freezes or stops on certain Android devices when enabling and disabling the Video multiple times
    (UUM-112470)



# 2022.3.72f1 Release Notes

## Improvements

- `Adaptive Performance`: Upgraded Adaptive Performance from 4 to 5 to add 16KB support and more useful features and bug fixes from the 5.x line.
    (UUM-126684)



## Fixes

- `Android`: Fixed instability in Android test "ExportGradleProjectForApk_WithSplitBinary_CreatesOBBAndShowsWarning".
    (UUM-122699)

- `Editor`: Fixed an issue where custom property drawers would be DIsposed when they were still in use.
    ([UUM-132087](https://issuetracker.unity3d.com/issues/propertydrawer-gets-disposed-while-still-being-active-when-adding-a-secondary-component))

- `Graphics`: Fixed rare deadlock scenario in AsyncResourceUploadBlocking\(\) occasionally happening when loading resources \(typically Textures\) from AssetBundles.
    ([UUM-126066](https://issuetracker.unity3d.com/issues/android-the-application-freezes-during-the-assetbundle-loading))

- `iOS`: Fixed iOS 26 logs appearing as &lt;private&gt; in Console app.
    ([UUM-129367](https://issuetracker.unity3d.com/issues/ios-debug-dot-log-appears-as-in-console-app))

- `iOS`: Fixed on screen keyboard not reopening when using number pad or phone pad keyboard type.
    (UUM-132968)

- `Shadergraph`: Nodes are now properly selected after copy-paste or duplication.
    ([UUM-110841](https://issuetracker.unity3d.com/issues/nodes-in-shader-graph-are-not-selected-when-they-are-duplicated))

- `Version Control`: Fixed a compilation error caused by an invalid duplicated GUID in WaitForPendingOperations.cs.meta in 2.11.2.

- `Version Control`: Fixed accessing Editor internals directly on versions below Unity 6.3.

- `Version Control`: Fixed intermittent failures in Version Control native tests on linux.
    (UUM-130258)




## Package changes in 2022.3.72f1

## Packages updated

- `com.unity.adaptiveperformance`: [4.0.1](https://docs.unity3d.com/Packages/com.unity.adaptiveperformance@4.0//changelog/CHANGELOG.html) to [5.1.6](https://docs.unity3d.com/Packages/com.unity.adaptiveperformance@5.1//changelog/CHANGELOG.html)

- `com.unity.adaptiveperformance.samsung.android`: [4.0.2](https://docs.unity3d.com/Packages/com.unity.adaptiveperformance.samsung.android@4.0//changelog/CHANGELOG.html) to [5.1.0](https://docs.unity3d.com/Packages/com.unity.adaptiveperformance.samsung.android@5.1//changelog/CHANGELOG.html)

- `com.unity.addressables`: [1.28.1](https://docs.unity3d.com/Packages/com.unity.addressables@1.28//changelog/CHANGELOG.html) to [1.28.2](https://docs.unity3d.com/Packages/com.unity.addressables@1.28//changelog/CHANGELOG.html)

- `com.unity.burst`: [1.8.27](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html) to [1.8.28](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html)

- `com.unity.collab-proxy`: [2.11.2](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.11//changelog/CHANGELOG.html) to [2.11.3](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.11//changelog/CHANGELOG.html)

- `com.unity.ide.rider`: [3.0.38](https://docs.unity3d.com/Packages/com.unity.ide.rider@3.0//changelog/CHANGELOG.html) to [3.0.39](https://docs.unity3d.com/Packages/com.unity.ide.rider@3.0//changelog/CHANGELOG.html)

- `com.unity.inputsystem`: [1.17.0](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.17//changelog/CHANGELOG.html) to [1.18.0](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.18//changelog/CHANGELOG.html)

- `com.unity.mobile.android-logcat`: [1.4.6](https://docs.unity3d.com/Packages/com.unity.mobile.android-logcat@1.4//changelog/CHANGELOG.html) to [1.4.7](https://docs.unity3d.com/Packages/com.unity.mobile.android-logcat@1.4//changelog/CHANGELOG.html)

- `com.unity.mobile.notifications`: [2.4.2](https://docs.unity3d.com/Packages/com.unity.mobile.notifications@2.4//changelog/CHANGELOG.html) to [2.4.3](https://docs.unity3d.com/Packages/com.unity.mobile.notifications@2.4//changelog/CHANGELOG.html)

- `com.unity.performance.profile-analyzer`: [1.2.3](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.2//changelog/CHANGELOG.html) to [1.3.1](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.3//changelog/CHANGELOG.html)

- `com.unity.purchasing`: [4.14.0](https://docs.unity3d.com/Packages/com.unity.purchasing@4.14//changelog/CHANGELOG.html) to [4.14.2](https://docs.unity3d.com/Packages/com.unity.purchasing@4.14//changelog/CHANGELOG.html)

- `com.unity.scriptablebuildpipeline`: [1.23.2](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@1.23//changelog/CHANGELOG.html) to [1.23.3](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@1.23//changelog/CHANGELOG.html)

- `com.unity.services.analytics`: [6.2.0](https://docs.unity3d.com/Packages/com.unity.services.analytics@6.2//changelog/CHANGELOG.html) to [6.2.1](https://docs.unity3d.com/Packages/com.unity.services.analytics@6.2//changelog/CHANGELOG.html)

- `com.unity.xr.arcore`: [5.2.0](https://docs.unity3d.com/Packages/com.unity.xr.arcore@5.2//changelog/CHANGELOG.html) to [5.2.2](https://docs.unity3d.com/Packages/com.unity.xr.arcore@5.2//changelog/CHANGELOG.html)

- `com.unity.xr.arfoundation`: [5.2.0](https://docs.unity3d.com/Packages/com.unity.xr.arfoundation@5.2//changelog/CHANGELOG.html) to [5.2.2](https://docs.unity3d.com/Packages/com.unity.xr.arfoundation@5.2//changelog/CHANGELOG.html)

- `com.unity.xr.arkit`: [5.2.0](https://docs.unity3d.com/Packages/com.unity.xr.arkit@5.2//changelog/CHANGELOG.html) to [5.2.2](https://docs.unity3d.com/Packages/com.unity.xr.arkit@5.2//changelog/CHANGELOG.html)

- `com.unity.xr.hands`: [1.7.2](https://docs.unity3d.com/Packages/com.unity.xr.hands@1.7//changelog/CHANGELOG.html) to [1.7.3](https://docs.unity3d.com/Packages/com.unity.xr.hands@1.7//changelog/CHANGELOG.html)

- `com.unity.profiling.systemmetrics.mali`: [1.1.0](https://docs.unity3d.com/Packages/com.unity.profiling.systemmetrics.mali@1.1//changelog/CHANGELOG.html) to [1.1.1](https://docs.unity3d.com/Packages/com.unity.profiling.systemmetrics.mali@1.1//changelog/CHANGELOG.html)

- `com.unity.memoryprofiler`: [1.1.9](https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.1//changelog/CHANGELOG.html) to [1.1.10](https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.1//changelog/CHANGELOG.html)

- `com.unity.dt.app-ui`: [1.0.2](https://docs.unity3d.com/Packages/com.unity.dt.app-ui@1.0//changelog/CHANGELOG.html) to [1.3.5](https://docs.unity3d.com/Packages/com.unity.dt.app-ui@1.3//changelog/CHANGELOG.html)

- `com.unity.microsoft.gdk`: [1.4.4](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk@1.4//changelog/CHANGELOG.html) to [1.5.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk@1.5//changelog/CHANGELOG.html)

- `com.unity.microsoft.gdk.tools`: [1.4.4](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.tools@1.4//changelog/CHANGELOG.html) to [1.5.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.tools@1.5//changelog/CHANGELOG.html)

- `com.unity.microsoft.gdk.discovery`: [1.1.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.discovery@1.1//changelog/CHANGELOG.html) to [1.2.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.discovery@1.2//changelog/CHANGELOG.html)

- `com.unity.asset-manager-for-unity`: [1.9.0](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.9//changelog/CHANGELOG.html) to [1.9.1](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.9//changelog/CHANGELOG.html)