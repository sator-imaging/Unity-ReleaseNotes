# Unity 4.0
https://unity3d.com/unity/whats-new/unity-4.0

## Fixes

<ul>
<li>Android: Added exception checking / propagation for script-based JNI Calls (AndroidJava* / AndroidJNI*).</li>
<li>Android: Loading a lot of assets through Resources.Load() could create a memory-leak-like behavior - this has been fixed.</li>
<li>Android: Fixed a rare case where libmono.so / libunity.so would not load due to "unable to link library".</li>
<li>Android: Cases with extremely slow loading times, when re-reading scene assets, has been fixed.</li>
<li>Android: The automatic binary splitting (for APK Expansion (.obb) support) was incorrectly omitting some files when using the Windows editor.</li>
<li>Android: Korean fonts were not rendered correctly on some Android devices.</li>
<li>Android: PlayerPrefs values queried with the wrong type would cause Java exceptions and application termination.</li>
<li>Android: Added additional registry entries to search when looking for the JDK installation on Windows.</li>
<li>Android: Requested RGBX32 instead of transparent when 32bit display buffer is selected.</li>
<li>Android: Workaround for mali and ics resulting in crash with shader that sample texture in vertex program.</li>
<li>Android: Crash when pausing/resuming on OS 4.1 / Jellybean has been fixed.</li>
<li>Android: If system environment variable JAVA_TOOLS_OPTIONS was set it could prevent the .apk to be signed.</li>
<li>Android: Webcam Texture now works on LG Optimus 3D (with OS 2.2 / Froyo).</li>
<li>Android: Portrait upside down orientation caused errors when building the .apk.</li>
<li>Android: EGL context recreation is fully supported (when pausing/resuming, or changing DisplayBuffer bit-depth, or anti-aliasing).</li>
<li>Android: Enforce that System.Net.Sockets use is only allowed with an Android Pro license.</li>
<li>Android: Added workaround for ARM Mali-400 GL ES 1.1 drivers sometimes referencing disabled vertex attrs (caused a crash).</li>
<li>Android: Script debugging yields/coroutines could sometimes cause a crash - this has been fixed.</li>
<li>Android: Application.streamingAssetsPath was incorrectly adding a slash before the jar delimiter (/!).</li>
<li>Android: Fixed failing to build signed APKs on Windows.</li>
<li>Android: Webcam resolution and frame rate selection is now more accurate.</li>
<li>Android: Webcam now works on Ice Cream Sandwich and JellyBean devices.</li>
<li>Android: Webcam now works on Motorola and OMAP devices.</li>
<li>Android: Microphone resources are now properly released when pausing the application.</li>
<li>Android: Audio should now play without any clicking noise on Kindle and Nook, although latency is still pretty bad.</li>
<li>Android: It should now be possible to play and record audio at the same time.</li>
<li>Android: Gyro.attitude did not compensate for screen orientation, nor device natural orientation (phone/tablet) - this has been fixed.</li>
<li>Android: Restarting an application right after calling Application.Quit() could cause a race condition between quitting the old and starting the new process.</li>
<li>Android: Input.multiTouchEnabled was returning false before the screen received an initial touch.</li>
<li>Android: Changed some tags in the AndroidManifest to have required="false".</li>
<li>Android: Fixed a problem where non-development ('release') builds would fail to load on devices with kernel 3.4 and later.</li>
<li>Android: Autorotation with only either portrait or landscape modes is now enforced by the manifest as well.</li>
<li>Android: Back button will quit the application while the first level has not yet been loaded.</li>
<li>Android: Renamed GameView resolutions to HVGA, WVGA, ..., and added WXGA (1280x800).</li>
<li>Android: Runtime class Ping now works.</li>
<li>Android: Added PowerVR performance stats to the internal profiler.</li>
<li>Android: Fixed a problem where multiple screen touches would lead to incorrect touch phases (especially during low framerate situations).</li>
<li>Android: The detection zone for screen touches resulting in increased tap count has been made resolution independent.</li>
<li>Android: Kindle Fire incorrectly reported having a camera.</li>
<li>Android: Fixed startup rotation when device is held in landscapeRight.</li>
<li>Android: Fixed an issue where the device might go to sleep before any script code was invoked.</li>
<li>Android: Added a wake lock to fullscreen video to make sure the device doesn't go to sleep during video playback.</li>
<li>Android: Fixed auto-rotation problem in landscape/reversed landscape on Kindle Fire HD.</li>
<li>Android/iOS: Incorrect mouse hover events stemming from screen touches has been fixed.</li>
<li>Android: Fixed an optimization error which could cause javac to crash/fail when loading UnityPlayer class.</li>
<li>Android: SystemInfo.deviceUniqueIdentifier is anonymized by calculating the MD5 sum of IMEI/MEID, ANDROID_ID or WiFi MAC - whichever is available.</li>
<li>Android: SystemInfo.deviceUniqueIdentifier didn't automatically add the right permissions in the manifest.</li>
<li>Android: Switched to Bouncycastle for keystore certificate creation.</li>
<li>Android: On pre-Gingerbread devices 16bit DisplayBuffer is no longer enforced (and fallback from 32bits to 16bits buffer is handled gracefully). Worked around compositor issue with DisplayBuffer alpha on pre-Honeycomb devices.</li>
<li>Android: Made sure Ping cannot hang (times out after 5s).</li>
<li>Android: Added JB (4.1) to the list of SDK APIs.</li>
<li>Android: Fixed crash on Kindle when quitting without ever pausing.</li>
<li>Android: Changing system time/date while application was running would cause an ANR.</li>
<li>Android: Fixed camera initialization on platforms without FPS range support.</li>
</ul>

