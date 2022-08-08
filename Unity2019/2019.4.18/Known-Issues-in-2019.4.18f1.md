# Unity 2019.4.18

https://unity3d.com/unity/whats-new/2019.4.18

## Known Issues in 2019.4.18f1



*   Asset Import Pipeline: Prefabs are reimporting every time a code change is made ([1294785](https://issuetracker.unity3d.com/issues/prefabs-are-reimporting-every-time-a-code-change-is-made))
    
*   Serialization: Crash on WalkTypeTreeComplete<`SerializedProperty::ContainsManagedReferences'::`2'::IsManagedReferenceVisitor> ([1302360](https://issuetracker.unity3d.com/issues/crash-on-walktypetreecomplete-serializedproperty-containsmanagedreferences-2-ismanagedreferencevisitor))
    
*   Shadows/Lights: Skybox lighting is not rendered after creating gameobjects in the new scene until the lighting is rebaked ([1250293](https://issuetracker.unity3d.com/issues/skybox-lighting-is-not-shown-after-creating-new-gameobjects-in-the-new-scene))
    
*   Audio: \[editor\]\[fmod\]\[macOS\] Editor is preventing Mac OS from entering sleep mode automatically ([995866](https://issuetracker.unity3d.com/issues/editor-is-preventing-mac-os-from-entering-sleep-mode-automatically))
    
*   Global Illumination: \[URP\] Transparencies are ignored because URP uses \_BaseMap as main texture identifier ([1246262](https://issuetracker.unity3d.com/issues/urp-shadows-from-alpha-materials-are-not-baked-into-a-lightmap-when-using-baked-lit-shader))
    
*   Graphics Device Backends: \[Mac\] Editor crashes on MTLGetEnvCase on startup when metalEditorSupport is set to 0 in the ProjectSettings ([1298617](https://issuetracker.unity3d.com/issues/mac-editor-crashes-on-mtlgetenvcase-on-startup-when-metaleditorsupport-is-set-to-0-in-the-projectsettings))
    
*   Profiling: Once paused, the Profiler does not resume recording when profiling WebGL player ([1271012](https://issuetracker.unity3d.com/issues/once-paused-the-profiler-does-not-resume-recording-when-profiling-webgl-player))
    
*   Shader System: Freeze or crash with various stack traces when opening a project while connected to a VPN service ([1025558](https://issuetracker.unity3d.com/issues/editor-freezes-slash-crashes-when-connected-to-nordvpn))
    
*   Linux: InputSystem's Mouse delta values do not change when the Cursor lockState is set to Locked ([1248389](https://issuetracker.unity3d.com/issues/linux-inputsystems-mouse-delta-values-do-not-change-when-the-cursor-lockstate-is-set-to-locked))
    
*   Global Illumination: \[macOS\] BugReporter doesn't get invoked when the project crashes ([1219458](https://issuetracker.unity3d.com/issues/macos-bugreporter-doesnt-get-invoked-when-the-project-crashes))
    
*   Global Illumination: gi::InitializeManagers() takes 0.6s during Editor startup ([1162775](https://issuetracker.unity3d.com/issues/gi-initializemanagers-takes-0-dot-4s-during-editor-startup))
    
*   iOS: \[iOS 14\] VideoPlayer crashes on EXC\_BAD\_ACCESS or signal SIGABRT when audioOutputMode is set to APIOnly or Audio Source ([1274837](https://issuetracker.unity3d.com/issues/ios-videoplayer-crashes-when-audiooutputmode-is-set-to-apionly-or-audiosource))
    
*   Asset Import Pipeline: Parent and child nested Scriptable Object Assets switch places when parent Scriptable Object Asset is renamed ([1189089](https://issuetracker.unity3d.com/issues/parent-and-child-nested-scriptable-object-assets-switch-places-when-parent-scriptable-object-asset-is-renamed))
    
*   iOS: Crash on il2cpp::vm::LivenessState::AddProcessObject when using Social.LoadUsers and then changing scenes ([1270230](https://issuetracker.unity3d.com/issues/ios-il2cpp-crash-on-il2cpp-vm-livenessstate-addprocessobject-when-using-social-dot-loadusers-and-then-changing-scenes))
    
*   XR: \[XR SDK\]\[Oculus\] EarlyUpdate.XRUpdate spikes inconsistently ([1262597](https://issuetracker.unity3d.com/issues/xr-sdk-oculus-earlyupdate-dot-xrupdate-spikes-inconsistently))
    
*   Packman: Package Manager doesn't show available updates ([1304459](https://issuetracker.unity3d.com/issues/package-manager-doesnt-show-available-updates))
    
*   WebGL: \[Audio\] "Cannot create FMOD" Error when importing 3D Game Kit project on webGL ([1293595](https://issuetracker.unity3d.com/issues/audio-cannot-create-fmod-error-when-importing-3d-game-kit-project-on-webgl))