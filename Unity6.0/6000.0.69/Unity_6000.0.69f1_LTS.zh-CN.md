# Unity 6000.0.69f1 LTS
发布于 星期三, 04 三月 2026 09:50:56 GMT
https://unity.com/releases/editor/whats-new/6000.0.69f1

# 6000.0.69f1 中的已知问题

- `6000.1.0a2,6000.0.64f1`: 单通道立体声渲染在进入播放模式时只显示天空盒
    ([uum-132342](https://issuetracker.unity3d.com/issues/single-pass-stereo-rendering-shows-only-skybox-when-entering-play-mode))

- `6000.2.0a2,6000.0.38f1`: [安卓][IL2CPP][ARMv7]当调用具有大结构值的泛型委托时，结构字段值损坏
    ([uum-134192](https://issuetracker.unity3d.com/issues/android-il2cpp-armv7-struct-field-value-corrupts-when-invoking-a-generic-delegate-with-a-large-struct-by-value))

- `6000.3.0a4,6000.0.62f1`: 取消上一次输入后，选择同一输入字段时，输入字段不会更新
    ([uum-133712](https://issuetracker.unity3d.com/issues/input-field-does-not-update-when-selecting-the-same-input-field-after-previous-input-was-canceled))

- `6000.5.0a3,6000.4.0b8,6000.3.8f1,6000.0.68f1`: [iOS] 在 Info.plist 中添加 UIApplicationSceneManifest 时，应用程序运行时不会调用 Application.deepLinkActivated
    ([uum-135497](https://issuetracker.unity3d.com/issues/ios-application-dot-deeplinkactivated-does-not-get-invoked-while-app-is-running-when-uiapplicationscenemanifest-is-added-in-info-dot-plist))

- `IL2CPP`: [iOS] [Android] 在 IL2CPP 构建过程中外部库泛型失败
    ([uum-125284](https://issuetracker.unity3d.com/issues/ios-android-external-library-generics-fail-during-il2cpp-build))

- 金属命令缓冲区超时错误后游戏冻结
    ([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- `金属"`: MacOS 在编辑器中的最小项目在播放模式下出现卡顿
    ([uum-85256](https://issuetracker.unity3d.com/issues/macos-stutters-in-a-minimal-project))

- `Windows`: 启用 "在后台运行 "并切换活动窗口时，播放器会挂起
    ([uum-130495](https://issuetracker.unity3d.com/issues/player-hangs-when-the-run-in-background-is-enabled-and-active-window-is-switched))

在 DirectX 12 独占全屏模式下切换焦点时播放器崩溃
    ([uum-134743](https://issuetracker.unity3d.com/issues/player-crash-when-switching-focus-in-exclusive-fullscreen-mode-with-directx-12))

[硅] 当 Razer Synapse 应用程序打开项目时，os_unfair_recursive_lock_lock_with_options 会崩溃
    ([uum-135043](https://issuetracker.unity3d.com/issues/silicon-crash-on-os-unfair-recursive-lock-lock-with-options-when-opening-a-project-while-the-razer-synapse-app-is-open))



# 6000.0.69f1 发布说明

## 改进

- 安装程序删除了 Windows 系统上的 .NET 3.5 激活。大大缩短了直接使用安装程序的安装时间。
    (UUM-133360)



## 修复

- 安卓版修正了当自定义 Gradle 模板具有 `compileSdkVersion` 属性时，会显示 `GradleTemplateUpdater` 对话框的问题。
    ([uum-134142](https://issuetracker.unity3d.com/issues/android-gradle-compilesdkversion-is-incorrectly-deprecated-on-6-dot-0-6-dot-4))

- `Android`: 修正了一个问题，即在 Android \(Act\)上，当 TouchScreenKeyboard 更改文本选择时，UI Toolkit 输入字段中的圆点位置不会更新，该行为目前在 GameActivity 上仍被破坏。
    ([uum-128088](https://issuetracker.unity3d.com/issues/android-soft-keyboards-arrows-and-select-tools-do-not-have-visual-feedback-when-hide-mobile-input-is-enabled))

- `Android`: 修正了使用 Android `GameActivity`时，`OnApplicationQuit`不能被持续调用的问题。
    (UUM-131090)

- `安卓`: 更新了设备模拟器设备定义，以使用通用的、基于特征的名称，而不是旧设备的特定型号名称。
    (UUM-134051)

- `DX12`: 修复了使用 DXC 着色器编译器时的群集光照问题。
    (UUM-134785)

- `DX12`: 在最终升维过程中，使代理缓冲 srv 格式与 swapchain rtv 格式相匹配。
    ([UUM-134064](https://issuetracker.unity3d.com/issues/dx12-player-brightness-changes-when-changing-display-resolution-with-screen-dot-setresolution))

- 编辑器添加了 Hub 页面以链接 Hub 安装和 Hub 文档。

- 编辑器Burst SharedStatic 内存现在会在编辑器关闭前清除，这修复了如果在关闭期间安排作业可能发生的崩溃。
    ([uum-133804](https://issuetracker.unity3d.com/issues/crash-on-extracthandles-when-shutting-down-the-editor-in-a-specific-scene-while-burst-jobs-are-in-progress))

- 编辑器修正了一个 Bug，在播放模式下尝试打开 "渲染管道转换器 "窗口会导致打开一个不相关的窗口。
    ([uum-132083](https://issuetracker.unity3d.com/issues/the-sprite-importer-window-is-opened-instead-of-the-render-pipeline-converter-window-when-opening-it-in-play-mode))

- 编辑器修正了一个问题，即 EditorUtility.CompressTexture / EditorUtility.CompressCubemapTexture 会在压缩过程中太迟中断对签名 EAC 格式的压缩，导致纹理处于破碎状态。请注意，有符号的 EAC 格式不支持压缩，这一点已添加到 API 文档中。

- 编辑器修正了在 Ubuntu 上的软件包管理器中打开 "导出软件包 "对话框时可能导致窗口挂起或出现垃圾的问题。
    ([uum-131283](https://issuetracker.unity3d.com/issues/ubuntu-package-managers-export-package-window-is-rendered-with-artifacts-when-editor-is-running-on-opengl))

- 编辑器修正了一个问题，即脚本编译在 Windows 和 Linux 上产生不同的结果，从而导致跨多个平台工作的团队不必要地更改资产文件。
    (UUM-133554)

- 编辑器修正了 EditorUtility.CompressTexture / EditorUtility.CompressCubemapTexture 中的一个问题，即有可能尝试将 NPOT mipmapped 纹理压缩为不支持的目标格式。有关此问题的其他详细信息已添加到 API 文档中。
    ([uum-129605](https://issuetracker.unity3d.com/issues/corrupted-mipmaps-are-generated-when-using-editorutility-dot-compresstexture-with-npot-textures))

- 编辑器修正了在播放器设置中添加和删除脚本定义列表项时不必要的应用弹出窗口。
    ([uum-121033](https://issuetracker.unity3d.com/issues/do-you-want-to-apply-changes-warning-pop-up-appears-when-adding-and-removing-list-items-in-player-settings))

- `编辑器"`: 修正了当地图册对于编辑器字体过大时的 Debug.Assert 警告。
    ([uum-85059](https://issuetracker.unity3d.com/issues/assert-error-is-thrown-when-the-editor-language-is-set-to-one-of-the-experimental-ones-in-an-hdrp-project))

- `编辑器"`: 在具有可脚本渲染通道的项目中，当在构建配置文件之间切换时，编辑器中会出现有关瞬态附件的控制台错误。现已修复。
    ([uum-97475](https://issuetracker.unity3d.com/issues/gbuffer-slash-render-deferred-lighting-and-render-pass-related-errors-constantly-thrown-after-switching-a-build-profile))

- 图形相机预览 - 更改管道时，渲染目标纹理未重新创建，导致渲染纹理选项无效。
    ([uum-133293](https://issuetracker.unity3d.com/issues/after-converting-a-built-in-project-to-urp-render-texture-setting-error-message-is-spammed))

- `图形"`: 修正了一个问题，当使用金属时，模板附件被错误地取消设置，这会导致金属验证错误。
    (UUM-133783)

- `图形`: 修正了 `TexturesD3D11Base::SetTexture` 中的 DX11 崩溃问题。
    ([UUM-134071](https://issuetracker.unity3d.com/issues/crash-on-texturesd3d11base-settexture-when-using-directx11))

- `图形`: 修正了在 WebGPU 中清除多个渲染目标的问题。
    ([uum-133743](https://issuetracker.unity3d.com/issues/webgpu-urp-rendergraph-renderpass-doesnt-clear-textures))

- `IL2CPP`: 修正了在 Switch 平台上使用 WebRequests 与调试 c++ 配置时的崩溃问题。
    (UUM-127898)

- `IL2CPP`: 通过改进通用参数类型的内部哈希函数，减少了启动时间。
    (UUM-133424)

- 输入引入了输入系统的滚动三角洲行为总是被规范化的回归。现在已修复。
    (UUM-134566)

- 输入系统修正了同步原语的不正确使用，在主线程以外的线程发现输入设备的平台上，该原语可能导致 Unity 崩溃或未定义的行为。
    (UUM-134537)

- `macOS`: 修正了在场景加载过程中键盘输入被重置的问题。
    ([UUM-132112](https://issuetracker.unity3d.com/issues/keyboard-state-is-reset-when-automatically-loading-a-scene-via-script))

- `macOS`: 修正了在 macOS 上打开许多文件时网络请求失败的问题。
    (UUM-134087)

- 莫诺修正了增量 GC 标记和根注销注册之间的竞赛条件。
    (UUM-131742)

- `软件包管理器软件包管理器`: 软件包管理器：使用 upm 软件包的 Url 深层链接在可发现的情况下显示所选软件包。如果指定了版本或软件包无法被发现，也会显示添加弹出窗口。
    (PAK-8687)

- 物理修复了布料检查器绘画工具的一个问题，即由于没有向内部碰撞网格发射光线投射，因此无法显示画笔。
    ([uum-61756](https://issuetracker.unity3d.com/issues/paintable-area-is-offset-from-the-mesh-when-editing-cloth-constraints))

- 玩家修正了当视频播放器打开路径包含空格的文件时出现的 URL 解析问题。
    ([uum-125789](https://issuetracker.unity3d.com/issues/video-does-not-play-in-macos-build-when-built-app-is-placed-in-a-path-with-a-space-in-it-on-a-specific-project))

- `场景/游戏视图`: 修正了在场景视图中聚焦活动选区可能会编辑覆盖内容的问题。
    ([uum-134399](https://issuetracker.unity3d.com/issues/overlays-are-focused-when-using-the-frame-selected-in-window-under-cursor-shortcut-just-after-editing-overlay-fields))

- `阴影图`: 修正了在某些平台上编译内置渲染管道阴影图着色器时，"fixed "被重新定义的警告。
    (UUM-126357)

- `着色器`: 修正了在计算中写入 RWTexture2D 的问题。
    (UUM-127198)

- `TextMeshPro`: 改进了对缺少 "href "部分的不正确格式化 &lt;a&gt; 标签的处理。格式正确的标记应为 &lt;a href="link ID"&gt;要高亮显示的文本&lt;/a&gt;。
    ([uum-130554](https://issuetracker.unity3d.com/issues/indexoutofrangeexception-occurs-when-entering-tags-in-a-textmeshpro-ui-field))

- `uGUI`: 修正了因矩形变换边界过大而导致的崩溃。
    ([uum-132182](https://issuetracker.unity3d.com/issues/crash-on-raiseexception-when-creating-a-multiplayer-room-while-toggling-ui))

- `uGUI`: 修正了因矩形变换边界过大而导致崩溃的根本原因。添加了链接到受影响场景 GameObject\(s\) 的警告。
    (UUM-134019)

- 用户界面工具包修正了一个问题，即当集合排序时，不正确的索引被应用到 MultiColumnTreeView 和 MultiColumnListView 数据源路径。
    ([uum-133865](https://issuetracker.unity3d.com/issues/multicolumnlistview-does-not-visually-sort-the-column-when-bindingsourceselection-is-set-to-auto-assign))

- 用户界面工具包PanelSettings.renderMode 现在是公共 API。
    (UUM-119486)

- 撤消系统修正了在多选根 GameObjects 上撤消/重做替换变换类型时根 GameObjects 会改变层次顺序的问题。
    ([uum-133391](https://issuetracker.unity3d.com/issues/gameobjects-change-hierarchy-order-when-undoing-adding-component-to-multiple-gameobjectsgameobjects-change-hierarchy-order-when-undoing-adding-component-to-multiple-gameobjects))

- 网络修正了一个在处理触摸取消事件时出现的错误。
    ([uum-132183](https://issuetracker.unity3d.com/issues/mouse-postion-can-become-max-value-or-infinity-when-using-touch-input-with-legacy-input-module))

- `WebGL`: 修正了 AudioSource.SetScheduledEndTime 的一个 Bug，当调用 SetScheduledEndTime 时，音频源播放请求在启动时处于待处理状态。
    ([uum-117576](https://issuetracker.unity3d.com/issues/setscheduled-end-time-does-not-work-on-webgl))

- `WebGL`: \修正了由于 CoreCopy 着色器导致的 MSAA 纹理的 RenderGraph 错误。
    ([uum-133838](https://issuetracker.unity3d.com/issues/webgpu-errors-when-corecopy-shader-is-used-to-copy-an-msaa-texture))




## 6000.0.69f1 中软件包的更改

## 更新的软件包

- `com.unity.addressables`: [2.8.1](https://docs.unity3d.com/Packages/com.unity.addressables@2.8//changelog/CHANGELOG.html) 到 [2.9.1](https://docs.unity3d.com/Packages/com.unity.addressables@2.9//changelog/CHANGELOG.html)

- `com.unity.inputsystem`: [1.18.0](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.18//changelog/CHANGELOG.html) 到 [1.19.0](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.19//changelog/CHANGELOG.html)

- `com.unity.probuilder`: [6.0.8](https://docs.unity3d.com/Packages/com.unity.probuilder@6.0//changelog/CHANGELOG.html) 到 [6.0.9](https://docs.unity3d.com/Packages/com.unity.probuilder@6.0//changelog/CHANGELOG.html)

- `com.unity.recorder`: [5.1.4](https://docs.unity3d.com/Packages/com.unity.recorder@5.1//changelog/CHANGELOG.html) 到 [5.1.5](https://docs.unity3d.com/Packages/com.unity.recorder@5.1//changelog/CHANGELOG.html)

- `com.unity.scriptablebuildpipeline`: [2.5.2](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@2.5//changelog/CHANGELOG.html) 到 [2.6.1](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@2.6//changelog/CHANGELOG.html)

- `com.unity.services.wire`: [1.4.0](https://docs.unity3d.com/Packages/com.unity.services.wire@1.4//changelog/CHANGELOG.html) 到 [1.4.2](https://docs.unity3d.com/Packages/com.unity.services.wire@1.4//changelog/CHANGELOG.html)

- `com.unity.splines`: [2.8.2](https://docs.unity3d.com/Packages/com.unity.splines@2.8//changelog/CHANGELOG.html) 到 [2.8.3](https://docs.unity3d.com/Packages/com.unity.splines@2.8//changelog/CHANGELOG.html)

- `com.unity.xr.management`: [4.5.3](https://docs.unity3d.com/Packages/com.unity.xr.management@4.5//changelog/CHANGELOG.html) 到 [4.5.4](https://docs.unity3d.com/Packages/com.unity.xr.management@4.5//changelog/CHANGELOG.html)

- `com.unity.xr.oculus`: [4.5.2](https://docs.unity3d.com/Packages/com.unity.xr.oculus@4.5//changelog/CHANGELOG.html) 到 [4.5.4](https://docs.unity3d.com/Packages/com.unity.xr.oculus@4.5//changelog/CHANGELOG.html)

- `com.unity.terrain-tools`: [5.3.1](https://docs.unity3d.com/Packages/com.unity.terrain-tools@5.3//changelog/CHANGELOG.html) 到 [5.3.2](https://docs.unity3d.com/Packages/com.unity.terrain-tools@5.3//changelog/CHANGELOG.html)

- `com.unity.ai.navigation`: [2.0.10](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html) 到 [2.0.11](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html)

- `com.unity.addressables.android`: [1.0.9](https://docs.unity3d.com/Packages/com.unity.addressables.android@1.0//changelog/CHANGELOG.html) 到 [1.0.10](https://docs.unity3d.com/Packages/com.unity.addressables.android@1.0//changelog/CHANGELOG.html)

- `com.unity.microsoft.gdk`: [1.4.4](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk@1.4//changelog/CHANGELOG.html) 到 [1.5.1](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk@1.5//changelog/CHANGELOG.html)

- `com.unity.microsoft.gdk.tools`: [1.4.4](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.tools@1.4//changelog/CHANGELOG.html) 到 [1.5.1](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.tools@1.5//changelog/CHANGELOG.html)

- `com.unity.microsoft.gdk.discovery`: [1.1.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.discovery@1.1//changelog/CHANGELOG.html) 到 [1.2.1](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.discovery@1.2//changelog/CHANGELOG.html)