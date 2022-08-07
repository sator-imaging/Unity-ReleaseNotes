# Unity 2021.2.1
https://unity3d.com/unity/whats-new/2021.2.1

## Known Issues in 2021.2.1f1

<ul>
<li><p>Android:  Sometimes text is not rendered when using OpengLES3 on a Xiaomi Redmi9A device. (<a href="https://issuetracker.unity3d.com/issues/android-the-text-is-missing-on-a-xiaomi-redmi9a-device">1347186</a>)</p></li>
<li><p>Android: * Devices might wake up from sleep when in split screen mode.<br></p> 
<ul>
<li>Chrome OS devices that support tablet mode might not pause apps when they are no longer visible.<br></li>
<li>Some Android devices may experience delayed resolution updates after resizing a window.<br></li>
<li>Minimum window size might not be respected properly on all Android devices.</li>
</ul></li>
<li><p>Asset Bundles: Building process of the AssetBundles is slow when there is a huge filecount. (<a href="https://issuetracker.unity3d.com/issues/building-process-of-the-assetbundles-is-slow-when-the-file-count-is-huge">1358059</a>)</p></li>
<li><p>Asset Import Pipeline: Crash on OnDemandScheduler::SetStandbyWorkerCount when opening a project with a symbolic link in it (<a href="https://issuetracker.unity3d.com/issues/crash-on-ondemandscheduler-setstandbyworkercount-when-opening-a-project-with-a-symbolic-link-in-it">1370389</a>)</p></li>
<li><p>CodeEditors: Crash on stopping debugging (<a href="https://issuetracker.unity3d.com/issues/crash-on-stopping-debugging">1355156</a>)</p></li>
<li><p>Customer QA Onboarding: Entering values into value fields in the Inspector window is delayed (<a href="https://issuetracker.unity3d.com/issues/entering-values-into-value-fields-in-the-inspector-window-is-delayed">1374222</a>)</p></li>
<li><p>Customer QA Onboarding: [macOS] Text input lags by one keystroke when inputting text in the Editor (<a href="https://issuetracker.unity3d.com/issues/text-input-lags-by-one-keystroke-when-inputting-text-in-the-editor">1376732</a>)</p></li>
<li><p>Global Illumination: Crash while sculpting Terrain and Baking Lightmaps (<a href="https://issuetracker.unity3d.com/issues/crash-while-sculpting-terrain">1266511</a>)</p></li>
<li><p>Global Illumination: Scene is brighter in Standalone player if it was open in the Editor at build time (<a href="https://issuetracker.unity3d.com/issues/scene-is-brighter-in-standalone-player-if-it-was-open-in-the-editor-at-build-time">1375015</a>)</p></li>
<li><p>Global Illumination: [GPU PLM] Fallback to CPU PLM in CL_INVALID_MEM_OBJECT after switching light color only and rebaking GI (<a href="https://issuetracker.unity3d.com/issues/gpu-plm-switch-light-color-only-and-rebake-causes-fallback">1356714</a>)</p></li>
<li><p>HD RP: HDRP Template fills the Console with "Shader error...couldn't open include file" messages after building the project (<a href="https://issuetracker.unity3d.com/issues/hdrp-template-fills-the-console-with-shader-error-dot-dot-dot-couldnt-open-include-file-messages-after-building-the-project">1342989</a>)</p></li>
<li><p>IL2CPP: System.Runtime.Serialization.Formatters.BinaryFormatter doesn't work when Project is build with IL2CPP Scripting Backend (<a href="https://issuetracker.unity3d.com/issues/il2cpp-system-dot-runtime-dot-serialization-dot-formatters-dot-binaryformatter-doesnt-work-when-project-is-build-with-il2cpp-scripting-backend">1374185</a>)</p></li>
<li><p>Input: The first Keyboard Input is Ignored and stored for later when renaming Assets causing all Keyboard Inputs to become mixed (<a href="https://issuetracker.unity3d.com/issues/the-first-keyboard-input-is-ignored-and-stored-for-later-when-renaming-assets-causing-all-keyboard-inputs-to-become-mixed">1375664</a>)</p></li>
<li><p>Input: Touch Input doesn't work in Play Mode when running an Editor on a Touchscreen device (<a href="https://issuetracker.unity3d.com/issues/touch-input-doesnt-work-in-play-mode-when-running-an-editor-on-a-touchscreen-device">1341159</a>)</p></li>
<li><p>Inspector Framework: Long Layer names are not fully visible in the drop-down list when selecting it in the Inspector window from Script component  (<a href="https://issuetracker.unity3d.com/issues/long-layer-names-are-not-fully-visible-in-the-drop-down-list-when-selecting-it-in-the-inspector-window-from-script-component">1366623</a>)</p></li>
<li><p>Linux: Linux Editor crashes at "__assert_fail_base.cold" when opening a project (<a href="https://issuetracker.unity3d.com/issues/linux-editor-crashes-at-assert-fail-base-dot-cold-when-opening-a-project">1375312</a>)</p></li>
<li><p>MacOS: [Mac] Performance regression in Editor UI (<a href="https://issuetracker.unity3d.com/issues/mac-performance-regression-in-editor-ui">1376273</a>)</p></li>
<li><p>Mono: .NETStandard 2.1 in the editor is missing System.Memory, System.Buffers at runtime (<a href="https://issuetracker.unity3d.com/issues/dot-netstandard-2-dot-1-in-the-editor-is-missing-system-dot-memory-system-dot-buffers-at-runtime">1367105</a>)</p></li>
<li><p>Mono: Microsoft.Extensions.Logging Nuget Package causes errors in console when built into UWP with .NET Standard 2.1 (<a href="https://issuetracker.unity3d.com/issues/microsoft-dot-extensions-dot-logging-nuget-package-causes-errors-in-console-when-built-into-uwp-with-net-standard-2-dot-1">1373389</a>)</p></li>
<li><p>Mono: NullReferenceException causes freeze when thrown in the Player (<a href="https://issuetracker.unity3d.com/issues/nullreferenceexception-causes-freeze-when-thrown-in-the-built-project">1364311</a>)</p></li>
<li><p>Profiling: Profiler's timeline view loses context frames when frames go out of Frame Count bounds (<a href="https://issuetracker.unity3d.com/issues/timeline-view-looses-context-frames-when-frames-go-out-of-frame-count-bounds">1367470</a>)</p></li>
<li><p>Scene Management: GameObjects, Parameters, and Windows doesn't update correctly on the last steps when doing Undo and Redo (<a href="https://issuetracker.unity3d.com/issues/gameobjects-parameters-and-windows-doesnt-update-correctly-on-the-last-steps-when-doing-undo-and-redo">1374538</a>)</p></li>
<li><p>Scene Management: Instantiated FBX through code throws error after leaving Play Mode (<a href="https://issuetracker.unity3d.com/issues/instantiated-fbx-through-code-throws-error-after-leaving-play-mode">1363573</a>)</p></li>
<li><p>Scene/Game View: Tool handles are invisible in Scene View when certain objects are selected (<a href="https://issuetracker.unity3d.com/issues/tool-handles-are-invisible-in-scene-view-when-certain-objects-are-selected">1374532</a>)</p></li>
<li><p>Scripting: Crash in CombineMeshFiltersForStaticBatching after switching active additively loaded scenes and entering Play mode (<a href="https://issuetracker.unity3d.com/issues/crash-in-combinemeshfiltersforstaticbatching-after-switching-active-scenes-and-entering-play-mode">1377416</a>)</p></li>
<li><p>Scripting: Error CS8035 is thrown on opening a project when using rulesets (<a href="https://issuetracker.unity3d.com/issues/error-cs8035">1349517</a>)</p></li>
<li><p>Scripting: Only some assemblies fail to be loaded when assembly name does not match the file name (<a href="https://issuetracker.unity3d.com/issues/only-some-assemblies-fail-to-be-loaded-when-assembly-name-does-not-match-the-file-name">1345099</a>)</p></li>
<li><p>Shader System: Shaders are ignored when executing Build Asset Bundles method from console with -nographics argument (<a href="https://issuetracker.unity3d.com/issues/shaders-are-ignored-when-executing-build-asset-bundles-method-from-console-with-nographics-argument">1369645</a>)</p></li>
<li><p>Templates: Editor crashes when exiting and keeping a tutorial project (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-when-exiting-and-keeping-a-new-micrograme-project">1338299</a>)</p></li>
<li><p>uGUI:  Poor performance when loading or unloading a large Scene (<a href="https://issuetracker.unity3d.com/issues/poor-performance-when-loading-or-unloading-a-large-scene-1">1375646</a>)</p></li>
<li><p>Universal Windows Platform: UnityWebRequest fails on UWP with HTTPS (<a href="https://issuetracker.unity3d.com/issues/unitywebrequest-fails-on-uwp-with-https">1375004</a>)</p></li>
<li><p>Vulkan: [Editor] The Scene's GameObjects textures are seemingly random and change colours depending on the Scene's Camera pos. (<a href="https://issuetracker.unity3d.com/issues/vulkan-editor-the-scenes-gameobjects-textures-are-seemingly-random-and-change-colours-depending-on-the-scenes-camera-pos">1337772</a>)</p></li>
<li><p>Window Management: Broken layout stops panels located in the top left corner of the Editor from rendering in the Karting Microgame project (<a href="https://issuetracker.unity3d.com/issues/broken-layout-stops-panels-located-in-the-top-left-corner-of-the-editor-from-rendering-in-the-karting-microgame-project">1367783</a>)</p></li>
<li><p>XR SDK: Severe flickering in Unity 2020.3.21f1 with OpenXR on HL2 (<a href="https://issuetracker.unity3d.com/issues/severe-flickering-in-unity-2020-dot-3-21f1-with-openxr-on-hl2">1376203</a>)</p></li>
<li><p>XR SDK: [XR][Linux] Scene View doesn't render when opening new AR or VR Template project or pressing "Show Tutorials" (<a href="https://issuetracker.unity3d.com/issues/xr-linux-scene-view-doesnt-render-when-opening-new-ar-or-vr-template-project-or-pressing-show-tutorials">1362435</a>)</p></li>
</ul>
