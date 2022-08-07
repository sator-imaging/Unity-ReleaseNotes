# Unity 5.0
https://unity3d.com/unity/whats-new/unity-5.0

## Fixes


### 2D
<ul>
<li>Sprite name can't be empty, or contain characters that are not supported in assets when created from Sprite Editor.</li>
</ul>

### AI
<ul>
<li>Fix for avoidance sampling being one frame delayed - resulting in error message: nei.params.priority &gt;= ag.params.priority.</li>
<li>Fix crash when calling NavMeshManager::Triangulate without baked data</li>
<li>Fix crash when navmesh is removed from disk when in use</li>
<li>Fix crash when OffMeshLink component has "AutoUpdate" enabled - but no endpoint transforms assigned.</li>
<li>Fix issue where auto-generated offmeshlinks were generated only at the origin.</li>
<li>Fix issue where baking navmesh for a duplicated scene would destroy the original scenes navmesh</li>
<li>Fix issue where obstacles and other agents wouldn't be avoided correctly by NavMeshAgents. The fix can cause the agents to avoid other agents more than before. You can reduce the avoidance prediction time (NavMesh.avoidancePredictionTime) to tune down the avoidance.</li>
<li>Fix issue where using navmesh built with "Height Mesh" enabled would sometimes crash Unity.</li>
<li>Fix memory leak after navmesh baking of terrain meshes.             </li>
<li>Fix problem where any change in rotation or scale would trigger re-carving regardless of specified move-threshold.          </li>
<li>Fix regression where NavMeshAgent velocity would always have zero y-component.</li>
<li>More robust raycast. Fixes occasional wrong height when raycast terminates at navmesh edge.</li>
<li>Navmesh is loaded before agents are created in additively loaded scenes - no need to wait one frame</li>
<li>Offmesh link drop arrow is not connected to navmesh with big heights</li>
<li>Prevent path query to invalid/infinity positions.</li>
</ul>

### Android
<ul>
<li>Compensate for polygon shader Offset bug on Mali 400 GPU.</li>
<li>Fixed auto rotation, Input.acceleration and gyroscope when using a non-native activity</li>
<li>Fixed fullscreen switch when called in Awake or Start in the first scene.</li>
<li>Fixed leak when using ActivityIndicator.</li>
<li>Fixed manifest detection for Android library project plugins</li>
<li>Limited support for anti-aliasing in OpenGL ES 2.0 to devices that support anti-aliased FBOs</li>
<li>Fixed resource leak when using antialiased RenderTexture with OpenGL ES 3</li>
<li>Fixed script compilation errors when regular .js file is present in Assets/Plugins/Android/assets</li>
<li>Fixed SDK auto-update</li>
<li>Fixed Water4 standard asset rendering on some devices.</li>
<li>Fixed audio playback when non-stereo mode selected (by forcing stereo).</li>
<li>Internet reachability check now returns proper value if switching in and out of airplane mode.</li>
<li>Project folder is no longer locked by adb after entering play mode in the editor.</li>
<li>Reporting correct screen orientation even if OS refused to apply requested orientation.</li>
</ul>

