# Unity 4.3
https://unity3d.com/unity/whats-new/unity-4.3

## Improvements

<ul>
<li>AI / NavMesh: Performance! Crowd update is multithreaded when there are more than 50 active navmesh agents - if supported by device.</li>
<li>AI / NavMesh: Obstacle carving support. NavMeshObstacle supports carving via the "Carve" flag on the component.</li>
<li>AI / NavMesh: OffMeshLink Component is dynamic. OffMeshLink component creation/modification/destruction has effect at runtime and in the editor. No baking of navmesh is required.</li>
<li>AI / NavMesh: 'CalculateTriangulation' calculates and returns a simple triangulation of the current navigation mesh. Returned is a struct containing the vertices, triangle indices and navmesh layers.</li>
<li>AI / NavMesh: OffMeshLink Component API additions: navMeshLayer, biDirectional, startTransform, endTransform, autoUpdatePositions, UpdatePosition.</li>
<li>Android: Always use non-linear z if available for 16 bit depth buffers</li>
<li>Android: Joystick input should now be more concise across different gamepads and devices.</li>
<li>Android: Support for secondary and tertiary mouse button (requires ICS).</li>
<li>Android: GL context recreation will only take place when strictly needed.</li>
<li>Android: Better EGL context selection. Now much more likely to pick a configuration with proper anti aliasing, stencil, depth etc.</li>
<li>Android: Native EGL/OpenGLES (no longer initialized through Java).</li>
<li>Animation Window: New clips are saved into project browser active folder instead of project root by default.</li>
<li>Animation Window: Recording goes through the new Undo system. Only changes that are Undoable are recorded.</li>
<li>Animation Window: Hotkey 'k' for add keyframe button.</li>
<li>Animation Window: Properties that are being animated show up in yellow.</li>
<li>BlackBerry: Added checkbox to allow users to indicate Gamepad support for their games</li>
<li>BlackBerry: It is now possible to specify build ID.</li>
<li>BlackBerry: Gamepad trigger buttons are now supported.</li>
<li>Documentation: undocumented APIs will now show up as empty stubs</li>
<li>Documentation: more Scripting docs for 2D APIs</li>
<li>DX11: Use new fixed function shader generator on Windows 8.1</li>
<li>Editor: Improve workflow when layout with custom windows failed to load due to compile errors.</li>
<li>Editor: Modified occlusion culling default baking parameters (smallest occluder value 1.0 -&gt; 5.0)</li>
<li>Editor: No longer downloads an ivy.xml file every time you push play.</li>
<li>Editor: Removed dysfunctional Xcode 4 setting</li>
<li>Editor: Updated Unity Logo and icons</li>
<li>Editor: Better performance when entering and exiting playmode</li>
<li>Editor: Improved search in Project Browser and Hierarchy: We now support searching for types in namespaces and base types can be used to find derived types.</li>
<li>Editor: Improve error handling of renaming/creating assets when inputing invalid file name chars</li>
<li>Editor: SHIFT+F or double-F locks the scene view camera to the selected GameObject.</li>
<li>Editor: "alpha is transparency" textures are displayed with a checker background in material inspector; and nicer display in project browser.</li>
<li>Editor: Optimize Inspector GUI by avoiding much of the string handling associated with PropertyDrawers.</li>
<li>Editor: Order and group menu items in Assets/Create menu so related items are together.</li>
<li>Editor: PropertyDrawers now have a fieldInfo property that can be used to obtain reflection data about the member that the property represents.</li>
<li>Editor: PropertyDrawers can now call EditorGUI.PropertyField to get the default implementation instead of getting infinite recursion.</li>
<li>Editor: New virtual method UseDefaultMargins on Editors as well as two styles in EditorStyles that can be used to customize margin use manually in custom Editors.</li>
<li>Editor: Add ability to cancel update static flags in children dialogs.</li>
<li>Editor: Made TextAsset also recognize .json, .csv, .yaml extensions.</li>
<li>Editor: Add Component menu now handles multiple search words and lists items that match all of them, so for example "ca co" lists Capsule Collider.</li>
<li>Editor: If a shader has a PreviewType=Plane tag, the material inspector will display a plane instead of 3D meshes in the preview.</li>
<li>Editor: Improve GenericMenu showing speed on Windows.</li>
<li>Editor: New commandline switch "-buildTarget " that allows to select the active build target before a project is loaded.</li>
<li>Editor: ETC2 texture formats now selectable from Texture Importer inspector.</li>
<li>Editor: Respect HideInHierarchy flag &amp; locked layers in drag-rectangle-box picking code as well.</li>
<li>iOS: added Ad Loaded callbacks</li>
<li>iOS: Added iPhone5S/C to the iPhoneGeneration enum</li>
<li>iOS: Fixed crash if user had selected OpenGL ES 3.0 as graphics API target (GL ES 3.0 is currently Android-only)</li>
<li>iOS: Fixed some warning in Xcode project</li>
<li>iOS: Added possibility to back rendering surface with CVTextureCache-ed texture.</li>
<li>iOS: Added AppDelegateListener with notifications about Local/Remote Notifications.</li>
<li>iOS: Added joystick support skeleton.</li>
<li>iOS: Improved native code integration with Unity Trampoline, look for RenderPluginDelegate and LifeCycleDelegate.</li>
<li>iOS: Make it possible to disable rendering to external display (to revert to simple mirroring). Added c# event for Display list changes.</li>
<li>Linux: Reduce development player size</li>
<li>Linux: Added screen selector / input configurator.</li>
<li>Linux: Implemented -popupwindow command line argument.</li>
<li>Linux: Add proxy support for WWW class via HTTP_PROXY/HTTPS_PROXY environment variables.</li>
<li>Linux: Reduce size of development players.</li>
<li>Math: Added "IsNormalized()" method to Vector2.</li>
<li>Mecanim: [Optimize game objects] Add support for dynamically attaching a SkinnedMeshRenderer to an existing character (like wearing glove). As long as the SkinnedMeshRenderer and the character have the same rig, they don't need to come from the same FBX file.</li>
<li>Mecanim: [Optimize game objects] Add support for exposing a Transform without reimport. Just create a new game object as a child of the root game object, and rename it to be exactly the same as the bone you want to expose.</li>
<li>Mecanim: [Optimize game objects] Optimize and de-optimize game objects at runtime with: void OptimizeTransformHierarchy(GameObject go) and DeoptimizeTransformHierarchy(GameObject go)</li>
<li>Mecanim: [Optimize game objects] Work better with prefab now. De-optimizing the imported model will not break the existing prefabs.</li>
<li>Mecanim: Added a popup menu in animation clip model importer to select/deselect all nodes in the mask inspector.</li>
<li>Mecanim: AnimationController is created without file dialog when 1st animation is added to GO.</li>
<li>Mecanim: Curve editing in Animation window should be faster for controller with many clip</li>
<li>Mecanim: When draging a clip on a GO that already has an AnimationController, simply add the clip instead of creating a new controller.</li>
<li>Mecanim: Reduced memory footprint for Animator component.</li>
<li>Mecanim: Animation clip importer automaticly detect the rig type (generic or humanoid) and setup the mask accordingly.</li>
<li>Mecanim: Rewrote iOS SIMD math library backend.</li>
<li>Mecanim: Added new animation compression mode 'optimal' for generic and humanoid rig.</li>
<li>Mecanim: When dragging a non-legacy clip on a GameObject, create an Animator + controller</li>
<li>Mecanim: Refactored AvatarMask use during import. Can now specify an asset on disk.</li>
<li>Mecanim: Added warning when humanoid transforms have Translation/Scale animation.</li>
<li>Mecanim: Removed warning message when previewing some objects that have component dependency.</li>
<li>Mobile: Improved GLES context recreation</li>
<li>Mobile: Mobiles now have separate rendering path setting</li>
<li>NavMesh: To ensure correct navmesh being baked, step height is clamped to be always less than agent height, and a warning is issued to user.</li>
<li>Physics: Can now set up material for TerrainData.</li>
<li>Physics: Joints can now have separate anchor points configured for both connected rigidbodies.</li>
<li>Physics: CharacterController will now report an error when trying to configure it as a trigger.</li>
<li>Profiler: Players now include the entire frame when profiling</li>
<li>Profiler: Correct unwinding of samples if an exception is thrown</li>
<li>Profiler: Now profiles OnGUI events when profiling editor.</li>
<li>Reduced memory consumption when importing 8k*8k textures</li>
<li>Scripting: WWW object now has a bytesDownloaded attribute, to monitor a download's activity if the remote host does not send a content-length header</li>
<li>Scripting: Add generic overloads for Resources class.</li>
<li>Terrain: Show a warning when unsupported shader is being used on terrain</li>
<li>Version Control: Create missing folder that have their .meta file present</li>
<li>Version Control: Reduced calls to VCS backend for getting status</li>
<li>Version Control: Show progress send from plugin in GUI</li>
<li>Version Control: Made a change lists optional trait for plugins</li>
<li>Version Control: Make "get latest" on asset subset or only changeset a plugin trait.</li>
<li>Version Control: Allow plugins to force handling of conflicts themselves</li>
<li>Version Control: Add support for PlasticSCM mergetool in unity preferences</li>
<li>Version Control: Support for plugin custom commands.</li>
<li>Version Control: Support for plugin provided icon overlays.</li>
<li>Version Control: Improve initial add of ProjectSettings folder to include future settings as well</li>
<li>Version Control: Show overlay legends in the settings inspector</li>
<li>Version Control: Handle files deleted externally to be reverted/deleted in vcs automatically</li>
<li>Version Control: Handle files renamed/moved outside unity and to be moved in version control as well</li>
<li>Windows Phone: Added default unity splash screens of all available orientations (landscape left, landscape right, portrait upside down in addition to portait).</li>
<li>Windows Phone: Added support for pixel perfect splashscreens.</li>
<li>Windows Phone: Debug.Log in user scripts will now output to Visual Studio output window as well if the project is built in debug and release configurations.</li>
<li>Windows Phone: If Windows Phone SDK cannot be found, its expected path is reported.</li>
<li>Windows Phone: Message box appears on the phone when using capability that was not enabled in application manifest file.</li>
<li>Windows Phone: Use latest UnityScript / Boo</li>
<li>Windows Phone: Implemented backround media player status API for Windows Phone at UnityEngine.WindowsPhone.Media.</li>
<li>Windows Phone: Show platform name in editor title.</li>
<li>Windows Phone/+ Windows Store Apps: Exposed application trial API.</li>
<li>Windows Phone: Added Emulator support.</li>
<li>Windows Store Apps: background color override support in extended splash screen on Windows 8.1</li>
<li>Windows Store Apps: Support rendering in non-native resolutions on Metro 8.1</li>
<li>Windows Store Apps - Windows 8.1: Input callbacks will now be processed on application thread instead of UI thread, thus reducing input lag.</li>
<li>Windows Store Apps - Windows 8.1: Will use Direct3D low-latency presentation API <a href="http://msdn.microsoft.com/en-us/library/windows/apps/bg182880.aspx#five">http://msdn.microsoft.com/en-us/library/windows/apps/bg182880.aspx#five</a>, this should improve input latency.</li>
<li>Windows Store Apps &amp; + Windows Phone: Windows 8 requirement to build for Windows Phone/Windows Store Apps is always listed in build settings if it isn't met.</li>
<li>Windows Store Apps: Added Master configuration to the exported solution, so now there will be three - Debug, Release, Master like on Windows Phone 8. Master configuration should be used when releasing the game. Release configuration is the same as Master, but has Profiler enabled, that's the only difference.</li>
<li>Windows Store Apps: Animator.GetCurrentAnimationClipState, Animator.GetNextAnimationClipState should work now.</li>
<li>Windows Store Apps: Added UnityEngine.WSA.Application.windowsActivated event, which can be used for capturing events when snapping begins and ends.</li>
<li>Windows Store Apps: Implemented Screen.sleepTimeout</li>
<li>Windows Store Apps: Fixed some of the issues with external plugins, for ex., Facebook.dll, EasyRoads3D.dll</li>
<li>Windows Store Apps: Windows 8.1 support.</li>
<li>Windows Store Apps: Cloth is supported now.</li>
<li>Windows Store Apps: Editor will check if plugins used by Editor and Windows Store Apps are compatible, for ex., it will check if assembly version matches.</li>
<li>Windows Store Apps: Editor will perform a check if user is running under Windows 8 or higher, if not Build buttons will be disabled.</li>
<li>Windows Store Apps: Unity splash screen will be shown if user doesn't have a Pro license.</li>
<li>Windows Store Apps: Added UnityEngine.WSA.Application.windowSizeChanged event, which will be invoked when user resizes the window, for ex., when performing snaping.</li>
<li>Windows Store Apps: Implemented LocationService and Compass.</li>
<li>Windows Store Apps: Compilation Overrides will only affect C# files not located in "Standard Assets", "Pro Standard Assets" or "Plugins" folders.</li>
<li>Windows Store Apps: Managed-To-Native functions now use Platform Invoke to perform interop, performance should be better now.</li>
<li>Windows Store Apps: New APIs. UnityEngine.Windows.File, UnityEngine.Windows.Directory for accessing directories and files. UnityEngine.WSA.Application for invoking calls on different threads.</li>
<li>Windows Store Apps: Resources.UnloadUnusedAssets should work correctly now.</li>
<li>Windows Store Apps: When generating C+/C# solution, Mixed Mode debugging will be enabled by default.</li>
<li>Windows Store Apps: Make sure gui password field is drawing mask char, even though os keyboard returns clear text.</li>
</ul>
