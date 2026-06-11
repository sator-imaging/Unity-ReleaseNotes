# Unity 6000.0.77f1 LTS
发布于 2026年6月10日 星期三 09:18:20 GMT  
https://unity.com/releases/editor/whats-new/6000.0.77f1

# 6000.0.77f1 中的已知问题

- `6000.0.61f1`: 使用 SDF16 或 SDF32 生成字体图集时，tlsf_free 会引发崩溃
    ([UUM-141061](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-generating-font-atlas-with-sdf16-or-sdf32))

- `6000.0.6f1`: [RenderGraph][D3D12] 在使用 AddComputePass 并同时启用 EnableAsyncCompute(true) 和 UseTexture 时，D3D12SwapChain::Present 会发生崩溃
    ([UUM-140183](https://issuetracker.unity3d.com/issues/rendergraph-d3d12-crash-on-d3d12swapchain-present-when-using-addcomputepass-with-enableasynccompute-true-and-usetexture))

- `资源导入器`: 进入播放模式时，编辑器在执行“(Unity) WriteObjectToVector”时崩溃
    ([UUM-112617](https://issuetracker.unity3d.com/issues/editor-crashes-on-unity-writeobjecttovector-when-entering-into-the-play-mode))

- `Metal`: 命令缓冲区超时错误后游戏卡死
    ([UUM-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- 文本 (TextMeshPro)：在 TMPro 字体资源创建器中生成多线程字体图集时，UNITY_FT_Load_Glyph 引发崩溃
    ([UUM-125366](https://issuetracker.unity3d.com/issues/crash-on-unity-ft-load-glyph-when-generating-multi-threaded-font-atlas-in-tmpro-font-asset-creator))

当运行多个 bee_backend 副本时，mono_log_write_logfile 发生崩溃
    ([UUM-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))

在包含特定资源的项目关闭时，ProfilerMutexLock 发生崩溃
    ([UUM-144371](https://issuetracker.unity3d.com/issues/crash-on-profilermutexlock-when-closing-a-project-with-specific-assets))



# 6000.0.77f1 版本说明

## 修复

- `2D`: 修复了添加 Lens Flare 组件时的错误，并增加了对正交摄像机的支持。
    ([UUM-141781](https://issuetracker.unity3d.com/issues/render-graph-execution-and-argumentexception-errors-are-spammed-when-adding-lens-flare-srp-component-in-a-2d-urp-project))

- `2D`: 修复了使用着色器图材质时，缩放值为负的精灵无法被选中的问题。
    ([UUM-141627](https://issuetracker.unity3d.com/issues/sprite-renderer-is-not-selectable-in-scene-view-when-using-a-sprite-shader-graph-material-on-a-negatively-scaled-object))

- `Android`: 修复了在启用 RunWithoutFocus 时将 Android 应用置于后台导致的 Vulkan 崩溃问题。
    (UUM-141888)

- `动画`: 修复了旧版动画系统中的精度不匹配问题，该问题会导致在高帧率下跳过动画事件。
    ([UUM-138951](https://issuetracker.unity3d.com/issues/the-animation-event-is-not-triggered-when-the-frame-rate-is-set-to-120-on-the-s26-ultra))

- `动画`: 修复了在进入或退出播放模式时，悬空的 GameObject 引用可能仍保留在选择列表中的问题。
    (UUM-142098)

- `音频`: 当所有 AudioListener 组件被禁用或其 GameObject 被停用时，音频在 Player 构建中仍会继续播放。
    ([UUM-127556](https://issuetracker.unity3d.com/issues/audiolisteners-still-listen-to-audio-when-their-components-are-disabled-in-player))

- `Audio`: 修复了在播放模式下，若 `MonoBehaviour` 初始状态为禁用，则在 `AudioListener` 上启用 `OnAudioFilterRead` 效果时无法听到声音的问题。
    ([UUM-116871](https://issuetracker.unity3d.com/issues/onaudiofilterread-does-not-affect-signal-on-audiolistener-after-enable))

- `编辑器`: 修复了打开“构建配置文件”窗口时，若未导入“播放器设置”资源会导致崩溃的问题。
    ([UUM-116727](https://issuetracker.unity3d.com/issues/crash-on-std-1-tree-const-iterator-when-opening-the-build-profiles-window-in-a-specific-project))

- `编辑器`: 修复了在 Mac 编辑器中将编辑器语言切换为日语时极少发生的崩溃问题。
    ([UUM-141719](https://issuetracker.unity3d.com/issues/crash-on-platform-strlen-when-the-editors-language-is-changed-to-japanese))

- `Editor`: 修复了在“播放模式”下导入预制体时，存储在 MonoBehaviour/ScriptableObject 字段中的引用可能会丢失的问题。
    ([UUM-139664](https://issuetracker.unity3d.com/issues/当预制体变体在父组件中序列化时，实例化过程中会丢失对其的引用))

- `Editor`: 修复了在批处理模式下使用 -nographics 开关打开包含自定义 DefaultCursor 的项目时，LinuxEditor 会崩溃的问题。
    ([UUM-142569](https://issuetracker.unity3d.com/issues/linuxeditor-crash-on-xaddextension-when-opening-the-unity-editor-on-linux-with-batchmode-and-nographics-on-a-project-with-a-custom-default-cursor))

- `编辑器`: 修复了 TextCore 中精灵资源的 Unicode 处理问题。
    ([UUM-141521](https://issuetracker.unity3d.com/issues/ui-toolkit-doesnt-render-the-assigned-sprites-when-using-unicode-characters-assigned-to-a-sprite))

- `编辑器`: 地形：修复了编辑选中地形的高程图时出现的性能退化问题。
    ([UUM-141526](https://issuetracker.unity3d.com/issues/the-editor-start-performing-very-poorly-when-editing-the-terrain-heightmap-with-terraindata))

- `编辑器`: \[Android\] 将“属性冲突”错误窗口中指向缺失的“Gradle 故障排除”页面的链接，替换为适用于 Unity 6.0 的有效“Android 版 Gradle”链接。
    ([UUM-142945](https://issuetracker.unity3d.com/issues/colliding-attributes-error-opens-a-missing-page-when-pressing-the-troubleshoot-button))

- `Graphics`: 修改了帧清理映射，以移除无效或无内存的纹理 ID，同时不删除这些 ID。
    (UUM-129828)

- `License`: 修复了许可证客户端的重新连接问题。
    ([UUM-142572](https://issuetracker.unity3d.com/issues/floating-license-is-lost-for-concurrent-jobs))

- `Linux`: 修复了 Linux 系统上读取大于 2 GiB 的 POSIX 文件失败的问题。
    ([UUM-140520](https://issuetracker.unity3d.com/issues/couldnt-open-file-for-reading-error-occurs-when-running-binary2text-on-a-file-larger-than-2-gib))

- `网络`: 通过支持多个自动代理，修复了 UUM-135025。
    ([UUM-135025](https://issuetracker.unity3d.com/issues/当Windows代理自动配置脚本返回多个代理时，UnityWebRequest返回curl错误5而非超时))

- `物理引擎`: 修复了因 NvCloth 内部在处理布料间碰撞时过度分配内存而导致的内存损坏问题。
    ([UUM-64185](https://issuetracker.unity3d.com/issues/crash-on-collideparticles-when-entering-play-mode))

- `Physics`: 修复了胶囊碰撞体的调试可视化问题，确保在应用缩放时胶囊顶点能保持曲率。
    ([UUM-142483](https://issuetracker.unity3d.com/issues/colliders-are-rendered-deformed-when-viewed-through-physics-debugger-in-scene-view))

- `Physics`: 修复了 NvCloth 求解器内核中若干 SIMD 运算导致 NaN 值的问题。
    ([UUM-64185](https://issuetracker.unity3d.com/issues/crash-on-collideparticles-when-entering-play-mode))

- `Prefabs`: 清理损坏的 `PrefabInstance` 时，已添加的对象不再被移除。
    ([UUM-142338](https://issuetracker.unity3d.com/issues/crash-on-mergeobjectcollection-when-repeatedly-selecting-a-prefab-asset-in-the-project-browser))

- `着色器`: 修复了 Material.GetTexturePropertyNameIDs 在处理材质变体时返回空值的问题。
    ([UUM-85842](https://issuetracker.unity3d.com/issues/an-empty-list-is-incorrectly-returned-for-material-variant-when-using-material-dot-gettexturepropertynameids))

- `着色器`: 着色器检查器中的“编译并显示代码”下拉菜单现已加宽，以避免元素重叠。
    ([UUM-143195](https://issuetracker.unity3d.com/issues/shader-inspector-compile-and-show-code-popup-clips-menu-item-text-and-overlaps-the-show-button-with-the-variants-included-label))

- `着色器`: 当处理大型着色器时，"编译并显示代码"下拉菜单不再导致编辑器卡死，因为我们避免了对每个着色器阶段的每个关键字进行遍历以计算 "包含变体" 的数量。
    ([UUM-141740](https://issuetracker.unity3d.com/issues/compile-and-show-code-dropdown-freezes-the-editor-for-a-long-time))

- `TextMeshPro`: 修复了 TMP 着色器始终使用 HDR 颜色选择器，而非匹配着色器中设置的颜色模式的问题。
    ([UUM-141742](https://issuetracker.unity3d.com/issues/the-eyedropper-tool-selects-an-incorrect-value-when-sampling-a-tmp-text-objects-face-or-outline-color-from-the-game-view))

- `URP`: 修复了帧调试器内存占用过高的回归问题。
    ([UUM-139160](https://issuetracker.unity3d.com/issues/frame-debugger-excessive-memory-usage-regression))

- `URP`: 修复了在 Frame Debugger 中展开“纹理”折叠面板时纹理预览图标缺失的问题。
    ([UUM-134917](https://issuetracker.unity3d.com/issues/texture-preview-icons-are-missing-in-frame-debugger-when-expanding-textures-foldout))

- `Video`: 修复了由异步调度器算法问题引发的回归问题。
    ([UUM-140747](https://issuetracker.unity3d.com/issues/audiosampleprovider-buffer-overflow-warnings-are-thrown-when-any-video-is-played-in-play-mode))




## 6000.0.77f1 版本中的包变更

## 已更新的包

- `com.unity.collections`: [2.6.6](https://docs.unity3d.com/Packages/com.unity.collections@2.6//changelog/CHANGELOG.html) 更新至 [2.6.7](https://docs.unity3d.com/Packages/com.unity.collections@2.6//changelog/CHANGELOG.html)

- `com.unity.entities`: 从 [1.4.6](https://docs.unity3d.com/Packages/com.unity.entities@1.4//changelog/CHANGELOG.html) 更新至 [1.4.7](https://docs.unity3d.com/Packages/com.unity.entities@1.4//changelog/CHANGELOG.html)

- `com.unity.netcode`: 从 [1.13.1](https://docs.unity3d.com/Packages/com.unity.netcode@1.13//changelog/CHANGELOG.html) 更新至 [1.13.2](https://docs.unity3d.com/Packages/com.unity.netcode@1.13//changelog/CHANGELOG.html)

- `com.unity.entities.graphics`: 从 [1.4.19](https://docs.unity3d.com/Packages/com.unity.entities.graphics@1.4//changelog/CHANGELOG.html) 更新至 [1.4.20](https://docs.unity3d.com/Packages/com.unity.entities.graphics@1.4//changelog/CHANGELOG.html)

- `com.unity.services.wire`: 从 [1.4.2](https://docs.unity3d.com/Packages/com.unity.services.wire@1.4//changelog/CHANGELOG.html) 至 [1.4.4](https://docs.unity3d.com/Packages/com.unity.services.wire@1.4//changelog/CHANGELOG.html)

- `com.unity.test-framework.performance`: 从 [3.4.0](https://docs.unity3d.com/Packages/com.unity.test-framework.performance@3.4//changelog/CHANGELOG.html) 更新至 [3.5.0](https://docs.unity3d.com/Packages/com.unity.test-framework.performance@3.5//changelog/CHANGELOG.html)

- `com.unity.xr.interaction.toolkit`: [3.0.10](https://docs.unity3d.com/Packages/com.unity.xr.interaction.toolkit@3.0//changelog/CHANGELOG.html) 至 [3.0.11](https://docs.unity3d.com/Packages/com.unity.xr.interaction.toolkit@3.0//changelog/CHANGELOG.html)

- `com.unity.addressables.android`: [1.0.10](https://docs.unity3d.com/Packages/com.unity.addressables.android@1.0//changelog/CHANGELOG.html) 升级至 [1.1.0](https://docs.unity3d.com/Packages/com.unity.addressables.android@1.1//changelog/CHANGELOG.html)