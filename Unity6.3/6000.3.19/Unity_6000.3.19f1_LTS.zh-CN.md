# Unity 6000.3.19f1 LTS
发布于 2026年7月1日 星期三 05:37:48 GMT  
https://unity.com/releases/editor/whats-new/6000.3.19f1

# 6000.3.19f1 中的已知问题

- `6000.0.11f1`: 在包含特定资源的项目关闭时，ProfilerMutexLock 会导致崩溃
    ([UUM-144371](https://issuetracker.unity3d.com/issues/crash-on-profilermutexlock-when-closing-a-project-with-specific-assets))

- `6000.0.67f1`: [iOS] 访问 iOS 控制中心时音频中断
    ([UUM-145522](https://issuetracker.unity3d.com/issues/ios-audio-is-cut-out-when-accessing-ios-control-center))

- `资源导入器`: 进入播放模式时，编辑器在执行“(Unity) WriteObjectToVector”操作时崩溃
    ([UUM-112617](https://issuetracker.unity3d.com/issues/editor-crashes-on-unity-writeobjecttovector-when-entering-into-the-play-mode))

- `Metal`: 命令缓冲区超时错误后游戏卡死
    ([UUM-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- `文本（TextMeshPro）`: 在 TMPro 字体资源创建器中生成多线程字体图集时，UNITY_FT_Load_Glyph 调用导致崩溃
 ([UUM-125366](https://issuetracker.unity3d.com/issues/在 TMPro 字体资源生成器中生成多线程字体图集时，UNITY_FT_Load_Glyph 引发崩溃))

在编辑器中执行各种操作时，mdb_cursor_sibling 引发崩溃
    ([UUM-141720](https://issuetracker.unity3d.com/issues/crash-on-mdb-cursor-sibling-when-performing-various-actions-in-the-editor))

当运行多个 bee_backend 实例时，mono_log_write_logfile 调用会导致崩溃
    ([UUM-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))

生成字体图集时发生崩溃并产生多个堆栈跟踪
    ([UUM-141061](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-generating-font-atlas-with-sdf16-or-sdf32))



# 6000.3.19f1 发布说明

## 改进

- `编辑器`: 改进了对 LMDB MDB_BAD_RSLOT 运行时错误的诊断检查。
    ([UUM-110320](https://issuetracker.unity3d.com/issues/crash-on-sourceassetdbreadtxn-sourceassetdbreadtxn-when-idling-on-a-specific-project))



## 修复

- `2D`: 修复了在使用 `TileChangeData` 的 `Tile` 获取器属性时抛出的 `InvalidCastException` 异常。
    ([UUM-142760](https://issuetracker.unity3d.com/issues/当鼠标悬停在包含空单元格的已保存随机笔刷选择的贴图上时抛出 InvalidCastException))

- `无障碍功能`: 修复了在桌面平台上移动或调整应用程序窗口大小时，无障碍框架被重置的问题。
    ([UUM-126569](https://issuetracker.unity3d.com/issues/accessibility-frames-reset-when-the-application-window-is-moved-or-resized-on-desktop-platforms))

- `Android`: 修复了基于 GameActivity 的应用在后台运行时被强制终止的问题。
    ([UUM-143555](https://issuetracker.unity3d.com/issues/android-gameactivity-app-fails-to-relaunch-after-it-was-closed-when-a-foreground-service-started-while-app-was-backgrounded))

- `Android`: 修复了按目标架构拆分的 APK 均获得相同版本码的问题。
    ([UUM-144372](https://issuetracker.unity3d.com/issues/arm64-and-armv7-apks-return-the-same-version-code-when-split-已启用按目标架构拆分APK))

- `Audio`: 修复了在 iOS Safari 中，当应用进入后台并恢复时，循环播放的 AudioSource 会从错误的播放位置恢复的问题。
    ([UUM-144080](https://issuetracker.unity3d.com/issues/looping-audiosource-resumes-from-the-wrong-playback-position-when-the-app-is-backgrounded-and-resumed-on-ios-safari))

- `文档`: 修复了 UI 工具包文档中的间距问题。

- `编辑器`: 新增了一项选项，用于阻止模型导入器执行全项目范围的纹理搜索。
    (UUM-137345)

- `编辑器`: 更改了在提示重启编辑器时，图形 API 自动切换逻辑的工作方式。
    ([UUM-140948](https://issuetracker.unity3d.com/issues/auto-graphics-api-chackbox-will-not-stay-disabled-if-the-api-change-is-canceled))

- `编辑器`: 修复了复制构建配置文件时，已添加但尚未编辑的“播放器设置”覆盖项会丢失的问题。
    (UUM-141702)

- `编辑器`: 修复了在更改场景模板时，场景模板检查器中的依赖项列表未更新的问题。
    ([UUM-143123](https://issuetracker.unity3d.com/issues/在场景模板检查器中选择依赖项类型时，排序依赖项会导致控制台出现ObjectDisposedException和NullReferenceException错误))

- `编辑器`: 修复了在 ATG 中将 FontAsset 从静态切换为动态时发生的崩溃问题。
    ([UUM-144549](https://issuetracker.unity3d.com/issues/windows-editor-freezes-and-consumes-all-available-disk-space-when-changing-a-referenced-font-assets-atlas-population-mode-from-static-to-dynamic))

- `编辑器`: 修复了 Linux 编辑器中鼠标前进和后退按钮无法响应的问题。
    ([UUM-143528](https://issuetracker.unity3d.com/issues/input-system-does-not-register-the-backbutton-or-forwardbutton-when-using-the-linux-editor))

- `编辑器`: 修复了在 FBX 模型预制体实例上使用包含嵌套序列化数组的组件时，检查器滚动区域会拉伸的问题。
    ([UUM-135480](https://issuetracker.unity3d.com/issues/inspector-scroll-area-stretches-when-using-components-with-nested-serialized-arrays-on-fbx-model-prefab-instances))

- `编辑器`: 修复了在 RedrawFromNative 期间若打开或关闭新窗口，InspectorWindow 会抛出异常的问题。
    ([UUM-141990](https://issuetracker.unity3d.com/issues/invalidoperationexception-is-thrown-when-clicking-ctrl-plus-z-after-opening-gradient-editor))

- `Editor`: 修复了“图形设置”中的重置问题。
    ([UUM-139127](https://issuetracker.unity3d.com/issues/resetting-graphics-settings-in-project-settings-window-throws-gpuresidentdrawer-batchrenderergroup-variants-must-be-keep-all-warnings-in-the-console-window))

- `编辑器`: 修复了在使用 Wacom 设备时，退出下拉菜单选择后“检查器”进入滚动模式的问题。
    ([UUM-138133](https://issuetracker.unity3d.com/issues/inspector-enters-scroll-mode-when-exiting-dropdown-menu-selection-and-using-wacom-device))

- `Editor`: 修复了 Perforce 中未跟踪文件夹导致 VCCache 陷入无限重新查询循环的问题。
    ([UUM-143313](https://issuetracker.unity3d.com/issues/cpu-usage-spikes-when-perforce-version-control-is-set-up-and-ai-assistant-is-installed))

- `编辑器`: 改进了向量的哈希码计算。
    ([UUM-143005](https://issuetracker.unity3d.com/issues/hdrp-bloom-renders-with-a-purple-blue-or-green-anomaly-in-the-game-view-when-toggling-bloom-anamorphic-volume-settings-with-camera-anamorphism-set-为1且宽高比可被16整除，同时图形API设置为DX11或DX12时，游戏视图中渲染的HDRP光晕效果会出现紫色、蓝色或绿色的异常现象))

- `编辑器`: 使用“重置”时，光照贴图模式和雾效模式会正确恢复。
    ([UUM-139005](https://issuetracker.unity3d.com/issues/dropdown-values-are-not-reverted-when-selecting-reset-in-graphics-project-settings))

- `编辑器`: 当启用“重新加载域”功能并进入“游戏模式”时，多人游戏模式的 `enterPlayModeFromMppm` 分析事件未被发送。
    (UUM-144601)

- `编辑器`: 修复了预制体使用保留字段时可能导致的崩溃问题。
    ([UUM-144557](https://issuetracker.unity3d.com/issues/crash-on-saveprefabasset-when-selecting-a-specific-prefab))

- `编辑器`: 层级设置编辑器窗口在调整大小时能正确处理长文本。
    ([UUM-138911](https://issuetracker.unity3d.com/issues/tier-settings-editor-window-does-not-handle-long-text-properly-on-resize))

- `编辑器`: 更新了画布渲染器的图标。
    ([UUM-142443](https://issuetracker.unity3d.com/issues/canvas-renderer-component-uses-a-low-resolution-icon))

- `Graphics`: 修复了在尝试加载 IDAT 块损坏的 PNG 文件时，“ImageConversion.LoadImage” 可能导致内存泄漏的问题。
    ([UUM-143641](https://issuetracker.unity3d.com/issues/alloc-temp-main-leaks-a-persistent-4096-byte-allocation-when-imageconversion-dot-loadimage-fails-to-decode-a-png-with-valid-headers-but-corrupted-idat-chunk-data))

- `Graphics`: 当材质启用了 GPU 实例化，但关联的着色器缺少实例化着色器变体时，防止运动向量被破坏。
    ([UUM-130621](https://issuetracker.unity3d.com/issues/gameobject-shows-visual-corruption-due-to-incorrect-previous-transform-matrix-while-using-active-spacewarp))

- `HDRP`: 通过修正 SSGI 计算着色器调度中的参数类型不匹配问题，修复了在使用屏幕空间全局照明（SSGI）配合自适应探针体积时出现的灯光颜色异常问题。
    ([UUM-143777](https://issuetracker.unity3d.com/issues/lighting-sometimes-produces-incorrect-colors-when-baking-lightmaps-with-screen-space-global-illumination-and-adaptive-probe-volumes))

- `Linux`: 添加了输入文本检查，以防止使用 AltGr 进行文本组合，从而避免触发快捷键路径。
    ([UUM-142414](https://issuetracker.unity3d.com/issues/linux-character-at-is-not-inputted-when-pressing-altgr-plus-q-with-a-german-keyboard-layout))

- `Linux`: 修复了在 Linux 编辑器中构建 Windows 播放器以及创建 Visual Studio 解决方案时出现的错误。
    ([UUM-140187](https://issuetracker.unity3d.com/issues/linuxeditor-building-for-windows-throws-agilitysdk-dll-could-not-be-retrieved-when-create-visual-studio-solution-was-enabled-before-switching-build-platform-to-windows))

- `网络`: 更新 Artifactory 中的 libcurl 版本，该版本采用了经过更新的 nghttp2，以缓解 CVE-2026-27135 漏洞。
    (UUM-140912)

- `粒子`: 修复了 URP 粒子光照（Particle Lit）和简单光照（Simple Lit）着色器的问题，确保其在延迟渲染（Deferred）和延迟+渲染（Deferred+）模式下，当以背景为渲染目标或应用 SSAO 时，能够正确进行光照渲染。
    (UUM-140364)

- `物理`: 修复了因已禁用的刚体组件实例使其内部 Actor 无限期存活而导致的崩溃问题。
    ([UUM-143658](https://issuetracker.unity3d.com/issues/crash-on-physicscommands-physx-bodysetpose-when-entering-play-mode-in-a-specific-project))

- `物理`: 修复了在特定项目中，当对未使用多盒子剪枝广相位（multi-box pruning broadphase）的物理场景调用 `Physics.RebuildBroadphaseRegions 方法中发生的崩溃，该问题可能出现在对未使用多盒子修剪广相（multi-box prunning broadphase）的物理场景调用该方法时。
    ([UUM-144472](https://issuetracker.unity3d.com/issues/physics-dot-rebuildbroadphaseregions-does-not-repopulate-them-with-pre-existing-shapes))

- `Physics`: 修复了调用 Physics.RebuildBroadphaseRegions 时，可能导致已存在的 Collider 组件被排除在新生成的广相区域之外的问题。
    ([UUM-144472](https://issuetracker.unity3d.com/issues/physics-dot-rebuildbroadphaseregions-does-not-repopulate-them-with-pre-existing-shapes))

- `Physics 2D`: 在现有的 UI-Toolkit 属性抽屉旁，为 PhysicsMask、ContactFilter、QueryFilter、PhysicsUserData、PolygonGeometry、PhysicsRotate 和 PhysicsLayer 添加了 IMGUI 属性抽屉。
    ([UUM-142727](https://issuetracker.unity3d.com/issues/no-gui-implemented-is-displayed-when-using-physicsmask-with-a-customeditor))

- `Physics 2D`: 修复了“PhysicsBody.collisionThreshold”被忽略的问题，使其能够控制 PhysicsBody 何时对所有形状类型（包括链段）进行连续碰撞检测。
    ([UUM-144698](https://issuetracker.unity3d.com/issues/physicsbody-dot-collisionthreshold-not-correctly-controlling-ccd))

- `Profiler`: 修复了 ProfilerSymbolsDelayedDeletion::AddCloneObject 中的崩溃问题。
    ([UUM-144194](https://issuetracker.unity3d.com/issues/crash-on-profilersymbolsdelayeddeletion-addcloneobject-when-deserializing-an-object-instantiate-marker-with-a-dangling-slash-corrupt-name-string))

- `Profiler`: 修复了当玩家使用“构建并运行”/“自动连接到 Profiler”设置时，Profiler 截图捕获速率/时机方面的问题。
    (UUM-144511)

- `Profiler`: 改进了 PersistentManager.Remapper 的内存追踪功能。
    (UUM-141167)

- `场景/游戏视图`: 修复了在使用多显示器时，游戏视图缩放滑块偶尔会出现异常行为的问题。
    ([UUM-135174](https://issuetracker.unity3d.com/issues/game-view-scale-drops-lower-than-is-possible-to-choose-manually-when-a-domain-reload-occurs))

- `Shadergraph`: 修复了在撤销或重做渐变更改时，渐变选择器窗口会关闭的问题。
    ([UUM-141977](https://issuetracker.unity3d.com/issues/hdr-gradient-editor-window-closes-when-undoing-changes-in-sample-gradient-node-with-ctrl-plus-z))

- `Shadergraph`: 修复了按下 Esc 键时节点搜索窗口无法关闭的问题。
    ([UUM-143233](https://issuetracker.unity3d.com/issues/shader-graphs-create-node-menu-cannot-be-closed-with-esc-button))

- `Shaders`: 现在使用渲染对象覆盖着色器时，原始材质的属性将被保留。
    ([UUM-100850](https://issuetracker.unity3d.com/issues/material-properties-are-not-preserved-when-overriding-shader-using-render-objects))

- `文本`: 修复了 macOS 系统中编辑器文本字段内 CJK 字符不可见的问题。
    ([UUM-144095](https://issuetracker.unity3d.com/issues/characters-are-invisible-in-the-textfield-when-certain-japanese-characters-are-used))

- `UI`: 修复了当内容完全适配时，ScrollView 拖动滚动会进入空白区域的问题。
    ([UUM-142498](https://issuetracker.unity3d.com/issues/blank-area-appears-at-the-top-of-inspector-and-build-settings-windows-使用Wacom数位板笔触摸并向下拖动时))

- `UI Toolkit`: 修复了 Painter2D 忽略 FillGradient.radius 的问题。
    ([UUM-138358](https://issuetracker.unity3d.com/issues/the-radius-of-a-radial-gradient-does-not-change-when-changing-its-fillgradient-dot-radius-property))

- `UI Toolkit`: 修复了抗锯齿弧形编码中 SVG 的轻微镶嵌问题。
    ([UUM-144586](https://issuetracker.unity3d.com/issues/svg-图标在抗锯齿弧形编码中存在镶嵌问题，但基本三角剖分无此问题))

- `UI Toolkit`: 修复了当多个检查器窗口显示包含 Grid Layout Group 组件的不同对象时，进入播放模式后抛出的 MissingReferenceException 错误。
    ([UUM-145062](https://issuetracker.unity3d.com/issues/missingreferenceexception-errors-are-thrown-after-entering-play-mode-when-multiple-inspector-windows-are-displaying-different-objects-with-grid-layout-group-component))

- `UI Toolkit`: 修复了作为 VectorImage 导入的 SVG 在项目浏览器中的图标显示问题。
    ([UUM-141655](https://issuetracker.unity3d.com/issues/svgs-imported-as-vector-image-dont-show-a-static-preview-in-the-project-browser))

- `UI Toolkit`: 修复了将 SVG 导入为“抗锯齿弧形编码”时，径向焦点无法正常工作的问题。
    ([UUM-138043](https://issuetracker.unity3d.com/issues/svg-radial-gradient-focus-isnt-working-with-antialiased-arc-encodings))

- `UI Toolkit`: 修复了在现有上下文模式结束后立即触发撤销/重做操作时，UI 构建器抛出空引用异常的问题。
    ([UUM-142693](https://issuetracker.unity3d.com/issues/index当在上下文菜单中撤销打开实例中元素的重命名操作时，会抛出越界异常和空引用异常，且该元素从 UI 构建器中消失))

- `撤销系统`: 更新了 EraseUndos 中的边界检查。
    (UUM-142925)

- `VFX 图`: 提高了“与有符号距离场碰撞”模块在粒子静止状态下的稳定性。
    ([UUM-99382](https://issuetracker.unity3d.com/issues/vfx-graph-position-jitter-in-reststate-with-collision-sdf))

- `Windows`: 修复了在独立运行的 Player 构建中使用输入管理器时，Windows 手写笔输入无法生成鼠标指针事件 \(`Input.GetMouseButtonDown`\) 的问题。
    ([UUM-140737](https://issuetracker.unity3d.com/issues/windows-pen-input-does-not-generate-mouse-pointer-events-when-using-input-manager))

- `Windows`: 修复了在 Windows 触摸屏设备上执行捏合手势后，UI 工具包按钮对触摸无响应的问题。
    ([UUM-138595](https://issuetracker.unity3d.com/issues/在 Windows 触控设备上使用新输入系统执行多点触控手势时，UI 工具包按钮不再响应单次点击))

- `Windows`: 修复了 Windows IL2CPP 构建时出现 LNK1104 错误的问题。
    ([UUM-139929](https://issuetracker.unity3d.com/issues/使用 IL2CPP 构建 Windows x64 版本时，若系统已安装 Visual Studio 2026 和 2022，会因链接错误导致构建失败))

- `XR`: 修复了 VrsResources.DisposeResources() 中已存在的内存泄漏问题。
    (UUM-143173)




## 6000.3.19f1 版本中的包变更

## 已更新的包

- `com.unity.netcode`: [1.13.2](https://docs.unity3d.com/Packages/com.unity.netcode@1.13//changelog/CHANGELOG.html) 更新至 [1.14.0](https://docs.unity3d.com/Packages/com.unity.netcode@1.14//changelog/CHANGELOG.html)

- `com.unity.probuilder`: 从 [6.0.9](https://docs.unity3d.com/Packages/com.unity.probuilder@6.0//changelog/CHANGELOG.html) 升级至 [6.1.2](https://docs.unity3d.com/Packages/com.unity.probuilder@6.1//changelog/CHANGELOG.html)

- `com.unity.services.authentication`: 从 [3.6.1](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.6//changelog/CHANGELOG.html) 更新至 [3.7.1](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.7//changelog/CHANGELOG.html)

- `com.unity.splines`: 从 [2.8.4](https://docs.unity3d.com/Packages/com.unity.splines@2.8//changelog/CHANGELOG.html) 更新至 [2.9.0](https://docs.unity3d.com/Packages/com.unity.splines@2.9//changelog/CHANGELOG.html)

- `com.unity.netcode.gameobjects`: 从 [2.12.0](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@2.12//changelog/CHANGELOG.html) 更新至 [2.13.0](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@2.13//changelog/CHANGELOG.html)

- `com.unity.multiplayer.tools`: 从 [2.2.8](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@2.2//changelog/CHANGELOG.html) 更新至 [2.2.9](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@2.2//changelog/CHANGELOG.html)