# Unity 2020.1.15

https://unity3d.com/unity/whats-new/2020.1.15

## Known Issues in 2020.1.15f1



*   Asset Import Pipeline: Texture Assets are reimported when the launched Editor is recovering from an unexpected close if there were compilation errors ([1264055](https://issuetracker.unity3d.com/issues/texture-assets-are-reimported-when-the-launched-editor-is-recovering-from-an-unexpected-close-if-there-were-compilation-errors))
    
*   Asset Importers: \[Performance Regression\] Importing an fbx model is noticeably slower when the model contains Animations ([1265275](https://issuetracker.unity3d.com/issues/performance-regression-importing-an-fbx-model-is-noticeably-slower-when-the-model-contains-animations))
    
*   Global Illumination: \[OSX\] Crash on 'Preparing Bake' stage when rebaking GI after changing lighting settings and clearing baked data ([1271626](https://issuetracker.unity3d.com/issues/osx-crash-on-preparing-bake-stage-when-rebaking-gi-after-changing-lighting-settings-and-clearing-baked-data))
    
*   Global Illumination: \[macOS\] BugReporter doesn't get invoked when the project crashes ([1219458](https://issuetracker.unity3d.com/issues/macos-bugreporter-doesnt-get-invoked-when-the-project-crashes))
    
*   Global Illumination: gi::InitializeManagers() takes 0.6s during Editor startup ([1162775](https://issuetracker.unity3d.com/issues/gi-initializemanagers-takes-0-dot-4s-during-editor-startup))
    
*   IL2CPP: UnityLinker strips classes used with the SerializeReference attribute ([1232785](https://issuetracker.unity3d.com/issues/unitylinker-strips-classes-used-with-the-serializereference-attribute))
    
*   Linux: InputSystem's Mouse delta values do not change when the Cursor lockState is set to Locked ([1248389](https://issuetracker.unity3d.com/issues/linux-inputsystems-mouse-delta-values-do-not-change-when-the-cursor-lockstate-is-set-to-locked))
    
*   Package: \[Reflect\] Standalone build fails with package errors if Unity Reflect is installed ([1266377](https://issuetracker.unity3d.com/issues/reflect-standalone-build-fails-with-package-errors-if-unity-reflect-is-installed))
    
*   Shadows/Lights: Skybox lighting is not rendered after creating gameobjects in the new scene until the lighting is rebaked ([1250293](https://issuetracker.unity3d.com/issues/skybox-lighting-is-not-shown-after-creating-new-gameobjects-in-the-new-scene))
    
*   XR: \[XR SDK\]\[Oculus\] EarlyUpdate.XRUpdate spikes inconsistently ([1262597](https://issuetracker.unity3d.com/issues/xr-sdk-oculus-earlyupdate-dot-xrupdate-spikes-inconsistently))
    
*   iOS: Crash on il2cpp::vm::LivenessState::AddProcessObject when using Social.LoadUsers and then changing scenes ([1270230](https://issuetracker.unity3d.com/issues/ios-il2cpp-crash-on-il2cpp-vm-livenessstate-addprocessobject-when-using-social-dot-loadusers-and-then-changing-scenes))
    
*   iOS: \[UaaL\] UnityFramework with 3rd party plugins triggers watchdog termination after launch ([1262272](https://issuetracker.unity3d.com/issues/ios-unityframework-with-3rd-party-plugins-triggers-watchdog-termination-after-launch))
    
*   iOS: \[iOS 14\] VideoPlayer crashes on EXC\_BAD\_ACCESS or signal SIGABRT when audioOutputMode is set to APIOnly or Audio Source ([1274837](https://issuetracker.unity3d.com/issues/ios-videoplayer-crashes-when-audiooutputmode-is-set-to-apionly-or-audiosource))