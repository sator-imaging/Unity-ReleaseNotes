# Unity 5.2
https://unity3d.com/unity/whats-new/unity-5.2

## Fixes


### 2D Fixes
<ul>
<li>After applying settings in sprite editor window, deselect any sprite rect.</li>
<li>Apply active color space onto texture in sprite editor.</li>
<li>Clear undos for SpriteEditorWindow when applying or window is closed. Also fix ClearUndo not working for ObjectUndo.</li>
<li>Do not trim sprite when Shift-T is pressed while entering name in Sprite Editor.</li>
<li>Ensure SpriteEditorWindow has the correct texture importer reference when texture importer inspector is applying changes</li>
<li>Fix NullReferenceException when creating a new sceneview</li>
<li>Fix pointer enter/exit detection order with sorting layers</li>
<li>Hide PerRendererData shader properties in inspector as property is retrieved from the renderer</li>
<li>Increase responsiveness of Sprite Editor in Mac OS X</li>
<li>Materials become transparent because of improper re-setting of material</li>
<li>Non-sprite textures will display in sprite editor window with no options</li>
<li>Quit 2D collider editing mode when user reset the collider component</li>
<li>Reimport texture if texture importer is reset</li>
<li>Remove a sprite rect if the selected sprite rect is empty when trimmed</li>
<li>Replaced assert with warning message to multiple materials in SpriteRenderer</li>
<li>Set correct zoom values for zoom bar in SpriteUtilityWindow</li>
<li>Set SpriteRenderer to dirty when color is set</li>
<li>Sprite Editor uses the actual image size for slicing operation. Force Sprite Editor preview to use mipmap if user machine does not support the image resolution</li>
<li>Sprite Packer no longer packs Truecolor sprites into the same Atlas if other format settings are different</li>
<li>Update sorting layer APIs and prevent setting invalid sorting layer ids to renderer</li>
<li>View tool (panning, rotating, zooming) in the scene view will not manipulate collider control point even in collider editing mode</li>
</ul>

### Android Fixes
<ul>
<li>Android: Added API level 22 to the minSdk list</li>
<li>Android: Added support to create a real 16bit RGB565 backbuffer. Deprecated Handheld.use32BitDisplayBuffer</li>
<li>Android: Audio - Fixed issues on GearVR when the device does not report FEATURE_AUDIO_LOW_LATENCY</li>
<li>Android: Buildpipe - Android Libraries can now be excluded from build in the Plugin Inspector</li>
<li>Android: Buildpipe - Fixed assets folders in aar files</li>
<li>Android: Fixed ATC texture compression for RGBA textures</li>
<li>Android: Fixed bug that caused texture format RGBA4444 to be used for RGBA textures even when overriding in build settings</li>
<li>Android: Fixed crash affecting some PowerVR 544 devices</li>
<li>Android: Fixed performance regression in Resource.Load when calling it multiple times for the same resource</li>
<li>Android: JNI - fixed long data type</li>
<li>Android: Stripping - don't strip AssetBundle class or it removes LoadAssetAsync</li>
<li>Android: WWW - report HTTP status and response in case of failure</li>
</ul>

