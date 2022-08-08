# Unity 2019.4.22

https://unity3d.com/unity/whats-new/2019.4.22

## Known Issues in 2019.4.22f1



*   Cloth: Cloth is broken when parent GameObject scale is lower than 1 and Surface Penetration constraints are set 0 ([1319488](https://issuetracker.unity3d.com/issues/cloth-is-broken-when-parent-gameobject-scale-is-lower-than-1-and-surface-penetration-constraints-are-set-0))
    
*   Linux: Linux Editor throws "X Server took longer than x miliseconds to respond to SetGtkWindowSizeAndPosition" error after opening ([1309607](https://issuetracker.unity3d.com/issues/linux-editor-throws-x-server-took-longer-than-x-miliseconds-to-respond-to-setgtkwindowsizeandposition-error-after-opening))
    
*   Global Illumination: \[macOS\] BugReporter doesn't get invoked when the project crashes ([1219458](https://issuetracker.unity3d.com/issues/macos-bugreporter-doesnt-get-invoked-when-the-project-crashes))
    
*   Profiling: \[Profiler\] Timeline sample names from surrounding frames disappear when zooming or panning ([1317697](https://issuetracker.unity3d.com/issues/profiler-timeline-sample-names-from-surrounding-frames-disappear-when-zooming-or-panning))
    
*   Shader System: Crash on PAL\_LocalIPC\_IsConnected when IPC fails on launch ([1319336](https://issuetracker.unity3d.com/issues/crash-on-pal-localipc-isconnected-when-ipc-fails-on-launch))
    
*   Mobile Rendering: \[Android\]\[URP\]\[OpenGLES\] Only RenderQueue Transparent GameObjects are rendered if Opaque Texture is enabled and MSAA is 4x or 8x ([1303685](https://issuetracker.unity3d.com/issues/android-urp-opengles-only-renderqueue-transparent-gameobjects-are-rendered-if-opaque-texture-is-enabled-and-msaa-is-4x-or-8x))
    
*   iOS: \[WebGL\] \[iOS\] video is not playing on iOS ([1288692](https://issuetracker.unity3d.com/issues/webgl-ios-video-is-not-playing-on-ios))
    
*   Metal: \[Apple M1\] Crash on MTLGetEnvCase on startup when 'm\_Automatic' is set to 0 in the ProjectSettings ([1306688](https://issuetracker.unity3d.com/issues/apple-m1-crash-on-mtlgetenvcase-on-startup-when-m-automatic-is-set-to-0-in-the-projectsettings))
    
*   Terrain: Terrain Lit Opacity as Density option causes alpha'd areas on the 5th layer or greater to appear with artifacts ([1283124](https://issuetracker.unity3d.com/issues/terrain-lit-opacity-as-density-option-causes-alphad-areas-on-the-5th-layer-or-greater-to-appear-with-artifacts))
    
*   Shadows/Lights: Crash on ProgressiveRuntimeManager::GetGBufferChartTexture when entering UV Charts mode before baking lights ([1309632](https://issuetracker.unity3d.com/issues/crash-on-progressiveruntimemanager-getgbuffercharttexture-when-entering-uv-charts-mode-before-baking-lights))
    
*   Global Illumination: gi::InitializeManagers() takes 0.6s during Editor startup ([1162775](https://issuetracker.unity3d.com/issues/gi-initializemanagers-takes-0-dot-4s-during-editor-startup))
    
*   Linux: InputSystem's Mouse delta values do not change when the Cursor lockState is set to Locked ([1248389](https://issuetracker.unity3d.com/issues/linux-inputsystems-mouse-delta-values-do-not-change-when-the-cursor-lockstate-is-set-to-locked))
    
*   Mobile Rendering: \[iOS\]\[tvOS\] Built-in deferred rendering path is not functioning on some devices ([1317077](https://issuetracker.unity3d.com/issues/ios-tvos-built-in-deferred-rendering-path-is-not-functioning-on-some-devices))
    
*   Asset Import Pipeline: Crash on mdb\_txn\_begin when SourceAssetDB has a lock on it from another process ([1208749](https://issuetracker.unity3d.com/issues/crash-on-mdb-txn-begin-when-sourceassetdb-has-a-lock-on-it-from-another-process))
    
*   Cloth: Skinned Mesh Renderer's Bounds Extent is set to half of the Transform's Scale when using a Cloth Component ([1209765](https://issuetracker.unity3d.com/issues/skinned-mesh-renderers-bounds-extent-is-set-to-half-of-the-transforms-scale-when-using-a-cloth-component))
    
*   Shuriken: Crash on ParticleSystem::EndUpdateAll ([1311212](https://issuetracker.unity3d.com/issues/shuriken-crash-on-particlesystem-endupdateall))
    
*   Audio: \[editor\]\[fmod\]\[macOS\] Editor is preventing Mac OS from entering sleep mode automatically ([995866](https://issuetracker.unity3d.com/issues/editor-is-preventing-mac-os-from-entering-sleep-mode-automatically))
    
*   Serialization: Editor crashes on RaiseException when allocating huge amount of memory ([1313492](https://issuetracker.unity3d.com/issues/editor-crashes-on-raiseexception-when-allocating-huge-amount-of-memory))
    
*   Linux: "Out of memory!" crash when opening Unity on Ubuntu 20.04 ([1262894](https://issuetracker.unity3d.com/issues/linux-out-of-memory-crash-when-opening-unity-on-ubuntu-20-dot-04))
    
*   Graphics - LowLevel: vSyncCount does not work and targetFrameRate is not ignored when vSyncCount is used in the Play Mode ([1305631](https://issuetracker.unity3d.com/issues/vsynccount-does-not-work-when-used-in-the-play-mode))
    
*   Mobile: Screen.dpi returns 0 on iPad Pro for projects built from 2019.4.16f1 ([1300359](https://issuetracker.unity3d.com/issues/screen-dot-dpi-returns-0-on-ipad-pro-for-projects-built-from-2019-dot-4-16f1))
    
*   Windows: The Cursor is visible when Cursor.visible is set to false and new InputSystem package is used ([1273522](https://issuetracker.unity3d.com/issues/the-cursor-dot-visible-equals-false-does-not-work-when-inputsystem-package-is-installed))
    
*   Serialization: JsonUtility Deserialization Corrupted Values ([1296236](https://issuetracker.unity3d.com/issues/jsonutility-deserialization-corrupted-values))
    
*   Polybrush: \[PolyBrush\] Something went wrong saving brush settings Warning is thrown when Saving a Brush after opening the PolyBrush Window ([1315475](https://issuetracker.unity3d.com/issues/polybrush-something-went-wrong-saving-brush-settings-warning-is-thrown-when-saving-a-brush-after-opening-the-polybrush-window))
    
*   Graphics Device Backends: \[Mac\] Editor crashes on MTLGetEnvCase on startup when metalEditorSupport is set to 0 in the ProjectSettings ([1298617](https://issuetracker.unity3d.com/issues/mac-editor-crashes-on-mtlgetenvcase-on-startup-when-metaleditorsupport-is-set-to-0-in-the-projectsettings))