### Animation
<ul>
<li>Animation Clip is now available immediately after being created automatically for GUI</li>
<li>Fixed bug where Avatar mask wasn't appliedcorrectly to animation clip preview in the model importer.</li>
<li>Fixed bug where Blending pivot wasnot scaled correctly. It mainly affected AvatarPreview gizmo display. It did not affect runtime eval.</li>
<li>Builtin materials are now editable in animation mode. The animation is stored on the clip not the material.</li>
<li>Changing a child blend tree will now update objects using that blend tree in the scene.</li>
<li>Changing Animator.applyRootMotion while playing will no longer reset the controller's state machine.</li>
<li>Delayed the graph rebuild when deleting transitions to fix a bug when deleting multiple transitions.</li>
<li>Fixed bug where deleting a transition would delete a layer.</li>
<li>Fixed various crashes, especially on malformed data values.</li>
<li>Fixed UI issues: UI not updating after undo, curves flickering in some cases, rename overlays not shown, applying body mask in import settings, preview sometimes changing values, blend shape previews and so on.</li>
<li>Fixed adding child to new BlendTree not showing up in graph</li>
<li>Fixed animation events executed incorrectly on mirrored states.</li>
<li>Fixed Animation not playing in previewer for Generic</li>
<li>Fixed Animation transition causing undefined movement (even with "apply root motion" disabled)</li>
<li>Fixed Animator.Play that did not work after Recording</li>
<li>Fixed Animator.Play() and Animator.CrossFade() playing the animator state at requested time 't + deltaTime' when it should be 't'.</li>
<li>Fixed AnimationClip with manually-created root motion curves with wrong Class type causes crashes</li>
<li>Fixed Blend tree adjust time scale for animation clip without speed, you should get a warning when there is no speed available to compute the time scale</li>
<li>Fixed Blend tree compute threshold. if there is not enough data to compute the threshold you should get a warning.</li>
<li>Fixed BlendTree that had child AnimationClip with the same name.</li>
<li>Fixed bug where an Avatar mask used for humanoid clip import was not setup with all human transform checked.</li>
<li>Fixed Characters stretch out during a transition interrupted by another transition</li>
<li>Fixed computation of Homogenous Speed in BlendTree with clips that have no speed</li>
<li>Fixed dependency of sprites in AnimationClip, sprites are missing when the game object with sprite Animation is loaded from Assetbundle.</li>
<li>Fixed drag of AnimationClip on GameObjet that has an AnimatorController.   </li>
<li>Fixed evaluation of Curves with only one key.</li>
<li>Fixed Event evaluation when mirroring states.</li>
<li>Fixed feet pivot weight blending. Feet pivot weight was affected by blended clips even when their weights were very small</li>
<li>Fixed Humanoid going to relax pose on transition to state with no clip on 2nd sync layer</li>
<li>Fixed Humanoid rig playing animations differently than generic rig.</li>
<li>Fixed layer switching performance issue.</li>
<li>Fixed linear scale blending for additive layers.</li>
<li>Fixed multiple AnimationEvents at time 0 that were only firing the first AnimationEvent.</li>
<li>Fixed "Not Initialized" displayed on an Animator with valid Controller.</li>
<li>Fixed OnStateMachineEnter and OnStateMachineExit callbacks not being called.</li>
<li>Fixed packed NPOT sprite textures</li>
<li>Fixed Rect Transform z component not being animated</li>
<li>Fixed root motion still moving even if Root Transform Position(XZ) is baked.</li>
<li>Fixed several issues with Animation Events (event not fired, fired twice).</li>
<li>Fixed StateMachineEnter/Exit not being called on multi-layer component</li>
<li>Fixed transition error when a state had a speed of zero.</li>
<li>Fixed Transition previewer for very short clips.</li>
<li>Fixed UnloadNonDirtyStreams to correctly handle stream with destroyed objects.</li>
<li>Fixed unsynced AnimatorStateInfo and AnimatorClipInfo.</li>
<li>Generic Root Motion will be used for an additional Layer when no Mask is specified.</li>
<li>Prevented deletion of root blendTree in the BlendTree graph.</li>
<li>Prevented adding legacy animation to Mecanim.</li>
<li>Prevented creation of cycles in Blend Trees.</li>
<li>Propagated Animator invalidation on modification to AnimatorOverrideController to fix a crash when changing speed.</li>
<li>Rebakes euler angle curves on sample rate change.</li>
<li>Fixed Root Motion failing for very short clips.</li>
</ul>

### Asset Bundles
<ul>
<li>Asset Bundle Export performance increase.</li>
<li>AssetBundle.LoadAll***() now only return the game object without the first component.</li>
<li>Fixed crash if user passes "./" as output path when building AssetBundles.</li>
<li>Fixed possible crash while loading multiple AssetBundles simultaneously.</li>
<li>Fixed the typo in .manifest file</li>
<li>Remove duplicate objects when building with BuildAssetBundleExplicitAssetNames(). Also output more meaningful log information for assetBundle object.</li>
</ul>

### Asset Import
<ul>
<li>Added ability to retry operation on write error when importing assets.</li>
<li>Added warning messages when paths to assets are invalid</li>
<li>Append required .fontsettings extension if needed in GenerateEditableFont</li>
<li>Check texture format that can be assigned the TextureImporter</li>
<li>Fixed AssetDatabase.ImportPackage fail when path to package has platform path separators.</li>
<li>Fixed crash when included blend shapes and needed to be split because of size.</li>
<li>Fixed crash when upgrading metadata files</li>
<li>Fixed import of empty .txt files.</li>
<li>Fixed import of Maya files with set driven keys.</li>
<li>Fixed problem when importing models with no diffuse color specified.</li>
<li>Fixed problems with animation importing incorrectly due to mirror/negative scale.</li>
<li>Support the manifest file in text importer.</li>
</ul>

### Asset Management
<ul>
<li>Added warning when using AssetDatabase.Load* function with an absolute path</li>
<li>Fix assets unload during load level operation</li>
<li>Fixed crash while loading scene Unity with mecanim animation and skinnedmesh filter.</li>
<li>Fixed invalid cache state after cancelling WWW download.</li>
<li>Fix the "input objects must be of exact same type" error message</li>
<li>Prefabs: Fix crash if using DestroyImmediate() on prefab instance objects during prefab instantiation.</li>
<li>Prefabs: Fix crash when accessing physics component properties during OnValidate(). This includes a general change in behavior for OnValidate() calls during prefab instantiation and undos such that it follows the same order as when loading from disk.</li>
<li>Prefabs including monobehaviours with missing scripts should not display a warning if the monobehaviour has been deleted on the prefab instance.</li>
<li>Resources.Load will now correctly return NULL when there is no Object of the desired type with that name (instead of returning an object with a different type if it exists)         </li>
<li>Serialization: Added ability to do automatic fix of invalid references to scripts in scene file (to valid registered scripts)</li>
<li>Serialization: Added error message with file information if SerializedFile header is corrupted</li>
<li>Serialization: Fixed bug that caused build corruption when serializing volatile fields.</li>
<li>Serialization: Fixed bug that caused build corruption when serializing classes for which a generic version exists</li>
<li>Serialization: Fixed the error message when removing an object in a custom inspector</li>
<li>Serialization: Fixed windows Layout loading if script for previously opened custom window is absent</li>
</ul>

