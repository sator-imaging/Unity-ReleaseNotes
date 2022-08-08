# Unity 5.3

https://unity3d.com/unity/whats-new/unity-5.3

## Improvement



*   2D: Clamp sprite pivot values (-100k..100k) instead of accepting any value (including infinity), previously clamped from (0..1)
*   Add convenience methods to Dropdown for adding or clearing the options.
*   Added a new property to control the width of the caret in UI.InputField.
*   Added a new property to FontData to control whether horizontal alignment is done by glyph metrics or actual geometry.
*   Added a ReadOnly property to UI.InputField
*   Added buildProgress property to Lightmapping.
*   Android: Optimized Standard Shader performance for OpenGL ES 2.0 devices
*   Android: WWW - report HTTP status and response in case of failure
*   API Updater: Report read only scripts instead of silently failing
*   Asset Loading: Serialisation errors that produce "serialisation layout mismatch" errors will now attempt to include the name of the root type being serialised when the error was encountered.
*   CacheServer: add '--check' and '--fix' command line options for integrity check.
*   Clear script function added to remove all points from a TrailRenderer
*   Core: Added SystemInfo.processorFrequency scripting API.
*   Crunch texture compression: Improve compression quality of normal maps
*   Debug.Assert got new overloads and Debug.LogAssert was added
*   Editor: Add Plane primitive preview option to material preview inspector
*   Editor: Added EditorGUIUtility.GetFlowLayoutedRects.
*   Editor: Added support for locking the inspector to multiple objects.
*   Editor: Components in the inspector with no options will no longer display an expansion arrow.
*   Expose method to Dropdown for refreshing the shown value since it is needed after modifying the list of options through API.
*   Expose the error tolerance on SpringJoint. This allows the springs to have a rest length shorter than the default 2.5 cm.
*   Exposed all particle module parameters to script
*   FrameDebugger: You can now see shader properties when you click on the draw call.
*   GetComponentsInChildren now correctly works if one of the parents of the gameobject being called on is inactive. This makes GetComponentInChildren work on prefabs, and only changes behaviour in cases where previously you were guaranteed to get an empty array as result.
*   GI: Greatly improved precompute performance (and bake as a side effect)! Clustering and light transport stages of the precompute are now considerably faster thanks to the upgrade to Enlighten 3.02. The entire precompute became 1.5-2 times faster. The precompute is currently a part of the bake, so bakes got faster too. ![description](/sites/default/files/5.3.0-relnotes-gi-perf-improvements.png)
    
*   GI: Increase maximum allowed GI cache size.
    
