# Unity 5.5.3
https://unity3d.com/unity/whats-new/unity-5.5.3

## Fixes

<ul>
<li>Animation: Fixed Assert Thread::CurrentThreadIsMainThread() from Animator::IsHuman() when run in a job thread.    (887998)</li>
<li>Analytics: Fix adds Internet permission on Android when Analytics service is used.    (861178)</li>
<li>Android: Acquire context on focus before notifying player.    (837483)</li>
<li>Android: Fixed an issue where ApplicationId was missing from AndroidManifest.xml in Gradle builds.    (888274) </li>
<li>Android: Fixed incorrect dangerous permissions dialog behavior when the app was suspended while the dialog was on screen. (851523) </li>
<li>Android: Fixed proguard template to actually keep Unity classes.  (857978) </li>
<li>Android: Fixed the failure to push OBB to certain Samsung devices.    (853474) </li>
<li>Android: Fixed the splash screen and black bar issues by applying immersive fullscreen mode as early as possible. (868612, 867887, 861069, 874761) </li>
<li>Android: Improved the WebRequest performance.   </li>
<li>Android: Input - Fixed issues with joystick polling and startup.  (863399) </li>
<li>Android: Manifest - Added layoutDirection to configChanges.   (867668) </li>
<li>Android: Opening the on-screen keyboard does not make webcam update slower.   (827454) </li>
<li>Animation : Fixed a race condition in the legacy animation system which could cause a crash if a GameObject and an Animation assigned to that GameObject were deleted in the same frame.  (868587) </li>
<li>Animation: Fixed a crash when re-enabling GameObject that was running a Playable. (884643) </li>
<li>Animation: Fixed an issue with using abstract classes behaviour on a StateMachineBehaviour.   (877623) </li>
<li>Animation: Playback range is now correctly displayed after changing the Samples of a clip.    (884523)</li>
<li>Asset Importer: Fixed the importing process so that asset paths with zero length are skipped. (869307)</li>
<li>Asset Pipeline: Fixed a crash that occurred when loading the same asset both synchronously and asynchronously simultaneously. (884472)</li>
<li>Cache Server: Do not ask to delete the local cache server data twice when switching from local to a different option in preferences   (878326) </li>
<li>Cache Server: The Cache Server preferences dialog now correctly recognises when the mode is changed.  (863299) </li>
<li>Core: Fixed the issue of job system ending up with high CPU usage in certain circumstances eg. using UnityWebRequest.Send() in Editor after exiting Play mode.    (879675) </li>
<li>DX12: Expose the command queue to DX12 plugins now.   (867573)</li>
<li>DX12: Only invoke plugin events from the "rendering" thread, not main thread. (863285)</li>
<li>Editor: Fix for time not updating in Editor if play mode is entered and then exited while paused. (864246) </li>
<li>Editor: Fixed a crash on OSX when the Editor loses context.   (837413) </li>
<li>Editor: Fixed an issue with deselect of single selected item in hierarchy with ctrl/cmd+click.    (864273) </li>
<li>Editor: Fixed an issue with vertex snapping jumping to extreme values in isometric view.  (861345) </li>
<li>Editor: Fixed the issue that Pro users can't skip the survey after Unity activation.  (878112) </li>
<li>EditorAnalytics: Honoring DisableEditorAnalytics settings.     </li>
<li>GameObject: Fixed position inconsistency when using generic instantiate.  (873836) </li>
<li>GI : Fix for lightmaps not being loaded in a standalone player when loading scene through an AssetBundle. (858292) </li>
<li>GI : Fix for lightprobe gizmos being rendered too bright in Linear color space.   (862215)</li>
<li>GI: Fixed a crash while baking lightmaps with custom shaders after Light Transport jobs finished. (856901) </li>
<li>Graphics : Fixed D3D12 cubemap mip generation.      </li>
<li>Graphics: Changes made to blending mode via shader properties are no longer ignored in Graphics.Blit. (865062) </li>
<li>Graphics: D3D9 to make sure that internal resolves don't result in a drawn pixel, i.e. single white pixel when using deferred mode.   (728324) </li>
<li>Graphics: Fixed a crash when switching from DX12 to DX11 graphics API in the Editor.  (851265) </li>
<li>Graphics: Fixed an issue with Assert "Texture aux property (unity_SpecCube0_HDR) should never be a built-in name!".   (864237) </li>
<li>Graphics: Fixed an issue with BC6 decompression and improve reading of textures with more than one byte per channel.  (865491) </li>
<li>Graphics: Fixed the issue of forward-only objects being rendered into Depth/DepthNormals textures multiple times when they have multiple submeshes and deferred shading is used.  (863954) </li>
<li>Graphics: For script created/instanced cameras only add Image Effects Callbacks if the Image Effect is already registered. Fixed the error message when disabling script during instantiate.  (862473) </li>
<li>Graphics: On DirectX avoid presenting a fresh-black frame whilst performing screen resizing.  (849424) </li>
<li>Graphics: Set the ambient probe for the deferred reflections pass to fix a difference between graphics jobs and non-graphics jobs rendering.  (863625) </li>
<li>Graphics: Stop RenderNow/DrawMeshNow crashing when shader had no matching vertex channels.    (876162) </li>
<li>Graphics: When calling Material.SetFloatArray, SetVectorArray, SetMatrixArray throw a NULL exception instead of crashing. (868016) </li>
<li>IL2CPP: Fixed the incorrectly managed stack traces on iOS devices in release mode.    (869696) </li>
<li>iOS, Android: Fixed - Light Probe Proxy Volumes don't fallback to normal probe blending.  (837679) </li>
<li>IOS: Added support in order to enable auto-rotation while broadcasting using ReplayKit.   (887912)</li>
<li>iOS: Fixed Airplay mirroring mode when using Open GLES.   (788515) </li>
<li>iOS: Fixed build errors in XCode when stripping is enabled using Mono scripting backend.  (866194) </li>
<li>IOS: Fixed WebRequest setting the IsError property correctly. (880773)</li>
<li>iOS: Removed extra notification sent on application launch.   (875180) </li>
<li>Kernel: Prevent scripts from adding Transform-derived components during their Awake methods.  (878716)</li>
<li>Mac Editor: Fixed the crashes while exporting projects.   (878783)</li>
<li>Metal: Fixed geometry corruption when dynamic batching was enabled.   (871026)</li>
<li>Metal: Fixed issues with setting DontCare load flag when running multithreaded.     </li>
<li>Mono: Fixed a C# compiler bug which could cause an incorrect compiler error in some cases when overloaded generic methods were used.  (869169)</li>
<li>Mono: Fixed a crash which could occur in the editor when deep profiling was enabled.  (878859) </li>
<li>Mono: Fixed rare issue due to timer collisions.   (881491)</li>
<li>Particles: Fixed a NullReferenceException, when Inherit Velocity was set to less or more than 0 and Rigidbody2D was set to Dynamic.   (876169) </li>
<li>Particles: Fixed an incorrect velocity for first frame when a rigidbody was first enabled.    (881847) </li>
<li>Physics 2D: CapsuleCollider2D now correctly calculates its mass when using auto-mass. (890937) </li>
<li>Physics: Fixed a crash caused by changing the value of the configuredInWorldSpace flag on a Joint attached to an inactive GameObject. (886574)</li>
<li>Scripting: Fixed a coroutine crash in Coroutine::CompareCoroutineEnumerator.  (888302) </li>
<li>Scripting: Fixed MonoBehaviour array field with initializer getting resized to 0 by serialization.    (868935) </li>
<li>Shaders: Fixed a crash in ShaderLab::shaderprops::GetMatrix when using OpenGL API when using specific graphics drivers on Windows.    (859418)</li>
<li>Shaders: Fixed advanced blend operations by requiring the shaders to be decorated with UNITY_REQUIRE_ADVANCED_BLEND(mode) declaration.    (750307)</li>
<li>Shaders: Fixed an internal error on a GLSL/Metal shader compiling corner case.    (881103) </li>
<li>Shaders: Make shader binary blob data deterministic to fix problems with asset bundle (or player data) changing with identical source inputs. (877123) </li>
<li>Shadows: Allow 2k shadowmap textures on devices with less than 2 GB of RAM when best quality shadows are selected (871606) </li>
<li>Sprites: Fixed an issue where OverrideGeometry on instantiated sprites produced differing results in the Editor and Standalone    (863256) </li>
<li>Terrain: Fixed a crash when loading a scene with a terrain and trees and then unloading the previous scene.   (857047) </li>
<li>Terrain: Fixed an issue where the default material could be more specular than expected.  (864935) </li>
<li>Texture Importer: Fixed an issue where a texture's colour model was set to RGBA without an alpha channel. (870830) </li>
<li>Texture Importer: Fixed an issue where BC7 didn't compress alpha textures correctly.  (858502) </li>
<li>Texture Importer: Fixed an issue where setting textureType reset sprite mode to single.   (856584) </li>
<li>Texture Importer: Fixed an issue where some textures were wrongly interpreted as single channel cube maps.    (858460) </li>
<li>Tizen: Fixed a crash that occurred when an app tried to exit.   </li>
<li>UI : Fixed the issue of fonts created at runtime not showing up when added to text.   (858645) </li>
<li>UI: Fixed an occasional masking issue when using deferred rendering path on Linux.    (873678) </li>
<li>UI: Fixed scrollrect performance being slow when it had a lot of content. (856380)</li>
<li>UI: Selection elements will update selection state when interactable is changed.  (861736, 872634)</li>
<li>UnityAds: Fixed callback executor from being destroyed on scene changes.</li>
<li>UnityWebRequest: Fixed high CPU usage/fareeze after aborting (leaving play mode) UWR with custom download handler script.     (876027, 880565)</li>
<li>UnityWebRequest: URLs without '%' character will be escaped and the ones with '%' will be assumed to be properly escaped. (876823) </li>
<li>VCS: Fix for editor not checking out scene file before first write in freshly loaded project. (850239) </li>
<li>VCS: Fixed an issue trying to add files from ProjectSettings folder to Version Control even if they were already under Version Control.     </li>
<li>VR: Fixed a subtle timing bug on Rift that could cause very minor view stuttering in certain situations.  (886841) </li>
<li>VR: Updated Oculus to version 1.12. This fixed a GearVR timeout issue.     </li>
<li>WebGL: Fixed "incorrect header check" builtin web server error when build folder contained non-URI characters.    (855985) </li>
<li>WebGL: Fixed buffer overflow that occurred when using UnityWebRequest and custom DownloadHandlerScript.   (865630) </li>
<li>WebGL: Fixed memory corruption when generating terrain base map textures. (868756) </li>
<li>Windows Store: Fixed the issue whereby secure connections were not working when using UnityWebRequest.    (874571)</li>
<li>Windows Store: Fixed the known issue reported in the previous release, 5.5.2 - player prefs might get corrupted on Windows 8.1 and Windows Phone 8.1 SDKs when forcefully closing the application right after saving them.      </li>
<li>Windows: Fixed the logging code in the Windows Editor/Standalone player so that messages got printed at once instead of one byte at the time. (886630)</li>
</ul>
