# Unity 3.5.1
https://unity3d.com/unity/whats-new/unity-3.5.1

## Fixes

<ul>
<li>Android: APK files created from Eclipse could sometimes not be read, causing the application to close immediately.</li>
<li>Android: If the Java classpath did not include the current directory ('.') the APK signing step would fail.</li>
<li>Audio: Fixed audio playback parameters being clamped incorrectly when too many audio sources are playing at the same time.</li>
<li>Editor: Fixed hang when building very large amounts of asset bundles.</li>
<li>Editor: Fixed static batching not working when loading level through Application.LoadLevel().</li>
<li>Editor: When entering play mode hide the 'default' quality settings as they are stripped for build.</li>
<li>Editor: Fixed out of memory crash while building when having many resources in resource folder.</li>
<li>Editor: Fixed rare crash when importing material with bumpmap shader but bumpmap texture was not assigned.</li>
<li>Editor: Fixed rare crash that could occur if user had changed gizmo icon on asset.</li>
<li>Editor: Fixed crash that would happen if you tried to get the asset path of the material passed to AssetPostprocessor.OnAssingMaterialModel.</li>
<li>Editor: Fixed bug where animation window would say an animation event has no receivers, when there are multiple MonoBehaviours.</li>
<li>Editor: Fixed bug where building a scene asset bundle would give incorrect error messages.</li>
<li>Editor: Fixed title of File saving dialog when building for NaCl (it incorrectly said "Unsupported Build Target").</li>
<li>Editor: Fixed editor freezing while debugging in some situations.</li>
<li>Editor: Fix for a situation where changing color in the gradient editor could change color of a previous edited colorfield. (OSX issue only)</li>
<li>Editor: Fixed shutting down the editor process when opening another or new project from within the editor. (Windows issue only)</li>
<li>Editor: Fixed crash when incorrect assembly is loaded in some rare scenarios.</li>
<li>Graphics: Fixed static batching adding extra polygons(meshes) because of extra(unused) materials on input meshes.</li>
<li>Graphics: Fixed projector culling so it only renders objects inside projector.</li>
<li>Graphics: Fixed shader compilation for shaders that used a lighting function needing view direction (e.g. BlinnPhong) and passed the 'dualforward' surface directive parameter.</li>
<li>Graphics: Removed warnings that can be safely ignored ("InsideCameraRender" and "VertexCompNone" warnings).</li>
<li>Graphics: Fixed lens flare rendering when deferred lighting with an image effect (with the ImageEffectOpaque attribute) was used and there was transparent geometry in the scene.</li>
<li>iOS: Fixed basic license splash screen issue when application is built with Xcode 4.3.x.</li>
<li>iOS: Fixed problem when logging to console via System.Console.Write* or JS/Boo print() was throwing exception on iOS 5.1 non-development devices.</li>
<li>Memory management: Reduced fragmentation in the heap allocators.</li>
<li>Memory management: Fixed race condition in realloc.</li>
<li>Mobile: Fixed random crashes with skinned meshes (Cloth in call stack). Re-enabled cloth simulation.</li>
<li>Mobiles: Fixed skinning performance regression.</li>
<li>Mobiles: Fixed performance regression with GuiTexture on Adreno devices.</li>
<li>MonoDevelop: Fixed a case where opening a newly-added script from Unity wouldn't cause the script to get focus.</li>
<li>Native Client: Fixed loading JPEG files as textures using WWW class.</li>
<li>OS X and Windows: Fixed very rare crash in SSE mesh skinning code.</li>
<li>OS X: Fixed standalone crash bug, where it would crash immediately on startup when the "Restore Windows" requester would appear after a previous crash.</li>
<li>Profiler: Fixed an issue where the player might crash when 'Autoconnect Profiler' was selected.</li>
<li>Substance: fixed colors being shuffled in the editor during the build process if "Fastest" quality mode is selected.</li>
<li>Web Player: Prevent Internet Explorer from crashing when more than one tab is used.</li>
<li>Web Player: Prevent Firefox from hanging on exit.</li>
<li>Web Player: Fixed bug where editor built incorrect data for compressed meshes in the webplayer.</li>
<li>Web Player: Make input more responsive for 2.x content.</li>
<li>Web Player: Fixed crash when assetbundle download was canceled.</li>
<li>Web Player: Fixed BeginScrollView missing method exception in 3.4 content.</li>
<li>Windows: Fixed a crash when using SkinnedCloth and switching into fullscreen mode.</li>
<li>Fixed issue where AssetBundle.Unload(false) caused lots of error messages to be printed when calling Resources.UnloadUnusesAssets () or loading a level.</li>
<li>Fixed out of memory crash when loading a corrupted .prefab file.</li>
<li>Fixed memory manager race condition.</li>
<li>Realtime only lights only affect dynamic geometry. This is the same behaviour as 3.4. Once content is published with 3.5 the fixed renderloop is used.</li>
</ul>
