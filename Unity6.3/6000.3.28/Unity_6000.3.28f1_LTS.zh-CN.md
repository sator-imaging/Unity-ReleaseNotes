# Unity 6000.3.28f1 LTS
发布于 2026年11月3日 星期二 16:15:25 GMT  
https://unity.com/releases/editor/whats-new/6000.3.28f1

# 6000.3.28f1 中的已知问题

- `Android`: 当启用“在后台运行”和“预测性返回支持”时，从后台返回后，使用返回手势或按钮会关闭应用
    ([UUM-159613](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-159613))

- `音频制作`: 当 USB 音频输出设备断开并重新连接后，主线程恢复运行时会导致应用崩溃并产生多个堆栈跟踪
    ([UUM-158166](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158166))

- `编辑器安装程序`: [macOS] 播放器库使用自定义权限进行了代码签名
    ([UUM-156884](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156884))

- `原生编辑器应用程序生命周期`: [WinEditor] 当以高轮询率移动鼠标光标时，播放模式的帧率会显著下降
    ([UUM-142550](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-142550))

- `着色器系统`: 使用 SceneManager.LoadSceneAsync 反复切换场景时，播放器会永久停止响应
    ([UUM-156125](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156125))

- `SRP Foundation`: 物理旋转设备时，Logcat 和控制台会记录与 RenderPass 相关的 Android 错误
    ([UUM-157974](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-157974))



# 6000.3.28f1 版本说明

## 改进

- `License`: 将授权客户端更新至 v1.19.0，启动速度更快。



## API 变更

- `iOS`: 新增：添加了 iPhone 18 Pro、iPhone 18 Pro Max 和 iPhone Duo 的设备代数枚举及屏幕开孔。



## 修复

- `2D`: 修复了在“播放”模式下撤销或重做 Shadow Caster 2D 形状编辑时出现的“ShadowCasterPath 没有脚本资源”警告。
    ([UUM-152935](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-152935))

- `2D`: 修复了当通过脚本创建的 2D 光源在未指定形状路径的情况下被设置为“自由形态”时引发的 NullReferenceException 异常。
    ([UUM-154810](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-154810))

- `2D`: 修复了在 Unity 6.0 或 6.3 中保存的项目于新版本中打开时，点光源 2D 会丢失其 cookie 贴图的问题。
    ([UUM-156931](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156931))

- `2D`: 修复了当 2D 投影器使用 2D 碰撞体（例如 2D 贴图地图碰撞体）作为投影源时，其投射的阴影在“场景”和“游戏”视图中闪烁的问题。
    ([UUM-147033](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147033))

- `Android`: 回溯移植了针对 Android 优化帧率调节（Swappy）的崩溃修复。
    (UUM-153366)

- `Android`: 修复了在调用 `AnimatorController.CreateNewStateMachineBehaviour` 时传入 `null` 的 `MonoScript` 导致的崩溃。现在该情况会抛出 `ArgumentNullException` 异常。
    ([UUM-150813](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150813))

- `Android`: 修复了 OpenGL 中的一个问题，此前 Unity 的渲染线程会在一个帧内多次连接/断开与 JVM 的连接，导致不必要的内存分配。
    (UUM-155309)

- `Android`: 修复了 Android 本机库中 GNU_RELRO 段未对齐到 16 KB 的问题。在下次 NDK 更新之前，`libc++_shared.so` 将保持未对齐状态。
    ([UUM-156603](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156603))

- `Android`: 修复了在应用重新获得焦点或另一款应用释放摄像头后（例如在分屏模式下），`WebCamTexture` 需要数秒才能恢复的问题。
    (UUM-155066)

- `Animation`: 修复了在传递超出范围的骨骼索引时，HumanTrait.GetParentBone 和 HumanTrait.RequiredBone 会引发崩溃的问题。现在，这些方法会抛出 ArgumentOutOfRangeException 异常。
    ([UUM-150938](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150938))

- `Animation`: 修复了在对无效或默认的 AnimationPlayableOutput 调用 AnimationPlayableOutput.SetSortingOrder 时发生的崩溃问题。现在该方法会抛出 NullReferenceException 异常。
    ([UUM-150941](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150941))

