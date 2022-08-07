# Unity 2019.1
https://unity3d.com/unity/whats-new/2019.1.0

## Improvements

<ul>
<li><p>2D: Added GridPaintSortingAttribute to allow users to specify the sorting of GameObjects listed in the Active Tilemaps list of the Tile Palette</p></li>
<li><p>Android: Add keystores dedicated location option</p></li>
<li><p>Android: Added <strong>Symlink Sources</strong> in the <strong>Build Settings</strong> window. This enables Java and Kotlin files to be directly referenced from Unity projects in an exported Gradle project.</p></li>
<li><p>Android: Added a check for Vulkan device compatibility on Build and Run</p></li>
<li><p>Android: Added Vulkan renderer compatibility to the Unity video player</p></li>
<li><p>Android: Disabled various Adreno Vulkan driver workarounds for latest drivers</p></li>
<li><p>Android: Enumerated all Android audio input device options, including the lowest-latency option, which can be selected via the name <strong>Android voice recognition input</strong></p></li>
<li><p>Android: Implemented Native Systrace profiling support</p></li>
<li><p>Android: Improved IL2CPP player startup by ~200ms for second and later launches.</p></li>
<li><p>Android: Made the number of worker threads adjust dynamically according to the number of online cores.</p></li>
<li><p>Android: Made the Proguard mapping file save at the same location after building the APK</p></li>
<li><p>Android: More devices can use OpenSL instead of AudioTrack.This reduces audio input and output latency.</p></li>
<li><p>Animation: Added Experimental methods to AnimationPlay.</p></li>
<li><p>Animation: Added property Avatar.humanDescription.</p></li>
<li><p>Animation: Aligned all Animator StateMachine nodes on the grid.</p></li>
<li><p>Animation: Changed default StateMachine node width so that all nodes align vertically.</p></li>
<li><p>Animation: Implemented shift-click and right-click context menu to add properties in animation window without closing popup window.</p></li>
<li><p>Animation: Improved performance for AvatarBuilder.</p></li>
<li><p>Animation: Unity now adds <code>TransformStreamHandle</code> bound to the Transform dynamically at run time. This improves support for animation jobs.</p></li>
<li><p>Animation: Upgraded the animation window preview/playback engine to use the Playable API.</p></li>
<li><p>Asset Import: Added support for cameras in Sketchup Importer.</p></li>
<li><p>Asset Import: Extended the <strong>Optimize Mesh</strong> option on Model Asset import settings, to allow you to independently control optimization of Vertex Order and Polygon Order, rather than using the same flag for both.  NOTE: Performance improvements to the underlying Mesh optimization code might cause Unity to generate vertices in a different order than in previous Unity versions. If you rely on vertex ordering in the optimized Mesh data (such as for vertex painting), be aware that you may need to re-generate this data.</p></li>
<li><p>Asset Import: Improved performance of DXT1/BC1 and DXT5/BC3 Texture compression This does not affect compression quality, but it does probably produce subtly different compression results.</p></li>
<li><p>Asset Pipeline: Scriptable objects that are loaded before a refresh/import, will after a refresh/import be reloaded, if the underlying asset had been modified before the refresh/import. This means that after the refresh/import scriptables objects will have the modified values from modified assets. Before this change, the scriptable object would get "null" value (when using operator==) after the refresh/import.</p></li>
<li><p>Compute: * Added new functionality to allow Unity to use more of the scripting <code>CommandBuffer</code> utility functions with command buffers executed on async compute (such as getting temporary render targets).</p> 
<ul>
<li>Added the concept of execution flags to <code>CommandBuffer</code> to describe how they should execute and allow for better error handling when those command buffers are built in script. This allows for generating exceptions when adding commands not valid for async compute.</li>
<li>Added in-Editor detection for potential GPU deadlock cases where you creates a GPU fence in one command buffer but then never execute that command buffer.</li>
</ul></li>
<li><p>Editor: Added a confirmation prompt when you delete a Shortcut Profile through the Shortcut Manager.</p></li>
<li><p>Editor: Added a keyboard shortcut for the submit button on the changeset submission window, and for some commonly used VCS operations. (1069130)</p></li>
<li><p>Editor: Added Field Of View axis selection drop-down in Camera Inspector.</p></li>
<li><p>Editor: Added <strong>Clear on Build</strong> option in Console.</p></li>
<li><p>Editor: Assembly Definition File inspector: Assembly Definition References, Assembly References and Define Constraints lists are now reorderable when editing a single Assembly Definition File.</p></li>
<li><p>Editor: Improved detecting of Visual Studio for Mac detecting when "Visual Studio.app" filename contains suffixes.</p></li>
<li><p>Editor: Improved performance of the Model Importer Inspector Material remapping section.</p></li>
<li><p>Editor: Improved performance when interacting with Model Inspector with some large Meshes.</p></li>
<li><p>Editor: Improved the performance of the UIElements renderer.</p></li>
<li><p>Editor: Made columns resizable in the Shortcuts Manager Command list.</p></li>
<li><p>Editor: Metal: Added Texture type validation to built-in Metal API validation feature.</p></li>
<li><p>Editor: Moved Camera Easing options to Camera Settings in SceneView from Preferences</p></li>
<li><p>Editor: Reworked Android keystore and key creation UI.</p></li>
<li><p>GI: Added support for shadow mask for rectangular area lights in the progressive lightmappers (available via HDRP).</p></li>
<li><p>GI: Added support for user defined range for area lights.</p></li>
<li><p>GI: Enabled the GPU lightmapper (preview) for macOS and Linux.</p></li>
<li><p>GI: GPU lightmapper now dumps a memory report to Editor.log when it falls back to CPU lightmapper.</p></li>
<li><p>GI: Lightprobe Gizmos are now affected by post-processing.</p></li>
<li><p>GI: Optimized baking of low occupancy lightmaps when using the GPU Lightmapper.</p></li>
<li><p>Graphics: Added filtering for sorting layers to the ScriptableRenderContext.</p></li>
<li><p>Graphics: Added fix to remove stalling on the render thread when loading large Textures.</p></li>
<li><p>Graphics: Added mixed area lights to cull results. This enables mixed rectangular lights in HDRP.</p></li>
<li><p>Graphics: Added Rendering.GraphicsSettings.realtimeDirectRectangularAreaLights to Scriptable Render Pipelines. This provides direct realtime area lighting.</p></li>
<li><p>Graphics: Added SRP hooks for detail rendering Shaders.</p></li>
<li><p>Graphics: Added support for Dynamic Resolution Scaling to the Lightweight Render Pipeline.</p></li>
<li><p>Graphics: Changed the Motion Vector behavior when the exclude motion vector flag is on: 1 - Motion Vector no longer skips nodes that only have Camera Motion
2 - Motion Vector now only skips submeshes with an explicit motion vector pass</p></li>
<li><p>Graphics: Emabled import and skinning of models with up to 32 bone weights for each vertex.</p></li>
<li><p>Graphics: Frame debugger now displays Shader properties for compute Shader dispatches.</p></li>
<li><p>Graphics: GraphicsFences are now available on Vulkan, Metal, D3D11, OpenGL, and OpenGL ES rendering backends.</p></li>
<li><p>Graphics: Made changes so that mesh creation is performed for Terrain details (such as grass) on parallel threads.</p></li>
<li><p>Graphics: Metal/iOS: Fixed Dynamic Resolution render surfaces to use heap allocation with aliasing to improve performance and memory usage.</p></li>
<li><p>Graphics: Metal/macOS: Moved immutable buffers and most Textures from using managed storage into private memory storage, to improve performance and CPU memory utilization.</p></li>
<li><p>Graphics: Metal: Applied a second iteration on the Metal heap allocation management to make it more fine-grained.</p></li>
<li><p>Graphics: Metal: Unity now defers creation of command buffers and render encoders until it actually needs them.</p></li>
<li><p>Graphics: Moved creation of Textures during async load on PC DX11 and Mac Metal off render thread into a job, to minimise problems during load.</p></li>
<li><p>Graphics: Not evaluating the light rectangles for oblique projection matrices</p></li>
<li><p>Graphics: Replaced Shader selection dropdown in Material Asset editor with a searchable drop-down.</p></li>
<li><p>Graphics: Revamped the DrawProcedural script API:</p> 
<ul>
<li>DrawProceduralNow replaces the existing API, because it submits draw calls immediately. The new DrawProcedural API submits calls to color, shadows, reflections etc. This now matches the DrawMesh/DrawMeshNow API.</li>
<li>Added overloads of DrawProcedural that take an Index Buffer</li>
</ul></li>
<li><p>Graphics: Unity now supports Texture Mipmap streaming in Edit Mode when <strong>Texture Streaming</strong> is enabled in the Editor Settings.</p></li>
<li><p>Graphics: Updated the ASTC texture compressor with faster multi-core compression.</p></li>
<li><p>Graphics: <code>Graphics.Blit</code> and <code>CommandBuffer.Blit</code> methods now support blitting to and from Texture arrays.</p></li>
<li><p>IL2CPP: Improve run time performance when script debugging is enabled.</p></li>
<li><p>IL2CPP: Improved the performance of code generated by IL2CPP by up to 20%.</p></li>
<li><p>IL2CPP: Setting IL2CPP compiler config to "Master" will now enable Link Time Optimization on Mac, Android and WebGL</p></li>
<li><p>iOS: Added Access WiFi Capability to the Xcode API (availabe from iOS 12/Xcode 10)</p></li>
<li><p>iOS: Added device generation enums for the 2018 iPad Pro</p></li>
<li><p>iOS: Added launch screen image fields for iPhone XS and XS Max.</p></li>
<li><p>iOS: Added support for the iPhone XS/XS Max (DPI and device detection)</p></li>
<li><p>iOS: Refactored iOS device generation parsing</p></li>
<li><p>Mobile: Added support for RGBM and native HDR lightmaps</p></li>
<li><p>OSX: Made V-sync handling in macOS standalone players more stable.</p></li>
<li><p>Package Manager: <em>Editor.log</em> now logs project load time.</p></li>
<li><p>Package Manager: Added <em>enablePackageManagerTraces</em> command argument functionality, so you can use it to increase the logging level of the UPM process (and increase the verbosity of the upm.log file).</p></li>
<li><p>Package Manager: Introducing scoped registry feature. This empower users to host their own package in a local private registry. This is experimental. The package manager UI was not updated for this feature.</p></li>
<li><p>Package Manager: Released Package Manager UI v2.1.0-preview-1:</p> 
<ul>
<li>Support maximize/minimize</li>
<li>You can now save the PackageManager UI as a maximized window in your Editor layout</li>
<li>Keep track of selected built-in package</li>
<li>Keep track of last selected filter</li>
<li>Fixed UI layout</li>
</ul></li>
<li><p>Package Manager: Removed reference to "package" or "package manager" in the extension manager logs to avoid confusion with the new Package Manager system.</p></li>
<li><p>Package Manager: The Package Manager now displays dependent packages and corresponding assemblies in Object Picker.</p></li>
<li><p>Particles: Added a new mode to the Texture Sheet Animation Module that allows animations to be specific to each mesh a particle is using.</p></li>
<li><p>Particles: Added missing script API for External Forces influencers list.</p></li>
<li><p>Particles: Exposed missing External Forces module properties to script API.</p></li>
<li><p>Particles: Exposed particle mesh indices to script, so you can get and set which mesh each particle is using.</p></li>
<li><p>Particles: Exposed particle mesh indices to shaders, so you know which mesh each particle is using.</p></li>
<li><p>Physics: Added "Collision.contactCount" to retrieve the number of contacts.</p></li>
<li><p>Physics: Added "Collision.GetContact(index)" to retrieve a specific contact.</p></li>
<li><p>Physics: Added "Collision.GetContacts(array)" to retrieve all contacts.</p></li>
<li><p>Physics: Added an <em>Info</em> section to the Rigidbody Inspector view that let's you examine the current velocities, centre of mass and inertia tensor of the Rigidbody.</p></li>
<li><p>Physics: Added an overload of <code>Rigidbody2D.MoveRotation</code> that accepts a Quaternion.</p></li>
<li><p>Physics: OnCollisionEnter, OnCollisionStay &amp; OnCollisionExit no longer create any GC allocations.</p></li>
<li><p>Physics: OnCollisionEnter2D, OnCollisionStay2D &amp; OnCollisionExit2D no longer create any GC allocations.</p></li>
<li><p>Physics: The Inspector <em>Info</em> sections for the Rigidbody2D and Collider2D components now remain expanded when entering and exiting Play mode or moving between components.</p></li>
<li><p>Plugins: Preloading is now supported for any native plug-in. Added PluginImporter.isPreloaded.</p></li>
<li><p>Plugins: When you double-click a plug-in in your Unity project, an associated IDE now opens.</p></li>
<li><p>Prefabs: Added method PrefabUtility.HasPrefabInstanceAnyOverrides to quickly check if there's any override on a Prefab instance.</p></li>
<li><p>Prefabs: Show a "Auto Saving..." badge next to the 'Auto Save' toggle button when saving duration is over 1 second.</p></li>
<li><p>Prefabs: You can now edit the root GameObject of a Prefab directly from the Project browser, without going into Prefab Mode. This supports multi-GameObject editing as well. (<a href="https://issuetracker.unity3d.com/issues/editing-prefabs-directly-in-the-project-browser-is-no-longer-possible">1120805</a>, 1120807)</p></li>
<li><p>Profiler: Added "Semaphore.WaitForSignal" profiler marker.</p></li>
<li><p>Profiler: Added Mono.JIT and Mono.DomainUnload profiler markers.</p></li>
<li><p>Profiler: Added profiler markers for static constructors.</p></li>
<li><p>Profiler: Enabled automatic scripting threads profiling for ILC2PP.</p></li>
<li><p>Profiler: Increased minimum memory usage for profiler to 4MB in Players and 64MB in the Editor.</p></li>
<li><p>Profiler: The Unity Profiler now shows the amount of time until the next frame consistently accross all player platforms, regardless of how V-sync is implemented.</p></li>
<li><p>ps4: Added <code>PS4Input.touchpadMouseSensitivity</code> to provide sensitivity support for touchpad pointer emulation.</p></li>
<li><p>Scripting: Added ability to create <code>NativeArrays</code> of bool and char and <code>types</code> containing bool and char. (1127499, 1129523)</p></li>
<li><p>Scripting: Added support for Visual Studio 2019 code editor.</p></li>
<li><p>Scripting Upgrade: Support C# 7.3 when targeting .NET 4.x Equivalent Scripting Runtime.</p></li>
<li><p>Shaders: Defined <code>UNITY_SEPARATE_TEXTURE_SAMPLER</code> in <code>HlslSupport.cginc</code> for platforms capable of separate texture and sampler objects.</p></li>
<li><p>Shaders: Improve shader debugging. Unity now disables the optimiser when it generates debug shaders (i.e. #pragma enable_d3d11_debug_symbols).</p></li>
<li><p>Shaders: Moved 38 built-in keywords to local keywords. The Shaders inspector now displays global/local keywords by shader.</p></li>
<li><p>Shaders: Shaders can now include files from packages directly like this: #include "Packages/packagename/IncludeFile.cginc"</p></li>
<li><p>Terrain: Added a direction bias to the Terrain smoothing Brush for increasing and decreasing blur.</p></li>
<li><p>Terrain: Added hotkeys to adjust Terrain tool brush size and opacity.</p></li>
<li><p>Terrain: Made changes to allow the setting of <code>shadowCastingMode</code> on Terrain.</p></li>
<li><p>Timeline: Added Volume, Pan and Spatial Blend controls to Audio Tracks, and volume controls to Audio Track Clips.</p></li>
<li><p>Timeline: Improved performance and reduced allocations when playing a Timeline</p></li>
<li><p>Timeline: Made performance improvements to the Timeline Editor Window display.</p></li>
<li><p>UI: Adding ability to modify the ui Dropdowns alpha fade when showing and hiding.</p></li>
<li><p>UI: Adding the ability to to use Sprite Tight mesh inside Unity UI</p></li>
<li><p>UI: Removing option for spritePacking tag in TextureImporter (sprites) when not using the legacy packing mode.</p></li>
<li><p>Universal Windows Platform: Added support for building player with Visual Studio 2019.</p></li>
<li><p>Universal Windows Platform: Added <code>ExecutableOnly</code> build type, which allows you to build without creating a Visual Studio project. This enables quicker iteration when using <strong>Build &amp; Run</strong>. See documentation for <code>UnityEditor.WSAUWPBuildType</code> for more information</p></li>
<li><p>Video: Improved the platform strings documentation for the Set, Get, and ClearTargetSettings methods, in the VideoClipImporter class.</p></li>
<li><p>Web: Added support to write to file in append mode in <code>DownloadHandlerFile</code>.</p></li>
<li><p>Web: UnityWebRequest now reports Content-Length to <code>DownloadHandlerScript</code> as 64-bit. 32-bit method is now deprecated. (<a href="https://issuetracker.unity3d.com/issues/scripting-downloadhandler-dot-receivecontentlength-2gb-integer-overflow">1092447</a>)</p></li>
<li><p>WebGL: Added multi-threading compatibility check.</p></li>
<li><p>WebGL: Added <code>Quit()</code> function support to the Unity instance.</p></li>
<li><p>WebGL: Added <code>UnityLoader.instantiateAsync()</code>, which returns a JavaScript <code>Promise</code>.</p></li>
<li><p>XR: Enable depthBufferSharing by default for Windows Mixed Reality.</p></li>
<li><p>XR: Fixed linear color space on Oculus Go and Quest. For Gear VR, driver issues might prevent linear color space from working with S7 Adreno phones on Android 7.0.</p></li>
<li><p>XR: Fixed wireframe shader in single-pass instancing stereo rendering mode.</p></li>
<li><p>XR: Update Vuforia to version 7.5.20</p></li>
<li><p>XR: Updated Google VR to version 1.18.0.</p></li>
<li><p>XR: Updated Oculus's minimum supported version to 1.28.0.</p></li>
<li><p>XR: Updated Vuforia to version 8.0.10.</p></li>
<li><p>XR: Updated Vuforia to version 8.1.7.</p></li>
<li><p>XR: UpdateVuforia to version 7.5.26</p></li>
<li><p>XR: XR LWRP improvements:</p> 
<ol>
<li>Implemented single-pass double wide rendering as a stereo rendering method fallback for Android devices that do not support single-pass instancing or multi-view.</li>
<li>Made stereo multi-pass rendering unselectable from the Player Settings when an SRP is in use.</li>
<li>Unity now automatically selects Single-Pass stereo rendering if multi-pass was previously selected before using an SRP.</li>
<li>Fixed Android y-flip issues.</li>
<li>Fixed shadow rendering on all Android platforms when using multi-view stereo rendering.</li>
<li>Removed the VR watermark on head-mounted displays.</li>
<li>Removed OpenGL invalid state errors from Android Debug Bridge (ADB) logs.</li>
</ol></li>
</ul>
