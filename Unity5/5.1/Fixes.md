# Unity 5.1

https://unity3d.com/unity/whats-new/unity-5.1

## Fixes



*   2D: Added Vector2.down and Vector2.left properties
*   2D: Always default to use "Rect" tool if project started as a 2D project.
*   2D: Always prompt user to apply unapplied texture setting before opening up Sprite Editor Window.
*   2D: Apply button now work correctly between sprite editor window and sprite inspector.
*   2D: Avoid editing/deleting a polygon collider point while panning the scene view.
*   2D: Do not display sprite mesh wireframe in scene view under any circumstances
*   2D: Double Clicking on a Sprite will not ignore External Tools prefs now.
*   2D: Fixed occasional crashes while building on 'Repacking sprite aliases'
*   2D: Fixed some edge cases that will result in odd shape during sprite editor's automatic slicing.
*   2D: Fixed Corrupted Sprites in Sprite Packer for iOS and Android
*   2D: Fixed error appeared if Sprite was sliced only for 1 slice
*   2D: Height and Width of a sprite rect in Sprite Editor Window will no longer be 0.
*   2D: Losing focus in Sprite Editor will now always show Apply/Revert popup.
*   2D: Material field from SpriteRenderer no longer behaves as array type.
*   2D: Revert button will reset value correctly in sprite editor window.
*   2D: Scene View picking always picks the visually top-most for different SortingLayers and z-depths
*   2D: Show both original and atlas format in the preview for packed sprite sheet.
*   2D: Slicing by grid in Sprite Editor Window will now limit the input values to the size of the texture.
*   2D: Sprite Atlas will no longer produces errors at low resolutions
*   2D: Sprites now generate Preview Images in the Inspector when using object field
*   2D: Undo will not undo applied Sprite Editor Window changes.
*   2D: Using trim button in Sprite Editor window will correctly enable Apply/Revert button.
*   Android: Buildpipe - detect plugin errors when package names differ only by cases
*   Android: Fix for spaces being replaced with underscores in app titles
*   Android: Input - Fix axis stuck on Android TV after hiding keyboard
*   Animation: Adding a new curve to an AnimationClip with AnimationClip.SetCurve now update correctly the animation length
*   Animation: Fixed a bug where callbacks called indirectly from ApplyOnAnimatorIK would reset the animator memory and cause a crash
*   Animation: Fixed animator controller window title
*   Animation: Fixed Animator exception (m\_IsVisibleInScene && IsInScene()) == m\_IsVisibleInScene) when disabling a game object with a disabled mesh renderer
*   Animation: Fixed copy paste of Animator State with StateMachineBehaviour , StateMachineBehaviour instances were not cloned correctly
*   Animation: Fixed crash when a StateMachineBehaviour disables his own animator component
*   Animation: Fixed CycleOffset range for animator state, valid range is between 0 and 1
*   Animation: Fixed direct blendtree editor slow down when there is too much motion
*   Animation: Fixed duplicated parameter in blend tree of blend tree
*   Animation: Fixed Livelink of AnyStateTransitions
*   Animation: Fixed transitions disappearing when importing a project from 4.x
*   Animation: Fixed update issue with Animator parameter window when going into playmode. Parameter list in the window was not updated anymore.
*   Animation: Fixes crash when disabling animator in OnAnimatorMove
*   Animation Window: Disable renaming items in animation window add property popup
*   Animation Window: Dragging sprite(s) to empty clip
*   Animation Window: Editing tangents in dopesheet context menu will save changes and handle undo correctly
*   Animation Window: Fixed an issue where keys on some curves were harder to click than others
*   Animation Window: Keyframe of missing sprite no longer has weird visual offset in the dopesheet
*   Animation Window: No more errors when changing to curve tab with sprite animation
*   Animation Window: Prevent dragging other object types to Sprite curve
*   Animation Window: Record mode is correctly cancelled when non-animated object is selected or new scene is created
*   Asset Loading: Always build the manifest AssetBundle and return the AssetBundleManifest object.
*   Asset Loading: Throw exception when calling Resources.LoadAll with null path.
*   Asset Management: Fix the crashes when saving with deleted gameobject
*   Asset Management: Unity packages now include .meta files for folders, allowing plugin settings for OS X native plugins to be transferred correctly
*   Asset Store: Fix download progress for packages larger than 2GB
*   Core: Fixed some memory leaks in the Editor and Players.
*   Editor: Breaking prefab instance through the menu "GameObjects->Break prefab instance" can now be undone
*   Editor: Calling Undo.RecordObject on editor objects no longer dirties the scene.
*   Editor: Clear old main menus on OSX
*   Editor: Do not change selection when duplicating while dragging
*   Editor: Fix crash when two inspector windows are open
*   Editor: Fix cubemap preview icons showing as white textures in Project Browser and Object Picker.
*   Editor: Fix DecoratorDrawers being shown twice for properties with custom PropertyDrawers that call into the default PropertyField implementation.
*   Editor: Fix default cursor appearing during editor startup on OSX
*   Editor: Fix Float Fields not accepting Infinity correctly
*   Editor: Fix GUIStyle errors on import (delay GUIStyle initialization to OnGUI).
*   Editor: Fix layers popup showing in the top left of the window and not below layers button.
*   Editor: Fix player settings window accessing non-initialized property.
*   Editor: Fix text fields content switch between build settings in some cases.
*   Editor: Fix undo of reset position/rotation/scale
*   Editor: Fixed crash when attempting to add the same component twice to a GameObject in the Editor
*   Editor: Fixed warning when dragging'n'dropping a mesh onto a GameObject
*   Editor: Make Android and iOS splash screen separate settings (no longer shared)
*   Editor: Plugin inspector - set ARMv6 Android plugins incompatible to avoid collisions
*   Editor: Scene View will no longer have tint applied when entering play mode.
*   Editor: Update m\_GUIDToPath when moving asset to path name with different case.
*   Editor: Update menu items when assemblies are loaded in the editor
*   Editor: Update ShaderGUI for MaterialEditor when shader changes
*   Editor: Use IntField instead of FloatField for Sprite Editor
*   Fix issue where UnityEvents would lose their target function on assembly rebuild
*   Fix null reference on EventTrigger component when accessing delegates list. Some situations could cause it to not be initialized.
*   GI: Fix temporary visual glitch caused by missing atlas textures when a new lighting build is switched in when in auto lighting mode.
*   GI: Fix temporary visual glitch caused by missing UVs when a new lighting build is switched in when in auto lighting mode.
*   Graphics: Fixed AfterDepthTexture and AfterDepthNormalsTexture command buffers to be executed after the texture is set as a shader property.
*   Graphics: Fixed crash in a case where particle system would not have a valid mesh
*   Graphics: Fixed crash in Instantiate(Mesh) when static batching is used for the Mesh
*   Graphics: Fixed crash where MeshCombiner would not allocate enough indices
*   IMGUI: Fixed NullReferenceException when calling GUI.BeginScrollView with 7 arguments
*   iOS: Fixed duplicate property value removal in certain Xcode projects
*   iOS: Fixed Xcode project supported platforms and SDKs settings
*   Lightmapping: Fixed race condition crash in lightmap bake when converting .exr files.
*   Linux: Fix applying vsync and antialiasing changes without changing quality level
*   Linux: Fix OS version check when lsb\_release isn't present.
*   Linux: Support more standard screen resolutions
*   Merge Tool: Handle regression in 5.0.1 introduced by stripped prefabs
*   Merge Tool: Fix auto fallback spec file detection
*   OSX: background image used for mac installer packages has been increased in size
*   OSX: Fix "Default is native resolution" setting.
*   OSX: Fix resolution update race when resizing window.
*   OSX: Prevent idle sleep while the player is active
*   Prevent accidentally moving multiple times when navigating UI with keyboard or controller by introducing a repeat delay to the StandaloneInputModule. This is similar to the delay before the repeating events that OSes have.
*   Profiler: Fix lockup in editor, if left in background with the profiler open
*   Profiler: Fix receive buffer error and hang connection when transferring large chunk of profiler's data
*   ReflectionProbes: Buttons "Bake All Reflection Probes" in Lighting window and Reflection Probes inspector should behave correctly now.
*   Scripting: Fix plugin verification crash on reload/shutdown
*   Scripting: Fix potential crashes on Webplayer
*   Serialization: Fix crash when loading text serialized scene with >32k components
*   Serialization: Reapplied part of non-deterministic material serialization fix, but without increasing memory usage during building
*   Shaders: Add warning when using SV\_POSITION in vertex shader inputs on DX11, and improve error message.
*   Shaders: Fix standard shader cutout rendering being wrong when rendering with shader replacement.
*   Shaders: Fixed #pragma target and #pragma exclude\_renderers parsing with trailing comments.
*   Shaders: Fixed HLSL log10() translation into OpenGL/Metal platforms.
*   Shaders: Fixed shader compilation warnings not being shown if there are no compilation errors.
*   Shaders: Fixed that surface shaders vertex color field had to actually be called "color" (now just COLOR semantic is enough, like the docs always said).
*   Substance: Fix hang in ProceduralMaterial::Clean().
*   Substance: Fix crash when assigning a shader that does not cause outputs to be generated (e.g. Unlit/Color) to a ProceduralMaterial.
*   Substance: Fix 'path != ""' assert when live-previewing a Substance from the Asset Store.
*   Substance: Global Illumination flags are now correctly handled by ProceduralMaterials.
*   Substance: Fix console spam related to the absence of '\_MainTex' shader property.
*   Terrain: Fixed an issue where painting terrain features while holding down the right mouse button could lock the view tool.
*   Terrain: Fixed crash on creating terrain with large heightmap resolution by script
*   Terrain: Fixed crash when terrains are neighbored and drawHeightmap is set to false
*   Terrain: Terrain brush no longer intercepts mouse events if the mouse cursor doesn't intersect with any terrain.
*   UI: Caret on InputField now blinks at proper frequency.
*   UI: Clamp setting canvas group alpha between 0-1 on API call
*   UI: Destroying a RectTransform that is queued to for a layout rebuild would freeze unity.
*   UI: Fix for issue with EventSystem and multiple sorting layers.
*   UI: Fix handling of the lastSelectedGameObject field on EventSystem. We don't use it so mark it obsolete.
*   UI: Fix instantiating a prefab containing a Selectables will not throw console errors.
*   UI: Fix issue where the pointer click world position/normal may not be properly associated with the event if multiple modules or hits are present.
*   UI: Fix Mac-only crash during Canvas sorting.
*   UI: Fix nested masking not getting the correct stencil value and failing
*   UI: Fix regression where deactivated UI components did not disappear.
*   UI: Fixed bug that multiple Layout Group components on the same GameObject was not prevented even though it is not supported.
*   UI: Fixed bug which caused caret to no longer appear in InputField after game object was deactivated and reactivated.
*   UI: Fixed crash when opening a scene with a deleted prefab canvas object.
*   UI: Fixed division by zero bug in GridLayoutGroup.
*   UI: Fixed events being blocked by disabled UI elements
*   UI: Making input field respect vertical alignment.
*   UI: Only do cut, copy, paste, and select all if holding down just Ctrl (Cmd on Mac), not if additional modifier keys are also held down. This prevents these actions from happening when intending to type characters that use Ctrl (Cmd on Mac) as part of the key combination.
*   UI: Prevent out of range exception that happened in InputField under certain circumstances due to an unwanted recursive call.
*   UI: Properly handle deselection if the current hovered object is destroyed.
*   Version control: Fix 'show in explorer' context menu
*   WebGL: Correctly show warning that building for WebGL is not supported in 32-bit editors
*   WebGL: Fix "Unknown Error" being displayed in Firefox at startup
*   WebGL: Fix artifacts in imported AudioClips
*   WebGL: Fix asm.js validation errors
*   WebGL: Fix audio channels being flipped left and right
*   WebGL: Fix AudioListener.volume
*   WebGL: Fix AudioSource.mute
*   WebGL: Fix banding issues in Standard Shader
*   WebGL: Fix build process running out of memory when compiling very large functions
*   WebGL: Fix Doppler effect simulation issues in various browsers
*   WebGL: Fix issue with Color32 serialization which could cause data corruption
*   WebGL: Fix Joystick buttons in WebGL when joystick ID is not specified
*   WebGL: Fix looping of audio
*   WebGL: Fix Marshal.StringToHGlobalUni
*   WebGL: Fix some keys being correctly detected in Chrome
*   WebGL: Fix Unity logo in default template
*   WebGL: Fix usage of custom templates on windows
*   WebGL: Handle gravity in particle systems better when physics module is stripped
*   WebGL: Make Profiler work on Windows
*   WebGL: Make WebGL correctly detect the Command key on OS X
*   WebGL: Memory sizes are now clamped to valid values
*   WebGL: OnApplicationQuit now correctly gets called
*   WebGL: Will now show rendering path UI in WebGL Player settings
*   WebGL: WWW class will correctly report errors
*   WebGL: WWW.progress now correctly reports values between 0 and 1
*   WebGL/iOS: Fix crash in UnusedBytecodeStripper on BoxCollider2D/CircleCollider2D center member access
*   Windows Phone/Store: Fix assembly converter crashing when a type generic class derives from a generic class which has a generic parameter that is array of generic parameters of the derived class (e. g. class Derived : MyBase).
*   Windows Phone/Store: Fix assembly converter crashing while postprocessing player if non-matching PDB is found.
*   Windows Phone: Fixed anti aliasing for render textures on phones with software navigation buttons.
*   Windows Store Apps/Windows Phone: fix AssemblyConverter failing for structs in other assemblies
*   Windows Store Apps: Added missing targets 'metroplayer', 'wsaplayer' when used with -buildTarget argument.
*   Windows Store Apps: extended splash screen should not be related to composition scale
*   Windows Store Apps: fix build failure when project path contains word "Assets"
*   Windows Store Apps: Fix building and running from directory with Unicode characters in ti.
*   Windows Store Apps: Fix reported log type for exceptions
*   Windows Store Apps: Fixed crash if using an unsupported image effect.
*   Windows Store Apps: Fixed deadlock when resizing window.
*   Windows Store Apps: Plugin folders (for ex., \*.bundle) will be ignored and won't cause an error, even if the plugin is selected as compatible with Windows Store Apps.
*   Windows Store Apps: Touch positions will be correctly reported when SwapChainPanel occupies only part of the screen.
*   Windows Store Apps: use XAML Frame and navigation
*   XboxOne: GI files that are part of the mainData will be included in the package manifest.
*   XboxOne: Launch range is now capped to the number of scenes rather than scenes+1.
*   XboxOne: Removed additional null character in persistantDataPath.
*   XboxOne: special characters are removed from Product name, avoiding use of characters the packaging tools don't like.
*   XboxOne: Systems that use a cache now use the console's T: drive.