- `Animation`: 修复了向 `AnimationPlayableOutputExtensions.SetAnimationStreamSource` 提供默认或无效的 `AnimationPlayableOutput` 时会导致程序崩溃的问题。
    ([UUM-150939](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150939))

- `资源包 (Asset Bundles)`：修复了在使用 Addressables 或可脚本化构建管道 (Scriptable Build Pipeline) 时，未更改内容的资源包 (AssetBundle) 内容哈希值在不同构建版本间发生变化，导致玩家重新下载未修改的资源包的问题。受影响的资源包在升级后的首次构建中会生成新的哈希值。
    ([UUM-148841](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-148841))

- `资源导入`: 修复了内置模块（如 SVGImporter）提供的导入器默认预设，在项目重启后不再生效的问题。
    ([UUM-146265](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146265))

- `资源导入`: 修复了在 Linux 编辑器中导入 crunch 压缩纹理时，编辑器有时会异常退出，且日志中显示“crn_threading_pthreads.cpp\(194\): 失败：信号量：sem_wait\(\) 或 sem_timedwait\(\) 失败”的问题。 crunch 压缩器此前将中断的等待视为致命错误；现在会重试该等待操作。
    ([UUM-150055](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150055))

- `构建系统`: Bee_backend 的过期输出清除功能不应无限期地重新检查同一文件。
    (UUM-158568)

- `构建系统`: 当之前的 bee_backend 仍在运行时，不要导致编辑器卡死。
    ([UUM-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))

- `DX12`: 修复了在 DirectX 12 环境下，当单帧内大型纹理（例如大型动态字体图集）被多次更新时导致的崩溃问题。
    ([UUM-140070](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-140070))

- `DX12`: 修复了 IUnityGraphicsD3D12::GetNextFrameFenceValue\(\) 返回的栅栏值，该值可能在图形任务启用时，比本机插件记录到 Unity 当前命令列表中的命令更早完成。
    (UUM-156768)

- `DX12`: 当单次重绘渲染的场景具有极高的每帧绘制量时，编辑器不再因内存不足或 GPU 设备重置而崩溃。 当累积的上传临时内存超过 1 GiB 时，Direct3D 12 现会在帧内再次提交 GPU 任务；可通过 d3d12-scratch-flush-threshold 启动配置参数。首次执行帧内刷新时，编辑器或播放器日志会记录该参数的名称。
    (UUM-93272)

- `编辑器`: 修复了在 Mac 编辑器中执行“强制退出”操作时 `NativeWindowManager` 发生的崩溃问题。
    ([UUM-157869](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-157869))

- `编辑器`: 修复了 ATG 小节高度未受限制时导致的崩溃问题。
    ([UUM-155956](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-155956))

- `编辑器`: 修复了在相邻链接之间切换时悬停事件无法触发的的问题。
    (UUM-156714)

- `编辑器`: 修复了在 Android 构建配置文件的 Unity 渲染服务中，当 Android 模块未安装时，“安装模块”按钮会打开无效下载链接的问题。
    (UUM-154168)

- `编辑器`: 修复了 TrueTypeFontImporter 帮助按钮的链接。
    ([UUM-144647](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-144647))

- `编辑器`: 多人游戏：当“游戏模式场景”窗口以较大尺寸重新打开后，选中区域的高亮范围会超出列表分隔线。
    ([UUM-137539](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-137539))

- `编辑器`: Windows：修复了编辑器在 Windows 系统上以批处理模式运行时无法创建主窗口而导致的崩溃问题。
    ([UUM-153339](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-153339))

- `编辑器`: \[Android\] 在 Unity 6.3 上安装 APK 时，若设备在安装过程中断开连接，将显示错误提示告知用户原因。
    (UUM-151550)

- `GI`: 修复了在 AMD GPU 上使用 Vulkan 进行烘焙时，自适应探针体积（Adaptive Probe Volumes）会将探针放置得仿佛场景中没有几何体一样的问题。
    ([UUM-137732](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-137732))

- `GI`: 修复了 APV 产生的斑点/白点问题。
    ([UUM-133626](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-133626))

- `Graphics`: 确保在使用多显示器时后缓冲区的尺寸正确。
    (UUM-134688)

