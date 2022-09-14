# Unity 2023.1.0 Alpha 10

https://unity3d.com/unity/alpha/2023.1.0a10

## Known Issues in 2023.1.0a10



*   2D: \[com.unity.2d.psdimporter\] - Fixed exception when showing PSDImporter inspector.  
    _First seen in 2023.1.0._  
    _Fixed in 2023.1.0a12._
    
*   2D: \[Lost Crypt\] Unable to find URP 12.1.0 package error when importing Lost Crypt ([1388129](https://issuetracker.unity3d.com/issues/2d-lost-crypt-unable-to-find-urp-12-dot-1-0-package-error-when-importing-lost-crypt))
    
*   AI Navigation Core: NavMesh::Raycast freezes the whole editor in an infinite loop on Application.UpdateScene ([UUM-2496](https://issuetracker.unity3d.com/issues/navmesh-raycast-freezes-the-whole-editor-in-an-infinite-loop-on-application-dot-updatescene))
    
*   Asset - Database: Crash when opening Project Settings window ([UUM-11898](https://issuetracker.unity3d.com/issues/crash-when-opening-project-settings-window))
    
*   Asset - Database: Infinite import on opening project (related to prefabs) ([1411189](https://issuetracker.unity3d.com/issues/infinite-import-on-opening-project-related-to-prefabs))
    
*   Asset Import: Fixes the import of packages that are registered during InitializeOnLoad making sure that package folders are scanned and imported prior to first Assets import (UUM-3699)  
    _Fixed in 2023.1.0a11._
    
*   Editor: Pressing Apply in the Avatar edition isolation inspector does not close the edition anymore. (UUM-1040)  
    _First seen in 2023.1.0a1._  
    _Fixed in 2023.1.0a12._
    
*   Editor: Renaming a material does not prevent the colour palette to open anymore. ([UUM-7988](https://issuetracker.unity3d.com/issues/inspector-hdrp-colour-palette-window-will-not-open-after-renaming-a-material))  
    _First seen in 2023.1.0a2._  
    _Fixed in 2023.1.0a12._
    
*   GI: Fix a crash in the GPU lightmapper because of a null pointer dereference during compositing. ([UUM-12768](https://issuetracker.unity3d.com/issues/gpuplm-crash-in-openclbufferwrapperbase-enqueuereadbuffer-after-launching-gpu-lightmapper-bake))  
    _First seen in 2023.1.0a6._  
    _Fixed in 2023.1.0a11._
    
*   IL2CPP: Linux IL2CPP builds fail with "BuildFailedException: Incremental Player build failed!" ([1427577](https://issuetracker.unity3d.com/issues/linux-il2cpp-builds-fail-with-buildfailedexception-incremental-player-build-failed))
    
*   Kernel: \[2021.3\] Editor crashes on GetTransformAccess when undoing GameObject duplication ([UUM-13617](https://issuetracker.unity3d.com/issues/2021-dot-3-editor-cashes-on-gettransformaccess-when-undoing-duplication-of-a-canvasrenderer-gameobject))
    
*   MacOS: \[Mac\] Editor performance drops on macOS when clicking and dragging on Position, Rotation and Scale values in Transform component ([UUM-7457](https://issuetracker.unity3d.com/issues/mac-editor-performance-drops-on-macos-when-clicking-and-dragging-on-position-rotation-and-scale-values-in-transform-component))
    
*   Package Manager: Fixed a regression where operations would fail when the project path contained quotes. ([UUM-13252](https://issuetracker.unity3d.com/issues/package-manager-enoent-no-such-file-or-directory-mkdir))  
    _First seen in 2023.1.0a2._  
    _Fixed in 2023.1.0a11._
    
*   Profiling: Profiler Modules submenu and window is missing Titles of Modules and Counters ([1419236](https://issuetracker.unity3d.com/issues/profiler-modules-submenu-and-window-is-missing-titles-of-modules-and-counters))
    
*   RP Workflow: \[HDRP\] Standalone Profiler throws "HDRP Material Upgrade" pop-up and crashes after pressing "Ok" ([1422062](https://issuetracker.unity3d.com/issues/hdrp-standalone-profiler-throws-hdrp-material-upgrade-pop-up-and-crashes-after-pressing-ok))
    
*   Scene Management: Undo crashes Unity with segmentation violation SIGSEGV ([1385565](https://issuetracker.unity3d.com/issues/undo-crashes-unity-with-segmentation-violation-sigsegv))
    
*   Scene Management: \[Undo\] Additional GameObjects and a Console error after Undoing and Redoing a Paste As Child ([UUM-9278](https://issuetracker.unity3d.com/issues/additional-gameobjects-and-a-console-error-after-undoing-and-redoing-a-paste-as-child))
    
*   Shader System: Shader variant build preparation does not scale ([UUM-3711](https://issuetracker.unity3d.com/issues/shader-variant-build-preparation-does-not-scale))
    
*   Video: Unity freeze/becomes unresponsive when multiple videos are playing in Play mode ([UUM-13294](https://issuetracker.unity3d.com/issues/unity-freeze-slash-becomes-unresponsive-when-multiple-videos-are-playing-in-play-mode))