# Unity 2017.2.2
https://unity3d.com/unity/whats-new/unity-2017.2.2

## Fixes

<ul>
<li>AI: Fixed NavMeshAgents swapping to different NavMeshes when they are disabled and re-enabled right on an edge. (970718)</li>
<li>Android: Fixed a rare static splash screen crash. (971571)</li>
<li>Android: Fixed decimal point button in decimal keyboard for older Samsungs. (973815)</li>
<li>Android: Fixed an issue where the full-screen movie player didn't autorotate. (962450)</li>
<li>Android: Fixed a bug causing the loading of native audio plugins to fail on Android. (992023)</li>
<li>Animation: Fixed an issue that was causing the Editor to throw an exception when selecting animator transitions in an undocked preview window. (967382)</li>
<li>Animation: Improved fix for creating an ongoing transition. (941945)</li>
<li>Animation: Fixed a crash caused by invoking QueryComponentByType() when code stripping is enabled. (989240)</li>
<li>Apple TV: Removed 2x App store icon slices that cause App Store validation to fail. (972927)</li>
<li>Asset Bundles: Fixed crash caused by a Sprite Atlas trying to load in sprites that were packaged in an Asset Bundle that hasn't been loaded. (985914)</li>
<li>Asset import: Fixed bug with import of FBX with custom framerate generating animationClips with an incorrect framerate. (973917)</li>
<li>Asset Import: Fixed crash when setting the property ModelImporter.clipAnimations, when the clip avatar mask is set to "Create From This Model". (960595)</li>
<li>Assets: Fixed Assetdatabase.Refresh taking longer than necessary. (969205)</li>
<li>Audio: Fixed a crash in AudioLowPassFilter on Nintendo Switch. (975345)</li>
<li>Audio: Fixed a bug where AudioManager::Update was generating a small amount of garbage memory, if a spatializer was selected. (991111)</li>
<li>Build Pipeline: Improved player and asset bundle build performance for large builds. (959444)</li>
<li>Cache Server: Fixed an issue which caused the Unity client to hang indefinitely. (953940)</li>
<li>Editor: Fixed being able to start multiple PlayMode and EditMode test runs at the same time from the test runner ui. (969114 (945000)</li>
<li>Editor: Fixed bootstrap scene sometiems being left behind if running PlayMode and EditMode tests from script. (969114)</li>
<li>Editor: Fixed lightingdata.asset files getting re-opened in text mode in certain situations. (975920)</li>
<li>Editor: Added an optional Async Query Mode for Perforce VCS integration (see Editor Settings) to stop the editor freezing when the Perforce - connection has high latency. (922829)</li>
<li>Facebook: Fixed unhandled BadImageFormatException for deleted SDK .dll. (975427 (956872)</li>
<li>GI: Fixed editor crash when when deleting a prefab which is used as a tree in Terrain inspector. (946550)</li>
<li>Graphics: Fixed asserts and potential memory leaks when Skinned Mesh Renderers with the "Update When Offscreen" property enabled are not visible. (961692, 964998)</li>
<li>Graphics: Fixed issue where DrawMeshInstanced calls will render with inverse normals if the previous draw call used negative scaling. (956919 (891894)</li>
<li>Graphics: Fixed changing the projectors render queue in script not having an effect. (841236)</li>
<li>Graphics: Fixed a crash in the job system related to light culling. (930408)</li>
<li>Graphics: Fixed crash in Canvas node extraction, usually triggering a crash on save. (973686)</li>
<li>Graphics: Fixed crash during a visibility callback when a GameObject which was not visible is set inactive followed by setting a visible GameObject inactive. (968591)</li>
<li>Graphics: Fixed crash in CommandBuffer.DrawMeshInstanced when called with a null property block. (951975)</li>
<li>Graphics: Fix for Crash in Projector::PrepareRenderNode after selecting GameObject in the Hierarchy. (976076)</li>
<li>IL2CPP: Fixed a crash on iOS which can occur when a device is awakened during a blocking socket call with a SIGPIPE signal. (957651)</li>
<li>IL2CPP: Work around for a C++ compiler bug in the Android r13b NDK that could cause the NullCheck method to be incorrectly removed from the - resulting binary. (962771)</li>
<li>IL2CPP: Fixed potential crash when default parameter values are used. (973052)</li>
<li>IL2CPP: Improved the performance of code conversion when many nested generic types are used. (975496)</li>
<li>IL2CPP: Fixed a problem with the decimal to double conversion implementation with the new scripting runtime. (959791)</li>
<li>IL2CPP: Fixed crash in Unity Linker (System.InvalidProgramException: Failed to resolve [UnityEngine]System.Resources.NeutralResourcesLanguageAttribute) when using a managed DLL that has a non-existing attribute on it. (969958)</li>
<li>IL2CPP: Implemented sending of email via SmtpClient with .NET 4.6. (947208)</li>
<li>IL2CPP: Fixed issue where android builds would crash on launch with the 4.5 runtime when the byte code stripping option was selected. (922979)</li>
<li>iOS: Fix iOS 11 crash when application is launched from URL and airplay screen mirroring is enabled. (980362)</li>
<li>iOS: Metal: Fixed MSAA corner case causing warning messages and validation error. (983853)</li>
<li>iOS: Fixed trampoline calling UI methods ([UIApplication delegate]) from a background thread. (956318) (57809)</li>
<li>iOS: Fixed locked orientation app getting rotations from portrait to landscape when sharing to another app on iOS 8 &amp; 9. (913856) (57503)</li>
<li>iOS: Fixed problem with missing keyboard Done/Cancel buttons for iPhone X. (979005) (58588)</li>
<li>iOS: Fixed an issue where fullscreen movies could no longer be dismissed with a tap on iOS 11. (940608)</li>
<li>iOS: Allow landscape startup on iOS11. (980303)</li>
<li>iOS: Fixed videos started with Handheld.PlayFullScreenMovie not resuming after returning to the app in some circumstances. (954593)</li>
<li>Launcher: Fix display of Unity Teams "Seat Required" message when project is both in the cloud and on disk. (963246)</li>
<li>License: Fixed issue when cached refresh token &amp; access token expired, command line activation will failed. (940084)</li>
<li>License: Removed misleading "This should not be called in batch mode" message when returning license. (877423 (972989)</li>
<li>Metal: Fixed an edge case crash when using grab-pass on metal. (973813)</li>
<li>Multiplayer: Skipped soft socket error, to prevent host to be closed. (None)</li>
<li>Package Manager: Fixed editor not starting because of custom proxy configuration on host machine. (None)</li>
<li>Particles: Fixed Stop Action when it should be used for off-screen Particle Systems. (974867)</li>
<li>Particles: Fixed Rate over Distance emission issues. (960527) (964537)</li>
<li>Particles: Fixed crash when using [RuntimeInitializeOnLoadMethod] attribute. (975289)</li>
<li>Particles: Fixed crash when enabling some modules from script (e.g. SizeOverLifetime). (977710)</li>
<li>Particles: Fixed emission properties being incorrectly upgraded from previous Unity versions. (966306)</li>
<li>Particles: Fixed Duration property when used on Sub-Emitters. (968096)</li>
<li>Physics: Fixed PhysX crash when calling Physics.OverlapBoxNonAlloc on Android devices. (878407)</li>
<li>Physics: Fixed potential crash in Rigidbody::GetVelocity() when opening certain scenes. (955697)</li>
<li>Physics: Fixed crashes when loading new scene and activating cloth gameobject in coroutine. (951789)</li>
<li>Physics: Fixed issue where Physics Debugger's layer mask does not filter GameObject correctly. (948201)</li>
<li>Scripting: Fixed an issue causing GC allocation for UnityEvent handler without parameters in some cases. (978101)</li>
<li>Scripting: Fixed random crash due to memory corruption on domain reload. (967206)</li>
<li>Scripting: Fixed URI processing on OSX. (907918)</li>
<li>Scripting: Fixed crash when using GitHub for Unity. (930358)</li>
<li>Scripting: Fixed deadlocks and pauses when using System.Threading.Monitor. (827984)</li>
<li>Scripting: Improved TypeLoadException messages. (957072)</li>
<li>Scripting: Fixed DllImport when library name is specified with path. (952631)</li>
<li>Scripting: Fixed TypeLoadException for types and array initializers larger than 1 MB. (962711)</li>
<li>Scripting: Fixed InternalsVisibleToAttribute. (945353)</li>
<li>Scripting Upgrade: Fixed Android crash when script debugger is enabled. (973794)</li>
<li>Scripting Upgrade: Corrected a C# compiler bug which could result in "the type cannot be used as type parameter `T' in the generic type or method" errors. (991464)</li>
<li>Scripting Upgrade: Fixed EntryPointNotFoundException when calling HTTPClient.GetAsync on Android. (935292)</li>
<li>Scripting Upgrade: Fixed Socket.Send failing silently on Windows. (984723)</li>
<li>Scripting Upgrade: Fixed Android crash when NullReferenceException is raised. (954427)</li>
<li>Scripting Upgrade: Fixed crash when using 'fixed' statement on a string. (960555)</li>
<li>Scripting Upgrade: Fixed crash when using named pipes. (942966)</li>
<li>Scripting Upgrade: Fixed crash on exit when script debugger is enabled. (974228)</li>
<li>Scripts Only Build: Fixed issue where a user could select a different destination than the last non-scripts only build. (978680)</li>
<li>Services: Performance Reporting: Report device model field for Managed Exceptions. (980816)</li>
<li>Shaders: Fixed some edge cases where shaders would be compiled using cached include file data which was out of date. (None)</li>
<li>Terrain: Removed Editor error about non read/write textures. (964302)</li>
<li>Terrain: Fixed default smoothness for terrain without a texture. (962764)</li>
<li>Timeline: Fixed console errors when using Default Playables package. (967026)</li>
<li>Timeline: Fixed preview mode for properties animated by Control Tracks. (965091)</li>
<li>Timeline: Fixed an issue where custom tracks could be lost if they contained compile errors. (979700)</li>
<li>Timeline: Fixed ArgumentOutOfRangeException that shows in console when shift-selecting a clip that was undo-move. (986872)</li>
<li>UGUI: Fixed a driven RectTransform causing a scene to be constantly flagged as dirty. (991019)</li>
<li>UGUI: Fixed undoing the activation of a UI layout component not undoing the side effects to the children RectTransforms. (991023)</li>
<li>Universal Windows Platform: Fixed debugging scripts on .NET scripting backend. (949806) (934783)</li>
<li>Universal Windows Platform: Fixed NavMeshObstacles being ignored on 64-bit master builds. (955086)</li>
<li>Universal Windows Platform: Fixed NotSupportedException being thrown on UWP builds with .NET scripting backend enabled when using Timeline. (966790)</li>
<li>Video: Fixed crash on attempting to upgrade project. (979757)</li>
<li>Video: Fixed not being able to Enable Transcoding on Video File. (958543)</li>
<li>Video: Fixed video not being played when trying to play it in the Video Clip Importer preview. (978449)</li>
<li>Video: Fixed videos being transcoded when switching platform even when they are cached in Cache Server. (963979 (976826)</li>
<li>Video: Meta files are updated for videos that were transcoded during platform switch resulting in litter for VCS. (962118)</li>
<li>Web: Fixed Content-Disposition for file sections not being standard-compliant in UnityWebRequest. (980327)</li>
<li>Web: Fixed crash when checking AssetBundle download progress, that gets aborted. (968877)</li>
<li>Web: Fixed DownloadHandlerFile not truncating file on overwrite. (None)</li>
<li>Web: UnityWebRequest: improve performance for DownloadHandlerScript. (965165)</li>
<li>Web: Fixed hang when busy waiting on a redirecting request. (963947)</li>
<li>WebGL: Added indexedDB caching mechanism for XMLHttpRequest in WebGL. (937594)</li>
<li>WebGL: Fixed UnityWebRequest with relative URL when running with custom port. (961465)</li>
<li>WebGL: Fixed crash for relative URL in UnityWebRequest when exceptions are disabled. (965094)</li>
<li>Windows: Fixed possible crash in UnityWebRequest on Windows platforms when using UnityWebRequest with custom download handler script. (None)</li>
<li>Windows: Fixed executable not having Unity version info. (964052)</li>
<li>Windows: Fixed game window not getting minimized when using exclusive fullscreen mode on Windows key press. (953086)</li>
<li>Windows Standalone: Fixed a regression where a fullscreen application would be restored to the native resolution of the attached display after losing focus. The expected outcome was that it should be restored to the original resolution that it was - launched on. (972924 (950056)</li>
<li>XR: Fixed Windows Mixed Reality controllers not being properly detected in Editor Play mode. (948931)</li>
<li>XR: Fixed early out of Virtual Reality SDK list when SDKs that are unsupported in play mode try to initialize. Also Improved log messages around the Virtual Reality SDK list in Play Mode. (971293)</li>
<li>XR: Fixed Oculus not reporting values for XRStats properties. (883630)</li>
<li>XR: Fixed a regression that would cause BEV cameras not to track properly. (None)</li>
<li>XR: Fixed shaders targeting XR platforms being included in builds where XR support is disabled. (971944)</li>
<li>XR: Fixed ScreenCapture.CaptureScreenshot() captures stereo instancing screenshots incorrectly. (970906)</li>
<li>XR: Fixed issue with grabpass when used single-pass stereo rendering. (963320)</li>
<li>XR: Fixed tracking loss never recovers in Windows Mixed Reality. (969944)</li>
<li>XR: Fixed a random crash in Windows Mixed Reality. (None)</li>
<li>XR: Fixed inconsistency between generic code path and WSA-namespace-specific path for whether select is pressed. (970844)</li>
<li>XR: Fixed UnityEngine.Experimental.XR.Boundary.TryGetGeometry throwing internal exception always failing. (963315)</li>
<li>XR: Removed application orientation settings disable when Virtual Reality Supported is enabled and update info message related to the settings. (986941)</li>
<li>XR: Android - Fixed errors when building for Daydream and Cardboard with Proguard enabled. (949379)</li>
</ul>

#### Revision: 1f4e0f9b6a50
