# Unity 2021.1.10

https://unity3d.com/unity/whats-new/2021.1.10

## Known Issues in 2021.1.10f1



*   2D: \[URP\] The Camera renders black screen when Post Processing is enabled in the 2D Renderer and in the Camera Component ([1318500](https://issuetracker.unity3d.com/issues/urp-the-camera-renders-black-screen-when-post-processing-is-enabled-in-the-2d-renderer-and-in-the-camera-component))
    
*   AI: Crash with ComputeTileMeshJob when generating Navmesh ([1329346](https://issuetracker.unity3d.com/issues/crash-with-computetilemeshjob-when-generating-navmesh))
    
*   Animation: \[Performance Regression\] AnimationWindowState:get\_allCurves takes approximately 5000ms to load animation in the Animation window ([1320250](https://issuetracker.unity3d.com/issues/perfomance-regression-animationwindowstate-get-allcurves-takes-approximately-5000ms-to-load-animation-in-the-animation-window))
    
*   Asset Import Pipeline: Infinity loop on importing Assets, when building appx package via MRTK build window ([1339823](https://issuetracker.unity3d.com/issues/infinity-loop-on-importing-assets-when-building-appx-package-via-mrtk-build-window))
    
*   Cloth: Cloth component assigned to subdivided plane mesh crashes editor ([1337649](https://issuetracker.unity3d.com/issues/cloth-cloth-component-assigned-to-subdivided-plane-mesh-crashes-editor))
    
*   Global Illumination: Reflection probes don't contain indirect scene lighting after the on-demand GI bake from the Lighting window ([1324246](https://issuetracker.unity3d.com/issues/reflection-probes-doesnt-contain-indirect-scene-lighting-after-the-on-demand-gi-bake-from-the-lighting-window))
    
*   Global Illumination: Reflection probes must be rebaked twice to update when using "Generate Lighting" button ([1334283](https://issuetracker.unity3d.com/issues/reflection-probes-must-be-rebaked-twice-to-update-when-using-generate-lighting-button))
    
*   Global Illumination: \[GPUPLM\] Crash in RadeonRaysMeshManager::RemoveGeometry while baking Terrain game object with 4k lightmaps on certain GPU ([1255993](https://issuetracker.unity3d.com/issues/global-illumination-editor-crashes-while-baking-terrain-game-object-using-progressive-gpu-lightmapper))
    
*   HD RP: Editor crashes on GfxDeviceD3D12Base::DrawBuffersCommon when switching between Scenes ([1329083](https://issuetracker.unity3d.com/issues/editor-crashes-on-gfxdeviced3d12base-drawbufferscommon-when-switching-between-scenes))
    
*   IL2CPP: Build fails when using a combination of messages, SyncVars and SyncList in a project ([1328966](https://issuetracker.unity3d.com/issues/il2cpp-build-fails-when-using-a-combination-of-messages-syncvars-and-synclist-in-a-project))
    
*   IMGUI: Contents of a ModalUtility window are invisible when it is launched from a Unity Context Menu ([1313636](https://issuetracker.unity3d.com/issues/error-displaying-showmodalutility-window))
    
*   Linux: Editor crashes at "GfxFramebufferGLES::SetBackBufferColorDepthSurface" or freezes when creating a new shortcut profile ([1334874](https://issuetracker.unity3d.com/issues/editor-crashes-at-gfxframebuffergles-setbackbuffercolordepthsurface-or-freezes-when-creating-a-new-shortcut-profile))
    
*   Linux: Linux Editor crashes at "\_XFreeX11XCBStructure" when loading tutorials ([1323204](https://issuetracker.unity3d.com/issues/linux-editor-crashes-at-xfreex11xcbstructure-when-loading-tutorials))
    
*   Metal: Performance in Game View is significantly impacted by Gfx.WaitForPresentOnGfxThread when a second monitor is connected ([1327408](https://issuetracker.unity3d.com/issues/performance-in-game-view-is-significantly-impacted-by-gfx-dot-waitforpresentongfxthread-when-a-second-monitor-is-connected))
    
*   Mobile: \[Android\] App stops due to OnPixelCopyFinishedListener not being supported on devices with lower than 24 SDK ([1331290](https://issuetracker.unity3d.com/issues/app-stops-due-to-onpixelcopyfinishedlistener-not-being-supported-on-devices-with-lower-than-24-sdk))
    
*   Mobile Graphics: \[iOS\] Player crashing when connecting external Display via USB-C port ([1321153](https://issuetracker.unity3d.com/issues/ios-player-crashing-when-connecting-external-display-via-usb-c-port))
    
*   Mono: \[macOS\] Unity crashes when exception thrown after a DLL has been loaded ([1318755](https://issuetracker.unity3d.com/issues/macos-unity-crashes-when-exception-thrown-after-a-dll-has-been-loaded))
    
*   OpenGL: SRP Batcher not working with OpenGL APIs when the project is built ([1331098](https://issuetracker.unity3d.com/issues/srp-batcher-not-working-with-opengl-apis-when-the-project-is-built))
    
*   Packman: User can't easily configure location of both UPM and Asset Store package local cache ([1317232](https://issuetracker.unity3d.com/issues/user-cant-easily-configure-location-of-both-upm-and-asset-store-package-local-cache))
    
*   Profiling: GarbageCollectAssets is triggered frequently when higher frame counts are set ([1332708](https://issuetracker.unity3d.com/issues/garbagecollectassets-is-triggered-frequently-when-higher-frame-counts-are-set))
    
*   Profiling: Poor profiler performance when navigating the timeline view and reviewing data with many threads ([1339407](https://issuetracker.unity3d.com/issues/poor-profiler-performance-when-navigating-the-timeline-view-and-reviewing-data-with-many-threads))
    
*   Scene Management: Crash on BuildPrefabInstanceCorrespondingObjectMap when overriding nested prefab inside AssetDatabase.StartAssetEditing() block ([1324978](https://issuetracker.unity3d.com/issues/crash-on-buildprefabinstancecorrespondingobjectmap-when-overriding-nested-prefab-inside-assetdatabase-dot-startassetediting-block))
    
*   Scene/Game View: Editor crashes when exiting and keeping a new microgame project ([1338299](https://issuetracker.unity3d.com/issues/editor-crashes-when-exiting-and-keeping-a-new-micrograme-project))
    
*   Scripting: Crashes on mono\_class\_init when entering Play Mode after recompiling scripts ([1262671](https://issuetracker.unity3d.com/issues/crashes-on-mono-class-init-when-entering-play-mode-after-recompiling-scripts))
    
*   Scripting: Increased Script Assembly reload time ([1323490](https://issuetracker.unity3d.com/issues/increased-reload-time))
    
*   Serialization: Crash in SerializedProperty::IsValid when reordering a SerializedProperty list ([1320319](https://issuetracker.unity3d.com/issues/crash-in-serializedproperty-isvalid-when-reordering-a-serializedproperty-list))
    
*   Terrain: Terrain Lit Opacity as Density option causes alpha'd areas on the 5th layer or greater to appear with artifacts ([1283124](https://issuetracker.unity3d.com/issues/terrain-lit-opacity-as-density-option-causes-alphad-areas-on-the-5th-layer-or-greater-to-appear-with-artifacts))
    
*   uGUI: RectMask2D Softness property has no effect when used on TextMeshPro Text ([1331297](https://issuetracker.unity3d.com/issues/rectmask2d-softness-property-has-no-effect-when-used-on-textmeshpro-text))