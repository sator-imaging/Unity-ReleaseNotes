# Unity 6000.0.75f1 LTS
发布于格林尼治标准时间 2026 年 5 月 13 日星期三 14:51:23
https://unity.com/releases/editor/whats-new/6000.0.75f1

# 6000.0.75f1 中的已知问题

- `6000.0.61f1`: 使用 SDF16 或 SDF32 生成字体图集时 tlsf_free 崩溃
    ([uum-141061](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-generating-font-atlas-with-sdf16-or-sdf32))

- `6000.0.6f1`: [渲染图][D3D12]当使用带有EnableAsyncCompute(true)和UseTexture的AddComputePass时，D3D12SwapChain::Present崩溃。
    ([uum-140183](https://issuetracker.unity3d.com/issues/rendergraph-d3d12-crash-on-d3d12swapchain-present-when-using-addcomputepass-with-enableasynccompute-true-and-usetexture))

- `金属"`: 命令缓冲区超时错误后游戏冻结
    ([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- `金属"`: MacOS 在编辑器中的最小项目在播放模式下出现卡顿
    ([uum-85256](https://issuetracker.unity3d.com/issues/macos-stutters-in-a-minimal-project))



# 6000.0.75f1 发行说明

## 改进

- `AI`: NavMeshHit 结构和相关概念的 API 文档缺少信息。
    (UUM-140847)

- `编译系统`: 将捆绑的 7-Zip 更新至 26.01 版本。

- 编辑器删除了在叠加模式下启用法线或切线时画布组件下的警告。
    ([uum-137367](https://issuetracker.unity3d.com/issues/additional-shader-channel-keeps-reverting-when-saving-prefab))



## API 更改

- `编辑器新增`: 新增公共 DeeplinkHandlerAttribute。



## 修复

- `2D`: 修正了 Hidden/Light2D 中的着色器警告。
    ([uum-134522](https://issuetracker.unity3d.com/issues/shader-warning-in-hidden-slash-light2d-implicit-truncation-of-vector-type-is-thrown-when-building-universal-2d-template))

- `2D`: 修正了一个关于 2D 阴影体积强度的问题。
    ([uum-136056](https://issuetracker.unity3d.com/issues/shadows-from-light2d-do-not-change-when-volumetric-shadow-strength-is-toggled-off))

- `2D`: 修正了当瓦片贴图的瓦片锚点与默认单元格中心不同时， Collider Type Grid 的瓦片无法正确对齐的问题。
    (UUM-136995)

- `2D`: 当使用 URP 2D 时，修复了预览相机中缺失的光照和阴影。
    (UUM-139229)

- 辅助功能修正了当节点ID达到`int.MaxValue`时`AccessibilityHierarchy`抛出异常，以及无障碍节点在最大ID值周围缠绕后以重复ID创建的问题。
    ([uum-137871](https://issuetracker.unity3d.com/issues/accessibilityhierarchy-throws-an-exception-when-node-id-reaches-int-dot-maxvalue))

- `Android`: 修正了当控制器将 L2/R2 报告为按钮事件而非轴事件时，Switch Pro 游戏手柄触发器在 Android 上不起作用的问题。
    (UUM-139567)

- 音频修复了当从资产包（AssetBundle）加载带有音轨的时间线且音频剪辑未能分配 FMOD 通道时，进入播放模式时崩溃的问题。
    ([uum-136551](https://issuetracker.unity3d.com/issues/crash-on-soundchannelinstance-setdelay-when-loading-an-assetbundle-containing-a-timeline-with-an-audioclip-at-scene-startup))

- `构建系统"`: 修正了一个问题，即在预构建回调过程中删除包含程序集的文件夹时，播放器会在启动时崩溃。
    ([uum-137492](https://issuetracker.unity3d.com/issues/player-crashes-upon-launch-when-a-folder-is-deleted-as-a-prebuild-step))

- `DX12`: 修正了大型场景中 D3D12 栅栏的缓慢内存泄漏。
    (UUM-140429)

- `Editor`: 2D: 修复了通过 "SpriteAtlasManager.atlasRequested "加载可寻址的 SpriteAtlas，并启用 Sprite Atlas V2 包装时，在编辑器播放模式中不可见 SpriteSkin 的情况。
    (UUM-137123)

- 编辑器修复了布局表和替换表在域重载之间泄漏的问题。
    ([UUM-138000](https://issuetracker.unity3d.com/issues/editor-memory-leak-in-visualelement-when-recompiling-in-a-blank-urp-project))

- `图形`: 修正了虚拟纹理剖析器模块的帮助按钮在具有多种像素密度的多显示器设置上的缩放问题。
    ([uum-137763](https://issuetracker.unity3d.com/issues/virtual-texturing-documentation-button-is-oversized-and-not-consistent-with-other-editor-documentation-buttons-when-virtual-texturing-module-is-selected-in-the-profiler-window))

- `图形"`: 修正了当为统一缓冲区绑定传递无效绑定槽时 OpenGLES 崩溃的问题。
    (UUM-138897)

- `图形`: 修正了流控制器组件文档的链接。
    ([UUM-139928](https://issuetracker.unity3d.com/issues/missing-documentation-page-opens-when-clicking-open-reference-button-on-streaming-controller-component))

- `图形"`: 修正了虚拟纹理剖析器模块文档的链接。
    ([uum-137763](https://issuetracker.unity3d.com/issues/virtual-texturing-documentation-button-is-oversized-and-not-consistent-with-other-editor-documentation-buttons-when-virtual-texturing-module-is-selected-in-the-profiler-window))

- `图形"`: \[Vulkan\]修正了在深度解析或计算着色器写入 "RenderTexture "后应用不正确的 "DontCare "加载动作，导致出现伪影。
    (UUM-46565)

- `HDRP"`: 修正了一个 Bug，在该 Bug 中，HDRP SSGI 会从屏幕的一侧向另一侧渗色。
    ([UUM-139120](https://issuetracker.unity3d.com/issues/lighting-leaks-from-right-and-top-edges-to-left-and-bottom-edges-when-screen-space-global-illumination-uses-ray-tracing-in-hdrp))

- `iOS`: 修正了多次从 GameCenter 加载成就时崩溃的问题。
    (UUM-138417)

- `iOS`: 进一步改进 UIScene 生命周期事件 - 通用深层链接处理，提前移动 AbsoluteURL 设置以避免在 Awake\(\) 中错过。
    (UUM-140746)

- 内核修正了从终结器访问作业系统时关闭时崩溃的问题。
    ([UUM-128777](https://issuetracker.unity3d.com/issues/crash-on-jobqueue-hasjobgroupidcompleted-when-closing-the-editor-while-in-play-mode-on-a-specific-project))

- `网络`: 在 Linux 播放器构建中添加了一些缺失的 Mono 配置文件，当尝试使用某些 .NET 网络 API 时，这些配置文件会导致异常抛出（尤其是 `WebRequest`\）。
    ([uum-135731](https://issuetracker.unity3d.com/issues/webrequest-dot-create-function-fails-with-uri-prefix-is-not-recognized-errors-when-the-project-is-built-for-linux-standalone-or-windows-dedicated-server))

- 网络修正了 MbedTLS 中的一个回归，当尝试从软件包管理器的 Asset Store 下载资产时，该回归会导致 TLS 握手错误。其他 HTTPS 端点也可能受到此回归的影响。
    (UUM-141298)

- 网络将 MbedTLS 更新至 3.6.6 版，以解决一些（次要且可能无法利用的）安全漏洞。
    (UUM-140908)

- 物理修正了一个问题，即 "Incremental Static Broadphase "的值不会被发送到物理 sdk，从而导致存在大量静态对撞机的设置出现问题。
    (UUM-141093)

- 脚本编写修复了容器中的整数溢出崩溃。
    ([UUM-134628](https://issuetracker.unity3d.com/issues/crash-on-memcpy-when-opening-a-scene-with-specific-assets))

- 着色器修正了在玩家构建中访问 `shaderCount` 和 `variantCount` 时，`ShaderVariantCollection` 返回 0 的问题。
    ([uum-137398](https://issuetracker.unity3d.com/issues/shadervariantcollection-dot-variantcount-and-shadervariantcollection-dot-shadercount-returns-0-in-builds))

- `uGUI`: 修正了在 OnValidate 事件中使用脚本改变输入框焦点时出现 nullReferenceException 的问题。
    ([uum-132637](https://issuetracker.unity3d.com/issues/nullreferenceexception-error-is-thrown-when-changing-input-field-focus-via-script-with-custom-validation))

- `uGUI`: 修正了当使用 Tab 键移动焦点时，InputField 无法获取 Hangul\(IME\) （韩文字符）文本的最后一个字符。
    ([uum-126213](https://issuetracker.unity3d.com/issues/inputfield-fails-to-get-the-last-character-of-a-hangul-ime-korean-character-text-when-focus-is-shifted-with-the-tab-key))

- 视频在基于 Windows 的平台上打开分段 MP4 文件时，添加了控制台警告，因为不支持这种媒体类型。
    ([uum-132004](https://issuetracker.unity3d.com/issues/video-player-does-not-throw-an-error-when-playing-a-video-with-unsupported-encoding-settings))

- `WebGL`: \[WebGPU\] 确保 WebCam 视频在移动设备上方向正确。
    ([uum-139017](https://issuetracker.unity3d.com/issues/ios-web-webgpu-webcamtextures-camera-orientation-is-fixed-relative-to-the-phones-right-edge))

- `XR`: 修正了镜头耀斑的一个 Bug，该 Bug 在不同视图中镜头耀斑的位置相同，从而导致视觉伪影。
    ([uum-108851](https://issuetracker.unity3d.com/issues/lens-flare-vfx-is-duplicated-when-observed-through-a-vr-headset))

- `XR`: 修正了在 URP 中使用多通道 XR 渲染模式时，内置着色器常量 unity_StereoEyeIndex 未正确设置的问题，该问题会影响 Skybox/Panoramic 等着色器，即使使用 3D 布局选项，这些着色器也无法显示为立体效果。
    ([uum-120719](https://issuetracker.unity3d.com/issues/stereoscopic-skybox-renders-as-monoscopic-when-using-multi-pass-render-mode-in-xr-plugin-while-using-urp))




## 6000.0.75f1 中软件包的更改

## 更新的软件包

- `com.unity.netcode`: [1.11.0](https://docs.unity3d.com/Packages/com.unity.netcode@1.11//changelog/CHANGELOG.html) 到 [1.13.1](https://docs.unity3d.com/Packages/com.unity.netcode@1.13//changelog/CHANGELOG.html)

- `com.unity.performance.profile-analyzer`: [1.3.3](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.3//changelog/CHANGELOG.html) 到 [1.3.4](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.3//changelog/CHANGELOG.html)

- `com.unity.services.user-reporting`: [2.0.14](https://docs.unity3d.com/Packages/com.unity.services.user-reporting@2.0//changelog/CHANGELOG.html) 到 [2.0.15](https://docs.unity3d.com/Packages/com.unity.services.user-reporting@2.0//changelog/CHANGELOG.html)

- `com.unity.asset-manager-for-unity`: [1.10.0](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.10//changelog/CHANGELOG.html) 到 [1.11.0](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.11//changelog/CHANGELOG.html)