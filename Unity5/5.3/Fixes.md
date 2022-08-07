# Unity 5.3
https://unity3d.com/unity/whats-new/unity-5.3

## Fixes

<ul>
<li>2D: Fix memory leak when using Sprite object field in custom inspector</li>
<li>Android: Add support for stencil buffer in RenderTextures on Tegra 3</li>
<li>Android: Android 6.0 - Ask for any dangerous permission on startup</li>
<li>Android: AndroidJava - Fixed recursion in AndroidJavaProxy</li>
<li>Android: Buildpipe - don't open file dialogs when in batch mode</li>
<li>Android: Buildpipe - Fixed an issue where projects created on Mac wouldn't build on Windows</li>
<li>Android: Buildpipe - Fixed an issue where the Editor would hang if in batch mode without SDK, NDK and JDK properly configured</li>
<li>Android: Buildpipe - Fixed IndexOutOfRangeException thrown on plugin package collisions</li>
<li>Android: Fix for missing SpeedTree leaves when using and 'best' quality wind zones on Adreno 3xx with OpenGL ES 3.0</li>
<li>Android: Fix for physics performance spikes on ARM big.LITTLE devices</li>
<li>Android: Fixed a problem where Plugins/Android/res wasn't bundled with the application</li>
<li>Android: Fixed an issue where a problematic EGL configuration was picked up on some Samsung devices</li>
<li>Android: Fixed an issue where passing large JNI arrays would cause a local reference table overflow</li>
<li>Android: Fixed an issue where PlayerPrefs with keys and values containing line breaks would break</li>
<li>Android: Fixed an issue where the application would crash if you sent emoji unicode characters to the OnScreenKeybaord</li>
<li>Android: Fixed crash affecting some PowerVR 544 devices</li>
<li>Android: Fixed crash in ASTC encoder</li>
<li>Android: Fixed crash in decompression of PVRTC textures on non-PVR devices</li>
<li>Android: Fixed INTERNET permission on Android even if there are no network calls in the scripts</li>
<li>Android: Fixed MSAA on newer ARM Mali devices like Samsung Galaxy S6</li>
<li>Android: Fixed MSAA RenderTextures on Tegra4 and K1 when using OpenGL ES 2.0</li>
<li>Android: Fixed non-working textures on some Tegra 3 and Tegra 4 devices</li>
<li>Android: Fixed OBB deployment on Android 6.0 and some older devices</li>
<li>Android: Fixed OnApplicationPause() event on app start</li>
<li>Android: Fixed reported texture size in profiler for formats that are decompressed during upload</li>
<li>Android: IL2CPP - Fixed compilation on paths with spaces</li>
<li>Android: Manual updates of the SDK should now take effect when prompted for an update in the Editor</li>
<li>Android: Removed some egl errors from the log when probing for GLES API level</li>
<li>Android: Removed the 'soft' cursor</li>
<li>Android: SoftInput - Fixed hint color</li>
<li>Android: Stripping - don't strip AssetBundle class or it removes LoadAssetAsync</li>
<li>Android: Support for galaxy camera volume buttons (zoom in/out)</li>
<li>Animation: Fixed a case where non-resampled curves would have overlapping keyframes</li>
<li>Animation: Fixed animation of material properties in the animation window.</li>
<li>Animation: Fixed animation window still recording when scene is saved.</li>
<li>API Updater: Fix crashing when checking for obsolete API in assemblies referencing unity extensions</li>
<li>API Updater: Fixed handling of multiple "defines" / references in a single argument in response files</li>
<li>Asset Importing: Fix main thread assert when releasing MonoScript object</li>
<li>Asset Loading: Allow extension dlls to be imported outside of project folder</li>
<li>AssetBundle: Fix the issue that the sprite atlas has been stored twice in AssetBundles.</li>
<li>Assets Management: All assets located inside the Resources folder are now reported in the summary area of the editor's output log.</li>
<li>BestFit min/max sizes are now clamped so that always include the starting/default font size. This guarantees that minSize &lt;= startingSize &lt;= maxSize.</li>
<li>Build Pipeline: Fixed warning message "Failed to add the asset file size for <strong>filename</strong>".</li>
<li>CacheServer: Add Cache Server version in terminal</li>
<li>CacheServer: Fix server crashes on command 'nc -zv'</li>
<li>Canvas is no longer has an incorrect x offset when the viewport rect is anything other than (0, 0, 1, 1) on D3D9, XBOX360, and PSP2.</li>
<li>Caret and selection highlight now draw with correct y position and height in UI.InputField for all formats and line spacings.</li>
<li>Copying to the clipboard is now disabled for UI.InputField with ContentType of Password.</li>
<li>Core: When building a player Editor.log displayed incorrect file size if project had Resource folder with textures in it</li>
<li>Crunch texture compression: Fix errors when baking light maps on scenes with crunched textures</li>
<li>Crunch texture compression: Fix memory corruption crash when using crunched textures as Cubemaps</li>
<li>Crunch texture compression: Fix using crunched textures on terrains</li>
<li>Disable expanding the navmesh clipping hull beyond the collected list of affected polygons - could cause t-junctions.</li>
<li>DisplayProgressBar replaces forward slash with a backslash</li>
<li>Editor: Fixed Handles.DrawDottedLines not working when intersecting near plane. Improved performance of the function as well.</li>
<li>Editor: Fix for NullReferenceExceptions while dropping prefab in the scene view</li>
<li>Editor Fix Shift-Delete in rename box deleting asset in scene.</li>
<li>Editor Fixed a case of new lines in labels when the display name comes from an array of strings.</li>
<li>Editor slowdown in Project window with Unity 5</li>
<li>Editor Use the correct image for Dark skin's horizontal scrollbar left button</li>
<li>Editor: Add drop target rendering for icon view in Project Browser when hovering over a drop target</li>
<li>Editor: Added a printed warning to the gameview if there is no fullscreen camera present</li>
<li>Editor: Assert Import dialog will correctly appear in the taskbar on Windows, previously you needed to click on the dialog for it to appear in the taskbar or wait until the import is finished.</li>
<li>Editor: Asset importer now skips assets and res folders inside Assets/Plugins/Android.</li>
<li>Editor: Better UI for ShaderVariantCollection "add variant" functionality.</li>
<li>Editor: EditorWindow OnClose() and OnDestroy() will now be called when the Unity Editor is closed.</li>
<li>Editor: Fix ArgumentOutOfRangeException when attempting to delete last character of TextField with length limit</li>
<li>Editor: Fix crash on Editor quit while the profiler is enabled</li>
<li>Editor: Fix for GUI methods in Update crashes the editor</li>
<li>Editor: Fix memory thrashing when Dragging and Dropping between panels, when the dragged object had a CustomEditor with no Preview.</li>
<li>Editor: Fix mismatched layout group in MeshRenderer editor</li>
<li>Editor: Fix project browser searching so 't:Object': also returns ScriptableObjects</li>
<li>Editor: Fix searching for labels with characters in front of the 'l:' syntax in the project browser</li>
<li>Editor: Fix so searching for special symbols (like @) works in project browser</li>
<li>Editor: Fix texture preview not showing mip previews for RenderTextures.</li>
<li>Editor: Fix that the search results in Project view is not refreshing when changing labels</li>
<li>Editor: Fixed "Ctrl" click on object selects another object in scene view</li>
<li>Editor: Fixed bug when opening new project throws "Moving file failed" dialog on Mac</li>
<li>Editor: Fixed changing a GameObject's icon failing when changing it for the first time.</li>
<li>Editor: Fixed error message when attempting to add a given component to the same game object more than once.</li>
<li>Editor: Fixed exception being thrown when multiple assets were selected and one or more contained ScriptableObjects with missing script references.</li>
<li>Editor: Fixed inspector preview bug when UI RawImage had negative UV values.</li>
<li>Editor: Fixed issue with unnecessary whitespace being added to generated MonoDevelop/VS solution (.sln) files after each update.</li>
<li>Editor: Fixed mispositioned arrows in the inspector.</li>
<li>Editor: Fixed rare crash when a component is missing a script reference</li>
<li>Editor: Fixes Nullref when trying to maximize a view through the Context menu.</li>
<li>Editor: Launch unity through command line with the –buildTarget switch and the scripting defines will not be set properly.</li>
<li>Editor: Multi selecting GameObjects should be as fast as it was in 4.6</li>
<li>Editor: Multiple object renaming in the inspector does not work in some conditions.</li>
<li>Editor: Multiselecting textures with different override settings now shows the correct "-" symbol.</li>
<li>Editor: Prefab properties will be preserved in case the Editor shuts down unexpectedly.</li>
<li>Editor: Prefab will be updated correctly in the Project View when Apply or GameObject/Apply Changes to Prefab is selected and Cache Server is enabled.</li>
<li>Editor: Removed MonoDevelop Solution Properties checkbox from External Tools. Unity no longer writes MonoDevelop code formatting settings into MonoDevelopSolutionProperties in .sln file.</li>
<li>Editor: Show a note in legacy cubemap inspector about destructive operations</li>
<li>Editor: Show a note next to texture aniso slider when it won't have effect due to global quality setting</li>
<li>Editor: Show import warning when manually selected texture compression format was changed due to unsupported platform</li>
<li>Editor: The camera culling mask would display "Mixed..." incorrectly in various situation. Now correctly reflects render layer state.</li>
<li>Editor: The current control with focus now correctly resets to none between Play runs of the open scene.</li>
<li>Ensure that when refreshing the shown value of a Dropdown while there are no options at all, the Dropdown value becomes blank rather than keeping showing a previously valid value.</li>
<li>Fix for regression - agent was reporting no path when moving over OffMeshLink.</li>
<li>Fix for regression - navmesh carving would sometimes collapse degenerate triangles in a way that could affect other polygons.</li>
<li>Fix for shadow-casting light occlusion issues - disappearing realtime lights</li>
<li>Fix issue where agent’s area cost settings were overwritten with global cost settings - when doing NavMeshAgent.CalculatePath.</li>
<li>Fix Mono Assembly stripping</li>
<li>Fixed an issue where opening the editor with a Preview window in the layout would cause the inspector tab icon to disappear</li>
<li>Fixed ArgumentOutOfRange being thrown when InputField Text component clips all text (e.g. when font is too large).</li>
<li>Fixed GUILayout.EndHorizontal() throwing an exception after calling BuildPipeline.BuildAssetBundles</li>
<li>Fixed incorrect behavior for GetHasMoved in UI.CanvasRenderer.</li>
<li>Fixed incorrect kerning calculations for scaled text.</li>
<li>Fixed incorrect line spacing when using rich text and  tag to set font size less than the value set in the Text property.</li>
<li>Fixed incorrect pixel perfect rounding on high DPI (retina) displays.</li>
<li>Fixed incorrect vertical positioning of wrapped word when word-wrapping text with pixel perfect rounding.</li>
<li>Fixed InputField selection highlight and caret no longer being visible.</li>
<li>Fixed issue that caused FontUpdateTracker to add an additional RebuildForFont handler whenever a Text component was enabled using a font with no other active Text components using that font.</li>
<li>Fixed issue where objects lit by light probes appear brighter than static objects with same material in gamma mode. See upgrade guide for details.</li>
<li>Fixed issue with all text not displaying correctly in UI.InputField.</li>
<li>Fixed problem where characters would sometimes get incorrect kerning information.</li>
<li>Frame Debugger: Fixed shader blend/depth/raster state settings sometimes not displayed correctly.</li>
<li>GetComponent, in cases where T is an interface, will no longer incorrectly skip matching non monobehaviours</li>
<li>GI: Brought back the separate Emission(Lightmapper) component in LegacyShaders/Self-Illumin that went missing in Unity 5.0</li>
<li>GI: Fix crash when exiting the editor while building lighting.</li>
<li>GI: Fix memory leak eventually causing a crash when baking lightmaps using bad UVs.</li>
<li>GI: Fix realtime GI errors about loading hashed files when opening different scenes.</li>
<li>GI: Fixed a crash when switching scenes when at least one of them was using realtime GI and light probes.</li>
<li>GI: Fixed additive loading of static lightmaps on terrains.</li>
<li>GI: Fixed Baking Progress Bar hanging with "Bake paused in play mode.</li>
<li>GI: Fixed clustering scene view causing loading bars to pop up all the time during bake when clustering files were reloaded.</li>
<li>GI: Fixed crash when calling SetEmissive for a system with no radiosity data available.</li>
<li>GI: Fixed crash when marking object from an FBX file containing 3DSMax Camera Nodes to be Lightmap Static.</li>
<li>GI: Fixed issue where Emission in Legacy Self Illum Diffuse was clamped to 8.</li>
<li>GI: Fixed light hashing always done even when GI is off, causing performance slowdown.</li>
<li>GI: Fixed light probes in player builds.</li>
<li>GI: Fixed orientation of skybox used for generating ambient probe (it was wrong on Windows and Linux).</li>
<li>GI: Now terrain heightmap painting can correctly trigger the baking of GI on that part of the terrain and the editor won't crash when a terrain is duplicated.</li>
<li>GI: Removed editor log spamming: Error: GetProbeInterpolants - probe sets that aren't regular grids require...</li>
<li>Graphics: Fix crash trying to set shader name on shader that failed to compile</li>
<li>Graphics: Fix crash when calling Texture.Compress for large textures</li>
<li>Graphics: Fix division by 0 issue in Shadows</li>
<li>Graphics: Fix for stalls when loading textures on single processor machines.</li>
<li>Graphics: Fix standalone player to render canvas even without a main camera.</li>
<li>Graphics: Fixed an issue when rendering to a render texture in deferred path with "Don't clear" or "Depth Only" clear flag.</li>
<li>Graphics: Fixed bug in ES 3 shader code generator that caused clipping problems in UI shaders</li>
<li>Graphics: Fixed fallback to Gamma color space rendering for projects that are configured to use linear rendering</li>
<li>Graphics: Fixed IMGUI asserts when doing supersized screenshot in linear color space.</li>
<li>Graphics: Fixed MSAA initialization on older devices which only support multisampled_render_to_texture</li>
<li>Graphics: Fixed potential problem capturing frames in RenderDoc</li>
<li>Graphics: Fixed some cases of Graphics.DrawMesh with a matrix argument not getting the correct MaterialPropertyBlock values.</li>
<li>Graphics: Prevent spam of D3D11 warning messages setting resource names</li>
<li>Graphics: Stopped reflection merging into emissive from stomping over render target alpha with 1.0</li>
<li>Graphics: Transfer Emission property when switching from Legacy shaders to Standard UI: - If there is no room inside the Canvas for a Dropdown popup, mirror alignment only on axis where it exceeds the canvas, not always on both axes.- IL2CPP: Fixed a crash which occurred when script derived from a class that implemented ISerializationCallbackReceiver, was compiled into a DLL and no other script referenced any class that implemented ISerializationCallbackReceiver</li>
<li>IL2CPP: Fixed an issue where an empty project would display "The class with classID: 43 is not registered (see ClassIDs.h)" error at runtime</li>
<li>IMGUI: Fix possible deadlock when accessing GUIStyleState.background</li>
<li>IMGUI: Fix visually broken scrollbars in GUI.BeginScrollView() when the view rect is smaller than the position rect and scrollbars are forced enabled.</li>
<li>IMGUI: GUI.TextField taking a GUIStyle is now single line like its 3 sister functions.</li>
<li>IMGUI: Move the gamma assert to the Repaint phase.</li>
<li>IMGUI: Take font size in account even for null font when estimating content text size</li>
<li>IMGUI: When a button contains an image and text the layout logic does not work properly</li>
<li>IMGUI: When resizing a GUIWindow the render caching could create render artifacts and draw window content over scroll bars as it got resized.</li>
<li>iOS: Fixed when splash screen xib is deleted from project</li>
<li>iOS: Fixed duplicate AdSupport in plugin inspector</li>
<li>iOS: Fixed crash when not keeping reference to WWW object.</li>
<li>iOS: Fixed crash when switching keyboard between single and multi line modes while open.</li>
<li>iOS: Fixed command line build crash caused by trailing slash</li>
<li>iOS: Fixed system dynamic font support on iOS 9 where only the first font could be read from certain font collections and font substitutes, as identified by the OS, were not handled.</li>
<li>iOS: Worked around some plugins not supporting complex shell scripts within Xcode project</li>
<li>iOS/OSX: Fixed text rendering performance regression</li>
<li>LOD: Disabled animated LOD fading when 8 LODs are all used up.</li>
<li>LOD: Fixed "false" messages when selecting more than 3 LODs in the hierarchy window in the Editor.</li>
<li>LOD: Fixed "false" messages when setting a low Maximum LOD in quality settings.</li>
<li>LOD: Fixed crash if an empty LODGroup is selected as a tree prefab.</li>
<li>Mathf: Fixed issue with Mathf.FloorToInt and float cast to int not producing same results on x64 as on x86.</li>
<li>Mecanim: Added a delete confirmation message when deleting BlendTree in inspector</li>
<li>Mecanim: Added AvatarMask enum to AvatarMask</li>
<li>Mecanim: Allow StateMachineBehaviour function call even when Animator is disabled but updated manually by user</li>
<li>Mecanim: Changed error message when animator transitions cannot be previewed</li>
<li>Mecanim: Changed the significance of Euler vs Quaternion interpolation toggle in the Animation</li>
<li>Mecanim: Fixed a bug where keyframes' default values were not initialized, sometimes causing issues when creating Curves from Euler.</li>
<li>Mecanim: Fixed a bug where setting LocalEulerAngles curve via animation API would have made a clip that couldn't be scrubbed in the animation window</li>
<li>Mecanim: Fixed a case where Legacy Animation parameters affected the import of non-Legacy clips</li>
<li>Mecanim: Fixed a problem with state machines where Animation events on the first frame wouldn't fire in some cases</li>
<li>Mecanim: Fixed an inconsistent selection when switching to and from the mini layer tool</li>
<li>Mecanim: Fixed an invalid parameter "Blend" error in Direct blend tree inspectors</li>
<li>Mecanim: Fixed Animation Window not displaying the proper sampled value.</li>
<li>Mecanim: Fixed Animator tool resetting when pressing Home and End keys in parameter view</li>
<li>Mecanim: Fixed AvatarTool's unfolding of Avatar body part when selecting from UI</li>
<li>Mecanim: Fixed CollectDependency not working for AnimatorControllers</li>
<li>Mecanim: Fixed crash when OnStateEnter is called on the 1st frame.</li>
<li>Mecanim: Fixed deletion of body part using delete/backspace in the AvatarTool</li>
<li>Mecanim: Fixed empty AvatarMask for humanoid enabling addition transforms in previewer.</li>
<li>Mecanim: Fixed error message when deleting entry transition</li>
<li>Mecanim: Fixed IK to animated position in model a frame behind when using Optimize Game Objects</li>
<li>Mecanim: Fixed imported asset file showing active Apply state when nothing has changed</li>
<li>Mecanim: Fixed importer body mask not working.</li>
<li>Mecanim: Fixed Invalid keys frame in additional curves hanging Unity when users expand curve list in animation window</li>
<li>Mecanim: Fixed Model importer clip animation not updating correctly when set from a script.</li>
<li>Mecanim: Fixed numerical instabilities in transition preview. State name was not unique and was interfering with calculations.</li>
<li>Mecanim: Fixed overlapping BlendTree graph nodes</li>
<li>Mecanim: Fixed parameters not being evaluated when AnimatorController used in Playable</li>
<li>Mecanim: Fixed Rotation not being blended properly in some cases</li>
<li>Mecanim: Fixed rounding issue in the AnimationClipImporter start/stop frame</li>
<li>Mecanim: Fixed transition start time was not initialized correctly for played State.</li>
<li>Mecanim: Fixed Transition time slider getting offsetted.</li>
<li>Mecanim: Prevent crash when setting Animation.frameRate to 0</li>
<li>Mecanim: Prevent creation of invalid AnimationEvent time in AnimationClipImporter</li>
<li>Mecanim: Published BlendTree.minThreshold/maxThreshold API.</li>
<li>Mecanim: Removed Clamp Modes for ModelImporter additional curves</li>
<li>Mecanim: State Machine transitions that lead nowhere will now automatically transition to the layer's default state</li>
<li>MonoDevelop: Fixed "Debugger operation failed. Argument cannot be null" error</li>
<li>MonoDevelop: Fixed "The requested item has been unloaded" when enabling/disabling breakpoints</li>
<li>MonoDevelop: Fixed "The requested item has been unloaded" when evaluating enums.</li>
<li>MonoDevelop: Fixed crashes on OSX</li>
<li>MonoDevelop: Fixed issue with not being able to set breakpoint condition.</li>
<li>MonoDevelop: FIxed missing syntax highlighting for ShaderLab files</li>
<li>MonoDevelop: Fixed Mono.Debugger.Soft.ObjectCollectedException error message when setting a breakpoint</li>
<li>MonoDevelop: Fixed Mono.Debugger.Soft.ObjectCollectedException thrown when setting breakpoint</li>
<li>MonoDevelop: Fixed regression where MonoDevelop would report ERR_UNLOADED when setting breakpoints.</li>
<li>MonoDevelop: Install GTK# when installing Unity Editor.</li>
<li>MonoDevelop: Removed "Show Error Reference" and "API Documentation" menu items that launch the documentation browser, which we do not include nor support.</li>
<li>Networking: Unity crashes when user stops the server and WebGL client connected</li>
<li>OpenGL legacy: Fixed editor picking when AA is enabled</li>
<li>OpenGL: Fixed texture memory usage reporting in profiler, was twice the actual size for most textures</li>
<li>Particles: Added new collision checkbox to allow users to work around 2 different bugs</li>
<li>Particles: Collision bug fixes</li>
<li>Particles: Culling bug fixes</li>
<li>Particles: Custom pivot point fixes</li>
<li>Particles: Fixed issue causing batched particles drawn after an object with negative scale to flip and become invisible.</li>
<li>Particles: Fixed sorting when using sort by distance.</li>
<li>Particles: Fixing threading race condition causing strange error message about particle counts</li>
<li>Particles: LateUpdate fix</li>
<li>Particles: Scaling fixes</li>
<li>Particles: Stretched particles now render even when they have zero speed</li>
<li>Physics2D: Ensure that animating a Joint2D property always updates the joint immediately.</li>
<li>Physics2D: Ensure that 'Infinity' cannot be specified for 2D collider offset.</li>
<li>Physics2D: Ensure that when recalculating contacts for an Effector2D, all relevant Rigidbody2D are woken.</li>
<li>Physics: Add note in Collider2D.Density tooltip that zero density has special meaning.</li>
<li>Physics: Added tooltips for JointLimits min and max values and freespin parameter</li>
<li>Physics: BoxCastAll, SphereCastAll, CapsuleCastAll now return zero RaycastHit.point for colliders overlapping with the sweep primitive at the initial position. Previously the result was undefined, which oftentimes matched the point returned by the previous sweep, but not necessarily so.</li>
<li>Physics: Ensure matched OnTriggerEnter/OnTriggerExit when changing collider size</li>
<li>Physics: Ensure that changing Collider2D.Density from script calculates the Rigidbody2D mass immediately.</li>
<li>Physics: Ensure that OnCollisionEnter2D is always called if a contact starts and ends during a single physics update.</li>
<li>Physics: Ensure that Physics2D OverlapAreaXXX checks are consistent with OverlapBoxXXX checks.</li>
<li>Physics: Ensure that when turning-on Rigidbody2D.AutoMass in the inspector, mass is immediately calculated.</li>
<li>Physics: Fix crashing when calling HingeJoint.useMotor or HingeJoint.useSpring on disabled a HingeJoint</li>
<li>Physics: Fix ignore settings not being applied to WheelCollider (when set with Physics.IgnoreCollision)</li>
<li>Physics: Fix NullReferenceException in the editor when dragging a Rigidbody2D in the scene whilst it is deleted.</li>
<li>Physics: Fix OnTriggerXXX not being called on Trigger Colliders that are children of GameObjects with a Rigidbody</li>
<li>Physics: Fix performance issue with unneeded error string formatting</li>
<li>Physics: Fix scaling of cars that had center of mass not at the Rigidbody's origin</li>
<li>Physics: Fixed a case where HingeJoint limits was not applied properly.</li>
<li>Physics: Fixed an axis-locking inconsistency in the HingeJoint when both min and max limits were set above 177 degrees, but still different.</li>
<li>Physics: Fixed cases where a ConfigurableJoint's JointDrive's spring stiffness and damping were not being set.</li>
<li>Physics: Fixed issues where PhysX SphereCasts would return an incorrect collision point for a scaled non-convex MeshCollider</li>
<li>Physics: Fixed PhysX wheels being created for inactive wheel colliders</li>
<li>Physics: When using AutoMass for Rigidbody2D, ensure that the mass is clamped correctly.</li>
<li>Placeholder text is no longer shown when UI.InputField has focus.</li>
<li>Plugins: Plugins located in StreamingAssets folder won't participate in the compilation.</li>
<li>Rich text now correctly word-wraps embedded images ( tags).</li>
<li>Scripting/Mono: Fixed Marshal.StructureToPtr crash when marshalling struct hierarchies on 64-bit.</li>
<li>Scripting: 'Editor' folders inside 'Plugins', 'Standard Assets' and 'Pro Standard Assets' no longer need to be at the root of those directories.</li>
<li>Scripting: Avoid Editor hang during close or script recompile if sockets are being used</li>
<li>Scripting: Do not set default System.Threading.SynchronizationContext.Current in .Net 2.0 Subset profile. Matches .Net 2.0 profile behavior.</li>
<li>Scripting: Fix crash when nested coroutine returns empty enumerator</li>
<li>Scripting: Fix enumerating Process.Modules and Threads in .Net 2.0 Subset profile.</li>
<li>Scripting: Fixed "Compile process is not finished yet" error</li>
<li>Scripting: Fixed crash in some scenarios when project has missing assembly references</li>
<li>Scripting: Fixed developer console not receiving log messages when using Application.logMessageReceived.</li>
<li>Scripting: LayerMask.GetMask() no longer ignores the Default layer.</li>
<li>Serialization: Fixed random float value corruption in the editor after multiple playing/stopping scene</li>
<li>Shaders: _CameraDepthTexture is now preserved across calls to RenderWithShader()</li>
<li>Shaders: Correctly determine blend mode emitted by alpha:auto setting</li>
<li>Shaders: Fixed a possible runtime failure on iOS if an HLSL shader used a GLSL built-in function like 'mix'</li>
<li>Shaders: Fixed some errors translating complex HLSL shaders - large shader constant arrays, and nested structure load/stores</li>
<li>Shaders: Strength of glossy reflections is now independent from cubemap resolution</li>
<li>Shaders: Upgraded obsolete 'alpha:blend' to 'alpha:fade' in builtin shaders</li>
<li>Terrain: Fixed incorrect rendering when switching template material.</li>
<li>TextGenerator no longer occasional truncates the final character when using horizontal word-wrapping and vertical truncation.</li>
<li>Texture: Fix NPOT texture import size</li>
<li>Trailing spaces are now accounted for when aligning text.</li>
<li>TreeCreator: Fixed incorrect baked textures under Linear.</li>
<li>UI:Text Best Fit now works properly when a word does not fit within a single line.</li>
<li>UI:TextField no longer causes multiple errors text length exceeds 16383 characters.</li>
<li>UI: Allow '-' to be entered into InputField if the selected range encompases position 0</li>
<li>UI: Fix nested canvas not rendering when it is the only renderable child</li>
<li>UI: Fix occasional crash caused by vertex/index buffers being destroyed before a geometry job terminates.</li>
<li>UI: Fixed canvas objects not updating correctly when an object's transformation is modified</li>
<li>UI: Fixed caret being visible even when the Gameobject is disabled</li>
<li>UI: Fixed InputField selection highlight and caret no longer being visible.</li>
<li>UI: Fixed issue where CanvasRenderer would crash if an animation was playing when the canvas was removed</li>
<li>UI: Fixed issue where deleting a canvas while paused wouldn't update the visual state</li>
<li>UI: Fixed issue where removing a canvas wouldn't trigger its children to register to listen for events on the correct canvas</li>
<li>UI: Fixed memory leak where the mesh wouldn't dereference the mesh data when destroy was called</li>
<li>UI: Fixed multiline InputField throwing a ArgumentOutOfRange when trying to calculate the caret position</li>
<li>UI: Fixed Toggle component not updating when animated.</li>
<li>UI: Force Input caret to end of text on mobile device</li>
<li>UI: Image will not use the material texture if there is no sprite defined</li>
<li>UI: Tiled sprites with zero center will assume the center is stretched</li>
<li>UI: When appending to the InputField allow more characters than just space</li>
<li>Unity Ads: Upgraded SDK to 1.5.4 (also available on Asset Store). Fixes issues on iOS 9.1</li>
<li>UnityWebRequest: Some headers are missed in the response</li>
<li>VR: Fix crash when exiting play mode in the Editor</li>
<li>VR: Fix crash when running GearVR Applications</li>
<li>VR: Fix disabling ShowDeviceView preventing drawing to the game view with any camera</li>
<li>VR: Fix Fov in Scene/Game view of the Editor</li>
<li>VR: Fix HMD content failure after disconnect and reconnect</li>
<li>VR: Fix incorrect info and toggles while HMD was disconnected</li>
<li>VR: Fix Loss of Window focus crashes upon return</li>
<li>VR: Fix Plugin loading when creating a new VR Supported Project</li>
<li>VR: Fix regression crash when HMD was disconnected at application start</li>
<li>VR: Fix stereoMirrorMode right eye flicker</li>
<li>VR: Fix VRDevice.IsPresent always returning true</li>
<li>VR: Fix wrong FOV on entering play mode</li>
<li>WebGL: Fix an issue which could cause various stripping-related crashes as a consequence</li>
<li>WebGL: Fix Application.dataPath</li>
<li>WebGL: Fix AudioClip.Create on Safari</li>
<li>WebGL: Fix backbuffer state if RenderTexture is set from user code.</li>
<li>WebGL: Fix crash related to stripping ParticleSystem class</li>
<li>WebGL: Fix crash when trying to use WWW.LoadFromCacheOrDownload if IndexedDB is not available.</li>
<li>WebGL: Fix crash when using Caching.Authorize</li>
<li>WebGL: Fix cursor images not rendering correctly</li>
<li>WebGL: Fix doppler effect being used on audio sources with spatial blend set to 2D</li>
<li>WebGL: Fix Firefox crashing on closing the page</li>
<li>WebGL: Fix GUI.TextArea issue caused by TextEditor stripping</li>
<li>WebGL: Fix heavy memory consumption when downloading asset bundles using WWW.LoadFromCacheOrDownload</li>
<li>WebGL: Fix importing wav files with floating point samples</li>
<li>WebGL: Fix Input.touches being flipped along the y-axis.</li>
<li>WebGL: Fix jerky mouse delta values</li>
<li>WebGL: Fix rescaling of default html template</li>
<li>WebGL: Fix Return/Enter keypress on Firefox</li>
<li>WebGL: Fix RightAlt key when used as AltGr to access special keyboard layouts</li>
<li>WebGL: Fix unnecessary warnings about rendering to mipmaps</li>
<li>WebGL: Fix WWW class response contents when status code is not 200</li>
<li>WebGL: Fixed GL_INVALID_OPERATION error in log caused by incorrect use of DrawBuffers</li>
<li>WebGL: InputString: fix truncation of UTF16 characters</li>
<li>WebGL: Make Application.targetFrameRate work</li>
<li>WebGL: Make AudioClip.SetData work</li>
<li>WebGL: Make Sound::getLength return the correct result</li>
<li>WebGL: Make touch input work with UnityEngine.UI.</li>
<li>WebGL: WebGL should now use "closer to desktop" Shader features: Standard Shader HQ BRDF, support for box-projected probes and probes blending.</li>
<li>Windows Editor: Fixed D3D9 crash when locking/unlocking windows, due to a DeviceLost event not being handled correctly</li>
<li>Windows Phone 10: fix touch screen keyboard</li>
<li>Windows Standalone: Configuration banner image will be properly scaled on operating systems like "Windows 7 Home Extended", etc.</li>
<li>Windows Standalone: Fixed a bug where sometimes graphics quality combo box was empty.</li>
<li>Windows Standalone: In startup screen available resolutions list is populated according to the selected monitor</li>
<li>Windows Standalone: Screen.sleepTimeout will work correctly.</li>
<li>Windows Standalone: Switching from windowed to fullscreen mode will fullscreen player in the same monitor where it was in the windowed mode</li>
<li>Windows Store Apps: add support for new UWP capabilities and their population to manifest</li>
<li>Windows Store Apps: add UWP specific icon support and fix manifest creation</li>
<li>Windows Store Apps: Fix AssemblyConverter failure for Array methods</li>
<li>Windows Store Apps: Fix occasional rendering freeze when leaving and coming back in landscape mode</li>
<li>Windows Store Apps: make explicit call UnityPause(1) to pause player until explicitly unpaused via UnityPause(0)</li>
<li>Windows Store Apps: make Input.gyro available if either OrientationSensor or Gyrometer is available</li>
<li>Windows Store Apps: setup initial orientations from Player Settings</li>
<li>Windows Store: building project with IL2CPP scripting backend no longer fails.</li>
<li>Windows Store: Fixed a memory leak which reduced memory usage by around 4 to 8 MB.</li>
<li>Windows Store: Fixed an issue which caused functions RunningOnUIThread and RunningOnAppThread in UnityEngine.WSA.Application to throw exceptions if called on non-main thread.</li>
<li>Windows Store: Fixed an issue which made UWP class libraries throw FileNotFoundException when invoking into native WinRT components.</li>
<li>XboxOne/IL2CPP: Correct metadata loading on startup.</li>
</ul>

### Changes since 5.3.0f2  (Release Candidate 2)