### Audio
<ul>
<li>AudioClip.SetData no longer prints out error messages when writing data at a position that will cause wrapping.</li>
<li>Calling AudioClip.SetData causes a crash fixed</li>
<li>Fixed a bug where the audio system stopped working when a game object had an AudioSource, an AudioListener and a custom audio filter attached. The system now outputs a warning as the custom audio filter can only be assigned to one Audio component at a time.</li>
<li>Fixed Crash when exposing a parameter of an effect that was added to a group</li>
<li>Fixed for regression where component effects are on the AudioListener cause a crash</li>
<li>Fix importing Tracker files so that by default, they are set to load Compressed In Memory. This is also now configurable.</li>
<li>Fixed leaking audio resources when having AudioSources within a Prefab</li>
<li>Prevent data-race condition in AudioManager</li>
<li>Prologic DTS can now be selected as an audio output.</li>
<li>Remove exposed parameters correctly when deleting and effect that has exposed parameters in it.</li>
<li>Stability fix for custom audio filters placed on the AudioListener.</li>
<li>When audio clip was set to Load In Background project crashed on Android immediately</li>
</ul>

### Blackberry
<ul>
<li>Event.shift and Event.alt now work as expected.</li>
</ul>

### Build Pipeline
<ul>
<li>Don't include inactive EditorOnly objects in builds.</li>
</ul>

### Cache Server
<ul>
<li>Fix "CacheServer Asset validation failed" error messages while Unity is importing project.</li>
<li>Fix editor crash when enabling the Cache Server in preferences with empty address.</li>
</ul>

### Core
<ul>
<li>Fix crash when initializing Light from prefab object during scene loading.</li>
<li>Fix the bug that loading from cache returns false.</li>
<li>Fixed data race in memory allocators.</li>
<li>Runtime: Error message is now shown if you try to add a component of invalid type</li>
<li>Runtime: Fix Time.realtimeSinceStartup being wrong during Awake calls in initial level load.</li>
<li>Runtime: GameObject.FindObject nolonger stops and returns null if first match is an inactive game object.</li>
</ul>

### Debugging
<ul>
<li>Allow evaluation of methods with string literal parameters.</li>
<li>Don't interrupt user waits (e.g. ManualResetEvent).</li>
<li>Fix setting breakpoints in generic method implementations.</li>
<li>Fix some instances of debugger freezing or hanging.</li>
</ul>