### Editor Fixes
<ul>
<li>Animation Window: Animated particle properties are now show up in red in Inspector</li>
<li>Animation Window: Animated property values are now updated in Particle Editor when scrubbing in Animation Window</li>
<li>Animation Window: Animation curve now updates after changing controller</li>
<li>Animation Window: Ctrl+A now selects all keys and properties</li>
<li>Animation Window: Highlight is now blue when selecting all properties from animation window</li>
<li>Animation Window: It’s now possible to move current time before the first key</li>
<li>Animation Window: Replacing existing animation now actually replaces the asset instead of creating new one with unique name</li>
<li>Automatically checkout ProjectSettings/ProjectVersion.txt if needed</li>
<li>Avoid division by zero in zero-sized SphereCollider</li>
<li>Avoid locking when framing terrain</li>
<li>Camera lock keeps working when dragging outside the scene view window</li>
<li>Clear old main menus on Windows</li>
<li>Dirty materials when fixing HDR texture to ensure previews are updated</li>
<li>Ensure selected asset is revealed in project browser when changing layout</li>
<li>Fix asset store preview blinking in the project browser</li>
<li>Fix camera frustum gizmo not properly showing custom projection matrices</li>
<li>Fix CapsuleCollider gizmo handles are offset by a 90 degree angle</li>
<li>Fix caret not moving in ObjectSelector when using left/right arrow keys (only when no items were selected)</li>
<li>Fix crash when deleting an object from a prefab instance where the prefab asset is missing</li>
<li>Fix creating a script from the right click menu throws "Rename not started" error</li>
<li>Fix creating new assets after deletion of assets would throw error</li>
<li>Fix Cursor flickering in editor while play testing if cursor.visible = false</li>
<li>Fix Cursor.visible not working until the game view is focused</li>
<li>Fix disabled scrollbar in lighting window lightmaps tab</li>
<li>Fix error when renaming items in project and hierarchy views</li>
<li>Fix Hierarchy type searching so 't:script' or 't:monobehaviour' shows all game objects with scripts attached</li>
<li>Fix icons in Project Browser 'jumping' when changing view</li>
<li>Fix IMGUI brightness on GameView when in Linear color space</li>
<li>Fix memory thrashing when Dragging and Dropping between panels, when the dragged object had a CustomEditor with no Preview</li>
<li>Fix multi-object selection of reflection probe cubemap to not incorrectly set same cubemaps</li>
<li>Fix non character keys being mixed up with character keys on shortcuts</li>
<li>Fix not being able to focus tabs after changing "Output" on Audio Source</li>
<li>Fix occasional recycle bin bypassing when deleting assets on Windows</li>
<li>Fix popped out container window not able to move when two editor windows are stacked one above/next to the other</li>
<li>Fix possible data loss on Windows when renaming folder with locked files</li>
<li>Fix rare case of invalid folder path shown in the Project Browser</li>
<li>Fix scene view window still being tinted in playmode when an overlay was active</li>
<li>Fix scene's GI is not updated after building AssetBundle or opening the same scene</li>
<li>Fixed bug which caused the Move Tool, when used on an object with a negatively scaled parent, to snap to whole units</li>
<li>Fixed Gradient not updating when an Undo is performed</li>
<li>Fixed occasional exception thrown when creating an asset/folder under Assets folder in Project pane with One Column Layout</li>
<li>Fixed Scene View audio play toggle not returning to previous state after exiting Play Mode</li>
<li>Fixed Scene View camera moving slightly while holding down right mouse button</li>
<li>In play mode, tick one more frame after the editor is not active, so that the game can get a chance to respond to being paused</li>
<li>Make sure GUISkin.current is set to GameSkin before invoking any user script</li>
<li>Scene view picking works when selection base object isn't under the mouse position</li>
<li>Terrain editor hotkeys no longer conflict with text field input</li>
</ul>

