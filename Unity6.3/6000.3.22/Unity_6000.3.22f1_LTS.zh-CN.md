# Unity 6000.3.22f1 LTS
发布于 2026年8月13日 星期四 06:39:34 GMT  
https://unity.com/releases/editor/whats-new/6000.3.22f1

# 6000.3.22f1 中的已知问题

- `6000.0.11f1`: 在对存储于 StreamingAssets 文件夹中的场景进行灯光烘焙时，_platform_memcmp 会引发崩溃
    ([UUM-149240](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149240))

- `6000.3.0a1`: 在 PVRAtlassingData::Build 时发生崩溃，且将“灯光可视化”叠加层切换为“预览”模式时出现内存泄漏
    ([UUM-149471](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149471))

- `资源导入器`: 进入播放模式时，在“(Unity) WriteObjectToVector”时，编辑器会崩溃
    ([UUM-112617](https://issuetracker.unity3d.com/issues/editor-crashes-on-unity-writeobjecttovector-when-entering-into-the-play-mode))

- `Metal`: 命令缓冲区超时错误后游戏卡死
    ([UUM-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- `文本（TextMeshPro）`: 在 TMPro 字体资源生成器中生成多线程字体图集时，UNITY_FT_Load_Glyph 引发崩溃
 ([UUM-125366](https://issuetracker.unity3d.com/issues/crash-on-unity-ft-load-glyph-when-generating-multi-threaded-font-atlas-in-tmpro-font-asset-creator))

当多个 bee_backend 实例同时运行时，mono_log_write_logfile 发生崩溃
    ([UUM-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))

生成字体图集时发生崩溃并产生多个堆栈跟踪
    ([UUM-141061](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-generating-font-atlas-with-sdf16-or-sdf32))



# 6000.3.22f1 版本更新日志

## 改进

- `编辑器`: 地形：现在，使用相同非实例化细节原型的地形瓦片之间会共享细节图集纹理，这在多瓦片地形配置中显著降低了内存占用。
    (UUM-148356)



## API 变更

- `Android`: 新增：支持 SDK Platform 37



## 修复

- `自适应性能`: 修复了自适应性能移至引擎模块后，视觉脚本节点 \(瓶颈、 thermal、performance level、boost、performance mode 以及 scaler 事件）在自适应性能移至引擎模块后，不再在播放器中触发的问题。这些事件现由自适应性能示例包程序集转发至可视化脚本 `EventBus`，该处 `VISUAL_SCRIPTING_ENABLED` 定义处于激活状态。
    (UUM-135587)

- `自适应性能`: 在包操作期间禁用自适应性能设置。
    ([UUM-140197](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-140197))

- `Android`: 修复了安装 Android 支持后 Unity 首选项文本字段出现卡顿的问题。
    (UUM-147435)

- `音频`: 修复了在音频子系统中获取锁时，访问版本必须为奇数这一断言问题，该问题发生在编辑器连续运行多天之后。
    ([UUM-146734](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146734))

- `编辑器`: 新增静态函数 CleanupRenderPipelineIfActive，以防止在释放非活动渲染管线时触发 activeRenderPipelineDisposed 事件。
    ([UUM-148022](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-148022))

- `编辑器`: 为“首选项”窗口中的“索引”设置添加了一些有效的搜索词/关键词。 “首选项”窗口中添加了一些有效的搜索词/关键词。
    ([UUM-146350](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146350))

- `编辑器`: 当启动画面处于禁用状态时，调用 `SplashScreen.Stop(FadeOut)` 不再导致应用程序卡死。
    (UUM-143481)

- `编辑器`: 对 Windows 编辑器随附的若干此前未签名的可执行文件进行了联合签名，这些文件此前有时会被杀毒软件拦截。
    (UUM-147382)

- `编辑器`: 禁用了 UITK 编辑器文本的高级字体功能。
    ([UUM-147689](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147689))

- `编辑器`: 在“播放”模式下，禁用了“构建配置文件”设置中的“删除”按钮。
    ([UUM-143194](https://issuetracker.unity3d.com/issues/adaptive-performance-settings-in-the-build-profile-window-can-be-removed-when-in-play-mode-which-results-in-serializedobjectnotcreatableexception-errors-thrown))

- `编辑器`: 修复了一个错误：在“脚本定义”设置列表中添加脚本定义值后，若构建配置文件失去焦点，此时点击弹出提示框中的“还原”按钮，并不会移除新添加的值。
    ([UUM-147113](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147113))

- `编辑器`: 修复了在使用 ATG 时，多行省略号会导致程序崩溃的问题。
    (UUM-147865)

- `编辑器`: 修复了使用 Android Provider 移除自适应性能设置时引发错误的问题。
    ([UUM-143194](https://issuetracker.unity3d.com/issues/adaptive-performance-settings-in-the-build-profile-window-can-be-removed-when-in-play-mode-which-results-in-serializedobjectnotcreatableexception-errors-thrown))

- `编辑器`: 修复了在 Linux 编辑器中，2D 贴图调色板窗口打开后立即关闭的问题。
    ([UUM-146416](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146416))

- `编辑器`: 修复了 ATG 中由制表符宽度导致的崩溃问题。
    (UUM-147528)

- `编辑器`: 通过在每次测试运行时强制导入纹理，修复了测试中的不稳定问题。
    (UUM-122895)

- `编辑器`: 修复了在检查器中，对于缺少脚本的组件，“移除组件”菜单缺失的问题。
    ([UUM-146874](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146874))

- `编辑器`: 修复了对象选择器打开时无法滚动至当前已分配对象的问题。
    ([UUM-143327](https://issuetracker.unity3d.com/issues/object-picker-scrolls-incorrectly-depending-on-which-asset-was-selected-previously-when-in-grid-view))

- `编辑器`: 脚本：修复了安装 AI 助手包（或任何引入简单名称重复的程序集的包）后，控制台出现的“生命周期错误”和“NullReferenceException”错误。
    ([UUM-135379](https://issuetracker.unity3d.com/issues/console-displays-lifecycle-error-and-nullreferenceexception-errors-after-ai-assistant-installation))

- `编辑器`: 更新了以管理员权限运行 Unity 时 WinEditor 的警告对话框文本。
    ([UUM-146796](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146796))

- `GI`: 修复了在“照明”窗口中更改“光源”时，自定义环境反射立方贴图会被遗忘的问题。
    (UUM-133122)
	
- `HDRP`: 在“仅前向光照着色器模式”下，当清漆值设为 0 时，清漆材质会产生屏幕空间反射。
    ([UUM-84980](https://issuetracker.unity.com/issues/8208/clear-coat-materials-produce-screen-space-reflections-when-the-clear-coat-value-is-0-in-forward-only-lit-shader-mode))

- `iOS`: 修复了一个错误，该错误会导致下拉 iOS 控制中心时，Unity 应用停止播放音频。
    ([UUM-145522](https://issuetracker.unity3d.com/issues/ios-audio-is-cut-out-when-accessing-ios-control-center))

- `iOS`: 修复了在 Apple GPU 系列 1-3 上，偶尔无法合并带有 MSAA 深度的渲染通道的问题。
    ([UUM-147831](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147831))

- `iOS`: 修复了旧设备（AppleFamily3及更早版本）上的着色器预热问题。
    ([UUM-147933](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147933))

- `iOS`: 修复了在 2019 年及之后发布的 iPad 上使用 Apple Pencil 时抛出的警告。
    ([UUM-147481](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147481))

- `Linux`: 修复了在新版内核上使用无线 Xbox 360 手柄时，方向键输入被映射到错误方向的问题。
    ([UUM-136083](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-136083))

- `Linux`: 修复了在 Linux 系统上通过蓝牙连接 Xbox 手柄时，Unity 输入系统中部分手柄输入被映射到错误按键的问题。
    ([UUM-144216](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-144216))

- `macOS`: 修复了 macOS 服务器构建中无法找到 libMonoPosixHelper.dylib 的问题。
    ([UUM-141263](https://issuetracker.unity3d.com/issues/macos-server-cannot-find-libmonoposixhelper-dot-dylib-when-calling-gzipstream))

- `多人游戏`: 在未启用多人游戏模式或未安装其软件包的项目中，编辑器窗口布局会加载一个显示“加载失败”的多人游戏模式窗口，且在将其停靠到周围时会抛出 NullReferenceException 异常。
    ([UUM-146870](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146870))

- `包管理器`: 修复了 Asset Store 上的自定义 UPM 包显示为“未安装”的问题。
    ([UUM-131282](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-131282))

- `QNX`: 启动时序可能导致报告的用户时间溢出。
    (UUM-148079)

- `脚本`: 在域重新加载期间，针对过期的 GC 句柄添加了防御性检查/修复。
    ([UUM-122598](https://issuetracker.unity3d.com/issues/crash-with-multiple-stack-traces-when-performing-various-actions-with-the-cesium-package-installed))

- `序列化`: 修复了因弱引用在主线程外被销毁而导致的崩溃问题，该情况与 Mon 垃圾回收器关于“弱引用仅应由主线程释放”的假设相冲突。此修复解决了垃圾回收器内部最终可能发生的崩溃。
    (UUM-143324)

- `SRP Core`: 修复了在不支持按样本着色的 OpenGL ES 3.1 设备上复制 MSAA 纹理时出现的着色器错误；此类设备现将回退到常规的位图复制操作。
    (UUM-147215)

- `UI Toolkit`: 修复了一个单帧闪烁问题，即当使用 `display: none` 隐藏世界空间 UIDocument 后再次显示时，该对象会短暂出现位置错位的情况。
    (UUM-119563)

- `UI Toolkit`: 修复了“对象选择器”窗口在被域重新加载中断时出现故障的问题。
    ([UUM-144436](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-144436))




## 6000.3.22f1 版本中的包变更

## 已更新的包

- `com.unity.netcode`: 从 [1.14.0](https://docs.unity3d.com/Packages/com.unity.netcode@1.14//changelog/CHANGELOG.html) 更新至 [1.14.1](https://docs.unity3d.com/Packages/com.unity.netcode@1.14//changelog/CHANGELOG.html)

- `com.unity.recorder`: 从 [5.1.6](https://docs.unity3d.com/Packages/com.unity.recorder@5.1//changelog/CHANGELOG.html) 升级至 [5.1.7](https://docs.unity3d.com/Packages/com.unity.recorder@5.1//changelog/CHANGELOG.html)

- `com.unity.searcher`: 从 [4.9.4](https://docs.unity3d.com/Packages/com.unity.searcher@4.9//changelog/CHANGELOG.html) 更新至 [4.9.5](https://docs.unity3d.com/Packages/com.unity.searcher@4.9//changelog/CHANGELOG.html)

- `com.unity.xr.meta-openxr`: 从 [2.3.1](https://docs.unity3d.com/Packages/com.unity.xr.meta-openxr@2.3//changelog/CHANGELOG.html) 更新至 [2.3.2](https://docs.unity3d.com/Packages/com.unity.xr.meta-openxr@2.3//changelog/CHANGELOG.html)

- `com.unity.netcode.gameobjects`: 从 [2.13.0](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@2.13//changelog/CHANGELOG.html) 更新至 [2.13.1](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@2.13//changelog/CHANGELOG.html)

- `com.unity.multiplayer.tools`: 从 [2.2.9](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@2.2//changelog/CHANGELOG.html) 更新至 [2.2.10](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@2.2//changelog/CHANGELOG.html)

- `com.unity.services.deployment`: 从 [1.7.1](https://docs.unity3d.com/Packages/com.unity.services.deployment@1.7//changelog/CHANGELOG.html) 更新至 [1.7.2](https://docs.unity3d.com/Packages/com.unity.services.deployment@1.7//changelog/CHANGELOG.html)

- `com.unity.polyspatial`: 从 [3.1.5](https://docs.unity3d.com/Packages/com.unity.polyspatial@3.1//changelog/CHANGELOG.html) 更新至 [3.2.2](https://docs.unity3d.com/Packages/com.unity.polyspatial@3.2//changelog/CHANGELOG.html)

- `com.unity.polyspatial.visionos`: 从 [3.1.5](https://docs.unity3d.com/Packages/com.unity.polyspatial.visionos@3.1//changelog/CHANGELOG.html) 升级至 [3.2.2](https://docs.unity3d.com/Packages/com.unity.polyspatial.visionos@3.2//changelog/CHANGELOG.html)

- `com.unity.polyspatial.xr`: 从 [3.1.5](https://docs.unity3d.com/Packages/com.unity.polyspatial.xr@3.1//changelog/CHANGELOG.html) 升级至 [3.2.2](https://docs.unity3d.com/Packages/com.unity.polyspatial.xr@3.2//changelog/CHANGELOG.html)

- `com.unity.polyspatial.extensions`: 从 [3.1.5](https://docs.unity3d.com/Packages/com.unity.polyspatial.extensions@3.1//changelog/CHANGELOG.html) 升级至 [3.2.2](https://docs.unity3d.com/Packages/com.unity.polyspatial.extensions@3.2//changelog/CHANGELOG.html)

- `com.unity.xr.visionos`: 从 [3.1.5](https://docs.unity3d.com/Packages/com.unity.xr.visionos@3.1//changelog/CHANGELOG.html) 更新至 [3.2.2](https://docs.unity3d.com/Packages/com.unity.xr.visionos@3.2//changelog/CHANGELOG.html)

- `com.unity.services.multiplayer`: 从 [2.2.4](https://docs.unity3d.com/Packages/com.unity.services.multiplayer@2.2//changelog/CHANGELOG.html) 更新至 [2.3.0](https://docs.unity3d.com/Packages/com.unity.services.multiplayer@2.3//changelog/CHANGELOG.html)