- `Graphics`: 修复了在通用 Windows 平台上使用 DirectX 12 并采用拆分图形任务的播放器中，退出时发生的崩溃问题。
    (UUM-152563)

- `Graphics`: 修复了使用 2D 精灵材质的线条渲染器或轨迹渲染器在动画窗口中关闭“预览”功能或调用 `Renderer.SetPropertyBlock。
    ([UUM-156620](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156620))

- `Graphics`: 修复了在触发资源导入时，若摄像机的目标缓冲区是通过 `Camera.SetTargetBuffers` 设置摄像机目标缓冲区时，`RenderTarget::SetActive` 引发的崩溃问题。
    ([UUM-148003](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-148003))

- `Graphics`: 修复了在某些渲染通道/子通道配置下，Mali GPU 上出现的 Vulkan 渲染瑕疵。
    ([UUM-147578](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147578))

- `Graphics`: 在<br>
    单核 Android 设备上，`SystemInfo.supportsParallelPSOCreation` 现可正确返回 `true`，从而启用并行 PSO 创建。
    (UUM-153032)

- `HDRP`: 修复了某些枚举材质属性中被添加了“默认”值的问题。
    ([UUM-134256](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-134256))

- `HDRP`: 修复了因默认质量级别设置为“高性能”导致 HD 模板在体积雾禁用状态下打开的问题。
    (UUM-149134)

- `License`: 修复了当两个相同版本的编辑器所需的许可客户端版本不兼容时，许可错误对话框在“重试”和“关闭”之间无限循环的问题。
    (UUM-153121)

- `Linux`: 修复了在 Linux 上未初始化视频子系统时（例如在 -nographics 批处理模式下或无显示器的情况下）运行程序导致的崩溃问题。
    ([UUM-156559](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156559))

- `Linux`: 修复了在 Linux 上使用 -nographics 参数但未使用 -batchmode 参数启动编辑器时发生的崩溃问题；现在编辑器会报告无效参数并以代码 1 退出。
    ([UUM-154576](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-154576))

- `macOS`: 当 Screen.sleepTimeout 设置为 SleepTimeout.SystemSetting 且系统设置并非“永不”时，允许系统进入睡眠状态。
    ([UUM-150222](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150222))

- `Mono`: 修复了与仅支持 TLS 1.3 的服务器建立 WebSocket 连接的问题。
    (UUM-158461)

- `Mono`: 当运行时统计信息被禁用时，通过跳过 JIT 阶段计时来降低 JIT 编译开销。
    (UUM-158476)

- `Physics`: 计算缩放后的球体与凸面网格碰撞体之间的穿透（ComputePenetration）时，现在将返回正确的结果。
    (UUM-139615)

- `Physics`: 修复了关节组件无法触发新连接的刚体组件重新评估其接触关系的问题。因此，“启用碰撞”等标志现在可以生效。
    ([UUM-156450](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156450))

- `2D 物理`: 修复了当“maxFraction”小于 1 时，“PhysicsAABB.CastRay”返回错误分数值的问题，以及“PhysicsAABB.center”和“PhysicsAABB.extents”警告中成员名称错误的问题。
    ([UUM-156920](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156920))

- `Physics 2D`: 修复了“PhysicsLayers”，确保“GetLayerMask”包含所有名称相同的图层，“GetLayerName”对未命名的图层返回空字符串，且当参数为 null 或超出范围时，抛出的异常会正确指明参数名称。
    ([UUM-156920](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156920))

- `Physics 2D`: 修复了“PhysicsMask”，使得包含第 31 层的“LayerMask”不再设置高 32 位， 对于空掩码，“AreBitsSet”返回 false，默认的“ResetBitIterator”包含第 0 位，且移位计数超出 0 到 63 的范围时会抛出异常。
    ([UUM-156920](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156920))

- `Physics 2D`: 修复了“PhysicsRotate.isNormalized”在旋转未归一化时记录警告的问题，以及“PhysicsRotate.Normalized”警告中方法名称错误的问题。
    ([UUM-156920](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156920))

- `Physics 2D`: 修复了“PhysicsTransform”验证警告中方法名称错误的问题。
    ([UUM-156920](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156920))

- `预制件`: 修复了在并行导入时，进程内与进程外导入预制件的行为不一致问题。

- `项目浏览器`: 修复了将复制的子资源粘贴到文件夹中时，会覆盖同名现有资源并导致对其引用失效的问题。
    ([UUM-121005](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-121005))

- `脚本`: 修复了在帧更新期间取消 `Awaitable.NextFrameAsync 或 Awaitable.EndOfFrameAsync 可等待对象，可能会导致一个无关的 Awaitable 提前完成并返回默认结果。
    ([UUM-156357](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156357))

