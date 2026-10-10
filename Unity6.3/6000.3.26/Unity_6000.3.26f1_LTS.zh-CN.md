# Unity 6000.3.26f1 LTS
发布于 2026年10月8日 星期四 13:38:24 GMT  
https://unity.com/releases/editor/whats-new/6000.3.26f1

# 6000.3.26f1 中的已知问题

- `6000.3.0a1,6000.0.51f1`: 当启用“光晕”效果且使用 2D 渲染器时，会出现黑屏
    ([UUM-150232](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150232))

- `6000.3.14f1`: [多人游戏模式] 当使用额外的编辑器实例和 Vulkan 图形 API 进入游戏模式时，游戏模式场景会一直处于“部署中”状态
    ([UUM-154645](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-154645))

- `7000.0.0a5`: 在构建 Addressables 内容时，若使用从 List<T> 派生的序列化类型，调用 mono_class_get_name 时会导致崩溃
    ([UUM-155711](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-155711))

- `7000.0.0a5`: 将项目从 Unity 6 升级至 7000.0.0a5 或更高版本时，在 Scripting::LogExceptionFromManaged 处发生崩溃，并出现“BadImageFormatException: Bad IL format.”致命错误
    ([UUM-156142](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156142))

当有多个 bee_backend 实例同时运行时，在调用 mono_log_write_logfile 时发生崩溃
    ([UUM-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))



# 6000.3.26f1 发布说明

## 功能

- `编辑器`: 为 Simulation Pro 客户端重新添加了 Linux 无头模拟构建目标



## 变更

- `Android`: 将 Android Gradle 插件（AGP）版本从 9.0.0 更新至 9.1.1。



## 修复

- `2D`: 修复了在编辑网格选择的缩放比例/旋转时 TilemapRenderer 闪烁的问题
    ([UUM-146002](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146002))

- `2D`: 修复了 2D 渲染器在放大时使用错误视口尺寸的问题
    ([UUM-151621](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151621))

- `2D`: 修复了当 `SetTiles` 仅更改了瓦片的变换或颜色时，`Tilemap.tilemapPositionsChanged` 和 `tilemapTileChanged` 回调未被调用的问题。
    (UUM-146094)

- `2D`: 修复了当某个瓦片没有法线贴图时，`TilemapRenderer` 会从其他瓦片继承法线贴图的问题。
    ([UUM-145359](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-145359))

- `2D`: 修复了相机排序层纹理分辨率受 2D 渲染器上“渲染比例”设置影响的问题。
    ([UUM-151723](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151723))

- `2D`: 修复了“打开贴图调色板”按钮和“贴图集焦点”下拉菜单未填满其场景视图叠加层全宽的问题。
    ([UUM-151417](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151417))

- `Android`: 修复了在选择目标 API 级别 37 时出现的“无法找到哈希字符串为 android-37 的目标”错误。
    ([UUM-150216](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150216))

- `资源包 (Asset Bundles)`：修复了从另一个资源包中预制体的子对象引用访问到的资源包中实例化预制体时，播放器崩溃的问题。
    (UUM-141605)

- `构建管道`: 修复了使用 -activeBuildProfile 参数启动的顺序命令行构建会为之前处于活动状态的平台编译脚本的问题。
    (UUM-150775)

- `编辑器`: 当 Vulkan 预变换可能旋转投影矩阵时，不再对其进行优化
    ([UUM-150650](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150650))

- `编辑器`: 修复了 Linux 编辑器未将“帮助”和“窗口”菜单锚定在主菜单栏末尾的错误。
    (UUM-113169)

- `编辑器`: 修复了在 Direct3D12 上，当异步着色器编译仍在进行时退出播放模式会导致死锁的问题。
    ([UUM-152966](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-152966))

- `编辑器`: 修复了进入播放模式时账户下拉菜单的显示问题
    ([UUM-150759](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150759))

