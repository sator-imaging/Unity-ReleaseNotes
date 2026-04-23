# Unity 6000.3.14f1 LTS
发布于 星期三, 22 四月 2026 12:21:09 GMT
https://unity.com/releases/editor/whats-new/6000.3.14f1

# 6000.3.14f1 中的已知问题

- `6000.0.6f1`: [渲染图形][D3D12]当使用带有 EnableAsyncCompute(true) 和 UseTexture 的 AddComputePass 时，D3D12SwapChain::Present 会崩溃。
    ([uum-140183](https://issuetracker.unity3d.com/issues/rendergraph-d3d12-crash-on-d3d12swapchain-present-when-using-addcomputepass-with-enableasynccompute-true-and-usetexture))

- `6000.2.0a10`: 首次打开项目时，TexturesD3D12::CreateTextureInternal()崩溃
    ([uum-135024](https://issuetracker.unity3d.com/issues/crash-on-checkdevicestatus-when-opening-a-project-for-the-first-time))

- `6000.3.0a3`: 当使用最小近剪切平面值制作自定义反射探针时，Umbra::QueryExt::queryStaticShadowCasters 会崩溃
    ([uum-137250](https://issuetracker.unity3d.com/issues/crash-on-umbra-queryext-querystaticshadowcasters-when-baking-a-custom-reflection-probe-with-the-minimum-near-clipping-planes-value))

- `6000.3.0a5`: 当距离摄像机超过 1000 个单位时，URP 贴纸变得不可见
    ([uum-138945](https://issuetracker.unity3d.com/issues/urp-decals-become-invisible-when-over-1000-units-away-from-the-camera))

- `6000.5.0a4,6000.0.66f1,6000.3.4f1,6000.4.0b4`: 在 Builds 中，ShaderVariantCollection.variantCount 和 ShaderVariantCollection.shaderCount 返回 0
    ([uum-137398](https://issuetracker.unity3d.com/issues/shadervariantcollection-dot-variantcount-and-shadervariantcollection-dot-shadercount-returns-0-in-builds))

- `6000.5.0a8,6000.6.0a1,6000.4.0b12,6000.3.12f1`: 生成照明时，xatlas::internal::pack::Atlas::findChartLocation_bruteForce 崩溃
    ([uum-139715](https://issuetracker.unity3d.com/issues/crash-on-xatlas-internal-pack-atlas-findchartlocation-bruteforce-when-generating-the-lighting))

- `6000.5.0a8,6000.6.0a1,6000.4.0b12,6000.3.12f1`: 在特定场景中构建照明时出现多个堆栈跟踪时崩溃
    ([uum-138494](https://issuetracker.unity3d.com/issues/crash-with-multiple-stacktraces-when-building-lighting-in-a-specific-scene))

- `6000.6.0a1,6000.3.11f1`: 使用 DrawText() 在用户界面文档中创建动态文本时，颜色参数被忽略
    ([uum-137907](https://issuetracker.unity3d.com/issues/color-parameter-is-ignored-when-creating-dynamic-text-in-a-ui-document-with-drawtext))

- `6000.6.0a1,6000.5.0a9,6000.3.12f1,6000.4.0f1`: 切换平台将触发着色器相关警告（TraceTransparentRays）
    ([uum-139001](https://issuetracker.unity3d.com/issues/switching-platforms-will-trigger-shader-related-warnings-tracetransparentrays))

- `Metal`: 命令缓冲区超时错误后游戏冻结
    ([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- `金属"`: MacOS 在编辑器中的最小项目在播放模式下出现卡顿
    ([uum-85256](https://issuetracker.unity3d.com/issues/macos-stutters-in-a-minimal-project))

在 List<T> 结构中使用嵌套 [SerializeReference] 字段时，"core::base_hash_set "崩溃
    ([uum-139722](https://issuetracker.unity3d.com/issues/crash-on-core-base-hash-set-when-using-nested-serializereference-fields-in-list-structures))

在空白 URP 项目中重新编译时，VisualElement 中的编辑器内存泄漏
    ([uum-138000](https://issuetracker.unity3d.com/issues/editor-memory-leak-in-visualelement-when-recompiling-in-a-blank-urp-project))

在打开子场景的预制模式中禁用子游戏对象时，材质会移动到预制中的其他游戏对象上
    ([uum-139663](https://issuetracker.unity3d.com/issues/materials-move-to-other-gameobjects-in-a-prefab-when-disabling-a-child-gameobject-in-prefab-mode-with-an-open-subscene))



# 6000.3.14f1 发行说明

## 功能

- `用户界面工具包用户界面工具包`: 引入了一个 UXML 升级框架，用于应用自动 UXML 升级来修复常见问题和过时的模式。可从 VisualTreeAsset 检查器或通过脚本 UnityEditor.UIElements.UxmlUpgradeService 进行访问。



### 改进

- `用户界面工具包在用户界面生成器中添加了一个选项，可按字母顺序导出元素的 UXML 属性。

- 用户界面工具包通过减少应用于默认网格的边缘抗锯齿区域，提高了 GPU 性能。

- 用户界面工具包提高了 VisualElement.UpdateWorldTransformInverse 的性能。

- XR`: 更新了元探索构建配置文件自定义质量设置的默认设置。



## API 更改

- `编辑器已更改`: 在未定义 ENABLE_UNITY_COLLECTIONS_CHECKS 时，公开 JobHandle.GetHashCode 和 Equals 以及 ==/\!= 运算符。

- `用户界面工具包新增`: 添加了一个新的 API 来清除 VisualElement 的内联样式（element.style.Clear\(\)）。



## 更改

- 音频在基于 Chromium 的网络浏览器上，内存压缩设置默认为加载时解压缩，以避免内存泄漏。
    ([uum-136929](https://issuetracker.unity3d.com/issues/detached-audio-source-is-not-released-from-browser-memory-when-audio-stops-playing-in-webgl-player))



## 修复

- `2D`: 添加了对使用 2D 渲染器的 Unity Recorder 的支持。
    (UUM-136415)

- `2D`: 剔除精灵皮肤时精灵闪烁/绘制调用波动。
    ([UUM-132924](https://issuetracker.unity3d.com/issues/draw-call-count-fluctuates-and-frame-debugger-output-flickers-when-viewing-a-psd-based-sprite-skin-with-always-update-disabled-in-game-view))

- 辅助功能修正了使用辅助功能 API 时的潜在崩溃问题。
    (UUM-132644)

- 辅助功能修正了 Windows 10 上 UI Automation 访问无效指针导致的播放器崩溃。
    ([UUM-126552](https://issuetracker.unity3d.com/issues/application-crash-when-setting-assistivesupport-dot-activehierarchy-with-narrator-enabled-on-windows-10))

- 辅助功能修复了在 Windows 10 上失败的 `AssistiveSupport` 播放模式测试，并重新启用了它们。
    (UUM-111323)

- `自适应性能`: 修正了自适应性能剖析器模块中的缩放器数据 UI 结构。
    (UUM-138268)

- 自适应性能重构自适应性能日志。无功能变更。
    (UUM-138191)

- 人工智能修复了半径小、目的地远的代理在绘制调试可视化时崩溃的问题。
    ([UUM-133552](https://issuetracker.unity3d.com/issues/crash-on-memcpy-repmovs-when-selecting-navmesh-agent-objects-while-in-play-mode-in-a-specific-scene))

- `Android`: 修正了在安卓平台上使用URP时，如果在播放器设置中禁用了深度/模版缓冲区，则会发生崩溃的问题。
    ([uum-109005](https://issuetracker.unity3d.com/issues/android-player-crashes-on-vk-renderpasses-getpackedrenderpass-when-using-vulkan-graphics-api-in-a-specific-project))

- `Android`: 修正了在 Pixel 10 上使用丢弃或剪辑着色器时出现伪影的问题。
    (UUM-139019)

- 动画修正了当添加至动画剪辑并在动画窗口中采样时，某些粒子系统属性会导致错误和警告的问题。
    ([uum-134950](https://issuetracker.unity3d.com/issues/unsupported-type-minmaxcurve-error-and-could-not-register-property-modification-for-animation-binding-dot-dot-dot-warnings-are-thrown-after-moving-playhead-when-particle-system-property-is-added-to-animation-window))

- 音频修正了在脚本生成器中从 IRealtime.Process 调用 Pipe.GetAvailableData 时抛出的异常。
    ([uum-133969](https://issuetracker.unity3d.com/issues/pipes-are-not-working-for-nested-generators))

- 音频修正了在非 Chromium 网页浏览器上使用压缩内存设置时的内存泄漏问题。
    ([uum-136929](https://issuetracker.unity3d.com/issues/detached-audio-source-is-not-released-from-browser-memory-when-audio-stops-playing-in-webgl-player))

- `DX12`: 当有过多命令缓冲区待处理时，执行周期性完全刷新。
    ([uum-138597](https://issuetracker.unity3d.com/issues/crash-on-checkdevicestatus-when-selecting-gameobjects-in-the-scene-view-while-using-dx12))

- `DX12`: 通过暂停渲染，减少在播放器中最小化（通过 Alt-Tab）"独占全屏 "窗口时的严重崩溃。其他模式和图形 API 不受影响。为了获得更好的稳定性，请考虑使用 "FullScreenWindow"（无边框）模式（https://devblogs.microsoft.com/directx/demystifying-full-screen-optimizations/）。
    ([uum-134743](https://issuetracker.unity3d.com/issues/player-crash-when-switching-focus-in-exclusive-fullscreen-mode-with-directx-12))

- 编辑器为自适应性能设置添加了重置按钮。
    ([uum-135693](https://issuetracker.unity3d.com/issues/adaptive-performance-settings-on-the-custom-build-profile-cant-be-reset))

- 编辑器修正了在某些停靠的 "构建配置文件 "窗口中单击 "预览 "时出现的 "NullReferenceException"。
    ([uum-134827](https://issuetracker.unity3d.com/issues/nullreferenceexception-error-is-thrown-when-clicking-to-preview-the-splash-image-in-build-profiles-window))

- 编辑器修正了在 "图形设置 "中更改默认体积配置文件时抛出的异常。
    (UUM-136748)

- 编辑器修正了当`EditorSettings.asset`升级失败或手动还原/修改时，禁用了进入播放模式时域重载仍会发生的问题。
    ([uum-138521](https://issuetracker.unity3d.com/issues/enterplaymodeoptions-doesnt-take-effect-if-user-manually-modifies-m-enterplaymodeoptionsenabled-to-0))

- 编辑器修正了在动画窗口中无法正确记录 HDR 颜色的问题。
    ([uum-83771](https://issuetracker.unity3d.com/issues/hdr-colors-are-recorded-in-gamma-compressed-values-instead-of-linear-values-when-using-the-animation-window))

- `编辑器"`: 修正了一个问题，当禁用类型树和开发播放器构建时，从资产包加载 VFX 资产会导致崩溃。
    ([uum-137538](https://issuetracker.unity3d.com/issues/crash-on-cachedreader-outofboundserror-when-loading-vfx-object-from-an-asset-bundle-with-disabletypetree))

- 编辑器修复了在编辑器中加载和卸载内容文件时的死锁竞赛条件。
    (UUM-137677)

- 编辑器修正了卷配置文件的哈希码生成不一致的问题。
    ([UUM-130711](https://issuetracker.unity3d.com/issues/switching-graphics-default-or-devlook-profile-to-nightskyrenderingsettings-profile-throws-keynotfoundexception-error-in-the-console-window))

- 编辑器修正了 `InvalidOperationException：在编辑器中使用位图文本时出现的 `InvalidOperationException: EnsureRunningOnMainThread` 问题。
    ([uum-137062](https://issuetracker.unity3d.com/issues/invalidoperationexception-ensurerunningonmainthread-can-only-be-called-from-the-main-thread-is-randomly-thrown-in-the-console-when-working-in-a-urp-project-on-a-non-4k-screen-with-the-editor-default-text-rendering-mode-set-to-bitmap))

- `编辑器"`: 还原启动时间优化，以便图形设备初始化可以再次看到本地插件。
    ([uum-134389](https://issuetracker.unity3d.com/issues/package-manager-vulkan-native-rendering-plugin-can-no-longer-intercept-vulkan-initialization-as-it-is-loaded-later-when-added-via-package-manager))

- 编辑器打开 "构建配置文件 "窗口时，特定的可脚本对象资产名不再导致警告。
    ([uum-135389](https://issuetracker.unity3d.com/issues/scriptableobject-asset-is-accessed-during-the-lookup-of-build-profiles-when-opening-the-build-profiles-window))

- 编辑器当未开启 vsync 时，从 cpuactivetime 中抽取 waitfromlastpresentation 时间。
    (UUM-131842)

- 编辑器\Linux] 修正了错误使用 GTK 在控制台中产生错误的情况。
    (UUM-138332)

- `GI`: 修正了一个 Bug，当没有一个场景同时包含阴影投射混合光和烘焙光贴图或光探针时，阴影遮罩或减法着色器变体会被错误地剥离。
    ([uum-127288](https://issuetracker.unity3d.com/issues/baked-shadows-are-missing-when-loading-a-scene-additively-and-lighting-was-baked-in-2022-dot-3))

- 图形为 "ImageConversion "类使用的 JPEG 解码器添加了预防措施，以防止利用 LJT-01-003 漏洞拒绝服务。Unity 现在会在解码 1000 次逐行扫描后自动中止 JPEG 文件的解码。
    (UUM-129186)

- 图形添加了 SystemInfo.SupportsTypedUAVShaderLoadStoreOnGraphicsFormat\(\) 用于在无人机上进行着色器类型加载/存储时检查给定硬件的格式支持。适用于 DX11 和 DX12。
    (UUM-101875)

- 图形修复了 Vulkan swapchain 获取下一幅图像时可能发生的崩溃。
    ([UUM-138508](https://issuetracker.unity3d.com/issues/crash-in-vk-onscreenswapchain-acquirenextimage))

- `图形`: 修正了在 Adreno 设备上使用 GPU 换肤时的崩溃问题。
    ([uum-93243](https://issuetracker.unity3d.com/issues/crash-on-apigles-clearbuffersubdata-when-running-the-player-a-second-time-on-meta-quest-2))

- `图形`: 修正了 Vulkan 编辑器中不正确的线程安全错误检查。
    ([uum-90240](https://issuetracker.unity3d.com/issues/databuffer-getcurrentresourcewriteable-error-is-thrown-in-custom-srp-when-using-vulkan-graphics-api))

- `图形`: 修复了使用 Vulkan 和 GraphicsJobs 时的 mip 流问题。
    (UUM-137032)

- `图形`: 当使用 Vulkan 时，修正了计算换肤伪影或崩溃的问题。
    ([UUM-135988](https://issuetracker.unity3d.com/issues/crash-on-vulkan-plus-mali-when-skinned-mesh-renderer-starts-enabled-off-screen-then-enabled-and-moved-on-screen))

- `图形`: 修正了在某些 Adreno Vulkan 驱动程序上使用未使用顶点属性的着色器时崩溃的问题。
    (UUM-137056)

- `图形`: 当使用金属图形 API 时，当使用动态分辨率与 STP 升频时，修复了图形损坏问题。
    (UUM-136227)

- 图形当使用 Vulkan 时，修正了某些 Adreno 7xx 驱动程序版本上不正确的 UV。
    ([UUM-126477](https://issuetracker.unity3d.com/issues/android-vulkan-the-uv-quad-is-displayed-incorrectly-with-vulkan-on-a-specific-device))

- `图形`: 修正了在 OpenGL 下使用 DXT1 纹理和 1bit alpha 时丢失 alpha 通道的问题。
    ([uum-86650](https://issuetracker.unity3d.com/issues/opengl-alpha-channel-loss-in-dds-textures-when-viewing-them-with-opengl-selected-as-graphics-api))

- `图形"`: 当使用 OpenGL 回读比回读矩形宽的目标纹理时，修正了 ReadPixels。
    ([uum-121817](https://issuetracker.unity3d.com/issues/android-texture2d-dot-readpixels-writes-pixels-into-a-texture-incorrectly-when-used-with-opengles3))

- 图形尽可能使用 `glClear` 而不是 clear quad，以避免在某些较旧的 Android 设备上出现伪影。
    ([uum-135708](https://issuetracker.unity3d.com/issues/visual-artifacts-appear-when-using-clip-method-in-custom-shader-and-running-on-gles))

- `HDRP`: 修正了启用 DRS 检查自定义通行卷时的 NullReferenceException。
    ([uum-136075](https://issuetracker.unity3d.com/issues/errors-thrown-into-the-console-when-adding-certain-custom-passes-to-a-custom-pass-volume-component-if-dynamic-resolution-is-enabled))

- `IL2CPP`: 修正了 libil2cpp 代码中的 C++ 警告。
    (UUM-138294)

- `IL2CPP`: 修正了可能导致生成无效代码的 C++ 指针别名问题。
    ([UUM-132447](https://issuetracker.unity3d.com/issues/ios-stripping-issue-on-xcode-26-when-use-incremental-gc-is-disabled))

- `Linux`: 修正了 "构建并运行 "两次启动 Linux 播放器的问题。
    ([uum-138018](https://issuetracker.unity3d.com/issues/build-and-run-on-ubuntu-opens-two-instances-of-the-player-at-once))

- `Linux`: 修正了因 SDK 对象文件使用超出 SSE2 的功能而导致的旧 CPU 崩溃问题。
    ([uum-137227](https://issuetracker.unity3d.com/issues/linux-crash-on-gl-projectpolygon-when-opening-the-editor-using-an-older-cpu))

- 剖析器修正了在主动记录时加载 Profiler 捕获会将加载的数据与未完成处理的帧混合的问题。
    ([uum-134269](https://issuetracker.unity3d.com/issues/load-profiler-capture-pop-up-window-appears-again-when-selecting-the-same-profiler-capture-for-the-second-time))

- 剖析器修正了在 Vulkan 上无法录制 Profiler 截图的问题。
    (UUM-126495)

- `场景/游戏视图`: 修正了编辑器工具上下文（EditorToolContext）行为，该行为可能会阻止场景中的常规游戏对象选择。
    ([UUM-135908](https://issuetracker.unity3d.com/issues/unable-to-select-a-gameobject-in-scene-view-when-using-a-custom-editor-tool))

- `脚本编写在 ScriptingCoverage`: FilterRecordedMethods 中添加了主线程保护，以确保脚本重载时的线程安全。
    ([uum-137724](https://issuetracker.unity3d.com/issues/crash-on-mono-jit-runtime-invoke-when-disabling-the-debug-mode-with-the-code-coverage-enabled))

- 序列化修正了一个问题，即在盒式结构对象上调用 `OnAfterDeserialize` 时，修改结构字段会损坏该对象的内存。接口方法调用目标现在指向盒装对象的结构数据。
    ([uum-119163](https://issuetracker.unity3d.com/issues/crash-on-buffer-add-value-full-when-hovering-over-serializedproperty-dot-boxedvalue-in-debug-mode-after-iserializationcallbackreceiver-dot-onafterdeserialize-modifies-value))

- `SRP Core`: 修正了一个问题，即在播放器构建中的 SRP 着色器的 `Awake()` 或 `Start()` 过程中，`Material.FindPass(...)` 返回-1。
    ([uum-101568](https://issuetracker.unity3d.com/issues/material-dot-findpass-returns-1-in-build-when-shader-pass-is-used))

- `用户界面工具包`: 添加了新属性 `UxmlCreateInstanceMethod`。指定在使用 `UxmlElement` 时用于创建实例而非默认构造函数的方法。

- `用户界面工具包为构建器层次结构添加了搜索功能。

- 用户界面工具包为构建器样式表添加了搜索功能。

- 用户界面工具包`: 在 Microsoft Basic 渲染器上禁用 UITK GPU 性能测试。
    (UUM-137559)

- `用户界面工具包`: 修正了使用 "反偏弧编码 "SVG 的 9 片。
    ([UUM-133494](https://issuetracker.unity3d.com/issues/svg-with-antialiased-arc-encoding-and-slices-dont-behave-well))

- `用户界面工具包`: 修正了 Mac 上会在最边缘显示无效像素的角落。
    (UUM-122540)

- `用户界面工具包`: 修正了 SVG Gradient 的覆盖（arcAA\ ）问题。
    ([UUM-115304](https://issuetracker.unity3d.com/issues/gradient-draw-larger-when-a-custom-shader-is-used))

- 用户界面工具包修正了 VectorImage 导入时忽略视口的问题。
    ([uum-133924](https://issuetracker.unity3d.com/issues/svgs-imported-as-antialiased-arc-encodings-do-no-honor-the-svg-provided-viewport))

- `用户界面工具包`: 修复了 SVG 矢量图像未显示视口选项的问题。
    ([uum-138244](https://issuetracker.unity3d.com/issues/viewport-options-are-not-exposed-in-the-inspector-when-svg-is-imported-as-ui-toolkit-vector-image))

- `用户界面工具包`: 修补了某些 T 结点导致的像素缺失。
    ([uum-121344](https://issuetracker.unity3d.com/issues/some-ui-toolkit-pixels-are-transparent-when-not-all-corners-are-rounded))

- `用户界面工具包用户界面工具包测试框架`: 标准化编辑器测试夹具的 panelSize。
    (UUM-133472)

- `URP`: 修正了当 *Color Space* 设置为 *Gamma* 时，on-tile PostPro 与传统 PostPro 的结果不同的问题。
    (UUM-135686)

- `VFX Graph`: 防止在 PrepareVFXRenderNodes 中出现容易崩溃的竞赛条件。
    (UUM-136687)

- `WebGL`: 当项目最大内存大于 2GB 时，修正了 WebGPU 错误。
    (UUM-139633)

- `WebGL`: 更新了 WebGPU 绑定库，进行了一般改进和内存修复。
    (UUM-139098)

- `XR`: 当使用帧缓冲获取复制 MSAA 相机颜色附件时，修正了选择不正确的解析附件的问题。
    ([UUM-132450](https://issuetracker.unity3d.com/issues/the-view-renders-black-when-using-framebuffer-fetch-with-foveated-rendering-in-a-player-for-meta-quest))




## 6000.3.14f1 中软件包的更改

## 更新的软件包

- `com.unity.editorcoroutines`: [1.0.1](https://docs.unity3d.com/Packages/com.unity.editorcoroutines@1.0//changelog/CHANGELOG.html) 到 [1.1.0](https://docs.unity3d.com/Packages/com.unity.editorcoroutines@1.1//changelog/CHANGELOG.html)

- `com.unity.recorder`: [5.1.5](https://docs.unity3d.com/Packages/com.unity.recorder@5.1//changelog/CHANGELOG.html) 到 [5.1.6](https://docs.unity3d.com/Packages/com.unity.recorder@5.1//changelog/CHANGELOG.html)

- `com.unity.services.leaderboards`: [2.3.3](https://docs.unity3d.com/Packages/com.unity.services.leaderboards@2.3//changelog/CHANGELOG.html) 到 [2.3.4](https://docs.unity3d.com/Packages/com.unity.services.leaderboards@2.3//changelog/CHANGELOG.html)

- `com.unity.microsoft.gdk`: [1.5.1](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk@1.5//changelog/CHANGELOG.html) 到 [1.6.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk@1.6//changelog/CHANGELOG.html)

- `com.unity.microsoft.gdk.tools`: [1.5.1](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.tools@1.5//changelog/CHANGELOG.html) 到 [1.6.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.tools@1.6//changelog/CHANGELOG.html)

- `com.unity.microsoft.gdk.discovery`: [1.2.1](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.discovery@1.2//changelog/CHANGELOG.html) 到 [1.3.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.discovery@1.3//changelog/CHANGELOG.html)

- `com.unity.ai.inference`: [2.6.0](https://docs.unity3d.com/Packages/com.unity.ai.inference@2.6//changelog/CHANGELOG.html) 到 [2.6.1](https://docs.unity3d.com/Packages/com.unity.ai.inference@2.6//changelog/CHANGELOG.html)