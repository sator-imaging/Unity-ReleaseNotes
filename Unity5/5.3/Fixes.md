# Unity 5.3

https://unity3d.com/unity/whats-new/unity-5.3

## Fixes



*   2D: Fix memory leak when using Sprite object field in custom inspector
*   Android: Add support for stencil buffer in RenderTextures on Tegra 3
*   Android: Android 6.0 - Ask for any dangerous permission on startup
*   Android: AndroidJava - Fixed recursion in AndroidJavaProxy
*   Android: Buildpipe - don't open file dialogs when in batch mode
*   Android: Buildpipe - Fixed an issue where projects created on Mac wouldn't build on Windows
*   Android: Buildpipe - Fixed an issue where the Editor would hang if in batch mode without SDK, NDK and JDK properly configured
*   Android: Buildpipe - Fixed IndexOutOfRangeException thrown on plugin package collisions
*   Android: Fix for missing SpeedTree leaves when using and 'best' quality wind zones on Adreno 3xx with OpenGL ES 3.0
*   Android: Fix for physics performance spikes on ARM big.LITTLE devices
*   Android: Fixed a problem where Plugins/Android/res wasn't bundled with the application
*   Android: Fixed an issue where a problematic EGL configuration was picked up on some Samsung devices
*   Android: Fixed an issue where passing large JNI arrays would cause a local reference table overflow
*   Android: Fixed an issue where PlayerPrefs with keys and values containing line breaks would break
*   Android: Fixed an issue where the application would crash if you sent emoji unicode characters to the OnScreenKeybaord
*   Android: Fixed crash affecting some PowerVR 544 devices
*   Android: Fixed crash in ASTC encoder
*   Android: Fixed crash in decompression of PVRTC textures on non-PVR devices
*   Android: Fixed INTERNET permission on Android even if there are no network calls in the scripts
*   Android: Fixed MSAA on newer ARM Mali devices like Samsung Galaxy S6
*   Android: Fixed MSAA RenderTextures on Tegra4 and K1 when using OpenGL ES 2.0
*   Android: Fixed non-working textures on some Tegra 3 and Tegra 4 devices
*   Android: Fixed OBB deployment on Android 6.0 and some older devices
*   Android: Fixed OnApplicationPause() event on app start
*   Android: Fixed reported texture size in profiler for formats that are decompressed during upload
*   Android: IL2CPP - Fixed compilation on paths with spaces
*   Android: Manual updates of the SDK should now take effect when prompted for an update in the Editor
*   Android: Removed some egl errors from the log when probing for GLES API level
*   Android: Removed the 'soft' cursor
*   Android: SoftInput - Fixed hint color
*   Android: Stripping - don't strip AssetBundle class or it removes LoadAssetAsync
*   Android: Support for galaxy camera volume buttons (zoom in/out)
*   Animation: Fixed a case where non-resampled curves would have overlapping keyframes
*   Animation: Fixed animation of material properties in the animation window.
*   Animation: Fixed animation window still recording when scene is saved.
*   API Updater: Fix crashing when checking for obsolete API in assemblies referencing unity extensions
*   API Updater: Fixed handling of multiple "defines" / references in a single argument in response files
*   Asset Importing: Fix main thread assert when releasing MonoScript object
*   Asset Loading: Allow extension dlls to be imported outside of project folder
*   AssetBundle: Fix the issue that the sprite atlas has been stored twice in AssetBundles.
*   Assets Management: All assets located inside the Resources folder are now reported in the summary area of the editor's output log.
*   BestFit min/max sizes are now clamped so that always include the starting/default font size. This guarantees that minSize <= startingSize <= maxSize.
*   Build Pipeline: Fixed warning message "Failed to add the asset file size for **filename**".
*   CacheServer: Add Cache Server version in terminal
*   CacheServer: Fix server crashes on command 'nc -zv'
*   Canvas is no longer has an incorrect x offset when the viewport rect is anything other than (0, 0, 1, 1) on D3D9, XBOX360, and PSP2.
*   Caret and selection highlight now draw with correct y position and height in UI.InputField for all formats and line spacings.
*   Copying to the clipboard is now disabled for UI.InputField with ContentType of Password.
*   Core: When building a player Editor.log displayed incorrect file size if project had Resource folder with textures in it
*   Crunch texture compression: Fix errors when baking light maps on scenes with crunched textures
*   Crunch texture compression: Fix memory corruption crash when using crunched textures as Cubemaps
*   Crunch texture compression: Fix using crunched textures on terrains
*   Disable expanding the navmesh clipping hull beyond the collected list of affected polygons - could cause t-junctions.
*   DisplayProgressBar replaces forward slash with a backslash
*   Editor: Fixed Handles.DrawDottedLines not working when intersecting near plane. Improved performance of the function as well.
*   Editor: Fix for NullReferenceExceptions while dropping prefab in the scene view
*   Editor Fix Shift-Delete in rename box deleting asset in scene.
*   Editor Fixed a case of new lines in labels when the display name comes from an array of strings.
*   Editor slowdown in Project window with Unity 5
*   Editor Use the correct image for Dark skin's horizontal scrollbar left button
*   Editor: Add drop target rendering for icon view in Project Browser when hovering over a drop target
*   Editor: Added a printed warning to the gameview if there is no fullscreen camera present
*   Editor: Assert Import dialog will correctly appear in the taskbar on Windows, previously you needed to click on the dialog for it to appear in the taskbar or wait until the import is finished.
*   Editor: Asset importer now skips assets and res folders inside Assets/Plugins/Android.
*   Editor: Better UI for ShaderVariantCollection "add variant" functionality.
*   Editor: EditorWindow OnClose() and OnDestroy() will now be called when the Unity Editor is closed.
*   Editor: Fix ArgumentOutOfRangeException when attempting to delete last character of TextField with length limit
*   Editor: Fix crash on Editor quit while the profiler is enabled
*   Editor: Fix for GUI methods in Update crashes the editor
*   Editor: Fix memory thrashing when Dragging and Dropping between panels, when the dragged object had a CustomEditor with no Preview.
*   Editor: Fix mismatched layout group in MeshRenderer editor
*   Editor: Fix project browser searching so 't:Object': also returns ScriptableObjects
*   Editor: Fix searching for labels with characters in front of the 'l:' syntax in the project browser
*   Editor: Fix so searching for special symbols (like @) works in project browser
*   Editor: Fix texture preview not showing mip previews for RenderTextures.
*   Editor: Fix that the search results in Project view is not refreshing when changing labels
*   Editor: Fixed "Ctrl" click on object selects another object in scene view
*   Editor: Fixed bug when opening new project throws "Moving file failed" dialog on Mac
*   Editor: Fixed changing a GameObject's icon failing when changing it for the first time.
*   Editor: Fixed error message when attempting to add a given component to the same game object more than once.
*   Editor: Fixed exception being thrown when multiple assets were selected and one or more contained ScriptableObjects with missing script references.
*   Editor: Fixed inspector preview bug when UI RawImage had negative UV values.
*   Editor: Fixed issue with unnecessary whitespace being added to generated MonoDevelop/VS solution (.sln) files after each update.
*   Editor: Fixed mispositioned arrows in the inspector.
*   Editor: Fixed rare crash when a component is missing a script reference
*   Editor: Fixes Nullref when trying to maximize a view through the Context menu.
*   Editor: Launch unity through command line with the –buildTarget switch and the scripting defines will not be set properly.
*   Editor: Multi selecting GameObjects should be as fast as it was in 4.6
*   Editor: Multiple object renaming in the inspector does not work in some conditions.
*   Editor: Multiselecting textures with different override settings now shows the correct "-" symbol.
*   Editor: Prefab properties will be preserved in case the Editor shuts down unexpectedly.
*   Editor: Prefab will be updated correctly in the Project View when Apply or GameObject/Apply Changes to Prefab is selected and Cache Server is enabled.
*   Editor: Removed MonoDevelop Solution Properties checkbox from External Tools. Unity no longer writes MonoDevelop code formatting settings into MonoDevelopSolutionProperties in .sln file.
*   Editor: Show a note in legacy cubemap inspector about destructive operations
*   Editor: Show a note next to texture aniso slider when it won't have effect due to global quality setting
*   Editor: Show import warning when manually selected texture compression format was changed due to unsupported platform
*   Editor: The camera culling mask would display "Mixed..." incorrectly in various situation. Now correctly reflects render layer state.
*   Editor: The current control with focus now correctly resets to none between Play runs of the open scene.
*   Ensure that when refreshing the shown value of a Dropdown while there are no options at all, the Dropdown value becomes blank rather than keeping showing a previously valid value.
*   Fix for regression - agent was reporting no path when moving over OffMeshLink.
*   Fix for regression - navmesh carving would sometimes collapse degenerate triangles in a way that could affect other polygons.
*   Fix for shadow-casting light occlusion issues - disappearing realtime lights
*   Fix issue where agent’s area cost settings were overwritten with global cost settings - when doing NavMeshAgent.CalculatePath.
*   Fix Mono Assembly stripping
*   Fixed an issue where opening the editor with a Preview window in the layout would cause the inspector tab icon to disappear
*   Fixed ArgumentOutOfRange being thrown when InputField Text component clips all text (e.g. when font is too large).
*   Fixed GUILayout.EndHorizontal() throwing an exception after calling BuildPipeline.BuildAssetBundles
*   Fixed incorrect behavior for GetHasMoved in UI.CanvasRenderer.
*   Fixed incorrect kerning calculations for scaled text.
*   Fixed incorrect line spacing when using rich text and tag to set font size less than the value set in the Text property.
*   Fixed incorrect pixel perfect rounding on high DPI (retina) displays.
*   Fixed incorrect vertical positioning of wrapped word when word-wrapping text with pixel perfect rounding.
*   Fixed InputField selection highlight and caret no longer being visible.
*   Fixed issue that caused FontUpdateTracker to add an additional RebuildForFont handler whenever a Text component was enabled using a font with no other active Text components using that font.
*   Fixed issue where objects lit by light probes appear brighter than static objects with same material in gamma mode. See upgrade guide for details.
*   Fixed issue with all text not displaying correctly in UI.InputField.
*   Fixed problem where characters would sometimes get incorrect kerning information.
*   Frame Debugger: Fixed shader blend/depth/raster state settings sometimes not displayed correctly.
*   GetComponent, in cases where T is an interface, will no longer incorrectly skip matching non monobehaviours
*   GI: Brought back the separate Emission(Lightmapper) component in LegacyShaders/Self-Illumin that went missing in Unity 5.0
*   GI: Fix crash when exiting the editor while building lighting.
*   GI: Fix memory leak eventually causing a crash when baking lightmaps using bad UVs.
*   GI: Fix realtime GI errors about loading hashed files when opening different scenes.
*   GI: Fixed a crash when switching scenes when at least one of them was using realtime GI and light probes.
*   GI: Fixed additive loading of static lightmaps on terrains.
*   GI: Fixed Baking Progress Bar hanging with "Bake paused in play mode.
*   GI: Fixed clustering scene view causing loading bars to pop up all the time during bake when clustering files were reloaded.
*   GI: Fixed crash when calling SetEmissive for a system with no radiosity data available.
*   GI: Fixed crash when marking object from an FBX file containing 3DSMax Camera Nodes to be Lightmap Static.
*   GI: Fixed issue where Emission in Legacy Self Illum Diffuse was clamped to 8.
*   GI: Fixed light hashing always done even when GI is off, causing performance slowdown.
*   GI: Fixed light probes in player builds.
*   GI: Fixed orientation of skybox used for generating ambient probe (it was wrong on Windows and Linux).
*   GI: Now terrain heightmap painting can correctly trigger the baking of GI on that part of the terrain and the editor won't crash when a terrain is duplicated.
*   GI: Removed editor log spamming: Error: GetProbeInterpolants - probe sets that aren't regular grids require...
*   Graphics: Fix crash trying to set shader name on shader that failed to compile
*   Graphics: Fix crash when calling Texture.Compress for large textures
*   Graphics: Fix division by 0 issue in Shadows
*   Graphics: Fix for stalls when loading textures on single processor machines.
*   Graphics: Fix standalone player to render canvas even without a main camera.
*   Graphics: Fixed an issue when rendering to a render texture in deferred path with "Don't clear" or "Depth Only" clear flag.
*   Graphics: Fixed bug in ES 3 shader code generator that caused clipping problems in UI shaders
*   Graphics: Fixed fallback to Gamma color space rendering for projects that are configured to use linear rendering
*   Graphics: Fixed IMGUI asserts when doing supersized screenshot in linear color space.
*   Graphics: Fixed MSAA initialization on older devices which only support multisampled\_render\_to\_texture
*   Graphics: Fixed potential problem capturing frames in RenderDoc
*   Graphics: Fixed some cases of Graphics.DrawMesh with a matrix argument not getting the correct MaterialPropertyBlock values.
*   Graphics: Prevent spam of D3D11 warning messages setting resource names
*   Graphics: Stopped reflection merging into emissive from stomping over render target alpha with 1.0
*   Graphics: Transfer Emission property when switching from Legacy shaders to Standard UI: - If there is no room inside the Canvas for a Dropdown popup, mirror alignment only on axis where it exceeds the canvas, not always on both axes.- IL2CPP: Fixed a crash which occurred when script derived from a class that implemented ISerializationCallbackReceiver, was compiled into a DLL and no other script referenced any class that implemented ISerializationCallbackReceiver
*   IL2CPP: Fixed an issue where an empty project would display "The class with classID: 43 is not registered (see ClassIDs.h)" error at runtime
*   IMGUI: Fix possible deadlock when accessing GUIStyleState.background
*   IMGUI: Fix visually broken scrollbars in GUI.BeginScrollView() when the view rect is smaller than the position rect and scrollbars are forced enabled.
*   IMGUI: GUI.TextField taking a GUIStyle is now single line like its 3 sister functions.
*   IMGUI: Move the gamma assert to the Repaint phase.
*   IMGUI: Take font size in account even for null font when estimating content text size
*   IMGUI: When a button contains an image and text the layout logic does not work properly
*   IMGUI: When resizing a GUIWindow the render caching could create render artifacts and draw window content over scroll bars as it got resized.
*   iOS: Fixed when splash screen xib is deleted from project
*   iOS: Fixed duplicate AdSupport in plugin inspector
*   iOS: Fixed crash when not keeping reference to WWW object.
*   iOS: Fixed crash when switching keyboard between single and multi line modes while open.
*   iOS: Fixed command line build crash caused by trailing slash
*   iOS: Fixed system dynamic font support on iOS 9 where only the first font could be read from certain font collections and font substitutes, as identified by the OS, were not handled.
*   iOS: Worked around some plugins not supporting complex shell scripts within Xcode project
*   iOS/OSX: Fixed text rendering performance regression
*   LOD: Disabled animated LOD fading when 8 LODs are all used up.
*   LOD: Fixed "false" messages when selecting more than 3 LODs in the hierarchy window in the Editor.
*   LOD: Fixed "false" messages when setting a low Maximum LOD in quality settings.
*   LOD: Fixed crash if an empty LODGroup is selected as a tree prefab.
*   Mathf: Fixed issue with Mathf.FloorToInt and float cast to int not producing same results on x64 as on x86.
*   Mecanim: Added a delete confirmation message when deleting BlendTree in inspector
*   Mecanim: Added AvatarMask enum to AvatarMask
*   Mecanim: Allow StateMachineBehaviour function call even when Animator is disabled but updated manually by user
*   Mecanim: Changed error message when animator transitions cannot be previewed
*   Mecanim: Changed the significance of Euler vs Quaternion interpolation toggle in the Animation
*   Mecanim: Fixed a bug where keyframes' default values were not initialized, sometimes causing issues when creating Curves from Euler.
*   Mecanim: Fixed a bug where setting LocalEulerAngles curve via animation API would have made a clip that couldn't be scrubbed in the animation window
*   Mecanim: Fixed a case where Legacy Animation parameters affected the import of non-Legacy clips
*   Mecanim: Fixed a problem with state machines where Animation events on the first frame wouldn't fire in some cases
*   Mecanim: Fixed an inconsistent selection when switching to and from the mini layer tool
*   Mecanim: Fixed an invalid parameter "Blend" error in Direct blend tree inspectors
*   Mecanim: Fixed Animation Window not displaying the proper sampled value.
*   Mecanim: Fixed Animator tool resetting when pressing Home and End keys in parameter view
*   Mecanim: Fixed AvatarTool's unfolding of Avatar body part when selecting from UI
*   Mecanim: Fixed CollectDependency not working for AnimatorControllers
*   Mecanim: Fixed crash when OnStateEnter is called on the 1st frame.
*   Mecanim: Fixed deletion of body part using delete/backspace in the AvatarTool
*   Mecanim: Fixed empty AvatarMask for humanoid enabling addition transforms in previewer.
*   Mecanim: Fixed error message when deleting entry transition
*   Mecanim: Fixed IK to animated position in model a frame behind when using Optimize Game Objects
*   Mecanim: Fixed imported asset file showing active Apply state when nothing has changed
*   Mecanim: Fixed importer body mask not working.
*   Mecanim: Fixed Invalid keys frame in additional curves hanging Unity when users expand curve list in animation window
*   Mecanim: Fixed Model importer clip animation not updating correctly when set from a script.
*   Mecanim: Fixed numerical instabilities in transition preview. State name was not unique and was interfering with calculations.
*   Mecanim: Fixed overlapping BlendTree graph nodes
*   Mecanim: Fixed parameters not being evaluated when AnimatorController used in Playable
*   Mecanim: Fixed Rotation not being blended properly in some cases
*   Mecanim: Fixed rounding issue in the AnimationClipImporter start/stop frame
*   Mecanim: Fixed transition start time was not initialized correctly for played State.
*   Mecanim: Fixed Transition time slider getting offsetted.
*   Mecanim: Prevent crash when setting Animation.frameRate to 0
*   Mecanim: Prevent creation of invalid AnimationEvent time in AnimationClipImporter
*   Mecanim: Published BlendTree.minThreshold/maxThreshold API.
*   Mecanim: Removed Clamp Modes for ModelImporter additional curves
*   Mecanim: State Machine transitions that lead nowhere will now automatically transition to the layer's default state
*   MonoDevelop: Fixed "Debugger operation failed. Argument cannot be null" error
*   MonoDevelop: Fixed "The requested item has been unloaded" when enabling/disabling breakpoints
*   MonoDevelop: Fixed "The requested item has been unloaded" when evaluating enums.
*   MonoDevelop: Fixed crashes on OSX
*   MonoDevelop: Fixed issue with not being able to set breakpoint condition.
*   MonoDevelop: FIxed missing syntax highlighting for ShaderLab files
*   MonoDevelop: Fixed Mono.Debugger.Soft.ObjectCollectedException error message when setting a breakpoint
*   MonoDevelop: Fixed Mono.Debugger.Soft.ObjectCollectedException thrown when setting breakpoint
*   MonoDevelop: Fixed regression where MonoDevelop would report ERR\_UNLOADED when setting breakpoints.
*   MonoDevelop: Install GTK# when installing Unity Editor.
*   MonoDevelop: Removed "Show Error Reference" and "API Documentation" menu items that launch the documentation browser, which we do not include nor support.
*   Networking: Unity crashes when user stops the server and WebGL client connected
*   OpenGL legacy: Fixed editor picking when AA is enabled
*   OpenGL: Fixed texture memory usage reporting in profiler, was twice the actual size for most textures
*   Particles: Added new collision checkbox to allow users to work around 2 different bugs
*   Particles: Collision bug fixes
*   Particles: Culling bug fixes
*   Particles: Custom pivot point fixes
*   Particles: Fixed issue causing batched particles drawn after an object with negative scale to flip and become invisible.
*   Particles: Fixed sorting when using sort by distance.
*   Particles: Fixing threading race condition causing strange error message about particle counts
*   Particles: LateUpdate fix
*   Particles: Scaling fixes
*   Particles: Stretched particles now render even when they have zero speed
*   Physics2D: Ensure that animating a Joint2D property always updates the joint immediately.
*   Physics2D: Ensure that 'Infinity' cannot be specified for 2D collider offset.
*   Physics2D: Ensure that when recalculating contacts for an Effector2D, all relevant Rigidbody2D are woken.
*   Physics: Add note in Collider2D.Density tooltip that zero density has special meaning.
*   Physics: Added tooltips for JointLimits min and max values and freespin parameter
*   Physics: BoxCastAll, SphereCastAll, CapsuleCastAll now return zero RaycastHit.point for colliders overlapping with the sweep primitive at the initial position. Previously the result was undefined, which oftentimes matched the point returned by the previous sweep, but not necessarily so.
*   Physics: Ensure matched OnTriggerEnter/OnTriggerExit when changing collider size
*   Physics: Ensure that changing Collider2D.Density from script calculates the Rigidbody2D mass immediately.
*   Physics: Ensure that OnCollisionEnter2D is always called if a contact starts and ends during a single physics update.
*   Physics: Ensure that Physics2D OverlapAreaXXX checks are consistent with OverlapBoxXXX checks.
*   Physics: Ensure that when turning-on Rigidbody2D.AutoMass in the inspector, mass is immediately calculated.
*   Physics: Fix crashing when calling HingeJoint.useMotor or HingeJoint.useSpring on disabled a HingeJoint
*   Physics: Fix ignore settings not being applied to WheelCollider (when set with Physics.IgnoreCollision)
*   Physics: Fix NullReferenceException in the editor when dragging a Rigidbody2D in the scene whilst it is deleted.
*   Physics: Fix OnTriggerXXX not being called on Trigger Colliders that are children of GameObjects with a Rigidbody
*   Physics: Fix performance issue with unneeded error string formatting
*   Physics: Fix scaling of cars that had center of mass not at the Rigidbody's origin
*   Physics: Fixed a case where HingeJoint limits was not applied properly.
*   Physics: Fixed an axis-locking inconsistency in the HingeJoint when both min and max limits were set above 177 degrees, but still different.
*   Physics: Fixed cases where a ConfigurableJoint's JointDrive's spring stiffness and damping were not being set.
*   Physics: Fixed issues where PhysX SphereCasts would return an incorrect collision point for a scaled non-convex MeshCollider
*   Physics: Fixed PhysX wheels being created for inactive wheel colliders
*   Physics: When using AutoMass for Rigidbody2D, ensure that the mass is clamped correctly.
*   Placeholder text is no longer shown when UI.InputField has focus.
*   Plugins: Plugins located in StreamingAssets folder won't participate in the compilation.
*   Rich text now correctly word-wraps embedded images ( tags).
*   Scripting/Mono: Fixed Marshal.StructureToPtr crash when marshalling struct hierarchies on 64-bit.
*   Scripting: 'Editor' folders inside 'Plugins', 'Standard Assets' and 'Pro Standard Assets' no longer need to be at the root of those directories.
*   Scripting: Avoid Editor hang during close or script recompile if sockets are being used
*   Scripting: Do not set default System.Threading.SynchronizationContext.Current in .Net 2.0 Subset profile. Matches .Net 2.0 profile behavior.
*   Scripting: Fix crash when nested coroutine returns empty enumerator
*   Scripting: Fix enumerating Process.Modules and Threads in .Net 2.0 Subset profile.
*   Scripting: Fixed "Compile process is not finished yet" error
*   Scripting: Fixed crash in some scenarios when project has missing assembly references
*   Scripting: Fixed developer console not receiving log messages when using Application.logMessageReceived.
*   Scripting: LayerMask.GetMask() no longer ignores the Default layer.
*   Serialization: Fixed random float value corruption in the editor after multiple playing/stopping scene
*   Shaders: \_CameraDepthTexture is now preserved across calls to RenderWithShader()
*   Shaders: Correctly determine blend mode emitted by alpha:auto setting
*   Shaders: Fixed a possible runtime failure on iOS if an HLSL shader used a GLSL built-in function like 'mix'
*   Shaders: Fixed some errors translating complex HLSL shaders - large shader constant arrays, and nested structure load/stores
*   Shaders: Strength of glossy reflections is now independent from cubemap resolution
*   Shaders: Upgraded obsolete 'alpha:blend' to 'alpha:fade' in builtin shaders
*   Terrain: Fixed incorrect rendering when switching template material.
*   TextGenerator no longer occasional truncates the final character when using horizontal word-wrapping and vertical truncation.
*   Texture: Fix NPOT texture import size
*   Trailing spaces are now accounted for when aligning text.
*   TreeCreator: Fixed incorrect baked textures under Linear.
*   UI:Text Best Fit now works properly when a word does not fit within a single line.
*   UI:TextField no longer causes multiple errors text length exceeds 16383 characters.
*   UI: Allow '-' to be entered into InputField if the selected range encompases position 0
*   UI: Fix nested canvas not rendering when it is the only renderable child
*   UI: Fix occasional crash caused by vertex/index buffers being destroyed before a geometry job terminates.
*   UI: Fixed canvas objects not updating correctly when an object's transformation is modified
*   UI: Fixed caret being visible even when the Gameobject is disabled
*   UI: Fixed InputField selection highlight and caret no longer being visible.
*   UI: Fixed issue where CanvasRenderer would crash if an animation was playing when the canvas was removed
*   UI: Fixed issue where deleting a canvas while paused wouldn't update the visual state
*   UI: Fixed issue where removing a canvas wouldn't trigger its children to register to listen for events on the correct canvas
*   UI: Fixed memory leak where the mesh wouldn't dereference the mesh data when destroy was called
*   UI: Fixed multiline InputField throwing a ArgumentOutOfRange when trying to calculate the caret position
*   UI: Fixed Toggle component not updating when animated.
*   UI: Force Input caret to end of text on mobile device
*   UI: Image will not use the material texture if there is no sprite defined
*   UI: Tiled sprites with zero center will assume the center is stretched
*   UI: When appending to the InputField allow more characters than just space
*   Unity Ads: Upgraded SDK to 1.5.4 (also available on Asset Store). Fixes issues on iOS 9.1
*   UnityWebRequest: Some headers are missed in the response
*   VR: Fix crash when exiting play mode in the Editor
*   VR: Fix crash when running GearVR Applications
*   VR: Fix disabling ShowDeviceView preventing drawing to the game view with any camera
*   VR: Fix Fov in Scene/Game view of the Editor
*   VR: Fix HMD content failure after disconnect and reconnect
*   VR: Fix incorrect info and toggles while HMD was disconnected
*   VR: Fix Loss of Window focus crashes upon return
*   VR: Fix Plugin loading when creating a new VR Supported Project
*   VR: Fix regression crash when HMD was disconnected at application start
*   VR: Fix stereoMirrorMode right eye flicker
*   VR: Fix VRDevice.IsPresent always returning true
*   VR: Fix wrong FOV on entering play mode
*   WebGL: Fix an issue which could cause various stripping-related crashes as a consequence
*   WebGL: Fix Application.dataPath
*   WebGL: Fix AudioClip.Create on Safari
*   WebGL: Fix backbuffer state if RenderTexture is set from user code.
*   WebGL: Fix crash related to stripping ParticleSystem class
*   WebGL: Fix crash when trying to use WWW.LoadFromCacheOrDownload if IndexedDB is not available.
*   WebGL: Fix crash when using Caching.Authorize
*   WebGL: Fix cursor images not rendering correctly
*   WebGL: Fix doppler effect being used on audio sources with spatial blend set to 2D
*   WebGL: Fix Firefox crashing on closing the page
*   WebGL: Fix GUI.TextArea issue caused by TextEditor stripping
*   WebGL: Fix heavy memory consumption when downloading asset bundles using WWW.LoadFromCacheOrDownload
*   WebGL: Fix importing wav files with floating point samples
*   WebGL: Fix Input.touches being flipped along the y-axis.
*   WebGL: Fix jerky mouse delta values
*   WebGL: Fix rescaling of default html template
*   WebGL: Fix Return/Enter keypress on Firefox
*   WebGL: Fix RightAlt key when used as AltGr to access special keyboard layouts
*   WebGL: Fix unnecessary warnings about rendering to mipmaps
*   WebGL: Fix WWW class response contents when status code is not 200
*   WebGL: Fixed GL\_INVALID\_OPERATION error in log caused by incorrect use of DrawBuffers
*   WebGL: InputString: fix truncation of UTF16 characters
*   WebGL: Make Application.targetFrameRate work
*   WebGL: Make AudioClip.SetData work
*   WebGL: Make Sound::getLength return the correct result
*   WebGL: Make touch input work with UnityEngine.UI.
*   WebGL: WebGL should now use "closer to desktop" Shader features: Standard Shader HQ BRDF, support for box-projected probes and probes blending.
*   Windows Editor: Fixed D3D9 crash when locking/unlocking windows, due to a DeviceLost event not being handled correctly
*   Windows Phone 10: fix touch screen keyboard
*   Windows Standalone: Configuration banner image will be properly scaled on operating systems like "Windows 7 Home Extended", etc.
*   Windows Standalone: Fixed a bug where sometimes graphics quality combo box was empty.
*   Windows Standalone: In startup screen available resolutions list is populated according to the selected monitor
*   Windows Standalone: Screen.sleepTimeout will work correctly.
*   Windows Standalone: Switching from windowed to fullscreen mode will fullscreen player in the same monitor where it was in the windowed mode
*   Windows Store Apps: add support for new UWP capabilities and their population to manifest
*   Windows Store Apps: add UWP specific icon support and fix manifest creation
*   Windows Store Apps: Fix AssemblyConverter failure for Array methods
*   Windows Store Apps: Fix occasional rendering freeze when leaving and coming back in landscape mode
*   Windows Store Apps: make explicit call UnityPause(1) to pause player until explicitly unpaused via UnityPause(0)
*   Windows Store Apps: make Input.gyro available if either OrientationSensor or Gyrometer is available
*   Windows Store Apps: setup initial orientations from Player Settings
*   Windows Store: building project with IL2CPP scripting backend no longer fails.
*   Windows Store: Fixed a memory leak which reduced memory usage by around 4 to 8 MB.
*   Windows Store: Fixed an issue which caused functions RunningOnUIThread and RunningOnAppThread in UnityEngine.WSA.Application to throw exceptions if called on non-main thread.
*   Windows Store: Fixed an issue which made UWP class libraries throw FileNotFoundException when invoking into native WinRT components.
*   XboxOne/IL2CPP: Correct metadata loading on startup.