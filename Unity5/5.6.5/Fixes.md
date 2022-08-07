# Unity 5.6.5
https://unity3d.com/unity/whats-new/unity-5.6.5

## Fixes

<ul>
<li>AI: Fixed unwanted gap in the NavMesh produced by a concave edge crossing a tile boundary. (930830) (936512)</li>
<li>Android: Fixed player crash when profiler with GPU profiling was enabled and graphics API was not OpenGL ES 3. (944118)</li>
<li>Android: Fixed realtime HDR reflection probes being black on older Android devices. (776875)</li>
<li>Android: Fixed build with target sdk 21-23. (956658)</li>
<li>Android: Fixed permissions popup crash. (934782)</li>
<li>Android: Fixed android video player stuttering and dropping frames. (931038)</li>
<li>Android: Fixed android video player playback lagging after activating input field. (934841)</li>
<li>Android: Fixed symbols.zip not including symbols file. (942625)</li>
<li>Android: Fixed header availability in UnityWebRequest when response uses chunked transfer. (956599)</li>
<li>Animation: Fixed an irrelevant assert in Animation Component. (943954) (924891)</li>
<li>Animation: Fixed assert when loading AnimationClip asynchronously in AssetBundles. (943438)</li>
<li>APIUpdater: Fixed unnecessary reference to mscorlib 4.0 being added to assemblies in some cases. (916719)</li>
<li>Audio: Quality of atrac9 clips can now be adjusted properly in the audio importer. (896143)</li>
<li>Build: Fixed exceptions in OnPreProcessBuild not halting the build process correctly. (942296)</li>
<li>Build: Fixed a crash in BuildReporting::BuildReport::BeginBuildStep caused when BuildAssetBundles was being called from an OnPreprocessBuild callback. (920536)(920116) (958239) (947004)</li>
<li>DX12: Fixed copy queue memory leak.</li>
<li>DX12: Fixed constant buffer memory being overwritten in certain circumstances. (938617)</li>
<li>DX12: Fixed bad pipeline state issue causing errors. (925955)</li>
<li>Editor: Fixed player settings not using the default icon when there are none specified. (953161)</li>
<li>Editor: Fixed an error messages when enabling Version Control "Work Offline" mode e.g. "InvalidOperationException: Operation is not valid due to the current state of the object". (879511)</li>
<li>Editor: Fixed an issue where LogAssert.Expect would ignore the the logtype when finding a satisfying event when running playmode and editmode tests. (944934, 935602)</li>
<li>Editor: Fixed lightmaps being generated even when the scene does not contain any baked light contribution. (926559)</li>
<li>Editor: Fixed occasional hang during Editor startup. (954607)</li>
<li>Editor: The generated TestResults.xml when running playmode and editmode tests is now updated to be in NUnit3 format. (940837, 910845)</li>
<li>GI: Fixed Enlighten not generating lightmaps for meshes imported without UVs and with Generate Lightmap UVs option enabled. (854349)</li>
<li>GI: Fixed a crash in 'RenderTexture::DiscardContents' when opening the scene. (935328)</li>
<li>GI: Fixed exception being thrown when the background color of a Reflection Probe is changed. (939947)</li>
<li>GI: Fixed terrain artefacts caused by Enlighten terrain mesh triangulation being different from the original mesh triangulation. (754298)</li>
<li>GI: Fixed project build errors when Reflection Probes Projection setting in Tier1(Graphics Settings) is unchecked. (925552)</li>
<li>GI: Progressive Lightmapper crashes with transparent shader. (949574)</li>
<li>Graphics: Fixed an issue where performing an undo on a Static Lightmap Object caused an error related to transforms to be reported. (955082)</li>
<li>Graphics: Fixed updating of bounding boxes for SkinnedMeshRenderers with 'Update When Offscreen' set. (935463)</li>
<li>Graphics: Fixed "group &lt; 0x7fff" errors when hitting undocumented limit for LOD groups. (667190)</li>
<li>Graphics: Fixed an issue where off-screen SkinnedMeshRenderer with 'update when off-screen' enabled was not skinned. (939897)</li>
<li>Graphics: Fixed asserts when animations disable newly visible renderers. (950215)</li>
<li>Graphics: Fixed a crash in CameraStackRenderingState::ReleaseResources e.g. searching in Hierarchy window. (926718)</li>
<li>Graphics: Fixed camera rendering to a temporary RenderTexture from clearing the stencil bits when it shouldn't i.e. for HDR cameras. (932065)</li>
<li>Graphics: Report an error instead of crashing when Mesh has invalid positions e.g. NaN. (930666)</li>
<li>Graphics: Fixed the Sprite Mode in the Inspector Import Settings so it defaults to Single rather than None, when an image is imported. (921598)</li>
<li>Graphics: Metal: Fix occasional GPU hangs when dispatching compute shaders. (950990)</li>
<li>Graphics: Fixed D3D11 errors in scenes containing a Camera that has HDR enabled and depth-only clear. (933768)</li>
<li>IL2CPP: Avoid stack overflow from occurring in Unity liveness logic (asset GC). (935563)</li>
<li>IL2CPP: Improve incremental build performance on OSX.</li>
<li>IL2CPP: Allow SetSocketOption to work properly for add membership and remove membership with IPv6. (944939)</li>
<li>IL2CPP: Fixed calling System.Collections.Generic.IList1 methods on native objects that implement Windows.Foundation.Collections.IVector1 interface and calling Windows.Foundation.Collections.IVector1 methods on managed objects that implement - System.Collections.Generic.IList1 interface.</li>
<li>IL2CPP: Fixed crash in thread pool during shutdown. (966623)</li>
<li>iOS: Fixed the Screen.dpi() method in the Trampoline code not returning the correct number of DPI in iPhone 8, iPhone 8+ and iPhone X. Also fixed the iPhone 8+ and iPhone X model checking. (962350 960914)</li>
<li>iOS: Fixed support for fonts of Tibetan, Armenian, Braille, Georgian and Thai languages in iOS 10 and iOS 11. (951089) (949036)</li>
<li>iOS: Fixed crash when connection is lost in the middle of AssetBundle download using WWW. (955760)</li>
<li>iOS: SystemInfo.supportedRenderTargetCount now correctly returns 8 for devices that support it. (949032)</li>
<li>Lighting: Fixed issue where Progressive Lightmapper was not transmitting indirect rays through translucent objects. (887019)</li>
<li>Lines: Fixed a case where looping lines with corner vertices were causing graphical corruption. (939661)</li>
<li>Metal: Fixed a shader compilation regression on macOS 10.11.6 and iOS 8.x and earlier. (952232, 952020)</li>
<li>Multiplayer: Fixed update timers internal time after io thread resuming.</li>
<li>Multiplayer: Fixed reliable message can be delivered twice.</li>
<li>OSX: Fix Editor crash when using GLCore on High Sierra with Intel 6xxx series GPU. (963867 956196)</li>
<li>OSX: Application.persistentDataPath always returns. Library/ApplicationSupport (instead of occasional Library/Caches). (898217)</li>
<li>OSX: Fixed High Sierra OS freeze while using Local Cache Server. (954747)</li>
<li>OSX: Fixed startup crash on OSX 10.11 and iOS 7 with Metal.</li>
<li>OSX: Fixed hang for Metal when using MSAA on OSX 10.11 for Nvidia GPUs. (963062)</li>
<li>Particles: Fixed an issue where some Shape Module properties could become corrupt during an upgrade (Radius, Arc, Random Direction). (910284)</li>
<li>Particles: Fixed an issue where the ParticleSystem.Emit() was ignoring the playback time when reading the Main Module curves/gradients. (936628)</li>
<li>Particles: Fixed an issue where Sorting Fudge was incorrect when using a Custom Sort Axis on a camera. (937693)</li>
<li>Physics: Ensure that the enter/exit collision/trigger callbacks are correctly matched when a single simulation step causes a contact to stop then start again. (932044)</li>
<li>Physics: Fixed GameObject with a disabled cloth component not following parent's transform. (946307)</li>
<li>Profiling: Fixed various instabilities with Integration tests, namely suites ProfilerSuite.ProfilerDynamicSampleTests and ProfilerSuite.ProfilerCustomSamplerTests.Resource Management: Optimized the loading of assets performed via Resources.Load. This - addresses a performance regression reported in Android platforms. (930803, 904652)</li>
<li>Scripting: Fix 64-bit type packing in the iOS runtime. (949127)</li>
<li>Scripting: Fixed crash in debugger when trying to stop while a single step operation is in progress. (951901)</li>
<li>Scripting: Fixed deadlocks and pauses when using System.Threading.Monitor. (827984)</li>
<li>Shaders: Fixed an issue with shadows precision on mobile platforms. (925180, 899829)</li>
<li>tvOS: Fixed icon asset catalog setup when certain multi-layer icons are missing. (959867)</li>
<li>UnityWebRequest: Fixed a resource leak when aborting an AssetBundle download, leading to higher memory usage and sometimes CPU throttling. (944301)</li>
<li>UWP: Fixed "Run in Background" player setting not making player to ignore minimize events. (759166)</li>
<li>VR: Fixed iOS Google VR Podfile not reporting the correct version. (962253)</li>
<li>WebGL: Enabled fullscreen support in Safari &gt;= 10.1. (941166)(775206)</li>
<li>Windows Standalone: Fixed an issue that caused recursive player loop error when moving window around. (946559)</li>
<li>XR: Fixed android driver issue by invalidating the depth and stencil buffers at the same time.XR: Fixed issue with Camera.stereoSeparation being incorrectly applied to Oculus HMDs. (957491)</li>
<li>XR: Fixed black screen on startup on Cardboard when GLES2 or GLES3 is used. (931397)</li>
<li>XR: Fixed handling of Screen resolution changes, especially in VR</li>
<li>XR: Fixed camera aspect ratio after disabling VR. (892084)</li>
<li>XR: Fixed mobile XR applications forcing landscape left orientation when right has been selected in the player settings.</li>
</ul>

#### Revision: 2cac56bf7bb6
