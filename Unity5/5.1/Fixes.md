# Unity 5.1
https://unity3d.com/unity/whats-new/unity-5.1

## Fixes

<ul>
<li>2D: Added Vector2.down and Vector2.left properties</li>
<li>2D: Always default to use "Rect" tool if project started as a 2D project.</li>
<li>2D: Always prompt user to apply unapplied texture setting before opening up Sprite Editor Window.</li>
<li>2D: Apply button now work correctly between sprite editor window and sprite inspector.</li>
<li>2D: Avoid editing/deleting a polygon collider point while panning the scene view.</li>
<li>2D: Do not display sprite mesh wireframe in scene view under any circumstances</li>
<li>2D: Double Clicking on a Sprite will not ignore External Tools prefs now.</li>
<li>2D: Fixed occasional crashes while building on 'Repacking sprite aliases'</li>
<li>2D: Fixed some edge cases that will result in odd shape during sprite editor's automatic slicing.</li>
<li>2D: Fixed Corrupted Sprites in Sprite Packer for iOS and Android</li>
<li>2D: Fixed error appeared if Sprite was sliced only for 1 slice</li>
<li>2D: Height and Width of a sprite rect in Sprite Editor Window will no longer be 0.</li>
<li>2D: Losing focus in Sprite Editor will now always show Apply/Revert popup.</li>
<li>2D: Material field from SpriteRenderer no longer behaves as array type.</li>
<li>2D: Revert button will reset value correctly in sprite editor window.</li>
<li>2D: Scene View picking always picks the visually top-most for different SortingLayers and z-depths</li>
<li>2D: Show both original and atlas format in the preview for packed sprite sheet.</li>
<li>2D: Slicing by grid in Sprite Editor Window will now limit the input values to the size of the texture.</li>
<li>2D: Sprite Atlas will no longer produces errors at low resolutions</li>
<li>2D: Sprites now generate Preview Images in the Inspector when using object field</li>
<li>2D: Undo will not undo applied Sprite Editor Window changes.</li>
<li>2D: Using trim button in Sprite Editor window will correctly enable Apply/Revert button.</li>
<li>Android: Buildpipe - detect plugin errors when package names differ only by cases</li>
<li>Android: Fix for spaces being replaced with underscores in app titles</li>
<li>Android: Input - Fix axis stuck on Android TV after hiding keyboard</li>
<li>Animation: Adding a new curve to an AnimationClip with AnimationClip.SetCurve now update correctly the animation length</li>
<li>Animation: Fixed a bug where callbacks called indirectly from ApplyOnAnimatorIK would reset the animator memory and cause a crash</li>
<li>Animation: Fixed animator controller window title</li>
<li>Animation: Fixed Animator exception (m_IsVisibleInScene &amp;&amp; IsInScene()) == m_IsVisibleInScene) when disabling a game object with a disabled mesh renderer</li>
<li>Animation: Fixed copy paste of Animator State with StateMachineBehaviour , StateMachineBehaviour instances were not cloned correctly</li>
<li>Animation: Fixed crash when a StateMachineBehaviour disables his own animator component</li>
<li>Animation: Fixed CycleOffset range for animator state, valid range is between 0 and 1</li>
<li>Animation: Fixed direct blendtree editor slow down when there is too much motion</li>
<li>Animation: Fixed duplicated parameter in blend tree of blend tree</li>
<li>Animation: Fixed Livelink of AnyStateTransitions</li>
<li>Animation: Fixed transitions disappearing when importing a project from 4.x</li>
<li>Animation: Fixed update issue with Animator parameter window when going into playmode. Parameter list in the window was not updated anymore.</li>
<li>Animation: Fixes crash when disabling animator in OnAnimatorMove</li>
<li>Animation Window: Disable renaming items in animation window add property popup</li>
<li>Animation Window: Dragging sprite(s) to empty clip</li>
<li>Animation Window: Editing tangents in dopesheet context menu will save changes and handle undo correctly</li>
<li>Animation Window: Fixed an issue where keys on some curves were harder to click than others</li>
<li>Animation Window: Keyframe of missing sprite no longer has weird visual offset in the dopesheet</li>
<li>Animation Window: No more errors when changing to curve tab with sprite animation</li>
<li>Animation Window: Prevent dragging other object types to Sprite curve</li>
<li>Animation Window: Record mode is correctly cancelled when non-animated object is selected or new scene is created</li>
<li>Asset Loading: Always build the manifest AssetBundle and return the AssetBundleManifest object.</li>
<li>Asset Loading: Throw exception when calling Resources.LoadAll with null path.</li>
<li>Asset Management: Fix the crashes when saving with deleted gameobject</li>
<li>Asset Management: Unity packages now include .meta files for folders, allowing plugin settings for OS X native plugins to be transferred correctly</li>
<li>Asset Store: Fix download progress for packages larger than 2GB</li>
<li>Core: Fixed some memory leaks in the Editor and Players.</li>
<li>Editor: Breaking prefab instance through the menu "GameObjects-&gt;Break prefab instance" can now be undone</li>
<li>Editor: Calling Undo.RecordObject on editor objects no longer dirties the scene.</li>
<li>Editor: Clear old main menus on OSX</li>
<li>Editor: Do not change selection when duplicating while dragging</li>
<li>Editor: Fix crash when two inspector windows are open</li>
<li>Editor: Fix cubemap preview icons showing as white textures in Project Browser and Object Picker. </li>
<li>Editor: Fix DecoratorDrawers being shown twice for properties with custom PropertyDrawers that call into the default PropertyField implementation.</li>
<li>Editor: Fix default cursor appearing during editor startup on OSX</li>
<li>Editor: Fix Float Fields not accepting Infinity correctly</li>
<li>Editor: Fix GUIStyle errors on import (delay GUIStyle initialization to OnGUI).</li>
<li>Editor: Fix layers popup showing in the top left of the window and not below layers button.</li>
<li>Editor: Fix player settings window accessing non-initialized property.</li>
<li>Editor: Fix text fields content switch between build settings in some cases.</li>
<li>Editor: Fix undo of reset position/rotation/scale</li>
<li>Editor: Fixed crash when attempting to add the same component twice to a GameObject in the Editor</li>
<li>Editor: Fixed warning when dragging'n'dropping a mesh onto a GameObject</li>
<li>Editor: Make Android and iOS splash screen separate settings (no longer shared)</li>
<li>Editor: Plugin inspector - set ARMv6 Android plugins incompatible to avoid collisions</li>
<li>Editor: Scene View will no longer have tint applied when entering play mode.</li>
<li>Editor: Update m_GUIDToPath when moving asset to path name with different case.</li>
<li>Editor: Update menu items when assemblies are loaded in the editor</li>
<li>Editor: Update ShaderGUI for MaterialEditor when shader changes</li>
<li>Editor: Use IntField instead of FloatField for Sprite Editor</li>
<li>Fix issue where UnityEvents would lose their target function on assembly rebuild</li>
<li>Fix null reference on EventTrigger component when accessing delegates list. Some situations could cause it to not be initialized.</li>
<li>GI: Fix temporary visual glitch caused by missing atlas textures when a new lighting build is switched in when in auto lighting mode.</li>
<li>GI: Fix temporary visual glitch caused by missing UVs when a new lighting build is switched in when in auto lighting mode.</li>
<li>Graphics: Fixed AfterDepthTexture and AfterDepthNormalsTexture command buffers to be executed after the texture is set as a shader property.</li>
<li>Graphics: Fixed crash in a case where particle system would not have a valid mesh</li>
<li>Graphics: Fixed crash in Instantiate(Mesh) when static batching is used for the Mesh</li>
<li>Graphics: Fixed crash where MeshCombiner would not allocate enough indices</li>
<li>IMGUI: Fixed NullReferenceException when calling GUI.BeginScrollView with 7 arguments</li>
<li>iOS: Fixed duplicate property value removal in certain Xcode projects</li>
<li>iOS: Fixed Xcode project supported platforms and SDKs settings</li>
<li>Lightmapping: Fixed race condition crash in lightmap bake when converting .exr files.</li>
<li>Linux: Fix applying vsync and antialiasing changes without changing quality level</li>
<li>Linux: Fix OS version check when lsb_release isn't present.</li>
<li>Linux: Support more standard screen resolutions</li>
<li>Merge Tool: Handle regression in 5.0.1 introduced by stripped prefabs</li>
<li>Merge Tool: Fix auto fallback spec file detection</li>
<li>OSX: background image used for mac installer packages has been increased in size</li>
<li>OSX: Fix "Default is native resolution" setting.</li>
<li>OSX: Fix resolution update race when resizing window.</li>
<li>OSX: Prevent idle sleep while the player is active</li>
<li>Prevent accidentally moving multiple times when navigating UI with keyboard or controller by introducing a repeat delay to the StandaloneInputModule. This is similar to the delay before the repeating events that OSes have.</li>
<li>Profiler: Fix lockup in editor, if left in background with the profiler open</li>
<li>Profiler: Fix receive buffer error and hang connection when transferring large chunk of profiler's data</li>
<li>ReflectionProbes: Buttons "Bake All Reflection Probes" in Lighting window and Reflection Probes inspector should behave correctly now.</li>
<li>Scripting: Fix plugin verification crash on reload/shutdown</li>
<li>Scripting: Fix potential crashes on Webplayer</li>
<li>Serialization: Fix crash when loading text serialized scene with &gt;32k components</li>
<li>Serialization: Reapplied part of non-deterministic material serialization fix, but without increasing memory usage during building</li>
<li>Shaders: Add warning when using SV_POSITION in vertex shader inputs on DX11, and improve error message.</li>
<li>Shaders: Fix standard shader cutout rendering being wrong when rendering with shader replacement.</li>
<li>Shaders: Fixed #pragma target and #pragma exclude_renderers parsing with trailing comments.</li>
<li>Shaders: Fixed HLSL log10() translation into OpenGL/Metal platforms.</li>
<li>Shaders: Fixed shader compilation warnings not being shown if there are no compilation errors.</li>
<li>Shaders: Fixed that surface shaders vertex color field had to actually be called "color" (now just COLOR semantic is enough, like the docs always said).</li>
<li>Substance: Fix hang in ProceduralMaterial::Clean().</li>
<li>Substance: Fix crash when assigning a shader that does not cause outputs to be generated (e.g. Unlit/Color) to a ProceduralMaterial.</li>
<li>Substance: Fix 'path != ""' assert when live-previewing a Substance from the Asset Store.</li>
<li>Substance: Global Illumination flags are now correctly handled by ProceduralMaterials.</li>
<li>Substance: Fix console spam related to the absence of '_MainTex' shader property.</li>
<li>Terrain: Fixed an issue where painting terrain features while holding down the right mouse button could lock the view tool.</li>
<li>Terrain: Fixed crash on creating terrain with large heightmap resolution by script</li>
<li>Terrain: Fixed crash when terrains are neighbored and drawHeightmap is set to false</li>
<li>Terrain: Terrain brush no longer intercepts mouse events if the mouse cursor doesn't intersect with any terrain.</li>
<li>UI: Caret on InputField now blinks at proper frequency.</li>
<li>UI: Clamp setting canvas group alpha between 0-1 on API call</li>
<li>UI: Destroying a RectTransform that is queued to for a layout rebuild would freeze unity.</li>
<li>UI: Fix for issue with EventSystem and multiple sorting layers.</li>
<li>UI: Fix handling of the lastSelectedGameObject field on EventSystem. We don't use it so mark it obsolete.</li>
<li>UI: Fix instantiating a prefab containing a Selectables will not throw console errors.</li>
<li>UI: Fix issue where the pointer click world position/normal may not be properly associated with the event if multiple modules or hits are present.</li>
<li>UI: Fix Mac-only crash during Canvas sorting.</li>
<li>UI: Fix nested masking not getting the correct stencil value and failing</li>
<li>UI: Fix regression where deactivated UI components did not disappear.</li>
<li>UI: Fixed bug that multiple Layout Group components on the same GameObject was not prevented even though it is not supported.</li>
<li>UI: Fixed bug which caused caret to no longer appear in InputField after game object was deactivated and reactivated.</li>
<li>UI: Fixed crash when opening a scene with a deleted prefab canvas object.</li>
<li>UI: Fixed division by zero bug in GridLayoutGroup.</li>
<li>UI: Fixed events being blocked by disabled UI elements</li>
<li>UI: Making input field respect vertical alignment.</li>
<li>UI: Only do cut, copy, paste, and select all if holding down just Ctrl (Cmd on Mac), not if additional modifier keys are also held down. This prevents these actions from happening when intending to type characters that use Ctrl (Cmd on Mac) as part of the key combination.</li>
<li>UI: Prevent out of range exception that happened in InputField under certain circumstances due to an unwanted recursive call.</li>
<li>UI: Properly handle deselection if the current hovered object is destroyed.</li>
<li>Version control: Fix 'show in explorer' context menu</li>
<li>WebGL: Correctly show warning that building for WebGL is not supported in 32-bit editors</li>
<li>WebGL: Fix "Unknown Error" being displayed in Firefox at startup</li>
<li>WebGL: Fix artifacts in imported AudioClips</li>
<li>WebGL: Fix asm.js validation errors</li>
<li>WebGL: Fix audio channels being flipped left and right</li>
<li>WebGL: Fix AudioListener.volume</li>
<li>WebGL: Fix AudioSource.mute</li>
<li>WebGL: Fix banding issues in Standard Shader</li>
<li>WebGL: Fix build process running out of memory when compiling very large functions</li>
<li>WebGL: Fix Doppler effect simulation issues in various browsers</li>
<li>WebGL: Fix issue with Color32 serialization which could cause data corruption</li>
<li>WebGL: Fix Joystick buttons in WebGL when joystick ID is not specified</li>
<li>WebGL: Fix looping of audio</li>
<li>WebGL: Fix Marshal.StringToHGlobalUni</li>
<li>WebGL: Fix some keys being correctly detected in Chrome</li>
<li>WebGL: Fix Unity logo in default template</li>
<li>WebGL: Fix usage of custom templates on windows</li>
<li>WebGL: Handle gravity in particle systems better when physics module is stripped</li>
<li>WebGL: Make Profiler work on Windows</li>
<li>WebGL: Make WebGL correctly detect the Command key on OS X</li>
<li>WebGL: Memory sizes are now clamped to valid values</li>
<li>WebGL: OnApplicationQuit now correctly gets called</li>
<li>WebGL: Will now show rendering path UI in WebGL Player settings</li>
<li>WebGL: WWW class will correctly report errors</li>
<li>WebGL: WWW.progress now correctly reports values between 0 and 1</li>
<li>WebGL/iOS: Fix crash in UnusedBytecodeStripper on BoxCollider2D/CircleCollider2D center member access</li>
<li>Windows Phone/Store: Fix assembly converter crashing when a type generic class derives from a generic class which has a generic parameter that is array of generic parameters of the derived class (e. g. class Derived : MyBase).</li>
<li>Windows Phone/Store: Fix assembly converter crashing while postprocessing player if non-matching PDB is found.</li>
<li>Windows Phone: Fixed anti aliasing for render textures on phones with software navigation buttons.</li>
<li>Windows Store Apps/Windows Phone: fix AssemblyConverter failing for structs in other assemblies</li>
<li>Windows Store Apps: Added missing targets 'metroplayer', 'wsaplayer' when used with -buildTarget argument.</li>
<li>Windows Store Apps: extended splash screen should not be related to composition scale</li>
<li>Windows Store Apps: fix build failure when project path contains word "Assets"</li>
<li>Windows Store Apps: Fix building and running from directory with Unicode characters in ti.</li>
<li>Windows Store Apps: Fix reported log type for exceptions</li>
<li>Windows Store Apps: Fixed crash if using an unsupported image effect.</li>
<li>Windows Store Apps: Fixed deadlock when resizing window.</li>
<li>Windows Store Apps: Plugin folders (for ex., *.bundle) will be ignored and won't cause an error, even if the plugin is selected as compatible with Windows Store Apps.</li>
<li>Windows Store Apps: Touch positions will be correctly reported when SwapChainPanel occupies only part of the screen.</li>
<li>Windows Store Apps: use XAML Frame and navigation</li>
<li>XboxOne: GI files that are part of the mainData will be included in the package manifest.</li>
<li>XboxOne: Launch range is now capped to the number of scenes rather than scenes+1.</li>
<li>XboxOne: Removed additional null character in persistantDataPath.</li>
<li>XboxOne: special characters are removed from Product name, avoiding use of characters the packaging tools don't like.</li>
<li>XboxOne: Systems that use a cache now use the console's T: drive.</li>
</ul>