- `搜索`: 修复了在搜索窗口的检查器中，位于只读包中的场景仍显示“添加场景”选项的错误。
    ([UUM-139396](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-139396))

- `着色器`: 修复了在计算着色器或光线追踪着色器为 null 时调用 `RenderingCommandBuffer.SetKeyword` 导致的崩溃问题。
    ([UUM-158327](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158327))

- `着色器`: 修复了在对空或已销毁的材质上执行 RenderingCommandBuffer 的 SetKeyword 操作时发生的崩溃。
    ([UUM-157105](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-157105))

- `着色器`: 修复了在进行构建时可能发生的罕见崩溃问题。
    ([UUM-148715](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-148715))

- `着色器`: 修复了在画布上渲染未编译或损坏的着色器时，编辑器会崩溃的问题。
    ([UUM-153265](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-153265))

- `着色器`: 修复了默认生成的 LocalKeyword 和 LocalKeywordSpace 字段访问导致编辑器崩溃的问题。
    ([UUM-156424](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156424))

- `着色器`: 修复了当提供的值超出有效枚举范围时，Material.GetPropertyNames 会导致崩溃的问题。
    ([UUM-157945](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-157945))

- `着色器`: 如果主纹理不存在，Material.mainTexture 将返回 null，而不是在控制台记录错误。
    ([UUM-103940](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-103940))

- `SRP Core`: 修复了当构建目标为移动平台时，TraceVirtualOffset 着色器中关于转换为较小类型的着色器警告。
    ([UUM-157091](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-157091))

- `uGUI`: 修复了当画布的“每单位参考像素数”、“缩放因子”、“像素完美”或“渲染摄像机”在 UI 元素（如切片图像、平铺图像和文本）首次绘制后发生变化时，这些元素无法更新的问题。
    ([UUM-151004](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151004))

- `UI Toolkit`: 修复了当某个键的值非常大时，AnimationCurve 的 UXML 属性在保存后会丢失其值的问题。
    ([UUM-156823](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156823))

- `UI 工具包`: 修复了当文本使用字体资源时，若该资源的图集填充较小且轮廓宽度为零或负值，字母周围会出现异常现象的问题。
    ([UUM-146020](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146020))

- `UI 工具包`: 修复了当编辑器启动时，布局中已打开某个窗口（例如渲染图查看器）所导致的日志错误。
    ([UUM-150211](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150211))

- `UI 工具包`: 修复了当对缩放后的元素应用滤镜时，这些元素看起来模糊的问题。
    ([UUM-155303](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-155303))

- `UI Toolkit`: 修复了在 WebGL 2 及部分 OpenGL ES 3.0 设备上保存的矢量图像中缺少纯色和渐变填充的问题，以及在纹理填充之前绘制纯色填充或描边时引发的 ArgumentOutOfRangeException 异常。
    (UUM-155233)

- `UI Toolkit`: 修复了“反转”和“对比度”滤镜在半透明像素上（例如在背景滤镜链中的不透明度之后，或经过滤镜处理的元素的抗锯齿边缘上）生成颜色过亮的问题。
    (UUM-155804)

- `UI Toolkit`: 修复了在编辑名称中包含空格的元素的覆盖规则时，UI Builder 会在“属性覆盖”中添加重复属性，导致 UXML 文件无效的问题。
    ([UUM-149755](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149755))

- `UI Toolkit`: 修复了 UIToolkitInteroperabilityBridge 每帧为每个 UI Toolkit 面板分配 GC 内存的问题。
    ([UUM-158158](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158158))

- `URP`: 修复了某些枚举材质属性中被添加“默认”值的问题。
    ([UUM-134256](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-134256))

- `URP`: 修复了在启用延迟渲染且禁用附加光照阴影、但启用阴影遮罩时，URP 会尝试使用精简变体的错误。
    ([UUM-153600](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-153600))

