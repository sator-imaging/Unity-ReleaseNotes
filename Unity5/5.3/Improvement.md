# Unity 5.3
https://unity3d.com/unity/whats-new/unity-5.3

## Improvement

<ul>
<li>2D: Clamp sprite pivot values (-100k..100k) instead of accepting any value (including infinity), previously clamped from (0..1)</li>
<li>Add convenience methods to Dropdown for adding or clearing the options.</li>
<li>Added a new property to control the width of the caret in UI.InputField.</li>
<li>Added a new property to FontData to control whether horizontal alignment is done by glyph metrics or actual geometry.</li>
<li>Added a ReadOnly property to UI.InputField</li>
<li>Added buildProgress property to Lightmapping.</li>
<li>Android: Optimized Standard Shader performance for OpenGL ES 2.0 devices</li>
<li>Android: WWW - report HTTP status and response in case of failure</li>
<li>API Updater: Report read only scripts instead of silently failing</li>
<li>Asset Loading: Serialisation errors that produce "serialisation layout mismatch" errors will now attempt to include the name of the root type being serialised when the error was encountered.</li>
<li>CacheServer: add '--check' and '--fix' command line options for integrity check.</li>
<li>Clear script function added to remove all points from a TrailRenderer</li>
<li>Core: Added SystemInfo.processorFrequency scripting API.</li>
<li>Crunch texture compression: Improve compression quality of normal maps</li>
<li>Debug.Assert got new overloads and Debug.LogAssert was added</li>
<li>Editor: Add Plane primitive preview option to material preview inspector</li>
<li>Editor: Added EditorGUIUtility.GetFlowLayoutedRects.</li>
<li>Editor: Added support for locking the inspector to multiple objects.</li>
<li>Editor: Components in the inspector with no options will no longer display an expansion arrow.</li>
<li>Expose method to Dropdown for refreshing the shown value since it is needed after modifying the list of options through API.</li>
<li>Expose the error tolerance on SpringJoint. This allows the springs to have a rest length shorter than the default 2.5 cm.</li>
<li>Exposed all particle module parameters to script</li>
<li>FrameDebugger: You can now see shader properties when you click on the draw call.</li>
<li>GetComponentsInChildren now correctly works if one of the parents of the gameobject being called on is inactive. This makes GetComponentInChildren work on prefabs, and only changes behaviour in cases where previously you were guaranteed to get an empty array as result.</li>
<li><p>GI: Greatly improved precompute performance (and bake as a side effect)! Clustering and light transport stages of the precompute are now considerably faster thanks to the upgrade to Enlighten 3.02. The entire precompute became 1.5-2 times faster. The precompute is currently a part of the bake, so bakes got faster too. <img src="/sites/default/files/5.3.0-relnotes-gi-perf-improvements.png" alt="description"></p></li>
<li><p>GI: Increase maximum allowed GI cache size.</p></li>
<li>GI: Move Atlas Size to Baked GI section in Lighting window.</li>
<li>GI: Renamed LightmapSnapshot to LightingDataAsset</li>
<li>Graphics: Added Mesh.GetUVs with overloads for List, List, List</li>
<li>Graphics: <a href="http://docs.unity3d.com/Manual/MultiDisplay.html">Ability to render to multiple displays on PC</a>.</li>
<li>Graphics: CommandBuffer.SetShadowSamplingMode() can be used to enable sampling raw depth value from shadowmaps, to be copied or post-processed by user effects.</li>
<li>Graphics: Expose GraphicsSettings class to scripting API.</li>
<li>Graphics: Fixed deferred lighting spot light artifacts on mobile (black pixels around edges of objects)</li>
<li>Graphics: Fixed OpenGL ES on desktop support: correctly fetch normal and specular maps</li>
<li>Graphics: More detailed breakdown of forward rendering pipeline in Profiler.</li>
<li>Graphics: Reflection cubemap convolution is GGX now.</li>
<li>Graphics: Reflection cubemap convolution preserves HDR highlights better.</li>
<li>Graphics: Various dynamic geometry systems (Particles, Sprites, Lines, Trails, Flares, Halos) use multi-threaded "geometry job" system. Yay more multi-threading!</li>
<li>Horizontal text alignment now uses the actual glyph geometry extents (rather than character advance) greatly improving the visual appearance of right alignment.</li>
<li>Imported fonts now match any other font with the same family name as implicit fallbacks. This allows multiple styles to be used with a single font and the text generator will automatically use the appropriate face.</li>
<li>Improved "The referenced script on this Behaviour" message with the game object name in the player, it will look now like 'The referenced script on this Behaviour (Game Object 'Main Camera') is missing!'.</li>
<li>Input: Added Input.backButtonLeavesApp, usable on Windows Store Apps/Windows Phone 8.1 and Android, see docs for more info</li>
<li>InputField no longer dirties the UI batch for the caret blink cycle when the caret is not visible.</li>
<li>Integrated the industry standard for tangent space "mikktspace" into Unity. This allows artists to get seamless lighting since compatibility is ensured between normal map baker and renderer (particular xNormal and several other bakers).</li>
<li>iOS: Added frameworks new in iOS 8.0 to 9.0 to the plugin importer UI.</li>
<li>iOS: Added support for iPad launch screens</li>
<li>MacOSX editor: The graphics API used by the editor is included in the editor title bar just like on Windows</li>
<li>Mecanim: Additive Layer improvement. You can now specify the reference pose for your additive animation clip. The additive reference pose can be defined in either the model importer when you import your clip or with a new API function AnimationUtility.SetAdditiveReferencePose()</li>
<li>MonoDevelop: Added missing documentation tool-tips for methods with optional/default arguments. Removed markup from documentation tool-tips.</li>
<li>MonoDevelop: Updated to version 5.9.6.</li>
<li>OpenGL: Fixed threaded rendering on Windows. It was previously disabled as a workaround.</li>
<li>OSX Standalone: Set player name to the value of PlayerSettings.ProductName</li>
<li>Particles: A percentage of particles can now be rotated in the opposite direction.</li>
<li>Particles: Added a warning in the inspector when using a rigidbody with no interpolation and inheritVelocity.</li>
<li>Particles: More collision options added, for extra flexibility and more intuitive behaviour</li>
<li>Particles: Pivot offset now supports 3D, to move particles back/forwards</li>
<li>Particles: Scripted particle emission is now more flexible (See ParticleSystem.Emit)</li>
<li>Particles: Simplifying Inherit Velocity UI, to remove duplicated functionality</li>
<li>Physics: Added 'OneWayGrouping' property to PlatformEffector2D to group contacts.</li>
<li>Physics: All new icons for all 2D physics types.</li>
<li>Physics: Always render the outline of a PolygonCollider2D in dark-green so that if an edge is discarded, it still shows.</li>
<li>Physics: Decouple centre of mass from inertia tensor. From now on, setting a custom centre of mass won't mark the inertia tensor as set explicitly as well. By analogy, setting inertia tensor won't have an instant effect on the centre of mass. Exposed two new API functions to reset the centre of mass and inertia tensor back to the automatically computed values. See also: Rigidbody.ResetCenterOfMass(),Rigidbody.ResetInertiaTensor(),Rigidbody.centerOfMass, Rigidbody.inertiaTensor, Rigidbody.inertiaTensorRotation.</li>
<li>Pointer selection across multiple lines in UI.InputField is improved.</li>
<li>Reflection Probes: Ability to turn off deferred reflections when using deferred shading. When "no support" is picked for deferred reflections in Graphics Settings, then in deferred shading reflection probes are done Unity 5.0/5.1 style (per-object).</li>
<li>Reflection Probes: blurriness of glossy reflections from Realtime Reflection Probes matches Baked probes better now</li>
<li>Scripting: Added CustomYieldInstruction class for implementing custom yield instructions</li>
<li>Scripting: Added Matrix4x4.determinant property.</li>
<li>Scripting: Added WaitWhile and WaitUntil yield instructions.</li>
<li>Select All keyboard command now works for UI.InputField in Editor mode.</li>
<li>Shaders: Improved shader storage and loading. This will decrease on-disk size of shaders in player builds, as well as making loading shaders faster and with a smaller memory spike.</li>
<li>SpeedTree: Billboard batching performance is improved a bit.</li>
<li>Text no longer clips the last line when only the leading would cause it to exceed the vertical bounds.</li>
<li>TextGenerator now exposes the topY position of each line in UILineInfo.</li>
<li>UI: Add caret color field to InputField as text color isn't always correct</li>
<li>UI: Added force update method to InputField to allow instant recalculations</li>
<li>UI: CanvasUpdateRegistry no longer checks for a element to be present twice</li>
<li>UI: initial pooling of renderers will no longer iterate unnecessary elements</li>
<li>UI: TouchInput module is no longer needed. Standalone is the only required module to get both touch and mouse/ keyboard events</li>
<li>UI: Updated the max number of submeshes from 5 to 9</li>
<li>Universal Windows Apps: Removed APIs from WinRTLegacy which were reintroduced by Microsoft in .NET Core 5.0.</li>
<li>WebGL: Compress player's data using LZ4</li>
<li>WebGL: Make the path names for all output files configurable in the html</li>
<li>WebGL: Release builds will now always use gzip compressed files, and decompress in JavaScript, if the server is not set up to handle gzip on the http protocol level -WebGL: Support soft shadows
-WebGL: Higher quality Standard Shader
-WebGL: Made it possible to relocate all build output files by changing only the main html output.</li>
<li>Windows Store Apps: LocationService will now start the first time it's Start() method is called with user consent being asked at that moment.</li>
<li>Windows Store Apps: Unity now will overwrite files in VS solution, if they are not modified. A file UnityOverwrite.txt will be placed next to generated solution file, read it for more details.</li>
<li>Windows Store: .NET Native will be disabled when doing Build And Run for Universal Windows 10 Apps, making the run faster</li>
<li>Windows Store: Added user friendly message when trying to build to Windows Store Apps SDK 8.1, but SDK 8.1 is missing.</li>
</ul>
