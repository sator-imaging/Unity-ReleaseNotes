# Unity 2019.4.20

https://unity3d.com/unity/whats-new/2019.4.20

## Known Issues in 2019.4.20f1



*   Asset Import Pipeline: Crash on mdb\_txn\_begin when SourceAssetDB has a lock on it from another process ([1208749](https://issuetracker.unity3d.com/issues/crash-on-mdb-txn-begin-when-sourceassetdb-has-a-lock-on-it-from-another-process))
    
*   Android: Crash with GenericRemote::CheckAndroidSDKPath when entering play mode ([1302221](https://issuetracker.unity3d.com/issues/crash-on-mono-jit-runtime-invoke-when-entering-play-mode))
    
*   Global Illumination: Reflection Probe is not baked after pressing "Bake" button in the per-probe Inspector window (1311231)
    
*   Asset Import Pipeline: Prefabs are reimporting every time a code change is made ([1294785](https://issuetracker.unity3d.com/issues/prefabs-are-reimporting-every-time-a-code-change-is-made))
    
*   Mobile Rendering: \[Android\]\[URP\]\[OpenGLES\] Only RenderQueue Transparent GameObjects are rendered if Opaque Texture is enabled and MSAA is 4x or 8x ([1303685](https://issuetracker.unity3d.com/issues/android-urp-opengles-only-renderqueue-transparent-gameobjects-are-rendered-if-opaque-texture-is-enabled-and-msaa-is-4x-or-8x))
    
*   Metal: \[Apple M1\] Crash on MTLGetEnvCase on startup when 'm\_Automatic' is set to 0 in the ProjectSettings ([1306688](https://issuetracker.unity3d.com/issues/apple-m1-crash-on-mtlgetenvcase-on-startup-when-m-automatic-is-set-to-0-in-the-projectsettings))
    
*   Cloth: Skinned Mesh Renderer's Bounds Extent is set to half of the Transform's Scale when using a Cloth Component ([1209765](https://issuetracker.unity3d.com/issues/skinned-mesh-renderers-bounds-extent-is-set-to-half-of-the-transforms-scale-when-using-a-cloth-component))
    
*   Terrain: Terrain Lit Opacity as Density option causes alpha'd areas on the 5th layer or greater to appear with artifacts ([1283124](https://issuetracker.unity3d.com/issues/terrain-lit-opacity-as-density-option-causes-alphad-areas-on-the-5th-layer-or-greater-to-appear-with-artifacts))
    
*   Shadows/Lights: Crash on ProgressiveRuntimeManager::GetGBufferChartTexture when entering UV Charts mode before baking lights ([1309632](https://issuetracker.unity3d.com/issues/crash-on-progressiveruntimemanager-getgbuffercharttexture-when-entering-uv-charts-mode-before-baking-lights))
    
*   Global Illumination: gi::InitializeManagers() takes 0.6s during Editor startup ([1162775](https://issuetracker.unity3d.com/issues/gi-initializemanagers-takes-0-dot-4s-during-editor-startup))
    
*   Global Illumination: \[macOS\] BugReporter doesn't get invoked when the project crashes ([1219458](https://issuetracker.unity3d.com/issues/macos-bugreporter-doesnt-get-invoked-when-the-project-crashes))
    
*   Texture: uGUI in Texture2D is different than in the Game view when calling ToTexture2D() method on a RenderTexture ([1301378](https://issuetracker.unity3d.com/issues/ugui-in-texture2d-is-different-than-in-the-game-view-when-calling-totexture2d-method-on-a-rendertexture))
    
*   Windows: The Cursor is visible when Cursor.visible is set to false and new InputSystem package is used ([1273522](https://issuetracker.unity3d.com/issues/the-cursor-dot-visible-equals-false-does-not-work-when-inputsystem-package-is-installed))
    
*   Linux: InputSystem's Mouse delta values do not change when the Cursor lockState is set to Locked ([1248389](https://issuetracker.unity3d.com/issues/linux-inputsystems-mouse-delta-values-do-not-change-when-the-cursor-lockstate-is-set-to-locked))
    
*   Graphics Device Backends: \[Mac\] Editor crashes on MTLGetEnvCase on startup when metalEditorSupport is set to 0 in the ProjectSettings ([1298617](https://issuetracker.unity3d.com/issues/mac-editor-crashes-on-mtlgetenvcase-on-startup-when-metaleditorsupport-is-set-to-0-in-the-projectsettings))
    
*   Audio: \[editor\]\[fmod\]\[macOS\] Editor is preventing Mac OS from entering sleep mode automatically ([995866](https://issuetracker.unity3d.com/issues/editor-is-preventing-mac-os-from-entering-sleep-mode-automatically))
    
*   Scene/Game View: \[Wild Crash\] Editor crashes on mono\_aot\_get\_cached\_class\_info when GizmoSetup has cached an outdated data ([1259765](https://issuetracker.unity3d.com/issues/wild-crash-editor-crashes-on-mono-aot-get-cached-class-info-when-gizmosetup-has-cached-an-outdated-data))
    
*   Profiling: Once paused, the Profiler does not resume recording when profiling WebGL player ([1271012](https://issuetracker.unity3d.com/issues/once-paused-the-profiler-does-not-resume-recording-when-profiling-webgl-player))
    
*   Profiling: \[Profiler\] playerLoop call is automatically expanded in Raw Hierarchy when Profiler.CollectEditorStats is expanded in Hierarchy ([1242253](https://issuetracker.unity3d.com/issues/profiler-playerloop-call-is-automatically-expanded-in-raw-hierarchy-when-profiler-dot-collecteditorstats-is-expanded-in-hierarchy))
    
*   Asset Import Pipeline: UnobservedTaskException:System.Exception: Failed to load an internal asset stored when using LoadInternalResource ([1296212](https://issuetracker.unity3d.com/issues/asset-load-fails-after-restarting-unity-editor))
    
*   Global Illumination: \[URP\] Transparencies are ignored because URP uses \_BaseMap as main texture identifier ([1246262](https://issuetracker.unity3d.com/issues/urp-shadows-from-alpha-materials-are-not-baked-into-a-lightmap-when-using-baked-lit-shader))
    
*   iOS: UnityWebRequest doesn't work when using a 14.2+ iOS device ([1299873](https://issuetracker.unity3d.com/issues/ios-unitywebrequest-doesnt-work-when-using-a-14-dot-2-plus-ios-device))
    
*   XR: \[XR SDK\]\[Oculus\] EarlyUpdate.XRUpdate spikes inconsistently ([1262597](https://issuetracker.unity3d.com/issues/xr-sdk-oculus-earlyupdate-dot-xrupdate-spikes-inconsistently))