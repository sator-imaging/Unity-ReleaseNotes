# Unity 6000.3.13f1 LTS
发布于 星期三, 08 四月 2026 09:59:17 GMT
https://unity.com/releases/editor/whats-new/6000.3.13f1

# 6000.3.13f1 中的已知问题

- `6000.0.17f1`: 使用 DX12 时在场景视图中选择游戏对象时 CheckDeviceStatus 崩溃
    ([uum-138597](https://issuetracker.unity3d.com/issues/crash-on-checkdevicestatus-when-selecting-gameobjects-in-the-scene-view-while-using-dx12))

- `6000.2.0a10`: 首次打开项目时，TexturesD3D12::CreateTextureInternal()崩溃
    ([uum-135024](https://issuetracker.unity3d.com/issues/crash-on-checkdevicestatus-when-opening-a-project-for-the-first-time))

- `6000.2.0b1`: 使用 DisableTypeTree 从资产包加载 VFX 对象时，因 "CachedReader::OutOfBoundsError "而崩溃
    ([uum-137538](https://issuetracker.unity3d.com/issues/crash-on-cachedreader-outofboundserror-when-loading-vfx-object-from-an-asset-bundle-with-disabletypetree))

- `6000.3.0a3`: 当使用最小近剪辑平面值制作自定义反射探针时，Umbra::QueryExt::queryStaticShadowCasters 会崩溃
    ([uum-137250](https://issuetracker.unity3d.com/issues/crash-on-umbra-queryext-querystaticshadowcasters-when-baking-a-custom-reflection-probe-with-the-minimum-near-clipping-planes-value))

- `6000.5.0a4,6000.0.66f1,6000.3.4f1,6000.4.0b4`: 在 Builds 中，ShaderVariantCollection.variantCount 和 ShaderVariantCollection.shaderCount 返回 0
    ([uum-137398](https://issuetracker.unity3d.com/issues/shadervariantcollection-dot-variantcount-and-shadervariantcollection-dot-shadercount-returns-0-in-builds))

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

在 vk::OnscreenSwapChain::AcquireNextImage 中崩溃
    ([uum-138508](https://issuetracker.unity3d.com/issues/crash-in-vk-onscreenswapchain-acquirenextimage))

当 ConfigurableJoint 使用 JointProjectionMode.PositionAndRotation 且连接的 Rigidbody 从运动模式切换为非运动模式时，在 ConstraintProjectionTree::projectionTreeBuildStep 中崩溃
    ([uum-135394](https://issuetracker.unity3d.com/issues/crash-on-constraintprojectiontree-projectiontreebuildstep-when-configurablejoint-uses-jointprojectionmode-dot-positionandrotation-and-connected-rigidbody-switches-from-kinematic-to-non-kinematic))

在空白 URP 项目中重新编译时，VisualElement 中的编辑器内存泄漏
    ([uum-138000](https://issuetracker.unity3d.com/issues/editor-memory-leak-in-visualelement-when-recompiling-in-a-blank-urp-project))

新版本发布时没有最新的 URP 和 HDRP 模板版本
    ([uum-137426](https://issuetracker.unity3d.com/issues/new-releases-are-shipped-without-the-newest-urp-and-hdrp-template-versions))

在 DirectX 12 独占全屏模式下切换焦点时播放器崩溃
    ([uum-134743](https://issuetracker.unity3d.com/issues/player-crash-when-switching-focus-in-exclusive-fullscreen-mode-with-directx-12))



# 6000.3.13f1 发布说明

## 功能

- 版本控制为项目浏览器和检查器中的文件夹添加了 "添加到源代码控制 "和 "撤销更改 "操作。

- 版本控制新增了分支资源管理器，用于可视化和导航分支。

- 版本控制为所有分割器位置添加了跨窗口重载和会话的持久性。

- 版本控制在合并视图中添加了部分应用搁置的支持。

- 版本控制添加了重命名分支和标签的 F2 快捷键。



## 改进

- 搜索提高了在启用 "深度索引 "后合并大型项目的搜索索引工件时的性能。
    (UUM-133013)



## 应用程序接口变更

- `音频已添加`: 已为 ScriptableAudioPipeline ControlContext 添加 API，以方便发现系统何时正在配置。
    ([uum-133107](https://issuetracker.unity3d.com/issues/configure-is-not-working-for-nested-generators))



## 更改

- `Android`: 将 GameActivity 库从 3.0.5 更新至 4.4.0。

- 文档将快速入门超链接指向 ECS 功能集 Unity 文档页面。

- 版本控制在状态栏中添加了变更集和标签图标。

- 版本控制从 Unity Hub 打开项目时延迟工作区的创建。

- 版本控制改进了跨对话框的文本字段焦点行为，使键盘工作流程更加一致。

- 版本控制改进了 "待更改 "视图中的空状态。

- 版本控制防止错误地将项目连接到不同的组织。

- 版本控制更新了新项目初始化，以执行完整的初始签入。

- 版本控制更新了 macOS 隐藏快捷键为 Cmd+Shift+H。



## 修复

- `2D`: 修正了 2D 渲染器不支持 RSUV 的问题。为 2D 渲染器添加 ShaderUserVariable 支持。
    (UUM-131692)

- `自适应性能"`: 修复了 gc 分配。
    (UUM-136604)

- `AI`: 在 Linux 上，NavMeshAgent 检查器的 "Agent Type "属性中的 "Open Agent Settings...（打开代理设置...）"选项会出错，并且不会打开__Navigation__窗口。
    ([uum-131690](https://issuetracker.unity3d.com/issues/opening-agent-settings-window-when-choosing-agent-type-throws-invalidoperationexception-error-in-the-console-window))

- `Android`: 修复了光标锁定时的鼠标输入问题（GameActivity 4.4.0 升级部分）。
    (UUM-91677)

- `Android`: 滑动触摸屏键盘时，输入框中不会出现乱码（GameActivity 4.4.0升级版的一部分）。
    ([UUM-116283](https://issuetracker.unity3d.com/issues/android-ui-toolkit-gameactivity-swipe-typed-word-overrides-a-last-entry-with-an-inputfield-with-a-large-amount-of-characters))

- `Android`: `AndroidApplication.onConfigurationChanged`将正确反映 GameActivity 上的语言/国家更改。

- `Asset Import`: 修正了关键字::LocalSpace::查找时因访问过期资源而导致的编辑器崩溃。
    ([uum-133882](https://issuetracker.unity3d.com/issues/crash-on-keywords-localspace-find-when-reimporting-specific-assets))

- 编辑器调整了质量等级列表显示，以匹配其他可重排列表。
    ([uum-136310](https://issuetracker.unity3d.com/issues/reorderable-list-containing-quality-levels-in-the-build-profiles-window-uses-different-padding-sizes-compared-with-the-player-settings-graphics-api-reorderable-list))

- 编辑器限制发布设置/WebAssembly 语言特点的内存设置，使其不能小于 0。
    ([uum-134687](https://issuetracker.unity3d.com/issues/memory-related-fields-in-the-webassembly-language-features-can-be-set-to-the-negative-numbers))

- 编辑器修正了 LinuxEditor 中使用 MemoryProfiler 时产生的 TLS 假阳性错误。
    ([uum-136317](https://issuetracker.unity3d.com/issues/linux-tls-allocator-alloc-temp-tls-underlying-allocator-alloc-temp-main-has-unfreed-allocations-dot-dot-dot-error-and-warnings-are-thrown-when-selecting-a-snapshot-in-memory-profiler))

- 编辑器修正了一个内存泄漏，在该泄漏中，用于截取 profiler 屏幕截图的 RenderTexture 对象未被正确销毁。
    ([uum-137789](https://issuetracker.unity3d.com/issues/rendertarget-memory-usage-is-cumulative-and-is-creating-a-memory-leak-when-changing-scenes))

- 编辑器修正了 QualitySettingsEditor 在每次更新调用时读取项目中所有构建配置文件的性能问题。
    (UUM-136760)

- 编辑器修正了自定义工具栏中 IMGUI 元素的错误。
    (UUM-135117)

- 编辑器修正了升级 Win64 插件的旧元文件会禁用插件的问题。
    ([UUM-137610](https://issuetracker.unity3d.com/issues/win64-cpu-is-set-to-none-when-applying-changes-to-plugin-where-the-meta-has-the-serializedversion-2))

- 编辑器修正了资产存储生成搜索命题的问题。
    ([uum-133640](https://issuetracker.unity3d.com/issues/pressing-plus-button-in-search-field-in-asset-store-search-window-throws-formatexception-error-in-the-console-window))

- `编辑器`: 固定资产商店快速点击导航。
    ([uum-133625](https://issuetracker.unity3d.com/issues/nullreferenceexception-errors-thrown-in-the-console-when-holding-arrow-key-down-to-navigate-through-not-fully-loaded-assets-in-search-asset-store-window))

- `编辑器`: 修复了在准备过程中导入工作程序崩溃，查找回退着色器。
    ([uum-107712](https://issuetracker.unity3d.com/issues/assetimportworkers-crash-when-changing-shader-precision-model))

- 编辑器修正了构建自动化模态无法添加更新构建配置文件的问题。
    (UUM-136372)

- 编辑器修正了同时在多个动画窗口之间同步预览模式的问题。
    (UUM-136817)

- 编辑器修正了播放器设置中的标签截断问题。
    ([UUM-136316](https://issuetracker.unity3d.com/issues/the-use-dxgi-flip-model-swapchain-for-d3d11-settings-label-is-not-truncated-when-viewing-player-settings-in-a-build-profile))

- `编辑器"`: 修正了在对 WinEditor 进行 DragDrop 操作时，鼠标移动窗口（mouseOverWindow）不更新的问题。
    ([uum-137200](https://issuetracker.unity3d.com/issues/gameobject-deletion-fails-when-deleting-gameobject-after-dragging-prefab-into-scene-view))

- `编辑器"`: 修正了 ObjectField 在没有对象的情况下显示 "属性 "的问题。
    ([uum-136445](https://issuetracker.unity3d.com/issues/scaler-profile-new-element-has-a-properties-button-in-the-context-menu-that-does-nothing-when-pressed))

- `编辑器"`: 修正了由于编译器优化错误导致的窗口激活时 WindowsEditor 崩溃的问题。
    ([uum-137226](https://issuetracker.unity3d.com/issues/crash-on-containerwindow-doactivateandbringtofront-when-performing-various-actions-in-the-editor))

- `编辑器"`: 修正了使用着色器构建设置时，在每次项目载入时重新导入着色器图资产的问题。
    ([uum-134390](https://issuetracker.unity3d.com/issues/shader-graphs-are-re-imported-every-time-the-project-is-opened-when-dynamic-branching-for-fog-is-enabled))

- `编辑器"`: 修正了一些性能标记函数，使其线程安全。
    (UUM-129081)

- 编辑器修正了为脚本定义和额外编译器参数启用或禁用应用和还原按钮的逻辑。
    ([UUM-126488](https://issuetracker.unity3d.com/issues/empty-lists-can-be-applied-in-additional-compiler-argument-list-in-project-settings))

- 编辑器修正了 WebGL 输入字段在键入后失焦的问题。
    ([uum-137597](https://issuetracker.unity3d.com/issues/input-fields-do-not-maintain-focus-when-they-are-selected-in-a-web-build))

- 编辑器如果无法加载 buildprofilecontext.asset，则重新创建以确保构建配置文件窗口的正常运行。
    ([uum-136377](https://issuetracker.unity3d.com/issues/nullreferenceexception-and-empty-build-profiles-window-when-buildprofilecontext-dot-asset-contains-invalid-script-reference))

- 编辑器在添加所有项目后，删除构建配置文件 "质量设置 "下拉菜单中多余的分隔线。
    ([uum-136313](https://issuetracker.unity3d.com/issues/an-unused-separation-line-is-present-in-the-quality-settings-lists-dropdown-menu-when-there-is-only-one-option-to-choose-from-in-the-build-profiles-window))

- 编辑器解决了 Ubuntu 25.10 及更高版本中 `libxml2` 被重命名的问题。Ubuntu 24.04仍然是编辑器支持的最高版本。
    (UUM-137582)

- `GI"`: 修正了与 URPReflectionProbeSettings 相关的升级错误。
    (UUM-126607)

- 图形当在包含着色器变体的 GraphicsStateCollection 上调用 GetVariants API 时，如果序列化的关键字无效，现在会显示警告。
    (UUM-136009)

- 图形修正了一个问题，即当追踪的 PSO 是在渲染传递之外记录的时候，使用 GraphicsStateCollection API 进行的管道状态对象（PSO）预热在 Metal 上会出现不正确的缓存丢失。
    (UUM-135455)

- 图形修正了当在 DirectX11 中使用 camera.SetTargetBuffers\(\) 而非渲染纹理设置时，GrabPass 无法正确设置矩形大小的问题。
    ([uum-135889](https://issuetracker.unity3d.com/issues/grabpass-does-not-correctly-set-the-rect-size-when-set-up-with-a-camera-dot-settargetbuffers-instead-of-a-render-texture-in-directx11))

- 图形在 Unity 6000.3 和 6000.4 的某些旧版本中，如果加载的集合资产之前已序列化，则某些查询特定着色器变量（ShaderVariants）的 GraphicsStateCollection API 将无法找到正确的变量。
    (UUM-136008)

- 图形\[Vulkan/]（Android）修复了在同一渲染通路子通路中使用深度读取和模版写入操作进行渲染时，在 Mali GPU（非 Midgard）上出现的视觉伪影。解决方法适用于存在该问题的 41.0.0 版之前的驱动程序。
    (UUM-31270)

- `HDRP`: 修正了样本描述中的错误资产引用。
    ([UUM-137827](https://issuetracker.unity3d.com/issues/asset-sg-eye-dot-shadergraph-could-not-be-found-error-thrown-in-the-console-when-clicking-shader-graph-link-in-inspector-window-eye-samples-showcase))

- `内核`: -.
    (UUM-113356)

- `N/A （内部）`: Clarify GeometryUtility.CalculateFrustumPlanes 平面方向。

- `N/A （内部）`: 修正了错误链接。

- `N/A （内部）`: 修正了拼写错误。

- 物理修正了一些问题，当从预制上下文执行时，Rigidbody 组件 API 并不完全安全。
    ([uum-137716](https://issuetracker.unity3d.com/issues/crash-on-physicscommands-physx-bodygetflags-when-changing-rigidbody-interpolation-value-through-api-for-prefab-objects))

- `物理`: 修正了一个问题，即检查器可以将对撞机组件数据（如中心/半径/高度/大小）设置为 +/-无限，这是不有效的，会导致不正确的模拟行为。
    ([uum-136447](https://issuetracker.unity3d.com/issues/invalid-aabb-aabb-errors-are-spammed-when-infinity-value-is-entered-in-collider-component-fields))

- 物理修正了 Rigidbody.centerOfMass 无法序列化设置值的问题。
    ([uum-137716](https://issuetracker.unity3d.com/issues/crash-on-physicscommands-physx-bodygetflags-when-changing-rigidbody-interpolation-value-through-api-for-prefab-objects))

- `物理`: 修正了在预制资产上调用 Rigidbody.constraints 时无法序列化对其设置的值的问题。
    ([uum-137716](https://issuetracker.unity3d.com/issues/crash-on-physicscommands-physx-bodygetflags-when-changing-rigidbody-interpolation-value-through-api-for-prefab-objects))

- `物理 2D"`: 在 "PhysicsBody "和 "PhysicsBodyDefinition "中添加了对 "collisionThreshold "的访问，允许配置何时使用 CCD。
    (UUM-137696)

- `物理 2D"`: 为物理体 "质量"、"转动惯量 "和 "局部质量中心 "添加了缺失的设置器，以补充现有的获取器。
    ([uum-137414](https://issuetracker.unity3d.com/issues/massconfiguration-issues-with-physicsbody))

- `物理 2D"`: 物理铰链连接（PhysicsHingeJoint）现在可以 "解钉"，这样就可以只使用点对点约束来提供旋转约束，从而有效地允许物理体移动，同时只应用旋转约束。
    (UUM-137810)

- `物理 2D"`: 更新了 Box2D 以包含各种错误修复和改进，其中最显著的是接触循环，以提高模拟过程中的接触性能。
    (UUM-137810)

- `物理 2D"`: 在添加已禁用 "PhysicsShapeDefinition.startMassUpdate "的物理体时，确保调用 "PhysicsBody.ApplyMassFromShapes "或 "PhysicsBody.massConfiguration "能够正确配置物理体碰撞检测。
    ([uum-137414](https://issuetracker.unity3d.com/issues/massconfiguration-issues-with-physicsbody))

- 探测器修复了剖析器窗口中捕获列表和时间线视图边界处的渲染假象。
    ([uum-116890](https://issuetracker.unity3d.com/issues/rendering-artefacts-visible-in-the-profiler-window-modules-section-when-capture-list-is-open))

- `阴影图"`: 修正了自定义灯光样本中错误的附加灯光索引。
    ([uum-137007](https://issuetracker.unity3d.com/issues/2-lights-are-rendered-when-8-lights-exist-and-using-custom-lighting-shader-graph-with-forward-or-deferred-rendering))

- `着色器`: 修正了保存着色器时偶尔出现的崩溃。
    ([uum-133627](https://issuetracker.unity3d.com/issues/crash-on-enumeratedisabledkeywordsinvariantsarray-or-unity-xxh32-when-rapidly-saving-shadergraph-or-vfxgraph-changes))

- `SRP 核心`: 提高了 "卷剖面检查器 "窗口的性能。
    (UUM-136456)

- 用户界面工具包修复了一个布局缓存内存泄漏问题，该问题会在长时间高负载时发生。
    (UUM-137552)

- `用户界面工具包`: 修正了图形验证后徽章无法正确显示的问题。
    (UUM-137317)

- `用户界面工具包`: 修复了起始颜色为透明时，边框颜色转换不起作用的问题。
    ([UUM-136876](https://issuetracker.unity3d.com/issues/border-is-not-rendered-when-transition-duration-is-set-and-border-color-is-transparent))

- `用户界面工具包`: 修正进入播放模式后过滤器折叠的问题。
    ([uum-137614](https://issuetracker.unity3d.com/issues/ui-builder-filter-foldout-collapses-when-entering-play-mode-or-docking-the-window))

- `用户界面工具包`: 修正了当提供 libraryPath 时，UI Builder 项目选项卡会呈现重复组的问题。
    ([uum-137536](https://issuetracker.unity3d.com/issues/duplicated-groups-and-incorrect-grouping-in-ui-builder-when-using-uxmlelementattribute-librarypath))

- `用户界面工具包`: 修正了带有 DynamicColor 提示的紧网格精灵不更新背景色调颜色的问题。
    ([uum-136987](https://issuetracker.unity3d.com/issues/button-with-dynamiccolor-doesnt-update-its-unity-background-image-tint-color))

- `URP`: 修正了 Bloom 纹理中的一个问题，即无效的纹理句柄可能会在各执行通道中重复使用，从而导致渲染图执行错误。
    ([uum-137390](https://issuetracker.unity3d.com/issues/crash-in-rendergraph-bloom-following-upgrade-to-unity-6-dot-3-6))

- `版本控制修正了右键单击侧边栏中的 "待处理更改 "时出现的布局异常。

- 版本控制`: 修正了从分支差异打开历史记录时的 NullReferenceException 异常。

- `版本控制修正了逐个变更集差异面板中可能出现的 NullReferenceException。

- 版本控制修复并本地化了签入对话框的进度标签。

- 版本控制修复了 "探索软件库 "窗口中的模糊图标。

- 版本控制修正了 Unity 版本控制窗口中按钮的大小写，以符合 Unity 标准。

- 版本控制修正了分支视图中逐个变更集差异的问题。

- 版本控制`: 修正了分支上下文菜单在表格为空时无法打开的问题。

- `版本控制`: 修正了签入对话框无法自动聚焦注释字段的问题。

- `版本控制`: 修正当表格为空时无法打开标签上下文菜单的问题。

- `版本控制"`: 修复了新建分支按钮在当前选择为变更集或标签时失效的问题。

- `版本控制`: 修复了退出播放模式后状态栏变灰的问题。

- `版本控制修复了 "创建工作区 "过程中的 "统一版本控制 "窗口刷新时不需要移动鼠标的问题。

- 版本控制修正了 Unity 版本控制窗口中验证信息的对齐方式。

- WebGL`: 修正了在使用 WebGPU 和 WebGL 的地形细节网格时出现的渲染错误。
    ([uum-91734](https://issuetracker.unity3d.com/issues/webgl-player-fails-to-render-scene-when-terrain-with-detail-mesh-is-added-and-webgpu-graphics-api-is-used))

- `WebGL`: \在绑定动态偏移无效的情况下，GPU 驻留绘图器实例化可能会失败。
    ([uum-135867](https://issuetracker.unity3d.com/issues/webgpu-error-with-fantasy-kingdom-and-gpu-resident-drawer))

- `WebGL`: \[WebGPU\] 某些纹理格式（如 RG8UNorm）在用作计算着色器的可写纹理时会失败，即使纹理格式_formats_tier1扩展可用。
    ([uum-136007](https://issuetracker.unity3d.com/issues/webgpu-rg8unorm-texture-says-it-doesnt-support-random-writes))

- `XR"`: 修正了在启用纹理压缩目标的情况下构建和运行 Meta Quest 应用程序时出现的问题。
    ([uum-131974](https://issuetracker.unity3d.com/issues/meta-quest-player-stuck-at-splashscreen-when-build-app-bundle-and-split-application-binary-are-enabled-with-multiple-texture-compression-formats))




## 6000.3.13f1 中软件包的更改

## 更新的软件包

- `com.unity.burst`: [1.8.28](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html) 到 [1.8.29](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html)

- `com.unity.collab-proxy`: [2.11.4](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.11//changelog/CHANGELOG.html) 到 [2.12.4](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.12//changelog/CHANGELOG.html)

- `com.unity.purchasing`: [4.14.2](https://docs.unity3d.com/Packages/com.unity.purchasing@4.14//changelog/CHANGELOG.html) 到 [4.15.0](https://docs.unity3d.com/Packages/com.unity.purchasing@4.15//changelog/CHANGELOG.html)

- `com.unity.services.authentication`: [3.6.0](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.6//changelog/CHANGELOG.html) 到 [3.6.1](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.6//changelog/CHANGELOG.html)

- `com.unity.services.vivox`: [16.9.0](https://docs.unity3d.com/Packages/com.unity.services.vivox@16.9//changelog/CHANGELOG.html) 到 [16.10.0](https://docs.unity3d.com/Packages/com.unity.services.vivox@16.10//changelog/CHANGELOG.html)

- `com.unity.test-framework.performance`: [3.2.0](https://docs.unity3d.com/Packages/com.unity.test-framework.performance@3.2//changelog/CHANGELOG.html) 到 [3.4.0](https://docs.unity3d.com/Packages/com.unity.test-framework.performance@3.4//changelog/CHANGELOG.html)

- `com.unity.timeline`: [1.8.11](https://docs.unity3d.com/Packages/com.unity.timeline@1.8//changelog/CHANGELOG.html) 到 [1.8.12](https://docs.unity3d.com/Packages/com.unity.timeline@1.8//changelog/CHANGELOG.html)

- `com.unity.xr.arcore`: [6.3.3](https://docs.unity3d.com/Packages/com.unity.xr.arcore@6.3//changelog/CHANGELOG.html) 到 [6.3.4](https://docs.unity3d.com/Packages/com.unity.xr.arcore@6.3//changelog/CHANGELOG.html)

- `com.unity.xr.arfoundation`: [6.3.3](https://docs.unity3d.com/Packages/com.unity.xr.arfoundation@6.3//changelog/CHANGELOG.html) 至 [6.3.4](https://docs.unity3d.com/Packages/com.unity.xr.arfoundation@6.3//changelog/CHANGELOG.html)

- `com.unity.xr.arkit`: [6.3.3](https://docs.unity3d.com/Packages/com.unity.xr.arkit@6.3//changelog/CHANGELOG.html) 到 [6.3.4](https://docs.unity3d.com/Packages/com.unity.xr.arkit@6.3//changelog/CHANGELOG.html)

- `com.unity.xr.compositionlayers`: [2.3.0](https://docs.unity3d.com/Packages/com.unity.xr.compositionlayers@2.3//changelog/CHANGELOG.html) 到 [2.4.0](https://docs.unity3d.com/Packages/com.unity.xr.compositionlayers@2.4//changelog/CHANGELOG.html)

- `com.unity.xr.meta-openxr`: [2.3.0](https://docs.unity3d.com/Packages/com.unity.xr.meta-openxr@2.3//changelog/CHANGELOG.html) 到 [2.3.1](https://docs.unity3d.com/Packages/com.unity.xr.meta-openxr@2.3//changelog/CHANGELOG.html)

- `com.unity.transport`: [2.7.1](https://docs.unity3d.com/Packages/com.unity.transport@2.7//changelog/CHANGELOG.html) 到 [2.7.2](https://docs.unity3d.com/Packages/com.unity.transport@2.7//changelog/CHANGELOG.html)

- `com.unity.netcode.gameobjects`: [2.10.0](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@2.10//changelog/CHANGELOG.html) 到 [2.11.0](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@2.11//changelog/CHANGELOG.html)

- `com.unity.ai.navigation`: [2.0.11](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html) 到 [2.0.12](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html)

- `com.unity.polyspatial`: [3.1.1](https://docs.unity3d.com/Packages/com.unity.polyspatial@3.1//changelog/CHANGELOG.html) 到 [3.1.4](https://docs.unity3d.com/Packages/com.unity.polyspatial@3.1//changelog/CHANGELOG.html)

- `com.unity.polyspatial.visionos`: [3.1.1](https://docs.unity3d.com/Packages/com.unity.polyspatial.visionos@3.1//changelog/CHANGELOG.html) 至 [3.1.4](https://docs.unity3d.com/Packages/com.unity.polyspatial.visionos@3.1//changelog/CHANGELOG.html)

- `com.unity.polyspatial.xr`: [3.1.1](https://docs.unity3d.com/Packages/com.unity.polyspatial.xr@3.1//changelog/CHANGELOG.html) 至 [3.1.4](https://docs.unity3d.com/Packages/com.unity.polyspatial.xr@3.1//changelog/CHANGELOG.html)

- `com.unity.polyspatial.extensions`: [3.1.1](https://docs.unity3d.com/Packages/com.unity.polyspatial.extensions@3.1//changelog/CHANGELOG.html) 到 [3.1.4](https://docs.unity3d.com/Packages/com.unity.polyspatial.extensions@3.1//changelog/CHANGELOG.html)

- `com.unity.xr.visionos`: [3.1.1](https://docs.unity3d.com/Packages/com.unity.xr.visionos@3.1//changelog/CHANGELOG.html) 到 [3.1.4](https://docs.unity3d.com/Packages/com.unity.xr.visionos@3.1//changelog/CHANGELOG.html)

- `com.unity.ai.inference`: [2.5.0](https://docs.unity3d.com/Packages/com.unity.ai.inference@2.5//changelog/CHANGELOG.html) 到 [2.6.0](https://docs.unity3d.com/Packages/com.unity.ai.inference@2.6//changelog/CHANGELOG.html)