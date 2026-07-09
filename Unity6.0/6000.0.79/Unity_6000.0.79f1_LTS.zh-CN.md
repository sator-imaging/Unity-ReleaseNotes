# Unity 6000.0.79f1 LTS
发布于 2026年7月8日 星期三 14:28:55 GMT  
https://unity.com/releases/editor/whats-new/6000.0.79f1

# 6000.0.79f1 版本中的已知问题

- `6000.0.67f1`: [iOS] 访问 iOS 控制中心时音频中断
    ([UUM-145522](https://issuetracker.unity3d.com/issues/ios-audio-is-cut-out-when-accessing-ios-control-center))

- `6000.0.6f1`: [RenderGraph][D3D12] 当使用 AddComputePass 并同时启用 EnableAsyncCompute(true) 和 UseTexture 时，D3D12SwapChain::Present 会发生崩溃
    ([UUM-140183](https://issuetracker.unity3d.com/issues/rendergraph-d3d12-crash-on-d3d12swapchain-present-when-using-addcomputepass-with-enableasynccompute-true-and-usetexture))

- `资源导入器`: 进入播放模式时，编辑器在执行“(Unity) WriteObjectToVector”操作时崩溃
    ([UUM-112617](https://issuetracker.unity3d.com/issues/editor-crashes-on-unity-writeobjecttovector-when-entering-into-the-play-mode))

- `Metal`: 命令缓冲区超时错误后游戏卡死
    ([UUM-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

当有多个 bee_backend 实例同时运行时，在调用 mono_log_write_logfile 时发生崩溃
    ([UUM-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))

生成字体图集时发生崩溃，并产生多个堆栈跟踪
    ([UUM-141061](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-generating-font-atlas-with-sdf16-or-sdf32))



# 6000.0.79f1 发布说明

## 改进

- `构建系统`: 将捆绑的 7-Zip 更新至 26.02 版本。

- `图形`: 更新了 Mipmap 流式传输手册页面，说明了 Unity 如何根据网格 UV 数据和摄像机位置选择 Mipmap 级别；澄清了 Unity 无法计算级别对象的行为（包括粒子系统等程序生成的几何体）；并添加了 `Texture2D.requestedMipmapLevel` 代码示例。
    ([UUM-131691](https://issuetracker.unity3d.com/issues/texture-rendered-at-different-fidelity-with-particle-system-renderer-when-using-a-different-material-derived-from-the-same-texture-with-identical-settings))



## 变更

- `Android`: 将 Gradle 升级至 9.1.0，将 AGP 升级至 9.0.0。



## 修复

- `2D`: 修复了 Light2D 序列化冲突。
    (UUM-141743)

- `2D`: 修复了质量设置无法传播到相机目标描述符的问题。
    ([UUM-141000](https://issuetracker.unity3d.com/issues/quality-fields-are-not-propagated-to-the-camera-target-descriptor-when-using-renderer2ds-rendergraph-path))

- `AI`: 修复了因错误使用 UNITY_FREE 代替 UNITY_DELETE 导致的内存泄漏。
    (UUM-144085)

- `Android`: 修复了按目标架构拆分的 APK 均获得相同版本码的问题。
    ([UUM-144372](https://issuetracker.unity3d.com/issues/arm64-and-armv7-apks-return-the-same-version-code-when-split-apks-by-target-architecture-is-enabled))

- `Android`: 将未使用的 Tools 26.1.1 下载文件替换为空文件夹。
    (UUM-141878)

- `文档`: 为 UITK 弹出窗口示例代码和操作步骤添加了更多背景信息和细节。

- `文档`: 更新了 VFX 运算符 Reciprocal 中错误的 'out' 属性。
    (UUM-144446)

- `编辑器`: 新增了一个选项，用于阻止模型导入器在整个项目范围内搜索纹理。
    (UUM-137345)

- `编辑器`: 音频：修复了打开包含损坏的音频混音器资源的项目时，编辑器会崩溃的问题。
    ([UUM-143706](https://issuetracker.unity3d.com/issues/crash-on-audiomixercontroller-removeinvalidsendlevelguidsrecursive-when-opening-a-project-with-specific-audio-files-for-the-first-time))

- `编辑器`: 修复了在编辑器关闭时，受管 `DomainUnload` 处理程序执行 `UnityEngine.Object` 空值检查时发生的崩溃（`ProfilerMutexLock / 断言 gPersistentManager \!= NULL`）。
    ([UUM-144371](https://issuetracker.unity3d.com/issues/crash-on-profilermutexlock-when-closing-a-project-with-specific-assets))

- `编辑器`: 修复了在 Wayland 环境下运行时，将文件拖入编辑器所引发的 LinuxEditor 错误。
    ([UUM-111593](https://issuetracker.unity3d.com/issues/linux-the-error-releasebutton-expects-buttonid-is-thrown-when-trying-to-add-file-using-drag-and-hold-in-the-project-window))

- `Editor`: 修复了在 RedrawFromNative 期间若打开或关闭新窗口，InspectorWindow 会抛出异常的问题。
    ([UUM-141990](https://issuetracker.unity3d.com/issues/invalidoperationexception-is-thrown-when-clicking-ctrl-plus-z-after-opening-gradient-editor))

- `Editor`: 修复了 Perforce 中未跟踪文件夹导致 VCCache 陷入无限重新查询循环的问题。
    ([UUM-143313](https://issuetracker.unity3d.com/issues/cpu-usage-spikes-when-perforce-version-control-is-set-up-and-ai-assistant-is-installed))

- `编辑器`: 改进了矢量图形的哈希码计算。
    ([UUM-143005](https://issuetracker.unity3d.com/issues/hdrp-bloom-renders-with-a-purple-blue-or-green-anomaly-in-the-game-view-当在纵横比可被16整除且图形API设置为DX11或DX12时，切换带摄像机变形的晕影和变形体积设置))

- `编辑器`: 本地文档曾被意外删除，现已恢复。
    (UUM-143984)

- `编辑器`: 修复了预制体使用保留字段时可能导致的崩溃问题。
    ([UUM-144557](https://issuetracker.unity3d.com/issues/crash-on-saveprefabasset-when-selecting-a-specific-prefab))

- `编辑器`: 修复了当选择操作打开原生模态对话框时，对象选择器会卡死的问题。
    ([UUM-139847](https://issuetracker.unity3d.com/issues/object-selector-becomes-unresponsive-when-selecting-root-ui-document-as-data-source-for-add-binding-in-ui-builder))

- `Graphics`: 修复了“ImageConversion.LoadImage”在尝试加载 IDAT 块损坏的 PNG 文件时可能导致内存泄漏的问题。
    ([UUM-143641](https://issuetracker.unity3d.com/issues/当ImageConversion.LoadImage无法解码一个头部有效但IDAT块数据损坏的PNG文件时，会分配一个持久的4096字节临时内存并导致内存泄漏))

- `Graphics`: 修复了在 Windows 上使用 Vulkan 并启用“拆分图形任务”时，缓存中可能插入空值的问题，这会导致 DrawCalls 尝试在已关闭的命令缓冲区中绘制，从而引发崩溃。
    (UUM-132307)

- `IL2CPP`: 修复了在 Linux 上生成空 .usym 文件的问题。
    ([UUM-142527](https://issuetracker.unity3d.com/issues/linux-stack-trace-file-path-and-line-number-information-is-missing-when-il2cpp-stacktrace-information-is-set-to-method-name-file-name-and-line-number))

- `输入系统`: 修复了 Windows 系统上一个错误，该错误导致具有大型供应商定义报告（例如 `ReportCount=1024`\) 会因发出重复的描述符元素而生成巨大的设备 `capabilities` 字符串。现在描述符大小已恢复正常，且不影响设备的实际控制功能。
    (UUM-144506)

- `内核`: 修复了作业系统中涉及大量外部线程和手动作业的潜在死锁问题。
    (UUM-143073)

- `Linux`: 修复了在 Linux 编辑器中构建 Windows 播放器以及创建 Visual Studio 解决方案时的错误。
    ([UUM-140187](https://issuetracker.unity3d.com/issues/linuxeditor-building-for-windows-throws-agilitysdk-dll-could-not-be-retrieved-when-create-visual-studio-solution-was-enabled-before-switching-build-platform-to-windows))

- `Linux`: 修复了在新输入系统下触摸屏双击无法被识别的问题。
    ([UUM-145665](https://issuetracker.unity3d.com/issues/linux-double-taps-on-touch-screens-are-not-recognized-on-new-input-system))

- `网络`: 修复了 UnityWebRequest 中一个问题，即恢复上传请求时，有时会记录错误代码 26 或 65（“无法执行必要的数据回卷”）。
    ([UUM-144767](https://issuetracker.unity3d.com/issues/webrequest-missing-curlopt-seekfunction-causes-curl-error-26-on-post-retry-with-reused-connections))

- `Physics`: 修复了 Physics.RebuildBroadphaseRegions 方法中的崩溃问题，该问题可能发生在对未使用多盒子剪枝广相法（multi-box prunning broadphase）的物理场景调用该方法时。
    ([UUM-144472](https://issuetracker.unity3d.com/issues/physics-dot-rebuildbroadphaseregions-does-not-repopulate-them-with-pre-existing-shapes))

- `Physics`: 修复了一个问题：调用 `Physics.RebuildBroadphaseRegions` 可能会导致已存在的 Collider 组件被排除在新生成的广相区域之外。
    ([UUM-144472](https://issuetracker.unity3d.com/issues/physics-dot-rebuildbroadphaseregions-does-not-repopulate-them-with-pre-existing-shapes))

- `Profiler`: 修复了 ProfilerSymbolsDelayedDeletion::AddCloneObject 中的崩溃问题。
    ([UUM-144194](https://issuetracker.unity3d.com/issues/crash-on-profilersymbolsdelayeddeletion-addcloneobject-when-deserializing-an-object-instantiate-marker-with-a-dangling-slash-corrupt-name-string))

- `UI 工具包`: 修复了使用触控设备在 SceneView 中拖动 GameObject 时，若移动路径穿过工具栏或其他编辑器窗口会导致程序崩溃的问题。
    ([UUM-142652](https://issuetracker.unity3d.com/issues/gameobject-movement-in-scene-view-becomes-stuttery-and-intermittently-freezes-when-using-non-standard-pointers-across-editor-tabs-or-window-boundaries))

- `URP`: 修复了 URP 独立播放器构建中导致播放器日志出现内存泄漏警告的问题。
    ([UUM-115886](https://issuetracker.unity3d.com/issues/jobtempalloc-memory-leak-warning-is-thrown-when-the-player-is-shut-down))

- `Windows`: 修复了在独立播放器构建中使用输入管理器时，Windows 手写笔输入无法触发鼠标指针事件（`Input.GetMouseButtonDown`）的问题。
    ([UUM-140737](https://issuetracker.unity3d.com/issues/windows-pen-input-does-not-generate-mouse-pointer-events-when-using-input-manager))

- `Windows`: 修复了在 Windows 触摸屏设备上执行捏合手势后，UI 工具包按钮对触摸无响应的问题。
    ([UUM-138595](https://issuetracker.unity3d.com/issues/ui-toolkit-buttons-stop-responding-to-single-taps-when-a-multi-touch-gesture-is-performed-with-the-new-input-system-on-windows-touch-devices))

- `Windows`: 修复了 Windows IL2CPP 构建时出现 LNK1104 错误的问题。
    ([UUM-139929](https://issuetracker.unity3d.com/issues/使用 IL2CPP 构建 Windows x64 版本时，若已安装 Visual Studio 2026 和 2022，会因链接错误导致构建失败))




## 6000.0.79f1 版本中的包变更

## 已更新的包

- `com.unity.netcode`: 从 [1.13.2](https://docs.unity3d.com/Packages/com.unity.netcode@1.13//changelog/CHANGELOG.html) 更新至 [1.14.0](https://docs.unity3d.com/Packages/com.unity.netcode@1.14//changelog/CHANGELOG.html)

- `com.unity.nuget.newtonsoft-json`: 从 [3.2.1](https://docs.unity3d.com/Packages/com.unity.nuget.newtonsoft-json@3.2//changelog/CHANGELOG.html) 升级至 [3.2.2](https://docs.unity3d.com/Packages/com.unity.nuget.newtonsoft-json@3.2//changelog/CHANGELOG.html)

- `com.unity.services.cloudcode`: 从 [2.7.1](https://docs.unity3d.com/Packages/com.unity.services.cloudcode@2.7//changelog/CHANGELOG.html) 更新至 [2.10.2](https://docs.unity3d.com/Packages/com.unity.services.cloudcode@2.10//changelog/CHANGELOG.html)

- `com.unity.services.core`: 从 [1.16.0](https://docs.unity3d.com/Packages/com.unity.services.core@1.16//changelog/CHANGELOG.html) 更新至 [1.18.0](https://docs.unity3d.com/Packages/com.unity.services.core@1.18//changelog/CHANGELOG.html)

- `com.unity.services.economy`: 从 [3.5.1](https://docs.unity3d.com/Packages/com.unity.services.economy@3.5//changelog/CHANGELOG.html) 更新至 [3.5.3](https://docs.unity3d.com/Packages/com.unity.services.economy@3.5//changelog/CHANGELOG.html)

- `com.unity.services.leaderboards`: 从 [2.2.1](https://docs.unity3d.com/Packages/com.unity.services.leaderboards@2.2//changelog/CHANGELOG.html) 更新至 [2.3.3](https://docs.unity3d.com/Packages/com.unity.services.leaderboards@2.3//changelog/CHANGELOG.html)

- `com.unity.multiplayer.tools`: 从 [2.2.8](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@2.2//changelog/CHANGELOG.html) 更新至 [2.2.9](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@2.2//changelog/CHANGELOG.html)

- `com.unity.services.deployment.api`: 从 [1.0.0](https://docs.unity3d.com/Packages/com.unity.services.deployment.api@1.0//changelog/CHANGELOG.html) 更新至 [1.1.3](https://docs.unity3d.com/Packages/com.unity.services.deployment.api@1.1//changelog/CHANGELOG.html)

**新增包**

- [com.unity.xr.compositionlayers@2.5.0](https://docs.unity3d.com/Packages/com.unity.xr.compositionlayers@2.5//changelog/CHANGELOG.html)