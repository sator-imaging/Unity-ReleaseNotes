# Unity 5.1

https://unity3d.com/unity/whats-new/unity-5.1

## Improvements



*   Android: Apply DeviceDefault theme if available, respect user's theme
*   Android: Improved soft input dialog
*   Android: New Sensor/rotation code that tries to figure out 'reversed rotation devices'
*   Animation: Added Animator.CrossFadeInFixedTime and Animator.PlayInFixedTime to support fixed time manual transitions.
*   Animation: Added AnimatorController.GetBehaviours() API function to simplify how user can query their behaviour on the asset
*   Animation: Added dragging controls on the time bar and on the background of the blending in the transition inspector
*   Animation: Added options "Add Motion", "Add Blend Tree" and "Delete" to contextual menu for blend tree
*   Animation: Allow animator window to be locked
*   Animation: Deleting a layer that has other layers synchronized on itself will also delete all the dependent layers (with a prompt)
*   Animation: Do not allow scene objects in AnimatorController's Motion ObjectField
*   Animation: Exposed ApplyBuiltinRootMotion to script
*   Animation: Retargeting import warnings are removed from the console and are now available in the model importer warning foldout. This will simplify the submission process for Animation Clip to the asset store.
*   Animation: Transition can now be copy pasted
*   Animation: Transition duration can now be specified in absolute time
*   Animation: You can now control your AnimatorState.speed/mirror/cycleOffset at runtime with controller's parameter
*   Animation Window: Copy-pasting keyframes in animation window curve view and between clips.
*   Animation Window: Curve editor supports range selection with shift-click
*   Animation Window: Curve editor supports toggle selection with command-click (control-click on Windows)
*   Animation Window: Direct editing of key values in curve editors. Use Enter/Return or context menu to start editing selected keys, Tab to switch between fields, Enter/Return to commit, and Escape to cancel editing
*   Animation Window: Dope sheet editor supports Control-click as well as right-click on Mac OS
*   Animation Window: Dragging a curve no longer loses the current selection
*   Animation Window: Keyframe selection is synced between dopesheet and curve view.
*   Animation Window: Lock button that locks the selection to currently selected clip and Animator.
*   Animation Window: Slightly increased the clickable radius for keyframes in the curve editor
*   Animation Window: When creating new clip from animation window, default to previously used path
*   BuildPipeline: There will be fewer differences between the exported data files from subsequent builds of your project when using the same version of Unity. For best results, close Unity and delete your project's Library folder before making an important build.
*   Curve Editor: Wrap mode enum popup modified to appear as a little gear, which fits nicely in the margin without being cropped.
*   Documentation: Show "construct type" for class/struct/interface
*   Editor: Added extensive support for copy/pasting colors: Copy/paste from focused color field, from context menu for color field, from color picker (with no text selected) and from hex field.
*   Editor: Adding an icon to an EditorWindow title is now exposed by using the GUIContent 'titleContent' property (the old string 'title' is now obsolete)
*   Editor: Create sprite animation clip from project window context menu.
*   Editor: Improved grid in Scene View. Eliminates the popping and inconsistent draw distance of the old grid, and also draws grid lines smaller than one unit (10th of a unit, 100th of a unit and so on) when sufficiently zoomed in. New grid shading makes it possible to have grid lines more dense in close parts of the grid without the parts further away being too dense.
*   Editor: Introduced CreateAssetMenu attribute. Apply it to ScriptableObject-derived types to cause them to show up automatically in the Assets/Create menu.
*   Editor: Introduced HelpURL attribute, for setting custom documentation URL for user-authored classes.
*   Editor: Simple expression evaluator for all number fields. Supports + - / \* % ( ) operators. This means that all number fields can be used as a calculator.
*   FrameDebugger: Shader blend, depth and raster states will be shown for draw calls.
*   GI: Final gather was moved into a separate stage. This allows the indirect baking stage to apply visibility aware upsampling to the indirect lightmap before final gather is applied for better quality.
*   GI: Reduce the amount of GI related information that is written to the log file
*   Graphics: Add CommandBuffer.DrawProcedural and DrawProceduralIndirect.
*   Graphics: Added a way to specify graphics APIs explicitly in player settings (defaults to "automatic" for each platform). For example, you could specify you only want to support Metal+ES2 in iOS builds, or only DX11 (without DX9 fallback) on Windows builds etc. This replaces the "Use DX11" and "Target iOS/GLES Graphics" settings.
*   Graphics: Added SetPixels32/GetPixels32 to Texture3D.
*   Graphics: Command Buffers can be set on Lights, see LightEvent enum and Light.AddCommandBuffer.
*   Graphics: Performance improvements on DX11 when many non-batchable objects are in view.
*   Importer: Added warning foldout to keep trace of all import warning in the ModelImporter animation tab.
*   Math: Rect(Vector2, Vector2) constructor overload added
*   Miscellaneous: Resolution.ToString() implemented
*   MonoDevelop: Including MonoDoc XML files for showing C# Intellisense tooltips in MonoDevelop
*   Physics: Add motion constraints to Rigidbody2D

