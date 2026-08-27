# Unity 6000.3.23f1 LTS
发布于 2026年8月26日 星期三 14:35:12 GMT  
https://unity.com/releases/editor/whats-new/6000.3.23f1

# 6000.3.23f1 中的已知问题

- `2021.3.34f1`: 播放模式下调节音量时音频混音器会发出咔嗒声
    ([UUM-150250](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150250))

- `6000.6.0a3,6000.5.0b8,6000.3.16f1`: 在 D3D12 环境下，当在调用 ShaderWarmup.WarmupShaderFromCollection() 后立即卸载着色器时，播放器会因“释放后使用”问题而崩溃
    ([UUM-149781](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149781))

- `文本（TextMeshPro）`: 在 TMPro 字体资源生成器中生成多线程字体图集时，UNITY_FT_Load_Glyph 会引发崩溃 
 ([UUM-125366](https://issuetracker.unity3d.com/issues/crash-on-unity-ft-load-glyph-when-generating-multi-threaded-font-atlas-in-tmpro-font-asset-creator))

当运行多个 bee_backend 实例时，在调用 mono_log_write_logfile 时发生崩溃
    ([UUM-142773](https://issuetracker.unity3d.com/issues/当运行多个 bee_backend 实例时 mono_log_write_logfile 发生崩溃))

生成字体图集时发生崩溃，并产生多个堆栈跟踪
    ([UUM-141061](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-generating-font-atlas-with-sdf16-or-sdf32))



# 6000.3.23f1 发布说明

## 改进

- `文档`: 在 MonoBehaviour.OnValidate 脚本参考中，明确说明了 OnValidate 设置的值何时会被保存，以及何时仅存在于内存中。
    ([UUM-134473](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-134473))



## 变更

- `安装程序`: 在 Windows 编辑器安装程序中添加了 -CPULightmapper=no 命令行开关，用于跳过仅由 CPU 渐进式光照贴图器所需的组件的安装，目前该组件为已停止维护的 Microsoft Visual C++ 2010 运行时。
    (UUM-149122)

- `Mono`: 从 ToFileDescriptor 中移除了断言
    ([UUM-145761](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-145761))



## 修复

- `2D`: 修复了在 3D 编辑器模式下，将纹理作为 Sprite 导入时，Sprite 生成功能未生成 Sprite 子资源的问题。
    ([UUM-142920](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-142920))

- `2D`: 修复了在 Sprite 编辑器窗口发生更改后进入快速播放模式时出现的错误提示。
    ([UUM-146790](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146790))

- `无障碍功能`: 修复了 Narrator（Windows 内置屏幕阅读器）不支持 `AssistiveSupport.screenReaderStatusChanged` 的问题。
    ([UUM-147175](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147175))

- `AI`: 由于配置不兼容，NavMeshAgent 会尝试通过向任意方向跳跃来脱离其自身的 NavMeshObstacle 组件。现在，该代理会朝一个稳定的方向移动。
    (UUM-141803)

- `AI`: 在箱形 NavMeshObstacle 内部创建或传送的 NavMeshAgent 无法移动出障碍物。
    ([UUM-146477](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146477))

- `Android`: 修复了 Android 外部工具设置面板中的对齐问题。
    (UUM-148378)

- `资源管道`: 修复了在进入“播放模式”时，`WriteObjectToVector` / `CreateOrReloadInspectorCopy` 可能导致编辑器崩溃的问题。
    ([UUM-112617](https://issuetracker.unity3d.com/issues/editor-crashes-on-unity-writeobjecttovector-when-entering-into-the-play-mode))

- `构建管道`: 在“内存设置”中（“主分配器” > “其他分配器” > “Remapper 初始容量”）增加了预留 PersistentManager.Remapper 容量的支持。
    (UUM-136275)

- `DX12`: 修复了在 Windows 系统上使用 Direct3D12 图形 API 时，小纹理被销毁后其占用的 VRAM 未释放回 GPU 驱动程序的问题。<br>
    现在，您可以通过 `d3d12-small-texture-tiles-per-heap` 启动配置参数调整小纹理堆大小，以在 VRAM 回收与堆分配开销之间取得平衡。
    ([UUM-142284](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-142284))

- `DX12`: 当动态缩放渲染目标在分辨率切换时对其共享放置堆进行重新抗锯齿处理时，HDRP 硬件动态分辨率不再产生亮像素瑕疵，也不会引发 D3D12 验证错误 1422。
    ([UUM-108671](https://issuetracker.unity3d.com/issues/visual-artifacts-appear-when-the-hd-dynamic-resolution-component-changes-the-resolution-scale))

- `编辑器`: 修复了在 ATG 中使用“源字体文件”缺失的备用方案时导致的崩溃问题。
    (UUM-148158)

- `编辑器`: 修复了 `services-gateway` 备用 URL 中的拼写错误，该错误可能导致当远程配置 CDN 不可达时，通过 Hub 启动的编辑器无法登录或云服务出现故障。
    (UUM-149207)

- `Editor`: 修复了在复制操作过程中尝试删除不存在的资源的问题。
    ([UUM-144993](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-144993))

- `Editor`: 修复了在构建过程中与加速器断开连接时导致的崩溃问题。
    ([UUM-148391](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-148391))

- `Editor`: 修复了在上下文模式下查看继承样式表时，样式表与所属文档名称之间缺少空格的问题。
    ([UUM-147743](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147743))

- `编辑器`: 修复了在导入或转码带有“裁剪”和“偏移”设置的视频时，Windows 版编辑器崩溃的问题。
    ([UUM-146426](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146426))

- `Editor`: 强化了 Hub 模式服务配置处理的内部安全性。用户可见的行为没有变化。
    (UUM-149208)

- `Editor`: ScreenCapture.CaptureScreenshotAsTexture\(\) 渲染的屏幕截图带有边框。
    ([UUM-130878](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-130878))

- `Editor`: 在 URP 和 HDRP 模板中禁用 GRD。
    ([UUM-143179](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-143179))

- `编辑器`: 在 MPPM 克隆处于活动状态时更新包会导致克隆崩溃。
    (UUM-148292)

- `EmbeddedLinux`: 修复了系统中不存在 `wl_seat` 时发生的崩溃问题。
    (UUM-148754)

- `GI`: 修复了在包含大型地形的场景中，将“照明可视化”叠加层的“照明数据”切换为“预览”模式时发生的崩溃及打包时间过长的问题。
    ([UUM-149471](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149471))

- `GI`: 修复了在包含足够大（以至于被拆分为多个光照贴图实例）的地形场景中使用交互式光照预览时，编辑器会崩溃的问题。
    (UUM-148850)

- `GI`: 修复了为放置在 StreamingAssets 中的场景烘焙光照时发生的崩溃问题。
    ([UUM-149240](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149240))

- `GI`: 修复了因对象没有有效的光照贴图 UV 坐标，导致其在烘焙光照时被移除，并伴随“网格 UV 布局中的每个三角形面积为零”警告的问题。
    ([UUM-148666](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-148666))

- `GI`: 修复了当未安装 Microsoft Visual C++ 2010 运行时，Windows 编辑器无法启动的问题；现在，CPU 渐进式光照贴图器会报告该功能不可用。
    (UUM-149122)

- `Graphics`: 为 `Resolution` 和 `RefreshRate` 添加了 `IEquatable<T>`、`GetHashCode` 以及相等运算符，以避免在比较这些值或将其用作字典键时触发垃圾回收分配。
    (UUM-146197)

- `Graphics`: 仅允许在通用渲染器上使用“按瓦片后处理”功能。
    ([UUM-148038](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-148038))

- `Graphics`: 启用 GRD 后，对 staticShadowCaster 的更改现可正确更新。
    ([UUM-140724](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-140724))

- `Graphics`: 修复了在使用 XR 并启用“最小化 Unity '屏幕' 尺寸”优化时，mipmap 级别计算不正确的问题。<br>
    在 XR 模式下，相机矩形现在会正确返回单眼尺寸，而非 SRP 模式下的立体组合尺寸。这会影响任何依赖相机矩形进行分辨率相关计算的系统，包括 Mipmap 流式传输以及基于分辨率的用户界面/文本渲染。如有需要，请调整 Mipmap 流式传输设置或用户界面缩放比例。
    ([UUM-47681](https://issuetracker.unity3d.com/issues/calculated-mipmap-level-does-not-taking-xr-resolution-into-account))

- `图形`: 图形设置 - “从当前场景导入”操作未添加到撤销列表中。
    ([UUM-148881](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-148881))

- `Graphics`: 从 URP 核心包中移除了 unifiedraytracing 资源包。
    ([UUM-135643](https://issuetracker.unity3d.com/issues/newly-created-project-contains-a-unifiedraytracing-assetbundle-when-universal-or-high-definition-templates-are-used))

- `输入系统`: 修复了 Windows 系统上一个错误：当 HID 设备具有较大的供应商定义报告（例如 `ReportCount=1024`）时，由于会输出重复的描述符元素，可能会生成巨大的设备 `capabilities` 字符串。现在描述符大小已恢复正常，且设备实际的控制功能不受影响。
    (UUM-144506)

- `许可证`: 修复了导入指定用户许可证文件时手动许可证激活失败的问题。

- `多人游戏`: 当启用 GPU 驻留抽屉且克隆对象的渲染组件被专用服务器角色移除时，编辑器会崩溃。
    ([UUM-147692](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147692))

- `网络`: 当 Web 请求被突然终止时，会解引用无效的纹理指针。
    ([UUM-144540](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-144540))

- `网络`: 修复了在编辑器中长时间会话（涉及多次域名刷新）时，若使用自定义证书处理程序配合 UnityWebRequest，可能导致编辑器崩溃的问题。
    ([UUM-147347](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147347))

- `包管理器`: 当选中多个资源或所选资源不是 UPM 包时，已禁用“导出 UPM 包”选项。
    ([UUM-135090](https://issuetracker.unity3d.com/issues/multi-select-is-not-handled-correctly-when-exporting-packages-in-the-project-window))

- `Shadergraph`: 修复了用于选择自定义节点颜色的颜色选择器。
    ([UUM-114854](https://issuetracker.unity3d.com/issues/could-not-invoke-color-picker-for-shadergraph-warning-is-thrown-when-changing-the-node-color-in-the-user-defined-color-mode))

- `SRP Core`: 修复了 AMDUnityPlugin 以使用静态链接的 CRT。
    (UUM-147060)

- `uGUI`: 修复了检查器中 UGUI/TMP 类的文档链接。
    ([UUM-144450](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-144450))

- `UI Toolkit`: 修复了在世界坐标系 UI 渲染过程中，当内部绘制范围列表在部分已满时继续增长时抛出的 ArgumentException 异常。
    (UUM-149611)

- `UI Toolkit`: 修复了当存在 8 个或更多按钮时，ToggleButtonGroup 值发生循环溢出的问题。
    ([UUM-149531](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149531))

- `UI 工具包`: 修复了 `Painter2D` 和 SVG 笔画中，长度为零的虚线图案条目会报错而非正常渲染的问题，并将长度为零的圆头虚线渲染为点。
    ([UUM-135766](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-135766))

- `版本控制`: 修复了在导入资源后通过 Perforce 获取文件时，未更改的文件会被自动添加到更改列表中的问题。
    ([UUM-49713](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-49713))




## 6000.3.23f1 版本中的包变更

## 已更新的包

- `com.unity.2d.animation`: [13.0.5](https://docs.unity3d.com/Packages/com.unity.2d.animation@13.0//changelog/CHANGELOG.html) 更新为 [13.0.6](https://docs.unity3d.com/Packages/com.unity.2d.animation@13.0//changelog/CHANGELOG.html)

- `com.unity.2d.common`: 从 [12.0.3](https://docs.unity3d.com/Packages/com.unity.2d.common@12.0//changelog/CHANGELOG.html) 更新为 [12.0.4](https://docs.unity3d.com/Packages/com.unity.2d.common@12.0//changelog/CHANGELOG.html)

- `com.unity.2d.tilemap.extras`: 从 [6.0.2](https://docs.unity3d.com/Packages/com.unity.2d.tilemap.extras@6.0//changelog/CHANGELOG.html) 升级至 [6.0.3](https://docs.unity3d.com/Packages/com.unity.2d.tilemap.extras@6.0//changelog/CHANGELOG.html)

- `com.unity.2d.tooling`: 从 [1.0.3](https://docs.unity3d.com/Packages/com.unity.2d.tooling@1.0//changelog/CHANGELOG.html) 更新为 [1.0.4](https://docs.unity3d.com/Packages/com.unity.2d.tooling@1.0//changelog/CHANGELOG.html)

- `com.unity.collab-proxy`: 从 [2.12.4](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.12//changelog/CHANGELOG.html) 更新至 [2.13.6](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.13//changelog/CHANGELOG.html)

- `com.unity.services.authentication`: 从 [3.7.3](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.7//changelog/CHANGELOG.html) 更新至 [3.7.4](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.7//changelog/CHANGELOG.html)

- `com.unity.timeline`: 从 [1.8.12](https://docs.unity3d.com/Packages/com.unity.timeline@1.8//changelog/CHANGELOG.html) 更新至 [1.8.13](https://docs.unity3d.com/Packages/com.unity.timeline@1.8//changelog/CHANGELOG.html)

- `com.unity.xr.management`: 从 [4.5.4](https://docs.unity3d.com/Packages/com.unity.xr.management@4.5//changelog/CHANGELOG.html) 更新至 [4.6.1](https://docs.unity3d.com/Packages/com.unity.xr.management@4.6//changelog/CHANGELOG.html)