- `URP`: 修复了在某些 iOS 设备上，当使用 Forward+ 渲染路径且渲染缩放未设置为 1 时发生的崩溃问题。
    ([UUM-151281](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151281))

- `URP`: 修复了当与深度/模板缓冲区已禁用的 2D 渲染器时，渲染器列表和剔除采样会每帧记录错误。
    ([UUM-157948](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-157948))

- `URP`: 修复了以下问题：如果同一编辑器会话中之前曾导入过启用了“支持 LOD 交叉淡入淡出”功能的着色器图，则后续导入的着色器图生成的着色器代码会不同，且资源包的哈希值也会不同。
    (UUM-155529)

- `URP`: 修复了已弃用的 LightingPhysicallyBased 重载方法忽略表面法线，并将“镜面高光”开关作为视图方向的问题。
    (UUM-149002)

- `VFX Graph`: 确保视觉效果区域中的所有本机分配都分配了本机根，且不会发生内存泄漏。
    (UUM-126944)

- `VFX Graph`: 修复了当某些特效实例位于摄像机视场外（尤其在多摄像机场景中）时，对已排序的视觉特效图输出处理会导致 GPU 崩溃或渲染损坏的问题。
    (UUM-149758)

- `XR`: 修复了在子系统被销毁后调用 `SubsystemWithProvider.Start` 时未抛出 `ArgumentNullException` 的问题，该问题会导致已销毁的提供程序被重新启动。
    ([UUM-151411](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151411))




## 6000.3.28f1 版本中的包变更

## 已更新的包

- `com.unity.collab-proxy`: [2.13.6](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.13//changelog/CHANGELOG.html) 更新至 [2.14.0](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.14//changelog/CHANGELOG.html)

- `com.unity.probuilder`: 从 [6.1.3](https://docs.unity3d.com/Packages/com.unity.probuilder@6.1//changelog/CHANGELOG.html) 更新至 [6.1.4](https://docs.unity3d.com/Packages/com.unity.probuilder@6.1//changelog/CHANGELOG.html)

- `com.unity.services.authentication`: 从 [3.8.0](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.8//changelog/CHANGELOG.html) 更新为 [3.8.1](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.8//changelog/CHANGELOG.html)

- `com.unity.services.cloud-build`: 从 [2.1.0](https://docs.unity3d.com/Packages/com.unity.services.cloud-build@2.1//changelog/CHANGELOG.html) 更新至 [2.1.1](https://docs.unity3d.com/Packages/com.unity.services.cloud-build@2.1//changelog/CHANGELOG.html)

- `com.unity.services.wire`: 从 [1.6.0](https://docs.unity3d.com/Packages/com.unity.services.wire@1.6//changelog/CHANGELOG.html) 更新至 [1.6.2](https://docs.unity3d.com/Packages/com.unity.services.wire@1.6//changelog/CHANGELOG.html)

- `com.unity.xr.compositionlayers`: 从 [2.6.0](https://docs.unity3d.com/Packages/com.unity.xr.compositionlayers@2.6//changelog/CHANGELOG.html) 更新至 [2.6.1](https://docs.unity3d.com/Packages/com.unity.xr.compositionlayers@2.6//changelog/CHANGELOG.html)

- `com.unity.memoryprofiler`: 从 [1.1.12](https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.1//changelog/CHANGELOG.html) 更新至 [1.2.0](https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.2//changelog/CHANGELOG.html)

- `com.unity.services.multiplayer`: 从 [2.4.0](https://docs.unity3d.com/Packages/com.unity.services.multiplayer@2.4//changelog/CHANGELOG.html) 更新至 [2.4.1](https://docs.unity3d.com/Packages/com.unity.services.multiplayer@2.4//changelog/CHANGELOG.html)

- `com.unity.asset-manager-for-unity`: 从 [1.12.0](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.12//changelog/CHANGELOG.html) 升级至 [1.12.1](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.12//changelog/CHANGELOG.html)

**新增软件包**

- [com.unity.steamworks-api@1.0.0](https://docs.unity3d.com/Packages/com.unity.steamworks-api@1.0//changelog/CHANGELOG.html)