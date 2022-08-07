# Unity 2017.1.3
https://unity3d.com/unity/whats-new/unity-2017.1.3

## Fixes

<ul>
<li>AI: Fixed NavMesh.SamplePoint failing for meshes in range when another navmesh was below the point and out of range. (935433)</li>
<li>AI: Fixed an unwanted gap in the navigation mesh produced by a concave edge crossing a tile boundary. (930830)</li>
<li>Android: Fixed an issue where "Success" message was shown on failed builds. (934735)</li>
<li>Android: Fixed a rare static splash screen crash. (971571)</li>
<li>Android: Fixed crash on some Adreno devices. (961094 (948200)</li>
<li>Android: Fixed loading player data for very specific file sizes/content. (959908)</li>
<li>Android: Disable GPU fences for two Android 6 devices which have been found to have compatibility issues causing performance loss: HTC 10 and LG G5 SE. (924891)</li>
<li>Android: Fixed symbols.zip not including symbols file. (942625)</li>
<li>Android: Fixed android video player playback starting to lag after activating input field. (934841)</li>
<li>Android: Fixed stuttering with android video player multithreaded rendering. (931038)</li>
<li>Android: Fixed android build failing with target SDKs 21-23. (956658)</li>
<li>Android: Fixed realtime HDR reflection probes being black on older Android devices. (776875)</li>
<li>Android: Fixed player crash when profiler with GPU profiling is enabled and graphics API was not OpenGL ES 3. (944118)</li>
<li>Android: Fixed header availability in UnityWebRequest on Android when response uses chunked transfer. (956599)</li>
<li>Android: Fixed crash when killing the application during permission request. (934782)</li>
<li>Android: Fixed an issue where apk signing would fail when using certain symbols in the passwords. (946291,941214)</li>
<li>Android: Fixed corrupted textures with mip maps on phones with VideoCore gpus. (913546)</li>
<li>Animation: Fixed assert when loading AnimationClip asynchronously in AssetBundles. (964932 (943438)</li>
<li>Animation: Fixed an irrelevant assert in Animation Component. (943954)</li>
<li>Animation: Fixed CurveField not updating animation curve when reference changes from render to render. (952170)</li>
<li>Animation: Fixed a crash when opening an animator controller with a circular reference through StateMachineBehaviours. (930354)</li>
<li>API Updater: Fixed an unnecessary reference to mscorlib 4.0 being added to assemblies in some cases. (952674)</li>
<li>Apple TV: Fixed icon asset catalog setup when certain multi-layer icons are missing. (959867)</li>
<li>Asset Import: Fixed psd import issue where a PSD looked different from a PNG. (931359)</li>
<li>Asset Pipeline: AssetDatabase.GetSubfolders now returns paths correctly, and API documentation has been updated to reflect that it takes a relative path as an argument. (931944)</li>
<li>Build: Fixed exceptions in OnPreProcessBuild halting the build process incorrectly;. (942296)</li>
<li>Build Pipeline: Fixed a crash in BuildReporting::BuildReport::BeginBuildStep caused when BuildAssetBundles was being called from an OnPreprocessBuild callback. (920537) (958238)</li>
<li>Build Pipeline: Implemented code optimization to reduce time spent entering playmode. (933679)</li>
<li>DX12: Fixed bad pipeline state issue causing errors. (925955)</li>
<li>DX12: Fixed constant buffer memory being overwritten in certain circumstances. (938617)</li>
<li>DX12: Fixed copy queue memory leak.</li>
<li>Editor: Fixed plugin Inspector showing only one option in Framework Dependencies for iOS platform and .NET 4.6. (948327 (930624)</li>
<li>Editor: Fixed command line activation failed when there is a old cached access token. (940084)</li>
<li>Editor: Fixed a crash when a cubemap with invalid metafile was imported. (905397)</li>
<li>Editor: Fixed an issue where lightmaps are generated even though the scene does not contain any baked light contribution. (926559)</li>
<li>Editor: Reduced size of LightingDataAsset when baking light probes with multiple scenes loaded. (913869)</li>
<li>Editor: Fixed editor restart prompt when selecting the same Active Input Handling option. (968535)</li>
<li>Editor: Fixed crash while processing input during destruction. (946958)</li>
<li>Editor: Fixed random hangs during Editor startup. (954607)</li>
<li>Editor: Fixed an issue where performing a drag and drop operation to a GameObject that is being edited in the Preview window of Timeline would apply changes to its associated Prefab that cannot be reverted. (964917 (925381)</li>
<li>Editor: Fixed Scene view picking sometimes not selecting the topmost object. (943051)</li>
<li>Editor: Fixed Player Settings, not using the default icon if there are no icons specified. (953161)</li>
<li>Facebook: Fixed unhandled BadImageFormatException for deleted SDK .dll. (969962 (956872)</li>
<li>Facebook: Minor fixes for upload package creation process. (950320) (950323)</li>
<li>Facebook: Fixed an incompatibility issue with Facebook SDK 7.10.1.</li>
<li>GI: Fixed project build errors when Reflection Probes Projection setting in Tier1(Graphics Settings) is unchecked. (925552)</li>
<li>GI: Fixed terrain artifacts caused by Enlighten terrain mesh triangulation being different from the original mesh triangulation. (754298)</li>
<li>GI: Fixed exception being thrown when the backgroung color of a Reflection Probe is changed. (939947)</li>
<li>GI: Fixed a crash in 'RenderTexture::DiscardContents' when opening a scene. (935328)</li>
<li>GI: Changed memory label for filtering in Progressive Lightmapper. (936003)</li>
<li>GI: Remove unnecessary error message being displayed in console. (930042)</li>
<li>GI: Fixed metadata pass values when using terrain mesh with MaterialPropertyBlock and Realtime GI. (935149)</li>
<li>GI: Fixed Enlighten not generating lightmaps for meshes imported without UVs and with Generate Lightmap UVs option enabled. (854349)</li>
<li>GI: Progressive Lightmapper crashes with transparent shader. (949574)</li>
<li>Graphics: Fixed lights on animated rigs thorwing errors and potentially crashing. (930408)</li>
<li>Graphics: Clarified behaviour for RenderTexture.autoGenerateMips specifically when using Graphics.CopyTexture. (840231)</li>
<li>Graphics: Fixed crash when creating sprite with unsupported texture format. (944413)</li>
<li>Graphics: Fixed GL_INVALID_ENUM error with OpenGL ES when using point primitives.</li>
<li>Graphics: Fixed crash when certain variables of CustomRenderTexture are used in script. (942563)</li>
<li>Graphics: Fixed atlased ETC1 textures with split alpha rendering in Editor outside of play mode. (942923)</li>
<li>Graphics: Fixed displaying incorrect light mode when multiple lights are selected. (929875)</li>
<li>Graphics: Fixed shadows when shadow prepare job is not run. (930221)</li>
<li>Graphics: Fixed batching with unused stencil bit in G-Buffer pass. (964921 (962696)</li>
<li>Graphics: Fixed OpenGL rendering to specific mip level in certain circumstances. (914192)</li>
<li>Graphics: Metal: Fix occasional GPU hangs when dispatching compute shader. (950989)</li>
<li>Graphics: Fixed an issue where performing an undo on a Static Lightmap Object causes an error related to transforms to be reported. (955082)</li>
<li>Graphics: Fixed an issue where off-screen SkinnedMeshRenderer with 'update when off-screen' enabled not being skinned. (939897)</li>
<li>Graphics: Fix startup crash on OS X 10.11 with Metal.</li>
<li>Graphics: Fixed updating of bounding boxes for SkinnedMeshRenderers with 'Update When Offscreen' set. (935463)</li>
<li>Graphics: Import Settings: Fixed changing texture type to Normal map not resetting existing alphaIsTransparency setting. (935870)</li>
<li>Graphics: Added GL support to be able to bind sRGB textures as RWTextures i.e. for compute shaders in linear rendering mode. (891510)</li>
<li>Graphics: Fixed "Assertion failed: 'IsNormalized(normal)'" when computing spotlight frustum planes. (922769)</li>
<li>Graphics: Fixed asserts when animations disable newly visible renderers. (950215)</li>
<li>IL2CPP: Fixed incorrect the behavior of DateTime.TryParse with the .NET 4.6 profile. (948887)</li>
<li>IL2CPP: Fixed an intermittent crash in the garbage collector on PS4. (955991)</li>
<li>IL2CPP: Improve stack traces for NullReferenceException cases on iOS when Xcode 8.3.1 or later is used with release builds. (950637)</li>
<li>IL2CPP: Adding support in IL2CPP for Module.ScopeName property, which is used by Assembly.GetModule() to find a module in an assembly by name. (947807)</li>
<li>IL2CPP: Fixed calling native ICommand interface methods on managed and native objects.</li>
<li>IL2CPP: Fixed marshaling System.DateTimeOffset to Windows.Foundation.DateTime when passing it to Windows Runtime APIs. (950465)</li>
<li>IL2CPP: Fixed crash in thread pool during shutdown. (966623)</li>
<li>IL2CPP: Improve incremental build performance on OSX.</li>
<li>IL2CPP: Fixed crash when calling Socket.GetSocketOption using latest scripting runtime. (952403)</li>
<li>IL2CPP: Fixed ArgumentException when accessing Socket.LocalEndPoint on .NET 4.6. (943671)</li>
<li>IL2CPP: Fixed an issue where android builds would crash on launch with the 4.5 runtime when the byte code stripping option was selected. (922979)</li>
<li>Internal: Fixed some test runs returning true when calling 'IsHumanControllingUs'.</li>
<li>iOS: Fixed the Screen.dpi() method from the Trampoline code in order to return the correct number of DPI in iPhone 8, iPhone 8+ and iPhone X. Also fixed - the iPhone 8+ and iPhone X model checking. (962352)</li>
<li>iOS: Added identification enums for iPhone 8, 8+ and X.</li>
<li>iOS: Fixed a multithreading issue where downloading and aborting a lot of files was causing instabilities. (944301)</li>
<li>iOS: Fixed screen not rotating away when disabling current autorotation using Screen.autorotateTo. (972893 (942401)</li>
<li>iOS: Fixed PlayerSettings.iOS.appleDeveloperTeamID being ignored if automatic signing is off. (967467 (966830)</li>
<li>iOS: Fixed support for fonts of Tibetan, Armenian, Braille, Georgian and Thai languages in iOS 10 and iOS 11. (951089) (949036)</li>
<li>iOS: Added an option to disable UISystemGestureGateGestureRecognizers touch delays in the Trampoline. These delays are meant to filter out accidental - clicks very close to the edges of the screen, but some users reported that they have been experiencing - issues related to them, DISABLE_TOUCH_DELAYS flag has been added in order to control this behaviour. (920200 (878689)</li>
<li>Lighting: Fixed issue where Progressive Lightmapper was not transmitting indirect rays through translucent objects. (887019)</li>
<li>Lighting: Lightmap import max size fix added. (847499)</li>
<li>Multiplayer: Fixed reliable message sometimes being delivered twice.</li>
<li>OSX: Fixed High Sierra OS freeze while using Local Cache Server. (954747)</li>
<li>OSX: Fixed Editor crash when using GLCore on High Sierra with Intel 6xxx series GPU. (963866)</li>
<li>OSX Metal: Fixed hang when using MSAA on OSX 10.11 on Nvidia GPUs. (963060)</li>
<li>Particles: Fixed an issue whereby Box Shape changed emission direction when scaled to 0. (935633)</li>
<li>Particles: Fixed am issue where Particle System could spawn bursts twice in some situations. (934787)</li>
<li>Particles: Fixed UI errors when using Planes collision mode. (930005)</li>
<li>Particles: Fixed batching issues when using Generate Lighting Data on Particle Trails. (944029)</li>
<li>Particles: Fixed crash when emitting from script and using a Size module. (957427)</li>
<li>Particles: Fixed an issue where Horizontal billboards had an incorrect vertex normal. (944205)</li>
<li>Particles: Fixed mesh particles being rendered upside-down when using view-space. (957899)</li>
<li>Physics: Fixed cloth pointer not being set to NULL when deactivating SkinnedMeshRenderer. (946356)</li>
<li>Physics: Ensure that when a Rigidbody2D is set to "StartAsleep" sleep mode that any initial contacts do not wake it. (941024)</li>
<li>Physics: Ensure that when a Collider2D material changes, any existing contacts change to match the material properties. (953653)</li>
<li>Physics: Fixed GameObject with disabled cloth component not following parent's transform. (946307)</li>
<li>Physics: Fixed recursive 2D physics callbacks happening when re-parenting inside a callback. (965075)</li>
<li>Physics: Fixed loading a scene with a Rigidbody2D with simulation off allowing interpolation when simulation is subsequently turned on. (965605)</li>
<li>Physics: Fixed matching of enter/exit collision/trigger callbacks when a single simulation step causes a contact to stop then start again. (932044)</li>
<li>Physics: Fixed previous collision not being ignored when recreating 2D physics contacts. (960530)</li>
<li>Physics: Ensure that the PlatformEffector2D ignores any contacts involving trigger colliders. (950833)</li>
<li>Physics: Updated physics documentation to better explain how friction and bounciness are combined. (922684)</li>
<li>Physics: Fixed TerrainData.SetHeights not updating the terrain collider properly at run-time. (916451)</li>
<li>Physics: Fixed collider from crashing or getting into a bad state when disabled from an animation. (957044)</li>
<li>Plugins: Removed warning messages about Audio spatializers in logs for applications that were not using spatializers. (869346) (835980)</li>
<li>Prefabs: Fixed issue where resetting SerializedProperty.prefabOverride for one property could incorrectly reset other properties in some - circumstances. (960775)</li>
<li>Profiler: Fixed a deadlock issue when creating a profiler sampler with a duplicate name eg: Profiler.BeginSample("Destroy"). (948379)</li>
<li>Scripting: Fixed Awake containing the wrong transform values when instantiated. (953068)</li>
<li>Scripting: Fixed crash if delegate is created on un-inflated generic type. (763091)</li>
<li>Scripting: Fixed crash in debugger when trying to stop while a single step operation is in progress. (951901)</li>
<li>Scripting: Fixed alignment of 64-bit types on iOS. (949127)</li>
<li>Scripting: Fixed hang on exit in batch mode. (958346)</li>
<li>Scripting: Fixed deadlocks and pauses when using System.Threading.Monitor. (827984)</li>
<li>Scripting: Fixed crash in AssemblyUpdater when property body contains reference to an obsolete API method / property. (935582)</li>
<li>Scripting: Fixed XMM registers getting overwritten in 64-bit mode. (952069)</li>
<li>Shaders: Fixed #pragma target 4.0, 4.6, 5.0 not working on some Android devices. (933203)</li>
<li>Shaders: Added errors in UsePass/Fallback snippets as runtime errors so they get properly cleared when the source shader is updated. (920303)</li>
<li>Terrain: Fixed crash when a splat texture only has a normal map. (963350)</li>
<li>Terrain: Remove Editor error about non read/write textures. (964302)</li>
<li>Terrain: Fix crash when loading a non read/write enabled texture from an asset bundle. Texture will not be shown unless it is marked as read/write. (951780)</li>
<li>UI: Fixed issue where canvas elements that are moved whilst they're disabled weren't displayed in the correct location upon being re-enabled. (958902 (924188)</li>
<li>UI: Fixed 'd3d11: failed to create buffer' error in CanvasRenderer. (953270)</li>
<li>UI: Fixed issue with input when a zero Z scale or zero X &amp; Y scale were used. (957844)</li>
<li>UI: Fixed tabbing between input fields not properly giving editing focus. (952802)</li>
<li>Video: Fixed crash when stopping the WebGL VideoPlayer if callbacks are pending.</li>
<li>Video: Fixed erroneous negative stride crash on Windows. (966690)</li>
<li>Video: Fixed crashing RemoteWebCamTexture (when Unity Remote helper app) when marked DontDestroy. (965363 (921560)</li>
<li>Video: Video Clip is not played when loading it from an Asset Bundle on Windows. (954117) (924562)</li>
<li>Video: Muting Game View does not mute video audio. (964785) (854484)</li>
<li>Video: Fixed VideoPlayer CameraNear/FarPlane RenderModes when used in conjunction with VR. (none)</li>
<li>Video: Fixed a rash at TestAndRemoveObject when closing Unity with video preview playing. (938819)</li>
<li>Video: Fixed video decoding errors due to bad file I/O for high res/bitrate video. (962255 (908289)</li>
<li>Video: [Windows][Standalone] Fixed a crash when exiting standalone 'UnityPlayer.dll caused an Access Violation'. (942012)</li>
<li>Video: Fixed an issue whereby video Clip Preview works only in Play mode. (931846)</li>
<li>Video: Fixed a rash in mono_marshal_get_cache when reentering Play mode after video clip was previewed. (930707)</li>
<li>Video: Fixed VideoPlayer crash on OSX 10.9 and iOS 7.0 or below. (965362)</li>
<li>Video: Fixed inspector preview not cropping video files name. (964789) (937173)</li>
<li>Web: Fixed WWW.responseHeaders returning NULL. (949038)</li>
<li>Web: UnityWebRequest: Fixed POST key/value dictionary containing very long values. (946124)</li>
<li>Web: Fixed header availability in UnityWebRequest when response is HTTP failure or there is no body.</li>
<li>WebGL: Fixed Timeline crash on missing DSPConnection::setMix(). (949858)</li>
<li>WebGL: Fixed division by zero when AudioSource.pitch is zero. (946393)</li>
<li>WebGL: Fixed MS Edge detection. (943241)</li>
<li>WebGL: Fixed missing slashes in https blob url. (940942)</li>
<li>WebGL: Fixed black screen / missing progress bar during loading. (900105)</li>
<li>WebRequest: Fixed resource leak when aborting a UnityWebRequest that downloads an AssetBundle. (950574)</li>
<li>WWW: Fixed WWW class regressions related to throwing NullReferenceException. (949418)</li>
<li>XR: Fixed a thread affinity issue on certain mobile devices that could affect performance when resuming VR apps. (None)</li>
<li>XR: Fixed handling of Android density (screen resolution) changes to avoid a crash. (950540)</li>
<li>XR: Fixed camera aspect ratio not being preserved when switching from VR to non-VR. (892084)</li>
<li>XR: Fixed black screen on startup on Cardboard when GLES2 or GLES3 was used. (931397)</li>
<li>XR: Fixed Cardboard iOS target frame-rate. (950229)</li>
<li>XR: Fixed Daydream applications hanging before quitting to Android home when calling Application.Quit. (966173)</li>
<li>XR: Combined depth/stencil invalidation to work around a driver bug on some Android platforms.</li>
<li>XR: Fixed an issue with Camera.stereoSeparation being incorrectly applied on Oculus HMDs. (957488)</li>
<li>XR: Fixed Podfile not reporting the correct version. (962253)</li>
<li>XR: Fixed forcing LandscapeLeft default Orientation on all mobile VR applications.</li>
</ul>

#### Revision: 574eeb502d14