###  
<ul>
<li>Animation: Exposed ModelImporter.generateAnimations as a bool, to allow control of over imported animation from an asset file.</li>
<li>Animation: Fixed a bug where animation wouldn't play if it's out of frustum and cullingType is switched to AlwaysAnimate in runtime.</li>
<li>Audio: Fixed problems playing back audio files whose paths contain special characters.</li>
<li>Audio: Fixed problems displaying audio files whose paths contain special characters in the inspector.</li>
<li>Audio: Fixed reverb filter diffuse slider inconsistency.</li>
<li>Audio: Fixed looping issue on tracked music files.</li>
<li>Audio: Fixed length determination for tracked music files.</li>
<li>Audio: Fixed m_IgnoreListenerVolume property (was not working in the expected way).</li>
<li>Audio: Fixed the length property of an AudioClip to be more accurate in the case of MP3s.</li>
<li>Audio/video: Gracefully handle importing corrupt OGG container assets.</li>
<li>Audio: Fixed crashes when using audio clips with read callbacks.</li>
<li>Audio: Various fixes related to handling of special characters.</li>
<li>Audio: Fixed incorrect display of waveform preview.</li>
<li>Audio: Fixed rare deadlocks.</li>
<li>Audio: Hardened AudioClip SetData and GetData to when the array argument is longer than the clip itself.</li>
<li>Asset Import: Default assets generated for failed imports are now persisted correctly.</li>
<li>AssetStore: Fixed out of memory crash when downloading large packages.</li>
<li>Bugreporter: Fixed the issue that log files would not be shown in bug reporter window, even though they existed.</li>
<li>Cache Server: Fixed connection problem when downloading assets.</li>
<li>Cache Server: Fixed other connection issues.</li>
<li>Debugger: Fixed hangs/deadlocks when debugging multithreaded script code.</li>
<li>Debugger: Fixed crash on debug-time evaluation of generic methods.</li>
<li>Documentation: Fixed script reference History page to reflect reality again.</li>
<li>Editor: Fixed crash when calling Close in the OnFocus callback.</li>
<li>Editor: Fixed object selector not working for ObjectFields in GUI.Window.</li>
<li>Editor: Fixed some vertically misaligned buttons in the dark skin.</li>
<li>Editor: Fixed EditorExtensionImpl showing up in the Project view in some projects imported from 3.4.</li>
<li>Editor: Will now use project name instead of the build file name as the title for published web players.</li>
<li>Editor: Scenes in Build Settings no longer get reordered alphabetically.</li>
<li>Editor: Undo now working if movement is cancelled by right click.</li>
<li>Editor: Fixed error message when resizing arrays.</li>
<li>Editor: Fixed crash when changing asset serialization to text mode.</li>
<li>Editor: Fixed hang when play mode is exited while a download is in progress.</li>
<li>Editor: Fixed crash when selecting multiple ScriptableObjects of different types.</li>
<li>Editor: Scene view uses the same rendering path as main camera. Much less confusion!</li>
<li>Editor: Soft particles usage hint in Quality Settings UI.</li>
<li>Editor: Screen.width and Screen.height much more consistently report actual game view size when used outside of editor window GUI code.</li>
<li>Editor: Made default values for sphere &amp; capsule colliders use 0,0,0 for the center (it previously was not precisely zero due to floating point inaccuracies).</li>
<li>Editor: Made the TextMesh inspector automatically change the material of the MeshRenderer when the font is changed.</li>
<li>Editor: Properly reset MovieTextures when entering play mode.</li>
<li>Editor: Fixed crash if importing an AudioClip fails during project re-import.</li>
<li>Editor: Fixed null ref when using "Open" button in the inspector for model files in some cases.</li>
<li>Editor: Fixed errors about not being allowed to access targets array.</li>
<li>Editor: Fixed profiler using deep profiling when exceptions occur.</li>
<li>Editor: Fixed DnD references being empty during DragExited after a DragPerform.</li>
<li>Editor: Update visible rect when horizontal scrollbar is needed because vertical scrollbar is used.</li>
<li>Editor: Clamping of the scroll position to account for the visible rect of the scrollview.</li>
<li>Editor: Fixed scrollview returning scroll position out of view rect size when using scrollwheel.</li>
<li>Editor: Correctly handle when null string is passed to a TextField.</li>
<li>Editor: Don't show Display Resolution Dialog when using CTRL-B from the editor and it's turned off.</li>
<li>Editor: Fixed EditorWindow.ShowPopup with initial position of 0, 0 not rendering correctly.</li>
<li>Editor: Fixed missing bold font in some inspectors (e.g. FBXImporter).</li>
<li>Editor: GizmoType.NotSelected attribute for DrawGizmo works correctly.</li>
<li>Editor: Component menu now handles custom namespaces.</li>
<li>Editor: Light probes are selectable in search mode.</li>
<li>Editor: Excess flood of Animation clips is not confusing the model importer inspector.</li>
<li>Editor: EnumMaskField returns consistent value when every item is selected.</li>
<li>Editor: Textfield word wrapping fixes.</li>
<li>Editor: Display names of colliding enumeration values in inspector</li>
<li>Editor: Fixed problem with the Asset Store window on retina display Macbook Pros.</li>
<li>Editor: Fixed hang while closing if plugins had created their own native threads.</li>
<li>Editor: Fixed odd drawing behavior when attempting to resize welcome screen.</li>
<li>Editor: GUI.color is reset properly for every CustomEditor</li>
<li>Editor: Fixed profiler causing an Out of Memory error in the console.</li>
<li>Editor: Improved error reporting when exporting a Unity package.</li>
<li>Editor: Fixed a bug where ARGB16 textures loaded from AssetBundles built for iOS/Android would load incorrectly.</li>
<li>Editor: Editor doesn't hang anymore if exiting while in play mode.</li>
<li>Editor: Made entering playmode faster by reducing the number of domain reloads.</li>
<li>Editor: Fixed null reference exception when a MonoBehaviour is missing in the inspector. Instead we display helpful warnings embedded in the inspector.</li>
<li>Editor: Fixed issue in fbx importer where prefab instance modifications would in some corner cases get applied to a different object on a different machine</li>
<li>Editor: Fixed bug where calling LoadLevel in OnDestroy when exiting playmode could lead to a crash.</li>
<li>Editor: Fixed bug where the import settings were not updated when a .meta file is changed.</li>
<li>Editor: Fixed various leaks in the asset import pipeline when importing large project folders.</li>
<li>Editor: Fixed prefab override recording issue where modifications would not get applied to array elements if the prefab array is empty and the size value was overridden after the property was overridden.</li>
<li>Editor: Fixed warning when changing import settings on a lot of fbx files.</li>
<li>Editor: Fixed crashbug when clicking on Apply prefab button in the game object inspector when the prefab would add / remove components on awake in edit mode.</li>
<li>Editor: Fixed drag and drop behaviour when dragging child prefab objects.</li>
<li>Editor: Improvements to Light Probe editing: don't change selection when duplicating them; render editable ones on top of baked ones.</li>
<li>Editor: Wireframe and Textured Wireframe scene view modes take actual vertex &amp; tessellation shaders into account now.</li>
<li>Editor: Fixed import of .EXR files with alpha channel.</li>
<li>Editor: Invoked OnFocus/OnLostFocus when switching tabs within the same DockArea.</li>
<li>Editor: Disallowed hiding cursor when GameView is out of focus.</li>
<li>Editor: Fixed crash caused by scene view overlays.</li>
<li>Editor: Fixed box collider handles not matching box collider gizmos.</li>
<li>Editor: Text fields support OS standard behavior of Command + Backspace deleting everything from the start of the current line to the cursor position.</li>
<li>Editor: Cleaned up LOD group inspector (button alignment, text clipping).</li>
<li>Editor: Make Unity 1.x GUI components never be shown in the Scene View.</li>
<li>Editor: Changed order of calculations during model import to improve normal calculation.</li>
<li>Editor: EditorUtility.CopySerialized now works correctly for components.</li>
<li>Editor: Fixed a bug where generated OS X icons would occasionally get corrupted.</li>
<li>Editor: Fixed a bug where the editor would fail to open projects if the root Assets folder has a .meta file.</li>
<li>Editor: Fixed delay when bringing up shader selection menu for the first time (4.0: fixed delay when bringing it up each time).</li>
<li>Editor: Fixed potential crash when editing multiple objects and resizing arrays.</li>
<li>Editor: Fixed Rendering Paths scene view mode to take camera's render path into account, not only what the shaders are capable of.</li>
<li>Editor: Fixed WebPlayer building code; now it does not try to recreate the outermost directory (a user might not have sufficient filesystem access rights anyway).</li>
<li>Editor: Allow for cmd+c and ctrl+c to be used on a SelectableLabel.</li>
<li>Editor: Do not show cut/paste context menu action for SelectableLabel</li>
<li>Editor: Popup windows no longer flicker for a frame on OSX.</li>
<li>Editor: Audio preview in Scene View now works correctly without any Audio Listeners in the scene.</li>
<li>Editor: Fix some importer inspectors constantly repainting.</li>
<li>Editor: Fix key navigation to assets store groups while showing local assets.</li>
<li>Editor: Fixed windows standalone icons alpha issues.</li>
</ul>

