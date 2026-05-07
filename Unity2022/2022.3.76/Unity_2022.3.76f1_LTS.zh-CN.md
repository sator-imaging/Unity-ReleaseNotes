# Unity 2022.3.76f1 LTS
发布于 星期三, 06 五月 2026 09:39:50 GMT
https://unity.com/releases/editor/whats-new/2022.3.76f1

# 2022.3.76f1 中的已知问题

- 金属命令缓冲区超时错误后游戏冻结
    ([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- `金属"`: MacOS 在编辑器中的最小项目在播放模式下出现卡顿
    ([uum-85256](https://issuetracker.unity3d.com/issues/macos-stutters-in-a-minimal-project))



# 2022.3.76f1 发布说明

## 修复

- `资产管道`: 更新了 Unity 手册中的加速器下载链接至最新版本。
    (EAD-2077)

- 编辑器修复了在编辑器中加载和卸载内容文件时的死锁竞赛条件。
    (UUM-137677)

- 编辑器解决了在使用 OpenGL ES 的 Mali GPU 上使用仅模板格式时崩溃的问题。
    ([UUM-111344](https://issuetracker.unity3d.com/issues/android-crash-on-startup-when-depth-stencil-format-is-set-to-s8-uint))

- `引擎诊断`: 向引擎诊断上传堆栈跟踪时添加了重试逻辑。
    (UUM-137962)

- `引擎诊断`: 修复了启用 CrashReportingSettings.captureEditorExceptions 时编辑器异常未报告至引擎诊断的问题。
    ([uum-136672](https://issuetracker.unity3d.com/issues/diagnostics-does-not-report-editor-exceptions-when-using-crashreportingsettings-dot-captureeditorexceptions))

- 图形为 "ImageConversion "类使用的 JPEG 解码器添加了预防措施，以防止利用 LJT-01-003 漏洞拒绝服务。Unity 现在会在解码 1000 次逐行扫描后自动中止 JPEG 文件的解码。
    (UUM-129186)

- 图形修复了在 Adreno 设备上使用 GPU 换肤时的崩溃问题。
    ([UUM-93243](https://issuetracker.unity3d.com/issues/crash-on-apigles-clearbuffersubdata-when-running-the-player-a-second-time-on-meta-quest-2))

- 图形修正了在 DX12、Metal 和传统 Vulkan 设备中使用 ScalableBufferManager 时 MSAA CameraDepthTexture 大小调整不一致的问题，以及修正了在构建独立或 Android 播放器时抛出隐式截断向量类型着色器警告的问题。
    ([uum-100367](https://issuetracker.unity3d.com/issues/android-ios-macos-inconsistent-cameradepthtexture-behavior-when-using-scalablebuffermanager-across-devices))

- 图形修正了为统一缓冲区绑定传递无效绑定槽时 OpenGLES 崩溃的问题。
    (UUM-138897)

- `IL2CPP`: 修正了 libil2cpp 代码中的 C++ 警告。
    (UUM-138294)

- `IL2CPP`: 修正了可能导致生成无效代码的 C++ 指针别名问题。
    ([UUM-132447](https://issuetracker.unity3d.com/issues/ios-stripping-issue-on-xcode-26-when-use-incremental-gc-is-disabled))

- `iOS`: 进一步改进了 UIScene 生命周期事件--通用深层链接处理，提前移动 AbsoluteURL 设置以避免在 Awake\(\) 中错过。
    (UUM-140746)

- 网络修正了 MbedTLS 中的一个回归，当尝试从软件包管理器的资产商店下载资产时，该回归会导致 TLS 握手错误。其他 HTTPS 端点也可能受到此回归的影响。
    (UUM-141298)

- 网络将 MbedTLS 更新至 3.6.6 版，以解决一些（次要且可能无法利用的）安全漏洞。
    (UUM-140908)

- `脚本在 ScriptingCoverage`: FilterRecordedMethods 中添加了主线程保护，以保证脚本重载时的线程安全。
    ([UUM-137724](https://issuetracker.unity3d.com/issues/crash-on-mono-jit-runtime-invoke-when-disabling-the-debug-mode-with-the-code-coverage-enabled))




## 2022.3.76f1 中的软件包变更

## 更新的软件包

- `com.unity.ide.rider`: [3.0.39](https://docs.unity3d.com/Packages/com.unity.ide.rider@3.0//changelog/CHANGELOG.html) 到 [3.0.40](https://docs.unity3d.com/Packages/com.unity.ide.rider@3.0//changelog/CHANGELOG.html)

- `com.unity.services.user-reporting`: [2.0.14](https://docs.unity3d.com/Packages/com.unity.services.user-reporting@2.0//changelog/CHANGELOG.html) 到 [2.0.15](https://docs.unity3d.com/Packages/com.unity.services.user-reporting@2.0//changelog/CHANGELOG.html)

- `com.unity.xr.core-utils`: [2.5.3](https://docs.unity3d.com/Packages/com.unity.xr.core-utils@2.5//changelog/CHANGELOG.html) 到 [2.6.0](https://docs.unity3d.com/Packages/com.unity.xr.core-utils@2.6//changelog/CHANGELOG.html)

- `com.unity.asset-manager-for-unity`: [1.10.0](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.10//changelog/CHANGELOG.html) 到 [1.11.0](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.11//changelog/CHANGELOG.html)