# Unity 6000.3.11f1 LTS
发布于 星期三, 11 三月 2026 14:52:35 GMT
https://unity.com/releases/editor/whats-new/6000.3.11f1

# 6000.3.11f1 中的已知问题

- `6000.2.0a10`: 首次打开项目时，TexturesD3D12::CreateTextureInternal()崩溃
    ([uum-135024](https://issuetracker.unity3d.com/issues/crash-on-checkdevicestatus-when-opening-a-project-for-the-first-time))

- `6000.3.5f1`: 在启用雕刻的情况下移动导航网格障碍物时增加了 CPU 占用率
    ([uum-133911](https://issuetracker.unity3d.com/issues/increased-cpu-usage-when-moving-navmesh-obstacles-with-carving-enabled))

- `6000.5.0a3,6000.4.0b8,6000.3.8f1,6000.0.68f1`: [iOS] 在 Info.plist 中添加 UIApplicationSceneManifest 时，应用程序运行时不会调用 Application.deepLinkActivated
    ([uum-135497](https://issuetracker.unity3d.com/issues/ios-application-dot-deeplinkactivated-does-not-get-invoked-while-app-is-running-when-uiapplicationscenemanifest-is-added-in-info-dot-plist))

- 核心运行时实体 ContentManagement GUID 不稳定，每次将播放器构建到不同目录时都会变得不同
    ([uum-129944](https://issuetracker.unity3d.com/issues/entities-contentmanagement-guids-are-unstable-and-become-different-each-time-a-player-is-built-to-a-different-directory))

- `金属"`: 命令缓冲区超时错误后游戏冻结
    ([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- `金属"`: MacOS 在编辑器中的最小项目在播放模式下出现卡顿
    ([uum-85256](https://issuetracker.unity3d.com/issues/macos-stutters-in-a-minimal-project))

使用 DirectX 12 在独占全屏模式下切换焦点时播放器崩溃
    ([uum-134743](https://issuetracker.unity3d.com/issues/player-crash-when-switching-focus-in-exclusive-fullscreen-mode-with-directx-12))

[硅] 当 Razer Synapse 应用程序打开项目时，os_unfair_recursive_lock_lock_with_options 会崩溃
    ([uum-135043](https://issuetracker.unity3d.com/issues/silicon-crash-on-os-unfair-recursive-lock-lock-with-options-when-opening-a-project-while-the-razer-synapse-app-is-open))



# 6000.3.11f1 发布说明

## 功能

- `许可证支持 Kerberos 代理身份验证。

- macOS`: 在 Mac 播放器上添加了对 `CAMetalDisplayLink` 的支持。
    默认情况下是禁用的，可以在播放器设置中切换 "Use MetalDisplayLink （仅限 Mac 播放器）"来启用。另外，你也可以使用环境变量 "UNITY_USE_METAL_DISPLAY_LINK=1"。
    使用 "CAMetalDisplayLink "可减少卡顿并改善帧间距。它还会使 `Time.deltaTime` 更加稳定。



## 改进

- `Android`: 在 AndroidPlayer 初始化过程中添加了剖析标记。
    ([uum-135048](https://issuetracker.unity3d.com/issues/android-fix-profiling-during-early-application-startup-to-match-other-platforms))

- 构建系统将与编辑器捆绑的 7-Zip 更新至 26.00。

- 安装程序删除了 Windows 系统上的 .NET 3.5 激活。大大缩短了直接使用安装程序的安装时间。
    (UUM-133360)

- `物理 2D"`: PhysicsComposer 现在实现了 IDisposable 接口，其中公共 IDisposable.Dispose 方法简单地调用了 "PhysicsComposer.Destroy\(\)"。
    ([UUM-134952](https://issuetracker.unity3d.com/issues/fix-for-6000-dot-6-x-fix-some-api-issues-from-user-feedback))

- 插件将 DLSS SDK 从 v310.4.0 升级到 v310.5.0，包括为 DLSS 超级分辨率添加预设 L 和 M。

- SRP 核心改进了 `VolumeManager` 收集 `VolumeComponent` 类型的方式，以避免播放器启动时反射开销过慢。
    (UUM-134911)



## API 更改

- `物理 2D"`: 已添加： 已添加 "PhysicsUserData.objectValueId "属性，用于显示 "objectValue "属性所使用的实体 ID。  该属性现在还以工具提示的形式显示实体 ID、对象名称和类型，如果没有实体，则显示 "无"，如果实体 ID 不代表有效对象，则显示 "无效对象 ID"。
    ([uum-134952](https://issuetracker.unity3d.com/issues/fix-for-6000-dot-6-x-fix-some-api-issues-from-user-feedback))

- `物理 2D"`: 新增： 已添加 "PhysicsUserData.objectValueId "属性，以显示 "objectValue "属性使用的实体 ID。  该属性现在还以工具提示的形式显示实体 ID、对象名称和类型，如果没有实体，则显示 "无"，如果实体 ID 不代表有效对象，则显示 "无效对象 ID"。
    ([uum-134952](https://issuetracker.unity3d.com/issues/fix-for-6000-dot-6-x-fix-some-api-issues-from-user-feedback))

- `物理 2D"`: 新增： PhysicsComposer 现在可以使用 "PhysicsComposer.GetComposers\(\)" 和 "PhysicsComposer.DestroyAll\(\)" 方法获取或销毁所有合成器。
    ([uum-134952](https://issuetracker.unity3d.com/issues/fix-for-6000-dot-6-x-fix-some-api-issues-from-user-feedback))

- `物理 2D"`: 新增： PhysicsComposer 现在可以使用 "PhysicsComposer.GetComposers\(\)" 和 "PhysicsComposer.DestroyAll\(\)" 方法获取或销毁所有合成器。
    ([uum-134952](https://issuetracker.unity3d.com/issues/fix-for-6000-dot-6-x-fix-some-api-issues-from-user-feedback))

- `物理 2D"`: 新增： PhysicsComposer 现在可以使用 "PhysicsComposer.ToPolygons\(\)" 静态方法将 "CircleGeometry "和 "CapsuleGeometry "转换为 "PolygonGeometry"。
    ([uum-134952](https://issuetracker.unity3d.com/issues/fix-for-6000-dot-6-x-fix-some-api-issues-from-user-feedback))

- `物理 2D"`: 新增： PhysicsComposer 现在可以使用 "PhysicsComposer.ToPolygons\(\)" 静态方法将 "CircleGeometry "和 "CapsuleGeometry "转换为 "PolygonGeometry"。
    ([uum-134952](https://issuetracker.unity3d.com/issues/fix-for-6000-dot-6-x-fix-some-api-issues-from-user-feedback))

- `物理 2D"`: 新增：PhysicsWorld、PhysicsBody、PhysicsShape 和 PhysicsJoint 可以使用 "SetOwnerUserData\(\) "设置只属于所有者的物理用户数据，并使用".ownerUserData "检索它。
    ([uum-134952](https://issuetracker.unity3d.com/issues/fix-for-6000-dot-6-x-fix-some-api-issues-from-user-feedback))

- `物理 2D"`: 新增： PhysicsWorld、PhysicsBody、PhysicsShape 和 PhysicsJoint 可以使用 "SetOwnerUserData(\) "设置只属于所有者的物理用户数据，并使用".ownerUserData "获取。
    ([uum-134952](https://issuetracker.unity3d.com/issues/fix-for-6000-dot-6-x-fix-some-api-issues-from-user-feedback))

- `SRP Core`: 已添加： 为结构 TextureHandle 添加了新的运算符 == 和 （！=）。



## 更改

- `Shadergraph`: 禁用代码生成过程中的剖析；在某些情况下，剖析会导致错误。
    ([uum-117133](https://issuetracker.unity3d.com/issues/switching-platform-while-profiling-in-edit-mode-throws-non-matching-profiler-dot-endsample-warnings))

- `uGUI`: 更新了 UI Canvas 模块的剖析器图标。
    (UUM-135623)



## 修复

- `2D`: 修正了 Light Batching Debugger 中名称溢出的问题。
    ([uum-132565](https://issuetracker.unity3d.com/issues/long-light-gameobject-names-are-overflowing-the-light-batching-debugger-text-fields))

- `2D`: 修正了 Light Batching Debugger 中名字无法刷新的问题。
    ([uum-132573](https://issuetracker.unity3d.com/issues/light-batching-debugger-doesnt-update-light-gameobjects-name-unless-the-window-is-restarted))

- `自适应性能`: 修正了自适应性能剖析器数据不显示的问题。
    (UUM-134873)

- `安卓批处理模式`: 如果安装了安卓支持，则移除编辑器启动时对安卓设备的自动扫描。
    ([UUM-133593](https://issuetracker.unity3d.com/issues/batchmode-the-editor-executes-code-that-is-not-relevant-to-the-target-build-platform-when-a-buildtarget-is-defined-in-batchmode))

- `Android`: 修正了一个问题，即在 Android \(Act\)上，当 TouchScreenKeyboard 更改文本选择时，UI Toolkit 输入字段中的圆点位置不会更新，该行为目前在 GameActivity 上仍被破坏。
    ([uum-128088](https://issuetracker.unity3d.com/issues/android-soft-keyboards-arrows-and-select-tools-do-not-have-visual-feedback-when-hide-mobile-input-is-enabled))

- `Android`: 修正了使用 Android `GameActivity`时，`OnApplicationQuit`不能被持续调用的问题。
    (UUM-131090)

- `安卓`: 修正了使用旧输入系统时，在不移动鼠标的情况下向负方向滚动时，安卓鼠标滚轮不起作用的问题。
    ([UUM-134074](https://issuetracker.unity3d.com/issues/android-the-y-value-of-input-dot-mousescrolldelta-is-positive-when-scrolling-in-both-directions-in-the-player))

- `安卓`: 更新了设备模拟器的设备定义，以使用通用的、基于特征的名称，而不是旧设备的具体型号名称。
    (UUM-134051)

- 音频修复了退出单机版播放器时与脚本生成器相关的崩溃问题。
    ([UUM-133608](https://issuetracker.unity3d.com/issues/scriptable-generator-crashes-player-on-exit))

- `构建管道"`: 修正了试图构建存储在软件包中的场景时会导致构建失败的问题。
    ([uum-133786](https://issuetracker.unity3d.com/issues/player-build-fails-with-failed-to-open-error-when-scene-is-located-in-a-package))

- `构建管道`: 修复了构建报告中的构建时间计算错误。
    ([uum-126318](https://issuetracker.unity3d.com/issues/project-auditor-build-time-calculation-can-get-broken))

- `DX12`: 在用户日志中添加了验证错误未涵盖的 Direct3D Graphics Infrastructure (DXGI) 错误。修正了在檢查設備狀態（CheckDeviceStatus）中誤報非錯誤返回代碼（即 087a0001）的問題。
    (UUM-135201)

- `DX12`: 修正了切换窗口焦点后播放器挂起的问题。
    ([UUM-130495](https://issuetracker.unity3d.com/issues/player-hangs-when-the-run-in-background-is-enabled-and-active-window-is-switched))

- `DX12`: 修正了使用 DXC 着色器编译器时的群集光照问题。
    (UUM-134785)

- `DX12`: 修正了纹理加载变慢的问题。
    (UUM-133332)

- `DX12`: 在最终升维过程中，使代理缓冲 srv 格式与交换链 rtv 格式相匹配。
    ([UUM-134064](https://issuetracker.unity3d.com/issues/dx12-player-brightness-changes-when-changing-display-resolution-with-screen-dot-setresolution))

- 编辑器为 UITK 添加 hideSoftkeyboard 选项，以及同时激活物理键盘和触摸屏键盘的选项。
    (UUM-122340)

- 编辑器在高级文本生成器中添加了自定义合成粗体和斜体角度的支持。
    (UUM-114774)

- 编辑器修改了网格 LOD 生成器，当选择曲线为负数时不再输出 LOD，这发生在某些双面几何的网格上。
    ([UUM-121461](https://issuetracker.unity3d.com/issues/meshlod-selection-is-inverted-when-importing-a-model-with-unknown-settings))

- 编辑器修正了一个 Bug，在播放模式下尝试打开 "渲染管道转换器 "窗口会导致打开一个不相关的窗口。
    ([uum-132083](https://issuetracker.unity3d.com/issues/the-sprite-importer-window-is-opened-instead-of-the-render-pipeline-converter-window-when-opening-it-in-play-mode))

- 编辑器修复了 D3D12 设备过滤器列表资产帮助文档链接的缺失。
    ([uum-123217](https://issuetracker.unity3d.com/issues/d3d12-device-filter-lists-asset-link-to-the-documentation-isnt-working))

- 编辑器修正了导致'IsRunningXRMobile'在当前上下文中不存在的问题。
    ([uum-135971](https://issuetracker.unity3d.com/issues/urp-broken-android-project-after-lazy-initialization-for-platformautodetect))

- `编辑器"`: 修正了 Mac 编辑器对话框无法响应某些键盘操作的问题。
    ([uum-134031](https://issuetracker.unity3d.com/issues/characters-cannot-be-deleted-when-pressing-delete-button-in-project-build-save-as-pop-up))

- 编辑器修正了一个问题，即脚本编译在 Windows 和 Linux 上产生不同的结果，导致跨平台工作的团队不必要地更改资产文件。
    (UUM-133554)

- 编辑器修复了使用 ATG 时的 AutoSize 警告记录。
    ([UUM-134814](https://issuetracker.unity3d.com/issues/textautosize-is-not-supported-with-the-standard-textgenerator-warning-is-shown-when-enabling-auto-size-in-ui-builder-while-enable-editor-extension-authoring-by-default-is-enabled))

- 编辑器修正了如果在预处理工件的过程中取消合并过多工件可能导致 LMDB 崩溃的 bug。
    ([uum-133590](https://issuetracker.unity3d.com/issues/crash-on-readwritelock-writelock-when-performing-various-unity-operations))

- 编辑器修正了在物理键盘上切换语言无法正常工作的问题。
    ([uum-130105](https://issuetracker.unity3d.com/issues/android-legacy-tmp-and-ui-toolkit-input-field-language-toggle-to-some-non-latin-alphabet-languages-does-not-work-with-external-keyboard))

- `编辑器"`: 修正了缩放器 UI 更改无法正确更新本地资产的问题。
    (UUM-135019)

- `编辑器`: 修正了在 ATG 中无法正确显示精灵资产的问题。
    ([UUM-134941](https://issuetracker.unity3d.com/issues/icons-are-not-displayed-when-font-is-applied-via-style-sheets))

- 编辑器修正了 IMGUI 调试器的样式选取器 UI 在拖动鼠标时突出显示视图的问题。
    ([uum-133941](https://issuetracker.unity3d.com/issues/pick-style-only-responds-to-elements-on-the-first-hovered-window-when-using-the-imgui-debugger))

- `编辑器"`: 修正了 "重绘点 "的大小，使其现在能根据缩放因子正确缩放。
    (UUM-135511)

- `编辑器修复 Hub 文档链接。

- GI`: 修复了使用 Vulkan 进行烘焙时 APV Sky Occlusion 略微过亮的问题。
    (UUM-101700)

- 图形相机预览 - 更改管道时，渲染目标纹理未重新创建，导致渲染纹理选项无效。
    ([UUM-133293](https://issuetracker.unity3d.com/issues/after-converting-a-built-in-project-to-urp-render-texture-setting-error-message-is-spammed))

- `图形"`: 修正了一个问题，当使用金属时，模板附件被错误地取消设置，这会导致金属验证错误。
    (UUM-133783)

- `图形`: 修正了 Vulkan 后端缓冲池中的数据竞赛。
    (UUM-134547)

- `图形`: 修正了在 WebGPU 中清除多个渲染目标的问题。
    ([UUM-133743](https://issuetracker.unity3d.com/issues/webgpu-urp-rendergraph-renderpass-doesnt-clear-textures))

- `图形`: 修正了：着色器编译错误 "调用 'tex3D' 有歧义"。
    ([uum-133088](https://issuetracker.unity3d.com/issues/error-shader-error-in-yscloudcover-call-to-tex3d-is-ambiguous-at-assets-slash-yscloudcovertext-dot-shader-606-on-d3d11-is-present-when-compiling-tex3d-shader-with-dxc))

- 圖形\URP（URP）] 修正了在启用贴花的情况下以批处理模式为移动平台构建时导致材质变黑的问题。
    ([uum-134298](https://issuetracker.unity3d.com/issues/urp-all-materials-render-black-when-building-via-batchmode-or-without-rendering-scene-slash-game-view-in-editor-if-decal-renderer-technique-is-set-to-automatic))

- `HDRP`: 装饰投影仪和局部体积雾缺少图标小工具。水贴组件在 "光 "主题中缺少暗色图标。
    ([uum-132819](https://issuetracker.unity3d.com/issues/hdrp-decal-projector-and-local-volumetric-fog-are-missing-their-icon-gizmos-hdrp-decal-projector-and-local-volumetric-fog-are-missing-their-icon-gizmos))

- `IL2CPP`: 修正了 lambda 表达式中无效的 MethodsToPreserve 条目。
    ([uum-124814](https://issuetracker.unity3d.com/issues/unity-cil-linker-fails-on-player-build-when-persistent-listeners-have-and-in-their-xml-attribute-names))

- 输入修正了一个问题，即对于禁用闪屏且仅使用输入管理器的项目，在调整单机版播放器窗口大小时，调整大小光标不会显示。
    ([uum-134058](https://issuetracker.unity3d.com/issues/double-sided-arrow-mouse-cursor-does-not-appear-when-resizing-the-player-and-input-backend-is-set-to-input-manager-old))

- 输入系统修正了同步原语的错误使用，该原语可能导致 Unity 在主线程以外的线程发现输入设备的平台上崩溃或出现未定义的行为。
    (UUM-134537)

- 安装程序MacOS 平台支持安装程序不再从其他不同版本的 Unity 编辑器安装中移除对同一平台的支持。
    (UUM-133396)

- 许可证禁止写入符号链接的 ULF。
    (UUM-121827)

- `macOS`: 修正了 Mac 播放器在使用新的 `CAMetalDisplayLink` 时出现的卡顿问题，可以在播放器设置中切换 "Use MetalDisplayLink \(Mac Player only\)" 来启用该功能。
    ([uum-112011](https://issuetracker.unity3d.com/issues/built-project-stutters-intermittently-when-vsync-is-enabled))

- `软件包管理器"`: 更改了每个字段下所有错误的位置，而不是 "应用 "按钮下的位置。
    ([uum-112552](https://issuetracker.unity3d.com/issues/validation-messages-in-inspector-window-are-displayed-too-low-during-package-editing-process))

- `软件包管理器"`: 修正了防止依赖版本出现空值的验证。
    ([uum-113308](https://issuetracker.unity3d.com/issues/editing-package-manifest-allows-adding-a-dependency-with-a-null-version))

- `软件包管理器`: 修正了验证，以防止技术名称与项目中已有的名称相匹配。
    ([uum-113396](https://issuetracker.unity3d.com/issues/while-editing-package-manifest-via-inspector-the-package-name-can-be-set-to-an-already-existing-packages-name))

- 软件包管理器导入 .unitypackage 会提取两倍的内容。
    (PAK-8613)

- `软件包管理器软件包管理器`: 修复检查器窗口中修改 Package.json 的 UI 问题。
    (UUM-133647)

- `软件包管理器软件包管理器`: 使用 upm 软件包的 Url 深度链接会在可发现的情况下显示所选软件包。如果指定了版本或软件包无法被发现，也会显示添加弹出窗口。
    (PAK-8687)

- 物理修复了预制板上的刚体组件仍会创建其内部物理对象的问题。这并不是有意为之，而是由于最近的安全变更而出现的，顺便说一下，这些变更也是导致此次崩溃重现的原因。
    ([uum-135381](https://issuetracker.unity3d.com/issues/crash-on-physicscommands-physx-bodysetpose-when-editing-rigidbody-component-settings-on-a-prefab))

- `物理 2D"`: 修正了 "PolygonGeometry.ClosestPoint\(\) "在重叠时不返回周长点的问题。
    ([uum-134804](https://issuetracker.unity3d.com/issues/polygongeometry-dot-closestpoint-not-returning-perimeter-point-when-overlapped))

- `物理 2D"`: 修正了物理调试渲染器错误使用深度测试的问题。
    (UUM-135992)

- `物理 2D"`: 修正了 "PhysicsComposer.GetGeometryIslands/(\) "没有读取锁定导致潜在并发问题的问题。
    (UUM-135939)

- `物理 2D"`: 修复了删除正在编辑的组件时 HingeJoint2D 工具句柄绘制的问题。
    ([UUM-134276](https://issuetracker.unity3d.com/issues/missingreferenceexception-and-gui-error-errors-thrown-when-deleting-a-sprite-with-box-collider-2d-and-hinge-joint-2d-components))

- `物理 2D"`: 修正了默认 "PolygonGeometry "构造函数生成无效边缘法线的问题。
    ([uum-134804](https://issuetracker.unity3d.com/issues/polygongeometry-dot-closestpoint-not-returning-perimeter-point-when-overlapped))

- 播放器修正了当视频播放器打开路径包含空格的文件时出现的 URL 解析问题。
    ([uum-125789](https://issuetracker.unity3d.com/issues/video-does-not-play-in-macos-build-when-built-app-is-placed-in-a-path-with-a-space-in-it-on-a-specific-project))

- `剖析器`: 修正了一个问题，即不完整的帧会影响高光视图汇总数据。
    (UUM-125642)

- `剖析器`: 修正了在录制剖析数据后减少最大捕获帧数设置时，在保存时创建剖析器捕获元数据的问题。
    ([UUM-134348](https://issuetracker.unity3d.com/issues/failed-to-read-highlights-data-from-file-dot-dot-dot-unable-to-read-beyond-the-end-of-the-stream-dot-error-is-thrown-after-saving-profiler-capture))

- 剖析器当 kDontCaptureEditor 或 kRecordTimestamp 不同时，防止不正确的共享 ProfilerRecorder 重用。
    (UUM-133664)

- 场景/游戏视图修正了一个问题，即聚焦于活动选区可能会编辑场景视图中的覆盖内容。
    ([UUM-134399](https://issuetracker.unity3d.com/issues/overlays-are-focused-when-using-the-frame-selected-in-window-under-cursor-shortcut-just-after-editing-overlay-fields))

- `脚本`: 修正了玩家构建中的 UnityEvent 内存泄漏问题。
    ([uum-131348](https://issuetracker.unity3d.com/issues/unityeventbase-dot-s-unityevents-memory-leak-occurs-when-loading-and-unloading-scenes-with-ugui-components))

- 着色器当不使用遮罩时，修正了画布着色器 uv1 通道的初始化。
    (UUM-133826)

- `着色器`: 修正了 ShaderGraph 自定义光照样本中的材质重写调试不起作用。
    ([UUM-134440](https://issuetracker.unity3d.com/issues/some-material-overrides-are-viewed-as-broken-when-using-the-shadergraph-customlighting-package-sample))

- `着色器`: 修正了标记为 HDR 的纹理属性的纹理采样操作。
    ([uum-122106](https://issuetracker.unity3d.com/issues/hdr-images-are-compressed-incorrectly-with-default-settings-on-android-platform))

- `阴影图`: 修正了 UGUI 着色器样本中的花式加载子图。
    (UUM-134638)

- 阴影图重命名关键字枚举字段和对关键字枚举的其他修改现在可以正确传播。
    ([UUM-134292](https://issuetracker.unity3d.com/issues/shadergraph-enum-node-labels-are-not-updated-when-a-new-entry-name-is-set))

- `Shadergraph`: Swizzle 节点现在能在撤销/重做后正确更新。
    ([uum-134112](https://issuetracker.unity3d.com/issues/shader-graph-swizzle-node-data-updates-incorrectly-after-undo-action))

- `着色器`: 修复了在计算中写入 RWTexture2D 的问题。
    (UUM-127198)

- 文字为 PanelTextSettings 和 FontAsset 添加了图标。
    (UUM-134700)

- 文字通过确保域重载后 OSFallbacks 被正确保存，修正了内存泄漏。
    ([UUM-132677](https://issuetracker.unity3d.com/issues/editor-memory-leak-when-entering-and-exiting-play-mode-in-a-blank-urp-project))

- `文本`: 修正了 RichTextTagParser 标签解析不完整的问题。
    (UUM-134299)

- `TextMeshPro`: 改进了对缺少 "href "部分的不正确格式化 &lt;a&gt; 标签的处理。格式正确的标记应为 &lt;a href="link ID"&gt;要高亮显示的文本&lt;/a&gt;。
    ([uum-130554](https://issuetracker.unity3d.com/issues/indexoutofrangeexception-occurs-when-entering-tags-in-a-textmeshpro-ui-field))

- `uGUI`: 键盘关闭后停用 InputFields。
    ([uum-133712](https://issuetracker.unity3d.com/issues/input-field-does-not-update-when-selecting-the-same-input-field-after-previous-input-was-canceled))

- `uGUI`: 修正了因矩形变换边界过大而导致的崩溃。
    ([uum-132182](https://issuetracker.unity3d.com/issues/crash-on-raiseexception-when-creating-a-multiplayer-room-while-toggling-ui))

- `uGUI`: 修正了因矩形变换边界过大而导致崩溃的根本原因。添加了链接到受影响场景 GameObject\(s\) 的警告。
    (UUM-134019)

- 用户界面工具包为 `Painter2D` 添加了缺失的 getter API。
    ([UUM-128715](https://issuetracker.unity3d.com/issues/certain-painter2d-properties-are-missing-the-get-accessors))

- `用户界面工具包`: 修正了用户界面生成器中的一个错字。
    ([uum-131438](https://issuetracker.unity3d.com/issues/misspelled-label-custorm-when-editing-aspect-ratio-in-ui-builder-inlined-styles))

- 用户界面工具包修正了在绘制带有某些尖角或接近退化线段的二维矢量图形的描边路径时可能出现的异常。
    (UUM-135440)

- 用户界面工具包修正了无法多次使用 SampleTextureElement 节点的代码生成错误。
    ([UUM-115301](https://issuetracker.unity3d.com/issues/cant-add-and-use-sample-element-texture-node-twice-in-a-graph))

- `用户界面工具包`: 修正了在移动设备上拖动集合视图控件滚动不起作用的问题。
    ([uum-135398](https://issuetracker.unity3d.com/issues/android-ios-ui-toolkit-listview-touch-pan-scrolling-does-not-work))

- `用户界面工具包`: 修正了 UIE_NOINTERPOLATION 重新定义导致警告的问题。
    ([uum-134991](https://issuetracker.unity3d.com/issues/uie-nointerpolation-macro-redefinition-warnings-are-thrown-on-vfx-graph-when-changing-the-shader-precision-model-on-web-platform))

- `用户界面工具包`: 修正了当在较早帧中修改溢出时，作为背景图片的 VectorImage 无法正确用作模版遮罩的问题。
    ([uum-110567](https://issuetracker.unity3d.com/issues/text-is-not-masked-when-creating-a-vector-image-and-using-a-mask-inside-a-visualelement))

- `用户界面工具包`: 修正了当使用动态颜色提示时，矢量图像以统一颜色显示的问题。
    ([uum-126859](https://issuetracker.unity3d.com/issues/svg-pictures-turn-white-on-hover-when-transition-animation-is-added-in-ui-builder))

- `用户界面工具包`: 修正将 SVG 导入精灵时使用错误材质的问题。
    ([uum-134795](https://issuetracker.unity3d.com/issues/svg-asset-sprite-materials-are-lost-when-upgrading-the-project-to-a-different-unity-editor-version))

- 用户界面工具包PanelSettings.renderMode 现在是公共 API。
    (UUM-119486)

- `URP`: Decal Projector 灯光主题现在显示为黑色。
    ([UUM-132819](https://issuetracker.unity3d.com/issues/hdrp-decal-projector-and-local-volumetric-fog-are-missing-their-icon-gizmos-hdrp-decal-projector-and-local-volumetric-fog-are-missing-their-icon-gizmos))

- `URP`: 修正播放器中反射探针旋转被禁用的问题。
    (UUM-134244)

- 版本控制修正了 Unity 6.4 及更高版本中过时的 instanceID API 使用。

- 视频修正了在使用 Vulkan 图形 API 的特定移动设备上无法播放视频的问题。
    ([uum-133914](https://issuetracker.unity3d.com/issues/video-player-renders-no-video-on-specific-devices-when-using-vulkan))

- `视频`: 使测试稳定。
    (UUM-71794)

- 网络修正了处理触摸取消事件时出现的错误。
    ([UUM-132183](https://issuetracker.unity3d.com/issues/mouse-postion-can-become-max-value-or-infinity-when-using-touch-input-with-legacy-input-module))

- `XR`: 修正了音频配置更改时编辑器偶尔崩溃的问题。
    ([uum-126803](https://issuetracker.unity3d.com/issues/crash-on-audiomanager-initfmod-when-performing-various-actions-in-the-editor))




## 6000.3.11f1 中的软件包变更

## 更新的软件包

- `com.unity.addressables`: [2.9.0](https://docs.unity3d.com/Packages/com.unity.addressables@2.9//changelog/CHANGELOG.html) 到 [2.9.1](https://docs.unity3d.com/Packages/com.unity.addressables@2.9//changelog/CHANGELOG.html)

- `com.unity.cinemachine`: [2.10.5](https://docs.unity3d.com/Packages/com.unity.cinemachine@2.10//changelog/CHANGELOG.html) 到 [2.10.6](https://docs.unity3d.com/Packages/com.unity.cinemachine@2.10//changelog/CHANGELOG.html)

- `com.unity.collab-proxy`: [2.11.3](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.11//changelog/CHANGELOG.html) 到 [2.11.4](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.11//changelog/CHANGELOG.html)

- `com.unity.inputsystem`: [1.18.0](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.18//changelog/CHANGELOG.html) 到 [1.19.0](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.19//changelog/CHANGELOG.html)

- `com.unity.performance.profile-analyzer`: [1.3.1](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.3//changelog/CHANGELOG.html) 到 [1.3.2](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.3//changelog/CHANGELOG.html)

- `com.unity.remote-config`: [4.2.4](https://docs.unity3d.com/Packages/com.unity.remote-config@4.2//changelog/CHANGELOG.html) 到 [4.2.5](https://docs.unity3d.com/Packages/com.unity.remote-config@4.2//changelog/CHANGELOG.html)

- `com.unity.scriptablebuildpipeline`: [2.6.0](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@2.6//changelog/CHANGELOG.html) 到 [2.6.1](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@2.6//changelog/CHANGELOG.html)

- `com.unity.services.analytics`: [6.2.0](https://docs.unity3d.com/Packages/com.unity.services.analytics@6.2//changelog/CHANGELOG.html) 到 [6.2.2](https://docs.unity3d.com/Packages/com.unity.services.analytics@6.2//changelog/CHANGELOG.html)

- `com.unity.services.wire`: [1.4.1](https://docs.unity3d.com/Packages/com.unity.services.wire@1.4//changelog/CHANGELOG.html) 到 [1.4.2](https://docs.unity3d.com/Packages/com.unity.services.wire@1.4//changelog/CHANGELOG.html)

- `com.unity.timeline`: [1.8.10](https://docs.unity3d.com/Packages/com.unity.timeline@1.8//changelog/CHANGELOG.html) 至 [1.8.11](https://docs.unity3d.com/Packages/com.unity.timeline@1.8//changelog/CHANGELOG.html)

- `com.unity.visualcripting`: [1.9.9](https://docs.unity3d.com/Packages/com.unity.visualscripting@1.9//changelog/CHANGELOG.html) 到 [1.9.10](https://docs.unity3d.com/Packages/com.unity.visualscripting@1.9//changelog/CHANGELOG.html)

- `com.unity.learn.inet-framework`: [5.0.2](https://docs.unity3d.com/Packages/com.unity.learn.iet-framework@5.0//changelog/CHANGELOG.html) 到 [5.0.3](https://docs.unity3d.com/Packages/com.unity.learn.iet-framework@5.0//changelog/CHANGELOG.html)

- `com.unity.learn.iet-framework.authoring`: [1.5.2](https://docs.unity3d.com/Packages/com.unity.learn.iet-framework.authoring@1.5//changelog/CHANGELOG.html) 到 [1.5.3](https://docs.unity3d.com/Packages/com.unity.learn.iet-framework.authoring@1.5//changelog/CHANGELOG.html)

- `com.unity.terrain-tools`: [5.3.1](https://docs.unity3d.com/Packages/com.unity.terrain-tools@5.3//changelog/CHANGELOG.html) 到 [5.3.2](https://docs.unity3d.com/Packages/com.unity.terrain-tools@5.3//changelog/CHANGELOG.html)

- `com.unity.ai.navigation`: [2.0.10](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html) 到 [2.0.11](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html)

- `com.unity.services.deployment`: [1.6.2](https://docs.unity3d.com/Packages/com.unity.services.deployment@1.6//changelog/CHANGELOG.html) 到 [1.7.1](https://docs.unity3d.com/Packages/com.unity.services.deployment@1.7//changelog/CHANGELOG.html)

- `com.unity.services.tooling`: [1.4.0](https://docs.unity3d.com/Packages/com.unity.services.tooling@1.4//changelog/CHANGELOG.html) 到 [1.4.1](https://docs.unity3d.com/Packages/com.unity.services.tooling@1.4//changelog/CHANGELOG.html)

- `com.unity.addressables.android`: [1.0.9](https://docs.unity3d.com/Packages/com.unity.addressables.android@1.0//changelog/CHANGELOG.html) 到 [1.0.10](https://docs.unity3d.com/Packages/com.unity.addressables.android@1.0//changelog/CHANGELOG.html)

- `com.unity.polyspatial`: [3.0.5](https://docs.unity3d.com/Packages/com.unity.polyspatial@3.0//changelog/CHANGELOG.html) 到 [3.1.0](https://docs.unity3d.com/Packages/com.unity.polyspatial@3.1//changelog/CHANGELOG.html)

- `com.unity.polyspatial.visionos`: [3.0.5](https://docs.unity3d.com/Packages/com.unity.polyspatial.visionos@3.0//changelog/CHANGELOG.html) 到 [3.1.0](https://docs.unity3d.com/Packages/com.unity.polyspatial.visionos@3.1//changelog/CHANGELOG.html)

- `com.unity.polyspatial.xr`: [3.0.5](https://docs.unity3d.com/Packages/com.unity.polyspatial.xr@3.0//changelog/CHANGELOG.html) 至 [3.1.0](https://docs.unity3d.com/Packages/com.unity.polyspatial.xr@3.1//changelog/CHANGELOG.html)

- `com.unity.polyspatial.extensions`: [3.0.5](https://docs.unity3d.com/Packages/com.unity.polyspatial.extensions@3.0//changelog/CHANGELOG.html) 到 [3.1.0](https://docs.unity3d.com/Packages/com.unity.polyspatial.extensions@3.1//changelog/CHANGELOG.html)

- `com.unity.xr.visionos`: [3.0.5](https://docs.unity3d.com/Packages/com.unity.xr.visionos@3.0//changelog/CHANGELOG.html) 到 [3.1.0](https://docs.unity3d.com/Packages/com.unity.xr.visionos@3.1//changelog/CHANGELOG.html)

- `com.unity.services.multiplayer`: [2.1.2](https://docs.unity3d.com/Packages/com.unity.services.multiplayer@2.1//changelog/CHANGELOG.html) 到 [2.1.3](https://docs.unity3d.com/Packages/com.unity.services.multiplayer@2.1//changelog/CHANGELOG.html)

- `com.unity.asset-manager-for-unity`: [1.9.1](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.9//changelog/CHANGELOG.html) 到 [1.9.2](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.9//changelog/CHANGELOG.html)

- `com.unity.web.stripping-tool`: [1.2.0](https://docs.unity3d.com/Packages/com.unity.web.stripping-tool@1.2//changelog/CHANGELOG.html) 到 [1.2.1](https://docs.unity3d.com/Packages/com.unity.web.stripping-tool@1.2//changelog/CHANGELOG.html)