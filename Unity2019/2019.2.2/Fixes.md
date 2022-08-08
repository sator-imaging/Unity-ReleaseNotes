# Unity 2019.2.2

https://unity3d.com/unity/whats-new/2019.2.2

## Fixes



*   macOS: Fixes an issue with macOS Catalina that causes Unity to request permission to receive keyboard input when using other apps in both the editor and standalone player. (1172758)
    
*   Android: Application.Quit will correctly quit the application process, previously it would only destroy Unity runtime, keeping activity alive, that lead to incorrect application resume. ([1171368](https://issuetracker.unity3d.com/issues/reopening-app-after-application-dot-quit-causes-unity-on-android-iap-sdk-to-not-initialise-successfully), 1172043)
    
*   Android: Fixed a Vulkan video playback crash. (1170411, 1174468)
    
*   Apple TV: Fixed regression, where clicking B on gamepad would show "JoystickButton0" as pressed. ([1151006](https://issuetracker.unity3d.com/issues/tvos-when-b-button-is-pressed-on-a-wireless-controller-connected-to-a-tvos-the-menu-button-joystickbutton0-is-shown-as-held), 1172037)
    
*   Apple TV: GetKeyDown and GetKeyUp will work correctly with Siri Remote buttons. Due platform limitation, GetKeyDown, GetKeyUp will work with delay when receiving events from keyboard, see documentation for more info. ([1143342](https://issuetracker.unity3d.com/issues/tvos-getkeydown-and-getkeyup-are-set-to-true-every-few-frames-when-holding-down-any-key-on-wireless-tv-remote-or-keyboard), 1172039)
    
*   Apple TV: Pressing menu button on Siri remote will correctly exit to home screen, if tvOS.Remote.allowExitToHome is set to true. ([1134856](https://issuetracker.unity3d.com/issues/ios-pressing-the-menu-button-on-appletv-remote-doesnt-exit-to-home-screen-when-tvos-dot-remote-dot-allowexittohome-is-set-to-true), 1171972)
    
*   Asset Import: Local fileIDs of FBX meshes are correctly upgraded from Unity 2018 and previous version when multiple meshes share the same name. (1169597, 1173704)
    
*   Editor: Fix incorrect colorspace for IMGUI in GameView. ([1168191](https://issuetracker.unity3d.com/issues/gui-dot-drawtexture-is-too-bright-slash-washed-out-when-color-space-is-set-to-linear-mode), 1173822)
    
*   Editor: MacEditor: "Unsupported image when converting for NSImage" log is now a DebugAssert, which will prevent the assert from being logged on build machines (1171194, 1172797)
    
*   Editor: Project Settings Window fails to appear after installing the Ryder Editor package. ([1168648](https://issuetracker.unity3d.com/issues/project-settings-window-fails-to-appear-after-installing-the-ryder-editor-package), 1173051)
    
*   Graphics: Fixed crash in the Editor that could be caused by having optimization enabled on meshes with empty sub-objects ([1166419](https://issuetracker.unity3d.com/issues/crash-on-optimizemeshjobdata-optimizemeshjob-when-calling-mesh-dot-optimize), 1174412)
    
*   Graphics: Fixed rare deadlock in CreateGpuProgram when multithreaded rendering is enabled on mobile devices. (1164492, 1174042)
    
*   IL2CPP: Fixed a crash when accessing the LocalEndpoint property of a socket using an IPV6 connection. ([1167971](https://issuetracker.unity3d.com/issues/constructor-ipendpoint-ipadress-int-throws-an-exception-when-using-ipv6-tcp-streams-in-il2cpp-builds), 1170304)
    
*   IL2CPP: Fixed an issue with nested type metadata being re-initialized without checking for previous initialization, which caused a memory leak in certain situations. ([1167380](https://issuetracker.unity3d.com/issues/il2cpp-memory-leak-in-particlesystem-dot-getparticles-when-using-a-mesh-particle), 1171265)
    
*   Kernel: Fixed player crash due to stack overflow in Loading.PreloadManager thread (1162496, 1174959)
    
*   Package Manager: Fix OSX - Package Manifest is not editable due to permission errors. ([1174911](https://issuetracker.unity3d.com/issues/osx-package-manifest-is-not-editable-due-to-permission-errors), 1175426)
    
*   Particles: Fix a case where particle trails could flicker if their owning system used ParticleSystem.SetParticles in script during LateUpdate. ([1155826](https://issuetracker.unity3d.com/issues/particlesystem-trails-cause-artefacts-when-using-setparticles-in-lateupdate-and-particle-gets-destroyed), 1171470)
    
*   Particles: Fix a crash if using a non-read-write mesh from an Asset Bundle in the Particle System Shape Module. ([1167081](https://issuetracker.unity3d.com/issues/editor-crashes-in-trianglearea3d-when-instantiating-a-particlesystem-prefab-reference-to-a-non-readable-mesh-in-an-assetbundle), 1171473)
    
*   Particles: Fix case where trails sometiems did not disappear. ([1162394](https://issuetracker.unity3d.com/issues/particle-system-trails-do-not-die-after-particles-die-when-instantiating-large-quantity-of-particle-systems-for-20-plus-seconds), 1171477)
    
*   Particles: Fix erroneous GetTransformInfoExpectUpToDate message. ([1098990](https://issuetracker.unity3d.com/issues/lwrp-instantiating-particle-system-prefabs-with-ienumerator-produces-errors), 1171479)
    
*   Particles: Fixed case where Auto Random Seed was ignored for the Emission Rate property. ([1166733](https://issuetracker.unity3d.com/issues/shuriken-auto-random-seed-doesnt-work-for-random-emission-rate-between-constants-or-curves), 1171468)
    
*   Physics: Fixed an issue when reparenting a GameObject with multiple static Collider2D which resulted in them not being correctly attached to the parent Rigidbody2D. ([1174519](https://issuetracker.unity3d.com/issues/collider-stays-behind-when-gameobject-with-multiple-colliders-is-set-as-child-in-script-of-object-which-moves-using-rigidbody2d), 1174697)
    
*   Physics: Fixed crash when changing Collider2D rigidbody while contacts are still active. ([1065886](https://issuetracker.unity3d.com/issues/crash-on-gameobject-sendmessageany-when-detached-child-gameobjects-collision-destroys-parent-gameobject), 1174064)
    
*   Physics: Fixed incorrect use of initial rotation of Rigidbody2D connected via a HingeJoint2D. ([1160213](https://issuetracker.unity3d.com/issues/hingejoint2d-angle-limits-are-not-respected-when-connected-objects-rotation-is-not-0), 1174067)
    
*   Prefabs: Added GameObjects and components with a DontSave flag (specifically DontSaveInEditor) will no longer show up in the Prefab overrides dropdown since they don't get applied or reverted anyway. ([1173465](https://issuetracker.unity3d.com/issues/child-gameobjects-with-hideanddontsave-flag-appear-as-overrides-on-prefab-instances), 1175218)
    
*   Profiler: Fixed crash when profiler runs out of memory budget on Job threads. ([1169456](https://issuetracker.unity3d.com/issues/gfxdevice-onprofilerframechanged-crash), 1172233)
    
*   ps4: Fix camera HDR textures (1161961, 1173670)
    
*   Scripting: ClampBlendShapes are now set to false by default when loading a 3D template. ([1148638](https://issuetracker.unity3d.com/issues/templates-clamp-blendshapes-are-set-to-true-by-default-when-creating-new-projects), 1154002)
    
*   Scripting: Editor: Added missing 2018\_4\_OR\_NEWER C# preprocessor directive when compiling C# scripts ([1169225](https://issuetracker.unity3d.com/issues/2018-4-or-newer-define-is-missing-slash-not-working-slash-broken), 1171407)
    
*   Serialization: Editor: Fixed issue with SerializedProperty.objectReferenceInstanceIDValue emitting asserts to the console ([1169801](https://issuetracker.unity3d.com/issues/serializedproperty-dot-objectreferenceinstanceidvalue-asserts-if-update-has-been-called-for-the-serialized-object), 1171719)
    
*   Shaders: Improved generation of GLSL Tessellation shaders in more situations. (1134172, 1166876)
    
*   Terrain: Brush inspector no longer spams Undo events, preventing Undo from working while it was open. ([1170735](https://issuetracker.unity3d.com/issues/having-the-custom-brush-menu-open-with-custom-brush-texture-set-to-none-breaks-undo-functionality), 1176667)
    
*   Windows: Allow P/Invoke calls where the library extension is included in the library file name in the \[DllImport\] attribute. ([1132730](https://issuetracker.unity3d.com/issues/fallback-p-slash-invoke-dll-resolution-is-broken-on-windows), 1148202)