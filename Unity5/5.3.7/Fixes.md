# Unity 5.3.7
https://unity3d.com/unity/whats-new/unity-5.3.7

## Fixes

<ul>
<li>2D: Fixed an assert  message "importer.GetNPOTScale() == TextureImporter::kNPOTKeep" showing when creating sprites in Advanced mode. Creating sprites now ignores TextureImporter's non power of two settings if the texture is already a power of two. (800914, 802831)</li>
<li>AI: Fix for regression where a pushed passive NavMeshAgent would sometimes move to its origin after navmesh carving. (830443)</li>
<li>AI: Fixed an issue where NavMeshAgent remaining distance property would be wrong right after setting the agent destination to the same polygon. (822015)</li>
<li>AI: Fixed an issue where NavMeshAgent would sometimes teleport right after NavMeshObstacle carving. (822362)</li>
<li>Android: Audio - Fixed glitches on GearVR audio when Best Latency is selected. (811963)</li>
<li>Android: Fix for crash on returning from Handheld.PlayFullScreenMovie. (811880)</li>
<li>Android: Fixed a crash on Android when using the Frame Debugger. (824107)</li>
<li>Android: Fixed an issue where projects without audio could stop external audio sources. (807983)</li>
<li>Android: Fixed build time regression when using the rResources folder. (808752)</li>
<li>Android: Fixed device screen clear bug on Vivante GC1000 GPUs andwhen using OpenGL ES 2.0GLES2 API. (754003)</li>
<li>Animation: Deleting an Override controller that was previously set as the runtime controller no longer resets the animator state machine memory.</li>
<li>Animation: Fixed a crash when changing AnimatorOverrideController during interrupted transition. (823410)</li>
<li>Animation: Fixed an issue where having animations with a mixed number of bones in a controller, and having Write Defaults to false would throw errors. (769505)</li>
<li>Animation: Fixed thea crash when triggering a newly created animation clip at runtime. (824596)</li>
<li>Animation: Fixed the OverrideController memory leak.</li>
<li>API Updater: Fixed a crash when updating Boo/UnityScript scritpts with empty "else" blocks. (769445)</li>
<li>API Updater: Fixed crashes / issues with paths containing either "exe" or "dll" in any part other than the file extension. (809268)</li>
<li>Asset Management: Assets added using AssetDatabase.AddObjectToAsset will no longer change their name when the project is saved. (811596)</li>
<li>AssetBundles: Fixed thean issue that error sometimes happens when LoadAssetAsync and UnloadUnusedAsset is called before prefab is instantiated. (822393)</li>
<li>AssetBundles: Fixed an issue where calling Resources.UnloadUnusedAssets while loading an AssetBundle with AssetBundleRequest.LoadAssetAsync caused an error &amp;and stopped the asset from being loaded properly (803481, 807275)</li>
<li>AssetBundles: Fixed AssetBundle.LoadFromFile usage with Application.streamingAssetsPath on Android. (763293)</li>
<li>Audio: Fixed a crash when/after building for standalone with empty project with several audio clips. (812396)</li>
<li>Audio: Fixed a memory leak when quickly loading and unloading lots of audio assets. (832271)</li>
<li>Cache Server: Fixed an issue where cache server could crash due to unhandled EEXIST error when creating directory. (821680)</li>
<li>Camera: Fixed an issue where rectviewport rect was ignored when using SetTargetBuffers. (814152)</li>
<li>Core: Added support for loading serialized files stored with 5.5.0a4.</li>
<li>Core: Assets added using AssetDatabase.AddObjectToAsset will no longer change their name when the project is saved. (811596)</li>
<li>D3D11: Take into account ColorSpace (linear/gamma) when capturing screenshots. (832996)</li>
<li>Deployment: Enabling free license users to access experimental builds. (778656)</li>
<li>DX11: Fixed bad GPU skinning interaction with tessellation shaders, crashesd some drivers.  (813805)</li>
<li>DX11: Take color space (linear/gamma) into account when capturing screenshots. (832996)</li>
<li>Editor Tests: Added first pass assemblies to be picked up by the editor tests runner. (819175)</li>
<li>Editor: Exceptions from PostProcessBuild callbacks now properly introduce errors to the build. (793567)</li>
<li>Editor: Fixed a crash when registering undo for a null object. (779052)</li>
<li>Editor: Fixed an issue where 'sub-assets' could appear in the wrong order in the Editor or change order when saving. (775290)</li>
<li>Editor: Fixed an issue where a project with no Library folder could raise a warning stating that the project was made before 5.0. (796046, 778891)</li>
<li>Editor: Fixed an issue where ColorPicker color was darker than the actual color picked in Linear color space. (708582)</li>
<li>Editor: Fixed Cef focus issue caused by multiple webview refreshes. (816585)</li>
<li>Editor: Fixed crash when trying to connect a GameObject to a prefab with no root GameObject set. (808080)</li>
<li>Editor: Fixed issue where objects in Inspector Preview appeared darker in Linear color space.</li>
<li>Editor: Fixed sa crash caused by leading and/or trailing slashes in MenuItem names. (771779)</li>
<li>Editor: Fixed the recursive directory copy problemsituation. (748499)</li>
<li>Editor: Fixed editor not starting properly Javascript PackageManager now supports with UNC paths on Windows. (764857)</li>
<li>Fixed HoloLens touch injection for flat apps.</li>
<li>Editor: Fixed syntax error in user-agent header string generated by API requests within Unity web views.</li>
<li>GI: Fixed a crash in Reflection Probe component when multiple scenes are used. (811241)</li>
<li>GI: Fixed an issue whereby the bake got stuck if the object was positioned far from the origin. (775153)</li>
<li>Graphics: Don't re-upload textures to the graphics device when a quality change is requested and the pixel data is unavailable. This applies to textures loaded from asset bundles unloaded with AssetBundle.Unload (false). (793679)</li>
<li>Graphics: Fixed a couple of bugs in the CPU mipmap generation (2D &amp; 3D) for floating point texture formats: RHalf, RFloat, RGHalf, RGFloat, RGBAHalf, RGBAFloat. (798702, 810632)</li>
<li>Graphics: Fixed a crash in the Editor when material and shader properties weren't updated correctly. (812576)</li>
<li>Graphics: Fixed a crash that would in some cases happen after Material.CopyPropertiesFromMaterial. (821208)</li>
<li>Graphics: Fixed a crash when blend shape value is changed for an object with cloth component. (710633)</li>
<li>Graphics: Fixed crashes on very large texture imports. (801677)</li>
<li>Graphics: Use Renderer::GetTransform() when calculating local AABB so that static batched renderers return the reference transform correctly.  (813671)</li>
<li>Graphics: Correctly unregister external native textures.</li>
<li>GUI: Fixed an issue where GUI::DrawTexture appeared darker than GUI::DrawTextureWithTexCoords when in Linear color space. (828145)</li>
<li>IL2CPP: Allow now Monitor.TryEnter to correctly obtain a previously taken lock that has been released, which did not work in some cases. (815783)</li>
<li>IL2CPP: Corrected some calls to HasValue on nullable types, which could return true when the nullable does not have a value. (819647, 821614)</li>
<li>IL2CPP: Corrected some calls to HasValue on nullable types, which could return true when the nullable does not have a value. (819647)</li>
<li>IL2CPP: Corrected the behavior of the is operator when used with a struct embedded in a parent generic class. (820071)</li>
<li>IL2CPP: Corrected the stack state handling during code conversion for some box opcodes. (826624)</li>
<li>IL2CPP: Fixed IPEndPoint on IPv6 network. (807653)</li>
<li>IL2CPP: Fixed the poor performance of string.Intern(). (821418)</li>
<li>IL2CPP: Generate C++ code properly now for two structs that contain arrays of each other as fields. (813962)</li>
<li>IL2CPP: Generate proper C++ code for some cases involving array parameters passed by reference. (818966)</li>
<li>IL2CPP: Prevent a stack overflow during code conversion which can occur for mutli-dimensional arrays with generic types. (815722)</li>
<li>IL2CPP: Properly marshal delegates when they are fields of a struct. (812570)</li>
<li>IL2CPP: Removed an unnecessary assert when GC.Collect(1) is called. The call will still have no impact though. (834376)</li>
<li>IL2CPP: Rename the types.h file to be il2cpp-string-types.h to avoid the possibility of is conflicted with a user-defined header file. (818102)</li>
<li>IL2CPP: Use the no-strict-overflow flag to compile generated C++ code on gcc and clang based compilers so that we match the integer overflow behavior of C#. (834633)</li>
<li>IL2CPP/Windows Store: Allow non-blocking sockets to work properly on 64-bit builds. (791721)</li>
<li>IL2CPP/XBboxOne: Prevent the C++ compiler from crashing while compiling the IL2CPPCompilerCalculateTypeValues.cpp file for some projects. This file was just too large in these cases, so IL2CPP will notw generate multiple smaller files instead. (805892)</li>
<li>Input: Mouse position is now updated but not clamped on wWindows when outside of game window. (827851)</li>
<li>Input: Work around an issue where cursor would disappear on touch based devices like Surface Pro 4. (817286)</li>
<li>iOS: Added missing iOSTargetOSVersion enum entries. (826595)</li>
<li>iOS: Building from GUI now uses a project relative path if the location is under the project folder (369773)</li>
<li>iOS: Corrected the default setting for bitcode on the XCTest target to fix a linker error. (824979)</li>
<li>iOS: Disabled certain Xcode debugging features in the project template causing memory usage to grow. (800209)</li>
<li>iOS: Fixed a crash due to linker error in simulator on startup in some cases certain Unity releases. (796762)</li>
<li>iOS: Fixed a crash when killing the app while a WWW Rrequest was in flight. (811959, 815928)</li>
<li>iOS: Fixed an issue where InputField.onEndEdit was called from an active InputField. (791844)</li>
<li>iOS: Fixed an issue where Touch.deltaTime was incorrectly returning zero when device had been on for approximately 30 days or more. (809752)</li>
<li>iOS: Fixed an issue with App store submissions with Xcode 8 when application is not using camera APIs (WebCamTexture).</li>
<li>iOS: Fixed iOS 10 simulator crash. (817335)</li>
<li>iOS: Fixed on-screen keyboard input for Chinese (Simplified) Pinyin 10 Key keyboard.</li>
<li>iOS: Fixed simulator crashes when device was rotated. (791063)</li>
<li>iOS: Fixed the appearance of apps freezing when locking/unlocking the device. (820863)</li>
<li>iOS: Fixed the run loop mode warning on iOS 10 devices.</li>
<li>iOS: Names for new iOS devices when selecting Unity Remote device. (815735)</li>
<li>Kernel: Fixed a crash resulting from redo after revert. (717587)</li>
<li>Kernel: Fixed a crash resulting from undo after reverting prefab. (804333)</li>
<li>Kernel: Fixed rounding error so Mathf.MoveTowardsAngle always reaches target angle. (790724)</li>
<li>Linux Standalone: Fixed an issue where pressing 'Alt' incorrectly reset Input.mousePosition. (816514)</li>
<li>Linux: Fallback to NET_WM_ICON for setting custom player icon. (735709)</li>
<li>Mono: Corrected a number of possible hangs with SSL sockets when the Unity Editor entered and exited the play mode. These hangs often showed up in the AuthenticateAsClient method. (759719, 759191, 733920)</li>
<li>Mono: Fixed a crash in compute_class_bitmap when using reflection. (822063, 816232)</li>
<li>Mono: Fixed a crash in find_method_in_metadata which can occur on startup. (763583)</li>
<li>Mono: Use an IPv4 address (if one exists) before an IPv6 address for .NET remoting connections. (826526)</li>
<li>Mono/IL2CPP: Corrected a rare deadlock in the C# lock implementation. (827984)</li>
<li>Networking: Fixed starting a server cashes on libwebsocket_service_fd. (810289)</li>
<li>Networking: ReliableFragmented channel stops working after client has disconnected, then reconnects. (810551, 810692)</li>
<li>OS X: Fixed HTTPS support for WWW/UnityWebRequest when Mac App Store receipt validation is on. (820523)</li>
<li>OS X: Fixed memory leak in joystick input handling code. (797793)</li>
<li>OS X: Fixed Screen.currentResolution.refreshRate being always 0. (764330)</li>
<li>OS X Player: The OSX standalone player now allows to switch out of the application by using Cmd+Tab when running in fullscreen mode. (798133)</li>
<li>OS X: Fixed a crash when building for OS X in certain circumstances to do with paths to splash screen and icon. (770034)</li>
<li>Particles: Fixed an issue where playing the scene with more than 270 particle prefabs caused a crash. (813872)</li>
<li>Plugins: Fixed an issue where DLL plugins with non-lowercase extensions cause the architecture platforms panel not to be displayed. (805669)</li>
<li>Prefabs: Fixed some issues and crashes related to undo-ing the creation of prefabs and prefab connections. (808187, 790220, 816014)</li>
<li>Shaders: Fixed frac(constant) sometimes being mis--compiled. (825235)</li>
<li>Shaders: Fixed shader compiler bug which could have caused errors in GLSL shaders that might crash the GPU on OSX.</li>
<li>Shaders: Fixed some cases of inout struct variables with COLOR semantic members wrongly translating into GLES2.0. (720704)</li>
<li>Shaders: Fixed transparent shader writing into DepthNormals texture, because material sometimes cache RenderType setting. (806751)</li>
<li>Shaders: Fixed UNITY_APPLY_FOG not working as expected if an expression is passed as fog coordinate. (822553)</li>
<li>Textures: Correctly unregister external native textures.</li>
<li>Tizen: Fixed a problem with UnityPluginLoad() not working.</li>
<li>tvOS: Fixed 2nd stage splash screen. (777937)</li>
<li>tvOS: Fixed allowed scripting implementations and architectures in player settings.</li>
<li>UAP: Fixed an incorrect resolution being reported when the composition scale changed and the game window was minimized. (832104)</li>
<li>UAP: Fixed the incorrect language being returned when system language was Spanish(Argentina). (820162)</li>
<li>UI: Fixed a memory leak caused by IntermediateRendererstemporary renderer objects not being cleaned up. (819470)</li>
<li>UI: Fixed a race condition in UI mesh processing leading to rare crashes. (797645)</li>
<li>UI: Fixed a random crash in SyncElement caused by unknown parent canvas.</li>
<li>UI: Fixed an issue with animating canvas properties not applying. (809374, 825435)</li>
<li>UI: Fixed an issue with Canvas sorting order being incorrect under certain cases. (821727)</li>
<li>UI: Fixed issue where Canvas/UI appeared darker when camera was disabled and color space was set to Linear. (797560, 633000)</li>
<li>UI: Fixed issue with OnPointerEnter event firing after touch ends.</li>
<li>UI: Fixed the issue with double rendering of world canvas in the Editor. (803901)</li>
<li>UnityWebRequest: Fixed a possible freeze when using custom download handler script. (820517)</li>
<li>VCS: Fixed a problem when moving folders in the project view end up with errors and inconsistent state between local file state and VCS state. (714707)</li>
<li>VCS: Stop a C++ method being called during C# constructor and serialization (which is a scripting warning as it is unsafe to do this).</li>
<li>VR: Fixed a crash at startup on GearVR if Focus is lost very close to the time or the app starting.</li>
<li>VR: Fixed a crash when an invalid Oculus plugin is used. Throws warning instead. (803937)</li>
<li>VR: Fixed different particle shader transparencies between editor and build when splash screen is active. (806810)</li>
<li>VR: Fixed HoloLens touch injection for flat apps.</li>
<li>VR: Removed an audio output warning when Unity Audio is Disabled. (826132)</li>
<li>WebGL: Fixed asset bundles memory usage at loading time, preventing some content to run on 32-bit browsers. (812567, 829765)</li>
<li>WebGL: Fixed browser lock-up when profiling. (759492)</li>
<li>WebGL: Fixed Code Blob memory leak.</li>
<li>WebGL: UnityWebRequest.downloadProgress now returns the actual progress as opposed to 0. (775178)</li>
<li>WebRequest: Fixed a possible freeze when using custom download handler script. (820517)</li>
<li>WebRequest: Allow empty headers as that is in general valid.</li>
<li>WebRequest: Allow setting Accept-Encoding header from scripting at users own risk. (825429)</li>
<li>WebRequest: More correctly follow the HTTP Specification for sending POST data during a Redirect. (814388)</li>
<li>Windows Standalone: Custom image will be correctly shown in screen selector dialog when building to directory with non-english letters. (801951)</li>
<li>Windows Standalone: Fixed a regression where "touch up" events would be lost when occurring outside window bounds. (803319)</li>
<li>Windows Store: Fixed a bug where mouse scroll wheel was returning inverted values. (813683)</li>
<li>Windows Store: Fixed a potential crash on Xbox One when retrieving advertising id.</li>
<li>Windows Store: Fixed a rare deadlock when recursively calling InvokeOnAppThread and InvokeOnUIThread many times.</li>
<li>Windows Store: Fixed an assert that happened on startup on Xbox One in debug builds.</li>
<li>Windows Store: Fixed touch screen keyboard input not working on UWP. (808700)</li>
<li>Windows Store: Fixed Unity PDB files not getting included into built .appxsym package. (831144)</li>
<li>Windows Store: Fixed Xbox Live SDK not being automatically referenced by C# scripts if installed on the machine</li>
<li>Windows Store: Gamepads (with UsagePage/Usage 0x0001/0x0005) will correctly connect to an application now. Usually these are device connected via bluetooth. Previously only joysticks (with UsagePage/Usage 0x0001/0x0004) would connect. You can check UsagePage/Usage of the device by right clicking Properties on the device-&gt;Hardware-&gt;HID-compliant game controller-&gt;Properties-&gt;Details-&gt;Hardware Ids. For ex., gamepads will contain an item "HID_DEVICE_UP:0001_U:0005) . You might need to delete Package.appxmanifest, because there's a new item for HID device. (816582)</li>
<li>Windows Store: UnityEvent.Remove listener will work correctly when .Net Native is enabled. Previously events were not removed as expected. (827748)</li>
<li>Windows Store: When updating Windows Phone 8 application to Windows Phone 8.1/10.0, player prefs will be auto updated if the following condition is met - UnityPlayer.upp file exist, but playerprefs.dat file doesn't exist in LocalFolder. (810622)</li>
<li>Windows: Added safety check when receive new window size with zero values, make minimum value 1, otherwise functions like CreateDepthStencilView will fail.</li>
<li>Windows: System resolution or orientation changes are now detected and responded to accordingly. (825230)</li>
<li>WWW: Make Dispose asynchronous to prevent freeze or performance drop, as it might be costly. (782109)</li>
</ul>

#### Revision: c347874230fb
