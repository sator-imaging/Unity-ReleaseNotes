# Unity 6000.3.27f2 LTS
发布于 2026年10月30日 星期五 16:57:42 GMT  
https://unity.com/releases/editor/whats-new/6000.3.27f2

# 6000.3.27f2 中的已知问题

- `Android`: 当启用“在后台运行”和“预测性返回支持”时，从后台返回后，使用返回手势或按钮会关闭应用
    ([UUM-159613](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-159613))

- `音频制作`: 当 USB 音频输出设备断开并重新连接后，主线程恢复运行时会导致崩溃并产生多个堆栈跟踪
    ([UUM-158166](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158166))

- `编辑器安装程序`: [macOS] 播放器库使用自定义权限进行了代码签名
    ([UUM-156884](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156884))

- `原生编辑器应用程序生命周期`: [WinEditor] 当以高轮询率移动鼠标光标时，播放模式的帧率会显著下降
    ([UUM-142550](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-142550))

- `脚本构建时`: 当有多个 bee_backend 实例同时运行时，调用 mono_log_write_logfile 会导致崩溃
    ([UUM-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))

- `着色器系统`: 使用 SceneManager.LoadSceneAsync 反复切换场景时，玩家会永久停止响应
    ([UUM-156125](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156125))

- `SRP Foundation`: 物理旋转设备时，Logcat 和控制台会记录与 RenderPass 相关的 Android 错误
    ([UUM-157974](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-157974))



# 6000.3.27f2 版本说明

## 改进

- `资源导入`: 通过将捆绑的 Autodesk FBX SDK 更新至 2020.3.11 版本，提升了模型导入的安全性，修复了 FBX 文件解析中的两个缓冲区溢出漏洞。
    (UUM-155199)



## API 变更

- `Graphics`: 新增：添加了 Graphics.disableDepthAndStencilBuffers，这是一个只读属性，用于返回“播放器设置”中是否启用了“禁用深度和模板缓冲区”选项。



## 变更

- `Physics 2D`: "PhysicsComposer.AddLayer"、"PhysicsComposer.ToPolygons"、"CircleGeometry.ToPolygons" 和 "CapsuleGeometry.ToPolygons" 现会在未提供几何体、顶点数少于三个或 "curveStride" 无效时，记录标准验证警告，而非抛出 "ArgumentOutOfRangeException" 异常。
    ([UUM-156367](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156367))



## 修复

- `2D`: 修复在 2D 渲染器中使用叠加摄像机时出现的 ArgumentException 异常。
    ([UUM-148111](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-148111))

- `2D`: 修复了渲染通道请求时中间纹理未创建的问题
    ([UUM-145892](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-145892))

- `2D`: 修复了 URP 2D 编辑器专属图标被包含在玩家构建版本中的问题。
    (UUM-144935)

- `2D`: 修复了在游戏对象上切换启用状态时，LineRenderer 无法正确初始化的问题。
    ([UUM-147747](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147747))

- `Android`: 修复了在 UaaL 模式下，卸载后立即重新启动 GameActivity 时发生的卡死问题。
    (UUM-149857)

- `Animation`: 修复了在调用 AnimationUtility.SetAdditiveReferencePose 时，若 clip 或 referenceClip 为 null 导致的崩溃问题。
    ([UUM-150816](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150816))

- `资源管道`: 修复了启动时，若目录监听未收到关于文件更改的预期通知，导致程序卡死的问题。
    ([UUM-149019](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149019))

- `音频`: 修复了 macOS 上当系统正在使用麦克风时，音频播放会变慢的 bug
    ([UUM-149880](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149880))

- `Audio`: 修复了在播放模式下，当 AudioSource 的音频片段在 Unity Audio 被关闭后又重新开启期间加载时，退出播放模式时记录的断言 \(m_ModifiedClips.empty\(\)\) 错误。
    ([UUM-148749](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-148749))

- `Core`: 修复了在从 `EnabledWithStackTrace` 切换为 `Enabled` 后，首次域重新加载时，内存泄漏检测报告了错误的泄漏问题。
    ([UUM-108870](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-108870))

- `DX12`: 修复了在 Windows 系统上使用 Direct3D12 图形 API 时，因释放 GPU 缓冲区时的“释放后使用”问题导致的随机崩溃。
    ([UUM-150682](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150682))

