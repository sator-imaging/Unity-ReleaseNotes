# Unity 5.0

https://unity3d.com/unity/whats-new/unity-5.0

## Fixes

- [2D](#2d)
- [AI](#ai)
- [Android](#android)
- [Animation](#animation)
- [Asset Bundles](#asset-bundles)
- [Asset Import](#asset-import)
- [Asset Management](#asset-management)
- [Audio](#audio)
- [Blackberry](#blackberry)
- [Build Pipeline](#build-pipeline)
- [Cache Server](#cache-server)
- [Core](#core)
- [Debugging](#debugging)
- [Editor](#editor)
- [Fonts](#fonts)
- [Graphics](#graphics)
- [iOS](#ios)
- [IL2CPP](#il2cpp)
- [Installers](#installers)
- [Linux](#linux)
- [MonoDevelop](#monodevelop)
- [Networking](#networking)
- [OS X](#os-x)
- [Physics](#physics)
- [Scripting](#scripting)
- [Shaders](#shaders)
- [Substance](#substance)
- [Terrain](#terrain)
- [Version Control](#version-control)
- [Web Player](#web-player)
- [Windows Player](#windows-player)
- [Windows Phone](#windows-phone)
- [Windows Store Apps](#windows-store-apps)


### 2D

*   Sprite name can't be empty, or contain characters that are not supported in assets when created from Sprite Editor.

### AI

*   Fix for avoidance sampling being one frame delayed - resulting in error message: nei.params.priority >= ag.params.priority.
*   Fix crash when calling NavMeshManager::Triangulate without baked data
*   Fix crash when navmesh is removed from disk when in use
*   Fix crash when OffMeshLink component has "AutoUpdate" enabled - but no endpoint transforms assigned.
*   Fix issue where auto-generated offmeshlinks were generated only at the origin.
*   Fix issue where baking navmesh for a duplicated scene would destroy the original scenes navmesh
*   Fix issue where obstacles and other agents wouldn't be avoided correctly by NavMeshAgents. The fix can cause the agents to avoid other agents more than before. You can reduce the avoidance prediction time (NavMesh.avoidancePredictionTime) to tune down the avoidance.
*   Fix issue where using navmesh built with "Height Mesh" enabled would sometimes crash Unity.
*   Fix memory leak after navmesh baking of terrain meshes.
*   Fix problem where any change in rotation or scale would trigger re-carving regardless of specified move-threshold.
*   Fix regression where NavMeshAgent velocity would always have zero y-component.
*   More robust raycast. Fixes occasional wrong height when raycast terminates at navmesh edge.
*   Navmesh is loaded before agents are created in additively loaded scenes - no need to wait one frame
*   Offmesh link drop arrow is not connected to navmesh with big heights
*   Prevent path query to invalid/infinity positions.

### Android

*   Compensate for polygon shader Offset bug on Mali 400 GPU.
*   Fixed auto rotation, Input.acceleration and gyroscope when using a non-native activity
*   Fixed fullscreen switch when called in Awake or Start in the first scene.
*   Fixed leak when using ActivityIndicator.
*   Fixed manifest detection for Android library project plugins
*   Limited support for anti-aliasing in OpenGL ES 2.0 to devices that support anti-aliased FBOs
*   Fixed resource leak when using antialiased RenderTexture with OpenGL ES 3
*   Fixed script compilation errors when regular .js file is present in Assets/Plugins/Android/assets
*   Fixed SDK auto-update
*   Fixed Water4 standard asset rendering on some devices.
*   Fixed audio playback when non-stereo mode selected (by forcing stereo).
*   Internet reachability check now returns proper value if switching in and out of airplane mode.
*   Project folder is no longer locked by adb after entering play mode in the editor.
*   Reporting correct screen orientation even if OS refused to apply requested orientation.

### Animation

*   Animation Clip is now available immediately after being created automatically for GUI
*   Fixed bug where Avatar mask wasn't appliedcorrectly to animation clip preview in the model importer.
*   Fixed bug where Blending pivot wasnot scaled correctly. It mainly affected AvatarPreview gizmo display. It did not affect runtime eval.
*   Builtin materials are now editable in animation mode. The animation is stored on the clip not the material.
*   Changing a child blend tree will now update objects using that blend tree in the scene.
*   Changing Animator.applyRootMotion while playing will no longer reset the controller's state machine.
*   Delayed the graph rebuild when deleting transitions to fix a bug when deleting multiple transitions.
*   Fixed bug where deleting a transition would delete a layer.
*   Fixed various crashes, especially on malformed data values.
*   Fixed UI issues: UI not updating after undo, curves flickering in some cases, rename overlays not shown, applying body mask in import settings, preview sometimes changing values, blend shape previews and so on.
*   Fixed adding child to new BlendTree not showing up in graph
*   Fixed animation events executed incorrectly on mirrored states.
*   Fixed Animation not playing in previewer for Generic
*   Fixed Animation transition causing undefined movement (even with "apply root motion" disabled)
*   Fixed Animator.Play that did not work after Recording
*   Fixed Animator.Play() and Animator.CrossFade() playing the animator state at requested time 't + deltaTime' when it should be 't'.
*   Fixed AnimationClip with manually-created root motion curves with wrong Class type causes crashes
*   Fixed Blend tree adjust time scale for animation clip without speed, you should get a warning when there is no speed available to compute the time scale
*   Fixed Blend tree compute threshold. if there is not enough data to compute the threshold you should get a warning.
*   Fixed BlendTree that had child AnimationClip with the same name.
*   Fixed bug where an Avatar mask used for humanoid clip import was not setup with all human transform checked.
*   Fixed Characters stretch out during a transition interrupted by another transition
*   Fixed computation of Homogenous Speed in BlendTree with clips that have no speed
*   Fixed dependency of sprites in AnimationClip, sprites are missing when the game object with sprite Animation is loaded from Assetbundle.
*   Fixed drag of AnimationClip on GameObjet that has an AnimatorController.
*   Fixed evaluation of Curves with only one key.
*   Fixed Event evaluation when mirroring states.
*   Fixed feet pivot weight blending. Feet pivot weight was affected by blended clips even when their weights were very small
*   Fixed Humanoid going to relax pose on transition to state with no clip on 2nd sync layer
*   Fixed Humanoid rig playing animations differently than generic rig.
*   Fixed layer switching performance issue.
*   Fixed linear scale blending for additive layers.
*   Fixed multiple AnimationEvents at time 0 that were only firing the first AnimationEvent.
*   Fixed "Not Initialized" displayed on an Animator with valid Controller.
*   Fixed OnStateMachineEnter and OnStateMachineExit callbacks not being called.
*   Fixed packed NPOT sprite textures
*   Fixed Rect Transform z component not being animated
*   Fixed root motion still moving even if Root Transform Position(XZ) is baked.
*   Fixed several issues with Animation Events (event not fired, fired twice).
*   Fixed StateMachineEnter/Exit not being called on multi-layer component
*   Fixed transition error when a state had a speed of zero.
*   Fixed Transition previewer for very short clips.
*   Fixed UnloadNonDirtyStreams to correctly handle stream with destroyed objects.
*   Fixed unsynced AnimatorStateInfo and AnimatorClipInfo.
*   Generic Root Motion will be used for an additional Layer when no Mask is specified.
*   Prevented deletion of root blendTree in the BlendTree graph.
*   Prevented adding legacy animation to Mecanim.
*   Prevented creation of cycles in Blend Trees.
*   Propagated Animator invalidation on modification to AnimatorOverrideController to fix a crash when changing speed.
*   Rebakes euler angle curves on sample rate change.
*   Fixed Root Motion failing for very short clips.

### Asset Bundles

*   Asset Bundle Export performance increase.
*   AssetBundle.LoadAll\*\*\*() now only return the game object without the first component.
*   Fixed crash if user passes "./" as output path when building AssetBundles.
*   Fixed possible crash while loading multiple AssetBundles simultaneously.
*   Fixed the typo in .manifest file
*   Remove duplicate objects when building with BuildAssetBundleExplicitAssetNames(). Also output more meaningful log information for assetBundle object.

### Asset Import

*   Added ability to retry operation on write error when importing assets.
*   Added warning messages when paths to assets are invalid
*   Append required .fontsettings extension if needed in GenerateEditableFont
*   Check texture format that can be assigned the TextureImporter
*   Fixed AssetDatabase.ImportPackage fail when path to package has platform path separators.
*   Fixed crash when included blend shapes and needed to be split because of size.
*   Fixed crash when upgrading metadata files
*   Fixed import of empty .txt files.
*   Fixed import of Maya files with set driven keys.
*   Fixed problem when importing models with no diffuse color specified.
*   Fixed problems with animation importing incorrectly due to mirror/negative scale.
*   Support the manifest file in text importer.

### Asset Management

*   Added warning when using AssetDatabase.Load\* function with an absolute path
*   Fix assets unload during load level operation
*   Fixed crash while loading scene Unity with mecanim animation and skinnedmesh filter.
*   Fixed invalid cache state after cancelling WWW download.
*   Fix the "input objects must be of exact same type" error message
*   Prefabs: Fix crash if using DestroyImmediate() on prefab instance objects during prefab instantiation.
*   Prefabs: Fix crash when accessing physics component properties during OnValidate(). This includes a general change in behavior for OnValidate() calls during prefab instantiation and undos such that it follows the same order as when loading from disk.
*   Prefabs including monobehaviours with missing scripts should not display a warning if the monobehaviour has been deleted on the prefab instance.
*   Resources.Load will now correctly return NULL when there is no Object of the desired type with that name (instead of returning an object with a different type if it exists)
*   Serialization: Added ability to do automatic fix of invalid references to scripts in scene file (to valid registered scripts)
*   Serialization: Added error message with file information if SerializedFile header is corrupted
*   Serialization: Fixed bug that caused build corruption when serializing volatile fields.
*   Serialization: Fixed bug that caused build corruption when serializing classes for which a generic version exists
*   Serialization: Fixed the error message when removing an object in a custom inspector
*   Serialization: Fixed windows Layout loading if script for previously opened custom window is absent

### Audio

*   AudioClip.SetData no longer prints out error messages when writing data at a position that will cause wrapping.
*   Calling AudioClip.SetData causes a crash fixed
*   Fixed a bug where the audio system stopped working when a game object had an AudioSource, an AudioListener and a custom audio filter attached. The system now outputs a warning as the custom audio filter can only be assigned to one Audio component at a time.
*   Fixed Crash when exposing a parameter of an effect that was added to a group
*   Fixed for regression where component effects are on the AudioListener cause a crash
*   Fix importing Tracker files so that by default, they are set to load Compressed In Memory. This is also now configurable.
*   Fixed leaking audio resources when having AudioSources within a Prefab
*   Prevent data-race condition in AudioManager
*   Prologic DTS can now be selected as an audio output.
*   Remove exposed parameters correctly when deleting and effect that has exposed parameters in it.
*   Stability fix for custom audio filters placed on the AudioListener.
*   When audio clip was set to Load In Background project crashed on Android immediately

### Blackberry

*   Event.shift and Event.alt now work as expected.

### Build Pipeline

*   Don't include inactive EditorOnly objects in builds.

### Cache Server

*   Fix "CacheServer Asset validation failed" error messages while Unity is importing project.
*   Fix editor crash when enabling the Cache Server in preferences with empty address.

### Core

*   Fix crash when initializing Light from prefab object during scene loading.
*   Fix the bug that loading from cache returns false.
*   Fixed data race in memory allocators.
*   Runtime: Error message is now shown if you try to add a component of invalid type
*   Runtime: Fix Time.realtimeSinceStartup being wrong during Awake calls in initial level load.
*   Runtime: GameObject.FindObject nolonger stops and returns null if first match is an inactive game object.

### Debugging

*   Allow evaluation of methods with string literal parameters.
*   Don't interrupt user waits (e.g. ManualResetEvent).
*   Fix setting breakpoints in generic method implementations.
*   Fix some instances of debugger freezing or hanging.

### Editor

*   Added "-force-gl-ref" cmd-line option support for the OSX Editor.
*   Added link to editor settings when sprite packer is disabled
*   Animation Window refreshed when tabbed into
*   AnimationState.time is updated when scrubbing animation in the AnimationWindow.
*   Audio preview is refreshed after import settings are changed
*   CanvasGroup methods were not getting registered in the UI module, resulting in MissingMethodExceptions
*   Changing framerate in animation window now repositions animation events correctly
*   Cloth inspector to support multi-editing
*   Color picker code now has correct color space conversion and is now working accurately.
*   Confined cursor mode doesn't confine cursor to last active editor pane
*   Create a new project upgrade warning system that does not depend on serialized files or version control.
*   Deleting an asset does not make deleted objects from other assets appear again.
*   Disallow empty names for sprites
*   Don't ignore assets whose names contain "StreamingAssets"
*   Don't immediately hide popup windows when there are unity windows on secondary screen on OSX
*   Don't let user rename GameObjects with HideFlags.NotEditable set
*   Drag-and-drop does not accept simple Renderers as a valid target for assigning skybox material.
*   Editor no longer freezes when scene view camera is really far from origin
*   Empty animation window no longer increases CPU usage
*   Ensure correct waking order of components when duplicating a GameObject.
*   Ensure screen width and height in player settings is at least 1
*   Expose static methods from context objects to JS.
*   Fixed an occasional crash when reimporting shaders.
*   Fixed assetBundle search filter doesn't work correctly.
*   Fixed assert when loading scene containing reference to one of its objects that no longer exist.
*   Fixed asserts when displaying multiple objects in inspector preview.
*   Fix asset when using hideFlags to make objects persist after exiting play mode.
*   Fixed audio source priority slider showing "–" when editing multiple objects
*   Fixed AudioSourceInspector.cs throwing null refs on UndoRedoPerformed
*   Fixed broken inspector setup with multiple inspectors when shaders are using custom editors
*   Fixed changing loaded level index before OnApplicationQuit message when exiting play mode.
*   Fixed clipping of multi-line text in text fields.
*   Fixed confirmation dialog "Losing Prefabs" shown twice when trying to delete child object
*   Fixed console errors when inspecting player settings in debug view.
*   Fixed crash occasionally happens when you create a prefab. Related to the object sorting in the prefab.
*   Fixed crash when executing a menu item from a static constructor.
*   Fixed crash when maximizing game view on OSX.
*   Fixed crash when removing components from a prefab, but prefab instances would have depending components.
*   Fixed crash when script name is longer than 32 characters.
*   Fixed crash with corrupted scene when having invalid references in the list of transform children.
*   Fixed custom cursors to properly update in OS X editor.
*   Fixed custom PropertyDrawer being called with wrong SerializedProperty when property is inside a nested class.
*   Fixed double firing of playmodeStateChanged
*   Fixed Edge Collider 2D sometimes not showing handles
*   Fixed editor errors when undoing the insertion of a new LOD level in LOD group.
*   Fixed error spam: "GUI Error: You are pushing more GUIClips than you are popping .." when setting cam.targetTexture = null in OnPostRender.
*   Fixed exceptions happening when a read-only plugin is used.
*   Fixed font corruption after asset import.
*   Fixed freeze during Editor startup when using input devices with large number of emulated buttons (some wireless mouses)Fixed GameObject not selectable by label icon
*   Fixed freeze on floating-point exception
*   Fixed Import Package window being broken due to illegal characters in path
*   Fixed incorrect fade group animation in player settings
*   Fixed inspector rendering when a script changes RenderTexture.active.
*   Fixed isPlayingOrWillChangePlaymode to work as expected.
*   Fixed keyboard shortcuts (home/end/page up/page down) in object selector
*   Fixed Mac Editor Projects with hidden folders inside Assets are usable again
*   Fixed many texture/mesh related error messages to ping the source object that caused it.
*   Fixed material inspector could collapse its controls by clicking on the header. Controls are now always visible.
*   Fixed memory leak when calling 'Object.Destroy' and returning to edit mode.
*   Fixed meshes getting lost if they only lived in the scene and only were referenced by a mesh collider.
*   Fixed missing header for state machine behaviours
*   Fixed navigation keyboard shortcuts in object selector
*   Fixed NullReferenceException from uninitialized icon if CurveEditor is shown before Inspector
*   Fixed NullReferenceException when Tools.viewTool is queried outside OnGUI
*   Fixed numeric accuracy of transform coordinates when copy/pasting or duplicating objects.
*   Fixed occasional crash/hang on exit.
*   Fixed page down in object selector on Windows
*   Fixed position of GUI elements in inspector when using PropertyDrawers.
*   Fixed possible corruption of editor window rendering in OS X Editor.
*   Fixed possible crash when placing prefabs with child objects.
*   Fixed projectsettings.asset serialization error
*   Fixed property list in Animation Controller editor allowing to drag invalid element from bottom of list.
*   Fixed race condition in memory allocation system.
*   Fixed rename overlay is not removed when undoing
*   Fixed Skybox components not taken into account in camera preview popup
*   Fixed so TextMesh text field uses TextArea instead of single text field
*   Fixed Sprite Editor crash when docked to top of the layout
*   Fixed stack traces not being generated correctly.
*   Fixed text corruption in TextMesh components when reimporting fonts.
*   Fixed that text fields in an unfocused window could break another windows textfield if busy repainting
*   Fixed tooltips not always showing up when they should.
*   Fixed typing into the search field between transition animations for Add Component menu
*   Fixed unparenting when deleting object in Editor once OnDestroy is called
*   Fixed updating color fields in material inspector to work when warnings are displayed.
*   Fixed user cannot close a custom editor window from a previous project.
*   Fixed utility windows always loading last width & height if larger than requested width & height.
*   Fixed when mouse was not processed in the Editor in play mode after building Android or iOS.
*   Fixed Windows Editor not showing progress over taskbar icon, when doing initial project import.
*   Fixed Windows Editor unresponsive to user's input in some tablets.
*   Folders named "something.unity" will be listed as folders and not scenes in a search
*   FPS controls now only affects the active scene view
*   I18n: Issues with Asian Input Method Editors inside the Windows version of the Editor.
*   I18n: Issues importing assets when their path/asset/component names contain Asian characters.
*   I18n: Issues storing/retrieving strings from PlayerPrefs when PC is set to Asian locale.
*   I18n: Editor crashes on start-up if computer / user / project name contains Asian characters.
*   IMGUI: Fixed crash when using GUI.Window recursively.
*   IMGUI: Fixed line spacing when multiple sizes are used in text markup
*   IMGUI: Fixed renaming of existing controls using GUI.SetNextControlName.
*   IMGUI: ContextClick events are now never received by in-game GUIs (as documented, the event is editor only).
*   Initialize Scene View 2D mode correctly when upgrading from version
*   Input.mousePosition now returns correct position when called in Awake and Start in the editor
*   Make key combinations ignore Caps Lock key.
*   No more errors after applying new preset in the curve editor
*   Object Picker is now able to show a hierarchy of sub assets (used for AudioMixerGroups for now).
*   Opened scene will no longer be accidentally marked as modified.
*   Opening multiple locked inspectors works
*   OSX corner resize gizmo doesn't block input when not shown.
*   Packages: Fix importing package with long paths on Windows
*   Particles: Fixed particles that are out of view casting incorrect shadows.
*   Particles: Fixed systems using Distance emission not stopping correctly.
*   Particles: ParticleSystem will no correctly remove any of its particles and reset its emitter state when being deactivated.
*   Prevent each script from opening in a new Visual Studio instance.
*   Prevent MinMaxSlider getting into error state when clicking in the thumb area
*   Prevent right clicking on controls behind preview window
*   Reduce serialization depth limit warnings
*   Remove unsupported OSX menu items (Start Dictation & Special Characters)
*   Removing curve in animation window doesn't remove other curves with similar name
*   Reverting a prefab no longer fails if two added components depends on each other.
*   Select Dependencies operation no longer breaks editor fonts
*   Shadows working correctly when zoomed in animation preview window
*   Show at most one error when attempting to deleting multiple components
*   Sprite name was emptied when copy pasting position etc. values on editor
*   Swatches in the Color Picker tool are now gamma corrected when using linear colour space.
*   Synchronize EditorUserBuildSettings.selectedStandaloneTarget when switching build targets with SwitchActiveBuildTarget() or -buildTarget.
*   Tooltips use current skin instead always using light skin
*   Warn in Lighting window UI when a skybox with nonsensical shader is used
*   Will exit play mode when switching build platform.
*   Unity crashes while adding component to destroyed object.
*   Undoing changes in the Animator throws an error.
*   Use unique sprite name when creating new sprites manually

### Fonts

*   Fixed a bug where regenerating font textures might miss needed characters from the last frame.
*   Fixed fallback to default font for characters missing in customs fonts on platforms without OS font access.

### Graphics

*   Camera.RenderToCubemap will correctly work with AA render texture.
*   D3D11: Fixed an issue which caused some objects not be rendered if shadows are enabled in the scene on feature level 9.x
*   Deferred Lighting is disabled for oblique camera projections; falls back to forward rendering now. Before, it was just not working properly, without a proper fallback.
*   DX11, fixed GL.Clear when we have MRTs (only first target was cleared before).
*   Fixed HDR support for SunShafts image effect.
*   Fixed incorrect warning about NPOT texture filtering
*   Fixed occasional crash on creating and immediately deleting particle renderer.
*   Fixed RenderTextureFormat.Default and DefaultHDR only working with RenderTexture.GetTemporary(), not with permanent RenderTextures.
*   Fixed shadow caster culling for orthographic cameras.
*   Fixed Skybox not rendering with some edge cases of supported vs. not supported shaders
*   Fixed Texture2D.EncodeToPNG being very slow for large images. E.g. for 4096x4096 image, it's now almost 10x faster!
*   Fixed "Tiled GPU perf. warning" in editor resulting in poor performance.
*   Fixed warning thrown on saving scene by mark the meshes as DontSave
*   GI: Fixed tetrahedralization issues with small floating point differences in probe positions.
*   GLES: Fixed rendering bug that occurs when native rendering plugin calls glViewport
*   Image Effects: Fixed some ImageEffectOpaque effects making later alpha blended geometry not render with correct Z-buffer.
*   Make sure to never use soft particles when in orthographic camera, since depth-based fadeout does not work there.
*   OpenGL: Detected cases on Windows when no OpenGL drivers are installed and exit properly.
*   OpenGL: Don't force texture/shader reload when changing resolution (breaks baked lighting, etc.)
*   OpenGL: Fixed GLSL fragment shader incorrectly tagged as a Fixed Function pipeline shader.
*   OpenGL: Fixed RenderTextures on Windows 64-bit standalone using OpenGL.
*   OpenGL ES: Enforce RGB normal maps even if source texture have alpha.
*   OpenGL ES: Some performance improvements by removing redundant GL API calls.
*   Rendering: Fix crash when closing Standalone player in DX11 render mode.
*   Rendering: Fix memory leak when dynamic geometry chunk did not add any vertices.
*   Rendering: Fixed crash when reading font's metadata for a font without style info.
*   Shadows: Fixed flickering/inconsistent shadows when light culling masks cause more than one light to be "main light" in forward rendering.
*   Shadows: Fixed shadowmaps being re-rendered when using deferred shading with some forward-shaded objects.
*   Shadows: Fixed some cases where alpha-tested shadow caster objects were wrongly batched together, even if they used different textures.
*   Shadows: Fixed spot light shadow bias to be more sensible. Was highly non-linear before.
*   Tint calculation in Skybox shaders is done more properly when in Linear color space now.

### iOS

*   Check whether an ad is loaded in ADInterstitialAd.Show()
*   Correctly implement Marshal.Copy for arrays.
*   Delete newlines when pasting into single line edit boxes
*   Disable informational warnings on non-development build
*   Don't pass touches through iOS keyboard's toolbar
*   Don't spam the console log with GameKit stuff on release builds
*   Fixed GetLoadedDylibs to not to include the app exe in the results
*   Fixed Info.plist append
*   Fixed launch screen support
*   Fixed memory leaks related to UTF8String.
*   Fixed project append
*   Fixed random crash when changing orientation by 180 degrees
*   Fixed severe visual issues when setting Screen.orientation when autorotation is disabled
*   Fixed special character treatment in Info.plist
*   Fixed splashscreens for landscape orientation on iOS 7 and newer
*   Fixed visual issue in Player settings
*   Fixed wrong frame buffer size on iPhone 6+
*   Ignore SIGPIPE signal which is thrown by broken sockets
*   Improved iOS device name detection.
*   Made advertisement ID calls dynamic to avoid App Store rejections.
*   Report size of assemblies after bytecode stripping
*   Support multiple permission types in {Request,Has}UserAuthorization
*   Use new remote notification API on iOS 8
*   Use separate font metadata caches for each iOS version
*   Workaround for iOS 8.0 GameController API crash bug

### IL2CPP

*   Correctly handle the Duv\_Un IL opcode with signed arguments to prevent an error from IL2CPP like this: "Unexpected types used with Div\_Un opcode. Types are Int32 and Int32"
*   Correctly throw a managed exception when an array is created with a negative size.
*   Handle custom attributes on events correctly.
*   UnityEngine.dll methods that are targets of UI events are no longer incorrectly stripped
*   Write proper include directives for all fields of marshaled structures or classes.

### Installers

*   Windows: No longer specifying the "Editor" subfolder of path when installing Unity.
*   Windows: Uninstall MonoDevelop when uninstalling Unity.

### Linux

*   Call OnApplicationQuit callbacks for all methods of quitting the player.
*   Constrain size of screen selector banner image.
*   Filter aspect ratios in screen selector.
*   Fix hotspot desynchronization with custom cursors when hiding/reshowing.
*   Fixed spotlight shadow filtering on Linux - now uses hardware PCF just like Win/Mac.
*   Improve system language detection.

### MonoDevelop

*   Fixed exception when resolving symbolic breakpoints.
*   Fixed issue with Cmd+A (Select All) keyboard shortcut not working correctly on OSX after using the main menu.
*   Fixed “jumping cursor” issue.
*   Fixed opening the same file twice in MonoDevelop.
*   Updated versions of Mono/GTK used, fixing scrolling issues with some mice.

### Networking

*   WWW on local file system can accept non-ASCII filenames on Windows.

### OS X

*   Mac OS X Standalone: Fix crash changing if resolution in batch mode.
*   Mac OS X Standalone: IME Input now works in the 64-bit Standalone player.

### Physics

*   Cloth: fixed cloth exploding for any non-trivial model imported from FBX.
*   Cloth: fixed rotation being applied twice
*   Cloth: improved simulation quality, fixed a bug where cloth simulation would be dramatically affected by fps
*   Collider.Raycast will now not hit disabled colliders
*   ConstantForce2D torque should be in degrees not radians.
*   Prevented negative values being set for CharacterController.stepOffset.
*   Enabled flag on CharacterController now correctly keeps its state.
*   Fixed cloth vertices renderer (was rendering vertices rotated in editor mode)
*   Fixed crash when applying force to inactive Rigidbody
*   Fixed crash when doing a Raycast() on a collider that failed initialization
*   Fixed explosion force when position is inside collider's world AABB.
*   Fixed HingeJoint spring's targetPosition range that was incorrect.
*   Fixed Physics.IgnoreCollision
*   Fixed regression where property changes in the editor did not update the 2D collider in the scene view.
*   Fixed rotation mode combo for ConfigurableJoint.
*   Fixed terrain colliders returning sharedMaterial == null
*   Fixed that TransformChanged events could re-create the Cloth component, even though the component was already cleaned up.
*   Implement Undo for Cloth editor.
*   Make sure explicit inertia tensor is not reset when modifying colliders
*   Send OnControllerColliderHit on collisions with another CharacterController reliably.
*   Set default physic material properties to match values in PhysX SDK
*   Support sending OnTriggerExit when collider is deactivated or destroyed
*   WheelCollider: fixed a bug where attachedRigidbody would be equal to null
*   WheelCollider: fixed a bug where editor would crash soon if you use sliders to tune WheelCollider properties.
*   WheelCollider: fixed wrong behaviour after changing mass of parent rigidbody

### Scripting

*   Ensure all children receive broadcast messages even if the transform hierarchy changes during a callback from the message.
*   Fixed adding EllipsoidParticleEmitter / MeshParticleEmitter components
*   Fixed crash if a MonoBehaviour was created in MonoBehaviour OnDisable.
*   Fixed crash in callback
*   Fixed crash when calling DestroyImmediate in MonoBehaviour constructor
*   Fixed crash when calling user log callback from a non-main thread
*   Fixed exceptions being thrown when calling Object.FindObjectsOfType().
*   Fixed ExclusiveAddressUse socket flag on windows
*   Fixed for some debugger freezes / crashes while debugging on OS X and Windows.
*   Fixed internal compiler error when script defines are duplicated
*   Fixed process querying on OSX
*   Fixed some cases when using a class name that collides with an internal class name in a different namespace (e.g. BuildSettings)
*   Fixed StackOverflowException handling on 64-bit Windows
*   Fixed webplayer not auto-starting as requested when calling BuildPlayer with Windows-style paths.
*   Invoking DllImport from various threads, should be thread-safe now.

### Shaders

*   Better error message when a shader is using properties that clash with built-in Unity global properties.
*   Fixed \_CameraToWorld and \_WorldToCamera matrices being wrong while rendering into a cubemap, or when custom camera.worldToCameraMatrix is set.
*   Fixed DirectX 11 shader compilation when Unity is installed in a path with non-ascii characters.
*   Fixed hlsl-to-glsl translation problem with expressions that initialize a matrix with a scalar (float3x3 m = 0).
*   Fixed issue with generated projects (.csproj) sometimes not having a reference to UnityEngine.UI.dll
*   Fixed legacy Diffuse Detail shader when in linear color space.
*   Fixed loading of some GLSLPROGRAM shaders with preprocessor macros on OpenGL ES
*   Fixed "Maximum number of shader keywords" error in editor resulting in really bad build-time performance.
*   Fixed some cases where surface shader compiler was producing error about "too many texture interpolators" with no further details.
*   Fixed surface shader compilation bug where keywords like "nolightmap novertexlights" were not properly excluding all needed variants.
*   Fixed surface shader compilation bug with some combinations of #pragma multi\_compile / shader\_feature.
*   Fixed unnecessary truncation of float constants on GLSL platforms.

### Substance

*   Emissive outputs assigned to \_EmissionMap shader slots now correctly trigger the emissive effect when the material is loaded.
*   Fix case where the editor-side Substance cache data would not be reused when it should.
*   Fix crash in standalone builds when loading a SBSAR with both BakeAndDiscard instances and non-baked instances.
*   Fix crash when inspecting baked ProceduralTextures.
*   Fix texture corruption issue in standalone builds where modifying an input value and calling RebuildTextures() on a ProceduralMaterial with image inputs and whose outputs have been read from cache would result in black textures being generated.
*   Grayscale image inputs are now supported.
*   ProceduralMaterials only referred to by their outputs and not by their attached material now load properly.

### Terrain

*   Custom material's shader keywords now will be correctly applied.
*   Doing vertex snapping for terrain objects no longer crashes the editor.
*   Fixed assertion when loading a scene with TerrainData objects embedded.
*   Fixed broken tree colliders.
*   Fixed corrupted rendering when being edited.
*   Fixed crash when importing detail meshes with float color channel.
*   Fixed "m\_UniqueThreadAllocator->GetAllocatedMemorySize() == 0" error after "Mass Place Trees".
*   Fixed some memory leaks.
*   Tree imposters lighting is now matched with lighting on mesh trees.

### Version Control

*   Add missing icon for incoming changesets.
*   Auto connect when connection is dropped.
*   Correct local/remote args for diff tool.
*   Do not print a warning when saving scene and file is not opened for edit unless necessary.
*   Fixed case handling on Windows when downloading files.
*   Fixed editor crash on loading terrain with corrupted detail layers.
*   Make it possible to retry a hanging connect while connecting.

### Web Player

*   Correctly verify generic reference type constraint for generic parameter with type constraint which is a reference type.

### Windows Player

*   Deployment Management: Simpler "Force Single Instance" error message on Windows
*   Deployment Management: Fix StandalonePlayer launched from UNC path
*   DirectX 11: Mip mapped cubemaps now work correctly on feature level 9.x. This fixes the smoothness setting in the standard shader.
*   DirectX 11: Unity will now correctly detect if hardware doesn't support a particular cubemap size, and will try to skip higher mip maps instead of failing to upload the cubemap at all.
*   Fixed fullscreen player sometimes disappearing behind other windows on startup.
*   Return the correct value from PlayerPrefs::SetString
*   Windows 10 reports SystemInfo.operatingSystem string properly.

### Windows Phone

*   Windows Phone 8.1: Enabling location capability no longer causes a crash.
*   Windows Phone 8: Tap count is now correctly calculated when using multiple fingers.
*   Windows Phone/Windows Store Apps: Generic list of structs is now properly serialized.
*   Windows Store Apps/Windows Phone: added support for animating script variables that are members of structs.
*   Windows Store Apps/Windows Phone: fixed sprite animation on GUI elements
*   Windows Phone 8.1: Enabling "Human Interface Device" capability in player settings no longer makes Unity generate invalid application certificate.
*   Windows Phone 8.1: Fixed Handheld.Vibrate().
*   Windows Phone: Fixed Handheld.PlayFullscreenMovie().
*   Windows Phone 8.0: Fixed GUI text rotation when device is in landscape orientation and rendering to a render texture.
*   Windows Phone 8.0: Fixed image effects when device is in landscape orientation.
*   Windows Phone 8.0: Trying to access webcam without appropriate capabilities in application manifest will no longer constantly throw exceptions.
*   Windows Phone 8.0: Fixed Unity generating invalid references in Visual Studio project, debug configuration.
*   Windows Phone: Texture2D.ReadPixels now works correctly in landscape modes.
*   Windows Phone: fix crash on application exit when location is enabled
*   Windows Store/Phone: Cloth.coefficients now work correctly
*   Windows Store Apps/Windows Phone: You can now render to cubemaps on DX11 9.x feature levels.
*   Windows Store/Phone: Depth render textures are not really supported on DX11 9.x feature levels, but previously they were wrongly claimed to be supported.
*   Windows Phone/Windows Store Apps: Gyroscope.gravity returns same values as other platforms. It used to be inverted before.
*   Windows Phone 8: Camera.ViewportToWorldPoint returns correct value in orthographic view.
*   Windows Store Apps/Windows Phone: fix taking detailed memory sample in profiler
*   Windows Phone 8: setting keyboard text just after creating it will not be in vain anymore.
*   Windows Store Apps / WIndows Phone 8: Matrix4x4 will be correctly serialized
*   Windows Store Apps/Windows Phone: fix profiler not working after reopening the editor
*   Windows Store Apps/Windows Phone: better error messages when AssemblyConverter fails to resolve type.
*   Windows Store Apps/Windows Phone: fix AssemblyConverter failing on struct from unprocessed or system assemblies

### Windows Store Apps

*   Added missing defines UNITY\_WSA, UNITY\_WSA\_8\_0/UNITY\_WSA\_8\_1 in generated Assembly-CSharp-\* projects.
*   Fixed building Universal apps in batch mode
*   Fixed crash when WebcamTexture is destroyed
*   Fixed errors in the editor when player settings are open and upgrading scripts or switching platform
*   Fixed high CPU when Unity is paused
*   Fixed issue when App bar couldn't be open with mouse right-click while Independent Input source is enabled.
*   Fixed mouse callbacks
*   Fixed native plugin not included in generated Visual Studio solution
*   Fixed serialization error when serializing object derived from System.Object and Compilation Overrides are set to .NET Core.
*   Fixed SerializationWeaver failure when scripts reference classes in plugins
*   Fixed UnityScript breaking exported solution with SDK 8.0
*   Native plugins now properly added to generated solution
*   Unity now regenerate test certificate, if it was deleted, rather than failing to build project.
*   runInBackground checkbox will now warn about wack failure that it might cause.
*   UNITY\_WINRT\_8\_1 and UNITY\_WINRT\_8\_0 will be correctly defined now.
*   Unity will now store certificate path as a relative path, so when project is moved to another PC, it will be still found.
*   When building player files are now copied directly to destination directory bypassing staging area, reduces project size when submitting a bug
*   You can now use HashAlgorithm & MD5CryptoServiceProviders classes in C# files compiled against .NET Core.