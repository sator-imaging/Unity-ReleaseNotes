# Unity 4.0

https://unity3d.com/unity/whats-new/unity-4.0

## Fixes

- [](#)
- [](#)


*   Android: Added exception checking / propagation for script-based JNI Calls (AndroidJava\* / AndroidJNI\*).
*   Android: Loading a lot of assets through Resources.Load() could create a memory-leak-like behavior - this has been fixed.
*   Android: Fixed a rare case where libmono.so / libunity.so would not load due to "unable to link library".
*   Android: Cases with extremely slow loading times, when re-reading scene assets, has been fixed.
*   Android: The automatic binary splitting (for APK Expansion (.obb) support) was incorrectly omitting some files when using the Windows editor.
*   Android: Korean fonts were not rendered correctly on some Android devices.
*   Android: PlayerPrefs values queried with the wrong type would cause Java exceptions and application termination.
*   Android: Added additional registry entries to search when looking for the JDK installation on Windows.
*   Android: Requested RGBX32 instead of transparent when 32bit display buffer is selected.
*   Android: Workaround for mali and ics resulting in crash with shader that sample texture in vertex program.
*   Android: Crash when pausing/resuming on OS 4.1 / Jellybean has been fixed.
*   Android: If system environment variable JAVA\_TOOLS\_OPTIONS was set it could prevent the .apk to be signed.
*   Android: Webcam Texture now works on LG Optimus 3D (with OS 2.2 / Froyo).
*   Android: Portrait upside down orientation caused errors when building the .apk.
*   Android: EGL context recreation is fully supported (when pausing/resuming, or changing DisplayBuffer bit-depth, or anti-aliasing).
*   Android: Enforce that System.Net.Sockets use is only allowed with an Android Pro license.
*   Android: Added workaround for ARM Mali-400 GL ES 1.1 drivers sometimes referencing disabled vertex attrs (caused a crash).
*   Android: Script debugging yields/coroutines could sometimes cause a crash - this has been fixed.
*   Android: Application.streamingAssetsPath was incorrectly adding a slash before the jar delimiter (/!).
*   Android: Fixed failing to build signed APKs on Windows.
*   Android: Webcam resolution and frame rate selection is now more accurate.
*   Android: Webcam now works on Ice Cream Sandwich and JellyBean devices.
*   Android: Webcam now works on Motorola and OMAP devices.
*   Android: Microphone resources are now properly released when pausing the application.
*   Android: Audio should now play without any clicking noise on Kindle and Nook, although latency is still pretty bad.
*   Android: It should now be possible to play and record audio at the same time.
*   Android: Gyro.attitude did not compensate for screen orientation, nor device natural orientation (phone/tablet) - this has been fixed.
*   Android: Restarting an application right after calling Application.Quit() could cause a race condition between quitting the old and starting the new process.
*   Android: Input.multiTouchEnabled was returning false before the screen received an initial touch.
*   Android: Changed some tags in the AndroidManifest to have required="false".
*   Android: Fixed a problem where non-development ('release') builds would fail to load on devices with kernel 3.4 and later.
*   Android: Autorotation with only either portrait or landscape modes is now enforced by the manifest as well.
*   Android: Back button will quit the application while the first level has not yet been loaded.
*   Android: Renamed GameView resolutions to HVGA, WVGA, ..., and added WXGA (1280x800).
*   Android: Runtime class Ping now works.
*   Android: Added PowerVR performance stats to the internal profiler.
*   Android: Fixed a problem where multiple screen touches would lead to incorrect touch phases (especially during low framerate situations).
*   Android: The detection zone for screen touches resulting in increased tap count has been made resolution independent.
*   Android: Kindle Fire incorrectly reported having a camera.
*   Android: Fixed startup rotation when device is held in landscapeRight.
*   Android: Fixed an issue where the device might go to sleep before any script code was invoked.
*   Android: Added a wake lock to fullscreen video to make sure the device doesn't go to sleep during video playback.
*   Android: Fixed auto-rotation problem in landscape/reversed landscape on Kindle Fire HD.
*   Android/iOS: Incorrect mouse hover events stemming from screen touches has been fixed.
*   Android: Fixed an optimization error which could cause javac to crash/fail when loading UnityPlayer class.
*   Android: SystemInfo.deviceUniqueIdentifier is anonymized by calculating the MD5 sum of IMEI/MEID, ANDROID\_ID or WiFi MAC - whichever is available.
*   Android: SystemInfo.deviceUniqueIdentifier didn't automatically add the right permissions in the manifest.
*   Android: Switched to Bouncycastle for keystore certificate creation.
*   Android: On pre-Gingerbread devices 16bit DisplayBuffer is no longer enforced (and fallback from 32bits to 16bits buffer is handled gracefully). Worked around compositor issue with DisplayBuffer alpha on pre-Honeycomb devices.
*   Android: Made sure Ping cannot hang (times out after 5s).
*   Android: Added JB (4.1) to the list of SDK APIs.
*   Android: Fixed crash on Kindle when quitting without ever pausing.
*   Android: Changing system time/date while application was running would cause an ANR.
*   Android: Fixed camera initialization on platforms without FPS range support.

*   Animation: Exposed ModelImporter.generateAnimations as a bool, to allow control of over imported animation from an asset file.
*   Animation: Fixed a bug where animation wouldn't play if it's out of frustum and cullingType is switched to AlwaysAnimate in runtime.
*   Audio: Fixed problems playing back audio files whose paths contain special characters.
*   Audio: Fixed problems displaying audio files whose paths contain special characters in the inspector.
*   Audio: Fixed reverb filter diffuse slider inconsistency.
*   Audio: Fixed looping issue on tracked music files.
*   Audio: Fixed length determination for tracked music files.
*   Audio: Fixed m\_IgnoreListenerVolume property (was not working in the expected way).
*   Audio: Fixed the length property of an AudioClip to be more accurate in the case of MP3s.
*   Audio/video: Gracefully handle importing corrupt OGG container assets.
*   Audio: Fixed crashes when using audio clips with read callbacks.
*   Audio: Various fixes related to handling of special characters.
*   Audio: Fixed incorrect display of waveform preview.
*   Audio: Fixed rare deadlocks.
*   Audio: Hardened AudioClip SetData and GetData to when the array argument is longer than the clip itself.
*   Asset Import: Default assets generated for failed imports are now persisted correctly.
*   AssetStore: Fixed out of memory crash when downloading large packages.
*   Bugreporter: Fixed the issue that log files would not be shown in bug reporter window, even though they existed.
*   Cache Server: Fixed connection problem when downloading assets.
*   Cache Server: Fixed other connection issues.
*   Debugger: Fixed hangs/deadlocks when debugging multithreaded script code.
*   Debugger: Fixed crash on debug-time evaluation of generic methods.
*   Documentation: Fixed script reference History page to reflect reality again.
*   Editor: Fixed crash when calling Close in the OnFocus callback.
*   Editor: Fixed object selector not working for ObjectFields in GUI.Window.
*   Editor: Fixed some vertically misaligned buttons in the dark skin.
*   Editor: Fixed EditorExtensionImpl showing up in the Project view in some projects imported from 3.4.
*   Editor: Will now use project name instead of the build file name as the title for published web players.
*   Editor: Scenes in Build Settings no longer get reordered alphabetically.
*   Editor: Undo now working if movement is cancelled by right click.
*   Editor: Fixed error message when resizing arrays.
*   Editor: Fixed crash when changing asset serialization to text mode.
*   Editor: Fixed hang when play mode is exited while a download is in progress.
*   Editor: Fixed crash when selecting multiple ScriptableObjects of different types.
*   Editor: Scene view uses the same rendering path as main camera. Much less confusion!
*   Editor: Soft particles usage hint in Quality Settings UI.
*   Editor: Screen.width and Screen.height much more consistently report actual game view size when used outside of editor window GUI code.
*   Editor: Made default values for sphere & capsule colliders use 0,0,0 for the center (it previously was not precisely zero due to floating point inaccuracies).
*   Editor: Made the TextMesh inspector automatically change the material of the MeshRenderer when the font is changed.
*   Editor: Properly reset MovieTextures when entering play mode.
*   Editor: Fixed crash if importing an AudioClip fails during project re-import.
*   Editor: Fixed null ref when using "Open" button in the inspector for model files in some cases.
*   Editor: Fixed errors about not being allowed to access targets array.
*   Editor: Fixed profiler using deep profiling when exceptions occur.
*   Editor: Fixed DnD references being empty during DragExited after a DragPerform.
*   Editor: Update visible rect when horizontal scrollbar is needed because vertical scrollbar is used.
*   Editor: Clamping of the scroll position to account for the visible rect of the scrollview.
*   Editor: Fixed scrollview returning scroll position out of view rect size when using scrollwheel.
*   Editor: Correctly handle when null string is passed to a TextField.
*   Editor: Don't show Display Resolution Dialog when using CTRL-B from the editor and it's turned off.
*   Editor: Fixed EditorWindow.ShowPopup with initial position of 0, 0 not rendering correctly.
*   Editor: Fixed missing bold font in some inspectors (e.g. FBXImporter).
*   Editor: GizmoType.NotSelected attribute for DrawGizmo works correctly.
*   Editor: Component menu now handles custom namespaces.
*   Editor: Light probes are selectable in search mode.
*   Editor: Excess flood of Animation clips is not confusing the model importer inspector.
*   Editor: EnumMaskField returns consistent value when every item is selected.
*   Editor: Textfield word wrapping fixes.
*   Editor: Display names of colliding enumeration values in inspector
*   Editor: Fixed problem with the Asset Store window on retina display Macbook Pros.
*   Editor: Fixed hang while closing if plugins had created their own native threads.
*   Editor: Fixed odd drawing behavior when attempting to resize welcome screen.
*   Editor: GUI.color is reset properly for every CustomEditor
*   Editor: Fixed profiler causing an Out of Memory error in the console.
*   Editor: Improved error reporting when exporting a Unity package.
*   Editor: Fixed a bug where ARGB16 textures loaded from AssetBundles built for iOS/Android would load incorrectly.
*   Editor: Editor doesn't hang anymore if exiting while in play mode.
*   Editor: Made entering playmode faster by reducing the number of domain reloads.
*   Editor: Fixed null reference exception when a MonoBehaviour is missing in the inspector. Instead we display helpful warnings embedded in the inspector.
*   Editor: Fixed issue in fbx importer where prefab instance modifications would in some corner cases get applied to a different object on a different machine
*   Editor: Fixed bug where calling LoadLevel in OnDestroy when exiting playmode could lead to a crash.
*   Editor: Fixed bug where the import settings were not updated when a .meta file is changed.
*   Editor: Fixed various leaks in the asset import pipeline when importing large project folders.
*   Editor: Fixed prefab override recording issue where modifications would not get applied to array elements if the prefab array is empty and the size value was overridden after the property was overridden.
*   Editor: Fixed warning when changing import settings on a lot of fbx files.
*   Editor: Fixed crashbug when clicking on Apply prefab button in the game object inspector when the prefab would add / remove components on awake in edit mode.
*   Editor: Fixed drag and drop behaviour when dragging child prefab objects.
*   Editor: Improvements to Light Probe editing: don't change selection when duplicating them; render editable ones on top of baked ones.
*   Editor: Wireframe and Textured Wireframe scene view modes take actual vertex & tessellation shaders into account now.
*   Editor: Fixed import of .EXR files with alpha channel.
*   Editor: Invoked OnFocus/OnLostFocus when switching tabs within the same DockArea.
*   Editor: Disallowed hiding cursor when GameView is out of focus.
*   Editor: Fixed crash caused by scene view overlays.
*   Editor: Fixed box collider handles not matching box collider gizmos.
*   Editor: Text fields support OS standard behavior of Command + Backspace deleting everything from the start of the current line to the cursor position.
*   Editor: Cleaned up LOD group inspector (button alignment, text clipping).
*   Editor: Make Unity 1.x GUI components never be shown in the Scene View.
*   Editor: Changed order of calculations during model import to improve normal calculation.
*   Editor: EditorUtility.CopySerialized now works correctly for components.
*   Editor: Fixed a bug where generated OS X icons would occasionally get corrupted.
*   Editor: Fixed a bug where the editor would fail to open projects if the root Assets folder has a .meta file.
*   Editor: Fixed delay when bringing up shader selection menu for the first time (4.0: fixed delay when bringing it up each time).
*   Editor: Fixed potential crash when editing multiple objects and resizing arrays.
*   Editor: Fixed Rendering Paths scene view mode to take camera's render path into account, not only what the shaders are capable of.
*   Editor: Fixed WebPlayer building code; now it does not try to recreate the outermost directory (a user might not have sufficient filesystem access rights anyway).
*   Editor: Allow for cmd+c and ctrl+c to be used on a SelectableLabel.
*   Editor: Do not show cut/paste context menu action for SelectableLabel
*   Editor: Popup windows no longer flicker for a frame on OSX.
*   Editor: Audio preview in Scene View now works correctly without any Audio Listeners in the scene.
*   Editor: Fix some importer inspectors constantly repainting.
*   Editor: Fix key navigation to assets store groups while showing local assets.
*   Editor: Fixed windows standalone icons alpha issues.

*   Flash: Replace no longer ignores parens.
*   Flash: Several code conversion issues resolved.
*   Flash: NavmeshPath can now be instantiated correctly.
*   Flash: Fixed translation of some shaders (e.g. Refractive Glass was causing errors).
*   Flash: Made AsyncOperation work.
*   Flash: Fixed division by long and ulong.
*   Flash: Fixed bug where assigning a struct to an object or interface would introduce two pointers to the same struct instead of two copies.
*   Flash: Fixed several cornercase bugs in support for generics.
*   Flash: Properly initialize fields of type DateTime in structs instantiated with default constructor.
*   Flash: Fixed memory corruption crash if WWW response .Length didn't match actual length of payload.
*   Flash: Support ++ and -- on arguments that are passed byref, whose result is assigned to an array.
*   Flash: Fixed mouse visibility bug.
*   Flash : Fixed equality comparison for ValueTypes.
*   Flash : Fixed hashtable comparison.
*   Flash : Fixed enum comparison
*   Flash : Fixed enum to enum cast.
*   Flash : Fixed keyboard input handling and TextArea input (control, delete, space, arrow keys).
*   Flash : Generic collections now work with interfaces.
*   Flash : Fixed crash when www.audioclip was used in a coroutine.
*   Flash : SweepTestAll now works.
*   Flash : UnityEngine.Flash.FlashPlayer allows retrieval of target player and swf version.
*   Flash: Fixed rare condition in which we ran out of stack space, resulting in an out of range error.
*   Flash: Fixed issues with anonymous delegates.
*   Flash: Implemented delegate comparison.
*   Flash: Implemented Double.TryParse.
*   Flash: Input.inputString now works.
*   Flash: No more compiler crashes on incorrect SWF dimensions.
*   Flash: Key repeat works.
*   Flash: Fixed NewInstance for Enum value types
*   Flash: Fixed getter/setter generation for System.Array.
*   Flash: Don't show Development Build watermark in non-dev builds.
*   Flash: Fixed issues with anonymous delegates.
*   Flash : Fix string marshalling. Now consistently UTF8.
*   Flash : Fix dynamic font textures generated larger then Flash max texture size (2048\*2048).
*   Flash : Fix dynamic font generation trashing memory.
*   Flash : Fix invalid agal generated for cube map samplers.
*   Flash : Fix backbuffer being cleared because of rtt.
*   Flash : Fix type inference for float division.
*   Flash : Fix issue with loitering objects in finalizermaps.
*   Flash : Fix issue with converted GetHashCode code being invalid when generated from a MS compiler.
*   Flash : Implemented Char.ConvertFromUtf32
*   Flash : Improved support for System.Convert
*   Flash : Adding support for TryParse for additional data types.
*   Font rendering: Fixed position of text cursor when a custom font size is used for the TextField.
*   Font rendering: Fixed kerning.
*   Graphics: Fixed crashes that sometimes occurred on OpenGL with mismatched GL.Begin/GL.End pairs.
*   Graphics: Fixed TrailRenderer culling issue.
*   Graphics: Don't break batching based on shadow distance when there aren't any shadow casting lights.
*   Graphics: Properly take line width into account when adding points to LineRenderer.
*   Graphics: SubShader tags (render queue etc.) take shader LOD into account properly now.
*   Graphics: Free up temporary memory used by non-uniformly scaled mesh when deactivating a mesh renderer.
*   Graphics: Static batching performs better when there are multiple lightmaps in the scene (before it could run into cases where it wasn't batching much).
*   Graphics: Fixed memory leak in Material.CopyPropertiesFromMaterial.
*   Graphics: Fixed a rare "invalid angle: inf" error message with terrain and shadows.
*   Graphics: Fixed Camera pixelWidth/pixelHeight/aspect queries done from Editor code being really confusing. Before, it was using the size of last drawn editor view for the calculations. Now, for regular cameras, Game View size is used.
*   Graphics: Fixed crash in Shuriken mesh particles, when source mesh has no normals or tangents.
*   Graphics: Fixed errors with statically batched meshes that are later modified by a script.
*   Graphics: Fixed issue with Deferred rendering and wireframe Scene View mode.
*   Graphics: Fixed various issues with shaders in asset bundles. E.g. you can actually put terrain with trees into an asset bundle, and the billboard shaders will work, without having to jump through various hoops.
*   Graphics: Properly include all shaders into game data files when editor is in "-nographics" mode.
*   Graphics: Batched Shuriken draw calls were not accounted for in the game view stats window.
*   Graphics: Don't load Occlusion Culling data in non-Pro editor licenses.
*   Graphics: Fixed console error messages when a terrain tree prefab is missing.
*   Graphics: Smoother framerate on Windows when using vsync.
*   Graphics: Fixed Screen.resolutions reporting zero for refresh rate in some cases.
*   Graphics: Fixed crash when using additive scene loading with missing lightmaps.
*   Graphics: Fixed small memory leak when loading shaders with syntax errors; made shader loading a bit faster as a byproduct ;)
*   Graphics: Fixed error messages in some situations when calling camera.Render from editor scripts.
*   Graphics: Fixed surface shader finalcolor modifier sometimes producing wrong results.
*   Graphics: Limit maximum texture size to 4096 on Retina MacBookPros due to OS X driver bugs.
*   Graphics: Removed limitation that Windows Standalone game window can't reach whole desktop screen size.
*   Graphics: On Linux, fixed lower resolution blit texture getting broken due to quality settings change.
*   Graphics: Improved deferred lighting depth buffer sharing workaround for some OpenGL systems. Mostly, much faster now on some Linux GPUs/drivers.
*   Graphics: Fixed different mesh compression setting to actually make a difference (previously it would always use "Low" compression, regardless of setting).
*   Graphics: Fixed some issues with Fog on Direct3D 9; in rare cases with some complex shaders it was not working properly.
*   Graphics: Fixed HDR rendering being off in the very first frame.
*   Graphics: Fixed Camera.hdr returning wrong value when called before render.
*   Graphics: Fixed occasional errors being reported when rendering objects with zero scale.
*   IMGUI: Fix BeginHorizontal not displaying content/tooltip when using GUIStyle.none.
*   Image Effects: Fixed Flash-related warning messages when importing Image Effects package.
*   Image Effects: Fixed Global Fog on Windows when MSAA is used.
*   Input: Fixed OnMouseDown and related callbacks being wrongly sent to cameras that render into RenderTextures.
*   Input: Gamepad buttons are now correctly initialized again.
*   iOS: Fixed Xcode crash when native plugin uses "+" in the name.
*   iOS: Fixed iPad splash handling when starting in portrait.
*   iOS: Made various orientation fixes.
*   iOS: Corrected texture atlas padding.
*   iOS: Fixed skinning corrupting UVs.
*   iOS: Fixed crash on suspending app while playing video.
*   iOS: Fixed recognition of more recent iPhone4/4S models.
*   iOS: Fixed various crashes when Script Call Optimization set to "fast but no exceptions".
*   iOS: Fixed text-area behavior when on-screen keyboard is hidden.
*   iOS: Fixed Screen.orientation on the first frame on iOS6.
*   iOS: Fixed interoperability of DisplayLink mode and iOS native UI.
*   iOS: Fixed iOS splash screen image not being released after game starts.
*   iOS: Fixed www.uploadProgress support.
*   iOS: Fixed loading indicator position.
*   iOS: Small GPU profiling (in the internal iPhone profiler) improvement.
*   iOS: Fixed basic license splash screen issue with Xcode 4.5.
*   iOS: Fixed support for native methods inside of inner classes.
*   iOS: More fixes to initial orientation handling.
*   iOS: Unity Remote support updated to work better with input compensation for screen orientation.
*   iOS: Fixed Screen.dpi for iPad Mini.
*   Javascript: Fixed error checking for array indices.
*   Javascript: Fixed regression on 'not in' operator. Operator has been brought back.
*   Javascript: Introduced 'for each' syntax for better compatibility with other javascript dialects.
*   Lightmapping: Fixed "Generate Lightmap UVs" difference between Windows & Mac!
*   Lightmapping: Fixed handling degenerate triangles in UV space, Beast no longer spits out "TexBakeSampleGenerator: Non-invertible matrix".
*   Lightmapping: Skipping tree instances that reference a prototype without a mesh.
*   Lightmapping: Improved error messages when failing to bake Light Probes; when meshes have UVs outside 0..1 range, when meshes have missing UVs.
*   Lightmapping: Take texture tiling into account for materials with cutout shaders.
*   Lightmapping: Fixed issues with some emissive materials.
*   Lightmapping: Fix harmless error when lightmap baking an unsaved scene on Mac.
*   LOD: Fix double GUI repaint error when caused by reparent renderers dialog.
*   Mobile: Better RenderTexture.DiscardContents implementation.
*   Mobile: Fixed wrong lighting when dynamically batching uniformly scaled meshes.
*   Mac OS X Editor: Fixed window focus issues when using a multiple screen setup in OS X 10.8 Mountain Lion.
*   Mac OS X: Event.clickCount behavior for double-clicks now matches windows (clickCount is always 1 for MouseUp events).
*   Mac OS X: Don't freeze Unity content when the System clock is changed while running.
*   Mac OS X: PlayerPrefs keys will now work if they contain an '@' character.
*   Mac OS X: Fix Webcam textures with non-native resolutions correctly picking up the desired texture size.
*   Mac OS X: Fixed some graphics issues on dual-GPU Mac models, e.g. editor windows occasionally becoming all white.
*   Mac OS X: Fixed Crash on quit if profiling had been enabled.
*   Mac OS X Standalone: Fixed problems when writing OS X icon format, leading to broken icon graphics in some cases.
*   Mac OS X Standalone: Used OS X Lion style fullscreen mode, to allow other windows to show up in front of fullscreen apps, and to allow switching in and out of fullscreen mode by clicking onto the fullscreen button in the window title bar (optional).
*   Mac OS X Standalone: Fix hiding of window when GameCenter is activated.
*   Mac OS X Standalone: Changed event processing to allow other windows to receive keyboard events, to allow better integration with OS services such as GameCenter using plugins.
*   Mac OS X Web Player: Made IME support work in all Mac browsers.
*   Mac OS X Web Player: Fixed focus handling when the browser is switched to the background or the user switches to another window/tab.
*   Mac OS X Web Player: Fixed memory leak.
*   Mac OS X WebPlayer: Fixed OnApplicationPause being called when window goes to the background.
*   Math: Fixed Plane.SameSide equation side error.
*   Misc: Improve Time.smoothDeltaTime so it's not affected by pausing/unpausing.
*   Native Client: Fixed download of JPG files as textures.
*   Native Client:: Fixed problem where preferences might get lost when the player is closed while writing preferences to disk.
*   Native Client: Fixed deadlock when loading mono DLLs.
*   Native Client: Fixed Build & Run with Chrome 23.
*   NavMeshAgent : Fix crash querying nextOffMeshLinkData when having no navmesh in scene.
*   NavMeshAgent: Fixed bug where Resume breaks updateRotation setting.
*   NavMeshAgent: Path request processing queue order fixed.
*   Physics: Fixed problem where CCD would incorrectly detect collisions if the center or scale of a collider was changed.
*   Networking: Fixed case where a MasterServerEvent.HostListReceived was triggered for each host in a host list.
*   Networking: Fixed problem with connecting to password protected servers with NAT punchthrough.
*   Player: Fixed race condition in WWW class that could cause a crash when aborting download.
*   Physics: Fixed MeshCollider not working if it had been scaled to be zero sized, and then scaled up again.
*   Physics: Fixed a bug where Raycasts against CapsuleColliders with a zero-length middle section would not always return correct results.
*   Physics: Fixed a bug where destroyed colliders would not be properly deallocated if Time.timeScale was zero.
*   Physics: Fixed colliders being properly inactive when they are on inactive child game objects of the rigidbody.
*   Physics: Fixed collision between two triggers to send OnTriggerEnter events to both triggers and both rigidbodies for consistent results.
*   Physics: Fixed memory leak when Time.timeScale is zero.
*   Physics: Fix problem with activation order when recursively activating hierarchies, causing rag dolls not to function properly in some cases.
*   Physics: Fixed a bug where rigidbody interpolation would have an effect on physics simulation results.
*   Physics cloth: Fixed tangents to match initial rotation of object.
*   Prefabs: Duplicating game objects with references to abstract classes behaves more reliable.
*   Profiler: Fixed hang on editor or player when connection could not keep up with the data.
*   Profiler: Made the profiler skip frames instead of freezing up if editor lacks behind player.
*   Profiler: GC memory was not propagated correctly up the call hierarchy.
*   ProfilerConnection: Fixed inifinite loop freeze if profiler sendbuffer is full on the player.
*   Scene View: Fix scene editor camera becoming locked out from user control.
*   Scripting: Added overloads to EditorGUI.IntSlider so it can take SerializedProperties.
*   Scripting: Fixed crash when calling material.GetFloat(null).
*   Scripting: Fixed crash when a component destroys itself while AddComponent is trying to create it.
*   Scripting: Fixed crash calling Resources.Load before resources have been imported.
*   Scripting: Fixed bug where AssetBundle.LoadFromFile would get unloaded by UnloadUnusedAssets.
*   Scripting: GameObject.Find will now correctly find children of objects of the same name as other objects which don't have children of that name.
*   Scripting: Fixed crash when a gameObject is being destroyed while calling SendMessage on it.
*   Scripting: Fixed script serialization bug where properties could not be #if-ed out for the player.
*   Serialization: For non-webplayer-targets, scenes (implicitly) referencing assets placed under the Resources folder will now always have the assets placed together with the scene (and not in the resources.assets).
*   Shaders: Fog shader variables (unity\_FogColor etc.) are set to produce no fog when it's off.
*   Shaders: round() and trunc() HLSL functions are now supported when compiling shaders for mobile.
*   Shaders: Updated HLSL-to-GLSL shader compilers; fixes some complex mobile shaders (e.g. Tree Creator ones, or Edge Detection image effect on some mobile GPUs).
*   Shaders: Fixed compile errors in some cases where custom directional lightmap lighting function is used.
*   Shadows: Fixed shadow caster culling when light direction is exactly parallel to one of camera's frustum planes.
*   Shuriken: Fixed particle system randomness. There should be a lot less visible correlation between parameters when using random between curves and values.
*   Shuriken: Can't remove disabled UI modules, gizmo scaling issue, simulation preview issues when scrubbing.
*   Shuriken: Fixed sub-emitter memory leaks, occasional crash.
*   Shuriken: Gracefully handle when mesh is invalid, instead of leaving the emitter in a bad state.
*   Shuriken: Fixed crash if using mesh particles without UVs.
*   Standard Assets: Projector uses smaller, but uncompressed textures; to avoid artifacts when looking from a distance.
*   Substances now handles iOS non-square unsupported PVRTC.
*   Substance: Fixed baking issues on unsupported platforms (Android, iOS, Flash).
*   Substance: Lower memory consumption in the Editor when importing projects and switching color space.
*   Substance: Fixed runtime re-generation of substances with bitmap inputs.
*   Substance: "Generate all outputs" now displays all generated textures in the Inspector.
*   Substance: Fixed cloning substances in the Inspector.
*   Substance: Fixed bitmap export.
*   Substance: Fixed several erroneous error messages appearing in the log.
*   Terrain: Fixed error messages when painting terrain grass with negative sizes, and when adding some tree models.
*   Terrain: Terrain renderer no longer causes invalid memory accesses during rendering traversal.
*   Time: Fixed timescale usage when single stepping.
*   UV generation is now more deterministic between platforms since it is performed prior to scaling of vertices.
*   UnityObject: The default templates works nicely over https now.
*   UnityObject: Running a offline build locally will not break the default templates.
*   WebCamTextures: Fixed error message when querying list of available devices while WebCams are in use.
*   Web Player: Application.dataPath will now work correctly if the player URLs has slash characters in the url parameters.
*   WebPlayer: Fixed the plugin ticking routine. It is simpler and less error prone.
*   WebPlayer: Updated the builtin resources; now there is a distinction between "Made with Unity 4 Beta" and "Unity 4 Beta" plugin.
*   WebPlayer: Fixed a variety of crashes when plugin was running on IE9.
*   Webplayer: Crash logs now contain stacktrace.
*   Webplayer: Fixed memory overwrite on startup when running in-process on Firefox.
*   WWW Class: Fixed parsing text encoding if the encoding http header contains more parameters.
*   Windows: Improved StackOverflowException handling in scripts.
*   Windows: Fixed issues with 64-bit player not launching when non-latin characters in path.
*   Windows Editor: Messages with "Failed: The operation has completed successfully" should not be presented anymore when operations on files fail.
*   Windows Editor: Fixed extracting .unitypackage files containing extended Unix file attributes.
*   Windows Editor: Asset Store window now works correctly in OpenGL mode.