# Unity 6000.3.16f1 LTS
发布于格林尼治标准时间 2026 年 5 月 20 日 (星期三) 14:16:31
https://unity.com/releases/editor/whats-new/6000.3.16f1

# 6000.3.16f1 中的已知问题

- `6000.0.61f1`: 使用 SDF16 或 SDF32 生成字体图集时 tlsf_free 崩溃
    ([uum-141061](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-generating-font-atlas-with-sdf16-or-sdf32))

- `6000.0.6f1`: [渲染图][D3D12]当使用带有EnableAsyncCompute(true)和UseTexture的AddComputePass时，D3D12SwapChain::Present崩溃。
    ([uum-140183](https://issuetracker.unity3d.com/issues/rendergraph-d3d12-crash-on-d3d12swapchain-present-when-using-addcomputepass-with-enableasynccompute-true-and-usetexture))

- `6000.4.0a2,6000.3.0b6`: 当悬停通过 ATG 渲染的带有 <link> 标记的 UITK 标签时，TextLib::FindIntersectingLink 中的编辑器崩溃
    ([uum-142829](https://issuetracker.unity3d.com/issues/editor-crashes-in-textlib-findintersectinglink-when-hovering-uitk-labels-with-tags-rendered-via-atg))

- 金属命令缓冲区超时错误后游戏冻结
    ([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- 文本 (TextMeshPro)：在 TMPro Font Asset Creator 中生成多线程字体图集时，在 UNITY_FT_Load_Glyph 上崩溃
    ([uum-125366](https://issuetracker.unity3d.com/issues/crash-on-unity-ft-load-glyph-when-generating-multi-threaded-font-atlas-in-tmpro-font-asset-creator))

当运行一个以上的bee_backend副本时，mono_log_write_logfile崩溃
    ([uum-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))

当DX12图形应用程序接口在图形应用程序接口列表中排在第一位时，未使用该程序接口
    ([uum-141555](https://issuetracker.unity3d.com/issues/dx12-graphics-api-is-not-used-when-it-is-first-in-the-graphics-api-list))

在打开子场景的预制模式中禁用子游戏对象时，材质会移动到预制中的其他游戏对象上
    ([uum-139663](https://issuetracker.unity3d.com/issues/materials-move-to-other-gameobjects-in-a-prefab-when-disabling-a-child-gameobject-in-prefab-mode-with-an-open-subscene))



# 6000.3.16f1 发行说明

## 改进

- `图形在 GfxDeviceGLES`: DrawBuffersBatchMode 中添加了对空索引缓冲的保护。
    (UUM-135891)



## API 更改

- `用户界面工具包`: 新增： 新增了带有 `CallbackOptions` 参数的 `CallbackEventHandler.RegisterCallbacks` 方法覆盖。

- `用户界面工具包已添加`: 已添加 `CallbackEventHandler.UnregisterAllRemovableCallbacks` 方法。

- `UI 工具包已添加`: 已添加 `CallbackOptions` 枚举。



## 更改

- `Android`: 更新 JDK 至 17.0.18+8。
    (UUM-141159)



## 修复

- `2D`: 修正了 Hidden/Light2D 中的着色器警告。
    ([uum-134522](https://issuetracker.unity3d.com/issues/shader-warning-in-hidden-slash-light2d-implicit-truncation-of-vector-type-is-thrown-when-building-universal-2d-template))

- `2D`: 修正了当在 "编辑 "模式下的 "场景视图 "中打开 "瓦片调色板 "时，在 "播放 "模式下选择 "瓦片 "时出现的异常。
    ([uum-137165](https://issuetracker.unity3d.com/issues/invalidoperationexception-and-nullreferenceexception-errors-are-thrown-when-clicking-inside-a-tile-palette-with-the-tile-palette-overlay-and-tile-palette-edit-enabled))

- `2D`: 修正了当使用 "雪碧编辑器 "窗口中的预览切换时，导入的纹理小于源纹理的异常。
    ([uum-134129](https://issuetracker.unity3d.com/issues/sprite-editor-argumentexception-error-when-scene-view-preview-option-is-used-on-psb-format-files))

- `2D`: 修正了一个问题，即在使用 "雪碧编辑器 "窗口预览切换并进入 "播放 "模式后，雪碧渲染器的雪碧引用不会还原为原始引用。现在只有在 "编辑 "模式下才能使用 "精灵编辑器 "窗口预览切换。
    ([uum-134128](https://issuetracker.unity3d.com/issues/sprite-does-not-revert-to-original-texture-when-entering-play-mode-with-scene-view-preview-enabled-in-the-sprite-editor-window))

- `2D`: 修正了一个问题，即当用户为磁贴调色板拖放雪碧资产但取消创建磁贴资产的操作时，磁贴调色板会显示一个空网格。
    ([uum-132388](https://issuetracker.unity3d.com/issues/tile-palette-texture-drag-area-label-drag-tile-sprite-or-texture-sprite-type-asset-slash-s-here-dot-disappears-when-the-asset-save-pop-up-is-closed-slash-canceled))

- `2D`: 修正了 2D 阴影体积强度的问题。
    ([uum-136056](https://issuetracker.unity3d.com/issues/shadows-from-light2d-do-not-change-when-volumetric-shadow-strength-is-toggled-off))

- `2D`: 修正了当瓦片贴图的瓦片锚点与默认单元格中心不同时， Collider Type Grid 的瓦片无法正确对齐的问题。
    (UUM-136995)

- `Android`: 添加了 RunInBackground 测试，以涵盖全屏用例。

- `Android`: 修正了应用程序暂停时媒体播放器暂停的问题。
    (UUM-140840)

- `Android`: 修正了 SeekTimeOnResumeVideo 测试不稳定的问题。
    (UUM-140837)

- `Android`: 修正了在Unity as a Library \(UAAL\)场景中，当Application.Unload或Reload期间发送UnitySendMessage时，Android上的UnitySendMessage调用被丢弃的问题。
    (UUM-141440)

- `Android`: 将 "无焦点运行 "切换为启用，现在可以确保在启动其他活动（包括从 Unity 启动的 Android 活动）时继续运行 Unity 活动。
    ([UUM-120304](https://issuetracker.unity3d.com/issues/android-unityplayer-gets-paused-when-another-activity-is-launched-even-with-run-without-focus-enabled))

- 动画修正了当未选择任何内容时出现的 "动画剪辑只读 "信息。
    ([uum-139142](https://issuetracker.unity3d.com/issues/animation-clip-is-read-only-is-shown-in-the-animation-window-when-nothing-is-selected))

- `音频`: 修复了从资产包加载带有音轨的时间线时，如果音频片段未能分配 FMOD 通道，则在进入播放模式时崩溃的问题。
    ([uum-136551](https://issuetracker.unity3d.com/issues/crash-on-soundchannelinstance-setdelay-when-loading-an-assetbundle-containing-a-timeline-with-an-audioclip-at-scene-startup))

- `构建管道"`: 构建管道：确保在 Rider IDE 中运行时，源生成器不会运行。
    (UUM-133605)

- `构建管道`: 修正 ILPP.Trigger 等待逻辑，以防止 unity 日志中出现 "管道正在关闭 "异常。
    (UUM-136791)

- `构建系统`: 修正了使用特定构建路径时，在构建过程中出现节点 GUID 重复错误的问题。
    ([UUM-128491](https://issuetracker.unity3d.com/issues/build-fails-with-duplicate-node-guids-error-when-using-specific-build-path))

- `文档`: 修正了 Flare Layer 帮助到用户手册的链接。
    ([uum-134470](https://issuetracker.unity3d.com/issues/the-help-icon-of-flare-layer-component-refers-to-a-missing-unity-documentation-page-when-clicked))

- `DX12`: 修正了特定硬件上的崩溃问题，即使 D3D12 未包含在项目的图形 API 列表中，D3D12 初始化代码仍会在启动过程中运行。
    ([uum-137629](https://issuetracker.unity3d.com/issues/unity-player-loads-d3d12-dll-even-when-direct3d12-is-removed-from-project-settings))

- 编辑器尽管指定了远程构建（Device Portal），但本地无效架构的构建和运行按钮呈灰色。
    ([uum-138399](https://issuetracker.unity3d.com/issues/build-and-run-button-greyed-out-for-locally-invalid-architecture-despite-remote-build-is-specified))

- 编辑器修正了一个错误，即在 macOS 上使用 -projectPath 命令行参数启动编辑器时，Unity Hub 会打开。
    ([uum-136928](https://issuetracker.unity3d.com/issues/unity-hub-opens-when-launching-the-editor-with-projectpath-argument))

- 编辑器修复了在两个碰撞器的中心重叠时，调用方框碰撞器和凸网格碰撞器的 computePenetration 时发生的崩溃。
    ([uum-100359](https://issuetracker.unity3d.com/issues/meshcollider-does-not-detect-collisions-with-capsules-and-charactercontroller-when-using-physics-dot-computepenetration))

- 编辑器修正了在启用 Forward+ 和禁用 Keep Lighting Variants 时渲染自定义照明 ShaderGraph 材质时的崩溃问题。
    ([uum-137255](https://issuetracker.unity3d.com/issues/crash-on-checkdevicestatus-when-rendering-custom-lighting-shadergraph-material-while-forward-plus-is-enabled-and-keep-lighting-variants-is-disabled))

- 编辑器修正了为接受任何 `UnityEngine.Object` 类型的字段打开对象选择器时的 `ArgumentException` 问题，例如预载资产列表中的条目。
    ([uum-135060](https://issuetracker.unity3d.com/issues/argumentexception-no-valid-types-in-required-type-list-error-is-thrown-when-opening-an-object-picker-menu-in-the-preloaded-assets-in-player-settings))

- 编辑器提高了 CapsuleCollider 和凸网格对撞器之间的 ComputePenetration 调用的可靠性。当距离为零时，ComputePenetration 将返回 true。
    ([uum-100359](https://issuetracker.unity3d.com/issues/meshcollider-does-not-detect-collisions-with-capsules-and-charactercontroller-when-using-physics-dot-computepenetration))

- 编辑器提高了 CharacterController 与凸网格对撞器之间调用 ComputePenetration 的可靠性。当距离为零时，ComputePenetration 将返回 true。
    ([uum-100359](https://issuetracker.unity3d.com/issues/meshcollider-does-not-detect-collisions-with-capsules-and-charactercontroller-when-using-physics-dot-computepenetration))

- 编辑器现在可以在帧调试器（FrameDebugger）中查看无记忆渲染图渲染目标（Memoryless RenderGraph RenderTargets）。
    ([uum-133585](https://issuetracker.unity3d.com/issues/draw-gbuffer-pass-appears-black-in-frame-debugger-when-deferred-or-deferred-plus-is-enabled))

- 编辑器为 Vulkan 编辑器提前设置软件包权限，以支持所有原生插件用例。
    ([uum-135157](https://issuetracker.unity3d.com/issues/vulkan-native-graphics-plugins-load-after-graphics-device-initialization-in-editor-when-placed-in-packages))

- `图形`: 当启用 V-Sync 时，修复了 Windows 上的 Vulkan 帧时间卡顿问题。
    (UUM-140217)

- `iOS`: 修正了帧捕捉在渲染到后缓冲区时无法工作的问题。
    ([UUM-141280](https://issuetracker.unity3d.com/issues/ios-frame-debugger-rendering-output-doesnt-work-with-ios-builds))

- `iOS`: 进一步改进了 UIScene 生命周期事件 - 通用深层链接处理，提前移动 AbsoluteURL 设置以避免在 Awake\(\) 中错过。
    (UUM-140746)

- 网络修正了 MbedTLS 中的一个回归，当尝试从软件包管理器的资产商店下载资产时，该回归会导致 TLS 握手错误。其他 HTTPS 端点也可能受到此回归的影响。
    (UUM-141298)

- 网络通过支持多个自动代理修复了 UUM-135025。
    ([UUM-135025](https://issuetracker.unity3d.com/issues/unitywebrequest-returns-curl-error-5-instead-of-timing-out-when-the-windows-proxy-auto-config-script-returns-multiple-proxies))

- `物理 2D`: 修正了 "PhysicsComposer.CreateChainGeometry\(\) "不正确地返回引用一个陈旧的内部缓冲区导致链顶点损坏的问题。
    ([uum-139048](https://issuetracker.unity3d.com/issues/physicscomposer-dot-createchaingeometry-is-returning-stale-vertex-geometry))

- `物理 2D"`: 修正了不允许创建 3 个顶点的 ChainGeometry \(triangle\) 的问题，因为之前的限制是 4 个顶点。
    ([uum-139044](https://issuetracker.unity3d.com/issues/chaingeometry-does-not-allow-3-vertex-buffers-even-when-using-isloop-equals-true))

- `物理 2D"`: 已废弃的 "ContactFilter2D.NoFilter\(\) "实例方法现在可以正确修改被调用的 "ContactFilter2D "实例，基本上恢复了以前的功能。不过，该方法仍被弃用。
    ([uum-139052](https://issuetracker.unity3d.com/issues/deprecated-contactfilter2d-dot-nofilter-method-should-assign-the-filter-to-the-instance))

- 插件修正了 Linux 原生插件无法指定其 CPU 架构的问题。
    ([uum-131765](https://issuetracker.unity3d.com/issues/native-plugins-experience-name-conflicts-when-built-for-both-x86-linux-and-arm64-linux))

- 剖析器修正了 Profiler 层次调用表中 None 文本的渲染。
    ([uum-114430](https://issuetracker.unity3d.com/issues/module-details-pane-window-and-text-is-too-dark-when-editor-theme-is-set-to-light))

- 脚本编写修正了容器中的整数溢出崩溃。
    ([uum-134628](https://issuetracker.unity3d.com/issues/crash-on-memcpy-when-opening-a-scene-with-specific-assets))

- 着色器修正了在玩家构建中访问 `shaderCount` 和 `variantCount` 时，`ShaderVariantCollection` 返回 0 的问题。
    ([uum-137398](https://issuetracker.unity3d.com/issues/shadervariantcollection-dot-variantcount-and-shadervariantcollection-dot-shadercount-returns-0-in-builds))

- 文本修正了与 `SpriteAsset` 一起使用时 `NoBR` 标记的问题。
    (UUM-139609)

- 用户界面工具包修正了使用 Painter2D.fillGradient 构建播放器或使用 VisualElement 切换场景时记录的 "Attempted to release an invalid texture \(index=-1\). "错误。
    ([uum-140738](https://issuetracker.unity3d.com/issues/ui-builder-window-throws-an-attempted-to-release-an-invalid-texture-index-equals-1-dot-error-when-building-a-project-after-changing-gradient-settings-of-a-visualelement))

- `用户界面工具包`: 修正了 UI 生成器中当模板具有同名元素时的无效铸造异常。
    ([uum-140739](https://issuetracker.unity3d.com/issues/invalid-cast-exception-in-ui-builder-when-template-has-element-with-same-name))

- `用户界面工具包`: 修正了 RenderSpriteToTexture2D，以便在可用时使用本地包着色器。
    ([uum-140566](https://issuetracker.unity3d.com/issues/svg-shaders-get-stripped-when-building-player))

- `用户界面工具包`: 修正了着色器图形主预览，当在 UI 工具包着色器中修改 BaseColor 等非连接槽值时，该预览不会更新。
    ([uum-138534](https://issuetracker.unity3d.com/issues/shader-graph-main-preview-color-is-not-updated-when-modifying-the-base-color-node-in-ui-shader-graph))

- `重做系统"`: 在通知对象跟踪之前清除重做时的空组件。
    ([uum-135948](https://issuetracker.unity3d.com/issues/crash-on-objecttotypedispatchdatahandle-when-redoing-canvas-creation-in-a-specific-project))

- `URP`: 修正了添加或删除可脚本渲染器功能时，项目窗口不会刷新更改的问题。
    ([uum-139513](https://issuetracker.unity3d.com/issues/urp-asset-sub-assets-show-changes-in-sub-assets-only-after-reimporting-the-urp-asset-manually))

- `URP`: 修正了当相机渲染到中间纹理时，后处理传递视口缩放不考虑后续自定义传递的存在。
    ([uum-109492](https://issuetracker.unity3d.com/issues/urp-camera-output-texture-has-wrong-scale-when-using-bilinear-upscale-filter-and-when-renderfeature-requires-intermediate-texture))

- `VFX Graph`: 修正了在 VisualEffectAsset 上意外列出大量依赖关系的问题。
    ([uum-140725](https://issuetracker.unity3d.com/issues/editorutility-dot-collectdependencies-returns-non-dependent-assets-when-checking-visual-effects-assets))




## 6000.3.16f1 中的软件包变更

## 更新的软件包

- `com.unity.collections`: [2.6.5](https://docs.unity3d.com/Packages/com.unity.collections@2.6//changelog/CHANGELOG.html) 到 [2.6.6](https://docs.unity3d.com/Packages/com.unity.collections@2.6//changelog/CHANGELOG.html)

- `com.unity.entities`: [1.4.5](https://docs.unity3d.com/Packages/com.unity.entities@1.4//changelog/CHANGELOG.html) 至 [1.4.6](https://docs.unity3d.com/Packages/com.unity.entities@1.4//changelog/CHANGELOG.html)

- `com.unity.physics`: [1.4.5](https://docs.unity3d.com/Packages/com.unity.physics@1.4//changelog/CHANGELOG.html) 至 [1.4.6](https://docs.unity3d.com/Packages/com.unity.physics@1.4//changelog/CHANGELOG.html)

- `com.unity.entities.graphics`: [1.4.18](https://docs.unity3d.com/Packages/com.unity.entities.graphics@1.4//changelog/CHANGELOG.html) 到 [1.4.19](https://docs.unity3d.com/Packages/com.unity.entities.graphics@1.4//changelog/CHANGELOG.html)

- `com.unity.2d.animation`: [13.0.4](https://docs.unity3d.com/Packages/com.unity.2d.animation@13.0//changelog/CHANGELOG.html) 到 [13.0.5](https://docs.unity3d.com/Packages/com.unity.2d.animation@13.0//changelog/CHANGELOG.html)

- `com.unity.2d.common`: [12.0.2](https://docs.unity3d.com/Packages/com.unity.2d.common@12.0//changelog/CHANGELOG.html) 到 [12.0.3](https://docs.unity3d.com/Packages/com.unity.2d.common@12.0//changelog/CHANGELOG.html)

- `com.unity.2d.psdimporter`: [12.0.1](https://docs.unity3d.com/Packages/com.unity.2d.psdimporter@12.0//changelog/CHANGELOG.html) 到 [12.0.2](https://docs.unity3d.com/Packages/com.unity.2d.psdimporter@12.0//changelog/CHANGELOG.html)

- `com.unity.2d.tilemap.extras`: [6.0.1](https://docs.unity3d.com/Packages/com.unity.2d.tilemap.extras@6.0//changelog/CHANGELOG.html) 到 [6.0.2](https://docs.unity3d.com/Packages/com.unity.2d.tilemap.extras@6.0//changelog/CHANGELOG.html)

- `com.unity.2d.aseprite`: [3.0.1](https://docs.unity3d.com/Packages/com.unity.2d.aseprite@3.0//changelog/CHANGELOG.html) 到 [3.0.2](https://docs.unity3d.com/Packages/com.unity.2d.aseprite@3.0//changelog/CHANGELOG.html)

- `com.unity.2d.tooling`: [1.0.2](https://docs.unity3d.com/Packages/com.unity.2d.tooling@1.0//changelog/CHANGELOG.html) 到 [1.0.3](https://docs.unity3d.com/Packages/com.unity.2d.tooling@1.0//changelog/CHANGELOG.html)

- `com.unity.ide.rider`: [3.0.39](https://docs.unity3d.com/Packages/com.unity.ide.rider@3.0//changelog/CHANGELOG.html) 到 [3.0.40](https://docs.unity3d.com/Packages/com.unity.ide.rider@3.0//changelog/CHANGELOG.html)

- `com.unity.performance.profile-analyzer`: [1.3.3](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.3//changelog/CHANGELOG.html) 到 [1.3.4](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.3//changelog/CHANGELOG.html)

- `com.unity.services.cloud-build`: [2.0.7](https://docs.unity3d.com/Packages/com.unity.services.cloud-build@2.0//changelog/CHANGELOG.html) 到 [2.0.8](https://docs.unity3d.com/Packages/com.unity.services.cloud-build@2.0//changelog/CHANGELOG.html)

- `com.unity.transport`: [2.7.2](https://docs.unity3d.com/Packages/com.unity.transport@2.7//changelog/CHANGELOG.html) 到 [2.7.3](https://docs.unity3d.com/Packages/com.unity.transport@2.7//changelog/CHANGELOG.html)

- `com.unity.netcode.gameobjects`: [2.11.1](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@2.11//changelog/CHANGELOG.html) 到 [2.11.2](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@2.11//changelog/CHANGELOG.html)

- `com.unity.toolchain.win-x86_64-linux`: [1.0.2](https://docs.unity3d.com/Packages/com.unity.toolchain.win-x86_64-linux@1.0//changelog/CHANGELOG.html) 到 [1.1.0](https://docs.unity3d.com/Packages/com.unity.toolchain.win-x86_64-linux@1.1//changelog/CHANGELOG.html)

- `com.unity.toolchain.win-arm64-linux`: [1.0.2](https://docs.unity3d.com/Packages/com.unity.toolchain.win-arm64-linux@1.0//changelog/CHANGELOG.html) 到 [1.1.0](https://docs.unity3d.com/Packages/com.unity.toolchain.win-arm64-linux@1.1//changelog/CHANGELOG.html)

- `com.unity.toolchain.macos-x86_64-linux`: [1.0.2](https://docs.unity3d.com/Packages/com.unity.toolchain.macos-x86_64-linux@1.0//changelog/CHANGELOG.html) 到 [1.1.0](https://docs.unity3d.com/Packages/com.unity.toolchain.macos-x86_64-linux@1.1//changelog/CHANGELOG.html)

- `com.unity.toolchain.macos-arm64-linux`: [1.0.2](https://docs.unity3d.com/Packages/com.unity.toolchain.macos-arm64-linux@1.0//changelog/CHANGELOG.html) 到 [1.1.0](https://docs.unity3d.com/Packages/com.unity.toolchain.macos-arm64-linux@1.1//changelog/CHANGELOG.html)

- `com.unity.toolchain.linux-x86_64-linux`: [1.0.2](https://docs.unity3d.com/Packages/com.unity.toolchain.linux-x86_64-linux@1.0//changelog/CHANGELOG.html) 到 [1.1.0](https://docs.unity3d.com/Packages/com.unity.toolchain.linux-x86_64-linux@1.1//changelog/CHANGELOG.html)

- `com.unity.sysroot.base`: [1.0.2](https://docs.unity3d.com/Packages/com.unity.sysroot.base@1.0//changelog/CHANGELOG.html) 到 [1.1.0](https://docs.unity3d.com/Packages/com.unity.sysroot.base@1.1//changelog/CHANGELOG.html)

- `com.unity.sdk.linux-x86_64`: [1.0.2](https://docs.unity3d.com/Packages/com.unity.sdk.linux-x86_64@1.0//changelog/CHANGELOG.html) 到 [1.1.0](https://docs.unity3d.com/Packages/com.unity.sdk.linux-x86_64@1.1//changelog/CHANGELOG.html)

- `com.unity.sdk.linux-arm64`: [1.0.2](https://docs.unity3d.com/Packages/com.unity.sdk.linux-arm64@1.0//changelog/CHANGELOG.html) 到 [1.1.0](https://docs.unity3d.com/Packages/com.unity.sdk.linux-arm64@1.1//changelog/CHANGELOG.html)