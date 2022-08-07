# Unity 4.3
https://unity3d.com/unity/whats-new/unity-4.3

## Fixes

<ul>
<li>AI / NavMesh: NavMesh.Raycast: Gives correct navmesh height (Y component) for hit position.</li>
<li>AI / NavMesh: Fix issue where disabling one navmesh obstacle would sometimes affect another obstacle.</li>
<li>AI / NavMesh: Fix NavMeshAgent occasionally getting NaN positions in cases where many agents are spawned/destroyed and avoidance is disabled/enabled.</li>
<li>AI / NavMesh: Fix NavMesh.CalculatePath returning path with wrong path endpoint when path is partial.</li>
<li>Android: Fixed a problem where "Unable to find suitable jdk installation" was presented even with a valid jdk in path</li>
<li>Android: Disabled glTexSubImage2D for adreno devices - fixes some of the dynamic font issues</li>
<li>Android: Fixed default orientation for 3rd gen kindle devices</li>
<li>Android: Fixed stripping issue which caused AndroidJavaRunnable to fail</li>
<li>Android: Fixed ToString error when unboxing java string for AndroidJavaProxy.</li>
<li>Android: Workaround for an issue with the android compositor on external displays.</li>
<li>Animation: Fixed leak in animator component</li>
<li>Animation: Will handle Enable binding correctly.</li>
<li>Animation Window: Update() isn't offered as an option in the add event popup anymore.</li>
<li>Animation Window: Add Curve dialog no longer pops up again after cancelling it</li>
<li>Animation Window: Adding new clips into read-only objects no longer allowed</li>
<li>Animation Window: Animation Event tooltip wasn't showed on mouse hover.</li>
<li>Animation Window: Animation Event window wasn't updated when selection was changed</li>
<li>Animation Window: Changing IsActive property keyframe via animation window is updated into scene view immediately</li>
<li>Animation Window: Curves-toggle is persistent if you close/reopen animation window</li>
<li>Animation Window: Dopesheet clamp framerate between 0-10 000 to avoid data loss for big number</li>
<li>Animation Window: Dopesheet is now able to show more than 50 sprite previews at the same time</li>
<li>Animation Window: Fixed Scale transform is marked yellow in the Inspector although it not animated</li>
<li>Animation Window: In record mode you should be able to animate an Animator Generic rig.</li>
<li>Animation Window: No error messages after removing the animated object</li>
<li>Animation Window: While moving selected keyframes, sometimes other keyframes would move also</li>
<li>Audio: Fix AudioListener.volume for AudioSource.PlayOneShot</li>
<li>Audio: Fix AudioImporterInspector: Compression slider shows wrong max</li>
<li>Audio: Fix Custom audio filter for AudioListener does not affect sounds played by PlayOneShot</li>
<li>Audio: Fixed StackOverflow in OSX Editor during AudioClip.Create</li>
<li>BlackBerry: Fixed issue where gravity was being reported in meters per second instead of G forces. Also landscape x and y for gravity was swapped.</li>
<li>BlackBerry: WebCamTexture.videoVerticallyMirrored is now set correctly.</li>
<li>BlackBerry: Fixed issue where tiling would occur when webcam framerate was set outside acceptable range.</li>
<li>BlackBerry: MailTo URI's now work as expected.</li>
<li>BlackBerry: Remapped gamepad buttons to match up to Xbox 360 controller.</li>
<li>Bug Reporter: Fix crash when submitting documentation bugs from OS X.</li>
<li>BuildPipeline: Custom cursor specified in PlayerSettings is now built and shown correctly.</li>
<li>Cursors: Fix regression with cursor not showing in OS X standalone build.</li>
<li>Documentation: Fixed documentation of EditorUtility.CollectDeepHierarchy.</li>
<li>Documentation: Readded the message "Inherits from" for classes that have a parent.</li>
<li>Documentation: Return types, parameter types and types in examples work as links.</li>
<li>DX11: Fix 100% cpu use on Win81, reduce it somewhat on older windows.</li>
<li>DX11: Handle "-adapter X" command line argument.</li>
<li>Editor: Fixed "set default parameters" button in occlusion-bake tab</li>
<li>Editor: Fixed crash while baking occlusion culling data</li>
<li>Editor: Workaround windows 8.1 + webkit regression causing crash on mouse wheel messages.</li>
<li>Editor: Fix external editor not opening files when double clicking errors in console and external editor arguments have been specified.</li>
<li>Editor: Fixed crash when Transform was referenced multiple times by parent Transform (only happens in corrupt scenes; editor will automatically remove extraneous references now).</li>
<li>Editor: Fixed ScriptableObject editor script reference field being incorrectly drawn with PropertyDrawer.</li>
<li>Editor: Fixed that EditorGUI.LabelField got key focus when tabbing (its now skipped when tabbing)</li>
<li>Editor: Fixed that mouse cursor over gradient alpha input field was showing as drag area instead of text area</li>
<li>Editor: Fixed that tabbing through controls jumps back to "active" checkbox for the game object instead of moving to the next gui control</li>
<li>Editor: Fixed that the static toggle in inspector does not update correctly when toggled, if the current value is "mixed"</li>
<li>Editor: Disabled GPU Profiler on Macs + NVIDIA GeForce 650M, turns out the drivers return garbage data.</li>
<li>Editor: Do not disable the lighting flag in the scene view after completing a build</li>
<li>Editor: Don't leak references to assemblies that are dynamically loaded from game code.</li>
<li>Editor: Fix input sometimes being sent to windows that have already been destroyed causing PPtr dereference asserts.</li>
<li>Editor: Fix static preview generation to have the right background color in linear mode</li>
<li>Editor: Fixed import of Reflection textures sometimes freezing the Editor when Fixup Edge Seams is checked.</li>
<li>Editor: Fixed unclear and flickering DX11 tool tip message in Player Settings on Mac.</li>
<li>Editor: It's now possible to undo changing batching settings in the PlayerSettings</li>
<li>Editor: Mark BeginGUI(Rect) as obsolete, as it leads to bad internal GUI state</li>
<li>Editor: Fix Object Picker causing nullrefs when shown outside of OnGUI.</li>
<li>Editor: Opening PopUp menus with the keyboard on windows will no longer beep.</li>
<li>Editor: Closing a editor tab shouldn't change the selected tab.</li>
<li>Editor: Fix that Preferences key shortcuts using toggle with CTRL didn't work on Windows.</li>
<li>Editor: Fixed searching for Terrain in the Hierarchy or Project window (use t:terrain)</li>
<li>Editor: Fixed searching for GUISkin in Project Browser (use t:guiskin)</li>
<li>Editor: Fixed that GUISkin was not showing in Object Picker for GUISkin object fields</li>
<li>Editor: Fixed: Occlusion Culling scene view overlay window once again always uses dark editor skin, so it is readable</li>
<li>Editor: Fixed: NavMesh scene view overlay window once again always uses dark editor skin, so it is readable</li>
<li>Editor: Fixed: Error spam in Console when modifying a box collider using collider handles</li>
<li>Editor: Only set keyboard focus upon clicking a PrefixLabel if the control supports keyboard focus.</li>
<li>Editor: Fixed two biggest progress bar leaks on OS X</li>
<li>Editor: Vertex snapping (V) now works for sprites.  </li>
<li>Editor: Fix script execution order on reload</li>
<li>Editor: Fix occasional crash when importing assets.</li>
<li>Editor: AssetPostprocessors without a default constructor no longer crashes the editor.</li>
<li>Editor: Fix ScriptableObject having wrong icon in ObjectField.</li>
<li>Editor: PropertyDrawer attributes on members that are arrays are now applied to each element in the array rather than the array as a whole. This was always the intention since there is no other way to apply attributes to array elements, but it didn't work correctly before. Apologies for the inconvenience to anyone who relied on the unintended behavior for custom drawing of arrays.</li>
<li>Editor: Fix context menu for ScriptableObject having nonsensical entries (mostly Component-related). Also, "Edit Script" is now only shown if a script is available for editing (not the case for e.g. GUISkin or Terrain).</li>
<li>Editor: Fix light skin inspector sometimes using game skin for drawing controls.</li>
<li>Editor: GameObjects that end up with multiple transform components will now have extraneous transforms removed automatically; prevents crashes.</li>
<li>Editor: Fixed a crash when calling AssetDatabase.CreateAsset on a GameObject.</li>
<li>Editor: Fixed errors and crashes when having non-ASCII characters somewhere in the paths for font assets.</li>
<li>Editor: Fixed crash when inspecting a disabled terrain; or deleting a material assigned to Terrain.</li>
<li>Editor: Fix Scene View Gizmo hover effect that has been broken for several releases.</li>
<li>Editor: Fix that clicking cancel on the build progress bar causes loss of scene and any unsaved work.</li>
<li>Editor: Fix that Windows progress bar displays incorrect progress when used from user scripts.</li>
<li>Editor: Ensure error sound is not playing on OSX when using keyboard shortcuts for particle effect. </li>
<li>Editor: Fix wrong context menu in the results of Asset Store searching in Project view.</li>
<li>Editor: Curve preset library now retains wrap settings.</li>
<li>Editor: Object picker prematurely populates Animation component.</li>
<li>Editor: Fixed undo not working with color picker.</li>
<li>Editor: When calling EditorGUI.PropertyField with includeChildren set to true, the children did not have correct spacing.</li>
<li>Editor: Labels and buttons no longer draw on top of each other in the preview of an animation clip from the asset store with a narrow inspector or preview window.</li>
<li>Editor: TextEditor now scrolls to show the composition string when using IME. Furthermore, scrolling offset is now respected when IME pane is positioned so it doesn't end up in weird positions if the text field has scrolled.</li>
<li>Editor: Fix scroll speed in Particle Effect window; and fixed broken UI layout in particle system scene view overlay.</li>
<li>Editor: Fix so shortcuts can be used to give the Project Browser window focus (Ctrl/Cmd + 5) and then start a search (Ctrl/Cmd + F).</li>
<li>Editor: Fix main editor window covering an auto-hidden taskbar when maximized on Windows.</li>
<li>Editor: Fix double dropshadowing issues for windows on Windows (fixes odd dropshadowing on adjacent monitors when the editor was maximized).</li>
<li>Editor: Fixed files showing multiple times when deleting multiple folders in Project Browser.</li>
<li>Editor: Fix assets could incorrectly be created in the Assets folder in two column mode.</li>
<li>Editor: Textures with Alpha Is Transparency Selected, will have their thumbnail correctly generated with a transparent background.</li>
<li>Editor: Prevent setting terrain resolution higher than 2049 via the inspector (can still be done from scripting API, to avoid breaking existing code).</li>
<li>Editor: 3D textures were not displayed properly in material inspector.</li>
<li>Editor: Catch errors when trying to rename classes in the project view.</li>
<li>Editor: Disable Compression option in Audio Importer for Native WAV files as they can't be compressed.</li>
<li>Editor: Fixed Camera Volumes legend in Occlusion Culling in-scene window.</li>
<li>Editor: Fixed changing the script type in the MonoBehaviour component when using multi-object selection.</li>
<li>Editor: Fixed IntPopup fields not opening on space.</li>
<li>Editor: Fixed tooltips for GUI.SelectionGrid; and log a warning if user tries to create invalid SelectionGrid.</li>
<li>Editor: Only focus dropdown window if doesn't have focus already.</li>
<li>Editor: On Windows EditorGUIUtility.AddCursorRect does not wait for a mouse movement to update the cursor anymore.</li>
<li>Editor: Fixed the hard crash happened when updating one package to a new version.</li>
<li>Editor: Fix the inappropriate cache server warnings</li>
<li>Editor: Fix the bug that crash unloading AssetBundle when exiting Play mode</li>
<li>Editor: Fix the crash when deleting ScriptableObject</li>
<li>Fix: ASTC textures were imported with Y-axis flipped</li>
<li>Fix crash when passing prefab instance to PrefabUtility.ReplacePrefab</li>
<li>Fix the Editor crash on getting component by type if type was null</li>
<li>Fix occlusion culling when camera is outside generated view volumes  </li>
<li>Fix occlusion culling license issue</li>
<li>Fixed profiling of shadow caster culling, cases where there are no shadow casting lights. </li>
<li>Fix error messages in Windows Store Apps and WP8 when checking for location capability</li>
<li>Fix errors when snapping on Windows Store Apps</li>
<li>Fix: GPU skinning on DX11 was limited to 128 bones per mesh, limit upped to 1024.</li>
<li>Fix F10 and Shift keys in Windows Store Apps</li>
<li>Fix crash in WSA/WP8 when using Compass</li>
<li>Fix internal exception and performance issue in WSA/WP8 using Compass on device without it</li>
<li>Fix serious performance drop in WSA/WP8 using Compass on some devices</li>
<li>Fix Editor hanging when entering play mode or quitting the application</li>
<li>Flash: Fix leaking AssetBundle APIs.</li>
<li>Flash: Fix Flash UnityContentLoader unloading. ("TypeError: Error #1034: Type Coercion failed: cannot convert System::ClassType...")</li>
<li>Flash: Fix Flash Monobehaviour Serialization issues</li>
<li>Flash: Support up to Flash 11.8, this allows 11.5 and upwards non-content debugger players to display a stack trace.</li>
<li>Flash: Fixed dynamic batching sometimes failing.</li>
<li>Font rendering: Fix alignment of text with embedded images.</li>
<li>Font rendering: Allow embedded images to render in non-square aspect ratios.</li>
<li>Graphics: Fixed a crash when accessing Camera.current in the Editor in Start().</li>
<li>Graphics: Fixed a crash when switching to DX11 mode and the scene has terrain in it.</li>
<li>Graphics: Fixed a deadlock in the mutithreaded renderer when entering the Lion-style fullscreen on Mac.</li>
<li>Graphics: Fixed a null reference exception in combining for static batching when there was no first material in Renderer's material array.</li>
<li>Graphics: Fixed asserts caused by broken render texture stats when using graphics emulation.</li>
<li>Graphics: Fixed changes to QualitySettings.vSyncCount after Screen.SetResolution() causing fullscreen setting to be ignored.</li>
<li>Graphics: Fixed GPU skinning (both DX11 and OpenGL ES 3.0) when the mesh is using a low number of bones</li>
<li>Graphics: Fixed QualitySettings.anisotropicFiltering changing values inconsistently when set from scripts.</li>
<li>Graphics: Fixed Texture.GetNativeTextureID() not being thread-safe with multi-threaded rendering.</li>
<li>Graphics: Fixed webplayer plugin crash</li>
<li>Graphics: Fixed wrong vertex count being reported in Stats window when static batching is used and editor is in Direct3D 9 mode.</li>
<li>Graphics: Fixed broken shadows with forward rendering to antialiased RenderTexture.</li>
<li>Graphics: Fixed crash when calling Texture2D.ReadPixels() with a negative offset.</li>
<li>Graphics: Fixed crash when using Graphics.Blit under some circumstances.</li>
<li>Graphics: Fixed Graphics.Blit crash issue.</li>
<li>Graphics: Fixed shaders using 2 UV sets not working in Player if mesh only has one set, and was imported without Read/Write Enabled.</li>
<li>Graphics: Fixed bounds of meshes generated by TextMesh component.</li>
<li>Graphics: RenderTextures are no longer unnecessarily cleared when loading a new level.</li>
<li>Graphics: OpenGL ES 2.0 now supports mipmapped render textures.</li>
<li>Graphics: Fixed cubemap + mipmap render textures on OpenGL.</li>
<li>Graphics: Fixed a rare case of light probe sampling taking too much time.</li>
<li>Graphics: Fix crash on scene load when baked occlusion data is present</li>
<li>IMGUI: MousePosition should work properly inside a GUI.window when GUI.matrix is not identity.</li>
<li>Input: Input state now being reset consistently cross-platform when player focus is lost.</li>
<li>iOS: Fixed iOS builing on Windows</li>
<li>iOS: Fixed various scrolling related crashes on iOS 7</li>
<li>iOS: Fixed Xcode 5 build &amp; run for simulator target</li>
<li>iOS: Fixed gyro reporting</li>
<li>iOS: Fixed iOS project building from script on Windows.</li>
<li>iOS: Fixed iOS7 simulator support.</li>
<li>iOS: Fixed managed code stripping when building project on Windows.</li>
<li>iOS: Fixed WebCamTexture support for iOS7</li>
<li>iOS: Fixed iOS7 icon size support</li>
<li>iOS: Xcode 5 Build&amp;Run support fixed</li>
<li>iOS: Fixed MeshCollider stripping issue.</li>
<li>iOS: Improved error propagation in WWW class.</li>
<li>iOS: Fixed Norwegian language detection.</li>
<li>iOS: Make sure all NSString backing device settings are retained.</li>
<li>iOS: Fixed OnCollision broken by stripping, when you don't use Collision class explicitly.</li>
<li>iOS: Fixed trampoline's precompiled header not working with .c/.m files.</li>
<li>Linux: Fix player crash when a user manually specifies an invalid resolution.</li>
<li>Linux: Fix custom cursor handling when hiding/showing cursor.</li>
<li>Mac OS X 64 bit Standalone: fix WebCam support</li>
<li>Mac OS X Standalone: Changed compile settings to disable running on 10.4 (which we did not support anyways), as this is now a requirement for publishing to Steam.</li>
<li>Mac OS X Standalone: Fix cursor locking when setting Screen.lockCursor in first Awake call</li>
<li>Mac OS X Standalone: Fixed Mouse coordinates on secondary screens</li>
<li>Mac OS X: Fixed support for cursors with NPOT cursor textures</li>
<li>Mac OS X: Make Icon and Splash screen work for 64 bit standalone builds.</li>
<li>Mac OS X: Fixed non-ASCII characters in Input.inputString</li>
<li>Mac OS X: Fixed issues with windows handling for GameCenter in standalone builds.</li>
<li>Mac OS X: Fix Input.inputString to correctly contain whitespace characters in the web player.</li>
<li>Mecanim: Model importer meta file shouldn't get dirty anymore when importing a file with a Humanoid rig.</li>
<li>Mecanim: Fix crash when previewing transition between empty states</li>
<li>Mecanim: Fix object hierarchy not being animated correctly in some cases</li>
<li>Mecanim: Fix remove State/StateMachine code that caused bad object access  </li>
<li>Mecanim: Fixed crash when trying to configure an Avatar with a mesh not yet skinned.</li>
<li>Mecanim: Fixed cannot configure a human avatar when optimize is ON.</li>
<li>Mecanim: Fixed crash when calling Animator.GetBoneTransform on Avatar with Optimize Game object On.</li>
<li>Mecanim: Fixed crashes when editing humanoid animation applied to a primitive object.</li>
<li>Mecanim: Fixed drag'n drop of State/StateMachine.</li>
<li>Mecanim: Fixed Optimize GameObject in import settings breaks preview window of Skinned Mesh,</li>
<li>Mecanim: Fixed preview of a transition on a layer with a mask, previewer was not using the mask to playback the transition.</li>
<li>Mecanim: Fixed root motion masking for all layer.</li>
<li>Mecanim: Fixed the crash which happened when we reimport the FBX file in play mode.</li>
<li>Mecanim: Fixed transitions bool parameter being overriden when creating the 1st Trigger parameter.</li>
<li>Mecanim: Hide "Optimize Game Objects" if Avatar Definition is "Copy From Other Avatar".</li>
<li>Mecanim: Proper clamping of start/stop times when importing an Animation clip.</li>
<li>Mecanim: Update Controller's clip duration when an AnimationClip is substituted by AnimationOverrideController.</li>
<li>Mecanim: Fixes animation set crash when clips are duplicated in controller.</li>
<li>Mecanim: Avatar created proceduraly should not expose Configure Avatar button.</li>
<li>Mecanim: User should get an error in the console when they try to create an avatar with duplicate transform in the human mapping.</li>
<li>Mecanim: Fix various crash with Optimize game object and configure Avatar.</li>
<li>Mecanim: Fix crash when user configure an existing avatar and try to edit the muscle limit,</li>
<li>Mecanim: Fix crash when user delete and animator component.</li>
<li>Mecanim: Fix crash when user set the root node on a generic rig to the top most object in hierarchy.</li>
<li>Mecanim: Animation Average Velocity was not computed correctly.</li>
<li>Mecanim: Preview of animation breaks on avatars with different hips orientation.</li>
<li>Mecanim: Switching from Generic to Humanoid rig when using source Avatar was breaking animation import.</li>
<li>Mecanim: Support scale of game object at runtime for Animator. Root Motion, IK, Optimize Hierachy.</li>
<li>Mecanim: Unroll muscle fix.</li>
<li>Mecanim: Sync editor curve for pre-4.3 duplicated muscle clip and backward compatibility problem with duplicated clips.</li>
<li>Mecanim: Change default behavior for human clip, do not import position, rotation and scale curve for all human transform.</li>
<li>Mecanim: StateMachine GraphGUI did not support properly to have its data modified externally.</li>
<li>Mecanim: Fixes webplayer compatibility for Mecanim bindings.</li>
<li>Mecanim: ModelImporter multi-edition of root node and expose transform should be disabled when transform from multiple file doesn't match.</li>
<li>Mecanim: Better validation of avatar creation.</li>
<li>Mecanim: Re-added AnimationUtility.GetAnimationClips(Animation animation) in the API as deprecated.</li>
<li>Mecanim: Fixed crash when applying change in Avatar Tools with an invalid avatar.</li>
<li>Mecanim: Fixed StopTime not being set properly when resampling a transition in the previewer.</li>
<li>Mecanim: Fixed scale curved that where not evaluated properly.</li>
<li>Mecanim: Fixed continuity issue on transitions with duration of zero.</li>
<li>Mecanim: Fixed broken additive layer evaluation.</li>
<li>Mecanim: Fixed broken bindings when source hierarchy differs from destination.</li>
<li>Mecanim: Prevent opening muscle previewer in Avatar Setup with incomplete Avatar.</li>
<li>Mecanim: Fixed Crash when clicking on Clear mapping button in Avatar tools.</li>
<li>Mecanim: Fix the default pose (when a character is not animated) when humanoid mode or a root bone is used. This makes it consistent with the default pose in the authoring tool (eg. Maya).</li>
<li>Mecanim: Fixed crash when calling Animator.GetBoneTransform with an Uninitialized Animator.</li>
<li>Mecanim: Recorder cannot longer play unrecorded frame.</li>
<li>Mecanim: Restrict use of negative animator speed while recording.</li>
<li>Mecanim: Fix Ctrl-click selection for states and transition.</li>
<li>Mecanim: Fix negative scale blending while in a transition.</li>
<li>Mecanim: Fix Additional curves tangent, Non default tangent was not supported correctly.</li>
<li>Mecanim: Fix in Muscle Unroll Algorithm.</li>
<li>Mecanim: Fix loading of .anim files generated in 4.0/4.1/4.2</li>
<li>Mecanim: Fix memory spill when using Layers</li>
<li>Memory Profiler shows Static Managed References as a reason for why an asset is loaded</li>
<li>Memory: Fixed leak when instantiating materials from code</li>
<li>Mobile: Do not include fonts into mobile build when rendering mode is OS and including the font is not specified.</li>
<li>Mobile: Fixed point topology rendering.</li>
<li>Mobiles: 24-bit Depth Buffer is now enabled by default</li>
<li>MonoDevelop: Disable broken fullscreen mode on OSX.</li>
<li>MonoDevelop: Fix exception when creating a new UnityScript or Boo class from MD.</li>
<li>MonoDevelop: Fix tab selector freeze when resizing the code editor UI.</li>
<li>MonoDevelop: Fix exception when jumping to declaration of a symbol in an external assembly.</li>
<li>MonoDevelop: Fix intermittent, unhandled exception when opening the Unity API reference.</li>
<li>MonoDevelop: Remove unsupported entries from menus.</li>
<li>MonoDevelop: Fix cursor warp.</li>
<li>MonoDevelop: Don't flush folding and undo data on document save.</li>
<li>MonoDevelop: Show debugging toolbar when attaching.</li>
<li>MonoDevelop: Make play button attach instead of launching new Unity instance.</li>
<li>MonoDevelop: Fix Boo compilation failure every first compile (Windows).</li>
<li>MonoDevelop: Fix Unityscript compilation (Windows).</li>
<li>NavMesh: Changed NavMeshAgent.hasPath to return consistent values on off-meshlinks and while walking.</li>
<li>NavMesh: Fixed issue where NavMeshAgents was restoring the velocity before entering offmeshlink when leaving it</li>
<li>NavMesh: Fix regression causing agents moving on terrain to have wrong height (y-position) when "Height Mesh" bake option is enabled</li>
<li>OSX Player: Fixed crash when loading a release build</li>
<li>OpenGL ES 3.0: Fixed shadow rendering in Deferred rendering mode.</li>
<li>OpenGL ES 3.0: Various fixes and stability improvements.</li>
<li>Physics: Fix OnTriggerEnter being called repeatedly for CharacterControllers when setting transform.parent</li>
<li>Physics: Fix potential crash when deleting colliders while Time.timeScale is zero</li>
<li>Physics: Fix Terrain.GetInterpolatedNormal to return correct normals</li>
<li>Physics: Fixed a bug where Continuous Collision detection would not work correctly when changing the scale of colliders.</li>
<li>Physics: It is now possible to have multiple SpringJoint components on a single GameObject, like with all other Joints.</li>
<li>Physics: Rigidbodies will now wake up when changing constraints, so that a Rigidbody which is being held in position by a constraint will start moving.</li>
<li>Physics: All combine modes are now correctly applied to friction and bounciness properties of physics materials. Before that, the interpretation of Multiply and Minimum modes was switched.</li>
<li>Physics: Fix crash when using MeshCollider with a mesh which only contains degenerate faces.</li>
<li>Physics: Fixed a bug where MeshColliders would enable themselves when changing the transform when they were disabled.</li>
<li>Physics: Fixed a crash related to sending collision notifications.</li>
<li>Physics: Fix the MovePosition feature of a kinematic compound rigidbody.</li>
<li>Physics: fix crash when reloading scene with invalid physics materialPrefabs: Fixed cases where prefab merging injected additional transform components into prefab instances.</li>
<li>Physics: Fix 2D colliders spamming console log with "m_InstanceId==0"</li>
<li>Prefabs: Fix awake order for prefabs which have other prefabs as children</li>
<li>Profiler: Camera render to Texture is now added to the profiler.</li>
<li>Rendering: Fixed accessing Cloth.vertices when there is no vertices assigned yet.</li>
<li>Scripting: Fixed a crash when trying to serialize abstract classes in MonoBehaviours.</li>
<li>Scripting: Fix memory leak occurring during Play/Stop and script compilation.</li>
<li>Scripting: CodeDomProvider can be used in Editor</li>
<li>Scripting: Fixed InvalidProgramException for binding delegate to instance method with null target.</li>
<li>Scripting: Fixed crash when calling ScriptableObject.CreateInstance with abstract type.</li>
<li>Scripting: More informative error message about use of enums with unsupported underlying type.</li>
<li>Scripting: Infinite Loop on RequireComponent.</li>
<li>Scripting: Fix crash when instantiating a scriptable object with a mismatched file name.</li>
<li>Scripting: Allow StopCoroutine from within a coroutine.</li>
<li>Scripting: Avoid spurious allocations when using terrains with shadows.</li>
<li>Scripting: Eliminate misplaced Editor.SetDirty warning in players.</li>
<li>Scripting: Fix crash when subclassing Component.</li>
<li>Shaders: hlsl-to-glsl translator now accepts "static" and "const" qualifiers on function return values.</li>
<li>Shaders: hlsl-to-glsl translator was producing variable names with double-underscore in some cases (which is not accepted by some drivers).</li>
<li>Shaders: Shader compiler now consistently accepts project-root relative #include paths.</li>
<li>Shaders: Fixed #pragma multi_compile shader variants not working with surface shaders in some cases.</li>
<li>Shaders: Fixed shader compiler crashing with out of memory on complex shaders (with lots of multi_compile variants).</li>
<li>Shaders: Fixed some Material properties getting into a non-save-able state sometimes (they would seem to be editable, but a Unity restart would revert the values back).</li>
<li>Shaders: Fixed texCUBEgrad &amp; tex3Dgrad, was not working on some platforms.</li>
<li>Shaders: Integer and boolean parameters in shaders (e.g. int, int4, bool) now work as expected on all platforms.</li>
<li>Shadows: Fixed performance regression in shadow rendering (introduced in 4.1).</li>
<li>Shuriken: Clamp both start lifetime and length in seconds to avoid precision issues.</li>
<li>Shuriken: Fixed crash when destroying Mesh used by ParticleSystemRenderer.</li>
<li>Substance: Added missing documentation for SubstanceImporter::Get/SetPlatformTextureSettings() and ProceduralTexture::GetPixels32().</li>
<li>Substance: Fixed a severe perf regression in scenes with more than 20 ProceduralMaterial instances.</li>
<li>Substance: ProceduralTexture::GetPixels32() now works with a simpler call sequence (see documentation).</li>
<li>Substance: It is no longer possible to rename the wrong ProceduralMaterial when switching ProceduralMaterial while editing the ProceduralMaterial name field.</li>
<li>Substance: Texture thumbnails are now properly spaced when the "Generate all outputs" checkbox is enabled.</li>
<li>Substance: The "Generated textures" foldout is no longer displayed when trying to multi-edit ProceduralMaterials.</li>
<li>Substance: Renaming a ProceduralMaterial to a recently renamed ProceduralMaterial's previous name will now display the correct preview textures.</li>
<li>Substance: Fix a potential Editor crash when trying to perform drag and drop in the SubstanceImporterInspector.</li>
<li>Terrain: Fixed popping tree shadow</li>
<li>Terrain: Tree colors in linear rendering mode are now rendered correctly.</li>
<li>Terrain: Fix crash when using Terrain.activeTerrain in a scene that has no terrain.</li>
<li>Terrain: Fixed incorrect color space setting on detail (grass) objects.</li>
<li>Text Markup: Fixed parsing of numeric parameters which sometimes read numbers incorrectly.</li>
<li>Umbra culling is no longer used for previews. Fixes a crash when selecting cubemaps.</li>
<li>Undo operation for asset import settings changes are no longer recorded</li>
<li>Undo operation for asset import settings changes are no longer recorded</li>
<li>Undo: Fixed undo recording of script changes on MonoBehaviour</li>
<li>UnityObject: Correctly identifies IE 11 as a supported browser.</li>
<li>Version Control: Fix Submit Window sometimes throwing exceptions on creation.</li>
<li>Version Control: Do not show checkout dialog for all reimported models</li>
<li>Version Control: Handle moving folder external to Unity</li>
<li>Version Control: Only checkout selected assets when user has enabled notify on save in preferences</li>
<li>Version Control: Increased timeout for getlatest and submit to better handle slow connections</li>
<li>Version Control: Refresh pending window on submit error</li>
<li>Version Control: Require ack from vcs plugins on shutdown to prevent deadlock</li>
<li>Version Control: Fix context menu for "open containing folder".</li>
<li>Version Control: Show correct error message on all submit errors.</li>
<li>Version Control: Support perforce workspaces and passwords with spaces.</li>
<li>Version Control: Support for perforce streams.</li>
<li>Version Control: Disable save option when VCS plugin does not support changelists.</li>
<li>WebPlayer: Fixed several XSS bugs</li>
<li>WebPlayer: Fixed web player legacy occlusion culling</li>
<li>WebPlayer: Web Players can now start on Windows XP systems with Terminal Services disabled, but will not be able to enter full-screen on those systems.</li>
<li>WebPlayer: Fixed lock-up issues that occurred when entering fullscreen on OS X.</li>
<li>WebPlayer Installer: EULA links have been removed and standard click-through EULAs introduced. The EULA itself has not changed.</li>
<li>Windows 64-bit Standalone: Removed dependency on MS CRT redistributable</li>
<li>Windows Phone/+ Windows Store Apps: Fixed unity player crashing if fields in user scripts were emitted with #if UNITY_EDITOR precessor flag.</li>
<li>Windows Phone/+ Windows Store Apps: Reference ReWriter will now correctly find replacement method with param arguments if original is not available in the target framework.</li>
<li>Windows Phone: Dependencies to WinRTLegacy.dll are now correctly rewrriten.</li>
<li>Windows Phone: fix LocationService status</li>
<li>Windows Phone: Fixed unity player crashing if back button was pressed while the engine was still reinitializing from application pause.</li>
<li>Windows Phone: Reference ReWriter now correctly recognizes System.Uri &lt;---&gt; Windows.Foundation.Uri type alias.</li>
<li>Windows Phone: Reference ReWriter now correctly recognizes WinRT aliases when they are a template argument of non-alias class.</li>
<li>Windows Phone: UnityScript compiler targets incorrect UnityScript.Lang.dll when building project for WP8</li>
<li>Windows Phone: Closing app should no longer crash it.</li>
<li>Windows Phone: Fix render texture camera orientation when app is started in landscape.</li>
<li>Windows Phone: Fixed a bug where using certain WinRT types would prevent the user from building a project.</li>
<li>Windows Phone: Fixed a build system crash if plugin contained a class that inherits from Windows Phone XAML classes.</li>
<li>Windows Phone: Fixed a crash caused by disabled sensors capability in project manifest.</li>
<li>Windows Phone: Fixed a crash when trying to access temporary and roaming directories.</li>
<li>Windows Phone: Fixed a crash when trying to use gyroscope on devices that don't have gyroscope.</li>
<li>Windows Phone: Make ScreenOverlay post effect rotate correctly with device orientation.</li>
<li>Windows Phone: handle exceptions when sensors are not found</li>
<li>Windows Phone: Fixed initialization of LocationService</li>
<li>Windows Phone: GameObject.SendMessage invokes correct overloaded method.</li>
<li>Windows Phone: WWW class correctly decodes escaped URL strings.</li>
<li>Windows Phone: Screenshots are correctly captured in landscape orientation.</li>
<li>Windows Phone: App no longer crashes if graphics device is accessed from OnApplicationPause method.</li>
<li>Windows Store Apps: fixed GUI events via touches when cursor is locked</li>
<li>Windows Store Apps: fixed LocationService DesiredAccuracy usage on Windows 8.1</li>
<li>Windows Store Apps: Fixed out of bounds error while batching 2D sprites.</li>
<li>Windows Store Apps: fixed parameter marshaling of type 'char' in UnityEngine API, this fixes following Unity functions - Event.character, Font::HasCharacter, Font::GetCharacterInfo. Because of this bug chinese, russian texts in some cases were being displayed incorrectly.</li>
<li>Windows Store Apps: fixed starting coroutines with arguments of wrong but compatible tipe</li>
<li>Windows Store Apps: PlayerPrefs will be loaded before calling OnEnable function.</li>
<li>Windows Store Apps: fix crash in mesh</li>
<li>Windows Store Apps: fix freeze on Windows 8.1 when waiting for input</li>
<li>Windows Store Apps: Screen.orientation will work correctly (was fixed in 4.3 a1).</li>
<li>Windows Store Apps / Windows 8.1: Fixed regression from 4.3 b3, any touch or mouse input won't longer hang the application.</li>
<li>Windows Store Apps / Windows 8.1: IDXGIDevice3::Trim will be called on application suspend event, WACK requirement.</li>
<li>Windows Store Apps: fix cursor move when Screen.showCursor is set to false</li>
<li>Windows Store Apps: Fix AssemblyResolutionException during game postprocess when code references members from Windows namespace.</li>
<li>Windows Store Apps: Show "Not applicable" for icon in player settings</li>
<li>Windows Store Apps: Allow to unfold and show "Not applicable" for splash in player settings</li>
<li>Windows Store Apps &amp; + Windows Phone: Fixed constructor injection, improved error reporting</li>
<li>Windows Store App/+ Windows Phone: String with unicode symbols (for ex., Chinese) will be correctly serialized.</li>
<li>Windows Store Apps: WWW will correctly load files via file:/// protocol, and won't require internet capability to be enabled.</li>
<li>Windows Store Apps: C# files located in Plugins, Standard Assets or Pro Standard Assets won't be compiled against .NET Core even if player setting are set to compile against .NET Core.  This way js/boo will be able to access classes from C# files, C# files in other locations can be compiled against .NET Core depending on Player Settings.</li>
<li>Windows Store Apps: RequireComponent works now.</li>
<li>WSA / WP8: Better error message when UnityScript code calls Eva() function on platforms that don't support it</li>
</ul>
