# Unity 2020.3.2

https://unity3d.com/unity/whats-new/2020.3.2

## Known Issues in 2020.3.2f1



*   Linux: Linux Editor crashes at "\_XFreeX11XCBStructure" when loading tutorials ([1323204](https://issuetracker.unity3d.com/issues/linux-editor-crashes-at-xfreex11xcbstructure-when-loading-tutorials))
    
*   Scripting: Increased Script Assembly reload time ([1323490](https://issuetracker.unity3d.com/issues/increased-reload-time))
    
*   MacOS: Resigning Unity built macOS app results in "code signature data out of place" out of place error ([1324168](https://issuetracker.unity3d.com/issues/resigning-unity-built-macos-app-results-in-code-signature-data-out-of-place-out-of-place-error))
    
*   Terrain: Crash on TreeRenderer::WillRenderTrees when being in Play Mode for several seconds ([1317966](https://issuetracker.unity3d.com/issues/crash-on-treerenderer-willrendertrees-when-being-in-play-mode-for-several-seconds))
    
*   IMGUI: Contents of a ModalUtility window are invisible when it is launched from a Unity Context Menu ([1313636](https://issuetracker.unity3d.com/issues/error-displaying-showmodalutility-window))
    
*   Global Illumination: Wintermute::Geometry::Verify errors are spammed when baking a Mesh with Mesh Compression set to Medium/High ([1319133](https://issuetracker.unity3d.com/issues/speedtree-asset-breaks-when-trying-to-lightmap))
    
*   Global Illumination: Reflection probes doesn't contain indirect scene lighting after the on-demand GI bake from the Lighting window ([1324246](https://issuetracker.unity3d.com/issues/reflection-probes-doesnt-contain-indirect-scene-lighting-after-the-on-demand-gi-bake-from-the-lighting-window))
    
*   Addressable Assets: Performance bug reported by the DOTS team in PreloadManager::WaitForAllOperationToComplete ([1322086](https://issuetracker.unity3d.com/issues/performance-bug-reported-by-the-dots-team-in-preloadmanager-waitforalloperationtocomplete))
    
*   Asset Bundles: Synchronous Asset Loading Does Not Correctly Load Preload Dependencies ([1321141](https://issuetracker.unity3d.com/issues/synchronous-asset-loading-does-not-correctly-load-preload-dependencies))
    
*   Packman: User can't easily configure location of both UPM and Asset Store package local cache ([1317232](https://issuetracker.unity3d.com/issues/user-cant-easily-configure-location-of-both-upm-and-asset-store-package-local-cache))
    
*   Cloth: Cloth is broken when parent GameObject scale is lower than 1 and Surface Penetration constraints are set 0 ([1319488](https://issuetracker.unity3d.com/issues/cloth-is-broken-when-parent-gameobject-scale-is-lower-than-1-and-surface-penetration-constraints-are-set-0))
    
*   Windows: \[Windows 7\] "WindowsVideoMedia error 0xc00d36b4" error is thrown when loading a video with the VideoPlayer ([1306350](https://issuetracker.unity3d.com/issues/windows-7-windowsvideomedia-error-0xc00d36b4-error-is-thrown-when-loading-a-video-with-the-videoplayer))
    
*   Templates: Editor Crashes when performing Undo and Redo after duplicating Game Object with LEGO Model Asset component ([1298503](https://issuetracker.unity3d.com/issues/crash-when-redoing-and-undoing-pasting-prefabs-in-scene-in-lego-microgame))
    
*   Asset Importers: \[Performance Regression\] Importing an fbx model is noticeably slower when the model contains Animations ([1265275](https://issuetracker.unity3d.com/issues/performance-regression-importing-an-fbx-model-is-noticeably-slower-when-the-model-contains-animations))
    
*   Linux: InputSystem's Mouse delta values do not change when the Cursor lockState is set to Locked ([1248389](https://issuetracker.unity3d.com/issues/linux-inputsystems-mouse-delta-values-do-not-change-when-the-cursor-lockstate-is-set-to-locked))
    
*   Mobile: FixedUpdate gets called multiple times before the first Update when Build is run on a Device ([1318647](https://issuetracker.unity3d.com/issues/mobile-fixedupdate-gets-called-multiple-times-before-the-first-update-when-build-is-run-on-a-device))
    
*   XR: OpenXR + URP + UWP rendering stuck ([1323833](https://issuetracker.unity3d.com/issues/openxr-plus-urp-plus-uwp-rendering-stuck))
    
*   MacOS: \[macOS\] "build is damaged and cannot be opened" error when downloading Unity build from internet ([1323501](https://issuetracker.unity3d.com/issues/macos-build-is-damaged-and-cannot-be-opened-error-when-downloading-unity-build-from-internet))
    
*   Shuriken: Crash on ParticleSystem\_ShapeModule\_CUSTOM\_set\_sprite\_Injected when changing the shape.sprite of a null ParticleSystem ([1319658](https://issuetracker.unity3d.com/issues/crash-on-particlesystem-shapemodule-custom-set-sprite-injected-when-changing-the-shape-dot-sprite-of-a-null-particlesystem))
    
*   Linux: Linux Editor throws "X Server took longer than x miliseconds to respond to SetGtkWindowSizeAndPosition" error after opening ([1309607](https://issuetracker.unity3d.com/issues/linux-editor-throws-x-server-took-longer-than-x-miliseconds-to-respond-to-setgtkwindowsizeandposition-error-after-opening))
    
*   Android: App installed using APK from app bundle option in Android Studio fails to run ([1314472](https://issuetracker.unity3d.com/issues/android-app-installed-using-apk-from-app-bundle-option-in-android-studio-fails-to-run))
    
*   Shader System: Editor crashes on UpgradeOldShaderSyntax when shaders are being upgraded during importing process ([1299790](https://issuetracker.unity3d.com/issues/editor-crashes-on-upgradeoldshadersyntax-when-shaders-are-being-upgraded-during-importing-process))
    
*   Mono: Built player takes multiple seconds to shut down ([1295072](https://issuetracker.unity3d.com/issues/built-player-takes-multiple-seconds-to-shut-down))
    
*   Scripting: Crashes on mono\_class\_init when entering Play Mode after recompiling scripts ([1262671](https://issuetracker.unity3d.com/issues/crashes-on-mono-class-init-when-entering-play-mode-after-recompiling-scripts))
    
*   Asset Importers: Wintermute::Geometry::Verify errors are spammed when baking a Mesh with Mesh Compression set to Medium/High ([1313968](https://issuetracker.unity3d.com/issues/wintermute-geometry-verify-errors-are-spammed-when-baking-a-mesh-with-mesh-compression-set-to-medium-slash-high))
    
*   Polybrush: \[PolyBrush\] Something went wrong saving brush settings Warning is thrown when Saving a Brush after opening the PolyBrush Window ([1315475](https://issuetracker.unity3d.com/issues/polybrush-something-went-wrong-saving-brush-settings-warning-is-thrown-when-saving-a-brush-after-opening-the-polybrush-window))
    
*   Templates: \[Linux\] Missing libdl.so library causes crash when entering Playmode for the second time or closing the Editor ([1237642](https://issuetracker.unity3d.com/issues/missing-libdl-dot-so-library-causes-crash-when-entering-playmode-for-the-second-time-or-closing-the-editor))