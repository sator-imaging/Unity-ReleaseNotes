# Unity 2019.4.19
https://unity3d.com/unity/whats-new/2019.4.19

## Known Issues in 2019.4.19f1

<ul>
<li><p>Asset Import Pipeline: UnobservedTaskException:System.Exception: Failed to load an internal asset stored when using LoadInternalResource (<a href="https://issuetracker.unity3d.com/issues/asset-load-fails-after-restarting-unity-editor">1296212</a>)</p></li>
<li><p>Graphics Device Backends: [Mac] Editor crashes on MTLGetEnvCase on startup when metalEditorSupport is set to 0 in the ProjectSettings (<a href="https://issuetracker.unity3d.com/issues/mac-editor-crashes-on-mtlgetenvcase-on-startup-when-metaleditorsupport-is-set-to-0-in-the-projectsettings">1298617</a>)</p></li>
<li><p>Audio: [editor][fmod][macOS] Editor is preventing Mac OS from entering sleep mode automatically (<a href="https://issuetracker.unity3d.com/issues/editor-is-preventing-mac-os-from-entering-sleep-mode-automatically">995866</a>)</p></li>
<li><p>Asset Import Pipeline: Prefabs are reimporting every time a code change is made (<a href="https://issuetracker.unity3d.com/issues/prefabs-are-reimporting-every-time-a-code-change-is-made">1294785</a>)</p></li>
<li><p>Android: Crash with GenericRemote::CheckAndroidSDKPath when entering play mode (<a href="https://issuetracker.unity3d.com/issues/crash-on-mono-jit-runtime-invoke-when-entering-play-mode">1302221</a>)</p></li>
<li><p>Mobile Rendering: [Android][URP][OpenGLES] Only RenderQueue Transparent GameObjects are rendered if Opaque Texture is enabled and MSAA is 4x or 8x (<a href="https://issuetracker.unity3d.com/issues/android-urp-opengles-only-renderqueue-transparent-gameobjects-are-rendered-if-opaque-texture-is-enabled-and-msaa-is-4x-or-8x">1303685</a>)</p></li>
<li><p>iOS:  UnityWebRequest doesn't work when using a 14.2+ iOS device (<a href="https://issuetracker.unity3d.com/issues/ios-unitywebrequest-doesnt-work-when-using-a-14-dot-2-plus-ios-device">1299873</a>)</p></li>
<li><p>Global Illumination: gi::InitializeManagers() takes 0.6s during Editor startup (<a href="https://issuetracker.unity3d.com/issues/gi-initializemanagers-takes-0-dot-4s-during-editor-startup">1162775</a>)</p></li>
<li><p>Global Illumination: [macOS] BugReporter doesn't get invoked when the project crashes (<a href="https://issuetracker.unity3d.com/issues/macos-bugreporter-doesnt-get-invoked-when-the-project-crashes">1219458</a>)</p></li>
<li><p>Texture: uGUI in Texture2D is different than in the Game view when calling ToTexture2D() method on a RenderTexture (<a href="https://issuetracker.unity3d.com/issues/ugui-in-texture2d-is-different-than-in-the-game-view-when-calling-totexture2d-method-on-a-rendertexture">1301378</a>)</p></li>
<li><p>Global Illumination: [URP] Transparencies are ignored because URP uses _BaseMap as main texture identifier (<a href="https://issuetracker.unity3d.com/issues/urp-shadows-from-alpha-materials-are-not-baked-into-a-lightmap-when-using-baked-lit-shader">1246262</a>)</p></li>
<li><p>Linux:  InputSystem's Mouse delta values do not change when the Cursor lockState is set to Locked (<a href="https://issuetracker.unity3d.com/issues/linux-inputsystems-mouse-delta-values-do-not-change-when-the-cursor-lockstate-is-set-to-locked">1248389</a>)</p></li>
<li><p>Shadows/Lights: Skybox lighting is not rendered after creating gameobjects in the new scene until the lighting is rebaked (<a href="https://issuetracker.unity3d.com/issues/skybox-lighting-is-not-shown-after-creating-new-gameobjects-in-the-new-scene">1250293</a>)</p></li>
<li><p>Profiling: [Profiler] playerLoop call is automatically expanded in Raw Hierarchy when Profiler.CollectEditorStats is expanded in Hierarchy (<a href="https://issuetracker.unity3d.com/issues/profiler-playerloop-call-is-automatically-expanded-in-raw-hierarchy-when-profiler-dot-collecteditorstats-is-expanded-in-hierarchy">1242253</a>)</p></li>
<li><p>UI Toolkit: [UIR] Rendering is broken with UIToolkit with many Intel GPUs (driver-bug) (<a href="https://issuetracker.unity3d.com/issues/rendering-is-broken-with-uitoolkit-with-many-intel-gpus-driver-bug">1309555</a>)</p></li>
<li><p>XR: [XR SDK][Oculus] EarlyUpdate.XRUpdate spikes inconsistently (<a href="https://issuetracker.unity3d.com/issues/xr-sdk-oculus-earlyupdate-dot-xrupdate-spikes-inconsistently">1262597</a>)</p></li>
<li><p>Shader System: Freeze or crash with various stack traces when opening a project while connected to a VPN service (<a href="https://issuetracker.unity3d.com/issues/editor-freezes-slash-crashes-when-connected-to-nordvpn">1025558</a>)</p></li>
<li><p>Profiling: Once paused, the Profiler does not resume recording when profiling WebGL player (<a href="https://issuetracker.unity3d.com/issues/once-paused-the-profiler-does-not-resume-recording-when-profiling-webgl-player">1271012</a>)</p></li>
<li><p>Window Management: A second blank editor window is opened and may cause a crash when opening a project (<a href="https://issuetracker.unity3d.com/issues/a-second-blank-editor-window-is-opened-and-may-cause-a-crash-when-opening-a-project">1286251</a>)</p></li>
<li><p>Scene/Game View: [Wild Crash] Editor crashes on mono_aot_get_cached_class_info when GizmoSetup has cached an outdated data (<a href="https://issuetracker.unity3d.com/issues/wild-crash-editor-crashes-on-mono-aot-get-cached-class-info-when-gizmosetup-has-cached-an-outdated-data">1259765</a>)</p></li>
</ul>
