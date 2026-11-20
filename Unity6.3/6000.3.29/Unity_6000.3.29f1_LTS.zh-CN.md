# Unity 6000.3.29f1 LTS
发布于 2026年11月19日 星期四 10:35:33 GMT  
https://unity.com/releases/editor/whats-new/6000.3.29f1

# 6000.3.29f1 中的已知问题

- `Android`: 当启用“在后台运行”和“预测性返回支持”时，从后台返回后，使用返回手势或按钮会关闭应用
    ([UUM-159613](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-159613))

- `编辑器安装程序`: [macOS] 播放器库使用自定义权限进行了代码签名
    ([UUM-156884](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156884))

- `Mecanim 动画`: 在对由旧版 Animation 组件控制的对象调用 AddClip 方法后，销毁该对象时，Animation::AnimationObjectDeletionCallback 会发生崩溃
    ([UUM-161463](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-161463))

- `Mecanim 动画`: 在采样一个具有属性名称为空的 Transform 曲线的 AnimationClip 时，调用 UnityEngine::Animation::SetBoundCurveFloatValue 会导致崩溃
    ([UUM-161382](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-161382))

- `多人游戏第一人称/第三人称模板`: 在采用多人游戏第一人称模板的项目中进入“播放”模式时，执行 memcpy 操作会导致崩溃
    ([UUM-151778](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151778))

- `搜索`: 域重新加载后调用 SearchService.Request 时，搜索数据库发生内存泄漏
    ([UUM-161715](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-161715))

- `SRP Foundation`: 物理旋转设备时，与 RenderPass 相关的 Android 错误会被记录到 Logcat 和控制台中
    ([UUM-157974](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-157974))



# 6000.3.29f1 发布说明

## 改进

- `Graphics`: 修复了异步上传缓冲区损坏时渲染线程卡死的问题，并在发布版构建中对此情况记录了错误日志。
    (UUM-150567)

- `uGUI`: 新增了脚本定义符号 DISABLE_UGUI_UITK_SUPPORT，该符号可排除 uGUI 与 UI Toolkit 的集成，从而使玩家构建版本能在仅在编辑器中使用 UI Toolkit 时，剥离该模块。
    (UUM-159610)

- `URP`: Forward+ 和 Deferred+ 渲染路径不再处理仅位于远平面之外或正交摄像机近平面之前的屏幕区域中的光照和反射探针。



## 变更

- `Profiler`: 修改了“应用已分配内存”计数器，使其在 Android 平台上返回驻留内存和交换内存的总和。
    (UUM-155041)

- `Text`: 将 FreeType 更新至 2.15.0 版本，该版本在 macOS 上增加了对镜像 Apple Color Emoji 字形的支持，并略微调整了“Hinted Smooth”和“OS Default”字体渲染模式下文本的渲染方式。



## 修复

- `2D`: 修复了一个问题：当一个 LineRenderer 或 TrailRenderer 的“蒙版交互”设置为“无”时，如果另一个使用相同材质的 LineRenderer 或 TrailRenderer 启用了“蒙版交互”，前者会被 Sprite 蒙版裁剪。
    ([UUM-158602](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158602))

- `2D`: 修复了当向 SpriteShapeUtility.Generate 传入一个包含两个重合控制点的闭合形状时，“pqInit” 会发生崩溃的问题。<br>
    请注意，此 API 专用于旧版的 Spriteshape 包，将在即将发布的版本中弃用。 如需在未来使用三角剖分功能，请参阅 Spriteshape 包中的 SpriteShapeGenerator.cs。
    ([UUM-156213](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156213))

- `2D`: 修复了在某些 OpenGL ES 设备上，当禁用 2D 渲染器的深度/模板缓冲区设置时，精灵和 UI 无法渲染的问题。
    ([UUM-159093](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-159093))

- `无障碍功能`: 修复了当 UI Automation 客户端（例如屏幕阅读器）正在运行时，Windows 播放器在退出时崩溃的问题。
    ([UUM-157903](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-157903))

- `Android`: 升级 Bouncy Castle（从 1.70 升级至 1.86）。由密钥库管理器 (Keystore Manager) 创建的新签名密钥采用 4096 位 RSA 算法和 SHA256withRSA 证书，而非 2048 位 RSA 算法和 SHA1withRSA 证书。 现有密钥保持不变。
    (UUM-156925)

