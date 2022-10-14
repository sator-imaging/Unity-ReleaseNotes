# Unity 2023.1.0 Alpha 14

https://unity3d.com/unity/alpha/2023.1.0a14

## Known Issues in 2023.1.0a14



*   2D: \[Lost Crypt\] Unable to find URP 12.1.0 package error when importing Lost Crypt ([1388129](https://issuetracker.unity3d.com/issues/2d-lost-crypt-unable-to-find-urp-12-dot-1-0-package-error-when-importing-lost-crypt))
    
*   AI Navigation Core: NavMesh::Raycast freezes the whole editor in an infinite loop on Application.UpdateScene ([UUM-2496](https://issuetracker.unity3d.com/issues/navmesh-raycast-freezes-the-whole-editor-in-an-infinite-loop-on-application-dot-updatescene))
    
*   Animation: Rig builder prevets GameObject movement when two animations are playing at once ([UUM-16486](https://issuetracker.unity3d.com/issues/rig-builder-prevets-gameobject-movement-when-two-animations-are-playing-at-once))
    
*   Asset - Database: Infinite import on opening project (related to prefabs) ([1411189](https://issuetracker.unity3d.com/issues/infinite-import-on-opening-project-related-to-prefabs))
    
*   Asset - Database: Prefab Importing gets stuck on project opening when Parallel Importing is enabled ([UUM-11957](https://issuetracker.unity3d.com/issues/prefab-importing-gets-stuck-on-project-opening-when-parallel-importing-is-enabled))
    
*   Asset Bundles: AssetBundle indeterminism caused by mesh streaming info ([UUM-12721](https://issuetracker.unity3d.com/issues/assetbundle-indeterminism-caused-by-mesh-streaming-info))
    
*   Editor: Fixed crash in standalone profiler during shutdown. ([UUM-13932](https://issuetracker.unity3d.com/issues/standalone-profiler-crash-in-rtlentercriticalsection-on-exit))  
    _First seen in 2023.1.0a10._  
    _Fixed in 2023.1.0a15._
    
*   HDRP: Fixed graphics issues with sky and fog in game view when filtering objects in the hierarchy. ([UUM-11952](https://issuetracker.unity3d.com/issues/hdrp-visual-glitching-appear-in-game-view-after-selecting-a-gameobject-from-hierarchy-searching-results-whilst-fog-volume-override-is-enabled))  
    _Fixed in 2023.1.0a15._
    
*   HDRP: Fixed nullref exception when trying to use the HD Wizard "fix all" button. ([UUM-12793](https://issuetracker.unity3d.com/issues/user-is-not-prompted-to-create-hdrp-settings-when-trying-to-set-up-hdrp-with-the-hdrp-wizard))  
    _Fixed in 2023.1.0a15._
    
*   IL2CPP: Fixed possible crash/corruption when invoking a virtual generic method on a generic type by reflection or when Faster (smaller) builds is enabled. ([UUM-12498](https://issuetracker.unity3d.com/issues/il2cpp-build-crashes-when-symbols-cannot-be-found))  
    _Fixed in 2023.1.0a15._
    
*   IL2CPP: Linux IL2CPP builds fail with "BuildFailedException: Incremental Player build failed!" ([1427577](https://issuetracker.unity3d.com/issues/linux-il2cpp-builds-fail-with-buildfailedexception-incremental-player-build-failed))
    
*   Inspector Framework: Editor unselects elements when entering and then exiting the Play Mode ([UUM-16018](https://issuetracker.unity3d.com/issues/editor-unselects-elements-when-entering-and-then-exiting-the-play-mode))
    
*   MacOS: Standalone profiler crashing before opening ([UUM-16838](https://issuetracker.unity3d.com/issues/mac-standalone-profiler-crashing-before-opening))
    
*   Mono: Fixed LINQ performance regression on linux by switching to a more efficient stack checking method. ([UUM-11526](https://issuetracker.unity3d.com/issues/linux-c-number-reflection-performance-is-50-to-60-times-slower))  
    _Fixed in 2023.1.0a15._
    
*   Profiler: Fixed InvalidOperationException in ProfilerRecorder in projects with Scriptable Render Pipeline for Release Player builds. (UUM-14623)  
    _First seen in 2023.1.0a12._  
    _Fixed in 2023.1.0a15._
    
*   Profiling: Profiler Modules submenu and window is missing Titles of Modules and Counters ([1419236](https://issuetracker.unity3d.com/issues/profiler-modules-submenu-and-window-is-missing-titles-of-modules-and-counters))
    
*   RP Workflow: \[HDRP\] Standalone Profiler throws "HDRP Material Upgrade" pop-up and crashes after pressing "Ok" ([1422062](https://issuetracker.unity3d.com/issues/hdrp-standalone-profiler-throws-hdrp-material-upgrade-pop-up-and-crashes-after-pressing-ok))
    
*   Scene Management: Undo crashes Unity with segmentation violation SIGSEGV ([1385565](https://issuetracker.unity3d.com/issues/undo-crashes-unity-with-segmentation-violation-sigsegv))
    
*   Scene Management: Undoing prefab instancing leaves ghost objects in scene that throw ArgumentNullExceptions and crash editor when dragged to project view ([UUM-16824](https://issuetracker.unity3d.com/issues/undoing-prefab-instancing-leaves-ghost-objects-in-scene-that-throw-argumentnullexceptions))
    
*   Serialization: Fixed performance regression reading yaml objects containing large number of SerializeReference instances which were created prior to 2021.2. ([UUM-15130](https://issuetracker.unity3d.com/issues/serializereference-content-in-yaml-from-prior-to-2021-dot-2-takes-much-longer-to-load))  
    _First seen in 2023.1.0a10._  
    _Fixed in 2023.1.0a15._
    
*   Text: NullReferenceException in TMPro.MaterialReference when creating a UI Button - TextMeshPro ([UUM-13929](https://issuetracker.unity3d.com/issues/nullreferenceexception-in-tmpro-dot-materialreference-when-creating-a-ui-button-textmeshpro))
    
*   Universal RP: Fixed for BatchRendererGroup global SH values and the URP unity\_ProbesOcclusion that use float16 on iOS, which caused rendering problems. (UUM-14877)  
    _First seen in 2023.1.0a10._  
    _Fixed in 2023.1.0a15._
    
*   Visual Effects - Legacy: "NullReferenceException" in Particle System's Shape Module while reference is set ([UUM-11674](https://issuetracker.unity3d.com/issues/nullreferenceexception-in-particle-systems-shape-module-while-reference-is-set))
    
*   XR SRP: Meta Quest performance loss between URP versions when built ([UUM-15608](https://issuetracker.unity3d.com/issues/meta-quest-performance-loss-between-urp-versions-when-built))