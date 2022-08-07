# Unity 2021.2.3
https://unity3d.com/unity/whats-new/2021.2.3

## Known Issues in 2021.2.3f1

<ul>
<li><p>2D:  Reordering "Sorting Layers" list causes Sprites to reference different Layer names and ID (<a href="https://issuetracker.unity3d.com/issues/2d-reordering-and-undoing-sorting-layer-list-causes-sprites-to-reference-different-layer-names-and-id">1376779</a>)</p></li>
<li><p>AI: NavMesh Agent can not pass through passable area between carving NavMesh Obstacles (<a href="https://issuetracker.unity3d.com/issues/navmesh-agent-can-not-pass-through-passable-area-between-carving-navmesh-obstacles">1346325</a>)</p></li>
<li><p>Android:  Sometimes text is not rendered when using OpengLES3 on a Xiaomi Redmi9A device. (<a href="https://issuetracker.unity3d.com/issues/android-the-text-is-missing-on-a-xiaomi-redmi9a-device">1347186</a>)</p></li>
<li><p>Android: * Devices might wake up from sleep when in split screen mode.<br></p> 
<ul>
<li>Chrome OS devices that support tablet mode might not pause apps when they are no longer visible.<br></li>
<li>Some Android devices may experience delayed resolution updates after resizing a window.<br></li>
<li>Minimum window size might not be respected properly on all Android devices.</li>
</ul></li>
<li><p>Asset Import Pipeline: Crash on OnDemandScheduler::SetStandbyWorkerCount when opening a project with a symbolic link in it (<a href="https://issuetracker.unity3d.com/issues/crash-on-ondemandscheduler-setstandbyworkercount-when-opening-a-project-with-a-symbolic-link-in-it">1370389</a>)</p></li>
<li><p>CodeEditors: Attaching an icon to a MonoBehaviour script disappears when Selecting the Game Object (<a href="https://issuetracker.unity3d.com/issues/attaching-an-icon-to-a-monobehaviour-script-disappears-when-selecting-the-game-object">1379500</a>)</p></li>
<li><p>CodeEditors: Crash on stopping debugging (<a href="https://issuetracker.unity3d.com/issues/crash-on-stopping-debugging">1355156</a>)</p></li>
<li><p>DirectX12:  Objects are not lighted in Game view when using SEGI system with Graphics API for Windows set to Direct3D12 (<a href="https://issuetracker.unity3d.com/issues/directx12-objects-are-not-lighted-in-game-view-when-using-segi-system-with-graphics-api-for-windows-set-to-direct3d12">1375746</a>)</p></li>
<li><p>HD RP: HDRP Template fills the Console with "Shader error...couldn't open include file" messages after building the project (<a href="https://issuetracker.unity3d.com/issues/hdrp-template-fills-the-console-with-shader-error-dot-dot-dot-couldnt-open-include-file-messages-after-building-the-project">1342989</a>)</p></li>
<li><p>IMGUI: List Elements in the PropertyField disappear when the window is displayed on the second screen (<a href="https://issuetracker.unity3d.com/issues/propertyfield-list-elements-disappear-when-the-window-is-displayed-on-the-second-screen">1371078</a>)</p></li>
<li><p>Input: Touch Input doesn't work in Play Mode when running an Editor on a Touchscreen device (<a href="https://issuetracker.unity3d.com/issues/touch-input-doesnt-work-in-play-mode-when-running-an-editor-on-a-touchscreen-device">1341159</a>)</p></li>
<li><p>Linux:  Player settings and other options are locked after script compilation (<a href="https://issuetracker.unity3d.com/issues/linux-player-settings-and-other-options-are-locked-after-script-compilation">1380015</a>)</p></li>
<li><p>Linux: Linux Editor crashes at "RegisterRuntimeInitializeAndCleanup::ExecuteCleanup()" when quitting from "Enter Safe Mode" prompt (<a href="https://issuetracker.unity3d.com/issues/linux-editor-crashes-at-registerruntimeinitializeandcleanup-executecleanup-when-quitting-from-enter-safe-mode-prompt">1374087</a>)</p></li>
<li><p>Linux: Linux Editor crashes at "__assert_fail_base.cold" when opening a project (<a href="https://issuetracker.unity3d.com/issues/linux-editor-crashes-at-assert-fail-base-dot-cold-when-opening-a-project">1375312</a>)</p></li>
<li><p>MacOS: Editor freezes when Vsync is enabled and Game View window is resized on macOS (<a href="https://issuetracker.unity3d.com/issues/apple-silicon-editor-freezes-when-resizing-game-view">1375973</a>)</p></li>
<li><p>MacOS: [OSX][Editor] DirectoryNotFoundException errors appear when a project is created inside a directory with unicode characters (<a href="https://issuetracker.unity3d.com/issues/multiple-directorynotfoundexception-errors-appear-when-a-project-is-created-inside-a-directory-with-unicode-characters">1377915</a>)</p></li>
<li><p>Progressive Lightmapper: Crash while sculpting Terrain and Baking Lightmaps (<a href="https://issuetracker.unity3d.com/issues/crash-while-sculpting-terrain">1266511</a>)</p></li>
<li><p>Progressive Lightmapper: [GPU PLM] Crash in (nvopencl64) clGetPlatformInfo after enabling Auto Generate checkbox at the end of GI Bake (<a href="https://issuetracker.unity3d.com/issues/gpu-plm-crash-in-nvopencl64-clgetplatforminfo-after-enabling-auto-generate-checkbox-at-the-end-of-gi-bake">1379762</a>)</p></li>
<li><p>Progressive Lightmapper: [GPU PLM] Fallback to CPU PLM in CL_INVALID_MEM_OBJECT after switching light color only and rebaking GI (<a href="https://issuetracker.unity3d.com/issues/gpu-plm-switch-light-color-only-and-rebake-causes-fallback">1356714</a>)</p></li>
<li><p>Scene Management: Instantiated FBX through code throws error after leaving Play Mode (<a href="https://issuetracker.unity3d.com/issues/instantiated-fbx-through-code-throws-error-after-leaving-play-mode">1363573</a>)</p></li>
<li><p>Scene Template: [Linux][HDRP] Editor crashes when opening HDRP Sample Scene Template Project (<a href="https://issuetracker.unity3d.com/issues/linux-hdrp-editor-crashes-when-opening-hdrp-sample-scene-template-project">1381237</a>)</p></li>
<li><p>Scripting: Crash in CombineMeshFiltersForStaticBatching after switching active additively loaded scenes and entering Play mode (<a href="https://issuetracker.unity3d.com/issues/crash-in-combinemeshfiltersforstaticbatching-after-switching-active-scenes-and-entering-play-mode">1377416</a>)</p></li>
<li><p>Scripting: Error CS8035 is thrown on opening a project when using rulesets (<a href="https://issuetracker.unity3d.com/issues/error-cs8035">1349517</a>)</p></li>
<li><p>Scripting: Only some assemblies fail to be loaded when assembly name does not match the file name (<a href="https://issuetracker.unity3d.com/issues/only-some-assemblies-fail-to-be-loaded-when-assembly-name-does-not-match-the-file-name">1345099</a>)</p></li>
<li><p>ShaderGraph: [General][AssetDB][URP] Adding URP to the project causes reimports of many assets and goes into infinite import loops (<a href="https://issuetracker.unity3d.com/issues/general-assetdb-urp-adding-urp-to-the-project-causes-reimports-of-many-assets-and-goes-into-infinite-import-loops">1374611</a>)</p></li>
<li><p>Shadows/Lights: Scene is brighter in Standalone player if it was open in the Editor at build time (<a href="https://issuetracker.unity3d.com/issues/scene-is-brighter-in-standalone-player-if-it-was-open-in-the-editor-at-build-time">1375015</a>)</p></li>
<li><p>Shuriken: [Particles] Inspector breaks and errors are thrown when the Material field is deleted from the Particle System (<a href="https://issuetracker.unity3d.com/issues/particles-inspector-breaks-and-errors-are-thrown-when-the-material-field-is-deleted-from-the-particle-system">1379541</a>)</p></li>
<li><p>Templates: Editor crashes when exiting and keeping a tutorial project (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-when-exiting-and-keeping-a-new-micrograme-project">1338299</a>)</p></li>
<li><p>Vulkan: [Editor] The Scene's GameObjects textures are seemingly random and change colours depending on the Scene's Camera pos. (<a href="https://issuetracker.unity3d.com/issues/vulkan-editor-the-scenes-gameobjects-textures-are-seemingly-random-and-change-colours-depending-on-the-scenes-camera-pos">1337772</a>)</p></li>
<li><p>Window Management: Broken layout stops panels located in the top left corner of the Editor from rendering in the Karting Microgame project (<a href="https://issuetracker.unity3d.com/issues/broken-layout-stops-panels-located-in-the-top-left-corner-of-the-editor-from-rendering-in-the-karting-microgame-project">1367783</a>)</p></li>
<li><p>XR SDK: Severe flickering in Unity 2020.3.21f1 with OpenXR on HL2 (<a href="https://issuetracker.unity3d.com/issues/severe-flickering-in-unity-2020-dot-3-21f1-with-openxr-on-hl2">1376203</a>)</p></li>
<li><p>XR SDK: [XR][Linux] Scene View doesn't render when opening new AR or VR Template project or pressing "Show Tutorials" (<a href="https://issuetracker.unity3d.com/issues/xr-linux-scene-view-doesnt-render-when-opening-new-ar-or-vr-template-project-or-pressing-show-tutorials">1362435</a>)</p></li>
</ul>
