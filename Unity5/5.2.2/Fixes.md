# Unity 5.2.2
https://unity3d.com/unity/whats-new/unity-5.2.2

## Fixes

<ul>
<li>(none) -  2D: Exposed alpha texture api for atlases compressed with ETC1.</li>
<li>(705196) -  Android: Fix for missing SpeedTree leaves when using and 'best' quality wind zones on Adreno 3xx with OpenGL ES 3.0.</li>
<li>(724509) -  Android: Fixed a problem where Plugins/Android/res wasn't bundled with the application.</li>
<li>(725153) -  Android: Fixed an issue where passing large JNI arrays would cause a local reference table overflow.</li>
<li>(720706) -  Android: Fixed crash in ASTC encoder.</li>
<li>(726878) -  Android: Fixed MSAA on newer Mali drivers such as SGS6.</li>
<li>(710191) -  Android: Fixed reported texture size in profiler for formats that are decompressed during upload.</li>
<li>(718206) -  Android: IL2CPP - Fixed compilation on DLLs with spaces.</li>
<li>(726121) -  Android: IL2CPP - Fixed crash on startup when OBB is enabled.</li>
<li>(none) -  Asset Loading: Serialisation errors that produce "serialisation layout mismatch" errors will now attempt to include the name of the root type being serialised when the error was encountered.</li>
<li>(730952) -  Build Pipeline: Fixed warning message "Failed to add the asset file size for&nbsp;filename".</li>
<li>(none) -  D3D11: ChangeDisplaySettings(..., CDS_TEST) causes stuttering on nvidias. Use DXGI instead.</li>
<li>(724093) -  Direct3D 11: Changing resolution through script will not stretch the screen anymore.</li>
<li>(726343) -  Editor: Fixed "Ctrl" click on object selects another object in scene view.</li>
<li>(726373) -  Editor: Fixed background object getting selected instead of the one in the front.</li>
<li>(699420) -  Editor: Fixed baking navmesh while building lighting.</li>
<li>(713420) -  Editor: Fixed crash when opening Frame Debugger that was happening on some machines (mostly Macs with NVIDIA GPUs).</li>
<li>(732454), (733335) -  Editor: Fixed crash when trying to build Universal Windows 10 Apps, but Windows 10 SDK is not installed.</li>
<li>(723116) -  Editor: Fixed Gizmos.DrawLine rendering with random colors when 3D Icons is turned off.</li>
<li>(none) -  Editor: Fixed HideFlags.DontSaveInBuild and HideFlags.DontUnloadUnusedAsset being swapped.</li>
<li>(712517) -  Editor: Support nested scene loading after introducing multi-scene-editing.</li>
<li>(719769) -  Editor: The selected platform is now properly switch when launching Unity through the command line with the –buildTarget switch.</li>
<li>(725677) -  FinalGather: "Template function should be specialized" error thrown when baking.</li>
<li>Mecanim :  Fixed Humanoid layer mask not working with AnimatorControllerPlayables.</li>
<li>(725106) -  Fixed issue with inputfield caret/ highlight not displaying</li>
<li>(none) -  Fixed issue with launching both MonoDevelop and Xamarin Studio when external script editor is set to Xamarin Studio on OSX.</li>
<li>(649000), (721553) -  Fixed Unity crash when inspecting UnityEditor.VersionControl.Asset while debugging.</li>
<li>(711044) -  Fixed: Cache Server crashes on command 'nc -zv'</li>
<li>(725070) -  GI: Fixed crash when switching scenes in specific circumstances.</li>
<li>(none) -  GI. Fixed crash when generating lightmaps.</li>
<li>(none) -  GLES: GLLEGACY: Fixed: glClear doesn't obey viewport, so render a quad instead when doing a non-fullscreen clear.</li>
<li>(none) -  GLLEGACY: Fixed: readpixels needs workaround for MSAA.</li>
<li>(726172) -  Graphics: Do not return pre-created RenderTextures from RenderTexture.GetTemporary; makes it possible to set useMipMap on them again.</li>
<li>(686243) -  Graphics: Fixed an issue whereby static batching didn't work in the Editor when scenes were loading from scripts e.g. Application.LoadLevel()</li>
<li>(730772), (722618) -  Graphics: Fixed resolution switches sometimes incorrect in DX11.</li>
<li>(730772), (728756) -  Graphics: Fixed UI disappearing when triggering a resolution change in DX9 standalone.</li>
<li>(729286) -  Graphics: Texture2D.format shows ARGB on RGB texture format.</li>
<li>(730541) -  Home Window: Make survey only show correct questions.</li>
<li>(731652) -  IL2CPP: Allow default parameter values for nullable types to be converted to C++ correctly.</li>
<li>(721065) -  IL2CPP: Convert I18N.dll assemblies if they are present to avoid not supported exceptions for some code pages.</li>
<li>(692240) -  IL2CPP: Corrected method collection in editor to preserve defining class rather than invoked class in some cases.</li>
<li>(732205) -  IL2CPP: Corrected the behavior of Array.SetValue and Array.GetValue for integer values used with an enum array.</li>
<li>(730563) -  IL2CPP: Corrected the generated C++ code when MonoPInvokeCallback is used to specify a type which has marshaling directives. The marshaling directives from that type will be used, and a compile error in the generated C++ code will no longer occur.</li>
<li>(707376) -  IL2CPP: Ensure IL2CPP generates valid numeric identifiers under all system languages.</li>
<li>(719378) -  IL2CPP: Ensure PreserveAttribute on type preserves default constructor.</li>
<li>(732814) -  IL2CPP: Fixed a crash in the il2cpp::icalls::mscorlib::System::Reflection::MonoMethod::get_base_definition method.</li>
<li>(703908) -  IL2CPP: Fixed Directory.GetFiles using search pattern with embedded '*'.</li>
<li>(722920) -  IL2CPP: Fixed race condition when accessing attributes.</li>
<li>(718708) -  IL2CPP: Generate correct C++ code when an extension method as a constrained generic type which is another generic type defined in a different assembly.</li>
<li>(719718) -  IL2CPP: Include assemblies referenced only by prefabs in the Resources folder in the build.</li>
<li>(732317) -  IL2CPP: Prevent a possible deadlock when using System.Threading.ReaderWriterLock.</li>
<li>(728134) -  iOS: Fixed Game Center authentication crash on iOS 9.0.</li>
<li>(722963) -  iOS: Fixed memory leak when changing orientation.</li>
<li>(730886) -  iOS: Fixed some corner cases of AA and image effects on OpenGL ES.</li>
<li>(725085) -  iOS: Made iAD code more robust on ios9: Fullscreen Ads now work and Banners do not crash on destruction.</li>
<li>(none) -  iOS: Pick 2-nd stage splash screens from asset catalogs when possible.</li>
<li>(714759) -  iOS/IL2CPP: Implement host name resolution with IPv6</li>
<li>(729165) -  iOS/IL2CPP: Prevent a crash that occurs when using Unity Ads and GameCenter together.</li>
<li>(721644) -  LegacyShaders: (Self-Illumin) No Emission (Lightmapper) component after Unity 5.</li>
<li>(none) -  Linux: Handle failure to create input method / input context on startup.</li>
<li>(none) -  Linux: Ignore driver-reported joystick axes with invalid range / fix mapping for these devices.</li>
<li>(713205) -  Linux/Tizen/STV: Fixed "special" characters (e.g. &amp;) in player pref names.</li>
<li>(728874) - Mecanim : Animator parameter gets 0/false value when animator not enabled.</li>
<li>(726413) -  Mecanim: Fixed AnimationEvents fired on animations that are weighted-out.</li>
<li>(718748) -  Mecanim: Fixed Animator memory being cleared when disabling the component the same behaviour as before 5.2b5 do not clear animator memory when only the animator.</li>
<li>(726448) -  Mecanim: Fixed Animator::Play generating invalid AnimationEvent invocations.</li>
<li>(730175) -  Mecanim: Fixed Animator.GetParameter throwing exceptions.</li>
<li>(727580) -  Mecanim: Fixed Animator.Play not working when AnimatorController.</li>
<li>(725512) -  Mecanim: Fixed AssetBundle created from 5.1 crashing in 5.2.</li>
<li>(729181), (730491), (729203), (730205) -  Mecanim: Fixed bad 1st frame when enabling Animator.</li>
<li>(726168) -  Mecanim: Fixed blending of rotations beign broken in some situations.</li>
<li>(726301) -  Mecanim: Fixed crash when Animator.speed is set to zero during transition.</li>
<li>(727765) -  Mecanim: Fixed crash when calling Animator.GetCurrentAnimatorClipInfo during an interrupted transition.</li>
<li>(730469) -  Mecanim: Fixed crash when calling Update() from OnStateEnter.</li>
<li>(724249) -  Mecanim: Fixed crash when changing Animator.updateMode in PlayMode.</li>
<li>(730086) -  Mecanim: Fixed crash when modifying in Playmode an AnimatorController used in Playable.</li>
<li>(726627) -  Mecanim: Fixed crash when multiple triggers happen on the same frame.</li>
<li>(726627) -  Mecanim: Fixed crash when setting invalid OverrideController.</li>
<li>(726426) -  Mecanim: Fixed crash when switching to empty controller.</li>
<li>(726871) -  Mecanim: Fixed crash with WriteDefaultValues set to false on an empty state.</li>
<li>(725767) -  Mecanim: Fixed game object with override controller not showing the base controller when selecting the GameObject.</li>
<li>(721127) -  Mecanim: Fixed IK not applied on feet when last layer does not have Foot IK active.</li>
<li>(729924) - Mecanim: Fixed issues with Animator view synchronization.</li>
<li>(719911) -  Mecanim: Fixed parameters not being evaluated when AnimatorController used in Playable.</li>
<li>(726207) -  Mecanim: Fixed transition to empty state on layers not driving layer weight.</li>
<li>(721499) -  Networking: Fix for 'aissp' error is thrown on the server side when a client disconnects.</li>
<li>(none) -  Networking: Fix for server websocket crashing in release mode.</li>
<li>(720747) -  Networking: Fixed Editor crashes on websocket disconnect.</li>
<li>(718824) -  Networking: Fixed: UNET doesn't check message length correct.</li>
<li>(719672) -  Networking: Fixed: User can create packet larger then defined in global config.</li>
<li>(718822) -  Networking: Fixed: User can set MinThreadAwakeTimeout to 0</li>
<li>(728735) -  Networking: Setup network authority properly for scene objects, and made NetworkTranform handle multiple authority changes.</li>
<li>(none) -  Networking: Support for UNet HLAPI on WebGL platform. 
<ul>
<li>Added useWebSockets field to NetworkManager and NetworkServer. When this is checked, the system will listen for WebSocket connects instead of the normal UNet Transport layer connections. This allows WebGL clients to connect to the server.</li>
<li>Fixed DNS issues using UNet on WebGL platform.</li>
<li>Fixed HLAPI update pump function on WebGL platform.</li>
</ul></li>
<li>(732956) -  OpenGL &amp; OSX: Fixed scene view picking when AA is enabled.</li>
<li>(725329), (730178) -  OSX: Fixed external texture crash with OpenGL2 device.</li>
<li>(726017) -  OSX: Fixed Input.GetKey and Input.inputString not working.</li>
<li>(496494) -  Particles: Fixing culling issue when SetParticles was called from script with 0 lifetime.</li>
<li>(719113) -  Physics: Added PlatformEffector2D.sideArc to replace PlatformEffector2D.sideAngleVariance as well as adding the missing gizmo for sides.</li>
<li>(730513) -  Physics: Fixed changes made to wheel collider's properties in Update causing wheel collider to twitch due to interpolation.</li>
<li>(719296) -  Physics: Fixed scaling of cars that had center of mass not at the Rigidbody's origin.</li>
<li>(697547) -  Physics: Restore the Rigidbody2D linear-velocity after a Rigidbody2D.MovePosition has completed.</li>
<li>(none) -  Samsung TV: Fixed problem where GUI controls would become unresponsive.</li>
<li>(568430) -  Script Debugging: Fixed issue with stepping in switch statements.</li>
<li>(691014) -  Script Debugging: Fixed occasional Unity crash when stepping many times in a row and then hitting a breakpoint.</li>
<li>(626569) -  Script Debugging: Fixed rare Unity crash when stepping.</li>
<li>(721288) -  Script Debugging: Fixed stepping over Resources.Load and other Unity API methods that use serialization.</li>
<li>(589577) -  Script Debugging: Fixed Unity crash when trying to evaluate generic methods that return an array of the generic type. Such as GameObject.GetComponents().</li>
<li>(717289) -  Script Debugging: Fixed Unity crash when trying to step after pause.</li>
<li>(none) - Script Debugging: Fixed Unity crash when debugging with Visual Studio Tools for Unity 2.1.</li>
<li>(none) -  Scripting: 'Editor' folders inside 'Plugins', 'Standard Assets' and 'Pro Standard Assets' no longer need to be at the root of those directories.</li>
<li>(382005) -  Scripting: Don't crash in mono_metadata_free_type when handed a null type instance.</li>
<li>(716872) -  Scripting: Fixed Unity crash when assembly references type in another assembly that is not present in the project.</li>
<li>(719574) -  Shaders: Fixed a crash that could happen when loading legacy shaders.</li>
<li>(712400) -  Shaders: Fixed the surface lighting model (alpha:auto) picking incorrect blend mode (alpha:premul) in legacy lighting functions.</li>
<li>(717292) -  Substance: Cached data written to disk by 32b and 64b players are now the same.</li>
<li>(716513) -  Substance: Fewer texture computations should now occur at the end of an asset import, which speeds up material instance addition/deletion.</li>
<li>(none) -  Substance: Fixed auto-setting of emissive-related properties when importing materials with emissive outputs.</li>
<li>(none) -  Substance: Fixed inspector sluggishness when a lot of visibleIf expressions are present (B2M for instance).</li>
<li>(722757) -  Substance: If unassigned, the _MainTex shader slot is now only auto-filled if nothing else was assigned to the current shader.</li>
<li>(732399) -  Substance: ProceduralMaterials should now be correctly rendered after a color space switch.</li>
<li>(none) -  Substance: Re-importing a ProceduralMaterial should no longer cause its texture thumbnails to disappear.</li>
<li>(725995) -  Substance: Runtime-instantiated ProceduralMaterials now update their own textures.</li>
<li>(729904) -  Substance: Standalone builds will no longer crash when trying to read cache data created by prior builds.</li>
<li>(697741) -  Substance: Storage size is now correctly reported for ProceduralTextures.</li>
<li>(707737) -  Substance: Unapplied import settings being discarded will cause an apply/revert dialog box to be displayed.</li>
<li>(none) -  Tizen: Deploying from Tizen SDK 2.3.1 is now supported.</li>
<li>(none) -  Tizen: Fixed a bug preventing the system notification bar from working.</li>
<li>(none) -  Tizen: Fixed a couple issues with audio using too much CPU time when Unity apps are in the background.</li>
<li>(none) -  Tizen: Fixed an issue where the audio thread would still do work when an app was in the background or the device locked.</li>
<li>(729291) -  Tizen: Fixed an issue with some keys on the software keyboard not working as expected.</li>
<li>(none) -  Tizen: Fixed WWW class failures when using https</li>
<li>(none) -  Tizen: Hide the textfield cursor to match behavior of our other mobile platforms.</li>
<li>(729291) -  Tizen: Resolved double keyboard input issue.</li>
<li>(633717) -  UI: Added [DisallowMultipleComponent] to Mask, RectMask2D, ScrollRect, and ToggleGroup</li>
<li>(none) -  UI: Added clear function to vertex helper.</li>
<li>(none) -  UI: Big fixes to GC pressure. We were non optimally creating garbage in the UI system when we should not have been.</li>
<li>(710495) -  UI: Do not render elements with an alpha == 0 or color.a == 0.</li>
<li>(709485) -  UI: Ensure that when a mask is disabled it does not filter pointer events.</li>
<li>(none) -  UI: Fix for multiple InputFields in a scene having a text being input in one field incorrectly changing the display of other fields while the keyboard is open.</li>
<li>(725938) -  UI: Fixed an issue where canvas initialization order was 'important' (it should not be). This was causing elements to be located on the wrong part of the screen.</li>
<li>(707026) -  UI: Fixed an issue where raycast result had the wrong ID which would break sorting.</li>
<li>(727000) -  UI: Fixed bad memory leak in canvas rendering caused by index buffer growing when it is not meant to. </li>
<li>(715921) -  UI: Fixed crash in best fit text rendering when canvas scaler has a scale of 0.</li>
<li>(727699) -  UI: Fixed crash on Mac when exiting play mode with a maximized game view.</li>
<li>(715921) -  UI: Fixed editor hang when attempting to cache a calculated font size &gt; 500 as a result of a canvas scaler.</li>
<li>(none) -  UI: Fixed performance regression in the UI system caused by accessing a mesh repeatedly. Fix is to use the UI helper class and only finalize to mesh as the last step. We've had to add a backwards compatibility flag to Graphic for determining if we should use mesh (now legacy) or VertexHelper. Both code paths work, but the new one is faster if you are using effects.</li>
<li>(none) -  UI: If the parent canvas changes update the drawing matrix to match.</li>
<li>(none) -  UI: Image will now use the white texture again if no texture is specified.</li>
<li>(none) -  UI: Invalid graphics need to clear the VertexHelper instead of using previous data.</li>
<li>(none) -  UI: Make sure the VertexHelper for Filled sprites are cleared before trying to add new data.</li>
<li>(632690) -  UI: Removed arbitrary limitation on the number of vertices generated by an image set to tiled mode.</li>
<li>(718250) -  UI: Return the correct Canvas rectangle when using nested canvases. We were returning the incorrect Canvas rectangle previously.</li>
<li>(625577) -  UI: Set velocity to 0 when a ScrollRect is disabled.</li>
<li>(726093) -  Universal Windows Apps: Assembly-CSharp projects are generated in subfolder so they wouldn't conflict with other projects in the root folder.</li>
<li>(726816) -  Universal Windows Apps: AssemblyConverter will correctly find Windows.winmd file when patching assemblies.</li>
<li>(728098) -  Universal WIndows Apps: Fixed compilation error which happened with extension APIs.</li>
<li>(728025) -  Universal Windows Apps: ReferenceRefwriter will correctly find *.winmd files from C:\Program Files (x86)\Windows Kits\10\References.</li>
<li>(none) -  Universal Windows Apps: Removed APIs from WinRTLegacy which were reintroduced by Microsoft in .NET Core 5.0. This should fix errors where same class is implemented both in WinRTLegacy.dll and System.*.dll .</li>
<li>(723821) -  Unregister http request callbacks on WWW destruction.</li>
<li>(730014) -  Version Control: Fixed slowdown in editor when connected to a version control backend e.g. Perforce or Plastic SCM.</li>
<li>(none) -  Visual Studio Integration: More robust error checking &amp; retry logic when opening visual studio.</li>
<li>(none) -  Visual Studio Integration: On mac, no longer ignore UnityVS assemblies in the assetsfolder, so that win-&gt;mac debugging works again</li>
<li>(715858), (726292) -  VR: Changing renderscale now reallocates to desired texture size in all cases.</li>
<li>(none) -  VR: D3D11 adapter ID now used to identify device if disconnected.</li>
<li>(726878) -  VR: Fixed anti aliasing on Samsung Galaxy S6 GearVR.</li>
<li>(720390) -  VR: Fixed aspect ratio value not correctly being set on Camera component. Also fixes reflections when tilting.</li>
<li>(716500) -  VR: Fixed Camera.stereoMirrorMode bug where right eye would display black or last frame when in mirror mode. Now displays left eye Image.</li>
<li>(none) -  VR: Fixed play mode crash when using MSAA on OSX.</li>
<li>(none) -  VR: Fixed startup crash when using D3D11.</li>
<li>(721694) -  VR: Fixed VRSettings.showDeviceView showing the last frame in the VR headset. Now clear's to camera's background color.</li>
<li>(none) -  VR: Fixed vsync disable not working correctly.</li>
<li>(none) - VR: Fixed Multithreaded Rendering crash on GearVR.</li>
<li>(none) -  VR: Removed extra blit from PC rendering path.</li>
<li>(none) -  WebGL: Workaround for IndexedDB not available in Firefox when running in iframe.</li>
<li>(none) -  WebRequest: Asset bundle loading.</li>
<li>(720416) -  WebRequest: Some headers are missed in the response.</li>
<li>(710903) -  Windows Phone 8: Fixed an issue affecting build and run for projects with spaces in their names.</li>
<li>(726088) -  Windows Store Apps: AssemblyConverter fixes for array handling and assembly resolving.</li>
<li>(none) -  Windows Store Apps: Fixed AssemblyConverter incorrectly picking native dll's, when there's winmd with same name.</li>
<li>(729507) -  Windows Store Apps: Unity will correctly generate Universal 8.1 projects, VS 2013 and VS 2015 should open them correctly.</li>
<li>(729551) -  Windows Store: Back button will be consumed in Universal Windows 10 Apps, you can detect with Input.GetKey(Keycode.Escape)</li>
<li>(724566) -  Windows Store: BuildPipeline.BuildPlayer works with relative paths.</li>
<li>(723973), (715315) -  Windows Store: Correctly generate Visual Studio project when product name begins with number or contains symbols '(' or ')'.</li>
<li>(625473) -  Windows Store: Default font is loaded from system folder.</li>
<li>(731088) -  Windows Store: Fixed crash in Universal Windows 10 apps when you click in the UI text field.</li>
<li>(710668) -  WSA/UWP: Fixed black screen when using Linear Color Space and Anti Aliasing.</li>
</ul>