- `编辑器`: 修复了切换回采用英特尔 32 位架构的 Windows 构建配置文件时，活动构建目标可能仍保留为英特尔 64 位 \(StandaloneWindows64\) 而非英特尔 32 位 \(StandaloneWindows\)。
    ([UUM-143128](https://issuetracker.unity3d.com/issues/windows-platform-architecture-switching-from-intel-32-bit-to-intel-64-bit-in-backend-when-switching-active-build-profile-back-to-windows-from-any-other-platform))

- `编辑器`: 修复了在显示“场景\(s\) 已被修改”对话框时，多次按下 Cmd+Q 会导致编辑器崩溃的问题。<br>
    修复了在“播放”模式下退出编辑器且存在未保存更改时，会显示两个“场景已修改”对话框的问题。<br>
    修复了当订阅了 EditorApplication.quitting 的脚本修改了编辑器窗口时，编辑器在退出时崩溃的问题。<br>
    修复了在编辑器对话框中按 Esc 键无法选择“取消”的问题。
    ([UUM-149668](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149668))

- `GI`: 修复了当场景中包含 VFXRenderer 时 APV 烘焙失败的错误。
    ([UUM-150965](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150965))

- `Graphics`: 修复了一个问题，该问题可能导致 Unity 在启用 GPU Resident Drawer 处理着色器任务时出现内存泄漏警告，主要发生在 macOS 系统上。
    ([UUM-140185](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-140185))

- `IMGUI`: 修复了文本字段在输入内容超过可见字段宽度时（例如在“项目”窗口中重命名资源时），无法滚动以保持光标可见的问题。
    ([UUM-149213](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149213))

- `iOS`: 修复了在具有相同参数的 TMP 输入字段之间切换时，键盘有时会关闭的问题。
    (UUM-149104)

- `macOS`: 修复了 macOS 编辑器在窗口失去焦点时忽略内部时钟请求的问题，该问题导致异步和协程执行速度比获得焦点时更慢。
    (UUM-151097)

- 不适用 \(内部\)：修复了 Android 版 Unity 渲染服务的线性渲染问题
    (UUM-129914)

- `网络`: 修复了当向同一主机发出的较快并发请求已设置了较新 Cookie 后，较慢的请求完成时，UnityWebRequest 的 Cookie 偶尔会恢复为较旧值的现象。
    ([UUM-150958](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150958))

- `网络`: UnityWebRequest：修复了在独立播放器退出时，若正在进行的请求仍在针对无响应或响应缓慢的 DNS 服务器进行 DNS 解析，会导致程序卡死的问题。
    ([UUM-151643](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151643))

- `播放器`: 在运行时修改 Shader.globalMaximumLOD 后，GameObject 会投射正确的阴影。
    ([UUM-150226](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150226))

- `Profiler`: 修复了保存空的独立运行版分析器录制文件时抛出的 NullReferenceException 异常。
    ([UUM-150588](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150588))

- `Profiler`: 修复了与 GraphicsStateCollection 分配相关的未根结分配的标签问题。
    ([UUM-139555](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-139555))

- `Profiler`: 修复了 Profiler 中“排查连接问题”按钮链接到与连接故障排除无关的文档页面的问题。
    ([UUM-153354](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-153354))

- `着色器`: 修复了因向着色器全局属性 API 提供超出范围的值而导致的崩溃问题。
    ([UUM-150856](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150856))

- `Terrain`: 修复了加载高度图分辨率超过设备最大渲染纹理大小的地形时发生的崩溃问题，例如在最大渲染纹理大小限制为 4096 的设备上加载 4097 分辨率的高度图。
    ([UUM-150551](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150551))

- `Text`: 修复了多段落自动调整大小的文本会折叠为省略第一行，而非缩小以适应显示区域的问题。
    (UUM-150602)

- `uGUI`: 修复了 WorldDocumentRaycaster.camera 中多余的 'new' 关键字引发的编译器警告。
    ([UUM-151722](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151722))

- `UI Toolkit`: 修复了当某个祖先节点的缩放值从零开始动画放大后，若另一个祖先节点使用了 GroupTransform 使用提示，则带有 DynamicTransform 使用提示的 VisualElement 直到鼠标悬停时才会显示的问题。
    ([UUM-140869](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-140869))

- `UI 工具包`: 修复了 SVG 渐变的 xlink:href 继承问题。
    ([UUM-150193](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150193))

- `UI Toolkit`: 修复了嵌套 svg 标签导致的 SVG 导入错误。
    ([UUM-150948](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150948))

- `URP`: 修复了重新加载场景会导致某些 `Blitter` 函数停止工作的错误。
    (UUM-153092)

- `URP`: 修复了因 uv4 输入语义差异导致的 ShaderGraph 编译失败问题。
    ([UUM-143884](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-143884))

- `URP`: 修复了在采用半精度（\(mobile\)）的平台上的盒形投影反射探针中出现接缝的错误的平台上，盒形投影反射探针上会出现接缝。
    ([UUM-141981](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-141981))

- `URP`: 当 UberPost \(后处理\) 作为最终渲染通道时，通过避免不必要的颜色加载，提升了基于瓦片平台的 URP 项目的 GPU 性能。
    (UUM-140408)

- `Web`: 修复了当输出资源大小超过 2 GB 时 Web 平台的构建问题，以及输出资源大小超过 4 GB 时出现的构建错误提示（不支持）。
    ([UUM-112909](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-112909))




## 6000.3.26f1 版本中的包变更

## 已更新的包

- `com.unity.netcode`: [1.14.2](https://docs.unity3d.com/Packages/com.unity.netcode@1.14//changelog/CHANGELOG.html) 更新至 [1.14.3](https://docs.unity3d.com/Packages/com.unity.netcode@1.14//changelog/CHANGELOG.html)

- `com.unity.mobile.notifications`: 从 [2.4.3](https://docs.unity3d.com/Packages/com.unity.mobile.notifications@2.4//changelog/CHANGELOG.html) 更新至 [2.5.0](https://docs.unity3d.com/Packages/com.unity.mobile.notifications@2.5//changelog/CHANGELOG.html)

- `com.unity.services.authentication`: 从 [3.7.4](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.7//changelog/CHANGELOG.html) 更新至 [3.8.0](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.8//changelog/CHANGELOG.html)

- `com.unity.services.cloud-build`: 从 [2.0.8](https://docs.unity3d.com/Packages/com.unity.services.cloud-build@2.0//changelog/CHANGELOG.html) 更新至 [2.1.0](https://docs.unity3d.com/Packages/com.unity.services.cloud-build@2.1//changelog/CHANGELOG.html)

- `com.unity.services.friends`: 从 [1.1.1](https://docs.unity3d.com/Packages/com.unity.services.friends@1.1//changelog/CHANGELOG.html) 更新至 [1.3.0](https://docs.unity3d.com/Packages/com.unity.services.friends@1.3//changelog/CHANGELOG.html)

- `com.unity.services.wire`: 从 [1.5.1](https://docs.unity3d.com/Packages/com.unity.services.wire@1.5//changelog/CHANGELOG.html) 升级至 [1.6.0](https://docs.unity3d.com/Packages/com.unity.services.wire@1.6//changelog/CHANGELOG.html)

- `com.unity.netcode.gameobjects`: 从 [2.13.2](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@2.13//changelog/CHANGELOG.html) 更新至 [2.13.3](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@2.13//changelog/CHANGELOG.html)

- `com.unity.multiplayer.tools`: 从 [2.2.11](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@2.2//changelog/CHANGELOG.html) 更新至 [2.2.12](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@2.2//changelog/CHANGELOG.html)

- `com.unity.ai.navigation`: 从 [2.0.14](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html) 更新至 [2.0.15](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html)

- `com.unity.dt.app-ui`: 从 [2.1.1](https://docs.unity3d.com/Packages/com.unity.dt.app-ui@2.1//changelog/CHANGELOG.html) 更新至 [2.2.4](https://docs.unity3d.com/Packages/com.unity.dt.app-ui@2.2//changelog/CHANGELOG.html)

- `com.unity.services.multiplayer`: 从 [2.3.1](https://docs.unity3d.com/Packages/com.unity.services.multiplayer@2.3//changelog/CHANGELOG.html) 更新至 [2.3.3](https://docs.unity3d.com/Packages/com.unity.services.multiplayer@2.3//changelog/CHANGELOG.html)

- `com.unity.asset-manager-for-unity`: 从 [1.11.0](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.11//changelog/CHANGELOG.html) 升级至 [1.12.0](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.12//changelog/CHANGELOG.html)