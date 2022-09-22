# Unity 2023.1.0 Alpha 11

https://unity3d.com/unity/alpha/2023.1.0a11

## Known Issues in 2023.1.0a11



*   2D: \[com.unity.2d.psdimporter\] - Fixed exception when showing PSDImporter inspector.  
    _First seen in 2023.1.0._  
    _Fixed in 2023.1.0a12._
    
*   2D: \[Lost Crypt\] Unable to find URP 12.1.0 package error when importing Lost Crypt ([1388129](https://issuetracker.unity3d.com/issues/2d-lost-crypt-unable-to-find-urp-12-dot-1-0-package-error-when-importing-lost-crypt))
    
*   AI Navigation Core: NavMesh::Raycast freezes the whole editor in an infinite loop on Application.UpdateScene ([UUM-2496](https://issuetracker.unity3d.com/issues/navmesh-raycast-freezes-the-whole-editor-in-an-infinite-loop-on-application-dot-updatescene))
    
*   Asset - Database: Infinite import on opening project (related to prefabs) ([1411189](https://issuetracker.unity3d.com/issues/infinite-import-on-opening-project-related-to-prefabs))
    
*   Editor: Pressing Apply in the Avatar edition isolation inspector does not close the edition anymore. (UUM-1040)  
    _First seen in 2023.1.0a1._  
    _Fixed in 2023.1.0a12._
    
*   Editor: Renaming a material does not prevent the colour palette to open anymore. ([UUM-7988](https://issuetracker.unity3d.com/issues/inspector-hdrp-colour-palette-window-will-not-open-after-renaming-a-material))  
    _First seen in 2023.1.0a2._  
    _Fixed in 2023.1.0a12._
    
*   IL2CPP: Linux IL2CPP builds fail with "BuildFailedException: Incremental Player build failed!" ([1427577](https://issuetracker.unity3d.com/issues/linux-il2cpp-builds-fail-with-buildfailedexception-incremental-player-build-failed))
    
*   MacOS: \[Mac\] Editor performance drops on macOS when clicking and dragging on Position, Rotation and Scale values in Transform component ([UUM-7457](https://issuetracker.unity3d.com/issues/mac-editor-performance-drops-on-macos-when-clicking-and-dragging-on-position-rotation-and-scale-values-in-transform-component))
    
*   Profiling: Profiler Modules submenu and window is missing Titles of Modules and Counters ([1419236](https://issuetracker.unity3d.com/issues/profiler-modules-submenu-and-window-is-missing-titles-of-modules-and-counters))
    
*   RP Workflow: \[HDRP\] Standalone Profiler throws "HDRP Material Upgrade" pop-up and crashes after pressing "Ok" ([1422062](https://issuetracker.unity3d.com/issues/hdrp-standalone-profiler-throws-hdrp-material-upgrade-pop-up-and-crashes-after-pressing-ok))
    
*   Scene Management: Undo crashes Unity with segmentation violation SIGSEGV ([1385565](https://issuetracker.unity3d.com/issues/undo-crashes-unity-with-segmentation-violation-sigsegv))
    
*   Scripting: ILPP runner and trigger executables are now signed (UUM-13575)  
    _First seen in 2023.1.0a6._  
    _Fixed in 2023.1.0a12._
    
*   Serialization: Fix regression where if a mesh was used in vfx and included in an AssetBundle there could be indeterminism in its streaming info offset field. ([UUM-12721](https://issuetracker.unity3d.com/issues/assetbundle-indeterminism-caused-by-mesh-streaming-info))  
    _First seen in 2023.1.0a6._  
    _Fixed in 2023.1.0a12._
    
*   Shader System: Shader variant build preparation does not scale ([UUM-3711](https://issuetracker.unity3d.com/issues/shader-variant-build-preparation-does-not-scale))
    
*   Shaders: Fixed an issue where shader requirements were not applied correctly to all variants (UUM-14327)  
    _First seen in 2023.1.0a11._  
    _Fixed in 2023.1.0a12._
    
*   Text: NullReferenceException in TMPro.MaterialReference when creating a UI Button - TextMeshPro ([UUM-13929](https://issuetracker.unity3d.com/issues/nullreferenceexception-in-tmpro-dot-materialreference-when-creating-a-ui-button-textmeshpro))
    
*   Visual Effects: \[Visual Effects Graph\] Closing the VFX Window autosaves any changes applied (UUM-4767)
    
*   Windows: Fixed certain cursors being invisible. (UUM-12529)  
    _First seen in 2023.1.0a8._  
    _Fixed in 2023.1.0a12._
    
*   Windows: Fixed editor failing to restart itself when requested (for instance, when changing active input backend or the graphics API). (UUM-12578)  
    _First seen in 2023.1.0a8._  
    _Fixed in 2023.1.0a12._