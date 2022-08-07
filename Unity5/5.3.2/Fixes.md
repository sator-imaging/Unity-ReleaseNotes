# Unity 5.3.2
https://unity3d.com/unity/whats-new/unity-5.3.2

## Fixes

<ul>
<li>Android: Fixed crash when loading many asset bundles. (743739)</li>
<li>Android: Fixed crash in Cloth vertex buffer setup. (750362)</li>
<li>Android: Fixed NullReferenceException on x86 devices running Android 5.0 or newer.</li>
<li>Animation: Fixed an issue with stepped keys having the wrong value. (745139)</li>
<li>Animation: Fixed animation events not firing on the last frame of a looping animation. (745781)</li>
<li>Animation: Fixed crash when deleting all Euler keys in animation curve. (754373)</li>
<li>Animation: Fixed Crossfade called subsequently not properly interrupting transition. (753866)</li>
<li>API Updater: Fixed possible crashes in script updater when resolving types.</li>
<li>AssetBundles: Fixed AssetBundle.CreateFromFile retaining file descriptor. (715753)</li>
<li>AssetBundles: Fixed excessive memory usage when decompressing asset bundles with many objects inside.</li>
<li>AssetBundles: Fixed memory leak when loading asset bundles with LZMA compression.</li>
<li>AssetBundles: Fixed possible asset bundle caching error when starting multiple downloads with an empty cache.</li>
<li>AssetBundles: Fixed the asset bundle reading bug when compressed data could be read as uncompressed.</li>
<li>Core: '~' folders were no longer ignored in projects; fixed. (687655)</li>
<li>DX11: Improved performance in GPU bound scenarios. (747492)</li>
<li>DX11: Fixed wrong VRAM detection on some Intel GPUs, resulting in shadows not being rendered.</li>
<li>DX11/XB1: Fixed FP16 static batched mesh vertex compression to actually work there, was always decompressing to FP32 before.</li>
<li>Editor: Display console platform doc items in the help menu, when console docs are present, but the main documentation is not installed. (754108)</li>
<li>Editor: Fixed MissingMethodException when using some APIs from UnityEngine.WSA namespace.</li>
<li>Editor: Make right and left arrow select next/previous parent for fast expand/collapse in hierarchy views. (752821)</li>
<li>Editor/Scenes: Fixed a crash when trying to get the root count on an invalid Scene. (752423)</li>
<li>Editor/Scenes: Fixed loading new unsaved scene during playmode using Application.LoadLevel(index) or SceneManager.LoadScene(index). (751923)</li>
<li>Editor/Scenes: Fixed the issue that script association was lost when another scene was loaded. (748904)</li>
<li>Editor/Scenes: Fixed the issue that the unloaded scenes would be removed from the hierarchy when entering playmode, if they were first in the hierarchy.</li>
<li>Editor/Scenes: Now make sure inspector in ActiveEditorTracker for MonoBehaviours are not garbage collected. The ActiveEditorTracked manages the objects itself. (753550)</li>
<li>Editor/Scenes: Throw null reference exception if SerializedObject has been disposed. (752599)</li>
<li>Global Illumination: Enlighten; fixed an issue where Unity crashed if scene was unloaded before it got a chance to fully load. (740808, 747666)</li>
<li>Global Illumination: Fixed light probes / skybox ambient being wrong in some cases, 5.3 regression. (754898)</li>
<li>Graphics: More consistency between editor &amp; player when setting up color space sRGB write modes. (754487)</li>
<li>Graphics: Fixed an issue where enabling vertex compression for positions could result in geometry not being rendered. (754928)</li>
<li>Graphics: Realtime reflection probes in some cases did not have trilinear filtering properly set on them; fixed. (752879)</li>
<li>Graphics: Fixed crash when setting shader properties.</li>
<li>IL2CPP: Do not incorrectly free blittable arrays marshaled as [In,Out] parameters. (760943)</li>
<li>IL2CPP: Ensure that the header file for a type defined in a different assembly is included when that type is used for a method parameter. (755088)</li>
<li>IL2CPP: Ensure thread ID is valid for all threads. (691038)</li>
<li>IL2CPP: Fixed an issue that caused a crash in Class::IsSubclassOf. (752737), (751428)</li>
<li>IL2CPP: Fixed double.Parse with InvariantCulture. (752197)</li>
<li>IL2CPP: Fixed ExecutionEngineException being thrown on System.Reflection.MonoProperty::GetterAdapterFrame. (737529)</li>
<li>IL2CPP: Fixed StateMachineBehaviour messages not being executed if stripping is enabled. (753610)</li>
<li>IL2CPP: Forward declare a type and marshaled type in the method declarations header for marshaling methods so that the order of includes does not matter. (756447)</li>
<li>IL2CPP: Implemented out marshaling for arrays correctly. (752153)</li>
<li>IL2CPP: Implemented support for MetadataToken property on the following types: FieldInfo, EventInfo, MethodInfo, ConstructorInfo, PropertyInfo, Type, and Module. (670027)</li>
<li>IL2CPP: Implemented the Thread::Abort and Thread::ResetAbort methods. This should allow a Socket to be closed properly while another thread is waiting in a call to Accept or Connect on that socket. (746822)</li>
<li>IL2CPP: Prevent a NotImplementedException exception from occurring in il2cpp.exe when the Unbox opcode is used with certain generics. This usually occurs when an assembly is built with Visual Studio. (758926)</li>
<li>IL2CPP: Properly cleanup when a native thread is cancelled rather than exiting normally. (749988, 733609)</li>
<li>IL2CPP: Provide a proper argument for instance methods on value types invoked via a delegate. (750153)</li>
<li>IL2CPP: Removed an unnecessary Box used to null check before calling a virtual method.</li>
<li>iOS: Added font containing Lao characters to the fallback list. (750357)</li>
<li>iOS: Added Xcode 7.2 to iOS plugin compatibility list. (750311)</li>
<li>iOS: Duplicate another image layer when not all are defined. (749289)</li>
<li>iOS: Fixed Apple Pencil position reporting on iPad Pro.</li>
<li>iOS: Hindi characters are displayed now. (725558)</li>
<li>iOS/IL2CPP: Correct stack traces in exception messages, which could sometimes miss managed frames. (754539)</li>
<li>iOS/IL2CPP: Fire all GC profiler events. Fixed GC data in internal profiler.</li>
<li>iOS/tvOS: Build all object files with correct SDK. (755365)</li>
<li>Linux: Fixed a corner case where tearing would occur on some window managers even with VSync enabled.</li>
<li>Mecanim: Fixed a bug where Euler rotations would be retained in scene after scrubbing animation. (754562)</li>
<li>Mecanim: Fixed a bug where Euler rotations would not work in Legacy Animations. (752955)</li>
<li>Mecanim: Fixed a bug where lights would not be animated in Legacy mode. (753595)</li>
<li>Mecanim: Fixed a bug where RectTransform couldn't be animated in Legacy. (752847)</li>
<li>Metal: Wrongly claimed to support DXT1/DXT5 texture formats on iOS, and ETC on Mac.</li>
<li>Mono: Preserve non-volatile XMM registers across calls on 64-bit Windows during JIT compilation. (691466)</li>
<li>Networking: Added a 'connecting' state and cancel button to NetworkManagerHUD UI to prevent multiple attempts to connect at the same time. (748936)</li>
<li>Networking: Fixed 'recursion depth exceeded' error for complex NetworkBehaviour scripts. (757766)</li>
<li>Networking: Fixed ClientScene object list being wrong after host migration. (746011)</li>
<li>Networking: Fixed NetworkAnimator not working for non-player objects (755391)</li>
<li>Networking: Fixed NetworkServer.SendToAll sends the message to the host twice. (756153)</li>
<li>Networking: Fixed SyncEvent regression issue. (755450)</li>
<li>Networking: Fixed SyncList updates don't use a configurable network channel. (745795)</li>
<li>Networking: Fixed UI that allowed host migration to be enabled for WebGl platform where it is not supported. (744002)</li>
<li>Networking: OnStopAuthority called on server when it should not be. (751239)</li>
<li>Networking: Prevent [Command] functions from accepting NetworkConnection objects as parameters, which causes a UNetWeaver error. (729157)</li>
<li>Networking: Prevent NetworkIdentity objects from being server-only and local-player-authority at the same time, as this is not a valid configuration. (749338)</li>
<li>OpenGL Core: Fixed a crash with AMD and NVIDIA on Windows when using RenderTexture with recent drivers.</li>
<li>OpenGL Core: Fixed a crash with Intel GPUs on Linux.</li>
<li>OpenGL Core: Fixed shaders with multiple constant arrays.</li>
<li>OpenGL Core: Fixed text rendering with AMD GPUs on OSX 10.9.</li>
<li>OpenGL ES: Fixed crashes with new Samsung firmware. (756734, 756754)</li>
<li>OpenGL ES: Fixed mipmap generation for render textures. (751743)</li>
<li>OpenGL: Fixed binary shader cache, cache was always disabled. (742591)</li>
<li>OpenGL (legacy): Added work around buffer state tracking failure.</li>
<li>Particles: Fixed error message spam on particle systems that have no particles (5.3.1 regression). (755423)</li>
<li>Physics: Fixed memory corruption/crash when deactivating a collider from inside of OnTriggerStay. (744007)</li>
<li>Physics: PlatformEffector2D now supports negative scaling on parent Transform. (755612)</li>
<li>Profiler: Fixed excessive memory usage in development players.</li>
<li>Samsung TV: Fixed the smarthub button problem.</li>
<li>Samsung TV: Fixed wrong JPG library access problem.</li>
<li>Scripting: UnusedByteCodeStripper2 will show a better error message when processing assemblies, so it will be easier to identify offending assembly. (750266)</li>
<li>Shaders: During surface shader generation, do not initialise non-vector type members of the Input struct i.e. a struct/int/matrix as a member variable of the Input struct. (759336)</li>
<li>Shaders: Fixed a bug in Standard shader GGX specular term, introduced in 5.3.</li>
<li>Shaders: More proper environment reflection in Standard shader for very rough surfaces.</li>
<li>Substance: Fixed a crash when checking/unchecking  'Generate all outputs' or 'Generate mipmaps' on OSX. (752039)</li>
<li>Substance: Fixed a crash when reimporting SBSARs with multiple material instances on OSX. (751300)</li>
<li>Substance: Fixed a rare crash that could happen around the destruction of animated ProceduralMaterials. (750442)</li>
<li>Substance: Fixed console spam about unavailable material properties.</li>
<li>Substance: Fixed editor stutter when using RebuildTextures on OSX. (663236)</li>
<li>Substance: Fixed emission color being set to opaque white when resetting a ProceduralMaterial.</li>
<li>Substance: Fixed textures not properly generated on player awake when affected only by constant inputs. (754556)</li>
<li>Substance: Output textures from ProceduralMaterials without any input are now always generated.</li>
<li>tvOS: Fixed missing symbols for simulator builds. (756044)</li>
<li>tvOS: Fixed rendering path selector in player settings. (753925)</li>
<li>tvOS: Fixed UnityEngine.Apple.TV.Remote API access in editor.</li>
<li>UI: Added fix so that the placeholder text is enabled when the InputField is deactivated and the text is empty.</li>
<li>UI: Fixed crash in some cases after deleting world space Canvas. (740782)</li>
<li>UI: Removed remaining uses of multiple display system (temporary fix while non-native resolutions are not supported). (741751)</li>
<li>VR: Fixed Lines &amp; Trail rendering; was offset for one eye. (754068)</li>
<li>VR: Fixed Render Scale not reverting after being edited in play mode. (731324)</li>
<li>VR: Fixed VRDevice.isPresent reporting true on first frame if Device was not connected at start. (732236)</li>
<li>VR: Stereo Cameras correctly respect camera depth when rendering to the game view and HMD. (753256)</li>
<li>WebGL: Fixed a crash when setting Application.runInBackground, if Strip Engine Code is enabled. (758120)</li>
<li>WebGL: Prevent browser from processing Arrow Keys. (740182)</li>
<li>WebGL: Prevent browser from processing Backspace and Tab key presses. (747236)</li>
<li>Windows Store: Fixed incorrect display of Korean characters on Windows 10 (if Korean language pack is not installed) and Windows Phone 10, Unity will now fallback to "Malgun Gothic" font.</li>
<li>Windows Store: Fixed Directory.CreateDirectory() for forward slashes. (752546)</li>
<li>Windows Store: Populate autorotation settings to screen manager. (751207)</li>
<li>Windows Store: Fixed a build failure (rrw failure) when calling methods with System.Numerics.Matrix4x4 as parameter. (754533)</li>
<li>Windows Store: Fixed AccessViolationException when initializing matchmaking in UNet. (747549)</li>
<li>Windows Store: Fixed player crashing on startup on .NET scripting backend. (746301)</li>
<li>Windows Store: Fixed Screen.SetResolution when upscaling lower resolution to fullscreen, previously you would see a corrupt image on the screen. (756086)</li>
<li>Windows Store: Fixed TouchScreenKeyboard crashes when it's members are used immediately after Open(). (755473)</li>
<li>Windows Store: Fixed WheelCollider on x64 (NullReferenceException occurring). (730289)</li>
<li>Windows Store: RunInBackground option will be respected when application window looses focus, and if enabled, the application will keep updating. Note: if application window is minimized it will be still paused, because OS suspends the application. (759166)</li>
</ul>

#### Revision: e87ab445ead0
