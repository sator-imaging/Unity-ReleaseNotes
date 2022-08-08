# Unity 2020.3.8

https://unity3d.com/unity/whats-new/2020.3.8

## Known Issues in 2020.3.8f1



*   Mobile: \[Android\] App stops due to OnPixelCopyFinishedListener not being supported on devices with lower than 24 SDK ([1331290](https://issuetracker.unity3d.com/issues/app-stops-due-to-onpixelcopyfinishedlistener-not-being-supported-on-devices-with-lower-than-24-sdk))
    
*   OpenGL: SRP Batcher not working with OpenGL APIs when the project is built ([1331098](https://issuetracker.unity3d.com/issues/srp-batcher-not-working-with-opengl-apis-when-the-project-is-built))
    
*   Mobile: \[Android\] Build fails when there are 680 or more files in the Streaming Assets folder ([1272592](https://issuetracker.unity3d.com/issues/android-build-fails-when-there-are-680-or-more-files-in-the-streaming-assets-folder))
    
*   MacOS: \[macOS\] Unity crashes when exception thrown after a DLL has been loaded ([1318755](https://issuetracker.unity3d.com/issues/macos-unity-crashes-when-exception-thrown-after-a-dll-has-been-loaded))
    
*   Linux: InputSystem's Mouse delta values do not change when the Cursor lockState is set to Locked ([1248389](https://issuetracker.unity3d.com/issues/linux-inputsystems-mouse-delta-values-do-not-change-when-the-cursor-lockstate-is-set-to-locked))
    
*   Global Illumination: Reflection probes don't contain indirect scene lighting after the on-demand GI bake from the Lighting window ([1324246](https://issuetracker.unity3d.com/issues/reflection-probes-doesnt-contain-indirect-scene-lighting-after-the-on-demand-gi-bake-from-the-lighting-window))
    
*   Linux: Linux Editor crashes at "\_XFreeX11XCBStructure" when loading tutorials ([1323204](https://issuetracker.unity3d.com/issues/linux-editor-crashes-at-xfreex11xcbstructure-when-loading-tutorials))
    
*   Metal: Performance in Game View is significantly impacted by Gfx.WaitForPresentOnGfxThread when a second monitor is connected ([1327408](https://issuetracker.unity3d.com/issues/performance-in-game-view-is-significantly-impacted-by-gfx-dot-waitforpresentongfxthread-when-a-second-monitor-is-connected))
    
*   Asset Import Pipeline: Prefabs are reimporting every time a code change is made ([1294785](https://issuetracker.unity3d.com/issues/prefabs-are-reimporting-every-time-a-code-change-is-made))
    
*   DirectX12: Editor crashes on GfxDeviceD3D12Base::DrawBuffersCommon when switching between Scenes ([1329083](https://issuetracker.unity3d.com/issues/editor-crashes-on-gfxdeviced3d12base-drawbufferscommon-when-switching-between-scenes))
    
*   Mono: Crash starting Unity when using NordVPN ([1308797](https://issuetracker.unity3d.com/issues/crash-on-system-dot-net-dot-sockets-dot-socket-queueioselectorjob-when-using-a-vpn-and-opening-a-project-that-uses-visual-studio))
    
*   AI: Crash with ComputeTileMeshJob when generating Navmesh ([1329346](https://issuetracker.unity3d.com/issues/crash-with-computetilemeshjob-when-generating-navmesh))
    
*   Animation: \[Performance Regression\] AnimationWindowState:get\_allCurves takes approximately 5000ms to load animation in the Animation window ([1320250](https://issuetracker.unity3d.com/issues/perfomance-regression-animationwindowstate-get-allcurves-takes-approximately-5000ms-to-load-animation-in-the-animation-window))
    
*   IL2CPP: Build fails when using a combination of messages, SyncVars and SyncList in a project ([1328966](https://issuetracker.unity3d.com/issues/il2cpp-build-fails-when-using-a-combination-of-messages-syncvars-and-synclist-in-a-project))
    
*   Scene Management: Crash on BuildPrefabInstanceCorrespondingObjectMap when overriding nested prefab inside AssetDatabase.StartAssetEditing() block ([1324978](https://issuetracker.unity3d.com/issues/crash-on-buildprefabinstancecorrespondingobjectmap-when-overriding-nested-prefab-inside-assetdatabase-dot-startassetediting-block))
    
*   Terrain: Crash on TreeRenderer::WillRenderTrees when being in Play Mode for several seconds ([1317966](https://issuetracker.unity3d.com/issues/crash-on-treerenderer-willrendertrees-when-being-in-play-mode-for-several-seconds))
    
*   Packman: User can't easily configure location of both UPM and Asset Store package local cache ([1317232](https://issuetracker.unity3d.com/issues/user-cant-easily-configure-location-of-both-upm-and-asset-store-package-local-cache))
    
*   Templates: Editor Crashes when performing Undo and Redo after duplicating Game Object with LEGO Model Asset component ([1298503](https://issuetracker.unity3d.com/issues/crash-when-redoing-and-undoing-pasting-prefabs-in-scene-in-lego-microgame))
    
*   IMGUI: Contents of a ModalUtility window are invisible when it is launched from a Unity Context Menu ([1313636](https://issuetracker.unity3d.com/issues/error-displaying-showmodalutility-window))
    
*   Asset Importers: \[Performance Regression\] Importing an fbx model is noticeably slower when the model contains Animations ([1265275](https://issuetracker.unity3d.com/issues/performance-regression-importing-an-fbx-model-is-noticeably-slower-when-the-model-contains-animations))
    
*   Physics: OnTriggerEnter gets called after reparenting a RigidBody ([1323883](https://issuetracker.unity3d.com/issues/onentertrigger-gets-called-after-reparenting-a-rigidbody))
    
*   Terrain: All the textures are cleared when creating Texture array ([1323870](https://issuetracker.unity3d.com/issues/all-the-textures-are-cleared-when-creating-texture-array))
    
*   Packman: Package resolution error when using a Git dependency referencing an annotated tag in its Git URL ([1325920](https://issuetracker.unity3d.com/issues/package-resolution-error-when-using-a-git-dependency-referencing-an-annotated-tag-in-its-git-url))
    
*   Animation: AnimationEvent is fired late or isn't fired at all when Animation's 'Motion Time' value is set manually ([1324763](https://issuetracker.unity3d.com/issues/animationevent-is-fired-late-or-isnt-fired-at-all-when-animations-motion-time-value-is-set-manually))
    
*   Asset Import Pipeline: Prefab script field reference is lost when project is upgraded ([1328724](https://issuetracker.unity3d.com/issues/prefab-script-field-reference-is-lost-when-project-is-upgraded))
    
*   HD RP: The camera doesn't rotate in HDRP Template with the SimpleCameraController.cs script ([1326816](https://issuetracker.unity3d.com/issues/the-camera-doesnt-rotate-in-hdrp-template-with-the-simplecameracontroller-dot-cs-script))
    
*   Packman: PackageManager.Client.SearchAll(offlineMode: true) returns an error if user offline ([1319585](https://issuetracker.unity3d.com/issues/packagemanager-dot-client-dot-searchall-offlinemode-true-returns-an-error-if-user-offline))
    
*   2D: \[Skinning Editor\] Vertex can't be created after modifying Vertexes weight and when Sprite is from the .psb file ([1322204](https://issuetracker.unity3d.com/issues/skinning-editor-vertex-cant-be-created-after-modifying-vertexes-weight-and-when-sprite-is-from-the-psb-file))
    
*   Scripting: Increased Script Assembly reload time ([1323490](https://issuetracker.unity3d.com/issues/increased-reload-time))
    
*   Scripting: Crashes on mono\_class\_init when entering Play Mode after recompiling scripts ([1262671](https://issuetracker.unity3d.com/issues/crashes-on-mono-class-init-when-entering-play-mode-after-recompiling-scripts))
    
*   MacOS: \[macOS\] "build is damaged and cannot be opened" error when downloading Unity build from internet ([1323501](https://issuetracker.unity3d.com/issues/macos-build-is-damaged-and-cannot-be-opened-error-when-downloading-unity-build-from-internet))
    
*   Asset Importers: Wintermute::Geometry::Verify errors are spammed when baking a Mesh with Mesh Compression set to Medium/High ([1313968](https://issuetracker.unity3d.com/issues/wintermute-geometry-verify-errors-are-spammed-when-baking-a-mesh-with-mesh-compression-set-to-medium-slash-high))
    
*   Polybrush: \[PolyBrush\] Something went wrong saving brush settings Warning is thrown when Saving a Brush after opening the PolyBrush Window ([1315475](https://issuetracker.unity3d.com/issues/polybrush-something-went-wrong-saving-brush-settings-warning-is-thrown-when-saving-a-brush-after-opening-the-polybrush-window))
    
*   Templates: \[Linux\] Missing libdl.so library causes crash when entering Playmode for the second time or closing the Editor ([1237642](https://issuetracker.unity3d.com/issues/missing-libdl-dot-so-library-causes-crash-when-entering-playmode-for-the-second-time-or-closing-the-editor))