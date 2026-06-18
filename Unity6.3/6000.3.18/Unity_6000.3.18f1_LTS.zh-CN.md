# Unity 6000.3.18f1 LTS
发布于 2026年6月17日 星期三 08:57:11 GMT  
https://unity.com/releases/editor/whats-new/6000.3.18f1

# 6000.3.18f1 中的已知问题

- `6000.0.11f1`: 关闭包含特定资源的项目时，在 ProfilerMutexLock 处发生崩溃
    ([UUM-144371](https://issuetracker.unity3d.com/issues/crash-on-profilermutexlock-when-closing-a-project-with-specific-assets))

- `6000.5.0a6`: 在特定项目中进入“播放”模式时，执行 PhysicsCommands::PhysX::BodySetPose 会发生崩溃
    ([UUM-143658](https://issuetracker.unity3d.com/issues/crash-on-physicscommands-physx-bodysetpose-when-entering-play-mode-in-a-specific-project))

- `资源导入器`: 进入“播放模式”时，编辑器在执行“(Unity) WriteObjectToVector”操作时崩溃
    ([UUM-112617](https://issuetracker.unity3d.com/issues/editor-crashes-on-unity-writeobjecttovector-when-entering-into-the-play-mode))

- `Metal`: 命令缓冲区超时错误后游戏卡死
    ([UUM-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- `文本（TextMeshPro）`: 在 TMPro 字体资源生成器中生成多线程字体图集时，UNITY_FT_Load_Glyph 调用会导致崩溃 
    ([UUM-125366](https://issuetracker.unity3d.com/issues/crash-on-unity-ft-load-glyph-when-generating-multi-threaded-font-atlas-in-tmpro-font-asset-creator))

在编辑器中执行各种操作时，mdb_cursor_sibling 发生崩溃
    ([UUM-141720](https://issuetracker.unity3d.com/issues/crash-on-mdb-cursor-sibling-when-performing-various-actions-in-the-editor))

当有多个 bee_backend 实例同时运行时，mono_log_write_logfile 会引发崩溃
    ([UUM-142773](https://issuetracker.unity3d.com/issues/当运行多个 bee_backend 实例时 mono_log_write_logfile 发生崩溃))

生成字体图集时发生崩溃，并产生多个堆栈跟踪
    ([UUM-141061](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-generating-font-atlas-with-sdf16-or-sdf32))



# 6000.3.18f1 发布说明

## 功能

- `文档`: 在 UDP 文档处理流程中新增一个步骤，用于解析引擎文档中的交叉引用链接。



## 改进

- `多人游戏`: 修复了在连接 Perforce 的情况下创建 MPPM 玩家标签时，“VirtualProjectSettings.json” 文件出现的写入访问错误
    (UUM-144074)



## 变更

- `编辑器`: macOS Rosetta 2 安装辅助应用已不再需要，现已移除。



## 修复

- `2D`: 修复了 \(Case IN-139653\) 中填充未在所有区域完全应用的问题。
    ([UUM-139518](https://issuetracker.unity3d.com/issues/sprite-packer-does-not-obey-padding-when-allow-rotation-is-enabled))

- `2D`: 修复了网格模式下“画笔选择”窗口打开时，滚动位置会跳转至网格末尾而非最后选定项的问题。
    (UUM-138222)

- `2D`: 修复了添加“镜头光晕”组件时出现的错误，并增加了对正交摄像机的支持。
    ([UUM-141781](https://issuetracker.unity3d.com/issues/render-graph-execution-and-argumentexception-errors-are-spammed-when-adding-lens-flare-srp-component-in-a-2d-urp-project))

- `2D`: 修复了在“瓷砖调色板画笔选择”界面中，滚动至 GridView 底部后显示空白区域的问题。
    ([UUM-142144](https://issuetracker.unity3d.com/issues/empty-scrollable-space-在包含大量已保存画笔的“瓷砖调色板画笔选择”覆盖窗口和列表视图中向下滚动时，滚动条会缩小))

- `2D`: 修复了 Light2D 和 Shadow Caster 2D 组件在检查器中显示错误图标的问题。
    ([UUM-132563](https://issuetracker.unity3d.com/issues/not-clear-abbreviation-ld-on-the-2d-light-overlay))

- `2D`: 修复了使用 ShaderGraph 材质时，缩放值为负的精灵无法被选中的问题。
    ([UUM-141627](https://issuetracker.unity3d.com/issues/sprite-renderer-is-not-selectable-in-scene-view-when-using-a-sprite-shader-graph-material-on-a-negatively-scaled-object))

- `2D`: 修复了精灵编辑器窗口有时会引用其预览纹理的问题。
    ([UUM-140054](https://issuetracker.unity3d.com/issues/selected-启用预览功能后重新打开精灵编辑器时，会显示“该对象不被精灵窗口支持”提示，且精灵变为不可编辑))

- `自适应性能`: 禁止在性能操作延迟和热操作延迟中使用负值。
    (UUM-135803)

- `AI`: 加载导航网格数据时，现在会在加载导航网格表面期间避免处理现有的导航网格链接，直到该表面的所有瓦片均已加载完毕，从而降低开销。
    ([UUM-126707](https://issuetracker.unity3d.com/issues/navmeshmanager-dot-loaddata-takes-a-long-time-and-启用已实例化NavMeshLinks的NavMeshSurface会导致性能骤升))

- `Android`: 修复了在启用 RunWithoutFocus 时将 Android 应用置于后台导致 Vulkan 崩溃的问题。
    (UUM-141888)

- `音频`: 修复了在正常音频处理器释放过程中出现的误报错误 \("无法访问处理器 - 句柄已过期..."\) 以及一条虚假的“必须强制更新嵌套处理器”警告。
    (UUM-142099)

- `DX12`: 当超过活动命令缓冲区限制时，不再等待 GPU 处理完成。
    (UUM-139697)

- `DX12`: 修复了在使用 `AddComputePass` 且 `EnableAsyncCompute`\(true\) 时，D3D12SwapChain::Present 引发的崩溃。
    ([UUM-140183](https://issuetracker.unity3d.com/issues/rendergraph-d3d12-crash-on-d3d12swapchain-present-when-using-addcomputepass-with-enableasynccompute-true-and-usetexture))

- `DX12`: 修复了 Sentis 姿态采样在 DirectML 中的崩溃问题。
    (UUM-143597)

- `DX12`: 修复了在着色器异步编译期间忽略 Meta 通道 CommandBuffer.DrawMesh\(\) 的问题。
    (UUM-139294)

- `编辑器`: 清理了不代表未保存状态的 SceneBackup 文件，以避免编辑器崩溃时出现错误的恢复对话框。
    (UUM-142761)

- `编辑器`: 在“项目设置” > “图形” > “着色器”中，撤销未保存的添加操作后，删除关键字声明覆盖时，编辑器不再抛出 `ArgumentOutOfRangeException` 异常。
    ([UUM-143037](https://issuetracker.unity3d.com/issues/argumentoutofrangeexception-is-thrown-removing-a-keyword-declaration-overrides-after-adding-and-reverting-one-of-them))

- `编辑器`: 修复了在添加专用服务器构建配置文件后，**切换配置文件**按钮不会在“构建配置文件”窗口中显示的问题，该问题需重新打开窗口后才会解决。
    ([UUM-143216](https://issuetracker.unity3d.com/issues/the-switch-profile-button-does-not-appear-when-a-dedicated-server-build-profile-is-added-until-the-build-profiles-window-is-reopened))

- `编辑器`: 修复了在打开“构建配置文件”窗口且“玩家设置”资源未导入时发生的崩溃问题。
    ([UUM-116727](https://issuetracker.unity3d.com/issues/crash-on-std-1-tree-const-iterator-when-opening-the-build-profiles-window-in-a-specific-project))

- `编辑器`: 修复了运动模糊平铺处理中的一种边界情况，即在某些物体速度下，每块平铺的最小速度可能保持未初始化状态。
    ([UUM-142360](https://issuetracker.unity3d.com/issues/invalid-blue-value-in-motionblurmergetilepass-when-objects-move-at-certain-speeds))

- `编辑器`: 修复了在字体资源生成器中创建时，RASTER_HINTED 字体图集出现损坏的问题。
    ([UUM-142852](https://issuetracker.unity3d.com/issues/some-glyphs-are-skewed-in-rendered-textmeshpro-font-asset-when-using-raster-hinted-render-mode))

- `编辑器`: 修复了某些情况下因异常日志记录导致的崩溃问题。
    ([UUM-141434](https://issuetracker.unity3d.com/issues/crash-on-scripting-logexception-when-async-http-callback-executes-after-scripting-domain-teardown))

- `编辑器`: 修复了使用超链接时发生的崩溃问题。
    ([UUM-142829](https://issuetracker.unity3d.com/issues/editor-crashes-in-textlib-findintersectinglink-when-hovering-uitk-labels-with-tags-rendered-via-atg))

- `编辑器`: 修复了在批处理模式下使用 -nographics 开关打开包含自定义 DefaultCursor 的项目时，Linux 编辑器崩溃的问题。
    ([UUM-142569](https://issuetracker.unity3d.com/issues/linuxeditor-crash-on-xaddextension-when-opening-the-unity-editor-on-linux-with-batchmode-and-nographics-on-a-project-with-a-custom-default-cursor))

- `编辑器`: 在“播放”模式下，通过“检查器”预览渲染纹理和原始纹理时会出现卡顿。
    ([UUM-140017](https://issuetracker.unity3d.com/issues/video-player-preview-stutters-slash-lags-when-played-in-the-inspector-preview-during-play-mode))

- `编辑器`: \[Android\] 将“属性冲突”错误窗口中指向已缺失的“Gradle 故障排除”页面的链接，替换为适用于 Unity 6.3 的有效“Android 版 Gradle”链接。
    ([UUM-142945](https://issuetracker.unity3d.com/issues/colliding-attributes-error-opens-a-missing-page-when-pressing-the-troubleshoot-button))

- `GI`: 修复了在未安装 Rosetta 2 的 macOS ARM 构建环境中烘焙灯光时可能发生的崩溃问题。
    (UUM-142663)

- `GI`: 当 Rosetta 不可用时，禁止在 macOS ARM 构建环境中进行 CPU 灯光烘焙。
    (UUM-142173)

- `Graphics`: 延迟在纹理流中添加渲染器，以避免性能突增。
    (UUM-140042)

- `Graphics`: 修复了应用旋转时反射探针中出现的图像瑕疵。
    ([UUM-137813](https://issuetracker.unity3d.com/issues/shadow-cast-by-rotated-reflection-probe-has-corners-culled-when-using-forward-plus-or-deferred-plus-rendering-path))

- `图形`: 在使用 Vulkan 图形 API 调整窗口大小时，提升了编辑器的性能。
    (UUM-141307)

- `图形`: 设置尚未加载的父对象时，材质属性不再丢失。
    ([UUM-113050](https://issuetracker.unity3d.com/issues/material-properties-are-lost-when-setting-a-parent-that-hasnt-been-loaded-yet))

- `Graphics`: \[OpenGLES\] 修复了在 Windows OpenGLES3 独立播放器中，使用 Alt+Enter 切换全屏模式后出现的渲染错误和 OpenGL 验证错误。
    ([UUM-109464](https://issuetracker.unity3d.com/issues/rendering-errors-are-thrown-在-Windows-构建中-通过-OpenGL-API-取消-全屏-时))

- `HDRP`: 修复了在切换构建目标后，`ReAllocateOffscreenUIColorBufferIfNeeded` 中发生的 NullReferenceException 异常。
    ([UUM-143038](https://issuetracker.unity3d.com/issues/nullreferenceexception-object-reference-not-set-to-an-instance-of-an-object-error-is-thrown-after-switching-to-the-default-build-profile-in-high-definition-3d-template))

- `HDRP`: 修复了启用路径追踪时 HDR UI 叠加层缺失的问题。
    ([UUM-142884](https://issuetracker.unity3d.com/issues/hdrp-game-view-is-rendered-black-when-using-pathtracing-on-a-hdr-display))

- `HDRP`: 修复了HDRP后处理体积覆盖设置需等到刷新后才会更新的问题。
    ([UUM-142661](https://issuetracker.unity3d.com/issues/some-post-processing-volume-overrides-only-update-after-a-refresh-when-using-hdrp))

- `IL2CPP`: 修复了在选择显示方法、文件和行号的选项时，日志中的调用堆栈有时会显示错误方法的问题。
    ([UUM-138416](https://issuetracker.unity3d.com/issues/build-stack-trace-contains-invalid-lines-when-building-with-il2cpp-using-scripts-with-delegates-containing-generic-signature-types))

- `IMGUI`: 修复了 IMGUI 的选择功能。
    ([UUM-137875](https://issuetracker.unity3d.com/issues/all-of-the-logs-text-is-selected-when-trying-仅-选择-其中-一部分-的问题))

- `包管理器`: 修复了在 Windows 上安装包时间歇性出现的 `EPERM: 操作不被允许，重命名` 错误。
    ([UUM-142421](https://issuetracker.unity3d.com/issues/package-installation-fails-安装-包-时-会-以-非-确定性-方式-出现-eperm-操作-不-被-允许-错误))

- `包管理器`: 修复了使用多个检查器选择同一个 package.json 时，错误信息不一致的问题。
    (UUM-142468)

- `物理引擎`: 铰接体关节的运动极限现已限制在物理 SDK 定义的范围内。
    ([UUM-91742](https://issuetracker.unity3d.com/issues/当上限定为超过 360 时，带回转关节类型的关节体行为异常))

- `物理引擎`: 修复了在求解布料间碰撞时，由于 NvCloth 内部过度分配内存导致的内存损坏问题。
    ([UUM-64185](https://issuetracker.unity3d.com/issues/crash-on-collideparticles-when-entering-play-mode))

- `Physics`: 修复了当覆盖 MeshCollider 所引用的网格资源文件时，MeshCollider 将无法正常工作的问题。
    ([UUM-141284](https://issuetracker.unity3d.com/issues/meshcollider-preview-gizmo-disappears-from-the-scene-view-when-overriding-the-mesh-asset-using-any-3d-editing-tool))

- `物理`: 修复了胶囊碰撞体的调试可视化问题，确保在应用缩放时胶囊顶点能保持曲率。
    ([UUM-142483](https://issuetracker.unity3d.com/issues/colliders-are-rendered-deformed-when-viewed-through-physics-debugger-in-scene-view))

- `物理`: 修复了 NvCloth 求解器内核中若干 SIMD 运算导致 NaN 值的问题。
    ([UUM-64185](https://issuetracker.unity3d.com/issues/crash-on-collideparticles-when-entering-play-mode))

- `Physics 2D`: “PhysicsAABB.Normalized\(\)” 现已更名为 “PhysicsAABB.Normalize\(\)”。
    (UUM-143279)

- `Physics 2D`: 修复了脚本文档中的各种不一致之处、拼写错误及类型引用问题。
    (UUM-143279)

- `Physics 2D`: 改进了 PhysicsCore2D 系统在多线程环境下的稳定性，修复了极少数可能在世界或对象销毁过程中导致崩溃的竞争条件。
    (UUM-143564)

- `预制件`: 清理损坏的 `PrefabInstance` 时，已添加的对象将不再被移除。
    ([UUM-142338](https://issuetracker.unity3d.com/issues/crash-on-mergeobjectcollection-when-repeatedly-selecting-a-prefab-asset-in-the-project-browser))

- `Profiler`: 禁用了独立运行版 Profiler 窗口中的 AI 助手按钮。
    ([UUM-142961](https://issuetracker.unity3d.com/issues/在通过包管理器移除 AI 助手包后，“询问助手”按钮仍保留在独立 profiler 中，点击时会在控制台引发错误))

- `分析器`: 修复了在分析器已附加的情况下，进程崩溃时其最后一个帧的 CPU 时间线渲染问题。
    ([UUM-71728](https://issuetracker.unity3d.com/issues/当帧超出屏幕宽度时，分析器时间轴滚动条无法完整显示该帧))

- `场景管理器`: 修复了当加载了多个场景并退出“播放”模式时，若用户脚本订阅了 `EditorSceneManager.sceneClosed` 并在处理程序中枚举打开的场景，会导致程序崩溃的问题。
    ([UUM-131346](https://issuetracker.unity3d.com/issues/crash-on-scene-custom-getpathinternal-when-exiting-在监听EditorSceneManager.sceneClosed事件并打印打开的场景时处于播放模式))

- `着色器`: 着色器检查器中的“编译并显示代码”下拉菜单现已加宽，以避免元素重叠。
    ([UUM-143195](https://issuetracker.unity3d.com/issues/着色器检查器-编译-和-显示-代码-下拉菜单-会-裁剪-菜单项-文本-并-与-包含-变体-的-“显示”按钮-重叠))

- `Text`: 修复了高级文本生成器（ATG）文本塑形中的性能瓶颈。
    (UUM-139797)

- `TextMeshPro`: 修复了 TMP 着色器始终使用 HDR 颜色选择器，而非匹配着色器中设置的颜色模式的问题。
    ([UUM-141742](https://issuetracker.unity3d.com/issues/the-eyedropper-tool-selects-an-incorrect-value-when-sampling-a-tmp-text-objects-face-or-outline-color-from-the-game-view))

- `UI Toolkit`: 修复了一个问题，当面板中的任何元素每帧更新样式时，ScrollView.ScrollTo 在被调用后，会在每帧覆盖手动滚动输入。
    ([UUM-142486](https://issuetracker.unity3d.com/issues/scrollview-snaps-back-to-the-target-after-scrollto-when-the-ui-updates-every-frame))

- `UI Toolkit`: 修复了使用滤镜时 GroupTransform 出现卡顿的问题。
    ([UUM-142586](https://issuetracker.unity3d.com/issues/scrollview-clips-content-when-under-an-ancestor-that-has-a-filter-set))

- `UI Toolkit`: 修复了在垂直滚动时，动态高度集合视图的水平滚动值被重置为 0 的问题。
    ([UUM-142573](https://issuetracker.unity3d.com/issues/multi-column-list-view-horizontal-scroll-resets-to-left-most-position-when-scrolling-vertically))

- `UI Toolkit`: 修复了当活动样式表被重新排序至另一个样式表下方时，UI Builder 将新选择器添加到错误的 USS 文件中的问题。
    ([UUM-143744](https://issuetracker.unity3d.com/issues/在 UI 构建器中使用“添加新选择器”功能时，新选择器被添加到最顶层的样式表而非当前活动的 USS 文件中))

- `UI Toolkit`: 修复了在重新打开基础模板已被编辑的 UXML 实例后，UI Builder 检查器中 `<AttributeOverrides>` 的列表值显示为过时的情况。
    ([UUM-141060](https://issuetracker.unity3d.com/issues/a-uxml-instance-with-an-shows-stale-list-state-in-ui-builder-inspector-when-editing-its-base-template-and-reopening-the-instance))

- `UI Toolkit`: 修复了在 UI 构建器中删除已分配数据源类型的视觉元素时，控制台抛出 `ObjectDisposedException` 的问题。
    ([UUM-129925](https://issuetracker.unity3d.com/issues/deleting-a-visual-element-in-ui-builder-throws-objectdisposedexception-if-it-had-data-source-type-assigned))

- `版本控制`: 当空数组被填充后，UnityYAMLMerge 在合并操作后可能会生成无效的预制体 YAML 文件。在某些情况下，这会导致预制体解析失败并无法使用。
    ([UUM-131530](https://issuetracker.unity3d.com/issues/prefabs-are-corrupted-due-to-inline-styled-yaml-when-unityyamlmerge-is-used-to-merge-prefabs))




## 6000.3.18f1 版本中的包变更

## 已更新的包

- `com.unity.netcode`: [1.13.1](https://docs.unity3d.com/Packages/com.unity.netcode@1.13//changelog/CHANGELOG.html) 更新至 [1.13.2](https://docs.unity3d.com/Packages/com.unity.netcode@1.13//changelog/CHANGELOG.html)

- `com.unity.formats.alembic`: 从 [2.4.4](https://docs.unity3d.com/Packages/com.unity.formats.alembic@2.4//changelog/CHANGELOG.html) 更新至 [2.4.5](https://docs.unity3d.com/Packages/com.unity.formats.alembic@2.4//changelog/CHANGELOG.html)

- `com.unity.performance.profile-analyzer`: 从 [1.3.4](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.3//changelog/CHANGELOG.html) 至 [1.4.0](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.4//changelog/CHANGELOG.html)

- `com.unity.purchasing`: 从 [4.15.0](https://docs.unity3d.com/Packages/com.unity.purchasing@4.15//changelog/CHANGELOG.html) 更新至 [4.15.1](https://docs.unity3d.com/Packages/com.unity.purchasing@4.15//changelog/CHANGELOG.html)

- `com.unity.services.core`: 从 [1.17.0](https://docs.unity3d.com/Packages/com.unity.services.core@1.17//changelog/CHANGELOG.html) 更新为 [1.18.0](https://docs.unity3d.com/Packages/com.unity.services.core@1.18//changelog/CHANGELOG.html)

- `com.unity.xr.arcore`: 从 [6.3.4](https://docs.unity3d.com/Packages/com.unity.xr.arcore@6.3//changelog/CHANGELOG.html) 更新至 [6.3.5](https://docs.unity3d.com/Packages/com.unity.xr.arcore@6.3//changelog/CHANGELOG.html)

- `com.unity.xr.arfoundation`: 从 [6.3.4](https://docs.unity3d.com/Packages/com.unity.xr.arfoundation@6.3//changelog/CHANGELOG.html) 升级至 [6.3.5](https://docs.unity3d.com/Packages/com.unity.xr.arfoundation@6.3//changelog/CHANGELOG.html)

- `com.unity.xr.arkit`: 从 [6.3.4](https://docs.unity3d.com/Packages/com.unity.xr.arkit@6.3//changelog/CHANGELOG.html) 更新至 [6.3.5](https://docs.unity3d.com/Packages/com.unity.xr.arkit@6.3//changelog/CHANGELOG.html)

- `com.unity.xr.interaction.toolkit`: 从 [3.3.1](https://docs.unity3d.com/Packages/com.unity.xr.interaction.toolkit@3.3//changelog/CHANGELOG.html) 更新至 [3.3.2](https://docs.unity3d.com/Packages/com.unity.xr.interaction.toolkit@3.3//changelog/CHANGELOG.html)

- `com.unity.formats.fbx`: 从 [5.1.4](https://docs.unity3d.com/Packages/com.unity.formats.fbx@5.1//changelog/CHANGELOG.html) 更新至 [5.1.6](https://docs.unity3d.com/Packages/com.unity.formats.fbx@5.1//changelog/CHANGELOG.html)

- `com.unity.netcode.gameobjects`: 从 [2.11.2](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@2.11//changelog/CHANGELOG.html) 更新至 [2.12.0](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@2.12//changelog/CHANGELOG.html)

- `com.unity.ai.navigation`: 从 [2.0.12](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html) 更新至 [2.0.13](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html)

- `com.unity.addressables.android`: 从 [1.0.10](https://docs.unity3d.com/Packages/com.unity.addressables.android@1.0//changelog/CHANGELOG.html) 更新至 [1.1.0](https://docs.unity3d.com/Packages/com.unity.addressables.android@1.1//changelog/CHANGELOG.html)

- `com.unity.sharp-zip-lib`: [1.4.1](https://docs.unity3d.com/Packages/com.unity.sharp-zip-lib@1.4//changelog/CHANGELOG.html) 升级至 [1.4.2](https://docs.unity3d.com/Packages/com.unity.sharp-zip-lib@1.4//changelog/CHANGELOG.html)

- `com.unity.services.multiplayer`: [2.1.3](https://docs.unity3d.com/Packages/com.unity.services.multiplayer@2.1//changelog/CHANGELOG.html) 更新至 [2.2.3](https://docs.unity3d.com/Packages/com.unity.services.multiplayer@2.2//changelog/CHANGELOG.html)

- `com.unity.platformtoolkit.steam`: 从 [1.0.2](https://docs.unity3d.com/Packages/com.unity.platformtoolkit.steam@1.0//changelog/CHANGELOG.html) 更新至 [1.1.0](https://docs.unity3d.com/Packages/com.unity.platformtoolkit.steam@1.1//changelog/CHANGELOG.html)

- `com.unity.platformtoolkit.playgamesservices`: 从 [1.0.1](https://docs.unity3d.com/Packages/com.unity.platformtoolkit.playgamesservices@1.0//changelog/CHANGELOG.html) 更新至 [1.1.0](https://docs.unity3d.com/Packages/com.unity.platformtoolkit.playgamesservices@1.1//changelog/CHANGELOG.html)

- `com.unity.platformtoolkit.gdk`: 从 [1.0.1](https://docs.unity3d.com/Packages/com.unity.platformtoolkit.gdk@1.0//changelog/CHANGELOG.html) 升级至 [1.1.0](https://docs.unity3d.com/Packages/com.unity.platformtoolkit.gdk@1.1//changelog/CHANGELOG.html)

- `com.unity.platformtoolkit.gamekit`: 从 [1.0.1](https://docs.unity3d.com/Packages/com.unity.platformtoolkit.gamekit@1.0//changelog/CHANGELOG.html) 更新为 [1.1.0](https://docs.unity3d.com/Packages/com.unity.platformtoolkit.gamekit@1.1//changelog/CHANGELOG.html)

- `com.unity.platformtoolkit`: 从 [1.0.1](https://docs.unity3d.com/Packages/com.unity.platformtoolkit@1.0//changelog/CHANGELOG.html) 更新至 [1.1.0](https://docs.unity3d.com/Packages/com.unity.platformtoolkit@1.1//changelog/CHANGELOG.html)