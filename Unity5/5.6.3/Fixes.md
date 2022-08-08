# Unity 5.6.3

https://unity3d.com/unity/whats-new/unity-5.6.3

## Fixes



*   2D: Fixed an issue where adjusting Collider2D's Offset when Using Tiled Draw Mode and Auto Tiling would result in inconsistent behaviour.
*   (917931)
*   2D: Fixed an issue where the Editor becomes unresponsive when switching from OpenGL to Metal with a tiled sprite in the scene. (918524)
*   Android: Buildpipe - Correctly split resources between APK and OBB when building with LZ4. (920360)
*   Android: Fixed a development build crash on Android 4.2.2 with VideoCore GPU. (922553)
*   Android: Fixed a Vulkan error when trying to use anisotropic filtering on Mali GPUs.
*   Android: Fixed an issue where Android IL2CPP builds might fail if built from an editor script. (921525)
*   Android: Fixed an issue where spot and point lights were too bright on low-end devices. (918785)
*   Android: Fixed an issue whereby H264 videos did not loop on Android 4.1 and 4.2 devices. (893527)
*   Android: Fixed an issue with alpha texture size in ETC1 texture compression with split alpha. (919308)
*   Android: Fixed an issue with enabling Split Application Binary flag in Android player settings would affect other platforms. (918606)
*   Android: Fixed the empty scene startup time regression. (917096)
*   Android: Fixed the NamePhonePad flag. (924516)
*   Android: Gradle - Do not explicitly set debuggable attribute when building with Gradle to avoid lint security warning. (924517)
*   Android: Gradle - Handle too many errors; filter out warnings and detect too long error list.
*   Android: Gradle - Make sure unity3d and other files from raw/ are uncompressed in the APK. (924519)
*   Android: Gradle - Removed debuggable from Manifest when creating APK. (924523)
*   Android: Gradle - Support custom library build.gradle files. (887824)
*   Android: Moved GoogleVR initialisation to run on UI Thread thus fixing startup crash. (922898)
*   Animation: AnimatorState's WriteDefaults is working properly on very specific setups. (893779)
*   Animation: Fixed a crash in Animator Editor window when closing Unity. (918033)
*   Animation: Fixed a crash in PlayableTraverser::RootByType that was triggered when disabling a GameObject by using OnStateMachineExit. (914365)
*   Animation: Fixed an issue where the Animation events would not trigger if animation had less than two frames. (921121)
*   Animation: Fixed an issue with preview of mirrored animations in the inspector. (916581)
*   Animation: Fixed Animator.GetBehaviour() returning null after recompiling a script while in play mode. (913301)
*   Animation: Fixed layer root motion broken on standalone. (925444)
*   API Updater: Fixed a crash when checking C# scripts with deep object initialization syntax. (902973)
*   API Updater: Fixed assembly corruption in assemblies containing references to UnityEditor.Animations.AvatarMask. (904030)
*   API Updater: Fixed nested types updating on local variable / parameter declarations.
*   Asset Bundles: Fixed a crash when loading GuiStyleState from an asset bundle. (909471)
*   Asset Pipeline: Fixed AssetDatabase.GetMainAssetTypeAtPath so that it returns the right type for ScriptableObjects instead of just 'MonoBehaviour'. (904653)
*   Editor: Fixed a transform precision issue when moving multiple objects. (907854)
*   Editor: Fixed an issue whereby moving multiple objects made only one of them to move according to handles.
*   (925765)
*   Editor: Fixed an issue which made deleted files moved to recycling bin on windows. (888995)
*   Editor: Fixed assets being marked for delete instead of opened for edit in Version Control in cases where the asset was deleted and recreated (e.g. re-baking NavMeshes). (895425)
*   Editor: Fixed the case of "Generate Lighting" drop down menu being hidden when inspector was resized to minimal width. (915524)
*   Editor: Restored SRGB write state after internal override. (901588)
*   Editor: Warn, rather than fail, if an external process Unity launches suspended has been unexpectedly resumed by another process. Note: Some versions of RenderDoc have a bug which can cause this. (906745)
*   GI Progressive Lightmapper: Fixed a crash in light probe rendering occurring when changing or removing probes.
*   GI: Fixed an issue where Auto mode overwrites Lightmap indices with wrong values when additively loading scenes. (916893)
*   GI: Fixed case of tiling being ignored by the Progressive Lightmapper.
*   GI: Progressive Lightmapper: Fixed an issue where alpha cutoff was not properly converting values.
*   GI: Progressive Lightmapper: Fixed an issue where auto-mode did not detect when changing material values for alpha cutoff.
*   GI: Progressive Lightmapper: Fixed scene dependent issues with dark edges on charts lying near the lightmap border.
*   Graphics: Added tier settings for Light Probe Proxy Volume. (908093)
*   Graphics: Fix for GetTransformInfoDoNotExpectUpToDate in renderer bounding volume updating (899009)
*   Graphics: Fix for miscalculating the size of the view required for a buffer which will be used as the source for an Indirect Draw/Dispatch call. (919044)
*   Graphics: Fixed a crash in non-native graphics jobs in specific scene configurations eg lots of particles, terrain. (918788)
*   Graphics: Fixed a crash triggered by setting the SkinnedMeshRenderer.updateWhenOffscreen flag to true via a script. (912723)
*   Graphics: Fixed a rare crash/hang which, could happen in very complex scenes, when graphics jobs were enabled. (918788)
*   Graphics: Fixed an assert when calling CommandBuffer.DrawRenderer on disabled mesh renderer (917188)
*   Graphics: Fixed an issue where a ComputeBuffer applied to a Material Block doesn't take effect when drawing via DrawMesh\*Indirect. (913828)
*   Graphics: Fixed an issue where overlapping cameras drawing to the same target would not composite correctly (923842)
*   Graphics: Fixed an occasional glitch when rendering lines/trails. (903807)
*   Graphics: Fixed Assert in Editor and crash in Standalone when disabling/enabling SkinnedMeshRenderer in very specific situations eg from animation during an OnBecameVisible callback. (901468)
*   Graphics: Fixed error message "Enabling or adding a Renderer during rendering; this is not allowed." when creating or enabling a game object during OnPreRender, OnWIllRenderObject, OnBecameVisible, OnBecameInvisible callbacks. (897994, 907626, 901242)
*   Graphics: Fixed metal editor shader warmup. (916950)
*   Graphics: Fixed OpenGL debug labels when using OpenGL ES.
*   Graphics: Fixed rare hang in the Editor when building lighting data. (918993)
*   Graphics: Fixed sRGB flag returning false on the LDR target texture from a HDR to LDR image effect in a linear project. (912603)
*   IL2CPP: Fixed a crash in QueryComponentByType when animation was used with engine code stripping enabled and there was no Sprite Renderer component in any scene in the build. (919058)
*   IL2CPP: Fixed an issue with setting enum type fields in .NET 4x with relfection using an integer value. (923517)
*   IL2CPP: Fixed an issue which caused IL2CPP to fail to convert assemblies if two non-existing methods with the same declaring type were referenced from any assemblies. (917343)
*   iOS: Fixed an issue where iOS screen info was retrieved for every request instead of being cached (894273)
*   iOS: Fixed Application.installMode for apps downloaded from AppStore. (913886)
*   iOS: Fixed auto-rotation on ReplayKit. (911935)
*   iOS: Fixed corrupted orientation view when forcing interface orientation via script (using Screen.orientation) on iOS10. (835745)
*   iOS: Rewrote the internal clock system and replaced it with a system that takes into account the time when the device is asleep. Also, the startup time is now calculated more accurately. (912594)
*   Linux : Associate provided icon with player window. (912675)
*   Linux: Added an additional fix for uninitialized screen dimensions(/mouse input) at startup with some window managers. (880426)
*   Linux: Don't add control characters to Input.inputString (916125)
*   Linux: Use default player icon when none is provided. (912675)
*   Linux: Work around change in glibc TLS allocation behavior in certain distributions.
*   Multiplayer: Added a new overload to NetworkManager.StartClient function which allows to specific which port should the local socket be bound to. (903860)
*   Multiplayer: Fixed an issue whereby reliable messages exchanging had been staled after couple of hours.
*   Multiplayer: Fixed an issue with network transport host being removed with invalid host id, when using custom network connection (NetworkConnection override). (881764)
*   Multiplayer: NetworkTransport.Send() leaks memory. (923903)
*   Navigation: Fix using NavMeshAgent and NavMeshObstacle simultaneously causing Y coordinate to snap to maximum value. (910223)
*   OSX: Added apple File System (APFS) compatibility fix.
*   Particles: Detect when a new mesh is selected in the Shape Module, and update the Scene View preview accordingly. (900928
*   Particles: Ensure trails are properly initialized when particles are being manipulated via script. (899881
*   Particles: Fixed an issue where bounding boxes were too small on some systems, causing culling problems. (914333)
*   Physics 2D: Fixed a crash when a 2D Collider is recreated during contact reevaluation. (920587)
*   Physics: Fix for "PolygonCollider2D.points" reporting "Assertion failed on expression: 'm\_data == NULL'" when setting a new Vector2 array to it. (923135)
*   Physics: Fix for a crash when repeatedly unloading/loading cloth on XBox One and PS4. (909248)
*   Physics: Fix for normals issue with cloth using tiny mesh. (766851)
*   Physics: Fix to avert 'value must be greater' errors in cloth. (895771)
*   Physics: Fix to avert cloth errors with prefabs: in cloth inspector we now check if cloth has no verts disabled and we eprocess mesh if re-enabled and previous cloth mesh had no verts. (893025)
*   Physics: Fixed a case of CharacterController starting to ignore collisions with certain objects after a number of scene reloads. (809914)
*   Physics: Fixed a memory leak issue in UnityWebRequest when Dispose was not called. (862095)
*   Physics: Fixed an error thrown when using a Rigidbody with an Interpolate mode (Interpolate or Extrapolate). (890470, 899631)
*   Scripting: Fixed a crash when invoking LINQ expressions in Editor. (920085)
*   Scripting: Fixed a regression causing ContextMenu attributes from base classes to not be used on derived classes. (860417)
*   Scripting: Fixed an issue where C# compiler incorrectly generating error CS1525 when using ternary operator with floating point values and no whitespace. (871725)
*   Scripting: Fixed end of frame event not being sent in batch mode. (914052)
*   Scripting: Fixed scripting exception being logged as Info instead of Error. (912719)
*   Services: Fixed an issue where Performance Reporting symbol upload tool could crash. (927884)
*   UI: Fix for Event System not updating when the application was not focused on macOS/Linux/UnityRemote/VR. (896933)
*   UI: Fixed a memory leak in UI::DepthSortLayer(). (907581)
*   UI: Fixed a rare Transform::kReceivedDueToParentTRSChanged assertion failure introduced in 5.6.1p1. (917177)
*   UI: Fixed a regression that caused a crash of the Editor when adding a Text component to a GameObject via a script. (886331)
*   UI: For Name content type, use NamePhonePad touch screen keyboard type. (924516)
*   UnityWebRequest: Fix for broken audio clip when download is chunked. (911562)
*   UnityWebRequest: Fixed the issue of absolute redirect URL not escaped. (921259)
*   Video: On Android 4.1/4.2, bigger resolution videos don't play. (908936)
*   Video: On Android, video stops playback if trying to play it faster than 1x. (915772)
*   VR: fix for single pass rendering w/one of the standard effects shaders doesn't render correctly on the right eye. (913882)
*   VR: Fixed an editor crash when user selected VR Camera while playing. (916987)
*   VR: Fixed an issue that was causing eye flickering in Daydream. (915277)
*   VR: Fixed CommandBuffers don't work w/ MSAA and VR. (906203)
*   VR: Fixed Stereo Display (non-head mount) produces only black screen in build. (913547)
*   VR: Fixed Stereo Display Standalone build runs at a low resolution regardless of settings. (890718)
*   VR: Removed an unnecessary blit when single-pass stereo rendering is used on Daydream devices.
*   VR: Updated GoogleVR SDK to 1.60.1 (859281, 911311, 901404)
*   WebGL: Fixed Corrupted Sprites on MS Edge. (904449)
*   Windows: Fixed switching to full screen from windowed when using dx11. (904471)
*   XR: Added missing Editor icons for world anchor, spatial mapping, touch input, and audio spatialization components. (857023)

#### Revision: d3101c3b8468