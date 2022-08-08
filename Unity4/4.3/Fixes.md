# Unity 4.3

https://unity3d.com/unity/whats-new/unity-4.3

## Fixes



*   AI / NavMesh: NavMesh.Raycast: Gives correct navmesh height (Y component) for hit position.
*   AI / NavMesh: Fix issue where disabling one navmesh obstacle would sometimes affect another obstacle.
*   AI / NavMesh: Fix NavMeshAgent occasionally getting NaN positions in cases where many agents are spawned/destroyed and avoidance is disabled/enabled.
*   AI / NavMesh: Fix NavMesh.CalculatePath returning path with wrong path endpoint when path is partial.
*   Android: Fixed a problem where "Unable to find suitable jdk installation" was presented even with a valid jdk in path
*   Android: Disabled glTexSubImage2D for adreno devices - fixes some of the dynamic font issues
*   Android: Fixed default orientation for 3rd gen kindle devices
*   Android: Fixed stripping issue which caused AndroidJavaRunnable to fail
*   Android: Fixed ToString error when unboxing java string for AndroidJavaProxy.
*   Android: Workaround for an issue with the android compositor on external displays.
*   Animation: Fixed leak in animator component
*   Animation: Will handle Enable binding correctly.
*   Animation Window: Update() isn't offered as an option in the add event popup anymore.
*   Animation Window: Add Curve dialog no longer pops up again after cancelling it
*   Animation Window: Adding new clips into read-only objects no longer allowed
*   Animation Window: Animation Event tooltip wasn't showed on mouse hover.
*   Animation Window: Animation Event window wasn't updated when selection was changed
*   Animation Window: Changing IsActive property keyframe via animation window is updated into scene view immediately
*   Animation Window: Curves-toggle is persistent if you close/reopen animation window
*   Animation Window: Dopesheet clamp framerate between 0-10 000 to avoid data loss for big number
*   Animation Window: Dopesheet is now able to show more than 50 sprite previews at the same time
*   Animation Window: Fixed Scale transform is marked yellow in the Inspector although it not animated
*   Animation Window: In record mode you should be able to animate an Animator Generic rig.
*   Animation Window: No error messages after removing the animated object
*   Animation Window: While moving selected keyframes, sometimes other keyframes would move also
*   Audio: Fix AudioListener.volume for AudioSource.PlayOneShot
*   Audio: Fix AudioImporterInspector: Compression slider shows wrong max
*   Audio: Fix Custom audio filter for AudioListener does not affect sounds played by PlayOneShot
*   Audio: Fixed StackOverflow in OSX Editor during AudioClip.Create
*   BlackBerry: Fixed issue where gravity was being reported in meters per second instead of G forces. Also landscape x and y for gravity was swapped.
*   BlackBerry: WebCamTexture.videoVerticallyMirrored is now set correctly.
*   BlackBerry: Fixed issue where tiling would occur when webcam framerate was set outside acceptable range.
*   BlackBerry: MailTo URI's now work as expected.
*   BlackBerry: Remapped gamepad buttons to match up to Xbox 360 controller.
*   Bug Reporter: Fix crash when submitting documentation bugs from OS X.
*   BuildPipeline: Custom cursor specified in PlayerSettings is now built and shown correctly.
*   Cursors: Fix regression with cursor not showing in OS X standalone build.
*   Documentation: Fixed documentation of EditorUtility.CollectDeepHierarchy.
*   Documentation: Readded the message "Inherits from" for classes that have a parent.
*   Documentation: Return types, parameter types and types in examples work as links.
*   DX11: Fix 100% cpu use on Win81, reduce it somewhat on older windows.
*   DX11: Handle "-adapter X" command line argument.
*   Editor: Fixed "set default parameters" button in occlusion-bake tab
*   Editor: Fixed crash while baking occlusion culling data
*   Editor: Workaround windows 8.1 + webkit regression causing crash on mouse wheel messages.
*   Editor: Fix external editor not opening files when double clicking errors in console and external editor arguments have been specified.
*   Editor: Fixed crash when Transform was referenced multiple times by parent Transform (only happens in corrupt scenes; editor will automatically remove extraneous references now).
*   Editor: Fixed ScriptableObject editor script reference field being incorrectly drawn with PropertyDrawer.
*   Editor: Fixed that EditorGUI.LabelField got key focus when tabbing (its now skipped when tabbing)
*   Editor: Fixed that mouse cursor over gradient alpha input field was showing as drag area instead of text area
*   Editor: Fixed that tabbing through controls jumps back to "active" checkbox for the game object instead of moving to the next gui control
*   Editor: Fixed that the static toggle in inspector does not update correctly when toggled, if the current value is "mixed"
*   Editor: Disabled GPU Profiler on Macs + NVIDIA GeForce 650M, turns out the drivers return garbage data.
*   Editor: Do not disable the lighting flag in the scene view after completing a build
*   Editor: Don't leak references to assemblies that are dynamically loaded from game code.
*   Editor: Fix input sometimes being sent to windows that have already been destroyed causing PPtr dereference asserts.
*   Editor: Fix static preview generation to have the right background color in linear mode
*   Editor: Fixed import of Reflection textures sometimes freezing the Editor when Fixup Edge Seams is checked.
*   Editor: Fixed unclear and flickering DX11 tool tip message in Player Settings on Mac.
*   Editor: It's now possible to undo changing batching settings in the PlayerSettings
*   Editor: Mark BeginGUI(Rect) as obsolete, as it leads to bad internal GUI state
*   Editor: Fix Object Picker causing nullrefs when shown outside of OnGUI.
*   Editor: Opening PopUp menus with the keyboard on windows will no longer beep.
*   Editor: Closing a editor tab shouldn't change the selected tab.
*   Editor: Fix that Preferences key shortcuts using toggle with CTRL didn't work on Windows.
*   Editor: Fixed searching for Terrain in the Hierarchy or Project window (use t:terrain)
*   Editor: Fixed searching for GUISkin in Project Browser (use t:guiskin)
*   Editor: Fixed that GUISkin was not showing in Object Picker for GUISkin object fields
*   Editor: Fixed: Occlusion Culling scene view overlay window once again always uses dark editor skin, so it is readable
*   Editor: Fixed: NavMesh scene view overlay window once again always uses dark editor skin, so it is readable
*   Editor: Fixed: Error spam in Console when modifying a box collider using collider handles
*   Editor: Only set keyboard focus upon clicking a PrefixLabel if the control supports keyboard focus.
*   Editor: Fixed two biggest progress bar leaks on OS X
*   Editor: Vertex snapping (V) now works for sprites.
*   Editor: Fix script execution order on reload
*   Editor: Fix occasional crash when importing assets.
*   Editor: AssetPostprocessors without a default constructor no longer crashes the editor.
*   Editor: Fix ScriptableObject having wrong icon in ObjectField.
*   Editor: PropertyDrawer attributes on members that are arrays are now applied to each element in the array rather than the array as a whole. This was always the intention since there is no other way to apply attributes to array elements, but it didn't work correctly before. Apologies for the inconvenience to anyone who relied on the unintended behavior for custom drawing of arrays.
*   Editor: Fix context menu for ScriptableObject having nonsensical entries (mostly Component-related). Also, "Edit Script" is now only shown if a script is available for editing (not the case for e.g. GUISkin or Terrain).
*   Editor: Fix light skin inspector sometimes using game skin for drawing controls.
*   Editor: GameObjects that end up with multiple transform components will now have extraneous transforms removed automatically; prevents crashes.
*   Editor: Fixed a crash when calling AssetDatabase.CreateAsset on a GameObject.
*   Editor: Fixed errors and crashes when having non-ASCII characters somewhere in the paths for font assets.
*   Editor: Fixed crash when inspecting a disabled terrain; or deleting a material assigned to Terrain.
*   Editor: Fix Scene View Gizmo hover effect that has been broken for several releases.
*   Editor: Fix that clicking cancel on the build progress bar causes loss of scene and any unsaved work.
*   Editor: Fix that Windows progress bar displays incorrect progress when used from user scripts.
*   Editor: Ensure error sound is not playing on OSX when using keyboard shortcuts for particle effect.
*   Editor: Fix wrong context menu in the results of Asset Store searching in Project view.
*   Editor: Curve preset library now retains wrap settings.
*   Editor: Object picker prematurely populates Animation component.
*   Editor: Fixed undo not working with color picker.
*   Editor: When calling EditorGUI.PropertyField with includeChildren set to true, the children did not have correct spacing.
*   Editor: Labels and buttons no longer draw on top of each other in the preview of an animation clip from the asset store with a narrow inspector or preview window.
*   Editor: TextEditor now scrolls to show the composition string when using IME. Furthermore, scrolling offset is now respected when IME pane is positioned so it doesn't end up in weird positions if the text field has scrolled.
*   Editor: Fix scroll speed in Particle Effect window; and fixed broken UI layout in particle system scene view overlay.
*   Editor: Fix so shortcuts can be used to give the Project Browser window focus (Ctrl/Cmd + 5) and then start a search (Ctrl/Cmd + F).
*   Editor: Fix main editor window covering an auto-hidden taskbar when maximized on Windows.
*   Editor: Fix double dropshadowing issues for windows on Windows (fixes odd dropshadowing on adjacent monitors when the editor was maximized).
*   Editor: Fixed files showing multiple times when deleting multiple folders in Project Browser.
*   Editor: Fix assets could incorrectly be created in the Assets folder in two column mode.
*   Editor: Textures with Alpha Is Transparency Selected, will have their thumbnail correctly generated with a transparent background.
*   Editor: Prevent setting terrain resolution higher than 2049 via the inspector (can still be done from scripting API, to avoid breaking existing code).
*   Editor: 3D textures were not displayed properly in material inspector.
*   Editor: Catch errors when trying to rename classes in the project view.
*   Editor: Disable Compression option in Audio Importer for Native WAV files as they can't be compressed.
*   Editor: Fixed Camera Volumes legend in Occlusion Culling in-scene window.
*   Editor: Fixed changing the script type in the MonoBehaviour component when using multi-object selection.
*   Editor: Fixed IntPopup fields not opening on space.
*   Editor: Fixed tooltips for GUI.SelectionGrid; and log a warning if user tries to create invalid SelectionGrid.
*   Editor: Only focus dropdown window if doesn't have focus already.
*   Editor: On Windows EditorGUIUtility.AddCursorRect does not wait for a mouse movement to update the cursor anymore.
*   Editor: Fixed the hard crash happened when updating one package to a new version.
*   Editor: Fix the inappropriate cache server warnings
*   Editor: Fix the bug that crash unloading AssetBundle when exiting Play mode
*   Editor: Fix the crash when deleting ScriptableObject
*   Fix: ASTC textures were imported with Y-axis flipped
*   Fix crash when passing prefab instance to PrefabUtility.ReplacePrefab
*   Fix the Editor crash on getting component by type if type was null
*   Fix occlusion culling when camera is outside generated view volumes
*   Fix occlusion culling license issue
*   Fixed profiling of shadow caster culling, cases where there are no shadow casting lights.
*   Fix error messages in Windows Store Apps and WP8 when checking for location capability
*   Fix errors when snapping on Windows Store Apps
*   Fix: GPU skinning on DX11 was limited to 128 bones per mesh, limit upped to 1024.
*   Fix F10 and Shift keys in Windows Store Apps
*   Fix crash in WSA/WP8 when using Compass
*   Fix internal exception and performance issue in WSA/WP8 using Compass on device without it
*   Fix serious performance drop in WSA/WP8 using Compass on some devices
*   Fix Editor hanging when entering play mode or quitting the application
*   Flash: Fix leaking AssetBundle APIs.
*   Flash: Fix Flash UnityContentLoader unloading. ("TypeError: Error #1034: Type Coercion failed: cannot convert System::ClassType...")
*   Flash: Fix Flash Monobehaviour Serialization issues
*   Flash: Support up to Flash 11.8, this allows 11.5 and upwards non-content debugger players to display a stack trace.
*   Flash: Fixed dynamic batching sometimes failing.
*   Font rendering: Fix alignment of text with embedded images.
*   Font rendering: Allow embedded images to render in non-square aspect ratios.
*   Graphics: Fixed a crash when accessing Camera.current in the Editor in Start().
*   Graphics: Fixed a crash when switching to DX11 mode and the scene has terrain in it.
*   Graphics: Fixed a deadlock in the mutithreaded renderer when entering the Lion-style fullscreen on Mac.
*   Graphics: Fixed a null reference exception in combining for static batching when there was no first material in Renderer's material array.
*   Graphics: Fixed asserts caused by broken render texture stats when using graphics emulation.
*   Graphics: Fixed changes to QualitySettings.vSyncCount after Screen.SetResolution() causing fullscreen setting to be ignored.
*   Graphics: Fixed GPU skinning (both DX11 and OpenGL ES 3.0) when the mesh is using a low number of bones
*   Graphics: Fixed QualitySettings.anisotropicFiltering changing values inconsistently when set from scripts.
*   Graphics: Fixed Texture.GetNativeTextureID() not being thread-safe with multi-threaded rendering.
*   Graphics: Fixed webplayer plugin crash
*   Graphics: Fixed wrong vertex count being reported in Stats window when static batching is used and editor is in Direct3D 9 mode.
*   Graphics: Fixed broken shadows with forward rendering to antialiased RenderTexture.
*   Graphics: Fixed crash when calling Texture2D.ReadPixels() with a negative offset.
*   Graphics: Fixed crash when using Graphics.Blit under some circumstances.
*   Graphics: Fixed Graphics.Blit crash issue.
*   Graphics: Fixed shaders using 2 UV sets not working in Player if mesh only has one set, and was imported without Read/Write Enabled.
*   Graphics: Fixed bounds of meshes generated by TextMesh component.
*   Graphics: RenderTextures are no longer unnecessarily cleared when loading a new level.
*   Graphics: OpenGL ES 2.0 now supports mipmapped render textures.
*   Graphics: Fixed cubemap + mipmap render textures on OpenGL.
*   Graphics: Fixed a rare case of light probe sampling taking too much time.
*   Graphics: Fix crash on scene load when baked occlusion data is present
*   IMGUI: MousePosition should work properly inside a GUI.window when GUI.matrix is not identity.
*   Input: Input state now being reset consistently cross-platform when player focus is lost.
*   iOS: Fixed iOS builing on Windows
*   iOS: Fixed various scrolling related crashes on iOS 7
*   iOS: Fixed Xcode 5 build & run for simulator target
*   iOS: Fixed gyro reporting
*   iOS: Fixed iOS project building from script on Windows.
*   iOS: Fixed iOS7 simulator support.
*   iOS: Fixed managed code stripping when building project on Windows.
*   iOS: Fixed WebCamTexture support for iOS7
*   iOS: Fixed iOS7 icon size support
*   iOS: Xcode 5 Build&Run support fixed
*   iOS: Fixed MeshCollider stripping issue.
*   iOS: Improved error propagation in WWW class.
*   iOS: Fixed Norwegian language detection.
*   iOS: Make sure all NSString backing device settings are retained.
*   iOS: Fixed OnCollision broken by stripping, when you don't use Collision class explicitly.
*   iOS: Fixed trampoline's precompiled header not working with .c/.m files.
*   Linux: Fix player crash when a user manually specifies an invalid resolution.
*   Linux: Fix custom cursor handling when hiding/showing cursor.
*   Mac OS X 64 bit Standalone: fix WebCam support
*   Mac OS X Standalone: Changed compile settings to disable running on 10.4 (which we did not support anyways), as this is now a requirement for publishing to Steam.
*   Mac OS X Standalone: Fix cursor locking when setting Screen.lockCursor in first Awake call
*   Mac OS X Standalone: Fixed Mouse coordinates on secondary screens
*   Mac OS X: Fixed support for cursors with NPOT cursor textures
*   Mac OS X: Make Icon and Splash screen work for 64 bit standalone builds.
*   Mac OS X: Fixed non-ASCII characters in Input.inputString
*   Mac OS X: Fixed issues with windows handling for GameCenter in standalone builds.
*   Mac OS X: Fix Input.inputString to correctly contain whitespace characters in the web player.
*   Mecanim: Model importer meta file shouldn't get dirty anymore when importing a file with a Humanoid rig.
*   Mecanim: Fix crash when previewing transition between empty states
*   Mecanim: Fix object hierarchy not being animated correctly in some cases
*   Mecanim: Fix remove State/StateMachine code that caused bad object access
*   Mecanim: Fixed crash when trying to configure an Avatar with a mesh not yet skinned.
*   Mecanim: Fixed cannot configure a human avatar when optimize is ON.
*   Mecanim: Fixed crash when calling Animator.GetBoneTransform on Avatar with Optimize Game object On.
*   Mecanim: Fixed crashes when editing humanoid animation applied to a primitive object.
*   Mecanim: Fixed drag'n drop of State/StateMachine.
*   Mecanim: Fixed Optimize GameObject in import settings breaks preview window of Skinned Mesh,
*   Mecanim: Fixed preview of a transition on a layer with a mask, previewer was not using the mask to playback the transition.
*   Mecanim: Fixed root motion masking for all layer.
*   Mecanim: Fixed the crash which happened when we reimport the FBX file in play mode.
*   Mecanim: Fixed transitions bool parameter being overriden when creating the 1st Trigger parameter.
*   Mecanim: Hide "Optimize Game Objects" if Avatar Definition is "Copy From Other Avatar".
*   Mecanim: Proper clamping of start/stop times when importing an Animation clip.
*   Mecanim: Update Controller's clip duration when an AnimationClip is substituted by AnimationOverrideController.
*   Mecanim: Fixes animation set crash when clips are duplicated in controller.
*   Mecanim: Avatar created proceduraly should not expose Configure Avatar button.
*   Mecanim: User should get an error in the console when they try to create an avatar with duplicate transform in the human mapping.
*   Mecanim: Fix various crash with Optimize game object and configure Avatar.
*   Mecanim: Fix crash when user configure an existing avatar and try to edit the muscle limit,
*   Mecanim: Fix crash when user delete and animator component.
*   Mecanim: Fix crash when user set the root node on a generic rig to the top most object in hierarchy.
*   Mecanim: Animation Average Velocity was not computed correctly.
*   Mecanim: Preview of animation breaks on avatars with different hips orientation.
*   Mecanim: Switching from Generic to Humanoid rig when using source Avatar was breaking animation import.
*   Mecanim: Support scale of game object at runtime for Animator. Root Motion, IK, Optimize Hierachy.
*   Mecanim: Unroll muscle fix.
*   Mecanim: Sync editor curve for pre-4.3 duplicated muscle clip and backward compatibility problem with duplicated clips.
*   Mecanim: Change default behavior for human clip, do not import position, rotation and scale curve for all human transform.
*   Mecanim: StateMachine GraphGUI did not support properly to have its data modified externally.
*   Mecanim: Fixes webplayer compatibility for Mecanim bindings.
*   Mecanim: ModelImporter multi-edition of root node and expose transform should be disabled when transform from multiple file doesn't match.
*   Mecanim: Better validation of avatar creation.
*   Mecanim: Re-added AnimationUtility.GetAnimationClips(Animation animation) in the API as deprecated.
*   Mecanim: Fixed crash when applying change in Avatar Tools with an invalid avatar.
*   Mecanim: Fixed StopTime not being set properly when resampling a transition in the previewer.
*   Mecanim: Fixed scale curved that where not evaluated properly.
*   Mecanim: Fixed continuity issue on transitions with duration of zero.
*   Mecanim: Fixed broken additive layer evaluation.
*   Mecanim: Fixed broken bindings when source hierarchy differs from destination.
*   Mecanim: Prevent opening muscle previewer in Avatar Setup with incomplete Avatar.
*   Mecanim: Fixed Crash when clicking on Clear mapping button in Avatar tools.
*   Mecanim: Fix the default pose (when a character is not animated) when humanoid mode or a root bone is used. This makes it consistent with the default pose in the authoring tool (eg. Maya).
*   Mecanim: Fixed crash when calling Animator.GetBoneTransform with an Uninitialized Animator.
*   Mecanim: Recorder cannot longer play unrecorded frame.
*   Mecanim: Restrict use of negative animator speed while recording.
*   Mecanim: Fix Ctrl-click selection for states and transition.
*   Mecanim: Fix negative scale blending while in a transition.
*   Mecanim: Fix Additional curves tangent, Non default tangent was not supported correctly.
*   Mecanim: Fix in Muscle Unroll Algorithm.
*   Mecanim: Fix loading of .anim files generated in 4.0/4.1/4.2
*   Mecanim: Fix memory spill when using Layers
*   Memory Profiler shows Static Managed References as a reason for why an asset is loaded
*   Memory: Fixed leak when instantiating materials from code
*   Mobile: Do not include fonts into mobile build when rendering mode is OS and including the font is not specified.
*   Mobile: Fixed point topology rendering.
*   Mobiles: 24-bit Depth Buffer is now enabled by default
*   MonoDevelop: Disable broken fullscreen mode on OSX.
*   MonoDevelop: Fix exception when creating a new UnityScript or Boo class from MD.
*   MonoDevelop: Fix tab selector freeze when resizing the code editor UI.
*   MonoDevelop: Fix exception when jumping to declaration of a symbol in an external assembly.
*   MonoDevelop: Fix intermittent, unhandled exception when opening the Unity API reference.
*   MonoDevelop: Remove unsupported entries from menus.
*   MonoDevelop: Fix cursor warp.
*   MonoDevelop: Don't flush folding and undo data on document save.
*   MonoDevelop: Show debugging toolbar when attaching.
*   MonoDevelop: Make play button attach instead of launching new Unity instance.
*   MonoDevelop: Fix Boo compilation failure every first compile (Windows).
*   MonoDevelop: Fix Unityscript compilation (Windows).
*   NavMesh: Changed NavMeshAgent.hasPath to return consistent values on off-meshlinks and while walking.
*   NavMesh: Fixed issue where NavMeshAgents was restoring the velocity before entering offmeshlink when leaving it
*   NavMesh: Fix regression causing agents moving on terrain to have wrong height (y-position) when "Height Mesh" bake option is enabled
*   OSX Player: Fixed crash when loading a release build
*   OpenGL ES 3.0: Fixed shadow rendering in Deferred rendering mode.
*   OpenGL ES 3.0: Various fixes and stability improvements.
*   Physics: Fix OnTriggerEnter being called repeatedly for CharacterControllers when setting transform.parent
*   Physics: Fix potential crash when deleting colliders while Time.timeScale is zero
*   Physics: Fix Terrain.GetInterpolatedNormal to return correct normals
*   Physics: Fixed a bug where Continuous Collision detection would not work correctly when changing the scale of colliders.
*   Physics: It is now possible to have multiple SpringJoint components on a single GameObject, like with all other Joints.
*   Physics: Rigidbodies will now wake up when changing constraints, so that a Rigidbody which is being held in position by a constraint will start moving.
*   Physics: All combine modes are now correctly applied to friction and bounciness properties of physics materials. Before that, the interpretation of Multiply and Minimum modes was switched.
*   Physics: Fix crash when using MeshCollider with a mesh which only contains degenerate faces.
*   Physics: Fixed a bug where MeshColliders would enable themselves when changing the transform when they were disabled.
*   Physics: Fixed a crash related to sending collision notifications.
*   Physics: Fix the MovePosition feature of a kinematic compound rigidbody.
*   Physics: fix crash when reloading scene with invalid physics materialPrefabs: Fixed cases where prefab merging injected additional transform components into prefab instances.
*   Physics: Fix 2D colliders spamming console log with "m\_InstanceId==0"
*   Prefabs: Fix awake order for prefabs which have other prefabs as children
*   Profiler: Camera render to Texture is now added to the profiler.
*   Rendering: Fixed accessing Cloth.vertices when there is no vertices assigned yet.
*   Scripting: Fixed a crash when trying to serialize abstract classes in MonoBehaviours.
*   Scripting: Fix memory leak occurring during Play/Stop and script compilation.
*   Scripting: CodeDomProvider can be used in Editor
*   Scripting: Fixed InvalidProgramException for binding delegate to instance method with null target.
*   Scripting: Fixed crash when calling ScriptableObject.CreateInstance with abstract type.
*   Scripting: More informative error message about use of enums with unsupported underlying type.
*   Scripting: Infinite Loop on RequireComponent.
*   Scripting: Fix crash when instantiating a scriptable object with a mismatched file name.
*   Scripting: Allow StopCoroutine from within a coroutine.
*   Scripting: Avoid spurious allocations when using terrains with shadows.
*   Scripting: Eliminate misplaced Editor.SetDirty warning in players.
*   Scripting: Fix crash when subclassing Component.
*   Shaders: hlsl-to-glsl translator now accepts "static" and "const" qualifiers on function return values.
*   Shaders: hlsl-to-glsl translator was producing variable names with double-underscore in some cases (which is not accepted by some drivers).
*   Shaders: Shader compiler now consistently accepts project-root relative #include paths.
*   Shaders: Fixed #pragma multi\_compile shader variants not working with surface shaders in some cases.
*   Shaders: Fixed shader compiler crashing with out of memory on complex shaders (with lots of multi\_compile variants).
*   Shaders: Fixed some Material properties getting into a non-save-able state sometimes (they would seem to be editable, but a Unity restart would revert the values back).
*   Shaders: Fixed texCUBEgrad & tex3Dgrad, was not working on some platforms.
*   Shaders: Integer and boolean parameters in shaders (e.g. int, int4, bool) now work as expected on all platforms.
*   Shadows: Fixed performance regression in shadow rendering (introduced in 4.1).
*   Shuriken: Clamp both start lifetime and length in seconds to avoid precision issues.
*   Shuriken: Fixed crash when destroying Mesh used by ParticleSystemRenderer.
*   Substance: Added missing documentation for SubstanceImporter::Get/SetPlatformTextureSettings() and ProceduralTexture::GetPixels32().
*   Substance: Fixed a severe perf regression in scenes with more than 20 ProceduralMaterial instances.
*   Substance: ProceduralTexture::GetPixels32() now works with a simpler call sequence (see documentation).
*   Substance: It is no longer possible to rename the wrong ProceduralMaterial when switching ProceduralMaterial while editing the ProceduralMaterial name field.
*   Substance: Texture thumbnails are now properly spaced when the "Generate all outputs" checkbox is enabled.
*   Substance: The "Generated textures" foldout is no longer displayed when trying to multi-edit ProceduralMaterials.
*   Substance: Renaming a ProceduralMaterial to a recently renamed ProceduralMaterial's previous name will now display the correct preview textures.
*   Substance: Fix a potential Editor crash when trying to perform drag and drop in the SubstanceImporterInspector.
*   Terrain: Fixed popping tree shadow
*   Terrain: Tree colors in linear rendering mode are now rendered correctly.
*   Terrain: Fix crash when using Terrain.activeTerrain in a scene that has no terrain.
*   Terrain: Fixed incorrect color space setting on detail (grass) objects.
*   Text Markup: Fixed parsing of numeric parameters which sometimes read numbers incorrectly.
*   Umbra culling is no longer used for previews. Fixes a crash when selecting cubemaps.
*   Undo operation for asset import settings changes are no longer recorded
*   Undo operation for asset import settings changes are no longer recorded
*   Undo: Fixed undo recording of script changes on MonoBehaviour
*   UnityObject: Correctly identifies IE 11 as a supported browser.
*   Version Control: Fix Submit Window sometimes throwing exceptions on creation.
*   Version Control: Do not show checkout dialog for all reimported models
*   Version Control: Handle moving folder external to Unity
*   Version Control: Only checkout selected assets when user has enabled notify on save in preferences
*   Version Control: Increased timeout for getlatest and submit to better handle slow connections
*   Version Control: Refresh pending window on submit error
*   Version Control: Require ack from vcs plugins on shutdown to prevent deadlock
*   Version Control: Fix context menu for "open containing folder".
*   Version Control: Show correct error message on all submit errors.
*   Version Control: Support perforce workspaces and passwords with spaces.
*   Version Control: Support for perforce streams.
*   Version Control: Disable save option when VCS plugin does not support changelists.
*   WebPlayer: Fixed several XSS bugs
*   WebPlayer: Fixed web player legacy occlusion culling
*   WebPlayer: Web Players can now start on Windows XP systems with Terminal Services disabled, but will not be able to enter full-screen on those systems.
*   WebPlayer: Fixed lock-up issues that occurred when entering fullscreen on OS X.
*   WebPlayer Installer: EULA links have been removed and standard click-through EULAs introduced. The EULA itself has not changed.
*   Windows 64-bit Standalone: Removed dependency on MS CRT redistributable
*   Windows Phone/+ Windows Store Apps: Fixed unity player crashing if fields in user scripts were emitted with #if UNITY\_EDITOR precessor flag.
*   Windows Phone/+ Windows Store Apps: Reference ReWriter will now correctly find replacement method with param arguments if original is not available in the target framework.
*   Windows Phone: Dependencies to WinRTLegacy.dll are now correctly rewrriten.
*   Windows Phone: fix LocationService status
*   Windows Phone: Fixed unity player crashing if back button was pressed while the engine was still reinitializing from application pause.
*   Windows Phone: Reference ReWriter now correctly recognizes System.Uri <---> Windows.Foundation.Uri type alias.
*   Windows Phone: Reference ReWriter now correctly recognizes WinRT aliases when they are a template argument of non-alias class.
*   Windows Phone: UnityScript compiler targets incorrect UnityScript.Lang.dll when building project for WP8
*   Windows Phone: Closing app should no longer crash it.
*   Windows Phone: Fix render texture camera orientation when app is started in landscape.
*   Windows Phone: Fixed a bug where using certain WinRT types would prevent the user from building a project.
*   Windows Phone: Fixed a build system crash if plugin contained a class that inherits from Windows Phone XAML classes.
*   Windows Phone: Fixed a crash caused by disabled sensors capability in project manifest.
*   Windows Phone: Fixed a crash when trying to access temporary and roaming directories.
*   Windows Phone: Fixed a crash when trying to use gyroscope on devices that don't have gyroscope.
*   Windows Phone: Make ScreenOverlay post effect rotate correctly with device orientation.
*   Windows Phone: handle exceptions when sensors are not found
*   Windows Phone: Fixed initialization of LocationService
*   Windows Phone: GameObject.SendMessage invokes correct overloaded method.
*   Windows Phone: WWW class correctly decodes escaped URL strings.
*   Windows Phone: Screenshots are correctly captured in landscape orientation.
*   Windows Phone: App no longer crashes if graphics device is accessed from OnApplicationPause method.
*   Windows Store Apps: fixed GUI events via touches when cursor is locked
*   Windows Store Apps: fixed LocationService DesiredAccuracy usage on Windows 8.1
*   Windows Store Apps: Fixed out of bounds error while batching 2D sprites.
*   Windows Store Apps: fixed parameter marshaling of type 'char' in UnityEngine API, this fixes following Unity functions - Event.character, Font::HasCharacter, Font::GetCharacterInfo. Because of this bug chinese, russian texts in some cases were being displayed incorrectly.
*   Windows Store Apps: fixed starting coroutines with arguments of wrong but compatible tipe
*   Windows Store Apps: PlayerPrefs will be loaded before calling OnEnable function.
*   Windows Store Apps: fix crash in mesh
*   Windows Store Apps: fix freeze on Windows 8.1 when waiting for input
*   Windows Store Apps: Screen.orientation will work correctly (was fixed in 4.3 a1).
*   Windows Store Apps / Windows 8.1: Fixed regression from 4.3 b3, any touch or mouse input won't longer hang the application.
*   Windows Store Apps / Windows 8.1: IDXGIDevice3::Trim will be called on application suspend event, WACK requirement.
*   Windows Store Apps: fix cursor move when Screen.showCursor is set to false
*   Windows Store Apps: Fix AssemblyResolutionException during game postprocess when code references members from Windows namespace.
*   Windows Store Apps: Show "Not applicable" for icon in player settings
*   Windows Store Apps: Allow to unfold and show "Not applicable" for splash in player settings
*   Windows Store Apps & + Windows Phone: Fixed constructor injection, improved error reporting
*   Windows Store App/+ Windows Phone: String with unicode symbols (for ex., Chinese) will be correctly serialized.
*   Windows Store Apps: WWW will correctly load files via file:/// protocol, and won't require internet capability to be enabled.
*   Windows Store Apps: C# files located in Plugins, Standard Assets or Pro Standard Assets won't be compiled against .NET Core even if player setting are set to compile against .NET Core. This way js/boo will be able to access classes from C# files, C# files in other locations can be compiled against .NET Core depending on Player Settings.
*   Windows Store Apps: RequireComponent works now.
*   WSA / WP8: Better error message when UnityScript code calls Eva() function on platforms that don't support it