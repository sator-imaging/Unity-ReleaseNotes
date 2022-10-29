# Unity 2023.1.0 Alpha 16

https://unity3d.com/unity/alpha/2023.1.0a16

## Known Issues in 2023.1.0a16



*   2D: \[Lost Crypt\] Unable to find URP 12.1.0 package error when importing Lost Crypt ([1388129](https://issuetracker.unity3d.com/issues/2d-lost-crypt-unable-to-find-urp-12-dot-1-0-package-error-when-importing-lost-crypt))
    
*   Asset - Database: Folder name is truncated when dot is used in the name ([UUM-7046](https://issuetracker.unity3d.com/issues/folder-name-is-truncated-when-dot-is-used-in-the-name))
    
*   Asset - Database: Infinite import on opening project (related to prefabs) ([1411189](https://issuetracker.unity3d.com/issues/infinite-import-on-opening-project-related-to-prefabs))
    
*   Asset Importers: Editor hangs when importing certain .fbx files ([UUM-15346](https://issuetracker.unity3d.com/issues/editor-hangs-when-importing-certain-fbx-files))
    
*   Editor: Fix scene view tools engaging too eagerly when bound to mouse buttons ([UUM-16835](https://issuetracker.unity3d.com/issues/macos-mouse-gets-stuck-on-right-click-drag-in-scene-after-right-clicking-anywhere-in-editor))  
    _First seen in 2023.1.0a13._  
    _Fixed in 2023.1.0a18._
    
*   Editor: Fixed an issue with missing data for Ray Tracing and Compute events in Frame Debugger. (UUM-16663)  
    _Fixed in 2023.1.0a17._
    
*   Editor: Fixed BatchRendererGroup performance issues with many draw commands. (UUM-16378)  
    _Fixed in 2023.1.0a17._
    
*   Editor: Fixed crash of profiler opened in standalone process ([UUM-16838](https://issuetracker.unity3d.com/issues/mac-standalone-profiler-crashing-before-opening))  
    _Fixed in 2023.1.0a18._
    
*   Editor: Fixed crash when calling EditorUtility.UnloadUnusedAssetsImmediate(false) ([UUM-11648](https://issuetracker.unity3d.com/issues/editor-crashes-when-editorutility-dot-unloadunusedassetsimmediate-is-called))  
    _First seen in 2023.1.0a12._  
    _Fixed in 2023.1.0a18._
    
*   Editor: Fixed SpriteShape so it now renders with SRP Batching disabled in URP. (UUM-17290)  
    _First seen in 2023.1.0a15._  
    _Fixed in 2023.1.0a17._
    
*   Editor: Revive RecompileAfterFinishedPlaying option (UUM-16168)  
    _Fixed in 2023.1.0a18._
    
*   GI: Fixed editor crash when viewing the texel validity. ([UUM-17235](https://issuetracker.unity3d.com/issues/texel-validity-scene-view-mode-crashes))  
    _First seen in 2023.1.0a16._  
    _Fixed in 2023.1.0a17._
    
*   Graphics: Fix ShadowMaps resolving AA when not necessary (UUM-13371)  
    _First seen in 2023.1.0a8._  
    _Fixed in 2023.1.0a18._
    
*   IL2CPP: Fixed possible memory corrupt/crash when calling into shared generic code. (UUM-14924)  
    _Fixed in 2023.1.0a17._
    
*   IL2CPP: Linux IL2CPP builds fail with "BuildFailedException: Incremental Player build failed!" ([1427577](https://issuetracker.unity3d.com/issues/linux-il2cpp-builds-fail-with-buildfailedexception-incremental-player-build-failed))
    
*   Metal: \[iOS\]Unable to maintain 120fps consistently in a near-empty scene on iPhone 13 Pro ([UUM-5944](https://issuetracker.unity3d.com/issues/ios-target-fps-is-ignored-on-iphone-13-pro))
    
*   Package: NullReferenceException in TMPro.MaterialReference when creating a UI Button - TextMeshPro ([UUM-13929](https://issuetracker.unity3d.com/issues/nullreferenceexception-in-tmpro-dot-materialreference-when-creating-a-ui-button-textmeshpro))
    
*   Particles: Enabled GetTriggerParticles to always return the correct results. ([UUM-14581](https://issuetracker.unity3d.com/issues/gettriggerparticles-returns-0-every-few-frames-when-getting-a-number-of-particles-inside))  
    _Fixed in 2023.1.0a17._
    
*   Profiling: Profiler Modules submenu and window is missing Titles of Modules and Counters ([1419236](https://issuetracker.unity3d.com/issues/profiler-modules-submenu-and-window-is-missing-titles-of-modules-and-counters))
    
*   RP Workflow: \[HDRP\] Standalone Profiler throws "HDRP Material Upgrade" pop-up and crashes after pressing "Ok" ([1422062](https://issuetracker.unity3d.com/issues/hdrp-standalone-profiler-throws-hdrp-material-upgrade-pop-up-and-crashes-after-pressing-ok))
    
*   Scene Management: Editor unselects elements when entering and then exiting the Play Mode ([UUM-16018](https://issuetracker.unity3d.com/issues/editor-unselects-elements-when-entering-and-then-exiting-the-play-mode))
    
*   Scene Management: Undo crashes Unity with segmentation violation SIGSEGV ([1385565](https://issuetracker.unity3d.com/issues/undo-crashes-unity-with-segmentation-violation-sigsegv))
    
*   Scene Management: Undoing prefab instancing leaves ghost objects in scene that throw ArgumentNullExceptions and crash editor when dragged to project view ([UUM-16824](https://issuetracker.unity3d.com/issues/undoing-prefab-instancing-leaves-ghost-objects-in-scene-that-throw-argumentnullexceptions))
    
*   Scene Management: \[Undo\] Additional GameObjects and a Console error after Undoing and Redoing a Paste As Child ([UUM-9278](https://issuetracker.unity3d.com/issues/additional-gameobjects-and-a-console-error-after-undoing-and-redoing-a-paste-as-child))
    
*   ShaderGraph: \[Shader Graph\] Shader instance property gets added to CBUFFER, which causes GPU instancing with instanced properties to not work ([UUM-10963](https://issuetracker.unity3d.com/issues/shader-graph-shader-instance-property-gets-added-to-cbuffer-which-causes-gpu-instancing-with-instanced-properties-to-not-work))
    
*   uGUI: Fixed various issues with Canvas. ([UUM-15518](https://issuetracker.unity3d.com/issues/canvas-is-still-receiving-input-after-the-canvas-was-disabled))  
    _First seen in 2023.1.0a10._  
    _Fixed in 2023.1.0a17._
    
*   UI Toolkit Framework: Unity Editor is rendered without the toolbar icons when using it on old hardware with integrated GPU ([UUM-13134](https://issuetracker.unity3d.com/issues/unity-editor-is-rendered-without-the-toolbar-icons-when-using-it-on-old-hardware-with-integrated-gpu))
    
*   Universal RP: Shader compilation time is higher in 2021.3 than in 2020.3 ([UUM-17405](https://issuetracker.unity3d.com/issues/shader-compilation-time-is-higher-in-2021-dot-3-than-in-2020-dot-3))