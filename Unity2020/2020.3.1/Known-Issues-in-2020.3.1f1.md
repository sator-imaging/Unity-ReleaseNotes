# Unity 2020.3.1

https://unity3d.com/unity/whats-new/2020.3.1

## Known Issues in 2020.3.1f1



*   Addressable Assets: Performance bug reported by the DOTS team in PreloadManager::WaitForAllOperationToComplete ([1322086](https://issuetracker.unity3d.com/issues/performance-bug-reported-by-the-dots-team-in-preloadmanager-waitforalloperationtocomplete))
    
*   Asset Bundles: Synchronous Asset Loading Does Not Correctly Load Preload Dependencies ([1321141](https://issuetracker.unity3d.com/issues/synchronous-asset-loading-does-not-correctly-load-preload-dependencies))
    
*   Packman: User can't easily configure location of both UPM and Asset Store package local cache ([1317232](https://issuetracker.unity3d.com/issues/user-cant-easily-configure-location-of-both-upm-and-asset-store-package-local-cache))
    
*   Cloth: Cloth is broken when parent GameObject scale is lower than 1 and Surface Penetration constraints are set 0 ([1319488](https://issuetracker.unity3d.com/issues/cloth-is-broken-when-parent-gameobject-scale-is-lower-than-1-and-surface-penetration-constraints-are-set-0))
    
*   Templates: Editor Crashes when performing Undo and Redo after duplicating Game Object with LEGO Model Asset component ([1298503](https://issuetracker.unity3d.com/issues/crash-when-redoing-and-undoing-pasting-prefabs-in-scene-in-lego-microgame))
    
*   Linux: InputSystem's Mouse delta values do not change when the Cursor lockState is set to Locked ([1248389](https://issuetracker.unity3d.com/issues/linux-inputsystems-mouse-delta-values-do-not-change-when-the-cursor-lockstate-is-set-to-locked))
    
*   Asset Importers: \[Performance Regression\] Importing an fbx model is noticeably slower when the model contains Animations ([1265275](https://issuetracker.unity3d.com/issues/performance-regression-importing-an-fbx-model-is-noticeably-slower-when-the-model-contains-animations))
    
*   Shader System: Editor crashes on UpgradeOldShaderSyntax when shaders are being upgraded during importing process ([1299790](https://issuetracker.unity3d.com/issues/editor-crashes-on-upgradeoldshadersyntax-when-shaders-are-being-upgraded-during-importing-process))
    
*   Mono: Built player takes multiple seconds to shut down ([1295072](https://issuetracker.unity3d.com/issues/built-player-takes-multiple-seconds-to-shut-down))
    
*   Scripting: Crashes on mono\_class\_init when entering Play Mode after recompiling scripts ([1262671](https://issuetracker.unity3d.com/issues/crashes-on-mono-class-init-when-entering-play-mode-after-recompiling-scripts))
    
*   Android: App installed using APK from app bundle option in Android Studio fails to run ([1314472](https://issuetracker.unity3d.com/issues/android-app-installed-using-apk-from-app-bundle-option-in-android-studio-fails-to-run))
    
*   Mobile: FixedUpdate gets called multiple times before the first Update when Build is run on a Device ([1318647](https://issuetracker.unity3d.com/issues/mobile-fixedupdate-gets-called-multiple-times-before-the-first-update-when-build-is-run-on-a-device))
    
*   Asset Importers: Wintermute::Geometry::Verify errors are spammed when baking a Mesh with Mesh Compression set to Medium/High ([1313968](https://issuetracker.unity3d.com/issues/wintermute-geometry-verify-errors-are-spammed-when-baking-a-mesh-with-mesh-compression-set-to-medium-slash-high))
    
*   Linux: Linux Editor throws "X Server took longer than x miliseconds to respond to SetGtkWindowSizeAndPosition" error after opening ([1309607](https://issuetracker.unity3d.com/issues/linux-editor-throws-x-server-took-longer-than-x-miliseconds-to-respond-to-setgtkwindowsizeandposition-error-after-opening))
    
*   Shuriken: Crash on ParticleSystem::EndUpdateAll ([1311212](https://issuetracker.unity3d.com/issues/shuriken-crash-on-particlesystem-endupdateall))
    
*   Shuriken: Crash on ParticleSystem\_ShapeModule\_CUSTOM\_set\_sprite\_Injected when changing the shape.sprite of a null ParticleSystem ([1319658](https://issuetracker.unity3d.com/issues/crash-on-particlesystem-shapemodule-custom-set-sprite-injected-when-changing-the-shape-dot-sprite-of-a-null-particlesystem))
    
*   Mobile: Calling Resources.Load() while asynchronously loading assetbundle by UnityWebRequest makes main thread stuck ([1277297](https://issuetracker.unity3d.com/issues/ios-android-calling-resources-dot-load-while-asynchronously-loading-assetbundle-by-unitywebrequest-makes-main-thread-stuck))
    
*   Shader System: Crash on PAL\_LocalIPC\_IsConnected when IPC fails on launch ([1319336](https://issuetracker.unity3d.com/issues/crash-on-pal-localipc-isconnected-when-ipc-fails-on-launch))
    
*   Shader System: \[URP Template\] Major performance drop in the Editor during Play Mode ([1277222](https://issuetracker.unity3d.com/issues/urp-template-major-performance-drop-in-the-editor-during-play-mode))
    
*   Packman: Package Manager's prompt keeps reappearing to resolve packages ([1315014](https://issuetracker.unity3d.com/issues/package-managers-prompt-keeps-reappearing-to-resolve-packages))
    
*   Mobile: Screen.dpi returns 0 on iPad Pro for projects built from 2019.4.16f1 ([1300359](https://issuetracker.unity3d.com/issues/screen-dot-dpi-returns-0-on-ipad-pro-for-projects-built-from-2019-dot-4-16f1))
    
*   Cloth: Skinned Mesh Renderer's Bounds Extent is set to half of the Transform's Scale when using a Cloth Component ([1209765](https://issuetracker.unity3d.com/issues/skinned-mesh-renderers-bounds-extent-is-set-to-half-of-the-transforms-scale-when-using-a-cloth-component))
    
*   Polybrush: \[PolyBrush\] Something went wrong saving brush settings Warning is thrown when Saving a Brush after opening the PolyBrush Window ([1315475](https://issuetracker.unity3d.com/issues/polybrush-something-went-wrong-saving-brush-settings-warning-is-thrown-when-saving-a-brush-after-opening-the-polybrush-window))
    
*   Templates: \[Linux\] Missing libdl.so library causes crash when entering Playmode for the second time or closing the Editor ([1237642](https://issuetracker.unity3d.com/issues/missing-libdl-dot-so-library-causes-crash-when-entering-playmode-for-the-second-time-or-closing-the-editor))