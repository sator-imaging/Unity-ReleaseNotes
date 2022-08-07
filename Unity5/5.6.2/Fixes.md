# Unity 5.6.2
https://unity3d.com/unity/whats-new/unity-5.6.2

## Fixes

<ul>
<li>2D: Added Sprite changes in play mode when using [TIGHT] texture packing and high quality compression.   (871871) </li>
<li>2D: Changed warning message "MaterialPropertyBlock is used to modify these values" to info message.  (888016) </li>
<li>2D: Fixed an issue where SpriteUtility.GetSpriteUvs returned invalid Uvs.    (898383) </li>
<li>2D: Fixed an issue whereby blue line briefly flickers when moving mouse in Sprite Editor "Edit Outline" mode in OSX Metal.   (903668) </li>
<li>2D: Fixed an issue whereby Sprite packer caused Out of memory error. (897066) </li>
<li>AI: Added missing API for minimum region area when building a NavMesh using the runtime API. (906017)</li>
<li>AI: Fixed a crash happening when Warp() is called many times for a NavMeshAgent. (904910) </li>
<li>AI: Fixed a regression where a NavMeshAgent with 'autoTraverseOffMeshLink' set to false would not move freely.   (905621)</li>
<li>AI: Fixed an internal limitation of slope maximum of 60 degrees when building a NavMesh using the runtime API.   (906012)</li>
<li>AI: Fixed an issue where carving obstacles could create wrongly shaped holes on NavMesh instances of arbitrary rotation. (902956) </li>
<li>AI: Fixed missing support for triangulating NavMesh instances with arbitrary rotation.   (886302) </li>
<li>Android: Buildpipe - Fixed slow loading with OBB by processing streaming assets in obbassets.</li>
<li>Android: Changed threshold to recognize big cores of ARM big.LITTLE architecture better. (915805) </li>
<li>Android: Dropped obscured touch events to prevent tapjacking.    (900191)</li>
<li>Android: Fixed a regression where Banner Ads are invisible, but still clickable. (916119)</li>
<li>Android: Fixed an out of memory crash when using a static splash screen. (905867) </li>
<li>Android: Fixed assertion failures of GLES calls without valid context on debug and development builds.   (898900,868921) </li>
<li>Android: Fixed pause/resume issues when loading with static splash image.    (867891) </li>
<li>Android: Fixed the build process when using Gradle so that checks for signed applications are performed at the beginning of the build process, instead of at the end.    (890531)</li>
<li>Android: Make SoftInput not take fullscreen on landscape orientation.    (905581)</li>
<li>Animation: Fixed a crash when loading an asset bundle with an override animator controller.  (908960)</li>
<li>Animation: Fixed an issue where using an override controller multiple times would not animate correctly. (910194)</li>
<li>Animation: Fixed animating Material Vector4 properties when in linear color space.   (908999) </li>
<li>Animation: Fixed animation root motion layering. (900109) </li>
<li>Animation: Fixed DeoptimizeTransformHierarchy crashing when a GameObject with a SkinnedMeshRenderer was attached to an exposed bone. (896498)</li>
<li>Animation: Fixed incorrect animated color values when in linear color space. (893042) </li>
<li>Animation: Improved build and AssetBundle data determinism for Human components.</li>
<li>Build Pipeline: Fixed a crash when building a project containing materials with missing shaders. (915659)</li>
<li>Build Pipeline: Fixed AssetBundle statistics that are printed to the editor log when building AssetBundles.  (890644) </li>
<li>Build Pipeline: Fixed issue with Scene AssetBundles that would cause multiple builds with the same Scene to generate different results.  (895452) </li>
<li>BuildPipeline: Fixed an issue when trying to build asset bundles for target other than what was selected in Build Settings.  (865770) </li>
<li>Editor: Fixed 1-dimensional sphere bounds handle had no wireframe representation.</li>
<li>Editor: Fixed an invalid index error when deleting custom resolution in game view.   (879531) </li>
<li>Editor: Fixed an issue where the editor would go unresponsive and text would turn red ("Missing built-n guistyle", "Unable to find style").  (888678)</li>
<li>Editor: Fixed issue where color picker would crash on Metal. (901529)</li>
<li>Editor: Fixed issue where Mesh and Model previews would not render in the Inspector window. </li>
<li>Editor: Fixed issue with NullReferenceException when deleting the last remaining quality setting.    (903620) </li>
<li>Editor: Fixed issue with Xcode project; queueDebuggingEnabled is now included.   (908964)</li>
<li>Editor: Fixed PrimitiveBoundsHandle.DrawHandle() not resetting Handles.color if alt-clicking to rotate camera.</li>
<li>Editor: Fixed SerializedObject.maxArraySizeForMultiEditing not being respected when using default property drawer.   (817640) </li>
<li>Fix to prevent crashes in the editor due to UI and animation (889776) </li>
<li>Fixed an issue where plugins would only clear part of the framebuffer when single pass stereo is enabled. This also fixes VRWorks' Single Pass Stereo and Lens matched shading.  (908990)</li>
<li>Fixed issue where profiler would crash when the active frame was out of view.    (903397) </li>
<li>Fixed TextureImporter to allow newly-imported textures to have their AssetBundle name/variant set.   (905640) </li>
<li>GI: Added support for negatively scaled Meshes in the progressive lightmapper. This now allows you to mirror Meshes using negative Transform values. (883844)</li>
<li>GI: Added support for quads in progressive lightmapper.  (890651) </li>
<li>GI: Avoid a threading issue, where the Progressive Lightmapper cannot find an instances when it was removed too fast.    (891834, 916806) </li>
<li>GI: Fixed "Bake paused in play mode" hanging on opening another scene in Play mode.  (726106)</li>
<li>GI: Fixed a crash when creating Reflection Probes from OnWillRenderObject.   (873026)</li>
<li>GI: Fixed AddInstanceProperties errors thrown when baking progressive lightmapper.   (899488) </li>
<li>GI: Fixed an issue where a certain combination of GI settings and multiple Scenes being additively loaded would make baked light maps vanish.    (815031)</li>
<li>GI: Fixed an issue where Final Gather would cause light bleeding when baking with the Enlighten lightmapper backend. (898200) </li>
<li>GI: Fixed baked Area light affecting objects behind meshes where light shouldn't be present. (875096) </li>
<li>GI: Fixed halos display when more than 64 of them.   (902205) </li>
<li>GI: Fixed quality Level button not wide enough and clips text.   (875894)</li>
<li>GI: Inverse squared falloff in progressive lightmapper.</li>
<li>GI: Stop Gauss filter from correcting certain pixel values in invalid regions.   (893958) </li>
<li>GI: Synchronized Box Projection option in Reflection Probe component with the global setting from current Tier Settings. When the option in Tier Settings is disabled, the probe UI with show a disabled unchecked checkbox for Box Projection.  </li>
<li>GI: Updated the tooltip for Box Projection option in Reflection Probe component. The setting can be affected by the Reflection Probes Box Projection setting in the Tier Settings.   </li>
<li>GI: Visible artifact when using point lights in linear color space.  (751629) </li>
<li>GI: When editing Lightprobes they can be duplicated. (900888) </li>
<li>Graphics: Disabled directional shadows when Screen Space Shadows (Edit &gt; Project Settings &gt; Graphics) is set to No Support but Cascaded Shadows is enabled in the Tier Settings.   (867797) </li>
<li>Graphics: Fixed a crash and error when attempting to set color surface as depth render target or vice-versa. (898318) </li>
<li>Graphics: Fixed a crash in DrawMeshNow. It will now throw a null reference exception instead of crashing.</li>
<li>Graphics: Fixed a crash in Graphics.Blit() with a NULL source and destination.   (896686) </li>
<li>Graphics: Fixed a crash that occurred when Texture.GetPixels or Texture.SetPixels were used with invalid input parameters.   (771031) </li>
<li>Graphics: Fixed a crash when mesh was removed from meshrenderer on an object with cloth component.   (898923) </li>
<li>Graphics: Fixed a crash when using DestroyImmediate() on a RenderTexture in OnPreRender callback.    (897665) </li>
<li>Graphics: Fixed an issue in mesh compression that under the 'right' circumstances would have caused the maximum value in the range to be rounded to the minimum value.   (883901) </li>
<li>Graphics: Fixed an issue where instancing variants being incorrectly stripped away for shaders that use fallback mechanism for e.g. shadow caster pass.  (903790) </li>
<li>Graphics: Fixed clear artifacts appearing on Metal when only the UI camera was used in the Scene.    (909607)</li>
<li>Graphics: Fixed coherent alpha channel importing for various image format especially formats with more than 32-bits per pixel. Do not generate alpha channel if the alpha value is constant in the source texture.   (901649) </li>
<li>Graphics: Fixed CommandBuffer.Blit always writing to the first depth slice of a 3D render target and ignoring the depthSlice parameter.  (879378) </li>
<li>Graphics: Fixed crash that occurred while turning off occlusion culling with high shadow distance.   (888704) </li>
<li>Graphics: Fixed Cubemap.GetPixel returning the wrong data from a BC6H compressed cubemap.    (871140) </li>
<li>Graphics: Fixed inconsistent initialization in ComputeScreenSpaceShadowMap.  (767050) </li>
<li>Graphics: Fixed issue where, when Scene is set to Validate Albedo mode, Unity would render Baked GameObjects and other GameObjects in the Scene as planes.   (893187)</li>
<li>Graphics: Fixed Mesh (and memory) leaks when the Profiler window is open.    (822255) </li>
<li>Graphics: Fixed R8 &amp; RG16 texture support for D3D11. </li>
<li>Graphics: Fixed rendering of multiple cameras and depth being ignored when setting camera viewports to be different to each other.   (885051) </li>
<li>Graphics: Fixed RenderToCubemap when using a HDR enabled Camera. This fixes prevents error message "Releasing render texture whose render buffer is set as Camera's target buffer with Camera.SetTargetBuffers!".    (902409) </li>
<li>Graphics: Fixed Texture and Cubemap Arrays only containing the first texture in Standalone builds.   (899324) </li>
<li>Graphics: Fixed Texture2D.PackTextures not copying the source texture data correctly in an uncompressed atlas with non-zero padding. (898285) </li>
<li>Graphics: Fixed UI and gizmo being rendered with the wrong gamma in scene view.  (878724) </li>
<li>Graphics: Fixed Windows Standalone player sometimes crashing on display activation when color space in player settings is set to Linear. (901270) </li>
<li>Graphics: Improve the documentation for RenderTexture to clarify the behaviour of RenderTexture.DiscardContents  .</li>
<li>Graphics: Update documention to clairfy that a MaterialPropertyBlock cannot set the render state.    (889652) </li>
<li>IL2CPP: Allow now the Guid attribute to be used on generic types.    (914197)</li>
<li>IL2CPP: Applied a fix to prevent the following exception occuring on some projects during runtime: 'NotSupportedException: IL2CPP encountered a managed type which it cannot convert ahead-of-time. The type uses generic or array types which are nested beyond the maximum depth which can be converted'.  (905659) </li>
<li>IL2CPP: Fixed an issue which caused IL2CPP to fail to convert assemblies if two non-existing methods with the same declaring type were referenced from any assemblies.   (917343) </li>
<li>INTERNAL: Android: Buildpipe - Print the step duration in the editor log . </li>
<li>iOS: Fixed broken microphone permissions when camera is not used in app. </li>
<li>Linux: Fixed uninitialized screen dimensions at startup with some window managers.   (880426) </li>
<li>Linux: Unlock cursor when switching from Locked to Confined mode. </li>
<li>Metal: Fixed GPU hang on A7/A8 devices in some MSAA scenarios.   (902650) </li>
<li>Metal: Fixed the issue of not rendering of standard shader with webgl emulator.  (916365)</li>
<li>Mobile: Disabled RunInBackground on Android and iOS. (826473) </li>
<li>Mono: Applied a fix to prevent a crash that might occur when deep profiling is enabled in the Unity Editor.  (898854) </li>
<li>Mono: Corrected a crash in the C# compiler when two or more overloaded operators were used in the same statement.    (910302) </li>
<li>Mono: Corrected an invalid C# compiler error with generic types in compiler generated code (like lambdas and enumerators). The error from the C# compiler often includes this text: "There is no boxing or type parameter conversion from...".   (847798) </li>
<li>Mono: Fixed Mono C# compiler on Windows when using "non-standard" locales.   (910101, 875075) </li>
<li>Mono: Prevent a crash in a crash in mono_class_from_mono_type when using "new Enum[]{}" array in the script. (914470) </li>
<li>Mono: Prevent an intermittent crash in Unity when the managed debugger is attached.  (914171) </li>
<li>Multiplayer: Fix for the issue where reliable messages can be dropped in high dropping rate environment. </li>
<li>Multiplayer: Network simulator works again.</li>
<li>NavMesh: Fixed the tile carving algorithm so that it's capable of handling colinear degenerate triangles. This was causing the generated NavMesh to have a double line on polygon and was causing a trembling movement for its associated GameObject.    (905335)</li>
<li>Networking: Fixed possible crash on old Android devices due to alignment problems. Note: this change breaks protocol compatibility with previous 5.6.x builds. You need to recompile and redeploy existing 5.6 projects and builds (5.5.x and older should work without problem). </li>
<li>OSX: Unity no longer destroys RenderTexture when switching the Standalone player between fullscreen and windowed.    (902663)</li>
<li>Particles: Correctly initialize default curves, when creating new Particle Systems.  (907449) </li>
<li>Particles: Fixed a crash on certain Android hardware caused by zero sized particles. (896001) </li>
<li>Particles: Fixed an occasional crash when emitting from a skinned mesh renderer shape.   (907277) </li>
<li>Particles: Fixed incorrect values for emission burst min and max when upgrading from an older Unity version.  </li>
<li>Particles: Fixed performance regression causing Update Jobs to be dispatched slowly on some platforms.   (904810) </li>
<li>Performance Reporting: Fixed an issue where native symbols for iOS builds were not uploaded when building on OSX Sierra. (916515) </li>
<li>Physics 2D: Fixed an issue where ContactFilter2D collision normal limits failed. (912158) </li>
<li>Physics 2D: Fixed an issue with Raycast not always detecting a CapsuleCollider2D or a BoxCollider2D. (917323) </li>
<li>Physics: Do not show missing Effector2D warning in Collider2D inspector when the Collider2D is using a CompositeCollider2D.  (907407) </li>
<li>Physics: Fixed a crash that happened when continuously scaling a MeshCollider while activating and deactivating it at the same time. (878740) </li>
<li>Physics: Fixed a crash that happened when scaling a Mesh that the physics system (PhysX) failed to process properly (like a convex MeshCollider with too many vertices). (892396) </li>
<li>Physics: Fixed a crash that occurred while updating active skinned Meshes.   (845868) </li>
<li>Physics: Fixed a crash when removing a CompositeCollider2D.  (907157) </li>
<li>Physics: Fixed a crash where contacts for Collider2D were not deleted correctly. (912024) </li>
<li>Physics: Fixed an issue where contacts between Effectors were not correctly evaluated when Effector Collider masks were used.    (901950) </li>
<li>Physics: Fixed an issue where Physics.ComputePenetration and Physics.ClosestPoint were not returning the correct value when a rotated Collider had its centre offset.    (865250) </li>
<li>Physics: Fixed an issue where unexpected trigger events were fired to scripts when a degenerate CapsuleCollider was used.    (701504) </li>
<li>Physics: Fixed an issue with Raycast not always detecting an EdgeCollider2D when attached to a Rigidbody2D in certain poses. (916478) </li>
<li>Scene Management : Fixed an issue where objects marked as 'DoNotDestroyOnLoad' and are disabled could be deleted on scene load/unload    (792933) </li>
<li>Shaders: Applied improvements to Metal shaders performance when using GroupMemoryBarrier().</li>
<li>Shaders: Fixed an incorrect shader translation to GLSL and Metal shader code from a logical OR on boolean vectors. Fixed shader compile errors on Vulkan eg "Shader error in 'Hidden/Post FX/Screen Space Reflection': '' : compilation terminated at line 141 (on vulkan)". (901719) </li>
<li>Shaders: Fixed an incorrect shader translation to GLSL and Metal shader code from unsigned divide operation.</li>
<li>Shaders: Prevent assert failures and crashes when attempting to compile tessellation or geometry shaders on platforms where they're not supported.   (891914)</li>
<li>Shaders: Vulkan added support for vector scalar expansion constructors. Fixed crashes with errors like "SymGetSymFromAddr64 error: 'Attempt to access invalid address.'" (898850) </li>
<li>UGUI: Fixed crash issues when re-parenting inactive GameObjects. (898809) </li>
<li>UI: Fixed an issue where UI Button didn’t update its SelectionState after interactable value changes.    (908073)</li>
<li>UI: Removed the extra call to CanvasRenderer.OnTransformChanged when the canvas is set to ScreenSpace.Camera render mode, and the Camera’s Transform is changed. (886258) </li>
<li>Video: Added support for transcoding to tiny VP8 resolutions.    (900524) </li>
<li>Video: Fixed an intermittent failure to load video tracks on iOS.    (898171) </li>
<li>Video: Fixed crash on Samsung Android devices with 4.1 OS when stopping playback.    (907048)</li>
<li>Video: Fixed failing VP8 transcode on Windows due to unsupported audio codec.    (904924) </li>
<li>Video: Fixed invalid video stride evaluation.    (906044) </li>
<li>Video: Fixed issue on Android where H.264 videos above 480p crash on devices with 4.1 OS and Adreno 203 graphics.    (907049)</li>
<li>Video: Fixed issue on Android where VP8 videos would not play on Samsung devices with 4.2 or 4.4 OS. (907051)</li>
<li>Video: Fixed issues regarding video looping/end detection.   (909020) </li>
<li>Video: On Android, applied a fix to prevent garbage collection from being over-used, and fixed an issue where the app would freeze when changing a video clip during playback.   (905282)</li>
<li>VR: Added support for different eye texture color formats on Oculus Rift.</li>
<li>VR: Enabled termination of Cardboard applicaiton when pressing the &lt;- button during the splash screen.    (911205)</li>
<li>VR: Fix for Android not being able to change AA (Anti-Aliasing) settings at runtime. (896253) </li>
<li>VR: Fixed iOS crash in SetTexture() with Google VR SDK 1.2.  (891965) </li>
<li>VR:Ffix for VR on PC doesn't render if rendertexture format RGB565 is created, crash possible.   (899030)</li>
<li>WebGL: Fixed AudioSource.time return value.  (904578) </li>
<li>WebGL: Fixed custom cursor support.  (905625) </li>
<li>WebGL: Fixed IE InvalidStateError load-time error.   (903767) </li>
<li>WebGL: Fixed Profiler connection.    (901252) </li>
<li>WebGL: Fixed Template Custom tags not being replaced at build time.  (903092) </li>
<li>WebGL: Fixed unresponsiveness when loading cashed AssetBundles with WWW.LoadFromCacheOrDownload. (895810)</li>
<li>WebGL: Fixed WebAssembly build failure with Full exceptions on Windows.  (892185) </li>
<li>WebGL: Fixed WebAssembly missing setTempRet function.    (897782) </li>
<li>WebGL: Fixed WebAssembly missing setThrow function.  (891835) </li>
<li>WebGL: Fixed WebAssembly runtime error: integer overflow/unrepresentable.    (891431) </li>
<li>WebGL: Released WebCam after use so other tabs can use it.   (898210) </li>
<li>Windows Store: Fixed a crash when animating scripting objects on .NET scripting backend. (899087) </li>
<li>Windows Store: Fixed a crash which happened when retrieving WheelHit.Collider after having previously set it to null on .NET scripting backend.  (871541) </li>
<li>Windows Store: Fixed a harmless assert which happens when building for Universal 8.1 SDK.    (903232)</li>
<li>Windows Store: Fixed a potential stack overflow when building a project with a large custom cursor.  (909977) </li>
<li>Windows Store: Fixed an out of bounds array access assert in Mesh code.  (866141) </li>
<li>Windows Store: Fixed Build &amp; Run with VS2017.    (897807) </li>
<li>Windows Store: Fixed building player when some files (like UnityOverwrite.txt, WSATestCertificate.pfx, project.lock.json) are set to read-only.  (888029) </li>
<li>Windows Store: Fixed exceptions thrown in OnGUI callback not being logged on .NET scripting backend. (914797) </li>
<li>Windows Store: Fixed IL2CPP not being able to build C++ code with VS 2017 Update 2.  (916281) </li>
<li>Windows Store: Fixed issue where Ctrl+C would delete input field instead of copying it.  (881845) </li>
<li>Windows Store: Fixed issue where pasting an item in the InputField always pastes the item that was first in the clipboard before launching the player.   (880362) </li>
<li>Windows Store: Fixed issue where pressing and holding Xbox One controller button A led to false keydown events during the first frame of a Scene.    (875834) </li>
<li>Windows Store: Fixed serialization when a serializable type derives from another serializable type in another assembly that has a serializable private field.    (892653) </li>
<li>Windows Store: Fixed System.Numerics.dll not being referenced by scripts when using IL2CPP scripting backend.    (912074) </li>
<li>Windows Store: Fixed UNetWeaver crashing when using .NET 4.6 API Compatibility level with IL2CPP scripting backend when deriving from .NET 4.6 specific types.   (909703) </li>
<li>Windows Store: Fixed WorldAnchorStore.GetAsync crashing the player.  (902234) </li>
</ul>

#### Revision: a2913c821e27
