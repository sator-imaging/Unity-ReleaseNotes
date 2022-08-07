# Unity 5.6.4
https://unity3d.com/unity/whats-new/unity-5.6.4

## Fixes

<ul>
<li>AI: NavMeshBuilder can now use non-read/write meshes to generate NavMeshes in edit mode. (935105) </li>
<li>Analytics: Switched the analytics events sent to the new protocol.     </li>
<li>Android : Fixed a shader compile error on devices not supporting GL_FRAGMENT_PRECISION_HIGH. (945953) </li>
<li>Android : Fixed the issue of black screen on startup on Android Oreo devices.     (945338, 946060) </li>
<li>Android : Resources.Load no longer stalls LoadScene and LoadSceneAsync.   (918875) </li>
<li>Android: Buildpipe - Don't force exported gradle projects to be signed.  (923652)</li>
<li>Android: Fixed a regression that was causing the incorrect scaling of the splash screen. (925797)</li>
<li>Android: Fixed an issue with having lots of VBOs allocated even for an empty scene on Android during application startup.    (937876)</li>
<li>Android: Gradle: Added settingsTemplate.gradle to allow user customization.  (924780, 924784) </li>
<li>Android: VideoPlayer - Fixed an issue where H264 video did not loop on HTC One (OS 4.2.2).   (925738) </li>
<li>Animation : Fixed alpha channel being animated when in linear color mode.    (935087) </li>
<li>Animation: Fix for events not being fired during CrossFade at 0F.    (920126) </li>
<li>Animation: Fixed a crash that was caused during the assignment of an incomplete AnimatorController stored in an AssetBundle. (927444)</li>
<li>Animation: Fixed a crash when changing OverrideController during interrupted transition. (928601) </li>
<li>Animation: Fixed a glitch that was causing a stuttering in the Animation curve when rotating a GameObject in the Animation window.   (930336)</li>
<li>Animation: Fixed a regression that was preventing Math symbols from being evaluated in the Animation window's input field.   (930988)</li>
<li>Asset Bundles: Fixed an issue where calling LoadAllAssets with a type parameter could cause loading errors.  (930819) </li>
<li>Asset Bundles: Fixed an issue where IK float values weren't getting blended if animations were split between two Asset Bundles.  (920973) </li>
<li>Build Pipeline : Fixed a bug where running Unity in batch mode wasn't selecting the correct build target group on startup.   (938685) </li>
<li>Build Pipeline : Fixed the behaviour of the build process so that all the scripts get recompiled if the build process fails. (921652, 937648) </li>
<li>Build Pipeline: Fix for corrupt OSX standalone app icons in certain situations.  (815319) </li>
<li>Build Pipeline: Fixed an assert and a potential crash when building projects with Materials or Shader Variant Collections which referenced missing shaders (i.e deleted).    (885275) </li>
<li>Build Pipeline: Fixed GameReleaseCollector crash on recursive function.  (865522) </li>
<li>Build Pipeline: Fixed incorrect mesh channel stripping when mesh was used as a shape emitter in particle systems.    (917568) </li>
<li>Build: Fixed an issue where scenes were not restored correctly if the build process was aborted. (891971) </li>
<li>Editor : Fixed Callback registration failed kMaxCallback&nbsp;crash when entering playmode.   (873467) </li>
<li>Editor : Fixed incorrect lighting when switching to Metal device if Editor was started in OpenGL.      </li>
<li>Editor: Calculate mipmap count properly when importing NPOT textures with '-nographics'  (925913) </li>
<li>Editor:  Fixed Security Vulnerability UNITY-SEC-844-https://unity3d.com/security.</li>
<li>Foundation : Fix for a fake memory leak spamming "ALLOC_TEMP_THREAD has unfreed allocations" when calling PluginImporter.SetPlatformData.    (925589) </li>
<li>GI : Fixed a case where object lighting preview was empty for meshes with no normals.    (726487) </li>
<li>GI : Fixed an issue where creating a new scene in project window affected the lighting settings of other scenes. (919234) </li>
<li>GI : Fixed environment Reflection Probe not updating when the user changed the context of the Skybox shader. (907378) </li>
<li>GI : Fixed Shadowmask in Forward rendering when multiple directional lights are used.    (925579) </li>
<li>Graphics : [Metal] Eliminated Z-fighting artifacts on certain devices.   (950977)</li>
<li>Graphics : Fixed a crash on exit from fullscreen player when using OpenGLCore graphics API.  (922715) </li>
<li>Graphics : Fixed a crash when a valid Mesh had no submeshes. (918642) </li>
<li>Graphics : Fixed a crash when assigning (invalid) Mesh to a SkinnedMeshRenderer from script in standalone player.    (922996) </li>
<li>Graphics : Fixed a crash when depth surface was missing from RenderTarget setup i.e. GrabPass.   (921083) </li>
<li>Graphics : Fixed a crash when trying to use 16-bit RenderTexture on systems which did not support them.  (906072) </li>
<li>Graphics : Fixed a crash when using Compute Shader with very large number of thread groups i.e. greater than 500,000.    (826751)</li>
<li>Graphics : Fixed a crash when Vulkan loader was installed but no drivers were installed and Vulkan was used as the default API.  (898184) </li>
<li>Graphics : Fixed a rare case when shader compilation failed with error message "Failed to find parameters of a compiled D3D9 shader".    (918636) </li>
<li>Graphics : Fixed a rare crash when dynamic batching is enabled.  (938089, 944773) </li>
<li>Graphics : Fixed an issue where by multiple display camera was not rendering after reloading the scene using SceneManager.LoadScene().   (782380) </li>
<li>Graphics : Fixed an issue where Terrain was not showing wireframe in shaded-wireframe mode.  (922739) </li>
<li>Graphics : Fixed dynamic batching overwriting the vertex colour stream on untextured meshes. (803067) </li>
<li>Graphics : Fixed incorrect rendering on Metal after switching from a scene which called Shader.SetGlobalTexture with cubemap texture.      </li>
<li>Graphics : Fixed loading shaders in a variant collection not loading the variants from all passes which match.     </li>
<li>Graphics : Fixed memory leak in Editor scene view.   (916425)</li>
<li>Graphics : Fixed Mesh becoming offset and scaled when accessing 'mesh' property on a MeshFilter on a static GameObject and static batching was enabled.  (733687) </li>
<li>Graphics : Fixed occlusion culling of shadows within the camera sightline.   (829193) </li>
<li>Graphics : Fixed TrailRenderer not recording the first position when instantiated using a position and rotation value.     </li>
<li>Graphics : Improved documentation to explain when using Graphics.Blit to a Null target it may get re-routed to a texture if the main camera had a RenderTexture as a target. (775291) </li>
<li>Graphics: Ensure textures with too high mip count on Metal are not created.  (915959)</li>
<li>Graphics: Fixed "Tiled GPU perf. warning: RenderTexture color surface was not cleared/discarded doing..." in Unity when emulating OpenGL ES 2.0 or 3.0.  (909148) </li>
<li>Graphics: Fixed a crash when building splash screen with only a portrait background image.   (913251) </li>
<li>Graphics: Fixed a crash when instancing was enabled on specific Material.    (911654) </li>
<li>Graphics: Fixed a race condition crash when using Native Graphics Jobs.  (929961)</li>
<li>Graphics: Fixed a rare crash caused by recursive rendering ie. Camera.Render() or Water rendering.   (878317) </li>
<li>Graphics: Fixed lighting rendering when using multiple cameras and at least one camera renders to a RenderTexture.   (903537) </li>
<li>Graphics: Fixed memory leak in Texture2DArray and CubeMapArrayTexture.   (919162) </li>
<li>Graphics: Fixed Nav Mesh Preview in Scene View being affected by lighting.   (913612) </li>
<li>Graphics: Fixed rendering issues when using a camera with a RenderTexture and non-fullscreen viewport.   (910036) </li>
<li>Graphics: Fixed runtime crash when modifying skinned mesh and GPU Skinning was enabled.  (811757) </li>
<li>Graphics: Removed code that tries to re-use dynamic gemometry buffers for multiple renders - there were too many edge cases to reliably detect when this was possible.   (916142, 933890) </li>
<li>IL2CPP : Added an extra check for a method with a body but an empty instruction list to prevent a crash in IL2CPP.   (940906) </li>
<li>IL2CPP : Fixed calling System.Collections.Generic.IDictionary2 methods on native objects that implement Windows.Foundation.Collections.IMap2 interface from managed code and calling Windows.Foundation.Collections.IMap2 methods on managed objects that implement System.Collections.Generic.IDictionary2 interface from native code.    </li>
<li>IL2CPP : Fixed calling Windows.Foundation.Collections.PropertySet methods that derive from IDictionary`2 interface from managed code.    (932981) </li>
<li>IL2CPP: Corrected a possible crash with the RegionInfo class in mscorlib.dll was incorrectly removed by the managed code linker. (930252) </li>
<li>IL2CPP: Fixed an issue with setting enum type fields in .NET 4x with relfection using an integer value.  (923517) </li>
<li>IL2CPP: Prevent a compilation error in the generated code for some Windows Store apps.   (921467) </li>
<li>IL2CPP: Prevent a failure during code conversion when a constrained method call is made on a volatile type.  (929802) </li>
<li>Input: Fixed an issue on Windows where IME for Chinese, Japanese and Korean was enabled when typing even though not focused on a text field. (821419) </li>
<li>iOS : Fixed a crash when Low Memory is signaled very early.  (941950)</li>
<li>iOS : Fixed an occasional crash on iOS when using UnityWebRequest.   (944462)</li>
<li>iOS : Fixed the underlying behaviour of the iOS player in order to make the Unity window the key window after an orientation change. This was causing problems when, for example, an attempt was made to open a URL when launching FBlogin through the Unity Facebook SDK when in portrait only autorotate state.    (933588, 944619) </li>
<li>iOS: Fixed 'Stale touch detected!' error message that showed up after minimizing, re-opening an app and immediate start tapping the screen with multiple fingers (934401)</li>
<li>iOS: Fixed trampoline compilation issues for iOS 11 simulator.     </li>
<li>iOS: Fixed: Cardboard Enable Transition View.    (940918)</li>
<li>Linux: Fixed native plugin lookup when the plugin was marked as compatible with both x86 and x86_64.   </li>
<li>OSX : Fix for memory leak in LocalFileSystemOSX::Enumerate when using AssetDatabase.CopyAsset.   (945175) </li>
<li>OSX : Fix for VSync not working on OpenGL Editor.      </li>
<li>OSX : Fixed VSync for Metal on OSX 10.13 to follow Quality Settings. (948070)</li>
<li>Particles : Fixed a crash when script changes quality level at runtime while Shuriken was active.    (901096) </li>
<li>Particles : Removed unnecessary sync between main and graphics threads improving performance when more than one camera is rendering  (925709)</li>
<li>Particles: Fixed a crash when a sub-emitter GameObject did not exist.    (930370) </li>
<li>Particles: Fixed problems when upgrading instanced Particle System Prefabs.  (911189) </li>
<li>Particles: Restore "Show Selected" mode to the Particle System Editor Window.     (901440) </li>
<li>Physics : Stop invalid warning being output to console when destroying a CompositeCollider2D component.  (916584) </li>
<li>Physics: Fixed an issue where ContactPoint2D.normalImpulse and ContactPoint2D.tangentImpulse were always zero when accessing via callbacks.  (927637) </li>
<li>Platforms: Fixed a crash when '-cleanedLogFile' was passed but no log file name was given.   (859361) </li>
<li>Profiler : Fixed memory leak when connection switched from player to editor. (928582, 941997, 795258) </li>
<li>Scripting : Avoid stack overflow from occurring in Unity liveness logic (asset GC).    </li>
<li>Scripting : Fixed a crash if delegate was created on un-inflated generic type.   (763091) </li>
<li>Scripting : Fixed a crash when invalid IL code was encountered.  (942459) </li>
<li>Scripting : Fixed a crash when Ldflda opcode was used and null check was missing.    (918046) </li>
<li>Scripting : Fixed debugger error of "Unable to step" when trying to step over dead code blocks.  (912607) </li>
<li>Scripting : Fixed Marshal.StructureToPtr when a field type was a multidimensional array of blittable types.    </li>
<li>Scripting : Raised MarshalDirectiveException rather than aborting when invalid array marshaling directive was encountered      </li>
<li>Scripting: Fixed a potential domain reload issue in play mode when trying to validate scripts.   (926516) </li>
<li>Scripting: Fixed alignment issue for 64-bit integers and doubles on Android and other non-iOS ARMv7 platforms.   (898636)</li>
<li>Scripting: Fixed an issue where the managed debugger on Windows was hanging when all scripts with OnAudioFilterRead had been disabled.    (918651) </li>
<li>Scripting: Prevent a failure during code conversion when a constrained method call is made on a volatile type.   (936096) </li>
<li>Shaders : Addressed an internal issue that was causing the same shader to be built different as part of an AssetBundle on each successive build run. This only affected certain shaders and only occurred in macOS.  (931791, 936519) </li>
<li>Shaders: Fixed GLSL shader compile errors due to lack of default precision specifier.    (899502) </li>
<li>Shaders: Vulkan- Fixed a rare incorrect shader generation on expressions with write masks.   (908903)</li>
<li>Terrain: Fixed a crash that could happen when there are a very large number of terrains with SpeedTree trees on them.    (935808)</li>
<li>Terrain: Fixed an issue where error messages about JobTempAlloc would appear in player output log if trees were used on a terrain.   (935800)</li>
<li>UI: Fixed unity crashing when undoing the deletion of a prefab with a UI element.    (876232) </li>
<li>UnityWebRequest : Ensure that headers are available in UnityWebRequest only after all of them are received.    </li>
<li>UnityWebRequest : Fixed a possible freeze on iOS, when running multiple UnityWebRequests with custom download handler scripts.   (936801) </li>
<li>UnityWebRequest : Fixed early availability of status code when UnityWebRequest was still running.      </li>
<li>UnityWebRequest : Fixed possible issues aborting UnityWebRequest when using a custom download handler script.      </li>
<li>Universal Windows Platform: Fixed building generated UWP projects with Visual Studio 2017.3 when using .NET scripting backend.     </li>
<li>Universal Windows Platform: Fixed the issue where locking the mouse in UWP player would cause wrong values returned from Input.GetAxis() on the next Update. (911008) </li>
<li>VR : Fixed an assert IsMatrixValid (matrix) when camera's target eye was set to left or right.   (899259) </li>
<li>VR : Fixed an issue were the right eye was not rendering with Single Pass rendering and camera had Allow HDR enabled.    (920106, 930441) </li>
<li>VR : Fixed an issue whereby CommandBuffer.Blit did not work when used in CameraEvent.AfterEverything.    (918916, 943111) </li>
<li>VR : Improved rendering performance of Daydream and Gear VR apps.      </li>
<li>VR: _MainTex_ST values are now correct in non VR mode.   (905062)</li>
<li>VR: Fixed - Stereo Convergence setting has no actual impact. (850334) </li>
<li>VR: Fixed blit to temporary RT not setting _MainTex_ST.  (918634) </li>
<li>VR: Removed some unnecessary GPU work at the end of the frame for VR apps.     </li>
<li>XR: Fixed volume buttons not adjusting sound for Google Cardboard applications after they have launched. (938063) </li>
</ul>

#### Revision: ac7086b8d112
