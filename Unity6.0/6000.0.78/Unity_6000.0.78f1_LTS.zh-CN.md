# Unity 6000.0.78f1 LTS
发布于 2026年6月25日 星期四 09:24:01 GMT  
https://unity.com/releases/editor/whats-new/6000.0.78f1

# 6000.0.78f1 版本中的已知问题

- `6000.0.11f1`: 包含特定资源的项目在关闭时，会在 ProfilerMutexLock 处发生崩溃
    ([UUM-144371](https://issuetracker.unity3d.com/issues/crash-on-profilermutexlock-when-closing-a-project-with-specific-assets))

- `6000.0.6f1`: 当使用 `AddComputePass` 并同时启用 `EnableAsyncCompute(true)` 和 `UseTexture` 时，在 `D3D12SwapChain::Present` 处发生崩溃
    ([UUM-140183](https://issuetracker.unity3d.com/issues/rendergraph-d3d12-crash-on-d3d12swapchain-present-when-using-addcomputepass-with-enableasynccompute-true-and-usetexture))

- `资源导入器`: 进入“播放模式”时，编辑器在“(Unity) WriteObjectToVector”处崩溃
    ([UUM-112617](https://issuetracker.unity3d.com/issues/editor-crashes-on-unity-writeobjecttovector-when-entering-into-the-play-mode))

- `Metal`: 命令缓冲区超时错误后游戏卡死
    ([UUM-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- `文本（TextMeshPro）`: 在 TMPro 字体资源创建器中生成多线程字体图集时，调用 UNITY_FT_Load_Glyph 会导致崩溃
 ([UUM-125366](https://issuetracker.unity3d.com/issues/crash-on-unity-ft-load-glyph-when-generating-multi-threaded-font-atlas-in-tmpro-font-asset-creator))

当多个 bee_backend 实例同时运行时，mono_log_write_logfile 发生崩溃
    ([UUM-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))

生成字体图集时发生崩溃，并产生多个堆栈跟踪
    ([UUM-141061](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-generating-font-atlas-with-sdf16-or-sdf32))



# 6000.0.78f1 发布说明

## 功能

- `文档`: 在 UDP 文档处理流程中新增了一步，用于解析引擎文档中的交叉引用链接。



## 修复

- `2D`: 修复了在编辑模式下场景视图中打开“贴图调色板”叠加层时，于“播放”模式下选择贴图会引发异常的问题。
    ([UUM-137165](https://issuetracker.unity3d.com/issues/invalidoperationexception-and-nullreferenceexception-errors-are-thrown-when-clicking-inside-a-tile-palette-with-the-tile-palette-overlay-and-tile-palette-edit-enabled))

- `2D`: 修复了在打开特定项目时 ShaderPropertySheet::FindPropertyIndex 引发的崩溃问题。
    ([UUM-110537](https://issuetracker.unity3d.com/issues/crash-on-shaderpropertysheet-findpropertyindex-when-opening-a-specific-project))

- `2D`: 修复了 Light2D 和 Shadow Caster 2D 组件在检查器中显示错误图标的问题。
    ([UUM-132563](https://issuetracker.unity3d.com/issues/not-clear-abbreviation-ld-on-the-2d-light-overlay))

- `Android`: 修复了基于 GameActivity 的应用程序在后台运行时被强制终止的问题。
    ([UUM-143555](https://issuetracker.unity3d.com/issues/android-gameactivity-app-fails-to-relaunch-after-it-was-closed-when-a-foreground-service-started-while-app-was-backgrounded))

- `DX12`: 修复了渲染在主屏幕而非副屏幕上进行的问题。
    ([UUM-102150](https://issuetracker.unity3d.com/issues/uitoolkit-dx3d12-通过在LateUpdate中将style.display属性从none改为flex来启用面板时，该面板会在1帧内渲染到错误的显示器上))

- `DX12`: 修复了在着色器异步编译期间，Meta pass CommandBuffer.DrawMesh\(\) 被忽略的问题。
    (UUM-139294)

- `编辑器`: 修复了“当项目未连接到 Unity Cloud 时，Unity 服务未被禁用，导致构建时间变长”的错误。
    (UUM-143898)

- `编辑器`: 修复了 Linux 编辑器中鼠标前进和后退按钮输入失效的问题。
    ([UUM-143528](https://issuetracker.unity3d.com/issues/input-system-does-not-register-the-backbutton-or-forwardbutton-when-using-the-linux-editor))

- `编辑器`: 更新了 Canvas Renderer 的图标。
    ([UUM-142443](https://issuetracker.unity3d.com/issues/canvas-renderer-component-uses-a-low-resolution-icon))

- `Graphics`: 修复了在某些渲染路径中，缺少骨骼的 `SkinnedMeshRenderer` 组件仍会被渲染的问题。
    (UUM-135684)

- `Graphics`: 设置尚未加载的父对象时，材质属性不再丢失。
    ([UUM-113050](https://issuetracker.unity3d.com/issues/material-properties-are-lost-when-setting-a-parent-that-hasnt-been-loaded-yet))

- `Graphics`: 减少了将渲染命令传递给渲染线程时占用的内存量，并改进了相关诊断功能。
    (UUM-127793)

- `图形`: 当材质启用了 GPU 实例化，但关联的着色器缺少实例化着色器变体时，防止运动向量被破坏。
    ([UUM-130621](https://issuetracker.unity3d.com/issues/gameobject-shows-visual-corruption-due-to-incorrect-previous-transform-matrix-while-using-active-spacewarp))

- `IL2CPP`: 修复了在选择显示方法、文件和行号选项时，日志中的调用堆栈有时会显示错误方法的问题。
    ([UUM-138416](https://issuetracker.unity3d.com/issues/build-stack-trace-contains-invalid-lines-when-building-with-il2cpp-using-scripts-with-delegates-containing-generic-types-in-the-signature))

- `Linux`: 添加了输入文本检查，以防止 AltGr 文本组合触发事件快捷键路径。
    ([UUM-142414](https://issuetracker.unity3d.com/issues/linux-character-at-is-not-inputted-when-pressing-altgr-plus-q-with-a-german-keyboard-layout))

- `粒子`: 修复了 URP 粒子照明（Particle Lit）和简单照明（Simple Lit）着色器在延迟渲染（Deferred）和延迟+（Deferred+）模式下，当渲染背景或应用 SSAO 时，能正确进行照明的问题。
    (UUM-140364)

- `场景管理器`: 修复了当加载多个场景并退出播放模式时，若用户脚本订阅了 `EditorSceneManager.sceneClosed` 并在处理程序中枚举打开的场景，会导致程序崩溃的问题。
    ([UUM-131346](https://issuetracker.unity3d.com/issues/crash-on-scene-custom-getpathinternal-when-exiting-play-mode-while-listening-to-editorscenemanager-dot-sceneclosed-and-printing-open-scenes))

- `场景/游戏视图`: 修复了在使用多显示器时，游戏视图缩放滑块有时会出现异常行为的问题。
    ([UUM-135174](https://issuetracker.unity3d.com/issues/game-view-scale-drops-lower-than-is-possible-to-choose-manually-when-a-domain-reload-occurs))

- `Shadergraph`: 修复了在撤销或重做渐变更改时，渐变选择器窗口会关闭的问题。
    ([UUM-141977](https://issuetracker.unity3d.com/issues/hdr-gradient-editor-window-closes-when-undoing-changes-in-sample-gradient-node-with-ctrl-plus-z))

- `着色器`: 现在使用渲染对象覆盖着色器时，原始材质的属性将被保留。
    ([UUM-100850](https://issuetracker.unity3d.com/issues/material-properties-are-not-preserved-when-overriding-shader-using-render-objects))

- `版本控制`: 当空数组被填充后，UnityYAMLMerge 在合并后可能会生成无效的预制体 YAML 文件。在某些情况下，这会导致预制体解析失败并无法使用。
    ([UUM-131530](https://issuetracker.unity3d.com/issues/prefabs-are-corrupted-due-to-inline-styled-yaml-when-unityyamlmerge-is-used-to-merge-prefabs))

- `WebGL`: 修复了 WebGPU 中未包含摄像机的场景中，面片绕行顺序不正确的问题。
    ([UUM-133894](https://issuetracker.unity3d.com/issues/invalid-front-face-configuration-when-building-with-graphicsapi-set-to-webgpu))




## 6000.0.78f1 版本中的包变更

## 已更新的包

- `com.unity.formats.alembic`: 从 [2.4.4](https://docs.unity3d.com/Packages/com.unity.formats.alembic@2.4//changelog/CHANGELOG.html) 更新至 [2.4.5](https://docs.unity3d.com/Packages/com.unity.formats.alembic@2.4//changelog/CHANGELOG.html)

- `com.unity.performance.profile-analyzer`: 从 [1.3.4](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.3//changelog/CHANGELOG.html) 更新至 [1.4.0](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.4//changelog/CHANGELOG.html)

- `com.unity.purchasing`: 从 [4.14.2](https://docs.unity3d.com/Packages/com.unity.purchasing@4.14//changelog/CHANGELOG.html) 更新至 [4.15.1](https://docs.unity3d.com/Packages/com.unity.purchasing@4.15//changelog/CHANGELOG.html)

- `com.unity.formats.fbx`: 从 [5.1.4](https://docs.unity3d.com/Packages/com.unity.formats.fbx@5.1//changelog/CHANGELOG.html) 更新至 [5.1.6](https://docs.unity3d.com/Packages/com.unity.formats.fbx@5.1//changelog/CHANGELOG.html)

- `com.unity.ai.navigation`: 从 [2.0.12](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html) 更新至 [2.0.13](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html)