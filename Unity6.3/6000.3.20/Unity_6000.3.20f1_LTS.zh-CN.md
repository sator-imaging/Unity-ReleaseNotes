# Unity 6000.3.20f1 LTS
发布于 2026年7月16日 星期四 13:36:03 GMT  
https://unity.com/releases/editor/whats-new/6000.3.20f1

# 6000.3.20f1 中的已知问题

- `6000.0.23f1`: 在动画器评估期间，若 RigBuilder 重新绑定后退出播放模式，Animator::OnPlayableUnbind 会引发崩溃
    ([UUM-146750](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146750))

- `6000.0.67f1`: [iOS] 访问 iOS 控制中心时音频中断
    ([UUM-145522](https://issuetracker.unity3d.com/issues/ios-audio-is-cut-out-when-accessing-ios-control-center))

- `资源导入器`: 进入播放模式时，编辑器在执行“(Unity) WriteObjectToVector”操作时崩溃
    ([UUM-112617](https://issuetracker.unity3d.com/issues/editor-crashes-on-unity-writeobjecttovector-when-entering-into-the-play-mode))

- `Metal`: 命令缓冲区超时错误后游戏卡死
    ([UUM-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

当有多个 bee_backend 实例同时运行时，在调用 mono_log_write_logfile 时发生崩溃
    ([UUM-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))

生成字体图集时发生崩溃，并产生多个堆栈跟踪
    ([UUM-141061](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-generating-font-atlas-with-sdf16-or-sdf32))



# 6000.3.20f1 发布说明

## 改进

- `构建系统`: 将捆绑的 7-Zip 更新至 26.02 版本。

- `图形`: 更新了 Mipmap 流式传输手册页面，说明了 Unity 如何根据网格 UV 数据和摄像机位置选择 Mipmap 级别， 澄清了 Unity 无法计算级别的对象的行为（包括粒子系统等程序生成的几何体），并添加了 `Texture2D.requestedMipmapLevel` 代码示例。
    ([UUM-131691](https://issuetracker.unity3d.com/issues/texture-rendered-at-different-fidelity-with-particle-system-renderer-when-using-a-different-material-derived-from-the-same-texture-with-identical-settings))

- `物理`: 在“项目设置” -&gt; “物理” -&gt; “设置” -&gt; “游戏对象”下，新增了一个下拉菜单，可用于在多线程和单线程模拟之间切换。
    (UUM-144574)



## 修复

- `2D`: 修复了检查器窗口中“精灵图集导入器”按钮的“打开参考文档”功能跳转至过时版本手册的问题。
    ([UUM-133073](https://issuetracker.unity3d.com/issues/open-reference-for-sprite-atlas-importer-button-in-inspector-window-redirects-to-an-outdated-version-of-the-manual))

- `2D`: 修复了“光批处理调试器”中按图层名称排序后未刷新的问题。
    ([UUM-136214](https://issuetracker.unity3d.com/issues/除非重新启动窗口或在重命名现有图层时添加新图层，否则“光批处理调试器”窗口中的图层名称不会更新))

- `2D`: 修复了在构建播放器时，所有包含在构建场景中的精灵图集纹理会一直保留在编辑器内存中的问题。
    ([UUM-137607](https://issuetracker.unity3d.com/issues/sprite-atlas-textures-from-all-included-build-scenes-persist-in-editor-memory-when-building-the-player))

- `2D`: 修复了在编辑状态下的“贴图调色板”上拖放操作时，创建新“贴图”资源会引发异常的问题。
    ([UUM-143122](https://issuetracker.unity3d.com/issues/missingreferenceexception-during-image-import-to-tile-palette-when-in-tile-palette-edit-mode))

- `2D`: 修复了 Light2D 序列化冲突。
    (UUM-141743)

- `2D`: 修复了在“块”模式下使用 `TilemapRenderer` 时，翻转瓦片的法线贴图问题。
    ([UUM-143429](https://issuetracker.unity3d.com/issues/flipped-tiles-with-normal-maps-are-inverted-with-tilemaprenderer-with-chunk-mode))

- `2D`: 修复了从“贴图调色板”使用“选择工具”后，切换至“绘图”等其他工具时，场景被标记为“已修改”的问题。
    ([UUM-141736](https://issuetracker.unity3d.com/issues/scene-becomes-dirty-when-selecting-a-tile-palette-cell-and-then-switching-to-the-paint-tool))

- `2D`: 修复了使用网格选择工具（GridSelectionTool）调整缩放比例至负值时，图块出现闪烁的问题。
    ([UUM-141782](https://issuetracker.unity3d.com/issues/tile-sprite-flickers-when-scaled-to-negative-values))

- `2D`: 使用 Delete 或 Backspace 键删除网格选择时，解锁色板以便编辑。
    ([UUM-141744](https://issuetracker.unity3d.com/issues/unable-to-delete-tiles-from-tile-palette-permanently-with-the-delete-key))

- `无障碍功能`: 记录了开发人员必须执行的步骤，以便 `AccessibilityRole.Slider`、`AccessibilityRole.TextField` 和 `AccessibilityRole.SearchField` 无障碍节点在 Android 上接收硬件键盘输入。
    ([UUM-126557](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-126557))

- `Android`: 将未使用的 Tools 26.1.1 下载文件替换为空文件夹。
    (UUM-141878)

- `Audio`: 修复了 `Sound.getOpenState` 在异步加载声音时因数据竞争而导致的罕见崩溃问题。
    ([UUM-145498](https://issuetracker.unity3d.com/issues/crash-in-fmod-when-using-load-in-background))

- `构建系统`: 在调用 dotnet 时，将 MSBUILDDEBUGPATH 添加到其他方法中。

- `核心`: 修复了克隆 GameObject 时 `Transform` 序列化值未正确初始化的问题。
    ([UUM-131305](https://issuetracker.unity3d.com/issues/transform-corruption-and-slash-or-crash-on-physx-createcharactercontroller-when-spawning-physics-objects-into-prefab-stages))

- `文档`: 增加了有关组件使用的更多资源。

- `文档`: 为 UITK 弹出窗口示例代码及操作步骤补充了更多背景信息和细节。

- `文档`: 更新了 VFX 运算符 Reciprocal 中错误的 'out' 属性。
    (UUM-144446)

- `编辑器`: 音频：修复了打开包含损坏的音频混音器资源的项目时编辑器崩溃的问题。
    ([UUM-143706](https://issuetracker.unity3d.com/issues/crash-on-audiomixercontroller-removeinvalidsendlevelguidsrecursive-when-opening-a-project-with-specific-audio-files-for-the-first-time))

- `编辑器`: 修复了在编辑器关闭时，受管 `DomainUnload` 处理程序执行 `UnityEngine.Object` 空值检查时发生的崩溃（`ProfilerMutexLock / 断言 gPersistentManager \!= NULL`）。
    ([UUM-144371](https://issuetracker.unity3d.com/issues/crash-on-profilermutexlock-when-closing-a-project-with-specific-assets))

- `Editor`: 修复了当场景文件中包含一个预制体实例，且其添加的组件列表格式不正确时发生的崩溃问题。
    ([UUM-145507](https://issuetracker.unity3d.com/issues/crash-on-deleteprefabinstanceobjectsformissingprefabs-when-opening-a-specific-scene))

- `编辑器`: 修复了将“搜索”窗口停靠后未能正确设置 QueryTree 处理程序的问题。
    ([UUM-132981](https://issuetracker.unity3d.com/issues/nullreferenceexception-errors-在停靠的搜索窗口中点击已保存的内置报告时，控制台会抛出错误))

- `Editor`: 修复了在 Wayland 环境下运行时，将文件拖入编辑器所导致的 LinuxEditor 错误。
    ([UUM-111593](https://issuetracker.unity3d.com/issues/linux-the-error-releasebutton-expects-buttonid-is-thrown-when-trying-to-add-file-using-drag-and-hold-in-the-project-window))

- `编辑器`: 修复了在使用两个指向同一字体的不同 FontAssets 时，ATG 出现的字体显示异常问题。
    (UUM-133996)

- `编辑器`: 修复了在使用“创建空父对象”（CreateEmptyParent）菜单项后，撤销/重做操作会清空默认父对象的问题。
    ([UUM-115213](https://issuetracker.unity3d.com/issues/performing-redo-create-empty-parent-object-action-resets-default-parent-object-in-the-scene))

- `编辑器`: 修复了选择一个平台并点击“添加构建配置文件”后，该平台在“平台浏览器”对话框中未被选中的问题。
    (UUM-130650)

- `编辑器`: 防止在选择操作打开原生模态对话框时，对象选择器出现卡死现象。
    ([UUM-139847](https://issuetracker.unity3d.com/issues/object-selector-becomes-unresponsive-when-selecting-root-ui-document-as-data-source-for-add-binding-in-ui-builder))

- `编辑器`: 修复了 LMDB 中的轻微内存泄漏问题。
    (UUM-138144)

- `编辑器`: 编辑器现在会在将播放器数据写入之前对引用进行清理，以防止类型不匹配。
    ([UUM-143556](https://issuetracker.unity3d.com/issues/crash-in-player-when-calling-setactive-on-a-gameobject-with-a-type-mismatched-reference))

- `编辑器`: 对 `QuaternionEulerField` 的输入进行了验证，因此不再接受 NaN 和无穷大作为有效输入。
    ([UUM-142032](https://issuetracker.unity3d.com/issues/在游戏对象刷子方向值字段中输入 NaN 或无穷大值会导致控制台不断出现四元数相关错误，且除非在贴图调色板窗口中撤销该值，否则该问题将持续存在))

- `GI`: 修复了在“照明 / 自适应探针体积 / 当前烘焙集”属性中选择当前设置的 APV 烘焙集无法正常工作的问题。
    ([UUM-145389](https://issuetracker.unity3d.com/issues/apv-data-becomes-incorrect-when-reselecting-the-currently-active-baking-set))

- `图形渲染`: 修复了在 DirectX12 分割图形任务中使用光线追踪时发生的崩溃问题。
    (UUM-145956)

- `Graphics`: 解决了在 Windows 系统上使用 Vulkan 并启用“拆分图形任务”时，缓存中可能插入空值的问题，该问题会导致 DrawCalls 尝试向已关闭的命令缓冲区绘制，从而引发崩溃。
    (UUM-132307)

- `IL2CPP`: 修复了在 Linux 上生成空 .usym 文件的问题。
    ([UUM-142527](https://issuetracker.unity3d.com/issues/linux-stack-trace-file-path-and-line-number-information-is-missing-当-il2cpp-堆栈跟踪信息-设置为-方法名-文件名-和-行号-时))

- `Kernel`: 修复了作业系统中涉及大量外部线程和手动作业的潜在死锁问题。
    (UUM-143073)

- `网络`: 修复了来自 UnityWebRequest 的 Curl 错误可能无法被正确记录的情况，该问题曾导致故障难以调试。请注意，即使在此情况下，错误仍会正确上报给调用代码。此缺陷仅影响日志记录。
    ([UUM-145433](https://issuetracker.unity3d.com/issues/unitywebrequest-can-lose-error-messages-from-curl))

- `网络`: 修复了 UnityWebRequest 中的一项问题：在恢复上传请求时，有时会记录错误代码 26 或 65（“无法执行必要的数据回卷”）。
    ([UUM-144767](https://issuetracker.unity3d.com/issues/webrequest-missing-curlopt-seekfunction-causes-curl-error-26-on-post-retry-with-reused-connections))

- `包管理器`: 修复了 Unity 启动时部分包的签名图标显示错误的问题。
    ([UUM-143201](https://issuetracker.unity3d.com/issues/signed-registry-packages-show-green-shield-icon-when-show-pre-release-package-versions-is-toggled-on))

- `分析器`: 修复了在 macOS 上直接加载分析数据时，无法过滤相关文件类型（.data、.raw）的问题。
    ([UUM-139554](https://issuetracker.unity3d.com/issues/profiler-data-stream-has-invalid-signature-errors-are-thrown-when-loading-a-highlights-file-in-the-profiler))

- `Search`: 修复了在域名重新加载时，由于后台线程未被正确取消，导致 Search LMDB 崩溃的问题。
    ([UUM-141720](https://issuetracker.unity3d.com/issues/crash-on-mdb-cursor-sibling-when-performing-various-actions-in-the-editor))

- `Search`: 修复了在域重新加载过程中，部分后台线程成为孤儿线程且无法停止，导致 Search LMDB 崩溃的问题。
    ([UUM-143640](https://issuetracker.unity3d.com/issues/crash-on-mdb-database-getmapsize-when-domain-reloads-while-background-search-indexing-is-active))

- `SRP Core`: 移除了 HDR 输出渲染过程中的一项罕见托管内存分配操作，该操作可能在 .NET 于帧与帧之间回收池化数组缓冲区时间歇性发生。
    (UUM-145447)

- `Text`: 修复了在 FT_Done_Face 事件触发时编辑器关闭导致崩溃的问题。
    ([UUM-144575](https://issuetracker.unity3d.com/issues/crash-on-unity-ft-done-face-when-closing-the-editor-after-rendering-text-with-the-advanced-text-generator-using-a-runtime-created-font-asset))

- `UI 工具包`: 对无效的 stroke-miterlimit 值进行裁剪处理，而非导致 SVG 导入失败。
    ([UUM-120825](https://issuetracker.unity3d.com/issues/svg-fails-to-import-when-stroke-miterlimit-is-less-than-1))

- `UI Toolkit`: 修复了一个问题，该问题会导致在使用自定义着色器输出常量颜色时，椭圆形显示为矩形。
    ([UUM-145855](https://issuetracker.unity3d.com/issues/arc-aa-isnt-applied-when-using-a-custom-shader-that-outputs-a-constant))

- `UI Toolkit`: 修复了在调试检查器中向列表添加或移除元素时抛出 ObjectDisposedException 的问题。
    ([UUM-143676](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-143676))

- `URP`: 修复了 URP 独立播放器构建中导致播放器日志中出现内存泄漏警告的问题。
    ([UUM-115886](https://issuetracker.unity3d.com/issues/jobtempalloc-memory-leak-warning-is-thrown-when-the-player-is-shut-down))

- `URP`: 修复了在启用“污垢纹理”（Dirt Texture）但其值为空时，Bloom 效果的运行时着色器变体选择错误的问题。
    ([UUM-141980](https://issuetracker.unity3d.com/issues/bloom-post-processing-effect-in-urp-is-missing-in-a-build-when-dirt-texture-is-enabled-in-the-bloom-override-of-a-global-volume))

- `Web`: 修复了当 Player Graphics API 设置为 WebGPU 时，VideoPlayer.frameReady 在播放过程中仅触发一次的问题。
    ([UUM-141418](https://issuetracker.unity3d.com/issues/web-videoplayer-dot-frameready-event-fires-only-once-in-a-video-when-the-player-graphics-api-is-set-to-webgpu))

- `WebGL`: WebGPU：修复了部分移动设备因缺少 float32-blendable WebGPU 扩展而导致的错误。
    ([UUM-145735](https://issuetracker.unity3d.com/issues/webgpu-urp-errors-when-float32-blendable-isnt-available))

- `WebGL`: \[WebGPU\] 修复了在销毁和创建着色器时可能发生的崩溃问题。
    ([UUM-145390](https://issuetracker.unity3d.com/issues/type-error-is-thrown-when-a-new-computeshader-is-instantiated-after-destroying-previous-computeshader))

- `Windows`: 修复了在 Windows 系统上使用新输入系统时，通过 `<Pointer>/position` 绑定，笔的位置在“游戏视图”中会受限于特定区域的问题。
    ([UUM-142269](https://issuetracker.unity3d.com/issues/pen-position-gets-constrained-to-a-limited-area-when-using-a-stylus-in-game-view-or-player))




## 6000.3.20f1 版本中的包变更

## 已更新的包

- `com.unity.ads`: 从 [4.16.4](https://docs.unity3d.com/Packages/com.unity.ads@4.16//changelog/CHANGELOG.html) 更新至 [4.19.0](https://docs.unity3d.com/Packages/com.unity.ads@4.19//changelog/CHANGELOG.html)

- `com.unity.services.cloudcode`: 从 [2.10.2](https://docs.unity3d.com/Packages/com.unity.services.cloudcode@2.10//changelog/CHANGELOG.html) 更新至 [2.10.3](https://docs.unity3d.com/Packages/com.unity.services.cloudcode@2.10//changelog/CHANGELOG.html)

- `com.unity.services.vivox`: 从 [16.10.0](https://docs.unity3d.com/Packages/com.unity.services.vivox@16.10//changelog/CHANGELOG.html) 更新为 [16.11.0](https://docs.unity3d.com/Packages/com.unity.services.vivox@16.11//changelog/CHANGELOG.html)

- `com.unity.xr.compositionlayers`: 从 [2.4.0](https://docs.unity3d.com/Packages/com.unity.xr.compositionlayers@2.4//changelog/CHANGELOG.html) 升级至 [2.5.0](https://docs.unity3d.com/Packages/com.unity.xr.compositionlayers@2.5//changelog/CHANGELOG.html)

- `com.unity.services.multiplayer`: 从 [2.2.3](https://docs.unity3d.com/Packages/com.unity.services.multiplayer@2.2//changelog/CHANGELOG.html) 更新至 [2.2.4](https://docs.unity3d.com/Packages/com.unity.services.multiplayer@2.2//changelog/CHANGELOG.html)