- `编辑器`: 修复了卸载 AssetBundles 或 Entities 内容存档时 TMP_FontAsset 内存泄漏的问题
    (UUM-145538)

- `编辑器`: 修复了仅在 Linux 系统上出现的编辑器崩溃问题，该问题由域重新加载期间重建菜单项时的再入性问题引起。
    (UUM-149839)

- `编辑器`: 修复了当打开包含未保存更改的窗口时，尝试切换到已保存的编辑器布局可能导致无法取消布局更改的错误。
    ([UUM-150448](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150448))

- `编辑器`: 修复了 UITK 中“标准文本”的并发访问问题
    ([UUM-151887](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151887))

- `编辑器`: 修复了在“高级文本”中同一字符串内使用多个脚本的问题。
    ([UUM-150208](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150208))

- `GI`: 添加到光线追踪加速结构中的地形不再泄漏网格及其 GPU 缓冲区。
    (UUM-151903)

- `Graphics`: 修复了在 Metal 环境下，当计算着色器请求的线程组规模超过图形管道支持范围时可能导致的 GPU 卡死问题（例如，某些 Intel GPU 上的“高质量线条渲染”）。
    (UUM-147457)

- `Graphics`: 修复了编辑器在 Metal 上渲染单通道 XR 至无内存纹理数组时，记录的“Metal：无内存纹理需要 2D 纹理”断言错误。
    (UUM-154442)

- `Graphics`: 修复了在启用 Graphics 作业时，Graphics.RenderPrimitives 和 Graphics.DrawProcedural 与 MeshTopology.Quads 配合使用时发生的崩溃问题。
    ([UUM-141117](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-141117))

- `HDRP`: 修复了在启用 MSAA 和云层时，几何体在天空背景下周围出现暗色轮廓的问题。
    ([UUM-150911](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150911))

- `IL2CPP`: 修复了 `Thread.VolatileWrite(ref object, object)` 中缺失的 GC 写屏障问题。
    (UUM-155582)

- `IL2CPP`: 修复了 System.IO.Compression.BrotliStream 和 BrotliDecoder 中存在的 Brotli 解码器安全漏洞 \(CVE-2026-111497\)，解码不受信任的数据可能导致远程代码执行。

- `IL2CPP`: 修复了垃圾回收器可能在线程对象退出后仍保留其内存的问题
    ([UUM-149541](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149541))

- `IL2CPP`: 修复了引用结构体类型中静态字段和 ThreadStatic 字段缺少增量 GC 写屏障的问题。
    ([UUM-153622](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-153622))

- `输入系统`: 此更新修复了 Windows 的 Xbox 游戏栏以及 macOS 叠加层（Spotlight 等）的问题。 在 Windows 上，Steam/Discord/NVIDIA 叠加层仍可正常工作。
    ([UUM-150045](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150045))

- `iOS`: 修复了在 Unity 初始化之前调用 `application:openURL` 或 `application:continueUserActivity` 时导致的崩溃问题。
    ([UUM-151801](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151801))

- `内核`: 修复了由 32 位整数溢出导致的 NativeSlice 崩溃问题。
    (UUM-154594)

- `macOS`: 修复了在较新版本的 macOS 上导入 X.509 证书时可能发生的崩溃问题。
    (UUM-154511)

- `macOS`: 修复了在 macOS 上，当编辑器的某个窗口失去焦点时，编辑器在批处理模式和自动化测试运行中变慢的问题。

- `Mono`: 修复了 System.IO.Compression.BrotliStream 和 BrotliDecoder 所使用的 Brotli 解码器中的一项安全漏洞 \(CVE-2026-111497\)，该漏洞可能导致解码不受信任的数据时发生远程代码执行。

- `Mono`: 修复了使用默认 GCHandle 时发生的崩溃问题
    ([UUM-153835](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-153835))

- `多人游戏`: 修复了在使用 Vulkan 图形 API 时，包含额外编辑器实例的“游戏模式”场景会一直处于“部署中”状态的问题。
    ([UUM-154645](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-154645))

- `网络`: 拒绝使用已泄露的 eMudhra 证书连接至服务器的 TLS 连接。
    (UUM-158231)

- `网络`: Unity Transport：修复了在创建 TLS/DTLS 会话时会发生的小量内存泄漏问题。
    ([UUM-151755](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151755))

