# Unity 6000.3.21f1 LTS
发布于 2026年7月29日 星期三 07:10:05 GMT  
https://unity.com/releases/editor/whats-new/6000.3.21f1

# 6000.3.21f1 中的已知问题

- `6000.0.67f1`: [iOS] 访问 iOS 控制中心时音频中断
    ([UUM-145522](https://issuetracker.unity3d.com/issues/ios-audio-is-cut-out-when-accessing-ios-control-center))

- `6000.0.72f1`: 在使用 DirectX12 时，全屏窗口模式下快速切换应用焦点会导致“UnityMain”播放器崩溃
    ([UUM-148214](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-148214))

- `资源导入器`: 进入播放模式时，编辑器在执行“(Unity) WriteObjectToVector”操作时崩溃
    ([UUM-112617](https://issuetracker.unity3d.com/issues/editor-crashes-on-unity-writeobjecttovector-when-entering-into-the-play-mode))

- `Metal`: 命令缓冲区超时错误后游戏卡死
    ([UUM-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

当有多个 bee_backend 实例同时运行时，在调用 mono_log_write_logfile 时发生崩溃
    ([UUM-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))

生成字体图集时发生崩溃，并产生多个堆栈跟踪
    ([UUM-141061](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-generating-font-atlas-with-sdf16-or-sdf32))



# 6000.3.21f1 发布说明

## 改进

- `无障碍功能`: 在 Android 上增加了对 `AccessibilityState.Expanded` 的支持。

- `资源管道`: 在
中添加了说明细节



## 修复

- `2D`: 修复了“安装 2D 包”按钮在不应禁用时被禁用的问题。
    ([UUM-143583](https://issuetracker.unity3d.com/issues/install-2d-sprite-package-button-in-sprite-renderer-is-disabled-when-no-sprite-is-assigned-contradicting-its-own-help-text))

- `无障碍功能`: 修复了在 Android 系统上 `AccessibilityRole.Toggle` 节点出现状态提示重复的问题。
    ([UUM-146950](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146950))

- `无障碍功能`: 修复了 UI Automation 客户端中，主应用程序窗口也会作为辅助窗口提供的问题。

- `无障碍功能`: 修复了屏幕阅读器在 Android 系统上从 `AccessibilityRole.下拉菜单`节点时导航速度过慢的问题。
    ([UUM-146949](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146949))

- `无障碍功能`: 修复了当 UI 自动化客户端 \（例如屏幕阅读器）与应用程序进行交互后，Windows 播放器在关闭时会崩溃。
    (UUM-146676)

- `Android`: ```Screen.brightness``` 的负值现在可恢复设备的首选屏幕亮度。
    ([UUM-145925](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-145925))

- `Android`: 放宽了 AGP 9 中对 R8 保持规则的严格执行要求。
    ([UUM-147136](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147136))

- `动画`: Animator.ResetControllerState(true) 无法重置非浮点型参数。
    ([UUM-146636](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146636))

- `Animation`: 修复了 Animator 过渡复制粘贴时无法粘贴中断参数的问题。
    ([UUM-143599](https://issuetracker.unity3d.com/issues/interruption-source-ordered-interruption-and-can-transition-to-self-fields-are-not-pasted-to-transition-settings-when-pasting-transition-parameters))

- `Animation`: 重构了“动画可播放输出”的绑定和解除绑定验证逻辑，以防止潜在的崩溃。
    ([UUM-146750](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146750))

- `资源管道`: 修复了在删除引用纹理并使用相同 GUID 恢复后，资源预览仍显示为白色的问题。
    ([UUM-138622](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-138622))

- `资源管道`: 在跨进程导入器上调用 `CreateAsset` 时，不再导致程序崩溃。
    ([UUM-141087](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-141087))

- `音频`: 修复了在音频混音器中删除快照时发生的错误。
    ([UUM-119443](https://issuetracker.unity3d.com/issues/error-is-thrown-when-deleting-snapshot-with-another-snapshot-present-in-audio-mixer-window))

- `音频`: 修复了 `RootOutputInstance.IRealtime` 在被请求时无法正确通过 Burst 运行的问题，尽管 Burst 能够编译并显示相关代码在检查器中。
    ([UUM-145622](https://issuetracker.unity3d.com/issues/scriptable-audio-processor-rootoutput-isnt-bursted-at-runtime))

- `编辑器`: 当在 URP 和 HDRP 中将支持 XR 渲染的摄像机设置为正交视图时，会显示一条警告消息。
    ([UUM-63527](https://issuetracker.unity3d.com/issues/quest-reflections-change-shape-and-performance-is-impacted-when-the-camera-projection-is-set-to-orthographic))

- `编辑器`: 将色彩空间同步推迟至初始资源数据库刷新之后，以避免启动时发生崩溃。
    ([UUM-141297](https://issuetracker.unity3d.com/issues/在打开包含已添加播放器设置的构建配置文件的项目时，an-refreshinternalv2-is-called-before-initialrefresh-error-is-thrown-错误会在初始刷新前抛出))

- `编辑器`: 确保 SpriteRenderer 的材质已建立索引。
    (UUM-144279)

- `编辑器`: 修复了在多选带有不同 MonoBehaviour 脚本且使用 `[SerializeReference]` 字段的 GameObject 时，`SerializableManagedRef::CallMethod` 引发的崩溃问题。
    ([UUM-142019](https://issuetracker.unity3d.com/issues/crash-on-serializablemanagedref-callmethod-when-performing-various-unity-operations))

- `编辑器`: 修复了由 `AsyncInstantiateOperation` 中未被释放的 `CancellationTokenSource` 对象导致的内存泄漏问题。
    ([UUM-147016](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147016))

- `Editor`: 修复了 Sprite 资源检查器窗口对齐不正确的问题。
    ([UUM-145514](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-145514))

- `编辑器`: 修复了 `Handles.SnapValue` 和 `Snapping.Snap` 方法仅对正值进行对齐的问题，此行为符合 `Handles.SnapValue` API 文档中的描述。
    ([UUM-143716](https://issuetracker.unity3d.com/issues/handles-handles-dot-snapvalue-is-not-snapping-properly-with-negative-values))

- `编辑器`: 修复了在特定 Windows DPI 缩放与 Unity UI 缩放组合下，WinEditor 中出现的黑色条纹 artifacts 问题。
    ([UUM-146885](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146885))

- `编辑器`: 修复了由 AssetImporter 进程打开的 EditorWindows 在任务栏中成为孤立窗口的问题。
    ([UUM-145778](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-145778))

- `编辑器`: 修复了在 MS Windows 系统上，当本地包无法解析时可能导致编辑器崩溃的问题。
    ([UUM-146678](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146678))

- `编辑器`: 修复了当 OpenGLES 为活动图形 API 时，编辑器中 MSAA 纹理无法渲染的问题。
    ([UUM-143867](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-143867))

- `编辑器`: 修复了“自适应性能”设置中“帧率缩放器”的间距问题。
    ([UUM-141453](https://issuetracker.unity3d.com/issues/adaptive-performance-settings-framerate-field-doesnt-display-the-supported-without-vsync-warning-when-the-field-is-collapsed-in-build-profiles))

- `编辑器`: 修复了文本溢出不一致的问题。
    (UUM-145644)

- `编辑器`: 修复了 ATG 中使用的精灵资源相关的各种问题。
    ([UUM-145506](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-145506))

- `GI`: 修复了提取具有 null 材质的光源时发生的崩溃问题。
    ([UUM-132304](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-132304))

- `Graphics`: 修复了在 XR 模式下，通过注入的 RenderObjects 渲染通道启用动态分辨率时出现的渲染问题。
    ([UUM-142592](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-142592))

- `Graphics`: 对于已预热（warmed up）的 GraphicsStateCollection 变体，跳过耗时的按变体操作。
    (UUM-139193)

- `HDRP`: 更新了 `ClearBuffer2D` 着色器，以支持多视图。
    ([UUM-137877](https://issuetracker.unity3d.com/issues/hdrp-xr-dx12-ssr-pbr-accumulation-algorithm-artifacts-are-present-in-one-eye-when-using-spi-openxr-rendering-mode))

- `iOS`: 修复了深度相机第二次创建时发生的崩溃问题。
    ([UUM-141173](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-141173))

- `iOS`: 修复了应用进入后台时 iOS 平台上出现的错误提示“Touch 已被释放”。
    ([UUM-145381](https://issuetracker.unity3d.com/issues/ios-when-application-is-sent-to-background-with-active-touch-error-message-is-printed))

- `网络`: 将 libcurl 库升级至 8.20 版本。

- `包管理器`: 修复了当 Unity 账号名称包含引号时会生成无效包的问题。
    ([UUM-133956](https://issuetracker.unity3d.com/issues/package-manager-create-package-creates-invalid-json-when-unity-account-name-includes-quotes))

- `软件包管理器`: 修复了刷新页面时也会刷新用户授权许可证的问题。
    (UUM-147523)

- `包管理器`: 激活“播放模式”场景的附加编辑器时，会抛出与包管理器相关的错误。
    ([UUM-147009](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147009))

- `包管理器`: 存在授权问题的包会在包管理器窗口中正确显示为“未安装”。
    (UUM-134515)

- `物理系统`: 修复了因未正确执行 64 级链接深度限制而导致的 ArticulationBody 组件层级结构崩溃问题。
    ([UUM-145530](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-145530))

- `物理`: 修复了 ConfigurableJoint 设置在达到距离约束上限时会发生抖动的问题，该问题是由于其接触距离未被正确处理所致。
    ([UUM-146852](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146852))

- `物理`: 修复了 Rigidbody 组件序列化中的一个问题：在 2022LTS 版本中保存到场景中的预制体覆盖设置（针对阻力/角阻力）在升级后无法保留。
    ([UUM-147601](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147601))

- `Profiler`: 内存分析器低估了 ALLOC_TEMP_JOB_ASYNC 的内存占用，导致未使用的内存块被标记为“未跟踪”。
    ([UUM-145712](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-145712))

- `场景/游戏视图`: 修复了 SRP 体积控件在场景视图中无法显示的问题。
    ([UUM-146740](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146740))

- `UI 工具包`: 公开了 VectorUtils.BuildVectorImage(SceneInfo, Rect) 方法。
    ([UUM-146278](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146278))

- `UI Toolkit`: 修复了在 UI Builder 绑定窗口中某些类型转换器会被忽略的问题。
    ([UUM-147357](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147357))

- `UI 工具包`: 修复了过滤后的元素中不透明度无法传播的问题。
    ([UUM-147157](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147157))

- `UI 工具包`: 修复了预制件覆盖标记在“检查器”中无法显示的问题，以及在修复“检查器”滚动区域后出现的异常水平滚动条。
    ([UUM-147367](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147367))

- `UI 工具包`: 修复了使用带有 9 片切片和切片缩放的大型精灵时出现的渲染问题。
    ([UUM-147415](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147415))

- `UI 工具包`: 修复了当引用资产的 Addressables 内容被卸载并重新加载后，使用 -unity-material（以及其他基于资源的样式属性，如 background-image 和 -unity-font）进行样式设置的 VisualElements 会以默认着色器（纯白色）渲染的问题。
    ([UUM-144652](https://issuetracker.unity3d.com/issues/ui-toolkit-uss-materials-in-assetbundles-break-due-to-instanceid-referencing-a-material-that-no-longer-exists-when-a-scene-is-loaded-through-addressables-for-the-second-time))

- `通用 Windows 平台 (UWP)`：修复了在 UWP 环境下鼠标移动时滚动操作被重新触发的现象。
    ([UUM-144660](https://issuetracker.unity3d.com/issues/uwp-mouse-movement-re-triggers-stale-slash-scroll-value-after-the-scroll-wheel-is-used-once))

- `视频`: 修复了在 macOS 上使用 VideoPlayer 时，若处于“仅 API”模式并禁用 Unity Audio，AudioSampleProvider.sampleFramesAvailable 回调永远不会触发的issues。
    ([UUM-143660](https://issuetracker.unity3d.com/issues/audiosampleprovider-dot-sampleframesavailable-callback-never-fires-when-using-macos))

- `Web`: 修复了当服务器未设置“Content-Length”标头时，UnityWebRequest 中响应正文的流式传输问题。
    ([UUM-146537](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146537))




## 6000.3.21f1 版本中的包变更

## 已更新的包

- `com.unity.collections`: 从 [2.6.6](https://docs.unity3d.com/Packages/com.unity.collections@2.6//changelog/CHANGELOG.html) 更新至 [2.6.8](https://docs.unity3d.com/Packages/com.unity.collections@2.6//changelog/CHANGELOG.html)

- `com.unity.entities`: 从 [1.4.6](https://docs.unity3d.com/Packages/com.unity.entities@1.4//changelog/CHANGELOG.html) 更新至 [1.4.8](https://docs.unity3d.com/Packages/com.unity.entities@1.4//changelog/CHANGELOG.html)

- `com.unity.physics`: 从 [1.4.6](https://docs.unity3d.com/Packages/com.unity.physics@1.4//changelog/CHANGELOG.html) 更新至 [1.4.7](https://docs.unity3d.com/Packages/com.unity.physics@1.4//changelog/CHANGELOG.html)

- `com.unity.entities.graphics`: 从 [1.4.19](https://docs.unity3d.com/Packages/com.unity.entities.graphics@1.4//changelog/CHANGELOG.html) 更新至 [1.4.21](https://docs.unity3d.com/Packages/com.unity.entities.graphics@1.4//changelog/CHANGELOG.html)

- `com.unity.burst`: 从 [1.8.29](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html) 更新至 [1.8.30](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html)

- `com.unity.formats.alembic`: 从 [2.4.5](https://docs.unity3d.com/Packages/com.unity.formats.alembic@2.4//changelog/CHANGELOG.html) 更新至 [2.4.7](https://docs.unity3d.com/Packages/com.unity.formats.alembic@2.4//changelog/CHANGELOG.html)

- `com.unity.inputsystem`: 从 [1.19.0](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.19//changelog/CHANGELOG.html) 更新至 [1.20.0](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.20//changelog/CHANGELOG.html)

- `com.unity.services.authentication`: 从 [3.7.1](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.7//changelog/CHANGELOG.html) 更新至 [3.7.3](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.7//changelog/CHANGELOG.html)

- `com.unity.services.cloudcode`: 从 [2.10.3](https://docs.unity3d.com/Packages/com.unity.services.cloudcode@2.10//changelog/CHANGELOG.html) 更新至 [2.10.4](https://docs.unity3d.com/Packages/com.unity.services.cloudcode@2.10//changelog/CHANGELOG.html)

- `com.unity.services.economy`: 从 [3.5.3](https://docs.unity3d.com/Packages/com.unity.services.economy@3.5//changelog/CHANGELOG.html) 更新至 [3.5.4](https://docs.unity3d.com/Packages/com.unity.services.economy@3.5//changelog/CHANGELOG.html)

- `com.unity.visualscripting`: 从 [1.9.11](https://docs.unity3d.com/Packages/com.unity.visualscripting@1.9//changelog/CHANGELOG.html) 更新至 [1.9.12](https://docs.unity3d.com/Packages/com.unity.visualscripting@1.9//changelog/CHANGELOG.html)

- `com.unity.transport`: 从 [2.7.3](https://docs.unity3d.com/Packages/com.unity.transport@2.7//changelog/CHANGELOG.html) 更新至 [2.7.4](https://docs.unity3d.com/Packages/com.unity.transport@2.7//changelog/CHANGELOG.html)

- `com.unity.ai.navigation`: 从 [2.0.13](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html) 更新至 [2.0.14](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html)

- `com.unity.microsoft.gdk`: 从 [1.6.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk@1.6//changelog/CHANGELOG.html) 更新至 [1.7.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk@1.7//changelog/CHANGELOG.html)

- `com.unity.microsoft.gdk.tools`: 从 [1.6.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.tools@1.6//changelog/CHANGELOG.html) 更新至 [1.7.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.tools@1.7//changelog/CHANGELOG.html)