### Graphics, Lightmapping and Shader Fixes
<ul>
<li>GI: Ambient GI value not changing based on disabled realtime/baked GI</li>
<li>GI: Fix crash following lighting builds in GetSystemTexture</li>
<li>GI: Fixed bake getting stuck on some terrains</li>
<li>GI: Fixed crash in CreateSnapshotForReflectionProbe when trying to rebake reflection probes</li>
<li>GI: Fixed environment reflection cubemap getting unloaded after the scene was loaded using Application.LoadLevel for scenes that used the Auto lighting build mode</li>
<li>GI: Fixed lightmap shader variant stripping for realtime lightmaps. Now each lightmaps mode (non-directional, directional and directional specular) variant can be picked for baked and realtime GI separately. Please review your settings if you selected a specific lightmaps mode variant in the Graphics Settings to make that mode work for realtime lightmaps</li>
<li>GI: Fixed radiosity core corruption error when baking lightmap</li>
<li>GI: Fixed UV packing for baked UVs not filling the 0-1 space (smaller or bigger). Fixes a bunch of issues where one object with stray UVs could overlap other objects and cause dark spots. Also makes the resolution assigned to each object work much more reliably if that object's unwrap is not filling the 0-1 space and also when its bounds are non-square. Please review the resolution on your instances for baked lightmaps</li>
<li>GI: Lightmap snapshot gets cleared when clearing GI Cache</li>
<li>Graphics: Crunch texture compression support for 8192x8192 textures (64-bit editor builds only)</li>
<li>Graphics: Apply hard limit on font size of 500 in more places than just font importer</li>
<li>Graphics: Fix for asset bundle content changes between subsequent generations due to uninitialised vertex buffer</li>
<li>Graphics: Fix for call to OpenGL ES API without current context when using the multi-threaded renderer</li>
<li>Graphics: Fixed a shader compiler error on OpenGL ES platforms where dot() between a vec3 and a float would fail to add an upcast</li>
<li>Graphics: Fixed bug in ES 3 shader code generator that caused clipping problems in UI shaders</li>
<li>Graphics: Fixed crash while using -force-gles on Mac OS X</li>
<li>Graphics: Fixed editor rendering black views when running with OpenGL ES 2.0</li>
<li>Graphics: Fixed Halo errors when they are on DontDestroyOnLoad objects</li>
<li>Graphics: Fixed Halo texture not being centered, causing half-texel clipping on top/right sides</li>
<li>Graphics: Fixed issue with MaterialPropertyBlock not working with Particles</li>
<li>Graphics: Fixed material keywords and renderQueue not copied over by new Material(material) constructor and Material.CopyPropertiesFromMaterial</li>
<li>Graphics: Fixed MSAA initialization on older Android devices which only support multisampled_render_to_texture</li>
<li>Graphics: Fixed spamming error message importing an EXR file as sprite</li>
<li>OpenGL core: Fixed crash when using -force-glcore on Mac OS X where it's not yet supported</li>
<li>OpenGL core: Fixed Radeon HD 2000 - 4000 support</li>
<li>OpenGL core: Gracefully fallback to D3D when requesting OpenGL/ES with -force-gl** when the platform doesn't have a good enough OpenGL support</li>
<li>OpenGL ES: Fixed blit from backbuffer into RenderTexture</li>
<li>OpenGL ES: Fixed Fire HD development player crash</li>
<li>OpenGL ES: Fixed crash with dynamic batching of empty meshes</li>
<li>OpenGL: Always rely GL_EXT/IMG_multisampled_render_to_texture when available to save a lot of bandwidth when using MSAA</li>
<li>OpenGL: Resolved various invalid operation / enum errors due to platform compatibility issues</li>
<li>Particles: Fixed culling issues when particles are set from script</li>
<li>Particles: Fixed curve editor preview not updating after undo</li>
<li>Particles: Fixed Limit Velocity over Lifetime being framerate-dependent</li>
<li>Particles: Fixed prewarming performance problems</li>
<li>Particles: Fixed some spawn parameters not being random enough</li>
<li>Particles: Fixed StartDelay not working from script</li>
<li>Particles: Fixed sub-emitters sometimes not firing</li>
<li>Particles: Fixed various crashes</li>
<li>Shaders: Fixed some cases of objects with unsupported shaders not rendering at all (instead of rendering in pink)</li>
<li>Shaders: Fixed some loop constructs being translated wrongly for GLSL/Metal</li>
</ul>

### Mecanim Fixes
<ul>
<li>Deprecated legacy culling modes BasedOnUserBounds and BasedOnClipBounds</li>
<li>Do not activate runtime State parameter on parameter rename</li>
<li>Fixed "Cleaning up leaked objects" message after using the Avatar Configure Tool</li>
<li>Fixed a bug where it would not be possible to animate the second material on a meshrenderer</li>
<li>Fixed a bug where the lock button on the Animator Window would reset after play mode</li>
<li>Fixed a case where going to play mode would prevent undo operations from being pushed</li>
<li>Fixed an editor performance issue with large blend trees</li>
<li>Fixed an error where transitions would disappear if a controller was edited without saving immediately after upgrade from 4.x to 5.x</li>
<li>Fixed an undo error in the blend tree inspector</li>
<li>Fixed an undo related crash</li>
<li>Fixed Animator.speed set in Start() not working</li>
<li>Fixed asserts with empty controller</li>
<li>Fixed Asset Store preview of Humanoid character</li>
<li>Fixed Avatar Configure broken ResetPose when OptmizeGameObject is on</li>
<li>Fixed Blend tree max/min thresholds not being updated when changed through dragging on the graph in the inspector</li>
<li>Fixed broken BlendTree slider with some BlendTree configuration</li>
<li>Fixed broken BlendTrees with identical negative blend values</li>
<li>Fixed changing controller files on disk not reloading BlendTree editor correctly</li>
<li>Fixed crash when building AnimatorController with empty layer</li>
<li>Fixed crash when calling SampleAnimation outside of the editor</li>
<li>Fixed crash when disabling GameObject in OnStateMachineEnter/Exit</li>
<li>Fixed crash when editing an Animation in the AnimationWindow with an AnimatorOverrideController</li>
<li>Fixed crash when importing some FBX files</li>
<li>Fixed crash when loading scene in playmode with an asset bundle containing a controller</li>
<li>Fixed crash when selecting a state with a null StateMachineBehaviour due to compilation errors</li>
<li>Fixed cutting a clip in FBX importer messing up other clips</li>
<li>Fixed display of transition pivot curves</li>
<li>Fixed false binding error on rig with Optimized Hierarchy On</li>
<li>Fixed GetStateMachineTransitions leaking memory</li>
<li>Fixed OnStateMachineEnter/Exit not being called on layers</li>
<li>Fixed renaming of states after exiting play mode</li>
<li>Fixed rotating view with mouse in the Avatar Configure Tool</li>
<li>Fixed runtime optimize/deoptimize hierarchy of GameObject</li>
<li>Fixed scaled UI buttons drifting when Animator has "Apply Root Motion" on</li>
<li>Fixed selection of blend tree items when multiple instances of the same motion occur in the same blend tree</li>
<li>Fixed sub-statemachine naming scheme</li>
<li>Fixed synced timing UI for additive layers</li>
<li>Fixed synchronization issue when you have both Animator's parameter window open</li>
<li>Fixed Transition interruption in destination State ExitTime</li>
<li>Fixed transition list temporarily loses its values on Editor re-compile</li>
<li>Fixed Transition Previewer handle manipulation</li>
<li>Prevented AnyState transitions to "Up" state machines from sub state machines because they were inconsistent</li>
<li>Removed Abstract StateMachineBehaviours from the list offered to users</li>
<li>Removed invalid multiple preview from the ModelImporter Animation sub-editor</li>
</ul>

