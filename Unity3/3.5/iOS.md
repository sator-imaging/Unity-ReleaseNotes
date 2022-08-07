# Unity 3.5
https://unity3d.com/unity/whats-new/unity-3.5

## iOS

<ul>
<li>Fixed appending of Xcode project when automatic native plugin inclusion is used.</li>
<li>Fixed Editor freeze when Remote Profiler is connecting to iPhone running iOS 5.0.</li>
<li>Fixed horizontal splash screen image pre-rotation to vertical orientation.</li>
<li>Fixed Mathf.Approximately and other math routines operating on de-normalized small numbers.</li>
<li>Fixed numerous iOS5 related problems (GL errors, keyboard, etc.).</li>
<li>Fixed Remote Profiler support.</li>
<li>Fixed simulator build when project has native plugins.</li>
<li>Fixed small memory leak.</li>
<li>Fixed some scary warnings in Xcode debugger console.</li>
<li>Fixed splashscreen pre-rotation when autorotation is enabled.</li>
<li>Fixed WebCamTexture.GetPixels.</li>
<li>icon-iPad.png renamed to icon-72.png.</li>
<li>SystemInfo.systemMemorySize returns correct memory size, SystemInfo.graphicsMemorySize is now estimated based on total memory size.</li>
<li>SystemLanguage handling overhaul - now region is correctly recognized (e.g. British English will result in English instead of Unknown).</li>
<li>Improved .NET 2.0 full profile out of the box compatibility with WebRequest API. Managed code stripping still needs manual care.</li>
</ul>

### Javascript
<ul>
<li>Fixed bug that would cause a for loop not to reuse an already declared variable.</li>
<li>Fixed multidimensional array of struct operations.</li>
<li>Script attributes can now appear before 'import' statements.</li>
</ul>

### Mac OS X
<ul>
<li>Mac OS X Editor: Properly recognize user setting to launch Editor in a specific Space/Desktop.</li>
<li>Mac OS X Standalone: Fixed mouse down events being reported for clicks on window title bar.</li>
<li>Mac OS X Standalone: Will not show window restore dialog and crash in OS X Lion.</li>
<li>Mac OS X Standalone: Don't quit, if cancel button was pressed during Quit dialog in windowed mode.</li>
<li>Mac OS X Web Player: Fixed a crash in Firefox 6 when loading Unity content in a background tab.</li>
<li>Mac OS X Web Player: Fixed a crash in Firefox 7 when resizing Unity content.</li>
<li>Mac OS X Web Player: Fixed scroll wheel events in full-screen mode in CoreAnimation plugin.</li>
<li>Mac OS X Web Player: IME input is now recognized in the OS X WebPlayer.</li>
<li>Mac OS X Web Player: Input.inputString will correctly contain backspace and delete characters.</li>
<li>Mac OS X Web Player: Make mouse input handling more robust. Fixes Magic Trackpad support in Safari 5.1.</li>
<li>Mac OS X: Fixed input from some gamepad hat switches.</li>
<li>Mac OS X: Fixed distinguishing between left and right modifier keys in the Input class.</li>
<li>Mac OS X: SystemInfo now returns actual device information.</li>
<li>Mac Web Player: Fixed different rendering issues when using image effects.</li>
</ul>

### Windows
<ul>
<li>Windows 64-bit standalone: Fixed setting executable icon.</li>
<li>Windows Fixed skinned meshes disappearing temporarily when returning from sleep mode or from locking computer.</li>
<li>Windows Web Player: Fixed occasionally corrupted graphics when locking computer or switching resolution during loading.</li>
<li>Windows: Focus is not lost when Web Player enters or exits fullscreen mode.</li>
<li>Windows: Joystick 0 now returns correct cumulative axes values.</li>
</ul>

