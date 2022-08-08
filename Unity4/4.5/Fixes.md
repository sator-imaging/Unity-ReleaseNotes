# Unity 4.5

https://unity3d.com/unity/whats-new/unity-4.5

## Fixes

- [2D Fixes](#2d-fixes)
- [Android Fixes:](#android-fixes)
- [Editor Fixes:](#editor-fixes)
- [Graphics Fixes:](#graphics-fixes)
- [iOS Fixes:](#ios-fixes)
- [Mecanim Fixes:](#mecanim-fixes)
- [Physics Fixes:](#physics-fixes)
- [Windows Phone / Windows Store Apps Fixes:](#windows-phone--windows-store-apps-fixes)
- [Other Fixes:](#other-fixes)


#### 4.5 brings a lot of fixes all over the place, so here they are split into sections:

### 2D Fixes

*   "Custom Pivot" value field made wider to fit 8 digit numbers in Sprite Editor.
*   2D polygon collider editor lines z position is now forced to zero.
*   Added confirmation window to grid slicing when creating large amounts of sprites in Sprite Editor.
*   Atlas texture will be correctly bundled in an atlas bundle when the bundle is created with kAssetBundleIncludeCompleteAssets flag and has a Texture with atlases Sprites as its main asset.
*   Cancelling packing won't prevent future packing attempts.
*   Correctly disable Sprite wireframe display.
*   Correctly handle initial default TextureImporter FilterMode in the DefaultSpritePackerPolicy in Sprite Packer.
*   Correctly initialise Sprite textureRect if all pixels are transparent.
*   Deselecting sprite in Sprite Packer window now works.
*   Destroying a Sprite's texture will not crash the SpriteRenderer that's using it.
*   Destroying a material array via UI will not break the Sprite inspector.
*   SpriteRenderer will not reset MaterialPropertyBlock.
*   Dropping sprite asset to hierarchy no longer changes texture of a random material.
*   Fixed light culling for scaled sprites.
*   Fixed precision errors in tight mesh generation code. It now correctly works together with PixelSnap shaders.
*   Fixed Sprite Packer issues when packing in editor automation mode.
*   Fixed Sprite Packer border generation to not sometimes write over the pixels of a nearby Sprite.
*   Handled Sprite Packer policy assembly type query failures. Fixes hangs when using 3rd party libraries such as pnunit.
*   PixelsToUnits property, when set to Infinity, will flip back to the default value of 100.
*   Prevented a false error when generating Sprites from a 1-pixel tall/wide texture.
*   Prevented sprites larger than max atlas size from participating in packing.
*   Removed a legacy assert which sometimes caused error messages during Sprite generation.
*   Reopening Unity will reopen the Sprite Packer window correctly.
*   Significantly reduced Sprite packing memory requirements.
*   Sprite editor rectangle values are now clamped properly.
*   Sprite Editor wasn't repainted when single sprite got unselected.
*   Sprite Packer policies with duplicate names will not throw exceptions.
*   Sprite Packer will not corrupt some textures when Unity is running in automation mode.
*   Sprite preview will correctly work in play mode for atlases sprites.
*   SpriteRenderer component will now correctly display an error message when a material with an incompatible shader (fixed function) is assigned.
*   Sprite-Diffuse shader now correctly uses color provided by the SpriteRenderer.
*   Sprites generated from NPOT textures when running with -nographics flag will now work correctly.
*   Sprites generated from NPOT textures will now work correctly on graphics cards where NPOT textures are not supported.
*   SpriteRenderer will now output normals and tangents if the active material require them.
*   Sprites with mipmaps can now be packed. A custom Sprite Packer policy is required to enable atlas texture mipmapping.
*   Stabilized packing to avoid cases where removing one Sprite could grow the final atlas size.
*   Undo added to the 2D Joint gizmos.
*   When determining if non-square textures can produce sprites, check the compressed format for square-requirement. NPOT PVRTC textures are not compressed and therefore are ok for generating sprites.
*   When loading an asset bundle that contains a SpriteRenderer in the editor, the sorting layer for the SpriteRenderer will not be reset to default.

### Android Fixes:

*   Fix for JVM picking up enviers when trying to build an android apk.
*   Fix for Samsung Game Pad axis mapping.
*   Fixed "Google Android Project" export.
*   Fixed AccelerationEvent.deltaTime.
*   Fixed an issue where some devices would freeze if unity was paused.
*   Fixed an issue where some joysticks/controllers weren't given a proper name.
*   Fixed crash on ART when calling methods with no arguments.
*   Fixed crash on ART when processing input.
*   Fixed crash on cancelling a video on Kindle Fire.
*   Fixed crash on TerrainData creation.
*   Fixed crash when using Font.RequestCharactersInTexture().
*   Fixed floating point errors on Tegra2.
*   Fixed input deadlock in OUYA console.
*   Fixed keyboardType handling.
*   Fixed Native Render plugins.
*   Fixed potential crash on soft-ime close.
*   Fixed setting audio sample rate on Android
*   Fixed some issues with graphics corruption when switching quality setting.
*   Fixed texCubeGrad and texCubeLod issues.
*   Fixed the error when wrong extension function could be used on GLES 2.
*   If a joystick is disconnected it will now show up as an empty string in the GetJoystickNames() array.
*   Logging a warning if merged manifest doesn't contain MAIN activity
*   Preload thread no longer consumes battery while application is in a paused state.
*   Re-added missing init() function.
*   Fixed crash on Android 4.4.2 when running on certain Adreno GPUs.

### Editor Fixes:

*   "Layout" button now displays the currently selected layout name.
*   2D Transform tool rotation is now disabled when the sprite is small enough in the scene view.
*   Active scenes count properly displayed when more than 100 scenes are added to Build Settings window.
*   Added missing platform strings to OS X build post-processor.
*   Asset importer confirmation dialog text is now different when multiple files are going to be changed.
*   Call to GetWindow() with focus makes sure the window always becomes visible.
*   Cancelling the drag of multiple sprites to scene view or hierarchy no longer generates GameObject.
*   Corrected error message when adding component with mismatched class and file name
*   Creating prefab from GameObjects which contains cloth no longer crashes.
*   Do not show linear color space setting in free version (Pro only feature).
*   Dragging single or multiple sprites to hierarchy works.
*   Fit tool windows on screen when resolution changes.
*   Fix the Script Execution Order Window to only show MonoBehaviours and ScriptableObjects. And fix dragging scripts from project browser so it only allows valid scripts.
*   Fixed a crash when rendering preview images for prefabs with ClothRenderer components.
*   Fixed changes being undone when dragging assets from Windows Explorer onto Unity Editor.
*   Fixed crash when adding trees to terrain with no tree prototype defined.
*   Fixed crash when resizing array to 0 in inspector with multiple objects selected.
*   Fixed crash when script name is 32 characters or longer.
*   Fixed crash when Sprite.Create's 1st argument (Texture) is null.
*   Fixed crash when switching from "Rig" to "Model" tab in model inspector when having unapplied changes.
*   Fixed crash when switching to play mode with scene that hides transform children with HideFlags.DontSave.
*   Fixed crash when trying to import unreadable font.
*   Fixed crash when undoing a prefab revert.
*   Fixed crash when using InitializeOnLoad attribute to execute code that calls back into engine.
*   Fixed GLES emulation when running in -force-opengl mode.
*   Fixed GUILayout errors when multi-selecting audio clips
*   Fixed memory leaking when moving terrains.
*   Fixed multi-editing arrays in custom property drawers.
*   Fixed non-monobehavior classes breaking the script execution order window.
*   Fixed order of backing up/disabling/enabling scripts when reimporting.
*   Fixed Package Import Window was missing folders and had incorrect indentation
*   Fixed popup windows sometimes overlapping with the taskbar on Windows.
*   Fixed script importing error if the script contains a field whose name is ended with "guid".
*   Fixed scripts being recompiled every time a project got loaded.
*   Fixed that popup windows was not closed when using keyboard shortcut to go into playmode. This caused null-reference exceptions.
*   Fixed that popups auto closes on OSX 10.9 (Maverick) on secondary displays.
*   Fixed that the project wizard selection for 2D did not work when creating a new project from an already running Unity instance (OSX issue only).
*   GameObject are no longer moved to the root of the scene hierarchy when using Undo.RegisterFullObjectHierarchyUndo().
*   Handles no longer get stuck when dragged outside of scene view.
*   Hide "Alpha is Transparency" when no alpha channel is generated.
*   Hide GPU-skinning option in Unity free since it's a pro feature.
*   Importing very wide sprites no longer triggers an assert message.
*   Inform user about platforms with no support for Splash Screen in Player Settings window.
*   Made chinese input to not print out duplicate Western characters
*   Made it possible to undo changes made to prefab assets.
*   Make curve editor popup initially show with correct ranges when present.
*   Make PropertyField foldouts (for e.g. arrays) work together with PrefixLabel.
*   No more null ref exceptions while changing tabs in FBXImporter.
*   Obey script execution order when reloading scripts.
*   Object creation now takes priority when naming an undo group.
*   Optimize transform hierarchy from Animator context menu can now be undo’ed.
*   Pivot-to-vertex snapping works again in scene view.
*   Prefab children in the Project Browser are now sorted in transform order, to match Hierarchy sorting.
*   ProjectSettings.asset (force text) can now be upgraded correctly.
*   Remove Components from GameObjects in m\_Undos list that were not registered for undo in m\_Undos .
*   Reverting to prefab value can now be undone.
*   Sub assets in the Project Browser are now sorted first by type then by name.
*   Texture importer inspector failed to render after reset from context menu.
*   Throw exception when attempting to build a development version of a Linux headless player (unsupported).
*   Undoing destruction of objects in serialized files will now correctly mark the recreated objects as persistent. This fixes dataloss.
*   Unity will throw an error during build type when you have classes with same name in the project, this was causing serialization issues during runtime which was hard to track.
*   Unity won't crash when setting material properties in OnValidate function.
*   Unity won't hang when importing some of the assets on PCs with Intel HD 4000.
*   Unsupported texture types are not shown in sprite editor.
*   When trees are placed at the border of terrain now they will respect brush density setting.

### Graphics Fixes:

*   Animating floating-point ParticleSystem properties no longer resets time whenever the property value changes.
*   Depth texture requirement removed from EdgeDetectEffectNormals image effect.
*   DirectX 11 fullscreen applications will always launch on main display now; the previous behavior was quite random.
*   Fixed \_ProjectionParams.x (negative when target buffer is upside-down) not being set when rendering without a camera.
*   Fixed 3D textures in DirectX 11 where height is not the same as depth.
*   Fixed "Disabled" Depth Test interpreted as "Never" on OpenGL ES 2.0.
*   Fixed ASTC texture importing.
*   Fixed crash when destroying an active RenderTexture.
*   Fixed crash when Mesh user is registered twice.
*   Fixed crash when using Shader Forge.
*   Fixed editor crash when working with mobile targets and using DXT compressed textures.
*   Fixed error messages with image effects at some game view aspect ratios.
*   Fixed GL.Clear in some cases not clearing stencil properly on DX9 and DX11.
*   Fixed Linear color space being wrong in the editor in DirectX 11 mode.
*   Fixed occasional crash when quitting standalone player that uses DirectX 11.
*   Fixed occlusion culling data bake error.
*   Fixed Skybox rendering when using custom camera projection matrices (e.g. when doing stereo rendering like Oculus Rift).
*   Fixed TextureFormat enumeration missing a few compressed texture formats (ETC2, ASTC).
*   Fixed Umbra related false occlusion and light flickering.
*   Fixed Umbra related occlusion culling errors when camera’s near plane intersects occluding geometry.
*   Fixed Umbra related portal index error that prevents occlusion culling working properly.
*   Fixed various issues with skinned meshes on GLES 2.0.
*   OpenGL ES 3.0 (Android and iOS) fixes:
    *   Fixed 2D sprite rendering.
    *   Fixed crash when using cloth simulation.
    *   Fixed first frame being corrupted.
    *   Fixed fog rendering.
    *   Fixed errors in some GLSL shaders.
    *   Fixed GPU memory leak when releasing RenderTextures.
    *   Fixed immediate mode rendering when GL.End is called multiple times.
    *   Fixed SSAO image effect.
    *   Improved reliability and correctness across wide range of supported devices.
*   Recursive rendering of camera from OnWillRender will now trigger error and return cleanly (instead of crashing in the worst case).
*   Shader fixes:
    *   .cginc files with UTF8 BOM markers don't confuse shader compilers. Include files at non-ASCII paths work on Windows properly now.
    *   Fixed crash if shaders have infinite (cyclic) fallback chains.
    *   Fixed editor graphics emulation (e.g. "shader model 2.0") not quite working when DX11 was used.
    *   Fixed GLSL translation of some global matrix initializers.
    *   Fixed shader errors on some platforms (e.g. DX11) being reported as warnings in the editor. Now all errors are errors, and warnings are warnings like it should be!
    *   Fixed shaders that use material-driven fixed function states (i.e. blend mode controlled from material properties) going wrong on graphics emulation level switching.
    *   Improved precision of EncodeFloatRGBA function.
    *   Shader.SetGlobalTexture no longer throws an exception when passed a null texture.
    *   Worked around DX11 shader compiler bug with spot light soft shadows that was affecting WindowsStore/WP8 apps.
*   Shuriken: Editor handles the case where Particle System component is deleted.
*   Umbra occlusion culling now returns error if scene has vertices that make bounds very large and can cause baking to hang.

### iOS Fixes:

*   Added workaround for iOS 7.1 slow/hanging scene loading on iPhone 4.
*   Fixed case when empty app was using 100% of CPU.
*   Fixed case when iOS application can not be built when the "Google Android Project" check-box is enabled.
*   Fixed handling of on screen keyboard input field.
*   Fixed iOS submission (missing icons) issue.
*   Fixed issues in RenderTexture (FBO) management.
*   Fixed mono AOT issue when calls are made via interface.
*   Fixed mscorlib support.
*   Fixed OpenGL ES context creation to adhere to Apple guidelines (should fix crashes on startup on context creation).
*   Fixed rendering issue (black screen) when non-native resolution was used.
*   Fixed Screen.orientation returning wrong values after you enabled previously disabled orientation that device currently has.
*   Fixed second stage iOS splashscreen issue.
*   Fixed Simulator build.
*   Fixed touch updating logic for Unity Remote.
*   Fixed unknown device type detection.
*   Fixed use of Advertising Identifier.
*   Fixed webcam on iOS 6.0 and later.
*   Fixed Windows crosscompiler crash with --debug.
*   Fixed WWW leak.
*   Fixed WWW.audio and WWW.assetBundle loading.
*   Updated XCode plugin to work with XCode 5.1 (build and run should work).
*   Warn user before deleting build target folder contents.
*   WWW will not accept self signed certificates by default anymore.

### Mecanim Fixes:

*   Fixed crash when Animator are disabled by other Animator during events.
*   Fixed crash when disabling GameObject during an Event.
*   Fixed animation not correctly producing transform changed messages.
*   Fixed AnimationClip.Length always returning 1 for all player.
*   Fixed animator causing issues with Collision contacts.
*   Fixed backward compatibility issue for WebPlayer. Mesh deformation for Game using Mesh.Combine were not working anymore with Animator Component.
*   Fixed bad dependency tracking of PPtr animations in AssetBundles.
*   Fixed character having double translation when interrupting a transition from an empty state.
*   Fixed crash in animation when changing bindings on some platforms.
*   Fixed crash in standalone when using HumanTrait.BoneName.
*   Fixed crash when building level with an AnimationClip for sprites referenced by more than one controller.
*   Fixed crash when playing an animation that ends with an animation event when an object is inactive.
*   Fixed crash when previewing disabled object.
*   Fixed crash when trying to undo layer deletion.
*   Fixed crash when undoing layer creation.
*   Fixed crash when using Animator.GetBoneTransform() on an Animator without an Avatar.
*   Fixed crash when you drag and drop an animation clip on a Game Object.
*   Fixed crash with corrupted controller.
*   Fixed crash with invalid BlendTree parameters.
*   Fixed invalid parameter when adding a BlendTree child to a BlendTree.
*   Fixed Lag causes avatar not to reach MatchPosition.
*   Fixed memory leaks.
*   Fixed NullReference exception when adding transitions in play mode.
*   Fixed NullReference exception when opening Animator Window.
*   Fixed Trigger parameter not reseting correctly for transition with a duration of 0 second.
*   Fixed undo of added BlendTree child.
*   Fixed undo of added Layer.
*   Fixed undo of changes done in the Avatar mapping tool using the body image.
*   Fixed update of transition so that 0 duration transitions are evaluated correctly.
*   Makes events be triggered when passed over in a transition.
*   Wrote docs for Motion - base class for AnimationClip and BlendTree.
*   Fixed scale not being applied in Transition previewer.

### Physics Fixes:

*   2D rigid-bodies now update their positions as well as perform interpolation/extrapolation in the correct order based upon their depth in a transform hierarchy.
*   2D rigid-body rotational inertia no longer scales with collider size but rather with the rigid-body mass.
*   Allow static/kinematic collisions and triggers to occur.
*   Box2D sub-stepping can cause missed Exit callbacks under certain conditions.
*   Can now set the Rigidbody2D rotational inertia.
*   Changing the GameObject layer should cause existing 2D collisions to be re-evaluated.
*   Child 2D rigid-body that is either Sleeping or Kinematic now follows any parent 2D rigid-body.
*   Clamp 2D rigid-body position/rotation to realistic bounds to stop numeric overflow.
*   Collision normal and other information not updated during OnCollisionStay2D callbacks.
*   Collision reports for 2D colliders can result in an "Exit" callback without an "Enter" callback.
*   Collision/Trigger callbacks are maintained correctly during processes that force Box2D to regenerate collider shapes.
*   Disabled Polygon Collider Editor when the component is not enabled.
*   Do not create 2D joint if either the object the joint is on or the connected object is inactive.
*   Don't send 2D physics callbacks if respective rigid-bodies are asleep.
*   Exposed a flag to enable collisions between rigid bodies connected with any type of joints.
*   Fixed 2D collider gizmo not rendering in expected position.
*   Fixed child Collider2D position when rotated under negative scale.
*   Fixed cloth simulation after re-activation.
*   Fixed crash caused by three or more collinear vertices used in a PolygonCollider2D.
*   Fixed crash when removing a 2D rigid-body that is currently reporting collisions or triggers.
*   Fixed crash when sphere casting to a mesh collider with less than 9 triangles on win64 target.
*   Fixed DistanceJoint2D incorrectly controling maximum distance only.
*   Fixed issue where changing the scale of a Collider2D during a collision callback could result in a duplicate callback being made.
*   Fixed issue where compound hierarchies of Collider2D would not correctly rotate.
*   Fixed problem in Box2D where joints can cause infinities in static body state when solving position constraints. This would persist even when exiting play mode due to the static ground-body being used.
*   Increased the range for JointAngleLimits2D so that angle limits can extend beyond a single rotation.
*   Made the default of 2D rigid-body center-of-mass to the rigid-body origin.
*   Physics2D.OverlapCircle() and Physics2D.OverlapArea() now check all edges on EdgeCollider2D.
*   Removing RigidBody2D in play mode incorrectly disables any attached 2D colliders.
*   The Editor reports modifications on "Physics2DSettings.asset".
*   Update HingeJoint2D and SliderJoint2D angle/reference angle when joint is forcibly modified via direct transform change.
*   When changing 2D collider trigger state, existing contacts will now be changed to match that state.
*   Can now add multiple 2D slider joints.
*   Fixed excessive cloth self collision simulation which rendered some games practically unplayable.

### Windows Phone / Windows Store Apps Fixes:

*   Application.internetReachability will now return proper values.
*   Creating ArrayList from native array will work correctly.
*   Field with AnimationCurve\[\] no longer crashes app.
*   Fixed a bug where Assembly Preprocessor would crash when it tries to load a PDB file that does not match DLL.
*   Fixed a regression, where class (derived from MonoBehavior) variables were not initialised if there's a private constructor.
*   Fixed animated script variables update when same script attached multiple times.
*   Fixed build failure when using Serializable or NonSerialized attributes in UnityScript.
*   Fixed detailed view of memory profiler.
*   Fixed Input.inputString not working with Unicode characters.
*   Fixed shadows in Editor when it's set to Windows Store Apps/Windows Phone 8 target and graphics emulation is set to Direct3D 11 Feature levels 9.1/9.3.
*   If you don't specify full path for Profiler.logFile, the file will be saved in the temporary folder, also if there's an error while creating a file, appropriate message will be printed in the log.
*   OnAudioFilterRead function will work correctly.
*   Plugins won't be ignored while in Editor if they're compatible.
*   Release/Master players are now compiled with /Oi (Generate Intrinsic Functions) optimisations.
*   Scripts with identical names get executed correctly.
*   SendMessage will correctly work in cases when argument is a native array.
*   Start, Update and similar methods in scripts derived from generic base class are now properly invoked.
*   Texture2D.ReadPixels now works on Windows Phone 8 and other platforms that use BGRA back buffer/render textures.
*   Unity will not call Update on Windows Phone 8/Windows Store Apps if it's static.
*   WP: Fixed a bug where accessing graphics device in OnApplicationPause() handler causes a crash if device screen times out.
*   WP: Fixed a crash which would sometimes occur during scene load if user pauses the game at the appropriate moment.
*   WP: Fixed an error, where some of the serialization functions were not found, during build from Unity.
*   WP: Fixed an issue where .NET would throw a generic constraint violation exception when calling a method that has a generic constraint, overrides base class method, returns IEnumerator and calls a delegate which has the same generic parameter constraint
*   WP: Fixed an issue where screen would get rotated after rendering screen to a texture while in landscape orientation.
*   WP: Fixed an issue where Visual Studio would sometimes refuse to deploy game to the phone.
*   WP: Fixed an issue which caused player to crash on application resume when unsupported shaders were present in the scene.
*   WP: Fixed reflections not working on standard pro asset water when application is in landscape orientation.
*   WP: Fixed spotlight culling when application is in landscape orientation.
*   WP: Fixed SystemInfo.operatingSystem and SystemInfo.processorType to report correct operating system on all players and correct CPU name on ARM.
*   WP: Generic instance methods now don't throw InvalidOperationException when defined in generic instance types.
*   WP: Graphics capabilities related to depth sampling are now correctly detected on Adreno 3xx GPUs (note: still doesn't work on Adreno 2xx due to driver issues).
*   WP: Make LocationService status update more reliable and accurate.
*   WP: Object.SendMessage() will now not throw missing method exception when it tries to send message to private inherited method.
*   WP: Project will now build correctly when project directory contains multiple .winmd files with the same filename.
*   WP: Resolution will now be correctly detected on phones than have larger screen than 768x1280.
*   WP: Screen.dpi now returns physical device DPI, rather than 0.
*   WP: Splashscreen is now positioned correctly on devices with aspect ratio other than 15:9.
*   WP: Usage of System.Reflection.BindingFlags and System.TypeCode are now not redirected incorrectly to WinRTLegacy.
*   WP: Using System.ApplicationException now doesn't throw missing method exception.
*   WP: Using System.Security.Cryptography.ICryptoTransform now doesn't throw missing method exception.
*   WSA: Application won't crash, when snapping is performed during application load.
*   WSA: Correctly serialize AnimationCurve if it's a null object.
*   WSA: Fix serialization of serializable types without public default constructors.
*   WSA: Fixed a rare WACK failure where 'Crashes and hangs' test woudn't pass.
*   WSA: Fixed an issue, where application would sometimes crash when calling RaycastHit.lightmapCoord.
*   WSA: Fixed an issue, where you couldn't enable Independent Input source, even if you enable that option in Player Settings
*   WSA: Fixed animated script variables when using inheritance or SerializeField attribute.
*   WSA: Fixed broken webcam image due to incorrect stride in YUY2 decoding routine.
*   WSA: Fixed buttons on virtual joystick 0.
*   WSA: Fixed crash caused by InvalidCastException in Boo.Lang.dll.
*   WSA: Fixed ctrl key stuck when alt is held down.
*   WSA: Fixed Cursor.SetCursor() does not hide native system cursor.
*   WSA: Fixed exception in graphics code.
*   WSA: Fixed forcing orientation on startup.
*   WSA: Fixed hang when resuming app with Independent Input Source enabled.
*   WSA: Fixed incorrect windows size created on Windows 8.1.
*   WSA: Fixed input events and Input.inputString broken on touch devices.
*   WSA: Fixed Input.multiTouchEnabled.
*   WSA: Fixed mouse events when using touch screen at the same time.
*   WSA: Fixed mouse position when resolution is not fullscreen.
*   WSA: Fixed post build event in generated Visual Studio project, if the project name contains spaces.
*   WSA: Fixed Screen.fullScreen property.
*   WSA: Fixed selecting this platform in build settings clears Development Build setting.
*   WSA: Fixed soft cursor going outside of screen.
*   WSA: Fixed UnityScript.lang.dll preprocessing stage - serializing UnityScript.Array will not crash anymore.
*   WSA: Fixed WWW.progress returns on 1 and 0.
*   WSA: Handle exception when receiving data from
*   WSA: Handle forbidden characters in product name.
*   WSA: Ignore linear color space setting, not supported on this platform.
*   WSA: Implemented better error message if application is already running when Build & Run.
*   WSA: Implemented better error message when doing Build & Run to network location.
*   WSA: Improve mouse position accuracy in scripts.
*   WSA: Instead of hardcoded path query env variable "ProgramFiles(x86)" to get path to Program Files.
*   WSA: Make 'Development Build' checkbox available, so that profiler usage is consistent with other platforms.
*   WSA: Make autorotation work for multiple specific orientations.
*   WSA: Plugins no longer fail project builds in the Editor.
*   WSA: Select Release or Master configuration based on 'Development Build' setting when Build & Run.
*   WSA: Serialization Weaver will now not crash when there are fields in C# scripts which Type is defined in WinRT API.
*   WSA: Set location desired accuracy as given by user on Windows 8.1.
*   WSA: Show touch screen keyboard for GUI text fields.
*   WSA: SystemInfo.devicetUniqueIdentifier will always return a valid string even if Advertising ID is disabled on Windows 8.1, please refer to documentation for more information.
*   WSA: Touches will not generate mouse clicks, when simulateMouseWithTouches=false.
*   WSA: Unity Editor will now correctly detect unavailable APIs when building Windows Store App game.
*   WSA: Unity will output a more user friendly message when .NET 4.5 or .NET 4.5.1 are not available.
*   WSA: Unity will throw an error if you're passing incorrect URI to Launcher.
*   WSA: Unity won't spam 'No such host is known' in certain cases when connecting to profiler.
*   WSA: Unity won't specify Content-Type header when using WWW, if Content-Type header is provided by user.
*   WSA: UnityScript.Lang.Array will not be serialized, thus will not produce a crash.
*   WSA: UnitySetInput won't crash when Independent Input Source is enabled.
*   WSA: When building player, Unity will mark all files as non read only, so overwriting shouldn't be a problem. This should solve issue for Perforce user, where some of the files were being marked as read only.
*   WSA: When generating Assembly-CSharp projects, they will reference WinRTLegacy.dll now.
*   WSA: When using Debug configuration, and D3D11 debug layers are not available - an informational message will be printed instead of error.
*   WSA: WWW will correctly send POST data.
*   WSA: When compiling scripts targeting Windows 8.1, all .NET 4.5.1 for Windows Store Apps references will get added.

### Other Fixes:

*   AI: Fixed a crash when trying to draw uninitialized path node debug info.
*   AI: Fixed erroneous rendering of agent debug info when navmesh uses height mesh, or when navmesh window is not visible.
*   AI: Fixed NavMeshAgent.Move sometimes undershooting terrain.
*   AI: Fixed OffMeshLinks trying to remap every frame when auto-updating was disabled.
*   AI: Fixed problem where agents would not use height-mesh when stopping at a carved boundary.
*   AI: Fixed problem where any change in rotation or scale would trigger re-carving regardless of specified move-threshold.
*   Animation: Animation Event popup no longer freezes for events of deleted scripts.
*   Animation: Fixed a crash when adding, at runtime, pre-4.3 asset bundles containing animations.
*   Animation: Optimize option is disabled from Animator context menu when it's missing an avatar.
*   Asset Bundles: Fixed script compatibility errors when loading asset bundles built in from a different project.
*   Asset Import: Modified directories no longer force their entire contents to be re-imported. Also fixes the issue of the cache server being spammed with requests that have no hashes.
*   Assets Management: Fix null callback call in coroutine invocation.
*   Audio: Fixed "Bypass Effects" on AudioSource which caused AudioSources to be muted when initialized with the flag set.
*   Audio: Fixed "m\_PausedSources.empty()" error when resuming game.
*   BlackBerry: Added "Run in Background" checkbox to player settings user interface.
*   BlackBerry: Microphone is now supported.
*   BlackBerry: Password fields will no longer lose text if the user deselects the field and then reselects it.
*   BlackBerry: Screen.sleepTimeout is now supported.
*   BlackBerry: Spaces are now supported in bar file name.
*   BlackBerry: The following typefaces are now supported: Chinese simplified, Japanese, Thai, Arabic, Indic, Hindi.
*   Build Pipeline: Icons are now applied before post-processing scripts are called.
*   Debugger: Don't hang when debugger evaluation triggers an exception.
*   Documentation: "Switch to component" button in Scripting Reference.
*   Documentation: Correctly expanding left side tree in Scripting Reference.
*   Documentation: Fixed many customer-reported bugs.
*   Documentation: Fixed bug which caused UnityEditor to be excluded from Scripting Reference.
*   Documentation: Improved display of generic classes and functions.
*   Documentation: Re-introduced API History in scripting reference docs.
*   Documentation: Showing name of current class/member in page title.
*   Documentation: Switching between C# and JS for sample code in Scripting API on IE11 has been fixed.
*   Events: Fixed OnMouseExit not being called properly.
*   IMGUI: Don't send OnMouseDown event for last used object when clicking IMGUI elements.
*   IMGUI: Fixed bug in GUI.ScrollTowards / GUI.ScrollTo that caused it to think it needed scrolling when it didn't. This also fixes a bug in the Highlighter API where a highlight would fail without warning for certain ScrollViews.
*   Input: Fixed touch tracing stuck to last game object.
*   Installers: DisplayVersion not set correctly by Windows installers.
*   Licence system: Re-enabled license logging in editor.log.
*   License system: Removed support for old PACE license files.
*   Linux: Fixed "jump" when initially locking mouse cursor.
*   Linux: Fixed DllImport of system libraries.
*   Linux: Fixed eventual runaway CPU usage on headless players.
*   Linux: Fixed non-ASCII text input.
*   Linux: Fixed OnApplicationFocus.
*   Linux: Fixed Ping implementation.
*   Linux: Fixed switching to fullscreen mode for window managers that do this in two steps.
*   Linux: Fixed translucent hardware cursors.
*   Linux: Report screen size as 640x480 in headless player (avoids crashes when user projects divide by screen size).
*   Linux/Windows: Don't unload asset bundles when their assets may need to be reloaded.
*   Mac OS X Standalone: Fix asserts when going in or out of fullscreen mode.
*   Mac OS X Standalone: Fix GetAllNetworkInterfaces.
*   Mac OS X Standalone: Fixed KeyUp events being registered for Command-Key combinations.
*   Mac OS X Standalone: Fixed mouse coordinates when requesting a window larger than the screen.
*   Mac OS X Standalone: Fixed position of IME candidate window in fullscreen mode.
*   Mac OS X Standalone: Joysticks now work in 64 bit builds.
*   Mac OS X Standalone: Screen Selector dialog can now show more than six quality settings.
*   Profiler: Fixed "autoconnect profiler" not working.
*   Scripting: Disallow invalid scripts in execution order UI.
*   Scripting: Fixed crash when disabling from constructor.
*   Scripting: Fixed crash when inspecting SerializedProperty.displayName.
*   Scripting: Fixed crash when passing null to Undo.RecordObject.
*   Scripting: Fixed crash when project contains mixed-mode assemblies.
*   Scripting: Fixed crash when unloading a domain with multiple threads.
*   Scripting: Fixed namespace detection for MonoBehaviors containing methods with default parameters.
*   Scripting: Fixed player build when unqualified class names collide.
*   Scripting: Fixed Resources.FindObjectsOfTypeAll sometimes returning objects of incorrect types.
*   Scripting: Only add the component if the required components are not conflicting with the existing ones.
*   Scripting: Undo/Redo of FullHierarchyUndo works now.
*   Serialization: Fixed crash on type load error.
*   Substance: Cache files for GenerateAndCache / DoNothingAndCache are no longer backuped to iCloud and should no longer cause AppStore rejection.
*   Substance: Color specular maps are now correctly generated, and the proper specular alpha channel is now used when the specular map is used as the alpha source for another ProceduralTexture. This might change the way some metallic materials are rendered.
*   Substance: Fixed a rare bug of DXT1 normal maps being used on Windows instead of DXT5.
*   Substance: Fixed a serialization bug which would cause webplayers to crash with newly built content.
*   Substance: Fixed crash when importing a Substance with usage-less outputs.
*   Substance: Fixed error message being displayed when serializing an uninitialized boolean.
*   Substance: Fixed some rare editor crashes.
*   Substance: If no input was modified, RebuildTextures() no longer causes ProceduralTextures that were read from cache to be re-computed from scratch.
*   Substance: If present, the component names of vector inputs are now properly displayed in the inspector instead of the default x, y, z, w.
*   Substance: Mipmap selector in the Texture preview now works on ProceduralTextures.
*   Substance: Non-default assignments of Substance outputs to shader properties are now correctly serialized and should no longer be reset when reimporting Substance materials.
*   Substance: Normal maps will no longer invert or bake incorrectly when being reimported after switching between desktop/web and mobile build targets.
*   Substance: ProceduralMaterial.ClearCache() now releases more memory than before when using image inputs.
*   Substance: ProceduralMaterial.ClearCache() now works correctly when queuing ClearCache() requests for multiple materials.
*   Substance: ProceduralMaterials are now always imported _after_ shaders and should no longer lose their shader assignment.
*   Substance: Undo/Redo operations now behave as expected in the ProceduralMaterial and SubstanceImporter inspectors.
*   Substances: Rebuilt substance textures don't obey sRGB encoding.
*   Terrain: Accessing to a destroyed terrain will not crash Unity any more.
*   Terrain: Established minimum size for all terrain wizards.
*   Terrain: Fixed crash in some cases where trees are manipulated if an invalid prototype is present.
*   Terrain: Fixed crashes on certain platforms
*   Terrain: Fixed terrain properties not being saved if they are edited in inspector debug mode.
*   Terrain: Fixed trees bending to wrong wind direction if trees are rotated.
*   Terrain: Mark TerrainData dirty after PhysicMaterial set for Heightmap.
*   Terrain: Object creation can now be undone.
*   Terrain: Removed unwanted message saying "A tree couldn't be loaded because the prefab is missing" when importing a project.
*   Version Control: Delete folders when the .meta file is deleted as part of a sync.
*   Version Control: Encrypt version control credentials before saving to file.
*   Version Control: Fix errors from too long vcs messages.
*   Version Control: Fix missing unlock command in pending window context meny for assets.
*   Version Control: Fix not being able to get incoming file if you had previously added the same file at the same time as remote and just before syncing deleted the asset.
*   Version Control: Fix script execution order inspector grayed out and meta files not modified with order info when applying.
*   Webplayer: OSX installs should no longer encounter update problems when installed via user accounts with unusual permissions.
*   Webplayer: OSX versions prior to 10.9 can again run Unity games built with Unity 2.x.
*   Webplayer: Several security holes have been closed.
*   Webplayer: Webplayer now requests and requires crossdomain.xml authorization for HTTP redirects to URLs on different servers/ports.
*   WebPlugin: Fixed UnityObject JS param options not working with IE.
*   WebPlugin: Updater does not need to self elevate if the plugin is installed in LocalLow.
*   WIndows Standalone: Disable window size adjustment by Windows on window move.
*   WWW: Editor and standalone players now correctly set the Accept-Encoding header to 'identity' when transmitting HTTP requests.
*   WWW: Fixed “bad file length” errors when loading scene bundle in editor or web player.
*   WWW: Fixed CRC tests for downloads of uncompressed AssetBundles to the Cache.
*   WWW: Fixed the race condition when the task was destroyed before the outstanding continuations were properly completed.
*   WWW: Several fixes to prevent XSS and header-forgery attacks.