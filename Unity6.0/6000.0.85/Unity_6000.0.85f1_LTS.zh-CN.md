# Unity 6000.0.85f1 LTS
发布于 2026年10月15日 星期四 11:57:40 GMT  
https://unity.com/releases/editor/whats-new/6000.0.85f1

# 6000.0.85f1 中的已知问题

- `6000.0.6f1`: [RenderGraph][D3D12] 当使用 AddComputePass 并同时启用 EnableAsyncCompute(true) 和 UseTexture 时，D3D12SwapChain::Present 会发生崩溃  
    ([UUM-140183](https://issuetracker.unity3d.com/issues/rendergraph-d3d12-crash-on-d3d12swapchain-present-when-using-addcomputepass-with-enableasynccompute-true-and-usetexture))

- `6000.0.75f1`: 使用 SceneManager.LoadSceneAsync 反复切换场景时，玩家会永久停止响应
    ([UUM-156125](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156125))

当有多个 bee_backend 实例同时运行时，mono_log_write_logfile 会引发崩溃
    ([UUM-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))



# 6000.0.85f1 发布说明

## 改进

- `构建系统`: 将捆绑的 7-Zip 更新至 26.03 版本。



## API 变更

- `Graphics`: 新增：添加了 Graphics.disableDepthAndStencilBuffers，这是一个只读属性，用于返回“播放器设置”中是否启用了“禁用深度和模板缓冲区”选项。



## 变更

- `Android`: 将 Android Gradle 插件（AGP）版本从 9.0.0 更新至 9.1.1。



## 修复

- `2D`: 修复了在 2D 渲染器中使用叠加摄像机时出现的 ArgumentException 异常。
    ([UUM-148111](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-148111))

- `2D`: 修复了在 Sprite 编辑器窗口发生变化时进入快速播放模式所引发的错误提示。
    ([UUM-146790](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146790))

- `2D`: 修复了渲染通道请求时未生成中间纹理的问题。
    ([UUM-145892](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-145892))

- `2D`: 修复了在游戏对象上切换启用状态时，LineRenderer 无法正确初始化的问题。
    ([UUM-147747](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147747))

- `2D`: 修复了相机排序层纹理分辨率受 2D Renderer 上“渲染比例”设置影响的问题。
    ([UUM-151723](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151723))

- `Android`: 修复了在选择目标 API 级别 37 时出现的“无法找到哈希字符串为 android-37 的目标”问题。
    ([UUM-150216](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150216))

- `Android`: 修复了输入时光标会退回文本末尾的问题。
    ([UUM-121294](https://issuetracker.unity3d.com/issues/android-ios-the-input-field-caret-moves-back-to-the-end-of-the-text-when-typing))

- `Android`: 修复了虚拟键盘与 UGUI 文本框之间的双向同步问题。
    (UUM-133870)

- `Android`: 修复了 `editText` 的 `setText` 方法会将输入法（IME）的内部光标重置为文本末尾的问题，无论 `EditText` 的选中状态如何。
    (UUM-142513)

- `Android`: 修复了在 UaaL 模式下，`GameActivity` 卸载后立即重新启动时出现的卡死问题。
    (UUM-149857)

- `Android`: 修复了 `TouchScreenKeyboard.selection.length` 始终返回 `0` 的问题。
    ([UUM-125821](https://issuetracker.unity3d.com/issues/android-touchscreenkeyboard-dot-selection-dot-length-always-returns-0-when-any-length-text-is-selected))

- `资源包 (Asset Bundles)`：修复了从一个资源包中实例化预制体时，若该资源包是通过另一个资源包中预制体的子对象引用访问的，会导致播放器崩溃的问题。
    (UUM-141605)

- `音频`: 修复了 macOS 上当系统正在使用麦克风时，音频播放会变慢的 bug。
    ([UUM-149880](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149880))

- `编辑器`: 修复了 Linux 编辑器未将“帮助”和“窗口”菜单锚定在主菜单栏末尾的错误。
    (UUM-113169)

- `编辑器`: 修复了在 Direct3D12 环境下，当异步着色器编译仍在进行时退出“播放模式”会导致死锁的问题。
    ([UUM-152966](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-152966))

- `编辑器`: 修复了访问叠加层容器的 rootVisualElement 可能导致递归调用并使编辑器崩溃的问题。
    ([UUM-149209](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149209))

- `编辑器`: 修复了在显示“场景已修改”对话框时，多次按下 Cmd+Q 会导致编辑器崩溃的问题。<br>
    修复了在“播放”模式下退出编辑器且存在未保存更改时，会显示两个“场景已修改”对话框的问题。
    ([UUM-149668](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149668))

- `Graphics`: 修复了在启用图形任务时，Graphics.RenderPrimitives 和 Graphics.DrawProcedural 与 MeshTopology.Quads 配合使用会导致程序崩溃的问题。
    ([UUM-141117](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-141117))

- `macOS`: 修复了在最新版本的 macOS 上导入 X.509 证书时可能发生的崩溃问题。
    (UUM-154511)

- `多人游戏`: Unity Transport：修复了使用 DTLS 或 TLS 关闭连接时发生的内存泄漏问题。
    ([UUM-151755](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151755))

- `网络`: 修复了当向同一主机发出的较快并发请求已设置了较新 Cookie 后，较慢的请求完成时，UnityWebRequest 的 Cookie 偶尔会恢复为较旧值的问题。
    ([UUM-150958](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150958))

- `网络`: UnityWebRequest：修复了在独立播放器退出时，若正在进行的请求仍在针对无响应或响应缓慢的 DNS 服务器进行 DNS 解析，会导致程序卡死的问题。
    ([UUM-151643](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151643))

- `粒子`: 修复了“摄像机淡出”与“柔和粒子”同时启用时，在某些设备上会导致粒子消失的问题。
    ([UUM-146249](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146249))

- `Player`: 添加了保护机制，以避免在开发版玩家构建中触发调试断言。
    (UUM-152365)

- `Player`: 在运行时修改 Shader.globalMaximumLOD 后，GameObject 会投射正确的阴影。
    ([UUM-150226](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150226))

- `Profiler`: 修复了 Profiler 中“排查连接问题”按钮链接到与连接故障排除无关的文档页面的问题。
    ([UUM-153354](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-153354))

- `着色器`: 修复了因向着色器全局属性 API 提供超出范围的值而导致的崩溃问题。
    ([UUM-150856](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150856))

- `源代码构建`: 修复了在采用土耳其地区格式的机器上，编辑器源代码构建失败的问题。
    (UUM-154501)

- `地形`: 修复了加载高度图分辨率超过设备最大渲染纹理大小的地形时发生的崩溃问题，例如在限制为 4096 的设备上加载 4097 的高度图。
    ([UUM-150551](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150551))

- `文本`: 修复了当 TextMesh 或旧版 UI 文本字符串以未终止的四边形标签参数结尾时发生的越界内存读取问题。
    (UUM-153129)

- `Text`: 修复了当 TextMesh 或旧版 UI Text 字符串以未结束的富文本标签结尾时发生的越界内存读取问题。
    (UUM-153128)

- `UI Toolkit`: 修复了在 macOS 上运行的 Web 构建中，多列列表和树形视图需要使用 Ctrl+点击而非 Cmd+点击才能按多列排序的问题。

- `UI Toolkit`: 修复了在 macOS 上运行的 Web 构建中，指针、鼠标、键盘和导航事件的操作键被设置为 Ctrl 而非 Cmd 的问题。
    ([UUM-153940](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-153940))

- `通用 Windows 平台 (UWP)`：修复了 Xbox 上确认屏幕键盘后，文本字段会被清空而非保留已输入文本的问题。
    (UUM-154127)

- `通用 Windows 平台 (UWP)`：修复了 Xbox 上按 B 键关闭屏幕键盘时，输入的文本会被保留而非恢复为先前值的问题。
    (UUM-149423)

- `URP`: 修复了一个错误，即重新加载场景会导致某些 `Blitter` 函数停止工作。
    (UUM-153092)

- `URP`: 修复了一个错误，即在半精度平台（移动端）上，盒形投影反射探针会出现接缝。
    ([UUM-141981](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-141981))

- `URP`: 修复了在某些 Android Vulkan 设备上 `RenderTexture.Create` 失败的问题。
    ([UUM-91313](https://issuetracker.unity3d.com/issues/android-vulkan-error-rendertexture-dot-create-failed-format-unsupported-for-random-writes-r16-sfloat-45-dot-logged-when-during-launch-on-an-project-with-urp-2d-renderer))

- `URP`: 修复了因 uv4 输入语义差异导致的 ShaderGraph 编译失败问题。
    ([UUM-143884](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-143884))

- `URP`: 修复了在“玩家设置”中启用“禁用深度和模板缓冲区”时，2D 渲染器仍在玩家中创建深度和模板缓冲区的问题。
    ([UUM-150232](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150232))

- `URP`: ScriptableRendererData.TryGetRendererFeature 会抛出 NullReferenceException 异常。
    ([UUM-150772](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150772))

- `VFX Graph`: 修复了在特定体素数量下使用 `MeshToSDFBaker` 时发生的越界访问问题。
    ([UUM-151674](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151674))

- `Web`: 修复了内存分析器中使用的 WASM_SIZE 和 wasmFileSize 相关问题。
    (UUM-149075)

- `Web`: 修复了当输出资源大小超过 2 GB 时的 Web 平台构建问题，以及输出资源大小超过 4 GB 时（不支持）出现的构建错误信息。
    ([UUM-112909](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-112909))




## 6000.0.85f1 版本中的包变更

## 已更新的包

- `com.unity.collections`: [2.6.8](https://docs.unity3d.com/Packages/com.unity.collections@2.6//changelog/CHANGELOG.html) 更新至 [2.7.1](https://docs.unity3d.com/Packages/com.unity.collections@2.7//changelog/CHANGELOG.html)

- `com.unity.entities`: 从 [1.4.8](https://docs.unity3d.com/Packages/com.unity.entities@1.4//changelog/CHANGELOG.html) 更新为 [1.5.0](https://docs.unity3d.com/Packages/com.unity.entities@1.5//changelog/CHANGELOG.html)

- `com.unity.netcode`: 从 [1.14.2](https://docs.unity3d.com/Packages/com.unity.netcode@1.14//changelog/CHANGELOG.html) 更新至 [1.14.3](https://docs.unity3d.com/Packages/com.unity.netcode@1.14//changelog/CHANGELOG.html)

- `com.unity.physics`: 从 [1.4.7](https://docs.unity3d.com/Packages/com.unity.physics@1.4//changelog/CHANGELOG.html) 更新至 [1.5.0](https://docs.unity3d.com/Packages/com.unity.physics@1.5//changelog/CHANGELOG.html)

- `com.unity.entities.graphics`: 从 [1.4.21](https://docs.unity3d.com/Packages/com.unity.entities.graphics@1.4//changelog/CHANGELOG.html) 更新至 [1.5.0](https://docs.unity3d.com/Packages/com.unity.entities.graphics@1.5//changelog/CHANGELOG.html)

- `com.unity.mobile.notifications`: 从 [2.4.3](https://docs.unity3d.com/Packages/com.unity.mobile.notifications@2.4//changelog/CHANGELOG.html) 更新至 [2.5.0](https://docs.unity3d.com/Packages/com.unity.mobile.notifications@2.5//changelog/CHANGELOG.html)

- `com.unity.services.authentication`: 从 [3.7.4](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.7//changelog/CHANGELOG.html) 更新至 [3.8.0](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.8//changelog/CHANGELOG.html)

- `com.unity.services.friends`: 从 [1.1.0](https://docs.unity3d.com/Packages/com.unity.services.friends@1.1//changelog/CHANGELOG.html) 更新至 [1.3.0](https://docs.unity3d.com/Packages/com.unity.services.friends@1.3//changelog/CHANGELOG.html)

- `com.unity.services.wire`: 从 [1.5.0](https://docs.unity3d.com/Packages/com.unity.services.wire@1.5//changelog/CHANGELOG.html) 更新至 [1.6.0](https://docs.unity3d.com/Packages/com.unity.services.wire@1.6//changelog/CHANGELOG.html)

- `com.unity.splines`: 从 [2.8.4](https://docs.unity3d.com/Packages/com.unity.splines@2.8//changelog/CHANGELOG.html) 升级至 [2.9.1](https://docs.unity3d.com/Packages/com.unity.splines@2.9//changelog/CHANGELOG.html)

- `com.unity.xr.management`: 从 [4.5.4](https://docs.unity3d.com/Packages/com.unity.xr.management@4.5//changelog/CHANGELOG.html) 更新至 [4.6.1](https://docs.unity3d.com/Packages/com.unity.xr.management@4.6//changelog/CHANGELOG.html)

- `com.unity.profiling.systemmetrics.mali`: 从 [1.1.1](https://docs.unity3d.com/Packages/com.unity.profiling.systemmetrics.mali@1.1//changelog/CHANGELOG.html) 升级至 [1.1.4](https://docs.unity3d.com/Packages/com.unity.profiling.systemmetrics.mali@1.1//changelog/CHANGELOG.html)

- `com.unity.multiplayer.tools`: 从 [2.2.10](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@2.2//changelog/CHANGELOG.html) 更新至 [2.2.12](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@2.2//changelog/CHANGELOG.html)

- `com.unity.ai.navigation`: 从 [2.0.14](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html) 更新至 [2.0.15](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html)

- `com.unity.asset-manager-for-unity`: 从 [1.11.0](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.11//changelog/CHANGELOG.html) 升级至 [1.12.0](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.12//changelog/CHANGELOG.html)

- `com.unity.cloud.draco`: 从 [5.4.3](https://docs.unity3d.com/Packages/com.unity.cloud.draco@5.4//changelog/CHANGELOG.html) 更新至 [5.5.0](https://docs.unity3d.com/Packages/com.unity.cloud.draco@5.5//changelog/CHANGELOG.html)

- `com.unity.cloud.ktx`: 从 [3.6.3](https://docs.unity3d.com/Packages/com.unity.cloud.ktx@3.6//changelog/CHANGELOG.html) 更新至 [3.7.1](https://docs.unity3d.com/Packages/com.unity.cloud.ktx@3.7//changelog/CHANGELOG.html)

- `com.unity.xr.compositionlayers`: 从 [2.5.0](https://docs.unity3d.com/Packages/com.unity.xr.compositionlayers@2.5//changelog/CHANGELOG.html) 更新至 [2.6.0](https://docs.unity3d.com/Packages/com.unity.xr.compositionlayers@2.6//changelog/CHANGELOG.html)