- `Android`: 修复了当“默认方向”设置为“自动旋转”且“自动旋转行为”设置为“用户”时，应用程序无法旋转至用户锁屏时设定的方向的问题。
    (UUM-158455)

- `Android`: 修复了光标被锁定时，鼠标移动会产生滚动值的问题。
    ([UUM-156720](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156720))

- `Android`: 修复了当输入设备未报告触控板输入源时，触控板输入被忽略且系统会记录错误的情况。
    (UUM-159337)

- `Android`: 将 OpenJDK 从 17.0.18+8 更新至 17.0.21+9，以修复受影响的 eMudhra 中间证书。
    ([UUM-158390](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158390))

- `Android`: 将捆绑的 Android SDK 命令行工具更新至 21.0，以便使用其 avdmanager 创建的 Android 17（API 37.0）模拟器能够正常启动。
    (UUM-157110)

- `资源导入`: 修复了在“变换”编辑器中，当重新导入资源时卸载了仍处于加载状态的对象而导致编辑器崩溃的问题。
    (UUM-126651)

- `资源管道`: 修复了在 macOS 上 exFAT 驱动器中创建项目或复制文件夹时显示“文件已存在”错误的问题。
    ([UUM-150634](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150634))

- `音频`: 修复了四声道模式下音频输出始终不超过 2 个声道的问题。
    ([UUM-146928](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146928))

- `音频`: 修复了当 Unity 无法恢复音频输出后，若重新连接音频输出设备，编辑器中会出现致命错误的问题。
    ([UUM-158166](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158166))

- `DX12`: 修复了在不支持 Direct3D12 的平台上，播放器设置中显示无法使用的 D3D12 设备过滤设置的问题。
    (UUM-149251)

- `编辑器`: 修复了在未接受 Unity 编辑器软件条款且条款文件缺失、为空 或无法读取时，启动时会发生崩溃。
    ([UUM-154911](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-154911))

- `编辑器`: 修复了在包含通过复杂泛型类型声明的 EditorApplication.delayCall 回调的项目中，打开“帮助”>“报告错误”或退出编辑器时发生的崩溃问题。
    ([UUM-122928](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-122928))

- `编辑器`: 修复了在“层级视图”中选择 GameObject 时，若“工具上下文”叠加层已显示但处于折叠状态，会抛出 NullReferenceException 的问题。
    ([UUM-141529](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-141529))

- `编辑器`: 修复了在 macOS 上退出编辑器时偶尔发生的崩溃问题。
    ([UUM-160348](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-160348))

- `编辑器`: 修复了创建会安装包（如 Android XR）的构建配置文件时，可能在包导入完成前就设置好配置文件的问题，这会导致其质量级别缺少渲染管线资源。
    (UUM-156303)

- `编辑器`: 修复了一个错误，即当 `Instantiate` 会考虑父级变换缩放时，`InstantiateAsync` 却不会考虑。
    ([UUM-154591](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-154591))

