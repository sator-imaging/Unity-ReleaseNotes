# Unity 5.0.2
https://unity3d.com/unity/whats-new/unity-5.0.2

## Fixes

<ul>
<li>AI: Allow setting slope above 60 deg by using serialized object.</li>
<li>AI: Fixed buggy example code for script API example.</li>
<li>AI: Handle out of memory when building huge world.</li>
<li>Android: Apply Holo or Material theme if the user did not specify other explicitly.</li>
<li>Android: Apply user theme if set.</li>
<li>Android: Fixed crash in Mono caused invocation of wrong method.</li>
<li>Android: Fixed crash on Application.Quit().</li>
<li>Android: Fixed issues with soft input caused by Samsung back button fix</li>
<li>Android: Fixed window buffer leakage</li>
<li>Android: Improved soft input dialog.</li>
<li>APIUpdater: APIUpdater assumes script encoding is UTF-8.</li>
<li>APIUpdater: APIUpdater crashes when updating methods that return arrays of generic types.</li>
<li>APIUpdater: Unity imports/upgrades DLL built for 4.x twice and it throws errors after first import.</li>
<li>Asset Bundles: AssetBundle.CreateFromMemory with uncompressed bundles will no longer block the main thread for several seconds.</li>
<li>Asset Importing: Fixed importing of an assembly that contains classes inherited from generic engine's classes.</li>
<li>Asset Management: PluginImporter settings for OSX native plugins will no longer be lost in .unitypackage files.</li>
<li>AssetBundle: Fixed the issue that prefab loaded from AssetBundle lost the reference to a material in a variant AssetBundle.</li>
<li>AssetBundle: Fixed the issue that scene AssetBundle didn't get rebuilt when the referenced prefabs were changed.</li>
<li>AssetBundle: Make the error message more informative when building AssetBundles.</li>
<li>D3D11: Fixed shaders that use min16float types.</li>
<li>Documentation: Fixes for 5.0, removed the "Overview" link.</li>
<li>Documentation: A number of bugs have been fixed.</li>
<li>Documentation: Ridigbody typos fixed.</li>
<li>Editor - Other: Fixed ScriptableObject assets to pull icons correctly from their associated script</li>
<li>Editor: Android - Fixed updating SDK on x86 Java on Windows.</li>
<li>Editor: Fixed crash when PlayerSettings.GetPropertyString is called for not existing property.</li>
<li>Editor: Fixed Camera.SetTargetBuffers with AA-ed renderbuffers.</li>
<li>Editor: Scene View content is no longer tinted in playmode.</li>
<li>GI: Ambient light is not shown after baked data is cleared.</li>
<li>GI: Entering play mode while baking with on demand makes bake indication get stuck and game show incorrect result.</li>
<li>GI: Fixed crash caused by Unity reading GI files as resource files and a certain GI file had data that looked like a header but caused a huge allocation.</li>
<li>GI: Fixed lightmap resolution overlay not showing up on Terrains.</li>
<li>GI: Reloading scene makes the background darker.</li>
<li>GI: With continuous baking enabled and baked light, light probes stop working after exiting play mode.</li>
<li>Graphics: Fixed double-fog in deferred shading + forward-only opaque objects + GlobalFog effect.</li>
<li>Graphics: Fixed printing of some loops in GLSL/Metal.</li>
<li>Graphics: Improved rough front-to-back sorting for opaque objects, for better GPU Z culling efficiency.</li>
<li>IMGUI: Fixed calculation of TextGenerator vertices position when lineSpacing is 0.</li>
<li>Input: Input.GetJoystickNames() on Windows no longer returns a single blank entry when no joysticks are connected.</li>
<li>Input: Input.mousePosition is clamped correctly when a Windows player is resized.</li>
<li>iOS: Added dummy vertex channel for missing shader channels when dynamic batching.</li>
<li>iOS: Added Xcode 6.3 Build &amp; Run support.</li>
<li>iOS: Fixed crash when rendering empty meshes.</li>
<li>iOS: Fixed HTTPs problem.</li>
<li>iOS: Fixed memory corruption and crash initiated by calling WebCamTexture.Stop().</li>
<li>iOS: Fixed memory leak in iOS WebCamTexture.GetPixels().</li>
<li>iOS: Fixed crash on rendering empty meshes.</li>
<li>iOS: Fixed duplicate property value removal in certain Xcode projects.</li>
<li>iOS: Fixed WebCamTexture.didUpdateThisFrame.</li>
<li>iOS: Fixed assert in corner case when webcam code is trying to pick supported FPS.</li>
<li>iOS/IL2CPP: Add a null terminator to string arrays when they are marshaled.</li>
<li>iOS/IL2CPP: Added support for string.Normalize.</li>
<li>iOS/IL2CPP: Additional code size improvements from generic sharing: 
<ul>
<li>Allow partial sharing (e.g. Dictionary is shared with Dictionary).</li>
<li>Allow sharing when the type parameter constraint is an interface.</li>
<li>Share enums and their base types as generic parameters.</li>
</ul></li>
<li>iOS/IL2CPP: Allow Encoding.GetEncoding to correctly.</li>
<li>iOS/IL2CPP: Allow thread-local static fields to work correctly in generic classes. Specifically, this corrects the Parse SDK crash in 4.6.4p1.</li>
<li>iOS/IL2CPP: AudioMixerSnapshot.TranslateTo no longer throws null reference exception on IL2CPP.</li>
<li>iOS/IL2CPP: AudioMixerSnapshot.TranslateTo no longer throws null reference exception on IL2CPP.</li>
<li>iOS/IL2CPP: Avoid class initialization and metadata construction deadlocks.</li>
<li>iOS/IL2CPP: Cast non-pointer references types to System.Object for comparison in conditional statements.</li>
<li>iOS/IL2CPP: Correct an InvalidCastException that can occur when setting an array value.</li>
<li>iOS/IL2CPP: Correct the behavior of CultureInfo.CreateSpecificCulture.</li>
<li>iOS/IL2CPP: Correctly lazy initialize the type information when Type.GetDeclaringType is called.</li>
<li>iOS/IL2CPP: Do not write extern declarations inside p/invoke wrappers for methods that return a class or delegate.</li>
<li>iOS/IL2CPP: Fix a number of problems related to WebRequest and asynchronous I/O: 
<ul>
<li>Fixed socket I/O requests getting stuck in ThreadPool on POSIX/iOS.</li>
<li>Fixed race condition in Monitor code that lead to 5 second stalls in Monitor.Exit().</li>
<li>Fixed ThreadPool not re-using idle worker threads (lead to potentially very high memory consumption and bad performance).</li>
<li>Fixed ThreadPool upper thread count limits being very low; now roughly the same as on Mono.</li>
<li>Fixed ThreadPool.SetMinThreads() and SetMaxThreads() having no effect.</li>
</ul></li>
<li>iOS/IL2CPP: Fixed an infinite recursion when constructing generic type.</li>
<li>iOS/IL2CPP: Fixed an issue with open delegates that return void.</li>
<li>iOS/IL2CPP: Fixed crashes in socket code due to sockets being destroyed too early and prevent Thread.IsAlive from returning true after thread has terminated.</li>
<li>iOS/IL2CPP: Fixed Interlocked.Exchange and Interlocked.CompareExchange for interfaces.</li>
<li>iOS/IL2CPP: Fixed issue with managed exceptions not being thrown by a method called by Method.Invoke in some cases.</li>
<li>iOS/IL2CPP: Fixed multidimensional array interfaces.</li>
<li>iOS/IL2CPP: Fixed a crash with StrangeIOC.</li>
<li>iOS/IL2CPP: Fixed an issue where IL2CPP would use -&gt; operator on value types in certain cases.</li>
<li>iOS/IL2CPP: Fixed code generation for binary comparisons containing expressions.</li>
<li>iOS/IL2CPP: Fixed code generation for unsafe fixed arrays.</li>
<li>iOS/IL2CPP: Fixed crash in some cases when accessing an enum inside a generic class.</li>
<li>iOS/IL2CPP: Fixed crash related to arrays of Enums on 64-bit.</li>
<li>iOS/IL2CPP: Fixed crash when using weak GC handle onstring constants.</li>
<li>iOS/IL2CPP: Fixed File::Replace when destinationBackupFileName is null.</li>
<li>iOS/IL2CPP: Fixed IL2CPP failing to convert an assembly which contains Ldtoken instruction on field that is declared in a generic type. This issue affected CSVHelper.dll plugin.</li>
<li>iOS/IL2CPP: Fixed issues with exception thrown from DateTime constructor, DateTime ToUniversalTime, DateTime ToLocalTime, DateTime IsDaylightSavingTime.</li>
<li>iOS/IL2CPP: Fixed memory leak when using audio callbacks.</li>
<li>iOS/IL2CPP: Fixed occasional code generation issues when multiple local enum variables are used in conditional expressions.</li>
<li>iOS/IL2CPP: Fixed overflow arithmetic instruction handling.</li>
<li>iOS/IL2CPP: Fixed overflow arithmetic instruction handling.</li>
<li>iOS/IL2CPP: Fixed stripping issue when NavMeshAgent was referenced only from scripts.</li>
<li>iOS/IL2CPP: Fixed support for enums nested in generic types.</li>
<li>iOS/IL2CPP: Fixed support for type/method names using non ASCII characters.</li>
<li>iOS/IL2CPP: Fixed System.Environment.TickCount on iOS.</li>
<li>iOS/IL2CPP: Fixed TerrainData.GetAlphaMaps crashing on IL2CPP.</li>
<li>iOS/IL2CPP: Fixed TerrainData.GetAlphaMaps crashing on IL2CPP.</li>
<li>iOS/IL2CPP: Fixed unordered comparison opcodes code generation.</li>
<li>iOS/IL2CPP: Fixed WebClient requests using a timeout.</li>
<li>iOS/IL2CPP: Forward declare empty types (created to end infinite recursion) that are used as method arguments.</li>
<li>iOS/IL2CPP: Generate C++ code which will compile when a nested generic passes the maximum depth for recursive nested generics.</li>
<li>iOS/IL2CPP: Generate C++ code which will compile when a nested generic passes the maximum depth for recursive nested generics.</li>
<li>iOS/IL2CPP: Implemented Assembly.CodeBase by returning the value of AssemblyName.Name.</li>
<li>iOS/IL2CPP: Implemented Assembly.CodeBase by returning the value of AssemblyName.Name.</li>
<li>iOS/IL2CPP: Make Activator.CreateInstance work for arrays.</li>
<li>iOS/IL2CPP: Match the behavior of the Mono scripting backend by not stripping the Animation code from the engine when code stripping is enabled.</li>
<li>iOS/IL2CPP: Match the Mono behavior which allows inflated generic delegate types like System.Action to be marshaled as normal delegates.</li>
<li>iOS/IL2CPP: Prevent a stack overflow in il2cpp.exe when it converts have an infinitely recursive generic type with an array generic argument.</li>
<li>iOS/IL2CPP: Removed the option to user precompiled headers in the Player Settings, as this option in no longer supported for the IL2CPP scripting backend.</li>
<li>iOS/IL2CPP: Return the correct number of write and error sockets from the Socket::Select method.</li>
<li>iOS/IL2CPP: Support Type.MakeGenericType for runtime creation of generic types where the generic arguments are reference types.</li>
<li>iOS/IL2CPP: Type.GetType throws an ArgumentException now when the provided type name was wrong.</li>
<li>iOS/IL2CPP: Use the proper type for the result of the IL sub opcode.</li>
<li>iOS/IL2CPP: Use the Size field of the StructLayout attribute to pad marshaled types if necessary. This allows Marshal.SizeOf to return the correct value for these types.</li>
<li>iOS/IL2CPP: Using AudioSettings.Reset() no longer crashes on IL2CPP.</li>
<li>iOS/ILCPP: Do not emit metadata for generic types at compile time. This significantly decreases the size of the final binary in most cases.</li>
<li>iOS/Metal: Fixed crash in WarmupAllShaders when called in update with AA-ed backbuffer.</li>
<li>iOS/Metal: Fixed WebCamTexture.videoVerticallyMirrored.</li>
<li>JobSystem: Fixed issue where job system would create long stalls in some cases on processors with hyper threading.</li>
<li>Mecanim: Fixed a bug where copy pasted states would share the same state machine behaviour instance</li>
<li>Mecanim: Fixed animation events not fired for non looping clip with length of 0 second.</li>
<li>Mecanim: Fixed Blend Tree parameter doesn't get updated in the graph view when changing the blend tree parameter.</li>
<li>Mecanim: Fixed cannot rename parameter in animator parameter window.</li>
<li>Mecanim: Fixed crash when a StateMachineBehaviour disable an animator component or change something that trigger a Rebind.</li>
<li>Mecanim: Fixed crash when calling AnimationClip.events from script.</li>
<li>Mecanim: Fixed lost transition when importing a project from 4.x to 5.0.</li>
<li>MonoDevelop: Fixed issue with Attach to Process dialog making MonoDevelop unresponsive on OSX.</li>
<li>MonoDevelop: Fixed issue with file tabs being unresponsive after using auto-hide of panels.</li>
<li>OpenGL ES 2.0: Fixed shadow acne on GPUs that do not support native shadow samplers.</li>
<li>OpenGL ES: Fixed crash when attempting to render a mesh with 0 vertices.</li>
<li>OpenGL: Fixed a crash in vertex stream management.</li>
<li>Physics 2D: 2D physics will now give deterministic results on the same device when entering play-mode in the editor.</li>
<li>Physics 2D: Don't suppress gravity when a Rigidbody2D.MovePosition is taking place.</li>
<li>Physics 2D: Ensure that 2D Box/Circle cast methods support shape being overlapped initially.</li>
<li>Physics 2D: Ensure that a 2D joint created from script is correctly enabled.</li>
<li>Physics 2D: Fixed regression where PlatformEffector2D 'One Way' would allow a collider to pass but then begin to collide with it.</li>
<li>Physics 2D: Setting center-of-mass on a Rigidbody2D now doesn't result in bad rotational inertia.</li>
<li>Physics: Don't allow to break rotational DoF lock by setting angularVelocity directly.</li>
<li>Physics: Fixed capsule height being incorrectly computed in sweeps and casts code.</li>
<li>Physics: Fixed cases where HingeJoint settings, like useMotor and useLimits, were not correctly applied.</li>
<li>Physics: Fixed crash on scene load when Cloth component is missing a SkinnedMeshRenderer component.</li>
<li>Physics: Fixed crash that could occur when a body had more than 64 contacts generated.</li>
<li>Physics: Fixed crash when the transform scale on a MeshCollider had an axis set to zero. Request will now be ignored.-</li>
<li>Physics: Fixed incorrect bounds of a capsule collider.</li>
<li>Physics: Fixed crash that happened when toggling "isKinematic" on a body with joint that had joint projection disabled and the body had also been connected to the same group of joints already.</li>
<li>Physics: Fixed crash when a collider has generated too many contacts.</li>
<li>Physics: Fixed WheelCollider applying inertia tensor rotation the wrong way.</li>
<li>Physics: Protect SetSteerAngle from setting wheel angles that are bad for PhysX.</li>
<li>Physics: Raised the max colliders per scene limit on mobile platforms, from 32K.</li>
<li>Physics: Report error when trying to create a non-convex MeshCollider with Trigger enabled.</li>
<li>Plugins: Fixed invalid plugin collisions, for ex., in cases where plugin is unsupported by OS, but was still being used.</li>
<li>Samsung TV: Fixed crash on close issue.</li>
<li>SamsungTV: Fixed bug where cursor would stop moving when timeScale was set to 0 on 2013 TVs.</li>
<li>SamsungTV: Fixed problem where native plugins would not be found on retail 2015 TVs.</li>
<li>SamsungTV: Fixed race condition crash that originated from within mono when NumberFormatter was being called from a non-main managed thread.</li>
<li>Scene/Game View: Fix the issue about cannot select objects after importing the legacy packages.</li>
<li>Scripting: Allow a component which derives from a type in UnityEngine.UI and is built in a custom assembly to be used in the project.</li>
<li>Scripting: Fixed EditorGUI.FloatField and EditorGUILayout.FloatField unable to return negative and positive infinity</li>
<li>Scripting: GizmoType works as expected</li>
<li>Scripting: Re-added a stub for Resources.LoadAssetAtPath which auto-upgrades to AssetDatabase.LoadAssetAtPath</li>
<li>Shaders: Don't crash in shader warmup on "-nographics" device.</li>
<li>Shaders: Fixed some loops being miscompiled for DX9.</li>
<li>Shaders: Fixed some sampler precision issues in glsl-optimizer; was resulting in missing cast on Metal when sampling depth texture with explicit LOD.</li>
<li>Substance: Entering play mode should no longer cause a rebuild of ProceduralMaterials.</li>
<li>Substance: Fixed 'path != ""' assert when live-previewing a Substance from the Asset Store.</li>
<li>Substance: Fixed console spam related to the absence of '_MainTex' shader property.</li>
<li>Substance: Fixed crash when assigning a shader that does not cause outputs to be generated (e.g. Unlit/Color) to a ProceduralMaterial.</li>
<li>Substance: Fixed hang in ProceduralMaterial::Clean().</li>
<li>Substance: Global Illumination flags are now correctly handled by ProceduralMaterials.</li>
<li>Substance: It is no longer possible to dynamically create a ProceduralMaterial using 'new'.</li>
<li>UI: PointerEventData.worldPosition and .worldNormal are now set correctly for right-mouse-button and middle-mouse-button events.</li>
<li>VR: Fixed GearVR startup crash on Galaxy S6 devices by enabling pbuffer Context support.</li>
<li>VR: MSAA autoresolve fixed for GLES 3.0 devices.</li>
<li>WebGL: Fixed stripping (previously failing to register WebCamTexture class in runtime).</li>
<li>WebGL:/iOS: Fix crash in UnusedBytecodeStripper on BoxCollider2D/CircleCollider2D center member access.</li>
<li>WebPlayer: Fixed WWW form posting.</li>
<li>WebPlayer: Workarounds for new Chrome, where NPAPI is disabled by default.</li>
<li>Windows Phone 8: Uppercase first letter in InputField.</li>
<li>Windows Phone 8: Windows Phone 8 specific plugins (compiled against Windows Phone 8 .NET) which don't have a placeholder won't be passed to the Mono compiler, like it was in 4.6.</li>
<li>Windows Standalone: Allow to close the main window even with the touch support enabled.</li>
<li>Windows Standalone: Connecting USB devices should no longer throw spurious  warnings.</li>
<li>Windows Store Apps: .NET Core plugins without placeholders, won't be passed to Mono compiler, like it was to 4.6.</li>
<li>Windows Store Apps: Build&amp;Run disabled when using Unity CSharp projects.</li>
<li>Windows Store Apps: Fixed the issue, build from editor when C-projects are enabled.</li>
<li>Windows Store Apps: Fixed issues with plugins in Universal apps, removed SDK property UniversalSDK81 from plugin inspector, as it didn't make sense. Also having Windows 8.1 and  Windows Phone 8.1 specific plugins won't longer cause building to Universal apps to fail.</li>
<li>Windows Store Apps: mouse presence now is detected by mouse activity, which is much more reliable.</li>
<li>Windows Store Apps/Windows Phone 8.1: Unity will correctly hide password when using GUI*.PasswordField on touch based devices.</li>
<li>Windows Store Apps/Windows Phone: Fixed AssemblyConverter failing due to types from other module.</li>
<li>Windows Store Apps/Windows Phone: Fixed NullReferenceException in SerializationWeaver.</li>
<li>Windows Store Apps/Windows Phone: System.IO.File.Exists should work even if you specify forward slashes which is invalid in WinRT platforms, Unity will convert them to backwards slashes.</li>
<li>Windows Store/Phone: Unity will always give postprocessed assemblies a new random MVID.</li>
<li>Windows Store/Windows Phone 8.1: Fixed an issue which caused types unavailable in .NET for Windows Store but available in Unity's replacement library not to be resolved if they were in a plugin.</li>
<li>WindowsPhone8: Fixed AssemblyConverter error, where sometimes it would fail to find references.</li>
<li>WWW: WWW.Dispose sometimes hung Unity on a very slow connection.</li>
<li>XboxOne: Application.OpenURL is now implemented on Xbox One. Calling it will open the Internet Explorer App.</li>
<li>XboxOne: Bad image from Kinect fixed, YUY2 support.</li>
<li>XboxOne: Bloom artefact when using MSAA is now fixed.</li>
<li>XboxOne: Crash when using Clear Depth Only, support for capturing RTs of different bit depths.</li>
<li>XboxOne: DOF image effect on fade sprites fixed.</li>
<li>XboxOne: Enabled support for deferred rendering and HDR.</li>
<li>XboxOne: Fixed a crash that can happen when shutting down the audio device.</li>
<li>XboxOne: Fixed a rare startup crash that usually manifested as a crash in the audio driver, sometimes showing up as a stack buffer overrun exception.</li>
<li>XboxOne: Fixed compute shader UAV buffer read/write and memory access.</li>
<li>XboxOne: Fixed port assignments so Unity Profiler and Debugger work more consistently</li>
<li>XboxOne: Lightmaps for scene 0 are now included in the package manifest.</li>
<li>XboxOne: Made Mono's exception handler treat unexpected exceptions (ex: not a breakpoint) better. This should remove some instances where a crash dump was not created.</li>
<li>XboxOne: Now matches PC (deferred rendering with HDR related).</li>
<li>XboxOne: The /updcompat option for makepkg.exe now has a space before it so it's read by the tool correctly.</li>
<li>XboxOne: The file path used for makepkg.exe is now quoted when a custom manifest file is used.</li>
</ul>