### Editor
<ul>
<li>Added "-force-gl-ref" cmd-line option support for the OSX Editor.</li>
<li>Added link to editor settings when sprite packer is disabled</li>
<li>Animation Window refreshed when tabbed into</li>
<li>AnimationState.time is updated when scrubbing animation in the AnimationWindow.</li>
<li>Audio preview is refreshed after import settings are changed</li>
<li>CanvasGroup methods were not getting registered in the UI module, resulting in MissingMethodExceptions</li>
<li>Changing framerate in animation window now repositions animation events correctly</li>
<li>Cloth inspector to support multi-editing</li>
<li>Color picker code now has correct color space conversion and is now working accurately.  </li>
<li>Confined cursor mode doesn't confine cursor to last active editor pane</li>
<li>Create a new project upgrade warning system that does not depend on serialized files or version control.</li>
<li>Deleting an asset does not make deleted objects from other assets appear again.</li>
<li>Disallow empty names for sprites</li>
<li>Don't ignore assets whose names contain "StreamingAssets"</li>
<li>Don't immediately hide popup windows when there are unity windows on secondary screen on OSX</li>
<li>Don't let user rename GameObjects with HideFlags.NotEditable set</li>
<li>Drag-and-drop does not accept simple Renderers as a valid target for assigning skybox material.</li>
<li>Editor no longer freezes when scene view camera is really far from origin</li>
<li>Empty animation window no longer increases CPU usage</li>
<li>Ensure correct waking order of components when duplicating a GameObject.</li>
<li>Ensure screen width and height in player settings is at least 1</li>
<li>Expose static methods from context objects to JS.</li>
<li>Fixed an occasional crash when reimporting shaders.</li>
<li>Fixed assetBundle search filter doesn't work correctly.</li>
<li>Fixed assert when loading scene containing reference to one of its objects that no longer exist.</li>
<li>Fixed asserts when displaying multiple objects in inspector preview.</li>
<li>Fix asset when using hideFlags to make objects persist after exiting play mode.</li>
<li>Fixed audio source priority slider showing "–" when editing multiple objects</li>
<li>Fixed AudioSourceInspector.cs throwing null refs on UndoRedoPerformed</li>
<li>Fixed broken inspector setup with multiple inspectors when shaders are using custom editors</li>
<li>Fixed changing loaded level index before OnApplicationQuit message when exiting play mode.</li>
<li>Fixed clipping of multi-line text in text fields.</li>
<li>Fixed confirmation dialog "Losing Prefabs" shown twice when trying to delete child object</li>
<li>Fixed console errors when inspecting player settings in debug view.</li>
<li>Fixed crash occasionally happens when you create a prefab. Related to the object sorting in the prefab.</li>
<li>Fixed crash when executing a menu item from a static constructor.</li>
<li>Fixed crash when maximizing game view on OSX.</li>
<li>Fixed crash when removing components from a prefab, but prefab instances would have depending components.</li>
<li>Fixed crash when script name is longer than 32 characters.</li>
<li>Fixed crash with corrupted scene when having invalid references in the list of transform children.</li>
<li>Fixed custom cursors to properly update in OS X editor.</li>
<li>Fixed custom PropertyDrawer being called with wrong SerializedProperty when property is inside a nested class.</li>
<li>Fixed double firing of playmodeStateChanged</li>
<li>Fixed Edge Collider 2D sometimes not showing handles</li>
<li>Fixed editor errors when undoing the insertion of a new LOD level in LOD group.</li>
<li>Fixed error spam: "GUI Error: You are pushing more GUIClips than you are popping .." when setting cam.targetTexture = null in OnPostRender.</li>
<li>Fixed exceptions happening when a read-only plugin is used.   </li>
<li>Fixed font corruption after asset import.</li>
<li>Fixed freeze during Editor startup when using input devices with large number of emulated buttons (some wireless mouses)Fixed GameObject not selectable by label icon</li>
<li>Fixed freeze on floating-point exception</li>
<li>Fixed Import Package window being broken due to illegal characters in path</li>
<li>Fixed incorrect fade group animation in player settings</li>
<li>Fixed inspector rendering when a script changes RenderTexture.active.</li>
<li>Fixed isPlayingOrWillChangePlaymode to work as expected.</li>
<li>Fixed keyboard shortcuts (home/end/page up/page down) in object selector</li>
<li>Fixed Mac Editor Projects with hidden folders inside Assets are usable again</li>
<li>Fixed many texture/mesh related error messages to ping the source object that caused it.</li>
<li>Fixed material inspector could collapse its controls by clicking on the header. Controls are now always visible.</li>
<li>Fixed memory leak when calling 'Object.Destroy' and returning to edit mode.</li>
<li>Fixed meshes getting lost if they only lived in the scene and only were referenced by a mesh collider.</li>
<li>Fixed missing header for state machine behaviours</li>
<li>Fixed navigation keyboard shortcuts in object selector</li>
<li>Fixed NullReferenceException from uninitialized icon if CurveEditor is shown before Inspector</li>
<li>Fixed NullReferenceException when Tools.viewTool is queried outside OnGUI</li>
<li>Fixed numeric accuracy of transform coordinates when copy/pasting or duplicating objects.</li>
<li>Fixed occasional crash/hang on exit.</li>
<li>Fixed page down in object selector on Windows</li>
<li>Fixed position of GUI elements in inspector when using PropertyDrawers.</li>
<li>Fixed possible corruption of editor window rendering in OS X Editor.</li>
<li>Fixed possible crash when placing prefabs with child objects.</li>
<li>Fixed projectsettings.asset serialization error</li>
<li>Fixed property list in Animation Controller editor allowing to drag invalid element from bottom of list.</li>
<li>Fixed race condition in memory allocation system.</li>
<li>Fixed rename overlay is not removed when undoing</li>
<li>Fixed Skybox components not taken into account in camera preview popup</li>
<li>Fixed so TextMesh text field uses TextArea instead of single text field</li>
<li>Fixed Sprite Editor crash when docked to top of the layout</li>
<li>Fixed stack traces not being generated correctly.</li>
<li>Fixed text corruption in TextMesh components when reimporting fonts.</li>
<li>Fixed that text fields in an unfocused window could break another windows textfield if busy repainting</li>
<li>Fixed tooltips not always showing up when they should.</li>
<li>Fixed typing into the search field between transition animations for Add Component menu</li>
<li>Fixed unparenting when deleting object in Editor once OnDestroy is called</li>
<li>Fixed updating color fields in material inspector to work when warnings are displayed.</li>
<li>Fixed user cannot close a custom editor window from a previous project.</li>
<li>Fixed utility windows always loading last width &amp; height if larger than requested width &amp; height.</li>
<li>Fixed when mouse was not processed in the Editor in play mode after building Android or iOS.</li>
<li>Fixed Windows Editor not showing progress over taskbar icon, when doing initial project import.</li>
<li>Fixed Windows Editor unresponsive to user's input in some tablets.</li>
<li>Folders named "something.unity" will be listed as folders and not scenes in a search</li>
<li>FPS controls now only affects the active scene view</li>
<li>I18n: Issues with Asian Input Method Editors inside the Windows version of the Editor.</li>
<li>I18n: Issues importing assets when their path/asset/component names contain Asian characters.</li>
<li>I18n: Issues storing/retrieving strings from PlayerPrefs when PC is set to Asian locale.</li>
<li>I18n: Editor crashes on start-up if computer / user / project name contains Asian characters.</li>
<li>IMGUI: Fixed crash when using GUI.Window recursively.</li>
<li>IMGUI: Fixed line spacing when multiple sizes are used in text markup</li>
<li>IMGUI: Fixed renaming of existing controls using GUI.SetNextControlName.</li>
<li>IMGUI: ContextClick events are now never received by in-game GUIs (as documented, the event is editor only).</li>
<li>Initialize Scene View 2D mode correctly when upgrading from version</li>
<li>Input.mousePosition now returns correct position when called in Awake and Start in the editor</li>
<li>Make key combinations ignore Caps Lock key.</li>
<li>No more errors after applying new preset in the curve editor</li>
<li>Object Picker is now able to show a hierarchy of sub assets (used for AudioMixerGroups for now).</li>
<li>Opened scene will no longer be accidentally marked as modified.</li>
<li>Opening multiple locked inspectors works</li>
<li>OSX corner resize gizmo doesn't block input when not shown.</li>
<li>Packages: Fix importing package with long paths on Windows</li>
<li>Particles: Fixed particles that are out of view casting incorrect shadows.</li>
<li>Particles: Fixed systems using Distance emission not stopping correctly.</li>
<li>Particles: ParticleSystem will no correctly remove any of its particles and reset its emitter state when being deactivated.</li>
<li>Prevent each script from opening in a new Visual Studio instance.</li>
<li>Prevent MinMaxSlider getting into error state when clicking in the thumb area</li>
<li>Prevent right clicking on controls behind preview window</li>
<li>Reduce serialization depth limit warnings</li>
<li>Remove unsupported OSX menu items (Start Dictation &amp; Special Characters)</li>
<li>Removing curve in animation window doesn't remove other curves with similar name</li>
<li>Reverting a prefab no longer fails if two added components depends on each other.</li>
<li>Select Dependencies operation no longer breaks editor fonts</li>
<li>Shadows working correctly when zoomed in animation preview window</li>
<li>Show at most one error when attempting to deleting multiple components</li>
<li>Sprite name was emptied when copy pasting position etc. values on editor</li>
<li>Swatches in the Color Picker tool are now gamma corrected when using linear colour space.</li>
<li>Synchronize EditorUserBuildSettings.selectedStandaloneTarget when switching build targets with SwitchActiveBuildTarget() or -buildTarget.</li>
<li>Tooltips use current skin instead always using light skin</li>
<li>Warn in Lighting window UI when a skybox with nonsensical shader is used</li>
<li>Will exit play mode when switching build platform.</li>
<li>Unity crashes while adding component to destroyed object.</li>
<li>Undoing changes in the Animator throws an error.</li>
<li>Use unique sprite name when creating new sprites manually</li>
</ul>

