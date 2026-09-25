# Unity 6000.3.25f1 LTS
发布于 2026年9月24日 星期四 12:52:52 GMT  
https://unity.com/releases/editor/whats-new/6000.3.25f1

# 6000.3.25f1 中的已知问题

- `6000.2.0b2`: [Vulkan] 当 vkAcquireNextImageKHR 返回 VK_TIMEOUT 时，vk::OnscreenSwapChain::AcquireNextImage 会因 SIGSEGV 导致崩溃
    ([UUM-153744](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-153744))

- `6000.3.0a1,6000.0.51f1`: 当启用 Bloom 效果且使用 2D 渲染器时，屏幕变黑
    ([UUM-150232](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150232))

- `6000.3.13f1`: 当启用图形任务（Graphics Jobs）时，若在退出播放模式（Play Mode）过程中销毁了一个着色器，而异步着色器编译队列中尚有针对另一个着色器的变体请求，则会导致死锁
    ([UUM-152966](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-152966))

当有多个 bee_backend 实例正在运行时，mono_log_write_logfile 会引发崩溃
    ([UUM-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))



# 6000.3.25f1 发布说明

## 改进

- `构建系统`: 将捆绑的 7-Zip 更新至 26.03 版本。



## 变更

- `Android`: 将编辑器随附的 Gradle 版本从 9.1.0 更新至 9.3.1。



## 修复

