# Unity 2017.2.3f1
https://unity3d.com/unity/whats-new/unity-2017.2.3

## Fixes

<ul>
<li>2D: Fixed an issue that was causing the Physics Shape of a Sprite2D to not being properly set unless the 'Edit Physics Shape' tab was opened first. (986368)(985912)</li>
<li>Android: Workaround gyroscope lag issues that happen on some android devices. (912848)</li>
<li>Android: Fixed Time.deltaTime sometimes returning a negative value on certain devices/Android versions. (1013174 (970945)</li>
<li>Android: Fixed unity pausing during Android Handheld.PlayFullScreenMovie start. (978599)</li>
<li>Android: Fixed possible crash with Performance Reporting enabled. (965024)</li>
<li>Android: Fixed Skybox distortion on specific Android devices with Vivante GC1000/GC2000 GPU. (967647)(903140)</li>
<li>Asset Import: Fixed crash when importing fbx .meta files that contain references to inexisting scripts. (999832)(960267)</li>
<li>AssetBundles: Fixed packing AudioMixerController, AudioMixerGroup and AudioMixerSnapshot into bundles with disabled type trees. (976768)</li>
<li>Audio: Fixed a bug where the matrices passed to spatializer and ambisonic plugins could be set to the identity matrix briefly when a sound starts playing. (991034)</li>
<li>Build Pipeline: Fixed old UnityChannel Xaiomi files not being deleted when new package manager package is installed. (None)</li>
<li>Editor: Fixed local assets being overwritten during collab update. (1014028)(952569)</li>
<li>Editor: Fixed editor crashing in "RenderSelectionOutline" when using ImageEffectAllowedInSceneView and set camera's targetTexture to null. (966404)</li>
<li>Editor: Fixed an issue where changing override format on a texture could cause Unity to crash. (961745)</li>
<li>Editor: Fixed vsync not always off in scene view on macOS. (1009687)</li>
<li>Editor: Fixed skinned mesh not being removed on undo. (925835)</li>
<li>Editor: Fixed input field staying highlighted after Enter key was pressed. (998785)</li>
<li>Editor: Fixed errors related to temp TLS allocations. (926833 (921915)</li>
<li>Editor: Fixed various UnityEditor.VersionControl.Provider APIs when used with newly created VersionControl.Assets. (905161)</li>
<li>Editor: Fixed early flipping of login page in Mac by increasing the timeout. (980070)</li>
<li>Editor: Fixed an issue where multiple precompiled test assemblies with the same name would cause an error. (997902)(995476)</li>
<li>Editor: Fixed a Windows-specific crash in YAMLMerge when trying to merge files. (1001449)</li>
<li>Editor: Fixed the issue where dragging the slider was producing multiple undo steps. (998785)</li>
<li>Editor: Fixed various performance issues in YAMLMerge. (1001460)</li>
<li>FMOD: Fixed a performance regression in FMOD. (None)</li>
<li>GI: Fixed realtime probes going black when unloading a scene that was a part of a multi-scene bake. (996127)</li>
<li>GI: Fixed brighter baked or real-time lightmaps compared to 2017.1 when using emissive materials. (986160)</li>
<li>GI: Fixed duplicate GI light probe data in the player build with scenes that were part of a multi-scene bake. (971907)</li>
<li>GI: Fixed an issue where LoadDataTimeSliced works on the wrong scene mapping in the Editor. (1000692)</li>
<li>GI: Fixed realtime probes not working when loading scenes (that were baked together) additively. (957736)</li>
<li>GI: Fixed the "m_ProbeSetHashes.empty()" error occuring in certain projects when clearing the GI cache or when quitting the standalone. (949117)</li>
<li>GI: Fixed harmless "Lighting data asset [...] is inconsistent" errors when moving those assets between projects. (990626)</li>
<li>GI: Fixed errors on loading Enlighten probesets in the Editor after clearing the GI cache. (980811)</li>
<li>GI: Fixed an issue where baking multiple scenes together resulted in a LightingData.asset file vastly bigger than the sum of the sizes of the assets being baked in scenes. (913869)</li>
<li>Graphics: Fixed a potential crash when using marquee selection in the Editor, to select dynamic geometry such as particles, lines and trails. (1021655)</li>
<li>Graphics: Fixed Android/OpenGLES Cubemap native texture not being registered correctly causing cubemap CopyTexture to native texture to fail. This also fixed Oculus Cubemap overlays not rendering. (1014884)</li>
<li>Graphics: Fixed OpenGL ES crash due to problem with cached VertexAttribArray. (989484)</li>
<li>Graphics: Fixed black screen on devices that do not support RGBA16F rendering to texture. (989654)</li>
<li>Home: Fixed multiple issues with styling to enable windows scaling. (None)</li>
<li>Home: Fixed the launcher manage license page not handling losing of the network properly. (None)</li>
<li>IL2CPP: Added Windows runtime storage extensions. (992138)</li>
<li>IL2CPP: Improved the startup performance of Unity players built with IL2CPP. (989476)</li>
<li>IL2CPP: Reduced Android build size. (None)</li>
<li>IL2CPP: Handle method parameter attributes for methods on generic types. (999803)</li>
<li>IL2CPP: Corrected a possible build failure with IL2CPP when an attribute constructor has two arguments of type object. (993422)</li>
<li>Inspector Functionality: Fixed objects using HideAndDontSave being visible in preview windows, after being disabled and enabled. (963576)</li>
<li>iOS: Fixed crashes on some iOS devices due to unbound textures when using Metal API. (1002408)</li>
<li>iOS: Fixed standard shader specular highlights on mobiles. (None)</li>
<li>iOS: Added support for iPhone X second stage splash screen. (972995)</li>
<li>iOS: Fixed ReadPixels() crash on Metal when reading out of bounds of current active render texture. (990594)(981074)</li>
<li>iOS: Fixed Display.SetResolution not working during the first frame. (1003879)(995079)</li>
<li>iOS: Fixed crash when creating texture from PNG image when cardboard VR is enabled. (1016615 (1013198)</li>
<li>iOS: Fixed an audio crash when moving an app to the background, and back to the foreground. (967197)</li>
<li>iOS: Metal: Fixed MSAA behavior when using RenderPass. (N/A)</li>
<li>iPhone X: Fixed navigating to home pressing buttons located at the bottom of the screen. (973437)</li>
<li>Linux: Fixed Linux touch input for mouse events. (947049)</li>
<li>Mobile: Fixed crash in SplatMaterials::FindMaterialProperties when opening a scene with a certain Terrain and Material combination. (919769)</li>
<li>Mono: Fixed random error when using UDPClient. (990979)</li>
<li>Multiplayer: Fixed server active disconnect client for web sockets. (N/A)</li>
<li>Multiplayer: Fixed editor crashing on AddWebsocketHost on second instance using the same port. (1008385)</li>
<li>OSX: Fixed crash in UnitcodeInputView during editor shutdown. (946958)</li>
<li>Package Manager: Fixed project stored on OneDrive causing Package Manager error and preventing a project from being opened. (841172)</li>
<li>Package Manager: Fixed building as the local system user failing on Windows. (960093)</li>
<li>Particles: Fixed alpha output not being clamped to ensure compatibility with HDR. (967476)</li>
<li>Particles: Fixed crash when emitting particles from script. (988854)</li>
<li>Particles: Fixed error when sorting by youngest/oldest. (988874)</li>
<li>Particles: Fix edperformance regressions when emitting from script with a Size module enabled. (983677)</li>
<li>Particles: Fixed Prefab modifications allowed to be added multiple times. (989631)</li>
<li>Particles: Fixed Rate over Distance emission in Edit Mode. (1009717 (967752)</li>
<li>Physics: Ensured that a Kinematic Rigidbody2D created in script stays in a relative position to any parent Rigidbody2D when reparented. (983374)</li>
<li>Physics: Fixed disabling and enabling a collider on an inactive gameobject producing transform error messages. (985757)(968882)</li>
<li>Physics: Ensured that recursive 2D physics callbacks do not causes a crash when reparenting/disabling with existing contacts. (1006679)</li>
<li>Scripting: Fixed incorrect value when using Math.Round with MidpointRounding.AwayFromZero. (993302)</li>
<li>Scripting: Fixed exception when binding delegate with Enum value to method with int parameter. (977917)</li>
<li>Scripting: Fixed crash when using named pipes. (929984)</li>
<li>Services: Fixed exception when building in Cloud Build with Performance Reporting enabled. (996951)</li>
<li>Shaders: Fixed an issue with the Shader Compiler which would result in GLSL based platforms not being able to compiler certain shaders. (919351)</li>
<li>Shaders: Fixed shader compiler crash when compiling specific D3D9 shaders. (968997)</li>
<li>Substance: Fixed a memory leak when using cloned ProceduralMaterials. (1005779)</li>
<li>Timeline: Fixed issues where copied Timeline tracks and clips could retain a link to the source asset, or end up being saved as part of the source asset. (979587) (991434)</li>
<li>UI: Fixed instances where Font.textureRebuilt would not be called even though the internal texture was regenerated. (988310)(939853)</li>
<li>UI: Fixed OnEndDrag not being called when dragging while the application loses focus. (995453)(937370)</li>
<li>UI: Fixed crash in profiler window when a linked Render Texture Camera is disabled. (984325)(966106)</li>
<li>Unity Connect: Fixed codeless IAP button missing its attached script when rebuilding the library. (None)</li>
<li>Universal Windows Platform: Fixed compiler warnings about inconsistent DLL linkage when using Windows 10 Fall Creators Update SDK. (None)</li>
<li>Universal Windows Platform: Fixed player getting stuck on a white screen when a fatal error (such as unable to load files or system doesn't meet minimum requirements) occurs during startup. (1010354)</li>
<li>Universal Windows Platform: Fixed a crash in .NET native compiler ("RHB0011: Internal error: 'pchTypeNameEnd[0] == L'&gt;"at'f:\dd\ndp\rh\src\tools\rhbind\makepdb.cpp:998") in certain scenarios involving plugins. (991154)</li>
<li>Universal Windows Platform: Fixed build failing on IL2CPP scripting backend if class library from Mono directory was copied into the project (like System.Data.dll). (997876)</li>
<li>Universal Windows Platform: Fixed Application.isMobilePlatform results to be consistent with SystemInfo.deviceType. Also update API docs for these APIs. (991466)</li>
<li>Universal Windows Platform: Fixed .NET native compiler crash when using List or List in a serializable class. (979741)</li>
<li>Universal Windows Platform: Fixed reference rewriter not fixing references for System.Net.Sockets.Socket when DLL where it's being referenced was compiled against .NET 3.5. (947209)</li>
<li>VR: Fixing crash involving VR Mock Device when using TrackedPoseDriver. (966990)</li>
<li>WebGL: Fixed not handling playBuffer exception when there is no audio output on Safari. (994913)(960863)</li>
<li>Windows: Fixed resolution dialog not showing monitor list and crashing on pressing 'Play' button on some weird monitor setups. (996015)</li>
<li>Windows: Fixed mouse events for non-primary display on Windows standalone player. (None)</li>
<li>Windows: Fixed assert when stopping and then immediately destroying DictationRecognizer. (986045)</li>
<li>Windows: Player executable is once again large address aware. (990939)</li>
<li>Windows: Fixed crash on startup in case screen width/height player preferences in registry got corrupted. (979198)</li>
<li>Windows: Fixed opening project in Editor causing Unity to terminate it without opening the new one. (1016692 (978204)</li>
<li>Xbox One: Updated Mono to support dynamic function calls on Xbox One. (938545)</li>
<li>XR: Fixed an issue with lights failing to completely illuminate scene geometry during stereo rendering. (965494)</li>
<li>XR: Update VR SDK not supported in Editor warning. (None)</li>
<li>XR: Fixed incorrect thread affinity setting on Gear VR. (None)</li>
<li>XR: Fixed stabilization plane not getting set correctly via the SetFocusPointForFrame() API, resulting in poor hologram stabilization and color separation on HoloLens. (995065)</li>
</ul>

#### Revision: 372229934efd
