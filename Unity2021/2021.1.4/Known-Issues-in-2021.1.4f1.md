# Unity 2021.1.4

https://unity3d.com/unity/whats-new/2021.1.4

## Known Issues in 2021.1.4f1



*   Asset Import Pipeline: Prefab script field reference is lost when project is upgraded ([1328724](https://issuetracker.unity3d.com/issues/prefab-script-field-reference-is-lost-when-project-is-upgraded))
    
*   Animation: AnimationEvent is fired late or isn't fired at all when Animation's 'Motion Time' value is set manually ([1324763](https://issuetracker.unity3d.com/issues/animationevent-is-fired-late-or-isnt-fired-at-all-when-animations-motion-time-value-is-set-manually))
    
*   Global Illumination: Performance regression when baking light probes with a light cookie in the scene ([1323393](https://issuetracker.unity3d.com/issues/performance-regression-when-baking-light-probes-with-a-light-cookie-in-the-scene))
    
*   Asset Bundles: \[macOS\] Editor crashes when trying to build Asset bundles in InitializeOnLoad or InitializeOnLoadMethod time ([1328463](https://issuetracker.unity3d.com/issues/macos-editor-crashes-when-trying-to-build-asset-bundles-in-initializeonload-or-initializeonloadmethod-time))
    
*   Scene/Game View: \[Game view\] Game stops accepting input when the Game view undocked and re-docked during Play Mode using the Input System ([1320678](https://issuetracker.unity3d.com/issues/game-stops-accepting-input-when-the-game-view-undocked-and-re-docked-during-play-mode-using-the-input-system))
    
*   Settings Window: Editor freezes when FixedTimestep value in the Preferences is set to 0/0 ([1326481](https://issuetracker.unity3d.com/issues/editor-freezes-when-fixedtimestep-value-in-the-preferences-is-set-to-0-slash-0))
    
*   2D: \[Skinning Editor\] Vertex can't be created after modifying Vertexes weight and when Sprite is from the .psb file ([1322204](https://issuetracker.unity3d.com/issues/skinning-editor-vertex-cant-be-created-after-modifying-vertexes-weight-and-when-sprite-is-from-the-psb-file))
    
*   AI: Crash with ComputeTileMeshJob when generating Navmesh ([1329346](https://issuetracker.unity3d.com/issues/crash-with-computetilemeshjob-when-generating-navmesh))
    
*   Global Illumination: Reflection probes don't contain indirect scene lighting after the on-demand GI bake from the Lighting window ([1324246](https://issuetracker.unity3d.com/issues/reflection-probes-doesnt-contain-indirect-scene-lighting-after-the-on-demand-gi-bake-from-the-lighting-window))
    
*   Animation: \[Performance Regression\] AnimationWindowState:get\_allCurves takes approximately 5000ms to load animation in the Animation window ([1320250](https://issuetracker.unity3d.com/issues/perfomance-regression-animationwindowstate-get-allcurves-takes-approximately-5000ms-to-load-animation-in-the-animation-window))
    
*   IL2CPP: Build fails when using a combination of messages, SyncVars and SyncList in a project ([1328966](https://issuetracker.unity3d.com/issues/il2cpp-build-fails-when-using-a-combination-of-messages-syncvars-and-synclist-in-a-project))
    
*   Metal: Performance in Game View is significantly impacted by Gfx.WaitForPresentOnGfxThread when a second monitor is connected ([1327408](https://issuetracker.unity3d.com/issues/performance-in-game-view-is-significantly-impacted-by-gfx-dot-waitforpresentongfxthread-when-a-second-monitor-is-connected))
    
*   Terrain: All the textures are cleared when creating Texture array ([1323870](https://issuetracker.unity3d.com/issues/all-the-textures-are-cleared-when-creating-texture-array))
    
*   HD RP: The camera doesn't rotate in HDRP Template with the SimpleCameraController.cs script ([1326816](https://issuetracker.unity3d.com/issues/the-camera-doesnt-rotate-in-hdrp-template-with-the-simplecameracontroller-dot-cs-script))
    
*   Scene Management: Crash on BuildPrefabInstanceCorrespondingObjectMap when overriding nested prefab inside AssetDatabase.StartAssetEditing() block ([1324978](https://issuetracker.unity3d.com/issues/crash-on-buildprefabinstancecorrespondingobjectmap-when-overriding-nested-prefab-inside-assetdatabase-dot-startassetediting-block))
    
*   WebGL: "SharedArrayBuffer will require cross-origin isolation as of M91" warning is thrown when launching Player on Chrome ([1323832](https://issuetracker.unity3d.com/issues/webgl-sharedarraybuffer-will-require-cross-origin-isolation-as-of-m91-warning-is-thrown-when-launching-player-on-chrome))
    
*   Linux: Linux Editor crashes at "\_XFreeX11XCBStructure" when loading tutorials ([1323204](https://issuetracker.unity3d.com/issues/linux-editor-crashes-at-xfreex11xcbstructure-when-loading-tutorials))
    
*   Terrain: Crash on TreeRenderer::WillRenderTrees when being in Play Mode for several seconds ([1317966](https://issuetracker.unity3d.com/issues/crash-on-treerenderer-willrendertrees-when-being-in-play-mode-for-several-seconds))
    
*   IMGUI: Contents of a ModalUtility window are invisible when it is launched from a Unity Context Menu ([1313636](https://issuetracker.unity3d.com/issues/error-displaying-showmodalutility-window))
    
*   Packman: User can't easily configure location of both UPM and Asset Store package local cache ([1317232](https://issuetracker.unity3d.com/issues/user-cant-easily-configure-location-of-both-upm-and-asset-store-package-local-cache))
    
*   Serialization: Crash in SerializedProperty::IsValid when reordering a SerializedProperty list ([1320319](https://issuetracker.unity3d.com/issues/crash-in-serializedproperty-isvalid-when-reordering-a-serializedproperty-list))
    
*   Global Illumination: \[GPUPLM\] Crash in RadeonRaysMeshManager::RemoveGeometry while baking Terrain game object with 4k lightmaps on certain GPU ([1255993](https://issuetracker.unity3d.com/issues/global-illumination-editor-crashes-while-baking-terrain-game-object-using-progressive-gpu-lightmapper))
    
*   Terrain: Terrain Lit Opacity as Density option causes alpha'd areas on the 5th layer or greater to appear with artifacts ([1283124](https://issuetracker.unity3d.com/issues/terrain-lit-opacity-as-density-option-causes-alphad-areas-on-the-5th-layer-or-greater-to-appear-with-artifacts))
    
*   Packman: Package resolution error when using a Git dependency referencing an annotated tag in its Git URL ([1325920](https://issuetracker.unity3d.com/issues/package-resolution-error-when-using-a-git-dependency-referencing-an-annotated-tag-in-its-git-url))
    
*   Scripting: Increased Script Assembly reload time ([1323490](https://issuetracker.unity3d.com/issues/increased-reload-time))
    
*   Scripting: Crashes on mono\_class\_init when entering Play Mode after recompiling scripts ([1262671](https://issuetracker.unity3d.com/issues/crashes-on-mono-class-init-when-entering-play-mode-after-recompiling-scripts))
    
*   Global Illumination: Wintermute::Geometry::Verify errors are spammed when baking a Mesh with Mesh Compression set to Medium/High ([1319133](https://issuetracker.unity3d.com/issues/speedtree-asset-breaks-when-trying-to-lightmap))
    
*   MacOS: \[macOS\] "build is damaged and cannot be opened" error when downloading Unity build from internet ([1323501](https://issuetracker.unity3d.com/issues/macos-build-is-damaged-and-cannot-be-opened-error-when-downloading-unity-build-from-internet))
    
*   Asset Importers: Wintermute::Geometry::Verify errors are spammed when baking a Mesh with Mesh Compression set to Medium/High ([1313968](https://issuetracker.unity3d.com/issues/wintermute-geometry-verify-errors-are-spammed-when-baking-a-mesh-with-mesh-compression-set-to-medium-slash-high))
    
*   2D: \[URP\] The Camera renders black screen when Post Processing is enabled in the 2D Renderer and in the Camera Component ([1318500](https://issuetracker.unity3d.com/issues/urp-the-camera-renders-black-screen-when-post-processing-is-enabled-in-the-2d-renderer-and-in-the-camera-component))