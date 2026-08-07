# Unity 6000.0.81f1 LTS
发布于 2026年8月6日 星期四 09:43:51 GMT  
https://unity.com/releases/editor/whats-new/6000.0.81f1

# 6000.0.81f1 中的已知问题

- `6000.0.6f1`: [RenderGraph][D3D12] 当使用 AddComputePass 并同时启用 EnableAsyncCompute(true) 和 UseTexture 时，D3D12SwapChain::Present 会发生崩溃
    ([UUM-140183](https://issuetracker.unity3d.com/issues/rendergraph-d3d12-crash-on-d3d12swapchain-present-when-using-addcomputepass-with-enableasynccompute-true-and-usetexture))

- `资源导入器`: 进入“播放模式”时，编辑器在“(Unity) WriteObjectToVector”处崩溃
    ([UUM-112617](https://issuetracker.unity3d.com/issues/editor-crashes-on-unity-writeobjecttovector-when-entering-into-the-play-mode))

- `Metal`: 命令缓冲区超时错误后游戏卡死
    ([UUM-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

在性能较低的设备上暂停带有流式剪辑的 AudioSource 时发生 ARC 崩溃
 ([UUM-148440](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-148440))

当有多个 bee_backend 实例同时运行时，调用 mono_log_write_logfile 会导致崩溃
    ([UUM-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))

生成字体图集时发生崩溃，并产生多个堆栈跟踪
    ([UUM-141061](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-generating-font-atlas-with-sdf16-or-sdf32))



# 6000.0.81f1 发布说明

## API 变更

- `Android`: 新增：支持 SDK Platform 37



## 修复

- `Android`: 修复了在安装 Android 支持后，Unity 首选项文本框出现卡顿的问题。
    (UUM-147435)

- `Android`: ```Screen.brightness``` 的负值现在可恢复设备首选的屏幕亮度。
    ([UUM-145925](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-145925))

- `Android`: 放宽了 AGP 9 对 R8 保留规则的严格执行。
    ([UUM-147136](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147136))

- `动画`: 重构了“动画可播放输出”的绑定和解除绑定验证逻辑，以防止潜在的崩溃。
    ([UUM-146750](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146750))

- `音频`: 修复了在音频混音器中删除快照时发生的错误。
    ([UUM-119443](https://issuetracker.unity3d.com/issues/error-is-thrown-when-deleting-snapshot-with-another-snapshot-present-in-audio-mixer-window))

- `编辑器`: 在“首选项”窗口的索引设置中添加了一些有效的搜索词/关键词。
    ([UUM-146350](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146350))

- `Editor`: 当启动画面处于禁用状态时，调用 `SplashScreen.Stop(FadeOut)` 不再导致应用程序卡死。
    (UUM-143481)

- `Editor`: 修复了由 `AsyncInstantiateOperation` 中未释放的 `CancellationTokenSource` 对象导致的内存泄漏问题。
    ([UUM-147016](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147016))

- `编辑器`: 更新了以管理员权限运行 Unity 时 WinEditor 的警告对话框文本。
    ([UUM-146796](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146796))

- `Graphics`: 修复了在 XR 模式下启用动态分辨率并使用注入的 RenderObjects 渲染通道时出现的渲染问题。
    ([UUM-142592](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-142592))

- `HDRP`: 更新了 `ClearBuffer2D` 着色器，以支持多视图。
    ([UUM-137877](https://issuetracker.unity3d.com/issues/hdrp-xr-dx12-ssr-pbr-accumulation-algorithm-artifacts-are-present-in-one-eye-when-using-spi-openxr-rendering-mode))

- `iOS`: 修复了一个错误，该错误会导致下拉 iOS 控制中心时，Unity 应用停止播放音频。
    ([UUM-145522](https://issuetracker.unity3d.com/issues/ios-audio-is-cut-out-when-accessing-ios-control-center))

- `iOS`: 修复了深度摄像头在第二次创建时崩溃的问题。
    ([UUM-141173](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-141173))

- `Linux`: 修复了在新版内核上使用无线 Xbox 360 手柄时，方向键输入被映射到错误方向的问题。
    ([UUM-136083](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-136083))

- `Linux`: 修复了在 Linux 系统上通过蓝牙连接 Xbox 手柄时，Unity 输入系统中部分手柄输入被映射到错误按键的问题。
    ([UUM-144216](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-144216))

- `macOS`: 修复了 macOS 服务器构建中无法找到 libMonoPosixHelper.dylib 的问题。
    ([UUM-141263](https://issuetracker.unity3d.com/issues/macos-server-cannot-find-libmonoposixhelper-dot-dylib-when-calling-gzipstream))

- `物理引擎`: 修复了 ConfigurableJoint 设置在达到距离约束上限时会发生抖动的问题，该问题是由于其接触距离未被正确处理所致。
    ([UUM-146852](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146852))

- `脚本`: 在域重新加载期间，针对过期的 GC 句柄添加了预防性检查及修复措施。
    ([UUM-122598](https://issuetracker.unity3d.com/issues/crash-with-multiple-stack-traces-when-performing-various-actions-with-the-cesium-package-installed))

- `通用 Windows 平台 (UWP)`：修复了在 UWP 上鼠标移动时滚动操作被重新触发的现象。
    ([UUM-144660](https://issuetracker.unity3d.com/issues/uwp-mouse-movement-re-triggers-stale-slash-scroll-value-after-the-scroll-wheel-is-used-once))

- `视频`: 修复了在 macOS 上使用 VideoPlayer 且处于“仅 API”模式并禁用 Unity Audio 时，AudioSampleProvider.sampleFramesAvailable 回调从未触发的issues。
    ([UUM-143660](https://issuetracker.unity3d.com/issues/audiosampleprovider-dot-sampleframesavailable-callback-never-fires-when-using-macos))

- `Web`: 修复了当服务器未设置“Content-Length”标头时，UnityWebRequest 中响应正文的流式传输问题。
    ([UUM-146537](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146537))




## 6000.0.81f1 版本中的包变更

## 已更新的包

- `com.unity.collections`: 从 [2.6.7](https://docs.unity3d.com/Packages/com.unity.collections@2.6//changelog/CHANGELOG.html) 更新至 [2.6.8](https://docs.unity3d.com/Packages/com.unity.collections@2.6//changelog/CHANGELOG.html)

- `com.unity.entities`: 从 [1.4.7](https://docs.unity3d.com/Packages/com.unity.entities@1.4//changelog/CHANGELOG.html) 更新至 [1.4.8](https://docs.unity3d.com/Packages/com.unity.entities@1.4//changelog/CHANGELOG.html)

- `com.unity.netcode`: 从 [1.14.0](https://docs.unity3d.com/Packages/com.unity.netcode@1.14//changelog/CHANGELOG.html) 更新至 [1.14.1](https://docs.unity3d.com/Packages/com.unity.netcode@1.14//changelog/CHANGELOG.html)

- `com.unity.physics`: 从 [1.4.6](https://docs.unity3d.com/Packages/com.unity.physics@1.4//changelog/CHANGELOG.html) 更新为 [1.4.7](https://docs.unity3d.com/Packages/com.unity.physics@1.4//changelog/CHANGELOG.html)

- `com.unity.entities.graphics`: 从 [1.4.20](https://docs.unity3d.com/Packages/com.unity.entities.graphics@1.4//changelog/CHANGELOG.html) 更新至 [1.4.21](https://docs.unity3d.com/Packages/com.unity.entities.graphics@1.4//changelog/CHANGELOG.html)

- `com.unity.2d.animation`: 从 [10.2.2](https://docs.unity3d.com/Packages/com.unity.2d.animation@10.2//changelog/CHANGELOG.html) 更新为 [10.2.3](https://docs.unity3d.com/Packages/com.unity.2d.animation@10.2//changelog/CHANGELOG.html)

- `com.unity.2d.common`: 从 [9.1.1](https://docs.unity3d.com/Packages/com.unity.2d.common@9.1//changelog/CHANGELOG.html) 更新至 [9.1.2](https://docs.unity3d.com/Packages/com.unity.2d.common@9.1//changelog/CHANGELOG.html)

- `com.unity.2d.psdimporter`: 从 [9.1.1](https://docs.unity3d.com/Packages/com.unity.2d.psdimporter@9.1//changelog/CHANGELOG.html) 升级至 [9.1.2](https://docs.unity3d.com/Packages/com.unity.2d.psdimporter@9.1//changelog/CHANGELOG.html)

- `com.unity.2d.spriteshape`: 从 [10.0.7](https://docs.unity3d.com/Packages/com.unity.2d.spriteshape@10.0//changelog/CHANGELOG.html) 更新至 [10.1.1](https://docs.unity3d.com/Packages/com.unity.2d.spriteshape@10.1//changelog/CHANGELOG.html)

- `com.unity.2d.tilemap.extras`: 从 [4.1.0](https://docs.unity3d.com/Packages/com.unity.2d.tilemap.extras@4.1//changelog/CHANGELOG.html) 更新至 [4.1.1](https://docs.unity3d.com/Packages/com.unity.2d.tilemap.extras@4.1//changelog/CHANGELOG.html)

- `com.unity.burst`: 从 [1.8.29](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html) 更新至 [1.8.30](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html)

- `com.unity.services.cloudcode`: 从 [2.10.2](https://docs.unity3d.com/Packages/com.unity.services.cloudcode@2.10//changelog/CHANGELOG.html) 更新至 [2.10.4](https://docs.unity3d.com/Packages/com.unity.services.cloudcode@2.10//changelog/CHANGELOG.html)

- `com.unity.services.economy`: 从 [3.5.3](https://docs.unity3d.com/Packages/com.unity.services.economy@3.5//changelog/CHANGELOG.html) 更新至 [3.5.4](https://docs.unity3d.com/Packages/com.unity.services.economy@3.5//changelog/CHANGELOG.html)

- `com.unity.transport`: 从 [2.7.2](https://docs.unity3d.com/Packages/com.unity.transport@2.7//changelog/CHANGELOG.html) 更新至 [2.7.4](https://docs.unity3d.com/Packages/com.unity.transport@2.7//changelog/CHANGELOG.html)

- `com.unity.microsoft.gdk`: 从 [1.6.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk@1.6//changelog/CHANGELOG.html) 更新为 [1.7.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk@1.7//changelog/CHANGELOG.html)

- `com.unity.microsoft.gdk.tools`: 从 [1.6.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.tools@1.6//changelog/CHANGELOG.html) 更新至 [1.7.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.tools@1.7//changelog/CHANGELOG.html)