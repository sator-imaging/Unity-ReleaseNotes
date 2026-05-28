# Unity 6000.0.76f1 LTS
发布于北京时间 2026 年 5 月 27 日星期三 09:43:20
https://unity.com/releases/editor/whats-new/6000.0.76f1

# 6000.0.76f1 中的已知问题

- `6000.0.61f1`: 使用SDF16或SDF32生成字体图集时，tlsf_free崩溃
    ([uum-141061](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-generating-font-atlas-with-sdf16-or-sdf32))

- `6000.0.6f1`: [渲染图][D3D12]当使用带有EnableAsyncCompute(true)和UseTexture的AddComputePass时，D3D12SwapChain::Present崩溃。
    ([uum-140183](https://issuetracker.unity3d.com/issues/rendergraph-d3d12-crash-on-d3d12swapchain-present-when-using-addcomputepass-with-enableasynccompute-true-and-usetexture))

- `6000.2.0a8`: 脚本域拆卸后执行异步 HTTP 回调时，在 Scripting::LogException 上崩溃
    ([uum-141434](https://issuetracker.unity3d.com/issues/crash-on-scripting-logexception-when-async-http-callback-executes-after-scripting-domain-teardown))

- `Asset Importers`: 进入播放模式时，编辑器在"(Unity) WriteObjectToVector "时崩溃
    ([uum-112617](https://issuetracker.unity3d.com/issues/editor-crashes-on-unity-writeobjecttovector-when-entering-into-the-play-mode))

- `金属"`: 命令缓冲区超时错误后游戏冻结
    ([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- 文本 (TextMeshPro)：在 TMPro Font Asset Creator 中生成多线程字体图集时，在 UNITY_FT_Load_Glyph 上崩溃
    ([uum-125366](https://issuetracker.unity3d.com/issues/crash-on-unity-ft-load-glyph-when-generating-multi-threaded-font-atlas-in-tmpro-font-asset-creator))

当运行一个以上的bee_backend副本时，mono_log_write_logfile崩溃
    ([uum-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))



# 6000.0.76f1 发行说明

## 改进

- `图形在 GfxDeviceGLES`: DrawBuffersBatchMode 中添加了对空索引缓冲的保护。
    (UUM-135891)



## 更改

- `Android`: 更新 JDK 至 17.0.18+8。
    (UUM-141159)



## 修复

- `2D`: 修复了一个问题，即当用户为磁贴调色板拖放精灵资产但取消创建磁贴资产的操作时，磁贴调色板会显示一个空网格。
    ([uum-132388](https://issuetracker.unity3d.com/issues/tile-palette-texture-drag-area-label-drag-tile-sprite-or-texture-sprite-type-asset-slash-s-here-dot-disappears-when-the-asset-save-pop-up-is-closed-slash-canceled))

- `Android`: 添加了 RunInBackground 测试，以涵盖全屏用例。

- `Android`: AndroidApplication.onConfigurationChanged 将正确反映 GameActivity 上的语言/国家变更。

- `Android`: EnhancedTouch.Touch.activeTouches.Count 将在释放轻扫/返回手势后正确减少（GameActivity 4.4.1 升级的一部分）。
    ([uum-128219](https://issuetracker.unity3d.com/issues/android-enhancedtouch-dot-touch-dot-activetouches-dot-count-does-not-decrease-after-releasing-the-swipe-slash-go-back-gesture))

- `Android`: 固定光标锁定时的鼠标输入（GameActivity 4.4.2升级版的一部分）。
    (UUM-91677)

- `Android`: 修复了在Unity作为库（UAAL\ ）场景中的Application.Unload或Reload期间发送UnitySendMessage调用时在Android上掉线的问题。
    (UUM-141440)

- `Android`: 修正了 SamsungA53 上的 ValidateAndroidEscapeButton 测试。
    (UUM-96035)

- `Android`: 将 "无焦点运行 "切换为启用，现在可以确保在启动其他活动时继续运行Unity活动，包括从Unity启动的Android活动。
    ([UUM-120304](https://issuetracker.unity3d.com/issues/android-unityplayer-gets-paused-when-another-activity-is-launched-even-with-run-without-focus-enabled))

- `Android`: 将 GameActivity 库从 3.0.5 更新至 4.4.2。注：4.4.0 版本仅兼容 Android 7 及以上版本，4.4.2 版本应用了修复程序，使 GameActivity 再次兼容 Android 6。

- 安卓滑动触摸屏键盘时，输入框中不会出现乱码（GameActivity 4.4.2 升级版的一部分）。
    ([uum-116283](https://issuetracker.unity3d.com/issues/android-ui-toolkit-gameactivity-swipe-typed-word-overrides-a-last-entry-with-an-inputfield-with-a-large-amount-of-characters))

- 动画修正了在动画窗口中选择短循环动画过渡时的 ArgumentOutOfRangeException。
    ([uum-139812](https://issuetracker.unity3d.com/issues/argumentoutofrangeexception-is-thrown-when-selecting-a-transition-to-an-animation-shorter-than-3-frames-with-loop-time-enabled))

- `构建管道"`: 新增了使用 BootConfig 关键字 "remapper-initial-capacity "为 PersistentManager.Remapper 预留容量的支持，该关键字指定了初始 hashmap 大小。
    (UUM-136275)

- `构建管道构建管道`: 在 Rider IDE 中运行时，确保源代码生成器不在运行。
    (UUM-133605)

- `构建管道`: 修正 ILPP.Trigger 等待逻辑，以防止 unity 日志中出现 "管道正在关闭 "异常。
    (UUM-136791)

- `构建系统`: 修正了使用特定构建路径时，在构建过程中出现节点 GUID 重复错误的问题。
    ([UUM-128491](https://issuetracker.unity3d.com/issues/build-fails-with-duplicate-node-guids-error-when-using-specific-build-path))

- `文档`: 修正了手柄脚本 API 文档链接中的拼写错误。

- `文档`: 修正了二维对撞机参考页面中的 Vale 错误。

- 编辑器添加了一个名为 "enableHeightmapLODFrustumCulling "的选项，该选项可在调试模式下的地形检查器设置中使用，以选择退出基于地形挫折的 LOD 裁剪。
    (UUM-141589)

- 编辑器尽管指定了远程构建，但本地无效架构的 "构建和运行 "按钮显示为灰色（Device Portal）。
    ([UUM-138399](https://issuetracker.unity3d.com/issues/build-and-run-button-greyed-out-for-locally-invalid-architecture-despite-remote-build-is-specified))

- 编辑器修正了一个错误，即在 macOS 上使用 -projectPath 命令行参数启动编辑器时，Unity Hub 会打开。
    ([uum-136928](https://issuetracker.unity3d.com/issues/unity-hub-opens-when-launching-the-editor-with-projectpath-argument))

- 编辑器修正了因文件损坏或外部文件锁定而无法打开 curl 文件缓存数据库时的启动崩溃问题。现在，编辑器会尝试删除并重新创建缓存数据库，如果磁盘文件仍然不可用，则会退回到内存缓存。
    ([uum-140399](https://issuetracker.unity3d.com/issues/crash-on-getdatabase-when-sqlite-database-for-the-curl-file-cache-fails-to-open-or-create))

- 编辑器修正了当对撞机中心重叠时，调用盒状对撞机和凸状网格对撞机的 computePenetration 时发生的崩溃。
    ([uum-100359](https://issuetracker.unity3d.com/issues/meshcollider-does-not-detect-collisions-with-capsules-and-charactercontroller-when-using-physics-dot-computepenetration))

- 编辑器修正了在固定时间步数字段中输入 Inf 或 NaN 时出现的 "无效双参数 "错误。
    ([uum-138227](https://issuetracker.unity3d.com/issues/argumentexception-invalid-double-parameter-dot-error-is-thrown-when-infinity-is-typed-into-the-fixed-timestep-field))

- 编辑器修正了在检查器数组（如 "玩家设置&gt;预载资产"）的 "大小 "字段中输入一个非常大的值（例如 24124124）时编辑器冻结的问题。
    ([uum-139781](https://issuetracker.unity3d.com/issues/the-editor-freezes-indefinitely-when-entering-24124124-into-the-preloaded-assets-size))

- 编辑器修正了一个问题，即当纹理设置为以 Cubemap 或无 mipmap 的形式导入时，无法与纹理导入器的 "Aniso 级别 "滑块进行交互，即使所选级别对这些纹理有影响。
    ([uum-138249](https://issuetracker.unity3d.com/issues/aniso-level-still-applies-when-generate-mipmap-is-disabled-in-texture-import-settings))

- 编辑器当使用 UI Toolkit \(default/)检查器模式时，修正了在检查器中还原 Prefab Variant 的属性覆盖后未调用 OnValidate 的问题。以前，拨动和下拉等非文本字段会错误地阻止 Prefab 资产在还原后自动保存，从而阻止 OnValidate，直到用户点击其他地方从字段移除焦点。
    ([uum-134476](https://issuetracker.unity3d.com/issues/the-onvalidate-method-is-not-invoked-when-reverting-changes-on-a-prefab-variant))

- 编辑器修正了更改色彩空间设置时项目窗口路径中断的问题。
    ([uum-139519](https://issuetracker.unity3d.com/issues/project-window-path-display-breaks-visually-when-player-settings-color-space-is-changed))

- 编辑器提高了 CapsuleCollider 和凸网格对撞器之间的 ComputePenetration 调用的可靠性。当距离为零时，ComputePenetration 将返回 true。
    ([uum-100359](https://issuetracker.unity3d.com/issues/meshcollider-does-not-detect-collisions-with-capsules-and-charactercontroller-when-using-physics-dot-computepenetration))

- 编辑器提高了 CharacterController 与凸网格对撞器之间调用 ComputePenetration 的可靠性。当距离为零时，ComputePenetration 将返回 true。
    ([uum-100359](https://issuetracker.unity3d.com/issues/meshcollider-does-not-detect-collisions-with-capsules-and-charactercontroller-when-using-physics-dot-computepenetration))

- `引擎诊断`: 修正了一个问题，在关闭过程中，由于异步崩溃报告管道在播放器循环停止后无法完成，导致重复管理的异常计数丢失。
    ([uum-141101](https://issuetracker.unity3d.com/issues/combined-log-and-throw-exceptions-function-does-not-show-up-in-diagnostics-cloud-dashboard-when-called-in-player))

- `引擎诊断`: 修正了因 JNI 本地方法过早注销注册而导致的崩溃，该崩溃导致在 nativeOnAndroidAppSetIdResult 上出现 java.lang.UnsatisfiedLinkError 错误。
    (UUM-137662)

- 图形修正了 GPU 驻留抽屉在 GPU 遮挡剔除过程中错误地将四边形拓扑网格渲染为三角形的问题。
    ([UUM-132444](https://issuetracker.unity3d.com/issues/automatic-lod-fails-and-gpu-occlusion-culling-incompatibility-occurs-when-using-spline-based-quad-topology-meshes))

- `图形"`: 当启用 V-Sync 时，修正了 Windows 上 Vulkan 帧时间卡顿问题。
    (UUM-140217)

- `IL2CPP`: 修正了秩超过 18 的多维数组的 IL2CPP 代码生成问题。
    ([UUM-138552](https://issuetracker.unity3d.com/issues/build-fails-when-building-a-project-containing-an-18-plus-dimension-array-with-il2cpp))

- `iOS`: 如果 il2cpp 命令构建 GameAssembly 失败，确保 Xcode 项目构建失败。
    (UUM-141609)

- 物理修正了一个问题，启用投影模式的 ConfigurableJoint 可能会由于其连接的体从运动模式变成动态模式而导致崩溃。
    ([UUM-135394](https://issuetracker.unity3d.com/issues/crash-on-constraintprojectiontree-projectiontreebuildstep-when-configurablejoint-uses-jointprojectionmode-dot-positionandrotation-and-connected-rigidbody-switches-from-kinematic-to-non-kinematic))

- 物理修正了网格对撞机组件接收非均匀缩放时处理不当的问题。
    ([uum-139681](https://issuetracker.unity3d.com/issues/mesh-collider-does-not-skew-slash-shear-correctly-when-nested-inside-another-gameobject))

- 着色器修正了着色器检查器对无属性的着色器显示空 "属性 "折叠的问题。
    ([uum-127146](https://issuetracker.unity3d.com/issues/planeocclusionshader-properties-foldout-does-not-display-any-content))

- `uGUI`: 修正了当禁用 "允许富文本编辑 "时，在 TMP 输入字段开始处向左移动游标时抛出的 "IndexOutOfRangeException"。
    ([uum-134157](https://issuetracker.unity3d.com/issues/indexoutofrangeexception-thrown-when-moving-caret-left-at-start-of-tmp-input-field-with-rich-text))

- 用户界面元素优化了导致某些 UIToolkit<br><br>.
    .Bindings.PerformanceTests 回归。
    (UUM-139531)

- `URP`: 修复了添加或删除可脚本渲染器功能时，项目窗口不会刷新更改的问题。
    ([UUM-139513](https://issuetracker.unity3d.com/issues/urp-asset-sub-assets-show-changes-in-sub-assets-only-after-reimporting-the-urp-asset-manually))

- `网络`: 修正了游戏手柄 API 在多线程网络构建中无法工作的问题。
    ([uum-136543](https://issuetracker.unity3d.com/issues/gamepad-input-does-not-work-in-a-web-build-when-native-c-slash-c-plus-plus-multithreading-is-enabled))




## 6000.0.76f1 中软件包的更改

## 更新的软件包

- `com.unity.collections`: [2.6.5](https://docs.unity3d.com/Packages/com.unity.collections@2.6//changelog/CHANGELOG.html) 到 [2.6.6](https://docs.unity3d.com/Packages/com.unity.collections@2.6//changelog/CHANGELOG.html)

- `com.unity.entities`: [1.4.5](https://docs.unity3d.com/Packages/com.unity.entities@1.4//changelog/CHANGELOG.html) 至 [1.4.6](https://docs.unity3d.com/Packages/com.unity.entities@1.4//changelog/CHANGELOG.html)

- `com.unity.physics`: [1.4.5](https://docs.unity3d.com/Packages/com.unity.physics@1.4//changelog/CHANGELOG.html) 至 [1.4.6](https://docs.unity3d.com/Packages/com.unity.physics@1.4//changelog/CHANGELOG.html)

- `com.unity.entities.graphics`: [1.4.18](https://docs.unity3d.com/Packages/com.unity.entities.graphics@1.4//changelog/CHANGELOG.html) 到 [1.4.19](https://docs.unity3d.com/Packages/com.unity.entities.graphics@1.4//changelog/CHANGELOG.html)