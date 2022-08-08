# Unity 4.0

https://unity3d.com/unity/whats-new/unity-4.0

## Other Improvements



*   Android: Exposed control over SYSTEM\_UI\_FLAG\_LOW\_PROFILE ("lights-out" mode) through Screen.fullScreen.
*   Android: Added support for Input.compenstateSensors.
*   Android: Added support ldpi/xhdpi icon images.
*   Android: Added support for non-US characters for key store keys and passwords.
*   Android uses compressed vertex streams (where available).
*   Animation : Can now preview non-Mecanim animation in previewer.
*   Cache Server: Now includes a 32-bit linux build.
*   Cache Server: Modifying the import settings and clicking on Apply will now also use the cache server if it is available.
*   Cache Server: Made sure the Editor does not connect to cache server when it's not needed.
*   Documentation: Improvements to shader authoring documentation (Built-in shader include files, Predefined shader preprocessor macros, DirectX 11).
*   Documentation: Extended Low-level Native Plugin Interface example to demonstrate DirectX 11 rendering from a plugin.
*   Editor: In the Build Settings Window it is now possible to change enabled state for all the selected scenes in one click (Use Ctrl + A for selecting all scenes).
*   Editor: Component context menu (gear icon) got Move Up/Down, Copy & Paste entries.
*   Editor: Light Probes scene view rendering mode gone; probe visualization in lightmapping window overlay.
*   Editor: Dragging a .unityPackage file into project view imports it now.
*   Editor: The Scene Gizmo axis cones no longer sets the camera to be orthographic. The center cube now toggles orthographic. The label below the gizmo now toggles between perspective and ortho as well. Shift-clicking or middle-mouse clicking the center cube will set the "nice" perspective view and shift-clicking or middle-mouse clicking the cones will enforce ortho.
*   Editor: Simplified mobile graphics emulation; only have OpenGL ES 1.1 & 2.0 now.
*   Editor: Lightmaps now get "best" compression quality for mobiles when available.
*   Editor: Added menu item in Component menu for Add Component drop-down.
*   Editor: Don't show animation import settings if no animation data is available.
*   Editor: Cleaned up indentation logic so LooksLikeInspector & LooksLikeControls are more similar.
*   Editor: Ignore symlinks in Windows so it behaves like OS X build.
*   Editor: Inspector Window recovers gracefully when a CustomEditor throws an exception or has missing layout group endings.
*   Editor: GameObject and Prefab inspector icons indicate active object status.
*   Editor: Counters for collapsed console entries.
*   Editor: Scene View now shows the current View Tool (Move, Orbit, Zoom, FPS) as the cursor to reinforce what's happening.
*   Editor: New icons throughout Unity.
*   Execution order of components and scripts is now always the same between Player and Editor.
*   Editor: Light picker icons (gizmo icons) now reflect the color (hue and saturation) and type (point/spot/directional/directional, main/area) of light.
*   Flash: Scripting overall; Better generics support.
*   Flash: Added FlashPlayer 11.3 and 11.4 support. Mouse middleclick and right click is supported on this subtarget.
*   Flash: Added support for Enum.GetValues() & Enum.GetNames().
*   Flash: Added support subset of field reflection.
*   Flash: Full support for animation events, including runtime scripting API.
*   Flash: Reduce black screen initialization time.
*   Flash: Reduced memory footprint.
*   Flash: Performance increased.
*   Flash: Improved support for static fields of generic type.
*   Flash: Implemented support for batching. No runtime scripting support for batching yet.
*   Flash: Injection of swf tag for 3rd party profilers.
*   Flash: Reduced number of Stage3D calls per frame.
*   Font rendering: Add Font.RequestCharactersInTexture, Font.GetCharacterInfo and Font.textureRebuildCallback to allow full control over dynamic fonts from scripting.
*   Font rendering: Made font texture rebuild callback get called less often.
*   Graphics: Exposed GUITexture.border to scripts.
*   Graphics: Added "Read/Write Enabled" checkbox to Model Import Settings. Disabling this will reduce memory footprint of meshes.
*   Graphics: Dynamic Batching with tangent vectors works on Windows & Mac now (was disabled before due to various driver issues).
*   Graphics: Surface shaders can use arbitrary vertex input data type (instead of appdata\_full); now the type of a vertex modifier parameter is used.
*   Graphics: Shader properties can have \[HideInInspector\] in front of them, which makes them hidden in inspector (useful for properties that are set from code).
*   Graphics: Optimized light culling; particularly noticeable when you have lots of baked lights.
*   Image Effects: Screen Overlay effect fixed "overlay" blend mode, and gained an intensity slider.
*   Image Effects: Some optimizations for Tonemapping effect.
*   Image Effects: Vignetting effect got a nicer inspector.
*   Image Effects: Moved chromatic aberration from Bloom to Vignetting image effect.
*   iOS: iOS view handling extracted to separate files in trampoline.
*   iOS: Added request for re-orientation on iOS5 and newer when allowed auto-rotation orientations were changed.
*   iOS Remote: Improved latency of touch events sent to editor.
*   iOS: Improved fog performance.
*   Mac OS X: Make installers and Editor application signed so they can be run with the default security settings in OS X 10.8 Mountain Lion.
*   Mac OS X Standalone: Added support for 256x256, 512x512 and 1024x1024 icons.
*   Mac OS X Standalone and Editor: WWW class will now correctly use the proxy selected in System Preferences.
*   Mac OS X Web Player: Respect system scroll direction in fullscreen mode.
*   Mobile: PowerVR texture compression tool updated to 2.10.87.4981.
*   Mobile: Introduced RGBA16 texture format.
*   Mobile: Added TouchScreenKeyboard.wasCanceled. On iOS, a “Cancel” button was added, on Android, the “back” button will be used for that
*   Mobile: TouchScreenKeyboard.text now can be used to set text to show in edit field.
*   Mobile: ActivityIndicator can now be started/stopped from script.
*   Mobile: SystemInfo.supportsVibration now queries device for actual support.
*   Mobile: OpenGL ES version selector is now shared between Android/iOS.
*   Mobile: Some optimizations regarding dynamic geometry.
*   Mobile: Increased max texture size for OpenGL ES 2.0 to 4096 and added handling of GPU imposed restrictions on texture size at runtime.
*   Mobile: Enabled OnMouse event processing for scripts that use it.
*   MonoDevelop: Updated Gtk+ for improved behavior and responsiveness (OSX).
*   NavMesh: Improved crowd avoidance. Now prioritize neighbours by the predicted time of impact instead of distance.
*   NavMesh: OffMeshLink has GUI for selection of NavMeshLayer.
*   Profiler can now profile the editor.
*   Runtime: Fixed rare issue where loading a level asynchronously could be interrupted by other loading operations.
*   Runtime: Instantiate now respects script execution order.
*   Runtime: GameObjects marked DontDestroyOnLoad are no longer temporarily deactivate when loading a level. This way they also will not receive a OnDisable / OnEnable call when loading a level.
*   Scene View: Show small icon next to Scene Gizmo label showing whether Scene View is in perspetive or isometric mode.
*   Scene View: When in axis-aligned view such as "Right", always show that in label and not "Iso" or "Persp".
*   Scene View - Mac: Make Scene View swipe gestures math the SceneView Gizmos
*   Scripting: Users can now add their own per-platform custom defines in the player settings.
*   Scripting: MonoBehaviours can now be inside namespaces.
*   Scripting: SkinnedMeshRenderer.rootBone is now exposed to scripting.
*   Scripting: Allow creation of editor scriptable objects from runtime scripts when inside the editor.
*   Shaders: Vertex shader inputs don't have to come from a struct with predefined names anymore. Just use proper semantics and you're good now.
*   Shaders: Added unity\_CameraWorldClipPlanes built-in shader variable. Contains camera's world space clipping planes.
*   Shuriken: Cone emitters: Support for emit from shell, emit from volume and controlling random direction.
*   Shuriken: Support for up to 4 meshes in particle system renderer. Selection of mesh happens randomly.
*   Shuriken: Support for up to 2 sub emitters per type (previously 1).
*   Shuriken: Dynamic batching support for particle sprites.
*   Shuriken: Particle updates are now multithreaded together with LateUpdate script calls. This should in most cases result in better performance.
*   Shuriken: It is now possible to specify a particle radius in the collision module which can be used for avoiding clipping artifacts.
*   Shuriken: Simulate() calls are much faster for most systems.
*   Shuriken: Exposed .randomSeed to script.
*   Shuriken: Exposed .particleSystem to GameObject scripting.
*   Shuriken: Improved API for Emit(count) and added 2 more Emit() functions.
*   Shuriken: Optimizations across the board for performance and less memory usage.
*   Social API: Added a GameCenterPlatform function for showing a specific Leaderboard UI based on ID + TimeScope.
*   Substance: Fast-forward reimport of a substance when leaving the substance Inspector.
*   Substance: Faster tweaking / import in the Editor (multi-threaded now activated by default only in the Editor).
*   Web Player: Make HTTP error handling more robust in Internet Explorer.