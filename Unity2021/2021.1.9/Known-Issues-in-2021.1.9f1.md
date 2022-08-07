# Unity 2021.1.9
https://unity3d.com/unity/whats-new/2021.1.9

## Known Issues in 2021.1.9f1

<ul>
<li><p>2D: [URP] The Camera renders black screen when Post Processing is enabled in the 2D Renderer and in the Camera Component (<a href="https://issuetracker.unity3d.com/issues/urp-the-camera-renders-black-screen-when-post-processing-is-enabled-in-the-2d-renderer-and-in-the-camera-component">1318500</a>)</p></li>
<li><p>AI: Crash with ComputeTileMeshJob when generating Navmesh (<a href="https://issuetracker.unity3d.com/issues/crash-with-computetilemeshjob-when-generating-navmesh">1329346</a>)</p></li>
<li><p>Animation: [Performance Regression] AnimationWindowState:get_allCurves takes approximately 5000ms to load animation in the Animation window (<a href="https://issuetracker.unity3d.com/issues/perfomance-regression-animationwindowstate-get-allcurves-takes-approximately-5000ms-to-load-animation-in-the-animation-window">1320250</a>)</p></li>
<li><p>Asset Import Pipeline: Editor crashes when executing Undo action after Audio Source component is added to Prefab (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-when-executing-undo-action-after-audio-source-component-is-added-to-prefab">1335691</a>)</p></li>
<li><p>Audio: AudioMixer exposed parameters cause assertions when hidden and prevent the drop-down from functioning (<a href="https://issuetracker.unity3d.com/issues/audiomixer-exposed-parameters-cause-assertions-when-hidden-and-prevent-the-drop-down-from-functioning">1336173</a>)</p></li>
<li><p>Global Illumination: Reflection probes don't contain indirect scene lighting after the on-demand GI bake from the Lighting window (<a href="https://issuetracker.unity3d.com/issues/reflection-probes-doesnt-contain-indirect-scene-lighting-after-the-on-demand-gi-bake-from-the-lighting-window">1324246</a>)</p></li>
<li><p>Global Illumination: Reflection probes must be rebaked twice to update when using "Generate Lighting" button (<a href="https://issuetracker.unity3d.com/issues/reflection-probes-must-be-rebaked-twice-to-update-when-using-generate-lighting-button">1334283</a>)</p></li>
<li><p>Global Illumination: [GPUPLM] Crash in RadeonRaysMeshManager::RemoveGeometry while baking Terrain game object with 4k lightmaps on certain GPU (<a href="https://issuetracker.unity3d.com/issues/global-illumination-editor-crashes-while-baking-terrain-game-object-using-progressive-gpu-lightmapper">1255993</a>)</p></li>
<li><p>HD RP: Editor crashes on GfxDeviceD3D12Base::DrawBuffersCommon when switching between Scenes (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-on-gfxdeviced3d12base-drawbufferscommon-when-switching-between-scenes">1329083</a>)</p></li>
<li><p>IL2CPP:  Build fails when using a combination of messages, SyncVars and SyncList in a project (<a href="https://issuetracker.unity3d.com/issues/il2cpp-build-fails-when-using-a-combination-of-messages-syncvars-and-synclist-in-a-project">1328966</a>)</p></li>
<li><p>IMGUI: Contents of a ModalUtility window are invisible when it is launched from a Unity Context Menu (<a href="https://issuetracker.unity3d.com/issues/error-displaying-showmodalutility-window">1313636</a>)</p></li>
<li><p>Linux: Linux Editor crashes at "_XFreeX11XCBStructure" when loading tutorials (<a href="https://issuetracker.unity3d.com/issues/linux-editor-crashes-at-xfreex11xcbstructure-when-loading-tutorials">1323204</a>)</p></li>
<li><p>Metal: Performance in Game View is significantly impacted by Gfx.WaitForPresentOnGfxThread when a second monitor is connected (<a href="https://issuetracker.unity3d.com/issues/performance-in-game-view-is-significantly-impacted-by-gfx-dot-waitforpresentongfxthread-when-a-second-monitor-is-connected">1327408</a>)</p></li>
<li><p>Mobile: [Android] App stops due to OnPixelCopyFinishedListener not being supported on devices with lower than 24 SDK (<a href="https://issuetracker.unity3d.com/issues/app-stops-due-to-onpixelcopyfinishedlistener-not-being-supported-on-devices-with-lower-than-24-sdk">1331290</a>)</p></li>
<li><p>Mobile: [Android] Time.deltaTime value becomes constant 0.3(3) after sending to the background and resuming an Application (<a href="https://issuetracker.unity3d.com/issues/android-time-dot-deltatime-value-becomes-constant-0-dot-3-3-after-sending-to-the-background-and-resuming-an-application">1328545</a>)</p></li>
<li><p>Mono: [macOS] Unity crashes when exception thrown after a DLL has been loaded (<a href="https://issuetracker.unity3d.com/issues/macos-unity-crashes-when-exception-thrown-after-a-dll-has-been-loaded">1318755</a>)</p></li>
<li><p>OpenGL: SRP Batcher not working with OpenGL APIs when the project is built (<a href="https://issuetracker.unity3d.com/issues/srp-batcher-not-working-with-opengl-apis-when-the-project-is-built">1331098</a>)</p></li>
<li><p>Packman: User can't easily configure location of both UPM and Asset Store package local cache (<a href="https://issuetracker.unity3d.com/issues/user-cant-easily-configure-location-of-both-upm-and-asset-store-package-local-cache">1317232</a>)</p></li>
<li><p>Profiling: GarbageCollectAssets is triggered frequently when higher frame counts are set (<a href="https://issuetracker.unity3d.com/issues/garbagecollectassets-is-triggered-frequently-when-higher-frame-counts-are-set">1332708</a>)</p></li>
<li><p>Scene Management: Crash on BuildPrefabInstanceCorrespondingObjectMap when overriding nested prefab inside AssetDatabase.StartAssetEditing() block (<a href="https://issuetracker.unity3d.com/issues/crash-on-buildprefabinstancecorrespondingobjectmap-when-overriding-nested-prefab-inside-assetdatabase-dot-startassetediting-block">1324978</a>)</p></li>
<li><p>Scripting: Crashes on mono_class_init when entering Play Mode after recompiling scripts (<a href="https://issuetracker.unity3d.com/issues/crashes-on-mono-class-init-when-entering-play-mode-after-recompiling-scripts">1262671</a>)</p></li>
<li><p>Scripting: Increased Script Assembly reload time (<a href="https://issuetracker.unity3d.com/issues/increased-reload-time">1323490</a>)</p></li>
<li><p>Serialization: Crash in SerializedProperty::IsValid when reordering a SerializedProperty list (<a href="https://issuetracker.unity3d.com/issues/crash-in-serializedproperty-isvalid-when-reordering-a-serializedproperty-list">1320319</a>)</p></li>
<li><p>Terrain: Terrain Lit Opacity as Density option causes alpha'd areas on the 5th layer or greater to appear with artifacts (<a href="https://issuetracker.unity3d.com/issues/terrain-lit-opacity-as-density-option-causes-alphad-areas-on-the-5th-layer-or-greater-to-appear-with-artifacts">1283124</a>)</p></li>
<li><p>uGUI: RectMask2D Softness property has no effect when used on TextMeshPro Text (<a href="https://issuetracker.unity3d.com/issues/rectmask2d-softness-property-has-no-effect-when-used-on-textmeshpro-text">1331297</a>)</p></li>
</ul>