- `编辑器`: 修复了当脚本使用 `UnityEngine.Device.SystemInfo.processorModel、processorManufacturer 或 supportsMachineLearning 时，玩家构建会因错误 CS0117 而失败。
    ([UUM-154729](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-154729))

- `编辑器`: 修复了在启用“自动保存”功能后，选中名称字段时预制体字段仅部分保存的问题。
    ([UUM-157667](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-157667))

- `编辑器`: 修复了在启用渲染图时，以立方体贴图为目标的渲染请求无法渲染任何内容的问题。
    (UUM-147726)

- `编辑器`: 修复了在域重新加载期间，编辑器有时会在 CloudJob 工作线程的 ujob_execute_job 函数中崩溃，随后在下次域重新加载时卡死的问题。分析服务会在域重新加载期间重启，而其队列中的第一个任务可能依赖于重启前的某个任务。
    ([UUM-158326](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158326))

- `Editor`: 缓解在 WinEditor 的 PlayMode 模式下使用高轮询率鼠标时出现的帧率卡顿问题。
    ([UUM-142550](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-142550))

- `编辑器`: 将 Windows 编辑器中内置的 VCRedist 更新至 14.51.36247 版本。
    (UUM-156578)

- `编辑器`: 当启用图形任务时，编辑器现在会渲染那些在帧内编译了着色器变体的渲染器。 此前因缺少着色器而显示为空白的资源预览和一次性渲染，现在应能通过 SRP Batcher 备用路径按预期渲染。
    (UUM-147205)

- `引擎诊断`: ANR 报告现会归因于该进程最后一次无响应的会话。
    (UUM-157717)

- `引擎诊断`: 在远程配置之前捕获的崩溃、异常和 ANR 报告现可保留其关键属性，包括发生这些问题的会话信息。
    (UUM-159169)

- `引擎诊断`: 修复了在应用引擎诊断配置时，若从工作线程记录崩溃报告可能导致的崩溃问题。
    (UUM-158113)

- `引擎诊断`: 修复了 Android 应用在启动时报告多余会话的问题，该问题会导致首个会话以无效时间戳结束。
    (UUM-157715)

- `GI`: 修复了一个错误，即在使用 APV 且禁用 L2 球面谐波时，混合光源会显示为完全被遮挡。
    ([UUM-156430](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156430))

- `GI`: 修复了在烘焙灯光时，若仅修改了 URP 特定设置，反射探针有时不会被重新烘焙的错误。
    ([UUM-133949](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-133949))

- `GI`: 修复了在 macOS 上使用 Unity Compute 光照烘焙器时，探针遮挡可能烘焙不正确的问题。
    ([UUM-160178](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-160178))

- `Graphics`: 修复了在 Vulkan 环境下使用 GraphicsStateCollection.WarmUpProgressively 预热管道状态对象时发生的崩溃问题。
    (UUM-154071)

- `Graphics`: 修复了在场景加载过程中，当采用半分辨率或更低分辨率流式传输Crunch压缩的立方贴图时，可能出现的卡死或崩溃问题。
    (UUM-150567)

- `Graphics`: 修复了在直接渲染到尚未配置有效附件格式的交换链时，应用着色器通道可能导致的 Vulkan 崩溃问题。
    ([UUM-134018](https://issuetracker.unity3d.com/issues/crash-on-nvoglv64-vkgetinstanceprocaddr-when-starting-the-project-with-vulkan-and-test-framework-performance))

- `图形`: 修复了在使用 Direct3D 12 图形 API 的编辑器中加载 RenderDoc 时，控制台会记录断言错误的问题。
    (UUM-115796)

- `图形`: 修复了使用 -batchmode -quit 导入项目时，URP 和 HDRP 无法升级材质的的问题。
    ([UUM-153768](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-153768))

- `Graphics`: 修复了当 BC 压缩纹理在 CPU 上解压时（例如 GPU 不支持该格式，且 MIP 级别小于 4x4 或其尺寸不是 4 的倍数）发生的内存损坏问题。
    (UUM-154799)

- `图形`: 修复了使用 GraphicsState.SetMeshData 为带骨骼的网格创建 GraphicsStateCollection 并进行预热时，生成的管道与渲染不匹配的问题，因此该管道在 Vulkan 首次渲染时仍会被创建。
    (UUM-156721)

- `Graphics`: Vulkan 交换链中的意外失败现在会正确记录。
    ([UUM-153744](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-153744))

- `Graphics`: Vulkan：修复了在启用图形作业的情况下卸载并重新加载着色器时，因无效着色器模块导致的随机崩溃问题。
    (UUM-136086)

- `许可证`: 修复了当编辑器无法连接到 Unity 许可证客户端时，编辑器在无许可证的情况下仍会继续运行，并在批处理模式下以代码 0 退出程序的问题。
    ([UUM-151817](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151817))

- `Linux`: 修复了在 Linux 系统上，当窗口管理器在项目加载期间关闭编辑器启动界面时导致的崩溃问题。
    ([UUM-132175](https://issuetracker.unity3d.com/issues/linux-crash-on-editorlaunchscreen-platformeditorlaunchscreen-setprogress-when-opening-a-project))

- `Linux`: 修复了在 Linux 上，当工具链生成 DWARF v5（Clang 15+）时，il2cpp.usym 文件生成时，源路径不可用（当工具链生成 DWARF v5 \(Clang 15+\) 时）。
    (UUM-150040)

- `网络`: 将默认随机种子设备从 `/dev/random` 更改为 `/dev/urandom`。

- `播放器`: 缓解了使用高轮询率鼠标时，窗口独立模式播放器出现的帧率卡顿问题。
    ([UUM-147395](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147395))

- `Profiler`: 修复了 ProfilerRecorder.ToArray 在记录器容量溢出后，返回的样本数量少于记录器实际持有的数量的问题。
    ([UUM-159078](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-159078))

- `脚本`: 修复了 `Object.Instantiate` 方法在 `InstantiateParameters` 中接受持久化父对象的问题；现在该方法会记录错误，并像其他 `Instantiate` 重载方法一样创建不带父对象的实例。
    (UUM-150465)

- `脚本`: 修复了 Plane.Equals 对于哈希码不同的平面返回 true 的问题，该问题曾导致 HashSet 和 Dictionary 的查找失败。
    ([UUM-157345](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-157345))

- `脚本`: 修复了运行 ScriptUpdater 时编辑器可能长时间冻结的问题。
    (UUM-154695)

- `序列化`: 修复了当场景中的 GameObject 隶属于在 Player 中加载或来自 AssetBundle 的预制体，且 Resources.UnloadUnusedAssets 卸载了该预制体时发生的崩溃问题。
    (UUM-150465)

- `序列化`: 修复了加载使用预编译程序集的场景时，若该程序集的编辑器版本和播放器版本名称相同，会导致播放器崩溃的问题。
    ([UUM-157381](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-157381))

- `着色器`: 确保材质属性在编辑器中不会被关键字覆盖。
    ([UUM-133561](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-133561))

- `着色器`: 确保材质属性，以防止在编辑器中覆盖关键字。
    ([UUM-76775](https://issuetracker.unity3d.com/issues/material-dot-enablekeyword-method-has-在手动实例化的材质上调用时对材质无影响))

- `着色器`: 修复了使用预加载的 ShaderVariantCollection 反复切换场景时玩家卡死的问题。
    ([UUM-156125](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156125))

- `着色器`: 修复了在后台编译着色器变体时读取着色器消息可能导致编辑器崩溃的问题。
    (UUM-154510)

- `着色器`: 修复了图形设置和构建配置文件中的“显示第一个场景后预加载着色器”选项在勾选后会自动取消勾选，且“每帧预加载时间限制 \(ms\)” 随后显示为 -1 的问题。
    ([UUM-151773](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151773))

- `着色器`: 修复了导入以 `#line` 指令结尾的着色器文件时编辑器崩溃的问题。
    (UUM-159786)

