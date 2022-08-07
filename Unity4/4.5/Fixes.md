# Unity 4.5
https://unity3d.com/unity/whats-new/unity-4.5

## Fixes


#### 4.5 brings a lot of fixes all over the place, so here they are split into sections:

### 2D Fixes
<ul>
<li>"Custom Pivot" value field made wider to fit 8 digit numbers in Sprite Editor.</li>
<li>2D polygon collider editor lines z position is now forced to zero. </li>
<li>Added confirmation window to grid slicing when creating large amounts of sprites in Sprite Editor.</li>
<li>Atlas texture will be correctly bundled in an atlas bundle when the bundle is created with kAssetBundleIncludeCompleteAssets flag and has a Texture with atlases Sprites as its main asset. </li>
<li>Cancelling packing won't prevent future packing attempts.</li>
<li>Correctly disable Sprite wireframe display.</li>
<li>Correctly handle initial default TextureImporter FilterMode in the DefaultSpritePackerPolicy in Sprite Packer.</li>
<li>Correctly initialise Sprite textureRect if all pixels are transparent.</li>
<li>Deselecting sprite in Sprite Packer window now works. </li>
<li>Destroying a Sprite's texture will not crash the SpriteRenderer that's using it.</li>
<li>Destroying a material array via UI will not break the Sprite inspector.</li>
<li>SpriteRenderer will not reset MaterialPropertyBlock.</li>
<li>Dropping sprite asset to hierarchy no longer changes texture of a random material. </li>
<li>Fixed light culling for scaled sprites. </li>
<li>Fixed precision errors in tight mesh generation code. It now correctly works together with PixelSnap shaders. </li>
<li>Fixed Sprite Packer issues when packing in editor automation mode. </li>
<li>Fixed Sprite Packer border generation to not sometimes write over the pixels of a nearby Sprite.</li>
<li>Handled Sprite Packer policy assembly type query failures. Fixes hangs when using 3rd party libraries such as pnunit.</li>
<li>PixelsToUnits property, when set to Infinity, will flip back to the default value of 100.</li>
<li>Prevented a false error when generating Sprites from a 1-pixel tall/wide texture.</li>
<li>Prevented sprites larger than max atlas size from participating in packing.</li>
<li>Removed a legacy assert which sometimes caused error messages during Sprite generation.</li>
<li>Reopening Unity will reopen the Sprite Packer window correctly.</li>
<li>Significantly reduced Sprite packing memory requirements. </li>
<li>Sprite editor rectangle values are now clamped properly. </li>
<li>Sprite Editor wasn't repainted when single sprite got unselected. </li>
<li>Sprite Packer policies with duplicate names will not throw exceptions. </li>
<li>Sprite Packer will not corrupt some textures when Unity is running in automation mode. </li>
<li>Sprite preview will correctly work in play mode for atlases sprites. </li>
<li>SpriteRenderer component will now correctly display an error message when a material with an incompatible shader (fixed function) is assigned. </li>
<li>Sprite-Diffuse shader now correctly uses color provided by the SpriteRenderer. </li>
<li>Sprites generated from NPOT textures when running with -nographics flag will now work correctly. </li>
<li>Sprites generated from NPOT textures will now work correctly on graphics cards where NPOT textures are not supported. </li>
<li>SpriteRenderer will now output normals and tangents if the active material require them. </li>
<li>Sprites with mipmaps can now be packed. A custom Sprite Packer policy is required to enable atlas texture mipmapping.</li>
<li>Stabilized packing to avoid cases where removing one Sprite could grow the final atlas size.</li>
<li>Undo added to the 2D Joint gizmos.</li>
<li>When determining if non-square textures can produce sprites, check the compressed format for square-requirement. NPOT PVRTC textures are not compressed and therefore are ok for generating sprites.</li>
<li>When loading an asset bundle that contains a SpriteRenderer in the editor, the sorting layer for the SpriteRenderer will not be reset to default.</li>
</ul>

### Android Fixes:
<ul>
<li>Fix for JVM picking up enviers when trying to build an android apk. </li>
<li>Fix for Samsung Game Pad axis mapping. </li>
<li>Fixed "Google Android Project" export. </li>
<li>Fixed AccelerationEvent.deltaTime.</li>
<li>Fixed an issue where some devices would freeze if unity was paused. </li>
<li>Fixed an issue where some joysticks/controllers weren't given a proper name. </li>
<li>Fixed crash on ART when calling methods with no arguments.</li>
<li>Fixed crash on ART when processing input.</li>
<li>Fixed crash on cancelling a video on Kindle Fire.</li>
<li>Fixed crash on TerrainData creation.</li>
<li>Fixed crash when using Font.RequestCharactersInTexture().</li>
<li>Fixed floating point errors on Tegra2.</li>
<li>Fixed input deadlock in OUYA console.</li>
<li>Fixed keyboardType handling.</li>
<li>Fixed Native Render plugins.</li>
<li>Fixed potential crash on soft-ime close. </li>
<li>Fixed setting audio sample rate on Android</li>
<li>Fixed some issues with graphics corruption when switching quality setting.</li>
<li>Fixed texCubeGrad and texCubeLod issues.</li>
<li>Fixed the error when wrong extension function could be used on GLES 2.</li>
<li>If a joystick is disconnected it will now show up as an empty string in the GetJoystickNames() array.</li>
<li>Logging a warning if merged manifest doesn't contain MAIN activity</li>
<li>Preload thread no longer consumes battery while application is in a paused state.</li>
<li>Re-added missing init() function. </li>
<li>Fixed crash on Android 4.4.2 when running on certain Adreno GPUs.</li>
</ul>

