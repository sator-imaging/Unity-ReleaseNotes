# Unity 2021.1.1

https://unity3d.com/unity/whats-new/2021.1.1

## Known Issues in 2021.1.1f1



*   Asset Importers: \[Performance Regression\] Importing an fbx model is noticeably slower when the model contains Animations ([1265275](https://issuetracker.unity3d.com/issues/performance-regression-importing-an-fbx-model-is-noticeably-slower-when-the-model-contains-animations))
    
*   Asset Bundles: Synchronous Asset Loading Does Not Correctly Load Preload Dependencies ([1321141](https://issuetracker.unity3d.com/issues/synchronous-asset-loading-does-not-correctly-load-preload-dependencies))
    
*   Cloth: Cloth is broken when parent GameObject scale is lower than 1 and Surface Penetration constraints are set 0 ([1319488](https://issuetracker.unity3d.com/issues/cloth-is-broken-when-parent-gameobject-scale-is-lower-than-1-and-surface-penetration-constraints-are-set-0))
    
*   Global Illumination: Wintermute::Geometry::Verify errors are spammed when baking a Mesh with Mesh Compression set to Medium/High ([1319133](https://issuetracker.unity3d.com/issues/speedtree-asset-breaks-when-trying-to-lightmap))
    
*   Linux: Linux Editor crashes at "\_XFreeX11XCBStructure" when loading tutorials ([1323204](https://issuetracker.unity3d.com/issues/linux-editor-crashes-at-xfreex11xcbstructure-when-loading-tutorials))
    
*   Scripting: Increased Script Assembly reload time ([1323490](https://issuetracker.unity3d.com/issues/increased-reload-time))
    
*   Terrain: Crash on TreeRenderer::WillRenderTrees when being in Play Mode for several seconds ([1317966](https://issuetracker.unity3d.com/issues/crash-on-treerenderer-willrendertrees-when-being-in-play-mode-for-several-seconds))
    
*   IMGUI: Contents of a ModalUtility window are invisible when it is launched from a Unity Context Menu ([1313636](https://issuetracker.unity3d.com/issues/error-displaying-showmodalutility-window))
    
*   Global Illumination: Reflection probes doesn't contain indirect scene lighting after the on-demand GI bake from the Lighting window ([1324246](https://issuetracker.unity3d.com/issues/reflection-probes-doesnt-contain-indirect-scene-lighting-after-the-on-demand-gi-bake-from-the-lighting-window))
    
*   Addressable Assets: Performance bug reported by the DOTS team in PreloadManager::WaitForAllOperationToComplete ([1322086](https://issuetracker.unity3d.com/issues/performance-bug-reported-by-the-dots-team-in-preloadmanager-waitforalloperationtocomplete))
    
*   Packman: User can't easily configure location of both UPM and Asset Store package local cache ([1317232](https://issuetracker.unity3d.com/issues/user-cant-easily-configure-location-of-both-upm-and-asset-store-package-local-cache))
    
*   Serialization: Crash in SerializedProperty::IsValid when reordering a SerializedProperty list ([1320319](https://issuetracker.unity3d.com/issues/crash-in-serializedproperty-isvalid-when-reordering-a-serializedproperty-list))
    
*   Windows: \[Windows 7\] "WindowsVideoMedia error 0xc00d36b4" error is thrown when loading a video with the VideoPlayer ([1306350](https://issuetracker.unity3d.com/issues/windows-7-windowsvideomedia-error-0xc00d36b4-error-is-thrown-when-loading-a-video-with-the-videoplayer))
    
*   Global Illumination: \[GPUPLM\] Crash in RadeonRaysMeshManager::RemoveGeometry while baking Terrain game object with 4k lightmaps on certain GPU ([1255993](https://issuetracker.unity3d.com/issues/global-illumination-editor-crashes-while-baking-terrain-game-object-using-progressive-gpu-lightmapper))
    
*   Terrain: Terrain Lit Opacity as Density option causes alpha'd areas on the 5th layer or greater to appear with artifacts ([1283124](https://issuetracker.unity3d.com/issues/terrain-lit-opacity-as-density-option-causes-alphad-areas-on-the-5th-layer-or-greater-to-appear-with-artifacts))
    
*   MacOS: Resigning Unity built macOS app results in "code signature data out of place" out of place error ([1324168](https://issuetracker.unity3d.com/issues/resigning-unity-built-macos-app-results-in-code-signature-data-out-of-place-out-of-place-error))
    
*   XR: OpenXR + URP + UWP rendering stuck ([1323833](https://issuetracker.unity3d.com/issues/openxr-plus-urp-plus-uwp-rendering-stuck))
    
*   MacOS: \[macOS\] "build is damaged and cannot be opened" error when downloading Unity build from internet ([1323501](https://issuetracker.unity3d.com/issues/macos-build-is-damaged-and-cannot-be-opened-error-when-downloading-unity-build-from-internet))
    
*   Mobile: FixedUpdate gets called multiple times before the first Update when Build is run on a Device ([1318647](https://issuetracker.unity3d.com/issues/mobile-fixedupdate-gets-called-multiple-times-before-the-first-update-when-build-is-run-on-a-device))
    
*   Packman: Package Manager incorrectly shows that there are no packages in a new project ([1319205](https://issuetracker.unity3d.com/issues/package-manager-falsely-shows-that-there-are-no-packages-in-a-new-project))
    
*   Scripting: Crashes on mono\_class\_init when entering Play Mode after recompiling scripts ([1262671](https://issuetracker.unity3d.com/issues/crashes-on-mono-class-init-when-entering-play-mode-after-recompiling-scripts))
    
*   Asset Importers: Wintermute::Geometry::Verify errors are spammed when baking a Mesh with Mesh Compression set to Medium/High ([1313968](https://issuetracker.unity3d.com/issues/wintermute-geometry-verify-errors-are-spammed-when-baking-a-mesh-with-mesh-compression-set-to-medium-slash-high))
    
*   2D: \[URP\] The Camera renders black screen when Post Processing is enabled in the 2D Renderer and in the Camera Component ([1318500](https://issuetracker.unity3d.com/issues/urp-the-camera-renders-black-screen-when-post-processing-is-enabled-in-the-2d-renderer-and-in-the-camera-component))
    
*   Polybrush: \[PolyBrush\] Something went wrong saving brush settings Warning is thrown when Saving a Brush after opening the PolyBrush Window ([1315475](https://issuetracker.unity3d.com/issues/polybrush-something-went-wrong-saving-brush-settings-warning-is-thrown-when-saving-a-brush-after-opening-the-polybrush-window))