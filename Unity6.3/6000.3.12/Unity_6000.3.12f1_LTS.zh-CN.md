# Unity 6000.3.12f1 LTS
发布于 Wed, 25 Mar 2026 11:55:21 GMT
https://unity.com/releases/editor/whats-new/6000.3.12f1

# 6000.3.12f1 中的已知问题

- `6000.2.0a10`: 首次打开项目时，TexturesD3D12::CreateTextureInternal()崩溃
    ([uum-135024](https://issuetracker.unity3d.com/issues/crash-on-checkdevicestatus-when-opening-a-project-for-the-first-time))

- `6000.2.0b1`: 使用 DisableTypeTree 从资产包加载 VFX 对象时，因 "CachedReader::OutOfBoundsError "而崩溃
    ([uum-137538](https://issuetracker.unity3d.com/issues/crash-on-cachedreader-outofboundserror-when-loading-vfx-object-from-an-asset-bundle-with-disabletypetree))

- `6000.3.0a3`: 当使用最小近剪切平面值制作自定义反射探针时，Umbra::QueryExt::queryStaticShadowCasters 会崩溃
    ([uum-137250](https://issuetracker.unity3d.com/issues/crash-on-umbra-queryext-querystaticshadowcasters-when-baking-a-custom-reflection-probe-with-the-minimum-near-clipping-planes-value))

- `6000.6.0a1,6000.3.11f1,6000.4.0b12,6000.5.0a9`: 通过预制对象的 API 更改刚体插值时，PhysicsCommands::PhysX::BodyGetFlags 崩溃
    ([uum-137716](https://issuetracker.unity3d.com/issues/crash-on-physicscommands-physx-bodygetflags-when-changing-rigidbody-interpolation-value-through-api-for-prefab-objects))

- 核心运行时实体内容管理 GUID 不稳定，每次播放器构建到不同目录时都会变得不同
    ([uum-129944](https://issuetracker.unity3d.com/issues/entities-contentmanagement-guids-are-unstable-and-become-different-each-time-a-player-is-built-to-a-different-directory))

- `金属"`: 命令缓冲区超时错误后游戏冻结
    ([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- `金属"`: MacOS 在编辑器中的最小项目在播放模式下出现卡顿
    ([uum-85256](https://issuetracker.unity3d.com/issues/macos-stutters-in-a-minimal-project))

当 ConfigurableJoint 使用 JointProjectionMode.PositionAndRotation 且连接的 Rigidbody 从运动模式切换为非运动模式时，ConstraintProjectionTree::projectionTreeBuildStep 会崩溃
    ([uum-135394](https://issuetracker.unity3d.com/issues/crash-on-constraintprojectiontree-projectiontreebuildstep-when-configurablejoint-uses-jointprojectionmode-dot-positionandrotation-and-connected-rigidbody-switches-from-kinematic-to-non-kinematic))

新版本发布时没有最新的 URP 和 HDRP 模板版本
    ([uum-137426](https://issuetracker.unity3d.com/issues/new-releases-are-shipped-without-the-newest-urp-and-hdrp-template-versions))

在 DirectX 12 独占全屏模式下切换焦点时播放器崩溃
    ([uum-134743](https://issuetracker.unity3d.com/issues/player-crash-when-switching-focus-in-exclusive-fullscreen-mode-with-directx-12))



# 6000.3.12f1 发布说明

## 功能

- 用户界面工具包在 UIToolkit 测试框架中添加了对世界空间内容的 `simulate.Click` 支持。



## 改进

- 文档添加了指向 Memory Profiler 软件包的直接链接。

- `Documentation`: 在内存管理文档中添加了有关清洁和脏页管理的信息。

- 安装程序由于优化了压缩策略，Windows 上的安装程序现在最多可减少 60% 的时间。
    (UUM-136633)



## API 更改

- `实体图形已废弃`: 实体图形已不再支持 OpenGL ES。虽然图形应用程序接口本身仍是一个有效的选择，但在未来的 Unity 版本中，实体图形包将不再支持它。

- `iOS`: 已添加： 已添加 iPhone 17e 设备生成枚举和屏幕剪裁。



## 修复

- `2D`: 修复了一个问题，即当展开磁贴调色板画笔选取叠加时，画笔选取列表项的初始化高度低于最小尺寸。
    ([uum-132593](https://issuetracker.unity3d.com/issues/saved-picks-list-items-are-initialised-with-a-lower-height-than-the-minimum-size-when-the-tile-palette-brush-pick-overlay-is-expanded))

- `2D`: 修正了一个问题，即当使用滑块减小拾取尺寸时，画笔拾取列表项会变得畸形，导致列表被切断。
    ([uum-132606](https://issuetracker.unity3d.com/issues/saved-tile-palette-brush-list-items-become-malformed-causing-the-list-to-become-cut-off-when-decreasing-the-pick-size-with-the-slider))

- `2D`: 修正了在调整拾取大小并将视图模式切换为网格后，画笔拾取名称会消失的问题。
    ([uum-132598](https://issuetracker.unity3d.com/issues/saved-tile-palette-brush-names-disappear-after-adjusting-the-size-of-the-picks-and-switching-view-mode-to-grid))

- `2D`: 修正了不允许销毁资产的问题，以避免在创建第二个瓷砖调色板画笔拾取资产时出现数据丢失错误。
    ([uum-132608](https://issuetracker.unity3d.com/issues/destroying-assets-is-not-permitted-to-avoid-data-loss-error-thrown-when-creating-a-second-tile-palette-brush-pick-asset))

- `2D`: 修复了保存大量画笔拾取时在画笔拾取列表中滚动的问题。
    ([uum-134369](https://issuetracker.unity3d.com/issues/scrolling-in-the-tile-palette-brush-pick-overlay-breaks-when-a-lot-of-brushes-are-saved-and-the-list-view-is-enabled))

- `2D`: 修正了创建磁贴调色板时单元格大小属性接受负值的问题。编辑器现在会将负值设置为 0。
    ([uum-130884](https://issuetracker.unity3d.com/issues/tile-palette-allows-negative-manual-cell-size-values-causing-asset-corruption-and-assertion-failed-on-expression-errors))

- `2D`: 修复了阴影投射器 2d 剔除。
    ([uum-135640](https://issuetracker.unity3d.com/issues/2d-freeform-light-shadows-disappear-when-light-center-is-offset-from-shape-bounds))

- `自适应性能`: 为缩放器配置文件名称长度添加了限制（256 字），以避免过长的名称冻结编辑器。
    ([uum-136422](https://issuetracker.unity3d.com/issues/the-editor-freezes-indefinitely-when-copy-pasting-large-amounts-of-characters-into-new-scaler-profile-name-field-in-the-adaptive-performance-settings))

- `自适应性能`: 修正了自适应性能的*记录频率*设置，使其不再接受负值。
    ([uum-133890](https://issuetracker.unity3d.com/issues/adaptive-performance-logging-frequency-can-be-set-to-a-negative-number))

- 动画修复了当头像的手骨无效时崩溃的问题。
    ([uum-136330](https://issuetracker.unity3d.com/issues/crash-on-mecanim-skeleton-skeletonsetdof-when-entering-play-mode-in-a-specific-scene-1))

- 文档删除了对 UnityEngine.Cache 类的 4GB 限制的提及。下载 AssetBundle 时缓存的最大大小受 Cache.maximumAvailableStorageSpace 值或物理磁盘空间的限制，以较低者为准。如果未设置，该值将是可用磁盘空间。
    (UUM-129965)

- `DX12`: 修复了当 `CommandBuffer.SetRenderTarget` 使用无效深度片时，在绑定渲染目标时崩溃的问题。
    (UUM-130121)

- `DX12`: 修复了在恢复绘制到之前绑定为计算着色器 SRV 的渲染目标后丢失资源屏障的问题。
    (UUM-127520)

- 编辑器自适应性能模式不再能在播放模式中切换。
    ([UUM-133323](https://issuetracker.unity3d.com/issues/the-referenced-script-unknown-on-this-behaviour-is-missing-warnings-and-scriptablesingleton-already-exists-errors-are-thrown-when-adaptive-performance-is-disabled-in-play-mode))

- `编辑器"`: 为了提高可读性，将动画窗口文本改为始终使用符号距离场(SDF\)渲染。
    ([uum-134486](https://issuetracker.unity3d.com/issues/animator-state-labels-are-not-rendered-correctly-when-using-the-bitmap-renderer-as-the-default-editor-text-renderer))

- 编辑器用括号区分重复的 BuildProfile，例如 Windows \(1\)。
    (UUM-130365)

- 编辑器如果编辑器以批处理模式启动，则不要关闭以恢复场景备份。
    (UUM-136292)

- 编辑器编辑器 "现在可以从预制板实例中正确清除与 "序列化参考 "相关的未使用重载。
    ([UUM-135932](https://issuetracker.unity3d.com/issues/prefabs-remove-unused-overrides-fails-to-clean-up-overrides-when-the-managed-instance-type-in-serializereference-is-changed))

- 编辑器修正了在特定情况下出现的 4 帧内存分配器警告。
    ([uum-86868](https://issuetracker.unity3d.com/issues/a-memory-leak-occurs-when-selecting-the-console-window-and-the-inspector-window-covers-the-game-view-window-when-specific-ui-elements-are-displayed-in-it))

- 编辑器修正了 USS 样式验证中无法识别制表符是空白的问题。
    ([uum-135915](https://issuetracker.unity3d.com/issues/warning-expected-end-of-value-but-found-is-shown-when-inserting-a-blank-line-between-opacity-and-scale-in-a-uss-file))

- 编辑器修正了 Linux 下可能导致光标图标状态不正确的问题。
    ([uum-112638](https://issuetracker.unity3d.com/issues/mouse-cursor-does-not-revert-to-the-default-mouse-cursor-when-pressing-the-add-column-button-in-the-search-window))

- 编辑器修正了一个与 ATG 从右向左 (RTL\) 输入的边缘删除和退格相关的问题。
    ([uum-134654](https://issuetracker.unity3d.com/issues/ui-toolkit-backspace-tries-to-delete-the-character-to-the-left-of-the-pointer-when-the-language-direction-is-set-to-rtl-and-the-text-generator-type-is-set-to-advanced))

- 编辑器修正了在 Linux 上重置布局时编辑器窗口尺寸不保留的问题。
    (UUM-131233)

- 编辑器修正了一个问题，即在切换*覆盖Windows、Mac、Linux*后，播放器设置图标尺寸和保留不被保留。
    ([UUM-131965](https://issuetracker.unity3d.com/issues/icon-override-texture2d-fields-in-the-player-settings-window-are-not-square-and-do-not-retain-data-after-disabling))

- 编辑器修正了在 "项目设置 "窗口中移除搜索过滤器会完全高亮显示部分文本的问题。
    ([uum-134769](https://issuetracker.unity3d.com/issues/all-text-in-the-project-settings-window-is-still-tinted-white-after-deleting-text-in-the-search-window))

- 编辑器修正了一个问题，即传统动画剪辑的换行模式选项无法正确显示。
    (UUM-135008)

- 编辑器修正了 Linux 编辑器在覆盖同名文件时不会提示的问题。
    ([UUM-134937](https://issuetracker.unity3d.com/issues/linux-no-file-already-exists-pop-up-thrown-when-saving-shader-variants-with-an-already-existing-name-from-build-profiles-or-project-settings-window))

- 编辑器修正了 "AddComponentMenu "中的一个问题，即具有相似路径片段的项目不会被正确分组，而是会被赋予各自的类别。
    ([uum-135817](https://issuetracker.unity3d.com/issues/physics-components-are-ungrouped-in-components-menu-and-each-physics-component-shown-separately-in-inspector-window-after-installing-unity-physics-package))

- 编辑器修正了当 FormerlySerializedAs 与类型中的字段碰撞时应用预制件属性修改的问题。
    ([uum-135039](https://issuetracker.unity3d.com/issues/object-reference-is-saved-on-an-incorrect-property-when-formerlyserializedas-is-used-on-an-overridden-prefab-variant-field))

- `编辑器"`: 修正了 UIBuilder 预览中的 ATG 警告。
    ([uum-136362](https://issuetracker.unity3d.com/issues/an-error-is-thrown-when-using-a-static-font-and-editor-text-generator-type-is-set-to-advanced))

- 编辑器修正了 TextCore 中的中日韩换行。
    ([uum-135887](https://issuetracker.unity3d.com/issues/cjk-text-goes-outside-of-the-bounds-of-a-label-in-ui-builder-when-wrapping-is-enabled))

- 编辑器修正了构建配置文件窗口中错误信息不能正确反映安装环境的外观问题。
    (UUM-112981)

- 编辑器修正了在 TextCore 中使用中日韩语言时的崩溃问题。
    ([UUM-136683](https://issuetracker.unity3d.com/issues/editor-freezes-when-rendering-wrapped-text-inside-japanese-parentheses-in-too-small-of-a-space))

- `编辑器"`: 修正在标准文本中使用粗体样式时找不到全局回退的问题。
    ([uum-136612](https://issuetracker.unity3d.com/issues/synthetic-bold-applies-to-a-label-instead-of-bold-font-weight-when-using-fallback-font-asset))

- `编辑器"`: 修正了 "图形设置 "部分的错位标签。
    (UUM-135081)

- 编辑器修复了在 MacEditor 中连续拖动鼠标时，场景视图最大化快捷键无法恢复视图的问题。
    ([UUM-134463](https://issuetracker.unity3d.com/issues/scene-view-cant-be-minimised-using-the-shortcut-when-it-was-maximised-using-a-shortcut-in-the-flythrough-mode))

- `编辑器"`: 修正了模块详情面板控制器脚本示例。

- 编辑器当通过代码修改时，脚本定义不再需要通过用户界面手动应用。
    ([uum-129228](https://issuetracker.unity3d.com/issues/build-profiles-modified-by-script-require-manual-apply-when-the-build-profiles-window-is-open))

- 编辑器脚本定义 "的 "复制定义 "按钮现在可以正确地从选定的列表中复制定义。
    (UUM-133917)

- 编辑器自适应性能设置文件不再可通过检查器用户界面访问。
    ([UUM-133313](https://issuetracker.unity3d.com/issues/keys-and-values-lists-in-the-adaptive-performance-general-settings-have-plus-buttons-that-are-active-but-do-nothing-when-clicked))

- `编辑器"`: 自适应性能设置文件不再可以通过检查器用户界面访问。
    ([uum-133314](https://issuetracker.unity3d.com/issues/adaptive-performance-general-settings-version-property-is-set-to-6000-dot-3-on-all-unity-editor-versions))

- `编辑器UI 工具包测试框架`: 修复 EditorWindowUITestFixture 以支持测试期间的域重载。
    (UUM-136644)

- `引擎诊断`: 修复了诊断原生崩溃报告上不正确的时间戳。
    (UUM-135436)

- `引擎诊断`: 修正了 usymtool 缺少某些日志输出的问题。
    (UUM-136272)

- `GI`: 修正了在使用 xAtlas lightmap packer 时某些畸形网格崩溃的问题。
    ([UUM-133550](https://issuetracker.unity3d.com/issues/crash-when-generating-lighting-using-the-xatlas-packing-method-in-a-specific-scene))

- `GI`: 修正了 xAtlas TaskScheduler 工作线程中的挂起问题。
    (UUM-133340)

- `GI`: 修正了 xAtlas TaskScheduler 工作线程中的挂起。
    (UUM-133352)

- `图形`: 修正了英伟达驱动更新后 SystemInfo.supportsInlineRayTracing 变为 false 的问题。
    ([UUM-137132](https://issuetracker.unity3d.com/issues/raytracing-updating-nv-graphics-drivers-to-595-dot-79-causes-systeminfo-dot-supportsinlineraytracing-to-become-false))

- `图形`: 修正了在某些 Android 设备上使用实例化时的地形接缝问题。
    (UUM-131277)

- `图形`: 将子通道最大数量的内部限制提高到 16。
    ([UUM-128596](https://issuetracker.unity3d.com/issues/number-of-srp-renderpass-subpasses-is-limited-to-8))

- `图形`: 确保内建RP blit copy 输出 float4 颜色（而不是 fxed4，后者在金属上被转换为 half4，导致 u16 或 f32 数据截断）。
    ([uum-128591](https://issuetracker.unity3d.com/issues/terrain-heightmap-loses-precision-on-android-and-ios-when-the-heightmap-texture-is-blitted-to-a-rendertexture-using-the-default-blit-shader))

- `HDRP"`: 如果nonMSAAColorBuffer和colorBuffer指向同一个纹理，自定义传递不会同时读取它们。
    ([uum-133557](https://issuetracker.unity3d.com/issues/game-view-turns-black-with-render-graph-and-invalidoperationexception-errors-when-forward-only-lit-shader-mode-and-msaa-are-enabled))

- `HDRP`: 修正了 VolumeProfile 在某些情况下可能无法收集所有组件类型的问题。
    (UUM-136181)

- 输入修正了 IOHIDDevice_GetUsage 中的无效长缓冲指针。
    ([UUM-135043](https://issuetracker.unity3d.com/issues/silicon-crash-on-os-unfair-recursive-lock-lock-with-options-when-opening-a-project-while-the-razer-synapse-app-is-open))

- `iOS`: 修正了在应用程序已运行时通过自定义 URL 方案或通用链接打开应用程序，或在某些情况下通过深度链接从冷启动启动应用程序时未调用 Application.deepLinkActivated 的问题。
    ([uum-135497](https://issuetracker.unity3d.com/issues/ios-application-dot-deeplinkactivated-does-not-get-invoked-while-app-is-running-when-uiapplicationscenemanifest-is-added-in-info-dot-plist))

- `iOS`: 仅在键盘布局发生变化时报告键盘布局，从而提高了性能。
    ([uum-134845](https://issuetracker.unity3d.com/issues/ios-high-cpu-load-when-device-keyboard-is-open))

- `许可证绕过权限缓存从软件包管理器进行查询，以确保结果准确。

- macOS`: 修正了退出时偶尔崩溃的问题。
    ([uum-136306](https://issuetracker.unity3d.com/issues/crash-slash-freeze-when-quitting-macos-standalone-player-that-is-actively-rendering-with-metal))

- 多人游戏修正了进入游戏模式时编辑器角色与 MPPM 游戏模式场景角色不同步的问题。
    ([uum-136438](https://issuetracker.unity3d.com/issues/editor-role-does-not-sync-with-the-mppm-play-mode-scenario-role-when-entering-play-mode))

- 网络在 UnityWebRequest 上公开 httpForcedVersion 属性，以便在需要时强制网络通信使用特定的 http 协议版本。
    (UUM-131759)

- 物理修正了在某些情况下可能引入的 NaN 值，在这些情况下，刚体（Rigidbody）会通过 ForceMode.Acceleration 应用加速度，同时其旋转受限。该问题通常会在手动调用 Physics.Simulate 时出现。
    (UUM-103515)

- 物理使用 "Use Fast Midphase "烹饪选项在 "MeshCollider "上进行射线投射时防止堆栈溢出。
    ([UUM-110564](https://issuetracker.unity3d.com/issues/silent-crash-when-raycasting-on-a-specific-dense-mesh))

- `物理 2D"`: 所有物理对象和参数验证现在都在最终的播放器构建中进行，以确保行为一致，并且如果使用编辑器/开发播放器未检测到警告（或忽略），则不会发生崩溃。
    ([uum-137011](https://issuetracker.unity3d.com/issues/physicscore2d-internal-validation-doesn-t-happen-in-non-dev-player-build))

- `Physics 2D`: PhysicsWorld.TestOverlapShape、PhysicsWorld.OverlapShape、PhysicsWorld.CastShape 和 PhysicsShape.CastShape 现在可以正确地返回世界空间中的结果，并按照预期忽略初始形状。
    (UUM-136473)

- `物理 2D`: 重新排列 ChainSegmentGeometry 序列化字段，使它们以更直观的顺序出现在检查器中。
    (UUM-137108)

- `QNX`: 修正了 QNX 窗口上的触摸/鼠标输入坐标。
    (UUM-135196)

- 阴影图修正了复制粘贴或复制节点会导致所有节点的预览根据偏好折叠或展开，而不是尊重原始状态的问题。
    (UUM-136522)

- 阴影图修正了当偏好设置为默认不展开预览时，创建的预览节点的预览会折叠的问题。
    (UUM-136521)

- 阴影图标修正了错误和警告节点徽章工具提示溢出其容器的问题。
    ([UUM-133930](https://issuetracker.unity3d.com/issues/validation-message-text-overflows-its-background-in-shader-graph-custom-function-node))

- `着色器`: 修正了构建过程中的一个罕见崩溃。
    ([uum-134784](https://issuetracker.unity3d.com/issues/crash-on-shadercompilation-transientdata-strippasses-when-building-a-project-with-specific-graphics-settings))

- 着色器设置流控制偏好标志以报告着色器编译警告而非错误。
    ([uum-130622](https://issuetracker.unity3d.com/issues/compute-shaders-throw-compilation-errors-when-show-compiled-code-is-pressed))

- `Text`: 确保链接标签在帮助框中有效。
    ([uum-135690](https://issuetracker.unity3d.com/issues/textgenerationinfo-pointer-is-null-dot-errors-are-spammed-and-link-doesnt-work-when-clicking-on-the-hyperlinks-in-the-build-profiles))

- `文本`: 修正了一个问题，即字母间距在文本居中和右对齐时不能正确工作。
    ([uum-134277](https://issuetracker.unity3d.com/issues/letters-on-the-left-side-move-further-as-letter-spacing-is-increased-when-advanced-text-generator-is-used-and-alignment-is-set-to-center))

- `文本`: 修正了 ATG 中的缓存中毒问题。
    ([uum-134255](https://issuetracker.unity3d.com/issues/uitoolkit-editor-window-text-is-not-displayed-when-using-advanced-text-generation))

- `文本`: 修正了 ATG 中的缓存问题。
    ([uum-135642](https://issuetracker.unity3d.com/issues/text-after-a-unicode-private-use-area-character-is-invisible-when-advanced-text-generator-is-used))

- `文本`: 修正了使用标准文本的位图时高亮度不正确的问题。
    ([uum-134691](https://issuetracker.unity3d.com/issues/project-settings-search-highlights-are-misaligned-when-using-the-bitmap-text-rendering-mode))

- `uGUI`: 修正了在字体重建范围内添加文本组件时的异常。
    ([uum-128580](https://issuetracker.unity3d.com/issues/invalidoperationexception-thrown-when-text-legacy-font-is-rebuilt-via-inputfield-legacy-onvaluechanged-callback))

- 用户界面元素修正了针对 UnityEvent 的 Inspector 复制/粘贴，现在它可以在带有自定义编辑器（如 Button\ ）的组件和不带自定义编辑器的组件之间工作。以前，由于剪贴板格式不兼容，在这两种组件之间粘贴复制的 UnityEvent 会无声地失败。
    ([uum-134401](https://issuetracker.unity3d.com/issues/unityevent-does-not-get-pasted-to-a-ugui-component-when-trying-to-copy-it-from-a-script))

- 用户界面工具包修正了支持 UITKPreview 而不影响其他预览。
    ([uum-133704](https://issuetracker.unity3d.com/issues/shadergraph-only-uv0-displays-a-propre-preview))

- 用户界面工具包公开 EditorUtility.activePlayModeTint，使自定义网格和 Painter2D 的颜色看起来与编辑器一致。
    (UUM-114424)

- 用户界面工具包修正了一个 Bug，该 Bug 在更改溢出或角半径后可能导致不正确的剪切。
    ([UUM-135869](https://issuetracker.unity3d.com/issues/invalid-clip-method))

- 用户界面工具包修正了在播放模式下检查 SVG 资产时出现的 "面板设置无主题样式表 "警告。
    ([uum-123228](https://issuetracker.unity3d.com/issues/no-theme-style-sheet-set-to-panelsettings-warnings-appear-when-changing-tessellation-mode-of-an-svg-asset-used-as-a-background-of-visual-element))

- 用户界面工具包修正了滤镜中的模版遮罩被渲染为正常几何体的问题。
    ([uum-135894](https://issuetracker.unity3d.com/issues/ui-toolkit-renders-visual-element-white-when-the-overflow-property-is-set-to-hidden-any-border-radius-is-applied-and-any-filter-is-applied))

- 用户界面工具包修正了当当前值从样式表继承时编辑 `FilterStyleField` 内联值的问题。
    (UUM-135010)

- `用户界面工具包`: 修正了 CommandList 泄漏。
    ([UUM-135928](https://issuetracker.unity3d.com/issues/ui-toolkit-leaks-4-persistant-allocates-when-the-displaystyle-of-a-visualelement-is-set-from-flex-to-none))

- `用户界面工具包`: 当使用自定义着色器时，修正了编辑器窗口的样本元素纹理节点的伽玛问题。
    ([uum-135360](https://issuetracker.unity3d.com/issues/ui-toolkit-visualelements-render-darker-when-a-custom-shader-graph-material-is-assigned-in-ui-builder))

- `用户界面工具包`: 修正了平面 UI（叠加或编辑器）中 Z 保留不一致的问题。
    ([uum-115032](https://issuetracker.unity3d.com/issues/dragging-search-query-block-can-remove-its-color))

- `用户界面工具包`: 修正了多列树形视图在排序时从 GetIdFromIndex 和 GetItemDataForIndex 返回错误数据的问题。
    (UUM-111055)

- 用户界面工具包修正了播放模式色调不总是被应用的问题。
    (UUM-136707)

- `用户界面工具包`: 修正了用户界面工具包着色器的预览代码生成。
    ([UUM-130869](https://issuetracker.unity3d.com/issues/ui-toolkit-custom-shaders-shows-incorrect-previews-for-preview-and-combine-nodes-when-inputting-the-default-solid-b-channel))

- `用户界面工具包`: 修正了 EditorMonitor 中的 RenderTexture 泄漏。
    (UUM-104256)

- `用户界面工具包`: 修正了 SVG 细分模式，该模式在切换生成的资产类型后不会持续。
    ([UUM-136307](https://issuetracker.unity3d.com/issues/tessellation-mode-changes-when-switching-svg-generated-asset-type-back-to-ui-toolkit-vector-image))

- `用户界面工具包`: 修正了 SVGImporter 不遵守某些导入文件的序列化 FileID 的问题。
    ([uum-136228](https://issuetracker.unity3d.com/issues/svg-image-component-loses-source-svg-image-field-references-when-upgrading-to-a-different-vector-graphics-package-version))

- `用户界面工具包`: 修正了 WebGL 着色器精度问题。
    ([uum-132006](https://issuetracker.unity3d.com/issues/ui-toolkit-text-becomes-visually-distorted-when-the-text-is-not-directly-facing-the-camera))

- `用户界面工具包`: 在渲染叠加 UI 时将 invertCulling 强制为 false，以增加对泄漏状态的安全性。
    (UUM-136734)

- VFX 图形修正了排序计算传递导致的 iOS 上的渲染伪像和冻结。
    (UUM-136074)

- 视频修正了 `WebGLSupport` 中 fakemod 模块中 `ChannelGroupI::getPitch` 的警告。
    ([UUM-134014](https://issuetracker.unity3d.com/issues/fmod-returns-error-code-78-message-repeatedly-shown-in-the-console-when-playing-audio-using-an-audio-random-container))

- `WebGL`: WebGPU：修正了着色器编译器中的一个错误，该错误导致某些着色器编译失败。
    ([uum-134978](https://issuetracker.unity3d.com/issues/shader-compiler-and-shader-errors-are-thrown-in-the-console-when-building-web-platform-with-webgpu-experimental-enabled-in-auto-graphics-api))




## 6000.3.12f1 中的软件包变更

## 更新的软件包

- `com.unity.collections`: [2.6.2](https://docs.unity3d.com/Packages/com.unity.collections@2.6//changelog/CHANGELOG.html) 到 [2.6.5](https://docs.unity3d.com/Packages/com.unity.collections@2.6//changelog/CHANGELOG.html)

- `com.unity.entities`: [1.4.2](https://docs.unity3d.com/Packages/com.unity.entities@1.4//changelog/CHANGELOG.html) 至 [1.4.5](https://docs.unity3d.com/Packages/com.unity.entities@1.4//changelog/CHANGELOG.html)

- `com.unity.physics`: [1.4.2](https://docs.unity3d.com/Packages/com.unity.physics@1.4//changelog/CHANGELOG.html) 至 [1.4.5](https://docs.unity3d.com/Packages/com.unity.physics@1.4//changelog/CHANGELOG.html)

- `com.unity.entities.graphics`: [1.4.15](https://docs.unity3d.com/Packages/com.unity.entities.graphics@1.4//changelog/CHANGELOG.html) 到 [1.4.18](https://docs.unity3d.com/Packages/com.unity.entities.graphics@1.4//changelog/CHANGELOG.html)

- `com.unity.cinemachine`: [2.10.6](https://docs.unity3d.com/Packages/com.unity.cinemachine@2.10//changelog/CHANGELOG.html) 到 [2.10.7](https://docs.unity3d.com/Packages/com.unity.cinemachine@2.10//changelog/CHANGELOG.html)

- `com.unity.performance.profile-analyzer`: [1.3.2](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.3//changelog/CHANGELOG.html) 到 [1.3.3](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.3//changelog/CHANGELOG.html)

- `com.unity.postprocessing`: [3.5.1](https://docs.unity3d.com/Packages/com.unity.postprocessing@3.5//changelog/CHANGELOG.html) 到 [3.5.4](https://docs.unity3d.com/Packages/com.unity.postprocessing@3.5//changelog/CHANGELOG.html)

- `com.unity.services.analytics`: [6.2.2](https://docs.unity3d.com/Packages/com.unity.services.analytics@6.2//changelog/CHANGELOG.html) 到 [6.3.0](https://docs.unity3d.com/Packages/com.unity.services.analytics@6.3//changelog/CHANGELOG.html)

- `com.unity.splines`: [2.8.3](https://docs.unity3d.com/Packages/com.unity.splines@2.8//changelog/CHANGELOG.html) 到 [2.8.4](https://docs.unity3d.com/Packages/com.unity.splines@2.8//changelog/CHANGELOG.html)

- `com.unity.visualcripting`: [1.9.10](https://docs.unity3d.com/Packages/com.unity.visualscripting@1.9//changelog/CHANGELOG.html) 到 [1.9.11](https://docs.unity3d.com/Packages/com.unity.visualscripting@1.9//changelog/CHANGELOG.html)

- `com.unity.multiplayer.playmode`: [2.0.1](https://docs.unity3d.com/Packages/com.unity.multiplayer.playmode@2.0//changelog/CHANGELOG.html) 到 [2.0.2](https://docs.unity3d.com/Packages/com.unity.multiplayer.playmode@2.0//changelog/CHANGELOG.html)

- `com.unity.transport`: [2.6.0](https://docs.unity3d.com/Packages/com.unity.transport@2.6//changelog/CHANGELOG.html) 到 [2.7.1](https://docs.unity3d.com/Packages/com.unity.transport@2.7//changelog/CHANGELOG.html)

- `com.unity.dedicated-server`: [2.0.1](https://docs.unity3d.com/Packages/com.unity.dedicated-server@2.0//changelog/CHANGELOG.html) 到 [2.0.2](https://docs.unity3d.com/Packages/com.unity.dedicated-server@2.0//changelog/CHANGELOG.html)

- `com.unity.memoryprofiler`: [1.1.11](https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.1//changelog/CHANGELOG.html) 到 [1.1.12](https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.1//changelog/CHANGELOG.html)

- `com.unity.netcode.gameobjects`: [2.9.1](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@2.9//changelog/CHANGELOG.html) 到 [2.10.0](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@2.10//changelog/CHANGELOG.html)

- `com.unity.polyspatial`: [3.1.0](https://docs.unity3d.com/Packages/com.unity.polyspatial@3.1//changelog/CHANGELOG.html) 到 [3.1.1](https://docs.unity3d.com/Packages/com.unity.polyspatial@3.1//changelog/CHANGELOG.html)

- `com.unity.polyspatial.visionos`: [3.1.0](https://docs.unity3d.com/Packages/com.unity.polyspatial.visionos@3.1//changelog/CHANGELOG.html) 到 [3.1.1](https://docs.unity3d.com/Packages/com.unity.polyspatial.visionos@3.1//changelog/CHANGELOG.html)

- `com.unity.polyspatial.xr`: [3.1.0](https://docs.unity3d.com/Packages/com.unity.polyspatial.xr@3.1//changelog/CHANGELOG.html) 到 [3.1.1](https://docs.unity3d.com/Packages/com.unity.polyspatial.xr@3.1//changelog/CHANGELOG.html)

- `com.unity.polyspatial.extensions`: [3.1.0](https://docs.unity3d.com/Packages/com.unity.polyspatial.extensions@3.1//changelog/CHANGELOG.html) 到 [3.1.1](https://docs.unity3d.com/Packages/com.unity.polyspatial.extensions@3.1//changelog/CHANGELOG.html)

- `com.unity.xr.visionos`: [3.1.0](https://docs.unity3d.com/Packages/com.unity.xr.visionos@3.1//changelog/CHANGELOG.html) 到 [3.1.1](https://docs.unity3d.com/Packages/com.unity.xr.visionos@3.1//changelog/CHANGELOG.html)

- `com.unity.asset-manager-for-unity`: [1.9.2](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.9//changelog/CHANGELOG.html) 到 [1.10.0](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.10//changelog/CHANGELOG.html)

- `com.unity.cloud.draco`: [5.4.2](https://docs.unity3d.com/Packages/com.unity.cloud.draco@5.4//changelog/CHANGELOG.html) 到 [5.4.3](https://docs.unity3d.com/Packages/com.unity.cloud.draco@5.4//changelog/CHANGELOG.html)

- `com.unity.cloud.ktx`: [3.6.2](https://docs.unity3d.com/Packages/com.unity.cloud.ktx@3.6//changelog/CHANGELOG.html) 到 [3.6.3](https://docs.unity3d.com/Packages/com.unity.cloud.ktx@3.6//changelog/CHANGELOG.html)