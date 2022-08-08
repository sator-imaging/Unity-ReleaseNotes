# Unity 4.5

https://unity3d.com/unity/whats-new/unity-4.5

## Improvements



*   2D: Default 2D shaders now emulate premultiplied alpha. This fixes rendering in certain cases such as when rendering into a transparent render texture.
*   2D: Padding and offset values added for grid slicing in Sprite Editor.
*   2D: Sprite textures will not default to 16-bit on iOS anymore when editor is in 2D mode.
*   2D: Sprite Editor works for single mode sprites.
*   2D: Sprites now have border property (specified in pixels) that can be changed on sprite import.
*   Scripting: Rect struct now has the properties min, max, and size. This makes it easier to reuse the same code for the X and Y axis.
*   Android: Added KitKat to the list of target devices.
*   Assets management: 'optimizeGameObjects' & 'extraExposedTransformPaths' are now accessible from asset post processor.
*   Profiling: Audio profiling is improved with more relevant data and more accurate memory stats.
*   BlackBerry: bar-descriptor.xml file no longer uses deprecated xml tags.
*   BlackBerry: Keyboard types are now supported.
*   BlackBerry: Introduced GLES 3.0 support on the z30 devices.
*   Scripting: Added LayerMask.GetMask method to return a mask given multiple layer names.
*   Coroutines: StopCoroutine can now take an enumerator argument.
*   Documentation: Added docs on how to debug DirectX11 shaders with Visual Studio, look for 'SL-Debugging DirectX 11 Shaders with Visual Studio'.
*   Documentation: API history updated.
*   Documentation: Introduced new look and feel.
*   Documentation: Revived API history
*   Editor API: Expose handles preference colors in the Handles class (as read-only).
*   Editor, Standalone: WWW object can now retrieve data from servers that serve compressed content (gzip or zlib).
*   Editor: Added 'Sprite' to the type filter popup in the Project Browser.
*   Editor: Created CustomPreview attribute and ObjectPreview class. It is now possible to add extra custom preview to any inspected object.
*   Editor: Created SelectionBase attribute. When applied to a script, GameObjects with that script on will work the same as prefab roots for Scene View picking.
*   Editor: Implemented editing of Asset Labels for multiple assets at once.
*   Editor: Exposed EditorGUI.MultiFloatField and EditorGUI.MultiPropertyField.
*   Editor: Expose EditorGUIUtility.standardVerticalSpacing to make it possible for people to create standard spacing between controls (for example in PropertyDrawers) without having to hardcode the amount.
*   Editor: Improved inspector customisation with \[Tooltip\] and \[ContextMenuItem\] script attributes.
*   Editor: Overall improvement of Sprite Editor. Better handling of sprite border, holding CTRL will hide the sprite boundaries so the hidden borders can be seen, and better mouse cursor feedback.
*   Editor: Package Import Window was redesigned and now shows import items as a proper tree view.
*   Editor: Preset libraries that have default presets now have a 'Add Factory Presets To Current Library' option in the context menu.
*   Editor: PropertyDrawers are now supplemented with DecoratorDrawers, which can be used for decorative elements in the Inspector such as spacing, headers, or notes.
*   Editor: Added AnimatedValues - Simple way to have tweened UI elements in EditorGUI.
*   Editor: Implemented display of fully qualified script name in execution order inspector.
*   Graphics: Added Texture2D.EncodeToJPG.
*   Graphics: GPU Skinning on OpenGL ES 3.0 now supports at least 4096 bones per mesh on all GL ES 3.0 targets.
*   Graphics: OpenGL ES 2.0 and 3.0 maximum simultaneous texture count upgraded from 8 to 16 (where supported by the GPU).
*   Graphics: Updated videoVerticallyMirrored docs.
*   iOS: Added ability to use profiler through USB.
*   iOS: Added iOS 7.1 target selector.
*   iOS: Added iPad Air and iPad Mini Retina entries to the iPhoneGeneration enum.
*   iOS: Added missing system languages.
*   iOS: Added reporting of environment variables when launching of mono process fails.
*   iOS: Added support for render events (GL.IssuePluginEvent). Please note that you need to manually register them, as iOS do not support dynamic libraries. Check trampoline for UnityRegisterRenderingPlugin function.
*   iOS: Added Xcode 5.x splashscreen compatibility.
*   iOS: Bumped minimum version of Xcode to 5.0.
*   iOS: Did minor trampoline refactoring.
*   iOS: Rebuilt FMOD, PhysX and PLCrashReporter with -mno-thumb.
*   iOS: Implemented small CrashReporter improvements: logging to console, disabled dSYM generation for debug builds.
*   iOS: WWW implementation exposed in trampoline.
*   Linux: Query webcam for dimensions when user doesn't specify them.
*   Linux: Worked around drivers grossly underreporting video memory.
*   Mecanim: Implemented user notification when humanoid animation has animation (TQS) in between human bones.
*   Mecanim: Added finger bones to c# HumanBodyBones enum.
*   Mecanim: Animator does not spam warning messages in standalone.
*   Mecanim: Humanoid auto-configure now only use rotation information from bind pose. Translations found in bind pose were different from the ones in animation. This was causing undesired retargeting differences.
*   Mecanim: Humanoid setup and retarget console warning have been improved. Less noise and more precise information.
*   Mecanim: Optimized Animator Enable() ( 2x speed on complex controllers ).
*   OpenGL ES: Improved GL ES version selection. There is now a new Target Graphics API option "Auto" that automatically selects the best available GL ES version.
*   OS X: Enabled stack trace output when player crashes.
*   Physics: Added the following methods and properties to DistanceJoint2D: limitState, GetReactionForce() and GetReactionTorque().
*   Physics: Added the following methods and properties to HingeJoint2D: limitState, referenceAngle, jointAngle, jointSpeed, GetReactionForce(), GetReactionTorque() and GetMotorTorque().
*   Physics: Added the following methods and properties to SliderJoint2D: limitState, referenceAngle, jointTranslation, jointSpeed and GetMotorForce().
*   Physics: Added the following methods and properties to WheelJoint2D: jointTranslation, jointSpeed and GetMotorTorque().
*   Physics: Added the following methods to SpringJoint2D: GetReactionForce() and GetReactionTorque().
*   Physics: Added "RigidBody2D.simulated" property that allows control of whether a Rigidbody2D component should be simulated or not.
*   Physics: Added 2D rigid-body MovePosition and MoveRotation methods.
*   Physics: Added ability to ignore collider/collider collisions (Physics2D.IgnoreCollision).
*   Physics: Added missing Physics2D CircleCast, CircleCastAll, CircleCastNonAlloc, BoxCast, BoxCastAll & BoxCastNonAlloc.
*   Physics: Added "bounds" property (read-only) to 2D collider types.
*   Physics: Added "centerOfMass" and "worldCenterOfMass" properties (read-only) to Rigidbody2D.
*   Physics: Added "inertia" property to Rigidbody2D.
*   Physics: Added ForceMode2D type to allow selection of force to be used for "Force" or "Impulse".
*   Physics: Added GetPoint & GetRelativePoint to Rigidbody2D.
*   Physics: Added GetPointVelocity & GetRelativePointVelocity to Rigidbody2D.
*   Physics: Added GetVector & GetRelativeVector to Rigidbody2D.
*   Physics: AddForce, AddRelativeForce, AddForceAtPosition & AddTorque on Rigidbody2D now accept ForceMode2D type to match 3D physics.
*   Physics: Dragging interaction of GameObjects containing dynamic Rigidbody2D components in editor during play-mode is allowed now.
*   Physics: Do not show disabled 2D joint gizmos.
*   Physics: Exposed several Box2D properties that were previously compile-time constants.
*   Physics: PolygonCollider2D gizmo renders only the outline shape.
*   Scripting: Added GetAllCameras(Camera\[\]) and allCamerasCount API's
*   Scripting: Added UNITY\_PRO\_LICENSE define.
*   Scripting: Added GetComponentsInParent function.
*   Scripting: Added MeshUtility.SetMeshCompression and MeshUtility.GetMeshCompression to set mesh compression for Meshes generated from scripting.
*   Scripting: Improved resolution of types that inherit from types in different user assemblies.
*   Serialisation (i.e. Instantiation & Level loading) performance of MonoBehaviors is now 2x-5x faster.
*   Serialisation: Print error message when maximum recursion limit is reached.
*   Substance: Alpha channel generation can now be explicitly disabled for ProceduralMaterials in order to use runtime DXT1/ETC compression or to bake DXT1/ETC/RGB24 bitmaps.
*   Substance: Baked ProceduralTextures are now created from full RGBA32 data instead of pre-existing (and potentially already compressed) editor data.
*   Substance: Decreased memory consumption in the editor.
*   Substance: Lower peak memory footprint when generating textures for materials that were queued roughly at the same time.
*   Substance: Material thumbnails are now listed in the static preview in the same 'semantically correct' order they appear in the SubstanceImporterInspector.
*   Substance: Mipmap generation can now be disabled (the default is 'enabled').
*   Substance: Outputs tagged as "Specular" will automatically map to the \_SpecTex shader property if present.
*   Substance: Outputs that are used solely as sources for other outputs's alpha channels (typically the specular output) are no longer generated separately and will not appear in the project window anymore unless they're directly assigned to a shader slot or the GenerateAllOutputs option is checked.
*   Substance: ProceduralMaterials being computed when exiting play mode are now discarded, making the transition from play mode to editor mode faster.
*   Substance: ProceduralMaterials loaded from AssetBundles can now be inspected in play mode.
*   Substance: Processing Substances in the Editor is now always multi-threaded when not in play mode.
*   Substance: Runtime PVRTC compression on iOS/Android is now faster and of higher quality.
*   Substance: Switching between graphs or instances in a SubstanceImporterInspector will no longer cause a reimport. The reimport of the modified SBSAR asset is now performed when the entire SubstanceImporterInspector is disabled.
*   Substance: The ProceduralMaterial memory budget will be increased in smaller increments on mobile targets to further lower the peak memory footprint on these platforms.
*   Windows: Unity Editor will fallback to DirectX 11 if DirectX 9 is not available, instead of showing the dialog graphics were not initialised.
*   Webplayer: Java Webplayer Installer is now updated with the latest Java security requirements.
*   Windows Phone: The preview resolution is as close as possible to what the user requested.
*   Windows Phone: Non uniformly scaled meshes use less memory.
*   Windows Phone: Webcam resolution selection is now chosen by the aspect ratio and the total area of the preview.
*   Windows Store Apps / Windows 8.1: Added support for SwapChainPanel, it will be used in XAML project files generated for Windows 8.1, you can still use SwapChainBackroundPanel if you want.
*   Windows Store Apps / Windows 8.1: Changed template code to handle application launch through protocol, basically we added OnActivated event handling in App.xaml.cs and App.xaml.cpp files.
*   Windows Store Apps / Windows Phone: Graphics related memory optimisations. Mesh and texture uploads use less memory.
*   Windows Store Apps: When building, instead of storing absolute Unity paths inside a project, they will be store in UnityCommon.props file instead, this way making it easier to share project between several PC's.
*   Windows Store Apps: \*.pdb, \*.ilk, \*.exp for Unity libraries won't be provided in Release, Master configurations, thus reducing the exported solution size significantly.
*   Windows Store Apps: AppCallbacks::UnitySetInput() made safe for multiple invocations.
*   Windows Store Apps: ComputeBuffer.SetData will work correctly.
*   Windows Store Apps: If running other OS than Windows 8/8.1, reports it as "Unknown Windows version ()" rather than hardcoded "Windows 8"/"Windows 8.1".
*   Windows Store Apps: NativeRenderPlugin example now properly works on Windows Store Apps.
*   Windows Store Apps: Removed splash screen after the first frame is drawn.
*   Windows Store Apps: D3D applications will consume less CPU percentage thus preserving battery.
*   Windows Store Apps: System.deviceModel will return a valid value whenever possible.
*   Windows Store Apps: Unity will output used Windows SDK version in UnityPlayer.log.
*   Windows Store Apps: Unity won't spam harmless D3D warning DEVICE\_DRAW\_RENDERTARGETVIEW\_NOT\_SET in Debug builds.
*   Windows Store Apps: Webcam support is more stable; webcams now also support MJPG streams.
*   Windows Store Apps: Windows 8.1 player will now respect CompositionScale of SwapChainPanel.
*   Windows Store Apps: You can now generate C# Assembly-Charp\* projects (in BuildSettings window) which will be referenced from generated solution, allowing you to easily debug and change your scripts on the fly, the only thing to keep in mind, if you'll add/remove serialised fields in classes, you'll need to rebuild your project from Editor to compensate for changed serialised data.
*   Windows Store Apps/ Windows 8.1: SystemInfo.deviceUniqueIdentifier will return value from AdvertisingManager (http://msdn.microsoft.com/en-us/library/windows/apps/windows.system.userprofile.advertisingmanager.advertisingid.aspx)
*   Windows Store Apps/Windows Phone: MaterialPropertyBlock property setting now supported on these platforms.
*   Windows Store Apps/Windows Phone: Unity allocates fewer managed objects for its own internal bookkeeping allowing .NET garbage collector to work faster. Overall memory consumption is also reduced.
*   Windows Store Apps/Windows Phone: Added support for animated script variables .
*   Windows Store Apps/WP8: Better handling of managed objects, causes less pressure to Garbage Collection.
*   WWW: All POST requests now automatically include an x-unity-version header with the version of the Unity runtime making the request.