### Fonts
<ul>
<li>Fixed a bug where regenerating font textures might miss needed characters from the last frame. </li>
<li>Fixed fallback to default font for characters missing in customs fonts on platforms without OS font access.</li>
</ul>

### Graphics
<ul>
<li>Camera.RenderToCubemap will correctly work with AA render texture.</li>
<li>D3D11: Fixed an issue which caused some objects not be rendered if shadows are enabled in the scene on feature level 9.x</li>
<li>Deferred Lighting is disabled for oblique camera projections; falls back to forward rendering now. Before, it was just not working properly, without a proper fallback.</li>
<li>DX11, fixed GL.Clear when we have MRTs (only first target was cleared before).</li>
<li>Fixed HDR support for SunShafts image effect.</li>
<li>Fixed incorrect warning about NPOT texture filtering</li>
<li>Fixed occasional crash on creating and immediately deleting particle renderer.</li>
<li>Fixed RenderTextureFormat.Default and DefaultHDR only working with RenderTexture.GetTemporary(), not with permanent RenderTextures.</li>
<li>Fixed shadow caster culling for orthographic cameras.</li>
<li>Fixed Skybox not rendering with some edge cases of supported vs. not supported shaders</li>
<li>Fixed Texture2D.EncodeToPNG being very slow for large images. E.g. for 4096x4096 image, it's now almost 10x faster!</li>
<li>Fixed "Tiled GPU perf. warning" in editor resulting in poor performance.</li>
<li>Fixed warning thrown on saving scene by mark the meshes as DontSave</li>
<li>GI: Fixed tetrahedralization issues with small floating point differences in probe positions.</li>
<li>GLES: Fixed rendering bug that occurs when native rendering plugin calls glViewport</li>
<li>Image Effects: Fixed some ImageEffectOpaque effects making later alpha blended geometry not render with correct Z-buffer.</li>
<li>Make sure to never use soft particles when in orthographic camera, since depth-based fadeout does not work there.</li>
<li>OpenGL: Detected cases on Windows when no OpenGL drivers are installed and exit properly.</li>
<li>OpenGL: Don't force texture/shader reload when changing resolution (breaks baked lighting, etc.)</li>
<li>OpenGL: Fixed GLSL fragment shader incorrectly tagged as a Fixed Function pipeline shader.</li>
<li>OpenGL: Fixed RenderTextures on Windows 64-bit standalone using OpenGL.</li>
<li>OpenGL ES: Enforce RGB normal maps even if source texture have alpha.</li>
<li>OpenGL ES: Some performance improvements by removing redundant GL API calls.</li>
<li>Rendering: Fix crash when closing Standalone player in DX11 render mode.</li>
<li>Rendering: Fix memory leak when dynamic geometry chunk did not add any vertices.</li>
<li>Rendering: Fixed crash when reading font's metadata for a font without style info.</li>
<li>Shadows: Fixed flickering/inconsistent shadows when light culling masks cause more than one light to be "main light" in forward rendering.</li>
<li>Shadows: Fixed shadowmaps being re-rendered when using deferred shading with some forward-shaded objects.</li>
<li>Shadows: Fixed some cases where alpha-tested shadow caster objects were wrongly batched together, even if they used different textures.</li>
<li>Shadows: Fixed spot light shadow bias to be more sensible. Was highly non-linear before.</li>
<li>Tint calculation in Skybox shaders is done more properly when in Linear color space now.</li>
</ul>

