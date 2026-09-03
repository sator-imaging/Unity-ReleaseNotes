# Unity 6000.0.83f1 LTS
发布于 2026年9月2日 星期三 10:47:00 GMT  
https://unity.com/releases/editor/whats-new/6000.0.83f1

# 6000.0.83f1 中的已知问题

- `2021.3.34f1`: 播放模式下调节音量时，音频混音器会发出咔嗒声
    ([UUM-150250](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150250))

- `6000.0.6f1`: [RenderGraph][D3D12] 当使用 AddComputePass 并同时启用 EnableAsyncCompute(true) 和 UseTexture 时，D3D12SwapChain::Present 会发生崩溃
    ([UUM-140183](https://issuetracker.unity3d.com/issues/rendergraph-d3d12-crash-on-d3d12swapchain-present-when-using-addcomputepass-with-enableasynccompute-true-and-usetexture))

当有多个 bee_backend 实例同时运行时，mono_log_write_logfile 会发生崩溃
    ([UUM-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))

生成字体图集时出现崩溃，并伴有多个堆栈跟踪
    ([UUM-141061](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-generating-font-atlas-with-sdf16-or-sdf32))



# 6000.0.83f1 发布说明

## 变更

- `Mono`: 从 `ToFileDescriptor` 中移除断言
    ([UUM-145761](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-145761))



## 修复

- `AI`: 由于配置不支持，NavMeshAgent 会尝试通过向任意方向跳跃来脱离其自身的 NavMeshObstacle 组件。现在，该代理会朝一个稳定的方向移动。
    (UUM-141803)

- `AI`: 在盒状 NavMeshObstacle 内部创建或传送而来的 NavMeshAgent 无法移动出障碍物。
    ([UUM-146477](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146477))

- `Android`: 修复了 Android 外部工具设置面板中的对齐问题。
    (UUM-148378)

- `音频`: 修复了暂停包含仍在加载中的流媒体片段的 AudioRandomContainer 时发生的崩溃问题。
    (UUM-148440)

- `音频`: 修复了重置音频设置后，某些音频片段的 LoadState 状态无效的问题。
    ([UUM-147700](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147700))

- `代码编辑器`: 修复了“首选项”>“外部工具”中的“重置参数”按钮，使其能立即更新“外部脚本编辑器参数”字段，而非仅在焦点切换后才更新。
    (UUM-150210)

- `编辑器`: 修复了在复制操作过程中尝试删除不存在的资源的问题。
    ([UUM-144993](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-144993))

- `编辑器`: 修复了在构建过程中与加速器断开连接时发生的崩溃问题。
    ([UUM-148391](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-148391))

- `编辑器`: 修复了浮动视频片段检查器预览错误及外观警告。
    ([UUM-147192](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147192))

- `编辑器`: 修复了在导入或转码带有“裁剪”和“偏移”设置的视频时，Windows 版编辑器崩溃的问题。
    ([UUM-146426](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146426))

- `EmbeddedLinux`: 修复了系统中不存在 `wl_seat` 时发生的崩溃问题。
    (UUM-148754)

- `GI`: 修复了为放置在 StreamingAssets 中的场景烘焙光照时发生的崩溃问题。
    ([UUM-149240](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149240))

- `Graphics`: 在启用 GRD 时，对 staticShadowCaster 的修改现在能正确更新。
    ([UUM-140724](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-140724))

- `Graphics`: 修复了 Vulkan 播放器不遵循 'PlayerSettings.vulkanNumSwapchainBuffers' 值，而是固定使用 3 个交换链缓冲区的问题。
    (UUM-148724)

- `图形`: 修复了在使用 XR 并启用“最小化 Unity '屏幕' 尺寸”优化时，Mipmap 级别计算不正确的问题。<br>
    在 SRP 模式下，XR 中的摄像机矩形现在会正确返回单眼尺寸，而非合并的立体尺寸。这会影响任何依赖摄像机矩形进行分辨率相关计算的系统，包括 Mipmap 流式传输和基于分辨率的用户界面/文本渲染。如有需要，请调整 Mipmap 流式传输设置或用户界面缩放比例。
    ([UUM-47681](https://issuetracker.unity3d.com/issues/calculated-mipmap-level-does-not-taking-xr-resolution-into-account))

- `SRP Core`: 修复了 AMDUnityPlugin，使其使用静态链接的 CRT。
    (UUM-147060)

- `uGUI`: 修复了当大型 Text \(TMP\) GameObject 的“溢出”属性设置为“省略号”时抛出 `IndexOutOfRangeException` 的问题。
    ([UUM-134477](https://issuetracker.unity3d.com/issues/indexoutofrangeexception-index-was-outside-the-bounds-of-the-array-dot-error-is-thrown-when-large-text-tmp-gameobject-overflow-field-is-set-to-ellipsis))

- `UI Toolkit`: 修复了在世界空间 UI 渲染过程中，当内部绘制范围列表处于部分已满状态时其长度增加所引发的 ArgumentException 异常。
    (UUM-149611)

- `UI Toolkit`: 修复了当存在 8 个或更多按钮时，ToggleButtonGroup 值发生循环溢出的问题。
    ([UUM-149531](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149531))

- `VFX Graph`: 修复了 URP 中的视锥体剔除问题。
    ([UUM-138375](https://issuetracker.unity3d.com/issues/vfx-graph-particles-are-not-culled-when-using-urp-and-frustum-culling-is-enabled-on-vfx-mesh-output))

- `视频`: 修复了在启用 NVIDIA “快速” 垂直同步时，Direct3D 环境下视频在调用 Stop\(\) 后无法重播的问题（解码设备丢失且未能恢复）。
    ([UUM-135548](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-135548))

- `视频`: 修复了 WebM Vorbis 音频轨道报告为 0 Hz 和 0 个声道的问题。
    (UUM-144045)




## 6000.0.83f1 版本中的包变更

## 已更新的包

- `com.unity.netcode`: 从 [1.14.1](https://docs.unity3d.com/Packages/com.unity.netcode@1.14//changelog/CHANGELOG.html) 更新至 [1.14.2](https://docs.unity3d.com/Packages/com.unity.netcode@1.14//changelog/CHANGELOG.html)

- `com.unity.services.authentication`: 从 [3.7.3](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.7//changelog/CHANGELOG.html) 更新至 [3.7.4](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.7//changelog/CHANGELOG.html)

- `com.unity.services.wire`: 从 [1.4.4](https://docs.unity3d.com/Packages/com.unity.services.wire@1.4//changelog/CHANGELOG.html) 更新至 [1.5.0](https://docs.unity3d.com/Packages/com.unity.services.wire@1.5//changelog/CHANGELOG.html)

- `com.unity.timeline`: 从 [1.8.12](https://docs.unity3d.com/Packages/com.unity.timeline@1.8//changelog/CHANGELOG.html) 更新为 [1.8.13](https://docs.unity3d.com/Packages/com.unity.timeline@1.8//changelog/CHANGELOG.html)

- `com.unity.visualscripting`: 从 [1.9.11](https://docs.unity3d.com/Packages/com.unity.visualscripting@1.9//changelog/CHANGELOG.html) 更新为 [1.9.12](https://docs.unity3d.com/Packages/com.unity.visualscripting@1.9//changelog/CHANGELOG.html)