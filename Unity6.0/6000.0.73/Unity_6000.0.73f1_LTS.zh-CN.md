# Unity 6000.0.73f1 LTS
发布于 星期三, 15 四月 2026 08:22:53 GMT
https://unity.com/releases/editor/whats-new/6000.0.73f1

# 6000.0.73f1 中的已知问题

- `6000.5.0a4,6000.0.66f1,6000.3.4f1,6000.4.0b4`: 在 Builds 中，ShaderVariantCollection.variantCount 和 ShaderVariantCollection.shaderCount 返回 0
    ([uum-137398](https://issuetracker.unity3d.com/issues/shadervariantcollection-dot-variantcount-and-shadervariantcollection-dot-shadercount-returns-0-in-builds))

- `IL2CPP`: [iOS] [Android] 在构建 IL2CPP 时外部类库失败
    ([uum-125284](https://issuetracker.unity3d.com/issues/ios-android-external-library-generics-fail-during-il2cpp-build))

- 金属命令缓冲区超时错误后游戏冻结
    ([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- `金属"`: MacOS 在编辑器中的最小项目在播放模式下出现卡顿
    ([uum-85256](https://issuetracker.unity3d.com/issues/macos-stutters-in-a-minimal-project))

在 List<T> 结构中使用嵌套 [SerializeReference] 字段时，"core::base_hash_set "崩溃
    ([uum-139722](https://issuetracker.unity3d.com/issues/crash-on-core-base-hash-set-when-using-nested-serializereference-fields-in-list-structures))

使用 DX12 时，在场景视图中选择游戏对象时 CheckDeviceStatus 崩溃
    ([uum-138597](https://issuetracker.unity3d.com/issues/crash-on-checkdevicestatus-when-selecting-gameobjects-in-the-scene-view-while-using-dx12))

当 ConfigurableJoint 使用 JointProjectionMode.PositionAndRotation 且连接的 Rigidbody 从运动式切换为非运动式时，在 ConstraintProjectionTree::projectionTreeBuildStep 上崩溃
    ([uum-135394](https://issuetracker.unity3d.com/issues/crash-on-constraintprojectiontree-projectiontreebuildstep-when-configurablejoint-uses-jointprojectionmode-dot-positionandrotation-and-connected-rigidbody-switches-from-kinematic-to-non-kinematic))

在空白 URP 项目中重新编译时，VisualElement 中的编辑器内存泄漏
    ([uum-138000](https://issuetracker.unity3d.com/issues/editor-memory-leak-in-visualelement-when-recompiling-in-a-blank-urp-project))



# 6000.0.73f1 发行说明

## API 更改

- `编辑器已更改`: 在未定义ENABLE_UNITY_COLLECTIONS_CHECKS时，公开 JobHandle.GetHashCode 和 Equals 以及 ==/\!= 操作符。



## 修复

- `2D`: 修正了调色板或画笔名称过长可能会隐藏磁贴调色板中其他 UI 元素的问题。
    ([uum-130336](https://issuetracker.unity3d.com/issues/long-tile-palette-name-breaks-window-ui))

- `2D`: 修正了一个问题，即当切换到名称长度不同的调色板或画笔时，调色板和画笔下拉菜单的大小会发生变化。
    ([uum-132618](https://issuetracker.unity3d.com/issues/tile-palette-dropdown-expands-when-palette-name-is-longer-in-tile-palette-window))

- `2D`: 修正了当删除精灵皮肤时精灵闪烁和绘制调用波动的问题。
    ([uum-132924](https://issuetracker.unity3d.com/issues/draw-call-count-fluctuates-and-frame-debugger-output-flickers-when-viewing-a-psd-based-sprite-skin-with-always-update-disabled-in-game-view))

- `2D`: 修正了使用分隔符折叠磁贴调色板视图并使用画笔视图按钮展开窗口后，磁贴调色板窗口被极度放大的问题。
    ([uum-132739](https://issuetracker.unity3d.com/issues/tile-palette-viewport-becomes-extremely-zoomed-in-after-disabling-a-previously-adjusted-brush-inspector-tab))

- `2D`: 截断目标、调色板和画笔下拉菜单的长目标、调色板和画笔名称。

- `AI`: 修复了半径小、目的地远的代理在绘制调试可视化时崩溃的问题。
    ([uum-133552](https://issuetracker.unity3d.com/issues/crash-on-memcpy-repmovs-when-selecting-navmesh-agent-objects-while-in-play-mode-in-a-specific-scene))

- `DX12`: 通过暂停渲染，减少了在播放器中最小化（通过 Alt-Tab）"独占全屏 "窗口时的严重崩溃。其他模式和图形 API 不受影响。为了获得更好的稳定性，请考虑使用 "FullScreenWindow"（无边框）模式（https://devblogs.microsoft.com/directx/demystifying-full-screen-optimizations/）。
    ([uum-134743](https://issuetracker.unity3d.com/issues/player-crash-when-switching-focus-in-exclusive-fullscreen-mode-with-directx-12))

- 编辑器限制了发布设置/WebAssembly 语言特性的内存设置，使其不能小于 0。
    ([uum-134687](https://issuetracker.unity3d.com/issues/memory-related-fields-in-the-webassembly-language-features-can-be-set-to-the-negative-numbers))

- 编辑器修正了升级 Win64 插件的旧元文件会禁用插件的问题。
    ([uum-137610](https://issuetracker.unity3d.com/issues/win64-cpu-is-set-to-none-when-applying-changes-to-plugin-where-the-meta-has-the-serializedversion-2))

- 编辑器如果无法加载 buildprofilecontext.asset，则重新创建，以确保构建配置文件窗口的正常运行。
    ([uum-136377](https://issuetracker.unity3d.com/issues/nullreferenceexception-and-empty-build-profiles-window-when-buildprofilecontext-dot-asset-contains-invalid-script-reference))

- `编辑器"`: 打开 "构建配置文件 "窗口时，特定的 ScriptableObject 资产名称不再导致警告。
    ([uum-135389](https://issuetracker.unity3d.com/issues/scriptableobject-asset-is-accessed-during-the-lookup-of-build-profiles-when-opening-the-build-profiles-window))

- `图形`: 添加了 SystemInfo.SupportsTypedUAVShaderLoadStoreOnGraphicsFormat\(\) 用于在无人机上进行着色器类型加载/存储时检查指定硬件的格式支持。适用于 DX11 和 DX12。
    (UUM-101875)

- 图形修正了在 Adreno 设备上使用 GPU 换肤时的崩溃问题。
    ([UUM-93243](https://issuetracker.unity3d.com/issues/crash-on-apigles-clearbuffersubdata-when-running-the-player-a-second-time-on-meta-quest-2))

- `图形`: 修复了在某些 Adreno Vulkan 驱动程序上使用未使用顶点属性的着色器时崩溃的问题。
    (UUM-137056)

- `图形`: 修复了 Android 上命令池内存耗尽时发生的崩溃。
    ([UUM-125566](https://issuetracker.unity3d.com/issues/vulkan-the-memory-allocation-increases-rapidly-when-there-are-multiple-three-or-more-real-time-reflection-probes-in-the-scene))

- `图形`: 修正了当在 DirectX11 中使用 camera.SetTargetBuffers\(\) 而不是渲染纹理时，GrabPass 无法正确设置矩形大小的问题。
    ([uum-135889](https://issuetracker.unity3d.com/issues/grabpass-does-not-correctly-set-the-rect-size-when-set-up-with-a-camera-dot-settargetbuffers-instead-of-a-render-texture-in-directx11))

- 图形当使用金属图形 API 时，修正了使用动态分辨率与 STP 升频时的图形损坏问题。
    (UUM-136227)

- 图形当使用 Vulkan 时，修正了某些 Adreno 7xx 驱动程序版本上不正确的 UV。
    ([UUM-126477](https://issuetracker.unity3d.com/issues/android-vulkan-the-uv-quad-is-displayed-incorrectly-with-vulkan-on-a-specific-device))

- `IL2CPP`: 修正 libil2cpp 代码中的 C++ 警告
    (UUM-138294)

- 物理修正了在某些情况下通过 ForceMode.Acceleration 对 Rigidbody 施加加速度，同时限制其旋转时可能引入的 NaN 值。该问题通常会在手动调用 Physics.Simulate 时出现。
    (UUM-103515)

- 着色器修复了保存着色器时偶尔出现的崩溃问题。
    ([UUM-133627](https://issuetracker.unity3d.com/issues/crash-on-enumeratedisabledkeywordsinvariantsarray-or-unity-xxh32-when-rapidly-saving-shadergraph-or-vfxgraph-changes))

- 文字为 UITK 添加了 hideSoftkeyboard 选项，以及同时激活物理键盘和触摸屏键盘的选项。
    (UUM-122340)

- 文字修复了在物理键盘上切换语言无法正常工作的问题。
    ([UUM-130105](https://issuetracker.unity3d.com/issues/android-legacy-tmp-and-ui-toolkit-input-field-language-toggle-to-some-non-latin-alphabet-languages-does-not-work-with-external-keyboard))

- `用户界面工具包`: 在 Microsoft Basic 渲染器上禁用 UITK GPU 性能测试。
    (UUM-137559)

- `用户界面工具包`: 修复了起始颜色为透明时边框颜色过渡不起作用的问题。
    ([UUM-136876](https://issuetracker.unity3d.com/issues/border-is-not-rendered-when-transition-duration-is-set-and-border-color-is-transparent))

- `XR`: 修正了在启用纹理压缩目标时构建和运行 Meta Quest 应用程序的问题。
    ([uum-131974](https://issuetracker.unity3d.com/issues/meta-quest-player-stuck-at-splashscreen-when-build-app-bundle-and-split-application-binary-are-enabled-with-multiple-texture-compression-formats))




## 6000.0.73f1 中软件包的更改

## 更新的软件包

- `com.unity.burst`: [1.8.28](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html) 到 [1.8.29](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html)

- `com.unity.recorder`: [5.1.5](https://docs.unity3d.com/Packages/com.unity.recorder@5.1//changelog/CHANGELOG.html) 到 [5.1.6](https://docs.unity3d.com/Packages/com.unity.recorder@5.1//changelog/CHANGELOG.html)

- `com.unity.services.authentication`: [3.6.0](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.6//changelog/CHANGELOG.html) 到 [3.6.1](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.6//changelog/CHANGELOG.html)

- `com.unity.test-framework.performance`: [3.3.0](https://docs.unity3d.com/Packages/com.unity.test-framework.performance@3.3//changelog/CHANGELOG.html) 到 [3.4.0](https://docs.unity3d.com/Packages/com.unity.test-framework.performance@3.4//changelog/CHANGELOG.html)

- `com.unity.timeline`: [1.8.10](https://docs.unity3d.com/Packages/com.unity.timeline@1.8//changelog/CHANGELOG.html) 到 [1.8.12](https://docs.unity3d.com/Packages/com.unity.timeline@1.8//changelog/CHANGELOG.html)