### Editor Fixes:
<ul>
<li>"Layout" button now displays the currently selected layout name. </li>
<li>2D Transform tool rotation is now disabled when the sprite is small enough in the scene view. </li>
<li>Active scenes count properly displayed when more than 100 scenes are added to Build Settings window.</li>
<li>Added missing platform strings to OS X build post-processor. </li>
<li>Asset importer confirmation dialog text is now different when multiple files are going to be changed. </li>
<li>Call to GetWindow() with focus makes sure the window always becomes visible. </li>
<li>Cancelling the drag of multiple sprites to scene view or hierarchy no longer generates GameObject. </li>
<li>Corrected error message when adding component with mismatched class and file name</li>
<li>Creating prefab from GameObjects which contains cloth no longer crashes. </li>
<li>Do not show linear color space setting in free version (Pro only feature).</li>
<li>Dragging single or multiple sprites to hierarchy works.</li>
<li>Fit tool windows on screen when resolution changes.</li>
<li>Fix the Script Execution Order Window to only show MonoBehaviours and ScriptableObjects. And fix dragging scripts from project browser so it only allows valid scripts. </li>
<li>Fixed a crash when rendering preview images for prefabs with ClothRenderer components. </li>
<li>Fixed changes being undone when dragging assets from Windows Explorer onto Unity Editor. </li>
<li>Fixed crash when adding trees to terrain with no tree prototype defined.</li>
<li>Fixed crash when resizing array to 0 in inspector with multiple objects selected. </li>
<li>Fixed crash when script name is 32 characters or longer.</li>
<li>Fixed crash when Sprite.Create's 1st argument (Texture) is null.</li>
<li>Fixed crash when switching from "Rig" to "Model" tab in model inspector when having unapplied changes. </li>
<li>Fixed crash when switching to play mode with scene that hides transform children with HideFlags.DontSave.</li>
<li>Fixed crash when trying to import unreadable font. </li>
<li>Fixed crash when undoing a prefab revert. </li>
<li>Fixed crash when using InitializeOnLoad attribute to execute code that calls back into engine.</li>
<li>Fixed GLES emulation when running in -force-opengl mode. </li>
<li>Fixed GUILayout errors when multi-selecting audio clips </li>
<li>Fixed memory leaking when moving terrains. </li>
<li>Fixed multi-editing arrays in custom property drawers.</li>
<li>Fixed non-monobehavior classes breaking the script execution order window. </li>
<li>Fixed order of backing up/disabling/enabling scripts when reimporting.</li>
<li>Fixed Package Import Window was missing folders and had incorrect indentation</li>
<li>Fixed popup windows sometimes overlapping with the taskbar on Windows.</li>
<li>Fixed script importing error if the script contains a field whose name is ended with "guid".</li>
<li>Fixed scripts being recompiled every time a project got loaded.</li>
<li>Fixed that popup windows was not closed when using keyboard shortcut to go into playmode. This caused null-reference exceptions. </li>
<li>Fixed that popups auto closes on OSX 10.9 (Maverick) on secondary displays.</li>
<li>Fixed that the project wizard selection for 2D did not work when creating a new project from an already running Unity instance (OSX issue only). </li>
<li>GameObject are no longer moved to the root of the scene hierarchy when using Undo.RegisterFullObjectHierarchyUndo(). </li>
<li>Handles no longer get stuck when dragged outside of scene view. </li>
<li>Hide "Alpha is Transparency" when no alpha channel is generated.</li>
<li>Hide GPU-skinning option in Unity free since it's a pro feature. </li>
<li>Importing very wide sprites no longer triggers an assert message. </li>
<li>Inform user about platforms with no support for Splash Screen in Player Settings window.</li>
<li>Made chinese input to not print out duplicate Western characters </li>
<li>Made it possible to undo changes made to prefab assets. </li>
<li>Make curve editor popup initially show with correct ranges when present.</li>
<li>Make PropertyField foldouts (for e.g. arrays) work together with PrefixLabel.</li>
<li>No more null ref exceptions while changing tabs in FBXImporter.</li>
<li>Obey script execution order when reloading scripts.</li>
<li>Object creation now takes priority when naming an undo group.</li>
<li>Optimize transform hierarchy from Animator context menu can now be undo’ed.</li>
<li>Pivot-to-vertex snapping works again in scene view. </li>
<li>Prefab children in the Project Browser are now sorted in transform order, to match Hierarchy sorting. </li>
<li>ProjectSettings.asset (force text) can now be upgraded correctly. </li>
<li>Remove Components from GameObjects in m_Undos list that were not registered for undo in m_Undos .</li>
<li>Reverting to prefab value can now be undone.</li>
<li>Sub assets in the Project Browser are now sorted first by type then by name. </li>
<li>Texture importer inspector failed to render after reset from context menu. </li>
<li>Throw exception when attempting to build a development version of a Linux headless player (unsupported). </li>
<li>Undoing destruction of objects in serialized files will now correctly mark the recreated objects as persistent. This fixes dataloss. </li>
<li>Unity will throw an error during build type when you have classes with same name in the project, this was causing serialization issues during runtime which was hard to track. </li>
<li>Unity won't crash when setting material properties in OnValidate function. </li>
<li>Unity won't hang when importing some of the assets on PCs with Intel HD 4000. </li>
<li>Unsupported texture types are not shown in sprite editor.</li>
<li>When trees are placed at the border of terrain now they will respect brush density setting. </li>
</ul>

