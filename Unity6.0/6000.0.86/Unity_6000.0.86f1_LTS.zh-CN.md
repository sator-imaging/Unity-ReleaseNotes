# Unity 6000.0.86f1 LTS
发布于 2026年11月12日 星期四 09:43:45 GMT  
https://unity.com/releases/editor/whats-new/6000.0.86f1

# 6000.0.86f1 中的已知问题

- `Android`: 当启用“在后台运行”和 “预测性返回支持”均已启用时，从后台返回后，后退手势/按钮会关闭应用
    ([UUM-159613](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-159613))

- `编辑器安装程序`: [macOS] 播放器库使用自定义权限进行了代码签名
    ([UUM-156884](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156884))

- `着色器系统`: 当使用 SceneManager.LoadSceneAsync 反复切换场景时，播放器会永久停止响应
    ([UUM-156125](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156125))

- `视频`: 打开包含特定 .mp4 视频文件的项目时，调用 `BitmapDataToImageReference` 会导致崩溃
    ([UUM-160889](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-160889))



# 6000.0.86f1 版本说明

## 改进

- `资源导入`: 通过将捆绑的 Autodesk FBX SDK 更新至 2020.3.11 版本，提升了模型导入的安全性，修复了 FBX 文件解析中的两个缓冲区溢出漏洞。
    (UUM-155199)

- `许可证`: 将许可证客户端更新至 v1.19.0，启动速度更快。



## API 变更

- `iOS`: 新增：添加了 iPhone 18 Pro、iPhone 18 Pro Max 和 iPhone Duo 设备代数枚举及屏幕裁剪区域。



## 修复

- `2D`: 修复了在“播放”模式下撤销或重做“阴影投射器”2D形状编辑时出现的“ShadowCasterPath 没有脚本资源”警告。
    ([UUM-152935](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-152935))

- `2D`: 修复了当通过脚本创建的 2D 光源在未指定形状路径的情况下被设置为“自由形态”时引发的 NullReferenceException 异常。
    ([UUM-154810](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-154810))

- `2D`: 修复了在运行时移除 `Tilemap Collider 2D` 的贴图后，`Shadow Caster 2D` 仍保留旧阴影的问题。
    ([UUM-149925](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149925))

- `2D`: 修复了当某个“线渲染器”或“轨迹渲染器”的“遮罩交互”设置为“无”时，若另一个使用相同材质的“线渲染器”或“轨迹渲染器”启用了“遮罩交互”，前者会被“精灵遮罩”裁剪的问题。
    ([UUM-158602](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158602))

- `2D`: 修复了在 Unity 6.0 或 6.3 中保存的项目于新版本中打开时，2D 点光源会丢失其“cookie”贴图的问题。
    ([UUM-156931](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156931))

- `2D`: 修复了当 2D 投影器使用 2D 碰撞体（例如 2D 贴图地图碰撞体）作为投影源时，其投射的阴影在“场景”和“游戏”视图中闪烁的问题。
    ([UUM-147033](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147033))

- `2D`: 修复了在某些 OpenGL ES 设备上，当 2D 渲染器的“深度/模板缓冲区”设置被禁用时，精灵和 UI 无法渲染的问题。
    ([UUM-159093](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-159093))

- `2D`: 修复了 URP 2D 编辑器专属图标被包含在播放器构建中的问题。
    (UUM-144935)

- `Android`: 将针对 Android 优化帧率控制（\(Swappy\)）的崩溃修复方案回溯移植。
    (UUM-153366)

- `Android`: 修复了 OpenGL 中一个问题：Unity 的渲染线程会在一个帧内多次连接/断开与 JVM 的连接，导致不必要的内存分配。
    (UUM-155309)

- `Android`: 修复了 Android 原生库中 GNU_RELRO 段未对齐到 16 KB 的问题。在下次 NDK 更新之前，`libc++_shared.so` 将保持未对齐状态。
    ([UUM-156603](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156603))

- `Android`: 修复了光标被锁定时，鼠标移动会产生滚动值的问题。
    ([UUM-156720](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156720))

- `Android`: 修复了在应用重新获得焦点或另一款应用释放摄像头后（例如在分屏模式下），WebCamTexture 需要数秒才能恢复的问题。
    (UUM-155066)

