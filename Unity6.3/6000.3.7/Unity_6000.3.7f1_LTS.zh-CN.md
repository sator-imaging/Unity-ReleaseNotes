# Unity 6000.3.7f1 LTS
发布于 Thu, 05 Feb 2026 07:53:48 GMT
https://unity.com/releases/editor/whats-new/6000.3.7f1

# 6000.3.7f1 中的已知问题

- `6000.0.55f1,6000.3.0a4`: 在切换用户界面时创建多人房间时发生 RaiseException 时崩溃
    ([uum-132182](https://issuetracker.unity3d.com/issues/crash-on-raiseexception-when-creating-a-multiplayer-room-while-toggling-ui))

- `6000.1.0a2,6000.0.64f1`: 进入游戏模式时，单通道立体渲染只显示天空盒
    ([uum-132342](https://issuetracker.unity3d.com/issues/single-pass-stereo-rendering-shows-only-skybox-when-entering-play-mode))

- `6000.3.0a1`: [WinEditor]当搜索本地对话框时，编辑器在焦点丢失后 "冻结
    ([uum-132303](https://issuetracker.unity3d.com/issues/the-editor-freezes-and-leaks-memory-when-cancelling-the-switch-of-the-default-render-pipeline-while-using-the-advanced-object-selector))

- `6000.3.0b1,6000.0.65f1`: 当质量设置（QualitySettings.maxQueuedFrames）设为 1 并使用 DX12 时，编辑器会冻结
    ([uum-131962](https://issuetracker.unity3d.com/issues/editor-freezes-when-qualitysettings-dot-maxqueuedframes-is-set-to-1-and-dx12-is-used))

- `6000.5.0a1,6000.3.2f1`: 在特定场景的场景视图中移动时，CheckDeviceStatus崩溃
    ([uum-131824](https://issuetracker.unity3d.com/issues/crash-on-checkdevicestatus-when-moving-in-the-scene-view-on-a-specific-scene))

- `6000.5.0a1,6000.3.2f1`: 使用 DX12 并选择所有样条线节时，出现多个堆栈跟踪的崩溃现象
    ([uum-131707](https://issuetracker.unity3d.com/issues/crash-with-multiple-stack-traces-when-using-dx12-and-selecting-all-spline-knots))

- `6000.5.0a3,6000.4.0b2`: 在 "剖面分析器 "比较工具中加载两个剖面捕获时，崩溃率为 100
    ([uum-132332](https://issuetracker.unity3d.com/issues/100-percent-crash-rate-when-loading-two-profiler-captures-in-the-profile-analyzer-compare-tool))

- `金属"`: 命令缓冲区超时错误后游戏冻结
    ([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- `金属`: [iOS]iOS闪屏后屏幕闪烁
    ([uum-121453](https://issuetracker.unity3d.com/issues/ios-screen-flashing-after-the-ios-splash-screen))

- `平台音频`: [Windows] 在编辑器中执行各种操作时，AudioManager::InitFMOD 会崩溃
    ([uum-126803](https://issuetracker.unity3d.com/issues/crash-on-audiomanager-initfmod-when-performing-various-actions-in-the-editor))

- : 在打开安装了特定插件的场景时，出现多个堆栈跟踪时崩溃
    ([uum-133643](https://issuetracker.unity3d.com/issues/crash-with-multiple-stack-traces-when-opening-scenes-with-a-certain-plugin-installed))

- : 在空白 URP 项目中进入和退出播放模式时，编辑器内存泄漏
    ([uum-132677](https://issuetracker.unity3d.com/issues/editor-memory-leak-when-entering-and-exiting-play-mode-in-a-blank-urp-project))



# 6000.3.7f1 发行说明

## 更改

- `uGUI`: 将 uGUI 的 profiler 模块 （UI 和 UI Details）重命名为 "UI （Canvas）" 和 "UI Details （Canvas）"。
    (UUM-132153)



## 修复

- `2D`: 修正了当 SpriteRenderer 的序列化属性发生变化且 MaterialPropertyBlock 恰好设置了两个属性时，SpriteRenderer 的 MaterialPropertyBlock 会被重置的问题。
    ([uum-127937](https://issuetracker.unity3d.com/issues/materialpropertyblock-of-a-spriterenderer-is-reset-when-it-is-updated-through-the-color-picker))

- `Android`: 修正了调用 Application.Unload 时基于 GameActivity 的应用程序未被后台化的问题。
    (UUM-129424)

- `动画修正曲线菜单无法在 DopeSheet 编辑器中应用切线变化的问题。
    ([UUM-132540](https`: //issuetracker.unity3d.com/issues/animation-keyframes-are-always-set-to-clamped-auto-when-another-option-is-selected))

- `资产管道`: 修正了保存场景时，OnWillSaveAssets 可能返回资产路径空列表的问题。
    ([uum-115091](https://issuetracker.unity3d.com/issues/onwillsaveassets-receives-an-empty-paths-array-when-saving-a-new-scene))

- `文档`: 修复了指向 "创建剖析器模块 "页面的链接。

- `DX12`: 启用 UWP 构建的渲染传递路径。修正了当渲染通行证功能不可用时可能错误设置某些通行证视口的问题。
    ([uum-89085](https://issuetracker.unity3d.com/issues/d3d12-mainlight-shadowmap-clear-incorrectly-when-using-uwp))

- `DX12`: 修正了使用 cpu 端时间采样时损坏的 `IDXGISwapChain::GetFrameStatistics` 问题。
    (UUM-107892)

- `编辑器为导航和寻路请求的所有内存分配添加了根标签（com.unity.module.ai\）。
    (UUM-126905)

- 编辑器在 Linux 编辑器中添加了保障措施，以减少项目加载过程中可能出现的崩溃。
    ([UUM-132175](https`: //issuetracker.unity3d.com/issues/linux-crash-on-editorlaunchscreen-platformeditorlaunchscreen-setprogress-when-opening-a-project))

- `编辑器在 UnityCrashHandler 可执行文件中添加了版本信息。
    (UUM-132574)

- 编辑器修复了保存布局时意外抛出警告的错误。
    ([UUM-131954](https`: //issuetracker.unity3d.com/issues/a-cannot-save-invalid-window-create-layout-warning-is-thrown-when-any-custom-layout-is-created))

- `编辑器修正了一个性能回归问题，该问题是由于在构建时未剥离 Meta 传递。
    (UUM-116130)

- 编辑器修正了从搜索窗口添加列的问题。
    ([UUM-132150](https`: //issuetracker.unity3d.com/issues/add-column-dot-dot-dot-button-does-not-work-in-the-search-window))

- `编辑器"`: 修正了崩溃报告符号上传验证，使用 TryLogin\(\) 和直接访问令牌验证，而不是不可靠的 LoggedIn\(\) 状态检查。
    (ULO-8719)

- `编辑器修复了在 URP 中编辑反射探针边界时，无法使用句柄独立编辑对边的问题。
    ([uum-132551](https`: //issuetracker.unity3d.com/issues/two-opposite-sides-of-the-reflection-probe-boundaries-are-moved-when-trying-to-move-only-one-side))

- `编辑器"`: 修复了加载/卸载资产包取消纹理流请求时的挂起问题。
    ([uum-116419](https://issuetracker.unity3d.com/issues/editor-and-android-player-hangs-slash-freezes-when-repeatedly-loading-slash-unloading-assetbundle-in-vulkan))

- `编辑器"`: 修正了复选框位置不一致的问题。
    (UUM-132515)

- `编辑器"`: 修正了 uGUI 游戏对象创建时菜单顺序不正确导致自动重命名失败的问题。
    ([UUM-132217](https://issuetracker.unity3d.com/issues/legacy-ui-elements-are-not-entering-auto-renaming-on-creation))

- `编辑器"`: 修正了内置场景的标签。
    ([uum-125472](https://issuetracker.unity3d.com/issues/default-scene-dropdown-field-contains-a-spelling-mistake-default-builtin))

- `编辑器"`: 修正了 "图形设置 "部分下拉框和复选框的错位。
    ([uum-126644](https://issuetracker.unity3d.com/issues/misaligned-dropdowns-and-checkboxes-in-graphics-settings-section))

- `编辑器"`: 修正了 shadergraph uGUI 样本的命名，使其遵循新的菜单名称。
    (UUM-132809)

- `编辑器修正了 AssetDatabaseScalability 的性能回归问题。
    (UUM-132351)

- 编辑器修复了使用 Light Editor 主题时项目选项卡几乎不可见的问题。
    ([UUM-132553](https`: //issuetracker.unity3d.com/issues/plus-button-below-project-tab-is-barely-visible-when-using-light-editor-theme))

- `编辑器"`: 更改变换类型时，根变换移到层次结构末尾的问题。
    ([uum-132190](https://issuetracker.unity3d.com/issues/gameobject-drops-to-the-last-position-in-the-hierarchy-when-a-recttransform-component-is-added))

- `编辑器"`: 修正主工具栏滑块的上下文菜单显示多个分隔符的问题。
    ([uum-131672](https://issuetracker.unity3d.com/issues/an-extra-separator-is-added-to-main-toolbar-context-menu-when-extending-maintoolbarelement-with-populatecontextmenu))

- `编辑器"`: 修正了下划线缠绕的问题。
    ([uum-132463](https://issuetracker.unity3d.com/issues/underline-vertex-left-position-is-greater-than-right-position-errors-when-enabling-advanced-text-generator-auto-size-and-resizing-the-ui-builder-panels))

- `编辑器"`: 修正了换行时的下划线问题。
    ([uum-132475](https://issuetracker.unity3d.com/issues/learn-more-underline-doesnt-appear-on-both-words-if-they-get-separated-into-two-lines))

- `编辑器"`: 修复了样本水面 VFX 图形节点中的水纹取样问题。
    (UUM-132609)

- `编辑器`: 修复了远处风速较高时的水面高度取样。
    ([UUM-121090](https://issuetracker.unity3d.com/issues/hdrp-water-surface-water-height-sampling-returns-false-height-when-distant-wind-speed-is-high))

- `编辑器改进了 `: worldToGUIPoint` 和 `OnDrawGizmos` API 行为的描述。

- `嵌入式Linux`: EmbeddedLinux：RaspiOS vulkan 崩溃修复。
    ([uum-129585](https://issuetracker.unity3d.com/issues/embedded-linux-crash-on-application-launch-with-vulkan))

- `图形`: 启用软阴影时点光源阴影伪影的修复。
    ([uum-128839](https://issuetracker.unity3d.com/issues/white-lighting-artifact-when-a-point-light-with-a-small-emission-range-and-hard-shadows-touches-an-object-while-a-directional-light-with-soft-shadows-and-another-point-light-are-present))

- `图形`: 修改了帧清理贴图，以移除无效或无内存的纹理 ID 而不删除它们。
    (UUM-129828)

- `iOS`: 修复了使用数字键盘或电话键盘类型时屏幕键盘无法重新打开的问题。
    (UUM-132968)

- `iOS`: 修正了在UaaL设置中调整unity视图大小会破坏渲染或崩溃的问题。
    ([UUM-130881](https://issuetracker.unity3d.com/issues/ios-rendering-freezes-and-unitygfxdeviceworker-crash-when-show-splash-screen-is-enabled-and-project-is-built-using-unity-as-a-library))

- `物理修正了在禁用场景重载的情况下制作布料组件时发生崩溃的问题。制作完成后立即进入播放模式仍会使布料实例处于 "仅制作 "状态，这意味着底层模拟对象并未创建。
    ([uum-110845](https`: //issuetracker.unity3d.com/issues/crash-on-clothscene-processcomponentupdates-when-entering-play-mode-after-editing-cloth-collision-points))

- `物理 2D"`: 修正了低级物理脚本文档中的错字和错误链接。
    (UUM-132991)

- `剖析器修正了当在路径值为空的播放器上调用 MemoryProfiler.TakeSnapshot 时未将内存捕获发送到正确文件夹的问题。
    (UUM-107629)

- 剖析器剖析器`: 修复了用于剖析器或使用 MemLabel kMemProfiling/kMemProfilingEditor 的内存的本机内存根植问题，该问题会在内存剖析器中显示为 Native &gt; Unity Subsystems &gt; Unrooted。
    (UUM-128226)

- `着色器修正了调用 `: ShaderUtil.GetMaterialProperties` 时的罕见崩溃。
    ([UUM-130712](https://issuetracker.unity3d.com/issues/crash-on-pptr-operator-shader-star-ptr64-when-opening-a-project-with-specific-assets))

- `着色器`: 修正了着色器编译日志信息中的数字格式。
    (UUM-132747)

- `SRP 核心`: 修正了联编后渲染调试器为空的问题。
    ([UUM-131802](https://issuetracker.unity3d.com/issues/renderingdebugger-opening-rendering-debugger-after-building-the-player-does-not-register-any-debug-items))

- `SRP Core`: 修正了多次打开/关闭软件包管理器窗口时 SampleDependencyImporter 的罕见错误。
    ([uum-132472](https://issuetracker.unity3d.com/issues/system-dot-nullreferenceexception-errors-logged-when-opening-the-package-manager-via-button-in-the-toolbar-whilst-packages-are-loading))

- `SRP Core`: 修正了当 MSAA 启用且 URP 中的装饰渲染器功能设置为自动或 DBuffer 时，渲染图无法处理 Gizmos 渲染的 DepthCopy 传递。
    ([uum-131330](https://issuetracker.unity3d.com/issues/black-game-view-screen-and-exception-mismatch-when-gizmos-are-enabled-in-game-view-with-msaa-enabled-and-the-decal-renderer-feature-set-to-automatic-or-dbuffer-in-urp))

- `文本"`: 已添加 ATG 行高支持。
    ([uum-132202](https://issuetracker.unity3d.com/issues/paragraph-spacing-and-the-line-height-tag-are-not-working-when-the-advanced-text-generator-is-enabled))

- `文本`: 已为 ATG 添加缩进标记支持。
    (UUM-131288)

- `用户界面工具包`: 删除元素后停靠生成器时抛出 NullReferenceException。
    ([UUM-128717](https://issuetracker.unity3d.com/issues/docked-ui-builder-corrupts-when-the-domain-isnt-reloaded-after-deleting-an-element))

- `用户界面工具包`: 当 VisualElement 材质不兼容时显示警告。
    ([uum-114770](https://issuetracker.unity3d.com/issues/material-applied-to-label-renders-over-ui-builder-window-when-zoomed-in))

- `版本控制修正了 2.11.2 中 WaitForPendingOperations.cs.meta 中因无效重复 GUID 而导致的编译错误。

- 版本控制修正了在 Unity 6.3 以下版本中直接访问编辑器内部的问题。

- WebGL`: WebGPU：修复了对 texture_formats_tier2 扩展处理不一致的问题，该扩展可对多种纹理格式进行读写存储纹理访问。
    (UUM-131865)




## 6000.3.7f1 中的软件包变更

## 更新的软件包

- `com.unity.2d.animation`: [13.0.2](https://docs.unity3d.com/Packages/com.unity.2d.animation@13.0//changelog/CHANGELOG.html) 到 [13.0.4](https://docs.unity3d.com/Packages/com.unity.2d.animation@13.0//changelog/CHANGELOG.html)

- `com.unity.2d.common`: [12.0.1](https://docs.unity3d.com/Packages/com.unity.2d.common@12.0//changelog/CHANGELOG.html) 到 [12.0.2](https://docs.unity3d.com/Packages/com.unity.2d.common@12.0//changelog/CHANGELOG.html)

- `com.unity.2d.tooling`: [1.0.0](https://docs.unity3d.com/Packages/com.unity.2d.tooling@1.0//changelog/CHANGELOG.html) 到 [1.0.2](https://docs.unity3d.com/Packages/com.unity.2d.tooling@1.0//changelog/CHANGELOG.html)

- `com.unity.collab-proxy`: [2.11.2](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.11//changelog/CHANGELOG.html) 到 [2.11.3](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.11//changelog/CHANGELOG.html)

- `com.unity.ide.rider`: [3.0.38](https://docs.unity3d.com/Packages/com.unity.ide.rider@3.0//changelog/CHANGELOG.html) 到 [3.0.39](https://docs.unity3d.com/Packages/com.unity.ide.rider@3.0//changelog/CHANGELOG.html)

- `com.unity.mobile.android-logcat`: [1.4.6](https://docs.unity3d.com/Packages/com.unity.mobile.android-logcat@1.4//changelog/CHANGELOG.html) 到 [1.4.7](https://docs.unity3d.com/Packages/com.unity.mobile.android-logcat@1.4//changelog/CHANGELOG.html)

- `com.unity.testtools.codecoverage`: [1.2.7](https://docs.unity3d.com/Packages/com.unity.testtools.codecoverage@1.2//changelog/CHANGELOG.html) 到 [1.3.0](https://docs.unity3d.com/Packages/com.unity.testtools.codecoverage@1.3//changelog/CHANGELOG.html)

- `com.unity.xr.hands`: [1.7.2](https://docs.unity3d.com/Packages/com.unity.xr.hands@1.7//changelog/CHANGELOG.html) 到 [1.7.3](https://docs.unity3d.com/Packages/com.unity.xr.hands@1.7//changelog/CHANGELOG.html)

- `com.unity.profiling.systemmetrics.mali`: [1.1.0](https://docs.unity3d.com/Packages/com.unity.profiling.systemmetrics.mali@1.1//changelog/CHANGELOG.html) 到 [1.1.1](https://docs.unity3d.com/Packages/com.unity.profiling.systemmetrics.mali@1.1//changelog/CHANGELOG.html)