### Graphics Fixes:
<ul>
<li>Animating floating-point ParticleSystem properties no longer resets time whenever the property value changes.</li>
<li>Depth texture requirement removed from EdgeDetectEffectNormals image effect.</li>
<li>DirectX 11 fullscreen applications will always launch on main display now; the previous behavior was quite random.</li>
<li>Fixed _ProjectionParams.x (negative when target buffer is upside-down) not being set when rendering without a camera.</li>
<li>Fixed 3D textures in DirectX 11 where height is not the same as depth.</li>
<li>Fixed "Disabled" Depth Test interpreted as "Never" on OpenGL ES 2.0.</li>
<li>Fixed ASTC texture importing.</li>
<li>Fixed crash when destroying an active RenderTexture.</li>
<li>Fixed crash when Mesh user is registered twice.</li>
<li>Fixed crash when using Shader Forge.</li>
<li>Fixed editor crash when working with mobile targets and using DXT compressed textures.</li>
<li>Fixed error messages with image effects at some game view aspect ratios. </li>
<li>Fixed GL.Clear in some cases not clearing stencil properly on DX9 and DX11.</li>
<li>Fixed Linear color space being wrong in the editor in DirectX 11 mode.</li>
<li>Fixed occasional crash when quitting standalone player that uses DirectX 11.</li>
<li>Fixed occlusion culling data bake error.</li>
<li>Fixed Skybox rendering when using custom camera projection matrices (e.g. when doing stereo rendering like Oculus Rift).</li>
<li>Fixed TextureFormat enumeration missing a few compressed texture formats (ETC2, ASTC).</li>
<li>Fixed Umbra related false occlusion and light flickering.</li>
<li>Fixed Umbra related occlusion culling errors when camera’s near plane intersects occluding geometry.</li>
<li>Fixed Umbra related portal index error that prevents occlusion culling working properly.</li>
<li>Fixed various issues with skinned meshes on GLES 2.0.</li>
<li>OpenGL ES 3.0 (Android and iOS) fixes: 
<ul>
<li>Fixed 2D sprite rendering.</li>
<li>Fixed crash when using cloth simulation.</li>
<li>Fixed first frame being corrupted.</li>
<li>Fixed fog rendering.</li>
<li>Fixed errors in some GLSL shaders.</li>
<li>Fixed GPU memory leak when releasing RenderTextures.</li>
<li>Fixed immediate mode rendering when GL.End is called multiple times.</li>
<li>Fixed SSAO image effect.</li>
<li>Improved reliability and correctness across wide range of supported devices.</li>
</ul></li>
<li>Recursive rendering of camera from OnWillRender will now trigger error and return cleanly (instead of crashing in the worst case).</li>
<li>Shader fixes: 
<ul>
<li>.cginc files with UTF8 BOM markers don't confuse shader compilers. Include files at non-ASCII paths work on Windows properly now.</li>
<li>Fixed crash if shaders have infinite (cyclic) fallback chains. </li>
<li>Fixed editor graphics emulation (e.g. "shader model 2.0") not quite working when DX11 was used. </li>
<li>Fixed GLSL translation of some global matrix initializers.</li>
<li>Fixed shader errors on some platforms (e.g. DX11) being reported as warnings in the editor. Now all errors are errors, and warnings are warnings like it should be! </li>
<li>Fixed shaders that use material-driven fixed function states (i.e. blend mode controlled from material properties) going wrong on graphics emulation level switching.</li>
<li>Improved precision of EncodeFloatRGBA function.</li>
<li>Shader.SetGlobalTexture no longer throws an exception when passed a null texture.</li>
<li>Worked around DX11 shader compiler bug with spot light soft shadows that was affecting WindowsStore/WP8 apps. </li>
</ul></li>
<li>Shuriken: Editor handles the case where Particle System component is deleted.</li>
<li>Umbra occlusion culling now returns error if scene has vertices that make bounds very large and can cause baking to hang.</li>
</ul>

