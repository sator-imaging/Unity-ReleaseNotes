# Unity 6000.0.74f1 LTS
发布于 星期三, 29 四月 2026 10:05:57 GMT
https://unity.com/releases/editor/whats-new/6000.0.74f1

# 6000.0.74f1 中的已知问题

- `6000.0.61f1`: 使用SDF16或SDF32生成字体图集时，tlsf_free崩溃
    ([uum-141061](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-generating-font-atlas-with-sdf16-or-sdf32))

- `6000.0.6f1`: [渲染图][D3D12]当使用带有EnableAsyncCompute(true)和UseTexture的AddComputePass时，D3D12SwapChain::Present崩溃。
    ([uum-140183](https://issuetracker.unity3d.com/issues/rendergraph-d3d12-crash-on-d3d12swapchain-present-when-using-addcomputepass-with-enableasynccompute-true-and-usetexture))

- `6000.5.0a4,6000.0.66f1,6000.3.4f1,6000.4.0b4`: 在 Builds 中，ShaderVariantCollection.variantCount 和 ShaderVariantCollection.shaderCount 返回 0
    ([uum-137398](https://issuetracker.unity3d.com/issues/shadervariantcollection-dot-variantcount-and-shadervariantcollection-dot-shadercount-returns-0-in-builds))

- `IL2CPP`: [iOS] [Android] IL2CPP 生成过程中外部库泛型失败
    ([uum-125284](https://issuetracker.unity3d.com/issues/ios-android-external-library-generics-fail-during-il2cpp-build))

- `Metal`: 命令缓冲区超时错误后游戏冻结
    ([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- `金属"`: MacOS 在编辑器中的最小项目在播放模式下出现卡顿
    ([uum-85256](https://issuetracker.unity3d.com/issues/macos-stutters-in-a-minimal-project))

在 List<T> 结构中使用嵌套 [SerializeReference] 字段时，"core::base_hash_set "崩溃
    ([uum-139722](https://issuetracker.unity3d.com/issues/crash-on-core-base-hash-set-when-using-nested-serializereference-fields-in-list-structures))

使用 DX12 时，在场景视图中选择游戏对象时 CheckDeviceStatus 崩溃
    ([uum-138597](https://issuetracker.unity3d.com/issues/crash-on-checkdevicestatus-when-selecting-gameobjects-in-the-scene-view-while-using-dx12))

在空白 URP 项目中重新编译时，VisualElement 中的编辑器内存泄漏
    ([uum-138000](https://issuetracker.unity3d.com/issues/editor-memory-leak-in-visualelement-when-recompiling-in-a-blank-urp-project))



# 6000.0.74f1 发行说明

## 更改

- 音频在基于 Chromium 的网络浏览器上，内存压缩设置默认为加载时解压缩，以避免内存泄漏。
    ([uum-136929](https://issuetracker.unity3d.com/issues/detached-audio-source-is-not-released-from-browser-memory-when-audio-stops-playing-in-webgl-player))



## 修复

- `2D`: 添加了对使用 2D 渲染器的 Unity Recorder 的支持。
    (UUM-136415)

- `Android`: 修复了在 Android 上使用 URP 时，如果在播放器设置中禁用了深度/模版缓冲区，则会发生崩溃的问题。
    ([UUM-109005](https://issuetracker.unity3d.com/issues/android-player-crashes-on-vk-renderpasses-getpackedrenderpass-when-using-vulkan-graphics-api-in-a-specific-project))

- `Android`: 修复了在 Pixel 10 上使用丢弃或剪辑着色器时出现伪影的问题。
    (UUM-139019)

- 音频修正了在非 Chromium 网页浏览器上使用压缩内存设置时的内存泄漏问题。
    ([UUM-136929](https://issuetracker.unity3d.com/issues/detached-audio-source-is-not-released-from-browser-memory-when-audio-stops-playing-in-webgl-player))

- 编辑器修正了当游戏帧率远低于视频帧率时播放视频文件时出现的无限跳帧循环。
    ([uum-131279](https://issuetracker.unity3d.com/issues/video-framerate-is-not-restored-when-trying-to-raise-it-after-lowering-it-to-10-fps))

- 编辑器修正了一个问题，即如果升级`EditorSettings.asset`失败，或手动还原/修改了`EditorSettings.asset`，则在禁用`Domain Reload on Enter Play Mode`的情况下，仍会发生 "Domain Reload on Play Mode"。
    ([uum-138521](https://issuetracker.unity3d.com/issues/enterplaymodeoptions-doesnt-take-effect-if-user-manually-modifies-m-enterplaymodeoptionsenabled-to-0))

- 编辑器修正了一个问题，即如果升级`EditorSettings.asset`失败，或手动还原/修改，则在禁用`Domain Reload on Enter Play Mode`时，仍会发生 Domain Reload。
    ([uum-138521](https://issuetracker.unity3d.com/issues/enterplaymodeoptions-doesnt-take-effect-if-user-manually-modifies-m-enterplaymodeoptionsenabled-to-0))

- 编辑器修正了与 TextCore 一起使用下划线时超出范围的异常。
    ([uum-137906](https://issuetracker.unity3d.com/issues/ui-builder-windows-text-rendering-breaks-when-using-rich-text-combined-with-an-underlined-emoji))

- `编辑器`: 为 Vulkan 编辑器提前设置软件包权限，以支持所有本地插件用例。
    ([uum-135157](https://issuetracker.unity3d.com/issues/vulkan-native-graphics-plugins-load-after-graphics-device-initialization-in-editor-when-placed-in-packages))

- 编辑器对 IL2CPP 相关文件进行签名，以防止杀毒软件将未签名的二进制文件标记为可疑文件而引发潜在问题。
    (UUM-137463)

- 编辑器解决在使用OpenGL ES的Mali GPU上使用stencil-only格式时崩溃的问题。
    ([UUM-111344](https://issuetracker.unity3d.com/issues/android-crash-on-startup-when-depth-stencil-format-is-set-to-s8-uint))

- 图形界面修正了一个 Bug，当没有一个场景同时包含阴影投射混合光和烘焙光贴图或光探针时，阴影遮罩或减法着色器变体会被错误地剥离。
    ([uum-127288](https://issuetracker.unity3d.com/issues/baked-shadows-are-missing-when-loading-a-scene-additively-and-lighting-was-baked-in-2022-dot-3))

- 图形为 "ImageConversion "类使用的 JPEG 解码器添加了预防措施，以防止利用 LJT-01-003 漏洞拒绝服务。Unity 现在会在解码 1000 次逐行扫描后自动中止 JPEG 文件的解码。
    (UUM-129186)

- 图形修复了 Vulkan swapchain 获取下一幅图像时可能发生的崩溃。
    ([UUM-138508](https://issuetracker.unity3d.com/issues/crash-in-vk-onscreenswapchain-acquirenextimage))

- `图形`: 修正了 Vulkan 编辑器中不正确的线程安全错误检查。
    ([uum-90240](https://issuetracker.unity3d.com/issues/databuffer-getcurrentresourcewriteable-error-is-thrown-in-custom-srp-when-using-vulkan-graphics-api))

- `图形`: 修正了在 DX12、Metal 和传统 Vulkan 设备中使用 ScalableBufferManager 时 MSAA CameraDepthTexture 大小调整不一致的问题，以及修正了在构建独立或 Android 播放器时抛出隐式截断向量类型着色器警告的问题。
    ([uum-100367](https://issuetracker.unity3d.com/issues/android-ios-macos-inconsistent-cameradepthtexture-behavior-when-using-scalablebuffermanager-across-devices))

- 图形修正了使用 Vulkan 时的计算换肤假象或崩溃问题。
    ([uum-135988](https://issuetracker.unity3d.com/issues/crash-on-vulkan-plus-mali-when-skinned-mesh-renderer-starts-enabled-off-screen-then-enabled-and-moved-on-screen))

- `图形`: 当使用 Vulkan 时，修正了 Pixel 10 上的实例化问题。
    (UUM-139629)

- `图形`: 修复了在 OpenGL 中使用 DXT1 纹理和 1bit alpha 时丢失 alpha 通道的问题。
    ([UUM-86650](https://issuetracker.unity3d.com/issues/opengl-alpha-channel-loss-in-dds-textures-when-viewing-them-with-opengl-selected-as-graphics-api))

- `图形"`: 当使用 OpenGL 回读比回读矩形宽的目标纹理时，修正了 ReadPixels。
    ([uum-121817](https://issuetracker.unity3d.com/issues/android-texture2d-dot-readpixels-writes-pixels-into-a-texture-incorrectly-when-used-with-opengles3))

- 图形删除了发布版本中关于 GraphicsStateCollection.Warmup 在使用不支持的图形 API 时回退到传统着色器变体加载的重复日志信息。
    (UUM-138841)

- 图形尽可能使用 glClear 代替 clear quad，以避免在某些较旧的 Android 设备上出现伪影。
    ([UUM-135708](https://issuetracker.unity3d.com/issues/visual-artifacts-appear-when-using-clip-method-in-custom-shader-and-running-on-gles))

- `HDRP`: 修正了添加自定义渲染通道后 DLSS &amp; FSR2 黑屏的问题。
    ([uum-113720](https://issuetracker.unity3d.com/issues/shadowmappass-breaks-the-game-view-when-dlss-is-enabled))

- `HDRP`: 修正彩色金字塔失真后 _ColorPyramidUvScaleAndLimitCurrentFrame 中的 limit.xy 值为空的问题。
    ([uum-130925](https://issuetracker.unity3d.com/issues/hdrp-liquid-sample-custom-injection-pass-breaks-transparency-and-refraction-when-set-to-before-post-process))

- 软件包在调整大小时为 RagdollWindow 添加了滚动视图支持。
    ([uum-139914](https://issuetracker.unity3d.com/issues/the-ragdoll-builder-window-has-no-scrollbar-making-elements-unreachable-unless-the-window-is-resized))

- 软件包管理器修正了更改软件包缓存位置会导致 "TLS 分配器 ALLOC_TEMP_MAIN 有未释放的分配 "错误反复出现在编辑器日志中的问题。
    ([uum-131286](https://issuetracker.unity3d.com/issues/tls-allocator-alloc-temp-tls-underlying-allocator-alloc-temp-main-has-unfreed-allocations-dot-dot-dot-error-when-changing-the-packages-cache-location-folder))

- `粒子"`: 防止嵌套子发射器的 TrailModule::Update 崩溃。
    ([uum-131142](https://issuetracker.unity3d.com/issues/crash-on-trailmodule-update-when-loading-particle-systems-with-trails-module-enabled-from-assetbundles))

- `粒子"`: 防止在使用嵌套子发射器与出生生成条件时发生崩溃。
    ([uum-115382](https://issuetracker.unity3d.com/issues/unity-player-crashes-on-unityplayer-unitymain-and-an-access-violation-reading-location-error-in-particlesystem-emit-occurs-when-running-player-with-debugallocator-and-using-particle-systems-with-a-complex-hierarchical-structure))

- 场景/游戏视图修正了一个 Bug，当在游戏模式中使用 PlayModeWindow.SetViewType 时，该 Bug 可能会导致编辑器崩溃。
    ([uum-139011](https://issuetracker.unity3d.com/issues/crash-on-repaintcontroller-renderplaymodeviewcameras-when-entering-play-mode-and-playmodewindow-dot-setviewtype-being-called-at-end-of-frame))

- `脚本"`: 在 ScriptingCoverage::FilterRecordedMethods 中添加了主线程保护，以确保重载脚本时的线程安全。
    ([uum-137724](https://issuetracker.unity3d.com/issues/crash-on-mono-jit-runtime-invoke-when-disabling-the-debug-mode-with-the-code-coverage-enabled))

- `URP`: 修正了 URP DepthBlit 样本，在不需要时防止手动深度解析。
    ([uum-134993](https://issuetracker.unity3d.com/issues/non-multisampled-texture-binding-errors-are-logged-when-running-the-depthblit-urp-scene-with-msaa-enabled-on-vulkan))

- `WebGL`: 修正了在 WebGPU 和 WebGL 下使用地形细节网格时出现的渲染错误。
    ([uum-91734](https://issuetracker.unity3d.com/issues/webgl-player-fails-to-render-scene-when-terrain-with-detail-mesh-is-added-and-webgpu-graphics-api-is-used))

- `WebGL`: 修正了 `R16UNorm`、`R16SNorm`、`RG16UNorm`、`RG16SNorm`、`RGBA16UNorm` 和 `RGBA16SNorm` 被错误地声明为可过滤的问题。
    ([uum-139873](https://issuetracker.unity3d.com/issues/r16unorm-texture-usage-fails-for-webgpu))

- `WebGL`: 修正了切换全屏状态时的 WebGL 控制台警告。
    ([uum-139208](https://issuetracker.unity3d.com/issues/webgl-console-warnings-switching-fullscreen))




## 6000.0.74f1 中软件包的更改

## 更新的软件包

- `com.unity.editorcoroutines`: [1.0.0](https://docs.unity3d.com/Packages/com.unity.editorcoroutines@1.0//changelog/CHANGELOG.html) 到 [1.1.0](https://docs.unity3d.com/Packages/com.unity.editorcoroutines@1.1//changelog/CHANGELOG.html)

- `com.unity.xr.arcore`: [6.0.6](https://docs.unity3d.com/Packages/com.unity.xr.arcore@6.0//changelog/CHANGELOG.html) 到 [6.0.7](https://docs.unity3d.com/Packages/com.unity.xr.arcore@6.0//changelog/CHANGELOG.html)

- `com.unity.xr.arfoundation`: [6.0.6](https://docs.unity3d.com/Packages/com.unity.xr.arfoundation@6.0//changelog/CHANGELOG.html) 到 [6.0.7](https://docs.unity3d.com/Packages/com.unity.xr.arfoundation@6.0//changelog/CHANGELOG.html)

- `com.unity.xr.arkit`: [6.0.6](https://docs.unity3d.com/Packages/com.unity.xr.arkit@6.0//changelog/CHANGELOG.html) 到 [6.0.7](https://docs.unity3d.com/Packages/com.unity.xr.arkit@6.0//changelog/CHANGELOG.html)

- `com.unity.xr.core-utils`: [2.5.3](https://docs.unity3d.com/Packages/com.unity.xr.core-utils@2.5//changelog/CHANGELOG.html) 到 [2.6.0](https://docs.unity3d.com/Packages/com.unity.xr.core-utils@2.6//changelog/CHANGELOG.html)

- `com.unity.dt.app-ui`: [1.3.5](https://docs.unity3d.com/Packages/com.unity.dt.app-ui@1.3//changelog/CHANGELOG.html) 到 [1.3.6](https://docs.unity3d.com/Packages/com.unity.dt.app-ui@1.3//changelog/CHANGELOG.html)

- `com.unity.microsoft.gdk`: [1.5.1](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk@1.5//changelog/CHANGELOG.html) 到 [1.6.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk@1.6//changelog/CHANGELOG.html)

- `com.unity.microsoft.gdk.tools`: [1.5.1](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.tools@1.5//changelog/CHANGELOG.html) 到 [1.6.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.tools@1.6//changelog/CHANGELOG.html)

- `com.unity.microsoft.gdk.discovery`: [1.2.1](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.discovery@1.2//changelog/CHANGELOG.html) 到 [1.3.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.discovery@1.3//changelog/CHANGELOG.html)

- `com.unity.ai.inference`: [2.5.0](https://docs.unity3d.com/Packages/com.unity.ai.inference@2.5//changelog/CHANGELOG.html) 至 [2.6.1](https://docs.unity3d.com/Packages/com.unity.ai.inference@2.6//changelog/CHANGELOG.html)