# Unity 2023.1.0 Alpha 12

https://unity3d.com/unity/alpha/2023.1.0a12

## Known Issues in 2023.1.0a12



*   2D: \[Lost Crypt\] Unable to find URP 12.1.0 package error when importing Lost Crypt ([1388129](https://issuetracker.unity3d.com/issues/2d-lost-crypt-unable-to-find-urp-12-dot-1-0-package-error-when-importing-lost-crypt))
    
*   AI: Colliders set as trigger are excluded from NavMesh generation ([UUM-10109](https://issuetracker.unity3d.com/issues/trigger-volumes-are-included-in-nav-mesh-generation-for-navmeshsurface-when-geometry-is-set-to-physics-colliders))  
    _Fixed in 2023.1.0a13._
    
*   Asset - Database: Infinite import on opening project (related to prefabs) ([1411189](https://issuetracker.unity3d.com/issues/infinite-import-on-opening-project-related-to-prefabs))
    
*   Asset Bundles: AssetBundle indeterminism caused by mesh streaming info ([UUM-12721](https://issuetracker.unity3d.com/issues/assetbundle-indeterminism-caused-by-mesh-streaming-info))
    
*   Asset Importers: Editor crashes when importing certain .mb files ([UUM-14446](https://issuetracker.unity3d.com/issues/editor-crashes-when-importing-certain-mb-files))
    
*   Asset Pipeline: Fix case of SRP changing mid refresh resulting in infinite imports ([UUM-11957](https://issuetracker.unity3d.com/issues/prefab-importing-gets-stuck-on-project-opening-when-parallel-importing-is-enabled))  
    _Fixed in 2023.1.0a13._
    
*   Editor: Fixed deadlock scenario in shader compiler. (UUM-14040)  
    _Fixed in 2023.1.0a13._
    
*   Editor: Job worker threads will now prefer executing jobs scheduled during job execution, avoiding long job wait --> steal --> wait -> steal chains which could result in a stack overflow. (UUM-10271)  
    _First seen in 2023.1.0a5._  
    _Fixed in 2023.1.0a13._
    
*   Graphics: Fix for depth submission crash when no MSAA is enabled (Quest 2). ([UUM-13249](https://issuetracker.unity3d.com/issues/graphics-crash-when-submitting-depth-with-no-msaa))  
    _First seen in 2023.1.0a5._  
    _Fixed in 2023.1.0a13._
    
*   IL2CPP: Linux IL2CPP builds fail with "BuildFailedException: Incremental Player build failed!" ([1427577](https://issuetracker.unity3d.com/issues/linux-il2cpp-builds-fail-with-buildfailedexception-incremental-player-build-failed))
    
*   Optimization: \[Mac\] Editor performance drops on macOS when clicking and dragging on Position, Rotation and Scale values in Transform component ([UUM-7457](https://issuetracker.unity3d.com/issues/mac-editor-performance-drops-on-macos-when-clicking-and-dragging-on-position-rotation-and-scale-values-in-transform-component))
    
*   Particles: Fix null reference exceptions when previewing particles in the Scene View. ([UUM-11674](https://issuetracker.unity3d.com/issues/nullreferenceexception-in-particle-systems-shape-module-while-reference-is-set))  
    _Fixed in 2023.1.0a13._
    
*   Physics 2D: Fix a crash when using the PlatformEffector2D and toggling the "Used By Effector" on any 2D Collider in the Editor Inspector view. ([UUM-12859](https://issuetracker.unity3d.com/issues/2d-changing-values-of-platform-effector-2d-component-fields-crashes-the-editor-when-before-the-used-by-effector-field-value-had-been-changed))  
    _Fixed in 2023.1.0a13._
    
*   Profiling: Profiler Modules submenu and window is missing Titles of Modules and Counters ([1419236](https://issuetracker.unity3d.com/issues/profiler-modules-submenu-and-window-is-missing-titles-of-modules-and-counters))
    
*   RP Workflow: \[HDRP\] Standalone Profiler throws "HDRP Material Upgrade" pop-up and crashes after pressing "Ok" ([1422062](https://issuetracker.unity3d.com/issues/hdrp-standalone-profiler-throws-hdrp-material-upgrade-pop-up-and-crashes-after-pressing-ok))
    
*   Scene Management: Undo crashes Unity with segmentation violation SIGSEGV ([1385565](https://issuetracker.unity3d.com/issues/undo-crashes-unity-with-segmentation-violation-sigsegv))
    
*   Shader System: Shader variant build preparation does not scale ([UUM-3711](https://issuetracker.unity3d.com/issues/shader-variant-build-preparation-does-not-scale))
    
*   Text: NullReferenceException in TMPro.MaterialReference when creating a UI Button - TextMeshPro ([UUM-13929](https://issuetracker.unity3d.com/issues/nullreferenceexception-in-tmpro-dot-materialreference-when-creating-a-ui-button-textmeshpro))
    
*   Video: Fixed a bug where video playback would cause severe CPU utilization. ([UUM-13294](https://issuetracker.unity3d.com/issues/unity-freeze-slash-becomes-unresponsive-when-multiple-videos-are-playing-in-play-mode))  
    _Fixed in 2023.1.0a13._
    
*   Visual Effects: \[Visual Effects Graph\] Closing the VFX Window autosaves any changes applied (UUM-4767)