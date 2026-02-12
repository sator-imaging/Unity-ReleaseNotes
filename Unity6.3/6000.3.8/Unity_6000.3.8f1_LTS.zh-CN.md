# Unity 6000.3.8f1 LTS
发布于 星期三, 11 二月 2026 10:40:25 GMT
https://unity.com/releases/editor/whats-new/6000.3.8f1

# 6000.3.8f1 中的已知问题

- `6000.0.55f1,6000.3.0a4`: 在切换用户界面时创建多人房间时发生 RaiseException 时崩溃
    ([uum-132182](https://issuetracker.unity3d.com/issues/crash-on-raiseexception-when-creating-a-multiplayer-room-while-toggling-ui))

- `6000.0.65f1,6000.5.0a4,6000.3.3f1,6000.4.0b2`: 当先前的地形曲率已被取消时，地形工具会沿用先前的地形曲率
    ([uum-134053](https://issuetracker.unity3d.com/issues/the-terrain-tools-follow-the-previous-terrain-curvature-when-it-was-already-undone))

- `6000.1.0a2,6000.0.64f1`: 进入播放模式时，单通道立体渲染只显示天空盒
    ([uum-132342](https://issuetracker.unity3d.com/issues/single-pass-stereo-rendering-shows-only-skybox-when-entering-play-mode))

- `6000.3.0a1`: 在禁用对象上调用方法时，PhysicsCommands::PhysX::GetShapeGeometryHolder崩溃
    ([uum-134161](https://issuetracker.unity3d.com/issues/crash-on-physicscommands-physx-getshapegeometryholder-when-calling-a-method-on-a-disabled-object))

- `6000.3.0b1,6000.0.65f1`: 当质量设置（QualitySettings.maxQueuedFrames）设为 1 并使用 DX12 时，编辑器会冻结
    ([uum-131962](https://issuetracker.unity3d.com/issues/editor-freezes-when-qualitysettings-dot-maxqueuedframes-is-set-to-1-and-dx12-is-used))

- `6000.3.5f1`: 在启用雕刻的情况下移动导航网格障碍物时 CPU 占用率增加
    ([uum-133911](https://issuetracker.unity3d.com/issues/increased-cpu-usage-when-moving-navmesh-obstacles-with-carving-enabled))

- `6000.5.0a1,6000.3.2f1`: 在特定场景的场景视图中移动时，在检查设备状态（CheckDeviceStatus）时崩溃
    ([uum-131824](https://issuetracker.unity3d.com/issues/crash-on-checkdevicestatus-when-moving-in-the-scene-view-on-a-specific-scene))

- `6000.5.0a1,6000.3.2f1`: 使用 DX12 并选择所有样条线节时，出现多个堆栈跟踪的崩溃现象
    ([uum-131707](https://issuetracker.unity3d.com/issues/crash-with-multiple-stack-traces-when-using-dx12-and-selecting-all-spline-knots))

- `6000.5.0a5`: 当使用 Screen.SetResolution() 改变显示分辨率时，DX12 播放器亮度发生变化
    ([uum-134064](https://issuetracker.unity3d.com/issues/dx12-player-brightness-changes-when-changing-display-resolution-with-screen-dot-setresolution))

- `金属'`: 命令缓冲区超时错误后游戏冻结
    ([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- `金属`: [iOS]iOS闪屏后屏幕闪烁
    ([uum-121453](https://issuetracker.unity3d.com/issues/ios-screen-flashing-after-the-ios-splash-screen))

- `平台音频`: [Windows] 在编辑器中执行各种操作时，AudioManager::InitFMOD 会崩溃
    ([uum-126803](https://issuetracker.unity3d.com/issues/crash-on-audiomanager-initfmod-when-performing-various-actions-in-the-editor))

在空白 URP 项目中进入和退出播放模式时编辑器内存泄漏
    ([uum-132677](https://issuetracker.unity3d.com/issues/editor-memory-leak-when-entering-and-exiting-play-mode-in-a-blank-urp-project))



# 6000.3.8f1 发行说明

## 改进

- `资产管道`: 提高了符号链接检测的性能。
    (UUM-132708)

- 阴影图节点折叠时 UV 节点上通道下拉菜单的外观改进。
    ([UUM-115034](https://issuetracker.unity3d.com/issues/uv-nodes-label-is-cut-off-when-preview-is-collapsed))



## 更改

- `图形纹理导入现在严格遵守 https`: //docs.unity3d.com/Documentation/Manual/ImportingTextures.html 中的支持格式。通过更改图像文件扩展名来规避这一规定的做法将不再奏效。如果需要某种图像文件格式，请提交功能请求，以便我们研究如何正确支持该格式。



## 修复

- `2D`: 修正了 "雪碧编辑器 "窗口中自定义枢轴字段溢出的问题。
    ([uum-133168](https://issuetracker.unity3d.com/issues/sprite-editors-custom-pivot-fields-get-pushed-out-of-their-bounds-when-entering-a-lot-of-numbers-in-the-property-field))

- `2D`: 修正了用户在任意位置用空画笔绘制并在（0, 0, 0\ ）处清除磁贴的问题。
    ([uum-128709](https://issuetracker.unity3d.com/issues/painting-on-a-tilemap-erases-random-tile-when-an-empty-tile-was-selected-in-the-tilemap-palette))

- 动画修正了一个问题，即在 `OnFocus` 回调期间，动画窗口会恢复到上一个选定对象。现在，动画窗口在获得焦点时会保留当前选择。
    ([uum-131198](https://issuetracker.unity3d.com/issues/last-selected-asset-before-docking-animation-window-gets-selected-when-a-domain-reload-occurs))

- 动画修复了 AnimationWindowEvent 检查器中损坏的文档链接。
    ([uum-131593](https://issuetracker.unity3d.com/issues/animation-event-is-missing-documentation-link))

- `错误报告`: 修正了将离线报告导出到 Unity 项目目录时 Bug Reporter 崩溃的问题。
    ([uum-129604](https://issuetracker.unity3d.com/issues/bug-reporter-crashes-when-exporting-offline-report-into-a-unity-project-directory))

- `错误报告器"`: 修正了悬停在聚焦下拉字段上滚动时值发生变化的问题。
    (SUS-5725)

- 编辑器在剖析器模块介绍中添加了默认剖析器模块列表。

- 编辑器修复了关闭一个 Unity 实例的 WinEditor SplashScreen 会关闭其他实例的问题。
    ([uum-124686](https://issuetracker.unity3d.com/issues/the-project-launching-process-moves-to-the-background-when-another-project-is-closed))

- 编辑器修正了使用高级对象选择器更改默认渲染管道时的双重确认对话框。
    ([uum-132296](https://issuetracker.unity3d.com/issues/a-second-prompt-asking-users-to-confirm-is-opened-when-cancelling-the-switch-of-the-graphics-default-render-pipeline-while-using-the-advanced-object-selector))

- `编辑器"`: 修正了在不同显示器上重新打开实用程序窗口时，WinEditor 中 DPI 缩放不正确的问题。
    (UUM-131238)

- 编辑器修正了在某些情况下显示模式对话框时，WinEditor 无法响应的问题。
    ([UUM-132303](https://issuetracker.unity3d.com/issues/the-editor-freezes-and-leaks-memory-when-cancelling-the-switch-of-the-default-render-pipeline-while-using-the-advanced-object-selector))

- `编辑器"`: SceneProvider 可以找到带有 t:behaviour 的条目。
    ([uum-114607](https://issuetracker.unity3d.com/issues/hierarchy-search-in-searchwindow-filtering-by-exact-type-monobehaviour))

- `编辑器`: 将普通 GameObject 重新连接到 prefab 时，保留任何子实例。
    ([uum-102262](https://issuetracker.unity3d.com/issues/child-prefab-instance-connection-lost-when-reconnecting-parent-prefab))

- `图形`: 修正了在解析 MSAA 无记忆深度缓冲区时出现金属验证错误的崩溃问题。
    (UUM-125478)

- `图形`: 修复了从 AssetBundles 加载资源（通常是纹理）时，在 AsyncResourceUploadBlocking\(\) 中偶尔发生的罕见死锁情况。
    ([uum-126066](https://issuetracker.unity3d.com/issues/android-the-application-freezes-during-the-assetbundle-loading))

- `物理 2D"`: "PhysicsShapeDefinition.moverData" 属性现在可以在 Unity 编辑器检查器中编辑。
    (UUM-133265)

- `物理 2D"`: 确保 "PhysicsWorld.CastMover "不会检测触发形状。
    (UUM-133265)

- `物理 2D"`: 确保 PhysicsTransform 和 PhysicsRotate 构造函数与 Burst 兼容。
    (UUM-133265)

- `物理 2D"`: PhysicsShape.define现在包括读取 "PhysicsShapeDefinition.startMassUpdate "和 "PhysicsShapeDefinition.startStaticContacts "属性。
    (UUM-133265)

- 脚本编写修正了 AssemblyUpdater 通过移除不应移除的程序集引用而破坏程序集的问题。
    ([UUM-132084](https://issuetracker.unity3d.com/issues/api-updater-strips-unity-owned-custom-attribute-references-within-precompiled-dlls))

- 脚本处理修正了 ScriptUpdater 在某些情况下的堆栈溢出。
    ([uum-130076](https://issuetracker.unity3d.com/issues/script-updater-for-dot-dot-dot-failed-with-exitcode-dot-dot-dot-and-stdout-stack-overflow-dot-errors-thrown-in-console-when-a-project-using-obsolete-api-is-opened))

- 阴影图添加了swizzle节点掩码中的大写有时会导致不正确结果的问题。
    ([uum-132879](https://issuetracker.unity3d.com/issues/expected-color-is-changed-to-black-when-using-swizzle-node))

- `着色器`: 修正了因跳过的变体关键字未定义而导致的着色器编译错误。
    ([uum-98633](https://issuetracker.unity3d.com/issues/number-pragma-skip-variants-fog-linear-does-not-remove-fog-linear-keyword-declared-keyword))

- 着色器ShaderUtil.IsGrahicsAPISupported现在可以正确地与exclude_renderers一起工作。
    (UUM-133092)

- 文本新增了 `vOffset` 标签支持。
    (UUM-132638)

- `uGUI`: \[UUM-130350\]修复了输入框的一个问题，现在当虚拟键盘状态设置为 "完成 "时触发 "OnSubmit "时，输入框会正确地停用。
    ([UUM-130350](https://issuetracker.unity3d.com/issues/ios-android-onsubmit-event-is-triggered-indefinitely-on-ugui-input-field-after-dismissing-keyboard-on-mobile))

- 用户界面工具包修正了当渲染正在进行时释放网格的处理。
    ([uum-126665](https://issuetracker.unity3d.com/issues/rendering-artifacts-appear-in-ui-builder-when-applying-high-blur-value-filter-for-mask64-or-toggle-elements))

- 用户界面工具包在编辑器和 XR 中启用滚动视图拖动。
    (UUM-117166)

- 用户界面工具包修正了当 UI 文档执行实时重载并附加了丢失的脚本时抛出的空引用异常。
    ([UUM-129344](https://issuetracker.unity3d.com/issues/nullreferenceexception-thrown-when-modifying-a-ui-document-while-a-scene-containing-a-gameobject-with-any-ui-document-and-a-missing-script-component-is-open))

- `用户界面工具包`: 修正了当尝试通过用户界面调试器将材质分配给 `-unity-material` 样式时的错误。
    ([uum-114133](https://issuetracker.unity3d.com/issues/ui-debugger-invalid-value-for-property-unity-material))

- `用户界面工具包`: 修正了当从样式表继承时，在用户界面生成器中无法正确覆盖材质属性的问题。
    ([uum-130880](https://issuetracker.unity3d.com/issues/inherited-material-reference-in-the-ui-builder-disappears-after-adding-a-material-property-override-for-a-child-visual-element))

- `用户界面工具包`: 修正了导入某些 SVG 资产时的静默崩溃。
    ([uum-132415](https://issuetracker.unity3d.com/issues/silent-crash-when-importing-svg-files))

- `用户界面工具包`: 修正了升级到 Unity 6.3 时 SVG 导入器设置丢失的问题。
    ([uum-133203](https://issuetracker.unity3d.com/issues/svg-importer-settings-are-lost-when-upgrading-to-unity-6-dot-3))

- `用户界面工具包`: 修正了大型 SVG 资产填充时的 SVG 细分问题。
    ([uum-133144](https://issuetracker.unity3d.com/issues/svg-importer-fill-errors-with-large-svg-asset))

- 版本控制修正了版本控制项目设置字段与窗口标题不一致的问题。
    ([uum-127155](https://issuetracker.unity3d.com/issues/version-control-information-does-not-align-with-window-title-1))

- `网络`: 修正了传统输入系统中通过触摸事件模拟鼠标位置的问题（Input.mousePosition\）。
    ([uum-130369](https://issuetracker.unity3d.com/issues/input-dot-mouseposition-stops-syncing-to-touch-input-when-using-downloadhandlertexture-in-webgl-build))

- `WebGL`: WebGPU: 解决控制台创建渲染管道（CreateRenderPipeline）时出现的着色器变量集合预热（ShaderVariantCollection warmup）错误。
    ([uum-131262](https://issuetracker.unity3d.com/issues/webgpu-createrenderpipeline-errors-with-shadervariantcollection-warmup))




## 6000.3.8f1 中的软件包变更

## 更新的软件包

- `com.unity.addressables`: [2.8.0](https://docs.unity3d.com/Packages/com.unity.addressables@2.8//changelog/CHANGELOG.html) 到 [2.8.1](https://docs.unity3d.com/Packages/com.unity.addressables@2.8//changelog/CHANGELOG.html)

- `com.unity.formats.alembic`: [2.4.2](https://docs.unity3d.com/Packages/com.unity.formats.alembic@2.4//changelog/CHANGELOG.html) 到 [2.4.4](https://docs.unity3d.com/Packages/com.unity.formats.alembic@2.4//changelog/CHANGELOG.html)

- `com.unity.scriptablebuildpipeline`: [2.5.1](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@2.5//changelog/CHANGELOG.html) 到 [2.5.2](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@2.5//changelog/CHANGELOG.html)

- `com.autodesk.fbx`: 5.1.2 到 5.1.3

- `com.unity.ai.navigation`: [2.0.9](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html) 到 [2.0.10](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html)

- `com.unity.ai.inference`: [2.4.1](https://docs.unity3d.com/Packages/com.unity.ai.inference@2.4//changelog/CHANGELOG.html) 至 [2.5.0](https://docs.unity3d.com/Packages/com.unity.ai.inference@2.5//changelog/CHANGELOG.html)