# Unity 5.3.3
https://unity3d.com/unity/whats-new/unity-5.3.3

## Fixes

<ul>
<li>2D: Fixed memory leak when applying changes to sprite. (754282) </li>
<li>2D: Occlusion Culling works correctly with X/Y flipped SpriteRenderers. (760062)</li>
<li>Android: Fixed internal profiler on Gear VR. (741003) </li>
<li>Android: Fixed missing styles.xml files. (768027) </li>
<li>Android: Fixed remote frame debugger. (742199) </li>
<li>Android: Marshmallow - Added the possibility to disable the permission dialog by adding metadata to the activity.  </li>
<li>Android: Mono - Fixed crash on startup with Unity Ads when stripping is enabled. (755510) </li>
<li>Android: Timeout no longer happens when an application is sent to the background. (738843) </li>
<li>Animation: Fixed a crash when changing OverrideController on Animator with no Avatar. (741043) </li>
<li>Animation: Fixed a crash where assigning an override controller with no controller to override. (764778) </li>
<li>Animation: Fixed changing Animator.runtimeAnimatorController while in play mode crashing the editor. (731237)</li>
<li>Animation: Fixed Euler angles on rotation causing Transform to be set to NaN in some cases. (759408, 760759)</li>
<li>AssetBundle: Change to use natural sorting when listing the AssetBundle names. (736556) </li>
<li>AssetBundle: Fixed loading error for asset bundles built with DisableWriteTypeTree flag. (756567) </li>
<li>AssetBundle: Fixed the hash collision when building AssetBundles. (716166) </li>
<li>AssetBundle: Fixed the issue that LoadAsset(name) returns null if a bundle contains a prefab and another asset with the same name. (743704) </li>
<li>AssetBundle: Loading multiple invalid asset bundles fails correctly now. (756198) </li>
<li>AssetBundles: Fixed AssetBundle.CreateFromFile retaining file descriptor. - The previous fix was incomplete. (715753) </li>
<li>Audio: Fixed mixer reverb effects getting cut off early in standalone builds. (760985) </li>
<li>Audio: Avoid random crashes when using audio callbacks in scripts. (739224, 761360) </li>
<li>Core: Fixed crash when game object that is a child of a missing prefab is deleted. (757799) </li>
<li>Core: Improved the error message when build data files are corrupted or from a mismatched version.</li>
<li>Core: Make sure persistent transforms are not added to the active scene when running in a player. (758058) </li>
<li>Editor: Fixed issue of a new scripts created in Editor folder if Unity installation path contains "test" word. (761664) </li>
<li>Editor: Fixed a bug where Undo recording would insert property modification on the prefab asset if it was being edited in the inspector. (711720) </li>
<li>Editor: Fixed crash when entering playmode if LoadScene was called during Awake or Start. (756409, 760459) </li>
<li>Editor: Fixed crash when replacing prefabs with Alt button pressed. (753176) </li>
<li>Editor: Fixed editor freeze when picking in scene with many overlapping game objects. (730441) </li>
<li>Editor: Fixed freeze/crash on project startup when async upload buffer is set too small. (754704) </li>
<li>Editor: Fixed game object duplicates on play when reference to that game object is set in another scene. (750117) </li>
<li>Editor: It is now possible to replace a prefab asset with a different prefab asset. (761995) </li>
<li>Frame Debugger: Even when it was not used, it was creating some overhead in development standalone builds. Reduced that. </li>
<li>GI: Fix for lightmaps in linear lighting mode looking different between the player and editor. (724426) </li>
<li>GI: Fix for LoadLevel in the player causing lightmaps to become brighter when in Linear mode. (728595, 738173) </li>
<li>GI: Fixed brightly coloured (green/red/white/blue) pixels appearing in the directional lightmap caused by interpolation from invalid indirect lightmap data. Note: Need to clear the GI cache and rebake to get the fixed lightmaps. (765205, 734187) </li>
<li>GI: Fixed missing Ambient when "Baked GI" is disabled and "Ambient GI" is set to Baked. (756506) </li>
<li>Graphics: Fixed a crash in the editor when switching graphics API from a non-DX9 API e.g. DX11. (740782) </li>
<li>Graphics: Fixed an issue where Standard shader using directional lightmaps could output NaN to the framebuffer. This would usually blow up when using HDR rendering with Bloom. </li>
<li>Graphics: Fixed building shaders correctly for WebGL in AssetBundles. (746302) </li>
<li>Graphics: Fixed crash when calling Graphics.DrawMesh with null material. (756849) </li>
<li>Graphics: Fixed crash when using GL.Begin quad rendering with non-multiple-of-4 vertex count. (761584) </li>
<li>Graphics: Fixed video memory leak in the splash screen animation. </li>
<li>Graphics: Fixed occasional Movie Texture crash with multiple movies present. (753593, 764084) </li>
<li>Graphics: Fixed profiling related information (SetGpuProgramName) performance issue in development player builds. </li>
<li>Graphics: Fixed rendering of deferred reflections when last object rendered before them had negative scale. (757330) </li>
<li>Graphics: Fixed skinned mesh memory leak. (760665) </li>
<li>Graphics: In Editor OpenGL ES 2.0 emulation increase max cubemap size to 1024 (from 512). (650870) </li>
<li>Graphics: Reduced framerate spikes where culling system could sometimes stall for several ms while waiting for jobs. </li>
<li>Graphics: Textures imported as cubemaps now are properly marked as non-readable if import option says so. Saves memory! (724664) </li>
<li>IL2CPP: Avoid crash on IL2CPP when searching for attributes. (766208) </li>
<li>IL2CPP: Avoid double allocation of memory for multi-dimensional arrays. (766168) </li>
<li>IL2CPP: Fixed performance regression in LivenessState calculation. The performance is back to where it was prior to 5.3.2p2. </li>
<li>IL2CPP: Fixed an occasional crash when capturing managed heap when parts of it are not committed. </li>
<li>IL2CPP: Fixed Array.Copy when destination array type is wider than source array type (e.g. int[] -&gt; long[]). (741166) </li>
<li>IL2CPP: Fixed Stfld/Ldfld opcode usage generated by MS C# compiler. (761530) </li>
<li>IL2CPP: Fixed Unity IAP on Android with IL2CPP. (761763) </li>
<li>IL2CPP: Generate proper C++ code for marshaling wrappers of methods that have System.Guid as a parameter type. (766642) </li>
<li>IL2CPP: Implemented support for Assembly.GetReferencedAssemblies and Module.GetTypes() (724547) </li>
<li>IL2CPP: Properly marshal arrays of four-byte bool values. (767334) </li>
<li>IL2CPP: Raised NullReferenceException when Ldvirtftn instruction had a null target. (766208) </li>
<li>iOS: Added missing icon for iPad Pro. (755415) </li>
<li>iOS: Fix for WWW deadlock. (759480) </li>
<li>iOS: Fixed a crash triggered by deactivating an input while app is going into background. (760747) </li>
<li>iOS: Fixed an issue where attached controllers were not found. (761326) </li>
<li>iOS: Fixed application freeze on iphone4 when rotating device. (761684) </li>
<li>iOS: Fixed code completion for iOS Editor Extensions. (759212) </li>
<li>iOS: Handheld.PlayFullScreenMovie only allows playing one movie at a time. </li>
<li>iOS: Notify Transport that we finished receiving data so we can mark the buffer as complete when we get an error. (761361) </li>
<li>iOS: While entering background/foreground, improve player pause/resume handling to check if external parties (like video player) currently manage the paused state. (534752) </li>
<li>iOS/IL2CPP: Prevent a managed exception on 64-bit builds during some array creation operations which has the message "ArgumentException: Destination array was not long enough. Check destIndex and length, and the array's lower bounds". (765910) </li>
<li>iOS/OSX: Fixed SIMD math, which fixes skinning on iOS and source code compilation on OSX. (754816) </li>
<li>iOS/Video: AVKit based player didn't show "done" button on iOS 8+. (736756) </li>
<li>iOS/Video: Fixed MPMoviePlayer error handling for invalid files.</li>
<li>iOS/Video: Improved MPMoviePlayer/AVKit orientation and view controller handling. (746018, 729470) </li>
<li>iOS/Video: Scaling mode behaviour fixes for iPad Pro. (745346) </li>
<li>iOS/Xcode: Added .tbd extension support.</li>
<li>Linux: Fixed flickering/corrupted rendering with OpenGL Core. (770160) </li>
<li>Linux: Fixed non-native-resolution fullscreen rendering with OpenGL Core. (763944) </li>
<li>Mono: Corrected a crash in mono_string_to_utf8_checked when Marshal.StructureToPtr is called from managed code. (759459) </li>
<li>Mono: Resolved intermittent crash caused by a race condition that occurs when using managed threads.</li>
<li>MSE: Fixed the issue that calling SceneManager.LoadScene** while exiting playmode causes scene unremovable from the hierarchy. (756218) </li>
<li>MSE: Fixed the issue that SceneManager.sceneCountInBuildSettings gives 0 until entering play mode. (754925) </li>
<li>Networking: Fixed issue where NetworkManager doesn't become "ready" if online scene is set and offline scene is not. (734218) </li>
<li>Networking: Fixed issue where OnStartAuthority is called twice on hosts. (748967) </li>
<li>Networking: SyncLists now only send updates when values change. (738047) </li>
<li>OpenGL Core: Various bug fixes to the shader compiler; often resulting in better performance for complex image effect shaders. </li>
<li>OpenGL Core: Fixed random crashes on compute shader dispatch. (761412) </li>
<li>Particles: Ensure consistent direction between 3D and 1D rotation. (760830) </li>
<li>Particles: Fix for terrains ignoring collision layers. (763041) </li>
<li>Particles: Fixed a collision crash. (757969) </li>
<li>Particles: Fixed IsFinite error spam with particles and second camera. (756786) </li>
<li>Particles: Fixed issue where particle system doesn't play if method is called via Invoke. (757461) </li>
<li>Particles: Fixed issue where particle system is stopped and cleared and after that it won't play when simulation space is set to local. (756971) </li>
<li>Particles: Fixed issue where particles are not drawn in the correct order on rotated particle systems. (696610) </li>
<li>Particles: Fixed issue where ParticleSystem.IsAlive() always returns True for particle systems with longer duration. (755677) </li>
<li>Particles: Fixed issue whereby particles systems are not looping correctly. (756742) </li>
<li>Particles: Fixed particle culling issues. (764701) </li>
<li>Particles: Fixed support for negative inherit velocity values. (758197) </li>
<li>Particles: Fixed the issue of particles disappearing after going offscreen and returning. (759502) </li>
<li>Particles: Fixed wrong culling of some particle objects caused by incorrect bounds calculation due to parent scaling. (723993) </li>
<li>Particles: Fixed: particle system not playing when triggered via Event Trigger. (756725) </li>
<li>Particles: Fixed: particle system only playing once. (756194) </li>
<li>Particles: Particles are now emitted with the correct position//rotation when using a Skinned Mesh Renderer or Mesh Renderer as shape. (745121) </li>
<li>Physics: Fixed center of mass and inertia tensor being reset after game object was reactivated. (765300) </li>
<li>Physics: Rigidbodies without non-trigger colliders can. have custom center of mass and inertia tensor again (763806) </li>
<li>Renderdoc: When making a RenderDoc capture from editor UI, make sure to include the whole frame including user script updates. </li>
<li>Scripting: Fixed issue that causes UnityScript to incorrectly detect some methods return type. (754405) </li>
<li>Scripting: Prevent the Particle System from being stripped if the Particle System Renderer is used and engine code stripping is enabled. (761784) </li>
<li>Shaders: Fixed a shader compiler crash if a compute shader declares a samplerstate that didn't match the naming scheme. </li>
<li>Shadows: Changed light shadows near plane minimum bound to either 1% of range or 0.1, whichever is lower. </li>
<li>Shadows: Fixed "half of scene all in shadows" artifacts in some scene/camera setups. (743239) </li>
<li>Smart TV: Fixed a problem to show custom splash screen.  </li>
<li>Sprites: Occlusion Culling works correctly with X/Y flipped SpriteRenderers. (760062) </li>
<li>Substance: Fixed corner cases of outputs not being impacted by any input not being generated. (754556, 534658, 762897) </li>
<li>Tizen: Fixed cursor initially starting in the wrong position on screen. (740180) </li>
<li>Tizen: Fixed OpenGL crashing issues on the Z300F. </li>
<li>Tizen: Input field will no longer show&nbsp; when return is pressed on an empty entry. (740172) </li>
<li>Tizen: System permissions that are not required are no longer requested. </li>
<li>tvOS: Fixed build error with Xcode trampoline. (767645) </li>
<li>tvOS: Fixed Game Center score reporting due to incorrect API check. (755395) </li>
<li>UI: Fixed "Trying to add (Layout Rebuilder for) Content (UnityEngine.RectTransform) for layout rebuild while we are already inside a layout rebuild loop." error. (739376, 740617) </li>
<li>UI: Fixed flickering/texture swapping issues. (753423, 758106) </li>
<li>UI: Fixed issue with incorrect accent calculation for non-dynamic fonts. (747512) </li>
<li>Upgrades: Delete the installed Playback Engines and Documentation before upgrading Unity. (756818) </li>
<li>VR: Dynamically switch to headset's audio output / input driver (Oculus SDK 1.0+).</li>
<li>VR: Fixed audio redirection in standalone builds (Oculus SDK 1.0+).</li>
<li>VR: Fixed crash when trying to enter play mode when the Plugin was not loaded or the Oculus runtime was not installed. (759841) </li>
<li>VR: Fixed Skybox clipping issues. (755122, 717989, 734122) </li>
<li>VR: Fixed VR Focus and VR ShouldQuit not respecting notifications when the Device was disconnected.</li>
<li>VR: Fixed VR Splash screen color precision. </li>
<li>WebGL: Corrected the following compiler error which might occur in generated C++ code: "error: non-constant-expression cannot be narrowed from type 'uintptr_t' (aka 'unsigned int') to 'il2cpp_array_size_t' (aka 'int') in initializer list [-Wc++11-narrowing]". (767744) </li>
<li>Windows Store : Building from Unity will no longer overwrite project.json file if it was modified in solution. (765876) </li>
<li>Windows Store : When building from Unity files in Visual Studio solution will not be overwritten if identical. (759735) </li>
<li>Windows Store: Fixed a "MdilXapCompile failed" error when trying to build Visual Studio project for Windows Phone 8.1. This used to happen when the Unity game had over 8000 classes across all assemblies. (762582) </li>
<li>Windows Store: Fixed a crash when loading C# type from plugin which was not included in the final build. (765893) </li>
<li>Windows Store: Fixed a crash which happened on "Windows N" versions when using IL2CPP scripting backend. (760989) </li>
<li>Windows Store: Fixed a rare crash in ARM linker (fatal error LNK1322: cannot avoid potential ARM hazard (QSD8960 P1 processor bug) in section #) when using IL2CPP scripting backend. (766755) </li>
<li>Windows Store: Fixed an issue which caused small tiles get copied to Visual Studio solution incorrectly for Windows Phone 8.1 SDK. (762926) </li>
<li>Windows Store: Fixed anti-alising when calling Screen.SetResolution on Universal Windows 10 Apps/. </li>
<li>Windows Store: Fixed Application.Quit() when using D3D project type or IL2CPP scripting backend. (764378) </li>
<li>Windows Store: Fixed error "Task 'ExpandPriContent' failed." which occurred when trying to build an application package with IL2CPP scripting backend when using default Unity icons. (764632) </li>
<li>Windows Store: Fixed Visual studio graphics debugger crashing when trying to debug Windows Phone 8.1 projects.  </li>
<li>Windows Store: Mouses and touches will work correctly after locking/unlocking the screen. (768929) </li>
<li>Windows Store: Screen.Resolution(x, y, true) will no longer ignore width and height, so you can set your desired resolution on Universal Windows 10 Apps. </li>
<li>Windows Store: Screen.resolutions will return a valid value. (748845) </li>
<li>WinRT/IL2CPP: Allow native DLLs to be loaded both with and without the .dll extension. (760041) </li>
<li>XboxOne: Fixed a bug with YUY2 processing on the XboxOne. </li>
<li>XboxOne/IL2CPP: Fixed a problem compiling generated C++ files when there is a space in the path to the project directory. (768193) </li>
</ul>

#### Revision: 910d71450a97
