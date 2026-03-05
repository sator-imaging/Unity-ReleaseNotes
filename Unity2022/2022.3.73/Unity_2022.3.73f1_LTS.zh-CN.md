# Unity 2022.3.73f1 LTS
发表于 星期三, 04 三月 2026 13:54:00 GMT
https://unity.com/releases/editor/whats-new/2022.3.73f1

# 2022.3.73f1 中的已知问题

- 金属命令缓冲区超时错误后游戏冻结
    ([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- `金属"`: MacOS 在编辑器中的最小项目在播放模式下出现卡顿
    ([uum-85256](https://issuetracker.unity3d.com/issues/macos-stutters-in-a-minimal-project))

- `视频修正 2022.3.X`: 在某些 Android 设备上多次启用和禁用视频时，视频播放器会冻结或停止
    (UUM-112470)

- `Windows`: 启用 "后台运行 "并切换活动窗口时，播放器会挂起
    ([UUM-130495](https://issuetracker.unity3d.com/issues/player-hangs-when-the-run-in-background-is-enabled-and-active-window-is-switched))



# 2022.3.73f1 发行说明

## 更改

- `图形纹理导入现在严格遵守 https`: //docs.unity3d.com/Documentation/Manual/ImportingTextures.html 中的支持格式。通过更改图像文件扩展名来规避这一规定的做法将不再奏效。如果需要某种图像文件格式，请提交功能请求，以便我们研究如何正确支持该格式。



## 修复

- `Asset Bundles`: 修正了一个问题，即 `AssetBundleUnloadOperation` 分配的持续时间比预期的要长，并且直到下一次 `GC.collect()` 才会被清除。
    (UUM-132703)

- 编辑器修正了一个问题，即 EditorUtility.CompressTexture / EditorUtility.CompressCubemapTexture 会在压缩过程中过早中断对签名 EAC 格式的压缩，导致纹理处于破碎状态。请注意，有符号的 EAC 格式不支持压缩，这一点已添加到 API 文档中。

- 编辑器修正了 EditorUtility.CompressTexture / EditorUtility.CompressCubemapTexture 中的一个问题，即有可能尝试将 NPOT mipmapped 纹理压缩为不支持的目标格式。有关此问题的其他详细信息已添加到 API 文档中。
    ([uum-129605](https://issuetracker.unity3d.com/issues/corrupted-mipmaps-are-generated-when-using-editorutility-dot-compresstexture-with-npot-textures))

- `iOS`: 调整了键盘 UI 以更好地适应液体玻璃。
    (UUM-133464)

- 软件包管理器使用 upm 软件包的 Url 深度链接会在可发现的情况下显示所选软件包。如果指定了版本或无法发现软件包，也会显示添加弹出窗口。
    (PAK-8687)




## 2022.3.73f1 中的软件包变更

## 更新的软件包

- `com.unity.inputsystem`: [1.18.0](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.18//changelog/CHANGELOG.html) 到 [1.19.0](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.19//changelog/CHANGELOG.html)

- `com.unity.services.analytics`: [6.2.1](https://docs.unity3d.com/Packages/com.unity.services.analytics@6.2//changelog/CHANGELOG.html) 到 [6.2.2](https://docs.unity3d.com/Packages/com.unity.services.analytics@6.2//changelog/CHANGELOG.html)

- `com.unity.memoryprofiler`: [1.1.10](https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.1//changelog/CHANGELOG.html) 到 [1.1.11](https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.1//changelog/CHANGELOG.html)

- `com.unity.microsoft.gdk`: [1.5.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk@1.5//changelog/CHANGELOG.html) 到 [1.5.1](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk@1.5//changelog/CHANGELOG.html)

- `com.unity.microsoft.gdk.tools`: [1.5.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.tools@1.5//changelog/CHANGELOG.html) 到 [1.5.1](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.tools@1.5//changelog/CHANGELOG.html)

- `com.unity.microsoft.gdk.discovery`: [1.2.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.discovery@1.2//changelog/CHANGELOG.html) 到 [1.2.1](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.discovery@1.2//changelog/CHANGELOG.html)