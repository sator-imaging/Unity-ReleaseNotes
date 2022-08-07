# Unity 4.0
https://unity3d.com/unity/whats-new/unity-4.0

## Other Improvements

<ul>
<li>Android: Exposed control over SYSTEM_UI_FLAG_LOW_PROFILE ("lights-out" mode) through Screen.fullScreen.</li>
<li>Android: Added support for Input.compenstateSensors.</li>
<li>Android: Added support ldpi/xhdpi icon images.</li>
<li>Android: Added support for non-US characters for key store keys and passwords.</li>
<li>Android uses compressed vertex streams (where available).</li>
<li>Animation : Can now preview non-Mecanim animation in previewer.</li>
<li>Cache Server: Now includes a 32-bit linux build.</li>
<li>Cache Server: Modifying the import settings and clicking on Apply will now also use the cache server if it is available.</li>
<li>Cache Server: Made sure the Editor does not connect to cache server when it's not needed.</li>
<li>Documentation: Improvements to shader authoring documentation (Built-in shader include files, Predefined shader preprocessor macros, DirectX 11).</li>
<li>Documentation: Extended Low-level Native Plugin Interface example to demonstrate DirectX 11 rendering from a plugin.</li>
<li>Editor: In the Build Settings Window it is now possible to change enabled state for all the selected scenes in one click (Use Ctrl + A for selecting all scenes).</li>
<li>Editor: Component context menu (gear icon) got Move Up/Down, Copy &amp; Paste entries.</li>
<li>Editor: Light Probes scene view rendering mode gone; probe visualization in lightmapping window overlay.</li>
<li>Editor: Dragging a .unityPackage file into project view imports it now.</li>
<li>Editor: The Scene Gizmo axis cones no longer sets the camera to be orthographic. The center cube now toggles orthographic. The label below the gizmo now toggles between perspective and ortho as well. Shift-clicking or middle-mouse clicking the center cube will set the "nice" perspective view and shift-clicking or middle-mouse clicking the cones will enforce ortho.</li>
<li>Editor: Simplified mobile graphics emulation; only have OpenGL ES 1.1 &amp; 2.0 now.</li>
<li>Editor: Lightmaps now get "best" compression quality for mobiles when available.</li>
<li>Editor: Added menu item in Component menu for Add Component drop-down.</li>
<li>Editor: Don't show animation import settings if no animation data is available.</li>
<li>Editor: Cleaned up indentation logic so LooksLikeInspector &amp; LooksLikeControls are more similar.</li>
<li>Editor: Ignore symlinks in Windows so it behaves like OS X build.</li>
<li>Editor: Inspector Window recovers gracefully when a CustomEditor throws an exception or has missing layout group endings.</li>
<li>Editor: GameObject and Prefab inspector icons indicate active object status.</li>
<li>Editor: Counters for collapsed console entries.</li>
<li>Editor: Scene View now shows the current View Tool (Move, Orbit, Zoom, FPS) as the cursor to reinforce what's happening.</li>
<li>Editor: New icons throughout Unity.</li>
<li>Execution order of components and scripts is now always the same between Player and Editor.</li>
<li>Editor: Light picker icons (gizmo icons) now reflect the color (hue and saturation) and type (point/spot/directional/directional, main/area) of light.</li>
<li>Flash: Scripting overall; Better generics support.</li>
<li>Flash: Added FlashPlayer 11.3 and 11.4 support. Mouse middleclick and right click is supported on this subtarget.</li>
<li>Flash: Added support for Enum.GetValues() &amp; Enum.GetNames().</li>
<li>Flash: Added support subset of field reflection.</li>
<li>Flash: Full support for animation events, including runtime scripting API.</li>
<li>Flash: Reduce black screen initialization time.</li>
<li>Flash: Reduced memory footprint.</li>
<li>Flash: Performance increased.</li>
<li>Flash: Improved support for static fields of generic type.</li>
<li>Flash: Implemented support for batching. No runtime scripting support for batching yet.</li>
<li>Flash: Injection of swf tag for 3rd party profilers.</li>
<li>Flash: Reduced number of Stage3D calls per frame.</li>
<li>Font rendering: Add Font.RequestCharactersInTexture, Font.GetCharacterInfo and Font.textureRebuildCallback to allow full control over dynamic fonts from scripting.</li>
<li>Font rendering: Made font texture rebuild callback get called less often.</li>
<li>Graphics: Exposed GUITexture.border to scripts.</li>
<li>Graphics: Added "Read/Write Enabled" checkbox to Model Import Settings. Disabling this will reduce memory footprint of meshes.</li>
<li>Graphics: Dynamic Batching with tangent vectors works on Windows &amp; Mac now (was disabled before due to various driver issues).</li>
<li>Graphics: Surface shaders can use arbitrary vertex input data type (instead of appdata_full); now the type of a vertex modifier parameter is used.</li>
<li>Graphics: Shader properties can have [HideInInspector] in front of them, which makes them hidden in inspector (useful for properties that are set from code).</li>
<li>Graphics: Optimized light culling; particularly noticeable when you have lots of baked lights.</li>
<li>Image Effects: Screen Overlay effect fixed "overlay" blend mode, and gained an intensity slider.</li>
<li>Image Effects: Some optimizations for Tonemapping effect.</li>
<li>Image Effects: Vignetting effect got a nicer inspector.</li>
<li>Image Effects: Moved chromatic aberration from Bloom to Vignetting image effect.</li>
<li>iOS: iOS view handling extracted to separate files in trampoline.</li>
<li>iOS: Added request for re-orientation on iOS5 and newer when allowed auto-rotation orientations were changed.</li>
<li>iOS Remote: Improved latency of touch events sent to editor.</li>
<li>iOS: Improved fog performance.</li>
<li>Mac OS X: Make installers and Editor application signed so they can be run with the default security settings in OS X 10.8 Mountain Lion.</li>
<li>Mac OS X Standalone: Added support for 256x256, 512x512 and 1024x1024 icons.</li>
<li>Mac OS X Standalone and Editor: WWW class will now correctly use the proxy selected in System Preferences.</li>
<li>Mac OS X Web Player: Respect system scroll direction in fullscreen mode.</li>
<li>Mobile: PowerVR texture compression tool updated to 2.10.87.4981.</li>
<li>Mobile: Introduced RGBA16 texture format.</li>
<li>Mobile: Added TouchScreenKeyboard.wasCanceled. On iOS, a “Cancel” button was added, on Android, the “back” button will be used for that</li>
<li>Mobile: TouchScreenKeyboard.text now can be used to set text to show in edit field.</li>
<li>Mobile: ActivityIndicator can now be started/stopped from script.</li>
<li>Mobile: SystemInfo.supportsVibration now queries device for actual support.</li>
<li>Mobile: OpenGL ES version selector is now shared between Android/iOS.</li>
<li>Mobile: Some optimizations regarding dynamic geometry.</li>
<li>Mobile: Increased max texture size for OpenGL ES 2.0 to 4096 and added handling of GPU imposed restrictions on texture size at runtime.</li>
<li>Mobile: Enabled OnMouse event processing for scripts that use it.</li>
<li>MonoDevelop: Updated Gtk+ for improved behavior and responsiveness (OSX).</li>
<li>NavMesh: Improved crowd avoidance. Now prioritize neighbours by the predicted time of impact instead of distance.</li>
<li>NavMesh: OffMeshLink has GUI for selection of NavMeshLayer.</li>
<li>Profiler can now profile the editor.</li>
<li>Runtime: Fixed rare issue where loading a level asynchronously could be interrupted by other loading operations.</li>
<li>Runtime: Instantiate now respects script execution order.</li>
<li>Runtime: GameObjects marked DontDestroyOnLoad are no longer temporarily deactivate when loading a level. This way they also will not receive a OnDisable / OnEnable call when loading a level.</li>
<li>Scene View: Show small icon next to Scene Gizmo label showing whether Scene View is in perspetive or isometric mode.</li>
<li>Scene View: When in axis-aligned view such as "Right", always show that in label and not "Iso" or "Persp".</li>
<li>Scene View - Mac: Make Scene View swipe gestures math the SceneView Gizmos</li>
<li>Scripting: Users can now add their own per-platform custom defines in the player settings.</li>
<li>Scripting: MonoBehaviours can now be inside namespaces.</li>
<li>Scripting: SkinnedMeshRenderer.rootBone is now exposed to scripting.</li>
<li>Scripting: Allow creation of editor scriptable objects from runtime scripts when inside the editor.</li>
<li>Shaders: Vertex shader inputs don't have to come from a struct with predefined names anymore. Just use proper semantics and you're good now.</li>
<li>Shaders: Added unity_CameraWorldClipPlanes built-in shader variable. Contains camera's world space clipping planes.</li>
<li>Shuriken: Cone emitters: Support for emit from shell, emit from volume and controlling random direction.</li>
<li>Shuriken: Support for up to 4 meshes in particle system renderer. Selection of mesh happens randomly.</li>
<li>Shuriken: Support for up to 2 sub emitters per type (previously 1).</li>
<li>Shuriken: Dynamic batching support for particle sprites.</li>
<li>Shuriken: Particle updates are now multithreaded together with LateUpdate script calls. This should in most cases result in better performance.</li>
<li>Shuriken: It is now possible to specify a particle radius in the collision module which can be used for avoiding clipping artifacts.</li>
<li>Shuriken: Simulate() calls are much faster for most systems.</li>
<li>Shuriken: Exposed .randomSeed to script.</li>
<li>Shuriken: Exposed .particleSystem to GameObject scripting.</li>
<li>Shuriken: Improved API for Emit(count) and added 2 more Emit() functions.</li>
<li>Shuriken: Optimizations across the board for performance and less memory usage.</li>
<li>Social API: Added a GameCenterPlatform function for showing a specific Leaderboard UI based on ID + TimeScope.</li>
<li>Substance: Fast-forward reimport of a substance when leaving the substance Inspector.</li>
<li>Substance: Faster tweaking / import in the Editor (multi-threaded now activated by default only in the Editor).</li>
<li>Web Player: Make HTTP error handling more robust in Internet Explorer.</li>
</ul>