- `着色器`: 修复了当基础材质发生变化后，若中间变体曾锁定该属性，则材质变体会保留旧属性值的问题。
    ([UUM-158581](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158581))

- `SRP Core`: 修复了渲染图在经过 8 次光栅化渲染通道后，即使实际使用的原生子通道少于 8 个，仍会关闭原生渲染通道的问题，这会导致后续通道（如 URP UI 叠加层）需要从内存中重新加载其附件。
    ([UUM-158401](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158401))

- `Text`: 修复了一个 FreeType 漏洞 \(CVE-2026-23865\)，该漏洞在加载格式错误的变量字体时可能导致越界读取。
    ([UUM-140975](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-140975))

- `TextMeshPro`: 修复了在导入 TMP 基本资源后关闭 TMP 导入器窗口时可能出现的“缺少 TextMesh Pro 基本资源”错误。
    ([UUM-147231](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147231))

- `UI Toolkit`: 修复了导入包含无色停点的渐变的 SVG 文件时发生的 NullReferenceException 异常。
    ([UUM-159742](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-159742))

- `UI 工具包`: 修复了在嵌套于另一个 ListView 中的 ListView 中点击或拖动某项时，也会同时选中或拖动父级 ListView 中相应项的问题。
    ([UUM-140195](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-140195))

- `UI Toolkit`: 修复了 Matrix2D.Equals\(Matrix2D\) 对于哈希码不同的矩阵返回 true 的问题。
    ([UUM-158175](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158175))

- `UI 工具包`: 修复了当被裁剪元素具有变换时，以 objectBoundingBox 为单位的 SVG 裁剪路径和蒙版位置偏移的问题。
    ([UUM-159735](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-159735))

- `UI 工具包`: 修复了将 SVG 文件导入为“矢量图像”并采用“抗锯齿弧编码”细分模式时，若使用以 objectBoundingBox 为单位的裁剪路径或蒙版，该文件会显示为空的问题。
    ([UUM-159735](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-159735))

- `UI 工具包`: 修复了当“&lt;radialGradient&gt;”的半径为零时，SVG 导入会生成无效的径向渐变的问题；现在该形状将使用最后一个渐变站的颜色进行填充。
    ([UUM-158256](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158256))

