# Unity 2023.1.0 Alpha 20

https://unity3d.com/unity/alpha/2023.1.0a20

## Known Issues in 2023.1.0a20



*   2D: \[Lost Crypt\] Unable to find URP 12.1.0 package error when importing Lost Crypt ([1388129](https://issuetracker.unity3d.com/issues/2d-lost-crypt-unable-to-find-urp-12-dot-1-0-package-error-when-importing-lost-crypt))
    
*   Asset - Database: Infinite import on opening project (related to prefabs) ([1411189](https://issuetracker.unity3d.com/issues/infinite-import-on-opening-project-related-to-prefabs))
    
*   Asset Pipeline: Fixed an issue where the standalone profiler could crash or emit errors when the script domain reloads in the editor. ([UUM-19179](https://issuetracker.unity3d.com/issues/edit-mode-recording-standalone-profiler-crashes-on-stopassetimportingv2internal-when-reloading-the-domain))  
    _First seen in 2023.1.0a19._  
    _Fixed in 2023.1.0a21._
    
*   Audio: Audio starts playing from the beginning when Undo/Redo Audio Source changes in Play Mode ([UUM-18551](https://issuetracker.unity3d.com/issues/audio-starts-playing-from-the-beginning-when-undo-slash-redo-audio-source-changes-in-play-mode))
    
*   Editor: Fix crash using unexpected ShaderGraph in VFX output ([UUM-13532](https://issuetracker.unity3d.com/issues/vfx-graph-crash-on-vfxmemoryserializer-storeobjects-when-undoing-actions-in-sg-blackboard))  
    _Fixed in 2023.1.0a22._
    
*   Editor: Fixed Editor crash when calling APIs to show modal dialogs while -drawRect is in progress. ([UUM-2293](https://issuetracker.unity3d.com/issues/crash-on-pthread-kill-when-editorutility-dot-openfolderpanel-is-executed))  
    _First seen in 2023.1.0a16._  
    _Fixed in 2023.1.0a21._
    
*   Editor: Fixed random plugin importer crash on Editor startup. (UUM-18397)  
    _Fixed in 2023.1.0a21._
    
*   Editor: Fixing silent crash caused by cache-server drop-down menu. ([UUM-11898](https://issuetracker.unity3d.com/issues/crash-when-opening-project-settings-window))  
    _First seen in 2023.1.0a4._  
    _Fixed in 2023.1.0a22._
    
*   Editor: Update Burst so URP/HDRP builds for PS5 (UUM-18929)  
    _First seen in 2023.1.0a17._  
    _Fixed in 2023.1.0a22._
    
*   Graphics: Fix BatchRendererGroup crashing due to threading race conditions in specific projects (UUM-18220)  
    _First seen in 2023.1.0a18._  
    _Fixed in 2023.1.0a22._
    
*   HD RP: \[HDRP\] DoF in half or quarter resolution results in cropped frame ([UUM-11354](https://issuetracker.unity3d.com/issues/hdrp-dof-in-half-or-quarter-resolution-results-in-cropped-frame))
    
*   IL2CPP: Linux IL2CPP builds fail with "BuildFailedException: Incremental Player build failed!" ([1427577](https://issuetracker.unity3d.com/issues/linux-il2cpp-builds-fail-with-buildfailedexception-incremental-player-build-failed))
    
*   MacOS: \[M1\]\[Rosseta\] Editor crashes on mono\_arch\_patch\_callsite when entering the Play Mode ([UUM-10411](https://issuetracker.unity3d.com/issues/m1-rosseta-editor-crashes-on-mono-arch-patch-callsite-when-entering-the-play-mode))
    
*   Metal: \[iOS\]Unable to maintain 120fps consistently in a near-empty scene on iPhone 13 Pro ([UUM-5944](https://issuetracker.unity3d.com/issues/ios-target-fps-is-ignored-on-iphone-13-pro))
    
*   Profiling: Profiler Modules submenu and window is missing Titles of Modules and Counters ([1419236](https://issuetracker.unity3d.com/issues/profiler-modules-submenu-and-window-is-missing-titles-of-modules-and-counters))
    
*   RP Workflow: \[HDRP\] Standalone Profiler throws "HDRP Material Upgrade" pop-up and crashes after pressing "Ok" ([1422062](https://issuetracker.unity3d.com/issues/hdrp-standalone-profiler-throws-hdrp-material-upgrade-pop-up-and-crashes-after-pressing-ok))
    
*   Scene Management: Undo crashes Unity with segmentation violation SIGSEGV ([1385565](https://issuetracker.unity3d.com/issues/undo-crashes-unity-with-segmentation-violation-sigsegv))
    
*   Shader System: GameObjects doesn't get rendered when using "Unlit.Unlit\_UsePass" Shader ([UUM-18980](https://issuetracker.unity3d.com/issues/sphere-gameobject-doesnt-get-rendered-when-using-unlit-dot-unlit-usepass-shader))
    
*   Shader System: Shader variant build preparation does not scale ([UUM-3711](https://issuetracker.unity3d.com/issues/shader-variant-build-preparation-does-not-scale))
    
*   Stadia: Folder name is truncated when dot is used in the name ([UUM-7046](https://issuetracker.unity3d.com/issues/folder-name-is-truncated-when-dot-is-used-in-the-name))
    
*   Universal RP: Fix post-process effects in scene view shaded mode ([UUM-11870](https://issuetracker.unity3d.com/issues/urp-post-processing-is-not-rendered-in-the-scene-view))  
    _First seen in 2023.1.0a5._  
    _Fixed in 2023.1.0a22._
    
*   Universal RP: Fixed an issue causing materials using Shader Graphs with material override to disappear when using the Deferred rendering path if alpha clipping is enabled in the material. ([UUM-18063](https://issuetracker.unity3d.com/issues/material-is-not-rendered-when-changing-the-rendering-path-from-forward-to-deferred))  
    _First seen in 2023.1.0a14._  
    _Fixed in 2023.1.0a22._
    
*   Universal RP: Fixed an issue with slower build-times caused by large Additional Light Shadows arrays in URP Shaders. ([UUM-17405](https://issuetracker.unity3d.com/issues/shader-compilation-time-is-higher-in-2021-dot-3-than-in-2020-dot-3))  
    _Fixed in 2023.1.0a22._
    
*   Universal RP: \[URP\] Memory leak when in Play Mode ([UUM-19089](https://issuetracker.unity3d.com/issues/urp-memory-leak-when-in-play-mode))
    
*   URP: Released render targets of non-used renderers. (UUM-16481)  
    _First seen in 2023.1.0a15._  
    _Fixed in 2023.1.0a21._