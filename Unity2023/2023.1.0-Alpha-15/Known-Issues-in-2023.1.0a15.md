# Unity 2023.1.0 Alpha 15

https://unity3d.com/unity/alpha/2023.1.0a15

## Known Issues in 2023.1.0a15



*   2D: \[Lost Crypt\] Unable to find URP 12.1.0 package error when importing Lost Crypt ([1388129](https://issuetracker.unity3d.com/issues/2d-lost-crypt-unable-to-find-urp-12-dot-1-0-package-error-when-importing-lost-crypt))
    
*   Asset - Database: Folder name is truncated when dot is used in the name ([UUM-7046](https://issuetracker.unity3d.com/issues/folder-name-is-truncated-when-dot-is-used-in-the-name))
    
*   Asset - Database: Infinite import on opening project (related to prefabs) ([1411189](https://issuetracker.unity3d.com/issues/infinite-import-on-opening-project-related-to-prefabs))
    
*   Editor: Fixed crash with TilemapCollider2D when used with a CompositeCollider2D and a Tile with no Sprite with Collider Type Sprite is set. (UUM-15912)  
    _Fixed in 2023.1.0a16._
    
*   Editor: Fixed scripted importer registration errors that occur when changing platform. ([UUM-14062](https://issuetracker.unity3d.com/issues/switching-target-platform-in-build-settings-throws-assetimporters-dot-scriptedimporter-errors))  
    _First seen in 2023.1.0a10._  
    _Fixed in 2023.1.0a16._
    
*   Editor: Frame Debugger: Fixed an issue with missing data for Ray Tracing and Compute events. (UUM-16663)  
    _Fixed in 2023.1.0a17._
    
*   Editor: Modified Experimental package versions so that patches of the package's lifecycle manifest version are no longer erroneously tagged as Release. (UUM-16118)  
    _First seen in 2023.1.0a14._  
    _Fixed in 2023.1.0a16._
    
*   Editor: Re-implemented the original fix for case 1393058. ([UUM-9278](https://issuetracker.unity3d.com/issues/additional-gameobjects-and-a-console-error-after-undoing-and-redoing-a-paste-as-child))  
    _Fixed in 2023.1.0a16._
    
*   IL2CPP: Fixed possible memory corrupt/crash when calling into shared generic code. (UUM-14924)  
    _Fixed in 2023.1.0a17._
    
*   IL2CPP: Linux IL2CPP builds fail with "BuildFailedException: Incremental Player build failed!" ([1427577](https://issuetracker.unity3d.com/issues/linux-il2cpp-builds-fail-with-buildfailedexception-incremental-player-build-failed))
    
*   Metal: \[iOS\]Unable to maintain 120fps consistently in a near-empty scene on iPhone 13 Pro ([UUM-5944](https://issuetracker.unity3d.com/issues/ios-target-fps-is-ignored-on-iphone-13-pro))
    
*   Package: NullReferenceException in TMPro.MaterialReference when creating a UI Button - TextMeshPro ([UUM-13929](https://issuetracker.unity3d.com/issues/nullreferenceexception-in-tmpro-dot-materialreference-when-creating-a-ui-button-textmeshpro))
    
*   Particles: Ensure GetTriggerParticles always returns the correct results. ([UUM-14581](https://issuetracker.unity3d.com/issues/gettriggerparticles-returns-0-every-few-frames-when-getting-a-number-of-particles-inside))  
    _Fixed in 2023.1.0a17._
    
*   Physics: Fixed an issue where having multiple Collider components on the same GameObject would cause a crash if one of the colliders was disabled. ([UUM-13922](https://issuetracker.unity3d.com/issues/crash-on-capsulecollider-setscale-when-rotating-a-gameobject-with-a-capsulecollider-component))  
    _First seen in 2023.1.0a10._  
    _Fixed in 2023.1.0a16._
    
*   Profiling: Profiler Modules submenu and window is missing Titles of Modules and Counters ([1419236](https://issuetracker.unity3d.com/issues/profiler-modules-submenu-and-window-is-missing-titles-of-modules-and-counters))
    
*   RP Workflow: \[HDRP\] Standalone Profiler throws "HDRP Material Upgrade" pop-up and crashes after pressing "Ok" ([1422062](https://issuetracker.unity3d.com/issues/hdrp-standalone-profiler-throws-hdrp-material-upgrade-pop-up-and-crashes-after-pressing-ok))
    
*   Scene Management: Editor unselects elements when entering and then exiting the Play Mode ([UUM-16018](https://issuetracker.unity3d.com/issues/editor-unselects-elements-when-entering-and-then-exiting-the-play-mode))
    
*   Scene Management: Undo crashes Unity with segmentation violation SIGSEGV ([1385565](https://issuetracker.unity3d.com/issues/undo-crashes-unity-with-segmentation-violation-sigsegv))
    
*   Scene Management: Undoing prefab instancing leaves ghost objects in scene that throw ArgumentNullExceptions and crash editor when dragged to project view ([UUM-16824](https://issuetracker.unity3d.com/issues/undoing-prefab-instancing-leaves-ghost-objects-in-scene-that-throw-argumentnullexceptions))
    
*   ShaderGraph: \[Shader Graph\] Shader instance property gets added to CBUFFER, which causes GPU instancing with instanced properties to not work ([UUM-10963](https://issuetracker.unity3d.com/issues/shader-graph-shader-instance-property-gets-added-to-cbuffer-which-causes-gpu-instancing-with-instanced-properties-to-not-work))
    
*   uGUI: Fixed various issues with Canvas. ([UUM-15518](https://issuetracker.unity3d.com/issues/canvas-is-still-receiving-input-after-the-canvas-was-disabled))  
    _First seen in 2023.1.0a10._  
    _Fixed in 2023.1.0a17._
    
*   UI Toolkit: Fixed an issue in play mode so ScrollView offset no longer resets to zero when doing drag operations on controls inside it. ([UUM-10441](https://issuetracker.unity3d.com/issues/ui-panel-position-resets-when-sliders-are-scrolled-in-play-mode))  
    _First seen in 2023.1.0a4._  
    _Fixed in 2023.1.0a16._
    
*   UI Toolkit Controls: Editor gets stuck when scrolling through the Reoredable List ([UUM-17067](https://issuetracker.unity3d.com/issues/editor-gets-stuck-when-scrolling-through-the-reoredable-list))