*   GI: Move Atlas Size to Baked GI section in Lighting window.
*   GI: Renamed LightmapSnapshot to LightingDataAsset
*   Graphics: Added Mesh.GetUVs with overloads for List, List, List
*   Graphics: [Ability to render to multiple displays on PC](http://docs.unity3d.com/Manual/MultiDisplay.html).
*   Graphics: CommandBuffer.SetShadowSamplingMode() can be used to enable sampling raw depth value from shadowmaps, to be copied or post-processed by user effects.
*   Graphics: Expose GraphicsSettings class to scripting API.
*   Graphics: Fixed deferred lighting spot light artifacts on mobile (black pixels around edges of objects)
*   Graphics: Fixed OpenGL ES on desktop support: correctly fetch normal and specular maps
*   Graphics: More detailed breakdown of forward rendering pipeline in Profiler.
*   Graphics: Reflection cubemap convolution is GGX now.
*   Graphics: Reflection cubemap convolution preserves HDR highlights better.
*   Graphics: Various dynamic geometry systems (Particles, Sprites, Lines, Trails, Flares, Halos) use multi-threaded "geometry job" system. Yay more multi-threading!
*   Horizontal text alignment now uses the actual glyph geometry extents (rather than character advance) greatly improving the visual appearance of right alignment.
*   Imported fonts now match any other font with the same family name as implicit fallbacks. This allows multiple styles to be used with a single font and the text generator will automatically use the appropriate face.
*   Improved "The referenced script on this Behaviour" message with the game object name in the player, it will look now like 'The referenced script on this Behaviour (Game Object 'Main Camera') is missing!'.
*   Input: Added Input.backButtonLeavesApp, usable on Windows Store Apps/Windows Phone 8.1 and Android, see docs for more info
*   InputField no longer dirties the UI batch for the caret blink cycle when the caret is not visible.
*   Integrated the industry standard for tangent space "mikktspace" into Unity. This allows artists to get seamless lighting since compatibility is ensured between normal map baker and renderer (particular xNormal and several other bakers).
*   iOS: Added frameworks new in iOS 8.0 to 9.0 to the plugin importer UI.
*   iOS: Added support for iPad launch screens
*   MacOSX editor: The graphics API used by the editor is included in the editor title bar just like on Windows
*   Mecanim: Additive Layer improvement. You can now specify the reference pose for your additive animation clip. The additive reference pose can be defined in either the model importer when you import your clip or with a new API function AnimationUtility.SetAdditiveReferencePose()
*   MonoDevelop: Added missing documentation tool-tips for methods with optional/default arguments. Removed markup from documentation tool-tips.
*   MonoDevelop: Updated to version 5.9.6.
*   OpenGL: Fixed threaded rendering on Windows. It was previously disabled as a workaround.
*   OSX Standalone: Set player name to the value of PlayerSettings.ProductName
*   Particles: A percentage of particles can now be rotated in the opposite direction.
*   Particles: Added a warning in the inspector when using a rigidbody with no interpolation and inheritVelocity.
*   Particles: More collision options added, for extra flexibility and more intuitive behaviour
*   Particles: Pivot offset now supports 3D, to move particles back/forwards
*   Particles: Scripted particle emission is now more flexible (See ParticleSystem.Emit)
*   Particles: Simplifying Inherit Velocity UI, to remove duplicated functionality
*   Physics: Added 'OneWayGrouping' property to PlatformEffector2D to group contacts.
*   Physics: All new icons for all 2D physics types.
*   Physics: Always render the outline of a PolygonCollider2D in dark-green so that if an edge is discarded, it still shows.
*   Physics: Decouple centre of mass from inertia tensor. From now on, setting a custom centre of mass won't mark the inertia tensor as set explicitly as well. By analogy, setting inertia tensor won't have an instant effect on the centre of mass. Exposed two new API functions to reset the centre of mass and inertia tensor back to the automatically computed values. See also: Rigidbody.ResetCenterOfMass(),Rigidbody.ResetInertiaTensor(),Rigidbody.centerOfMass, Rigidbody.inertiaTensor, Rigidbody.inertiaTensorRotation.
*   Pointer selection across multiple lines in UI.InputField is improved.
*   Reflection Probes: Ability to turn off deferred reflections when using deferred shading. When "no support" is picked for deferred reflections in Graphics Settings, then in deferred shading reflection probes are done Unity 5.0/5.1 style (per-object).
*   Reflection Probes: blurriness of glossy reflections from Realtime Reflection Probes matches Baked probes better now
*   Scripting: Added CustomYieldInstruction class for implementing custom yield instructions
*   Scripting: Added Matrix4x4.determinant property.
*   Scripting: Added WaitWhile and WaitUntil yield instructions.
*   Select All keyboard command now works for UI.InputField in Editor mode.
*   Shaders: Improved shader storage and loading. This will decrease on-disk size of shaders in player builds, as well as making loading shaders faster and with a smaller memory spike.
*   SpeedTree: Billboard batching performance is improved a bit.
*   Text no longer clips the last line when only the leading would cause it to exceed the vertical bounds.
*   TextGenerator now exposes the topY position of each line in UILineInfo.
*   UI: Add caret color field to InputField as text color isn't always correct
*   UI: Added force update method to InputField to allow instant recalculations
*   UI: CanvasUpdateRegistry no longer checks for a element to be present twice
*   UI: initial pooling of renderers will no longer iterate unnecessary elements
*   UI: TouchInput module is no longer needed. Standalone is the only required module to get both touch and mouse/ keyboard events
*   UI: Updated the max number of submeshes from 5 to 9
*   Universal Windows Apps: Removed APIs from WinRTLegacy which were reintroduced by Microsoft in .NET Core 5.0.
*   WebGL: Compress player's data using LZ4
*   WebGL: Make the path names for all output files configurable in the html
*   WebGL: Release builds will now always use gzip compressed files, and decompress in JavaScript, if the server is not set up to handle gzip on the http protocol level -WebGL: Support soft shadows -WebGL: Higher quality Standard Shader -WebGL: Made it possible to relocate all build output files by changing only the main html output.
*   Windows Store Apps: LocationService will now start the first time it's Start() method is called with user consent being asked at that moment.
*   Windows Store Apps: Unity now will overwrite files in VS solution, if they are not modified. A file UnityOverwrite.txt will be placed next to generated solution file, read it for more details.
*   Windows Store: .NET Native will be disabled when doing Build And Run for Universal Windows 10 Apps, making the run faster
*   Windows Store: Added user friendly message when trying to build to Windows Store Apps SDK 8.1, but SDK 8.1 is missing.