*   Physics: Added HingeJoint BounceMinVelocity. When bounciness is enabled this is the minimum impact velocity which will cause the joint to bounce. Setting this very low, like zero, will cause the joint to never stop bouncing. This can lead to jittering and performance problems. Setting this very high will cause joint to never bounce.
*   Physics: Optimized performance of ‘OnTriggerStay’ messaging.
*   Physics: Rigidbodies connected to a HingeJoint will now automatically be woken up when the joint is updated.
*   Plugin Inspector: You can now select multiple plugins and change compatible platforms. Note - you cannot yet change per platform settings if multiple plugins are selected.
*   Profiler: Change ms markers in timeline view to use same label style which makes it also properly visible in both skins.
*   Profiler: Don't show FPS for every ms marker along the x axis in the timeline view - only for the last one.
*   Profiler: Fix unaligned labels for ms counts in current frame.
*   Scripting: Added Vector2.Reflect function.
*   Serialization: Extended SerializedFile size limit to 4GB
*   Shaders: Support VFACE in surface shader inputs; just use a float variable with VFACE semantic.
*   SpeedTree: A new importer setting "Animate Cross-fading" is added to SpeedTree assets. With this option on (by default), the dithering LOD transition between mesh/billboard and billboard/culled will be animated by time. This should make the trees look better in most of the scenarios.
*   SpeedTree: Now wind animation will not be interrupted if the tree gets out side of the view.
*   SpeedTree: Tree casts shadow when in cross-fading to billboard
*   Texture2D: Add Texture2D.GetRawTextureData() API
*   UI: Allow dragging anchors outside of bounds of parent when holding down Ctrl (Cmd on Mac) - the same key that disables snapping. This makes it easier to author screen transitions that support multiple resolutions, since content can be animated to move a distance that's a percentage of the screen width or height.
*   UI: Changed default blink rate and widget range of InputField caret to match the new frequency behavior.
*   Version Control: CheckoutIsValid now accept a CheckoutMode
*   Version Control: Collapse assets and their .meta files in versioning window when they have the same state
*   WebGL: Made "Explicitly Thrown Exceptions Only" mode much faster and be the default setting
*   WebGL: Support Input.touches and Input.acceleration
*   Windows Store Apps: Copy pasting will also work outside the application.
*   Windows Store Apps: Exposed Rendering path in Player Settings
*   Windows Store Apps: Refactored App.xaml.cs and MainPage.xaml.cs, it's easier now to add additional XAML pages to the project
*   XboxOne: Added functions to XboxOnePLM (GetActivationUri, GetActivationTileId, GetActivationArguments) to retrieve cached values. We still recommend listening to OnActivationEvent in your Start() frame, and processing them that way, but this provides an alternative for last-provided values.
*   XboxOne: Added support for XMA audio format
*   XboxOne: IPv6 lookup and DNS support added for C# code.
*   XboxOne: Lightmap files are now split up per level and put in separate chunks in the package manifest.
*   XboxOne: More comments have been added to the default package manifest.
*   XboxOne: Worker threads created by Unity's core systems (Physics, AI) will no longer run on cores 0 and 1, which are reserved for the Rendering thread and Unity's main thread respectively. This will be a performance gain in most cases by avoiding thread context switches.