- `Android`: 修复了输入时光标会自动跳回文本末尾的问题。
    ([UUM-121294](https://issuetracker.unity3d.com/issues/android-ios-the-input-field-caret-moves-back-to-the-end-of-the-text-when-typing))

- `Android`: 修复了虚拟键盘与 UGUI 文本框之间的双向同步问题。
    (UUM-133870)

- `Android`: 修复了 `editText` 的 `setText` 方法会将输入法（IME）的内部光标重置为文本末尾的问题，无论 `EditText` 的选中状态如何。
    (UUM-142513)

- `Android`: 修复了 `TouchScreenKeyboard.selection.length` 始终返回 `0` 的问题。
    ([UUM-125821](https://issuetracker.unity3d.com/issues/android-touchscreenkeyboard-dot-selection-dot-length-always-returns-0-when-any-length-text-is-selected))

- `Android`: 在 Android API 级别低于 32 的情况下，SystemInfo.processorModel 和 SystemInfo.processorManufacturer 现返回“未知”，而非警告字符串，这与其他平台的行为一致。
    (UUM-150389)

- `音频`: 修复了播放模式下音频混音器推子发出的咔嗒声。
    ([UUM-150250](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150250))

- `Audio`: 当音频输出设备在经历一段时间静默后恢复输出时，若无法重新初始化，编辑器不再记录错误。现在输出将保持暂停状态，系统会记录一条警告，并在下次使用音频时重试恢复。同时修复了当无法恢复输出时，编辑器关闭可能导致的崩溃问题。
    (UUM-115959)

- `构建系统`: 修复了在构建过程中系统时钟倒转时，IL2CPP Analytics 工具在构建成功后因 JsonException 异常而退出的问题。
    ([UUM-150019](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150019))

- `编辑器`: 修复了当源网格使用非浮点顶点格式（如 8 位 UNorm）时，网格粒子渲染的 UV \(及其他顶点通道\) 不正确的问题。
    ([UUM-141864](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-141864))

- `编辑器`: 修复了检查器中材质“GPU 实例化”和“双面全局光照”字段的撤销/重做功能。
    ([UUM-143569](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-143569))

- `IMGUI`: 在 OnGUI 期间分配 GUISkin 样式时，减少了垃圾回收（GC）的内存分配。
    ([UUM-134155](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-134155))

- `Linux`: 修复了在场景加载过程中打开对话框时，编辑器会在启动画面卡死的问题。
    ([UUM-151324](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151324))

- `粒子效果`: 修复了在某些设备上，启用“摄像机淡出”与“柔和粒子”组合时，粒子会消失的问题。
    ([UUM-146249](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146249))

- `播放器`: 添加了保护机制，以避免在开发版播放器构建中触发调试断言。
    (UUM-152365)

- `Profiler`: 修复了在启用 UI Toolkit 实时刷新选项后，通过独立 Profiler 窗口顶部菜单保存 Profiler 数据时抛出的 NullReferenceException 异常。
    ([UUM-150706](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150706))

- `脚本`: 解决了编译过程中出现的卡死问题。
    (UUM-126023)

- `SRP Core`: 修复了在旧版 iOS 设备（Apple GPU 家族 3 及以下）上，当原生渲染通道被判定超过了单瓦片像素存储限制时，渲染通道无法合并的问题；此前该问题会导致每个渲染通道将整帧数据序列化为单个原生渲染通道。
    ([UUM-148865](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-148865))

- `文本`: 修复了在文本度量中，当连字符前有空格时出现的无限循环问题。
    ([UUM-144559](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-144559))

- `Text`: 修复了源字体卸载/重新加载后字体样式过时的问题。
    (UUM-150877)

- `TextCore`: 修复了在“字体资源创建器”中生成字体资源时可能发生的崩溃问题。
    ([UUM-125366](https://issuetracker.unity3d.com/issues/crash-on-unity-ft-load-glyph-when-generating-multi-threaded-font-atlas-in-tmpro-font-asset-creator))

- `TextCore`: 修复了在“字体资源创建器”中生成字体资源时可能导致的崩溃问题。
    ([UUM-141061](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-generating-font-atlas-with-sdf16-or-sdf32))

- `TextCore`: 修复了在“字体资源生成器”中生成字体资源时，可能使用替代字体样式的问题。
    ([UUM-137866](https://issuetracker.unity3d.com/issues/glyph-adjustment-table-is-modified-when-using-an-existing-tmp-font-atlas-to-generate-a-new-tmp-font-atlas-with-the-same-settings))

- `TextCore`: 修复了在“字体资源生成器”中取消生成字体资源图集时可能发生的内存泄漏问题。
    ([UUM-142952](https://issuetracker.unity3d.com/issues/memory-leak-warnings-are-thrown-when-cancelling-the-creation-of-a-font-asset-using-render-mode-sdf16-or-sdf32))

- `uGUI`: 修复了当字体缺少省略号字形且选中了“省略号溢出”模式时，省略号换行递归的问题。
    ([UUM-134066](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-134066))

- `UI Toolkit`: 修复了从面板中移除的元素会一直保存在内存中，直到下一次焦点导航时才释放的问题。
    ([UUM-151139](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151139))

- `UI Toolkit`: 修复了在 UI Builder 中使用“剪切”操作时，UXML 文档被标记为存在未保存更改的问题。
    ([UUM-151306](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151306))

- `URP`: 修复了贴图地图网格线缺失的问题。 确保使用 SRP 渲染后，预览摄像机的渲染目标正确。
    ([UUM-122618](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-122618))

- `URP`: 修复了在“延迟+”渲染路径中，反射探针无法正确应用于着色器图材质的的问题。
    (UUM-151317)

- `URP`: ScriptableRendererData.TryGetRendererFeature 会抛出 NullReferenceException 异常。
    ([UUM-150772](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150772))

- `VFX Graph`: 禁止对内置属性进行重新分类。
    ([UUM-151058](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151058))

- `VFX Graph`: 修复了在使用 `MeshToSDFBaker` 处理特定体素数量时发生的越界访问问题。
    ([UUM-151674](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151674))

- `视频`: 修复了 VideoPlayer 在进入播放模式时循环播放片段可能导致的卡死问题，该问题会导致播放停止且无法恢复。
    (UUM-144106)

- `视频`: \[Android\] 修复了因 Vulkan 视频解码变通方案应用不当导致的崩溃问题。
    ([UUM-145932](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-145932))

- `Web`: 修复了 NameFilesAsHashes 功能的问题。
    (UUM-148663)

- `WebGL`: 修复了当着色器预期使用立方体纹理，但纹理未被显式绑定时出现的错误。
    ([UUM-150746](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150746))




## 6000.3.25f1 版本中的包变更

## 已更新的包

- `com.unity.addressables`: [2.9.1](https://docs.unity3d.com/Packages/com.unity.addressables@2.9//changelog/CHANGELOG.html) 更新为 [2.10.3](https://docs.unity3d.com/Packages/com.unity.addressables@2.10//changelog/CHANGELOG.html)

- `com.unity.scriptablebuildpipeline`: 从 [2.6.1](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@2.6//changelog/CHANGELOG.html) 更新至 [2.6.2](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@2.6//changelog/CHANGELOG.html)

- `com.unity.services.wire`: 从 [1.5.0](https://docs.unity3d.com/Packages/com.unity.services.wire@1.5//changelog/CHANGELOG.html) 更新至 [1.5.1](https://docs.unity3d.com/Packages/com.unity.services.wire@1.5//changelog/CHANGELOG.html)

- `com.unity.splines`: 从 [2.9.0](https://docs.unity3d.com/Packages/com.unity.splines@2.9//changelog/CHANGELOG.html) 更新为 [2.9.1](https://docs.unity3d.com/Packages/com.unity.splines@2.9//changelog/CHANGELOG.html)

- `com.unity.xr.compositionlayers`: 从 [2.5.0](https://docs.unity3d.com/Packages/com.unity.xr.compositionlayers@2.5//changelog/CHANGELOG.html) 更新为 [2.6.0](https://docs.unity3d.com/Packages/com.unity.xr.compositionlayers@2.6//changelog/CHANGELOG.html)

- `com.unity.profiling.systemmetrics.mali`: 从 [1.1.1](https://docs.unity3d.com/Packages/com.unity.profiling.systemmetrics.mali@1.1//changelog/CHANGELOG.html) 升级至 [1.1.4](https://docs.unity3d.com/Packages/com.unity.profiling.systemmetrics.mali@1.1//changelog/CHANGELOG.html)