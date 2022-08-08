# Unity 2021.1.3

https://unity3d.com/unity/whats-new/2021.1.3

## Known Issues in 2021.1.3f1



*   Metal: Performance in Game View is significantly impacted by Gfx.WaitForPresentOnGfxThread when a second monitor is connected ([1327408](https://issuetracker.unity3d.com/issues/performance-in-game-view-is-significantly-impacted-by-gfx-dot-waitforpresentongfxthread-when-a-second-monitor-is-connected))
    
*   Terrain: All the textures are cleared when creating Texture array ([1323870](https://issuetracker.unity3d.com/issues/all-the-textures-are-cleared-when-creating-texture-array))
    
*   Animation: \[Perfomance Regression\] AnimationWindowState:get\_allCurves takes approximately 5000ms to load animation in the Animation window ([1320250](https://issuetracker.unity3d.com/issues/perfomance-regression-animationwindowstate-get-allcurves-takes-approximately-5000ms-to-load-animation-in-the-animation-window))
    
*   HD RP: The camera doesn't rotate in HDRP Template with the SimpleCameraController.cs script ([1326816](https://issuetracker.unity3d.com/issues/the-camera-doesnt-rotate-in-hdrp-template-with-the-simplecameracontroller-dot-cs-script))
    
*   Scene Management: Crash on BuildPrefabInstanceCorrespondingObjectMap when overriding nested prefab inside AssetDatabase.StartAssetEditing() block ([1324978](https://issuetracker.unity3d.com/issues/crash-on-buildprefabinstancecorrespondingobjectmap-when-overriding-nested-prefab-inside-assetdatabase-dot-startassetediting-block))
    
*   WebGL: "SharedArrayBuffer will require cross-origin isolation as of M91" warning is thrown when launching Player on Chrome ([1323832](https://issuetracker.unity3d.com/issues/webgl-sharedarraybuffer-will-require-cross-origin-isolation-as-of-m91-warning-is-thrown-when-launching-player-on-chrome))
    
*   2D: \[Skinning Editor\] Vertex can't be created after modifying Vertexes weight and when Sprite is from the .psb file ([1322204](https://issuetracker.unity3d.com/issues/skinning-editor-vertex-cant-be-created-after-modifying-vertexes-weight-and-when-sprite-is-from-the-psb-file))
    
*   Scripting: Increased Script Assembly reload time ([1323490](https://issuetracker.unity3d.com/issues/increased-reload-time))
    
*   Linux: Linux Editor crashes at "\_XFreeX11XCBStructure" when loading tutorials ([1323204](https://issuetracker.unity3d.com/issues/linux-editor-crashes-at-xfreex11xcbstructure-when-loading-tutorials))
    
*   Terrain: Crash on TreeRenderer::WillRenderTrees when being in Play Mode for several seconds ([1317966](https://issuetracker.unity3d.com/issues/crash-on-treerenderer-willrendertrees-when-being-in-play-mode-for-several-seconds))
    
*   IMGUI: Contents of a ModalUtility window are invisible when it is launched from a Unity Context Menu ([1313636](https://issuetracker.unity3d.com/issues/error-displaying-showmodalutility-window))
    
*   Global Illumination: Reflection probes doesn't contain indirect scene lighting after the on-demand GI bake from the Lighting window ([1324246](https://issuetracker.unity3d.com/issues/reflection-probes-doesnt-contain-indirect-scene-lighting-after-the-on-demand-gi-bake-from-the-lighting-window))
    
*   Packman: User can't easily configure location of both UPM and Asset Store package local cache ([1317232](https://issuetracker.unity3d.com/issues/user-cant-easily-configure-location-of-both-upm-and-asset-store-package-local-cache))
    
*   Serialization: Crash in SerializedProperty::IsValid when reordering a SerializedProperty list ([1320319](https://issuetracker.unity3d.com/issues/crash-in-serializedproperty-isvalid-when-reordering-a-serializedproperty-list))
    
*   Global Illumination: \[GPUPLM\] Crash in RadeonRaysMeshManager::RemoveGeometry while baking Terrain game object with 4k lightmaps on certain GPU ([1255993](https://issuetracker.unity3d.com/issues/global-illumination-editor-crashes-while-baking-terrain-game-object-using-progressive-gpu-lightmapper))
    
*   Terrain: Terrain Lit Opacity as Density option causes alpha'd areas on the 5th layer or greater to appear with artifacts ([1283124](https://issuetracker.unity3d.com/issues/terrain-lit-opacity-as-density-option-causes-alphad-areas-on-the-5th-layer-or-greater-to-appear-with-artifacts))
    
*   Asset Bundles: Synchronous Asset Loading Does Not Correctly Load Preload Dependencies ([1321141](https://issuetracker.unity3d.com/issues/synchronous-asset-loading-does-not-correctly-load-preload-dependencies))
    
*   Addressable Assets: Performance bug in PreloadManager::WaitForAllOperationToComplete ([1322086](https://issuetracker.unity3d.com/issues/performance-bug-reported-by-the-dots-team-in-preloadmanager-waitforalloperationtocomplete))
    
*   Packman: Package Manager incorrectly shows that there are no packages in a new project ([1319205](https://issuetracker.unity3d.com/issues/package-manager-falsely-shows-that-there-are-no-packages-in-a-new-project))
    
*   Windows: \[Windows 7\] "WindowsVideoMedia error 0xc00d36b4" error is thrown when loading a video with the VideoPlayer ([1306350](https://issuetracker.unity3d.com/issues/windows-7-windowsvideomedia-error-0xc00d36b4-error-is-thrown-when-loading-a-video-with-the-videoplayer))
    
*   Scripting: Crashes on mono\_class\_init when entering Play Mode after recompiling scripts ([1262671](https://issuetracker.unity3d.com/issues/crashes-on-mono-class-init-when-entering-play-mode-after-recompiling-scripts))
    
*   Global Illumination: Wintermute::Geometry::Verify errors are spammed when baking a Mesh with Mesh Compression set to Medium/High ([1319133](https://issuetracker.unity3d.com/issues/speedtree-asset-breaks-when-trying-to-lightmap))
    
*   Cloth: Cloth is broken when parent GameObject scale is lower than 1 and Surface Penetration constraints are set 0 ([1319488](https://issuetracker.unity3d.com/issues/cloth-is-broken-when-parent-gameobject-scale-is-lower-than-1-and-surface-penetration-constraints-are-set-0))
    
*   MacOS: \[macOS\] "build is damaged and cannot be opened" error when downloading Unity build from internet ([1323501](https://issuetracker.unity3d.com/issues/macos-build-is-damaged-and-cannot-be-opened-error-when-downloading-unity-build-from-internet))
    
*   Asset Importers: Wintermute::Geometry::Verify errors are spammed when baking a Mesh with Mesh Compression set to Medium/High ([1313968](https://issuetracker.unity3d.com/issues/wintermute-geometry-verify-errors-are-spammed-when-baking-a-mesh-with-mesh-compression-set-to-medium-slash-high))
    
*   2D: \[URP\] The Camera renders black screen when Post Processing is enabled in the 2D Renderer and in the Camera Component ([1318500](https://issuetracker.unity3d.com/issues/urp-the-camera-renders-black-screen-when-post-processing-is-enabled-in-the-2d-renderer-and-in-the-camera-component))