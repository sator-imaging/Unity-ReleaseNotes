# Unity 6000.3.24f1 LTS
发布于 2026年9月10日 星期四 14:47:57 GMT  
https://unity.com/releases/editor/whats-new/6000.3.24f1

# 6000.3.24f1 中的已知问题

- `6000.3.0a1`: 当启用“光晕”效果且使用 2D 渲染器时，会出现黑屏
    ([UUM-150232](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150232))

- `6000.6.0a3、6000.5.0b8、6000.3.16f1`: 在 D3D12 环境下，若在调用 ShaderWarmup.WarmupShaderFromCollection() 后立即卸载着色器，将因“释放后使用”（use-after-free）导致播放器崩溃
    ([UUM-149781](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149781))

- `文本（TextMeshPro）`: 在 TMPro 字体资源生成器中生成多线程字体图集时，UNITY_FT_Load_Glyph 操作会导致崩溃
 ([UUM-125366](https://issuetracker.unity3d.com/issues/crash-on-unity-ft-load-glyph-when-generating-multi-threaded-font-atlas-in-tmpro-font-asset-creator))

当有多个 bee_backend 实例同时运行时，在调用 mono_log_write_logfile 时发生崩溃
    ([UUM-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))

生成字体图集时发生崩溃，并产生多个堆栈跟踪
    ([UUM-141061](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-generating-font-atlas-with-sdf16-or-sdf32))



# 6000.3.24f1 发布说明

## 改进

- `着色器`: 通过“材质集\[类型\] API 会将材质标记为已修改。



## 修复

- `AI`: 修复了在烘焙包含会导致边界极大的对象的导航网格时，编辑器崩溃的问题。
    ([UUM-134462](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-134462))

- `Android`: 修正了 Android 版本标签，使其符合 Google 的命名规范。
    (UUM-150412)

- `Android`: 修复了在 Android 系统中设置“Run Without Focus”时，WebCamTexture 无法恢复的问题。
    (UUM-149681)

- `音频`: 修复了在“播放模式”退出时，若可脚本化处理器在释放阶段从实时回调中读取管道数据，会记录错误日志的问题。
    ([UUM-141072](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-141072))

- `音频`: 修复了暂停包含仍在加载中的流式剪辑的 AudioRandomContainer 时发生的崩溃问题。
    (UUM-148440)

- `音频`: 修复了重置音频设置后，部分音频片段的 LoadState 状态无效的问题。
    ([UUM-147700](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147700))

- `代码编辑器`: 修复了“首选项”>“外部工具”中的“重置参数”按钮，使其能够立即更新“外部脚本编辑器参数”字段，而非仅在焦点切换后才更新。
    (UUM-150210)

- `编辑器`: 修复了通过卸载 Unity 场景删除 MeshCollider 组件时可能发生的卡死问题。
    ([UUM-149370](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149370))

- `编辑器`: 修复了在检查 TextMeshPro 字体资源时导致编辑器崩溃的问题。
    ([UUM-145753](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-145753))

- `编辑器`: 修复了在粒子系统中设置关键帧数量超过 8 个的曲线时，编辑器会崩溃的问题。
    ([UUM-144792](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-144792))

- `编辑器`: 修复了访问叠加层容器的 `rootVisualElement` 可能导致递归调用并使编辑器崩溃的问题。
    ([UUM-149209](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149209))

- `编辑器`: 修复了在 INspector 的“添加组件 - 新脚本”视图中按下 **Enter** 键后脚本未被创建的问题。
    ([UUM-149682](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149682))

- `编辑器`: 修复了浮动视频片段检查器预览错误及外观警告。
    ([UUM-147192](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147192))

- `编辑器`: 修复了 `Vector4` 检查器中“W”分量标签被截断为“...”的问题。
    ([UUM-143161](https://issuetracker.unity3d.com/issues/shadergraph-graph-inspector-vector4-w-label-is-always-truncated-to-dot-dot-dot))

- `编辑器`: 移除了在新建项目中“打开最近场景”下拉菜单中显示的“路径缺失或无效\(\)”提示。 \(\[UUM-113848\]\(https://jira.unity3d.com/browse/UUM-113848\)\)。
    ([UUM-113848](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-113848))

- `编辑器`: 搜索：修复了在启用编辑模式分析器记录的情况下创建脚本时，“SearchImporter.IndexingRequest”会抛出“Profiler.EndSample 不匹配”错误的问题。
    ([UUM-143780](https://issuetracker.unity3d.com/issues/non-matching-profiler-dot-endsample-error-is-thrown-for-searchimporter-dot-indexingrequest-when-creating-a-script-with-edit-mode-profiler-recording-enabled))

- `EmbeddedLinux`: 修复了首次触摸输入丢失的问题。
    (UUM-150086)

- `Graphics`: 修复了在大型场景中烘焙遮挡剔除时发生的崩溃问题。
    ([UUM-143361](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-143361))

- `图形`: 修复了当 Blit 类型设置为“自动”时，Midgard Mali GPU 设备会冻结的问题。
    (UUM-149414)

- `图形`: 修复了 Vulkan 播放器不遵循 'PlayerSettings.vulkanNumSwapchainBuffers' 设置值，而是固定使用 3 个交换链缓冲区的问题。
    (UUM-148724)

- `图形`: 修复了在使用 OpenGL ES 时，因与每种材质（Material）相关的常量缓冲区相关的内存错误导致的崩溃。
    (UUM-150590)

- `图形`: 质量设置——为默认平台添加了省略号，并为名称过长的质量级别添加了质量级别标题。
    ([UUM-148889](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-148889))

- `HDRP`: 修复了启用“光照贴图双立方采样”时着色器筛选错误的问题。
    ([UUM-134794](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-134794))

- `IMGUI`: 修复了当属性矩形位于负 GUI 坐标时，属性字段的子字段无法渲染的问题。
    ([UUM-149255](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149255))

- `iOS`: 修复了连接鼠标时 ScrollView 无法响应鼠标滚轮输入的问题。
    ([UUM-141279](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-141279))

- `Linux`: 修复了首次触摸输入丢失的情况。
    (UUM-150086)

- `Linux`: 将 glibc 版本降至 2.34。
    (UUM-150342)

- `物理引擎`: 修复了 PhysX 4 SDK 中的一个问题，该问题导致 CharacterController 无法同时与超过 100 个形状发生碰撞。
    ([UUM-132204](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-132204))

- `物理`: 优化了销毁 Collider 时 IgnoreCollision 的清理性能。
    ([UUM-115186](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-115186))

- `Physics 2D`: 在激活包含 Collider2D 的子 GameObject 时唤醒 Rigidbody2D。
    ([UUM-149852](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149852))

- `QNX`: 修复了首次触摸输入被丢失的情况。
    (UUM-150086)

- `uGUI`: 修复了在查看 TMP 字体资源时可能发生的崩溃问题，该资源的 **图集填充模式** 设置为 **静态** 且启用了 **多图集纹理**，同时其材质预览处于可见状态。
    ([UUM-145753](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-145753))

- `uGUI`: 修复了当大型文本（TMP）GameObject 的“溢出”属性设置为“省略号”时抛出的 `IndexOutOfRangeException` 异常。
    ([UUM-134477](https://issuetracker.unity3d.com/issues/indexoutofrangeexception-索引-超出-数组-边界-当-大型-Text \(TMP\) GameObject-的-溢出-字段-设置为-省略号-时-会-抛出-错误))

- `uGUI`: 抑制了因 TMP_FontAsset.fontWeight 中未使用的赋值而产生的编译器警告。
    (UUM-137669)

- `UI Toolkit`: 修复了在“质量”设置中将“各向异性纹理”设为“强制开启”时，使用“镜像”或“环绕”地址模式的渐变中出现的白色线条 artifacts，并修复了渐变起始点之前区域的渲染错误。
    ([UUM-139509](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-139509))

- `URP`: 修复了在某些 Android 设备上使用 Vulkan 时，启用深度法线会导致画面出现异常的问题。
    ([UUM-133583](https://issuetracker.unity3d.com/issues/android-vulkan-visual-artifacts-when-using-depth-normals-with-vulkan-api))

- `版本控制`: 修复了编辑器启动时引发“UpdateSettings：未知版本控制插件：XYZ”版本控制错误的竞争条件。
    ([UUM-149884](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149884))

- `VFX 图`: 解决了 NaN 值可能导致图长期处于“脏”状态的问题。
    ([UUM-139398](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-139398))

- `VFX Graph`: 修复了 URP 中的视锥体剔除问题。
    ([UUM-138375](https://issuetracker.unity3d.com/issues/vfx-graph-particles-are-not-culled-when-using-urp-and-frustum-culling-is-enabled-on-vfx-mesh-output))

- `VFX Graph`: 当前一个和下一个切线相互抵消时，防止条带中出现 NaN。
    ([UUM-141608](https://issuetracker.unity3d.com/issues/nan-normals-produced-when-using-custom-y-mode-in-an-orient-node-of-a-vfx-graph))

- `Video`: 修复了在启用 NVIDIA “快速”垂直同步时，Direct3D 环境下视频在调用 Stop\(\) 后无法重播的问题（解码设备丢失且无法恢复）。
    ([UUM-135548](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-135548))

- `视频`: 修复了 WebM Vorbis 音频轨道报告 0 Hz 和 0 个声道的问题。
    (UUM-144045)

- `XR`: 修复了 XR 平台上可能出现的块状或偏移的光照伪影，尤其是在延迟渲染或前向+渲染路径中使用动态分辨率时。
    (UUM-143709)

- `XR`: 修复了在启用深度纹理提交的情况下，运行时更改 MSAA 级别时 XR 图形会冻结的问题。




## 6000.3.24f1 版本中的包变更

## 已更新的包

- `com.unity.netcode`: 从 [1.14.1](https://docs.unity3d.com/Packages/com.unity.netcode@1.14//changelog/CHANGELOG.html) 更新至 [1.14.2](https://docs.unity3d.com/Packages/com.unity.netcode@1.14//changelog/CHANGELOG.html)

- `com.unity.charactercontroller`: 从 [1.4.1](https://docs.unity3d.com/Packages/com.unity.charactercontroller@1.4//changelog/CHANGELOG.html) 更新为 [1.4.5](https://docs.unity3d.com/Packages/com.unity.charactercontroller@1.4//changelog/CHANGELOG.html)

- `com.unity.services.wire`: 从 [1.4.4](https://docs.unity3d.com/Packages/com.unity.services.wire@1.4//changelog/CHANGELOG.html) 更新至 [1.5.0](https://docs.unity3d.com/Packages/com.unity.services.wire@1.5//changelog/CHANGELOG.html)

- `com.unity.terrain-tools`: 从 [5.3.2](https://docs.unity3d.com/Packages/com.unity.terrain-tools@5.3//changelog/CHANGELOG.html) 更新至 [5.3.3](https://docs.unity3d.com/Packages/com.unity.terrain-tools@5.3//changelog/CHANGELOG.html)

- `com.unity.netcode.gameobjects`: 从 [2.13.1](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@2.13//changelog/CHANGELOG.html) 更新至 [2.13.2](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@2.13//changelog/CHANGELOG.html)

- `com.unity.multiplayer.tools`: 从 [2.2.10](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@2.2//changelog/CHANGELOG.html) 更新至 [2.2.11](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@2.2//changelog/CHANGELOG.html)

- `com.unity.services.multiplayer`: 从 [2.3.0](https://docs.unity3d.com/Packages/com.unity.services.multiplayer@2.3//changelog/CHANGELOG.html) 更新至 [2.3.1](https://docs.unity3d.com/Packages/com.unity.services.multiplayer@2.3//changelog/CHANGELOG.html)