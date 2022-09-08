# Unity 2023.1.0 Alpha 9

https://unity3d.com/unity/alpha/2023.1.0a9

## Known Issues in 2023.1.0a9



*   2D: \[Lost Crypt\] Unable to find URP 12.1.0 package error when importing Lost Crypt ([1388129](https://issuetracker.unity3d.com/issues/2d-lost-crypt-unable-to-find-urp-12-dot-1-0-package-error-when-importing-lost-crypt))
    
*   Android: Fix incorrect aspect ration when phone is landscape mode, "Apply display rotation during rendering" is enabled and URP post processing is used with Vulkan (UUM-5653)  
    _Fixed in 2023.1.0a10._
    
*   Asset - Database: Crash when opening Project Settings window ([UUM-11898](https://issuetracker.unity3d.com/issues/crash-when-opening-project-settings-window))
    
*   Asset - Database: Infinite import on opening project (related to prefabs) ([1411189](https://issuetracker.unity3d.com/issues/infinite-import-on-opening-project-related-to-prefabs))
    
*   Editor: Fixed crash when entering playmode with an asset in a property window. (UUM-12079)  
    _First seen in 2023.1.0a5._  
    _Fixed in 2023.1.0a10._
    
*   Editor: Tooltips no longer prevent keyboard shortcuts (UUM-12140)  
    _First seen in 2023.1.0a5._  
    _Fixed in 2023.1.0a10._
    
*   GI: Fix a crash in the GPU lightmapper because of a null pointer dereference during compositing. ([UUM-12768](https://issuetracker.unity3d.com/issues/gpuplm-crash-in-openclbufferwrapperbase-enqueuereadbuffer-after-launching-gpu-lightmapper-bake))  
    _First seen in 2023.1.0a6._  
    _Fixed in 2023.1.0a11._
    
*   IL2CPP: Linux IL2CPP builds fail with "BuildFailedException: Incremental Player build failed!" ([1427577](https://issuetracker.unity3d.com/issues/linux-il2cpp-builds-fail-with-buildfailedexception-incremental-player-build-failed))
    
*   MacOS: \[Mac\] Editor performance drops on macOS when clicking and dragging on Position, Rotation and Scale values in Transform component ([UUM-7457](https://issuetracker.unity3d.com/issues/mac-editor-performance-drops-on-macos-when-clicking-and-dragging-on-position-rotation-and-scale-values-in-transform-component))
    
*   Package Manager: Fixed a regression where operations would fail when the project path contained quotes. ([UUM-13252](https://issuetracker.unity3d.com/issues/package-manager-enoent-no-such-file-or-directory-mkdir))  
    _First seen in 2023.1.0a2._  
    _Fixed in 2023.1.0a11._
    
*   Profiling: Profiler Modules submenu and window is missing Titles of Modules and Counters ([1419236](https://issuetracker.unity3d.com/issues/profiler-modules-submenu-and-window-is-missing-titles-of-modules-and-counters))
    
*   RP Workflow: \[HDRP\] Standalone Profiler throws "HDRP Material Upgrade" pop-up and crashes after pressing "Ok" ([1422062](https://issuetracker.unity3d.com/issues/hdrp-standalone-profiler-throws-hdrp-material-upgrade-pop-up-and-crashes-after-pressing-ok))
    
*   Scene Management: Undo crashes Unity with segmentation violation SIGSEGV ([1385565](https://issuetracker.unity3d.com/issues/undo-crashes-unity-with-segmentation-violation-sigsegv))
    
*   Scene Management: \[Undo\] Additional GameObjects and a Console error after Undoing and Redoing a Paste As Child ([UUM-9278](https://issuetracker.unity3d.com/issues/additional-gameobjects-and-a-console-error-after-undoing-and-redoing-a-paste-as-child))
    
*   Scripting: Some Native libraries was not loaded with platform specific extensions (UUM-11681)  
    _First seen in 2023.1.0a3._  
    _Fixed in 2023.1.0a10._
    
*   Shader System: Shader variant build preparation does not scale ([UUM-3711](https://issuetracker.unity3d.com/issues/shader-variant-build-preparation-does-not-scale))
    
*   Shaders: Fixed "State comes from an incompatible keyword space" assertion firing sometimes when building asset bundles. (UUM-11958)  
    _Fixed in 2023.1.0a10._
    
*   Video: Unity freeze/becomes unresponsive when multiple videos are playing in Play mode ([UUM-13294](https://issuetracker.unity3d.com/issues/unity-freeze-slash-becomes-unresponsive-when-multiple-videos-are-playing-in-play-mode))