### Physics Fixes
<ul>
<li>Don't create PhysX shapes for disabled terrains</li>
<li>Ensure that both friction and bounce are updated when the PhysicsMaterial2D is set on a Collider2D from script</li>
<li>Fix a crash in the HingeJoint when enabling a GameObject containing a HingeJoint where the Connected Body was disabled</li>
<li>Fix problems where QNaNs leaked out of the physics system when using infinites as limit parameters for the ConfigurableJoint</li>
<li>Fix wheel collider applying the inertia tensor rotation the wrong way</li>
<li>Fixed incorrect depth sorting for results of 'Physics2D.GetRayIntersectionXXX' methods</li>
<li>Remove invalid tire contact shapes from the vehicles queries cache up on collider deactivation</li>
<li>Report scene hierarchy path of Collider when setting a transform that contains non-finite numbers</li>
<li>Reset query filters when removing wheels, to stay on the safe side as PhysX can actually run queries of almost zero length for disabled wheels</li>
</ul>

### Scripting, Mono and IL2CPP Fixes
<ul>
<li>IL2CPP: Correct a C++ compiler error in generated code: "No matching function for call to 'il2cpp_codegen_raise_exception'"</li>
<li>IL2CPP: Fix crash when using OnCollisionEnter with no parameters</li>
<li>IL2CPP: Fix crash when using OnCollisionEnter2D with no parameters</li>
<li>IL2CPP: Prevent the exception "ArgumentException: Value does not fall within the expected range." during a call to the JoinMulticastGroup method</li>
<li>IL2CPP: Throw exceptions when classes are stripped instead of crashing</li>
<li>Mono: Fix issue with Socket.Select never returning sockets ready for read on Mac OS X</li>
<li>Mono: Fix Unity crash when detecting recursive type definition</li>
<li>Mono: Fixed issue with default property values and object initializers</li>
<li>Prefs: Show "MonoDevelop Solution Properties" whenever an external MonoDevelop or XamarinStudio is selected</li>
<li>Serialization: Fix crash when selecting "Scripting Backend" option in Other Settings</li>
<li>Serialization: Fixed not being able to serialize a field called "Base"</li>
</ul>

### UI Fixes
<ul>
<li>Allow UI elements to render in overlay mode even if they don't have a shader that requires lighting</li>
<li>Disallowed InputFields with ContentType Password from copying text to the clipboard</li>
<li>Ensured that the parent canvas sorting layer/order is used unless override sorting is specified</li>
<li>Fix issue with UI stencil breaking in editor due to materials that were deleted being passed through to the render pipeline</li>
<li>Fixed dropdown editor not working due to bad file name</li>
<li>Fixed issue with text not showing properly after certain edit operations in InputField</li>
<li>Force children canvas to use the parent canvas matrix such that distance sorting is not applied</li>
<li>Only call PointerDrop callback if we have begun a pointer drag</li>
<li>Stop disabled graphics from blocking raycasts</li>
<li>Stop OnValidate being called at inappropriate times for UI elements</li>
<li>Update the Canvas RectTransform after LateUpdate to catch any Canvas camera positioning changes</li>
<li>When overriding sorting ensure to calculate the bounds using the generated mesh of the correct sub Canvas</li>
</ul>