- `Android`: 将捆绑的 Android SDK 命令行工具更新至 21.0 版本，因此使用其 avdmanager 创建的 Android 17（API 37.0）模拟器可正常启动。
    (UUM-157110)

- `Animation`: 当调用 `AnimationUtility.SetAdditiveReferencePose` 时，若 clip 或 referenceClip 为 null，会导致崩溃。
    ([UUM-150816](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150816))

- `资源包`: 修复了在使用 Addressables 或可脚本化构建管道时，未更改内容的资源包内容哈希值在不同构建版本间发生变化，导致玩家重新下载未修改的资源包的问题。受影响的资源包在升级后的首次构建中会获得新的哈希值。
    ([UUM-148841](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-148841))

- `资源导入`: 修复了在 Linux 编辑器中导入 crunch 压缩纹理时，编辑器有时会异常退出，日志中显示“crn_threading_pthreads.cpp\(194\): 失败：信号量：sem_wait\(\) 或 sem_timedwait\(\) 失败"。Crunch 压缩器此前将中断的等待视为致命错误；现已改为重试等待。
    ([UUM-150055](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150055))

- `资源管道`: 资源管道： 修复了启动时，当目录监听未收到关于文件更改的预期通知而导致程序卡死的问题。
    ([UUM-149019](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149019))

- `音频`: 修复了在播放模式下，当 AudioSource 的片段在播放模式期间 Unity Audio 被关闭后又重新开启时加载，且在退出播放模式时记录的断言 \(m_ModifiedClips.empty\(\)\)。
    ([UUM-148749](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-148749))

- `构建系统`: 在调用 dotnet 时，将 MSBUILDDEBUGPATH 添加到其他方法中。

- `构建系统`: Bee_backend 的过期输出清理功能不应无限期地重新检查同一文件。
    (UUM-158568)

- `构建系统`: 当之前的 bee_backend 仍在运行时，编辑器不会卡死。
    ([UUM-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))

