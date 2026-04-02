# Unity 6000.0.72f1 LTS
发布于 星期三, 01 四月 2026 09:38:47 GMT
https://unity.com/releases/editor/whats-new/6000.0.72f1

# 6000.0.72f1 中的已知问题

- `6000.5.0a4,6000.0.66f1,6000.3.4f1,6000.4.0b4`: 在 Builds 中，ShaderVariantCollection.variantCount 和 ShaderVariantCollection.shaderCount 返回 0
    ([uum-137398](https://issuetracker.unity3d.com/issues/shadervariantcollection-dot-variantcount-and-shadervariantcollection-dot-shadercount-returns-0-in-builds))

- `IL2CPP`: [iOS] [Android] IL2CPP 生成过程中外部库泛型失败
    ([uum-125284](https://issuetracker.unity3d.com/issues/ios-android-external-library-generics-fail-during-il2cpp-build))

- 金属命令缓冲区超时错误后游戏冻结
    ([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- `金属"`: MacOS 在编辑器中的最小项目在播放模式下出现卡顿
    ([uum-85256](https://issuetracker.unity3d.com/issues/macos-stutters-in-a-minimal-project))

当 ConfigurableJoint 使用 JointProjectionMode.PositionAndRotation 且连接的 Rigidbody 从运动模式切换为非运动模式时，ConstraintProjectionTree::projectionTreeBuildStep 会崩溃
    ([uum-135394](https://issuetracker.unity3d.com/issues/crash-on-constraintprojectiontree-projectiontreebuildstep-when-configurablejoint-uses-jointprojectionmode-dot-positionandrotation-and-connected-rigidbody-switches-from-kinematic-to-non-kinematic))

在空白 URP 项目中重新编译时，VisualElement 中的编辑器内存泄漏
    ([uum-138000](https://issuetracker.unity3d.com/issues/editor-memory-leak-in-visualelement-when-recompiling-in-a-blank-urp-project))

在 DirectX 12 独占全屏模式下切换焦点时播放器崩溃
    ([uum-134743](https://issuetracker.unity3d.com/issues/player-crash-when-switching-focus-in-exclusive-fullscreen-mode-with-directx-12))



# 6000.0.72f1 发布说明

## 功能

- 版本控制为项目浏览器和检查器中的文件夹添加了 "添加到源代码控制 "和 "撤销更改 "操作。

- 版本控制新增了分支资源管理器，用于可视化和导航分支。

- 版本控制为所有分割器位置添加了跨窗口重载和会话的持久性。

- 版本控制在合并视图中添加了部分应用搁置的支持。

- 版本控制添加了重命名分支和标签的 F2 快捷键。



## 改进

- 文档添加了指向 Memory Profiler 软件包的直接链接。

- `Documentation`: 在内存管理文档中添加了有关清洁和脏页管理的信息。

- 安装程序由于优化了压缩策略，Windows 上的安装程序现在最多可减少 60% 的时间。
    (UUM-136633)



## 更改

- 版本控制在状态栏中添加了变更集和标签图标。

- 版本控制从 Unity Hub 打开项目时延迟工作区的创建。

- 版本控制改进了跨对话框的文本字段焦点行为，使键盘工作流程更加一致。

- 版本控制改进了 "待更改 "视图中的空状态。

- 版本控制防止错误地将项目连接到不同的组织。

- 版本控制更新了新项目初始化，以执行完整的初始签入。

- 版本控制更新了 macOS 隐藏快捷键为 Cmd+Shift+H。



## 修复

- `2D`: 将磁贴调色板中用作警告图标的图片更改为更高分辨率的图片，使其在编辑器中看起来不那么模糊。
    ([uum-129885](https://issuetracker.unity3d.com/issues/help-box-icon-in-tile-palette-window-is-blurry-in-both-unity-themes))

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

- `2D`: 修正阴影投射器 2d 裁剪。
    ([uum-135640](https://issuetracker.unity3d.com/issues/2d-freeform-light-shadows-disappear-when-light-center-is-offset-from-shape-bounds))

- `DX12`: 修正了当 `CommandBuffer.SetRenderTarget` 使用了无效的深度片时，在绑定渲染目标时崩溃的问题。
    (UUM-130121)

- `DX12`: 修复了在恢复绘制到之前绑定为计算着色器 SRV 的渲染目标后丢失资源屏障的问题。
    (UUM-127520)

- 编辑器用括号区分重复的 BuildProfile，例如 Windows （1\）。
    (UUM-130365)

- 编辑器修正了当 FormerlySerializedAs 与类型中的字段碰撞时应用预制件属性修改的问题。
    ([UUM-135039](https://issuetracker.unity3d.com/issues/object-reference-is-saved-on-an-incorrect-property-when-formerlyserializedas-is-used-on-an-overridden-prefab-variant-field))

- `编辑器"`: 修正了在 TextCore 中使用中日韩时崩溃的问题。
    ([uum-136683](https://issuetracker.unity3d.com/issues/editor-freezes-when-rendering-wrapped-text-inside-japanese-parentheses-in-too-small-of-a-space))

- `编辑器"`: 修正在标准文本中使用粗体样式时找不到全局回退的问题。
    ([uum-136612](https://issuetracker.unity3d.com/issues/synthetic-bold-applies-to-a-label-instead-of-bold-font-weight-when-using-fallback-font-asset))

- `编辑器"`: 修正了播放器设置中的标签截断问题。
    ([uum-136316](https://issuetracker.unity3d.com/issues/the-use-dxgi-flip-model-swapchain-for-d3d11-settings-label-is-not-truncated-when-viewing-player-settings-in-a-build-profile))

- 编辑器修正了在提供多个网格的情况下，MeshToSDFBaker 中网格销毁的缺失。
    ([uum-128633](https://issuetracker.unity3d.com/issues/memory-leaks-are-caused-when-using-meshtosdfbaker-dot-dispose))

- `GI`: 通过在单独进程中使用 x64 仿真运行 CPU lightmapper，在苹果硅编辑器和 Windows ARM 编辑器上启用 CPU lightmapper。
    (UUM-102347)

- `GI"`: 修复了 AMD 上的 APV 虚拟偏移烘烤。
    ([UUM-114563](https://issuetracker.unity3d.com/issues/look-rotation-viewing-vector-is-zero-messages-are-logged-in-the-console-when-baking-lighting-with-display-probes-setting-enabled-in-rendering-debugger-while-using-the-android-build-profile-on-amd-hardware))

- `图形"`: 修正了一个问题，即当追踪的 PSO 是在渲染传递之外记录的时候，使用 GraphicsStateCollection API 进行的管道状态对象（PSO）预热在 Metal 上会出现不正确的缓存丢失。
    (UUM-135455)

- 图形修正了英伟达驱动更新后 SystemInfo.supportsInlineRayTracing 变为 false 的问题。
    ([UUM-137132](https://issuetracker.unity3d.com/issues/raytracing-updating-nv-graphics-drivers-to-595-dot-79-causes-systeminfo-dot-supportsinlineraytracing-to-become-false))

- `图形`: 修正了在某些 Android 设备上使用实例化时的地形接缝问题。
    (UUM-131277)

- 图形\[Vulkan/][Android/]修复了在同一渲染传递子传递中使用深度读取和模版写入操作进行渲染时，在 Mali GPU（非 Midgard）上出现的视觉伪影。解决方法适用于存在该问题的 41.0.0 版之前的驱动程序。
    (UUM-31270)

- `IL2CPP`: 修正了 lambda 表达式中无效的 MethodsToPreserve 条目。
    ([UUM-124814](https://issuetracker.unity3d.com/issues/unity-cil-linker-fails-on-player-build-when-persistent-listeners-have-and-in-their-xml-attribute-names))

- `用户界面工具包`: 修正了在平面 UI（覆盖或编辑器）中保存 Z 的不一致性。
    ([uum-115032](https://issuetracker.unity3d.com/issues/dragging-search-query-block-can-remove-its-color))

- `用户界面工具包`: 修正了多列树形视图在排序时从 GetIdFromIndex 和 GetItemDataForIndex 返回错误数据的问题。
    (UUM-111055)

- 用户界面工具包修正了播放模式色调并非总是应用的问题。
    (UUM-136707)

- `用户界面工具包`: 修正了 WebGL 着色器精度问题。
    ([UUM-132006](https://issuetracker.unity3d.com/issues/ui-toolkit-text-becomes-visually-distorted-when-the-text-is-not-directly-facing-the-camera))

- `用户界面工具包`: 在渲染叠加 UI 时将 invertCulling 强制为 false，以增加对泄漏状态的安全性。
    (UUM-136734)

- `版本控制修正了右键单击侧栏中的 "待更改 "时出现的布局异常。

- 版本控制`: 修正了从分支差异打开历史记录时的 NullReferenceException 异常。

- `版本控制修正了逐个变更集差异面板中可能出现的 NullReferenceException。

- 版本控制修复并本地化了签入对话框的进度标签。

- 版本控制修复了 "探索软件库 "窗口中的模糊图标。

- 版本控制修正了 Unity 版本控制窗口中按钮的大小写，以符合 Unity 标准。

- 版本控制修正了分支视图中逐个变更集的差异问题。

- 版本控制`: 修正了分支上下文菜单在表格为空时无法打开的问题。

- `版本控制`: 修正了签入对话框无法自动聚焦注释字段的问题。

- `版本控制`: 修正当表格为空时无法打开标签上下文菜单的问题。

- `版本控制"`: 修复了新建分支按钮在当前选择为变更集或标签时失效的问题。

- `版本控制`: 修复了退出播放模式后状态栏变灰的问题。

- `版本控制修复了在创建工作区期间刷新 Unity 版本控制窗口而无需移动鼠标的问题。

- 版本控制修正了 Unity 版本控制窗口中验证信息的对齐方式。

- VFX 图形"`: 修复了域重载后 ColorField 丢失的问题（submesh mask 或 sliders 也有类似问题）。
    (UUM-124799)

- `VFX Graph`: 不正确的自定义属性评估导致错误的行为和着色器警告。
    ([UUM-135239](https://issuetracker.unity3d.com/issues/vfx-warning-and-simulation-error-when-using-a-specific-custom-attribute-configuration))

- 视频修正了 `WebGLSupport` 中 fakemod 模块中 `ChannelGroupI::getPitch` 的警告。
    ([uum-134014](https://issuetracker.unity3d.com/issues/fmod-returns-error-code-78-message-repeatedly-shown-in-the-console-when-playing-audio-using-an-audio-random-container))




## 6000.0.72f1 中软件包的更改

## 更新的软件包

- `com.unity.collections`: [2.6.2](https://docs.unity3d.com/Packages/com.unity.collections@2.6//changelog/CHANGELOG.html) 到 [2.6.5](https://docs.unity3d.com/Packages/com.unity.collections@2.6//changelog/CHANGELOG.html)

- `com.unity.entities`: [1.4.2](https://docs.unity3d.com/Packages/com.unity.entities@1.4//changelog/CHANGELOG.html) 至 [1.4.5](https://docs.unity3d.com/Packages/com.unity.entities@1.4//changelog/CHANGELOG.html)

- `com.unity.physics`: [1.4.2](https://docs.unity3d.com/Packages/com.unity.physics@1.4//changelog/CHANGELOG.html) 至 [1.4.5](https://docs.unity3d.com/Packages/com.unity.physics@1.4//changelog/CHANGELOG.html)

- `com.unity.entities.graphics`: [1.4.15](https://docs.unity3d.com/Packages/com.unity.entities.graphics@1.4//changelog/CHANGELOG.html) 到 [1.4.18](https://docs.unity3d.com/Packages/com.unity.entities.graphics@1.4//changelog/CHANGELOG.html)

- `com.unity.2d.aseprite`: [1.1.10](https://docs.unity3d.com/Packages/com.unity.2d.aseprite@1.1//changelog/CHANGELOG.html) 至 [1.1.11](https://docs.unity3d.com/Packages/com.unity.2d.aseprite@1.1//changelog/CHANGELOG.html)

- `com.unity.cinemachine`: [2.10.6](https://docs.unity3d.com/Packages/com.unity.cinemachine@2.10//changelog/CHANGELOG.html) 到 [2.10.7](https://docs.unity3d.com/Packages/com.unity.cinemachine@2.10//changelog/CHANGELOG.html)

- `com.unity.collab-proxy`: [2.11.4](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.11//changelog/CHANGELOG.html) 到 [2.12.4](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.12//changelog/CHANGELOG.html)

- `com.unity.nuget.mono-cecil`: [1.11.5](https://docs.unity3d.com/Packages/com.unity.nuget.mono-cecil@1.11//changelog/CHANGELOG.html) 到 [1.11.6](https://docs.unity3d.com/Packages/com.unity.nuget.mono-cecil@1.11//changelog/CHANGELOG.html)

- `com.unity.postprocessing`: [3.5.0](https://docs.unity3d.com/Packages/com.unity.postprocessing@3.5//changelog/CHANGELOG.html) 到 [3.5.4](https://docs.unity3d.com/Packages/com.unity.postprocessing@3.5//changelog/CHANGELOG.html)

- `com.unity.profiling.core`: [1.0.2](https://docs.unity3d.com/Packages/com.unity.profiling.core@1.0//changelog/CHANGELOG.html) 到 [1.0.3](https://docs.unity3d.com/Packages/com.unity.profiling.core@1.0//changelog/CHANGELOG.html)

- `com.unity.serialization`: [3.1.2](https://docs.unity3d.com/Packages/com.unity.serialization@3.1//changelog/CHANGELOG.html) 到 [3.1.5](https://docs.unity3d.com/Packages/com.unity.serialization@3.1//changelog/CHANGELOG.html)

- `com.unity.services.vivox`: [16.8.0](https://docs.unity3d.com/Packages/com.unity.services.vivox@16.8//changelog/CHANGELOG.html) 到 [16.10.0](https://docs.unity3d.com/Packages/com.unity.services.vivox@16.10//changelog/CHANGELOG.html)

- `com.unity.splines`: [2.8.3](https://docs.unity3d.com/Packages/com.unity.splines@2.8//changelog/CHANGELOG.html) 到 [2.8.4](https://docs.unity3d.com/Packages/com.unity.splines@2.8//changelog/CHANGELOG.html)

- `com.unity.test-framework.performance`: [3.2.0](https://docs.unity3d.com/Packages/com.unity.test-framework.performance@3.2//changelog/CHANGELOG.html) 到 [3.3.0](https://docs.unity3d.com/Packages/com.unity.test-framework.performance@3.3//changelog/CHANGELOG.html)

- `com.unity.visualcripting`: [1.9.10](https://docs.unity3d.com/Packages/com.unity.visualscripting@1.9//changelog/CHANGELOG.html) 到 [1.9.11](https://docs.unity3d.com/Packages/com.unity.visualscripting@1.9//changelog/CHANGELOG.html)

- `com.unity.transport`: [2.6.0](https://docs.unity3d.com/Packages/com.unity.transport@2.6//changelog/CHANGELOG.html) 到 [2.7.2](https://docs.unity3d.com/Packages/com.unity.transport@2.7//changelog/CHANGELOG.html)

- `com.unity.memoryprofiler`: [1.1.11](https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.1//changelog/CHANGELOG.html) 到 [1.1.12](https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.1//changelog/CHANGELOG.html)

- `com.unity.ai.navigation`: [2.0.11](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html) 到 [2.0.12](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html)