- `UI 工具包`: 修复了在导入 SVG 时，若其形状或组的目标在文件后文中才被定义，会导致“&lt;use&gt;”元素被省略的问题。
    ([UUM-158220](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158220))

- `UI 工具包`: 修复了在文件后半部分定义渐变时，SVG 导入会遗漏渐变描边的问题。
    ([UUM-158255](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158255))

- `UI Toolkit`: 修复了在导入 SVG 时，若存在半径恰为零的弧线，该弧线会被省略的问题；现在该弧线将作为直线绘制。
    ([UUM-158225](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158225))

- `UI 工具包`: 修复了 SVG 导入时，当后面的 “&lt;style&gt;” 元素为同一选择器设置了其他属性，会导致前面 “&lt;style&gt;” 元素的声明被省略的问题。
    ([UUM-158217](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158217))

- `UI 工具包`: 修复了在 SVG 导入时，若“&lt;style&gt;”元素中紧跟“@import" 语句之后的样式规则。
    ([UUM-158228](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158228))

- `UI 工具包`: 修复了 SVG 导入时会丢失“&lt;style&gt;”元素中“@media”代码块后面的样式规则的问题。
    ([UUM-158229](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158229))

- `UI 工具包`: 修复了 SVG 导入时，当多个元素使用文件后文定义的“&lt;clipPath&gt;”时，导致元素未被裁剪的问题。
    ([UUM-158251](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158251))

- `UI 工具包`: 修复了在导入 SVG 时，文件中位于 “&lt;style&gt;” 元素之前的元素未应用 “&lt;style&gt;” 规则的问题。
    ([UUM-158230](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158230))

- `UI Toolkit`: 修复了当“&lt;use&gt;”元素引用另一个“&lt;use&gt;”元素时，SVG 导入会抛出 KeyNotFoundException 的问题。
    ([UUM-158249](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158249))

