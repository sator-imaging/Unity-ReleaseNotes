# Unity 6000.0.80f1 LTS
发布于 2026年7月22日 星期三 11:25:57 GMT  
https://unity.com/releases/editor/whats-new/6000.0.80f1

# 6000.0.80f1 中的已知问题

- `6000.0.23f1`: 在动画器评估期间，若 RigBuilder 重新绑定后退出播放模式，Animator::OnPlayableUnbind 会引发崩溃
    ([UUM-146750](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146750))

- `6000.0.67f1`: [iOS] 访问 iOS 控制中心时音频中断
    ([UUM-145522](https://issuetracker.unity3d.com/issues/ios-audio-is-cut-out-when-accessing-ios-control-center))

- `6000.0.6f1`: [RenderGraph][D3D12] 当使用 AddComputePass 并同时启用 EnableAsyncCompute(true) 和 UseTexture 时，D3D12SwapChain::Present 会发生崩溃
    ([UUM-140183](https://issuetracker.unity3d.com/issues/rendergraph-d3d12-crash-on-d3d12swapchain-present-when-using-addcomputepass-with-enableasynccompute-true-and-usetexture))

- `资源导入器`: 进入播放模式时，编辑器在“(Unity) WriteObjectToVector”步骤发生崩溃
    ([UUM-112617](https://issuetracker.unity3d.com/issues/editor-crashes-on-unity-writeobjecttovector-when-entering-into-the-play-mode))

- `Metal`: 命令缓冲区超时错误后游戏卡死
    ([UUM-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

当有多个 bee_backend 实例同时运行时，在调用 mono_log_write_logfile 时发生崩溃
    ([UUM-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))

生成字体图集时出现崩溃，并伴有多个堆栈跟踪
    ([UUM-141061](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-generating-font-atlas-with-sdf16-or-sdf32))



# 6000.0.80f1 发布说明

## 改进

- `资源管道`: 在
中添加了说明细节



## 修复

- `2D`: 修复了光批处理调试器中按图层名称排序后未刷新的问题。
    ([UUM-136214](https://issuetracker.unity3d.com/issues/layer-names-in-the-light-batching-debugger-window-do-no-update-unless-the-window-is-restarted-or-a-new-layer-is-added-when-renaming-existing-layers))

- `2D`: 修复了“安装 2D 包”按钮在不应禁用时被禁用的问题。
    ([UUM-143583](https://issuetracker.unity3d.com/issues/当未分配任何精灵时，精灵渲染器中的“安装 2D 精灵包”按钮处于禁用状态，这与其自身帮助文本相矛盾))

- `无障碍功能`: 修复了 Android 平台上 `AccessibilityRole.Toggle` 节点状态提示重复的问题。
    ([UUM-146950](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146950))

- `资源导入`: 修复了因访问过期资源导致在关键词::LocalSpace::Find 操作时编辑器崩溃的问题。
    ([UUM-133882](https://issuetracker.unity3d.com/issues/crash-on-keywords-localspace-find-when-reimporting-specific-assets))

- `资源管道`: 修复了在删除引用纹理并使用相同 GUID 恢复后，资源预览仍显示为白色的问题。
    ([UUM-138622](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-138622))

- `文档`: 添加了有关组件使用的补充资源。

- `编辑器`: 修复了在使用 `[SerializeReference]` 字段的多选带有不同 MonoBehaviour 脚本的 GameObject 时，`SerializableManagedRef::CallMethod` 引发崩溃的问题。
    ([UUM-142019](https://issuetracker.unity3d.com/issues/crash-on-serializablemanagedref-callmethod-when-performing-various-unity-operations))

- `编辑器`: 修复了选择一个平台后点击“添加构建配置文件”时，该平台在“平台浏览器”对话框中未被选中的问题。
    (UUM-130650)

- `图形处理`: 修复了在使用光线追踪时，DirectX12 分割图形任务会发生崩溃的问题。
    (UUM-145956)

- `iOS`: 修复了应用进入后台时，iOS 上出现的错误提示“Touch 已被释放”。
    ([UUM-145381](https://issuetracker.unity3d.com/issues/ios-when-application-is-sent-to-background-with-active-touch-error-message-is-printed))

- `网络`: 修复了 UnityWebRequest 产生的 Curl 错误可能无法被正确记录的情况，该问题曾导致故障难以调试。请注意，即使在此情况下，错误仍会正确上报给调用代码。此问题仅影响日志记录。
    ([UUM-145433](https://issuetracker.unity3d.com/issues/unitywebrequest-can-lose-error-messages-from-curl))

- `URP`: 修复了当“污垢纹理”已启用但值为空时，Bloom 效果的运行时着色器变体选择错误的问题。
    ([UUM-141980](https://issuetracker.unity3d.com/issues/bloom-post-processing-effect-in-urp-is-missing-in-a-build-when-dirt-texture-is-enabled-in-the-bloom-override-of-a-global-volume))

- `WebGL`: WebGPU：修复了因缺少 float32-blendable WebGPU 扩展而在某些移动设备上出现的错误。
    ([UUM-145735](https://issuetracker.unity3d.com/issues/webgpu-urp-errors-when-float32-blendable-isnt-available))

- `Windows`: 修复了在 Windows 上使用新输入系统时，通过 `<Pointer>/position` 绑定，笔的位置在游戏视图中会受限于特定区域的问题。
    ([UUM-142269](https://issuetracker.unity3d.com/issues/pen-position-gets-constrained-to-a-limited-area-when-using-a-stylus-in-game-view-or-player))




## 6000.0.80f1 版本中的包变更

## 已更新的包

- `com.unity.services.authentication`: [3.6.1](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.6//changelog/CHANGELOG.html) 更新至 [3.7.3](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.7//changelog/CHANGELOG.html)

- `com.unity.services.qos`: 从 [1.3.0](https://docs.unity3d.com/Packages/com.unity.services.qos@1.3//changelog/CHANGELOG.html) 更新至 [1.4.1](https://docs.unity3d.com/Packages/com.unity.services.qos@1.4//changelog/CHANGELOG.html)