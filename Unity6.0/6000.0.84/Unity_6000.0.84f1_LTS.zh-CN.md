# Unity 6000.0.84f1 LTS
发布于 2026年9月16日 星期三 08:37:48 GMT  
https://unity.com/releases/editor/whats-new/6000.0.84f1

# 6000.0.84f1 中的已知问题

- `6000.0.6f1`: [RenderGraph][D3D12] 当在 D3D12SwapChain::Present 中同时使用 AddComputePass、EnableAsyncCompute(true) 和 UseTexture 时发生崩溃
    ([UUM-140183](https://issuetracker.unity3d.com/issues/rendergraph-d3d12-crash-on-d3d12swapchain-present-when-using-addcomputepass-with-enableasynccompute-true-and-usetexture))

- `6000.3.0a1,6000.0.51f1`: 当使用 2D 渲染器且开启布鲁姆效果时，会出现黑屏
    ([UUM-150232](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150232))

当有多个 bee_backend 实例同时运行时，执行 mono_log_write_logfile 会导致崩溃
    ([UUM-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))

生成字体图集时出现崩溃并产生多个堆栈跟踪
    ([UUM-141061](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-generating-font-atlas-with-sdf16-or-sdf32))

[WinEditor] 在高轮询率下移动鼠标光标时，播放模式的帧率会显著下降
    ([UUM-142550](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-142550))



# 6000.0.84f1 发布说明

## 变更

- `Android`: 将编辑器随附的 Gradle 版本从 9.1.0 更新至 9.3.1。



## 修复

- `Android`: 修正了 Android 版本标签，使其符合 Google 的命名规范。
    (UUM-150412)

- `Android`: 修复了在 Android 设备上设置“无焦点运行”时，WebCamTexture 无法恢复的问题。
    (UUM-149681)

- `Android`: 在 Android API 级别低于 32 的情况下，SystemInfo.processorModel 和 SystemInfo.processorManufacturer 现返回“未知”而非警告字符串，与其他平台的行为保持一致。
    (UUM-150389)

- `音频`: 修复了播放模式下音频混音器推子发出咔嗒声的问题。
    ([UUM-150250](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150250))

- `Audio`: 当音频输出设备在经历一段时间静默后恢复输出时，若无法重新初始化，编辑器不再记录错误。现在输出将保持暂停状态，系统会记录一条警告，并在下次使用音频时重试恢复。此外，还修复了当无法恢复输出时，编辑器关闭可能导致的潜在崩溃问题。
    (UUM-115959)

- `构建系统`: 修复了在构建过程中系统时钟倒转时，IL2CPP Analytics 工具在构建成功后因 JsonException 异常而退出的问题。
    ([UUM-150019](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150019))

- `编辑器`: 修复了动画窗口中 HDR 颜色未被正确记录的问题。
    ([UUM-83771](https://issuetracker.unity3d.com/issues/hdr-colors-are-recorded-in-gamma-compressed-values-instead-of-linear-values-when-using-the-animation-window))

- `嵌入式Linux`: 修复了首次触摸输入丢失的情况。
    (UUM-150086)

- `图形`: 修复了当“Blit Type”设置为“自动”时，Midgard Mali GPU 设备会冻结的问题。
    (UUM-149414)

- `图形`: 修复了在使用 OpenGL ES 时，因与每种材质（Material）的常量缓冲区相关的内存错误导致的崩溃。
    (UUM-150590)

- `图形`: 质量设置——现在为默认平台添加了省略号，并对名称过长的质量级别添加了“质量级别”标题。
    ([UUM-148889](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-148889))

- `Linux`: 修复了首次触摸输入被丢弃的情况。
    (UUM-150086)

- `QNX`: 修复了首次触摸输入被丢弃的情况。
    (UUM-150086)

- `uGUI`: 修复了当字体缺少省略号字符且选择了“省略号溢出”模式时，省略号换行递归的问题。
    ([UUM-134066](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-134066))

- `URP`: 修复了瓦片地图网格线缺失的问题。 确保使用 SRP 渲染后，预览摄像机的渲染目标正确。
    ([UUM-122618](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-122618))

- `版本控制`: 修复了编辑器启动时引发“UpdateSettings: 未知版本控制插件：XYZ”错误的竞争条件。
    ([UUM-149884](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149884))

- `VFX 图`: 修复了导致内置属性被重新分类的问题。
    ([UUM-151058](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151058))

- `Web`: 修复了 NameFilesAsHashes 功能。
    (UUM-148663)

- `WebGL`: 修复了当着色器期望立方体纹理但未显式绑定纹理时出现的错误。
    ([UUM-150746](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150746))

- `XR`: 修复了在 XR 平台上可能出现的块状或偏移的光照伪影，尤其是在延迟渲染或 Forward+ 渲染路径中使用动态分辨率时。
    (UUM-143709)

- `XR`: 修复了在启用深度纹理提交的情况下，运行时更改 MSAA 级别时 XR 图形会出现卡死的情况。




## 6000.0.84f1 版本中的包更改

## 已更新的包

- `com.unity.addressables`: [2.9.1](https://docs.unity3d.com/Packages/com.unity.addressables@2.9//changelog/CHANGELOG.html) 更新至 [2.10.3](https://docs.unity3d.com/Packages/com.unity.addressables@2.10//changelog/CHANGELOG.html)

- `com.unity.inputsystem`: 从 [1.19.0](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.19//changelog/CHANGELOG.html) 更新至 [1.20.0](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.20//changelog/CHANGELOG.html)

- `com.unity.scriptablebuildpipeline`: 从 [2.6.1](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@2.6//changelog/CHANGELOG.html) 更新至 [2.6.2](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@2.6//changelog/CHANGELOG.html)

- `com.unity.terrain-tools`: 从 [5.3.2](https://docs.unity3d.com/Packages/com.unity.terrain-tools@5.3//changelog/CHANGELOG.html) 更新至 [5.3.3](https://docs.unity3d.com/Packages/com.unity.terrain-tools@5.3//changelog/CHANGELOG.html)