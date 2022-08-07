# Unity 5.5.1
https://unity3d.com/unity/whats-new/unity-5.5.1

## Fixes

<ul>
<li>AI: Fix for "!InCrowdSystem" and "!handle.IsValid()" errors seen in console when calling Warp and enabling a disabled NavMeshAgent. (833396)</li>
<li>Analytics: Fixed occasional Windows editor crash on shutdown. (858785)</li>
<li>Android: Disabled fence sync on poor performing drivers. (827110)</li>
<li>Android: First scene is now loaded asynchronously while the splash screen is displayed. (835453)</li>
<li>Android: Fixed a crash when reloading or resuming scene which uses WebCamTexture. (855603, 859268)</li>
<li>Android: Fixed an exception when trying to build to a non-existent path. (848830)</li>
<li>Android: Fixed an issue where pausing during the splash screen would cause sprites to be black. (845080)</li>
<li>Android: Fixed auto-rotation on Android 4.1 and older. (854739)</li>
<li>Android: Gradle build and project export now support icon override. (855612)</li>
<li>Android: Input.backButtonLeavesApp = true now exits gracefully. (845646)</li>
<li>Android: Post process now executed before app is pushed to device. (803872)</li>
<li>Android: The platform setting for Android plugins now defaults to "Android" instead of "Any Platform". (824462)</li>
<li>Animation: Fix a crash using Resources.UnloadUnusedAssets with Animators caused by orphaned references. (855545)</li>
<li>Animation: Re-enabled multithreaded StateMachine evaluation.</li>
<li>AR: Fixed a crash when exiting play mode during a Holographic Simulation session. (858208)</li>
<li>Asset Import: Fixed a bug where importing multiple native DCC source files resulted in the contents of imported prefabs randomly switching places. (848920, 858080, 860956)</li>
<li>Asset Import: Fixed an issue where deleting asset labels manually from .meta files would not be picked up by the editor. (793711)</li>
<li>Asset Import: Fixed an issue where asset and timestamp maps could get out of sync. (668043, 837519)</li>
<li>Asset Import: Fixed a bug when importing Alpha8 textures didn't import them as a single channel texture. (849376)</li>
<li>Asset Import: Fixed a crash during texture importing if the import failed. (852116)</li>
<li>Asset Import: Fixed a crash during texture importing if the texture format wasn't supported by the platform. (853722)</li>
<li>Asset Bundles: Fixed redundant asset bundles rebuild when external DLL changes. (741525)</li>
<li>Audio: Changed default behaviour of native spatializer plugins to only load at start for the editor. Platforms now load when requested only.</li>
<li>Audio: Fixed FSBTool crashing when importing Ogg files with non-standard sample rates. (849972)</li>
<li>Build Pipeline: VR Splash Screen texture will no longer be included when building a project for a non-VR platform. (853618)</li>
<li>Cache Server: Fix for 'last resource used' behaviour; a file that it requested from the cache server will have its LRU state refreshed and its lifetime extended. (853250)</li>
<li>Cache Server: Fixed editor-local cache server not working if there were spaces in the path to the Unity Editor executable.</li>
<li>Collab: Fixed an issue whereby the Collab toolbar continued to have 'sign in' button even after signing in. (849875)</li>
<li>Collab: Fixed case of sign-in window getting stuck when launched from the toolbar menu. (836131)</li>
<li>Core: Fixed hangs in the job system when running on certain platforms with a low number of cores e.g. older Windows Phones, UWP dual core machines. (791434)</li>
<li>Editor: Fixed an issue related to the 'Remember Me' functionality in login window. (859728)</li>
<li>Editor: Fixed ArgumentOutOfRangeException triggered when closing tabs in dock area. (840151)</li>
<li>Editor: Fixed case of some properties being set to a single value when entering multi select mode for Trails and Lines. (849022)</li>
<li>Editor: Fixed disappearing tab when closing 3 or more of them successively. (849138)</li>
<li>Editor: Fixed launching Unity getting stuck on a grey screen for a minute or longer when the internet connection is bad. (793891)</li>
<li>Editor: Fixed NullReferenceException when undocking preview window. (857037)</li>
<li>Editor: Fixed a crash when baking occlusion. This also fixed a crash in rare cases at the end of occlusion baking if your scene contains portals. (843280)</li>
<li>Editor: Fixed Sprite Editor not always grid slicing fully black sprites correctly. (858043)</li>
<li>Editor: Fixed the splash screen 'Preview' button showing the NoiseModule preview texture. (857504)</li>
<li>Editor: Reduced heap allocations for each frame when rotating the scene view in the editor. (828286)</li>
<li>Editor: Tweaked the output of the generated Visual Studio solution file to better match Visual Studio standard format, in order to fix problems opening Unity generated projects with Rider IDE. (833866)</li>
<li>Editor: Fixed a curve preview cache not updating preview if curve data had changed but not the bounds. (856733)</li>
<li>Game Performance: Fixed a potential crash on player exit if Game Performance Service is enabled. (840591)</li>
<li>Graphics: Added Material.SetBuffer with nameID overload. (853627)</li>
<li>Graphics: Disabled GPU skinning on OpenGL and OpenGL ES APIs, due to performance and driver quality issues. (805221, 605171)</li>
<li>Graphics: Don't let GC dispose of ComputeBuffers. Added a warning for the user to release it manually. (830217)</li>
<li>Graphics: Fix to ensure that ETC1 alpha split option only shows for ETC1 4bit format in texture importer. (821298)</li>
<li>Graphics: Fixed a crash during shutdown when using the DX9 graphics API. (846989)</li>
<li>Graphics: Fixed a crash when calling Graphics.Blit(null, destination). (860626)</li>
<li>Graphics: Fixed a crash when deleting a Shader that is used by some Materials in the scene. (851359)</li>
<li>Graphics: Fixed a crash when using Material.SetColor and similar functions with some built-in Unity variable names. (849344)</li>
<li>Graphics: Fixed a problem where the Windows standalone would appear on a different display from that selected in the game launcher. (829120)</li>
<li>Graphics: Fixed a problem with objects not rendering after resolution changes or entering/exiting fullscreen when using DX9 graphics API. (840897)</li>
<li>Graphics: Fixed an issue where GrabPass could cause lighting to break on translucent objects in a scene. (844799)</li>
<li>Graphics: Fixed case of the Windows player build being disabled when using linear rendering and OpenGL ES graphics API in the editor.</li>
<li>Graphics: Fixed console error generated when using WWW.movie. (825464)</li>
<li>Graphics: Fixed errors in the console when performing GPU profiling on a DX11 Standalone build. (767034)</li>
<li>Graphics: Fixed lightmap decoding in the editor when the target platform is mobile. (849671)</li>
<li>Graphics: Fixed memory leak when instantiating materials (e.g. via renderer.material). (851689)</li>
<li>Graphics: Fixed OpenGL color space support on Windows (WGL_EXT_colorspace detection).</li>
<li>Graphics: Fixed rendering bug when GrabPass is used with forward rendering and graphics jobs are enabled. (836947)</li>
<li>Graphics: Fixed the GPU Profiler in standalone mode.</li>
<li>Graphics: Fixed the GPU Profiler to work in the MacOS Editor using OpenGL. Can only profile a single game window whilst it is in play mode. (823371)</li>
<li>Grahics: Fixed UI image mask when running in upscaled fullscreen mode in OpenGL. (849681)</li>
<li>Graphics: Fixed warped lens flare and halo effects when not in stereo rendering. (825046, 824894)</li>
<li>Graphics: Stopped rendering projectors twice if there is any transparent object visible to the camera. (732380)</li>
<li>Graphics: Stopped the texture importer ignoring pure white Alpha channels by default. It is now a user option to choose to ignore it. (849356)</li>
<li>Graphics: Fixed a memory leak and assert when shadows are cast from lights with specific properties and in a specific scene setup. (764734)</li>
<li>HoloLens: Fixed a crash in Editor when terminating Remoting App during an active Holographic Remoting session.</li>
<li>HoloLens: Fixed resume-from-suspend bugs that would occasionally crash the app or not render anything. (800796, 851897, 825951)</li>
<li>HoloLens: Improved error reporting when failing to load PerceptionRemotingPlugin.dll (used by Holographic Remoting). (848237)</li>
<li>IL2CPP: A more useful error message is now returned from IL2CPP when trying to build a WebGL project with the Facebook SDK. (850383)</li>
<li>IL2CPP: Added proper support for a class that is marshalled as a field of another class or struct, including the proper return value for a call to Marshal.Sizeof in this case. (852445)</li>
<li>IL2CPP: Added support for managed stack traces on Android. (846956)</li>
<li>IL2CPP: Corrected a crash that can occur in the player when a virtual method is called on a value type and that value type implements an interface which has an overload of that virtual method. (849701)</li>
<li>IL2CPP: Corrected managed stack traces when Xcode 8 is used to build on iOS with link-time optimization enabled. (845666)</li>
<li>IL2CPP: Emit proper C++ for unsafe methods that cast a void pointer to a type pointer and access a field from that type.</li>
<li>IL2CPP: Fix to prevent a compiler error in generated C++ code when calling Interlocked.CompareExchange from some managed code. (847838)</li>
<li>IL2CPP: Fix to prevent a stack overflow exception in the player at run time when an infinitely nested generic method is used. (845174)</li>
<li>IL2CPP: Fixed an issue with attribute classes that have overridden properties. (853468)</li>
<li>IL2CPP: Implemented the array SetValue method for arrays of nullable types. (849072)</li>
<li>IL2CPP: Now allow the Unity Ads engine integration to correctly build with Android on IL2CPP.. (857296)</li>
<li>IL2CPP: Prevent a stack overflow in the player runtime when metadata for an infinitely nested recursive generic type used (like the FullName of that type). (856410)</li>
<li>IL2CPP: Fixed issue where the error output from the Android compiler/linker was not captured. (851098)</li>
<li>iOS: Added Taiwanese language support. (853532)</li>
<li>iOS: Fix 2nd stage splash on iPhones with landscapeRight orientation (810286)</li>
<li>iOS: Fixed crash in application:openURL:sourceApplication:annotation due to missing null check with Facebook SDK. (856989)</li>
<li>iOS: Fixed crashes in WWWConnection. (852363)</li>
<li>iOS: Fixed Module Registration and Code Stripping for builds with the Mono scripting backend. (763240)</li>
<li>iOS: Removed extra offset in constraint in default launchscreens. (831195)</li>
<li>Lighting: Stopped the first probe being rendered multiple times when drawing the light probe visualization gizmo in the editor.</li>
<li>Lighting: Fixed a problem with reflection probes updating during runtime even when "Refresh Mode" was set to "Via Scripting". (820587)</li>
<li>Lighting: Only clear the lighting progress bar when lighting is in progress. Stops lighting system accidentally closing other (non-lighting) progress bars. (851764)</li>
<li>Metal: Fixed a crash on startup on some iOS devices. (857032)</li>
<li>Metal: Fixed a memory leak when loading scene. (867312)</li>
<li>Multiplayer: Error creating/requesting Network matches on WebGL. (810267)</li>
<li>Multiplayer: Fixed host migration sync issue. (807091)</li>
<li>Multiplayer: Fixed InvalidOperationException when selecting NeworkManager in Hierarchy for the first time. (812479)</li>
<li>Multiplayer: Made sure isLocalPlayer works as expected on OnDestroy. (853316, 826931)</li>
<li>Networking: Fix to prevent using a packet size greater than defined in global config. (719672)</li>
<li>Networking: Skip proxy check when using the "file://" protocol on Windows.</li>
<li>Particles: Added animation support for simulation speed property. (837602)</li>
<li>Particles: Calling Destroy() with particle system object in IEnumerator Start() could cause a crash (855467)</li>
<li>Particles: Fixed crash in CopyFromArrayAOS when calling Emit(position, velocity, size, lifetime, color). (858235)</li>
<li>Particles: Fixed error in TLS Allocator when simulating particle system. (856877)</li>
<li>Particles: Fixed occasional crash when using external forces module. (849084)</li>
<li>Particles: Fixed rare memory overwrite which would have caused problems (crashes) in random other areas.</li>
<li>Particles: Game crashes when new particles are spawned using deprecated Emit method. (856871)</li>
<li>Particles: Particle System Lights Module would not generate lights if particle positions were modified by script. (856224)</li>
<li>Particles: Particle System Renderer wouldn't allow rendering using multiple materials. (852817)</li>
<li>Particles: Particle System subsequent Sub Emitter inherit properties were overridden with the first inherit property. (846516)</li>
<li>Particles: Particle System editor was using incorrect handle matrix when scaling mode was set to Hierarchy. (851712)</li>
<li>Particles: Unity could crash in EmitterStoreData function when a Particle System was "aligned to direction" during Play mode. (850638)</li>
<li>Physics 2D: Ensure that Rigidbody2D interpolation is reset if the Transform rotation is changed. (829769)</li>
<li>Physics 2D: Fixed some 2D polygon outlines that were almost collinear causing collision detection problems. (715922)</li>
<li>Physics 2D: Continuously setting Rigidbody2D 'bodyType' or 'IsKinematic' to the same value should not cause contact recalculations; this can cause instabilities. (835334)</li>
<li>Physics 2D: Display message in Inspector for Rigidbody2D when auto-mass is used on a Prefab or an inactive object. (828188)</li>
<li>Physics 2D: Scaling a CapsuleCollider2D using a Transform component scale in X or Y of zero in the inspector no longer causes a warning in the console. (853163)</li>
<li>Physics: Fixed an accuracy issue where a capsule would jitter and bounce erratically after being placed on top of a scaled mesh at specific locations when the PCM collision mode was enabled. (850059)</li>
<li>Physics: Fixed interpolation of Rigidbodies causing position and rotation to be inaccurate when accessed via Transform from within FixedUpdate. (858816)</li>
<li>Prefabs: Fixed an issue where a prefab instance could be incorrectly marked inactive when first loading a scene. (801761)</li>
<li>Profiler: Fixed isse where taking a detailed memory snapshot did not work in some cases. (836589)</li>
<li>ReplayKit : Fixed a crash when creating objects from broadcasting start callback. (848718)</li>
<li>ReplayKit : Fixed ReplayKit.StartBroadcasting not pausing the app. (833159)</li>
<li>Scripting: Fixed case of WaitForSeconds waiting forever when receiving NaN as the parameter. (759338)</li>
<li>Scripting: Fixed MonoDevelop build errors when building UnityScript and Boo projects. (850350)</li>
<li>Shaders: Automatically upgrade any shaders using unity_SpecCube1. This fixes unity_SpecCube1 related shader compile errors after a project upgrade. (825418)</li>
<li>Shaders: Bug fixes in translating shaders from HLSL to GLSL/Metal: 
<ul>
<li>Crash fix on partial precision parsing.</li>
<li>Added support for missing texture gather ops and sample count query.</li>
<li>Fixed bugs in swapc, SM5 variant of shift ops, atomic compare exchange, texture array coord translation, texture array element index rounding, texel fetch swizzle and GLSL extension handling.</li>
</ul></li>
<li>Shaders: Fixed a problem when compiling shaders using windows style directory separator ("\") in #include paths on macOS.</li>
<li>Shaders: Fixed a rare problem on DX11 with NaNs happening during the depth pass of forward rendering mode, resulting in shadow artefacts. (814063, 812479)</li>
<li>Shaders: Fixed a shader compiler crash for surface shaders which had extra "}" tokens in them. (844355)</li>
<li>Shaders: Fixed crash when compiling very complex surface shaders. Optimised the memory usage during surface shader compilation. (825408)</li>
<li>Shaders: Fixed UNITY_VERSION macro not being setup in surface shaders. (852264)</li>
<li>Standalone: Fixed the incorrect display labels when using more than 2 monitors. (829120)</li>
<li>Substance: Fixed a crash when compressing small non-square textures to ETC with 'fast' quality. (857270)</li>
<li>Substance: Fixed case of ProceduralTexture inspector preview sometimes showing invalid size and format. (829162)</li>
<li>Substance: Fixed case of SubstanceArchive inspector unselecting ProceduralMaterials after being renamed. (840177)</li>
<li>Substance: Fixed crash when loading a substance with corrupted data, (842999)</li>
<li>Substance: Fixed issue where the emission shader parameter was not properly set on import when emission global illumination was set to realtime. (840181)</li>
<li>Tizen: Fixed a deploying failure problem. (861611)</li>
<li>UI: Fixed a NullReferenceException when changing font to none. (845756)</li>
<li>UI: Fixed jittery movement when scrolling ScrollRect. (819300)</li>
<li>Unity Ads: Fixed Cloud Build issue.</li>
<li>UnityWebRequest: Fixed case of incorrect Content-Type request header for multipart form data in POST requests. (826626)</li>
<li>UnityWebRequest: Fixed case of POST requests not working with empty data. (851921)</li>
<li>UnityWebRequest: Fixed issue where escaped characters in URL would get unescaped. (850018)</li>
<li>UnityWebRequest: Fixed the issue of a request continuing execution after exiting playmode, resulting in high CPU usage. (855646)</li>
<li>VCS: Don't attempt to connect to a Perforce server if any of the following parameters are unset: Server, User or Client. (861467)</li>
<li>VCS: Fixed null reference exception that could occur after resolving an asset (e.g. prefab) whilst the asset is selected and displaying in the inspector. (657131)</li>
<li>VR: Fixed a memory leak when using a canvas and VRFocus is lost. (824508)</li>
<li>VR: Fixed an issue where only the shadows from the first light would render in both eyes when using single pass instancing. (851967)</li>
<li>VR: Fixed case of error shader rendering in one eye only when using single pass instancing. (851891)</li>
<li>VR: Fixed crash when checking for Stereo VR Device during build. (845179)</li>
<li>VR: Fixed the usage of VRSettings.renderViewportScale in Camera's OnPreCull so that it was not a frame latent on all supporting SDKs. Fixed issues with Valve's The Lab Renderer adaptive quality feature.</li>
<li>VR: OpenVR app built and run with d3d12 crashes on start. (834072)</li>
<li>VR: Switching stereo rendering during playback causes rendering issues. (852569)</li>
<li>VR: Fixed camera strobing between head poses once game is built. (858763)</li>
<li>VR: Y-Axis Range For VR Controllers now match XBox controllers (858634)</li>
<li>WebGL: Disabled deferred rendering on WebGL1.0. (759286, 782587)</li>
<li>WebGL: Fixed build with improperly tagged plugins. (850383)</li>
<li>WebGL: Fixed Content-Length header field for local web server response that caused some audio files to have .duration of infinity or zero. This was not reproducible with the normal workflow but could occur with a specific asset store plugin for webgl audio streaming.</li>
<li>Windows Store: Building project for Windows Store targeting Windows 10 SDK now works when only Visual Studio 2017 is installed. (859650)</li>
<li>Windows Store: Fixed duplicate assembly warning when building Universal 8.1. (822480)</li>
<li>Windows Store: Fixed the issue of UnityWebRequest not working in Master builds. (854650)</li>
<li>Windows Store: Generated VS project now builds once again when targeting ARM with IL2CPP scripting backend. (859389)</li>
<li>Windows: Fixed issue where Application.systemLanguage would return the region language rather than the UI language. (820871)</li>
</ul>

#### Revision: 88d00a7498cd
