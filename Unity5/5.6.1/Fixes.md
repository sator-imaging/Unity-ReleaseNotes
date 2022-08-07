# Unity 5.6.1
https://unity3d.com/unity/whats-new/unity-5.6.1

## Fixes

<ul>
<li>2D: Added POT options in TextureImporter for Sprite. (884926) </li>
<li>2D: Fixed a misleading warning when using Sprite in 'Polygon Mode' for tiling in SpriteRenderer. (889106) </li>
<li>2D: Fixed an error message "Dynamic batching: index buffer destination/source is NULL" when dragging a blank sub-sprite to scene.    (890858)</li>
<li>2D: Fixed an occasional crash when SpriteRenderer.size was set multiple times in a single frame. (898946) </li>
<li>2D: Fixed Sprite data not copy when using EditorUtility.CopySerialized.  (884970) </li>
<li>2D: Fixed the issue of SpriteRenderer not rendering Sprite in tiling mode when tile size was too big.    (891644)</li>
<li>AI: Expose missing API for agent type ID for NavMeshAgent component. (877784)</li>
<li>Analytics: RemoteSettings adding debug_device flag in http header.     </li>
<li>Android: AndroidJava - return null instead of throwing exceptions on functions which return object, class or array.  (839005) </li>
<li>Android: Buildpipe - Fixed an error message on wrong NDK version.    (884540)</li>
<li>Android: Buildpipe - Fixed the user resources library build issues with Gradle.    </li>
<li>Android: Disabled MSAA for backbuffer on older ARM Mali Vulkan drivers.    </li>
<li>Android: Disabled Debug markers on PowerVR Series 5 devices. (780958)</li>
<li>Android: Fixed a rare crash when seeking in an audio file (reported on MotoZ phones).    (871615) </li>
<li>Android: Fixed an issue where ApplicationId was missing from AndroidManifest.xml in Gradle builds    (888274) </li>
<li>Android: Fixed an issue whereby ctrl+b shortcut pushing app package even if it failed to build.  (894074) </li>
<li>Android: Fixed android application building with the latest android sdk. (888859) </li>
<li>Android: Fixed an incorrect error message in the Editor when selecting a non-default version of the NDK. (895550)</li>
<li>Android: Fixed manifest merging with new android sdk tools.    </li>
<li>Android: Fixed Vulkan shadow texture linear filtering.     </li>
<li>Android: Fixed WebCamTexture crash with denied permissions.  (877837) </li>
<li>Android: SoftInput - Fixed input field hidden under keyboard when translucent flag was set.    </li>
<li>Android: Webcam - Fixed the wrong orientation returned on first frames.  (875247) </li>
<li>Animation: Animator.Rebind should reset AnimatorController.  (899553) </li>
<li>Animation: Changing Animator.Speed during an animation transition will now correctly affect the cross-fade speed.    (898503)</li>
<li>Animation: Fixed a crash when using an Avatar built in 5.5 or earlier.   (896033) </li>
<li>Animation: Fixed a performance issue with GetLayerWeight.      </li>
<li>Animation: Fixed a performance regression when destroying many GameObject with Animator. (889109)</li>
<li>Animation: Fixed an issue whereby animation clip range was not updating after undoing 'Add Key' operation.   (892337) </li>
<li>Animation: Fixed a crash in prepare frame due to deactivating Animator in script.    (896659)</li>
<li>Animation: Fixed disabled Animator affecting scene objects.  (901268) </li>
<li>Animation: Fixed IK on Feet not working properly when interrupting transitions.  (892043) </li>
<li>Animation: Fixed OnAnimatorIK not being fired in editor mode.    (894061) </li>
<li>Animation: Fixed StateMachineBehaviour callback on interrupted transition.   (900875) </li>
<li>Animation: Fixed the issue of disabling GameObject not resetting StateMachine.   (894062) </li>
<li>API Updater: Fixed a crash in ScriptUpdater.exe when user scripts contains methods taking pointers as parameters.    (899198) </li>
<li>Asset Bundles: Fixed a performance regression when building many small asset bundles.    (878712)</li>
<li>Asset Pipeline: Fixed an issue when importing assets with name changes that could cause a timestamp mismatch in the database.    (896185)</li>
<li>Audio: Fixed an issue in AudioSource::IsPlaying for streaming audio clips, where false would sometimes be returned incorrectly.  (840294) </li>
<li>Buildpipeline: Fixed an issue with reported texture size being smaller than actual size. (885258) </li>
<li>Cluster Rendering: Fixed the issue of VRPN stopped working in Editor.      </li>
<li>DX12: Fixed double present causing screen blinking.  (885895)</li>
<li>Editor: Attempt to identify and use the cancel option for dialogs that are launched on worker threads, as they can otherwise soft-lock or force-quit  the editor.    (896793)</li>
<li>Editor: Fixed 'Build and Run' attempts to push a build to device even if error (during the build) was encountered.   (894074) </li>
<li>Editor: Fixed "Sprite Mode" so it defaults to "Single" instead of "None" when switching Texture Type to "Sprite (2D and UI)".    (890468) </li>
<li>Editor: Fixed a bug which broke holding alt to pin center of PrimitiveBoundsHandle (affects edit modes for BoxCollider, CapsuleCollider, BoxCollider2D, CapsuleCollider2D, etc.).      </li>
<li>Editor: Fixed an issue where nunit exposed system classes, that could clash with other libraries implementations.    (897850)</li>
<li>Editor: Fixed GUI related Asserts when connected to an active VCS provider.  (895453)</li>
<li>Editor: Fixed screen offsets updates for tooltips.   (884238)</li>
<li>Editor: Switching Cache Server mode from local to a different mode no longer throws exceptions.  (883808)</li>
<li>Editor/macOS: Fixed an issue where exception was being thrown when Visual Studio for Mac was selected as an external script editor. </li>
<li>GI: Fixed lightmap texture inspector preview being too bright when using linear color space. (885492)</li>
<li>Google VR: Fixed the issue of indefinitely flashing screen after changing VRSettings.renderScale.    (896321) </li>
<li>Graphics: Behavior of the VFACE semantic on DX12 is now consistent with the editor.  (895474)</li>
<li>Graphics: Disallow material to be used with CommandBuffer.DrawMeshInstanced if enableInstancing is false.    (898851) </li>
<li>Graphics: Fixed a crash when manually deleting occlusion data.   (877367) </li>
<li>Graphics: Fixed a periodic crash in shadow culling job code (GenerateCombinedDynamicVisibleListJob). (882704) </li>
<li>Graphics: Fixed a regression where a Deferred Camera was throwing a "Dimensions of color surface does not match dimensions of depth surface" error message when a RenderTexture was used.    (899285)</li>
<li>Graphics: Fixed a regression where image effects weren't working as expected in the Scene View.  (900527)</li>
<li>Graphics: Fixed a regression where the objects shaders become unlit when a RenderTexture with Anti-aliasing is active and the Camera RenderingPath is set to Deferred.   (899365)</li>
<li>Graphics: Fixed an editor crash on old OpenGL drivers.   (888339) </li>
<li>Graphics: Fixed an issue on PS Vita causing the default sky to be black. (833583)</li>
<li>Graphics: Fixed Android Adreno chipset frame buffer invalidation appearing as if rendering had frozen.   (894999)</li>
<li>Graphics: Fixed generating invalid raycasts causing "Invalid AABB b0" error appears in console.  (884547) </li>
<li>Graphics: Fixed SceneView GUI elements being very bright when HDR and Linear mode are enabled.   (878724) </li>
<li>Graphics: Fixed the Dynamic Batching rendering code in order to be able to handle valid meshes that have no submeshes.   (903086)</li>
<li>Graphics: Fixed the issue of render texture not being cleared on stop for windows.   (884057) </li>
<li>Graphics: Fixed Vulkan fullscreen scaling on Windows.    (863272) </li>
<li>Graphics: Improved the mechanism for handling imposters. This fixed the error message, 'Internal: Possible leak. All textures should be removed from IdMap when destructed using RemoveTexture(TextureID texid).' which was being triggered when switching a graphics API in a project that contained terrain.   (890527)</li>
<li>Graphics: Mark main splash screen as finished when VR splashscreen was used. (876718) </li>
<li>Graphics: Render texture will no longer be vertically flipped in forward rendering when assigning a null texture.    (899331)</li>
<li>IL2CPP: Allow more deeply nested generic recursion for method metadata. Throw a managed exception when the recursion is too deep.    (889446) </li>
<li>IL2CPP: Fixed a compiler error when using generic delegates with variance.   (881013) </li>
<li>IL2CPP: Fixed marshaling of System.Uri to Windows.Foundation.Uri and back in Windows Runtime interop scenarios.   (887036).</li>
<li>IL2CPP: Fixed memory snapshot profiler not showing multidimensional arrays.  (888796) </li>
<li>IL2CPP: Implemented RegionInfo.CurrentRegion.    (891471)</li>
<li>IL2CPP: Modified the implementation of the IL Switch opcode to workaround a possible C++ compiler bug in Xcode 8.3.  (898861) </li>
<li>IL2CPP: Protect against the usage of attributes that don't exist in .NET 3.5.    (867606) </li>
<li>Installer: Fixed an issue issue with Visual Studio 2017 installer sometimes restarting Windows without warning.    </li>
<li>iOS: Added an option to select whether extra frame was rendered on pause.    (807273) </li>
<li>iOS: Fixed a crash that could occur in callbacks for Social.localUser.Authenticate when the error parameter was read.    (868697) </li>
<li>iOS: Fixed a crash when font's material was assigned to game object. (869947) </li>
<li>iOS: Fixed an issue whereby local notifications were not cleared on iOS10.   (885096) </li>
<li>iOS: Fixed framework search paths in Xcode project being incorrectly quoted if they contained spaces.    (866673) </li>
<li>iOS: Fixed inclusion of ReplayKit framework in plugins.  (882013) </li>
<li>iOS: Fixed some icons not getting copied into Xcode project when Target Device was set to iPhone Only.   (888370) </li>
<li>Kernel : Fixed an issue in JSON parsing that could cause a deserialized box collider to change size. (898787) </li>
<li>Kernel: Obsoleted undocumented FindChild method. (364754)</li>
<li>Lines: Initialized new line vertices to zero, to prevent bad uninitialized data existing in the positions array. (900357) </li>
<li>Lines: Reintroduce missing texture mapping mode, to restore pre-5.5 functionality.   (903466) </li>
<li>macOS: Fixed standalone app compatibility issues when uploading to the Appstore with Application Loader 3.6.   </li>
<li>Metal: Fixed unnecessary half to float casts in generated shaders.   (898788) </li>
<li>Mono: Corrected the handling of C# compiler errors in a column that are more than 255 characters wide.   (902758) </li>
<li>Mono: Prevent DeflateStream from throwing an exception when an empty stream is flushed.  (889296)</li>
<li>MonoDevelop: Allow breakpoints to properly load in MonoDevelop in some situations where they did not load before.    (889998)</li>
<li>Particles: Fixed a case where ping-pong emission could occasionally spawn particles at the wrong end of the line shape.  (876597) </li>
<li>Particles: Fixed an incorrect error message about sub-emitter parenting. (899574) </li>
<li>Particles: Fixed trail interpolation in Edit Mode, when using slow-motion previewing.      </li>
<li>Particles: Reduced Particle System memory usage, to improve the large increase seen since Unity 5.2. (888236) </li>
<li>Particles: Reinstated ability to animate EmissionModule.enabled, plus add bindings for the enabled flag of every module.   </li>
<li>Particles: Reinstated random emission modes.   </li>
<li>Particles: Revert particle simulation space to world space, when custom transform is missing.    (874999) </li>
<li>Physic 2D: Fixed physics animation transform change not correctly rotating a Rigidbody2D.    (896867) </li>
<li>Physics 2D: Fixed a crash and infinite loop when triangulating Polygon2D.    (880353, 891305, 905608) </li>
<li>Physics 2D: Fixed a crash during reparenting of a Rigidbody2D.   (901465) </li>
<li>Physics 2D: Do not draw Collider AABB gizmo if attached to a Rigidbody2D with 'simulated' property set to false.   </li>
<li>Physics 2D: Fix for Rigidbody2D interpolation loosing precision with time.   (843507) </li>
<li>Physics 2D: Fix for where infinite 2D raycast misses EdgeCollider2D edge.    (895732) </li>
<li>Physics 2D: Fixed an issue with minimum threshold size for BoxCollider2D.      </li>
<li>Physics 2D: Fixed backward compatibility for Physics2D.queriesHitTriggers, Physics2D.queriesStartInColliders, Physics2D.defaultContactOffset &amp; PolygonCollider2D.points. (896824) </li>
<li>Physics 2D: Removed duplicate profiler entry of "Physics2D.Simulate".     </li>
<li>Profiler: Changed the colour of the 'Others' field in order to clearly differentiate it from the one used by 'Scripts'.  (898513)</li>
<li>Purchasing: Fixed an issue with Unity IAP emitting DuplicateTransaction failure for all non-consumable purchases when initialized.   (889321)</li>
<li>Scripting: Fixed a parameter corruption and potential crashes for some delayed callbacks.    (868697) </li>
<li>Scripting: Fixed an issue with scripts always being compiled on project open.      </li>
<li>Shaders: Fixed a subtle metal shader generation bug in bit field insert operations.    </li>
<li>Shaders: Fixed an incorrect translation from HLSL assembly for AND and OR operands. Also fixed a crash when compiling shaders for GLCore.    (883080) </li>
<li>Shaders: Removed fastmath compiler option from Metal compute shaders, as it could create different results compared to other platforms.    </li>
<li>SkinnedMeshRenderer: Fixed bugs related to updating. (904904, 904905, 904906, 904907) </li>
<li>SpeedTree: Fixed GPU instancing break when the trees came back into view.    (883720)</li>
<li>Terrain: Fixed an assert that got triggered by deleting a folder that contained a Terrain object.    (895548)</li>
<li>Tizen: Changed symbols in mono to HIDDEN.      </li>
<li>UGUI: Fixed a memory leak in UGUI.     </li>
<li>UI: Fixed NaN issues with ScrollRect when using clamped mode.    (893559) </li>
<li>UI: Fixed nested canvas returning a null world camera after its root canvas had been disabled and then re-enabled.   (892913) </li>
<li>Unity Ads: Prevent Unity Ads internal MonoBehaviours from showing in the inspector now.  (858540) </li>
<li>Unity test runner: Fixed EditorPref to be Project setting.   (895742)</li>
<li>UnityWebRequest: Allow overriding user-agent.    (806211) </li>
<li>UnityWebRequest: Fixed an issue with getting texture from download handler after scene change.   (884291) </li>
<li>UnityWebRequest: Fixed formatting multiform post request with section list.  (899017) </li>
<li>UnityWebRequest: Fixed getting stuck when using custom download handler script in Editor in edit mode.   (893302) </li>
<li>UnityWebRequest: Fixed nonReadable parameter in UnityWebRequestTexture.GetTexture() working the opposite way.    (876648)</li>
<li>Video: Fixed issues related to video preparation.    (893939, 897708, 899233, 893910) </li>
<li>Video: Better error handling and reporting when attempting an OSX H.264 transcoding exceeding profile level limits.  (891028) </li>
<li>Video: Fixed an incorrect crop happening on Android Samsung devices Samsung with OS 4.3, resulting in a few uninitialized lines showing at the bottom of the video.  (903657)</li>
<li>Video: Fixed clip selection dialog video preview for non-transcoded material.    (887882) </li>
<li>Video: Prevent a crash when playing vp8 movies on Android OS 4.1 / 4.2 on Samsung and Meizu devices. (893945)</li>
<li>Video: Prevent crash on negative resolution custom resize transcode. (893837) </li>
<li>VR: Accessing PlayerSettings.VRDaydream.* scripting API no longer results in MissingMethodException. (898357) </li>
<li>VR: Added Fade out to VR Splash Screen for Daydream.   </li>
<li>VR: Fixed a bug where particles shaders displayed compile errors if stereo instancing was enabled.   (872164)</li>
<li>VR: Fixed a bug where the occlusion mesh was visible from the game window.   (902791) </li>
<li>VR: Fixed a crash when there were no renderable cameras. (901617) </li>
<li>VR: Fixed a potential crash when entering play mode. (896314) </li>
<li>VR: Fixed an editor crash when performing a bloom gesture while using HoloLens remoting. (897406) </li>
<li>VR: Fixed Render Viewport Scale for Forward rendering. Deferred still has issues that should be addressed in a later patch.    </li>
<li>VR: Fixed some shader related issues when using single-pass stereo rendering on Android devices.   </li>
<li>VR: Standalone VR build crashes with Graphics Jobs and Soft Particles.   (889591) </li>
<li>VR: Update GearVR to version 1.13.1 to fix black screen when multiview, monoscopic, or double-wide eye buffers are used.   </li>
<li>Windows Store: Fixed a build error "Failed to resolve assembly: 'Windows.Foundation.UniversalApiContract, Version=3.0.0.0, Culture=neutral, PublicKeyToken=null'"." when using default parameters of Windows Runtime types in method signatures and "C# projects" build option on .NET scripting backend.    (884058)</li>
<li>Windows Store: Fixed a build error on .NET scripting backend when a method with name OnMouseDown was defined in a non-monobehaviour class.   (869168) </li>
<li>Windows Store: Fixed a crash that could occur with D3D build type when the window was minimized or closed.   (885964) </li>
<li>Windows Store: Fixed a crash when using "SceneManager.UnloadSceneAsync" on .NET scripting backend with .NET native enabled.  (869407) </li>
<li>Windows Store: Fixed a rare build error "Failed to resolve assembly: 'System.Reflection.TypeExtensions, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b03f5f7f11d50a3a'" on .NET scripting backend when using "C# projects" option.   (885997) </li>
<li>Windows Store: Fixed a rare build error "Version not supported: 255.255.255.255" when using certain .winmd plugins and "C# projects" option on .NET scripting backend.   (886049)</li>
<li>Windows Store: Fixed a System.TypeInitializationException on startup with .NET scripting backend when a nested class derives from a non-nested class and overrides one of its methods.   (872058) </li>
<li>Windows Store: Fixed an issue whereby not being able to switch to Windows Store platform when Windows 10 SDK was not installed.  (890043) </li>
<li>Windows Store: Fixed non-alloc physics overlap functions causing a crash on .NET Scripting Backend.  (888660) </li>
<li>Windows Store: Fixed Screen.SetResolution not accounting for DPI settings.   (875849) </li>
<li>Windows: Fixed a case of Screen.DPI returning the DPI of the primary monitor when the window was on a secondary monitor. (870209) </li>
<li>Windows: Fixed window automatically resizing to fill the screen when in windowed mode and the monitor's display mode got changed through windows display settings.   (891481) </li>
<li>WWW: Fixed an issue whereby new WWW object without internet connection did not set Error field.  (776552) </li>
</ul>

#### Revision: 2860b30f0b54
