# Unity 2022.3.75f1 LTS
发布于 星期三, 08 四月 2026 06:21:50 GMT
https://unity.com/releases/editor/whats-new/2022.3.75f1

# 2022.3.75f1 中的已知问题

- 金属命令缓冲区超时错误后游戏冻结
    ([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- `金属"`: MacOS 在编辑器中的最小项目在播放模式下出现卡顿
    ([uum-85256](https://issuetracker.unity3d.com/issues/macos-stutters-in-a-minimal-project))



# 2022.3.75f1 发行说明

## 功能

- `版本控制为项目浏览器和检查器中的文件夹添加了 "添加到源代码控制 "和 "撤销更改 "操作。

- 版本控制新增了分支资源管理器，用于可视化和导航分支。

- 版本控制为所有分割器位置添加了跨窗口重载和会话的持久性。

- 版本控制在合并视图中添加了部分应用搁置的支持。

- 版本控制添加了重命名分支和标签的 F2 快捷键。



## 更改

- 版本控制在状态栏中添加了变更集和标签图标。

- 版本控制从 Unity Hub 打开项目时延迟工作区的创建。

- 版本控制改进了跨对话框的文本字段焦点行为，使键盘工作流程更加一致。

- 版本控制改进了 "待更改 "视图中的空状态。

- 版本控制防止错误地将项目连接到不同的组织。

- 版本控制更新了新项目初始化，以执行完整的初始签入。

- 版本控制更新了 macOS 隐藏快捷键为 Cmd+Shift+H。



## 修复

- DX12`: 修复了在恢复绘制到之前绑定为计算着色器 SRV 的渲染目标后缺少资源屏障的问题。
    (UUM-127520)

- 图形确保内置RP blit copy 输出 float4 颜色（而不是 fxed4，后者在金属上被转换为 half4，导致 u16 或 f32 数据截断）。
    ([uum-128591](https://issuetracker.unity3d.com/issues/terrain-heightmap-loses-precision-on-android-and-ios-when-the-heightmap-texture-is-blitted-to-a-rendertexture-using-the-default-blit-shader))

- `IL2CPP`: 修正了 lambda 表达式中无效的 MethodsToPreserve 条目。
    ([uum-124814](https://issuetracker.unity3d.com/issues/unity-cil-linker-fails-on-player-build-when-persistent-listeners-have-and-in-their-xml-attribute-names))

- 输入修正了 IOHIDDevice_GetUsage 中无效的长缓冲指针。
    ([uum-135043](https://issuetracker.unity3d.com/issues/silicon-crash-on-os-unfair-recursive-lock-lock-with-options-when-opening-a-project-while-the-razer-synapse-app-is-open))

- `iOS`: 将 iOS/tvOS minspec 从 12.0 提升至 13.0。
    (UUM-136440)

- `iOS`: 修正了当应用程序已运行时通过自定义 URL 方案或通用链接打开应用程序，或在某些情况下通过深度链接从冷启动启动应用程序时，Application.deepLinkActivated 未被调用的问题。
    ([uum-135497](https://issuetracker.unity3d.com/issues/ios-application-dot-deeplinkactivated-does-not-get-invoked-while-app-is-running-when-uiapplicationscenemanifest-is-added-in-info-dot-plist))

- 物理使用 "Use Fast Midphase "烹饪选项在 "MeshCollider "上进行射线投射时，防止堆栈溢出。
    ([uum-110564](https://issuetracker.unity3d.com/issues/silent-crash-when-raycasting-on-a-specific-dense-mesh))

- `版本控制修正了右键单击侧边栏中的 "待更改 "时出现的布局异常。

- 版本控制`: 修正了从分支差异打开历史记录时的 NullReferenceException 异常。

- `版本控制修正了逐个变更集差异面板中可能出现的 NullReferenceException。

- 版本控制修复并本地化了签入对话框的进度标签。

- 版本控制修复了 "探索软件库 "窗口中的模糊图标。

- 版本控制修正了 Unity 版本控制窗口中按钮的大小写，以符合 Unity 标准。

- 版本控制修正了 Unity 6.4 及更高版本中过时的 instanceID API 使用。

- 版本控制修正了分支视图中逐个变更集 diff 的问题。

- 版本控制修正了分支上下文菜单在表格为空时无法打开的问题。

- 版本控制`: 修正了签入对话框无法自动聚焦注释字段的问题。

- `版本控制`: 修正当表格为空时无法打开标签上下文菜单的问题。

- `版本控制"`: 修复了新建分支按钮在当前选择为变更集或标签时失效的问题。

- `版本控制`: 修复了退出播放模式后状态栏变灰的问题。

- 版本控制修复了 "创建工作区 "过程中的 "统一版本控制 "窗口刷新时不需要移动鼠标的问题。

- 版本控制修正了 Unity 版本控制窗口中验证信息的对齐方式。

- 视频修正了在使用 Vulkan 图形 API 的特定移动设备上无法播放视频的问题。
    ([uum-133914](https://issuetracker.unity3d.com/issues/video-player-renders-no-video-on-specific-devices-when-using-vulkan))




## 2022.3.75f1 中的软件包变更

## 更新的软件包

- `com.unity.2d.aseprite`: [1.1.10](https://docs.unity3d.com/Packages/com.unity.2d.aseprite@1.1//changelog/CHANGELOG.html) 到 [1.1.11](https://docs.unity3d.com/Packages/com.unity.2d.aseprite@1.1//changelog/CHANGELOG.html)

- `com.unity.addressables`: [1.28.2](https://docs.unity3d.com/Packages/com.unity.addressables@1.28//changelog/CHANGELOG.html) 至 [1.29.0](https://docs.unity3d.com/Packages/com.unity.addressables@1.29//changelog/CHANGELOG.html)

- `com.unity.ads`: [4.16.4](https://docs.unity3d.com/Packages/com.unity.ads@4.16//changelog/CHANGELOG.html) 至 [4.17.0](https://docs.unity3d.com/Packages/com.unity.ads@4.17//changelog/CHANGELOG.html)

- `com.unity.burst`: [1.8.28](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html) 到 [1.8.29](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html)

- `com.unity.collab-proxy`: [2.11.3](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.11//changelog/CHANGELOG.html) 到 [2.12.4](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.12//changelog/CHANGELOG.html)

- `com.unity.performance.profile-analyzer`: [1.3.1](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.3//changelog/CHANGELOG.html) 到 [1.3.3](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.3//changelog/CHANGELOG.html)

- `com.unity.postprocessing`: [3.5.0](https://docs.unity3d.com/Packages/com.unity.postprocessing@3.5//changelog/CHANGELOG.html) 到 [3.5.4](https://docs.unity3d.com/Packages/com.unity.postprocessing@3.5//changelog/CHANGELOG.html)

- `com.unity.scriptablebuildpipeline`: [1.23.3](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@1.23//changelog/CHANGELOG.html) 到 [1.23.4](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@1.23//changelog/CHANGELOG.html)

- `com.unity.services.analytics`: [6.2.2](https://docs.unity3d.com/Packages/com.unity.services.analytics@6.2//changelog/CHANGELOG.html) 到 [6.3.0](https://docs.unity3d.com/Packages/com.unity.services.analytics@6.3//changelog/CHANGELOG.html)

- `com.unity.services.vivox`: [16.9.0](https://docs.unity3d.com/Packages/com.unity.services.vivox@16.9//changelog/CHANGELOG.html) 到 [16.10.0](https://docs.unity3d.com/Packages/com.unity.services.vivox@16.10//changelog/CHANGELOG.html)

- `com.unity.timeline`: [1.8.10](https://docs.unity3d.com/Packages/com.unity.timeline@1.8//changelog/CHANGELOG.html) 到 [1.8.12](https://docs.unity3d.com/Packages/com.unity.timeline@1.8//changelog/CHANGELOG.html)

- `com.unity.memoryprofiler`: [1.1.11](https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.1//changelog/CHANGELOG.html) 至 [1.1.12](https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.1//changelog/CHANGELOG.html)

- `com.unity.asset-manager-for-unity`: [1.9.1](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.9//changelog/CHANGELOG.html) 到 [1.10.0](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.10//changelog/CHANGELOG.html)

- `com.unity.cloud.draco`: [5.4.2](https://docs.unity3d.com/Packages/com.unity.cloud.draco@5.4//changelog/CHANGELOG.html) 到 [5.4.3](https://docs.unity3d.com/Packages/com.unity.cloud.draco@5.4//changelog/CHANGELOG.html)

- `com.unity.cloud.ktx`: [3.6.2](https://docs.unity3d.com/Packages/com.unity.cloud.ktx@3.6//changelog/CHANGELOG.html) 到 [3.6.3](https://docs.unity3d.com/Packages/com.unity.cloud.ktx@3.6//changelog/CHANGELOG.html)