### WebGL Fixes
<ul>
<li>Correctly return errors on WWW downloads for invalid URLs</li>
<li>Fix iframe gaining focus when clicking on WebGL canvas</li>
<li>Fix Standard shader usage in Safari</li>
<li>Fixed DXT5 decompressor which resulted in slightly imperfect textures</li>
<li>Make AudioClip.Create print an error when used with the stream option in WebGL</li>
<li>Make AudioMixer work for controlling volume</li>
<li>Make Directory.Create and Directory.GetCurrent work correctly</li>
<li>Make state created in Application.ExternalEval persistent between calls, like in the web player</li>
<li>Make sure WebGL builds will not require any calls to JavaScript "eval" to run, as that is not permitted in some environments</li>
<li>Normalize scroll wheel inputs to give more consistent results</li>
<li>Remove non-functional icon settings from WebGL build settings</li>
<li>When Application.runInBackground is enabled, run the WebGL update loop at least once a second, even when the tab is not visible</li>
</ul>

### Other Fixes
<ul>
<li>AssetBundle: Check if the manifest AssetBundle name has conflict with the user predefined AssetBundle name</li>
<li>AssetBundle: Fix the issue that Resources.UnloadUnusedAssets() doesn't unload fonts if they were loaded from an asset bundle</li>
<li>AssetBundle: Fix the issue that search result window won't get updated when the AssetBundle name is changed</li>
<li>AssetBundle: Fix the wrong size breakdown in the Editor.log when building AssetBundles</li>
<li>AssetBundle: Fixed issue that AssetBundleManifest.GetAssetBundleHash() returns wrong hash</li>
<li>AssetBundle: Fixed issue that AssetDatabase.GetAssetPathsFromAssetBundle only returns assets explicitly included in the AssetBundle</li>
<li>AssetBundle: Fixed issue that AssetDatabase.GetAssetPathsFromAssetBundleAndAssetName returns paths in random order</li>
<li>AssetBundle: Throw a warning when getting hash from AssetBundleManifest with a non-existing bundle name</li>
<li>AssetBundle: Fix non-first scene loading from streamed asset bundle with multiple scenes</li>
<li>Audio: Fixed AudioSource inspector not updating to show new pitch value when this is set from script</li>
<li>Audio: Fixed occasional crash at editor shutdown</li>
<li>Audio: Fixed occasional crashes that could occur with non-blocking sounds if the audio source was stopped right after being started</li>
<li>Audio: Fixed some memory leaks</li>
<li>Audio: Fixed undo of AudioMixerGroup colour changing and Solo/Mute/Bypass toggling</li>
<li>Audio: Now able to import from 32 bit fixed point and big-endian AIFF audio files</li>
<li>Audio: Transition to null snapshot in AudioMixer was crashing editor</li>
<li>Core: Enabled SSE2 optimizations on 64 bit OS X builds</li>
<li>Core: Fixed hang when passing large arrays to the Undo system</li>
<li>Core: Fixed several memory leaks when running standalone players with -batchmode</li>
<li>Core: References to "Resources/unity_builtin_extra" should get preloaded</li>
<li>Home: Go to Accounts and Manage Organizations now authenticate you before opening Accounts page</li>
<li>Home: Fixed stay on “connecting” window if there’s no internet connection</li>
<li>Importing: Changes to scripts are now correctly processed synchronously, fixing a range of issues with scripts relating to asset processing at import time</li>
<li>Importing: Fixed quit with 'Fatal Error' when out of memory during importing large cubemap with smooth edges enabled</li>
<li>Input: Fixed touch input hanging a Windows application if a second 'touch window' is created in a plugin</li>
<li>iOS: Don't fail fatally when Unity Xcode plugin can't be installed</li>
<li>iOS: Fixed stripping of GameCenter social platform</li>
<li>iOS: Fixed value of InputField.text when another field is being edited with keyboard</li>
<li>iOS: Xcode 7 build failures worked around by disabling Bitcode. Bitcode support will come later</li>
<li>Linux: Fix button down reports when querying any joystick and multiple joysticks are connected</li>
<li>Linux: Make window size locking more Window Manager-agnostic</li>
<li>Networking: Fixed MatchMakingClient constructor generating an error when created outside the main thread</li>
<li>Networking: Fixed NetworkServer.ReplacePlayerForConnection not setting up ownership of the new player object properly</li>
<li>Networking: Fixed NetworkServer.Spawn failing silently when the server is not active</li>
<li>Networking: Fixed NetworkServer.Unspawn not allowing objects to re-spawned</li>
<li>Networking: Fixed NullReferenceException when a client disconnects after the player object was deleted</li>
<li>Networking: Fixed incorrect serialization of some 64 bit numbers</li>
<li>Networking: Fixed NetworkTransform cause corruption of SyncVars on other scripts</li>
<li>Networking: Fixed NetworkTransform not updating if only velocity has changed</li>
<li>Networking: NetworkTransform not syncing character controller rotation when not moving.</li>
<li>OS X Standalone: Fixed fullscreen mode</li>
<li>OS X Editor: Fix RunOpenPanel() with extension non-empty filter</li>
<li>Plugins: Default Standalone settings for CPU specific plugins will be correctly set once again, additional this path variation is now possible as well, for ex., "Assets\MyPackage\Plugins\x86\Plugin.dll"</li>
<li>Substance: Fix memory leak in the Editor</li>
<li>Substance: Fix Resources.Load() and Resources.LoadAll() not waiting for ProceduralTexture generation completion before returning</li>
<li>Substance: Fixed caching-related regression where the cache would neither be read at startup nor written afterwards</li>
<li>Substance: Improved the handling of input groups in the inspector (a single group can no longer be split into several input groups)</li>
<li>Substance: It is no longer possible to change the size of a Substance asset that was published with a fixed size, a warning is displayed in the inspector instead</li>
<li>Terrain: Fixed crash after baking navmesh if there are LOD trees painted</li>
<li>Terrain: Fixed crash when reimporting a billboard asset</li>
<li>Terrain: Fixed crash when reimporting the prefabs that are selected as tree prototypes on an active terrain</li>
<li>Terrain: Fixed incorrect lighting effect on grass when rendered in deferred path</li>
<li>Terrain: Fixed occasional editor error message when a terrain is selected</li>
<li>Terrain: Fixed rendering artifacts with Tree Creator trees in deferred rendering paths</li>
<li>Version Control: Allow adding a new file under the name of a deleted file even if the deletion hasn't been committed</li>
<li>Version Control: Correct overlays for assets where .meta files are out of sync with their assets</li>
<li>Version Control: Grey out outgoing changeset 'delete empty changeset' context menu item when changeset is not empty</li>
<li>Windows Phone 8.1: Fix simulator build</li>
<li>Windows Phone 8.1: OnApplicationFocus and OnApplicationPause will be called now, same as on other mobile platforms</li>
<li>Windows Phone 8: Fixed corrupted display resolution when screen is rotated in Landscape mode</li>
<li>Windows Phone 8: Global shader parameters will be correctly reset when the application is resumed</li>
<li>Windows Phone: Anisotropic texture filtering works now</li>
<li>Windows Phone: Do not show Portrait Upside Down option in player settings (both 8.0 &amp; 8.1)</li>
<li>Windows Phone: Fix SerializationWeaver failure when using enums from .NET framework</li>
<li>Windows Store Apps/Phone: AvatarBuilder.BuildHumanAvatar should work correctly now</li>
<li>Windows Store Apps/Phone: Fix build when native plugin uses collection interfaces with nested generic parameters</li>
<li>Windows Store Apps/Phone: Fixed Input.gyro.useracceleration to not include gravity.</li>
<li>Windows Store Apps: Application will correctly change its resolution when you change display resolution</li>
<li>Windows Store Apps: Fix a memory leak which happened on quality settings change</li>
<li>Windows Store Apps: Fix build for editor using Universal SDK</li>
<li>Windows Store Apps: Fixed framerate drop when "Low Latency Presentation API" is enabled</li>
<li>Windows Store Apps: Set orientation from player settings on startup</li>
<li>Windows Store Apps: Support JPEG files for visual assets</li>
<li>Windows: Fixed window size when switching back from fullscreen</li>
<li>WinRT: Fixed Networking sometimes throwing NotImplementedException</li>
<li>XboxOne: Fixed the "EditorOnlyPlayerSettings property  not initialized" error</li>
</ul>
