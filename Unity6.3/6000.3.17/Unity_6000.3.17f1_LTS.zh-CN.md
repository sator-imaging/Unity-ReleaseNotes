# Unity 6000.3.17f1 LTS
发布于 2026年6月4日 星期四 13:42:33 GMT  
https://unity.com/releases/editor/whats-new/6000.3.17f1

# 6000.3.17f1 中的已知问题

- `6000.0.61f1`: 使用 SDF16 或 SDF32 生成字体图集时，tlsf_free 会引发崩溃
    ([UUM-141061](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-generating-font-atlas-with-sdf16-or-sdf32))

- `6000.0.6f1`: [渲染图][D3D12] 在 D3D12SwapChain::Present 调用中，当使用 AddComputePass 并同时启用 EnableAsyncCompute(true) 和 UseTexture 时发生崩溃
    ([UUM-140183](https://issuetracker.unity3d.com/issues/rendergraph-d3d12-crash-on-d3d12swapchain-present-when-using-addcomputepass-with-enableasynccompute-true-and-usetexture))

- `6000.2.0a8`: 当异步 HTTP 回调在脚本域销毁后执行时，会因 Scripting::LogException 导致崩溃
    ([UUM-141434](https://issuetracker.unity3d.com/issues/crash-on-scripting-logexception-when-async-http-callback-executes-after-scripting-domain-teardown))

- `6000.3.15f1`: [Windows] 安装软件包时，会出现“EPERM: 操作不被允许”错误，导致安装非确定性失败
    ([UUM-142421](https://issuetracker.unity3d.com/issues/package-installation-fails-安装-包-时-会-以-非-确定性-方式-出现-错误-EPERM-操作-不被-允许))

- `6000.5.0a6`: 在特定项目中进入播放模式时，执行 PhysicsCommands::PhysX::BodySetPose 会导致崩溃
    ([UUM-143658](https://issuetracker.unity3d.com/issues/crash-on-physicscommands-physx-bodysetpose-在特定项目中进入播放模式时))

- `6000.5.0a7,6000.0.69f1,6000.3.11f1,6000.4.0b11`: [Android][GameActivity] 当应用处于后台运行时启动前台服务，关闭后无法重新启动
    ([UUM-143555](https://issuetracker.unity3d.com/issues/android-gameactivity-app-fails-to-relaunch-after-it-was-closed-when-a-foreground-service-started-while-app-was-backgrounded))

- `资源导入器`: 进入播放模式时，编辑器在执行“(Unity) WriteObjectToVector”操作时崩溃
    ([UUM-112617](https://issuetracker.unity3d.com/issues/editor-crashes-on-unity-writeobjecttovector-when-entering-into-the-play-mode))

- `Metal`: 命令缓冲区超时错误后游戏卡死
    ([UUM-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- 文本 (TextMeshPro)： 在 TMPro 字体资源生成器中生成多线程字体图集时，UNITY_FT_Load_Glyph 调用会导致崩溃
 ([UUM-125366](https://issuetracker.unity3d.com/issues/crash-on-unity-ft-load-glyph-when-generating-multi-threaded-font-atlas-in-tmpro-font-asset-creator))

在编辑器中执行各种操作时，mdb_cursor_sibling 发生崩溃
    ([UUM-141720](https://issuetracker.unity3d.com/issues/crash-on-mdb-cursor-sibling-when-performing-various-actions-in-the-editor))

当运行多个 bee_backend 实例时，mono_log_write_logfile 发生崩溃
    ([UUM-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))



# 6000.3.17f1 发布说明

## 改进

- `编辑器`: 在叠加模式下启用“法线”或“切线”时，移除了画布组件下的警告。
    ([UUM-137367](https://issuetracker.unity3d.com/issues/additional-shader-channel-keeps-reverting-when-saving-prefab))

- `着色器`: 新增“未应用的更改”对话框，当用户在着色器构建设置界面中存在待处理修改时离开该界面，该对话框将弹出。



## 变更

- `Android`: 将 Gradle 升级至 9.1.0，AGP 升级至 9.0.0。



## 修复

- `2D`: 修复了在启用 Sprite Atlas V2 打包并通过 "SpriteAtlasManager.atlasRequested" 加载 Addressables SpriteAtlas 时，带有 SpriteSkin 的 Sprite 在编辑器播放模式下不可见的问题
    (UUM-137123)

- `2D`: 修复了在场景视图（SceneView）或贴图面板（Tile Palette）窗口外部释放鼠标按钮时，对贴图集（Tilemap）执行的“选择”、“拾取”、“框选”和“移动”工具操作无法正确取消或完成的问题。
    ([UUM-139284](https://issuetracker.unity3d.com/issues/drag-selecting-on-tilemap-gameobject-outside-of-scene-view-causes-the-selection-mode-get-stuck-on-mouse))

- `2D`: 修复了笔刷选择列表视图中的问题，此前用户可禁用列表视图中的所有列，导致出现错误信息并丢失 SceneView。
    ([UUM-141552](https://issuetracker.unity3d.com/issues/all-tile-palette-brush-pick-overlays-columns-can-be-disabled-that-leads-to-nullreferenceexception-errors-being-spammed))

- `2D`: 修复了当网格设置了非零单元间距值时，GetCellCenterLocal/World 返回值的问题。
    (UUM-137327)

- `Android`: 修复了 Android 平台上全屏模式下关闭触摸屏键盘后导航栏会显示出来的问题。
    ([UUM-142004](https://issuetracker.unity3d.com/issues/android-navigation-bar-does-not-go-away-when-tapping-on-the-screen-to-close-the-keyboard))

- `Android`: 修复了选择自定义 Gradle 模板时的源代码构建问题。
    (UUM-138551)

- `动画`: 修复了旧版动画系统中的精度不匹配问题，该问题会导致在高帧率下跳过动画事件。
    ([UUM-138951](https://issuetracker.unity3d.com/issues/the-animation-event-is-not-triggered-when-the-frame-rate-is-set-to-120-on-the-s26-ultra))

- `动画`: 修复了在进入或退出播放模式时，悬空的 GameObject 引用可能仍保留在选中列表中的问题。
    (UUM-142098)

- `Animation`: 修复了在 Dopesheet 中右键单击混合了变换和精灵关键帧时出现的错误。
    ([UUM-142341](https://issuetracker.unity3d.com/issues/errors-are-thrown-and-contextual-menu-does-not-open-when-right-clicking-multiple-mixed-keyframes-in-dopesheet))

- `音频`: 当所有 AudioListener 组件被禁用或其 GameObject 被停用时，音频在 Player 构建中仍会继续播放。
    ([UUM-127556](https://issuetracker.unity3d.com/issues/audiolisteners-still-listen-to-audio-when-their-components-are-disabled-in-player))

- `Audio`: 修复了在播放模式下，若 `MonoBehaviour` 初始处于禁用状态，启用 `AudioListener` 上的 `OnAudioFilterRead` 效果时无声响的问题。
    ([UUM-116871](https://issuetracker.unity3d.com/issues/onaudiofilterread-does-not-affect-signal-on-audiolistener-after-enable))

- `构建管道`: 新增支持通过 BootConfig 键 "remapper-initial-capacity" 为 PersistentManager.Remapper 预留容量，该键用于指定初始哈希表大小。
    (UUM-136275)

- `文档`: 修复了 2D 碰撞体参考页面中的 Vale 错误。

- `DX12`: 修复了在 DX12 环境下执行内存密集型操作时发生的崩溃问题。
    (UUM-141699)

- `编辑器`: 新增名为 `enableHeightmapLODFrustumCulling` 的选项，该选项可在调试模式下的地形检查器设置中找到，用于禁用地形视锥体基于LOD的剔除。
    (UUM-141589)

- `编辑器`: 在自定义构建配置文件中修改图形 API 列表现已正常工作。
    (UUM-127416)

- `编辑器`: 修复了当输入网格包含大量共享单条边且相互重叠的三角形时，网格 LOD 生成器会崩溃的问题。
    ([UUM-137244](https://issuetracker.unity3d.com/issues/crash-on-meshlodutils-buildclustermergejobsgeneric-when-generating-mesh-lods-for-a-specific-model))

- `编辑器`: 修复了因文件损坏或外部文件锁定导致无法打开 curl 文件缓存数据库 \(CurlRequestCache.db\) 时，启动程序会崩溃的问题。
    ([UUM-140399](https://issuetracker.unity3d.com/issues/crash-on-getdatabase-when-sqlite-database-for-the-curl-file-cache-fails-to-open-or-create))

- `编辑器`: 修复了将轮廓路径细分成多边形时发生的崩溃问题。 这可能影响 PolygonCollider2D、TilemapCollider2D 和 PhysicsComposer。
    ([UUM-142017](https://issuetracker.unity3d.com/issues/editor-crashes-on-outputpolymesh-when-running-a-specific-scene-in-play-mode-or-player))

- `编辑器`: 修复了在构建前，当 BuildPlayerProcessor.PrepareForBuild 回调删除包含程序集的文件夹时，导致玩家崩溃的问题
    ([UUM-137492](https://issuetracker.unity3d.com/issues/player-crashes-upon-launch-when-a-folder-is-deleted-as-a-prebuild-step))

- `编辑器`: 修复了在 Mac 编辑器中将编辑器语言切换为日语时极少发生的崩溃问题
    ([UUM-141719](https://issuetracker.unity3d.com/issues/crash-on-platform-strlen-when-the-editors-language-is-changed-to-japanese))

- `Editor`: 修复了在“固定时间步长”字段中输入 Inf 或 NaN 时出现的“无效的双参数”错误。
    ([UUM-138227](https://issuetracker.unity3d.com/issues/argumentexception-invalid-double-parameter-dot-error-is-thrown-when-infinity-is-typed-into-the-fixed-timestep-field))

- `编辑器`: 修复了在“检查器”数组的“大小”字段（例如“玩家设置”>“预加载资源”）中输入极大数值（例如 24124124）时，编辑器会卡死的问题。
    ([UUM-139781](https://issuetracker.unity3d.com/issues/the-editor-freezes-indefinitely-when-entering-24124124-into-the-preloaded-assets-size))

- `编辑器`: 修复了一个问题：当纹理设置为以立方体贴图（Cubemap）形式导入或不使用Mipmap时，即使所选级别对这些纹理有影响，也无法操作纹理导入器的“各向异性级别”滑块。
    ([UUM-138249](https://issuetracker.unity3d.com/issues/aniso-level-still-applies-when-generate-mipmap-is-disabled-in-texture-import-settings))

- `编辑器`: 修复了在“播放模式”下导入预制体时，存储在 MonoBehaviour/ScriptableObject 字段中的引用可能会丢失的问题。
    ([UUM-139664](https://issuetracker.unity3d.com/issues/the-reference-to-a-prefab-variant-is-lost-on-instantiation-when-it-is-serialized-in-a-parents-component))

- `编辑器`: 修复了 macOS 和 Linux 编辑器在关闭后，仍有 VBCSCompiler 进程继续运行的问题。
    (UUM-142615)

- `编辑器`: 修复了应用加粗格式时文本溢出的问题。
    ([UUM-137212](https://issuetracker.unity3d.com/issues/bold-text-unexpectedly-overflows))

- `Editor`: 通过为图形 API 设置重启条件添加额外检查，修复了切换构建配置文件时出现编辑器重启提示的问题。
    (UUM-139685)

- `Editor`: 修复了当编辑器使用 -projectPath 参数启动时，Hub 仍会通过重新连接循环打开的问题。
    ([UUM-142653](https://issuetracker.unity3d.com/issues/unity-hub-opens-when-launching-the-editor-with-projectpath-argument-v2))

- `编辑器`: 修复了更改最小探针间距后探针照明不正确的问题。
    ([UUM-141983](https://issuetracker.unity3d.com/issues/adaptive-probe-volumes-require-a-second-bake-for-correct-probe-lighting-data-when-min-probe-spacing-is-changed-in-urp))

- `编辑器`: 修复了在构建配置文件中，若在缩放器配置文件中添加了空的自定义缩放器字段并重置 UI 时发生的空指针异常。
    ([UUM-140845](https://issuetracker.unity3d.com/issues/argumentnullexception-thrown-when-reseting-adaptive-performance-settings-with-no-reference-set-in-defaultscaler))

- `Editor`: 修复了在使用 UI Toolkit \(default\) 检查器模式时，于检查器中撤销预制体变体的属性覆盖后，OnValidate 未被调用的问题。此前，切换按钮和下拉菜单等非文本字段会错误地阻止预制体资源在撤销后自动保存，从而阻塞 `OnValidate` 方法，直到用户点击其他位置移除该字段的焦点。
    ([UUM-134476](https://issuetracker.unity3d.com/issues/the-onvalidate-method-is-not-invoked-when-reverting-changes-on-a-prefab-variant))

- `Editor`: 修复了导入工作线程中单例的重新加载顺序，以防止在切换构建配置文件时工作线程崩溃。
    ([UUM-133886](https://issuetracker.unity3d.com/issues/assetimportworker-crash-on-kernelbase-raiseexception-when-switching-between-web-and-uwp-platforms-in-build-profiles))

- `Editor`: 修复了更改色彩空间设置后项目窗口路径失效的问题。
    ([UUM-139519](https://issuetracker.unity3d.com/issues/project-window-path-display-breaks-visually-when-player-settings-color-space-is-changed))

- `编辑器`: 修复了在多人游戏模式克隆场景中，当场景包含精灵图集时出现的精灵图集资源导入错误。
    (UUM-139265)

- `编辑器`: 修复了 TextCore 精灵资源中的 Unicode 处理问题。
    ([UUM-141521](https://issuetracker.unity3d.com/issues/ui-toolkit-doesnt-render-the-assigned-sprites-when-using-unicode-characters-assigned-to-a-sprite))

- `编辑器`: 地形：修复了编辑选中地形的高程图时出现的性能退化问题。
    ([UUM-141526](https://issuetracker.unity3d.com/issues/the-editor-start-performing-very-poorly-when-editing-the-terrain-heightmap-with-terraindata))

- `EmbeddedLinux`: 为 `GameWindow.DisposeAsync` 添加了缺失的文档。
    (UUM-141650)

- `引擎诊断`: 修复了因异步崩溃报告管道在播放器循环停止后无法完成，导致关机时重复的托管异常计数丢失的问题。
    ([UUM-141101](https://issuetracker.unity3d.com/issues/combined-log-and-throw-exceptions-function-does-not-show-up-in-diagnostics-cloud-dashboard-when-called-in-player))

- `引擎诊断`: 修复了因 JNI 本机方法过早注销而导致的崩溃，该问题会在 `nativeOnAndroidAppSetIdResult` 方法中引发 `java.lang.UnsatisfiedLinkError` 错误。
    (UUM-137662)

- `GI`: 修复了由 `PruneCellIndexList` 中过期的单元格索引导致的 APV 崩溃。
    ([UUM-142091](https://issuetracker.unity3d.com/issues/crash-on-rendererscene-notifyinvisible-when-gameobjects-are-deleted-from-the-hierarchy-in-a-specific-scene))

- `GI`: 修复了黑色方块的视觉异常。
    ([UUM-142681](https://issuetracker.unity3d.com/issues/black-square-shadow-artifacts-visible-when-using-screen-space-reflections-without-maximum-smoothing))

- `Graphics`: 在条件允许时，对仅包含混合形状的网格应用 GPU 皮肤处理。
    ([UUM-137953](https://issuetracker.unity3d.com/issues/low-performance-when-multiple-meshes-using-blendshape-are-rendered-on-screen))

- `Graphics`: 修复了 `validateCommonDrawErrors` 中因缓冲区溢出而触发的 Metal 验证断言。
    ([UUM-138495](https://issuetracker.unity3d.com/issues/mac-metal-failed-assertion-on-validatecommondrawerrors-when-buffer-is-overrun))

- `Graphics`: 修复了在 GPU 遮挡剔除过程中，驻留于 GPU 的绘制器错误地将四边形拓扑网格渲染为三角形的问题。
    ([UUM-132444](https://issuetracker.unity3d.com/issues/automatic-lod-fails-and-gpu-occlusion-culling-incompatibility-occurs-when-using-spline-based-quad-topology-meshes))

- `图形`: 修复了当检查器窗口较窄时，文本溢出“打开项目设置 &gt; 图形...”按钮的问题。
    ([UUM-141971](https://issuetracker.unity3d.com/issues/全局设置-资源-打开项目设置-图形-省略号-文本-在-检查器-窗口-变窄时-溢出-按钮边界))

- `图形`: 修复了“着色器通道”中“最近命中着色器”的 UAV 导致崩溃的问题。目前该功能不被支持，在此情况下着色器编译器将报告错误。
    ([UUM-137197](https://issuetracker.unity3d.com/issues/crash-on-writehitgrouprecordjob-when-material-closesthit-uses-rwtexture2d-uav))

- `Graphics`: 减少了向渲染线程传递渲染命令时占用的内存量，并改进了相关诊断信息。
    (UUM-127793)

- `IL2CPP`: 将用于构建 GameCore C++ 代码的 MSVC 最高版本从 16 提升至 17。
    (UUM-109593)

- `IL2CPP`: 修复了 IL2CPP 在处理秩大于 18 的多维数组时的代码生成问题。
    ([UUM-138552](https://issuetracker.unity3d.com/issues/build-fails-when-building-a-project-containing-an-18-plus-dimension-array-with-il2cpp))

- `iOS`: 确保当 il2cpp 命令构建 GameAssembly 失败时，Xcode 项目构建也会失败。
    (UUM-141609)

- `License`: 修复了授权客户端的重新连接问题。
    ([UUM-142572](https://issuetracker.unity3d.com/issues/floating-license-is-lost-for-concurrent-jobs))

- `Linux`: 修复了在 Linux 上读取大于 2 GiB 的 POSIX 文件时失败的问题。
    ([UUM-140520](https://issuetracker.unity3d.com/issues/couldnt-open-file-for-reading-error-occurs-when-running-binary2text-on-a-file-larger-than-2-gib))

- `粒子系统`: 修复了子发射器在子发射器模块中多次出现时导致的崩溃问题。
    ([UUM-142083](https://issuetracker.unity3d.com/issues/crash-on-particlesystemupdatedata-cachesubemitters-particlesystem-and-when-shared-subemitter-referenced-by-multiple-nested-particle-systems))

- `物理`: 修复了启用投影模式的 ConfigurableJoint 因连接的刚体从运动学模式转为动态模式而导致崩溃的问题
    ([UUM-135394](https://issuetracker.unity3d.com/issues/crash-on-constraintprojectiontree-projectiontreebuildstep-当-可配置关节-使用-关节投影模式-点位置和旋转-且-连接的刚体-从-运动学-切换-为-非运动学时))

- `Physics`: 当 Ragdoll Builder 窗口中的动画器为空时，将“自动填充”按钮设为不可用。
    (UUM-142958)

- `Physics 2D`: 修复了 PhysicsCore2D 渲染器在叠加摄像机上渲染的问题。
    ([UUM-142142](https://issuetracker.unity3d.com/issues/physicscore2d-renderer-should-ensure-it-only-renders-to-a-base-camera-in-urp))

- `预制体`: 在“ExecuteInEditMode 预制体模式”警告对话框中添加了会话退出选项。
    (UUM-139861)

- `QNX`: 为 `GameWindow.DisposeAsync` 添加了缺失的文档。
    (UUM-141650)

- `Shadergraph`: 修复了使用预定义关键字着色器输入的着色器在编辑器中打开时，会因重新定义导致着色器编译错误的问题。
    ([UUM-142398](https://issuetracker.unity3d.com/issues/redefinition-of-lod-fade-crossfade-shader-errors-thrown-when-opening-speedtree9-urp-dot-shadergraph-in-universal-3d-template))

- `着色器`: 新增了“未应用的更改”对话框，当用户在着色器构建设置界面中存在待处理修改时离开该界面，该对话框将弹出。
    ([UUM-138992](https://issuetracker.unity3d.com/issues/用户在点击离开图形设置转至其他设置窗口时，未被提示是否应用或撤销更改))

- `着色器`: 修复了 Material.GetTexturePropertyNameIDs 在材质变体中返回空值的问题。
    ([UUM-85842](https://issuetracker.unity3d.com/issues/an-empty-list-is-incorrectly-returned-for-material-variant-when-using-material-dot-gettexturepropertynameids))

- `着色器`: 修复了着色器构建设置中“关键字声明覆盖”部分的错误提示信息显示不清晰的问题。
    ([UUM-132639](https://issuetracker.unity3d.com/issues/light-editor-theme-the-error-message-keyword-declaration-override-cannot-be-empty-is-poorly-visible-in-the-graphics-settings-window))

- `着色器`: 修复了着色器检查器在处理没有属性的着色器时，其“属性”折叠面板显示为空的问题。
    ([UUM-127146](https://issuetracker.unity3d.com/issues/planeocclusionshader-properties-foldout-does-not-display-any-content))

- `着色器`: 当处理大型着色器时，使用“编译并显示代码”下拉菜单不再导致编辑器卡死，因为我们避免了遍历每个着色器阶段的每个关键字来计算“包含变体”的数量。
    ([UUM-141740](https://issuetracker.unity3d.com/issues/compile-and-show-code-dropdown-freezes-the-editor-for-a-long-time))

- `测试框架`: 修复了 Unity 测试框架将发布设置 SCID 覆盖为默认值的问题。
    (UUM-138637)

- `uGUI`: 修复了在“允许富文本编辑”功能禁用时，于 TMP InputField 开头向左移动光标会抛出 `IndexOutOfRangeException` 的问题。
    ([UUM-134157](https://issuetracker.unity3d.com/issues/indexoutofrangeexception-thrown-when-moving-caret-left-at-start-of-tmp-input-field-with-rich-text))

- `UI Elements`: 优化了导致部分 UIToolkit.<br>
    .Bindings.PerformanceTests 回归的新代码
    (UUM-139531)

- `UI Toolkit`: 修复了在 TreeView 中仅左侧 XR 控制器能够执行项目选择的问题。
    ([UUM-141157](https://issuetracker.unity3d.com/issues/tree-view-from-ui-toolkit-will-take-one-xr-controller-as-primary-input-and-ignore-the-secondary-when-the-game-is-unpaused))

- `UI Toolkit`: 修复了在检查器中选中 UIDocument 时，其根 VisualElement 会被重新生成的 bug。
    ([UUM-127851](https://issuetracker.unity3d.com/issues/uidocument-generatevisualcontent-callback-is-not-assigned-when-uidocument-is-shown-in-the-inspector))

- `UI Toolkit`: 修复了在层级视图中选中 UI 文档时进入播放模式会引发 `MissingReferenceException` 错误的问题。
    ([UUM-131364](https://issuetracker.unity3d.com/issues/missingreferenceexception-error-is-thrown-when-entering-play-mode-while-ui-document-is-selected-in-hierarchy))

- `URP`: 修复了帧调试器内存占用过高的回归问题。
    ([UUM-139160](https://issuetracker.unity3d.com/issues/frame-debugger-excessive-memory-usage-regression))

- `URP`: 修复了在帧调试器中展开“纹理”折叠面板时，纹理预览图标缺失的问题。
    ([UUM-134917](https://issuetracker.unity3d.com/issues/texture-preview-icons-are-missing-in-frame-debugger-when-expanding-textures-foldout))

- `URP`: URP Gbuffer 着色器现指定 `#pragma rendertarget_format_hint`，以修复在需要此信息的平台上的渲染问题。
    (UUM-134506)

- `VFX Graph`: 修复了使用 `-nographics` 构建时，VFX Graph 位置 \(Depth\) 无法正常工作的问题。
    ([UUM-141265](https://issuetracker.unity3d.com/issues/building-with-nographics-breaks-vfx-graph-position-depth-as-an-operator))

- `Video`: 修复了在快进/快退时，平台报告的帧 ID 与我们报告给 C# 层的帧 ID 之间可能发生的竞争条件。
    (UUM-134928)

- `Web`: 修复了多线程 Web 构建中 Gamepad API 无法正常工作的问题。
    ([UUM-136543](https://issuetracker.unity3d.com/issues/gamepad-input-does-not-work-in-a-web-build-when-native-c-slash-c-plus-plus-multithreading-is-enabled))




## 6000.3.17f1 版本中的包变更

## 已更新的包

- `com.unity.services.core`: [1.16.0](https://docs.unity3d.com/Packages/com.unity.services.core@1.16//changelog/CHANGELOG.html) 更新至 [1.17.0](https://docs.unity3d.com/Packages/com.unity.services.core@1.17//changelog/CHANGELOG.html)

- `com.unity.services.wire`: [1.4.2](https://docs.unity3d.com/Packages/com.unity.services.wire@1.4//changelog/CHANGELOG.html) 更新至 [1.4.4](https://docs.unity3d.com/Packages/com.unity.services.wire@1.4//changelog/CHANGELOG.html)

- `com.unity.test-framework.performance`: 从 [3.4.0](https://docs.unity3d.com/Packages/com.unity.test-framework.performance@3.4//changelog/CHANGELOG.html) 升级至 [3.5.0](https://docs.unity3d.com/Packages/com.unity.test-framework.performance@3.5//changelog/CHANGELOG.html)