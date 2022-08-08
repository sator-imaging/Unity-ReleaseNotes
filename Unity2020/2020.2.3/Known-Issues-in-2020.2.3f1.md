# Unity 2020.2.3

https://unity3d.com/unity/whats-new/2020.2.3

## Known Issues in 2020.2.3f1



*   Scene/Game View: \[Wild Crash\] Editor crashes on mono\_aot\_get\_cached\_class\_info when GizmoSetup has cached an outdated data ([1259765](https://issuetracker.unity3d.com/issues/wild-crash-editor-crashes-on-mono-aot-get-cached-class-info-when-gizmosetup-has-cached-an-outdated-data))
    
*   uGUI: AspectRatioFitter gives a warning when changing the Components Aspect Ratio if it's attached to a Canvas ([1302464](https://issuetracker.unity3d.com/issues/aspectratiofitter-new-restriction-in-2020-dot-2))
    
*   Global Illumination: Reflection Probe is not baked after pressing "Bake" button in the per-probe Inspector window (1311231)
    
*   Build Pipeline: \[Cache Server\] Building process freezes on compiling shader variants when connected to Accelerator ([1296800](https://issuetracker.unity3d.com/issues/cache-server-building-process-freezes-on-compiling-shader-variants-when-connected-to-accelerator))
    
*   Shuriken: Infinity loop issue about Sub-Emitters of Particle System Editor ([1311111](https://issuetracker.unity3d.com/issues/infinity-loop-issue-about-sub-emitters-of-particle-system-editor))
    
*   Templates: Editor Crashes when performing Undo and Redo after duplicating Game Object with LEGO Model Asset component ([1298503](https://issuetracker.unity3d.com/issues/crash-when-redoing-and-undoing-pasting-prefabs-in-scene-in-lego-microgame))
    
*   Android: Crash with GenericRemote::CheckAndroidSDKPath when entering play mode ([1302221](https://issuetracker.unity3d.com/issues/crash-on-mono-jit-runtime-invoke-when-entering-play-mode))
    
*   Global Illumination: \[macOS\] BugReporter doesn't get invoked when the project crashes ([1219458](https://issuetracker.unity3d.com/issues/macos-bugreporter-doesnt-get-invoked-when-the-project-crashes))
    
*   Visual Effects: \[URP\] OutputUpdate.compute: Kernel at index (0) is invalid when using compute culling, Lod, or Multi-mesh ([1309174](https://issuetracker.unity3d.com/issues/urp-outputupdate-dot-compute-kernel-at-index-0-is-invalid-when-using-compute-culling-lod-or-multi-mesh))
    
*   Cloth: Skinned Mesh Renderer's Bounds Extent is set to half of the Transform's Scale when using a Cloth Component ([1209765](https://issuetracker.unity3d.com/issues/skinned-mesh-renderers-bounds-extent-is-set-to-half-of-the-transforms-scale-when-using-a-cloth-component))
    
*   UI Toolkit: Editor Crashes when name of Serialized Sprite variable is edited ([1302872](https://issuetracker.unity3d.com/issues/editor-crashes-when-name-of-serialized-sprite-variable-is-edited))
    
*   Input: \[Input System\] MultiplayerEventSystem throws a warning when more than one MultiplayerEventSystem is active ([1303961](https://issuetracker.unity3d.com/issues/input-system-multiplayereventsystem-throws-a-warning-when-more-than-one-multiplayereventsystem-is-active))
    
*   Texture: uGUI in Texture2D is different than in the Game view when calling ToTexture2D() method on a RenderTexture ([1301378](https://issuetracker.unity3d.com/issues/ugui-in-texture2d-is-different-than-in-the-game-view-when-calling-totexture2d-method-on-a-rendertexture))
    
*   Asset Importers: \[Performance Regression\] Importing an fbx model is noticeably slower when the model contains Animations ([1265275](https://issuetracker.unity3d.com/issues/performance-regression-importing-an-fbx-model-is-noticeably-slower-when-the-model-contains-animations))
    
*   Linux: InputSystem's Mouse delta values do not change when the Cursor lockState is set to Locked ([1248389](https://issuetracker.unity3d.com/issues/linux-inputsystems-mouse-delta-values-do-not-change-when-the-cursor-lockstate-is-set-to-locked))
    
*   Asset Import Pipeline: UnobservedTaskException:System.Exception: Failed to load an internal asset stored when using LoadInternalResource ([1296212](https://issuetracker.unity3d.com/issues/asset-load-fails-after-restarting-unity-editor))
    
*   Quality of Life: Infinite load when trying to display Lists of custom classes in Inspector ([1298594](https://issuetracker.unity3d.com/issues/infinite-load-when-trying-to-display-lists-of-custom-classes-in-inspector))
    
*   Profiling: Once paused, the Profiler does not resume recording when profiling WebGL player ([1271012](https://issuetracker.unity3d.com/issues/once-paused-the-profiler-does-not-resume-recording-when-profiling-webgl-player))
    
*   Asset Import Pipeline: Prefabs are reimporting every time a code change is made ([1294785](https://issuetracker.unity3d.com/issues/prefabs-are-reimporting-every-time-a-code-change-is-made))
    
*   Vulkan: Crash in Windows Standalone when Vulkan is set as rendering API and player window is out of focus ([1309519](https://issuetracker.unity3d.com/issues/vulkan-crash-in-windows-standalone-when-vulkan-is-set-as-rendering-api-and-player-window-is-out-of-focus))
    
*   Profiling: \[Profiler\] playerLoop call is automatically expanded in Raw Hierarchy when Profiler.CollectEditorStats is expanded in Hierarchy ([1242253](https://issuetracker.unity3d.com/issues/profiler-playerloop-call-is-automatically-expanded-in-raw-hierarchy-when-profiler-dot-collecteditorstats-is-expanded-in-hierarchy))
    
*   Asset Import Pipeline: CPU usage spikes in the Loading.LockPersistentManager when async loading/unloading Scenes with Terrain ([1276854](https://issuetracker.unity3d.com/issues/cpu-usage-spikes-in-the-loading-dot-lockpersistentmanager-when-async-loading-slash-unloading-scenes-with-terrain))
    
*   UI Toolkit: \[UIR\] Rendering is broken with UIToolkit with many Intel GPUs (driver-bug) ([1309555](https://issuetracker.unity3d.com/issues/rendering-is-broken-with-uitoolkit-with-many-intel-gpus-driver-bug))
    
*   XR: \[XR SDK\]\[Oculus\] EarlyUpdate.XRUpdate spikes inconsistently ([1262597](https://issuetracker.unity3d.com/issues/xr-sdk-oculus-earlyupdate-dot-xrupdate-spikes-inconsistently))
    
*   iOS: UnityWebRequest doesn't work when using a 14.2+ iOS device ([1299873](https://issuetracker.unity3d.com/issues/ios-unitywebrequest-doesnt-work-when-using-a-14-dot-2-plus-ios-device))
    
*   Scene Management: Crash on StackAllocator::WalkAllocations when loading another Scene whilst in Play Mode ([1297307](https://issuetracker.unity3d.com/issues/crash-on-stackallocator-walkallocations-when-loading-another-scene-whilst-in-play-mode))
    
*   Shadows/Lights: Skybox lighting is not rendered after creating gameobjects in the new scene until the lighting is rebaked ([1250293](https://issuetracker.unity3d.com/issues/skybox-lighting-is-not-shown-after-creating-new-gameobjects-in-the-new-scene))
    
*   Packman: Unable to filter on downloaded assets ([1307862](https://issuetracker.unity3d.com/issues/unable-to-filter-on-downloaded-assets))