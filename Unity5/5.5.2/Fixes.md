# Unity 5.5.2
https://unity3d.com/unity/whats-new/unity-5.5.2

## Fixes

<ul>
<li>Android: Fixed a crash when doing simultaneous SceneManager.LoadSceneAsync and Resources.Load. - (782183)</li>
<li>Android: Fixed a player crash when using Location services. - (866556)</li>
<li>Android: Fixed an incorrect behaviour with Application.persistentDataPath. - (854214)</li>
<li>Android: Fixed readback from float RenderTexture into half -float Texture.</li>
<li>Android: Fixed splash screen flicker and artifacts. - (863528)</li>
<li>Android: Gradle export -; Ffixed colliding package name for unity-android-resources. - (854535)</li>
<li>Android: Gradle export should now work with SDK version &gt; 6.0. - (856650)</li>
<li>Android: Identified unaccounted spikes in profiler. - (836697)</li>
<li>Android: Improved asynchronous loading time when showing splash screen.</li>
<li>Android: Play audio from background applications at the original volume when it is not muted.</li>
<li>Android/IL2CPP: Prevent a crash which can occur with the use of OnAudioFilterRead callbacks on kKrait CPUs. - (852307)</li>
<li>Android/MetroWindowsStore: Fixed the issues preventing the Application.Unload API from functioning correctly.</li>
<li>Animation: Fixed a bug that was preventing AnimationEvents that were added to legacy AnimationClips during runtime from being called. - (877033)</li>
<li>Animation: Fixed a crash when setting Animator.updateMode when no AnimatorController is set. - (869582)</li>
<li>Animation: Fixed crash in animation window when starting playback on invalid optimized game object - (865057)</li>
<li>Animation: Fixed edit key overriding key frames in curve editor. - (860366)</li>
<li>Animation: Fixed vertical and horizontal flips using Box Tool with tangents set to Infinity. - (849656)</li>
<li>Asset and Scene ManagementAsset Importing: Fixed a crash while importing an FBX where individual component X/Y/Z curves had different frame ranges. - (845966)</li>
<li>Asset Bundles: Fixed a crash when loading a scene with occlusion culling from an asset bundle in editor play mode. - (846853)</li>
<li>Asset Bundles: Fixed loading asset by file name and extension to work identical to loading by file name. - (845762, 841092)</li>
<li>Asset Bundles: Fixwsed intermittent freeze that could occur when calling AssetBundle.LoadAssetAsync multiple times in a single frame. - (862004)</li>
<li>Asset Importing: Significant performance improvements to DXT1, DXT5, BC4 and BC5 texture compressor, resulting in faster asset imports.</li>
<li>Audio: Fixed a WACK certification failure in UWP player builds using the Microsoft HRTF audio spatializer. - (865507)</li>
<li>Cache Server: Can now handle paths with spaces on Mac when calling RunOSX.command with the --path argument. Paths with spaces must be within quotes. - (874677)</li>
<li>Cache Server: Displays a warning in the Cache Server Editor Preferences when the Local Cache Server location cannot be reached (e.g. on a disconnected disk). - (858923)</li>
<li>Cache Server: Fixed an issue when building,; an unreachable cache server was reported as a warning not an error and did not cause the build to fail. - (840009)</li>
<li>Cache Server: Fixed the custom port missing for the remote option. - (871730)</li>
<li>Cloudbuild Analytics: Fix for iOS and Android crash when all services are OFF.</li>
<li>Deployment Management: Corrected the behaviour on Windows where using -logfile on batch mode with an emptry string would cause output to go to stdout, consistent with all other platforms. - (857206)</li>
<li>DX11: Fixed D3D11 Device creation failures on Windows Vista and Windows 7 systems without DX11.1 runtimeupdate. - (877407, 867093, 877210)</li>
<li>Editor: Disallow setting DontSave on a tTransform unless it is already set on the GameObject. - (857507)</li>
<li>Editor: Fixed a crash for D3D platforms if shader compilation did not return any compiled shader data ie, a shader contained #error pre-processor directive. - (824020)</li>
<li>Editor: Fixed a crash whilst reloading scene(s) after using version control merge and resolve operations. - (876733)</li>
<li>Editor: Fixed a rare issue where building the player and saving the project later could cause the Editor to lock up. - (857117)</li>
<li>Editor: Fixed an issue whereby new installed Unity would report timeout error in commandline activation. - (790345)</li>
<li>Editor: Fixed light probe rendering in LookDev HDRIs. Previously it could go wrong depending on the lighting panel parameters set for the project.</li>
<li>Global Illumination: Fixed a rare issue where spawning external processes (such as GI Baking) could fail or cause a deadlock. - (799748)</li>
<li>Graphics: Don't render the screencamera depth texture space depth buffer if nothing requires it i.e. screenspace shadows are disabled. - (836737)</li>
<li>Graphics: DrawProcedural draws geometry only in the left eye when Single Pass VR is enabled - (859819)</li>
<li>Graphics: Fixed a crash in some circumstances if object disabled renderer when culling updated the visibility. - (849079)</li>
<li>Graphics: Fixed a crash that occurred when loading models from AssetBundles with Tangents set to Calculate Legacy. - (861445)</li>
<li>Graphics: Fixed crash in occlusion culling when loading multiple scenes. - (862005)</li>
<li>Graphics: Fixed large objects lit by a directional light self shadowing in editor when player was set to aAndroid. - (866230)</li>
<li>Graphics: Line Renderer; fixed gaps when values are repeated - (861293)</li>
<li>Graphics: LineRenderer; fixed issue where setting endColor failed if using different number of color/alpha keys - (864043)</li>
<li>HoloLens: Fixed a crash that occurs on device when downloading files with WWW. - (860775)</li>
<li>HoloLens: Fixed an issue with InputField automatically getting activated for text entry as soon as you gaze at it. - (850327, 851586)</li>
<li>HoloLens: Prevented a potential memory stomps in very rare repro cases when resuming from suspend.</li>
<li>IL2CPP: Allow the build to succeed when the .NET 4 TargetFrameworkAttribute attribute is used in an assembly. - (867606)</li>
<li>IL2CPP: Allow the Unity Ads engine integration to work properly on iOS builds that are archived and uploaded to TestFlight. - (874227)</li>
<li>IL2CPP: Correct an error in UnusedBytecodeStripper2 related to UnityEngine.RenderTexture that can occur during some project builds. - (863806)</li>
<li>IL2CPP: Corrected the behavior of Assembly.GetExecutingAssembly on platforms that did not support stack walking properly. - (871948)</li>
<li>IL2CPP: Fixed a compile error related to missing header when compiling code using SizeOf IL opcode. - (874838)</li>
<li>IL2CPP: Fixed a rare crash in IL2CPP on some Visual Studio installation setups with message "Unhandled Exception: System.InvalidOperationException: Builder is unable to build using selected toolchain (MsvcDesktopToolChain) or architecture (Unity.IL2CPP.Building.x64Architecture)!"</li>
<li>IL2CPP: Fixed an issue with race condition of the monitor implementation of IL2CPP that could cause a crash. - (870810)</li>
<li>IL2CPP: Fixed System.IO.WindowsRuntimeStreamExtensions class not being present in System.Runtime.WindowsRuntime.dll.</li>
<li>IL2CPP: Prevented an error during code generation when IL code had a try/finally as the last block in a method. - (872641)</li>
<li>IL2CPP: Prevented an ExecutionEngineException from being thrown at run time when a virtual generic method was called via a delegate. - (869676)</li>
<li>iOS: Added missing icon slots for Spotlight and Settings. (815299)</li>
<li>iOS: Don't indicate that microphone and camera is used when it isn't. - (869099)</li>
<li>iOS: Don't strip alpha channel out of launch screens textures. - (847494)</li>
<li>iOS: Fixed a bug that would prevent the text field input caret from updating when the virtual left and right arrow keys were pressed. - (850430)</li>
<li>iOS: Fixed a crash with advertisingIdentifier in iOS Simulator. - (869305)</li>
<li>iOS: Fixed an exception when disposed ODR object was collected by GC. - (850619)</li>
<li>iOS: Fixed an issue where the ReplayKit API might be reported as available on unsupported devices - (828288)</li>
<li>iOS: Fixed Application.isShowingSplashScreen to return the correct state and deprecated it in favour of SplashScreen.isFinished. - (824499)</li>
<li>iOS: Fixed inability to change Launch Screen Mode in Player Settings. - (869283)</li>
<li>iOS: Fixed orientation requests from the app getting out of sync with iOS orientation. - (796649)</li>
<li>iOS: Fixed UnityRepaint crash due to internal inconsistency error. - (862754)</li>
<li>iOS: Hide the status bar while playing movies with CancelOnInput or Hidden modes. - (871989)</li>
<li>iOS: Internal profiler reports non-sensical CPU time values in pretty much all cases.. - (843172)</li>
<li>iOS: UnityEngine.iOS.Device.SetNoBackupFlag can now be called from background threads. - (851113)</li>
<li>iOS: Warn when CameraDepthTexture uses wrong Metal sampler type. - (786455)</li>
<li>iOS: Warn when SV_POSITION is used as input in vertex shader. - (809737)</li>
<li>Kernel: Fixed an issue when undoing the reverting of a prefab which added components with dependencies (such as ConfigurableJoint depending on RigidBody existing). - (870498)</li>
<li>Kernel: JsonJSON serialisation now supports correct parsing of NaN and +/-Inf. - (829753)</li>
<li>Lighting: Fixed baked light map visualisation shading mode in the Editor.</li>
<li>LineRenderer: fixed gaps when values are repeated - (861293)</li>
<li>LineRenderer: Fixed issue where setting endColor failed if using different number of color/alpha keys - (864043)</li>
<li>macOS: Added a fix to hide the 'Picture in Picture' button in the movie player when played using Handheld.PlayFullScreenMovie. - (739557)</li>
<li>Metal: Fixed lack of support for the Hidden/FastBloom shader on Metal devices. - (876956)</li>
<li>Mono: Correct an invalid C# compiler error with generic types in compiler generated code (like lambdas and enumerators). The error from the C# compiler often includes this text: "There is no boxing or type parameter conversion from..." - (847798)</li>
<li>Networking: Fixed issue where unspawn handler was not properly invoked during object cleanup (like in NetworkManager.StopClient()) - (836770)</li>
<li>OS X: Added a fix to hide the 'Picture in Picture' button in the movie player when played using Handheld.PlayFullScreenMovie. - (739557)</li>
<li>Particles: Fixed "TLS ALLOCATOR ALLOC_TEMP_THREAD" error messages - (864122)</li>
<li>Particles: Fixed an issue whereby animation curves causing assert errors when using scripted emission. - (865738)</li>
<li>Particles: Fixed an issue whereby lights were not cleared when Stop() and Clear() were called. - (869710)</li>
<li>Particles: Fixed an issue whereby particle trails were reusing old position data when emitted by script. - (858243)</li>
<li>Particles: Fixed an issue with allowing circular references in sub emitters. - (853996, 845817)</li>
<li>Particles: Fixed crash in LightsModule when destroying systems - (862777)</li>
<li>Particles: Fixed crash in ParticleSystem.Emit() - (862897)</li>
<li>Particles: Fixed issue where distance-based emission was not working - (856842)</li>
<li>Particles: Fixed issue where particle bounding boxes could become corrupted, resulting in "Invalid AABB" messages - (862352)</li>
<li>Particles: Fixed issue where sub-emitters were causing memory leaks - (861347, 863060 )</li>
<li>Particles: Fixed issue where switching Render Mode could cause rendering artifacts - (862976)</li>
<li>Particles: Fixed rare crash when using the Trail Renderer and Multithreaded Rendering is enabled. - (868648)</li>
<li>Particles: Fixed rotation bug with mesh particles - (862921)</li>
<li>Particles: Fixed the issue of color not being updated correctly when material properties were changed when using shape module. - (778213)</li>
<li>Particles: Fixed the issue of distance emission not working when scale was not 1 and using hierarchy scaling mode. - (844815)</li>
<li>Particles: Fixed TrailModule crash when enabling trails and using ParticleSystem.SetParticles - (864208)</li>
<li>Particles: Particles Anim Shader now works when using mesh render mode. - (869386)</li>
<li>Particles: Stretched billboards could apply scale twice if using Speed Scale - (861409)</li>
<li>Particles: Texture Animation could skip frames and display invalid data - (859436v</li>
<li>Physics 2D: Ensure all 2D physics profile items provide an object reference.</li>
<li>Physics 2D: Ensure that a PhysicsMaterial2D can be reassigned to a Collider2D.</li>
<li>Physics 2D: Fixed an issue of rendering CapsuleCollider2D with very small sizes. - (863939)</li>
<li>Physics 2D: Optimize the CapsuleCollider2D component intersection tests for speed and accuracy.</li>
<li>Physics 2D: When turning on Rigidbody2D.simulated, the body position/rotation should be synchronized to the current Transform. - (871727)</li>
<li>Physics: Fixed a crash when applying prefab changes in the editor when a component contains a Rigidbody2D. - (878576)</li>
<li>Playables: Fixed blending of AnimatorControllerPlayable not working properly. - (873587)</li>
<li>Prefabs: Fixed Editor crash when trying to connect a prefab to an instance marked with DontSave. - (866855)</li>
<li>Purchasing: Fixed a bug where a duplicate transaction could fail without calling the failure callback.</li>
<li>SceneManagement: Fixed unloading Scene using Scene as parameter. - (860750, 871607)</li>
<li>Scripting: Added the following non-allocating accessors to Mesh. These accessors write into a user-specified List. The accessors are GetBindposes, GetBoneWeights, GetColors, GetIndices, GetNormals, GetTangents, GetTriangles, and GetVertices.</li>
<li>Scripting: Allow serialization of classes extending Dictionary. - (699250)</li>
<li>Scripting: Fixed a deadlock when debugging in MonoDevelop. - (819887)</li>
<li>Scripting: Fixed a rare failure when building players. - (852993)</li>
<li>Scripting: Fixed an issue with StopCoroutine not stopping IEnumerator and CustomYieldInstruction based coroutines. - (852360)</li>
<li>Scripting: Fixed RequireComponent not working with nested namespaces. - (856277)</li>
<li>Shaders: Fixed shader compilation error when compiling certain surface shaders using WorldNormalVector from INTERNAL_DATA e.g. shadow pass variations. - (856507)</li>
<li>Splash Screen: Fixed an issue where the splash could be truncated by a first scene taking a long time to load - (810571)</li>
<li>Tizen: Change the minimum API level to Tizen 2.4 in PlayerSettings. - (872286)</li>
<li>Tizen: Fix a NULLnull dereferencinge while exiting the game. - (869995)</li>
<li>Tizen: Improve error when failing to discover a deployment target. - (834785)</li>
<li>Tizen: Improvements to emulator deployment.</li>
<li>Tizen: SystemInfo.processorFrequency now returns proper values.</li>
<li>TrailRenderer: Fixed visual artifacts when manually enabled during Play mode - (869964)</li>
<li>UI: Fixed miscoloured mesh when this was created with CanvasRenderer.SetMesh, passing an array of Color objects to Mesh.colors. - (857087)</li>
<li>UnityWebRequest: fix proxy support, so that debuggers like Fiddler work. - (861828)</li>
<li>UnityWebRequest: Fixed an issue with redirect in editor when not in play mode. - (878300)</li>
<li>Virtual Reality: Fixed inconsistency in game view between Singlepass Stereo and Multi Pass when using Split Stereo Diplay. - (814290)</li>
<li>Virtual Reality: Fixed incorrect culling in Split Stereo Display. - (830612)</li>
<li>Virtual Reality: Fixed incorrect eye view in Split Stereo Display. - (832185)</li>
<li>Virtual Reality: Fixed incorrect viewport bounds in Singlepass Stereo. - (832283)</li>
<li>Windows Store: Fixed build &amp; run failing on windows phone 10 with IL2CPP scripting backend. - (862914)</li>
<li>Windows Store: Fixed building Windows Store player against Windows 10 "Creators Update" SDK. - (876078)</li>
<li>Windows Store: Fixed IL2CPP not finding tools from Windows SDK directory in some installation setups.</li>
<li>Windows Store: Fixed player pref corruption on power loss. - (855595)</li>
<li>Windows Store: Fixed the folder Structure missing from Assembly-CSharp.csproj. - (858579)</li>
<li>Windows: When standalone player is embedded into other window, Alt+Enter shortcut for full screen is disabled.</li>
</ul>