### iOS Fixes:
<ul>
<li>Added workaround for iOS 7.1 slow/hanging scene loading on iPhone 4.</li>
<li>Fixed case when empty app was using 100% of CPU.</li>
<li>Fixed case when iOS application can not be built when the "Google Android Project" check-box is enabled.</li>
<li>Fixed handling of on screen keyboard input field.</li>
<li>Fixed iOS submission (missing icons) issue.</li>
<li>Fixed issues in RenderTexture (FBO) management.</li>
<li>Fixed mono AOT issue when calls are made via interface.</li>
<li>Fixed mscorlib support.</li>
<li>Fixed OpenGL ES context creation to adhere to Apple guidelines (should fix crashes on startup on context creation).</li>
<li>Fixed rendering issue (black screen) when non-native resolution was used.</li>
<li>Fixed Screen.orientation returning wrong values after you enabled previously disabled orientation that device currently has.</li>
<li>Fixed second stage iOS splashscreen issue.</li>
<li>Fixed Simulator build.</li>
<li>Fixed touch updating logic for Unity Remote.</li>
<li>Fixed unknown device type detection.</li>
<li>Fixed use of Advertising Identifier.</li>
<li>Fixed webcam on iOS 6.0 and later.</li>
<li>Fixed Windows crosscompiler crash with --debug.</li>
<li>Fixed WWW leak.</li>
<li>Fixed WWW.audio and WWW.assetBundle loading. </li>
<li>Updated XCode plugin to work with XCode 5.1 (build and run should work).</li>
<li>Warn user before deleting build target folder contents.</li>
<li>WWW will not accept self signed certificates by default anymore.</li>
</ul>

### Mecanim Fixes:
<ul>
<li>Fixed crash when Animator are disabled by other Animator during events.</li>
<li>Fixed crash when disabling GameObject during an Event.</li>
<li>Fixed animation not correctly producing transform changed messages.</li>
<li>Fixed AnimationClip.Length always returning 1 for all player.</li>
<li>Fixed animator causing issues with Collision contacts.</li>
<li>Fixed backward compatibility issue for WebPlayer. Mesh deformation for Game using Mesh.Combine were not working anymore with Animator Component.</li>
<li>Fixed bad dependency tracking of PPtr animations in AssetBundles.</li>
<li>Fixed character having double translation when interrupting a transition from an empty state. </li>
<li>Fixed crash in animation when changing bindings on some platforms. </li>
<li>Fixed crash in standalone when using HumanTrait.BoneName.</li>
<li>Fixed crash when building level with an AnimationClip for sprites referenced by more than one controller.</li>
<li>Fixed crash when playing an animation that ends with an animation event when an object is inactive.</li>
<li>Fixed crash when previewing disabled object.</li>
<li>Fixed crash when trying to undo layer deletion. </li>
<li>Fixed crash when undoing layer creation.</li>
<li>Fixed crash when using Animator.GetBoneTransform() on an Animator without an Avatar.</li>
<li>Fixed crash when you drag and drop an animation clip on a Game Object.</li>
<li>Fixed crash with corrupted controller.</li>
<li>Fixed crash with invalid BlendTree parameters.</li>
<li>Fixed invalid parameter when adding a BlendTree child to a BlendTree.</li>
<li>Fixed Lag causes avatar not to reach MatchPosition.</li>
<li>Fixed memory leaks.</li>
<li>Fixed NullReference exception when adding transitions in play mode.</li>
<li>Fixed NullReference exception when opening Animator Window.</li>
<li>Fixed Trigger parameter not reseting correctly for transition with a duration of 0 second.</li>
<li>Fixed undo of added BlendTree child.</li>
<li>Fixed undo of added Layer.</li>
<li>Fixed undo of changes done in the Avatar mapping tool using the body image.</li>
<li>Fixed update of transition so that 0 duration transitions are evaluated correctly.</li>
<li>Makes events be triggered when passed over in a transition.</li>
<li>Wrote docs for Motion - base class for AnimationClip and BlendTree.</li>
<li>Fixed scale not being applied in Transition previewer.</li>
</ul>

### Physics Fixes:
<ul>
<li>2D rigid-bodies now update their positions as well as perform interpolation/extrapolation in the correct order based upon their depth in a transform hierarchy.</li>
<li>2D rigid-body rotational inertia no longer scales with collider size but rather with the rigid-body mass.</li>
<li>Allow static/kinematic collisions and triggers to occur.</li>
<li>Box2D sub-stepping can cause missed Exit callbacks under certain conditions. </li>
<li>Can now set the Rigidbody2D rotational inertia. </li>
<li>Changing the GameObject layer should cause existing 2D collisions to be re-evaluated.</li>
<li>Child 2D rigid-body that is either Sleeping or Kinematic now follows any parent 2D rigid-body.</li>
<li>Clamp 2D rigid-body position/rotation to realistic bounds to stop numeric overflow. </li>
<li>Collision normal and other information not updated during OnCollisionStay2D callbacks.</li>
<li>Collision reports for 2D colliders can result in an "Exit" callback without an "Enter" callback. </li>
<li>Collision/Trigger callbacks are maintained correctly during processes that force Box2D to regenerate collider shapes.</li>
<li>Disabled Polygon Collider Editor when the component is not enabled.</li>
<li>Do not create 2D joint if either the object the joint is on or the connected object is inactive. </li>
<li>Don't send 2D physics callbacks if respective rigid-bodies are asleep. </li>
<li>Exposed a flag to enable collisions between rigid bodies connected with any type of joints.</li>
<li>Fixed 2D collider gizmo not rendering in expected position. </li>
<li>Fixed child Collider2D position when rotated under negative scale. </li>
<li>Fixed cloth simulation after re-activation.</li>
<li>Fixed crash caused by three or more collinear vertices used in a PolygonCollider2D. </li>
<li>Fixed crash when removing a 2D rigid-body that is currently reporting collisions or triggers. </li>
<li>Fixed crash when sphere casting to a mesh collider with less than 9 triangles on win64 target.</li>
<li>Fixed DistanceJoint2D incorrectly controling maximum distance only. </li>
<li>Fixed issue where changing the scale of a Collider2D during a collision callback could result in a duplicate callback being made. </li>
<li>Fixed issue where compound hierarchies of Collider2D would not correctly rotate. </li>
<li>Fixed problem in Box2D where joints can cause infinities in static body state when solving position constraints. This would persist even when exiting play mode due to the static ground-body being used. </li>
<li>Increased the range for JointAngleLimits2D so that angle limits can extend beyond a single rotation. </li>
<li>Made the default of 2D rigid-body center-of-mass to the rigid-body origin.</li>
<li>Physics2D.OverlapCircle() and Physics2D.OverlapArea() now check all edges on EdgeCollider2D. </li>
<li>Removing RigidBody2D in play mode incorrectly disables any attached 2D colliders.</li>
<li>The Editor reports modifications on "Physics2DSettings.asset". </li>
<li>Update HingeJoint2D and SliderJoint2D angle/reference angle when joint is forcibly modified via direct transform change. </li>
<li>When changing 2D collider trigger state, existing contacts will now be changed to match that state.</li>
<li>Can now add multiple 2D slider joints.</li>
<li>Fixed excessive cloth self collision simulation which rendered some games practically unplayable.</li>
</ul>

