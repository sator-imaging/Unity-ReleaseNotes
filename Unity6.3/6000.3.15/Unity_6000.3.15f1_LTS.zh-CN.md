# Unity 6000.3.15f1 LTS
发布于 Fri, 08 May 2026 05:39:58 GMT
https://unity.com/releases/editor/whats-new/6000.3.15f1

# 6000.3.15f1 中的已知问题

- `6000.0.61f1`: 使用 SDF16 或 SDF32 生成字体图集时 tlsf_free 崩溃
    ([uum-141061](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-generating-font-atlas-with-sdf16-or-sdf32))

- `6000.0.6f1`: [渲染图][D3D12]当使用带有EnableAsyncCompute(true)和UseTexture的AddComputePass时，D3D12SwapChain::Present崩溃。
    ([uum-140183](https://issuetracker.unity3d.com/issues/rendergraph-d3d12-crash-on-d3d12swapchain-present-when-using-addcomputepass-with-enableasynccompute-true-and-usetexture))

- `6000.5.0a4,6000.0.66f1,6000.3.4f1,6000.4.0b4`: 在 Builds 中，ShaderVariantCollection.variantCount 和 ShaderVariantCollection.shaderCount 返回 0
    ([uum-137398](https://issuetracker.unity3d.com/issues/shadervariantcollection-dot-variantcount-and-shadervariantcollection-dot-shadercount-returns-0-in-builds))

- `金属"`: 命令缓冲区超时错误后游戏冻结
    ([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- `金属"`: MacOS 在编辑器中的最小项目在播放模式下出现卡顿
    ([uum-85256](https://issuetracker.unity3d.com/issues/macos-stutters-in-a-minimal-project))

当 DX12 图形应用程序接口在图形应用程序接口列表中排在第一位时，没有使用它
    ([uum-141555](https://issuetracker.unity3d.com/issues/dx12-graphics-api-is-not-used-when-it-is-first-in-the-graphics-api-list))

在打开子场景的预制模式下禁用子游戏对象时，材质会移动到预制中的其他游戏对象上
    ([uum-139663](https://issuetracker.unity3d.com/issues/materials-move-to-other-gameobjects-in-a-prefab-when-disabling-a-child-gameobject-in-prefab-mode-with-an-open-subscene))



# 6000.3.15f1 发行说明

## 改进

- `编译系统将捆绑的 7-Zip 更新至 26.01 版本。

- iOS`: 添加了播放器设置切换以启用金属显示链接（无需使用代码）。

- `iOS`: 在严重/临界热状态下切换到 ca 显示链接。



## API 更改

- `物理已添加`: 为 `Collision` 类型添加了 `angularVelocity` 属性。
    ([uum-140799](https://issuetracker.unity3d.com/issues/unable-to-access-linear-slash-angular-velocity-inside-collision-in-order-to-use-relativevelocity))

- `物理`: 新增： 为`ContactPairHeader`类型添加了`bodyAngularVelocity`属性。
    ([uum-140799](https://issuetracker.unity3d.com/issues/unable-to-access-linear-slash-angular-velocity-inside-collision-in-order-to-use-relativevelocity))

- `物理新增`: 为`ContactPairHeader`类型添加了`bodyLinearVelocity`属性。
    ([uum-140799](https://issuetracker.unity3d.com/issues/unable-to-access-linear-slash-angular-velocity-inside-collision-in-order-to-use-relativevelocity))

- `物理新增`: 为`碰撞`类型添加了`linearVelocity`属性。
    ([uum-140799](https://issuetracker.unity3d.com/issues/unable-to-access-linear-slash-angular-velocity-inside-collision-in-order-to-use-relativevelocity))

- `物理`: 新增： 为`ContactPairHeader`类型添加了`otherBodyAngularVelocity`属性。
    ([uum-140799](https://issuetracker.unity3d.com/issues/unable-to-access-linear-slash-angular-velocity-inside-collision-in-order-to-use-relativevelocity))

- `物理新增`: 为`ContactPairHeader`类型添加了`otherBodyLinearVelocity`属性。
    ([uum-140799](https://issuetracker.unity3d.com/issues/unable-to-access-linear-slash-angular-velocity-inside-collision-in-order-to-use-relativevelocity))

- `物理新增`: 为`Collision`类型添加了`thisAngularVelocity`属性。
    ([uum-140799](https://issuetracker.unity3d.com/issues/unable-to-access-linear-slash-angular-velocity-inside-collision-in-order-to-use-relativevelocity))

- `物理`: 新增： 为`碰撞`类型添加了`thisArticulationBody`属性。
    ([uum-140799](https://issuetracker.unity3d.com/issues/unable-to-access-linear-slash-angular-velocity-inside-collision-in-order-to-use-relativevelocity))

- `物理`: 新增： 为`碰撞`类型添加了`thisBody`属性。
    ([uum-140799](https://issuetracker.unity3d.com/issues/unable-to-access-linear-slash-angular-velocity-inside-collision-in-order-to-use-relativevelocity))

- `物理`: 已添加： 为`碰撞`类型添加了`thisGameObject`属性。
    ([uum-140799](https://issuetracker.unity3d.com/issues/unable-to-access-linear-slash-angular-velocity-inside-collision-in-order-to-use-relativevelocity))

- `物理`: 已添加： 为`碰撞`类型添加了`thisLinearVelocity`属性。
    ([uum-140799](https://issuetracker.unity3d.com/issues/unable-to-access-linear-slash-angular-velocity-inside-collision-in-order-to-use-relativevelocity))

- `物理`: 新增： 为`碰撞`类型添加了`thisRigidbody`属性。
    ([uum-140799](https://issuetracker.unity3d.com/issues/unable-to-access-linear-slash-angular-velocity-inside-collision-in-order-to-use-relativevelocity))

- `物理`: 已添加： 为`碰撞`类型添加了`thisTransform`属性。
    ([uum-140799](https://issuetracker.unity3d.com/issues/unable-to-access-linear-slash-angular-velocity-inside-collision-in-order-to-use-relativevelocity))



## 修复

- `2D`: 修复了打开特定项目时 ShaderPropertySheet::FindPropertyIndex 崩溃的问题。
    ([uum-110537](https://issuetracker.unity3d.com/issues/crash-on-shaderpropertysheet-findpropertyindex-when-opening-a-specific-project))

- `2D`: 当使用 URP 2D 时，修复了预览相机中光照和阴影缺失的问题。
    (UUM-139229)

- 辅助功能修正了无障碍节点在绕过最大 ID 值后以重复 ID 创建的问题。
    ([UUM-137871](https://issuetracker.unity3d.com/issues/accessibilityhierarchy-throws-an-exception-when-node-id-reaches-int-dot-maxvalue))

- `自适应性能`: 将自适应性能重新计算的描述符大小限制为 1，以避免在渲染纹理大小为零时出现错误。
    ([uum-138049](https://issuetracker.unity3d.com/issues/urp-rendergraph-throws-rendertexturedesc-height-must-be-greater-than-zero-when-camera-pixel-height-becomes-0-due-to-small-window-resolution-and-fractional-viewport-rect))

- 人工智能修正了当使用 navAgent.Move 移动时，NavMeshAgent 被卡在方框障碍物的角落上的问题。
    ([uum-136684](https://issuetracker.unity3d.com/issues/navmeshagent-gets-stuck-on-the-corner-of-a-box-shape-navmeshobstacle-when-it-is-moved-with-navagent-dot-move))

- `Android`: 当控制器将 L2/R2 报告为按钮事件而不是轴事件时，修正了 Switch Pro 游戏手柄触发器在 Android 上不起作用的问题。
    (UUM-139567)

- 动画修正了在 Animator 窗口中选择短循环动画过渡时出现 ArgumentOutOfRangeException 的问题。
    ([UUM-139812](https://issuetracker.unity3d.com/issues/argumentoutofrangeexception-is-thrown-when-selecting-a-transition-to-an-animation-shorter-than-3-frames-with-loop-time-enabled))

- `DX12`: 修正了大型场景中 D3D12 栅栏的缓慢内存泄漏。
    (UUM-140429)

- `DX12`: 确保我们不会访问负索引的数组。
    (UUM-134479)

- 编辑器在用户界面生成器的类型选择器中添加了 `None`。
    ([UUM-137289](https://issuetracker.unity3d.com/issues/none-data-source-type-option-is-missing-when-opening-select-type-dot-dot-dot-in-ui-builder-bindings))

- 编辑器复制到剪贴板适用于包含特殊字符（如 \{ \}）的查询。
    ([uum-137347](https://issuetracker.unity3d.com/issues/save-to-clipboard-for-search-query-that-contains-a-function-block-throws-a-formatexception-error))

- 编辑器修正了嵌套标签在 ATG 中不起作用的问题。
    (UUM-139569)

- 编辑器修正了与 TextCore 一起使用下划线时超出范围的异常。
    ([UUM-137906](https://issuetracker.unity3d.com/issues/ui-builder-windows-text-rendering-breaks-when-using-rich-text-combined-with-an-underlined-emoji))

- `编辑器"`: 修正了 LinuxEditor 中锚预设用户界面不响应 Shift/Alt 修改器键的问题。
    ([uum-137598](https://issuetracker.unity3d.com/issues/linux-shift-slash-alt-modifier-keys-are-not-recognized-in-anchor-presets-when-adjusting-rect-transform))

- `编辑器"`: 修正了枚举值的多重编辑。
    ([uum-138913](https://issuetracker.unity3d.com/issues/cant-change-the-shape-of-multiple-lights-at-the-same-time-using-lighting-search))

- `编辑器"`: 修正自适应性能设置中提供商名称列表偏离中心的问题。
    ([uum-136419](https://issuetracker.unity3d.com/issues/the-provider-name-text-is-off-centered-in-the-adaptive-performance-settings))

- `编辑器"`: 修复了布局表和替换表在域重载时泄漏的问题。
    ([uum-138000](https://issuetracker.unity3d.com/issues/editor-memory-leak-in-visualelement-when-recompiling-in-a-blank-urp-project))

- `编辑器"`: 修正了在窗口间切换时视图无法正确重新聚焦的问题。
    ([uum-139948](https://issuetracker.unity3d.com/issues/cannot-interact-with-gameobjects-in-the-hierarchy-window-by-using-shortcuts-or-edit-menu-when-selecting-a-gameobject-in-the-hierarchy-with-a-select-window-opened))

- `编辑器"`: 修正了 `DrawText` 不能以提供的颜色绘制。
    ([uum-137907](https://issuetracker.unity3d.com/issues/color-parameter-is-ignored-when-creating-dynamic-text-in-a-ui-document-with-drawtext))

- 编辑器为 IL2CPP 相关文件签名，以防止杀毒软件将未签名的二进制文件标记为可疑文件。
    (UUM-137463)

- 编辑器所有光类型都支持撤消。
    ([UUM-136891](https://issuetracker.unity3d.com/issues/light-type-slash-mode-changes-are-not-undone-with-ctrl-plus-z-shortcut-when-edited-from-lighting-search-window))

- 编辑器解决在使用 OpenGL ES 的 Mali GPU 上使用纯模板格式时崩溃的问题。
    ([uum-111344](https://issuetracker.unity3d.com/issues/android-crash-on-startup-when-depth-stencil-format-is-set-to-s8-uint))

- `嵌入式Linux`: 修正了回调中的嵌套窗口异步操作。
    (UUM-138651)

- `引擎诊断`: 修正了当启用 CrashReportingSettings.captureEditorExceptions 时，编辑器异常未报告给引擎诊断的问题。
    ([uum-136672](https://issuetracker.unity3d.com/issues/diagnostics-does-not-report-editor-exceptions-when-using-crashreportingsettings-dot-captureeditorexceptions))

- `GI"`: 修正了一个 Bug，当场景包含 UV 布局面积为零的网格时，使用 xAtlas 会导致光图打包失败。
    ([uum-139715](https://issuetracker.unity3d.com/issues/crash-on-xatlas-internal-pack-atlas-findchartlocation-bruteforce-when-generating-the-lighting))

- 图形界面修正了一个 Bug，当使用 xAtlas 打包器时，具有未参照顶点位置的网格有时会在烘焙过程中导致崩溃。
    ([uum-138494](https://issuetracker.unity3d.com/issues/crash-with-multiple-stacktraces-when-building-lighting-in-a-specific-scene))

- `GI"`: 抑制了 UnifiedRT TraceRay 着色器中虚假的 FXC 警告。
    ([uum-139001](https://issuetracker.unity3d.com/issues/switching-platforms-will-trigger-shader-related-warnings-tracetransparentrays))

- `GI`: UnifiedRT： 修复了一个问题，即在播放器构建中，`RayTracingRenderPipelineResources`必须为公共资源。
    ([uum-137604](https://issuetracker.unity3d.com/issues/unifiedraytracing-raytracingrenderpipelineresources-being-internal-prevents-loading-raytracingresources-in-the-player))

- 图形修复了在激活地形的项目中单击 "加载渲染文档 "时崩溃的问题。
    ([uum-99314](https://issuetracker.unity3d.com/issues/crash-on-d3d12descriptorcache-deallocate-or-vkgetinstanceprocaddr-when-loading-renderdoc-in-a-specific-scene))

- `图形`: 修复了在 DX12、Metal 和传统 Vulkan 设备中使用 ScalableBufferManager 时 MSAA CameraDepthTexture 大小调整不一致的问题，以及修复了在构建单机版或 Android 播放器时抛出隐式截断向量类型着色器警告的问题。
    ([uum-100367](https://issuetracker.unity3d.com/issues/android-ios-macos-inconsistent-cameradepthtexture-behavior-when-using-scalablebuffermanager-across-devices))

- 图形修正了虚拟纹理剖析器模块的帮助按钮在具有多种像素密度的多显示器设置上的缩放问题。
    ([uum-137763](https://issuetracker.unity3d.com/issues/virtual-texturing-documentation-button-is-oversized-and-not-consistent-with-other-editor-documentation-buttons-when-virtual-texturing-module-is-selected-in-the-profiler-window))

- `图形"`: 修复了使用 Vulkan 时 Pixel 10 上的实例化问题。
    (UUM-139629)

- `图形`: 修复了在 Direct3D 上导入 `R16G16B16` 格式纹理时的问题。
    ([UUM-104117](https://issuetracker.unity3d.com/issues/texture-displays-visual-artifacts-and-has-a-broken-aspect-ratio-when-it-is-imported-in-rgb-48-bit-format))

- `图形`: 修正了为统一缓冲区绑定传递无效绑定槽时 OpenGLES 崩溃的问题。
    (UUM-138897)

- 图形修正了流控制器组件文档的链接。
    ([UUM-139928](https://issuetracker.unity3d.com/issues/missing-documentation-page-opens-when-clicking-open-reference-button-on-streaming-controller-component))

- `图形"`: 修正了虚拟纹理剖析器模块文档的链接。
    ([uum-137763](https://issuetracker.unity3d.com/issues/virtual-texturing-documentation-button-is-oversized-and-not-consistent-with-other-editor-documentation-buttons-when-virtual-texturing-module-is-selected-in-the-profiler-window))

- 图形删除了发布版本中关于 GraphicsStateCollection.Warmup 在使用不支持的图形 API 时回退到传统着色器变体加载的重复日志信息。
    (UUM-138841)

- 图形\[Vulkan\]修正了在深度解析或计算着色器写入 "渲染纹理 "后应用不正确的 "DontCare "加载操作，从而导致出现伪影的问题。
    (UUM-46565)

- `HDRP"`: 修正了一个 Bug，在该 Bug 中，HDRP SSGI 会从屏幕的一侧向另一侧渗色。
    ([UUM-139120](https://issuetracker.unity3d.com/issues/lighting-leaks-from-right-and-top-edges-to-left-and-bottom-edges-when-screen-space-global-illumination-uses-ray-tracing-in-hdrp))

- `HDRP`: 修正了渲染调试器的一个问题，即 *Freeze Camera For Culling* 下拉菜单只显示 *None* 作为选项。
    ([uum-137626](https://issuetracker.unity3d.com/issues/none-is-only-present-when-using-hdrp-rendering-debuggers-freeze-camera-for-culling-dropdown))

- `HDRP"`: 修正了彩色金字塔失真后 _ColorPyramidUvScaleAndLimitCurrentFrame 中的 null limit.xy 值。
    ([uum-130925](https://issuetracker.unity3d.com/issues/hdrp-liquid-sample-custom-injection-pass-breaks-transparency-and-refraction-when-set-to-before-post-process))

- `iOS`: 修复了多次从 GameCenter 加载成就时的崩溃。
    (UUM-138417)

- 内核修正了从终结器访问作业系统时在关机过程中崩溃的问题。
    ([UUM-128777](https://issuetracker.unity3d.com/issues/crash-on-jobqueue-hasjobgroupidcompleted-when-closing-the-editor-while-in-play-mode-on-a-specific-project))

- `Linux`: 修正了 Linux 自动工具链安装程序无法为 Linux Arm64 服务器安装 Arm64 sysroot 的问题。
    (UUM-136647)

- 网络在 Linux 播放器构建中添加了一些缺失的 Mono 配置文件，当尝试使用某些 .NET 网络 API 时（尤其是 `WebRequest`），这些配置文件会导致异常抛出。
    ([uum-135731](https://issuetracker.unity3d.com/issues/webrequest-dot-create-function-fails-with-uri-prefix-is-not-recognized-errors-when-the-project-is-built-for-linux-standalone-or-windows-dedicated-server))

- 网络将 MbedTLS 更新到 3.6.6 版，以解决一些（次要且可能无法利用的）安全漏洞。
    (UUM-140908)

- 软件包在调整大小时为 RagdollWindow 添加了 ScrollView 支持。
    ([UUM-139914](https://issuetracker.unity3d.com/issues/the-ragdoll-builder-window-has-no-scrollbar-making-elements-unreachable-unless-the-window-is-resized))

- 软件包管理器修正了更改软件包缓存位置会导致 "TLS 分配器 ALLOC_TEMP_MAIN 有未释放的分配 "错误反复出现在编辑器日志中的问题。
    ([uum-131286](https://issuetracker.unity3d.com/issues/tls-allocator-alloc-temp-tls-underlying-allocator-alloc-temp-main-has-unfreed-allocations-dot-dot-dot-error-when-changing-the-packages-cache-location-folder))

- 物理修正了网格对撞机组件接收非均匀缩放时处理不当的问题。
    ([uum-139681](https://issuetracker.unity3d.com/issues/mesh-collider-does-not-skew-slash-shear-correctly-when-nested-inside-another-gameobject))

- 物理修正了一个问题，当与 "ArticulationBody "组件碰撞时，如果 "ArticulationBody "组件和 "Collider "组件位于不同的 GameObjects 上，则 "Collision.transform "会返回不正确的 "Transform"。
    ([uum-140799](https://issuetracker.unity3d.com/issues/unable-to-access-linear-slash-angular-velocity-inside-collision-in-order-to-use-relativevelocity))

- `Plugins`: \NVUnityPlugin] 修正了一个 DLSS 抖动和闪烁问题。
    ([uum-134012](https://issuetracker.unity3d.com/issues/game-view-jitters-on-high-frame-rates-when-dlss-is-enabled-and-the-mode-is-set-to-ultra-performance))

- `Profiler`: 更新了 `FrameTimingManager.GetLatestTimings` API，因此当播放器未暂停时，背景时间不会包含在下一个聚焦帧中。
    ([uum-132089](https://issuetracker.unity3d.com/issues/frametimingmanager-dot-getlatesttimings-adds-background-time-to-the-next-focused-frame-when-the-player-is-unfocused))

- `QNX`: 修正了回调中的嵌套窗口异步操作。
    (UUM-138651)

- 场景/游戏视图修正了在播放模式下使用 PlayModeWindow.SetViewType 时可能导致编辑器崩溃的错误。
    ([UUM-139011](https://issuetracker.unity3d.com/issues/crash-on-repaintcontroller-renderplaymodeviewcameras-when-entering-play-mode-and-playmodewindow-dot-setviewtype-being-called-at-end-of-frame))

- `脚本"`: 在装配体定义资产检查器中添加新的空引用条目并单击 "应用 "时，该条目会错误地复制列表中的最后一个条目，而不是保持为空。
    (UUM-119332)

- `阴影图`: 为 `enum` 关键字输入添加了一个设置，允许项目的着色器构建设置覆盖它们。还添加了一个设置，可在 `enum` 中添加一个 `none` 条目。
    (UUM-135644)

- 文字确保 "渐变色 "与 "阴影 "和 "轮廓 "结合使用时有效。
    ([UUM-140065](https://issuetracker.unity3d.com/issues/ui-toolkit-color-gradient-not-applying-to-label-text-when-outline-width-is-set-to-more-than-0))

- `文本`: 修正了当单词包装 sup 和 sub 标记时的 NullReferenceException。
    ([uum-139927](https://issuetracker.unity3d.com/issues/nullreferenceexception-is-thrown-when-resizing-a-text-element-in-the-ui-builder-when-it-contains-sup-or-sub-elements-and-wrap-mode-is-enabled))

- `uGUI`: 修正了在OnValidate事件中使用脚本改变输入框焦点时出现nullReferenceException的问题。
    ([uum-132637](https://issuetracker.unity3d.com/issues/nullreferenceexception-error-is-thrown-when-changing-input-field-focus-via-script-with-custom-validation))

- `uGUI`: 修正了当使用 Tab 键移动焦点时，InputField 无法获取 Hangul\(IME\) （韩文字符）文本的最后一个字符。
    ([uum-126213](https://issuetracker.unity3d.com/issues/inputfield-fails-to-get-the-last-character-of-a-hangul-ime-korean-character-text-when-focus-is-shifted-with-the-tab-key))

- 用户界面工具包修正了在启用可空引用类型时生成属性包代码时的编译错误。
    ([uum-126159](https://issuetracker.unity3d.com/issues/createproperty-on-nullable-generic-types-causes-compilation-error-when-using-a-non-nullable-type))

- `用户界面工具包`: 修正了作为纹理导入时 SVG 预览的 alpha 值。
    ([uum-137765](https://issuetracker.unity3d.com/issues/project-window-preview-icon-is-fully-black-when-a-black-svg-shape-is-imported-and-set-as-a-texture2d))

- `用户界面工具包`: 修正了一个 IndexOutOfRangeException 异常，以及在编辑文字阴影模糊半径和另一个属性后使用 Ctrl+S/Cmd+S 保存时模糊半径值还原的问题。
    ([uum-139822](https://issuetracker.unity3d.com/issues/indexoutofrangeexception-is-thrown-and-blur-radius-value-reverts-when-saving-after-modifying-blur-radius-and-another-property-in-ui-builder))

- 用户界面工具包修正了一个问题，即使用 ToSource 绑定模式的绑定会在 UI 更改后更新 UI。
    ([uum-120902](https://issuetracker.unity3d.com/issues/uitk-textfield-value-is-overwritten-incorrectly-by-the-converter-result-when-binding-mode-is-set-to-to-source))

- `用户界面工具包`: 修正了一个问题，即通过运行时绑定系统绑定到 UnityEngine.Object 的属性无法将 null 设回源。
    ([uum-134627](https://issuetracker.unity3d.com/issues/ui-toolkit-throws-warning-and-fails-to-clear-references-when-fields-are-not-typed-as-unityengine-dot-object))

- 用户界面工具包修正了为 `StyleSheet` 导出颜色时精度不够的问题。
    ([uum-127703](https://issuetracker.unity3d.com/issues/ui-builder-background-color-picker-alpha-values-are-set-to-even-numbers-when-saving-alpha-value-as-an-odd-number))

- 用户界面工具包修正了打包的精灵可能进入动态图集的问题。
    ([uum-137771](https://issuetracker.unity3d.com/issues/9-sliced-sprite-assigned-as-background-in-a-ui-toolkit-visual-element-is-rendered-blurry))

- `用户界面工具包`: 修正了在 UI 创建器层次结构中搜索时无法在 UI 创建器中添加元素的问题。
    ([uum-138485](https://issuetracker.unity3d.com/issues/unable-to-add-elements-in-ui-builder-when-searching-in-ui-builder-hierarchy))

- `用户界面工具包`: 修正了 SVGImporter 和 FilterFunctionDefinition 的文档帮助链接。
    ([uum-139170](https://issuetracker.unity3d.com/issues/clicking-in-inspector-for-svg-importer-opens-missing-documentation-page-instead-of-relevant-manual))

- `用户界面工具包`: 修正了导入的矢量图像资产检查器标题上缺少的文档链接。
    ([uum-139560](https://issuetracker.unity3d.com/issues/vector-image-asset-documentation-link-is-missing))

- `用户界面工具包`: 修正了 `[HelpURL]`中的嵌套手册主题解析到 "page missing "文档页面的问题。
    ([uum-140384](https://issuetracker.unity3d.com/issues/sorry-dot-dot-dot-that-page-seems-to-be-missing-is-shown-on-the-browser-when-clicking-the-help-icon-on-a-panel-renderer-component))

- `用户界面工具包`: 固定搜索模式在任何结果元素被操作时退出。
    ([uum-138487](https://issuetracker.unity3d.com/issues/search-mode-is-exited-when-any-resulting-element-is-manipulated-with))

- `用户界面工具包`: 修正了删除陈旧数据时 TryRemoveItem 无效操作异常。
    ([uum-137639](https://issuetracker.unity3d.com/issues/an-invalidoperationexception-error-is-thrown-when-tryremoveitem-is-used-with-rebuildtree-set-to-false))

- `URP`: 已添加文档，说明自适应性能可在运行时覆盖贴花绘制距离。
    ([uum-138945](https://issuetracker.unity3d.com/issues/urp-decals-become-invisible-when-over-1000-units-away-from-the-camera))

- `URP`: 为在着色器图形中编写的自定义 UITK 着色器添加了立体实例化支持。
    ([uum-131994](https://issuetracker.unity3d.com/issues/spi-xr-custom-ui-toolkit-ui-shader-graph-materials-only-render-in-one-eye-when-using-single-pass-instanced-rendering))

- `URP`: 修正了 URP DepthBlit 样本，在不需要时防止手动深度解析。
    ([uum-134993](https://issuetracker.unity3d.com/issues/non-multisampled-texture-binding-errors-are-logged-when-running-the-depthblit-urp-scene-with-msaa-enabled-on-vulkan))

- 视频在基于 Windows 的平台上打开分割的 MP4 文件时，添加了控制台警告，因为不支持这种媒体类型。
    ([uum-132004](https://issuetracker.unity3d.com/issues/video-player-does-not-throw-an-error-when-playing-a-video-with-unsupported-encoding-settings))

- `WebGL`: 修正了 `R16UNorm`、`R16SNorm`、`RG16UNorm`、`RG16SNorm`、`RGBA16UNorm` 和 `RGBA16SNorm` 被错误地声明为可过滤的问题。
    ([uum-139873](https://issuetracker.unity3d.com/issues/r16unorm-texture-usage-fails-for-webgpu))

- `WebGL`: 修正了切换全屏状态时的 WebGL 控制台警告。
    ([uum-139208](https://issuetracker.unity3d.com/issues/webgl-console-warnings-switching-fullscreen))

- `WebGL`: \修正了由于 CoreCopy 着色器导致的 MSAA 纹理的 RenderGraph 错误。
    ([uum-133838](https://issuetracker.unity3d.com/issues/webgpu-errors-when-corecopy-shader-is-used-to-copy-an-msaa-texture))

- `WebGL`: \确保 WebCam 视频在移动设备上方向正确。
    ([uum-139017](https://issuetracker.unity3d.com/issues/ios-web-webgpu-webcamtextures-camera-orientation-is-fixed-relative-to-the-phones-right-edge))

- `XR`: 修正了在 URP 中使用多通道 XR 渲染模式时无法正确设置内置着色器常量 unity_StereoEyeIndex，这会影响 Skybox/Panoramic 等着色器，即使使用 3D 布局选项也无法显示为立体效果。
    ([uum-120719](https://issuetracker.unity3d.com/issues/stereoscopic-skybox-renders-as-monoscopic-when-using-multi-pass-render-mode-in-xr-plugin-while-using-urp))




## 6000.3.15f1 中的软件包变更

## 更新的软件包

- `com.unity.netcode`: [1.10.0](https://docs.unity3d.com/Packages/com.unity.netcode@1.10//changelog/CHANGELOG.html) 到 [1.13.1](https://docs.unity3d.com/Packages/com.unity.netcode@1.13//changelog/CHANGELOG.html)

- `com.unity.services.user-reporting`: [2.0.14](https://docs.unity3d.com/Packages/com.unity.services.user-reporting@2.0//changelog/CHANGELOG.html) 到 [2.0.15](https://docs.unity3d.com/Packages/com.unity.services.user-reporting@2.0//changelog/CHANGELOG.html)

- `com.unity.xr.core-utils`: [2.5.3](https://docs.unity3d.com/Packages/com.unity.xr.core-utils@2.5//changelog/CHANGELOG.html) 到 [2.6.0](https://docs.unity3d.com/Packages/com.unity.xr.core-utils@2.6//changelog/CHANGELOG.html)

- `com.unity.netcode.gameobjects`: [2.11.0](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@2.11//changelog/CHANGELOG.html) 到 [2.11.1](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@2.11//changelog/CHANGELOG.html)

- `com.unity.polyspatial`: [3.1.4](https://docs.unity3d.com/Packages/com.unity.polyspatial@3.1//changelog/CHANGELOG.html) 到 [3.1.5](https://docs.unity3d.com/Packages/com.unity.polyspatial@3.1//changelog/CHANGELOG.html)

- `com.unity.polyspatial.visionos`: [3.1.4](https://docs.unity3d.com/Packages/com.unity.polyspatial.visionos@3.1//changelog/CHANGELOG.html) 至 [3.1.5](https://docs.unity3d.com/Packages/com.unity.polyspatial.visionos@3.1//changelog/CHANGELOG.html)

- `com.unity.polyspatial.xr`: [3.1.4](https://docs.unity3d.com/Packages/com.unity.polyspatial.xr@3.1//changelog/CHANGELOG.html) 至 [3.1.5](https://docs.unity3d.com/Packages/com.unity.polyspatial.xr@3.1//changelog/CHANGELOG.html)

- `com.unity.polyspatial.extensions`: [3.1.4](https://docs.unity3d.com/Packages/com.unity.polyspatial.extensions@3.1//changelog/CHANGELOG.html) 到 [3.1.5](https://docs.unity3d.com/Packages/com.unity.polyspatial.extensions@3.1//changelog/CHANGELOG.html)

- `com.unity.xr.visionos`: [3.1.4](https://docs.unity3d.com/Packages/com.unity.xr.visionos@3.1//changelog/CHANGELOG.html) 到 [3.1.5](https://docs.unity3d.com/Packages/com.unity.xr.visionos@3.1//changelog/CHANGELOG.html)

- `com.unity.asset-manager-for-unity`: [1.10.0](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.10//changelog/CHANGELOG.html) 到 [1.11.0](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.11//changelog/CHANGELOG.html)

- `com.unity.web.stripping-tool`: [1.2.1](https://docs.unity3d.com/Packages/com.unity.web.stripping-tool@1.2//changelog/CHANGELOG.html) 到 [1.3.0](https://docs.unity3d.com/Packages/com.unity.web.stripping-tool@1.3//changelog/CHANGELOG.html)

新增**软件包**

- [com.unity.platformtoolkit.steam@1.0.2](https://docs.unity3d.com/Packages/com.unity.platformtoolkit.steam@1.0//changelog/CHANGELOG.html)

- [com.unity.platformtoolkit.playgamesservices@1.0.1](https://docs.unity3d.com/Packages/com.unity.platformtoolkit.playgamesservices@1.0//changelog/CHANGELOG.html)

- [com.unity.platformtoolkit.gdk@1.0.1](https://docs.unity3d.com/Packages/com.unity.platformtoolkit.gdk@1.0//changelog/CHANGELOG.html)

- [com.unity.platformtoolkit.gamekit@1.0.1](https://docs.unity3d.com/Packages/com.unity.platformtoolkit.gamekit@1.0//changelog/CHANGELOG.html)

- [com.unity.platformtoolkit@1.0.1](https://docs.unity3d.com/Packages/com.unity.platformtoolkit@1.0//changelog/CHANGELOG.html)