# Unity 2023.1.0 Alpha 4

https://unity3d.com/unity/alpha/2023.1.0a4

## Known Issues in 2023.1.0a4



*   2D: \[Lost Crypt\] Unable to find URP 12.1.0 package error when importing Lost Crypt ([1388129](https://issuetracker.unity3d.com/issues/2d-lost-crypt-unable-to-find-urp-12-dot-1-0-package-error-when-importing-lost-crypt))
    
*   AI Navigation Core: NavMesh::Raycast freezes the whole editor in an infinite loop on Application.UpdateScene ([UUM-2496](https://issuetracker.unity3d.com/issues/navmesh-raycast-freezes-the-whole-editor-in-an-infinite-loop-on-application-dot-updatescene))
    
*   Asset - Database: Infinite import on opening project (related to prefabs) ([1411189](https://issuetracker.unity3d.com/issues/infinite-import-on-opening-project-related-to-prefabs))
    
*   DirectX12: Camera.Render causes a memory leak in HDRP using DirectX 12 ([UUM-5879](https://issuetracker.unity3d.com/issues/camera-dot-render-causes-a-memory-leak-in-hdrp-using-directx-12-1))
    
*   DOTS: Crash when creating Assembly Definition Asset while Unity Logging package is installed ([UUM-8727](https://issuetracker.unity3d.com/issues/crash-when-creating-assembly-definition-asset-while-unity-logging-package-is-installed))
    
*   Editor: Fix the TimeManager for DragAndDropForwarding tests (UUM-6233)  
    _First seen in 2023.1.0a1._  
    _Fixed in 2023.1.0a5._
    
*   HD RP: \[HDRP\] "No more space in Reflection Probe Atlas" error is spammed on creating a HDRP 3D Sample Template ([UUM-5735](https://issuetracker.unity3d.com/issues/hdrp-no-more-space-in-reflection-probe-atlas-error-is-spammed-on-creating-a-hdrp-3d-sample-template))
    
*   IL2CPP: Fixed incorrect code generation for references to void\* pointers. ([UUM-4299](https://issuetracker.unity3d.com/issues/il2cpp-build-fails-when-code-has-public-ref-void-star-this-int-index-function))  
    _Fixed in 2023.1.0a5._
    
*   IL2CPP: Linux IL2CPP builds fail with "BuildFailedException: Incremental Player build failed!" ([1427577](https://issuetracker.unity3d.com/issues/linux-il2cpp-builds-fail-with-buildfailedexception-incremental-player-build-failed))
    
*   Incremental Build Pipeline: \[iOS\] Building an iOS project for Simulator fails in Xcode ([UUM-9393](https://issuetracker.unity3d.com/issues/ios-building-a-project-for-simulator-fails-in-xcode))
    
*   MacOS: \[Mac\] Editor performance drops on macOS when clicking and dragging on Position, Rotation and Scale values in Transform component ([UUM-7457](https://issuetracker.unity3d.com/issues/mac-editor-performance-drops-on-macos-when-clicking-and-dragging-on-position-rotation-and-scale-values-in-transform-component))
    
*   Package Manager: Keyboard navigation in package manager has been fixed. We can now properly use up/down, page up/down with optional shift key in asset tab. (UUM-6478)  
    _Fixed in 2023.1.0a5._
    
*   Prefabs: Fix after 'Apply All' is clicked in the overrides window then properties are still shown as overriden (UUM-6917)  
    _First seen in 2023.1.0a1._  
    _Fixed in 2023.1.0a5._
    
*   Profiling: Profiler Modules submenu and window is missing Titles of Modules and Counters ([1419236](https://issuetracker.unity3d.com/issues/profiler-modules-submenu-and-window-is-missing-titles-of-modules-and-counters))
    
*   RP Workflow: \[HDRP\] Standalone Profiler throws "HDRP Material Upgrade" pop-up and crashes after pressing "Ok" ([1422062](https://issuetracker.unity3d.com/issues/hdrp-standalone-profiler-throws-hdrp-material-upgrade-pop-up-and-crashes-after-pressing-ok))
    
*   Scene Management: Scene causes Editor crash when specific Lighting Data Asset is used ([UUM-9319](https://issuetracker.unity3d.com/issues/scene-causes-editor-crash-when-specific-lighting-data-asset-is-used))
    
*   Scene Management: Undo crashes Unity with segmentation violation SIGSEGV ([1385565](https://issuetracker.unity3d.com/issues/undo-crashes-unity-with-segmentation-violation-sigsegv))
    
*   Scene Management: \[Undo\] Additional GameObjects and a Console error after Undoing and Redoing a Paste As Child ([UUM-9278](https://issuetracker.unity3d.com/issues/additional-gameobjects-and-a-console-error-after-undoing-and-redoing-a-paste-as-child))
    
*   Shader System: Crash on ComputeShader::SetValueParam when opening a certain Scene ([UUM-495](https://issuetracker.unity3d.com/issues/crash-on-computeshader-setvalueparam-when-opening-a-certain-scene))
    
*   Shader System: Shader variant build preparation does not scale (UUM-3711)
    
*   Shadergraph: Fix the TimeManager for MaterialVariant tests (UUM-8013)  
    _First seen in 2023.1.0a3._  
    _Fixed in 2023.1.0a5._
    
*   Shadows/Lights: Scene is brighter in Standalone player if it was open in the Editor at build time ([1375015](https://issuetracker.unity3d.com/issues/scene-is-brighter-in-standalone-player-if-it-was-open-in-the-editor-at-build-time))
    
*   uGUI: UI Components OnCursorEnter state is ended when hovering cursor over smaller sized child UI objects ([UUM-505](https://issuetracker.unity3d.com/issues/ui-components-oncursorenter-state-is-ended-when-hovering-cursor-over-smaller-sized-child-ui-objects))
    
*   UI Toolkit: Fixed inspector alignment. (UUM-3476)  
    _First seen in 2023.1.0a1._  
    _Fixed in 2023.1.0a5._
    
*   UI Toolkit: Improved performance of the UITK NonReorderable and Reorderable ListView in the inspector. (UUM-3483)  
    _First seen in 2023.1.0a1._  
    _Fixed in 2023.1.0a5._
    
*   Undo System: Fix the TimeManager for UndoManager tests (UUM-8019)  
    _First seen in 2023.1.0a3._  
    _Fixed in 2023.1.0a5._
    
*   Universal: Fix depth pre-pass being always executed on GLES devices ([UUM-8381](https://issuetracker.unity3d.com/issues/urp-depth-pre-pass-is-always-executed-regardless-of-project-slash-pipeline-settings-when-opengles3-graphics-api-is-used))  
    _Fixed in 2023.1.0a5._
    
*   Universal: Fix incorrect light brightness when using SimpleLit shader ([UUM-7851](https://issuetracker.unity3d.com/issues/lights-appear-significantly-brighter-when-using-the-simple-lit-shader))  
    _Fixed in 2023.1.0a5._
    
*   Universal RP: Crash on UndoManager::RegisterUndoOperation when exiting Play Mode after saving changes in Shader Graph ([UUM-9631](https://issuetracker.unity3d.com/issues/crash-on-undomanager-registerundooperation-when-exiting-play-mode-after-saving-changes-in-shader-graph))
    
*   URP: Fixed SpeedTree Shadergraph causes errors spammed in console. (UUM-3126)  
    _First seen in 2023.1.0a1._  
    _Fixed in 2023.1.0a5._
    
*   Visual Effects: \[Visual Effects Graph\] Closing the VFX Window autosaves any changes applied (UUM-4767)