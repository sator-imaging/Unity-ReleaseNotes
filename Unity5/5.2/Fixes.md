# Unity 5.2

https://unity3d.com/unity/whats-new/unity-5.2

## Fixes

- [2D Fixes](#2d-fixes)
- [Android Fixes](#android-fixes)
- [Editor Fixes](#editor-fixes)
- [Graphics, Lightmapping and Shader Fixes](#graphics-lightmapping-and-shader-fixes)
- [Mecanim Fixes](#mecanim-fixes)
- [Physics Fixes](#physics-fixes)
- [Scripting, Mono and IL2CPP Fixes](#scripting-mono-and-il2cpp-fixes)
- [UI Fixes](#ui-fixes)
- [WebGL Fixes](#webgl-fixes)
- [Other Fixes](#other-fixes)


### 2D Fixes

*   After applying settings in sprite editor window, deselect any sprite rect.
*   Apply active color space onto texture in sprite editor.
*   Clear undos for SpriteEditorWindow when applying or window is closed. Also fix ClearUndo not working for ObjectUndo.
*   Do not trim sprite when Shift-T is pressed while entering name in Sprite Editor.
*   Ensure SpriteEditorWindow has the correct texture importer reference when texture importer inspector is applying changes
*   Fix NullReferenceException when creating a new sceneview
*   Fix pointer enter/exit detection order with sorting layers
*   Hide PerRendererData shader properties in inspector as property is retrieved from the renderer
*   Increase responsiveness of Sprite Editor in Mac OS X
*   Materials become transparent because of improper re-setting of material
*   Non-sprite textures will display in sprite editor window with no options
*   Quit 2D collider editing mode when user reset the collider component
*   Reimport texture if texture importer is reset
*   Remove a sprite rect if the selected sprite rect is empty when trimmed
*   Replaced assert with warning message to multiple materials in SpriteRenderer
*   Set correct zoom values for zoom bar in SpriteUtilityWindow
*   Set SpriteRenderer to dirty when color is set
*   Sprite Editor uses the actual image size for slicing operation. Force Sprite Editor preview to use mipmap if user machine does not support the image resolution
*   Sprite Packer no longer packs Truecolor sprites into the same Atlas if other format settings are different
*   Update sorting layer APIs and prevent setting invalid sorting layer ids to renderer
*   View tool (panning, rotating, zooming) in the scene view will not manipulate collider control point even in collider editing mode

### Android Fixes

*   Android: Added API level 22 to the minSdk list
*   Android: Added support to create a real 16bit RGB565 backbuffer. Deprecated Handheld.use32BitDisplayBuffer
*   Android: Audio - Fixed issues on GearVR when the device does not report FEATURE\_AUDIO\_LOW\_LATENCY
*   Android: Buildpipe - Android Libraries can now be excluded from build in the Plugin Inspector
*   Android: Buildpipe - Fixed assets folders in aar files
*   Android: Fixed ATC texture compression for RGBA textures
*   Android: Fixed bug that caused texture format RGBA4444 to be used for RGBA textures even when overriding in build settings
*   Android: Fixed crash affecting some PowerVR 544 devices
*   Android: Fixed performance regression in Resource.Load when calling it multiple times for the same resource
*   Android: JNI - fixed long data type
*   Android: Stripping - don't strip AssetBundle class or it removes LoadAssetAsync
*   Android: WWW - report HTTP status and response in case of failure

### Editor Fixes

*   Animation Window: Animated particle properties are now show up in red in Inspector
*   Animation Window: Animated property values are now updated in Particle Editor when scrubbing in Animation Window
*   Animation Window: Animation curve now updates after changing controller
*   Animation Window: Ctrl+A now selects all keys and properties
*   Animation Window: Highlight is now blue when selecting all properties from animation window
*   Animation Window: It’s now possible to move current time before the first key
*   Animation Window: Replacing existing animation now actually replaces the asset instead of creating new one with unique name
*   Automatically checkout ProjectSettings/ProjectVersion.txt if needed
*   Avoid division by zero in zero-sized SphereCollider
*   Avoid locking when framing terrain
*   Camera lock keeps working when dragging outside the scene view window
*   Clear old main menus on Windows
*   Dirty materials when fixing HDR texture to ensure previews are updated
*   Ensure selected asset is revealed in project browser when changing layout
*   Fix asset store preview blinking in the project browser
*   Fix camera frustum gizmo not properly showing custom projection matrices
*   Fix CapsuleCollider gizmo handles are offset by a 90 degree angle
*   Fix caret not moving in ObjectSelector when using left/right arrow keys (only when no items were selected)
*   Fix crash when deleting an object from a prefab instance where the prefab asset is missing
*   Fix creating a script from the right click menu throws "Rename not started" error
*   Fix creating new assets after deletion of assets would throw error
*   Fix Cursor flickering in editor while play testing if cursor.visible = false
*   Fix Cursor.visible not working until the game view is focused
*   Fix disabled scrollbar in lighting window lightmaps tab
*   Fix error when renaming items in project and hierarchy views
*   Fix Hierarchy type searching so 't:script' or 't:monobehaviour' shows all game objects with scripts attached
*   Fix icons in Project Browser 'jumping' when changing view
*   Fix IMGUI brightness on GameView when in Linear color space
*   Fix memory thrashing when Dragging and Dropping between panels, when the dragged object had a CustomEditor with no Preview
*   Fix multi-object selection of reflection probe cubemap to not incorrectly set same cubemaps
*   Fix non character keys being mixed up with character keys on shortcuts
*   Fix not being able to focus tabs after changing "Output" on Audio Source
*   Fix occasional recycle bin bypassing when deleting assets on Windows
*   Fix popped out container window not able to move when two editor windows are stacked one above/next to the other
*   Fix possible data loss on Windows when renaming folder with locked files
*   Fix rare case of invalid folder path shown in the Project Browser
*   Fix scene view window still being tinted in playmode when an overlay was active
*   Fix scene's GI is not updated after building AssetBundle or opening the same scene
*   Fixed bug which caused the Move Tool, when used on an object with a negatively scaled parent, to snap to whole units
*   Fixed Gradient not updating when an Undo is performed
*   Fixed occasional exception thrown when creating an asset/folder under Assets folder in Project pane with One Column Layout
*   Fixed Scene View audio play toggle not returning to previous state after exiting Play Mode
*   Fixed Scene View camera moving slightly while holding down right mouse button
*   In play mode, tick one more frame after the editor is not active, so that the game can get a chance to respond to being paused
*   Make sure GUISkin.current is set to GameSkin before invoking any user script
*   Scene view picking works when selection base object isn't under the mouse position
*   Terrain editor hotkeys no longer conflict with text field input

### Graphics, Lightmapping and Shader Fixes

*   GI: Ambient GI value not changing based on disabled realtime/baked GI
*   GI: Fix crash following lighting builds in GetSystemTexture
*   GI: Fixed bake getting stuck on some terrains
*   GI: Fixed crash in CreateSnapshotForReflectionProbe when trying to rebake reflection probes
*   GI: Fixed environment reflection cubemap getting unloaded after the scene was loaded using Application.LoadLevel for scenes that used the Auto lighting build mode
*   GI: Fixed lightmap shader variant stripping for realtime lightmaps. Now each lightmaps mode (non-directional, directional and directional specular) variant can be picked for baked and realtime GI separately. Please review your settings if you selected a specific lightmaps mode variant in the Graphics Settings to make that mode work for realtime lightmaps
*   GI: Fixed radiosity core corruption error when baking lightmap
*   GI: Fixed UV packing for baked UVs not filling the 0-1 space (smaller or bigger). Fixes a bunch of issues where one object with stray UVs could overlap other objects and cause dark spots. Also makes the resolution assigned to each object work much more reliably if that object's unwrap is not filling the 0-1 space and also when its bounds are non-square. Please review the resolution on your instances for baked lightmaps
*   GI: Lightmap snapshot gets cleared when clearing GI Cache
*   Graphics: Crunch texture compression support for 8192x8192 textures (64-bit editor builds only)
*   Graphics: Apply hard limit on font size of 500 in more places than just font importer
*   Graphics: Fix for asset bundle content changes between subsequent generations due to uninitialised vertex buffer
*   Graphics: Fix for call to OpenGL ES API without current context when using the multi-threaded renderer
*   Graphics: Fixed a shader compiler error on OpenGL ES platforms where dot() between a vec3 and a float would fail to add an upcast
*   Graphics: Fixed bug in ES 3 shader code generator that caused clipping problems in UI shaders
*   Graphics: Fixed crash while using -force-gles on Mac OS X
*   Graphics: Fixed editor rendering black views when running with OpenGL ES 2.0
*   Graphics: Fixed Halo errors when they are on DontDestroyOnLoad objects
*   Graphics: Fixed Halo texture not being centered, causing half-texel clipping on top/right sides
*   Graphics: Fixed issue with MaterialPropertyBlock not working with Particles
*   Graphics: Fixed material keywords and renderQueue not copied over by new Material(material) constructor and Material.CopyPropertiesFromMaterial
*   Graphics: Fixed MSAA initialization on older Android devices which only support multisampled\_render\_to\_texture
*   Graphics: Fixed spamming error message importing an EXR file as sprite
*   OpenGL core: Fixed crash when using -force-glcore on Mac OS X where it's not yet supported
*   OpenGL core: Fixed Radeon HD 2000 - 4000 support
*   OpenGL core: Gracefully fallback to D3D when requesting OpenGL/ES with -force-gl\*\* when the platform doesn't have a good enough OpenGL support
*   OpenGL ES: Fixed blit from backbuffer into RenderTexture
*   OpenGL ES: Fixed Fire HD development player crash
*   OpenGL ES: Fixed crash with dynamic batching of empty meshes
*   OpenGL: Always rely GL\_EXT/IMG\_multisampled\_render\_to\_texture when available to save a lot of bandwidth when using MSAA
*   OpenGL: Resolved various invalid operation / enum errors due to platform compatibility issues
*   Particles: Fixed culling issues when particles are set from script
*   Particles: Fixed curve editor preview not updating after undo
*   Particles: Fixed Limit Velocity over Lifetime being framerate-dependent
*   Particles: Fixed prewarming performance problems
*   Particles: Fixed some spawn parameters not being random enough
*   Particles: Fixed StartDelay not working from script
*   Particles: Fixed sub-emitters sometimes not firing
*   Particles: Fixed various crashes
*   Shaders: Fixed some cases of objects with unsupported shaders not rendering at all (instead of rendering in pink)
*   Shaders: Fixed some loop constructs being translated wrongly for GLSL/Metal

### Mecanim Fixes

*   Deprecated legacy culling modes BasedOnUserBounds and BasedOnClipBounds
*   Do not activate runtime State parameter on parameter rename
*   Fixed "Cleaning up leaked objects" message after using the Avatar Configure Tool
*   Fixed a bug where it would not be possible to animate the second material on a meshrenderer
*   Fixed a bug where the lock button on the Animator Window would reset after play mode
*   Fixed a case where going to play mode would prevent undo operations from being pushed
*   Fixed an editor performance issue with large blend trees
*   Fixed an error where transitions would disappear if a controller was edited without saving immediately after upgrade from 4.x to 5.x
*   Fixed an undo error in the blend tree inspector
*   Fixed an undo related crash
*   Fixed Animator.speed set in Start() not working
*   Fixed asserts with empty controller
*   Fixed Asset Store preview of Humanoid character
*   Fixed Avatar Configure broken ResetPose when OptmizeGameObject is on
*   Fixed Blend tree max/min thresholds not being updated when changed through dragging on the graph in the inspector
*   Fixed broken BlendTree slider with some BlendTree configuration
*   Fixed broken BlendTrees with identical negative blend values
*   Fixed changing controller files on disk not reloading BlendTree editor correctly
*   Fixed crash when building AnimatorController with empty layer
*   Fixed crash when calling SampleAnimation outside of the editor
*   Fixed crash when disabling GameObject in OnStateMachineEnter/Exit
*   Fixed crash when editing an Animation in the AnimationWindow with an AnimatorOverrideController
*   Fixed crash when importing some FBX files
*   Fixed crash when loading scene in playmode with an asset bundle containing a controller
*   Fixed crash when selecting a state with a null StateMachineBehaviour due to compilation errors
*   Fixed cutting a clip in FBX importer messing up other clips
*   Fixed display of transition pivot curves
*   Fixed false binding error on rig with Optimized Hierarchy On
*   Fixed GetStateMachineTransitions leaking memory
*   Fixed OnStateMachineEnter/Exit not being called on layers
*   Fixed renaming of states after exiting play mode
*   Fixed rotating view with mouse in the Avatar Configure Tool
*   Fixed runtime optimize/deoptimize hierarchy of GameObject
*   Fixed scaled UI buttons drifting when Animator has "Apply Root Motion" on
*   Fixed selection of blend tree items when multiple instances of the same motion occur in the same blend tree
*   Fixed sub-statemachine naming scheme
*   Fixed synced timing UI for additive layers
*   Fixed synchronization issue when you have both Animator's parameter window open
*   Fixed Transition interruption in destination State ExitTime
*   Fixed transition list temporarily loses its values on Editor re-compile
*   Fixed Transition Previewer handle manipulation
*   Prevented AnyState transitions to "Up" state machines from sub state machines because they were inconsistent
*   Removed Abstract StateMachineBehaviours from the list offered to users
*   Removed invalid multiple preview from the ModelImporter Animation sub-editor

### Physics Fixes

*   Don't create PhysX shapes for disabled terrains
*   Ensure that both friction and bounce are updated when the PhysicsMaterial2D is set on a Collider2D from script
*   Fix a crash in the HingeJoint when enabling a GameObject containing a HingeJoint where the Connected Body was disabled
*   Fix problems where QNaNs leaked out of the physics system when using infinites as limit parameters for the ConfigurableJoint
*   Fix wheel collider applying the inertia tensor rotation the wrong way
*   Fixed incorrect depth sorting for results of 'Physics2D.GetRayIntersectionXXX' methods
*   Remove invalid tire contact shapes from the vehicles queries cache up on collider deactivation
*   Report scene hierarchy path of Collider when setting a transform that contains non-finite numbers
*   Reset query filters when removing wheels, to stay on the safe side as PhysX can actually run queries of almost zero length for disabled wheels

### Scripting, Mono and IL2CPP Fixes

*   IL2CPP: Correct a C++ compiler error in generated code: "No matching function for call to 'il2cpp\_codegen\_raise\_exception'"
*   IL2CPP: Fix crash when using OnCollisionEnter with no parameters
*   IL2CPP: Fix crash when using OnCollisionEnter2D with no parameters
*   IL2CPP: Prevent the exception "ArgumentException: Value does not fall within the expected range." during a call to the JoinMulticastGroup method
*   IL2CPP: Throw exceptions when classes are stripped instead of crashing
*   Mono: Fix issue with Socket.Select never returning sockets ready for read on Mac OS X
*   Mono: Fix Unity crash when detecting recursive type definition
*   Mono: Fixed issue with default property values and object initializers
*   Prefs: Show "MonoDevelop Solution Properties" whenever an external MonoDevelop or XamarinStudio is selected
*   Serialization: Fix crash when selecting "Scripting Backend" option in Other Settings
*   Serialization: Fixed not being able to serialize a field called "Base"

### UI Fixes

*   Allow UI elements to render in overlay mode even if they don't have a shader that requires lighting
*   Disallowed InputFields with ContentType Password from copying text to the clipboard
*   Ensured that the parent canvas sorting layer/order is used unless override sorting is specified
*   Fix issue with UI stencil breaking in editor due to materials that were deleted being passed through to the render pipeline
*   Fixed dropdown editor not working due to bad file name
*   Fixed issue with text not showing properly after certain edit operations in InputField
*   Force children canvas to use the parent canvas matrix such that distance sorting is not applied
*   Only call PointerDrop callback if we have begun a pointer drag
*   Stop disabled graphics from blocking raycasts
*   Stop OnValidate being called at inappropriate times for UI elements
*   Update the Canvas RectTransform after LateUpdate to catch any Canvas camera positioning changes
*   When overriding sorting ensure to calculate the bounds using the generated mesh of the correct sub Canvas

### WebGL Fixes

*   Correctly return errors on WWW downloads for invalid URLs
*   Fix iframe gaining focus when clicking on WebGL canvas
*   Fix Standard shader usage in Safari
*   Fixed DXT5 decompressor which resulted in slightly imperfect textures
*   Make AudioClip.Create print an error when used with the stream option in WebGL
*   Make AudioMixer work for controlling volume
*   Make Directory.Create and Directory.GetCurrent work correctly
*   Make state created in Application.ExternalEval persistent between calls, like in the web player
*   Make sure WebGL builds will not require any calls to JavaScript "eval" to run, as that is not permitted in some environments
*   Normalize scroll wheel inputs to give more consistent results
*   Remove non-functional icon settings from WebGL build settings
*   When Application.runInBackground is enabled, run the WebGL update loop at least once a second, even when the tab is not visible

### Other Fixes

*   AssetBundle: Check if the manifest AssetBundle name has conflict with the user predefined AssetBundle name
*   AssetBundle: Fix the issue that Resources.UnloadUnusedAssets() doesn't unload fonts if they were loaded from an asset bundle
*   AssetBundle: Fix the issue that search result window won't get updated when the AssetBundle name is changed
*   AssetBundle: Fix the wrong size breakdown in the Editor.log when building AssetBundles
*   AssetBundle: Fixed issue that AssetBundleManifest.GetAssetBundleHash() returns wrong hash
*   AssetBundle: Fixed issue that AssetDatabase.GetAssetPathsFromAssetBundle only returns assets explicitly included in the AssetBundle
*   AssetBundle: Fixed issue that AssetDatabase.GetAssetPathsFromAssetBundleAndAssetName returns paths in random order
*   AssetBundle: Throw a warning when getting hash from AssetBundleManifest with a non-existing bundle name
*   AssetBundle: Fix non-first scene loading from streamed asset bundle with multiple scenes
*   Audio: Fixed AudioSource inspector not updating to show new pitch value when this is set from script
*   Audio: Fixed occasional crash at editor shutdown
*   Audio: Fixed occasional crashes that could occur with non-blocking sounds if the audio source was stopped right after being started
*   Audio: Fixed some memory leaks
*   Audio: Fixed undo of AudioMixerGroup colour changing and Solo/Mute/Bypass toggling
*   Audio: Now able to import from 32 bit fixed point and big-endian AIFF audio files
*   Audio: Transition to null snapshot in AudioMixer was crashing editor
*   Core: Enabled SSE2 optimizations on 64 bit OS X builds
*   Core: Fixed hang when passing large arrays to the Undo system
*   Core: Fixed several memory leaks when running standalone players with -batchmode
*   Core: References to "Resources/unity\_builtin\_extra" should get preloaded
*   Home: Go to Accounts and Manage Organizations now authenticate you before opening Accounts page
*   Home: Fixed stay on “connecting” window if there’s no internet connection
*   Importing: Changes to scripts are now correctly processed synchronously, fixing a range of issues with scripts relating to asset processing at import time
*   Importing: Fixed quit with 'Fatal Error' when out of memory during importing large cubemap with smooth edges enabled
*   Input: Fixed touch input hanging a Windows application if a second 'touch window' is created in a plugin
*   iOS: Don't fail fatally when Unity Xcode plugin can't be installed
*   iOS: Fixed stripping of GameCenter social platform
*   iOS: Fixed value of InputField.text when another field is being edited with keyboard
*   iOS: Xcode 7 build failures worked around by disabling Bitcode. Bitcode support will come later
*   Linux: Fix button down reports when querying any joystick and multiple joysticks are connected
*   Linux: Make window size locking more Window Manager-agnostic
*   Networking: Fixed MatchMakingClient constructor generating an error when created outside the main thread
*   Networking: Fixed NetworkServer.ReplacePlayerForConnection not setting up ownership of the new player object properly
*   Networking: Fixed NetworkServer.Spawn failing silently when the server is not active
*   Networking: Fixed NetworkServer.Unspawn not allowing objects to re-spawned
*   Networking: Fixed NullReferenceException when a client disconnects after the player object was deleted
*   Networking: Fixed incorrect serialization of some 64 bit numbers
*   Networking: Fixed NetworkTransform cause corruption of SyncVars on other scripts
*   Networking: Fixed NetworkTransform not updating if only velocity has changed
*   Networking: NetworkTransform not syncing character controller rotation when not moving.
*   OS X Standalone: Fixed fullscreen mode
*   OS X Editor: Fix RunOpenPanel() with extension non-empty filter
*   Plugins: Default Standalone settings for CPU specific plugins will be correctly set once again, additional this path variation is now possible as well, for ex., "Assets\\MyPackage\\Plugins\\x86\\Plugin.dll"
*   Substance: Fix memory leak in the Editor
*   Substance: Fix Resources.Load() and Resources.LoadAll() not waiting for ProceduralTexture generation completion before returning
*   Substance: Fixed caching-related regression where the cache would neither be read at startup nor written afterwards
*   Substance: Improved the handling of input groups in the inspector (a single group can no longer be split into several input groups)
*   Substance: It is no longer possible to change the size of a Substance asset that was published with a fixed size, a warning is displayed in the inspector instead
*   Terrain: Fixed crash after baking navmesh if there are LOD trees painted
*   Terrain: Fixed crash when reimporting a billboard asset
*   Terrain: Fixed crash when reimporting the prefabs that are selected as tree prototypes on an active terrain
*   Terrain: Fixed incorrect lighting effect on grass when rendered in deferred path
*   Terrain: Fixed occasional editor error message when a terrain is selected
*   Terrain: Fixed rendering artifacts with Tree Creator trees in deferred rendering paths
*   Version Control: Allow adding a new file under the name of a deleted file even if the deletion hasn't been committed
*   Version Control: Correct overlays for assets where .meta files are out of sync with their assets
*   Version Control: Grey out outgoing changeset 'delete empty changeset' context menu item when changeset is not empty
*   Windows Phone 8.1: Fix simulator build
*   Windows Phone 8.1: OnApplicationFocus and OnApplicationPause will be called now, same as on other mobile platforms
*   Windows Phone 8: Fixed corrupted display resolution when screen is rotated in Landscape mode
*   Windows Phone 8: Global shader parameters will be correctly reset when the application is resumed
*   Windows Phone: Anisotropic texture filtering works now
*   Windows Phone: Do not show Portrait Upside Down option in player settings (both 8.0 & 8.1)
*   Windows Phone: Fix SerializationWeaver failure when using enums from .NET framework
*   Windows Store Apps/Phone: AvatarBuilder.BuildHumanAvatar should work correctly now
*   Windows Store Apps/Phone: Fix build when native plugin uses collection interfaces with nested generic parameters
*   Windows Store Apps/Phone: Fixed Input.gyro.useracceleration to not include gravity.
*   Windows Store Apps: Application will correctly change its resolution when you change display resolution
*   Windows Store Apps: Fix a memory leak which happened on quality settings change
*   Windows Store Apps: Fix build for editor using Universal SDK
*   Windows Store Apps: Fixed framerate drop when "Low Latency Presentation API" is enabled
*   Windows Store Apps: Set orientation from player settings on startup
*   Windows Store Apps: Support JPEG files for visual assets
*   Windows: Fixed window size when switching back from fullscreen
*   WinRT: Fixed Networking sometimes throwing NotImplementedException
*   XboxOne: Fixed the "EditorOnlyPlayerSettings property not initialized" error