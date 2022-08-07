# Unity 5.4.2
https://unity3d.com/unity/whats-new/unity-5.4.2

## Fixes

<ul>
<li>AI: Fix for regression where a pushed passive NavMeshAgent would sometimes move to its origin after navmesh carving. (830443) </li>
<li>Analytics: DeviceInfo now matches hwstats data. (none) </li>
<li>Android: Buildpipe: Fixed streaming assets folders starting with _ ignored. (819800) </li>
<li>Android: IL2CPP - Fixed missing config files for il2cpp build. (821806) </li>
<li>Android: Sensors - Fixed location isEnabledByUser returning true when the service is disabled. (821688) </li>
<li>Android: WebRequest - Fixed a crash when using GetAudioClip() with file protocol. (818992) </li>
<li>Android: WWW - Fixed an application freeze on WWW.Dispose when the connection was canceled. (777663) </li>
<li>Animation: Fixed blending between two additive clip when some properties are animated in one clip but not in the other one. (828199) </li>
<li>Animation: Fixed OverrideController memory leak. (none) </li>
<li>Animation: The Animation preview will correctly display a preview animation when a model is dragged to the preview area. (819905) </li>
<li>Api updater: Fixed a crash when updating Boo/UnityScript scritps with empty "else" blocks. (769445) </li>
<li>Api-updater: Fixed crashes / issues with paths containing either "exe" or "dll" in any part other than the file extension. (809268) </li>
<li>AssetBundle: Fixed the issue that error sometimes happens when LoadAssetAsync and UnloadUnusedAsset is called before prefab is instantiated. (822393) </li>
<li>AssetBundles: Fixed high CPU usage while downloading asset bundles. (755398) </li>
<li>Audio: Fixed memory leak when quickly loading and unloading lots of audio assets. (832271) </li>
<li>Canvas: Fixed a regression introduced in 5.4.0p4 where non-native fullscreen player appeared darker when Canvas was present, in Linear color space. (834100, 833996) </li>
<li>D3D11: Added check and return when trying to ReadPixels from outside the RenderTarget's bounds, fixes crash on nVidia hardware. (819793) </li>
<li>D3D12: Fixed a crash caused by using DXGI_PRESENT_ALLOW_TEARING with exclusive fullscreen swapchains. (814533) </li>
<li>D3D12: Fixed a crash when creating RenderTargetView for 3D RenderTextures. (none) </li>
<li>D3D12: Fixed missing splash screen. (796521) </li>
<li>Editor Test Runner: Added firstpass assemblies to be picked up by the Editor Test Runner. (819175) </li>
<li>Editor: Fixed a crash when registering undo for null object. (779052) </li>
<li>Editor: Fixed an extra erroneous characters in path passed to PostProcessBuild callbacks. (821728) </li>
<li>Editor: Fixed an issue with [FormerlySerializedAs] not working with scripts assigned to prefabs. (732717) </li>
<li>Editor: Fixed path error when building into the same folder again. (818346) </li>
<li>Editor: Fixed services tab not getting focused when a service refresh occurs. (704234, 807773, 829992, 822715) </li>
<li>Editor: JavascriptPackageManager now supports UNC path on Windows. (764857) </li>
<li>FrameDebugger: Fixed crash on Android. (824107) </li>
<li>GI: Fix for out-of-memory failure in Visibility Upsampling when baking lightmaps for a large scene. (819841) </li>
<li>GI: Fixed a crash that can happen when building lightmaps when a procedural texture was used for transparency. (818910) </li>
<li>Graphics: DisableBatching tag now works correctly in depth pass and legacy deferred base/final passes. (819602) </li>
<li>Graphics: Fix for incorrect calculation of projection matrix on some platforms. (826406) </li>
<li>Graphics: Fixed a crash in the Editor when material and shader properties weren't updated correctly. (812576) </li>
<li>Graphics: Fixed a crash that would in some cases happen after Material.CopyPropertiesFromMaterial. (821208) </li>
<li>Graphics: Fixed a rare deadlock that can happen when graphics jobs are enabled. (827364) </li>
<li>Graphics: Fixed a threading issue causing game view to corrupt or go blank randomly in OSX editor. (820693) </li>
<li>Graphics: Fixed an Assert in AssignProjectorQueuesJob about calling GetRenderJobThreadCount() when not on the main thread. Triggers when running gfx jobs in scenes with projectors. (none) </li>
<li>Graphics: Fixed an unnecessary assert in static batching loop. (818781) </li>
<li>Graphics: Fixed Display renderingWidth and renderingHeight incorrectly returning system resolution values. (none) </li>
<li>Graphics: Fixed large delta values in the the motion vector matrix when a camera is enabled after being disabled. (none) </li>
<li>Graphics: Fixed lightmap texture corruption when changing quality levels. (785547) </li>
<li>Graphics: Fixed the issue of projectors rendering twice if transparent objects are in the scene. (814282) </li>
<li>Graphics: More prevention against invalid data causing crashes in CommandBuffer.DrawRenderer. (813052) </li>
<li>Graphics: Now use Renderer::GetTransform() when calculating local AABB so that static batched renderers return the reference transform correctly. (813671) </li>
<li>GUI: Fixed an issue where GUI::DrawTexture appeared darker than GUI::DrawTextureWithTexCoords when in Linear color space. (828145) </li>
<li>GUI: Fixed the regressions introduced in 5.4.1f1 and 5.4.1p1 where GUI.DrawTexture &amp; GUI.DrawTextureWithTexCoords appeared lighter in Linear color space. (832155) </li>
<li>IL2CPP: Allow now Monitor.TryEnter to correctly obtain a previously taken lock that has been released, which did not work in some cases. (815783) </li>
<li>IL2CPP: Correct the stack state handling during code conversion for some box opcodes. (826624) </li>
<li>IL2CPP: Removed an unnecessary assert when GC.Collect(1) is called. The call will still have no impact though. (834376) </li>
<li>Input: Mouse position is now updated but not clamped when outside of game window. (827851) </li>
<li>iOS: Added missing iOSTargetOSVersion enum entries. (826595) </li>
<li>iOS: Corrected the default setting for bitcode on the XCTest target to fix a linker error. (824979) </li>
<li>iOS: Fixed a crash when killing the app while a WWW Request was in flight. (811959, 815928) </li>
<li>IOS: Fixed an iOS 10 warning for improper use of runloop. (none) </li>
<li>iOS: Fixed an issue where Touch.deltaTime was incorrectly returning zero when device had been on for approximately 30 days or more. (809752) </li>
<li>iOS: Fixed App Store submissions with Xcode 8 when phone camera is not being used by game. (none) </li>
<li>iOS: Fixed iPhone6+ reported resolution in first Start/Awake calls. (803581) </li>
<li>iOS: Fixed the appearance of apps freezing when locking/unlocking the device. (820863) </li>
<li>iOS: Fixed the GI crash on 32bit devices. (827107) </li>
<li>iOS: Fixed the iOS crash when screen resolution is changed from script. (827431) </li>
<li>IOS: Fixed the Remote notification detection code. (830528) </li>
<li>Linux: Fixed the nographics crash in non-headless player. (none) </li>
<li>Linux: Improved the robustness of opengl legacy fallback. (none) </li>
<li>Metal: Fixed an issue whereby view was not scaling properly when using Screen.SetResolution in fullscreen mode. (818563) </li>
<li>Metal: Fixed grab pass combined with image effects appears darker. (830273) </li>
<li>Metal: Improved MSAA support with Image Effects, where previously the framebuffer load operation could have shown black screen instead. (none) </li>
<li>Metal: Various rendering correctness fixes. (none) </li>
<li>Mono: Use an IPv4 address (if one exists) before an IPv6 address for .NET remoting connections. (826526) </li>
<li>Mono/IL2CPP: Corrected a rare deadlock in the C# lock implementation. (827984) </li>
<li>Networking: Fixed an issue with SyncList hook having old value when it's invoked. (774970) </li>
<li>Networking: Fixed issue with infinitely growing profiler stats when more than one client is connected. (765235) </li>
<li>Networking: Fixed the SerializeProperty issues with NetworkManager inspector (channels and prefabs). (798973, 764771) </li>
<li>Networking: Made sure NetworkConnection is not null before usage. (770215) </li>
<li>Networking: Made sure we reset the NetworkIdentity on destruction. (784474) </li>
<li>Networking: Removed extra call to OnServerConnect. (784913) </li>
<li>Networking: Resolved issue with crash on exit with standalone player. (776536) </li>
<li>OpenVR: Entered playmode with unsupported gfx api = crash. (799533) </li>
<li>OS X: Fixed memory leak in joystick input handling code. (797793) </li>
<li>Particles: Fixed Out-of-memory crash when using Sub-Emtiters and long playback/preview times. (819599) </li>
<li>Particles: Particles: Size over lifetime label in the curve editor would incorrectly display "Z" label instead of "Size" when not using separate axis mode. (822051) </li>
<li>Particles: ParticleSystem.Emit would activate the emission module settings in a particle system. (819331) </li>
<li>Particles: Start frame in Texture Animation Module was allowed to be 1 frame longer than max frames. (786561) </li>
<li>SceneView: Fixed an issue where additive materials were not showing in Wireframe mode. (813117) </li>
<li>SceneView: Fixed an issue where the alpha color value had no affect to Wireframe. For the same reason Wireframes also appeared thicker. (810908, 823582) </li>
<li>SceneView: Fixed an issue where Wireframe was not showing when using stencil buffer in shaders. (795953) </li>
<li>Scripting: Coroutines now breaks out if yielding on the same coroutine twice. (813808) </li>
<li>Scripting: Detect and unload broken assemblies when processing InitializeOnLoad. (808748) </li>
<li>Scripting: Fixed a crash caused by SetActive being invoked from OnDestroy. (807000) </li>
<li>Shaders: Fixed frac(constant) sometimes being mis-compiled. (825235) </li>
<li>Shaders: Fixed shader compiler bug which could have caused errors in GLSL shaders that might crash the GPU on OSX. (none) </li>
<li>Shaders: Fixed UNITY_APPLY_FOG not working as expected if an expression was passed as fog coordinate. (822553) </li>
<li>SpritePacker: Fixed an issue where TightRotateEnabledSpritePackerPolicy flipped sprites in playmode. (773660) </li>
<li>Substance: Fixed a crash when switching build platform. (820301) </li>
<li>Substance: Fixed an asset import crash. (822217) </li>
<li>Textures: Correctly unregister external native textures. (786163) </li>
<li>Tizen: Resolved an error that didn't call OnApplicationQuit() when TaskManager killed the app. (none) </li>
<li>tvOS: Fixed the issue of UnityEngine.Apple.TV.Remote API not working in editor. (825406) </li>
<li>tvOS: Fixed the issues when menu button was clicked while playing videos. (814084) </li>
<li>tvOS: Fixed the UI to correctly activate tvOS keyboard. (747529) </li>
<li>UAP: Fixed an incorrect language being returned when system language was Spanish(Argentina). (820162) </li>
<li>UAP: Fixed the issue of incorrect resolution being reported when the composition scale changed and the game window was minimized. (832104) </li>
<li>UI: Fixed a memory leak caused by IntermediateRenderers not being cleaned up. (819470) </li>
<li>UI: Fixed a random crash in SyncElement caused by unknown parent canvas. (none) </li>
<li>UI: Fixed an issue with animating canvas properties not applying. (825435) </li>
<li>UI: Fixed an issue with Canvas sorting order being incorrect under certain cases. (821727) </li>
<li>UI: Fixed Canvas related crash when some elements are being deleted. (818122) </li>
<li>UI: Fixed the Canvas related crash when some elements are being deleted. (818294) </li>
<li>UI: Multiple display support is fixed and has been re-enabled. (741751) </li>
<li>UNET: OnDisconnectError "Server client disconnect error" is generated on timeout. (790431) </li>
<li>VCS: Marked some VCS settings as private. (642194) </li>
<li>VR: Fixed issue with WaitForEndOfFrame when VR is active. (none) </li>
<li>VR: Recreate when Oculus service requests restart. (none) </li>
<li>VR: Removed audio output warning when Unity Audio is Disabled. (826132) </li>
<li>WebGL: Fixed asset bundles memory usage at loading time, preventing some content to run on 32-bit browsers. (812567, 829765) </li>
<li>WebGL: Fixed compressed build files (.*gz) creation if they already exist. (818044) </li>
<li>WebGL: Fixed GUID code to return correct value instead of&nbsp;00000000000000000000000000000000. (none) </li>
<li>WebRequest: More correctly follow the HTTP Specification for sending POST data during a Redirect. (814388) </li>
<li>Windows Store: Correctly reference SDK specific plugins in Universal 8.1 projects. (824400, 794675, 829404) </li>
<li>Windows Store: Fixed a WWW request formatting when headers contained 'content-type' in lower case instead of 'Content-Type'. (819349) </li>
<li>Windows Store: Fixed errors from reference rewriter when buidling script with nested generic types as fields. (827446) </li>
<li>Windows Store: Fixed invalid visual studio project generation on IL2CPP scripting backend when project name contains dots. (829141) </li>
<li>Windows Store: Fixed Unity PDB files not getting included into built .appxsym package. (831144) </li>
<li>Windows Store: Properly copy pdb files when .NET Native is enabled, breakpoints set in C# files in Assembly-CSharp* projects should work again. (822625) </li>
<li>Windows Store: SystemInfo.deviceType will return Console when application is ran on Xbox One, and Handheld when ran on IoT devices like Raspberry Pi. (827089) </li>
<li>Windows Store: UnityEvent.Remove listener will work correctly when .Net Native is enabled. (827748) </li>
<li>Windows: Fixed Unity crashing when initializing UnityEngine.Windows.Speech.KeywordRecognizer with an array that contains null string as one of its items (833091) </li>
<li>Windows: System resolution or orientation changes are now detected and responded to accordingly. (825230) </li>
<li>WindowsStandalone: Application launched with high integrity level will no longer act as low integrity application. (818601) </li>
<li>WWW/UnityWebRequest: Fixed the issue of handling multiple headers with the same name in server responses. (791722) </li>
</ul>

#### This also includes various bugs fixed in 5.3.x patch releases.

#### Revision: b7e030c65c9b