### Physics
<ul>
<li>Collider.bounds will now alway return empty bounds for disabled colliders (before it was inconsistent by collider type).Fixed behavior of rotated capsule colliders when continuous collision detection is used.</li>
<li>Fixed CCD not working in first level of a game.</li>
<li>Fixed crash when disabling a CharacterController inside a CharacterController callback.</li>
<li>Fixed slow duplicate creation of colliders when using GameObject.SetActiveRecursively().</li>
<li>Physics contact count is now correctly reported in the Profiler, and will not appear to increment indefinitely.</li>
<li>Removed "Solver rigidbodies" field in physics profiler, as it did not do anything.</li>
<li>Fixed a crash when creating a Terrain with too many Tree colliders.</li>
</ul>

### Miscellaneous
<ul>
<li>Asset Server: Fixed a bug that caused a crash when reverting a project setting to an older version in the Asset Server history view.</li>
<li>Asset Server: Local project settings no longer show up as conflicts when checking out new projects.</li>
<li>AssetBundles: Fixed AssetBundle.mainAsset loading all dependencies of the mainAsset.</li>
<li>AssetBundles: Fixed a crash sometimes caused by simultaneously downloading multiple asset bundles with caching enabled.</li>
<li>Asset Import: Fixed crash when selecting asset with name including ".."</li>
<li>Asset Import: Fixed an issue causing animations including scaling to (0,0,0) to be imported as having extremely large bounding boxes, which in turn caused issues with shadows and culling.</li>
<li>AssetStore: Fixed crash when exiting Unity or switching projects while the Asset Store window was loading a page.</li>
<li>Execution order for prefabs is now 100% consistent. It works exactly the same as having non-prefab objects (Removes superfluos OnDisable / OnEnable calls).</li>
<li>Fixed a synchronization issue between Renderthread and GPU. This has fixed the stuttering and reduced the input lag.</li>
<li>Fixed an issue that caused the editor to freeze if left in the background with the profiler open.</li>
<li>Fixed AsyncOperation.progress to properly indicate loading progress.</li>
<li>Fixed font kerning when using GUIStyle.fontSize.</li>
<li>Fixed path names for Cache and Application.persistentDataPath not to be garbled up. If old path names are present, they will still be used.</li>
<li>Made Assembly.Location return actual location of the assembly and not "data-09340sdf9gsd0fg".</li>
<li>Made FindObjectsOfType not return Cubemaps when searching for Texture2D.</li>
<li>MonoDevelop: Fixed unhandled exception when attaching debugger.</li>
<li>MonoDevelop: More robust script encoding detection.</li>
<li>MonoDevelop: Don't open script projects twice.</li>
<li>MonoDevelop: Ensure selected script gains focus.</li>
<li>Networking: Fixed case where NetworkView state synchronization was not relayed properly through a proxy connection.</li>
<li>Networking: Fixed cases where connection tester failed to return a result.</li>
<li>Networking: Fixed crash when reading NetworkPlayer.guid when networking was not initialized.</li>
<li>Networking: Fixed possible crash when reading NetworkMessageInfo.networkView inside OnNetworkInstantiate.</li>
<li>Networking: Fixed problems with built-in multiplayer networking on Windows when using VPN/proxy software which manipulates traffic coming from the browser. DNS and interface IP address lookup are now done differently.</li>
<li>Occlusion culling: Fixed several out of memory issues, made many occlusion accuracy improvements.</li>
<li>Profiler: GPU profiler now shows better info on image effects.</li>
<li>Profiler: More reliable player connection discovery.</li>
<li>Profiler: Not sending instance Ids back, since these don't match the instance Ids of the editor - caused detail view to display wrong instance names.</li>
<li>Script: Fixed crash when reparenting GameObjects durring Scene Destroy.</li>
<li>Substance: Fixed crash after modification(resizing and etc.) of texture parameters.</li>
<li>We no longer get send multiple mousedown / mouse up while hovering over an object.</li>
<li>WebPlayer and Standalone: Return correct Event.delta value on Windows.</li>
<li>WebPlayer: Fixed memory leak on windows when unloading.</li>
<li>WebPlayer: Reduced visual artifacts produced when WebPlayer size is changed on Windows.</li>
</ul>
