# Unity 5.3.1
https://unity3d.com/unity/whats-new/unity-5.3.1

## Fixes


#### Relevant fixes from Unity 5.2.4 are also included into 5.3.1.
<ul>
<li>Android: AndroidJNI - fixed crash when no params passed to AndroidJavaProxy with  AndroidJNIHelper.debug set to true. (740472, 740023)</li>
<li>Android: Buildpipe - don't run dex if exporting the project. (746248)</li>
<li>Android: Buildpipe - don't unpack AARs if exporting the project. (747567)</li>
<li>Android: Fixed querying for custom permissions on Android Marshmallow. (750227)</li>
<li>Android: Fixed VRAM calculation on devices with 4GB or more RAM.</li>
<li>Android: Fixed 5.3 performance regression in dynamic batching. (749690)</li>
<li>Android: Immersive - fixed black bar in the bottom on Android M and L. (689552, 738518)</li>
<li>Android: Workaround for OpenGL ES 3.0 shader compiler issues on Adreno 3xx. (735299)</li>
<li>Animation: Fixed 1st frame of Animation displaying default state of the object. (751714)</li>
<li>Animation: Fixed AnimationClip dependency collection not working for AnimatorControllers. (717286)</li>
<li>API Updater: Fixed crashing when checking for obsolete API in assemblies referencing unity extensions. (734221)</li>
<li>Audio: Fixes issue when modifying exposed parameters in AudioMixer loaded from asset bundle. (734258)</li>
<li>Core: Fixed multithreading related memory allocations; removes a number of JobAlloc.Overflow instances in profiler.</li>
<li>Editor: Fix for prefab modifications making the scene dirty immediately after loading. (709639)</li>
<li>Editor: Fixed restoring Hierarchy View after exiting the Avatar Editor or running Editor tests. (745634)</li>
<li>Editor: Force reimport all models to ensure that generated lightmap UVs are consistent across platforms. (739787, 745698)</li>
<li>Editor: Stopped exponential growth of the undo stack when undo-redoing selection changes.</li>
<li>Editor Webview UI: Right click in text input would show a blank menu on windows 8 and 10. (718718)</li>
<li>GI: Fixed a problem where Final Gather was always being recomputed.</li>
<li>GI: Remove CPU cost of Enligten Post Update when there is no realtime GI.</li>
<li>Graphics: Enabled rendering to cube map faces with multisample AA. (730570, 648624)</li>
<li>Graphics: Fixed incorrect stripping of vertex streams in certain situations when a mesh has a mixture on lightmapped and non-lightmapped shaders; e.g. the vertex colour stream was previously being incorrectly stripped. (683178, 725562)</li>
<li>HomeWindow: Fixed Home Window closing after sign-in if cache is empty. (746120)</li>
<li>HomeWindow: Fixed black screen on 32-bit Windows. (745427, 753800)</li>
<li>IL2CPP: Allow the [Preserve] attribute to correctly prevent stripping of a method in a nested type. (738356)</li>
<li>IL2CPP: Avoid compiler error due to duplicate FieldInfo definition.</li>
<li>IL2CPP: Avoid duplicate data files in iOS packages. (746329)</li>
<li>IL2CPP: Avoid stack overflow crash due to large allocation with alloca. (739685)</li>
<li>IL2CPP: Correctly initialize the metadata for default parameter values that are obtained via reflection. (745793, 737565)</li>
<li>IL2CPP: Fixed race condition during cleanup of threadpool threads. (738232)</li>
<li>IL2CPP: Fixed an issue which caused "callback cannot take parameters" error message if there was a DLL in the project that inherited from animation state machine classes, but project did not use animation. (743502, 734472)</li>
<li>IL2CPP: Prevent generated C++ code from including a header file that was not generated when the type which could have been generated in that header is used only in an attribute applied to an assembly. (737996)</li>
<li>IL2CPP: Properly handle additional, subtraction, and multiplication when the type of the left argument is smaller than the type of the right argument and the result will not fit in the type of the left argument and the result is stored across an IL block. (745691)</li>
<li>IL2CPP: Provide proper managed stack traces when the C++ compiler inlines method calls. (739956)</li>
<li>IL2CPP: Set default stack size on iOS to 1MB to match Mono behavior. (733799)</li>
<li>iOS: Disable the toggle for 'Show Unity Splash Screen' if user does not have a Pro license. (730103)</li>
<li>iOS: Don't crash when social platform API is used incorrectly. (683359)</li>
<li>iOS: Don't incorrectly cache social platform local user auth status. (683359)</li>
<li>iOS: Ensure that game center authentication callback is called once. (643154)</li>
<li>iOS: Fixed achievement completion banner display. (738722)</li>
<li>iOS: Fixed crash on iOS 6.0 devices. (747022)</li>
<li>iOS: Fixed hidden portion of multiline text area so users can view the last line of text. (745175)</li>
<li>iOS: Fixed ODR progress reporting. (736477)</li>
<li>iOS: Fixed WWW connection redirect functionality. (723960)</li>
<li>iOS: Don't override iPod music when corresponding player setting is not set. (734640)</li>
<li>iOS: Send focus events when entering and exiting game center dialogs. (738720)</li>
<li>iOS: Update remote notification callback API. (692374)</li>
<li>iOS: Added workaround for iOS launch screen asset catalog bug. (736683, 739007)</li>
<li>JsonUtility: Fixed memory leak when FromJson() throws exceptions. (752057)</li>
<li>Linux: Fixed crash on shutdown.</li>
<li>Linux: Work around crash when FMOD can't detect available audio drivers.</li>
<li>Mecanim: Fixed an error in the Animator inspector when selecting multiple files. (743247)</li>
<li>Mecanim: Fixed Animator.CrossFade failing when already crossfading. (741799)</li>
<li>Mecanim: Fixed crash when deleting game object with rendering effect during play mode. (742537)</li>
<li>Mecanim: Fixed Euler angles not being displayed as animated in the transform inspector. (744156)</li>
<li>MonoDevelop: Display error dialog if GTK# is not installed on Windows. (735412)</li>
<li>MonoDevelop: Fixed issue with MonoDevelop not starting on OSX if installed in /Applications and user is not admin. (739514)</li>
<li>Networking: Added check for too-large buffer. (726466)</li>
<li>Networking: Added error message when [SyncEvent] used with UnityEvent. (737287)</li>
<li>Networking: Better scene slot handling in NetworkLobbyManager. (733731)</li>
<li>Networking: Fixed: Can't set registered spawn prefab to null. (730504)</li>
<li>Networking: Exception in editor for NetworkTransform in preview window. (741974)</li>
<li>Networking: Fixed LargePacket warning during RelayServer games. (746992)</li>
<li>Networking: Fixed NetworkHash128.ToString() error when string has embedded zeroes. (738032)</li>
<li>Networking: Fixed NetworkManager singleton management regression issue. (742033)</li>
<li>Networking: Fixed numPlayers on NetworkManager. (746022)</li>
<li>Networking: Fixed slow compilation with many ClientRpc functions. (738517)</li>
<li>Networking: Fixed SyncLists becoming invalid after host migration. (746006)</li>
<li>Networking: Fixed SyncLists losing registered callbacks when scene changed. (736052)</li>
<li>Networking: Fixed UNetWeaver build error when a SyncListStruct contains a field and array of the same type.</li>
<li>Networking: Fixed UNetWeaver error with 15 SyncVars in a NetworkBehaviour. (749253)</li>
<li>Networking: Fixed warning message from NetworkAnimator in editor. (740186)</li>
<li>Networking: Handle script reloads while network is active. This shuts down the network properly, and if there is a NetworkManager, switches to the offline scene.</li>
<li>Networking: Fixed host migration error when no players. (736702)</li>
<li>Networking: Fixed log spam when profiler window open after deleting network host. (695592)</li>
<li>Networking: Fixed network operations stats not resetting when 'clear' is pressed. (738999)</li>
<li>Networking: NetworkManager HUD updated to not allow MM use. (740634)</li>
<li>Networking: Scene slots of NetworkLobbyManager broken after project upgrade. (742039)</li>
<li>Networking: Unable to restart host after reloading scripts while in play mode and running as host. (738167)</li>
<li>Networking: Wrong item index for SyncList add operation. (736703)</li>
<li>OpenGL Core: Work around desynchronization of default vertex array with active GL context.</li>
<li>OpenGL ES: Fixed occasional omitting of precision specification in shaders. (748944)</li>
<li>Particles: Fixed crashes when deleting meshes used by a particle system. (745282, 745390)</li>
<li>Particles: Fixed graphical corruption when rendering particle meshes with different vertex sizes.</li>
<li>Particles: Fixed vertex normals, 5.2 regression. (732483)</li>
<li>Particles: Fixed scale when in Local billboarding mode. (728663)</li>
<li>Particles: Improved script API example documentation.</li>
<li>Particles: Improved particle multi-threading performance.</li>
<li>Physics: Ensure that Joint2D CollideConnected is correctly upgraded to EnableCollision for all joints. (749797)</li>
<li>Physics: Fixed an issue where a static trigger collider would not report a contact when moved. (752059)          </li>
<li>Physics: Fixed an issue where collision/trigger callbacks would not report if constantly modifying a Collider2D (that caused it to be regenerated).   (752764)</li>
<li>Plugins: Fixed invalid assert when there's a plugin containing 'UnityEngine.dll' inside its name, e.g. Something.UnityEngine.dll. (752340)</li>
<li>Samsung TV: Center cursor before locking and then ignore mouse motion event while cursor is locked.</li>
<li>SceneManagement: Fixed crash caused by loading a scene additively in the same frame as unloading the active scene, if there are no other scenes loaded. (747223)</li>
<li>SceneManagement: Fixed unloading a scene using the full path.</li>
<li>Scripting: Log error instead of crashing when Start() like methods are defined as generic. (733194)</li>
<li>Scripting: OnTransformChildrenChanged message is now correctly sent to both old parent and new parent. (688317, 713431)</li>
<li>Shadows: Correctly handle custom off-center projection matrices for directional lights. (686520)</li>
<li>Substance: Changing the random seed of a DoNothing material that has not been generated yet does not cause its textures to be generated anymore.</li>
<li>Substance: Cloned ProceduralTextures now inherit the color space of the source texture. (738483)</li>
<li>Substance: Exported preset strings now have a valid package URL, label, and description, and can now be loaded in Substance Player.</li>
<li>Substance: isProcessing now works correctly for BakeAndDiscard materials and for cloned materials. (740158, 732705)</li>
<li>Substance: The Substance part of BakeAndDiscard materials could sometimes remain in the standalone builds. (732705)</li>
<li>TreeEditor: Fixed crash on adding branch nodes under GLCore devices. (741520)</li>
<li>UI: Fixed color conversion in BatchGenerator when using Linear color space. (730457)</li>
<li>UI: Fixed issue when instantiating and re-parenting canvases and prefabs. (736161, 742081)</li>
<li>UI: Fixed dropdown menu not being displayed when Time.timeScale is set to 0.</li>
<li>UI: Fixed incorrect culling when a MaskableGraphic had a negative scale value inside of a mask.</li>
<li>UI: Multiple display support disabled on all platforms except WiiU and 3DS. This will be re-enabled once the non-native resolution bug is fixed. (741751)</li>
<li>UI: Unity GPU profiler now correctly accounts for UI draw calls.</li>
<li>VR: Fixed a crash when trying to toggle showDeviceView to false before first Update. (749329)</li>
<li>VR: Fixed an issue where Oculus was starting while building the standalone player while Virtual Reality Supported is true. (748988)</li>
<li>VR: Fixed an issue where showDeviceView was not caching between runs in the Editor. Now forces to true on play. (750510)</li>
<li>Windows Phone 8.0: Fixed regression with System.IO classes. (745932)</li>
<li>Windows Standalone: Fixed Unity Crash on Application.Quit with MultiTouch.</li>
<li>Windows Store Apps: Added bluetooth capability. (744371)</li>
<li>Windows Store Apps: Fixed AppCallbacks::UnitySetInput throw ClassNotRegisterred exception on UWP. (736419) Windows Store Apps: Fixed FileStream occasionally failing when writing large data. (745355)
Windows Store Apps: Fixed same files referenced by Assembly-CSharp and Assembly-CSharp-firstpass projects. (746296)</li>
<li>Windows Store Apps: Fixed touch screen keyboard not opening after dismiss via X button. (750396)</li>
<li>Windows Store Apps: Fixed Unity splash screen not showing. (745415)</li>
<li>Windows Store Apps: Modify template sources while still in StagingArea, to prevent issues if Visual Studio is open. (741518)</li>
<li>Windows Store Apps: SpriteState is now correctly serialized. (715720)</li>
<li>Windows Store Apps: Use current orientations on startup, only populate manifest from Player Settings. (740535)</li>
<li>Windows Store Apps: When building to SDK 8.1, you no longer need Visual Studio 2013, it's enough to have Visual Studio 2015 with Windows SDK 8.1. (741455)</li>
<li>Windows Store Apps: On screen keyboard reliability fixes on Windows 10. (744936)</li>
<li>Windows Store: Fixed HID controllers when targeting Windows 10 SDK.</li>
<li>Windows Store: Fixed Unity producing invalid Visual Studio project files if Windows 10 SDK 10.0.10586.0 is installed (749600)</li>
<li>Windows Store: Fixed WinMD references in generated C# projects when building a project with "C# projects" checkbox checked.</li>
<li>Windows Store: Soft shadows now work correctly on ARM devices with D3D feature level &gt;= 10.0.</li>
<li>WindowsInstaller: Detect Unity version from the current install path, instead of using the Windows Registry.</li>
<li>WindowsInstaller: The /D command line option in the Documentation and TargetSupport Installers is correctly handled now. (752093)</li>
<li>WinRT/IL2CPP: Remove compiler warnings in generated C++ code. (742021)</li>
</ul>

#### Revision: cc9cbbcc37b4
