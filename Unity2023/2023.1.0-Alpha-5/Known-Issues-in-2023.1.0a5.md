# Unity 2023.1.0 Alpha 5

https://unity3d.com/unity/alpha/2023.1.0a5

## Known Issues in 2023.1.0a5



*   2D: \[Lost Crypt\] Unable to find URP 12.1.0 package error when importing Lost Crypt ([1388129](https://issuetracker.unity3d.com/issues/2d-lost-crypt-unable-to-find-urp-12-dot-1-0-package-error-when-importing-lost-crypt))
    
*   AI Navigation Core: Trigger volumes are included in nav mesh generation for NavMeshSurface when geometry is set to Physics Colliders ([UUM-10109](https://issuetracker.unity3d.com/issues/trigger-volumes-are-included-in-nav-mesh-generation-for-navmeshsurface-when-geometry-is-set-to-physics-colliders))
    
*   Android: Workaround for crash on many PowerVR based devices ([UUM-7782](https://issuetracker.unity3d.com/issues/android-urp-project-crashes-when-built-on-a-device-with-powervr-rogue-ge8320-gpu))  
    _Fixed in 2023.1.0a6._
    
*   Asset - Database: Infinite import on opening project (related to prefabs) ([1411189](https://issuetracker.unity3d.com/issues/infinite-import-on-opening-project-related-to-prefabs))
    
*   Editor: Fix hang when dragging first root GameObject below itself in the Hierarchy ([UUM-10504](https://issuetracker.unity3d.com/issues/editor-hangs-when-gameobject-is-dragged-down-and-released-when-blue-line-appears))  
    _First seen in 2023.1.0a5._  
    _Fixed in 2023.1.0a7._
    
*   Editor: Fix Unity Event callback list calculating its height incorrectly (UUM-8350)  
    _First seen in 2023.1.0a1._  
    _Fixed in 2023.1.0a6._
    
*   Editor: Fixed crash in LightProbe Gizmo Rendering. (UUM-10958)  
    _First seen in 2023.1.0a5._  
    _Fixed in 2023.1.0a7._
    
*   Editor: Fixed SceneView exceptions on some mouse interactions ([UUM-6908](https://issuetracker.unity3d.com/issues/scene-window-stuck-in-orbit-after-context-menu-click-from-hierarchy))  
    _First seen in 2023.1.0a1._  
    _Fixed in 2023.1.0a6._
    
*   Graphics: Fix for new XR Display headers breaking Oculus App Spacewarp (ASW) due to a problem in back-compat code path. Fix for Vulkan validation error when GFR is disabled. (UUM-7369, UUM-9583)  
    _Fixed in 2023.1.0a7._
    
*   IL2CPP: Linux IL2CPP builds fail with "BuildFailedException: Incremental Player build failed!" ([1427577](https://issuetracker.unity3d.com/issues/linux-il2cpp-builds-fail-with-buildfailedexception-incremental-player-build-failed))
    
*   MacOS: \[Mac\] Editor performance drops on macOS when clicking and dragging on Position, Rotation and Scale values in Transform component ([UUM-7457](https://issuetracker.unity3d.com/issues/mac-editor-performance-drops-on-macos-when-clicking-and-dragging-on-position-rotation-and-scale-values-in-transform-component))
    
*   Mono: \[Linux\] C# Reflection performance is 50 to 60 times slower ([UUM-11526](https://issuetracker.unity3d.com/issues/linux-c-number-reflection-performance-is-50-to-60-times-slower))
    
*   Profiling: Profiler Modules submenu and window is missing Titles of Modules and Counters ([1419236](https://issuetracker.unity3d.com/issues/profiler-modules-submenu-and-window-is-missing-titles-of-modules-and-counters))
    
*   RP Workflow: \[HDRP\] Standalone Profiler throws "HDRP Material Upgrade" pop-up and crashes after pressing "Ok" ([1422062](https://issuetracker.unity3d.com/issues/hdrp-standalone-profiler-throws-hdrp-material-upgrade-pop-up-and-crashes-after-pressing-ok))
    
*   Scene Management: Undo crashes Unity with segmentation violation SIGSEGV ([1385565](https://issuetracker.unity3d.com/issues/undo-crashes-unity-with-segmentation-violation-sigsegv))
    
*   Scene Management: \[Undo\] Additional GameObjects and a Console error after Undoing and Redoing a Paste As Child ([UUM-9278](https://issuetracker.unity3d.com/issues/additional-gameobjects-and-a-console-error-after-undoing-and-redoing-a-paste-as-child))
    
*   Shader System: Shader variant build preparation does not scale (UUM-3711)
    
*   Shaders: fixed a crash when calling GetShaderKeywords on a user-constructed ShaderKeywordSet. ([UUM-2536](https://issuetracker.unity3d.com/issues/editor-crashes-when-building-if-calling-shaderkeyword-methods-in-ipreprocessshaders-classes))  
    _Fixed in 2023.1.0a6._
    
*   uGUI: Fixed calculation of pointer position when running in multiple display mode and the main display was fullscreen with a non-native aspect ratio. ([UUM-7893](https://issuetracker.unity3d.com/issues/broken-mouse-pointer-input-coordinates-in-graphicraycaster-for-certain-window-sizes-in-build-when-run-in-windowed-mode))  
    _Fixed in 2023.1.0a6._
    
*   UI Toolkit: Fixed an issue with numeric fields where entering negative value would yield incorrect values. ([UUM-10177](https://issuetracker.unity3d.com/issues/float-field-is-broken-when-entering-a-negative-value-after-highlighting))  
    _First seen in 2023.1.0a4._  
    _Fixed in 2023.1.0a7._
    
*   UI Toolkit: Fixed ListView to accept drag and drop to populate serialized arrays in the Editor. ([UUM-7948](https://issuetracker.unity3d.com/issues/inspector-cannot-drag-and-drop-to-populate-an-array-that-is-a-public-variable))  
    _First seen in 2023.1.0a2._  
    _Fixed in 2023.1.0a6._
    
*   Undo System: Handle additional changes when entering and exiting playmode ([UUM-9631](https://issuetracker.unity3d.com/issues/crash-on-undomanager-registerundooperation-when-exiting-play-mode-after-saving-changes-in-shader-graph))  
    _First seen in 2023.1.0a4._  
    _Fixed in 2023.1.0a7._
    
*   Windows: Fixed an Editor issue where entering an IP address for profiling would crash the Editor. (UUM-9247)  
    _First seen in 2023.1.0a3._  
    _Fixed in 2023.1.0a6._