- `UI Toolkit`: 修复了当“mask”属性引用文件后文定义的“&lt;mask&lt;”时，或引用缺失的蒙版，导致 SVG 导入抛出 ArgumentNullException 的问题。([UUM-158239](https://issuetracker.unity.com/api/v1.0/redirects))"（该元素在文件中定义在后）或指向缺失的蒙版时，会抛出 ArgumentNullException。
    ([UUM-158239](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158239))

- `UI 工具包`: 修复了当“&lt;polygon&gt;”或“&lt;polyline&gt;”的点未分隔（例如“-10-10”）时，SVG 导入会抛出错误的问题。
    ([UUM-158257](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158257))

- `UI 工具包`: 修复了当属性设置为“inherit”时，SVG导入会抛出错误的问题。
    ([UUM-158226](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158226))

- `UI 工具包`: 修复了 VectorUtils.Bounds 对于某些弯曲的贝塞尔曲线段返回的边界过小的问题。
    ([UUM-158205](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158205))

- `UI 工具包`: 修复了 VectorUtils.FlipVerticesInBounds 在边界未从 y = 0 开始时，会将顶点移动到边界之外的问题。
    ([UUM-158215](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158215))

- `UI 工具包`: 修复了当扫掠角度为 0 时，VectorUtils.MakeArc 会返回四分之一圆的问题。
    ([UUM-158218](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158218))

- `UI Toolkit`: 修复了当扫掠角度为一整圈时，VectorUtils.MakeArc 返回空路径的问题。
    ([UUM-158219](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158219))

- `UI 工具包`: 修复了 VectorUtils.SceneNodeBounds 忽略闭合轮廓的闭合曲线的问题。
    ([UUM-158209](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158209))

- `UI 工具包`: 修复了 VectorUtils.SegmentsLength 将闭合路径的闭合曲线误测为直线的问题。
    ([UUM-158208](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158208))

- `URP`: 修复了在使用 WebGL 且 Chromium 运行于 DX11 后端时，灯光渲染形状不正确的错误。
    ([UUM-142771](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-142771))

- `URP`: 修复了渲染管线转换器将预制体报告为已转换，但在同时转换未打开场景中的对象时，这些预制体的更改会丢失的问题。
    ([UUM-160400](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-160400))

- `URP`: 修复了当聚光灯附加到摄像机上时，在 Forward+ 和 Deferred+ 模式下聚光灯边缘出现锯齿状空隙的问题。
    ([UUM-154016](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-154016))

- `URP`: 修复了在使用 Forward+ 或 Deferred+ 渲染路径时，某些聚光灯朝向以及靠近摄像机近平面的聚光灯在屏幕部分区域缺失的问题。

- `URP`: 修复了在 Forward+ 和 Deferred+ 渲染模式下，点光源和聚光灯在屏幕边缘及摄像机近平面附近消失的问题。
    ([UUM-146356](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146356))

- `URP`: 修复了当精灵的骨骼未移动但精灵本身被翻转时，精灵皮肤上的 2D 阴影投射器仍保留未翻转阴影的问题。
    ([UUM-158409](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158409))

- `URP`: 修复了在使用 Forward+ 或 Deferred+ 渲染路径时，位于摄像机后方的聚光灯其照明区域顶部会丢失的问题。
    ([UUM-159132](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-159132))

- `URP`: 修复了独立运行的 URP 2D/3D 应用程序中的多显示器支持问题。
    (UUM-155833)

- `VFX Graph`: 为 URP 添加了管道标签。
    ([UUM-160198](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-160198))

- `VFX Graph`: 修复了当 HLSL 源代码以空格开头时，自定义 HLSL 块和运算符会生成无效着色器代码的问题。
    ([UUM-158603](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158603))

- `XR`: 修复了提交至 XR 深度交换链的深度数据比例错误的问题。
    ([UUM-149514](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149514))




## 6000.3.29f1 版本中的包变更

## 已更新的包

- `com.unity.ads.ios-support`: [1.0.1](https://docs.unity3d.com/Packages/com.unity.ads.ios-support@1.0//changelog/CHANGELOG.html) 更新至 [1.3.0](https://docs.unity3d.com/Packages/com.unity.ads.ios-support@1.3//changelog/CHANGELOG.html)

- `com.unity.services.friends`: 从 [1.3.0](https://docs.unity3d.com/Packages/com.unity.services.friends@1.3//changelog/CHANGELOG.html) 更新至 [1.4.0](https://docs.unity3d.com/Packages/com.unity.services.friends@1.4//changelog/CHANGELOG.html)

- `com.unity.splines`: 从 [2.9.1](https://docs.unity3d.com/Packages/com.unity.splines@2.9//changelog/CHANGELOG.html) 升级至 [2.9.2](https://docs.unity3d.com/Packages/com.unity.splines@2.9//changelog/CHANGELOG.html)

- `com.unity.test-framework.performance`: 从 [3.5.0](https://docs.unity3d.com/Packages/com.unity.test-framework.performance@3.5//changelog/CHANGELOG.html) 更新至 [3.7.0](https://docs.unity3d.com/Packages/com.unity.test-framework.performance@3.7//changelog/CHANGELOG.html)

- `com.unity.visualscripting`: 从 [1.9.12](https://docs.unity3d.com/Packages/com.unity.visualscripting@1.9//changelog/CHANGELOG.html) 更新至 [1.9.13](https://docs.unity3d.com/Packages/com.unity.visualscripting@1.9//changelog/CHANGELOG.html)

- `com.unity.xr.oculus`: 从 [4.5.2](https://docs.unity3d.com/Packages/com.unity.xr.oculus@4.5//changelog/CHANGELOG.html) 更新至 [4.5.6](https://docs.unity3d.com/Packages/com.unity.xr.oculus@4.5//changelog/CHANGELOG.html)

- `com.unity.netcode.gameobjects`: 从 [2.13.3](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@2.13//changelog/CHANGELOG.html) 更新至 [2.14.0](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@2.14//changelog/CHANGELOG.html)

- `com.unity.dt.app-ui`: 从 [2.2.4](https://docs.unity3d.com/Packages/com.unity.dt.app-ui@2.2//changelog/CHANGELOG.html) 升级至 [2.3.1](https://docs.unity3d.com/Packages/com.unity.dt.app-ui@2.3//changelog/CHANGELOG.html)

- `com.unity.cloud.draco`: 从 [5.5.0](https://docs.unity3d.com/Packages/com.unity.cloud.draco@5.5//changelog/CHANGELOG.html) 升级至 [5.6.0](https://docs.unity3d.com/Packages/com.unity.cloud.draco@5.6//changelog/CHANGELOG.html)

- `com.unity.cloud.ktx`: 从 [3.7.1](https://docs.unity3d.com/Packages/com.unity.cloud.ktx@3.7//changelog/CHANGELOG.html) 升级至 [3.8.0](https://docs.unity3d.com/Packages/com.unity.cloud.ktx@3.8//changelog/CHANGELOG.html)