### iOS
<ul>
<li>Check whether an ad is loaded in ADInterstitialAd.Show()</li>
<li>Correctly implement Marshal.Copy for arrays.</li>
<li>Delete newlines when pasting into single line edit boxes</li>
<li>Disable informational warnings on non-development build</li>
<li>Don't pass touches through iOS keyboard's toolbar</li>
<li>Don't spam the console log with GameKit stuff on release builds</li>
<li>Fixed GetLoadedDylibs to not to include the app exe in the results</li>
<li>Fixed Info.plist append</li>
<li>Fixed launch screen support</li>
<li>Fixed memory leaks related to UTF8String.</li>
<li>Fixed project append</li>
<li>Fixed random crash when changing orientation by 180 degrees</li>
<li>Fixed severe visual issues when setting Screen.orientation when autorotation is disabled</li>
<li>Fixed special character treatment in Info.plist</li>
<li>Fixed splashscreens for landscape orientation on iOS 7 and newer</li>
<li>Fixed visual issue in Player settings</li>
<li>Fixed wrong frame buffer size on iPhone 6+</li>
<li>Ignore SIGPIPE signal which is thrown by broken sockets</li>
<li>Improved iOS device name detection.</li>
<li>Made advertisement ID calls dynamic to avoid App Store rejections.</li>
<li>Report size of assemblies after bytecode stripping</li>
<li>Support multiple permission types in {Request,Has}UserAuthorization</li>
<li>Use new remote notification API on iOS 8</li>
<li>Use separate font metadata caches for each iOS version</li>
<li>Workaround for iOS 8.0 GameController API crash bug</li>
</ul>

### IL2CPP
<ul>
<li>Correctly handle the Duv_Un IL opcode with signed arguments to prevent an error from IL2CPP like this: "Unexpected types used with Div_Un opcode. Types are Int32 and Int32" </li>
<li>Correctly throw a managed exception when an array is created with a negative size.</li>
<li>Handle custom attributes on events correctly.</li>
<li>UnityEngine.dll methods that are targets of UI events are no longer incorrectly stripped</li>
<li>Write proper include directives for all fields of marshaled structures or classes.</li>
</ul>

### Installers
<ul>
<li>Windows: No longer specifying the "Editor" subfolder of path when installing Unity.</li>
<li>Windows: Uninstall MonoDevelop when uninstalling Unity.</li>
</ul>

### Linux
<ul>
<li>Call OnApplicationQuit callbacks for all methods of quitting the player.</li>
<li>Constrain size of screen selector banner image.</li>
<li>Filter aspect ratios in screen selector.</li>
<li>Fix hotspot desynchronization with custom cursors when hiding/reshowing.</li>
<li>Fixed spotlight shadow filtering on Linux - now uses hardware PCF just like Win/Mac.</li>
<li>Improve system language detection.</li>
</ul>

### MonoDevelop
<ul>
<li>Fixed exception when resolving symbolic breakpoints.</li>
<li>Fixed issue with Cmd+A (Select All) keyboard shortcut not working correctly on OSX after using the main menu.</li>
<li>Fixed “jumping cursor” issue.</li>
<li>Fixed opening the same file twice in MonoDevelop.</li>
<li>Updated versions of Mono/GTK used, fixing scrolling issues with some mice.</li>
</ul>

### Networking
<ul>
<li>WWW on local file system can accept non-ASCII filenames on Windows.</li>
</ul>

### OS X
<ul>
<li>Mac OS X Standalone: Fix crash changing if resolution in batch mode.</li>
<li>Mac OS X Standalone: IME Input now works in the 64-bit Standalone player.</li>
</ul>

### Physics
<ul>
<li>Cloth: fixed cloth exploding for any non-trivial model imported from FBX.          </li>
<li>Cloth: fixed rotation being applied twice         </li>
<li>Cloth: improved simulation quality, fixed a bug where cloth simulation would be dramatically affected by fps            </li>
<li>Collider.Raycast will now not hit disabled colliders</li>
<li>ConstantForce2D torque should be in degrees not radians.</li>
<li>Prevented negative values being set for CharacterController.stepOffset.</li>
<li>Enabled flag on CharacterController now correctly keeps its state.</li>
<li>Fixed cloth vertices renderer (was rendering vertices rotated in editor mode)</li>
<li>Fixed crash when applying force to inactive Rigidbody</li>
<li>Fixed crash when doing a Raycast() on a collider that failed initialization</li>
<li>Fixed explosion force when position is inside collider's world AABB.</li>
<li>Fixed HingeJoint spring's targetPosition range that was incorrect.</li>
<li>Fixed Physics.IgnoreCollision</li>
<li>Fixed regression where property changes in the editor did not update the 2D collider in the scene view.</li>
<li>Fixed rotation mode combo for ConfigurableJoint.</li>
<li>Fixed terrain colliders returning sharedMaterial == null</li>
<li>Fixed that TransformChanged events could re-create the Cloth component, even though the component was already cleaned up.</li>
<li>Implement Undo for Cloth editor.</li>
<li>Make sure explicit inertia tensor is not reset when modifying colliders</li>
<li>Send OnControllerColliderHit on collisions with another CharacterController reliably.</li>
<li>Set default physic material properties to match values in PhysX SDK</li>
<li>Support sending OnTriggerExit when collider is deactivated or destroyed</li>
<li>WheelCollider: fixed a bug where attachedRigidbody would be equal to null         </li>
<li>WheelCollider: fixed a bug where editor would crash soon if you use sliders to tune WheelCollider properties.</li>
<li>WheelCollider: fixed wrong behaviour after changing mass of parent rigidbody</li>
</ul>

