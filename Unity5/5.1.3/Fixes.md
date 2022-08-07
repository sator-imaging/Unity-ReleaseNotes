# Unity 5.1.3
https://unity3d.com/unity/whats-new/unity-5.1.3

## Fixes

<ul>
<li>(709326) -  2D: Fixed spriteRenderer overwriting materials for objects in case of multiple selection.</li>
<li>(707880) -  2D: Prevent all editing in Sprite Editor Window during play mode.</li>
<li>(none) -  Android: Audio - Fixed CPU consumption by FMODAudioDevice thread on GearVR.</li>
<li>(none) -  Android:&nbsp;Fixed call to ES API without current context.</li>
<li>(701873) -  Android: Fixed performance regression in Resources.Load.</li>
<li>(703999) -  Android: Fixed texture compression setting for RGBA textures.</li>
<li>(694503) -  Asset Loading: Fixed missing references when scene is loaded from an asset bundle which contains multiple scenes.</li>
<li>(707079) -  AssetBundle: Fixed the crash when a scriptable object is referenced from the scene.</li>
<li>(683134) -  AssetBundle: Fixed the issue that AssetBundle with packed textures includes source textures in addition to the atlased version.</li>
<li>(670282) -  BlackBerry: Fixed crash that would happen with some projects on the Passport after consecutive runs.</li>
<li>(704009) -  BlackBerry: Fixed crash when using Development builds on the STL-001 device.</li>
<li>(none) -  BlackBerry: Fixed issue that would cause a grey screen to appear between the splash screen and the start of the game.</li>
<li>(673296) -  Editor: Enabling Script Only Build option will only affect platforms that allow the option.</li>
<li>(708787) -  Editor: Fixed 'Timestamps and assets out of sync' error when renaming a folder outside of Unity and deleting an asset inside of it.</li>
<li>(709495) -  Editor: When saving a scene in the Windows editor, the characters from the dynamic fonts would disappear.</li>
<li>(707688) -  GI: Fixed crash when building lighting.</li>
<li>(none) -  GI: Fixed issue with baking getting stuck on the bake indirect stage.</li>
<li>(690395) -  Graphics: Added extra protection against depth buffer in editor windows being accidentally disabled.</li>
<li>(693316) -  Graphics:&nbsp;Configurable vertex compression to fix lightmap UVs shifting.</li>
<li>(697054) -  Graphics: Fixed a crash compressing an already compressed texture in script.</li>
<li>(678429) -  Graphics: Fixed an issue where setting RenderSettings.reflectionIntensity via script had no effect on the scene.</li>
<li>(700698) -  Graphics: Fixed artifacts in alpha channel of ATC-compressed RGBA textures when using Mac OS X Editor.</li>
<li>(679342) -  Graphics: Fixed CaptureScreenshot on DX11 when using non-native fullscreen resolution.</li>
<li>(691477) -  Graphics: Fixed crash calling GetPixels with a 0x0 texture</li>
<li>(662018) -  Graphics: Fixed swizzling of BGRA32 texture data on D3D11 and Xbox360.</li>
<li>(681662) -  Graphics: Switching shaders in material inspector should reset material's render queue to default.</li>
<li>(701319) -  Graphics: When using COLORMASK and D3D9, the mask was not correctly set for MRT render targets.</li>
<li>(702323) -  IMGUI: Fixed text vertical position shifting during edit when the line height is too big for the box.</li>
<li>(697178) -  Input / OSX standalone: Mouse buttons are registered when configuring input settings.</li>
<li>(704815) -  Input: Fixed touch input hanging a Windows application if a second 'touch window' is created in a plugin.</li>
<li>(704335) -  Inspector Functionality: Fixed component Help buttons on OS X.</li>
<li>(701951) -  iOS: Added Xcode 6.4 compatibility.</li>
<li>(706601) -  iOS: Fixed a regression that caused very poor performance of trying to load non-existing system fonts.</li>
<li>(709024) -  iOS: Fixed crash accesing WebCamTexture videoRotationAngle and videoVerticallyMirrored before it is fully inited.</li>
<li>(709063) -  iOS: Fixed snapshot creation (when going to background) on pre-ios8.</li>
<li>(674706) -  iOS/IL2CPP: Allow GetCurrentProcess to work.</li>
<li>(none) -  iOS/IL2CPP: Allow il2cpp.exe to run when its installation path includes a '#' character followed by a space character.</li>
<li>(711284) -  iOS/IL2CPP: Allow the AssemblyName::GetPublicKeyToken method to return an array of only eight bytes.</li>
<li>(709995) -  iOS/IL2CPP: Corrected a problem with the generated C++ code which caused the C++ compiler error: "Member reference base type 'intptr_t' (aka 'long') is not a structure or union" when unsafe C# code was used to index into an array of pointers to structures.</li>
<li>(689976) -  iOS/IL2CPP: Corrected an intermittent hang which could occur in the garbage collector.</li>
<li>(712470) -  iOS/IL2CPP: Corrected Marshal.OffsetOf when using enums fields with FieldOffsetAttribute.</li>
<li>(712713) -  iOS/IL2CPP: Ensure methods needed for enum arrays are converted.</li>
<li>(708876) -  iOS/IL2CPP: Fixed binary operations using mixed integer types.</li>
<li>(770440) -  iOS/IL2CPP: Fixed bug in Boo script related to generic interface methods.</li>
<li>(689586) -  iOS/IL2CPP: Fixed CultureInfo.GetCultures().</li>
<li>(none) -  iOS/IL2CPP: Fixed marshaling code for IntPtr parameters marked with [Out] attribute.</li>
<li>(708527) -  iOS/IL2CPP: If "Fast but no Exceptions" is selected, any managed exception which escapes out of managed code will cause the AppDomain.UnhandledException event - to be executed and application will abort (this is the same behavior as the Mono scripting backend).</li>
<li>(676797) -  iOS/IL2CPP: Implemented the IsTransparentProxy icall, which always returns false.</li>
<li>(705751) -  iOS/IL2CPP: Implemented the previously unsupported AppDomain::InternalGetDefaultContext and AppDomain::InternalGetContext icalls.</li>
<li>(none) -  iOS/IL2CPP: Improved performance of 'is' operator, 'as' operator, and casting in some cases.</li>
<li>(710797), (705882) -  iOS/IL2CPP: Prevent a type T from being stripping if it is used an GenericClass field in a MonoBehavior or ScriptableObject that is already being preserved.</li>
<li>(711712) -  iOS/IL2CPP: Prevent the following error from il2cpp.exe at conversion time: "Attempting to constrain a value of type 'X' to type 'Y'." for two different types X and Y.</li>
<li>(none) -  iOS/IL2CPP: Properly look up a type using the Type.GetType(string) method during a case-insensitive search.</li>
<li>(none) -  iOS/Metal: Fix potential geometry corruption</li>
<li>(650630) -  Mac OS X Standalone: Fixed stripping of debug symbols in release player builds.</li>
<li>(none) -  Mecanim: Fixed a bug where a state machine moved to another state machine would disappear.</li>
<li>(705342) -  Mecanim: Fixed performance regression for AnimationUtility.SetEditorCurve().</li>
<li>(none) -  Merge Tool: Correctly handle invalid non-unique mapping keys that Unity generates.</li>
<li>(none) -  Merge Tool: Fixed empty base/right files when falling back and used from cmdline and premerge dests are not set.</li>
<li>(none) -  Merge Tool: Fixed merge conflict when mine and theirs have both added a component of different type to the same GameObject.</li>
<li>(none) -  Merge Tool: Fixed the error about non existing merge tool path after falling back to 3rd party merge tool on OSX.</li>
<li>(693714) -  Metal: Fixed shader translation of matrix+scalar, matrix-scalar, matrix/scalar operations.</li>
<li>(693714) -  Metal: Fixed some issues with shader translation of matrices with different precision.</li>
<li>(none) -  Mono: Double traverse object count to avoid stack overflow when freeing huge amounts of objects.</li>
<li>(none) -  Mono: Fixed monotonic timer overflow to allow usage of timing functions like those in System.Threading with extended uptime.</li>
<li>(none) -  Networking: Fix for llapi statistic function + new statistic function GetNetworkLostPacketNum().</li>
<li>(none) -  Networking: Timing service is working now.</li>
<li>(none) -  OS X: Fixed building on OS X El Capitan.</li>
<li>(706330) -  OSX standalone: Fixed mouse input and rendering issues after the application is moved to a different screen and is made fullscreen.</li>
<li>(704468) -  Physics: Fixed 'Physics2D.GetRayIntersectionXXX' methods being affected by 'Physics2D.raycastsStartInColliders'.</li>
<li>(703073) -  Physics: Fixed an issue where OnTriggerStay would not be called on children in compound colliders.</li>
<li>(705148) -  Physics: Fixed incorrect depth sorting for results of 'Physics2D.GetRayIntersectionXXX' methods.</li>
<li>(692675) -  Physics: Fixed WheelCollider not being able to ignore collisions with vehicle body colliders that were added to the already initialised vehicle.</li>
<li>(691057) -  Physics: Fixed WheelCollider suspension raycasts being unable to ignore intersections with the car’s body the wheel has been attached to, occasionally.</li>
<li>(none) -  Physics2D: Now 'Infinity' cannot be specified for 2D collider offset.</li>
<li>(707400) -  Physics2D: Stop Rigidbody2D X/Y Constraints from occasionally moving the body to the world origin.</li>
<li>(713073) -  Physics2D: Stop trigger-contacts being reported early when using continuous collision detection.</li>
<li>(none) -  Samsung TV: Added missing Indian character sets to 2015 TV.</li>
<li>(none) -  Samsung TV: Fixed freetype crash on 2013 TV.</li>
<li>(none) -  Samsung TV: Fixed issue where UnityAnalytics was initializing improperly.</li>
<li>(none) -  Samsung TV: Fixed race condition that could cause intermittent crashes when managed threads were being used.</li>
<li>(695246) -  Scripting: Fixed potential crashes during domain reloads when user code throws NullReferenceException in AppDomain.DomainUnload / AppDomain.ProcessExit events.</li>
<li>(643440) -  Serialization: Fixed incorrect clamping of LayerMask when set through SerializedProperty.intValue.</li>
<li>(711981) -  Substance: Fixed crash in iOS/il2cpp builds caused by uninitialized SubstanceSystem.</li>
<li>(706380) -  Substance: Fixed crash with BakeAndDiscard ProceduralMaterials.</li>
<li>(none) -  Substance: Using _TexelSize in shaders now works correctly with ProceduralTextures.</li>
<li>(none) -  Tizen: Fixed an issue with sound stopping when apps are interrupted.</li>
<li>(none) -  Tizen: Fixed corrupted audio.</li>
<li>(none) -  Tizen: Fixed errors when building projects that contain spaces in the path.</li>
<li>(715415) -  Tizen: Fixed issue where Good autorotation orientations were incorrect.</li>
<li>(none) -  Tizen: Resolve deployment problems on Windows.</li>
<li>(693283), (672115) -  UI: Fixed issue in UI components Slider, Outline, Shadow &amp; Position as UV1 not updating when their values are animated.</li>
<li>(714670) -  UI: Fixed Toggle component not updating when animated.</li>
<li>(none) -  UnityAnalytics: Fixed RemoteConfig restore of int values.</li>
<li>(none) -  UnityAnalytics: Remote config fix added.</li>
<li>(none) -  Version Control: Fixed assets version control cache state not being updated after scene reload.</li>
<li>(none) -  Version Control: Invalidate version control cache on refresh button click in versioning window.</li>
<li>(695727) -  VR Oculus: Camera Viewport Rect now takes up the appropriate amount of Screen space.</li>
<li>(703281) -  VR Oculus: Fixed crash when trying to access VRSettings.GetNativePtr while the Oculus HMD was not connected.</li>
<li>(none) -  VR Oculus: HMD can now be connected to application after it has already started. It can also be disconnected and reconnected during application run time.</li>
<li>(none) -  VR Oculus: Update to latest oculus dependencies.</li>
<li>(none) -  VR: Camera transforms now reset when VRSettings.enabled is false or the loadedDevice is set to none. Camera parent transforms are not effected.</li>
<li>(713630) -  VR: Fixed several VR lifecycle related crashes.</li>
<li>(none) -  VR: Fixed stereo rendering regression.</li>
<li>(none) -  VR: Improved MSAA performance by only antialiasing eye textures, not the composited back buffer.</li>
<li>(691345) -  VR: Reenable vsync when device is disconnected.</li>
<li>(none) -  VR: Virtual Reality Supported toggle in player settings no longer recreates the Graphics Device. VRSettings defaults to enabled and oculus if Virtual Reality is supported.</li>
<li>(714022) -  VR: VRDevice.isPresent now returns expected value.</li>
<li>(none) -  WebGL: Allow Type.GetType(string) and its overloaded methods to work without Exception Support set to Full. IL2CPP: Properly look up a type using the Type.GetType(string) method during a case-insensitive search.</li>
<li>(700861) -  WebGL: Fixed backspace key navigating away from page in Chrome.</li>
<li>(714545) -  WebGL: Fixed empty Input.inputString.</li>
<li>(705045) -  WebGL: Fixed mouse button state after double click.</li>
<li>(712636) -  WebGL: Fixed UI keyboard inputs.</li>
<li>(704235) -  WebGL: Fixed WebGL builds of projects with long path names on Windows.</li>
<li>(711745) -  Windows Store Apps: Application.isMobilePlatform will now return true.</li>
<li>(710069) -  Windows Store Apps: Fixed incorrectly reported PlayerPrefs corruption after upgrading to Unity 5.1.</li>
<li>(710038) -  Xbox One: Fixed error for uninitialized player settings </li>
<li>(708668) -  Xbox One: Fixed instances where Compute Shaders would not compile.</li>
<li>(705618) -  Xbox One: Fixed spelling errors in ESRB ratings strings in the Player Settings.</li>
<li>(701308) -  Xbox One: Level and asset files are paired correctly in the auto-generated package manifest.</li>
<li>(none) -  Xbox One:&nbsp;Mono: Double traverse object count to avoid stack overflow when freeing huge amounts of objects.</li>
</ul>
