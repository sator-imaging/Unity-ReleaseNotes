# Unity 6000.0.82f1 LTS
发布于 2026年8月19日 星期三 13:32:25 GMT  
https://unity.com/releases/editor/whats-new/6000.0.82f1

# 6000.0.82f1 中的已知问题

- `6000.0.11f1`: 在对存储于 StreamingAssets 文件夹中的场景进行灯光烘焙时，调用 _platform_memcmp 会导致崩溃
    ([UUM-149240](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149240))

- `6000.0.6f1`: 当在启用 EnableAsyncCompute(true) 和 UseTexture 时使用 AddComputePass，D3D12SwapChain::Present 会引发崩溃
    ([UUM-140183](https://issuetracker.unity3d.com/issues/rendergraph-d3d12-crash-on-d3d12swapchain-present-when-using-addcomputepass-with-enableasynccompute-true-and-usetexture))

当有多个 bee_backend 实例正在运行时，mono_log_write_logfile 会发生崩溃
    ([UUM-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))

生成字体图集时出现崩溃，并伴随多个堆栈跟踪
    ([UUM-141061](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-generating-font-atlas-with-sdf16-or-sdf32))



# 6000.0.82f1 发布说明

## 修复项

- `AI`: 修复了 NavMeshAgent 在使用 navAgent.Move 移动时卡在箱形障碍物角落的问题。
    ([UUM-136684](https://issuetracker.unity3d.com/issues/navmeshagent-gets-stuck-on-the-corner-of-a-box-shape-navmeshobstacle-when-it-is-moved-with-navagent-dot-move))

- `资源管道`: 修复了在进入“播放”模式时，WriteObjectToVector / CreateOrReloadInspectorCopy 可能导致编辑器崩溃的问题。
    ([UUM-112617](https://issuetracker.unity3d.com/issues/editor-crashes-on-unity-writeobjecttovector-when-entering-into-the-play-mode))

- `构建管道`: 在“内存设置”中（“主分配器” > “其他分配器” > “Remapper 初始容量”），新增了预留 PersistentManager.Remapper 容量的支持。
    (UUM-136275)

- `DX12`: 修复了在 Windows 系统上使用 Direct3D12 图形 API 时，小型纹理被销毁后其占用的 VRAM 未释放回 GPU 驱动程序的问题。<br>
    现在，您可以通过 `d3d12-small-texture-tiles-per-heap` 启动配置参数调整小纹理堆大小，以在 VRAM 回收与堆分配开销之间取得平衡。
    ([UUM-142284](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-142284))

- `编辑器`: 对 Windows 编辑器随附的若干此前未签名的可执行文件进行了联合签名，这些文件此前有时会被杀毒软件拦截。
    (UUM-147382)

- `图形`: 为 `Resolution` 和 `RefreshRate` 添加了 `IEquatable<T>`、`GetHashCode` 以及相等运算符，以避免在比较它们或将其用作字典键时触发垃圾回收分配。
    (UUM-146197)

- `图形`: 修复了 URP 在混合叠加层 UI 纹理的 MSAA 采样计数时出现的问题。

- `图形`: 图形设置中的“从当前场景导入”操作未被添加到撤销列表中。
    ([UUM-148881](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-148881))

- `iOS`: 修复了在 Apple GPU 系列 1-3 上，偶尔无法合并带有 MSAA 深度的渲染通道的问题。
    ([UUM-147831](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147831))

- `iOS`: 修复了旧设备（AppleFamily3及更早版本）上的着色器预热问题。
    ([UUM-147933](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147933))

- `iOS`: 修复了在 2019 年及之后发布的 iPad 上使用 Apple Pencil 时抛出的警告。
    ([UUM-147481](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147481))

- `许可证`: 修复了导入指定用户许可证文件时手动许可证激活失败的问题。

- `多人游戏`: 当启用 GPU 驻留抽屉，且克隆对象的渲染组件被专用服务器角色移除时，编辑器会崩溃。
    ([UUM-147692](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147692))

- `网络`: 当 Web 请求被突然中断时，会解引用无效的纹理指针。
    ([UUM-144540](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-144540))

- `网络`: 修复了在编辑器中长时间运行且涉及多次域名重新加载时，若使用自定义证书处理程序配合 UnityWebRequest，可能导致编辑器崩溃的问题。
    ([UUM-147347](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147347))

- `QNX`: 启动时，报告的用户时间可能发生溢出。
    (UUM-148079)

- `序列化`: 修复了因弱引用在主线程外被销毁而导致的崩溃问题，该情况与 Mon 垃圾回收器关于“弱引用仅应从主线程释放”的假设存在冲突。此修复解决了垃圾回收器内部最终可能发生的崩溃。
    (UUM-143324)

- `SRP Core`: 修复了在不支持按样本着色的 OpenGL ES 3.1 设备上复制 MSAA 纹理时出现的着色器错误；此类设备现将回退到常规的位块传输。
    (UUM-147215)

- `URP`: 修复了当质量级别发生变化时，Metal 和 OpenGL 后缓冲区会保留过时的 MSAA 采样计数的问题，该问题曾导致渲染通过报错“附件 0 是使用 N 个采样创建的，但请求了 M 个采样”。
    (UUM-140492)

- `WebGL`: 修复了具有多层和 Mipmap 的 ASTC 压缩纹理其纹理数据上传不正确的问题。
    (UUM-145086)




## 6000.0.82f1 版本中的包变更

## 已更新的包

- `com.unity.collab-proxy`: [2.12.4](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.12//changelog/CHANGELOG.html) 更新至 [2.13.6](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.13//changelog/CHANGELOG.html)

- `com.unity.formats.alembic`: 从 [2.4.5](https://docs.unity3d.com/Packages/com.unity.formats.alembic@2.4//changelog/CHANGELOG.html) 更新至 [2.4.7](https://docs.unity3d.com/Packages/com.unity.formats.alembic@2.4//changelog/CHANGELOG.html)

- `com.unity.recorder`: 从 [5.1.6](https://docs.unity3d.com/Packages/com.unity.recorder@5.1//changelog/CHANGELOG.html) 更新至 [5.1.7](https://docs.unity3d.com/Packages/com.unity.recorder@5.1//changelog/CHANGELOG.html)

- `com.unity.multiplayer.tools`: 从 [2.2.9](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@2.2//changelog/CHANGELOG.html) 更新至 [2.2.10](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@2.2//changelog/CHANGELOG.html)

- `com.unity.ai.navigation`: 从 [2.0.13](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html) 更新至 [2.0.14](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html)

- `com.unity.services.deployment`: 从 [1.3.0](https://docs.unity3d.com/Packages/com.unity.services.deployment@1.3//changelog/CHANGELOG.html) 升级至 [1.7.2](https://docs.unity3d.com/Packages/com.unity.services.deployment@1.7//changelog/CHANGELOG.html)