### Scripting
<ul>
<li>Ensure all children receive broadcast messages even if the transform hierarchy changes during a callback from the message.</li>
<li>Fixed adding EllipsoidParticleEmitter / MeshParticleEmitter components</li>
<li>Fixed crash if a MonoBehaviour was created in MonoBehaviour OnDisable.</li>
<li>Fixed crash in callback</li>
<li>Fixed crash when calling DestroyImmediate in MonoBehaviour constructor</li>
<li>Fixed crash when calling user log callback from a non-main thread</li>
<li>Fixed exceptions being thrown when calling Object.FindObjectsOfType().</li>
<li>Fixed ExclusiveAddressUse socket flag on windows </li>
<li>Fixed for some debugger freezes / crashes while debugging on OS X and Windows.</li>
<li>Fixed internal compiler error when script defines are duplicated</li>
<li>Fixed process querying on OSX</li>
<li>Fixed some cases when using a class name that collides with an internal class name in a different namespace (e.g. BuildSettings)</li>
<li>Fixed StackOverflowException handling on 64-bit Windows</li>
<li>Fixed webplayer not auto-starting as requested when calling BuildPlayer with Windows-style paths.</li>
<li>Invoking DllImport from various threads, should be thread-safe now.</li>
</ul>

### Shaders
<ul>
<li>Better error message when a shader is using properties that clash with built-in Unity global properties.</li>
<li>Fixed _CameraToWorld and _WorldToCamera matrices being wrong while rendering into a cubemap, or when custom camera.worldToCameraMatrix is set.</li>
<li>Fixed DirectX 11 shader compilation when Unity is installed in a path with non-ascii characters.</li>
<li>Fixed hlsl-to-glsl translation problem with expressions that initialize a matrix with a scalar (float3x3 m = 0).</li>
<li>Fixed issue with generated projects (.csproj) sometimes not having a reference to UnityEngine.UI.dll</li>
<li>Fixed legacy Diffuse Detail shader when in linear color space.</li>
<li>Fixed loading of some GLSLPROGRAM shaders with preprocessor macros on OpenGL ES</li>
<li>Fixed "Maximum number of shader keywords" error in editor resulting in really bad build-time performance.</li>
<li>Fixed some cases where surface shader compiler was producing error about "too many texture interpolators" with no further details. </li>
<li>Fixed surface shader compilation bug where keywords like "nolightmap novertexlights" were not properly excluding all needed variants.</li>
<li>Fixed surface shader compilation bug with some combinations of #pragma multi_compile / shader_feature.</li>
<li>Fixed unnecessary truncation of float constants on GLSL platforms.</li>
</ul>

### Substance
<ul>
<li>Emissive outputs assigned to _EmissionMap shader slots now correctly trigger the emissive effect when the material is loaded.</li>
<li>Fix case where the editor-side Substance cache data would not be reused when it should.</li>
<li>Fix crash in standalone builds when loading a SBSAR with both BakeAndDiscard instances and non-baked instances.</li>
<li>Fix crash when inspecting baked ProceduralTextures.</li>
<li>Fix texture corruption issue in standalone builds where modifying an input value and calling RebuildTextures() on a ProceduralMaterial with image inputs and whose outputs have been read from cache would result in black textures being generated.</li>
<li>Grayscale image inputs are now supported.</li>
<li>ProceduralMaterials only referred to by their outputs and not by their attached material now load properly.</li>
</ul>

### Terrain
<ul>
<li>Custom material's shader keywords now will be correctly applied.</li>
<li>Doing vertex snapping for terrain objects no longer crashes the editor.</li>
<li>Fixed assertion when loading a scene with TerrainData objects embedded.  </li>
<li>Fixed broken tree colliders.</li>
<li>Fixed corrupted rendering when being edited.</li>
<li>Fixed crash when importing detail meshes with float color channel.</li>
<li>Fixed "m_UniqueThreadAllocator-&gt;GetAllocatedMemorySize() == 0" error after "Mass Place Trees".</li>
<li>Fixed some memory leaks.</li>
<li>Tree imposters lighting is now matched with lighting on mesh trees.</li>
</ul>

### Version Control
<ul>
<li>Add missing icon for incoming changesets.</li>
<li>Auto connect when connection is dropped.</li>
<li>Correct local/remote args for diff tool.</li>
<li>Do not print a warning when saving scene and file is not opened for edit unless necessary.</li>
<li>Fixed case handling on Windows when downloading files.</li>
<li>Fixed editor crash on loading terrain with corrupted detail layers.</li>
<li>Make it possible to retry a hanging connect while connecting.</li>
</ul>

