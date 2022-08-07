# Unity 5.4.5
https://unity3d.com/unity/whats-new/unity-5.4.5

## Fixes

<ul>
<li>Analytics: Fix adds Internet permission on Android when Analytics service is used.   (861178)</li>
<li>Analytics: Fixed an issue where transaction events could send the wrong value for "amount" on the WebGL platform.    </li>
<li>Android: Enabled TLSv1.1 and TLSv1.2 on JellyBean and KitKat devices.    (776003)</li>
<li>Android: Enhanced big.LITTLE core detection-specifically fixed core detection on Parker. </li>
<li>Android: Fixed a crash when doing simultaneous SceneManager.LoadSceneAsync and Resources.Load.   (782183)</li>
<li>Android: Fixed an issue where ApplicationModeVR would threw an error in the log file.    </li>
<li>Android: Fixed incorrect behaviour with Application.persistentDataPath.  (854214)</li>
<li>Android: Fixed startup crash on Adreno when protected graphics memory was used.  (832025)</li>
<li>Android: Fixed UI flickering issue that was affecting specific Vivante devices.  (712890)</li>
<li>Android: Identified unaccounted spikes in profiler.      (836697)</li>
<li>Android: OBB - Fixed loading performance regression and split APK not running without OBB.   (842286)</li>
<li>Android: Play audio from background applications at the original volume when it is not muted.     </li>
<li>Android: Post process is now executed before app is pushed to device.    (803872)</li>
<li>Android: Updated JNIBridge to fix Bundle class regression in API 21. (856259)</li>
<li>Android/IL2CPP: Prevent a crash which could occur with the use of OnAudioFilterRead callbacks on krait CPUs. (852307)</li>
<li>Animation: Fix for a crash using Resources.UnloadUnusedAssets with Animators caused by orphaned references.  (855546)</li>
<li>Animation: Re-enabled StateMachine multithreaded evaluation.  </li>
<li>Cache Server: Can now handle paths with spaces on Mac when calling RunOSX.command with the -path argument. Paths with spaces must be quoted. (874678)</li>
<li>Cache Server: Fix for 'last resource used' behaviour; a file that it requested from the cache server will have its LRU state refreshed and its lifetime extended.        (853251)</li>
<li>Cache Server: When building, an unreachable cache server was reported as a warning not an error and did not cause the build to fail. (840009)</li>
<li>Deployment Management: Corrected a behaviour on Windows where using -logfile on batch mode with an emptry string would cause the output to go to stdout, consistent with all other platforms.    (857203)</li>
<li>DX11: Fixed D3D11 Device creation failures on Windows Vista and Windows 7 systems without DX11.1 runtime.    (877407, 867093, 877210) </li>
<li>Editor: Fixed a crash for D3D platforms if shader compilation did not return any compiled shader data ie, a shader contained #error pre-processor directive. (824020)</li>
<li>Editor: Fixed a rare issue where building the player and saving the project after could cause the Editor to lock up. (857117)</li>
<li>Editor: Fixed an issue that personal user was able to skip a mandatory survey.   (834243)</li>
<li>Editor: Fixed Assertion failed error in console: '(sharedData.instructionCount == 0) || sharedData.combinedBounds.IsValid()'.    (878784)</li>
<li>Editor: Fixed Gizmos only being displayed for the first camera in the Game View. (780168)</li>
<li>Editor: PVRTexTool updated to 4.17 (SDK version 16.2@4273839).   </li>
<li>Editor: Removed old editor assemblies when reimporting assets.    </li>
<li>Global Illumination: Fixed a rare issue where spawning external processes (such as GI Baking) could fail or cause a deadlock.   (799748)</li>
<li>Graphics: Don't render the screen space depth buffer if nothing required it. i.e screenspace shadows were disabled.      (836737)</li>
<li>Graphics: Fixed a crash in some circumstances if object disables renderer when culling updates visibility.   (849079)</li>
<li>Graphics: Fixed a crash that occurred when loading models from AssetBundles with Tangents set to Calculate Legacy.   (861446)</li>
<li>Graphics: Fixed an issue where grab pass could cause lighting to break on translucent objects in a scene.    (844799)</li>
<li>Graphics: Fixed console error generated when using WWW.movie to create a movie texture.  -(825464)</li>
<li>Graphics: Fixed errors spamming the console when performing GPU profiling on a DX11 Standalone build.    (767034)</li>
<li>Graphics: Fixed the GPU Profiler to work in the MacOS Editor using the GLcore graphics API. Can only profile a single game window whilst it is in play mode. (823371)</li>
<li>Graphics: Stopped rendering projectors twice if there was any transparent object visible to the camera.  (732380)</li>
<li>IL2CPP: Fixed a compile error related to missing header when compiling code using SizeOf IL opcode.  (874838)</li>
<li>IL2CPP: Fixed an issue with race condition of the monitor implementation of IL2CPP that could cause a crash. (870810)</li>
<li>iOS: Add missing iPod touch 6th gen enumeration. (834663)</li>
<li>iOS: Added Taiwanese language support.   (853532)</li>
<li>iOS: Document settings are shared across iOS and tvOS.   (786207)</li>
<li>iOS: Don't strip alpha channel out of launch screens.    (847494)</li>
<li>iOS: Fixed UnityRepaint crash due to internal inconsistency error    .   (862754)</li>
<li>iOS: Fixed 2nd stage splash on iPhones with landscapeRight orientation.  (810286)</li>
<li>iOS: Fixed a full screen video player crash on simulator.    (814079)</li>
<li>IOS: Fixed an issue where the ReplayKit API might be reported as available on unsupported devices.   (828288)</li>
<li>iOS: Removed extra offset in constraint in default launchscreens.    (831195)</li>
<li>Kernel: JSON serialisation now supports correct parsing of NaN and +/- Inf.  (829753)</li>
<li>Metal: Fixed a memory leak when loading scene.   (850332)</li>
<li>Multiplayer: Fixed hostmigration sync issue. (807091)</li>
<li>Multiplayer: Made sure isLocalPlayer worked as expected on OnDestroy.    (826931, 853316) </li>
<li>Networking: Skip proxy check when using the "file://" protocol.  </li>
<li>Purchasing: Fixed a bug where a duplicate transaction could fail without calling the failure callback.   </li>
<li>ReplayKit : Fixed a crash when creating objects from broadcasting start callback.    (848718)</li>
<li>ReplayKit : Fixed ReplayKit.StartBroadcasting not pausing the app.   (833159)</li>
<li>Scripting: Fix issue with StopCoroutine not stopping IEnumerator and CustomYieldInstruction based coroutines.    (852360)</li>
<li>Scripting: Fixed a rare failure when building players.   (852993)</li>
<li>Scripting: Fixed deadlock when debugging in MonoDevelop. (819887)</li>
<li>Shaders: Bugfixes in shader translation from HLSL to GLSL : 
<ul>
<li>Fixed a crash on HLSLcc partial precision parsing. </li>
<li>Fixed bugs in swapc, SM5 variant of shift ops and GLSL extension handling.  </li>
</ul></li>
<li>Shadows: Fixed a memory leak and assert when shadows were cast from lights with specific properties and in a specific scene setup.   (764734)</li>
<li>UI: Fixed miscoloured mesh when this was created with CanvasRenderer.SetMesh, passing an array of Color objects to Mesh.colors.  (857087)</li>
<li>UnityWebRequest: Fixed a high CPU usage issue when a request was continuing execution after exiting playmode.    (855646)</li>
<li>UnityWebRequest: Fixed the proxy support so that debugging tools like Fiddler work.  (861828)</li>
<li>VCS: Don't attempt to connect to a Perforce server if any of the following parameters are unset: Server, User or Client. (861468)</li>
<li>VCS: Fixed an issue which was trying to add files from ProjectSettings folder to Version Control even if they were already under Version Control.     </li>
<li>VR: Fixed usage of VRSettings.renderViewportScale in Camera's OnPreCull so that it was not a frame latent on all supporting SDKs. Fixed issues with Valve's Renderer adaptive quality feature.   </li>
<li>WebGL: Fixed Content-Length header field for local web server response that caused some audio files to have a duration of infinity or zero. This required an asset store plugin for webgl audio streaming and was not reproducible using other web servers.   </li>
<li>Windows Store: UnityWebRequest now works in master builds.   (862888)</li>
<li>Windows: Fixed -hideWindow briefly showing the window before hiding it on standalone players.     </li>
</ul>

#### Revision: 68943b6c8c42