- `包管理器`: 通过将包管理器使用的 Node.js 运行时更新至 v24.22.1，修复了一个可能导致远程代码执行的安全漏洞 \(CVE-2026-111497\)。

- `物理引擎`: 修复了 Rigidbody.mass 接受 NaN 值的问题，该问题会导致刚体穿过所有碰撞体。
    ([UUM-154143](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-154143))

- `Physics 2D`: 为多个 Physics Core 2D 方法添加了缺失的公共参数验证。
    ([UUM-156367](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156367))

- `Physics 2D`: 修复了在设置“PhysicsChain.friction”、“PhysicsChain.bounciness”、“PhysicsChain.frictionMixing”或“PhysicsChain.bouncinessMixing”后可能发生的崩溃或内存损坏问题。

- `Profiler`: 修复了在加载操作进行中捕获内存分析器快照时，PreloadManager 出现的死锁问题
    (UUM-143493)

- `Shadergraph`: 修复了在同时使用关键字节点和虚拟纹理采样的图形中出现的渲染错误。
    (UUM-139845)

- `源代码构建`: 修复了在使用土耳其地区格式的机器上编辑器源代码构建失败的问题。
    (UUM-154501)

- `文本`: 修复了当 TextMesh 或旧版 UI 文本字符串以未终止的四边形标签参数结尾时发生的越界内存读取问题。
    (UUM-153129)

- `文本`: 修复了当 TextMesh 或旧版 UI 文本字符串以未结束的富文本标签结尾时发生的越界内存读取问题。
    (UUM-153128)

- `TextMeshPro`: 修复了“当输入字段中使用变体字符时，TextMeshPro 输入字段在首次按退格键时无法删除字符”的错误
    ([UUM-140383](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-140383))

- `TextMeshPro`: 修复了当包含“内容大小适配器”的 TextMeshPro 文本在窄宽度下出现空格前带连字符时，编辑器会卡死的问题。
    ([UUM-152921](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-152921))

- `uGUI`: 修复了当 RectMask2D 的柔化值设为零时，会使被裁剪内容的边缘出现柔化现象的问题
    ([UUM-150815](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150815))

- `UI Toolkit`: 修复了当面板缩放比例不是整数时，应用了滤镜（如投影）的元素中文字和内容出现模糊的问题。
    ([UUM-155009](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-155009))

- `UI Toolkit`: 修复了在仅支持水平滚动的 ScrollView 和列表视图中，触控板水平滚动几乎无法移动或方向错误的问题。
    (UUM-152573)

- `UI Toolkit`: 修复了在 macOS 上运行的 Web 构建中，多列列表和树形视图需要使用 Ctrl+点击而非 Cmd+点击才能按多列排序的问题。

- `UI Toolkit`: 修复了在 macOS 上运行的 Web 构建中，指针、鼠标、键盘和导航事件的操作键被设置为 Ctrl 而非 Cmd 的问题。
    ([UUM-153940](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-153940))

- `UI Toolkit`: 修复了在重新创建 UI Toolkit 调试器窗口后（例如将停靠窗口最大化并恢复，或在调试器上切换 UI Toolkit 实时刷新功能时），动态图集查看器无法显示图集的问题。
    ([UUM-150663](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150663))

- `UI Toolkit`: 修复了当 USS 的 transition-timing-function 声明使用非关键字值（例如 5px）时，编辑器和播放器会卡死的问题。
    ([UUM-155159](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-155159))

- `UI 工具包`: 修复了在切换具有不同组件的预制体后，“选择 GameObject”窗口会无提示地忽略第二个检查器中选中的预制体的问题。
    ([UUM-154149](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-154149))

- `URP`: 修复了在启用兼容性模式且叠加摄像机使用的渲染器与其基础摄像机不同时，DX11 环境下出现的“CommandBuffer：执行过程中未找到临时渲染纹理”警告。
    ([UUM-117369](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-117369))

- `URP`: 修复了在“玩家设置”中启用“禁用深度和模板缓冲区”后，2D 渲染器仍在玩家中创建深度和模板缓冲区的问题。
    ([UUM-150232](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150232))

- `Web`: 修复了内存分析器中使用的 WASM_SIZE 和 wasmFileSize
    (UUM-149075)

- `WebGL`: WebGPU：优化统一缓冲区和动态顶点缓冲区的内存使用
    (UUM-152972)




## 6000.3.27f2 版本中的包变更