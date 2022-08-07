# Unity 5.1
https://unity3d.com/unity/whats-new/unity-5.1

## Improvements

<ul>
<li>Android: Apply DeviceDefault theme if available, respect user's theme</li>
<li>Android: Improved soft input dialog</li>
<li>Android: New Sensor/rotation code that tries to figure out 'reversed rotation devices'</li>
<li>Animation: Added Animator.CrossFadeInFixedTime and Animator.PlayInFixedTime to support fixed time manual transitions.</li>
<li>Animation: Added AnimatorController.GetBehaviours() API function to simplify how user can query their behaviour on the asset</li>
<li>Animation: Added dragging controls on the time bar and on the background of the blending in the transition inspector</li>
<li>Animation: Added options "Add Motion", "Add Blend Tree" and "Delete" to contextual menu for blend tree</li>
<li>Animation: Allow animator window to be locked </li>
<li>Animation: Deleting a layer that has other layers synchronized on itself will also delete all the dependent layers (with a prompt)</li>
<li>Animation: Do not allow scene objects in AnimatorController's Motion ObjectField </li>
<li>Animation: Exposed ApplyBuiltinRootMotion to script</li>
<li>Animation: Retargeting import warnings are removed from the console and are now available in the model importer warning foldout. This will simplify the submission process for Animation Clip to the asset store.</li>
<li>Animation: Transition can now be copy pasted</li>
<li>Animation: Transition duration can now be specified in absolute time</li>
<li>Animation: You can now control your AnimatorState.speed/mirror/cycleOffset at runtime with controller's parameter</li>
<li>Animation Window: Copy-pasting keyframes in animation window curve view and between clips.</li>
<li>Animation Window: Curve editor supports range selection with shift-click</li>
<li>Animation Window: Curve editor supports toggle selection with command-click (control-click on Windows)</li>
<li>Animation Window: Direct editing of key values in curve editors. Use Enter/Return or context menu to start editing selected keys, Tab to switch between fields, Enter/Return to commit, and Escape to cancel editing</li>
<li>Animation Window: Dope sheet editor supports Control-click as well as right-click on Mac OS</li>
<li>Animation Window: Dragging a curve no longer loses the current selection</li>
<li>Animation Window: Keyframe selection is synced between dopesheet and curve view.</li>
<li>Animation Window: Lock button that locks the selection to currently selected clip and Animator.</li>
<li>Animation Window: Slightly increased the clickable radius for keyframes in the curve editor</li>
<li>Animation Window: When creating new clip from animation window, default to previously used path</li>
<li>BuildPipeline: There will be fewer differences between the exported data files from subsequent builds of your project when using the same version of Unity.  For best results, close Unity and delete your project's Library folder before making an important build.</li>
<li>Curve Editor: Wrap mode enum popup modified to appear as a little gear, which fits nicely in the margin without being cropped.</li>
<li>Documentation: Show "construct type" for class/struct/interface</li>
<li>Editor: Added extensive support for copy/pasting colors: Copy/paste from focused color field, from context menu for color field, from color picker (with no text selected) and from hex field.</li>
<li>Editor: Adding an icon to an EditorWindow title is now exposed by using the GUIContent 'titleContent' property (the old string 'title' is now obsolete)</li>
<li>Editor: Create sprite animation clip from project window context menu.</li>
<li>Editor: Improved grid in Scene View. Eliminates the popping and inconsistent draw distance of the old grid, and also draws grid lines smaller than one unit (10th of a unit, 100th of a unit and so on) when sufficiently zoomed in. New grid shading makes it possible to have grid lines more dense in close parts of the grid without the parts further away being too dense.</li>
<li>Editor: Introduced CreateAssetMenu attribute. Apply it to ScriptableObject-derived types to cause them to show up automatically in the Assets/Create menu.</li>
<li>Editor: Introduced HelpURL attribute, for setting custom documentation URL for user-authored classes.</li>
<li>Editor: Simple expression evaluator for all number fields. Supports + - / * % ( ) operators. This means that all number fields can be used as a calculator.</li>
<li>FrameDebugger: Shader blend, depth and raster states will be shown for draw calls.</li>
<li>GI: Final gather was moved into a separate stage. This allows the indirect baking stage to apply visibility aware upsampling to the indirect lightmap before final gather is applied for better quality.</li>
<li>GI: Reduce the amount of GI related information that is written to the log file</li>
<li>Graphics: Add CommandBuffer.DrawProcedural and DrawProceduralIndirect.</li>
<li>Graphics: Added a way to specify graphics APIs explicitly in player settings (defaults to "automatic" for each platform). For example, you could specify you only want to support Metal+ES2 in iOS builds, or only DX11 (without DX9 fallback) on Windows builds etc. This replaces the "Use DX11" and "Target iOS/GLES Graphics" settings.</li>
<li>Graphics: Added SetPixels32/GetPixels32 to Texture3D.</li>
<li>Graphics: Command Buffers can be set on Lights, see LightEvent enum and Light.AddCommandBuffer.</li>
<li>Graphics: Performance improvements on DX11 when many non-batchable objects are in view.</li>
<li>Importer: Added warning foldout to keep trace of all import warning in the ModelImporter animation tab. </li>
<li>Math: Rect(Vector2, Vector2) constructor overload added</li>
<li>Miscellaneous: Resolution.ToString() implemented</li>
<li>MonoDevelop: Including MonoDoc XML files for showing C# Intellisense tooltips in MonoDevelop</li>
<li>Physics: Add motion constraints to Rigidbody2D</li>
</ul>

