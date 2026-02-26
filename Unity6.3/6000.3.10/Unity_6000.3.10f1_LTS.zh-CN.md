# Unity 6000.3.10f1 LTS
发布于 星期三, 25 二月 2026 14:01:36 GMT
https://unity.com/releases/editor/whats-new/6000.3.10f1

# 6000.3.10f1 中的已知问题

- `6000.0.55f1,6000.3.0a4`: 在切换用户界面时创建多人房间时发生 RaiseException 时崩溃
    ([uum-132182](https://issuetracker.unity3d.com/issues/crash-on-raiseexception-when-creating-a-multiplayer-room-while-toggling-ui))

- `6000.0.66f1,6000.3.4f1,6000.4.0b4,6000.5.0a5`: 使用 Screen.SetResolution() 更改显示分辨率时，DX12 播放器亮度发生变化
    ([uum-134064](https://issuetracker.unity3d.com/issues/dx12-player-brightness-changes-when-changing-display-resolution-with-screen-dot-setresolution))

- `6000.1.0a2,6000.0.64f1`: 进入播放模式时，单通道立体渲染只显示天空盒
    ([uum-132342](https://issuetracker.unity3d.com/issues/single-pass-stereo-rendering-shows-only-skybox-when-entering-play-mode))

- `6000.2.0a10`: 首次打开项目时，TexturesD3D12::CreateTextureInternal()崩溃
    ([uum-135024](https://issuetracker.unity3d.com/issues/crash-on-checkdevicestatus-when-opening-a-project-for-the-first-time))

- `6000.2.0a7,6000.0.48f1`: [URP] 如果贴花渲染器技术设置为 "自动"，在编辑器中通过批处理模式构建或不渲染场景/游戏视图时，所有材质都渲染为黑色
    ([uum-134298](https://issuetracker.unity3d.com/issues/urp-all-materials-render-black-when-building-via-batchmode-or-without-rendering-scene-slash-game-view-in-editor-if-decal-renderer-technique-is-set-to-automatic))

- `6000.3.0a4,6000.0.62f1`: 取消上一次输入后，选择同一输入字段时，输入字段不会更新
    ([uum-133712](https://issuetracker.unity3d.com/issues/input-field-does-not-update-when-selecting-the-same-input-field-after-previous-input-was-canceled))

- `6000.3.5f1`: 在启用雕刻的情况下移动导航网格障碍物时 CPU 占用率增加
    ([uum-133911](https://issuetracker.unity3d.com/issues/increased-cpu-usage-when-moving-navmesh-obstacles-with-carving-enabled))

- `6000.3.7f1,6000.4.0b7`: 编辑预制件上的刚体组件设置时，PhysicsCommands::PhysX::BodySetPose 崩溃
    ([uum-135381](https://issuetracker.unity3d.com/issues/crash-on-physicscommands-physx-bodysetpose-when-editing-rigidbody-component-settings-on-a-prefab))

- `6000.5.0a7,6000.3.8f1,6000.4.0b9`: [Android][iOS] UI 工具包 ListView 触摸平移滚动不起作用
    ([uum-135398](https://issuetracker.unity3d.com/issues/android-ios-ui-toolkit-listview-touch-pan-scrolling-does-not-work))

- 核心运行时实体 ContentManagement GUID 不稳定，每次播放器构建到不同目录时都会变得不同
    ([uum-129944](https://issuetracker.unity3d.com/issues/entities-contentmanagement-guids-are-unstable-and-become-different-each-time-a-player-is-built-to-a-different-directory))

- `DirectX12`: 创建新的 "Get Started With Unity "项目时，D3D12DeviceState::ApplyRenderTargets崩溃
    ([uum-105801](https://issuetracker.unity3d.com/issues/crash-on-d3d12devicestate-applyrendertargets-when-creating-a-new-get-started-with-unity-project))

- `金属"`: 命令缓冲区超时错误后游戏冻结
    ([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- `金属"`: MacOS 在编辑器中的最小项目在播放模式下出现卡顿
    ([uum-85256](https://issuetracker.unity3d.com/issues/macos-stutters-in-a-minimal-project))

- `Windows`: 启用 "在后台运行 "并切换活动窗口时，播放器会挂起
    ([uum-130495](https://issuetracker.unity3d.com/issues/player-hangs-when-the-run-in-background-is-enabled-and-active-window-is-switched))

在空白 URP 项目中进入和退出播放模式时编辑器内存泄漏
    ([uum-132677](https://issuetracker.unity3d.com/issues/editor-memory-leak-when-entering-and-exiting-play-mode-in-a-blank-urp-project))

在 DirectX 12 独占全屏模式下切换焦点时播放器崩溃
    ([uum-134743](https://issuetracker.unity3d.com/issues/player-crash-when-switching-focus-in-exclusive-fullscreen-mode-with-directx-12))

[硅] 在打开 Razer Synapse 应用程序时打开项目时，os_unfair_recursive_lock_lock_with_options 崩溃
    ([uum-135043](https://issuetracker.unity3d.com/issues/silicon-crash-on-os-unfair-recursive-lock-lock-with-options-when-opening-a-project-while-the-razer-synapse-app-is-open))



# 6000.3.10f1 发布说明

## 应用程序接口变更

- `脚本新增`: 为 `Random` API 添加了 `onUnitCircle` 属性，该属性以 Vector2 的形式返回单位圆周上的随机点。
    (UUM-133714)



## 更改

- 编辑器添加了带有安装链接和 Hub 文档网站链接的 Unity Hub 页面。



## 修复

- 安卓版修正了当自定义 Gradle 模板具有 `compileSdkVersion` 属性时，会显示 `GradleTemplateUpdater` 对话框的问题。
    ([uum-134142](https://issuetracker.unity3d.com/issues/android-gradle-compilesdkversion-is-incorrectly-deprecated-on-6-dot-0-6-dot-4))

- 动画修正了在 AnimationWindow 中通过 AddCurves 创建的四元数关键帧的错误。
    ([uum-133953](https://issuetracker.unity3d.com/issues/assertion-failed-on-expression-compareapproximately-error-thrown-when-keyframes-are-added-for-rotation-animation))

- `编辑器"`: 为*着色器构建设置*下的字符串添加了截断功能。
    ([uum-133326](https://issuetracker.unity3d.com/issues/selected-keywords-string-under-shader-build-settings-is-cut-off-not-truncated-in-minimized-build-profiles-window))

- 编辑器处理着色速率 LUT 以避免帧调试器中的内存泄漏。
    (UUM-131230)

- 编辑器修正了在调试模式下使用检查器会在控制台中产生错误的错误。
    ([UUM-133467](https://issuetracker.unity3d.com/issues/selecting-multiple-visual-elements-in-the-hierarchy-with-enabled-debug-mode-results-in-malformed-inspector-window-with-thrown-notimplementedexception-and-unityeditor-dot-guiview-processevent-errors))

- 编辑器修正了在 Ubuntu 上打开软件包管理器中的导出软件包对话框可能导致窗口挂起或出现垃圾的问题。
    ([uum-131283](https://issuetracker.unity3d.com/issues/ubuntu-package-managers-export-package-window-is-rendered-with-artifacts-when-editor-is-running-on-opengl))

- 编辑器修正了在播放器设置中添加和删除脚本定义列表项时不必要的应用弹出窗口。
    ([uum-121033](https://issuetracker.unity3d.com/issues/do-you-want-to-apply-changes-warning-pop-up-appears-when-adding-and-removing-list-items-in-player-settings))

- `编辑器"`: 修正了 D3D12 设备过滤列表资产信息框中的过多空白。
    ([uum-123221](https://issuetracker.unity3d.com/issues/d3d12-device-filter-lists-asset-information-box-has-too-much-empty-space))

- `编辑器"`: 修正了LinuxEditor从其他应用程序切换时无法重新编译脚本的问题。
    ([uum-133944](https://issuetracker.unity3d.com/issues/linux-auto-refresh-fails-to-reimport-and-compile-script-changes-when-editing-files-outside-the-editor))

- 编辑器改进了构建配置文件窗口中加载旋转器图标的可见性。
    ([uum-132018](https://issuetracker.unity3d.com/issues/progress-indicator-in-meta-quest-build-profile-configuration-is-barely-visible))

- `编辑器`: 在具有可脚本呈现通道的项目中，在构建配置文件之间切换时，编辑器中会出现有关瞬态附件的控制台错误。现已修复。
    ([uum-97475](https://issuetracker.unity3d.com/issues/gbuffer-slash-render-deferred-lighting-and-render-pass-related-errors-constantly-thrown-after-switching-a-build-profile))

- `GI"`: 修正了 APV 工具提示中的小错字：Steaming &gt; Streaming.
    ([uum-134159](https://issuetracker.unity3d.com/issues/streaming-is-misspelled-as-steaming-in-enable-gpu-streaming-and-enable-disk-streaming-tooltpis))

- `图形`: 修正了 `TexturesD3D11Base::SetTexture` 中的 DX11 崩溃。
    ([uum-134071](https://issuetracker.unity3d.com/issues/crash-on-texturesd3d11base-settexture-when-using-directx11))

- `IL2CPP`: 修正了在 Switch 平台上使用 WebRequests 与调试 c++ 配置时的崩溃问题。
    (UUM-127898)

- `IL2CPP`: 通过改进通用参数类型的内部哈希函数，减少了启动时间。
    (UUM-133424)

- `macOS`: 修正了在场景加载过程中键盘输入被重置的问题。
    ([UUM-132112](https://issuetracker.unity3d.com/issues/keyboard-state-is-reset-when-automatically-loading-a-scene-via-script))

- `macOS`: 修正了在 macOS 上打开许多文件时网络请求失败的问题。
    (UUM-134087)

- 莫诺修正了增量 GC 标记和根注销注册之间的竞赛条件。
    (UUM-131742)

- 物理修复了在禁用对撞机上调用 Collider.GetGeometry&lt;T&gt;\(\) 时会发生的崩溃。
    ([UUM-134161](https://issuetracker.unity3d.com/issues/crash-on-physicscommands-physx-getshapegeometryholder-when-calling-a-method-on-a-disabled-object))

- 物理修正了物理关节组件小工具的一个问题，在关节连接到世界空间中的一个固定点的情况下，自动配置的连接锚会跟随关节。
    ([uum-134423](https://issuetracker.unity3d.com/issues/spring-joint-shows-only-one-anchor-gizmo-in-scene-view-when-auto-configure-connected-anchor-is-enabled))

- `物理 2D"`: 修复了编辑器中的一个问题，当暂停并单步时，使用插值模式的 "物理体 "将无法与任何变形写入保持同步，从而导致渲染器在视觉上不同步。
    (UUM-134580)

- 剖析器修复了多次点击导致配置文件捕获重复重新打开的问题。
    ([UUM-133429](https://issuetracker.unity3d.com/issues/profiler-capture-loading-process-is-deferred-until-the-final-click-is-released-when-selecting-a-capture-in-the-profiler-list-multiple-times-consecutively))

- 阴影图修正了在某些平台上编译内置渲染管道着色器时，"fixed "被重新定义的警告。
    (UUM-126357)

- `文本"`: 确保超长 ATG 文本正确渲染。
    ([UUM-133940](https://issuetracker.unity3d.com/issues/ui-toolkit-label-stops-rendering-text-in-a-custom-editor-window-when-using-advanced-text-generation))

- 用户界面工具包修正了生成器中选择的性能回归。
    (UUM-132445)

- 用户界面工具包修正了当集合排序时，不正确的索引被应用到 MultiColumnTreeView 和 MultiColumnListView 数据源路径的问题。
    ([uum-133865](https://issuetracker.unity3d.com/issues/multicolumnlistview-does-not-visually-sort-the-column-when-bindingsourceselection-is-set-to-auto-assign))

- Undo系统修正了在多选根 GameObjects 上撤消/重做替换变换类型时，根 GameObjects 会改变层次顺序的问题。
    ([uum-133391](https://issuetracker.unity3d.com/issues/gameobjects-change-hierarchy-order-when-undoing-adding-component-to-multiple-gameobjectsgameobjects-change-hierarchy-order-when-undoing-adding-component-to-multiple-gameobjects))

- `WebGL"`: 修正了 AudioSource.SetScheduledEndTime 的一个 Bug，当调用 SetScheduledEndTime 时，音频源播放请求在启动时处于待处理状态。
    ([uum-117576](https://issuetracker.unity3d.com/issues/setscheduled-end-time-does-not-work-on-webgl))




## 6000.3.10f1 中的软件包变更

## 更新的软件包

- `com.unity.addressables`: [2.8.1](https://docs.unity3d.com/Packages/com.unity.addressables@2.8//changelog/CHANGELOG.html) 到 [2.9.0](https://docs.unity3d.com/Packages/com.unity.addressables@2.9//changelog/CHANGELOG.html)

- `com.unity.probuilder`: [6.0.8](https://docs.unity3d.com/Packages/com.unity.probuilder@6.0//changelog/CHANGELOG.html) 到 [6.0.9](https://docs.unity3d.com/Packages/com.unity.probuilder@6.0//changelog/CHANGELOG.html)

- `com.unity.recorder`: [5.1.4](https://docs.unity3d.com/Packages/com.unity.recorder@5.1//changelog/CHANGELOG.html) 到 [5.1.5](https://docs.unity3d.com/Packages/com.unity.recorder@5.1//changelog/CHANGELOG.html)

- `com.unity.scriptablebuildpipeline`: [2.5.2](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@2.5//changelog/CHANGELOG.html) 到 [2.6.0](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@2.6//changelog/CHANGELOG.html)

- `com.unity.splines`: [2.8.2](https://docs.unity3d.com/Packages/com.unity.splines@2.8//changelog/CHANGELOG.html) 到 [2.8.3](https://docs.unity3d.com/Packages/com.unity.splines@2.8//changelog/CHANGELOG.html)

- `com.unity.xr.arcore`: [6.3.2](https://docs.unity3d.com/Packages/com.unity.xr.arcore@6.3//changelog/CHANGELOG.html) 至 [6.3.3](https://docs.unity3d.com/Packages/com.unity.xr.arcore@6.3//changelog/CHANGELOG.html)

- `com.unity.xr.arfoundation`: [6.3.2](https://docs.unity3d.com/Packages/com.unity.xr.arfoundation@6.3//changelog/CHANGELOG.html) 至 [6.3.3](https://docs.unity3d.com/Packages/com.unity.xr.arfoundation@6.3//changelog/CHANGELOG.html)

- `com.unity.xr.arkit`: [6.3.2](https://docs.unity3d.com/Packages/com.unity.xr.arkit@6.3//changelog/CHANGELOG.html) 到 [6.3.3](https://docs.unity3d.com/Packages/com.unity.xr.arkit@6.3//changelog/CHANGELOG.html)

- `com.unity.xr.management`: [4.5.3](https://docs.unity3d.com/Packages/com.unity.xr.management@4.5//changelog/CHANGELOG.html) 到 [4.5.4](https://docs.unity3d.com/Packages/com.unity.xr.management@4.5//changelog/CHANGELOG.html)

- `com.unity.microsoft.gdk`: [1.4.5](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk@1.4//changelog/CHANGELOG.html) 到 [1.5.1](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk@1.5//changelog/CHANGELOG.html)

- `com.unity.microsoft.gdk.tools`: [1.4.5](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.tools@1.4//changelog/CHANGELOG.html) 到 [1.5.1](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.tools@1.5//changelog/CHANGELOG.html)

- `com.unity.microsoft.gdk.discovery`: [1.1.1](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.discovery@1.1//changelog/CHANGELOG.html) 到 [1.2.1](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.discovery@1.2//changelog/CHANGELOG.html)

- `com.unity.services.multiplayer`: [2.1.1](https://docs.unity3d.com/Packages/com.unity.services.multiplayer@2.1//changelog/CHANGELOG.html) 到 [2.1.2](https://docs.unity3d.com/Packages/com.unity.services.multiplayer@2.1//changelog/CHANGELOG.html)