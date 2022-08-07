# Unity 2017.2.1
https://unity3d.com/unity/whats-new/unity-2017.2.1

## Fixes

<ul>
<li>XR: Fixed background rendering in ARCore apps running on Pixel XL no longer appearing stretched.</li>
<li>XR: Fixed issues with using values other than 1.0 for eyeTextureResolutionScale on Windows MR.</li>
<li>2D: Fixed crash when Sprite Atlas scale results in a non-power-of-two texture and Crunch Compression is enabled. (960808, 953058)</li>
<li>2D: Fixed ReflectionTypeLoadException from TilePalette when TilePalette is opened with 4.6 .Net and a user assembly cannot be loaded. (952556)</li>
<li>2D: Fixed SetMinMax for Bounds/RectInt.</li>
<li>2D: Fixed SortingGroup not applying sorting changes when child objects are duplicated or added dynamically.</li>
<li>2D: Fixed switching platform and building project without making any changes will not cause Sprite Atlas asset to change. (968721)</li>
<li>2D: Fixed the generation of Sprite Physics Shape for Sprites when the Texture is set to multiple Sprites mode, has no user Sprite Physics Shape set and does not generate a tight mesh for the Sprite.</li>
<li>2D: Fixed tiled sprite renderer crash when a sprite is being packed in a Sprite Atlas which is not included in the build. (960807, 954812)</li>
<li>2D: Fixed Tilemap Move to show correct Move preview. (952529)</li>
<li>2D: Fixed TilemapRenderer showing tiles when Tilemap.ClearAllTiles() is called. (951514)</li>
<li>2D: Fixed updating an active Tilemap palette prefab not exposing it into the SceneView. (947462)</li>
<li>AI: Fixed NavMesh.SamplePoint failing for meshes in range when another navmesh was below the point and out of range. (935433)</li>
<li>AI: Fixed unwanted gap in the NavMesh produced by a concave edge crossing a tile boundary. (930830)(959526)</li>
<li>Android: Disable GPU fences for two Android 6 devices which have been found to have compatibility issues causing performance loss: HTC 10 and LG G5 SE. (924891)</li>
<li>Android: Fixed a player crash caused by enabling GPU profiling when the selected graphics API was not OpenGL ES 3. (946913, 944118)</li>
<li>Android: Fixed android build failing with target SDKs 21-23. (956658)</li>
<li>Android: Fixed android video player playback starting to lag after activating input field. (934841)</li>
<li>Android: Fixed android video player stuttering and dropping frames. (931038)</li>
<li>Android: Fixed crash on some Adreno devices. (961094)</li>
<li>Android: Fixed crash while processing input during destruction. (934782)</li>
<li>Android: Fixed loading player data for very specific file sizes/content. (959908)</li>
<li>Android: Fixed plugin importer architecture selection. (963291)</li>
<li>Android: Fixed project export overwriting res/ directory when exporting to keep local changes to layouts etc. intact.</li>
<li>Android: Fixed realtime HDR reflection probes being black on older Android devices. (776875)</li>
<li>Android: Fixed setting multiple response headers with same name in UnityWebRequest. (944091)</li>
<li>Android: Fixed shader compile error on devices not supporting GL_FRAGMENT_PRECISION_HIGH.(945953)</li>
<li>Android: Fixed symbols.zip not including symbols file. (942625)</li>
<li>Animation: Fixed an issue where PrepareFrame was called at the wrong moment in the frame. (927919)</li>
<li>Animation: Fixed assert in play mode when Culling Type is set to "Based on Renderers". (943954)</li>
<li>Animation: Fixed assert when loading AnimationClip asynchronously in AssetBundles. (964932, 943438)</li>
<li>Animation: Fixed being unable to set the transition time in Animator.CrossFade(). (941945)</li>
<li>Animation: Fixed bool property not properly restored to initial value when exiting animation window. (948768, 947491)</li>
<li>Animation: Fixed case where sprite and material reference were not animatable at the same time in the SpriteRenderer. (945292)</li>
<li>Animation: Fixed case where transition between animations makes GetIKRotation and GetIKPosition returned incorrect value. (945035)</li>
<li>Animation: Fixed CurveField not updating animation curve when reference changes from render to render. (952170)</li>
<li>Asset Import: Fixed psd import issue where a psd looked different from a png. (931359, 931267)</li>
<li>AssetDatabase: Fixed an issue where AssetDatabase.GetSubFolders() didn't return any results, and updated the manual to reflect that this method only accepts relative paths. (931944)</li>
<li>Build Pipeline: Fixed a crash in BuildReporting::BuildReport::BeginBuildStep caused when BuildAssetBundles was being called from an OnPreprocessBuild callback. (941192, 958237)</li>
<li>Build: Exceptions in OnPreProcessBuild will now halt the build process correctly. (942296)</li>
<li>Collab: Fixed project manifest not being tracked in Collab. (951350)</li>
<li>DirectX 12: Fixed a crash when running on Windows 7 machine with first API in the list being DX12 and Graphics Jobs enabled. (964073)</li>
<li>DX12: Fixed memory leak when rendering procedurally generated meshes while using the Direct3D12 graphics API in the Windows Standalone build. (956272)</li>
<li>Editor: Fixed an issue where lightmaps are generated even though the scene does not contain any baked light contribution. (926559)</li>
<li>Editor: Fixed crash when dragging component without managed instance to hierarchy. (950172)</li>
<li>Editor: Fixed crash while processing input during destruction. (946958)</li>
<li>Editor: Fixed curve WrapModeIcon drawing when the Curve window is embedded into another window. (947024)</li>
<li>Editor: Fixed editor restart prompt when selecting the same Active Input Handling option. (968535)</li>
<li>Editor: Fixed importing a cubemap with invalid metafile crashing. (905397, 918819)</li>
<li>Editor: Fixed incorrect framing of GameObject hierarchies in Scene View. (957525)</li>
<li>Editor: Fixed incorrect tool placement when pivot mode was set to Center. (962721)</li>
<li>Editor: Fixed incorrect wrap icon button in particle curve editor window. (947024)</li>
<li>Editor: Fixed issue where performing a drag and drop operation to a GameObject that is being edited in the Preview window of Timeline would apply changes to its associated Prefab that cannot be reverted. (961428, 925381)</li>
<li>Editor: Fixed player settings not using the default icon if non are specified. (953161)</li>
<li>Editor: Fixed Plugin Inspector showing only one option in Framework Dependencies when switching to iOS platform and .NET 4.6. (948326, 930624)</li>
<li>Editor: Fix random hangs during Editor startup. (945607)</li>
<li>Editor: Fixed Scene view picking sometimes not selecting the topmost object. (943051)</li>
<li>Editor: Fixed SceneView bounds calculations not taking multiple colliders and renderers into account when calculating the framing and centre - point. (953301)</li>
<li>Editor: Reduced size of LightingDataAsset when baking light probes with multiple scenes loaded. (913869)</li>
<li>GI: Fix a crash in ApplyMaterialPassWithCache when generating lighting and Lightmap Static option is enabled. (946517)</li>
<li>GI: Fixed 'Show Lightmap Resolution' checkbox not working. (956577)</li>
<li>GI: Fixed crash when deleting Speedtree asset files from project folder when in use by prefab.</li>
<li>GI: Fixed Enlighten not generating lightmaps for meshes imported without UVs and with Generate Lightmap UVs option enabled. (854349)</li>
<li>GI: Fixed MaterialPropertyBlock values for Meta pass when using on terrain mesh with Realtime GI. (935149)</li>
<li>GI: Fixed navigating in scene view restarting baking when trees are painted on terrain. (955739, 955667)</li>
<li>GI: Fixed shadows when shadow prepare job is not run. (930221)</li>
<li>GI: Fixed terrain artifacts caused by Enlighten terrain mesh triangulation being different from the original mesh triangulation. (754298)</li>
<li>GI: Fixed terrain trees do not casting shadows into baked lightmaps. (685764)</li>
<li>GI: Fixed the UI in inspector not correctly showing light mode when multiple lights are selected. (851817, 929875)</li>
<li>Graphics: Added error message for graphics APIs that do not support texture wrap mode "mirror once" (Android Vulkan, Android GLES3 and WebGL). (912323)</li>
<li>Graphics: Emit error messages instead of assert when the screen position is out of view frustum.(947342)</li>
<li>Graphics: Fix Vulkan validation layer errors (on Windows) when switching to fullscreen. (941149)</li>
<li>Graphics: Fix Vulkan validation layer errors associated with image barriers.</li>
<li>Graphics: Fixed a crash in 'RenderTexture::DiscardContents' when opening the scene. (935328)</li>
<li>Graphics: Fixed an issue where an off-screen SkinnedMeshRenderer with 'update when off-screen' enabled was not being skinned. (939897)</li>
<li>Graphics: Fixed asserts when animations disable newly visible renderers. (950215)</li>
<li>Graphics: Fixed atlased ETC1 textures with split alpha rendering in editor outside of play mode. (942923)</li>
<li>Graphics: Fixed batching with unused stencil bit in G-Buffer pass. (962696)</li>
<li>Graphics: Fixed crash when certain variables of CustomRenderTexture are used in script. (942563)</li>
<li>Graphics: Fixed crash when creating sprite with unsupported texture format. (944413)</li>
<li>Graphics: Fixed culling of projectors not matching Editor scene cameras. (954828)</li>
<li>Graphics: Fixed D3D11 driver assert message and potential crash "Invalid mask passed to GetVertexDeclaration() when using post-effect". (932940)</li>
<li>Graphics: Fixed exception being thrown when the backgroung color of a Reflection Probe is changed. (939947)</li>
<li>Graphics: Fixed GL_INVALID_ENUM error with OpenGL ES when using point primitives.</li>
<li>Graphics: Fixed incorrect calculation of the Umbra occlusion culling near plane from the camera settings. (840098)</li>
<li>Graphics: Fixed incorrect definition of _ShadowCoord in AutoLight.cginc leading to unexpected compilation errors or extra useless interpolator. (924464)</li>
<li>Graphics: Fixed issue where some user shader keywords were handled incorrectly leading to compilation errors when building for standalone. (944334)</li>
<li>Graphics: Fixed not being able to set any Mesh on a Skinned Mesh Renderer. (946068)</li>
<li>Graphics: Fixed object with "Dynamic Occludee" property being disabled rendering in Preview window when selecting a different object. (944223)</li>
<li>Graphics: Fixed potential hang with DirectX11 or DirectX12 when using different sized render targets and multiple cameras. (950907)</li>
<li>Graphics: Fixed project build errors when Reflection Probes Projection setting in Tier1(Graphics Settings) is unchecked. (925552)</li>
<li>Graphics: Fixed specific case where not all requested shader variants ending up in an asset bundle. (948053)</li>
<li>Graphics: Fixed Tree shadows being culled when zoomed in on Occlusion Visualization mode. (941334)</li>
<li>Graphics: Fixed updating of bounding boxes for SkinnedMeshRenderers with 'Update When Offscreen' set. (935463)</li>
<li>Graphics: MeshRenderers with disabled "Dynamic Occluded" property were not being frustum culled. (956877)</li>
<li>IL2CPP: Added support in IL2CPP for Module.ScopeName property, which is used by Assembly.GetModule() to find a module in an assembly by name. (947807)</li>
<li>IL2CPP: Fixed an exception that would occur during conversion when processing an exception filter that calls a method. (944157)</li>
<li>IL2CPP: Fixed ArgumentException when accessing Socket.LocalEndPoint. (943671)</li>
<li>IL2CPP: Fixed calling DateTime.Parse() in IL2CPP builds for UWP throwing IndexOutOfRangeException. (948887)</li>
<li>IL2CPP: Fixed calling native ICommand interface methods on managed and native objects.</li>
<li>IL2CPP: Fixed calling System.Collections.Generic.IList`1 methods on managed and native objects.</li>
<li>IL2CPP: Fixed crash in thread pool during shutdown. (966623)</li>
<li>IL2CPP: Fixed crash when calling Socket.GetSocketOption using latest scripting runtime. (952043)</li>
<li>IL2CPP: Fixed marshaling System.DateTimeOffset to Windows.Foundation.DateTime when passing it to Windows Runtime APIs. (950465)</li>
<li>IL2CPP: Fixed SetSocketOption not working properly for add membership and remove membership with IPv6. (944939)</li>
<li>IL2CPP: Fixed stack overflow from occurring in Unity liveness logic (asset GC). (935563)</li>
<li>IL2CPP: Fixed unimplemented COM related internal calls in System.Runtime.InteropServices.Marshal class. (930386)</li>
<li>IL2CPP: Implemented a previously unimplemented internal call method to support System.Environment.HashShutDownStarted property. (947420)</li>
<li>IL2CPP: Improved stack traces for NullReferenceException cases on iOS when Xcode 8.3.1 or later is used with release builds. (950637)</li>
<li>IL2CPP: Prevented an intermittent crash in the GC for on PS4. (955991)</li>
<li>iOS: Fixed an issue where the development team ID was not written to the Xcode project in manual signing mode. (966830)</li>
<li>iOS: Fixed crash in Handheld.PlayFullScreenMovie when playback ends. (949361)</li>
<li>iOS: Fixed screen not always automatically rotating correctly after disabling and enabling auto-rotation. (942401)</li>
<li>iOS: Fixed support for fonts of Tibetan, Armenian, Braille, Georgian and Thai languages in iOS 10 and iOS 11. (951089, 949036)</li>
<li>iOS: Fixed support of wide colors on new devices. (955685)</li>
<li>iOS: Fixed SystemInfo.supportedRenderTargetCount not correctly returning 8 for devices that support it. (949032)</li>
<li>iOS: Fixed the Screen.dpi() method in the Trampoline code not returning the correct number of DPI in iPhone 8, iPhone 8+ and iPhone X. (962793, 960914)</li>
<li>Lighting: Fixed asset bundles not working correctly with global illumination data. (924597)</li>
<li>Lighting: Fixed issue where Progressive Lightmapper was not transmitting indirect rays through translucent objects. (887019)</li>
<li>Lighting: Fixed maximum lightmap import size. (847499)</li>
<li>Multiplayer: Fixed reliable message being delivered twice.</li>
<li>OSX: Fixed Editor crash when using GLCore on High Sierra with Intel 6xxx series GPU. (963865)</li>
<li>OSX: Fixed High Sierra OS freeze while using Local Cache Server. (954747)</li>
<li>OSX: Fixed incorrect mouse position when running in full screen and non-native aspect ratio. (944450) (964731)</li>
<li>OSX: Metal: Fix hang when using MSAA on OSX 10.11 on Nvidia GPUs. (963059)</li>
<li>Package Manager: Fixed creation of empty folder named 'etc'.</li>
<li>Package Manager: Fixed error/crash if there is a comma symbol in the project name. (957436)</li>
<li>Package Manager: Fixed initialisation failure when host file is missing or empty. (957000)</li>
<li>Particles: Fixed Birth SubEmitter not always firing when using random between two constants lifetime. (941076)</li>
<li>Particles: Fixed burst curves on new particle systems not being initialized. (956592)</li>
<li>Particles: Fixed issue with incorrect bounds calculation causing incorrect culling in rare cases. (956753)</li>
<li>Particles: Fixed scripted emission emitting particles in the wrong direction, if transform was moving/rotating. (957633)</li>
<li>Physics: Ensure that we correctly match enter/exit collision/trigger callbacks when a single simulation step causes a contact to stop then start again. (932044)</li>
<li>Physics: Ensured that 'Collision2D.GetContacts()' returns a single contact when passing a single element array. (967740)</li>
<li>Physics: Ensured that loading a scene with a Rigidbody2D with simulation off allows interpolation when simulation is subsequently turned on. (965605)</li>
<li>Physics: Ensured that manual transform sync correctly updates the Rigidbody2D pose correctly. (963200)</li>
<li>Physics: Fixed cloth pointer not being set to null to null in SkinnedMeshRenderer when deactivating causing attempted use of deallocated object. (946356)</li>
<li>Physics: Fixed Collider2D crashing when disabled by an animation. (957044)</li>
<li>Physics: Fixed Collider2D material changes not being propagated to existing contacts. (953653)</li>
<li>Physics: Fixed colliders missing pose updates when they were inactive during the scene load. (945332)</li>
<li>Physics: Fixed physics settings being always marked as dirty on the editor start, even when nothing was changed. (948866)</li>
<li>Physics: Fixed PlatformEffector2D not ignoring contacts involving trigger colliders. (950833)</li>
<li>Physics: Fixed previously ignored collision not being ignored when recreating 2D physics contacts. (960530)</li>
<li>Physics: Fixed RigidBody2Ds being woken when set to "StartAsleep" sleep mode. (941024)</li>
<li>Physics: Fixes GameObject which has a disabled cloth component not following parent's transform. (946307)</li>
<li>Playables: Fixed crash when setting an invalid source playable. (956316)</li>
<li>Plugins: Fixed warning messages about Audio spatializers in logs for applications that were not using spatializers. (869346, 835980)</li>
<li>Prefabs: Fixed issue where resetting SerializedProperty.prefabOverride for one property could incorrectly reset other properties. (960775)</li>
<li>Scripting: Fixed alignment of 64-bit types on iOS. (949127)</li>
<li>Scripting: Fixed Awake containing the wrong transform values when instantiated. (953068)</li>
<li>Scripting: Fixed crash if delegate is created on un-inflated generic type. (763091)</li>
<li>Scripting: Fixed crash in debugger when trying to stop while a single step operation is in progress. (951901)</li>
<li>Scripting: Fixed crash on OSX when socket error ENXIO is encountered. (944464)</li>
<li>Scripting: Fixed crash when closing Windows Standalone player with Alt-F4 using latest scripting runtime. (952292)</li>
<li>Scripting: Fixed crash when struct has array field of same type. (807575)</li>
<li>Scripting: Fixed startup-crash on macOS 10.13 when using multiple monitors. (958250, 955089)</li>
<li>Scripting: Fixed XMM registers being trampled in 64-bit mode. (952069)</li>
<li>Shaders: Disable instancing support when performing surface shader analysis. (935126l, 941827)</li>
<li>Shaders: Fixed HLSLcc shader conversion not handling F32TO16 and F16TO32 opcodes.</li>
<li>Shaders: Fixed importing a shader include file only clearing the include cache on a single shader compiler process leaving all the other processes with outdated include files in the cache.</li>
<li>Shaders: Fixed incorrect translation of shaders using resinfo with mask operators. (943340)</li>
<li>Shaders: Fixed incorrect translation to GLSL of compute shaders using bfi instructions with mask operators. (927339)</li>
<li>Shaders: Fixed shadow precision for mobile platforms. (951875, 899729)</li>
<li>Terrain: Fixed crash when loading a non read/write enabled texture from an asset bundle. Texture will not be shown unless it is marked as read/write. (951780)</li>
<li>Timeline: Fixed crash when deleting animation track which has a binding attached to an ActivationTrack. (956129)</li>
<li>Timeline: Fixed timeline window having a white background when running on .NET 4.6 depending on the set system language. (960039, 938534)</li>
<li>tvOS: Fixed icon asset catalog setup when certain multi-layer icons are missing. (959867)</li>
<li>UI: Fixed many bugs/performance problems caused by driven properties in uGUI by reverting to the 2017.1 driven property system.</li>
<li>UI: Fixed RectMask2D not masking when it's child has a child with Mask and Image components inside the RectMask2d area. (969932)</li>
<li>UI: Fixed 'd3d11: failed to create buffer' error in CanvasRenderer. (953270)</li>
<li>UWP: Fix building VS project after manually switching it to Windows SDK 15063 on .NET scripting backend. (940555)</li>
<li>UWP: Fixed "Run in Background" player setting not causing player to ignore minimize events. (759166)</li>
<li>UWP: Fixed an assert when trying to access missing material properties on debug builds. (945336)</li>
<li>UWP: Fixed issue where ComputeBuffer.SetData() and ComputeBuffer.GetData() returned empty result when running on .NET scripting backend and the array types weren't referenced from any parameters. (951036)</li>
<li>UWP: Fixed Reference Rewriter complaining about missing operators == and != on System.Type on .NET scripting backend. (955651)</li>
<li>UWP: Fixed StateMachineBehaviour not working on private fields before loading any scenes on .NET scripting backend. (937501)</li>
<li>UWP: Fixed Unity not referencing facade class libraries when targeting UWP and using IL2CPP with .NET 4.6 API Compatibility level. (949209)</li>
<li>Video: Fixed clip from asset bundle not played. (964652)</li>
<li>Video: Fixed crash in VideoPlayer when stopping and callbacks were pending.</li>
<li>Video: Fixed crashing RemoteWebCamTexture (when using the Unity Remote helper app) when marked DontDestroy. (973008)</li>
<li>Video: Fixed editor crash when previewing/playing video on older OSX version. (973005)</li>
<li>Video: Fixed erroneous stride crash on Windows. (966690)</li>
<li>Video: Fixed inspector preview not cropping title. (969299) (937173)</li>
<li>Video: Fixed muting game view does not mute video audio. (969297)</li>
<li>Video: Fixed video decoding errors due to bad file I/O for high res/bitrate video. (962204)</li>
<li>Video: Fixed video not playing in build when building for another platform. (969298)</li>
<li>Video: Fixed Video Player component rendering video with artifacts on OSX. (973009)</li>
<li>Video: Fixed VideoPlayer CameraNear/FarPlane RenderModes when used in conjunction with VR.</li>
<li>VR: Fixed incorrect stereo eye offsets in Windows Mixed Reality.</li>
<li>Web: Fixed POST key/value dictionary containing very long values in UnityWebRequest. (946124)</li>
<li>Web: Fixed WWW.responseHeaders returning null. (949038)</li>
<li>WebGL - Fixed missing logo/progress bar during loading screen. (900105)</li>
<li>WebGL: Fixed divide by zero when AudioSource.pitch is zero. (946393)</li>
<li>WebGL: Fixed missing slash in WebRequest formatted blob url when using https. (940942)</li>
<li>WebGL: Fixed MS Edge detection. (943241)</li>
<li>WebGL: Fixed Timeline crash on missing DSPConnection::setMix(). (949858)</li>
<li>Windows: Fixed DictationRecognizer asserting when stopping or starting the speech recognition twice in a row. (918146)</li>
<li>Windows: Fixed loading animation on cursor continuing to play after the game is loaded. (860330)</li>
<li>Windows: Fixed ProcessMouseInWindow causing CPU spikes up to 4ms on Standalone builds. (931829)</li>
<li>Windows: Fixed Windows touch input events being out of sync from positioning events. (899209)</li>
<li>WWW: Fixed reading of local files not working in UWP with UnityWebRequest. (910488)</li>
<li>WWW: Fixed WWW class regressions related to throwing NullReferenceException (949418)</li>
<li>XR: Added back Stereo Display (non head-mounted).</li>
<li>XR: Camera transform changes during and after tracking loss now mimics other platforms' behavior. (949193)</li>
<li>XR: Eliminated errors and warnings showing per frame in console during Holographic Emulation. (943109)</li>
<li>XR: Fix Podfile version to reflect correct version. (962253)</li>
<li>XR: Fixed a performance regression on Microsoft HoloLens. (959749)</li>
<li>XR: Fixed a rendering issue on Windows Mixed Reality when using multiple cameras with different depth ranges. (927404, 953255)</li>
<li>XR: Fixed an issue with blitting between VR and non-VR render textures.</li>
<li>XR: Fixed Assert when playing Mixed Reality applications in Editor without Mixed Reality Portal running. (950519)</li>
<li>XR: Fixed black screen on startup on Cardboard when GLES2 or GLES3 is used. (931397)</li>
<li>XR: Fixed camera aspect ratio not being preserved when switching from VR to non-VR. (892084)</li>
<li>XR: Fixed crash in Editor when toggling play mode aftering blooming to shell on Windows Mixed Reality. (948814)</li>
<li>XR: Fixed Daydream applications hanging before quiting to Android home when calling Application.Quit. (966173)</li>
<li>XR: Fixed forcing LandscapeLeft default Orientation on all mobile VR applications.</li>
<li>XR: Fixed Holographic Simulation not working in Editor. (952039)</li>
<li>XR: Fixed incorrect culling when using multiple cameras with Windows Mixed Reality. (927404)</li>
<li>XR: Fixed issue with "Unsupported texture format .." warnings appearing when XR is enabled. (956693)</li>
<li>XR: Fixed issue with being able to set tracking space type to Stationary. (946714)</li>
<li>XR: Fixed landscape left being forced when landscape right is disabled. (946829)</li>
<li>XR: Fixed stereo separation regression on Oculus HMDs.</li>
<li>XR: Fixed stretched background image for ARCore apps running on Samsung S8.</li>
<li>XR: Fixed Windows Mixed Reality applications not reporting an updated boundary if it has been reconfigured while the app was running.</li>
<li>XR: Fixed Windows Mixed Reality apps rendering with incorrect eye offsets. (963878)</li>
<li>XR: Fixed Windows Mixed Reality XAML apps launching to a black screen. (954629)</li>
<li>XR: Fixed Windows Mixed Reality XAML apps not able to get back to exclusive mode after blooming to the shell. (953314)</li>
<li>XR: Fixed Windows Mixed Reality XAML apps not rendering on desktop. (922492)</li>
<li>XR: InputTracking.Recenter is now hooked up properly on Windows Mixed Reality. (909869)</li>
<li>XR: Removed some unnecessary graphics API state resets.</li>
<li>XR: Tracking loss screen no longer appears on WindowsMR headsets, now mimics the behavior of other platforms during tracking loss. (942154)</li>
<li>XR: Tracking space type now falls back to Stationary when boundary hasn't been configured. (945163)</li>
<li>XR: Updated the code to invalidate the eye texture's depth and stencil in one call.</li>
<li>XR: Updated messaging in XR Settings for Android applications attempting to use Daydream and Oculus.</li>
</ul>

#### Revision: 94bf3f9e6b5e
