# Unity 2017.4.0f1
https://unity3d.com/unity/whats-new/unity-2017.4.0

## Fixes

<ul>
<li>2D: Fixed an issue that was causing the Physics Shape of a Sprite2D to not being properly set unless the 'Edit Physics Shape' tab was opened first.  (990691)</li>
<li>2D: Fixed a crash after building and loading an Asset Bundle with Tilemap in the Editor. (976411) </li>
<li>2D: Fixed a crash when Tilemap is loaded with invalid Tiles in the Editor.   (972214) </li>
<li>2D: Fixed an error message "A script behaviour has a different serialization layout when loading" when a Tilemap was loaded in players with code stripping.  (969827) </li>
<li>2D: Fixed Physics2D.TilemapCollider.TileUpdate taking an extremely long time to update every time a script recompile happens.    (966605) </li>
<li>2D: Fixed Tilemap not setting Tiles with the correct data in players with code stripping.    (965608) </li>
<li>Android: Fixed a bug causing the loading of native audio plugins to fail on Android. (992023)</li>
<li>Android: Fixed an issue where the full-screen movie player didn't autorotate.    (962450) </li>
<li>Android: Fixed animation not played when screen sharing is enabled.  (995841, 958223) </li>
<li>Android: Fixed a crash when a compute shader is being used that did not compile/link on a device.      </li>
<li>Android: Fixed gyroscope lag issues that happen on some android devices. (912848) </li>
<li>Android: Fixed an issues when trying to use jobified rendering on certain graphics devices like GLES.    (985591) </li>
<li>Android: Fixed a problem when there is no valid EGL context when running the player loop.    (952769) </li>
<li>Android: Fixed Skybox distortion on specific Android devices with Vivante GC1000/GC2000 GPU. (967646)(903140) </li>
<li>Animation: Fixed a crash caused by invoking QueryComponentByType() when code stripping is enabled.   (962745) (938640) </li>
<li>Animation: Fixed an issue where AnimatorOverrideController.ApplyOverrides was executing unnecessary operations, causing performance issues.  (996351) </li>
<li>Animation: Fixed Animator Layer not deselected when clicking on the graph part of the UI.    (996153) </li>
<li>Animation: Fixed Animator.GetBehaviours returning an empty array after saving scene. (975824) (966082) </li>
<li>Animation: Fixed a crash when calling Animator.MatchTarget without a controller. (975555)</li>
<li>Animation: Fixed a crash when importing animator controller with null transitions.   (986004)</li>
<li>Animation: Fixed editor crashing on WalkTypeTree after removing any component while in Animation record mode.    (978930) </li>
<li>Animation: Fixed state deselection in the Animator State Machine.    (950805)</li>
<li>Animation: Fixed Timeline Sequence not firing Animation Events.  (947918) </li>
<li>Asset Bundles: Fixed a crash when loading meshes from asset bundles that contain both compressed and uncompressed meshes.    (984070) </li>
<li>Asset Bundles: Fixed packing AudioMixerController, AudioMixerGroup and AudioMixerSnapshot into bundles with disabled type trees. (976768) </li>
<li>Asset Import: Fixed AssetPostprocessor.OnAssignMaterialModel not being called for all models when importing materials as sub-assets. (983321) </li>
<li>Asset Import: Fixed a crash when importing fbx .meta files that contain references to non-existing scripts or when scripts ID was too large. (999833, 990267) </li>
<li>Asset Importing: Fixed an issue with MonoScripts for StateMachineBehaviour derived classes not being extracted from managed plugins. (963958) </li>
<li>Audio: Fixed a bug where AudioManager::Update was generating a small amount of garbage memory, if a spatializer was selected, that would later need to get garbage-collected.    (991111)</li>
<li>Cache Server: Fixed an issue where using a Cache Server and reimporting Assembly Definition files would fail to trigger rebuilding of the assembly.  (975773) </li>
<li>Cloud: Fixed exception when building in Cloud Build with Performance Reporting enabled.  (996950)</li>
<li>Editor: Fixed a Windows-specific crash in YAMLMerge when trying to merge files.  (1001450)</li>
<li>Editor: Fixed early flipping of login page in Mac by increasing the timeout. (980070) </li>
<li>Editor: Fixed an editor crash when renaming GameObject with long name on Windows.    (991619) </li>
<li>Editor: Fixed an Editor hang when merging large changesets or large scene files with Collaborate.    (971434) </li>
<li>Editor: Fixed Editor window, Panel and all related managed object leaking.   (996204, 988580) </li>
<li>Editor: Fixed issue with "Rider 2017.2.1.app" not being recognized as Rider code editor. Now recognizes "Rider*.app".      </li>
<li>Editor: Fixed an issue with only assemblies whose name start with "Assembly" being debuggable on IL2CPP platforms.     </li>
<li>Editor: Fixed an issue with UWP build failing when using .asmdef assemblies. (979704) </li>
<li>Editor: Fixed Skinned Mesh not being removed on undo.    (925835) </li>
<li>Editor: Fixed YAMLMerge performance issue when merging large files.  (1001461)</li>
<li>Fixed uninstalling Unity leaving sketchupapi.dll behind. (994283) </li>
<li>GI: Fixed the intensity of baked and real-time emissive materials in Enlighten.  (986160)</li>
<li>Graphics: Fixed OpenGL ES crash due to problem with cached VertexAttribArray.    (989484)</li>
<li>IL2CPP: Added Windows runtime storage extensions.    (992138) </li>
<li>IL2CPP: Corrected a possible build failure with IL2CPP when an attribute constructor has two arguments of type object.   (993422) </li>
<li>IL2CPP: Enabled dead code stripping for clang toolchain. (976218) </li>
<li>IL2CPP: Fixed a crash in Unity Linker (System.InvalidProgramException: Failed to resolve  [UnityEngine]System.Resources.NeutralResourcesLanguageAttribute) when using a managed - DLL that has a non-existing attribute on it.   (969958) </li>
<li>IL2CPP: Fixed a hang on iOS devices when a socket operation is in progress and the app is put into the background with the new scripting runtime.    (989536) </li>
<li>IL2CPP: Fixed a problem with the decimal to double conversion implementation with the new scripting runtime. (959791) </li>
<li>IL2CPP: Fixed an unlikely, but possible crash when default parameter values are used.    (973052) </li>
<li>IL2CPP: Fixed incorrect code generation for nullable types when they are passed to a virtual function.   (995663) </li>
<li>IL2CPP: Implemented sending of email via SmtpClient with .NET 4.6.   (947208) </li>
<li>IL2CPP: Implemented the EnsureSufficientExecutionStack method for .NET 4.6.  (976623) </li>
<li>IL2CPP: Improved the performance of code conversion when many nested generic types are used. (975496) </li>
<li>IL2CPP: Improvedthe startup performance of Unity players built with IL2CPP.  (989476) </li>
<li>iOS: Fixed a problem preventing a user from being prompted to log into GameCenter.   (1000658) </li>
<li>iOS: Fixed Display.SetResolution to work during first frame. (1003875, 995079) </li>
<li>iOS: Fixed UnityWebRequest instability when starting and aborting a lot of requests. (995992, 944301) </li>
<li>iOS: Metal: Fixed MSAA behavior when using RenderPass.     </li>
<li>iOS: Metal: Fixed ReadPixels() crash when reading out of active textures bounds. (990595, 981074) </li>
<li>Linux: Fixed a crash on player startup in GfxDeviceVKBase::GrabIntoRenderTexture.    (1002211)</li>
<li>Metal: Fixed an edge case crash when using grab-pass on metal.   (973813) </li>
<li>OSX: Fixed a crash on Editor panel close on select versions of macOS.    (982435) </li>
<li>OSX: Fixed a crash on Editor panel close on select versions of macOS.    (982435) </li>
<li>OSX: Fixed an editor crash on certain hotkeys and menu selections during project import. (988776) </li>
<li>Package Manager: Fixed a project being stored on OneDrive resulting in a Package Manager error and preventing a project from being opened.   (841172)</li>
<li>Package Manager: Fixed building as local system user failing on Windows. (960093) </li>
<li>Particles: Fixed flickering due to a floating point error when sorting by youngest/oldest.   (988874) </li>
<li>Physics: Ensured that "Collider2D.Distance" with very small distances produces a valid normal.   (969960) </li>
<li>Physics: Fixed Assert message being displayed when reparenting a Collider2D component that is using a CompositeCollider2D.   (977687) </li>
<li>Physics: Fixed crash during simulation after destroying Rigidbody2D that has a child Kinematic Rigidbody2D.  (989323) </li>
<li>Physics: Fixed disabling and enabling a collider on an inactive gameobject producing transform error messages.   (977568, 968882) </li>
<li>Physics: Fixed double full stop added to the dropdown boxes in the physics settings. (998183, 958814) </li>
<li>Physics: Fixed issue where MeshCollider is added to prefab in Hierarchy when selected from the project folder.   (998186, 960479) </li>
<li>Physics: Fixed PhysX crash when calling Physics.OverlapBoxNonAlloc on Android devices.   (878407) </li>
<li>Physics: Increased the accuracy of rotating a tile clockwise/anti-clockwise by 90-degrees when tilemap painting. This ensures that TilemapCollider2D can be accurately composited using the CompositeCollider2D. (974119) </li>
<li>Profiler: Fixed EndThreadProfiler crashing Unity when called from main thread.   (980553) </li>
<li>PS4: Fixed a crash when calling DateTime.Now whilst using il2cpp.    (996508)</li>
<li>PS4: Fixed a native rendering plugin GetContext() not returning correct value.   (991969)</li>
<li>Scene Management: Fixed BuildPipelineInterfaces.InitializeBuildCallbacks() being called on every scene load when loading the same scenes multiple times. (978564) </li>
<li>Scripting Upgrade: Fixed a C# compiler bug which could result in "the type cannot be used as type parameter `T' in the generic type or method" errors.   (991464) </li>
<li>Scripting Upgrade: Fixed a crash on exit when script debugger is enabled.    (974228)</li>
<li>Scripting Upgrade: Fixed a crash when using named pipes. (942966) </li>
<li>Scripting Upgrade: Fixed EntryPointNotFoundException when calling HTTPClient.GetAsync on Android.    (935292) </li>
<li>Scripting: Fixed a crash when using named pipes. (929984) </li>
<li>Scripting: Fixed a crash when using unsafe code in an assembly built with VS2017.    (990559) </li>
<li>Scripting: Fixed an incorrect value when using Math.Round with MidpointRounding.AwayFromZero.    (993302) </li>
<li>Scripting: Fixed memory snapshot errors related to invalid GCHandle values.  (977003) </li>
<li>Scripting: Fixed memory snapshot naming for nested types.    (974042) </li>
<li>Scripting: Fixed memory snapshot naming for types without a namespace.   (974031) </li>
<li>Scripting: Fixed regression with Assembly-CSharp.dll and friends referencing editor only assemblies. (982271) </li>
<li>Services: Performance Reporting: Report device model field for Managed Exceptions.   (980815, 980816) </li>
<li>Shaders: Fixed bad swizzles on GLSL &amp; Metal shader image size queries.   (938614) </li>
<li>Timeline: Fixed ArgumentOutOfRangeException when shift-selecting a clip, if that clip was moved and the move operation was undo. (986871)</li>
<li>Timeline: Fixed group tracks being saved under the wrong asset when copied to a different Timeline.  (991434) </li>
<li>Timeline: Fixed object binding when inline curves are opened.    (998182)</li>
<li>Timeline: Fixed Playing a Timeline causing GC allocations when using the 4.6 Scripting Runtime.  (998642)</li>
<li>UI: Fixed an issue where undoing the activation of a UI layout component did not undo the side effects to the children RectTransforms.   (990752)</li>
<li>UI: Fixed AspectRatioFitter not driving the RectTransform on the first frame.    (999338)(988706) </li>
<li>UI: Fixed crash in RectTransform::ShouldUpdateTransformBefore.   (986584) </li>
<li>UI: Fixed entering playmode with profiler open and UI in the scene crashes in UI::Canvas::CaptureBatchFrame. (984325) (966106) </li>
<li>UI: Fixed instances where Font.textureRebuilt would not be called even though the internal texture was regenerated.  (988311) (939853) </li>
<li>UI: Fixed issue where a driven RectTransform could cause a scene to be constantly flagged as dirty.  (988136) (966172) </li>
<li>UI: Fixed issue where position and rotation specified when calling Object.Instantiate was not applied properly to a RectTransform.   (992286, 980300)</li>
<li>UI: Fixed issue with UI and prefab positioning.  (977959) </li>
<li>UI: Fixed OnEndDrag not being called when dragging as the app loses focus.   (995452, 937370) </li>
<li>UI: iOS Fixed incorrect processing of touch canceled events. (973437) </li>
<li>UWP: Fixed .NET native compiler crash when using List or List in a serializable class.   (979741) </li>
<li>UWP: Fixed Application.isMobilePlatform results to be consistent with SystemInfo.deviceType. Also update API docs for these APIs.    (991466) </li>
<li>UWP: Fixed reference rewriter not fixing references for System.Net.Sockets.Socket when DLL where it's being referenced was compiled against .NET 3.5.    (947209) </li>
<li>UWP: Fixed keyboard input not distinguishing left/right shift keys.  (968801) </li>
<li>VR: Fixing crash involving VR Mock Device when using TrackedPoseDriver.  (966990) </li>
<li>Web: Fixed file URI with host component in UnityWebRequest.  (991606, 971557) </li>
<li>Web: Fixed handling special URIs in UnityWebRequest with colon in them, like blob:http.  (995845, 992221) </li>
<li>Web: Fixed native UnityWebRequest not destroyed until garbage collected even if explicitly disposed. (988818)</li>
<li>WebGL: Added handling of playBuffer exception when there is no audio output on Safari.   (994912, 960863) </li>
<li>Windows: Fixed an assert when stopping and then immediately destroying DictationRecognizer.  (986045)</li>
<li>Windows: Fixed a crash on startup in case screen width/height player prefs in registry got corrupted.    (979198) </li>
<li>Windows: Fixed default width/height not honored for 'Windowed' mode. (968584) </li>
<li>Windows: Player executable is once again large address aware.    (990939) </li>
<li>XR: Fixed a crash that would occur if an application used Unity's Spatial Mapping component without VR being enabled or without using Windows Mixed Reality. (973172)</li>
<li>XR: Fixed an issue with lights failing to completely illuminate scene geometry during stereo rendering.  (965494) </li>
<li>XR: Fixed build crashes when using stereo display.   (987306)</li>
<li>XR: Fixed calling touch keyboard causing unhandled exception to be thrown and app closing.   (993425)</li>
<li>XR: Fixed calling XRSettings.LoadDeviceByName on an already loaded device causing issues.    (998801)</li>
<li>XR: Fixed a crash when connecting simulator device while running in editor.  (998862, 980089)</li>
<li>XR: Fixed a crash when holographic emulation set to remote with no device connected. (952777) </li>
<li>XR: Fixed the documentation around XRSettings.LoadDeviceByName and add a warning message when we detect that a user is trying to reload an already loaded VR Device. (998801)</li>
<li>XR: Fixed errors when building for Daydream and Cardboard with Proguard enabled. (991170, 946104) </li>
<li>XR: Fixed frame rate throttling when Windows MR device loses tracking.   (994652)</li>
<li>XR: Fixed losing focus causing the thread to sleep causing fps to drop.  (994652)</li>
<li>XR: Fixed stabilization plane not getting set correctly via the SetFocusPointForFrame() API, resulting in poor hologram stabilization and color separation on HoloLens.  (993880)</li>
<li>XR: Ported missing properties on the Pose type, which broke user code for Windows Mixed Reality when porting from 2017.2.    (988571)</li>
</ul>

#### Revision: b5bd171ee9ba
