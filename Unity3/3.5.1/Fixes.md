# Unity 3.5.1

https://unity3d.com/unity/whats-new/unity-3.5.1

## Fixes



*   Android: APK files created from Eclipse could sometimes not be read, causing the application to close immediately.
*   Android: If the Java classpath did not include the current directory ('.') the APK signing step would fail.
*   Audio: Fixed audio playback parameters being clamped incorrectly when too many audio sources are playing at the same time.
*   Editor: Fixed hang when building very large amounts of asset bundles.
*   Editor: Fixed static batching not working when loading level through Application.LoadLevel().
*   Editor: When entering play mode hide the 'default' quality settings as they are stripped for build.
*   Editor: Fixed out of memory crash while building when having many resources in resource folder.
*   Editor: Fixed rare crash when importing material with bumpmap shader but bumpmap texture was not assigned.
*   Editor: Fixed rare crash that could occur if user had changed gizmo icon on asset.
*   Editor: Fixed crash that would happen if you tried to get the asset path of the material passed to AssetPostprocessor.OnAssingMaterialModel.
*   Editor: Fixed bug where animation window would say an animation event has no receivers, when there are multiple MonoBehaviours.
*   Editor: Fixed bug where building a scene asset bundle would give incorrect error messages.
*   Editor: Fixed title of File saving dialog when building for NaCl (it incorrectly said "Unsupported Build Target").
*   Editor: Fixed editor freezing while debugging in some situations.
*   Editor: Fix for a situation where changing color in the gradient editor could change color of a previous edited colorfield. (OSX issue only)
*   Editor: Fixed shutting down the editor process when opening another or new project from within the editor. (Windows issue only)
*   Editor: Fixed crash when incorrect assembly is loaded in some rare scenarios.
*   Graphics: Fixed static batching adding extra polygons(meshes) because of extra(unused) materials on input meshes.
*   Graphics: Fixed projector culling so it only renders objects inside projector.
*   Graphics: Fixed shader compilation for shaders that used a lighting function needing view direction (e.g. BlinnPhong) and passed the 'dualforward' surface directive parameter.
*   Graphics: Removed warnings that can be safely ignored ("InsideCameraRender" and "VertexCompNone" warnings).
*   Graphics: Fixed lens flare rendering when deferred lighting with an image effect (with the ImageEffectOpaque attribute) was used and there was transparent geometry in the scene.
*   iOS: Fixed basic license splash screen issue when application is built with Xcode 4.3.x.
*   iOS: Fixed problem when logging to console via System.Console.Write\* or JS/Boo print() was throwing exception on iOS 5.1 non-development devices.
*   Memory management: Reduced fragmentation in the heap allocators.
*   Memory management: Fixed race condition in realloc.
*   Mobile: Fixed random crashes with skinned meshes (Cloth in call stack). Re-enabled cloth simulation.
*   Mobiles: Fixed skinning performance regression.
*   Mobiles: Fixed performance regression with GuiTexture on Adreno devices.
*   MonoDevelop: Fixed a case where opening a newly-added script from Unity wouldn't cause the script to get focus.
*   Native Client: Fixed loading JPEG files as textures using WWW class.
*   OS X and Windows: Fixed very rare crash in SSE mesh skinning code.
*   OS X: Fixed standalone crash bug, where it would crash immediately on startup when the "Restore Windows" requester would appear after a previous crash.
*   Profiler: Fixed an issue where the player might crash when 'Autoconnect Profiler' was selected.
*   Substance: fixed colors being shuffled in the editor during the build process if "Fastest" quality mode is selected.
*   Web Player: Prevent Internet Explorer from crashing when more than one tab is used.
*   Web Player: Prevent Firefox from hanging on exit.
*   Web Player: Fixed bug where editor built incorrect data for compressed meshes in the webplayer.
*   Web Player: Make input more responsive for 2.x content.
*   Web Player: Fixed crash when assetbundle download was canceled.
*   Web Player: Fixed BeginScrollView missing method exception in 3.4 content.
*   Windows: Fixed a crash when using SkinnedCloth and switching into fullscreen mode.
*   Fixed issue where AssetBundle.Unload(false) caused lots of error messages to be printed when calling Resources.UnloadUnusesAssets () or loading a level.
*   Fixed out of memory crash when loading a corrupted .prefab file.
*   Fixed memory manager race condition.
*   Realtime only lights only affect dynamic geometry. This is the same behaviour as 3.4. Once content is published with 3.5 the fixed renderloop is used.