# Unity 4.3

https://unity3d.com/unity/whats-new/unity-4.3

## Improvements



*   AI / NavMesh: Performance! Crowd update is multithreaded when there are more than 50 active navmesh agents - if supported by device.
*   AI / NavMesh: Obstacle carving support. NavMeshObstacle supports carving via the "Carve" flag on the component.
*   AI / NavMesh: OffMeshLink Component is dynamic. OffMeshLink component creation/modification/destruction has effect at runtime and in the editor. No baking of navmesh is required.
*   AI / NavMesh: 'CalculateTriangulation' calculates and returns a simple triangulation of the current navigation mesh. Returned is a struct containing the vertices, triangle indices and navmesh layers.
*   AI / NavMesh: OffMeshLink Component API additions: navMeshLayer, biDirectional, startTransform, endTransform, autoUpdatePositions, UpdatePosition.
*   Android: Always use non-linear z if available for 16 bit depth buffers
*   Android: Joystick input should now be more concise across different gamepads and devices.
*   Android: Support for secondary and tertiary mouse button (requires ICS).
*   Android: GL context recreation will only take place when strictly needed.
*   Android: Better EGL context selection. Now much more likely to pick a configuration with proper anti aliasing, stencil, depth etc.
*   Android: Native EGL/OpenGLES (no longer initialized through Java).
*   Animation Window: New clips are saved into project browser active folder instead of project root by default.
*   Animation Window: Recording goes through the new Undo system. Only changes that are Undoable are recorded.
*   Animation Window: Hotkey 'k' for add keyframe button.
*   Animation Window: Properties that are being animated show up in yellow.
*   BlackBerry: Added checkbox to allow users to indicate Gamepad support for their games
*   BlackBerry: It is now possible to specify build ID.
*   BlackBerry: Gamepad trigger buttons are now supported.
*   Documentation: undocumented APIs will now show up as empty stubs
*   Documentation: more Scripting docs for 2D APIs
*   DX11: Use new fixed function shader generator on Windows 8.1
*   Editor: Improve workflow when layout with custom windows failed to load due to compile errors.
*   Editor: Modified occlusion culling default baking parameters (smallest occluder value 1.0 -> 5.0)
*   Editor: No longer downloads an ivy.xml file every time you push play.
*   Editor: Removed dysfunctional Xcode 4 setting
*   Editor: Updated Unity Logo and icons
*   Editor: Better performance when entering and exiting playmode
*   Editor: Improved search in Project Browser and Hierarchy: We now support searching for types in namespaces and base types can be used to find derived types.
*   Editor: Improve error handling of renaming/creating assets when inputing invalid file name chars
*   Editor: SHIFT+F or double-F locks the scene view camera to the selected GameObject.
*   Editor: "alpha is transparency" textures are displayed with a checker background in material inspector; and nicer display in project browser.
*   Editor: Optimize Inspector GUI by avoiding much of the string handling associated with PropertyDrawers.
*   Editor: Order and group menu items in Assets/Create menu so related items are together.
*   Editor: PropertyDrawers now have a fieldInfo property that can be used to obtain reflection data about the member that the property represents.
*   Editor: PropertyDrawers can now call EditorGUI.PropertyField to get the default implementation instead of getting infinite recursion.
*   Editor: New virtual method UseDefaultMargins on Editors as well as two styles in EditorStyles that can be used to customize margin use manually in custom Editors.
*   Editor: Add ability to cancel update static flags in children dialogs.
*   Editor: Made TextAsset also recognize .json, .csv, .yaml extensions.
*   Editor: Add Component menu now handles multiple search words and lists items that match all of them, so for example "ca co" lists Capsule Collider.
*   Editor: If a shader has a PreviewType=Plane tag, the material inspector will display a plane instead of 3D meshes in the preview.
*   Editor: Improve GenericMenu showing speed on Windows.
*   Editor: New commandline switch "-buildTarget " that allows to select the active build target before a project is loaded.
*   Editor: ETC2 texture formats now selectable from Texture Importer inspector.
*   Editor: Respect HideInHierarchy flag & locked layers in drag-rectangle-box picking code as well.
*   iOS: added Ad Loaded callbacks
*   iOS: Added iPhone5S/C to the iPhoneGeneration enum
*   iOS: Fixed crash if user had selected OpenGL ES 3.0 as graphics API target (GL ES 3.0 is currently Android-only)
*   iOS: Fixed some warning in Xcode project
*   iOS: Added possibility to back rendering surface with CVTextureCache-ed texture.
*   iOS: Added AppDelegateListener with notifications about Local/Remote Notifications.
*   iOS: Added joystick support skeleton.
*   iOS: Improved native code integration with Unity Trampoline, look for RenderPluginDelegate and LifeCycleDelegate.
*   iOS: Make it possible to disable rendering to external display (to revert to simple mirroring). Added c# event for Display list changes.
*   Linux: Reduce development player size
*   Linux: Added screen selector / input configurator.
*   Linux: Implemented -popupwindow command line argument.
*   Linux: Add proxy support for WWW class via HTTP\_PROXY/HTTPS\_PROXY environment variables.
*   Linux: Reduce size of development players.
*   Math: Added "IsNormalized()" method to Vector2.
*   Mecanim: \[Optimize game objects\] Add support for dynamically attaching a SkinnedMeshRenderer to an existing character (like wearing glove). As long as the SkinnedMeshRenderer and the character have the same rig, they don't need to come from the same FBX file.
*   Mecanim: \[Optimize game objects\] Add support for exposing a Transform without reimport. Just create a new game object as a child of the root game object, and rename it to be exactly the same as the bone you want to expose.
*   Mecanim: \[Optimize game objects\] Optimize and de-optimize game objects at runtime with: void OptimizeTransformHierarchy(GameObject go) and DeoptimizeTransformHierarchy(GameObject go)
*   Mecanim: \[Optimize game objects\] Work better with prefab now. De-optimizing the imported model will not break the existing prefabs.
*   Mecanim: Added a popup menu in animation clip model importer to select/deselect all nodes in the mask inspector.
*   Mecanim: AnimationController is created without file dialog when 1st animation is added to GO.
*   Mecanim: Curve editing in Animation window should be faster for controller with many clip
*   Mecanim: When draging a clip on a GO that already has an AnimationController, simply add the clip instead of creating a new controller.
*   Mecanim: Reduced memory footprint for Animator component.
*   Mecanim: Animation clip importer automaticly detect the rig type (generic or humanoid) and setup the mask accordingly.
*   Mecanim: Rewrote iOS SIMD math library backend.
*   Mecanim: Added new animation compression mode 'optimal' for generic and humanoid rig.
*   Mecanim: When dragging a non-legacy clip on a GameObject, create an Animator + controller
*   Mecanim: Refactored AvatarMask use during import. Can now specify an asset on disk.
*   Mecanim: Added warning when humanoid transforms have Translation/Scale animation.
*   Mecanim: Removed warning message when previewing some objects that have component dependency.
*   Mobile: Improved GLES context recreation
*   Mobile: Mobiles now have separate rendering path setting
*   NavMesh: To ensure correct navmesh being baked, step height is clamped to be always less than agent height, and a warning is issued to user.
*   Physics: Can now set up material for TerrainData.
*   Physics: Joints can now have separate anchor points configured for both connected rigidbodies.
*   Physics: CharacterController will now report an error when trying to configure it as a trigger.
*   Profiler: Players now include the entire frame when profiling
*   Profiler: Correct unwinding of samples if an exception is thrown
*   Profiler: Now profiles OnGUI events when profiling editor.
*   Reduced memory consumption when importing 8k\*8k textures
*   Scripting: WWW object now has a bytesDownloaded attribute, to monitor a download's activity if the remote host does not send a content-length header
*   Scripting: Add generic overloads for Resources class.
*   Terrain: Show a warning when unsupported shader is being used on terrain
*   Version Control: Create missing folder that have their .meta file present
*   Version Control: Reduced calls to VCS backend for getting status
*   Version Control: Show progress send from plugin in GUI
*   Version Control: Made a change lists optional trait for plugins
*   Version Control: Make "get latest" on asset subset or only changeset a plugin trait.
*   Version Control: Allow plugins to force handling of conflicts themselves
*   Version Control: Add support for PlasticSCM mergetool in unity preferences
*   Version Control: Support for plugin custom commands.
*   Version Control: Support for plugin provided icon overlays.
*   Version Control: Improve initial add of ProjectSettings folder to include future settings as well
*   Version Control: Show overlay legends in the settings inspector
*   Version Control: Handle files deleted externally to be reverted/deleted in vcs automatically
*   Version Control: Handle files renamed/moved outside unity and to be moved in version control as well
*   Windows Phone: Added default unity splash screens of all available orientations (landscape left, landscape right, portrait upside down in addition to portait).
*   Windows Phone: Added support for pixel perfect splashscreens.
*   Windows Phone: Debug.Log in user scripts will now output to Visual Studio output window as well if the project is built in debug and release configurations.
*   Windows Phone: If Windows Phone SDK cannot be found, its expected path is reported.
*   Windows Phone: Message box appears on the phone when using capability that was not enabled in application manifest file.
*   Windows Phone: Use latest UnityScript / Boo
*   Windows Phone: Implemented backround media player status API for Windows Phone at UnityEngine.WindowsPhone.Media.
*   Windows Phone: Show platform name in editor title.
*   Windows Phone/+ Windows Store Apps: Exposed application trial API.
*   Windows Phone: Added Emulator support.
*   Windows Store Apps: background color override support in extended splash screen on Windows 8.1
*   Windows Store Apps: Support rendering in non-native resolutions on Metro 8.1
*   Windows Store Apps - Windows 8.1: Input callbacks will now be processed on application thread instead of UI thread, thus reducing input lag.
*   Windows Store Apps - Windows 8.1: Will use Direct3D low-latency presentation API [http://msdn.microsoft.com/en-us/library/windows/apps/bg182880.aspx#five](http://msdn.microsoft.com/en-us/library/windows/apps/bg182880.aspx#five), this should improve input latency.
*   Windows Store Apps & + Windows Phone: Windows 8 requirement to build for Windows Phone/Windows Store Apps is always listed in build settings if it isn't met.
*   Windows Store Apps: Added Master configuration to the exported solution, so now there will be three - Debug, Release, Master like on Windows Phone 8. Master configuration should be used when releasing the game. Release configuration is the same as Master, but has Profiler enabled, that's the only difference.
*   Windows Store Apps: Animator.GetCurrentAnimationClipState, Animator.GetNextAnimationClipState should work now.
*   Windows Store Apps: Added UnityEngine.WSA.Application.windowsActivated event, which can be used for capturing events when snapping begins and ends.
*   Windows Store Apps: Implemented Screen.sleepTimeout
*   Windows Store Apps: Fixed some of the issues with external plugins, for ex., Facebook.dll, EasyRoads3D.dll
*   Windows Store Apps: Windows 8.1 support.
*   Windows Store Apps: Cloth is supported now.
*   Windows Store Apps: Editor will check if plugins used by Editor and Windows Store Apps are compatible, for ex., it will check if assembly version matches.
*   Windows Store Apps: Editor will perform a check if user is running under Windows 8 or higher, if not Build buttons will be disabled.
*   Windows Store Apps: Unity splash screen will be shown if user doesn't have a Pro license.
*   Windows Store Apps: Added UnityEngine.WSA.Application.windowSizeChanged event, which will be invoked when user resizes the window, for ex., when performing snaping.
*   Windows Store Apps: Implemented LocationService and Compass.
*   Windows Store Apps: Compilation Overrides will only affect C# files not located in "Standard Assets", "Pro Standard Assets" or "Plugins" folders.
*   Windows Store Apps: Managed-To-Native functions now use Platform Invoke to perform interop, performance should be better now.
*   Windows Store Apps: New APIs. UnityEngine.Windows.File, UnityEngine.Windows.Directory for accessing directories and files. UnityEngine.WSA.Application for invoking calls on different threads.
*   Windows Store Apps: Resources.UnloadUnusedAssets should work correctly now.
*   Windows Store Apps: When generating C+/C# solution, Mixed Mode debugging will be enabled by default.
*   Windows Store Apps: Make sure gui password field is drawing mask char, even though os keyboard returns clear text.