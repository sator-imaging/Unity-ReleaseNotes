# Unity 2023.1.0 Alpha 13

https://unity3d.com/unity/alpha/2023.1.0a13

## Known Issues in 2023.1.0a13



*   2D: \[Lost Crypt\] Unable to find URP 12.1.0 package error when importing Lost Crypt ([1388129](https://issuetracker.unity3d.com/issues/2d-lost-crypt-unable-to-find-urp-12-dot-1-0-package-error-when-importing-lost-crypt))
    
*   Asset - Database: Infinite import on opening project (related to prefabs) ([1411189](https://issuetracker.unity3d.com/issues/infinite-import-on-opening-project-related-to-prefabs))
    
*   Asset - Database: Prefab Importing gets stuck on project opening when Parallel Importing is enabled ([UUM-11957](https://issuetracker.unity3d.com/issues/prefab-importing-gets-stuck-on-project-opening-when-parallel-importing-is-enabled))
    
*   Asset Bundles: AssetBundle indeterminism caused by mesh streaming info ([UUM-12721](https://issuetracker.unity3d.com/issues/assetbundle-indeterminism-caused-by-mesh-streaming-info))
    
*   Core: Fixed slow native memory leak when in Playmode caused by the temp memory allocator not flushing correctly when requested. Previously leaving Playmode running could result in Out of Memory if left running for hours. ([UUM-12094](https://issuetracker.unity3d.com/issues/urp-builds-leak-memory-at-a-0-dot-1-mb-slash-sec-rate))  
    _First seen in 2023.1.0a6._  
    _Fixed in 2023.1.0a14._
    
*   Editor: Enabling shader keyword pre-filtering so that build process does not have to enumerate through full shader variant space. This fixes the issue of URP builds even with warm shader cache taking really long time. This fix does not reduce the time spent on actually compiling shaders. ([UUM-3711](https://issuetracker.unity3d.com/issues/shader-variant-build-preparation-does-not-scale))  
    _Fixed in 2023.1.0a14._
    
*   Editor: Fixes crash in standalone profiler during shutdown ([UUM-13932](https://issuetracker.unity3d.com/issues/standalone-profiler-crash-in-rtlentercriticalsection-on-exit))  
    _First seen in 2023.1.0a10._  
    _Fixed in 2023.1.0a15._
    
*   Editor: Memory fix, where an object could be accessed after it has been freed. (UUM-12903)  
    _Fixed in 2023.1.0a14._
    
*   HDRP: Fix nullref exception when trying to use the HD Wizard "fix all" button. ([UUM-12793](https://issuetracker.unity3d.com/issues/user-is-not-prompted-to-create-hdrp-settings-when-trying-to-set-up-hdrp-with-the-hdrp-wizard))  
    _Fixed in 2023.1.0a15._
    
*   IL2CPP: Linux IL2CPP builds fail with "BuildFailedException: Incremental Player build failed!" ([1427577](https://issuetracker.unity3d.com/issues/linux-il2cpp-builds-fail-with-buildfailedexception-incremental-player-build-failed))
    
*   Profiling: Profiler Modules submenu and window is missing Titles of Modules and Counters ([1419236](https://issuetracker.unity3d.com/issues/profiler-modules-submenu-and-window-is-missing-titles-of-modules-and-counters))
    
*   RP Workflow: \[HDRP\] Standalone Profiler throws "HDRP Material Upgrade" pop-up and crashes after pressing "Ok" ([1422062](https://issuetracker.unity3d.com/issues/hdrp-standalone-profiler-throws-hdrp-material-upgrade-pop-up-and-crashes-after-pressing-ok))
    
*   Scene Management: Undo crashes Unity with segmentation violation SIGSEGV ([1385565](https://issuetracker.unity3d.com/issues/undo-crashes-unity-with-segmentation-violation-sigsegv))
    
*   Serialization: Fix performance regression reading yaml objects containing large number of SerializeReference instances which were created prior to 2021.2. ([UUM-15130](https://issuetracker.unity3d.com/issues/serializereference-content-in-yaml-from-prior-to-2021-dot-2-takes-much-longer-to-load))  
    _First seen in 2023.1.0a10._  
    _Fixed in 2023.1.0a15._
    
*   Text: NullReferenceException in TMPro.MaterialReference when creating a UI Button - TextMeshPro ([UUM-13929](https://issuetracker.unity3d.com/issues/nullreferenceexception-in-tmpro-dot-materialreference-when-creating-a-ui-button-textmeshpro))
    
*   VFX Graph: Fixed compilation time increase due to DXR passes (UUM-14869)  
    _First seen in 2023.1.0a10._  
    _Fixed in 2023.1.0a14._
    
*   VFX Graph: Unexpected unrecognized identifier 'GraphValues' while using SG (UUM-15183)  
    _First seen in 2023.1.0a12._  
    _Fixed in 2023.1.0a14._