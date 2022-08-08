# Unity 3.5

https://unity3d.com/unity/whats-new/unity-3.5

## iOS

- [Javascript](#javascript)
- [Mac OS X](#mac-os-x)
- [Windows](#windows)
- [Physics](#physics)
- [Miscellaneous](#miscellaneous)


*   Fixed appending of Xcode project when automatic native plugin inclusion is used.
*   Fixed Editor freeze when Remote Profiler is connecting to iPhone running iOS 5.0.
*   Fixed horizontal splash screen image pre-rotation to vertical orientation.
*   Fixed Mathf.Approximately and other math routines operating on de-normalized small numbers.
*   Fixed numerous iOS5 related problems (GL errors, keyboard, etc.).
*   Fixed Remote Profiler support.
*   Fixed simulator build when project has native plugins.
*   Fixed small memory leak.
*   Fixed some scary warnings in Xcode debugger console.
*   Fixed splashscreen pre-rotation when autorotation is enabled.
*   Fixed WebCamTexture.GetPixels.
*   icon-iPad.png renamed to icon-72.png.
*   SystemInfo.systemMemorySize returns correct memory size, SystemInfo.graphicsMemorySize is now estimated based on total memory size.
*   SystemLanguage handling overhaul - now region is correctly recognized (e.g. British English will result in English instead of Unknown).
*   Improved .NET 2.0 full profile out of the box compatibility with WebRequest API. Managed code stripping still needs manual care.

### Javascript

*   Fixed bug that would cause a for loop not to reuse an already declared variable.
*   Fixed multidimensional array of struct operations.
*   Script attributes can now appear before 'import' statements.

### Mac OS X

*   Mac OS X Editor: Properly recognize user setting to launch Editor in a specific Space/Desktop.
*   Mac OS X Standalone: Fixed mouse down events being reported for clicks on window title bar.
*   Mac OS X Standalone: Will not show window restore dialog and crash in OS X Lion.
*   Mac OS X Standalone: Don't quit, if cancel button was pressed during Quit dialog in windowed mode.
*   Mac OS X Web Player: Fixed a crash in Firefox 6 when loading Unity content in a background tab.
*   Mac OS X Web Player: Fixed a crash in Firefox 7 when resizing Unity content.
*   Mac OS X Web Player: Fixed scroll wheel events in full-screen mode in CoreAnimation plugin.
*   Mac OS X Web Player: IME input is now recognized in the OS X WebPlayer.
*   Mac OS X Web Player: Input.inputString will correctly contain backspace and delete characters.
*   Mac OS X Web Player: Make mouse input handling more robust. Fixes Magic Trackpad support in Safari 5.1.
*   Mac OS X: Fixed input from some gamepad hat switches.
*   Mac OS X: Fixed distinguishing between left and right modifier keys in the Input class.
*   Mac OS X: SystemInfo now returns actual device information.
*   Mac Web Player: Fixed different rendering issues when using image effects.

### Windows

*   Windows 64-bit standalone: Fixed setting executable icon.
*   Windows Fixed skinned meshes disappearing temporarily when returning from sleep mode or from locking computer.
*   Windows Web Player: Fixed occasionally corrupted graphics when locking computer or switching resolution during loading.
*   Windows: Focus is not lost when Web Player enters or exits fullscreen mode.
*   Windows: Joystick 0 now returns correct cumulative axes values.

### Physics

*   Collider.bounds will now alway return empty bounds for disabled colliders (before it was inconsistent by collider type).Fixed behavior of rotated capsule colliders when continuous collision detection is used.
*   Fixed CCD not working in first level of a game.
*   Fixed crash when disabling a CharacterController inside a CharacterController callback.
*   Fixed slow duplicate creation of colliders when using GameObject.SetActiveRecursively().
*   Physics contact count is now correctly reported in the Profiler, and will not appear to increment indefinitely.
*   Removed "Solver rigidbodies" field in physics profiler, as it did not do anything.
*   Fixed a crash when creating a Terrain with too many Tree colliders.

### Miscellaneous

*   Asset Server: Fixed a bug that caused a crash when reverting a project setting to an older version in the Asset Server history view.
*   Asset Server: Local project settings no longer show up as conflicts when checking out new projects.
*   AssetBundles: Fixed AssetBundle.mainAsset loading all dependencies of the mainAsset.
*   AssetBundles: Fixed a crash sometimes caused by simultaneously downloading multiple asset bundles with caching enabled.
*   Asset Import: Fixed crash when selecting asset with name including ".."
*   Asset Import: Fixed an issue causing animations including scaling to (0,0,0) to be imported as having extremely large bounding boxes, which in turn caused issues with shadows and culling.
*   AssetStore: Fixed crash when exiting Unity or switching projects while the Asset Store window was loading a page.
*   Execution order for prefabs is now 100% consistent. It works exactly the same as having non-prefab objects (Removes superfluos OnDisable / OnEnable calls).
*   Fixed a synchronization issue between Renderthread and GPU. This has fixed the stuttering and reduced the input lag.
*   Fixed an issue that caused the editor to freeze if left in the background with the profiler open.
*   Fixed AsyncOperation.progress to properly indicate loading progress.
*   Fixed font kerning when using GUIStyle.fontSize.
*   Fixed path names for Cache and Application.persistentDataPath not to be garbled up. If old path names are present, they will still be used.
*   Made Assembly.Location return actual location of the assembly and not "data-09340sdf9gsd0fg".
*   Made FindObjectsOfType not return Cubemaps when searching for Texture2D.
*   MonoDevelop: Fixed unhandled exception when attaching debugger.
*   MonoDevelop: More robust script encoding detection.
*   MonoDevelop: Don't open script projects twice.
*   MonoDevelop: Ensure selected script gains focus.
*   Networking: Fixed case where NetworkView state synchronization was not relayed properly through a proxy connection.
*   Networking: Fixed cases where connection tester failed to return a result.
*   Networking: Fixed crash when reading NetworkPlayer.guid when networking was not initialized.
*   Networking: Fixed possible crash when reading NetworkMessageInfo.networkView inside OnNetworkInstantiate.
*   Networking: Fixed problems with built-in multiplayer networking on Windows when using VPN/proxy software which manipulates traffic coming from the browser. DNS and interface IP address lookup are now done differently.
*   Occlusion culling: Fixed several out of memory issues, made many occlusion accuracy improvements.
*   Profiler: GPU profiler now shows better info on image effects.
*   Profiler: More reliable player connection discovery.
*   Profiler: Not sending instance Ids back, since these don't match the instance Ids of the editor - caused detail view to display wrong instance names.
*   Script: Fixed crash when reparenting GameObjects durring Scene Destroy.
*   Substance: Fixed crash after modification(resizing and etc.) of texture parameters.
*   We no longer get send multiple mousedown / mouse up while hovering over an object.
*   WebPlayer and Standalone: Return correct Event.delta value on Windows.
*   WebPlayer: Fixed memory leak on windows when unloading.
*   WebPlayer: Reduced visual artifacts produced when WebPlayer size is changed on Windows.