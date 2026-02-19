# Unity 6000.3.9f1 LTS
发布于 星期三, 18 二月 2026 11:29:51 GMT
https://unity.com/releases/editor/whats-new/6000.3.9f1

# 6000.3.9f1 中的已知问题

- `6000.0.55f1,6000.3.0a4`: 在切换用户界面时创建多人房间时发生 RaiseException 时崩溃
    ([uum-132182](https://issuetracker.unity3d.com/issues/crash-on-raiseexception-when-creating-a-multiplayer-room-while-toggling-ui))

- `6000.0.65f1,6000.5.0a4,6000.3.3f1,6000.4.0b2`: 当先前的地形曲率已被取消时，地形工具会沿用先前的地形曲率
    ([uum-134053](https://issuetracker.unity3d.com/issues/the-terrain-tools-follow-the-previous-terrain-curvature-when-it-was-already-undone))

- `6000.2.0a7,6000.0.48f1`: [URP] 如果贴花渲染器技术设置为 "自动"，则通过批量模式构建或在编辑器中不渲染场景/游戏视图时，所有材质都会呈现黑色
    ([uum-134298](https://issuetracker.unity3d.com/issues/urp-all-materials-render-black-when-building-via-batchmode-or-without-rendering-scene-slash-game-view-in-editor-if-decal-renderer-technique-is-set-to-automatic))

- `6000.3.0a1`: 在禁用对象上调用方法时，PhysicsCommands::PhysX::GetShapeGeometryHolder 崩溃
    ([uum-134161](https://issuetracker.unity3d.com/issues/crash-on-physicscommands-physx-getshapegeometryholder-when-calling-a-method-on-a-disabled-object))

- `6000.3.0a4,6000.0.62f1`: [iOS] 当在软键盘上使用 "取消 "按钮时，文本输入字段停止接收更改
    ([uum-133751](https://issuetracker.unity3d.com/issues/ios-text-input-field-stops-receiving-changes-when-the-cancel-button-is-used-on-the-soft-keyboard))

- `6000.3.5f1`: 启用雕刻后移动导航网格障碍物时 CPU 占用率增加
    ([uum-133911](https://issuetracker.unity3d.com/issues/increased-cpu-usage-when-moving-navmesh-obstacles-with-carving-enabled))

- `6000.5.0a5`: 当使用 Screen.SetResolution() 改变显示分辨率时，DX12 播放器亮度会发生变化
    ([uum-134064](https://issuetracker.unity3d.com/issues/dx12-player-brightness-changes-when-changing-display-resolution-with-screen-dot-setresolution))

- `6000.5.0a5,6000.3.6f1,6000.4.0b6`: [LinuxEditor] 在编辑器外编辑文件时，自动刷新无法重新导入和编译脚本更改
    ([uum-133944](https://issuetracker.unity3d.com/issues/linux-auto-refresh-fails-to-reimport-and-compile-script-changes-when-editing-files-outside-the-editor))

- `Metal`: 命令缓冲区超时错误后游戏冻结
    ([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- `平台音频`: [Windows] 在编辑器中执行各种操作时，AudioManager::InitFMOD 会崩溃
    ([uum-126803](https://issuetracker.unity3d.com/issues/crash-on-audiomanager-initfmod-when-performing-various-actions-in-the-editor))

- 文本 (TextMeshPro)：在 TMPro 字体资产创建器中生成多线程字体图集时，在 UNITY_FT_Load_Glyph 上发生崩溃
    ([uum-125366](https://issuetracker.unity3d.com/issues/crash-on-unity-ft-load-glyph-when-generating-multi-threaded-font-atlas-in-tmpro-font-asset-creator))

在位于远程驱动器路径（OneDrive、Dropbox 等）下的项目中执行各种 Unity 操作时，在 mdb_txn_renew0 上发生崩溃
    ([uum-134234](https://issuetracker.unity3d.com/issues/crash-on-mdb-txn-renew0-when-performing-various-unity-operations-in-a-project-thats-located-under-a-remote-drive-path-onedrive-dropbox-etc))

在空白 URP 项目中进入和退出播放模式时编辑器内存泄漏
    ([uum-132677](https://issuetracker.unity3d.com/issues/editor-memory-leak-when-entering-and-exiting-play-mode-in-a-blank-urp-project))

在 DirectX 12 独占全屏模式下切换焦点时播放器崩溃
    ([uum-134743](https://issuetracker.unity3d.com/issues/player-crash-when-switching-focus-in-exclusive-fullscreen-mode-with-directx-12))



# 6000.3.9f1 发布说明

# # 更改

- 编辑器更改了设置了 targetVelocity 的棱柱关节类型（速度驱动棱柱关节），因此现在将目标速度设置为正值会在模拟过程中产生正线速度。同样，将目标速度设置为负值将导致线速度为负值。
    ([uum-113920](https://issuetracker.unity3d.com/issues/prismatic-articulationbody-moves-in-opposite-direction-when-using-targetvelocity))



# # 修复

- `2D`: 将磁贴调色板中用作警告图标的图像更改为更高分辨率的图像，使其在编辑器中看起来不那么模糊。
    ([uum-129885](https://issuetracker.unity3d.com/issues/help-box-icon-in-tile-palette-window-is-blurry-in-both-unity-themes))

- `2D`: 修正了调色板或画笔名称过长会隐藏磁贴调色板中其他 UI 元素的问题。
    ([uum-130336](https://issuetracker.unity3d.com/issues/long-tile-palette-name-breaks-window-ui))

- `2D`: 修正了当切换到名称长度不同的调色板或画笔时，调色板和画笔下拉菜单的大小会发生变化的问题。
    ([uum-132618](https://issuetracker.unity3d.com/issues/tile-palette-dropdown-expands-when-palette-name-is-longer-in-tile-palette-window))

- `2D`: 修正了当瓷砖调色板的旋转轴设置为非 XY/YX 值时，当放大或缩小瓷砖调色板时，瓷砖调色板会向前轴移动的问题。
    (UUM-133308)

- `2D`: 修正了磁贴调色板窗口的问题，即当磁贴调色板窗口首次显示时，分割视图线未与底视图对齐。
    ([UUM-129883](https://issuetracker.unity3d.com/issues/drop-down-component-is-overlapped-with-the-default-tile-palette-layout-line))

- `2D`: 修正了 "雪碧编辑器 "窗口信息框被模块用户界面遮挡的问题。
    ([uum-131899](https://issuetracker.unity3d.com/issues/inactive-skinning-editor-toolbar-overlaps-the-help-box-in-the-sprite-editor-when-asset-is-not-editable))

- `2D`: 截断目标、调色板和画笔下拉菜单的长目标、调色板和画笔名称。
    ([uum-132825](https://issuetracker.unity3d.com/issues/tile-palette-dropdown-menu-doesnt-truncate-longer-tilemap-names-in-tile-palette-window))

- `2D`: 将 Tilemap 在用户界面中使用的文字从场景视图更新为场景视图。
    ([uum-130251](https://issuetracker.unity3d.com/issues/tile-palette-sceneroot-and-sceneview-are-not-rendered-with-correct-ui-spacing))

- `安卓`: 修正了 Linux/Mac 中显示警告的 gdb 路径。
    (UUM-133333)

- `安卓`: 移除 Android 库文档中多余的空格。
    (UUM-133945)

- `Asset Bundles`: 修正了一个问题，即 `AssetBundleUnloadOperation` 分配的持续时间比预期的要长，并且直到下一次 `GC.collect()` 才会被清除。
    (UUM-132703)

- `DX12`: 已通过允许在渲染传递内进行异步计算栅栏等待进行了修复。
    ([UUM-105302](https://issuetracker.unity3d.com/issues/dx12-crash-on-d3d12rendersubpassinfo-begin-when-changing-property-value-on-custom-render-pass-feature))

- `DX12`: 修正了与划痕内存分配有关的崩溃。
    ([uum-131707](https://issuetracker.unity3d.com/issues/crash-with-multiple-stack-traces-when-using-dx12-and-selecting-all-spline-knots))

- `DX12`: 修正了与从头分配内存相关的崩溃。
    ([uum-131824](https://issuetracker.unity3d.com/issues/crash-on-checkdevicestatus-when-moving-in-the-scene-view-on-a-specific-scene))

- `DX12`: 修正了使用 D3D12 时编辑器中 maxQueuedFrames 为 1 时的死锁。
    ([uum-131962](https://issuetracker.unity3d.com/issues/editor-freezes-when-qualitysettings-dot-maxqueuedframes-is-set-to-1-and-dx12-is-used))

- `编辑器`: 当切换回保存的编辑器布局时，停靠的多人游戏模式窗口会消失。
    ([uum-133602](https://issuetracker.unity3d.com/issues/docked-multiplayer-play-mode-window-disappears-when-switching-back-to-a-saved-editor-layout))

- `编辑器"`: 修复了当主字体中缺少省略号字形时高级文本生成器崩溃的问题。
    ([uum-133551](https://issuetracker.unity3d.com/issues/crash-on-textlayoutservice-computeglyphoverflow-when-opening-a-specific-uxml))

- `编辑器"`: 修正了空文本生成信息异常。
    ([uum-133791](https://issuetracker.unity3d.com/issues/textgenerationinfo-pointer-is-null-errors-are-logged-when-hovering-over-inspected-element-in-the-ui-debugger))

- 编辑器修正了域重载时删除文件时，打开编辑器首选项选项卡引发的错误。
    ([uum-133958](https://issuetracker.unity3d.com/issues/nullreferenceexception-error-is-thrown-during-addressables-cleanup-when-the-project-settings-window-is-open))

- 编辑器修正了在项目中使用水样本构建播放器时产生错误的问题。
    (UUM-133713)

- 编辑器修正了一个问题，即 EditorUtility.CompressTexture / EditorUtility.CompressCubemapTexture 会在压缩过程中太迟中断对签名 EAC 格式的压缩，导致纹理处于破碎状态。请注意，有符号的 EAC 格式不支持压缩，这一点已添加到 API 文档中。

- 编辑器修复了在 Windows 上显示模态对话框时编辑器变得无响应的问题。
    ([uum-132303](https://issuetracker.unity3d.com/issues/the-editor-freezes-and-leaks-memory-when-cancelling-the-switch-of-the-default-render-pipeline-while-using-the-advanced-object-selector))

- 编辑器修正了 iOS 构建对话框中替换和取消按钮位置互换的问题。
    ([uum-133660](https://issuetracker.unity3d.com/issues/clean-build-replace-button-does-nothing-when-pressed-and-building-a-project-for-the-ios-platform))

- 编辑器修正了 EditorUtility.CompressTexture / EditorUtility.CompressCubemapTexture 可能会尝试将 NPOT mipmapped 纹理压缩为不支持的目标格式的问题。有关此问题的其他详细信息已添加到 API 文档中。
    ([uum-129605](https://issuetracker.unity3d.com/issues/corrupted-mipmaps-are-generated-when-using-editorutility-dot-compresstexture-with-npot-textures))

- 编辑器修正了 adp 配置文件名称折页无法通过点击其标签文本展开的问题。
    ([uum-133311](https://issuetracker.unity3d.com/issues/adaptive-performance-scaler-profile-foldouts-dont-open-when-clicked-on-the-foldout-title))

- `编辑器"`: 修正了如何在搜索命题中匹配替换。
    ([uum-132679](https://issuetracker.unity3d.com/issues/vfx-graph-template-windows-search-filter-returns-no-results-for-any-category-when-a-template-category-contains-special-characters))

- 编辑器外部工具中签名团队ID和iOS/tvOS配置文件ID不一致的问题。
    ([uum-132053](https://issuetracker.unity3d.com/issues/inconsistent-id-values-between-signing-team-id-and-ios-slash-tvos-profile-id-in-external-tools))

- `编辑器"`: 修正了使用 ATG 选择段落的问题。
    ([uum-133353](https://issuetracker.unity3d.com/issues/text-selection-slash-highlighting-is-not-rendered-properly-when-selecting-slash-highlighting-package-description-that-has-multiple-lines-in-the-package-manager-window))

- `编辑器"`: 修正了当对话框包含过长信息时控制台中出现的杂散错误信息。该信息可在编辑器日志中查看。
    (UUM-121610)

- 编辑器修复了在不同DPI比例的显示器上拖动时，WinEditor闪屏图像损坏的问题。
    ([UUM-124825](https://issuetracker.unity3d.com/issues/windows-the-launch-screen-does-not-redraw-correctly-when-moved-to-a-display-of-a-different-scale))

- 编辑器安卓的发布设置 "构建 "部分现在只能通过全局安卓设置进行编辑。
    ([uum-126778](https://issuetracker.unity3d.com/issues/publishing-settings-are-shared-across-different-custom-build-profiles-when-modifying-build-options))

- `编辑器"`: 在 ProjectSettings 中设置 AssetPipeline 设置时刷新设置。
    (UUM-129185)

- 编辑器多人游戏模式工具看不到游戏模式场景列表。
    ([UUM-133716](https://issuetracker.unity3d.com/issues/the-multiplayer-play-mode-tool-doesnt-see-the-list-of-play-mode-scenarios-when-using-6000-dot-3-x))

- `图形`: 修复了即时模式绘图消耗大量内存的问题。
    ([uum-132332](https://issuetracker.unity3d.com/issues/100-percent-crash-rate-when-loading-two-profiler-captures-in-the-profile-analyzer-compare-tool))

- `iOS`: 调整键盘 UI 以更好地适应液体玻璃。
    (UUM-133464)

- 软件包管理器修复了一个 Windows 问题，即当 Unity 从带有空控制台标题的命令提示符启动时，Unity 软件包管理器可能会在启动时崩溃。
    (PAK-8605)

- 物理修复了 Rigidbody.SweepTest 和 Rigidbody.SweepTestAll 的一个问题，在刚性体的 Collider 组件位于子 GameObject 上的情况下，碰撞层设置会影响刚性体的 Collider 组件。
    ([uum-91192](https://issuetracker.unity3d.com/issues/the-gameobjects-layer-which-contains-the-rigidbody-is-used-for-rigidbody-dot-sweeptest-when-retrieving-a-collider-from-a-child-gameobject-with-a-non-collide-able-layer))

- 物理修正了 "布料检查器 "绘画工具的一个问题，即由于没有向内部碰撞网格发射光线投射，因此无法显示画笔。
    ([uum-61756](https://issuetracker.unity3d.com/issues/paintable-area-is-offset-from-the-mesh-when-editing-cloth-constraints))

- `物理 2D"`: 修复了多摄像头调试渲染中的一个问题，以确保精确的自定义绘制元素生命周期，停止早期清除。此外，自定义绘制元素现在总是在任何自动场景绘制之后绘制。
    (UUM-133990)

- `物理 2D"`: 修正了 "drawThickness "和 "drawPointScale "属性的调试 SDF 着色器中的一个问题，使它们能正确地以像素比例渲染。建议将 "PhysicsWorldDefinition "重置为默认值，或将 "drawThickness "和 "drawPointScale "分别设置为 1 和 0.5。  如果不这样做，你会发现轮廓渲染比以前稍厚了一些。
    (UUM-133990)

- `物理 2D"`: 修复了 "PhysicsRotate "属性抽屉在检查器中同时显示 "角度 "和 "方向 "的问题。这可能会造成混淆，因此已简化为 "旋转 "的单一字段。
    (UUM-133990)

- 剖析器修正了捕获列表工具提示和迷你亮点栏中显示的 "帧数超过目标 "百分比与主窗口的 "亮点 "视图不同步的问题。
    ([uum-120289](https://issuetracker.unity3d.com/issues/profiler-saving-whilst-profiling-is-recording-can-result-in-highlights-data-not-matching))

- 剖析器修正了在 Win32 平台上添加带有元数据的样本时，Profiler 中可能出现的缓冲区超限和崩溃问题。
    (UUM-129792)

- 剖析器当剖析器在数据处理过程中内存不足时，引发内存不足致命错误。
    ([UUM-130676](https://issuetracker.unity3d.com/issues/profiler-crash-on-dynamicheapallocator-getblockpointer))

- 项目浏览器修正了试图删除不可变资产时会在控制台中抛出重复警告的问题。
    ([uum-121159](https://issuetracker.unity3d.com/issues/two-warnings-appear-for-every-soft-delete-operation-when-deleting-sub-assets-in-the-project-browser))

- 文本为 nobr 标签添加了 ATG 支持。
    (UUM-133007)

- 用户界面工具包修正了过滤器不考虑 DPI 的问题。
    ([UUM-122745](https://issuetracker.unity3d.com/issues/filters-do-not-take-dpi-into-account))

- `用户界面工具包`: 修正当改变绑定且元素在层次结构中移动时，使用不正确的绑定。
    ([uum-133584](https://issuetracker.unity3d.com/issues/script-enum-fields-show-none-when-expanding-nested-inspector-elements))

- `用户界面工具包`: 解决了一个 Vulkan 定义重新定义错误。
    ([uum-132686](https://issuetracker.unity3d.com/issues/ui-shader-graph-throws-unitydisplayorientationpretransform-error-when-android-is-the-selected-platform))

- `用户界面工具包用户界面工具包`: 修正了 painter2D Fill\(\) 无法渲染具有极端长宽比的形状（例如 36000x36）的问题。

- `URP`: \编辑] 在 URP 图形设置中添加了可选的地形着色器包含设置。不选中它将阻止地形细节着色器被添加到构建中。
    ([uum-109540](https://issuetracker.unity3d.com/issues/urp-terrain-shaders-are-always-included-when-building-on-any-target-platform))

- VFX 图形修正了一个问题，即曲线和梯度上的分支会导致一些无意义的重新制作并上传到 GPU。
    (UUM-129743)

- `WebGL`: WebGPU： 自动处理绑定到着色器的纹理的读取和写入。
    ([UUM-131864](https://issuetracker.unity3d.com/issues/webgpu-cant-bind-compute-rwtexture-for-read-and-write))

- `WebGL`: WebGPU： 修复在着色器中使用 RWTexture2D 纹理时的流水线错误，并简化 unorm RWTextures 的使用。
    ([uum-131863](https://issuetracker.unity3d.com/issues/webgpu-errors-with-unorm-and-half4-rwtexture))




# # 6000.3.9f1 中的软件包变更

# # 更新的软件包

- `com.unity.burst`: [1.8.27](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html) 到 [1.8.28](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html)

- `com.unity.mobile.notifications`: [2.4.2](https://docs.unity3d.com/Packages/com.unity.mobile.notifications@2.4//changelog/CHANGELOG.html) 到 [2.4.3](https://docs.unity3d.com/Packages/com.unity.mobile.notifications@2.4//changelog/CHANGELOG.html)

- `com.unity.ui.test-framework`: [1.0.0](https://docs.unity3d.com/Packages/com.unity.ui.test-framework@1.0//changelog/CHANGELOG.html) 到 [6.3.0](https://docs.unity3d.com/Packages/com.unity.ui.test-framework@6.3//changelog/CHANGELOG.html)

- `com.unity.memoryprofiler`: [1.1.9](https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.1//changelog/CHANGELOG.html) 到 [1.1.11](https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.1//changelog/CHANGELOG.html)

- `com.unity.netcode.gameobjects`: [2.8.0](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@2.8//changelog/CHANGELOG.html) 到 [2.9.1](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@2.9//changelog/CHANGELOG.html)

- `com.unity.multiplayer.tools`: [2.2.7](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@2.2//changelog/CHANGELOG.html) 到 [2.2.8](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@2.2//changelog/CHANGELOG.html)

- `com.unity.services.multiplayer`: [2.0.0](https://docs.unity3d.com/Packages/com.unity.services.multiplayer@2.0//changelog/CHANGELOG.html) 到 [2.1.1](https://docs.unity3d.com/Packages/com.unity.services.multiplayer@2.1//changelog/CHANGELOG.html)