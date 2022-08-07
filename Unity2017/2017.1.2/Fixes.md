# Unity 2017.1.2
https://unity3d.com/unity/whats-new/unity-2017.1.2

## Fixes

<ul>
<li>2D : Correctly use Sprite Atlas packed offset when calculating UVs for OverrideGeometry().   (941884)</li>
<li>2D : Editing 2D primitive asset no longer show error in console. (937147, 946596, 937126, 946595) </li>
<li>2D : Expose sRGB (gamma color space) option and packing padding option to Sprite Atlas inspector.    (941882)</li>
<li>AI : UpdateNavMeshData will process non read/write meshes in editor when not in playmode.    (935105)</li>
<li>Android : Resources.Load no longer stalls LoadScene and LoadSceneAsync.  (918875)</li>
<li>Android: Buildpipe - Fixed permissions popping up when providing resources in res/ . (940999, 939414) </li>
<li>Android: Fixed a shader compile error on devices not supporting GL_FRAGMENT_PRECISION_HIGH.  (945953) </li>
<li>Android: Fixed black screen on startup on Android O devices. (946059, 945338) </li>
<li>Android: Permissions - Fixed ephemeral permissions not popping up on Android Oreo.   (946377, 946349) </li>
<li>Android: Removed API 16 - 19 from target sdk version selection list. (944010, 898416) </li>
<li>Android: SoftInput - Fixed the Korean input on Samsung phones.   (946429, 945994) </li>
<li>Animation : Fix for events not being fired during CrossFade at 0F.   (920126)</li>
<li>Animation : Fixed a case where sprite and material reference were not animatable at the same time in the SpriteRenderer. (945292)</li>
<li>Animation : Fixed a case where transition between animations made GetIKRotation and GetIKPosition return an incorrect value. (945035)</li>
<li>Animation : Fixed alpha channel being animated when in linear color mode.    (935087)</li>
<li>Animation: Fixed a crash when spawning an Animator with a state machine that uses OnStateMachineEnter.   (930814)</li>
<li>Animation: Fixed animation events firing twice when using Animator manual update.    (938978)</li>
<li>Animation: Fixed root motion not correctly aligning avatar on WebGL. (934626)</li>
<li>Build pipeline : Fixed a regression where the working directory of a Standalone build would default to the Assets folder, which was not allowed. (934848)</li>
<li>Build pipeline : Fixed the behaviour of the build process so that all the scripts got recompiled if the build process failed.    (921652, 941913) </li>
<li>Collab: Fixed an issue where renamed files with new changes were not being pushed to the server and were ignored when comparing client/server states.    (916233)</li>
<li>Editor : Don't give fatal error on plugin importer query for nonexistent platform.</li>
<li>Editor : Fixed ""TLS Allocator ALLOC_TEMP_THREAD, underlying allocator ALLOC_TEMP_THREAD had unfreed allocations" while calling PluginImporter.SetPlatformData.  (925589)</li>
<li>Editor : Fixed an issue where Launcher did not allow user to login and do re-activate when license was invalid.  (942743)</li>
<li>Editor : Fixed the Callback registration failed kMaxCallback&nbsp;crash when entering playmode.   (873467)</li>
<li>Editor : Fixed a crash when building splash with a portrait background but no landscape background was assigned. (913251)</li>
<li>Editor : Fixed modifiers being discarded when pressing hotkey.   (936062, 942636) </li>
<li>Editor : Fixed prefab preview displaying all game objects in each individual game object preview during multi-selection. (941177)</li>
<li>Editor : Fixed sprite preview generation.    (943905)</li>
<li>Editor : Plugins will be correctly excluded from player build, when using combination Any Platform = true with specific platforms excluded.  (941182)</li>
<li>Editor: The crash on macOS when canceling undock of Hierarchy or Scene View has been fixed.  (942253)</li>
<li>Editor: Fixed an issue where LogAssert.Expect would ignore the the logtype when finding a satisfying event when running playmode and editmode tests. (935602, 944933) </li>
<li>Editor: Fixed an issue where OnHierarchyChange()&nbsp;and EditorApplication.hierarchyWindowChanged events were not sent when selecting gameobjects with previews and when adding gameobjects to a scene if they had the HideInHierarchy flag. (946016, 935289) </li>
<li>Editor: Fixed incorrect lighting when switching to Metal device if Editor was started in OpenGL. </li>
<li>Editor: The generated TestResults.xml when running playmode and editmode tests is now updated to be in NUnit3 format.    (910845, 940838) </li>
<li>GI : Fixed a case of object lighting preview being empty for meshes with no normals. (726487)</li>
<li>GI : Fixed an issue where creating a new scene in project window affected the lighting settings of other scenes. (919234)</li>
<li>GI : Fixed shadowmask in Forward rendering when multiple directional lights are used.    (925579)</li>
<li>GI: Added A-Trous filter for the Progressive Lightmapper.</li>
<li>Graphics : Changing worldPos in gles2 to be fp32.    (899729, 925179) </li>
<li>Graphics : Fixed a rare crash when dynamic batching was enabled. (938089, 944773) </li>
<li>Graphics : Fixed occlusion culling of shadows within the camera sightline.   (829193)</li>
<li>Graphics : Fixed the case of Light Cookie rendering differently in Forward and Deferred mode.    (923026)</li>
<li>Graphics : Fixed TrailRenderer not recording the first position when instantiated using a position and rotation value.   (921297)</li>
<li>Graphics : Improved motion vectors precision when dynamic batching is disabled.  (941966)</li>
<li>Graphics : Made ImageEffects always use the right source buffer, and blit to the final destination if necessary.</li>
<li>Graphics : Metal: Eliminate z-fighting artifacts on certain devices. (950945, 950947) </li>
<li>Graphics: Fixed #pragma target 4.0, 4.6, 5.0 not working on some Android devices.    (933203)</li>
<li>Graphics: Fixed a crash when calling Graphics.SetRenderTarget with a RenderBuffer.   (923977)</li>
<li>Graphics: Fixed an incorrect rendering on Metal after switching from a scene which called Shader.SetGlobalTexture with cubemap texture.</li>
<li>Graphics: Fixed Assert "Invalid mask passed to GetVertexDeclaration() when using post-effect" being triggered e.g. a custom post-effect. (932940)</li>
<li>Graphics: Fixed camera rendering to a temporary RenderTexture from clearing the stencil bits when it should not i.e. for HDR cameras.    (932065)</li>
<li>Graphics: Fixed a crash in CameraStackRenderingState::ReleaseResources e.g. searching in Hierarchy window.   (926718)</li>
<li>Graphics: Fixed a crash in player when using non RGBA32 format 3D textures.  (927145)</li>
<li>Graphics: Fixed D3D11 errors in scenes with a Camera having HDR enabled and depth-only clear.    (933768)</li>
<li>Graphics: Fixed sprite mode to be not a blank when texture type was change via script.   (921598)</li>
<li>Graphics: Report an error instead of crashing when Mesh had invalid positions e.g. NaN.  (930666)</li>
<li>IL2CPP : Allow SetSocketOption to work properly for add membership and remove membership with IPv6.  (944939)</li>
<li>IL2CPP : Fixed calling System.Collections.Generic.IList1 methods on native objects that implement Windows.Foundation.Collections.IVector1 interface and calling Windows.Foundation.Collections.IVector1 methods on managed objects that implement System.Collections.Generic.IList1 interface.</li>
<li>IL2CPP : Implemented a previously unimplemented internal call method to support System.Environment.HashShutDownStarted property.  (947420)</li>
<li>IL2CPP: Added an extra check for a method with a body but an empty instruction list to prevent a crash in IL2CPP.    (940906)</li>
<li>IL2CPP: Avoid stack overflow from occurring in Unity liveness logic. (935563)</li>
<li>IL2CPP: Do not strip System.Reflection types used by Mono.   (930414)</li>
<li>IL2CPP: Fixed calling System.Collections.Generic.IDictionary2 methods on native objects that implement Windows.Foundation.Collections.IMap2 interface from managed code and calling Windows.Foundation.Collections.IMap2 methods on managed objects that implement System.Collections.Generic.IDictionary2 interface from native code.   </li>
<li>IL2CPP: Fixed calling Windows.Foundation.Collections.PropertySet methods that derive from IDictionary`2 interface from managed code. (932981)</li>
<li>IL2CPP: Prevent a NotSupportedException from occurring when System.Net.WebRequest was used with the .NET 4.6 profile on iOS. (938702)</li>
<li>iOS : Cardboard Enable Transition View fix added.    (940917)</li>
<li>iOS : Fixed an occasional crash on iOS when using UnityWebRequest.   (944462)</li>
<li>iOS : Fixed SetIconsForTargetGroup when settings icons for iOS.  (937886)</li>
<li>iOS: Fixed a crash when Low Memory was signalled very early. (941950)</li>
<li>iOS: Fixed Metal TextureUsage crash when Metal API Validation was enabled.   (947026, 940902) </li>
<li>iOS: Fixed the underlying behaviour of the iOS player in order to make the Unity window to be the key window after an orientation change. This was causing problems when, for example, an attempt was made to open an URL when launching FBlogin through the Unity Facebook SDK when in portrait only autorotate state.  (936504, 933588) </li>
<li>Multiplayer : Properly traversing inheritance chain. (933033)</li>
<li>Multiplayer: Force sync internal timers internal time after io thread resuming. </li>
<li>Networking: Fixed an issue where&nbsp;NetworkTransport.SendMulticast&nbsp;caused Unity to crash.   (938980)</li>
<li>OSX: Fix for memory leak in LocalFileSystemOSX::Enumerate when using AssetDatabase.CopyAsset.    (945175)</li>
<li>OSX: Fixed Metal VSync on OSX 10.13 to follow Quality Settings.  (948069, 926730) </li>
<li>Particles : Fixed a crash when script changes quality level at runtime while Shuriken is active. (901096)</li>
<li>Particles : Fixed an upgrade issue where prefab instance shape module values could get corrupted.    (914038)</li>
<li>Particles: Fixed a performance regression when using Size modules.   (930933)</li>
<li>Particles: Removed unnecessary sync between main and graphics threads improving performance when more than one camera is rendering.  (925709)</li>
<li>Physics: Fixed an occasional crash due to orphaned 2D physics contacts.  (938951)</li>
<li>Physics: Stop invalid warning being output to console when destroying a CompositeCollider2D component.   (916584)</li>
<li>Profiler: Fixed a memory leak when connection switched from player to editor.    (928582, 941997, 795258) </li>
<li>Resource Management : Optimized the loading of assets performed via Resources.Load. This addresses a performance regression reported in Android platforms.   (930802)</li>
<li>Scripting Upgrade: Avoid allocating GC memory when calling List.Sort with Comparer`1.    (935845)</li>
<li>Scripting Upgrade: Fixed an issue of "About" window not displaying correctly when using latest scripting runtime.    (944305)</li>
<li>Scripting Upgrade: Fixed a crash when constructing delegate on null reference with virtual method target.    (941391)</li>
<li>Scripting Upgrade: Fixed a crash when inspecting values in managed debugger. (926881)</li>
<li>Scripting Upgrade: Fixed a crash when using managed debugger on OSX. (941204)</li>
<li>Scripting Upgrade: Fixed a hang when closing Editor after opening bug reporter.  (921175)</li>
<li>Scripting Upgrade: Fixed a hang when closing Editor. (944152)</li>
<li>Scripting Upgrade: Report GC pause time correctly in profiler.   (931981)</li>
<li>Scripting: Avoid stack overflow from occurring in Unity liveness logic (asset GC).   (935563)</li>
<li>Scripting: Fixed the debugger error, "Unable to step", when trying to step over dead code blocks (912607)</li>
<li>Scripting: Fix to avoid boxing of values when invoking UnityEvents if the types of the event and listener matches exactly.   (932039)</li>
<li>Scripting: Fixed "Unity extensions are not yet initialized" assertions when opening a project on Windows.    (923633, 944636) </li>
<li>Scripting: Fixed a crash when invalid IL code was encountered.   (942459)</li>
<li>Scripting: Fixed a crash when Ldflda opcode is used and null check was missing.  (918046)</li>
<li>Scripting: Fixed an alignment issue for 64-bit integers and doubles on Android and other non-iOS ARMv7 platforms.    (898636)</li>
<li>Scripting: Fixed an infinite compilation caused by being unable to delete files in Library/ScriptAssemblies on Windows.  (940368)</li>
<li>Scripting: Fixed an internal compiler error due to yield in a lambda statement.  (634364)</li>
<li>Scripting: Fixed an issue with Unity not using the latest changes made to scripts after recompile in Unity on Windows.</li>
<li>Scripting: Fixed Marshal.StructureToPtr when a field type is a multidimensional array of blittable types.    (940012)</li>
<li>Scripting: Fixed use of System.Net.WebRequest in OSX Standalone player.  (940280)</li>
<li>Scripting: Raise MarshalDirectiveException rather than aborting when invalid array marshaling directive is encountered.  (935726)</li>
<li>Shaders: Addressed an internal issue that was causing the same shader to be built different as part of an AssetBundle on each successive build run. This only affected certain shaders and only occurred in macOS.   (933557, 931791) </li>
<li>Timeline : Fix for ExecutionEngineException being thrown at runtime when using Timeline on iOS.  (937737)</li>
<li>Timeline : Fixed the issue of time ruler being inaccessible after relaunching Unity. (935900)</li>
<li>Timeline : Fix for timeline clips not properly being set as dirty.   (926861)</li>
<li>Timeline : Fixed preview mode not always working for humanoid root transforms and custom clips.  (931859)</li>
<li>Timeline : Fixed a crash with playable director holding a reference to a non-playable asset. (936079)</li>
<li>Timeline : Fixed Activation and Control Tracks when application was Paused.  (938170)</li>
<li>Timeline : Fixed preview mode on humanoid root and custom tracks.    (936047)</li>
<li>UI : Fixed memory leak caused by profiler.   (946442)</li>
<li>UnityWebRequest : Allow comments in header values except when known to be unsupported.   (932312)</li>
<li>UnityWebRequest : Ensure that headers are available in UnityWebRequest only after all of them are received.  </li>
<li>UnityWebRequest : Fixed a possible freeze on iOS, when running multiple UnityWebRequests with custom download handler scripts.   (936801)</li>
<li>UnityWebRequest : Fixed automatic scheme prepending to web address (prepend http://) (931602)</li>
<li>UnityWebRequest : Fixed early availability of status code when UnityWebRequest was still running.    </li>
<li>UnityWebRequest : Fixed possible issues aborting UnityWebRequest when using a custom download handler script.    </li>
<li>UWP: Fixed web request not being sent.   (918041, 914981) </li>
<li>Video: (1) is added to VideoPlayer name when added with drag-and-drop.   (948876, 920816) </li>
<li>Video: Fixed audio getting desynchronized from video after seek operations.  (889059, 947404) </li>
<li>Video: Transcoding issues with uncompressed RGBA .mov .  (948877, 856784) </li>
<li>Video: Typo in VideoPlayer editor for Audio Source property tooltip fixed.   (948878, 923258) </li>
<li>VR : Fixed a flickering image on Oculus when MSAA and HDR are disabled.  (949510, 950758) </li>
<li>VR : Fixed an assert&nbsp;IsMatrixValid (matrix)&nbsp;when camera's target eye was set to left or right.   (899259)</li>
<li>VR : Fixed an issue were the right eye was not rendering with Single Pass rendering and camera had Allow HDR enabled.    (920106, 930441) </li>
<li>VR : Fixed an issue whereby CommandBuffer.Blit did not work when used in CameraEvent.AfterEverything.    (918916, 943111) </li>
<li>VR : Improved rendering performance of Daydream and Gear VR apps.</li>
<li>WebGL : Fixed back-buffer anti-aliasing on WebGL1.0. (923698)</li>
<li>WebGL : Fixed file:// protocol warning on browsers that do not allow it. (926842)</li>
<li>WebGL : Fixed Fullscreen mode on Safari. (775206)</li>
<li>WebGL : Fixed server compression configuration warning.  (927459)</li>
<li>Windows Standalone: Fixed an issue that would sometimes cause recursive player loop error.   (946558)</li>
<li>Windows Standalone: Fixed Windows Standalone player failing to load Mono when built to a path with non-ascii characters in it with .NET 4.6 runtime. (944408)</li>
<li>Windows Store Apps: Fixed an issue that was preventing Unity from loading if it is part of an optional store package (941345, 942736) </li>
<li>Windows Store Apps: Fixed an issue where input was being queued on scene load.   (933341, 942734) </li>
<li>XR : Fixed volume buttons not adjusting sound for Google Cardboard applications after they had launched. (938063)</li>
</ul>

#### Revision: cc85bf6a8a04