#### 
<ul>
<li>Physics: Added HingeJoint BounceMinVelocity. When bounciness is enabled this is the minimum impact velocity which will cause the joint to bounce. Setting this very low, like zero, will cause the joint to never stop bouncing. This can lead to jittering and performance problems. Setting this very high will cause joint to never bounce.</li>
<li>Physics: Optimized performance of ‘OnTriggerStay’ messaging.</li>
<li>Physics: Rigidbodies connected to a HingeJoint will now automatically be woken up when the joint is updated.</li>
<li>Plugin Inspector: You can now select multiple plugins and change compatible platforms. Note - you cannot yet change per platform settings if multiple plugins are selected.</li>
<li>Profiler: Change ms markers in timeline view to use same label style which makes it also properly visible in both skins.</li>
<li>Profiler: Don't show FPS for every ms marker along the x axis in the timeline view - only for the last one.</li>
<li>Profiler: Fix unaligned labels for ms counts in current frame.</li>
<li>Scripting: Added Vector2.Reflect function.</li>
<li>Serialization: Extended SerializedFile size limit to 4GB</li>
<li>Shaders: Support VFACE in surface shader inputs; just use a float variable with VFACE semantic.</li>
<li>SpeedTree: A new importer setting "Animate Cross-fading" is added to SpeedTree assets. With this option on (by default), the dithering LOD transition between mesh/billboard and billboard/culled will be animated by time. This should make the trees look better in most of the scenarios.</li>
<li>SpeedTree: Now wind animation will not be interrupted if the tree gets out side of the view.</li>
<li>SpeedTree: Tree casts shadow when in cross-fading to billboard</li>
<li>Texture2D: Add Texture2D.GetRawTextureData() API</li>
<li>UI: Allow dragging anchors outside of bounds of parent when holding down Ctrl (Cmd on Mac) - the same key that disables snapping. This makes it easier to author screen transitions that support multiple resolutions, since content can be animated to move a distance that's a percentage of the screen width or height.</li>
<li>UI: Changed default blink rate and widget range of InputField caret to match the new frequency behavior.</li>
<li>Version Control: CheckoutIsValid now accept a CheckoutMode</li>
<li>Version Control: Collapse assets and their .meta files in versioning window when they have the same state</li>
<li>WebGL: Made "Explicitly Thrown Exceptions Only" mode much faster and be the default setting</li>
<li>WebGL: Support Input.touches and Input.acceleration</li>
<li>Windows Store Apps: Copy pasting will also work outside the application.</li>
<li>Windows Store Apps: Exposed Rendering path in Player Settings</li>
<li>Windows Store Apps: Refactored App.xaml.cs and MainPage.xaml.cs, it's easier now to add additional XAML pages to the project</li>
<li>XboxOne: Added functions to XboxOnePLM (GetActivationUri, GetActivationTileId, GetActivationArguments) to retrieve cached values.  We still recommend listening to OnActivationEvent in your Start() frame, and processing them that way, but this provides an alternative for last-provided values.</li>
<li>XboxOne: Added support for XMA audio format</li>
<li>XboxOne: IPv6 lookup and DNS support added for C# code.</li>
<li>XboxOne: Lightmap files are now split up per level and put in separate chunks in the package manifest.</li>
<li>XboxOne: More comments have been added to the default package manifest.</li>
<li>XboxOne: Worker threads created by Unity's core systems (Physics, AI) will no longer run on cores 0 and 1, which are reserved for the Rendering thread and Unity's main thread respectively.  This will be a performance gain in most cases by avoiding thread context switches. </li>
</ul>
