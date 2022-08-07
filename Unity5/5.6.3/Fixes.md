# Unity 5.6.3
https://unity3d.com/unity/whats-new/unity-5.6.3

## Fixes

<ul>
<li>2D: Fixed an issue where adjusting Collider2D's Offset when Using Tiled Draw Mode and Auto Tiling would result in inconsistent behaviour.   </li>
<li>(917931) </li>
<li>2D: Fixed an issue where the Editor becomes unresponsive when switching from OpenGL to Metal with a tiled sprite in the scene.       (918524)</li>
<li>Android: Buildpipe - Correctly split resources between APK and OBB when building with LZ4.       (920360)</li>
<li>Android: Fixed a development build crash on Android 4.2.2 with VideoCore GPU.        (922553)</li>
<li>Android: Fixed a Vulkan error when trying to use anisotropic filtering on Mali GPUs.    </li>
<li>Android: Fixed an issue where Android IL2CPP builds might fail if built from an editor script.       (921525)</li>
<li>Android: Fixed an issue where spot and point lights were too bright on low-end devices.      (918785)</li>
<li>Android: Fixed an issue whereby H264 videos did not loop on Android 4.1 and 4.2 devices.         (893527)</li>
<li>Android: Fixed an issue with alpha texture size in ETC1 texture compression with split alpha.       (919308)</li>
<li>Android: Fixed an issue with enabling Split Application Binary flag in Android player settings would affect other platforms.        (918606)</li>
<li>Android: Fixed the empty scene startup time regression.         (917096)</li>
<li>Android: Fixed the NamePhonePad flag.       (924516)</li>
<li>Android: Gradle - Do not explicitly set debuggable attribute when building with Gradle to avoid lint security warning.      (924517)</li>
<li>Android: Gradle - Handle too many errors; filter out warnings and detect too long error list.    </li>
<li>Android: Gradle - Make sure unity3d and other files from raw/ are uncompressed in the APK. (924519)</li>
<li>Android: Gradle - Removed debuggable from Manifest when creating APK.       (924523)</li>
<li>Android: Gradle - Support custom library build.gradle files.        (887824)</li>
<li>Android: Moved GoogleVR initialisation to run on UI Thread thus fixing startup crash.       (922898)</li>
<li>Animation: AnimatorState's WriteDefaults is working properly on very specific setups.       (893779)</li>
<li>Animation: Fixed a crash in Animator Editor window when closing Unity.      (918033)</li>
<li>Animation: Fixed a crash in PlayableTraverser::RootByType that was triggered when disabling a GameObject by using OnStateMachineExit.       (914365)</li>
<li>Animation: Fixed an issue where the Animation events would not trigger if animation had less than two frames.       (921121)</li>
<li>Animation: Fixed an issue with preview of mirrored animations in the inspector.         (916581)</li>
<li>Animation: Fixed Animator.GetBehaviour() returning null after recompiling a script while in play mode.      (913301)</li>
<li>Animation: Fixed layer root motion broken on standalone.        (925444)</li>
<li>API Updater: Fixed a crash when checking C# scripts with deep object initialization syntax.         (902973)</li>
<li>API Updater: Fixed assembly corruption in assemblies containing references to UnityEditor.Animations.AvatarMask.        (904030)</li>
<li>API Updater: Fixed nested types updating on local variable / parameter declarations.     </li>
<li>Asset Bundles: Fixed a crash when loading GuiStyleState from an asset bundle.       (909471)</li>
<li>Asset Pipeline: Fixed AssetDatabase.GetMainAssetTypeAtPath so that it returns the right type for ScriptableObjects instead of just 'MonoBehaviour'.         (904653)</li>
<li>Editor: Fixed a transform precision issue when moving multiple objects.         (907854)</li>
<li>Editor: Fixed an issue whereby moving multiple objects made only one of them to move according to handles. </li>
<li>(925765) </li>
<li>Editor: Fixed an issue which made deleted files moved to recycling bin on windows.      (888995)</li>
<li>Editor: Fixed assets being marked for delete instead of opened for edit in Version Control in cases where the asset was deleted and recreated (e.g. re-baking NavMeshes).       (895425)</li>
<li>Editor: Fixed the case of "Generate Lighting" drop down menu being hidden when inspector was resized to minimal width.      (915524)</li>
<li>Editor: Restored SRGB write state after internal override.      (901588)</li>
<li>Editor: Warn, rather than fail, if an external process Unity launches suspended has been unexpectedly resumed by another process. Note: Some versions of RenderDoc have a bug which can cause this.         (906745)</li>
<li>GI Progressive Lightmapper: Fixed a crash in light probe rendering occurring when changing or removing probes.   </li>
<li>GI: Fixed an issue where Auto mode overwrites Lightmap indices with wrong values when additively loading scenes.        (916893)</li>
<li>GI: Fixed case of tiling being ignored by the Progressive Lightmapper.   </li>
<li>GI: Progressive Lightmapper: Fixed an issue where alpha cutoff was not properly converting values.   </li>
<li>GI: Progressive Lightmapper: Fixed an issue where auto-mode did not detect when changing material values for alpha cutoff.   </li>
<li>GI: Progressive Lightmapper: Fixed scene dependent issues with dark edges on charts lying near the lightmap border.      </li>
<li>Graphics: Added tier settings for Light Probe Proxy Volume.         (908093)</li>
<li>Graphics: Fix for GetTransformInfoDoNotExpectUpToDate in renderer bounding volume updating      (899009)</li>
<li>Graphics: Fix for miscalculating the size of the view required for a buffer which will be used as the source for an Indirect Draw/Dispatch call.        (919044)</li>
<li>Graphics: Fixed a crash in non-native graphics jobs in specific scene configurations eg lots of particles, terrain.         (918788)</li>
<li>Graphics: Fixed a crash triggered by setting the SkinnedMeshRenderer.updateWhenOffscreen flag to true via a script.         (912723)</li>
<li>Graphics: Fixed a rare crash/hang which, could happen in very complex scenes, when graphics jobs were enabled.      (918788)</li>
<li>Graphics: Fixed an assert when calling CommandBuffer.DrawRenderer on disabled mesh renderer         (917188)</li>
<li>Graphics: Fixed an issue where a ComputeBuffer applied to a Material Block doesn't take effect when drawing via DrawMesh*Indirect.      (913828)</li>
<li>Graphics: Fixed an issue where overlapping cameras drawing to the same target would not composite correctly         (923842)</li>
<li>Graphics: Fixed an occasional glitch when rendering lines/trails.       (903807)</li>
<li>Graphics: Fixed Assert in Editor and crash in Standalone when disabling/enabling SkinnedMeshRenderer in very specific situations eg from animation during an OnBecameVisible callback.      (901468)</li>
<li>Graphics: Fixed error message "Enabling or adding a Renderer during rendering; this is not allowed." when creating or enabling a game object during OnPreRender, OnWIllRenderObject, OnBecameVisible, OnBecameInvisible callbacks. (897994, 907626, 901242) </li>
<li>Graphics: Fixed metal editor shader warmup.         (916950)</li>
<li>Graphics: Fixed OpenGL debug labels when using OpenGL ES.    </li>
<li>Graphics: Fixed rare hang in the Editor when building lighting data.        (918993)</li>
<li>Graphics: Fixed sRGB flag returning false on the LDR target texture from a HDR to LDR image effect in a linear project.         (912603)</li>
<li>IL2CPP: Fixed a crash in QueryComponentByType when animation was used with engine code stripping enabled and there was no Sprite Renderer component in any scene in the build.      (919058)</li>
<li>IL2CPP: Fixed an issue with setting enum type fields in .NET 4x with relfection using an integer value.         (923517)</li>
<li>IL2CPP: Fixed an issue which caused IL2CPP to fail to convert assemblies if two non-existing methods with the same declaring type were referenced from any assemblies.      (917343)</li>
<li>iOS: Fixed an issue where iOS screen info was retrieved for every request instead of being cached       (894273)</li>
<li>iOS: Fixed Application.installMode for apps downloaded from AppStore.       (913886)</li>
<li>iOS: Fixed auto-rotation on ReplayKit.      (911935)</li>
<li>iOS: Fixed corrupted orientation view when forcing interface orientation via script (using Screen.orientation) on iOS10.        (835745)</li>
<li>iOS: Rewrote the internal clock system and replaced it with a system that takes into account the time when the device is asleep. Also, the startup time is now calculated more accurately.      (912594)</li>
<li>Linux : Associate provided icon with player window.         (912675)</li>
<li>Linux: Added an additional fix for uninitialized screen dimensions(/mouse input) at startup with some window managers.      (880426)</li>
<li>Linux: Don't add control characters to Input.inputString        (916125)</li>
<li>Linux: Use default player icon when none is provided.       (912675)</li>
<li>Linux: Work around change in glibc TLS allocation behavior in certain distributions.     </li>
<li>Multiplayer: Added a new overload to NetworkManager.StartClient function which allows to specific which port should the local socket be bound to.       (903860)</li>
<li>Multiplayer: Fixed an issue whereby reliable messages exchanging had been staled after couple of hours.      </li>
<li>Multiplayer: Fixed an issue with network transport host being removed with invalid host id, when using custom network connection (NetworkConnection override).      (881764)</li>
<li>Multiplayer: NetworkTransport.Send() leaks memory.      (923903)</li>
<li>Navigation: Fix using NavMeshAgent and NavMeshObstacle simultaneously causing Y coordinate to snap to maximum value.        (910223)</li>
<li>OSX: Added apple File System (APFS) compatibility fix.  </li>
<li>Particles: Detect when a new mesh is selected in the Shape Module, and update the Scene View preview accordingly.       (900928</li>
<li>Particles: Ensure trails are properly initialized when particles are being manipulated via script.      (899881</li>
<li>Particles: Fixed an issue where bounding boxes were too small on some systems, causing culling problems.        (914333)</li>
<li>Physics 2D: Fixed a crash when a 2D Collider is recreated during contact reevaluation.      (920587)</li>
<li>Physics: Fix for "PolygonCollider2D.points" reporting "Assertion failed on expression: 'm_data == NULL'" when setting a new Vector2 array to it.        (923135)</li>
<li>Physics: Fix for a crash when repeatedly unloading/loading cloth on XBox One and PS4.       (909248)</li>
<li>Physics: Fix for normals issue with cloth using tiny mesh.      (766851)</li>
<li>Physics: Fix to avert 'value must be greater' errors in cloth.      (895771)</li>
<li>Physics: Fix to avert cloth errors with prefabs: in cloth inspector we now check if cloth has no verts disabled and we eprocess mesh if re-enabled and previous cloth mesh had no verts.        (893025)</li>
<li>Physics: Fixed a case of CharacterController starting to ignore collisions with certain objects after a number of scene reloads.        (809914)</li>
<li>Physics: Fixed a memory leak issue in UnityWebRequest when Dispose was not called.      (862095)</li>
<li>Physics: Fixed an error thrown when using a Rigidbody with an Interpolate mode (Interpolate or Extrapolate).   (890470, 899631) </li>
<li>Scripting: Fixed a crash when invoking LINQ expressions in Editor.      (920085)</li>
<li>Scripting: Fixed a regression causing ContextMenu attributes from base classes to not be used on derived classes.       (860417)</li>
<li>Scripting: Fixed an issue where C# compiler incorrectly generating error CS1525 when using ternary operator with floating point values and no whitespace.       (871725)</li>
<li>Scripting: Fixed end of frame event not being sent in batch mode.       (914052)</li>
<li>Scripting: Fixed scripting exception being logged as Info instead of Error.         (912719)</li>
<li>Services: Fixed an issue where Performance Reporting symbol upload tool could crash.        (927884)</li>
<li>UI: Fix for Event System not updating when the application was not focused on macOS/Linux/UnityRemote/VR.       (896933)</li>
<li>UI: Fixed a memory leak in UI::DepthSortLayer().       (907581)</li>
<li>UI: Fixed a rare Transform::kReceivedDueToParentTRSChanged assertion failure introduced in 5.6.1p1.        (917177)</li>
<li>UI: Fixed a regression that caused a crash of the Editor when adding a Text component to a GameObject via a script.        (886331)</li>
<li>UI: For Name content type, use NamePhonePad touch screen keyboard type.        (924516)</li>
<li>UnityWebRequest: Fix for broken audio clip when download is chunked.       (911562)</li>
<li>UnityWebRequest: Fixed the issue of absolute redirect URL not escaped.         (921259)</li>
<li>Video: On Android 4.1/4.2, bigger resolution videos don't play.        (908936)</li>
<li>Video: On Android, video stops playback if trying to play it faster than 1x.       (915772)</li>
<li>VR: fix for single pass rendering w/one of the standard effects shaders doesn't render correctly on the right eye.         (913882)</li>
<li>VR: Fixed an editor crash when user selected VR Camera while playing.      (916987)</li>
<li>VR: Fixed an issue that was causing eye flickering in Daydream.        (915277)</li>
<li>VR: Fixed CommandBuffers don't work w/ MSAA and VR.        (906203)</li>
<li>VR: Fixed Stereo Display (non-head mount) produces only black screen in build.         (913547)</li>
<li>VR: Fixed Stereo Display Standalone build runs at a low resolution regardless of settings.         (890718)</li>
<li>VR: Removed an unnecessary blit when single-pass stereo rendering is used on Daydream devices.</li>
<li>VR: Updated GoogleVR SDK to 1.60.1    (859281, 911311, 901404) </li>
<li>WebGL: Fixed Corrupted Sprites on MS Edge.         (904449)</li>
<li>Windows: Fixed switching to full screen from windowed when using dx11.         (904471)</li>
<li>XR: Added missing Editor icons for world anchor, spatial mapping, touch input, and audio spatialization components.        (857023)</li>
</ul>

#### Revision: d3101c3b8468
