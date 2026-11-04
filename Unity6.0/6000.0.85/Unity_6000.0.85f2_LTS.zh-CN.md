# Unity 6000.0.85f2 LTS
发布于 2026年11月3日 星期二 16:15:34 GMT  
https://unity.com/releases/editor/whats-new/6000.0.85f2

# 6000.0.85f2 中的已知问题

- `Android`: 当启用“在后台运行”和“预测性返回支持”时，从后台返回后，使用返回手势或按钮会关闭应用
    ([UUM-159613](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-159613))

- `DirectX12`: 当使用 AddComputePass 并同时启用 EnableAsyncCompute(true) 和 UseTexture 时，D3D12SwapChain::Present 会发生崩溃
    ([UUM-140183](https://issuetracker.unity3d.com/issues/rendergraph-d3d12-crash-on-d3d12swapchain-present-when-using-addcomputepass-with-enableasynccompute-true-and-usetexture))

- `编辑器安装程序`: [macOS] 播放器库已使用定制权限进行代码签名
    ([UUM-156884](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156884))

- `脚本构建时`: 当有多个 bee_backend 实例同时运行时，调用 mono_log_write_logfile 会导致崩溃
    ([UUM-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))

- `着色器系统`: 使用 SceneManager.LoadSceneAsync 反复切换场景时，玩家会永久停止响应
    ([UUM-156125](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156125))



# 6000.0.85f2 发布说明

## 改进

- `构建系统`: 将捆绑的 7-Zip 更新至 26.03 版本。



## API 变更

- `Graphics`: 新增：添加了 Graphics.disableDepthAndStencilBuffers，这是一个只读属性，用于返回“播放器设置”中是否启用了“禁用深度和模板缓冲区”选项。



## 变更

- `Android`: 将 Android Gradle 插件 (AGP) 版本从 9.0.0 更新至 9.1.1。



## 修复

- `2D`: 修复了在 2D 渲染器中使用叠加摄像机时出现的 ArgumentException 异常。
    ([UUM-148111](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-148111))

- `2D`: 修复了在 Sprite 编辑器窗口发生更改后进入快速播放模式时出现的错误信息。
    ([UUM-146790](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146790))

- `2D`: 修复了渲染通道请求时未生成中间纹理的问题。
    ([UUM-145892](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-145892))

- `2D`: 修复了在游戏对象上切换启用状态时，LineRenderer 无法正确初始化的问题。
    ([UUM-147747](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147747))

- `2D`: 修复了相机排序层的纹理分辨率受 2D Renderer 上“渲染比例”设置影响的问题。
    ([UUM-151723](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151723))

- `Android`: 修复了在选择目标 API 级别 37 时出现的“无法找到哈希字符串为 android-37 的目标”错误。
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

- `编辑器`: 修复了访问叠加层容器的 `rootVisualElement` 可能导致递归调用并使编辑器崩溃的问题。
    ([UUM-149209](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149209))

- `编辑器`: 修复了在显示“场景已修改”对话框时，多次按下 Cmd+Q 会导致编辑器崩溃的问题。<br>
    修复了在“播放模式”下退出编辑器且存在未保存更改时，会显示两个“场景 已修改”对话框同时显示的问题。
    ([UUM-149668](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149668))

- `Graphics`: 修复了在启用图形任务时，Graphics.RenderPrimitives 和 Graphics.DrawProcedural 与 MeshTopology.Quads 配合使用会导致崩溃的问题。
    ([UUM-141117](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-141117))

- `IL2CPP`: 修复了 System.IO.Compression.BrotliStream 和 BrotliDecoder 所使用的 Brotli 解码器中存在的安全漏洞 \(CVE-2026-111497\)，该漏洞可能导致解码不受信任的数据时发生远程代码执行。

- `macOS`: 修复了在较新版本的 macOS 上导入 X.509 证书时可能发生的崩溃问题。
    (UUM-154511)

- `Mono`: 修复了 System.IO.Compression.BrotliStream 和 BrotliDecoder 所使用的 Brotli 解码器中存在的安全漏洞 \(CVE-2026-111497\)，该漏洞可能导致解码不受信任的数据时发生远程代码执行。

- `多人游戏`: Unity Transport：修复了使用 DTLS 或 TLS 关闭连接时出现的内存泄漏问题。
    ([UUM-151755](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151755))

- `网络`: 修复了当向同一主机发出的较快并发请求已设置了较新 Cookie 后，较慢的请求完成时，UnityWebRequest 的 Cookie 偶尔会恢复为较旧值的问题。
    ([UUM-150958](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150958))

- `网络`: 拒绝与使用已泄露的 eMudhra 证书的服务器建立 TLS 连接。
    (UUM-158231)

- `网络`: UnityWebRequest：修复了在独立播放器退出时，若正在进行的请求仍在对无响应或响应缓慢的 DNS 服务器进行 DNS 解析，会导致程序卡死的问题。
    ([UUM-151643](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151643))

- `包管理器`: 通过将包管理器使用的 Node.js 运行时更新至 v22.23.4，修复了一个可能导致远程代码执行的安全漏洞 \(CVE-2026-111497\)。

- `粒子效果`: 修复了“摄像头淡出”与“柔和粒子”同时启用时，在某些设备上会导致粒子消失的问题。
    ([UUM-146249](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146249))

- `Player`: 添加了保护机制，以避免在开发版播放器构建中触发调试断言。
    (UUM-152365)

- `Player`: 在运行时更改 Shader.globalMaximumLOD 后，GameObject 会投射正确的阴影。
    ([UUM-150226](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150226))

- `Profiler`: 修复了 Profiler 中“排查连接问题”按钮链接到与连接故障排除无关的文档页面的问题。
    ([UUM-153354](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-153354))

- `着色器`: 修复了因向着色器全局属性 API 提供超出范围的值而导致的崩溃问题。
    ([UUM-150856](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150856))

- `源代码构建`: 修复了在采用土耳其地区格式的机器上，编辑器源代码构建失败的问题。
    (UUM-154501)

- `地形`: 修复了加载高度图分辨率超过设备最大渲染纹理大小的地形时发生的崩溃问题，例如在最大渲染纹理大小限制为 4096 的设备上加载 4097 分辨率的高度图。
    ([UUM-150551](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150551))

- `文本`: 修复了当 TextMesh 或旧版 UI 文本字符串以未终止的四边形标签参数结尾时发生的越界内存读取问题。
    (UUM-153129)

- `Text`: 修复了当 TextMesh 或旧版 UI Text 字符串以未终止的富文本标签结尾时发生的越界内存读取问题。
    (UUM-153128)

- `UI Toolkit`: 修复了在 macOS 上运行的 Web 构建中，多列列表和树形视图需要使用 Ctrl+点击而非 Cmd+点击才能按多列排序的问题。

- `UI Toolkit`: 修复了在 macOS 上运行的 Web 构建中，指针、鼠标、键盘和导航事件的操作键被设置为 Ctrl 而非 Cmd 的问题。
    ([UUM-153940](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-153940))

- `URP`: 修复了重新加载场景会导致某些 `Blitter` 函数停止工作的错误。
    (UUM-153092)

- `URP`: 修复了在半精度平台（移动端）上，盒形投影反射探针上出现接缝的错误。
    ([UUM-141981](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-141981))

- `URP`: 修复了 RenderTexture。Create 失败的问题。
    ([UUM-91313](https://issuetracker.unity3d.com/issues/android-vulkan-error-rendertexture-dot-create-failed-format-unsupported-for-random-writes-r16-sfloat-45-dot-logged-when-during-launch-on-an-project-with-urp-2d-renderer))

- `URP`: 修复了因 uv4 输入语义差异导致的 ShaderGraph 编译失败问题。
    ([UUM-143884](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-143884))

- `URP`: 修复了在“玩家设置”中启用“禁用深度和模板缓冲区”后，2D 渲染器仍在玩家中创建深度和模板缓冲区的问题。
    ([UUM-150232](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150232))

- `URP`: ScriptableRendererData.TryGetRendererFeature 会抛出 NullReferenceException 异常。
    ([UUM-150772](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150772))

- `VFX Graph`: 修复了在使用 `MeshToSDFBaker` 处理特定体素数量时发生的越界访问问题。
    ([UUM-151674](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151674))

- `Web`: 修复了内存分析器中使用的 WASM_SIZE 和 wasmFileSize 相关问题。
    (UUM-149075)

- `Web`: 修复了当输出资源大小超过 2 GB 时的 Web 平台构建问题，以及输出资源大小超过 4 GB 时（不支持）的构建错误信息。
    ([UUM-112909](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-112909))




## 6000.0.85f2 版本中的包变更