- `DX12`: 修复了在使用 AddComputePass 并设置 EnableAsyncCompute\(true\) 时，D3D12SwapChain::Present 引发的崩溃问题。
    ([UUM-140183](https://issuetracker.unity3d.com/issues/rendergraph-d3d12-crash-on-d3d12swapchain-present-when-using-addcomputepass-with-enableasynccompute-true-and-usetexture))

- `DX12`: 修复了当启用图形任务时，IUnityGraphicsD3D12::GetNextFrameFenceValue\(\) 返回的栅栏值可能在原生插件记录到 Unity 当前命令列表中的命令完成之前就已完成的 bug。
    (UUM-156768)

- `编辑器`: 修复了在打开包含未保存更改的窗口时，尝试切换到已保存的编辑器布局可能会导致无法取消布局更改的错误。
    ([UUM-150448](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150448))

- `Editor`: 修复了 `InstantiateAsync` 不会考虑父级变换缩放比例的错误，而 `Instantiate` 则会考虑。
    ([UUM-154591](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-154591))

- `编辑器`: 修复了当脚本使用 UnityEngine.Device.SystemInfo.processorModel、processorManufacturer 或 supportsMachineLearning 时，玩家构建会因错误 CS0117 而失败。
    ([UUM-154729](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-154729))

- `编辑器`: 修复了在启用“自动保存”功能后，选中名称字段时预制体字段仅部分保存的问题。
    ([UUM-157667](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-157667))

- `编辑器`: 修复了 TrueTypeFontImporter 帮助按钮的链接。
    ([UUM-144647](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-144647))

- `编辑器`: 将 Windows 编辑器中随附的 VCRedist 更新至 14.51.36247 版本。
    (UUM-156578)

- `编辑器`: URP：在开始构建资源包之前，先保存 URP 资源。
    ([UUM-153206](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-153206))

- `编辑器`: 启用图形任务时，编辑器现在会渲染那些在帧内编译了着色器变体的渲染器。此前因缺少着色器而显示为空白的资源预览和一次性渲染，现在应能通过 SRP Batcher 备用路径按预期渲染。
    (UUM-147205)

- `编辑器`: \[Android\] 在 Unity 6.0 上安装 APK 时，若设备在安装过程中断开连接，将显示错误提示，告知用户原因。
    (UUM-151550)

- `引擎诊断`: 在远程配置之前捕获的崩溃、异常和 ANR 报告现在会保留其关键属性，包括发生这些问题的会话信息。
    (UUM-159169)

- `引擎诊断`: 修复了在应用引擎诊断配置时，若从工作线程记录崩溃报告可能导致的崩溃问题。
    (UUM-158113)

- `GI`: 修复了一个错误：在烘焙灯光时，如果仅修改了 URP 专有的设置，反射探针有时不会被重新烘焙。
    ([UUM-133949](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-133949))

- `GI`: 修复了在 AMD GPU 上使用 Vulkan 进行烘焙时，自适应探针体积会将探针放置得仿佛场景中没有几何体一样的问题。
    ([UUM-137732](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-137732))

- `GI`: 修复了 APV 产生的斑点/白点问题。
    ([UUM-133626](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-133626))

- `Graphics`: 修复了在通用 Windows 平台上使用 DirectX 12 并采用拆分图形任务的播放器中，退出时发生的崩溃问题。
    (UUM-152563)

- `图形`: 修复了编辑器在 Metal 上渲染单通道 XR 至无内存纹理数组时记录的“Metal：无内存纹理需要 2D 纹理”断言错误。
    (UUM-154442)

- `图形`: 修复了使用 2D 精灵材质的线条渲染器或轨迹渲染器在动画窗口中关闭“预览”功能后，或在调用 `Renderer.SetPropertyBlock` 后变为不可见的问题。
    ([UUM-156620](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156620))

- `Graphics`: 修复了在使用 Vulkan 和 GraphicsJobs 时 Mip 流式传输的问题。
    (UUM-137032)

- `Graphics`: 修复了在 CPU 上解压 BC 压缩纹理时发生的内存损坏问题，例如当 GPU 不支持该格式， 且 Mip 级别小于 4x4 或其尺寸不是 4 的倍数时，会在 CPU 上解压 BC 压缩纹理时导致内存损坏。
    (UUM-154799)

- `Graphics`: 在 <br> 条件下，`SystemInfo.supportsParallelPSOCreation` 现可正确返回 `true`
    Android 设备上，当单核支持并行 PSO 创建时，`SystemInfo.supportsParallelPSOCreation` 现能正确返回 `true`。
    (UUM-153032)

- `HDRP`: 修复了某些枚举材质属性中被添加“默认”值的问题。
    ([UUM-134256](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-134256))

- `HDRP`: 修复了在启用 MSAA 和云层时，几何体在天空背景下出现深色轮廓线的问题。
    ([UUM-150911](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150911))

- `输入系统`: 此更新修复了 Windows 的 Xbox 游戏栏以及 macOS 叠加层（如 Spotlight 等）的问题。在 Windows 系统上，Steam/Discord/NVIDIA 叠加层仍可照常使用。
    ([UUM-150045](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150045))

- `iOS`: 修复了在 Unity 初始化之前调用 `application:openURL` 或 `application:continueUserActivity` 时发生的崩溃问题。
    ([UUM-151801](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151801))

- `内核`: 修复了由 32 位整数溢出导致的 NativeSlice 崩溃问题。
    (UUM-154594)

- `License`: 修复了当无法连接到 Unity 授权客户端时，编辑器在未获得授权的情况下仍会继续运行，并在批处理模式下以代码 0 退出的问题。
    ([UUM-151817](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151817))

- `许可证`: 修复了当两个相同版本的编辑器所需的许可证客户端版本不兼容时，许可证错误对话框在“重试”和“关闭”之间无限循环的问题。
    (UUM-153121)

- `Linux`: 修复了在 Linux 上使用 -nographics 参数但未使用 -batchmode 参数启动编辑器时发生的崩溃问题；现在编辑器会报告无效参数并以代码 1 退出。
    ([UUM-154576](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-154576))

- `macOS`: 当 Screen.sleepTimeout 设置为 SleepTimeout.SystemSetting 且系统设置并非“永不”时，允许系统进入睡眠状态。
    ([UUM-150222](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150222))

- `macOS`: 修复了在 macOS 上，当编辑器的某个窗口失去焦点时，编辑器在批处理模式和自动化测试运行中变慢的问题。

- `网络`: Unity 传输：修复了创建 TLS/DTLS 会话时会发生的小量内存泄漏问题。
    ([UUM-151755](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151755))

- `脚本`: 修复了在帧更新期间取消 `Awaitable.NextFrameAsync` 或 `Awaitable.EndOfFrameAsync` 待处理操作时，可能会导致无关的 `Awaitable` 提前完成并返回默认结果的问题。
    ([UUM-156357](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156357))

- `着色器`: 修复了在计算着色器为 null 时调用 `RenderingCommandBuffer.SetKeyword` 会导致程序崩溃的问题。
    ([UUM-158327](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158327))

- `着色器`: 修复了在对空或已销毁的材质上执行带有 SetKeyword 的 RenderingCommandBuffer 时发生的崩溃问题。
    ([UUM-157105](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-157105))

- `着色器`: 修复了在后台编译着色器变体时读取着色器消息可能导致编辑器崩溃的问题。
    (UUM-154510)

- `着色器`: 修复了在画布上渲染未编译或损坏的着色器时，编辑器发生崩溃的问题。
    ([UUM-153265](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-153265))

- `着色器`: 修复了当提供的值超出有效枚举范围时，`Material.GetPropertyNames` 会导致崩溃的问题。
    ([UUM-157945](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-157945))

- `SRP Core`: 修复了在较旧的 iOS 设备（Apple GPU 家族 3 及以下）上，一旦原生渲染通道被判定超过了单瓦片像素存储限制，渲染通道便无法合并的问题；此前系统会将整个帧序列化为每个渲染通道对应一个原生渲染通道。
    ([UUM-148865](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-148865))

- `SRP Core`: 修复了渲染图在经过 8 个光栅化渲染通道后，即使原生子通道数量少于 8 个，仍会关闭原生渲染通道的问题，这导致后续通道（如 URP UI 叠加层）需要从内存中重新加载其附件。
    ([UUM-158401](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158401))

- `UI 工具包`: 修复了当某个关键帧的值非常大时，AnimationCurve 的 UXML 属性在保存后会丢失其值的问题。
    ([UUM-156823](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156823))

- `UI 工具包`: 修复了当文本使用具有较小图集填充且轮廓宽度为零或负值的字体资源时，字母周围出现的视觉瑕疵。
    ([UUM-146020](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146020))

- `UI 工具包`: 修复了在重新创建 UI 工具包调试器窗口后（例如将停靠窗口最大化并恢复，或在调试器上切换 UI 工具包实时刷新功能时），动态图集查看器无法显示图集的问题。
    ([UUM-150663](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150663))

- `URP`: 修复了在启用兼容性模式且叠加摄像机使用的渲染器与其基础摄像机不同时，DX11 环境下出现的“CommandBuffer：执行过程中未找到临时渲染纹理”警告。
    ([UUM-117369](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-117369))

- `URP`: 修复了某些枚举材质属性中被添加“Default”值的问题。
    ([UUM-134256](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-134256))

- `URP`: 修复了当启用延迟渲染、禁用附加光照阴影但启用阴影遮罩时，URP 会尝试使用精简变体的错误。
    ([UUM-153600](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-153600))

- `URP`: 修复了一个问题：当与禁用了深度/模板缓冲区的 2D 渲染器配合使用时，URP RenderGraph 样本中的“渲染器列表”和“剔除”样本会在每帧记录错误。
    ([UUM-157948](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-157948))

- `URP`: 修复了以下问题：如果同一编辑器会话中之前曾导入过启用了“支持 LOD 交叉淡入淡出”功能的着色器图，则后续导入的着色器图生成的着色器代码及资源包哈希值会发生变化。
    (UUM-155529)

- `XR`: 修复了在子系统被销毁后调用 `SubsystemWithProvider.Start` 时，该方法未抛出 `ArgumentNullException` 的问题，这会导致已销毁的提供程序被重新启动。
    ([UUM-151411](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151411))




## 6000.0.86f1 版本中的包变更

## 已更新的包

- `com.unity.2d.animation`: 从 [10.2.3](https://docs.unity3d.com/Packages/com.unity.2d.animation@10.2//changelog/CHANGELOG.html) 更新至 [10.2.4](https://docs.unity3d.com/Packages/com.unity.2d.animation@10.2//changelog/CHANGELOG.html)

- `com.unity.2d.psdimporter`: 从 [9.1.2](https://docs.unity3d.com/Packages/com.unity.2d.psdimporter@9.1//changelog/CHANGELOG.html) 更新至 [9.1.3](https://docs.unity3d.com/Packages/com.unity.2d.psdimporter@9.1//changelog/CHANGELOG.html)

- `com.unity.2d.tilemap.extras`: 从 [4.1.1](https://docs.unity3d.com/Packages/com.unity.2d.tilemap.extras@4.1//changelog/CHANGELOG.html) 更新至 [4.1.2](https://docs.unity3d.com/Packages/com.unity.2d.tilemap.extras@4.1//changelog/CHANGELOG.html)

- `com.unity.burst`: 从 [1.8.30](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html) 更新至 [1.8.31](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html)

- `com.unity.collab-proxy`: [2.13.6](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.13//changelog/CHANGELOG.html) 升级至 [2.14.0](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.14//changelog/CHANGELOG.html)

- `com.unity.performance.profile-analyzer`: 从 [1.4.0](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.4//changelog/CHANGELOG.html) 更新至 [1.4.2](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.4//changelog/CHANGELOG.html)

- `com.unity.services.authentication`: 从 [3.8.0](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.8//changelog/CHANGELOG.html) 更新至 [3.8.1](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.8//changelog/CHANGELOG.html)

- `com.unity.services.cloudsave`: 从 [3.4.0](https://docs.unity3d.com/Packages/com.unity.services.cloudsave@3.4//changelog/CHANGELOG.html) 升级至 [3.4.2](https://docs.unity3d.com/Packages/com.unity.services.cloudsave@3.4//changelog/CHANGELOG.html)

- `com.unity.services.wire`: 从 [1.6.0](https://docs.unity3d.com/Packages/com.unity.services.wire@1.6//changelog/CHANGELOG.html) 更新至 [1.6.2](https://docs.unity3d.com/Packages/com.unity.services.wire@1.6//changelog/CHANGELOG.html)

- `com.unity.test-framework.performance`: 从 [3.5.0](https://docs.unity3d.com/Packages/com.unity.test-framework.performance@3.5//changelog/CHANGELOG.html) 更新为 [3.7.0](https://docs.unity3d.com/Packages/com.unity.test-framework.performance@3.7//changelog/CHANGELOG.html)

- `com.unity.xr.oculus`: 从 [4.5.4](https://docs.unity3d.com/Packages/com.unity.xr.oculus@4.5//changelog/CHANGELOG.html) 更新至 [4.5.6](https://docs.unity3d.com/Packages/com.unity.xr.oculus@4.5//changelog/CHANGELOG.html)

- `com.unity.ai.navigation`: 从 [2.0.15](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html) 更新至 [2.0.16](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html)

- `com.unity.asset-manager-for-unity`: 从 [1.12.0](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.12//changelog/CHANGELOG.html) 升级至 [1.12.1](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.12//changelog/CHANGELOG.html)

- `com.unity.cloud.draco`: 从 [5.5.0](https://docs.unity3d.com/Packages/com.unity.cloud.draco@5.5//changelog/CHANGELOG.html) 更新至 [5.6.0](https://docs.unity3d.com/Packages/com.unity.cloud.draco@5.6//changelog/CHANGELOG.html)

- `com.unity.cloud.ktx`: 从 [3.7.1](https://docs.unity3d.com/Packages/com.unity.cloud.ktx@3.7//changelog/CHANGELOG.html) 升级至 [3.8.0](https://docs.unity3d.com/Packages/com.unity.cloud.ktx@3.8//changelog/CHANGELOG.html)

- `com.unity.xr.compositionlayers`: 从 [2.6.0](https://docs.unity3d.com/Packages/com.unity.xr.compositionlayers@2.6//changelog/CHANGELOG.html) 更新至 [2.6.1](https://docs.unity3d.com/Packages/com.unity.xr.compositionlayers@2.6//changelog/CHANGELOG.html)

**新增包**

- [com.unity.steamworks-api@1.0.0](https://docs.unity3d.com/Packages/com.unity.steamworks-api@1.0//changelog/CHANGELOG.html)