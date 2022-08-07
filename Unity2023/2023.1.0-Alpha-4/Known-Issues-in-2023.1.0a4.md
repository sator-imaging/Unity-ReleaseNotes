# Unity 2023.1.0 Alpha 4
https://unity3d.com/unity/alpha/2023.1.0a4

## Known Issues in 2023.1.0a4

<ul>
<li><p>2D: [Lost Crypt] Unable to find URP 12.1.0 package error when importing Lost Crypt (<a href="https://issuetracker.unity3d.com/issues/2d-lost-crypt-unable-to-find-urp-12-dot-1-0-package-error-when-importing-lost-crypt">1388129</a>)</p></li>
<li><p>AI Navigation Core: NavMesh::Raycast freezes the whole editor in an infinite loop on Application.UpdateScene (<a href="https://issuetracker.unity3d.com/issues/navmesh-raycast-freezes-the-whole-editor-in-an-infinite-loop-on-application-dot-updatescene">UUM-2496</a>)</p></li>
<li><p>Asset - Database: Infinite import on opening project (related to prefabs) (<a href="https://issuetracker.unity3d.com/issues/infinite-import-on-opening-project-related-to-prefabs">1411189</a>)</p></li>
<li><p>DirectX12: Camera.Render causes a memory leak in HDRP using DirectX 12 (<a href="https://issuetracker.unity3d.com/issues/camera-dot-render-causes-a-memory-leak-in-hdrp-using-directx-12-1">UUM-5879</a>)</p></li>
<li><p>DOTS: Crash when creating Assembly Definition Asset while Unity Logging package is installed (<a href="https://issuetracker.unity3d.com/issues/crash-when-creating-assembly-definition-asset-while-unity-logging-package-is-installed">UUM-8727</a>)</p></li>
<li><p>Editor: Fix the TimeManager for DragAndDropForwarding tests (UUM-6233)<br>
<em>First seen in 2023.1.0a1.</em>    <br><em>Fixed in 2023.1.0a5.</em></p></li>
<li><p>HD RP: [HDRP] "No more space in Reflection Probe Atlas" error is spammed on creating a HDRP 3D Sample Template (<a href="https://issuetracker.unity3d.com/issues/hdrp-no-more-space-in-reflection-probe-atlas-error-is-spammed-on-creating-a-hdrp-3d-sample-template">UUM-5735</a>)</p></li>
<li><p>IL2CPP: Fixed incorrect code generation for references to void* pointers. (<a href="https://issuetracker.unity3d.com/issues/il2cpp-build-fails-when-code-has-public-ref-void-star-this-int-index-function">UUM-4299</a>)    <br><em>Fixed in 2023.1.0a5.</em></p></li>
<li><p>IL2CPP: Linux IL2CPP builds fail with "BuildFailedException: Incremental Player build failed!" (<a href="https://issuetracker.unity3d.com/issues/linux-il2cpp-builds-fail-with-buildfailedexception-incremental-player-build-failed">1427577</a>)</p></li>
<li><p>Incremental Build Pipeline: [iOS] Building an iOS project for Simulator fails in Xcode (<a href="https://issuetracker.unity3d.com/issues/ios-building-a-project-for-simulator-fails-in-xcode">UUM-9393</a>)</p></li>
<li><p>MacOS: [Mac] Editor performance drops on macOS when clicking and dragging on Position, Rotation and Scale values in Transform component  (<a href="https://issuetracker.unity3d.com/issues/mac-editor-performance-drops-on-macos-when-clicking-and-dragging-on-position-rotation-and-scale-values-in-transform-component">UUM-7457</a>)</p></li>
<li><p>Package Manager: Keyboard navigation in package manager has been fixed. We can now properly use up/down, page up/down with optional shift key in asset tab. (UUM-6478)    <br><em>Fixed in 2023.1.0a5.</em></p></li>
<li><p>Prefabs: Fix after 'Apply All' is clicked in the overrides window then properties are still shown as overriden (UUM-6917)<br>
<em>First seen in 2023.1.0a1.</em>    <br><em>Fixed in 2023.1.0a5.</em></p></li>
<li><p>Profiling: Profiler Modules submenu and window is missing Titles of Modules and Counters (<a href="https://issuetracker.unity3d.com/issues/profiler-modules-submenu-and-window-is-missing-titles-of-modules-and-counters">1419236</a>)</p></li>
<li><p>RP Workflow: [HDRP] Standalone Profiler throws "HDRP Material Upgrade" pop-up and crashes after pressing "Ok" (<a href="https://issuetracker.unity3d.com/issues/hdrp-standalone-profiler-throws-hdrp-material-upgrade-pop-up-and-crashes-after-pressing-ok">1422062</a>)</p></li>
<li><p>Scene Management: Scene causes Editor crash when specific Lighting Data Asset is used (<a href="https://issuetracker.unity3d.com/issues/scene-causes-editor-crash-when-specific-lighting-data-asset-is-used">UUM-9319</a>)</p></li>
<li><p>Scene Management: Undo crashes Unity with segmentation violation SIGSEGV (<a href="https://issuetracker.unity3d.com/issues/undo-crashes-unity-with-segmentation-violation-sigsegv">1385565</a>)</p></li>
<li><p>Scene Management: [Undo] Additional GameObjects and a Console error after Undoing and Redoing a Paste As Child (<a href="https://issuetracker.unity3d.com/issues/additional-gameobjects-and-a-console-error-after-undoing-and-redoing-a-paste-as-child">UUM-9278</a>)</p></li>
<li><p>Shader System: Crash on ComputeShader::SetValueParam when opening a certain Scene (<a href="https://issuetracker.unity3d.com/issues/crash-on-computeshader-setvalueparam-when-opening-a-certain-scene">UUM-495</a>)</p></li>
<li><p>Shader System: Shader variant build preparation does not scale (UUM-3711)</p></li>
<li><p>Shadergraph: Fix the TimeManager for MaterialVariant tests (UUM-8013)<br>
<em>First seen in 2023.1.0a3.</em>    <br><em>Fixed in 2023.1.0a5.</em></p></li>
<li><p>Shadows/Lights: Scene is brighter in Standalone player if it was open in the Editor at build time (<a href="https://issuetracker.unity3d.com/issues/scene-is-brighter-in-standalone-player-if-it-was-open-in-the-editor-at-build-time">1375015</a>)</p></li>
<li><p>uGUI: UI Components OnCursorEnter state is ended when hovering cursor over smaller sized child UI objects (<a href="https://issuetracker.unity3d.com/issues/ui-components-oncursorenter-state-is-ended-when-hovering-cursor-over-smaller-sized-child-ui-objects">UUM-505</a>)</p></li>
<li><p>UI Toolkit: Fixed inspector alignment. (UUM-3476)<br>
<em>First seen in 2023.1.0a1.</em>    <br><em>Fixed in 2023.1.0a5.</em></p></li>
<li><p>UI Toolkit: Improved performance of the UITK NonReorderable and Reorderable ListView in the inspector. (UUM-3483)<br>
<em>First seen in 2023.1.0a1.</em>    <br><em>Fixed in 2023.1.0a5.</em></p></li>
<li><p>Undo System: Fix the TimeManager for UndoManager tests (UUM-8019)<br>
<em>First seen in 2023.1.0a3.</em>    <br><em>Fixed in 2023.1.0a5.</em></p></li>
<li><p>Universal: Fix depth pre-pass being always executed on GLES devices (<a href="https://issuetracker.unity3d.com/issues/urp-depth-pre-pass-is-always-executed-regardless-of-project-slash-pipeline-settings-when-opengles3-graphics-api-is-used">UUM-8381</a>)    <br><em>Fixed in 2023.1.0a5.</em></p></li>
<li><p>Universal: Fix incorrect light brightness when using SimpleLit shader (<a href="https://issuetracker.unity3d.com/issues/lights-appear-significantly-brighter-when-using-the-simple-lit-shader">UUM-7851</a>)    <br><em>Fixed in 2023.1.0a5.</em></p></li>
<li><p>Universal RP: Crash on UndoManager::RegisterUndoOperation when exiting Play Mode after saving changes in Shader Graph (<a href="https://issuetracker.unity3d.com/issues/crash-on-undomanager-registerundooperation-when-exiting-play-mode-after-saving-changes-in-shader-graph">UUM-9631</a>)</p></li>
<li><p>URP: Fixed SpeedTree Shadergraph causes errors spammed in console. (UUM-3126)<br>
<em>First seen in 2023.1.0a1.</em>    <br><em>Fixed in 2023.1.0a5.</em></p></li>
<li><p>Visual Effects: [Visual Effects Graph] Closing the VFX Window autosaves any changes applied (UUM-4767)</p></li>
</ul>