### Windows Phone / Windows Store Apps Fixes:
<ul>
<li>Application.internetReachability will now return proper values. </li>
<li>Creating ArrayList from native array will work correctly.</li>
<li>Field with AnimationCurve[] no longer crashes app.</li>
<li>Fixed a bug where Assembly Preprocessor would crash when it tries to load a PDB file that does not match DLL. </li>
<li>Fixed a regression, where class (derived from MonoBehavior) variables were not initialised if there's a private constructor. </li>
<li>Fixed animated script variables update when same script attached multiple times. </li>
<li>Fixed build failure when using Serializable or NonSerialized attributes in UnityScript. </li>
<li>Fixed detailed view of memory profiler. </li>
<li>Fixed Input.inputString not working with Unicode characters. </li>
<li>Fixed shadows in Editor when it's set to Windows Store Apps/Windows Phone 8 target and graphics emulation is set to Direct3D 11 Feature levels 9.1/9.3.</li>
<li>If you don't specify full path for Profiler.logFile, the file will be saved in the temporary folder, also if there's an error while creating a file, appropriate message will be printed in the log. </li>
<li>OnAudioFilterRead function will work correctly.</li>
<li>Plugins won't be ignored while in Editor if they're compatible. </li>
<li>Release/Master players are now compiled with /Oi (Generate Intrinsic Functions) optimisations. </li>
<li>Scripts with identical names get executed correctly.</li>
<li>SendMessage will correctly work in cases when argument is a native array.</li>
<li>Start, Update and similar methods in scripts derived from generic base class are now properly invoked. </li>
<li>Texture2D.ReadPixels now works on Windows Phone 8 and other platforms that use BGRA back buffer/render textures.</li>
<li>Unity will not call Update on Windows Phone 8/Windows Store Apps if it's static.</li>
<li>WP: Fixed a bug where accessing graphics device in OnApplicationPause() handler causes a crash if device screen times out. </li>
<li>WP: Fixed a crash which would sometimes occur during scene load if user pauses the game at the appropriate moment.</li>
<li>WP: Fixed an error, where some of the serialization functions were not found, during build from Unity. </li>
<li>WP: Fixed an issue where .NET would throw a generic constraint violation exception when calling a method that has a generic constraint, overrides base class method, returns IEnumerator and calls a delegate which has the same generic parameter constraint </li>
<li>WP: Fixed an issue where screen would get rotated after rendering screen to a texture while in landscape orientation.</li>
<li>WP: Fixed an issue where Visual Studio would sometimes refuse to deploy game to the phone. </li>
<li>WP: Fixed an issue which caused player to crash on application resume when unsupported shaders were present in the scene.</li>
<li>WP: Fixed reflections not working on standard pro asset water when application is in landscape orientation.</li>
<li>WP: Fixed spotlight culling when application is in landscape orientation.</li>
<li>WP: Fixed SystemInfo.operatingSystem and SystemInfo.processorType to report correct operating system on all players and correct CPU name on ARM. </li>
<li>WP: Generic instance methods now don't throw InvalidOperationException when defined in generic instance types. </li>
<li>WP: Graphics capabilities related to depth sampling are now correctly detected on Adreno 3xx GPUs (note: still doesn't work on Adreno 2xx due to driver issues).</li>
<li>WP: Make LocationService status update more reliable and accurate. </li>
<li>WP: Object.SendMessage() will now not throw missing method exception when it tries to send message to private inherited method. </li>
<li>WP: Project will now build correctly when project directory contains multiple .winmd files with the same filename. </li>
<li>WP: Resolution will now be correctly detected on phones than have larger screen than 768x1280. </li>
<li>WP: Screen.dpi now returns physical device DPI, rather than 0.</li>
<li>WP: Splashscreen is now positioned correctly on devices with aspect ratio other than 15:9. </li>
<li>WP: Usage of System.Reflection.BindingFlags and System.TypeCode are now not redirected incorrectly to WinRTLegacy. </li>
<li>WP: Using System.ApplicationException now doesn't throw missing method exception.</li>
<li>WP: Using System.Security.Cryptography.ICryptoTransform now doesn't throw missing method exception.</li>
<li>WSA: Application won't crash, when snapping is performed during application load. </li>
<li>WSA: Correctly serialize AnimationCurve if it's a null object.</li>
<li>WSA: Fix serialization of serializable types without public default constructors.</li>
<li>WSA: Fixed a rare WACK failure where 'Crashes and hangs' test woudn't pass. </li>
<li>WSA: Fixed an issue, where application would sometimes crash when calling RaycastHit.lightmapCoord. </li>
<li>WSA: Fixed an issue, where you couldn't enable Independent Input source, even if you enable that option in Player Settings </li>
<li>WSA: Fixed animated script variables when using inheritance or SerializeField attribute.</li>
<li>WSA: Fixed broken webcam image due to incorrect stride in YUY2 decoding routine.</li>
<li>WSA: Fixed buttons on virtual joystick 0.</li>
<li>WSA: Fixed crash caused by InvalidCastException in Boo.Lang.dll.</li>
<li>WSA: Fixed ctrl key stuck when alt is held down.</li>
<li>WSA: Fixed Cursor.SetCursor() does not hide native system cursor.</li>
<li>WSA: Fixed exception in graphics code.</li>
<li>WSA: Fixed forcing orientation on startup.</li>
<li>WSA: Fixed hang when resuming app with Independent Input Source enabled. </li>
<li>WSA: Fixed incorrect windows size created on Windows 8.1.</li>
<li>WSA: Fixed input events and Input.inputString broken on touch devices. </li>
<li>WSA: Fixed Input.multiTouchEnabled.</li>
<li>WSA: Fixed mouse events when using touch screen at the same time.</li>
<li>WSA: Fixed mouse position when resolution is not fullscreen.</li>
<li>WSA: Fixed post build event in generated Visual Studio project, if the project name contains spaces.</li>
<li>WSA: Fixed Screen.fullScreen property.</li>
<li>WSA: Fixed selecting this platform in build settings clears Development Build setting. </li>
<li>WSA: Fixed soft cursor going outside of screen. </li>
<li>WSA: Fixed UnityScript.lang.dll preprocessing stage - serializing UnityScript.Array will not crash anymore. </li>
<li>WSA: Fixed WWW.progress returns on 1 and 0.</li>
<li>WSA: Handle exception when receiving data from</li>
<li>WSA: Handle forbidden characters in product name.</li>
<li>WSA: Ignore linear color space setting, not supported on this platform. </li>
<li>WSA: Implemented better error message if application is already running when Build &amp; Run.</li>
<li>WSA: Implemented better error message when doing Build &amp; Run to network location.</li>
<li>WSA: Improve mouse position accuracy in scripts.</li>
<li>WSA: Instead of hardcoded path query env variable "ProgramFiles(x86)" to get path to Program Files.</li>
<li>WSA: Make 'Development Build' checkbox available, so that profiler usage is consistent with other platforms. </li>
<li>WSA: Make autorotation work for multiple specific orientations.</li>
<li>WSA: Plugins no longer fail project builds in the Editor. </li>
<li>WSA: Select Release or Master configuration based on 'Development Build' setting when Build &amp; Run.</li>
<li>WSA: Serialization Weaver will now not crash when there are fields in C# scripts which Type is defined in WinRT API.</li>
<li>WSA: Set location desired accuracy as given by user on Windows 8.1. </li>
<li>WSA: Show touch screen keyboard for GUI text fields.</li>
<li>WSA: SystemInfo.devicetUniqueIdentifier will always return a valid string even if Advertising ID is disabled on Windows 8.1, please refer to documentation for more information. </li>
<li>WSA: Touches will not generate mouse clicks, when simulateMouseWithTouches=false. </li>
<li>WSA: Unity Editor will now correctly detect unavailable APIs when building Windows Store App game.</li>
<li>WSA: Unity will output a more user friendly message when .NET 4.5 or .NET 4.5.1 are not available. </li>
<li>WSA: Unity will throw an error if you're passing incorrect URI to Launcher.</li>
<li>WSA: Unity won't spam 'No such host is known' in certain cases when connecting to profiler.</li>
<li>WSA: Unity won't specify Content-Type header when using WWW, if Content-Type header is provided by user.</li>
<li>WSA: UnityScript.Lang.Array will not be serialized, thus will not produce a crash. </li>
<li>WSA: UnitySetInput won't crash when Independent Input Source is enabled.</li>
<li>WSA: When building player, Unity will mark all files as non read only, so overwriting shouldn't be a problem. This should solve issue for Perforce user, where some of the files were being marked as read only. </li>
<li>WSA: When generating Assembly-CSharp projects, they will reference WinRTLegacy.dll now.</li>
<li>WSA: When using Debug configuration, and D3D11 debug layers are not available - an informational message will be printed instead of error. </li>
<li>WSA: WWW will correctly send POST data.</li>
<li>WSA: When compiling scripts targeting Windows 8.1, all .NET 4.5.1 for Windows Store Apps references will get added.</li>
</ul>

### Other Fixes:
<ul>
<li>AI: Fixed a crash when trying to draw uninitialized path node debug info.</li>
<li>AI: Fixed erroneous rendering of agent debug info when navmesh uses height mesh, or when navmesh window is not visible. </li>
<li>AI: Fixed NavMeshAgent.Move sometimes undershooting terrain.</li>
<li>AI: Fixed OffMeshLinks trying to remap every frame when auto-updating was disabled.</li>
<li>AI: Fixed problem where agents would not use height-mesh when stopping at a carved boundary.</li>
<li>AI: Fixed problem where any change in rotation or scale would trigger re-carving regardless of specified move-threshold.</li>
<li>Animation: Animation Event popup no longer freezes for events of deleted scripts.</li>
<li>Animation: Fixed a crash when adding, at runtime, pre-4.3 asset bundles containing animations.</li>
<li>Animation: Optimize option is disabled from Animator context menu when it's missing an avatar. </li>
<li>Asset Bundles: Fixed script compatibility errors when loading asset bundles built in from a different project.</li>
<li>Asset Import: Modified directories no longer force their entire contents to be re-imported. Also fixes the issue of the cache server being spammed with requests that have no hashes.</li>
<li>Assets Management: Fix null callback call in coroutine invocation.</li>
<li>Audio: Fixed "Bypass Effects" on AudioSource which caused AudioSources to be muted when initialized with the flag set.</li>
<li>Audio: Fixed "m_PausedSources.empty()" error when resuming game.</li>
<li>BlackBerry: Added "Run in Background" checkbox to player settings user interface. </li>
<li>BlackBerry: Microphone is now supported.</li>
<li>BlackBerry: Password fields will no longer lose text if the user deselects the field and then reselects it. </li>
<li>BlackBerry: Screen.sleepTimeout is now supported.</li>
<li>BlackBerry: Spaces are now supported in bar file name.</li>
<li>BlackBerry: The following typefaces are now supported: Chinese simplified, Japanese, Thai, Arabic, Indic, Hindi.</li>
<li>Build Pipeline: Icons are now applied before post-processing scripts are called.</li>
<li>Debugger: Don't hang when debugger evaluation triggers an exception.</li>
<li>Documentation: "Switch to component" button in Scripting Reference. </li>
<li>Documentation: Correctly expanding left side tree in Scripting Reference. </li>
<li>Documentation: Fixed many customer-reported bugs.</li>
<li>Documentation: Fixed bug which caused UnityEditor to be excluded from Scripting Reference.</li>
<li>Documentation: Improved display of generic classes and functions.</li>
<li>Documentation: Re-introduced API History in scripting reference docs.</li>
<li>Documentation: Showing name of current class/member in page title.</li>
<li>Documentation: Switching between C# and JS for sample code in Scripting API on IE11 has been fixed.</li>
<li>Events: Fixed OnMouseExit not being called properly.</li>
<li>IMGUI: Don't send OnMouseDown event for last used object when clicking IMGUI elements.</li>
<li>IMGUI: Fixed bug in GUI.ScrollTowards / GUI.ScrollTo that caused it to think it needed scrolling when it didn't. This also fixes a bug in the Highlighter API where a highlight would fail without warning for certain ScrollViews.</li>
<li>Input: Fixed touch tracing stuck to last game object. </li>
<li>Installers: DisplayVersion not set correctly by Windows installers.</li>
<li>Licence system: Re-enabled license logging in editor.log.</li>
<li>License system: Removed support for old PACE license files.</li>
<li>Linux: Fixed "jump" when initially locking mouse cursor.</li>
<li>Linux: Fixed DllImport of system libraries. </li>
<li>Linux: Fixed eventual runaway CPU usage on headless players.</li>
<li>Linux: Fixed non-ASCII text input.</li>
<li>Linux: Fixed OnApplicationFocus.</li>
<li>Linux: Fixed Ping implementation. </li>
<li>Linux: Fixed switching to fullscreen mode for window managers that do this in two steps.</li>
<li>Linux: Fixed translucent hardware cursors.</li>
<li>Linux: Report screen size as 640x480 in headless player (avoids crashes when user projects divide by screen size).</li>
<li>Linux/Windows: Don't unload asset bundles when their assets may need to be reloaded.</li>
<li>Mac OS X Standalone: Fix asserts when going in or out of fullscreen mode.</li>
<li>Mac OS X Standalone: Fix GetAllNetworkInterfaces. </li>
<li>Mac OS X Standalone: Fixed KeyUp events being registered for Command-Key combinations.</li>
<li>Mac OS X Standalone: Fixed mouse coordinates when requesting a window larger than the screen.</li>
<li>Mac OS X Standalone: Fixed position of IME candidate window in fullscreen mode.</li>
<li>Mac OS X Standalone: Joysticks now work in 64 bit builds.</li>
<li>Mac OS X Standalone: Screen Selector dialog can now show more than six quality settings.</li>
<li>Profiler: Fixed "autoconnect profiler" not working.</li>
<li>Scripting: Disallow invalid scripts in execution order UI.</li>
<li>Scripting: Fixed crash when disabling from constructor.</li>
<li>Scripting: Fixed crash when inspecting SerializedProperty.displayName.</li>
<li>Scripting: Fixed crash when passing null to Undo.RecordObject.</li>
<li>Scripting: Fixed crash when project contains mixed-mode assemblies.</li>
<li>Scripting: Fixed crash when unloading a domain with multiple threads.</li>
<li>Scripting: Fixed namespace detection for MonoBehaviors containing methods with default parameters.</li>
<li>Scripting: Fixed player build when unqualified class names collide.</li>
<li>Scripting: Fixed Resources.FindObjectsOfTypeAll sometimes returning objects of incorrect types.</li>
<li>Scripting: Only add the component if the required components are not conflicting with the existing ones.</li>
<li>Scripting: Undo/Redo of FullHierarchyUndo works now.</li>
<li>Serialization: Fixed crash on type load error.</li>
<li>Substance: Cache files for GenerateAndCache / DoNothingAndCache are no longer backuped to iCloud and should no longer cause AppStore rejection.</li>
<li>Substance: Color specular maps are now correctly generated, and the proper specular alpha channel is now used when the specular map is used as the alpha source for another ProceduralTexture. This might change the way some metallic materials are rendered. </li>
<li>Substance: Fixed a rare bug of DXT1 normal maps being used on Windows instead of DXT5. </li>
<li>Substance: Fixed a serialization bug which would cause webplayers to crash with newly built content. </li>
<li>Substance: Fixed crash when importing a Substance with usage-less outputs. </li>
<li>Substance: Fixed error message being displayed when serializing an uninitialized boolean. </li>
<li>Substance: Fixed some rare editor crashes. </li>
<li>Substance: If no input was modified, RebuildTextures() no longer causes ProceduralTextures that were read from cache to be re-computed from scratch. </li>
<li>Substance: If present, the component names of vector inputs are now properly displayed in the inspector instead of the default x, y, z, w. </li>
<li>Substance: Mipmap selector in the Texture preview now works on ProceduralTextures. </li>
<li>Substance: Non-default assignments of Substance outputs to shader properties are now correctly serialized and should no longer be reset when reimporting Substance materials.</li>
<li>Substance: Normal maps will no longer invert or bake incorrectly when being reimported after switching between desktop/web and mobile build targets.</li>
<li>Substance: ProceduralMaterial.ClearCache() now releases more memory than before when using image inputs. </li>
<li>Substance: ProceduralMaterial.ClearCache() now works correctly when queuing ClearCache() requests for multiple materials. </li>
<li>Substance: ProceduralMaterials are now always imported <em>after</em> shaders and should no longer lose their shader assignment. </li>
<li>Substance: Undo/Redo operations now behave as expected in the ProceduralMaterial and SubstanceImporter inspectors. </li>
<li>Substances: Rebuilt substance textures don't obey sRGB encoding.</li>
<li>Terrain: Accessing to a destroyed terrain will not crash Unity any more. </li>
<li>Terrain: Established minimum size for all terrain wizards.</li>
<li>Terrain: Fixed crash in some cases where trees are manipulated if an invalid prototype is present. </li>
<li>Terrain: Fixed crashes on certain platforms</li>
<li>Terrain: Fixed terrain properties not being saved if they are edited in inspector debug mode. </li>
<li>Terrain: Fixed trees bending to wrong wind direction if trees are rotated. </li>
<li>Terrain: Mark TerrainData dirty after PhysicMaterial set for Heightmap.</li>
<li>Terrain: Object creation can now be undone.</li>
<li>Terrain: Removed unwanted message saying "A tree couldn't be loaded because the prefab is missing" when importing a project. </li>
<li>Version Control: Delete folders when the .meta file is deleted as part of a sync. </li>
<li>Version Control: Encrypt version control credentials before saving to file. </li>
<li>Version Control: Fix errors from too long vcs messages. </li>
<li>Version Control: Fix missing unlock command in pending window context meny for assets. </li>
<li>Version Control: Fix not being able to get incoming file if you had previously added the same file at the same time as remote and just before syncing deleted the asset. </li>
<li>Version Control: Fix script execution order inspector grayed out and meta files not modified with order info when applying. </li>
<li>Webplayer: OSX installs should no longer encounter update problems when installed via user accounts with unusual permissions.</li>
<li>Webplayer: OSX versions prior to 10.9 can again run Unity games built with Unity 2.x.</li>
<li>Webplayer: Several security holes have been closed.</li>
<li>Webplayer: Webplayer now requests and requires crossdomain.xml authorization for HTTP redirects to URLs on different servers/ports. </li>
<li>WebPlugin: Fixed UnityObject JS param options not working with IE. </li>
<li>WebPlugin: Updater does not need to self elevate if the plugin is installed in LocalLow.</li>
<li>WIndows Standalone: Disable window size adjustment by Windows on window move.</li>
<li>WWW: Editor and standalone players now correctly set the Accept-Encoding header to 'identity' when transmitting HTTP requests.</li>
<li>WWW: Fixed “bad file length” errors when loading scene bundle in editor or web player.</li>
<li>WWW: Fixed CRC tests for downloads of uncompressed AssetBundles to the Cache.</li>
<li>WWW: Fixed the race condition when the task was destroyed before the outstanding continuations were properly completed.</li>
<li>WWW: Several fixes to prevent XSS and header-forgery attacks.</li>
</ul>
