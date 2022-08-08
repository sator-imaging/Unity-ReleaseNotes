# Unity 2020.3.12

https://unity3d.com/unity/whats-new/2020.3.12

## Known Issues in 2020.3.12f1



*   AI: Crash with ComputeTileMeshJob when generating Navmesh ([1329346](https://issuetracker.unity3d.com/issues/crash-with-computetilemeshjob-when-generating-navmesh))
    
*   Animation: \[Performance Regression\] AnimationWindowState:get\_allCurves takes approximately 5000ms to load animation in the Animation window ([1320250](https://issuetracker.unity3d.com/issues/perfomance-regression-animationwindowstate-get-allcurves-takes-approximately-5000ms-to-load-animation-in-the-animation-window))
    
*   Asset Import Pipeline: Infinity loop on importing Assets, when building appx package via MRTK build window ([1339823](https://issuetracker.unity3d.com/issues/infinity-loop-on-importing-assets-when-building-appx-package-via-mrtk-build-window))
    
*   Asset Import Pipeline: Prefabs are reimporting every time a code change is made ([1294785](https://issuetracker.unity3d.com/issues/prefabs-are-reimporting-every-time-a-code-change-is-made))
    
*   Global Illumination: Crash while sculpting Terrain and Baking Lightmaps ([1266511](https://issuetracker.unity3d.com/issues/crash-while-sculpting-terrain))
    
*   Global Illumination: Reflection probes don't contain indirect scene lighting after the on-demand GI bake from the Lighting window ([1324246](https://issuetracker.unity3d.com/issues/reflection-probes-doesnt-contain-indirect-scene-lighting-after-the-on-demand-gi-bake-from-the-lighting-window))
    
*   Global Illumination: Reflection probes must be rebaked twice to update when using "Generate Lighting" button ([1334283](https://issuetracker.unity3d.com/issues/reflection-probes-must-be-rebaked-twice-to-update-when-using-generate-lighting-button))
    
*   IL2CPP: Build fails when using a combination of messages, SyncVars and SyncList in a project ([1328966](https://issuetracker.unity3d.com/issues/il2cpp-build-fails-when-using-a-combination-of-messages-syncvars-and-synclist-in-a-project))
    
*   Linux: Editor crashes at 'GfxFramebufferGLES::SetBackBufferColorDepthSurface' or freezes when creating a new shortcut profile ([1334874](https://issuetracker.unity3d.com/issues/editor-crashes-at-gfxframebuffergles-setbackbuffercolordepthsurface-or-freezes-when-creating-a-new-shortcut-profile))
    
*   Linux: Linux Editor crashes at "\_XFreeX11XCBStructure" when loading tutorials ([1323204](https://issuetracker.unity3d.com/issues/linux-editor-crashes-at-xfreex11xcbstructure-when-loading-tutorials))
    
*   Metal: Performance in Game View is significantly impacted by Gfx.WaitForPresentOnGfxThread when a second monitor is connected ([1327408](https://issuetracker.unity3d.com/issues/performance-in-game-view-is-significantly-impacted-by-gfx-dot-waitforpresentongfxthread-when-a-second-monitor-is-connected))
    
*   Mobile Graphics: \[iOS\] Player crashing when connecting external Display via USB-C port ([1321153](https://issuetracker.unity3d.com/issues/ios-player-crashing-when-connecting-external-display-via-usb-c-port))
    
*   OpenGL: SRP Batcher not working with OpenGL APIs when the project is built ([1331098](https://issuetracker.unity3d.com/issues/srp-batcher-not-working-with-opengl-apis-when-the-project-is-built))
    
*   Packman: Package Manager/My Assets: 401 Response code trying to download a paid asset store package ([1335976](https://issuetracker.unity3d.com/issues/package-manager-slash-my-assets-401-response-code-trying-to-download-a-paid-asset-store-package))
    
*   Packman: User can't easily configure location of both UPM and Asset Store package local cache ([1317232](https://issuetracker.unity3d.com/issues/user-cant-easily-configure-location-of-both-upm-and-asset-store-package-local-cache))
    
*   Polybrush: \[PolyBrush\] Something went wrong saving brush settings Warning is thrown when Saving a Brush after opening the PolyBrush Window ([1315475](https://issuetracker.unity3d.com/issues/polybrush-something-went-wrong-saving-brush-settings-warning-is-thrown-when-saving-a-brush-after-opening-the-polybrush-window))
    
*   Profiling: GarbageCollectAssets is triggered frequently when higher frame counts are set ([1332708](https://issuetracker.unity3d.com/issues/garbagecollectassets-is-triggered-frequently-when-higher-frame-counts-are-set))
    
*   Profiling: Poor profiler performance when navigating the timeline view and reviewing data with many threads ([1339407](https://issuetracker.unity3d.com/issues/poor-profiler-performance-when-navigating-the-timeline-view-and-reviewing-data-with-many-threads))
    
*   Scene Management: Crash on BuildPrefabInstanceCorrespondingObjectMap when overriding nested prefab inside AssetDatabase.StartAssetEditing() block ([1324978](https://issuetracker.unity3d.com/issues/crash-on-buildprefabinstancecorrespondingobjectmap-when-overriding-nested-prefab-inside-assetdatabase-dot-startassetediting-block))
    
*   Scripting: Crashes on mono\_class\_init when entering Play Mode after recompiling scripts ([1262671](https://issuetracker.unity3d.com/issues/crashes-on-mono-class-init-when-entering-play-mode-after-recompiling-scripts))
    
*   Scripting: Increased Script Assembly reload time ([1323490](https://issuetracker.unity3d.com/issues/increased-reload-time))
    
*   Scripting: \[Android\]\[Mono\]\[IL2CPP\] "Unable to find libc" error thrown when executing certain SslStream constructor ([1022228](https://issuetracker.unity3d.com/issues/android-mono-il2cpp-unable-to-find-libc-error-thrown-when-executing-certain-sslstream-constructor))
    
*   Templates: Editor Crashes when performing Undo and Redo after duplicating Game Object with LEGO Model Asset component ([1298503](https://issuetracker.unity3d.com/issues/crash-when-redoing-and-undoing-pasting-prefabs-in-scene-in-lego-microgame))
    
*   Templates: \[Linux\] Missing libdl.so library causes crash when entering Playmode for the second time or closing the Editor ([1237642](https://issuetracker.unity3d.com/issues/missing-libdl-dot-so-library-causes-crash-when-entering-playmode-for-the-second-time-or-closing-the-editor))
    
*   Terrain: Crash on TreeRenderer::WillRenderTrees when being in Play Mode for several seconds ([1317966](https://issuetracker.unity3d.com/issues/crash-on-treerenderer-willrendertrees-when-being-in-play-mode-for-several-seconds))
    
*   uGUI: RectMask2D Softness property has no effect when used on TextMeshPro Text ([1331297](https://issuetracker.unity3d.com/issues/rectmask2d-softness-property-has-no-effect-when-used-on-textmeshpro-text))
    
*   Windows: Editor crashes when exiting and keeping a tutorial project ([1338299](https://issuetracker.unity3d.com/issues/editor-crashes-when-exiting-and-keeping-a-new-micrograme-project))