### Web Player
<ul>
<li>Correctly verify generic reference type constraint for generic parameter with type constraint which is a reference type.</li>
</ul>

### Windows Player
<ul>
<li>Deployment Management: Simpler "Force Single Instance" error message on Windows</li>
<li>Deployment Management: Fix StandalonePlayer launched from UNC path</li>
<li>DirectX 11: Mip mapped cubemaps now work correctly on feature level 9.x. This fixes the smoothness setting in the standard shader.</li>
<li>DirectX 11: Unity will now correctly detect if hardware doesn't support a particular cubemap size, and will try to skip higher mip maps instead of failing to upload the cubemap at all.</li>
<li>Fixed fullscreen player sometimes disappearing behind other windows on startup.</li>
<li>Return the correct value from PlayerPrefs::SetString</li>
<li>Windows 10 reports SystemInfo.operatingSystem string properly.</li>
</ul>

### Windows Phone
<ul>
<li>Windows Phone 8.1: Enabling location capability no longer causes a crash.</li>
<li>Windows Phone 8: Tap count is now correctly calculated when using multiple fingers.</li>
<li>Windows Phone/Windows Store Apps: Generic list of structs is now properly serialized.</li>
<li>Windows Store Apps/Windows Phone: added support for animating script variables that are members of structs.</li>
<li>Windows Store Apps/Windows Phone: fixed sprite animation on GUI elements</li>
<li>Windows Phone 8.1: Enabling "Human Interface Device" capability in player settings no longer makes Unity generate invalid application certificate.</li>
<li>Windows Phone 8.1: Fixed Handheld.Vibrate().</li>
<li>Windows Phone: Fixed Handheld.PlayFullscreenMovie().</li>
<li>Windows Phone 8.0: Fixed GUI text rotation when device is in landscape orientation and rendering to a render texture.</li>
<li>Windows Phone 8.0: Fixed image effects when device is in landscape orientation.</li>
<li>Windows Phone 8.0: Trying to access webcam without appropriate capabilities in application manifest will no longer constantly throw exceptions.</li>
<li>Windows Phone 8.0: Fixed Unity generating invalid references in Visual Studio project, debug configuration.</li>
<li>Windows Phone: Texture2D.ReadPixels now works correctly in landscape modes.</li>
<li>Windows Phone: fix crash on application exit when location is enabled</li>
<li>Windows Store/Phone: Cloth.coefficients now work correctly</li>
<li>Windows Store Apps/Windows Phone: You can now render to cubemaps on DX11 9.x feature levels.</li>
<li>Windows Store/Phone: Depth render textures are not really supported on DX11 9.x feature levels, but previously they were wrongly claimed to be supported.</li>
<li>Windows Phone/Windows Store Apps: Gyroscope.gravity returns same values as other platforms. It used to be inverted before.</li>
<li>Windows Phone 8: Camera.ViewportToWorldPoint returns correct value in orthographic view.</li>
<li>Windows Store Apps/Windows Phone: fix taking detailed memory sample in profiler</li>
<li>Windows Phone 8: setting keyboard text just after creating it will not be in vain anymore.</li>
<li>Windows Store Apps / WIndows Phone 8: Matrix4x4 will be correctly serialized   </li>
<li>Windows Store Apps/Windows Phone: fix profiler not working after reopening the editor</li>
<li>Windows Store Apps/Windows Phone: better error messages when AssemblyConverter fails to resolve type.</li>
<li>Windows Store Apps/Windows Phone: fix AssemblyConverter failing on struct from unprocessed or system assemblies</li>
</ul>

### Windows Store Apps
<ul>
<li>Added missing defines UNITY_WSA, UNITY_WSA_8_0/UNITY_WSA_8_1 in generated Assembly-CSharp-* projects.</li>
<li>Fixed building Universal apps in batch mode</li>
<li>Fixed crash when WebcamTexture is destroyed</li>
<li>Fixed errors in the editor when player settings are open and upgrading scripts or switching platform</li>
<li>Fixed high CPU when Unity is paused</li>
<li>Fixed issue when App bar couldn't be open with mouse right-click while Independent Input source is enabled.</li>
<li>Fixed mouse callbacks</li>
<li>Fixed native plugin not included in generated Visual Studio solution</li>
<li>Fixed serialization error when serializing object derived from System.Object and Compilation Overrides are set to .NET Core.</li>
<li>Fixed SerializationWeaver failure when scripts reference classes in plugins</li>
<li>Fixed UnityScript breaking exported solution with SDK 8.0</li>
<li>Native plugins now properly added to generated solution</li>
<li>Unity now regenerate test certificate, if it was deleted, rather than failing to build project.</li>
<li>runInBackground checkbox will now warn about wack failure that it might cause.</li>
<li>UNITY_WINRT_8_1 and UNITY_WINRT_8_0 will be correctly defined now.</li>
<li>Unity will now store certificate path as a relative path, so when project is moved to another PC, it will be still found.</li>
<li>When building player files are now copied directly to destination directory bypassing staging area, reduces project size when submitting a bug</li>
<li>You can now use HashAlgorithm &amp; MD5CryptoServiceProviders classes in C# files compiled against .NET Core.</li>
</ul>
