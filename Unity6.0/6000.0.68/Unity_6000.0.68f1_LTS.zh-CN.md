# Unity 6000.0.68f1 LTS
发布于 Wed, 18 Feb 2026 14:49:24 GMT
https://unity.com/releases/editor/whats-new/6000.0.68f1

# 6000.0.68f1 中的已知问题

- `6000.0.55f1,6000.3.0a4`: 在切换用户界面时创建多人房间时发生 RaiseException 时崩溃
    ([uum-132182](https://issuetracker.unity3d.com/issues/crash-on-raiseexception-when-creating-a-multiplayer-room-while-toggling-ui))

- `6000.0.65f1,6000.5.0a4,6000.3.3f1,6000.4.0b2`: 当先前的地形曲率已被取消时，地形工具会沿用先前的地形曲率
    ([uum-134053](https://issuetracker.unity3d.com/issues/the-terrain-tools-follow-the-previous-terrain-curvature-when-it-was-already-undone))

- `6000.2.0a7,6000.0.48f1`: [URP] 如果贴花渲染器技术设置为 "自动"，则通过批量模式构建或在编辑器中不渲染场景/游戏视图时，所有材质都会呈现黑色
    ([uum-134298](https://issuetracker.unity3d.com/issues/urp-all-materials-render-black-when-building-via-batchmode-or-without-rendering-scene-slash-game-view-in-editor-if-decal-renderer-technique-is-set-to-automatic))

- `6000.3.0a4,6000.0.62f1`: [iOS] 当在软键盘上使用 "取消 "按钮时，文本输入字段停止接收更改
    ([uum-133751](https://issuetracker.unity3d.com/issues/ios-text-input-field-stops-receiving-changes-when-the-cancel-button-is-used-on-the-soft-keyboard))

- `6000.5.0a5`: 当使用 Screen.SetResolution() 改变显示分辨率时，DX12 播放器亮度发生变化
    ([uum-134064](https://issuetracker.unity3d.com/issues/dx12-player-brightness-changes-when-changing-display-resolution-with-screen-dot-setresolution))

- `IL2CPP`: [iOS] [Android] 在 IL2CPP 构建过程中外部库泛型失败
    ([uum-125284](https://issuetracker.unity3d.com/issues/ios-android-external-library-generics-fail-during-il2cpp-build))

- 金属命令缓冲区超时错误后游戏冻结
    ([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- `金属"`: MacOS 在编辑器中的最小项目在播放模式下出现卡顿
    ([uum-85256](https://issuetracker.unity3d.com/issues/macos-stutters-in-a-minimal-project))

- 平台音频[Windows] 在编辑器中执行各种操作时，AudioManager::InitFMOD 会崩溃
    ([uum-126803](https://issuetracker.unity3d.com/issues/crash-on-audiomanager-initfmod-when-performing-various-actions-in-the-editor))

- 文本 (TextMeshPro)：在 TMPro Font Asset Creator 中生成多线程字体图集时，在 UNITY_FT_Load_Glyph 上发生崩溃
    ([uum-125366](https://issuetracker.unity3d.com/issues/crash-on-unity-ft-load-glyph-when-generating-multi-threaded-font-atlas-in-tmpro-font-asset-creator))

在空白 URP 项目中进入和退出播放模式时编辑器内存泄漏
    ([uum-132677](https://issuetracker.unity3d.com/issues/editor-memory-leak-when-entering-and-exiting-play-mode-in-a-blank-urp-project))

在 DirectX 12 独占全屏模式下切换焦点时播放器崩溃
    ([uum-134743](https://issuetracker.unity3d.com/issues/player-crash-when-switching-focus-in-exclusive-fullscreen-mode-with-directx-12))



# 6000.0.68f1 发布说明

## 改进

- 阴影图改进了折叠节点时 UV 节点上通道下拉菜单的外观。
    ([uum-115034](https://issuetracker.unity3d.com/issues/uv-nodes-label-is-cut-off-when-preview-is-collapsed))



## 更改

- 编辑器更改了目标速度（targetVelocity）设置的棱柱关节（Prismatic Articulation Joint）类型，现在将目标速度（Target Velocity）设置为正值会在模拟过程中产生正线速度。同样，将目标速度设置为负值将导致线速度为负值。
    ([uum-113920](https://issuetracker.unity3d.com/issues/prismatic-articulationbody-moves-in-opposite-direction-when-using-targetvelocity))

- `图形纹理导入现在严格遵守 https`: //docs.unity3d.com/Documentation/Manual/ImportingTextures.html 中的支持格式。通过更改图像文件扩展名来规避这一点的做法将不再奏效。如果有必要使用某种图像文件格式，请提交功能请求，以便我们研究如何正确支持该格式。



## 修复

- `2D`: 修正了 Sprite Editor 窗口信息框被模块用户界面遮挡的问题。
    ([uum-131899](https://issuetracker.unity3d.com/issues/inactive-skinning-editor-toolbar-overlaps-the-help-box-in-the-sprite-editor-when-asset-is-not-editable))

- `Android`: 删除了 Android 库文档中多余的空格。
    (UUM-133945)

- 动画修复了 AnimationWindowEvent 检查器中损坏的文档链接。
    ([UUM-131593](https://issuetracker.unity3d.com/issues/animation-event-is-missing-documentation-link))

- `Asset Bundles`: 修正了一个问题，即 `AssetBundleUnloadOperation` 分配的持续时间比预期的要长，并且直到下一次 `GC.collect()` 才会被清除。
    (UUM-132703)

- 错误报告器修复了将离线报告导出到 Unity 项目目录时 Bug Reporter 崩溃的问题。
    ([UUM-129604](https://issuetracker.unity3d.com/issues/bug-reporter-crashes-when-exporting-offline-report-into-a-unity-project-directory))

- `DX12`: 修正了使用 D3D12 时编辑器中 maxQueuedFrames 为 1 时的死锁。
    ([uum-131962](https://issuetracker.unity3d.com/issues/editor-freezes-when-qualitysettings-dot-maxqueuedframes-is-set-to-1-and-dx12-is-used))

- 编辑器在剖析器模块介绍中添加了默认剖析器模块列表。

- 编辑器修正了当 GameObject 检查器被禁用时检查器可能抛出的 NullRefException。
    ([uum-130843](https://issuetracker.unity3d.com/issues/endlayoutgroup-beginlayoutgroup-must-be-called-first-error-is-thrown-when-manually-saving-a-complex-ui-prefab-asset))

- 编辑器修正了外部工具中签名团队 ID 和 iOS/tvOS 配置文件 ID 之间不一致的 ID 值。
    ([uum-132053](https://issuetracker.unity3d.com/issues/inconsistent-id-values-between-signing-team-id-and-ios-slash-tvos-profile-id-in-external-tools))

- 编辑器安卓的发布设置 "构建 "部分现在只能通过全局安卓设置进行编辑。
    ([uum-126778](https://issuetracker.unity3d.com/issues/publishing-settings-are-shared-across-different-custom-build-profiles-when-modifying-build-options))

- `编辑器"`: 在 ProjectSettings 中设置 AssetPipeline 设置时刷新设置。
    (UUM-129185)

- 编辑器当重新连接一个普通的 GameObject 到 prefab 时，保留任何子实例。
    ([UUM-102262](https://issuetracker.unity3d.com/issues/child-prefab-instance-connection-lost-when-reconnecting-parent-prefab))

- `编辑器`: 视窗：当用户右键单击 "后台运行 "应用程序的窗口标题栏时，更新游戏循环。
    ([uum-124735](https://issuetracker.unity3d.com/issues/main-thread-freezes-when-right-clicking-on-the-title-bar-of-a-windowed-player-on-windows))

- `图形`: 修复了从 AssetBundles 加载资源（通常是纹理）时，AsyncResourceUploadBlocking\(\) 中偶尔出现的罕见死锁情况。
    ([uum-126066](https://issuetracker.unity3d.com/issues/android-the-application-freezes-during-the-assetbundle-loading))

- `iOS`: 修复了在 UaaL 设置中调整 unity 视图大小导致渲染中断或崩溃的问题。
    ([uum-130881](https://issuetracker.unity3d.com/issues/ios-rendering-freezes-and-unitygfxdeviceworker-crash-when-show-splash-screen-is-enabled-and-project-is-built-using-unity-as-a-library))

- `iOS`: 调整键盘 UI 以更好地适应液体玻璃。
    (UUM-133464)

- 内核更新了所有转换选项的 TransformAccess 同步。
    (UUM-126050)

- 软件包管理器修复了一个 Windows 问题，即当 Unity 从带有空控制台标题的命令提示符启动时，Unity 软件包管理器可能会在启动时崩溃。
    (PAK-8605)

- 物理修复了在禁用场景重载的情况下制作布料组件时发生崩溃的问题。制作完成后立即进入 Playmode 仍会使 Cloth 实例处于 "仅制作 "状态，这意味着底层模拟对象并未创建。
    ([uum-110845](https://issuetracker.unity3d.com/issues/crash-on-clothscene-processcomponentupdates-when-entering-play-mode-after-editing-cloth-collision-points))

- `阴影图"`: 添加了swizzle节点掩码中的大写有时会导致不正确结果的问题。
    ([uum-132879](https://issuetracker.unity3d.com/issues/expected-color-is-changed-to-black-when-using-swizzle-node))

- `阴影图"`: 现在复制粘贴或复制后节点会被正确选中。
    ([uum-110841](https://issuetracker.unity3d.com/issues/nodes-in-shader-graph-are-not-selected-when-they-are-duplicated))

- 用户界面工具包修正了当 UI 文档执行实时重载并附加了丢失的脚本时抛出的空引用异常。
    ([uum-129344](https://issuetracker.unity3d.com/issues/nullreferenceexception-thrown-when-modifying-a-ui-document-while-a-scene-containing-a-gameobject-with-any-ui-document-and-a-missing-script-component-is-open))

- `用户界面工具包`: 删除元素后停靠生成器时抛出 NullReferenceException。
    ([uum-128717](https://issuetracker.unity3d.com/issues/docked-ui-builder-corrupts-when-the-domain-isnt-reloaded-after-deleting-an-element))

- `VFX Graph`: 修正了一个问题，即曲线和梯度上的分支会导致一些无意义的重新制作并上传到 GPU。
    (UUM-129743)

- 网络修正了在传统输入系统中通过触摸事件模拟鼠标位置的问题（Input.mousePosition\）。
    ([UUM-130369](https://issuetracker.unity3d.com/issues/input-dot-mouseposition-stops-syncing-to-touch-input-when-using-downloadhandlertexture-in-webgl-build))

- `WebGL`: WebGPU：自动处理与着色器绑定的纹理的读取和写入。
    ([uum-131864](https://issuetracker.unity3d.com/issues/webgpu-cant-bind-compute-rwtexture-for-read-and-write))

- `WebGL`: WebGPU： 修复在着色器中使用 RWTexture2D 纹理时的流水线错误，并简化 unorm RWTextures 的使用。
    ([uum-131863](https://issuetracker.unity3d.com/issues/webgpu-errors-with-unorm-and-half4-rwtexture))

- `WebGL`: WebGPU： 使用着色器变量集合预热解决控制台 CreateRenderPipeline 错误。
    ([uum-131262](https://issuetracker.unity3d.com/issues/webgpu-createrenderpipeline-errors-with-shadervariantcollection-warmup))




## 6000.0.68f1 中软件包的更改

## 更新的软件包

- `com.unity.addressables`: [2.8.0](https://docs.unity3d.com/Packages/com.unity.addressables@2.8//changelog/CHANGELOG.html) 到 [2.8.1](https://docs.unity3d.com/Packages/com.unity.addressables@2.8//changelog/CHANGELOG.html)

- `com.unity.burst`: [1.8.27](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html) 到 [1.8.28](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html)

- `com.unity.formats.alembic`: [2.4.2](https://docs.unity3d.com/Packages/com.unity.formats.alembic@2.4//changelog/CHANGELOG.html) 到 [2.4.4](https://docs.unity3d.com/Packages/com.unity.formats.alembic@2.4//changelog/CHANGELOG.html)

- `com.unity.ide.visualstudio`: [2.0.26](https://docs.unity3d.com/Packages/com.unity.ide.visualstudio@2.0//changelog/CHANGELOG.html) 到 [2.0.27](https://docs.unity3d.com/Packages/com.unity.ide.visualstudio@2.0//changelog/CHANGELOG.html)

- `com.unity.mobile.notifications`: [2.4.2](https://docs.unity3d.com/Packages/com.unity.mobile.notifications@2.4//changelog/CHANGELOG.html) 到 [2.4.3](https://docs.unity3d.com/Packages/com.unity.mobile.notifications@2.4//changelog/CHANGELOG.html)

- `com.unity.scriptablebuildpipeline`: [2.5.1](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@2.5//changelog/CHANGELOG.html) 到 [2.5.2](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@2.5//changelog/CHANGELOG.html)

- `com.autodesk.fbx`: 5.1.1 至 5.1.3

- `com.unity.memoryprofiler`: [1.1.9](https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.1//changelog/CHANGELOG.html) 至 [1.1.11](https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.1//changelog/CHANGELOG.html)

- `com.unity.multiplayer.tools`: [2.2.7](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@2.2//changelog/CHANGELOG.html) 到 [2.2.8](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@2.2//changelog/CHANGELOG.html)

- `com.unity.dt.app-ui`: [1.3.1](https://docs.unity3d.com/Packages/com.unity.dt.app-ui@1.3//changelog/CHANGELOG.html) 到 [1.3.5](https://docs.unity3d.com/Packages/com.unity.dt.app-ui@1.3//changelog/CHANGELOG.html)

- `com.unity.ai.inference`: [2.4.1](https://docs.unity3d.com/Packages/com.unity.ai.inference@2.4//changelog/CHANGELOG.html) 至 [2.5.0](https://docs.unity3d.com/Packages/com.unity.ai.inference@2.5//changelog/CHANGELOG.html)