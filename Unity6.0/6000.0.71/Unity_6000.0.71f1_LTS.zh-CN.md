# Unity 6000.0.71f1 LTS
发布于 星期三, 18 三月 2026 07:40:01 GMT
https://unity.com/releases/editor/whats-new/6000.0.71f1

# 6000.0.71f1 中的已知问题

- `IL2CPP`: [iOS] [Android] 在构建 IL2CPP 时外部库泛型失败
    ([uum-125284](https://issuetracker.unity3d.com/issues/ios-android-external-library-generics-fail-during-il2cpp-build))

- 金属命令缓冲区超时错误后游戏冻结
    ([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- `金属"`: MacOS 在编辑器中的最小项目在播放模式下出现卡顿
    ([uum-85256](https://issuetracker.unity3d.com/issues/macos-stutters-in-a-minimal-project))

使用 DirectX 12 在独占全屏模式下切换焦点时播放器崩溃
    ([uum-134743](https://issuetracker.unity3d.com/issues/player-crash-when-switching-focus-in-exclusive-fullscreen-mode-with-directx-12))



# 6000.0.71f1 发布说明

## 修复

- `2D`: 修复了创建平铺调色板时单元格大小属性接受负值的问题。编辑器现在会将负值设置为 0。
    ([uum-130884](https://issuetracker.unity3d.com/issues/tile-palette-allows-negative-manual-cell-size-values-causing-asset-corruption-and-assertion-failed-on-expression-errors))

- `2D`: 修复了 Light Batching Debugger 中名称溢出的问题。
    ([uum-132565](https://issuetracker.unity3d.com/issues/long-light-gameobject-names-are-overflowing-the-light-batching-debugger-text-fields))

- `2D`: 修正了 Light Batching Debugger 中名字无法刷新的问题。
    ([uum-132573](https://issuetracker.unity3d.com/issues/light-batching-debugger-doesnt-update-light-gameobjects-name-unless-the-window-is-restarted))

- `2D`: 将 Tilemap 在 UI 中使用的文字从 SceneView 更新为 Scene View。
    ([uum-130251](https://issuetracker.unity3d.com/issues/tile-palette-sceneroot-and-sceneview-are-not-rendered-with-correct-ui-spacing))

- `DX12`: 在用户日志中添加了验证错误未涵盖的 Direct3D Graphics Infrastructure (DXGI) 错误。修正了在檢查設備狀態（CheckDeviceStatus）中誤報非錯誤返回代碼（即 087a0001）的問題。
    (UUM-135201)

- `DX12`: 修正了切换窗口焦点后播放器挂起的问题。
    ([UUM-130495](https://issuetracker.unity3d.com/issues/player-hangs-when-the-run-in-background-is-enabled-and-active-window-is-switched))

- 编辑器修改了动画窗口文本，使其始终使用 Signed Distance Field （SDF）渲染，以提高可读性。
    ([uum-134486](https://issuetracker.unity3d.com/issues/animator-state-labels-are-not-rendered-correctly-when-using-the-bitmap-renderer-as-the-default-editor-text-renderer))

- 编辑器编辑器现在可以正确清除预制件实例中与 `SerializeReference` 相关的未使用的重载。
    ([uum-135932](https://issuetracker.unity3d.com/issues/prefabs-remove-unused-overrides-fails-to-clean-up-overrides-when-the-managed-instance-type-in-serializereference-is-changed))

- 编辑器修正了在特定情况下出现的 4 帧内存分配器警告。
    ([uum-86868](https://issuetracker.unity3d.com/issues/a-memory-leak-occurs-when-selecting-the-console-window-and-the-inspector-window-covers-the-game-view-window-when-specific-ui-elements-are-displayed-in-it))

- 编辑器修正了导致当前上下文中不存在'IsRunningXRMobile'的问题。
    ([uum-135971](https://issuetracker.unity3d.com/issues/urp-broken-android-project-after-lazy-initialization-for-platformautodetect))

- `编辑器"`: 修正了 USS 样式验证中无法识别制表符是空白的问题。
    ([uum-135915](https://issuetracker.unity3d.com/issues/warning-expected-end-of-value-but-found-is-shown-when-inserting-a-blank-line-between-opacity-and-scale-in-a-uss-file))

- 编辑器修正了一个问题，即切换*覆盖Windows、Mac、Linux*后，播放器设置图标大小和保留不被保留。
    ([uum-131965](https://issuetracker.unity3d.com/issues/icon-override-texture2d-fields-in-the-player-settings-window-are-not-square-and-do-not-retain-data-after-disabling))

- 编辑器修正了在 "项目设置 "窗口中移除搜索过滤器会完全高亮显示部分文本的问题。
    ([uum-134769](https://issuetracker.unity3d.com/issues/all-text-in-the-project-settings-window-is-still-tinted-white-after-deleting-text-in-the-search-window))

- 编辑器修正了 Linux 编辑器的一个问题，即不会提示你覆盖同名文件。
    ([uum-134937](https://issuetracker.unity3d.com/issues/linux-no-file-already-exists-pop-up-thrown-when-saving-shader-variants-with-an-already-existing-name-from-build-profiles-or-project-settings-window))

- 编辑器修正了 TextCore 中的中日韩换行问题。
    ([uum-135887](https://issuetracker.unity3d.com/issues/cjk-text-goes-outside-of-the-bounds-of-a-label-in-ui-builder-when-wrapping-is-enabled))

- `编辑器修正了模块详情面板控制器脚本示例。

- 编辑器修复 Hub 文档链接。

- 引擎诊断`: 修复了诊断原生崩溃报告中错误的时间戳。
    (UUM-135436)

- `GI`: 修正了 APV 工具提示中的一个小错字：Steaming &gt; Streaming.
    ([UUM-134159](https://issuetracker.unity3d.com/issues/streaming-is-misspelled-as-steaming-in-enable-gpu-streaming-and-enable-disk-streaming-tooltpis))

- `图形`: 修正了 Vulkan 后端缓冲池中的数据竞赛。
    (UUM-134547)

- `图形`: 确保内建RP blit copy 输出 float4 颜色（而不是 fxed4，后者在金属上会转换为 half4，导致 u16 或 f32 数据截断）。
    ([uum-128591](https://issuetracker.unity3d.com/issues/terrain-heightmap-loses-precision-on-android-and-ios-when-the-heightmap-texture-is-blitted-to-a-rendertexture-using-the-default-blit-shader))

- 图形\URP\]修复了在启用贴花的情况下以批处理模式为移动平台构建时导致材质变黑的问题。
    ([uum-134298](https://issuetracker.unity3d.com/issues/urp-all-materials-render-black-when-building-via-batchmode-or-without-rendering-scene-slash-game-view-in-editor-if-decal-renderer-technique-is-set-to-automatic))

- 输入修正了一个问题，对于禁用闪屏且仅使用输入管理器的项目，在调整单机版播放器窗口大小时，调整大小光标不会显示。
    ([uum-134058](https://issuetracker.unity3d.com/issues/double-sided-arrow-mouse-cursor-does-not-appear-when-resizing-the-player-and-input-backend-is-set-to-input-manager-old))

- 输入修正了 IOHIDDevice_GetUsage 中无效的长缓冲指针。
    ([uum-135043](https://issuetracker.unity3d.com/issues/silicon-crash-on-os-unfair-recursive-lock-lock-with-options-when-opening-a-project-while-the-razer-synapse-app-is-open))

- 安装程序MacOS 平台支持安装程序不再从其他不同版本的 Unity Editor 安装程序中移除对同一平台的支持。
    (UUM-133396)

- `iOS`: 修复了在应用程序已运行时通过自定义 URL 方案或通用链接打开应用程序，或在某些情况下通过深度链接从冷启动启动应用程序时未调用 Application.deepLinkActivated 的问题。
    ([uum-135497](https://issuetracker.unity3d.com/issues/ios-application-dot-deeplinkactivated-does-not-get-invoked-while-app-is-running-when-uiapplicationscenemanifest-is-added-in-info-dot-plist))

- `iOS`: 仅在键盘布局发生变化时报告键盘布局，从而提高了性能。
    ([uum-134845](https://issuetracker.unity3d.com/issues/ios-high-cpu-load-when-device-keyboard-is-open))

- 物理修正了物理关节组件小工具的一个问题，在关节连接到世界空间中的一个固定点的情况下，自动配置的连接锚会跟随关节。
    ([uum-134423](https://issuetracker.unity3d.com/issues/spring-joint-shows-only-one-anchor-gizmo-in-scene-view-when-auto-configure-connected-anchor-is-enabled))

- 物理在使用 "使用快速中相 "烹饪选项的 "网格对撞机 "上进行射线投射时，防止堆栈溢出。
    ([uum-110564](https://issuetracker.unity3d.com/issues/silent-crash-when-raycasting-on-a-specific-dense-mesh))

- `阴影图"`: 修正了标记为 HDR 的纹理属性的纹理采样操作。
    ([uum-122106](https://issuetracker.unity3d.com/issues/hdr-images-are-compressed-incorrectly-with-default-settings-on-android-platform))

- `文本`: 修正使用标准文本的位图时高光不正确的问题。
    ([uum-134691](https://issuetracker.unity3d.com/issues/project-settings-search-highlights-are-misaligned-when-using-the-bitmap-text-rendering-mode))

- `uGUI`: 关闭键盘后，停用 InputFields。
    ([uum-133712](https://issuetracker.unity3d.com/issues/input-field-does-not-update-when-selecting-the-same-input-field-after-previous-input-was-canceled))

- `uGUI`: 修正了在字体重建范围内添加文本组件时的异常。
    ([uum-128580](https://issuetracker.unity3d.com/issues/invalidoperationexception-thrown-when-text-legacy-font-is-rebuilt-via-inputfield-legacy-onvaluechanged-callback))

- 用户界面元素修正了针对 UnityEvent 的 Inspector 复制/粘贴，现在它可以在带有自定义编辑器（如 Button\ ）的组件和不带自定义编辑器的组件之间工作。以前，由于剪贴板格式不兼容，在这两种组件之间粘贴复制的 UnityEvent 会无声地失败。
    ([uum-134401](https://issuetracker.unity3d.com/issues/unityevent-does-not-get-pasted-to-a-ugui-component-when-trying-to-copy-it-from-a-script))

- 用户界面工具包公开 EditorUtility.activePlayModeTint，使自定义网格和 Painter2D 的颜色与编辑器一致。
    (UUM-114424)

- 用户界面工具包修正了一个 Bug，该 Bug 在更改溢出或角半径后可能导致不正确的剪切。
    ([UUM-135869](https://issuetracker.unity3d.com/issues/invalid-clip-method))

- `用户界面工具包`: 修正了一个可能导致在更改后不完全更新剪切状态的情况。
    (UUM-108710)

- `用户界面工具包`: 修正了在绘制带有某些尖角或接近退化线段的二维矢量图形的描边路径时可能发生的异常。
    (UUM-135440)

- 用户界面工具包修复了编辑器监视器中的渲染纹理泄漏。
    (UUM-104256)

- `用户界面工具包`: 修正了当在较早帧中修改溢出时，作为背景图片的 VectorImage 无法正确用作模版遮罩的问题。
    ([UUM-110567](https://issuetracker.unity3d.com/issues/text-is-not-masked-when-creating-a-vector-image-and-using-a-mask-inside-a-visualelement))

- 版本控制修正了 Unity 6.4 及更高版本中过时的 instanceID API 使用。

- 视频修正了在使用 Vulkan 图形 API 的特定移动设备上无法播放视频的问题。
    ([uum-133914](https://issuetracker.unity3d.com/issues/video-player-renders-no-video-on-specific-devices-when-using-vulkan))

- `WebGL`: WebGPU：修正了着色器编译器中的一个错误，该错误导致某些着色器编译失败。
    ([uum-134978](https://issuetracker.unity3d.com/issues/shader-compiler-and-shader-errors-are-thrown-in-the-console-when-building-web-platform-with-webgpu-experimental-enabled-in-auto-graphics-api))

- `XR`: 修正了音频配置更改时编辑器偶尔崩溃的问题。
    ([uum-126803](https://issuetracker.unity3d.com/issues/crash-on-audiomanager-initfmod-when-performing-various-actions-in-the-editor))




## 6000.0.71f1 中软件包的更改

## 更新的软件包

- `com.unity.cinemachine`: [2.10.4](https://docs.unity3d.com/Packages/com.unity.cinemachine@2.10//changelog/CHANGELOG.html) 到 [2.10.6](https://docs.unity3d.com/Packages/com.unity.cinemachine@2.10//changelog/CHANGELOG.html)

- `com.unity.collab-proxy`: [2.11.3](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.11//changelog/CHANGELOG.html) 到 [2.11.4](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.11//changelog/CHANGELOG.html)

- `com.unity.performance.profile-analyzer`: [1.3.1](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.3//changelog/CHANGELOG.html) 到 [1.3.3](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.3//changelog/CHANGELOG.html)

- `com.unity.remote-config`: [4.2.2](https://docs.unity3d.com/Packages/com.unity.remote-config@4.2//changelog/CHANGELOG.html) 到 [4.2.5](https://docs.unity3d.com/Packages/com.unity.remote-config@4.2//changelog/CHANGELOG.html)

- `com.unity.services.analytics`: [6.2.1](https://docs.unity3d.com/Packages/com.unity.services.analytics@6.2//changelog/CHANGELOG.html) 到 [6.3.0](https://docs.unity3d.com/Packages/com.unity.services.analytics@6.3//changelog/CHANGELOG.html)

- `com.unity.visualcripting`: [1.9.7](https://docs.unity3d.com/Packages/com.unity.visualscripting@1.9//changelog/CHANGELOG.html) 到 [1.9.10](https://docs.unity3d.com/Packages/com.unity.visualscripting@1.9//changelog/CHANGELOG.html)

- `com.unity.asset-manager-for-unity`: [1.9.1](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.9//changelog/CHANGELOG.html) 到 [1.10.0](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.10//changelog/CHANGELOG.html)

- `com.unity.cloud.draco`: [5.4.0](https://docs.unity3d.com/Packages/com.unity.cloud.draco@5.4//changelog/CHANGELOG.html) 到 [5.4.3](https://docs.unity3d.com/Packages/com.unity.cloud.draco@5.4//changelog/CHANGELOG.html)

- `com.unity.cloud.ktx`: [3.6.1](https://docs.unity3d.com/Packages/com.unity.cloud.ktx@3.6//changelog/CHANGELOG.html) 到 [3.6.3](https://docs.unity3d.com/Packages/com.unity.cloud.ktx@3.6//changelog/CHANGELOG.html)