###  
<ul>
<li>Flash: Replace no longer ignores parens.</li>
<li>Flash: Several code conversion issues resolved.</li>
<li>Flash: NavmeshPath can now be instantiated correctly.</li>
<li>Flash: Fixed translation of some shaders (e.g. Refractive Glass was causing errors).</li>
<li>Flash: Made AsyncOperation work.</li>
<li>Flash: Fixed division by long and ulong.</li>
<li>Flash: Fixed bug where assigning a struct to an object or interface would introduce two pointers to the same struct instead of two copies.</li>
<li>Flash: Fixed several cornercase bugs in support for generics.</li>
<li>Flash: Properly initialize fields of type DateTime in structs instantiated with default constructor.</li>
<li>Flash: Fixed memory corruption crash if WWW response .Length didn't match actual length of payload.</li>
<li>Flash: Support ++ and -- on arguments that are passed byref, whose result is assigned to an array.</li>
<li>Flash: Fixed mouse visibility bug.</li>
<li>Flash : Fixed equality comparison for ValueTypes.</li>
<li>Flash : Fixed hashtable comparison.</li>
<li>Flash : Fixed enum comparison</li>
<li>Flash : Fixed enum to enum cast.</li>
<li>Flash : Fixed keyboard input handling and TextArea input (control, delete, space, arrow keys).</li>
<li>Flash : Generic collections now work with interfaces.</li>
<li>Flash : Fixed crash when www.audioclip was used in a coroutine.</li>
<li>Flash : SweepTestAll now works.</li>
<li>Flash : UnityEngine.Flash.FlashPlayer allows retrieval of target player and swf version.</li>
<li>Flash: Fixed rare condition in which we ran out of stack space, resulting in an out of range error.</li>
<li>Flash: Fixed issues with anonymous delegates.</li>
<li>Flash: Implemented delegate comparison.</li>
<li>Flash: Implemented Double.TryParse.</li>
<li>Flash: Input.inputString now works.</li>
<li>Flash: No more compiler crashes on incorrect SWF dimensions.</li>
<li>Flash: Key repeat works.</li>
<li>Flash: Fixed NewInstance for Enum value types</li>
<li>Flash: Fixed getter/setter generation for System.Array.</li>
<li>Flash: Don't show Development Build watermark in non-dev builds.</li>
<li>Flash: Fixed issues with anonymous delegates.</li>
<li>Flash : Fix string marshalling. Now consistently UTF8.</li>
<li>Flash : Fix dynamic font textures generated larger then Flash max texture size (2048*2048).</li>
<li>Flash : Fix dynamic font generation trashing memory.</li>
<li>Flash : Fix invalid agal generated for cube map samplers.</li>
<li>Flash : Fix backbuffer being cleared because of rtt.</li>
<li>Flash : Fix type inference for float division.</li>
<li>Flash : Fix issue with loitering objects in finalizermaps.</li>
<li>Flash : Fix issue with converted GetHashCode code being invalid when generated from a MS compiler.</li>
<li>Flash : Implemented Char.ConvertFromUtf32</li>
<li>Flash : Improved support for System.Convert</li>
<li>Flash : Adding support for TryParse for additional data types.</li>
<li>Font rendering: Fixed position of text cursor when a custom font size is used for the TextField.</li>
<li>Font rendering: Fixed kerning.</li>
<li>Graphics: Fixed crashes that sometimes occurred on OpenGL with mismatched GL.Begin/GL.End pairs.</li>
<li>Graphics: Fixed TrailRenderer culling issue.</li>
<li>Graphics: Don't break batching based on shadow distance when there aren't any shadow casting lights.</li>
<li>Graphics: Properly take line width into account when adding points to LineRenderer.</li>
<li>Graphics: SubShader tags (render queue etc.) take shader LOD into account properly now.</li>
<li>Graphics: Free up temporary memory used by non-uniformly scaled mesh when deactivating a mesh renderer.</li>
<li>Graphics: Static batching performs better when there are multiple lightmaps in the scene (before it could run into cases where it wasn't batching much).</li>
<li>Graphics: Fixed memory leak in Material.CopyPropertiesFromMaterial.</li>
<li>Graphics: Fixed a rare "invalid angle: inf" error message with terrain and shadows.</li>
<li>Graphics: Fixed Camera pixelWidth/pixelHeight/aspect queries done from Editor code being really confusing. Before, it was using the size of last drawn editor view for the calculations. Now, for regular cameras, Game View size is used.</li>
<li>Graphics: Fixed crash in Shuriken mesh particles, when source mesh has no normals or tangents.</li>
<li>Graphics: Fixed errors with statically batched meshes that are later modified by a script.</li>
<li>Graphics: Fixed issue with Deferred rendering and wireframe Scene View mode.</li>
<li>Graphics: Fixed various issues with shaders in asset bundles. E.g. you can actually put terrain with trees into an asset bundle, and the billboard shaders will work, without having to jump through various hoops.</li>
<li>Graphics: Properly include all shaders into game data files when editor is in "-nographics" mode.</li>
<li>Graphics: Batched Shuriken draw calls were not accounted for in the game view stats window.</li>
<li>Graphics: Don't load Occlusion Culling data in non-Pro editor licenses.</li>
<li>Graphics: Fixed console error messages when a terrain tree prefab is missing.</li>
<li>Graphics: Smoother framerate on Windows when using vsync.</li>
<li>Graphics: Fixed Screen.resolutions reporting zero for refresh rate in some cases.</li>
<li>Graphics: Fixed crash when using additive scene loading with missing lightmaps.</li>
<li>Graphics: Fixed small memory leak when loading shaders with syntax errors; made shader loading a bit faster as a byproduct ;)</li>
<li>Graphics: Fixed error messages in some situations when calling camera.Render from editor scripts.</li>
<li>Graphics: Fixed surface shader finalcolor modifier sometimes producing wrong results.</li>
<li>Graphics: Limit maximum texture size to 4096 on Retina MacBookPros due to OS X driver bugs.</li>
<li>Graphics: Removed limitation that Windows Standalone game window can't reach whole desktop screen size.</li>
<li>Graphics: On Linux, fixed lower resolution blit texture getting broken due to quality settings change.</li>
<li>Graphics: Improved deferred lighting depth buffer sharing workaround for some OpenGL systems. Mostly, much faster now on some Linux GPUs/drivers.</li>
<li>Graphics: Fixed different mesh compression setting to actually make a difference (previously it would always use "Low" compression, regardless of setting).</li>
<li>Graphics: Fixed some issues with Fog on Direct3D 9; in rare cases with some complex shaders it was not working properly.</li>
<li>Graphics: Fixed HDR rendering being off in the very first frame.</li>
<li>Graphics: Fixed Camera.hdr returning wrong value when called before render.</li>
<li>Graphics: Fixed occasional errors being reported when rendering objects with zero scale.</li>
<li>IMGUI: Fix BeginHorizontal not displaying content/tooltip when using GUIStyle.none.</li>
<li>Image Effects: Fixed Flash-related warning messages when importing Image Effects package.</li>
<li>Image Effects: Fixed Global Fog on Windows when MSAA is used.</li>
<li>Input: Fixed OnMouseDown and related callbacks being wrongly sent to cameras that render into RenderTextures.</li>
<li>Input: Gamepad buttons are now correctly initialized again.</li>
<li>iOS: Fixed Xcode crash when native plugin uses "+" in the name.</li>
<li>iOS: Fixed iPad splash handling when starting in portrait.</li>
<li>iOS: Made various orientation fixes.</li>
<li>iOS: Corrected texture atlas padding.</li>
<li>iOS: Fixed skinning corrupting UVs.</li>
<li>iOS: Fixed crash on suspending app while playing video.</li>
<li>iOS: Fixed recognition of more recent iPhone4/4S models.</li>
<li>iOS: Fixed various crashes when Script Call Optimization set to "fast but no exceptions".</li>
<li>iOS: Fixed text-area behavior when on-screen keyboard is hidden.</li>
<li>iOS: Fixed Screen.orientation on the first frame on iOS6.</li>
<li>iOS: Fixed interoperability of DisplayLink mode and iOS native UI.</li>
<li>iOS: Fixed iOS splash screen image not being released after game starts.</li>
<li>iOS: Fixed www.uploadProgress support.</li>
<li>iOS: Fixed loading indicator position.</li>
<li>iOS: Small GPU profiling (in the internal iPhone profiler) improvement.</li>
<li>iOS: Fixed basic license splash screen issue with Xcode 4.5.</li>
<li>iOS: Fixed support for native methods inside of inner classes.</li>
<li>iOS: More fixes to initial orientation handling.</li>
<li>iOS: Unity Remote support updated to work better with input compensation for screen orientation.</li>
<li>iOS: Fixed Screen.dpi for iPad Mini.</li>
<li>Javascript: Fixed error checking for array indices.</li>
<li>Javascript: Fixed regression on 'not in' operator. Operator has been brought back.</li>
<li>Javascript: Introduced 'for each' syntax for better compatibility with other javascript dialects.</li>
<li>Lightmapping: Fixed "Generate Lightmap UVs" difference between Windows &amp; Mac!</li>
<li>Lightmapping: Fixed handling degenerate triangles in UV space, Beast no longer spits out "TexBakeSampleGenerator: Non-invertible matrix".</li>
<li>Lightmapping: Skipping tree instances that reference a prototype without a mesh.</li>
<li>Lightmapping: Improved error messages when failing to bake Light Probes; when meshes have UVs outside 0..1 range, when meshes have missing UVs.</li>
<li>Lightmapping: Take texture tiling into account for materials with cutout shaders.</li>
<li>Lightmapping: Fixed issues with some emissive materials.</li>
<li>Lightmapping: Fix harmless error when lightmap baking an unsaved scene on Mac.</li>
<li>LOD: Fix double GUI repaint error when caused by reparent renderers dialog.</li>
<li>Mobile: Better RenderTexture.DiscardContents implementation.</li>
<li>Mobile: Fixed wrong lighting when dynamically batching uniformly scaled meshes.</li>
<li>Mac OS X Editor: Fixed window focus issues when using a multiple screen setup in OS X 10.8 Mountain Lion.</li>
<li>Mac OS X: Event.clickCount behavior for double-clicks now matches windows (clickCount is always 1 for MouseUp events).</li>
<li>Mac OS X: Don't freeze Unity content when the System clock is changed while running.</li>
<li>Mac OS X: PlayerPrefs keys will now work if they contain an '@' character.</li>
<li>Mac OS X: Fix Webcam textures with non-native resolutions correctly picking up the desired texture size.</li>
<li>Mac OS X: Fixed some graphics issues on dual-GPU Mac models, e.g. editor windows occasionally becoming all white.</li>
<li>Mac OS X: Fixed Crash on quit if profiling had been enabled.</li>
<li>Mac OS X Standalone: Fixed problems when writing OS X icon format, leading to broken icon graphics in some cases.</li>
<li>Mac OS X Standalone: Used OS X Lion style fullscreen mode, to allow other windows to show up in front of fullscreen apps, and to allow switching in and out of fullscreen mode by clicking onto the fullscreen button in the window title bar (optional).</li>
<li>Mac OS X Standalone: Fix hiding of window when GameCenter is activated.</li>
<li>Mac OS X Standalone: Changed event processing to allow other windows to receive keyboard events, to allow better integration with OS services such as GameCenter using plugins.</li>
<li>Mac OS X Web Player: Made IME support work in all Mac browsers.</li>
<li>Mac OS X Web Player: Fixed focus handling when the browser is switched to the background or the user switches to another window/tab.</li>
<li>Mac OS X Web Player: Fixed memory leak.</li>
<li>Mac OS X WebPlayer: Fixed OnApplicationPause being called when window goes to the background.</li>
<li>Math: Fixed Plane.SameSide equation side error.</li>
<li>Misc: Improve Time.smoothDeltaTime so it's not affected by pausing/unpausing.</li>
<li>Native Client: Fixed download of JPG files as textures.</li>
<li>Native Client:: Fixed problem where preferences might get lost when the player is closed while writing preferences to disk.</li>
<li>Native Client: Fixed deadlock when loading mono DLLs.</li>
<li>Native Client: Fixed Build &amp; Run with Chrome 23.</li>
<li>NavMeshAgent : Fix crash querying nextOffMeshLinkData when having no navmesh in scene.</li>
<li>NavMeshAgent: Fixed bug where Resume breaks updateRotation setting.</li>
<li>NavMeshAgent: Path request processing queue order fixed.</li>
<li>Physics: Fixed problem where CCD would incorrectly detect collisions if the center or scale of a collider was changed.</li>
<li>Networking: Fixed case where a MasterServerEvent.HostListReceived was triggered for each host in a host list.</li>
<li>Networking: Fixed problem with connecting to password protected servers with NAT punchthrough.</li>
<li>Player: Fixed race condition in WWW class that could cause a crash when aborting download.</li>
<li>Physics: Fixed MeshCollider not working if it had been scaled to be zero sized, and then scaled up again.</li>
<li>Physics: Fixed a bug where Raycasts against CapsuleColliders with a zero-length middle section would not always return correct results.</li>
<li>Physics: Fixed a bug where destroyed colliders would not be properly deallocated if Time.timeScale was zero.</li>
<li>Physics: Fixed colliders being properly inactive when they are on inactive child game objects of the rigidbody.</li>
<li>Physics: Fixed collision between two triggers to send OnTriggerEnter events to both triggers and both rigidbodies for consistent results.</li>
<li>Physics: Fixed memory leak when Time.timeScale is zero.</li>
<li>Physics: Fix problem with activation order when recursively activating hierarchies, causing rag dolls not to function properly in some cases.</li>
<li>Physics: Fixed a bug where rigidbody interpolation would have an effect on physics simulation results.</li>
<li>Physics cloth: Fixed tangents to match initial rotation of object.</li>
<li>Prefabs: Duplicating game objects with references to abstract classes behaves more reliable.</li>
<li>Profiler: Fixed hang on editor or player when connection could not keep up with the data.</li>
<li>Profiler: Made the profiler skip frames instead of freezing up if editor lacks behind player.</li>
<li>Profiler: GC memory was not propagated correctly up the call hierarchy.</li>
<li>ProfilerConnection: Fixed inifinite loop freeze if profiler sendbuffer is full on the player.</li>
<li>Scene View: Fix scene editor camera becoming locked out from user control.</li>
<li>Scripting: Added overloads to EditorGUI.IntSlider so it can take SerializedProperties.</li>
<li>Scripting: Fixed crash when calling material.GetFloat(null).</li>
<li>Scripting: Fixed crash when a component destroys itself while AddComponent is trying to create it.</li>
<li>Scripting: Fixed crash calling Resources.Load before resources have been imported.</li>
<li>Scripting: Fixed bug where AssetBundle.LoadFromFile would get unloaded by UnloadUnusedAssets.</li>
<li>Scripting: GameObject.Find will now correctly find children of objects of the same name as other objects which don't have children of that name.</li>
<li>Scripting: Fixed crash when a gameObject is being destroyed while calling SendMessage on it.</li>
<li>Scripting: Fixed script serialization bug where properties could not be #if-ed out for the player.</li>
<li>Serialization: For non-webplayer-targets, scenes (implicitly) referencing assets placed under the Resources folder will now always have the assets placed together with the scene (and not in the resources.assets).</li>
<li>Shaders: Fog shader variables (unity_FogColor etc.) are set to produce no fog when it's off.</li>
<li>Shaders: round() and trunc() HLSL functions are now supported when compiling shaders for mobile.</li>
<li>Shaders: Updated HLSL-to-GLSL shader compilers; fixes some complex mobile shaders (e.g. Tree Creator ones, or Edge Detection image effect on some mobile GPUs).</li>
<li>Shaders: Fixed compile errors in some cases where custom directional lightmap lighting function is used.</li>
<li>Shadows: Fixed shadow caster culling when light direction is exactly parallel to one of camera's frustum planes.</li>
<li>Shuriken: Fixed particle system randomness. There should be a lot less visible correlation between parameters when using random between curves and values.</li>
<li>Shuriken: Can't remove disabled UI modules, gizmo scaling issue, simulation preview issues when scrubbing.</li>
<li>Shuriken: Fixed sub-emitter memory leaks, occasional crash.</li>
<li>Shuriken: Gracefully handle when mesh is invalid, instead of leaving the emitter in a bad state.</li>
<li>Shuriken: Fixed crash if using mesh particles without UVs.</li>
<li>Standard Assets: Projector uses smaller, but uncompressed textures; to avoid artifacts when looking from a distance.</li>
<li>Substances now handles iOS non-square unsupported PVRTC.</li>
<li>Substance: Fixed baking issues on unsupported platforms (Android, iOS, Flash).</li>
<li>Substance: Lower memory consumption in the Editor when importing projects and switching color space.</li>
<li>Substance: Fixed runtime re-generation of substances with bitmap inputs.</li>
<li>Substance: "Generate all outputs" now displays all generated textures in the Inspector.</li>
<li>Substance: Fixed cloning substances in the Inspector.</li>
<li>Substance: Fixed bitmap export.</li>
<li>Substance: Fixed several erroneous error messages appearing in the log.</li>
<li>Terrain: Fixed error messages when painting terrain grass with negative sizes, and when adding some tree models.</li>
<li>Terrain: Terrain renderer no longer causes invalid memory accesses during rendering traversal.</li>
<li>Time: Fixed timescale usage when single stepping.</li>
<li>UV generation is now more deterministic between platforms since it is performed prior to scaling of vertices.</li>
<li>UnityObject: The default templates works nicely over https now.</li>
<li>UnityObject: Running a offline build locally will not break the default templates.</li>
<li>WebCamTextures: Fixed error message when querying list of available devices while WebCams are in use.</li>
<li>Web Player: Application.dataPath will now work correctly if the player URLs has slash characters in the url parameters.</li>
<li>WebPlayer: Fixed the plugin ticking routine. It is simpler and less error prone.</li>
<li>WebPlayer: Updated the builtin resources; now there is a distinction between "Made with Unity 4 Beta" and "Unity 4 Beta" plugin.</li>
<li>WebPlayer: Fixed a variety of crashes when plugin was running on IE9.</li>
<li>Webplayer: Crash logs now contain stacktrace.</li>
<li>Webplayer: Fixed memory overwrite on startup when running in-process on Firefox.</li>
<li>WWW Class: Fixed parsing text encoding if the encoding http header contains more parameters.</li>
<li>Windows: Improved StackOverflowException handling in scripts.</li>
<li>Windows: Fixed issues with 64-bit player not launching when non-latin characters in path.</li>
<li>Windows Editor: Messages with "Failed: The operation has completed successfully" should not be presented anymore when operations on files fail.</li>
<li>Windows Editor: Fixed extracting .unitypackage files containing extended Unix file attributes.</li>
<li>Windows Editor: Asset Store window now works correctly in OpenGL mode.</li>
</ul>
