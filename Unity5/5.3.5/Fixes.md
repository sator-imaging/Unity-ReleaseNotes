# Unity 5.3.5
https://unity3d.com/unity/whats-new/unity-5.3.5

## Fixes

<ul>
<li>Analytics: Fixed a rare crash. Only occurs when analytics is on and importing a complete project from asset store with analytics off.</li>
<li>Android: Audio - Fixed OpenSL output not selected when default buffer size selected. (784899)</li>
<li>Android: Buildpipe - Don't make use of preview SDK tools installed. (788040)</li>
<li>Android: Buildpipe - Fixed AAPT errors on project export. (786918)</li>
<li>Android: Buildpipe - Fixed AAR plugin and resource issues on exported projects. (765396)</li>
<li>Android: Disabled Debug markers on PowerVR Series5 devices due to driver issues. (780958)</li>
<li>Android: Fix for EGL_BAD_NATIVE_WINDOW error on resume. (747898)</li>
<li>Android: Fix for GPU skinning on Adreno GPUs. (763755)</li>
<li>Android: Fix for syncing to low framerate with VSync off. (777167)</li>
<li>Android: Fixed a crash in the Development build for some Android devices with PowerVR GPUs (e.g. Asus Memo Pad). (787491)</li>
<li>Android: Fixed blending with background on Unity splash screen.</li>
<li>Android: Fixed crash on Nvidia Shield tablet. (765744)</li>
<li>Android: Fixed crash when loading scenes intermittently. (751530)</li>
<li>Android: Fixed immersive mode switching off on some KitKat devices when pressing volume buttons. (779338)</li>
<li>Android: Fixed incorrect width/height when changing orientation after changing anti-aliasing settings. (771542)</li>
<li>Android: Fixed potential crash when using WWW without having Internet permission (also affects use of Unity Analytics). (779877)</li>
<li>Android: Fixed potential race condition in atomic operations on ARM processors.</li>
<li>Android: Fixed Standard Shader lighting issue caused by half-precision overflow on Mali GPUs. (761744)</li>
<li>Android: Fixed value of trackingEnabled.</li>
<li>Android: Workarounds for OpenGL ES 3 shader compiler problems on Adreno GPUs. (777617)</li>
<li>Animation Window: Fixed Null Reference Exception in Curve Editor. (775565)</li>
<li>Animation Window: Disabled animation sampling of an optimized game object hierarchy in the animation window. (753270)</li>
<li>Animation Window: Fixed custom components not appearing in the Add Property menu of the Animation Window. (760809, 759069)</li>
<li>Animation Window: Fixed selection loss in animation window when pasting keyframes. (715416)</li>
<li>Animation: Fixed a crash related to exposed skeleton. (784942)</li>
<li>Animation: Fixed a crash when importing an animation where a whole curve was corrupted. (774052)</li>
<li>Animation: Fixed a performance issue for AnimatorOverrideController rebind. (779058)</li>
<li>Animation: Fixed an issue where instantiating a prefab with an Animator Component for the first time took longer than the subsequent times. (771609)</li>
<li>Animation: Fixed an issue where rotation curves would be created as Euler curves by default when using the Animation Component. (772668)</li>
<li>Animation: Fixed an issue where the scale was not working in editor on GameObject with OptimizeGameObject. (774484)</li>
<li>Animation: Fixed animation event inheriting from ScriptableObject not getting triggered. (762952)</li>
<li>Animation: Fixed crash when an animation key tried to activate a game object which had animator attached to it. (786873)</li>
<li>Animation: Fixed crash when calling Animator.Update(0) in an AnimationEvent. (783821)</li>
<li>Animation: Fixed crash when GameObject with Animator is instantiated in StateMachineEnter/Exit. (770045)</li>
<li>Animation: Fixed crash when shutting down standalone app with Script Playables. (775677)</li>
<li>Animation: Fixed error message in console while optimizing animation hierarchy from the inspector. (775773)</li>
<li>Animation: Fixed issue where Animation was distorted when animated object was scaled and Optimize Game Objects was selected. (766898, 758322)</li>
<li>Animation: Fixed scale value getting zeroed when removing scale curve components in AnimationWindow. (689644)</li>
<li>APIUpdater: Fixed AssemblyUpdater crash when verifying WSA  / Windows Phone assemblies. (767506)</li>
<li>APIUpdater: Fixed ScriptUpdater crash when processing Boo / UnityScript containing Hash literals. (769880)</li>
<li>Asset Bundles: Fixed issue where WWW.LoadFromCacheOrDownload would not take into account space on device, and could hang. (762829)</li>
<li>Asset Bundles: Fixed the error messages when building variant asset bundles. (769858)</li>
<li>Asset Bundles: Fixed an issue where unloading an asset bundle with animated objects (legacy animation) during play mode crashes the editor. (775822)</li>
<li>Asset Bundles: Added back scene asset bundles compression statistics. (768965)</li>
<li>Asset Bundles: Fixed a crash while loading asset bundle asynchronously. (747800)</li>
<li>Asset Bundles: Fixed a potential crash when decompressing corrupted LZMA bundles. (782773)</li>
<li>Asset Bundles: Fixed Compress Assets On Import setting ignored when switching platform (762739)</li>
<li>Asset Bundles: Fixed CreateFromMemory not working with "." in filenames. (734216)</li>
<li>Asset Import: Fixed a crash on FBX import in some rare circumstances. (768846)</li>
<li>Asset IMport: Fixed issue where changing date modified on directory meta file caused all files below that directory to be reprocessed. This was also affecting VCS. (756559)</li>
<li>Audio: Don't try to load any sounds when Unity audio is disabled. (776044, 763036)</li>
<li>Audio: Fixed an issue where Low Pass Filter didn't work on Audio Listener. (732854)</li>
<li>Batch mode: Fixed an issue where BuildPlayer calls might cause compilation errors to be logged in subsequent runs. (703290, 786195)</li>
<li>Cache Server: Upgraded the node.js version 0.12.7. (760234)</li>
<li>Compute: Do not log warnings/errors when current build target does not support compute shaders.</li>
<li>Core: Added stacktrace for logging statements and exceptions called on threads. (697872, 633905)</li>
<li>Core: ArgumentCache.TidyAssemblyTypeName is now alloc-free if the type name is already clean. (738249)</li>
<li>Core: Fixed crash when scaling prefab with mesh that is not read/write enabled. (766019)</li>
<li>Core: When exporting a package with scene's dependencies, checkboxes are available next to folder icon. (752733)</li>
<li>Core: WWW.responseHeaders is now a case-insensitive Dictionary, as per RFC2616 spec. (770155)</li>
<li>D3D11: Fixed a deadlock which would occur when trying to restore focus to a minimized standalone player running in Fullscreen Exclusive mode. (523691)</li>
<li>D3D11: Fixed exclusive mode window reactivation issues after focus has been lost. (788555)</li>
<li>D3D11: Fixed some rare crashes on memory constrained systems (log would contain resource creation failure messages).</li>
<li>D3D9: Player loop will now be processed in the background again when the graphics device is lost (Windows are locked, window is minimized, etc.). (752626)</li>
<li>Editor: Fix for core assemblies not being reloaded after encountering errors in user scripts. (750423)</li>
<li>Editor: Added support for resizing the height of the preferences window. (763313)</li>
<li>Editor: Adjusted the width of the 'Build Settings' window so that it properly display its contents, even if support for some of the players is not currently available. (728634)</li>
<li>Editor: Files with invalid names can no longer be dragged into a project. (663994)</li>
<li>Editor: Fixed a crash that could happen when animation window is open, and playmode is entered. (696623)</li>
<li>Editor: Fixed a crash when locking cursor from constructor or static initializer. (765466)</li>
<li>Editor: Fixed a crash when padding ASTC texture when building from command line. (759288)</li>
<li>Editor: Fixed an inconsistency between visible and hidden meta file modes, where empty folders were recreated in 'visible' mode. (588531)</li>
<li>Editor: Fixed an issue that could cause scenes containing prefab instances with driven transforms to immediately become dirty. (709639)</li>
<li>Editor: Fixed an issue that was causing transformations to be modified when entering and subsequently coming back from play mode. (759115)</li>
<li>Editor: Fixed an issue where compression wasn't being applied in calls to BuildPipeline.BuildStreamedSceneAssetBundle(). (781866)</li>
<li>Editor: Fixed an issue where unloaded scenes were removed from hierarchy after exiting playmode. (769613)</li>
<li>Editor: Fixed an issue with dragging a Sprite/Texture2D into the inspector causing a PolygonCollider2D to use it even though it is not dropped on the component editor itself. (778125, 780607)</li>
<li>Editor: Fixed changing order of components not getting saved. It now also support undo. (764986)</li>
<li>Editor: Fixed crash on launch if "metadata" folder is deleted before launching. (746964)</li>
<li>Editor: Fixed newly installed Unity command line activation issue. (790345)</li>
<li>Editor: Fixed performance issue in Sprite Inspector. (709059)</li>
<li>Editor: Fixed Target Support module download URLs in Build Settings.</li>
<li>Editor: Fixed the asset importer error when calling Refresh() during an assembly import. (730559)</li>
<li>Editor: Fixed WebViewWindow's freed memory access. (775366)</li>
<li>Editor: Fixed wrong error message when returning license via command line. (784727)</li>
<li>Editor: Fixed an issue when logging off and opening the Service Window would be missing. (781863)</li>
<li>Editor: If a read only file or folder is duplicated, the read only status is no longer duplicated. (730245)</li>
<li>Editor: Improved error messages for unsupported target platform in batch mode. (782752)</li>
<li>Editor: Now show alert popover for invalid serial format. (775898)</li>
<li>Editor: Remove SelectionBase from LOD Group. (763231)</li>
<li>Editor: Sped up importing of some Fonts by updating progress bar less often than "crazy often".</li>
<li>Editor: Fixed access to destroyed window during shutdown. (775244)</li>
<li>Editor: Fixed access violation in some editor GUIView operations. (769833)</li>
<li>GI: Fixed incorrect normal mapping on Directional Specular lightmaps; shader code was not matching up what Enlighten was baking. (755421, 766533, 766546, 779696, 756020, 780025)</li>
<li>GI: Clamped DynamicGI.indirectScale to allowed range. (664953)</li>
<li>GI: Disabled LightProbeGroup components no longer display visualization in the scene view. (662572)</li>
<li>GI: Fixed errors when using baked lightmaps &amp; multi-scene editing. (753822)</li>
<li>GI: Fixed realtime GI texture coordinates sometimes going wrong on static-batches meshes. (743273)</li>
<li>GI: Fixed some cases of scenes not referencing the correct lighting data asset after bake. (757575)</li>
<li>GI: Improved wording of various Enlighten error messages.</li>
<li>GI: Now properly initialize baked scenes in some code paths to avoid error on console. (753822)</li>
<li>GI: Upgraded to Enlighten3.02p4. Fixes direct lighting getting baked into lightmap (697565). Fixes a precision issue and out-of-bounds texture access in baking, which could lead to a crash in the Final Gather stage. (767110)</li>
<li>GI: Changing Reflection Probe component positioning in the inspector makes realtime probe black. (653592)</li>
<li>GI: Fixed a Reflection Probe baking issue when multiple scenes are used in a project.</li>
<li>GI: Fix for baking a scene with objects added before saving the scene not being included in the result. (728610)</li>
<li>GI: Fixed a crash when building reflection probe data on specific scenes containing Canvas elements. (767560, 763045)</li>
<li>Graphics: Fixed a glitch in Crunch format compressed non-alpha texture after using sprite packer. (774638, 768171)</li>
<li>Graphics: Fixed internal profiler for static batching on Android, iPhone and Windows Store. (769539)</li>
<li>Graphics: Fixed material index not being used when calling Graphics.DrawMeshNow with rotation. (765378)</li>
<li>Graphics: Fixed MovieTexture crash when loading a video with no audio stream.</li>
<li>Graphics: Fixed potential crash in SetGpuProgramName.</li>
<li>Graphics: Fixed static batching errors when meshes have additional vertex data streams with mismatching vertex count. (775261)</li>
<li>Graphics: Fixed TrailRenderer showing a gap between current position and the last update. (779129)</li>
<li>Graphics: Upgrading a shader with a DX11 [annotation] at the start of the file now doesn't crash. (766992)</li>
<li>IL2CPP: Correct an intermittent crash when Environment.GetCommandLineArguments is called. (775804)</li>
<li>IL2CPP: Emit proper C++ code for COM marshaling of methods that have at least one parameter that cannot be marshaled. (789905)</li>
<li>IL2CPP: Fixed a rare deadlock during Resources.UnloadUnusedAssets. (756912)</li>
<li>IL2CPP: Fixed an intermittent crash in the experimental memory profiler. (776152)</li>
<li>IL2CPP: Fixed an issue with Socket.Select and IL2CPP where a socket could be reported as being in an error state when it should have been reported as being in a write state. (759488)</li>
<li>IL2CPP: Generate C++ code to properly handle circular references for field types in unsafe C# code. (780472)</li>
<li>IL2CPP: Generate proper C++ code for a C# class with the StructLayout attribute when its base class does not have a StructLayout attribute. (767367)</li>
<li>IL2CPP: Generate proper C++ code for a method that is marked as both an internal call and a runtime call. (781439)</li>
<li>IL2CPP: Generate proper C++ code for the OnSerialize method injected by UNET in classes deriving from NetworkProximityChecker. (786499)</li>
<li>IL2CPP: Generate proper C++ code for the p/invoke wrapper for a delegate that accepts another delegate as an output parameter. (778146)</li>
<li>IL2CPP: Generated proper C++ code for assemblies compiled with Visual Studio when a method returning an IntPtr returns an integer value. (787687)</li>
<li>IL2CPP: Improved message for PathTooLongException being encountered in IL2CPP. (717343)</li>
<li>IL2CPP: Increased maximum heap size.</li>
<li>IL2CPP: Now correctly return the remote end point from a UDP socket receive call in an IPv6 network. (767741)</li>
<li>IL2CPP: Now generate proper code for COM marshaling of a struct that contains a field of type object array. (781921)</li>
<li>IL2CPP: Prevent a compile error in the generated C++ code due to a missing header when we generic exception type is used in a catch statement. (776087)</li>
<li>IL2CPP: Properly handle numeric conversion from an unsigned integer to floating point types in some edge cases. (780659)</li>
<li>IL2CPP: Properly handle type casts and check for value type arrays when they are casted to generic collection interfaces. (782653)</li>
<li>IL2CPP: Support proper default marshaling of string parameters and return values when the CharSet attribute is provided on a method with a value of Unicode. (692653)</li>
<li>IL2CPP: Throw informative exception when MonoPInvokeCallback delegate type is incompatible with target method signature. (732438)</li>
<li>Input: Input.mousePosition is no longer clamped to the client area on windows standalone, the last position is kept instead. (769666)</li>
<li>iOS: Added Xcode 7.3 Build &amp; Run support.</li>
<li>iOS: Allow IPv6 to work on iOS with the .NET 2.0 profile. (730146)</li>
<li>iOS: Allow third party plugins that use PLCrashReporter library. (768572)</li>
<li>iOS: Apple Pencil pressure will now be exposed the same way 3D Touch pressure already is.</li>
<li>iOS: Do not export non-prefixed freetype2 symbols now. (778668)</li>
<li>iOS: Ensure asset bundles are not flagged for iCloud backup by default upon download. (771597)</li>
<li>iOS: Ensure that our symbols are not overridden by user libraries. (774685)</li>
<li>iOS: Fixed a crash when playing a scene in the Editor with an iOS device attached as a Unity Remote. (771132)</li>
<li>iOS: Fixed GLES error 0x0506 and various graphics corruption when using WebCam textures. (763342)</li>
<li>iOS: Fixed incompatible pointer cast warning in trampoline. (776105)</li>
<li>iOS: Fixed memory leak when using On Demand Resources. (776528)</li>
<li>iOS: Fixed support for non-native resolutions in GLES 2. (779738)</li>
<li>iOS: Fixed the incorrect ABI for int64 types on iOS. (774544)</li>
<li>iOS: Fixed UnityWebRequest hanging on responses &gt; 64k when using a custom DownloadHandlerScript. (780329)</li>
<li>iOS: Made Social.ShowLeaderboardUI to show the leaderboards tab, instead of achievements tab. (777596)</li>
<li>iOS: Pause application on GameCenter dialogs on tvOS. (767633)</li>
<li>iOS: Switching between different input fields will not leave input accessory fields on screen. (775710)</li>
<li>iOS: TouchInputModule and StandaloneInputModule will now handle all touch phases preventing unwanted module switches. (764054)</li>
<li>iOS/IL2CPP: Prevent unnecessary changes to the timestamps of the libil2cpp headers during a build. This allows incremental builds to work correctly in Xcode.</li>
<li>iOS/tvOS: AdSupport is now removed from Default Frameworks and needs to be explicitly selected under Framework Dependencies in Platform Settings if required. (732878)</li>
<li>iOS/tvOS: Fixed a regression which caused artefacts when using GLES2 Graphics API. (785036)</li>
<li>JsonUtility: Fixed EditorJsonUtility throwing MissingMethodException (769085)</li>
<li>Linux: Don't query displays when running in nographics mode.</li>
<li>Linux: Exit with nice message instead of crashing when GPU/driver doesn't meet minimum requirements. (777564, 783842)</li>
<li>Linux: Fixed a crash when stereoscopic mode is requested on non-stereoscopic display. (784075)</li>
<li>Linux: Fixed an occasional crash when creating texture properties.</li>
<li>Mac Editor: Added functionality in order to prevent the processing of folders that contain the ".unity" extension, as this was causing the editor to crash when executing in batch mode. (761639)</li>
<li>MacDownloadAssistant: Fixed window focus issue after security prompt.</li>
<li>Mac Editor: Fixed UI text rendering on Radeon HD 4000 series and older AMD GPUs. (783713)</li>
<li>Mac Editor: Application.version now returns the application's version. It no longer returns Application.unityVersion. (764054)</li>
<li>MemoryProfiler: Added toggle to exclude references in detailed memory dump to reduce memory footprint used. (783527)</li>
<li>Mono: Fixed GC related test instability in OSX Editor. (777945)</li>
<li>Mono: Make the Personal folder be the same on all profiles.  (776268)</li>
<li>Networking: Fixed issue with SyncList change callback where the old value was given there instead of the updated one. (774970)</li>
<li>Networking: Fixed problem when transferring data via reliable sequenced QoS channel could lose messages in "bad" network conditions. (781177)</li>
<li>Networking: Fixed problem where HostTopology.MessagePoolSizeGrowthFactor was ignored. (773411)</li>
<li>Networking: Fixed WebGL client unable to free connections in NetworkServer when using WebSocket. (768030)</li>
<li>OpenGL: Fixed a bunch of compute shader structured buffer access corner case issues. (767348)</li>
<li>OpenGL: Fixed invalid shader code generation when using gl_PrimitiveID or bitFieldInsert().</li>
<li>OpenGL: Fixed mislocated fragment shader default float precision. Now also basing the default precision on actual GPU capabilities. (763638)</li>
<li>OpenGL: Fixed multiple simultaneous append/consume compute buffers usage.</li>
<li>OpenGL: Fixed rendering when Graphics.Blit is being called after WaitForEndOfFrame. (784880)</li>
<li>OpenGL: Shader compiler, added unused global uniform pruning.</li>
<li>OpenGL: Shader compiler, avoid temporary variable name collisions. (780831)</li>
<li>OpenGL: Shader compiler, fixed shader translation bugs. (782514)</li>
<li>OpenGL/ES: Fixed GPU profiler on Android for Tegra 2/3/4 devices. (776539)</li>
<li>Particles: Do not restart simulation when becoming visible, and use bigger timesteps, to reduce performance spikes. (765905)</li>
<li>Particles: Fixed a case where if OnWillRenderObject renders, it breaks the main scene. (773226)</li>
<li>Particles: Fixed a crash caused when using Inherit Velocity Module. (783433)</li>
<li>Particles: Fixed a crash when material is missing and mesh colors are requested. (774931)</li>
<li>Particles: Fixed a crash when using SubEmitters with separate rotation axes. (757377)</li>
<li>Particles: Fixed an issue where the Material Property Blocks not working with mesh particles. (776143)</li>
<li>Particles: Fixed batching issues when using multiple cameras in the same position. (788023)</li>
<li>Particles: Fixed culling when using SetParticles. (496494)</li>
<li>Physics: Cloth deletes MeshRenderer component when entering playmode fixed. (769137)</li>
<li>Physics: Disabling cloth component doesn't seem to really disable it fixed. (669622)</li>
<li>Physics: Ensure that OnTriggerExit2D is not called when changing Rigidbody2D.isKinematic property.</li>
<li>Physics: Fix for Collision2D.relativeVelocity being reported with incorrect values. (758422)</li>
<li>Physics: Fixed an issue for 2D collider: line &amp; ray casting not detecting initial overlapped state.</li>
<li>Physics: Fixed an issue with Box2D changes slowing the editor down when lots of changes are made without entering play-mode. (777591)</li>
<li>Physics: Fixed cloth issue where adding cloth to an object throws GetLocalizedString error. (769136)</li>
<li>Physics: Provide feedback to allow working around crashes occurring when input meshes contain invalid vertices. (766891)</li>
<li>Physics2D: Fix to ensure that changing a Collider2D property via the inspector doesn't reset the OnCollision or OnTrigger state back to 'Enter'. (786032)</li>
<li>Physics2D: Fixed a problem where both AreaEffector2D and PointEffector2D scaled-up forces for each additional collider on a rigidbody. (780257)</li>
<li>Physics2D: Fixed a problem where constantly changing an Effector2D collider would mean that no contacts were ever processed stopping the effector from working.</li>
<li>Prefabs: Implemented OnWillSaveAssets callback when applying prefabs. (754351)</li>
<li>Profiler: Fixed a crash when adding data from thread which was started during a frame. (758264)</li>
<li>Resources: Enable warnings for and prevent crashes and memory corruptions when non-assets, or non-unloadable assets are tried to be unloaded through Resources.UnloadAsset in release builds. (767120)</li>
<li>Samsung TV: Enabled a "Show Unity Splash Screen" check box on Samsung TV's PlayerSettings.</li>
<li>Samsung TV: Fixed multiple crashes on the NT14U TV that would prevent games from launching.</li>
<li>SpeedTree: Fixed "GetLocalizedString is not allowed to be called" error message when using the Tree Editor. (779965)</li>
<li>Terrain: Fixed crash when exiting Editor after creating TerrainData with HideAndDontSave flag. (780365)</li>
<li>Tizen: Fixed issue deploying after upgrading to the Tizen 2.4rev4 SDK. (743653)</li>
<li>tvOS: Enabled game controller in tvOS on-screen keyboard. (776446)</li>
<li>tvOS: Fixed a bug that caused splash screen properties being not applied. (775008)</li>
<li>tvOS: Fixed a crash when calling OnDemandResourcesRequest.Dispose() in a coroutine.</li>
<li>tvOS: Fixed build targeting tvOS 9.2 with Xcode 7.3 beta. (770115)</li>
<li>tvOS: Separated tvOS SDK and OS version settings from iOS. (749311)</li>
<li>UI: Fix for child UI elements not being rendered when scaling World Space Canvas from zero. (768807)</li>
<li>UI: Fixed ArgumentOutOfRange exception sometimes being thrown when editing InputField on mobile. (762080)</li>
<li>UI: Fixed dropdown destroy coroutine being started when the component is not active. (758873)</li>
<li>UI: Fixed issue with crash due to dirty renderer being in the dirty list after being destroyed. (764711)</li>
<li>UI: Fixed issue with double rendering of canvas on Vive VR.</li>
<li>UI: Fixed object culling when unparenting from a mask type. (740604)</li>
<li>UI: Fixed Selectable not handling when the EventSystem is null. (788037)</li>
<li>UI: Fixed setting Input Field text when in Decimal/Integer with invalid values.</li>
<li>UI: Setting Input field text through script will now be validated.</li>
<li>UnityWebRequest: Downgrade to HTTP GET on 302 and 303 redirect codes (751798)</li>
<li>UnityWebRequest: Honor negative redirectLimit. (751794)</li>
<li>UWP: Build &amp; Run will correctly work with Universal Windows 10 Apps. (771326)</li>
<li>UWP: Screen.currentResolution will return desktop resolution when application is in windowed mode. (771541)</li>
<li>VisualStudio: Fixed a crash that could sometimes happen when opening Visual Studio.</li>
<li>VR: Fixed an issue with incorrect Render Texture size being used. Most notable with deferred rendering.</li>
<li>VR: VRFocus now respects RunInBackground. Run In Background value of true will now disable rendering if VRFocus is lost.</li>
<li>WebGL: Fixed SimpleWebServer bug causing 'Uncaught incorrect header check'. (770266)</li>
<li>Wii U: Added crash fixes, memory efficiency and 16-bit texture support.</li>
<li>Wii U: Fixed issues causing known crashes.</li>
<li>Windows: SystemInfo.deviceModel will now report model name and manufacturer. (784466)</li>
<li>Windows Standalone: P/Invoke will work correctly with native libraries which reference other native libraries, if those libraries are located in the same directory. (776918)</li>
<li>Windows Store: Assembly-CSharp-firstpass will no longer reference itself. (775216)</li>
<li>Windows Store: Correctly generate Visual Studio namespace when product name contains ' symbol. an underscore will be used instead. (754102)</li>
<li>Windows Store: Disable Generate C# option when scripting backend is set to il2cpp. (775344)</li>
<li>Windows Store: Files located in Assets\Resources won't end up in generated Assembly-CSharp-firstpass project, but will be correctly placed in Assembly-CSharp project.</li>
<li>Windows Store: Fixed $(OutDir) and $(IntDir) paths for generated IL2CPP Visual Studio solutions which prevented appx bundles to build correctly.</li>
<li>Windows Store: Fixed a rare crash at startup related to serialization on debug mode. (778905)</li>
<li>Windows Store: Fixed an assert happening during mesh compression.</li>
<li>Windows Store: Fixed an exception while marshalling UnityEngine.NavMeshTriangulation.</li>
<li>Windows Store: Fixed an issue with populating visual assets (tiles, logos, etc.) to Visual Studio solution (correct file names, manifest entries) and check format consistency (JPEG vs PNG). (775592, 775624, 777575, 777580)</li>
<li>Windows Store: Fixed Build &amp; Run for Universal 8.1 solution. (789538)</li>
<li>Windows Store: Fixed generics related AssemblyConverter failure and give better error messages. (762780)</li>
<li>Windows Store: Fixed incorrect orientation of extended splash screen on Windows Phone 8.1. (770092)</li>
<li>Windows Store: Fixed marshaling of UnityEngine.HumanDescription, previously the field hasTranslationDoF was not mashaled at all.</li>
<li>Windows Store: Fixed marshaling of UnityEngine.SplatPrototype, previously fields specularMetallic, smoothness were not marshaled, because of this sometimes terrain would be rendered incorrectly. (786889)</li>
<li>Windows Store: Fixed Screen.orientation returning AutoRotation on startup. (787522)</li>
<li>Windows Store: Fixed stacktraces on IL2CPP scripting backend. (781907)</li>
<li>Windows Store: Fixed Tab key duplication in XAML controls when Unity input is enabled. (775931)</li>
<li>Windows Store: Fixed www.error return result, previously it would return only an error code, now it will also contain error message returned by the server.</li>
<li>Windows Store: Having many generic types in the project no longer makes .NET Native compiler run out of memory.</li>
<li>Windows Store: Help SerializationWeaver find references which have Windows SDK specified when building to Universal 8.1. (781994)</li>
<li>Windows Store: Hindi characters will show up correctly, Nirmala UI from Windows fonts will be used. (779136)</li>
<li>Windows Store: Package.appxmanifest for Universal Windows 10 Apps will be produced correctly when protocol for association launching is specified. (780971)</li>
<li>Windows Store: RuntimeInitializeOnLoadMethod will work correctly. (777878)</li>
<li>Windows Store: Screen.SetResolution will correctly work on Windows Phone 10. (773877)</li>
<li>Windows Store: Slightly fix generated Assembly-CSharp* projects to fix "System.BadImageFormatException: Duplicate type with name 'UnityEngine.Internal.$FieldNamesStorage' .. " (781935)</li>
<li>Windows Store: EventType.ScrollWheel is now properly detected. (784975)</li>
<li>Windows Store: The maximum amount of characters for short name for tiles will be 40 now. (789439)</li>
<li>Windows Store/IL2CPP: Allow the MapFileParser utility to handle input and output files with paths containing non-ASCII characters. (779968)</li>
<li>Windows Store/IL2CPP: Fixed a crash on windows when using asynchronous socket APIs (.BeginSend/.BeginReceive/etc). (771883)</li>
<li>Windows: Fixed standalone Windows player position when bigger than primary monitor. (760215)</li>
<li>WindowsDownloadAssistant: Fixed setting VisualStudio 2015 as Unity script editor.</li>
<li>WindowsDownloadAssistant: Fixed the bug which was freezing installation UI during bad network connection. (732955)</li>
</ul>

#### Revision: 960ebf59018a
